---
layout: page_jiaf
show_meta: false
permalink: jiaf/programme
title: Programme des JIAF
published: true
---

{% for agenda in site.data.programme_jiaf %}
## {{ agenda.day }}

| Horaire | Activités        |
|---------+------------------|
{% for session in agenda.sessions -%}
| {{ session.time }} | {{ session.info}} |
{% endfor -%}
{% endfor -%}
