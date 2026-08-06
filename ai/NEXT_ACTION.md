# NEXT ACTION — C0027

## Objective

C0026의 색상·Spacing·Radius·Typography Token과 zero-pixel visual parity를 보존하면서 Button·Card·Form component contract를 한 곳으로 통합하고, Legacy CSS에 남은 superseded declaration을 실제로 제거한다.

## Required evidence

1. C0026 SHA `8088b95c03d5663547a66eb79698d2da673863f96937aa0509fe32a1b643c44e`를 direct parent로 잠금
2. Button·Card·Form 중복 selector·declaration baseline 측정
3. Component contract와 migration boundary 작성
4. 별도 C0027 Review Candidate 생성
5. C0026 Desktop·Mobile computed style 및 screenshot parity 검사
6. HTML 15/15, JS, CSS, refs, fragments, IDs, Alt, JSON-LD 검사
7. Products 23, application links 86, prices, service IDs, apply URLs 보존
8. CSS byte 또는 duplicate declaration의 측정 가능한 추가 감소

## Stop conditions

- 중복 또는 CSS bytes가 측정 가능하게 감소하지 않음
- C0026 시각 방향 회귀
- 가격·서비스·신청 회귀
- 새 증거 없이 동일 검사 반복

이 경우 `HOLD — 새 결론 없음` 또는 Candidate 폐기.

## Promotion

C0027도 `/upgrade-auto` 전까지 Review Candidate다.
