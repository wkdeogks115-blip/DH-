# C0028 — Visual Shell Component Consolidation

Status: `READY_NOT_PROMOTED`

- Candidate SHA-256: `4bdbe123a6e5860979f8af580a06ffd2407c63e2739ef802111679f679315cb7`
- Direct parent: C0027 `0db244b8f483e030d330d66f43b4d2bd262ed06460abf919209e627b996cdd7d`
- Scope: Home, PC pricing, Apply presentation only
- Design score: 80/100, unchanged from C0027 by intent
- Functional heuristic: 84/100 maintained

## Consolidation result

- Runtime CSS: 187,722 → 181,422 bytes
- Visual Shell CSS: 26,397 → 20,097 bytes
- Long repeated scope prefixes: 164 → 0
- Exact visual comparison: 8 audited Desktop/Mobile views, 0 changed pixels
- JavaScript bytes: unchanged from C0027
- Application options: 23
- Application links: 86
- Price / service ID / apply URL drift: 0

## Remaining debt

`!important` declarations in the visual shell remain 473. C0028 does not claim this dependency is resolved.

Actual URL browser Runtime, real-device, assistive-technology and user-conversion tests remain UNVERIFIED / NOT_EXECUTED.

Do not promote or deploy without `/upgrade-auto`.