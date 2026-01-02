---
layout: default
title: Home
---

# Welcome to My Math Journal

This is my personal mathematics journal where I document mathematical explorations, proofs, and insights.

## Recent Posts

{% for post in site.posts limit:5 %}
- **[{{ post.title }}]({{ post.url | relative_url }})** - {{ post.date | date: "%B %d, %Y" }}
{% endfor %}

[View all posts →]({{ '/posts' | relative_url }})

