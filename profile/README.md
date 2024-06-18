# Description
The organization Variational Sublinear Clustering aims at bundling different projects on efficient clustering in order to (A) disseminate
the algorithms for interested researchers and practitioners, and (B) to encourage further developments and to support future projects.

The organization currently contains two repositories vc-GMM and var-GMMs. Further repositories are currently developed within ongoing research projects. If repositories become mature enough they are made publicly available.

The available source code allows the application of k-means-like and GMM-like clustering algorithms at large and very large scales.
If N is the number of data point, C the number of clusters, and D the dimensionality of data points, then standard optimization algorithms
scale roughly with the product NCD. Therefore, applications of k-means or GMMs at large scales quickly become prohibitive.
The basic novelty the here developed algorithms is a sublinear scaling with the product NC. This means that, e.g., doubling the number of clusters does not double computational complexity. The novel k-means and GMM versions can consequently be applied at scales or with speeds at which previous algorithms could not be applied. For standard benchmarks we measured up to an order of magnitude faster execution times. References to scientific publications are provided below. A detailed technical description with a list of algorithms is available here:

https://uol.de/en/machine-learning/research/variational-em-for-big-fast-clustering

## Announcement of Future Updates

We are currently undertaking both technical and scientific improvements for the optimization of mixture models at very large scales. On the software side, the updates in development include the following:

- **Performance:** Overall improvements, including enhanced shared memory parallelization.
- **Simplified Installation Process:** To get up and running quickly with an easier installation procedure.
- **User-Friendly Interface:** An intuitive and streamlined Python interface for easier applicability.
- **Enhanced Documentation:** A more comprehensive documentation to further support the use of our algorithms.

Future results will be communicated through scientific papers, and the associated algorithms will be released upon publication.
If you are interested in large-scale mixture models and clustering and wish to try out our algorithms prior to their release, please contact us via E-Mail: [till.kahlke@uol.de](mailto:till.kahlke@uol.de).

## Repository vc-GMM

The repository contains efficient C++ source code for a combination of variational and coreset approaches to train
Gaussian Mixture Models (GMMs). The algorithm scales sublinearly with the product NC and is suitable for data with
large numbers of data points N, large numbers of clusters C and potentially large data dimensionality D. Improvements
and documentation of the source code are ongoing.

A detailed description and extensive benchmarking results of the algorithms can be found in this paper:

"A Variational EM Acceleration for Efficient Clustering at Very Large Scales", Florian Hirschberger*, Dennis Forster*, Jörg Lücke.  
<em>IEEE Transactions on Pattern Analysis and Machine Intelligence</em>, vol. 44, no. 12, pp. 9787-9801, 2022.  
*joint first authors. DOI:10.1109/TPAMI.2021.3133763, https://ieeexplore.ieee.org/document/9645327

For further descriptions of the source code itself, please see the README file of the vc-GMM repository.

## Repository var-GMM

The repository contains the first versions of variationally accelerated clustering algorithms. It contains corresponding
python code. The code is not optimized for execution speed. For optimized code we kindly refer to the repository vc-GMM.

A detailed description of the algorithms implemented in var-GMM can be found in the paper Hirschberger, Forster, Lücke, TPAMI 2022 (see above) with preliminary results reported in the paper:

"Can clustering scale sublinearly with its clusters? A variational EM acceleration of GMMs and k-means.", Dennis Forster, Jörg Lücke.  
<em>International Conference on Artificial Intelligence and Statistics (AISTATS), 84:124-132.
http://proceedings.mlr.press/v84/forster18a.html

 
 



