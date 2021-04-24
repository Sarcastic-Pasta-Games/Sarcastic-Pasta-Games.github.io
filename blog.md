---
layout: default
title: Blog
---
<div class="white-background">
  <h1>Latest Posts</h1>


  <ul>
    {% for post in site.posts %}
    <li>
      <h3><a href="{{ post.url }}" class="white-background">{{ post.title }}</a></h3>
      {{ post.excerpt }}
    </li>
    {% endfor %}
  </ul>
</div>