# DH PROJECT SNAPSHOT R22

업데이트: 2026-08-07 KST

이 문서는 대화가 닫혀도 DH 세팅센터 제작·운영 작업을 이어가기 위한 현재 Source of Truth다. GitHub 저장은 Active 승격이나 Production 배포가 아니다.

## Control state

```text
Control Plane: READY
Active Control: R0003
Parent Control: R0002
Active Preview Baseline: C0009A D2
Current Review Candidate: C0026
Direct Parent / Design Rollback: C0025
Functional Rollback: C0022
Runtime Rollback: R0002 R1
Latest Answer Pack: R22
Latest Handoff: A18
Infrastructure: BASELINE_LOCKED
External Preview: DEFERRED_BY_USER
Browser URL Runtime: UNVERIFIED
Payment: NOT_IMPLEMENTED
Production: HOLD
Promotion: NOT_EXECUTED
```

## C0026 identity

- Candidate: `DH_SITE_CANDIDATE_C0026_LAYOUT_TYPE_TOKEN_MIGRATION_REVIEW.zip`
- SHA-256: `8088b95c03d5663547a66eb79698d2da673863f96937aa0509fe32a1b643c44e`
- Direct Parent C0025 SHA-256: `60080d9f6898fc6b3d6a7c6bab15b4073bf99a0225facd0d85083f1c8a3cf922`
- Role: `REVIEW_CANDIDATE_NOT_DEPLOY_PAYLOAD`

## Material result

- spacing, radius and typography semantic token roles added
- application-flow layout/type literals migrated to equivalent semantic values
- runtime CSS: 167,629 → 161,325 bytes
- reduction: 6,304 bytes, 3.761%
- target raw layout/type literals: 98 → 37
- raw literal reduction: 61
- Chromium desktop/mobile computed styles identical to C0025
- four audited screenshots changed pixels 0, RMS 0

## Preserved

- application options 23
- application links 86
- prices, service IDs and application URLs
- C0025 color and visual direction
- C0022 form error recovery

## Verification boundary

Static QA and self-contained Chromium CSS/layout rendering passed. Actual URL navigation, complete JavaScript runtime, real mobile device, assistive technology and user conversion tests remain UNVERIFIED or NOT_EXECUTED.

## Current GitHub sources

- `AI_START_HERE.md`
- `AGENTS.md`
- `ai/STATE.json`
- `ai/SOURCE_REGISTRY.json`
- `continuation/A18_HANDOFF.md`
- `current-c0026/`
- `audits/DH_C0026_*`

## Next controlled work

C0027: consolidate Button·Card·Form component contracts and remove superseded legacy declarations with measurable additional reduction while preserving C0026 computed style and screenshot parity.

Do not promote or deploy without `/upgrade-auto`.
