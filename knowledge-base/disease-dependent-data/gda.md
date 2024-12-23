---
description: Gene Disease Association score, ranging from 0 to 1
---

# GDA

Gene disease association score is from Open Targets portal. It qualifies the strength of the association between a gene and a disease. This score is derived using a combination of evidence from diverse data sources, e.g. genetic studies, transcriptomics, somatic mutations, drugs and pathways, etc.

Let's take the data of PSP disease as an example. The PSP data in Open Targets is shown as below, where you can see the scores of different gene-disease association combinations.

<figure><img src="../../.gitbook/assets/image (27).png" alt=""><figcaption><p>PSP data in Open Targets platform</p></figcaption></figure>

We transformed the data from Open Targets into the CSV format below, then inserted into our knowledge base.&#x20;

<figure><img src="../../.gitbook/assets/image.png" alt=""><figcaption><p>GDA data in our knowledge base</p></figcaption></figure>

The naming convention of GDA data in the knowledge base follows the format of **{"GDA"}\_{disease name}\_{gene-disease association type}**, for example, "GDA\_PSP\_OT Crispr validation", shown as below:

<figure><img src="../../.gitbook/assets/Screenshot 2024-12-04 220414.png" alt=""><figcaption><p>GDA data naming convention</p></figcaption></figure>
