# NEXT ACTION — C0034 PC + APPLY BRAND-DEPTH EXTENSION

## Baseline

- Active Control: R0003
- Active Preview: C0009A D2
- Current Review Candidate: C0033
- C0033 SHA: `db4659fb9f7f28ac4ce03c43f71472391a2badcdcc0db1762c281356cc49ad68`
- Direct parent / design rollback: C0032
- Secondary design rollback: C0031
- Functional rollback: C0022
- C0032 direction prototype heuristic: 88/100 (heuristic only)
- Functional prototype heuristic: 84/100
- Production: HOLD
- Actual external URL Runtime: UNVERIFIED

## Mandatory C0033 safety invariant

Any C0034 Apply visual change must re-execute the actual candidate `apply.js` and prove:

1. both `safety_ack` and `scope_ack` unchecked → no summary; exactly those two acknowledgement errors once other required data is valid;
2. safety only → `scope_ack` remains required;
3. both checked → summary generated;
4. error summary focus works;
5. blocked submission preserves existing inputs;
6. one availability time remains rejected by the 2-time rule;
7. mobile horizontal overflow remains zero.

Do not regress to the C0032 unchecked-checkbox behavior.

## C0034 design scope

Only:
- PC pricing / scope page;
- Apply page presentation.

Use the C0032 design direction:
- keep C0031 information hierarchy;
- keep semantic tokens and single-primary-CTA logic;
- restore only selective navy/cyan depth;
- group important decision surfaces;
- use elevation only for a small number of primary anchors;
- avoid glow-heavy buttons, independent cards everywhere, bright multi-color gradients and billboard typography.

## Required regression gate

- Home + Creator Hub C0032 visual direction preserved;
- Rescue + Stream Ready + YouTube + Editing preserved;
- non-target Desktop/Mobile comparisons: zero changed pixels;
- application options 23;
- application links 86;
- prices/service IDs/Apply URLs preserved.

## Stop conditions

- the PC/Apply version becomes merely more decorative rather than more trustworthy/readable;
- Apply mobile compression becomes materially worse;
- any C0033 safety acknowledgement regression;
- any non-target visual regression;
- accessibility or form behavior regression.

## Promotion boundary

C0033/C0034 remain Review Candidates. Do not promote or deploy without `/upgrade-auto`.
