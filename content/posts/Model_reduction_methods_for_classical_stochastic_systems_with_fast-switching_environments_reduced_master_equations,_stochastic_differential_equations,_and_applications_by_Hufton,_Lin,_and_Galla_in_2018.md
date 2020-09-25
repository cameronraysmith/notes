+++
title = "Model reduction methods for classical stochastic systems with fast-switching environments reduced master equations, stochastic differential equations, and applications by Hufton, Lin, and Galla in 2018"
author = ["Cameron Smith"]
lastmod = 2020-09-20T17:35:26-04:00
slug = "Model_reduction_methods_for_classical_stochastic_systems_with_fast-switching_environments_reduced_master_equations,_stochastic_differential_equations,_and_applications_by_Hufton,_Lin,_and_Galla_in_2018"
draft = false
+++

## arXiv version {#arxiv-version}


### I. Introduction {#i-dot-introduction}


### II. General definitions {#ii-dot-general-definitions}

<!--list-separator-->

-  A. Model

<!--list-separator-->

-  B. Simplification in the adiabatic limit


### III. Analysis for fast but finite environments {#iii-dot-analysis-for-fast-but-finite-environments}

<!--list-separator-->

-  A. General formalism

<!--list-separator-->

-  B. Switching dynamics independent of state of the system with two environmental states

<!--list-separator-->

-  C. Basic example


### IV. Several species and reduced master equations with negative transition rates {#iv-dot-several-species-and-reduced-master-equations-with-negative-transition-rates}

<!--list-separator-->

-  A. Model

<!--list-separator-->

-  B. Positive correlation between the species

<!--list-separator-->

-  C. Anti-correlations and negative transition rates

<!--list-separator-->

-  D. Lack of positivity in initial transients


### V. Numerical approaches to a master equation with negative rates {#v-dot-numerical-approaches-to-a-master-equation-with-negative-rates}

<!--list-separator-->

-  A. Distribution-level simulation

<!--list-separator-->

-  B. 'Path-level' simulation


### VI. An intuition to our expansion on the level of sample paths {#vi-dot-an-intuition-to-our-expansion-on-the-level-of-sample-paths}

<!--list-separator-->

-  A. Effective time-averaged reaction rates

<!--list-separator-->

-  B. Averaging out the environmental process

<!--list-separator-->

-  C. Resulting event statistics

<!--list-separator-->

-  D. Simulation procedure for discrete-time sample paths


### VII. Expansion in system size {#vii-dot-expansion-in-system-size}

<!--list-separator-->

-  A. Overview

    <!--list-separator-->

    -  1. Expansion in environmental time scale

    <!--list-separator-->

    -  2. Expansion in powers of inverse system size

    <!--list-separator-->

    -  3. Combined expansion

    <!--list-separator-->

    -  4. Piecewise-deterministic process

<!--list-separator-->

-  B. Example

<!--list-separator-->

-  C. Linear-noise approximation

<!--list-separator-->

-  D. Analytical approximation for power spectra


### VIII. Further applications {#viii-dot-further-applications}

<!--list-separator-->

-  A. Model of protein production

    <!--list-separator-->

    -  1. Motivation and model definitions

    <!--list-separator-->

    -  2. Comparison of different approximation schemes

<!--list-separator-->

-  B. Bimodal genetic switch

    <!--list-separator-->

    -  1. Model

    <!--list-separator-->

    -  2. Comparison of the different approximation schemes

    <!--list-separator-->

    -  3. Efficient simulations and required computing time

<!--list-separator-->

-  C. Genetic network with multiple genes

<!--list-separator-->

-  D. Genetic circuit with exclusive binding

<!--list-separator-->

-  E. Staged switching of the environment

<!--list-separator-->

-  F. Reliability analysis and crack propagation


### IX. Summary and conclusions {#ix-dot-summary-and-conclusions}


### Appendix A: State-dependent environmental process {#appendix-a-state-dependent-environmental-process}

<!--list-separator-->

-  1. Adiabatic limit

<!--list-separator-->

-  2. Next-order contribution


### Appendix B: Further remarks relating to power spectra in Sec. V B {#appendix-b-further-remarks-relating-to-power-spectra-in-sec-dot-v-b}

<!--list-separator-->

-  1. Cross spectra in adiabatic limit

<!--list-separator-->

-  2. Independence of \\[S\_{AA} (\omega)\\] from \\[\Delta \beta\\]


### Appendix C: Kramers-Moyal expansion {#appendix-c-kramers-moyal-expansion}

<!--list-separator-->

