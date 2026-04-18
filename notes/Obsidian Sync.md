# Obsidian Vault Git Sync

**Vault location on VPS:** `/root/.openclaw/workspace/rufus-vault`

This vault is shared between Rufus (VPS) and Amanda (local Obsidian via Working Copy on iOS). Changes must be committed and pushed to be visible on either end.

-----

## After Editing a File (Push)

Run this from the vault directory after any file write:

```bash
cd /root/.openclaw/workspace/rufus-vault
git add -A
git commit -m "rufus: <brief description of what changed>"
git push origin main
```

> Always push after editing. Amanda won’t see changes until they’re in the remote repo.

-----

## Before Editing a File (Pull)

Before writing to any vault file, pull first to avoid conflicts:

```bash
cd /root/.openclaw/workspace/rufus-vault
git pull origin main
```

-----

## Full Sync Sequence (Recommended)

When in doubt, do a full pull-then-push cycle:

```bash
cd /root/.openclaw/workspace/rufus-vault
git pull origin main
# ... make edits ...
git add -A
git commit -m "rufus: <description>"
git push origin main
```

-----

## Setup Notes

- **Remote:** The vault repo must have a `git remote` pointing to the shared repo (GitHub or similar). Verify with `git remote -v`.
- **Auth:** If pushing requires credentials, ensure an SSH key or token is configured on the VPS. Check with `ssh -T git@github.com`.
- **Branch:** Assumes `main`. Adjust if your default branch differs.
- **Conflicts:** If `git pull` reports a conflict, do not auto-resolve — flag Amanda before proceeding.
- **Working Copy (iOS):** Amanda pulls/pushes manually via Working Copy. Auto-sync may not always be on, so Rufus should always push promptly after edits.

-----

## Commit Message Convention

```
rufus: update <filename> - <one line reason>
```

Examples:

- `rufus: update projects.md - added BankBud deploy notes`
- `rufus: create defi-notes.md - new LP bot research`