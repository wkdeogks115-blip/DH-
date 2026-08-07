# NEXT ACTION — C0028 VISUAL SHELL COMPONENT CONSOLIDATION

## Baseline

- Active Control: R0003
- Active Preview: C0009A D2
- Direct parent / immutable visual rollback: C0027
- C0027 SHA: `0db244b8f483e030d330d66f43b4d2bd262ed06460abf919209e627b996cdd7d`
- Functional rollback: C0022
- Design heuristic: C0026 72 → C0027 80
- Functional prototype heuristic: 84 maintained
- Production: HOLD
- Actual URL Runtime: UNVERIFIED

## Why this is next

C0027 proves the visual direction on Home, PC pricing and Apply, but it adds a temporary 26,397-byte high-specificity visual-shell layer. Expanding that layer to the rest of the site before consolidation would increase maintenance and regression risk.

## Objective

Create a separate C0028 Review Candidate that converts the approved C0027 shell into reusable, lower-specificity component contracts for:

1. page/section shell
2. primary/secondary actions
3. pricing rail/cards
4. form stages/options/summary
5. shared responsive spacing and type rules

Preserve C0027 appearance on the three prototype pages while reducing duplicate/high-specificity declarations. Do not expand to additional service pages until this consolidation has measurable benefit.

## Required evidence

- Lock C0027 as direct parent.
- Preserve 23 products, 86 application links, prices, service IDs and apply URLs.
- Preserve all C0026/C0027 application JS and accessibility behavior.
- Reduce temporary visual-shell CSS bytes or duplicate declarations by a measurable amount.
- Preserve C0027 targeted desktop/mobile appearance with computed-style or screenshot parity.
- Re-run HTML, JS, CSS, refs, fragments, duplicate IDs, Alt and JSON-LD checks.
- Keep actual URL Runtime, real-device and assistive-technology status UNVERIFIED unless actually executed.

## Stop conditions

- No measurable CSS/consolidation benefit.
- Visual regression against C0027.
- Functional, data or accessibility regression.
- Expansion to additional pages before component consolidation passes.

## Promotion boundary

C0028 remains a Review Candidate. Do not promote or deploy without `/upgrade-auto`.
