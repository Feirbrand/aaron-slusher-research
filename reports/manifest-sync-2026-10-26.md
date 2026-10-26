# Manifest Sync Receipt — October 26, 2026

## Scope and diagnostic

This batch applied the supplied `MANUS_BATCH_Oct26_2026_README_correction.md` exactly within its declared scope. The only public-content change is one additive correction-note entry in `Feirbrand/synoeticos-public/README.md`. The published manuscript body, `PUBLICATIONS.md`, Notion, Hugging Face, and all other files were left untouched.

Fresh diagnostic fetch confirmed `synoeticos-public` remote `main` at `4f16ba48c2506ab2e749efca3df1d193ac9d240e`; the local clone was one clean fast-forward behind at `c7509926d2cf1a8db445dad443e20e29925dd138`. The fast-forward contained only the upstream `codex/dna-codex/README.md` correction, outside this task. The manuscript contains the cited chi-square statistics at the expected evidence locations, including the primary `χ²(4) = 3.21, p = 0.523` statement and the related MI Agents, UNICA, and UTME figures. No manuscript edit was made.

## Applied commit

| Repository | Commit | Message | File |
|---|---|---|---|
| `Feirbrand/synoeticos-public` | `bd5f1c0ecc88ad7148a6cfa7fbf2c746bdacbc46` | `docs: add Neuroformation statistics correction note` | `README.md` |

The note is positioned immediately above the existing March 24, 2026 Neuroformation entry. It states that the cited statistical claims are unverified pending recovered data or independent replication, identifies the related UNICA/UTME figures, limits the caveat to those statistics, and explicitly says the manuscript text is unchanged and the note is additive rather than a retraction.

## File evidence

| Path | Commit | Git blob SHA-1 | SHA-256 content hash | Bytes |
|---|---|---|---|---:|
| `README.md` | `bd5f1c0ecc88ad7148a6cfa7fbf2c746bdacbc46` | `64c3e38162b258686b2365c4dea15f38d826c17d` | `aeeddc7935c47759057fa60777de7b8c4734f107742ff71427f0640d9f53c7d1` | 28,512 |

## Verification

Quarto `1.8.0` rendered all 53 HTML documents successfully to a temporary output directory. `git diff --check` passed. The working diff before commit contained exactly `README.md`; the frozen `whitepapers/academic-papers/neuroformation-v1.0.md` had no diff. The correction note occurs exactly once and precedes the March 24 entry.

No new Artifact Corpus row was created. No Hugging Face update was attempted. No paper body, `PUBLICATIONS.md`, or Notion record was changed.

## Post-push closure

The authorized pushes completed without force-push. Final heads before this receipt-closure commit were `c694d7544b6fbd1bd87feb9ea4057eb248943cdd` for `aaron-slusher-research` and `bd5f1c0ecc88ad7148a6cfa7fbf2c746bdacbc46` for `synoeticos-public`.

[Aaron Research workflow run 40389143407](https://github.com/Feirbrand/aaron-slusher-research/actions/runs/40389143407) completed successfully for head `c694d7544b6fbd1bd87feb9ea4057eb248943cdd`. [Synoeticos Public workflow run 40389146722](https://github.com/Feirbrand/synoeticos-public/actions/runs/40389146722) completed successfully for head `bd5f1c0ecc88ad7148a6cfa7fbf2c746bdacbc46`.

The live Synoeticos and Aaron Research Pages roots both returned HTTP 200. The raw README at the pushed Synoeticos commit returned HTTP 200, contained the October 26 correction note exactly once, and placed it before the March 24 entry. Both local clones matched their remote `origin/main` refs and had clean working trees. The receipt was publicly accessible at `https://raw.githubusercontent.com/Feirbrand/aaron-slusher-research/c694d7544b6fbd1bd87feb9ea4057eb248943cdd/reports/manifest-sync-2026-10-26.md`.

GitHub workflow annotations were informational only: Node.js 20 action deprecation and the planned `ubuntu-latest` migration to Ubuntu 26. They did not affect the successful builds or deployments.
