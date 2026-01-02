# Math Journal

A personal mathematics journal built with Jekyll, designed to be hosted on GitHub Pages. This journal supports LaTeX rendering via MathJax and makes it easy to add new mathematical content.

## Features

- ✅ **LaTeX Support**: Full LaTeX rendering using MathJax
- ✅ **Easy Content Creation**: Simply add markdown files to `_posts/`
- ✅ **GitHub Pages Ready**: Works out of the box with GitHub Pages
- ✅ **Clean Design**: Modern, readable layout optimized for mathematical content
- ✅ **Responsive**: Works on desktop and mobile devices

## Getting Started

### Local Development

1. **Install Ruby and Jekyll** (if not already installed):
   ```bash
   gem install bundler jekyll
   ```

2. **Install dependencies**:
   ```bash
   bundle install
   ```

3. **Run the development server**:
   ```bash
   bundle exec jekyll serve
   ```

4. **View your site**: Open [http://localhost:4000](http://localhost:4000) in your browser

### Adding New Posts

To add a new post to your math journal:

1. Create a new markdown file in the `_posts/` directory
2. Name it using the format: `YYYY-MM-DD-title.md`
3. Add front matter at the top:

```markdown
---
layout: post
title: "Your Post Title"
date: 2024-01-21
categories: [Category1, Category2]
---

Your content here...
```

4. Use LaTeX syntax:
   - Inline math: `$formula$` or `\(formula\)`
   - Display math: `$$formula$$` or `\[formula\]`

### Example Post

```markdown
---
layout: post
title: "The Fundamental Theorem of Calculus"
date: 2024-01-21
categories: [Calculus, Analysis]
---

## Theorem

If $f$ is continuous on $[a,b]$ and $F$ is an antiderivative of $f$, then:

$$\int_a^b f(x) \, dx = F(b) - F(a)$$

### Proof

[Your proof here...]
```

## Deploying to GitHub Pages

1. **Create a GitHub repository** (or use this one)

2. **Update `_config.yml`**:
   - If using `username.github.io`, set `url: "https://username.github.io"` and `baseurl: ""`
   - If using a project repository, set `url: "https://username.github.io"` and `baseurl: "/repository-name"`

3. **Push to GitHub**:
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/username/repository-name.git
   git push -u origin main
   ```

4. **Enable GitHub Pages**:
   - Go to your repository settings
   - Navigate to "Pages"
   - Select the source branch (usually `main`)
   - Select the folder (usually `/ (root)`)
   - Click Save

5. **Your site will be live** at `https://username.github.io` (or `https://username.github.io/repository-name`)

## Customization

- **Styling**: Edit `assets/css/style.css` to customize the appearance
- **Navigation**: Update the `navigation` section in `_config.yml`
- **Layout**: Modify the layout files in `_layouts/`

## LaTeX Examples

### Inline Math
```
The quadratic formula is $x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}$.
```

### Display Math
```
$$
\int_{-\infty}^{\infty} e^{-x^2} \, dx = \sqrt{\pi}
$$
```

### Complex Expressions
```
$$
\begin{align}
\nabla \times \mathbf{F} &= \begin{vmatrix}
\mathbf{i} & \mathbf{j} & \mathbf{k} \\
\frac{\partial}{\partial x} & \frac{\partial}{\partial y} & \frac{\partial}{\partial z} \\
F_x & F_y & F_z
\end{vmatrix}
\end{align}
$$
```

## License

Feel free to use this template for your own math journal!

