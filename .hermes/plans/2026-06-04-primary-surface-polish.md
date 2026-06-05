# Nocturne Signal primary-surface polish

## Request

Proceed with the next iteration after live review found that the hero/opening stayed strong but the page drifted into a dense proof-dashboard lower down.

## Assumptions

- Preserve the dark techno-oracle/product-cockpit visual identity.
- Keep all existing static proof modules available.
- Do not add analytics, forms, payments, tracking, backend runtime, or unsupported claims.
- Prioritize landing-page rhythm over showing every archive module inline.

## Scope

- Rewrite the operating-context copy so it reads like visitor-facing site copy, not the original generation prompt.
- Move trust/boundary messaging earlier.
- Add a featured proof-trail section to explain the verification chain before exposing data-heavy modules.
- Select artifacts as the primary surface.
- Collapse search index, roadmap, and run ledger into secondary archive panels using static `<details>` disclosure.
- Update CSS for primary-surface and secondary-module layout.
- Update the site contract to record boundaries, secondary archive, and `primary-surface-layout`.

## Non-goals

- No new external dependencies.
- No backend, auth, telemetry, analytics, forms, payment links, or live data.
- No redesign of the hero aesthetic.
- No removal of existing proof modules.

## Acceptance criteria

- The live flow no longer places artifact gallery, search index, roadmap, and run ledger back-to-back at equal visual weight.
- The page preserves the strong hero identity while improving editorial pacing.
- Secondary modules remain accessible and testable by visual QA.
- `npm run qa:full` passes.
- `npm audit --audit-level=moderate` passes.
- Deploy succeeds and live URL verifies expected text.

## Verification commands

```bash
npm run qa:full
npm audit --audit-level=moderate
git diff --check
LIVE_URL="https://castiliad.github.io/nocturne-signal/" EXPECT_TEXT="Browse the proof first" REPO="castiliad/nocturne-signal" npm run verify:deploy
```
