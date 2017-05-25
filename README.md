# PCA
Widely used method for unsupervised, linear dimensionality reduction.


GOAL: account for variance of data in as few dimensions as possible (using linear projection)
Find a line, such that when the data is projected onto that line, it has the maximum variance
Find a second line, orthogonal to the first, that has maximum projected variance
Repeat until have k orthogonal lines


The projected position of a point on these lines gives the coordinates in the k-dimensional reduced space

## Steps in pca
1.Mean center the data


2.Compute covariance matrix sigma


3.Calculate eigenvalues and eigenvectors of sigma

4.Eigenvector with largest eigenvalue lamda1 is 1st principal component (PC)

5.Eigenvector with kth largest eigenvalue lamda k is kth PC

6.lamda k / sigma i lamda i = proportion of variance captured by kth PC

7.Full set of PCs comprise a new orthogonal basis for feature space, whose axes are aligned with the maximum variances of   original data.

8.Projection of original data onto first k PCs gives a reduced dimensionality representation of the data.

# T-SNE

Visualizes high-dimensional data in a 2- or 3-dimensional map.
Better than existing techniques at creating a single map that reveals structure at many different scales.
Particularly good for high-dimensional data that lie on several different, but related, low-dimensional manifolds.

## Steps in T-sne

The t-SNE algorithm comprises two main stages.

1. t-SNE constructs a probability distribution over pairs of high-dimensional objects in such a way that similar objects have a high probability of being picked, whilst dissimilar points have an extremely small probability of being picked. 
2. t-SNE defines a similar probability distribution over the points in the low-dimensional map, and it minimizes the Kullback–Leibler divergence between the two distributions with respect to the locations of the points in the map. Note that whilst the original algorithm uses the Euclidean distance between objects as the base of its similarity metric, this should be changed as appropriate.


 
