# LatticePhysics Tutorials

Tutorials and Examples for the julia module [`LatticePhysics.jl`](https://github.com/janattig/LatticePhysics.jl) for julia version `1.0.*`.
The tutorials are presented in the form of `IJulia` notebooks, therefore the `IJulia` package is mandatory to install.



## Basic Workflow of `LatticePhysics.jl`

The main workflow of `LatticePhysics.jl` can be captured in three main steps
1.  Create (and modify) a `Unitcell` object
2.  Create (and modify) a `Lattice` object out of the `Unitcell` object
3.  Use either of those two objects for a variety of applications:
    - plotting
    - Monte Carlo
    - Luttinger Tisza analysis
    - ...


## Table of Contents

1.  _Basics_ -- covers most of the basic types of `LatticePhysics.jl`
    1. _Unitcells_
    2. _Lattices_
    3. _Reciprocal space_
2.  _Plotting (in PyPlot)_ -- covers plotting aspects of `LatticePhysics.jl` by using PyPlot
    1. _Lattices_
    2. _Reciprocal space_
