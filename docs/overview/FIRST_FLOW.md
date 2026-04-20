# First Minimal Cross-Repo Flows

## Purpose
This note defines the current minimal structural end-to-end flows across RTS artifacts, without runtime implementation details.

## Artifact Mapping
- **Skill artifacts**
  - `weekly_dev_report.skill.yaml`
  - `issue_to_fix_pr.skill.yaml`
- **Shared pack artifact**
  - `dev_pack.pack.yaml`
  - supports: `weekly_dev_report`, `issue_to_fix_pr`
- **Shared drive artifact**
  - `hermes_drive.drive.yaml`
  - supports: `weekly_dev_report`, `issue_to_fix_pr`
- **RTS record target**
  - `execution_record.schema.yaml` (common record target)

## Minimal Supported Flows
```text
hermes_drive -> weekly_dev_report -> dev_pack -> execution_record
hermes_drive -> issue_to_fix_pr -> dev_pack -> execution_record
```

## Boundary
This is **structural linkage only** for validating artifact compatibility and ordering, not full runtime execution logic.
