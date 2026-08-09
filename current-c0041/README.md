# C0041 — Human-Craft Refinement

Status: `READY_FOR_CONTROL_PLANE_REVIEW_NOT_PROMOTED`

Active Control remains **R0004**. Active Preview remains **C0038**.

Candidate SHA-256: `cfc16576777f8da9b46d54ce174bd496e1c85bc56b9030c155713aa7e2ddfe23`
Direct parent: **C0040**.

## Material Delta

C0040 fixed the main dark/AI-template problem but fresh A/B visual QA found residual template grammar:
- Home/PC still used rounded white dashboard-like Hero objects;
- Home/PC Hero structure remained too similar;
- Apply still used decorative status pills and a rounded floating progress-card treatment;
- Hero heading scale remained slightly billboard-like.

C0041 changes only those visual patterns:
- Home: flat Service Ledger + calmer hero typography;
- PC: desktop integrated Diagnostic Scale + mobile flat paper diagnostic strip;
- Apply: plain metadata + rule-based journey rail; actual input/summary surfaces remain cards.

## Executed Gates

- Candidate CRC: PASS
- Deterministic rebuild: PASS
- Static gate: PASS
- Runtime routes: 15
- Apply safety/form runtime: PASS
- 320px Home/PC/Apply overflow: 0
- non-target 12 pages × Desktop/Mobile: PASS 24/24 zero changed pixels
- application options: 23
- application links: 86
- service IDs: 23
- prices / Apply URLs: preserved
- Apply JS: byte-identical to C0040
- Preview noindex guard: PASS

## Visual heuristic

- Home 94
- PC 92
- Apply 95
- Direction 93.7

Heuristic only; not conversion evidence.

## Boundary

C0041 is **not Active**, is **not deployed**, and does not clear Production HOLD. Control Plane review is next. Explicit `/upgrade-auto` remains required for any promotion.