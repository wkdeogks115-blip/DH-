# C0038 — Active Preview Baseline

Status: `ACTIVE_PREVIEW_NOT_DEPLOYED`

Control: R0004
Previous Active / current Rollback: C0009A D2
Active SHA-256: `b1c2628e02de28c3ccabc1247513bab4db93d2a6ee04427c1fd951025bde1114`
Active artifact: `DH_SITE_PREVIEW_ACTIVE_C0038_R0004.zip`

## Accepted material lineage

C0016→C0038 accepted lineage, 23 artifacts, final-audit hash match 23/23. The superseded C0033 PC/APPLY intermediate is excluded; the accepted branch is C0032 → C0033 Safety Ack Fix → C0034.

## C0038 final material delta

C0037 `diagnose/` generated a valid recommendation result but left keyboard focus on the submit button and lacked named/live result semantics. C0038 fixed only that completion-state accessibility transition.

## R36 explicit promotion evidence

- control R0001→R0002→R0003 lineage: PASS
- ZIP CRC / unsafe path / deterministic rebuild / manifest / inventory: PASS
- 15 runtime routes: PASS
- JS syntax: 9/9
- CSS structure: 19/19
- Desktop/Mobile Chromium: 30/30 PASS
- horizontal overflow: 0
- Apply safety/form runtime: PASS
- Diagnose focus/semantics runtime: PASS
- price value set vs C0009A D2: preserved
- application options: 23
- application links: 86
- service IDs: 23
- Preview noindex guard: PASS

Decision: `PASS_PROMOTE_C0038_TO_ACTIVE_PREVIEW_R0004_PRODUCTION_HOLD`.

## Boundary

This promotion is logical Control Plane state only. External Preview deployment/runtime remains UNVERIFIED and Production remains HOLD. The next meaningful step is manual Preview-only deployment followed by actual URL Runtime QA.