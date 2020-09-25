+++
title = "Effective fluctuation and response theory by Polettini and Esposito in 2018"
author = ["Cameron Smith"]
lastmod = 2020-09-20T17:34:19-04:00
slug = "Effective_fluctuation_and_response_theory_by_Polettini_and_Esposito_in_2018"
draft = false
+++

## I. Prologue {#i-dot-prologue}


### The FR states that the rate at which a system delivers entropy to the environment is a measure of the arrow of time, viz. of the asymmetry between the probability of microscopic paths and their time-reversed. {#the-fr-states-that-the-rate-at-which-a-system-delivers-entropy-to-the-environment-is-a-measure-of-the-arrow-of-time-viz-dot-of-the-asymmetry-between-the-probability-of-microscopic-paths-and-their-time-reversed-dot}


### The purpose of this paper is to present a general theory of the thermodynamics of a ****marginal set of currents**** and of the effective forces that drive them, under the assumption that somewhere in the belly of these coarser observables there lurk fundamental currents and forces that abide by the principles of Markovian stochastic thermodynamics. {#the-purpose-of-this-paper-is-to-present-a-general-theory-of-the-thermodynamics-of-a-marginal-set-of-currents-and-of-the-effective-forces-that-drive-them-under-the-assumption-that-somewhere-in-the-belly-of-these-coarser-observables-there-lurk-fundamental-currents-and-forces-that-abide-by-the-principles-of-markovian-stochastic-thermodynamics-dot}


### in the marginal theory the analog of an equilibrium state is a stalling state in which the marginal currents vanish, while the hidden currents might still be flowing, as if the observer was in the eye of a hurricane. {#in-the-marginal-theory-the-analog-of-an-equilibrium-state-is-a-stalling-state-in-which-the-marginal-currents-vanish-while-the-hidden-currents-might-still-be-flowing-as-if-the-observer-was-in-the-eye-of-a-hurricane-dot}


### as the observer adds more and more currents and forces to his accounting, a “hierarchy” of marginal theories is explored: a cross-hierarchical FR holds, that is the ultimate core result of the whole construction {#as-the-observer-adds-more-and-more-currents-and-forces-to-his-accounting-a-hierarchy-of-marginal-theories-is-explored-a-cross-hierarchical-fr-holds-that-is-the-ultimate-core-result-of-the-whole-construction}


### The validity of FRs under coarse-graining and of FDRs far from equilibrium, in particular at stalling, are two questions that have been frequently addressed. {#the-validity-of-frs-under-coarse-graining-and-of-fdrs-far-from-equilibrium-in-particular-at-stalling-are-two-questions-that-have-been-frequently-addressed-dot}


### In the formalism of chaotic dynamical systems, Gallavotti heuristically defined a local entropy production rate associated to a microscopic region of space that satisfies a FR. {#in-the-formalism-of-chaotic-dynamical-systems-gallavotti-heuristically-defined-a-local-entropy-production-rate-associated-to-a-microscopic-region-of-space-that-satisfies-a-fr-dot}


### The validity of FRs for coarse-grained observables has been considered in Refs. [16] and [17], where the IFR is studied when the observer has incomplete information. {#the-validity-of-frs-for-coarse-grained-observables-has-been-considered-in-refs-dot-16-and-17-where-the-ifr-is-studied-when-the-observer-has-incomplete-information-dot}


### Biological applications {#biological-applications}

<!--list-separator-->

-  The coarse-graining of the statistics of the currents for biochemical systems has been considered in Ref. [18].

<!--list-separator-->

-  For chemical networks where only some molecular species can be monitored experimentally, Bravi and Sollich [21] derived systematic models for subsystem dynamics that can help with the inference problem of estimating properties of the environment from observed sub-network dynamics.


