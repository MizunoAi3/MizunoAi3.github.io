---
layout: default
title: Home
---

<section class="hero">
  <h2>欢迎来到 {{ site.title }}</h2>
  <p class="lead">分享 AI、工程、学习笔记 — 使用 GitHub Pages 自动发布。</p>
  <div class="search">
    <input placeholder="搜索文章（示例）" aria-label="search">
  </div>
</section>

<section>
  <h3>最新文章</h3>
  <div class="posts-grid">
    {% for post in site.posts %}
      <article class="post-card">
        <a class="post-link" href="{{ post.url | relative_url }}">
          <h3>{{ post.title }}</h3>
          <p class="meta">{{ post.date | date: "%Y-%m-%d" }}</p>
          <p>{{ post.excerpt | strip_html | truncate: 120 }}</p>
        </a>
      </article>
    {% endfor %}
  </div>
</section>

<p style="margin-top:1.25rem">写新的文章：在 <code>_posts/</code> 中创建 Markdown，命名为 <code>YYYY-MM-DD-your-title.md</code> 并添加 front matter。</p>
