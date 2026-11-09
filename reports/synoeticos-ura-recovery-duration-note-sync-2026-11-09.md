# Synoeticos URA Recovery-Duration Note Receipt — November 9, 2026

## Scope

This patch added one dated, additive correction note to `Feirbrand/synoeticos-public/README.md`. The note documents unresolved inconsistencies among the published URA v1.5 Stage 4/Full-Phoenix recovery-duration claims.

The allowlist contained exactly one file:

- `README.md`

The note was inserted immediately above the existing 2026-11-05 UTME correction note, placing it at the top of the correction-note block. The UTME, PME, and Neuroformation notes remain below it unchanged.

No DOI, published manuscript line, license, implementation file, or other README content was modified. The manuscript remains untouched; this is an additive correction note, not a retraction.

## Diagnostics

Before editing, `synoeticos-public` was clean on `main`, with local `HEAD` and `origin/main` at `389632c520e0707bd19e533ee2d3d530265a722d`.

The supplied pre-edit README blob matched exactly:

- `README.md`: `9dfa32bbf9d891661ad421e12dbd31ef916e57cb`

The supplied UTME anchor occurred exactly once. The resulting README was verified byte-for-byte as the pre-edit README with only the supplied URA note and its surrounding blank-line spacing inserted.

## Commit

| Repository | Commit | Parent | Message |
|---|---|---|---|
| `synoeticos-public` | `f5cfb668935c5a2ee87b4dba2bb3ff7d2726dc40` | `389632c520e0707bd19e533ee2d3d530265a722d` | `docs: add URA recovery-duration correction note` |

## File evidence

| Repository | Path | Change commit SHA | Git blob SHA-1 | SHA-256 content hash | Bytes |
|---|---|---|---|---|---:|
| `synoeticos-public` | `README.md` | `f5cfb668935c5a2ee87b4dba2bb3ff7d2726dc40` | `408f8d734cab9307458fe1580b1376ec53983134` | `63d86f7f72d6ae021402092c8fc224186792e73dacf589cef9619415d0a3ffcc` | 31301 |

## Verification

- Exact anchor and insertion checks passed.
- The changed-file allowlist was exactly `README.md`.
- The commit contains exactly 2 insertions and 0 deletions.
- The URA note appears immediately above the UTME note, at the top of the correction-note block.
- Existing UTME, PME, and Neuroformation correction notes remain below it unchanged.
- `git diff --check` passed.
- The worktree was clean after commit.
- Push and post-push remote-parity verification are recorded after the commit is pushed.
- No Quarto render was required: this is a living README correction note, and no published manuscript or Pages source was changed.
