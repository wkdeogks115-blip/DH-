# AI START HERE — DH 세팅센터 제작·운영 스튜디오

이 저장소를 처음 읽는 AI는 아래 순서를 지켜라.

1. [`ai/STATE.json`](ai/STATE.json)
2. [`AGENTS.md`](AGENTS.md)
3. [`ai/SOURCE_REGISTRY.json`](ai/SOURCE_REGISTRY.json)
4. [`ai/SOURCE_OF_TRUTH.md`](ai/SOURCE_OF_TRUTH.md)
5. [`continuation/PROJECT_SNAPSHOT_R33.md`](continuation/PROJECT_SNAPSHOT_R33.md)
6. [`continuation/A29_HANDOFF.md`](continuation/A29_HANDOFF.md)
7. [`current-c0037/README.md`](current-c0037/README.md)
8. [`current-c0037/GAME_BRAND_CONSISTENCY_CONTRACT.md`](current-c0037/GAME_BRAND_CONSISTENCY_CONTRACT.md)
9. [`ai/NEXT_ACTION.md`](ai/NEXT_ACTION.md)

## 절대 혼동 금지

- Active Control은 **R0003**이다.
- Active Preview는 **C0009A D2**다.
- **C0037은 Review Candidate이며 Active가 아니다.**
- C0036은 C0037의 Direct Parent이자 즉시 Rollback이다.
- C0034는 PC + Apply Brand Depth rollback이다.
- C0033은 안전 확인 검증 invariant의 원본이다.
- C0032는 Brand Depth 방향 원형이다.
- C0031은 초절제 디자인 Rollback이다.
- C0022는 Functional Rollback이다.
- `/upgrade-auto` 없이는 승격하지 않는다.
- Production은 HOLD다.
- 실제 외부 URL Browser Runtime은 UNVERIFIED다.
- 결제 기능은 구현되지 않았다.

## C0037 핵심 결론

남은 7개 utility/trust surface를 먼저 감사했다.

- `game/`: **MIGRATE** — 한 페이지에 Orange / Mint / Cyan 3계열 Primary Action이 동시에 존재해 현재 단일 Cyan 브랜드 규칙과 충돌했다.
- `partners/`: KEEP
- `cases/`: KEEP
- `reviews/`: KEEP
- `policies/`: KEEP
- `diagnose/`: KEEP
- `404`: KEEP

따라서 C0037은 `game/` 한 페이지만 수정했다.

- Game primary action: Cyan family PASS
- Game mobile height: 6,444px → 6,384px (-0.931%)
- 다른 14페이지 Desktop/Mobile: 28/28 zero changed pixels
- application options 23, application links 86, 가격, service IDs, Apply URLs 유지
- Apply JS는 C0036과 byte-identical

## C0033 안전 invariant

실제 Candidate `apply.js`를 self-contained Chromium에서 재실행했다.

- 빈 신청서: 오류 6개 + 오류요약 Focus PASS
- 안전 확인 2개 미체크: `safety_ack`, `scope_ack` 오류 + 요약 차단
- safety만 체크: `scope_ack` 오류 유지
- 가능한 시간 1개: 차단
- 차단 후 입력값 유지
- 안전 확인 2개 + 가능한 시간 2개: 요약 생성
- 모바일 가로 Overflow 0

## 디자인 방향

광범위한 디자인 마이그레이션은 C0037에서 중단한다. 앞으로는 사이트 전체를 감사하고 실제 기능·신뢰·접근성·Route·Data 또는 눈에 띄는 시각 결함이 재현된 경우에만 Candidate를 만든다.

## 다음 작업

C0038은 **site-wide consistency + production-blocker audit**이다. 장식 목적 변경은 금지한다.

## Binary 주의

일부 ZIP·PNG·JPG는 SHA-256과 Audit만 저장소에 기록되고 원본 바이트 전체는 미러되지 않을 수 있다. 실제 파일을 읽지 못했다면 UNVERIFIED로 기록한다.
