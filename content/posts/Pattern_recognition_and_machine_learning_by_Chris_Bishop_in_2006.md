+++
title = "Pattern recognition and machine learning by Chris Bishop in 2006"
author = ["Cameron Smith"]
lastmod = 2020-09-20T17:35:34-04:00
slug = "Pattern_recognition_and_machine_learning_by_Chris_Bishop_in_2006"
draft = false
+++

## "<span class="underline"><span class="underline">This is the first textbook on pattern recognition to present the Bayesian viewpoint. The book presents approximate inference algorithms that permit fast approximate answers in situations where exact answers are not feasible. It uses graphical models to describe probability distributions when no other books apply graphical models to machine learning.</span></span> — via [Pattern Recognition and Machine Learning (Information Science and Statistics): Bishop, Christopher M.: 9780387310732: Amazon.com: Books](<https://www.amazon.com/Pattern-Recognition-Learning-Information-Statistics/dp/0387310738/>) brought back to my attention via <https://bloomberg.github.io/foml/#lectures> " {#via-pattern-recognition-and-machine-learning--information-science-and-statistics--bishop-christopher-m-dot-9780387310732-amazon-dot-com-books--https-www-dot-amazon-dot-com-pattern-recognition-learning-information-statistics-dp-0387310738--brought-back-to-my-attention-via-https-bloomberg-dot-github-dot-io-foml-lectures}


## "Found another source pointing to [Pattern recognition and machine learning by Chris Bishop in 2006]({{< relref "Pattern_recognition_and_machine_learning_by_Chris_Bishop_in_2006" >}}) on the [pymc3 discourse](<https://discourse.pymc.io/t/machine-learning-textbook-with-a-bayesian-perceptive/68>)" {#found-another-source-pointing-to-pattern-recognition-and-machine-learning-by-chris-bishop-in-2006--pattern-recognition-and-machine-learning-by-chris-bishop-in-2006-dot-md--on-the-pymc3-discourse--https-discourse-dot-pymc-dot-io-t-machine-learning-textbook-with-a-bayesian-perceptive-68}


## [books]({{< relref "books" >}}), [probabilistic inference]({{< relref "probabilistic_inference" >}}) {#books--books-dot-md--probabilistic-inference--probabilistic-inference-dot-md}


## 1. Introduction {#1-dot-introduction}


### 1.1 Example polynomial curve fitting {#1-dot-1-example-polynomial-curve-fitting}

<!--list-separator-->

-  maximum likelihood

<!--list-separator-->

