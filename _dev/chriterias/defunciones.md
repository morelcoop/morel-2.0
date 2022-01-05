---
layout: page
---
{% for author in site.authors %}
{% assign muerte = author.date-death | date: "%d %m" %}
<h1>{{ muerte }}</h1>
<p>{{ author.title }}</p>
{% endfor %}