+++
title = "turing.jl"
author = ["Cameron Smith"]
lastmod = 2020-09-20T17:37:52-04:00
slug = "turingjl"
draft = false
+++

## [probabilistic inference]({{< relref "probabilistic_inference" >}}), [computation]({{< relref "computation" >}}), [julia]({{< relref "julia" >}}), [software library]({{< relref "software_library" >}}) {#probabilistic-inference--probabilistic-inference-dot-md--computation--computation-dot-md--julia--julia-dot-md--software-library--software-library-dot-md}


## tutorials {#tutorials}


### <https://turing.ml/dev/tutorials/> {#https-turing-dot-ml-dev-tutorials}


### tutorial on the beta-bernoulli model {#tutorial-on-the-beta-bernoulli-model}


### tutorial on [linear models]({{< relref "linear_models" >}}) {#tutorial-on-linear-models--linear-models-dot-md}


### tutorial on [variational inference]({{< relref "variational_inference" >}}): <https://turing.ml/dev/tutorials/9-variationalinference/> {#tutorial-on-variational-inference--variational-inference-dot-md--https-turing-dot-ml-dev-tutorials-9-variationalinference}

<!--list-separator-->

-  By default, i.e. when calling \`vi(m, advi)\`, Turing uses a [mean-field approximation]({{< relref "mean-field approximation" >}}) with a multivariate normal as the base-distribution. Mean-field refers to the fact that we assume all the latent variables to be \_\_independent\_\_. This is the “standard” ADVI approach; see [Automatic Differentiation Variational Inference by Dustin Tran, Andrew Gelman, David Blei et al in 2016]({{< relref "Automatic_Differentiation_Variational_Inference_by_Dustin_Tran,_Andrew_Gelman,_David_Blei_et_al_in_2016" >}}) for more. In Turing, one can obtain such a [mean-field approximation]({{< relref "mean-field_approximation" >}}) by calling Variational.meanfield(model) for which there exists an internal implementation for update


###  {#}


## [Gaussian process]({{< relref "Gaussian_process" >}}) {#gaussian-process--gaussian-process-dot-md}


### <https://discourse.julialang.org/t/gaussian-process-model-with-turing/42453/13> {#https-discourse-dot-julialang-dot-org-t-gaussian-process-model-with-turing-42453-13}
