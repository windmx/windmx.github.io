---
layout: page
title: Links
description: 人是社会性动物，website也是。
keywords: 友情链接
comments: true
menu: 链接
permalink: /links/
---

> 桃花潭水深千尺 不及汪伦送我情

<ul>
{% for link in site.data.links %}
  {% if link.src == 'life' %}
  <li><a href="{{ link.url }}" target="_blank">{{ link.name}}</a></li>
  {% endif %}
{% endfor %}
</ul>

> 友情链接

<ul>
{% for link in site.data.links %}
  {% if link.src == 'www' %}
  <li><a href="{{ link.url }}" target="_blank">{{ link.name}}</a></li>
  {% endif %}
{% endfor %}
</ul>
