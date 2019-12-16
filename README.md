# TGPA

this repo forked to explain the original repo and apply some changes (for newer Julia versions).

## Install julia language
- install Julia>=1.0
    - currently Ubuntu 16.04LTS tested and working
    - windows 64bit not working (install of some packages not successful)!
- install Julia 0.6
    - not tested, but apparently the original repo is made with this

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
    - HigherOrderClustering
        - if you have julia<0.7
            - ```import Pkg; Pkg.add("HigherOrderClustering")``` 
        - else
            - entering Pkg REPL
                - press **]** 
            - ```add  https://github.com/arbenson/HigherOrderClustering.jl.git```
            - exit Pkg REPL
                - press backspace
                
- python packages
    - igraph
        - ```sudo apt-get install libigraph0-dev```
        - ```pip3 install python-igraph ```


## Tests
- run test.jl to check julia working (expect no output if there was no problem!)
- run Visualize_Network.jl
- HOC_test.jl NOT WORKING with Julia >=0.7!
    - HigherOrderClustering is not supporting julia>=0.7
        - working on fixing the package for Julia>=0.7

## some edits to make the repo work!
- change ```using base.Test``` line to ```using Test``` inside test.jl
- change ```/Users/eikmeier/Dropbox/TGPA/WWW/images/``` strings(paths) in Visualize_Network.jl to ```./plots/```
- ... to make it work with julia >= 1.0 
    - no need to do it if you install julia<0.7
