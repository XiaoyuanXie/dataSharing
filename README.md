### Evolving Ranking-Based Failure Proximities
This is the repository containing the data and source code for the paper "Evolving Ranking-Based Failure Proximities for Better
Clustering in Fault Isolation".

+ The folder `data` is threefold, including all individuals in each generation along with their fitness scores 
(in the training phase), 12 groups of REFs and 10 EFFs' fitness scores, and the values of *k* in the
scenario of "*k* ≠ *r*".
    * `allData (training).pdf` provides 2400 (160 individuals per generation * 15 generations)
        individuals' expressions and their fitness scores in the training phase.
    * `allData (test).pdf` provides 10 selected EFFs' expressions and fitness scores
       in the test phase.
    * `deviation.pdf` provides the values of *k* (the estimated number of faults) when it is not
       equal to *r* (the number of faults contained in the program).

+ The folder `code` is the source code of the proposed evolution framework.
    * `dependencies.py` lists the modules utilized in the framework.
    * `registration.py` initializes the services of the GP model and configures the evolving operators.
    * `initialPopulation.py` produces the initial population when the evolving process starts.
    * `select.py` performs the selection step to determine parents.
    * `getNextGeneration.py` conducts the operations of crossover, copy, or mutation, to deliver the next generation.
