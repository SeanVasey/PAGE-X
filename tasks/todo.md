# Task Plan

## Session 3: Fix CI Dependencies & Add Deployment

- [x] Create `.markdownlint-cli2.jsonc` config file (fix inline config error)
- [x] Update `ci.yml`: upgrade actions/checkout v4→v6, markdownlint-cli2-action v19→v22, remove inline config
- [x] Add GitHub Pages deployment workflow (`deploy-pages.yml`)
- [x] Add Vercel deployment config (`vercel.json`)
- [x] Update CHANGELOG.md, README.md, docs/MANIFEST.md
- [x] Update tasks/lessons.md with CI config lessons
- [ ] Commit, push, and create PR

## Session 2: Core Application Implementation

- [x] Create `index.html` with full application (CSS + HTML + JS)
- [x] Fix critical CSS bug: EN DASH (U+2013) → double hyphens in all custom properties
- [x] Remove markdown code fence artifacts from HTML
- [x] Create `manifest.json` for PWA support
- [x] Create `sw.js` for offline caching
- [x] Update `README.md` with tech stack, usage instructions, project structure
- [x] Update `CHANGELOG.md` with new files and bug fixes
- [x] Update `docs/MANIFEST.md` with new file entries
- [x] Commit and push

## Session 1: Repository Scaffolding

- [x] Create `CLAUDE.md` with project standards and workflow guidelines
- [x] Create `tasks/` directory with `todo.md` and `lessons.md`
- [x] Create `CHANGELOG.md`, `SECURITY.md`, `CODE_OF_CONDUCT.md`
- [x] Create `.editorconfig`, `.gitignore`
- [x] Update `README.md` with full project documentation
- [x] Create GitHub Actions CI workflow
- [x] Create `docs/MANIFEST.md`

## Review

Session 3: Fixed broken CI pipeline (markdownlint config error, Node.js 20 deprecation). Added GitHub Pages and Vercel deployment support. All action versions upgraded to latest (checkout v6, markdownlint-cli2-action v22).
