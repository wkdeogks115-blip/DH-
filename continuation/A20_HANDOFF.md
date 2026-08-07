# DH R0003 Visual Shell Component Handoff A20

role: `HANDOFF_ADDENDUM_NOT_CONTROL`
supersedes: `A19`
source_action: `REPLACE_A19_WITH_A20`
keep_A19_and_A20_together: `false`
assumed_persistent_sources_after_replacement: `15`
actual_ui_source_count: `USER_CONFIRMATION_REQUIRED`

## Locked state

- Active Control: R0003
- Active Preview: C0009A D2
- Current Review Candidate: C0028 `READY_NOT_PROMOTED`
- C0028 SHA-256: `4bdbe123a6e5860979f8af580a06ffd2407c63e2739ef802111679f679315cb7`
- Direct parent / visual rollback: C0027 `0db244b8f483e030d330d66f43b4d2bd262ed06460abf919209e627b996cdd7d`
- Functional rollback: C0022 `5f9e8749b02ff210e7a1729224e58a315e4cf023e59fc356c3529209c7af9128`
- Production: HOLD

## C0028 material result

- C0027 appearance preserved exactly in 8 audited Desktop/Mobile views: 0 changed pixels.
- Total runtime CSS: 187,722 → 181,422 bytes (-6,300, -3.356%).
- Visual Shell CSS: 26,397 → 20,097 bytes (-6,300, -23.866%).
- Repeated long visual-shell scope prefix occurrences: 164 → 0.
- `!important` count remains 473; this remains CSS debt.
- 23 application options, 86 application links, prices, service IDs, apply URLs preserved.
- All JavaScript bytes unchanged from C0027.
- Static QA PASS. Self-contained Chromium visual parity PASS.
- Actual URL Runtime UNVERIFIED.

## Source persistence

Before promotion do not persist Candidate ZIP, R24 Answer Pack, Local V22 or visual ZIP as permanent Project Sources. Replace A19 with A20 only.

## Next controlled work

Use C0028 as immutable visual parent. Current first choice: reduce Apply mobile decision/scroll burden while preserving validation, accessibility and all business data.
