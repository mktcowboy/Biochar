---
tags: [science, permanence, hub]
aliases: [Persistence, Biochar permanence, Permanence hub]
updated: 2026-09-16
---

# Permanence

Hub for **persistence / permanence science**: how long biochar organic carbon remains in soil after application, which material and environmental factors control that longevity, and which laboratory proxies inventories and markets use. Credit-program thresholds and issuance rules live in [[Permanence Science for Credits]] — this cluster stays on the **science**. Report context: **2026-09-16**.

> **Companion chapters (2026-09-16):** [[H-Corg and O-Corg]] · [[Permanence Factors Fperm|inventory permanence factors]] · [[Reflectance Ro and HyPy]] · [[Soil Temperature and Environment]] · [[Permanence Debates]]. This note is the **spine**—definitions, mechanism snapshot, chapter map, and practice takeaway—without duplicating registry methodology text.

**Related notes:** [[Properties]] · [[Quantitative Benchmarks]] · [[CDR Potential and IPCC Accounting]] · [[Consensus vs Debates]] · [[Permanence Science for Credits]] · [[Production]] · [[Biochar Quality from Process]] · [[Science Hub]] · [[Key Sources]]

---

## 1. What “permanence” means here

Biochar carbon mineralizes **1–2 orders of magnitude more slowly** than unpyrolysed biomass because pyrolysis builds **fused aromatic** structures that microbes oxidize poorly ([[Biochar in Climate Change Mitigation|reviews biochar climate mitigation]] · [DOI](https://doi.org/10.1038/s41561-021-00852-8); [[Biochar Soil GHG Inventory Model|models soil GHG from biochar]] · [DOI](https://doi.org/10.1021/acs.est.1c02425)). Persistence is **not** literal forever: it is probabilistic over **centennial–millennial** horizons for well-made chars, and it depends on **material chemistry** (aromatic condensation) **and** environment (soil temperature, moisture, minerals, microbes) ([Schmidt et al., 2025](https://doi.org/10.1111/gcbb.70092); [Woolf 2021](https://doi.org/10.1021/acs.est.1c02425)).

Policy and inventory practice usually compress that dynamics into a single **permanence factor** \(F_\mathrm{perm}\) = fraction of biochar organic C still unmineralized after a chosen horizon—commonly **100 years** for IPCC-style accounting ([[IPCC Biochar Soil Carbon Method|estimates soil C stock change from biochar]] · [PDF](https://www.ipcc-nggip.iges.or.jp/public/2019rf/pdf/4_Volume4/19R_V4_Ch02_Ap4_Biochar.pdf)). Always state **horizon + soil temperature** with any \(F_\mathrm{perm}\) number ([[Permanence Factors Fperm|inventory permanence factors]], [[Soil Temperature and Environment]]).

---

## 2. Mechanism in one paragraph

During pyrolysis, cellulose/hemicellulose/lignin rearrange into **condensed aromatic** domains; H and O are lost relative to C, so **H/C_org** and **O/C_org** fall as condensation rises ([[Biochar Structure vs Charring Temperature|maps structure vs charring temperature]] · [DOI](https://doi.org/10.1021/es9031419); [[H-Corg and O-Corg]]). Labile aliphatic / incompletely carbonized fractions mineralize in months–years; the recalcitrant aromatic pool decays much more slowly, so multi-pool (at least two-pool exponential) models are the inventory workhorse ([IPCC App. 4](https://www.ipcc-nggip.iges.or.jp/public/2019rf/pdf/4_Volume4/19R_V4_Ch02_Ap4_Biochar.pdf); [Woolf 2021](https://doi.org/10.1021/acs.est.1c02425)). Aging in soil also includes **stabilization** pathways (organo-mineral associations, aggregation)—decomposition and stabilization run in parallel ([Schmidt 2025](https://doi.org/10.1111/gcbb.70092)).

---

## 3. Proxy map (science side)

| Proxy | What it tracks | Typical use | Deep chapter |
|---|---|---|---|
| **H/C_org** | Aromatic condensation (H lost as fused rings grow) | Preferred inventory input when measured; EBC/IBI quality gate | [[H-Corg and O-Corg]] |
| **O/C_org** | Oxygenation / condensation (Spokas half-life classes) | Historical rule-of-thumb; standards often ≤0.4 | [[H-Corg and O-Corg]] |
| **Pyrolysis T class** | Process intensity when elemental analysis unavailable | IPCC / Woolf temperature bins → \(F_\mathrm{perm}\) | [[Permanence Factors Fperm|inventory permanence factors]] · [[Pyrolysis Systems and Temperatures]] |
| **BC_HyPy** | Hydropyrolysis-resistant C | CSI / advanced MRV “inert” fraction | [[Reflectance Ro and HyPy]] |
| **Random reflectance Ro** | Optical rank / inertinite-like condensation | Isometric 1000y / CSI upper class / Sanei benchmark | [[Reflectance Ro and HyPy]] |
| **Solid EC** | Batch homogeneity / condensation correlate (EBC) | Process QC, not a standalone \(F_\mathrm{perm}\) | [[Properties]] · EBC Guidelines ([PDF](https://www.european-biochar.org/media/doc/7/ebc_en_10_5_red.pdf)) |
| **Soil temperature** | Environmental decay rate (Q10) | Adjust \(F_\mathrm{perm}\) to site climate | [[Soil Temperature and Environment]] |

Test-method recipes (how to measure H:C_org, O:C_org, Ro): [[Biochar Lab Measurement Standard|standardizes biochar lab testing]] · [PDF](https://biochar.org/wp-content/uploads/2026/05/ANSI-S668.pdf) §10. Pass/fail credit thresholds: [[Permanence Science for Credits]].

---

## 4. Headline numbers (checked vault sources)

| Source | Finding | Link |
|---|---|---|
| **[IPCC 2019 App. 4](https://www.ipcc-nggip.iges.or.jp/public/2019rf/pdf/4_Volume4/19R_V4_Ch02_Ap4_Biochar.pdf)** · [[IPCC Biochar Soil Carbon Method|estimates soil C stock change from biochar]] | 100-yr \(F_\mathrm{perm}\): **0.65** (350–450 °C), **0.80** (450–600 °C), **0.89** (>600 °C); ±~11–15%; ~20 °C basis | Full text ✓ |
| **[[Biochar Soil GHG Inventory Model|models soil GHG from biochar]]** ([DOI](https://doi.org/10.1021/acs.est.1c02425); [open PDF](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)) | At **14.9 °C** (global cropland mean): 100-yr ≈ **0.63 / 0.71 / 0.82**; 1000-yr high-T ~**0.25** | Full text ✓ |
| **[[Biochar in Climate Change Mitigation|reviews biochar climate mitigation]]** ([DOI](https://doi.org/10.1038/s41561-021-00852-8)) | Of chars with **H/C_org < 0.5**, 95% showed >50% C remaining after 100 yr (mean **~82%** in that subset) | Full-text figure **not re-checked** (paywalled)—use with care |
| **[Spokas 2010](https://doi.org/10.4155/cmt.10.32)** | O/C half-life classes (approximate; not inventory-grade alone) | See [[H-Corg and O-Corg]] |
| **[[Inertinite Permanence Benchmark|inertinite permanence benchmark]]** ([DOI](https://doi.org/10.1016/j.coal.2023.104409)) | Inertinite benchmark **Ro = 2%** (IBRo2%); 76% of studied commercial chars entirely above 2% | Abstract ✓ |
| **[Schmidt et al. 2025](https://doi.org/10.1111/gcbb.70092)** | Policy: estimate persistence on **centuries**, not millennia; refuse 100% permanence claims | Abstract ✓ |

Cross-sheet: [[Quantitative Benchmarks]].

---

## 5. Practice takeaway (science → project)

1. Prefer **measured H/C_org + site soil temperature** for \(F_\mathrm{perm}\) when elemental analysis is available ([Woolf 2021](https://doi.org/10.1021/acs.est.1c02425)).
2. Fall back to **IPCC / Woolf temperature class** when only production logs exist ([IPCC PDF](https://www.ipcc-nggip.iges.or.jp/public/2019rf/pdf/4_Volume4/19R_V4_Ch02_Ap4_Biochar.pdf)).
3. Do **not** claim “permanent” without a **time horizon** (usually 100 years in inventory policy; credit programs may use 200y / 1000y / “several centuries”—see [[Permanence Science for Credits]]).
4. Treat **Ro / HyPy** as complementary high-condensation indicators, not drop-in replacements for Woolf-style decay factors, unless a specific protocol says otherwise ([[Reflectance Ro and HyPy]], [[Permanence Debates]]).
5. Warmer soils **lower** \(F_\mathrm{perm}\) for the same char ([[Soil Temperature and Environment]]).

---

## 6. Chapter index

| Chapter | Role |
|---|---|
| [[H-Corg and O-Corg]] | Elemental-ratio proxies, Spokas classes, EBC/IBI gates, Woolf H/C regression |
| [[Permanence Factors Fperm|inventory permanence factors]] | Temperature bins, Table 3 values, how IPCC and Woolf relate (do not mix tables) |
| [[Reflectance Ro and HyPy]] | Petrographic Ro, hydropyrolysis-resistant C, inertinite debate pointer |
| [[Soil Temperature and Environment]] | Q10, cropland means, moisture/minerals/aging |
| [[Permanence Debates]] | Two-pool overestimation, Ro vs decay-model camps, policy commentary |

---

## 7. Primary links

- [IPCC 2019 App. 4 PDF](https://www.ipcc-nggip.iges.or.jp/public/2019rf/pdf/4_Volume4/19R_V4_Ch02_Ap4_Biochar.pdf) · [[IPCC Biochar Soil Carbon Method|estimates soil C stock change from biochar]]
- [Woolf et al. 2021](https://doi.org/10.1021/acs.est.1c02425) · [open PDF](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content) · [[Biochar Soil GHG Inventory Model|models soil GHG from biochar]]
- [Lehmann et al. 2021](https://doi.org/10.1038/s41561-021-00852-8) · [[Biochar in Climate Change Mitigation|reviews biochar climate mitigation]]
- [Schmidt et al. 2025](https://doi.org/10.1111/gcbb.70092)
- [Sanei et al. 2024](https://doi.org/10.1016/j.coal.2023.104409) · [[Inertinite Permanence Benchmark|inertinite permanence benchmark]]
- [Spokas 2010](https://doi.org/10.4155/cmt.10.32)
- [Keiluweit et al. 2010](https://doi.org/10.1021/es9031419)
- [EBC Guidelines 10.5E PDF](https://www.european-biochar.org/media/doc/7/ebc_en_10_5_red.pdf)
- [ANSI S668 PDF](https://biochar.org/wp-content/uploads/2026/05/ANSI-S668.pdf) · [[Biochar Lab Measurement Standard|standardizes biochar lab testing]]
- Credit interpretation (no method duplication): [[Permanence Science for Credits]]

## Related hubs

- [[Science Hub]] · [[Production Hub]] · [[Carbon Markets Hub]] · [[Biochar Home]] · [[Key Sources]]
