---
layout: default
title: SFPC Blog (2016)
permalink: /sfpc-blog-index/
---

# School for Poetic Computation Blog (2016)

In fall 2016, I attended the School for Poetic Computation, an experimental school in New York City focused on the intersection of art, code, hardware, and critical theory.

At the time, SFPC felt like a small, intense, artist-run school/residency: part classroom, part studio, part research group. We studied creative coding, computation, electronics, networks, critical theory, and the politics of technology while making projects together.

SFPC still exists today, though it has changed significantly since I attended. The current school describes itself as an experimental school in New York and online, founded in 2013, with programs grounded in art, code, hardware, critical theory, decolonization, and transformative justice. It is now led by a different group of organizers and co-directors than the one I studied with in 2016.

This archive is just my personal blog from that 2016 session.

*I blogged every day for 10 weeks while at the [School for Poetic Computation](https://sfpc.io/) in 2016.*

---

{% for post in site.sfpc-blog %}
- [{{ post.title }}]({{ post.url }})
{% endfor %}

{% include post_navigation.html %}
