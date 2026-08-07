# DH 세팅센터 제작·운영 스튜디오

이 저장소는 DH 세팅센터의 사이트·상품·디자인·검증·릴리스 상태를 다음 AI 대화로 이어가기 위한 공개 Control Archive입니다.

## AI는 여기서 시작

1. [`AI_START_HERE.md`](AI_START_HERE.md)
2. [`AGENTS.md`](AGENTS.md)
3. [`ai/STATE.json`](ai/STATE.json)
4. [`ai/SOURCE_REGISTRY.json`](ai/SOURCE_REGISTRY.json)
5. [`ai/SOURCE_OF_TRUTH.md`](ai/SOURCE_OF_TRUTH.md)
6. [`continuation/PROJECT_SNAPSHOT_R25.md`](continuation/PROJECT_SNAPSHOT_R25.md)
7. [`continuation/A21_HANDOFF.md`](continuation/A21_HANDOFF.md)
8. [`ai/NEXT_ACTION.md`](ai/NEXT_ACTION.md)

## 새 AI 대화에서 보낼 문장

> `wkdeogks115-blip/DH-` 저장소를 열고 `AI_START_HERE.md`부터 순서대로 읽어. Active Control R0003과 Active Preview C0009A D2를 잠그고, C0029는 승격되지 않은 Review Candidate로 유지한 뒤 `ai/NEXT_ACTION.md`의 C0030 작업을 계속 진행해. `/upgrade-auto` 없이는 승격·배포하지 마.

## 현재 잠금 상태

```text
Active Control: R0003
Active Preview Baseline: C0009A D2
Current Review Candidate: C0029
Direct Parent / Visual Rollback: C0028
Functional Rollback: C0022
Latest Answer Pack: R25
Latest Handoff: A21
Actual external URL Runtime: UNVERIFIED
Payment: NOT_IMPLEMENTED
Production: HOLD
```

## C0029 결과

- 390px 모바일 Apply 초기 높이: 4,903 → 3,390 px (-30.859%)
- 요약 생성 후 높이: 5,325 → 4,359 px (-18.141%)
- Desktop C0028/C0029 changed pixels: 0
- Self-contained Chromium에서 실제 `js/apply.js` 상호작용 PASS
- one-time availability rejection / error-summary focus / input retention / valid summary generation PASS
- `js/apply.js` bytes와 Apply form-control signature C0028과 동일
- 상품 23, 신청 링크 86, 가격·서비스 ID·신청 URL 유지

## 다음 작업

C0030은 `rescue/`와 `stream-ready/` 두 서비스 결정 페이지에 승인된 Visual Shell을 확장합니다. C0029 Apply 모바일 UX는 보존하고 Creator 페이지는 같은 Candidate에 포함하지 않습니다.

## 저장소 지도

- `control/`: Control Snapshot과 Update Bundle
- `continuation/`: 최신 Snapshot·Handoff
- `current-c0028/`: C0028 parent component source
- `current-c0029/`: C0029 모바일 Apply delta와 현재 Candidate record
- `audits/`: C0029 UX·Final Audit
- `ai/`: 기계 판독 상태·Source Registry·다음 작업

기존 실제 홈페이지 Source 저장소는 [`wkdeogks115-blip/dh-setup-center-web`](https://github.com/wkdeogks115-blip/dh-setup-center-web)입니다.

## 공개 저장소 주의

비밀번호·인증번호·API Key·Token·결제정보·고객 개인정보는 커밋하지 않습니다. Binary 원본이 없는 경우 읽었다고 주장하지 않고 UNVERIFIED로 기록합니다.
