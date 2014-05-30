---
layout: page
---
{% include JB/setup %}

<ul class="posts">
  {% for post in site.posts %}
     ## <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
     <li><span>{{ post.date | date_to_string }}</span>
      {{ site.content }}
  {% endfor %}
</ul>


