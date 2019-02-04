# LatticePhysics Tutorials

Tutorials and Examples for the julia module [`LatticePhysics.jl`](https://github.com/janattig/LatticePhysics.jl) for julia version `1.0.*`.
The tutorials are presented in the form of `IJulia` notebooks, therefore the `IJulia` package is mandatory to install.


## How to use `IJulia` notebooks

After installing all modules (i.e. [`LatticePhysics.jl`](https://github.com/janattig/LatticePhysics.jl), linked plotting libraries as well as `IJulia` and `PyPlot`), one can clone this repository into a local directory and navigate a julia REPL there. Then, use
```julia-REPL
julia> using IJulia
julia> notebook(dir="")
```
to open a new julia notebook in the browser within the current directory. Navigate to the tutorial file of your choice within jupyter
and open the tutorial there as well.



## Table of Contents

1.  **Introduction**
    - first tutorial and introduction to general workflow of `LatticePhysics.jl` [[notebook](https://github.com/janattig/LatticePhysics_Tutorials/blob/master/introduction/introduction.ipynb)]
2.  **Basic Types**
    1. _Sites_ and _Bonds_
        -  site types and interface [[notebook](https://github.com/janattig/LatticePhysics_Tutorials/blob/master/basics/sites_bonds/site_type_interface.ipynb)]
        -  site dispatch examples [[notebook](https://github.com/janattig/LatticePhysics_Tutorials/blob/master/basics/sites_bonds/site_dispatch.ipynb)]
        -  bond types and interface [[notebook](https://github.com/janattig/LatticePhysics_Tutorials/blob/master/basics/sites_bonds/bond_type_interface.ipynb)]
        -  bond dispatch examples [[notebook](https://github.com/janattig/LatticePhysics_Tutorials/blob/master/basics/sites_bonds/bond_dispatch.ipynb)]
    2. _Unitcells_
        -  unitcell types and interface [[notebook](https://github.com/janattig/LatticePhysics_Tutorials/blob/master/basics/unitcells/unitcell_type_interface.ipynb)]
        -  how to access pre-implemented unitcells [[notebook](https://github.com/janattig/LatticePhysics_Tutorials/blob/master/basics/unitcells/pre-implemented_unitcells.ipynb)]
        -  how to extend pre-implemented unitcells and define your own [[notebook](https://github.com/janattig/LatticePhysics_Tutorials/blob/master/basics/unitcells/implementing_new_unitcells.ipynb)]
        -  unitcell dispatch examples [[notebook](https://github.com/janattig/LatticePhysics_Tutorials/blob/master/basics/unitcells/unitcell_dispatch.ipynb)]
    3. _Lattices_
        -  lattice types and interface [[notebook](https://github.com/janattig/LatticePhysics_Tutorials/blob/master/basics/lattices/lattice_type_interface.ipynb)]
        -  pre-implemented lattice building from unitcells [[notebook](https://github.com/janattig/LatticePhysics_Tutorials/blob/master/basics/lattices/lattice_building.ipynb)]
        -  lattice dispatch examples [[TODO](https://github.com/janattig/LatticePhysics_Tutorials/blob/master/basics/lattices/lattice_dispatch.ipynb)]
        -  lattice tips and tricks [TODO] (accessing organized bonds, ...)
    4. _Reciprocal space_
        -  reciprocal point type and interface [TODO]
        -  reciprocal path type and interface [TODO]
        -  building reciprocal paths [TODO]
        -  reciprocal unitcell type and interface [TODO]
        -  Brillouin zone type and interface [TODO]
        -  building Brillouin zones [TODO]
3.  **Plotting (in PyPlot)**
    1. _Lattices_
        -  introduction to plotting of lattices [[notebook](https://github.com/janattig/LatticePhysics_Tutorials/blob/master/plotting_PyPlot/lattices/plotting_lattice_introduction.ipynb)]
        -  plotting lattices in 2D [TODO]
        -  plotting lattices in 3D [TODO]
        -  plotting tips and tricks [TODO] (site colors, faster plots, ...)
    2. _Reciprocal space_
        -  plotting Brillouin zones [TODO]
        -  plotting reciprocal paths [TODO]
4.  **Luttinger Tisza calculations**
    1. _Introduction_ [TODO]
    2. _Hamiltonians_
        - bond hamiltonian type and interface [TODO]
        - bond hamiltonian dispatch examples [TODO]
        - how to engineer your own hamiltonain [TODO]
    3. _Luttinger Tisza ground states_
        - calculating Luttinger Tisza ground states [TODO]
    4. _Plotting of Luttinger Tisza ground states_
        - plotting Luttinger Tisza ground states [TODO]




## Basic Workflow of `LatticePhysics.jl`

The main workflow of `LatticePhysics.jl` can be captured in three main steps
1.  Create (and modify) a `Unitcell` object
2.  Create (and modify) a `Lattice` object out of the `Unitcell` object
3.  Use either of those two objects for a variety of applications:
    - plotting
    - Monte Carlo
    - Luttinger Tisza analysis
    - ...
