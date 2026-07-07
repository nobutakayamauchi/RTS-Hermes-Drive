# RTS-Hermes-Drive Next Actions

The next goal is an inventory pass, not runtime or publishing expansion.

## Next Tasks

1. List existing drive declarations and shells.
2. Identify which drives are ready, draft, stale, duplicate, risky, or misplaced.
3. Confirm trigger, skill, pack, and output relations for each drive.
4. Confirm whether each drive is purely declarative.
5. Confirm whether social or external workflows remain draft/review only.
6. Check local documentation links.
7. Decide which drive declarations should remain here and which belong in adjacent repositories.

## Suggested Follow-up Files

```text
docs/inventory/drive_inventory.md
docs/contracts/drive_manifest_contract.md
docs/relations/adjacent_repo_boundaries.md
```

## Inventory Categories

Use these labels during the next pass:

- READY: usable as a minimal declarative drive
- DRAFT: useful but incomplete
- STALE: likely outdated or superseded
- DUPLICATE: overlaps another drive
- RISKY: trigger, output, publishing, or external action needs review
- MOVE: belongs in another repository
- ARCHIVE: preserve for history only

## Drive Review Checklist

Each drive should explicitly describe:

- `drive_id`
- `purpose`
- `trigger`
- `skill`
- `packs`
- `outputs_to_rts`
- `runtime_notes`

If a drive implies publishing, autonomous external actions, or broad runtime behavior, mark it as `RISKY` and do not expand it until reviewed.

## Do Not Do Yet

Do not:

- add publishing automation
- add autonomous external actions
- add runtime execution code
- add API keys, tokens, or secrets
- import canonical skill manifests
- import canonical pack manifests
- import registry canonical records
- rewrite all drive manifests at once
- promote a drive to canonical status without review

## Next Recommended Task

Create `docs/inventory/drive_inventory.md`.

That file should list each known drive declaration with:

1. name
2. path
3. purpose
4. status label
5. trigger
6. skill relation
7. pack relation
8. outputs-to-RTS relation
9. external action risk
10. next smallest safe action
