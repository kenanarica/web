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
      <div class="post_content">
      <a href="{{ post.url }}">
        {{ post.title }}
      </a>
      - <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time>
      {{ post.content }}
      </div>
      </div>
  {% endfor %}
</ul>