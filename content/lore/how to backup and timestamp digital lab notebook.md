---
title: how to backup and timestamp digital lab notebook
publish: "true"
timestamp: 2024-08-13 12:10
---
digital files are note immutable. here is how I am backing up my lab notebook and also making sure edit history is tracked. this is to maintain integrity and honesty in the work I am doing and make sure there is always a backup of my files. 

I backup and push to github once a week. but this is subject to change! usually I try to sync often, whenever I remember to. 
## make a local backup folder
I keep my lab notebook in dropbox so i can access it on any computer I want, without paying for obsidian sync. I think the sync feature may be useful in the future because obsidian sometimes doesnt play well with dropbox... Because of this, i dont want to add additional complexity, because sometimes github and dropbox dont play well together either. So i sync to a local folder and this serves another purpose of creating a local backup in case dropbox and github decide to lock you out of your notes.

I use rclone to sync all changes in my dropbox vault to my local copy folder. this just takes one line of code!
rclone sync is nice because it preserves file modification times and also will update changes to files that have been modified not just look if the file exists or not. 

```
$ rclone sync dropbox:notes ~/repos/labbook_backup/notes
```

see [[how to use rclone to sync remote drives]] for more information about rclone, and setting it up
## setup github repo
I then create a github repo outside of the obsidian vault folder. for example, my folder hierarchy:
```
├── labbook_backup     (local folder)    
│	└── notes          (obsidian vault)
│	     └── ...
│	└── .git
│
```

if you dont have a github repo already setup make sure to create a repository on the github website. then in the terminal use: 
```
git init
git add .
git commit -m "today's date"
git branch -M main
git remote add origin https://github.com/your_reposotory.git
git push -u origin main
```

If you already have a githup repo setup, then to add your vault changes to the repository all you need to do is :
```
git add .
git commit -m "today's date"
git push
```

## my weekly routine
it takes a minute, you just have to remember to do it!

```
$ rclone sync dropbox:notes ~/repos/labbook_backup/notes
$ cd ~/repos/labbook_backup
$ git add .
$ git commit -m "today's date"
$ git push
```


#🥚 [[⨳ how to]] | [[how I keep a digital lab notebook]]