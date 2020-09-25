+++
title = "pyro"
author = ["Cameron Smith"]
lastmod = 2020-09-20T17:37:36-04:00
slug = "pyro"
draft = false
+++

## [variational inference]({{< relref "variational_inference" >}}), [probabilistic inference]({{< relref "probabilistic_inference" >}}), [computation]({{< relref "computation" >}}) {#variational-inference--variational-inference-dot-md--probabilistic-inference--probabilistic-inference-dot-md--computation--computation-dot-md}


## lectures {#lectures}


### [Du Phan]({{< relref "Du_Phan" >}}) implemented [Statistical rethinking by Richard McElreath in 2020]({{< relref "Statistical_rethinking_by_Richard_McElreath_in_2020" >}}) in [pyro]({{< relref "pyro" >}}) {#du-phan--du-phan-dot-md--implemented-statistical-rethinking-by-richard-mcelreath-in-2020--statistical-rethinking-by-richard-mcelreath-in-2020-dot-md--in-pyro--pyro-dot-md}


### [talk on pyro by Chi Nhan Nguyen at ML conference](<https://youtu.be/mtFBfOmdFQk>) {#talk-on-pyro-by-chi-nhan-nguyen-at-ml-conference--https-youtu-dot-be-mtfbfomdfqk}


### technical talk including implementation information [Uber Open Summit 2018 Pyro: Deep Probabilistic Programming](<https://youtu.be/aLFJ5ERxt2c>) {#technical-talk-including-implementation-information-uber-open-summit-2018-pyro-deep-probabilistic-programming--https-youtu-dot-be-alfj5erxt2c}


## documentation {#documentation}


### introduction {#introduction}

<!--list-separator-->

