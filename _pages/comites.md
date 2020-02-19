---
layout: page
show_meta: false
permalink: team/
title: Comités
published: true
---

## JFPC

{% for comite in site.data.comites_jfpc %}
### Comité {{ comite.type }}

{% include list_members members = comite.presidence %}
{% endfor %}

## JIAF

{% for comite in site.data.comites_jiaf %}
### Comité {{ comite.type }}

{% include list_members members = comite.presidence %}
{% endfor %}

Les comités détaillés pour les JFPC se trouvent [ici]({{ site.baseurl }}/jfpc/comites/), et ceux pour les JIAF est [ici]({{ site.baseurl }}/jiaf/comites/)