# SOURCE OF TRUTH

## Current

| Role | Current value | Status |
|---|---|---|
| Active Control | R0003 | LOCKED |
| Active Preview | C0009A D2 | unchanged |
| Current Review Candidate | C0038 | READY_FOR_EXPLICIT_UPGRADE_AUTO |
| C0039 site Candidate | none | NOT_CREATED_NO_NEW_MATERIAL_DEFECT |
| Direct parent / immediate rollback | C0037 | preserved |
| Safety rollback / invariant source | C0033 | preserved |
| Brand-depth direction parent | C0032 | preserved |
| Functional rollback | C0022 | preserved |
| Latest Answer Pack | R35 | integrated promotion-readiness pack |
| Latest Handoff | A31 | promotion-readiness handoff |
| Promotion | NOT_EXECUTED | explicit `/upgrade-auto` required |
| Production | HOLD | blockers remain |

## R35 integrated conclusion

C0039 was executed as an **audit ID only**. No C0039 site-design Candidate was created because the integrated audit found no new material site defect after C0038.

Decision:

`READY_FOR_EXPLICIT_UPGRADE_AUTO_PREVIEW_PROMOTION_PRODUCTION_HOLD`

Current promotion target remains C0038:

- artifact SHA-256: `b1c2628e02de28c3ccabc1247513bab4db93d2a6ee04427c1fd951025bde1114`
- Active D2 SHA-256: `d799a0622159989afc7009d17d47d35a711ebcd3369ee760ec998b86c339b22e`

## Fresh integrated evidence

- accepted C0016→C0038 lineage artifacts: 23, CRC PASS
- superseded C0033 PC/APPLY intermediate: excluded
- Active runtime routes: 14
- Current runtime routes: 15
- price value set vs Active D2: equal
- application options: 23
- application links: 86
- service IDs: 23
- current C0038 ZIP CRC: PASS
- unsafe ZIP paths: 0
- local refs/fragments/duplicate IDs/Alt/JSON-LD/ARIA refs/form labels: PASS
- JS syntax: PASS
- CSS structural checks: PASS
- 15 routes × Desktop/Mobile Chromium: PASS 30/30
- horizontal overflow: 0
- render page errors: 0
- Apply safety/form Runtime: PASS
- Diagnose completion focus/semantics Runtime: PASS
- external executable script/stylesheet dependencies: 0
- Preview noindex guard: PASS

## Preview vs Production

C0038 is ready for an explicit **logical Preview Baseline promotion attempt** only.

Production remains HOLD because the following evidence/gates are unresolved:

- deployed external Preview Runtime: UNVERIFIED
- final business identity/disclosure and final terms: HOLD
- Production noindex/robots flip: HOLD
- final Production domain: USER_CONFIRMATION_REQUIRED
- real physical device: NOT_EXECUTED
- real assistive technology/screen reader: NOT_EXECUTED
- external Review/Case evidence-link Runtime: UNVERIFIED
- payment execution/integration evidence: NOT_IMPLEMENTED_OR_NOT_EVIDENCED

The current Policies page itself retains a `FINAL PUBLICATION GATE`; do not silently mark that PASS.

## Current hashes

- C0038 Candidate: `b1c2628e02de28c3ccabc1247513bab4db93d2a6ee04427c1fd951025bde1114`
- R35 Answer Pack: `981885174a1658661e37f51ceeb2281a658c75a273c1346cc48e7fcf120a68f2`
- R35 Audit Markdown: `49b8cda07247a74f6ce9195d235a906ed474151f5cf2e63b648910f40a43b402`
- R35 Final Audit JSON: `d1646310560ee792958071be12102fe83c1001694198057b46114045df12f36f`
- A31 Handoff: `10240f7483ea819aeb39a922a3b22b93eca3d20a69c211bcf5b0c318e46fae36`

## Promotion boundary

GitHub storage does not promote C0038. `/upgrade-auto` remains required before Active Control/Preview changes.

If the same C0038 artifact and the same evidence are reviewed again without new input, return `HOLD — 새 결론 없음` rather than creating another design Candidate.
