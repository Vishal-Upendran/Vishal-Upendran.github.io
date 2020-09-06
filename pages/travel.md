---
layout: default
title: Travel
---

{% for post in site.posts %}
{% assign loopindex = forloop.index | modulo: 2 %}
{% if loopindex == 1 %}
  <div>
      <!-- <a href="{{ post.url }}" ><img src="{{ post.thumbnail }}" width="300" />
      <a href="{{ post.url }}" >{{ post.title }}</a> -->
      <figure>
        <a href="{{ post.url }}" > <img src="{{post.thumbnail}}" style="width:30%"></a>
        <figcaption> <a href="{{ post.url }}" >{{ post.title }}</a> </figcaption>
      </figure>
{% else %}
    <figure>
        <a href="{{ post.url }}" > <img src="{{post.thumbnail}}" style="width:30%"></a>
        <figcaption> <a href="{{ post.url }}" >{{ post.title }}</a> </figcaption>
      </figure>

{% endif %}
  </div>
{% endfor %}