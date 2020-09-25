+++
title = "Large deviations and dynamical phase transitions in stochastic chemical networks by Lazarescu and Esposito in 2019"
author = ["Cameron Smith"]
lastmod = 2020-09-20T17:35:09-04:00
slug = "Large_deviations_and_dynamical_phase_transitions_in_stochastic_chemical_networks_by_Lazarescu_and_Esposito_in_2019"
draft = false
+++

## [papers]({{< relref "papers" >}}), [stochastic processes]({{< relref "stochastic_processes" >}}), [chemical reaction network theory]({{< relref "chemical_reaction_network_theory" >}}), [large deviations]({{< relref "large_deviations" >}}) {#papers--papers-dot-md--stochastic-processes--stochastic-processes-dot-md--chemical-reaction-network-theory--chemical-reaction-network-theory-dot-md--large-deviations--large-deviations-dot-md}


## I. Introduction {#i-dot-introduction}


### ****Chemical reaction networks**** are ****linear Markov jump processes**** on a ****composition space**** \\[\mathbb{N}^N\\] where \\[N\\] is the number of chemical species. {#chemical-reaction-networks-are-linear-markov-jump-processes-on-a-composition-space-mathbb-n-n-where-n-is-the-number-of-chemical-species-dot}


### We describe the large deviation behavior of generic chemical reaction networks, starting from the chemical master equation74 which describes their microscopic dynamics. This ****paper aims at being pedagogical and self-contained****, and therefore contains many formulae and derivations that are not entirely necessary for practical computations of, say, large deviation functions of time-averaged currents {#we-describe-the-large-deviation-behavior-of-generic-chemical-reaction-networks-starting-from-the-chemical-master-equation74-which-describes-their-microscopic-dynamics-dot-this-paper-aims-at-being-pedagogical-and-self-contained-and-therefore-contains-many-formulae-and-derivations-that-are-not-entirely-necessary-for-practical-computations-of-say-large-deviation-functions-of-time-averaged-currents}


### Section II. we introduce those models, along with a few important concepts to analyze them, and we define the ****mesoscopic variables**** that will be relevant in the ****large-volume limit**** {#section-ii-dot-we-introduce-those-models-along-with-a-few-important-concepts-to-analyze-them-and-we-define-the-mesoscopic-variables-that-will-be-relevant-in-the-large-volume-limit}


### Section III. we ****take the said large-volume limit**** and show that the ****dynamics of those systems can be described through a path integral**** with a Lagrangian that can be computed explicitly. That ****path integral is dominated by a trajectory solving an Euler-Lagrange equation**** or equivalently Hamilton’s equations for an appropriate Hamiltonian. {#section-iii-dot-we-take-the-said-large-volume-limit-and-show-that-the-dynamics-of-those-systems-can-be-described-through-a-path-integral-with-a-lagrangian-that-can-be-computed-explicitly-dot-that-path-integral-is-dominated-by-a-trajectory-solving-an-euler-lagrange-equation-or-equivalently-hamilton-s-equations-for-an-appropriate-hamiltonian-dot}


### Section IV. application of the previously developed formalism to compute the SCGF of currents and densities of the model class under consideration, which is the Legendre transform of the large deviation function of stationary currents and densities. Systems whose deterministic equations have several attractors (i.e., that are multistable) generically undergo first-order dynamical phase transitions around small values of the dynamical biases. {#section-iv-dot-application-of-the-previously-developed-formalism-to-compute-the-scgf-of-currents-and-densities-of-the-model-class-under-consideration-which-is-the-legendre-transform-of-the-large-deviation-function-of-stationary-currents-and-densities-dot-systems-whose-deterministic-equations-have-several-attractors--i-dot-e-dot-that-are-multistable--generically-undergo-first-order-dynamical-phase-transitions-around-small-values-of-the-dynamical-biases-dot}


