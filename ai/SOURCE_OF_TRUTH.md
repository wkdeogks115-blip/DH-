# SOURCE OF TRUTH

## Current

| Role | Current value | Status |
|---|---|---|
| Active Control | R0003 | LOCKED |
| Active Preview | C0009A D2 | unchanged |
| Current Review Candidate | C0030 | READY_NOT_PROMOTED |
| Direct parent / visual rollback | C0029 | preserved |
| Functional rollback | C0022 | preserved |
| Latest Answer Pack | R26 | current review pack |
| Latest Handoff | A22 | current handoff |
| Production | HOLD | blocker remains |

## C0030 material result

- Only `rescue/` and `stream-ready/` migrated to the approved reusable visual shell.
- Rescue mobile document height reduced by 13.029%.
- Stream Ready mobile document height reduced by 12.937%.
- Service-page commercial visual heuristic: 70 → 80.
- Overall site design heuristic remains 80; functional prototype heuristic remains 84.
- Home, PC pricing and Apply desktop/mobile were re-rendered after the shared CSS change: 6/6 comparisons returned zero changed pixels.
- 23 application options and 86 application links preserved.
- Prices, service IDs and Apply URLs preserved.
- Static QA PASS; no horizontal overflow in targeted service renders.
- An intermediate broad mobile-container rule changed core mobile pages and was rejected. Only the corrected C0030 artifact is valid.
- Actual external URL Runtime UNVERIFIED; real device, assistive technology and user conversion NOT_EXECUTED.

## Current hashes

- C0030 Candidate: `e3caadb915360ab36fa9cbbc9bc13feddbfb29f2ccc97d32a916371cf0ba1bbd`
- R26 Answer Pack: `e4bf48a30fc35c00ec065e79b5f384f492c94b514ebcdcf64397258a496238c2`
- C0030 Local Review V24: `9c529827a6f31dd53837da16bdf70c340ec28d3b4cb97488216f36b14ab072bf`
- C0030 Visual Evidence: `37a54706e436b0cc2c96c0888fed4935036e1b53ac5bf2f23d7df9f9ad6a4be0`
- A22 Handoff local source hash: `32f229ccb7726e3208be0ee107a8da1ede730c3305b59b9bbaec6fc094e91d9f`

## Promotion boundary

GitHub storage does not promote C0030. `/upgrade-auto` is still required before Active Control/Preview changes. Production remains HOLD.

## Next

Use C0030 as immutable visual parent. C0031 should migrate the approved shell to `creator/`, `creator/youtube/`, and `creator/editing/` only. Preserve C0030 Rescue/Stream Ready and C0029 Apply behavior. Do not combine policies/cases/reviews in the same Candidate.
