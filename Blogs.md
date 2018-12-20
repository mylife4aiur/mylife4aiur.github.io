---
bg: "seek.jpg"
layout: page
title: "Blog"
crawlertitle: "Haoyu's blogs"
permalink: /blogs/
summary: "Seek the Extraordinary"
active: about
weight: 1
---

{% for post in site.posts %}
  <article class="index-page">
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    {{ post.excerpt }}
  </article>
{% endfor %}
