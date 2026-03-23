<p align="center">
  <img src="icon-512.png" alt="PAGE•X logo — cyan document icon with page extraction arrows" width="128" height="128">
</p>

<h1 align="center">PAGE•X</h1>

<p align="center">
  Extract, paginate, and format oversized images, scrolling screenshots, and PDFs into standard printable pages.
</p>

<p align="center">
  <a href="https://github.com/SeanVasey/PAGE-X/actions/workflows/ci.yml"><img src="https://github.com/SeanVasey/PAGE-X/actions/workflows/ci.yml/badge.svg" alt="CI status"></a>
  <a href="https://github.com/SeanVasey/PAGE-X/actions/workflows/deploy-pages.yml"><img src="https://github.com/SeanVasey/PAGE-X/actions/workflows/deploy-pages.yml/badge.svg" alt="Deploy status"></a>
  <a href="LICENSE"><img src="https://img.shields.io/badge/license-Apache%202.0-blue.svg" alt="License: Apache 2.0"></a>
  <a href="https://seanvasey.github.io/PAGE-X/"><img src="https://img.shields.io/badge/demo-live-brightgreen.svg" alt="Live demo"></a>
</p>

-----

## Demo

**[Launch PAGE•X →](https://seanvasey.github.io/PAGE-X/)**

<!-- TODO(#1): Add hero screenshot showing the app in use once UI is finalized -->

-----

## Features

- Upload long/scrolling screenshots, images (PNG, JPG, WEBP), or PDFs
- Paginate into US Letter or A4 page format
- Export as PDF or DOCX
- Configurable safe margins, page numbers, and page overlap
- Client-side only — no server uploads, files never leave your browser
- PWA-enabled — installable, works offline after first load
- Responsive, mobile-friendly dark UI with cyan-teal accent palette

## Tech Stack

| Layer           | Technology                                            |
| --------------- | ----------------------------------------------------- |
| Frontend        | Vanilla HTML, CSS, JavaScript (no build step)         |
| PDF Generation  | [jsPDF](https://github.com/parallax/jsPDF) v2.5.1    |
| PDF Parsing     | [pdf.js](https://github.com/mozilla/pdfjs-dist) v3.11.174 |
| DOCX Generation | [docx](https://github.com/dolanmiu/docx) v8.5.0      |
| Fonts           | Google Fonts (Bebas Neue, Reddit Sans, Space Mono)    |
| CDN             | jsDelivr (runtime dependencies)                       |
| CI              | GitHub Actions (markdown lint + link check)           |
| Hosting         | GitHub Pages + Vercel                                 |

## Getting Started

No build step required. Open `index.html` directly or serve with any static file server:

```bash
# Option 1: Open directly
open index.html

# Option 2: Python
python3 -m http.server 8000

# Option 3: Node
npx serve .
```

Then navigate to `http://localhost:8000` (if using a server).

## Usage

1. **Upload** — Drop or tap to upload an image (PNG, JPG, WEBP), PDF, or DOCX
2. **Configure** — Select output format (PDF/DOCX), page size (Letter/A4), margins, page numbers, and overlap
3. **Process** — Click "Extract & Paginate"
4. **Download** — Save the paginated output

## Deployment

### GitHub Pages

Pushes to `main` automatically deploy via the `deploy-pages.yml` workflow. Enable Pages in your repository settings under **Settings → Pages → Source → GitHub Actions**.

### Vercel

Import the repository into Vercel. The included `vercel.json` handles static site configuration — no build command or framework selection needed.

## Project Structure

```text
PAGE-X/
├── .github/workflows/       # CI + GitHub Pages deployment
├── docs/                     # Documentation and manifests
├── tasks/                    # Task tracking (todo.md, lessons.md)
├── index.html                # Core web application
├── manifest.json             # PWA manifest
├── sw.js                     # Service worker for offline support
├── vercel.json               # Vercel deployment configuration
├── icon.svg                  # App icon (SVG)
├── icon-192.png              # PWA icon 192×192
├── icon-512.png              # PWA icon 512×512
├── apple-touch-icon.png      # iOS home screen icon
├── CLAUDE.md                 # AI assistant conventions
├── CHANGELOG.md              # Change log
├── CODE_OF_CONDUCT.md        # Contributor code of conduct
├── LICENSE                   # Apache License 2.0
├── README.md                 # This file
└── SECURITY.md               # Vulnerability reporting policy
```

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feat/your-feature`)
3. Commit using [Conventional Commits](https://www.conventionalcommits.org/) (`feat:`, `fix:`, etc.)
4. Open a pull request

Please read [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md) before contributing.

## Security

See [SECURITY.md](SECURITY.md) for reporting vulnerabilities.

## License

Licensed under the [Apache License 2.0](LICENSE).

A [VASEY/AI](https://vasey.ai) production. © 2026 [VASEY Multimedia](https://vaseymultimedia.com).
