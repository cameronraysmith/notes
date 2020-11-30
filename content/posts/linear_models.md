+++
title = "linear models"
author = ["Cameron Smith"]
lastmod = 2020-11-30T00:42:14-05:00
slug = "linear_models"
draft = false
+++

## [statistics]({{< relref "statistics" >}}), [probabilistic inference]({{< relref "probabilistic_inference" >}}), [model construction]({{< relref "model_construction" >}}) {#statistics--statistics-dot-md--probabilistic-inference--probabilistic-inference-dot-md--model-construction--model-construction-dot-md}


## references {#references}

-   <https://en.wikipedia.org/wiki/Generalized%5Flinear%5Fmodel#Link%5Ffunction>
-   <sup id="108a9c399b8f98eb2a775abba7ac1e4d"><a href="#Gelman2006" title="Gelman \&amp; Hill, {Data Analysis Using Regression and Multilevel/Hierarchical Models}, Cambridge University Press (2006).">Gelman2006</a></sup><sup>,</sup><sup id="2d9f9e8d5ebdccee1bcd79a3334839ba"><a href="#Gelman2014" title="Gelman, Carlin, Stern, Dunson, Vehtari \&amp; Rubin, {Bayesian Data Analysis}, (2014).">Gelman2014</a></sup><sup>,</sup><sup id="74996cdbeac95be74bb458cbb6fa2381"><a href="#McElreath2019" title="McElreath, {Statistical Rethinking: A Bayesian Course with Examples in R and STAN}, Chapman and Hall/CRC (2020).">McElreath2019</a></sup><sup>,</sup><sup id="ca9b820c33d6bd378a227b35718b35e0"><a href="#Barber2012" title="Barber, {Bayesian Reasoning and Machine Learning}, Cambridge University Press (2012).">Barber2012</a></sup><sup>,</sup><sup id="603a9cec1ef00532d826b458b4001cff"><a href="#Bishop2007" title="Bishop, {Pattern Recognition and Machine Learning (Information Science and Statistics)}, Springer (2007).">Bishop2007</a></sup>


## test remote jupyter kernel {#test-remote-jupyter-kernel}

```jupyter-julia
x = "foo"
y = "bar"
println(x)
println(y)
```


## examples {#examples}

