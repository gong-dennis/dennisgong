---
title: "Fantastic Papers and Where to Find Them"
date: "2021-05-20T12:00:00.000Z"
template: "post"
draft: False
slug: "/blog/Fantastic/"
category: "Life Sciences"
tags:
  - "Life Sciences"
  - "Healthcare"
description: "Recent papers + a repository"
---

Tis the season for some of the biggest academic conferences in the life sciences. AACR was early April, this week we had ASGCT, and in a few weeks we will have ASCO at the beginning of June. Already, there have been some incredible results released, ranging from [curing 50 out of 50 children with adenosine deaminase deficiency](https://www.nejm.org/doi/full/10.1056/NEJMoa2027675) to preclinical data showing [500% improvement in editing efficiency for Beam's lead liver candidate](https://www.globenewswire.com/news-release/2021/05/11/2226966/0/en/Beam-Therapeutics-Presents-LNP-Formulation-Data-at-ASGCT-and-Reports-First-Quarter-2021-Financial-Results.html). Unfortunately I don't have memberships to any of these societies and I can't really pay entrance fees so there are probably just the headlines that made my Twitter timeline. However, this was also quite an amazing week in general for papers in Nature.

We had [confirmation that immune aging drives senescence and aging of solid organs](https://www.nature.com/articles/s41586-021-03547-7). Key experiments included demonstration that premature onset of immunosenescent immune cells was associated with increased organ senescence and damage, and importantly that this happened even in a healthy mouse if senescent immune cells were transplanted. Additional experiments showed that transplantation of healthy (young) immune cells ameliorated organ level senescence and that treatment of immune cells with rapamycin reduced immune senescence. This study is big for a couple of reasons, principally because it confirms my priors that the immune system is a master regulator of disease :). A lot of aging papers I have come across are really focused on molecular mechanisms or epigenetics which can be interesting, but is less familiar to me how they can be translated to therapeutic strategies. Our experience in liquid cancers for example have shown that targeted small molecules can be powerful for some small patient subgroups, but cell therapy has made a great case for itself as a strategy that works more broadly. I'm not sure if we need a cell therapy for senescent cells, but immunomodulatory strategies should hopefully begin to gain prominence (for ex. figuring out if there are certain senescent subpopulations, what causes immune senescence on an epigenetic level, possibilities for immunomodulatory biomaterials to reprogram out senescence, etc.)

Another really [awesome paper](https://www.nature.com/articles/s41586-021-03512-4) that came out recently was from a former professor of mine, Faisal Mahmood, and led by a former student, Max Lu, from the same departments as me at Hopkins! This paper addresses a key problem in clinical care of mestastatic cancer, namely where the origin of metastasis is. It turns out that cancers from different tissues behave differently and respond differently to treatment. Patients with cancers of unknown primary (CUP) thus have lower survival odds as they lose out on more targeted therapies and typically get generic chemotherapy regimens. As a result, a variety of clinical tests have been developed based mostly on IHC, but also other molecular diagnostics to help clinicians understand where the cancer came from. Amazingly, using just the patient's sex and a histology slide, Lu and colleagues were able to predict origin of difficult metastases (ie. those that required multiple histological and clinical workups) at 60%, 82%, and 92% for top 1, 3, and 5 predictions respectively. This is potentially a game changer not only for places where advanced workups can't be done, or to help clinicians be more targeted in the workups that they order. There is so much data in an image and modern algorithms have gotten very good at decoding them. We should take pictures of all the things.

Very outside of my knowledge base, but researchers [published yesterday](https://www.nature.com/articles/s41586-021-03486-3) a battery technology that keeps 80% capacity with 10,000 charge drain cycles, with >2.5 the specific energy as the latest iPhone battery. The specific numbers cited were a specific power of 110.6 kw/kg and specific energy of 631.1 wh/kg. In comparison, the latest iPhone tops out at roughly 250 wh/kg and Tesla batteries top out in the 260 wh/kg range. The structure of the battery is a multilayer design that has the structure of a less-stable electrolyte sandwiched between more-stable solid electrolytes. While the current battery is made of lithium metal, the authors highlight that different materials could potentially be used in the multilayer structure.

Finally, the most mind blowing advance from this week (all of the papers were from this past week, how crazy is that btw) is a [brain-to-text communication device](https://www.nature.com/articles/s41586-021-03506-2). Here we have an intracortical BCI (microelectrode arrays in the hand ‘knob’ area of the precentral gyrus (a premotor area)), with signal decoded by a recurrent neural network and translated into text in real time. Amazingly, just 'thinking' of handwriting gives you a speed of 90 characters per minute at 99% accuracy with autocorrect (94% without autocorrect). This is pretty close to the typical smartphone typing speed of 115 characters per minute, and I don't know, but this seems maybe even faster than what I could write on a piece of paper myself. This was a tetraplegic individual who had written before, and the model required pre-training and had a library of vocabulary words (I think there might be a parallel to swipe to type keyboards on iPhones here), and also the computing required to decode the signal obviously requires some hardwire outside the brain with a cord. But wow amazing, amazing work.

***

Outside of these papers that showed up on Twitter, I've been reading papers from two labs that have been really exciting over the past months.

1. [James Dahlman](https://www.dahlmanlab.org/), founder of Guide Therapeutics which sold to Beam in February has assembled the largest non-viral delivery dataset using high throughput barcode screening of LNPs. Important results include demonstration of basically r = 0 correlation between in vitro and in vivo nanoparticle performance for delivery to non hepatocytes, efficient delivery to hard to transfect cell types including T cells, bone marrow, and endothelial cells in vivo, and the beginnings of an effort to characterize the biology of drug delivery. The last point is very important to enabling more intelligent design of next generation vectors and is often ignored by the chemists designing current nanoparticles, probably because it is outside their expertise.

2. [Matthias Stephen](https://stephanlab-fhcrc.squarespace.com/), founder of Tidal Therapeutics which sold to Sanofi in April does some of the best biomaterials cell therapy work in the field. Examples include developing the in-vivo PBAE delivery technology to enable in situ CAR-T or other genetic reprogramming to immune cells using mRNAs. Also amazing was work to develop nitinol films among other biomaterials for in situ delivery of cell therapy and other molecules to eliminate solid tumors. Each of these technologies deserves to be translated into startups, and what I respect a lot about his work is how thorough it is. His lab really employs the go big or go home approach and to great success.

***

## Repository for great papers:

Finally, I want to create a repository for myself to hold some of the biggest hits I've read. Currently some sit on my desktop, but most others disappear upon closing the tab and removing from OneTab. I want them more easily accessible (ie. over internet) so I don't forget about them. Key inclusion criteria here are probably whether or not I would drop out and start a company based on the technology if I invented or helped develop it (and of course almost all of these are already companies). I also mainly like gene/cell based therapeutics, biomaterials, nanotechnology, synthetic biology, drug delivery, and their intersections. Clearly a lot missing.

1. [Nitinol thin films functionalized with CAR-T cells for the treatment of solid tumours](https://www.nature.com/articles/s41551-019-0486-0#citeas). Stephan Lab. Dec 2019. Nat BME

2. [In situ programming of leukaemia-specific T cells using synthetic DNA nanocarriers](https://www.nature.com/articles/nnano.2017.57). Stephan Lab. Apr 2017. Nat Nanotech

3. [SynNotch CAR circuits enhance solid tumor recognition and promote persistent antitumor activity in mouse models](https://stm.sciencemag.org/content/13/591/eabd8836). Roybal Lab. Apr 2021. SciTM

4. [A biomaterial-based vaccine eliciting durable tumour-specific responses against acute myeloid leukaemia](https://www.nature.com/articles/s41551-019-0503-3). Mooney Lab. Jan 2020. Nat BME

5. [A divalent siRNA chemical scaffold for potent and sustained modulation of gene expression throughout the central nervous system](https://www.nature.com/articles/s41587-019-0205-0.epdf?sharing_token=P3TE4XJztLU8FNk3mUvzydRgN0jAjWel9jnR3ZoTv0O6ZfgNfj_IJbLNxU9YOZtQgry_cD_iVvDjZuB-GFJFct1xv_-JvLmyHShHEMJgk9QIhwVIXDkvAw4EKxTa_xpStZ5X0R0t3_q7vkNY_SO8lFCQnWVPz_fJatBhZsmlzXxWcmsNJkB_6dT3ZqUy1_kAVZ39SJj7-mMNOQRqzpf0FJmVa59kBDc7Z2ofgIq2chM%3D&tracking_referrer=www.biospace.com). Khvorova Lab. Aug 2019. Nat Biotech

6. [Reconstituting Organ-Level Lung Functions on a Chip](https://science.sciencemag.org/content/328/5986/1662.abstract). Ingber Lab. Jun 2010. Science

7. [Search-and-replace genome editing without double-strand breaks or donor DNA](https://www.nature.com/articles/s41586-019-1711-4;). Liu Lab. Oct 2019. Nature

8. [A system for the continuous directed evolution of biomolecules](https://www.nature.com/articles/nature09929). Liu Lab. Apr 2011. Nature

9. [De novo design of potent and selective mimics of IL-2 and IL-15](https://www.nature.com/articles/s41586-018-0830-7). Baker Lab. Jan 2019. Nature

10. [Senolytic CAR T cells reverse senescence-associated pathologies](https://www.nature.com/articles/s41586-020-2403-9). Sadelain & Lowe Labs. Jun 2020. Nature

11. [Glutamine blockade induces divergent metabolic programs to overcome tumor immune evasion](https://science.sciencemag.org/content/366/6468/1013.abstract). Powell Lab. Nov 2019. Science

12. [Genome-wide programmable transcriptional memory by CRISPR-based epigenome editing](https://www.sciencedirect.com/science/article/pii/S0092867421003536?casa_token=5VMYg8MT8TUAAAAA:sMEfwutRjkwK9EaM1CZLgF9byts-cuvXk0miqHHwIUy1zWlZ9dtJuInh7qvFOu66nWPemf8c). Weissman Lab. Apr 2021. Cell

13. [High-throughput and high-dimensional single-cell analysis of antigen-specific CD8+ T cells](https://www.nature.com/articles/s41590-021-01073-2). Jiang Lab. Nov 2021. Nat Imm

14. [Perturb-Seq: Dissecting Molecular Circuits with Scalable Single-Cell RNA Profiling of Pooled Genetic Screens](https://www.cell.com/cell/comments/S0092-8674%2816%2931610-5). Regev Lab. Dec 2016. Cell
