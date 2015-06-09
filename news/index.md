---
layout: default
title: "Project news"
---

{% for doc in site.categories.news %}
**{{ doc.title | xml_escape }}** ({{ doc.author }}, [{{ doc.date | date: "%d %b %Y" }}]({{ doc.url }}))

{{ doc.content }}
<hr>

{% endfor %}

