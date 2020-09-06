---
layout: default
title: Travel
---

{% for post in site.posts %}
<div>
    <a href="{{ post.url }}" ><img src="{{ post.thumbnail }}" />
    <a href="{{ post.url }}" >{{ post.title }}</a>
</div>
{% endfor %}