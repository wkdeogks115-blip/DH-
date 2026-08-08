# SOURCE OF TRUTH

## Current

| Role | Current value | Status |
|---|---|---|
| Active Control | R0003 | LOCKED |
| Active Preview | C0009A D2 | unchanged |
| Current Review Candidate | C0038 | READY_NOT_PROMOTED |
| Direct parent / immediate rollback | C0037 | preserved |
| PC/Apply rollback | C0034 | preserved |
| Safety rollback / invariant source | C0033 | preserved |
| Brand-depth direction parent | C0032 | preserved |
| Secondary design rollback | C0031 | preserved |
| Functional rollback | C0022 | preserved |
| Latest Answer Pack | R34 | current review pack |
| Latest Handoff | A30 | current handoff |
| Production | HOLD | blocker remains |

## C0038 material result

C0038 is not a new visual migration. It is a focused accessibility repair produced by the site-wide Production-Blocker audit.

### Reproduced Parent defect

On C0037 `diagnose/`, a valid form submission made the recommendation result visible and scrolled it into view, but keyboard focus remained on the submit button. The generated result also lacked named region/live semantics.

### C0038 fix

The Diagnose result now uses:
- `role="region"`;
- `aria-labelledby="diagnose-result-title"`;
- `aria-live="polite"`;
- `aria-atomic="true"`;
- `tabindex="-1"`;
- valid generation moves focus to the result with `preventScroll:true`.

### Executed evidence

- Parent valid-result focus defect: REPRODUCED.
- Candidate valid-result focus: PASS.
- Candidate result semantics: PASS.
- Native invalid-form focus: PASS.
- Diagnose resting visual parity Desktop/Mobile: 2/2 zero changed pixels.
- Other 14 pages Desktop/Mobile: 28/28 zero changed pixels.
- C0033 safety acknowledgement runtime: PASS.
- application options: 23.
- application links: 86.
- prices: preserved.
- service IDs: preserved.
- Apply URLs: preserved.
- Apply JS: byte-identical to C0037.

## Current hashes

- C0038 Candidate: `b1c2628e02de28c3ccabc1247513bab4db93d2a6ee04427c1fd951025bde1114`
- R34 Answer Pack: `b4be02e2166bb9530bbd56baa569d6f3aed8a851d903830d1d695e6f9291824a`
- C0038 Local Review V32: `a7da5e00b8f664d81685e722778e8f8259717e6c72bf4e62629cb7b523d1ea63`
- C0038 Browser Evidence: `cc9ee523b17cdba1c8549c698d69d33bf4c421b94bec7d7296a0702bbac4a268`
- A30 Handoff: `7291c56e434d981260fc1a1d8b871bbf4b42c911dbf4c7b53b92e02470518662`

## Unverified

- Actual external URL Runtime: UNVERIFIED
- Real mobile device: NOT_EXECUTED
- Assistive technology: NOT_EXECUTED
- User conversion test: NOT_EXECUTED

## Promotion boundary

GitHub storage does not promote C0038. `/upgrade-auto` remains required before Active Control/Preview changes. Production remains HOLD.

## Next

C0039 is an integrated promotion-readiness audit from Active Preview C0009A D2 through current Review Candidate C0038. Do not create another design Candidate unless a new material defect is reproduced.
