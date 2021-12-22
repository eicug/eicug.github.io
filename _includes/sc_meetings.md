{%- for item in site.data.sc_meetings -%}
{%- assign minlink='minutes' -%}
* {{ item.date }}:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[agenda]({{ item.url }}){:target="_blank"}/[{{minlink}}]({{ item.minutes }}){:target="_blank"}
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;{{ item.comment}}
{% endfor %}