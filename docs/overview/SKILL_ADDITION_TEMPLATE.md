# SKILL_ADDITION_TEMPLATE: Semi-Automated Cross-Repo Skill Addition

## Purpose
This document is a concise operating template for coordinating semi-automated skill addition across the current RTS multi-repo structure. It is not a runtime implementation specification.

## When to use this template
Use this template when introducing a new skill that must be represented structurally across shared manifests, pack linkage, and drive-level support.

## Standard repository order
1. `RTS-Skills-`
2. `RTS-MCP-Packs`
3. `RTS-Hermes-Drive`
4. `RTS` (only if schema change is truly needed)

## Standard addition flow
1. Create one new skill manifest in `RTS-Skills-`.
2. In `RTS-MCP-Packs`, update one target pack or create a new pack as needed.
3. In `RTS-Hermes-Drive`, update `hermes_drive.drive.yaml` `supports_skills`.
4. Update `FIRST_FLOW.md` when structural coverage changes enough to justify synchronization.

## Pack decision rule
- Extend an existing pack when the new skill clearly fits that pack's current `usage_scope`.
- Create a new pack when the new skill introduces a distinct operational surface or `usage_scope`.

## Flow document sync rule
- Sync `FIRST_FLOW.md` after meaningful structural expansion.
- Do not require immediate flow-document edits for every tiny manifest-only change.

## Boundary
This template is for structural coordination only. It does not define runtime logic, connector implementation, or evidence/checkpoint internals.
