# FIRST_FLOW: Minimal Cross-Repo Structural Flows

## Purpose
This document is a concise structural linkage note for the current minimal supported cross-repo flows. It is not a runtime implementation design.

## Artifact Mapping
- **`dev_pack.pack.yaml`**
  - `usage_scope: development_workflows`
  - shared pack supporting:
    - `weekly_dev_report.skill.yaml`
    - `issue_to_fix_pr.skill.yaml`
    - `failed_build_to_patch_plan.skill.yaml`
    - `sentry_error_to_root_cause_report.skill.yaml`
- **`hermes_drive.drive.yaml`**
  - `operation_scope: multi_skill_development_flow`
  - shared drive supporting:
    - `weekly_dev_report.skill.yaml`
    - `issue_to_fix_pr.skill.yaml`
    - `failed_build_to_patch_plan.skill.yaml`
    - `sentry_error_to_root_cause_report.skill.yaml`
- **`execution_record.schema.yaml`**
  - `record_scope: cross_repo_skill_execution`
  - common execution record target for all four flows

## Minimal Supported Flows
```text
hermes_drive -> weekly_dev_report -> dev_pack -> execution_record
hermes_drive -> issue_to_fix_pr -> dev_pack -> execution_record
hermes_drive -> failed_build_to_patch_plan -> dev_pack -> execution_record
hermes_drive -> sentry_error_to_root_cause_report -> dev_pack -> execution_record
```

## Boundary
This note defines structural linkage and artifact ordering only; it does not define full runtime execution logic.
