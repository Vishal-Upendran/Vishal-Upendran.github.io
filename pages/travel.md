---
layout: default
title: Travel
---

{% for post in site.posts %}
  <div class="btn">
      <a href="{{ post.url }}" ><img src="{{ post.thumbnail }}" width="300" />
      <a href="{{ post.url }}" >{{ post.title }}</a>
  </div>
{% endfor %}