-  1. Kramers-Moyal expansion of reduced master equation

<!--list-separator-->

-  2. Reduced Liouville equation

<!--list-separator-->

-  3. Kramers-Moyal expansion for two-species model


### Appendix D: Applications--Further details {#appendix-d-applications-further-details}

<!--list-separator-->

-  1. Reduced master equation for bi-stable genetic circuit

<!--list-separator-->

-  2. Gene circuit with exclusive binding


## Classical stochastic systems with fast-switching environments: Reduced master equations, their interpretation, and limits of validity (published March 2019) {#classical-stochastic-systems-with-fast-switching-environments-reduced-master-equations-their-interpretation-and-limits-of-validity--published-march-2019}


### I. Introduction {#i-dot-introduction}


### II. General definitions and reduced master equation {#ii-dot-general-definitions-and-reduced-master-equation}

<!--list-separator-->

-  A. Model

    <!--list-separator-->

    -  Definitions

        <!--list-separator-->

        -  the system and environment are represented by sets of discrete-states evolving in continuous time

        <!--list-separator-->

        -  \\[\ell\\] states of classical system

        <!--list-separator-->

        -  \\[\sigma\\] states of the environment

        <!--list-separator-->

        -  \\[p(\ell, \sigma, t)\\] joint probability of finding the system in state \\[\ell\\] and the environment in state \\[\sigma\\] at time \\[t\\]

        <!--list-separator-->

        -  \\[R^{(\sigma)}\_{\ell' \rightarrow \ell}\\] is the rate at which the system transitions from state \\[\ell'\\] to state \\[\ell\\] when the environment is in state \\[\sigma\\]

        <!--list-separator-->

        -  \\[\mathcal{M}\_{\sigma}\\] operator that determines changes of the system relative to the environment in state \\[\sigma\\] given by

            <!--list-separator-->

            -  \\[\mathcal{M}\_{\sigma} p(\ell, \sigma, t) \equiv \sum\_{\ell'} R^{(\sigma)}\_{\ell' \rightarrow \ell} p(\ell, \sigma, t)\\]

        <!--list-separator-->

        -  \\[\lambda A\_{\sigma' \rightarrow \sigma}(\ell)\\] is the rate at which the environment transitions from state \\[\sigma'\\] to \\[\sigma\\]

            <!--list-separator-->

            -  Note that in general these rates are considered to be functions that are dependent upon the state of the system \\[\ell\\]

            <!--list-separator-->

            -  \\[\lambda\\] is nothing more than a scaling parameter that allows for the tuning of the rate of environmental switching relative to the rate of switching of the system

        <!--list-separator-->

        -  \\[\Pi (\ell, t) = \sum\_{\sigma} p(\ell, \sigma, t)\\] the marginal probability over states of the system that results from integrating over states of the environment

        <!--list-separator-->

        -  The transition operators \\[R\\] and \\[A\\] are chosen so that their diagonal elements are constrained by

            <!--list-separator-->

            -  \\[ R^{(\sigma)}\_{\ell \rightarrow \ell} = \* \sum\_{\ell' \neq \ell} R^{(\sigma)}\_{\ell \rightarrow \ell'} \\]

            <!--list-separator-->

            -  \\[ A\_{\sigma \rightarrow \sigma}(\ell) = -\sum\_{\sigma' \neq \sigma} A\_{\sigma \rightarrow \sigma'}(\ell) \\]

    <!--list-separator-->

    -  Dynamics

        <!--list-separator-->

        -  \\[\frac{d}{dt} p(\ell, \sigma, t) = \mathcal{M}\_{\sigma} p(\ell, \sigma, t) + \lambda \sum\_{\sigma'} A\_{\sigma' \rightarrow \sigma}(\ell) p(\ell, \sigma', t)\\]

    <!--list-separator-->

    -  Notes on the regime of interest

        <!--list-separator-->

        -  This paper focuses on the situation where \\[\lambda \gg 1\\] which corresponds to a characteristic timescale of environmental dynamics that is much shorter (or, equivalently, that the environmental dynamics are much faster) than that of the system under study

<!--list-separator-->

-  B. Simplification in the adiabatic limit

    <!--list-separator-->

    -  The adiabatic limit in this case is associated with that of infinitely fast environmental switching encoded by \\[\lambda \rightarrow \infty\\]

    <!--list-separator-->

    -

<!--list-separator-->

-  C. Reduced master equation for large but finite separation of timescales


### III. Two envrionmental states: reduced master equation and basic example {#iii-dot-two-envrionmental-states-reduced-master-equation-and-basic-example}

<!--list-separator-->

-  A. Environmental dynamics independent of the state of the system

<!--list-separator-->

-  B. Example: population with two species

    <!--list-separator-->

    -  1. Reduced dynamics

    <!--list-separator-->

    -  2. Positive correlation between the species

    <!--list-separator-->

    -  3. Anticorrelations and negative transition rates


### IV. Interpretation of negative rates: continuous time {#iv-dot-interpretation-of-negative-rates-continuous-time}

<!--list-separator-->

-  A. Flow of probability and renormalized reaction rates\\

<!--list-separator-->

-  B. Lack of positivity in initial transients


### V. Interpretation in discrete time {#v-dot-interpretation-in-discrete-time}

<!--list-separator-->

-  A. Effective time-averaged reaction rates

<!--list-separator-->

-  B. Averaging out the environmental process

<!--list-separator-->

-  C. Resulting event statistics

<!--list-separator-->

-  D. Simulation procedure for discrete-time sample paths


### VI. Criterion for the emergence of negative rates {#vi-dot-criterion-for-the-emergence-of-negative-rates}

<!--list-separator-->

-  A. Model and notation

<!--list-separator-->

-  B. Reduced master equation


### VII. Summary and conclusions {#vii-dot-summary-and-conclusions}


### Appendix A: State-dependent environmental process {#appendix-a-state-dependent-environmental-process}

<!--list-separator-->

-  1. Adiabatic limit

<!--list-separator-->

-  2. Next-order contribution


### Appendix B: Continuous-time simulation algorithms for reduced master equations with negative rates {#appendix-b-continuous-time-simulation-algorithms-for-reduced-master-equations-with-negative-rates}

<!--list-separator-->

-  1. Path-level simulation

    <!--list-separator-->

    -  a. Description of the simulation algorithm

    <!--list-separator-->

    -  b. Test of the algorithm

<!--list-separator-->

-  2. Distribution-level simulation


## Model reduction methods for population dynamics with fast-switching environments: Reduced master equations, stochastic differential equations, and applications (published March 2019) {#model-reduction-methods-for-population-dynamics-with-fast-switching-environments-reduced-master-equations-stochastic-differential-equations-and-applications--published-march-2019}


### I. Introduction {#i-dot-introduction}


### II. Model definitions and background {#ii-dot-model-definitions-and-background}

<!--list-separator-->

-  A. Model

<!--list-separator-->

-  B. Reduced master equation

<!--list-separator-->

-  C. Objective of the present work


### III. Expansion in system size {#iii-dot-expansion-in-system-size}

<!--list-separator-->

-  A. Overview

    <!--list-separator-->

    -  1. Expansion in environmental

    <!--list-separator-->

    -  2. Expansion in powers of inverse system size

    <!--list-separator-->

    -  3. Combined expansion

    <!--list-separator-->

    -  4. Piecewise-deterministic process

<!--list-separator-->

-  B. Simple examples

    <!--list-separator-->

    -  1. Population with one species

    <!--list-separator-->

    -  2. Population dynamics with two species


### IV. Applications {#iv-dot-applications}

<!--list-separator-->

-  A. Bimodal genetic switch

    <!--list-separator-->

    -  1. Model

    <!--list-separator-->

    -  2. Comparison of the different approximation schemes

    <!--list-separator-->

    -  3. Efficient simulations and required computing time

<!--list-separator-->

-  B. Genetic circuit with exclusive binding

<!--list-separator-->

-  C. Reliability analysis and crack propagation


### V. Summary and conclusions {#v-dot-summary-and-conclusions}


### Appendix A: Further details of the analysis of the model in Section III. B. 1. {#appendix-a-further-details-of-the-analysis-of-the-model-in-section-iii-dot-b-dot-1-dot}

<!--list-separator-->

-  1. Kramers-Moyal expansion of the reduced master equation

<!--list-separator-->

-  2. Reduced Liouville equation


### Appendix B: Kramers-Moyal expansion for the two-species model in Section III. B. 2. {#appendix-b-kramers-moyal-expansion-for-the-two-species-model-in-section-iii-dot-b-dot-2-dot}


### Appendix C: Applications: Further Details {#appendix-c-applications-further-details}

<!--list-separator-->

-  1. Reduced master equation for the bistable genetic circuit

<!--list-separator-->

-  2. Gene circuit with exclusive binding


### Appendix D: Further applications {#appendix-d-further-applications}

<!--list-separator-->

-  1. Genetic network with multiple genes

<!--list-separator-->

-  2. Staged switching of the environment
