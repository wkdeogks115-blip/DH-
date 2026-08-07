# C0033 — Safety Acknowledgement Validation Fix

Status: `READY_NOT_PROMOTED`

Direct parent: C0032 `66fa34cbe48977aa9a0bd1dcc906e45975da38828b59818e2803954b8f468464`

Candidate SHA-256: `db4659fb9f7f28ac4ce03c43f71472391a2badcdcc0db1762c281356cc49ad68`

## Material defect reproduced in C0032

The Apply helper read the `.value` of a single checkbox even when the checkbox was not checked. Therefore the required `safety_ack` and `scope_ack` fields were treated as completed when both were visibly unchecked.

Browser reproduction on C0032:
- safety checkbox: unchecked
- scope checkbox: unchecked
- all other required data valid
- application summary generated: **YES — defect**

## C0033 correction

For a single checkbox/radio `HTMLInputElement`, the value helper now returns the field value only when `.checked === true`.

Executed candidate browser evidence:
- both safety boxes unchecked → summary blocked; errors `safety_ack`, `scope_ack`
- safety only → `scope_ack` remains required
- both checked → summary generated
- empty form → 6 errors because Kakao handoff is intentionally default-selected
- error-summary focus → PASS
- failed-submit input preservation → PASS

## Preserved

- application options: 23
- application links: 86
- prices: preserved
- service IDs: preserved
- Apply URLs: preserved
- CSS: byte-identical to C0032
- Home/PC/Apply static visual parity: 6/6 zero changed pixels

## Boundary

This GitHub record does not promote C0033. Active Control remains R0003, Active Preview remains C0009A D2, Production remains HOLD, and `/upgrade-auto` is still required for promotion.
