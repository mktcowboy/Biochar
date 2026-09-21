---
tags: [production, contaminants, PFAS, biosolids, testing]
aliases: [PFAS and Emerging Contaminants, PFAS biochar, PFAS and biochar, Biosolids PFAS, Emerging contaminants]
updated: 2026-09-16
---

# PFAS and Biochar

A standalone chapter on **per- and polyfluoroalkyl substances (PFAS)** in biochar systems: how PFAS can enter feedstocks, what pyrolysis does and does not prove, where fluorinated material may go, how biochar can immobilize PFAS in soil, and how to test and communicate results. Regulatory snapshot: **2026-09-16**.

**Related notes:** [[Contaminants and Quality]] · [[Feedstocks]] · [[Woody vs Manure Ag Feedstocks]] · [[Pyrolysis Systems and Temperatures]] · [[Testing EBC IBI S668]] · [[Biochar Lab Measurement Standard|standardizes biochar lab testing]] · [[PAHs]] · [[Heavy Metals and Ash]] · [[Product Standards EBC IBI]] · [[Risks and Controversies]] · [[Key Sources]]

---

## TL;DR

1. **A clean char result is not, by itself, proof of PFAS destruction.** Pyrolysis can move PFAS or fluorinated transformation products from the solid into condensate, oil, gas, scrubber water, or stack emissions. A 2023 biosolids study removed **>99%** of targeted PFAS and precursors from char at 500, 650, and 800 °C, yet NMeFOSE and NEtFOSE masses in py-liquid rose by **more than two orders of magnitude** ([McNamara et al. 2023](https://doi.org/10.1039/D2EW00677D)).
2. **Temperature matters, but it is not a universal pass/fail surrogate.** One sewage-sludge series found >99% targeted-PFAS removal from solids at 400 °C and >99.9% at 600 °C, while recommending at least 600 °C for commercial heterogeneity; the authors also detected PFAS in primary pyrolysis gas ([Hušek et al. 2024](https://doi.org/10.1007/s42773-024-00322-5)). A 2026 study found only **24–88%** removal at 500 °C for industrially impacted biosolids but **>95%** at 800 °C ([McNamara et al. 2026](https://doi.org/10.1002/wer.70352)).
3. **Integrated off-gas treatment can greatly improve a measured target-PFAS balance.** A laboratory pyrolysis-plus-thermal-oxidizer train reported **99.4% molar removal** of targeted PFAS and flue-gas PFAS equal to **0.200%** of input; short-chain species dominated what remained, and the authors still flagged unmeasured/recombined products as a gap ([Winchell et al. 2024](https://doi.org/10.1002/wer.11149)).
4. **Biochar can also be a PFAS sorbent, which is containment—not destruction.** Activated waste-timber biochar reduced PFAS leaching by >90% at doses ≥0.5% in a low-organic-carbon soil, but results weakened in a high-organic-carbon soil and for short-chain PFAS ([Sørmo et al. 2021](https://doi.org/10.1016/j.scitotenv.2020.144034)).
5. **Use a matrix-appropriate analytical stack.** ANSI/ASABE/USBI S668 recommends periodic PFAS testing for biochar from biosolids or other potentially high-PFAS waste feedstocks, using **EPA Method 1633A**; S668 supplies methods, not PFAS limits ([S668 §12.1.4](https://biochar.org/wp-content/uploads/2026/05/ANSI-S668.pdf)). Method 1633A measures **40 named PFAS** in aqueous, solid, biosolids, and tissue matrices—not “all PFAS” ([EPA Method 1633A](https://www.epa.gov/system/files/documents/2024-12/method-1633a-december-5-2024-508-compliant.pdf)).
6. **Do not borrow drinking-water numbers as a biochar standard.** U.S. federal MCLs, CERCLA designations, state biosolids programs, product standards, and laboratory methods are different legal/technical layers ([EPA drinking-water rule](https://www.epa.gov/sdwa/and-polyfluoroalkyl-substances-pfas); [EPA CERCLA page](https://www.epa.gov/superfund/designation-perfluorooctanoic-acid-pfoa-and-perfluorooctanesulfonic-acid-pfos-cercla)).

---

## 1. What PFAS are

PFAS are a large family of manufactured fluorinated chemicals. Their carbon–fluorine bonds confer useful resistance to heat, oil, water, and stains, while many members or transformation products can be unusually persistent and mobile; “PFAS” therefore names a **class**, not one chemical with one behavior ([EPA, “PFAS Explained”](https://www.epa.gov/pfas/pfas-explained)).

Important distinctions for biochar work:

- **Perfluoroalkyl** substances have a fully fluorinated alkyl moiety; **polyfluoroalkyl** substances are not fully fluorinated and may transform into persistent perfluoroalkyl acids ([OECD terminology overview](https://www.oecd.org/chemicalsafety/portal-perfluorinated-chemicals/terminology-per-and-polyfluoroalkyl-substances.pdf)).
- Familiar terminal acids include PFOA, PFOS, PFNA, PFHxS, PFBS, PFBA, and others; precursor classes include fluorotelomers and sulfonamides. A target list sees only the compounds on that list ([ITRC PFAS fact sheets](https://pfas-1.itrcweb.org/fact-sheets/)).
- Long-chain PFAS often sorb more strongly to organic matter and carbonaceous sorbents; short- and ultrashort-chain species are generally more mobile and harder to retain, so conversion of a long-chain target into a short-chain product is not equivalent to mineralization ([Behnami et al. 2024](https://doi.org/10.1016/j.chemosphere.2024.142088)).
- **Mineralization** means conversion of organofluorine toward inorganic fluoride/HF plus nonfluorinated end products. Disappearance from one targeted chromatogram, one phase, or one target list proves less than mineralization ([Longendyke et al. 2022](https://doi.org/10.1039/D1EM00465D)).

### Vocabulary used in this chapter

| Term | What it can support | What it cannot support alone |
|---|---|---|
| Solid-phase removal | Less measured analyte in char than feed, yield-corrected where possible | Destruction across the whole plant |
| Target-PFAS destruction/removal efficiency | Closure for the named analytes and sampled streams | Fate of nontarget PFAS, volatile fluorocarbons, or all organofluorine |
| Phase transfer | Movement to oil, aqueous condensate, gas, dust, or scrubber water | Detoxification |
| Transformation | Parent disappears and another fluorinated compound forms | Complete defluorination |
| Mineralization | Organic fluorine converted to inorganic end products | Established without fluorine/end-product balance |
| Immobilization | Lower leaching or uptake while sorbent remains effective | Destruction or permanent risk elimination |

This terminology follows the central warning in PFAS thermal-treatment reviews: temperature, atmosphere, residence time, feed matrix, target scope, and end-product measurement jointly determine what a “removal” number means ([Longendyke et al. 2022](https://doi.org/10.1039/D1EM00465D)).

---

## 2. How PFAS enter a biochar system

A PFAS pathway should be mapped **before** selecting a reactor or end use:

```text
upstream use/release
  → biomass, wastewater, sludge, compost, paper waste, or contaminated soil
  → drying / blending / storage
  → pyrolysis reactor
  → char + dust
  → py-oil / aqueous condensate
  → permanent gas / combustion unit
  → scrubber water / ash / stack
  → product use, disposal, or further treatment
```

Every arrow can change measured concentration through moisture loss, char yield, dilution, volatilization, condensation, precursor conversion, or actual destruction ([McNamara et al. 2023](https://doi.org/10.1039/D2EW00677D); [Sørmo et al. 2023](https://doi.org/10.1016/j.jhazmat.2023.131447)).

### 2.1 Wastewater sludge and biosolids

PFAS reach wastewater facilities through industrial discharges, commercial and household products, landfill leachate, pulp-and-paper activity, and aqueous film-forming foam (AFFF) releases. Conventional treatment was not designed to destroy them; some PFAS partition to solids and some precursors transform during treatment ([EPA biosolids PFAS page](https://www.epa.gov/biosolids/and-polyfluoroalkyl-substances-pfas-sewage-sludge); [EPA NPDES PFAS memo](https://www.epa.gov/system/files/documents/2022-12/NPDES_PFAS_State%20Memo_December_2022.pdf)).

That makes biosolids a high-priority feedstock for source tracing and lot-specific testing. A survey of sludge/biosolids from **27** North American water resource recovery facilities documented both terminal PFAS and precursors and showed that treatment can change profiles rather than simply eliminate the class ([Winchell et al. 2025](https://pmc.ncbi.nlm.nih.gov/articles/PMC11847621/)).

Industrial inputs matter. Bench tests published in 2026 found >95% removal at both 500 and 800 °C for non-industrially impacted material, but industrially impacted biosolids achieved only 24–88% at 500 °C and >95% at 800 °C ([McNamara et al. 2026](https://doi.org/10.1002/wer.70352)).

### 2.2 Compost and food-contact paper

Compost is not intrinsically PFAS-free. U.S. composts containing food packaging had higher perfluoroalkyl-acid burdens than composts without those inputs, implicating PFAS-treated food-contact materials as a pathway ([Choi et al. 2019](https://doi.org/10.1021/acs.estlett.9b00280)). Target and nontarget screening in France likewise found fluorinated substances in biosolids, composts, and other land-applied organic wastes, including paper-related materials ([Munoz et al. 2022](https://doi.org/10.1021/acs.est.1c03697)).

A compost-derived feedstock therefore needs procurement controls for food-serviceware, coated paper, textiles, and mixed residuals. “Compost” describes processing history, not contaminant status; the same logic applies to [[Biochar Compost and Manure Blends]] after production.

### 2.3 Pulp, paper, cardboard, and paper-mill residuals

PFAS have been used to impart oil, grease, and water resistance to paper and packaging. Releases can occur during manufacture, recycling, wastewater treatment, composting, and disposal ([EPA Multi-Industry PFAS Study](https://www.epa.gov/system/files/documents/2021-09/multi-industry-pfas-study_preliminary-2021-report_508_2021.09.08.pdf)).

Paper fiber itself is not a reliable screening category: untreated clean fiber and coated food-contact paper do not have the same risk. For mixed paper sludge or recycled-fiber residues, supplier declarations should be supplemented by analytical testing when soil use is contemplated ([Munoz et al. 2022](https://doi.org/10.1021/acs.est.1c03697)).

### 2.4 AFFF-impacted land, biomass, and remediation residuals

Fire-training areas and other AFFF release sites can contaminate soil, groundwater, vegetation, and remediation media. If harvested biomass, excavated organic material, spent sorbent, or treatment sludge from such a site is proposed as a pyrolysis feed, its provenance—not its botanical label—sets the PFAS risk ([EPA AFFF information](https://www.epa.gov/pfas/aqueous-film-forming-foam-afff)).

A 2025 phytoremediation study found PFAS translocation factors of **3.07–58.6** in *Oenothera rosea*; pyrolysis above 500 °C removed **99.2%** of measured PFAS from the biomass, but total fluorine increased, underscoring the risk of unidentified fluorinated products ([Nature Communications study](https://doi.org/10.1038/s41467-025-65191-3)). Contaminated biomass-to-char should therefore be treated as a waste-treatment train, not automatically as ordinary clean biochar production.

### 2.5 Manure and animal agriculture: make the pathway explicit

PFAS can enter farms through contaminated water, soil, forage, biosolids-amended fields, dust, or products used on-site; transfer to crops, livestock, milk, eggs, and meat is part of EPA’s biosolids exposure modeling ([EPA 2025 draft sewage-sludge risk assessment](https://www.epa.gov/system/files/documents/2025-01/draft-sewage-sludge-risk-assessment-pfoa-pfos.pdf)). Manure from an impacted herd or site can therefore be a plausible secondary feedstock pathway, but “manure” alone does not establish a high PFAS burden.

Do **not** infer PFAS contamination merely from veterinary treatment. Fluorinated pharmaceuticals and fluoroquinolone antibiotics are distinct chemical/regulatory categories; direct evidence that routine treatment creates a material PFAS load in manure is limited. Where animal treatment is suspected, identify the actual active ingredient and transformation products rather than relabeling all organofluorine as PFAS ([OECD PFAS terminology](https://www.oecd.org/chemicalsafety/portal-perfluorinated-chemicals/terminology-per-and-polyfluoroalkyl-substances.pdf); [Wohde et al. 2016 veterinary-drug review](https://doi.org/10.1186/s12302-016-0091-8)).

### 2.6 “Clean” woody and crop feedstocks

Woody or crop-residue feedstocks are generally lower-risk than wastewater residuals only when sourcing excludes impacted land, coated/treated wood, mixed demolition debris, AFFF sites, and contaminated process water. Sørmo et al. detected PFAS across waste fractions that included wood-based materials, with feed concentrations spanning **56–3,651 ng g⁻¹**, showing that a feedstock label cannot replace measurement where provenance is uncertain ([Sørmo et al. 2023](https://doi.org/10.1016/j.jhazmat.2023.131447)).

See [[Feedstocks]] and [[Woody vs Manure Ag Feedstocks]] for the broader feedstock screen; PFAS is one contaminant family among metals, PAHs, salts, plastics, and pathogens.

---

## 3. Process fate: carry-through, transfer, transformation, and destruction

### 3.1 Concentration is not mass

Drying and pyrolysis remove water and volatile matter, so comparing feed and char in ng g⁻¹ without correcting for dry mass and char yield can misstate removal. At minimum, report:

- dry feed mass and moisture;
- dry char, oil/condensate, dust, and aqueous-residual masses;
- gas volume or normalized dry gas flow;
- concentration, detection/quantitation limits, and recovery in each stream;
- analyte-specific and fluorine-based input/output balances.

This is why Sørmo et al. yield-corrected solid removal and separately calculated emissions per tonne of biochar ([Sørmo et al. 2023](https://doi.org/10.1016/j.jhazmat.2023.131447)).

### 3.2 Drying is already a PFAS unit operation

Drying can transfer PFAS before the pyrolysis reactor. A 2026 study reported **43–74%** reduction from biosolids during drying (mean **58%**, moisture correlation **R² = 0.61**) and recovered **12–22%** of initial measured PFAS in dryer condensate, especially 5:3 FTCA, 7:3 FTCA, NMeFOSE, and NEtFOSE ([McNamara et al. 2026](https://doi.org/10.1039/D5EW01120E)).

Consequences:

- A dryer-condensate sample is part of the PFAS balance, not optional housekeeping.
- Comparing wet feed with dried feed can confuse water loss, volatilization, and transformation.
- Condensate recirculation can return PFAS to the front of the process.

### 3.3 What lower-temperature treatment shows

In sewage sludge heated from 200 to 700 °C, Hušek et al. found poor removal below 400 °C; reported solid-phase targeted-PFAS removal exceeded 99% at 400 °C and 99.9% at 600 °C, while organic-fluorine measurements and gas capture showed that primary gas still required purification or combustion ([Hušek et al. 2024](https://doi.org/10.1007/s42773-024-00322-5)).

This does **not** create a universal “400 °C destroys PFAS” rule. Reactor scale, heating profile, residence time, feed heterogeneity, initial concentration, atmosphere, mineral matrix, and gas handling differ. The same authors recommended at least 600 °C for commercial sludge units because real feed is heterogeneous ([Hušek et al. 2024](https://doi.org/10.1007/s42773-024-00322-5)).

### 3.4 Evidence table: pyrolysis and integrated systems

| Study / system | Conditions | Solid result | Other phases / interpretation |
|---|---|---|---|
| Commercial biosolids pilot, 41 targets | Commercial system; target analysis by two labs | 21 feed targets at about 2–85 µg kg⁻¹; none detected in char; estimated mean removal >97.4% | No nontarget-PFAS or complete product-of-incomplete-combustion balance; authors called for more research ([Thoma et al. 2022](https://doi.org/10.1080/10962247.2021.2009935); [open full text](https://pmc.ncbi.nlm.nih.gov/articles/PMC9128340/)) |
| Biosolids batch pyrolysis | 500, 650, 800 °C; triplicate; 30 min | >99% of targeted PFAS and TOP-measured precursors removed from solid | PFBA increased; NMeFOSE and NEtFOSE in py-liquid increased >100× at all temperatures, showing transformation/transfer ([McNamara et al. 2023](https://doi.org/10.1039/D2EW00677D)) |
| Diverse contaminated organic wastes | 500–800 °C; about 20 min; sludge and wood-based wastes | ≥96.9% yield-corrected removal; residual 0.1–3.4 ng g⁻¹ in chars up to 750 °C | Stack load 0.01–3.1 mg per tonne biochar and <3% of input target-PFAS mass; short chains dominated emissions; oil/unmeasured products remained uncertain ([Sørmo et al. 2023](https://doi.org/10.1016/j.jhazmat.2023.131447)) |
| Sewage sludge + spiked sand | 200–700 °C; lab plus commercial check | >99% target removal at 400 °C; >99.9% at 600 °C; organic fluorine below quantitation above 400 °C in tested solids | PFAS were present in primary gas; authors recommend gas purification/combustion and ≥600 °C commercially ([Hušek et al. 2024](https://doi.org/10.1007/s42773-024-00322-5)) |
| Pyrolysis + thermal oxidizer | Lab train reflecting full-scale configuration | Compound-specific system reduction 91.5% to >99.9% | Overall 99.4% molar target removal; flue gas 0.200% of input; short chains were 54.4–79.5% of exhaust PFAS moles; recombination/incomplete degradation unresolved ([Winchell et al. 2024](https://doi.org/10.1002/wer.11149)) |
| Fixed-bed biosolids / co-pyrolysis | 600 °C; gas ~10 s; solids ~1 h; 1:1 alum sludge or wheat straw in co-runs | Total PFAS 409.9 → 0.31 ng g⁻¹ in char | Bio-oil 5.5 ng g⁻¹; scrubber water 0.15 ng g⁻¹; reported target-PFAS destruction 99.4%; long solids residence limits scale-up transferability ([Rathnayake et al. 2025](https://doi.org/10.1016/j.jaap.2025.106970)) |
| Nonindustrial vs industrial biosolids | 500 and 800 °C; triplicate | Nonindustrial: >95% at both; industrial: 24–88% at 500 °C, >95% at 800 °C | About half the nonindustrial input target-PFAS mass appeared in liquid + gas, requiring downstream polishing ([McNamara et al. 2026](https://doi.org/10.1002/wer.70352)) |
| Fluidized-bed pilot | ~15 kg dry biosolids h⁻¹ for 14 days | Feed 58.1 ng g⁻¹; target PFAS nondetect in char | Nondetect in sampled scrubber water and flue gas; still target- and detection-limit-dependent evidence ([Hakeem et al. 2026](https://doi.org/10.1016/j.jaap.2025.107343)) |
| Full-scale byproduct characterization | Complementary target, total-organic-fluorine, and extractable-organic-fluorine methods | Total organic fluorine decreased 81%, but extractable organic fluorine only 12%; PFBA/PFBS and TFA were enriched in char | Demonstrates how a targeted panel can miss short-chain/nontarget fluorinated residuals ([Edirisinghe et al. 2026](https://doi.org/10.1021/acs.est.5c17517)) |

### 3.5 What the temperature evidence really says

The evidence supports five bounded statements:

1. **Below ~400 °C is poorly supported for sludge PFAS treatment.** In the 200–700 °C series, 300 °C left substantial PFAS in char, while 400 °C changed the outcome sharply ([Hušek et al. 2024](https://doi.org/10.1007/s42773-024-00322-5)).
2. **500 °C can clean some chars but fail on a more contaminated or less-converted matrix.** Compare the >99% solid removal in one 500–800 °C batch study with 24–88% at 500 °C for industrially impacted biosolids in the later study ([McNamara et al. 2023](https://doi.org/10.1039/D2EW00677D); [McNamara et al. 2026](https://doi.org/10.1002/wer.70352)).
3. **600–800 °C generally improves solid-phase target removal, but gas/liquid management remains part of treatment.** This pattern appears across sludge and mixed-waste studies ([Hušek et al. 2024](https://doi.org/10.1007/s42773-024-00322-5); [Sørmo et al. 2023](https://doi.org/10.1016/j.jhazmat.2023.131447)).
4. **Long residence can make a 600 °C bench result look stronger than a short-contact commercial reactor.** Rathnayake et al. used about 1 h solids residence and explicitly called for confirmation under large-scale operating parameters ([Rathnayake et al. 2025](https://doi.org/10.1016/j.jaap.2025.106970)).
5. **A secondary combustor/thermal oxidizer is not automatically validated by its set point.** A credible claim includes measured temperature, gas residence, oxygen/mixing, upset conditions, sampled streams, target list, and fluorinated products of incomplete destruction ([EPA 2026 interim destruction/disposal guidance](https://www.epa.gov/system/files/documents/2026-04/2026-interim-guidance-on-pfas-destruction-and-disposal.pdf)).

### 3.6 Why PFAS can appear to “form” during pyrolysis

Heating can:

- release a PFAS that was not efficiently extracted from the feed matrix;
- cleave a precursor into a terminal acid on the target list;
- shorten a fluorinated chain into PFBA, PFBS, TFA, or another mobile product;
- move a semivolatile precursor into condensate;
- create volatile fluorocarbons or carbonyl fluoride not included in a liquid LC-MS/MS panel.

The >100-fold FOSE increase in py-liquid and PFBA increase observed by McNamara et al. are measured examples of apparent formation/transformation ([McNamara et al. 2023](https://doi.org/10.1039/D2EW00677D)). The 2026 total/extractable-organic-fluorine study provides a second warning: large target-PFAS reductions can coexist with residual or enriched short-chain organofluorines ([Edirisinghe et al. 2026](https://doi.org/10.1021/acs.est.5c17517)).

### 3.7 Thermal chemistry is compound- and matrix-specific

Pure-compound thermal studies show PFOA and PFOS decompose through different pathways and can produce HF, COF₂, fluorocarbons, and shorter perfluorinated products. Atmosphere, water/steam, minerals, and oxygen affect pathways; substantial parent loss can occur below the conditions needed for broad fluorine mineralization ([Longendyke et al. 2022](https://doi.org/10.1039/D1EM00465D)).

EPA’s 2026 interim guidance does not endorse ordinary pyrolysis or sewage-sludge incineration as universally demonstrated PFAS destruction. It describes pyrolysis as promising but calls for characterization of biochar, gas, products of incomplete combustion, and products of incomplete destruction; for some permitted hazardous-waste combustion cases it discusses >1,100 °C, good mixing, and adequate residence rather than treating one temperature as transferable to all units ([EPA 2026 guidance](https://www.epa.gov/system/files/documents/2026-04/2026-interim-guidance-on-pfas-destruction-and-disposal.pdf)).

---

## 4. What happens after soil application?

Two different questions are often conflated:

1. Is a **waste-derived char itself** sufficiently free of PFAS for the proposed use?
2. Can a **selected clean biochar sorbent** reduce mobility of PFAS already in soil or water?

A “yes” to the second does not rescue a contaminated product under the first.

### 4.1 Leaching from biosolids-amended soil

Undisturbed Wisconsin soil columns receiving biosolids showed PFAS leaching, and adding biochar reduced leaching of several longer-chain PFAS by about **40–64%**; the effect was compound- and soil-dependent, and legacy soil PFAS complicated interpretation ([Holly et al. 2024](https://doi.org/10.1021/acsestwater.3c00414); [open dataset](https://doi.org/10.5061/dryad.59zw3r2dg)).

This is evidence for mitigation, not zero release. Preferential flow, dissolved organic matter, saturation, amendment mixing, and antecedent contamination can all bypass or compete with sorption sites ([Holly et al. 2024](https://doi.org/10.1021/acsestwater.3c00414)).

### 4.2 Activated biochar as a stabilizing amendment

In a low-total-organic-carbon soil, activated waste-timber biochar at ≥0.5% reduced measured PFAS leaching by >90%; at 1–5%, reductions exceeded 98% for PFBS, PFHxS, PFOS, PFHxA, and PFOA, while PFBA reduction remained lower (>79%). In a high-organic-carbon soil, performance ranged **23–100%** and generally required the 5% dose ([Sørmo et al. 2021](https://doi.org/10.1016/j.scitotenv.2020.144034)).

Activated carbon-like surface area and pore structure matter. Unactivated commodity biochar should not inherit performance claims from a steam/CO₂-activated product made near 900 °C ([Sørmo et al. 2021](https://doi.org/10.1016/j.scitotenv.2020.144034)).

### 4.3 Plant uptake

A one-year soil–lettuce–rainfall study using 2% and 4% biochar reported **62.1–94.9%** immobilization of PFOA in amended topsoil and lower leaching and plant uptake over 360 days; increasing nonextractable residues raised the separate question of long-term reversibility and bioavailability ([Fu et al. 2025](https://doi.org/10.1016/j.jhazmat.2025.139101)).

A field trial in PFAS-contaminated soil used woody biochar at **80 t ha⁻¹**. Relative to unamended plots, tomato leaves had 70% lower PFBS, 45% lower PFHpA, and 84% lower PFOA; tomato-fruit PFBA was 61% lower. Red-chicory responses were smaller or time-dependent, illustrating that crop and compound matter ([Ranzani et al. 2025](https://doi.org/10.3390/soilsystems9030100)).

Do not generalize these dose-specific trials to ordinary agronomic rates or all PFAS. Lower uptake may reflect sorption, dilution, growth effects, root distribution, or changed soil chemistry, and the sorbed inventory remains in the soil–biochar system.

### 4.4 Long-term containment uncertainty

Carbon amendments may age, clog, fragment, oxidize, or experience competition from dissolved organic matter. A multi-year field study found that amendment performance persisted overall but short-chain retention weakened with time, and a 2026 aging study found biochar more sensitive than activated carbon to property change ([Sørmo et al. 2026](https://doi.org/10.1016/j.jhazmat.2026.142119); [aging study](https://doi.org/10.1016/j.jhazmat.2026.142258)).

A remediation plan therefore needs monitoring endpoints for leachate/groundwater and crops, not only an initial batch-sorption result. See [[Soil and Agriculture]] and [[On-farm Trial Design]] for trial structure, while retaining PFAS-specific analytical controls from this chapter.

---

## 5. Testing biochar and the whole process

### 5.1 EPA Method 1633A: the primary targeted method

EPA Method 1633A (December 2024, EPA 820-R-24-007) uses isotope-dilution LC-MS/MS for **40 PFAS** in aqueous samples, soils, sediments, biosolids, other solids, and fish/shellfish tissue. For a biochar, confirm the laboratory treats the material as a solid and validates extraction, cleanup, dilution, recovery, and reporting limits for that high-carbon/high-ash matrix ([EPA Method 1633A](https://www.epa.gov/system/files/documents/2024-12/method-1633a-december-5-2024-508-compliant.pdf)).

Method 1633A answers: “How much of these 40 compounds did the method recover?” It does not answer: “How much total fluorinated organic matter exists?”

### 5.2 Methods that should not be casually substituted

- EPA Methods **533** and **537.1** are drinking-water methods, not validated solid/biochar methods ([EPA drinking-water laboratory methods](https://www.epa.gov/pfas/epa-pfas-drinking-water-laboratory-methods)).
- SW-846 Method **8327** addresses selected PFAS in nonpotable aqueous matrices; EPA removed solid-matrix references because compatible preparation was not validated ([EPA Method 8327 response to comments](https://www.epa.gov/system/files/documents/2021-07/final-response-to-comments-update-vii-methods-3512-and-8327.pdf)).
- EPA Method **1621** measures adsorbable organic fluorine in **aqueous** matrices by combustion ion chromatography. It can complement targeted analysis for process water but is not a ready-made biochar-solids method ([EPA Method 1621](https://www.epa.gov/system/files/documents/2024-01/method-1621-for-web-posting.pdf)).

### 5.3 Complementary tools

| Tool | Why use it | Main limitation |
|---|---|---|
| Method 1633A target panel | Comparable quantitation of 40 named PFAS in solids/liquids | Target list is finite ([EPA](https://www.epa.gov/system/files/documents/2024-12/method-1633a-december-5-2024-508-compliant.pdf)) |
| TOP assay | Reveals oxidizable precursors as increases in terminal PFAAs | Does not identify every precursor and can be matrix-sensitive ([McNamara et al. 2023](https://doi.org/10.1039/D2EW00677D)) |
| EOF/AOF/TOF or combustion ion chromatography | Indicates a broader fluorine gap | Includes different organofluorines; method/matrix definitions differ ([Edirisinghe et al. 2026](https://doi.org/10.1021/acs.est.5c17517)) |
| Inorganic fluoride | Supports defluorination/mineralization balance | HF/fluoride may partition into scrubbers, solids, or corrosion products ([Longendyke et al. 2022](https://doi.org/10.1039/D1EM00465D)) |
| Nontarget/high-resolution MS | Searches for unexpected transformation products | Identification confidence and quantitation vary ([Munoz et al. 2022](https://doi.org/10.1021/acs.est.1c03697)) |
| OTM-45 / OTM-50 stack methods | Characterize semivolatile and volatile fluorinated air emissions | Specialized and not a substitute for all-stream fluorine balance ([EPA 2026 guidance](https://www.epa.gov/system/files/documents/2026-04/2026-interim-guidance-on-pfas-destruction-and-disposal.pdf)) |

### 5.4 Sampling and QA/QC

PFAS work is vulnerable to both contamination and poor extraction. Method 1633A specifies isotope standards, blanks, spikes, recoveries, cleanup, calibration, holding, and quality-control acceptance. Project plans should also avoid fluoropolymer contact materials where they can bias the analytes of interest and should use lab-supplied containers and matrix-specific instructions ([EPA Method 1633A](https://www.epa.gov/system/files/documents/2024-12/method-1633a-december-5-2024-508-compliant.pdf)).

For a production campaign, collect paired and time-aligned samples of:

1. incoming feed before drying;
2. dryer condensate and dried feed;
3. char and entrained fines/dust;
4. aqueous condensate and organic py-oil separately;
5. raw pyrolysis gas where feasible;
6. thermal-oxidizer inlet and outlet;
7. scrubber liquor and spent air-pollution-control media;
8. ash/deposits; and
9. final product lots released to market.

A nondetect should always travel with the sample dry mass, preparation, reporting limit, detection limit, recovery, dilution, and list of analytes. The commercial pilot’s “no PFAS detected” result, for example, supported a bounded target-panel conclusion and explicitly did not cover nontarget PFAS or all incomplete-combustion products ([Thoma et al. 2022](https://pmc.ncbi.nlm.nih.gov/articles/PMC9128340/)).

---

## 6. What standards do—and do not—say

### 6.1 ANSI/ASABE/USBI S668

[[Biochar Lab Measurement Standard|standardizes biochar lab testing]] is a **methods standard**, not a product certificate or regulatory limit. Section 12.1.4 says PFAS are more likely in biochar from high-PFAS feedstocks such as wastewater-treatment biosolids, recommends periodic analysis for such feeds, and points to EPA Method 1633A. It sets no PFAS pass/fail number and tells users to consult applicable jurisdictional guidance ([S668 PDF](https://biochar.org/wp-content/uploads/2026/05/ANSI-S668.pdf)).

This is the most direct current biochar-standard PFAS language in the vault. Pair it with [[Testing EBC IBI S668]] for sampling and the wider analytical package.

### 6.2 European Biochar Certificate (EBC)

EBC Standard 10.5E allows sewage sludge only for **EBC-Basic**, subject to a worker-safety treatment plan and pyrolysis above **500 °C for at least 3 minutes**; the standard says metals normally prevent Agro/Urban soil uses ([EBC 10.5E §4.9](https://www.european-biochar.org/media/doc/7/ebc_en_10_5_red.pdf)).

EBC 10.5E does **not** name PFAS/PFOA/PFOS or set a PFAS limit; its explicit contaminant tables address metals, PAHs, PCBs, PCDD/F, and other class-specific parameters ([EBC 10.5E](https://www.european-biochar.org/media/doc/7/ebc_en_10_5_red.pdf)). The >500 °C/3 min biosolids condition must not be rebranded as demonstrated PFAS destruction.

### 6.3 IBI

The IBI Biochar Standard was retired in **April 2024** and will not be updated further ([IBI process/history PDF](https://biochar-international.org/wp-content/uploads/2024/07/IBI_Biochar_Standards_Process_History-1.pdf)). Legacy IBI criteria should not be presented as a current PFAS standard; the retired document did not supply the current S668/1633A framework.

### 6.4 Carbon-credit documents

Do not imply that a carbon certificate independently verifies PFAS unless the named methodology or incorporated product standard explicitly requires that test. Carbon permanence, lifecycle accounting, and PFAS product safety are separate evidence tracks. This chapter therefore links standards only where they actually contain PFAS or feedstock-contaminant language; see [[Product Standards EBC IBI]] for the broader standards hierarchy.

---

## 7. U.S. regulatory and guidance context

> This section summarizes documents as of 2026-09-16; it is not legal advice. Facility permits, waste classification, product registration, land-application rules, air requirements, and cleanup duties are jurisdiction- and fact-specific.

### 7.1 Federal biosolids documents

EPA released a **draft** sewage-sludge risk assessment for PFOA and PFOS in January 2025. It models certain highly exposed farm and disposal scenarios, identifies potential risks even at low biosolids concentrations in some scenarios, and treats incineration qualitatively because emissions data were insufficient. It is a risk assessment, not a regulation or universal safe concentration ([EPA FAQ](https://www.epa.gov/biosolids/frequent-questions-and-answers-draft-sewage-sludge-risk-assessment-pfoa-and-pfos); [draft assessment PDF](https://www.epa.gov/system/files/documents/2025-01/draft-sewage-sludge-risk-assessment-pfoa-pfos.pdf)).

EPA’s July 2026 **draft voluntary guidance** recommends source identification/reduction and risk-management practices for PFOA/PFOS in biosolids; it clarifies that **1 ppb** was a modeling starting point, not a regulatory threshold or “safe” cutoff. Public comments were scheduled through **October 5, 2026** ([EPA draft-guidance page](https://www.epa.gov/biosolids/draft-guidance-reducing-risk-perfluorooctanoic-acid-pfoa-and-perfluorooctane-sulfonic); [Federal Register notice](https://www.federalregister.gov/documents/2026/07/06/2026-13615/draft-guidance-for-reducing-risk-from-perfluorooctanoic-acid-pfoa-and-perfluorooctane-sulfonic-acid)).

### 7.2 Destruction/disposal guidance

EPA’s 2026 interim PFAS destruction/disposal guidance evaluates thermal treatment, landfills, and underground injection. For pyrolysis, it calls for testing of feed, char, gas, air-control residues, products of incomplete combustion, and products of incomplete destruction; it does not establish a universal validated pyrolysis operating window ([EPA 2026 interim guidance](https://www.epa.gov/system/files/documents/2026-04/2026-interim-guidance-on-pfas-destruction-and-disposal.pdf)).

### 7.3 CERCLA and drinking water are separate layers

PFOA and PFOS, including salts and structural isomers, became CERCLA hazardous substances effective **July 8, 2024**; releases at or above the reportable quantity of **1 pound in 24 hours** can trigger federal reporting. This is not a biochar product limit ([EPA CERCLA designation](https://www.epa.gov/superfund/designation-perfluorooctanoic-acid-pfoa-and-perfluorooctanesulfonic-acid-pfos-cercla)).

The federal drinking-water MCLs for PFOA and PFOS are **4.0 ng L⁻¹ (ppt)** each. Those water limits are useful exposure context but cannot be converted directly into a permissible ng g⁻¹ biochar concentration without a validated leaching/exposure model and applicable legal authority ([EPA PFAS drinking-water page](https://www.epa.gov/sdwa/and-polyfluoroalkyl-substances-pfas)).

### 7.4 States vary substantially

- **Maine** ended land application of sludge, biosolids, and sludge-derived products in 2022 rather than relying on a concentration screen ([Maine DEP PFAS page](https://www.maine.gov/dep/spills/topics/pfas/)).
- **Michigan’s** interim biosolids strategy uses PFOS/PFOA concentration bands: <20 µg kg⁻¹ with no additional PFAS restrictions; 20 to <100 µg kg⁻¹ with reduced application and added controls; and ≥100 µg kg⁻¹ treated as industrially impacted and not eligible for land application under the strategy ([Michigan EGLE interim strategy](https://www.michigan.gov/egle/about/organization/water-resources/biosolids/pfas-related/interim-strategy)).

These examples demonstrate why “U.S.-compliant” is too vague. A biochar decision needs the state, use, product/waste status, source material, and date of the applicable document.

---

## 8. European Union and international context

### 8.1 EU fertilising products

Under Commission Delegated Regulation (EU) **2021/2088**, Component Material Category 14 for pyrolysis and gasification materials excludes sewage sludge, industrial sludge, and dredging sludge as eligible inputs. A sewage-sludge char therefore does not become an EU CMC 14 fertilising-product component merely because it was pyrolyzed ([EUR-Lex 2021/2088](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A32021R2088)).

This EU market-access rule is separate from EBC-Basic certification, national waste rules, and evidence of PFAS destruction.

### 8.2 POP restrictions and broader PFAS policy

PFOS is listed for restriction under Annex B of the Stockholm Convention; PFOA and PFHxS families are listed for elimination under Annex A, subject to the Convention’s specific terms ([Stockholm Convention PFAS overview](https://www.pops.int/Implementation/IndustrialPOPs/PFAS/Overview/tabid/5221/Default.aspx); [all POP listings](https://www.pops.int/TheConvention/ThePOPs/AllPOPs/tabid/2509/Default.aspx)). EU POPs controls implement restrictions on these named families, but they are not a harmonized “total PFAS in biochar” limit ([EU POPs Regulation consolidated text](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A02019R1021-20250804)).

As of this chapter’s date, the proposed broad EU/EEA PFAS restriction remained under ECHA evaluation rather than being a final universal biochar limit ([ECHA PFAS restriction page](https://echa.europa.eu/hot-topics/perfluoroalkyl-chemicals-pfas)).

---

## 9. Greenwashing-adjacent claims and better wording

| Weak or overbroad claim | Why it fails | Evidence-bounded replacement |
|---|---|---|
| “Pyrolysis destroys PFAS.” | Ignores temperature, residence, matrix, off-gas, liquids, and analyte scope | “Under the stated conditions, the system achieved X% removal of Y target PFAS across sampled streams; unmeasured organofluorine remains a limitation.” |
| “PFAS-free biochar.” | “Nondetect” depends on method, target list, sample mass, recovery, and reporting limit | “None of the 40 Method 1633A analytes was detected above compound-specific reporting limits in this lot.” |
| “800 °C guarantees destruction.” | Set point alone does not establish particle history, gas residence, oxygen, or fluorine mineralization | Report actual temperature distribution, residence, off-gas treatment, and full sampling plan ([EPA 2026 guidance](https://www.epa.gov/system/files/documents/2026-04/2026-interim-guidance-on-pfas-destruction-and-disposal.pdf)). |
| “99% removed from char.” | Could mean transfer to oil or gas | Say “solid-phase removal,” then report liquid/gas/fluorine closure ([McNamara et al. 2023](https://doi.org/10.1039/D2EW00677D)). |
| “Biochar remediates PFAS permanently.” | Sorption is reversible/age-dependent and short chains are less retained | Say “reduced leaching by X% for named PFAS over Y duration at Z dose,” with monitoring ([Sørmo et al. 2021](https://doi.org/10.1016/j.scitotenv.2020.144034)). |
| “Certified biochar means PFAS tested.” | EBC 10.5E has no PFAS parameter; S668 is methods-only | Name the certificate and attach the separate PFAS report ([EBC 10.5E](https://www.european-biochar.org/media/doc/7/ebc_en_10_5_red.pdf); [S668](https://biochar.org/wp-content/uploads/2026/05/ANSI-S668.pdf)). |
| “Meets the EPA 1-ppb limit.” | EPA says 1 ppb in its draft assessment was a modeling starting point, not a federal limit | Identify the actual state/federal document and legal status ([EPA 2026 draft guidance](https://www.epa.gov/biosolids/draft-guidance-reducing-risk-perfluorooctanoic-acid-pfoa-and-perfluorooctane-sulfonic)). |

### A practical claim ladder

From weakest to strongest evidence:

1. **Parent not detected in one char sample.**
2. **Target panel not detected in replicated char lots with adequate reporting limits.**
3. **Yield-corrected targeted mass balance across feed, char, oil, water, gas, and residues.**
4. **Target + precursor + nontarget + organic-fluorine/inorganic-fluoride closure.**
5. **The same package under steady state, startup, shutdown, and upset conditions at commercial scale.**
6. **Independent replication plus exposure/end-use monitoring.**

Most published pyrolysis studies sit between levels 2 and 4; the 2024 thermal-oxidizer study advanced whole-train target accounting but still identified recombination and unmeasured products as gaps ([Winchell et al. 2024](https://doi.org/10.1002/wer.11149)).

---

## 10. Procurement, operations, and release checklist

### Feedstock acceptance

- Map industrial, landfill-leachate, paper-coating, AFFF, and impacted-farm inputs.
- Require chain of custody and representative lot sampling.
- Use Method 1633A for suspect solids and retain samples for later nontarget/fluorine work ([EPA Method 1633A](https://www.epa.gov/system/files/documents/2024-12/method-1633a-december-5-2024-508-compliant.pdf)).
- Do not blend a high result with clean feed merely to dilute below a reporting or policy threshold.

### Process validation

- Record feed moisture, throughput, reactor-zone temperatures, solids and gas residence distributions, pressure, oxygen, and char yield.
- Include drying and condensate in the system boundary.
- Validate thermal oxidizer temperature, oxygen, turbulence/mixing, and residence at real load.
- Sample startup, steady operation, shutdown, bypass, and representative upset conditions consistent with EPA’s call for facility-specific thermal testing ([EPA 2026 guidance](https://www.epa.gov/system/files/documents/2026-04/2026-interim-guidance-on-pfas-destruction-and-disposal.pdf)).

### Product release

- Pair PFAS with the broader contaminant package: [[PAHs]], [[Heavy Metals and Ash]], PCBs/PCDD/F where triggered, pH/EC, and agronomic properties.
- State sample basis, method, target list, reporting limits, recoveries, date, and jurisdiction.
- Keep waste-derived char segregated until analytical and end-use review is complete.
- If the char is intended as a PFAS sorbent, document sorption/leaching performance for the actual soil, water, dose, PFAS mixture, and duration rather than relying on generic “biochar” literature.

### Decision gate

| Situation | Minimum defensible response |
|---|---|
| Clean, traceable wood/crop residual | Risk-based periodic verification; do not claim “PFAS-free” without data |
| Compost or paper-rich mixed residual | Supplier controls + lot testing; investigate coated paper and industrial inputs |
| Municipal biosolids | Routine Method 1633A + precursor/fluorine research package + whole-train validation |
| Industrially impacted biosolids | Treat as high-risk; test at feed acceptance and validate higher-severity treatment/off-gas control |
| AFFF-site biomass or remediation residual | Manage as contaminated treatment feed; no soil release based on char nondetect alone |
| Biochar used to immobilize PFAS | Verify clean sorbent, leaching reduction, short-chain performance, aging, and monitoring |

---

## 11. Research gaps

1. **Fluorine closure.** Many studies report tens of target compounds while thousands of PFAS and other organofluorines may exist; the difference between 81% TOF reduction and 12% EOF reduction in a 2026 byproduct study shows that analytical definition can dominate the conclusion ([Edirisinghe et al. 2026](https://doi.org/10.1021/acs.est.5c17517)).
2. **Commercial residence distributions.** Bench solids residence of ~1 h at 600 °C is not representative of every screw, rotary, or fluidized-bed unit ([Rathnayake et al. 2025](https://doi.org/10.1016/j.jaap.2025.106970)).
3. **Startup and upset emissions.** Most datasets emphasize steady operation; bypass and cold-zone condensation can control real emissions ([EPA 2026 guidance](https://www.epa.gov/system/files/documents/2026-04/2026-interim-guidance-on-pfas-destruction-and-disposal.pdf)).
4. **Ultrashort PFAS and volatile products.** Standard target panels may miss TFA, volatile fluorocarbons, COF₂, and other products ([Longendyke et al. 2022](https://doi.org/10.1039/D1EM00465D)).
5. **Matrix effects.** Industrial load, ash/minerals, moisture, organic carbon, and conversion efficiency can change removal at the same nominal temperature ([McNamara et al. 2026](https://doi.org/10.1002/wer.70352)).
6. **Field-scale containment life.** Biochar aging and weaker short-chain retention need multi-year monitoring under unsaturated flow and real crop rotations ([Sørmo et al. 2026](https://doi.org/10.1016/j.jhazmat.2026.142119)).
7. **Toxicity of mixtures and transformation products.** Parent loss is not enough when toxicity and exposure data for many products are absent ([Longendyke et al. 2022](https://doi.org/10.1039/D1EM00465D)).
8. **Validated biochar-specific extraction.** Method 1633A covers solids, but high-carbon/high-ash chars need documented matrix spikes, dilution, and cleanup performance ([EPA Method 1633A](https://www.epa.gov/system/files/documents/2024-12/method-1633a-december-5-2024-508-compliant.pdf)).
9. **Regulatory harmonization.** S668 has a method but no limit; EBC has no PFAS parameter; U.S. state biosolids policies vary; EU CMC 14 excludes sewage sludge ([S668](https://biochar.org/wp-content/uploads/2026/05/ANSI-S668.pdf); [EBC](https://www.european-biochar.org/media/doc/7/ebc_en_10_5_red.pdf); [EU 2021/2088](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A32021R2088)).

---

## 12. Bottom line

- For **biosolids or suspect waste feedstocks**, design PFAS control as a whole-plant mass-balance problem. A low char result is necessary for soil use but cannot establish destruction by itself.
- Evidence across 400–800 °C shows strong solid-phase removal is possible, while the 500 °C industrially impacted result, py-liquid transformation, and short-chain stack residuals rule out a universal temperature guarantee ([McNamara et al. 2026](https://doi.org/10.1002/wer.70352); [McNamara et al. 2023](https://doi.org/10.1039/D2EW00677D); [Winchell et al. 2024](https://doi.org/10.1002/wer.11149)).
- For **remediation**, selected activated biochars can sharply reduce leaching and crop uptake, especially for longer-chain PFAS, but they immobilize an inventory that needs long-term monitoring ([Sørmo et al. 2021](https://doi.org/10.1016/j.scitotenv.2020.144034)).
- For **testing**, begin with Method 1633A and then close the blind spots with precursor, nontarget, organic-fluorine, inorganic-fluoride, and air-emission measurements appropriate to the claim.
- For **communications**, report exactly which compounds, phases, methods, conditions, limits, and jurisdiction support the statement. Avoid “PFAS-free,” “complete destruction,” or “certified safe” unless the evidence actually reaches that level.

---

## Primary sources and official documents

### Thermal fate and process studies

- McNamara et al. (2023), py-liquid transfer and transformation — https://doi.org/10.1039/D2EW00677D
- Thoma et al. (2022), commercial pilot target-PFAS study — https://doi.org/10.1080/10962247.2021.2009935
- Sørmo et al. (2023), wastes, char, and stack emissions — https://doi.org/10.1016/j.jhazmat.2023.131447
- Hušek et al. (2024), 200–700 °C sludge/sand and organic fluorine — https://doi.org/10.1007/s42773-024-00322-5
- Winchell et al. (2024), pyrolysis plus thermal oxidizer — https://doi.org/10.1002/wer.11149
- Rathnayake et al. (2025), biosolids co-pyrolysis at 600 °C — https://doi.org/10.1016/j.jaap.2025.106970
- McNamara et al. (2026), industrial-impact and temperature comparison — https://doi.org/10.1002/wer.70352
- Hakeem et al. (2026), fluidized-bed pilot — https://doi.org/10.1016/j.jaap.2025.107343
- Edirisinghe et al. (2026), complementary fluorinated-organic analyses — https://doi.org/10.1021/acs.est.5c17517
- Longendyke et al. (2022), thermal fate/destruction review — https://doi.org/10.1039/D1EM00465D

### Soil, leaching, and plant uptake

- Sørmo et al. (2021), activated-biochar stabilization — https://doi.org/10.1016/j.scitotenv.2020.144034
- Holly et al. (2024), biosolids and undisturbed soil columns — https://doi.org/10.1021/acsestwater.3c00414
- Fu et al. (2025), one-year PFOA soil–plant–leaching study — https://doi.org/10.1016/j.jhazmat.2025.139101
- Ranzani et al. (2025), tomato and red-chicory field trial — https://doi.org/10.3390/soilsystems9030100
- Sørmo et al. (2026), unsaturated field performance — https://doi.org/10.1016/j.jhazmat.2026.142119
- Critical remediation review — https://doi.org/10.1016/j.scitotenv.2024.174962

### Standards, methods, and policy

- EPA Method 1633A — https://www.epa.gov/system/files/documents/2024-12/method-1633a-december-5-2024-508-compliant.pdf
- ANSI/ASABE/USBI S668 — https://biochar.org/wp-content/uploads/2026/05/ANSI-S668.pdf · [[Biochar Lab Measurement Standard|standardizes biochar lab testing]]
- EPA 2026 destruction/disposal guidance — https://www.epa.gov/system/files/documents/2026-04/2026-interim-guidance-on-pfas-destruction-and-disposal.pdf
- EPA 2025 draft sewage-sludge risk assessment — https://www.epa.gov/system/files/documents/2025-01/draft-sewage-sludge-risk-assessment-pfoa-pfos.pdf
- EPA 2026 draft biosolids guidance — https://www.epa.gov/biosolids/draft-guidance-reducing-risk-perfluorooctanoic-acid-pfoa-and-perfluorooctane-sulfonic
- EBC Standard 10.5E — https://www.european-biochar.org/media/doc/7/ebc_en_10_5_red.pdf
- EU Delegated Regulation 2021/2088 — https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A32021R2088
- IBI standards history/retirement — https://biochar-international.org/wp-content/uploads/2024/07/IBI_Biochar_Standards_Process_History-1.pdf

## Related notes

- [[Contaminants and Quality]] · [[Testing EBC IBI S668]] · [[PAHs]] · [[Heavy Metals and Ash]]
- [[Feedstocks]] · [[Woody vs Manure Ag Feedstocks]] · [[Pyrolysis Systems and Temperatures]] · [[Biochar Quality from Process]]
- [[Biochar vs Activated Carbon]] · [[Soil and Agriculture]] · [[Biochar Compost and Manure Blends]] · [[On-farm Trial Design]]
- [[Product Standards EBC IBI]] · [[Biochar Lab Measurement Standard|standardizes biochar lab testing]] · [[Risks and Controversies]] · [[Production Hub]] · [[Key Sources]]
