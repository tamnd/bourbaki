---
book: alg
book_title: Algebra
chapter: III
chapter_title: TENSOR ALGEBRAS, EXTERIOR ALGEBRAS, SYMMETRIC ALGEBRAS
section: 8
section_title: Determinants
lang: en
source: alg-i-iii
source_edition: 1998, Springer
pdf_pages: 0546-0565, 0661-0668
extraction: ocr
subsections:
    - "no": 1
      title: DETERMINANTS OF AN ENDOMORPHISM
      page: 0
      pdf_page: 546
    - "no": 2
      title: CHARACTERIZATION OF AUTOMORPHISMS OF A FINITE-DIMENSIONAL FREE MODULE
      page: 0
      pdf_page: 547
    - "no": 3
      title: DETERMINANT OF A SQUARE MATRIX
      page: 0
      pdf_page: 548
    - "no": 4
      title: CALCULATION OF A DETERMINANT
      page: 0
      pdf_page: 550
    - "no": 5
      title: MINORS OF A MATRIX
      page: 0
      pdf_page: 552
    - "no": 6
      title: EXPANSIONS OF A DETERMINANT
      page: 0
      pdf_page: 554
    - "no": 7
      title: APPLICATION TO LINEAR EQUATIONS
      page: 0
      pdf_page: 558
    - "no": 8
      title: CASE OF A COMMUTATIVE FIELD
      page: 0
      pdf_page: 560
    - "no": 9
      title: THE UNIMODULAR GROUP $\mathbf{SL}(n, A)$
      page: 0
      pdf_page: 561
    - "no": 10
      title: THE $\mathbf{A}[X]$-MODULE ASSOCIATED WITH AN $\mathbf{A}$-MODULE ENDOMORPHISM
      page: 0
      pdf_page: 562
    - "no": 11
      title: CHARACTERISTIC POLYNOMIAL OF AN ENDOMORPHISM
      page: 0
      pdf_page: 564
statements: 36
exercises: 26
content_sha256: 960444600d0318311b60e4017068e8754d6a4a4672665f9e3dd261fa82222e35
---

## § 8. DETERMINANTS

### 1. DETERMINANTS OF AN ENDOMORPHISM

Let $M$ be an $A$-module with a finite basis of $n$ elements and $u$ an endomorphism of $M$. The $A$-module $\bigwedge^n(M)$ is a monogenous free module, that is isomorphic to $A$ (no. 8, Corollary 1 to Theorem 1); $\bigwedge^n(u)$ is an endomorphism of this module and is therefore a homothety $z \mapsto \lambda z$ of ratio $\lambda \in A$ determined uniquely (II, § 2, no. 3, Proposition 5).

#### Definition 1 {#alg-iii-s8-def-1 .statement}

*The determinant of an endomorphism $u$ of a free $A$-module $M$ of finite dimension $n$* (II, § 7, no. 2, Corollary to Proposition 3 and Remark 1), *denoted by* $\det u$, *is the scalar $\lambda$ such that* $\bigwedge^n(u)$ *is the homothety of ratio* $\lambda$.

By formula (4) of § 7, no. 2, $\det u$ is the unique scalar such that

(1)
$$
u(x_1) \wedge u(x_2) \wedge \cdots \wedge u(x_n) = (\det u) \cdot x_1 \wedge x_2 \wedge \cdots \wedge x_n
$$
for every sequence $(x_i)_{1 \leq i \leq n}$ of $n$ elements of $M$. If $\det(u) = 1$, $u$ is said to be *unimodular*.

#### Proposition 1 {#alg-iii-s8-prop-1 .statement}

(i) *If $u$ and $v$ are two endomorphisms of a finite-dimensional free $A$-module $M$, then*

(2)
$$
\det(u \circ v) = (\det u)(\det v).
$$

(ii) $\det(1_M) = 1$; *for every automorphism* $u$ *of* $M$, $\det u$ *is invertible in* $A$ *and*

(3)
$$
\det(u^{-1}) = (\det u)^{-1}.
$$

If $n$ is the dimension of $M$, this follows immediately from the relation $\bigwedge^n(u \circ v) = (\bigwedge^n(u)) \circ (\bigwedge^n(v))$ § 7, no. 2, formula (3)).

Let $M$ be a free $A$-module with a finite basis $(e_i)_{1 \leq i \leq n}$; given a sequence $(x_i)_{1 \leq i \leq n}$ of $n$ elements of $M$, the determinant of this sequence *with respect to* the given basis $(e_i)$, denoted by $\det(x_1, x_2, \ldots, x_n)$ when no confusion can arise over the basis, is the determinant of the endomorphism $u$ of $M$ such that $u(e_i) = x_i$ for $1 \leq i \leq n$. Then by formula (1)

$$
x_1 \wedge x_2 \wedge \cdots \wedge x_n = \det(x_1, x_2, \ldots, x_n) \ e_1 \wedge e_2 \wedge \cdots \wedge e_n
$$

and this relation characterizes the mapping $(x_i) \mapsto \det(x_1, x_2, \ldots, x_n)$ of $M^n$ into $A$. It shows that this mapping is an *alternating n-linear form*. As, by virtue of § 7, no. 4, Proposition 7, the $A$-module of alternating $n$-linear forms is canonically isomorphic to the dual of $\bigwedge^n(M)$ and $\bigwedge^n(M)$ is isomorphic to $A$, it is seen that *every alternating n-linear form on $M^n$ can be written*

$$(x_1, \ldots, x_n) \mapsto \alpha \det(x_1, x_2, \ldots, x_n)$$

for some $\alpha \in A$.

#### Proposition 2 {#alg-iii-s8-prop-2 .statement}

*Let $M$ be a free $A$-module with a finite basis $(e_i)_{1 \leq i \leq n}$ and $v$ an endomorphism of $M$. For every sequence $(x_i)_{1 \leq i \leq n}$ of $n$ elements of $M$,*

$$
\det(v(x_1), \ldots, v(x_n)) = (\det v) \det(x_1, \ldots, x_n).
$$

If $u$ is the endomorphism of $M$ such that $u(e_i) = x_i$ for all $i$, then

$$
v(x_i) = (v \circ u)(e_i)
$$

and (5) therefore follows from (2).

### 2. CHARACTERIZATION OF AUTOMORPHISMS OF A FINITE-DIMENSIONAL FREE MODULE

#### Theorem 1 {#alg-iii-s8-thm-1 .statement}

*Let $M$ be a finite-dimensional free $A$-module and $u$ an endomorphism of $M$. The following conditions are equivalent:*
(a) $u$ is bijective;
(b) $u$ is right invertible (II, § 1, no. 9, Corollary 1 to Proposition 15);
(c) $u$ is left invertible (II, § 1, no. 9, Corollary 2 to Proposition 15);
(d) $u$ is surjective;
(e) $\det u$ is invertible in $A$.

Let $(e_i)_{1 \leq i \leq n}$ be a basis of $M$. If $x_i = u(e_i)$ for $1 \leq i \leq n$, then

$$
x_1 \wedge x_2 \wedge \cdots \wedge x_n = (\det u) e_1 \wedge e_2 \wedge \cdots \wedge e_n.
$$

By § 7, no. 9, Theorem 2 a necessary and sufficient condition for the $x_i$ to form a basis of $M$ is that $\det u$ be an invertible element of $A$; this proves the equivalence of (a) and (e). Observe that (a) obviously implies each of conditions (b), (c) and (d); it remains to prove that each of conditions (b), (c) and (d) implies (e). Now, if there exists an endomorphism $v$ of $M$ such that $v \circ u = 1_M$ or $u \circ v = 1_M$, then $(\det v)(\det u) = 1$ and hence $\det u$ is invertible in $A$. If $u$ is surjective, so is $\bigwedge^n(u)$ (§ 7, no. 2, Proposition 3), in other words the homothety of ratio det $u$ in $A$ is surjective, which immediately implies that det $u$ is invertible.

