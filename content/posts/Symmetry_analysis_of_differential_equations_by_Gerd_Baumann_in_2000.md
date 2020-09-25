+++
title = "Symmetry analysis of differential equations by Gerd Baumann in 2000"
author = ["Cameron Smith"]
lastmod = 2020-09-20T17:36:02-04:00
slug = "Symmetry_analysis_of_differential_equations_by_Gerd_Baumann_in_2000"
draft = false
+++

## 1. Introduction {#1-dot-introduction}


### Symmetry principles ... summarize the regularities of the laws that are independent of the specific details of a particular instantiation of a system's dynamics. {#symmetry-principles-dot-dot-dot-summarize-the-regularities-of-the-laws-that-are-independent-of-the-specific-details-of-a-particular-instantiation-of-a-system-s-dynamics-dot}


### So-called <span class="underline"><span class="underline">laws of nature</span></span> provide a structure and coherence to the set of events. <span class="underline"><span class="underline">Invariance principles</span></span>, in turn, provide a structure and coherence to the laws of nature. {#so-called-in-turn-provide-a-structure-and-coherence-to-the-laws-of-nature-dot}


### \_\_Invariance of the laws of nature under space-time translations\_\_ is precisely what is the same about otherwise equivalent experiments performed at different times and places. {#invariance-of-the-laws-of-nature-under-space-time-translations-is-precisely-what-is-the-same-about-otherwise-equivalent-experiments-performed-at-different-times-and-places-dot}


### For every <span class="underline"><span class="underline">global continuous symmetry</span></span> there is an associated time-independent quantity which was proved in 1918 by Emmy Noether and is known as <span class="underline"><span class="underline">Noether's theorem</span></span>. {#for-every-dot}


### From 1872-1899, Sophus Lie developed the theory that places symmetry at the top of the hierarchy of features of nature that constrain the space of allowable dynamical laws. {#from-1872-1899-sophus-lie-developed-the-theory-that-places-symmetry-at-the-top-of-the-hierarchy-of-features-of-nature-that-constrain-the-space-of-allowable-dynamical-laws-dot}


### Symmetry analysis is a rare theory in that it allows for the derivation of solutions to differential equations in a completely algorithmic way. {#symmetry-analysis-is-a-rare-theory-in-that-it-allows-for-the-derivation-of-solutions-to-differential-equations-in-a-completely-algorithmic-way-dot}


### "The older examinations of ordinary differential equations as found in standard books are not systematic ... the mathematicians did not realize that the special theories for different classes of differential equations are all contained in the theory of infinitesimal transformations" from <span class="underline"><span class="underline">Differentialgleichungen</span></span> by Sophus Lie in 1891 {#the-older-examinations-of-ordinary-differential-equations-as-found-in-standard-books-are-not-systematic-dot-dot-dot-the-mathematicians-did-not-realize-that-the-special-theories-for-different-classes-of-differential-equations-are-all-contained-in-the-theory-of-infinitesimal-transformations-from-by-sophus-lie-in-1891}


### One of the deficiencies of Lie's theory is the tremendous amount of work necessary to derive a solution of a particular differential equation ... but today we can overcome this problem of rote manual algebraic manipulation via computer algebra systems. {#one-of-the-deficiencies-of-lie-s-theory-is-the-tremendous-amount-of-work-necessary-to-derive-a-solution-of-a-particular-differential-equation-dot-dot-dot-but-today-we-can-overcome-this-problem-of-rote-manual-algebraic-manipulation-via-computer-algebra-systems-dot}


### The fundamentals are based on invariance of the equations of motion to transformations of independent and dependent variables in a manner that forms a local group of point transformations that correspond to a diffeomorphism on the space of independent and dependent variables that maps solutions to solutions. {#the-fundamentals-are-based-on-invariance-of-the-equations-of-motion-to-transformations-of-independent-and-dependent-variables-in-a-manner-that-forms-a-local-group-of-point-transformations-that-correspond-to-a-diffeomorphism-on-the-space-of-independent-and-dependent-variables-that-maps-solutions-to-solutions-dot}


