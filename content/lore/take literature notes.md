---
title: take literature notes
publish: "true"
timestamp: 2023-12-11 09:36
tags:
  - 🐛
---
literature notes are the homepage for papers I take notes on in my vault. I like to keep citation info, the doi link, the abstract, and various other metadata about the paper when I import it from zotero. I can then make modular notes as i go

see #📚 for examples
## zotero integration
this obsidian plugin imports information from papers saved in my zotero library. it will import annotations and images if I take them in the pdf viewer of zotero
- to import highlights, just use the highlight tool
- to import images, use the rectangle selection tool and draw around the plot
	- images are saved to `/attachments/{{citekey}}_image_location.png` in my obsidian vault

see my zotero import template at the bottom of this page!
## fleeting notes
the fleeting notes section is a place to jot down any thoughts or notes while reading just to help process information. Anything written in this section will persist even if the paper is imported again to refresh highlights or images pulled into obsidian. 
this is a good place to start formulating modular notes 


#🐛  | [[⨳ how to]] | [[how I read academic papers]]


---
## zotero import template file
```
---
paper_title: "{{title}}"
year: '{{date | format("YYYY")}}'
authors: "{{authors}}"
type: literature note
note date: '{{exportDate | format ("YYYY-MM-DD")}}'
modified: 
summary: 
tags:
  - 📚
status:
---

# {{title}}
**authors**: *{{authors}}*
**doi**: {{DOI}}

> [!INFO] CITATION
> {{bibliography}}

> [!NOTE] ABSTRACT
> {%- if abstractNote %}
> {{abstractNote}} {% else %} {{summaryNote}}
> {%- endif %} 

## fleeting notes
---
{% persist  "notes"%} 


{% endpersist %} 
## highlights
---
{% for annotation in annotations -%} 
    {%- if annotation.annotatedText -%} 
    "=={{annotation.annotatedText}}==”[Page {{annotation.page}}](zotero://open-pdf/library/items/{{annotation.attachment.itemKey}}?page={{annotation.page}}&annotation={{annotation.id}}) 
    {%- endif %} 
    {%- if annotation.imageRelativePath -%}
    ![[{{annotation.imageRelativePath}}]][Page {{annotation.page}}](zotero://open-pdf/library/items/{{annotation.attachment.itemKey}}?page={{annotation.page}}&annotation={{annotation.id}}) 
    {%- endif %} 

{% if annotation.comment %} 
{{annotation.comment}} 
{% endif %} 
{% endfor -%}
```