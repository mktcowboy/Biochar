---
tags: [carbon-markets, isometric, modules, soil, burial, built]
aliases: [Isometric soil module, Isometric burial, Isometric built environment biochar]
updated: 2026-09-16
---

# Isometric Modules Soil Built Burial

**Parent hub:** [[Isometric Biochar Protocol]]  
**Permanence math:** [[Isometric Permanence Pathways 200y and 1000y]]  
**MRV:** [[Isometric Project Cycle and MRV]]  
**Applications:** [[Soil and Agriculture]] · [[Materials and Built Uses]]

Isometric splits **where** biochar is stored into dedicated modules. Production stays under [Biochar Production and Storage v1.3](https://registry.isometric.com/protocol/biochar/1.3); durability and site rules live in the storage module.

---

## Module roster

| Module | Version (fetched 2026-09-16) | Durability framing | URL |
|---|---|---|---|
| **Soil Environments** | v1.3 | **200y** or **1000y** | https://registry.isometric.com/module/biochar-storage-soil-environments/1.3 |
| Agricultural Soils (earlier) | v1.1 | Same two-option logic | https://registry.isometric.com/module/biochar-storage-agricultural-soils/1.1 |
| **Low Oxygen Burial** | v1.1 | ≥ **1000y** | https://registry.isometric.com/module/biochar-storage-low-oxygen/1.1 |
| **Built Environment** | v1.0 (page may note newer) | **> 1000y** | https://registry.isometric.com/module/biochar-storage-built-environment/1.0 |

---

## Soil Environments v1.3

### Eligible land uses

Agricultural soils (FAO cropland / meadows / pasture), forestry soils, amenity/recreational land (parks, golf courses). Other environments (rangeland, horticulture, urban landscapes) possible with prior Isometric approval if risk ≤ agricultural soils and ESS met ([soil module](https://registry.isometric.com/module/biochar-storage-soil-environments/1.3)).

**Ineligible:** projects causing sustained net decrease in crop yields / land productivity.

### Chemistry & permanence

See [[Isometric Permanence Pathways 200y and 1000y]] — H/Corg < 0.5, O/Corg < 0.2, WBC contaminant ceilings, 200y Woolf path or 1000y Ro path.

### Safeguards

Application rates within local regulation; minimize dust; incorporate where appropriate; monitor N, pH, salts, WHC, nutrients; heavy-metal remediation plan if soils already elevated; stakeholder process for free distribution (commercial offtake exempt from some consultation rules).

### Buffer

Typically **0%** (No Observable Risk).

### Example

Charm Range & Plains — land application of biochar ([registry](https://registry.isometric.com/project/prj_1JN6XNWDQ1S0BSN7)).

---

## Low Oxygen Burial v1.1

### Applicability (strict)

1. Burial in **permitted lined landfill** solid-waste sites under local authority  
2. Permit includes EIS if required; **≥ 20 years** post-closure care; adaptive management; disturbance safeguards  
3. If **Daily Cover**: not removed from active area; permanently buried within **1 week**  
4. Functional low-oxygen / anoxic storage conditions  
5. Default geography: **US, Canada, UK, EU** (other jurisdictions if equally rigorous, Isometric-approved)  

Future versions may expand to purpose-built burial pits ([module](https://registry.isometric.com/module/biochar-storage-low-oxygen/1.1)).

### Quantification

Two Ro-centric frameworks:

- **Option 1:** Ro inertinite fraction **plus** incubation-derived labile persistence with **safety factor 3**  
- **Option 2:** Ro-only (deducts non-passing fraction entirely)  

### Site / legal permanence

Hydrology, geology, seismicity target values (module Table 3); base liner & leachate; landfill gas management; oxygen monitoring (report if exceed permit / 5% default); **ownership + restrictive covenant/easement + enforcement stakeholder** (module Table 4).

### Buffer

Typically **0%**.

### Example + offtake

**Carba Burnsville** (MN) — woody waste → biochar as landfill daily cover; registry approval 25 Jun 2026; expected first certificates 2026 ([registry](https://registry.isometric.com/project/prj_1JRZWM3BP1S071QG)).  
Microsoft agreement: **44,000** credits over **5 years**; 1000-year durability via Isometric ([Carba press 2025-04-24](https://carba.com/press/carba-announces-5-year-carbon-removal-credit-purchase-agreement-with-microsoft)).

---

## Built Environment v1.0+

### Applicable products

- **Concrete:** SCM, filler, admixture, aggregate substitute  
- **Asphalt:** aggregate or modifier  
- Other building materials (bricks, tiles, geopolymers, plasters) case-by-case with similarity proof  

**Not applicable:** carbonate mineralization pathways; lumber storage ([module](https://registry.isometric.com/module/biochar-storage-built-environment/1.0)).

Must meet **same performance** as conventional product; no disproportionate extra installation/maintenance.

### Permanence sketch

\[
F_{Durable,Material} = F_{Inertinite} + [1 - (3 \times F_{Reversal})] F_{Labile}
\]

- Inertinite from Ro ≥ 2% + non-reactive C (mean − 1 SD framing)  
- Default concrete \(F_{Reversal}\) **2%** (PHREEQC worst-case acid weathering) × safety factor **3**  
- Asphalt: labile fraction treated as **100%** lost to abrasion over horizon  

Storage point for crediting: **incorporation into built material**. Downstream manufacturing emissions may be excluded if product parity proven; transport exclusion needs national-average distance justification.

### Buffer

**2%** (Very Low Risk).

### Development notes

Public consultation feedback from suppliers **alterBiota** and **ecoLocked** ([Isometric article](https://isometric.com/writing-articles/a-new-module-for-storing-biochar-in-built-materials); [Carbon Herald 2025-03-12](https://carbonherald.com/isometric-certifies-its-module-on-biochar-storage-in-built-materials/)).

Vault applications: [[Materials and Built Uses]].

---

## Chooser (storage module)

| Choose **Soil** when… | Choose **Burial** when… | Choose **Built** when… |
|---|---|---|
| Agronomic offtake / compost matrix pathways | Co-located landfill daily cover partners | Concrete/asphalt customers want 1000y claims |
| Can run H/Corg labs; Ro optional for 1000y premium | Can meet permit + legal easement bar | Can run Ro + material performance testing |
| Want 200y path without petrography | Want engineered anoxic storage narrative | Buyer demands built-environment CDR |

Cross-registry: Verra non-soil is a **PR_de** path inside VM0044, not a separate module ([[Verra VM0044 Methodology and Eligibility]]); Puro use pathways live in Edition 2025 Table 3.2 ([[Puro Biochar Methodology Edition 2025]]).

---

## Primary links

- [Soil v1.3](https://registry.isometric.com/module/biochar-storage-soil-environments/1.3)
- [Burial v1.1](https://registry.isometric.com/module/biochar-storage-low-oxygen/1.1)
- [Built v1.0](https://registry.isometric.com/module/biochar-storage-built-environment/1.0)
- [Built module article](https://isometric.com/writing-articles/a-new-module-for-storing-biochar-in-built-materials)
- [Carba–Microsoft](https://carba.com/press/carba-announces-5-year-carbon-removal-credit-purchase-agreement-with-microsoft)

## Related notes

- [[Isometric Biochar Protocol]] · [[Isometric Permanence Pathways 200y and 1000y]] · [[Isometric Project Cycle and MRV]]
- [[Materials and Built Uses]] · [[Soil and Agriculture]] · [[Verra vs Isometric vs Puro]]