#### Proposition 3 {#alg-iii-s8-prop-3 .statement}

*Let $M$ be a finite-dimensional free $A$-module. For every endomorphism $u$ of $M$, the following conditions are equivalent:*
  (f) $u$ is injective;
  (g) det $u$ is not a divisor of zero in $A$.

With the same notation as in the proof of Theorem 1, for $u$ to be injective, it is necessary and sufficient that the $x_i$ be linearly independent. By § 7, no. 9, Proposition 12, it is necessary and sufficient for this that the relation $\lambda x_1 \wedge x_2 \wedge \cdots \wedge x_n = 0$ (with $\lambda \in A$) imply $\lambda = 0$. But this is equivalent to $\lambda (\det u) = 0$ since $e_1 \wedge \cdots \wedge e_n$ is a basis of $\Lambda^n(M)$; whence the proposition.

#### Remark {#alg-iii-s8-n2-rem-1 .statement}

When $A$ is a field, condition (e) of Theorem 2 is equivalent to condition (g) of Proposition 3, since they both mean that $\det u \neq 0$. In this case therefore all the conditions of Theorem 1 and Proposition 3 are equivalent (cf. II, § 7, no. 4, Corollary to Proposition 9).

### 3. DETERMINANT OF A SQUARE MATRIX

#### Definition 2 {#alg-iii-s8-def-2 .statement}

*Let $I$ be a finite set, $A$ a commutative ring and $X$ a square matrix of type $(I, I)$ over the ring $A$ (II, § 10, no. 7). The determinant of the endomorphism $u$ of the $A$-module $A^I$, whose matrix with respect to the canonical basis of $A^I$ is $X$, is called the determinant of $X$ and denoted by $\det X$.*

If $X = (\xi_{ij})_{(i,j) \in I \times I}$ and $(e_i)_{i \in I}$ is the canonical basis of $A^I$, the endomorphism $u$ is then given by
$$
u(e_i) = \sum_{j \in J} \xi_{ji} e_j.
$$

When $I = \{1, n\} \subset \mathbf{N}$, if we write $x_i = u(e_i)$ for $i \in I$, the determinant of $X$ is then defined in the relation
$$
x_1 \wedge x_2 \wedge \cdots \wedge x_n = (\det X) e_1 \wedge e_2 \wedge \cdots \wedge e_n
$$
in other words, $\det X$ is equal to the determinant $\det(x_1, x_2, \ldots, x_n)$ with respect to the canonical basis of $A^n$. Consequently:

#### Proposition 4 {#alg-iii-s8-prop-4 .statement}

*For $n$ vectors $x_1, \ldots, x_n$ of $A^n$, let $X(x_1, \ldots, x_n)$ denote the square matrix of order $n$ whose $i$-th column is $x_i$ for $1 \leq i \leq n$. Then the mapping*
$$
(x_1, \ldots, x_n) \mapsto \det(X(x_1, \ldots, x_n))
$$
*of $(A^n)^n$ into $A$ is alternating and $n$-linear.*

In particular, the determinant of a matrix two of whose columns are equal is zero. If a permutation is performed on the columns of a matrix, the determinant of the new matrix is equal to that of the old multiplied by $\varepsilon_{\sigma}$. If to one column of a matrix is added a scalar multiple of a column of a different index, the determinant of the new matrix is equal to that of the old.

More generally, let $M$ be a free $A$-module of finite dimension $n$ and let $(e_i)_{i \in I}$ be a basis of $M$; for every automorphism $u$ of $M$, if $X$ is the matrix of $u$ with respect to the basis $(e_i)$, then

$$
\det(u) = \det(X)
$$

as follows immediately from the definitions.

When $I = \{1, n\}$, the determinant of $X$ is also denoted by

$$
\det(\xi_{ij})_{1 \leq i \leq n, 1 \leq j \leq n}
$$

or simply $\det(\xi_{ij})$ if this causes no confusion, or also

$$
\begin{vmatrix}
\xi_{11} & \xi_{12} & \ldots & \xi_{1n} \\
\xi_{21} & \xi_{22} & \ldots & \xi_{2n} \\
\ldots & \ldots & \ldots & \ldots \\
\xi_{n1} & \xi_{n2} & \ldots & \xi_{nn}
\end{vmatrix}
$$

When $X = 1$, the matrix $X$ is called unimodular.

#### Example {#alg-iii-s8-n3-exa-1 .statement}

(1) The determinant of the empty matrix is equal to 1; the determinant of a square matrix of order 1 is equal to the unique element of this matrix. For a matrix of order 2

$$
\begin{pmatrix}
\xi_{11} & \xi_{12} \\
\xi_{21} & \xi_{22}
\end{pmatrix}
$$

then, in the above notation,

$$
x_1 \wedge x_2 = (\xi_{11} e_1 + \xi_{21} e_2) \wedge (\xi_{12} e_1 + \xi_{22} e_2) = \xi_{11} \xi_{22} e_1' \wedge e_2 + \xi_{21} \xi_{12} e_2 \wedge e_1
$$

whence

$$
\begin{vmatrix}
\xi_{11} & \xi_{12} \\
\xi_{21} & \xi_{22}
\end{vmatrix} = \xi_{11} \xi_{22} - \xi_{12} \xi_{21}.
$$

We translate into the language of matrices some of the results of nos. 1 and 2:

#### Proposition 5 {#alg-iii-s8-prop-5 .statement}

*If $X$ and $Y$ are two square matrices over a commutative ring $A$ with the same finite indexing set, then*

$$
\det(XY) = (\det X)(\det Y).
$$

For X to be invertible, it is necessary and sufficient that det X be an invertible element of A, and then

(9) $$
\det(X^{-1}) = (\det X)^{-1}.
$$

This follows immediately from no. 1, Proposition 1 and no. 2, Theorem 1.

#### Corollary {#alg-iii-s8-n3-cor-1 .statement}

*Two similar square matrices have equal determinants.*

If P is an invertible square matrix, then $\det(PXP^{-1}) = \det X$ by (8) and (9).

#### Proposition 6 {#alg-iii-s8-prop-6 .statement}

*For the columns of a square matrix X of finite order to be linearly independent, it is necessary and sufficient that det X be not a divisor of zero in A.*

This follows from no. 2, Proposition 3.

### 4. CALCULATION OF A DETERMINANT

#### Lemma 1 {#alg-iii-s8-lem-1 .statement}

*Let A be a commutative ring and M a free A-module with a basis $(e_j)_{j \in J}$, where the indexing set J is totally ordered. For every integer $p \leq \mathrm{Card}(J)$, every alternating p-linear function $f : M^p \to N$ (where N is an A-module) and every family of p elements $x_i = \sum_{j \in J} \xi_{ji} e_j$ of M $(1 \leq i \leq p)$,

$$
f(x_1, x_2, \ldots, x_p)
= \sum_{j_1 < j_2 < \cdots < j_p} \left( \sum_{\sigma \in S_p} \varepsilon_\sigma \cdot \xi_{j_{\sigma(1)}, 1} \xi_{j_{\sigma(2)}, 2} \cdots \xi_{j_{\sigma(p)}, p} \right) f(e_{j_1}, \ldots, e_{j_p})
$$

*where* $(j_k)_{1 \leq k \leq p}$ *runs through the set of strictly increasing sequences of p elements of J.*

Now

$$
f(x_1, \ldots, x_p) = \sum_{(j_k)} \xi_{j_1, 1} \xi_{j_2, 2} \cdots \xi_{j_p, p} f(e_{j_1}, e_{j_2}, \ldots, e_{j_p})
$$

where $(j_k)_{1 \leq k \leq p}$ runs through *all* the sequences of p elements of J; it then suffices to apply Corollary 1 to Proposition 7 of § 7, no. 4 to f.

In particular, if J is finite and has n elements and $x_i = \sum_{j \in J} \xi_{ji} e_j$ $(1 \leq i \leq n)$ are n elements of M, then

