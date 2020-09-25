+++
title = "A free energy principle for a particular physics by Karl Friston in 2019"
author = ["Cameron Smith"]
lastmod = 2020-09-20T17:33:39-04:00
slug = "A_free_energy_principle_for_a_particular_physics_by_Karl_Friston_in_2019"
draft = false
+++

## [variational inference]({{< relref "variational_inference" >}}) {#variational-inference--variational-inference-dot-md}


## 0. Introduction {#0-dot-introduction}


### We assume that for something to exist it must possess (internal or intrinsic) states that can be separated statistically from (external or extrinsic) states that do not constitute the thing. {#we-assume-that-for-something-to-exist-it-must-possess--internal-or-intrinsic--states-that-can-be-separated-statistically-from--external-or-extrinsic--states-that-do-not-constitute-the-thing-dot}


### the states of things (i.e., particles) comprise mixtures of blanket states, where the Markov blanket surrounds things at a smaller scale {#the-states-of-things--i-dot-e-dot-particles--comprise-mixtures-of-blanket-states-where-the-markov-blanket-surrounds-things-at-a-smaller-scale}


### the Langevin formulation of dynamics – at any given spatiotemporal scale – can be decomposed into an ensemble of Markov blankets. These blanket states have a dynamics at a higher scale with exactly the same (Langevin) form as the dynamics of the original scale. When lifting the dynamics from one scale to the next, internal states are effectively eliminated, leaving only slow, macroscopic dynamics of blanket states. These become the states of things at the next level, which have their own Markov blankets and so on. The endpoint of this formalism is a description of everything at progressively higher spatial and temporal scales. The implicit separation of temporal scales is used in subsequent sections to examine the sorts of dynamics, physics or mechanics of progressively larger things. {#the-langevin-formulation-of-dynamics-at-any-given-spatiotemporal-scale-can-be-decomposed-into-an-ensemble-of-markov-blankets-dot-these-blanket-states-have-a-dynamics-at-a-higher-scale-with-exactly-the-same--langevin--form-as-the-dynamics-of-the-original-scale-dot-when-lifting-the-dynamics-from-one-scale-to-the-next-internal-states-are-effectively-eliminated-leaving-only-slow-macroscopic-dynamics-of-blanket-states-dot-these-become-the-states-of-things-at-the-next-level-which-have-their-own-markov-blankets-and-so-on-dot-the-endpoint-of-this-formalism-is-a-description-of-everything-at-progressively-higher-spatial-and-temporal-scales-dot-the-implicit-separation-of-temporal-scales-is-used-in-subsequent-sections-to-examine-the-sorts-of-dynamics-physics-or-mechanics-of-progressively-larger-things-dot}


### Organization {#organization}

<!--list-separator-->

-  part 1: basic results

    <!--list-separator-->

    -  constraints on the dynamics of Markov blankets that possess measurable characteristics

    <!--list-separator-->

    -  ****measurability as a constraint**** requires the existence of an invariant measure (in the sense of Ergodic theory) over sufficiently long periods of time within the context of the dynamics of the system under consideration

        <!--list-separator-->

        -  Consider a measurable space \\[(X, \Sigma)\\]

            <!--list-separator-->

            -  Example

                <!--list-separator-->

                -  Let \\[X = \\{ 1, 2, 3 \\}\\] and let \\[\Sigma = \mathcal{P}(X)\\]

                <!--list-separator-->

                -  Let \\[X = \\{ 1, 2, 3 \\}\\] and let \\[\Sigma = \\{ X, \emptyset \\}\\]

        <!--list-separator-->

        -  A function \\[\mu \colon \Sigma \rightarrow \mathbb{R}\\] is a measure if it satisfies

            <!--list-separator-->

            -  non-negativity, null set-maps-to-zero, and countable additivity

        <!--list-separator-->

        -  Let \\[f \colon X \rightarrow X\\] be a measurable function on the measurable space \\[(X, \Sigma)\\]. A measure \\[\mu\\] is invariant under \\[f\\] if \\[\forall A \in \Sigma\\], \\[\mu(f^{-1}(A))= \mu(A)\\]

        <!--list-separator-->

        -  general invariant measures can be formulated in terms of the push forward as

            <!--list-separator-->

            -  \\[ f\_\* (\mu) = \mu \\]

        <!--list-separator-->

        -  the collection of invariant measures on \\[X\\] with respect to a given function \\[f\\] is denoted \\[M\_f(X)\\]

    <!--list-separator-->

    -

<!--list-separator-->

-  part 2: apply basic results to limiting cases of dynamical systems to recover quantum, statistical, and classical mechanics

<!--list-separator-->

