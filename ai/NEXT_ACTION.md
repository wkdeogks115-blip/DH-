# NEXT ACTION — C0041 PREVIEW DEPLOYMENT + ACTUAL URL QA

## Current state

- Active Control: **R0005**
- Active Preview: **C0041**
- Active SHA: `cfc16576777f8da9b46d54ce174bd496e1c85bc56b9030c155713aa7e2ddfe23`
- Active Rollback: **C0038**
- Latest Promotion Audit: **R38 PASS**
- Latest Handoff: **A36**
- External Preview: **NOT DEPLOYED**
- Production: **HOLD**

## Promotion result

C0041 is now the logical Preview Baseline. R38 re-ran the promotion-critical gates and passed.

## Next meaningful action

Deploy `DH_SITE_PREVIEW_ACTIVE_C0041_R0005.zip` to a **Preview-only environment**.

Requirements:
- preserve all `noindex` controls;
- do not deploy Production;
- return the actual accessible Preview URL;
- then run external Runtime QA for routes/assets/mobile/Apply/Diagnose/noindex/external evidence links.

Do not create C0042 unless actual Preview Runtime or new evidence reproduces a material defect.
