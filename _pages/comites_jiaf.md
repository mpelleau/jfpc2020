---
layout: page
show_meta: false
permalink: jiaf/comites/
title: Comités
published: true
conference: jiaf
---

{% for comite in site.data.comites_jiaf %}
## Comité {{ comite.type }}

### Présidence
{% include list_members members = comite.presidence %}

### Autre Membres
{% include list_members members = comite.autre %}

{% endfor %}
