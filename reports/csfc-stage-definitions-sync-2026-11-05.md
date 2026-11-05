# CSFC Stage Definitions Sync Receipt — November 5, 2026

## Scope

This batch expanded `Feirbrand/csfc-research` with substantive public-level technical definitions for the five CSFC failure stages, the Vulnerability Window, and a directory index. It also added the explicitly authorized one-line pointer in the root `README.md`.

The allowlist contained exactly these eight files:

- `README.md`
- `docs/stages/README.md`
- `docs/stages/stage-1-data-fragmentation.md`
- `docs/stages/stage-2-symbolic-identity-fracturing.md`
- `docs/stages/stage-3-symbolic-drift-cascade.md`
- `docs/stages/vulnerability-window.md`
- `docs/stages/stage-4-role-obsolescence-cascade.md`
- `docs/stages/stage-5-complete-collapse.md`

No published paper body, DOI record, license file, implementation file, or unrelated repository path was modified. Protected implementation details—including thresholds, formulas, percentages, response timings, telemetry, and private recovery mechanics—were not added.

## Diagnostics

The `csfc-research` working tree was clean at `e1b945a7d9b20e15ca41886c420447f3e39bbe2b`, and `origin/main` matched that parent before the change. The repository remained on `main` with the authorized `Feirbrand/csfc-research` origin.

The seven stage files were matched byte-for-byte against the supplied Patch 6 content before commit. The root README change was verified as exactly one insertion: the authorized pointer immediately after the five-stage table.

## Commit

| Repository | Commit | Parent | Message |
|---|---|---|---|
| `Feirbrand/csfc-research` | `9767911a2c6495eaa1fd7532bdc09c077d2c49a9` | `e1b945a7d9b20e15ca41886c420447f3e39bbe2b` | `docs: add public CSFC stage definitions` |

## File evidence

| Repository | Path | Commit SHA | Git blob SHA-1 | SHA-256 content hash | Bytes |
|---|---|---|---|---|---:|
| `csfc-research` | `README.md` | `9767911a2c6495eaa1fd7532bdc09c077d2c49a9` | `7c922f78ce6c00347b6197a6a27eb4b0430a0743` | `a63cdb018a0e7bdc571525524a321b01eedd86f8c53bf316d7e9363d1b537a2d` | 5579 |
| `csfc-research` | `docs/stages/README.md` | `9767911a2c6495eaa1fd7532bdc09c077d2c49a9` | `25bbf1a96249688142e40dcf17a65aafcb9381c9` | `2e2223372815b1ef965374463af56fd914e2bea66c5827122a46238a990881da` | 1243 |
| `csfc-research` | `docs/stages/stage-1-data-fragmentation.md` | `9767911a2c6495eaa1fd7532bdc09c077d2c49a9` | `bc621e2ff99d4cd24f3d50ad04d2060dbc5f9a93` | `28a39773fa8a410138263f90dea2d47306f7d2c885877dd01ddd8f98d271e0cb` | 3009 |
| `csfc-research` | `docs/stages/stage-2-symbolic-identity-fracturing.md` | `9767911a2c6495eaa1fd7532bdc09c077d2c49a9` | `67022834610bd1192aceb2b4a8404ef660fa7a85` | `a39af55939aba3c15e85dfaf5babf1c610c0f15e7c51a219b6ca727632df22bc` | 3145 |
| `csfc-research` | `docs/stages/stage-3-symbolic-drift-cascade.md` | `9767911a2c6495eaa1fd7532bdc09c077d2c49a9` | `54c6697b1b1bfc86dadf18dd9009c20b1b76a786` | `f398108cca3fb4a0594947959e70e604092496a72cde9c2919ea99a947768cec` | 2879 |
| `csfc-research` | `docs/stages/vulnerability-window.md` | `9767911a2c6495eaa1fd7532bdc09c077d2c49a9` | `c2169ac6e04e686b06d72505d469d4dac65008d1` | `4c77fae9bde489e9bcd58ec40528cf565da0ea4a1490a54d1063f9cc4ee46289` | 3202 |
| `csfc-research` | `docs/stages/stage-4-role-obsolescence-cascade.md` | `9767911a2c6495eaa1fd7532bdc09c077d2c49a9` | `9922ba1717429d043defbcc5e88fc3f4709d1e5d` | `5e1982b78c95d27f63fb33f0b822fa0d00409fcb33eb9ad28ca3efbb1bb7d2a3` | 3108 |
| `csfc-research` | `docs/stages/stage-5-complete-collapse.md` | `9767911a2c6495eaa1fd7532bdc09c077d2c49a9` | `968685116d164aebdb79e098b589a50a0d9fcde9` | `0482037aed7520688c76fef6641049741c7b22a5001c2d1a37360e1498b8db81` | 3179 |

## Verification

- The staged changed-file allowlist was exactly the eight paths listed above.
- The seven stage files matched the supplied Patch 6 content byte-for-byte.
- The README proof was exact: one insertion and zero deletions, with the authorized pointer text.
- `git diff --cached --check` passed; no whitespace errors were reported.
- Relative links in every file under `docs/stages/` resolved locally.
- The protected-IP scan passed: no percent signs, `RIM_variance`, `THRESHOLD_MAP`, or explicit response-duration markers were present in the stage files.
- The commit changed exactly eight files and added 307 lines.
- Push and post-push remote-parity verification are recorded after the commit is pushed.
- The CSFC repository is a documentation spoke; no Quarto Pages deployment was specified for this Patch 6 brief. The local Markdown/link and content-scope checks above are the applicable pre-push validation.
