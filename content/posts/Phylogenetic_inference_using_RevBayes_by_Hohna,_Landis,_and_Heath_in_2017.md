+++
title = "Phylogenetic inference using RevBayes by Hohna, Landis, and Heath in 2017"
author = ["Cameron Smith"]
lastmod = 2020-09-20T17:35:35-04:00
slug = "Phylogenetic_inference_using_RevBayes_by_Hohna,_Landis,_and_Heath_in_2017"
draft = false
+++

## \![RevBayes homepage](<https://lh3.googleusercontent.com/eZrgzeB0zszjoCjTpiR8SaamsiWHZ92Wr2TrZbb1Rel%5FyFwDX-ylYxr0WoQf3irtkvyV0SvIJR-6Ko8VmWrrWVqzi09WirJVGhz0aQFfygKGzsuoxTsiqTx7tpp2W9%5F0Pvt6DgpBcog=w613-h668-no>) {#revbayes-homepage--https-lh3-dot-googleusercontent-dot-com-ezrgzeb0zszjocjtpir8saamsiwhz92wr2trzbb1rel-yfwdx-ylyxr0woqf3irtkvyv0svijr-6ko8vmwrrwvqzi09wirjvghz0aqffygkgzsuoxtsiqtx7tpp2w9-0pvt6dgpbcog-w613-h668-no}


## I. Getting started with RevBayes {#i-dot-getting-started-with-revbayes}


### 1. Introduction {#1-dot-introduction}


### 2. Introduction to RevBayes and Rev {#2-dot-introduction-to-revbayes-and-rev}


### 3. Reading and manipulating data {#3-dot-reading-and-manipulating-data}


## II. Inference {#ii-dot-inference}


### 4. Introduction to Markov chain Monte Carlo algorithms {#4-dot-introduction-to-markov-chain-monte-carlo-algorithms}


## III. Basic phylogeny estimation {#iii-dot-basic-phylogeny-estimation}


### 5. Continuous time Markov model for discrete character evolution {#5-dot-continuous-time-markov-model-for-discrete-character-evolution}

<!--list-separator-->

-  5.1 Overview

    <!--list-separator-->

    -  See [Markov Processes for Stochastic Modeling by Oliver Ibe in 2013]({{< relref "Markov_Processes_for_Stochastic_Modeling_by_Oliver_Ibe_in_2013" >}}) section 5.2 for a derivation of the solution to the stationary continuous-time Markov process in terms of the matrix exponential of the instantaneous rate matrix, which is usually named \\[Q\\] "5.2 Transient analysis"

    <!--list-separator-->

    -  The substitution models of molecular evolution

        <!--list-separator-->

        -  JC69

        <!--list-separator-->

        -  F81

        <!--list-separator-->

        -  HKY85

        <!--list-separator-->

        -  GTR

        <!--list-separator-->

        -  GTR+Gamma

        <!--list-separator-->

        -  GTR+Gamma+I

<!--list-separator-->

-  5.2 Data and files

<!--list-separator-->

-  5.3 Example: character evolution under the Jukes-Cantor substitution model

    <!--list-separator-->

    -  Steps

        <!--list-separator-->

        -  (1) setting up a Jukes-Cantor (JC) substitution model for an alignment of the cytochrome b subunit;

        <!--list-separator-->

        -  (2) approximating the posterior probability of the tree topology and node ages (and all other parameters) using MCMC, and;

        <!--list-separator-->

        -  (3) summarizing the MCMC output by computing the maximum a posteriori tree.

    <!--list-separator-->

    -  \![Graphical model representation of the Jukes-Cantor phylogenetic model](<https://lh3.googleusercontent.com/XsxT1xV-uWFmuy5ifQpYoWLVrjruIFh9FapTQW4GmgaicMz6aoorx7Qb27UEg%5FSCbUHrIvWqk3OIfcZOKP4bsNe2%5FJPxsD4gcy%5F5MWejvhe0vXSmC3TllIjxZ8e4fMt4F2qawtlBox2%5FgTnqwCiLObpVlvv3uMZ5Ow1VH59ZzXGzL6EZ%5F%5F2LLxvv3s%5FDD0nztMnEV6ufOG1LLQCDUVJb5DngFnVwrLSz4n4VspNiuZhboFBXILAEUbbMYfNFl3nrOR0LVEIbycQ7U74fmoOtN%5F1vSPOQppWW4RqKXi%5F8ISqrM94YFxkUgI66ziOSnKs3iGnw4I2pbtMdkyI1Q0QV8N-Qr3G1ykeTWvbcBB1x0iO1kQ6B9D6FqlUKfhLGYAO31rNQFNhFv%5FROYXIB5aGu3Lwrz4SIH91%5F1Sz5pH53oSVDvmaSi0cQ7O2G14uNhFuy3lPh5kO49SO9apZkkGcK8Q3pvl4VZNTYiqHLDGw5MLlLPT5DGM8CyLTihryQKEq2ZjQFgXKwR7IGJuG9nVeVv95OiXtDodx8hJoKhu6J9XhS6NjepBcOz1eCrLRyxRwDuzcprk2ijy5-CEQlreTplY5tfsKV78Lrbp1daKwNji7Xhb5P3VHQoyiQH5ORDR1eS%5Fym-nUQDd5HFbHeDjny9TbhzppJKj9cP%5Fge9i%5F4laeIIDI6DPvibWZZdjhWc8ihyfSFA1AYS9WhARa9PFFvc189j4uMRDeiYsARCtZH95TYRBeI=w1018-h475-no>)

    <!--list-separator-->

    -  \![Jukes-Cantor 1969 substitution model](<https://lh3.googleusercontent.com/gK5SYbUVLY4h8baOGYBOt5OyLVKYQlm%5FYKMS%5FVl7x5KISoTYVmZpFAfVdED9w1kAzhyyzK6ZhqExV71AKQrpaYqdEfYdEFv0isJ5buKi9iWEI9RunyX4SCnApQ-PRIbM0kaDbcVg0LU=w960-h399-no>)

    <!--list-separator-->

    -

    <!--list-separator-->

    -  \\[t\\] is the branch length in units of time

<!--list-separator-->

-  5.4 The Hasegawa-Kishino-Yano (HKY) 1985 substitution model

<!--list-separator-->

-  5.5 The General Time-Reversible (GTR) substitution model

<!--list-separator-->

-  5.6 The discrete gamma model of among site rate variation

<!--list-separator-->

-  5.7 Modeling invariable sites


## IV. Model selection, model averaging, and model testing {#iv-dot-model-selection-model-averaging-and-model-testing}


### 6. {#6-dot}


## V. More on substitution models {#v-dot-more-on-substitution-models}


### 7. {#7-dot}


## VI. Divergence time estimation {#vi-dot-divergence-time-estimation}


### 8. {#8-dot}


### 9. {#9-dot}


### 10. {#10-dot}


## VII. Diversification rate estimation {#vii-dot-diversification-rate-estimation}


### 11. {#11-dot}


### 12. {#12-dot}


### 13. {#13-dot}


### 14. {#14-dot}


### 15. {#15-dot}


### 16. {#16-dot}


## VIII. Gene tree-species tree estimation {#viii-dot-gene-tree-species-tree-estimation}


### 17. {#17-dot}


### 18. {#18-dot}


### 19. {#19-dot}


## IX. Biogeography {#ix-dot-biogeography}


### 20. {#20-dot}


### 21. {#21-dot}


## X. Phylogenetic comparative method {#x-dot-phylogenetic-comparative-method}


### 22. {#22-dot}


##  {#}
