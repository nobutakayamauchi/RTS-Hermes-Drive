# First Minimal Cross-Repo Flow

## Purpose
This note defines the first minimal structural end-to-end test flow across the four RTS artifacts, without runtime implementation details.

## Artifact Mapping
- **Skill used:** `weekly_dev_report.skill.yaml` (declares inputs and outputs)
- **Pack required:** `dev_pack.pack.yaml` (supports `weekly_dev_report`)
- **Drive used:** `hermes_drive.drive.yaml` (supports `weekly_dev_report`)
- **RTS record target:** `execution_record.schema.yaml` includes `skill_id`, `drive_id`, `pack_id`, `trigger`, `result`, and `timestamp`

## Minimal Flow
```text
hermes_drive -> weekly_dev_report -> dev_pack -> execution_record
```

## Boundary
This is a **structural test flow only** for validating artifact linkage and ordering, not a full runtime implementation.
