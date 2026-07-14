# giwa-gasok

Team dossier for **h402's GASOK (GIWA accelerator) application**, submitted as the
"Team introduction" link on the application form.

## What's here

- `index.html` — the dossier. A single static page, no build step, no dependencies
  (system fonts only). EN/KO language toggle in the top bar (default EN, choice saved
  in localStorage). Sections: intro + Upbit-hackathon proof, core strengths (with
  handshake diagram, product shot, team avatars), what we build on GIWA (x402 flow
  diagram), members, main projects, and a chronological 2018 → now track record.
- `assets/` — member avatars and project screenshots (downscaled from `town-web-2`).

Earlier design concepts (Field Manifest, Terminal/TUI) were moved out of the repo to
`~/Projects/z-others/giwa-gasok-archive/`.

## Local preview

```bash
python3 -m http.server 8747
# → http://127.0.0.1:8747/
```

## Deploy (Vercel, static)

1. Vercel → Add New → Project → Import `realproject7/giwa-gasok`
2. Framework Preset: **Other** · no build command · root directory `/`
3. Deploy. `index.html` is served at `/`.

Make sure Deployment Protection / Vercel Authentication is **off** so reviewers can
open the link without logging in.
