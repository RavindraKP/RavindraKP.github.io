---
layout: default
title: Blog
permalink: /blog/
---
# Blog

<ul class="card-list">
{% for post in site.posts %}
  <li>
    <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
    <p>{{ post.date | date: "%-d %B %Y" }}{% if post.summary %}. {{ post.summary }}{% endif %}</p>
  </li>
{% endfor %}
</ul>
