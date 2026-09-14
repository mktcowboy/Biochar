---
tags: [applications, science, GHG, N2O, CH4, agriculture]
aliases: [N2O, methane, priming, Soil GHG]
updated: 2026-09-14
---

# GHG Fluxes

Agricultural framing of how soil-applied biochar changes **nitrous oxide (N₂O)**, **methane (CH₄)**, and **soil organic carbon priming / CO₂** fluxes. CDR credit math is still dominated by **stable biochar carbon** ([[Permanence]], [[Biochar as Durable CDR]]); flux co-benefits are secondary and highly variable.

Sibling notes: [[Soil and Agriculture]] · [[Crop Yield Effects]] · [[Application Rates and Methods]].

## Summary table

| Gas / process | Typical cited ranges | Caveats | Primary URL |
|---|---|---|---|
| **N₂O** | Classic meta ~**−54%** (Cayuela 2014); field-focused Jia 2023 **−26.8%**; Woolf inventory illustrative **−23%** year 1 only | Effect fades / uncertain beyond year 1; H:C_org matters | https://doi.org/10.1016/j.agee.2013.10.009 · https://doi.org/10.1002/ldr.4868 · https://doi.org/10.1021/acs.est.1c02425 |
| **CH₄** | Jia 2023 global **−13.0%**; paddies sometimes stronger ↓; other metas often ns overall | System-dependent (upland vs flooded) | https://doi.org/10.1002/ldr.4868 |
| **CO₂ / priming** | Short-term **positive priming** common; longer-term often **negative priming** (Wang 2016 mean SOC mineralization ~**−4%**; Weng 2017 decade-scale accrual) | Do **not** apply Woolf 2021 N₂O inventory method to organic/forest soils | https://doi.org/10.1111/gcbb.12266 · https://doi.org/10.1038/nclimate3276 · https://doi.org/10.1021/acs.est.1c02425 |
| **GWP (Jia 2023)** | Combined GWP **−7.7%** in that global analysis | Bundled metric; read paper for boundaries | https://doi.org/10.1002/ldr.4868 |

## N₂O — mechanisms and metas

### Classic and follow-on metas

