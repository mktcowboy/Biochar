---
tags: [source, science, carbon-markets]
aliases: [Woolf 2021, Woolf et al. (2021), Woolf et al. 2021]
source_type: model
peer_reviewed: true
authors: ["Woolf, Dominic", "Lehmann, Johannes", "Ogle, Stephen", "Kishimoto-Mo, Ayaka W.", "McConkey, Brian", "Baldock, Jeffrey"]
year: 2021
title: "Greenhouse Gas Inventory Model for Biochar Additions to Soil"
venue: "Environmental Science & Technology 55(21): 14795–14805"
doi: "10.1021/acs.est.1c02425"
url: "https://doi.org/10.1021/acs.est.1c02425"
checked_against: full text
verified: 2026-09-14
---

# Biochar Soil GHG Inventory Model

**Citation:** Woolf D, Lehmann J, Ogle S, Kishimoto-Mo AW, McConkey B, Baldock J (2021). Greenhouse gas inventory model for biochar additions to soil. *Environmental Science & Technology* 55(21): 14795–14805. https://doi.org/10.1021/acs.est.1c02425 · open copy: [Canada federal science repository PDF](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)

**What it is:** A greenhouse-gas accounting method for biochar added to mineral soils. It extends the [[IPCC 2019 Biochar Appendix]] approach with soil temperature and H/C_org. It's the most-cited source in the vault: permanence tables, carbon-market methodologies, and N₂O accounting all lean on it.

## Key figures

| Figure | Value | Where | Check |
|---|---|---|---|
| Carbon content of biochar | From **7%** (gasified biosolids) to **79%** (wood pyrolysed above 600 °C) | [Abstract](https://doi.org/10.1021/acs.est.1c02425) | ✓ full text |
| Carbon fraction (FC) of wood biochar | Low / medium / high temperature **0.70 / 0.77 / 0.81**; mean **0.76**; gasification 0.63 | [Table 2 (open PDF)](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content) | ✓ full text |
| Temperature classes | Low 350–450 °C; medium 450–600 °C; high ≥600 °C | [§3.1 (open PDF)](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content) | ✓ full text |
| 100-year permanence factor (F_perm) at 14.9 °C, the global cropland mean | Low / medium / high **0.63 / 0.71 / 0.82**; this is the abstract's "63–82% remains after 100 years" | [Table 3 (open PDF)](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content) | ✓ full text |
| F_perm at 14.9 °C over longer horizons | 500 years: 0.19 / 0.32 / 0.44; 1,000 years: **0.084 / 0.16 / 0.25** | [Table 3](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content) | ✓ full text |
| F_perm vs soil temperature (100 years, high class) | 0.94 at 5 °C; 0.88 at 10 °C; 0.79 at 20 °C; 0.76 at 25 °C | [Table 3](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content) | ✓ full text |
| Temperature sensitivity used | Q10 = 1.1 + 12.0·e^(−0.19T) | [Methods](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content) | ✓ full text |
| N₂O adjustment | **−23%** (95% CI 5–41%), first year only, only where more than **10 Mg C ha⁻¹** is applied; fitted to field trials, with pot and incubation studies excluded | [§3.3.2](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content) | ✓ full text |
| Earlier N₂O meta-analyses it weighs | −54% ([[Cayuela et al. 2014]]), −12.4% (Verhoeven), −38% (Borchard); Verhoeven's reanalysis correcting for non-independent treatments gave −9.2%, not significant | [§3.3.2](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content) | ✓ full text |
| CH₄ | No effect assumed; too few field data to predict size or direction | [§2.4 and §3.5](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content) | ✓ full text |
| Priming of native soil carbon | Not credited, because net negative priming wasn't statistically significant in meta-analyses | [§3.3](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content) | ✓ full text |
| Where the method applies | Mineral soils only; not organic soils (Histosols) or forest soils with an organic horizon, where positive priming is possible | [§3.3](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content) | ✓ full text |
| Worked example | Maize stover pyrolysed at 500 °C: FC 0.68, F_perm 0.79 at 10 °C; 15,000 Mg biochar plus the N₂O term → **29,710 Mg CO₂e** | [§3.4.1](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content) | ✓ full text |

## Use with care

- The abstract's 79% carbon content and Table 2's FC of 0.81 for high-temperature wood aren't the same statistic. Quote the table when you need a class value.
- F_perm drops quickly in warmer soils and over longer horizons, so always state the temperature and time horizon with a permanence number.
- The N₂O term is small and conditional. Don't apply it at typical farm rates below 10 Mg C ha⁻¹.

Related: [[Permanence]] · [[Woolf IPCC Fperm]] · [[H-Corg and O-Corg]] · [[Soil Temperature and Environment]] · [[IPCC 2019 Biochar Appendix]] · [[GHG Fluxes]] · [[Permanence Science for Credits]] · [[Key Sources]]
