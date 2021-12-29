---
layout: default
title: welcome to the campfire
---

<div class="homeheader">
hmm.camp
  <div class="what">
    <a href="what"> what </a>
  </div>
</div>

<ul>
  {% for post in site.posts %}
      <div class="post">
      <a href="{{ post.url }}">
        {{ post.title }}
      </a>
      - <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time>
      {{ post.content }}
      </div>
  {% endfor %}
</ul>