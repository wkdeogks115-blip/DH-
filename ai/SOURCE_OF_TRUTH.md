# SOURCE OF TRUTH

## Current

| Role | Current value | Status |
|---|---|---|
| Active Control | **R0005** | PROMOTED |
| Parent Control | R0004 | preserved |
| Active Preview | **C0041** | ACTIVE_PREVIEW_NOT_DEPLOYED |
| Active Preview SHA | `cfc16576777f8da9b46d54ce174bd496e1c85bc56b9030c155713aa7e2ddfe23` | locked |
| Active Rollback | **C0038** | ACTIVE_ROLLBACK_NOT_EXECUTED |
| Archive Candidate | C0009A D2 | retained |
| Latest Promotion Audit | **R38** | PASS |
| Latest Handoff | **A36** | active handoff |
| External Preview Runtime | UNVERIFIED | not deployed |
| Production | HOLD | blockers remain |

## R0005 truth

R0005 promoted C0041 as the logical Preview Baseline after explicit `/upgrade-auto` and fresh R38 verification.

Fresh R38 evidence:
- Candidate CRC PASS / unsafe paths 0
- deterministic rebuild PASS
- Manifest 166 / Inventory 165 PASS
- 15 runtime routes
- Desktop/Mobile render: 30/30 PASS
- Home/PC/Apply 320px: 3/3 PASS
- non-target route HTML vs C0038: 12/12 byte-identical
- prior R37 non-target pixel evidence: 24/24 zero changed pixels
- Apply runtime: PASS
- Diagnose runtime: PASS
- application options: 23
- application links: 86
- service IDs: 23
- price value set / service IDs / Apply URLs: preserved vs C0038
- Apply JS / Diagnose JS: byte-identical to C0038
- Preview noindex guard: PASS

Semantic C0040 → C0041 delta remains limited to:
- added: `css/human-craft-c0041.css`
- changed: `index.html`, `pc/index.html`, `apply/index.html`
- removed: none

## Role transition

- C0041 → SITE_PREVIEW_BASELINE_ACTIVE
- C0038 → SITE_ROLLBACK_ACTIVE
- C0009A D2 → SITE_ARCHIVE_CANDIDATE
- R0002 Runtime R1 → ARCHIVE_RETAINED

## Preview / Production boundary

C0041 is **Active logically but not externally deployed**. External Preview URL Runtime remains UNVERIFIED.

Production HOLD items remain:
- external deployed Preview Runtime
- final business identity/disclosure and final terms
- Production indexing flip
- final Production domain confirmation
- real physical device validation
- assistive technology/screen reader validation
- external Review/Case evidence-link Runtime
- payment execution/integration evidence

## Canonical hashes

- R0005 Source-ready bundle: `c73bec95966f4f45fd5a9f2c777b5e2e7bfeca63c49299b047518d25338487f1`
- C0041 Active Preview: `cfc16576777f8da9b46d54ce174bd496e1c85bc56b9030c155713aa7e2ddfe23`
- C0038 Rollback: `b1c2628e02de28c3ccabc1247513bab4db93d2a6ee04427c1fd951025bde1114`
- C0009A D2 Archive Candidate: `d799a0622159989afc7009d17d47d35a711ebcd3369ee760ec998b86c339b22e`
- R38 Promotion Audit: `e8f76d1f1b814903c308250909f33a3581806edc50dfaaec6f71c36c25929103`

## Next state-changing scope

Deploy C0041 to a **Preview-only environment**, preserve noindex, and return the actual Preview URL for external Runtime QA. Do not create C0042 without new material evidence. Production deployment remains prohibited.
