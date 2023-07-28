---
layout: default
title: My Portfolio
permalink: /portfolio/
published: false
---

<!-- 
    07/28/2023 -
    trying to create a sortable spreadsheet of all professional writing work
    rn, content is not displaying. like the md files don't populate the page at all
 -->

<script>
function filterContent(category) {
    const items = document.querySelectorAll('.portfolio-item');
    items.forEach(item => {
        if (category === 'all' || item.classList.contains(category)) {
            item.style.display = 'block';
        } else {
            item.style.display = 'none';
        }
    });
}
</script>

<!-- Buttons to sort the content -->
<div class="portfolio-buttons">
    <button onclick="filterContent('all')">All</button>
    <button onclick="filterContent('content_writing')">Content Writing</button>
    <button onclick="filterContent('technical_writing')">Technical Writing</button>
    <button onclick="filterContent('content_strategy')">Content Strategy</button>
</div>

<div id="portfolio-list">
    {% for item in site.content_writing %}
    <div class="portfolio-item content_writing">
        <a href="{{ item.url }}">{{ item.title }}</a>
    </div>
    {% endfor %}

    {% for item in site.technical_writing %}
    <div class="portfolio-item technical_writing">
        <a href="{{ item.url }}">{{ item.title }}</a>
    </div>
    {% endfor %}

    {% for item in site.content_strategy %}
    <div class="portfolio-item content_strategy">
        <a href="{{ item.url }}">{{ item.title }}</a>
    </div>
    {% endfor %}
</div>
