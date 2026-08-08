# NEXT ACTION — C0040 VISUAL REBASE PROTOTYPE

## Current state

- Active Control: R0004
- Active Preview: C0038
- Active SHA: `b1c2628e02de28c3ccabc1247513bab4db93d2a6ee04427c1fd951025bde1114`
- Active Rollback: C0009A D2
- Promotion: EXECUTED_LOGICAL_PREVIEW_BASELINE
- External Preview Runtime: UNVERIFIED
- External Preview deployment: DEFERRED_PENDING_VISUAL_REBASE
- Production: HOLD

## New material evidence

Fresh visual review of 15 routes × Desktop/Mobile plus comparison against older Home visuals confirmed that the current shell is too uniformly dark and repetitive. Core issues are continuous dark visual mass, repeated large-heading/right-proof-card hero grammar, excessive bordered-container repetition, and weak page-specific personality.

Approximate first-fold dark-pixel coverage (`relative luminance < 0.12`) increased from older Home Desktop 85.3% to C0038 Home 92.6%, PC 94.0%, Apply 95.0%. This is diagnostic evidence, not a brightness KPI.

## Next meaningful action

Delivery Plane (`01_사이트·상품·운영`) should build planned **C0040 Visual Rebase Prototype** from C0038 on exactly:

- Home
- PC
- Apply

Use `delivery/C0040_VISUAL_REBASE_DELIVERY_BRIEF_V1.md` as the build contract.

Do not build the design Candidate in Control Plane. Do not deploy C0038 to external Preview yet. Do not roll back C0038 functionality.

## Required direction

- deepest navy becomes framing, not the entire canvas;
- introduce mid-tone/lighter sustained reading/work surfaces;
- primary CTA stays cyan;
- reduce generic right-side proof cards, pills, bordered boxes and repeated 3-card patterns;
- one meaningful real-content bespoke visual per target page;
- Apply is the highest priority for tonal/work-surface relief;
- preserve all C0038 business, safety, accessibility and routing invariants.

## Required A/B gate

Home / PC / Apply each require Desktop + Mobile before/after plus actual Apply Chromium interaction. Non-target routes should remain pixel-identical unless a shared-token Material Delta is declared first.

## Stop condition

Reject if the prototype merely gets brighter, returns to card/glow-heavy styling, weakens price/scope/CTA clarity, increases mobile burden, adds fake proof, or regresses C0038 behavior.