(11) $$
x_1 \wedge x_2 \wedge \cdots \wedge x_n
= \left( \sum_{\sigma \in S_n} \varepsilon_\sigma \xi_{j_{\sigma(1)}, 1} \xi_{j_{\sigma(2)}, 2} \cdots \xi_{j_{\sigma(n)}, n} \right) e_{j_1} \wedge e_{j_2} \wedge \cdots \wedge e_{j_n}
$$

where $(j_k)_{1 \leq k \leq n}$ is the unique sequence of the n elements of J arranged in increasing order, whence

(12) $$
\det(x_1, x_2, \ldots, x_n) = \sum_{\sigma \in S} \varepsilon_\sigma \cdot \xi_{j_{\sigma(1)}, 1} \xi_{j_{\sigma(2)}, 2} \cdots \xi_{j_{\sigma(n)}, n}.
$$

With the notation of Lemma 1, comparing formulae (10) and (12) gives

$$
x_1 \wedge x_2 \wedge \cdots \wedge x_p = \sum_{H \in \mathcal{F}_p(J)} \det(x_{H,1}, x_{H,2}, \ldots, x_{H,p}) e_H
$$

where $\mathcal{F}_p(J)$ is the set of subsets of $J$ with $p$ elements and, for every subset $H \in \mathcal{F}_p(J)$, we write $x_{H,i} = \sum_{j \in H} \xi_{ji} e_j$ and $e_H = e_{j_1} \wedge e_{j_2} \wedge \cdots \wedge e_{j_p}$, $(j_k)_{1 \leq k \leq p}$ being the sequence of elements of $H$ arranged in increasing order, it being understood that $\det(x_{H,1}, \ldots, x_{H,p})$ is taken with respect to the basis $(e_{jk})_{1 \leq k \leq p}$.

#### Proposition 7 {#alg-iii-s8-prop-7 .statement}

*Let $I$ be a finite set and $X = (\xi_{ji})_{(j, i) \in I \times I}$ a square matrix of type (I, I) over a commutative ring $A$. Then*

$$
\det X = \sum_{\sigma \in S_I} \varepsilon_\sigma \left( \prod_{i \in I} \xi_{\sigma(i), i} \right)
$$

*where $\sigma$ runs through the group $S_I$ of permutations of $I$ and $\varepsilon_\sigma$ is the signature of $\sigma$* (I, § 5, no. 7).

Attention may be confined to the case where $I = \{1, n\} \subset \mathbf{N}$ and it then suffices to apply formula (12), where $(e_i)_{1 \leq i \leq n}$ is the canonical basis of $A^n$ and the $x_i$ are the columns of $X$ (cf. no. 3, formula (6)).

In particular, for the determinant of a matrix of order 3

$$
X = \begin{pmatrix}
\xi_{11} & \xi_{12} & \xi_{13} \\
\xi_{21} & \xi_{22} & \xi_{23} \\
\xi_{31} & \xi_{32} & \xi_{33}
\end{pmatrix}
$$

we have

$$
\det(X) = \xi_{11} \xi_{22} \xi_{33} + \xi_{12} \xi_{23} \xi_{31} + \xi_{21} \xi_{32} \xi_{13} - \xi_{13} \xi_{22} \xi_{31} - \xi_{12} \xi_{21} \xi_{33} - \xi_{11} \xi_{23} \xi_{32}.
$$

#### Proposition 8 {#alg-iii-s8-prop-8 .statement}

*For every square matrix $X$ over a commutative ring, the determinant of the transpose matrix ${}^t X$ is equal to the determinant of $X$.*

Suppose that $X$ is of type (I, I). For every ordered pair of permutations $\sigma, \tau$ of $S_I$, (since multiplication is commutative)

$$
\prod_{i \in I} \xi_{\sigma(i), i} = \prod_{j \in I} \xi_{\sigma(\tau(j)), \tau(j)}.
$$

In particular take $\tau = \sigma^{-1}$; using the fact that $\varepsilon_{\sigma^{-1}} = \varepsilon_\sigma$, it is seen that

$$
\det X = \sum_{\sigma \in S_I} \varepsilon_\sigma \left( \prod_{i \in I, i} \xi_{i, \sigma(i)} \right),
$$

which proves the proposition.

#### Corollary 1 {#alg-iii-s8-prop-8-cor-1 .statement}

For n vectors $x_1, \ldots, x_n$ of $\mathbf{A}^n$, let $Y(x_1, \ldots, x_n)$ denote the square matrix of order n whose i-th row is $x_i$, for $1 \leq i \leq n$. Then the mapping
$$
(x_1, \ldots, x_n) \mapsto \det(Y(x_1, \ldots, x_n))
$$
from $(\mathbf{A}^n)^n$ to $\mathbf{A}$ is alternating and n-linear.

#### Corollary 2 {#alg-iii-s8-prop-8-cor-2 .statement}

For a square matrix $X$ of finite order over a commutative ring $\mathbf{A}$ the following conditions are equivalent:
(i) the rows of $X$ are linearly independent;
(ii) the columns of $X$ are linearly independent;
(iii) $\det X$ is not a divisor of zero in $\mathbf{A}$.

This follows immediately from no. 3, Proposition 6 and Proposition 8 above.

#### Corollary 3 {#alg-iii-s8-prop-8-cor-3 .statement}

Let $u$ be an endomorphism of a finite-dimensional free $\mathbf{A}$-module $M$ and $^t u$ the transpose endomorphism of the dual $M^*$ (II, § 2, no. 5, Definition 5); then
$$
\det(^t u) = \det(u).
$$
If $X$ is the matrix of $u$ with respect to a basis of $M$, $^t X$ is the matrix of $^t u$ with respect to the dual basis (II, § 10, no. 4, Proposition 3); as $\det(u) = \det(X)$ and $\det(^t u) = \det(^t X)$, the conclusion follows from Proposition 8.

### 5. MINORS OF A MATRIX

Let $X$ be a rectangular matrix $(\xi_{ij})_{(i,j) \in I \times J}$ of type (I, J) whose indexing sets I and J are totally ordered. If $H \subset I$ and $K \subset J$ are finite subsets with the same number $p$ of elements, there exists a unique increasing bijection $\phi : H \to K$ (Set Theory, III, § 5, no. 3, Proposition 6); we shall denote by $X_{H,K}$ the square matrix of type (H, H) equal to $(\xi_{i,\phi(j)})_{(i,j) \in H \times H}$. If the elements of $X$ belong to a commutative ring $\mathbf{A}$, the determinant $\det(X_{H,K})$ is called the minor of the matrix $X$ of indices H, K; these determinants (for all ordered pairs (H, K) of subsets of I and J respectively with $p$ elements) are also called the minors of $X$ of order $p$. With this notation:

#### Proposition 9 {#alg-iii-s8-prop-9 .statement}

Let $M$ be an $\mathbf{A}$-module with a basis $(e_i)_{i \in J}$ (finite or otherwise) whose indexing set $J$ is totally ordered. For every integer $p > 0$, let $(e_H)_{H \in \mathfrak{S}_p(J)}$ be the corresponding basis of $\wedge^p(M)$ (§ 7, no. 8). Let $(x_i)_{1 \leq i \leq p}$ be a sequence of $p$ elements of $M$; let
$$
x_i = \sum_{j \in J} \xi_{ji} e_j \quad \text{for } i \in I = \{1, p\}
$$

and let $X$ denote the matrix $(\xi_{ji})$ of type $(J, I)$. Then

$$
x_1 \wedge x_2 \wedge \cdots \wedge x_p = \sum_{H \in \mathfrak{F}_p(J)} (\det X_{H,I}) e_H.
$$

where $H$ runs through the set $\mathfrak{F}_p(J)$ of subsets of $J$ with $p$ elements.

This follows immediately from formula (12) of no. 4 and formula (6) of no. 3.

#### Proposition 10 {#alg-iii-s8-prop-10 .statement}

