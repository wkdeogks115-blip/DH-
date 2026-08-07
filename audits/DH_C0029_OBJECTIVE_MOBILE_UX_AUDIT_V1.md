# DH C0029 Objective Mobile UX Audit V1

## Decision

**PASS — measurable mobile task compression without business-logic or desktop visual regression.**

## Measured result at 390 × 844

| Metric | C0028 | C0029 | Delta |
|---|---:|---:|---:|
| Initial document height | 4,903 px | 3,390 px | **-1,513 px / -30.859%** |
| Generated-summary height | 5,325 px | 4,359 px | **-966 px / -18.141%** |
| Progress shell | 146 px | 94 px | **-52 px** |
| Form height | 2,549 px | 1,903 px | **-646 px** |
| Stage 1 | 396 px | 269 px | -127 px |
| Stage 2 | 459 px | 354 px | -105 px |
| Stage 3 | 1,111 px | 833 px | -278 px |
| Stage 4 | 528 px | 392 px | -136 px |

## Interaction evidence

Actual `js/apply.js` was executed inside self-contained Chromium.

- one availability time → correct 2-time validation error
- error summary receives focus
- issue and availability values remain after failed submission
- two availability times + required acknowledgements → summary generated
- selected product is present in generated summary
- horizontal overflow: 0
- Desktop C0028 → C0029 screenshot changed pixels: 0

## What changed on mobile

- application hero vertical space reduced
- progress steps compressed from 2×2 to 1×4
- secondary stage-head descriptions visually clipped while remaining in DOM
- stage padding and textarea height reduced
- Stage 3 secondary option explanations visually suppressed; primary option names remain visible
- safety confirmation explanations remain visible
- empty application-summary card hidden until a valid summary is created

## Boundaries

- `js/apply.js`: byte-identical to C0028
- application form control signature: identical
- 23 application options: preserved
- 86 application links: preserved
- prices/service IDs/apply URLs: preserved
- Actual external URL navigation: UNVERIFIED
- Real mobile device: NOT_EXECUTED
- Assistive technology: NOT_EXECUTED
- Production: HOLD
- Promotion: NOT_EXECUTED
