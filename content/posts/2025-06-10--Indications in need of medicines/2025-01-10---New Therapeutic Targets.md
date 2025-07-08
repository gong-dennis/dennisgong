---
title: "Developing new medicines (Part I)"
date: "2025-06-30T12:00:00.000Z"
template: "post"
draft: False
slug: "/blog/newmedicines/"
category: "Life Sciences"
tags:
  - "Life sciences"
  - "Healthcare"
description: "heuristics for indication selection in I&I"
---

The goal for today is to develop and apply a pipeline for understanding the landscape of drug targets for any given indication. This is going to be a two part series. In this article, I will tell you where the unmet needs are, and in the next, hopefully posted next month, I'll tell you what kinds of drugs can be developed right now to make a difference.

Two questions that I always want to know the answers to when getting up to speed are: 

1. What are the major recent and upcoming therapeutic developments? 
2. What are the most biological hypotheses waiting for answers from pivotal clinical trials? 

In other words, what are the targets and what are the results of modulating them? I'll answer each of these questions in a short summary of key ideas to think about when evaluating each of the 60 indications covered in this post.

![Defining the therapeutic frontier](beijing.jpg "Defining the therapeutic frontier")

***

Indications exist on a spectrum of maturity. Here, I'll classify them as 'mature', 'maturing', and 'nascent', but of course they are a continuous spectrum. 

For 'mature' indications, there may already be a list of 3-5 targets that have been proven out in clinical trials. For this category of indication, major clinical trials could be combinations of existing drugs, or trials of novel mechanisms of action (MOA) in refractory patients. As an example, some people are interested in novel MOAs for 4th line rheumatoid arthritis. These indications, stereotypically, are highly prevalent and chronic diseases where patients cycle through multiple therapies over the course of their treatment history. For an indication that already has 3-4 classes approved, you need to think about what the incremental advance of another new medicine is, versus all of the potential combinations of new therapy +/- each of the previously approved drugs.

Then, there are indications where there are no approved targeted therapies, but proof of concept clinical trials have identified a mechanism. This is APRIL inhibition in IgAN, or KRAS inhibition in PDAC. The appeal of building in a 'maturing' indication needs to be seriously considered, as the attractiveness can quickly turn sour. When something new gets approved, it is worth seriously thinking about whether the indication is still an unmet need. Immediately, large studies of combinations funded by big pharma will initiate and a swath of competing me-better molecules will spawn and improve on whatever therapeutic signal was demonstrated.

Finally, 'nascent' indications are often those where chatter on patient forums is still louder than Wall Street. Fibromyalgia, celiac disease, autoimmune hepatitis. These indications can be highly prevalent, but due to lack of research, difficulty of diagnosis, or simply the complexity of the disease, very little therapeutic inroads have been made. These are indications without a north star; drug development on hard mode.

*** 

For many indications, there will be a 'winner' mechanism. For example, in atopic dermatitis, it is IL-13. In psoriasis, it was neutralization of IL-17. Subsequent therapeutic development will be in refractory patients, or in creative ways of enhancing the primary response, either by increasing potency or combinations. 

Broadly speaking, companies have built value by being best in class in 'mature' indications and being first in class in 'nascent' indications, but the blockbuster outcomes have come from being both first and best in class in 'maturing' indications. Revolution Medicines, Acceleron Pharma, Blueprint Medicines.

How do we identify targets? Here is a sampling of resources to cover the first 50% of work: 

## Genetic association: 

