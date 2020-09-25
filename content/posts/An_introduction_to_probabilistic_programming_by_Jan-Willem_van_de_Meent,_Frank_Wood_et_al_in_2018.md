+++
title = "An introduction to probabilistic programming by Jan-Willem van de Meent, Frank Wood et al in 2018"
author = ["Cameron Smith"]
lastmod = 2020-09-20T17:33:44-04:00
slug = "An_introduction_to_probabilistic_programming_by_Jan-Willem_van_de_Meent,_Frank_Wood_et_al_in_2018"
draft = false
+++

## [probabilistic programming]({{< relref "probabilistic_programming" >}}), [probabilistic inference]({{< relref "probabilistic_inference" >}}), [programming languages]({{< relref "programming_languages" >}}), [logic]({{< relref "logic" >}}), [Frank Wood]({{< relref "Frank_Wood" >}}) {#probabilistic-programming--probabilistic-programming-dot-md--probabilistic-inference--probabilistic-inference-dot-md--programming-languages--programming-languages-dot-md--logic--logic-dot-md--frank-wood--frank-wood-dot-md}


## citation {#citation}


### van de Meent, J.-W., Paige, B., Yang, H., & Wood, F. (2018). An Introduction to Probabilistic Programming. Retrieved from <http://arxiv.org/abs/1809.10756> {#van-de-meent-j-dot-w-dot-paige-b-dot-yang-h-dot-and-wood-f-dot--2018--dot-an-introduction-to-probabilistic-programming-dot-retrieved-from-http-arxiv-dot-org-abs-1809-dot-10756}


## contents {#contents}


### 0. Abstract {#0-dot-abstract}

<!--list-separator-->

-  We start with a discussion of model-based reasoning and explain why conditioning as a foundational computation is central to the fields of probabilistic machine learning and artificial intelligence.

<!--list-separator-->

-  a simple first-order probabilistic programming language (PPL) whose programs define static-computation-graph, finite-variable\* cardinality models

<!--list-separator-->

-  a higher-order probabilistic programming language, with a functionality analogous to that of established programming languages

<!--list-separator-->

-  models with dynamic computation graphs, at the cost of requiring inference methods that generate samples by repeatedly executing the program

<!--list-separator-->

-  interface between program executions and an inference controller


### 1. Introduction {#1-dot-introduction}

<!--list-separator-->

-  1.1 Model-based Reasoning . . . . . . . . . . . . . . . . . . . 10

<!--list-separator-->

-  1.2 Probabilistic Programming . . . . . . . . . . . . . . . . . 21

<!--list-separator-->

-  1.3 Example Applications . . . . . . . . . . . . . . . . . . . . 26

<!--list-separator-->

-  1.4 A First Probabilistic Program . . . . . . . . . . . . . . . . 29


### 2. A probabilistic programming language without recursion {#2-dot-a-probabilistic-programming-language-without-recursion}

<!--list-separator-->

-  2.1 Syntax . . . . . . . . . . . . . . . . . . . . . . . . . . . . 32

<!--list-separator-->

-  2.2 Syntactic Sugar . . . . . . . . . . . . . . . . . . . . . . . 37

<!--list-separator-->

-  2.3 Examples . . . . . . . . . . . . . . . . . . . . . . . . . . . 42

<!--list-separator-->

-  2.4 A Simple Purely Deterministic Language . . . . . . . . . . 48


### 3. Graph-based inference {#3-dot-graph-based-inference}

<!--list-separator-->

-  3.1 Compilation to a Graphical Model . . . . . . . . . . . . . 51

<!--list-separator-->

-  3.2 Evaluating the Density . . . . . . . . . . . . . . . . . . . 66

<!--list-separator-->

-  3.3 Gibbs Sampling . . . . . . . . . . . . . . . . . . . . . . . 74

<!--list-separator-->

-  3.4 Hamiltonian Monte Carlo . . . . . . . . . . . . . . . . . . 80

<!--list-separator-->

-  3.5 Compilation to a Factor Graph . . . . . . . . . . . . . . . 89

<!--list-separator-->

-  3.6 Expectation Propagation . . . . . . . . . . . . . . . . . . 94


### 4. Evaluation-based inference I {#4-dot-evaluation-based-inference-i}

<!--list-separator-->

-  4.1 Likelihood Weighting . . . . . . . . . . . . . . . . . . . . 105

<!--list-separator-->

-  4.2 Metropolis-Hastings . . . . . . . . . . . . . . . . . . . . . 116

<!--list-separator-->

-  4.3 Sequential Monte Carlo . . . . . . . . . . . . . . . . . . . 125

<!--list-separator-->

-  4.4 Black Box Variational Inference . . . . . . . . . . . . . . . 131


### 5. A probabilistic programming language with recursion {#5-dot-a-probabilistic-programming-language-with-recursion}

<!--list-separator-->

-  5.1 Syntax . . . . . . . . . . . . . . . . . . . . . . . . . . . . 142

<!--list-separator-->

-  5.2 Syntactic sugar . . . . . . . . . . . . . . . . . . . . . . . 143

<!--list-separator-->

-  5.3 Examples . . . . . . . . . . . . . . . . . . . . . . . . . . . 144


### 6. Evaluation-based inference II {#6-dot-evaluation-based-inference-ii}

<!--list-separator-->

-  6.1 Explicit separation of model and inference code . . . . . . 156

<!--list-separator-->

-  6.2 Addressing Transformation . . . . . . . . . . . . . . . . . 161

<!--list-separator-->

-  6.3 Continuation-Passing-Style Transformation . . . . . . . . . 165

<!--list-separator-->

-  6.4 Message Interface Implementation . . . . . . . . . . . . . 171

<!--list-separator-->

-  6.5 Likelihood Weighting . . . . . . . . . . . . . . . . . . . . 175

<!--list-separator-->

-  6.6 Metropolis-Hastings . . . . . . . . . . . . . . . . . . . . . 175

<!--list-separator-->

-  6.7 Sequential Monte Carlo . . . . . . . . . . . . . . . . . . . 178


### 7. Advanced topics {#7-dot-advanced-topics}

<!--list-separator-->

-  7.1 Inference Compilation . . . . . . . . . . . . . . . . . . . . 181

<!--list-separator-->

-  7.2 Model Learning . . . . . . . . . . . . . . . . . . . . . . . 186

<!--list-separator-->

-  7.3 Hamiltonian Monte Carlo and Variational Inference . . . . 191

<!--list-separator-->

-  7.4 Nesting . . . . . . . . . . . . . . . . . . . . . . . . . . . . 193

<!--list-separator-->

-  7.5 Formal Semantics . . . . . . . . . . . . . . . . . . . . . . 196


### 8. Conclusion {#8-dot-conclusion}
