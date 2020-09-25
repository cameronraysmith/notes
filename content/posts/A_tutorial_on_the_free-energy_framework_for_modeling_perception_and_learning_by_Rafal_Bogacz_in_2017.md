+++
title = "A tutorial on the free-energy framework for modeling perception and learning by Rafal Bogacz in 2017"
author = ["Cameron Smith"]
lastmod = 2020-09-20T17:33:41-04:00
slug = "A_tutorial_on_the_free-energy_framework_for_modeling_perception_and_learning_by_Rafal_Bogacz_in_2017"
draft = false
+++

## [papers]({{< relref "papers" >}}), [free energy principle]({{< relref "free_energy_principle" >}}), [probabilistic inference]({{< relref "probabilistic_inference" >}}) {#papers--papers-dot-md--free-energy-principle--free-energy-principle-dot-md--probabilistic-inference--probabilistic-inference-dot-md}


## 1. Introduction {#1-dot-introduction}


### The model of Friston (2005) and the [predictive coding model]({{< relref "predictive_coding_model" >}}) of Rao and Ballard (1999) provide a powerful mathematical framework to describe how the sensory cortex extracts information from noisy stimuli. The [predictive coding model]({{< relref "predictive_coding_model" >}}) (Rao & Ballard, 1999) suggests that visual cortex infers the most likely properties of stimuli from noisy sensory input. {#the-model-of-friston--2005--and-the-predictive-coding-model--predictive-coding-model-dot-md--of-rao-and-ballard--1999--provide-a-powerful-mathematical-framework-to-describe-how-the-sensory-cortex-extracts-information-from-noisy-stimuli-dot-the-predictive-coding-model--predictive-coding-model-dot-md----rao-and-ballard-1999--suggests-that-visual-cortex-infers-the-most-likely-properties-of-stimuli-from-noisy-sensory-input-dot}


### Friston's model added the explicit representation of uncertainy to the [predictive coding model]({{< relref "predictive_coding_model" >}}) framework {#friston-s-model-added-the-explicit-representation-of-uncertainy-to-the-predictive-coding-model--predictive-coding-model-dot-md--framework}

<!--list-separator-->

-  learning about the variance and covariance of features can also be implemented by simple synaptic plasticity rules

<!--list-separator-->

-  the perceptual system may differentially weight sources of sensory information depending on their level of noise

<!--list-separator-->

-  sensory networks can learn to recognize features encoded in patterns of covariance between inputs

<!--list-separator-->

-  it provides a natural way to implement attentional modulation as the reduction in variance of attended features

<!--list-separator-->

-  this model can be viewed as an approximate Bayesian inference based on minimization of the so-called "free-energy" function


### Any computational model would need to satisfy the following constraints to be considered biologically plausible {#any-computational-model-would-need-to-satisfy-the-following-constraints-to-be-considered-biologically-plausible}

<!--list-separator-->

-  1. Local computation: A neuron performs computations only on the basis of the activity of its input neurons and synaptic weights associated with these inputs (rather than information encoded in other parts of the circuit).

<!--list-separator-->

-  2. Local plasticity: Synaptic plasticity is only based on the activity of pre-synaptic and post-synaptic neurons.


### Outline of the paper {#outline-of-the-paper}

<!--list-separator-->

-  2. Introduces the model using a very simple example and with simple mathematical concepts for the purpose of maximizing accessibility

<!--list-separator-->

-  3. provides mathematical foundations for the model and shows how the inference in the model is related to minimizing free-energy

<!--list-separator-->

-  4. Application to biological neural networks: scaling up the model to describe sensory cortex

<!--list-separator-->

-  5. An extension of the Friston 2005 model that satisfies the constraint of local plasticity


## 2. Simplest example of perception {#2-dot-simplest-example-of-perception}


### 2.0 Introduction {#2-dot-0-introduction}

<!--list-separator-->

-  Consider attempting to infer the size of an object \\[v\\] from light intensity \\[u\\] where the relationship providing the expected value of light intensity from object size is given by \\[ g(v) = v^2 \\].

<!--list-separator-->

-  The likelihood of observing a given light intensity given a particular object is then

    <!--list-separator-->

    -  \\[p(u \vert v) = f(u;\; g(v), \, \Sigma\_u)\\]

<!--list-separator-->

-  We would now like to invert this relationship to estimate the probability of a particular object size given an observation: \\[ p(v \vert u)\\].


### 2.1 Exact solution {#2-dot-1-exact-solution}

<!--list-separator-->

-


## 3. Scaling up the model of perception {#3-dot-scaling-up-the-model-of-perception}


## 4. Local plasticity {#4-dot-local-plasticity}


## 5. Discussion {#5-dot-discussion}
