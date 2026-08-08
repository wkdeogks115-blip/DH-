# DH C0040 VISUAL REBASE DELIVERY BRIEF V1

Role: DELIVERY_PLANE_BUILD_BRIEF
Source Finding: DH C0038 FINAL VISUAL DIRECTION REVIEW V1
Control Baseline: R0004
Active Preview Baseline: C0038
Active Preview SHA-256: b1c2628e02de28c3ccabc1247513bab4db93d2a6ee04427c1fd951025bde1114
Production: HOLD
External Preview: NOT_DEPLOYED
Build Status: NOT_EXECUTED_IN_CONTROL_PLANE

## Decision

**VISUAL_DIRECTION_REBASE_REQUIRED_BEFORE_PREVIEW_DEPLOYMENT**

Do not roll back C0038 functionality or information architecture. Do not continue spreading the current dark SaaS/editorial shell. Build one controlled visual prototype on exactly Home, PC, Apply.

## Diagnostic evidence

Fresh review basis:
- C0038: 15 routes × Desktop/Mobile = 30 fresh renders.
- Older Home Desktop/Mobile project visuals.
- Functional baseline R0004/C0038 remains valid.

Approximate first-viewport dark-pixel coverage (`relative luminance < 0.12`):
- Older Home Desktop: 85.3%
- C0038 Home Desktop: 92.6%
- C0038 PC Desktop: 94.0%
- C0038 Apply Desktop: 95.0%
- Older Home Mobile: 63.7%
- C0038 Home Mobile: 78.8%

Interpretation: the problem is excessive continuous low-luminance visual mass and repeated shell grammar, not simply dark mode. Do not optimize to a brightness quota.

## New visual north star

**Premium Technical Service, not Dark SaaS Dashboard.**

The site should feel technically competent, commercially clear, authored by a real specialist, visually calm, recognizably DH, and different page-to-page without losing the system.

## Core rules

1. Dark is a framing device, not the entire canvas. Use deepest navy for header/hero/footer or selected high-trust sections; introduce mid-tone/lighter sustained reading/work surfaces.
2. Primary action remains cyan.
3. Limited service-specific non-action accents may vary but may not compete with CTA semantics.
4. Cards only for selectable packages, evidence/case/review objects, or independent actionable units.
5. Reduce AI-template markers: decorative pills, numbered micro-labels, generic right-proof cards, repeated 3-card rows, thin boxes around ordinary text, generic hero glows.
6. Use more natural Korean typography: calmer hero scale, better word breaks, stronger body contrast.
7. One meaningful bespoke visual object per core page, derived only from real content.
8. Price, scope, CTA, proof and next-step clarity may not regress.
9. Mobile must be visually lighter than desktop; do not merely stack dark desktop cards.
10. No fake testimonials, logos, customer counts, performance claims, or fabricated screenshots.

## Prototype assignments

### Home
- Replace the cloned large-left-title/right-proof-card feel.
- Keep a dark branded hero, then transition to a visibly lighter/mid-tone service-discovery surface.
- Preserve transparent price-range/route clarity.
- Bespoke visual candidate: **DH Scope Map** using real issue → service family → output / price-entry data.

### PC
- Preserve package logic and one recommended package emphasis.
- Convert symptom/process exposition to open layout + dividers where possible.
- Introduce a lighter diagnostic/work surface between dark hero and final CTA.
- Bespoke visual candidate: **Symptom → Scope → Package Map** using existing service data only.

### Apply — highest priority
- Preserve current 4-step form behavior, progress, summary and mobile compression.
- Dark brand intro, then transition immediately to a lighter/mid-tone application work surface.
- Reduce nested border/card layers and use spacing/type/state for grouping.
- Bespoke visual candidate: **Application Journey Rail** tied to the real 4-step structure.

## Locked invariants

Preserve:
- 23 application options
- 86 application links
- 23 service IDs
- prices and Apply URLs
- current `js/apply.js` safety/error/input-retention behavior
- Diagnose result focus/ARIA semantics
- Preview noindex guard
- local routes/fragments/accessibility labels
- no horizontal overflow.

## Non-target lock

C0040 may modify only Home, PC, Apply and strictly demonstrated shared visual tokens that do not alter non-target pages. Preferred gate: other 12 public routes × Desktop/Mobile = 24/24 zero changed pixels.

## Acceptance scorecard

- Brand distinctiveness / human craft: 20, minimum 16
- First-impression hierarchy: 15, minimum 13
- Light/dark rhythm: 15, minimum 12
- Commercial clarity: 15, minimum 14
- Reduction of AI-template patterns: 15, minimum 12
- Typography/readability: 10, minimum 8
- Mobile visual load: 10, minimum 8

Each target page >= 83/100 and whole prototype direction >= 86/100, with zero functional/accessibility/business regression. Heuristics are internal review aids, not conversion evidence.

## Required A/B evidence

For Home / PC / Apply:
- Desktop full-page before/after
- Mobile full-page before/after
- Desktop first-fold side-by-side
- Mobile first-fold side-by-side
- first-fold dark-mass comparison
- border/card/container count comparison
- hero-pattern diversity review
- typography line-break review
- mobile scroll-height delta
- actual Chromium interaction audit for Apply.

## Reject conditions

Reject if the prototype merely changes brightness, weakens price/scope/CTA clarity, increases cards/glows/gradients, uses stock SaaS illustration, repeats the same hero layout on all three pages, materially increases mobile burden without decision value, makes Apply more decorative but harder to complete, regresses C0038 behavior, or adds fake proof.

## Rollout rule

Do not propagate C0040 beyond Home/PC/Apply until the A/B is clearly preferred over C0038, all runtime/invariant gates pass, Control Plane reviews the Candidate, and any promotion remains explicit.
