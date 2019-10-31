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
{% for membre in comite.presidence -%}
  {%- if membre.website %} 
  - [{{ membre.name }}]({{ membre.website }}) ({{ membre.institution }})
  {%- else %} 
  - {{ membre.name }} ({{ membre.institution }}) 
  {%- endif -%}
{% endfor %}

### Autre Membres
{% for membre in comite.autre -%}
  {%- if membre.website %} 
  - [{{ membre.name }}]({{ membre.website }}) ({{ membre.institution }})
  {%- else %} 
  - {{ membre.name }} ({{ membre.institution }}) 
  {%- endif -%}
{% endfor %}
{% endfor -%}
