---
layout: default
title: SFPC Blog (2016)
permalink: /sfpc-blog-index/
---

# School for Poetic Computation Blog (2016)

*I blogged every day for 10 weeks while at the [School for Poetic Computation](https://sfpc.io/) in 2016.*

---

{% for post in site.sfpc-blog %}
- [{{ post.title }}]({{ post.url }})
{% endfor %}

{% include post_navigation.html %}
