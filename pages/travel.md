---
layout: default
title: Travel
---

{% for post in site.posts %}
  <div>
      <!-- <a href="{{ post.url }}" ><img src="{{ post.thumbnail }}" width="300" />
      <a href="{{ post.url }}" >{{ post.title }}</a> -->
      <figure>
        <a href="{{ post.url }}" > <img src="{{post.thumbnail}}" style="width:30%"></a>
        <figcaption style="text-align: center"> <a href="{{ post.url }}" >{{ post.title }}</a> </figcaption>
      </figure>
  </div>
{% endfor %}