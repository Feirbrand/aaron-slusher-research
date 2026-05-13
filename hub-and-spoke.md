# Hub-and-Spoke Architecture Reference

Internal reference document. Not for public promotion — this is the operating map.

---

## Identity and Discovery Layers

```
┌─────────────────────────────────────────────────────────────┐
│  ORCID 0009-0000-9923-3207                                  │
│  Canonical academic identity — persistent, immutable        │
└──────────────────────┬──────────────────────────────────────┘
                       │
┌──────────────────────▼──────────────────────────────────────┐
│  aaronslusher.com                                           │
│  Human-facing hub — brand-agnostic, personal domain         │
└──────────────────────┬──────────────────────────────────────┘
                       │
┌──────────────────────▼──────────────────────────────────────┐
│  GitHub Profile README (Feirbrand)                          │
│  Discovery layer — mini-hub linking to all repos            │
└──────┬───────────────────────────────────┬──────────────────┘
       │                                   │
┌──────▼──────────────────┐   ┌────────────▼─────────────────┐
│  aaron-slusher-research │   │  synoeticos-public (VGS)     │
│  Personal methodology   │   │  Applied AI-resilience       │
│  hub — THIS REPO        │   │  technical ecosystem         │
│  NF · EG · NAM · AA     │   │  Synoetic OS · vgs-loadout   │
└─────────────────────────┘   └──────────────────────────────┘
```

---

## Spoke Ownership Rules

| Repo | Owner | What it contains | What it does NOT contain |
|---|---|---|---|
| `aaron-slusher-research` | Aaron M. Slusher, Independent Researcher | Methodology papers, NF/EG/NAM/AA, treatise track | VGS product infrastructure, APP coaching, FF theology, ASFA private |
| `synoeticos-public` | ValorGrid Solutions | AI-resilience frameworks, Synoetic OS, TTT, vgs-loadout, HF demos | Personal methodology papers, ASFA private |
| APP repo (future) | Aaron M. Slusher / APP | Athletic performance application lane | Owns no methodology — APP is field context, not method owner |
| ASFA (private) | Aaron M. Slusher | Private R&D substrate | Never public |

---

## Publication Authority

| Paper type | Author credit | Affiliation | Repo | Zenodo |
|---|---|---|---|---|
| Methodology / formation architecture | Aaron M. Slusher | Independent Researcher | `aaron-slusher-research` | Minted from this repo |
| AI-resilience / security / VGS technical | Aaron M. Slusher | ValorGrid Solutions | `synoeticos-public` | Minted from that repo |
| APP coaching / field application | Aaron M. Slusher | APP / Independent | APP repo (future) | Minted from APP repo |

**Rule:** Methodology papers belong under your name. APP is context, not owner. VGS is implementation lane.

---

## PUBLICATIONS.md Hierarchy

```
aaron-slusher-research/PUBLICATIONS.md    ← MASTER (all affiliations)
  └── synoeticos-public/publications.md  ← SUBSET (VGS-scoped, points up to master)
  └── APP repo/publications.md           ← SUBSET (APP-scoped, points up to master)
```

Edit the master. Treat subsets as views of the master, eventually automatable.

---

## DOI Gate

A public folder in `aaron-slusher-research` earns its place only when:
1. Permanent Zenodo DOI is issued
2. Paper PDF + `CITATION.cff` + `README.md` exist in the folder
3. `PUBLICATIONS.md` is updated

No empty sprawl. No pre-announced content.

---

## NAM Trigger Checklist

When the NAM paper is ready:

- [ ] NAM paper draft finalized
- [ ] Uploaded to Zenodo and DOI permanently minted
- [ ] `papers/neuro-access-method/` populated with PDF, `CITATION.cff`, `README.md`
- [ ] `methods/neuro-access-method/README.md` updated with real DOI and date
- [ ] `PUBLICATIONS.md` updated with real date and DOI
- [ ] GitHub release `v1.0.0-nam` cut (triggers Zenodo integration)
- [ ] `synoeticos-public/PUBLICATIONS.md` updated with cross-reference
- [ ] ORCID profile verified — both repo URLs listed under Websites
- [ ] Zenodo metadata for NF and EG updated to add `aaron-slusher-research` as related identifier
- [ ] Repo visibility changed from **private → public**
- [ ] GitHub Profile README pinned repos updated to include this repo
- [ ] aaronslusher.com/research pointed at GitHub Pages (if Pages is live)

---

## HTML Strategy

For this repo specifically:

| Format | Use |
|---|---|
| Markdown | Source of truth — papers, method READMEs, board notes, AI-to-AI workflow |
| HTML artifacts | Human-facing companion surfaces — explainers, interactive paper navigators, scorecards |
| PDF / Zenodo | Archival layer — permanent DOI record |

**Rule:** If your reader is a model or system, use Markdown. If your reader is a human exploring complex content, use HTML. Board notes stay Markdown always.

HTML artifacts live in `artifacts/` (to be created when Quarto migration is complete and first HTML companion is ready — do not create the folder empty).
