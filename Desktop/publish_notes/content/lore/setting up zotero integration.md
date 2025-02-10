---
title: setting up zotero integration
publish: "true"
timestamp: 2024-07-05 17:31
---
zotero integration is what I use to import my zotero notes and papers to obsidian. 

First, zotero must be downloaded onto the computer. For mac and windows, this is pretty straightforward just download from the zotero download site. for linux, you can download from this [repo](https://github.com/retorquere/zotero-deb) and it will update whenever you update the computer. 

then you need to download better bibtex as an add on to zotero. you can [follow the instructions here](https://retorque.re/zotero-better-bibtex/installation/index.html)

I like to set my citation key to a custom format so it is the first author et al and the year. To change this, go into the better bibtex settings in zotero and change the citation key format. I use:

```
authEtal2+year
```

then I select all of the papers in my zotero library, right click, then in the better bibtex dropdown select refresh citation key and this will update them all. 