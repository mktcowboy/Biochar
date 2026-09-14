---
tags: [carbon-markets, methodology, puro, corc200, permanence, durable-cdr]
aliases: [CORC200+, CORC200, Puro biochar credit, Biochar CORC200+]
updated: 2026-09-14
---

# Puro CORC200+

**What this note is:** the durable-credit **concept** note — what **CORC200+** means as a permanence claim and labelling transition, and how it sits in the Puro product family.  
**What this note is not:** a full reprint of Edition 2025 rules. For exhaustive eligibility, feedstock, end uses, LCA, and equations, open **[[Puro Biochar Methodology Edition 2025]]**. For audits and US producer ops, open **[[Puro Project Cycle and MRV]]**.

| | |
|---|---|
| **Operator** | [[Puro.earth Overview\|Puro.earth]] (Puro Standard + Registry) |
| **Unit** | CO₂ Removal Certificate labelled **CORC200+** = **1 tCO₂e** net removal |
| **Current biochar method** | [[Puro Biochar Methodology Edition 2025]] — V1 **12 Jun 2025**; **v2** (retail R3) **27 Nov 2025** |
| **Prior biochar label** | **CORC100+** under Edition 2022 |
| **Index** | [[Puro Pricing and CORC Indexes\|CORCCHAR]] |
| **Compare** | [[Puro vs Other Standards]] |

Science: [[Permanence]] · [[Permanence Science for Credits]] · [[Biochar as Durable CDR]] · [[Properties]]

---

## One-sentence definition

**CORC200+** is Puro’s Edition 2025 biochar credit label asserting **net durable CDR** with a permanence framing of **several centuries (≥200 years)**, quantified with a revised **power-law** decay model (H/C_org + soil temperature, **80% CI lower bound**), and issued **ex-post** only after biochar reaches a **durable eligible use**.

---

## Snapshot table

| Item | Value |
|---|---|
| What it credits | Net CDR across biomass → thermochemical conversion → **eligible use** |
| Durability label | **Several centuries** (≥200 years); EU “permanent removal” alignment cited by Puro |
| Prior label | CORC100+ (Edition 2022; [[Woolf et al. 2021]] multi-pool) |
| H/C_org gate | **< 0.70** |
| Crediting period (Ed. 2025) | **10 years**, renewable twice |
| Issuance | **Ex-post** after durable eligible use + Output Audit |
| Ro / reflectance | Reporting **encouraged**; **does not affect quantification** yet |
| Buffer | **No default** reversal buffer |
| Index (Aug 2026) | **CORCCHAR €135.35** |
| ICVCM | Program CCP-Eligible (General Rules **v4.2+**, Dec 2025); biochar **methodology not yet CCP-Approved** |
| Biochar projects since 2019 | **70+** (Puro permanence post) |

---

## Label history: from Spokas / 100+ to 200+

| Label | Biochar methodology | Permanence framing | Decay basis |
|---|---|---|---|
| Early (Edition 2019) | Spokas 2010 O:C framing | 100-year style | Spokas |
| **CORC100+** | Edition 2022 | ~100 years | Woolf et al. 2021 multi-pool exponential; H/C_org + soil T |
| **CORC200+** | **Edition 2025** (v1 Jun 2025; v2 Nov 2025) | **Several centuries** (≥200 years) | Revised **power-law** decay; H/C_org + soil T; **80% CI lower bound**; open-source notebook |

