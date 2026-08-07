# DH PROJECT SNAPSHOT R23

## Locked state

- Active Control: R0003
- Active Preview: C0009A D2
- Current Review Candidate: C0027
- C0027 SHA-256: `0db244b8f483e030d330d66f43b4d2bd262ed06460abf919209e627b996cdd7d`
- Direct Parent / Visual Rollback: C0026 `8088b95c03d5663547a66eb79698d2da673863f96937aa0509fe32a1b643c44e`
- Functional Rollback: C0022 `5f9e8749b02ff210e7a1729224e58a315e4cf023e59fc356c3529209c7af9128`
- Latest Answer Pack: R23 `caf51941b3c60b58c641e72f340dfb0966ad2e2499500e359827dc3c624cfc15`
- Latest Handoff: A19
- Production: HOLD
- Promotion: NOT_EXECUTED

## C0027 scope

Only Home, PC pricing and Apply receive the new Visual Shell. C0026 function, data model, prices, routes, application JavaScript, validation, error recovery, keyboard focus and accessibility behavior are preserved.

## Evidence

- Candidate ZIP CRC: PASS
- Deterministic rebuild: PASS
- HTML count: 15
- Visual-shell pages: 3
- JS syntax: PASS 9/9
- Missing local refs: 0
- Broken fragments: 0
- Duplicate IDs: 0
- Missing Alt: 0
- JSON-LD errors: 0
- Application options: 23 preserved
- Application links: 86 preserved
- Prices/service IDs/apply URLs: preserved
- Targeted self-contained Chromium desktop/mobile layout: PASS, no horizontal overflow
- Objective design heuristic: 72 → 80
- Functional prototype heuristic: 84 maintained

## Unverified

- Actual URL navigation Runtime
- Complete browser JavaScript Runtime
- Real mobile device
- Assistive technology
- User conversion test

## Important debt

C0027 is intentionally a reversible prototype layer and adds 26,397 CSS bytes over C0026. Do not expand the override layer across the site. C0028 must consolidate the approved shell into reusable component contracts with measurable reduction before wider migration.
