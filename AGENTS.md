# AGENTS.md

## Cursor Cloud specific instructions

### Product overview
This repository is a single-file static personal portfolio / résumé website for
"Rachel Swimmer · Account Executive". The entire site lives in `index.html`
(HTML5 with inline CSS). There is **no** JavaScript, backend, database, build
step, package manager, or dependency manifest.

### Running the site (development)
There is no build step. Serve the single file with any static HTTP server, e.g.:

```bash
python3 -m http.server 8000   # run from repo root, then open http://localhost:8000/
```

Opening `index.html` directly via `file://` also works, but serving over HTTP is
preferred for accurate rendering.

### Fonts / network note
Typography is loaded from the Google Fonts CDN (`fonts.googleapis.com`). If the
VM has no outbound internet, the page still renders correctly using system
fallback fonts — this is expected and not a failure.

### Lint / test / build
None are configured. There is no linter, no test framework, and no build system.
"Testing" is manual/visual verification of `index.html` in a browser.
