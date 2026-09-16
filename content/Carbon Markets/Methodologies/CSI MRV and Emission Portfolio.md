---
tags: [carbon-markets, methodology, csi, mrv]
aliases: [CSI MRV, CSI emission portfolio, CSI dMRV, Global Biochar Tool]
updated: 2026-09-16
---

# CSI MRV and Emission Portfolio

Project-cycle, **emission portfolio**, offsetting rules, efficiency gates, and post-production **dMRV** under **[[CSI Global Biochar C-Sink]]** v3.3.

Primary: [4000039EN.pdf](https://www.carbon-standards.com/docs/transfer/4000039EN.pdf) Ch. 4–12 · [Formulas](https://www.carbon-standards.com/docs/transfer/4000115EN.pdf) · [service page](https://www.carbon-standards.com/en/standards/service-501~global-biochar-c-sink.html) · vault [[MRV Stack]].

---

## Lifecycle logic (industrial)

```
EBC/WBC product cert + batch analytics
        ↓
Emission portfolio (biomass → application) + MoS
        ↓
Offset portfolio (GPC for CO₂/N₂O; TCE-matched temporary for CH₄)
        ↓
dMRV track packaging units to eligible matrix / soil
        ↓
Register C-sink in Global C-Sink Registry (after validation)
```

CSI requires associated emissions **offset before** the C-sink is validated/usable for compensation ([v3.3 Summary & §1.2–1.3, Ch. 4](https://www.carbon-standards.com/docs/transfer/4000039EN.pdf)). That is a sharper “pay the footprint first” culture than buffer-pooled VCS issuance.

Prerequisite product layer: [[Product Standards EBC IBI]]. Permanence splits: [[CSI GPC vs SPC Permanence Classes]].

---

## What enters the emission portfolio (§4.2)

| Block | Content |
|---|---|
| Biomass provision | Production, processing, transport (Ch. 5.3 factors / positive list) |
| Biomass storage | Ch. 6 |
| Pyrolysis & site equipment | Ch. 7.1 (energy, fuels, CH₄ from unit) |
| Post-production → C-sink | Transport, processing, application (Ch. 10) |
| **Margin of safety** | Flat **20 kg CO₂e / t biochar DM** at producer factory gate |

Emissions logged separately as t CO₂, t N₂O, t CH₄. Emission factor = total expenditures / batch dry biochar mass ([§4.2](https://www.carbon-standards.com/docs/transfer/4000039EN.pdf)).

### GWP100 factors (v3.3)

| Gas | Factor | Note |
|---|---|---|
| N₂O | **298** | Geological offset required |
| Biogenic CH₄ | **27.0** | AR6; was 25 through v3.2 |
| Fossil CH₄ | **29.8** | AR6 |

Transition: contracts may still use GWP **25** until **1 January 2027** ([§4.4](https://www.carbon-standards.com/docs/transfer/4000039EN.pdf)).

---

## Offsetting rules (§4.3–4.4)

| Emission | Must be offset with | Rationale (CSI) |
|---|---|---|
| Fossil **CO₂** | **GPC** (geological C-sinks in registry) | Long radiative lifetime |
| **N₂O** | **GPC** | Long residence time |
| **CH₄** | Temporary C-sink delivering equal **TCE** within **5 ≤ H_del ≤ 20** years | Most CH₄ warming is near-term; geological GPC is “neither efficient nor adequate” for CH₄ |

Self-offsetting with the same batch’s registered sink is allowed once the portfolio is covered ([§4.3](https://www.carbon-standards.com/docs/transfer/4000039EN.pdf)).

**Order-of-magnitude CH₄ math (standard narrative):** ~**94.6 t CO₂e** stored constantly over 20 years offsets 1 t biogenic CH₄; using decaying **SPC** raises required initial removal to ~**122 t CO₂e** per t CH₄ ([§4.4](https://www.carbon-standards.com/docs/transfer/4000039EN.pdf)).

Figure 3 in the standard shows GPC partially retired to cover production fossil CO₂, residual GPC for CINK_1000+ sales, and SPC curve for temporary services.

---

## Margin of safety (§4.7)

- **20 kg CO₂e / t biochar (DM)** ≈ ~0.7% of biochar carbon  
- Applied at **producer factory gate**  
- **Not** reduced by pro-rata allocation  
- Covers unquantified Scope 3 (bags, servers, commuting, capital equipment, sampling imprecision, etc.)  
- Size reviewed at least every two years  

([§4.7](https://www.carbon-standards.com/docs/transfer/4000039EN.pdf))

---

## Pro-rata GHG attribution (§4.6)

When biochar is one of several marketable pyrolysis products, facility emissions may be split on an **energy (LHV)** basis (ISO 14040 framing) **if** non-biochar products generate income/value **≥ 30%** of biochar income.

- Feedstock drying heat used for the pyrolyzer itself stays with biochar  
- Emissions **after** biochar leaves the unit → 100% to biochar portfolio  
- Worked Box 6 example: biochar energy share **20.6%** of outputs → that share of CO₂/N₂O/CH₄ (excl. MoS mechanics as specified)

([§4.6](https://www.carbon-standards.com/docs/transfer/4000039EN.pdf))

---

## Fossil reduction plan & efficiency gates

### Fossil carbon reduction (§4.5 / §1.3)

Producers must maintain an **annual** fossil emission reduction plan (Global Biochar Tool or upload) covering biomass production → packaging at the facility (biogenic CH₄ from storage/pyrolysis excluded from the *fossil* plan; transport after gate is trader/processor responsibility).

| Deadline | Target (exec summary §1.3) |
|---|---|
| **2030** | Fossil emissions **< 100 kg CO₂e / t biochar** |
| **2035** | **< 20 kg CO₂e / t biochar** |

**Wording watch:** §4.5 body text says “per ton of **biochar-carbon**” while §1.3 and the energy chapter cross-ref say “per ton of **biochar**.” Until CSI clarifies, diligence both; vault default for checklists = **exec summary per ton biochar**.

### Energy-use efficiency (§8.2)

For each certified batch, **≥ 60%** of (feedstock LHV energy + process energy expenditures) must appear as used energy / beneficial products (heat, power, biochar LHV, pyro-oil, drying credit, marketed fuels, limited CCU credit, etc.). Failure → batch not C-Sink eligible.

### Carbon efficiency (§8.1)

Declared (sequestrable pyrolytic C / feedstock C); **no hard threshold** yet — transparency / additionality control that pyrolytic use does not replace a more C-efficient baseline.

---

## Feedstock additionality (pointer)

Ch. 5 sets carbon neutrality of biomass, additionality / baseline logic (prefer residues over primary wood that would have been long-lived timber), approved biomasses and default expenditures, and monitoring for perennial systems. Operational detail lives in the PDF + biomass positive lists; do not invent EF tables here — cite [v3.3 Ch. 5](https://www.carbon-standards.com/docs/transfer/4000039EN.pdf) and EBC biomass positive list ([4000095EN](https://www.carbon-standards.com/docs/transfer/4000095EN.pdf)).

---

## Post-production dMRV (Ch. 10–11)

| Requirement | Detail |
|---|---|
| Tracking | Every packaging unit labeled (QR); Batch ID, analytics link, production date, CO₂-removal year, owner, departure GPS, DM tons, C content, emission-portfolio link |
| Custody | Scan at destination; online ownership transfer confirmation |
| Soil consent | Landowner/tenant agrees soil is entry to geological storage (ToS / invoice OK); landowner need not be C-sink owner |
| Matrix end | Incorporation into approved matrix can end geographic tracking if oxidation loss is precluded |
| Tools | CSI-endorsed **dMRV** providers ([4000162EN](https://www.carbon-standards.com/docs/transfer/4000162EN.pdf)); may use own QR if linked to Global Biochar Tool batch page |
| Storage >1 year on site | May register as **temporary** C-sink (Ch. 12.6) |
| Processors / traders | Must be EBC/WBC certified as processor and/or trader; footprints enter portfolios |

**Dry matter:** on-site DM protocol per ≤ **10 m³** (or ≤7 big bags): ≥20 subsamples → ≥10 L; dry 110 °C ≥16 h (or endorsed LOD analyzer); round DM % to whole percent; label each unit with dry weight ([§9.2](https://www.carbon-standards.com/docs/transfer/4000039EN.pdf)).

**Geo-localization:** GPS in field for defined applications; photo with date/geolocation recommended ([Ch. 11](https://www.carbon-standards.com/docs/transfer/4000039EN.pdf)). Diffuse C-sinks: Ch. 11.2 + matrix list.

---

## Eligible applications (Ch. 12 snapshot)

| Use | Key rule |
|---|---|
| **Soil** | ≥ **50:50 vol** mix with soil/amendment (else temporary storage); high root-zone concentration OK if covered in agronomic context |
| **Animal farming** | Feed/bedding/manure additive OK if manure ultimately to soil; exclude energetic manure paths (horse/poultry caution); pet feed generally excluded |
| **Concrete / mineral construction** | Sink while structure exists; EoL landfill / recycle pathways detailed in §12.3 |
| **Asphalt / composites** | §12.4–12.5 + matrix positive list |
| **Other** | Only forms allowed by matrix positive list / §12.7 |

Matrix list: [4000078EN.pdf](https://www.carbon-standards.com/docs/transfer/4000078EN.pdf) (v4_17, 28 May 2026).

---

## Validation / verification culture

| Step | Actor | Notes |
|---|---|---|
| Product cert | EBC/WBC + endorsed lab + annual on-site | Prerequisite |
| Technical / C-sink controls | CSI tools + endorsed dMRV | Emission portfolio, efficiency, tracking |
| Validation & verification | Endorsed VVB (**CERES-CERT AG** highlighted) | PDD template on [service page](https://www.carbon-standards.com/en/standards/service-501~global-biochar-c-sink.html); public consultation while `Ongoing Validation` |
| Issuance / trade | Global C-Sink Registry; endorsed traders for transfer/retirement | [[CSI Overview]] |

Artisan track uses a distinct Manager endorsement → VVB path — [[CSI Overview]].

---

## Contrast with other BCR MRV cultures

| Theme | CSI | Puro | Verra | Isometric |
|---|---|---|---|---|
| Credit exists when… | C-sink registered **after portfolio offset** | After durable **eligible use** + Output Audit | After VCS V/V period | After **storage** verified |
| Product cert | **Mandatory** EBC/WBC | Characterization practice | Characterization practice | Characterization practice |
| Risk instrument | MoS + mandatory emission offsets | No default buffer % | VCS tools | Often 0% soil / small built buffer |
| CH₄ | Dedicated TCE temporary-sink rules | Method GHG accounting | Method GHG accounting | Method GHG accounting |

Deep peers: [[Puro Project Cycle and MRV]] · [[Verra VM0044 Project Cycle and MRV]] · [[Isometric Project Cycle and MRV]] · [[MRV Stack]].

---

## Primary links

- [C-Sink 3.3 PDF](https://www.carbon-standards.com/docs/transfer/4000039EN.pdf)
- [Formulas & EFs](https://www.carbon-standards.com/docs/transfer/4000115EN.pdf)
- [dMRV endorsement](https://www.carbon-standards.com/docs/transfer/4000162EN.pdf)
- [Matrix positive list](https://www.carbon-standards.com/docs/transfer/4000078EN.pdf)
- [Service page / PDD](https://www.carbon-standards.com/en/standards/service-501~global-biochar-c-sink.html)
- [Global C-Sink Registry](https://global-c-registry.org/)

## Related notes

- [[CSI Global Biochar C-Sink]] · [[CSI Overview]] · [[CSI GPC vs SPC Permanence Classes]]
- [[Product Standards EBC IBI]] · [[MRV Stack]] · [[Double Counting and Credit Ownership]]
- [[Carbon Markets Hub]] · [[Key Sources]]
