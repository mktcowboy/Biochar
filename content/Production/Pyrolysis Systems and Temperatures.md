---
tags: [production, pyrolysis, reactors]
aliases: [Pyrolysis systems, Pyrolysis temperature, Reactor types]
updated: 2026-09-16
---

# Pyrolysis Systems and Temperatures

Chapter on **reactor modes, temperature classes, residence time, and heat management**—the controllable engineering variables that set biochar yield and chemistry. Report context: **2026-09-16**.

**Related notes:** [[Production]] · [[Biochar Quality from Process]] · [[Gasification Residues]] · [[Feedstocks]] · [[Woolf IPCC Fperm]] · [[PAHs]] · [[Production Hub]] · [[Key Sources]]

---

## 1. Temperature classes used in inventories

[[Biochar Soil GHG Inventory Model|models soil GHG from biochar]] / [[IPCC 2019 Biochar Appendix]] permanence and FC tables use:

| Class | Peak temperature | Typical role |
|---|---|---|
| Low | **350–450 °C** | Higher yield, higher H/C_org, lower \(F_\mathrm{perm}\) |
| Medium | **450–600 °C** | Common agronomic / CDR operating window |
| High | **≥600 °C** | More condensed aromatics; often lower mass yield |

([Woolf DOI](https://doi.org/10.1021/acs.est.1c02425); [IPCC PDF](https://www.ipcc-nggip.iges.or.jp/public/2019rf/pdf/4_Volume4/19R_V4_Ch02_Ap4_Biochar.pdf)). Materials **<350 °C** excluded from these permanence methods ([Woolf §2.1.1](https://doi.org/10.1021/acs.est.1c02425)).

EBC batch rule of thumb: declared pyrolysis temperature may fluctuate by up to **±20%** (e.g. 600 °C → short-term 480–720 °C) without breaking the batch, if documented ([EBC 10.5E](https://www.european-biochar.org/media/doc/7/ebc_en_10_5_red.pdf) §5.5). EBC-FeedPlus / Swiss-style agricultural rules often require **≥500 °C for ≥10 min**, proxied by H/C_org < 0.4 ([EBC §10.4](https://www.european-biochar.org/media/doc/7/ebc_en_10_5_red.pdf)).

---

## 2. Heating rate and residence time

| Mode | Heating rate / solids residence | Product emphasis |
|---|---|---|
| **Slow pyrolysis** | Low °C/min; minutes–hours | Maximize **biochar** |
| **Fast / flash** | Very high heating; seconds | Maximize **liquids** |
| **Gasification** | Limited oxidant; often >700–800 °C bed | Maximize **syngas**; solid = residue |

Residence time at peak T matters as much as the peak number for condensation ([Keiluweit et al. 2010](https://doi.org/10.1021/es9031419); Woolf notes T is a weaker condensation proxy than H/C_org because time also matters — [DOI](https://doi.org/10.1021/acs.est.1c02425)).

---

## 3. Reactor families (descriptive)

Commercial and farm-scale systems span:

- **Continuous auger / rotary / screw** pyrolyzers — steady T profiles, good batch documentation for MRV.
- **Fixed / moving bed** and **fluidized bed** — industrial throughput; fluid beds favor fast heat transfer (often liquids if configured that way).
- **Kilns / retorts / flame-curtain (e.g. Kon-Tiki class)** — farmer-scale; EBC cites flame-curtain examples as capable of low PAH when vapor handling is correct ([EBC 10.5E](https://www.european-biochar.org/media/doc/7/ebc_en_10_5_red.pdf) §7.11; Cornelissen et al. 2016 emissions/char quality study cited therein · [DOI](https://doi.org/10.1371/journal.pone.0154617)).
- **Gasifiers** (downdraft, updraft, fluidized) — see [[Gasification Residues]].

EBC requires each pyrolysis **unit** certified individually (with limited exceptions for identical parallel lines sharing feedstock/output) ([EBC §8.6](https://www.european-biochar.org/media/doc/7/ebc_en_10_5_red.pdf)).

---

## 4. Energy and emissions engineering

From Woolf life-cycle framing and EBC:

- ~**35–60%** of feedstock energy often ends in pyrolysis gas that is burned in-plant ([EBC §8.5](https://www.european-biochar.org/media/doc/7/ebc_en_10_5_red.pdf)).
- Modern plants should fully combust organics to CO₂; simple kilns may emit **CH₄** and VOCs that erase climate benefit if unmanaged ([Woolf 2021](https://doi.org/10.1021/acs.est.1c02425) §2.1.2 item 7; [Woolf et al. 2017 open-source reactor](https://doi.org/10.1002/bbb.1814)).
- EBC: no uncombusted pyrolysis-gas release; fossil fuel banned for reactor heat except preheat; electric heat must be renewable/surplus ([EBC §8.1–8.4](https://www.european-biochar.org/media/doc/7/ebc_en_10_5_red.pdf)).

---

## 5. Link to permanence and contaminants

| Higher peak T / longer residence | Typical effect | Notes |
|---|---|---|
| H/C_org, O/C_org | ↓ | [[H-Corg and O-Corg]] |
| \(F_\mathrm{perm}\) | ↑ | [[Woolf IPCC Fperm]] |
| Mass yield | Often ↓ | Trade-off vs C per tonne feedstock |
| BET surface area | ↑ then may ↓ at very high T | [[Properties]] |
| PAH | **Not** a simple T function—**vapor condensation** dominates | [[PAHs]] |

---

## 6. Practice takeaway

1. Log **peak T + residence + feedstock blend** for every batch (EBC Biochar Tool culture).
2. Prefer measured **H/C_org** over T-class alone for CDR math ([[Woolf IPCC Fperm]]).
3. Design **vapor–solid separation** before cooling to control PAHs ([[PAHs]]).

---

## Primary links

- [Woolf et al. 2021](https://doi.org/10.1021/acs.est.1c02425)
- [IPCC 2019 App. 4](https://www.ipcc-nggip.iges.or.jp/public/2019rf/pdf/4_Volume4/19R_V4_Ch02_Ap4_Biochar.pdf)
- [Keiluweit et al. 2010](https://doi.org/10.1021/es9031419)
- [EBC 10.5E](https://www.european-biochar.org/media/doc/7/ebc_en_10_5_red.pdf)
- [Cornelissen et al. 2016 Kon-Tiki](https://doi.org/10.1371/journal.pone.0154617)

## Related notes

- [[Production]] · [[Biochar Quality from Process]] · [[Gasification Residues]] · [[PAHs]] · [[Production Hub]]
