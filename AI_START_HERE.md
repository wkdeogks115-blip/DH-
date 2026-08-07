# AI START HERE — DH 세팅센터 제작·운영 스튜디오

이 저장소를 처음 읽는 AI는 아래 순서를 지켜라.

1. [`ai/STATE.json`](ai/STATE.json)
2. [`AGENTS.md`](AGENTS.md)
3. [`ai/SOURCE_REGISTRY.json`](ai/SOURCE_REGISTRY.json)
4. [`ai/SOURCE_OF_TRUTH.md`](ai/SOURCE_OF_TRUTH.md)
5. [`continuation/PROJECT_SNAPSHOT_R26.md`](continuation/PROJECT_SNAPSHOT_R26.md)
6. [`continuation/A22_HANDOFF.md`](continuation/A22_HANDOFF.md)
7. [`audits/DH_C0030_FINAL_AUDIT_R26.json`](audits/DH_C0030_FINAL_AUDIT_R26.json)
8. [`audits/DH_C0030_OBJECTIVE_SERVICE_SHELL_AUDIT_V1.md`](audits/DH_C0030_OBJECTIVE_SERVICE_SHELL_AUDIT_V1.md)
9. [`ai/NEXT_ACTION.md`](ai/NEXT_ACTION.md)
10. 구현이 필요할 때 `current-c0028/`, `current-c0029/`, `current-c0030/`을 읽는다.

## 절대 혼동 금지

- Active Control은 **R0003**이다.
- Active Preview는 **C0009A D2**다.
- **C0030은 Review Candidate이며 Active가 아니다.**
- C0029는 Direct Parent·Visual Rollback, C0022는 Functional Rollback이다.
- `/upgrade-auto` 없이는 승격하지 않는다.
- Production은 HOLD다.
- 실제 외부 URL Browser Runtime은 UNVERIFIED다.
- 결제 기능은 구현되지 않았다.

## C0030 핵심 결론

- `rescue/`, `stream-ready/`만 승인된 Visual Shell로 이동.
- Rescue 모바일 길이 -13.029%, Stream Ready -12.937%.
- 두 서비스 페이지 디자인 휴리스틱 70 → 80.
- 전체 사이트 디자인 휴리스틱은 80 유지, 기능 휴리스틱 84 유지.
- Home/PC/Apply Desktop+Mobile 6개 비교는 모두 0 changed pixels.
- 23 application options, 86 application links, prices, service IDs, apply URLs 유지.
- 중간 빌드에서 공통 모바일 container 회귀가 발견되어 폐기됐고, 최종 C0030은 Rescue/Stream Ready에만 Scope됨.

## Binary 주의

일부 ZIP·PNG·JPG는 SHA-256과 Audit만 등록돼 있고 원본 바이트 전체가 이 저장소에 미러되지 않았다. 정확한 파일을 읽지 못했다면 반드시 UNVERIFIED로 기록한다.

## 현재 다음 작업

C0031에서 C0030을 Parent로 잠그고 `creator/`, `creator/youtube/`, `creator/editing/` 세 Creator 페이지에만 동일한 Visual Shell을 확장한다. C0030 Rescue/Stream Ready와 C0029 Apply를 보존하고 policies/cases/reviews까지 같은 Candidate에서 확장하지 않는다.
