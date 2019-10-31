
{% for membre in thecomite -%}
  {%- if membre.website %} 
  - [{{ membre.name }}]({{ membre.website }}) ({{ membre.institution }})
  {%- else %} 
  - {{ membre.name }} ({{ membre.institution }}) 
  {%- endif -%}
{%- endfor %}