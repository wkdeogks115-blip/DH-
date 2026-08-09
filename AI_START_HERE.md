# AI START HERE — DH 세팅센터 제작·운영 스튜디오

처음 읽는 AI는 아래 순서를 따른다.

1. `ai/STATE.json`
2. `AGENTS.md`
3. `ai/SOURCE_REGISTRY.json`
4. `ai/SOURCE_OF_TRUTH.md`
5. `continuation/A35_HANDOFF.md`
6. `current-c0038/README.md`
7. `current-c0041/README.md`
8. `current-c0041/CONTROL_REVIEW_R37.md`
9. `audits/DH_C0041_CONTROL_REVIEW_R37.json`
10. `ai/NEXT_ACTION.md`

## 현재 잠금 상태

- Active Control: **R0004**
- Active Preview: **C0038**
- Active SHA: `b1c2628e02de28c3ccabc1247513bab4db93d2a6ee04427c1fd951025bde1114`
- Active Rollback: **C0009A D2**
- Current Review Candidate: **C0041**
- C0041 SHA: `cfc16576777f8da9b46d54ce174bd496e1c85bc56b9030c155713aa7e2ddfe23`
- C0041 status: **READY_FOR_EXPLICIT_UPGRADE_AUTO**
- Latest Control Review: **R37 PASS**
- Latest Handoff: **A35**
- External Preview deployment/runtime: **DEFERRED / UNVERIFIED**
- Production: **HOLD**

## 중요 구분

C0038은 현재 논리적 Active Preview Baseline이다.
C0041은 R37 Control Review까지 통과했지만 아직 Active가 아니다.
C0040은 C0041의 직접 Parent이며 검토 우선순위는 C0041이다.

## R37 Control Review

Fresh Control gates:

- CRC PASS / unsafe paths 0
- Manifest 166 / Inventory 165 integrity PASS
- 15 runtime routes
- static refs/fragments/IDs/Alt/JSON-LD/ARIA PASS
- JS/CSS structural PASS
- Home/PC/Apply 1440 + 390 + 320 = 9/9 no overflow, no page errors
- Apply safety/error/focus/value-preservation/availability/valid-summary PASS
- application options 23 / application links 86 / service IDs 23
- prices preserved vs C0038 and C0040
- Apply URLs preserved
- Apply JS byte-identical to C0038 and C0040
- Diagnose HTML/JS byte-identical to C0038
- Preview noindex guard PASS

Semantic C0040 → C0041 change is limited to Home/PC/Apply plus `human-craft-c0041.css`. No new C0042 was created.

## 다음 작업

The next state-changing command is explicit **`/upgrade-auto`** for C0041.
Do not create another design Candidate from the same evidence. Do not deploy Preview or Production before the promotion decision.
