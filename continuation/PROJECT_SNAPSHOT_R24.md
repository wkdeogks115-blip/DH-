# DH PROJECT SNAPSHOT R24 — C0028 Visual Shell Component Consolidation

## Locked control state

- Active Control: `R0003`
- Active Preview: `C0009A D2`
- Infrastructure: `BASELINE_LOCKED`
- Production: `HOLD`
- External Preview: `DEFERRED_BY_USER`
- Payment: `NOT_IMPLEMENTED`

## Current review lineage

- Current Review Candidate: `C0028`
- C0028 SHA-256: `4bdbe123a6e5860979f8af580a06ffd2407c63e2739ef802111679f679315cb7`
- Direct parent / visual rollback: C0027 `0db244b8f483e030d330d66f43b4d2bd262ed06460abf919209e627b996cdd7d`
- Functional rollback: C0022 `5f9e8749b02ff210e7a1729224e58a315e4cf023e59fc356c3529209c7af9128`
- Promotion: `NOT_EXECUTED`

## C0028 material result

C0028 does not change the approved C0027 appearance. It consolidates the temporary visual-shell layer for Home, PC pricing and Apply.

- Total runtime CSS: `187,722 → 181,422 bytes` (`-6,300`, `-3.356%`)
- Visual Shell CSS: `26,397 → 20,097 bytes` (`-6,300`, `-23.866%`)
- Repeated long visual-shell scope prefix occurrences: `164 → 0`
- `!important` declarations: `473 → 473` — still unresolved CSS debt
- Audited Desktop/Mobile views: 8
- Exact changed pixels: `0`
- JavaScript bytes: unchanged from C0027
- Application options: 23 preserved
- Application links: 86 preserved
- Prices, service IDs, apply URLs: preserved

## Validation

- Candidate ZIP CRC: PASS
- Deterministic rebuild: PASS
- Manifest / Inventory: PASS
- HTML / JS syntax / CSS / local references / fragments / IDs / Alt / JSON-LD: PASS
- Self-contained Chromium static visual parity: PASS, 0 changed pixels
- Actual URL Browser Runtime: `UNVERIFIED`
- Real mobile device: `NOT_EXECUTED`
- Assistive technology: `NOT_EXECUTED`
- User conversion test: `NOT_EXECUTED`

## Current design score

- C0027: 80/100
- C0028: 80/100
- Functional prototype heuristic: 84/100 maintained

The score does not increase because C0028 intentionally preserves the same rendered design.

## Latest package identities

- Answer Pack: R24 `b1f1ea366e18235f29d228c5e925e8e3c2725130f4d3ded7ebee0f4493f32207`
- Local Review V22: `9b769b6c414a73a2d9f2c2f1e6f6644df612f194b1b00aaf3cdc742f5b422df3`
- Browser Visual Evidence: `6d637f530d87a562ab88b2c5e17c8a73d2c8a7b73044f7f2dce688e84ef50c26`
- Latest Handoff: A20

## Next controlled work

Use C0028 as immutable visual parent. The current first-choice user-facing improvement is Apply mobile decision/scroll compression while preserving all validation, focus recovery, input retention, accessibility, product and pricing invariants. Do not promote or deploy without `/upgrade-auto`.