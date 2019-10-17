---
layout: page_jiaf
show_meta: false
permalink: jiaf/soumission
title: Soumission
published: true
---

Modalités pour la soumission d'articles

# Dates importantes

{% for date in site.data.dates_jiaf %}
  - {{ date.title }} {% if date.info -%} <span style="font-size:0.75em;">{{ date.info }} </span>{% endif -%} : {{ date.date }}
{% endfor %}
