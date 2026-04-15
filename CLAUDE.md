# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

Personal blog built with Jekyll using custom layouts (no external theme dependency).

## Commands

```bash
bundle exec jekyll serve   # Start local dev server at http://localhost:4000
bundle install             # Install Ruby dependencies (if Gemfile exists)
```

## Architecture

```
├── _config.yml        # Site config (title, description, social, permalinks)
├── _layouts/          # HTML templates
│   ├── default.html   # Base layout with header/nav/footer
│   ├── post.html      # Single post layout
│   └── posts.html     # Posts listing layout
├── _includes/         # Reusable partials (e.g., disqus.html)
├── _sass/             # SCSS partials (if using SCSS)
├── assets/css/        # Compiled CSS (main.css)
├── posts/             # Pages (posts/index.md)
├── _posts/            # Blog posts (YYYY-MM-DD-title.md format)
└── index.md           # Homepage
```

## Post Front Matter

```yaml
---
layout: post
title: "Post Title"
date: 2026-04-15
author: weiwei
tags: [tag1, tag2]
description: "Optional description"
---
```

## Notes

- Deploy target: `https://weiwei-geo.github.io`
- Permalink format: `/posts/:year/:month/:day/:title/`
- RSS feed auto-generated at `/feed.xml` (jekyll-feed plugin)
