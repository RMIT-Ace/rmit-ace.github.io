{% for post in site.posts limit:5 %}
<div style="padding-bottom: 10px;">
<h3>{{ post.title | markdownify }}</h3>
{{ post.excerpt | markdownify }}
<sub>{{ post.date | date_to_string }} <a href="{{ post.url }}">View Post</a></sub>
</div>
{% endfor %}