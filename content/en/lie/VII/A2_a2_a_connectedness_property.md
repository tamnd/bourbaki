---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VII
chapter_title: CARTAN SUBALGEBRAS AND REGULAR ELEMENTS
section: 2
section_title: A connectedness property
appendix: true
lang: en
source: lie-vii-ix
book_pages: 48-49, 67
pdf_pages: 0058-0059, 0076-0076
extraction: native
statements: 3
exercises: 2
content_sha256: e52c40721671251b25cbd21bd6c6376bf20e17aa16de77c1b806f74183e1c74a
---

## APPENDIX II A CONNECTEDNESS PROPERTY

#### Lemma 1 {#lie-vii-a2-lem-1 .statement tag=00XN}

Let X be a connected topological space and $\Omega$ a dense open subset of X. If, for any $x\in X$, there exists a neighbourhood V of $x$ such that $V\cap \Omega$ is connected, then $\Omega$ is connected.

Indeed, let $\Omega_0$ be a non-empty open and closed subset of $\Omega$. Let $x\in X$ and let V be a neighbourhood of $x$ such that $V\cap \Omega$ is connected. If $x\in \overline{\Omega}_0$,

$$
(V\cap \Omega )\cap \Omega_0= V\cap \Omega_0\not=\emptyset
$$

so $V\cap \Omega \subset \Omega_0$. Thus, since $\Omega$ is dense in $X,\overline{\Omega}_0$ is a neighbourhood of $x$. Consequently, $\Omega_0$ is non-empty, open and closed, and since X is connected, $\overline{\Omega}_0= X$. Since $\Omega_0$ is closed in $\Omega$, this implies that $\Omega_0=\Omega \cap \overline{\Omega}_0=\Omega$, which proves that $\Omega$ is connected.

#### Lemma 2 {#lie-vii-a2-lem-2 .statement tag=00XO}

Let U be an open ball in $\mathbf{C}^n$ and $f: U\rightarrow \mathbf{C}$ a holomorphic function, not identically zero. Let A be a subset of U such that $f= 0$ on A. Then U **--** A is dense in U and connected.

The density of U**--** A follows from Differentiable and Analytic Manifolds, Results, 3.2.5. Assume first that $n= 1$. If $a\in A$, the power series expansion of $f$ about $a($Differentiable and Analytic Manifolds, Results, 3.2.1) is not reduced to 0, and it follows that there exists a neighbourhood $V_a$ of $a$ in U such that $f$ does not vanish on $V_a$ **--** $\{a\}$. Thus, $a$ is isolated in A, which proves that A is a discrete subset of U, hence countable since U is countable at infinity. Let $x, y\in U$ **--** A. The union of the real affine lines joining $x$ (resp. $y$) to a point of A is meagre (General Topology, Chap. IX, §5, no. 2, Def. 2). Hence, there exists $z\in U$ **--** A such that neither of the segments $[x, z]$ and $[y, z]$ meets A. The points $x, y, z$ thus belong to the same connected component of U **--** A, which proves the lemma in the case $n= 1$. We turn to the general case. We can assume that A is the set of zeros of $f($General Topology, Chap. I, §11, no. 1, Prop. 1). Let $x, y\in U$**--** A and let L be an affine line containing $x$ and $y$. The restriction of $f$ to $L\cap U$ is not identically zero since $x\in L\cap U$. By what has already been proved, $x$ and $y$ belong to the same connected component of $(L\cap U)$ **--** $(L\cap A)$ and hence to the same connected component of U **--** A.

#### Lemma 3 {#lie-vii-a2-lem-3 .statement tag=00XP}

Let X be a finite dimensional connected complex-analytic manifold and let A be a subset of X satisfying the following condition:

For any $x\in X$, there exists an analytic function germ $f_x$, not vanishing

at $x$, such that the germ of A at $x$ is contained in the germ at $x$ of the set

of zeros of $f_x$.

Then X **--** A is dense in X and connected.

The density of X**--** A follows from Differentiable and Analytic Manifolds, Results, 3.2.5. We can assume that A is closed (General Topology, Chap. I, §11, no. 1, Prop. 1). For any $x\in X$, there exists an open neighbourhood V of $x$ and an isomorphism $c$ from V to an open ball in $\mathbf{C}^n$ such that $c(A\cap V)$ is contained in the set of zeros of a holomorphic function not identically zero on $c(V)$. Then, by Lemma $2, V\cap (X$ **--** A) is connected. In view of Lemma 1, this proves that X **--** A is connected.

### Exercises {#lie-vii-a2-exercises}

See the [exercises for Appendix 2](exercises/a2/).