Let $M$ and $N$ be two free $A$-modules of respective dimensions $m$ and $n$, $u : M \to N$ a linear mapping and $X$ the matrix of $u$ with respect to a basis $(e_i)_{1 \leq i \leq m}$ of $M$ and a basis $(f_j)_{1 \leq j \leq n}$ of $N$. Then, for every integer $p \leq \inf(m, n)$, the matrix of $\wedge^p(u)$ with respect to the basis $(e_K)_{K \in \mathfrak{F}_p(I)}$ of $\wedge^p(M)$ and the basis $(f_H)_{H \in \mathfrak{F}_p(J)}$ of $\wedge^p(N)$ (where we have written $I = \{1, m\}$ and $J = \{1, n\}$) is the matrix $(\det(X_{H,K}))$ of type $(\mathfrak{F}_p(J), \mathfrak{F}_p(I))$ (and hence with $\binom{n}{p}$ rows and $\binom{m}{p}$ columns).

For a subset $K \subset J$ with $p$ elements, let $(j_k)_{1 \leq k \leq p}$ be the sequence of elements of $K$ arranged in increasing order; by definition of $\wedge^p(u)$, by § 7, no. 2, formula (4)

$$
\wedge^p(u)(e_K) = u(e_{j_1}) \wedge u(e_{j_2}) \wedge \cdots \wedge u(e_{j_p}).
$$

Hence the element of the matrix of $\wedge^p(u)$ which is in the row of index $H$ and the column of index $K$ is the component of index $H$ of the element $u(e_{j_1}) \wedge \cdots \wedge u(e_{j_p})$; it is therefore equal to $\det(X_{H,K})$ by Proposition 9.

The matrix $(\det(X_{H,K}))$ is called the $p$-th exterior power of the matrix $X$ and is denoted by $\wedge^p(X)$. When $p = m = n$, $\wedge^n(X)$ is the matrix with the single element $\det(X)$.

#### Proposition 11 {#alg-iii-s8-prop-11 .statement}

Let $M$ be a free $A$-module of finite dimension $n$; for every endomorphism $u$ of $M$ and every ordered pair of elements $\xi, \eta$ of $A$,

$$
\det(\xi 1_M + \eta u) = \sum_{k \geq 0} \operatorname{Tr}(\wedge^k(u)) \xi^{n-k} \eta^k.
$$

Let $(e_i)_{1 \leq i \leq n}$ be a basis of $M$ and let $I = \{1, n\}$; to calculate the left hand side of (18), we must form the product

$$
(\xi e_1 + \eta u(e_1)) \wedge (\xi e_2 + \eta u(e_2)) \wedge \cdots \wedge (\xi e_n + \eta u(e_n))
$$

which is equal to the sum of the terms $\xi^{n-p} \eta^p z_K$, where

$$
z_K = x_1 \wedge x_2 \wedge \cdots \wedge x_n
$$

with $x_i = u(e_i)$ for $i \in K$, $x_i = e_i$ for $i \in H = I - K$, where the integer $p$ runs through the interval $[0, n]$ and, for each $p$, $K$ runs through the set of subsets of I with $p$ elements. If $i_1 < i_2 < \cdots < i_{n-p}$ (resp. $j_1 < j_2 < \cdots < j_p$) are the elements of H (resp. K) arranged in increasing order, we can write ($\S 7$, no. 8, Corollary 1 to Theorem 1 and formula (19))

$$
z_K = \rho_{H, K} e_{i_1} \wedge e_{i_2} \wedge \cdots \wedge e_{i_{n-p}} \wedge u(e_{j_1}) \wedge \cdots \wedge u(e_{j_p}).
$$

But if $X$ is the matrix of $u$ with respect to the basis $(e_i)$, then by Proposition 10

$$
u(e_{j_1}) \wedge \cdots \wedge u(e_{j_p}) = \sum_{L \in \mathfrak{F}_p(I)} (\det X_{L, K}) e_L
$$

and hence

$$
z_K = \rho_{H, K} \sum_{L \in \mathfrak{F}_p(I)} (\det X_{L, K}) e_H \wedge e_L.
$$

Now $H \cap L \neq \varnothing$ except for $L = K$; it therefore follows from $\S 7$, no. 8, formula (20) that $z_K = (\det X_{K, K}) e_1 \wedge e_2 \wedge \cdots \wedge e_n$ and formula (18) then follows from Proposition 10 and the definition of the trace of a matrix (II, $\S 10$, no. 11, formulae (49) and (50)).

#### Corollary {#alg-iii-s8-n5-cor-1 .statement}

*Under the same hypotheses as in Proposition 11, for the endomorphism $\bigwedge(u)$ of the A-module $\bigwedge(M)$*

$$(19)$$
$$
\operatorname{Tr}(\bigwedge(u)) = \det(1_M + u).
$$

It suffices to replace $\xi$ and $\eta$ by 1 in (18) and observe that the matrix of $\bigwedge(u)$ with respect to the basis of the $e_H$ ($H \in \mathfrak{F}(I)$) is the diagonal matrix of the matrices of the $\bigwedge^k(u)$ for $\geq k$ 0 (II, $\S 10$, no. 7, *Example* IV).

### 6. EXPANSIONS OF A DETERMINANT

Let I be a totally ordered finite indexing set. For every subset H of I let H' denote the complement I - H. Let $X = (\xi_{ij})$ be a square matrix of type (I, I), which can be considered as the matrix of an endomorphism $u$ of $M = A^I$ with respect to the canonical basis $(e_i)_{i \in I}$ of M. Let $n = \operatorname{Card}(I)$ and let H be a subset of I with $q \leq n$ elements and K a subset of I with $n - q$ elements; then we can write (no. 5, Proposition 10)

$$
(\bigwedge^q(u))(e_H) = \sum_R \det(X_{R, H}) e_R
$$
$$
(\bigwedge^{n-q}(u))(e_K) = \sum_S \det(X_{S, K}) e_S
$$

where R (resp. S) runs through the set of subsets of I with $q$ (resp. $n - q$) elements. It follows from $\S 7$, no. 8, formulae (19) and (20) that

$$
e_R \wedge e_S = 0
$$

except when $S = R'$, whence the formula

$$
(20) \quad (\wedge^q(u)(e_H)) \wedge (\wedge^{n-q}(u)(e_K)) = \sum_R \rho_{R, R'} \det(X_{R, H}) \det(X_{R', K}) e_I
$$

where $R$ runs through the set $\mathcal{F}_q(I)$ of subsets of $I$ with $q$ elements.

If we take $K = H'$, it follows from the definition of $\wedge^n(u)$ (\S 7, no. 2, formula (4)) and \S 7, no. 3, Corollary 1 to Proposition 5 that the right hand side of (20) is $\rho_{H, H'} \wedge^n(u)(e_I)$. Hence (no. 1, formula (1) and \S 7, no. 2, formula (4))

$$
(21) \quad \det(X) = \rho_{H, H'} \sum_{R \in \mathcal{F}_q; R' \neq R} \rho_{R, R'} \det(X_{R, H}) \det(X_{R', H'}).
$$

If on the other hand $K \neq H'$, then $H \cap K \neq \varnothing$; as the left hand side of (20) is $\pm \wedge^n(u)(e_H \wedge e_K)$, it is zero, whence

$$
(22) \quad \sum_R \rho_{R, R'} \det(X_{R, H}) \det(X_{R', K}) = 0 \quad \text{for } K \neq H'.
$$

The right hand side of (21) is called the *Laplace expansion* of the determinant of the matrix $X$ *by the q columns whose indices belong to H and the n - q columns whose indices belong to the complement H' of H*. The minors $\det(X_{R, H})$ and $\det(X_{R', H'})$ are sometimes called *complementary*.

