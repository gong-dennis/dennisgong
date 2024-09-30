---
title: "Human First Drug Discovery"
date: "2023-02-19T12:00:00.000Z"
template: "post"
draft: False
slug: "/blog/HumanDrugDiscovery/"
category: "Life Sciences"
tags:
  - "Life Sciences"
  - "Healthcare"
description: "Considerations for new target discovery and biobank construction"
---

![Targeted Therapy](archer.jpg "Targeted Therapy")

A growing suite of technologies have promised the ability to go entirely from target to drug while using only human datasets. While this is certainly an extreme position, I think it speaks to broader patterns in the industry of rewiring the drug discovery process so that humans come not just last during clinical trials, but first too as part of the discovery process.

At Regeneron, there is an obsession with focusing on genetics. They have built an entire infrastructure around identification via large genomic biobanks, knockout/in mouse libraries for validation, and expertise in target driven drug candidates (antibodies) for pushes to the clinic. More recently, this concept of drug discovery guided by human genetics has been a large motivator of Tyk2 programs at BMS and beyond, PCSK9 at Verve and others before them, and the amazing wealth of targets that the gene editing field has generated. These large biobanks are able to identify individuals that are uniquely protected from disease, allowing scientists to figure out how these protective qualities are manifested in genetics. In the opposite manner, many of us are familiar with using biobanks of cancer patients to understand the genetic drivers of disease and to design the appropriate targeted therapies for those identified drivers. 

The emergence of biobanks as a driver of discovery is a relatively new phenomena driven by rapidly falling costs of sequencing. Traditionally, the drug industry has relied upon phenotypic screening, or more favorably, targets identified through more rigorous hypothesis driven science in academia. For example, PD-1 and its impact on the immune system was discovered in the 1990s using knockout mice. Her2 and the whole RAS family was discovered as the first set of oncogenes by Rob Weinberg at MIT in 1984 by using rats as a model. These have been identified through first principles driven research, and you can similarly argue that chemo, radio, and surgical approaches to therapy are also driven by hypothetical science. Alternatively, there are targets like EGFR or chromosomal translocations that were discovered by empirical observation. Using genetic engineering tools and older sequencing technologies, certain genetic alterations were discovered to be overrepresented in very specific cancers or isolated in case studies, and steadily their significance was expanded to more and more settings. 

It will forever be a debate, the relative utility of reasoning from first principles versus learning from empirical observation, but the scales are tipping in favor of the latter, at least with what is currently in style. The power of high throughput and unbiased discovery is fantastic, but I think the reason why it is tempting is that you don't need a hypothesis to do this. You pay for the sequencing and you get your Nature paper. Pretty soon, this won't be as impressive to journals, and what will is new analysis techniques to validate findings with hypothesis driven discovery. And so the cycle continues.

***

It can be easy to criticize the boring "__Just sequence it__" approach to discovery, but there is one interesting new twist that it enables, a new drug discovery model to brute force your way to novel targets and new biology. The general idea is very simple in that all we do is generate a biobank, identify statistically robust hits, validate them in preclinical experiments, and return back into humans. Verge Genomics is a fashionable startup that did this but you could also argue that academics and large pharmas have been collaboratively doing this for decades. The difficult part, the part where we are potentially at an inflection point, is the quality of the biobank. We can collect many more -omes, at much higher fidelity. As we gain more and more statistical power, soon more modalities past GWAS will reach their inflection points and generate robust and replicable hits. 

However, there are some areas where paradoxically, the more precision we engage to measure, the harder it is to generate a high quality biobank. This happens in diseases where the underlying biology is driven by heterogeneity and stochasticity, which makes it difficult for biobanks to be representative. For example, the grandfather of biobanks in cancer is The Cancer Genome Atlas (TCGA). The issue with the TCGA is that there are biases for what kinds of tumors find their way into the database. These are primarily tumors that are resectable, which are very different from tumors that have undergone therapy and evolved in response to it. Through time, tumors evolve and this makes it very difficult to apply learnings towards patients who have gone through 10 lines of therapy already.

The utility of a biobank is only as good as how representative it is of the population you are developing therapies for, and this is especially important when you are measuring very high dimensional data. The price you pay for comprehensiveness is statistical power. How then, do you apply a biobank driven discovery approach to the setting of targeted cancer therapy? 

***

The answer is to return to the scale of the 1980s targeted therapy and paradoxically, the idea of truly personalizing the discovery. Embrace the fact that you will never create a representative biobank, and solve for this using temporal measurements on single patients. Channel mechanistic science using a controlled experiment in the n of 1 setting. 

By removing the requirement for a biobank, the model becomes: 
1. Collect temporal measurements from single patients
2. Contextualize tumor specific biomarkers
3. Validate in cell lines and preclinical models
4. Return with a patient specific perturbation 

Such a strategy raises many many questions. Where does your statistical power come from? How is it possible to collect temporal measurements? How do you generate confidence in your hits? How do you make the hits you generate actionable? 

To start, we need single cell resolution to generate move statistics to the cellular domain. By measuring what is in each cell, each statistical test becomes whether the alterations you observe cause that cell to be cancerous or not, and in concert with the temporal data, we can reduce noise and gain confidence in our signal. To make it possible to collect temporal measurements, you need a non-invasive assay, which introduces an additional requirement of not removing too much tissue. A high sensitivity _in situ_ needs to be used. For validation of these hits, we need to rely on well developed preclinical models. Many will gripe that by themselves, mouse and other preclinical models aren't adequate for modeling human systems. However, this is overblown in the sense that it is clear that they can be powerful methods of reducing variance and isolating specific variables that you can't do in a clinical setting. A powerful result in setting up robust animal models is that we pretty much guarantee that what works in humans will work in mice. We can say that animal models have high sensitivity, low specificity. So if we can find hits that we think are promising in humans, test them in mice and it works, this gives us more confidence that the hit that we found in discovery work is real.

To answer the last question is the most difficult, and potentially requires an entirely new model for cancer care. Clearly, it is possible that after steps 1-3 of our model, we can discover many new things about how tumors evolve and evade therapy. Potentially some of these may become diagnostic tests or generate hypotheses about how to progress mechanistic science. But how do we make this actionable for the patient who we are taking biopsies from? One idea is to design a clinical trial similar to Beat AML or other precision medicine trials, where we can assay your tumor and based on whatever alterations you have, we match you to a drug. This likely isn't a reality currently, but the day is coming where repurposing of off patent medicines overtakes prescription sales of branded drugs. If we have a growing armory of targeted therapies and the understanding that eventually all of these will become cheaply replicable off patent, investigator choice of targeted therapy can enable less expensive precision medicine. This is a new vision of cancer care, where we address heterogeneity head on. As tumors evolve, so can our therapy.

If any of this is interesting to you or especially if you think any of this is wrong, please shoot me an email! 
