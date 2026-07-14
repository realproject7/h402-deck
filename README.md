# giwa-gasok

Web assets for **Hunt Town's GASOK (GIWA) accelerator application**.

## Pages

- `index.html` — **Team dossier** (design concept: *Field Manifest*). A single static
  page introducing the team, submitted as the "Team introduction" link on the GASOK
  application form.

## Design

Dark **Blueprint** system inherited from `town-web-2` / h402: canvas `#0a0a0b`, single
coral accent `#fc6f6f`, Geist / Geist Mono, faint blueprint grid, soft coral top-glow.
Terminal / markdown-native aesthetic — reads like a builder's manifest. No build step,
no dependencies; fonts load from Google Fonts.

## Local preview

```bash
python3 -m http.server 8747
# → http://127.0.0.1:8747/
```

## Deploy (Vercel — static)

No framework. Import the repo in Vercel and set **Framework Preset: Other** (root
directory `/`, no build command, output = repo root). Vercel serves `index.html` at `/`.
