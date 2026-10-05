---
layout: default
title: Home
---
# {{ site.title }}

{{ site.tagline }}. Notes and projects by {{ site.author }}. I work on AI products in education and write about applied machine learning, statistics and high-dimensional data. This site holds my project write-ups and learning notes.

## Featured projects

<ul class="card-list">
{% assign items = site.projects | sort: "order" %}
{% for p in items limit:3 %}
  <li>
    <span class="tag">{{ p.sector }}</span><span class="tag">{{ p.status | default: "Planned" }}</span>
    <h3><a href="{{ p.url | relative_url }}">{{ p.title }}</a></h3>
    <p>{{ p.summary }}</p>
  </li>
{% endfor %}
</ul>

[See all projects]({{ '/projects/' | relative_url }})

## Latest writing

<ul class="card-list">
{% for post in site.posts limit:3 %}
  <li>
    <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
    <p>{{ post.date | date: "%-d %B %Y" }}. {{ post.summary }}</p>
  </li>
{% endfor %}
</ul>

[See all posts]({{ '/blog/' | relative_url }})
