# SOURCE OF TRUTH

## Current

| Role | Current value | Status |
|---|---|---|
| Active Control | R0003 | LOCKED |
| Active Preview | C0009A D2 | unchanged |
| Current Review Candidate | C0032 | READY_NOT_PROMOTED_DIRECTION_PROTOTYPE |
| Direct parent / visual rollback | C0031 | preserved |
| Functional rollback | C0022 | preserved |
| Latest Answer Pack | R28 | current review pack |
| Latest Handoff | A24 | current handoff |
| Production | HOLD | blocker remains |

## Why the direction changed

After C0031 the user reported that the current design felt visually worse/flatter than the earlier direction. This is material design evidence. The remaining-surface migration was paused rather than blindly extending the C0031 visual language.

## C0032 material result

- Scope is Home + Creator Hub only.
- C0031 information hierarchy and semantic-token foundation are preserved.
- Selective navy/cyan depth, moderate hero typography, one elevated decision surface and grouped pricing/choice surfaces were restored.
- Old card-heavy/glow-heavy styling was not restored.
- C0031 direction heuristic: 80/100.
- C0032 direction prototype heuristic: 88/100. This is a heuristic only, not conversion evidence.
- PC, Apply, Rescue, Stream Ready, YouTube and Editing were re-rendered Desktop+Mobile: 12/12 comparisons returned zero changed pixels.
- 23 application options and 86 application links preserved.
- Prices, service IDs and Apply URLs preserved.
- Static QA PASS; target Home/Creator renders have no horizontal overflow.
- Actual external URL Runtime UNVERIFIED; real device, assistive technology and user conversion NOT_EXECUTED.

## Current hashes

- C0032 Candidate: `66fa34cbe48977aa9a0bd1dcc906e45975da38828b59818e2803954b8f468464`
- R28 Answer Pack: `98ce855c28f454acfc7483751e8c12ca8e5d9735ad03acfb5bb2bc0ab2da8e3b`
- C0032 Local Review V26: `850964563c9341c6c6a39a5dc05e18241e2be35e0c436b183c0275fbd7d91cf8`
- C0032 Visual Evidence: `e4436618363f35385c70265bae1b15103f7aec79f6851cbe8c773fe27a395e4f`
- A24 Handoff local source hash: `999f648be526ef6edc828d7d057bc6116bfeae1ece1c3adfcc7e2610b527a30b`

## Promotion boundary

GitHub storage does not promote C0032. `/upgrade-auto` is still required before Active Control/Preview changes. Production remains HOLD.

## Next

C0033 must not blindly extend C0032 to every page. First use the Home + Creator A/B as direction evidence. If this balance remains stronger, extend in small groups. If not, keep C0031 and create an alternate direction prototype.
