# Description
The organization Variational Sublinear Clustering aims at bundling different projects on efficient clustering in order to (A) disseminate
the algorithms for interested researchers and practitioners, and (B) to encourage further developments and to support future projects.

The organization is started with the repository vc-GMM and is currently extended by adding further repositories. Further source
code and descriptions are provided on this website:

https://uol.de/en/machine-learning/research/variational-em-for-big-fast-clustering

But we plan to migrate the website to this github organization.



# Repository vc-GMM

The repository contains efficient C++ source code for a combination of variational and coreset approaches to train
Gaussian Mixture Models (GMMs). The algorithm scales sublinearly with the product NC and is suitable for data with
large numbers of data points N, large number of clusters C and potentially large data dimensionality D. Improvements
and documentation of the source code are ongoing.

A detailed description and extensive benchmarking results of the algorithms can be found in this paper:

"A Variational EM Acceleration for Efficient Clustering at Very Large Scales", 
Florian Hirschberger, Dennis Forster, Jörg Lücke.
IEEE Transactions on Pattern Analysis and Machine Intelligence, accepted, 2021.
https://ieeexplore.ieee.org/document/9645327
DOI:10.1109/TPAMI.2021.3133763

For further descriptions of the source code itself, please see the README file of the vc-GMM repository.







