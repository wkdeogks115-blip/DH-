# C0034 — PC + Apply Brand Depth Review Candidate

Status: `READY_NOT_PROMOTED`

## Identity

- Candidate SHA-256: `55b1eee33f6c03c44ad627b69b952dfe1303fe07055dac35f966abea7d5fd263`
- Direct Parent: C0033
- Parent SHA-256: `db4659fb9f7f28ac4ce03c43f71472391a2badcdcc0db1762c281356cc49ad68`
- Active Control remains R0003
- Active Preview remains C0009A D2
- Production remains HOLD

## Scope

Only:
- `pc/`
- `apply/`

C0034 extends the selective navy/cyan Brand Depth direction into the two main conversion screens. It keeps the existing information architecture and uses grouped surfaces/elevation only for important decision anchors.

## Required safety behavior retained

C0034 keeps C0033 `apply.js` byte-identical. Executed Chromium evidence passed:

- empty form: 6 errors + summary focus;
- both safety boxes unchecked: no result, errors exactly `safety_ack` and `scope_ack`;
- safety only: `scope_ack` remains;
- one availability time: rejected;
- blocked submission: entered issue/time preserved;
- both safety acknowledgements and two times: result generated;
- mobile overflow: 0.

## Design results

- PC mobile page: 8,439 → 7,871 px (-6.731%)
- Apply mobile page: 3,390 → 3,457 px (+1.976%)
- PC commercial clarity heuristic: 80 → 87
- Apply trust/completion heuristic: 82 → 88
- Overall Brand Depth direction heuristic: 88 maintained

## Regression

Home, Creator, Rescue, Stream Ready, YouTube, Editing Desktop/Mobile: 12/12 zero changed pixels.

## Invariants

- application options: 23
- application links: 86
- prices: preserved
- service IDs: preserved
- Apply URLs: preserved

## Boundary

This directory documents a Review Candidate. It does not mean promotion or deployment. `/upgrade-auto` remains required.
