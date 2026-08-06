# DH 세팅센터 제작·운영 스튜디오

이 저장소는 DH 세팅센터의 사이트·상품·디자인·검증·릴리스 상태를 다음 AI 대화로 이어가기 위한 공개 Control Archive입니다.

## AI는 여기서 시작

1. [`AI_START_HERE.md`](AI_START_HERE.md)
2. [`AGENTS.md`](AGENTS.md)
3. [`ai/STATE.json`](ai/STATE.json)
4. [`ai/SOURCE_REGISTRY.json`](ai/SOURCE_REGISTRY.json)
5. [`ai/SOURCE_OF_TRUTH.md`](ai/SOURCE_OF_TRUTH.md)
6. [`continuation/PROJECT_SNAPSHOT_R22.md`](continuation/PROJECT_SNAPSHOT_R22.md)
7. [`continuation/A18_HANDOFF.md`](continuation/A18_HANDOFF.md)
8. [`ai/NEXT_ACTION.md`](ai/NEXT_ACTION.md)

## 새 AI 대화에서 보낼 문장

> `wkdeogks115-blip/DH-` 저장소를 열고 `AI_START_HERE.md`부터 순서대로 읽어. Active Control R0003과 Active Preview C0009A D2를 잠그고, C0026은 승격되지 않은 Review Candidate로 유지한 뒤 `ai/NEXT_ACTION.md`의 C0027 작업을 계속 진행해. `/upgrade-auto` 없이는 승격·배포하지 마.

## 현재 잠금 상태

```text
Active Control: R0003
Active Preview Baseline: C0009A D2
Current Review Candidate: C0026
Direct Parent / Design Rollback: C0025
Functional Rollback Parent: C0022
Latest Answer Pack: R22
Latest Handoff: A18
Actual URL Browser Runtime: UNVERIFIED
Payment: NOT_IMPLEMENTED
Production: HOLD
```

C0026은 GitHub에 기록돼 있지만 Active로 승격되지 않았습니다.

## C0026 결과

- Runtime CSS 167,629 → 161,325 bytes
- 6,304 bytes, 3.761% 감소
- Target raw spacing/radius/type literals 98 → 37
- Chromium desktop/mobile four-view comparison: changed pixels 0
- Products 23, application links 86, prices, service IDs and apply URLs preserved

## 저장소 지도

- `control/`: Control Snapshot과 Update Bundle
- `continuation/`: Snapshot·Handoff·Autopilot
- `current-c0026/`: 최신 Review Candidate 핵심 CSS·migration spec·summary
- `audits/`: C0026 정적·CSS debt·Chromium·final audit
- `ai/`: 기계 판독 상태, Source Registry, next action, artifact catalog
- `history/`: Candidate·Handoff 계보

기존 실제 홈페이지 Source 저장소는 [`wkdeogks115-blip/dh-setup-center-web`](https://github.com/wkdeogks115-blip/dh-setup-center-web)입니다.

## 공개 저장소 주의

사용자의 명시적 선택으로 Public입니다. 비밀번호·인증번호·API Key·Token·결제정보·고객 개인정보는 커밋하지 않습니다. Binary 원본이 없는 경우 읽었다고 주장하지 않고 UNVERIFIED로 기록합니다.
