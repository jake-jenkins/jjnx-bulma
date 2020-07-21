---
title: Portfolio
date: 2020-07-21 23:08:00 Z
---

<div class="content">
<ul>
{% for portfolio in site.portfolio %}
<li><a href="{{ portfolio.url }}"> {{ portfolio.title }}</a> - {{ portfolio.categories }} </li>
{% endfor %}
</ul>
</div>