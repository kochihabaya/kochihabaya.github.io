## Kochi Habaya

Hello y'all

{% for post in site.posts %}
    - [{{ post.title }}]({{ post.url }}) - {{ post.excerpt }}
{% endfor %}
