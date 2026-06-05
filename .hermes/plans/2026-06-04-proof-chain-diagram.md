# Proof-chain diagram iteration

## Request

Proceed with the next Pattern Lab iteration. The lab marked "Proof-chain diagram" as next-ready: turn claim → contract → QA → deploy into a visual system map so visitors understand the AgentSite operating envelope faster.

## Assumptions

- Keep the existing dark product-cockpit identity.
- Use a static inline SVG/HTML diagram: no new dependency, no external runtime, no tracking, no backend.
- The diagram should replace/supplement the current four proof cards, not add another huge dense module.
- It should remain accessible with text labels and explanatory cards.

## Scope

- Add a reusable `ProofChainDiagram.astro` component with inline SVG and semantic fallback text.
- Replace the current four-card featured proof trail with the diagram plus compact explanatory nodes.
- Update Pattern Lab to mark proof-chain diagram as promoted/active.
- Update the site contract to include `proof_chain_diagram` as a required section and allowed public-safe static experiment.
- Preserve all existing archive modules and static-safety boundaries.

## Non-goals

- No p5.js/GSAP animation in this pass.
- No generated images, media, analytics, forms, payment, backend, or external scripts.
- No change to deployment target.

## Acceptance criteria

- The live page contains "Proof-chain diagram" and "Claim → Contract → QA → Deploy → Live" semantics.
- The featured proof trail is more visual and easier to scan than four equal cards.
- `npm run qa:full`, `npm audit --audit-level=moderate`, `git diff --check`, deployment, and live verification pass.

## Verification commands

```bash
npm run qa:full
npm audit --audit-level=moderate
git diff --check
LIVE_URL="https://castiliad.github.io/nocturne-signal/" EXPECT_TEXT="Proof-chain diagram" REPO="castiliad/nocturne-signal" npm run verify:deploy
```
