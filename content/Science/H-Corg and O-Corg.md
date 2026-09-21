---
tags: [science, permanence, elemental-ratios]
aliases: [H/Corg, O/Corg, H:Corg, O:Corg, Elemental ratio permanence]
updated: 2026-09-16
---

# H/C_org and O/C_org

Chapter on **molar hydrogen-to-organic-carbon** and **oxygen-to-organic-carbon** ratios as the primary chemical proxies for biochar aromatic condensation and soil persistence. Companion to [[Permanence]] · [[Woolf IPCC Fperm]] · [[Properties]]. Report context: **2026-09-16**.

**Related notes:** [[Reflectance Ro and HyPy]] · [[Biochar Quality from Process]] · [[Product Standards EBC IBI]] · [[Testing EBC IBI S668]] · [[Permanence Science for Credits]] · [[Biochar Lab Measurement Standard|standardizes biochar lab testing]] · [[Science Hub]] · [[Key Sources]]

---

## 1. Why elemental ratios track permanence

Pyrolysis drives condensation reactions that grow fused aromatic domains. As aromatic sheets enlarge, C–C bonds replace C–H and C–O bonds, so **H/C_org** and **O/C_org** fall ([[Keiluweit et al.|Keiluweit et al., 2010]] · [DOI](https://doi.org/10.1021/es9031419); [[Biochar Soil GHG Inventory Model|models soil GHG from biochar]] · [DOI](https://doi.org/10.1021/acs.est.1c02425)). Lower ratios therefore indicate a more condensed, typically more persistent solid—**relative** indicators, not absolute half-lives by themselves ([Schmidt et al., 2025](https://doi.org/10.1111/gcbb.70092)).

IUPAC’s biochar glossary frames biochar as a pyrolysis solid with molar **H/C_org < 0.7** and **O/C_org < 0.4** to ensure abundant fused aromatics and distinguish inadequately carbonized materials ([[IUPAC Biochar Terminology|IUPAC biochar terminology]] · [DOI](https://doi.org/10.1515/pac-2021-0106)).

---

## 2. Definitions and calculation

| Symbol | Meaning | Notes |
|---|---|---|
| **C_org** | Organic carbon mass fraction (dry basis) | Total C minus inorganic C (carbonates); see [[Biochar Lab Measurement Standard|standardizes biochar lab testing]] §9 · [PDF](https://biochar.org/wp-content/uploads/2026/05/ANSI-S668.pdf) |
| **H/C_org** (also H:C_org) | Moles H / moles C_org | Preferred condensation proxy in Woolf inventory model ([DOI](https://doi.org/10.1021/acs.est.1c02425)) |
| **O/C_org** (also O:C_org) | Moles O / moles C_org | Classic Spokas predictor ([DOI](https://doi.org/10.4155/cmt.10.32)); O often calculated by difference |

**ANSI/ASABE/USBI S668** formulas ([PDF](https://biochar.org/wp-content/uploads/2026/05/ANSI-S668.pdf) §10.1–10.2):

\[
\mathrm{H{:}C_{org}} = \frac{(\%\mathrm{H}/1.0079)}{(\%\mathrm{C_{org}}/12.011)}
\qquad
\mathrm{O{:}C_{org}} = \frac{(\%\mathrm{O}/15.999)}{(\%\mathrm{C_{org}}/12.011)}
\]

S668 notes that **high-ash** chars need care on oxygen (alternate calculation in §14.2)—important for manure/sludge/gasification residues ([[Gasification Residues]], [[Heavy Metals and Ash]]).

EBC accepts calculating O from C, H, N, S, and ash when direct O measurement is expensive ([EBC 10.5E PDF](https://www.european-biochar.org/media/doc/7/ebc_en_10_5_red.pdf) §7.3).

---

## 3. H/C_org as inventory input (Woolf)

[[Biochar Soil GHG Inventory Model|models soil GHG from biochar]] recommends **H/C_org over pyrolysis temperature** when elemental analysis is available, because H/C_org correlates more tightly with condensation (temperature alone ignores residence time and other process factors) ([DOI](https://doi.org/10.1021/acs.est.1c02425); [open PDF](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content) §3.2).

Permanence is fit as a linear regression:

\[
F_\mathrm{perm} = c_\mathrm{hc} - m_\mathrm{hc}\,(H/C_\mathrm{org})
\]

Coefficients \(c_\mathrm{hc}\), \(m_\mathrm{hc}\) depend on **soil temperature** and **time horizon** (Woolf Table 3). Example at **14.9 °C**, 100 years: \(c_\mathrm{hc}=1.04\), \(m_\mathrm{hc}=-0.64\), \(R^2=0.32\) ([open PDF](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content) Table 3). Full coefficient grid: [[Woolf IPCC Fperm]].

**Gasification** chars often combine high process temperature with **low H/C_org** despite low carbon fraction—persistence of the organic C can still be high even when FC is low ([Woolf 2021](https://doi.org/10.1021/acs.est.1c02425) §3.2; [[Gasification Residues]]).

---

## 4. O/C_org and Spokas half-life classes

[Spokas (2010)](https://doi.org/10.4155/cmt.10.32) reviewed biochar stability and proposed **O:C molar ratio** as a predictor of soil half-life. The review is foundational for standards language and practitioner rules-of-thumb; treat the binned half-lives as **approximate**, not inventory-grade alone ([[Quantitative Benchmarks]], science report framing).

Widely cited interpretive bins from that literature (cite Spokas DOI when using):

| Approx. O/C | Interpreted half-life class | Practice reading |
|---|---|---|
| **< ~0.2** | Millennial-scale | Highly condensed / high-T chars |
| **~0.2–0.6** | Centennial-scale | Typical mid-range pyrolysis |
| **> ~0.6** | Decadal / shorter | Incompletely carbonized / low-T |

Woolf argues **H/C_org is preferred over O/C_org** for high-ash materials because inorganic oxygen in ash confounds O/C more than H/C ([DOI](https://doi.org/10.1021/acs.est.1c02425) §3.2).

---

## 5. Product-standard gates (not credit methodologies)

| Framework | H/C_org | O/C_org | Source |
|---|---|---|---|
| **IUPAC glossary** | < **0.7** | < **0.4** | [[IUPAC Biochar Terminology|IUPAC biochar terminology]] · [DOI](https://doi.org/10.1515/pac-2021-0106) |
| **EBC all classes** | < **0.7** | should be < **0.4** | [EBC 10.5E](https://www.european-biochar.org/media/doc/7/ebc_en_10_5_red.pdf) §7.2–7.3 |
| **EBC-FeedPlus** | < **0.4** (proxy for ≥500 °C / ≥10 min) | — | Same PDF §10.4 |
| **EBC manure chars** | < **0.4** required | — | Same PDF §4.8 |
| **IBI Biochar Standards** | ≤ **0.7** classically required for “biochar” | often ≤ **0.4** | [IBI standards](https://biochar-international.org/biochar-standards/) · [[Product Standards EBC IBI]] |
| **NRCS CPS 336** | H:C_org **max 0.7** (practice eligibility) | — | [[Soil Carbon Amendment Standard|defines NRCS practice 336]] · [PDF](https://www.nrcs.usda.gov/sites/default/files/2022-11/336-NHCP-CPS-Soil-Carbon-Amendment-2022.pdf) |

Credit programs map these ratios into **different** permanence tables and horizons—do not copy thresholds here; see [[Permanence Science for Credits]].

---

## 6. Lehmann H/C_org < 0.5 subset (use with care)

[[Biochar in Climate Change Mitigation|reviews biochar climate mitigation]] is widely cited for: among biochars with **H/C_org < 0.5**, **95%** showed **>50%** C remaining after 100 years, with mean remaining ~**82%** in that subset ([DOI](https://doi.org/10.1038/s41561-021-00852-8)). The vault’s source note flags these figures as **not re-checked against the paywalled full text**—confirm before diligence use ([[Biochar in Climate Change Mitigation|reviews biochar climate mitigation]]). Abstract-checked claim that remains solid: persistence is **1–2 orders of magnitude** longer than source biomass ([same DOI](https://doi.org/10.1038/s41561-021-00852-8)).

---

## 7. Measurement pitfalls

- **Ash and inorganic C:** Always use **C_org**, not total C, in the denominator ([S668](https://biochar.org/wp-content/uploads/2026/05/ANSI-S668.pdf) §9–10).
- **Post-pyrolysis oxidation / additives:** EBC notes O/C_org can exceed 0.4 after oxidative post-treatment or co-pyrolysis with catalysts; CSI may grant exemptions after plausibility checks ([EBC 10.5E](https://www.european-biochar.org/media/doc/7/ebc_en_10_5_red.pdf) §7.3).
- **Lab method package:** Pair elemental analysis with contaminant and ag packages when selling soil products ([[Testing EBC IBI S668]]).
- **Process link:** Higher peak T and longer residence generally lower H/C_org ([[Pyrolysis Systems and Temperatures]], [[Biochar Quality from Process]]; [Keiluweit 2010](https://doi.org/10.1021/es9031419)).

---

## 8. Practice takeaway

1. Measure **H/C_org** (and report O/C_org) on every batch destined for CDR accounting or EBC/IBI labeling.
2. Use H/C_org → Woolf \(F_\mathrm{perm}\) when soil T and horizon are known ([[Woolf IPCC Fperm]]).
3. Treat Spokas O/C bins as **orientation**, not as Verra/Puro/Isometric factors.
4. For high-ash manure/sludge/gasification solids, prefer H/C_org and direct C_org measurement over default FC tables ([[Woody vs Manure Ag Feedstocks]], [[Gasification Residues]]).

---

## Primary links

- [Woolf et al. 2021](https://doi.org/10.1021/acs.est.1c02425) · [[Biochar Soil GHG Inventory Model|models soil GHG from biochar]]
- [Spokas 2010](https://doi.org/10.4155/cmt.10.32)
- [Keiluweit et al. 2010](https://doi.org/10.1021/es9031419)
- [Bilias et al. 2024](https://doi.org/10.1515/pac-2021-0106) · [[IUPAC Biochar Terminology|IUPAC biochar terminology]]
- [EBC 10.5E PDF](https://www.european-biochar.org/media/doc/7/ebc_en_10_5_red.pdf)
- [IBI Biochar Standards](https://biochar-international.org/biochar-standards/)
- [ANSI S668 PDF](https://biochar.org/wp-content/uploads/2026/05/ANSI-S668.pdf) · [[Biochar Lab Measurement Standard|standardizes biochar lab testing]]
- [Lehmann et al. 2021](https://doi.org/10.1038/s41561-021-00852-8) · [[Biochar in Climate Change Mitigation|reviews biochar climate mitigation]]

## Related notes

- [[Permanence]] · [[Woolf IPCC Fperm]] · [[Properties]] · [[Permanence Debates]] · [[Permanence Science for Credits]] · [[Science Hub]]
