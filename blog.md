---
layout: default
title: Blog
---

<link rel="stylesheet" href="/assets/css/style.css">

<style>
  .custom-blog-container {
    max-width: 900px;
    margin: 0 auto;
    padding: 20px;
  }
  
  .custom-banner {
    position: relative;
    margin-bottom: 40px;
    border-radius: 16px;
    overflow: hidden;
    box-shadow: 0 4px 20px rgba(0,0,0,0.1);
  }
  
  .custom-banner-image {
    width: 100%;
    height: 300px;
    object-fit: cover;
    display: block;
  }
  
  .custom-banner-overlay {
    position: absolute;
    bottom: 0;
    left: 0;
    right: 0;
    background: linear-gradient(to top, rgba(0,0,0,0.7), transparent);
    padding: 40px 30px 20px;
  }
  
  .custom-banner-title {
    color: white;
    font-size: 2.5em;
    margin: 0 0 10px 0;
  }
  
  .custom-banner-subtitle {
    color: rgba(255,255,255,0.9);
    font-size: 1.1em;
    margin: 0;
  }
  
  .custom-section-title {
    font-size: 1.8em;
    margin: 40px 0 20px 0;
    color: var(--blog-text);
    border-left: 4px solid var(--blog-accent);
    padding-left: 15px;
  }
  
  .custom-article-card {
    background: var(--blog-surface);
    border: 1px solid var(--blog-border);
    border-radius: 12px;
    margin-bottom: 30px;
    overflow: hidden;
    transition: transform 0.2s, box-shadow 0.2s;
  }
  
  .custom-article-card:hover {
    transform: translateY(-2px);
    box-shadow: 0 8px 25px rgba(0,0,0,0.1);
  }
  
  .custom-article-content {
    padding: 30px;
  }
  
  .custom-article-title {
    font-size: 1.8em;
    margin: 0 0 15px 0;
    color: var(--blog-text);
  }
  
  .custom-article-meta {
    color: var(--blog-text-secondary);
    font-size: 0.9em;
    margin-bottom: 20px;
    display: flex;
    gap: 20px;
  }
  
  .custom-article-text {
    color: var(--blog-text);
    line-height: 1.8;
    margin-bottom: 25px;
  }
  
  .custom-article-text p {
    margin-bottom: 16px;
  }
  
  .custom-article-text h2 {
    font-size: 1.5em;
    margin: 30px 0 15px 0;
    color: var(--blog-text);
  }
  
  .custom-article-text h3 {
    font-size: 1.3em;
    margin: 25px 0 12px 0;
    color: var(--blog-text);
  }
  
  .custom-article-text ul {
    margin: 15px 0;
    padding-left: 25px;
  }
  
  .custom-article-text li {
    margin: 8px 0;
  }
  
  .custom-code-block {
    margin: 20px 0;
    border-radius: 10px;
    overflow: hidden;
    background: var(--blog-code-bg);
  }
  
  .custom-code-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 10px 15px;
    background: var(--blog-code-surface);
    border-bottom: 1px solid var(--blog-code-comment);
  }
  
  .custom-code-header span {
    color: var(--blog-code-text);
    font-family: var(--font-mono);
    font-size: 0.85em;
  }
  
  .custom-copy-btn {
    background: rgba(255,255,255,0.1);
    border: none;
    padding: 5px 12px;
    border-radius: 6px;
    color: var(--blog-code-text);
    cursor: pointer;
    font-family: var(--font-mono);
    font-size: 0.8em;
    transition: background 0.2s;
  }
  
  .custom-copy-btn:hover {
    background: rgba(255,255,255,0.2);
  }
  
  .custom-code-block pre {
    margin: 0;
    padding: 20px;
    overflow-x: auto;
  }
  
  .custom-code-block code {
    font-family: var(--font-mono);
    font-size: 0.85em;
    line-height: 1.6;
    color: var(--blog-code-text);
  }
  
  .custom-tag {
    display: inline-block;
    background: var(--blog-tag-bg);
    color: var(--blog-tag-text);
    padding: 4px 12px;
    border-radius: 20px;
    font-size: 0.8em;
    font-weight: 500;
    margin-right: 10px;
  }
  
  .custom-tags-container {
    margin: 20px 0 0 0;
  }
  
  @media (max-width: 768px) {
    .custom-banner-image {
      height: 200px;
    }
    
    .custom-banner-title {
      font-size: 1.5em;
    }
    
    .custom-article-content {
      padding: 20px;
    }
    
    .custom-article-title {
      font-size: 1.4em;
    }
  }
</style>

<div class="custom-blog-container">
  <!-- Banner Image -->
  <div class="custom-banner">
    <img src="/image_2.jpeg" alt="Blog Banner" class="custom-banner-image">
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
        <span>📅 January 15, 2024</span>
        <span>⏱️ 5 min read</span>
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

  <!-- Article 2 (Example of another post) -->
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
