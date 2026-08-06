# DH CONTROL SNAPSHOT R0001

```yaml
schema_version: 2
control_revision: 1
parent_revision: null
generated_at: 2026-07-29T17:41:00+09:00
project_id: DH_SETUP_CENTER
operating_mode: CONTINUOUS_EVOLUTION_LOW_TOUCH
operation_playbook: DH_OPERATION_PLAYBOOK_v3.2.2

roles:
  INFRA_RUNTIME_ACTIVE:
    source: 01_DH_INFRA_RUNTIME_CAPSULE.md
    status: ACTIVE
  PAGE_LOCAL_ACTIVE:
    embedded_in: 01_DH_INFRA_RUNTIME_CAPSULE.md
    version: v1.3.3
    status: ACTIVE_PROMOTION_CANDIDATE
  SITE_PREVIEW_BASELINE_ACTIVE:
    source: 02_DH_SITE_BASELINE_CURRENT.txt
    lineage: PHASE9_4_RECOVERY_CANDIDATE_V1_4_0_R1
    status: RECOVERY_PREVIEW_BASELINE
  SITE_GOVERNANCE_ACTIVE:
    source: 03_DH_SITE_GOVERNANCE_AND_FIRST5.md
    status: ACTIVE
  SITE_ROLLBACK:
    source: 04_DH_ROLLBACK_REFERENCE.md
    lineage: PHASE9_3_v1.3.0
    status: REFERENCE_ROLLBACK
  RECOVERY_AUDIT:
    source: 05_DH_RECOVERY_AUDIT.md
    status: AUDIT_REFERENCE

excluded:
  - DH_SETUP_CENTER_FOUNDING_LAUNCH_BUNDLE_v1_1_0_CORRUPT
  - PROJECT_INSTRUCTIONS_V2
  - PAGE_LOCAL_v1.3.0_TO_v1.3.2_AS_ACTIVE

validation:
  page_local_crc: PASS
  page_local_static_validator: PASS
  page_local_install_contract: PASS
  page_local_behavior_schema: PASS_21_OF_21
  isolated_new_project_behavior: UNVERIFIED
  site_static_qa: PASS
  site_release_gate: FAIL_HOLD

infrastructure:
  status: BASELINE_LOCKED
  reopen_when:
    - material_finding
    - new_source
    - new_execution_result
    - operating_data
    - model_or_project_migration

production:
  status: HOLD
  blockers:
    - missing_release_gate_documents
    - verified_founding_replacement_or_explicit_recovery_acceptance
    - business_identity
    - final_terms
    - payment_flow
    - analytics_provider_and_consent_verification
    - deployed_preview_runtime_qa
    - explicit_release_approval

source_budget:
  normal_target: 10
  warning_at: 15
  gc_due_at: 18
  hard_hold_at: 20
  gc_every_promotions: 5
  promotions_since_gc: 0

current_work:
  control_chat: 00_인프라·검증·릴리스
  delivery_chat: 01_사이트·상품·운영
  next_stage: 새 프로젝트 설치 검증 후 Preview Baseline 뉴리모델링
  pilot_target: first_5_paid_cases

update_policy:
  command: /upgrade-auto
  project_instructions_change_on_version_only: false
  control_selection: highest_valid_revision_with_parent_lineage
  save_generated_outputs_to_project_sources: true
```
