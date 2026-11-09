# Synoeticos Hugging Face Link-Map Sync Receipt — November 9, 2026

## Scope

This patch updated stale Hugging Face Space links in exactly three allowlisted Markdown files in `Feirbrand/synoeticos-public`:

- `README.md`
- `vgs-loadout/frameworks/fce/README.md`
- `vgs-loadout/frameworks/slv/README.md`

The replacements were limited to the supplied demo and explorer URL changes: Phoenix, Torque, FCE, DNA Codex, and SLV. No published paper body, DOI record, license, implementation, or unrelated repository path was modified.

## Diagnostics

The pre-edit repository was clean on `main`, with local `HEAD` and `origin/main` at `0382992e95140ebe017cec0ad069e5fdcc86404b`.

All supplied pre-edit blob SHAs matched exactly:

- `README.md`: `c91d40167ccdfb6730c1b18c1ebb4affd3837a43`
- `vgs-loadout/frameworks/fce/README.md`: `249eb172d1c9c08b4f70abea1bccbda6613f8591`
- `vgs-loadout/frameworks/slv/README.md`: `adaff78f5f6fc2f21c4f0ea61116e81e92e6e44f`

Every supplied old-link occurrence was present in its expected file before editing. The working tree contained no unexpected changes.

## Commit

| Repository | Commit | Parent | Message |
|---|---|---|---|
| `synoeticos-public` | `a22e6cc34c37d2eed0540e26c7dcdfd268f641fd` | `0382992e95140ebe017cec0ad069e5fdcc86404b` | `docs: update Hugging Face demo links` |

## File evidence

| Repository | Path | Change commit SHA | Git blob SHA-1 | SHA-256 content hash | Bytes |
|---|---|---|---|---|---:|
| `synoeticos-public` | `README.md` | `a22e6cc34c37d2eed0540e26c7dcdfd268f641fd` | `9dfa32bbf9d891661ad421e12dbd31ef916e57cb` | `61adeb609aa34ad40a0ec2e98c509adac1e6c7467ab1dbcaba675655c1dfa1cd` | 30244 |
| `synoeticos-public` | `vgs-loadout/frameworks/fce/README.md` | `a22e6cc34c37d2eed0540e26c7dcdfd268f641fd` | `9df24eff59aa9d9942e4b8fea9ae8992b38ccb51` | `11ed0cfc64d2f302e9e53a328e983fd9f47d386661af0c39bc2495cfcfcc4712` | 5401 |
| `synoeticos-public` | `vgs-loadout/frameworks/slv/README.md` | `a22e6cc34c37d2eed0540e26c7dcdfd268f641fd` | `742c158995b9c7b1e51da5df15da97643b4e8ae0` | `e9a3f46bc1fa2294aacadf8fbc02fc4c43ccee3124326094310ed7abfca379e5` | 6948 |

## Verification

- Exact supplied old-link contexts were verified before editing.
- The changed-file allowlist was exactly the three files above.
- The resulting commit contains 9 insertions and 9 deletions, all limited to the requested URL substitutions.
- The repository-wide stale-link scan passed. No tracked working-tree occurrence remained for `phoenix-resurrect`, `torque-monitor`, `fce-compressor)`, `dna-codex-search`, or `slv-demo)`.
- `git diff --check` reported only the intentional two trailing spaces on the changed DNA Codex line, preserved from the source Markdown hard-break formatting. No other whitespace issue was present.
- The worktree was clean after commit.
- Push and post-push remote-parity verification are recorded after the commit is pushed.
- No Quarto render was required: the allowlist contains Markdown documentation files only, and the brief specified a stale-link scan rather than a Pages-render check.
