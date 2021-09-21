---
layout: page
title: About
description: 代码改变世界
keywords: VCG
comments: true
menu: 关于
permalink: /about/
---

这是VCG的博客

仰慕互联网

仰慕自由，开放，共享的互联网

![Aaron_Hillel_Swartz_King_of_the Web](http://shit.vcgplus.xyz/images/Aaron_Hillel_Swartz.png)

## 联系

<ul>
{% for website in site.data.social %}
<li>{{website.sitename }}：<a href="{{ website.url }}" target="_blank">@{{ website.name }}</a></li>
{% endfor %}
{% if site.url contains 'mazhuang.org' %}
{% endif %}
</ul>


## 技能

{% for skill in site.data.skills %}
### {{ skill.name }}
<div class="btn-inline">
{% for keyword in skill.keywords %}
<button class="btn btn-outline" type="button">{{ keyword }}</button>
{% endfor %}
</div>
{% endfor %}
