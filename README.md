# PAGE-X

**PAGE•X** is a client-side web tool that extracts, paginates, and formats oversized images, scrolling screenshots, and PDFs into standard, printable A4/Letter page documents.

[![CI](https://github.com/SeanVasey/PAGE-X/actions/workflows/ci.yml/badge.svg)](https://github.com/SeanVasey/PAGE-X/actions/workflows/ci.yml)

## Features

- Upload long/scrolling screenshots, images, or PDFs
- Paginate into US Letter or A4 page format
- Export as PDF or DOCX
- Configurable safe margins, page numbers, and page overlap
- Client-side only — no server uploads, files never leave your browser
- PWA-enabled — installable, works offline after first load
- Responsive, mobile-friendly dark UI

## Tech Stack

- **Frontend**: Vanilla HTML, CSS, JavaScript (no build step)
- **PDF Generation**: [jsPDF](https://github.com/parallax/jsPDF) v2.5.1
- **PDF Parsing**: [pdf.js](https://mozilla.github.io/pdf.js/) v3.11.174
- **DOCX Generation**: [docx](https://github.com/dolanmiu/docx) v8.2.3
- **Fonts**: Google Fonts (Bebas Neue, Reddit Sans, Space Mono)

## Getting Started

No build step required. Open `index.html` directly in a browser, or serve it with any static file server:

```bash
# Option 1: Open directly
open index.html

# Option 2: Serve with Python
python3 -m http.server 8000

# Option 3: Serve with Node
npx serve .
```

Then navigate to `http://localhost:8000` (if using a server).

## Usage

1. **Upload** — Drop or tap to upload an image (PNG, JPG, WEBP), PDF, or DOCX
2. **Configure** — Select output format (PDF/DOCX), page size (Letter/A4), margins, page numbers, and overlap
3. **Process** — Click "Extract & Paginate"
4. **Download** — Save the paginated output

## Project Structure

```
PAGE-X/
├── .github/workflows/   # CI/CD pipelines
├── docs/                 # Documentation and manifests
├── tasks/                # Task tracking (todo.md, lessons.md)
├── index.html            # Core web application
├── manifest.json         # PWA manifest
├── sw.js                 # Service worker for offline support
├── CLAUDE.md             # AI assistant conventions
├── CHANGELOG.md          # Change log
├── CODE_OF_CONDUCT.md    # Contributor code of conduct
├── LICENSE               # Apache License 2.0
├── README.md             # This file
└── SECURITY.md           # Vulnerability reporting policy
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
