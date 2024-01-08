---
aliases:
  - "{{title}}"
authors: [{{authors}}]
DOI: {{DOI}}
Journal: {{publicationTitle}}
tags:
  - {{allTags}}
title: "{{citekey}}"
url: {{url}}
year: {{date | format("YYYY")}}
---

- Zotero Link : {{pdfZoteroLink}}

## Abstract

{{abstractNote}}

## Annotations

{% for annotation in annotations %}
{%- if annotation.annotatedText %}
{%- if annotation.comment %}

> [!cite] {{citekey}} [(go to citation)](zotero://open-pdf/library/items/{{annotation.attachment.itemKey}}?page={{annotation.page}}&annotation={{annotation.id}})
> {{annotation.annotatedText}}
>
> > [!info] Comment
> > {{annotation.comment}}

{%- else %}

> [!cite] {{citekey}} [(go to citation)](zotero://open-pdf/library/items/{{annotation.attachment.itemKey}}?page={{annotation.page}}&annotation={{annotation.id}})
> {{annotation.annotatedText}}

{%- endif %}
{%- elif annotation.imageRelativePath %}
![[{{annotation.imageRelativePath}}]]
[Go to annotation](zotero://open-pdf/library/items/{{annotation.attachment.itemKey}}?page={{annotation.page}}&annotation={{annotation.id}})
{%- if annotation.comment  %}

> [!info] Comment
> {{annotation.comment}}

{%- endif %}
{%- else %}

> > [!info] Comment [(Go to Comment)](zotero://open-pdf/library/items/{{annotation.attachment.itemKey}}?page={{annotation.page}}&annotation={{annotation.id}})
> > {{annotation.comment}}

{%- endif %}
{% endfor -%}
