---
layout: default
title: Travel
---

{% for post in site.categories %}
<div>
    <a href="{{ post.url }}" ><img src="{{ post.thumbnail }}" />
    <a href="{{ post.url }}" >Hi Lol</a>
</div>
{% endfor %}