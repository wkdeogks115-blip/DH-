# AI START HERE — DH 세팅센터 제작·운영 스튜디오

이 저장소를 처음 읽는 AI는 아래 순서를 지켜라.

1. [`ai/STATE.json`](ai/STATE.json)
2. [`AGENTS.md`](AGENTS.md)
3. [`ai/SOURCE_REGISTRY.json`](ai/SOURCE_REGISTRY.json)
4. [`ai/SOURCE_OF_TRUTH.md`](ai/SOURCE_OF_TRUTH.md)
5. [`continuation/PROJECT_SNAPSHOT_R22.md`](continuation/PROJECT_SNAPSHOT_R22.md)
6. [`continuation/A18_HANDOFF.md`](continuation/A18_HANDOFF.md)
7. [`ai/TEST_STATUS.md`](ai/TEST_STATUS.md)
8. [`ai/COMPLETENESS_REPORT_R22.md`](ai/COMPLETENESS_REPORT_R22.md)
9. [`ai/NEXT_ACTION.md`](ai/NEXT_ACTION.md)
10. 구현이 필요할 때 [`current-c0026/`](current-c0026/)와 [`audits/`](audits/)를 읽는다.

## 절대 혼동 금지

- Active Control은 **R0003**이다.
- Active Preview는 **C0009A D2**다.
- **C0026은 Review Candidate이며 Active가 아니다.**
- C0025는 Direct Parent·Design Rollback, C0022는 Functional Rollback이다.
- `/upgrade-auto` 없이는 승격하지 않는다.
- Production은 HOLD다.
- 외부 Preview는 사용자 요청으로 DEFERRED다.
- 실제 URL Browser Runtime은 UNVERIFIED다.
- 결제 기능은 구현되지 않았다.

## C0026 핵심 결론

- Runtime CSS: 167,629 → 161,325 bytes
- CSS 감소: 6,304 bytes, 3.761%
- Target raw spacing/radius/type literals: 98 → 37
- Desktop·Mobile Chromium 4개 감사 범위: computed style 동일, changed pixels 0
- 23 application options, 86 links, prices, service IDs, application URLs 유지

## Binary 주의

일부 ZIP·PNG·JPG는 SHA-256과 Audit만 등록돼 있고 원본 바이트 전체가 이 저장소에 미러되지 않았다. 정확한 파일을 읽지 못했다면 반드시 UNVERIFIED로 기록한다.

## 현재 다음 작업

C0027에서 Button·Card·Form component contract를 통합하고 superseded legacy declaration을 실제 수치로 제거한다. C0026 시각 parity와 가격·신청 회귀 0을 동시에 입증하지 못하면 HOLD한다.
