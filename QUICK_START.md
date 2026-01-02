# Quick Start Guide

## Adding a New Post

1. **Create a new file** in the `_posts/` directory
2. **Name it** using the format: `YYYY-MM-DD-title.md` (e.g., `2024-01-21-my-theorem.md`)
3. **Add front matter** at the top:

```markdown
---
layout: post
title: "Your Post Title"
date: 2024-01-21
categories: [Category1, Category2]
---

Your content here...
```

4. **Write your content** using Markdown and LaTeX

## LaTeX Syntax

- **Inline math**: `$formula$` or `\(formula\)`
- **Display math**: `$$formula$$` or `\[formula\]`

### Examples

```markdown
The quadratic formula is $x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}$.

$$
\int_{-\infty}^{\infty} e^{-x^2} \, dx = \sqrt{\pi}
$$
```

## Testing Locally

```bash
bundle exec jekyll serve
```

Then visit http://localhost:4000

## Deploying to GitHub Pages

1. Create a GitHub repository
2. Update `_config.yml` with your GitHub Pages URL
3. Push to GitHub:
   ```bash
   git remote add origin https://github.com/username/repo-name.git
   git push -u origin main
   ```
4. Enable GitHub Pages in repository settings

