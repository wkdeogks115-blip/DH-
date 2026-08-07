# SOURCE OF TRUTH

## Current

| Role | Current value | Status |
|---|---|---|
| Active Control | R0003 | LOCKED |
| Active Preview | C0009A D2 | unchanged |
| Current Review Candidate | C0029 | READY_NOT_PROMOTED |
| Direct parent / visual rollback | C0028 | preserved |
| Functional rollback | C0022 | preserved |
| Latest Answer Pack | R25 | current review pack |
| Latest Handoff | A21 | current handoff |
| Production | HOLD | blocker remains |

## C0029 material result

- Mobile Apply task density reduced without changing business logic.
- 390×844 initial document height: 4,903 → 3,390 px (-30.859%).
- Generated-summary document height: 5,325 → 4,359 px (-18.141%).
- Progress shell: 146 → 94 px; form height: 2,549 → 1,903 px.
- Empty application summary is hidden on mobile until a valid summary is generated.
- Stage 3 secondary option text is visually compressed; primary option names remain visible and text remains in DOM.
- Safety acknowledgement explanations remain visible.
- Actual `js/apply.js` executed in self-contained Chromium: one-time availability rejection, error-summary focus, input retention and valid two-time summary generation PASS.
- Desktop C0028/C0029 changed pixels: 0.
- `js/apply.js` bytes and Apply form control signature are identical to C0028.
- 23 application options and 86 application links preserved.
- Prices, service IDs and apply URLs preserved.
- Static QA PASS.
- Actual external URL Runtime UNVERIFIED; real device, assistive technology and user conversion NOT_EXECUTED.

## Current hashes

- C0029 Candidate: `ba0de866143c9c68a3c5c0e9804390afeacbd43969c1dd8e135a804a59789930`
- R25 Answer Pack: `620564f8ac4e2747a8fbaf53dedb62c10c6d1399eb538b5bcccc013b3ce0a0d5`
- C0029 Local Review V23: `a138f18ba2b5428de7f8643b4534fff7701b7c3ba18272b238c9ca8926397501`
- C0029 Visual Evidence: `e5f17571fa8f6fda78722d24fc5048451e37baffc2296a6870c23e5c3ba02134`
- A21 Handoff local source hash: `73de4301cfa0258fd02e9d11037cb1606714063fb50edd190501ee005a0180c1`

## Promotion boundary

GitHub storage does not promote C0029. `/upgrade-auto` is still required before Active Control/Preview changes. Production remains HOLD.

## Next

Use C0029 as immutable visual parent. C0030 should migrate the approved reusable visual shell to `rescue/` and `stream-ready/` only. Preserve C0029 Apply behavior and do not expand into Creator pages in the same Candidate.
