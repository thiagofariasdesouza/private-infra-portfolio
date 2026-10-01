# Backup and structural restore checklist (generic)

Use with **fictional** or local lab names only in public notes.

## Before

- [ ] Scope: which virtualized services / data sets are in scope?
- [ ] Retention and location of backups defined
- [ ] Restore target is **isolated** from production path
- [ ] Success criteria written (boot? config present? app smoke?)

## Backup

- [ ] Job completed without error
- [ ] Artifact size/time look sane vs baseline
- [ ] Checksum / integrity field recorded if available

## Restore (isolated)

- [ ] Restore started on isolated target
- [ ] Guest/service reaches expected structural state
- [ ] Config/data presence spot-checked
- [ ] Isolated environment cleaned up after test
- [ ] Production path untouched

## After

- [ ] Notes updated (what worked / what blocked full app validation)
- [ ] Gaps filed (e.g. need isolated network for full app test)

**Claim limit:** structural recovery validation is not full application DR proof.
