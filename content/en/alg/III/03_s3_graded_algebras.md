---
book: alg
book_title: Algebra
chapter: III
chapter_title: TENSOR ALGEBRAS, EXTERIOR ALGEBRAS, SYMMETRIC ALGEBRAS
section: 3
section_title: Graded algebras
lang: en
source: alg-i-iii
source_edition: 1998, Springer
pdf_pages: 0481-0484, 0650-0650
extraction: ocr
subsections:
    - "no": 1
      title: GRADED ALGEBRAS
      page: 0
      pdf_page: 481
    - "no": 2
      title: GRADED SUBALGEBRAS, GRADED IDEALS OF A GRADED ALGEBRA
      page: 0
      pdf_page: 483
    - "no": 3
      title: DIRECT LIMITS OF GRADED ALGEBRAS
      page: 0
      pdf_page: 484
statements: 4
exercises: 1
content_sha256: 38b7965ea4ef3a096ea51873d498f423f82feaa31641e8044291d726b3d90f91
---

## § 3. GRADED ALGEBRAS

The graduations considered in this paragraph will have as set of degrees a *commutative monoid written additively whose identity element is denoted by 0*.

### 1. GRADED ALGEBRAS

#### Definition 1 {#alg-iii-s3-def-1 .statement}

*Let $\Delta$ be a commutative monoid, $A$ a graded ring of type $\Delta$* (II, § 11, no. 2), $(A_\lambda)_{\lambda \in \Delta}$ *its graduation and E an A-algebra. A graduation* $(E_\lambda)_{\lambda \in \Delta}$ *of type $\Delta$ on the additive group E is said to be compatible with the A-algebra structure on E if it is compatible both with the A-module and with the ring structure on E, in other words, if, for all $\lambda, \mu$ in $\Delta$,*

(1) $$ A_\lambda E_\mu \subset E_{\lambda + \mu} $$
(2) $$ E_\lambda E_\mu \subset E_{\lambda + \mu}. $$

*The A-algebra E, with this graduation, is then called a graded algebra of type $\Delta$ over the graded ring A.*

When the graduation on A is *trivial* (that is (II, § 11, no. 1) $A_0 = A, A_\lambda = \{0\}$ for $\lambda \neq 0$), condition (1) means that the $E_\lambda$ are *sub-A-modules* of E. This leads to the definition of the notion of graded algebra of type $\Delta$ over a *non-graded* commutative ring $A$: $A$ is given the trivial graduation of type $\Delta$ and the above definition is applied.

When we consider graded $A$-algebras $E$ with a *unit element* $e$, it will always be understood that $e$ is *of degree* 0 (cf. Exercise 1).

It follows that if an invertible element $x \in E$ is *homogeneous* and of degree $p$, its inverse $x^{-1}$ is *homogeneous* and of degree $-p$: it suffices to decompose $x^{-1}$ as a sum of homogeneous elements in the relations $x^{-1}x = xx^{-1} = e$.

Let $E$ and $E'$ be two graded algebras of type $\Delta$ over a graded ring $A$ of type $\Delta$. An $A$-algebra homomorphism $u : E \to E'$ is called a *graded algebra homomorphism* if $u(E_\lambda) \subset E'_\lambda$ for all $\lambda \in \Delta$ (where $(E_\lambda)$ and $(E'_\lambda)$ denote the respective graduations of $E$ and $E'$); where $E$ and $E'$ are associative and unital and $u$ is unital, this condition means that $u$ is a graded ring homomorphism (II, § 11, no. 2).

Let $E$ be a graded $A$-algebra of type $N$. $E$ is identified with a graded $A$-algebra of type $\mathbf{Z}$ by writing $E_n = \{0\}$ for $n < 0$.

#### Remark {#alg-iii-s3-n1-rem-1 .statement}

Definition 1 can also be interpreted by saying that $E$ is a graded $A$-module and that the $A$-linear mapping

$$
m : E \otimes_A E \to E
$$

defining the multiplication on $E$ (\S 1, no. 3), is *homogeneous of degree* 0 when $E \otimes_A E$ is given its graduation of type $\Delta$ (II, § 11, no. 5).

To define a graded $A$-algebra structure of type $\Delta$ on the graded ring $A$, with $E$ as underlying graded $A$-module, therefore amounts to defining for each ordered pair $(\lambda, \mu)$ of elements of $\Delta$ a $\mathbf{Z}$-bilinear mapping

