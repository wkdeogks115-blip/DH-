# AI START HERE — DH 세팅센터 제작·운영 스튜디오

이 저장소를 처음 읽는 AI는 아래 순서를 지켜라.

1. [`ai/STATE.json`](ai/STATE.json)
2. [`AGENTS.md`](AGENTS.md)
3. [`ai/SOURCE_REGISTRY.json`](ai/SOURCE_REGISTRY.json)
4. [`ai/SOURCE_OF_TRUTH.md`](ai/SOURCE_OF_TRUTH.md)
5. [`continuation/PROJECT_SNAPSHOT_R30.md`](continuation/PROJECT_SNAPSHOT_R30.md)
6. [`continuation/A26_HANDOFF.md`](continuation/A26_HANDOFF.md)
7. [`current-c0034/README.md`](current-c0034/README.md)
8. [`current-c0034/BRAND_DEPTH_CONTRACT.md`](current-c0034/BRAND_DEPTH_CONTRACT.md)
9. [`ai/NEXT_ACTION.md`](ai/NEXT_ACTION.md)

## 절대 혼동 금지

- Active Control은 **R0003**이다.
- Active Preview는 **C0009A D2**다.
- **C0034는 Review Candidate이며 Active가 아니다.**
- C0033은 C0034의 Direct Parent이며 안전 확인 검증이 고쳐진 즉시 Rollback이다.
- C0032는 현재 Brand Depth 디자인 방향의 원형이다.
- C0031은 그 이전 초절제 디자인 Rollback이다.
- C0022는 Functional Rollback이다.
- `/upgrade-auto` 없이는 승격하지 않는다.
- Production은 HOLD다.
- 실제 외부 URL Browser Runtime은 UNVERIFIED다.
- 결제 기능은 구현되지 않았다.

## C0034 핵심 결론

C0034는 C0033의 안전 검증 수정본을 Parent로 유지한 채 `pc/`와 `apply/`에만 선택적 Navy/Cyan Brand Depth를 확장했다.

실행 증거:
- C0033 `apply.js` byte-identical 유지;
- 빈 신청서: 오류 6개 + 오류요약 Focus PASS;
- 안전 확인 2개 미체크: 정확히 `safety_ack`, `scope_ack` 오류 + 신청요약 차단;
- safety만 체크: `scope_ack` 오류 유지;
- 가능한 시간 1개: 2개 이상 규칙으로 차단;
- 차단된 제출의 기존 입력값 보존;
- 두 안전 확인 + 가능한 시간 2개: 신청요약 생성;
- 모바일 가로 Overflow 0.

디자인/레이아웃 결과:
- PC 모바일 높이 8,439px → 7,871px (-6.731%);
- Apply 모바일 높이 3,390px → 3,457px (+1.976%);
- Home/Creator/Rescue/Stream/YouTube/Editing Desktop+Mobile 12/12 zero changed pixels;
- application options 23, application links 86, 가격, service IDs, Apply URLs 유지.

## 디자인 방향

Brand Depth는 단순 장식 확장이 아니다. C0031의 정보 구조를 유지하면서 중요한 결정 지점에만 Navy/Cyan 깊이와 그룹 Surface를 사용한다. Glow-heavy 버튼, 다색 Gradient, 독립 Card 남발, billboard typography로 돌아가지 않는다.

## Binary 주의

일부 ZIP·PNG·JPG는 SHA-256과 Audit만 저장소에 기록되고 원본 바이트 전체는 미러되지 않을 수 있다. 실제 파일을 읽지 못했다면 UNVERIFIED로 기록한다.
