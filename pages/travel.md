---
layout: default
title: Travel
---
{% assign posts = site.categories.Trips %}
{% for post in posts %}
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
  </div>
{% endif %}
  
{% endfor %}