Enough has been written about the value of human genetics evidence for evaluating a target. This Atlas "From the trenches" [article](https://lifescivc.com/2024/04/deconstructing-the-diligence-process-an-approach-to-vetting-new-product-theses/) from Aimee Raleigh and Robert Plenge's [blog](https://www.plengegen.com/) are great starting points.

The [GWAS catalog](https://www.ebi.ac.uk/gwas/home) keeps track of top hits for all diseases, and recently several groups [1](https://www.nature.com/articles/s41588-023-01609-2), [2](https://rstudio-connect.hpc.mssm.edu/mlgps/) have offered fancy machine learning based polygenic risk scores that help prioritize pathogenic genetic associations. 

Outside of these simplified lists for public consumption, there is some creative alpha that can be mined by a professional geneticist. Marea had the creative insight that [remnant cholesterol](https://www.biopharmadive.com/news/marea-therapeutics-remnant-cholesterol-angptl4-launch/719149/) may be an underappreciated biomarker for cardiovascular disease, identifying ANGPTL4 as a target whose genetic absence is associated with lower remnant cholesterol. 

As serum proteomics offerings continue to expand (e.g. Olink, SomaScan, Nomic, etc.) a rich new frontier of discovery will be the plasma proteome. So far, ~50k samples from the UKBB have been processed and published ([Nature](https://metabolomips.org/ukbbpgwas/), [Cell](https://www.cell.com/cell/fulltext/S0092-8674(24)01268-6), [portal](https://proteome-phenome-atlas.com/)), but increasing sample size to the full 500k UKBB cohort should power many more discoveries. If I were a rheumatologist, I would be publishing so many plasma (or disease associated fluid/tissue) proteomic atlases right now.

In cancer, functional genomic profiling (e.g. the [Cancer Dependency Map](https://depmap.org/portal/)) can be used to brute force your way to drug targets. However, I haven't seen this approach be successful outside oncology, and even within oncology, everyone has this data. This is no longer useful as a primary resource for novelty.

## The public domain

Outside of the academic work one can do to identify targets from first principles, publicly accessible resources provide critical 'color' on how the real world performance of a drug is, or whether there is excitement from researchers about a given mechanism (which may reflect unpublished findings). 

Follow all the patient forums on Reddit/etc. to really understand where the unmet need is. Do people really care about convenience, or are they still unsatisfied with efficacy? Reddit forums also commonly provide early patient experiences from clinical trials. Are patients dropping out? Are patients experiencing miraculous benefit or otherwise generally happy with how an investigational therapy is performing?

Follow conferences and their social media coverage. The ones I have previously followed and found most useful are EULAR, ASCO, ESMO, AACR, ASH. 

Twitter is an evergreen resource for news, opinions, and debate.

LLM assisted [search](https://www.nature.com/articles/s41591-024-03233-x) for rare diseases or drug repurposing has in theory progressed, though practically I have no idea how to use or evaluate these tools. There are all sorts of data leakage issues and obfuscations that probably aren't answerable. It is true in my experience however, that large language models have improved significantly. ChatGPT's o3 model in particular helped tremendously in writing this piece and while it still hallucinates (it came up with irsegedibep as a long half life TSLP antibody), it is able to surface new information that would have taken me longer to find otherwise. Prompting strategy should be focused on how to reach 'high-value' areas of the latent space (e.g. using jargon in prompts to demonstrate expertise).

### Clinical trials

I could wax poetic about NEJM, the Lancet, or whatever else your favorite journal is. Cutting to the chase -- the fact of the matter is that clinical trial literacy is skill #1. What is the trial population, what was the trial protocol, how did patients flow through/drop out of the trial are all just as important as what the topline results were. If you want to really understand how well a drug works, don't make any inferences until you see the supplementary information. Plot the data yourself, count the lines on the spider plot, and never trust a press release.

If a trial isn't published (yet) physician trade publications (e.g. [Dermatology Times](https://www.dermatologytimes.com/)) or the results page on Clinicaltrials.gov may have your data.

For getting up to speed, borrow a doctor friend's UpToDate account (though LLMs are possibly just as good now). Pharma projects, Global Data, or other paid resources can help too if you are part of an organization that subscribes.

Where to find alpha? Off label use of drugs (e.g. Dupixent) has uncovered efficacy across a much broader set of both atopic and non-atopic diseases that were not marketed as the initial TAM. Smart Pubmed queries can point you to tons of studies conducted by pharma, where you can read discussion sections for how industry scientists (or collaborating physicians) view the future development path. 

### Company filings

Companies are required to describe the competitive landscape in quarterly and annual reports. Investor presentations will also often have 'prettier' versions of competitive landscape graphics.

If your organization gives access to Refinitiv/Bloomberg or any other sell-side news source, those reports can contain some useful information.

### Scientific literature

It really is the wild wild west out there. You can find supporting evidence for whatever you want so don't take anything too seriously. Depending on your level of scientific literacy, reading too much literature can ironically be counterproductive for your diligence process, especially with LLMs now. That being said, I'll offer a few points worth digging into:

1. Predictive validity of model systems. What is the sensitivity and specificity of the model system? What endotype or 'pace' (e.g. acute or chronic) does it resemble?
2. When comparing data from the 'same' model, make sure they really are the same model. Experimental details matter.
3. Target expression. Try to figure out how many molecules per cell there are and what the therapeutic stoichiometry looks like. For ex., will there be TMDD issues? What is the resynthesis/secretion/turnover rate?
4. Try to do some basic PK/PD modeling. What is the receptor occupancy necessary for therapeutic effect? Is there an exposure efficacy relationship? What are the factors making the dosing schedule what it is?

## Table of Contents

On to the content. There are 10 broader indication areas I categorized within I&I, and a total of 60 individual indications. A summary is provided up front and brief concluding thoughts are at the end. 

Why I&I? I know nothing about cardiology or neurology. My PhD is in cancer biology but cancer is uninteresting to me from a therapeutic development perspective. There are so many people working on it and so many clinical trials already. The pace of improvement, aside from like GBM, is rapidly making the outlook for patients better. If truly interested, I wrote an [article](https://www.dennisgong.com/blog/CancerTypes/) more than a year ago covering all the major cancer types and treatment regimens. Much of it is outdated, which speaks to the pace of progress.

My summaries below are heuristics meant to be taken 'as is' -- definitively incomplete, and often probably wrong due to my own lack of understanding. Nevertheless, we persist. If nothing else, you can use me as a contra.

- [Summary of the unmet needs](#what-are-unmet-needs)

- [Dermatology & Skin Autoimmunity](#dermatology--skin-autoimmunity)
  - [Atopic Dermatitis (AD)](#atopic-dermatitis-ad)
  - [Vitiligo](#vitiligo)
  - [Alopecia Areata (AA)](#alopecia-areata-aa)
  - [Hidradenitis Suppurativa (HS)](#hidradenitis-suppurativa-hs)
  - [Prurigo Nodularis (PN)](#prurigo-nodularis-pn)
  - [Psoriasis (PsO)](#psoriasis-pso)
  - [Pemphigus Vulgaris (PV)](#pemphigus-vulgaris-pv)
  - [Bullous Pemphigoid (BP)](#bullous-pemphigoid-bp)

- [Gastroenterology & Hepato-Pancreato-Biliary](#gastroenterology--hepato-pancreato-biliary)
  - [Eosinophilic Esophagitis (EoE)](#eosinophilic-esophagitis-eoe)
  - [Celiac Disease](#celiac-disease)
  - [Inflammatory Bowel Disease (IBD)](#inflammatory-bowel-disease-ibd)
    - [Crohn’s Disease](#crohns-disease)
  - [Primary Sclerosing Cholangitis (PSC)](#primary-sclerosing-cholangitis-psc)
  - [Autoimmune Hepatitis](#autoimmune-hepatitis)
  - [Autoimmune Pancreatitis](#autoimmune-pancreatitis)

- [Ophthalmic Diseases](#ophthalmic-diseases)
  - [Thyroid Eye Disease (TED)](#thyroid-eye-disease-ted)
  - [Geographic Atrophy (GA)](#geographic-atrophy-ga)
  - [Uveitis](#uveitis)

- [Rheumatology & Connective-Tissue Diseases](#rheumatology--connective-tissue-diseases)
  - [Rheumatoid Arthritis (RA)](#rheumatoid-arthritis-ra)
  - [Psoriatic Arthritis (PsA)](#psoriatic-arthritis-psa)
  - [Axial Spondyloarthritis (AxSpA)](#axial-spondyloarthritis-axspa)
    - [Ankylosing Spondylitis (AS)](#ankylosing-spondylitis-as)
  - [Osteoarthritis (OA)](#osteoarthritis-oa)
  - [Polymyalgia Rheumatica (PMR)](#polymyalgia-rheumatica-pmr)
  - [Still’s Disease](#stills-disease)
  - [Systemic Lupus Erythematosus (SLE)](#systemic-lupus-erythematosus-sle)
  - [Systemic Sclerosis (SSc)](#systemic-sclerosis-ssc)
  - [Relapsing Polychondritis](#relapsing-polychondritis)
  - [Vasculitides](#vasculitides)
  - [Myositis](#myositis)
  - [Recurrent Pericarditis](#recurrent-pericarditis)

- [Allergy & Type-2-Driven Disorders](#allergy--type-2-driven-disorders)
  - [Chronic Spontaneous Urticaria (CSU)](#chronic-spontaneous-urticaria-csu)
  - [Severe Asthma](#severe-asthma)
  - [Chronic Rhinosinusitis with Nasal Polyps (CRSwNP)](#chronic-rhinosinusitis-with-nasal-polyps-crswnp)
  - [Food Allergy](#food-allergy)

- [Pulmonology & Interstitial Lung Disease](#pulmonology--interstitial-lung-disease)
  - [Idiopathic Pulmonary Fibrosis (IPF)](#idiopathic-pulmonary-fibrosis-ipf)
  - [Sarcoidosis](#sarcoidosis)
  - [Pulmonary Arterial Hypertension (PAH)](#pulmonary-arterial-hypertension-pah)
  - [Chronic Obstructive Pulmonary Disease (COPD)](#chronic-obstructive-pulmonary-disease-copd)
  - [Anti-synthetase syndrome](#anti-synthetase-syndrome)

- [Nephrology & Glomerular Disease](#nephrology--glomerular-disease)
  - [Minimal Change Disease (MCD)](#minimal-change-disease-mcd)
  - [Membranous Nephropathy (MN)](#membranous-nephropathy-mn)
  - [IgA Nephropathy (IgAN)](#iga-nephropathy-igan)
  - [Lupus Nephritis (LN)](#lupus-nephritis-ln)
  - [Chronic Kidney Disease (CKD)](#chronic-kidney-disease-ckd)

- [Hematology & Immuno-hematology](#hematology--immuno-hematology)
  - [Immune Thrombocytopenic Purpura (ITP)](#immune-thrombocytopenic-purpura-itp)
  - [Thrombotic Thrombocytopenic Purpura (TTP)](#thrombotic-thrombocytopenic-purpura-ttp)
  - [Autoimmune Hemolytic Anemia (AIHA)](#autoimmune-hemolytic-anemia-aiha)
  - [Cold Agglutinin Disease (CAD)](#cold-agglutinin-disease-cad)
  - [Antiphospholipid Syndrome (APS)](#antiphospholipid-syndrome-aps)
  - [IgM-mediated Disorders](#igm-mediated-disorders)
  - [VEXAS Syndrome](#vexas-syndrome)
  - [Hemochromatosis](#hemochromatosis)

- [Neuro-Immunology](#neuro-immunology)
  - [Multiple Sclerosis (MS)](#multiple-sclerosis-ms)
  - [Neuromyelitis Optica (NMOSD)](#neuromyelitis-optica-nmosd)
  - [Myasthenia Gravis (MG)](#myasthenia-gravis-mg)
  - [Chronic Inflammatory Demyelinating Polyneuropathy (CIDP)](#chronic-inflammatory-demyelinating-polyneuropathy-cidp)

- [Endocrine & Exocrine Autoimmune](#endocrine--exocrine-autoimmune)
  - [Graves Disease](#graves-disease)
  - [IgG4-Related Disease (IgG4-RD)](#igg4-related-disease-igg4-rd)
  - [Primary Sjögren’s Syndrome (SS)](#primary-sjogrens-syndrome-ss)

## What are unmet needs?

If looking for the TLDR, I think there are significant unmet needs (unaddressed by currently publicly disclosed drugs) in:

1. Vitiligo & Alopecia Areata (CD122, lest we get rezpegged)
2. Celiac Disease (CD122 / IL-15 class)
3. Primary Sclerosing Cholangitis (idk, CCL24 / TL1A maybe)
4. Geographic atrophy (cell therapy)
5. Bullous Pemphigoid (some Kit combo w/ topical steroids)
6. Osteoarthritis (Nav1.7?)
7. Psoriatic arthritis / Axial Spondyloarthritis / Ankylosing spondylitis (Tyk2 / IL-17A/F combo, maybe make sweeping)
8. IPF (IL-11)
9. Sjogren's Syndrome (IRF5)
10. Polymyalgia Rheumatica (IL-1 inhibition)
11. Sarcoidosis / anti-synthetase syndrome (CCL24 / TL1A)
12. Non-T2 endotype Severe COPD / Asthma (DPP1)

Truthfully, there aren't a lot of unsolved diseases left. A lot of what I've covered below has a mechanism in clinical trials (e.g. B cell depletion/inhibition) which many people expect will work. In parentheses above are some ideas which maybe aren't 'priced in' yet. We'll think harder about new mechanisms and develop a framework for TPPs in our next post. 

On to the indications!

## Dermatology and Skin Autoimmunity

### Atopic Dermatitis (AD)

Giant market, 16.5 million US adults (7.3%) have AD, ~40% have moderate or severe symptoms. ~9.6 million US children under the age of 18 have AD. Biologic addressable population is estimated at ~10 million annually.

Dupixent launched in 2017, and AD has relatively lower biologic penetration (~10% vs 25% in psoriasis), so the bull case for Sanofi/Regeneron and also for me-betters like Apogee is that there is significant room to grow.

Eczema is complicated. On the one hand, Dupixent has a reputation for being this 'miracle' drug. Most patients respond and improve on the drug, so much so that some physicians will say that if you don't, you were misdiagnosed. If you want numbers, approximately 9% of moderate cases and 16% of severe cases are refractory to the drug. Different docs/centers will give you different numbers though, some say 1/2 to 2/3 might respond. Due to the high expectations of therapeutic benefit set by Dupi, it can be hard to run trials due to high placebo response (see \$ANAB). 

On the other hand, patients often get conjunctivitis, and many patients have said that the drug can be hit or miss or can even attribute new flares to starting the drug. Some patients may lose response to the drug and if you have chronic eczema, you can't really be relying on JAKs or steroids to fill the gap.

Apogee is developing long half life versions of IL-13 and OX-40L antibodies to eventually compete with Dupi. You can compete on infrequent dosing, faster onset, and deeper remission, and Apogee is in theory competing on all three. The other approved drugs are from Galderma (Nemolizumab; IL-31), LEO Pharma (Adbry; IL-13), Lilly (Lebrikizumab; IL-13). Nemolizumab is marketed to improve on itch symptoms but differences in trial design make this point at least a little murky. It certainly doesn't compete on EASI endpoints. Adbry targets a non-optimal epitope on IL-13 and has reduced efficacy relative to Lebrikizumab. Both Nemo and Lebri have had strong commercial launches, indicating that AD is still a strong and healthy market, with unmet needs.

### Vitiligo

Vitiligo is another underpenetrated market where patients don't seek treatment due to lack of effective options. On the other hand, morbidity associated with vitiligo is typically only psychosocial in nature. There is no impact on all cause mortality and one study even found that vitiligo patients have longer life expectancy than propensity matched controls.

Still, the addressable U.S. population is 2–3 million (0.8-1.1 % prevalence) and >70 % remain untreated or inadequately repigmented, especially those with extensive (≥10 % BSA), acral, or rapidly progressive disease. Topical JAK (Opzelura; aka ruxolitinib) and calcineurin inhibitors do a pretty good job, albeit with reservations about boxed warnings that limit prescriptions from dermatologists. However, you can imagine that usage of topical therapies is often restricted to localized disease.

Vitiligo is potentially a 'good' indication for drug development because you can rapidly see skin improvements and the risk for placebo response isn't as high (repigmentation is an objective endpoint, not a symptom scale). 

One new mechanism, which I think is ___the___ critical experiment, is targeting the IL-15 / CD122 axis, which is being pursued by Teva/Forte/Anaptys/Incyte. The rationale is to deplete tissue resident cytotoxic T/NK cells by blocking IL-15 and in CD122's case IL-2, which are both responsible for maintenance of these cell types. Auremolimab which Incyte acquired from its acquisition of Villaris is the furthest along (Ph2), and several patients in forums are quite excited. $VYNE has another approach Repibresib which is a BET inhibitor in Ph2 trials. I'm not going to pretend to understand the biology here of how BET inhibition inhibits NFKB (seems super hand-wavey if you ask me), but there seems to be a nice dose response in Ph1b trials plus some nice preclinical data. 

### Alopecia Areata (AA)

Alopecia areata is similar to vitiligo in that in vitiligo there is autoimmunity against melanocytes, while in alopecia, there is immunity against hair follicles. The disease manifests as patchy hair loss, with significant psychosocial burdens. Similar to vitiligo, there is no systemic impact on life expectancy, outside of risk of self harm. 

The primary efficacy benchmark is the Severity of Alopecia Tool (SALT) which quantifies the amount of hair loss. Hitting SALT <= 20, corresponding to 80% hair regrowth is seen as the approval bar. On high dose systemic JAKi (baricitinib), the response rate is only 32-35%. Baricitinib is currently only dosed orally, and with the black box warnings dermatologists likely want safer options. Due to the high psychosocial burden, there is a high willingness to pay for new therapeutic options.

HLA-DR is the top GWAS hit, indicating that an antigen specific mechanism (e.g. autoreactive tissue resident T cells) are important in disease pathology. Like in vitiligo, patients are excited about CD122/IL-15 based approaches. [Topical Tyk2](https://pmc.ncbi.nlm.nih.gov/articles/PMC10687936/) inhibition can be tried and [Abatacept](https://www.jaad.org/article/S0190-9622(20)32694-3/fulltext) (CTLA4-Ig) can work in some patients as well. Finally, Dupixent can work in patients with high IgE at baseline (in a population with comorbid AD).

### Hidradenitis Suppurativa (HS)

HS is a highly morbid condition and is associated with worsened all cause mortality and both physical and psychosocial impacts. Lesions are painful and smelly. There are stages of severity and HS is currently seen as a chronic progressive disease which only gets worse over time.

The pathophysiology of HS is complex. There is evidence that it is Th17 driven, and IL-17 antibodies do have some efficacy. However TNFa antibodies also have activity and the Abbvie lutikizumab data is validating of the IL1-a/b pathway. Novartis is also developing Ianalumab, a BAFF receptor antibody in Ph2. Disease prevalence is higher in obese/overweight populations and losing weight reduces disease severity. Triple G incoming. 

There doesn't seem to be a north star yet for biology, but many are excited about the IRAK4 degrader approach pioneered by Kymera. IRAK4 inhibition didn't work but the differentiation is that IRAK4 also has various scaffolding functions that contribute to inflammation.

I am also excited about IL1RAP blocking antibodies, which block all IL-1, IL-33, and IL-36 signaling. In theory IRAK4 provides broader coverage than IL1RAP, but you could engineer a long half life IL1RAP for less frequent dosing and potentially differentiated side effect/efficacy profile. Sanofi is in the IL1RAP space already (SAR445399), but just in Ph1.

Ultimately, HS is a crowded marketplace for a small-medium sized opportunity that is waiting for a big clinical win.

### Prurigo Nodularis (PN)

PN is often co-morbid with atopic dermatitis, but is a distinct entity with painful nodules that appear throughout the body. The biology is understudied, but generally involves some dysregulated signaling between keratinocytes, immune cells, and neurons. Th2 biology is significant, and there is aberrant expression of IL-31 in lesions. However, PN is associated with a variety of systemic disorders and worse overall mortality, hinting at some broader immunological issue.

Itch relief is a major patient need, which Nemolizumab (IL-31RA antibody) hits the hardest and fastest. Dupixent gets there more slowly by resolving Th2 inflammation. Both drugs don't saturate on efficacy, with only 30% of patients achieving complete response.

The market is smaller, just \$2 billion annually, but underpenetrated by biologics. There are ~75k biologic eligible pts, 181k overall. Drug development has typically started in AD, then spilled into PN. Some interesting assets are IL-31 / IL-13 bispecifics, of which it looks like Zai lab with their long half life bispecific in Ph1, is in the lead.

### Psoriasis (PsO)

In my mind, psoriasis is essentially cured. Mild cases are well managed with topical creams/ointments like corticosteroids. Moderate to severe cases are addressed with long half life IL-17 or IL-23 targeting antibodies. Oruka Therapeutics from the Paragon family has the blueprint for competing commercially in moderate/severe patients (e.g. combine IL-17/23, and shoot for higher + longer exposure with half life extension).

This gigantic market (~3% of adults in the U.S.) has multiple blockbusters and has gradually shifted to long half life versions to support patient convenience. IL-17 antibodies have faster onset of effect and clinical use in more severe cases, while IL-23 blockers have been associated with more sustained responses and use in more moderate disease.

Peak revenue for Skyrizi, a p19 IL-23 antibody, is estimated to be $25 billion, a significant beat over initial estimates. Bimikizumab IL-17A/F blocker is also beating sales estimates. IL-17A has a more potent inflammatory effect, while IL-17F is more abundant in skin lesions. Blocking both seems to have enhanced efficacy versus IL-17A alone. There is an IL-17RA antibody brodalumab that has struggled commercially due to risk of suicidal thoughts in clinical trials. The relatively lower abundance of soluble IL-17A/F versus IL-17RA receptor molecules has enabled the soluble cytokine blocking approach to have comparable/improved efficacy. Lilly has a IL-17 oral small molecule from the Dice acquisition and J&J has a IL-23R small molecule inhibitor. Many have noted that small molecules do not match biologics on efficacy. 

Generalized pustular psoriasis is a rare subset of patients (~1% of psoriasis patients). It is a more severe and systemic disease. In addition to IL-23 and IL-17 blockers, IL-36 blockers such as spesolimab are also used.

### Pemphigus vulgaris (PV)

Pemphigus vulgaris is an autoimmune skin blistering disease which is caused (in part) by autoantibodies against desmoglein antigens present in the skin and mucous membranes. Patients typically start with mouth sores but the disease may evolve to include skin sores. Pemphigus foliaceus is a skin predominant subset of the disease, which typically does not involve mucous membranes. The total prevalence of pemphigus is 5.2 cases per 100k in the U.S. Interestingly, pemphigus foliaceus has some endemic form where up to 3% of certain populations in Brazil may have it.

GWAS studies have found associations with predominantly HLA gene variants, supporting an antigen mediated disease pathology (e.g. presentation of desmoglein peptides and CD4 T cell supported B cell class switching). IgG4 predominates the autoantibody repertoire.

Now patients can get Rituximab, which is effective in most patients, reaching 90% steroid sparing at 2 years. However, the effect size of BTK inhibition is small, and there was a subcutaneously delivered FcRn fail from Argenyx in PV. With Efgartigimod, Argenyx's FcRn blocker, they saw reduction in autoantibodies up to 75% with their drug, and a decrease of autoantibodies up to 70% with steroids. In the trial, response rates for complete remission were only 35% and 30% respectively. These data hint at additional mechanisms beyond antibody mediated disruption of desmoglein signaling. IL-17A has also been linked to Pemphigus in a series of mouse modeling [experiments](https://pubmed.ncbi.nlm.nih.gov/30219389/), and Dupixent has also been used in some case [reports](https://pmc.ncbi.nlm.nih.gov/articles/PMC9720249/). Indication expansion seems like the name of the game in pemphigus; trials are coming but will take time.

Pemphigus is derived from the Greek pemphix which means bubble or blister. Vulgaris means 'common' in latin. 

### Bullous Pemphigoid (BP)

Bullous pemphigoid typically affects older patients and is the most common autoimmune skin blistering disease (37.7 cases/100k). The etymology is shared with pemphigus, both coming from the Greek pemphix, with the suffix seemingly chosen for the sole reason of differentiating the two conditions. Bullous pemphigoid typically presents as itchy, red, skin blisters, commonly with fluid inside. There is a small subset called cicatricial pemphigoid which is present on mucous membranes. 

High potency steroid creams are typically first line management, with systemic prednisone or doxycycline/nicotinamide as second options. Dupixent is approved as of a few days ago (June 20, 2025). The Dupixent data are not yet published in a journal but initial topline numbers from press releases aren't that impressive. Patients are looking at a ~20% remission rate (defined as no more steroid use after a 16 week taper or new lesion growth). Roughly 40-50% of patients are benefiting. 

So there remains a significant unmet need and commercial opportunity in bullous pemphigoid, both for improved biomarkers and new therapeutics. Evidence from [mouse models](https://pmc.ncbi.nlm.nih.gov/articles/PMC3199483/) suggests a predominant role of mast cells. Omalizumab and rituximab have retrospective studies demonstrating efficacy in 60-80% of patients depending on the patient cohort. Given that the disease pathology is complex, involving autoantibodies, mast cells, Th2 inflammation, and potentially other axes, maybe there are opportunities for co-formulation or bispecifics. As new mechanisms including TSLP and OX40 mature, perhaps these will also be able to demonstrate efficacy.

## Gastroenterology & Hepato-Pancreato-Biliary

### Eosinophilic Esophagitis (EoE)

EoE is a very interesting indication for expansion of Th2 targeting drugs (e.g. IL-13, IL-4R, TSLP, STAT6, etc.). Both TSLP and its receptor along with STAT6 are GWAS hits, and Dupixent is approved for children and adults age 1 or older with EoE. Frontline therapy is PPIs, with topical corticosteroids like oral budosenide suspension recently approved for patients 11 or older. In patients refractory to PPIs, Dupixent had ~60% histological remission rate (reduction of eosinophils in esophageal biopsy) when dosed at either weekly or Q2W, but only hit on the dysphagia (trouble swallowing) patient reported outcome measure at weekly dosing, which is what is on the label.

The dysphagia endpoints are harder to hit on because they reflect a baseline level of esophageal fibrosis. Median diagnostic delay is ~5 years (and overall the condition is underdiagnosed) and many adults with EoE need some sort of dilation procedure. You can sort of think of it like Barrett's esophagus which also induces remodeling of esophageal epithelium but instead of acid reflux, you have persistent inflammation that induces fibrosis.

Dupixent is the only approved biologic (2022) and the theoretical TAM is 3-7 billion and growing (biologics and even topical budosenide have limited market penetration; ~15% of 200k total patients). Relapse rate off treatment is high (60-70%) so continued chronic treatment provides a lasting market. The key experiment with EoE is whether more potent Th2 shutdown with bispecifics or more potent antibodies (e.g. IL-13/TSLP, APG777) will continue to improve on efficacy. The success of weekly but not biweekly Dupi suggests there is an exposure efficacy relationship that has not yet been saturated. Additionally, adding on an anti-fibrotic into the management of these patients (e.g. [Losartan](https://pubmed.ncbi.nlm.nih.gov/39059581/)) to hit both upstream Th2 and downstream fibrosis that is causing dysphagia is logical.

### Celiac Disease

Highly prevalent disease (1% global population) that has essentially been abandoned by large pharma (with exception of Teva/Takeda). There are a very complicated set of patient presentations ranging from those who can seemingly tolerate gluten with no symptoms but histological damage, to patients that have it so bad that they can even develop celiac-associated T cell leukemia. It is safe to say that this is indeed a massive market that causes significant patient morbidity and inconvenience -- a large unmet medical need. 

Teva, Calypso/Novartis, Forte, and other groups have recently reported data from IL-15 / CD122 targeting antibodies. Collectively, the data indicate that blocking this pathway can reverse disease associated pathology on histology in biopsy specimens. As of this writing, Forte is the first to also demonstrate reductions in GI symptoms from a gluten challenge. 

CD122 in my opinion makes more sense than just targeting IL-15 for a couple reasons. First, it's the receptor, meaning that you can get greater efficacy with less dose (receptor internalization, easier to saturate in terms of molarity, less need to worry about resynthesis). Second, IL-2 signaling which is also blocked by targeting CD122 is most correlated with patient symptoms. Both IL-15 and CD122 antibodies cause significant NK cell depletion, detectable in peripheral blood. While there were no dropouts in the Forte Ph1b study, longer trial designs may detect whether there are consequences to sustained NK cell depletion. Updated data from Teva's IL-15 antibody, which has more potent NK cell depletion than Calypso's antibody plus a longer half life, will read out 2h2025 so we will get start to understand the relative merit of solely targeting IL-15 versus the combination with CD122. The Forte molecule is currently being dosed weekly I.V., which likely isn't commercially viable so there is an opportunity to innovate on the antibody design side as well.

Other approaches for celiac disease include tolerance inducing vaccines (e.g. TAK-101 and VTP-1000) and transglutaminase inhibitors (e.g. ZED1227). A fun fact is that my boss at the time when I was an intern at Vaccitech (now Barinthus) designed the peptide sequences for VTP-1000 and I had some very peripheral involvement. VED1227 is a transglutaminase inhibitor dosed daily which hit on a Ph2b trial published in [NEJM](https://www.nejm.org/doi/full/10.1056/NEJMoa2032441). This was all the way back in 2021 with no apparent update on the Ph3 status. Ultimately, the ideal product is a tolerance inducing therapeutic vaccine, but the jury is still out whether the efficacy will ever get there. In the interim, a long half life IL-15/CD122 product in combination with GFD could significantly improve clinical symptoms and outcomes.

### Inflammatory Bowel Disease (IBD)

The biologics market typically refers to the moderate to severe subset, meaning Mayo score >6. Mayo score is a composite scoring system based on stool frequency, rectal bleeding, physician's global assessment, and endoscopic appearance.

The blueprint to addressing this one is laid out by Charlie Lees on his [Substack](https://substack.com/@charlielees). Essentially, you will cycle through a TNFa first (the sequencing may change, for ex TNFa got beat by Vedo h2h), then through various other biologics like Vedolizumab (against α4β7 integrin), Skyrizi (a IL-23A blocker), and now likely some TL1A blocker and S1P inhibitors (and Obefazimod maybe??). Patients never get cured, so will be managed chronically the rest of their lives. While somewhat depressing, this is great for biopharmas, as you don't necessarily need to show superiority. You just need to be an orthogonal mechanism that demonstrates efficacy in a biologic experienced population. 

Great market and certainly open for business. Up to 1% of adults in the U.S. have some form of IBD. Combinations, co-formulations, and competition on half life (e.g. $SYRE) will dominate care until most drugs go generic in 2032.

Moving forward, I think the way IBD pushes forward is more widespread use of endotypes to guide care. Multiplex ELISA based measurements from patient serum, or staining based biomarker tests on biopsies. Very bullish on Prometheus Laboratories (distinct from Prometheus Biosciences) to continue to expand their diagnostic offerings in IBD to aid patient selection and therapy monitoring. I could see several distinct patient segments with clear therapeutic strategies:

1. TL1A high
2. Th17/IL-23 high
3. Lymphocyte high
4. TNFa high

Prometheus Biosciences has also developed the first companion diagnostic for TL1A, a genomics based SNP test. This has already shown utility in their landmark NEJM paper to be able to guide care. 

### Crohn's Disease

Chron's disease is sort of the same story as IBD. You have the same efficacious mechanisms (TNFa, IL-23, a4b7, TL1A). The differentiator is that it can affect any part of the digestive tract and can have many complications. 

Business wise, this doesn't mean too much. Similar to IBD, the name of the game is increasing drug exposure, layering on multiple mechanisms simultaneously, and increasing convenience. Charlie Lees [again](https://charlielees.substack.com/p/after-tnf-failure-in-crohns-disease).

### Primary Sclerosing Cholangitis (PSC)

Primary sclerosing cholangitis is a fibrotic inflammatory disease of the bile duct. Strictures prevent bile flow, leading to a diverse set of symptoms including fatigue, vitamin deficiencies, dry mouth/eyes, and itching. There is a 3-fold mortality increase, with mOS in the 10-20 year range post diagnosis (median age of diagnosis 30-40 years old). No drugs are approved and liver transplant is the only disease modifying therapy, but is not curative. A bile acid analogue, norucholic acid, recently demonstrated pbo adj. response rates of ~10% in a large Ph3. This is likely to be approved. However, the pill burden is 6 capsules / day, 250mg each. Over the course of 2 years, that is a kilogram of drug per patient.

What kind of new mechanisms for disease modifying therapy exist? Chemomab has a CCL24 antibody, nebokitug, which has some directionally positive Ph2 data but likely doesn't have a way forward without the company raising a large sum of money for their Ph3 trial. TL1A could have a significant role here as well. [Mice](https://patents.google.com/patent/US8766034B2/en) with TL1A overexpression in lymphocytes or myeloid cells are a serviceable model for the disease.

### Autoimmune Hepatitis 

Autoimmune hepatitis (AIH) is a severe chronic liver disease with 40-50% mortality rate if untreated. Patients typically present with increased IgG titer, fatigue, jaundice, and liver fibrosis on biopsy. There are 140k patients in the U.S. There are no approved biologics, and while calcineurin inhibitors, MMF, and high dose prednisone (0.5-1 mg/kg) are able to significantly extend lifespan, there is significant treatment associated toxicity. 35% don't respond and >50% relapse after going into remission.

Zetomipzonib from Kezar is currently the most promising new treatment option. It is a selective immunoproteasome-β5i/β1i inhibitor, which achieved remission in 28% of patients (3% w/ placebo) at 24 weeks in a Ph2a trial. 

A small 35 patient retrospective analysis of AIH patients treated with Rituximab showed that 31/35 (89%) of patients achieved a complete response. This disease is begging for a randomized TCE or other B cell depletion trial. 

### Autoimmune Pancreatitis

This is a rare (<20k pts in U.S.) form of chronic pancreatitis driven by inflammation of primarily pancreatic ducts. There are two variants, type 1 which is driven by IgG4, and is really a category of IgG4-related disease, and the other which is more neutrophilic. Both variants are treated with high dose steroids, typically over 4 weeks, with a 3-6 month taper. Type 1 is more likely to relapse but is responsive to B cell depletion strategies, and Type 2 mostly resolves after a treatment course of steroids. Honestly not a huge unmet need.

## Ophthalmic Diseases

### Thyroid Eye Disease (TED)

There are 190k people with moderate to severe TED in the U.S., and commercial penetration of biologics continues to grow. The pathophysiology is well understood -- autoantibodies activate IGF-1R and/or TSHR pathways. TSHR blocking antibodies would cause hypothyroidism, and as a result, the majority of drug development has targeted the IGF-1R pathway. 

Tepezza, an IGF1R blocking antibody, did $1.9 billion in sales in 2024 as the only approved biologic for TED. A treatment course can run >$200k. While a SC formulation is being developed, Tepezza currently is given once every 3 weeks for 8 total infusions (60-90 minutes each). There are also tolerability questions, with >10-15% of patients experiencing hearing loss, and some patients having muscle cramps and hyperglycemia. The relapse rates are seemingly also pretty high. In a small published [study](https://pubmed.ncbi.nlm.nih.gov/38142982/), only 33% continued a response to Tepezza at 2 years, and almost no patients had improvement in diplopia. 

[Viridian](https://s203.q4cdn.com/807813999/files/doc_presentations/2025/06/Viridian-June-Corporate-Deck_FINAL.pdf) is developing a long half life IGF-1R antibody. Lassen Therapeutics is taking an orthogonal approach by targeting IL-11R with an antibody. IL-11 is responsible for orbital fibroblast activation and pathway blockade could address pathophysiology untouched by Tepezza or other IGF-1R approaches and without IGF-1R associated toxicities.

[Here](https://eyewiki.org/Biologics_for_Thyroid_Eye_Disease) is a good review of the TED space (EyeWiki).

### Geographic Atrophy (GA)

Geographic Atrophy remains 'uncracked' from a therapeutic perspective. While complement blockers can slow the rate of progression, [enthusiasm](https://www.aao.org/eye-health/tips-prevention/syfovre-izervay-geographic-atrophy-amd-macular-deg) for this class of agents is not high and most patients remain untreated. Marginal efficacy, frequent dosing, and rare sight threatening toxicities (retinal vasculitis, development of wet AMD) are responsible for poor commercial penetration.

GA is also known as late stage dry aged-related macular degeneration (AMD). There is localized atrophy of retinal tissue, including retinal pigment epithelium (RPE) and their capillaries. As a patient, you get 'islands' of lost sight which continue to grow as the disease progresses.

What to do about GA? Some are [excited by cell therapy](https://www.nature.com/articles/d41586-025-00659-2). This could be one area where cell replacement gets its first win.

### Uveitis

Uveitis is the 4th leading cause of blindness, accounting for 10% of blindness cases in the U.S.. Non-infectious uveitis compromises ~400k patients. It is often idiopathic and presents with typical inflammation associated symptoms including redness, swelling, and pain. First line treatment is topical steroids, with 2nd line treatment being more aggressive immunosuppression. Allergan/Abbvie has developed Ozurdex, a dexamethasone intravitreal implant and Humira (TNFa blocker) is also used in the 2nd line.

There is steroid toxicity in the eye including increasing IOP (causing glaucoma), and cataracts.

Brepocitinib, a TYK2/JAK1 inhibitor from Priovant/Roivant/Pfizer, is poised to disrupt the 2nd line market. In the POC NEPTUNE trial, the week 24 treatment failure rate was ~30%, compared to [~50% for Humira](https://www.nejm.org/doi/full/10.1056/NEJMoa1509852). IL-6 mabs are also in play, and tocilizumab is often prescribed off label, with significant efficacy in both TNF naïve and experienced patients.

Trials can be very small. The Brepocitinib Ph2 trial enrolled only 26 patients, and randomized to a high vs low dose of the drug (no placebo). Their Ph3 trial is ongoing and will enroll 300 patients worldwide. Estimated completion is in Q1 2028.

## Rheumatology & Connective-Tissue Diseases

### Rheumatoid Arthritis (RA)

The key question you need to answer is whether 4th line RA is interesting to you. RA is obviously a massive indication, affecting up to 1% of the U.S. population. The pathophysiology is complex, with multiple endotypes. The common features are inflammation of joints, commonly with autoantibodies against citrullinated peptides, rheumatoid factor, various collagens, and proteoglycans, fibrosis and proliferation of fibroblast like synoviocytes, T cell activation, and myeloid cell infiltration.

Methotrexate is given first line and afterwards, IL-6 and TNF-a classes are dominated by biosimilars at this point. Abatacept (CTLA-4 mimic), Rituximab, and JAK inhibitors are all also approved and used. Difficult to treat RA (D2T RA) or aka polyrefractory RA represents ~15% of patients and refers to patients who have failed 2+ disease modifying drugs. This might mean cycling through an IL-6 and a TNFa blocker, or multiple other medications including from clinical trials. D2T RA is a market worth ~\$1 billion, but you wonder if the difficulty of the disease makes it even more difficult to find a drug effect.

Some interesting new mechanisms are in development including PD-1 agonism (\$ANAB). However, the PD-1 agonism data is really quite unimpressive.

Spyre is running a TL1A trial. They have found that TL1A inhibition has a strong effect in preclinical models of RA, including the collagen induced arthritis model. Does the rat collagen induced arthritis model mean anything? On one hand, it has very good specificity, as all approved treatments work in the model. However, it didn't screen out failures on IL-17 and p38 inhibitors. This model is more acute and resolves upon treatment, while RA in human patients is obviously a chronic lifelong disease. TL1A abundance is correlated with disease severity, and TL1A gene polymorphisms confer higher TL1A abundance and are associated with disease prevalence.

TCEs could find a role in D2T RA according to this [small trial](https://www.nature.com/articles/s41591-024-02964-1#Sec2). For patients with really no other options, immune reset has sort of remarkable efficacy. If even polyrefractory RA is amenable to cure with immune reset, this is kind of Nobel prize winning news is it not? Cures for autoimmunity is something that I don't think many imagined to be possible and it's a very simple idea.

### Psoriatic Arthritis (PsA)

Psoriatic arthritis differs from rheumatoid arthritis in that the aetiology much more resembles psoriasis (ie. Th17 driven) than RA (ie. autoantibodies, synoviocytes, fibrotic remodeling, etc.). There are maybe 2 million people who have this disease in the U.S., with average onset in the one's 30s-50s. Symptoms are thick scaly plaques on skin and nails, swelling and pain on peripheral joints, hands, and feet, stiffness, and back pain, fatigue, and significant psychosocial burden. Bone remodeling including both erosion and spur formation is a unique feature. 

This is a $12 billion market where therapies still only have middling efficacy. The major classes include TNFa, IL-17/23, JAKs, PDE-4, abatacept, and soon TYK2. In the lowest responder bar, ACR20, the most effective classes (TNFa, IL-17/23, JAK) only reach ~55-75% response rates. Hitting both IL-17A and IL-17F is more effective than IL-17A alone. New mechanisms that work and enable stacking will be able to penetrate a massive market. Interestingly, this market has not seen basically any biotech penetration except Oruka, which is developing a me-better IL-17A/F.

### Axial Spondyloarthritis (AxSpA)

Axial refers to an axis of rotation and Spondyl refers to the spine. Axial spondyloarthritis is inflammation of tendons, joints, and ligaments, typically manifesting at the sacroiliac joints and spine (ie. chronic back pain). 0.9-1.4% of the overall population have it, so it is similar to RA in terms of prevalence. In its extreme form, the disease can lead to the bony fusion of vertebral joints. Cardiovascular disease, depression, and fatigue are all associated with AxSpA, so significant morbidity is associated. Also, hi. Median onset is 26 years old.

Humira seems to work pretty well according to patient forums, but only in ~60% of patients. If patients develop ADAs or run out of TNFa blockers, they can move on to IL-17A blockers like Cosentyx which are also approved. 

There is certainly therapeutic whitespace to address the ~40% non-responders and it's a large market. Women, older patients, those with higher functional impairment and high BMI, and those without elevated blood inflammation are less likely to respond to anti-TNF. However, earlier diagnosis and treatment probably significantly improves response rates. TYK2 inhibition is in the pipeline. While the IL-17 and TNF-a class both work, response rates are not at psoriasis levels of 90+%. Given how large an indication this is and the significant (chronic) morbidity associated with it, there remains a large unmet need. New mechanisms with improved potency or that enable more 'stackable' combinations would definitely be commercially viable.

### Ankylosing spondylitis (AS)

Ankylosing spondylitis is a subset of AxSpA that can be seen on radiographic imaging, and many patients with AsSpA convert to the more severe AS diagnosis.

A Nature Medicine paper came out in 2023 describing a [prototype therapy](https://www.nature.com/articles/s41591-023-02613-z) for patients with AS. It turns out that patients with this disease commonly have expansion of a specific T cell TCRb CDR3 motif, particularly containing TRBV9 that recognizes an autoantigen in the spine and large joints. You can raise an antibody against TRBV9 and treat patients with it, thus clearing out the autoinflammatory CD8 T cells and resolving symptoms. This approach is now being pioneered by [Hillstar Bio](https://endpts.com/hillstar-bio-raises-67m-for-immunology-drugs/) which just raised money in March 2025. 

In addition to this precision approach, the typical gamut of IL-17s, TNFa, JAKs, etc all work to varying degrees. None are curative or get anywhere above the 50-60% efficacy range.

### Osteoarthritis (OA)

Osteoarthritis will affect nearly 10% of the world population. It already costs Medicare/Medicaid more than \$185 billion. As drug indications go, thinking about and being able to improve osteoarthritis symptoms would be magic. This is a prototypical disease of aging, with the pathophysiology involving cell senescence and local sterile inflammation and 'wear and tear' of cartilage and breakdown. Obesity and weight gain in aging is significantly associated with the disease due to the excess load placed on knees. In fact, most of the GWAS hits are related to weight, and weight loss medications are highly effective at reducing OA symptoms. 

Managing pain is a major goal of care. Patients wake up with morning stiffness and any sudden movements can be painful, which significantly worsens mobility and prevents patients from experiencing the benefits of exercise. The standard of care is simply management with weight loss and exercise, NSAIDs (both systemic and topical), steroid injections, and eventually knee/hip replacement surgeries. Unfortunately, there just aren't any disease modifying drugs approved yet.

The approval bar admittedly is high. You need both structural modification plus pain relief. FGF-18 injections and Cathepsin K inhibition improve structural features, but don't address pain. Several pain pathway blockers including targeting NGF and TRKa have entered or completed clinical trials. Expectedly, they improve pain but in some cases make the OA even worse. There is one drug being trialed by this very interesting company called BioSplice/Samumed. It is a [CLK/DYRK inhibitor](https://ard.bmj.com/content/83/Suppl_1/194.2?utm_source=chatgpt.com) which is only administered at 0.07 mg, annually via intraarticular injection. The effect size is small with lots of variability but alas there is a difference.

While the pipeline for this disease is barren, I'm excited about the opportunities for drug development. You have a disease where intraarticular injections are commonly performed, allowing you to play with pathways that might be toxic systemically and also to potentially get intraarticular biomarker measurements. So many people have it and suffer significantly, and the target space is clearly distinct from other rheumatological diseases so there is room to be creative. You can think about cell therapies that secrete FGF-18 and pain blocking antibodies, or drug depots to modulate the Wnt pathway over a more sustained window. Other animals that weigh a lot more seemingly have very robust joints, which we could study to understand whether there are specific protective features. One group at NYU made the fascinating discovery that [chondrocytes express the sodium channel Nav1.7](https://www.nature.com/articles/s41586-023-06888-7#Sec4) and that conditional deletion protects against OA and reduces pain.

### Polymyalgia Rheumatica (PMR)

There was a great 'call to action' [article](https://www.sciencedirect.com/science/article/pii/S2665991325000955) that came out while I was writing this post. Written by David Lieu, a rheumatologist in Melbourne, he argues that PMR has been underestimated and understudied. IL-6 inhibition with the IL-6R antibody [sarilumab](https://www.nejm.org/doi/10.1056/NEJMoa2303452) is the only approved biologic, and most patients are managed chronically with steroids. While steroid doses are not acutely as high as other conditions, the chronic nature of them make the cumulative dose quite high. For whatever reason, it is difficult to taper off of steroids in PMR, and even in sarilumab's landmark NEJM paper, only 28% were able to remain in remission of steroids after a year of treatment, compared to 10% in the placebo group.

The lifetime incidence of this disease is 2%, and patients suffer from shoulder and hip girdle pain and stiffness. Lots of people have it, no one is developing drugs for it, and morbidity, while not as bad as some other disorders described in this post, is still significant. Target ID is obviously the tough part here. Plasma proteomics indicates that there is enriched IL1RL1, IL15, CXCL13, TGFA, PLAUR, and IGF2R in patients relative to controls.

### Still's Disease

There are two presentations of this IL-1/18 driven systemic autoimmune disease. sJIA stands for systemic juvenile idiopathic arthritis and is the child form of Still's and ASOD is adult onset Still's disease. The dangerous part of this disease is potential for escalation into macrophage activation syndrome (MACS), which is a cytokine storm syndrome with significant risk of mortality. 

Patients present with a high fever, rash, arthralgia, and sore throat. Steroids are given and tapered with an IL-1 blocker (Canakinumab or Anakinra). Tocilizumab or JAK inhibition can also be given if the response is inadequate. MACS needs to be managed separately with IFNg blockade. New therapeutic development for Still's is quite rich. Given the recent understanding that this is IL-18 driven, bispecifics combining IL-1b blockade with IL-18 (MAS825; Novartis) or systemic administration of IL-18BP (Tadekinig alfa) are both in Ph2 and Ph3 respectively. While most patients are controlled, there are still kids that die from inadequate control of MACS, and some who get erosive arthritis. 

### Systemic Lupus Erythematosus (SLE)

330k patients in the U.S. have this disease. It slowly progresses into lupus nephritis, a devastating kidney disease.

Lupus is B cell and interferon driven, and thus far only two therapies (Belimumab, the BlyS antibody, and Anifrolumab, the IFNAR1 antibody) are approved. Autoantibodies against nuclear antigens (e.g. dsDNA) develop and immune complexes circulate, activating complement and causing tissue damage. Flares of inflammation, driven by type I interferon and plasmacytoid DCs (pDCs), cause fever, rash, and fatigue.  

A lot is in the pipeline, including B cell depletion approaches, pDC depletion (BDCA2), and Tyk2 inhibition. Several CAR-T studies have shown that immune reset works. The question is whether that can be achieved with more mild therapy, such as TCEs. Combinations and bispecifics obviously are in the works as well.

### Systemic Sclerosis (SSc)

This disease is also known as scleroderma. SSc commonly presents with interstitial lung disease (SSc-ILD), where fibrosis and inflammation in lung tissues cause shortness of breath, cough, and fatigue. It can be either limited or diffuse (more severe, involving skin). First line therapies include MMF, nintedanib, rituximab, and tocilizumab. It is an interesting disease because while these therapies all help, none seem to address the root of what is causing the ILD.

B cell depletion seems to work according to CAR-T trials. In 22 patients dosed so far, all had improvement.  

Atyr has a NRP2 modulator, which has an interesting connection to the disease. SSc patients commonly have anti-tRNA synthetase antibodies, which are notable because certain tRNA synthetases are known to have splice variants secreted extracellularly. The company has characterized these splice variants, finding that they bind to NRP2 and have protective properties, reducing inflammation. An initial analysis in a set of patients showed some clinical improvement in sarcoidosis patients, a related condition, and 3q25 is the Ph3 readout in pulmonary sarcoidosis. An interim analysis in SSc-ILD was conducted in Jun 2025 and showed clinical improvements in 3/4 patients with diffuse SSc-ILD. The drug is given intravenous monthly. 

There are lots of interesting GWAS hits including TNSF4 (OX40L), IL12RB1/2/IL12A, STAT4, IRF5, BLK, IRF7/CDHR5, GSDMB/IKZF3, IRF8, and TNFAIP3. Several of these are druggable and active programs within biotech including OX40 and IRF5. A TL1A Ph2 trial ([ATHENA-SSc-ILD](https://clinicaltrials.gov/study/NCT05270668)) has primary completion in May 2026. Once these cards flip over and combinations are inevitably tested, we might get a better idea of the pathophysiology. Overall, this one is a mystery to me.

### Relapsing Polychondritis

This is a rare orphan indication with maybe 10k cases in the U.S., though concrete prevalence/incidence is not yet known. Patients get painful inflammation of the cartilage and proteoglycan rich tissues. Many of the classic signs of autoimmunity are present including autoreactive antibodies (in this case against type 2 collagen), elevated Th1/Th17 cytokines, complement activation, and neutrophilic infiltrate. Interestingly, relapsing polychondritis is commonly secondary to VEXAS syndrome (which is covered below).

As you may imagine, patients are treated with the classic first line steroids, methotrexate, MMF, colchicine, etc. In non-responders, relapsing patients, and patients progressing due to treatment toxicity, you start reaching for the IL-6, TNFa, and IL-17 classes. Abatacept, the CTLA-4 mimic, has shown effectiveness in preliminary clinical trials as well. It is an orphan indication with multiple effective drug classes so RP is not a first choice for drug development. However, add it to the list of indications where tolerenogenic vaccines could be trialed.

### Vasculitides

Inflammation of blood vessels has many manifestations, each with distinct clinical presentation, but I am grouping them all into one category. While each individually are rare, they collectively represent tens of thousands of patients and thus a sizable unmet need. There are commonly autoantibodies or immune complexes that deposit, activate complement, and damage vessel integrity. A non exhaustive list of some of the more common ones include:

- Primary CNS vasculitis
- Giant cell arteritis (IL-6 driven)
- Takayasu arteritis
- Polyarteritis nodosa
- Kawasaki disease
- ANCA associated vasculitis
- Eosinophilic granulomatosis with polyangiitis (IL-5 driven)
- IgA vasculitis 
- Rheumatoid vasculitis
- Churg-Strauss syndrome
- Behcet's Disease

Avacopan, Rituximab, and Tocilizumab are the major set of drugs used, with response rates (defined as steroid free remission) hovering around 50-60%. In light of growing appreciation that these are autoantibody driven, FcRn inhibition and IgG depleting strategies are being explored. 

### Myositis

These are a diverse set of clinical syndromes (Dermatomyositis (DM) / polymyositis (PM) / Inclusion-body myositis (IBM) / immune-mediated necrotizing myopathy (IMNM)) that all involve immune mediated muscle damage. Altogether, these represent tens of thousands of patients, a sizable market. 

These each involve a distinct set of autoantibodies and clinical presentations depending on where the damage lies. In IBM and PM, there is more CD8 T cell involvement, while in DM and IMNM, disease is more autoantibody driven.

IVIg was the first FDA approved biologic, achieving 79% response rate versus 44% on placebo, and in some patients, Rituximab is effective. Early line management involves high dose steroids, methotrexate, and MMF. Matt Gline is bullish on FcRn in myositis. I think this is another condition where we will see how far B cell depletion will take us. It's hard to start thinking about alternative approaches until these data are mature. CD-19 CAR-T has been tried in 13 patients so far, with major clinical responses in all of them. 

### Recurrent Pericarditis

Recurrent pericarditis, as the name implies, is a chronic inflammation of the heart. There is typically a trigger, such as an infection or other comorbid autoimmune disorder (maybe even covid/mRNA vaccine), but symptoms such as fever, elevated CRP, chest pain, etc may persist. Steroids with taper and colchicine are typically first line. Targeting the IL-1 pathway with canakinumab, and especially rilonacept, which is an IL-1a/b trap, is extraordinarily effective. Rilonacept is dosed weekly SC, but achieves flare control and pain relief in >90% of patients. Potentially an opportunity for improving half life via conjugation to Fc but this is already a fantastic drug that is already beating sales estimates and will eventually do >$1b in sales. NLRP3 inhibitors (Dapansutrile; Olatec Therapeutics) are also in trials and may provide a daily oral option.

## Allergy & Type-2-Driven Disorders

### Chronic Spontaneous Urticaria (CSU)

Chronic spontaneous urticaria translates to persistent random itchiness. >500k people in the US live with this disease and the overall prevalence is estimated at 230 cases per 100,000 adults. Antihistamines, at recommended doses, relieve symptoms in less than 50% of patients, with up to 25-33% remaining symptomatic even after 4x dose escalation.

The disease pathology involves mast cell activation, IgE and IgG autoantibodies, and type 2 inflammation, and accordingly treatment options include Dupixent, Omalizumab, and soon, KIT blockers / inhibitors (Jasper (Briquilimab) and CellDex (Barzolvolimab) on the antibody side, and Cogent Biosciences & Blueprint Medicines (now Sanofi) with wild type KIT small molecule inhibitors). Biologic penetration is, to date, still poor so there is still significant room to penetrate what is a sizable market.

KIT, IgE, and IL-13 are already three blockbuster medicines that haven't penetrated CSU in monotherapy, let alone in combinations. Hard to say the unmet need is pressing until these large Ph3 experiments read out.

### Severe Asthma

Just like in COPD, there is the T2 endotype which is driven by Th2 inflammation and responds to biologics like Dupixent, IL-5, TSLP, and IgE blockers, and a non-Th2 endotype (~15% of patients) which does not have elevated cytokines or eosinophil biomarkers and may be driven by alternative biology, such as chronic infection, smoking, neutrophilic infiltrate, etc. It is another massive market where there is room for multiple biologics to compete and have patients cycle through if there is lack of response. Better biomarkers are being developed to better stratify patients. 

I'm excited about longer half life IL-13 and TSLP / TSLP receptor blocking molecules from Upstream and Apogee. For the non-Th2 driven endotype, TSLP blockade does still have some level of efficacy, albeit lower than in the Th2 endotype. Verona's PDE3/4 inhibitor that has had stunning uptake in COPD is also being trialed in asthma. Between TSLP, PDE3/4, and combination studies, patients with severe asthma have many future options to look forward to.

### Chronic Rhinosinusitis with Nasal Polyps (CRSwNP)

CRSwNP is very often co-morbid with asthma and the biology is very similar in that both are driven by Th2 inflammation. 

Omalizumab, Depokimab, and Dupi are approved. Tezspire should be approved later this year (Q4W), Lebrikizumab (Q2-8W) is in a Ph3, and verekitug, Upstream’s TSLPR (Q12W) should have Ph2 data later this year.

This is a disease which in my mind is basically cured by Dupixent. The outcomes are very good according to [this](https://onlinelibrary.wiley.com/doi/10.1111/all.15796) article. There are maybe 10-20% of patients who don’t have an adequate response, and the investigators linked showed you can taper Dupi doses over the course of 2 years, in some cases out to Q12W. Dupi efficacy saturates around 24 weeks and you could make the argument for deeper responses, but I think the rationale to push for better efficacy is definitely higher in other indications.

Additionally, the prevalence is ~6-7x lower than other Th2 respiratory indications such as asthma/COPD. Dupi reached $1B in sales and there are still ~900k pts in U.S./Europe, but definitely smaller than asthma / COPD / other Th2 driven diseases. In a sample size of ~75k pts from 2018-2023, biologic penetration is at ~12%, with the vast share (90%) going to Dupi. However, ~50% discontinue and only 2.6% switch therapy which to me says that they get better and then stop drug.

### Food Allergy

Food allergy is undoubtedly a large indication and has significant potential to impact quality of life. The [success](https://www.nejm.org/doi/full/10.1056/NEJMoa2312382) of Omalizumab in food allergy has reawakened drug development. The dosing regimens for Omalizumab are not ideal, as some larger patients require up to 4 pre-filled syringe injections to see the requisite IgE inhibition. Thus, there is an opportunity for a long half life version of Omalizumab with improved IgE clearing and inhibition of resynthesis.

However, there will be little pricing power as omalizumab will be generic in 2 years and there are 4 other public IgE approaches including RAPT, Merida Biosciences, Lycia Therapeutics, Seismic Therapeutics.

Oral immunotherapy as antigen sensitization is the alternate approach, and this works but is very arduous. Roche/Genentech likely has interest in lifecycle management for Omalizumab and may be able to develop or in-license a long half life version (e.g. \$RAPT). Regeneron has dreams of curing food allergy through autoantibody producing plasma cell depletion (via BCMA) and administering Dupixent on top to prevent class switching and relapse of the allergic B cell response. Lots of creative strategies and ultimately I do think food allergy is curable within our lifetimes. 

## Pulmonology & Interstitial Lung Disease 

### Idiopathic Pulmonary Fibrosis (IPF)

IPF is another disease of old age where patients have difficulty breathing, painful cough, and a high infection rate. Patients have very short median overall survival of just 2.5-5 years, most commonly passing away due to respiratory failure -- a horrible way to die. Each year, there are 30-40k patients diagnosed, totalling a 100k overall prevalence in the U.S.

There are two approved drugs: nintedanib (multispecific PDGFR, FGFR, VEGFR inhibitor) and pirfenidone (anti-fibrotic with unknown mechanism). Several new drugs have shown proof of concept including [nerandomilast](https://www.nejm.org/doi/full/10.1056/NEJMoa2503643), a PDE4B inhibitor, and BMS-986278, an LPA antagonist.

Locally acting TGF-beta blocker could be interesting (older versions failed due to systemic toxicity). Additional approaches directly targeting fibrosis via various fibrotic factors (e.g. CTGF, LOXL2) haven't worked either. I included this section mainly because I wanted to mention the IL-11 antibodies that are being trialed here. Being currently trialed by Boehringer Ingelheim (current king of fibrosis), this class, in addition to the famous [longevity benefits](https://www.nature.com/articles/s41586-024-07701-9), has shown impressive [disease reversing](https://www.science.org/doi/10.1126/scitranslmed.aaw1237?url_ver=Z39.88-2003&rfr_id=ori:rid:crossref.org&rfr_dat=cr_pub%20%200pubmed) activity in mouse models of IPF. 

### Sarcoidosis

Sarcoidosis is another very difficult pulmonary condition, driven by the formation of granulomas. Antigens are typically unknown but common are associated with air pollution, so likely an inhaled environmental antigen. There is significant mortality, as granulomas in the lung can cause difficulty breathing, inflammation, fibrosis, etc. Though most commonly in the lungs and lymph nodes, there can also be neurosarcoidosis, and sarcoidosis in the heart, eyes, and skin.

First line treatment is of course steroids, but long term steroid toxicity makes non-steroid options a major unmet need. TNFa blockers work, but with a small effect size. JAK inhibition works for skin granulomas. As previously written in the SSc section, there is an interesting hypothesis being tested by Atyr Pharma, where their hypothesis is that tRNA synthetase autoantibodies provide a clue into the formation of granulomas and therapeutic targeting may be beneficial.

Endpoints for trials are improvement in lung function and reduction in steroid dose. Ultimately, drug development in sarcoidosis is very slow, making it a terrific opportunity for new drug development, provided there is a differentiated strategy. CSF1R inhibition? Seems like a terrific application for spatial -omics. 

### Pulmonary Arterial Hypertension (PAH)

Pulmonary arterial hypertension is a lung disease of the pulmonary arterioles. Remodeling of arterioles increases pulmonary vascular resistance, making it difficult for the right ventricle to pump blood into the lungs for oxygenation. It is a progressive disease that eventually causes right heart failure and mortality (5 yr OS 71%) if untreated. It is a subset (1%) of the much larger indication of pulmonary hypertension, which affects roughly 40,000 patients annually. Distinct from PH, there are efficacious targeted therapies for PAH. These include prostacyclins (e.g. treprostinil), vasodilators, multitargeted TKIs (e.g. seralutinib, imatinib), PDE5 inhibitors, and endothelin receptor antagonists. Recently, sotatercept, a TGF beta / activin ligand trap, was approved by the FDA after Merck acquired the biologic from Acceleron. 

Sotatercept is 'revolutionary' because it targets a genetically validated pathway (mutations in BMPR2 are found in many PAH patients), remodels vasculature (offering histologic improvement), and has significant improvement on clinical parameters (far more than other classes). The question is 'how far will sotatercept go', rather than 'will anything surpass sotatercept'.

### Chronic Obstructive Pulmonary Disease (COPD)

COPD is the world's 4th leading cause of death (~3.5 million annually). It is commonly a consequence of chronic irritant exposure (e.g. environmental pollution, smoking, etc.) and because of this, largely preventable. 660 million people worldwide have it, with enrichment in low and middle income countries (only 15 million in the U.S.). Most patients are on bronchodilators and reassessed every 3-6 months. The most aggressive treatment regimen is inhaled corticosteroids (ICS), long acting beta agonists (LABA), and long acting muscarinic agonists (LAMA). Now, an inhaled PDE3/4 inhibitor, Ohtuvayre, developed by Verona Pharma, is being added to this regimen for patients still not adequately controlled. 

Still, many patients have severe disease that slips through all inhaled therapy. These patients with Moderate to severe airflow limitation, >2 moderate or >1 severe exacerbations within the last year, and high levels of blood eosinophils, are the 'biologic eligible' population, also known as the T2 endotype. This is roughly 5-8% of the overall COPD population.

An eosinophil cutoff of >=300 cells/ul is commonly used as a threshold for a 'biologic targetable' endotype, and is the cutoff used for prescribing approved drugs Dupixent and Nucala (IL-5 antibody; GSK). In addition to IL-4Ra and IL-5, TSLP blockade has shown to be an efficacious mechanism in eosinophil cutoffs of >150 and >300 cells/ul. Proof of concept has come via AstraZeneca's tezepelumab, but additional drugs including Upstream Bio TSLPR antibody, various long half life TSLP antibodies, and bispecifics are being trialed. Ultimately, the biologic eligible share will never go away, but may be meaningfully shrunk by Ohtuvayre and other inhaled therapy (potentially including inhaled biologics). The market is still *very enormous*,  underpenetrated by biologics, and without more sophisticated biomarkers so still a very strong reason to develop new drugs. 

### Anti-synthetase syndrome 

This is a rare condition characterized by autoantibodies against tRNA synthetase antigens, the most common of which is Jo-1. Prognosis is pretty bad -- in the range of 70-80% over 10 years. This is in large part due to the commonly arising ILD. Inflammatory myopathy, arthralgias, and Raynaud's are other common symptoms. Treatments include high dose steroids, B cell depletion, and anti-fibrotics or other treatments for dealing with the ILD. 

Anti-synthetase syndrome is something that seems like a solvable academic problem. Figure out the significance of the tRNA synthetase antigens. Potentially design a therapy to compensate for lack of endogenous tRNA synthetase. Alternatively, if an academic physician wants to run an immune reset trial with TCEs, perhaps one could cure this disease by eliminating B cells secreting these autoantibodies.

## Nephrology & Glomerular Disease

Kidney diseases have become somewhat boring in that everyone has woken up to B cell inhibition or depletion strategies. FcRn and antibody degrading strategies are cute but the big commercial (and clinical) stories for the next several years are going to be anti-APRIL/BAFF, BTK, and depleting approaches like CD19/20/BCMA/CD38, in a TCE/naked antibody/cell therapy (hopefully LNP based vs auto/allo; Capstan Therapeutics) format. Some people may make money betting on the optimal therapeutic format.

Meanwhile, endothelin receptor antagonists and complement blockers compete for commercial share and utilization in patients with more moderate disease. Each of these indications offer an interesting case study on clinical trial positioning and commercial dynamics. With attractive markets but many competitive approved options, patients will have a much better outlook than just a few years ago.

### Minimal Change Disease (MCD)

This is an interesting nephrotic syndrome that is highly prevalent in both children and adults that surprisingly has minimal change in tissue organization on light microscopy (hence the name). 

Most patients respond to steroids and/or B cell depletion in the form of vitamin R (Rituximab). BTK and other forms of B cell depletion are certainly in the pipeline as Rituximab isn't perfect. 

### Membranous Nephropathy (MN)

The pathophysiology of membranous nephropathy is better understood than minimal change disease. There are well defined autoantibodies against podocyte antigens including PLA2R and THSD7A, which form immune complexes on the glomerular basement membrane. These complexes activate complement and damage podocytes, causing nephrotic syndrome. 

BTK inhibition and various mechanisms of B cell inhibition/depletion (CD20, CD38, others I'm sure) are working in MN and in many institutions are first line. 

Obinutuzumab, a 'next generation' CD20 antibody with an afucosylated Fc (enhanced ADCC) and a type II CD20 epitope which reduced internalization, has posted impressive data in MN, lupus, and other indications.

Felzartamab was the primary asset in Biogen's acquisition of HI-Bio and is being trialed in MN with early signs of efficacy despite high injection site reactions.

### IgA Nephropathy (IgAN)

IgAN has seen the most biotech activity in nephrology over the past 5 years. There is a large biopsy proven population (~160k) in the U.S., and more in other countries where screening is more aggressive. Average age at diagnosis is in one's 30s and this disease is currently seen as incurable so decades of therapy is possible. Many branded drugs will be entering the market at the same time, including a powerhouse portfolio from Novartis (Fabhalta; oral complement inhibitor, Vanrafia; endothelin receptor antagonist, and the not yet approved zigakibart, an anti-APRIL monoclonal antibody). Tarpeyo, a locally acting budesonide and Filspari, another dual endothelin receptor antagonist have also been approved within the last 5 years. Many patients are on additional medication, such as SGLT2s. Safety and the ability to stack in combinations could drive commercial uptake.

In biotech land, we have Povetacicept and Sibeprenlimab as the two leading B cell inhibitors. Both will have monthly dosing and preserve or even improve eGFR. Investors were very excited about Biohaven's IgA degrader but I'm not sure there is reason to be anymore.

Atacicept from Vera (and the lack of enhanced efficacy vs anti-APRIL alone) has shown us that perhaps APRIL alone is just as good as dual APRIL/BAFF inhibition. Jade's presumably ultra long half life APRIL antibody will be another great test of this. Overall, it is incredibly crowded (why is VOR a thing? the AUPH TACI-fc looks similar to povetacicept but atacicept and telitacicept simply look inferior). Trials may get harder to run (ie. more expensive recruitment, higher placebo variability; similar to AD) once anti-APRIL drugs get commercialized.

### Lupus Nephritis (LN)

Lupus nephritis is by several metrics one of the 'nastiest' kidney diseases you can get. Near the end stage of SLE, not only do you present with the typical symptoms of rash, edema, fatigue, etc., but with LN you have a build up of immune complexes in the kidney mesangium. With the triad of complement activation, fibrosis, and local inflammation, the progression to end stage renal disease can happen quite quickly.

There are ~160k patients in the U.S. who are currently managed with a smattering of cyclosporine analogues ($AUPH), Rituximab, steroids, MMF, and clinical trials. Lupus patients have been the benefactor of several successful CAR-T studies (e.g. Kyverna; totaling 91 patients). BTK inhibition is starting to be proven out in pivotal clinical trials as well. Do patients here need CAR-T, or will TCEs suffice? Maybe this is somewhere where allo thrives. How much of the success of CAR-T is CyFlu versus T cell mediated killing? Due to its relative severity, LN could certainly be the indication where the I&I CAR-T thesis actually ends up being successful. We'll get our answer in ~5 years.

### Chronic Kidney Disease (CKD)

Lastly, chronic kidney disease is the largest segment, affecting 1 in 7 adults. The reason for this staggeringly high number is really that CKD captures a largely asymptomatic patient population. The definition of CKD is eGFR < 60 or urine albumin/creatine >= 30. Normal eGFR is 90 and normal urine albumin/creatine is < 30. eGFR drops by 1 each year after age 40 so say you live until age 70, you basically are guaranteed to have CKD. However, you don't really have any symptoms until eGFR is ~20-30 so 9 in 10 adults with CKD are unaware. CKD is often comorbid with heart disease and diabetes as well.

Most patients with CKD get managed on some combination of RAS / SGLT2 / MRA. Not super interesting from a biotech perspective as management is really just 'art of medicine'. Make sure your patients take meds, control their weight, and manage their aging process.

There are a couple interesting problems in the CKD space:

1. It is irreversible; we never regrow nephrons. Is there a role for cell therapy here to provide patients with end stage renal disease a new lease on life? Or is transplant (human or other genetically modified animals) the only way to go?
2. There are genetic subsets (and likely other biomarker defined populations). For example, certain APOL1 variants confer genetic for kidney disease, and Vertex has developed approaches to inhibit active APOL1
3. CKD can be exacerbated by fibrosis and inflammation. We can wonder about the IL-11 class and whether CKD fibrosis can be reversed.

## Hematology & Immuno-hematology

### Immune Thrombocytopenic Purpura (ITP)

Purpura are typically rounded collections of extravascular blood found in the skin. An immune thrombocytopenic purpura refers to a condition where autoimmunity against platelets causes reduced platelet counts (thrombocytopenia) and bleeding (purpura). There are on the order of 50k patients, split roughly 60/40 adults to children. 

First line treatment is either a short course of steroids or IVIg can stabilize disease, but most patients recur. In the second line, TPO-receptor agonists, which increase platelet production, provide patients responses without immunosuppressants, but also have a significant recurrence rate -- only ~25% are treatment free. Rituximab provides a roughly ~20-25% cure rate as well, but splenectomy has the largest benefit, curing 60-70% of patients. 

FcRn inhibitors are now approved, which enable platelet counts to rise within a week. Rilzabrutinib, Sanofi's BTK inhibitor, also has a positive Ph3 and may start being used in earlier lines. Overall, patients are doing quite well, with very low mortality outside the rare patients with persistently low counts and brain bleeds.

### Thrombotic Thrombocytopenic Purpura (TTP)

This is a very interesting condition driven by lack of functional activity of the von-Willebrand-factor–cleaving protease (ADAMTS13). This protease cleaves VWF (as advertised) which is involved in the early stages of clot formation by helping platelets aggregate. If you don't have ADAMTS13, you get a bunch of microthrombi, because nothing is breaking down clots. There is a congenital form (cTTP) from mutations in the ADAMTS13 gene (10% of cases), and an immune acquired (iTTP) form (90% of cases) where you get autoantibodies against ADAMTS13. If untreated, basically everyone dies, and even with therapy 10-15% of patients still die (mostly from thromboses).

For iTTP, treatment is daily plasma exchange, high dose steroids, and an antibody fragment called Caplacizumab which inhibits the VWF/platelet interaction. Sometimes patients get Rituximab as well, and some are interested in trialing FcRn inhibition. Recombinant ADAMTS13 was approved just in 2023 for congenital TTP, and works quite well. It is dosed Q1/2W as an IV infusion. Probably an opportunity for half life extended subQ dosing? 

Long term, patients with iTTP still have issues even if in remission. During periods of high VWF, there can still be overwhelming production of microthrombi that damages the heart and the brain. Long term cognitive and mood issues as well as cardiovascular mortality commonly affect former TTP patients. In order to limit this as much as possible, recombinant ADAMTS13 will eventually be used in the maintenance setting in iTTP.

### Autoimmune hemolytic anemia (AIHA)

AIHA (a subset of Evans' syndrome) is a rare (1-3 pts / 100k) autoimmune disorder where autoantibodies bind and activate the complement pathway against red blood cells (interestingly, the majority of hemolysis happens in the spleen). Warm AIHA makes up the majority of cases (70-80%), and is IgG driven, whereas cold AIHA (described below) is typically IgM driven. It is quite serious, and ~10% of people die, commonly due to thromboses, infection, and anemia.

High dose steroids are currently first line, though may not be for long, as most patients relapse. Rituximab is commonly used and with the increasing use of more aggressive B cell depletion mechanisms such as CAR-T and T cell engagers. One example is this case report of a [BCMA targeted T cell engager](https://www.nejm.org/doi/full/10.1056/NEJMc2502297?af=R&rss=currentIssue) which was successfully used in two cases that relapsed on CD19 CAR-T. Immune reset to the rescue once again. 

### Cold Agglutinin Disease (CAD)

When it is cold, CAD patients get aggregation of certain cold sensitive antibodies (often IgM) that crosslink red blood cells and lead to autoimmune hemolytic anemia (above) via activation of the classic complement pathway. It is rare (affecting less than 10k in the U.S.), but this is a chronic disease so there is certainly a market.

Sutimlimab, a C1s antibody that is given at a massive 6.5 or 7.5 ___gram___ dose every two weeks I.V., is effective. This drug was sold by Sanofi for \$825 million to Recordati, an Italian pharmaceutical developer. However, I don't think anyone is happy with this dosing schedule and we can certainly do better here. Dianthus Therapeutics (\$DNTH) is trading at a \$524 mn market cap for a 60 day half-life C1s antibody. 

In addition to inhibiting the complement pathway, B cell depletion can also be effective. Around half of CAD cases are due to a clonal lymphoproliferative disorder, sometimes even just overt B cell lymphoma or Waldenstrom's macroglobulinemia. 

### Antiphospholipid syndrome (APS)

As advertised this is an autoimmune syndrome characterized by autoantibodies against phospholipid complexes. These autoantibodies cause coagulation of immune complexes and thromboses that cause DVTs, stroke, PE, etc. For pregnant women, these complexes significantly reduce birth rates.

1-5% of the population can test positive for antiphospholipid antibodies, but the clinical syndrome is only present in 40-50/100k, and more commonly if the patient has SLE as a comorbidity. Most patients are well managed with anticoagulants like warfarin or aspirin. Some patients have what is called "catastrophic" APS, with significant (30%) mortality. While extremely rare, on the order of a few hundred cases annually, these patients are managed with more typical immunosuppressants like IVIg, steroids, complement inhibitors, and B cell depletion.

### IgM mediated disorders

There are a set of rare disorders where abundant IgM protein causes a set of common clinical symptoms. Structurally, IgM is pentameric and larger (970 kDa) than the more common IgG (150 kDa). The larger size makes aggregation and complement activation easier and also can make plasma/blood more viscous and easier to precipitate. These biophysical properties can lead to peripheral neuropathy, renal and vascular disease, and hemolytic disorders. Hyperviscosity leads to vision changes, headache, and nosebleeds.

Collectively, there may be 20-25k patients, whereas each individual disorder may be more rare. IgM mediated disorders are commonly a symptom of MGUS, or specifically Waldenstrom's macroglobulinemia, which is a clonal IgM B-cell disorder. Broad B-cell depletion/inhibition strategies are effective, as well as complement inhibition. Specific extracellular protein degradation strategies targeting IgM in theory sound attractive but IgM already has a short half-life (is not recycled via FcRn) and thus it may make more sense to turn off the faucet rather than trying to clear what is already there.

### VEXAS syndrome

Super interesting disease which was only just discovered in 2020 from whole genome sequencing many patients with unexplainable fevers and inflammation. 

The pathophysiology is based on somatic mutations, specifically in the myeloid lineage, in the gene UBA1, which initiates the ubiquitination cascade. Cells with defective ubiquitination activate the unfolded protein response (UPR) and upregulate inflammatory pathways. For reasons not entirely clear to me, these cells have a survival advantage and grow to form a significant clonal population amongst myeloid progenitors.

This is a serious disease. 5-year mortality rate of 18-40% according to some [cohorts](https://pubmed.ncbi.nlm.nih.gov/39470174/). Fevers, relapsing polychondritis, and cytopenias are amongst the symptoms. Clinical management thus far is high dose corticosteroids, which does not have sustained efficacy in all patients and is also associated with the expected toxicities. JAK and IL-6 targeted therapies are effective in subsets of patients. Patients in theory can be cured with HSCT. 

David Beck, a rheumatologist physician scientist at NYU, is the co-discoverer of this syndrome and made the discovery as a fellow at the NIH. His lab is more or less dedicated to studying this disease. Some interesting work they have done suggests that small molecule inhibitors targeting the unfolded protein response (e.g. IRE1a) may be effective at addressing UBA1 induced inflammation. 

### Hemochromatosis

This is a disease of pathogenic iron overload. This is most commonly due to genetics: recessive carriers of mutations in the gene HFE cause 90% of cases. I remember the first day of pathology lab they showed us a dark red liver from a patient donor. Patients get iron deposition in the liver, heart, pancreas, joints, and skin, causing all sorts of pathology, including liver cirrhosis and hepatocellular carcinoma.

The major effective treatment is weekly phlebotomy, though iron chelating medications can also slow iron deposition (though less effective than phlebotomy and can be toxic). Disk Medicine has a TMPRSS6 antibody (indicated for Polycythemia Vera) that can increase hepcidin and thus reduce iron absorption. While a weekly phlebotomy may not be the most palatable thing to do for the rest of one's life, the blood can be used so in theory you are helping many people. Still, perhaps there are mechanisms of correcting HFE mutations that would benefit patient quality of life significantly.

## Neuro-Immunology

### Multiple Sclerosis (MS)

Multiple sclerosis is a CNS compartment autoreactive disorder against myelin. It occurs most often in women, with peak onset between 20-40 years old. Nearly 1 million people in the U.S. have it. Recent evidence that a subset of patients may have it because of prior Epstein Barr virus infection. Apparently there are viral epitopes that are similar to autoreactive epitopes in MS patients.

MS is a mature indication where the landscape of approved therapies is diverse with both breadth and depth. There are 23 approved therapies spanning 8 distinct disease modifying mechanisms. The most efficacious seem to be BTK / B cell depletion (CD20), S1P inhibition, and inhibition of T cell trafficking (natalizumab). Autologous hematopoietic stem cell transplant has also been used with good outcomes. 

There are two major phenotypes: relapsing-remitting (RRMS) and primary-progressive (PPMS). RRMS is much more common (85% of patients) and is characterized by cyclical periods of acute attacks, followed by improvement, and recurrent attacks. PPMS in contrast is a more sustained and gradual worsening. The life expectancy gap continues to narrow, but patients still do not have disease reversing therapy. Perhaps in the future, we can see combinations of remyelinating therapy (which was not effective as a monotherapy) in combination with immunomodulatory therapy. Maybe we see something with vidofludimus calcium (\$IMUX; readout end of 2026). 

### Neuromyelitis optica (NMOSD)

Autoantibodies attack the optic nerve and spinal cord by binding aquaporin-4 on astrocytes. This causes complement dependent cytotoxicity and demyelination. Median onset is late 30s early 40s, and the global addressable pool is 200k patients. 

There are three approved drugs: Satralizumab, an IL-6R sweeping antibody, Eculizumab, a C5 complement inhibitor, and Inebilizumab, a CD19 antibody for depleting B cells. Patients generally have good outcomes on these drugs. Inebilizumab in particular is associated with long term disease control.

### Myasthenia Gravis (MG)

Much has already been written and discussed about myasthenia gravis. It is the spawning ground of the FcRn class, and a source of much debate around the relative merit of B cell versus autoantibody depletion. Myasthenia gravis involves autoimmunity at the neuromuscular junction, leading to characteristic weakness in skeletal muscle. There are two categories of MG, depending on the type of autoantibodies that develop. Acetylcholine receptor (AChR+) MG is the vastly more common form, and muscle specific kinase (MuSK+) MG is a more severe B cell depletion responsive variant.

In the first line, pyridostigmine, an acetylcholinesterase inhibitor) is effective for controlling symptoms of MG, like droopy eyelids. If symptoms worsen, patients get broad immunosuppressants such as steroids, azathioprine, mycophenolate mofetil, and cyclosporine. Biologics are used in refractory MG (for patients not responsive to 2 or more immunosuppressants)

Efgartigimod, the first approved FcRn inhibitor, has had rapid uptake and sales growth in MG. Complement inhibition downstream of autoantibody binding is also quite effective, especially in AChR+ MG. Finally, B cell depletion approaches including CAAR-T, CD19/CD20/BCMA TCEs or depleting antibodies, have all demonstrated efficacy. Chalk up MG as another indication where immune reset via B cell depletion is a winner. 

### Chronic Inflammatory Demyelinating Polyneuropathy (CIDP)

CIDP is a rare disease affecting on the order of tens of thousands of patients in the U.S.. The disease mechanism involves autoreactivity against myelin on peripheral nerves, which can lead to muscle weakness, loss of perception, and functional deficiencies.

First line therapy is still IVIg, steroids, or plasmapheresis. Second line therapy is also pretty inspiring: azathioprine, mycophenolate mofetil, cyclophosphamide, and sometimes Rituximab.

FcRn inhibition (efgartigimod) in theory is also approved in the second line, but in the real world some have [raised questions](https://pubmed.ncbi.nlm.nih.gov/39578164/) about transitioning patients from an efficacious therapy like IVIg in the first line, into FcRn inhibition (as obviously IVIg + FcRn inhibition concurrently doesn't make a lot of sense. It seems that some patients rapidly deteriorate during the switching period. Sanofi is also running a C1s inhibitor Phase III trial with primary readout in q425, and final efficacy in 2027. 

## Endocrine & Exocrine Autoimmune

### Graves Disease 

Graves disease is caused by autoantibodies that agonize TSHR, inducing hyperthyroidism. A hyper-active thyroid causes weight loss, heat intolerance, tremor, and often thyroid eye disease (see above). Treatment includes thyroid antagonism, via iodine or methimazole, but this is often ineffective. 330k patients have failed all therapeutic options other than surgical removal of thyroid. This is undesirable for many reasons, and as a result there is significant need for disease modifying therapy.

IGF-1R modulating antibodies can work (and are the only FDA approved biologic) because IGF-1R and TSHR exist in a complex and allosteric modulation of IGF-1R can inhibit autoantibodies from agonizing TSHR. Immunovant is running large trials for their FcRn antagonist, with the idea that depletion of pathogenic autoantibodies may help. Their 1st generation compound batoclimab, worked in a Phase 2a (60-70% response rate), and are trialing a 'next generation' version IMVT-1402 currently in a Ph2b. Because FcRns work, Graves should in theory be addressable with IgG degraders (enzymes or TPD) or B cell depletion. Rituximab works off label (~50% response rate), but more potent depletion mechanisms may prove to work even better.

### IgG4 Related Disease (IgG4-RD)

IgG4-RD is a nasty disease with a broad range of clinical presentations depending on the affected organ. B cell class switching to IgG4 leads to abundant production and tissue deposition. The antigen is not yet known, but common sites include the pancreas/biliary tract, kidney, lungs, small vessels, and salivary/lacrimal glands. There are interesting histologic patterns including dense infiltration of lymphocytes, "storiform" fibrosis (a sort of swirly pattern), and obliterative phlebitis (blockage of vessels due to immune infiltrate). High dose steroids continuously dosed over long time horizons have been standard of care and have high cumulative toxicity.

However, Amgen's CD19 antibody Uplizna has made major progress in treating IgG4-RD. 42% of patients go into histologic remission at 1 year (likely deepens over time), with 87% flare reduction. Short of any other safe strategy of depleting B cells, I think the market here is saturated, at least until there are reliable reports of patients relapsing off of Uplizna. A very interesting mystery to study how this works though. Would love to do spatial proteomics/transcriptomics on some of these lesions.

### Primary Sjogren's Syndrome (SS)

Sjogren's syndrome is characterized by dry eyes and dry mouth, caused by autoimmunity against salivary and lacrimal glands. The disease mostly occurs in older women, and up to 1% of the U.S. population may develop Sjrogen's in their lifetime. It is often secondary to SLE, and there are similarities in pathophysiology. For example, pDCs and interferon, Th17 inflammation, and B cell activity are shared disease mechanisms. While there are no FDA approved biologics yet, B cell targeting agents, such as BAFF receptor blocking monoclonal antibodies, have shown proof of concept in clinical trials.

GWAS hits include TYK2, IFN, IL12A, and IRF5. Looking forward to trials of small molecules targeting TYK2 and IRF5. There is also probably room to trial bispecifics here. Zura's IL-17/BAFF bispecific tibulizumab probably works here. I'm sure a BDCA2/IL-17 or BDCA2/BAFF might work as well. 

# Concluding Remarks

Does all this sound complicated? Do you trust an LLM to digest this information and your prompting ability to optimally pull out insights?

Expertise is still worth something. The most exciting position of the next 20 years, in a world where everything is druggable with whatever pharmacology you want, will be director of biology. Make sure you hire a good one.

1. ___Reducing steroid toxicity___ is a major goal of basically every later line therapy. There are lots of parallels to oncology drug development, where steroids are this blunt chemo-analogous instrument, which are slowly becoming replaced by targeted therapy. In some cases improved disease understanding can allow you to get deeper remission by improving the therapeutic window. A really interesting approach being pioneered by Lifordi is the steroid ADC. 

2. Sort of interesting that ___modulating macrophages just doesn't work___. There are mechanisms for targeting T cells (abatacept/MMF/azathioprine/integrin class), B cells BTK/APRIL/BAFF/depletion, etc), eosinophils (IL-5), mast cells (KIT), pDCs (BDCA2), neutrophils (DPP1), and even neurons (IL-31R). Macrophages are like water. Always necessary, and takes the shape of whatever is happening locally. 

3. ___Immune reset with B cell depletion / inhibition is incredible___. In nearly every organ system, there is an autoimmune disorder driven by autoantibodies which is addressable by B cell depletion or inhibition. The fact that you can get *curative efficacy* in just a few doses of antibody, TCE, or cell therapy is very encouraging. It suggests that even in ostensibly unhealthy patients, homeostasis is still king. The generation and progression from autoantibodies into autoimmunity is stochastic and certainly not deterministic. It is reassuring that this 'bad luck' can be reversed.

4. ___Indication expansion___ is the name of the game. The IL-6 class is a prototypical example where it is approved in RA, GCA, acute settings (e.g. CRS, COVID-19), NMOSD, SSc-ILD, and perhaps soon in cardiovascular disease. IL-13 went into AD, and now is in EoE, CRSwNP, asthma, COPD, PN, and CSU. The IL-17/23 class started in psoriasis and now is in psoriatic arthritis, IBD, AxPsA, HS, relapsing polychondritis, and maybe in PV. So on and so forth. What does this mean for new medicines? Never underestimate the size of the market. B cell depletion/inhibition, IL-1, Kit, TL1A, as well as speculative new mechanisms such as IL-11 and IL-15/CD122 (if they hit), can all become blockbusters. No where else is the value of a positive Ph2 trial is higher.

***

The next post will be about exploiting the limited whitespace that is left for new therapeutic development. We now know the targets, and soon we will design the medicines to match. Thanks for reading.
