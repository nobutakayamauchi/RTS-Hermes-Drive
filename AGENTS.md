# AGENTS.md

## Scope
This file applies to the entire repository.

## Purpose
RTS-Hermes-Drive is a thin runtime / drive declaration layer in the RTS ecosystem.

## Guardrails
- Keep the drive layer thin.
- Do not place canonical Skill manifests in this repository.
- Do not place canonical MCP Pack manifests in this repository.
- Do not place Talent Registry canonical records in this repository.
- Do not place Signal Feed registry canonical records in this repository.
- Do not place RTS trust record canonical data in this repository.
- Do not add API keys or implementation secrets.
- Prefer declaration-only drive manifests.
- Keep social workflow at draft/review stage; do not add publishing automation.

## Drive manifest shape
Use this minimal shape for new drive manifests:
- drive_id
- purpose
- trigger
- skill
- packs
- outputs_to_rts
- runtime_notes
