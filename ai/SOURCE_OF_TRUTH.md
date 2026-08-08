# SOURCE OF TRUTH

## Current

| Role | Current value | Status |
|---|---|---|
| Active Control | R0003 | LOCKED |
| Active Preview | C0009A D2 | unchanged |
| Current Review Candidate | C0034 | READY_NOT_PROMOTED |
| Direct parent / immediate rollback | C0033 | preserved |
| Brand-depth direction parent | C0032 | preserved |
| Secondary design rollback | C0031 | preserved |
| Functional rollback | C0022 | preserved |
| Latest Answer Pack | R30 | current review pack |
| Latest Handoff | A26 | current handoff |
| Production | HOLD | blocker remains |

## C0034 material result

C0034 extends the C0032 selective Brand Depth direction to only `pc/` and `apply/`, but uses C0033 as its direct parent so the safety acknowledgement validation fix remains mandatory.

### Design outcome

- PC commercial clarity heuristic: 80 → 87;
- Apply trust/completion heuristic: 82 → 88;
- overall Brand Depth direction heuristic: 88 maintained;
- functional prototype heuristic: 84 maintained;
- PC mobile height: 8,439px → 7,871px (-6.731%);
- Apply mobile height: 3,390px → 3,457px (+1.976%), within the 8% compression guard.

### Mandatory C0033 safety gate

The actual candidate `apply.js` is byte-identical to C0033 and was executed in self-contained Chromium:
- empty form → 6 errors + error-summary focus PASS;
- both `safety_ack` and `scope_ack` unchecked with other required data valid → no summary, errors exactly `safety_ack`, `scope_ack`;
- safety only → `scope_ack` remains;
- one availability time → rejected by the 2-time rule;
- blocked submission → issue/time inputs preserved;
- both safety acknowledgements + two availability times → summary generated;
- mobile horizontal overflow → 0.

### Regression / business invariants

- Home + Creator Hub + Rescue + Stream Ready + YouTube + Editing Desktop/Mobile: 12/12 zero changed pixels;
- application options: 23;
- application links: 86;
- prices: preserved;
- service IDs: preserved;
- Apply URLs: preserved.

## Current hashes

- C0034 Candidate: `55b1eee33f6c03c44ad627b69b952dfe1303fe07055dac35f966abea7d5fd263`
- R30 Answer Pack: `96e579fe097c254c600a821c82dfd2a7a4799d2539bb399d51f45808a73506c0`
- C0034 Local Review V28: `cd9c2c0f321ea811612a90a53062f0188bcfc7f5d3bcd23b1dd7b98e579b2ff8`
- C0034 Browser Evidence: `3000cfa3f711ac47e8c9bf00e104f27033282b0f17e209a4619e3b7ec47a5c3f`
- A26 Handoff: `29cbbe79c7065aea2412b0aff1ab10c425a348d957ca5c8d1b1d43827b69fa64`

## Unverified

- Actual external URL Runtime: UNVERIFIED
- Real mobile device: NOT_EXECUTED
- Assistive technology: NOT_EXECUTED
- User conversion test: NOT_EXECUTED

## Promotion boundary

GitHub storage does not promote C0034. `/upgrade-auto` remains required before Active Control/Preview changes. Production remains HOLD.

## Next

C0035 should extend the validated selective Brand Depth language to only Rescue + Stream Ready, preserving C0034 PC/Apply and all C0033 safety validation gates.
