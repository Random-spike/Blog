---
layout: default
title: 我的博客
---

# ✨ 我的文章

{% for post in site.posts %}
<div style="margin-bottom: 1em;">
  <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
  <p><small>{{ post.date | date: "%Y-%m-%d" }}</small></p>
  <p>{{ post.excerpt | strip_html | truncate: 100 }}</p>
</div>
{% endfor %}
