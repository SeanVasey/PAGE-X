# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).

## [Unreleased]

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
