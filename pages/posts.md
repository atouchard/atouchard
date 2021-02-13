---
title: Blog
layout: default
permalink: /blog
---

# Blog

{% for post in site.posts %}
  <div class="row mb-2">
      <div class="col-sm-9">
          <a href="{{ post.url | relative_url }}">{{ post.title | smartify }}</a>
      </div>
      <div class="col-sm-3 text-muted text-right small">
          {{ post.date | date: '%B %-d, %Y' }}
      </div>
  </div>
{% endfor %}
