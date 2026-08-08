# SOURCE OF TRUTH

## Current

| Role | Current value | Status |
|---|---|---|
| Active Control | R0003 | LOCKED |
| Active Preview | C0009A D2 | unchanged |
| Current Review Candidate | C0036 | READY_NOT_PROMOTED |
| Direct parent / immediate rollback | C0035 | preserved |
| PC/Apply rollback | C0034 | preserved |
| Safety rollback / invariant source | C0033 | preserved |
| Brand-depth direction parent | C0032 | preserved |
| Secondary design rollback | C0031 | preserved |
| Functional rollback | C0022 | preserved |
| Latest Answer Pack | R32 | current review pack |
| Latest Handoff | A28 | current handoff |
| Production | HOLD | blocker remains |

## C0036 material result

C0036 extends the validated selective Brand Depth language only to `creator/youtube/` and `creator/editing/`, using C0035 as the direct parent.

### Design outcome

- creator-detail trust / visual anchoring: 80 → 87;
- package decision clarity: 84 → 88;
- cross-page brand consistency: 82 → 90;
- overall Brand Depth direction heuristic: 88 maintained;
- functional prototype heuristic: 84 maintained;
- YouTube mobile height: 8,460px → 8,444px (-0.189%);
- Editing mobile height: 8,524px → 8,497px (-0.317%).

The Creator Detail pages keep the C0031 information hierarchy. Hero proof, service choice, pricing and route/result areas gain selective depth. Existing purple Creator/Editing primary CTAs are normalized to a restrained Cyan family.

### Mandatory C0033 safety gate

The actual candidate `apply.js` is byte-identical to C0035 and was executed in self-contained Chromium:
- empty form → 6 errors + error-summary focus PASS;
- both `safety_ack` and `scope_ack` unchecked with other required data valid → no summary, errors exactly `safety_ack`, `scope_ack`;
- safety only → `scope_ack` remains;
- one availability time → rejected by the 2-time rule;
- blocked submission → issue/time inputs preserved;
- both safety acknowledgements + two availability times → summary generated;
- mobile horizontal overflow → 0.

### Regression / business invariants

- Home + Creator Hub + PC + Apply + Rescue + Stream Ready Desktop/Mobile: 12/12 zero changed pixels;
- target YouTube/Editing horizontal overflow: 0;
- application options: 23;
- application links: 86;
- prices: preserved;
- service IDs: preserved;
- Apply URLs: preserved.

## Current hashes

- C0036 Candidate: `ee9bda1f4dfa0ff47e2b155640250a63c270062a61d3c82981f6deb58e33ea87`
- R32 Answer Pack: `b4a649b8bc7e5de76e85a9795ede06815dad5a4be286144f73bafe6c2d5802ff`
- C0036 Local Review V30: `5cbb29fab73318899755dc675f851a1974a27ad9d3a8098069b8acf7c8c0f1f7`
- C0036 Browser Evidence: `829dd2ab2b415f023bd0be11a7a28fa6f4710d204119b5fe6558246668830064`
- A28 Handoff: `ef8d7a21fefec174ce8364bfc967b28395922e4e5a85dadecc3ab31f57bb69ac`

## Unverified

- Actual external URL Runtime: UNVERIFIED
- Real mobile device: NOT_EXECUTED
- Assistive technology: NOT_EXECUTED
- User conversion test: NOT_EXECUTED

## Promotion boundary

GitHub storage does not promote C0036. `/upgrade-auto` remains required before Active Control/Preview changes. Production remains HOLD.

## Next

C0037 audits the remaining utility/trust surfaces first: `game/`, `partners/`, `cases/`, `reviews/`, `policies/`, `diagnose/`, `404`. Build only where a material inconsistency is reproduced.
