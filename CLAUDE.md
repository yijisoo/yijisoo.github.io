# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Jekyll Now-based GitHub Pages personal blog for Ji Soo Yi. Deploys automatically to GitHub Pages on push to master.

## Development Commands

```bash
# Local development server (http://127.0.0.1:4000/)
jekyll serve

# Build static site to _site/
jekyll build

# Install dependencies
gem install github-pages
```

## Architecture

- **Jekyll static site** using Kramdown (GFM) and Rouge syntax highlighting
- **Layouts** (`_layouts/`): `default.html` → `post.html` / `page.html` inheritance chain
- **Content**: Posts in `_posts/` (YYYY-MM-DD-title.md format), drafts in `_drafts/`, static pages at root (`about.md`, `404.md`)
- **Styling**: SCSS in `_sass/`, imported via `style.scss`. Variables defined in `_variables.scss`
- **Includes** (`_includes/`): analytics (Google), disqus comments, meta tags, social SVG icons
- **Config**: `_config.yml` controls site metadata, social links, plugins (jekyll-sitemap, jekyll-feed), permalink structure (`/:title/`)

## Content Conventions

- Posts use front matter: `layout: post`, `title: "..."`
- Pages use front matter: `layout: page`, `title: "..."`
- Content is a mix of English and Korean
- Navigation links ("About" and "Thoughts") are hardcoded in `_layouts/default.html`
