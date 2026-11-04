# CSFC Research Spoke Sync Receipt — November 4, 2026

## Scope

This batch seeded `Feirbrand/csfc-research` and linked it into the existing research spine and brand hub without duplicating the canonical v1.0 paper or series.

Patch 3 touched exactly two files in `csfc-research`:

- `README.md` — exact supplied active-development hub text
- `LICENSE` — exact supplied restricted-public/source-available license text

Patch 4 touched exactly four existing files:

- `synoeticos-public/README.md`
- `synoeticos-public/vulnerability-research/csfc-series/README.md`
- `aaron-slusher-research/ecosystem.md`
- `aaron-slusher-research/PUBLICATIONS.md`

No published paper body, quarantined CSFC detector file, Hugging Face demo, or other file was changed. The Stage 0-6 to Stage 1-5 correction is limited to the authorized Aaron Research publications keyword row.

## Diagnostics

Before editing, both existing repositories were clean and matched their supplied live blob SHAs:

- `synoeticos-public` HEAD/origin: `4734131d5d920962c0d9540aca5d8fa2f47a87f6`
- `aaron-slusher-research` HEAD/origin: `cb91506756480d244065d9c19acb516929898bf7`

The new `csfc-research` repository was not empty as originally described: it contained a single placeholder README in initial commit `d001717925836aa6527126359e8e34c07030ca94`. The placeholder content was:

```text
# csfc-research
Complete Symbolic Fracture Cascade (CSFC) Research
```

After confirmation, that placeholder was replaced by the exact Patch 3 README and the exact supplied LICENSE was added. The resulting root tree contains exactly `README.md` and `LICENSE`.

Supplied Patch 4 blob checks passed:

- `synoeticos-public/README.md`: `ba11d9bd587b2d2be306f3becf46276e9c7b5282`
- `synoeticos-public/vulnerability-research/csfc-series/README.md`: `1bdc6de9d29949e623d3c00907b1302052d76a89`
- `aaron-slusher-research/ecosystem.md`: `5951e30f443003f7537f505e72d951c6d1457c90`
- `aaron-slusher-research/PUBLICATIONS.md`: `9643196c096bcccf11f717d0fe3e764bea8cc505`

## Commits

| Repository | Commit | Message |
|---|---|---|
| `Feirbrand/csfc-research` | `279b752dfe5012755f2fad483cf17c34b05e1f82` | `feat: seed CSFC research spoke` |
| `Feirbrand/synoeticos-public` | `79602f6c933b622831a5c211efa11f12d813493a` | `docs: link CSFC active development repo` |
| `Feirbrand/aaron-slusher-research` | `0ee4e5e594584958dc0df494a899a3b0d4d726f1` | `docs: link CSFC research spoke` |

## File evidence

| Repository | Path | Commit SHA | Git blob SHA-1 | SHA-256 content hash | Bytes |
|---|---|---|---|---|---:|
| `csfc-research` | `README.md` | `279b752dfe5012755f2fad483cf17c34b05e1f82` | `0bb6cf058a7be023960222eac0cf132b5574e2ed` | `facb5e89562cdcdde9a38d8c154d9e60e61d2cd9a0ce09480851f9dfbbd1111d` | 3632 |
| `csfc-research` | `LICENSE` | `279b752dfe5012755f2fad483cf17c34b05e1f82` | `911a56ef95db75442893f474c38e3d781b4d3bfb` | `4b7ee33ef59516149f8402467a27e966fc2bad9283a540a8f9b3cb6b5d622927` | 1935 |
| `synoeticos-public` | `README.md` | `79602f6c933b622831a5c211efa11f12d813493a` | `fa3c3cafaf9ddf63469edadaa295ad2daa0fcc83` | `c067c7cff7f81d06eb6e06041d6931b2c4792fd381d28ecd0a07aac659218ffb` | 28683 |
| `synoeticos-public` | `vulnerability-research/csfc-series/README.md` | `79602f6c933b622831a5c211efa11f12d813493a` | `62ae749e5b9ff3263aa0e6a09d2d0b3f47a751dd` | `5881b268c4ea0adcbaead2c88f477f1cd5319427cbf6df3b906bf0efdaa76025` | 3982 |
| `aaron-slusher-research` | `ecosystem.md` | `0ee4e5e594584958dc0df494a899a3b0d4d726f1` | `b17d97bac18f40f04fc344e4dc69be0f0faa240e` | `c2cc97e3e7473be565f1a8fb406060427becaf85dfd0dd793419611b7b99bdf0` | 6341 |
| `aaron-slusher-research` | `PUBLICATIONS.md` | `0ee4e5e594584958dc0df494a899a3b0d4d726f1` | `72bea5f421bf522a0177e5788c08b0cc913506ab` | `b972d93f093da3ae896df669bbc2fe7d44d59d90b7bd928af7e6428f459dfc96` | 9629 |

## Verification

- Patch 3 README and LICENSE matched the supplied brief byte-for-byte.
- `csfc-research` root tree contains exactly `README.md` and `LICENSE`.
- Patch 4 supplied blobs matched before editing.
- All four Patch 4 new pointers and provenance notes are present.
- `Stage 0-6` is absent from `aaron-slusher-research`.
- The withdrawn `/vgs-loadout/frameworks/csfc/` reference sentence is absent from the CSFC series README.
- Existing canonical DOI paths remain unchanged.
- Only the four allowlisted files changed in Patch 4.
- The intentional two-space Markdown hard break in the Synoeticos root README was preserved.
