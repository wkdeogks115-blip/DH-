# SOURCE OF TRUTH

## Current

| Role | Current value | Status |
|---|---|---|
| Active Control | R0003 | LOCKED |
| Parent Control | R0002 | lineage valid |
| Active Preview | C0009A D2 | unchanged |
| Current Review Candidate | C0026 | READY_NOT_PROMOTED |
| Direct parent / design rollback | C0025 | preserved |
| Functional rollback | C0022 | preserved |
| Runtime rollback | R0002 R1 | preserved |
| Latest Answer Pack | R22 | current review pack |
| Latest Handoff | A18 | current handoff |
| Production | HOLD | blocker remains |

## C0026 material result

- spacing, radius and typography semantic roles added
- application flow raw layout/type values migrated to semantic roles with equal computed values
- runtime CSS reduced 167,629 → 161,325 bytes
- reduction 6,304 bytes, 3.761%
- target raw layout/type literals reduced 98 → 37
- application products 23 and application links 86 preserved
- price, service ID and application URL drift 0
- static QA PASS
- self-contained Chromium desktop/mobile visual parity PASS
- four audited screenshot comparisons changed pixels 0
- actual URL runtime UNVERIFIED

## Current hashes

- C0026 Candidate: `8088b95c03d5663547a66eb79698d2da673863f96937aa0509fe32a1b643c44e`
- R22 Answer Pack: `dd9f0101f6a27159b4410e75856ff67d84da19eff8ed3a4f3700249de6210f5f`
- C0026 Local Pack: `b2a8340d38ff2ca015e8a2a02abb60b7d6194e6b76d8499249c6311c4ac1f62f`
- C0026 Visual Evidence: `594e83eba40ef1335d27d7e9d90e7aa4066f6720ad7428cfcd08b1dd41750c97`
- A18 Handoff: `fde6e9721b52267dca1941737778d9143c31c3e2d645d7a09eeaec49cce68d21`

## Promotion boundary

GitHub에 저장돼 있어도 C0026은 Active가 아니다. `/upgrade-auto` 전에는 Active Control·Active Preview·Production을 변경하지 않는다.

## Next

C0027 Button·Card·Form component contract consolidation with measurable additional legacy CSS reduction and C0026 visual parity.
