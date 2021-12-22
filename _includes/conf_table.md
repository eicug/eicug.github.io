{%- assign upcoming=site.data.conferences | where: "status", "upcoming" -%}
{%- assign past=site.data.conferences | where: "status", "past" -%}

<table width="80%" border="1" align="center">
<tr>
<th>Conference/Workshop</th><th>EICUG Participation/Speaker</th>
</tr>
{%- for conf in upcoming -%}
<tr>
<td>
{%- if conf.url=='' -%}
{{ conf.name }}
{%- else %}
<a href="{{ conf.url }}" target="_blank">{{ conf.name}}</a>
{%- endif %}
</td>
<td>
{{ conf.eicug }}
</td>
</tr>
{%- endfor -%}
</table>
