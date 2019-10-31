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
  {%- if membre.website %} 
  - [{{ membre.name }}]({{ membre.website }}) ({{ membre.institution }})
  {%- else %} 
  - {{ membre.name }} ({{ membre.institution }}) 
  {%- endif -%}
{%- endfor %}

### Autre Membres
{% for membre in comite.autre %}
  {%- if membre.website %} 
  - [{{ membre.name }}]({{ membre.website }}) ({{ membre.institution }})
  {%- else %} 
  - {{ membre.name }} ({{ membre.institution }}) 
  {%- endif -%}
{% endfor %}
{% endfor -%}
