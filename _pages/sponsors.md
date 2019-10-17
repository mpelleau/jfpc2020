---
layout: page
show_meta: false
permalink: /sponsors
title: Sponsors
published: true
---

{% for sponsor in site.data.sponsors -%}
    ![{{ sponsor.name }}](/images/sponsor/{{ sponsor.img }}){: style="max-width: 20%;height: auto !important;"}
{% endfor %}