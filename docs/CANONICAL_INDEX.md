# Canonical Index (External Ownership)

This repository is intentionally a thin drive layer and does **not** host canonical domain manifests/registries.

## Canonical artifacts intentionally out-of-repo
- Skill manifests (canonical)
- MCP Pack manifests (canonical)
- Talent Registry (canonical)
- Signal Feed registry (canonical)
- RTS trust records (canonical)

## In-repo declaration role
This repository declares drive-level wiring only:
- trigger
- skill reference
- pack references
- outputs_to_rts
- runtime_notes

No API keys, trust ledger data, or social publish automation are included here.
