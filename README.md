# Truck Scheduling at Container Terminals Project

> This repository contains project files to solve a truck scheduling problem using two models: a mixed integer programming (MIP) model built in Gurobi and a constraint programming (CP) model using CPLEX. 

## Setup

1. In the main directory, we have two iPythonNotebook (ipynb) files:
    * **cp_model.ipynb**
    * **mip_model.ipynb**
  
2. Each file can be opened in jupyter notebook as long as the appropriate packages are downloaded (see [Packages Used](#packages-used)).

3. Various instances (scenarios of different combinations of containers, carriers and chassis) are contained in the **instances** folder.  These were generated by the ipynb file: **instance_generator.ipynb**.  In total, there are 10 instances from base (1) to 10 that can be run by either model.  In order to run a respective instance, all that needs to be done is to change the file name in the code at the top of the document.

4. For the MIP model, html files will be generated for the chassis and container perspective in the same instance folder.

## Packages Used

* Python           - version 3.7.7
* jupyter notebook - version 6.1.4
* numpy            - version 1.19.1
* pandas           - version 1.1.3
* plotly           - version 4.12.0
* matplotlib       - version 3.3.1
* gurobi           - version 9.0.3
* docplex          - version 2.18.200

## References

1. **Gurobi Optimizer:** Gurobi is an industrial mixed-integer programming solver that works with many programming languages including Python.  In order to use Gurobi, you need an academic license, which can be found here: https://www.gurobi.com/academia/academic-program-and-licenses/.  In addition, you must download the gurobi software from this site or if you use the Anaconda Distribution for Python, you can run the following code:

  ```
  conda config --add channels http://conda.anaconda.org/gurobi
  conda install gurobi
  ```
2. **IBM Decision Optimization CPLEX (docplex):** docplex is IBM's CP solver using Python.  Similar to Gurobi, you will need to install the packages from this location: http://ibmdecisionoptimization.github.io/docplex-doc/getting_started_python.html#installing-the-cplex-modeling-library-with-pip.  On the Anaconda distribution, you can run the following code:

  ```
  conda install -c ibmdecisionoptimization docplex
  ```

