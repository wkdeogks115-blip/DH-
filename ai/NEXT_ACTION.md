# NEXT ACTION — C0030 RESCUE + STREAM READY VISUAL SHELL MIGRATION

## Baseline

- Active Control: R0003
- Active Preview: C0009A D2
- Direct parent / immutable visual rollback: C0029
- C0029 SHA: `ba0de866143c9c68a3c5c0e9804390afeacbd43969c1dd8e135a804a59789930`
- Functional rollback: C0022
- Core design heuristic: 80/100
- Functional prototype heuristic: 84/100
- Production: HOLD
- Actual external URL Runtime: UNVERIFIED

## Why this is next

Home, PC pricing and Apply now use the approved Visual Shell, and C0029 materially reduced the mobile Apply burden. The largest visible inconsistency in the primary customer journey is that the two main service decision pages `rescue/` and `stream-ready/` still use the older presentation language.

## Objective

Create a separate C0030 Review Candidate that migrates only:

1. `rescue/`
2. `stream-ready/`

onto the reusable C0028/C0029 Visual Shell principles while preserving all business data, links, service IDs, prices, routes and C0029 Apply behavior.

## Design contract

- neutral dark surfaces + one cyan action accent
- fewer nested bordered cards
- one primary customer question per page
- decision rail / section hierarchy before decorative panels
- no invented testimonials, logos, customer counts or performance claims
- reuse current component tokens; do not create another high-specificity page-wide override layer if a reusable contract can express the change

## Required evidence

- C0029 locked as direct parent.
- C0029 Apply CSS/behavior unchanged.
- 23 application options and 86 application links preserved.
- prices, service IDs and Apply URLs preserved.
- Desktop and mobile screenshots for both migrated pages.
- no horizontal overflow or clipped CTA/control.
- static HTML/JS/CSS/refs/fragments/IDs/Alt/JSON-LD PASS.
- measurable reduction in visual inconsistency versus C0029, with no regression on Home/PC/Apply.

## Stop conditions

- functional/data/route/accessibility regression.
- migration needs fabricated proof or unsupported claims.
- no clear hierarchy improvement over current service pages.
- scope expands into Creator pages in the same Candidate.

## Promotion boundary

C0030 remains a Review Candidate. Do not promote or deploy without `/upgrade-auto`.
