# SOURCE OF TRUTH

## Current

| Role | Current value | Status |
|---|---|---|
| Active Control | **R0004** | PROMOTED |
| Parent Control | R0003 | preserved |
| Active Preview | **C0038** | ACTIVE_PREVIEW_NOT_DEPLOYED |
| Active Preview SHA | `b1c2628e02de28c3ccabc1247513bab4db93d2a6ee04427c1fd951025bde1114` | locked |
| Active Rollback | C0009A D2 | ACTIVE_ROLLBACK_NOT_EXECUTED |
| Current Review Candidate | **C0041** | READY_FOR_CONTROL_PLANE_REVIEW_NOT_PROMOTED |
| C0041 SHA | `cfc16576777f8da9b46d54ce174bd496e1c85bc56b9030c155713aa7e2ddfe23` | locked for review |
| Direct Parent | C0040 | superseded by C0041 for review |
| Latest Handoff | **A34** | Delivery → Control |
| Promotion | C0041 NOT_EXECUTED | explicit `/upgrade-auto` required |
| External Preview Runtime | UNVERIFIED | deployment deferred |
| Production | HOLD | blockers remain |

## Active R0004 truth

R0004 promoted C0038 as the logical Preview Baseline after R36 PASS. That remains unchanged.

- application options: 23
- application links: 86
- service IDs: 23
- Apply safety/form runtime: PASS
- Diagnose focus/semantics runtime: PASS
- Preview noindex guard: PASS

## C0041 Delivery Candidate

A fresh visual review after C0040 reproduced residual AI/SaaS-template grammar. C0041 changes only Home/PC/Apply visual treatment:

- Home: flat Service Ledger instead of rounded dashboard-style Hero object;
- PC: desktop integrated Diagnostic Scale and mobile flat paper diagnostic strip;
- Apply: plain metadata and rule-based journey rail instead of decorative pills / rounded progress card;
- calmer Hero typography.

Executed C0041 evidence:

- Candidate CRC: PASS
- deterministic rebuild: PASS
- static gate: PASS
- runtime routes: 15
- Apply safety/form runtime: PASS
- 320px Home/PC/Apply overflow: 0
- non-target 12 pages × Desktop/Mobile: PASS 24/24 zero changed pixels
- application options: 23
- application links: 86
- service IDs: 23
- price value set: preserved
- Apply URLs: preserved
- Apply JS: byte-identical to C0040
- Preview noindex guard: PASS

Visual heuristic: Home 94 / PC 92 / Apply 95 / direction 93.7. This is not conversion evidence.

Decision: `PASS_C0041_READY_FOR_CONTROL_PLANE_REVIEW_NOT_PROMOTED`.

## Preview / Production boundary

C0041 is **not Active** and has not been deployed. External Preview deployment remains deferred until Control Plane review and any later explicit promotion.

Production HOLD items remain:

- external deployed Preview Runtime: UNVERIFIED
- final business identity/disclosure and final terms: HOLD
- Production indexing flip: HOLD
- final Production domain: USER_CONFIRMATION_REQUIRED
- real physical device: NOT_EXECUTED
- real assistive technology/screen reader: NOT_EXECUTED
- external Review/Case evidence-link Runtime: UNVERIFIED
- payment execution/integration evidence: NOT_IMPLEMENTED_OR_NOT_EVIDENCED

## Canonical hashes

- R0004 Source-ready bundle: `f77dfca2f99fb32d5c94fb5175ae5c2fe18d0dea964e65e960ad78188ad4f963`
- C0038 Active Preview: `b1c2628e02de28c3ccabc1247513bab4db93d2a6ee04427c1fd951025bde1114`
- C0009A D2 Rollback: `d799a0622159989afc7009d17d47d35a711ebcd3369ee760ec998b86c339b22e`
- C0041 Candidate: `cfc16576777f8da9b46d54ce174bd496e1c85bc56b9030c155713aa7e2ddfe23`
- C0041 Delivery Audit: `e49d16dd169a729a36a8c72e072766568b9542364bdfae8df57ceb5990bfe23f`

## Next state-changing scope

Control Plane reviews C0041 against Active C0038 and parent C0040. No new design Candidate should be created without new material evidence. Promotion is prohibited until explicit `/upgrade-auto`.
