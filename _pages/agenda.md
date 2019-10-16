---
layout: page
show_meta: false
permalink: /agenda
title: Agenda
published: true
---

{% for agenda in site.data.programme %}
## {{ agenda.day }}

| Horaire | Activités        |
|---------+------------------|
{% for session in agenda.sessions -%}
| {{ session.time }} | {{ session.info}} |
{% endfor -%}
{% endfor -%}
