# DoubleDriveSimulator
___
This repository contains jupyter notebooks associated with the publication "Double drives and private alleles for localised population genetic control" available at https://journals.plos.org/plosgenetics/article?id=10.1371/journal.pgen.1009333.

We are currently using this to explore other questions. If you are interested in extending the code please get in touch.

Katie Willis1 and Austin Burt1.

1 Department of Life Sciences, Imperial College, Silwood Park, Ascot, SL5 7PY, UK

For correspondence: katie.willis16@imperial.ac.uk

___
## Requirements

* Jupyter notebook
* Julia 1.5 or above
* All dependencies can be installed by running the following code in julia from the location of the downloaded files to initiate the environment (This only needs to be done once)
```
using Pkg
Pkg.activate("./Environment/")
Pkg.instantiate()
```

The environment can loaded at the beginning of each jupyter session by running:
```
] activate "./Environment/"
```

And the required packages can be loaded by running:
```
using NBInclude
@nbinclude("./Environment/Setup.ipynb");
```

___
## User notes

For clarity some parameter labels have been changed for publication. None of the differences result in changes to the results, but are noteworthy to aid interpretation of the code.

* Allele labels differ in the baseline and 4-allele models compared to publication. In the publication α and β refer to the construct and a and b refer to cleavage-resistant alleles, whereas in the code this is reversed.
* Locus labels differ in the 4-allele model compared to publication. In the publication the differentiated site (the locus with 4 alleles) is the insertion site for the β construct, whereas in the code this is the insertion site for the α construct.
* In the publication μ refers to the homing-associated loss-of-function probability, in the code this is referred to as d.
* In the publication gamma refers to the density-dependent parameter of the Beverton-Holt population dynamics model, in the code this is referred to as α, not to be confused with the allele label α which is not a user-defined parameter.
