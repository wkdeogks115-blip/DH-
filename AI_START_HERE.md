# AI START HERE — DH 세팅센터 제작·운영 스튜디오

처음 읽는 AI는 아래 순서를 따른다.

1. `ai/STATE.json`
2. `AGENTS.md`
3. `ai/SOURCE_REGISTRY.json`
4. `ai/SOURCE_OF_TRUTH.md`
5. `continuation/PROJECT_SNAPSHOT_R36.md`
6. `continuation/A33_HANDOFF.md`
7. `current-c0038/README.md`
8. `audits/DH_C0038_UPGRADE_AUTO_AUDIT_R36.json`
9. `delivery/C0040_VISUAL_REBASE_DELIVERY_BRIEF_V1.md`
10. `ai/NEXT_ACTION.md`

## 현재 잠금 상태

- Active Control: **R0004**
- Active Preview: **C0038**
- Active SHA: `b1c2628e02de28c3ccabc1247513bab4db93d2a6ee04427c1fd951025bde1114`
- Active Rollback: **C0009A D2**
- Promotion: **EXECUTED_LOGICAL_PREVIEW_BASELINE**
- External Preview deployment/runtime: **DEFERRED / UNVERIFIED**
- Production: **HOLD**

## R36 promotion result

Explicit `/upgrade-auto` was executed. Fresh gates passed: control lineage, Candidate CRC/unsafe path, deterministic rebuild, manifest/inventory, 15-route static validation, JS/CSS checks, 30/30 Desktop/Mobile Chromium, Apply safety/form runtime, Diagnose focus/semantics runtime, preserved price value set, 23 application options, 86 application links, 23 service IDs, and Preview noindex guard.

C0038 remains the logical Active Preview Baseline. It is functionally valid and remains the rollback-safe source for the next design prototype.

## New visual-direction evidence

A fresh 15-route Desktop/Mobile visual review plus comparison against older Home visuals found a material visual-direction issue: the current shell is too uniformly dark, repetitive, and SaaS/AI-template-like. This does not invalidate C0038 functionality; it changes the next delivery priority.

Decision: **DEFER_PREVIEW_DEPLOYMENT_PENDING_VISUAL_REBASE_PROTOTYPE**.

Planned C0040 is a Delivery Plane prototype on exactly Home + PC + Apply. Use `delivery/C0040_VISUAL_REBASE_DELIVERY_BRIEF_V1.md`. Do not create or promote it from Control Plane.

## Rollback

- Immediate active rollback: C0009A D2
- Previous R0002 rollback: Archive Candidate only

## Production blockers

External Preview Runtime, final business identity/terms, Production indexing flip, Production domain confirmation, real device, assistive technology, external evidence-link Runtime, payment execution/integration evidence.

## Next work

Delivery Plane builds C0040 Home + PC + Apply visual rebase prototype from C0038, preserving all functional/business/accessibility invariants. External Preview deployment remains deferred until the A/B direction review passes.
