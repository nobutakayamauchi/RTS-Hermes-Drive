# RTS-Hermes-Drive Status

Status: PARTS / ORCHESTRATION / INVENTORY NEEDED

RTS-Hermes-Drive is the thin drive declaration and orchestration bridge layer for the RTS ecosystem.

It is a component repository, not RTS core.

It is not RTS-Skills.

It is not RTS-MCP-Packs.

It is not RTS-AGE.

It is not a publishing automation system.

It is not a runtime execution engine by default.

## Current Position

This repository should hold thin drive declarations that describe how skills, packs, triggers, and outputs may be connected in a reviewable operator workflow.

Drive manifests should stay declarative.

Social or external workflows should remain at draft/review stage unless separately approved.

Allowed by default:

- document drive declarations
- add concise drive manifests
- clarify trigger, skill, pack, and output relations
- improve drive indexing
- document orchestration boundaries and risks
- keep outputs-to-RTS expectations explicit
- preserve draft/review posture for social or external workflows

Prohibited by default:

- adding publishing automation
- adding autonomous external actions
- adding runtime execution engines
- adding API keys or secrets
- importing canonical RTS-Skills manifests
- importing canonical RTS-MCP-Packs manifests
- importing Talent Registry canonical records
- importing Signal Feed canonical records
- importing RTS trust record canonical data
- turning this repository into RTS core
- turning this repository into RTS-AGE
- broad refactors without an inventory decision

## Drive Manifest Shape

Use a minimal drive manifest shape:

```text
drive_id
purpose
trigger
skill
packs
outputs_to_rts
runtime_notes
```

Any broader runtime behavior should require a separate decision record.

## Boundary

RTS defines the protocol and canonical trust records.

RTS-Skills holds reusable job-shaped skill definitions.

RTS-MCP-Packs holds declarative connector pack definitions.

RTS-AGE may execute or prepare implementation artifacts.

RTS-Hermes-Drive should remain the thin orchestration declaration layer between these parts.

## Minimum Alive Definition

This repository is considered Minimum Alive when:

1. Its role as a thin drive declaration layer is explicit.
2. Its boundaries from skills, packs, runtime, registry, and core repositories are clear.
3. The drive manifest shape is documented.
4. Its next inventory pass is documented.
5. No publishing automation, runtime execution, external action, or secret material is added by the rescue documentation itself.

## Current Decision

Keep this repository.

Treat it as a parts shelf for thin RTS drive and orchestration bridge declarations.

Do not expand it into runtime, publishing, registry, or canonical data implementation without a separate decision record.
