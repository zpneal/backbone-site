### Getting started
The **backbone** package can extract the backbone from a network stored as an adjacency matrix in a _matrix_ or _sparse Matrix_ class object, or as an _igraph_ object in **R**. 

Given a network stored in `dat`, running `backbone(dat)` will:
* Detect the type of network stored in `dat`
* Choose an appropriate backbone extraction model
* Use reasonable defaults to extract the backbone
* Return the backbone in the same class as `dat`

For example, if `dat` is an adjacency matrix for a weighted network, then `backbone(dat)` returns the adjacency matrix for the network's backbone extracted using the _Disparity Filter_ with $\alpha$ = 0.05.

### Weighted networks
XXX

### Weighted projections
XXX

### Unweighted networks
XXX
