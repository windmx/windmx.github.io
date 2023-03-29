---
layout: page
title: About
description: 虚惊一场是人世间最美好的成语。
keywords: 人间漫游指南
comments: true
menu: 关于
permalink: /about/
---
情感的乐观主义者，历史的悲观主义者

VC从业人员，移动互联网第一代原住民

拥有一辆 SUZUKI Jimny

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
