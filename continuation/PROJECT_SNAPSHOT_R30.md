# DH PROJECT SNAPSHOT R30

## Locked state

- Active Control: R0003
- Active Preview: C0009A D2
- Current Review Candidate: C0034
- C0034 SHA-256: `55b1eee33f6c03c44ad627b69b952dfe1303fe07055dac35f966abea7d5fd263`
- Direct Parent / immediate rollback: C0033
- C0033 SHA-256: `db4659fb9f7f28ac4ce03c43f71472391a2badcdcc0db1762c281356cc49ad68`
- Brand-depth direction parent: C0032
- Production: HOLD
- Promotion: NOT_EXECUTED

## R30 conclusion

C0034 applies the selective Brand Depth direction to only PC pricing and Apply. It does not change prices, service IDs, Apply URLs, application service options, application link counts, or application JS.

### Design evidence

- PC commercial clarity heuristic: 80 → 87
- Apply trust/completion heuristic: 82 → 88
- overall direction heuristic: 88 maintained
- PC mobile height: 8,439 → 7,871 px (-6.731%)
- Apply mobile height: 3,390 → 3,457 px (+1.976%)

### Mandatory safety evidence

C0033 `apply.js` is byte-identical in C0034 and was executed in Chromium.

- empty form → 6 errors, error-summary focus PASS
- both safety acknowledgements unchecked with other required data valid → no summary, errors `safety_ack`, `scope_ack`
- safety only → `scope_ack` remains
- one availability time → rejected
- blocked submission → input preserved
- both acknowledgements + two availability times → summary generated
- mobile horizontal overflow → 0

### Regression

Home, Creator, Rescue, Stream Ready, YouTube and Editing at Desktop/Mobile: 12/12 zero changed pixels.

### Business invariants

- application options: 23
- application links: 86
- prices: PRESERVED
- service IDs: PRESERVED
- Apply URLs: PRESERVED

## Artifacts

- C0034 Candidate SHA: `55b1eee33f6c03c44ad627b69b952dfe1303fe07055dac35f966abea7d5fd263`
- Local Review V28 SHA: `cd9c2c0f321ea811612a90a53062f0188bcfc7f5d3bcd23b1dd7b98e579b2ff8`
- Browser Evidence SHA: `3000cfa3f711ac47e8c9bf00e104f27033282b0f17e209a4619e3b7ec47a5c3f`
- R30 Answer Pack SHA: `96e579fe097c254c600a821c82dfd2a7a4799d2539bb399d51f45808a73506c0`
- A26 Handoff SHA: `29cbbe79c7065aea2412b0aff1ab10c425a348d957ca5c8d1b1d43827b69fa64`

## Unverified

- external URL Runtime: UNVERIFIED
- real mobile device: NOT_EXECUTED
- assistive technology: NOT_EXECUTED
- conversion study: NOT_EXECUTED

## Next

C0035: Rescue + Stream Ready Brand Depth extension only. Preserve C0034 and all C0033 safety gates.
