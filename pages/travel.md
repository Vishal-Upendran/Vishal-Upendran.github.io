---
layout: default
title: Travel
---
{% assign posts = site.categories.Trips %}
{% for post in posts %}
{% assign loopindex = forloop.index | modulo: 2 %}
{% if loopindex == 1 %}
  <div class="row">
  <div class="column">
      <figure>
        <a href="{{ post.url }}" > <img src="{{post.thumbnail}}" style="width:100%"></a>
        <figcaption style="text-align: center"> <a href="{{ post.url }}" >{{ post.title }}</a> </figcaption>
      </figure>
  </div>
{% else %}
  <div class="column">
    <figure>
        <a href="{{ post.url }}" > <img src="{{post.thumbnail}}" style="width:100%"></a>
        <figcaption style="text-align: center"> <a href="{{ post.url }}" >{{ post.title }}</a> </figcaption>
      </figure>
  </div>
  </div>
{% endif %}
  
{% endfor %}