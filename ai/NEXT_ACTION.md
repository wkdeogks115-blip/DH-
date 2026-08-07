# NEXT ACTION — C0033 SELECTIVE BRAND-DEPTH EXTENSION

## Baseline

- Active Control: R0003
- Active Preview: C0009A D2
- Current Review Candidate: C0032
- C0032 SHA: `66fa34cbe48977aa9a0bd1dcc906e45975da38828b59818e2803954b8f468464`
- Direct parent / immutable visual rollback: C0031
- Functional rollback: C0022
- Current-direction heuristic: 80/100
- C0032 prototype-direction heuristic: 88/100 (heuristic only)
- Functional prototype heuristic: 84/100
- Production: HOLD
- Actual external URL Runtime: UNVERIFIED

## Why the priority changed

User feedback after C0031 reported that the current design felt worse/flatter than earlier versions. This is a material design signal. C0032 therefore paused the planned remaining-page audit/migration and tested a direction correction on Home + Creator Hub only.

## C0032 direction

Keep:
- C0031 information architecture;
- semantic tokens;
- single primary CTA logic;
- lower card repetition;
- accessibility and business invariants.

Restore selectively:
- quiet navy/cyan spatial depth;
- moderate hero typography instead of billboard-scale text;
- one elevated decision surface;
- grouped pricing/choice surfaces;
- stronger but restrained DH visual memory.

Do not return to bright multi-color gradients, glow-heavy buttons, or independent cards everywhere.

## C0033 gate

1. Review C0032 Home + Creator A/B evidence first.
2. If the direction remains stronger, extend only one small group:
   - preferred first group: PC pricing + Apply, because they are the main decision/conversion funnel; or
   - Rescue + Stream Ready if preserving form presentation is safer.
3. Re-render all non-target pages and require zero regression outside explicit scope.
4. Preserve 23 application options, 86 application links, prices, service IDs, Apply URLs, application validation and accessibility behavior.

## Stop conditions

- C0032 looks merely more decorative but not more trustworthy/readable;
- visual depth begins to reintroduce card/glow clutter;
- any non-target regression;
- accessibility or application behavior regression;
- no material improvement over C0031.

## Promotion boundary

C0032/C0033 remain Review Candidates. Do not promote or deploy without `/upgrade-auto`.
