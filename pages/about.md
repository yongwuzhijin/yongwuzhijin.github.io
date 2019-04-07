---
layout: page
title: About
description: 一个前端小白的日常
keywords: jace, yongwuzhijin, 永无止晋
comments: true
menu: 关于
permalink: /about/
---

我是永无止晋。

前端小白一枚。

践行做一件事，做好一件事。

## 联系

{% for website in site.data.social %}
* {{ website.sitename }}：[@{{ website.name }}]({{ website.url }})
{% endfor %}

## Skill Keywords

{% for category in site.data.skills %}
### {{ category.name }}
<div class="btn-inline">
{% for keyword in category.keywords %}
<button class="btn btn-outline" type="button">{{ keyword }}</button>
{% endfor %}
</div>
{% endfor %}
