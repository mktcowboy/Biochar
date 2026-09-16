---
tags: [production, quality, process]
aliases: [Process effects on biochar, Quality from pyrolysis]
updated: 2026-09-16
---

# Biochar Quality from Process

Chapter mapping **process settings → material quality**: elemental ratios, pH, surface area, volatile matter, nutrients, and contaminant risk. Bridges [[Production]] / [[Pyrolysis Systems and Temperatures]] to [[Properties]] and [[Contaminants and Quality]]. Report context: **2026-09-16**.

**Related notes:** [[H-Corg and O-Corg]] · [[Permanence]] · [[PAHs]] · [[Heavy Metals and Ash]] · [[Testing EBC IBI S668]] · [[Production Hub]] · [[Key Sources]]

---

## 1. Causal chain

```
Feedstock chemistry + Peak T + Residence + Heating rate + Vapor path
        → molecular structure (Keiluweit transitions)
        → H/C_org, O/C_org, FC, ash%, pH, SA, VM
        → permanence proxies + agronomic behavior + contaminant load
```

Molecular transitions with charring temperature: [Keiluweit et al. 2010](https://doi.org/10.1021/es9031419). Inventory mapping of T / H/C → \(F_\mathrm{perm}\): [[Woolf IPCC Fperm]].

---

## 2. Carbonization intensity

| Process direction | H/C_org & O/C_org | Aromatic condensation | Typical \(F_\mathrm{perm}\) | Mass yield |
|---|---|---|---|---|
| Milder / shorter | Higher | Lower | Lower | Higher |
| Harsher / longer | Lower | Higher | Higher | Lower |

([Keiluweit 2010](https://doi.org/10.1021/es9031419); [Woolf 2021](https://doi.org/10.1021/acs.est.1c02425)). EBC uses **H/C_org < 0.7** as the universal carbonization gate; **< 0.4** for FeedPlus / manure safety proxy ([EBC 10.5E](https://www.european-biochar.org/media/doc/7/ebc_en_10_5_red.pdf) §7.2, §10.4).

FC sensitivity to T is **weak for high-ash feedstocks** because ash concentration offsets organic C enrichment ([Woolf 2021](https://doi.org/10.1021/acs.est.1c02425) §3.1)—measure FC directly when ash is high.

---

## 3. pH, surface area, volatile matter

- **pH / liming:** many lignocellulosic biochars become alkaline as acidic functional groups are lost and ash oxides/carbonates remain ([[Properties]]; agronomic liming narrative in [[Soil and Agriculture]]).
- **BET surface area:** generally rises with T into mid/high range, then can collapse at very high T as pores sinter ([[Properties]]; measurement caveats in [S668](https://biochar.org/wp-content/uploads/2026/05/ANSI-S668.pdf) §11.3 and [EBC §7.9](https://www.european-biochar.org/media/doc/7/ebc_en_10_5_red.pdf)).
- **Volatile matter / labile C:** higher at low T → more short-term mineralization and immobilization risk ([[Zimmerman 2010]] pattern via [DOI](https://doi.org/10.1021/es903140c); inoculation context [[Biochar Inoculation for Fertilizer]]).

---

## 4. Contaminants as process quality signals

| Contaminant class | Process lever | Feedstock lever |
|---|---|---|
| **PAHs** | Vapor residence, condensation on cooling char, quench design | Weak (EBC: negligible influence) |
| **Heavy metals** | Mostly conserved/concentrated (Hg volatilizes) | Dominant |
| **Dioxins/PCBs** | Same vapor-condensation pathway as PAHs; test if Σ8 EFSA PAH high | Cl-rich / contaminated feeds |
| **PFAS** | High T + residence can remove from solid; may transfer to liquids/gas | Biosolids / contaminated wastes |

Deep chapters: [[PAHs]] · [[Heavy Metals and Ash]] · [[PFAS and Emerging Contaminants]]. EBC PAH narrative: [EBC 10.5E §7.11](https://www.european-biochar.org/media/doc/7/ebc_en_10_5_red.pdf).

---

## 5. Homogeneity and batch control

Quality is only as good as **batch definition**: same feedstock blend (±20% composition), same T window, documented interruptions ([EBC §5](https://www.european-biochar.org/media/doc/7/ebc_en_10_5_red.pdf)). Solid-phase electrical conductivity helps compare within-batch homogeneity ([EBC §7.8](https://www.european-biochar.org/media/doc/7/ebc_en_10_5_red.pdf)). Start-up/shut-down char may need segregation from Agro/Feed grades ([EBC §5.5](https://www.european-biochar.org/media/doc/7/ebc_en_10_5_red.pdf)).

---

## 6. Practice takeaway

1. Specify **T, residence, feedstock, vapor path** in specs—not “biochar” alone.
2. Release products against **H/C_org + contaminant package + FC**, not temperature warranty alone ([[Testing EBC IBI S668]]).
3. For CDR contracts, pair process logs with Woolf/IPCC permanence inputs ([[Permanence]]).

---

## Primary links

- [Keiluweit et al. 2010](https://doi.org/10.1021/es9031419)
- [Woolf et al. 2021](https://doi.org/10.1021/acs.est.1c02425)
- [Zimmerman 2010](https://doi.org/10.1021/es903140c)
- [EBC 10.5E](https://www.european-biochar.org/media/doc/7/ebc_en_10_5_red.pdf)
- [ANSI S668](https://biochar.org/wp-content/uploads/2026/05/ANSI-S668.pdf)

## Related notes

- [[Production]] · [[Properties]] · [[Contaminants and Quality]] · [[Pyrolysis Systems and Temperatures]]
