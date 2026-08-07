# AI START HERE — DH 세팅센터 제작·운영 스튜디오

이 저장소를 처음 읽는 AI는 아래 순서를 지켜라.

1. [`ai/STATE.json`](ai/STATE.json)
2. [`AGENTS.md`](AGENTS.md)
3. [`ai/SOURCE_REGISTRY.json`](ai/SOURCE_REGISTRY.json)
4. [`ai/SOURCE_OF_TRUTH.md`](ai/SOURCE_OF_TRUTH.md)
5. [`continuation/PROJECT_SNAPSHOT_R28.md`](continuation/PROJECT_SNAPSHOT_R28.md)
6. [`continuation/A24_HANDOFF.md`](continuation/A24_HANDOFF.md)
7. [`audits/DH_C0032_FINAL_AUDIT_R28.json`](audits/DH_C0032_FINAL_AUDIT_R28.json)
8. [`audits/DH_C0032_OBJECTIVE_DESIGN_DIRECTION_AUDIT_V1.md`](audits/DH_C0032_OBJECTIVE_DESIGN_DIRECTION_AUDIT_V1.md)
9. [`ai/NEXT_ACTION.md`](ai/NEXT_ACTION.md)
10. 구현이 필요할 때 `current-c0031/`과 `current-c0032/`를 비교한다.

## 절대 혼동 금지

- Active Control은 **R0003**이다.
- Active Preview는 **C0009A D2**다.
- **C0032는 Review Candidate이자 방향 Prototype이며 Active가 아니다.**
- C0031은 Direct Parent·Visual Rollback, C0022는 Functional Rollback이다.
- `/upgrade-auto` 없이는 승격하지 않는다.
- Production은 HOLD다.
- 실제 외부 URL Browser Runtime은 UNVERIFIED다.
- 결제 기능은 구현되지 않았다.

## C0032 핵심 결론

- C0031 이후 사용자 피드백에서 디자인이 이전보다 평면적이고 덜 좋아 보인다는 Material Delta가 발생했다.
- 따라서 남은 페이지의 무조건적 Visual Shell 확장은 중단했다.
- C0032는 Home + Creator Hub에서만 브랜드 깊이를 재조정한 A/B Prototype이다.
- C0031의 정보 구조·CTA 절제는 유지한다.
- 선택적 Navy/Cyan 깊이, 적정 Hero 크기, 중요한 의사결정 Surface에만 Elevation을 복원한다.
- C0031 방향 휴리스틱 80 → C0032 Prototype 88. 단, 사용자 전환 실험이 아닌 디자인 휴리스틱이다.
- PC/Apply/Rescue/Stream/YouTube/Editing Desktop+Mobile 12개 비교는 모두 0 changed pixels.
- 23 application options, 86 application links, prices, service IDs, apply URLs 유지.

## Binary 주의

일부 ZIP·PNG·JPG는 SHA-256과 Audit만 등록돼 있고 원본 바이트 전체가 이 저장소에 미러되지 않았다. 정확한 파일을 읽지 못했다면 반드시 UNVERIFIED로 기록한다.

## 현재 다음 작업

C0033에서는 C0032 방향을 모든 페이지에 자동 확장하지 않는다. Home + Creator A/B가 여전히 더 강하면 작은 페이지 묶음으로 확장하고, 그렇지 않으면 C0031을 보존한 채 다른 방향 Prototype을 만든다.
