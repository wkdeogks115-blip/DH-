# NEXT ACTION — C0029 APPLY MOBILE DECISION COMPRESSION

## Baseline

- Active Control: R0003
- Active Preview: C0009A D2
- Direct parent / immutable visual rollback: C0028
- C0028 SHA: `4bdbe123a6e5860979f8af580a06ffd2407c63e2739ef802111679f679315cb7`
- Functional rollback: C0022
- Design heuristic: 80/100
- Functional prototype heuristic: 84/100
- Production: HOLD
- Actual URL Runtime: UNVERIFIED

## Why this is next

C0028 successfully consolidated the C0027 visual shell with exact pixel parity and 6,300 bytes of CSS reduction. The most visible remaining weakness in the audited core flow is the long Apply mobile page and decision burden.

## Objective

Create a separate C0029 Review Candidate that reduces mobile Apply decision/scroll burden without changing business data or validated application behavior.

Preferred methods:

- reduce repeated guidance visible at once;
- use progressive disclosure only for secondary explanation;
- keep required labels, errors and current-stage context visible;
- do not hide information needed to choose a service or complete the form;
- preserve desktop C0028 unless a shared improvement is clearly justified.

## Required evidence

- C0028 locked as direct parent.
- 23 application options, 86 application links, prices, service IDs and apply URLs preserved.
- `js/apply.js` validation, error summary, focus recovery, input retention and two-time availability rule preserved.
- Touch targets and keyboard focus preserved.
- Mobile Apply rendered height / decision-density improvement measured.
- No horizontal overflow or clipped controls.
- Static QA PASS.
- Actual URL Runtime remains UNVERIFIED unless truly executed.

## Stop conditions

- No measurable mobile decision/scroll improvement.
- Required information becomes hidden or harder to understand.
- Accessibility, function, price or service regression.
- Improvement depends only on aesthetic preference without task benefit.

## Promotion boundary

C0029 remains a Review Candidate. Do not promote or deploy without `/upgrade-auto`.