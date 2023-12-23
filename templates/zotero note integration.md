---
type: literature-note
alias: {{title | safe}}
---

---

| |
|------------ | ------------|
| Title | {{title}} |
| Authors | {{authors}} |
| Publication | {{publicationTitle}} |
| Zotero link | {{pdfZoteroLink}} |
| Web link | {{url}} |

### Citation

{{bibliography}}

{% if abstractNote %}

### Abstract
{{abstractNote}}

{% endif %}

---

### Annotations

##### Exported: {{exportDate | format("YYYY-MM-DD h:mm a")}}

{% for annotation in annotations %}
{% if annotation.annotatedText %}
> <mark style="background-color: {{annotation.color}};color: black">Highlight</mark> 
> {{annotation.annotatedText}}
> [Page {{annotation.page}}](zotero://open-pdf/library/items/{{annotation.attachment.itemKey}}?page={{annotation.page}})
{% endif %}
{% if annotation.comment %}
> <mark style="background-color: {{annotation.color}};color: black">Comment</mark>
> {{annotation.comment}}
> [Page {{annotation.page}}](zotero://open-pdf/library/items/{{annotation.attachment.itemKey}}?page={{annotation.page}})
{% endif %}
{% if annotation.imageRelativePath %}
![{{annotation.imageRelativePath}}]({{annotation.imageRelativePath}})
{% endif %}
{% endfor %}

---

{% persist "notes" %}

### Take-aways

-  

### Related

- 

{% endpersist %}