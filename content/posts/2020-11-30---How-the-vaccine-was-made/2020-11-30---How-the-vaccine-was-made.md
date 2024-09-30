---
title: "How Moderna made the vaccine"
date: "2020-11-30T12:00:00.000Z"
template: "post"
draft: False
slug: "/blog/mRNA/"
category: "Life Sciences"
tags:
  - "Healthcare"
  - "Life Sciences"
description: "Platform vaccine development"
---

![logo](/moderna.jpg "logo")

On November 16th 2020, Moderna Therapeutics announced an interim analysis of its Phase III coronavirus vaccine, demonstrating that their mRNA based vaccine hit 94.5% efficacy in preventing coronavirus infections.

It feels cliche to say, but its the first time since the shutdowns in March that it feels like progress was being made to curb the pandemic and restore life to normal. It came 8 months after the NBA shut down on March 11th and my school sent all undergrads home. Within these 8 months, we've had an abridged NBA playoffs, an entire summer of internships, and almost an entire Fall semester online. We've also had more than 275 thousand deaths, and more than 14 million cases. While basketball, school, and the internet went on, too many lives didn't. We cannot forget what happened to our country, our world, and each and every one of our friends, family, and community members. It might feel normal now, but __this can't be the new normal__.

What is encouraging however, is the continued wonder of human innovation and resilience. The biopharmaceutical industry designed and tested a coronavirus vaccine in 8 months, and outside of celebrating this remarkable achievement, I wanted to take the time to fully digest how it was done, and how in the future we can continue to utilize technology to solve our biggest problems. This pandemic proved to me that our biggest and most meaningful problems won't be solved by policy, but rather the grind it out discovery of science.

### The mRNA-LNP

The Moderna mRNA vaccine is delivered via a saline injection into the upper arm. The mRNA is encapsulated by a lipid nanoparticle (LNP), essentially a lipid film that protects the sensitive mRNA from degradation or other interference from blood serum or enzymes. Once inside the cell, the liposome degrades and releases the mRNA into the cytosol, where it can be transcribed by ribosomes into the spike protein antigen. The liposome itself is made from a molar ratio of 50:10:38.5:1.5 (ionizable lipid:DSPC:cholesterol:PEG-lipid).

But what are we actually delivering? A high level overview is that the mRNA encodes the virus's spike protein. This is the characteristic specific to the virus that allows it to breach the cell membrane, enter, and replicate. The mRNA LNP is taken up (endocytosed) by immune cells (macrophages), which then follow the instructions encoded by the mRNA to produce the spike protein segment.

mRNA vaccines are particularly promising because they elicit both a humoral (antibody) and cellular immune response. They also have advantages in manufacturing speed. Nucleic acids are much easier to synthesize than proteins for example.

This mRNA is not exactly the same sequence as the identified spike protein. Rather, scientists built upon previous research demonstrating a modification with 2 proline (2P) substitutions at the apex of the central helix that stabilized the spike protein in the prefusion conformation. Just because you have the protein sequence doesn't mean it will fold into the protein expressed on the virus, because the viral protein still has the virus attached to it! In addition, the stabilization of the the protein was found to be more immunogenic than the wild type spike protein. This optimization is non-trivial. This vaccine was thus built on an already robust pipeline of research, highlighting the importance of funding basic science research.

They were able to produce testable mRNA-LNP product within 5 days of the sequence being published. An overview of the methods used to develop the formulations is described below. Imagine trying to do this at scale and at cost. It is truly a wonder how millions of doses are able to be manufactured.

![methods](/method.jpg "methods")

### Preclinical Testing

I'm going to go over this very briefly, for all the experiments, visit their [paper](https://www.biorxiv.org/content/10.1101/2020.06.11.145920v1.full).

In short, they did (read: published) 3 experiments:

1. Immunogenicity
2. VAERD (Vaccine-associated enhanced respiratory disease)
3. Viral Replication

In the immunogenicity experiments, they essentially delivered the mRNA-LNP formulation to mice at varying doses and measured neutralizing antibody responses. I'll let the data speak for itself:

![Fig1](/F2.large.jpg "Fig1")

The VAERD experiments were done to ensure safety. Previously it had been observed that children immunized with whole-inactivated virus vaccines against RSV and measles virus and who devloped Th2-biased immune responses, developed VAERD. Although the mechanisms behind VAERD are unknown, symptoms include severe respiratory disease with prolonged fever and clinical signs, and pathological changes of increased areas of lung consolidation and moderate to severe bronchointerstitial pneumonia and necrotizing bronchiolitis. To assess the safety profile in this regard, the scientists essentially probed the Th1/Th2 balance in T-cell responses via flow and determined that there was no Th2 bias.

Finally, the researchers assessed viral replication and infection in upper and lower airways. Briefly, mice were immunized with a challenge and booster dose and 5 weeks post boost, they were challenged with SARS-CoV-2. Both histology and assay results demonstrate minimal viral load in the high 1 ug dose group.  

![Fig2](/F4.large.jpg "Fig2")

### Clinical Trials

Laboratory work once the protein sequence was released took 66 days before it was tested in first human clinical trials. Phase 1 trials began on March 16, 2020, and a Phase 2 began 74 days later on May 29, 2020. The Phase II trials had 2 cohorts (300 ages 18-55 and 50 age 50+)

From their [Phase I study](https://www.nejm.org/doi/full/10.1056/nejmoa2022483), we now know that high levels of neutralizing antibodies were observed through 119 days following first vaccination and 90 days following second vaccination (~1 month between challenge and booster).

The key Phase III efficacy trial started in July, enrolling 30,000 participants in a 1:1 study design with prevention of coronavirus infection as the primary endpoint. The dose was 100 ug, based on results from the Phase I study.

So what is the efficacy? The calculation is hard to find in news reporting, but the CDC website has a [formula](https://www.cdc.gov/csels/dsepd/ss1978/lesson3/section6.html) ((Risk among unvaccinated - risk among vaccinated) / risk among unvaccinated).

We're all familiar at this point with the 94.5% efficacy and 0 severe cases among the vaccinated group (11 in placebo group). Adverse events included injection site pain (2.7%), and after the second dose included fatigue (9.7%), myalgia (8.9%), arthralgia (5.2%), headache (4.5%), pain (4.1%) and erythema/redness at the injection site (2.0%). The 95 total coronavirus cases included 15 older adults (ages 65+), 12 Hispanic or LatinX, 4 Black or African Americans, 3 Asian Americans and 1 multiracial.

### Manufacturing and Distribution

Moderna is partnering with Lonza and Catalent to manufacture the vaccine with hopes of 500 million - 1 billion doses per year. Further segmenting this by time period, there is expected to be 20 million doses by the end of 2020, and between 100-125 million through Q1 2021.

Once distributed, the vaccine is expected to remain stable at refrigerated temperatures (2-8 degrees C) for up to 30 days, and at standard freezer temperatures (-20 C) for 6 months. The vaccine can be handled at room temperature for 12 hours and does not require dilution prior to delivery.
