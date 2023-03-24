---
layout: page
title: About
description: 虚惊一场是人世间最美好的成语。
keywords: 人间漫游指南
comments: true
menu: 关于
permalink: /about/
---

VC从业者

拥有一辆 SUZUKI JIMNY

朴树｜伍佰 & China Blue 二十年老粉

INFP｜天蝎座

## 联系

<ul>
{% for website in site.data.social %}
<li>{{website.sitename }}：<a href="{{ website.url }}" target="_blank">@{{ website.name }}</a></li>
{% endfor %}
{% if site.url contains 'dumengxi.com' %}
<li>
微信公众号：<br />
<img style="height:192px;width:192px;border:1px solid lightgrey;" src="{{ site.url }}/assets/images/qrcode.jpg" alt="人间漫游指南" />
</li>
{% endif %}
</ul>


## Skill Keywords

{% for skill in site.data.skills %}
### {{ skill.name }}
<div class="btn-inline">
{% for keyword in skill.keywords %}
<button class="btn btn-outline" type="button">{{ keyword }}</button>
{% endfor %}
</div>
{% endfor %}
