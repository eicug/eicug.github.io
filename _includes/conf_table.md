{%- if include.year=='' -%}
{%- assign selection=site.data.conferences | where: "status", include.status -%}
{%- else -%}
{%- assign selection=site.data.conferences | where: "status", include.status | where: "year", include.year -%}
{%- endif %}

<table width="80%" border="1" align="center">
<tr><th>Conference/Workshop</th><th>Dates</th></tr>
{%- for conf in selection -%}
<tr>
<td width="75%">
{%- if conf.url=='' -%}
{{ conf.name }}
{%- else %}
<a href="{{ conf.url }}" target="_blank">{{ conf.name }}</a>
{%- endif %}
</td>
<td width="25%">{{ conf.dates }}</td>
</tr>
{%- endfor -%}
</table>
