
{% assign stub='/content/' %}

{% if include.active contains 'index' %}
{% assign stub='/' %}
{% endif %}

{% assign page_name=include.name %}

{% assign content_link=stub | append: include.active | append: ".html" | relative_url %}

{% if page_name contains include.active %}
{% assign return_stub='<a class="nav-link active" href="' %}
{% else %}
{% assign return_stub='<a class="nav-link" href="' %}
{% endif %}


{% assign return_string=return_stub  | append: content_link | append: '"><span style="color:coral;" data-feather="' | append: include.icon | append: '"></span>' %}

{{ return_string }}
