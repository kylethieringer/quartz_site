---
paper_title: "{{title}}"
year: '{{date | format("YYYY")}}'
authors: "{{authors}}"
type: literature note
note date: '{{exportDate | format ("YYYY-MM-DD")}}'
modified: 
summary: 
tags: []
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


#📚 