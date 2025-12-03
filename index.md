Hi my name is JadenG welcome to my blog


<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      <a href="{{ post.url | relative_url }}">{{ }}</a>
    </li>
  {% endfor %}
</ul>