# SCHISM

## About

SCHISM is a computational tool designed to infer subclonal hierarchy and the tumor evolution from somatic mutations. The inference process involves computational assessment of two fundamental properties of tumor evolution: lineage precedence rule and lineage divergence rule. 

First, SCHISM combines information about somatic mutation cellularity (aka mutation cancer cell fraction) across all tumor sample(s) available from a patient in a hypothesis testing framework to identify the statistical support for the lineage relationship between each pair of mutations or mutation clusters. The results of the hypothesis test are represented as Cluster Order Precedence Violation (CPOV) matrix which informs the subsequent step in SCHISM and ensures compliance of candidate tree topologies with lineage precedence rule.

Next, an implementation of genetic algorithm (GA) based on a fitness function that incorporates considerations for both lineage precedence (CPOV) rule and lineage divergence rule explores the space of tree topologies and returns a prioritized list of candidate subclonal phylogenetic trees, most compatible with observed cellularity data. 

## Links
* [Installation](http://github.com/Niknafs/SCHISM/wiki/Installation)
* [Tutorial](http://github.com/Niknafs/SCHISM/wiki/Tutorial)
* [Usage Examples](http://github.com/Niknafs/SCHISM/wiki/Usage-Examples)

## Releases 

* SCHISM-1.0.0&nbsp;&nbsp;&nbsp;&nbsp;2015-03-10&nbsp;&nbsp;&nbsp;&nbsp;Initial release at the time of manuscript submission
* SCHISM-1.0.1&nbsp;&nbsp;&nbsp;&nbsp;2016-01-01&nbsp;&nbsp;&nbsp;&nbsp;Minor visualization update. Citation info updated.
* SCHISM-1.1.0&nbsp;&nbsp;&nbsp;&nbsp;2016-01-26&nbsp;&nbsp;&nbsp;&nbsp;Mutation clustering module added.
* SCHISM-1.1.1&nbsp;&nbsp;&nbsp;&nbsp;2016-02-19&nbsp;&nbsp;&nbsp;&nbsp;POV matrix visualization, Mutation/Cluster cellularity visualization added.
* SCHISM-1.1.2&nbsp;&nbsp;&nbsp;&nbsp;2016-05-11&nbsp;&nbsp;&nbsp;&nbsp;Better color handling in cluster cellularity plots, addition of docker file
* SCHISM-1.1.3&nbsp;&nbsp;&nbsp;&nbsp;2017-06-21&nbsp;&nbsp;&nbsp;&nbsp;Addition of cellularity estimation for mutations in aneuploid regions of the genome.
* SCHISM-1.1.4&nbsp;&nbsp;&nbsp;&nbsp;2025-02-25&nbsp;&nbsp;&nbsp;&nbsp;Adapted to Python 3.8.

## Citation

If you use SCHISM in your research, please cite:

* Niknafs N, Beleva-Guthrie V, Naiman DQ, and Karchin R. SubClonal Hierarchy Inference from Somatic Mutations: automatic reconstruction of cancer evolutionary trees from multi-region next generation sequencing <http://dx.plos.org/10.1371/journal.pcbi.1004416>


## Platform

Basic functionality of SCHISM scripts developed in python should be available across all platforms. 

The plotting functionality of SCHISM relies on matplotlib, igraph c core and python-igraph. Matplotlib should run across all platforms. igraph dependencies (c core, and python-igraph), however, have been tested on Fedora and Ubuntu linux distributions only. An installation <a href="https://gist.github.com/Niknafs/6b50d9df9d5396a2e92e">guide</a> for igraph dependencies is available on the project wiki page. 

## Support
Please contact the package developer Noushin Niknafs (niknafs at jhu dot edu) with suggestions, questions or bug reports.

