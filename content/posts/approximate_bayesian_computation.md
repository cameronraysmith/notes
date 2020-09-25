+++
title = "approximate bayesian computation"
author = ["Cameron Smith"]
lastmod = 2020-09-24T22:43:03-04:00
slug = "approximate_bayesian_computation"
draft = false
+++

## [probabilistic inference]({{< relref "probabilistic_inference" >}}), [algorithms]({{< relref "algorithms" >}}), [probabilistic programming]({{< relref "probabilistic_programming" >}}) {#probabilistic-inference--probabilistic-inference-dot-md--algorithms--algorithms-dot-md--probabilistic-programming--probabilistic-programming-dot-md}


## [wikipedia]({{< relref "wikipedia" >}}) {#wikipedia--wikipedia-dot-md}

In all model-based statistical inference, the likelihood function is of central importance, since it expresses the probability of the observed data under a particular statistical model, and thus quantifies the support data lend to particular values of parameters and to choices among different models. For simple models, an analytical formula for the likelihood function can typically be derived. However, for more complex models, an analytical formula might be elusive or the likelihood function might be computationally very costly to evaluate.

ABC methods bypass the evaluation of the likelihood function. In this way, ABC methods widen the realm of models for which statistical inference can be considered. ABC methods are mathematically well-founded, but they inevitably make assumptions and approximations whose impact needs to be carefully assessed. Furthermore, the wider application domain of ABC exacerbates the challenges of parameter estimation and model selection.


## questions {#questions}


### How does [[file:approximate\_bayesian\_computation.org][approximate bayesian computation](https://fehiepsi.github.io/rethinking-numpyro/16-generalized-linear-madness.html) compare to the Lotka-Volterra parameter inference in [Chapter 16. Generalized Linear Madness]] of [Du Phan's implementation of Statistical rethinking in pyro]({{< relref "Du_Phan's_implementation_of_Statistical_rethinking_in_pyro" >}})? {#how-does-file-approximate-bayesian-computation-dot-org-approximate-bayesian-computation-compare-to-the-lotka-volterra-parameter-inference-in-chapter-16-dot-generalized-linear-madness-of-du-phan-s-implementation-of-statistical-rethinking-in-pyro--du-phan-s-implementation-of-statistical-rethinking-in-pyro-dot-md}


### More generally, how does [approximate bayesian computation]({{< relref "approximate_bayesian_computation" >}}) compare to [mean-field approximation]({{< relref "mean-field_approximation" >}}), [variational inference]({{< relref "variational_inference" >}})? {#more-generally-how-does-approximate-bayesian-computation--approximate-bayesian-computation-dot-md--compare-to-mean-field-approximation--mean-field-approximation-dot-md--variational-inference--variational-inference-dot-md}


## code {#code}


### <https://github.com/tanhevg/GpABC.jl> [julia]({{< relref "julia" >}}) {#https-github-dot-com-tanhevg-gpabc-dot-jl-julia--julia-dot-md}


### <https://github.com/icb-dcm/pyabc> [python]({{< relref "python" >}}) {#https-github-dot-com-icb-dcm-pyabc-python--python-dot-md}


### <https://github.com/pyprob/pyprob> [python]({{< relref "python" >}}) {#https-github-dot-com-pyprob-pyprob-python--python-dot-md}


## papers {#papers}


### [approximate bayesian computation scheme for parameter inference and model selection in dynamical systems by Tina Toni, Michael P. H. Stumpf et al in 2009]({{< relref "approximate_bayesian_computation_scheme_for_parameter_inference_and_model_selection_in_dynamical_systems_by_Tina_Toni,_Michael_P_H_Stumpf_et_al_in_2009" >}}) {#approximate-bayesian-computation-scheme-for-parameter-inference-and-model-selection-in-dynamical-systems-by-tina-toni-michael-p-dot-h-dot-stumpf-et-al-in-2009--approximate-bayesian-computation-scheme-for-parameter-inference-and-model-selection-in-dynamical-systems-by-tina-toni-michael-p-h-stumpf-et-al-in-2009-dot-md}


