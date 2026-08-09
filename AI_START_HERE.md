# AI START HERE — DH 세팅센터 제작·운영 스튜디오

처음 읽는 AI는 아래 순서를 따른다.

1. `ai/STATE.json`
2. `AGENTS.md`
3. `ai/SOURCE_REGISTRY.json`
4. `ai/SOURCE_OF_TRUTH.md`
5. `continuation/PROJECT_SNAPSHOT_R38.md`
6. `continuation/A36_HANDOFF.md`
7. `current-c0041/README.md`
8. `audits/DH_C0041_UPGRADE_AUTO_AUDIT_R38.json`
9. `ai/NEXT_ACTION.md`

## 현재 잠금 상태

- Active Control: **R0005**
- Active Preview: **C0041**
- Active SHA: `cfc16576777f8da9b46d54ce174bd496e1c85bc56b9030c155713aa7e2ddfe23`
- Active Rollback: **C0038**
- C0038 SHA: `b1c2628e02de28c3ccabc1247513bab4db93d2a6ee04427c1fd951025bde1114`
- Latest Promotion Audit: **R38 PASS**
- Latest Handoff: **A36**
- External Preview: **NOT DEPLOYED / Runtime UNVERIFIED**
- Production: **HOLD**

## R38 `/upgrade-auto`

C0041 was promoted logically after fresh verification:

- CRC PASS / unsafe paths 0
- deterministic rebuild PASS
- Manifest 166 / Inventory 165 PASS
- 15 routes × Desktop/Mobile = 30/30 PASS
- Home/PC/Apply 320px = 3/3 PASS
- non-target 12 route HTML files byte-identical to C0038; prior R37 pixel parity remains 24/24 zero changed pixels
- Apply runtime PASS
- Diagnose runtime PASS
- 23 application options / 86 application links / 23 service IDs
- price value set / service IDs / Apply URLs preserved vs C0038
- Apply JS / Diagnose JS byte-identical to C0038
- Preview noindex guard PASS

## Role transition

- C0041 → Active Preview
- C0038 → Active Rollback
- C0009A D2 → Archive Candidate
- R0002 Runtime R1 → Archive Retained

## 다음 작업

C0041을 **Preview 환경에만** 배포하고 noindex를 유지한 뒤 실제 Preview URL로 external Runtime QA를 실행한다.
Production 배포는 하지 않는다.
