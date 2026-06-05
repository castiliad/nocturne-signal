# Static Site Pattern Lab iteration

## Request

Turn Nocturne Signal into a canvas for testing static-site skills, recipes, and different approaches so we can learn together while keeping the public site polished and safe.

## Assumptions

- Keep the current dark product-cockpit identity.
- Treat the Pattern Lab as public-safe: no private data, no analytics, no forms, no payment, no backend runtime.
- The lab should explain what experiments are available, which Hermes skills/AgentSite recipes they use, and what would qualify an experiment to graduate into the primary page.
- Add the lab as a curated section, not another huge archive dump.

## Scope

- Add a primary nav link to the lab.
- Add a "Static Site Pattern Lab" section with experiment cards.
- Add a skill-to-site matrix mapping Hermes skills to static-site capabilities.
- Add promotion rules for experiments.
- Update the site contract to include the pattern lab requirement and allowed claims.
- Preserve existing proof/archive modules.

## Non-goals

- No new dependencies.
- No new backend, analytics, lead capture, or external scripts.
- No generated media assets in this pass.
- No implementation of every experiment yet; this pass creates the durable canvas.

## Acceptance criteria

- The live page contains "Static Site Pattern Lab".
- The lab clearly maps at least six experiment ideas to skills/recipes.
- The skill matrix includes creative/static-site skills such as pretext, p5js, gsap, hyperframes, architecture-diagram, and swarmui-zimage-api.
- The lab states promotion rules that preserve clarity, delight, maintainability, and static safety.
- `npm run qa:full`, `npm audit --audit-level=moderate`, `git diff --check`, deploy, and live verification pass.

## Verification commands

```bash
npm run qa:full
npm audit --audit-level=moderate
git diff --check
LIVE_URL="https://castiliad.github.io/nocturne-signal/" EXPECT_TEXT="Static Site Pattern Lab" REPO="castiliad/nocturne-signal" npm run verify:deploy
```
