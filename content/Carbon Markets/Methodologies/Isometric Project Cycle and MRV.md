---
tags: [carbon-markets, mrv, isometric, project-cycle]
aliases: [Isometric MRV, Isometric project cycle, Isometric CoC]
updated: 2026-09-16
---

# Isometric Project Cycle and MRV

**Parent hub:** [[Isometric Biochar Protocol]]  
**Permanence:** [[Isometric Permanence Pathways 200y and 1000y]]  
**Modules:** [[Isometric Modules Soil Built Burial]]  
**Generic:** [[MRV Stack]]  
**Compare:** [[Puro Project Cycle and MRV]] · [[Verra VM0044 Project Cycle and MRV]]

Primary sources: [Biochar Production and Storage v1.3](https://registry.isometric.com/protocol/biochar/1.3); [Soil Environments v1.3](https://registry.isometric.com/module/biochar-storage-soil-environments/1.3).

---

## End-to-end cycle

```
PDD (protocol + modules + ESS + additionality)
        ↓
Validation (Isometric-approved VVB; site visits)
        ↓
Produce → characterize (Method A/B) → store
        ↓
Reporting Period GHG Statement
        ↓
Verification (ex-post after durable storage)
        ↓
Credit issuance on Isometric Registry / Certify
        ↓
Transfer / retirement (± buffer contribution if applicable)
```

**Critical rule:** Credits issued **only after** CO₂ is durably stored — not at factory gate alone ([protocol](https://registry.isometric.com/protocol/biochar/1.3)).

---

## Documentation & validation

| Artifact | Role |
|---|---|
| **PDD** | Locations (biomass, pyrolysis, storage); feedstock counterfactual; reactor design diagrams; characterization plan; models; ESS |
| **GHG Statement** | Net removal quantification for Reporting Period |
| **VVB** | Validate feedstock module; verify storage module; verify quantification; ESS; Isometric Standard compliance |
| **Materiality** | **5%** threshold (protocol) |
| **Uncertainty** | Sensitivity analysis; parameters <1% impact may be omitted from uncertainty analysis |

### Site visits

Minimum: site visits during first Validation/Verification to **biomass pyrolysis site** and **biochar application site** (ISO 14064-3 framing). Representative sampling of multiple application sites allowed ([protocol](https://registry.isometric.com/protocol/biochar/1.3)).

---

## Batches and sampling

| Concept | Rule |
|---|---|
| Production batch | Project-defined but **≤ 1 month**; consistent feedstock/process |
| Storage batch | One or multiple production batches blended before storage |
| **Method A** | Sample every batch (≥3 samples preferred) until statistical basis for Method B |
| **Method B** | After ≥ **30** samples (example: 3×10 batches), conservative mean − SEM for unsampled; refresh every ≤10 batches; 6-month sample eligibility window |
| Outliers (Method B) | Winsorize beyond ±3σ after ≥30 measurements |

Mass: preferred **weighbridge** at delivery; alternative documentation only with Isometric pre-approval. Retain carbon analyses and scale tickets ≥ **5 years** after monitoring period.

---

## Pyrolysis emissions MRV

Two quantification options ([protocol §10](https://registry.isometric.com/protocol/biochar/1.3)):

1. **Direct continuous measurement** of flow + composition (CH₄, N₂O, CO, CO₂) upstream of emission point — preferred  
2. **Accredited periodic emissions testing** (≥ annually) when continuous not feasible  

Permissible gas end-uses: venting; venting after control system; combustion for process energy; provision to third party (allocation rules). N₂O concern elevated for low C/N feedstocks (manure, biosolids, seaweed) — justify if not monitoring.

Reactor design diagrams, materials, pressure-vessel standards (e.g., 2014/68/EU), and maintenance plans required in PDD.

Production variants: mobile / distributed / combustion co-product modules referenced in protocol §9.

---

## End-use proof & chain of custody (soil)

From [soil module §8](https://registry.isometric.com/module/biochar-storage-soil-environments/1.3):

### Direct soil application

- Geotagged photos/videos: stockpile, spreading, incorporation  
- GIS / maps of application boundaries + dated quantity logs  

### Mixing with organic matrices (crediting at mix + transfer)

- Biochar **< 50% v/v** of final product; product unsuitable as fuel  
- Defined eligible end-use pathway  
- Verified transfer of custody to third party  
- Burden of proof that product goes to land (not incineration-dominant jurisdictions without soil proof)  

### Third-party sales

- Purchaser affidavit (intended use, geography for soil-T conservatism, evidence retention)  
- Invoices / BOLs / delivery proof  
- Mixing process evidence  

### CoC hygiene

- Unique batch IDs  
- Documentation at every handoff  
- Retain records ≥ **5 years**  
- Stockpile ≤ **12 months** unless agreed; store wet/covered; keep away from waterways  

Fuel-diversion risk: if material picking risk is non-negligible, ≥95% by weight ≤ **10 mm** particle size (module).

---

## Additionality dynamics

- Project-specific baseline/counterfactual per Isometric Standard  
- Reassess when regulations or financials change (tipping fees, farmer payments, cheaper capital, co-product revenue)  
- Finding of non-additionality **stops future crediting only** — does not claw back past/current periods ([protocol](https://registry.isometric.com/protocol/biochar/1.3))  

Contrast Verra v1.2 VT0008 investment analysis + activity method ([[Verra VM0044 Project Cycle and MRV]]); Puro facility/output audits ([[Puro Project Cycle and MRV]]).

---

## Data transparency

Evidence for quantification and ESS generally public on Isometric’s platform (PDD, GHG Statement, measurements, EFs, literature, permits). Limited confidential carve-outs (e.g., licensed EF databases) with buyer/registry/VVB access ([protocol Data Sharing](https://registry.isometric.com/protocol/biochar/1.3)).

---

## Buffer contributions (by module)

| Module | Typical buffer framing |
|---|---|
| Soil Environments | **0%** (No Observable Risk; discount in \(F_{durable}\)) |
| Low Oxygen Burial | **0%** (same framing) |
| Built Environment | **2%** (Very Low Risk) |

Confirm live project pages for actual buffer pool contributions (e.g., Charm registry counters).

---

## Example projects (MRV archetypes)

| Archetype | Project | MRV flavor | Source |
|---|---|---|---|
| Soil / land application | Charm Range & Plains | Biochar trucked to land application sites | [registry](https://registry.isometric.com/project/prj_1JN6XNWDQ1S0BSN7) |
| Landfill burial | Carba Burnsville | Daily cover → low-oxygen burial; Microsoft offtake | [registry](https://registry.isometric.com/project/prj_1JRZWM3BP1S071QG); [Carba](https://carba.com/press/carba-announces-5-year-carbon-removal-credit-purchase-agreement-with-microsoft) |

---

## US producer practical path

1. Choose storage module early (soil vs burial vs built) — locks lab suite (Ro or not)  
2. Define production batch ≤ 1 month; write Method A→B sampling plan into PDD  
3. Contract ISO 17025 labs; if pursuing 1000y, secure petrography (≥500 R₀ points) + TGA  
4. Instrument pyrolysis emissions (continuous or accredited annual)  
5. Build geotag / GIS / affidavit CoC **before** first offtake season  
6. Allocate credit ownership contractually across feedstock, pyrolyzer, applicator  
7. Budget VVB site visits to both plant and fields/landfill  

Ag adjacency: [[Soil and Agriculture]] · [[Application Rates and Methods]] · [[Soil Carbon Amendment and US Ag|NRCS soil carbon amendment in US ag]] (policy, not Isometric MRV).

---

## Primary links

- [Protocol v1.3](https://registry.isometric.com/protocol/biochar/1.3)
- [Soil module v1.3](https://registry.isometric.com/module/biochar-storage-soil-environments/1.3)
- [Charm project](https://registry.isometric.com/project/prj_1JN6XNWDQ1S0BSN7)
- [Carba Burnsville](https://registry.isometric.com/project/prj_1JRZWM3BP1S071QG)

## Related notes

- [[Isometric Biochar Protocol]] · [[Isometric Permanence Pathways 200y and 1000y]] · [[Isometric Modules Soil Built Burial]]
- [[MRV Stack]] · [[Double Counting and Credit Ownership]] · [[Verra vs Isometric vs Puro]]
