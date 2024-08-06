---
title: how to use rclone to sync remote drives
publish: "true"
timestamp: 2024-08-05 17:53
---
there are a number of ways to synchronize and backup data across different cloud services or from a local machine to a cloud storage drive. [rclone](https://rclone.org/) is one solution that is pretty easy to setup and only requires one line of code to synch data in two different places. 

## setup
first, make sure rclone is installed on your device. 

on mac you can install using [homebrew](https://brew.sh/)
```
$ brew install rclone
```

see [these instructions](https://rclone.org/install/) for other operating systems

then you will need to configure rclone to have access to any of your remote drives. there are detailed instructions on how to do that for many, many different options [here](https://rclone.org/docs/#configure). The steps involve using the APIs and essentially generating a key and password so rclone can safely transfer data.

[google drive configuration](https://rclone.org/drive/)
[google cloud configuration](https://rclone.org/googlecloudstorage/)
[dropbox configuration](https://rclone.org/dropbox/)

the above steps will walk you through setting up access through the interactive configuration in your terminal:
```
$ rclone config
```

i currently have two drives set up:
```
$ rclone config
Current remotes:

Name                 Type
====                 ====
dropbox              dropbox
gdrive               drive
```

## usage
i can easily sync my data from my local machine to one either dropbox or google drive. or I can sync between dropbox and google drive. 

for example, these notes are currently in a folder on dropbox (so that I can open the vault on any computer) but I would like to have a backup on google drive just in case. to do this, I just run the following line of code:
```
$ rclone sync dropbox:notes gdrive:backups/notes -v -P
```
I use the rclone sync command then specify the source which is the dropbox i configured earlier. then i specify the folder in the dropbox called "notes". I then specify the destination which is the other remote I configured earlier called gdrive. and I specify the folder destination I would like it to sync to which is the notes folder within backups. the `-v` option says I want verbose mode which just increases the information that is read out during the syncing. the `-P` option says that I want a progress bar to be displayed. You can also use the `--dry-run` option to test things out before actually copying any files or changing anything. 


#🥚 
## references
---
rclone documentation