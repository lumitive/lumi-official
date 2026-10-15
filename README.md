# lumi-official

The Lumi Business marketing site. Static, single HTML file, no build step,
no framework — extracted from `lumi/apps/frontend/public/business/` so it
can ship on its own (GitHub Pages) instead of riding the main product's
deploy gate.

- **Source**: [`index.html`](index.html)
- **Fonts**: `fonts/` — D-DIN + IBM Plex Mono, self-hosted (see `fonts/COPYING.txt`)
- **Hosting**: GitHub Pages, served from the `main` branch root via the
  `Deploy static site` workflow (`.github/workflows/pages.yml`)
- **Editing**: this is the only source file. Edit `index.html` directly and
  push to `main` — Pages redeploys automatically, no server deploy, no gate.

Both Chinese (default) and English copy live side by side in the same
elements via `data-en` / `data-en-ph` attributes; see the comment block near
the top of `index.html` for how the language switch works.
