---
tags: [carbon-markets, methodology, puro, permanence]
aliases: [Edition 2025, Biochar Edition 2025, Puro biochar methodology]
updated: 2026-09-14
---

# Puro Biochar Methodology Edition 2025

Parent: [[Puro CORC200+]] · Operator: [[Puro.earth Overview]]

## Versions

| Version | Approval | Notes |
|---|---|---|
| Edition 2025 **V1** | **12 Jun 2025** (published 30 Jun) | CORC200+; revised decay model; stricter sourcing; mobile rules |
| Edition 2025 **v2** | **27 Nov 2025** | Makes retail-to-individuals (**Category R3**) CORC-eligible under safeguards |

PDF: [Edition 2025 v2](https://7518557.fs1.hubspotusercontent-na1.net/hubfs/7518557/Puro%20Biochar%20Methodology%20-%20Edition%202025%20%28version%202%29%20-%20For%20Publication.pdf)

## From Edition 2022 → 2025 (what changed)

| Theme | Edition 2022 | Edition 2025 |
|---|---|---|
| Label | CORC100+ | **CORC200+** |
| Decay model | Woolf et al. 2021 multi-pool exponential | **Power model**, 200y horizon + deeper-soil assumption; **80% CI** lower bound |
| Ro / reflectance | — | **Encouraged**, not quantifying |
| Crediting period | Often cited as 5y in transition docs for legacy facilities | **10 years**, renew twice |
| Biomass | Prior rules | Stricter **Biomass Sourcing Criteria** categories |
| Mobile units | Limited treatment | Explicit **Stationary vs Mobile** facility rules |
| Retail R3 | — | Initially excluded; **v2** adds eligibility + RDF |
| Launch / phase-out | — | Audits from **1 Nov 2025**; Ed. 2022 ends **12 Jun 2030** |

Transition PDF: [link](https://7518557.fs1.hubspotusercontent-na1.net/hubfs/7518557/Biochar%20Public%20Consultation%202025/03_Methodology%20Transition%20Plan%20for%20Biochar%20Edition%202025.pdf)

## Eligibility pillars

1. **Eligible biomass** (categories B–O typically CORC-capable; A mixed MSW and J food crops out; P land-clearing processable but **no CORCs**)
2. **Production** with H/C_org **< 0.70**; combustion / co-product / emissions safeguards
3. **Eligible use** per Table 3.2 (soil AF*, substrates, animal cascades, built environment BE*, remediation, landfill with evidence, retail R3/R4 with controls…)
4. **Baseline + additionality** (carbon / regulatory / financial)
5. **Net positive quantification** after LCA + leakage

Baselines: **New Facility**, **Retrofit Facility**, **Charcoal Repurpose**.

## Permanence equations

\[
C_{\mathrm{stored}} = Q_{\mathrm{biochar}} \times C_{\mathrm{org}} \times \frac{44}{12}
\]

\[
C_{\mathrm{loss}} = C_{\mathrm{stored}} \times (100 - PF)\ \text{(PF in \%)}
\]

\[
PF = M - a \times (H/C_{\mathrm{org}})
\]

\(M,a\) from Table 6.1 by soil temperature (°C); **floor 7 °C**. Open-source model: [GitHub puro-earth/PuroBiocharPersistenceEdition2025](https://github.com/puro-earth/PuroBiocharPersistenceEdition2025).

Example (Table 6.1): at **20 °C**, \(M=89.87\), \(a=35.29\).

Science context: [[Permanence Science for Credits]] · [Puro permanence post](https://puro.earth/insights/post/biochar-permanence/) · Woolf et al. 2021 [DOI](https://doi.org/10.1021/acs.est.1c02425) · Sanei et al. 2024 [DOI](https://doi.org/10.1016/j.coal.2023.104409) · Azzi et al. 2024 [DOI](https://doi.org/10.1016/j.geoderma.2023.116761)

## Retail Category R3 (v2)

Eligible for CORCs only with: product-level particle size/moisture controls; consumer labelling; contractual clarity with last tracked intermediary; **country-level reversal-risk discount (RDF)** on \(C_{\mathrm{stored}}\); conservative transport accounting. ([Dec 2025 update](https://puro.earth/insights/post/354-puro-earth-biochar-methodology-update-a-collaborative-step-forward-for-retail-use/))

## Reversal policy

No **default buffer** deduction (rule 4.2.1). Risks managed via use eligibility + evidence; supplier liable for reversals caused by non-compliance.

## See also

[[Puro Project Cycle and MRV]] · [[Puro vs Other Standards]] · [[MRV Stack]]
