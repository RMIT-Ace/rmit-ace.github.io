
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a><sub>({{ post.date | date_to_string }})</sub>
    </li>
  {% endfor %}
</ul>
