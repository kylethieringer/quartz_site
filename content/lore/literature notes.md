---
cssclasses:
  - dashboard
title: literature notes
publish: "true"
timestamp: 2023-12-11 01:12
tags:
  - 📚
---
this page contains a dataview table of my literature notes. if viewing online version of [mimir](notes.kylethieringer.com), you will not be able to see the results of the following code block... sorry

click on the 📚 tag for a list of papers I have published notes about for the next best thing!

```dataview

TABLE authors, paper_title, summary, status
FROM "lore"
where type = "literature note"
SORT file.name
```
