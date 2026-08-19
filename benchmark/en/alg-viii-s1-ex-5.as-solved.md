For a left ideal $L$ of $\mathbf M_n(A)$, let $N_i$ be the set of row vectors occurring as the $i$-th row of matrices belonging to $L$. Since multiplication on the left by the matrix units $e_{ji}$ carries the $i$-th row onto the $j$-th row and annihilates all the other rows, we have $N_i=N_j$ for all $i,j$. Moreover, each $N_i$ is a left $A$-submodule of the left $A$-module $A^n$. Thus, writing $N=N_1$, we have
$$
L=\{(x_{ij})\in\mathbf M_n(A)\mid\text{each row }(x_{i1},\ldots,x_{in})\text{ belongs to }N\}.
$$
Conversely, this set is a left ideal of $\mathbf M_n(A)$ for every left $A$-submodule $N$ of $A^n$. Consequently, the correspondence
$$
N\longmapsto L_N
$$
is an inclusion-preserving bijection from the set of left $A$-submodules of $A^n$ onto the set of left ideals of $\mathbf M_n(A)$.

It follows from Definition 2 that $\mathbf M_n(A)$ is left Artinian (resp. left Noetherian) if and only if the left $A$-module $A^n$ is Artinian (resp. Noetherian). If $A$ is left Artinian (resp. left Noetherian), then $A^n$ has the same property by Example 5 of §1. Conversely, if $A^n$ is Artinian (resp. Noetherian), its direct summand $A$ is Artinian (resp. Noetherian), by Proposition 3 of §1 applied to
$$
A^n=A\oplus A^{n-1}.
$$
Thus $A$ is left Artinian (resp. left Noetherian) if and only if $\mathbf M_n(A)$ is.

Finally suppose that $A$ is left Artinian. By Theorem 1 of §1, $A$ has finite length. The inclusion-preserving bijection above identifies the lattices of submodules of the left $A$-module $A^n$ and of left ideals of $\mathbf M_n(A)$; hence the two modules have the same length. By additivity of length for finite direct sums,
$$
\operatorname{length}_{A}(A^n)
=n\,\operatorname{length}_{A}(A).
$$
Since the left length of a ring is the length of its left regular module, this gives
$$
\operatorname{length}_{\mathbf M_n(A)}\mathbf M_n(A)
=n\,\operatorname{length}_{A}A.
$$
