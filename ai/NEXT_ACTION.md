# NEXT ACTION — C0027 VISUAL SHELL REDESIGN PROTOTYPE

## Why the priority changed

C0026 objective design audit scored the current site **72/100 overall**, with **84/100 functional prototype quality** but **64/100 commercial brand design quality**. Further micro-consolidation of Legacy CSS is lower-value than improving brand differentiation, page rhythm, trust proof and decision density.

Read `audits/DH_C0026_OBJECTIVE_DESIGN_AUDIT_V1.md` before implementation.

## Objective

Keep C0026's function, content model, prices, product/service IDs, routes, application JavaScript, error recovery, keyboard focus and accessibility behavior unchanged. Build a separate C0027 Review Candidate that redesigns only the Visual Shell of:

1. Home
2. PC pricing/products
3. Apply

## Design direction

- Preserve neutral dark surfaces and one cyan action accent, but reduce generic nested Card/Border repetition.
- Make each page answer one primary customer question.
- Reduce mobile scroll and repeated explanatory copy.
- Strengthen real-service trust, process clarity and decision evidence without inventing testimonials, logos or performance numbers.
- Use a new coherent component layer rather than stacking more high-specificity overrides.

## Required evidence

1. Lock C0026 SHA `8088b95c03d5663547a66eb79698d2da673863f96937aa0509fe32a1b643c44e` as direct parent and immutable rollback.
2. Preserve 23 products, 86 application links, prices, service IDs and apply URLs.
3. Preserve application validation, error summary, focus recovery, value retention and schedule-two-options rule.
4. Produce desktop and mobile screenshots for Home, PC pricing and Apply.
5. Compare C0026 and C0027 using the objective design rubric; target overall score >= 80 without reducing functional prototype score below 84.
6. Run HTML, JS, CSS, refs, fragments, duplicate IDs, Alt and JSON-LD checks.
7. Keep actual URL Runtime, real-device and assistive-technology status UNVERIFIED unless executed.

## Stop conditions

- Functional or data regression.
- Accessibility regression.
- New design does not improve the rubric by at least 6 points.
- Visual change relies on invented customer proof or unsupported business claims.
- Scope expands beyond the three prototype pages before evidence is reviewed.

## Promotion boundary

C0027 remains a Review Candidate. Do not promote, deploy or replace Active Control without `/upgrade-auto`.
