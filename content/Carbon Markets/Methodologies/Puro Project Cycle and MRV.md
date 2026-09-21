---
tags: [carbon-markets, mrv, puro, project-cycle, audits, us-producer]
aliases: [Puro MRV, Puro certification journey, Puro audits, Puro project cycle]
updated: 2026-09-14
---

# Puro Project Cycle and MRV

**Parent concept:** [[Puro CORC200+]]  
**Method detail:** [[Puro Biochar Methodology Edition 2025]]  
**Operator:** [[Puro.earth Overview]]  
**Generic MRV framing:** [[MRV Stack]]

This chapter walks the full path from listing a facility to retiring CORCs: audits, lab metrics, chain of custody, auditor allocation, public fees, and a practical **US producer** path with common pitfalls. Facts from the Puro deep-dive research (2026-09-14) and primary fee/V&V documents cited there.

---

## End-to-end cycle (one page)

```
Initial Qualification
        ↓
Platform Agreement + KYC → MyPuro (€1,400/yr)
        ↓
Facility Registration
        ↓
Audit Package (± optional Preliminary Assessment / Future Facility)
        ↓
Facility Audit (Puro-allocated VVB) → Certified Facility
        ↓
Produce → Apply to eligible use → Monitor
        ↓
Output Report → Output Audit (≥ annually)
        ↓
CORC issuance → transfer / sale → Buyer retirement
```

**Critical rule:** Point of CORC creation = first **durable eligible use** (rule 2.3.1) — **ex-post** relative to application, **not** factory gate alone. Claiming credits before use proof is a top failure mode. Eligibility of uses: [[Puro Biochar Methodology Edition 2025]] · ownership: [[Double Counting and Credit Ownership]].

---

## Certification journey (detailed)