### Section V. exhibition of a few of those dynamical phase transitions in variants of a simple bistable system called the Schlögl model {#section-v-dot-exhibition-of-a-few-of-those-dynamical-phase-transitions-in-variants-of-a-simple-bistable-system-called-the-schlögl-model}


### Section VI. hands-on summary of how one may compute large deviation functions of dynamical observables in a chemical reaction network, meant as a quick reference or a minimal guide {#section-vi-dot-hands-on-summary-of-how-one-may-compute-large-deviation-functions-of-dynamical-observables-in-a-chemical-reaction-network-meant-as-a-quick-reference-or-a-minimal-guide}


## II. Definition of the microscopic process and observables {#ii-dot-definition-of-the-microscopic-process-and-observables}


### A. Definition of the process {#a-dot-definition-of-the-process}

<!--list-separator-->

-  \\[N\\] species \\[A\_x\\] for \\[x \in [[0, N[[\\]

<!--list-separator-->

-  microscopic state (vector) \\[n\\] with components \\[n\_x\\] given by the number of indistinguishable particles of each species

<!--list-separator-->

-  volume \\[V\\]

<!--list-separator-->

-  chemical reactions whereby a set of reactants is destroyed and replaced by a set of products defines a Markov jump process on the state-space \\[\mathbb{N}^N\\]

<!--list-separator-->

-  \\[\gamma\\] are all sets of particles occurring on either side of a reaction referred to as <span class="underline"><span class="underline">complexes</span></span>

<!--list-separator-->

-  \\[\nu^{\gamma}\_x\\] are <span class="underline"><span class="underline">stoichiometric coefficients</span></span> defining the number of particles of species \\[A\_x\\] in complex \\[\gamma\\]

<!--list-separator-->

-  the reaction destroying complex \\[\gamma\\] and creating complex \\[\gamma'\\] is

    <!--list-separator-->

    -  \\[ \sum\_x \nu^{\gamma}\_x A\_x \rightarrow \sum\_x \nu^{\gamma'}\_x A\_x\\]

<!--list-separator-->

-  the rate at which this reaction occurs from state \\[n\\] is

    <!--list-separator-->

    -  \\[W\_{\gamma, \gamma'} (n)\\]

<!--list-separator-->

-  For stoichiometric vectors \\[\nu^\gamma = \\{ \nu^{\gamma}\_x \\}\\] the difference between states \\[\\{n\_x \\}\\] and \\[\\{n\_x \* \nu^{\gamma}\_x + \nu^{\gamma'}\_x \\}\\] induced by a given reaction from \\[\gamma\\] to \\[\gamma'\\] is defined as a generalized divergence

    <!--list-separator-->

    -  \\[ \nabla\_{\gamma' \gamma} = \nu^{\gamma} \* \nu^{\gamma'}\\] a matrix that acts on functions of reactions and yields a variation of particle number

        <!--list-separator-->

        -  \\[ (\nabla \lambda)\_x = \sum\_{\gamma' \gamma} (\nu^{\gamma}\_x \* \nu^{\gamma'}\_x) \lambda\_{\gamma' \gamma} \\]

        <!--list-separator-->

        -  \\[\nabla = \nu \mathfrak{d}\\]

            <!--list-separator-->

            -  \\[\mathfrak{d}\\] is the discrete divergence on the graph of complexes (incidence matrix) where \\[\mathfrak{d}\_{\gamma' \gamma} = \delta\_{\gamma} \* \delta\_{\gamma'}\\]

            <!--list-separator-->

            -  \\[\nu\\] is the matrix containing stoichiometric coefficients acting on complexes and yielding particle numbers

    <!--list-separator-->

    -  \\[(\nabla f)\_{\gamma' \gamma} = \sum\_x (\nu^{\gamma'}\_x \* \nu^{\gamma}\_x)f\_x\\] is the conjugate gradient mapping functions of the species to antisymmetric functions of the reactions

<!--list-separator-->

-  Master equation

    <!--list-separator-->

    -  \\[d\_t P(n) = \sum\_{\gamma' \gamma} W\_{\gamma' \gamma}(n + \nabla\_{\gamma' , \gamma}) P(n + \nabla\_{\gamma', \gamma}) \* W\_{\gamma' \gamma} (n) P(n)\\]

    <!--list-separator-->

    -  \\[d\_t  | P \rangle = W | P \rangle\\]

        <!--list-separator-->

        -  \\[W = \sum\_{\gamma' , \gamma , n} W\_{\gamma' \gamma} (n) | n \* \nabla\_{\gamma' , \gamma} \rangle \langle n | \* W\_{\gamma' \gamma} (n) | n \rangle \langle n |\\]

    <!--list-separator-->

    -  \\[W\_{\gamma' \gamma} (n) = k\_{\gamma' \gamma} \prod\_x \frac{[n\_x]!}{[n\_x \* \nu^{\gamma}\_{x}]!} V^{1-\sum\_x \nu^{\gamma}\_x}\\] is the <span class="underline"><span class="underline">mass action</span></span> prescription where the dependence on \\[n\\] comes from the number of ways to choose the reactants for the complex serving as input to a reaction with <span class="underline"><span class="underline">kinetic constant</span></span> \\[k\_{\gamma' \gamma}\\] independent of \\[n\\] and \\[V\\]

    <!--list-separator-->

    -


### B. Time-additive dynamical observables {#b-dot-time-additive-dynamical-observables}


### C. A caveat on conserved quantities {#c-dot-a-caveat-on-conserved-quantities}


### D. Example {#d-dot-example}


### E. Aside: Long-time large deviations {#e-dot-aside-long-time-large-deviations}


## III. Dynamical large deviation formalism {#iii-dot-dynamical-large-deviation-formalism}


### A. Standard formalism {#a-dot-standard-formalism}

<!--list-separator-->

-  1. Standard Lagrangian

<!--list-separator-->

-  2. Equations of motion

<!--list-separator-->

-  3. Standard Hamiltonian and Hamilton's equations

<!--list-separator-->

-  4. Two-field picture


### B. Detailed formalism {#b-dot-detailed-formalism}

<!--list-separator-->

-  1. Detailed Lagrangian

<!--list-separator-->

-  2. Equations of motion

<!--list-separator-->

-  3. Detailed Hamiltonian and Hamilton's detailed equations


### C. Biased formalism {#c-dot-biased-formalism}

<!--list-separator-->

-  1. Detailed biased dynamics

<!--list-separator-->

-  2. Contraction of the currents and two-field picture


## IV. Stationary large deviations and dynamical phase transitions {#iv-dot-stationary-large-deviations-and-dynamical-phase-transitions}


### A. Boundary conditions {#a-dot-boundary-conditions}


### B. Density-phase picture and global Hamiltonian attractors {#b-dot-density-phase-picture-and-global-hamiltonian-attractors}


### C. Conserved quantities in the two-field picture {#c-dot-conserved-quantities-in-the-two-field-picture}


### D. Generic dynamical phase transitions for multistable systems {#d-dot-generic-dynamical-phase-transitions-for-multistable-systems}


## V. A few examples of dynamical phase transitions {#v-dot-a-few-examples-of-dynamical-phase-transitions}


### A. Schlogl model {#a-dot-schlogl-model}


### B. Generalized Schlogl model {#b-dot-generalized-schlogl-model}


### C. Runaway Schlogl model {#c-dot-runaway-schlogl-model}


## VI. Practical summary of formulae and results {#vi-dot-practical-summary-of-formulae-and-results}


## VII. Conclusion {#vii-dot-conclusion}


## Appendix: Computations of the chemical Lagrangians and Hamiltonians {#appendix-computations-of-the-chemical-lagrangians-and-hamiltonians}
