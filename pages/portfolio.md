---
layout: default
title: Portfolio Work
permalink: /portfolio/
published: true
---

<h1>Portfolio Work</h1>

<h2>Writing</h2>

<ul>
  {% for post in site.portfolio %}
    <li>
      <b><a href="{{ post.url }}">{{ post.title }}</a></b>
      <p>{{ post.excerpt }}</p>
    </li>
  {% endfor %}
</ul>