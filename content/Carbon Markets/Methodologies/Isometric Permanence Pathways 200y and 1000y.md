---
tags: [carbon-markets, isometric, permanence, quantification, reflectance]
aliases: [Isometric 200 year, Isometric 1000 year, Isometric Ro, Isometric permanence]
updated: 2026-09-16
---

# Isometric Permanence Pathways 200y and 1000y

**Parent hub:** [[Isometric Biochar Protocol]]  
**Modules:** [[Isometric Modules Soil Built Burial]]  
**Science:** [[Permanence Science for Credits]] · [[Woolf et al. 2021]] · [[Sanei et al. 2024]] · [[Permanence]]  
**Compare:** [[Verra VM0044 Permanence and Quantification]] · [[Puro CORC200+]] · [[CSI Global Biochar C-Sink]]

Primary source for soil equations: [Biochar Storage in Soil Environments v1.3](https://registry.isometric.com/module/biochar-storage-soil-environments/1.3). Protocol framing: [Biochar Production and Storage v1.3](https://registry.isometric.com/protocol/biochar/1.3). Launch rationale: [Isometric science article (2024-10-10)](https://isometric.com/writing-articles/certified-protocol-for-biochar-production-and-storage).

---

## Two soil crediting options

| Option | Durability label | Core inputs | Conservatism |
|---|---|---|---|
| **1** | **200 years** | H/Corg + mean annual **soil temperature** | ~17th percentile Woolf fit; \(F\) capped at **0.95**; soil T floor **7 °C** |
| **2** | **1,000 years** | Random reflectance **R₀ ≥ 2%** on **non-reactive C** | Mean − **1 SD** on both fractions; \(F\) capped at **0.95** |

Stored carbon:

\[
CO_2e_{stored} = C_{biochar} \times m_{biochar} \times F_{durable} \times \frac{44.01}{12.01}
\]

where \(C_{biochar} =\) Total C − \(C_{inorg}\) (only organic C credited).

Projects may combine both tiers under one validation **if** production batches are temporally and spatially separated with chain-of-custody — each batch under **exactly one** tier ([soil module](https://registry.isometric.com/module/biochar-storage-soil-environments/1.3)).

---

## Eligibility chemistry before either option

| Parameter | Threshold | Source |
|---|---|---|
| Molar **H/Corg** | **< 0.5** | Soil module Table 2 |
| Molar **O/Corg** | **< 0.2** | Soil module Table 2 |
| Heavy metals / PAH / PCDD/F / PCB | WBC upper bounds (module tables) | Soil module |
| Labs | **ISO 17025** or Isometric-agreed equivalent | Soil module |
| Samples | Prefer ≥ **3** per measured batch | Protocol §8.3 / module |

Contrast Verra soil gate **H:Corg ≤ 0.7** ([[Verra VM0044 Permanence and Quantification]]).

---

## Option 1 — 200-year (Woolf-conservative)

\[
F_{durable,200} = \min\Bigl(0.95,\; 1 - \bigl[c + (a + b \cdot \ln(T_{soil})) \cdot H/C_{org}\bigr]\Bigr)
\]

| Coefficient | Value |
|---|---|
| \(a\) | **-0.383** |
| \(b\) | **0.350** |
| \(c\) | **-0.048** |

Fit uses the **17th percentile** of the Woolf et al. (2021) durability distribution (~ one SD below the mean under normality assumptions) ([soil module Table 4](https://registry.isometric.com/module/biochar-storage-soil-environments/1.3); [Woolf DOI](https://doi.org/10.1021/acs.est.1c02425)).

### Soil temperature rules

- Prefer project-specific annual soil T baselining (ISO 4974 or equivalent); ≥ 10 measurements per site-month average narrative in module  
- Or justified value from global soil T datasets (e.g., Lembrechts et al. 2022)  
- **Air temperature may not proxy soil T** (module notes soil often 2–4 °C warmer)  
- If within-boundary soil T varies by **> 1 °C**, split project or use **highest** (most conservative) T  

### EU alignment note

Isometric’s science article links the 200-year option to the EU Carbon Removal Certification Framework “permanent removal” framing ([article](https://isometric.com/writing-articles/certified-protocol-for-biochar-production-and-storage)). Policy detail: vault EU CRCF references in [[Carbon Markets Hub]] / research report — do not invent delegated-act thresholds here.

---

## Option 2 — 1000-year (Ro / inertinite)

Science basis: [[Sanei et al. 2024]] ([DOI](https://doi.org/10.1016/j.coal.2023.104409)) — biochars with mean **R₀ ≥ 2%** structurally akin to inertinite macerals with geological persistence.

### Measurement requirements

| Requirement | Detail |
|---|---|
| Method | Random reflectance, e.g. ISO 7404-5:2009 |
| Density | ≥ **500** maceral-level R₀ measurements **per sample** |
| Replication | ≥ **3** samples; submit R₀ histogram at verification |
| Non-reactive C | Thermogravimetric residual organic C (Hawk / Rock-Eval-style re-pyrolysis then combustion) |
| Crediting math | \((\bar{R}_{pass} - s_{R}) \times (\bar{C}_{non\text{-}reactive} - s_{C})\) then min(0.95, max(0, ·)) |

Only the fraction passing the **2%** benchmark, applied to the **non-reactive** pool, is credited — reactive C is discounted.

### Comparison to CSI upper class

CSI Global Biochar C-Sink upper class uses higher Ro (**≥ 3.8%**) or HyPy ≥ 90% for **90% GPC** — different threshold and pool logic ([[CSI Global Biochar C-Sink]]). Isometric’s 2% inertinite benchmark is the Sanei et al. framing, not CSI’s 3.8% upper class.

---

## Buffer philosophy (soil)

Soil module projects are typically **No Observable Risk** → **0% buffer pool**, because labile decay is already discounted in \(F_{durable}\). Risk reassessed at crediting-period renewal ([soil module](https://registry.isometric.com/module/biochar-storage-soil-environments/1.3)).

Built-environment module uses a **2%** buffer under Very Low Risk framing ([[Isometric Modules Soil Built Burial]]).

---

## Non-soil horizons (pointer)

| Module | Horizon | Permanence approach |
|---|---|---|
| Low-oxygen burial | ≥ **1000y** | Ro paths ± incubation safety factor 3 |
| Built environment | **> 1000y** | Inertinite + labile × (1 − 3×F_reversal); asphalt labile 100% abraded |

Detail: [[Isometric Modules Soil Built Burial]].

---

## Intellectual map across standards

| Camp | Programs | Inputs |
|---|---|---|
| Decay-model / centuries | Isometric **200y**; Puro **CORC200+**; Verra **100y** Table 3 | H/Corg and/or temperature class, soil T |
| Inertinite / Ro millennial | Isometric **1000y**; CSI upper GPC | R₀, HyPy, non-reactive C |

Puro explicitly **encourages** Ro reporting but does **not yet quantify** with it ([[Puro CORC200+]]).

---

## Primary links

- [Soil module v1.3](https://registry.isometric.com/module/biochar-storage-soil-environments/1.3)
- [Protocol v1.3](https://registry.isometric.com/protocol/biochar/1.3)
- [Science article — two durability options](https://isometric.com/writing-articles/certified-protocol-for-biochar-production-and-storage)
- [Woolf et al. 2021](https://doi.org/10.1021/acs.est.1c02425)
- [Sanei et al. 2024](https://doi.org/10.1016/j.coal.2023.104409)

## Related notes

- [[Isometric Biochar Protocol]] · [[Isometric Project Cycle and MRV]] · [[Isometric Modules Soil Built Burial]]
- [[Verra VM0044 Permanence and Quantification]] · [[Puro CORC200+]] · [[Verra vs Isometric vs Puro]]
