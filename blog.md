---
layout: default
title: Blog
permalink: /blog/
---

<div class="custom-blog-wrapper">
  <div class="custom-blog-header">
    <h1 class="custom-blog-title">Blog</h1>
    <p class="custom-blog-subtitle">Here are my posts:</p>
  </div>

  <div class="custom-posts-list">
    {% for post in site.posts %}
      <div class="custom-post-card">
        <h2 class="custom-post-card-title">
          <a href="{{ post.url | relative_url }}" class="custom-post-link">{{ post.title }}</a>
        </h2>
        <p class="custom-post-date">{{ post.date | date: "%B %d, %Y" }}</p>
        <p class="custom-post-excerpt">{{ post.excerpt | strip_html | truncate: 150 }}</p>
      </div>
    {% endfor %}
  </div>
</div>

<style>
  .custom-blog-wrapper {
    max-width: 800px;
    margin: 0 auto;
    padding: 20px;
  }
  
  .custom-blog-header {
    text-align: center;
    margin-bottom: 40px;
  }
  
  .custom-blog-title {
    color: #333;
    font-size: 2.5em;
    margin-bottom: 10px;
  }
  
  .custom-blog-subtitle {
    color: #666;
    font-size: 1.1em;
  }
  
  .custom-posts-list {
    display: flex;
    flex-direction: column;
    gap: 20px;
  }
  
  .custom-post-card {
    background: white;
    border: 1px solid #e0e0e0;
    border-radius: 8px;
    padding: 20px;
    transition: transform 0.2s, box-shadow 0.2s;
  }
  
  .custom-post-card:hover {
    transform: translateY(-2px);
    box-shadow: 0 4px 12px rgba(0,0,0,0.1);
  }
  
  .custom-post-card-title {
    margin: 0 0 10px 0;
  }
  
  .custom-post-link {
    color: #2c3e50;
    text-decoration: none;
    font-size: 1.5em;
  }
  
  .custom-post-link:hover {
    color: #3498db;
  }
  
  .custom-post-date {
    color: #7f8c8d;
    font-size: 0.9em;
    margin: 0 0 10px 0;
  }
  
  .custom-post-excerpt {
    color: #555;
    line-height: 1.6;
    margin: 0;
  }
</style>
