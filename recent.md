  {% for post in site.posts %}
    <div>
    {{ post.title }}<br/>
    {{ post.excerpt }}
    </div>
  {% endfor %}