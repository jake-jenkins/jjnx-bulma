---
title: Blog
permalink: "/blog/"
layout: page
---

This is something new which is coming soon.

<div class="content">
<ul>
{% assign blog1 = site.blog | sort: 'date' | reverse %}
{% for blog in blog1 %}
<li><a href="{{ blog.url }}"> {{ blog.title }}</a> - {{ blog.categories }} - {{ blog.date | date: "%B %Y"}} </li>
{% endfor %}
</ul>
</div>