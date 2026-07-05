# Repo rules — read first (N4 standard)

**Zone A — AI-OS internal repo** (solo writer, cross-device sync is the point). Canonical standard: `cowork-memory/ai-os/git-repo-topology.md` (ratified 2026-07-01).

- **`main` is the sync branch — commit small, commit to `main`.** Do not accumulate `claude/*` or feature branches; anything branched merges back to `main` before the session ends.
- No force-pushes; never rebase-squash sync history.
- **What never lands here:** privileged case/matter substance, live secrets, client deliverable code (that goes in the client's own Zone-B repo).
- Cross-session state also captures to OB1 at close — repo files alone are not durable across devices.
