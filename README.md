# Hadamard-Matrices

This repo contains various programs implementing algorithms that deal with Hadamard matrices. A description of each program can be found below.

## Defect

The (dephased) defect of a Hadamard matrix $H$ is the dimension of the tangent space of (dephased) Hadamard matrices at $H$, and it can be a useful tool when studying families of Hadamard matrices. In particular, it gives an upper bound on the number of parameters that a family passing through $H$ can contain. This program implements two algorithms that can be used to find the defect of a given Hadamard matrix. The first method relies on using commutators to find the dimension of the commutator subspace, and the second method uses a formula coming from group theory (with the second method only working for the fourier matrix $F_n$; the formula can be found [here](https://web.math.utk.edu/~rnicoara/defect.pdf)). We include some examples of Hadamard matrices and their defects.

## Fingerprint

The fingerprint of a Hadamard matrix is an invariant for Hadamard matrices (if two Hadamard matrices are equivalent, then they have the same fingerprint). This program implements an algorithm to compute the fingerprint of a Hadamard matrix, as seen [here](https://arxiv.org/abs/1001.3062). We also include some examples of Hadamard matrices and their fingerprints.

## Sinkhorn

This program uses the algorithm outlined in section 3 of the paper [Block-Circulant Complex Hadamard Matrices](https://arxiv.org/abs/2204.11727) to find complex Hadamard matrices. Recall that a complex Hadamard matrix must satisfy two properties:
* All entries of the matrix have absolute value $1$
* The rows of the matrix are pairwise orthogonal

In a sense, the algorithm described in the paper alternates back and forth between these two properties in the hopes of converging to a Hadamard matrix. To go further, here we add extra steps to the algorithm in order to force the resulting Hadamard matrix to satisfy certain symmetries, such as forcing the matrix to be symmetric or forcing it to have certain specific entries.

## Visualize

Visualizing a Hadamard matrix can make it easier to see the underlying patterns of the matrix, as can be seen [here](https://www.flickr.com/photos/nasa-jpl/16680460890/in/photostream/). In this program we implement a function that can be used to visualize both real and complex Hadamard matrices; the function colors the entries of the matrix based off of their argument (or angle). We include some examples of Hadamard matrices being visualized. In these examples we include some methods of generating real Hadamard matrices, such as Sylvester's construction or Paley's construction, which can be found [here](https://trace.tennessee.edu/utk_chanhonoproj/2266/). Finally, at the end, we create some animations involving families of complex Hadamard matrices.