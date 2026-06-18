# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

This is a personal academic website for Yuxin Yao, built on the [academicpages](https://github.com/academicpages/academicpages.github.io) template — a fork of the Minimal Mistakes Jekyll theme. It is hosted on GitHub Pages at `https://YuxinYao620.github.io`.

## Local Development

```bash
# Install dependencies (first time)
bundle install

# Serve locally with live reload (recommended)
bundle exec jekyll liveserve

# Serve with dev config overrides (disables analytics/comments)
bundle exec jekyll liveserve --config _config.yml,_config.dev.yml
```

The site is served at `http://localhost:4000`. Changes to most files rebuild automatically; changes to `_config.yml` require a server restart.

## Site Architecture

### Content Collections

Content lives in these directories and maps to URL paths:

| Directory | URL path | Purpose |
|---|---|---|
| `_pages/` | varies (set by `permalink`) | Static pages (about, cv, etc.) |
| `_publications/` | `/publications/:filename/` | Research papers |
| `_talks/` | `/talks/:filename/` | Conference talks |
| `_teaching/` | `/teaching/:filename/` | Teaching entries |
| `_posts/` | `/:categories/:title/` | Blog posts |
| `_portfolio/` | `/portfolio/:filename/` | Portfolio items |

### Key Files

- `_pages/about.md` — Homepage (permalink: `/`). This is the primary page to edit for research content; it contains inline HTML for the project cards layout.
- `_config.yml` — Site-wide config: author profile, social links, site metadata, collection/layout defaults.
- `_data/navigation.yml` — Top navigation bar links.
- `files/` — PDFs and media assets (CV, paper images, GIFs) served at `/files/`.

### Layouts and Includes

- `_layouts/` — Page layout templates (archive, compress)
- `_includes/` — Reusable HTML partials (author profile sidebar, head, masthead, etc.)
- `_sass/` — SCSS stylesheets

### Front Matter Defaults

Defaults are set in `_config.yml` under `defaults`. Each collection has its own default layout:
- Posts: `single` layout, with author profile, read time, comments, share
- Pages: `single` layout, with author profile
- Talks: `talk` layout, with author profile and share

## Content Conventions

### Adding a Project to the Homepage

Projects on `_pages/about.md` use a flex-based HTML layout with the `.project-pub` CSS class defined inline at the top of the file. Each project block follows this pattern:

```html
<div class="project-pub">
  <img src="../files/image.jpg" alt="Project title" />
  <div class="body">
    <h3 class="title"><a href="URL">Title</a></h3>
    <p class="meta">Authors</p>
    <p class="meta">Venue/Year</p>
    <p class="links"><a href="#">Paper</a> / <a href="#">GitHub</a></p>
    <p class="tldr"><strong>TLDR:</strong> Description.</p>
  </div>
</div>
```

### CV / PDF

The CV PDF is linked directly in `_data/navigation.yml` (currently `files/YuxinYaoCV2026.pdf`). Update this path when replacing the CV file.

### Collection Entries

Each file in `_publications/`, `_talks/`, etc. uses YAML front matter. The `_pages/cv.md` uses Liquid loops (`{% for post in site.publications %}`) to auto-populate CV sections from these collections.
