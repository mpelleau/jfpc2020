---
layout: page
show_meta: false
permalink: /agenda
title: Programme
published: true
---

Le programme détaillé pour les JFPC se trouve [ici]({{ site.baseurl }}/jfpc/programme), et celui pour les JIAF est [ici]({{ site.baseurl }}/jiaf/programme)

## Dates importantes

### Pour les JFPC
{% for date in site.data.dates_jfpc -%}
  - {{ date.title }} {% if date.info -%} <span style="font-size:0.75em;">{{ date.info }} </span>{% endif -%} : {{ date.date }}
{% endfor %}

### Pour les JIAF
{% for date in site.data.dates_jiaf -%}
  - {{ date.title }} {% if date.info -%} <span style="font-size:0.75em;">{{ date.info }} </span>{% endif -%} : {{ date.date }}
{% endfor %}