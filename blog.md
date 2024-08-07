---
layout: default
title: Blog
permalink: /blog/
---

# Blog

Here you will find all the latest posts.

{% for post in site.posts %}
  <article>
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    <p>{{ post.excerpt | markdownify }}</p>
    <p><small>Posted on {{ post.date | date: "%b %d, %Y" }}</small></p>
  </article>
{% endfor %}
