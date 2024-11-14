# Centre-based modelling of embryonic organoid development

![Language: Julia](https://img.shields.io/badge/language-Julia-ed207b)
![Jupyter Notebook](https://img.shields.io/badge/Notebook-Jupyter-f37821)

### This repository will eventually be moved to the [Multiscale Physics of Living Systems Group](https://github.com/MPoLS-lab)'s GitHub.

## Introduction

This repository contains the code, figures and report of my master thesis, titled "Centre-based modelling of embryonic organoid development", developed as part of the Master's degree in Advanced Mathematics and Mathematical Engineering at Universitat Politècnica de Catalunya. It was carried out at the Computational Biology and Complex Systems research group ([BIOCOM-SC](https://biocomsc.upc.edu/en)), and supervised by [David Oriola Santandreu](https://davidoriola.mystrikingly.com/). 

**The model has been programmed using [CellBasedModels.jl](https://github.com/dsb-lab/CellBasedModels.jl), the Julia package for multicellular modelling developed by Gabriel Torregrosa-Cortés.**

## Installation process

The following instructions provide a guide to set up your computer to run the code, and been tested to work on Linux and Windows.

Download Julia from [their website](https://julialang.org/downloads/). Download version 1.9 and, optionally, set it as default and remove the release version.

```
juliaup add 1.9
juliaup default 1.9
juliaup rm release
```

Run Julia.
```
julia
```
In case 1.9 is not the default version, run
```
julia +1.9
```

Add CellBasedModels.jl and the packages used across the code
```julia-repl
julia> using Pkg
julia> add CellBasedModels
julia> add DifferentialEquations, Distributions, Random, GLMakie, Printf, Dates, Glob, NBInclude, MathTeXEngine, IJulia
```
Note that IJulia is only necessary to run the notebooks in Jupyter notebooks. You can use [JupyterLab](https://jupyter.org/install). Another option is to use VS Code along with the Julia extension.

## Examples

Formation of an aggregate:

![](https://github.com/villegas-morral/masters-thesis/blob/d086ff95580073c4d3a6a28fdd8cde3903875bc3/figures/400-example-program/400-aggregate-formation.png)

Differentiation of an aggregate while it proliferates:

![](https://github.com/villegas-morral/masters-thesis/blob/d086ff95580073c4d3a6a28fdd8cde3903875bc3/figures/411-diff-adhesion-growing/411-aggregate-afaster-all.png)

![](https://github.com/villegas-morral/masters-thesis/blob/d086ff95580073c4d3a6a28fdd8cde3903875bc3/figures/411-diff-adhesion-growing/411-aggregate-afaster-b.png)
