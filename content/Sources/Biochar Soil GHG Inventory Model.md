---
tags: [source, science, carbon-markets]
aliases: ["soil GHG inventory model", "biochar GHG inventory"]
source_type: model
peer_reviewed: true
authors: ["Woolf, Dominic", "Lehmann, Johannes", "Ogle, Stephen", "Kishimoto-Mo, Ayaka W.", "McConkey, Brian", "Baldock, Jeffrey"]
year: 2021
title: "Greenhouse Gas Inventory Model for Biochar Additions to Soil"
venue: "Environmental Science & Technology 55(21): 14795–14805"
doi: "10.1021/acs.est.1c02425"
url: "https://doi.org/10.1021/acs.est.1c02425"
checked_against: full text
verified: 2026-09-16
updated: 2026-09-16
---

# Biochar Soil GHG Inventory Model

**Citation:** Woolf D, Lehmann J, Ogle S, Kishimoto-Mo AW, McConkey B, Baldock J (2021). Greenhouse gas inventory model for biochar additions to soil. *Environmental Science & Technology* 55(21): 14795–14805. [https://doi.org/10.1021/acs.est.1c02425](https://doi.org/10.1021/acs.est.1c02425) · open copy: [Canada federal science repository PDF](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)

This note is a plain-language walkthrough of that paper: what problem the authors were trying to solve, what you actually type into the method, what comes out, and what they deliberately refused to count. Every number below is from the paper itself ([DOI](https://doi.org/10.1021/acs.est.1c02425); [open PDF](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)). Companion science notes — [[Permanence Factors Fperm]], [[H-Corg and O-Corg]], [[Soil Temperature and Environment]], [[Permanence]], [[Nitrous Oxide Fluxes]], [[Methane Fluxes]], [[Priming and SOC Interactions]] — go deeper on each piece. This chapter stays with Woolf et al. 2021 as a standalone method.

---

## 1. Why they wrote it

Climate policy now assumes we will have to *remove* some carbon dioxide from the air, not only cut emissions. Biochar is one of the few removal practices that already exists at commercial scale: grow plants, heat the biomass with almost no oxygen, and put the resulting solid into soil so that a large share of that carbon stays out of the atmosphere for a long time ([abstract](https://doi.org/10.1021/acs.est.1c02425)).

By 2021 there was still no simple, general way to *count* that soil carbon. Life-cycle studies existed, but each one described a particular plant, a particular feedstock, and a particular field. Global potential papers used rough permanence assumptions that did not change with feedstock, kiln temperature, chemistry, or climate. The [[IPCC Biochar Soil Carbon Method|estimates soil C stock change from biochar]] had sketched a national-inventory method, but it lived in an annex that was not yet “good practice,” it used only pyrolysis temperature to judge persistence, and it did not let a user with lab data do any better ([§1](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)).

Woolf and colleagues set out to fill that gap with an **emission-factor model**: a short equation that a farm, a supply chain, a national inventory, or a carbon-market protocol can run with data that are actually collectable. National inventories often do not know the soil type or cropping details of every field that received biochar. Projects in places without easy lab access may know only the feedstock and the kiln temperature. The method is built so that those users can still produce a number, and so that users who *do* have elemental analysis can tighten the estimate ([§1](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)).

The authors’ own one-sentence claim is that carbon content of biochar ranges from **7%** (gasified biosolids) to **79%** (wood pyrolysed above 600 °C), and that of that initial carbon, **63–82%** remains unmineralized after 100 years at the global mean annual cropland temperature of **14.9 °C** ([abstract](https://doi.org/10.1021/acs.est.1c02425)). The rest of this chapter unpacks how they got there and how to use the result.

Typical users they name in the introduction are national greenhouse-gas inventories, voluntary and compliance carbon markets, and life-cycle analysts who need a soil-C module they did not have to build themselves ([§1 and §3.5](https://doi.org/10.1021/acs.est.1c02425)). A farm can run it too: the inputs are a truck ticket, a feedstock name, a kiln temperature or a lab sheet, and a climate normal.



---

## 2. What this method is not

Three boundaries matter, and mixing them up is how people mis-quote the paper.

**It is not a life-cycle assessment of the whole biochar plant.** The method counts the *direct* effect of putting biochar into mineral soil: the carbon that stays in the char, plus a small optional nitrous-oxide term. It does not add or subtract kiln methane, diesel for trucks, fertilizer displaced, energy co-products, or the carbon that would have stayed in the raw biomass if you had left it in the field. Those fluxes belong in other IPCC inventory chapters (energy, waste, land use) or in a separate LCA. Japan’s J-Credit scheme, which the paper cites as an example, required an LCA *on top of* the inventory model when it registered “biochar addition to mineral soil” ([§2.1.2 and §3.5](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)).

**It is not a farm recipe.** Nothing in the paper tells you how many tonnes to spread, whether to band or broadcast, or whether maize will yield more. Application mass is an *input* the user already has. Agronomy lives in [[Application Rates and Methods]] and [[Crop Yield Effects]].

**It applies only to mineral soils.** The authors refuse to run the method on organic soils (Histosols) or on forest soils that have a distinct organic horizon, because positive priming — speeding up loss of the native soil carbon — cannot be ruled out there. One often-cited charcoal-in-forest-humus study (Wardle et al. 2008) reported large carbon losses, and although that study could not separate charcoal decay from leaching or from native-humus loss, the inventory method stays off those soils on purpose ([§3.3.1](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)). See [[Priming and SOC Interactions]].

Two process types are also out of scope. **Torrefaction** and **hydrothermal carbonization** usually run below 350 °C and do not make a solid that lasts much longer in soil than the original biomass, so they are excluded. The method covers **pyrolysis** (almost no oxidant) and **gasification** (enough oxidant to make syngas, but not enough to burn the solid) ([§2.1.1](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)).

---

## 3. What you need to know to run it

The inventory reduces to one idea: how much *organic carbon* you put in the ground, multiplied by the fraction of that carbon that is still there after a chosen number of years, converted to carbon dioxide equivalent. In the paper that is equation 6 ([§3.4](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)):

> avoided GHG (as CO₂e) ≈ (44/12) × mass of biochar × carbon fraction × permanence factor, plus an optional first-year N₂O term.

The only activity data a compiler *must* collect are ([§2.1.3](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)):

1. **Mass of biochar added to soil** (dry basis). Someone has to weigh or ticket this. The method does not estimate it.
2. **Feedstock class** — wood, maize stover, manure, sewage sludge, and so on — so the carbon fraction can be looked up if it was not measured.
3. **Pyrolysis temperature**, or, better, the biochar’s **H/C_org** from a lab. Temperature is binned into low (**350–450 °C**), medium (**450–600 °C**), and high (**≥600 °C**) ([§3.1](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)).
4. **Mean annual soil temperature** at the application site, so the permanence factor can be read from the right row of Table 3. If you do not have a local number, the paper’s default is **14.9 °C**, the spatial mean of the world’s croplands ([§2.3](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)). US croplands sit at **10.9 °C** in the same table ([Table 3](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)).

If the lab already measured organic carbon content, use that measured **F_C** and skip the feedstock look-up. If it measured **H/C_org**, use that for permanence and skip the temperature bin. If you have *neither* temperature nor H/C_org, the paper says to use the **low-temperature** permanence factor — the conservative end of the range ([§3.2 and §3.4](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)).

The 44/12 factor is the usual conversion from a mass of carbon to a mass of carbon dioxide (CO₂ is 44 g mol⁻¹; C is 12 g mol⁻¹).

---

## 4. Carbon fraction of the biochar — wood vs manure vs sludge

Biochar is not a fixed percentage carbon. The abstract’s range, **7% to 79%**, is the whole story in one line ([abstract](https://doi.org/10.1021/acs.est.1c02425)). Table 2 then breaks that range into feedstock × process so an inventory compiler can pick a number ([Table 2](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)).

**F_C** in the paper is the *organic* carbon mass fraction on a **dry-mass** basis — grams of organic carbon per gram of dry biochar, ash included. That is the number that multiplies the truckload.

### 4.1 Why ash dominates the differences

Woody feedstocks are already low-ash. In the Phyllis2 biomass compilation the authors use, wood averages **2.2%** ash on a dry basis, maize stover **5.2%**, manure **28.5%**, paper sludge **32.7%**, and sewage sludge **39.4%** ([Table 1](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)). Ash does not burn away during pyrolysis; it is conserved, so as organic matter leaves as gas, the ash *concentrates* in the solid. A high-ash feedstock therefore produces a high-ash biochar, and F_C on a dry-mass basis falls even if the organic part of the char is very carbon-rich.

The organic fraction itself *does* get richer in carbon as temperature rises. The authors estimate that dry-ash-free carbon content with an exponential fit to a 128-measurement meta-analysis (R² = 0.65) ([§2.2](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)). But on a dry-mass basis that gain is partly cancelled by the extra ash, so Table 2’s F_C barely moves with temperature for manure and sludge, and only modestly for wood. That is why the [[IPCC Biochar Soil Carbon Method|estimates soil C stock change from biochar]] was willing to publish a single F_C per feedstock. Woolf still prefers the temperature-specific column when you already know the kiln temperature, because you get a little more accuracy at no extra data cost ([§3.1](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)).

Lignin matters for *yield* (how much solid you get), not for F_C directly. Wood and pits/shells/stones are lignin-rich (**24.7%** and **33.2%**); sewage sludge is lignin-poor (**6.0%**) ([Table 1](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)). Higher lignin, all else equal, leaves more solid.

### 4.2 Table 2 in words

All values below are F_C on a dry-mass basis, with standard deviations in the paper’s parentheses omitted here for readability. Full table: [open PDF, Table 2](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content).

| Feedstock | Low T (350–450 °C) | Medium (450–600 °C) | High (≥600 °C) | Pyrolysis mean | Gasification |
|---|---|---|---|---|---|
| Wood | **0.70** | **0.77** | **0.81** | **0.76** | **0.63** |
| Pits / shells / stones | 0.67 | 0.73 | 0.76 | 0.72 | 0.52 |
| Bamboo | 0.66 | 0.72 | 0.75 | 0.71 | 0.51 |
| Maize stover | 0.63 | **0.68** | 0.70 | 0.67 | 0.45 |
| Herbaceous (grasses, forbs, leaves; not rice) | 0.60 | 0.65 | 0.66 | 0.64 | 0.38 |
| Wheat straw | 0.59 | 0.64 | 0.65 | 0.63 | 0.38 |
| Bagasse | 0.57 | 0.62 | 0.64 | 0.61 | 0.43 |
| Rice hulls and straw | 0.46 | 0.48 | 0.48 | 0.47 | 0.20 |
| Manure | **0.39** | **0.39** | **0.39** | **0.39** | **0.14** |
| Paper sludge | 0.39 | 0.41 | 0.42 | 0.41 | 0.12 |
| Sewage sludge | **0.35** | **0.37** | **0.38** | **0.37** | **0.10** |

Read the table as three stories.

**Wood is the carbon-dense end.** High-temperature wood biochar is **81%** organic carbon by dry mass; the pyrolysis mean is **76%**. That **0.81** is *not* the same statistic as the abstract’s **79%**, which is the top of a broader observed range. Quote Table 2 when you need a class default ([Table 2](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content); [abstract](https://doi.org/10.1021/acs.est.1c02425)).

**Manure and sludge are the ash-dense end.** Manure pyrolysis biochar sits at **39%** carbon at every temperature class; sewage sludge at **35–38%**. Gasifying those feedstocks without removing the ash drops F_C to **0.14** (manure) and **0.10** (sewage sludge) — the abstract’s “7%” biosolids case lives in this neighbourhood ([abstract](https://doi.org/10.1021/acs.est.1c02425); [Table 2](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)). The paper notes that such residues may equally be called “ash with biochar” or “high-ash biochar”; there is no standard name. Because the method only credits *organic* carbon, extra ash does not change the carbon-sequestration arithmetic, even if the ash is useful as a lime or nutrient source ([§3.1](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)).

**Gasification is not a synonym for high-temperature pyrolysis.** Gasification chars are typically made hotter, so the organic carbon that remains can be highly condensed (low H/C_org, high persistence). But if the ash has not been separated, F_C is much lower than the matching pyrolysis class. If the ash *has* been partly or fully removed, **do not use Table 2** — measure carbon content directly ([§3.1](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)).

Food waste and other highly variable feedstocks are not in Table 1 or Table 2; the paper says F_C then has to be measured ([§2.2](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)).

---

## 5. Permanence (F_perm): the fraction that is still there

[[Permanence]] here means: of the organic carbon you put in the soil, what fraction has *not* yet been mineralized back to CO₂ after some number of years, at some soil temperature. The paper calls that fraction **F_perm**. It is the inventory’s way of compressing a slow decay curve into one number, the same way a 100-year global warming potential compresses a gas’s radiative effect into one number ([§2.3](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)). Deep dive on the tables: [[Permanence Factors Fperm]]. Deep dive on climate: [[Soil Temperature and Environment]]. Deep dive on the chemistry proxy: [[H-Corg and O-Corg]].

### 5.1 Two pools, not one

Biochar is a mixture. Some of it is still aliphatic or only partly carbonized and decays in months to years. Some of it is fused aromatic carbon that microbes oxidize much more slowly. A single exponential cannot describe both, so the authors fit **at least a two-pool** (fast + slow) exponential decay model to published mineralization studies, and a three-pool model when two pools were a poor fit. They only used studies with **at least one year** of decay data, so the slow pool is actually constrained ([§2.3](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)).

That is also why a 20-year or 50-year “remaining fraction” would look too flattering. The labile pool is mostly gone by then; the slow pool has barely started. The authors recommend a **100-year** horizon for the same reason UNFCCC uses 100-year GWPs: long enough to see century-scale climate, short enough to match the policy window we are actually managing. Using a shorter horizon would overstate mitigation over the coming century. Using 500 or 1,000 years would understate the next hundred years, which is what current climate policy is about. They still *publish* 500- and 1,000-year factors so users who need them can be honest, and they note that if biochar became a large mitigation item, 22nd-century inventories would have to start counting the slow leak as a CO₂ source ([§2.3](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)).

### 5.2 Headline 100-year values at 14.9 °C

At the global cropland mean of **14.9 °C**, Table 3 gives ([Table 3](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content); [abstract](https://doi.org/10.1021/acs.est.1c02425)):

| Class | Peak pyrolysis T | F_perm after 100 years (SE) |
|---|---|---|
| Low | 350–450 °C | **0.63** (0.045) |
| Medium | 450–600 °C | **0.71** (0.03) |
| High | ≥600 °C | **0.82** (0.028) |

That is the abstract’s “**63–82%** remains after 100 years.” It is *not* a claim that the carbon is permanent. It is a claim about one climate and one time horizon.

### 5.3 Longer horizons at the same temperature

Keep soil temperature at 14.9 °C and stretch the clock ([Table 3](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)):

| Horizon | Low | Medium | High |
|---|---|---|---|
| 100 years | 0.63 | 0.71 | 0.82 |
| 500 years | **0.19** | **0.32** | **0.44** |
| 1,000 years | **0.084** | **0.16** | **0.25** |

High-temperature char that is 82% still there at 100 years is only **25%** still there at 1,000 years, under this decay model, in an average cropland climate. That drop is the quantitative heart of [[Permanence Debates]]: a 100-year inventory factor and a millennial “permanent” claim are not the same number, and this paper’s own table says so.

### 5.4 Soil temperature moves the answer a lot

Decay studies in the literature were run at many temperatures. The authors rescale every study to a common soil temperature using a temperature-dependent Q10, after Lehmann et al. (2015):

> Q10 = 1.1 + 12.0 × e^(−0.19 T)

([§2.3](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)). Q10 here means “how many times faster decay gets when the soil is 10 °C warmer.” It is *not* a constant 2; it is larger in cold soil and smaller in warm soil, which is why a single “double every 10 degrees” rule would mis-scale the data.

For the **high-temperature** class over 100 years, Table 3 then reads ([Table 3](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)):

| Soil T | High-class F_perm (100 years) |
|---|---|
| 5 °C | **0.94** |
| 10 °C | **0.88** |
| 10.9 °C (US cropland mean) | **0.87** |
| 14.9 °C (global cropland mean) | **0.82** |
| 20 °C | **0.79** |
| 25 °C | **0.76** |

A high-T char in a cool soil (5 °C) is credited at **94%** remaining after a century; the same class in a hot soil (25 °C) is credited at **76%**. Always state **horizon + soil temperature** with an F_perm number. The paper’s supporting spreadsheet can recompute F_perm at any temperature and any time period ([SI from the ACS page](https://doi.org/10.1021/acs.est.1c02425)).

Low-temperature char is even more sensitive: 100-year F_perm falls from **0.84** at 5 °C to **0.54** at 25 °C ([Table 3](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)).

### 5.5 H/C_org is preferred over kiln temperature when you have lab data

Pyrolysis temperature is a *proxy* for how condensed the char is. For a given residence time, hotter usually means more fused aromatic rings, fewer C–H bonds, slower decay. But residence time, heating rate, and other process details also change condensation, so temperature is a noisy predictor. The molar hydrogen-to-organic-carbon ratio, **H/C_org**, tracks condensation more directly: as aromatic sheets grow, carbon-to-carbon bonds replace carbon-to-hydrogen bonds, and H/C_org falls ([§3.2](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)). See [[H-Corg and O-Corg]].

The paper therefore offers two parameterizations of F_perm:

- **Temperature class** — look up low / medium / high in Table 3.
- **H/C_org regression** — F_perm = intercept + slope × (H/C_org), with intercept and slope taken from the right-hand columns of Table 3 for the chosen soil temperature and horizon. The slope is negative: more hydrogen per carbon means less permanence. At **14.9 °C** and **100 years**, the intercept is **1.04** and the slope is **−0.64** (R² = **0.32**). All of these linear fits are significant at *p* < 0.001 ([Table 3 and eq. 5](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)).

**H/C_org is preferred over O/C_org** as well, especially for high-ash chars. Inorganic oxygen in ash is hard to tell from organic oxygen, so O/C_org is confounded by ash. Hydrogen is not present in ash in significant amounts, so H/C_org stays a cleaner condensation proxy for manure, sludge, and gasification residues ([§3.2](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)). That is why a gasification char can have a *low* carbon fraction and still a *high* F_perm: the organic carbon that is there is highly condensed.

The recommended order of operations is therefore ([§3.4](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)):

1. Measured F_C and measured H/C_org, if you have them.
2. Else F_C from Table 2 and F_perm from the temperature class in Table 3.
3. Else the **low-temperature** F_perm as a conservative default.

Figure 1’s middle panel also reports wildfire and other uncontrolled pyrogenic carbon, where neither temperature nor H/C_org is known and physical movement cannot be separated from mineralization: mean remaining carbon after 100 years at 14.9 °C is **56%**. That is a lower-bound persistence for “char we did not make on purpose,” not a number to use for engineered biochar ([Figure 1](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)).

---

## 6. What they left out on purpose

The paper lists a long menu of greenhouse-gas effects that a *full* biochar system can have: soil N₂O and CH₄, avoided decay of the original biomass, extra plant growth, priming of native soil carbon, less fertilizer manufacture, bioenergy co-products, kiln methane if the plant is leaky, land-use change if the feedstock is unsustainable, and transport ([§2.1.2](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)). For this *inventory* method they keep only what they can defend with meta-analytic significance, and they set the rest to zero. That is a conservative choice, not a claim that those effects are physically zero.

### 6.1 Priming is not credited

Biochar can speed up or slow down the decay of the native, non-pyrogenic soil carbon. Faster decay is **positive priming**; slower is **negative priming**. A meta-analysis of 21 studies (Wang et al. 2016, cited in the paper) reported a mean **4% decrease** in native-SOC mineralization with biochar, but the 95% confidence interval included zero. Modelling, long incubations, and long field studies all *suggest* that priming becomes more negative over years, which would add to the climate benefit. Because the net effect was not significant at *p* < 0.05 in the available metas, **priming is omitted**. Future methods could fold it into a dynamic SOC model or a multiplicative stock correction; this one does not ([§3.3.1](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)). Agricultural framing: [[Priming and SOC Interactions]].

The mineral-soil restriction in §2 is the other half of this choice. On organic soils and forest organic horizons, positive priming is the risk they will not take.

### 6.2 Methane is assumed to be zero

Field papers go both ways on methane. One meta-analysis found paddy CH₄ **up 19%**; another found paddy CH₄ **down**; a third found **negligible** change. Across all studies, none of those metas found a significant net change. The inventory therefore assumes **no net change in soil CH₄** ([§3.3.3](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)). That is an accounting default, not a prediction that your paddy will be unchanged. See [[Methane Fluxes]] for the flooded-versus-upland split this paper refused to parameterize.

### 6.3 Nitrous oxide: first year only, and only at high rates

Biochar often cuts soil N₂O, but the size of the cut depends on how you average the literature, and the cut fades. The paper walks through three inverse-variance metas: [[Nitrous Oxide Mitigation Meta-analysis|meta-analyzes N2O mitigation]] **−54%** (n = 261, 30 studies), Verhoeven et al. **−12.4%** (n = 122, 40 studies), and Borchard et al. **−38%** (n = 435, 48 studies). Inverse-variance weighting treats many treatments from the same site as independent. When Verhoeven re-weighted by the inverse of observations-per-site, the effect shrank to **−9.2%** and was no longer significant at *p* < 0.05 ([§3.3.2](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)).

Persistence over time is the other problem. The N₂O reduction has not been shown to be statistically significant after **one year**, partly because the effect gets smaller and partly because long field series are scarce ([§3.3.2](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)).

So the inventory rule is narrow:

- Count N₂O only in **year 1**.
- Count it only where application exceeds **10 Mg C ha⁻¹** (ten tonnes of biochar *carbon* per hectare, not ten tonnes of biochar).
- Use a field-trial-only re-fit of the Borchard data set, pots and incubations dropped, analysed with robust variance estimation and study as a random effect: **−23%** (95% CI **5–41%**).
- Apply that percent to the *entire* direct N₂O flux from that land, not only to fertilizer N.

The authors then say the year-1 N₂O term is usually small next to the carbon term, so **including it is optional**. Omitting it barely changes the total ([§3.3.2](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)). Typical farm rates under NRCS CPS 336 often sit below 10 Mg C ha⁻¹, which means this optional term does not even unlock. Agricultural chapter: [[Nitrous Oxide Fluxes]].

For the conversion of N₂O to CO₂e they recommend the latest IPCC 100-year GWP, which at the time of writing was **273** (AR6). Their worked example still uses **298** (the older AR4/AR5 value) — quote whichever GWP you actually applied ([§3.4](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)).

---


### 6.4 The rest of the climate ledger (counted elsewhere)

Section 2.1.2 of the paper lists the other greenhouse-gas items a *system* study would still have to handle. Equation 6 ignores them on purpose; an LCA or a national inventory’s other chapters would pick them up ([§2.1.2](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)):

1. **Avoided decay or burning of the original biomass.** If maize stover would have been left to rot or burned, some N₂O and CH₄ would have been emitted. Diverting that stover into char avoids those emissions — but in a national inventory that shows up in the waste or agriculture chapters, not here.
2. **Extra plant growth.** Biochar can raise net primary productivity, which pulls more CO₂ out of the air, especially if the extra biomass is itself charred or used for bioenergy. The inventory does not credit that feedback.
3. **Less fertilizer manufacture.** If nutrient-use efficiency improves, fertilizer plants emit less. That is an industrial-sector effect.
4. **Bioenergy co-product.** Syngas or heat from the kiln can displace fossil fuels. Energy-sector accounting.
5. **Kiln leaks.** Roughly half of biomass carbon leaves as volatiles during pyrolysis. A well-run modern plant combusts those to CO₂; simple kilns can emit methane and other products of incomplete combustion. Those emissions belong to energy or industry, and they can erase a lot of the soil-C benefit if the kiln is dirty.
6. **Unsustainable feedstock.** Cutting live trees, or converting forest to biomass plantations, can lose vegetation carbon stocks that dwarf the char you make. Land-use chapters already have methods for that.
7. **Growing and hauling dedicated crops.** Residues and wastes are the clean case; purpose-grown biomass is not free.

The authors’ test for including any of these in *this* model was statistical significance in meta-analyses, not mechanistic plausibility. That is why a process everyone believes is real (negative priming, paddy methane) can still be set to zero here ([§3.5](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)).

---

## 7. Worked maize-stover example, in words

Section 3.4.1 of the paper walks through one calculation so a reader can see the moving parts. Here it is without the algebra-first presentation ([§3.4.1](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)).

A project pyrolyses **maize stover** at a peak temperature of **500 °C**. Nobody has measured the carbon fraction or H/C_org of this batch, so everything comes from the look-up tables.

500 °C is in the **medium** class (450–600 °C). Table 2 therefore gives F_C = **0.68**: each dry tonne of this biochar is 68% organic carbon by mass ([Table 2](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)).

The char is put into cropland whose mean annual soil temperature is **10 °C**, and the project wants a **100-year** permanence. Table 3 gives F_perm = **0.79** for medium-class char at 10 °C over 100 years ([Table 3](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)). In words: of the organic carbon that went into the soil, the model expects **79%** to still be there a century later in that climate.

The project applies **15,000 tonnes** of biochar on **1,000 hectares**. That is 15 tonnes of biochar per hectare. At F_C = 0.68, that is about **10.2 tonnes of carbon per hectare**, which is just over the **10 Mg C ha⁻¹** gate, so the optional N₂O term is allowed. The land receives **150 kg mineral N ha⁻¹ yr⁻¹** and no legumes or organic N. Using IPCC Tier 1 for baseline N₂O, the paper’s arithmetic is: 1,000 ha × 0.15 Mg N ha⁻¹ × 0.01 (emission factor) × 1.57 (N₂O / N₂O-N) = **2.4 Mg N₂O** from the land that received enough biochar ([§3.4.1](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)).

Carbon term, in words: 15,000 tonnes of biochar × 0.68 carbon × 0.79 remaining × 44/12 to convert C to CO₂ ≈ **29,546 tonnes CO₂e**. That is the sequestration credit for the char itself.

N₂O term, in words: 23% of 2.4 tonnes of N₂O, times a GWP of **298**, is about **164 tonnes CO₂e**. That is the optional avoided-N₂O bonus in year 1 only.

Add them: **29,710 Mg CO₂e** ([§3.4.1](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)).

Two things to notice. First, the carbon term is about **180 times** the N₂O term, which is why the authors call N₂O optional. Second, this 29,710 is *not* a life-cycle result. Kiln emissions, trucks, the maize stover you no longer left on the field, and any yield change are outside the equation. If you need those, you run an LCA with this inventory number as the soil-C piece.

If the same 15,000 tonnes had been high-temperature wood instead of medium maize stover, both F_C and F_perm would rise (wood high-T F_C **0.81**, high-class F_perm at 10 °C **0.88**), and the carbon term would be larger before any N₂O is added ([Table 2 and Table 3](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)). If they had been placed in 25 °C soil rather than 10 °C soil, medium-class 100-year F_perm would fall from **0.79** to **0.64**, and the credit would shrink ([Table 3](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)). That is the whole point of building temperature and chemistry into the look-up rather than publishing one global percentage.



---

## 8. How this sits next to IPCC 2019 and carbon-market methods

### 8.1 IPCC 2019 Appendix 4

This paper is an update and expansion of the [[IPCC Biochar Soil Carbon Method|estimates soil C stock change from biochar]], not a replacement that inventories are required to use. The appendix is still labelled a basis for *future* Tier 1 development, not complete good-practice guidance ([IPCC PDF](https://www.ipcc-nggip.iges.or.jp/public/2019rf/pdf/4_Volume4/19R_V4_Ch02_Ap4_Biochar.pdf)). Woolf adds three things the appendix did not have: an H/C_org pathway, an explicit soil-temperature grid, and emission factors refitted to a later decay compilation ([§1](https://doi.org/10.1021/acs.est.1c02425)).

The two 100-year tables should **not be mixed in one calculation**. IPCC’s factors, adjusted to a conservative ~**20 °C** basis, are **0.65 / 0.80 / 0.89** (low / medium / high) ([IPCC PDF](https://www.ipcc-nggip.iges.or.jp/public/2019rf/pdf/4_Volume4/19R_V4_Ch02_Ap4_Biochar.pdf)). Woolf’s factors at 14.9 °C are **0.63 / 0.71 / 0.82**; at 20 °C they are **0.57 / 0.67 / 0.79** ([Table 3](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)). Woolf is lower, even on a like-for-like 20 °C comparison, because the underlying decay data set was updated. Pick one stack and stay with it. Side-by-side: [[Permanence Factors Fperm]].

Shared vocabulary is the temperature bins (350–450 / 450–600 / ≥600 °C), the mineral-soil cropland/grassland scope, the two-pool decay idea, and the 100-year reporting convention.

### 8.2 Carbon markets — related math, not the same method

Several credit methodologies cite this paper or the same family of decay math. That does **not** mean they issue Woolf’s 100-year F_perm. Cross-link, do not overclaim. The map lives in [[Permanence Science for Credits]].

- **[[Puro CORC200+]] / [[Puro Biochar Methodology Edition 2025]]**. Puro’s 2022 methodology (CORC100+) used a Woolf-style multi-pool exponential with H/C_org and soil temperature. Edition 2025 moved to a revised **power-law** decay over **200 years**, an 80% confidence-interval lower bound, an H/C_org domain of 0–0.7, and a soil-temperature floor of 7 °C. Ro is encouraged but does not yet quantify credits. Puro is in the decay-model camp, not a verbatim Woolf table ([Puro permanence post](https://puro.earth/insights/post/biochar-permanence/); [[Puro.earth Overview]]).
- **[[Isometric Permanence Pathways 200y and 1000y]]**. Isometric’s *soil* module offers a **200-year** path that fits a conservative (about 17th-percentile) Woolf-style durability function with H/C_org and soil temperature, F capped at 0.95 and soil T floored at 7 °C, *or* a **1,000-year** path that uses random reflectance / inertinite instead of Woolf. Citing Woolf for Isometric is accurate only for the 200-year soil path ([Isometric soil module](https://registry.isometric.com/module/biochar-storage-soil-environments/1.3); [Woolf DOI](https://doi.org/10.1021/acs.est.1c02425)).
- **[[Verra VM0044 Permanence and Quantification]]**. VM0044’s Table 3 defaults are the IPCC 100-year temperature factors (0.89 / 0.80 / 0.65), with Woolf in the framing and as the reason torrefaction and HTC are excluded ([VM0044 v1.1 PDF](https://verra.org/wp-content/uploads/2023/07/VM0044-Methodology-for-Biochar-Utilization-in-Soil-and-Non-Soil-Applications-v1.1.pdf)).
- **[[CSI Global Biochar C-Sink]]**. CSI cites Woolf in the literature list but does **not** apply a global soil-temperature adjustment in v3.3 operations; its GPC/SPC split is H/C_org- and Ro/HyPy-based ([[CSI GPC vs SPC Permanence Classes]]).

The honest sentence is: Woolf 2021 is the peer-reviewed inventory model that a lot of market methods *grew from* or *argue with*. It is not the credit calculator.

---

## 9. Limitations the authors themselves list

Section 3.5 is the authors’ own research-needs list. Paraphrased in everyday language ([§3.5](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)):

1. **N₂O after year 1.** A first-year cut is now clear in field data. There are not enough long field trials, and not enough mechanism, to predict N₂O in year 2 and beyond. That is why they stop at year 1.
2. **Methane.** Many papers report a change; too few agree on the *sign* under given field conditions. That is why they set CH₄ to zero rather than guess.
3. **Priming over decades.** Long incubations, soils with historical pyrogenic carbon, and models all point toward negative priming adding native-SOC stocks in the long run. The size is still too loosely constrained to put a number in an inventory factor. Dynamic SOC models that actually contain a biochar interaction are the proposed next step.
4. **Environment beyond temperature.** Texture, moisture, and the ash chemistry of the char itself almost certainly change decay. The current F_perm grid only rescales for temperature. More decomposition studies are needed before those covariates can join the look-up table.
5. **Future warming.** Because decay is temperature-sensitive, today’s F_perm tables will overstate permanence if soils warm and the temperature input is not updated. The method can take a new temperature; it does not forecast one.
6. **Conservative by design.** Each of the omissions above is resolved by counting *less* benefit, not more. The authors’ closing claim is that the method can already be used “with confidence that it will not be overestimating the mitigation impact of biochar additions” ([§3.5](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)).

Practical cautions that follow from the paper even when they are not labelled “limitations”:

- Do not apply the method to Histosols or forest soils with an organic horizon ([§3.3.1](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)).
- Do not treat torrefied or hydrochar solids as biochar under this method ([§2.1.1](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)).
- Do not use Table 2 F_C for gasification char after ash has been removed — measure it ([§3.1](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)).
- Do not quote the abstract’s 79% carbon and Table 2’s 0.81 high-T wood F_C as if they were the same statistic ([abstract](https://doi.org/10.1021/acs.est.1c02425); [Table 2](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)).
- Do not paste a 100-year F_perm onto a 1,000-year credit claim, or a 14.9 °C factor onto a tropical field, without saying so ([Table 3](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)).

---


## 10. How to quote this paper without mixing statistics

Three mix-ups show up constantly in slide decks. The paper itself gives you the material to avoid all three ([DOI](https://doi.org/10.1021/acs.est.1c02425)).

**Carbon content is not permanence.** A high-temperature wood char that is **81%** carbon (Table 2 F_C) is not “81% permanent.” Permanence is F_perm, a different fraction, applied *to* that carbon. At 14.9 °C over 100 years the matching high-class F_perm is **0.82**, so the inventory carbon is roughly 0.81 × 0.82 ≈ **66%** of the dry mass of that char, expressed as carbon that is still expected to be in the soil after a century, before you convert to CO₂e ([Table 2 and Table 3](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)).

**The abstract’s 79% and Table 2’s 0.81 are different jobs.** 79% is the top of an observed carbon-content range in the abstract. 0.81 is the modelled class default for high-temperature wood on a dry-mass basis. Use the abstract for the span; use Table 2 for a look-up ([abstract](https://doi.org/10.1021/acs.est.1c02425); [Table 2](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)).

**A 100-year factor is not a 1,000-year factor.** High-class F_perm at 14.9 °C is **0.82** at 100 years and **0.25** at 1,000 years. Credit methodologies that issue on a 200-year or 1,000-year horizon are doing extra work (or different science) on top of this paper. Point to [[Puro CORC200+]] or [[Isometric Permanence Pathways 200y and 1000y]] for those rules; do not stretch Table 3 by hand ([Table 3](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)).

If you need one spoken sentence: *Woolf 2021 is a mineral-soil inventory method in which biochar mass × organic-carbon fraction × a temperature- and chemistry-dependent remaining fraction, usually over 100 years, is the carbon credit to the soil; N₂O is optional, methane and priming are left at zero, and the whole plant LCA sits somewhere else.*

---

## 11. Supporting spreadsheet and IPCC-style tiers

The journal page hosts a supporting Excel file with the decay studies behind Table 3, the R code used for the N₂O effect size, and a calculator that recomputes F_perm for any time horizon and any soil temperature ([ACS supporting information](https://doi.org/10.1021/acs.est.1c02425)). Table 3 in the paper is the printed slice of that calculator at 5 °C steps plus the two cropland means.

The authors place the method in IPCC tier language so inventory compilers know what they are holding ([§1](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)):

- **Tier 1** is a linear emission-factor equation with default coefficients — exactly this paper’s Table 2 × Table 3 structure.
- **Tier 2** would replace those defaults with country-specific F_C or F_perm values, which this paper’s H/C_org pathway already invites if a country measures its chars.
- **Tier 3** would be a dynamic model run by specialists. The authors are not offering a Tier 3 model. They are offering a Tier-1-shaped tool that can absorb better chemistry when you have it.

They also remind readers that the 2019 IPCC annex was parked outside “good practice” because IPCC requires methods to already be supported in the peer-reviewed literature. This 2021 paper is part of that missing literature trail ([§1](https://doi.org/10.1021/acs.est.1c02425)). Whether a given country actually reports biochar in its UNFCCC inventory is a policy choice, not something the equation decides.

A last boundary that is easy to miss: if biochar is a **co-product of energy**, the paper says production emissions can be attributed to the energy, and only the *after-production* soil effects attributed to land application — but that allocation lives in the energy-sector inventory, not in equation 6 ([§2.1.2](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content)).

---

## 12. Numbers at a glance

| Figure | Value | Where |
|---|---|---|
| Carbon content range | **7%** (gasified biosolids) to **79%** (wood >600 °C) | [Abstract](https://doi.org/10.1021/acs.est.1c02425) |
| Wood F_C, low / med / high / mean / gasification | **0.70 / 0.77 / 0.81 / 0.76 / 0.63** | [Table 2](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content) |
| Manure F_C (any pyrolysis T) / gasification | **0.39 / 0.14** | [Table 2](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content) |
| Sewage-sludge F_C mean / gasification | **0.37 / 0.10** | [Table 2](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content) |
| Temperature classes | Low 350–450 °C; medium 450–600 °C; high ≥600 °C | [§3.1](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content) |
| 100-year F_perm at 14.9 °C | Low / medium / high **0.63 / 0.71 / 0.82** | [Table 3](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content) |
| 500-year F_perm at 14.9 °C | **0.19 / 0.32 / 0.44** | [Table 3](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content) |
| 1,000-year F_perm at 14.9 °C | **0.084 / 0.16 / 0.25** | [Table 3](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content) |
| High-class 100-year F_perm vs soil T | 0.94 at 5 °C; 0.88 at 10 °C; 0.87 at 10.9 °C; 0.79 at 20 °C; 0.76 at 25 °C | [Table 3](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content) |
| Q10 used to rescale studies | 1.1 + 12.0·e^(−0.19T) | [§2.3](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content) |
| H/C_org fit at 14.9 °C, 100 years | intercept **1.04**, slope **−0.64**, R² **0.32** | [Table 3](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content) |
| Wildfire / uncontrolled pyrogenic C remaining (100 years, 14.9 °C) | **56%** | [Figure 1](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content) |
| N₂O inventory term | **−23%** (95% CI 5–41%), year 1 only, only if **>10 Mg C ha⁻¹**; field trials only | [§3.3.2](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content) |
| Prior N₂O metas it weighs | Cayuela **−54%**; Verhoeven **−12.4%** (reanalysis **−9.2%**, ns); Borchard **−38%** | [§3.3.2](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content) |
| CH₄ | No net effect assumed | [§2.4, §3.3.3, §3.5](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content) |
| Priming | Not credited; meta mean −4% with CI crossing zero | [§3.3.1](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content) |
| Scope | Mineral soils only; not Histosols or forest soils with an organic horizon | [§3.3.1](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content) |
| Worked example | Maize stover, 500 °C, F_C 0.68, F_perm 0.79 at 10 °C; 15,000 Mg biochar + year-1 N₂O → **29,710 Mg CO₂e** | [§3.4.1](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content) |

---

## Primary links

- [DOI 10.1021/acs.est.1c02425](https://doi.org/10.1021/acs.est.1c02425) — journal record and supporting spreadsheet
- [Open PDF (Canada federal science repository)](https://open-science.canada.ca/server/api/core/bitstreams/112fc297-0352-4683-ae0e-dd1271f59d77/content) — full text used to check every figure above
- [[IPCC Biochar Soil Carbon Method|estimates soil C stock change from biochar]] — the 2019 annex this model extends ([PDF](https://www.ipcc-nggip.iges.or.jp/public/2019rf/pdf/4_Volume4/19R_V4_Ch02_Ap4_Biochar.pdf))

## Related notes

- Science: [[Permanence]] · [[Permanence Factors Fperm]] · [[H-Corg and O-Corg]] · [[Soil Temperature and Environment]] · [[Permanence Debates]] · [[CDR Potential and IPCC Accounting]] · [[Science Hub]]
- Soil GHG: [[GHG Fluxes]] · [[Nitrous Oxide Fluxes]] · [[Methane Fluxes]] · [[Priming and SOC Interactions]]
- Markets (pointer only): [[Permanence Science for Credits]] · [[Puro CORC200+]] · [[Isometric Permanence Pathways 200y and 1000y]] · [[Verra VM0044 Permanence and Quantification]] · [[CSI Global Biochar C-Sink]]
- Index: [[Key Sources]]