### All these approaches differ from ours as we assess properties of marginal observables ****without resorting to ad hoc redefinitions of the stochastic observable**** under consideration (the currents). {#all-these-approaches-differ-from-ours-as-we-assess-properties-of-marginal-observables-without-resorting-to-ad-hoc-redefinitions-of-the-stochastic-observable-under-consideration--the-currents--dot}


### authors of Ref. [29] comment that “in order to re-establish the laws of thermodynamics, one not only has to look at the local marginal systems, but also [at] the correlations between them”, and this can be achieved by some effective description. Effective thermodynamic potentials also play a role in systems strongly coupled to their surroundings [30] {#authors-of-ref-dot-29-comment-that-in-order-to-re-establish-the-laws-of-thermodynamics-one-not-only-has-to-look-at-the-local-marginal-systems-but-also-at-the-correlations-between-them-and-this-can-be-achieved-by-some-effective-description-dot-effective-thermodynamic-potentials-also-play-a-role-in-systems-strongly-coupled-to-their-surroundings-30}


## II. Parode: Enunciation of the main results {#ii-dot-parode-enunciation-of-the-main-results}


### Introduction {#introduction}

<!--list-separator-->

-  here is a less technical, yet self-contained discussion of the main results, which can be considered to be independent but less detailed


### A. Strophe: "Complete" fluctuations and response {#a-dot-strophe-complete-fluctuations-and-response}

<!--list-separator-->

-  ****Macroscopic thermodynamics**** describes systems through which a number \\[\vert \alpha \vert\\] of steady currents \\[\phi\_{\alpha}\\] flow

<!--list-separator-->

-  ****Affinities**** are conjugate (to?) thermodynamic forces \\[ \mathcal{A}\_{\alpha}\\]

<!--list-separator-->

-  One interpretation of this framework is as a model of interfaces between reservoirs

<!--list-separator-->

-  Together, the currents and affinities are considered as the irreducible observables of the theory where all conservation laws have been implemented via <span class="underline"><span class="underline">gauging out</span></span> reference reservoirs

<!--list-separator-->

-  The ****macroscopic entropy production rate**** (EPR) is a bilinear form

    <!--list-separator-->

    -  \\[\sigma \equiv \sum\_{\alpha} \phi\_{\alpha} \mathcal{A}\_{\alpha}\\]

    <!--list-separator-->

    -  The second law of thermodynamics states that \\[\sigma \geq 0\\] (this is stated later in Eq. 6)

<!--list-separator-->

-  At the ****microscopic**** scale, currents must become random variables to account for fluctuations. These may be due, for example, to thermal noise.

<!--list-separator-->

-  A single realization = path = trajectory in a timeframe \\[[0, t]\\] is (a function?) denoted \\[\omega^t\\]

<!--list-separator-->

-  ****Stochastic time-integrated currents**** \\[\Phi\_{\alpha}^{t} \equiv \Phi\_{\alpha} [\omega^t]\\] are functionals of these trajectories \\[\omega^t\\]

<!--list-separator-->

-  The ****expectation**** of the stochastic time-integrated currents is given by a functional integral with respect to a measure on trajectories \\[P(\omega^t) \mathcal{D} \omega^t\\] to be described in more detail later

    <!--list-separator-->

    -  \\[\langle  \Phi\_{\alpha}^{t}  \rangle = \int \mathcal{D} \omega^t P(\omega^t) \Phi\_{\alpha} [\omega^t]\\]

<!--list-separator-->

-  ****Temporal mean steady currents**** are then given in terms of the expectation of the stochastic time-integrated currents

    <!--list-separator-->

    -  \\[\phi\_{\alpha} \equiv \lim\_{t \rightarrow \infty} \frac{1}{t} \int \mathcal{D} \omega^t P(\omega^t) \Phi\_{\alpha} [\omega^t]\\]

    <!--list-separator-->

    -  \\[ \phi\_{\alpha} \equiv \lim\_{t \rightarrow \infty} \frac{\langle  \Phi\_{\alpha}^{t}  \rangle}{t} \\]

<!--list-separator-->