Source: [Puro permanence explainer, 2025-07-03](https://puro.earth/insights/post/biochar-permanence/); Edition 2025 v2 §1.1, §6.2.

### Why the rename matters commercially

- Buyers and offtake term sheets increasingly distinguish **100-year**, **200-year / centuries**, and **1000-year / millennial** claims ([[Puro vs Other Standards]] · [[Buyers and Offtakes]]).
- Marketing baseline CORCs still often say “100+ year durability” across pathways; **biochar Edition 2025 specifically issues CORC200+** — do not conflate pathway-generic CORC marketing with the biochar label.
- CCP methodology labels are a **separate** integrity layer: Puro program eligible ≠ biochar method CCP-Approved ([[Puro.earth Overview]]).

---

## Permanence claim — what is asserted, what is not

### Asserted

1. Quantification horizon of **200 years** under a **power-law** persistence model.
2. After 200 years, **deeper-soil protection** is assumed for **further centuries** → marketing/label claim of **several centuries / CORC200+**.
3. Conservatism via the **lower bound of an 80% confidence interval**.
4. Soil temperature from Puro dataset with a **7 °C floor**; H/C_org domain **0–0.7**.

### Not asserted (yet)

1. **Millennial / 1000+ year** inertinite-equivalent permanence as a quantified CORC factor.
2. That **Ro** (random reflectance) changes the number of CORCs — it is **encouraged reporting only**.
3. That program CCP-Eligibility equals a CCP **credit** label on biochar CORCs.

Puro **explicitly stopped at centuries**, not millennia, pending integration ([permanence post](https://puro.earth/insights/post/biochar-permanence/)). Contrast:

| Program | Horizon path |
|---|---|
| Puro CORC200+ | Centuries (200+) |
| Verra VM0044 | **100 years** |
| Isometric | **200y** or **1000y** if Ro≥2% |
| CSI | GPC **>1000y** / SPC ≤1000y (upper path Ro≥3.8% or HyPy≥90%) |

Science debate map: [[Permanence Science for Credits]] · [[Permanence]] · [[Risks and Controversies]]  
Equations and Table 6.1: [[Puro Biochar Methodology Edition 2025]]

---

## Quantification sketch (pointer, not full method)

Net CORCs:

\[
\mathrm{CORCs} = C_{\mathrm{stored}} - C_{\mathrm{baseline}} - C_{\mathrm{loss}} - E_{\mathrm{project}} - E_{\mathrm{leakage}}
\]

- \(C_{\mathrm{stored}} = Q_{\mathrm{biochar}} \times C_{\mathrm{org}} \times 44/12\)
- Persistence fraction: \(PF = M - a \times (H/C_{\mathrm{org}})\) with \(M,a\) from soil-T Table 6.1
- Worked intuition at 20 °C: H/C_org 0.4 → PF ≈ **75.8%**; H/C_org 0.2 → ≈ **82.8%**

Open-source model: https://github.com/puro-earth/PuroBiocharPersistenceEdition2025  
Full eligibility, LCA, baselines, Table 3.2: **[[Puro Biochar Methodology Edition 2025]]**  
Lab cadence / CoC: **[[Puro Project Cycle and MRV]]** · [[MRV Stack]]

---

## Transition milestones (label + method)

| Milestone | Date |
|---|---|
| Public consultation | 3–28 Apr 2025 |
| Edition 2025 V1 approval | **12 Jun 2025** |
| Publishing | **30 Jun 2025** |
| Launch (Facility Audits under 2025) | **1 Nov 2025** |
| Last 2022 Audit Package (pre-launch regs) | **15 Dec 2025** |
| Edition 2022 termination | **12 Jun 2030** |
| Retail R3 enabled (v2) → still **CORC200+** units | **27 Nov 2025** |

**Implications for the label:**

- New facilities after Launch **must** issue under Edition 2025 → **CORC200+**, not CORC100+.
- Legacy Edition 2022 facilities may finish their period as CORC100+ pathway credits, then renew only on latest edition (CORC200+ rules).
- Preliminary Assessments against 2022 **do not carry over**.

Detail: [[Puro Biochar Methodology Edition 2025]] · ops: [[Puro Project Cycle and MRV]]

---

## Where CORC200+ sits in the market

| Signal | Note |
|---|---|
| Public price | [[Puro Pricing and CORC Indexes\|CORCCHAR]] Aug 2026 **€135.35**; all-CORC **CORCX €150.40** |
| Liquidity | Issuance→transfer/retirement **95 → 22 days** (2021 → mid-2025, CDR.fyi via Puro) |
| Scale | ~1.88M issued / ~1.08M retired / 119 projects (all methods, registry 2026-09-14); **70+** biochar projects since 2019 |
| Buyers | Early Microsoft CORCs; CDR.fyi BCR leaders include Microsoft, Google, BCG, JPMorgan, Swiss Re, SEB (Puro narrative) — [[Buyers and Offtakes]] |
| Integrity gap | Program CCP-Eligible; biochar method **pending** category CCP approval |

Market volumes: [[Market Volumes and Pricing]] · chooser: [[Puro vs Other Standards]]

---

## Architecture of the vault’s Puro cluster

| Note | Role |
|---|---|
| **This note ([[Puro CORC200+]])** | Durable-credit **concept** — label, claim, transition, pointers |
| [[Puro.earth Overview]] | Company, registry, scale, ICVCM, link map |
| [[Puro Biochar Methodology Edition 2025]] | Exhaustive method chapter |
| [[Puro Project Cycle and MRV]] | Audits, labs, CoC, US path, pitfalls |
| [[Puro Pricing and CORC Indexes]] | CORCCHAR/CORCX, fees, deals |
| [[Puro vs Other Standards]] | Comparison + chooser |

---

## Common confusions (quick FAQ)

**Is every CORC a CORC200+?**  
No. CORC200+ is the **biochar Edition 2025** label. Other Puro methodologies use other durability labels (100+ / 200+ / 1,000+ depending on pathway).

**Is CORC200+ the same as a 1000-year credit?**  
No. Puro stopped at **centuries**. Millennial claims live elsewhere (e.g., Isometric Ro path, CSI GPC upper class).

**Does Ro unlock more CORCs under Puro?**  
Not yet. Encouraged reporting only; does not change quantification under Edition 2025.

**Does CCP-Eligible program status put a CCP label on my biochar CORCs?**  
Not by itself. Methodology-category approval is separate; as of 2025-12-11 biochar was **not yet** CCP-Approved.

**When is the credit created?**  
At first **durable eligible use** + successful Output Audit — not at the kiln door alone.

---

## Primary links

1. [Permanence science](https://puro.earth/insights/post/biochar-permanence/)
2. [Edition 2025 v2 PDF](https://7518557.fs1.hubspotusercontent-na1.net/hubfs/7518557/Puro%20Biochar%20Methodology%20-%20Edition%202025%20%28version%202%29%20-%20For%20Publication.pdf)
3. [Transition plan PDF](https://7518557.fs1.hubspotusercontent-na1.net/hubfs/7518557/Biochar%20Public%20Consultation%202025/03_Methodology%20Transition%20Plan%20for%20Biochar%20Edition%202025.pdf)
4. [Retail v2 update](https://puro.earth/insights/post/354-puro-earth-biochar-methodology-update-a-collaborative-step-forward-for-retail-use/)
5. [CORC indexes](https://puro.earth/buy-carbon-credits/removal-certificate-corc/carbon-removal-indexes/)
6. [Fees / journey](https://puro.earth/certified-carbon-credits/fees/)
7. [CORC page](https://puro.earth/buy-carbon-credits/removal-certificate-corc/)
8. Persistence model — https://github.com/puro-earth/PuroBiocharPersistenceEdition2025
9. Woolf et al. 2021 — https://doi.org/10.1021/acs.est.1c02425
10. [[Sanei et al. 2024]] — https://doi.org/10.1016/j.coal.2023.104409
11. Azzi et al. 2024 — https://doi.org/10.1016/j.geoderma.2023.116761

Also: [[Key Sources]]

---

## See also

[[Puro.earth Overview]] · [[Puro Biochar Methodology Edition 2025]] · [[Puro Project Cycle and MRV]] · [[Puro Pricing and CORC Indexes]] · [[Puro vs Other Standards]] · [[Biochar as Durable CDR]] · [[Permanence Science for Credits]] · [[Permanence]] · [[MRV Stack]] · [[Market Volumes and Pricing]] · [[Buyers and Offtakes]] · [[Risks and Controversies]] · [[Verra VM0044]] · [[Isometric Biochar Protocol]] · [[CSI Global Biochar C-Sink]] · [[Double Counting and Credit Ownership]] · [[Properties]] · [[Carbon Markets Hub]] · [[Key Sources]]
