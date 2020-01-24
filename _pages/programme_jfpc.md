---
layout: page
show_meta: false
permalink: jfpc/programme/
title: Programme des JFPC
published: true
conference: jfpc
---

Le programme détaillé n'est pas encore disponible.

<!--
{% for agenda in site.data.programme_jfpc %}
## {{ agenda.day }}

| Horaire | Activités        |
|---------+------------------|
{% for session in agenda.sessions -%}
| {{ session.time }} | {{ session.info}} |
{% endfor -%}
{% endfor %}-->

{% comment %}
{% include programme program = site.data.programme_jfpc %}
{% endcomment %}