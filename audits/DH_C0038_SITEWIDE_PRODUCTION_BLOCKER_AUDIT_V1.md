# DH C0038 Site-wide Production-Blocker Audit V1

## Decision

**MATERIAL DELTA FOUND — Diagnose result focus/announcement accessibility defect.**

The C0037 site was audited for form behavior, keyboard/focus, local references/fragments, ARIA references, business routing, mobile overflow and high-salience visual consistency.

## Reproduced defect

On `diagnose/`, a valid keyboard submission generated and scrolled the result into view, but focus remained on the `추천 범위 확인` submit button. The generated result had no named region/live semantics.

This is a meaningful keyboard/screen-reader completion-state gap: a sighted pointer user sees the result, while a keyboard or assistive-technology user may miss the state transition.

## C0038 fix

- `role="region"`
- `aria-labelledby="diagnose-result-title"`
- `aria-live="polite"`
- `aria-atomic="true"`
- `tabindex="-1"`
- valid generation moves focus to the result with `preventScroll:true`

## Executed evidence

- Parent valid result focus: FAIL reproduced — focus remained on submit button.
- Candidate valid result focus: PASS.
- Candidate native invalid submit: PASS — first required `issue` radio receives browser focus.
- Diagnose resting visual parity Desktop/Mobile: 2/2 zero changed pixels.
- Other 14 pages Desktop/Mobile: 28/28 zero changed pixels.
- C0033 Apply safety runtime: PASS.
- Local refs/fragments/duplicate IDs/Alt/JSON-LD/ARIA references: PASS.
- Application options: 23.
- Application links: 86.
- Prices/service IDs/Apply URLs: preserved.
- Apply JS: byte-identical to C0037.

## Boundary

No new design migration was performed. External URL Runtime remains UNVERIFIED. Real assistive-technology and physical-device testing remain NOT_EXECUTED. Production remains HOLD and promotion remains NOT_EXECUTED.
