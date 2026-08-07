# DH 세팅센터 제작·운영 스튜디오

이 저장소는 DH 세팅센터의 사이트·상품·디자인·검증·릴리스 상태를 다음 AI 대화로 이어가기 위한 공개 Control Archive입니다.

## AI는 여기서 시작

1. [`AI_START_HERE.md`](AI_START_HERE.md)
2. [`ai/STATE.json`](ai/STATE.json)
3. [`ai/SOURCE_REGISTRY.json`](ai/SOURCE_REGISTRY.json)
4. [`ai/SOURCE_OF_TRUTH.md`](ai/SOURCE_OF_TRUTH.md)
5. [`continuation/PROJECT_SNAPSHOT_R24.md`](continuation/PROJECT_SNAPSHOT_R24.md)
6. [`continuation/A20_HANDOFF.md`](continuation/A20_HANDOFF.md)
7. [`ai/NEXT_ACTION.md`](ai/NEXT_ACTION.md)

## 새 AI 대화에서 보낼 문장

> `wkdeogks115-blip/DH-` 저장소를 열고 `AI_START_HERE.md`부터 순서대로 읽어. Active Control R0003과 Active Preview C0009A D2를 잠그고, C0028은 승격되지 않은 Review Candidate로 유지한 뒤 `ai/NEXT_ACTION.md`의 다음 작업을 계속 진행해. `/upgrade-auto` 없이는 승격·배포하지 마.

## 현재 잠금 상태

```text
Active Control: R0003
Active Preview Baseline: C0009A D2
Current Review Candidate: C0028
Direct Parent / Visual Rollback: C0027
Functional Rollback: C0022
Latest Answer Pack: R24
Latest Handoff: A20
Actual URL Browser Runtime: UNVERIFIED
Payment: NOT_IMPLEMENTED
Production: HOLD
```

## C0028 결과

- C0027 디자인과 8개 Desktop/Mobile 화면 픽셀 동일
- changed pixels: 0
- Runtime CSS: 187,722 → 181,422 bytes
- Visual Shell CSS: 26,397 → 20,097 bytes
- 긴 반복 Scope Prefix: 164 → 0
- `!important`: 473 유지 — 남은 CSS 부채
- 상품 23, 신청 링크 86, 가격·서비스 ID·신청 URL 유지
- JavaScript bytes C0027과 동일
- 디자인 휴리스틱 80, 기능 휴리스틱 84 유지

## 저장소 지도

- `control/`: Control Snapshot과 Update Bundle
- `continuation/`: 최신 Snapshot·Handoff
- `current-c0028/`: C0028 Candidate 핵심 Source
- `audits/`: C0028 구조·디자인·Final Audit
- `ai/`: 기계 판독 상태·Source Registry·다음 작업

기존 실제 홈페이지 Source 저장소는 [`wkdeogks115-blip/dh-setup-center-web`](https://github.com/wkdeogks115-blip/dh-setup-center-web)입니다.

## 공개 저장소 주의

비밀번호·인증번호·API Key·Token·결제정보·고객 개인정보는 커밋하지 않습니다. Binary 원본이 없는 경우 읽었다고 주장하지 않고 UNVERIFIED로 기록합니다.