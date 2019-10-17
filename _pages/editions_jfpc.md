---
layout: page_jfpc
show_meta: false
permalink: jfpc/editions
title: Précédentes éditions
published: true
---

{% for edition in site.data.editions_jfpc %}
  - [{{ edition.lieu }}]({{ edition.website }}) -- {{ edition.annee }}
{% endfor %}