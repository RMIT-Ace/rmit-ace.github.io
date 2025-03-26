  {% for post in site.posts %}
    {% include_relative post.url %}
  {% endfor %}