# DH C0037 Remaining Utility / Trust Surface Audit V1

## Decision
A material inconsistency was reproduced on **game/** only. C0037 therefore changes only `game/`; it does not blanket-migrate the other audited surfaces.

| Surface | Classification | Evidence / rationale |
|---|---|---|
| `game/` | **MIGRATE** | C0036 displayed Orange, Mint and Cyan primary actions on one page. This conflicts with the current single restrained Cyan action family and is high-salience. |
| `partners/` | **KEEP** | Primary actions are already Cyan; B2B flow is task-led and no material route/overflow/trust defect was reproduced. |
| `cases/` | **KEEP** | Proof-first source layout and Cyan/Ghost hierarchy are already coherent. |
| `reviews/` | **KEEP** | Review evidence cards are semantically justified and source actions remain clear. |
| `policies/` | **KEEP** | Policy/trust utility benefits from restrained document-like presentation; more depth would be decorative. |
| `diagnose/` | **KEEP** | Interactive diagnosis should remain utilitarian; no task or overflow defect reproduced. |
| `404` | **KEEP** | Minimal recovery task is already clear; extra visual treatment would not improve completion. |

## C0037 correction
- keeps all game copy, LoL service identity, price, review/source links and Apply routes;
- unifies all vivid primary game actions to one Cyan family;
- adds selective depth to hero proof, decision rail, price object, report and final CTA without restoring glow/card overload.

## Executed gates
- Game mobile height: 6,444 → 6,384 px (-0.931%).
- Game horizontal overflow: 0.
- Other 14 pages × Desktop/Mobile: **28/28 zero changed pixels**.
- C0033 safety/form runtime gate: PASS.
- Application options: 23.
- Application links: 86.
- Prices / service IDs / Apply URLs: preserved.
- Apply JS: byte-identical to C0036.

External URL Runtime remains UNVERIFIED. Real-device and assistive-technology tests remain NOT_EXECUTED.
