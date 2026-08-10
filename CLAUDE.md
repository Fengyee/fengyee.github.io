# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What This Is

A personal academic website for Haoan Feng (PhD student at UMD), built with [Hugo](https://gohugo.io/) and the [Hugo Blox](https://hugoblox.com/) (formerly Wowchemy) framework.

**Deployment:** the live site at <https://fengyee.github.io/> is built and published by GitHub Actions (`.github/workflows/publish.yaml`) on every push to `main`, using Hugo **0.140.0**. `netlify.toml` and `hugoblox.yaml` still declare `0.126.3`, but Netlify is not the live deploy path — treat `publish.yaml` as the authority.

**Local Hugo:** use the vendored `./bin/hugo` (0.140.0, matching CI). Newer Hugo releases break this site's Hugo Blox modules, so do not upgrade or fall back to a system-installed `hugo`.

## Commands

```bash
# Local dev server with live reload
hugo server --disableFastRender

# Production-style build (mirrors Netlify, minus pagefind)
hugo --gc --minify -b http://localhost:1313

# Full release build (matches netlify.toml exactly)
hugo --gc --minify -b $URL && npx pagefind --source 'public'

# Update Hugo Blox module dependencies
hugo mod get -u
```

No test suite exists. Verification is a clean `hugo` build with no warnings, followed by spot-checking pages in the dev server.

## Architecture

### Content model

All site content lives in `content/` as Markdown with YAML front matter:

- `content/_index.md` — Homepage, assembled from Hugo Blox "blocks" (resume-biography-3, markdown, collection). This is where the landing page sections (News, Publications, Presentations) are configured.
- `content/authors/Haoan Feng/_index.md` — The primary author profile: bio, social links, education, work, awards, skills. This is the main biographical data store.
- `content/publication/<slug>/index.md` — One directory per paper; front matter drives the publication card (title, authors, date, abstract, tags, links, `featured`).
- `content/event/<slug>/index.md` — Conference talks and presentations.
- `content/project/<slug>/index.md` — Project showcases.
- `content/experience.md`, `content/services.md`, `content/projects.md` — Standalone pages for CV-style sections.
- `content/teaching/` — Teaching materials (e.g., JS tutorial).

### Configuration

All Hugo config is in `config/_default/`:
- `hugo.yaml` — Site title, base URL, taxonomies, build settings.
- `params.yaml` — Appearance (light mode, sky color), SEO, navbar, footer, math rendering.
- `menus.yaml` — Top navigation links and their weights.
- `languages.yaml` — Language settings.
- `module.yaml` — Hugo module imports (blox-plugin-netlify, blox-tailwind).

`hugoblox.yaml` at the repo root pins the Hugo version for Hugo Blox.

### Overrides

- `layouts/partials/` — Custom partial templates that override Hugo Blox defaults (hooks and views subdirectories).
- `assets/css/` — Custom CSS overrides (Tailwind-compatible).
- `assets/media/` — Profile images, icons, and other pipeline-processed media.
- `static/` — Files served as-is (e.g., PDFs like CV, poster files referenced directly in front matter with `url_poster`).

### Generated / do not edit

- `public/` — Local build output. Gitignored and **not** tracked; GitHub Actions rebuilds it on deploy. The copy on disk may be stale (e.g. baked with a `localhost:1313` baseURL) — never read it to check what the live site says; fetch <https://fengyee.github.io/> instead.
- `resources/` — Hugo asset cache.
- `hugo_stats.json` — Used for CSS purging; regenerated on build.

## Content conventions

- Front matter: YAML, 2-space indentation, ISO dates (`2024-09-15`).
- File/directory naming: kebab-case.
- Publication PDFs (posters, slides) go in the same directory as `index.md` and are referenced relatively in front matter (`url_poster: 'file.pdf'`).
- Custom SVG icons for skills/hobbies go in `assets/media/icons/`.
- The `publications.bib` at repo root is a bibliography file (not directly consumed by Hugo builds, kept for reference).
