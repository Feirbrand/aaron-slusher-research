# CSFC and Torque DOI Scope Cleanup Sync Receipt — November 14, 2026

## Scope

This synchronization covered two repositories.

### `Feirbrand/csfc-research`

Exactly five files were changed:

- `README.md`
- `ROADMAP.md`
- `docs/csfc-sub-hub-status.md`
- `docs/torque-measurement-lens.md`
- `docs/torque-doi-provenance.md`

The nine authorized edits removed stale URA cross-links and the URA dependency section, resolved the ROADMAP status wording, removed the URA DOI row while retaining the three non-URA DOI rows, and neutralized the Torque cross-document wording. No published paper body was modified.

### `Feirbrand/synoeticos-public`

Exactly one file was changed:

- `README.md`

One additive dated correction note was inserted above the November 10 note, documenting the Torque DOI citation conflict. Published manuscript text remains unchanged.

## Diagnostics

Both repositories were clean on `main` before editing, and each local `HEAD` matched `origin/main`.

Baseline commits:

- `csfc-research`: `3ef587d45e7c6feab7e494623a36011b88e7e1c3`
- `synoeticos-public`: `202066b19b0dddb18a1ccdeb1a89d688f300dd67`

All supplied file blobs matched exactly:

- `csfc-research/README.md`: `0a0ea829c855443b139eaf4b93519f1eb86c36f9`
- `csfc-research/ROADMAP.md`: `7584afc91b706eca0e3cd244e1dcc1354da51e65`
- `csfc-research/docs/csfc-sub-hub-status.md`: `8ae7ddf1438659091a07cda082c07232357a00bb`
- `csfc-research/docs/torque-measurement-lens.md`: `3068d7ff8f9eab5b27413749eaf82d2c5a731eca`
- `csfc-research/docs/torque-doi-provenance.md`: `1dd22c0304f75e0c056007e9711761d8a0ab1e10`
- `synoeticos-public/README.md`: `68a10b924f645c1d5dd30199d5918b3178183186`

The exact Edit 5 block and the corrected full Edit 8 block were supplied before editing after two scope ambiguities were identified and resolved. No fuzzy matching was used.

## Commits

| Repository | Commit | Parent | Message |
|---|---|---|---|
| `csfc-research` | `3bd564e23e2208a5803c6cd3c39be3ed61648955` | `3ef587d45e7c6feab7e494623a36011b88e7e1c3` | `docs: remove stale URA cross-links from CSFC hub` |
| `synoeticos-public` | `fc1ac0f79856721c74613c88f7c3c199d0e0caa2` | `202066b19b0dddb18a1ccdeb1a89d688f300dd67` | `docs: record Torque DOI citation conflict` |

## File evidence

| Repository | Path | Commit SHA | Git blob SHA-1 | SHA-256 content hash | Bytes |
|---|---|---|---|---|---:|
| `csfc-research` | `README.md` | `3bd564e23e2208a5803c6cd3c39be3ed61648955` | `f42005364aa5ce9270e2ce780e6e43548768be12` | `5204430951e0d7e150dd4104683b1c66e58b1496cec656a1b0357c3a21e89c0f` | 5887 |
| `csfc-research` | `ROADMAP.md` | `3bd564e23e2208a5803c6cd3c39be3ed61648955` | `df0edd99a88381ef19a293e29fc5403e60169003` | `e3fbfdf4edbebdecce1c4a5fc9ff60af4fcb2e0b4f048523da0b350333db053b` | 5510 |
| `csfc-research` | `docs/csfc-sub-hub-status.md` | `3bd564e23e2208a5803c6cd3c39be3ed61648955` | `dd8959cb3e97c730b55907e7de477f3e7a6ef6f0` | `62d412d46600e263c0ed0aab2c199f7fcfb547e16836765b002c866ca20ca431` | 7838 |
| `csfc-research` | `docs/torque-measurement-lens.md` | `3bd564e23e2208a5803c6cd3c39be3ed61648955` | `b8e68ecd553d6d748cb5d5bda4459848b06bbff6` | `09f408c9715c93f1515b7a862bf11306c863c848ebe2235beaebdcbdab4990c0` | 5053 |
| `csfc-research` | `docs/torque-doi-provenance.md` | `3bd564e23e2208a5803c6cd3c39be3ed61648955` | `bfccb79c77f953467646bcbb4d0443e44495d79b` | `20357229cc31174a0fe86ea1464383bfbcdf78c90eabab3fc74c2afc39c18923` | 3476 |
| `synoeticos-public` | `README.md` | `fc1ac0f79856721c74613c88f7c3c199d0e0caa2` | `8477af02e92fbb9ac50ba6e25a73663d7e537ea9` | `4b7bb11825e47885b5220eb4cf849d839c9e415041ca44954644f88c72371bb3` | 33468 |

## Verification

- Case-sensitive `URA` count is zero in all five changed CSFC files.
- `ROADMAP.md` priorities run 1–6 with no gap or duplicate.
- The ROADMAP now records the Nov. 6, 2026 canonical-page resolution and the “reported separately” wording with the documented `τ₃ = 2·r·F·√(D·(1−D))` identity.
- `docs/torque-doi-provenance.md` contains exactly three DOI rows: `17373552`, `17379750`, and `17297590`; the URA DOI row is gone.
- The public README note is newest and precedes the Nov. 10 note.
- Protected published files were byte-identical before and after the patch.
- `git diff --check` passed in both repositories.
- Changed-file allowlists were exact: five CSFC files and one public README.
- No Quarto source file was changed; the public repository change is README-only. Pages deployment verification is recorded after push.
- Both content worktrees were clean after their commits.
- Push and post-push remote-parity verification are recorded after the receipt is pushed.
