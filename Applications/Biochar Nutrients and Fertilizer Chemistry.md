---
tags: [applications, nutrients, fertilizer, chemistry, NPK, CEC, BBF, soil]
aliases: [Biochar nutrients, Fertilizer chemistry, Biochar NPK, Biochar-based fertilizer chemistry]
updated: 2026-09-14
---

# Biochar Nutrients and Fertilizer Chemistry

Chapter-length note on **how biochar interacts with plant nutrients**—N (NH₄⁺ / NO₃⁻ / immobilization / volatilization), P, K, Ca/Mg, micronutrients, liming/pH—and how that chemistry drives **inoculation, charging, and biochar-based fertilizers (BBF/BCF)**. Report context: **2026-09-14**.

**Hard rule:** every quantitative or named claim below carries an outbound URL or DOI. Companion dump: `/workspace/biochar-research/biochar-nutrients.md`. Practice/protocol depth for charging lives in [[Biochar Inoculation for Fertilizer]]—this chapter is the **nutrient-chemistry spine**; cross-link heavily, do not duplicate that entire chapter.

**Related notes:** [[Biochar Inoculation for Fertilizer]] · [[Biochar Microbes and Soil Biology]] · [[Biochar Compost and Manure Blends]] · [[Soil and Agriculture]] · [[Crop Yield Effects]] · [[GHG Fluxes]] · [[Application Rates and Methods]] · [[Agronomic Economics]] · [[Properties]] · [[Contaminants and Quality]] · [[Product Standards EBC IBI]] · [[NRCS CPS 336 and US Ag]] · [[Applications Hub]] · [[Key Sources]]

---

## 1. Purpose and problem statement

