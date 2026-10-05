---
layout: default
title: Projects
permalink: /projects/
---
# Projects

Six hands-on projects applying high-dimensional data analysis to real public datasets, one per sector. Each has a code repository, a plain-language write-up and a short theory note.

<ul class="card-list">
{% assign items = site.projects | sort: "order" %}
{% for p in items %}
  <li>
    <span class="tag">{{ p.sector }}</span><span class="tag">{{ p.status | default: "Planned" }}</span>
    <h3><a href="{{ p.url | relative_url }}">{{ p.title }}</a></h3>
    <p>{{ p.summary }}</p>
  </li>
{% endfor %}
</ul>
