Lora.jl
==============================

[![Build Status](https://travis-ci.org/JuliaStats/MCMC.jl.png)](https://travis-ci.org/JuliaStats/MCMC.jl)
[![MCMC](http://pkg.julialang.org/badges/MCMC_release.svg)](http://pkg.julialang.org/?pkg=MCMC&ver=release)
[![Docs](https://readthedocs.org/projects/mcmcjl/badge/?version=latest)](http://mcmcjl.readthedocs.org/en/latest/)

*MCMC* has moved to *Lora*. Development in *Lora* will continue. *MCMC* is a placeholder for the future merge of
various independent MCMC implementations in Julia, including *Lora*.

The *Lora* package has just gone through a major upgrade. For this reason, some aspects of the packages haven't been
fully ported yet. Furthermore, the README package is not entirely up-to-date. The porting of the remaining code and
the documentation will be completely ready in a few days' time. All the basic functionality of the package is already
available as far as serial simulations are concerned.

The Julia *Lora* package provides a generic engine for Markov Chain Monte Carlo (MCMC) inference.


Features
------------------------------

Briefly, *Lora* implements:

* imperative model specification,
* a range of Monte Carlo samplers,
* serial and sequential Monte Carlo methods,
* tuning of the samplers' parameters,
* various job managers for controlling the flow of simulations,
* descriptive statistics for MCMC and MCMC diagnostic tools,
* output managemement,
* resuming Monte Carlo simulations,
* Monte Carlo sampling with the help of automatic differentiation.


Outline
------------------------------

*Jobs* are the central input entities for handling MCMC simulations. A job is first instantiated to delineate the MCMC
configuration. The main defining components of a job are the *model*, *sampler* and *runner*. Once set up, the job can
be run or resumed.

*Chains* form the building block for managing the output of MCMC simulations. Jobs return chains. Descriptive
statistics, MCMC diagnostics and output processing can be performed on chains.


Documentation
------------------------------

* [User Guide](http://mcmcjl.readthedocs.org/en/latest/) ([PDF](https://readthedocs.org/projects/mcmcjl/downloads/pdf/latest/))
* Cheat Sheet (to appear soon)
