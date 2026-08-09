# NEXT ACTION — C0041 EXPLICIT UPGRADE AUTO

## Current state

- Active Control: **R0004**
- Active Preview: **C0038**
- Active SHA: `b1c2628e02de28c3ccabc1247513bab4db93d2a6ee04427c1fd951025bde1114`
- Active Rollback: **C0009A D2**
- Current Review Candidate: **C0041**
- C0041 SHA: `cfc16576777f8da9b46d54ce174bd496e1c85bc56b9030c155713aa7e2ddfe23`
- Direct parent: C0040
- Latest Control Review: **R37 PASS**
- Latest Handoff: **A35**
- C0041 status: **READY_FOR_EXPLICIT_UPGRADE_AUTO**
- External Preview: DEFERRED / NOT_DEPLOYED
- Production: HOLD

## Fresh Control result

R37 re-ran the minimum sufficient gates rather than relying only on Delivery evidence:

- CRC PASS / unsafe paths 0
- Manifest 166 entries / 0 bad hashes
- Inventory 165 entries / 0 mismatches
- 15 runtime routes
- static refs/fragments/IDs/Alt/JSON-LD/ARIA PASS
- JS syntax / CSS structural PASS
- Home/PC/Apply at 1440 + 390 + 320: **9/9 no overflow, no page errors**
- Apply safety/error/focus/value-preservation/availability/valid-summary runtime PASS
- 23 application options / 86 application links / 23 service IDs
- prices preserved vs Active C0038 and C0040
- Apply URLs preserved vs C0040
- Apply JS byte-identical to Active C0038 and C0040
- Diagnose HTML/JS byte-identical to Active C0038
- Preview noindex guard PASS

Semantic C0040 → C0041 delta is limited to `index.html`, `pc/index.html`, `apply/index.html` plus `css/human-craft-c0041.css`. No semantic removal.

## Next meaningful action

Explicit **`/upgrade-auto`** may now be run for C0041.

Do not create C0042 from the same evidence.
Do not deploy Preview or Production before promotion is separately completed.
Production blockers remain unchanged.
