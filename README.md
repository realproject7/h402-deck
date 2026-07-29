# h402 · Verified Agent Commerce on Arc

Build on Arc hackathon submission for **h402**.

h402 does not recreate an x402 facilitator or payment rail. It adds the decision
and evidence layer for agent commerce: a policy-bound provider choice, a USDC
payment reference, and an outcome receipt that can improve future routing.

## Included

- `index.html` — English-only team and product site.
- `deck.html` — English-only 12-slide Arc submission deck.
- `deck.pdf` — rendered submission PDF.
- `assets/deck/live-20260729/` — current product screenshots captured from
  `https://h402-test.hunt.town/` on 29 July 2026.

## Arc MVP

1. Define task scope, USDC cap, and provider eligibility in an agent policy.
2. Choose a provider through h402 and settle the call using the existing
   Circle Nanopayments/x402 payment primitive.
3. Anchor a decision receipt on Arc Testnet with the provider, quote, payment
   reference, and outcome hash.
4. Use ERC-8004 feedback for verified reputation and prototype an ERC-8183
   job path for conditional, higher-value work.

## Local preview

```bash
python3 -m http.server 8747
# http://127.0.0.1:8747/
```

## Vercel

The site is served as a static project with no build or install command.
The public production URL is `https://arc-hack-dun.vercel.app/`.
