
{% assign stub='/content/' %}
{% assign content_link=stub | append: include.active | append: ".html" | relative_url %}


{% if include.active contains 'index' %}
{% assign stub='/' %}
{% assign content_link=stub | relative_url %}
{% endif %}


{% assign page_name=include.name %}


{% if page_name contains include.active %}
{% assign return_stub='<a class="nav-link active" href="' %}
{% else %}
{% assign return_stub='<a class="nav-link" href="' %}
{% endif %}


{% assign return_string=return_stub  | append: content_link | append: '"><span style="color:coral;" data-feather="' | append: include.icon | append: '"></span>' %}

{{ return_string }}
