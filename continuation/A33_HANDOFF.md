# DH R0004 VISUAL REBASE HANDOFF A33

Role: `HANDOFF_ADDENDUM_NOT_CONTROL`
Supersedes: `A32`
Source action: `REPLACE_A32_WITH_A33`

## Current state
- Active Control: R0004
- Active Preview Baseline: C0038
- Active SHA-256: `b1c2628e02de28c3ccabc1247513bab4db93d2a6ee04427c1fd951025bde1114`
- Active Rollback: C0009A D2
- External Preview: NOT_DEPLOYED
- Production: HOLD

## New Material Delta
Fresh visual review of 15 routes × Desktop/Mobile plus comparison against older Home visuals shows excessive continuous dark visual mass, repeated large-heading + right-proof-card hero grammar, too many thin border/container repetitions, and weak page personality.

First-fold dark-pixel diagnostic (`luminance < 0.12`):
- older Home Desktop: 85.3%
- C0038 Home Desktop: 92.6%
- C0038 PC Desktop: 94.0%
- C0038 Apply Desktop: 95.0%
- older Home Mobile: 63.7%
- C0038 Home Mobile: 78.8%

This is visual-mass diagnostic evidence, not a brightness KPI.

## Decision
`DEFER_PREVIEW_DEPLOYMENT_PENDING_VISUAL_REBASE_PROTOTYPE`

Do not roll back C0038 functionality. Do not change Active Control. Do not build the visual Candidate in Control Plane.

## Delivery Plane next action
Build planned C0040 Visual Direction Prototype on exactly Home, PC, Apply using `delivery/C0040_VISUAL_REBASE_DELIVERY_BRIEF_V1.md`.

## Locked invariants
- 23 application options
- 86 application links
- 23 service IDs
- prices and Apply URLs
- C0033 safety validation
- C0038 Diagnose focus/semantics
- Preview noindex protection
- no horizontal overflow

## Stop / Reject
Reject if C0040 merely brightens surfaces, returns to card/glow-heavy styling, worsens commercial clarity/mobile completion, regresses C0038 behavior, or adds fake proof.

## Source budget
Expected persistent Source count after A32→A33 replacement: 15.
Actual UI Source count: USER_CONFIRMATION_REQUIRED.
Status: WARNING.
