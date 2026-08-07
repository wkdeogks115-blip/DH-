# DH 세팅센터 제작·운영 스튜디오

이 저장소는 DH 세팅센터의 사이트·상품·디자인·검증·릴리스 상태를 다음 AI 대화로 이어가기 위한 공개 Control Archive입니다.

## AI는 여기서 시작

1. [`AI_START_HERE.md`](AI_START_HERE.md)
2. [`AGENTS.md`](AGENTS.md)
3. [`ai/STATE.json`](ai/STATE.json)
4. [`ai/SOURCE_REGISTRY.json`](ai/SOURCE_REGISTRY.json)
5. [`ai/SOURCE_OF_TRUTH.md`](ai/SOURCE_OF_TRUTH.md)
6. [`continuation/PROJECT_SNAPSHOT_R27.md`](continuation/PROJECT_SNAPSHOT_R27.md)
7. [`continuation/A23_HANDOFF.md`](continuation/A23_HANDOFF.md)
8. [`ai/NEXT_ACTION.md`](ai/NEXT_ACTION.md)

## 새 AI 대화에서 보낼 문장

> `wkdeogks115-blip/DH-` 저장소를 열고 `AI_START_HERE.md`부터 순서대로 읽어. Active Control R0003과 Active Preview C0009A D2를 잠그고, C0031은 승격되지 않은 Review Candidate로 유지한 뒤 `ai/NEXT_ACTION.md`의 C0032 감사를 계속 진행해. `/upgrade-auto` 없이는 승격·배포하지 마.

## 현재 잠금 상태

```text
Active Control: R0003
Active Preview Baseline: C0009A D2
Current Review Candidate: C0031
Direct Parent / Visual Rollback: C0030
Functional Rollback: C0022
Latest Answer Pack: R27
Latest Handoff: A23
Actual external URL Runtime: UNVERIFIED
Payment: NOT_IMPLEMENTED
Production: HOLD
```

## C0031 결과

- Creator Hub·YouTube·Editing Visual Shell 통합
- Creator-family 디자인 휴리스틱 68 → 80
- 전체 디자인 휴리스틱 80, 기능 휴리스틱 84 유지
- YouTube 모바일 길이 -6.982%, Editing -3.290%, Creator Hub -0.947%
- Home·PC·Apply·Rescue·Stream Ready Desktop/Mobile 10개 화면 changed pixels 0
- 상품 옵션 23, 신청 링크 86, 가격·서비스 ID·신청 URL 유지
- 중간 Creator Hub 모바일 16px overflow 시안은 폐기하고 최종본에서 overflow 0 확인

## 다음 작업

C0032는 `game/`, `partners/`, `cases/`, `reviews/`, `policies/`, `diagnose/`, 404의 **감사부터** 수행합니다. Material inconsistency가 없는 페이지는 억지로 재설계하지 않습니다.

## 저장소 지도

- `control/`: Control Snapshot과 Update Bundle
- `continuation/`: 최신 Snapshot·Handoff
- `current-c0028/`: shared shell parent source
- `current-c0029/`: Apply mobile delta
- `current-c0030/`: Rescue/Stream Ready service-shell delta
- `current-c0031/`: Creator shell delta
- `audits/`: 최신 C0031 audits
- `ai/`: 기계 판독 상태·Source Registry·다음 작업

기존 실제 홈페이지 Source 저장소는 [`wkdeogks115-blip/dh-setup-center-web`](https://github.com/wkdeogks115-blip/dh-setup-center-web)입니다.

## 공개 저장소 주의

비밀번호·인증번호·API Key·Token·결제정보·고객 개인정보는 커밋하지 않습니다. Binary 원본이 없는 경우 읽었다고 주장하지 않고 UNVERIFIED로 기록합니다.
