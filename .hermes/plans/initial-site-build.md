# Initial site build plan: Nocturne Signal

## Request
Create a dark, edgy, technical GitHub Pages static site for a personal AI/operator lab. It should feel like a techno-oracle command center: xAI-style monochrome restraint, Linear-level precision, VoltAgent terminal energy, and one signature kinetic typography / pretext-inspired hero. It must remain static, public-safe, no analytics, no tracking, no fake metrics, no fake testimonials.

## Audience
- Technical collaborators reviewing AI/operator experiments
- Hiring or project leads who need a credible technical signal without marketing fluff
- Future agents maintaining the site from contracts, QA gates, and deploy evidence

## Site sections
- Signal over spectacle (signal)
- Systems you can inspect (systems)
- Agent-maintainable by design (handoff)

## Proof/artifacts
- Static deploy evidence: GitHub Pages publishes the built output and npm run verify:deploy checks the live URL after deployment.
- Agent contracts: .agent/site.contract.yaml and .agent/brand.contract.yaml define the mission, allowed claims, forbidden claims, visual posture, and approval boundaries.
- Local QA gates: npm run qa and npm run qa:full validate contracts, claims, links, generated indexes, build output, and browser-visible behavior.

## Assumptions
- The site remains static and deploys to GitHub Pages.
- No analytics, payments, fake customers, fake metrics, or unsupported claims are included.

## Scope
- Generate a safe first-pass landing page and repo guardrails.

## Non-goals
- Payment, analytics, custom domains, server runtime, and unsupported claims.

## Files expected to change
- `AGENTS.md`
- `.agent/**`
- `.github/workflows/deploy.yml`
- `package.json`
- `scripts/**`
- `src/**`

## Acceptance criteria
- Hero and core sections reflect the brief.
- Contracts exist and payment remains disabled/no-payment.
- `npm run qa` passes locally.
- GitHub Pages deploy succeeds and live URL contains `Nocturne Signal`.

## QA commands
```bash
npm run qa
npm audit --audit-level=moderate
```

## Deploy/verify
```bash
LIVE_URL="https://castiliad.github.io/nocturne-signal/" EXPECT_TEXT="Nocturne Signal" REPO="castiliad/nocturne-signal" npm run verify:deploy
```
