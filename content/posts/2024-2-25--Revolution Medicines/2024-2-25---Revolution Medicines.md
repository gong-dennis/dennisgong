---
title: "Revolution Medicines"
date: "2024-02-25T12:00:00.000Z"
template: "post"
draft: False
slug: "/blog/RVMD/"
category: "Life Sciences"
tags:
  - "Life sciences"
  - "Healthcare"
description: "Stock analysis"
---

Revolution Medicines (\$RVMD) is a pharmaceutical company focused on RAS driven cancers. It was founded in 2014, and is worth early \$5 billion as of this writing. RVMD completed an acquisition of \$1.85 billion in cash (EQRx) which makes up their cash position as of Q4 2023 (EV = \$3.15 billion). They currently burn ~\$400 million annually, giving them a healthy 3-4 years of runway. The purpose of this post is to discuss the prospect of RVMD's RAS inhibitors in lung and pancreas cancers.


### RAS Biology ### 

RAS is a GTPase that act as binary switches during signal transduction to activate RAS/MAPK signaling. KRAS requires guanidine exchange factors (GEFs) to bind and cause a conformational change to turn them off, and analogously, GTPase activating proteins to switch them off. KRAS is mutated or amplified in >30% of patient tumors which leads to constitutive signaling in the (ON) state. Targeting KRAS is difficult because it is an intracellular protein (requiring a small molecule approach), and there is a lack of drug binding pockets on the protein. The protein is relatively smooth and has high affinity with its ligands GTP and GDP. RAS proteins also have high affinities for effector RAF kinases, which are in the 10–50 nM range. To therapeutically target the protein, groups have developed approaches to trap KRAS in the (OFF) conformation and now recently, methods for degrading the (ON) conformation. The goal overall is to limit the amount of time in the (ON) state as much as possible.

Here is a good [review](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5555610/).

Allele specific inhibitors like Adagrasib and Sotorasib trap KRAS G12C proteins in the (OFF) state, while RVMD has famously developed an [first in class inhibitor](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC10474815/) of RAS (ON). They did this by designing a molecule that remodels the surface of cyclosporin A to create a complex with high affinity and specificity for KRAS proteins with G12 mutations. This causes a steric clash that prevents binding of RAF effector proteins that continue the signaling cascade.

![Tri-complex](Tricomplex.jpg "Tricomplex")

RVMD makes the argument and provides data that the tricomplex approach is both faster and results in greater potency of inhibition of KRAS than allele specific inhibitors of the inactive (OFF) state. This is because the (ON) state is the effector state of the protein, and also because the tricomplex may provide a greater degree of steric hindrance than a pocket inhibitor might. At AACR 2024, preclinical modeling of a tricomplex inhibitor demonstrated that mechanisms of KRAS inhibitor resistance involving KRAS and KRAS effector pathways (ie. KRAS mutations, KRAS amplification, amplification/mutation of MAPK or PI3K signaling) are not observed in treatment resistant tumors. Rather, resistance mechanisms most commonly involve focal amplifications of Myc, Jun, and Yap/Taz/Tead signaling. 

Importantly, all mice treated with KRAS inhibitors relapse and KRAS inhibitors have been shown in some instances to only be cytostatic in nature. Inhibition of RAS signaling enables tumor regressions by engaging anti-tumor immunity. The growth promoting signaling components downstream of RAS involve immunosuppression via a variety of mechanisms such as downregulating MHC-I and recruitment of immunosuppressive cell types via chemokine secretion. 


### KRAS inhibition in PDAC

In PDAC, >90% of patient tumors have KRAS alterations. This is at similar levels to Philadelphia chromosome CML and suggests there is an [intrinsic dependency on KRAS for oncogenesis](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC9733946/). In PDAC tumor models, KRAS inhibition is remarkably effective, more than any other therapies or combinations of therapies. A tricomplex inhibitor, RMC-7977, which resembles the RMC-6236 drug currently in human clinical trials is studied extensively [here](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC10723304/), and a competitor G12D allele specific inhibitor from Mirati Therapeutics is studied [here](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC9900321/). Additional studies published at conferences and in preprints have detailed other characteristics of these compounds including resistance mechanisms, impact on the microenvironment, and combination strategies. Below are results of these compounds in human cell line xenografts.

