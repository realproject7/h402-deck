# h402 · AI Capability Market on Arc

Build on Arc hackathon submission for **h402**.

Mount h402 once and an agent gets the whole capability catalog: one call path
per capability, a pinned default provider per route, and pay-per-call USDC
settlement on Arc through h402's self-hosted facilitator. No API keys, no
plans, no subscriptions.

## Included

- `index.html` — English-only team and product site.
- `deck.pdf` — 16-page submission deck (the deliverable; `deck.html` redirects
  to it).
- `assets/deck/live-20260729/` — product screenshots captured from
  `https://h402-test.hunt.town/` on 29 July 2026.

## What runs today

- Live capability market at `https://h402-test.hunt.town/` — 141 capabilities,
  71 provider contracts, 100% paid-tested (live catalog, 6 Aug 2026).
- x402 pay-per-call on Arc Testnet: USDC quotes, local EIP-3009 signing,
  per-call spend caps.
- Self-hosted Arc facilitator; settlements visible on Arc Explorer
  (chain 5042002).

## Roadmap

1. h402 mainnet launch on Arc Mainnet day (Sep 16, 2026).
2. 300+ capabilities by end of 2026.
3. Nanopayments (Circle's gas-free batched USDC on Arc) for sub-$0.0001
   pricing.
4. Onchain decision receipts and ERC-8004 provider reputation.

## Local preview

```bash
python3 -m http.server 8747
# http://127.0.0.1:8747/
```

## Vercel

The site is served as a static project with no build or install command.
The public production URL is `https://arc-hack-dun.vercel.app/`.