-  part 3: special case of active systems in terms of \`Bayesian mechanics\` for particles with internal states that correlate with the distribution of interactions those particles have with their respective environments


## 1. The setup {#1-dot-the-setup}


### 1.1 Something or nothing {#1-dot-1-something-or-nothing}

<!--list-separator-->

-  Some preliminaries

    <!--list-separator-->

    -  Langevin

    <!--list-separator-->

    -  Path integral

    <!--list-separator-->

    -  Fokker-Planck

<!--list-separator-->

-  Nonequilibrium steady states

    <!--list-separator-->

    -  the action of any path can be expressed in terms of a motion-dependent (kinetic) term, a (path\* independent) term – that depends upon the change in surprisal – and a (path-dependent) term that scales with the amplitude of random fluctuations

<!--list-separator-->

-  Fluctuations and information length

    <!--list-separator-->

    -

<!--list-separator-->

-  [random dynamical systems]({{< relref "random_dynamical_systems" >}}) and Markov blankets

<!--list-separator-->

-  Markov blankets and marginal

<!--list-separator-->

-  Summary


### 1.2 Symmetry breaking and self-organization {#1-dot-2-symmetry-breaking-and-self-organization}

<!--list-separator-->

-  Self-organization and self-evidencing

<!--list-separator-->

-  Self-organization, frustration, and supersymmetry

<!--list-separator-->

-  Self-organization and information length


### 1.3 Synthetic soups and active matter {#1-dot-3-synthetic-soups-and-active-matter}

<!--list-separator-->

-  An active soup

<!--list-separator-->

-  A random dynamical attractor and its Markov blankets

<!--list-separator-->

-  The Markov blanket

<!--list-separator-->

-  The emergence of order

<!--list-separator-->

-  Summary


### 1.4 States, particles, and fluctuations {#1-dot-4-states-particles-and-fluctuations}

<!--list-separator-->

-  Starting at the end

<!--list-separator-->

-  The Markovian partition

<!--list-separator-->

-  The adiabatic reduction

<!--list-separator-->

-  Elimination and renormalization

<!--list-separator-->

-  Summary


## 2. Some special cases {#2-dot-some-special-cases}


### 2.1 A theory of small things \* quantum mechanics {#2-dot-1-a-theory-of-small-things-quantum-mechanics}

<!--list-separator-->

-  The Schrodinger equation from first principles

<!--list-separator-->

-  Wave particle duality and the de Broglie hypothesis

<!--list-separator-->

-  Heisenberg uncertainty principle

<!--list-separator-->

-  Inference, measurement and wave function collapse?

<!--list-separator-->

-  Summary


### 2.2 A theory of lots of little things \* statistical mechanics {#2-dot-2-a-theory-of-lots-of-little-things-statistical-mechanics}

<!--list-separator-->

-  Stochastic thermodynamics

<!--list-separator-->

-  Stochastic energetics

<!--list-separator-->

-  Fluctuation theorems

<!--list-separator-->

-  Summary


### 2.3 A theory of big things \* classical mechanics {#2-dot-3-a-theory-of-big-things-classical-mechanics}

<!--list-separator-->

-  Conservative systems

<!--list-separator-->

-  Random fluctuations and generalized motion

<!--list-separator-->

-  Summary


## 3. A particular case {#3-dot-a-particular-case}


### 3.1 A theory of autonomous things \* Bayesian mechanics {#3-dot-1-a-theory-of-autonomous-things-bayesian-mechanics}

<!--list-separator-->

-  Risk and ambiguity

<!--list-separator-->

-  Inference and measurement

<!--list-separator-->

-  Information geometry

<!--list-separator-->

-  Variational Bayes

<!--list-separator-->

-  Summary


### 3.2 Simulating sentience {#3-dot-2-simulating-sentience}

<!--list-separator-->

-  The representation of order

<!--list-separator-->

-  Summary


### 3.3 Active inference and self-evidencing {#3-dot-3-active-inference-and-self-evidencing}

<!--list-separator-->

-  Active inference with continuous states

<!--list-separator-->

-  Active inference with discrete states

<!--list-separator-->

-  Deep inference: gradient flows or least action?

<!--list-separator-->

-  Summary


### 3.4 The thermodynamics of inference {#3-dot-4-the-thermodynamics-of-inference}

<!--list-separator-->

-  Potentials and surprisal

<!--list-separator-->

-  Ensemble free energies

<!--list-separator-->

-  Summary


### Discussion {#discussion}

<!--list-separator-->

-  Conclusion


## Appendices {#appendices}


### A. Stratonovich path integrals {#a-dot-stratonovich-path-integrals}


### B. Lemmas and proofs {#b-dot-lemmas-and-proofs}


### C. Nonequilibrium steady-state energy functions {#c-dot-nonequilibrium-steady-state-energy-functions}


### D. the Fokker-Planck operator {#d-dot-the-fokker-planck-operator}


### E. Generalized motion {#e-dot-generalized-motion}


### F. Discrete state-space models {#f-dot-discrete-state-space-models}
