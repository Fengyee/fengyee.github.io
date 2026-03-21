# Repository Guidelines

## Project Structure & Module Organization
- Core content lives in `content/` (pages, posts, and section indexes with YAML/TOML front matter). Authors live under `content/authors/`, and media referenced in Markdown should be stored in `static/` or `assets/` (for pipeline-processed files).
- Site-wide configuration sits in `config/_default/` and `hugoblox.yaml`. Theme/layout overrides belong in `layouts/`.
- Build outputs: `public/` is generated; `resources/` caches Hugo assets; avoid manual edits in either directory.
- Data helpers: `publications.bib` feeds publication blocks; `hugo_stats.json` supports purge/tree-shaking.

## Build, Test, and Development Commands
- `hugo server --disableFastRender`: Run the local dev server at `http://localhost:1313` with live reload; use when editing content or layouts.
- `hugo --gc --minify -b http://localhost:1313`: Production-style build with garbage collection and minification; mirrors Netlify’s build minus `pagefind`.
- `hugo --gc --minify -b $URL && npx pagefind --source 'public'`: Full release build (matches `netlify.toml`); ensure `npm` is available for `pagefind`.
- If modules are outdated, run `hugo mod get -u` to refresh Hugo Blox dependencies.

## Coding Style & Naming Conventions
- Front matter: prefer YAML with 2-space indentation; quote strings with punctuation or leading numbers. Use ISO dates (`2024-09-15`).
- File naming: kebab-case for pages/sections (e.g., `data-science.md`), lowercase image names with hyphens.
- Content: write in Markdown, lean on Hugo Blox shortcodes/blocks, and keep headings hierarchical. Avoid editing generated `public/` or `resources/` files.
- CSS/JS overrides go in `assets/` (processed) or `static/` (served as-is); keep Tailwind-friendly class names where possible.

## Testing Guidelines
- Primary verification is a clean Hugo build: run the production command above before proposing changes. Fix any front-matter or missing-content warnings.
- Spot-check critical pages (home, posts, projects, publications) in the dev server for broken links, images, and block rendering.
- For search, ensure `npx pagefind --source 'public'` completes without errors after a production build.

## Commit & Pull Request Guidelines
- Commit messages follow short, imperative phrases seen in history (`fix typo`, `update resume`). Group related edits; avoid noisy generated diffs.
- Before opening a PR: summarize intent, list major pages touched, and note any visual changes (screenshots/gifs welcome). Link related issues or TODOs if applicable.
- Exclude `public/` and other generated artifacts from manual edits unless the workflow requires them; keep diffs focused on source content and configuration.
