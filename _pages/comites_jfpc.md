---
layout: page
show_meta: false
permalink: jfpc/comites
title: Comités
published: true
conference: jfpc
---

{% for comite in site.data.comites_jfpc %}
## Comité {{ comite.type }}

### Présidence
{% include list_members members = comite.presidence %}

### Autre Membres
{% include list_members members = comite.autre %}

{% endfor %}