-  [An Introduction to Models in Pyro](<https://pyro.ai/examples/intro%5Fpart%5Fi.html>)

    <!--list-separator-->

    -  [Primitive Stochastic Functions](<https://pyro.ai/examples/intro%5Fpart%5Fi.html#Primitive-Stochastic-Functions>)

    <!--list-separator-->

    -  [A Simple Model](<https://pyro.ai/examples/intro%5Fpart%5Fi.html#A-Simple-Model>)

    <!--list-separator-->

    -  [The pyro.sample Primitive](<https://pyro.ai/examples/intro%5Fpart%5Fi.html#The-pyro.sample-Primitive>)

    <!--list-separator-->

    -  [Universality: Stochastic Recursion, Higher-order Stochastic Functions, and Random Control Flow](<https://pyro.ai/examples/intro%5Fpart%5Fi.html#Universality:-Stochastic-Recursion,-Higher-order-Stochastic-Functions,-and-Random-Control-Flow>)

    <!--list-separator-->

    -  [Next Steps](<https://pyro.ai/examples/intro%5Fpart%5Fi.html#Next-Steps>)

<!--list-separator-->

-  [An Introduction to Inference in Pyro](<https://pyro.ai/examples/intro%5Fpart%5Fii.html>)

    <!--list-separator-->

    -  [A Simple Example](<https://pyro.ai/examples/intro%5Fpart%5Fii.html#A-Simple-Example>)

    <!--list-separator-->

    -  [Conditioning](<https://pyro.ai/examples/intro%5Fpart%5Fii.html#Conditioning>)

    <!--list-separator-->

    -  [Flexible Approximate Inference With Guide Functions](<https://pyro.ai/examples/intro%5Fpart%5Fii.html#Flexible-Approximate-Inference-With-Guide-Functions>)

    <!--list-separator-->

    -  [Parametrized Stochastic Functions and Variational Inference](<https://pyro.ai/examples/intro%5Fpart%5Fii.html#Parametrized-Stochastic-Functions-and-Variational-Inference>)

    <!--list-separator-->

    -  [Next Steps](<https://pyro.ai/examples/intro%5Fpart%5Fii.html#Next-Steps>)

<!--list-separator-->

-  [SVI Part I: An Introduction to Stochastic Variational Inference in Pyro](<https://pyro.ai/examples/svi%5Fpart%5Fi.html>)

    <!--list-separator-->

    -  [Setup](<https://pyro.ai/examples/svi%5Fpart%5Fi.html#Setup>)

        <!--list-separator-->

        -  The different pieces of a \`model()\` are encoded via the mapping:

            <!--list-separator-->

            -  1. observations \\[\Longleftrightarrow\\] \`pyro.sample\` with the \`obs\` argument

            <!--list-separator-->

            -  2. latent random variables \\[\Longleftrightarrow\\] \`pyro.sample\`

            <!--list-separator-->

            -  3. parameters \\[\Longleftrightarrow\\] \`pyro.param\`

        <!--list-separator-->

        -  When random variables are specified in Pyro with the primitive statement \`pyro.sample()\` the first argument denotes the name of the random variable. These names are used to align the random variables in the model and guide.

    <!--list-separator-->

    -  [Model Learning](<https://pyro.ai/examples/svi%5Fpart%5Fi.html#Model-Learning>)

    <!--list-separator-->

    -  [Guide](<https://pyro.ai/examples/svi%5Fpart%5Fi.html#Guide>)

        <!--list-separator-->

        -  The guide is a variational distribution

        <!--list-separator-->

        -  Just like the model, the guide is encoded as a stochastic function \`guide()\` that contains \`pyro.sample\` and \`pyro.param\` statements.

        <!--list-separator-->

        -  It does <span class="underline"><span class="underline">not</span></span> contain observed data, since the guide needs to be a properly normalized distribution.

        <!--list-separator-->

        -  Pyro enforces that \`model()\` and \`guide()\` have the same call signature, i.e. both callables should take the same arguments.

    <!--list-separator-->

    -  [ELBO](<https://pyro.ai/examples/svi%5Fpart%5Fi.html#ELBO>)

        <!--list-separator-->

        -  the gap between the ELBO and the log evidence is given by the KL divergence between the guide and the posterior

    <!--list-separator-->

    -  [SVI Class](<https://pyro.ai/examples/svi%5Fpart%5Fi.html#SVI-Class>)

    <!--list-separator-->

    -  [Optimizers](<https://pyro.ai/examples/svi%5Fpart%5Fi.html#Optimizers>)

        <!--list-separator-->

        -  Indeed parameters may be created dynamically during the course of inference. In other words the space we’re doing optimization over, which is parameterized by 𝜃θ and 𝜙ϕ, can grow and change dynamically.

    <!--list-separator-->

    -  [A simple example](<https://pyro.ai/examples/svi%5Fpart%5Fi.html#A-simple-example>)

    <!--list-separator-->

    -  [References](<https://pyro.ai/examples/svi%5Fpart%5Fi.html#References>)

<!--list-separator-->

-  [SVI Part II: Conditional Independence, Subsampling, and Amortization](<https://pyro.ai/examples/svi%5Fpart%5Fii.html>)

    <!--list-separator-->

    -  [The Goal: Scaling SVI to Large Datasets](<https://pyro.ai/examples/svi%5Fpart%5Fii.html#The-Goal:-Scaling-SVI-to-Large-Datasets>)

    <!--list-separator-->

    -  [Marking Conditional Independence in Pyro](<https://pyro.ai/examples/svi%5Fpart%5Fii.html#Marking-Conditional-Independence-in-Pyro>) [progress indicators]({{< relref "progress_indicators" >}})

        <!--list-separator-->

        -  Sequential

            <!--list-separator-->

            -  \_\_pyro.plate\_\_\_\_ is not appropriate for temporal models where each iteration of a loop depends on the previous iteration; in this case a \_\_\_\_range\_\_\_\_ or \_\_\_\_pyro.markov\_\_\_\_ should be used instead.\_\_

        <!--list-separator-->

        -  Vectorized

            <!--list-separator-->

            -  \_\_Conceptually vectorized \_\_\_\_plate\_\_\_\_ is the same as sequential \_\_\_\_plate\_\_\_\_ except that it is a vectorized operation (as \_\_\_\_torch.arange\_\_\_\_ is to \_\_\_\_range\_\_\_\_)\_\_

    <!--list-separator-->

    -  [Subsampling](<https://pyro.ai/examples/svi%5Fpart%5Fii.html#Subsampling>)

    <!--list-separator-->

    -  [Amortization](<https://pyro.ai/examples/svi%5Fpart%5Fii.html#Amortization>)

    <!--list-separator-->

    -  [Tensor shapes and vectorized plate](<https://pyro.ai/examples/svi%5Fpart%5Fii.html#Tensor-shapes-and-vectorized-plate>)

    <!--list-separator-->

    -  [References](<https://pyro.ai/examples/svi%5Fpart%5Fii.html#References>)

<!--list-separator-->

-  [SVI Part III: ELBO Gradient Estimators](<https://pyro.ai/examples/svi%5Fpart%5Fiii.html>)

    <!--list-separator-->

    -  [Setup](<https://pyro.ai/examples/svi%5Fpart%5Fiii.html#Setup>)

    <!--list-separator-->

    -  [Easy Case: Reparameterizable Random Variables](<https://pyro.ai/examples/svi%5Fpart%5Fiii.html#Easy-Case:-Reparameterizable-Random-Variables>)

    <!--list-separator-->

    -  [Tricky Case: Non-reparameterizable Random Variables](<https://pyro.ai/examples/svi%5Fpart%5Fiii.html#Tricky-Case:-Non-reparameterizable-Random-Variables>)

    <!--list-separator-->

    -  [Variance or Why I Wish I Was Doing MLE Deep Learning](<https://pyro.ai/examples/svi%5Fpart%5Fiii.html#Variance-or-Why-I-Wish-I-Was-Doing-MLE-Deep-Learning>)

    <!--list-separator-->

    -  [References](<https://pyro.ai/examples/svi%5Fpart%5Fiii.html#References>)


### advanced {#advanced}


### examples {#examples}

<!--list-separator-->

-


### contributed {#contributed}

<!--list-separator-->

-  [dirichlet process mixture model](<https://pyro.ai/examples/dirichlet%5Fprocess%5Fmixture.html>)


## notes {#notes}


### [stochastic variational inference in variational bayesian methods](<https://en.wikipedia.org/wiki/Variational%5FBayesian%5Fmethods>) {#stochastic-variational-inference-in-variational-bayesian-methods--https-en-dot-wikipedia-dot-org-wiki-variational-bayesian-methods}