### [A framework for parameter estimation and model selection from experimental data in systems biology using approximate bayesian computation by Juliane Liepe, Michael P. H. Stumpf et al in 2014]({{< relref "A_framework_for_parameter_estimation_and_model_selection_from_experimental_data_in_systems_biology_using_approximate_bayesian_computation_by_Juliane_Liepe,_Michael_P_H_Stumpf_et_al_in_2014" >}}) {#a-framework-for-parameter-estimation-and-model-selection-from-experimental-data-in-systems-biology-using-approximate-bayesian-computation-by-juliane-liepe-michael-p-dot-h-dot-stumpf-et-al-in-2014--a-framework-for-parameter-estimation-and-model-selection-from-experimental-data-in-systems-biology-using-approximate-bayesian-computation-by-juliane-liepe-michael-p-h-stumpf-et-al-in-2014-dot-md}


### [A Simulated Annealing Approach to Bayesian Inference by Carlo Albert in 2018]({{< relref "A_Simulated_Annealing_Approach_to_Bayesian_Inference_by_Carlo_Albert_in_2018" >}}) {#a-simulated-annealing-approach-to-bayesian-inference-by-carlo-albert-in-2018--a-simulated-annealing-approach-to-bayesian-inference-by-carlo-albert-in-2018-dot-md}


### [GpABC a Julia package for approximate bayesian computation with Gaussian process emulation by Evgeny Tankhilevich, Michael P. H. Stumpf et al in 2020]({{< relref "GpABC_a_Julia_package_for_approximate_bayesian_computation_with_Gaussian_process_emulation_by_Evgeny_Tankhilevich,_Michael_P_H_Stumpf_et_al_in_2020" >}}) {#gpabc-a-julia-package-for-approximate-bayesian-computation-with-gaussian-process-emulation-by-evgeny-tankhilevich-michael-p-dot-h-dot-stumpf-et-al-in-2020--gpabc-a-julia-package-for-approximate-bayesian-computation-with-gaussian-process-emulation-by-evgeny-tankhilevich-michael-p-h-stumpf-et-al-in-2020-dot-md}


### [Efficient exact inference for dynamical systems with noisy measurements using sequential approximate bayesian computation by Yannik Schalte and Jan Hasenauer in 2020]({{< relref "Efficient_exact_inference_for_dynamical_systems_with_noisy_measurements_using_sequential_approximate_bayesian_computation_by_Yannik_Schalte_and_Jan_Hasenauer_in_2020" >}}) {#efficient-exact-inference-for-dynamical-systems-with-noisy-measurements-using-sequential-approximate-bayesian-computation-by-yannik-schalte-and-jan-hasenauer-in-2020--efficient-exact-inference-for-dynamical-systems-with-noisy-measurements-using-sequential-approximate-bayesian-computation-by-yannik-schalte-and-jan-hasenauer-in-2020-dot-md}


### [Statistical inference for stochastic simulation models theory and application by Florian Hartig, Andreas Huth, et al in 2011]({{< relref "Statistical_inference_for_stochastic_simulation_models_-_theory_and_application_by_Florian_Hartig,_Andreas_Huth,_et_al_in_2011" >}}) {#statistical-inference-for-stochastic-simulation-models-theory-and-application-by-florian-hartig-andreas-huth-et-al-in-2011--statistical-inference-for-stochastic-simulation-models-theory-and-application-by-florian-hartig-andreas-huth-et-al-in-2011-dot-md}


### [Efficient probabilistic inference in the quest for physics beyond the Standard Model by Atilim Baydin, Frank Wood et al in 2019]({{< relref "Efficient_probabilistic_inference_in_the_quest_for_physics_beyond_the_Standard_Model_by_Atilim_Baydin,_Frank_Wood_et_al_in_2019" >}}) {#efficient-probabilistic-inference-in-the-quest-for-physics-beyond-the-standard-model-by-atilim-baydin-frank-wood-et-al-in-2019--efficient-probabilistic-inference-in-the-quest-for-physics-beyond-the-standard-model-by-atilim-baydin-frank-wood-et-al-in-2019-dot-md}
