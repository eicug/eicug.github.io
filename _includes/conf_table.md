{%- assign upcoming=site.data.conferences | where: "status", include.status -%}

<table width="80%" border="1" align="center">
<tr>
<th>Conference/Workshop</th><th>Dates</th><th>EICUG Participation/Speaker</th>
</tr>
{%- for conf in upcoming -%}
<tr>
<td width="50%">
{%- if conf.url=='' -%}
{{ conf.name }}
{%- else %}
<a href="{{ conf.url }}" target="_blank">{{ conf.name}}</a>
{%- endif %}
</td>
<td width="25%">
{{ conf.dates }}
</td>
<td width="25%">
{{ conf.eicug }}
</td>
</tr>
{%- endfor -%}
</table>
