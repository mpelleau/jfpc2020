---
layout: page
show_meta: false
permalink: jfpc/programme/index
title: Programme des JFPC
published: true
conference: jfpc
---

{% for agenda in site.data.programme_jfpc %}
## {{ agenda.day }}

| Horaire | Activités        |
|---------+------------------|
{% for session in agenda.sessions -%}
| {{ session.time }} | {{ session.info}} |
{% endfor -%}
{% endfor %}
