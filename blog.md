---
layout: default
title: Blog
permalink: /blog/
---

<link rel="stylesheet" href="{{ '/assets/css/style.css' | relative_url }}">

<div class="custom-blog-container">
  <div class="custom-banner">
    <img src="{{ '/assets/image_2.jpeg' | relative_url }}" alt="Blog Banner" class="custom-banner-image">
    <div class="custom-banner-overlay">
      <h1 class="custom-banner-title">My Blog</h1>
      <p class="custom-banner-subtitle">Thoughts, tutorials, and insights</p>
    </div>
  </div>

  {% for post in site.posts %}
  <article class="custom-article-card">
    <div class="custom-article-content">
      <h2 class="custom-article-title">
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      </h2>
      <div class="custom-article-meta">
        <span>By Rida Batool {{ post.date | date: "%b %Y" }}</span>
        <span>5 min read</span>
      </div>
      <div class="custom-article-text">
        <p>{{ post.excerpt | strip_html | truncate: 150 }}</p>
      </div>
    </div>
  </article>
  {% endfor %}

</div>
