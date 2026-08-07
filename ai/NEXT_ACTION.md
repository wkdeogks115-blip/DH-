# NEXT ACTION — C0032 REMAINING SURFACE AUDIT FIRST

## Baseline

- Active Control: R0003
- Active Preview: C0009A D2
- Direct parent / immutable visual rollback: C0031
- C0031 SHA: `45d1b8d7fd70fcfe16ce450c6fe5ad4957b26c40cf4bb3b3924260a2863e3ddd`
- Functional rollback: C0022
- Overall design heuristic: 80/100
- Functional prototype heuristic: 84/100
- Production: HOLD
- Actual external URL Runtime: UNVERIFIED

## Why this is audit-first

The main conversion funnel and the two primary service branches now share a consistent shell. The remaining pages have different jobs: game product, partner intake, evidence/reviews, policy/reference and diagnosis. Forcing one visual template across all of them could reduce task clarity or create unnecessary CSS debt.

## Objective

Audit these remaining surfaces before creating any C0032 build:

1. `game/`
2. `partners/`
3. `cases/`
4. `reviews/`
5. `policies/`
6. `diagnose/`
7. `404.html`

Classify each as `KEEP`, `MIGRATE`, `MINOR_FIX`, or `UNVERIFIED` using actual desktop/mobile render evidence and task role.

## Build gate

Create a separate C0032 Candidate only if at least one material inconsistency is found, such as:

- the primary action or user question is visually unclear;
- mobile layout or density creates measurable task friction;
- the page visibly conflicts with the approved shell in a way that harms trust or comprehension;
- duplicate/high-specificity styling can be removed with measurable benefit;
- accessibility or interaction state is materially weaker than the current core funnel.

Do **not** redesign legal/policy pages merely for novelty. Preserve information density when it serves reference scanning.

## Required evidence if a build is opened

- C0031 locked as direct parent.
- Existing Home/PC/Apply/Rescue/Stream Ready/Creator pages remain unchanged outside explicitly selected scope.
- 23 application options and 86 application links preserved.
- prices, service IDs and Apply URLs preserved.
- Desktop/Mobile evidence for every page changed.
- no horizontal overflow or clipped controls.
- HTML/JS/CSS/refs/fragments/IDs/Alt/JSON-LD PASS.

## Stop conditions

- no material inconsistency after audit → `HOLD — 새 결론 없음` and do not create C0032;
- proposed change is aesthetic-only with no task/trust benefit;
- scope begins to merge unrelated policy, evidence and product pages into one generic layout;
- functional/data/accessibility regression.

## Promotion boundary

Any C0032 build remains a Review Candidate. Do not promote or deploy without `/upgrade-auto`.
