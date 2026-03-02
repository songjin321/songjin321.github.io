# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Academic personal website for Song Jin, hosted on GitHub Pages at `www.sjin.top`. Pure HTML/CSS/JS with no build tools, frameworks, or static site generators.

## Development

No build step required. To serve locally:

```bash
python -m http.server
```

Then open `http://localhost:8000` in a browser.

Deployment is automatic via GitHub Pages on push to `master`.

## Architecture

- `index.html` — Single-page site with fixed nav + anchor sections (About, News, Publications, Projects, Experience, Blog)
- `assets/css/style.css` — All styles; CSS custom properties design system, responsive breakpoints at 768px and 480px
- `assets/images/profile/` — Profile photo (`head.jpeg`)
- `assets/images/projects/` — Project images
- `assets/pdfs/` — PDF papers
- `CNAME` — Maps to custom domain `www.sjin.top`
- `.gitignore` — Ignores `.DS_Store` and `*.ppm` files

External dependencies (CDN): Google Fonts (Inter), Academicons (Google Scholar icon).

The page is structured as: nav → about → news → publications → projects (industry/research/competitions) → experience timeline → blog → footer.
