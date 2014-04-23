AD_StatTest-julia
=================

An implementation of the Anderson Darling statistical test for exponential or Rayleigh distributions in Julia

Requirements
____________

* Julia v0.2+

Example
_______

    using Distributions
    include("ADTest.jl")
    X = rand(Exponential(1),100);
    ADTest(X,"Exponential")
    ADTest(sqrt(X),"Rayleigh")
