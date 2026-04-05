---
layout: default
title: Blog
permalink: /blog/
---

<link rel="stylesheet" href="{{ '/assets/css/style.css' | relative_url }}">

<div class="custom-blog-container">
  <!-- Banner Image -->
  <div class="custom-banner">
    <img src="{{ '/assets/image_2.jpeg' | relative_url }}" alt="Blog Banner" class="custom-banner-image">
    <div class="custom-banner-overlay">
      <h1 class="custom-banner-title">My Blog</h1>
      <p class="custom-banner-subtitle">Thoughts, tutorials, and insights</p>
    </div>
  </div>

  <!-- Article 1 -->
  <article class="custom-article-card">
    <div class="custom-article-content">
      <h2 class="custom-article-title">Using Flexbox for easy alignment</h2>
      
      <div class="custom-article-meta">
        <span>By Rida Batool Mar 2026</span>
        <span>5 min read</span>
      </div>
      
      <div class="custom-article-text">
        <p>Flexbox made it easy to align cards and navigation links. I used it for row and column layouts instead of trying complex positioning.</p>

        <div class="custom-code-block">
          <div class="custom-code-header">
            <span>layout.css (flexbox)</span>
            <button class="custom-copy-btn" onclick="copyCode(this)">Copy</button>
          </div>
          <pre><code>.card-row {
  display: flex;
  gap: 16px;
  flex-wrap: wrap;
}

.card {
  flex: 1 1 280px;
  background: #ffffff;
  border-radius: 12px;
  padding: 16px;
}</code></pre>
        </div>

        <h2>Improving readability with spacing</h2>
        <p>I learned that text is easier to read with proper line-height and margin. Small spacing changes can make a big visual difference.</p>

        <div class="custom-code-block">
          <div class="custom-code-header">
            <span>typography.css</span>
            <button class="custom-copy-btn" onclick="copyCode(this)">Copy</button>
          </div>
          <pre><code>body {
  line-height: 1.7;
  color: #2a2b3e;
}

h2 {
  margin-top: 24px;
  margin-bottom: 8px;
}

p {
  margin-bottom: 14px;
}</code></pre>
        </div>

        <h3>My beginner CSS checklist</h3>
        <ul>
          <li>Use consistent spacing values.</li>
          <li>Keep color palette small and clean.</li>
          <li>Test layout on smaller screens.</li>
          <li>Avoid too many effects and animations.</li>
        </ul>

        <h2>How I made the layout responsive</h2>
        <p>I used media queries to change card layout from three columns to one column on smaller devices. This made the content easier to read on mobile phones.</p>
        <p>I also reduced image height and font size slightly on small screens so the page feels more balanced and user-friendly.</p>

        <h2>Key lesson from CSS practice</h2>
        <p>Good design is not always advanced design. For beginner projects, simple colors, readable text, and consistent spacing create a professional result.</p>
      </div>
      
      <div class="custom-tags-container">
        <span class="custom-tag">#CSS</span>
        <span class="custom-tag">#Flexbox</span>
        <span class="custom-tag">#WebDesign</span>
      </div>
    </div>
  </article>

  <!-- Article 2 -->
  <article class="custom-article-card">
    <div class="custom-article-content">
      <h2 class="custom-article-title">Getting Started with JavaScript</h2>
      
      <div class="custom-article-meta">
        <span>📅 January 8, 2024</span>
        <span>⏱️ 4 min read</span>
      </div>
      
      <div class="custom-article-text">
        <p>JavaScript is essential for modern web development. Here's how I started my journey with this powerful language.</p>
        
        <h2>Variables and Data Types</h2>
        <p>Understanding variables is the first step. JavaScript has let, const, and var declarations.</p>
        
        <div class="custom-code-block">
          <div class="custom-code-header">
            <span>variables.js</span>
            <button class="custom-copy-btn" onclick="copyCode(this)">Copy</button>
          </div>
          <pre><code>let name = "John";
const age = 25;
var isActive = true;

console.log(`Hello, I'm ${name} and I'm ${age} years old`);</code></pre>
        </div>
        
        <h2>Functions Made Simple</h2>
        <p>Functions are reusable blocks of code that make your program organized.</p>
        
        <div class="custom-code-block">
          <div class="custom-code-header">
            <span>functions.js</span>
            <button class="custom-copy-btn" onclick="copyCode(this)">Copy</button>
          </div>
          <pre><code>function greet(name) {
  return `Hello, ${name}!`;
}

const arrowGreet = (name) => `Hello, ${name}!`;

console.log(greet("Developer"));</code></pre>
        </div>
      </div>
      
      <div class="custom-tags-container">
        <span class="custom-tag">#JavaScript</span>
        <span class="custom-tag">#Programming</span>
        <span class="custom-tag">#Beginner</span>
      </div>
    </div>
  </article>
</div>

<script>
function copyCode(button) {
  const codeBlock = button.closest('.custom-code-block');
  const code = codeBlock.querySelector('code').innerText;
  
  navigator.clipboard.writeText(code).then(() => {
    const originalText = button.innerText;
    button.innerText = 'Copied!';
    setTimeout(() => {
      button.innerText = originalText;
    }, 2000);
  });
}
</script>
