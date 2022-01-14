---
layout: page
title: Collections
permalink: /collections/
---

<ul>
  {% for post in site.posts %}
  {% if post.categories contains "collections" %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      {{ post.excerpt }}
    </li>
  {% endif %}
  {% endfor %}
</ul>