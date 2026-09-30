This repo contains reproducible workflows for the study *[Intestinal microbes: an axis of functional diversity among large marine consumers](https://doi.org/10.1098/rspb.2019.2367)*. Repo contains all the R Markdown files and R code for processing and analyzing different data types.

## Goals of the Study

1. Assess the taxonomic composition of intestinal communities from herbivorous reef fish.
2. Determine the diversity of these communities and their similarity/dissimilarity.
3. Identify differentially abundant ASVs across the host species.
4. Predict the specificity of differentially abundant ASVs.

## Code Availability

To access the code, you have a few options:

1) Visit the project website at https://projectdigest.github.io/.
2) Clone or download this repo.
3) Visit specific workflow pages and/or download individual R Markdown (.Rmd) files. Details for this option are provided below under **Workflows**.

## Data Availability

For information on all raw data and data products, please see the [Data Availability](https://projectdigest.github.io/data_availability.html) page. There you will find more details and links to the figshare project site and European Nucleotide Archive project page. Please also check at the bottom of individual workflow pages for access to related data.

## Supplemental Material for Paper

In addition to the Supplemental Material available online we include [a page on the website](https://projectdigest.github.io/supplemental_material.html) that contains all seven supplementary tables, figures, and methods for the paper. Tables are horizontally scrollable. You can sort tables and download (or copy) the data. Some tables contain external hyperlinks. you can download the raw [Rmd file](https://github.com/projectdigest/web/blob/master/build/supplemental_material.Rmd).

## Workflows

You can access each step of the workflows by using the navigation bar at the top of the [Project DIGEST](https://projectdigest.github.io/) website or by downloading the R Markdown (.Rmd) files in this repo. Below is a brief description of each workflow, as well as information on how to access the code. Workflows appear in order.

### A. Field Analyses

#### No 1. Field Observations

In the first section we run some analyses on field-based behavioral assays of the different herbivorous reef fish species. Workflows can be found on the [Field Observations page](https://projectdigest.github.io/1_field_observations.html) or you can download the raw [Rmd file](https://github.com/projectdigest/web/blob/master/build/1_field_observations.Rmd).

### B. 16S rRNA Analysis

This section contains four separate workflows for processing and analyzing the 16s rRNA data set.

#### No 2. DADA2 Workflow

In this part we go through the process of processing raw 16S rRNA read data including assessing read quality, filtering reads, correcting errors, and infersing amplicon sequence variants (ASVs). Workflows can be found on the [DADA2 page](https://projectdigest.github.io/2_dada2.html) or you can download the raw [Rmd file](https://github.com/projectdigest/web/blob/master/build/2_dada2.Rmd).

#### No 3. Data Preparation

Next we go through the steps of defining sample groups, creating phyloseq objects, removing unwanted samples, and removing contaminant ASVs. Various parts of this section can easily be modified to perform different analyses. For example, if you were only interested in a specific taxa or group of samples, you could change the code here to create new phyloseq objects. Workflows can be found on the [Data Preparation page](https://projectdigest.github.io/3_data_prep.html) or you can download the raw [Rmd file](https://github.com/projectdigest/web/blob/master/build/3_data_prep.Rmd).

#### No 4. Composition & Diversity

Here we assess taxonomic composition, alpha diversity, and beta diversity. Phyloseq offers many options for assessing diversity, including several alpha diversity metrics, additional ordination and distance methods, and so on. You can play around with these settings to how it affects the results. Workflows can be found on the [Composition & Diversity page](https://projectdigest.github.io/4_diversity.html) or you can download the raw [Rmd file](https://github.com/projectdigest/web/blob/master/build/4_diversity.Rmd).

#### No 5. Differentially Abundant ASVs

We wanted to understand how ASVs partitioned across host species. We also wanted to assess the specificity of each ASV to determine habitat preference. To our knowledge there is no quantitative way to do this. The only attempt we are aware of was [MetaMetaDB](http://mmdb.aori.u-tokyo.ac.jp/) but it is based on a 454 database and no longer seems to be in active development. So we used an approach based on the work of [Sullam et. al.](https://doi.org/10.1111/j.1365-294X.2012.05552.x), first identifying differentially abundant ASVs, then searching for closest database hits, and finally using phylogenetic analysis and top hit metadata (isolation source, natural host) to infer habitat preference. Workflows can be found on the [Differentially Abundant ASVs page](https://projectdigest.github.io/5_da_asv.html) or you can download the raw [Rmd file](https://github.com/projectdigest/web/blob/master/build//5_da_asv.Rmd).

#### No 6. Synthesis

In this section we pull together the results and try to make sense of the microbiomes from these herbivorous reef fish. How are ASVs partitioning across host? How similar are these ASVs to sequences from other studies? What can these patterns tell us about host specificity?Workflows can be found on the [Synthesis page](https://projectdigest.github.io/6_synthesis.html) or you can download the raw [Rmd file](https://github.com/projectdigest/web/blob/master/build//6_synthesis.Rmd).