-  The ****entropy production**** along a single realization of a given process is

    <!--list-separator-->

    -  \\[\sum \Phi\_{\alpha}^t \mathcal{A}\_{\alpha} + O(1)\\]

<!--list-separator-->

-  The exponential of the entropy production is equal to the relative probability of time-integrated currents in the forward and reverse directions

    <!--list-separator-->

    -  \\[ \frac{ P( \\{ \Phi\_{\alpha} \\} ) }{ P( \\{ -\Phi\_{\alpha} \\} ) } = \exp \sum \Phi\_{\alpha} \mathcal{A}\_{\alpha}\\]

<!--list-separator-->

-  Finite-time fluctuation relations can be dealt with on the same footing as asymptotic ones whereby exact equality holds at all times rather than only in the limit of long times provided that the initial configuration associated with any given trajectory has an appropriate probability distribution

<!--list-separator-->

-  The integral fluctuation relation states

    <!--list-separator-->

    -  \\[ \langle \exp \* \sum \Phi\_{\alpha} \mathcal{A}\_{\alpha} \rangle = 1\\]

    <!--list-separator-->

    -  ^^Question^^: is this \\[\int \mathcal{D} \omega^t P(\omega^t)   \exp \left( \* \sum \Phi\_{\alpha} [\omega^t] \mathcal{A}\_{\alpha} \right) \\] ?

<!--list-separator-->

-  ****Detailed balance**** is attained when all affinities \\[\mathcal{A}\_{\alpha}\\] are zero, which implies all mean steady currents \\[\phi\_{\alpha}\\] are also zero and vice versa

<!--list-separator-->

-  Introduce an explicit dependence of the structural properties of the system on parameters

    <!--list-separator-->

    -  \\[ \mathbf{x} = \\{  x\_{\kappa}  \\}^{|\kappa|}\_{\kappa = 1}, \; | \kappa | \geq | \alpha | \\]

    <!--list-separator-->

    -  such that \\[|\alpha|\\] of them are <span class="underline"><span class="underline">thermodynamic</span></span> meaning that they have well defined equilibrium values with respect to which the affinities take non-zero values when the \\[x\_{\alpha}\\] are perturbed away from those equilibrium values

        <!--list-separator-->

        -  \\[\mathcal{A}\_{\alpha} (\mathbf{x}) = x\_{\alpha} \* x^{\mathrm{eq}}\_{\alpha}\\]

    <!--list-separator-->

    -  and that the remaining \\[x\_{\alpha}\\] on which the affinities do not depend are considered <span class="underline"><span class="underline">kinetic</span></span>

<!--list-separator-->

