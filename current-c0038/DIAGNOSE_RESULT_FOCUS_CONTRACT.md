# C0038 Diagnose Result Focus Contract

Direct parent: C0037.

## Reproduced defect

A valid Diagnose submission revealed the result and scrolled it into view, but keyboard focus remained on the submit button. The generated result did not expose a named region/live transition.

## Fix

- result `role="region"`
- `aria-labelledby="diagnose-result-title"`
- `aria-live="polite"`
- `aria-atomic="true"`
- `tabindex="-1"`
- after valid generation, move focus to the result with `focus({preventScroll:true})`

## Scope boundary

Only Diagnose result semantics/focus are changed.

Must preserve:
- C0037 Game consistency;
- C0036 YouTube + Editing;
- C0035 Rescue + Stream Ready;
- C0034 PC + Apply;
- C0032 Home + Creator Hub;
- C0033 safety acknowledgement runtime;
- 23 application options;
- 86 application links;
- prices, service IDs and Apply URLs;
- Apply JS byte identity.

No visual migration, testimonial, pricing, service-content or route change is authorized by this Candidate.