In most cases we do not need to modify the default `:results output verbatim replace` in the `:header-args:`. See [Header arguments - Org Babel reference card](https://org-babel.readthedocs.io/en/latest/header-args/#results).


### julia tests {#julia-tests}

<a id="code-snippet--define-vars"></a>
```jupyter-julia
x = "foo"
y = "bar"
println(x)
println(y)
```

```text
foo
bar
```

Since `jupyter-julia` supports sessions, we can make use of the variables defined in the previous block

```jupyter-julia
print(join([x, " ", y]))
```

```text
foo bar
```


### load common libraries {#load-common-libraries}

Load libraries

```jupyter-julia
@time begin
using Dates
using Turing
using CSV, DataFrames, Distributions
using MCMCChains, StatsFuns, StatsPlots
end
now()
```

```text
 35.783676 seconds (79.42 M allocations: 4.116 GiB, 4.30% gc time)
2020-10-29T21:39:30.7
```

Print list of loaded modules

```jupyter-julia
loaded_modules = Base.loaded_modules_array()
println(loaded_modules)
now()
```


### models {#models}

<!--list-separator-->

-  testing

    <!--list-separator-->

    -  model definition

        See [load libraries](#load-common-libraries) for those used across examples.

        ```jupyter-julia
        @time begin
        end
        now()
        ```

        Print current working directory

        ```jupyter-julia
        println(pwd())
        now()
        ```

        ```text
        /Users/crs58/projects/notes/org
        2020-10-17T11:24:44.226
        ```

        Define the `Turing.jl` model

        ```jupyter-julia

        @time begin
        # Define a simple Normal model with unknown mean and variance.
        @model gdemo(x, y) = begin
            s ~ InverseGamma(2, 3)
            m ~ Normal(0, sqrt(s))
            x ~ Normal(m, sqrt(s))
            y ~ Normal(m, sqrt(s))
        end
        end
        now()

        ```

        ```text
          0.000082 seconds (85 allocations: 7.407 KiB)
        2020-10-29T21:39:51.823
        ```

    <!--list-separator-->

    -  sampling

        Run and profile the sampler

        ```jupyter-julia
        #  Run sampler, collect results
        @time chn = sample(gdemo(1.5, 2), NUTS(0.65), 1000)
        now()
        ```

        ```text
        ┌ Info: Found initial step size
        │   ϵ = 1.6
        └ @ Turing.Inference /Users/crs58/.julia/packages/Turing/RzDvB/src/inference/hmc.jl:625
        Sampling: 100%|█████████████████████████████████████████| Time: 0:00:00
         16.546298 seconds (42.02 M allocations: 2.128 GiB, 4.43% gc time)
        2020-10-29T21:40:08.642
        ```

        Print the result summary

        ```jupyter-julia
        # Summarise results (currently requires the master branch from MCMCChains)
        display(chn)
        # describe(chn; sections = :internals)
        # show(stdout, "text/plain", chn)
        now()
        ```

        ```text
        Chains MCMC chain (500×14×1 Array{Float64,3}):

        Iterations        = 1:500
        Thinning interval = 1
        Chains            = 1
        Samples per chain = 500
        parameters        = m, s
        internals         = acceptance_rate, hamiltonian_energy, hamiltonian_energy_error, is_accept, log_density, lp, max_hamiltonian_energy_error, n_steps, nom_step_size, numerical_error, step_size, tree_depth

        Summary Statistics
          parameters      mean       std   naive_se      mcse        ess      rhat
              Symbol   Float64   Float64    Float64   Float64    Float64   Float64

                   m    1.2898    0.8406     0.0376    0.0795   138.8908    1.0138
                   s    1.9378    1.6108     0.0720    0.1375   109.5077    1.0028

        Quantiles
          parameters      2.5%     25.0%     50.0%     75.0%     97.5%
              Symbol   Float64   Float64   Float64   Float64   Float64

                   m   -0.1236    0.7457    1.2822    1.7125    2.9355
                   s    0.6235    1.1054    1.5581    2.1717    5.7594
        ```

        ```text
        2020-10-29T21:40:39.455
        ```

    <!--list-separator-->

    -  plotting

        <!--list-separator-->

        -  statsplots

            Plot the results

            ```jupyter-julia
            # Plot and save results
            p = plot(chn)
            savefig("data/linear_models/basic-example-plot.pdf")
            savefig("data/linear_models/basic-example-plot.png")
            ```

            {{< figure src="/ox-hugo/basic-example-plot.png" >}}

        <!--list-separator-->

        -  arviz

            Load additional libraries

            ```jupyter-julia
            using ArviZ, PyPlot, PyCall
            now()
            ```

            ```text
            2020-10-29T21:40:50.04
            ```

            The following may be useful if the `Latin Modern` fonts are not installed or setup to work with `matplotlib`.

            ```text
            mpl = pyimport("matplotlib")
            mplfm = pyimport("matplotlib.font_manager")
            mplfm.fontManager.addfont("~/Library/Fonts/lmsans10-regular.otf")
            mplfm.fontManager.addfont("~/Library/Fonts/lmroman10-regular.otf")
            mplfm.findfont("Latin Modern Sans")
            mplfm._rebuild()
            print(mpl.rcParams)
            ```

            Make `InferenceData` object

            ```jupyter-julia
            idata = from_mcmcchains(chn, library = "Turing")
            ```

            ```text
            InferenceData with groups:
            	> posterior
            	> sample_stats
            ```

            Print posterior and `sample_stats` from `InferenceData` object

            ```jupyter-julia
            print(idata.posterior)
            print(idata.sample_stats)
            now()
            ```

            ```text
            Dataset (xarray.Dataset)
            Dimensions:  (chain: 1, draw: 500)
            Coordinates:
              * chain    (chain) int64 0
              * draw     (draw) int64 0 1 2 3 4 5 6 7 8 ... 492 493 494 495 496 497 498 499
            Data variables:
                m        (chain, draw) float64 1.589 1.183 3.026 ... -0.02606 1.485 -0.3521
                s        (chain, draw) float64 1.985 1.348 5.464 1.353 ... 1.573 1.399 4.237
            Attributes:
                created_at:         2020-10-18T18:52:46.016452
                arviz_version:      0.9.0
                inference_library:  TuringDataset (xarray.Dataset)
            Dimensions:           (chain: 1, draw: 500)
            Coordinates:
              * chain             (chain) int64 0
              * draw              (draw) int64 0 1 2 3 4 5 6 ... 493 494 495 496 497 498 499
            Data variables:
                energy            (chain, draw) float64 5.718 5.12 8.651 ... 5.826 8.27
                energy_error      (chain, draw) float64 0.115 -0.09808 ... -0.2852 0.4234
                depth             (chain, draw) int64 2 2 2 2 1 2 2 2 2 ... 2 1 2 2 2 1 2 2
                diverging         (chain, draw) bool False False False ... False False False
                log_density       (chain, draw) float64 -5.151 -4.634 -8.2 ... -4.762 -7.393
                max_energy_error  (chain, draw) float64 0.2966 -0.09808 ... -0.2852 0.4626
                nom_step_size     (chain, draw) float64 0.7675 0.7675 ... 0.7675 0.7675
                is_accept         (chain, draw) float64 1.0 1.0 1.0 1.0 ... 1.0 1.0 1.0 1.0
                tree_size         (chain, draw) int64 7 3 3 7 1 3 7 3 3 ... 3 1 3 3 3 1 7 3
                lp                (chain, draw) float64 -5.151 -4.634 -8.2 ... -4.762 -7.393
                step_size         (chain, draw) float64 0.7675 0.7675 ... 0.7675 0.7675
                mean_tree_accept  (chain, draw) float64 0.8756 1.0 0.5808 ... 0.985 0.6447
            Attributes:
                created_at:         2020-10-18T18:52:46.263700
                arviz_version:      0.9.0
                inference_library:  Turing
            ```

            ```text
            2020-10-18T14:55:35.997
            ```

            Plot

            ```jupyter-julia
            # Plot and save results
            p_arviz_trace = plot_trace(idata)
            PyPlot.savefig("data/linear_models/normal-model-arviz-trace.pdf")
            PyPlot.savefig("data/linear_models/normal-model-arviz-trace.png")
            ```

            {{< figure src="/ox-hugo/normal-model-arviz-trace.png" >}}

<!--list-separator-->

-  template

    <!--list-separator-->

    -  model definition

        See [load libraries](#load-common-libraries) for those used across examples.

        Define the `Turing.jl` model

        ```jupyter-julia

        @time begin
        # Define a simple Normal model with unknown mean and variance.
        @model gdemo(x, y) = begin
            s ~ InverseGamma(2, 3)
            m ~ Normal(0, sqrt(s))
            x ~ Normal(m, sqrt(s))
            y ~ Normal(m, sqrt(s))
        end
        end
        now()

        ```

        ```text
          0.000082 seconds (85 allocations: 7.407 KiB)
        2020-10-29T21:39:51.823
        ```

    <!--list-separator-->

    -  sampling

        Run and profile the sampler

        ```jupyter-julia
        #  Run sampler, collect results
        @time chn = sample(gdemo(1.5, 2), NUTS(0.65), 1000)
        now()
        ```

        ```text
        ┌ Info: Found initial step size
        │   ϵ = 1.6
        └ @ Turing.Inference /Users/crs58/.julia/packages/Turing/RzDvB/src/inference/hmc.jl:625
        Sampling: 100%|█████████████████████████████████████████| Time: 0:00:00
         16.546298 seconds (42.02 M allocations: 2.128 GiB, 4.43% gc time)
        2020-10-29T21:40:08.642
        ```

        Print the result summary

        ```jupyter-julia
        # Summarise results (currently requires the master branch from MCMCChains)
        display(chn)
        # describe(chn; sections = :internals)
        # show(stdout, "text/plain", chn)
        now()
        ```

        ```text
        Chains MCMC chain (500×14×1 Array{Float64,3}):

        Iterations        = 1:500
        Thinning interval = 1
        Chains            = 1
        Samples per chain = 500
        parameters        = m, s
        internals         = acceptance_rate, hamiltonian_energy, hamiltonian_energy_error, is_accept, log_density, lp, max_hamiltonian_energy_error, n_steps, nom_step_size, numerical_error, step_size, tree_depth

        Summary Statistics
          parameters      mean       std   naive_se      mcse        ess      rhat
              Symbol   Float64   Float64    Float64   Float64    Float64   Float64

                   m    1.2898    0.8406     0.0376    0.0795   138.8908    1.0138
                   s    1.9378    1.6108     0.0720    0.1375   109.5077    1.0028

        Quantiles
          parameters      2.5%     25.0%     50.0%     75.0%     97.5%
              Symbol   Float64   Float64   Float64   Float64   Float64

                   m   -0.1236    0.7457    1.2822    1.7125    2.9355
                   s    0.6235    1.1054    1.5581    2.1717    5.7594
        ```

        ```text
        2020-10-29T21:40:39.455
        ```

    <!--list-separator-->

    -  plotting

        Load additional libraries

        ```jupyter-julia
        using ArviZ, PyPlot, PyCall
        now()
        ```

        ```text
        2020-10-29T21:40:50.04
        ```

        Make `InferenceData` object

        ```jupyter-julia
        idata = from_mcmcchains(chn, library = "Turing")
        ```

        ```text
        InferenceData with groups:
        	> posterior
        	> sample_stats
        ```

        Print posterior and `sample_stats` from `InferenceData` object

        ```jupyter-julia
        print(idata.posterior)
        print(idata.sample_stats)
        now()
        ```

        ```text
        Dataset (xarray.Dataset)
        Dimensions:  (chain: 1, draw: 500)
        Coordinates:
          * chain    (chain) int64 0
          * draw     (draw) int64 0 1 2 3 4 5 6 7 8 ... 492 493 494 495 496 497 498 499
        Data variables:
            m        (chain, draw) float64 1.589 1.183 3.026 ... -0.02606 1.485 -0.3521
            s        (chain, draw) float64 1.985 1.348 5.464 1.353 ... 1.573 1.399 4.237
        Attributes:
            created_at:         2020-10-18T18:52:46.016452
            arviz_version:      0.9.0
            inference_library:  TuringDataset (xarray.Dataset)
        Dimensions:           (chain: 1, draw: 500)
        Coordinates:
          * chain             (chain) int64 0
          * draw              (draw) int64 0 1 2 3 4 5 6 ... 493 494 495 496 497 498 499
        Data variables:
            energy            (chain, draw) float64 5.718 5.12 8.651 ... 5.826 8.27
            energy_error      (chain, draw) float64 0.115 -0.09808 ... -0.2852 0.4234
            depth             (chain, draw) int64 2 2 2 2 1 2 2 2 2 ... 2 1 2 2 2 1 2 2
            diverging         (chain, draw) bool False False False ... False False False
            log_density       (chain, draw) float64 -5.151 -4.634 -8.2 ... -4.762 -7.393
            max_energy_error  (chain, draw) float64 0.2966 -0.09808 ... -0.2852 0.4626
            nom_step_size     (chain, draw) float64 0.7675 0.7675 ... 0.7675 0.7675
            is_accept         (chain, draw) float64 1.0 1.0 1.0 1.0 ... 1.0 1.0 1.0 1.0
            tree_size         (chain, draw) int64 7 3 3 7 1 3 7 3 3 ... 3 1 3 3 3 1 7 3
            lp                (chain, draw) float64 -5.151 -4.634 -8.2 ... -4.762 -7.393
            step_size         (chain, draw) float64 0.7675 0.7675 ... 0.7675 0.7675
            mean_tree_accept  (chain, draw) float64 0.8756 1.0 0.5808 ... 0.985 0.6447
        Attributes:
            created_at:         2020-10-18T18:52:46.263700
            arviz_version:      0.9.0
            inference_library:  Turing
        ```

        ```text
        2020-10-18T14:55:35.997
        ```

        Plot

        ```jupyter-julia
        # Plot and save results
        p_arviz_trace = plot_trace(idata)
        PyPlot.savefig("data/linear_models/normal-model-arviz-trace.pdf")
        PyPlot.savefig("data/linear_models/normal-model-arviz-trace.png")
        ```

        {{< figure src="/ox-hugo/normal-model-arviz-trace.png" >}}
