# Papers

This folder contains DOI-backed methodology papers by Aaron M. Slusher.

## DOI Gate Rule

A paper sub-folder is created here **only** when:
1. The paper has a permanent Zenodo DOI
2. The sub-folder contains a `README.md`, the paper PDF, and a `CITATION.cff`
3. `PUBLICATIONS.md` at the repo root has been updated

No placeholder folders. No pre-published content.

## Current Papers

| Paper | Folder | Status |
|---|---|---|
| Neuroformation v1.0 | `neuroformation/` | Pending migration from synoeticos-public |
| Elevation Grid v1.1 | `elevation-grid/` | Pending migration from synoeticos-public |
| Neural Access Method v1.0 | `neuro-access-method/` | **In preparation — NAM triggers repo going public** |

## Migration Protocol (for NF and EG)

When migrating papers from `synoeticos-public`:
1. **Do not delete** the original from synoeticos-public — leave it and its DOI path intact
2. Copy PDF + `CITATION.cff` into the sub-folder here
3. Add a `NOTICE.md` to the synoeticos-public location pointing to the canonical home here
4. Edit the Zenodo metadata (title, creators) to add `aaron-slusher-research` as a related identifier — this does not change the DOI
5. For future revisions, publish from this repo and mint a new version-DOI
