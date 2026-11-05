# CSFC and Synoeticos Content Corrections Sync Receipt — November 5, 2026

## Scope

This batch applied the independently verified factual and mathematical corrections from the supplied patch brief:

1. Two targeted publication-boundary replacements in `Feirbrand/csfc-research/README.md`.
2. One domain caveat inserted into `Feirbrand/csfc-research/docs/torque-measurement-lens.md`.
3. Two additive, dated correction notes inserted into `Feirbrand/synoeticos-public/README.md` immediately above the existing 2026-10-26 correction note.

The allowlist contained exactly these three files:

- `csfc-research/README.md`
- `csfc-research/docs/torque-measurement-lens.md`
- `synoeticos-public/README.md`

Published paper bodies, DOI records, licenses, implementation files, and all other repository paths were left unchanged. The five existing README mentions of the UTME/PME figures were not rewritten; the authorized additive notes document the issue without churning those references.

## Diagnostics

### `Feirbrand/csfc-research`

- Supplied baseline `HEAD` and `origin/main`: `f5746c00184441824300e96eb3e22cfb759e217c`
- Supplied `README.md` blob matched: `a3fa6992ed34561e857130222ee5f1e91ac6747e`
- Supplied Torque-document blob matched: `622841a415b9b2cdd2b8a3808adb902c3de01222`
- Both README replacement strings occurred exactly once.
- The Torque insertion sentence occurred exactly once.
- The working tree was clean before editing.

### `Feirbrand/synoeticos-public`

- The local clone was clean but one fast-forward behind; it was advanced from `b9ebb9baffb5eed093fb00b1b86f2a1f3767bf20` to the supplied `origin/main` baseline `79602f6c933b622831a5c211efa11f12d813493a` before editing.
- Supplied `README.md` blob matched: `fa3c3cafaf9ddf63469edadaa295ad2daa0fcc83`
- The 2026-10-26 correction-note anchor occurred exactly once.
- The two new entries were inserted in the required order immediately above that anchor.

## Commits

| Repository | Commit | Parent | Message |
|---|---|---|---|
| `csfc-research` | `4922989c556e84df7be9f0ec4201f5ced4af631f` | `f5746c00184441824300e96eb3e22cfb759e217c` | `docs: qualify CSFC publication boundaries` |
| `csfc-research` | `3ef587d45e7c6feab7e494623a36011b88e7e1c3` | `4922989c556e84df7be9f0ec4201f5ced4af631f` | `docs: add Torque identity domain caveat` |
| `synoeticos-public` | `0382992e95140ebe017cec0ad069e5fdcc86404b` | `79602f6c933b622831a5c211efa11f12d813493a` | `docs: add UTME and PME correction notes` |

## File evidence

| Repository | Path | Change commit SHA | Git blob SHA-1 | SHA-256 content hash | Bytes |
|---|---|---|---|---|---:|
| `csfc-research` | `README.md` | `4922989c556e84df7be9f0ec4201f5ced4af631f` | `0a0ea829c855443b139eaf4b93519f1eb86c36f9` | `bc487047f37c884675b8fd064ea3c894b2843b978dc1b211c007d0ac4525f735` | 5945 |
| `csfc-research` | `docs/torque-measurement-lens.md` | `3ef587d45e7c6feab7e494623a36011b88e7e1c3` | `3068d7ff8f9eab5b27413749eaf82d2c5a731eca` | `802c90e807a1aa7f3385fe2d3e911130eaa0e3bc1be972e69a47f2095ee4a3db` | 5113 |
| `synoeticos-public` | `README.md` | `0382992e95140ebe017cec0ad069e5fdcc86404b` | `c91d40167ccdfb6730c1b18c1ebb4affd3837a43` | `953ef56463f218bfccc099a94458e4bf92c96ca81e5d717268882c1231b2c4a5` | 30225 |

## Verification

- All three logical units passed exact-context checks before editing.
- `git diff --check` passed for every repository and commit.
- Each logical commit changed only its allowlisted file.
- CSFC README commit: exactly 2 insertions and 2 deletions.
- Torque commit: exactly 2 insertions and 0 deletions.
- Synoeticos README commit: exactly 4 insertions and 0 deletions.
- The CSFC README replacements match the supplied replacement strings exactly.
- The Torque domain note appears directly after the specified sentence and matches the supplied text exactly.
- The two Synoeticos correction entries appear exactly as supplied, in the required order, immediately above the existing 2026-10-26 entry.
- No published manuscript text was changed.
- The receipt itself is a separate documentation commit in `aaron-slusher-research`; push and post-push parity verification are recorded after that commit is pushed.
- No Quarto render was required: all authorized edits are living Markdown README/documentation corrections, and the brief specified no Pages URL check.
