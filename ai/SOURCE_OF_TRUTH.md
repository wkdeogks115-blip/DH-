# SOURCE OF TRUTH

## Current

| Role | Current value | Status |
|---|---|---|
| Active Control | R0003 | LOCKED |
| Active Preview | C0009A D2 | unchanged |
| Current Review Candidate | C0028 | READY_NOT_PROMOTED |
| Direct parent / visual rollback | C0027 | preserved |
| Functional rollback | C0022 | preserved |
| Latest Answer Pack | R24 | current review pack |
| Latest Handoff | A20 | current handoff |
| Production | HOLD | blocker remains |

## C0028 material result

- C0027 rendered design preserved exactly on Home, PC pricing and Apply.
- 8 audited Desktop/Mobile screenshot views: 0 changed pixels.
- Runtime CSS: 187,722 → 181,422 bytes (-6,300; -3.356%).
- Visual Shell CSS: 26,397 → 20,097 bytes (-6,300; -23.866%).
- Long repeated scope prefix occurrences: 164 → 0.
- `!important`: 473 → 473; this remains unresolved debt.
- 23 application options and 86 application links preserved.
- Prices, service IDs and apply URLs preserved.
- All JavaScript bytes unchanged from C0027.
- Static QA PASS; self-contained Chromium visual parity PASS.
- Actual URL Runtime UNVERIFIED; real device, assistive technology and user conversion NOT_EXECUTED.

## Current hashes

- C0028 Candidate: `4bdbe123a6e5860979f8af580a06ffd2407c63e2739ef802111679f679315cb7`
- R24 Answer Pack: `b1f1ea366e18235f29d228c5e925e8e3c2725130f4d3ded7ebee0f4493f32207`
- C0028 Local Review V22: `9b769b6c414a73a2d9f2c2f1e6f6644df612f194b1b00aaf3cdc742f5b422df3`
- C0028 Visual Evidence: `6d637f530d87a562ab88b2c5e17c8a73d2c8a7b73044f7f2dce688e84ef50c26`
- A20 Handoff local source hash: `044ab03ea1976912a03a07750e1f72dac19b65998a0601fa498c8be0b8f5b3c5`

## Promotion boundary

GitHub storage does not promote C0028. `/upgrade-auto` is still required before Active Control/Preview changes. Production remains HOLD.

## Next

Use C0028 as immutable visual parent. Current first-choice C0029: reduce Apply mobile decision/scroll burden without changing validation, focus recovery, input retention, accessibility, products, prices, service IDs or URLs.