---
layout: page
title: Home
---
{% include JB/setup %}

<ul class="posts">
  {% for post in site.posts limit 5 %}
      <div class="page-header">
        <h1> <a href="{{ BASE_PATH }}{{ post.url}}">{{ post.title }}</a> <small>{{ post.date | date_to_long_string }}</small></h1>
        </div>
          <div class="content">
            {{ post.content | truncatewords:75 }}
            <a href="{{ post.url }}"> Read More...</a>
          </div>
  {% endfor %}
</ul>


