# SOURCE OF TRUTH

## Current

| Role | Current value | Status |
|---|---|---|
| Active Control | **R0004** | PROMOTED |
| Parent Control | R0003 | preserved |
| Active Preview | **C0038** | ACTIVE_PREVIEW_NOT_DEPLOYED |
| Active Preview SHA | `b1c2628e02de28c3ccabc1247513bab4db93d2a6ee04427c1fd951025bde1114` | locked |
| Active Rollback | C0009A D2 | ACTIVE_ROLLBACK_NOT_EXECUTED |
| Previous Rollback | R0002 Runtime R1 | ARCHIVE_CANDIDATE |
| Upgrade Audit | R36 | PASS |
| Latest Handoff | A32 | current |
| Promotion | EXECUTED_LOGICAL_PREVIEW_BASELINE | complete |
| External Preview Runtime | UNVERIFIED | not deployed |
| Production | HOLD | blockers remain |

## `/upgrade-auto` result

C0038 was revalidated against Active Control R0003 / Active Preview C0009A D2 and passed the explicit promotion gate.

Fresh R36 evidence:

- R0001→R0002→R0003 control lineage: PASS
- C0038 SHA/CRC: PASS
- unsafe ZIP paths: 0
- deterministic rebuild: PASS
- manifest / inventory: PASS
- runtime HTML routes: 15
- local refs/fragments/IDs/Alt/JSON-LD/ARIA/form labels: PASS
- JS syntax: 9/9
- CSS structure: 19/19
- 15 routes × Desktop/Mobile Chromium: PASS 30/30
- horizontal overflow: 0
- browser page errors: 0
- Apply safety/form runtime: PASS
- Diagnose focus/semantics runtime: PASS
- price value set vs previous Active D2: preserved
- application options: 23
- application links: 86
- service IDs: 23
- external executable dependencies: 0
- Preview noindex guard: PASS

Decision: `PASS_PROMOTE_C0038_TO_ACTIVE_PREVIEW_R0004_PRODUCTION_HOLD`.

## Rollback transition

- C0038 → `SITE_PREVIEW_BASELINE_ACTIVE`
- C0009A D2 → `SITE_ROLLBACK_ACTIVE`
- R0002 Runtime R1 → `ARCHIVE_CANDIDATE`

No external website deployment, website-source commit/push, Production release or deletion was executed by this promotion.

## Production HOLD

- deployed external Preview Runtime: UNVERIFIED
- final business identity/disclosure and final terms: HOLD
- Production noindex/robots flip: HOLD
- final Production domain: USER_CONFIRMATION_REQUIRED
- real physical device: NOT_EXECUTED
- real assistive technology/screen reader: NOT_EXECUTED
- external Review/Case evidence-link Runtime: UNVERIFIED
- payment execution/integration evidence: NOT_IMPLEMENTED_OR_NOT_EVIDENCED

The current Preview package intentionally retains noindex. Do not interpret R0004 as Production approval.

## Canonical hashes

- R0004 Source-ready bundle: `f77dfca2f99fb32d5c94fb5175ae5c2fe18d0dea964e65e960ad78188ad4f963`
- C0038 Active Preview: `b1c2628e02de28c3ccabc1247513bab4db93d2a6ee04427c1fd951025bde1114`
- C0009A D2 Rollback: `d799a0622159989afc7009d17d47d35a711ebcd3369ee760ec998b86c339b22e`
- R36 Upgrade Audit: `030aabab158c0b358e446df6f657bf522072a9d4e5359fcf7e2d26faa6e12b97`

## Next state-changing scope

Manually deploy C0038 to a **Preview environment only**, then run actual URL Runtime QA. Until a deployed Preview URL or other new material evidence exists, do not create another design Candidate.