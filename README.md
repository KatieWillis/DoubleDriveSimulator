# DoubleDriveSimulator
___
This repository contains jupyter notebooks associated with the paper "Double drives and private alleles for localised population genetic control" pending publication in PLOS Genetics, and available at https://www.biorxiv.org/content/10.1101/2021.01.08.425856v2.

Katie Willis1 and Austin Burt1.

1 Department of Life Sciences, Imperial College, Silwood Park, Ascot, SL5 7PY, UK

For correspondence: katie.willis16@imperial.ac.uk

This code is currently being used for other projects...
___
## Requirements

* Julia 1.5 or above
* Jupyter notebook
* The following Julia packages: 
    * NBInclude
    * SymPy
    * DataFrames
    * LinearAlgebra
    * CSV
    * Distributed
    * Plots
    * PyPlot
___
## User notes

For clarity some parameter labels have been changed for publication. None of the differences result in changes to the results, but are noteworthy to aid interpretation of the code.

* Allele labels differ in the baseline and 4-allele models compared to publication. In the publication α and β refer to the construct and a and b refer to cleavage-resistant alleles, whereas in the code this is reversed. 
* Locus labels differ in the 4-allele model compared to publication. In the publication the differentiated site (the locus with 4 alleles) is the insertion site for the β construct, whereas in the code this is the insertion site for the α construct.
* In the publication μ refers to the homing-associated loss-of-function probability, in the code this is referred to as d.
* In the publication gamma refers to the density-dependent parameter of the Beverton-Holt population dynamics model, in the code this is referred to as α, not to be confused with the allele label α which is not a user-defined parameter.