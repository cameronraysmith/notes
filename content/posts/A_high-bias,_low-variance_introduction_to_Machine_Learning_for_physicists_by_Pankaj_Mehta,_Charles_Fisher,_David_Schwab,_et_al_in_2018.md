+++
title = "A high-bias, low-variance introduction to Machine Learning for physicists by Pankaj Mehta, Charles Fisher, David Schwab, et al in 2018"
author = ["Cameron Smith"]
lastmod = 2020-09-20T17:33:39-04:00
slug = "A_high-bias,_low-variance_introduction_to_Machine_Learning_for_physicists_by_Pankaj_Mehta,_Charles_Fisher,_David_Schwab,_et_al_in_2018"
draft = false
+++

## [probabilistic inference]({{< relref "probabilistic_inference" >}}), [statistical physics]({{< relref "statistical_physics" >}}), [variational inference]({{< relref "variational_inference" >}}), [information geometry]({{< relref "information_geometry" >}}), [renormalization]({{< relref "renormalization" >}})  [Non-equilibrium statistical physics]({{< relref "Non-equilibrium_statistical_physics" >}}) {#probabilistic-inference--probabilistic-inference-dot-md--statistical-physics--statistical-physics-dot-md--variational-inference--variational-inference-dot-md--information-geometry--information-geometry-dot-md--renormalization--renormalization-dot-md--non-equilibrium-statistical-physics--non-equilibrium-statistical-physics-dot-md}


## code {#code}


### "✔ Containerize the notebooks for High-bias low-variance introduction to ML paper (see <https://github.com/cameronraysmith/mlreview%5Fnotebooks> ) @est(1h) @done(19-10-14 21:56) @project(Computation.Machine learning)" {#containerize-the-notebooks-for-high-bias-low-variance-introduction-to-ml-paper--see-https-github-dot-com-cameronraysmith-mlreview-notebooks--est--1h--done--19-10-14-21-56--project--computation-dot-machine-learning}


### <https://physics.bu.edu/~pankajm/MLnotebooks.html> {#https-physics-dot-bu-dot-edu-pankajm-mlnotebooks-dot-html}


### notebooks {#notebooks}

<!--list-separator-->

-  NB01 CII polynomial regression

<!--list-separator-->

-  NB02 CIV gradient descent

<!--list-separator-->

-  NB03 CVI linear regression for diabetes data

<!--list-separator-->

-  NB04 CVI linear regression for the Ising model

<!--list-separator-->

-  NB05 CVII logistic regression SUSY

<!--list-separator-->

-  NB06 CVII logistic regression Ising

<!--list-separator-->

-  NB07 CVII logistic regression MNIST

<!--list-separator-->

-  NB08 CVIII bagging perceptron

<!--list-separator-->

-  NB09 CVIII random forests Ising

<!--list-separator-->

-  NB10 CVIII XGboost SUSY

<!--list-separator-->

-  NB11 CIX DNN MNIST keras

<!--list-separator-->

-  NB12 CIX DNN SUSY tensorflow

<!--list-separator-->

-  NB13 CIX DNN Ising pytorch

<!--list-separator-->

-  NB14 CX CNN Ising pytorch

<!--list-separator-->

-  NB15 CXIII clustering

<!--list-separator-->

-  NB16 CXIV EM coin toss

<!--list-separator-->

-  NB17 CXVI Restricted Boltzmann Machine MNIST

<!--list-separator-->

-  NB18 CXVI Restricted Boltzmann Machine Ising

<!--list-separator-->

-  NB19 CXVII Keras Variational Autoencoder MNIST

<!--list-separator-->

-  NB20 CXVII Keras Variational Autoencoder Ising


## citation {#citation}


### Mehta, P., Bukov, M., Wang, C.-H., Day, A. G. R., Richardson, C., Fisher, C. K., & Schwab, D. J. (2018). A high-bias, low-variance introduction to Machine Learning for physicists. Retrieved from <https://arxiv.org/pdf/1803.08823.pdf> {#mehta-p-dot-bukov-m-dot-wang-c-dot-h-dot-day-a-dot-g-dot-r-dot-richardson-c-dot-fisher-c-dot-k-dot-and-schwab-d-dot-j-dot--2018--dot-a-high-bias-low-variance-introduction-to-machine-learning-for-physicists-dot-retrieved-from-https-arxiv-dot-org-pdf-1803-dot-08823-dot-pdf}


## list of topics {#list-of-topics}


### polynomial regression {#polynomial-regression}


### linear regression {#linear-regression}


### logistic regression {#logistic-regression}


### combining models {#combining-models}


### feed-forward deep neural networks {#feed-forward-deep-neural-networks}


### convolutional neural networks {#convolutional-neural-networks}


### clustering {#clustering}


### expectation maximization {#expectation-maximization}


### restricted boltzmann machines {#restricted-boltzmann-machines}


### variational autoencoders {#variational-autoencoders}


## contents {#contents}


### XVI. DEEP GENERATIVE MODELS: LATENT VARIABLES AND RESTRICTED BOLTZMANN MACHINES (RBMS) {#xvi-dot-deep-generative-models-latent-variables-and-restricted-boltzmann-machines--rbms}

<!--list-separator-->

-  A. Why hidden (latent) variables?

    <!--list-separator-->

    -  Latent or hidden variables are a powerful yet elegant

        way to encode sophisticated correlations between observ\* able features. The underlying reason for this is that marginalizing over a subset of variables – “integrating out” degrees of freedom in the language of physics – in\* duces complex interactions between the remaining vari\* ables. The idea that integrating out variables can lead to complex correlations is a familiar component of many physical theories. For example, when considering free electrons living on a lattice, integrating out phonons gives rise to higher-order electron-electron interactions (e.g. su\* perconducting or magnetic correlations). More generally, in the Wilsonian renormalization group paradigm, all ef\* fective field theories can be thought of as arising from integrating out high-energy degrees of freedom (Wilson and Kogut, 1974).

    <!--list-separator-->

    -  Generative models with latent variables run this logic

        in reverse – encode complex interactions between visible variables by introducing additional, hidden variables that interact with visible degrees of freedom in a simple man\* ner, yet still reproduce the complex correlations between visible degrees in the data once marginalized over (integrated out). This allows us to encode complex higher\* order interactions between the visible variables using sim\* pler interactions at the cost of introducing new latent variables/degrees of freedom. This trick is also widely exploited in physics (e.g. in the Hubbard-Stratonovich transformation (Hubbard, 1959; Stratonovich, 1957) or the introduction of ghost fields in gauge theory (Faddeev and Popov, 1967)).
