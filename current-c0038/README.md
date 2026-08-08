# C0038 — Diagnose Result Focus

Status: `READY_NOT_PROMOTED`

Direct parent: C0037
Candidate SHA-256: `b1c2628e02de28c3ccabc1247513bab4db93d2a6ee04427c1fd951025bde1114`

## Material Delta

C0037 `diagnose/` generated a valid recommendation result but left keyboard focus on the submit button. The result also lacked named region/live semantics.

C0038 fixes only that accessibility transition:
- `role="region"`
- `aria-labelledby="diagnose-result-title"`
- `aria-live="polite"`
- `aria-atomic="true"`
- `tabindex="-1"`
- valid generation moves focus to the result with `preventScroll:true`

## Executed evidence

- parent focus defect: REPRODUCED
- candidate result focus: PASS
- result semantics: PASS
- native invalid-form focus: PASS
- Diagnose static visual parity Desktop/Mobile: 2/2 zero changed pixels
- other 14 pages Desktop/Mobile: 28/28 zero changed pixels
- C0033 safety acknowledgement runtime: PASS
- application options: 23
- application links: 86
- prices/service IDs/Apply URLs: preserved
- Apply JS: byte-identical to C0037

## Boundary

This is a Review Candidate only. It does not change Active Preview C0009A D2, does not authorize deployment and does not clear Production HOLD. `/upgrade-auto` is still required for promotion.
