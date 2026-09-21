---
tags: [carbon-markets, methodology, csi, permanence]
aliases: [GPC, SPC, CSI permanence, CINK_H, CSI upper persistence class]
updated: 2026-09-16
---

# CSI GPC vs SPC Permanence Classes

How **[[CSI Global Biochar C-Sink]]** v3.3 splits soil-applied biochar carbon into **geologically persistent (GPC)** and **semi-persistent (SPC)** pools, and how **Ro / HyPy** unlock the upper class.

Primary: [Global Biochar C-Sink 3.3 PDF](https://www.carbon-standards.com/docs/transfer/4000039EN.pdf) Ch. 3 · [Formulas PDF](https://www.carbon-standards.com/docs/transfer/4000115EN.pdf) · science context [[Permanence Science for Credits]].

---

## Definitions (v3.3 glossary)

| Term | Meaning |
|---|---|
| **GPC** | Fraction expected to persist **>1000 years** and enter the geological carbon cycle |
| **SPC** | Fraction expected to decay within the **first 1000 years** after soil application (temporary C-sink) |
| **CINK_H / C-Sink_H** | Annual average mass of biochar carbon stored over horizon **H** years (t aCO₂e) — integral average of the remaining SPC (and display conventions for GPC) |
| **TCE** | Total Climate Effect — time-integrated radiative forcing (tCO₂e·yr); positive = warming, negative = cooling |

Source: [v3.3 glossary](https://www.carbon-standards.com/docs/transfer/4000039EN.pdf).

CSI’s framing shift: not “how stable is biochar?” but “**what size is the GPC fraction?**” once applied to soil ([v3.3 §3.2](https://www.carbon-standards.com/docs/transfer/4000039EN.pdf)).

---

## Three operative classes (v3.3)

| Class | Gate | % GPC | % SPC |
|---|---|---|---|
| **SPC-only** | H/C_org **> 0.40** | **0** | **100** |
| **Lower persistence** | H/C_org **≤ 0.40**, upper criteria not met | **75** | **25** |
| **Upper persistence** | H/C_org ≤ 0.40 **and** Ro **or** HyPy gate | **90** | **10** |

([v3.3 §1.1, §3.5–3.6](https://www.carbon-standards.com/docs/transfer/4000039EN.pdf); [formulas §2.1.2](https://www.carbon-standards.com/docs/transfer/4000115EN.pdf))

### Upper-class analytical gates (either suffices)

1. **Mean random reflectance Ro ≥ 3.8%**, with:
   - ≤ **3%** of measured points with Ro **< 2%**
   - ≥ **500** measured points
   - Gaussian distribution
   - heterogeneity score **≤ 8**
2. **BC_HyPy ≥ 90%** of total organic carbon (hydropyrolysis-resistant fraction)

Ro resolves microscale heterogeneity / mixed batches; HyPy isolates a condensed-carbon operational fraction. CSI accepts **either** to keep lab access practical ([v3.3 §3.6](https://www.carbon-standards.com/docs/transfer/4000039EN.pdf)).

**Sampling rule:** Ro/HyPy must be on the **same representative EBC/WBC batch sample**; separate campaigns are rejected. Retroactive Ro/HyPy requires the sample registered in the Global Biochar Tool plus elemental analysis + SEC per EBC Table 1 ([v3.3 §3.7](https://www.carbon-standards.com/docs/transfer/4000039EN.pdf)).

---

## Worked example (standard Table 2)

**100 t** biochar DM, **80% C** → **80 t C** ≈ **293.3 t CO₂e** total.

| Row | H/C_org | Ro | GPC (t CO₂e) | SPC (t CO₂e) | CINK_100 from SPC | CO₂-offsettable GPC |
|---|---|---|---|---|---|---|
| Upper | 0.15 | 3.90% | **264** | 29.3 | 15.4 | 264 |
| Lower | 0.30 | 2.80% | **220** | 73.3 | 38.5 | 220 |
| SPC-only | 0.60 | 1.80% | **0** | 293.3 | 153.9 | 0 |

([v3.3 Table 2](https://www.carbon-standards.com/docs/transfer/4000039EN.pdf)). Online SPC calculator referenced on Carbon Standards site from the same table caption.

---

## SPC decay function

From the formulas companion ([4000115EN §2.1.2](https://www.carbon-standards.com/docs/transfer/4000115EN.pdf)):

\[
C_{\mathrm{remain}}(y) = M_{BC}\cdot C_{\mathrm{cont}}\cdot\Big(\%GPC + \%SPC\cdot\big(0.1787\,e^{-0.5337 y} + 0.8237\,e^{-0.00997 y}\big)\Big)
\]

SPC is described as having a **minimum half-life of ~50 years** (MRT ~83 years) in the narrative intro ([v3.3 §1.1](https://www.carbon-standards.com/docs/transfer/4000039EN.pdf)).

**Climate-service use of SPC:** CINK_H (e.g. CINK_20, CINK_100, CINK_200) for methane compensation and temporary offsetting — **transparently distinct** from geological CO₂ offsetting, which CSI restricts to the **GPC** pool ([v3.3 §3.4, §3.7](https://www.carbon-standards.com/docs/transfer/4000039EN.pdf)). See also [[CSI MRV and Emission Portfolio]] for CH₄ TCE matching.

---

## Proxies and science stance

| Proxy | Role in CSI | Caveat in-standard |
|---|---|---|
| **H/C_org** | Class gate (0.40); bulk aromatic condensation proxy with longest incubation/field empirical base | Average property; ash-rich chars can under/over-estimate; mineral-bound H; see Azzi / Lebrun Thauront citations in §3.3 |
| **Ro** | Upper-class gate (≥3.8%); microscale | Needs endorsed lab + ≥500 points + distributional QC |
| **BC_HyPy** | Alternate upper-class gate (≥90%) | Operational fraction; availability differs by lab |
| **Soil temperature (Woolf-style)** | **Not** used as a global adjustment in v3.3 ops | Footnote: lab vs field stabilizing mechanisms; data insufficient for global T effect ([v3.3 Ch. 3 footnote](https://www.carbon-standards.com/docs/transfer/4000039EN.pdf)) |

Literature cited in-standard includes [[Biochar Soil GHG Inventory Model|models soil GHG from biochar]] ([DOI](https://doi.org/10.1021/acs.est.1c02425)), [[Inertinite Permanence Benchmark|inertinite permanence benchmark]] ([DOI](https://doi.org/10.1016/j.coal.2023.104409)), Schmidt et al. 2025 ([DOI](https://doi.org/10.1111/gcbb.70092)), Azzi et al. 2024 ([DOI](https://doi.org/10.1016/j.geoderma.2023.116761)).

**Forward look:** v3.3 says classes will be refined in the **2026/27** update; higher GPC for a batch may be adjusted retrospectively under future rules ([§3.7](https://www.carbon-standards.com/docs/transfer/4000039EN.pdf)). Draft **v4.0** existed in consultation (closed 30 Apr 2026) but **v3.3 is the live standard** ([service page](https://www.carbon-standards.com/en/standards/service-501~global-biochar-c-sink.html)).

---

## Materials vs soil

| Pathway | Persistence treatment (high level) | Source |
|---|---|---|
| **Soil / geological entry** | GPC/SPC split by class; SPC decays from year 0 | Ch. 3, 12.1 |
| **Composites / plastics** (matrix positive list) | Entire C persists **while the material exists**; removed from registry at destruction/disposal | §1.1; [matrix list](https://www.carbon-standards.com/docs/transfer/4000078EN.pdf) |
| **Concrete / asphalt / mineral binders** | 100% persistence during structure life; EoL landfill can start soil-like curves after a protected period (concrete narrative: ≥100y protected then curves — see Ch. 12.3–12.4) | Ch. 12.3–12.4; §3.7 |

Matrix positive list header (v4_17, 28 May 2026) restates the same GPC/SPC splits for H/C_org < 0.40 ([4000078EN](https://www.carbon-standards.com/docs/transfer/4000078EN.pdf)).

---

## Cross-standard comparison (permanence only)

| Program | Horizon / claim | Quantifying gate closest to CSI upper class |
|---|---|---|
| **CSI v3.3** | GPC **>1000y** / SPC **≤1000y** | Ro **≥ 3.8%** or HyPy **≥ 90%** → 90% GPC |
| **Isometric** | **200y** or **1000y** | Ro **≥ 2%** path → 1000y module ([protocol](https://registry.isometric.com/protocol/biochar/1.3)) |
| **Puro Ed. 2025** | Several centuries (**CORC200+**) | Ro **encouraged, not quantifying** ([permanence post](https://puro.earth/insights/post/biochar-permanence/)) |
| **Verra VM0044** | **100 years** | H/C_org → Table 3 temperature factors |

Chooser: [[Verra vs Isometric vs Puro]] · [[Puro vs Other Standards]]. Science camps: [[Permanence Science for Credits]].

**Practical lab note:** CSI’s **3.8%** Ro bar is materially stricter than Isometric’s **2%** 1000-year threshold — budget petrography early if upper-class GPC is the commercial product.

---

## Primary links

- [C-Sink 3.3 PDF](https://www.carbon-standards.com/docs/transfer/4000039EN.pdf)
- [Formulas & EFs](https://www.carbon-standards.com/docs/transfer/4000115EN.pdf)
- [Matrix positive list](https://www.carbon-standards.com/docs/transfer/4000078EN.pdf)
- Sanei et al. 2024 — https://doi.org/10.1016/j.coal.2023.104409
- Schmidt et al. 2025 — https://doi.org/10.1111/gcbb.70092
- Woolf et al. 2021 — https://doi.org/10.1021/acs.est.1c02425

## Related notes

- [[CSI Global Biochar C-Sink]] · [[CSI Overview]] · [[CSI MRV and Emission Portfolio]]
- [[Permanence Science for Credits]] · [[Permanence]] · [[Isometric Permanence Pathways 200y and 1000y]] · [[Puro CORC200+]]
- [[Product Standards EBC IBI]] · [[Key Sources]]
