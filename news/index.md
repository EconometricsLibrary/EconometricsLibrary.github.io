---
layout: default
title: "EFLP News"
---

{% for doc in site.categories.blog %}
**{{ doc.title | xml_escape }}** ({{ doc.author }}, [{{ doc.date | date: "%d %b %Y" }}]({{ doc.url }}))

{{ doc.content }}
<hr>

{% endfor %}

