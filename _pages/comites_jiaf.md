---
layout: page_jiaf
show_meta: false
permalink: jiaf/comites
title: Comités
published: true
---

{% for comite in site.data.comites_jiaf %}
## Comité {{ comite.type }}

### Présidence
{% assign thecomite = comite.presidence %}
{% include _list_members.md %}

### Autre Membres
{% assign thecomite = comite.autre %}
{% include _list_members.md %}

{% endfor %}
