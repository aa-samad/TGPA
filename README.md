# TGPA - forked

how to use these codes:

## Install julia language
- currently Ubuntu 16.04LTS tested and working
- windows 64bit not working (install of some packages not successful)!

## Pre-requisiteries 
- julia packages (type the following commands inside julia console)
    - MatrixNetworks
    	- ```import Pkg; Pkg.add("MatrixNetworks")```
    - Distributions
    	- ```import Pkg; Pkg.add("Distributions")```
    - PyCall
    	- ```import Pkg; Pkg.add("PyCall")```
    - ColorTypes
        - ```import Pkg; Pkg.add("ColorTypes")``` 
- python packages
    - igraph
        - ```pip3 install igraph```


## Tests
- run test.jl to check julia working (expect no output if there was no problem!)
    - if you install **julia >= 1.0**: edit ```using base.Test``` line to ```using Test```
- run HOC_test.jl to get the values of higher clustering coeff of TGPA per given parameters
- run Visualize_Network.jl


