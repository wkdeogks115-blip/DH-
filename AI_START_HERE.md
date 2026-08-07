# AI START HERE — DH 세팅센터 제작·운영 스튜디오

이 저장소를 처음 읽는 AI는 아래 순서를 지켜라.

1. [`ai/STATE.json`](ai/STATE.json)
2. [`AGENTS.md`](AGENTS.md)
3. [`ai/SOURCE_REGISTRY.json`](ai/SOURCE_REGISTRY.json)
4. [`ai/SOURCE_OF_TRUTH.md`](ai/SOURCE_OF_TRUTH.md)
5. [`continuation/PROJECT_SNAPSHOT_R29.md`](continuation/PROJECT_SNAPSHOT_R29.md)
6. [`continuation/A25_HANDOFF.md`](continuation/A25_HANDOFF.md)
7. [`current-c0033/README.md`](current-c0033/README.md)
8. [`current-c0033/APPLY_VALUE_HELPER_PATCH.md`](current-c0033/APPLY_VALUE_HELPER_PATCH.md)
9. [`audits/DH_C0033_FINAL_AUDIT_R29.json`](audits/DH_C0033_FINAL_AUDIT_R29.json)
10. [`audits/DH_C0033_SAFETY_ACK_RUNTIME_AUDIT.json`](audits/DH_C0033_SAFETY_ACK_RUNTIME_AUDIT.json)
11. [`ai/NEXT_ACTION.md`](ai/NEXT_ACTION.md)

## 절대 혼동 금지

- Active Control은 **R0003**이다.
- Active Preview는 **C0009A D2**다.
- **C0033은 Review Candidate이며 Active가 아니다.**
- C0032는 Direct Parent이자 현재 디자인 방향 Rollback이다.
- C0031은 그 이전의 초절제 디자인 Rollback이다.
- C0022는 Functional Rollback이다.
- `/upgrade-auto` 없이는 승격하지 않는다.
- Production은 HOLD다.
- 실제 외부 URL Browser Runtime은 UNVERIFIED다.
- 결제 기능은 구현되지 않았다.

## C0033 핵심 결론

C0033은 디자인 Candidate가 아니다. C0032에서 실제 신청 동작을 검증하다 더 높은 우선순위의 버그가 발견되어 범위를 바꿨다.

C0032에서는 `safety_ack`와 `scope_ack`가 체크되지 않아도 단일 checkbox의 `.value="confirmed"`가 읽혀 신청 요약을 만들 수 있었다.

C0033에서는 checkbox/radio가 실제 checked일 때만 값을 반환한다.

실행 증거:
- Parent C0032: 두 안전 확인 unchecked → 신청 요약 생성됨 — DEFECT REPRODUCED
- Candidate C0033: 두 안전 확인 unchecked → 요약 차단 + `safety_ack`, `scope_ack` 오류
- 안전 확인 1개만 체크 → 나머지 1개 오류 유지
- 둘 다 체크 → 요약 생성
- 빈 Candidate 신청서 → 오류 6개. Kakao 전달 채널은 기본 선택 상태이므로 handoff 오류는 없음.
- 오류요약 Focus, 입력값 보존 → PASS
- 23 application options, 86 application links, 가격, service IDs, Apply URLs 유지
- Home/PC/Apply Desktop+Mobile 정적 화면 6/6 zero changed pixels

## 디자인 방향

C0032의 Brand Depth 방향은 폐기되지 않았다. C0033은 그 디자인 위에 안전 검증 버그만 고친 Candidate다. C0034에서 PC + Apply Brand Depth 확장을 다시 진행하되, C0033 안전 검증 동작을 필수 Gate로 잠근다.

## Binary 주의

일부 ZIP·PNG·JPG는 SHA-256과 Audit만 등록돼 있고 원본 바이트 전체가 이 저장소에 미러되지 않았다. 정확한 파일을 읽지 못했다면 반드시 UNVERIFIED로 기록한다.
