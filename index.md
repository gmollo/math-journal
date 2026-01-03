---
layout: default
title: Home
---

<div class="hero-section">
  <h1 class="hero-title">Covering space</h1>
  <p class="hero-subtitle">Mathematical explorations, proofs, and insights</p>
</div>

<div class="recent-posts-section">
  <h2 class="section-title">Recent Posts</h2>
  <div class="posts-grid">
    {% for post in site.posts limit:6 %}
    <article class="post-card">
      <div class="post-card-header">
        <time class="post-date">{{ post.date | date: "%B %d, %Y" }}</time>
        {% if post.categories.size > 0 %}
        <div class="post-categories">
          {% for category in post.categories limit:2 %}
            <span class="category-tag">{{ category }}</span>
          {% endfor %}
        </div>
        {% endif %}
      </div>
      <h3 class="post-card-title">
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      </h3>
      {% if post.excerpt %}
      <p class="post-card-excerpt">{{ post.excerpt | strip_html | truncatewords: 20 }}</p>
      {% endif %}
      <a href="{{ post.url | relative_url }}" class="post-card-link">Read more →</a>
    </article>
    {% endfor %}
  </div>
  <div class="view-all-link">
    <a href="{{ '/posts' | relative_url }}" class="btn-primary">View All Posts</a>
  </div>
</div>
