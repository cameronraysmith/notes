+++
title = "Towards A Principled Bayesian Workflow by Michael Betancourt in 2020"
author = ["Cameron Smith"]
lastmod = 2020-09-24T01:27:05-04:00
slug = "Towards_A_Principled_Bayesian_Workflow_by_Michael_Betancourt_in_2020"
draft = false
+++

## keywords {#keywords}

-   [probabilistic inference]({{< relref "probabilistic_inference" >}}), [probabilistic programming]({{< relref "probabilistic_programming" >}}), [model construction]({{< relref "model_construction" >}})


## See also {#see-also}


### Schad, D. J., Betancourt, M., & Vasishth, S. (2019). Toward a principled Bayesian workflow in cognitive science. Retrieved from <http://arxiv.org/abs/1904.12765> {#schad-d-dot-j-dot-betancourt-m-dot-and-vasishth-s-dot--2019--dot-toward-a-principled-bayesian-workflow-in-cognitive-science-dot-retrieved-from-http-arxiv-dot-org-abs-1904-dot-12765}


### pymc3 implementation of principled bayesian workflow {#pymc3-implementation-of-principled-bayesian-workflow}

<!--list-separator-->

-  <https://github.com/lstmemery/principled-bayesian-workflow-pymc3> last updated in August/November 2018 as of <span class="timestamp-wrapper"><span class="timestamp">&lt;2020-08-09 Sun&gt;</span></span>


## Contents {#contents}


### 1. Questioning authority {#1-dot-questioning-authority}

<!--list-separator-->

-  How do we construct models ****consistent with our domain expertise**** that are ****adequate to capture the structure of the phenomena of interest****, and support ****accurate**** and ****relevant inference**** from ****observations we can feasibly perform**** with respect to the ****specific questions we need to answer**** in order to make ****well-informed decisions****?

<!--list-separator-->

-  Questions

    <!--list-separator-->

    -  Is our model consistent with our domain expertise?

        <!--list-separator-->

        -  \_\_domain expertise consistency\_\_

    <!--list-separator-->

    -  Will our computational tools be sufficient to accurately fit our posteriors?

        <!--list-separator-->

        -  \_\_computational faithfulness\_\_

    <!--list-separator-->

    -  Will our inferences provide enough information to answer our questions?

        <!--list-separator-->

        -  \_\_inferential adequacy\_\_

    <!--list-separator-->

    -  Is our model rich enough to capture the relevant structure of the true data generating process?

        <!--list-separator-->

        -  \_\_model adequacy\_\_

<!--list-separator-->

-  1.1 Domain expertise consistency

    <!--list-separator-->

    -  1.1.1 Quantifying consequences

    <!--list-separator-->

    -  1.1.2 Prior pushforward checks

    <!--list-separator-->

    -  1.1.3 Prior predictive checks

<!--list-separator-->

-  1.2 Computational faithfulness

    <!--list-separator-->

    -

<!--list-separator-->

-  1.3 Inferential calibration

<!--list-separator-->

-  1.4 Model adequacy

    <!--list-separator-->

    -  1.4.1

    <!--list-separator-->

    -  1.4.2

    <!--list-separator-->

    -  1.4.3 Posterior retrodiction checks

    <!--list-separator-->

    -  1.4.4 Limitations of posterior retrodiction checks


### 2. Building a mystery {#2-dot-building-a-mystery}

<!--list-separator-->

-


### 3. Components of a principled Bayesian workflow {#3-dot-components-of-a-principled-bayesian-workflow}

<!--list-separator-->

-  Phases of the workflow

    <!--list-separator-->

    -  Pre-model, Pre-data

        <!--list-separator-->

        -  1. Conceptual analysis

        <!--list-separator-->

        -  2. Define observation space

        <!--list-separator-->

        -  3. Construct summary statistics

    <!--list-separator-->

    -  Post-model, Pre-data

        <!--list-separator-->

        -  4. Develop model

        <!--list-separator-->

        -  5. Construct summary functions

        <!--list-separator-->

        -  6. Simulate Bayesian ensemble

        <!--list-separator-->

        -  7. Prior checks

        <!--list-separator-->

        -  8. Configure algorithm

        <!--list-separator-->

        -  9. Fit simulated ensemble

        <!--list-separator-->

        -  10. Algorithmic calibration

        <!--list-separator-->

        -  11. Inferential calibration

    <!--list-separator-->

    -  Post-model, Post-data

        <!--list-separator-->

        -  12. Fit observed data

        <!--list-separator-->

        -  13. Diagnose posterior fit

        <!--list-separator-->

        -  14. Posterior retrodictive checks

<!--list-separator-->

-  Example workflow executions

    <!--list-separator-->

    -  Incompatible model assumptions

    <!--list-separator-->

    -


### 4. Close enough for an effective demonstration {#4-dot-close-enough-for-an-effective-demonstration}

<!--list-separator-->

-  4.1 First iteration

    <!--list-separator-->

    -  4.1.1 Conceptual analysis

    <!--list-separator-->

    -  4.1.2 Define observational space

    <!--list-separator-->

    -  4.1.3 Construct summary statistics

    <!--list-separator-->

    -  4.1.4 Model development

    <!--list-separator-->

    -  4.1.5 Construct summary functions

    <!--list-separator-->

    -  4.1.6 Simulate Bayesian ensemble

    <!--list-separator-->

    -  4.1.7 Prior checks

    <!--list-separator-->

    -  4.1.8 Configure algorithm

    <!--list-separator-->

    -  4.1.9 Fit simulated ensemble

    <!--list-separator-->

    -  4.1.10 Algorithm calibration

    <!--list-separator-->

    -  4.1.11 Inferential calibration

    <!--list-separator-->

    -  4.1.12 Fit the observation

    <!--list-separator-->

    -  4.1.13 Diagnose posterior fit

    <!--list-separator-->

    -  4.1.14 Posterior retrodictive checks

<!--list-separator-->

-  4.2 Second iteration

    <!--list-separator-->

    -
