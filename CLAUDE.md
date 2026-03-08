# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Personal blog/portfolio site for gianhiltbrunner.ch, built with Hugo. Content is primarily ramen recipes and cooking posts, book reviews, and an about page.

## Commands

```bash
# Local development (live reload)
hugo server

# Production build
hugo --gc --minify --baseURL "https://gianhiltbrunner.ch/"
```

There are no tests or linters. The CI pipeline (GitHub Actions) validates that the Hugo build succeeds on push to `main`.

## Architecture

- **Hugo static site** with the custom [Archie theme](https://github.com/gianhiltbrunner/archie) (git submodule in `themes/archie/`)
- **Configuration**: `hugo.toml` (TOML format)
- **Content**: Markdown files in `content/` with TOML frontmatter (`+++`)
  - `content/posts/` — blog posts (recipes, etc.)
  - `content/books/` — book recommendations page
  - `content/about/` — about page
- **Layouts**: Custom templates in `layouts/` override the theme
  - `layouts/index.html` — homepage with pinned posts support
  - `layouts/_default/single.html` and `list.html` — post templates
  - `layouts/books/single.html` — book gallery with responsive grid
  - `layouts/shortcodes/mermaid.html` — Mermaid diagram support
- **Custom CSS**: `assets/css/` (books.css, mermaid.css, pin.css) — referenced in `hugo.toml` under `[params]`
- **Static assets**: `static/` (favicons, book cover images)
- **LLM resources**: `llm_resources/` contains reference material (e.g., ramen cookbook (Book of Ramen))

## Content Conventions

- Posts use TOML frontmatter with: `title`, `description`, `date`, `tldr`, `draft`, `tags`, `pin`
- Setting `pin=true` in frontmatter pins a post to the top of the homepage
- Measurements in recipes use metric (grams, milliliters) with practical equivalents in parentheses
- Recipe posts follow a structure: intro → sources → bowl assembly → component sections with ingredients, explanation, and numbered steps

## Deployment

Automated via GitHub Actions (`.github/workflows/hugo.yaml`): push to `main` triggers build and deploy to GitHub Pages. Requires Hugo extended edition (0.152.2) with Dart Sass.