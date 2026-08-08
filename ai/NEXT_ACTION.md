# NEXT ACTION — C0036 YOUTUBE + EDITING BRAND-DEPTH EXTENSION

## Baseline

- Active Control: R0003
- Active Preview: C0009A D2
- Current Review Candidate: C0035
- C0035 SHA: `c9369108b2f1fb39df78583c23700c6bfe083f1f0e0a42bf6b054b2edd7a217c`
- Direct parent / immediate rollback: C0034
- Safety invariant source: C0033
- Brand-depth direction parent: C0032
- Production: HOLD
- Actual external URL Runtime: UNVERIFIED

## C0036 scope

Only:
- `creator/youtube/`
- `creator/editing/`

Use the validated C0032/C0034/C0035 design language:
- preserve C0031 information hierarchy;
- selective navy/cyan depth only at major decision anchors;
- one strong primary accent family;
- grouped decision/pricing surfaces;
- avoid bright multi-color gradients, glow-heavy buttons, billboard typography and independent-card repetition.

## Mandatory regression gate

- C0035 Rescue + Stream Ready unchanged;
- C0034 PC + Apply unchanged;
- C0032 Home + Creator Hub unchanged;
- C0033 safety acknowledgement runtime remains mandatory;
- non-target Desktop/Mobile pixel comparison: zero changed pixels;
- application options 23;
- application links 86;
- prices/service IDs/Apply URLs preserved;
- target horizontal overflow zero.

## Stop conditions

- Creator-detail pages become visually heavier without clearer decisions;
- color identity becomes multi-accent again;
- any C0033 safety behavior regression;
- any non-target visual regression;
- accessibility or route/data regression.

## Promotion boundary

C0035/C0036 remain Review Candidates. Do not promote or deploy without `/upgrade-auto`.
