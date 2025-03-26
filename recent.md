{% for post in site.posts limit:5 %}
<div style="padding-bottom: 12px;">
<h3 style="padding-bottom: 2px;">{{ post.title | markdownify }}</h3>
<sub>{{ post.date | date_to_string }}</sub>
{{ post.excerpt | markdownify }}
<sub><a href="{{ post.url }}">View Post</a></sub>
</div>
{% endfor %}