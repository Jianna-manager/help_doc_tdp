---
description: Odd ratio or Beta-values from population studies, ranging from -1 to 1
---

# Genetics

Genetic data in knowledge base is imported from Open Targets portal, and NHGRI GWAS catalog. The data is formatted to map SNPs level statistics to gene-level statistics i.e. odd-ratio or beta-value.

We have 4 different diseases — PSP, ALS, FTD and OI.

## PSP

## FTD

## ALS & OI

The delimited column headers for Genetics data are a bit harder to understand, but they should correspond to “{analysis\_type}_{score\_type}_{source}_{disease\_id}_{publication\_id}” (for example, “GWAS\_beta\_otgenetics\_MONDO0004976\_PMID19451621”). You can thereby decompose this to get a dict of information about the score (i.e., that could be used in a text box that appears on mouse-hover). Let me know if this kind of information works as a sufficient descriptor of each data set. I see that I need to fix some of these headers to be properly splittable, as in some cases internal underscores came through that will disrupt decomposing the delimited strings.

**{disease name}\_{"GWAS"}\_{**_**score type**_**}\_{source}\_{disease id}\_{publication\_id}**, for example, “GWAS\_beta\_otgenetics\_MONDO0004976\_PMID19451621”
