# AGENTS.md

## Scope
This file applies to the entire repository.

## Required reading

Before editing, read:

1. `README.md`
2. `docs/STATUS.md`
3. `docs/NEXT.md`

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

## Inventory pass boundary
- Treat the next pass as drive inventory and risk review, not runtime or publishing expansion.
- Prefer adding or improving index, inventory, and boundary documentation before changing drive declarations.
- Do not promote a drive to canonical status without a separate review decision.
- If a drive implies publishing, autonomous external actions, or broad runtime behavior, mark it as `RISKY` in inventory documentation instead of expanding it immediately.
- If a drive belongs in another repository, mark it as `MOVE` instead of moving it immediately.

## Drive manifest shape
Use this minimal shape for new drive manifests:
- drive_id
- purpose
- trigger
- skill
- packs
- outputs_to_rts
- runtime_notes

## Validation
- Check for broken local doc links when adding index or onboarding docs.
- For documentation-only changes, report changed files and confirm that no runtime, publishing, external action, secret, registry, or canonical data implementation was added.
