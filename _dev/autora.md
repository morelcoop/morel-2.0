---
layout: page
title: Obras por autora
---
<div>
{% for author in site.authors %}
  <div>
    <h2>{{ author.title }}</h2>
    {% for book in site.books %}
      {% if book.author == author.title or book.author2 == author.title  or book.author3 == author.title %}
    <div>
      <h4><a class="morel" href="{{ site.baseurl }}{{ book.url }}">{{book.title}}</a></h4>
    </div>
      {% endif %}
    {% endfor %}
  </div>
{% endfor %}
</div>