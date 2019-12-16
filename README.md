# TGPA - forked

how to use these codes:

## install julia language
    - currently Ubuntu 16.04LTS tested and working
    - windows 64bit not working (install of some packages not successful)!

## pre-requisiteries (type the following commands inside julia console)
	- MatrixNetworks package
		- ```import Pkg; Pkg.add("MatrixNetworks")```
	- Distributions package
		- ```import Pkg; Pkg.add("Distributions")```
    - PyCall package
		- ```import Pkg; Pkg.add("PyCall")```
    - ColorTypes package
        - ```import Pkg; Pkg.add("ColorTypes")``` 

## tests
- run test.jl to check julia working (expect no output if there was no problem!)
- run HOC_test.jl to get the values of higher clustering coeff of TGPA per given parameters
- run Visualize_Network.jl


