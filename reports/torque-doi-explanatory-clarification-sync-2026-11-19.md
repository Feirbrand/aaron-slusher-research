# Torque DOI Explanatory Clarification Sync Receipt — November 19, 2026

## Scope

This synchronization covered two living explanatory documents only.

### `Feirbrand/synoeticos-public`

Exactly one file changed:

- `README.md`

The existing November 14, 2026 correction note received one clause clarification. The four-DOI list, dates, framing, and all unrelated correction notes remain unchanged.

### `Feirbrand/csfc-research`

Exactly one file changed:

- `docs/torque-doi-provenance.md`

Edits A, B, and C clarify settled canonical DOI ownership while preserving historical citation/provenance discrepancies as an open reconciliation matter.

Explicit exclusions:

- No published manuscript was changed.
- No DOI was reassigned.
- No workflow, `PUBLICATIONS.md`, `LICENSE`, or DOI metadata file was changed.
- The DOI table and the “What this document deliberately does not do” section were preserved byte-for-byte.
- The license header was preserved byte-for-byte.

## Diagnostics

Both repositories were freshly fetched and clean before editing, with local `HEAD` matching `origin/main`.

Baselines:

- `synoeticos-public`: `cb9bd63aef568a6b73147032a4049527b7fe4d92`
- `csfc-research`: `3bd564e23e2208a5803c6cd3c39be3ed61648955`

Supplied baseline blobs matched exactly:

- `synoeticos-public/README.md`: `8477af02e92fbb9ac50ba6e25a73663d7e537ea9`
- `csfc-research/docs/torque-doi-provenance.md`: `bfccb79c77f953467646bcbb4d0443e44495d79b`

All exact old contexts were verified. Edit B was applied against the actual Markdown-wrapped source context (`with a third DOI's` followed by `ownership itself in dispute.`), with no fuzzy matching or unrelated reflow.

## Commits

| Repository | Commit | Parent | Message |
|---|---|---|---|
| `synoeticos-public` | `a8f52cdae0e3811d0ae36f89e61b5b156d9b6d63` | `cb9bd63aef568a6b73147032a4049527b7fe4d92` | `docs: clarify Torque DOI citation history` |
| `csfc-research` | `b35ffdf74de1bb0ba7624bc6c79d54273d7dd77e` | `3bd564e23e2208a5803c6cd3c39be3ed61648955` | `docs: clarify Torque DOI canonical ownership` |

## File evidence

| Repository | Path | Commit SHA | Git blob SHA-1 | SHA-256 content hash | Bytes |
|---|---|---|---|---|---:|
| `synoeticos-public` | `README.md` | `a8f52cdae0e3811d0ae36f89e61b5b156d9b6d63` | `e4c1034780a037581b002c3ac888011134d92d12` | `dbac5801d6a86dcd81f1ae39eaa6da58887d47ad1d47961fad3877337a45c171` | 33794 |
| `csfc-research` | `docs/torque-doi-provenance.md` | `b35ffdf74de1bb0ba7624bc6c79d54273d7dd77e` | `7aeead122ae040599416fec7bd02eb10c6c3cae0` | `418cdf116cbdb3cb0fd8f37ec5e1aa73b0351af80631e574595d60bc2d04fa8a` | 4302 |

## Verification

- README clause replacement matches the approved New text exactly.
- All unrelated README correction notes and the surrounding four-DOI structure are unchanged.
- Edit A appears immediately before `## The conflict`.
- Edit B uses the approved canonical-ownership clarification.
- Edit C matches the approved replacement Status section exactly.
- DOI table unchanged byte-for-byte.
- “What this document deliberately does not do” section unchanged byte-for-byte.
- License header unchanged byte-for-byte.
- `git diff --check` passed in both repositories.
- Changed-file allowlist is exact: one file in each repository.
- No paper, workflow, DOI metadata, `PUBLICATIONS.md`, or license file changed.

Push, remote parity, receipt availability, and Pages deployment verification are recorded after the receipt commit and push.
