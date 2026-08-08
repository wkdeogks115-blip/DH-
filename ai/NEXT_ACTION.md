# NEXT ACTION — PREVIEW RUNTIME QA

## Current state

- Active Control: R0004
- Active Preview: C0038
- Active SHA: `b1c2628e02de28c3ccabc1247513bab4db93d2a6ee04427c1fd951025bde1114`
- Active Rollback: C0009A D2
- Upgrade Audit: R36 PASS
- Promotion: EXECUTED_LOGICAL_PREVIEW_BASELINE
- External Preview Runtime: UNVERIFIED
- Production: HOLD

## Next meaningful action

Deploy the C0038 Active Artifact to a **Preview environment only** using the user's normal hosting workflow, then provide the deployed Preview URL for actual Runtime QA.

Do not deploy to Production. Do not remove noindex/robots protections yet.

## Runtime QA scope after URL exists

- all public routes open successfully;
- local navigation and fragments;
- mobile/desktop layout;
- application flow and safety acknowledgements;
- Diagnose result focus/semantics;
- external contact/evidence links;
- analytics/consent behavior where applicable;
- noindex/robots headers remain correct for Preview.

## Stop condition

Without a deployed Preview URL or other new material evidence, do not create a new site Candidate. Keep Production HOLD.