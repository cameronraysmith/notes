+++
title = "PyClone Statistical inference of clonal population structure in cancer by Roth and Shah in 2014"
author = ["Cameron Smith"]
lastmod = 2020-09-20T17:35:40-04:00
slug = "PyClone_Statistical_inference_of_clonal_population_structure_in_cancer_by_Roth_and_Shah_in_2014"
draft = false
+++

## Lectures {#lectures}


### "[Andrew  Roth’s  lectures](<https://www.youtube.com/playlist?list=PLAFFlrzSa6m8PiKPKLBl8Av7RNw4F5-2F>)" {#andrew-roth-s-lectures--https-www-dot-youtube-dot-com-playlist-list-plafflrzsa6m8pikpklbl8av7rnw4f5-2f}


## Paper {#paper}


### [pyclone]({{< relref "pyclone" >}}) is a bayesian clustering method for grouping sets of deeply sequenced somatic mutations into ****putative clonal clusters**** while estimating their cellular prevalences and ****accounting for allelic imbalances**** introduced by ****segmental copy-number changes**** and ****normal-cell contamination**** {#pyclone--pyclone-dot-md--is-a-bayesian-clustering-method-for-grouping-sets-of-deeply-sequenced-somatic-mutations-into-putative-clonal-clusters-while-estimating-their-cellular-prevalences-and-accounting-for-allelic-imbalances-introduced-by-segmental-copy-number-changes-and-normal-cell-contamination}


### Online Methods {#online-methods}

<!--list-separator-->

-  [pyclone]({{< relref "pyclone" >}}) model and implementation

<!--list-separator-->

-  Running [pyclone]({{< relref "pyclone" >}}) and MCMC analysis

<!--list-separator-->

-  Evaluation and benchmarks

<!--list-separator-->

-  Alternative methods

<!--list-separator-->

-  Normal-tissue mixture experiments

<!--list-separator-->

-  Copy-number analysis

<!--list-separator-->

-  HIgh-grade serous ovarian cancer

<!--list-separator-->

-  Single-cell genotyping of frozen high-grade serous ovarian cancers


### Supplementary results {#supplementary-results}

<!--list-separator-->

-  1. Simulated data results

<!--list-separator-->

-  2. High grade serous ovarian cancer results

<!--list-separator-->

-  3. Stability of predictions using different copy number predictions


### Supplementary discussion {#supplementary-discussion}

<!--list-separator-->

-  1. Incorporating external sources of copy number information

    <!--list-separator-->

    -  See [Interfaces of Malignant and Immunologic Clonal Dynamics in Ovarian Cancer by Zhang and Shah in 2018]({{< relref "Interfaces_of_Malignant_and_Immunologic_Clonal_Dynamics_in_Ovarian_Cancer_by_Zhang_and_Shah_in_2018" >}}) for integration with [ReMixT Clone-specific genomic structure estimation in cancer by McPherson and Shah 2017]({{< relref "ReMixT_Clone-specific_genomic_structure_estimation_in_cancer_by_McPherson_and_Shah_2017" >}})

<!--list-separator-->

-  2. Limitations

    <!--list-separator-->

    -  pyclone clusters mutations that appear at similar cellular frequencies as opposed to clustering cells by mutational composition

        <!--list-separator-->

        -  if any pair of two subclones exists at similar cellular frequencies the model will falsely cluster the mutations associated to each subclone together as if there were only one...so there could be merging of subclones

    <!--list-separator-->

    -  A key assumption of our model is that all cells within each populations have the same genotype.

    <!--list-separator-->

    -  We note that our assumptions are predicated on the notion of a ’perfect’ and ’persistent phylogeny whereby mutations accrue over time and persist in clones and their descendants and mutations occur exactly once.

    <!--list-separator-->

    -  We have shown that our model can accommodate multi-sample data in a principled way by using hierarchical Bayesian modelling where statistical strength is borrowed across datasets, dramatically decreasing uncertainty while increasing accuracy.

<!--list-separator-->

-  3. Alternative applications


### Supplementary note: statistical inference of clonal population structure in cancer {#supplementary-note-statistical-inference-of-clonal-population-structure-in-cancer}

<!--list-separator-->

-  1 The [pyclone]({{< relref "pyclone" >}}) model description

    <!--list-separator-->

    -

<!--list-separator-->

-  2 Multiple samples modeling

    <!--list-separator-->

    -

<!--list-separator-->

-  3 Addressing overdispersion

    <!--list-separator-->

    -

<!--list-separator-->

-  4 Methods for eliciting [pyclone]({{< relref "pyclone" >}}) priors over mutational genotypes

    <!--list-separator-->

    -

<!--list-separator-->

-  5 Generation of synthetic data

    <!--list-separator-->

    -
