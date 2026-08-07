# AI START HERE — DH 세팅센터 제작·운영 스튜디오

이 저장소를 처음 읽는 AI는 아래 순서를 지켜라.

1. [`ai/STATE.json`](ai/STATE.json)
2. [`AGENTS.md`](AGENTS.md)
3. [`ai/SOURCE_REGISTRY.json`](ai/SOURCE_REGISTRY.json)
4. [`ai/SOURCE_OF_TRUTH.md`](ai/SOURCE_OF_TRUTH.md)
5. [`continuation/PROJECT_SNAPSHOT_R25.md`](continuation/PROJECT_SNAPSHOT_R25.md)
6. [`continuation/A21_HANDOFF.md`](continuation/A21_HANDOFF.md)
7. [`audits/DH_C0029_FINAL_AUDIT_R25.json`](audits/DH_C0029_FINAL_AUDIT_R25.json)
8. [`audits/DH_C0029_OBJECTIVE_MOBILE_UX_AUDIT_V1.md`](audits/DH_C0029_OBJECTIVE_MOBILE_UX_AUDIT_V1.md)
9. [`ai/NEXT_ACTION.md`](ai/NEXT_ACTION.md)
10. 구현이 필요할 때 [`current-c0029/`](current-c0029/)와 C0028 parent component source를 읽는다.

## 절대 혼동 금지

- Active Control은 **R0003**이다.
- Active Preview는 **C0009A D2**다.
- **C0029는 Review Candidate이며 Active가 아니다.**
- C0028은 Direct Parent·Visual Rollback, C0022는 Functional Rollback이다.
- `/upgrade-auto` 없이는 승격하지 않는다.
- Production은 HOLD다.
- 실제 외부 URL Browser Runtime은 UNVERIFIED다.
- 결제 기능은 구현되지 않았다.

## C0029 핵심 결론

- 390px 모바일 Apply 초기 높이 4,903 → 3,390 px (-30.859%).
- 요약 생성 후 높이 5,325 → 4,359 px (-18.141%).
- Desktop C0028/C0029 changed pixels 0.
- Actual `js/apply.js` self-contained Chromium interaction PASS: 1-time rejection, error-summary focus, input retention, valid summary generation.
- `js/apply.js` bytes and form-control signature are identical to C0028.
- 23 application options, 86 links, prices, service IDs, apply URLs 유지.
- Real device, assistive technology and user conversion tests remain NOT_EXECUTED.

## Binary 주의

일부 ZIP·PNG·JPG는 SHA-256과 Audit만 등록돼 있고 원본 바이트 전체가 이 저장소에 미러되지 않았다. 정확한 파일을 읽지 못했다면 반드시 UNVERIFIED로 기록한다.

## 현재 다음 작업

C0030에서 C0029를 Parent로 잠그고 승인된 Visual Shell을 `rescue/`와 `stream-ready/`에만 확장한다. Apply 모바일 변경을 건드리지 말고, Creator 페이지까지 같은 Candidate에서 확장하지 않는다. Material Delta가 없거나 기능·가격·Route 회귀가 있으면 HOLD한다.
