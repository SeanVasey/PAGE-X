# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).

## [Unreleased]

### Fixed

- CI workflow reliability: corrected `actions/checkout` from invalid `v6` to supported `v4` in CI and Pages workflows
- PWA install/runtime stability: removed cross-origin CDN URLs from service worker pre-cache list to prevent install failures
- Runtime dependency loading: switched browser script CDNs to stable jsDelivr package URLs and aligned PDF worker path

### Added

- `index.html` — Core web application with image/PDF/DOCX pagination
- `manifest.json` — PWA manifest for installability
- `sw.js` — Service worker for offline caching
- Repository scaffolding with full project structure
- `CLAUDE.md` — AI assistant conventions and project standards
- `CHANGELOG.md`, `SECURITY.md`, `CODE_OF_CONDUCT.md`
- `tasks/` directory for task tracking (`todo.md`, `lessons.md`)
- `.editorconfig` and `.gitignore`
- GitHub Actions CI workflow for markdown linting
- Expanded `README.md` with project overview, tech stack, and usage instructions
- `docs/MANIFEST.md` — file manifest

### Fixed

- CSS custom properties: replaced EN DASH (U+2013) with correct double hyphens in all declarations and var() references
- Removed markdown code fence artifacts from HTML template
- Fixed broken docx library link in README (`dolanminda` → `dolanmiu`)
- Added `.lycheeignore` to prevent CI failures on owner-controlled external sites
- Markdownlint CI failure: moved inline config to `.markdownlint-cli2.jsonc` file (inline `config` parameter not supported)
- Node.js 20 deprecation warnings: upgraded `markdownlint-cli2-action` v19 → v22

### Added (CI/Deployment)

- `.markdownlint-cli2.jsonc` — external markdownlint configuration
- `.github/workflows/deploy-pages.yml` — GitHub Pages deployment workflow
- `vercel.json` — Vercel static site deployment configuration
