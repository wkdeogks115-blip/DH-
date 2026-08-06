# DH R0003 LAYOUT·TYPE TOKEN HANDOFF A18 — SOURCE READY

```yaml
role: HANDOFF_ADDENDUM_NOT_CONTROL
control_revision: R0003
parent_handoff: A17
source_action: REPLACE_A17_WITH_A18
active_control: R0003
active_preview_baseline: C0009A_D2
current_review_candidate: C0026
candidate_sha256: 8088b95c03d5663547a66eb79698d2da673863f96937aa0509fe32a1b643c44e
direct_parent: C0025
direct_parent_sha256: 60080d9f6898fc6b3d6a7c6bab15b4073bf99a0225facd0d85083f1c8a3cf922
production: HOLD
promotion: NOT_EXECUTED
actual_url_browser_runtime: UNVERIFIED
external_preview: DEFERRED_BY_USER
payment: NOT_IMPLEMENTED
assumed_source_count_after_replacement: 15
actual_ui_source_count: USER_CONFIRMATION_REQUIRED
```

## Material Delta

- spacing, radius and typography semantic roles added
- application-flow layout/type literals migrated to identical role values
- runtime CSS reduced from 167,629 bytes to 161,325 bytes
- CSS byte reduction: 6,304 bytes, 3.761%
- target raw layout/type literals reduced from 98 to 37
- raw literal reduction: 61
- C0025 vs C0026 Chromium desktop/mobile computed styles: identical
- screenshot changed pixels: 0 across four audited views

## Preserved

- 23 application options
- 86 application links
- prices, service IDs and application URLs
- C0025 neutral-surface and single-cyan-accent direction
- C0022 error summary, focus recovery and input preservation

## Verified

- ZIP CRC, safe paths and deterministic rebuild PASS
- Inventory 111/111 PASS
- Manifest 112/112 PASS
- HTML 15/15, JS 9/9 and CSS 13/13 PASS
- missing refs, broken fragments, duplicate IDs, missing Alt, JSON-LD and target-blank errors: 0
- external font and framework runtime dependencies: 0
- Chromium self-contained desktop/mobile static visual parity: PASS, zero-pixel difference

## Unverified

- actual URL navigation and complete JavaScript browser runtime
- real mobile device and assistive technology
- user conversion testing

## Next controlled work

C0027 should consolidate Button·Card·Form component contracts and remove superseded declarations from legacy layers only when measurable declaration reduction and C0026 visual parity can both be proven.

Do not promote C0026 without `/upgrade-auto`.