An important simple case of the Laplace expansion is that where $I = \{1, n\}$ and $q = 1$, hence $H = \{i\}$; for every subset $R = \{j\}$ of $I$ with one element then $\det X_{R, H} = \xi_{ji}$. The minor of $\det X_{R', H'}$ is the determinant of the square matrix derived canonically (no. 5) from the matrix obtained by suppressing in $X$ the row of index $j$ and the column of index $i$. We denote this square matrix by $X^{ji}$. Obviously $\rho_{H, H'} = (-1)^{i-1}$ and $\rho_{R, R'} = (-1)^{j-1}$; therefore (21) becomes in this case

$$
(23) \quad \det X = \sum_{j=1}^n (-1)^{i+j} \xi_{ji} \det(X^{ji})
$$

and we obtain similarly from (22)

$$
(24) \quad \sum_{j=1}^n (-1)^{ji} \xi_{ji} \det(X^{jk}) = 0 \quad \text{for } k \neq i.
$$

Formula (23) is known as the *expansion of the determinant of X by the column of index i*. The scalar $(-1)^{i+j} \det(X^{ji})$ is called the *cofactor* of indices $j$ and $i$ (or, by an abuse of language, the cofactor of $\xi^{ji}$) in $X$.

The *matrix of cofactors* of $X$ is the matrix

$$
(25) \quad Y = ((-1)^{i+j} \det(X^{ji}))
$$

whose element in the $j$-th row and $i$-th column is the cofactor of indices $j$ and $i$. Formulae (23) and (24) are equivalent to the formula

$$(26)$$
$$
{}^tY . X = (\det X) I_n.
$$

Therefore:

#### Proposition 12 {#alg-iii-s8-prop-12 .statement}

*For every invertible square matrix $X$ of type $(n, n)$, the inverse of $X$ is given by the formula*

$$(27)$$
$$
X^{-1} = (\det X)^{-1} {}^t Y
$$

*where $Y$ is the cofactor matrix of $X$.*

By considering the *transpose* of $X$ and using Proposition 8 of no. 5, the Laplace expansions could be obtained relative to two complementary sets of rows and, in particular, the expansion of $\det X$ by a row, thus there are formulae equivalent to

$$(28)$$
$$
X . {}^t Y = (\det X) I_n,
$$

in the above notation.

It is easily verified that if $X$ is the matrix of an endomorphism $u$ of a free $\mathbf{A}$-module $M$ of dimension $n$ with respect to a basis $(e_i)_{1 \leq i \leq n}$, ${}^t Y$ is the matrix of the endomorphism $\tilde{u}$ of $M$ defined by the following condition: for every set of $n$ elements $x, y_2, \ldots, y_n$ of $M$,

$$
\tilde{u}(x) \wedge y_2 \wedge \cdots \wedge y_n = x \wedge u(y_2) \wedge \cdots \wedge u(y_n).
$$

$\tilde{u}$ is called the *cotranspose* of $u$ (cf. § 11, no. 11, Corollary to Proposition 13).

#### Example {#alg-iii-s8-n6-exa-1 .statement}

(1) *Vandermonde determinant.* Given a sequence $(\zeta_i)_{1 \leq i \leq n}$ of $n$ elements of $\mathbf{A}$, the *Vandermonde determinant* of this sequence is the determinant

$$
V(\zeta_1, \zeta_2, \ldots, \zeta_n) = \begin{vmatrix}
1 & 1 & \ldots & 1 \\
\zeta_1 & \zeta_2 & \ldots & \zeta_n \\
\zeta_1^2 & \zeta_2^2 & \ldots & \zeta_n^2 \\
\vdots & \vdots & \ddots & \vdots \\
\zeta_1^{n-1} & \zeta_2^{n-1} & \ldots & \zeta_n^{n-1}
\end{vmatrix}
$$

We shall show that

$$(29)$$
$$
V(\zeta_1, \zeta_2, \ldots, \zeta_n) = \prod_{i < j} (\zeta_j - \zeta_i).
$$

Since the proposition is immediate for $n = 1$, we argue by induction on $n$.

For each index $k \geq 2$, we subtract from the row of index $k$ the row of index $k - 1$ multiplied by $\zeta_1$; the value of the determinant is unaltered and hence

$$
V(\zeta_1, \zeta_2, \ldots, \zeta_n) = \begin{vmatrix}
1 & 1 & \cdots & 1 \\
0 & \zeta_2 - \zeta_1 & \cdots & \zeta_n - \zeta_1 \\
0 & \zeta_2(\zeta_2 - \zeta_1) & \cdots & \zeta_n(\zeta_n - \zeta_1) \\
\cdots & \cdots & \cdots & \cdots \\
0 & \zeta_2^{n-2}(\zeta_2 - \zeta_1) & \cdots & \zeta_n^{n-2}(\zeta_n - \zeta_1)
\end{vmatrix}
$$

whence, expanding by the first column and then taking out the factor $\zeta_k - \zeta_1$ from the column of index $k - 1$ from the minor thus obtained ($2 \leq k \leq n$)

$$
V(\zeta_1, \ldots, \zeta_n) = (\zeta_2 - \zeta_1)(\zeta_3 - \zeta_1) \cdots (\zeta_n - \zeta_1) V(\zeta_2, \ldots, \zeta_n)
$$

which establishes (29) by induction.

(2) Consider a square matrix of order $n$ which is presented in the form of an "upper triangular matrix of matrices" (II, § 10, no. 7, Example IV)

$$
X = \begin{pmatrix} Y & T \\ 0 & Z \end{pmatrix}
$$

We show that

$$
\det X = (\det Y)(\det Z).
$$

Let $n$ be the order of the matrix $X$, $h$ that of $Y$, $(e_i)_{1 \leq i \leq n}$ the canonical basis of $\mathbf{A}^n$ and $x_i$ ($1 \leq i \leq n$) the columns of $X$; the hypothesis implies that the columns $x_1, \ldots, x_h$ belong to the submodule of $\mathbf{A}^n$ with basis $e_1, \ldots, e_h$ and then by definition (no. 3, formula (6))

$$
x_1 \wedge x_2 \wedge \cdots \wedge x_n = (\det Y)e_1 \wedge e_2 \wedge \cdots \wedge e_h.
$$

On the other hand, for every index $i > h$, we can write $x_i = y_i + z_i$, where $y_i$ is a linear combination of $e_1, e_2, \ldots, e_h$ and $z_i$ is a linear combination of $e_{h+1}, \ldots, e_n$. By (30), $x_1 \wedge x_2 \wedge \cdots \wedge x_n \wedge y_i = 0$ for all $i > h$, therefore

$$
x_1 \wedge x_2 \wedge \cdots \wedge x_n = (\det Y)e_1 \wedge e_2 \wedge \cdots \wedge e_h \wedge z_{h+1} \wedge \cdots \wedge z_n.
$$

But by definition

$$
z_{h+1} \wedge z_{h+2} \wedge \cdots \wedge z_n = (\det Z)e_{h+1} \wedge e_{h+2} \wedge \cdots \wedge e_n
$$

whence formula (30).

By induction on $p$, it follows that if $X$ is of the form of an upper triangular matrix of matrices:

$$
X = \begin{pmatrix}
X_{11} & X_{12} & \cdots & X_{1p} \\
0 & X_{22} & \cdots & X_{2p} \\
\cdots & \cdots & \cdots & \cdots \\
0 & 0 & \cdots & X_{pp}
\end{pmatrix}
$$

(31) $$
\det X = (\det X_{11})(\det X_{22}) \ldots (\det X_{pp}).
$$

This can be applied in particular to a triangular matrix (where all the $X_{ii}$ are of order 1) and more particularly to a diagonal matrix:

(32) $$
\det(\operatorname{diag}(\alpha_1, \alpha_2, \ldots, \alpha_n)) = \alpha_1 \alpha_2 \ldots \alpha_n.
$$

(3) Let $M, M'$ be two free $A$-modules of respective dimensions $n, n'$, $u$ an endomorphism of $M$ and $u'$ an endomorphism of $M'$. Then

