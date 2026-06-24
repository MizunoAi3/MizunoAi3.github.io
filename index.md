---
layout: default
title: Home
---

Welcome to the Mizuno AI Blog.

<ul>
  {% for post in site.posts %}
    <li><a href="{{ post.url | relative_url }}">{{ post.title }}</a> - {{ post.date | date: "%Y-%m-%d" }}</li>
  {% endfor %}
</ul>

Write posts as Markdown files in the _posts/ folder with filename format: YYYY-MM-DD-title.md
