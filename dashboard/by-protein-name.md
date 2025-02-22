---
description: This approach is based on the interactions existing in our database
---

# By protein name

When you enter the main page of our website, simply click the tab "By protein name" <img src="../.gitbook/assets/image (11).png" alt="" data-size="line"> on the left panel, you will see the corresponding dashboard on the right as below:

<figure><img src="../.gitbook/assets/1727212576614.png" alt=""><figcaption><p>Dashboard for "By protein name"</p></figcaption></figure>

There are 3 different sections on the dashboard, which corresponds to 3 steps to construct your network by using gene information.&#x20;

### Step 1: Entering Seed Genes

You can either type into the "Seed Genes" textbox or upload a txt file.&#x20;

* **Type into textbox**: Manually type in seed gene names or their Ensembl IDs to generate the network. You can also mix gene names and Ensembl IDs together. The format can be comma-separated or line-separated.
* **Upload a txt file**: The gene names or Ensembl IDs can also be uploaded as txt format. The format is the same as the "Seed Genes" textbox.

The seed genes are the foundation of the network generation, your network will be expanded based on the seed genes you provided. Once you determine the seed genes, you can proceed to Step 2 to generate your own network.

### Step 2: Selecting Preferable Options

Now you can select different options from different parameters to integrate your own feature styles into your network. We offer 4 parameters here -- Disease map, Order, Interaction type and Min interaction score. Let's go through them one by one:

* **Disease map**: You can determine your network falls into which disease category, and no worries, if you want to change the disease after generating the network, you can easily change it on the [left panel](../network-visualization/left-panel.md) of the network visualization page. We offer 4 different diseases -- PSP, ALS, FTD and OI, with the full names as:
  * PSP: Progressive Supranuclear Palsy.
  * ALS: Amyotrophic lateral sclerosis.
  * FTD: Frontotemporal dementia.
  * OI: Osteogenesis imperfecta.
* **Order**: Based on the seed genes you provided, you can expand the network from different perspective. We provide 3 different orders:
  * Zero order: This option only gives you the interactions among the seed genes.
  * First order: This option involves the neighbors of the seed genes. Besides the interactions among the seed genes in Zero order, it also gives the interactions among seed genes and their neighbors.
  * Second order: This option is a combination of First order and Zero order. It not only contains the interactions among seed genes themselves & the interactions among the seed genes and their neighbors, it also contains the interactions among the neighbors of seed genes.
* **Interaction type**: We provide 4 different interaction types for you to construct your own network:
  * PPI: Protein-protein interactions.
  * FunPPI: Functional protein-protein interactions.
  * BIKG: Currently not available.
  * ComPPlete: Currently not available.
* **Min interaction score**: Each interaction has its own score, from computer science perspective, we also call it edge weight. You can select the cutoff here to make your network thinner or fatter. There are 4 different cutoff available: Low (0.15), Medium (0.4), High (0.7) and Highest (0.9).

### Step 3: Clicking "Submit" Button

After click "Submit", a confirmation page will pop up. There are 2 tabs available in the pop-up window: **Available Genes** and **Unavailable Genes**.

* **Available Genes**: The listed genes are available in our database, you can confirm the information of seed genes.
* **Unavailable Genes**: The listed genes have no records in our database. You probably entered a wrong name or wrong Ensembl ID, you go back to the "Seed Genes" textbox or your uploaded file to make the corresponding changes and submit again. Or you can simply click "Confirm" button and proceed to the [Network Visualization page](../network-visualization/).

<figure><img src="../.gitbook/assets/1731621737030.png" alt=""><figcaption><p>Available genes.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/1731621794199.png" alt=""><figcaption><p>Unavailable genes.</p></figcaption></figure>
