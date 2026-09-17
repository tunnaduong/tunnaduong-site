# tunnaduong.com

A minimal personal website built with Astro.

## Getting started

```bash
npm install
npm run dev
```

## Build

```bash
npm run build
npm run preview
```

## Pages

- `/` - Home (tools I've made)
- `/about` - About me
- `/blog` - Blog posts (dynamically generated from markdown files)

## Blog Posts

Blog posts are stored as markdown files in `src/content/blog/`. Each post needs frontmatter with:

```yaml
---
title: Your post title
date: 2026-01-15
description: Optional brief description
---
```

### Adding a blog post

1. Create a new `.md` file in `src/content/blog/`:
   ```
   src/content/blog/my-new-post.md
   ```

2. Add frontmatter and content:
   ```markdown
   ---
   title: My New Post
   date: 2026-09-17
   description: A brief description
   ---

   Your markdown content here...
   ```

3. The post will automatically appear on `/blog` and be accessible at `/blog/my-new-post`

### Removing a blog post

Simply delete the `.md` file from `src/content/blog/` and it will disappear from the blog.

### Pushing to GitHub

Commit your markdown files and push to GitHub. The blog will update automatically when you redeploy.

```bash
git add src/content/blog/*.md
git commit -m "Add new blog post"
git push
```

## Design

Minimal, responsive design with system fonts. All styles are defined in the Layout component.
