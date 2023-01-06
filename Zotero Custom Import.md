---
title: "{{title}}"
authors: [{{authors}}]
tags: [{{allTags}}]
year: {{date | format("YYYY")}}
url: {{url}}
DOI: {{DOI}}
Journal: {{publicationTitle}}
---

- Zotero Link : {{pdfZoteroLink}}

## Abstract

{{abstractNote}}

## Annotations

{% for annotation in annotations %}
{%- if annotation.annotatedText %}
{%- if annotation.comment %}
````ad-cite
title:{{citekey}} [(go to citation)](zotero://open-pdf/library/items/{{annotation.attachment.itemKey}}?page={{annotation.page}}&annotation={{annotation.id}})
{{annotation.annotatedText}}
```ad-info
title: Comment
{{annotation.comment}}
```
````
{%- else %}
```ad-cite
title:{{citekey}} [(go to citation)](zotero://open-pdf/library/items/{{annotation.attachment.itemKey}}?page={{annotation.page}}&annotation={{annotation.id}})
{{annotation.annotatedText}}
```
{%- endif %}
{%- elif annotation.imageRelativePath %}
![[{{annotation.imageRelativePath}}]]
[Go to annotation](zotero://open-pdf/library/items/{{annotation.attachment.itemKey}}?page={{annotation.page}}&annotation={{annotation.id}})
{%- if annotation.comment  %}
```ad-info
title: Comment
{{annotation.comment}}
```
{%- endif %}
{%- else %}
```ad-info
title: Comment [(Go to Comment)](zotero://open-pdf/library/items/{{annotation.attachment.itemKey}}?page={{annotation.page}}&annotation={{annotation.id}})
{{annotation.comment}}
```
{%- endif %}
{% endfor -%}
