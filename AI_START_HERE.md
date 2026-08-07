# AI START HERE — DH 세팅센터 제작·운영 스튜디오

이 저장소를 처음 읽는 AI는 아래 순서를 지켜라.

1. [`ai/STATE.json`](ai/STATE.json)
2. [`AGENTS.md`](AGENTS.md)
3. [`ai/SOURCE_REGISTRY.json`](ai/SOURCE_REGISTRY.json)
4. [`ai/SOURCE_OF_TRUTH.md`](ai/SOURCE_OF_TRUTH.md)
5. [`continuation/PROJECT_SNAPSHOT_R24.md`](continuation/PROJECT_SNAPSHOT_R24.md)
6. [`continuation/A20_HANDOFF.md`](continuation/A20_HANDOFF.md)
7. [`audits/DH_C0028_FINAL_AUDIT_R24.json`](audits/DH_C0028_FINAL_AUDIT_R24.json)
8. [`ai/NEXT_ACTION.md`](ai/NEXT_ACTION.md)
9. 구현이 필요할 때 [`current-c0028/`](current-c0028/)를 읽는다.

## 절대 혼동 금지

- Active Control은 **R0003**이다.
- Active Preview는 **C0009A D2**다.
- **C0028은 Review Candidate이며 Active가 아니다.**
- C0027은 Direct Parent·Visual Rollback, C0022는 Functional Rollback이다.
- `/upgrade-auto` 없이는 승격하지 않는다.
- Production은 HOLD다.
- 실제 URL Browser Runtime은 UNVERIFIED다.
- 결제 기능은 구현되지 않았다.

## C0028 핵심 결론

- C0027 디자인을 8개 Desktop/Mobile 감사 화면에서 0 changed pixels로 유지.
- Runtime CSS 187,722 → 181,422 bytes.
- Visual Shell CSS 26,397 → 20,097 bytes.
- 긴 반복 Scope Prefix 164 → 0.
- `!important` 473개는 아직 남아 있음.
- 23 application options, 86 links, prices, service IDs, apply URLs 유지.
- JavaScript bytes는 C0027과 동일.
- 디자인 점수 80, 기능 점수 84 유지.

## Binary 주의

일부 ZIP·PNG·JPG는 SHA-256과 Audit만 등록돼 있고 원본 바이트 전체가 이 저장소에 미러되지 않았다. 정확한 파일을 읽지 못했다면 반드시 UNVERIFIED로 기록한다.

## 현재 다음 작업

C0029 후보는 Apply 모바일의 판단·스크롤 부담 감소다. C0028을 Parent로 잠그고 validation, focus recovery, input retention, accessibility, prices/products/service IDs/URLs를 보존해야 한다. Material Delta가 없으면 새 Candidate를 만들지 않는다.