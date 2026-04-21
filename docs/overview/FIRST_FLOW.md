# FIRST_FLOW: Minimal Cross-Repo Structural Flows

## Purpose
This document is a concise structural linkage note for the current minimal cross-repo flow. It is not a runtime implementation design.

## Artifact Mapping
- **`dev_pack.pack.yaml`**
  - `usage_scope: development_workflows`
  - shared pack for `weekly_dev_report` and `issue_to_fix_pr`
- **`hermes_drive.drive.yaml`**
  - `operation_scope: multi_skill_development_flow`
  - shared drive for `weekly_dev_report` and `issue_to_fix_pr`
- **`execution_record.schema.yaml`**
  - `record_scope: cross_repo_skill_execution`
  - shared execution record target

## Minimal Supported Flows
```text
hermes_drive -> weekly_dev_report -> dev_pack -> execution_record
hermes_drive -> issue_to_fix_pr -> dev_pack -> execution_record
```

## Boundary
This note defines structural linkage and artifact ordering only; it does not define full runtime execution logic.
