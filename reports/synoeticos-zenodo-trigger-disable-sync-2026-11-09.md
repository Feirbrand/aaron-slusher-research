# Synoeticos Zenodo Trigger Disable Receipt — November 9, 2026

## Scope

This patch changed exactly one GitHub Actions workflow in `Feirbrand/synoeticos-public`:

- `.github/workflows/zenodo-metadata.yml`

The automatic `release.types: [published]` trigger was replaced with a manual-only `workflow_dispatch` trigger and the supplied explanatory comment. Permissions, jobs, steps, paper-selection logic, metadata generation, and commit/push behavior were left unchanged.

No published paper body, DOI record, license, repository data file, or unrelated workflow was modified.

## Diagnostics

Before editing, `synoeticos-public` was clean on `main`, with local `HEAD` and `origin/main` at `a22e6cc34c37d2eed0540e26c7dcdfd268f641fd`.

The pre-edit workflow blob matched the supplied value exactly:

- `.github/workflows/zenodo-metadata.yml`: `b252d5421b74c607e718f2045886bfaaf26a85c5`

The exact current trigger block occurred once and was replaced once. The post-edit file was verified byte-for-byte against the pre-edit file with only that trigger-block replacement.

## Commit

| Repository | Commit | Parent | Message |
|---|---|---|---|
| `synoeticos-public` | `389632c520e0707bd19e533ee2d3d530265a722d` | `a22e6cc34c37d2eed0540e26c7dcdfd268f641fd` | `ci: disable automatic Zenodo metadata release trigger` |

## File evidence

| Repository | Path | Change commit SHA | Git blob SHA-1 | SHA-256 content hash | Bytes |
|---|---|---|---|---|---:|
| `synoeticos-public` | `.github/workflows/zenodo-metadata.yml` | `389632c520e0707bd19e533ee2d3d530265a722d` | `eb84622c7e225a46444a24b93d00e31aa76fc5a9` | `9ab9a029f9d89bc66a92717bdca5fb4bb99740e9b323ecbc2d9ec104798a025d` | 2563 |

## Verification

- Exact trigger-block replacement passed.
- The changed-file allowlist was exactly `.github/workflows/zenodo-metadata.yml`.
- The commit changed 7 lines and removed 2 lines, with no unrelated workflow changes.
- `git diff --check` passed.
- The resulting trigger is manual-only: `workflow_dispatch`.
- The release trigger is absent, preventing automatic Zenodo metadata updates on release publication until paper selection is bound to the release tag.
- The worktree was clean after commit.
- Push and post-push remote-parity verification are recorded after the commit is pushed.
- No Pages deployment was implicated; the workflow trigger change is verified through raw GitHub workflow content and repository parity.
