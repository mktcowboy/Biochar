---
tags: [carbon-markets, methodology, verra, permanence, quantification]
aliases: [VM0044 permanence, VM0044 Table 3, Verra biochar permanence]
updated: 2026-09-16
---

# Verra VM0044 Permanence and Quantification

**Parent hub:** [[Verra VM0044]]  
**Eligibility rules:** [[Verra VM0044 Methodology and Eligibility]]  
**Science context:** [[Permanence Science for Credits]] · [[Permanence]] · [[Biochar Soil GHG Inventory Model|models soil GHG from biochar]] · [[IPCC Biochar Soil Carbon Method|estimates soil C stock change from biochar]]  
**Compare:** [[Isometric Permanence Pathways 200y and 1000y]] · [[Puro CORC200+]] · [[Verra vs Isometric vs Puro]]

This chapter covers **how much carbon is credited** and over what horizon under VM0044. Numbers below are taken from the public [VM0044 v1.1 PDF](https://verra.org/wp-content/uploads/2023/07/VM0044-Methodology-for-Biochar-Utilization-in-Soil-and-Non-Soil-Applications-v1.1.pdf) unless labeled otherwise. Active program version is **v1.2** ([methodology page](https://verra.org/methodologies/vm0044-biochar-utilization-in-soil-and-non-soil-applications-v1-2/)) — confirm Table 3 / equations unchanged in the live v1.2 PDF before locking a project model.

---

## Horizon claim

| Item | VM0044 (v1.1 PDF) | Peer contrast |
|---|---|---|
| Crediting permanence window | **100 years** | Puro **CORC200+** (several centuries); Isometric **200y** or **1000y** |
| Framing | “100-year permanence value … based on 100-year global warming potential horizon” | [[Puro CORC200+]] · [[Isometric Permanence Pathways 200y and 1000y]] |

Utilization must occur within **one year** of production so pre-application decay does not undermine the 100-year factor (v1.1 applicability).

---

## Core high-tech stored-carbon equation

For **Option P.1 — High Technology Production Facility** (v1.1 §8.2.2.1):

\[
CC_{t,k,y} = \sum_p \left( M_{t,k,p,y} \times FC_{p,t,p} \times PR_{de,k} \right)
\]

Then organic carbon is converted to CO₂e with the stoichiometric factor **44/12**.

| Symbol | Meaning |
|---|---|
| \(CC_{t,k,y}\) | Organic C (dry) for biochar type \(t\), application \(k\), year \(y\) (tonnes) |
| \(M_{t,k,p,y}\) | Dry mass of that biochar from facility \(p\) |
| \(FC_{p,t,p}\) | Organic carbon content (dry weight percent) — **lab analysis** for high-tech |
| \(PR_{de,k}\) | Permanence / decay adjustment factor for application type \(k\) |

Lab methods: latest **IBI Biochar Testing Guidelines** or **EBC Production Guidelines** or other internationally/nationally accredited standards (v1.1).

Net removals also subtract **project emissions** at production (pre-treatment, conversion, auxiliary energy) and account for leakage / transport per methodology tools — see [[Verra VM0044 Project Cycle and MRV]] and [[MRV Stack]].

---

## Table 3 — default \(PR_{de,k}\) for soil

**Table 3** (v1.1) provides default permanence adjustment factors drawn from **IPCC (2019)** Table 4AP.2 and [[Biochar Soil GHG Inventory Model|models soil GHG from biochar]] framing, keyed to **production temperature** \(T_{prod}\):

| Temperature class | Default \(PR_{de,k}\) |
|---|---|
| High temperature pyrolysis / gasification (**> 600 °C**) | **0.89** |
| Medium temperature pyrolysis (**450 – 600 °C**) | **0.80** |
| Low temperature (**350 – 450 °C**) | **0.65** |

Sources: [VM0044 v1.1 PDF](https://verra.org/wp-content/uploads/2023/07/VM0044-Methodology-for-Biochar-Utilization-in-Soil-and-Non-Soil-Applications-v1.1.pdf); [IPCC 2019 App. 4 PDF](https://www.ipcc-nggip.iges.or.jp/public/2019rf/pdf/4_Volume4/19R_V4_Ch02_Ap4_Biochar.pdf); [Woolf et al. 2021](https://doi.org/10.1021/acs.est.1c02425).

### Important clarification — Table 3 vs H:Corg

| Concept | Role in VM0044 v1.1 |
|---|---|
| **Table 3 \(PR_{de,k}\)** | **Temperature-class** default fraction of organic C treated as remaining over 100 years |
| **H:Corg ≤ 0.7** | **Soil eligibility gate** (aromaticity / quality), **not** the Table 3 lookup key |

Do not conflate with Isometric’s continuous H/Corg + soil-temperature decay function or CSI’s H/Corg ≤ 0.40 GPC split. Science map: [[Permanence Science for Credits]].

---

## Non-soil \(PR_{de,k}\)

If scientifically robust permanence information for the non-soil product is unavailable, use the **soil Table 3** default for the production temperature class (v1.1).

Project proponents **may propose** an alternate \(PR_{de,k}\) with evidence meeting VCS Methodology Requirements default-factor rules (peer-reviewed). If literature conflicts, adopt the **lower** value. White papers / non-peer-reviewed research are **not** accepted (v1.1).

Only **high-tech** biochar qualifies for non-soil pathways; biochar must be ≥ **50% C** dry weight ([[Verra VM0044 Methodology and Eligibility]]).

---

## Low-technology quantification path

Facilities that fail the four-condition high-tech definition use the **low-tech** option (v1.1):

- Organic carbon content may rely on **IPCC default tables/figures** (e.g., Table 4 / Figure 4Ap.1 themes in methodology) rather than full batch lab \(FC\)
- CH₄ / soot minimization must still be demonstrated (convection-zone kiln examples discussed in §8 narrative)
- Generally **less flexible / more conservative** than high-tech lab path

High-tech definition (recap): GHG recovery/combustion; ≥70% heat use; pollution controls; measured temperature — full text in [[Verra VM0044 Methodology and Eligibility]].

---

## Project emissions at production (high-tech sketch)

\[
PE_{PS,p,y} = (PE_{D,p,y} + PE_{P,p,y} + PE_{C,p,y}) \times \frac{\sum_t\sum_k M_{t,k,p,y}}{M_{p,y}}
\]

| Term | Meaning (v1.1) |
|---|---|
| \(PE_D\) | Pre-treatment of waste biomass (drying, pelletizing, etc.) |
| \(PE_P\) | Conversion / pyrolysis-related accounted emissions |
| \(PE_C\) | Auxiliary energy for pyrolysis |

Biogenic CO₂ from biomass is treated within the carbon-cycle framing of the methodology; **CH₄ and soot** remain material because of higher GWP (methodology narrative citing Amonette et al. 2021). High-tech condition (a) (combust/recover pyrolytic gases) underpins de minimis treatment of some direct process emission categories — see PDF footnotes.

Full boundary GHG table: v1.1 Table 2 (confirm in PDF).

---

## H:Corg eligibility vs other programs

| Program | Chemistry gate | Permanence model |
|---|---|---|
| **Verra VM0044** | Soil **H:Corg ≤ 0.7** | Table 3 **temperature** defaults @ 100y |
| **Isometric soil** | **H/Corg < 0.5**, **O/Corg < 0.2** | Woolf-style **200y** function **or** Ro≥2% **1000y** |
| **Puro Ed. 2025** | H/Corg domain in power model (see method) | **CORC200+** power decay + 80% CI |
| **CSI C-Sink 3.3** | H/Corg ≤0.40 → 75% GPC; Ro≥3.8% or HyPy≥90% → 90% GPC | GPC / SPC pools |

Sources: v1.1 PDF; [Isometric soil module](https://registry.isometric.com/module/biochar-storage-soil-environments/1.3); [[Puro Biochar Methodology Edition 2025]]; [[CSI Global Biochar C-Sink]].

---

## What VM0044 does **not** do (as of v1.x)

- Does **not** issue millennial **inertinite / Ro** credits like Isometric Option 2 or CSI upper GPC  
- Does **not** use soil temperature as a continuous decay input in Table 3 defaults  
- Does **not** (yet) make H/Corg the Table 3 lookup key — though **v2.0** consultation proposes enhanced H/Corg & moisture monitoring ([consultation](https://verra.org/consultation-major-revision-to-biochar-methodology-vm0044/))

---

## Worked intuition (illustrative only)

Suppose high-tech biochar, dry mass 1.0 t, lab organic C = 80%, produced at 650 °C → \(PR_{de}=0.89\):

\[
CC = 1.0 \times 0.80 \times 0.89 = 0.712\ \text{t C}
\]
\[
CO_2e\ \text{before PE/leakage} \approx 0.712 \times 44/12 \approx 2.61\ \text{tCO}_2e
\]

Then subtract project emissions, leakage, and apply any VCS buffer rules. **Do not use this as a credit quote** — it ignores PE, transport, application evidence, and verification findings.

---

## Science anchors

- [[IPCC Biochar Soil Carbon Method|estimates soil C stock change from biochar]] — temperature-class \(F_{perm}\) inventory guidance  
- [[Biochar Soil GHG Inventory Model|models soil GHG from biochar]] — [DOI](https://doi.org/10.1021/acs.est.1c02425)  
- [[Inertinite Permanence Benchmark|inertinite permanence benchmark]] — [DOI](https://doi.org/10.1016/j.coal.2023.104409) (used by Isometric/CSI, **not** VM0044 Table 3)  
- [[Permanence Science for Credits]] · [[Permanence]] · [[Consensus vs Debates]]

---

## Primary links

- [VM0044 v1.1 PDF (Table 3)](https://verra.org/wp-content/uploads/2023/07/VM0044-Methodology-for-Biochar-Utilization-in-Soil-and-Non-Soil-Applications-v1.1.pdf)
- [VM0044 v1.2 methodology page](https://verra.org/methodologies/vm0044-biochar-utilization-in-soil-and-non-soil-applications-v1-2/)
- [IPCC 2019 App. 4](https://www.ipcc-nggip.iges.or.jp/public/2019rf/pdf/4_Volume4/19R_V4_Ch02_Ap4_Biochar.pdf)
- [Woolf et al. 2021](https://doi.org/10.1021/acs.est.1c02425)
- [v2.0 consultation](https://verra.org/consultation-major-revision-to-biochar-methodology-vm0044/)

## Related notes

- [[Verra VM0044]] · [[Verra VM0044 Methodology and Eligibility]] · [[Verra VM0044 Project Cycle and MRV]]
- [[Isometric Permanence Pathways 200y and 1000y]] · [[Puro CORC200+]] · [[Verra vs Isometric vs Puro]]
