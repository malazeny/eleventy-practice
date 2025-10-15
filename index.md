---
layout: base.njk
title: Home
---

# Hello, Welcome to my Site
Everything you need to know about me!

<div class="banner-list">
  {% for post in collections.post %}
  <a href="{{ post.url | prefixedUrl }}" class="banner-full">
    <div class="banner-bg" style="background-image: url('{{ post.data.banner | prefixedUrl }}')">
      <div class="banner-text">
        <h2>{{ post.data.title }}</h2>
        <p>{{ post.data.description }}</p>
      </div>
    </div>
  </a>
  {% endfor %}
</div>

np