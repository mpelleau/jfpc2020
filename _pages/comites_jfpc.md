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
{% for membre in comite.presidence -%}
  - [{{ membre.name }}]({{ membre.website }}) ({{ membre.institution }})
{% endfor %}

### Autre Membres
{% for membre in comite.autre -%}
  - [{{ membre.name }}]({{ membre.website }}) ({{ membre.institution }})
{% endfor %}
{% endfor -%}
