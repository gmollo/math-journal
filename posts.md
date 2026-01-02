---
layout: page
title: Posts
---

# All Posts

<ul class="posts-list">
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | relative_url }}" class="post-link">{{ post.title }}</a>
      <p class="post-meta">{{ post.date | date: "%B %d, %Y" }}</p>
      {% if post.categories.size > 0 %}
        <p class="post-categories">
          {% for category in post.categories %}
            <span class="category-tag">{{ category }}</span>
          {% endfor %}
        </p>
      {% endif %}
      {% if post.excerpt %}
        <p class="post-excerpt">{{ post.excerpt }}</p>
      {% endif %}
    </li>
  {% endfor %}
</ul>

