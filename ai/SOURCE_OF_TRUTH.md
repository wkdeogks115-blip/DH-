# SOURCE OF TRUTH

## Current

| Role | Current value | Status |
|---|---|---|
| Active Control | R0003 | LOCKED |
| Parent Control | R0002 | lineage valid |
| Active Preview | C0009A D2 | unchanged |
| Current Review Candidate | C0027 | READY_NOT_PROMOTED |
| Direct parent / design rollback | C0026 | preserved |
| Functional rollback | C0022 | preserved |
| Latest Answer Pack | R23 | current review pack |
| Latest Handoff | A19 | current handoff |
| Production | HOLD | blocker remains |

## C0027 material result

- C0026 function/data/accessibility preserved.
- Visual shell redesigned only for Home, PC pricing and Apply.
- Repeated nested Card/Border language reduced in the three prototype pages.
- Home hero changed to an editorial split with an unboxed service chooser.
- Home/PC pricing changed toward a pricing rail/decision-table presentation.
- Apply changed to a continuous form canvas with stage dividers and quieter sticky summary.
- Application options 23 preserved.
- Application links 86 preserved.
- Price, service ID and application URL drift 0.
- HTML/JS/CSS/reference/fragment/ID/Alt/JSON-LD static gates PASS.
- Self-contained Chromium desktop/mobile targeted layout PASS with no horizontal overflow and all key sections visible.
- Objective design heuristic 72 → 80 while functional prototype heuristic remains 84.
- The design score is not conversion evidence.
- Actual URL Runtime UNVERIFIED; real device, assistive technology and user conversion tests NOT_EXECUTED.
- Prototype cost: visual-shell override adds 26,397 CSS bytes. Consolidate only after direction approval.

## Current hashes

- C0027 Candidate: `0db244b8f483e030d330d66f43b4d2bd262ed06460abf919209e627b996cdd7d`
- R23 Answer Pack: `caf51941b3c60b58c641e72f340dfb0966ad2e2499500e359827dc3c624cfc15`
- C0027 Local Review V21: `c6cb05ef8280bc80d8e7d0ea6725bbd315ebd1a740ffbab4a7b1cac9935e0c39`
- C0027 Visual Evidence: `b183a4d0b0ffaac4042d5d125ef09f29ad11a8d7dfc0919c825f6a7237eb11a9`
- A19 Handoff: `e4943a13882e5b727963153c21f458ebee8372844173f4c3efe6b494f6e2c684`

## Promotion boundary

GitHub에 저장돼 있어도 C0027은 Active가 아니다. `/upgrade-auto` 전에는 Active Control·Active Preview·Production을 변경하지 않는다.

## Next

C0028 should consolidate the approved C0027 prototype shell into reusable Button/Pricing/Form/Section component contracts and reduce the temporary override cost before expanding the shell to more service pages.