### Outline of the book {#outline-of-the-book}

<!--list-separator-->

-  Chapter 2: description of Lie groups and Lie algebras

<!--list-separator-->

-  Chapter 3: fundamental aspects of derivatives and their definitions

<!--list-separator-->

-  Chapter 4: application of Lie's integration theory in connection with point symmetries

<!--list-separator-->

-  Chapter 5: point symmetries of partial differential equations

<!--list-separator-->

-  Chapter 6: non-classical symmetries

<!--list-separator-->

-  Chapter 7: potential symmetries

<!--list-separator-->

-  Chapter 8: approximate symmetries

<!--list-separator-->

-  Chapter 9: generalized symmetries

<!--list-separator-->

-  Chapter 10: automatic solution of a system of overdetermined equations


## 2. Elements of symmetry analysis {#2-dot-elements-of-symmetry-analysis}


### Outline {#outline}

<!--list-separator-->

-  Lie groups are connected to their Lie algebras which are closely related to vector fields


### 2.1 Groups and Lie groups {#2-dot-1-groups-and-lie-groups}

<!--list-separator-->

-  2.1.1 Groups

<!--list-separator-->

-  2.1.2 Isomorphism

<!--list-separator-->

-  2.1.3 Lie groups

    <!--list-separator-->

    -  A Lie group is a group that also carries the structure necessary to qualify as a manifold

    <!--list-separator-->

    -  The global study of a Lie group may be reduced to its local study and the study of the local structure can be reduced to the study of the infinitesimal structure


### 2.2 Lie algebras {#2-dot-2-lie-algebras}

<!--list-separator-->

-  The study of a Lie group, \\[\mathfrak{G}\\], may be simplified by considering the tangent space \\[V\\] of \\[\mathfrak{G}\\] around the identity of the group. The tangent space is called a <span class="underline"><span class="underline">Lie algebra</span></span>

<!--list-separator-->

