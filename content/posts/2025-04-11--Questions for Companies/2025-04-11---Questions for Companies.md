---
title: "Questions for Biotech Companies"
date: "2025-04-17T12:00:00.000Z"
template: "post"
draft: False
slug: "/blog/biotechquestions/"
category: "Life Sciences"
tags:
  - "Life sciences"
  - "Healthcare"
description: "and prompts for an LLM"
---

Shorter post today. I have to write a thesis proposal and prepare for a DAC meeting. 

One thing that I think is painful about the current biotech ecosystem, specifically for therapeutics investing, is how difficult it is to have a detailed discussion about a target or a drug. The circle of competence for people that understand basic PK/PD, what aspects of a molecule design are worth paying attention to, how to interpret clinical datasets, etc. seems small to me. Biotech sits at a massive discount relative to other industries and if there ever was a time to buckle in and learn how to pick companies, it is now. 

Having a clearer understanding of what makes a molecule good or bad, or how to critique a development plan gives you a leg up if you want to do anything useful yourself. Differentiating between the me-toos should be a learnable skill.

I don't think I'm good by any means at being a biotech investor. Be gentle. This blog post is simply a list of questions I've found useful to help frame diligence. Even simply knowing certain key words for prompting makes ChatGPT way more useful to you. Garbage in, garbage out.

## Questions to Ask Companies

### Market
- How large is the addressable patient population
    - What proportion of this is refractory to standard of care versus treatment naïve?
- What are the major competitors and data readouts in the next 24 months
- What are the major competitive differentiators of the molecule?
- Are there any strategic advantages that the company has over competitors (IP, KOLs, BD relationships, etc.)

### Molecule
- What is the dosing interval?
- What is the expected injection or pill burden?
    - Any formulation issues?
- What is the off-target toxicity profile?
    - Any selectivity issues?
    - Any delivery issues if directed towards a specific tissue?
    - hERG, CYP, genotoxicity
    - What are the tox profiles of expected metabolites?
- Has there been a clear PK/PD relationship identified?
    - Are there assays with good in vitro in vivo efficacy correlation?
    - Does the PK/PD relationship hold over disparate chemical matter?
- What exposure is the molecule able to achieve? How does this compare with competitors?
    - Bioavailability (%F), Cmax, Cmin, T1/2, Koff, Kp
- Does the molecule satisfy Lipinski’s rule of 5
    - More than 5 hydrogen bond donors (sum of OH and NH groups)
    - More than 10 hydrogen bond acceptors (sum of N and O atoms)
    - A molecular weight (MW) over 500 daltons
    - A logP (octanol–water partition coefficient) greater than 5 (indicates high lipophilicity). Or really logP or logD outside 1 - 3.5
- Are there other small molecule red flags (thank you topical and vague)?
    - Unprotected amines (reactive, off target binding, metabolized readily)
    - Carboxylic acids (idiosyncratic tox)
    - Check basicity, whether it is a substrate of membrane transporters
    - Nitro or furan groups (reactive/toxic), sulfonamides or anilines?
    - Phenyls (easy hydroxylation)
- Any structural alerts from in silico tox screens (e.g. Derek Nexus)?
- Is there any CMC / manufacturability risk? E.g. Is the compound chemically tractable at large scale (multi-kg GMP)?
    - Does the molecule have a difficult synthetic route? tricyclic or higher-order fused system?
- Are there tissue penetration considerations?
- For antibodies, what kind of properties have been engineered / what mutations?

### Biology
- What is the expected on-target toxicity profile?
    - KO mice, previous clinical datasets
- What does the human genetics evidence say? (GWAS of target and upstream/downstream pathways)
- Are there clinical datasets that derisk the target?
- What are the PD biomarkers and how good are they?
- What are the known resistance pathways?
- What is the rate of target turnover (e.g. half-life and resynthesis)? Any TMDD issues?
- How important is the pathway and modulated target (effect size)
- How compelling is the preclinical evidence?
    - Do the potency assays translate to clinical efficacy?
- Is there a thesis for why modulating the target exceeds efficacy of existing treatments?
- What is the level of target expression in various stages of disease, and after treatment with different therapies?
- How easy is it to measure target expression and will a companion diagnostic need to be developed?
- Can the biology be generalized to other novel indications?
- Are there combinatorial strategies being tested or envisioned?

### Clinical Strategy
- What is the clinical development plan beyond the current stage? (esp. if moving from POC to pivotal)
- What endpoints are being pursued in upcoming trials? Are they clinically meaningful or surrogate?
- What is the likelihood of regulatory acceptance of the selected endpoints?
- Any adaptive trial designs or enrichment strategies being used?
- Has the company engaged with FDA or EMA? Any feedback from pre-IND/Type B meetings?
- What are the potential bottlenecks in patient recruitment or trial site setup?

### Company specific
- Can you talk about your fundraising history, how you spent the money, how the story has changed over time.
- If we could skip straight to the money slides: key proof of concept data for demonstrating why your asset or technology is a step up from competitors that would be great.
- Can we walk through the TPP together step by step?
- What have others shown about this target, what is the competition and why is your approach better?
- What are the near-term inflection points for partnering or acquisition?
- Has there been pharma diligence or interest in co-development?
- What is the fallback plan if clinical data is mid? What is the bar for success?