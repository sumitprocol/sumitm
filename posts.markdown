---
layout: page
title: Posts
permalink: /posts/
---

<ul>
  {% for post in site.posts %}
  {% if post.categories contains "blogs" %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      {{ post.excerpt }}
    </li>
  {% endif %}
  {% endfor %}
</ul>