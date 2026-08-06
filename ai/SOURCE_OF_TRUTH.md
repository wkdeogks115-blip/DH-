# SOURCE OF TRUTH

## Current

| Role | Current value | Status |
|---|---|---|
| Active Control | R0003 | LOCKED |
| Parent Control | R0002 | lineage valid |
| Active Preview | C0009A D2 | unchanged |
| Current Review Candidate | C0025 | READY_NOT_PROMOTED |
| Design rollback | C0024 | preserved |
| Functional rollback | C0022 | preserved |
| Runtime rollback | R0002 R1 | preserved |
| Latest Answer Pack | R21 | current review pack |
| Latest Handoff | A17 | current handoff |
| Production | HOLD | blocker remains |

## C0025 material result

- Primitive → Semantic → Component Contract → Legacy Alias 색상 구조
- Primitive tokens 19
- Semantic tokens 22
- Legacy aliases 27
- Component raw color literals outside token block 0
- Application products 23 유지
- Application links 86 유지
- Price drift 0
- Service ID drift 0
- External font dependencies 0
- Static QA PASS
- Self-contained Chromium visual PASS
- Actual URL runtime UNVERIFIED

## Current hashes

- C0025 Candidate: `60080d9f6898fc6b3d6a7c6bab15b4073bf99a0225facd0d85083f1c8a3cf922`
- R21 Answer Pack: `d08b6f1cf77b3a20d99d9d23660f12f385e1ea7aa61f06027cbe5fbaf8070735`
- C0025 Local Pack: `9d5d2279cb139059fec518c6a380b1a7461fc43146eac38c4da84c6fdcd49dea`
- C0025 Visual Evidence: `b41608f1cd042576e69032aeac53c23d11660aaf5c8710bf417b8dd9527e125d`

## Promotion boundary

GitHub에 저장돼 있어도 C0025는 Active가 아니다. `/upgrade-auto`를 받은 뒤 Parent·Active cumulative delta, manifest, inventory, CRC, reproducible SHA, rollback, source replacement를 검증해야 한다.
