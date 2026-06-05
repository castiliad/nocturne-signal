# Nocturne Signal

A dark techno-oracle GitHub Pages site for presenting projects, agent workflows, artifacts, and operating principles with verified static-site boundaries.

## Brief
Create a dark, edgy, technical GitHub Pages static site for a personal AI/operator lab. It should feel like a techno-oracle command center: xAI-style monochrome restraint, Linear-level precision, VoltAgent terminal energy, and one signature kinetic typography / pretext-inspired hero. It must remain static, public-safe, no analytics, no tracking, no fake metrics, and no fabricated endorsements.

## Recipe registry
Selected recipes:
- product-cockpit
- artifact-gallery
- search-index
- agent-run-ledger
- copy-evidence-strip

Visual preset: `cockpit-dark`

auto_recipe_selection: not requested; default recipe selection unchanged

Auto-selection signals:
- No auto-selection signals recorded

Registry commands:
```bash
npm run list:recipes
npm run score:recipes
npm run recommend:recipes -- --brief "Create a dark, edgy, technical GitHub Pages static site for a personal AI/operator lab. It should feel like a techno-oracle command center: xAI-style monochrome restraint, Linear-level precision, VoltAgent terminal energy, and one signature kinetic typography / pretext-inspired hero. It must remain static, public-safe, no analytics, no tracking, no fake metrics, and no fabricated endorsements."
```

## Audience
- Technical collaborators reviewing AI/operator experiments
- Hiring or project leads who need a credible technical signal without marketing fluff
- Future agents maintaining the site from contracts, QA gates, and deploy evidence

## Live URL
https://castiliad.github.io/nocturne-signal/

## Repository
https://github.com/castiliad/nocturne-signal

## Local development
```bash
npm install
npm run dev
```

## QA
`npm run qa` is the fast local gate. Browser/mobile visual QA is explicit so normal edits stay quick.

## Recipe-enabled generation
Selecting `recipes: ["product-cockpit"]`, `visualPreset: "cockpit-dark"`, or `visualPreset: "product-cockpit"` renders the cockpit UI template instead of only recording metadata. The output remains static-safe: no analytics, payments, backend, authentication, live telemetry, fake metrics, customer logos, or quoted endorsements.

```bash
npm run qa
npm run test:visual
npm run qa:full
npm audit --audit-level=moderate
```

Visual QA builds and serves the static site, checks desktop and mobile layouts, fails on console/page errors, horizontal overflow, missing hero/nav/CTA visibility, broken hash anchors, and visible nav ellipses, then writes screenshots to `.agent/audits/screenshots/`. If Chromium is not installed yet, run `npx playwright install chromium` once.

## Deploy verification
```bash
LIVE_URL="https://castiliad.github.io/nocturne-signal/" \
EXPECT_TEXT="Nocturne Signal" \
REPO="castiliad/nocturne-signal" \
npm run verify:deploy
```

## Agent maintenance notes
- Read `AGENTS.md` before editing.
- Keep visible copy aligned with `.agent/site.contract.yaml` and `.agent/brand.contract.yaml`.
- Payment mode is disabled in `.agent/payment.contract.yaml`; do not add payment links without explicit approval.
- Deployment is GitHub Pages via `.github/workflows/deploy.yml`.
