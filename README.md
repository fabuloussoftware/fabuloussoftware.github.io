# Fabulous Software Website

This is the Jekyll-based website for Fabulous Software, Inc., a solo contract programming business by James Ehly.

## Setup Instructions

### For GitHub Pages Deployment

1. **Create a new repository** on your GitHub account named `jamesehly.github.io` (or `<username>.github.io`)

2. **Push this code** to the repository:
   ```bash
   git init
   git add .
   git commit -m "Initial commit: Jekyll site for Fabulous Software"
   git branch -M main
   git remote add origin https://github.com/jamesehly/jamesehly.github.io.git
   git push -u origin main
   ```

3. **Enable GitHub Pages**:
   - Go to repository Settings → Pages
   - Under "Source", select "GitHub Actions"
   - The site will automatically build and deploy when you push changes

4. **Access your site** at: `https://jamesehly.github.io`

### For Local Development

1. **Install Ruby and Bundler** (if not already installed)

2. **Install dependencies**:
   ```bash
   bundle install
   ```

3. **Run the site locally**:
   ```bash
   bundle exec jekyll serve
   ```

4. **View at**: `http://localhost:4000`

## File Structure

- `_config.yml` - Jekyll configuration
- `index.md` - Homepage content
- `blog.md` - Blog listing page
- `_posts/` - Blog posts (markdown files)
- `_layouts/` - Custom page layouts
- `_sass/` - Custom SCSS styles
- `assets/` - Images, brand assets, and compiled CSS

## Adding Blog Posts

Create new files in `_posts/` with the naming format: `YYYY-MM-DD-title.md`

Example:
```markdown
---
layout: post
title: "Your Post Title"
date: 2025-09-15 10:00:00 -0500
categories: category-name
excerpt: "Brief description of the post"
---

Your content here...
```

## Customization

- Brand colors are defined in `_sass/_fabulous.scss`
- Site settings in `_config.yml`
- Navigation links can be modified in `_config.yml` under `header_pages`

## Contact

For questions about this website setup, contact James Ehly at contact@fabsoft.io