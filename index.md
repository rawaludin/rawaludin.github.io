---
layout: default
title: Rahmat Awaludin
---

<div id="postlist">
  {% for post in site.posts %}
   {% unless post.draft %}
  <div class="post">
    <h3><a href="{{ BASE_PATH }}{{ post.url }}" title="Permalink to this article">{{ post.title }}</a></h3>
    <div class="postinfo">
      <p class="published" title="{{ post.date | date_to_string }}"> {{ post.date | date_to_string }} </p>
    </div>
  </div>
   {% endunless %}
  {% endfor %}
</div>