Public journey from [Fees / certify pages](https://puro.earth/certified-carbon-credits/fees/):

| Step | What happens | Notes |
|---|---|---|
| 1. **Initial Qualification** | Supplier interest / questionnaire | Screens fit for Puro engineered-CDR pathways |
| 2. **Platform Agreement + KYC** | Become MyPuro Account Holder | **Annual Fee €1,400** / 12 months |
| 3. **Facility Registration** | Unique Production Facility ID in registry | Stationary vs Mobile definitions matter under Ed. 2025 |
| 4. **Audit Package** | Biomass evidence, LCA, Monitoring Plan, additionality questionnaire, permits, SDG/safeguards | Heaviest prep step for most producers |
| 5. **Preliminary Assessment** (optional) | Future Facility listing | **2022 PAs do not transfer** to Edition 2025 |
| 6. **Facility Audit** | Third-party VVB; typically **on-site** first audit | Puro **allocates** VVB; Puro covers verification costs per public fees narrative |
| 7. **Operations + Output Audits** | Output Report → Output Audit → issuance | ≥ annually; more frequent by volume tiers |
| 8. **Issuance → sale → retirement** | CORCs to supplier account | Retirement fee **€0.25**/CORC unless offtake waiver |

Crediting period under Edition 2025: **10 years**, renewable **twice** after new Facility Audit against **latest** rules. Capacity expansion of similar reactors possible without resetting period (rules 3.1.6–3.1.8).

Output frequency scales with volume (General Rules 4.4 table on fees page): from **1×/yr** below ~10k CORCs up to **12×/yr** above 60k (per deep-dive extraction of fees page).

---

## Who the supplier is

- **CO₂ Removal Supplier** = biochar producer **or** contracted representative with **sole CORC claim rights** and end-to-end data access (rules 2.1.1–2.1.3)
- Must comply with methodology + **Puro Standard General Rules** + local law
- Double-claiming / intermediary diversion risks: [[Double Counting and Credit Ownership]]

---

## MRV stack under Edition 2025

| Layer | Requirements |
|---|---|
| **Biomass CoC** | Declared sources + batch records; BSC category / traceability / sustainability; impurity & fossil-C monitoring |
| **Process** | Temperature/residence monitoring for Regime A (1-min); combustion uptime; CH₄/N₂O; waste & co-product fate |
| **Lab** | Accredited lab preference; elemental analysis standards (ISO 16948, ASTM D5373, etc.); moisture/bulk density methods listed in methodology §6.1 |
| **Sampling frequency** | Regime A: ≥**2×/year**/biochar type; Regime B: ≥**4×/year**; auditor may resample on site |
| **End-use evidence** | Proof of eligible use (geotag/application docs, sales contracts, intermediary agreements); cascading-use evidence where required; retail R3: particle size/moisture, labelling, last-intermediary contracts, country RDF |
| **Digital MRV** | MyPuro portal + registry tracking; third-party dMRV platforms (e.g., Carbonfuture) used by some suppliers in market practice — **not** a universal Puro mandate in the methodology text |
| **Auditors** | Puro-approved VVBs; Puro **allocates** auditor (geography, expertise, rotation, fees) |
| **Records** | Monitoring Plan; Output Report; retention per General Rules |

Generic vault framing of the same layers: [[MRV Stack]] · production science: [[Production]] · quality: [[Contaminants and Quality]] · permanence metrics: [[Properties]] · [[Permanence]]

---

## Lab metrics and sampling regimes

### What must be measured for quantification

| Analytic | Why |
|---|---|
| Dry mass (impurity-corrected) | Mass basis for \(Q_{\mathrm{biochar}}\) |
| \(C_{\mathrm{org}} = C_{\mathrm{tot}} - C_{\mathrm{inorg}}\) | Enters \(C_{\mathrm{stored}}\) |
| **H** → **H/C_org** | Enters persistence fraction PF; hard gate **H/C_org < 0.70** |
| Contaminants / environmental quality | Table 3.2 → WBC class thresholds where local regulation absent |
| **Ro / petrography** | Optional complementary reporting; **does not change CORC math yet** |

Methods listed in methodology §6.1 include ISO 16948, ASTM D5373, DIN carbonate methods, etc. Auditor may request on-site resample.

Permanence equations and worked PF examples: [[Puro Biochar Methodology Edition 2025]] · [[Puro CORC200+]] · [[Permanence Science for Credits]]

### Sampling frequency

| Regime | When | Minimum lab frequency (permanence + C) |
|---|---|---|
| **A** | Continuous uniform carbonization monitoring (1-min T & residence; ±10% stability) | **≥2× per year** per biochar type |
| **B** | No continuous uniform proof | **≥4× per year** per biochar type |

**Pitfall:** batches with H/C_org **≥ 0.70** fail the quantification gate; under-sampling Regime B facilities is a common audit risk.

---

## Chain of custody and end-use evidence

### Biomass

- Source list + batch records
- BSC category coding + sustainability evidence
- Impurity & fossil-C monitoring (plastics, paints, sludge fossil C)
- Stockpile CH₄ controls; biohazard treatment (≥500 °C × 3 min if relying on carbonization) — method detail in [[Puro Biochar Methodology Edition 2025]]

### Product

- Batch IDs, weigh tickets, moisture
- Separation of ineligible / no-CORC streams (e.g., category P land-clearing may be processed but **shall not issue CORCs**)

### Use / application

- Proof matching Table 3.2 (application records, contracts, geotags/GIS as applicable)
- Cascading-fate evidence where required (e.g., animal cascades **AH***)
- Intermediary agreements preventing diversion / double claiming ([[Double Counting and Credit Ownership]])
- Retail **R3**: last-intermediary contracts + country-level **RDF** + product particle size/moisture + labelling

US ag practice context (not a credit methodology): [[Soil Carbon Amendment and US Ag|NRCS soil carbon amendment in US ag]]

---

## Emissions MRV highlights

| Topic | Rule / practice |
|---|---|
| Combustion uptime | Systems ≥**95%** normal operating time; flameout procedures |
| Residual CH₄ / N₂O | Monitoring rules for carbonization |
| Stockpile CH₄ | Quantify unless negligible criteria met |
| Fossil C in plastics / paints / **sewage sludge** | Counted as project emissions (assumed fully re-emitted) |
| Full LCA | Operational + embodied; co-product allocation; cut-offs |
| Leakage | Identify, mitigate, quantify residual market/activity-shifting leakage |
| Fossil support fuel | Allowed for ignition/support if no fossil C enters biochar and LCA includes emissions; **coal as process fuel not allowed** |

Net equation reminder:

\[
\mathrm{CORCs} = C_{\mathrm{stored}} - C_{\mathrm{baseline}} - C_{\mathrm{loss}} - E_{\mathrm{project}} - E_{\mathrm{leakage}}
\]

Full quantification: [[Puro Biochar Methodology Edition 2025]]

---

## Auditors (VVBs)

Source: [Validation & Verification Requirements v1.3](https://7518557.fs1.hubspotusercontent-na1.net/hubfs/7518557/Supplier%20Documents/Validation%20and%20Verification%20Requirements%20v1.3.pdf)

| Rule | Detail |
|---|---|
| Approval | Must be **Puro-approved** (application + methodology training) |
| Allocation | **Puro allocates** VVB (geography, expertise, availability, rotation, fees) — suppliers do **not** freely shop from a public list |
| Contracting | Framework or per-audit contracting negotiated by Puro |
| Conflicts | Conflict-of-interest checks required |
| Cost narrative | Puro covers verification costs per public fees page narrative; suppliers pay annual + volume service fees |

This allocation model differs from many VCS-style shop-your-auditor practices — relevant when comparing [[Verra VM0044]] in [[Puro vs Other Standards]].

---

## Public fee anchors

Source: [puro.earth/certified-carbon-credits/fees](https://puro.earth/certified-carbon-credits/fees/)

| Item | Amount |
|---|---|
| Annual account fee | **€1,400** / 12 months |
| Service fee (volume) | Tiered **€10.00 → €0.40** per CORC by trailing 12-mo volume |
| Low-volume audits (≤1,000 CORC) | **€12,000 flat** when audit booked |
| Biochar complexity premium | **0%** |
| Retirement fee | **€0.25** / CORC (waivable for qualifying multi-year offtakes reported in MyPuro spanning >1 calendar year) |
| Secondary trading fee | **0%** |
| Pooling admin | **€2,000** / facility / year if pooling |
| Issuance-time payment | **5%** service-fee discount |

Market pricing / indexes (CORCCHAR, CORCX) and deal structures: **[[Puro Pricing and CORC Indexes]]** · [[Market Volumes and Pricing]] · [[Buyers and Offtakes]]

**Honesty:** Fees change — re-pull before investment decisions.

---

## Practical path for a US biochar producer

### Recommended sequence

1. Confirm feedstock fit against BSC categories (avoid A, J; understand P = processable but **no CORCs**).
2. Map end-use channel to Table 3.2 **before** promising buyers CORC volumes (farm contracts vs retail R3).
3. Submit Initial Qualification → Platform Agreement + KYC → MyPuro.
4. Register Production Facility (Stationary vs Mobile; host-country spatial extent for fleets).
5. Build Audit Package early: biomass evidence, LCA (stockpile CH₄, impurities, sludge fossil C, transport), Monitoring Plan, additionality questionnaire (especially **financial** additionality), permits, SDG/safeguards.
6. Optional Preliminary Assessment — remember **2022 PAs are obsolete** for Edition 2025.
7. Facility Audit (VVB allocated by Puro).
8. Produce, apply, monitor → Output Audit → issuance → sell/retire.
9. Budget annual €1,400 + volume service tiers + retirement €0.25 (or offtake waiver).

### Edition 2025 transition checklist

| Situation | Action |
|---|---|
| New registration on/after **1 Nov 2025** | **Must** use Edition 2025 |
| Pre-launch registration, not yet audited | Prefer 2025; 2022 only if complete Audit Package by **15 Dec 2025** |
| Certified under 2022 | Finish current period; renew on latest edition; optional early upgrade at next Output Audit |
| Planning beyond **12 Jun 2030** | Edition 2022 **terminated** — design for 2025 now |

---

## Common pitfalls (from deep dive)

1. **Weak waste/residue / BSC evidence**; mixing ineligible feedstock (A, J) or issuing CORCs on category **P**
2. **Claiming CORCs before eligible end-use proof**
3. **Retail / diffuse channels** without R3 safeguards / RDF
4. **Underestimating LCA** — stockpile CH₄, plastic impurities, sludge fossil C, transport
5. **Failing financial additionality** when biochar product margins / waste-treatment savings already make the project viable without CORCs
6. **Mobile fleet spatial-extent / multi-state host-country issues**
7. **Lab cadence** shortfalls; H/C_org **≥ 0.70** batches
8. **Edition 2022→2025 transition** — renewals must meet 2025; Preliminary Assessments don’t transfer
9. **Double counting** across registries or intermediaries — [[Double Counting and Credit Ownership]]
10. **Assuming CCP credit labels** from program eligibility alone — biochar methodology **not yet** CCP-Approved ([[Puro.earth Overview]] · [[Puro vs Other Standards]])

Broader market/integrity risks: [[Risks and Controversies]]

---

## When to choose Puro vs other standards (ops lens)

| Choose **Puro** when… | Choose **Verra VM0044** when… | Choose **Isometric** when… | Choose **CSI** when… |
|---|---|---|---|
| Mature BCR buyer recognition + **CORCCHAR** price signal + Nasdaq registry ops; mobile/retrofit/charcoal-repurpose fit | Need **CCP-labelled methodology today** + VCS buyer familiarity; clearly **new** waste facility | Buyer demands **1000-year Ro path** or maximal soil MRV stringency | Already hold **EBC/WBC** and want GPC/SPC + EU CRCF alignment path; artisan track |

Many large buyers are registry-agnostic on BCR but diligence MRV; **dual pathways are uncommon for the same tonne** (double-counting rules). Full comparison: [[Puro vs Other Standards]] · peer notes: [[Verra VM0044]] · [[Isometric Biochar Protocol]] · [[CSI Global Biochar C-Sink]]

---

## Primary citations

1. [Fees / supplier journey](https://puro.earth/certified-carbon-credits/fees/)
2. [V&V Requirements v1.3](https://7518557.fs1.hubspotusercontent-na1.net/hubfs/7518557/Supplier%20Documents/Validation%20and%20Verification%20Requirements%20v1.3.pdf)
3. [Edition 2025 v2 PDF](https://7518557.fs1.hubspotusercontent-na1.net/hubfs/7518557/Puro%20Biochar%20Methodology%20-%20Edition%202025%20%28version%202%29%20-%20For%20Publication.pdf)
4. [Transition plan PDF](https://7518557.fs1.hubspotusercontent-na1.net/hubfs/7518557/Biochar%20Public%20Consultation%202025/03_Methodology%20Transition%20Plan%20for%20Biochar%20Edition%202025.pdf)
5. [Retail v2 update](https://puro.earth/insights/post/354-puro-earth-biochar-methodology-update-a-collaborative-step-forward-for-retail-use/)
6. [Registry](https://registry.puro.earth/)

Also: [[Key Sources]]

---

## See also

[[Puro CORC200+]] · [[Puro.earth Overview]] · [[Puro Biochar Methodology Edition 2025]] · [[Puro Pricing and CORC Indexes]] · [[Puro vs Other Standards]] · [[MRV Stack]] · [[Double Counting and Credit Ownership]] · [[Soil Carbon Amendment and US Ag|NRCS soil carbon amendment in US ag]] · [[Biochar as Durable CDR]] · [[Permanence Science for Credits]] · [[Permanence]] · [[Production]] · [[Properties]] · [[Contaminants and Quality]] · [[Buyers and Offtakes]] · [[Market Volumes and Pricing]] · [[Risks and Controversies]] · [[Verra VM0044]] · [[Isometric Biochar Protocol]] · [[CSI Global Biochar C-Sink]] · [[Carbon Markets Hub]] · [[Key Sources]]
