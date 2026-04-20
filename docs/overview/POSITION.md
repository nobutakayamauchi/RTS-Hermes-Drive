# RTS Hermes Drive Repository Position

## What this repository is

RTS Hermes Drive is the orchestration and runtime bridge layer.

This repository is responsible for running skills, dispatching jobs, routing triggers, and connecting operational execution to the RTS ecosystem through a Hermes-oriented drive model.

This repository is not RTS itself.
This repository is not the canonical home of skill definitions.
This repository is not the canonical home of MCP pack definitions.

It is the drive layer.

## Core responsibility

RTS Hermes Drive is responsible for:
- receiving triggers from manual, scheduled, or event-based sources
- selecting and invoking compatible skills
- loading or connecting required packs
- dispatching execution in a Hermes-oriented runtime model
- routing outputs to their destinations
- returning execution results in a form recordable by RTS

## Non-responsibility

RTS Hermes Drive does not:
- define the canonical trust model
- own the long-term source of truth for records
- redefine skill meaning
- absorb pack responsibility into runtime glue
- become the only valid execution environment for RTS

## Design stance

The drive layer should remain thin.

It should run skills, not redefine them.
It should connect packs, not replace them.
It should return results to RTS, not become the trust ledger itself.

If Hermes proves useful, this repository should integrate with it.
If Hermes proves unsuitable, the RTS architecture should still survive without collapsing.

## Dependency stance

This repository may depend on:
- skill definitions
- pack declarations
- Hermes-compatible runtime interfaces
- routing, scheduling, and dispatch logic

This repository should avoid creating deep lock-in that would make future replacement of Hermes impossible.

## Expected artifacts

Typical artifacts in this repository include:
- drive manifests
- trigger routing definitions
- scheduler hooks
- dispatch logic
- skill launch contracts
- result handoff logic
- runtime integration notes
