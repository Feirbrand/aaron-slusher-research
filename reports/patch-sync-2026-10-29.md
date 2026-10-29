# Patch Sync Receipt — October 29, 2026

## Scope

Applied `/home/ubuntu/upload/synoeticos-public-validation-language.patch` to `Feirbrand/synoeticos-public`. The patch changed only `README.md` and `docs/elevation-grid/index.qmd`.

The patch removes unsupported or overly strong Elevation Grid validation and habit-retention language and replaces it with neutral diagnostic wording. No DOIs, citations, data values outside the supplied patch, or published paper bodies were changed.

## Patch application

- Base commit: `3fd57298a12fef9e7d0b8c1d559c90143a27240c`
- `git apply --check`: PASS
- Applied commit: `1dc29f2be6c52a7c1276d9c93811a47784816a57`
- Commit message: `docs: neutralize Elevation Grid validation language`
- `git diff --check`: PASS

## Touched-file evidence

| Path | Git blob SHA-1 | SHA-256 content hash | Bytes |
|---|---|---|---:|
| `README.md` | `82fec27ef48cebefde49bc9afb20421c97493bde` | `83a895d1d5db050927e50f85c424963a0de0ee1d6c17e592abd807a904024d32` | 28,492 |
| `docs/elevation-grid/index.qmd` | `81cef68599e4c6ffaea04e524fbbe9aed8a29319` | `48755fe6c29a9b493e01542c7ea017c04bbe592265cb2fd3b5524e759b10b083` | 11,627 |

## Verification

- Quarto: `1.8.0`
- Rendered documents: 53
- Targeted removed claims absent from source and rendered Elevation Grid page: PASS
- All 53 rendered pages have titles and descriptions: PASS
- Broken internal path links: 0
- Broken internal fragment anchors: 0
- Working tree after commit: clean
