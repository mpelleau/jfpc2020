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

{% assign thecomite = comite.presidence %}
{% include _list_members.md %}
{% endfor %}

## JIAF

{% for comite in site.data.comites_jiaf %}
### Comité {{ comite.type }}

{% assign thecomite = comite.presidence %}
{% include _list_members.md %}
{% endfor %}

Les comités détaillés pour les JFPC se trouvent [ici]({{ site.baseurl }}/jfpc/comites), et ceux pour les JIAF est [ici]({{ site.baseurl }}/jiaf/comites)