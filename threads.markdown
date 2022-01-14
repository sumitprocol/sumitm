---
layout: page
title: Threads
permalink: /threads/
order: 4
---


{%- if site.posts.size > 0 -%}
    <ul class="post-list">
      {%- for post in site.posts -%}
      {% if post.categories contains "threads" %}
      <li>
        {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
        <span class="post-meta">{{ post.date | date: date_format }}</span>
        <h3>
          <a class="post-link" href="{{ post.url | relative_url }}">
            {{ post.title | escape }}
          </a>
        </h3>
        {%- if site.show_excerpts -%}
          {{ post.excerpt }}
        {%- endif -%}
      </li>
      {% endif %}
      {%- endfor -%}
    </ul>
{%- endif -%}