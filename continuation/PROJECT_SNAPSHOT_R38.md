# DH PROJECT SNAPSHOT R38

## Active state
- Active Control: **R0005**
- Parent Control: R0004
- Active Control Bundle SHA-256: `c73bec95966f4f45fd5a9f2c777b5e2e7bfeca63c49299b047518d25338487f1`
- Active Preview: **C0041**
- Active Preview SHA-256: `cfc16576777f8da9b46d54ce174bd496e1c85bc56b9030c155713aa7e2ddfe23`
- Active Rollback: **C0038**
- C0038 SHA-256: `b1c2628e02de28c3ccabc1247513bab4db93d2a6ee04427c1fd951025bde1114`
- Archive Candidate: **C0009A D2**
- Previous R0002 Runtime R1: Archive Retained
- Latest Promotion Audit: **R38 PASS**
- Latest Handoff: **A36**

## R38 decision
`PASS_PROMOTE_C0041_TO_ACTIVE_PREVIEW_R0005_PRODUCTION_HOLD`

Fresh promotion gates passed: CRC/unsafe/deterministic/manifest/inventory/static, 15 routes × Desktop/Mobile 30/30, target 320px 3/3, non-target route HTML 12/12 byte-identical vs C0038, Apply runtime, Diagnose runtime, 23 options, 86 application links, 23 service IDs, price value set / Apply URLs preserved, Preview noindex guard.

Prior R37 visual evidence remains: non-target 12 pages × Desktop/Mobile = 24/24 zero changed pixels.

## External boundary
- Preview deployed URL: **NONE / NOT DEPLOYED**
- External URL Runtime: **UNVERIFIED**
- Production: **HOLD**
- Real device: NOT_EXECUTED
- Assistive technology: NOT_EXECUTED
- Payment Runtime: NOT_IMPLEMENTED_OR_NOT_EVIDENCED

## Next action
Deploy `DH_SITE_PREVIEW_ACTIVE_C0041_R0005.zip` to a Preview-only environment with noindex preserved, then run actual URL Runtime QA. Do not create C0042 without new material evidence.
