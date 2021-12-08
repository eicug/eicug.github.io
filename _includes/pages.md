{% if include.active=='index' %}
{% assign the_name='index' %}
{% assign stub='/' %}
{% else %}
{% assign the_name=include.active %}
{% assign stub='/content/' %}
{% endif %}

{% assign content_link=stub | append: the_name | append: ".html" | relative_url %}

{% if include.name==include.active %}
{% assign return_string='<a class="nav-link active" href="' | append: content_link | append: '">' %}
{% else %}
{% assign return_string='<a class="nav-link" href="' | append: content_link | append: '">' %}
{% endif %}

{{ return_string }}