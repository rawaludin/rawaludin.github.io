---
layout: page
title: Rahmat Awaludin
---


<ul class="posts">
  {% for post in site.posts %}
   {% unless post.draft %}
    <li><span>{{ post.date | date_to_string }}</span> <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
   {% endunless %}
  {% endfor %}
</ul>
