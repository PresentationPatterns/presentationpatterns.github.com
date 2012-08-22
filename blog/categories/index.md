---
layout: fullNav
title: Blog Post Categories
tagline: The Blog Posts By Category
---
{% include JB/setup %}

<article>

<h2>Categories</h2>
<ul>
  {% assign categories_list = site.categories %}
  {% include JB/categories_list %}
</ul>

<hr>

{% for category in site.categories %} 
  <h2 id="{{ category[0] }}-ref">{{ category[0] | join: "/" }}</h2>
  <ul>
    {% assign pages_list = category[1] %}  
    {% include JB/pages_list %}
  </ul>
{% endfor %}
</article>
