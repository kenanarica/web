---
layout: default
---

some content
<ul>
  {% for post in site.posts %}

      <a href="{{ post.url }}">
        {{ post.title }}
      </a>
      - <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time>
      {{ post.content }}

  {% endfor %}
</ul>