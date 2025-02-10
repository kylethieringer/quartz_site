---
title: how I made this site
tags:
  - 🐛
publish: "true"
---
## obsidian backbone
this site is built on top of [obsidian](https://www.obsidian.md). at its core, its just a wrapper for markdown files that allows for the incredibly useful backlinking (links to other notes within notes). markdown files are nice because they are simple text files that can be read by any computer with any basic text editor. While obsidian is not open source, the markdown files are all stored locally so we dont run into proprietary issues with note taking systems like evernote, google docs, microsoft word, etc. if obsidian dissolves as a company, we still own our files and can easily port them over to another markdown based system like [logseq](https://logseq.com/) 

I have my obsidian vault saved in my iCloud drive so I can access it on any mac computer I use or on my iphone. (I cant quite justify the paid obsidian sync feature right now)

## website deployment
something I decided to do but is not necessary for creating a website is to buy a domain name. I decided to buy www.kylethieringer.com through [squarespace](www.squarespace.com) because it was only $12-20 / year and offered me a few more options with regards to the experience of using the site.

obsidian offers a publish feature but this too is a paid subscription. I decided against publishing through obsidian for a few reasons. The biggest barrier was the price--more than I wanted to spend. The next was a security/privacy reason. I didn't want to host the notes on obsidian's servers, mostly because I wanted full autonomy over these notes. The final reason was that obsidian publish was not super flexible with what I can choose to publish vs not publish. I have a lot of personal notes, notes in progress, or notes containing info that should not be published to the interwebs. with all of these considerations, I needed to find another option!

One extremely common and relatively simple method of creating a basic static website is [github pages](https://pages.github.com/) (plus its free). in order to deploy this obsidian vault as something that can be navigated on the internet, the markdown files need to be converted to html files, plus some additional styling to make everything look nice. Luckily, there is an incredible project that has made this process effortless, called [quartz](https://quartz.jzhao.xyz/). 

the documentation is fantastic, getting things up and running was fast, plus the discord community is super friendly and helpful. [[connecting a github pages site to a custom domain]] was the only tricky part. I wanted the fancy https://notes.kylethieringer.com subdomain for my notes rather than kylethieringer.com/notes (purely for aesthetics lol). 

## obsidian vault organization
in my vault, I have a couple of folders but I try to minimize any sort of hierarchy as much as possible. 
- `/attachments` folder is where all of the non `.md` files are saved
- `/lore` is where all of my public notes are stored
- `/private` is where all of my daily notes, or other private notes are kept. this folder is included in the `.gitignore` file so none of them are pushed to the github repository that hosts the site
- `/tags` is only used to make descriptions for the tags pages online
- `/templates` contains my template files (also not pushed to github)

quartz takes advantage of the frontmatter in all of my notes. Each note needs: 
- `title:` what to call the note 
- `tags:` which tags to associate the note with
- `publish:` whether to actually publish the note online or not 

the only tags I have in my notes right now are emoji tags (see [[metamorphosis of a note]]). everything else is connected to each other through backlinks. 



#🐛  | [[⨳ how to]]
## references
---
https://quartz.jzhao.xyz/
https://github.com/alshedivat/al-folio