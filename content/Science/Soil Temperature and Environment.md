---
tags: [science, permanence, soil, climate]
aliases: [Soil temperature permanence, Q10 biochar, Environmental controls on permanence]
updated: 2026-09-16
---

# Soil Temperature and Environment

Chapter on **environmental controls** on biochar carbon persistence—especially soil temperature (Q10), with notes on moisture, minerals, microbes, and aging. Complements material proxies in [[H-Corg and O-Corg]] and [[Reflectance Ro and HyPy]]. Report context: **2026-09-16**.

**Related notes:** [[Permanence]] · [[Woolf IPCC Fperm]] · [[Permanence Debates]] · [[CDR Potential and IPCC Accounting]] · [[Consensus vs Debates]] · [[Science Hub]] · [[Key Sources]]

---

## 1. Material × environment

Persistence is jointly controlled by **intrinsic chemistry** (aromatic condensation) and **extrinsic environment** (temperature, moisture, mineralogy, biology) ([[Biochar in Climate Change Mitigation|reviews biochar climate mitigation]] · [DOI](https://doi.org/10.1038/s41561-021-00852-8); [Schmidt et al. 2025](https://doi.org/10.1111/gcbb.70092)). A high-T wood char in cool temperate mineral soil will outlast the same chemistry in warm tropical soil on a 100-year \(F_\mathrm{perm}\) basis ([[Biochar Soil GHG Inventory Model|models soil GHG from biochar]] · [DOI](https://doi.org/10.1021/acs.est.1c02425)).

---

## 2. Temperature and Q10 (Woolf framework)

[[Biochar Soil GHG Inventory Model|models soil GHG from biochar]] rescale mineralization studies to a common soil temperature using a **temperature-dependent Q10**:

\[
Q_{10} = 1.1 + 12.0\,e^{-0.19\,T}
\]

after Lehmann et al. (2015) persistence chapter (cited in Woolf Methods) ([open PDF](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)).

**Reference climates in Woolf Table 3:**

| Reference | Mean annual T | Use |
|---|---|---|
| Global croplands | **14.9 °C** | Default headline \(F_\mathrm{perm}\) |
| US croplands | **10.9 °C** | Regional US inventories |
| Grid | 5, 10, 15, 20, 25 °C | Site-specific |

Example: high-T class, 100 years — \(F_\mathrm{perm}\) falls from **0.94** at 5 °C to **0.76** at 25 °C ([Table 3](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)). IPCC App. 4 instead embeds a conservative **~20 °C** basis into its single 100-yr table ([PDF](https://www.ipcc-nggip.iges.or.jp/public/2019rf/pdf/4_Volume4/19R_V4_Ch02_Ap4_Biochar.pdf)).

**Climate feedback:** future warming increases decay rates, so today’s \(F_\mathrm{perm}\) tables **overstate** permanence under warmer future soils if T is not updated ([[Consensus vs Debates]]; [Woolf 2021](https://doi.org/10.1021/acs.est.1c02425)).

---

## 3. Horizon length interacts with temperature

At fixed soil T, remaining fraction drops sharply from 100 → 500 → 1000 years (Woolf Table 3). At **14.9 °C**, high-T \(F_\mathrm{perm}\) ≈ **0.82 / 0.44 / 0.25** for those horizons ([open PDF](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)). Warm soil + long horizon is the most punishing combination for decay-model accounting—and the main quantitative reason “millennial permanence” claims need Ro/HyPy-style arguments or different system boundaries ([[Permanence Debates]], [[Reflectance Ro and HyPy]]).

---

## 4. Moisture, minerals, microbes, aging

Schmidt et al. (2025) emphasize that longevity is not chemistry alone: **soil mineralogy**, **biological activity**, and **climate** mediate both **decomposition** and **stabilization** (organo-mineral associations, aggregation with native OM) ([DOI](https://doi.org/10.1111/gcbb.70092)). Practical implications:

| Factor | Direction of effect (qualitative) | Evidence posture |
|---|---|---|
| Higher soil T | Faster mineralization → lower \(F_\mathrm{perm}\) | Quantified in Woolf Q10 |
| Mineral association / aggregation | Can stabilize pyrogenic C | Mechanistic / field aging literature; not in IPCC Tier-1 factor |
| Microbial community | Degrades labile pools first; slow attack on aromatics | Basis for multi-pool models |
| Moisture extremes | Can limit or enhance oxidation | Site-specific; sparse in inventory EFs |
| Organic soils / forest organic horizons | Risk of positive priming / out-of-scope | Woolf: **do not apply** method on Histosols or organic horizons ([DOI](https://doi.org/10.1021/acs.est.1c02425) §3.3) |

Priming of native SOC is conservatively **excluded** from Woolf’s GHG method because meta-mean negative priming was not significant at p<0.05 ([DOI](https://doi.org/10.1021/acs.est.1c02425); [[Stability and Priming Meta-analysis|meta-analyzes stability and priming]] · [DOI](https://doi.org/10.1111/gcbb.12266)).

---

## 5. Scope limits that are environmental

From IPCC App. 4 and Woolf:

- **In:** mineral soils, cropland/grassland applications of purpose-made pyrolysis/gasification biochar.
- **Out:** wetlands (IPCC), forest organic horizons, Histosols (Woolf conservative), wildfire/open-fire chars (IPCC), non-soil matrices (concrete, etc.—different permanence pathways; [[Materials and Built Uses]]).

---

## 6. Practice takeaway

1. Always attach **mean annual soil (or air-as-proxy) temperature** to \(F_\mathrm{perm}\).
2. Prefer Woolf Table 3 (or SI spreadsheet) over a single global factor for project MRV ([DOI](https://doi.org/10.1021/acs.est.1c02425)).
3. Do not apply mineral-soil permanence factors to organic soils.
4. Treat mineral stabilization as a **bonus narrative**, not an automatic uplift to inventory \(F_\mathrm{perm}\), unless a methodology explicitly allows it.

---

## Primary links

- [Woolf et al. 2021](https://doi.org/10.1021/acs.est.1c02425) · [open PDF](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content) · [[Biochar Soil GHG Inventory Model|models soil GHG from biochar]]
- [IPCC 2019 App. 4](https://www.ipcc-nggip.iges.or.jp/public/2019rf/pdf/4_Volume4/19R_V4_Ch02_Ap4_Biochar.pdf) · [[IPCC Biochar Soil Carbon Method|estimates soil C stock change from biochar]]
- [Schmidt et al. 2025](https://doi.org/10.1111/gcbb.70092)
- [Wang et al. 2016](https://doi.org/10.1111/gcbb.12266) · [[Stability and Priming Meta-analysis|meta-analyzes stability and priming]]

## Related notes

- [[Permanence]] · [[Woolf IPCC Fperm]] · [[Permanence Debates]] · [[Consensus vs Debates]] · [[GHG Fluxes]]
