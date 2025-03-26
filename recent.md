{% for post in site.posts %}
<div>
<h3>{{ post.title | markdownify }}</h3>
{{ post.excerpt | markdownify }}
<sub>{{ post.date | markdownify }}</sub>
</div>
{% endfor %}