![MRTX1133 xenograft panel](MRTX1133_xeno.jpg "MRTX1133 xenograft panel")

![RMC-7977 xenograft panel](Tricomplex_PDACXeno.jpg "RMC-7977 xenograft panel")

In human clinical trials, tricomplex inhibition has shown remarkable efficacy in heavily pretreated patients. This is comparable to results from sotorasib in pretreated advanced G12C mutated PDAC. The prognosis from treated patients remains bleak, however. In the advanced treated setting, KRAS inhibition is affording a meager mOS of 7 months with sotorasib (21% response rate) and from the early data from 6236, it doesn't look like the tumor regressions are significantly better.

![Phase I RMC-6236](RMC6236_PDAC.jpg "Phase I RMC-6236")

![Sotorasib PDAC](Sotorasib_PDAC.jpg "Sotorasib PDAC")

For reference, these are results from advanced PDAC patients in the untreated setting. 

![SOC PDAC](FOLFIRINOX_GEM_PDAC.jpg "SOC PDAC")

The role of KRAS inhibitors in PDAC in my view are in the adjuvant setting post surgery and also in combination with existing chemotherapy regimens. There has been interest in combining other targeted therapies or immunotherapies with KRAS inhibitor in search of synergy but according to Adam Palmer these [approaches are not promising](https://www.nature.com/articles/s43018-023-00667-z). 

### KRAS inhibition in NSCLC

KRAS is mutated in roughly 30% of NSCLC cases and most commonly at the G12C locus (40% of mutations) in contrast to PDAC where most mutations are at G12D. KRAS inhibition has admittedly also not been exciting thus far in NSCLC. Sotorasib, a G12C inhibitor, seemed to have equal or worse overall survival than docetaxel in first line patients.

![Soto1](SotoVsDocetaxel.jpg "Soto1")

![Soto2](SotoVsDocetaxel2.jpg "Soto2")

Adagrasib seems to be performing slightly better in G12C NSCLC, with a cleaner tox profile and as a result potential to be combined with immunotherapy. 

![Adagrasib 2 year followup in NSCLC](Adagrasib_NSCLC.jpg "Adagrasib 2 year followup in NSCLC")

![Adagrasib tox](Adagrasib_Tox.jpg "Adagrasib tox")

![Combination with PD-1 inhibitor](AdagrasibPD1.jpg "Combination with PD-1")

After adagrasib is divarasib, a G12C inhibitor from Roche/Genentech. This molecule looks the best of the three so far. 

![Divarasib NSCLC](Divarasib_NSCLC.jpg "Divarasib NSCLC")

RMC-6236 looks competitive with sotorasib and adagrasib but looks potentially beat by divarasib. All these studies are signal finding with few patients so hard to say definitively. 

![Phase I RMC-6236](RMC6236_NSCLC.jpg "Phase I RMC-6236")

KRAS amplifications or mutations were common mechanisms of resistance to all the allele specific inhibitors of KRAS (soto, ada, diva) and it remains to be seen what kinds of alterations are found in tricomplex resistant patients. RVMD has released several preclinical vignettes demonstrating combination approaches with RMC-6236. There is a doublet with an allele specific KRAS (ON) inhibitor they have developed (RMC-6291) and also an immunotherapy combination with PD-1 blocker pembrolizumab. 

![RMC-6236 Doublet](Doublet_NSCLC.jpg "Combination with allele specific RMC-6291")

![Combination immunotherapy](ImmunoComboNSCLC.jpg "Combination immunotherapy")

What to say about the opportunity in NSCLC? Given the competition, the success or failure of the drug seems highly dependent on clinical development strategy. The major question is how to carve out your share in a crowding landscape of KRAS inhibitors, chemotherapies, immunotherapies, and other targeted therapies. Try to run head to heads with ada and soto while pushing combination strategies to form a data moat that is hard to touch with comparable trials? The safety data look competitive with the allele specific inhibitors so perhaps the best path is to push ahead with the largest addressable market. It is scary days in oncology, where Enhertu level step changes are rare. These are developing markets where uncertainty means you have to gamble. For patients, at the very least you have another agent with monotherapy activity, but perhaps the biggest benefits are felt following patent expiry and physicians are comfortable adding them to first line combination regimens.

![RMC-6236 TRAE](RMC6236_TRAE.jpg "RMC-6236 TRAE")

~80% of treated patients are getting rash but generally safe as Gr3+ tox <5% at the optimized 300 mg dosage. 

### Pipeline

The flagship of RVMD's efforts is the multi-selective RAS (ON) inhibitor RMC-6236. The stated priority from the management team is to propel 6236 into one or more 2L indications in NSCLC, PDAC, or CRC, then roadmap potential 1L indications. The major sources of risk are tolerability in combination, for example with checkpoint blockade.

Pipeline
![RVMD Pipeline](pipeline.jpg "RVMD Pipeline")

Clinical development strategy
![Clinical development](clindev.jpg "RVMD Pipeline")

After 6236, RVMD is developing a suite of allele specific inhibitors, which curiously seem to be less potent than 6236, but with monotherapy data, could represent the backbone of a combination approach with 6236 (see the doublet approach in the above section). 

The most advanced of these allele specific inhibitors is the RAS(ON) G12C selective inhibitor RMC-6291 which is being developed in NSCLC and CRC.

![Phase I RMC-6291](RMC6291_CRC.jpg "Phase I RMC-6291")
![Phase I RMC-6291](RMC6291_NSCLC.jpg "Phase I RMC-6291")

Finally, there is a G12D selective inhibitor RMC-9805 which has preclinical data in a variety of G12D mutated xenografts.

![RMC-9805 xenografts](RMC9805_G12D_xeno.jpg "RMC-9805 xenografts")


### Conclusions

The company is clearly operating at a high level, commercializing a really exciting and novel class of compounds. There is tremendous academic excitement and the company has hit all major clinical development milestones, being 'first' in PDAC despite preclinical MRTX1133 data being published earlier. The initial cut of data from RMC-6236 was relatively underwhelming but with more time on drug, it is expected that the data will mature and improve.

We are understanding more and more about RAS inhibition and what kind of role it will play in practice, whether via RVMD or not. Unfortunately, RAS inhibition isn't as potent as was thought given the genetics of the disease. There could be use in the adjuvant setting given the monotherapy potency. But if you were to ask, "how big is your hammer?" KRAS inhibition definitely plays second or even third fiddle to advances in ADCs, immunotherapy, and other targeted therapies. KRAS inhibition is cytostatic and relies on immunity to clear disease.

The KRAS inhibitor landscape is growing rapidly, not only with the emergence of divarasib, but with new allele specific and pan-RAS inhibitors that are being disclosed each year. Different KRAS inhibitors have different safety profiles that make them more or less likely to be combined with other therapies like immunotherapy -- this may be the key difference maker.

What might a KRAS inhibitor be worth? Comparing the data package to clinical benefit and sales of [other oncology assets](https://xtalks.com/top-40-best-selling-cancer-drugs-in-2023-by-2022-data-3702/), do we really think that KRAS is a multibillion dollar opportunity for all parties involved? Analysts seem to think so, as Krazati peak sales estimates without indication expansion to CRC sits at \$1.7 billion. As a clinician, are you rushing to give your patient a RAS inhibitor? These drugs seem to have guaranteed resistance (no chance at a cure), and will inevitably be very expensive. 

Are there catalysts for this stock? The registrational trials all start in 2024 and hopefully have data in 2026. What will make RVMD the next \$10 billion oncology acquisition? Mirati was acquired for \$5.8 billion and RVMD is currently worth \$5 billion. For whatever reason, people really care about KRAS, despite the disappointing clinical data. In PDAC, I find it inevitable that every patient will be on a KRAS inhibitor, and RVMD is far and away in the lead there. That in itself is probably reason enough to be excited. At least this armchair analyst buys the story and is seriously looking forward to their success.