-  2.2.1 Representation of a Lie algebra

    <!--list-separator-->

    -  A representation of a Lie algebra \\[\mathfrak{g}\\] on a vector space \\[V\\] is a mapping \\[\rho\\] from \\[\mathfrak{g}\\] to a linear transformation of \\[V\\]

    <!--list-separator-->

    -  The basis elements of a Lie algebra are also called vector fields

    <!--list-separator-->

    -  the [structure constants](<https://en.wikipedia.org/wiki/Structure%5Fconstants>) of an algebra over a field are used to explicitly specify the product of two basis vectors in the algebra as a linear combination.

<!--list-separator-->

-  2.2.2 Properties of Lie algebras

    <!--list-separator-->

    -  properties of Lie algebras useful in the classification of the solutions of differential equations

        <!--list-separator-->

        -  derived algebra

            <!--list-separator-->

            -  The first derived algebra of Lie algebra \\[V\\] is \\[V^{(1)} = [V,V]\\], which is an ideal by construction

            <!--list-separator-->

            -  Higher-order derived algebras \\[V^{(n+1)} = [V^{(n)},V^{(n)}], n = 1,2,3, \ldots\\]

        <!--list-separator-->

        -  derivation of an algebra

            <!--list-separator-->

            -  a derivation \\[\mathfrak{D}\\] of a Lie algebra \\[V\\] is a linear mapping of \\[V\\] into itself satisfying \\[\mathfrak{D} ([\vec{v}, \vec{w}]) = [\mathfrak{D}(\vec{v}), \vec{w}] + [\vec{v}, \mathfrak{D}(\vec{w})] \\]

            <!--list-separator-->

            -  the commutator of two distinct derivations is also a derivation

        <!--list-separator-->

        -  adjoint algebra

            <!--list-separator-->

            -  Consider the linear map \\[\mathrm{ad} \vec{v}\\] of \\[V\\] onto itself given by \\[\mathrm{ad} \vec{v} (\vec{w}) := [\vec{v}, \vec{w}]\\], which is a derivation of \\[V\\]

            <!--list-separator-->

            -  The kernel of the homomorphism \\[\phi \colon \vec{v} \rightarrow \mathrm{ad} \vec{v} \\] is the center of \\[V\\]

            <!--list-separator-->

            -  the representation of \\[\mathrm{ad} \vec{v}\\] called the adjoint representation of the Lie algebra provide a matrix representation of the algebra

            <!--list-separator-->

            -  if we know the structure constants of a Lie algebra, we also know the matrix representation of the adjoint Lie algebra

        <!--list-separator-->

        -  Killing form

            <!--list-separator-->

            -  A symmetric bilinear form \\[\langle \vec{v}, \vec{w} \rangle = \mathrm{Tr}(\mathrm{ad} \vec{v} \mathrm{ad} \vec{w})\\]

            <!--list-separator-->

            -  This can be written in terms of the Cartan metric tensor of the Lie algebra \\[ g\_{lm} = \sum\_{i,k=1}^{n} c^{i}\_{lk}c^{k}\_{mi}\\]

            <!--list-separator-->

            -

        <!--list-separator-->

        -  solvability

            <!--list-separator-->

            -  Lie algebra \\[V\\] is solvable if \\[V^{(n)} = 0\\] for some \\[n \gt 0\\]

                <!--list-separator-->

                -  simplest examples are just those Lie algebras that are commutative so that \\[V^{(1)} = 0\\]

            <!--list-separator-->

            -  If a Lie algebra is solvable, then the related differential equation can be solved

            <!--list-separator-->

            -  The six-dimensional Lie algebra of the diffusion equation is not solvable because the first derived Lie algebra contains all operators of the six-dimensional Lie algebra

            <!--list-separator-->

            -  The Lie algebra given by the vector fields for the Korteweg-de Vries (KdV) equation is solvable


## 3. Derivatives {#3-dot-derivatives}


### Outline {#outline}

<!--list-separator-->

-  The basis of the symmetry analysis of differential equations is the prolongation; however this is not implemented in <span class="underline"><span class="underline">Mathematica</span></span>


### 3.1 Ordinary and partial derivatives {#3-dot-1-ordinary-and-partial-derivatives}


### 3.2 Tangent vector {#3-dot-2-tangent-vector}


### 3.3 The total derivative {#3-dot-3-the-total-derivative}


### 3.4 Prolongations {#3-dot-4-prolongations}


### 3.5 The Frechet derivative {#3-dot-5-the-frechet-derivative}


### 3.6 The Euler derivative {#3-dot-6-the-euler-derivative}

<!--list-separator-->

-  3.6.1 The problem of variation

<!--list-separator-->

-  3.6.2 Euler's equation

<!--list-separator-->

-  3.6.3 Euler operator

<!--list-separator-->

-  3.6.4 Algorithm used in the calculus of variations

<!--list-separator-->

-  3.6.5 Euler operator for <span class="underline"><span class="underline">q</span></span> dependent variables

<!--list-separator-->

-  3.6.6 Euler operator for <span class="underline"><span class="underline">q+p</span></span> dimensions


### 3.7 Prolongation of vector fields {#3-dot-7-prolongation-of-vector-fields}


## 4. Symmetries of ordinary differential equations {#4-dot-symmetries-of-ordinary-differential-equations}


### 4.1 Introduction {#4-dot-1-introduction}


### 4.2 Symmetry transformations of functions {#4-dot-2-symmetry-transformations-of-functions}

<!--list-separator-->

-  4.2.1 Symmetries

<!--list-separator-->

-  4.2.2 Infinitesimal transformations

<!--list-separator-->

-  4.2.3 Group invariants

<!--list-separator-->

-  4.2.4 Tangent vector

<!--list-separator-->

-  4.2.5 Prolongation of transformations


### 4.3 Symmetry transformations of differential equations {#4-dot-3-symmetry-transformations-of-differential-equations}

<!--list-separator-->

-  4.3.1 Definition of a symmetry group

<!--list-separator-->

-  4.3.2 Main properties of symmetry groups

<!--list-separator-->

-  4.3.3 Calculation of the infinitesimal symmetries

<!--list-separator-->

-  4.3.4 Canonical variables


### 4.4 Analysis of ordinary differential equations {#4-dot-4-analysis-of-ordinary-differential-equations}

<!--list-separator-->

-  4.4.1 First-order equations

<!--list-separator-->

-  4.4.2 Second-order ordinary differential equations

<!--list-separator-->

-  4.4.3 Higher-order ordinary differential equations


## 5. Point symmetries of partial differential equations {#5-dot-point-symmetries-of-partial-differential-equations}


### 5.1 Introduction {#5-dot-1-introduction}


### 5.2 Lie's theory used in <span class="underline"><span class="underline">MathLie</span></span> {#5-dot-2-lie-s-theory-used-in}


### 5.3 Invariance based on Frechet derivatives {#5-dot-3-invariance-based-on-frechet-derivatives}


### 5.4 Application of the theory {#5-dot-4-application-of-the-theory}

<!--list-separator-->

-  5.4.1 Calculation of prolongations

<!--list-separator-->

-  5.4.2 Derivation of determining equations

<!--list-separator-->

-  5.4.3 Interactive solution of determining equations

<!--list-separator-->

-  5.4.4 Data basis of symmetries


### 5.5 Similarity reduction of partial differential equations {#5-dot-5-similarity-reduction-of-partial-differential-equations}


### 5.6 Working examples {#5-dot-6-working-examples}

<!--list-separator-->

-  5.6.1 The diffusion equation

<!--list-separator-->

-  5.6.2 The earthworm's new year problem

<!--list-separator-->

-  5.6.3 Single flux line in superconductors

<!--list-separator-->

-  5.6.4 The Korteweg-de Vries Equation and its generalizations

<!--list-separator-->

-  5.6.6 Two-dimensional boundary layer flows: group classification

<!--list-separator-->

-  5.6.7 The plane jet

<!--list-separator-->

-  5.6.8 Drop formation

<!--list-separator-->

-  5.6.9 The Rayleigh particle

<!--list-separator-->

-  5.6.10 Molecular beam epitaxy

<!--list-separator-->

-  5.6.11 The first atomic explosion


## 6. Non-classical symmetries of partial differential equations {#6-dot-non-classical-symmetries-of-partial-differential-equations}


### 6.1 Introduction {#6-dot-1-introduction}


### 6.2 Mathematical background of the non-classical method {#6-dot-2-mathematical-background-of-the-non-classical-method}


### 6.3 Applications of the non-classical method {#6-dot-3-applications-of-the-non-classical-method}

<!--list-separator-->

-  6.3.1 The heat equation

<!--list-separator-->

-  6.3.2 The Boussinesq eqaution

<!--list-separator-->

-  6.3.3 The Fokker-Planck equation


## 7. Potential symmetries of partial differential equations {#7-dot-potential-symmetries-of-partial-differential-equations}


### 7.1 Introduction {#7-dot-1-introduction}


### 7.2 Basics of potential symmetries {#7-dot-2-basics-of-potential-symmetries}


### 7.3 Calculation of potential symmetries {#7-dot-3-calculation-of-potential-symmetries}


### 7.4 Applications of potential symmetries {#7-dot-4-applications-of-potential-symmetries}

<!--list-separator-->

-  7.4.1 A non-linear reaction diffusion equation

<!--list-separator-->

-  7.4.2 Cylindrical Korteweg-de Vries equation

<!--list-separator-->

-  7.4.3 The Burgers equation


## 8. Approximate symmetries of partial differential equations {#8-dot-approximate-symmetries-of-partial-differential-equations}


### 8.1 Introduction {#8-dot-1-introduction}


### 8.2 Approximations {#8-dot-2-approximations}


### 8.3 One-parameter approximation group {#8-dot-3-one-parameter-approximation-group}


### 8.4 Approximate group generator {#8-dot-4-approximate-group-generator}


### 8.5 The determining equations and an algorithm of calculation {#8-dot-5-the-determining-equations-and-an-algorithm-of-calculation}


### 8.6 Examples {#8-dot-6-examples}

<!--list-separator-->

-  8.6.1 Isentropic liquid

<!--list-separator-->

-  8.6.2 Perturbed Korteweg-de Vries equation


## 9. Generalized symmetries {#9-dot-generalized-symmetries}


### 9.1 Introduction {#9-dot-1-introduction}


### 9.2 Elements of generalized symmetries {#9-dot-2-elements-of-generalized-symmetries}


### 9.3 Algorithm for calculation of generalized symmetries {#9-dot-3-algorithm-for-calculation-of-generalized-symmetries}


### 9.4 Examples {#9-dot-4-examples}

<!--list-separator-->

-  9.4.1 Diffusion equation

<!--list-separator-->

-  9.4.2 Potential Burgers equation

<!--list-separator-->

-  9.4.3 Generalized Korteweg-de Vries equations

<!--list-separator-->

-  9.4.4 Coupled system of wave equations


### 9.5 Second-order ODEs and the Euler-Lagrange equation {#9-dot-5-second-order-odes-and-the-euler-lagrange-equation}

<!--list-separator-->

-  9.5.1 Generalized symmetries and second-order ODEs

<!--list-separator-->

-  9.5.2 Conservation laws


### 9.6 Algorithm for conservation laws of second-order ODEs {#9-dot-6-algorithm-for-conservation-laws-of-second-order-odes}


### 9.7 Examples for second-order ODEs {#9-dot-7-examples-for-second-order-odes}

<!--list-separator-->

-  9.7.1 The Henon-Heiles model

<!--list-separator-->

-  9.7.2 Two-dimensional quartic oscillators

<!--list-separator-->

-  9.7.3 Two ions in a trap


## 10. Solution of coupled linear partial differential equations {#10-dot-solution-of-coupled-linear-partial-differential-equations}


### 10.1 Introduction {#10-dot-1-introduction}


### 10.2 General canonical form of PDEs {#10-dot-2-general-canonical-form-of-pdes}

<!--list-separator-->

-  10.2.1 Application of the general canonical form algorithm


### 10.3 Solution of linear PDEs {#10-dot-3-solution-of-linear-pdes}

<!--list-separator-->

-  10.3.1 Integration of monomials

<!--list-separator-->

-  10.3.2 Integrating ODEs and pseudo-ODEs

<!--list-separator-->

-  10.3.3 Integrating exact PDEs

<!--list-separator-->

-  10.3.4 Potential representation


### 10.4 Simplification of equations {#10-dot-4-simplification-of-equations}

<!--list-separator-->

-  10.4.1 Direct separation

<!--list-separator-->

-  10.4.2 Indirect separation

<!--list-separator-->

-  10.4.3 Reducing the number of dependent variables


### 10.5 Example {#10-dot-5-example}

<!--list-separator-->

-  10.5.1 Liouville-type equation of quantum gravity theory


## 11. Appendix {#11-dot-appendix}


### A. Marius Sophus Lie {#a-dot-marius-sophus-lie}


### B. List of key symbols used in <span class="underline"><span class="underline">Mathematica</span></span> {#b-dot-list-of-key-symbols-used-in}


### C. Installing <span class="underline"><span class="underline">MathLie</span></span> {#c-dot-installing}
