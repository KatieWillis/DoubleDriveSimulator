# DoubleDriveSimulator
___
This repository contains jupyter notebooks associated with the paper "Double drives and private alleles for localised population genetic control" pending publication in PLOS Genetics, and available at https://www.biorxiv.org/content/10.1101/2021.01.08.425856v2.

Katie Willis1 and Austin Burt1.

1 Department of Life Sciences, Imperial College, Silwood Park, Ascot, SL5 7PY, UK

For correspondence: katie.willis16@imperial.ac.uk

___
## Requirements

* Jupyter notebook
* Julia 1.5 or above
* All dependencies can be installed by running the following code in julia from the location of the downloaded files (This only needs to be done once) 
```
using Pkg
Pkg.activate("./Project/")
Pkg.instantiate()
```

The environment can then be loaded at the beginning of each jupyter session by running the following:
```
] activate "./Project/"
```
___
## User notes

For clarity some parameter labels have been changed for publication. None of the differences result in changes to the results, but are noteworthy to aid interpretation of the code.

* Allele labels differ in the baseline and 4-allele models compared to publication. In the publication α and β refer to the construct and a and b refer to cleavage-resistant alleles, whereas in the code this is reversed.
* Locus labels differ in the 4-allele model compared to publication. In the publication the differentiated site (the locus with 4 alleles) is the insertion site for the β construct, whereas in the code this is the insertion site for the α construct.
* In the publication μ refers to the homing-associated loss-of-function probability, in the code this is referred to as d.
* In the publication gamma refers to the density-dependent parameter of the Beverton-Holt population dynamics model, in the code this is referred to as α, not to be confused with the allele label α which is not a user-defined parameter.
