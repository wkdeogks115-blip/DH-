# DH 세팅센터 제작·운영 스튜디오

이 저장소는 DH 세팅센터의 사이트·상품·디자인·검증·릴리스 상태를 다음 AI 대화로 이어가기 위한 공개 Control Archive입니다.

## AI는 여기서 시작

1. [`AI_START_HERE.md`](AI_START_HERE.md)
2. [`AGENTS.md`](AGENTS.md)
3. [`ai/STATE.json`](ai/STATE.json)
4. [`ai/SOURCE_OF_TRUTH.md`](ai/SOURCE_OF_TRUTH.md)
5. [`continuation/PROJECT_SNAPSHOT_R21.md`](continuation/PROJECT_SNAPSHOT_R21.md)
6. [`continuation/A17_HANDOFF.md`](continuation/A17_HANDOFF.md)
7. [`ai/NEXT_ACTION.md`](ai/NEXT_ACTION.md)

## 현재 잠금 상태

```text
Active Control: R0003
Active Preview Baseline: C0009A D2
Current Review Candidate: C0025
Design Rollback Parent: C0024
Functional Rollback Parent: C0022
Latest Answer Pack: R21
Latest Handoff: A17
Actual URL Browser Runtime: UNVERIFIED
Payment: NOT_IMPLEMENTED
Production: HOLD
```

C0025는 GitHub에 기록돼 있지만 Active로 승격되지 않았습니다. `/upgrade-auto` 없이는 Control·Active·Production을 변경하지 않습니다.

## 저장소 지도

- `control/`: Control Snapshot과 Update Bundle
- `continuation/`: 새 대화 복원용 Snapshot·Handoff·Prompt
- `current-c0025/`: 최신 Review Candidate의 핵심 Source·Audit
- `audits/`: C0025 정적·시각·색상 검증
- `ai/`: AI용 기계 판독 상태, Source 우선순위, 다음 작업, Artifact 목록
- `history/`: Candidate·Handoff 계보 요약

다음 작업은 [Issue #1](https://github.com/wkdeogks115-blip/DH-/issues/1)에 기록되어 있습니다.

기존 실제 홈페이지 Source 저장소는 [`wkdeogks115-blip/dh-setup-center-web`](https://github.com/wkdeogks115-blip/dh-setup-center-web)입니다.

## 공개 저장소 주의

사용자의 명시적 선택으로 Public입니다. 비밀번호·인증번호·API Key·Token·결제정보·고객 개인정보는 커밋하지 않습니다.
