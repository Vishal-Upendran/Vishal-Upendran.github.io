---
layout: default
title: Graduate School
description: 
category: iucaaprojs
---

You may find below a list of publications, and (in some cases) associated pages which simply the work for the common reader. The requisite citation is also mentioned in the content.

- **Solar wind prediction using deep learning**: Upendran, V., Cheung, M. C. M., Hanasoge, S., & Krishnamurthi, G. ( 2020). Solar wind prediction using deep learning. Space Weather, 18, e2020SW002478. https://doi.org/10.1029/2020SW002478. Arxiv: https://arxiv.org/abs/2006.05825. Git: https://github.com/Vishal-Upendran/WindNet. ML-Helio: https://zenodo.org/record/3866169#.X1CjaIbhV0A. 


{% for post in site.posts %}
|<img width=1604 src="{{site.url}}/{{post.img}}"> <a href="{{site.url}}/{{post.url}}">{{ post.title }} |
{% endfor %}