Cayuela et al. (2014) reviewed and meta-analyzed soil N₂O responses and reported a large mean reduction (~**54%** in that analysis) ([DOI](https://doi.org/10.1016/j.agee.2013.10.009); author PDF mirror: https://digital.csic.es/bitstream/10261/273052/4/Cayuela2014AgricEcosysEnv.pdf).

Cayuela et al. (2015) show the **molar H:C_org** ratio is a key factor: more aromatic / lower H:C_org chars tend to mitigate N₂O more strongly ([DOI](https://doi.org/10.1016/j.agee.2014.12.015)). This is one scientific reason NRCS and EBC/IBI stress **H:C_org < 0.7** (and producers chase lower still) — see [[NRCS CPS 336 and US Ag]], [[Product Standards EBC IBI]], [[Properties]].

Mechanistic denitrification work (electron shuttling / buffering): Cayuela et al. (2013) *Scientific Reports* ([DOI](https://doi.org/10.1038/srep01732)).

### Field-oriented update

Jia et al. (2023) report global mean **N₂O −26.8%** under biochar application alongside yield and other GHG metrics ([DOI](https://doi.org/10.1002/ldr.4868)). Treat this as more conservative than the 2014 laboratory-heavy mean.

### Inventory / MRV conservatism (Woolf 2021)

Woolf et al. (2021) greenhouse-gas inventory method for biochar soil additions allows an **optional** N₂O adjustment of **−23%** for the **first year only**, and only when application exceeds **10 Mg C ha⁻¹**; they assume **no net CH₄ change** for inventory simplicity ([DOI](https://doi.org/10.1021/acs.est.1c02425)). Organic and forest soils are **out of scope** for that optional credit.

**Farm takeaway:** do not budget large multi-year N₂O offsets into agronomic NPV unless measured on-site. Credit programs primarily remunerate **durable C**, not flux co-benefits ([[MRV Stack]]).

## CH₄ — upland vs flooded systems

- Jia et al. (2023): mean **CH₄ −13.0%** ([DOI](https://doi.org/10.1002/ldr.4868)).
- Rice paddies and other anaerobic systems can show reductions in some East Asian metas cited in secondary literature, but responses remain **mixed** (increases or non-significant results appear in the wider corpus). Site hydrology, labile C, and iron redox chemistry matter.
- Woolf 2021 default: **no net CH₄ change** for national inventory–style accounting ([DOI](https://doi.org/10.1021/acs.est.1c02425)).

## Priming and SOC stocks

| Source | Finding | URL |
|---|---|---|
| Wang et al. 2016 | Decomposition + priming meta; mean SOC mineralization change ~**−4%** (negative priming on average) | https://doi.org/10.1111/gcbb.12266 |
| Weng et al. 2017 | Field evidence of **decade-scale negative priming** / SOC accrual | https://doi.org/10.1038/nclimate3276 |
| Jia et al. 2023 | Broader GHG + productivity synthesis including soil C interactions | https://doi.org/10.1002/ldr.4868 |

NRCS FAQ contrasts biochar’s multi-century C persistence framing (**~60–80%** remaining at 100 years in their cited range) with compost (**~2–14%**), while noting compost’s superior short-term nutrient/microbial pulse ([FAQ PDF](https://nrcs-prod.azureedge.us/sites/default/files/2026-04/soil-carbon-amendment-ac-336-faq.pdf)). Cross-check F_perm tables in [[Permanence]] / [[Quantitative Benchmarks]] ([IPCC 2019 appendix](https://www.ipcc-nggip.iges.or.jp/public/2019rf/pdf/4_Volume4/19R_V4_Ch02_Ap4_Biochar.pdf)).

## Interactions with rate, blends, and management

- **Rate:** Woolf’s optional N₂O inventory term only at **>10 Mg C ha⁻¹** year 1 — far above many CPS 336 planning rates (~4 yd³/ac baseline) ([Woolf](https://doi.org/10.1021/acs.est.1c02425); [NRCS FAQ](https://nrcs-prod.azureedge.us/sites/default/files/2026-04/soil-carbon-amendment-ac-336-faq.pdf)).
- **Compost / manure blends:** can change labile C, moisture, and N availability that drive N₂O — see [[Biochar Compost and Manure Blends]]; Earth Foundries Napa trial reported process GHG co-benefit as **VOC −33%** during composting with 10% biochar ([PDF](https://www.earthfoundriesinc.com/wp-content/uploads/2024/02/Earth-Foundries-Green-Compost-Biochar-Composting-Project-Report-2023.pdf)) — a **facility** emission metric, not soil N₂O.
- **Fertilizer N:** Ye et al. (2020) yield meta emphasizes fertilizer interactions ([PDF](https://www.css.cornell.edu/faculty/lehmann/publ/SoilUseManage%2036%2C%202-18%202020%20Ye.pdf)); N rate also modulates N₂O baselines.

## Real-world projects noting GHG / CDR co-benefits

These claim climate benefits primarily via **soil C storage**; flux claims should be read as supplementary:

- Exomad Green — Puro CORC soil end-use + stated N₂O co-benefit language on facility page: https://puro.earth/cdr-credit-suppliers/facilities/exomad-green-concepcion/
- Charm Range & Plains — Isometric soil land application: https://registry.isometric.com/project/prj_1JN6XNWDQ1S0BSN7
- Oasis Vineyard — cites Woolf 2021 persistence (>80% projected 100-yr for high-T wood char used): https://pacificbiochar.com/wp-content/uploads/Oasis-Vineyard-Trial_-5th-harvest_-Final-Draft_12.12.2023.pdf

Full project list: [[Real World Soil Projects]].

## Related notes

- [[Crop Yield Effects]] · [[Soil and Agriculture]] · [[Permanence]] · [[Consensus vs Debates]]
- [[Quantitative Benchmarks]] · [[Science Hub]] · [[Applications Hub]]
