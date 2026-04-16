---
title: ADC payloads
date: 2026-04-21T12:00:00.000Z
template: post
draft: false
slug: /blog/ADCpayloads/
category: Life sciences
tags:
  - Life sciences
description: poisons
---
Cancer care is changing. My hot take is that most cancers will see a study provide 2x mPFS benefit in the next 5 years, maybe 2x OS benefit in the next 10. There are a couple of reasons for this:

1. China has entered the game. Their growth in R&D capabilities, expertise in chemistry, and vast clinical trial infrastructure dwarfs what the U.S. has. Furthermore, the culture is undeterred by competition and relatively small market sizes, which is increasingly the unmet capital need in oncology.
2. New modalities have unlocked improved therapeutic windows. Remember when Abraxane became a blockbuster simply by improving the therapeutic window of paclitaxel? Liposomal doxorubicin? Now we have much more sophisticated ways of improving the TI including ADCs and RIPTACs.

These new modalities and faster execution speed will enable us to better utilize our existing arsenal of poisons (aka chemotherapy, pan-essential targeted drugs, broadly cytotoxic agents, etc.). This is a [good review](https://pmc.ncbi.nlm.nih.gov/articles/PMC8157671/) describing how large of an arsenal we really have and how poorly we have utilized it to date. 

Right ***now*** is a particularly good time to revisit and study our toolbox of 'chemotherapies', for the following reasons:
1. Payload resistance seems to be the major mechanism of resistance to Enhertu and other 'top' ADCs. In general, independently efficacious mechanisms of action are [expected](https://www.nature.com/articles/s43018-023-00667-z) to increase therapeutic efficacy. Dual payload, coformulated, or sequentially administered ADCs with orthogonal payloads are expected to improve survival
2. Irrespective of what you think of the '[magic bullet](https://www.cell.com/cancer-cell/fulltext/S1535-6108(22)00445-7)' ADC hypothesis (are stable linkers important?), ADC formats increase the therapeutic window for highly toxic chemotherapy payloads, making many of the existing poisons we have that were previously disqualified, a potentially new part of the toolbox.
3. Antigen discovery efforts have yielded a nearly complete 'map' of targetable tumor antigens. TME activated platforms (e.g. CytoMx) make even EPCAM a viable target. Every tumor will have a dysregulated surfaceome, meaning that the TAM will not be limited by biology.
4. In contrast, most targeted therapies based on molecular pathways have been discovered already and these are only actionable in a fraction (albeit a growing one) of patients. Hotspot mutations are already a high signal source of targets and CRISPR screens have not identified many more interesting targets.
5. Thus, the proportion of patients with actionable genetic mutations is likely always going to be smaller than the population without them. In other words, the TAM for chemo is always going to be larger for the TAM of targeted therapy.
6. Most chemotherapies were discovered in a more 'primitive' era, prior to RNAseq, high-plex proteomics, CRISPR screens, and other discovery tools. Improvements in chemistry and screening should in theory translate to improved 'next generation' payloads that utilize new technology (e.g. PROTACs)
7. New modalities (e.g. [RIPTACs](https://pmc.ncbi.nlm.nih.gov/articles/PMC11371387/)) can utilize learnings from the ADC payload space

### Technical challenges

There are several technical requirements to make a good payload:
1. The selective delivery of an ADC or other modality requires that the payload be relatively high potency. It is far easier for a drug to get across a cell membrane via diffusion vs antibody internalization. Thus, any payload will need to kill a cell more efficiently on a per molecule basis. Generally the rule I've seen is that the free drug cellular potency needs to be <1 nM. As a result, most focus on next gen ADC payloads have been on DNA damaging agents, and catalytic molecules like PROTACs, which are both highly potent. However, I see no reason why this couldn't be addressed by just dosing higher though and potentially using a 1st generation unstable linker. If the potency is >1 nM, the tox profile will also be better, so no worries if the payload falls off in the TME rather than intracellularly.
2. You want the linker to be hydrophilic to improve pharmacokinetics, stability, and cytotoxin exposure. A challenge for ADCs is that while naked antibodies are soluble and hydrophilic, the payloads that are attached are often hydrophobic, making the ADC overall less soluble and more sticky/prone to aggregation. This is because small molecules need to cross fat containing cell membranes. 
3. An ideal payload also needs accessible functional groups. Most ADC payloads have a self immolative linker which enables traceless cleavage of the payload, but this still requires a site to install the linker. Maleimide-thiol based linkers were initially used with thiol containing payloads like DM1 and DM4, but now [recent work](https://www.nature.com/articles/s41467-026-68605-y#Abs1) (Tubulis) has expanded the possible space of conjugation handles to aliphatic and aromatic alcohols. Solvent exposed conjugation handles that do not compromise efficacy are even more important for non-cleaving molecules like RIPTACs. It is not always straightforward to engineer a molecule simply using off the shelf parts.
4. A major mechanism of resistance not only for ADCs but also other chemotherapies is upregulation of drug efflux pumps like ABCB1 (P-gp). An important design consideration for next generation payloads, especially those used in later line settings is whether the payload is a P-gp substrate. Ideally, the payload is unaffected by drug efflux pumps.

Using DepMap screening data (hundreds of cancer cell lines screened with hundreds of drugs), I plotted the most potent 40 compounds both overall, and in a 'difficult to treat' tumor. Camptothecin (TOPOi) is pretty high up, but there are certainly other mechanisms that could be explored and also offer high potency. Proteasome inhibitors, HDAC inhibitors, anthracyclines, and more. When you use an LLM to search these against just the potency and P-gp substrate filter, very few actually come out. This highlights the need for further medicinal chemistry optimization, but also shows that there is a lot of green space!

![[poisons.jpg]]
### Novel payloads

It is now somewhat well understood that TOPO1 inhibitors are the 'best' payloads. Enhertu, a HER2 targeted, DXd payload ADC showed clear superiority over a microtubule inhibitor payload ADC in Kadcyla. If a microtubule inhibitor payload has worked in an indication, you better believe that there is a next generation TOPO1 in the pipeline. Now, basically every new ADC target antigen is developed first with a TOPO1 payload, and the majority of new studies are with some sort of exatecan derivative. 

The entire list of FDA approved ADC payloads consists of a relatively small list:
1. Topoisomerase 1 inhibitors
	1. Exatecan derivatives (DXd)
	2. Other camptothecin derivatives (SN-38)
2. Microtubule inhibitor
	1. Auristatins (MMAE/MMAF)
	2. Maytansinoids (DM1/DM4)
3. DNA damaging agents
	1. PDB
	2. Ozogamicin

To the industry's credit, there are many innovations in the payload space advancing through Ph1 clinical trials. These include:

- BRD4 inhibitors/degraders: Roche / C4 Therapeutics signed a partnering deal. Unconfirmed, but its possible C4 is working on BRD4 degraders for them
- [Zymeworks](https://www.zymeworks.com/):
	- Hemiasterlins (new class of microtubule inhibitors)
	- [Translation inhibitors](https://aacrjournals.org/cancerres/article/86/7_Supplement/2400/778448/Abstract-2400-Design-and-evaluation-of-mRNA?searchresult=1) (eIF4A)
- [Adlai Nortye](https://www.adlainortye.com/): [KRAS inhibitors](https://www.adlainortye.com/upload/2025/10/27/176153251345035q9de.pdf )
- [Akari Therapeutics](https://akaritx.com/): RNA splicing inhibitor. Increases neoantigen purden
- [Prelude Therapeutics](https://preludetx.com/): SMARCA2/4 and CDK9 degrader payloads
- [Bolt Biotherapeutics](https://www.boltbio.com/): ISAC platform (TLR7/8 agonist). Only worked in CDX, not PDX
- [Myricx](https://myricxbio.com/): NMT inhibitors
- [Iksuda](https://www.iksuda.com/) - ProAlk duocarmycin analog
- [Heidelberg Pharma](https://heidelberg-pharma.com/de/): Amanitin / RNA Pol II inhibitors
- [Hutchmed](https://www.hutch-med.com/) PI3K/PIKK inhibitor
- [Accutar Biotechnology](https://www.accutarbio.com/workflow/) unveiled preclinical data for a degrader-based antibody conjugate that uses its proprietary PI3Kα degrader, AC4847
- Abbvie: [pan PI3K/mTOR](https://aacrjournals.org/cancerres/article/86/7_Supplement/338/775827/Abstract-338-Discovery-of-novel-pan-PI3K-and-mTOR?searchresult=1)
- Sting agonists: 
	- Daiichi Sankyo DS3610
	- Mersana XMT-2056
- Others:
	- Translation inhibitor: psymberin
	- HSP90 inhibitor: geldanamycin derivatives
	- Proteasome inhibitors: Carmaphycin B analogues

There is a broad spectrum of 'targeted therapy', directed at pan-essential genes. These include AURKA/B, CHK1/2, HDAC, CDKs, WEE1, XPO1, etc. Could these all be repurposed as payloads?I'm interested in mitomycin C as well.

### Dual payload

In addition to novel payloads which may be useful in TOPO1 resistant disease, many groups are developing dual payload ADCs which in a single ADC allow conjugation of multiple payload classes. The reasoning here is that having both payloads be delivered at the same time makes it more unlikely that the cancer cell can evade both drugs simultaneously.

A list of dual-payload abstracts/companies from an initial AACR2026 abstract screen I did is below. Most groups used a TOPO1i / microtubule inhibitor combination, which simply combines the two most clinically validated payloads into a single molecule. MMAE and MMAF are commonly used as both are in the microtubule class but MMAE is more membrane permeable (better bystander effect) and MMAF is less permeable which leads to higher killing in the target cell. There are also several TOPO1i/DNA damage repair inhibitors, which make sense because the TOPO1i induces DNA damage and the DDR inhibitor prevents repair (e.g. PARP/PARG). Just a couple days ago, Lilly acquired CrossBridge Bio, which has a dual payload conjugation platform. Their lead is a TOPOi + ATR inhibitor system, which is of this mechanism.

In the clinic already, there is KH815, which is a TROP2 directed TOPO1i / RNA Pol II inhibitor dual payload ADC. There is also IBI3020, which is a CEACAM5 directed TOPO/MMAE dual payload ADC.

### Evaluation of ADCs

Finally, I wanted to include some notes on evaluation of ADC preclinical datasets. Companies will often use the same CDX models and compare head to head vs approved ADCs to make the argument that their ADC is better optimized. Largely, these produce a lot of false positives because of the deficiencies of CDX models (uniform antigen expression, no tumor heterogeneity, rapid proliferation rate). PDX models can be [much more representative](https://www.science.org/doi/10.1126/sciadv.adk1894). 

I think a good checklist is:
1. Efficacy in multiple PDX models at relevant dose levels but at single doses
2. Efficacy in cell line pools with high, low, and no antigen expression. 
3. Evidence of rapid internalization and bystander activity
4. Good payload properties
5. High NHP tolerable doses

As ADC design gets more complex (dual payload, bispecific, dual modality, non traditional Ig formats, etc), other evaluation frameworks can be useful (e.g. [frameworks ](https://aacrjournals.org/cancerres/article/86/7_Supplement/2397/778426/Abstract-2397-Cell-based-payload-release?searchresult=1)for quantifying payload release ratios for dual payload systems, [screening platforms](https://aacrjournals.org/cancerres/article/86/7_Supplement/2964/777486/Abstract-2964-Identification-of-synergistic-dual?searchresult=1) for dual payload synergy). However, the basics to answer "will this work in human" should be relatively consistent with a high bar. Preclinical in vivo ADC studies are simply not that expensive or difficult to execute.

### Dual Payload Companies

Kanghong Pharmaceutical Group:
- [HER3 dual payload](https://aacrjournals.org/cancerres/article/85/8_Supplement_1/1587/756560/Abstract-1587-A-novel-dual-payload-HER3-directed)
- [TROP2 dual payload](https://aacrjournals.org/cancerres/article/85/8_Supplement_1/1585/755015/Abstract-1585-KH815-a-novel-dual-payload-TROP2) This one is in human

ICE Bioscience:
- [Dual payload TOPO/DDR](https://aacrjournals.org/cancerres/article/86/7_Supplement/5632/779797/Abstract-5632-Enhancing-dual-payload-ADC-discovery?searchresult=1)

WuXi:
- [Optimized TOPO payload for dual-payload](https://aacrjournals.org/cancerres/article/86/7_Supplement/4430/779639/Abstract-4430-WuXiTecan2-A-hydrophilic-exatecan?searchresult=1)

Sutro:
- [HER2 dual payload MMAE/TOPOi](https://aacrjournals.org/cancerres/article/86/7_Supplement/1685/781550/Abstract-1685-The-HER2-targeting-dual-payload?searchresult=1)
- [TROP2 dual payload TOPO/STING agonist](https://aacrjournals.org/cancerres/article/86/7_Supplement/1289/776867/Abstract-1289-ASP2998-a-TROP2-targeted?searchresult=1)
- [PTK7 dual payload TOPO/tubulin](https://aacrjournals.org/cancerres/article/86/7_Supplement/1695/780877/Abstract-1695-Preclinical-characterization-of-STRO?searchresult=1)

Affinity Biopharmaceutical:
- [RASi/TOPOi dual payload](https://aacrjournals.org/cancerres/article/86/7_Supplement/4426/779325/Abstract-4426-Novel-tumor-microenvironment-TME?searchresult=1)
- [TME-activated dual payload (Legumain)](https://aacrjournals.org/cancerres/article/86/7_Supplement/4426/779325/Abstract-4426-Novel-tumor-microenvironment-TME?searchresult=1)

CatenaBio:
- [TROP2 dual payload](https://aacrjournals.org/clincancerres/article/32/4_Supplement/PS4-06-12/773800/Abstract-PS4-06-12-Dual-payload-TROP2-targeted)

OBI Pharma:
- [MET/HER3 MMAE/TOPOi dual payload](https://aacrjournals.org/cancerres/article/86/7_Supplement/2665/779347/Abstract-2665-The-MET-HER3-antibody-drug-conjugate?searchresult=1)

CanWell Pharma:
- [CLDN18.2/PD-L1 dual payload](https://aacrjournals.org/cancerres/article/86/7_Supplement/7161/782339/Abstract-7161-A-novel-StarLinkerTM-based-CLDN18-2?searchresult=1)

DualityBio:
- [TA-MUC1 TOPO/ecteinascidin derivative dual payload](https://aacrjournals.org/cancerres/article/86/7_Supplement/2657/779409/Abstract-2657-DB-1326-a-novel-dual-payload-TA-MUC1?searchresult=1)

Phrontline Biopharma:
- [Biparatopic HER2 TOPO/microtubule](https://aacrjournals.org/cancerres/article/86/7_Supplement/3298/777998/Abstract-3298-Preclinical-development-of-TJ106-a?searchresult=1)

Hangzhou DAC:
- [cMET dual payload](https://aacrjournals.org/cancerres/article/86/7_Supplement/2393/778094/Abstract-2393-DXC016-a-novel-cMET-targeting-dual?searchresult=1)
- [FRa dual payload](https://aacrjournals.org/cancerres/article/86/7_Supplement/2395/778092/Abstract-2395-DXC011-a-novel-dual-payload-antibody?searchresult=1)
- [CDH17/GUCY2C bispecific TOPO/antimetabolite dual payload](https://aacrjournals.org/cancerres/article/86/7_Supplement/2396/778427/Abstract-2396-A-novel-2-2-IgG-like-bispecific?searchresult=1)

Sanyou Biopharma:
- [Coformulation ADC gemcitabine + exatecan FRa](https://aacrjournals.org/cancerres/article/86/7_Supplement/1764/781376/Abstract-1764-MC003-A-novel-bi-epitope-dual?searchresult=1)

MediLink:
- [HER2 dual payload TOPO/microtubule](https://aacrjournals.org/cancerres/article/86/7_Supplement/1765/781375/Abstract-1765-YL413-A-novel-dual-payload-anti-HER2?searchresult=1)

Hongcheng Biopharma:
- [PSMA/STEAP1 bispecific dual payload tubulin/TOPO](https://aacrjournals.org/cancerres/article/86/7_Supplement/6943/781436/Abstract-6943-Bispecific-antibody-with-dual?searchresult=1)

QiLu Pharmaceutical:
- [EGFR/B7H3 bispecific dual payload](https://aacrjournals.org/cancerres/article/86/7_Supplement/5650/776790/Abstract-5650-Preclinical-development-of-LUA006-A?searchresult=1)

Baylink Biosciences:
- [GPC3 dual payload](https://aacrjournals.org/cancerres/article/86/7_Supplement/1664/780925/Abstract-1664-Novel-GPC3-targeting-antibody-drug?searchresult=1)

Callio Therapeutics:
- [HER2 TOPO ATRi dual payload](https://aacrjournals.org/cancerres/article/86/7_Supplement/4427/779324/Abstract-4427-Development-of-CLIO-8221-A-HER2?searchresult=1)

Hangzhou Adcoris:
- [cMET/EGFR bispecific dual payload](https://aacrjournals.org/cancerres/article/86/7_Supplement/1775/781095/Abstract-1775-ACR335-a-novel-cMET-EGFR-bispecific?searchresult=1)

Zhejiang Doer:
- [Nectin4/TROP2 TOPO/microtubule](https://aacrjournals.org/cancerres/article/86/7_Supplement/4541/779683/Abstract-4541-DR319-DP-A-Nectin-4-Trop-2?searchresult=1)

FDC Biotech:
- [ADAM9 dual payload TOPO/microtubule](https://aacrjournals.org/cancerres/article/86/7_Supplement/3172/780410/Abstract-3172-XYD-8006-A-novel-ADAM9-targeting?searchresult=1)