-  shrinkage methods

    <!--list-separator-->

    -  [Tikhonov regularization](<https://en.wikipedia.org/wiki/Tikhonov%5Fregularization>) / ridge regression (Hoerl and Kennard, 1970) and weight decay

        <!--list-separator-->

        -  \\[\tilde{E}(w) = \frac{1}{2} \sum\_{n=1}^{N} \\{ y(x\_n, \mathbf{w}) \* t\_n \\}^2 + \frac{\lambda}{2} || \mathbf{w} ||^2\\]


### 1.2 Probability theory {#1-dot-2-probability-theory}

<!--list-separator-->

-  1.2.1 Probability densities

<!--list-separator-->

-  1.2.2 Expectations and covariances

<!--list-separator-->

-  1.2.3 Bayesian probabilities

    <!--list-separator-->

    -  Consider an uncertain event, for example whether the moon was once in its own orbit around the sun, or whether the Arctic ice cap will have disappeared by the end of the century. These are not events that can be repeated numerous times in order to define a notion of probability as we did earlier in the context of boxes of fruit. Nevertheless, we will generally have some idea, for example, of how quickly we think the polar ice is melting.

    <!--list-separator-->

    -  we would like to be able to quantify our expression of uncertainty and make precise revisions of uncertainty in the light of new evidence, as well as subsequently to be able to take optimal actions or decisions as a consequence

    <!--list-separator-->

    -  candidate axiomatizations of probability

        <!--list-separator-->

        -  Ramsey, F. (1931). Truth and probability. In R. Braithwaite (Ed.), The Foundations of Mathematics and other Logical Essays. Humanities Press.

        <!--list-separator-->

        -  Cox, R. T. (1946). Probability, frequency and reasonable expectation. American Journal of Physics 14(1), 1–13.

        <!--list-separator-->

        -  Good, I. (1950). Probability and the Weighing of Evidence. Hafners.

        <!--list-separator-->

        -  Savage, L. J. (1961). The subjective basis of statistical practice. Technical report, Department of Statistics, University of Michigan, Ann Arbor.

        <!--list-separator-->

        -  deFinetti, B. (1970). Theory of Probability. Wiley and Sons.

        <!--list-separator-->

        -  Lindley, D. V. (1982). Scoring rules and the inevitability of probability. International Statistical Review 50, 1–26.

        <!--list-separator-->

        -  Jaynes, E. T. (2003). Probability Theory: The Logic of Science. Cambridge University Press.

<!--list-separator-->

-  1.2.4 The Gaussian distribution

<!--list-separator-->

-  1.2.5 Curve fitting re-visited

<!--list-separator-->

-  1.2.6 Bayesian curve fitting [key subsection]({{< relref "key_subsection" >}})

    <!--list-separator-->

    -  Look for reference with code / derivation of the analytical form given in equations 1.69-1.72


### 1.3 Model selection [progress indicators]({{< relref "progress_indicators" >}}) {#1-dot-3-model-selection-progress-indicators--progress-indicators-dot-md}


### 1.4 The curse of dimensionality {#1-dot-4-the-curse-of-dimensionality}


### 1.5 Decision theory {#1-dot-5-decision-theory}

<!--list-separator-->

-  1.5.1 Minimizing the misclassification rate

<!--list-separator-->

-  1.5.2 Minimizing the expected loss

<!--list-separator-->

-  1.5.3 The reject option

<!--list-separator-->

-  1.5.4 Inference and decision

    <!--list-separator-->

    -  Cross-references

        <!--list-separator-->

        -  "4.2 Probabilistic generative models (for classification) [key subsection]({{< relref "key_subsection" >}})"

    <!--list-separator-->

    -

<!--list-separator-->

-  1.5.5 Loss functions for regression


### 1.6 Information theory {#1-dot-6-information-theory}

<!--list-separator-->

-  1.6.1 Relative entropy and mutual information


## 2. Probability distributions {#2-dot-probability-distributions}


### 2.1 Binary variables {#2-dot-1-binary-variables}

<!--list-separator-->

-  2.1.1 The beta distribution


### 2.2 Multinomial variables {#2-dot-2-multinomial-variables}

<!--list-separator-->

-  2.2.1 The Dirichlet distribution


### 2.3 The Gausssian distribution {#2-dot-3-the-gausssian-distribution}

<!--list-separator-->

-  2.3.1 Conditional Gaussian distributions

<!--list-separator-->

-  2.3.2 Marginal Gaussian distributions

<!--list-separator-->

-  2.3.3 Bayes' theorem for Gaussian variables

<!--list-separator-->

-  2.3.4 Maximum likelihood for the Gaussian

<!--list-separator-->

-  2.3.5 Sequential estimation

<!--list-separator-->

-  2.3.6 Bayesian inference for the Gaussian

<!--list-separator-->

-  2.3.7 Student's t-distribution

<!--list-separator-->

-  2.3.8 Periodic variables

<!--list-separator-->

-  2.3.9 Mixtures of Gaussians


### 2.4 The exponential family {#2-dot-4-the-exponential-family}

<!--list-separator-->

-  2.4.1 Maximum likelihood and sufficient statistics

<!--list-separator-->

-  2.4.2 Conjugate priors

<!--list-separator-->

-  2.4.3 Noninformative priors


### 2.5 Nonparametric methods {#2-dot-5-nonparametric-methods}

<!--list-separator-->

-  2.5.1 Kernel density estimators

<!--list-separator-->

-  2.5.2 Nearest-neighbor methods


## 3. Linear models for regression {#3-dot-linear-models-for-regression}


### 3.1 Linear basis function models {#3-dot-1-linear-basis-function-models}

<!--list-separator-->

-  3.1.1 Maximum likelihood and least squares

<!--list-separator-->

-  3.1.2 Geometry of least squares

<!--list-separator-->

-  3.1.3 Sequential learning

<!--list-separator-->

-  3.1.4 Regularized least squares

<!--list-separator-->

-  3.1.5 Multiple outputs


### 3.2 The bias-variance decomposition {#3-dot-2-the-bias-variance-decomposition}


### 3.3 Bayesian linear regression [key subsection]({{< relref "key_subsection" >}}) {#3-dot-3-bayesian-linear-regression-key-subsection--key-subsection-dot-md}

<!--list-separator-->

-  3.3.1 Parameter distribution

<!--list-separator-->

-  3.3.2 Predictive distribution

<!--list-separator-->

-  3.3.3 Equivalent kernel


### 3.4 Bayesian model comparison {#3-dot-4-bayesian-model-comparison}


### 3.5 The evidence approximation {#3-dot-5-the-evidence-approximation}

<!--list-separator-->

-  3.5.1 Evaluation of the evidence function

<!--list-separator-->

-  3.5.2 Maximizing the evidence function

<!--list-separator-->

-  3.5.3 Effective number of parameters


### 3.6 Limitations of fixed basis functions {#3-dot-6-limitations-of-fixed-basis-functions}


## 4. Linear models for classification {#4-dot-linear-models-for-classification}


### 4.1 Discriminant functions {#4-dot-1-discriminant-functions}

<!--list-separator-->

-  4.1.1 Two classes

<!--list-separator-->

-  4.1.2 Multiple classes

<!--list-separator-->

-  4.1.3 Least squares for classification

<!--list-separator-->

-  4.1.4 Fisher's linear discriminant

<!--list-separator-->

-  4.1.5 Relation to least squares

<!--list-separator-->

-  4.1.6 Fisher's discriminant for multiple classes

<!--list-separator-->

-  4.1.7 The perceptron algorithm


### 4.2 Probabilistic generative models (for classification) [key subsection]({{< relref "key_subsection" >}}) {#4-dot-2-probabilistic-generative-models--for-classification--key-subsection--key-subsection-dot-md}

<!--list-separator-->

-  4.2.0 Introduction

    <!--list-separator-->

    -  We turn next to a ****probabilistic view of classification**** and show how ****models with linear decision boundaries**** arise from ****simple assumptions about the distribution of the data****.

    <!--list-separator-->

    -  The class-conditional densities \\[p(\mathbf{x} \vert \mathcal{C}\_k)\\] and class priors \\[p(\mathcal{C}\_k)\\] can be used to compute the class posteriors \\[p(\mathcal{C}\_k \vert x)\\].

    <!--list-separator-->

    -  In general, the posterior distribution takes the form of a [normalized exponential function]({{< relref "normalized_exponential_function" >}}), which is a multiclass generalization of the [logistic sigmoid function]({{< relref "logistic_sigmoid_function" >}}).

        <!--list-separator-->

        -  \\[p(\mathcal{C}\_k \vert x) = \frac{\exp(a\_k)}{\Sigma\_j \exp(a\_j)}\\]

        <!--list-separator-->

        -  where \\[a\_k = \ln p(\mathbf{x} \vert \mathcal{C}\_k) p(\mathcal{C}\_k)\\]

<!--list-separator-->

-  4.2.1 Continuous inputs

    <!--list-separator-->

    -  Let us assume that the class-conditional densities are Gaussian and then explore the resulting form for the posterior probabilities.

<!--list-separator-->

-  4.2.2 Maximum likelihood solution

<!--list-separator-->

-  4.2.3 Discrete features

<!--list-separator-->

-  4.2.4 Exponential family


### 4.3 Probabilistic discriminative models {#4-dot-3-probabilistic-discriminative-models}

<!--list-separator-->

-  4.3.1 Fixed basis functions

<!--list-separator-->

-  4.3.2 Logistic regression

<!--list-separator-->

-  4.3.3 Iteratively reweighted least squares

<!--list-separator-->

-  4.3.4 Multiclass logistic regression

<!--list-separator-->

-  4.3.5 Probit regression

<!--list-separator-->

-  4.3.6 Canonical link functions


### 4.4 The Laplace approximation [key subsection]({{< relref "key_subsection" >}}) {#4-dot-4-the-laplace-approximation-key-subsection--key-subsection-dot-md}

<!--list-separator-->

-  4.4.0 Introduction

<!--list-separator-->

-  4.4.1 Model comparison and BIC


### 4.5 Bayesian logistic regression [key subsection]({{< relref "key_subsection" >}}) {#4-dot-5-bayesian-logistic-regression-key-subsection--key-subsection-dot-md}

<!--list-separator-->

-  4.5.0 Introduction

    <!--list-separator-->

    -  Exact Bayesian inference for logistic regression is intractable.

    <!--list-separator-->

    -  Here we consider the application of the Laplace approximation to the problem of Bayesian logistic regression

        <!--list-separator-->

        -  Spiegelhalter and Lauritzen, 1990;

            <!--list-separator-->

            -  Spiegelhalter, D. and S. Lauritzen (1990). Sequential updating of conditional probabilities on directed graphical structures. Networks 20, 579–605.

        <!--list-separator-->

        -  MacKay, 1992b

            <!--list-separator-->

            -  MacKay, D. J. C. (1992b). The evidence framework applied to classification networks. Neural Computation 4(5), 720–736.

<!--list-separator-->

-  4.5.1 Laplace approximation

<!--list-separator-->

-  4.5.2 Predictive distribution

<!--list-separator-->

-


## 5. Neural networks {#5-dot-neural-networks}


### 5.1 Feed-forward network functions {#5-dot-1-feed-forward-network-functions}

<!--list-separator-->

-  5.1.1 Weight-space symmetries


### 5.2 Network training {#5-dot-2-network-training}

<!--list-separator-->

-  5.2.1 Parameter optimization

<!--list-separator-->

-  5.2.2 Local quadratic approximation

<!--list-separator-->

-  5.2.3 Use of gradient information

<!--list-separator-->

-  5.2.4 Gradient descent optimization


### 5.3 Error backpropagation {#5-dot-3-error-backpropagation}

<!--list-separator-->

-  5.3.1 Evaluation of error-function derivatives

<!--list-separator-->

-  5.3.2 A simple example

<!--list-separator-->

-  5.3.3 Efficiency of backpropagation

<!--list-separator-->

-  5.3.4 The Jacobian matrix


### 5.4 The Hessian matrix {#5-dot-4-the-hessian-matrix}

<!--list-separator-->

-  5.4.1 Diagonal approximation

<!--list-separator-->

-  5.4.2 Outer product approximation

<!--list-separator-->

-  5.4.3 Inverse Hessian

<!--list-separator-->

-  5.4.4 Finite differences

<!--list-separator-->

-  5.4.5 Exact evaluation of the Hessian

<!--list-separator-->

-  5.4.6 Fast multiplication by the Hessian


### 5.5 Regularization in neural networks {#5-dot-5-regularization-in-neural-networks}

<!--list-separator-->

-  5.5.1 Consistent Gaussian priors

<!--list-separator-->

-  5.5.2 Early stopping

<!--list-separator-->

-  5.5.3 Invariances

<!--list-separator-->

-  5.5.4 Tangent propagation

<!--list-separator-->

-  5.5.5 Training with transformed data

<!--list-separator-->

-  5.5.6 Convolutional networks

<!--list-separator-->

-  5.5.7 Soft weight sharing


### 5.6 Mixture density networks {#5-dot-6-mixture-density-networks}


### 5.7 Bayesian neural networks {#5-dot-7-bayesian-neural-networks}

<!--list-separator-->

-  5.7.1 Posterior parameter distribution

<!--list-separator-->

-  5.7.2 Hyperparameter optimization

<!--list-separator-->

-  5.7.3 Bayesian neural networks for classification


## 6. Kernel methods {#6-dot-kernel-methods}


### 6.0 Introduction {#6-dot-0-introduction}


### 6.1 Dual representations {#6-dot-1-dual-representations}


### 6.2 Constructing kernels {#6-dot-2-constructing-kernels}


### 6.3 Radial basis function networks {#6-dot-3-radial-basis-function-networks}

<!--list-separator-->

-  6.3.1 Nadaraya-Watson model


### 6.4 Gaussian processes [key subsection]({{< relref "key_subsection" >}}) {#6-dot-4-gaussian-processes-key-subsection--key-subsection-dot-md}

<!--list-separator-->

-  6.4.1 Linear regression revisited

<!--list-separator-->

-  6.4.2 Gaussian processes for regression

<!--list-separator-->

-  6.4.3 Learning the hyperparameters

<!--list-separator-->

-  6.4.4 Automatic relevance determination

<!--list-separator-->

-  6.4.5 Gaussian processes for classification

<!--list-separator-->

-  6.4.6 Laplace approximation

<!--list-separator-->

-  6.4.7 Connection to neural networks

    <!--list-separator-->

    -  In a Bayesian neural network, the prior distribution over the parameter vector w, in conjunction with the network function f(x,w), produces a prior distribution over functions from y(x) where y is the vector of network outputs. Neal (1996) has shown that, for a broad class of prior distributions over w, the distribution of functions generated by a neural network will tend to a Gaussian process in the limit M →∞. It should be noted, however, that in this limit the output variables of the neural network become independent. One of the great merits of neural networks is that the outputs share the hidden units and so they can ‘borrow statistical strength’ from each other, that is, the weights associated with each hidden unit are influenced by all of the output variables not just by one of them. This property is therefore lost in the Gaussian process limit.


## 7. Sparse kernel machines {#7-dot-sparse-kernel-machines}


### 7.1 Maximum margin classifiers {#7-dot-1-maximum-margin-classifiers}

<!--list-separator-->

-  7.1.1 Overlapping class distributions

<!--list-separator-->

-  7.1.2 Relation to logistic regression

<!--list-separator-->

-  7.1.3 Multiclass SVMs

<!--list-separator-->

-  7.1.4 SVMs for regression

<!--list-separator-->

-  7.1.5 Computational learning theory


### 7.2 Relevance vector machines {#7-dot-2-relevance-vector-machines}

<!--list-separator-->

-  7.2.1 RVM for regression

<!--list-separator-->

-  7.2.2 Analysis of sparsity

<!--list-separator-->

-  7.2.3 RVM for classification


## 8. Graphical models {#8-dot-graphical-models}


### 8.1 Bayesian networks {#8-dot-1-bayesian-networks}

<!--list-separator-->

-  8.1.1 Example: polynomial regression

<!--list-separator-->

-  8.1.2 Generative models

<!--list-separator-->

-  8.1.3 Discrete variables

<!--list-separator-->

-  8.1.4 Linear-Gaussian models


### 8.2 Conditional independence {#8-dot-2-conditional-independence}

<!--list-separator-->

-  8.2.1 Three example graphs

<!--list-separator-->

-  8.2.2 D-separation


### 8.3 Markov random fields {#8-dot-3-markov-random-fields}

<!--list-separator-->

-  8.3.1 Conditional independence properties

<!--list-separator-->

-  8.3.2 Factorization properties

<!--list-separator-->

-  8.3.3 Illustration: Image de-noising

<!--list-separator-->

-  8.3.4 Relation to directed graphs


### 8.4 Inference in graphical models {#8-dot-4-inference-in-graphical-models}

<!--list-separator-->

-  8.4.1 Inference on a chain

<!--list-separator-->

-  8.4.2 Trees

<!--list-separator-->

-  8.4.3 Factor graphs

<!--list-separator-->

-  8.4.4 The sum-product algorithm

<!--list-separator-->

-  8.4.5 The max-sum algorithm

<!--list-separator-->

-  8.4.6 Exact inference in general graphs

<!--list-separator-->

-  8.4.7 Loopy belief propagation

<!--list-separator-->

-  8.4.8 Learning the graph structure


## 9. Mixture models and expectation maximization (EM) {#9-dot-mixture-models-and-expectation-maximization--em}


### 9.1 K-means clustering {#9-dot-1-k-means-clustering}

<!--list-separator-->

-  9.1.1 Image segmentation and compression


### 9.2 Mixtures of Gaussians {#9-dot-2-mixtures-of-gaussians}

<!--list-separator-->

-  9.2.1 Maximum likelihood

<!--list-separator-->

-  9.2.2 EM for Gaussian mixtures


### 9.3 An alternative view of EM {#9-dot-3-an-alternative-view-of-em}

<!--list-separator-->

-  9.3.1 Gaussian mixtures revisited

<!--list-separator-->

-  9.3.2 Relation to K-means

<!--list-separator-->

-  9.3.3 Mixtures of Bernoulli distributions

<!--list-separator-->

-  9.3.4 EM for Bayesian linear regression


### 9.4 The EM algorithm in general {#9-dot-4-the-em-algorithm-in-general}


## 10. Approximate inference {#10-dot-approximate-inference}


### 10.1 Variational inference {#10-dot-1-variational-inference}

<!--list-separator-->

-  10.1.1 Factorized distributions

<!--list-separator-->

-  10.1.2 Properties of factorized approximations

<!--list-separator-->

-  10.1.3 Example: the univariate Gaussian

<!--list-separator-->

-  10.1.4 Model comparison


### 10.2 Illustration: Variational mixture of Gaussians {#10-dot-2-illustration-variational-mixture-of-gaussians}

<!--list-separator-->

-  10.2.1 Variational distribution

<!--list-separator-->

-  10.2.2 Variational lower bound

<!--list-separator-->

-  10.2.3 Predictive density

<!--list-separator-->

-  10.2.4 Determining the number of components

<!--list-separator-->

-  10.2.5 Induced factorizations


### 10.3 Variational linear regression {#10-dot-3-variational-linear-regression}

<!--list-separator-->

-  10.3.1 Variational distribution

<!--list-separator-->

-  10.3.2 Predictive distribution

<!--list-separator-->

-  10.3.3 Lower bound


### 10.4 Exponential family distributions {#10-dot-4-exponential-family-distributions}

<!--list-separator-->

-  10.4.0 Introduction

    <!--list-separator-->

    -  Up to now we have grouped the variables in the model into ****observed variables**** and ****hidden variables****. We now make a further distinction between <span class="underline"><span class="underline">latent variables</span></span>, denoted \\[Z\\], and <span class="underline"><span class="underline">parameters</span></span>, denoted \\[\theta\\], where ****parameters**** are ****intensive**** ^^(fixed in number independent of the size of the data set)^^, whereas ****latent variables**** are ****extensive**** ^^(scale in number with the size of the data set)^^.

<!--list-separator-->

-  10.4.1 Variational message passing


### 10.5 Local variational methods {#10-dot-5-local-variational-methods}


### 10.6 Variational logistic regression {#10-dot-6-variational-logistic-regression}

<!--list-separator-->

-  10.6.1 Variational posterior distribution

<!--list-separator-->

-  10.6.2 Optimizing the variational parameters

<!--list-separator-->

-  10.6.3 Inference of hyperparameters


### 10.7 Expectation propagation {#10-dot-7-expectation-propagation}

<!--list-separator-->

-  10.7.1 Example: the clutter problem

<!--list-separator-->

-  10.7.2 Expectation propagation on graphs


## 11. Sampling methods {#11-dot-sampling-methods}


### 11.1 Basic sampling algorithms {#11-dot-1-basic-sampling-algorithms}

<!--list-separator-->

-  11.1.1 Standard distributions

<!--list-separator-->

-  11.1.2 Rejection sampling

<!--list-separator-->

-  11.1.3 Adaptive rejection sampling

<!--list-separator-->

-  11.1.4 Importance sampling

<!--list-separator-->

-  11.1.5 Sampling-importance-resampling

<!--list-separator-->

-  11.1.6 Sampling and the EM algorithm


### 11.2 Markov Chain Monte Carlo {#11-dot-2-markov-chain-monte-carlo}

<!--list-separator-->

-  11.2.1 Markov chains

<!--list-separator-->

-  11.2.2 The Metropolis-Hastings algorithm


### 11.3 Gibbs sampling {#11-dot-3-gibbs-sampling}


### 11.4 Slice sampling {#11-dot-4-slice-sampling}


### 11.5 The hybrid Monte Carlo algorithm {#11-dot-5-the-hybrid-monte-carlo-algorithm}

<!--list-separator-->

-  11.5.1 Dynamical systems

<!--list-separator-->

-  11.5.2 Hybrid Monte Carlo


### 11.6 Estimating the partition function {#11-dot-6-estimating-the-partition-function}


## 12. Continuous latent variables {#12-dot-continuous-latent-variables}


### 12.1 Principal component analysis {#12-dot-1-principal-component-analysis}

<!--list-separator-->

-  12.1.1 Maximum variance formulation

<!--list-separator-->

-  12.1.2 Minimum-error formulation

<!--list-separator-->

-  12.1.3 Applications of PCA

<!--list-separator-->

-  12.1.4 PCA for high-dimensional data


### 12.2 Probabilistic PCA {#12-dot-2-probabilistic-pca}

<!--list-separator-->

-  12.2.1 Maximum likelihood PCA

<!--list-separator-->

-  12.2.2 EM algorithm for PCA

<!--list-separator-->

-  12.2.3 Bayesian PCA

<!--list-separator-->

-  12.2.4 Factor analysis


### 12.3 Kernel PCA {#12-dot-3-kernel-pca}


### 12.4 Nonlinear latent variable models {#12-dot-4-nonlinear-latent-variable-models}

<!--list-separator-->

-  12.4.1 Independent component analysis

<!--list-separator-->

-  12.4.2 Autoassociative neural networks

<!--list-separator-->

-  12.4.3 Modelling nonlinear manifolds


## 13. Sequential data {#13-dot-sequential-data}


### 13.0 Introduction {#13-dot-0-introduction}

<!--list-separator-->

-  Although such models are tractable, they are also severely limited. We can obtain a more general framework, while still retaining tractability, by the introduction of latent variables, leading to state space models.

<!--list-separator-->

-  The two most important examples of state space models are the hidden Markov model, in which the latent variables are discrete, and linear dynamical systems, in which the latent variables are Gaussian.

<!--list-separator-->

-  Both models are described by directed graphs having a tree structure (no loops) for which inference can be performed efficiently using the sum-product algorithm.


### 13.1 Markov models {#13-dot-1-markov-models}


### 13.2 Hidden Markov models {#13-dot-2-hidden-markov-models}

<!--list-separator-->

-  13.2.1 Maximum likelihood for the HMM

<!--list-separator-->

-  13.2.2 The forward-backward algorithm

<!--list-separator-->

-  13.2.3 The sum-product algorithm for the HMM

<!--list-separator-->

-  13.2.4 Scaling factors

<!--list-separator-->

-  13.2.5 The Viterbi algorithm

<!--list-separator-->

-  13.2.6 Extensions of the hidden Markov model


### 13.3 Linear dynamical systems {#13-dot-3-linear-dynamical-systems}

<!--list-separator-->

-  13.3.0 Introduction

    <!--list-separator-->

    -  We now consider extensions to other distributions for the latent variables. In particular, we consider continuous latent variables in which the summations of the sum-product algorithm become integrals. The general form of the inference algorithms will, however, be the same as for the hidden Markov model. ^^It is interesting to note that, historically, hidden Markov models and linear dynamical systems were developed independently. Once they are both expressed as graphical models, however, the deep relationship between them immediately becomes apparent.^^

    <!--list-separator-->

    -  Because the linear dynamical system is a linear-Gaussian model, the joint distribution over all variables, as well as all marginals and conditionals, will be Gaussian. It follows that ^^the sequence of individually most probable latent variable values is the same as the most probable latent sequence. There is thus no need to consider the analogue of the Viterbi algorithm for the linear dynamical system.^^

<!--list-separator-->

-  13.3.1 Inference in LDS

<!--list-separator-->

-  13.3.2 Learning in LDS

<!--list-separator-->

-  13.3.3 Extensions of LDS

<!--list-separator-->

-  13.3.4 Particle filters


## 14. Combining models {#14-dot-combining-models}


### 14.1 Bayesian model averaging {#14-dot-1-bayesian-model-averaging}


### 14.2 Committees {#14-dot-2-committees}


### 14.3 Boosting {#14-dot-3-boosting}

<!--list-separator-->

-  14.3.1 Minimizing exponential error

<!--list-separator-->

-  14.3.2 Error functions for boosting


### 14.4 Tree-based models {#14-dot-4-tree-based-models}


### 14.5 Conditional mixture models {#14-dot-5-conditional-mixture-models}

<!--list-separator-->

-  14.5.1 Mixtures of linear regression models

<!--list-separator-->

-  14.5.2 Mixtures of logistic models

<!--list-separator-->

-  14.5.3 Mixtures of experts
