# Synoeticos Incident Badge and Operational Records Sync Receipt — November 10, 2026

## Scope

This locked patch changed exactly one file in `Feirbrand/synoeticos-public`:

- `README.md`

Two authorized edits were applied. The incidents badge now says “682 Reported” rather than “682 Documented.” The introductory operational-outcomes text now reports the 682 AI incidents and the 679 prevented cascade failures, 3 recoveries, and zero permanent losses as historical operational records, explicitly stating that they are not independently benchmarked recovery times.

The summary bullet, all historical research, TASK-70, manuscript bodies, DOI records, licenses, and every file outside `README.md` were left untouched.

## Diagnostics

Before editing, `synoeticos-public` was clean on `main`, with local `HEAD` and `origin/main` at `a28d9ad9c1d4a4078382377d066001e9736a3993`.

The supplied pre-edit README blob matched exactly:

- `README.md`: `bd96e43dfe2ad79d0693cdff8073e57ce691666e`

The badge context and complete introductory block each occurred exactly once. The resulting file was verified byte-for-byte as the pre-edit README with only the two supplied replacements applied.

## Commit

| Repository | Commit | Parent | Message |
|---|---|---|---|
| `synoeticos-public` | `395b16ee79730c87e3437707feb4e2a9844ea4f4` | `a28d9ad9c1d4a4078382377d066001e9736a3993` | `docs: qualify incident badge and recovery claims` |

## File evidence

| Repository | Path | Change commit SHA | Git blob SHA-1 | SHA-256 content hash | Bytes |
|---|---|---|---|---|---:|
| `synoeticos-public` | `README.md` | `395b16ee79730c87e3437707feb4e2a9844ea4f4` | `df5b3c8721d65d0e89f1369705f447121d021cfd` | `589e41a92285a9b78551108781c90ea3f3bd3679a4bbd578dea2a032075c1f0f` | 31466 |

## Verification

- Exact two-edit transformation passed.
- Changed-file allowlist was exactly `README.md`.
- Commit diff: 5 insertions and 3 deletions.
- `git diff --check` passed.
- The new badge text and operational-records paragraph match the supplied patch exactly.
- The removed industry-baseline sentence and “hours, not days” claim are absent from the replaced intro block.
- The summary bullet, historical research, and other README content were not changed.
- No manuscript, DOI, license, or external record was modified.
- The worktree was clean after commit.
- Push and post-push remote-parity verification are recorded after the commit is pushed.
- No Quarto source file was changed; live README and Pages checks are recorded after deployment.
