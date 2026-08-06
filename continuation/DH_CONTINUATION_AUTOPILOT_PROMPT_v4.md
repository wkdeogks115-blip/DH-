# DH CONTINUATION AUTOPILOT PROMPT v4

Use the latest valid DH Control, ACTIVE Source, latest Handoff, Answer Pack and Candidate as the locked baseline.

When the user says `계속 진행`, select the highest-priority new Material Delta for the DH consumer-service site and execute a reversible patch Candidate with minimum sufficient tests.

## Automatic design approval

Automatically accept and continue from the latest design direction when:
- the parent and rollback are locked,
- static and scope-specific visual tests pass,
- the change is reversible,
- prices, service IDs, core scope, policy, payment and business identity do not change,
- regressions are zero.

Do not ask the user to approve each reversible design Candidate.

## Explicit gates retained

Do not promote Active Control, deploy, commit, push, delete, or change price, offer, policy, payment, refund or business identity without the existing explicit command or evidence gate. `/upgrade-auto` remains required for promotion.

## Execution rules

- update the Answer Pack only when the conclusion, hashes, priority or artifacts materially change;
- patch one main Material Delta at a time;
- preserve the DH concept: simple, readable, premium, one-accent, consumer-decision first;
- use external repositories as research references, not runtime dependencies, unless explicitly justified;
- keep actual URL Runtime, real device and user tests UNVERIFIED when not executed;
- if no new evidence or Material Delta exists, create no new version and stop with `HOLD — 새 결론 없음`.

End non-trivial responses with:

## 다음 자동 진행
- 현재 1순위
- 완료 조건
- 중단 조건
- 다음 입력: `계속 진행`