(33) $$
\det(u \otimes u') = (\det u)^{n'} (\det u')^n.
$$

For we can write $u \otimes u' = (u \otimes 1_{M'}) \circ (1_M \otimes u')$ and are then led to the case where one of the two endomorphisms $u, u'$ is the identity. For example if $u' = 1_{M'}$ and $X$ is the matrix of $u$ with respect to a basis $(e_i)$ of $M$, then the matrix of $u \otimes 1_{M'}$ with respect to the tensor product of $(e_i)$ and a basis of $M'$ can be written as a matrix (with $n'$ rows and $n'$ columns) of matrices with $n$ rows and $n$ columns

$$
\begin{pmatrix}
X & 0 & \ldots & 0 \\
0 & X & \ldots & 0 \\
\ldots & \ldots & \ldots & \ldots \\
0 & 0 & \ldots & X
\end{pmatrix}
$$

whence, by virtue of *Example 2*,

$$
\det(u \otimes 1_{M'}) = (\det X)^{n'} = (\det u)^{n'}
$$

which immediately gives formula (33).

### 7. APPLICATION TO LINEAR EQUATIONS

Consider a system of $n$ scalar linear equations in $n$ unknowns over a (*commutative*) ring $A$ (II, § 2, no. 8):

(34) $$
\sum_{j=1}^n \lambda_{ij} x_j = \eta_i \quad (1 \leq i \leq n).
$$

Let $L$ be the square matrix $(\lambda_{ij})$ of order $n$; by identifying as usual the matrix with one column consisting of the $\xi_i$ (resp. the $\eta_i$) with an element $x = (\xi_i)$ of $\mathbf{A}^n$ (resp. the element $y = (\eta_i)$ of $\mathbf{A}^n$), system (34) may also be written (II, § 10, no. 3, Proposition 2)

(35)
$$
L.x = y.
$$

Let $u$ be the endomorphism $x \mapsto L.x$ of $\mathbf{A}^n$, with $L$ as matrix with respect to the canonical basis; to say that equation (35) has (at least) one solution for all $y \in \mathbf{A}^n$ means that $u$ is surjective; Theorem 1 of no. 2 then implies the following proposition:

#### Proposition 13 {#alg-iii-s8-prop-13 .statement}

*For a system of $n$ linear equations in $n$ unknowns over a commutative ring to admit at least one solution regardless of the right hand sides, it is necessary and sufficient that the determinant of the matrix of the system be invertible; in this case the system admits a single solution.*

If $\det L$ is not a divisor of zero in $\mathbf{A}$, equation (34) is equivalent to the equation
$$
(\det L)L.x = (\det L)y.
$$
If $M$ is the cofactor matrix of $L$, we derive from (34) and formula (26) of no. 6 the relation
(36)
$$
(\det L)x = {}^tM.y
$$
which may also be written
(37)
$$
(\det L)\xi_i = \sum_{j=1}^n (-1)^{i+j}(\det L^{ij})\eta_j = \det L_i \quad (1 \leq i \leq n)
$$
where $L_i$ denotes the matrix obtained by replacing the column of $L$ of index $i$ by $y$. Formulae (37) are called *Cramer's formulae* for system (34); every solution of (34) is also a solution of (37). Conversely, we derive from (36), taking account of formula (28) of no. 6,
(38)
$$
(\det L)(L.x - y) = 0
$$
and hence, if $\det L$ is not a divisor of zero in $\mathbf{A}$, systems (34) and (37) are *equivalent*; if $\det L$ is invertible, the unique solution of (34) is given by
(39)
$$
\xi_i = (\det L)^{-1}(\det L_i) \quad (1 \leq i \leq n).
$$
A system (34) such that $\det L$ is invertible is also called a *Cramer system*.

In particular let $y = 0$; it then follows from Proposition 3 of no. 2 that:

#### Proposition 14 {#alg-iii-s8-prop-14 .statement}

*For a homogeneous linear system of $n$ equations in $n$ unknowns over a commutative ring to admit a non-zero solution, it is necessary and sufficient that the determinant of its matrix be a divisor of zero.*

### 8. CASE OF A COMMUTATIVE FIELD

All the above applies when the ring $\mathbf{A}$ is a commutative field; but there are simplifications and additional results.

Thus Proposition 12 of § 7, no. 9 can be formulated in this case as follows:

#### Proposition 15 {#alg-iii-s8-prop-15 .statement}

Let $\mathbf{E}$ be a vector space over a commutative field; for $p$ vectors $x_i \in \mathbf{E}$ ($1 \leq i \leq p$) to be linearly independent, it is necessary and sufficient that $x_1 \wedge x_2 \wedge \cdots \wedge x_p \neq 0$.

#### Corollary {#alg-iii-s8-n8-cor-1 .statement}

Let $X$ be a matrix of type $(m, n)$ over a commutative field. The rank of $X$ is equal to the greatest integer $p$ such that there exists at least one minor of $X$ of order $p$ which is $\neq 0$.

The rank of $X$ is the maximum number of linearly independent columns of $X$ (II, § 10, no. 12, Definition 7). The corollary then follows from Proposition 15 and formula (17) of no. 5.

Consider now the case of a system of $m$ linear equations in $n$ unknowns over a commutative field $\mathbf{K}$:

$$
\sum_{j=1}^n \lambda_{ij} \xi_j = \eta_i \quad (1 \leq i \leq m).
$$

(41)

#### Proposition 16 {#alg-iii-s8-prop-16 .statement}

Let $L = (\lambda_{ij})$ be the matrix (of type $(m, n)$) of system (41). Let $M$ be the matrix of type $(m, n+1)$ obtained by adding to $L$ the $(n+1)$-th column $(\eta_i)$ (II, § 10, no. 1). Let $p$ be the rank of $L$ (calculated by applying the Corollary to Proposition 15). Suppose that the minor $\Delta$ of $L$, the determinant of the matrix by suppressing the rows and columns of index $\geq p + 1$ in $L$, is $\neq 0$ (which is always possible by means of a suitable permutation on the rows of $L$ and a suitable permutation on the columns of $L$). Then, for system (41) to have at least one solution it is necessary and sufficient that all the minors of order $p + 1$ of $M$, the determinants of the submatrices of order $p + 1$ of $M$ whose columns have indices $1, 2, \ldots, p$ and $n+1$, be zero. If this is so, the solutions of system (41) are those of the system consisting of the first $p$ equations; if they are written

$$
\sum_{j=1}^p \lambda_{ij} \xi_j = \eta_i - \sum_{k=p+1}^n \lambda_{ik} \xi_k \quad (1 \leq i \leq p)
$$

all the solutions of this system are obtained by taking for the $\xi_k$ of index $k > p$ arbitrary values and applying Cramer's formulae (no. 7, formulae (37)) to calculate the $\xi_j$ of index $j \leq p$.

We know (II, § 10, no. 12, Proposition 12) that for the system (41) to have at least one solution, it is necessary and sufficient that the matrices $L$ and $M$ have the same rank. With the rows and columns of $L$ permuted to satisfy the condition of the statement, let $a_i$ ($1 \leq i \leq p$) denote the first $p$ columns of $L$ and $y = (\eta_i)$ the $(n+1)$-th column of $M$; since all the columns of $L$ are by hypothesis linear combinations of the $a_i$, to say that $M$ has the same rank $p$ as $L$ means that $y$ is a linear combination of the $a_i$, or also (Proposition 15) that $a_1 \wedge \cdots \wedge a_p \wedge y = 0$. The possibility condition in the statement is the translation of the latter relation, taking account of formula (17) of no. 5. Moreover, since the first $p$ rows of $M$ are linearly independent, the rows of index $> p$ are linear combinations of them and hence every solution of (42) is also a solution of (41). The last assertion is then an immediate consequence of Proposition 13 of no. 7.

### 9. THE UNIMODULAR GROUP $\mathbf{SL}(n, A)$

Let $\mathbf{M}_n(A)$ denote the ring of square matrices of order $n$ over $A$. Consider the mapping $\det : \mathbf{M}_n(A) \to A$. The group $\mathbf{GL}(n, A)$ of invertible elements of $\mathbf{M}_n(A)$ (isomorphic to the group of automorphisms of the $A$-module $A^n$ (II, § 10, no. 7)) is just the inverse image under this mapping of the multiplicative group $A^*$ of invertible elements of $A$ (no. 3, Proposition 5). Note on the other hand that the mapping $\det : \mathbf{GL}(n, A) \to A^*$ is a group homomorphism (no. 3, Proposition 5).

The mapping $\det : \mathbf{M}_n(A) \to A$ is moreover *surjective* (and therefore so is the homomorphism $\det : \mathbf{GL}(n, A) \to A^*$); since, for all $\lambda \in A$,

$$
\det(\operatorname{diag}(\lambda, 1, \ldots, 1)) = \lambda
$$

by virtue of formula (32) of no. 6.

The *kernel* of the surjective homomorphism $\det : \mathbf{GL}(n, A) \to A^*$ is a normal subgroup of $\mathbf{GL}(n, A)$, which is composed of *unimodular* matrices; it is denoted by $\mathbf{SL}_n(A)$ or $\mathbf{SL}(n, A)$ and is often called the *unimodular group* or *special linear group* of square matrices of order $n$ over $A$.

In this no. we shall examine the case where $A$ is a *field*. Recall that for $1 \leq i \leq n, 1 \leq j \leq n$, $E_{ij}$ denotes the square matrix of order $n$ all of whose elements are zero except the one in the row of index $i$ and the column of index $j$, which is equal to 1; with $I_n$ denoting the unit matrix of order $n$, we write $B_{ij}(\lambda) = I_n + \lambda E_{ij}$ for every ordered pair of *distinct* indices $i, j$ and all $\lambda \in A$ (II, § 10, no. 13).

#### Proposition 17 {#alg-iii-s8-prop-17 .statement}

*Let $K$ be a commutative field. The unimodular group $\mathbf{SL}(n, K)$ is generated by the matrices $B_{ij}(\lambda)$ with $i \neq j$ and $\lambda \in K$.*

By II, § 10, no. 13, Proposition 14, we know that every matrix in $\mathbf{GL}(n, K)$ is a product of matrices of the form $B_{ij}(\lambda)$ and a matrix of the form $\operatorname{diag}(1, 1, \ldots, 1, \alpha)$ with $\alpha \in K^*$. Now it is immediate that $\det(B_{ij}(\lambda)) = 1$ and $\det(\operatorname{diag}(1, \ldots, 1, \alpha)) = \alpha$ (no. 6, *Example 2*); whence the proposition.

#### Corollary {#alg-iii-s8-n9-cor-1 .statement}

*The group* $\mathbf{SL}(n, K)$ *is the group of commutators of* $\mathbf{GL}(n, K)$, *except in the case where* $n = 2$ *and where* $K$ *is a field with 2 elements*.

As $\mathbf{SL}(n, K)$ is the kernel of the homomorphism det of $\mathbf{GL}(n, K)$ to a commutative group $K^*$, $\mathbf{SL}(n, K)$ contains the commutator group $\Gamma$ of $\mathbf{GL}(n, K)$ (I, § 6, no. 2). To prove that $\mathbf{SL}(n, K) = \Gamma$, it will suffice, by Proposition 17, to show that, for all $\lambda \in K^*$, $B_{ij}(\lambda)$ belongs to $\Gamma$. Now, $B_{ij}(\lambda)$ is a conjugate of $B_{ij}(1)$ in $\mathbf{GL}(n, K)$ since $B_{ij}(\lambda) = Q . B_{ij}(1) . Q^{-1}$, where $Q$ denotes the matrix with respect to the canonical basis $(e_i)$ of the automorphism $v$ of $K^n$ such that $v(e_i) = \lambda e_i, v(e_k) = e_k$ for $k \neq i$. On the other hand, let $u_{ij}$ (for $i \neq j$) be the automorphism of $K^n$ such that $u_{ij}(e_i) = -e_j, \ u_{ij}(e_j) = e_i, \ u_{ij}(e_k) = e_k$ for $k \notin \{i, j\}$, which belongs to $\mathbf{SL}(n, K)$; then $B_{ji}(\lambda) = U_{ij} B_{ij}(-\lambda) U_{ij}^{-1}$, where $U_{ij}$ is the matrix of $u_{ij}$ with respect to the canonical basis. Similarly, if $1 < i < j$, then $B_{1j}(\lambda) = U_{1i} B_{ij}(\lambda) U_{1i}^{-1}$ and finally, for $2 < j$, $B_{12}(\lambda) = U_{2j} B_{1j}(\lambda) U_{2j}^{-1}$. This proves that all the $B_{ij}(\lambda)$ have the same image $s$ in $\mathbf{GL}(n, K)/\Gamma$ and it remains to show that $s$ is the identity element.

Suppose first that $K$ contains an element $\lambda$ distinct from 0 and 1; then $1 = \lambda + (1 - \lambda)$, the two terms on the right hand side being $\neq 0$; the relation $B_{12}(1) = B_{12}(\lambda) B_{12}(1 - \lambda)$ shows that $s^2 = s$ and hence $s$ is the identity element.

Suppose now that $n \geq 3$. The product $B_{21}(1) B_{31}(1)$ is the matrix of an automorphism $u$ of $K^n$ such that $u(e_1) = e_1 + e_2 + e_3, u(e_i) = e_i$ for $i \neq 1$. If $S$ is the matrix of the automorphism $u'$ of $K^n$ such that $u'(e_2) = e_2 + e_3, u'(e_i) = e_i$ for $i \neq 2$, then $S . B_{21}(1) B_{31}(1) . S^{-1} = B_{21}(1)$; we also deduce that $s^2 = s$, which completes the proof.

#### Remark {#alg-iii-s8-n9-rem-1 .statement}

(1) $\mathbf{GL}(2, \mathbf{F}_2) = \mathbf{SL}(2, \mathbf{F}_2)$; this is a solvable group of order 6, whose commutator group is of index 2 (II, § 10, Exercise 14).

(2) With the same notation as above, it can be proved as in I, § 5, no. 7, Proposition 9 that, for $i < j, j - i > 1$, $u_{ij} = u_{j-1, j} u_i, _{j-1} u_{j-1, j}^{-1}$; hence *the group* $\mathbf{SL}(n, K)$ *is generated by the matrices* $B_{12}(\lambda)$ *and* $U_{i, i+1}$ *for* $1 \leq i \leq n - 1$.

### 10. THE $\mathbf{A}[X]$-MODULE ASSOCIATED WITH AN $\mathbf{A}$-MODULE ENDOMORPHISM

Let $M$ be an $\mathbf{A}$-module and $u$ an endomorphism of $M$. Consider the polynomial ring $\mathbf{A}[X]$ in one indeterminate $X$ over $\mathbf{A}$. For every polynomial $p \in \mathbf{A}[X]$ and all $x \in M$, we write

$$
p . x = p(u)(x).
$$

As $(pq)(u) = p(y) \circ q(u)$ for two polynomials $p, q$ of $\mathbf{A}[X]$, and $\mathbf{A}[X]$-module structure is thus defined on $M$; the set $M$, with this structure, will be denoted by $M_u$; the $\mathbf{A}$-module structure given on $M$ is obtained by restricting the ring of operators of $M_u$ to $\mathbf{A}$. Note that the submodules of $M_u$ are just the submodules of $M$ which are *stable* under $u$.

As the mapping $(p, x) \mapsto p.x$ of $A[X] \times M$ into $M$ is $A$-bilinear, it defines canonically an $A$-linear mapping $\phi : A[X] \otimes_A M \to M$ such that
$$
\phi(p \otimes x) = p.x = p(u)(x).
$$
On the other hand, $A[X] \otimes_A M$ has canonically an $A[X]$-module structure (II, § 5, no. 1); we shall denote this $A[X]$-module by $M[X]$; the mapping $\phi : M[X] \to M_u$ is $A[X]$-linear since, for $p, q$ in $A[X]$ and $x \in M$,
$$
\phi(q(p \otimes x)) = \phi((qp) \otimes x) = (qp).x = q(u)(p(u)(x)) = q.\phi(p \otimes x).
$$
Moreover, $u$ is an $A[X]$-endomorphism of $M_u$, for
$$
u(p.x) = u(p(u)(x)) = (up(x))(x) = p.u(x).
$$
Finally, an $A[X]$-endomorphism $\bar{u}$ of $M[X]$ is defined by writing (II, § 5, no. 1)
$$
\bar{u}(p \otimes x) = p \otimes u(x).
$$
Moreover it follows from formulae (44) and (45) that that $A[X]$-linear mappings $u, \bar{u}$ and $\phi$ are related by the relation
$$
\phi \circ \bar{u} = u \circ \phi.
$$
Let $\psi$ denote the $A[X]$-endomorphism $X - \bar{u}$ of $M[X]$, so that $\psi(p \otimes x) = (Xp) \otimes x - p \otimes u(x)$. We have the following proposition:

#### Proposition 18 {#alg-iii-s8-prop-18 .statement}

*The sequence of $A[X]$-homomorphisms*
$$
M[X] \xrightarrow{\psi} M[X] \xrightarrow{\phi} M_u \longrightarrow 0
$$
is exact.

As $\phi(1 \otimes x) = x$ for all $x \in M$, clearly $\phi$ is surjective; on the other hand,
$$
\phi(X(p \otimes x)) = X.\phi(p \otimes x) = u(\phi(p \otimes x)),
$$
in other words, $\phi \circ X = u \circ \phi = \phi \circ \bar{u}$ by (46); this proves that $\phi \circ \psi = 0$. It remains to verify that $\operatorname{Ker} \phi \subset \operatorname{Im} \psi$. For this note that, since the monomials $X^k$ ($k \geq 0$) form a basis of the $A$-module $A[X]$, every element $z \in M[X]$ can be written uniquely in the form $z = \sum_k X^k \otimes x_k$, where $(x_k)$ is a family of elements of $M$, of finite support. If $z \in \operatorname{Ker} \phi$, then $\phi(z) = \sum_k u^k(x_k) = 0$ and we can write
$$
z = \sum_k (X^k \otimes x_k - 1 \otimes u^k(x_k)) = \sum_k (X^k - \bar{u}^k)(1 \otimes x_k).
$$
But as the $A[X]$-endomorphisms $X$ and $\bar{u}$ of $M[X]$ are permutable, then

X^k - \bar{u}^k = (X - \bar{u}) \circ \left( \sum_{j=0}^{k-1} X^j \bar{u}^{k-j-1} \right) which proves that there exists a $y \in M[X]$ such that $z = \psi(y)$.

Now let $M'$ be another $A$-module and $u'$ an endomorphism of $M'$; let $M'_{u'}$, $\phi'$, $\bar{u}'$, $\psi'$ be the module and mapping obtained from $M'$ and $u'$ as $M_u$, $\phi$, $\bar{u}$, $\psi$ are obtained from $M$ and $u$. Then:

#### Proposition 19 {#alg-iii-s8-prop-19 .statement}

*For a mapping g of M into M' to be an A[X]-homomorphism of M_u into M'_u, it is necessary and sufficient that g be an A-homomorphism of M into M' such that $g \circ u = u' \circ g$. When this is so, if $\bar{g}$ is the A[X]-homomorphism of M[X] into M'[X] equal to $1_{A[x]} \otimes g$ (II, § 5, no. 1), the diagram*

$$
\begin{array}{cccccc}
M[X] & \xrightarrow{\psi} & M[X] & \xrightarrow{\phi} & M_u & \longrightarrow 0 \\
\downarrow \bar{g} & & \downarrow \bar{g} & & \downarrow g & \\
M'[X] & \xrightarrow{\psi'} & M'[X] & \xrightarrow{\phi'} & M'_{u'} & \longrightarrow 0
\end{array}
$$

is *commutative*.

The condition $g \circ u = u' \circ g$ is obviously necessary by (43) for $g$ to be an A[X]-homomorphism; it is sufficient, for it implies by induction that $g \circ u^n = {u'}^n \circ g$ for every integer $n > 0$. On the other hand, for all $x \in M$ and all $p \in A[X]$,

