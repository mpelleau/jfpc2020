---
layout: page_jfpc
show_meta: false
permalink: jfpc/comites
title: Comités
published: true
---

{% for comite in site.data.comites_jfpc %}
## Comité {{ comite.type }}

### Présidence
{% assign thecomite = comite.presidence %}
{% include _list_members.md %}

### Autre Membres
{% assign thecomite = comite.autre %}
{% include _list_members.md %}

{% endfor %}
