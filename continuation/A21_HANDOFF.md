# DH R0003 APPLY MOBILE COMPRESSION HANDOFF A21

Role: `HANDOFF_ADDENDUM_NOT_CONTROL`

Supersedes: A20  
Source action: `REPLACE_A20_WITH_A21`

## Locked state

- Active Control: R0003
- Active Preview: C0009A D2
- Current Review Candidate: C0029
- Direct Parent / Visual Rollback: C0028
- Functional Rollback: C0022
- Production: HOLD
- External Preview: DEFERRED_BY_USER
- Payment: NOT_IMPLEMENTED
- Promotion: NOT_EXECUTED

## C0029 material result

- Candidate SHA-256: `ba0de866143c9c68a3c5c0e9804390afeacbd43969c1dd8e135a804a59789930`
- Initial mobile Apply height: 4,903 → 3,390 px (-30.859%)
- Generated-summary height: 5,325 → 4,359 px (-18.141%)
- Desktop changed pixels: 0
- `js/apply.js`: byte-identical to C0028
- one-time availability rejection: PASS
- error-summary focus: PASS
- failed-submit input retention: PASS
- valid two-time summary generation: PASS
- 23 application options, 86 application links, prices, service IDs and apply URLs preserved

## Unverified

- Actual URL Runtime: UNVERIFIED
- Real device: NOT_EXECUTED
- Assistive technology: NOT_EXECUTED
- User conversion test: NOT_EXECUTED

## Next

C0030 should migrate the approved reusable visual shell to `rescue/` and `stream-ready/` only while preserving C0029 Apply behavior and all business invariants.

## Source budget

- Expected persistent Source count after replacing A20 with A21: 15
- Actual UI Source count: USER_CONFIRMATION_REQUIRED
- Status: WARNING
- Keep A20 + A21 together: false
