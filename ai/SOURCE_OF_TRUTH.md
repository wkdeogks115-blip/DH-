# SOURCE OF TRUTH

## Current

| Role | Current value | Status |
|---|---|---|
| Active Control | R0003 | LOCKED |
| Active Preview | C0009A D2 | unchanged |
| Current Review Candidate | C0035 | READY_NOT_PROMOTED |
| Direct parent / immediate rollback | C0034 | preserved |
| Safety rollback / invariant source | C0033 | preserved |
| Brand-depth direction parent | C0032 | preserved |
| Secondary design rollback | C0031 | preserved |
| Functional rollback | C0022 | preserved |
| Latest Answer Pack | R31 | current review pack |
| Latest Handoff | A27 | current handoff |
| Production | HOLD | blocker remains |

## C0035 material result

C0035 extends the validated selective Brand Depth language to only `rescue/` and `stream-ready/`, using C0034 as the direct parent.

### Design outcome

- service trust / visual anchoring heuristic: 80 → 87;
- decision comparison clarity: 84 → 88;
- overall Brand Depth direction heuristic: 88 maintained;
- functional prototype heuristic: 84 maintained;
- Rescue mobile height: 7,296px → 7,335px (+0.535%);
- Stream Ready mobile height: 7,295px → 7,224px (-0.973%).

A first visual audit found a residual purple Stream Ready primary CTA. That intermediate result was rejected. The final C0035 uses a Cyan-family primary accent on the target pages.

### Mandatory C0033 safety gate

The actual candidate `apply.js` is byte-identical to C0034 and was executed in self-contained Chromium:
- empty form → 6 errors + error-summary focus PASS;
- both `safety_ack` and `scope_ack` unchecked with other required data valid → no summary, errors exactly `safety_ack`, `scope_ack`;
- safety only → `scope_ack` remains;
- one availability time → rejected by the 2-time rule;
- blocked submission → issue/time inputs preserved;
- both safety acknowledgements + two availability times → summary generated;
- mobile horizontal overflow → 0.

### Regression / business invariants

- Home + Creator Hub + PC + Apply + YouTube + Editing Desktop/Mobile: 12/12 zero changed pixels;
- target Rescue/Stream horizontal overflow: 0;
- application options: 23;
- application links: 86;
- prices: preserved;
- service IDs: preserved;
- Apply URLs: preserved.

## Current hashes

- C0035 Candidate: `c9369108b2f1fb39df78583c23700c6bfe083f1f0e0a42bf6b054b2edd7a217c`
- R31 Answer Pack: `71c3425d46424e3b8957502259421f5b6a4c5cd945c9860923a684f42181c41f`
- C0035 Local Review V29: `2f67f47ea68bfee7d493fb4d7d87674374acbd7c3cdcf702b3ce5f9d8ef05edb`
- C0035 Browser Evidence: `23cd3d4e4b7c2acc9dde0b625f807c405e35363ebef7c3fba58337ce06ace062`
- A27 Handoff: `9ecb1ee6a1e36c3a96730225ee13057ef25ea5bca9bd1431265e78a4757e4e93`

## Unverified

- Actual external URL Runtime: UNVERIFIED
- Real mobile device: NOT_EXECUTED
- Assistive technology: NOT_EXECUTED
- User conversion test: NOT_EXECUTED

## Promotion boundary

GitHub storage does not promote C0035. `/upgrade-auto` remains required before Active Control/Preview changes. Production remains HOLD.

## Next

C0036 should extend the validated Brand Depth language to only YouTube + Editing creator-detail pages, preserving C0035 service pages, C0034 PC/Apply and the C0033 safety gate.
