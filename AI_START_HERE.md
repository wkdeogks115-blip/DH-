# AI START HERE — DH 세팅센터 제작·운영 스튜디오

이 저장소를 처음 읽는 AI는 아래 순서를 지켜라.

1. [`ai/STATE.json`](ai/STATE.json)
2. [`AGENTS.md`](AGENTS.md)
3. [`ai/SOURCE_REGISTRY.json`](ai/SOURCE_REGISTRY.json)
4. [`ai/SOURCE_OF_TRUTH.md`](ai/SOURCE_OF_TRUTH.md)
5. [`continuation/PROJECT_SNAPSHOT_R21.md`](continuation/PROJECT_SNAPSHOT_R21.md)
6. [`continuation/A17_HANDOFF.md`](continuation/A17_HANDOFF.md)
7. [`ai/TEST_STATUS.md`](ai/TEST_STATUS.md)
8. [`ai/COMPLETENESS_REPORT_R21.md`](ai/COMPLETENESS_REPORT_R21.md)
9. [`ai/NEXT_ACTION.md`](ai/NEXT_ACTION.md)
10. 구현이 필요할 때 [`current-c0025/`](current-c0025/)와 [`audits/`](audits/)를 읽는다.

## 절대 혼동 금지

- Active Control은 **R0003**이다.
- Active Preview는 **C0009A D2**다.
- **C0025는 Review Candidate이며 Active가 아니다.**
- C0024는 Design Rollback Parent, C0022는 Functional Rollback Parent다.
- `/upgrade-auto` 없이는 승격하지 않는다.
- Production은 HOLD다.
- 외부 Preview는 사용자 요청으로 DEFERRED다.
- 실제 URL Browser Runtime은 UNVERIFIED다.
- 결제 기능은 구현되지 않았다.

## 이 저장소의 역할

대화가 닫혀도 프로젝트를 복원하고 이어가기 위한 AI-readable Control Archive다. GitHub 저장은 승격·배포와 동일하지 않다.

## Binary 주의

일부 ZIP·PNG·JPG는 SHA-256과 Audit만 등록돼 있고 원본 바이트 전체가 이 저장소에 미러되지 않았다. 정확한 파일을 읽지 못했다면 반드시 UNVERIFIED로 기록한다. 자세한 범위는 `ai/COMPLETENESS_REPORT_R21.md`와 `ai/ARTIFACT_CATALOG.md`를 따른다.

## 현재 다음 작업

C0025의 색상 Token 방향을 보존하면서 Spacing·Radius·Typography를 Semantic Token으로 통합하고 Legacy CSS 중복을 측정 가능하게 줄이는 C0026 Candidate를 별도로 만든다. 회귀가 있거나 부채 감소가 없으면 HOLD한다.
