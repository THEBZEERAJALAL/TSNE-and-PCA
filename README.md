# PCA
Widely used method for unsupervised, linear dimensionality reduction.


GOAL: account for variance of data in as few dimensions as possible (using linear projection)
Find a line, such that when the data is projected onto that line, it has the maximum variance
Find a second line, orthogonal to the first, that has maximum projected variance
Repeat until have k orthogonal lines


The projected position of a point on these lines gives the coordinates in the k-dimensional reduced space

## steps in pca
1.Mean center the data


2.Compute covariance matrix sigma


3.Calculate eigenvalues and eigenvectors of sigma

4.Eigenvector with largest eigenvalue lamda1 is 1st principal component (PC)

5.Eigenvector with kth largest eigenvalue lamda k is kth PC

6.lamda k / sigma i lamda i = proportion of variance captured by kth PC

7.Full set of PCs comprise a new orthogonal basis for feature space, whose axes are aligned with the maximum variances of   original data.

8.Projection of original data onto first k PCs gives a reduced dimensionality representation of the data.

#T-SNE

Visualizes high-dimensional data in a 2- or 3-dimensional map.
Better than existing techniques at creating a single map that reveals structure at many different scales.
Particularly good for high-dimensional data that lie on several different, but related, low-dimensional manifolds.
Example: images of objects from multiple classes seen from multiple viewpoints.

 
