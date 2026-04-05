---
layout: post
title: "My First Post"
---

<div class="custom-post-wrapper">
  <div class="custom-post-header">
    <h1 class="custom-post-heading">My First Post</h1>
    <p class="custom-post-meta">{{ page.date | date: "%B %d, %Y" }}</p>
  </div>
  
  <div class="custom-featured-image">
    <img src="/assets/image_1.jpeg" alt="Featured image" class="custom-image">
  </div>
  
  <div class="custom-post-body">
    <p class="custom-paragraph">This is my first blog post.</p>
    
    <p class="custom-paragraph">I created this post using Jekyll's post system so I can keep adding weekly posts without changing the website structure.</p>
  </div>
  
  <a href="/blog/" class="custom-back-button">← Back to Blog</a>
</div>

<style>
  .custom-post-wrapper {
    max-width: 800px;
    margin: 0 auto;
    padding: 20px;
  }
  
  .custom-post-header {
    text-align: center;
    margin-bottom: 40px;
    border-bottom: 2px solid #f0f0f0;
    padding-bottom: 20px;
  }
  
  .custom-post-heading {
    color: #2c3e50;
    font-size: 2.5em;
    margin-bottom: 10px;
  }
  
  .custom-post-meta {
    color: #7f8c8d;
    font-size: 0.9em;
  }
  
  .custom-featured-image {
    text-align: center;
    margin: 30px 0;
  }
  
  .custom-image {
    max-width: 100%;
    height: auto;
    border-radius: 8px;
    box-shadow: 0 2px 8px rgba(0,0,0,0.1);
  }
  
  .custom-post-body {
    font-size: 1.1em;
    line-height: 1.8;
    color: #34495e;
  }
  
  .custom-paragraph {
    margin-bottom: 20px;
  }
  
  .custom-back-button {
    display: inline-block;
    margin-top: 40px;
    padding: 10px 20px;
    background: #3498db;
    color: white;
    text-decoration: none;
    border-radius: 5px;
    transition: background 0.2s;
  }
  
  .custom-back-button:hover {
    background: #2980b9;
  }
</style>
