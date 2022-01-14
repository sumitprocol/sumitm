---
layout: page
title: Books
permalink: /books/
---


<ul>
  {% for post in site.posts %}
  {% if post.categories contains "books" %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      {{ post.excerpt }}
    </li>
  {% endif %}
  {% endfor %}
</ul>