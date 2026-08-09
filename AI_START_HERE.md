# AI START HERE — DH 세팅센터 제작·운영 스튜디오

처음 읽는 AI는 아래 순서를 따른다.

1. `ai/STATE.json`
2. `AGENTS.md`
3. `ai/SOURCE_REGISTRY.json`
4. `ai/SOURCE_OF_TRUTH.md`
5. `continuation/PROJECT_SNAPSHOT_R36.md`
6. `continuation/A34_HANDOFF.md`
7. `current-c0038/README.md`
8. `current-c0041/README.md`
9. `audits/DH_C0041_DELIVERY_AUDIT_V1.json`
10. `delivery/C0041_VISUAL_SCORECARD_V1.md`
11. `ai/NEXT_ACTION.md`

## 현재 잠금 상태

- Active Control: **R0004**
- Active Preview: **C0038**
- Active SHA: `b1c2628e02de28c3ccabc1247513bab4db93d2a6ee04427c1fd951025bde1114`
- Active Rollback: **C0009A D2**
- Current Review Candidate: **C0041**
- C0041 SHA: `cfc16576777f8da9b46d54ce174bd496e1c85bc56b9030c155713aa7e2ddfe23`
- C0041 status: **READY_FOR_CONTROL_PLANE_REVIEW_NOT_PROMOTED**
- External Preview deployment/runtime: **DEFERRED / UNVERIFIED**
- Production: **HOLD**

## 중요 구분

C0038은 현재 논리적 Active Preview Baseline이다.
C0041은 디자인 Delivery Candidate이며 아직 Active가 아니다.
C0040은 C0041의 직접 Parent이며 현재 검토 대상으로는 C0041이 우선한다.

## C0041 Material Delta

C0040에서 남아 있던 SaaS/AI-template 문법을 다시 실제 A/B로 검토해 다음을 수정했다.

- Home: rounded dashboard Hero → flat Service Ledger
- PC: 반복되는 white Hero Card → desktop Diagnostic Scale + mobile flat paper strip
- Apply: decorative pills / rounded progress card → plain metadata + rule-based journey rail
- Hero typography scale 완화

## C0041 Gate

- CRC / deterministic rebuild: PASS
- static: PASS
- Apply runtime: PASS
- 320px overflow: Home/PC/Apply 0
- non-target: 12 pages × Desktop/Mobile = 24/24 zero changed pixels
- application options 23 / application links 86 / service IDs 23
- prices / Apply URLs preserved
- Apply JS byte-identical to C0040
- Preview noindex guard PASS

Visual heuristic: Home 94 / PC 92 / Apply 95 / direction 93.7. 전환율 증거는 아니다.

## 다음 작업

`00_인프라·검증·릴리스`에서 C0041을 Control review한다. 새 Material defect가 없으면 새 디자인 Candidate를 만들지 않는다. 승격은 명시적 `/upgrade-auto` 전에는 실행하지 않는다.
