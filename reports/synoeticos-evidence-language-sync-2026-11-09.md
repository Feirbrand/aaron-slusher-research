# Synoeticos Evidence-Language Sync Receipt — November 9, 2026

## Scope

This patch made six authorized wording corrections in exactly two files in `Feirbrand/synoeticos-public`:

- `README.md`
- `docs/elevation-grid/index.qmd`

The changes reduce evidentiary overstatement without adding stronger claims. The README incident wording now identifies an operational corpus rather than independent scientific validation, and the bibliography wording now describes a reference bibliography across component mechanisms. The Elevation Grid athlete descriptions and timeline heading were generalized exactly as supplied.

No file outside the two-file allowlist was modified. The Chris Oats paragraph, the “Validated in stroke recovery…” line, the License/Affiliation section, and the “Combat Sports Validation” label were explicitly out of scope and remained untouched. No published paper body, DOI, license, or citation record was changed.

## Diagnostics

Before editing, `synoeticos-public` was clean on `main`, with local `HEAD` and `origin/main` at `f5cfb668935c5a2ee87b4dba2bb3ff7d2726dc40`.

The supplied pre-edit blobs matched exactly:

- `README.md`: `408f8d734cab9307458fe1580b1376ec53983134`
- `docs/elevation-grid/index.qmd`: `4fd86b7ac1a28fa4d5c8dd5082b1a77e71a125da`

All six supplied old contexts occurred exactly once before editing.

## Commit

| Repository | Commit | Parent | Message |
|---|---|---|---|
| `synoeticos-public` | `a28d9ad9c1d4a4078382377d066001e9736a3993` | `f5cfb668935c5a2ee87b4dba2bb3ff7d2726dc40` | `docs: qualify incident and athlete evidence wording` |

## File evidence

| Repository | Path | Change commit SHA | Git blob SHA-1 | SHA-256 content hash | Bytes |
|---|---|---|---|---|---:|
| `synoeticos-public` | `README.md` | `a28d9ad9c1d4a4078382377d066001e9736a3993` | `bd96e43dfe2ad79d0693cdff8073e57ce691666e` | `e0e7f466564f0e1b91bfbf33c6717a1139651395403339777845076cb27c9180` | 31356 |
| `synoeticos-public` | `docs/elevation-grid/index.qmd` | `a28d9ad9c1d4a4078382377d066001e9736a3993` | `7512ff522e4d7eb712e5c9f252af3c930f76d04c` | `ee7a6a6d23a3629d2f0602e2b1b6bc56b97b50d7013bea1d7c7ea0bee7dd7738` | 11416 |

## Verification

- Exact six-edit transformation passed.
- Changed-file allowlist was exactly `README.md` and `docs/elevation-grid/index.qmd`.
- Commit diff: 8 insertions and 8 deletions.
- The proof scan found none of the following in either changed file: `682 Documented Incidents`, `Complete 250+ study bibliography`, `Team USA`, `Gold Medalist`, `Player of the Game`, or `28-Year Timeline`.
- Required replacement wording is present.
- Excluded-context counts for Chris Oats, “Validated in stroke recovery”, “Combat Sports Validation”, License, and Affiliation were unchanged from the pre-edit versions.
- `git diff --check` passed.
- Quarto 1.8.0 render passed for `docs/elevation-grid/index.qmd`, with the expected Elevation Grid title and description metadata emitted.
- The worktree was clean after commit.
- Push and post-push remote-parity verification are recorded after the commit is pushed.
- No claim-strength increase was introduced; the edits narrow or qualify wording as authorized.
