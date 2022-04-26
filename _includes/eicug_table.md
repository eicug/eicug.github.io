<table width="100%" border="1" align="center">

<tr><th>Meeting</th><th>Dates</th></tr>

{%- for meet in site.data.eicug_meetings -%}
<tr>
<td width="60%">
{%- if meet.url=='' -%}
{{ meet.name }}
{%- else %}
<a href="{{ meet.url }}" target="_blank">{{ meet.name}}</a>
{%- endif %}
</td>
<td width="40%">
{{ meet.dates }}
</td>
</tr>
{%- endfor -%}
</table>