$$
m_{\lambda \mu} : E_\lambda \times E_\mu \to E_{\lambda + \mu}
$$

such that for every triple of indices $(\lambda, \mu, \nu)$ and for $\alpha \in A_\lambda,\ x \in E_\mu,\ y \in E_\nu$,

$$
\alpha . m_{\mu \nu}(x, y) = m_{\lambda + \mu, \nu}(\alpha x, y) = m_{\mu, \lambda + \nu}(x, \alpha y).
$$

#### Example {#alg-iii-s3-n1-exa-1 .statement}

(1) Let $B$ be a *graded ring* of type $\Delta$; if $B$ is given its canonical $\mathbf{Z}$-algebra structure (\S 1, no. 1, *Example* 2), $B$ is a graded $A$-algebra ($\mathbf{Z}$ being given the trivial graduation).

(2) Let $A$ be a graded commutative ring of type $\Delta$ and $M$ a graded $A$-module of type $\Delta$. Suppose that all the elements of the monoid $\Delta$ are *cancellable*, which allows (II, § 11, no. 6) us to define on $\mathrm{Homgr}_A(M, M) = \mathrm{Endgr}_A(M)$ a graded $A$-module structure of type $\Delta$; as this graduation is compatible with the ring structure on $\mathrm{Endgr}_A(M)$ (II, § 11, no. 6), it defines a *unital graded $A$-algebra* structure on the $A$-algebra $\mathrm{Endgr}_A(M)$.

(3) *Algebra of a magma.* Let $S$ be a magma and $\phi : S \to \Delta$ a homomorphism. For all $\lambda \in \Delta$, we write $S_\lambda = \phi^{-1}(\lambda)$; then $S_\lambda S_\mu \subset S_{\lambda + \mu}$. Let $A$ be a graded commutative ring of type $\Delta$ and $(A_\lambda)_{\lambda \in \Delta}$ its graduation; we shall define a graded $A$-algebra structure on the algebra $E = A^{(S)}$ of the magma $S$ (\S 2, no. 6). To this end, let $E_{\lambda}$ denote the additive subgroup of $E$ generated by the elements of the form $\alpha.s$ such that $\alpha \in A_{\mu}, s \in S_{\nu}$ and $\mu + \nu = \lambda$. As the $S_{\lambda}$ are pairwise disjoint, $E$ is the direct sum of the $A_{\mu}S_{\nu}$ and hence also the direct sum of the $E_{\lambda}$ and it is immediate that the $E_{\lambda}$ satisfy conditions (1) and (2) and therefore define on $E$ the desired graded $A$-algebra structure. If $S$ admits an identity element $e$, it may also be supposed that $\phi(e) = 0$. A particular case is the one where the graduation of the ring $A$ is trivial; then $E_{\lambda}$ is the sub-$A$-module of $E$ generated by $S_{\lambda}$. More particularly, if we take $S = \mathbf{N}^{(1)}, \Delta = \mathbf{N}$ and $\phi$ the mapping such that $\phi((n_i)) = \sum_{i \in I} n_i$, the ring $A$ having the trivial graduation, a graduation is thus obtained on the polynomial algebra $A[X_i]_{i \in I}$, for which the degree of a homogeneous polynomial $\neq 0$ is the total degree defined in § 2, no. 9 (cf. § 6, no. 6).

We now take $S$ to be the free monoid $Mo(B)$ of a set $B$ (I, § 7, no. 2) and $\phi$ the homomorphism $Mo(B) \to \mathbf{N}$ which associates with each word its length. Thus a graded $A$-algebra structure is obtained on the free associative algebra of the set $B$ (§ 2, no. 7; cf. § 5, no. 5).

### 2. GRADED SUBALGEBRAS, GRADED IDEALS OF A GRADED ALGEBRA

Let $E$ be a graded algebra of type $\Delta$ over a graded ring $A$ of type $\Delta$. If $F$ is a sub-$A$-algebra of $E$ which is a graded sub-$A$-module, then the graduation $(F_{\lambda})$ on $F$ is compatible with its $A$-algebra structure, since $F_{\lambda} = F \cap E_{\lambda}$; in this case $F$ is called a graded subalgebra of $E$ and the canonical injection $F \to E$ is a graded algebra homomorphism.

