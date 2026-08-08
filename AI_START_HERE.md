# AI START HERE — DH 세팅센터 제작·운영 스튜디오

이 저장소를 처음 읽는 AI는 아래 순서를 지켜라.

1. [`ai/STATE.json`](ai/STATE.json)
2. [`AGENTS.md`](AGENTS.md)
3. [`ai/SOURCE_REGISTRY.json`](ai/SOURCE_REGISTRY.json)
4. [`ai/SOURCE_OF_TRUTH.md`](ai/SOURCE_OF_TRUTH.md)
5. [`continuation/PROJECT_SNAPSHOT_R34.md`](continuation/PROJECT_SNAPSHOT_R34.md)
6. [`continuation/A30_HANDOFF.md`](continuation/A30_HANDOFF.md)
7. [`current-c0038/README.md`](current-c0038/README.md)
8. [`current-c0038/DIAGNOSE_RESULT_FOCUS_CONTRACT.md`](current-c0038/DIAGNOSE_RESULT_FOCUS_CONTRACT.md)
9. [`ai/NEXT_ACTION.md`](ai/NEXT_ACTION.md)

## 절대 혼동 금지

- Active Control은 **R0003**이다.
- Active Preview는 **C0009A D2**다.
- **C0038은 Review Candidate이며 Active가 아니다.**
- C0037은 C0038의 Direct Parent이자 즉시 Rollback이다.
- C0034는 PC + Apply rollback이다.
- C0033은 안전 확인 검증 invariant의 원본이다.
- C0032는 Brand Depth 방향 원형이다.
- C0031은 초절제 디자인 Rollback이다.
- C0022는 Functional Rollback이다.
- `/upgrade-auto` 없이는 승격하지 않는다.
- Production은 HOLD다.
- 실제 외부 URL Browser Runtime은 UNVERIFIED다.
- 결제 기능은 구현되지 않았다.

## C0038 핵심 결론

C0037 이후 광범위한 디자인 확장은 중단했다. C0038은 사이트 전체 Production-Blocker 감사를 수행했고, `diagnose/`에서 실제 접근성 Material Delta 한 건을 재현했다.

Parent C0037에서는 유효한 진단 결과가 표시돼도 keyboard focus가 `추천 범위 확인` 제출 버튼에 남았고, 결과 영역에 named region/live semantics가 없었다.

C0038은 Diagnose 결과에만 다음을 추가했다.

- `role="region"`
- `aria-labelledby="diagnose-result-title"`
- `aria-live="polite"`
- `aria-atomic="true"`
- `tabindex="-1"`
- 유효 결과 생성 직후 `focus({preventScroll:true})`

실제 self-contained Chromium 결과:
- Parent valid result focus defect: REPRODUCED
- Candidate result focus: PASS
- Candidate result semantics: PASS
- 필수 항목 누락 시 native browser focus: PASS
- Diagnose resting visual parity: 2/2 zero changed pixels
- 다른 14페이지 Desktop/Mobile: 28/28 zero changed pixels
- C0033 안전 invariant: PASS
- application options 23 / application links 86
- 가격, service IDs, Apply URLs 유지
- Apply JS는 C0037과 byte-identical

## 디자인 방향

추가 광범위 디자인 마이그레이션은 하지 않는다. 앞으로는 실제 기능·신뢰·접근성·Route·Data 결함이 재현될 때만 별도 Candidate를 만든다.

## 다음 작업

C0039는 **통합 승격 준비 감사**다. Active Preview `C0009A D2`와 최신 통합 Review Candidate `C0038` 사이의 전체 Material Delta와 Production blocker를 검증한다. 새 결함이 없으면 새 디자인 Candidate를 만들지 않는다. `/upgrade-auto` 없이는 승격하지 않는다.

## Binary 주의

일부 ZIP·PNG·JPG는 SHA-256과 Audit만 저장소에 기록되고 원본 바이트 전체는 미러되지 않을 수 있다. 실제 파일을 읽지 못했다면 UNVERIFIED로 기록한다.
