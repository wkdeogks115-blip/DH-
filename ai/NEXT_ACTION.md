# NEXT ACTION — C0037 REMAINING SURFACE AUDIT

## Baseline

- Active Control: R0003
- Active Preview: C0009A D2
- Current Review Candidate: C0036
- C0036 SHA: `ee9bda1f4dfa0ff47e2b155640250a63c270062a61d3c82981f6deb58e33ea87`
- Direct parent / immediate rollback: C0035
- PC/Apply rollback: C0034
- Safety invariant source: C0033
- Brand-depth direction parent: C0032
- Production: HOLD
- Actual external URL Runtime: UNVERIFIED

## C0037 scope

Audit first, do not migrate blindly:
- `game/`
- `partners/`
- `cases/`
- `reviews/`
- `policies/`
- `diagnose/`
- `404`

Classify each surface as:
- KEEP
- MINOR_FIX
- MIGRATE
- UNVERIFIED

Build a new Candidate only where a material task, trust, accessibility or visual inconsistency is actually reproduced.

## Mandatory regression gate

- C0036 YouTube + Editing unchanged;
- C0035 Rescue + Stream Ready unchanged;
- C0034 PC + Apply unchanged;
- C0032 Home + Creator Hub unchanged;
- C0033 safety acknowledgement runtime remains mandatory;
- application options 23;
- application links 86;
- prices/service IDs/Apply URLs preserved;
- non-target Desktop/Mobile pixel parity zero;
- any changed target horizontal overflow zero.

## Stop conditions

- no material inconsistency is found → `HOLD — 새 결론 없음`;
- change is decorative only;
- multi-accent identity returns;
- any C0033 safety behavior regression;
- accessibility, route or business-data regression.

## Promotion boundary

C0036 and any future C0037 build remain Review Candidates. Do not promote or deploy without `/upgrade-auto`.
