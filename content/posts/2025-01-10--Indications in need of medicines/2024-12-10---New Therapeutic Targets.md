---
title: "How to find new targets"
date: "2024-11-16T12:00:00.000Z"
template: "post"
draft: True
slug: "/blog/newtargets/"
category: "Life Sciences"
tags:
  - "Life sciences"
  - "Healthcare"
description: "and what to do about them"
---

One of the most common tasks for the life sciences consultant is to perform an exercise called 'target identification and indication selection'. The client has typically developed a platform technology that has the potential to be applied across a wide range of therapeutic areas. For example, you may encounter a discover platform to discover RNA targeting small molecules, or a screening platform for so-called catalytic antibodies that can degrade extracellular proteins. The consultant's job is to decide which nails to hit first. 

Finding targets is the best example of "artisinal alpha" that is difficult to automate with artificial intelligence. Its a multimodal task with a low rate of success, and when there is success, a lot of redundancy (me-too targets). There is always going to be an information limit with regard to competitive intelligence. It is impossible to know and be up to date with everything (including non-public information), while simultaneously knowing who to trust and who not to trust.

While doing this exercise, one question has consistently bothered me. Understanding competitive differentiation or what to believe from industry or academic publications is important and can help narrow in on a candidate. But I think the most impressive and high leverage thing a biologist can do is to have the spine to go after unknown mechanims that are uniquely enabled by the platform. Why does everyone go after the same handful of targets for the same handful of large indications? There are roughly 20k genes in the human genome, and only a fraction are currently actionable or currently drugged. Depending on the classification system, there are thousands of indications, very few of them have effective therapies. 

The first part of this issue, that only a fraction of the genome is druggable, is being solved by advancements in chemistry and AI. For example, transcription factors which have long been appreciated to be bonafide drivers of cancer, are only now druggable with technologies like molecular glues or PROTACs. Other difficult to ligand oncoproteins like KRAS and VAV1 are also newly druggable. Technology is no longer rate limiting.

__Now, it is the biologist's turn to contribute.__ No longer can we complain that there aren't tool compounds, that its too labor intensive to develop antibodies, or that we don't have sensitive measurement technologies. There are only 20,000 genes, that need to be matched to just a few thousand diseases. Most genes can be ruled out as drug targets very easily with common sense (e.g. can't be drugging essential proteins outside of oncology). We could have very easily had millions of targetable proteins across millions of potential diseases.

## Why care about targets?

It is a good question given the comparably better success of phenotypic screening vs target based drug discovery. But starting with targets has several important benefits:

1. _Being able to better predict toxicity._ If you know what your molecule targets, you can start to understand where the toxicity is coming from (e.g. is it on target or off target), whether there are toxicity/efficacy tradeoffs, or which parts of the molecule can be engineered to avoid the toxicity.

2. _Being able to run optimization on a target_ (making it easier to explore chemical space). If you know the target, then you can know its structure. With a structure, you can optimize binding. Modeling binding to a target is generally easier (due to physics based modeling) than trying to predict efficacy on a biological endpoint (which is likely also more expensive).

3. _Being able to rationally design combinations._ If you understand the target, you can do biomarker studies on patients and understand resistance mechanisms and efficacy biomarkers. This could help you pick how to combine certain targets (e.g. EGFR antibody + BRAF inhibitor in CRC due to pathway reactivation). On the other hand, Adam Palmer has taught us that synergy is rare and really all we should be doing is combining two drugs that both have efficacy which in theory you could do just with phenotypic screening. However, I think that we will one day be able to design rational synergistic regimens or at the very least have biomarkers (which are harder to find if you use a phenotypic approach). 

From a practical point of view, targets are also becoming the most scarce resource in biotech. Chemistry and engineering are going to be commoditized by AI. There will be innovation around the edges like half life or delivery mechanisms, or developing more complicated products (e.g. glucose responsive insulin, CAR-T). But I would argue that these are all secondary to picking the right mechanism. Target selection cannot really be commoditized (unless working in the 'best in class' space) because it relies on clinical development -- you can't really commoditize clinical trials since its people's lives.

Picking a target is being __'directionally correct'__ as Peter Thiel would say, in the context of uncertainty.

## How are targets discovered today?

Target discovery is all -omics. The complexity comes in where to apply it. I think that there are 3 layers of omics, which I'll term primary, secondary, and tertiary. These relate to how directly connected the discovery was to an -omics readout.

1. Primary Omics 

