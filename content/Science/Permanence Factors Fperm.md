---
tags: [science, permanence, accounting, IPCC]
aliases: [F_perm, Woolf Fperm, IPCC permanence factors, Permanence factors, Woolf IPCC Fperm]
updated: 2026-09-16
---

# Permanence Factors (F_perm)

Chapter on **inventory permanence factors**: how [[IPCC Biochar Soil Carbon Method|estimates soil C stock change from biochar]] and [[Biochar Soil GHG Inventory Model]] turn production temperature (or H/C_org) into the fraction of biochar organic carbon remaining after a chosen time. Credit methodologies that cite these tables are mapped in [[Permanence Science for Credits]]—this note stays on the **science/model**. Report context: **2026-09-16**.

**Related notes:** [[Permanence]] · [[H-Corg and O-Corg]] · [[Soil Temperature and Environment]] · [[CDR Potential and IPCC Accounting]] · [[Quantitative Benchmarks]] · [[Science Hub]] · [[Key Sources]]

---

## 1. What \(F_\mathrm{perm}\) is

\[
F_\mathrm{perm}(t,T_\mathrm{soil}) = \text{fraction of biochar organic C still unmineralized after time } t \text{ at soil temperature } T_\mathrm{soil}
\]

Both IPCC App. 4 and Woolf fit **multi-pool exponential decay** (minimum two-pool) to incubation and field datasets lasting **≥1 year**, then evaluate remaining C at policy-relevant horizons ([IPCC PDF](https://www.ipcc-nggip.iges.or.jp/public/2019rf/pdf/4_Volume4/19R_V4_Ch02_Ap4_Biochar.pdf); [Woolf DOI](https://doi.org/10.1021/acs.est.1c02425)).

**Do not mix IPCC and Woolf tables in one calculation**—Woolf re-derived factors with newer data and explicit soil-temperature adjustment; values differ ([[IPCC Biochar Soil Carbon Method|estimates soil C stock change from biochar]] “Use with care”).

---

## 2. Temperature classes (shared vocabulary)

| Class | Peak pyrolysis temperature | Notes |
|---|---|---|
| **Low** | **350–450 °C** | IPCC / Woolf bin |
| **Medium** | **450–600 °C** | |
| **High** | **≥600 °C** (IPCC also flags high-T gasification) | |

Materials below ~350 °C (torrefaction, typical HTC) are **out of scope** for these permanence tables ([Woolf 2021](https://doi.org/10.1021/acs.est.1c02425) §2.1.1; [IPCC definition](https://www.ipcc-nggip.iges.or.jp/public/2019rf/pdf/4_Volume4/19R_V4_Ch02_Ap4_Biochar.pdf)).

Process engineering context: [[Pyrolysis Systems and Temperatures]].

---

## 3. IPCC 2019 Appendix 4 (100-year factors)

Source: [[IPCC Biochar Soil Carbon Method|estimates soil C stock change from biochar]] · [PDF](https://www.ipcc-nggip.iges.or.jp/public/2019rf/pdf/4_Volume4/19R_V4_Ch02_Ap4_Biochar.pdf) (full text checked in vault).

| Production class | 100-yr \(F_\mathrm{perm}\) | Uncertainty |
|---|---|---|
| High (>600 °C) | **0.89** | ±**13%** |
| Medium (450–600 °C) | **0.80** | ±**11%** |
| Low (350–450 °C) | **0.65** | ±**15%** |

**Temperature basis:** factors adjusted to a conservative **~20 °C** ambient (against ~10 °C mean land-surface temperature in the appendix background). Scope: **mineral soils** in cropland/grassland only—not organic soils, forests with organic horizons, wetlands, or wildfire chars ([same PDF](https://www.ipcc-nggip.iges.or.jp/public/2019rf/pdf/4_Volume4/19R_V4_Ch02_Ap4_Biochar.pdf)). Status: basis for **future** Tier 1 development, not complete good-practice inventory guidance yet.

Carbon content \(F_{C_p}\) is tabulated separately by feedstock/process (Neves et al. regressions + ash correction)—see [[Production]], [[Woody vs Manure Ag Feedstocks]].

---

## 4. Biochar Soil GHG Inventory Model (Woolf et al. 2021, temperature- and H/C-resolved)

Source: [[Biochar Soil GHG Inventory Model]] · [DOI](https://doi.org/10.1021/acs.est.1c02425) · [open PDF](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content) (full text checked).

### 4.1 Headline 100-year values at global cropland mean (14.9 °C)

| Class | \(F_\mathrm{perm}\) (100 yr, 14.9 °C) |
|---|---|
| Low | **0.63** (SE 0.045) |
| Medium | **0.71** (SE 0.03) |
| High | **0.82** (SE 0.028) |

Abstract phrasing: **63–82%** of initial biochar C remains after 100 years at that temperature ([DOI](https://doi.org/10.1021/acs.est.1c02425)).

### 4.2 Longer horizons at 14.9 °C (Table 3)

| Horizon | Low | Medium | High |
|---|---|---|---|
| **500 yr** | 0.19 | 0.32 | 0.44 |
| **1000 yr** | **0.084** | **0.16** | **0.25** |

### 4.3 Soil-temperature sensitivity (100 yr, high class examples)

| Soil T (°C) | High-class \(F_\mathrm{perm}\) (100 yr) |
|---|---|
| 5 | **0.94** |
| 10 | **0.88** |
| 14.9 (global cropland mean) | **0.82** |
| 20 | **0.79** |
| 25 | **0.76** |

US cropland mean **10.9 °C** also tabulated (high 100-yr = **0.87**). Full grid: Woolf Table 3 ([open PDF](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)). Deep dive: [[Soil Temperature and Environment]].

### 4.4 H/C_org pathway

When H/C_org is measured, use Woolf eq. 5 with Table 3 regression coefficients rather than temperature bins ([[H-Corg and O-Corg]]). Preference order in Woolf §3.4: measured FC + H/C_org → else FC from Table 2 + T-class \(F_\mathrm{perm}\) → else **conservative low-T** \(F_\mathrm{perm}\).

### 4.5 Inventory equation (soil C term)

\[
\mathrm{GHG_{bc}} \approx \frac{44}{12}\,M_\mathrm{bc}\,F_C\,F_\mathrm{perm} \;+\; \text{(optional year-1 N₂O term)}
\]

([Woolf eq. 6](https://doi.org/10.1021/acs.est.1c02425)). Optional N₂O: **−23%** first year only, only if application **>10 Mg C ha⁻¹**—usually small vs C sequestration; not the focus of this permanence chapter ([[GHG Fluxes]]).

---

## 5. Why Woolf numbers are lower than IPCC’s

| Factor | IPCC App. 4 | Woolf 2021 (this model) |
|---|---|---|
| Dataset vintage | Pre-2019 appendix synthesis | Updated decay compilation |
| Climate basis | ~**20 °C** conservative | Explicit T grid; headline at **14.9 °C** |
| H/C_org option | Noted as future option | Fully parameterized |
| FC | Separate feedstock table | Table 2 by feedstock × T / gasification |

Using IPCC 0.89 with a Woolf-style cool-climate narrative (or vice versa) silently mis-states certainty. Pick **one** method stack and document it.

---

## 6. Worked intuition (from Woolf §3.4.1)

Maize stover pyrolysed at **500 °C** (medium), FC = **0.68** (Table 2), sequestered at **10 °C** soil → \(F_\mathrm{perm}=0.79\). With 15,000 Mg biochar + conditional N₂O term, Woolf’s example yields **29,710 Mg CO₂e** ([open PDF](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content) §3.4.1). Scale and boundaries matter for LCA vs inventory ([[CDR Potential and IPCC Accounting]]).

---

## 7. Link to carbon markets (pointer only)

Registries interpret these science tables differently (100y vs 200y vs 1000y; T-class vs H/C_org vs Ro). **Do not** paste methodology thresholds here—use [[Permanence Science for Credits]] · [[Verra VM0044 Permanence and Quantification]] · [[Isometric Permanence Pathways 200y and 1000y]] · [[Puro CORC200+]] · [[CSI Global Biochar C-Sink]].

---

## 8. Practice takeaway

1. Quote **horizon + soil T + method (IPCC vs Woolf)** every time you cite \(F_\mathrm{perm}\).
2. Prefer Woolf + H/C_org when lab data exist; IPCC T-class when only kiln temperature is known.
3. Remember 1000-year remaining fractions are **much lower** than 100-year ones at the same T ([Woolf Table 3](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content))—central to [[Permanence Debates]].

---

## Primary links

- [IPCC 2019 App. 4 PDF](https://www.ipcc-nggip.iges.or.jp/public/2019rf/pdf/4_Volume4/19R_V4_Ch02_Ap4_Biochar.pdf) · [[IPCC Biochar Soil Carbon Method|estimates soil C stock change from biochar]]
- [Woolf et al. 2021](https://doi.org/10.1021/acs.est.1c02425) · [open PDF](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content) · [[Biochar Soil GHG Inventory Model]]
- Supporting spreadsheet (Woolf SI): linked from [ACS page](https://doi.org/10.1021/acs.est.1c02425)

## Related notes

- [[Permanence]] · [[H-Corg and O-Corg]] · [[Soil Temperature and Environment]] · [[Permanence Debates]] · [[Permanence Science for Credits]] · [[Quantitative Benchmarks]]
