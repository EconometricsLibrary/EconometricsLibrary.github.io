---
layout: entitled
title: "EFLP News"
---

{% for doc in site.posts %}
**{{ doc.title | xml_escape }}** ({{ doc.author }}, [{{ doc.date | date: "%d %b %Y" }}]({{ doc.url }}))

{{ doc.content }}
<hr>

{% endfor %}

