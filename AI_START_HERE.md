# AI START HERE — DH 세팅센터 제작·운영 스튜디오

이 저장소를 처음 읽는 AI는 아래 순서를 지켜라.

1. [`ai/STATE.json`](ai/STATE.json)
2. [`AGENTS.md`](AGENTS.md)
3. [`ai/SOURCE_REGISTRY.json`](ai/SOURCE_REGISTRY.json)
4. [`ai/SOURCE_OF_TRUTH.md`](ai/SOURCE_OF_TRUTH.md)
5. [`continuation/PROJECT_SNAPSHOT_R32.md`](continuation/PROJECT_SNAPSHOT_R32.md)
6. [`continuation/A28_HANDOFF.md`](continuation/A28_HANDOFF.md)
7. [`current-c0036/README.md`](current-c0036/README.md)
8. [`current-c0036/CREATOR_DETAIL_BRAND_DEPTH_CONTRACT.md`](current-c0036/CREATOR_DETAIL_BRAND_DEPTH_CONTRACT.md)
9. [`ai/NEXT_ACTION.md`](ai/NEXT_ACTION.md)

## 절대 혼동 금지

- Active Control은 **R0003**이다.
- Active Preview는 **C0009A D2**다.
- **C0036은 Review Candidate이며 Active가 아니다.**
- C0035는 C0036의 Direct Parent이자 즉시 Rollback이다.
- C0034는 PC + Apply Brand Depth rollback이다.
- C0033은 안전 확인 검증 invariant의 원본이다.
- C0032는 Brand Depth 방향 원형이다.
- C0031은 초절제 디자인 Rollback이다.
- C0022는 Functional Rollback이다.
- `/upgrade-auto` 없이는 승격하지 않는다.
- Production은 HOLD다.
- 실제 외부 URL Browser Runtime은 UNVERIFIED다.
- 결제 기능은 구현되지 않았다.

## C0036 핵심 결론

C0036은 `creator/youtube/`와 `creator/editing/` 두 Creator Detail 페이지만 선택적 Navy/Cyan Brand Depth로 확장했다.

- Creator-detail trust heuristic: 80 → 87
- Package decision clarity: 84 → 88
- Cross-page brand consistency: 82 → 90
- YouTube mobile: 8,460px → 8,444px (-0.189%)
- Editing mobile: 8,524px → 8,497px (-0.317%)
- 기존 purple Creator/Editing primary CTA는 Cyan 계열로 통일했다.
- Home/Creator Hub/PC/Apply/Rescue/Stream Desktop+Mobile: 12/12 zero changed pixels.
- application options 23, application links 86, 가격, service IDs, Apply URLs 유지.
- Apply JS는 C0035와 byte-identical.

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

Brand Depth는 장식 확장이 아니다. C0031 정보 구조를 유지하면서 Hero proof, package decision, pricing, route/result 같은 주요 결정 지점에만 깊이를 사용한다. Glow-heavy 버튼, 다색 Gradient, billboard typography, 독립 Card 남발로 돌아가지 않는다.

## 다음 작업

C0037은 `game/`, `partners/`, `cases/`, `reviews/`, `policies/`, `diagnose/`, `404`를 먼저 감사한다. Material inconsistency가 재현된 페이지에만 Candidate 변경을 허용한다.

## Binary 주의

일부 ZIP·PNG·JPG는 SHA-256과 Audit만 저장소에 기록되고 원본 바이트 전체는 미러되지 않을 수 있다. 실제 파일을 읽지 못했다면 UNVERIFIED로 기록한다.
