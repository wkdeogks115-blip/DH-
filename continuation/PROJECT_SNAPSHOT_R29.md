# DH PROJECT SNAPSHOT R29

## Locked state

- Active Control: R0003
- Active Preview: C0009A D2
- Current Review Candidate: C0033
- Direct parent / design rollback: C0032
- Secondary visual-direction rollback: C0031
- Functional rollback: C0022
- Latest Answer Pack: R29
- Latest Handoff: A25
- Production: HOLD
- Promotion: NOT_EXECUTED

## Why C0033 changed scope

C0033 was originally scheduled to extend the C0032 brand-depth direction to PC + Apply. During real Apply interaction testing, a higher-priority runtime bug was reproduced in C0032: the two required safety acknowledgement checkboxes were treated as complete even when unchecked.

The incomplete design-extension attempt was discarded. C0033 was reassigned to the validation bug only.

## Parent defect

With valid service, issue, schedule and two availability slots, while both `safety_ack` and `scope_ack` remained unchecked:

- C0032 generated the application summary.
- no safety acknowledgement errors were shown.

Root cause: the generic form value helper returned the `.value` of an unchecked single checkbox.

## C0033 result

- Candidate SHA-256: `db4659fb9f7f28ac4ce03c43f71472391a2badcdcc0db1762c281356cc49ad68`
- both safety boxes unchecked → summary blocked
- errors → `safety_ack`, `scope_ack`
- safety only → `scope_ack` remains
- both checked → summary generated
- empty candidate form → 6 errors because Kakao handoff is default-selected
- error-summary focus → PASS
- blocked-submit input preservation → PASS
- Home/PC/Apply static visual parity → 6/6 zero changed pixels
- application options → 23
- application links → 86
- prices/service IDs/Apply URLs → PRESERVED

## Validation status

- Candidate ZIP CRC: PASS
- deterministic rebuild: PASS
- JavaScript syntax: PASS
- Node validation simulation: PASS
- self-contained Chromium actual Apply interaction: PASS
- actual external URL Runtime: UNVERIFIED
- real mobile device: NOT_EXECUTED
- assistive technology: NOT_EXECUTED
- user conversion test: NOT_EXECUTED

## Design direction

C0032 brand-depth direction remains the latest design-direction prototype and remains a valid parent. C0033 does not visually redesign the site.

Next C0034 resumes the deferred PC + Apply brand-depth extension, but the C0033 safety-validation behavior becomes a mandatory invariant.

## Promotion boundary

Do not promote or deploy C0033 without `/upgrade-auto`. Active Control R0003 and Active Preview C0009A D2 remain unchanged.
