# Fabulous Software Website

This is the Jekyll-based website for Fabulous Software, Inc.

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