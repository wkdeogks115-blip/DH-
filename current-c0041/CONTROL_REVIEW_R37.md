# C0041 Control Review R37

Decision: **READY_FOR_EXPLICIT_UPGRADE_AUTO**.

Active remains R0004 / C0038. C0041 is not promoted.

## Freshly executed Control gates
- Candidate SHA: `cfc16576777f8da9b46d54ce174bd496e1c85bc56b9030c155713aa7e2ddfe23`
- Direct parent C0040 SHA: `7bc9e35da20e8c06d802b9435527698d027529af6b3bb0446da6fd985237df11`
- CRC PASS / unsafe paths 0
- Manifest 166 entries, 0 bad hashes
- Inventory 165 entries, 0 mismatches
- 15 routes; static refs/fragments/IDs/Alt/JSON-LD/ARIA PASS
- JS syntax / CSS brace checks PASS
- Home/PC/Apply at 1440, 390, 320: 9/9 no overflow, no page errors
- Apply runtime: 6-error empty state, safety gates, focus, input preservation, 2-time availability and valid summary PASS
- 23 application options / 86 application links / 23 service IDs
- prices preserved vs Active C0038 and C0040
- Apply URLs preserved vs C0040
- Apply JS byte-identical to Active C0038 and C0040
- Diagnose HTML/JS byte-identical to Active C0038
- Preview noindex guard PASS

## Semantic delta C0040 → C0041
- add `css/human-craft-c0041.css`
- change `index.html`
- change `pc/index.html`
- change `apply/index.html`
- no semantic removal

No C0042 was created. External Preview remains not deployed and Production remains HOLD.

Next state-changing command: `/upgrade-auto`.
