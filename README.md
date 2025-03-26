# [Blogs](all-blogs.md)

{% for post in site.posts %}
<div>
{{ post.title | markdownify }}<br/>
{{ post.excerpt | markdownify }}
</div>
{% endfor %}

[More Blog Posts](all-blogs.md)

# Projects

- [Apple Health & Fitness](https://github.com/RMIT-Ace/Apple-Health-and-Fitness)
- [Apple Foundation Program App](https://github.com/RMIT-Ace/AFP)
    - [AFP People Management System](https://github.com/RMIT-Ace/AFP-People-Db)
    - [AFP People Management App](https://github.com/RMIT-Ace/AFP-People-App)
