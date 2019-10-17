---
layout: page_jfpc
show_meta: false
permalink: jfpc/programme
title: Programme des JFPC
published: true
---

{% for agenda in site.data.programme_jfpc %}
## {{ agenda.day }}

| Horaire | Activités        |
|---------+------------------|
{% for session in agenda.sessions -%}
| {{ session.time }} | {{ session.info}} |
{% endfor -%}
{% endfor -%}
