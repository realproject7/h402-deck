# h402 · AI Capability Market on Base

Pitch deck and product site for **h402**.

Mount h402 once and an agent gets the whole capability catalog: one call path
per capability, a pinned default provider per route, and pay-per-call USDC
settlement on Base. No API keys, no plans, no subscriptions.

## Included

- `index.html` — English-only team and product site.
- `deck.pdf` — 16-page deck (the deliverable; `deck.html` redirects to it).
- `assets/deck/live-20260729/` — product screenshots captured from
  `https://h402-test.hunt.town/`.

## What runs today

- Live capability market at `https://h402-test.hunt.town/` — 141 capabilities,
  71 provider contracts, 100% paid-tested (live catalog, 3 Sep 2026).
- x402 pay-per-call on Base Mainnet: USDC quotes, local EIP-3009 signing,
  per-call spend caps.
- Buyer payments settle into the h402 treasury through the Coinbase CDP x402
  facilitator; providers are paid over Base x402, or Tempo MPP when a
  candidate has no Base x402 rail.

## Roadmap

1. Public launch: production domain plus a published toolkit.
2. 300+ paid-verified capabilities by end of 2026.
3. Circle Gateway Nanopayments for batched sub-cent calls.
4. Portable, ERC-8004-compatible provider reputation from paid-call outcomes.

## Deck build

Source of truth is `/Users/cho/Projects/z-others/h402-deck/deck-v2/` (design
assets stay out of this repo). Read `.agent-history/DECK-PDF-PLAYBOOK.md`
before touching the PDF, then from that directory:

```bash
node render-deck.mjs      # renders/dNN.png at 2x + overflow check
node export-pdf.mjs       # deck-v2.pdf, vector master, never shipped
python build-raster.py    # deck-final.pdf, full-raster + linearized
cp deck-final.pdf <this repo>/deck.pdf
```

## Local preview

```bash
python3 -m http.server 8747
# http://127.0.0.1:8747/
```

## Vercel

The site is served as a static project with no build or install command.
Canonical URL: `https://h402-deck.vercel.app/` (deck at `/deck.pdf`).
The old `arc-hack-dun.vercel.app` alias still resolves to the same deployment.
