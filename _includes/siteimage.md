{% assign image_link = '/assets/images/site/' | append: include.file | relative_url %}
{% if include.width %}
<img src="{{ image_link }}" width="{{ include.width }}">
{% else %}
<img src="{{ image_link }}">
{% endif %}