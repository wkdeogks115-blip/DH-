# AI START HERE — DH 세팅센터 제작·운영 스튜디오

이 저장소를 처음 읽는 AI는 아래 순서를 지켜라.

1. [`ai/STATE.json`](ai/STATE.json)
2. [`AGENTS.md`](AGENTS.md)
3. [`ai/SOURCE_REGISTRY.json`](ai/SOURCE_REGISTRY.json)
4. [`ai/SOURCE_OF_TRUTH.md`](ai/SOURCE_OF_TRUTH.md)
5. [`continuation/PROJECT_SNAPSHOT_R27.md`](continuation/PROJECT_SNAPSHOT_R27.md)
6. [`continuation/A23_HANDOFF.md`](continuation/A23_HANDOFF.md)
7. [`audits/DH_C0031_FINAL_AUDIT_R27.json`](audits/DH_C0031_FINAL_AUDIT_R27.json)
8. [`audits/DH_C0031_OBJECTIVE_CREATOR_SHELL_AUDIT_V1.md`](audits/DH_C0031_OBJECTIVE_CREATOR_SHELL_AUDIT_V1.md)
9. [`ai/NEXT_ACTION.md`](ai/NEXT_ACTION.md)
10. 구현이 필요할 때 `current-c0028/`, `current-c0029/`, `current-c0030/`, `current-c0031/`을 읽는다.

## 절대 혼동 금지

- Active Control은 **R0003**이다.
- Active Preview는 **C0009A D2**다.
- **C0031은 Review Candidate이며 Active가 아니다.**
- C0030은 Direct Parent·Visual Rollback, C0022는 Functional Rollback이다.
- `/upgrade-auto` 없이는 승격하지 않는다.
- Production은 HOLD다.
- 실제 외부 URL Browser Runtime은 UNVERIFIED다.
- 결제 기능은 구현되지 않았다.

## C0031 핵심 결론

- `creator/`, `creator/youtube/`, `creator/editing/`만 승인된 Visual Shell 언어로 이동.
- Creator-family 디자인 휴리스틱 68 → 80.
- 전체 사이트 디자인 휴리스틱 80 유지, 기능 휴리스틱 84 유지.
- Creator Hub 모바일 3,274 → 3,243px, YouTube 9,095 → 8,460px, Editing 8,814 → 8,524px.
- Home/PC/Apply/Rescue/Stream Ready Desktop+Mobile 10개 비교는 모두 0 changed pixels.
- 23 application options, 86 application links, prices, service IDs, apply URLs 유지.
- 첫 Creator Hub 모바일 시안의 16px horizontal overflow는 검증에서 발견되어 폐기됨.

## Binary 주의

일부 ZIP·PNG·JPG는 SHA-256과 Audit만 등록돼 있고 원본 바이트 전체가 이 저장소에 미러되지 않았다. 정확한 파일을 읽지 못했다면 반드시 UNVERIFIED로 기록한다.

## 현재 다음 작업

C0032는 무조건적인 디자인 확장이 아니라 남은 Surface 감사다. `game/`, `partners/`, `cases/`, `reviews/`, `policies/`, `diagnose/`, 404를 실제로 비교하고 Material visual/task inconsistency가 있을 때만 별도 Candidate를 만든다.
