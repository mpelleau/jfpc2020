---
layout: page
show_meta: false
permalink: jiaf/programme
title: Programme des JIAF
published: true
conference: jiaf
---

{% for agenda in site.data.programme_jiaf %}
## {{ agenda.day }}

| Horaire | Activités        |
|---------+------------------|
{% for session in agenda.sessions -%}
| {{ session.time }} | {{ session.info}} |
{% endfor -%}
{% endfor %}
