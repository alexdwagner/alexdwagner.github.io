---
layout: default
title: Blog
permalink: /blog/
---

<h1>Blog</h1>

<ul>
  {% for post in site.blog %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      <p>{{ post.excerpt }}</p>
    </li>
  {% endfor %}
</ul>
