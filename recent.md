{% for post in site.posts limit:5 %}
<div style="padding-bottom: 12px;">
<h3 style="margin: 0px; padding: 0px;">{{ post.title | markdownify }}</h3>
{{ post.excerpt | markdownify }}
<sub style="margin: 0px; padding-top: 0px; padding-bottom: 8px;">
{{ post.date | date_to_string }}
<a href="{{ post.url }}">View Post</a>
</sub>
<hr/>
</div>
{% endfor %}