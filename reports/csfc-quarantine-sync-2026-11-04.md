# CSFC Quarantine Sync Receipt — November 4, 2026

## Scope

Quarantined the leaked CSFC v2.0 detector materials in `Feirbrand/synoeticos-public` by replacing exactly these two allowlisted files:

- `vgs-loadout/frameworks/csfc/README.md`
- `vgs-loadout/frameworks/csfc/csfc-detector.py`

The replacements match the supplied Patch 2 contents byte-for-byte. No other file in `synoeticos-public` was changed. The Hugging Face demo, published CSFC papers and series parts, the root README Patch 1, the CSFC v2.0 teaser, and all other out-of-scope files were left unchanged.

## Diagnostics

The working tree was clean and local `main` matched `origin/main` at `fb2d081081fccdea46338e98637b6fa93ffc5c4f`. Both supplied current blob SHAs matched exactly:

- `vgs-loadout/frameworks/csfc/README.md`: `86312a795826460f8608376659773988142decf0`
- `vgs-loadout/frameworks/csfc/csfc-detector.py`: `e4c0a816da22ed0f853131ac39efb30dff9d671c`

The pre-edit diagnostic confirmed the leaked threshold map, `RIM_variance_ms` trigger, stage percentages, and operational claims were present.

## Commit

| Repository | Commit | Message |
|---|---|---|
| `Feirbrand/synoeticos-public` | `4734131d5d920962c0d9540aca5d8fa2f47a87f6` | `security: quarantine leaked CSFC v2 detector` |

## File evidence

| Path | Commit SHA | Git blob SHA-1 | SHA-256 content hash | Bytes |
|---|---|---|---|---:|
| `vgs-loadout/frameworks/csfc/README.md` | `4734131d5d920962c0d9540aca5d8fa2f47a87f6` | `7c9e6130f1708ff5fea8cf3188040097329e2886` | `fd867afd9c198c59a55c4840ab746ce94a66ea6648b6d1638236c0dd1b7bc779` | 2404 |
| `vgs-loadout/frameworks/csfc/csfc-detector.py` | `4734131d5d920962c0d9540aca5d8fa2f47a87f6` | `22918f1af6518a05775e604075ce02ec335a2201` | `7b832ac0801fde14a7b35b1a501ef48f77e0d52b1476634d906d5e22bbd34581` | 975 |

## Verification

- Both replacement files matched the supplied brief byte-for-byte.
- Python syntax validation passed without executing the withdrawn stub.
- Scoped leak-marker scan passed for both quarantined files.
- `git diff --check` passed.
- Diff names contained only the two allowlisted files.
- Diff statistics were exactly 35 insertions and 404 deletions across those two files.
- A repository-wide marker scan still finds unrelated `682 documented` and `173 days` claims in explicitly out-of-scope framework READMEs (FCE, MBM, Phoenix Protocol, SLV, and UTME). Those files were not touched because the brief’s allowlist prohibits it; the scoped quarantine proof is the applicable result.
