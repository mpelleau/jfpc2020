---
layout: page
show_meta: false
permalink: sponsors/
title: Sponsors
published: true
---

{% for sponsor in site.data.sponsors -%}
    [![{{ sponsor.name }}]({{ site.url }}{{ site.baseurl }}/images/sponsor/{{ sponsor.img }}){: class="sponsor-img small"}]({{ sponsor.website }}){: target="_blank"}
{% endfor %}