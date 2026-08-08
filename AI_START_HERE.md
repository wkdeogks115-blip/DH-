# AI START HERE — DH 세팅센터 제작·운영 스튜디오

이 저장소를 처음 읽는 AI는 아래 순서를 지켜라.

1. [`ai/STATE.json`](ai/STATE.json)
2. [`AGENTS.md`](AGENTS.md)
3. [`ai/SOURCE_REGISTRY.json`](ai/SOURCE_REGISTRY.json)
4. [`ai/SOURCE_OF_TRUTH.md`](ai/SOURCE_OF_TRUTH.md)
5. [`continuation/PROJECT_SNAPSHOT_R35.md`](continuation/PROJECT_SNAPSHOT_R35.md)
6. [`continuation/A31_HANDOFF.md`](continuation/A31_HANDOFF.md)
7. [`current-c0038/README.md`](current-c0038/README.md)
8. [`current-c0038/PROMOTION_READINESS_R35.md`](current-c0038/PROMOTION_READINESS_R35.md)
9. [`ai/NEXT_ACTION.md`](ai/NEXT_ACTION.md)

## 절대 혼동 금지

- Active Control은 **R0003**이다.
- Active Preview는 **C0009A D2**다.
- **C0038은 아직 Review Candidate이며 Active가 아니다.**
- C0039 사이트 Candidate는 만들지 않았다. C0039는 통합 승격 준비 Audit ID다.
- C0037은 C0038 Direct Parent/즉시 Rollback이다.
- C0033은 안전 확인 검증 invariant의 원본이다.
- `/upgrade-auto` 없이는 승격하지 않는다.
- Production은 HOLD다.
- 실제 외부 Preview URL Runtime은 UNVERIFIED다.

## R35 통합 결론

Active Preview `C0009A D2`부터 현재 `C0038`까지 승격 준비 감사를 새로 실행했다.

- accepted C0016→C0038 lineage artifacts: 23, CRC PASS
- superseded `C0033_PC_APPLY` intermediate: lineage에서 제외
- Active runtime routes 14 → Current 15
- 가격 value set: Active D2와 동일
- application options 23
- application links 86
- service IDs 23
- 15 routes × Desktop/Mobile Chromium: PASS 30/30
- horizontal overflow 0
- page errors 0
- static local refs/fragments/IDs/Alt/JSON-LD/ARIA/form labels PASS
- Apply safety/form Runtime PASS
- Diagnose result focus/semantics Runtime PASS
- external executable script/stylesheet dependencies 0
- Preview noindex guard PASS

판정: **`READY_FOR_EXPLICIT_UPGRADE_AUTO_PREVIEW_PROMOTION_PRODUCTION_HOLD`**.

즉 C0038은 명시적 `/upgrade-auto`에 제출할 준비가 됐지만, Production 승인은 아니다.

## Production HOLD 항목

- 실제 배포 Preview Runtime: UNVERIFIED
- 사업자 신원정보/최종 공개정보/최종 약관: HOLD
- Production noindex 해제: HOLD
- 최종 Production 도메인: USER_CONFIRMATION_REQUIRED
- 실제 물리 기기: NOT_EXECUTED
- 실제 보조기술/스크린리더: NOT_EXECUTED
- 외부 후기/사례 증거 링크 Runtime: UNVERIFIED
- 실제 결제 실행/통합 증거: NOT_IMPLEMENTED_OR_NOT_EVIDENCED

## 다음 작업

새 디자인 Candidate를 만들지 않는다. 상태를 바꾸려면 사용자가 **`/upgrade-auto`**를 명시해야 한다. 같은 C0038과 같은 증거로 `계속 진행`을 반복하면 `HOLD — 새 결론 없음`으로 종료한다.

## Binary 주의

일부 ZIP·PNG·JPG는 SHA-256과 Audit만 저장소에 기록되고 원본 바이트 전체는 미러되지 않을 수 있다. 실제 파일을 읽지 못했다면 UNVERIFIED로 기록한다.
