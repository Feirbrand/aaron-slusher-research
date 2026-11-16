# UTME Zenodo Metadata Fix Sync Receipt — November 16, 2026

## Scope

Repository: `Feirbrand/synoeticos-public`

Exactly one file was changed:

- `.zenodo.json`

The approved correction fills the UTME metadata description, version, publication date, and creator affiliation. Existing title, creator name, ORCID, upload type, publication type, access right, and license remain unchanged.

Explicit exclusions:

- `.github/workflows/zenodo-metadata.yml` was not changed. The Nov. 9 manual-trigger containment remains in place.
- No published paper file was changed.
- No GitHub Action was dispatched by this patch.
- No other repository file was changed.

## Diagnostics

The worktree was clean before editing and local `HEAD` matched `origin/main`.

Baseline commit:

- `fc1ac0f79856721c74613c88f7c3c199d0e0caa2`

Supplied baseline blobs matched exactly:

- `.zenodo.json`: `791e959004a965ad0bc66156aaf25cecf56192a7`
- `.github/workflows/zenodo-metadata.yml`: `eb84622c7e225a46444a24b93d00e31aa76fc5a9`

The current `.zenodo.json` matched the supplied old JSON byte-for-byte before editing. The source UTME paper front matter was inspected and confirmed the approved description, date `2025-10-31`, and `ValorGrid Solutions` affiliation and publisher values.

## Commit

| Repository | Commit | Parent | Message |
|---|---|---|---|
| `synoeticos-public` | `cb9bd63aef568a6b73147032a4049527b7fe4d92` | `fc1ac0f79856721c74613c88f7c3c199d0e0caa2` | `fix: correct UTME Zenodo metadata` |

## File evidence

| Repository | Path | Commit SHA | Git blob SHA-1 | SHA-256 content hash | Bytes |
|---|---|---|---|---|---:|
| `synoeticos-public` | `.zenodo.json` | `cb9bd63aef568a6b73147032a4049527b7fe4d92` | `94a0906cf573e10edd7eb9533b8bb99f2032bbff` | `0751e914e7726602795a60afd108eeb99391d21871749122eceb2aae72fe0885` | 683 |

## Verification

- JSON parses successfully.
- Exactly nine keys are present in the required order.
- Description is non-empty and matches the UTME paper front matter verbatim.
- `version` is `v1.0`.
- `publication_date` is `2025-10-31`.
- `creators[0].affiliation` is exactly `ValorGrid Solutions`.
- The file ends with a trailing newline and uses the required two-space indentation.
- Commit diff is exactly 4 insertions and 4 deletions in `.zenodo.json`.
- `git diff --check` passed.
- Workflow blob remains `eb84622c7e225a46444a24b93d00e31aa76fc5a9`.
- No paper file or other path changed.

Push and post-push remote-parity verification will be recorded after the authorized push.
