# DH PROJECT SNAPSHOT R28

## Locked control state

- Active Control: R0003
- Active Preview: C0009A D2
- Infrastructure: BASELINE_LOCKED
- Production: HOLD
- External Preview: DEFERRED_BY_USER
- Payment: NOT_IMPLEMENTED

## Current review state

- Current Review Candidate: C0032
- Candidate SHA-256: `66fa34cbe48977aa9a0bd1dcc906e45975da38828b59818e2803954b8f468464`
- Direct Parent / Visual Rollback: C0031
- C0031 SHA-256: `45d1b8d7fd70fcfe16ce450c6fe5ad4957b26c40cf4bb3b3924260a2863e3ddd`
- Functional Rollback: C0022
- Latest Answer Pack: R28 `98ce855c28f454acfc7483751e8c12ca8e5d9735ad03acfb5bb2bc0ab2da8e3b`
- Latest Handoff: A24
- Promotion: NOT_EXECUTED

## Material Delta

After C0031 the user reported that the current design looked worse/flatter than the earlier direction. The feedback was treated as material evidence and the planned remaining-page migration was stopped.

C0032 is a controlled A/B direction prototype on Home + Creator Hub only. It preserves C0031 information architecture but restores selective navy/cyan depth, moderate hero typography, one elevated decision surface and grouped pricing/choice surfaces. It deliberately does not return to bright multi-color, glow-heavy, or card-heavy styling.

## Evidence

- C0031 direction heuristic: 80/100
- C0032 prototype direction heuristic: 88/100, heuristic only
- PC/Apply/Rescue/Stream/YouTube/Editing Desktop+Mobile: 12/12 zero changed pixels
- Application options: 23
- Application links: 86
- Prices/service IDs/Apply URLs: preserved
- Candidate ZIP CRC/reproducibility: PASS
- Local Review V26 CRC/reproducibility: PASS
- Visual Evidence CRC/reproducibility: PASS
- Answer Pack R28 CRC/reproducibility: PASS

## Unverified

- Actual external URL Browser Runtime: UNVERIFIED
- Real mobile device: NOT_EXECUTED
- Assistive technology: NOT_EXECUTED
- User conversion test: NOT_EXECUTED

## Next

C0033 must evaluate the C0032 A/B direction before extension. If the direction remains stronger, extend in small groups. If not, preserve C0031 and create a different prototype. Do not blindly redesign every remaining page.
