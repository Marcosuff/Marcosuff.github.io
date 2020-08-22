# Where to get data for drug discovery projects

Welcome to the first post of my blog! In this post I'm going to show some resources to build your first dataset to start working with small molecules. Before we start coding and looking at thousands of resources, let's introduce the theme.

## What is computational drug discovery?

The drug discovery process is quite complicated, involding professionals of different expertises and years of research in order to deliver safe and efficient drugs to pacients. When I say years I mean it. The whole takes between 10 - 15 years, from the initial development of a prototype molecule to regulatory approval and marketing. In addition, the current drug discovery scenario is expensive. To deliver a single new drug to market, pharmaceutical companies usually spend around U$S 1 billion, including costs with initial screening to preclinical and clinical trials. 

To complicate even more, the failure rate in drug discovery campaigns is extremely high. Less than 1% of drug candidates screened at initial stages reach preclinical and clinical phases. This means that  the bulk of expenses come from initial screening and failures to optimize the molecules before testing in humans. Therefore, pharma companies are always looking for ways to accelerate the discovery of good drug candidates and methods to optimize these candidates to potential drug inververntions for clinical trials.  But how can we do that? Is it possible to work smarter and identify the best candidates before expending with biological tests and chemical synthesis? 

Yes. There is a way! Computational drug discovery (CDD) is the yellow brick road to prioritize molecules for screening. In CDD, computer programs can be used to generate research hyphotesis on the fly, leading to a high throughput of ideas that can be explorered even without any molecule available for testing. We can roughly classify CDD methods in three groups: 

A) **Ligand-based**: in ligand-based strategies the information about a biological target for the small molecules is limited. On the other hand, we have much more information on biologically active / inactive molecules for the target. Methods in this class include: 1) Searching databases for similar molecules to a query and 2) searching for molecules that contain a specific chemical group. 

B) **Structure-based**: structure-based discovery involves more information about the biological target, including it's basic building blocks (e.g., amino acid sequence for proteins) and an experimentally determined 3D structure  (e.g., by X-ray crystallography, cryoEM and other methods). By using a 3D structure, it's possible to study how the biological target interacts with small molecules and how to modify it's behaviour to treat or cure a disease. 

In summary, the amount of information available about a biological target will dictate which strategy to follow. However, it's also possible to used combined approachs as more data becomes available. For instance, an initial similarity search (ligand-based) can be used to select a small fraction of molecules from a chemical vendor. These initial hits can be further evaluated for using molecular docking and dynamics (structure-based) in order to select the ones with the best interaction pattern with the target. 

## Let's get to it: Getting data for CDD projects!

Biological and chemical data are becoming more abundat now due. Different online databases to download chemical data and biological tests results are available for free and some Pharma companies also make their datases available. In addition, data from academic groups can also be obtained by request or as supplementary information on scientific papers. The main question you need to answer is: **what kind of data are you looking for?**

In this post we will explore [ChEMBL](https://www.ebi.ac.uk/chembl/), a freely available database of chemical and biological data for over 13K targets, with more than 1 million curated biological tests results. ChEMBL includes results of many biological endpoints including, inhibition and dissociation constants (K<sub>i</sub> andK<sub>d</sub>, respectivelly), the concentration that inhibits 50% of activity (IC<sub>50</sub>); and also pharmacokinetics parameters, such as absorption, distribution, metabolism and toxicity (ADMET). 
