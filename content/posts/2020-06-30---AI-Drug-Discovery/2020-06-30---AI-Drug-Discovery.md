---
title: "AI Powered Drug Discovery"
date: "2020-06-30T12:00:00.000Z"
template: "post"
draft: False
slug: "/blog/AI_Drug_Discovery/"
category: "Healthcare"
tags:
  - "Healthcare"
  - "Life Sciences"
description: "A New Paradigm for Drug Development"
---

It's no secret that the traditional drug discovery model is expensive, time consuming, and has recently produced compounds with marginal efficacy in clinical trials and high failure rates. Large biopharma companies are increasingly outsourcing R&D to academic labs and small/mid size startups via licensing partnerships or acquisitions. Biopharma is among the most active industry sectors in terms of mergers and acquisitions and this trend looks to grow as companies stockpile more and more cash. This is all evidence to demonstrate that large cap biopharma companies have yet to create efficient internal R&D programs and thus have a need for high efficiency screening and discovery programs.

![High Attrition](/AI_Drug/Attrition.jpg "Attrition")

Increasingly, companies have also focused on biologics, such as antibodies, vaccines, and DNA/RNA therapies. These are typically larger structures that rely on the body's internal biological machinery. This is in contrast to small molecule therapeutics which are used to drug specific receptors or structures by fitting in a shape pocket. Small molecule compounds are synthesized using traditional organic chemistry techniques and include medications like Sovaldi for Hepatitis, Aspirin for pain relief, and Abilify for Schizophrenia. 

Small molecule therapeutics make up roughly 90% of drugs available on today's market. However, since 2014, biologics have accounted for 93% of spending growth in discovery platforms. This makes sense, since 9 out of the top 10 best selling drugs in 2019 are biologics, compared to just 5 in 2014. Biologics have advantages over small molecule therapeutics such as higher specificity and better safety profiles, lower attrition in clinical trials, and less competition due to difficulty developing biosimilars. However, with the simpler drug discovery and development process of small molecules and superior delivery and distribution characteristics, small molecule drugs are here to stay.

### A Perfect Use Case for AI

So what is causing the growth of biologics and stagnant investment in small molecule therapeutics programs? The current drug discovery pathway relies heavily on human derived research and capabilities. 'Rational drug design' comprises discovering a mechanism, identifying a druggable target, and the design of a drug to hit the target, mostly in an iterative, linear process. There is an increasing sense that the low hanging fruit has been picked, that the easy mechanisms and targets are already drugged. Still, others have suggested that we are more so held back by our ability to design molecules.

This drug design process is highly automated, but increasing speed and compute power has not kept pace with costs/demand in an efficient manner. Computers are adept at simulating molecule interactions, but the binding profile is only one of many important drug design considerations. Adding to the inefficiencies, old techniques will only simulate existing molecule compounds, or try new ones, but not intelligently, merely tweaking the structure in an arbitrary manner. For each of these millions of such simulations, algorithms may use molecular mechanics and predictive binding equations to estimate the affinity of the designed ligand. These equations have limited efficacy because they rely on human derived models, and are not trained on extensive previous data libraries.

This is the perfect use case for artificial intelligence. Human logic has driven us to utilize a design approach for solving drug discovery. We used first principles to develop rational drug design and to contrive equations that model molecule interactions. Yet, we are still unable to understand many aspects of biophysics and molecular interactions, so changing our model to a search approach makes much more sense. With exponential growth in compute power, data, and infrastructure, we have the computational resources to power a search strategy, where we can rely on machines to tell us what is correct. 

Given clean, large, and relevant datasets, AI algorithms can independently decode and organize data in ways that we wouldn't initially think of. Prediction, classification, and even imagination are all problems an AI engine can solve now without any dependencies on biological knowledge or principles that humans may be tied to. This set of advantages that AI provides us is what is powering the rapid growth of modern computational drug design.

### Modern Drug Design Technologies

