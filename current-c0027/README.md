# C0027 Visual Shell Redesign — source record

## Identity

- Candidate: C0027
- Candidate SHA-256: `0db244b8f483e030d330d66f43b4d2bd262ed06460abf919209e627b996cdd7d`
- Direct parent: C0026 `8088b95c03d5663547a66eb79698d2da673863f96937aa0509fe32a1b643c44e`
- Role: REVIEW_CANDIDATE_NOT_DEPLOY_PAYLOAD
- Promotion: NOT_EXECUTED
- Production: HOLD

## Visual shell source

The Candidate adds `css/visual-shell-c0027.css` only to Home, PC pricing and Apply.

- CSS SHA-256: `5cff2fda4b8f822c5b0b5b6a14a0f4ec8edafdb48621585503b9570a6b9d0184`
- CSS bytes: 26,397
- Runtime CSS total: C0026 161,325 → C0027 187,722 bytes

The exact Candidate ZIP is registered by hash but cannot be mirrored byte-for-byte through the current GitHub connector file transport. Do not claim the full Candidate bytes were read from this repository if they are unavailable.

## Architecture

- Dark neutral technical-service canvas
- One muted cyan action accent
- Home: editorial split hero, unboxed service chooser, pricing rail
- PC: pricing rail/decision table, lower card repetition
- Apply: continuous form canvas, stage dividers, sticky quieter summary
- No external font/framework/design-system dependency

## Invariants

- 23 application options preserved
- 86 application links preserved
- prices preserved
- service IDs preserved
- apply URLs preserved
- application JS unchanged from C0026
- error recovery, focus, touch and value-retention behavior preserved by source parity

Read `audits/DH_C0027_FINAL_AUDIT_R23.json` and `audits/DH_C0027_OBJECTIVE_DESIGN_AUDIT_V2.md` for verified scope and limitations.
