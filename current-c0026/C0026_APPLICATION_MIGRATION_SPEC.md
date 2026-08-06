# C0026 Application Migration Spec

## Direct parent

- C0025 Candidate SHA-256: `60080d9f6898fc6b3d6a7c6bab15b4073bf99a0225facd0d85083f1c8a3cf922`
- Target file: `css/application-c0016.css`
- C0026 Candidate SHA-256: `8088b95c03d5663547a66eb79698d2da673863f96937aa0509fe32a1b643c44e`

## Migration rule

Raw application-flow values were replaced with semantic variables resolving to the same C0025 computed values. The resulting runtime CSS was deterministically compacted.

### Spacing roles

- `20px 22px` → `var(--dh-space-panel) var(--dh-space-panel-x)`
- `16px` → `var(--dh-space-layout)`
- `12px` → `var(--dh-space-stack)` where used as stack spacing
- `10px` → `var(--dh-space-compact)`
- `8px` → `var(--dh-space-inline)`
- `24px` → `var(--dh-space-card)`
- `18px` → `var(--dh-space-section)`
- `14px 15px` → `var(--dh-space-control-y) var(--dh-space-control-x)`
- `26px` → `var(--dh-space-summary)`

### Radius roles

- `20px` → `var(--dh-radius-shell)`
- `22px` → `var(--dh-radius-stage)`
- `12px` → `var(--dh-radius-card)`
- `13px` → `var(--dh-radius-input)`
- `14px` → `var(--dh-radius-option)`
- `16px` → `var(--dh-radius-panel)`

### Typography roles

- `.76rem` → `var(--dh-type-caption)`
- `.82rem` → `var(--dh-type-meta)`
- `.86rem` → `var(--dh-type-support)`
- `.88rem` → `var(--dh-type-copy-small)`
- `.9rem` → `var(--dh-type-copy)`
- `.98rem` → `var(--dh-type-control)`
- `1.25rem` → `var(--dh-type-section)`
- `1.35` → `var(--dh-leading-compact)`
- `1.58` → `var(--dh-leading-copy)`
- `1.65` → `var(--dh-leading-summary)`
- `-.025em` → `var(--dh-tracking-control)`
- `-.035em` → `var(--dh-tracking-heading)`
- `var(--font-sans)` → `var(--dh-font-sans)`

## HTML identity migration

All 15 public HTML pages:

- replace `dh-design-system-c0025.css` with `dh-design-system-c0026.css`
- replace body class `dh-design-system-c0025` with `dh-design-system-c0026`
- replace `data-build="c0025-semantic-color-token-foundation-review"` with `data-build="c0026-layout-type-token-migration-review"`

## Verification

Desktop and mobile Chromium computed styles and screenshots matched C0025 in all four audited views with zero changed pixels. Actual URL runtime remains UNVERIFIED.
