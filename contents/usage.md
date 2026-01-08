The **backbone** package can extract the backbone from a network stored as an adjacency matrix in a _matrix_ or _sparse Matrix_ class object, or as an _igraph_ object in **R**. 

Given a network stored in `dat`, running `backbone(dat)` will:
* Detect the type of network stored in `dat`
* Choose an appropriate backbone extraction model
* Use reasonable defaults to extract the backbone
* Return the backbone in the same class as `dat`
* Display a brief summary of what the function did

For example, if `dat` is an adjacency matrix for a weighted network, then `backbone(dat)` returns the adjacency matrix for the network's backbone extracted using the _Disparity Filter_ with $\alpha$ = 0.05.

The **backbone** package offers the following backbone models that can be specified using the `model` argument:
* For weighted networks
  * Global threshold
  * [Disparity filter](https://doi.org/10.1073/pnas.0808904106)
  * [Locally adaptive network sparsification](https://doi.org/10.1371/journal.pone.0016431)
  * [Marginal likelihood filter](https://doi.org/10.1103/PhysRevE.93.012304)
* For weighted bipartite projections
  * [Stochastic degree sequence](https://doi.org/10.1038/s41598-021-03238-3)
  * [Fixed degree sequence](https://doi.org/10.1007/s13278-011-0021-0)
  * [Fixed row](https://doi.org/10.1038/s41598-021-03238-3)
  * [Fixed column](https://doi.org/10.1038/s41598-021-03238-3)
  * [Fixed fill](https://doi.org/10.1038/s41598-021-03238-3)
* For unweighted networks
  * [Local sparsification](https://doi.org/10.1145/1989323.1989399)
  * [Global sparsification](https://doi.org/10.1145/1989323.1989399)
  * [Local degree](https://doi.org/10.1007/s13278-016-0332-2)
  * [Skeleton](https://doi.org/10.1145/195058.195422)
  * [Simmelian](https://doi.org/10.1145/2492517.2492569)
  * [Simmelian quadrilateral](https://doi.org/10.7155/jgaa.00370)
  * [Jaccard](https://doi.org/10.1073/pnas.0735871100)
  * [Meetmin](https://doi.org/10.1073/pnas.0735871100)
  * [Geometric](https://doi.org/10.1073/pnas.0735871100)
  * [Hypergeometric](https://doi.org/10.1073/pnas.0735871100)

