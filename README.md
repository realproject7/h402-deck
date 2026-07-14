# giwa-gasok

Web assets for **Hunt Town's GASOK (GIWA) accelerator application**.

## Pages (two design concepts — pick one to submit)

- `index.html` — **Field Manifest**. Dark **Blueprint** system inherited from
  `town-web-2` / h402: canvas `#0a0a0b`, single coral accent `#fc6f6f`, Geist /
  Geist Mono, blueprint grid, soft coral top-glow. Centered display hero.
- `editor.html` — **Editor (v3, current pick)**. Ulysses-dark markdown document, dark-matte
  gray + green accent, JetBrains Mono, KO/EN language toggle (default KO), media-rich core
  strengths, x402-on-GIWA diagram, chronological 19-entry timeline with thumbnails.
- `terminal.html` — **Terminal / TUI**. Monotone (grayscale + minimal terminal green),
  JetBrains Mono throughout, Hacker-News-builder aesthetic: a status line, `$` prompt
  section headers (`cat team.txt`, `ls -la track-record/`), `[NN]` records, an
  aligned data table, blinking caret. Left-aligned, information-dense.

Both are the same content (team intro + track record) submitted as the "Team
introduction" link on the GASOK application form.

## Design

No build step, no dependencies; fonts load from Google Fonts. Both pages share the
same copy source (`team-intro`) and only differ in visual concept.

## Local preview

```bash
python3 -m http.server 8747
# → http://127.0.0.1:8747/
```

## Deploy (Vercel — static)

No framework. Import the repo in Vercel and set **Framework Preset: Other** (root
directory `/`, no build command, output = repo root). Vercel serves `index.html` at `/`.
