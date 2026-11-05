# CSFC Research README Sync Receipt — November 5, 2026

## Scope

This batch replaced the front-door README in `Feirbrand/csfc-research` with the exact supplied substance-first version. The allowlist contained exactly one file: `README.md`.

`ROADMAP.md`, all files under `docs/`, `LICENSE`, and every other repository path were explicitly left unchanged. The question of deleting `ROADMAP.md` was treated as out of scope because the supplied allowlist says no other file may be touched; it remains in place.

No published paper body, DOI record, implementation file, or existing documentation was modified.

## Diagnostics

The local clone was initially clean at `279b752dfe5012755f2fad483cf17c34b05e1f82` but behind the remote. A fresh fetch showed `origin/main` at `b54b83b7d1ffee4f1eb932a4d7f7757939ce726b`, with root entries `LICENSE`, `README.md`, `ROADMAP.md`, and `docs/`. The local clone was fast-forwarded cleanly before editing.

The pre-edit remote README blob was `3baba51b2cc294d6208e4dd491fe4376a8e74b33`. The replacement was extracted from the supplied brief and matched byte-for-byte before commit.

## Commit

| Repository | Commit | Message |
|---|---|---|
| `Feirbrand/csfc-research` | `e1b945a7d9b20e15ca41886c420447f3e39bbe2b` | `docs: lead CSFC research README with substance` |

Parent commit: `b54b83b7d1ffee4f1eb932a4d7f7757939ce726b`

## File evidence

| Repository | Path | Commit SHA | Git blob SHA-1 | SHA-256 content hash | Bytes |
|---|---|---|---|---|---:|
| `csfc-research` | `README.md` | `e1b945a7d9b20e15ca41886c420447f3e39bbe2b` | `a214a46dda765d09789abcf11c933f7d3c3546cb` | `640ef265429b522c9c6b62d2b7682148e76aeee33fb9efb441f65d5e3b666c0c` | 5429 |

## Verification

- The replacement matched the supplied README content byte-for-byte.
- `git diff --check` passed.
- The pre-commit changed-file allowlist was exactly `README.md`.
- The commit changed exactly `README.md`.
- `ROADMAP.md`, `docs/`, and `LICENSE` were not changed.
- The final local branch equals `origin/main` at `e1b945a7d9b20e15ca41886c420447f3e39bbe2b`.
- The final worktree is clean.
- The remote README at `origin/main` was re-read and matched the supplied brief byte-for-byte.
- This repository is a documentation spoke and has no configured Pages deployment requirement in this brief; verification was performed against the pushed raw GitHub content.
