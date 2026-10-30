# License/Affiliation Sync Receipt — October 30, 2026

## Scope and clarification

Applied `manus_patch_license_affiliation_VERIFIED_2026-10-30.md` to the seven allowlisted files across `Feirbrand/synoeticos-public` and `Feirbrand/aaron-slusher-research`. The frozen DOI paper bodies and root `LICENSE.md` were not changed.

The supplied clarification authorizes preserving the three unrelated historical or biographical `Achieve Peak Performance` references in `synoeticos-public/docs/elevation-grid/index.qmd`: the citation journal, the APA citation, and the author biography. They are outside the four license/affiliation edits and remain unchanged.

## Commits

| Repository | Commit | Message |
|---|---|---|
| `Feirbrand/synoeticos-public` | `4cb1096c44ba910021f2f8c1d3058aa2780c3be8` | `docs: correct Elevation Grid registered license` |
| `Feirbrand/aaron-slusher-research` | `7e716bf7f680805ad128f6e0581f185328187bf7` | `docs: align registered affiliations and licenses` |

## File evidence

| Repository | Path | Git blob SHA-1 | SHA-256 content hash |
|---|---|---|---|
| `synoeticos-public` | `docs/elevation-grid/index.qmd` | `4fd86b7ac1a28fa4d5c8dd5082b1a77e71a125da` | `ca125fbb8d09d13c47755a3bae6136aa204f536473696093b05549fe9ab3f7e9` |
| `aaron-slusher-research` | `PUBLICATIONS.md` | `9643196c096bcccf11f717d0fe3e764bea8cc505` | `4517a5fe2d69c27626379ae2fa5899ddae1dff3b09204d9137af74fe450ec3d7` |
| `aaron-slusher-research` | `ecosystem.md` | `5951e30f443003f7537f505e72d951c6d1457c90` | `87e5af2afb9f1b548d736179c69a49bf2db91822c1a8dd71dc3da00584f0885f` |
| `aaron-slusher-research` | `docs/methods/elevation-grid/index.qmd` | `a5f74c607f7890e34cde6d05f8cd2e89a32c1036` | `8ec99c28474aade2296e211c5f43bde2159f44685853b5810e16c2b009e9ac85` |
| `aaron-slusher-research` | `architecture/elevation-grid/README.md` | `cc5a48600985c00d7c3d3b6fd0a218d764d21332` | `01510000f8a70dce4028381af0b37c05ace97f8373626f25777ac3847aff0c2e` |
| `aaron-slusher-research` | `docs/methods/neuroformation/index.qmd` | `a74cddf78ac209d327b5d60dddad0174a1e7219d` | `249359a694eaf64a23099c39daf4d00cc3bef24f4a8e48f3267861dfef3d6e64` |
| `aaron-slusher-research` | `architecture/neuroformation/README.md` | `868b41cd8ad4ef89d29204b35759d493ad1d5aea` | `2a234e74ad737b0e71202c763d4b7f315359d07614304d7a70bae9c70e4a0328` |

## Verification

The seven-file allowlist passed. `git diff --check` passed in both repositories. Synoeticos Public rendered successfully with Quarto 1.8.0, producing 53 HTML documents; the Elevation Grid page emitted the registered CC BY 4.0 license. Aaron Research proof checks passed: stale Oct 17 Manifest wording was removed from all six files, registered-record values are present, and `whitepapers/academic-papers/neuroformation-v1.0.md`, `whitepapers/academic-papers/elevation-grid-academic-v1.1.md`, and `LICENSE.md` were unchanged.
