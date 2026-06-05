# AGENTS.md

## Mission
Nocturne Signal is a static AgentSite generated from this requester brief: Create a dark, edgy, technical GitHub Pages static site for a personal AI/operator lab. It should feel like a techno-oracle command center: xAI-style monochrome restraint, Linear-level precision, VoltAgent terminal energy, and one signature kinetic typography / pretext-inspired hero. It must remain static, public-safe, no analytics, no tracking, no fake metrics, and no fabricated endorsements.

## Audience
- Technical collaborators reviewing AI/operator experiments
- Hiring or project leads who need a credible technical signal without marketing fluff
- Future agents maintaining the site from contracts, QA gates, and deploy evidence

## Stack
- Astro static site
- Astro production build checks
- GitHub Pages via GitHub Actions
- Lightweight repo-local scripts in `scripts/`

## Recipe registry
Selected recipes: product-cockpit, artifact-gallery, search-index, agent-run-ledger, copy-evidence-strip
Archetype: product-cockpit
Visual preset: cockpit-dark
auto_recipe_selection: not requested; default recipe selection unchanged

Use `npm run list:recipes`, `npm run score:recipes`, and `npm run recommend:recipes` before applying or changing registered patterns. Recipe guidance is static-safe composition guidance, not permission to add live data, analytics, payments, or unsupported claims.

## Safe edit boundaries
Agents may safely edit:
- `src/components/**`, `src/pages/**`, `src/styles/**`, `src/data/**`
- Copy that remains consistent with `.agent/site.contract.yaml` and `.agent/brand.contract.yaml`
- Supported claims listed in `.agent/site.contract.yaml`
- Documentation, runbooks, and plan files that reflect actual behavior

## Approval-required changes
Get explicit human approval before:
- Adding analytics, cookies, tracking pixels, or forms
- Adding payment links, lead capture, or external scripts
- Publishing private project details, customer names, or unsupported claims
- Changing deployment target away from GitHub Pages

## QA commands
Run before handoff:
```bash
npm run qa
```

Individual gates:
```bash
npm run check:contract
npm run check:claims
npm run check:seo
npm run check:links
npm run check:artifacts
npm run check:roadmap
npm run build:search-index
npm run check:search-index
npm run check:atlas
npm run check:runs
npm run check:requests
npm run build:briefing
npm run check:briefing
npm run check:layout
npm run build
```

## Feature-request process
1. Capture the natural-language request as a short brief.
2. Compare it with `.agent/site.contract.yaml`, `.agent/brand.contract.yaml`, and `.agent/payment.contract.yaml`.
3. Record assumptions and acceptance criteria in an issue or plan file.
4. Implement the smallest coherent change.
5. Run QA and include command output summary in the handoff.
6. Deploy only after checks pass.
7. Verify the live URL contains expected current copy.