The most common method of target discovery has been genomic sequencing of diseased samples and comparing mutations versus ostensibly normal tissue. This applies both on the population level (ie. GWAS), but also on the individual level (tumor vs normal tissue analysis). 

Historically, these targets not only have a [high success rate](https://www.nature.com/articles/s41586-024-07316-0) in clinical trials, but they are also just low hanging fruit. A mutated gene is highly likely to be contributing to pathology and by understanding the downstream effects of loss of function or gain of function mutations, one can rationally design a therapy. Alternatively, the absence of mutations in a healthy population protected from pathology can also be used to nominate targets. For example, PCSK9 loss of function mutations are protective for hypercholesterolemia and as a result PCSK9 therapeutic antibodies have been developed.

Analysis of the transcriptome or proteome can also be useful particularly in cancer. Cell surface targeted drugs like therapeutic antibodies or CAR-T benefit from large cohort staining or RNAseq experiments to identify tumor associated antigens.

For more complicated targets like cytokines, RNAseq has also been used to identify increased expression in diseased lesions. 

2. Secondary Omics

Secondary to the simple approach of analyzing diseased tissue is deriving targets from phenotype. "Phenotypic screening" goes beyond the simplicity of screening libraries of small molecules on cell lines and looking for signs of disease reversal. This category also includes CRISPR screens, cell line libraries, and other methods of 'brute forcing' target discovery.

These approaches have had a history of success, with many drugs being approved solely from the results of a phenotypic screening approach. Indeed, many drugs don't even have a solid understanding of the target (e.g. aspirin, acetaminophen, etc). 

Pioneered in cancer but certainly expanding to other indications, CRISPR screens are not frequently used to identify gene targets capable of inducing a phenotype. For cancer, the readout is typically loss in proliferative capacity, but there are many other creative ways to design screening endpoints. In vivo screens have identified new cancer immunotherapy targets like [Ptpn2](https://www.nature.com/articles/nature23270).

3. Tertiary Omics

Finally, tertiary -omics is what I refer to as 'artisinal alpha'. These are the targets which require new model systems or new techniques to uncover. These are hypothesis driven and are much more difficult to brute force. Maybe a metabolic pathway had to be figured out first. Maybe we needed to understand how the immune system worked before understanding that cells instead of specific proteins can be pathogenic. Tertiary omics targets have historically led to giant breakthroughs, and many of the best selling and most impactful drugs are not from brute force approaches (PD1 antibodies, steroids, statins, Dupixent, anti-cytokine drugs in general, Advair, GLP1s, etc.)

Beyond background knowledge, tertiary omics targets often require new discovery formats. For example, many immunotherapy targets including PD1, LAG3, and CTLA-4 were discovered in reductionist T cell activation and exhaustion models, sometimes involving transgenic OT1 mice. Inventing this system was crucial to discovering these molecules and their functions. Another example is the discovery of IL-11. This came in an RNAseq assay simply measuring the transcriptional output of treatment with TGFb. The critical insight was understanding that TGFb itself may not been druggable, but its effector proteins may be, and now there is an emerging story of IL-11 inhibition in fibrotic diseases. Similar tricks can be used for other pathogenic secreted proteins (e.g. STAT6 inhibition in type 2 autoimmunity driven conditions).

Mouse models are often a critical aspect of untangling the biology behind teriary omics targets. While these certainly can be brute forced (e.g. the work of the [IMPC](https://www.mousephenotype.org/) to create KO mouse strains for every single gene), making organ or cell type specific knockouts is probably not going to happen. Thus, building mouse models in a hypothesis driven format requires a degree of artisinal decision making. Tissue specific gene knockout mouse models have been critical for verifying phenotypes, especially for pathogenic secreted proteins like cytokines, and are also useful as gold standard preclinical models for testing new therapeutic agents.

You can also get lucky by identifying off target effects of selective inhibitors of a certain target. This is a form of backwards phenotypic screening which requires an astute scientist to notice and followup on clinical observations.

## The topic of today

Here, we will review 75 drug targets from the past 6 years of drug approvals (from NRDD's new targets series), and describe how each target was discovered. 

As promised, I have reviewed new therapeutic targets from NRDD's new targets series (e.g. the [most recent](https://www.nature.com/articles/d41573-024-00057-9) from earlier this year)



Average of 20 years between discovery and approval of a therapeutic. 

![approval gap](approval_gap.jpg "approval gap")


Antibody drug conjugates (enfortumab vedotin)
siRNAs




