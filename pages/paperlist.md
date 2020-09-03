---
layout: default
title: Material collation
description: Collection of papers, articles, and books
---


{% for post in site.posts %}
|<img width=1604 src="{{site.url}}/img/eclipse2.jpg"> {{ post.title }} |
{% endfor %}
