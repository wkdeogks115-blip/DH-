# NEXT ACTION — C0031 CREATOR SHELL MIGRATION

## Baseline

- Active Control: R0003
- Active Preview: C0009A D2
- Direct parent / immutable visual rollback: C0030
- C0030 SHA: `e3caadb915360ab36fa9cbbc9bc13feddbfb29f2ccc97d32a916371cf0ba1bbd`
- Functional rollback: C0022
- Overall design heuristic: 80/100
- Functional prototype heuristic: 84/100
- Production: HOLD
- Actual external URL Runtime: UNVERIFIED

## Why this is next

Home, PC pricing, Apply, Rescue and Stream Ready now share the approved visual language. The largest remaining customer-facing inconsistency is the Creator branch.

## Objective

Create a separate C0031 Review Candidate that migrates only:

1. `creator/`
2. `creator/youtube/`
3. `creator/editing/`

onto the same reusable shell principles while preserving C0030 Rescue/Stream Ready, C0029 Apply behavior, prices, product/service IDs, routes and application links.

## Design contract

- retain the neutral dark shell and restrained action accent;
- reduce nested cards and repeated decorative containers;
- express Creator service differences through hierarchy and content rather than unrelated color systems;
- preserve existing real claims only; invent no testimonials, logos, customer counts or performance metrics;
- reuse C0028/C0030 component contracts rather than creating a separate page-wide override system.

## Required evidence

- C0030 locked as direct parent.
- C0030 Rescue/Stream Ready and C0029 Home/PC/Apply remain visually unchanged in audited views.
- 23 application options and 86 application links preserved.
- prices, service IDs and Apply URLs preserved.
- desktop/mobile screenshots for all three Creator pages.
- no horizontal overflow or clipped CTA/control.
- HTML/JS/CSS/refs/fragments/IDs/Alt/JSON-LD PASS.
- measurable hierarchy/consistency improvement.

## Stop conditions

- functional/data/route/accessibility regression;
- Creator migration requires unsupported claims;
- no clear visual hierarchy improvement;
- scope expands into policies/cases/reviews/game in the same Candidate.

## Promotion boundary

C0031 remains a Review Candidate. Do not promote or deploy without `/upgrade-auto`.
