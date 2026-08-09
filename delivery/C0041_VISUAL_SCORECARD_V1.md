# DH C0041 VISUAL SCORECARD V1

> 내부 A/B 디자인 판단용 Heuristic이다. 고객 전환율 증거가 아니다.

## 결과
- Home: **94/100**
- PC: **92/100**
- Apply: **95/100**
- Direction 평균: **93.7/100**

## C0040 → C0041 Material Delta

### Home
- 둥근 흰색 Dashboard Card → 평평한 Service Ledger
- Hero 제목 Billboard Scale 축소
- 강한 Shadow 제거
- 실제 범위 데이터만 유지

### PC
- Home과 같은 흰색 Hero Card 문법 제거
- Desktop은 Hero 내부 Diagnostic Scale
- Mobile은 Dark slab을 끊는 Flat Paper Diagnostic Strip
- Home과 PC가 같은 Template Hero로 보이지 않게 분리

### Apply
- 상태 정보 Pill → 평문 Metadata
- 둥근 Floating Progress Card → Rule-based Journey Rail
- 실제 입력/요약 Surface만 Card 역할 유지

## First-fold Dark Coverage
- Home Desktop: 63.3% → **53.6%**
- Home Mobile: 75.6% → **69.2%**
- PC Desktop: 57.0% → **62.2%**
- PC Mobile: 69.8% → **63.9%**
- Apply Desktop: 46.0% → **44.6%**
- Apply Mobile: 42.7% → **42.1%**

PC Desktop Dark 비율 증가는 흰색 Dashboard Card를 제거하고 고유 Diagnostic Scale을 Hero에 통합한 의도적 Trade-off다. Mobile은 Flat Paper Strip으로 보정했다.

## 결론
`PASS_C0041_HUMAN_CRAFT_DIRECTION`

C0041은 C0040보다 잔여 AI/SaaS 템플릿 반복을 줄였고, 기능·상업 정보·접근성 회귀 없이 Control Plane 검수에 제출할 수 있다.
