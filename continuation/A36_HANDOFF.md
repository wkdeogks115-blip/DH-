# DH R0005 C0041 ACTIVE HANDOFF A36
Role: `HANDOFF_ADDENDUM_NOT_CONTROL`
Supersedes: `A35`
Source action: `REPLACE_A35_WITH_A36`

## Active state
- Active Control: R0005
- Active Preview: C0041
- Active artifact: `DH_SITE_PREVIEW_ACTIVE_C0041_R0005.zip`
- Active SHA-256: `cfc16576777f8da9b46d54ce174bd496e1c85bc56b9030c155713aa7e2ddfe23`
- Active Rollback: C0038
- Rollback SHA-256: `b1c2628e02de28c3ccabc1247513bab4db93d2a6ee04427c1fd951025bde1114`
- Archive Candidate: C0009A D2
- Production: HOLD
- External Preview Runtime: UNVERIFIED

## Promotion evidence
- R38 decision: `PASS_PROMOTE_C0041_TO_ACTIVE_PREVIEW_R0005_PRODUCTION_HOLD`
- R38 audit SHA-256: `e8f76d1f1b814903c308250909f33a3581806edc50dfaaec6f71c36c25929103`
- CRC / deterministic rebuild / manifest / inventory: PASS
- 15 routes × Desktop/Mobile: PASS 30/30
- 320px Home/PC/Apply: PASS
- non-target route HTML vs C0038: PASS 12/12 byte-identical; R37 pixel evidence 24/24 remains valid
- Apply runtime: PASS
- Diagnose runtime: PASS
- 23 options / 86 application links / 23 service IDs
- prices / service IDs / Apply URLs preserved
- Preview noindex guard: PASS

## Next controlled work
Deploy **C0041 only to a Preview environment**, preserve noindex, then provide the actual Preview URL for external Runtime QA.
Do not deploy Production.

## Source budget
Expected persistent Source count after exact replacements: 15.
Actual UI Source count: USER_CONFIRMATION_REQUIRED.
Status: WARNING.
