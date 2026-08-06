# DH PROJECT SNAPSHOT R21

업데이트: 2026-08-06 KST

이 문서는 ChatGPT 대화가 닫혀도 DH 세팅센터 제작·운영 작업을 이어가기 위한 압축 Source of Truth다. GitHub 저장은 보존·연속 작업 목적이며 Active 승격이나 Production 배포가 아니다.

## 1. Control 상태

```text
Control Plane: READY
Active Control: R0003
Parent Control: R0002
Active Preview Baseline: C0009A D2
Current Review Candidate: C0025
Design Rollback Parent: C0024
Functional Rollback Parent: C0022
Active Runtime Rollback: R0002 R1
Infrastructure: BASELINE_LOCKED
External Preview: DEFERRED_BY_USER
Browser URL Runtime: UNVERIFIED
Payment: NOT_IMPLEMENTED
Production: HOLD
Project Instructions: STABLE_VERSIONLESS
```

### 주요 Active 해시

- Active Control R0003 Source: `b6546f8bf2968f666713073dca5dd6253ee9363ed985ff5e5c54ecfd272c3704`
- Active Preview C0009A D2: `d799a0622159989afc7009d17d47d35a711ebcd3369ee760ec998b86c339b22e`
- Active Runtime Rollback R0002 R1: `f5f86f4e544b5e86186f7b7bcd5ab6f73f3bc0913776c506e717871a66aff6da`

## 2. 최신 Candidate C0025

- Candidate: `DH_SITE_CANDIDATE_C0025_SEMANTIC_COLOR_TOKEN_FOUNDATION_REVIEW.zip`
- SHA-256: `60080d9f6898fc6b3d6a7c6bab15b4073bf99a0225facd0d85083f1c8a3cf922`
- Direct Parent C0024 SHA-256: `f3aa5922cb42bd454deffc7b4076fa6e13c819a4ef9bb6606efbfded03b5267f`
- Role: `REVIEW_CANDIDATE_NOT_DEPLOY_PAYLOAD`
- Promotion: `NOT_EXECUTED`

### C0025 Material Delta

- C0024 Premium Restraint 디자인 방향 승인 유지
- Primitive → Semantic → Component → Legacy Alias 색상 Token 구조
- 하나의 Cyan Action Accent와 저채도 Neutral Surface
- Interactive Border 대비 `3.193:1`
- Focus·Text·Surface·Border·Action·Status 색상 중앙화
- 외부 Color Package·Font·UI Framework Runtime 의존성 0
- 가격·서비스 ID·핵심 범위·정책·결제 변경 0

### C0025 검증

```text
ZIP CRC: PASS
ZIP Entries: 106
Deterministic Rebuild: PASS
Inventory: PASS 104/104
Manifest: PASS 105/105
HTML: PASS 15/15
JavaScript: PASS 9/9
CSS: PASS 13/13
Application Options: 23
Application Links: 86
Missing References: 0
Broken Fragments: 0
Duplicate IDs: 0
Missing Alt: 0
JSON-LD Errors: 0
Price Drift: 0
Service ID Drift: 0
External Font Dependencies: 0
External Framework Dependencies: 0
Browser Static Visual: PASS_SELF_CONTAINED_CHROMIUM
Actual URL Navigation: UNVERIFIED_ENVIRONMENT_BLOCKED
Real Device / Assistive Technology / User Conversion: NOT_EXECUTED
```

### 최신 Artifact 해시

- R21 Answer Pack: `d08b6f1cf77b3a20d99d9d23660f12f385e1ea7aa61f06027cbe5fbaf8070735`
- Local HTML V18: `9d5d2279cb139059fec518c6a380b1a7461fc43146eac38c4da84c6fdcd49dea`
- Visual Evidence ZIP: `b41608f1cd042576e69032aeac53c23d11660aaf5c8710bf417b8dd9527e125d`
- A17 Handoff Source: stored as `continuation/A17_HANDOFF.md`

## 3. Candidate 계보 요약