-  For systems slightly out of equilibrium

    <!--list-separator-->

    -  define

        <!--list-separator-->

        -  affinities and currents evaluated at equilibrium values of the parameters \\[\mathbf{x}\\]

            <!--list-separator-->

            -  \\[\mathcal{A}^{\mathrm{eq}}\_{\alpha} \equiv \mathcal{A}\_{\alpha}(\mathbf{x}^{\mathrm{eq}}) = 0\\]

            <!--list-separator-->

            -  \\[\phi^{\mathrm{eq}}\_{\alpha} \equiv \phi\_{\alpha}(\mathbf{x}^{\mathrm{eq}})=0\\]

        <!--list-separator-->

        -  response coefficients

            <!--list-separator-->

            -  \\[\phi\_{\alpha ; \kappa} \equiv \frac{\partial \phi\_{\alpha}}{\partial x\_{\kappa}}\\]

        <!--list-separator-->

        -  the time-scaled steady-state variance of the currents

            <!--list-separator-->

            -  \\[\phi\_{\alpha \alpha'} \equiv \lim\_{t \rightarrow \infty} \frac{1}{t} \langle \left( \Phi^t\_{\alpha} \* \langle \Phi^t\_{\alpha} \rangle  \right)  \left( \Phi^t\_{\alpha'} \* \langle \Phi^t\_{\alpha'} \rangle  \right) \rangle\\]

    <!--list-separator-->

    -  two near-equilibrium relations hold

        <!--list-separator-->

        -  the symmetrized fluctuation-dissipation relations (S-FDR)

            <!--list-separator-->

            -  \\[\phi^{\mathrm{eq}}\_{\alpha ; \alpha'} + \phi^{\mathrm{eq}}\_{\alpha' ; \alpha} = \phi^{\mathrm{eq}}\_{\alpha \alpha'}\\]

        <!--list-separator-->

        -  the reciprocal relations (RR)

            <!--list-separator-->

            -  \\[\phi^{\mathrm{eq}}\_{\alpha ; \alpha'} \* \phi^{\mathrm{eq}}\_{\alpha' ; \alpha} = 0\\]

<!--list-separator-->

-


### B. Antistrophe: marginal fluctuations and response {#b-dot-antistrophe-marginal-fluctuations-and-response}


### C. Epode: discussion and perspectives {#c-dot-epode-discussion-and-perspectives}


## III. Episode 1: Setup {#iii-dot-episode-1-setup}


### A. Algebraic graph theory in a pistachio-shell {#a-dot-algebraic-graph-theory-in-a-pistachio-shell}


### B. Master equation dynamics {#b-dot-master-equation-dynamics}


### C. Master equation thermodynamics {#c-dot-master-equation-thermodynamics}


### D. Cycle analysis {#d-dot-cycle-analysis}


### E. Stochastic thermodynamics {#e-dot-stochastic-thermodynamics}


## IV. Episode 2: Single edge current {#iv-dot-episode-2-single-edge-current}


### A. Main result {#a-dot-main-result}


### B. Dynamics: marginal and hidden {#b-dot-dynamics-marginal-and-hidden}


### C. Thermodynamics: the effective affinity {#c-dot-thermodynamics-the-effective-affinity}


### D. Graphical representation {#d-dot-graphical-representation}


### E. Marginal entropy production rate {#e-dot-marginal-entropy-production-rate}


### F. Stalling {#f-dot-stalling}


### G. Response at stalling {#g-dot-response-at-stalling}


### H. Fluctuation relations for marginal currents {#h-dot-fluctuation-relations-for-marginal-currents}


### I. Fluctuation relations for marginal cycle currents {#i-dot-fluctuation-relations-for-marginal-cycle-currents}


### J. The case of multiple edges {#j-dot-the-case-of-multiple-edges}


## V. Episode 3: Several edge currents {#v-dot-episode-3-several-edge-currents}


### A. Main result {#a-dot-main-result}


### B. Graphical representation {#b-dot-graphical-representation}


### C. Fluctuation relations {#c-dot-fluctuation-relations}


### D. The hierarchy of marginal theories {#d-dot-the-hierarchy-of-marginal-theories}


### E. Stalling and response at stalling {#e-dot-stalling-and-response-at-stalling}


### F. Inequalities between effective affinities {#f-dot-inequalities-between-effective-affinities}


### G. Gauge invariance {#g-dot-gauge-invariance}


### H. Marginally thermodynamic parametrizations {#h-dot-marginally-thermodynamic-parametrizations}


### I. Disconnecting the configuration space {#i-dot-disconnecting-the-configuration-space}


## VI. Episode 4: Phenomenological currents {#vi-dot-episode-4-phenomenological-currents}


### A. Marginal phenomenological currents {#a-dot-marginal-phenomenological-currents}


### B. Marginal consistency {#b-dot-marginal-consistency}


### C. Internal stalling {#c-dot-internal-stalling}


### D. Response {#d-dot-response}


### E. Complete vs. marginal consistency {#e-dot-complete-vs-dot-marginal-consistency}


## VII. Stasimon: a negative result {#vii-dot-stasimon-a-negative-result}


## VIII. Exode: conclusions {#viii-dot-exode-conclusions}
