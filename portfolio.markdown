---
title: Portfolio
date: 2020-07-21 23:08:00 Z
layout: page
---

<div class="content">
<ul>
{% assign portfolio1 = site.portfolio | sort: 'date' | reverse %}
{% for portfolio in portfolio1 %}
<li><a href="{{ portfolio.url }}"> {{ portfolio.title }}</a> - {{ portfolio.categories }} - {{ portfolio.date | date: "%B %Y"}} </li>
{% endfor %}
</ul>
</div>