Modern computational drug design strategies are able to factor in many more factors including toxicity, formulation, and kinetics due to tremendous growth in available training data. Using machine learning, we are able to predict key properties of molecules such as absorption, distribution, metabolism, elimination, and toxicity (ADMET properties) based off a vectorized representation of a molecule. The inability to properly predict these properties are estimated to account for up to 50% of clinical trial failures, so algorithms that can predict ADMET properties in silico before expensive clinical trials are of tremendous value. 

The team at Genesis Therapeutics has developed PotentialNet, a deep learning algorithm for precisely this purpose. A neural net can be trained on molecules we already know to be successful, in order to screen molecules we aren't sure about. The human factor here is to calibrate the data into the correct format, but there is no need to rely on archaic equations to predict binding as before.

Another example comes from a group from MIT who used a deep learning approach to discover halicin as a novel antibiotic. Halicin is structurally divergent from traditional antibiotics, but demonstrated curative antibiotic activity in-vivo and favorable pharmacokinetics in mice. This approach has demonstrated how deep learning networks such as these can be trained on libraries of existing compounds and their properties to predict not only important drug properties like ADMET, but also their therapeutic efficacy. 

The speed and efficiency of deep learning approaches versus previous brute force screening methods is a major advance here. This has significant implications especially for fields like antibiotics, where the business model doesn't allow for large R&D programs where scale allows brute force methods to work. If we're able to outsource the expensive creative work to machines, traditional commercial barriers to innovation can be bypassed, which is especially important for antibiotics and other low cost medications.

### Next Generation Computational Tools

Thus far, we have seen AI deployed primarily as a prediction tool. We can predict bioactivity and we can predict important drug properties, which is a crucial need for drug screening and improving the attrition rate during clinical trials. This type of work is especially valuable for large cap biopharma companies who already have hundreds of thousands of compounds and must bear the costs for bringing drugs to market. Startups doing this type of predictive work are thus frequent targets for industry collaboration. 

However, the next paradigm in AI drug discovery is not the efficacy prediction of existing molecules, but the creation of generative models that are able to 'imagine' de novo structures, pathways, and mechanisms. The first completely AI imagined molecule to be used in a human clinical trial will start enrollment in 2020. This molecule, created by another AI drug discovery startup, Exscientia, took 12 months from conception to clinical trial enrollment, 5x faster than the traditional workflow. Their system automatically extracts key performance markers from high-dimensional phenotypic readouts and uses these to generate and optimize new iterations of compounds, to rapidly evolve compounds that satisfy key performance criteria.

![Exscientia](/AI_Drug/Exscientia.jpg "Exscientia")

Platforms like these are in theory not only scalable, but also computationally less expensive than the traditional screening approach. This means that new molecules can be developed in a democratized manner, for indications traditionally avoided for not providing large enough returns on investment. As a 'full stack' AI drug discovery company generating its own data, Exscientia is able to leverage internal data collection capabilities to develop drug candidates in therapy areas where data is limited. Generative drug discovery thus is also an economically disruptive force, enabling the targeting of therapeutic areas that haven't previously been addressed. 

### Evaluating Startups in the Space

When evaluating a company in this space, it's important to consider exactly what problem the AI hopes to solve, whether it be speed, attrition, modeling accuracy, molecule design, or otherwise. The best companies will address multiple of these at once. Exscientia's full stack drug discovery platform addresses in some way, all of these. 

Another key consideration is data. When dealing with biological systems, it takes much longer to validate than deep learning for computer vision in driverless cars for instance because you need to carryout experiments with real organisms eventually. This impacts data collection and model feedback iteration speeds, making progress slower. Some start-ups have set up contractual partnerships with academia and research centers, enabling them to benefit from access to proprietary data and talent to help solve this problem. Many others collaborate directly with industry, but typically only once past the stage of developing several promising compounds.

