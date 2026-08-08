# C0035 — Rescue + Stream Ready Brand Depth Review Candidate

Status: `READY_NOT_PROMOTED`

## Identity
- Candidate SHA-256: `c9369108b2f1fb39df78583c23700c6bfe083f1f0e0a42bf6b054b2edd7a217c`
- Direct parent: C0034
- Direct parent SHA-256: `55b1eee33f6c03c44ad627b69b952dfe1303fe07055dac35f966abea7d5fd263`
- Scope: `rescue/`, `stream-ready/`

## Material delta
C0035 extends the selective Navy/Cyan Brand Depth direction to the two service pages while preserving the C0030/C0031 information architecture.

It adds selective depth to:
- hero proof;
- service-choice rail;
- scope/readiness matrix;
- report/step grouped surface;
- pricing comparison.

It does not reintroduce independent-card repetition, glow-heavy buttons or multi-color gradients.

## Visual audit correction
The first visual render retained one purple Stream Ready primary CTA. That intermediate result was rejected. The final candidate normalizes target-page primary CTAs to a cyan family.

## Measured result
- Service trust heuristic: 80 → 87
- Decision clarity: 84 → 88
- Rescue mobile: 7,296 → 7,335 px (+0.535%)
- Stream Ready mobile: 7,295 → 7,224 px (-0.973%)
- Non-target parity: PASS 12/12 zero changed pixels
- Target overflow: 0

## Mandatory safety invariant
C0033 safety validation was rerun using the actual candidate `apply.js` and passed. `apply.js` is byte-identical to C0034.

## Business invariants
- application options: 23
- application links: 86
- prices: preserved
- service IDs: preserved
- Apply URLs: preserved

## Boundaries
- Active Control remains R0003.
- Active Preview remains C0009A D2.
- Production remains HOLD.
- Promotion is NOT_EXECUTED.
- External URL Runtime remains UNVERIFIED.
