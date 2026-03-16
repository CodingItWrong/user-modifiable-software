# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Commands

```bash
bundle install       # Install dependencies (requires Ruby 3.1.2)
bin/serve            # Run local development server (bundle exec jekyll serve)
```

## Architecture

This is a Jekyll static site using the `minima` theme, deployed to GitHub Pages at `user-modifiable.codingitwrong.com`. The site is an essay examining Smalltalk and HyperCard as user-modifiable software systems.

**Content structure:** The essay is organized as top-level pages (`introduction.md`, `conclusion.md`, `bibliography.md`, `ted.md`) plus two subdirectories (`smalltalk/`, `hypercard/`) each containing the same five sections: `motivation.md`, `properties.md`, `impact.md`, `challenges.md`, `competitors-and-successors.md`. The `index.md` uses the `home` layout and serves as the table of contents.

**Theme customizations** (overriding `minima`):
- `_layouts/page.html` — custom page layout
- `_includes/head.html`, `header.html`, `google-analytics.html` — custom includes
- `assets/custom.css` — style overrides

**Deployment:** The `github-pages` branch is what gets served. Content changes go to `main`; the GitHub Pages branch tracks separately.

**`scratch-pad.md`** is excluded from the Jekyll build (see `_config.yml`) and is used for work-in-progress notes.