Talent in particular is the biggest priority in this field. Drug discovery is a very academic field, yet you need a very multidisciplinary team of medicinal chemists, ML engineers, assay developers, etc. Every biopharma is trying to build up the internal expertise and is hiring data scientists, and you also need to compete with tech companies on the other end for data and ML engineers. A magnetic core with strong academic background, already demonstrating proof of concept is important. For example, the core technology from Genesis Therapeutics was developed during the CEO's PhD. Successful companies require highly trained, specialist data experts and experts in AI and computational biology, and the core team needs to be able to recruit such talent.

Lastly, this is a hyper competitive industry, which has both pros and cons. On one end, you need a very fast paced and competitive team that can easily detach and move on from their own research, since this field moves so quickly. It's easy to drown, either from the success of competitors, inability to secure collaborations, or simply due to the difficulty of the task at hand. It's possible even that the center of innovation in this field no longer happens in the U.S., as China has the most drug discovery AI research centers and the largest datasets to work with. On the other hand, this field is flooding with funding. VC dollars quadrupled in three years from 2016 to 2019, and the total R&D market is estimated to grow from $700 million in 2018 to $20 billion in the next five years. Large biopharma are seeking diversification of deals and collaborations to diversify drug discovery pipeline, and much of this growth has been and will be via AI driven solutions.

### The Bottom Line

The incredible pace of development demonstrates the immediate promise of using AI models to both intelligently screen and design therapeutics. We can integrate toxicity, pharmacokinetics, and formulation into the training set to improve the quality of molecules for the next steps of clinical testing. Even more promising is that the next generation of medicinal chemists can work collaboratively with algorithms, each able to creatively design compounds and mutually checking each other's work.

The bottom line here is that AI introduces a new paradigm of non-linearity in drug discovery. While previously we would try to answer the question of how to make screening, optimization, and testing faster, now we are asking how we do these processes smarter. We're solving both attrition and speed here. We can rely on machines to transition from our limitations as designers and turn biology into a search problem. We know AI can analyze data, we didn't know it could generate creative insights in this field, yet.

Personally, I think that this shift in mindset will be the transformation that propels drug discovery to break Eroom's Law. Biology for decades has been known to lag behind other fields, commanding huge amounts of human capital in an attempt to 'think' our way to cures. Finally, we have a tool that can quite literally predict biology, offloading the creative burden and covering our blindspots. In the immediate future, this technology will be used to democratize our search for small molecule therapeutics in indications previously economically unfeasible. 

In the long term, with the confluence of quantum computing and generation of more and more patient data, theres no obvious limit to what this platform can do. Large molecule therapeutics, protein therapeutics, and eventually even custom biologic design is not out of the question. On our existing library of drugs, we can optimize to reduce toxicity and improve other ADME properties, or even to achieve improved clinical outcomes.
Drug discovery is becoming supercharged.

### Select Startups in AI Drug Discovery

[Genesis Therapeutics](https://www.genesistherapeutics.ai/): A seed stage company developing tools to improve screening by better predicting pharmacological properties of drug compounds. Their AI platform, PotentialNet, predicts 20+ different ADMET properties.

[LabGenius](https://www.labgeni.us/): The Series A stage team at LabGenius is the first biopharmaceutical company developing next generation protein therapeutics using a machine learning-driven evolution engine (EVA™️). They use advanced deep-learning neural networks to explore protein fitness landscapes and improve multiple drug properties simultaneously.

[Exscientia](https://www.exscientia.ai/): Series B stage company working on drug target selection and de novo molecule design using machine learning. Exscientia is another frequent industry collaborator, and is the first company to develop an entirely AI generated compound for clinical trials. 

[Atomwise](https://www.atomwise.com/): Atomwise is a Series A stage industry collaborator that uses machine learning to improve drug hit rates by up to 10,000x and results 100 times faster than ultra high throughput screening. Atomwise's deep convolutional neural network, AtomNet, screens more than 100 million compounds each day for potency, selectivity, and polypharmacology, and guard against off-target toxicity.
