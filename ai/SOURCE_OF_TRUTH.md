# SOURCE OF TRUTH

## Current

| Role | Current value | Status |
|---|---|---|
| Active Control | R0003 | LOCKED |
| Active Preview | C0009A D2 | unchanged |
| Current Review Candidate | C0031 | READY_NOT_PROMOTED |
| Direct parent / visual rollback | C0030 | preserved |
| Functional rollback | C0022 | preserved |
| Latest Answer Pack | R27 | current review pack |
| Latest Handoff | A23 | current handoff |
| Production | HOLD | blocker remains |

## C0031 material result

- Only `creator/`, `creator/youtube/`, and `creator/editing/` migrated to the approved visual language.
- Creator Hub uses an editorial hero and one service-choice rail.
- YouTube and Editing use the same evidence/choice/pricing hierarchy as Rescue and Stream Ready.
- Creator-family commercial visual heuristic: 68 → 80.
- Overall site design heuristic remains 80; functional prototype heuristic remains 84.
- Mobile height: Creator Hub 3,274 → 3,243 px; YouTube 9,095 → 8,460 px; Editing 8,814 → 8,524 px.
- Home, PC pricing, Apply, Rescue and Stream Ready were re-rendered Desktop+Mobile: 10/10 comparisons returned zero changed pixels.
- 23 application options and 86 application links preserved.
- Prices, service IDs and Apply URLs preserved.
- Static QA PASS; target Creator renders have no horizontal overflow.
- An intermediate Creator Hub mobile draft produced 16px horizontal overflow and was rejected before final packaging.
- Actual external URL Runtime UNVERIFIED; real device, assistive technology and user conversion NOT_EXECUTED.

## Current hashes

- C0031 Candidate: `45d1b8d7fd70fcfe16ce450c6fe5ad4957b26c40cf4bb3b3924260a2863e3ddd`
- R27 Answer Pack: `23f8c4ea999b7f5cd743b640ffde072370d4e2418024fa5720cdb595500ac741`
- C0031 Local Review V25: `eae4741523450f0170ff28aee270d78490a93091bbf583da18014b70516c65b5`
- C0031 Visual Evidence: `45ee15fb87a072658514ff718a8152f0246077e38898dad4be6435b625345716`
- A23 Handoff local source hash: `a65d79d0ccd2158ca76b0a99f9ed9ac2e7ab28d3f0e8b82d06e44b7af28c530c`

## Promotion boundary

GitHub storage does not promote C0031. `/upgrade-auto` is still required before Active Control/Preview changes. Production remains HOLD.

## Next

C0032 is an audit-first step. Inspect `game/`, `partners/`, `cases/`, `reviews/`, `policies/`, `diagnose/` and 404 for material visual or task inconsistency. Do not create another redesign Candidate merely to make every page look identical; build only where evidence supports a material improvement.
