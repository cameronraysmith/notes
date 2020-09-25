+++
title = "Probabilistic Modeling and Statistical Inference by Michael Betancourt in 2019"
author = ["Cameron Smith"]
lastmod = 2020-09-24T01:26:09-04:00
slug = "Probabilistic_Modeling_and_Statistical_Inference_by_Michael_Betancourt_in_2019"
draft = false
+++

## keywords {#keywords}

-   [probabilistic inference]({{< relref "probabilistic_inference" >}}), [probabilistic programming]({{< relref "probabilistic_programming" >}}), [model construction]({{< relref "model_construction" >}})


## contents {#contents}


### 1. Probabilistic modeling {#1-dot-probabilistic-modeling}

<!--list-separator-->

-  1.1 The observational process

    <!--list-separator-->

    -  Distinct interfaces between measurement devices, the phenomenon of interest, and their environment lead to distinct observational processes that may each require careful tailoring within the model-construction process.

<!--list-separator-->

-  1.2 The true data generating process

    <!--list-separator-->

    -  observation space: \\[Y\\]

    <!--list-separator-->

    -  data generating process: probability distribution over the observation space

    <!--list-separator-->

    -  space of all data generating processes: \\[\mathcal{P}\\]

    <!--list-separator-->

    -  true data generating process, \\[\pi^{\dagger}\\]: probability distribution that exactly captures the observational process in a given application

    <!--list-separator-->

    -  explicitly realized observations from the observational process: \\[\tilde{y}\\]

    <!--list-separator-->

    -  arbitrary points in the observation space: \\[y\\]

<!--list-separator-->

-  1.3 The observational model

    <!--list-separator-->

    -  observational model vs model configuration space: the subspace, \\[\mathcal{S} \subset \mathcal{P}\\], of data generating processes considered in any particular application

    <!--list-separator-->

    -  parametrization: a map from a model configuration space \\[\mathcal{S}\\] to a parameter space \\[\mathcal{\Theta}\\] assigning to each model configuration \\[s \in \mathcal{S}\\] a parameter \\[\theta \in \mathcal{\Theta}\\]

    <!--list-separator-->

    -  probability density for an observational model: \\[\pi\_{\mathcal{S}}(y; s)\\] in general using the parametrization to assign \\[\pi\_{\mathcal{S}}(y; \theta)\\]

    <!--list-separator-->

    -  1.3.1 The generative structure of an observational model

    <!--list-separator-->

    -  1.3.2 Limitation of observational models

    <!--list-separator-->

    -  1.3.3 Model-based calibration

<!--list-separator-->

-  1.4 Model-based inferences


### 2. Frequentist inference {#2-dot-frequentist-inference}

<!--list-separator-->

-  2.1 Point estimators

<!--list-separator-->

-  2.2 Set estimators

<!--list-separator-->

-  2.3 Frequentist inference in practice


### 3. Bayesian inference {#3-dot-bayesian-inference}

<!--list-separator-->

-  3.1 Probabilistic scholarship

    <!--list-separator-->

    -  3.1.1 The prior distribution

    <!--list-separator-->

    -  3.1.2 The likelihood function

    <!--list-separator-->

    -  3.1.3 The posterior distribution

    <!--list-separator-->

    -  3.1.4 The complete Bayesian model

<!--list-separator-->

-  3.2 Employing our education

    <!--list-separator-->

    -  3.2.1 Making inferences

    <!--list-separator-->

    -  3.2.2 Making decisions

    <!--list-separator-->

    -  3.2.3 Making predictions

<!--list-separator-->

-  3.3 Bayesian calibration

    <!--list-separator-->

    -  3.3.1 Calibrating predictions

        <!--list-separator-->

        -  Good’s “device of imaginary results” [[12](<https://betanalpha.github.io/assets/case%5Fstudies/modeling%5Fand%5Finference.html#ref-Good:1950>)].

    <!--list-separator-->

    -  3.3.2 Calibrating posterior behaviors

    <!--list-separator-->

    -  3.3.3 Calibrating posterior computation


### 4. Comparing asymptotic apples to preasymptotic oranges {#4-dot-comparing-asymptotic-apples-to-preasymptotic-oranges}


### 5. Conclusion {#5-dot-conclusion}


## references {#references}


### frequentist perspective {#frequentist-perspective}

<!--list-separator-->

-  [1] Casella, G. and Berger, R. L. (2002). \_\_Statistical inference\_\_. Duxbury Thomson Learning.

<!--list-separator-->

-  [2] Lehmann, E. L. and Casella, G. (2006). \_\_Theory of point estimation\_\_. Springer Science &amp; Business Media.

<!--list-separator-->

-  [3] Keener, R. W. (2011). \_\_Theoretical statistics: Topics for a core course\_\_. Springer.


### Bayesian perspective {#bayesian-perspective}

<!--list-separator-->

-  [4] Bernardo, J.-M. and Smith, A. F. M. (2009). \_\_Bayesian theory\_\_. John Wiley &amp; Sons, Ltd., Chichester.

<!--list-separator-->

-  [5] Lindley, D. V. (2014). \_\_Understanding uncertainty\_\_. John Wiley &amp; Sons, Inc., Hoboken, NJ.

<!--list-separator-->

-  [6] MacKay, D. J. C. (2003). \_\_Information theory, inference and learning algorithms\_\_. Cambridge University Press, New York.


### [7] Sivia, D. S. (2006). \_\_Data analysis\_\_. Oxford University Press, Oxford. {#7-sivia-d-dot-s-dot--2006--dot-data-analysis-dot-oxford-university-press-oxford-dot}


### [8] McElreath, R. (2016). \_\_Statistical rethinking: A bayesian course with examples in r and stan\_\_. CRC Press. {#8-mcelreath-r-dot--2016--dot-statistical-rethinking-a-bayesian-course-with-examples-in-r-and-stan-dot-crc-press-dot}


### [9] Box, G. E. P. and Draper, N. R. (1987). \_\_Empirical model-building and response surfaces\_\_. John Wiley &amp; Sons, Inc., New York. {#9-box-g-dot-e-dot-p-dot-and-draper-n-dot-r-dot--1987--dot-empirical-model-building-and-response-surfaces-dot-john-wiley-and-amp-sons-inc-dot-new-york-dot}


### [10] Diaconis, P. and Skyrms, B. (2017). \_\_Ten great ideas about chance\_\_. Princeton University Press. {#10-diaconis-p-dot-and-skyrms-b-dot--2017--dot-ten-great-ideas-about-chance-dot-princeton-university-press-dot}


### [11] Betancourt, M. (2015). A unified treatment of predictive model comparison. {#11-betancourt-m-dot--2015--dot-a-unified-treatment-of-predictive-model-comparison-dot}


### [12] Good, I. (1950). \_\_Probability and the weighing of evidence\_\_. Hafners, New York. {#12-good-i-dot--1950--dot-probability-and-the-weighing-of-evidence-dot-hafners-new-york-dot}


### [13] Talts, S., Betancourt, M., Simpson, D., Vehtari, A. and Gelman, A. (2018). Validating bayesian inference algorithms with simulation-based calibration. {#13-talts-s-dot-betancourt-m-dot-simpson-d-dot-vehtari-a-dot-and-gelman-a-dot--2018--dot-validating-bayesian-inference-algorithms-with-simulation-based-calibration-dot}


### [14] Stan Development Team. (2018). Stan: A C++ library for probability and sampling, version 2.17.1. {#14-stan-development-team-dot--2018--dot-stan-a-c-plus-plus-library-for-probability-and-sampling-version-2-dot-17-dot-1-dot}
