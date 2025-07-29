# Hadamard-Matrices

This repo contains various programs implementing algorithms that deal with Hadamard matrices. A description of each program can be found below.

## Defect

The (dephased) defect of a Hadamard matrix $H$ is the dimension of the tangent space of (dephased) Hadamard matrices at $H$, and it can be a useful tool when studying families of Hadamard matrices. In particular, it gives an upper bound on the number of parameters that a family passing through $H$ can contain. This program implements two algorithms that can be used to find the defect of a given Hadamard matrix. The first method relies on using commutators to find the dimension of the commutator subspace, and the second method uses a formula coming from group theory (with the second method only working for the fourier matrix $F_n$). We include some examples of Hadamard matrices and their defects.

## Fingerprint

The fingerprint of a Hadamard matrix is an invariant for Hadamard matrices (if two Hadamard matrices are equivalent, then they have the same fingerprint). This program implements an algorithm to compute the fingerprint of a Hadamard matrix, as seen [here](https://arxiv.org/abs/1001.3062). We also include some examples of Hadamard matrices and their fingerprints.