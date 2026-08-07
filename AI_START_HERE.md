# AI START HERE — DH 세팅센터 제작·운영 스튜디오

이 저장소를 처음 읽는 AI는 아래 순서를 지켜라.

1. [`ai/STATE.json`](ai/STATE.json)
2. [`AGENTS.md`](AGENTS.md)
3. [`ai/SOURCE_REGISTRY.json`](ai/SOURCE_REGISTRY.json)
4. [`ai/SOURCE_OF_TRUTH.md`](ai/SOURCE_OF_TRUTH.md)
5. [`continuation/PROJECT_SNAPSHOT_R23.md`](continuation/PROJECT_SNAPSHOT_R23.md)
6. [`continuation/A19_HANDOFF.md`](continuation/A19_HANDOFF.md)
7. [`ai/TEST_STATUS.md`](ai/TEST_STATUS.md)
8. [`audits/DH_C0027_OBJECTIVE_DESIGN_AUDIT_V2.md`](audits/DH_C0027_OBJECTIVE_DESIGN_AUDIT_V2.md)
9. [`ai/NEXT_ACTION.md`](ai/NEXT_ACTION.md)
10. 구현이 필요할 때 [`current-c0027/`](current-c0027/)와 [`audits/`](audits/)를 읽는다.

## 절대 혼동 금지

- Active Control은 **R0003**이다.
- Active Preview는 **C0009A D2**다.
- **C0027은 Review Candidate이며 Active가 아니다.**
- C0026은 Direct Parent·Design Rollback, C0022는 Functional Rollback이다.
- `/upgrade-auto` 없이는 승격하지 않는다.
- Production은 HOLD다.
- 외부 Preview는 사용자 요청으로 DEFERRED다.
- 실제 URL Browser Runtime은 UNVERIFIED다.
- 결제 기능은 구현되지 않았다.

## C0027 핵심 결론

- Home, PC pricing, Apply 3개 화면만 Visual Shell 재설계.
- 23 application options, 86 application links, prices, service IDs, apply URLs 유지.
- 정적 QA PASS.
- Self-contained Chromium targeted desktop/mobile layout PASS; horizontal overflow 0.
- 디자인 휴리스틱 72 → 80, 기능 휴리스틱 84 유지.
- 실제 사용자 전환 근거가 아니라 전문가 휴리스틱임.
- 임시 Visual Shell CSS +26,397 bytes. 더 넓게 확장하기 전에 C0028에서 통합해야 함.

## Binary 주의

일부 ZIP·PNG·JPG는 SHA-256과 Audit만 등록돼 있고 원본 바이트 전체가 이 저장소에 미러되지 않았다. 정확한 파일을 읽지 못했다면 반드시 UNVERIFIED로 기록한다.

## 현재 다음 작업

C0028에서 C0027의 승인된 Visual Shell을 재사용 가능한 Section/Button/Pricing/Form component contract로 통합하고 임시 Override 비용을 측정 가능하게 줄인다. C0027 시각 parity와 가격·신청 회귀 0을 동시에 입증하지 못하면 HOLD한다.
