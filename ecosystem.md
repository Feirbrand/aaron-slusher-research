# Research Ecosystem Map

Operating map for this repo and how it connects to the broader work.

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
│  Discovery layer — links to all repos                       │
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

## What Each Repo Holds

| Repo | Contains | Does not contain |
|---|---|---|
| `aaron-slusher-research` | Methodology papers, NF · EG · NAM · AA | VGS framework code, APP coaching content, F&F theology |
| `synoeticos-public` | AI-resilience frameworks, Synoetic OS, vgs-loadout, HF demos | Personal methodology papers |
| APP repo (future) | Athletic performance application work | — |
| F&F repo (future) | Faith formation content and research | — |

---

## The Broader Work

Three public brands, one underlying architecture.

**Achieve Peak Performance** — human performance coaching. Athletes, adaptive athletes, combat sports, neurotrauma, return-to-sport.

**ValorGrid Solutions** — applied AI resilience research. The mechanism is Tacit-to-Technical Transduction: practitioner pattern recognition extracted into publishable frameworks through a structured human-AI process.

**Foundations & Fire** — the intersection of formation science and faith.

In the background: a private R&D hardening layer that protects, tests, and extends the public architecture. Not public-facing.

---

## Publication Authority

| Paper type | Affiliation | Repo | DOI source |
|---|---|---|---|
| Methodology / formation architecture | Independent Researcher | `aaron-slusher-research` | Minted from this repo |
| AI-resilience / VGS technical | ValorGrid Solutions | `synoeticos-public` | Minted from that repo |
| APP coaching / field application | APP / Independent | APP repo (future) | Minted from APP repo |

---

## PUBLICATIONS.md Hierarchy

```
aaron-slusher-research/PUBLICATIONS.md    ← MASTER (the full cross-repo ledger)
  ├── synoeticos-public/PUBLICATIONS.md   ← self-contained (lists only VGS papers)
  └── APP repo/PUBLICATIONS.md            ← self-contained (lists only APP papers)
```

This repo is the hub. Its `PUBLICATIONS.md` is the only ledger that lists every paper across every repo, and it is the only place the ecosystem total is stated.

Each spoke repo keeps its own `PUBLICATIONS.md` listing only its own papers. A spoke ledger is self-contained: it does not reference this master, it does not reference another spoke, and it does not state the ecosystem total. The spoke counts itself; the hub counts everything. This map is maintained here, in the hub — spokes do not carry it.

---

## DOI Gate

A public folder in this repo earns its place only when:

1. Permanent Zenodo DOI is issued
2. Paper PDF + `CITATION.cff` + `README.md` exist in the folder
3. `PUBLICATIONS.md` is updated

No empty folders. No pre-announced content. Method overview pages may exist before DOI release when they describe the public stack.
