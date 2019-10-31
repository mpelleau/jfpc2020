---
layout: page
show_meta: false
permalink: /team
title: Comités
published: true
---

## JFPC

{% for comite in site.data.comites_jfpc %}
### Comité {{ comite.type }}

{% for membre in comite.presidence -%}
  {%- if membre.website %} 
  - [{{ membre.name }}]({{ membre.website }}) ({{ membre.institution }})
  {%- else %} 
  - {{ membre.name }} ({{ membre.institution }}) 
  {%- endif -%}
{% endfor %}
{% endfor %}


## JIAF

{% for comite in site.data.comites_jiaf %}
### Comité {{ comite.type }}

{% for membre in comite.presidence -%}
  {%- if membre.website %} 
  - [{{ membre.name }}]({{ membre.website }}) ({{ membre.institution }})
  {%- else %} 
  - {{ membre.name }} ({{ membre.institution }}) 
  {%- endif -%}
{% endfor %}
{% endfor %}

Les comités détaillés pour les JFPC se trouvent [ici]({{ site.baseurl }}/jfpc/comites), et ceux pour les JIAF est [ici]({{ site.baseurl }}/jiaf/comites)