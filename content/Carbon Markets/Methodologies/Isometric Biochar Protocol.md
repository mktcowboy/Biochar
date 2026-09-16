---
tags: [carbon-markets, methodology, isometric, overview]
aliases: [Isometric, Isometric biochar, Isometric Overview]
updated: 2026-09-16
---

# Isometric Biochar Protocol

**Operator:** Isometric (registry + Certify platform)  
**Active biochar protocol:** **Biochar Production and Storage v1.3** ([registry](https://registry.isometric.com/protocol/biochar/1.3))  
**What it credits:** Ex-post **net CO₂e removal** = stored − counterfactual − lifecycle emissions  
**Minimum durability:** Project must provide storage **> 200 years**

This note is the **map of the Isometric biochar cluster**. Child notes hold permanence math, MRV cycle, and storage modules. Research dump: `/workspace/biochar-research/isometric-biochar-deep-dive.md` (2026-09-16).

Cross-standards: [[Verra vs Isometric vs Puro]] · [[Puro vs Other Standards]] · [[Verra VM0044]] · [[Puro.earth Overview]] · [[CSI Global Biochar C-Sink]].

---

## Why it matters for biochar

Isometric is a **modular CDR** program: one production/storage protocol plus specialized **soil**, **low-oxygen burial**, and **built-environment** modules (plus production variants for mobile / distributed / combustion co-product). It is currently the clearest mainstream path to **1000-year** biochar claims via **random reflectance (R₀)** / inertinite science ([[Sanei et al. 2024]]), while still offering a **200-year** Woolf-style path for projects without petrographic labs.

Registry positioning claim: “largest certifier of carbon removal by contracted volume”; “fully accredited by **ICVCM, ICROA, and CORSIA**” ([protocol page](https://registry.isometric.com/protocol/biochar/1.3)) — treat as operator claims; confirm category-level CCP status separately for diligence.

Related: [[Biochar as Durable CDR]] · [[Permanence Science for Credits]] · [[MRV Stack]] · [[Carbon Markets Hub]] · [[Materials and Built Uses]]

---

## Cluster map

| Note | Role |
|---|---|
| **[[Isometric Biochar Protocol]]** (this page) | Hub / architecture / net CDR equation |
| [[Isometric Permanence Pathways 200y and 1000y]] | Soil 200y vs Ro 1000y math |
| [[Isometric Project Cycle and MRV]] | PDD → V/V → ex-post issuance; CoC |
| [[Isometric Modules Soil Built Burial]] | Storage module applicability |
| [[Verra vs Isometric vs Puro]] | Decision chooser |

---

## Protocol architecture

```
Isometric Standard
        ↓
Biochar Production and Storage v1.3
        ├── Biomass Feedstock Accounting
        ├── GHG Accounting / Energy Use Accounting
        ├── Production modules (mobile / distributed / combustion co-product)
        └── Storage modules
                ├── Soil Environments v1.3  → 200y or 1000y
                ├── Low Oxygen Burial v1.1 → ≥1000y
                └── Built Environment v1.0+ → >1000y
```

Protocol cites ISO **14064-2:2019** and references ISO 14064-3, 14040/44. Literature review during development explicitly assessed Puro Edition 2025, Verra VM0044 v1.2, and CSI C-Sink standards ([protocol Sources](https://registry.isometric.com/protocol/biochar/1.3)).

Minimum review cadence: at least every **2 years** or when science/policy changes (protocol Future Versions).

---

## Net CDR equation

\[
CO_2e_{Removal,RP} = CO_2e_{Stored,RP} - CO_2e_{Counterfactual,RP} - CO_2e_{Emissions,RP}
\]

([protocol §8](https://registry.isometric.com/protocol/biochar/1.3))

| Term | Meaning |
|---|---|
| Stored | Durable organic C in biochar × mass × \(F_{durable}\) (module-specific) × 44.01/12.01 |
| Counterfactual | Biogenic C that would have remained durable without the project (Feedstock Accounting Module) |
| Emissions | Establishment + operations + end-of-life allocation + leakage |

**Issuance is ex-post** after durable storage ([protocol](https://registry.isometric.com/protocol/biochar/1.3); [science article](https://isometric.com/writing-articles/certified-protocol-for-biochar-production-and-storage)).

---

## Applicability gates (protocol)

Projects must:

1. Provide **net-negative** CO₂e impact per GHG Statement  
2. Meet ESS / no disproportionate harm to underserved communities  
3. Be **additional** (Isometric Standard; project-specific)  
4. Provide long-duration storage **> 200 years**

Ownership: single contractual Project Proponent for credits when multi-party supply chains exist — [[Double Counting and Credit Ownership]].

---

## Snapshot vs Verra / Puro

| Dimension | Isometric | Verra VM0044 | Puro Ed. 2025 |
|---|---|---|---|
| Horizon | **200y** / **1000y** | **100y** | **CORC200+** |
| Facility newness | Not greenfield-locked | **New** (v1.x) | New/Retrofit/Repurpose |
| Soil H/Corg gate | **< 0.5** (+ O/Corg < 0.2) | ≤ **0.7** | Model domain in method |
| Ro / inertinite | **Crediting path** | Not Table 3 basis | Encouraged, not quantifying |
| Buffer (soil) | Often **0%** | VCS risk tools | No default buffer |
| Public index | — | — | CORCCHAR/CORCX |

Detail: [[Verra vs Isometric vs Puro]].

---

## Notable projects (examples)

| Project | Notes | Source |
|---|---|---|
| **Charm Range & Plains Biochar** | Land application; issued certificates on registry; Fort Lupton CO | [registry](https://registry.isometric.com/project/prj_1JN6XNWDQ1S0BSN7) |
| **Carba Burnsville** | Landfill daily cover / low-oxygen; Microsoft **44,000** credits / 5 years | [registry](https://registry.isometric.com/project/prj_1JRZWM3BP1S071QG); [Carba press](https://carba.com/press/carba-announces-5-year-carbon-removal-credit-purchase-agreement-with-microsoft) |

---

## Primary links

- [Biochar Production and Storage v1.3](https://registry.isometric.com/protocol/biochar/1.3)
- [Soil Storage Module v1.3](https://registry.isometric.com/module/biochar-storage-soil-environments/1.3)
- [Low Oxygen Burial v1.1](https://registry.isometric.com/module/biochar-storage-low-oxygen/1.1)
- [Built Environment v1.0](https://registry.isometric.com/module/biochar-storage-built-environment/1.0)
- [Certified protocol article](https://isometric.com/writing-articles/certified-protocol-for-biochar-production-and-storage)
- [Built module article](https://isometric.com/writing-articles/a-new-module-for-storing-biochar-in-built-materials)
- [Woolf et al. 2021](https://doi.org/10.1021/acs.est.1c02425)
- [Sanei et al. 2024](https://doi.org/10.1016/j.coal.2023.104409)

## Related notes

- [[Isometric Permanence Pathways 200y and 1000y]] · [[Isometric Project Cycle and MRV]] · [[Isometric Modules Soil Built Burial]]
- [[Permanence Science for Credits]] · [[MRV Stack]] · [[Carbon Markets Hub]] · [[Key Sources]]
