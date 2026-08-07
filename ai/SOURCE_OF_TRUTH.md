# SOURCE OF TRUTH

## Current

| Role | Current value | Status |
|---|---|---|
| Active Control | R0003 | LOCKED |
| Active Preview | C0009A D2 | unchanged |
| Current Review Candidate | C0033 | READY_NOT_PROMOTED |
| Direct parent / design rollback | C0032 | preserved |
| Secondary design rollback | C0031 | preserved |
| Functional rollback | C0022 | preserved |
| Latest Answer Pack | R29 | current review pack |
| Latest Handoff | A25 | current handoff |
| Production | HOLD | blocker remains |

## C0033 material result

While preparing the planned PC + Apply design extension, real Apply interaction testing reproduced a higher-priority C0032 validation defect.

### Parent defect

With all core application data valid and both required safety acknowledgement checkboxes visibly unchecked, C0032 generated the application summary. The generic value helper returned the checkbox HTML value even when `.checked` was false.

### Candidate correction

C0033 returns a single checkbox/radio value only when the input is checked.

Executed self-contained Chromium evidence:
- C0032 both safety boxes unchecked → summary generated, no acknowledgement errors;
- C0033 both unchecked → summary blocked, errors `safety_ack` + `scope_ack`;
- C0033 safety only → `scope_ack` remains;
- C0033 both checked → summary generated;
- C0033 empty form → 6 errors because Kakao handoff is intentionally default-selected;
- error-summary focus → PASS;
- failed-submit input preservation → PASS.

Business invariants:
- application options: 23;
- application links: 86;
- prices: preserved;
- service IDs: preserved;
- Apply URLs: preserved;
- CSS: unchanged from C0032;
- Home/PC/Apply Desktop+Mobile static visual parity: 6/6 zero changed pixels.

## Design direction

C0032 remains the current design-direction prototype: C0031 hierarchy plus selective navy/cyan depth and grouped decision surfaces. C0033 does not replace that direction; it fixes the safety acknowledgement runtime behavior on top of C0032.

## Current hashes

- C0033 Candidate: `db4659fb9f7f28ac4ce03c43f71472391a2badcdcc0db1762c281356cc49ad68`
- R29 Answer Pack: `d2a2500f66de62b23301605247dca64af486d4561766b1bae5439b9891e31c67`
- C0033 Local Review V27: `fc8f25f888ba445a19c635bc7cfee3ea803d216def04242eebf06ca381e9bd32`
- C0033 Final Audit R29 local hash: `9dead505d158c178e552e7b22f82da623129de7f6ad1af4515c958b8ef6e19d3`
- C0033 Runtime Audit local hash: `0c507f7bb3039255e99d2ea3e7a12559f44e75701c8ddf585335f1a0ad6eba6b`
- A25 Handoff local source hash: `78be44482cd8a05a3a3749716a91c71ab90f538b6892c77fcc38a0077b6953d2`

## Unverified

- Actual external URL Runtime: UNVERIFIED
- Real mobile device: NOT_EXECUTED
- Assistive technology: NOT_EXECUTED
- User conversion test: NOT_EXECUTED

## Promotion boundary

GitHub storage does not promote C0033. `/upgrade-auto` is still required before Active Control/Preview changes. Production remains HOLD.

## Next

C0034 resumes the deferred PC + Apply selective Brand Depth extension. C0033 safety acknowledgement behavior is now a mandatory invariant and must be executed again after any Apply visual change.
