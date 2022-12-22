---
layout: default
title: the sewer of the internet 
---



<!-- <div class="homeheader">
hmm.camp
  <div class="what">
    <a href="what"> what </a>
  </div>
</div> -->
<div class="reactContainer">
<div class="sideCol"></div>
<div class="postCol">
  <div class="homeheaderDiv">
            <h1 class="homeheader"> my little internet hideout </h1>
  </div>
  <ul>
    {% for post in site.posts %}
      <div class="post">
        <div class="postContent">
        <h3>
          {{ post.title }}
        </h3>
          - <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_string }}</time>
          {{ post.content }}
        </div>
      </div>
    {% endfor %}
  </ul>
  </div>
  <div class="sideCol"></div>
</div>

<!-- <div class="reactContainer">
      <div class="sideCol">
        asdasd  
      </div>
      <div class="postCol">
        <div class="homeheaderDiv">
          <h1 class="homeheader"> my little internet hideout </h1>
        </div>

        {% for post in site.posts %}
        <div class="post">
          <div class="postContent">
            <a href="{{ post.url }}">
              {{ post.title }}
            </a>
            - <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_string }}</time>
            {{ post.content }}
          </div>
        </div>
      {% endfor %}

      </div>
      <div class="sideCol">
        ;ll;kl;k;lk  
      </div>
</div> -->