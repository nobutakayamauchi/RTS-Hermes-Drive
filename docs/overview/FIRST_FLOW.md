# First Minimal Cross-Repo Flow

## Purpose
This note defines the first minimal structural end-to-end test flow across the four RTS artifacts, without runtime implementation details.

## Artifact Mapping
- **Skill used:** `weekly_dev_report.skill.yaml`
- **Pack required:** `dev_pack.pack.yaml`
- **Drive used:** `hermes_drive.drive.yaml`
- **RTS record target:** `execution_record.schema.yaml`

## Minimal Flow
```text
hermes_drive.drive.yaml -> weekly_dev_report.skill.yaml -> dev_pack.pack.yaml -> execution_record.schema.yaml
```

## Boundary
This is a **structural test flow only** for validating artifact linkage and ordering, not a full runtime implementation.
