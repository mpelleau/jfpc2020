---
layout: page_jiaf
show_meta: false
permalink: jiaf/editions
title: Précédentes éditions
published: true
---

{% for edition in site.data.editions_jiaf %}
  - [{{ edition.lieu }}]({{ edition.website }}) -- {{ edition.annee }}
{% endfor %}