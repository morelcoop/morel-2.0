---
layout: page
---
{% for author in site.authors %}
{% assign nacimiento = author.date-born | date: "%d %m" %}
<h1>{{ nacimiento }}</h1>
<p>{{ author.title }}</p>
{% endfor %}