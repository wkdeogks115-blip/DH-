# AGENTS.md — DH Control Contract

## Scope

이 저장소는 `DH 세팅센터 제작·운영 스튜디오`의 Control Plane Archive다. 사이트·상품·디자인·검증·릴리스 상태를 증거 기반으로 유지한다.

## Source priority

1. 최신 유효 Control Snapshot
2. Control이 지정한 ACTIVE Source Capsule
3. 현재 작업의 실제 Candidate·실행 결과
4. 최신 Handoff
5. Rollback·Reference·Archive

낮은 revision이나 오래된 Handoff를 현재 상태에 섞지 않는다.

## Required behavior

- 파일을 실제로 읽은 범위만 근거로 사용한다.
- 실행하지 않은 테스트는 PASS가 아니라 UNVERIFIED다.
- 보고서와 실제 hash·manifest·exit 결과가 다르면 실제 결과를 우선한다.
- 변경은 별도 Candidate에서 수행한다.
- 가역적 디자인 개선은 조건을 통과할 때 자동 승인할 수 있지만 Active 승격은 별도다.
- `/upgrade-auto` 없이는 Active Control·Active Preview를 변경하지 않는다.
- 가격·상품·정책·결제·사업자 정보는 명시적 근거 없이 변경하지 않는다.
- Material Delta가 없으면 새 Candidate·Answer Pack·Handoff를 만들지 않고 `HOLD — 새 결론 없음`으로 종료한다.
- Production 배포, Cloudflare 변경, 삭제, 외부 전송은 명시적 Gate 없이는 실행하지 않는다.

## Current locks

- Active Control: R0003
- Active Preview: C0009A D2
- Review Candidate: C0029
- Direct Parent / Visual Rollback: C0028
- Functional Rollback: C0022
- Latest Answer Pack: R25
- Latest Handoff: A21
- Production: HOLD
- Browser external URL Runtime: UNVERIFIED
- External Preview: DEFERRED_BY_USER

C0029는 GitHub에 저장됐지만 Active가 아니다.

## C0029 evidence boundary

Self-contained Chromium에서 실제 `js/apply.js` 상호작용은 실행되어 PASS했다. 그러나 외부 URL navigation, real-device, assistive-technology, user conversion은 실행되지 않았으므로 각각 UNVERIFIED/NOT_EXECUTED로 유지한다.

## Continuation command

사용자가 `계속 진행`, `그다음 진행`, `알아서 다음`이라고 하면 최신 상태를 잠그고 가장 중요한 Material Delta 1개만 선택해 검증·별도 Candidate 패치·최소 충분 테스트까지 진행한다.

현재 다음 작업은 C0030: `rescue/`와 `stream-ready/` 두 페이지의 Visual Shell migration이다. Creator 페이지까지 같은 Candidate에서 확장하지 않는다.

## Response ending

비단순 작업의 마지막에는 다음을 포함한다.

- 현재 1순위
- 완료 조건
- 중단 조건
- 다음 입력: `계속 진행`
