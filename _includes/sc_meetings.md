{%- for item in site.data.sc_meetings -%}
* {{ item.date }}:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[agenda]({{ item.url }}){:target="_blank"}/[minutes]({{ item.minutes }}){:target="_blank"}&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;{{ item.comment}}
{% endfor %}