- C0010 Preview Governance Hardening — SHA `f6c9a1a155b7ec27ec3a285f599558888d582e687377e26dc7fb6889315e11d6`
- C0011 Site Build Sequence Alignment — SHA `dfcb1db1fc9dccf952406d94a06ef34a08a2f327b8184b3f9035d11c8696c85f`
- C0012 Sales/Service Start UX — SHA `040a88f38d39232aa696f6f4f93214be89eb9b3810bc989b73b76ece3c7a72cd`
- C0013 Application Catalog — SHA `8b6eee7d58119b9d297244b92c5af8f597de6ac695070895a2fe455a769a8edc`
- C0014 Application Funnel — SHA `5bad3179612a12f307299ac45fa4b719e93410ba85d2f34fc5665aea26763a06`
- C0015 Application Completion — SHA `c7ead06df7d860bf3604f420a99a3f85305725cccbcc7af3cce3ff8201a717d3`
- C0016 Application Visual Hierarchy — SHA `9169303e606a6727429c5bfc8eafb1fba035ec30f4522e05c847b179cf3d3a3d`
- C0017 Content Density / Progressive Disclosure — archived as superseded review Candidate
- C0018 Consumer Decision First — archived as superseded review Candidate
- C0019 Cross-service Decision Parity — archived as superseded review Candidate
- C0020 Consumer Language / Self-contained — archived as superseded review Candidate
- C0021 Mobile Accessibility / Touch — archived as superseded review Candidate
- C0022 Form Error Recovery — SHA `5f9e8749b02ff210e7a1729224e58a315e4cf023e59fc356c3529209c7af9128`; functional rollback
- C0023 Premium Restraint — superseded after rendered cascade finding
- C0024 Premium Cascade Enforcement — SHA `f3aa5922cb42bd454deffc7b4076fa6e13c819a4ef9bb6606efbfded03b5267f`; approved visual parent
- C0025 Semantic Color Token Foundation — current review Candidate

## 4. 디자인·소비자 흐름 원칙

1. 소비자가 무엇을 파는지 즉시 이해할 것
2. 대상·가격·시간·핵심 범위를 쉽게 비교할 것
3. 한 화면의 Primary CTA는 하나의 자연스러운 신청 흐름으로 연결할 것
4. 기본 화면은 간결하고 스캔 가능하게 유지할 것
5. 핵심 가격·범위·CTA는 숨기지 않고 근거·예외·FAQ만 선택 공개할 것
6. 하나의 Accent, Neutral Surface, 의미 있는 상태 색상만 사용할 것
7. 카드·색상·배지·장식을 반복해 화면을 채우지 않을 것
8. 모바일 Touch Target, Focus, Safe Area, 줄바꿈을 보존할 것
9. 신청 오류는 오류 요약 → 해당 입력 Focus → 입력값 보존 → 재시도 흐름을 제공할 것
10. 실제 브라우저·기기·사용자 검증 전에는 과도한 확신을 표시하지 않을 것

## 5. 자동 승인 경계

가역적인 디자인 Candidate는 다음 조건에서 자동 승인 후 다음 작업으로 진행한다.

- Parent와 Rollback이 잠겨 있음
- 정적·범위별 시각 검증 PASS
- 가격·서비스 ID·핵심 범위·정책·결제·사업자 정보 변경 없음
- 회귀 0건
- Review Candidate 상태 유지
- 실행하지 않은 Runtime·사용자 테스트는 UNVERIFIED 유지

다음은 자동 승인하지 않는다.

- Active Control 승격
- Production 배포
- 가격·상품·환불·정책·결제 변경
- 사업자 정보 확정
- 삭제·commit·push
- Rollback 없는 대규모 변경

## 6. Source Budget

```text
assumed_persistent_source_count: 15
warning_at: 15
gc_due_at: 18
hard_hold_at: 20
actual_ui_source_count: USER_CONFIRMATION_REQUIRED
```

동일 역할 Handoff는 추가하지 않고 최신본으로 교체한다. A17이 A16을 대체한다.

## 7. 다음 작업

현재 1순위는 색상 다음 단계인 Spacing·Radius·Typography Semantic Token 통합과 Legacy CSS 중복 제거다.

완료 조건:

- CSS 부채가 측정 가능하게 감소
- C0025 Desktop·Mobile 계산 스타일 보존
- 가격·서비스·신청 기능 회귀 0
- 정적·시각 검증 PASS
- 새 Material Delta가 없으면 버전 생성 없이 `HOLD — 새 결론 없음`

승격은 명시적인 `/upgrade-auto`에서만 수행한다.

## 8. 새 ChatGPT 대화 시작 순서

1. 이 파일을 읽는다.
2. `continuation/CURRENT_STATE.md`를 읽는다.
3. `continuation/A17_HANDOFF.md`를 읽는다.
4. `continuation/DH_CONTINUATION_AUTOPILOT_PROMPT_v4.md`를 적용한다.
5. `audits/`와 `current-c0025/`를 확인한다.
6. 기존 공식 사이트 Source는 `wkdeogks115-blip/dh-setup-center-web` 저장소를 참고한다.
7. 이후 사용자는 `계속 진행`만 입력한다.