Similarly, if $a$ is a left (resp. right) ideal of $E$ which is a graded sub-$A$-module, then $E_{\lambda}a_{\mu} \subset a_{\lambda+\mu}$ (resp. $a_{\lambda}E_{\mu} \subset a_{\lambda+\mu}$), since $a_{\lambda} = a \cap E_{\lambda}$; then $a$ is called a graded ideal of the algebra $E$. If $b$ is a graded two-sided ideal of $E$ the quotient graduation on the module $E/b$ is compatible with the algebra structure on $E/b$ and the canonical homomorphism $E \to E/b$ is a graded algebra homomorphism.

If $u : E \to E'$ is a graded algebra homomorphism, $\operatorname{Im}(u)$ is a graded subalgebra of $E'$, $\operatorname{Ker}(u)$ is a graded two-sided ideal of $E$ and the bijection $E/\operatorname{Ker}(u) \to \operatorname{Im}(u)$ canonically associated with $u$ is a graded algebra isomorphism.

#### Proposition 1 {#alg-iii-s3-prop-1 .statement}

*Let $A$ be a graded commutative ring of type $\Delta$, $E$ a graded $A$-algebra of type $\Delta$ and $S$ a set of homogeneous elements of $E$. Then the sub-$A$-algebra (resp. left ideal, right ideal, two-sided ideal) generated by $S$ is a graded subalgebra (resp. graded ideal).*.

The subalgebra of $E$ generated by $S$ is the sub-$A$-module generated by the finite products of elements of $S$, which are homogeneous; similarly, the left (resp. right) ideal generated by $S$ is the sub-$A$-module generated by the elements of the form $u_1(u_2(\ldots(u_n s))\ldots)$ (resp. $(\ldots((s u_n) u_{n-1})\ldots) u_2$ ) $u_1$ ) where s ∈ S and the u_j ∈ E are homogeneous (n arbitrary) and these products are homogeneous, whence in this case the conclusion by virtue of II, § 11, no. 3, Proposition 2); finally the two-sided ideal generated by S is the union of the sequence (\mathfrak{I}_n)_{n \geq 1}, where \mathfrak{I}_1 is the left ideal generated by S and \mathfrak{I}_{2n} (resp. \mathfrak{I}_{2n+1}) the right (resp. left) ideal generated by \mathfrak{I}_{2n-1} (resp. \mathfrak{I}_{2n}), which completes the proof.

### 3. DIRECT LIMITS OF GRADED ALGEBRAS

Let (A_\alpha, \phi_{\beta \alpha}) be a directed direct system of graded commutative rings of type \Delta (II, § 11, no. 3, Remark 3) and for each \alpha let E_\alpha be a graded A_\alpha-algebra of type \Delta; for \alpha \leq \beta let f_{\beta \alpha}: E_\alpha \to E_\beta be an A_\alpha-homomorphism of graded algebras and suppose that f_{\gamma \alpha} = f_{\gamma \beta} \circ f_{\beta \alpha} for \alpha \leq \beta \leq \gamma; then we shall call (E_\alpha, f_{\beta \alpha}) a directed direct system of graded algebras of type \Delta over the directed direct system (A_\alpha, \phi_{\beta \alpha}) of graded commutative rings of type \Delta. Then we know (II, § 11, no. 3) that E = \lim \to E_\alpha has canonically a graded module structure of type \Delta over the graded ring A = \lim \to A_\alpha and a multiplication such that E^\lambda E^\mu \subset E^{\lambda + \mu} (where (E^\lambda) denotes the graduation on E); then this multiplication and the graded A-module structure on E define on E a graded A-algebra structure of type \Delta; E, with this structure, is called the direct limit of the direct system (E_\alpha, f_{\beta \alpha}) of graded algebras. The canonical homomorphisms E_\alpha \to E are taken A_\alpha-homomorphisms of graded algebras. Moreover, if F is a graded A-algebra of type \Delta and (u_\alpha) a direct system of A_\alpha-homomorphisms u_\alpha: E_\alpha \to F, u = \lim \to u_\alpha is an A-homomorphism of graded algebras.

### Exercises {#alg-iii-s3-exercises}

See the [exercises for § 3](exercises/s3/).
