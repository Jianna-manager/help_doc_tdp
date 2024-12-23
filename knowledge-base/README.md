---
description: Disease-dependent and disease-independent data
icon: layer-group
---

# Knowledge Base

The knowledge base provides the node and edge properties of network visualization and analysis, which relies on the [Reference Genome data](reference-genome-data.md) and [Protein-Protein Interaction (PPI) network data](protein-protein-interaction-ppi-data.md).

Data types are transformed to defined representations, so that they can be handled consistently and displayed intuitively by the frontend.

We have different kinds of data available on the left panel of network visualization page, which allows you to change the network property based on personal needs. The data behind each feature is divided into 2 different types -- [**disease-dependent**](disease-dependent-data/) and [**disease independent**](disease-independent-data/).

* **Disease-dependent** data varies with different diseases, including [LogFC](disease-dependent-data/logfc.md) (_Differential expression in Log2 fold change_), [GDA ](disease-dependent-data/gda.md)(_Gene Disease Association score_) and [Genetics](disease-dependent-data/genetics.md) (_Odd ratio or Beta-values from population studies_). Currently, you can switch among 4 different diseases — ALS, FTD, OI and PSP. You can find the full names of these 4 diseases [here](../dashboard/by-protein-name.md#step-2-selecting-preferable-options).
* **Disease-independent** data DO NOT vary with different diseases, including [Pathway](disease-independent-data/pathway.md) (_Pathway membership from KEGG and Reactome_), [Druggability](disease-independent-data/druggability.md) (_Druggability score form OpenTargets_), [Tissue Enrichment](disease-independent-data/tissue-enrichment.md) (_Tissue-specific expression from GTEX and HPA_) and [Database](disease-independent-data/database.md) (_Membership in various database_).

### Knowledge Base Summary

<table data-full-width="false"><thead><tr><th width="194">Data type</th><th width="154">Representation</th><th width="228">Experiment types</th><th>Sources</th></tr></thead><tbody><tr><td>LogFC</td><td>[-Inf, +Inf]</td><td>RNAseq, Ptoteomics</td><td>Verge, AD (Mayo, ROSMAP, MSBB)</td></tr><tr><td>GDA</td><td>[0, 1]</td><td>AI, Meta-scores</td><td>Open Targets</td></tr><tr><td>Genetics</td><td>[-1, 1]</td><td><p>GWAS w/ eQTL (OR/Beta),</p><p>GeneBurden (OR/Beta)</p></td><td>Open Targets Genetics</td></tr><tr><td>Pathway</td><td>Binary</td><td>Curation</td><td>KEGG, Reactome</td></tr><tr><td>Druggability</td><td>[0, 1]</td><td>AI, Meta-scores</td><td>DrugnomeAI, Pharose</td></tr><tr><td>Tissue Enrichment</td><td>[0, +Inf]</td><td>single cell RNAseq &#x26; single cell databases</td><td>GTEx, HPA</td></tr><tr><td>Database</td><td>Binary</td><td></td><td></td></tr></tbody></table>

