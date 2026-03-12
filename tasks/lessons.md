# Lessons Learned

Accumulated patterns from corrections and mistakes. Review at the start of each session.

---

## CI / GitHub Actions

1. **markdownlint-cli2-action does not support inline `config` YAML.** The `config` parameter expects a file path, not embedded JSON. Always use a dedicated config file (`.markdownlint-cli2.jsonc`) in the repo root.

2. **Pin GitHub Actions to current major versions.** Node.js 20 is deprecated (EOL April 2026, forced to Node.js 24 starting June 2026). Use `actions/checkout@v6` and `markdownlint-cli2-action@v22` or later. Check action release pages before adding to workflows.

3. **lychee-action is a Rust binary action** — not affected by Node.js runtime deprecations. `@v2` remains current.