Woody biochars used for durable carbon are typically **nutrient-poor**, porous, and surface-reactive. Applied raw, they can **sorb plant-available nutrients** from soil solution and, especially in the first weeks to months, contribute to **temporary inorganic-N decline** and yield drag. Nguyen et al. (2017) meta-analyzed 56 studies (1080 cases) and found mean reductions of roughly **−11 ± 2% NH₄⁺-N** and **−10 ± 1.6% NO₃⁻-N**, with 95% of observations within one year of application ([DOI](https://doi.org/10.1016/j.geoderma.2016.11.004)). USDA NRCS states that fresh biochar “has a chance to reduce crop yields by binding and immobilizing nutrients” and recommends charging with compost or manure ([CPS 336 FAQ, Apr 2026](https://nrcs-prod.azureedge.us/sites/default/files/2026-04/soil-carbon-amendment-ac-336-faq.pdf)); CPS 336 requires inoculating biochar with compost, compost tea, or manure ([2022 PDF](https://www.nrcs.usda.gov/sites/default/files/2022-11/336-NHCP-CPS-Soil-Carbon-Amendment-2022.pdf)).

USBI (American Biochar Institute) agricultural guidelines treat charging / inoculating / activating as post-processing that fills surface functional groups with nutrients and microbes, calling inoculation **critical** to minimize first-year immobilization ([USBI Ag Guidelines](https://farmlandinfo.org/wp-content/uploads/sites/2/2023/06/usbi-biochar-guidelines-for-ag-application.pdf)).

The controlled contrast that frames this chemistry for practitioners: Kammann et al. (2015) showed **2% (w/w) untreated** high-temperature wood biochar reduced quinoa aboveground biomass to **~60% of control**, while the **same rate of co-composted** biochar increased biomass by up to **~305%**, with captured **nitrate and phosphate** as central mechanisms ([DOI](https://doi.org/10.1038/srep11080); [PMC4460888](https://pmc.ncbi.nlm.nih.gov/articles/PMC4460888/)).

This chapter answers: *what does biochar do to each nutrient pool, how does aging/enrichment change that, and how do BBF formulations and fertilizer co-management convert chemistry into fertilizer-use efficiency?*

---

## 2. Conceptual map — ash nutrients vs organic C matrix

| Component | What it delivers | What it does to nutrients | Primary sources |
|---|---|---|---|
| **Ash / mineral fraction** | K, Ca, Mg, Na, P (feedstock-dependent); liming bases (carbonates, oxides) | Immediate base cation supply; raises pH/EC; can precipitate P with Ca/Mg/Fe/Al | Ippolito et al. 2020 meta ([DOI](https://doi.org/10.1007/s42773-020-00067-x)); NRCS FAQ wood vs manure contrast ([PDF](https://nrcs-prod.azureedge.us/sites/default/files/2026-04/soil-carbon-amendment-ac-336-faq.pdf)); NPK cycle review ([DOI](https://doi.org/10.1186/s40538-020-00182-8)) |
| **Organic C matrix** | Condensed aromatic C; labile residual C (esp. low-T); surface functional groups | Sorption / desorption; CEC evolution with aging; habitat & priming | Keiluweit-type chemistry lineage via [[Properties]]; Nguyen 2017 ([DOI](https://doi.org/10.1016/j.geoderma.2016.11.004)); Cheng et al. 2008 oxidation ([DOI](https://doi.org/10.1016/j.gca.2008.01.010)) |
| **Organic coating (co-compost / field aging)** | DOC, nitrate, phosphate, Ca/K hotspots on patchy surfaces | Non-conventional anion retention; slow release; fertility stimulation without bulk aromatic change | Hagemann et al. 2017 *Nat. Commun.* ([DOI](https://doi.org/10.1038/s41467-017-01123-0)); Archanjo et al. 2017 ([DOI](https://doi.org/10.1016/j.geoderma.2017.01.038)); Joseph et al. 2018 ([DOI](https://doi.org/10.1016/j.scitotenv.2017.09.200)) |
| **Engineered enrichment (BBF)** | Added NPK, clays, Mg, struvite, urine, digestate, microbes | Designed slow-release; lower agronomic rates | Ndoung et al. 2021 ([DOI](https://doi.org/10.1016/j.heliyon.2021.e08473)); Melo et al. 2022 ([DOI](https://doi.org/10.1007/s11104-021-05276-2)) |

**Practice takeaway:** high-C wood chars are mostly a **C matrix + sponge**; manure/bone chars are partly **ash fertilizers**. Enrichment / co-composting adds the **coating + nutrient payload** that turns sponge into slow-release carrier ([[Biochar Inoculation for Fertilizer]]).

---

## 3. Nitrogen chemistry in detail

### 3.1 Forms and pathways

Clough et al. (2013) review biochar–soil N dynamics across sorption, immobilization, nitrification, denitrification, fixation, and plant uptake ([DOI](https://doi.org/10.3390/agronomy3020275)). Nguyen et al. (2017) organize abiotic vs biotic pathways that jointly determine soil inorganic N (SIN) after amendment ([DOI](https://doi.org/10.1016/j.geoderma.2016.11.004)).

| Pathway | Direction for plant-available N | Mechanism sketch | Sources |
|---|---|---|---|
| **NH₄⁺ electrostatic sorption (CEC)** | Temporary ↓ in solution; later desorption possible | Carboxyl/phenolic acid groups; increases with aging/oxidation | Nguyen 2017; Cheng 2008 ([DOI](https://doi.org/10.1016/j.gca.2008.01.010)) |
| **NH₃ chemisorption / covalent retention** | Stored N; can remain plant-bioavailable | Fire-derived OM covalent ammonia bonding; urine-NH₃ capture | Hestrin et al. 2019 ([DOI](https://doi.org/10.1038/s41467-019-08401-z)); Taghizadeh-Toosi et al. 2012 ([DOI](https://doi.org/10.1007/s11104-011-0870-3)); urine NH₃ capture ([DOI](https://doi.org/10.1007/s11104-011-1010-9)) |
| **NO₃⁻ unconventional retention** | ↓ leaching; partial plant availability; under-detected by standard extracts | H-bonding / micropore ion–water interactions; organic coatings | Kammann 2015 ([DOI](https://doi.org/10.1038/srep11080)); Hagemann 2017 PLOS ([DOI](https://doi.org/10.1371/journal.pone.0171214)); Conte/H-bonding discussion in Kammann paper |
| **Microbial immobilization** | Short-term ↓ SIN | Labile C fuels microbes that compete for NH₄⁺/NO₃⁻ | Bruun et al. 2012 ([DOI](https://doi.org/10.1016/j.soilbio.2011.11.019)); Cross & Sohi 2011 ([DOI](https://doi.org/10.1016/j.soilbio.2011.06.016)) |
| **Nitrification / denitrification shifts** | Form conversion; N₂O implications | Liming, aeration, nosZ; H:C_org moderates N₂O | Clough 2013; Cayuela N₂O metas in [[GHG Fluxes]] |
| **NH₃ volatilization** | Loss risk when pH rises | Alkaline ash liming + NH₄⁺ sources | Clough 2013; Nguyen discussion of coarse acidic soils |

### 3.2 Meta-analytic magnitude (do not universalize)

| Finding | Figure | Source |
|---|---|---|
| Mean NH₄⁺-N change | **−11 ± 2%** | https://doi.org/10.1016/j.geoderma.2016.11.004 |
| Mean NO₃⁻-N change | **−10 ± 1.6%** | same |
| Hydrochar NH₄⁺-N | **−46 ± 7%** | same |
| Strongest NH₄⁺ drop timing | Within ~**1 month** after application | same — authors suggest apply ≥1 month before planting |
| Long-term (>1 y) evidence | Sparse in that meta (few cases) | same |

Woody biochars reduced SIN **less** than carbohydrate/herbaceous chars in that meta—consistent with lower labile C and often lower CEC—while still capable of physisorption at high BET ([DOI](https://doi.org/10.1016/j.geoderma.2016.11.004)).

### 3.3 Fertilizer-type interactions (Nguyen 2017)

- Biochar **+ NH₄-based** fertilizers: NH₄⁺-N decreased vs biochar with no fertilizer.
- Biochar **+ organic fertilizer**: SIN increased vs biochar alone (organic N mineralization offsets immobilization).
- Biochar **+ urea**: NO₃⁻-N often increased (nitrification of urea-N).
- Biochar **alone (unfertilized)**: significant NO₃⁻-N reduction (sorption + immobilization).

This is the chemical rationale for NRCS/USBI **charge-with-organics** guidance ([FAQ](https://nrcs-prod.azureedge.us/sites/default/files/2026-04/soil-carbon-amendment-ac-336-faq.pdf); [USBI](https://farmlandinfo.org/wp-content/uploads/sites/2/2023/06/usbi-biochar-guidelines-for-ag-application.pdf)).

### 3.4 Nitrate capture in co-composted particles (quantitative)

Kammann et al. (2015) and Hagemann et al. (2017 *PLOS ONE*) document nitrate enrichment of co-composted particles on the order of **~3–5+ g NO₃⁻-N kg⁻¹** (sequential washing recovered more than EUF: Kammann washing mean ~**5214 mg nitrate-N kg⁻¹** across particle sizes vs EUF ~**2.1 g kg⁻¹**), largely protected from leaching, partly plant-available, without stimulating N₂O in those experiments ([DOI](https://doi.org/10.1038/srep11080); [DOI](https://doi.org/10.1371/journal.pone.0171214)). Standard 1–2 h KCl extracts can **underestimate** captured nitrate—farm soil tests may miss char-bound N.

Hagemann et al. (2017 *Nat. Commun.*) show an **organic coating**—not bulk oxidation of aromatic C—explains enhanced nutrient retention; bulk aromatic speciation/stability was **not substantially altered** by composting ([DOI](https://doi.org/10.1038/s41467-017-01123-0)). Permanence implication: co-composting does not erase durable C chemistry for credit MRV ([[Permanence]], [[MRV Stack]]).

### 3.5 Volatilization and ammonia bioavailability

Taghizadeh-Toosi et al. demonstrate that NH₃ adsorbed on biochar can remain **plant-bioavailable** ([DOI](https://doi.org/10.1007/s11104-011-0870-3)), including capture from ruminant urine-N ([DOI](https://doi.org/10.1007/s11104-011-1010-9)). Hestrin et al. (2019) add a covalent-bonding pathway distinct from simple electrostatic NH₄⁺ sorption ([DOI](https://doi.org/10.1038/s41467-019-08401-z)). Composting literature shows biochar can cut NH₃ losses (e.g. Steiner et al. 2010 poultry litter: NH₃ − up to **64%**, N loss − up to **52%** at up to 20% DW biochar — [DOI](https://doi.org/10.2134/jeq2009.0337)).

---

## 4. Phosphorus chemistry

### 4.1 Direct P delivery vs soil P dynamics

Biochar affects P by (i) **inherent ash P** (bones, manures, sludge), (ii) altering **sorption/desorption** on soil minerals, (iii) **precipitation** (Ca–P, Mg–P, Fe/Al–P), and (iv) microbial/mycorrhizal mediation. Reviews: NPK cycles ([DOI](https://doi.org/10.1186/s40538-020-00182-8)); P fate in soil/water ([DOI](https://doi.org/10.1016/j.chemosphere.2021.131176)).

Ippolito et al. (2020) meta-data analysis (~5400 papers) concludes **feedstock choice** dominates nutrient contents and that plant-available fractions of N, P, K, Ca, Mg, Fe, Cu can be predicted from feedstock and totals ([DOI](https://doi.org/10.1007/s42773-020-00067-x)).

### 4.2 Enrichment and slow-release P (sourced examples via Ndoung)

Ndoung et al. (2021) compile P-enrichment routes ([DOI](https://doi.org/10.1016/j.heliyon.2021.e08473); [PMC](https://pmc.ncbi.nlm.nih.gov/articles/PMC8646155/)):

| Approach | Example finding (as reported in review/primary) | URL |
|---|---|---|
| Bone waste pyrolysis | Total P ~**12.7%** (350 °C) to **15.3%** (750 °C) (Zwetsloot et al. cited) | https://doi.org/10.1016/j.heliyon.2021.e08473 |
| Dairy carcass biochar | ~**10%** total P (Ma & Matsunaka cited) | same |
| Pre-pyrolysis Mg / TSP impregnation | Slower P release vs TSP; plant P uptake gains (Carneiro, Lustosa Filho lines) | https://doi.org/10.1016/j.scitotenv.2020.143955 · https://doi.org/10.1016/j.scitotenv.2019.136028 |
| Mg–P precipitates on Mg-enriched char | Low-solubility Mg–P + “P-trap” reprecipitation (Luo et al. 2021) | https://doi.org/10.1016/j.scitotenv.2020.144454 |
| Co-composted wood char | Phosphate enrichment alongside nitrate (Kammann EUF curves) | https://doi.org/10.1038/srep11080 |

**Antagonism note:** Gunes et al. (2015) (cited in Ndoung) found P-enriched poultry-manure biochar increased N/P/K uptake in lettuce but **decreased** leaf Fe, Zn, Cu, Mn—dilution and/or immobilization pathways ([DOI](https://doi.org/10.1016/j.heliyon.2021.e08473) table entry; primary Soil Use Manage lineage).

### 4.3 Desorption and plant availability

Silber et al. (2010) show **pH-dependent** mineral release and surface charge evolution for cornstraw biochar—agronomic implication: liming and rhizosphere acidification change what desorbs ([DOI](https://doi.org/10.1021/es101283d)). Negatively charged fresh surfaces can **repel** phosphate; Ca/Mg/Fe/Al bridges and coatings reverse that (P-fate review [DOI](https://doi.org/10.1016/j.chemosphere.2021.131176)).

---

## 5. Potassium, calcium, magnesium, micronutrients

### 5.1 K — often the most plant-available ash cation

High extractable K in many ash-rich chars contributes directly to soil K supply and liming couples (NPK review [DOI](https://doi.org/10.1186/s40538-020-00182-8)). Kammann EUF showed K enrichment of co-composted particles (~1.6-fold vs untreated) with more release in the readily available EUF fraction 1 ([DOI](https://doi.org/10.1038/srep11080)). Karim et al. banana-peduncle plasma processing (cited in Ndoung) raised available K dramatically vs feedstock—example of feedstock-specific K concentration ([DOI](https://doi.org/10.1016/j.heliyon.2021.e08473)).

### 5.2 Ca / Mg and liming couples

Ash Ca/Mg carbonates and oxides drive liming. Jeffery et al. (2011) linked stronger yield responses in **acidic** soils (+14% subgroup) to liming + water-holding mechanisms ([DOI](https://doi.org/10.1016/j.agee.2011.08.015)). NRCS FAQ: biochar is usually alkaline; on soils already **pH > 7**, check liming equivalency and add cautiously; worked example—1 ton biochar/acre at **9% CaCO₃** liming equivalency offsets ~**9%** of a 1 ton lime/acre recommendation ([FAQ](https://nrcs-prod.azureedge.us/sites/default/files/2026-04/soil-carbon-amendment-ac-336-faq.pdf)).

Kammann composting raised Ca on particles (BCpure ~3735 → BCcomp ~6077 mg kg⁻¹ in EUF totals reported) while Mg was low and slightly reduced ([DOI](https://doi.org/10.1038/srep11080)).

### 5.3 Micronutrients (Fe, Zn, Cu, Mn, B, Mo)

- Manure/sludge chars can elevate micronutrients **and** potentially toxic elements—test to EBC/IBI/NRCS limits ([[Contaminants and Quality]]; [EBC](https://www.european-biochar.org/); [IBI](https://biochar-international.org/)).
- Fe-enriched chars used for **Cd immobilization** while releasing N slowly (Chen 2018; Dad 2021 via Ndoung [DOI](https://doi.org/10.1016/j.heliyon.2021.e08473)).
- Biological N fixation literature links biochar to B/Mo availability affecting nodulation (Rondon et al. 2007 lineage summarized in Clough 2013 [DOI](https://doi.org/10.3390/agronomy3020275))—see also [[Biochar Microbes and Soil Biology]].

---

## 6. CEC, AEC, sorption vs desorption

### 6.1 Cation exchange capacity

Fresh high-temperature wood chars often have **modest CEC** until oxidized or coated. Aging forms carboxyl/hydroxyl groups that increase NH₄⁺ retention (Nguyen synthesis; Cheng 2008 [DOI](https://doi.org/10.1016/j.gca.2008.01.010)). High HTT (>600 °C) can **destroy** oxygenated acid groups even as BET surface area rises—tradeoff between physisorption and chemisorption ([DOI](https://doi.org/10.1016/j.geoderma.2016.11.004)).

Crop-/grass-based biochars often show higher CEC than wood in Ippolito meta framing ([DOI](https://doi.org/10.1007/s42773-020-00067-x)). Co-compost coatings and organo-mineral complexes (Fe, Al, Si, Ca, Mg, P, K) add exchange and precipitation sites (Archanjo 2017 [DOI](https://doi.org/10.1016/j.geoderma.2017.01.038); Hagemann 2017 [DOI](https://doi.org/10.1038/s41467-017-01123-0)).

### 6.2 Anion exchange capacity and non-conventional nitrate retention

Conventional AEC of biochars is typically **orders of magnitude lower** than CEC (Silber/Graber framing cited in Kammann discussion [DOI](https://doi.org/10.1038/srep11080)). Yet co-composted chars retain large nitrate loads—**AEC alone does not explain** the phenomenon; micropore H-bonding and organic coatings are the leading hypotheses ([DOI](https://doi.org/10.1371/journal.pone.0171214); [DOI](https://doi.org/10.1038/s41467-017-01123-0)).

### 6.3 Sorption ↔ desorption ↔ plant uptake

Desorption depends on N loading, soil hydraulic regime, plant demand, and method (Nguyen/Clough). Taghizadeh-Toosi bioavailability work shows adsorbed NH₃ is not a dead end ([DOI](https://doi.org/10.1007/s11104-011-0870-3)). Marschner et al. (2022) caution that **sorption capacity of unmodified biochar is often too low** to make high-analysis slow-release N fertilizers from sorption alone—**coating / composites** are usually required for true controlled-release N products ([DOI](https://doi.org/10.1007/s11104-022-05365-w)).

---

## 7. Fresh vs aged vs inoculated / enriched — nutrient behavior

| State | Typical nutrient behavior | Agronomic implication | Sources |
|---|---|---|---|
| **Fresh high-C wood, uncharged** | SIN ↓ (~10%); hungry sponge; possible yield drag | Charge or co-apply fertilizer; or apply ≥1 month pre-plant | Nguyen 2017; NRCS FAQ; Kammann untreated |
| **Fresh manure/bone char** | Intrinsic N/P/K/ash; high EC risk | Soil-test P/EC; may still blend for biology | Ndoung direct-treatment; NRCS FAQ |
| **Field-aged / oxidized** | ↑ oxygenated groups, organo-mineral phases | Better CEC; still may need fertility program | Cheng 2008; Joseph 2010 lineage |
| **Co-composted (COMBI)** | Organic coating; NO₃⁻/PO₄ capture; growth ↑↑ | Prefer over raw for agronomy | Kammann 2015; Hagemann 2017; Antonangelo 2021 ([DOI](https://doi.org/10.1016/j.jenvman.2020.111443)) |
| **Post-pyrolysis BBF (NPK/urine/digestate)** | Designed payload; slow release; low dose | Band/root-zone; NUE gains | Melo 2022; Schmidt 2015/2017; Puga 2020 |
| **Physicochemical post-process only** | Particle size / heating / leaching; **not** biological charge | Gale meta +14% plant growth vs raw; excluded co-compost | Gale 2021 ([DOI](https://doi.org/10.1007/s42773-021-00115-0)) |

---

## 8. Biochar-based fertilizers (BBF / BCF) — formulations and evidence

### 8.1 Production typology (Ndoung 2021)

**Correct DOI:** https://doi.org/10.1016/j.heliyon.2021.e08473 ([PMC8646155](https://pmc.ncbi.nlm.nih.gov/articles/PMC8646155/)).

1. **Direct treatment** — pyrolyze inherently nutrient-rich feedstocks (manures, sludge, algae, bones). Low T (~300–400 °C) favors **N retention**; higher T (~700 °C) favors **P/K concentration** (Biederman & Harpole 2013 cited therein; [DOI](https://doi.org/10.1111/gcbb.12037)).
2. **Pre-treatment** — impregnate biomass with minerals/fertilizers **before** pyrolysis (MgCl₂, TSP, phosphate rock, urea+clays, etc.).
3. **Post-treatment** — treat finished biochar with fertilizers, clays, composts, wastewater, digestate, microbes (~**60%** of enrichment studies in their sample). May include granulation, starch/bentonite/PVA coatings, re-pyrolysis.

### 8.2 Coating and impregnation — what the evidence supports

| Design | Evidence highlight | DOI / URL |
|---|---|---|
| Urea–bentonite–biochar granules / Bio-MUC | Slower N release; maize growth gains (Shi et al. via Ndoung) | https://doi.org/10.1016/j.scitotenv.2019.134424 |
| Biochar-coated urea | Controlled N loss; ↑ NUE (Jia et al. 2021) | https://doi.org/10.1186/s40538-020-00205-4 |
| Eucalyptus biochar + urea (field) | NUE **+12%** vs urea; maize yield **+26%**; GHG intensity −14% (Puga et al. 2020) | https://doi.org/10.1016/j.scitotenv.2019.135375 |
| Urine 1:1 vol + compost, root-zone | Pumpkin **82.6 t ha⁻¹**; >300% vs urine-only (Schmidt 2015); biochar DM **0.75 t ha⁻¹** | https://doi.org/10.3390/agriculture5030723 |
| Liquid enrichment 21 trials / 13 crops | Framework for biochar-based fertilization (Schmidt 2017) | https://doi.org/10.1002/ldr.2761 |
| Digestate impregnation | ↑ SOM/macronutrients vs unenriched char (Kizito 2019 via Ndoung) | https://doi.org/10.1016/j.heliyon.2021.e08473 |
| Struvite–biochar composites | Longer N/P release cycle (Hu et al. via Ndoung) | same |
| Marschner 2022 review | Sorption alone often insufficient for high-N BCF; coatings needed | https://doi.org/10.1007/s11104-022-05365-w |

### 8.3 Melo et al. 2022 productivity meta (headline numbers)

148 pairwise comparisons; BBFs applied at very low mean rate **0.9 t ha⁻¹** ([DOI](https://doi.org/10.1007/s11104-021-05276-2)):

| Contrast | Mean productivity change |
|---|---|
| BBF vs fertilized control | **+10%** |
| BBF vs unfertilized control | **+186%** |
| HHT >400 °C vs ≤400 °C | **+12%** vs no increase |
| Final mixture C >30% vs ≤30% | **+17%** vs no effect |
| Cluster: soils unresponsive to conventional fertilizer | potential **+15%** |

Authors interpret biochar as a **matrix that raises fertilizer-use efficiency** beyond fertilizer alone—comparable mean productivity lift to much higher bulk-conditioner rates (15–30 t ha⁻¹ class) in prior metas.

### 8.4 2025 review pointer

Agronomy BCF advancements review (2025): https://doi.org/10.3390/agronomy15051104 — use for formulation taxonomy; prefer Melo/Ndoung/Puga/Schmidt for farm numbers.

---

## 9. Synergy and antagonism with mineral fertilizers

### 9.1 Synergy (FUE / yield)

| Source | Finding | URL |
|---|---|---|
| Ye et al. 2020 field meta | Biochar **+ inorganic fertilizer** ~**+15%** yield vs fertilizer alone | https://www.css.cornell.edu/faculty/lehmann/publ/SoilUseManage%2036%2C%202-18%202020%20Ye.pdf |
| Melo 2022 | BBF +10% vs fertilized controls at ~0.9 t ha⁻¹ | https://doi.org/10.1007/s11104-021-05276-2 |
| Puga 2020 | NUE +12%; yield +26% vs urea | https://doi.org/10.1016/j.scitotenv.2019.135375 |
| Liao et al. 2020 (via Ndoung) | Controlled-release biochar-N: rape NUE ~**+58.8%**, yield ~**+16.6%** vs urea framing in review table | https://doi.org/10.1016/j.heliyon.2021.e08473 |
| Jeffery 2017 | Temperate mean raw-char benefit weak — fertilizer/compost co-management matter more | https://doi.org/10.1088/1748-9326/aa67bd |

### 9.2 Antagonism / risks

- Fresh wood char + inadequate N → immobilization / yield drag (Kammann untreated; NRCS FAQ).
- High liming char on alkaline soils → micronutrient / P availability issues (NRCS FAQ).
- High-P manure chars on high-P soils → water-quality risk (NRCS P-index discussion in FAQ).
- Micronutrient depression with some P-enriched products (Gunes via Ndoung).
- Excess BCF N/P or metals if enrichment ratios poorly optimized (Ndoung future perspectives).

---

## 10. Application implications — rates, banding, blends

Deep practice detail: [[Application Rates and Methods]], [[Biochar Inoculation for Fertilizer]], [[Biochar Compost and Manure Blends]].

| Goal | Sourced guidance | URL |
|---|---|---|
| Bulk soil conditioner (CDR + structure) | NRCS start **4–10 yd³/ac**; FY2024 100% biochar scenario **4 yd³/ac** | https://nrcs-prod.azureedge.us/sites/default/files/2026-04/soil-carbon-amendment-ac-336-faq.pdf |
| Agronomic BBF / enriched fertilizer | Often **≪2 t ha⁻¹**; Melo mean **0.9 t ha⁻¹**; Schmidt urine protocol **0.75 t ha⁻¹** DM | Melo DOI; Schmidt 2015 DOI |
| Co-compost loading | Roughly **5–15%** biochar w/w early (Pacific 5–10%; Antonangelo 10–15%) | Pacific PDF; Antonangelo DOI |
| Charge time | **1–3 weeks** moist activation | USBI PDF |
| Timing if raw | ≥**1 month** before planting (Nguyen recommendation) | Nguyen DOI |
| Placement | Root-zone pits / banding for low-dose enriched; broadcast+incorporate for bulk | Schmidt protocols; NRCS FAQ |

Oasis vineyard evidence that **compost+biochar** beat either alone (+36% five-harvest mean vs control): [Oasis PDF](https://pacificbiochar.com/wp-content/uploads/Oasis-Vineyard-Trial_-5th-harvest_-Final-Draft_12.12.2023.pdf).

---

## 11. Master quantitative table (nutrients)

| Claim | Number | Source URL |
|---|---|---|
| SIN NH₄⁺ mean change | −11 ± 2% | https://doi.org/10.1016/j.geoderma.2016.11.004 |
| SIN NO₃⁻ mean change | −10 ± 1.6% | same |
| Untreated BC biomass (quinoa, 2%) | ~60% of control | https://doi.org/10.1038/srep11080 |
| Co-composted BC biomass | up to ~305% of control | same |
| Co-composted NO₃⁻-N (washing) | ~5.2 g kg⁻¹ mean | same |
| Co-composted NO₃⁻-N (EUF, cited range) | ~3–5 g kg⁻¹ class | https://doi.org/10.1371/journal.pone.0171214 |
| BBF vs fertilized productivity | +10% | https://doi.org/10.1007/s11104-021-05276-2 |
| BBF vs unfertilized | +186% | same |
| BBF mean application rate | 0.9 t ha⁻¹ | same |
| Biochar+IF vs IF alone (field) | ~+15% | https://www.css.cornell.edu/faculty/lehmann/publ/SoilUseManage%2036%2C%202-18%202020%20Ye.pdf |
| Puga NUE vs urea | +12% | https://doi.org/10.1016/j.scitotenv.2019.135375 |
| Puga maize yield vs urea | +26% | same |
| Steiner compost NH₃ reduction | up to −64% | https://doi.org/10.2134/jeq2009.0337 |
| Jeffery 2011 grand mean yield | ~+10% | https://doi.org/10.1016/j.agee.2011.08.015 |
| Jeffery acid-soil subgroup | +14% | same |
| Jeffery biosolids subgroup | −28% | same |
| Jeffery 2017 tropics | ~+25% | https://doi.org/10.1088/1748-9326/aa67bd |

---

## 12. Safety — salts, EC, heavy metals from ash-rich feedstocks

| Risk | Guidance / evidence | URL |
|---|---|---|
| High EC / salinity | Manure chars can be high-EC; wood chars typically lower; match to soil EC | NRCS FAQ https://nrcs-prod.azureedge.us/sites/default/files/2026-04/soil-carbon-amendment-ac-336-faq.pdf |
| Alkaline over-liming | Check liming equivalency if soil pH >7 | same FAQ |
| Biosolids / PFAS | **Excluded** from CPS 336 cost-share | same FAQ |
| PTE / PAHs | Meet EBC/IBI/NRCS Table 3; see [[Contaminants and Quality]] | https://www.european-biochar.org/ · https://biochar-international.org/ |
| Yield harm from contaminated feedstocks | Jeffery 2011 biosolids subgroup **−28%** | https://doi.org/10.1016/j.agee.2011.08.015 |
| Excess N/P from poorly designed BCF | Optimize biochar:enrichment ratios (Ndoung gaps) | https://doi.org/10.1016/j.heliyon.2021.e08473 |
| Heavy-metal immobilization upside | Fe/P-enriched chars can reduce labile Cd (Chen/Dad/Zhao lines in Ndoung) | same — still require feedstock testing |

---

## 13. Link to inoculation / fertilizer use (bridge)

Nutrient chemistry explains **why** the three enrichment modes in [[Biochar Inoculation for Fertilizer]] work:

1. **Nutrient charging** fills CEC/pores and builds coatings so desorption matches crop demand.
2. **Microbial inoculation** couples biology to nutrient transformations (immobilization ↔ mineralization; P solubilization)—see [[Biochar Microbes and Soil Biology]].
3. **Co-composting** simultaneously conserves N (Steiner), builds organic coating (Hagemann), and captures nitrate/phosphate (Kammann).

Without that bridge, high-C CDR char remains a sponge; with it, the same carbon becomes a **fertilizer-efficiency technology** at lower mass rates (Melo 2022).

---

## 14. Open gaps (as stated by reviews — do not invent answers)

- Long-term (>1–5 y) field SIN after biochar (Nguyen: limited >1 y cases).
- Multi-nutrient BCF complexes vs single-nutrient enrichment (Ndoung).
- True controlled-release N without polymer coatings at fertilizer-grade analysis (Marschner 2022).
- Standardized desorption assays that recover micropore-captured nitrate (Kammann method discussion).
- Head-to-head FUE at CPS 336–realistic bulk rates vs BBF banding rates.

---

## 15. Decision rules (evidence-based)

1. **Soil-test first** — pH, EC, P, K, OM (NRCS FAQ logic).
2. **If high-C wood char for agronomy** — charge 1–3 weeks or co-compost; do not expect fertilizer substitution (USBI; Kammann).
3. **If BBF/enriched product** — treat as fertilizer placement problem (band/root-zone); rates often <2 t ha⁻¹ (Melo; Schmidt).
4. **If manure/bone char** — credit ash nutrients; manage EC/P index (NRCS).
5. **If alkaline soil** — verify liming equivalency before high rates (NRCS).
6. **If selling CDR** — document eligible soil use; coating does not erase aromatic stability (Hagemann 2017; [[MRV Stack]]).

---

## Primary outbound links

- Nguyen 2017 SIN meta — https://doi.org/10.1016/j.geoderma.2016.11.004
- Clough 2013 N dynamics — https://doi.org/10.3390/agronomy3020275
- Kammann 2015 — https://doi.org/10.1038/srep11080
- Hagemann 2017 Nat Commun — https://doi.org/10.1038/s41467-017-01123-0
- Hagemann 2017 PLOS — https://doi.org/10.1371/journal.pone.0171214
- Ndoung 2021 (e08473) — https://doi.org/10.1016/j.heliyon.2021.e08473
- Melo 2022 — https://doi.org/10.1007/s11104-021-05276-2
- Marschner 2022 — https://doi.org/10.1007/s11104-022-05365-w
- Puga 2020 — https://doi.org/10.1016/j.scitotenv.2019.135375
- Ye 2020 PDF — https://www.css.cornell.edu/faculty/lehmann/publ/SoilUseManage%2036%2C%202-18%202020%20Ye.pdf
- Taghizadeh-Toosi 2012 — https://doi.org/10.1007/s11104-011-0870-3
- Hestrin 2019 — https://doi.org/10.1038/s41467-019-08401-z
- Ippolito 2020 — https://doi.org/10.1007/s42773-020-00067-x
- NPK cycles review — https://doi.org/10.1186/s40538-020-00182-8
- P fate review — https://doi.org/10.1016/j.chemosphere.2021.131176
- Jeffery 2011 — https://doi.org/10.1016/j.agee.2011.08.015
- Jeffery 2017 — https://doi.org/10.1088/1748-9326/aa67bd
- Schmidt 2015 — https://doi.org/10.3390/agriculture5030723
- Schmidt 2017 — https://doi.org/10.1002/ldr.2761
- Steiner 2010 — https://doi.org/10.2134/jeq2009.0337
- Bruun 2012 — https://doi.org/10.1016/j.soilbio.2011.11.019
- Cross & Sohi 2011 — https://doi.org/10.1016/j.soilbio.2011.06.016
- Joseph 2018 — https://doi.org/10.1016/j.scitotenv.2017.09.200
- Archanjo 2017 — https://doi.org/10.1016/j.geoderma.2017.01.038
- Gale 2021 — https://doi.org/10.1007/s42773-021-00115-0
- Silber 2010 — https://doi.org/10.1021/es101283d
- Cheng 2008 — https://doi.org/10.1016/j.gca.2008.01.010
- Lehmann 2021 — https://doi.org/10.1038/s41561-021-00852-8
- NRCS FAQ — https://nrcs-prod.azureedge.us/sites/default/files/2026-04/soil-carbon-amendment-ac-336-faq.pdf
- CPS 336 2022 — https://www.nrcs.usda.gov/sites/default/files/2022-11/336-NHCP-CPS-Soil-Carbon-Amendment-2022.pdf
- USBI Ag Guidelines — https://farmlandinfo.org/wp-content/uploads/sites/2/2023/06/usbi-biochar-guidelines-for-ag-application.pdf
- EBC — https://www.european-biochar.org/
- IBI — https://biochar-international.org/
- Oasis PDF — https://pacificbiochar.com/wp-content/uploads/Oasis-Vineyard-Trial_-5th-harvest_-Final-Draft_12.12.2023.pdf
- Pacific compost white paper — https://pacificbiochar.com/wp-content/uploads/Pacific-Biochar_Biochar-Compost_white-paper.pdf
- 2025 BCF review — https://doi.org/10.3390/agronomy15051104
- Jia coated urea — https://doi.org/10.1186/s40538-020-00205-4
- Luo Mg-P — https://doi.org/10.1016/j.scitotenv.2020.144454
- Biederman & Harpole 2013 — https://doi.org/10.1111/gcbb.12037
- Antonangelo 2021 — https://doi.org/10.1016/j.jenvman.2020.111443

---

## See also

- [[Biochar Inoculation for Fertilizer]] — protocols, commercial products, decision trees
- [[Biochar Microbes and Soil Biology]] — habitat, inocula, priming, disease
- [[Biochar Compost and Manure Blends]] · [[Crop Yield Effects]] · [[GHG Fluxes]]
- [[Soil and Agriculture]] · [[Applications Hub]] · [[Key Sources]] · [[Biochar Home]]


---

## 16. Deep dive — mechanisms of N retention (abiotic)

### 16.1 Acid functional groups and NH₄⁺

Nguyen et al. (2017) summarize that carboxylic, hydroxyl, lactone, and lactol groups create negative surface charge that electrostatically attracts NH₄⁺ ([DOI](https://doi.org/10.1016/j.geoderma.2016.11.004)). Grassy feedstocks can develop higher carboxyl density than woody feedstocks at comparable pyrolysis temperatures (Harvey et al. lineage summarized therein), helping explain why woody chars reduced SIN less in that meta.

### 16.2 Physisorption and BET

Inner-surface physisorption scales with BET and pore volume. High-temperature and slow-pyrolysis chars generally increase BET until a deformation threshold destroys micropores (pine ~750 °C, wheat ~700 °C examples in Nguyen synthesis). Bruun et al. (2012) report BET of wheat-straw biochars **0.6 vs 1.6 m² g⁻¹** for fast vs slow pyrolysis ([DOI](https://doi.org/10.1016/j.soilbio.2011.11.019))—physical sorption capacity is process-dependent even at fixed feedstock.

### 16.3 Base groups and weak conventional NO₃⁻ sorption

Chromenes, ketones, and pyrones can facilitate limited NO₃⁻ adsorption, but conventional anion capacity remains weak relative to cation capacity ([DOI](https://doi.org/10.1016/j.geoderma.2016.11.004); Kammann discussion [DOI](https://doi.org/10.1038/srep11080)). The large nitrate inventories in co-composted particles therefore require the **non-conventional** mechanisms in §3.4.

### 16.4 Temperature window during composting

Kammann et al. note thermophilic composting (60–70 °C) may strengthen nutrient capture relative to cooler model composting (~35 °C in Prost et al. comparisons discussed in their paper), consistent with Conte et al. NMR work on temperature-dependent water–biochar bonding cited therein ([DOI](https://doi.org/10.1038/srep11080)). Practical implication: **aerobic quality windrow composting** of char is not equivalent to cold mixing for nitrate capture.

---

## 17. Deep dive — biotic N pathways that change fertilizer chemistry

| Process | Short-term SIN effect | Longer-term / management note | Sources |
|---|---|---|---|
| Mineralization / positive priming | Can ↑ SIN briefly | Stronger with low-T / manure chars | Zimmerman 2011 ([DOI](https://doi.org/10.1016/j.soilbio.2011.02.005)); Luo et al. cited in Nguyen |
| Immobilization | ↓ SIN | C:N threshold ~20–32; labile C matters more than bulk C:N of wood | Chan & Xu / Kuzyakov framing in Nguyen; Bruun 2012 |
| Nitrification | NH₄⁺ → NO₃⁻ | Liming of acid soils; AOA/AOB increases may take >1 year | Prommer / Bai lineage in Nguyen; Clough 2013 |
| Denitrification / N₂O | ↓ NO₃⁻; GHG co-benefit | Cayuela metas; H:C_org moderator | [[GHG Fluxes]]; https://doi.org/10.1016/j.agee.2013.10.009 |
| Biological N₂ fixation | Can offset SIN decline in legumes | Nodulation responses mixed; Quilliam 2013 clover caveat | Clough 2013; Quilliam https://doi.org/10.1016/j.soilbio.2013.06.004 |

Fertilizer chemistry takeaway: **organic co-amendments** change the biotic balance toward mineralization (Nguyen), which is why compost charging simultaneously addresses abiotic sorption and biotic immobilization ([[Biochar Compost and Manure Blends]]).

---

## 18. Feedstock × pyrolysis temperature — nutrient design space

Synthesized from Ippolito et al. 2020 ([DOI](https://doi.org/10.1007/s42773-020-00067-x)), Ndoung 2021 ([DOI](https://doi.org/10.1016/j.heliyon.2021.e08473)), and Nguyen 2017 ([DOI](https://doi.org/10.1016/j.geoderma.2016.11.004)):

| Design goal | Lean toward | Watch-outs |
|---|---|---|
| Maximum durable C + structure | High-T wood (>500–600 °C); high SSA | Low nutrients; charge required; micropores may be poorly colonized ([[Biochar Microbes and Soil Biology]]) |
| Intrinsic fertilizer value | Manure, bone, algae; moderate–high T for P/K | EC, metals, PFAS policy (biosolids) |
| N retention in char | Lower T (300–400 °C) on N-rich feedstocks | More labile C → immobilization risk if uncharged |
| P/K concentration | Higher T on ash-rich feedstocks | Plant-available fraction ≠ total; test Olsen/Mehlich etc. |
| Slow-release engineered P | Pre-pyrolysis Mg/TSP impregnation | Rate as fertilizer, not as bulk conditioner |
| Nitrate capture product | Co-compost high-T wood in N-rich windrows | Process control (moisture, turning, maturity) |

NRCS FAQ spec-sheet contrast (high-C wood vs poultry-manure char) is the extension-facing version of this design space ([FAQ](https://nrcs-prod.azureedge.us/sites/default/files/2026-04/soil-carbon-amendment-ac-336-faq.pdf)).

---

## 19. Analytical blind spots for farm labs

1. **Standard KCl / water extracts underestimate** micropore-captured nitrate (Kammann sequential washing >> EUF >> quick extract) ([DOI](https://doi.org/10.1038/srep11080)).
2. **Total ash P ≠ plant-available P** — use agronomic soil tests after application, not only char totals (Ippolito availability framing [DOI](https://doi.org/10.1007/s42773-020-00067-x)).
3. **Liming equivalency** must be measured, not assumed from pH alone (NRCS FAQ arithmetic).
4. **EC** on manure chars can dominate first-year risk even when NPK looks attractive (NRCS FAQ).
5. **H:C_org and C_org** remain the permanence/quality gates for CPS 336 and credits even when nutrients are the farm goal ([[Properties]]; [CPS 336 PDF](https://www.nrcs.usda.gov/sites/default/files/2022-11/336-NHCP-CPS-Soil-Carbon-Amendment-2022.pdf)).

---

## 20. Worked planning scenarios (sourced numbers only)

### Scenario A — Temperate fertile row crop, wood char, yield goal
Expect weak mean raw-char yield response ([Jeffery 2017](https://doi.org/10.1088/1748-9326/aa67bd)). Charge 1–3 weeks with compost ([USBI](https://farmlandinfo.org/wp-content/uploads/sites/2/2023/06/usbi-biochar-guidelines-for-ag-application.pdf)) or use CPS 336 blend scenarios ([FAQ](https://nrcs-prod.azureedge.us/sites/default/files/2026-04/soil-carbon-amendment-ac-336-faq.pdf)). Co-apply fertilizer; Ye 2020 supports biochar+IF synergy ([PDF](https://www.css.cornell.edu/faculty/lehmann/publ/SoilUseManage%2036%2C%202-18%202020%20Ye.pdf)).

### Scenario B — Acid tropical sandy soil
Liming + WHC mechanisms more likely to reward even less-enriched char ([Jeffery 2011](https://doi.org/10.1016/j.agee.2011.08.015); [Jeffery 2017](https://doi.org/10.1088/1748-9326/aa67bd)), but nutrient charging still improves FUE (Melo; Schmidt).

### Scenario C — Low-dose BBF program
Target Melo-class rates (~1 t ha⁻¹) with documented enrichment (urine/NPK/compost) and root-zone placement ([Schmidt 2015](https://doi.org/10.3390/agriculture5030723); [Melo 2022](https://doi.org/10.1007/s11104-021-05276-2)).

### Scenario D — CDR-primary with secondary agronomy
Meet H:C_org / eligible-use MRV; still inoculate for farm relations and to avoid year-1 drag (NRCS/USBI); Hagemann shows composting coating does not erase aromatic stability ([DOI](https://doi.org/10.1038/s41467-017-01123-0)).

---

## 21. Glossary (nutrient chemistry)

- **AEC** — anion exchange capacity (usually low on biochar vs CEC).
- **BBF / BCF** — biochar-based fertilizer / biochar-based compound fertilizer.
- **CEC** — cation exchange capacity.
- **COMBI** — co-composted biochar–compost product (Antonangelo framing).
- **EUF** — electro-ultrafiltration nutrient extraction (Kammann method).
- **FUE / NUE / PUE** — fertilizer / nitrogen / phosphorus use efficiency.
- **SIN** — soil inorganic nitrogen (NH₄⁺ + NO₃⁻).
- **Liming equivalency** — % CaCO₃ neutralizing value of the amendment.

---

## 22. Related notes (navigation)

| Need | Go to |
|---|---|
| How to charge / inoculate / protocols | [[Biochar Inoculation for Fertilizer]] |
| Microbes, AMF, disease, priming biology | [[Biochar Microbes and Soil Biology]] |
| Compost ratios & facility trials | [[Biochar Compost and Manure Blends]] |
| Yield metas | [[Crop Yield Effects]] |
| N₂O / priming fluxes | [[GHG Fluxes]] |
| yd³/ac & banding | [[Application Rates and Methods]] |
| Contaminants | [[Contaminants and Quality]] |
| Soil chapter hub | [[Soil and Agriculture]] |
