---
title: "How to develop new medicines"
date: "2025-04-10T12:00:00.000Z"
template: "post"
draft: True
slug: "/blog/newmedicines/"
category: "Life Sciences"
tags:
  - "Life sciences"
  - "Healthcare"
description: "heuristics for indication selection in I&I"
---

The goal for today is to develop and apply a pipeline for understanding the landscape of drug targets for a given indication. 

My summaries are heuristics meant to be taken 'as is' -- definitively incomplete, and often probably wrong due to my own lack of understanding.

### Genetic association: 

Link to Atlas article (Aimee Raleigh)

Genetic priority score (Duffy et al. 2024): https://www.nature.com/articles/s41588-023-01609-2
ML-Genetic priority score (Chen et al. 2024): https://rstudio-connect.hpc.mssm.edu/mlgps/

Plasma proteome association: https://www.cell.com/cell/fulltext/S0092-8674(24)01268-6

LLM assisted search (for rare disease, drug repurposing): https://www.nature.com/articles/s41591-024-03233-x

Functional genomic profiling: [Cancer Dependency Map](https://depmap.org/portal/)

### Clinical trials

NEJM
UpToDate
Clinicaltrials.gov

Pharma projects

Off label use of drugs (e.g. Dupixent). 

### Company filings
They are required to describe competitive landscape


## Table of Contents

- [What are unmet needs?](#what-are-unmet-needs)
  - [Cancer (link to previous article)](#cancer-link-to-previous-article)

- [Dermatology](#dermatology)
  - [Atopic Dermatitis](#atopic-dermatitis)
  - [Vitiligo](#vitiligo)
  - [Chronic Rhinosinusitis with Nasal Polyps](#chronic-rhinosinusitis-with-nasal-polyps)
  - [Hidradenitis Suppurativa](#hidradenitis-suppurativa)
  - [Prurigo Nodularis](#prurigo-nodularis)

- [Ophthalmic Diseases](#ophthalmic-diseases)
  - [Thyroid Eye Disease](#thyroid-eye-disease)
  - [Geographic Atrophy](#geographic-atrophy)
  - [Uveitis](#uveitis)

- [Gastrointestinal](#gastrointestinal)
  - [Celiac Disease](#celiac-disease)
  - [Crohn's Disease](#crohns-disease)
  - [Inflammatory Bowel Disease](#inflammatory-bowel-disease)

- [Systemic Autoimmune and Inflammatory Disease](#systemic-autoimmune-and-inflammatory-disease)
  - [Rheumatoid Arthritis](#rheumatoid-arthritis)
  - [Chronic Spontaneous Urticaria](#chronic-spontaneous-urticaria)
  - [Myasthenia Gravis](#myasthenia-gravis)
  - [Systemic Lupus Erythematosus (SLE)](#systemic-lupus-erythematosus-sle)
  - [Osteoporosis](#osteoporosis)
  - [Food Allergy](#food-allergy)
  - [IgG4 Related Disease](#igg4-related-disease)
  - [Primary Sjögren's Syndrome](#primary-sjogrens-syndrome)

- [Kidney Disease](#kidney-disease)
  - [Membranous Nephropathy](#membranous-nephropathy)
  - [IgA Nephropathy](#iga-nephropathy)
  - [Chronic Kidney Disease](#chronic-kidney-disease)
  - [Lupus Nephritis](#lupus-nephritis)

- [Pulmonology](#pulmonology)
  - [Idiopathic Pulmonary Fibrosis (IPF)](#idiopathic-pulmonary-fibrosis-ipf)
  - [Chronic Obstructive Pulmonary Disease (COPD)](#chronic-obstructive-pulmonary-disease-copd)
  - [Severe Asthma](#severe-asthma)

- [Hematology](#hematology)
  - [Thrombotic Thrombocytopenic Purpura (TTP)](#thrombotic-thrombocytopenic-purpura-ttp)


## What are unmet needs?

If looking for the TLDR, I think there are unmet needs (unaddressed by currently publicly disclosed drugs) in:

1. Vitiligo
2. COPD
3. Hidradenitis Suppurativa
4. Celiac Disease
5. Alopecia Areata


Cancer (link to previous article)

## Dermatology

### Atopic Dermatitis (AD)

Giant market, 16.5 million US adults (7.3%) have AD, ~40% have moderate or severe symptoms. ~9.6 million US children under the age of 18 have AD. Biologic addressable population is estimated at ~10 million annually.

Dupixent launched in 2017, and AD has relatively lower biologic penetration (~10% vs 25% in psoriasis), so definitely room to grow.

Dupixent is already very good, with only 9% of moderate cases and 16% of severe cases that are refractory to the drug. As a result, it can be hard to run trials due to high placebo response (see \$ANAB).

Apogee is developing long half life versions of IL-13 and OX-40L antibodies to eventually compete with Dupi. You can compete on infrequent dosing, faster onset, and deeper remission, and Apogee is in theory competing on all three.

The other approved drugs are from Galderma (Nemolizumab; IL-31), Sanofi/Regeneron (Dupixent; IL-4Ra), Lilly (Lebrikizumab; IL-13).

### Vitiligo

Topical JAK and calcineurin inhibitors do a pretty good job, albeit with toxicity. Another underpenetrated market where patients don't seek treatment due to lack of effective options. 

Vitiligo is a good indication for drug development because you can rapidly see skin improvements and the risk for placebo response isn't as high. 

One new mechanism is the IL-15 / CD122 axis, being developed by Teva/Forte. $VYNE has another approch Repibresib which is a BET inhibitor in Ph2 trials.

### Hidradenitis Suppurativa (HS)

Pathophysiology is complex. There is evidence that it is Th17 driven, and IL-17 antibodies do have some efficacy. However TNFa antibodies also have activity and the Abbvie lutikizumab data is validating of the IL1-a/b pathway. Novartis is also developing Ianalumab, a BAFF receptor antibody in Ph2.

There doesn't seem to be a north star yet for biology, but many are excited about the IRAK4 degrader approach pioneered by Kymera. IRAK4 inhibition didn't work but the differentiation is that IRAK4 also has various scaffolding functions that contribute to inflammation.

I am also excited about IL1RAP blocking antibodies, which block all IL-1, IL-33, and IL-36 signaling. In theory IRAK4 provides broader coverage than IL1RAP, but you could engineer a long half life IL1RAP for less frequent dosing and potentially differentiated side effect/efficacy profile.

Ultimately, HS is a crowded marketplace for a small-medium sized opportunity, that is waiting for a big clinical win.

### Prurigo Nodularis (PN)

Often co-morbid with atopic dermatitis. Th2 biology is significant, and there is aberrant expression of IL-31. Nemolizumab, IL-31 and Dupixent, IL-13 are approved.

Itch relief is a major patient need, which Nemolizumab hits the hardest and fastest. Dupixent gets there more slowly by resolving Th2 inflammation. Both drugs don't saturate on efficacy, with only 30% of patients achieving complete response.

Market is smaller, just \$2 billion annually, but underpenetrated by biologics. There are ~75k biologic eligible pts, 181k overall. Drug development has typically started in AD, then spilled into PN. Some interesting assets are IL-31 / IL-13 bispecifics, of which it looks like Zai lab with their long half life bispecific in Ph1, is in the lead.

### Psoriasis (PsO)

In my mind psoriasis is essentially cured. Mild cases are well managed with topical creams/ointments like cortocosteroids. Moderate to severe cases are addressed with IL-17 or IL-23 targeting antibodies. Oruka Therapeutics from the Paragon family has the blueprint for competing commercially in moderate/servere pateints. 

Simply combine IL-17/23, and shoot for higher + longer exposure with half life extension.

### Alopecia Areata



## Gastrointestinal

### Eosinophilic Esophagitis (EoE)

Frontline therapy is corticosteroids and PPIs

Underdiagnosed, Dupixent in 2022 is the only approved biologic. TAM is 3-7 billion. Relapse rate off treatment is high (60-70%)

Dupixent needs to be dosed Q1W in EoE

Histologic and dysphagia (trouble swallowing) endpoints have been hard to hit on simultaneously.

### Celiac Disease

Highly prevalent disease that has essentially been abandoned by large pharma (with exception of Teva/Takeda). There are a very complicated set of patient presentations ranging from those who can seemingly tolerate gluten with no symptoms but histological damage, to patients that have it so bad that they can even develop celiac associated T cell leukemia.

Teva, Calypso/Novartis, Forte, and other groups have recently reported data from IL-15 / CD122 targeting antibodies. Collectively, the data indicate that blocking this pathway can reverse disease associated pathology on histology in biopsy specimens.

CD122 in my opinion makes more sense than just targeting IL-15 for a couple reasons. First, its the receptor, meaning that you can get greater efficacy with less dose (receptor internalization, easiier to saturate in terms of molarity, less need to worry about resynthesis). Second, IL-2 signaling which is also blocked by targeting CD122 is most correlated with patient symptoms.

### Inflammatory Bowel Disease

The blueprint to addressing this one is laid out by Charlie Lees on his [Substack](https://substack.com/@charlielees). Essentially, you will cycle through a TNFa first, then through various other biologics like Vedolizumab (against α4β7 integrin), Skyrizi (a IL-23A blocker), and now likely some TL1A blocker (and Obefazimod maybe??). Patients never get cured, so will be managed chronically the rest of their lives. While somewhat depressing, this is great for biopharms, as you don't necessarily need to show superiority. You just need to be an orthogonal mechanism that demonstrates efficacy in a biologic experienced population.

Great market and certainly open for business.

Combinations, co-formulations, and competition on half life will dominate care until most drugs go genertic in 2032.

### Crohn's Disease

Chron's disease is sort of the same story as IBD. You have the same efficacious mechanisms (TNFa, IL-23, a4b7, TL1A). The differentiator is that it can affect any part of the digestive tract and can have many complications. 

Business wise, this doesn't mean too much. Similar to IBD, the name of the game is increasing drug exposure, layering on multiple mechanisms simultaneously, and increasing convenience. Charlie Lees [again](https://charlielees.substack.com/p/after-tnf-failure-in-crohns-disease).


## Opthalmic Diseases

### Thyroid Eye Disease

IGF1R

IL-11

### Geographic Atrophy 



### Uveitis


## Systemic Autoimmune and Inflammatory Disease

### Rheumatoid Arthritis




4th line RA

IL-6, TNF-a

Some interesting new mechanisms including PD-1 agonism (\$ANAB)

### Psoriatic Arthritis (PsA)



### Axial Spondyloarthritis (AxSpA)



### Ankylosing spondylitis (AS)

A Nature Medicine paper came out in 2023 describing a [prototype therapy](https://www.nature.com/articles/s41591-023-02613-z) for patients with AS. It turns out that patients with this disease commonly have expansion of a specific T cell TCRb CDR3 motif, particularly containing TRBV9 that recognizes an autoantigen in the spine and large joints. You can raise an antibody against TRBV9 and treat patients with it, thus clearing out the autoinflammatory CD8 T cells and resolving symptoms. 

This approach is now being pioneered by [Hillstar Bio](https://endpts.com/hillstar-bio-raises-67m-for-immunology-drugs/) which just raised money in March 2025. 

### Pemphigus / Bullous Pemphigoid (BP)

FcRn fail from Argenyx

### Chronic Inflammatory Demyelinating Polyneuropathy (CIDP)

### Cold Agglutinin Disease 

When it is cold, you get aggregation of certain cold sensitive antibodies (often IgM) that crosslink red blood cells and leads to autoimmune hemolytic anemia via activation of the classic complement pathway. It is rare, but this is a chronic disease so there is certainly a market.

Sutimlimab, a C1s antibody that is given at a massive 6.5 or 7.5 __gram__ dose every two weeks I.V., is effective. This drug was sold by Sanofi for \$825 million to Recordati, an Italian pharmaceutical developer.

However, I don't think anyone is happy with this dosing schedule and we can certainly do better here. Dianthus Therapeutics (\$DNTH) is trading at a \$524 mn market cap for a 60 day half-life C1s antibody

### IgM mediated disorders

There are a set of collectively rare disorders where abundant IgM protein causes neuropathy, 

Commonly a symptom of MGUS

### Chronic Spontaneuous Urticaria (CSU)

Chronic random itchiness. 

>500k people in the US live with chronic urticaria.
The overall prevalence is estimated at 230 cases per 100,000 adults.
Affects up to 20% of people worldwide.

Antihistamines, at recommended doses, relieve symptoms in less than 50% of patients, with up to 25-33% remaining symptomatic even after 4x dose escalation.

Mast cell activation, IgE and IgG autoantibodies, Type 2 inflammation

KIT: Jasper (Briquilimab) and CellDex (Barzolvolimab)

IgE

### Myasthenia Gravis (MG)

FcRn

### Graves Disease 

330k pts who have failed all therapuetic options other than surgical removal of thyroid

Addressable with FcRn or IgG degraders (enzymes or TPD)

### Myositis

tens of thousands of pts

Addressable with FcRn

### Systemic Lupus Erethymatosus (SLE)

Anifrolumab (IFNAR1 antibody)

### Osteoporosis

RANKL antibodies

### Food Allergy

Food allergy is undoubtedly a large indication and has significant potential to impact quality of life. The [success](https://www.nejm.org/doi/full/10.1056/NEJMoa2312382) of Omalizumab in food allergy has reawakened drug development. The dosing regimens for Omalizumab are not ideal, as some larger patients require up to 4 pre-filled syringe injections to see the requisite IgE inhibition. Thus, there is an opportunity for a long half life version of Omalizumab with improved IgE clearing and inhibition of resynthesis.

However, there will be little pricing power as omalizumab will be generic in 2 years and there are 4 other public IgE approaches including RAPT, Merida Biosciences, Lycia Therapeutics, Seismic Therapeutics.

Oral immunotherapy as antigen sensitization is the alternate approach, and this works but is very arduous. Roche/Genentech likely has interest in lifecycle management for Omalizumab and may be able to develop or in license a long half life version. I personally am not interested in this market.

### IgG4 Related Disease (IgG4-RD)

Amgen's CD19 antibody Uplizna has made major progress in treating IgG4-RD. Short of any other safe strategy of depleting B cells, I think the market here is saturated, at least until there are reliable reports of patients relapsing off of Uplizna.

### Primary Sjrogen's Syndrome (SS)

IFNAR1 antibodies


### Systemic Sclerosis (SSc)

This disease 

TL1A


## Kidney Disease

### Membranous Nephropathy

### IgA Nephropathy



### Lupus Nephritis

Cyclosporine ($AUPH), Rituximab


## Pulmonology

### Idiopathic Pulmonary Fibrosis (IPF): 
Progressive fibrosis with poor prognosis.

### Chronic Obstructive Pulmonary Disease (COPD): 
Limited disease-modifying treatments.

Upstream Bio TSLPR antibody

### Severe Asthma: 
Biologic treatments don’t address all patient phenotypes.

T2 high phenotype which seems driven by Th2 inflammation, has high biomarkers (e.g. eosinophils, FeNO), and is targetable by Dupixent, Tezspire, and Nucala.

The non-Th2

TSLP

Dupixent 

IL-5, IgE (Omalizumab)


### Chronic Rhinosinusitis with Nasal Polylps (CRSwNP)

CRSwNP is very often co-morbid with asthma and the biology is very similar in that both are driven by Th2 inflammation. 

Omalizumab, Depokimab, and Dupi are approved. Tezspire should be approved later this year (Q4W), Lebrikizumab (Q2-8W) is in a Ph3, and verekitug, Upstream’s TSLPR (Q12W) should have Ph2 data later this year.

This is a disease which in my mind is basically cured by Dupixent. The outcomes are very good according to [this](https://onlinelibrary.wiley.com/doi/10.1111/all.15796) article. There are maybe 10-20% of patients who don’t have an adequate response, and the investigators linked showed you can taper Dupi doses over the course of 2 years, in some cases out to Q12W. Dupi efficacy saturates around 24 weeks and you could make the argument for deeper responses, but I think the rationale to push for better efficacy is definitely higher in other indications.

Additionally, the prevalence is ~6-7x lower than ohter Th2 respiratory indications such as asthma/COPD. Dupi reached $1B in sales and there are still ~900k pts in U.S./Europe, but definitely smaller. In a sample size of ~75k pts from 2018-2023, biologic penetration is at ~12%, with the vast share (90%) going to Dupi. However, ~50% discontinue and only 2.6% switch therapy which to me says that they get better and then stop drug.

## Hematology

### Thrombotic Thrombocytopenic Purpura (TTP): 
Targeted therapies are needed for refractory cases.