$$
\phi'(\bar{g}(p \otimes x)) = \phi'(p \otimes g(x)) = p(u')(g(x)) = g(p(u)(x)) = g(\phi(p \otimes x))
$$
and
$$
\bar{u}'(g(p \otimes x)) = \bar{u}'(p \otimes g(x)) = p \otimes u'(g(x)) = p \otimes g(u(x)) = \bar{g}(\bar{u}(p \otimes x))
$$
which proves the commutativity of diagram (48).

### 11. CHARACTERISTIC POLYNOMIAL OF AN ENDOMORPHISM

Let $M$ be a free $A$-module of dimension $n$ and $u$ an endomorphism of $M$. Consider the polynomial ring in two indeterminates $A[X, Y]$ and the $A[X, Y]$-module $M[X, Y] = A[X, Y] \otimes_A M$; let $\bar{u}$ be the endomorphism of the $A[X, Y]$-module $M[X, Y]$ canonically derived from $u$ (II, § 5, no. 1). It follows from no. 5, Proposition 11 that

$$
\det(X - Y \bar{u}) = \sum_{j=0}^n (-1)^j \mathrm{Tr}(\wedge^j(u)) X^{n-j} Y^j
$$

for if $U$ is the matrix of $u$ with respect to a basis $(e_i)_{1 \leq i \leq n}$ of $M$, $U$ is the matrix of $\bar{u}$ with respect to the basis $(1 \otimes e_i)_{1 \leq i \leq n}$ of $M[X, Y]$, hence

$$
\mathrm{Tr}(\wedge^j(\bar{u})) = \mathrm{Tr}(\wedge^j(u)).
$$

#### Definition 3 {#alg-iii-s8-def-3 .statement}

Let $M$ be a finite-dimensional free $A$-module and $u$ an endomorphism of $M$. The determinant of the endomorphism $X - \bar{u}$ of the free $A[X]$-module $M[X]$ is called the characteristic polynomial of $u$ and is denoted by $\chi_u(X)$.

If $M$ is of rank $n$, it follows from (49) that

$$
\chi_u(X) = \sum_{j=0}^n (-1)^j \operatorname{Tr}(\wedge^j(u)) X^{n-j}
$$

for $\det(X - Y \bar{u}) = \det(X . I_n + Y U)$ and $\det(X - \bar{u}) = \det(X . I_n - U)$. It is therefore seen that $\chi_u(X)$ is a monic polynomial of degree $n$, in which the coefficient of $X^{n-1}$ is $-\operatorname{Tr}(u)$ and the constant term is $(-1)^n \det(u)$.

#### Proposition 20 ("Cayley–Hamilton theorem") {#alg-iii-s8-prop-20 .statement}

For every endomorphism $u$ of a finite-dimensional free $A$-module, $\chi_u(u) = 0$.

In the notation of Proposition 18 ($\S 3$, no. 10), for all $x \in M$, $\chi_u(u)(x)$ is the image under $\phi$ of $\chi_u(X) \otimes x$. But if $v$ is the endomorphism of $M[X]$, the co-transpose of $X - \bar{u}$ (no. 6), then

$$
\chi_u(X) \otimes x = \chi_u(X)(1 \otimes x) = (X - \bar{u})(v(1 \otimes x))
$$

and the conclusion follows from Proposition 18 of no. 10.

### Exercises {#alg-iii-s8-exercises}

See the [exercises for § 8](exercises/s8/).
