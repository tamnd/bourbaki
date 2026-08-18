---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 20
section_title: Linear Representations of Algebras
lang: en
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.373-A VIII.395
pdf_pages: 0390-0412
extraction: native
subsections:
    - "no": 1
      title: Linear Representations of Algebras
      page: 373
      pdf_page: 390
    - "no": 2
      title: Restricted Dual of an Algebra
      page: 375
      pdf_page: 392
    - "no": 3
      title: Coefficients of a Module
      page: 377
      pdf_page: 394
    - "no": 4
      title: Restricted Dual and Matrix Coefficients
      page: 379
      pdf_page: 396
    - "no": 5
      title: Dual of a Semisimple Algebra
      page: 380
      pdf_page: 397
    - "no": 6
      title: Character of a Representation
      page: 382
      pdf_page: 399
    - "no": 7
      title: Coefficients of a Set of Classes of Modules
      page: 387
      pdf_page: 404
    - "no": 8
      title: Cogebra Structure on the Restricted Dual
      page: 388
      pdf_page: 405
statements: 31
exercises: 6
content_sha256: ab1eeb296cdba4d1b5d1004662d942df3022c1945cba00edb9d329ba7f5e562b
---

## § 20. LINEAR REPRESENTATIONS OF ALGEBRAS

In this section, K is a commutative ring, and A is a K-algebra. From No. 2 on, we assume that K is a field, and we denote by $A^*$ the dual of the vector space A over K. In this section, the notation $A^*$ never refers to the multiplicative group of the ring A.

### 1. Linear Representations of Algebras

#### Definition 1 {#alg-viii-s20-def-1 .statement tag=00MD}

Let M be a K-module. A linear representation of the algebra A in M is a K-homomorphism $\pi$ from A to the algebra End$_K(M)$.

We also say that the pair $(M, \pi )$ is a linear representation of the algebra A. When M is a free K-module, the dimension of M is called the degree (or dimension) of $\pi$.

Let $\pi$ be a linear representation of A in M. The additive law on M and the external law $(a, x)\mapsto \pi (a)(x)$ define a left A-module structure on M, which we denote by $M_{\pi}$. We say that $M_{\pi}$ is the module of the representation $\pi$. The K-module structure on M is obtained from the A-module structure on $M_{\pi}$ by restriction of scalars.

Conversely, let E be a left A-module. Let M be the K-module deduced from E by restriction of scalars from A to K, and let $\pi$ be the homomorphism $a\mapsto a_E$ from A to End$_K(M)$. Then $\pi$ is a representation of A in M, and we have $E = M_{\pi}$. We say that $\pi$ is the linear representation associated with the A-module E.

Studying A-modules or linear representations of A amounts to the same. We will translate certain definitions concerning modules to the language of linear representations.

Let $\pi$ be a linear representation of A in M. The kernel of the homomorphism $\pi$ is a two-sided ideal of A, which is simply the annihilator of the A-module $M_{\pi}$. The homomorphism $\pi$ is injective if and only if the A-module $M_{\pi}$ is faithful; we then say that $\pi$ is a faithful representation of A.

Let $(M, \pi )$ and $(M', \pi ')$ be linear representations of A. An A-linear mapping from $M_{\pi}$ to $M'_{\pi'}$ is a K-linear mapping $u: M\rightarrow M'$ that satisfies the relation

$$
\pi '(a)\circ u=u\circ \pi (a) \tag{1}
$$

for $a\in A$. An isomorphism from $M_{\pi}$ to $M'_{\pi'}$ is an isomorphism of K-modules $u: M\rightarrow M'$ satisfying the condition

$$
\pi '(a) =u\circ \pi (a)\circ u^{-1} \tag{2}
$$

for $a\in A$. We say that $\pi$ and $\pi '$ are isomorphic if the A-modules $M_{\pi}$ and $M'_{\pi'}$ are isomorphic. We say that $\pi$ is a subrepresentation (resp. a quotient representation) of $\pi '$ if $M_{\pi}$ is a submodule (resp. a quotient module) of $M'_{\pi'}$.

Suppose given a family $(M_i, \pi_i)$ of linear representations of A. Let M be the K-module that is the direct sum of the $M_i$; for any $a\in A$, let $\pi (a)$ be the endomorphism $(x_i)_{i\in I}\mapsto (\pi_i(a)(x_i))_{i\in I}$ of M. Then $\pi$ is a linear representation of A in M. The A-module $M_{\pi}$ is the direct sum of the A-modules $(M_i)_{\pi}(i\in I)$; we say that $\pi$ is the direct sum of the $\pi_i$, and we write $\pi =\bigoplus\pi_{i^i}$.

We say that the representation $\pi$ of A in M is simple or irreducible if the A-module $M_{\pi}$ is simple; we say that the representation $\pi$ of A on M is semisimple or completely reducible if the A-module $M_{\pi}$ is semisimple.

Let $\pi$ be a linear representation of A in M. Let $M^*$ be the K-module dual to M. The mapping $a\mapsto^t(\pi (a))$ from $A^o$ to End$_K(M^*)$ is the transposed representation of $\pi$.

Let L be a commutative K-algebra, and let $(M, \pi )$ be a linear representation of the K-algebra A. The homomorphism $\pi_{(L)}: A_{(L)}\rightarrow$ End$_L(M_{(L)})$ corresponding to the $A_{(L)}$-module structure on $M_{(L)}$ is a linear representation of the L-algebra $A_{(L)}$. We say that $\pi_{(L)}$ is the linear representation of the algebra $A_{(L)}$ deduced from the representation $\pi$ by extending the ring of scalars K to L.

Suppose that K is a field and that L is a nonzero commutative K-algebra.

Let $\pi$ and $\pi '$ be linear representations of the algebra A. It follows from VIII, p. 37, Theorem 3 that the representations $\pi$ and $\pi '$ are isomorphic if and only if $\pi_{(L)}$ and $\pi '_{(L)}$ are.

Suppose that K is a field. Let L be an extension of K. Consider the Grothendieck group $R_K(A)$ (resp. $R_L(A_{(L)}))$ of the A-modules that are finite-dimensional over K (resp. of the $A_{(L)}$-modules that are finite-dimensional over L). We have seen that the group homomorphism

$$
u: R_K(A)\longrightarrow R_L(A_{(L)})
$$

defined by extension of scalars is injective; moreover, an element $\xi \in R_K(A)$ is effective if and only if $u(\xi )$ is (VIII, p. 195, Theorem 1).

### 2. Restricted Dual of an Algebra

We assume from now on that K is a field.

For $a\in A$, denote by $\boldsymbol{\gamma }(a)$ the mapping $x\mapsto ax$ and by $\boldsymbol{\delta }(a)$ the mapping $x\mapsto xa$ from A to A. Then $\boldsymbol{\gamma }$ is a linear representation of A in A, called the left regular representation; likewise, $\boldsymbol{\delta }$ is a linear representation of $A^o$ in A, called (by abuse of language) the right regular representation of A. By transposition, we deduce from $\boldsymbol{\delta }$ and $\boldsymbol{\gamma }$ linear representations of the algebras A and $A^o$ in the vector space $A^*$ that define on $A^*$ a left A-module structure and a left $A^o$-module structure. These two structures correspond to an $(A$, A)-bimodule structure on $A^*$ with external laws defined by the formulas

$$
\langle af, b\rangle =\langle f, ba\rangle \tag{3}
$$

$$
\langle f a, b\rangle =\langle f, ab\rangle \tag{4}
$$

for $a, b,\in A$ and $f\in A^*$.

Recall (II, §2, No. 4, p. 234, Definition 4) that if E is a linear subspace of A, then its orthogonal $E'$ in $A^*$ is the set of linear forms on A whose restriction to E is zero. Likewise, the orthogonal $F'$ in A of a linear subspace F of $A^*$ is the intersection of the kernels of the linear forms belonging to F.

We know (II, §7, No. 5, p. 299, Theorem 7) that the mapping $\varphi : E\mapsto E'$ is a bijection from the set of linear subspaces of A of finite codimension to the set of linear subspaces of $A^*$ of finite dimension. The inverse mapping $\varphi^{-1}$ sends a finite-dimensional subspace F of $A^*$ to its orthogonal $F'$ in A.

#### Proposition 1 {#alg-viii-s20-prop-1 .statement tag=00ME}

a) The mapping $\varphi$ induces a bijection from the set of left (resp. right, two-sided) ideals of A of finite codimension to the set of right A-submodules (resp. left A-submodules, sub-bimodules) of $A^*$ of finite dimension over K.

b) Every left or right ideal of A of finite codimension contains a two-sided ideal of finite codimension.

Formulas (3) and (4) prove that if E is a left ideal of A, then $E'$ is a right A-submodule of $A^*$; if V is a right A-submodule of $A^*$, then $V'$ is a left ideal of A. The cases of right ideals and of two-sided ideals are treated analogously. This proves a).

Let $\mathfrak{a}$ be a left ideal of A of finite codimension. The left A-module $E = A_s/\mathfrak{a}$ is finite-dimensional over K, and so is End$_K(E)$. The kernel of the homomorphism $a\mapsto a_E$ from A to End$_K(E)$ is therefore a two-sided ideal of A of finite codimension contained in $\mathfrak{a}$. Passing to the opposite ring $A^o$, we see that every right ideal of A of finite codimension contains a two-sided ideal of finite codimension.

#### Definition 2 {#alg-viii-s20-def-2 .statement tag=00MF}

The restricted dual

of the K-algebra A, denoted by Θ(A), is the union in $A^*$ of the orthogonals of the two-sided ideals of A of finite codimension.

By Proposition 1, we can give the following equivalent descriptions of Θ(A):

– the union of the orthogonals of the left ideals of A of finite codimension

– the union of the orthogonals of the right ideals of A of finite codimension – the union of the orthogonals of the two-sided ideals of A of finite codimension – the union of the left A-submodules of $A^*$ of finite dimension over K

– the union of the right A-submodules of $A^*$ of finite dimension over K

– the union of the $(A$, A)-sub-bimodules of $A^*$ of finite dimension over K.

We have $\Theta (A) = \Theta (A^o)$, and $\Theta (A) = A^*$ if A has finite degree over K. Let $f\in A^*$; then $f$ belongs to Θ(A) if and only if $Af$ (resp. $fA, AfA)$ is a linear subspace of $A^*$ of finite dimension over K.

The sum of two $(A$, A)-sub-bimodules of $A^*$ of finite dimension over K has finite dimension over K. It follows that Θ(A) is an $(A$, A)-sub-bimodule of $A^*$.

### 3. Coefficients of a Module

Let E be a left A-module. Let $E^*$ be the dual of the vector space E over K; we endow it with its natural right A-module structure. Given elements $x$ of E and $x^*$ of $E^*$, we denote by $c_E(x, x^*)$ the linear form

$$
c_E(x, x^*) :a\mapsto  \langle x^*, ax\rangle \tag{5}
$$

on A. These linear forms are called the coefficients of E. The subspace of $A^*$ generated by the coefficients of E is denoted by $\Theta_E(A)$. It is nonzero if E is nonzero.

If F is an A-module isomorphic to E, then E and F have the same coefficients and we have $\Theta_F(A) = \Theta_E(A)$. Let us view $E^*$ as a left $A^o$-module; a coefficient of E is a coefficient of $E^*$, and $\Theta_E(A)\subset \Theta_{E^*}(A^o)$. Consequently, if E is finite-dimensional over K, then E and $E^*$ have the same coefficients, and we have $\Theta_E(A) = \Theta_{E^*}(A^o)$.

Let $(M, \pi )$ be a linear representation of the algebra A. The coefficients of the A-module $M_{\pi}$ are also called the coefficients of the representation $\pi$. The coefficient $c_{M_{\pi}}(x, x^*)$, for $x\in M$ and $x^*\in M^*$, is also denoted by $c_{\pi}(x, x^*)$; the vector space $\Theta_{M_{\pi}}(A)$ is also denoted by $\Theta_{\pi}(A)$.

#### Remark 1 {#alg-viii-s20-n3-rem-1 .statement tag=00MG}

Suppose that M is finite-dimensional over K. Let $(e_1, . . . , e_n)$ be a basis of V, and let $(e^*_1, . . . , e^*_n)$ be its dual basis. Denote by $(\pi_{ij}(a))$ the matrix of $\pi (a)$ with respect to the basis $(e_1, . . . , e_n)$ of V; we have $\pi_{ij}=$ $c_{\pi}(e_j, e^*_i)$. The mapping $a\mapsto (\pi_{ij}(a))$ is a homomorphism from A to $\mathbf{M}_n(K)$; such a homomorphism is sometimes called a matrix representation of the algebra A.

#### Remark 2 {#alg-viii-s20-n3-rem-2 .statement tag=00MH}

Let E be an A-module, and let $E'$ be a submodule of E. By the corollary of Theorem 5 of II, §7, No. 5, p. 299, we have $\Theta_{E'}(A)\subset \Theta_E(A)$ and $\Theta_{E/E'}(A)\subset \Theta_E(A)$.

Let $\gamma_E$ be the unique K-linear mapping from $E\otimes_KE^*$ to $A^*$ that sends $x\otimes x^*$ to $c_E(x, x^*)$. It is $(A$, A)-bilinear, and its image is $\Theta_E(A)$. We deduce from it A-linear mappings $c'_E: E\rightarrow$ Hom$_A(E^*,A^*)$ and $c''_E: E^*\rightarrow$ Hom$_A(E,A^*)$ such that

$$
c'_E(x)(x^*) =c_E(x, x^*) =c''_E(x^*)(x)
$$

Denote by $\theta_E$ the K-linear mapping $\theta_E: E\otimes E^*\rightarrow$ End$_K(E)$ characterized by the relation

$$
\theta_E(x\otimes x^*)(y) =\langle x^*, y\rangle x
$$

for $x, y\in E$ and $x^*\in E^*$. Its image is the set End$^f_K(E)$ of endomorphisms of E of finite rank (VIII, p. 463). By the definition of the trace (loc. cit.), we have

Tr($\theta_E(x\otimes x^*)$) $=\langle x^*, x\rangle$

for $x\in E$ and $x^*\in E^*$; we therefore have

$\langle \gamma_E(x\otimes x^*), a\rangle =\langle x^*, ax\rangle =$ Tr($\theta_E(ax\otimes x^*)$) $=$ Tr($\theta_E(x\otimes x^*)a$).

This gives the relation

$\langle \gamma_E(h), a\rangle =$ Tr($\theta_E(h)\circ a_E$)

for $a\in A$ and $h\in E\otimes_KE^*$. This proves that $\Theta_E(A)$ is the set of linear forms $a\mapsto$ Tr($u\circ a_E$) on A, where $u$ runs through End$^f_K(E)$.

#### Lemma 1 {#alg-viii-s20-lem-1 .statement tag=00MI}

The mapping $c''_E$ is bijective. If E is finite-dimensional, then so is $c'_E$.

When F is a right A-module and G is a K-vector space, we defined in II, §4, No. 1, p. 268, Proposition 1, a) an isomorphism $\gamma$ of K-vector spaces from Hom$_K(F\otimes_AE,G)$ to Hom$_A(E$, Hom$_K(F,G))$. This isomorphism sends $\varphi : F\otimes_AE\rightarrow G$ to the homomorphism $e\mapsto (f\mapsto \varphi (f\otimes e))$. Through the canonical isomorphism from $A_d\otimes_AE$ to E (II, §3, No. 4, p. $249),\gamma$ can be identified with $c''_E$ when $F = A_d$ and G = K.

Analogously, the isomorphism $\beta$ defined in II, §4, No. 1, p. 268, Proposition 1, b) specializes to an isomorphism $\beta$ from Hom$_K(E^*\otimes_AA_s,K)$ to Hom$_A(E^*$, Hom$_K(A_s,K))$. When E is finite-dimensional, E can be canonically identified with Hom$_K(E^*,K)$ and $E^*$ with $E^*\otimes_AA_s$; the homomorphism $\beta$ is then identified with $c'_E$.

#### Proposition 2 {#alg-viii-s20-prop-2 .statement tag=00MJ}

Let E be a left A-module.

a) The set of coefficients of E is the union of the images of the A-linear mappings from E to $A^*$.

b) Suppose, moreover, that E has finite dimension $n$ over K. Then the left A-module $\Theta_E(A)$ is isomorphic to a quotient of $E^n$, the A-module E is isomorphic to a submodule of $\Theta_E(A)^n$, and every element of $\Theta_E(A)$ is a coefficient of $E^n$.

Assertion a) follows from the surjectivity of $c''_E$.

Let us prove b). Let $(e^*_1, . . . , e^*_n)$ be a basis of $E^*$ over K. Since $\Theta_E(A)$ is generated by the coefficients of E, the A-linear mapping

$$
(x_1, . . . , x_n)\mapsto \sum_{i=1}^nc_E(x_i, e^*_i)
$$

from $E^n$ to $\Theta_E(A)$ is surjective. By a), every element of $\Theta_E(A)$ is a coefficient of $E^n$. Moreover, the A-linear mapping

$$
x\mapsto (c_E(x, e^*_1), . . . , c_E(x, e^*_n))
$$

from E to $\Theta_E(A)^n$ is injective; this gives b).

#### Remark 3 {#alg-viii-s20-n3-rem-3 .statement tag=00MK}

Let E be a left A-submodule of $A^*$. Let $\varepsilon$ be the linear form $y\mapsto y(1)$ on E. For every $x$ in E, we have $x=c_E(x, \varepsilon )$, so E is an A-submodule of $\Theta_E(A)$.

### 4. Restricted Dual and Matrix Coefficients

#### Proposition 3 {#alg-viii-s20-prop-3 .statement tag=00ML}

Let $(V, \pi )$ be a finite-dimensional linear representation of the algebra A. The kernel $\mathfrak{a}$ of $\pi$ is a two-sided ideal of A of finite codimension, and $\Theta_{\pi}(A)$ is the orthogonal of $\mathfrak{a}$ in $A^*$. The transpose of the mapping $\pi$ defines an isomorphism from the dual of the K-vector space $\pi (A)$ to $\Theta_{\pi}(A)$.

Since End$_K(V)$ is finite-dimensional over $K,\mathfrak{a}$ is a two-sided ideal of A of finite codimension. The vector space $\Theta_{\pi}(A)$ is a finite-dimensional subspace of $A^*$, and its orthogonal in A is equal to $\mathfrak{a}$; by Theorem 7 of II, §7, No. 5, p. 301, the space $\Theta_{\pi}(A)$ is therefore the orthogonal of $\mathfrak{a}$ in $A^*$. Moreover, since $\mathfrak{a}$ is the kernel of $\pi$, the transpose of the mapping $\pi$ defines an isomorphism from the dual of $\pi (A)$ to the orthogonal of $\mathfrak{a}$ in $A^*$ (II, §7, No. 5, p. 299, Corollary of Theorem 5).

#### Corollary {#alg-viii-s20-n4-cor-1 .statement tag=00MM}

The restricted dual Θ(A) of A is the set of coefficients of the finite-dimensional linear representations of A.

By definition, Θ(A) is the union of the orthogonals of the two-sided ideals of A of finite codimension. We therefore have $\Theta_{\pi}(A)\subset \Theta (A)$ for every finite-dimensional linear representation $\pi$ of A. Conversely, let $f$ be an element of Θ(A), and let $\mathfrak{a}$ be a two-sided ideal of finite codimension, contained in the kernel of $f$ (VIII, p. 376, Definition 2). Denote by $\pi$ the linear representation of A in $A/\mathfrak{a}$ deduced from the left regular representation in A by passing to the quotient. Let $x$ be the class of 1 (mod $\mathfrak{a})$, and let $x^*$ be the linear form on $A/\mathfrak{a}$ deduced from $f$. We have $f=c_{\pi}(x, x^*)$, so that $f$ is a coefficient of $\pi$.

Take note that if $(V, \pi )$ is a linear representation of A that is not finite-dimensional over K, then the space $\Theta_{\pi}(A)$ is not necessarily contained in Θ(A).

### 5. Dual of a Semisimple Algebra

Let $\Theta^{ss}(A)$ be the socle of the left A-module Θ(A), that is, (VIII, p. 65) the largest semisimple submodule of Θ(A). We denote by $\mathscr{S}_K$ the set of classes of simple (left) A-modules that are finite-dimensional over K. When A is a semisimple algebra of finite degree over K, we have $A^*= \Theta (A) = \Theta^{ss}(A)$ because every left A-module is semisimple (VIII, p. 138, Proposition 4).

#### Theorem 1 {#alg-viii-s20-thm-1 .statement tag=00MN}

a) The set $\Theta^{ss}(A)$ consists of the coefficients of the finite-dimensional semisimple representations of A. It is an $(A,A)$-sub-bimodule of $A^*$.

b) For every $S\in \mathscr{S}_K$, the isotypical component of Θ(A) of type S is equal to $\Theta_S(A)$. The left A-module $\Theta^{ss}(A)$ is the direct sum of the submodules $\Theta_S(A)$, where S runs through $\mathscr{S}_K$.

c) For every S in $\mathscr{S}_K$, the right A-module $S^*$ is simple, and $\Theta_S(A)$ is the isotypical component of type $S^*$ of the right A-module Θ(A). The mapping that sends S to cl(S$^*)$ is a bijection from $\mathscr{S}_K$ to the set of classes of simple $A^o$-modules of finite dimension over K.

d) Viewed as a right A-module, Θ(A) has socle $\Theta^{ss}(A)$.

Let E be a semisimple A-module of finite dimension over K. Every coefficient of E belongs to the image of an A-linear mapping from E to $A^*$ (VIII, p. 378, Proposition 2) and therefore belongs to $\Theta^{ss}(A)$. Conversely, let $f\in \Theta^{ss}(A)$. Then the A-module $Af$ is finite-dimensional over K and is semisimple. By the remark in VIII, p. 367$,f$ is a coefficient of $Af$.

For every S in $\mathscr{S}_K$, the isotypical component of Θ(A) of type S is generated by the images of the A-linear mappings from S to $A^*$; it is therefore equal to $\Theta_S(A)$ by Proposition 2, a) of VIII, p. 378. On the other hand, if S is a simple A-module that is not finite-dimensional over K, then the isotypical component of Θ(A) of type S is zero: indeed, every simple submodule of Θ(A) is monogenous and therefore finite-dimensional over K. Since the socle of Θ(A) is the direct sum of its isotypical components (VIII, p. 65, Proposition 4), this proves b).

Let S be a simple A-module of finite dimension over K. Since the K-vector space S is not reduced to 0, the same holds for $S^*$. Let E be a submodule of the right A-module $S^*$; its orthogonal $E'$ in S is an A-submodule of S. Since S is simple, we have either $E'= 0$, in which case $E = S^*$, or $E'= S$, in which case E = 0. Hence $S^*$ is a simple right A-module.

We have $\Theta (A^o) = \Theta (A)$ (VIII, p. 376); we identify right A-modules with left $A^o$-modules. Since every vector space of finite dimension over K is isomorphic to its bidual, the above proves that the mapping $S\mapsto$ cl(S$^*)$ is a bijection from $\mathscr{S}_K$ to the set of classes of simple $A^o$-modules of finite dimension over K. Now, for S in $\mathscr{S}_K$, the isotypical component of $\Theta (A^o)$ of type $S^*$ is equal to $\Theta_{S^*}(A^o)$ by assertion b) applied to the algebra $A^o$, and we have $\Theta_{S^*}(A^o) = \Theta_S(A)$. Assertions c) and d) follow immediately.

#### Corollary 1 {#alg-viii-s20-thm-1-cor-1 .statement tag=00MO}

Every simple A-module of finite dimension over K is isomorphic to an A-submodule of Θ(A).

This follows from Theorem 1, b) because we have $\Theta_E(A)\not= 0$ for every nonzero A-module E.

#### Corollary 2 {#alg-viii-s20-thm-1-cor-2 .statement tag=00MP}

If two simple A-modules of finite dimension over K have a common nonzero coefficient, then they are isomorphic.

Let $S_1$ and $S_2$ be simple A-modules of finite dimension over K with a common nonzero coefficient. We then have $\Theta_{S_1}(A)\cap \Theta_{S_2}(A)\not= 0$. Now, $\Theta_{S_1}(A)$ is isotypical of type $S_1$, and $\Theta_{S_2}(A)$ is isotypical of type $S_2$. So $S_1$ is isomorphic to $S_2$.

By Theorem 1, $\Theta^{ss}(A)$ is an $(A$, A)-sub-bimodule of $A^*$, the direct sum of the $(A$, A)-bimodules $\Theta_S(A)$ for S running through $\mathscr{S}_K$. These bimodules are pairwise nonisomorphic because they are already nonisomorphic as left A-modules.

Fix an S in $\mathscr{S}_K$. Denote by D the opposite field of End$_A$(S), and view S as a right D-module and $S^*$ as a left D-module. With these conventions, S is an $(A$, D)-bimodule, $S^*$ is a $(D$, A)-bimodule, and $S\otimes_DS^*$ is an $(A$, A)-bimodule.

#### Proposition 4 {#alg-viii-s20-prop-4 .statement tag=00MQ}

a) There exists a group homomorphism $\lambda_S$ from $S\otimes_DS^*$ to $\Theta_S(A)$, characterized by

$$
\lambda_S(x\otimes x^*) =c_S(x, x^*) \tag{6}
$$

for $x\in S$ and $x^*\in S^*$. This mapping is an isomorphism of $(A,A)$-bimodules.

b) The $(A,A)$-bimodule $\Theta_S(A)$ is simple.

The mapping $\gamma_S: S\otimes_KS^*\rightarrow \Theta_S(A)$ characterized by the formula $\gamma_S(x\otimes x^*) =c_S(x, x^*)$ is $(A$, A)-linear and surjective and satisfies $\gamma_S(xd\otimes x^*)$ $=\gamma_S(x\otimes dx^*)$ for $x\in S,x^*\in S^*$, and $d\in D$. It therefore defines a surjective $(A$, A)-linear mapping $\lambda_S: S\otimes_DS^*\rightarrow \Theta_S(A)$ characterized by formula (6).

Let us prove that $S\otimes_DS^*$ is a simple $(A$, A)-bimodule. By Corollary 2 of VIII, p. 63, every $(A$, A)-sub-bimodule of $S\otimes_DS^*$ is of the form $S\otimes_DH$, where H is a $(D$, A)-sub-bimodule of $S^*$. Since $S^*$ is a simple right A-module (VIII, p. 380, Theorem 1, c)), we have H = 0 or $H = S^*$; the assertion follows.

The homomorphism $\lambda_S$ is $(A$, A)-linear and nonzero; since $S\otimes_DS^*$ is a simple bimodule, $\lambda_S$ is injective (VIII, p. 47, Proposition 2, a)).

#### Remark {#alg-viii-s20-n5-rem-1 .statement tag=00MR}

When the field K is algebraically closed, we have D = K by Theorem 1 of VIII, p. 47, and $\lambda_S$ is an isomorphism of $(A$, A)-bimodules from $S\otimes_KS^*$ to $\Theta_S(A)$.

### 6. Character of a Representation

Let E be a left A-module of finite dimension over K. The character of E or trace of E, denoted by Tr$_E$, is the linear form $a\mapsto$ Tr($a_E$). Let $(e_1, . . . , e_n)$ be a basis of E and $(e^*_1, . . . , e^*_n)$ its dual basis. By definition, we have the relation

(7) Tr$_E=\sum_{i=1}^nc_E(e_i, e^*_i)$.

The linear form Tr$_E$ belongs to $\Theta_E(A)$. We have Tr$_E=$ Tr$_{E'}$ if E and $E'$ are two isomorphic A-modules. So Tr$_E$ depends only on the isomorphism class of E.

Let $\pi$ be a linear representation of A in a vector space V of finite dimension over K. The trace of $\pi$, or sometimes character of $\pi$, is defined as the character of the A-module $V_{\pi}$. We denote it by Tr$_{\pi}$. If $(e_1, . . . , e_n)$ is a basis of V over K and if $(\pi_{ij}(a))$ is the matrix of $\pi (a)$ with respect to this basis, then we have

(8) Tr$_{\pi}(a) =\sum_{i=1}^n\pi_{ii}(a)$.

The linear form Tr$_{\pi}$ belongs to $\Theta_{\pi}(A)$.

#### Proposition 5 {#alg-viii-s20-prop-5 .statement tag=00MS}

Let S be a simple A-module of finite dimension over K, let D be the opposite field of the commutant of S, and let Z be the center of D. The following properties are equivalent:

(i) The character Tr$_S$ of S is not zero.

(ii) There exists an element $d\in D$ such that Tr$_{D/K}(d)\not= 0$.

(iii) The extension Z of K is separable, and the characteristic $p$ of K does not divide the degree [D : Z].

The right D-vector space S is finite-dimensional. Let $(e_1, . . . , e_n)$ be a basis of S over D, and let $u$ be an element of End$_D(S)$. Let $(d_{ij})$ be the matrix of $u$ with respect to the basis $(e_1, . . . , e_n)$. We have $u(e_j) =\sum^n_{i=1}e_id_{ij}$ for $j\in [1, n]$. Denote by $u_K$ the mapping $u$ viewed as an endomorphism of the K-vector space S and by $(u_{ij})$ the matrix of $u_K$ with respect to the decomposition $(e_iD)$ of the K-vector space S as a direct sum (II, §10, No. 5, p. 346). We have Tr($u_K$) $=\sum_i$ Tr($u_{ii}$). Moreover, $u_{ii}$ is the endomorphism of the K-vector space $e_iD$ defined by $u_{ii}(e_id) =e_id_{ii}d$ for $d\in D$, so its trace is equal to Tr$_{D/K}(d_{ii})$. We have thus proved the equality

(9) Tr($u_K$) $=$ Tr$_{D/K}(\sum_id_{ii})$.

By Burnside’s theorem (VIII, p. 83, Corollary 1 of Proposition 4), the mapping $a\mapsto a_S$ from A to End$_D(S)$ is surjective. The equivalence of properties (i) and (ii) therefore follows from formula (9).

If the extension Z of K is separable, then there exists an element $d\in Z$ such that Tr$_{Z/K}(d)\not= 0$ (V, §8, No. 2, p. 49, Corollary of Proposition 1). Moreover, we have Tr$_{D/K}(d) = [D : Z]$ Tr$_{Z/K}(d)$ (III, §9, No. 4, p. 548, Corollary); consequently, if $p$ does not divide [D : Z], then we have Tr$_{D/K}(d)\not=$ 0. This proves that (iii) implies (ii).

If the extension Z of K is not separable, then we have Tr$_{Z/K}(x) = 0$ for every $x\in Z$, and therefore Tr$_{D/K}(d) =$ Tr$_{Z/K}$(Tr$_{D/Z}(d)) = 0$ for every $d\in D$.

Now suppose that $p$ divides the degree [D : Z]. It then divides the reduced degree of D over Z. For every $d\in D$, we have Tr$_{D/Z}(d) = 0$ (VIII, p. 344, Remark), and therefore Tr$_{D/K}(d) =$ Tr$_{Z/K}$(Tr$_{D/Z}(d)) = 0$. This completes the proof of the implication (ii) $\Rightarrow$ (iii).

#### Corollary {#alg-viii-s20-n6-cor-1 .statement tag=00MT}

If the field K is perfect, then properties (i) through (iii) hold.

Since the field is perfect, the extension Z of K is separable (V, §15, No. 5, p. 125, Theorem 3). Property (iii) then follows from Corollary 3 of VIII, p. 323.

#### Proposition 6 {#alg-viii-s20-prop-6 .statement tag=00MU}

Let $\mathscr{S}_0$ be the set of classes of simple A-modules of finite dimension over K with nonzero trace. The family of linear forms (Tr$_S)_{S\in\mathscr{S}_0}$ is free over K.

Let F be a finite subset of $\mathscr{S}_0$, and let S be an element of F. By assumption, there exists an element $a\in A$ such that Tr$_S(a)\not= 0$. By Corollary 1 of Proposition 4 (VIII, p. 83), there exists an element $b\in A$ such that $b_S=a_S$ and $b_T= 0$ for every $T\in F-\{S\}$. We have Tr$_S(b)\not= 0$ and Tr$_T(b) = 0$ for $T\in F-\{S\}$. The family (Tr$_S)_{S\in F}$ is therefore free. Proposition 6 follows.

#### Remark {#alg-viii-s20-n6-rem-1 .statement tag=00RR}

Let $\mathscr{S}_K$ be the set of classes of simple A-modules of finite dimension over K. Proposition 6 also follows from the fact that the sum of the $\Theta_S$(A), for S running through $\mathscr{S}_K$, is direct.

Let

$$
0\longrightarrow E'\longrightarrow E\longrightarrow E''\longrightarrow 0
$$

be an exact sequence of A-modules, all finite-dimensional over K. By Proposition 1 of III, §9, No. 2, p. 543, we have Tr$_E=$ Tr$_{E'}+$ Tr$_{E''}$. By the definition of the Grothendieck group $R_K(A)$ (VIII, p. 194) and its universal property (VIII, p. 186, Proposition 4), there exists a homomorphism of additive groups $\theta$ from $R_K(A)$ to $A^*$ characterized by the relation $\theta ([E]) =$ Tr$_E$ for every A-module E of finite dimension over K. In particular, the trace of a semisimplification of E is equal to that of E. We deduce from $\theta$ a K-linear mapping $\theta_K: K\otimes_{\mathbf{Z}}R_K(A)\rightarrow A^*$.

#### Corollary {#alg-viii-s20-n6-cor-2 .statement tag=00MV}

a) Suppose that the field K has characteristic 0. The homomorphisms $\theta$ and $\theta_K$ are injective. Two semisimple A-modules of finite dimension over K are isomorphic if and only if their characters are equal.

b) Suppose that the field K is perfect of nonzero characteristic $p$. Then the homomorphism $\theta_K$ is injective, and the kernel of $\theta$ is $pR_K(A)$. Let E be a semisimple A-module of finite dimension over K. The linear form Tr$_E$ is zero if and only if there exists an A-module F such that E is isomorphic to $F^p$.

Let $\mathscr{S}_K$ be the set of classes of simple A-modules of finite dimension over K. The elements [S], where S runs through $\mathscr{S}_K$, form a basis of the $\mathbf{Z}$-module $R_K$(A), so the elements $1\otimes [S]$ form a basis of the K-vector space $K\otimes_{\mathbf{Z}}R_K(A)$ (VIII, p. 195).

Suppose that the field K is perfect. By Proposition 6 and the corollary of VIII, p. 383, the elements $\theta ([S]) =\theta_K(1\otimes [S]) =$ Tr$_S$ of $A^*$ are linearly independent over K. It follows that the homomorphism $\theta_K$ is injective and that the kernel of the homomorphism $\theta$ consists of the elements $\sum_{S\in\mathscr{S}_K}n_S[S]$ of $R_K(A)$ such that $n_S\cdot 1_K= 0$ for every $S\in \mathscr{S}_K$. The kernel of $\theta$ is therefore equal to $pR_K$(A), where $p$ is the characteristic of K. In particular, if K has characteristic 0, then the homomorphism $\theta$ is injective.

The last assertion of a) follows from the corollary of VIII, p. 190.

Suppose that the assumptions of b) are satisfied, and let E be a semisimple A-module of finite dimension over K. If there exists an A-module F such that E is the direct sum of $p$ submodules isomorphic to F, then the module F is semisimple and finite-dimensional over K and we have Tr$_E=p$ Tr$_F= 0$. Conversely, suppose Tr$_E= 0$. We have $[E]\in pR_K$(A), so the multiplicity of every simple module $S\in \mathscr{S}_K$ in E is a multiple of $p$ (VIII, p. 190, Proposition 7); we can write it as $p n_S$ with $n_S\in \mathbf{N}$. The family $(n_S)$ has finite support. Set $F =\oplus_{S\in\mathscr{S}_K}S^{n_S}$. We then have $[E] = [F^p]$, so that E and $F^p$ are isomorphic (VIII, p. 190, Corollary).

Let E be an A-module of finite dimension over K. Let $a\in A$. Denote by $\chi_E(a; T)$ the determinant of the endomorphism $1_E+ Ta_E$ of the K[T]-module $E[T] = K[T]\otimes_KE$ (III, §8, No. 11, p. 541). We have the relation

(10) $\chi_E(a; T)\equiv 1 +$ Tr$_E(a)T$ (mod $T^2K[T])$

(loc. cit., formula (49)). Since this polynomial has constant term equal to 1, it is an invertible formal power series (IV, §4, No. 4, p. 30). Moreover, if

$$
0\longrightarrow E'\longrightarrow E\longrightarrow E''\longrightarrow 0
$$

is an exact sequence of A-modules, all finite-dimensional over K, then we have $\chi_E(a; T) =\chi_{E'}(a; T)\chi_{E''}(a,T)$ (III, §8, No. 7, p. 534, formula (31)). By the definition of the Grothendieck group $R_K(A)$ (VIII, p. 194) and its universal property (VIII, p. 186, Proposition 4), there exists a unique homomorphism $\chi_a$ from the group $R_K(A)$ to the multiplicative group 1 + TK[[T]] such that $\chi_a([E]) =\chi_E(a; T)$ for every A-module E of finite dimension over K. We deduce from formula (10) the relation

(11) $\chi_a(x)\equiv 1 +\theta (x)(a)T$ (mod $T^2K[[T]])$

for $x\in R_K(A)$ and $a\in A$.

If E and $E'$ are two A-modules of finite dimension over K with isomorphic semisimplifications, then we have $\chi_E(a; T) =\chi_{E'}(a; T)$.

#### Theorem 2 {#alg-viii-s20-thm-2 .statement tag=00MW}

Let $\mathscr{A}$ be a generating subset of the K-vector space A. The homomorphism $\chi_{\mathscr{A}}: R_K(A)\rightarrow$ (1 + TK[[T]])$^{\mathscr{A}}$ defined by the relation $\chi_{\mathscr{A}}(x) = (\chi_a(x))_{a\in\mathscr{A}}$ is injective.

Let $x$ be an element of $R_K(A)$ such that $\chi_{\mathscr{A}}(x) = 1$. By (11), we have $\theta (x)(a) = 0$ for every $a\in \mathscr{A}$, and therefore $\theta (x) = 0$ because $\theta (x)$ is a K-linear form on A and $\mathscr{A}$ generates the K-vector space A. If the characteristic of K is zero, then this implies $x= 0$ (VIII, p. 384, Corollary of Proposition 6), and therefore the result in this case. Suppose from now on that the characteristic $p$ of K is nonzero.

Let us first treat the case when K is algebraically closed. By the above and loc. cit., we then have $x\in pR_K(A)$. Let $y\in R_K(A)$ be such that $x=py$. For every element $a$ of $\mathscr{A}$, we have $\chi_a(y)^p=\chi_a(py) =\chi_a(x) = 1$. So we have $(\chi_a(y)-1)^p= 0$, and therefore $\chi_a(y) = 1$ because the ring K[[T]] is an integral domain. So $y$ belongs to the kernel of the endomorphism $\chi_{\mathscr{A}}$. It follows by induction that $x$ belongs to $p^nR_K(A)$ for every integer $n\geqslant 1$. Since $R_K(A)$ is a free $\mathbf{Z}$-module, this implies $x= 0$, and therefore the injectivity of $\chi_{\mathscr{A}}$ in this case.

If K is no longer supposed to be algebraically closed, then we choose an algebraic closure K of K and consider the diagram of groups and group homomorphisms

$R_K(A)^{\chi_{\mathscr{A}}}$ // (1 + TK[[T]])$_{\mathscr{A}}$

$$
ui \tag{12}
$$

$R_{\overline{K}}(A_{(K)})^{\overline{\chi}_{\mathscr{A}}}$ // (1 + TK[[T]])$_{\mathscr{A}}$,

where $u$ is the homomorphism deduced from the extension of scalars from K to K (VIII, p. 195$),i$ is the canonical injection, and $\overline{\chi}_{\mathscr{A}}$ is the homomorphism $z\mapsto (\chi_{1\otimes a}(z))_{a\in\mathscr{A}}$. By formula (12) of III, §9, No. 1, p. 542, diagram (12) is commutative. By the above, the homomorphism $\overline{\chi}_{\mathscr{A}}$ is injective. Since $u$ is injective (VIII, p. 195, Theorem 1), the homomorphism $\chi_{\mathscr{A}}$ is injective.

#### Corollary 1 {#alg-viii-s20-thm-2-cor-1 .statement tag=00MX}

Let E and F be semisimple A-modules of finite dimension over K, and let $\mathscr{A}$ be a generating subset of the K-vector space A. Suppose that for every $a\in \mathscr{A}$, the characteristic polynomials of the endomorphisms $a_E$ and $a_F$ of the K-vector spaces E and F are equal. Then the A-modules E and F are isomorphic.

Let $a$ be an element of $\mathscr{A}$. The characteristic polynomials of $a_E$ and $a_F$ have the same degree, so the dimension of E is equal to that of F; we denote it by $n$. Let Pc$_E(a; T)$ be the characteristic polynomial of $a_E$. In K(T), we have the equalities

$\chi_E(a; T) =$ det$(1 +a_ET)= (-T)^n$ det$(\frac{-1}{T}-a_E)= (-T)^n$ Pc$_E(a;\frac{-1}{T})$,

and $\chi_F(a; T)$ is given by an analogous formula. Because of our assumptions, we have $\chi_E(a; T) =\chi_F(a; T)$. By Theorem 2, we have [E] = [F], which implies that E and F are isomorphic (VIII, p. 190, Corollary of Proposition 7).

#### Corollary 2 {#alg-viii-s20-thm-2-cor-2 .statement tag=00MY}

Let A be a central simple algebra of finite degree over K. Let B be a semisimple K-algebra, let $f$ and $g$ be algebra homomorphisms from B to A, and let $\mathscr{B}$ be a generating subset of the K-vector space B. The following properties are equivalent:

(i) There exists an inner automorphism $\theta$ of A such that $g=\theta \circ f$.

(ii) For every $b\in \mathscr{B}$, we have Pc$_{A/K}(f(b); X) =$ Pc$_{A/K}(g(b); X)$. When K has characteristic zero, these properties are equivalent to the following:

(iii) For every $b\in \mathscr{B}$, we have Tr$_{A/K}(f(b)) =$ Tr$_{A/K}(g(b))$.

Denote by M and N the left B-modules obtained by endowing the additive group of A with the external laws $(b, a)\mapsto f(b)a$ and $(b, a)\mapsto g(b)a$, respectively. By Proposition 1 of VIII, p. 257, property (i) is equivalent to the fact that the B-modules M and N are isomorphic. By construction, the homothety $b_M$ associated with an element $b$ of B is left multiplication by $f(b)$ in A; consequently, we have the relations

Pc$_M(b; X) =$ Pc$_{A/K}(f(b); X)$,

Tr$_M(b) =$ Tr$_{A/K}(f(b))$

and two analogous relations where we replace M with N and $f$ with $g$. We know (VIII, p. 386, Corollary 1) that the B-modules M and N are isomorphic if and only if we have Pc$_M(b; X) =$ Pc$_N(b; X)$ for every $b\in \mathscr{B}$. When the field K has characteristic 0, this relation is also equivalent to Tr$_M(b) =$ Tr$_N(b)$ for every $b\in \mathscr{B}$ (VIII, p. 384, Corollary of Proposition 6). The equivalence of properties (i) and (ii), and also of (i) and (iii) when K has characteristic 0, follows.

### 7. Coefficients of a Set of Classes of Modules

Let $\mathscr{C}$ be a hereditary set of classes of A-modules (VIII, p. 183, Definition 1). We suppose that every A-module of type $\mathscr{C}$ is finite-dimensional over K and denote by $\Theta_{\mathscr{C}}(A)$ the set of coefficients of the A-modules of type $\mathscr{C}$. By Proposition 2 of VIII, p. 378, the set $\Theta_{\mathscr{C}}(A)$ is also the union of the images of the A-linear mappings $u: E\rightarrow A^*$, where E runs through $\mathscr{C}$; it is also the union of the subspaces $\Theta_E(A)$ of $A^*$, where E runs through $\mathscr{C}$ (loc. cit.). The family of $(A$, A)-sub-bimodules $(\Theta_E(A))_{E\in\mathscr{C}}$ of $A^*$ is directed, so its union $\Theta_{\mathscr{C}}(A)$ is an $(A$, A)-sub-bimodule of $A^*$.

#### Proposition 7 {#alg-viii-s20-prop-7 .statement tag=00MZ}

A left A-submodule of $A^*$ of finite dimension over K is contained in $\Theta_{\mathscr{C}}(A)$ if and only if it is of type $\mathscr{C}$.

Let V be a left A-submodule of $A^*$ of finite dimension over K. We saw in VIII, p. 379, Remark 3 that we have $V\subset \Theta_V(A)$. If V is of type $\mathscr{C}$, then we have $\Theta_V(A)\subset \Theta_{\mathscr{C}}$ (A), so V is contained in $\Theta_{\mathscr{C}}(A)$. Conversely, suppose that V is contained in $\Theta_{\mathscr{C}}(A)$. Since $\Theta_{\mathscr{C}}(A)$ is the union of the directed family $(\Theta_E(A))_{E\in\mathscr{C}}$ and V is finite-dimensional over K, there exists a module E of type $\mathscr{C}$ such that V is contained in $\Theta_E(A)$. Now, there exists a natural number $n$ such that $\Theta_E(A)$ is isomorphic to a quotient of $E^n$ (VIII, p. 378, Proposition 2). Since $\mathscr{C}$ is hereditary, V is of type $\mathscr{C}$.

#### Corollary {#alg-viii-s20-n7-cor-1 .statement tag=00N0}

Let E be an A-module of finite dimension over K. Then E is of type $\mathscr{C}$ if and only if $\Theta_E(A)$ is contained in $\Theta_{\mathscr{C}}(A)$.

The condition is obviously necessary.

Conversely, suppose that $\Theta_{\mathscr{C}}(A)$ contains $\Theta_E(A)$. The A-module $\Theta_E(A)$ is finite-dimensional over K (VIII, p. 378, Proposition 2), so it is of type $\mathscr{C}$ by Proposition 7. Now, there exists an integer $n\geqslant 0$ such that E is isomorphic to an A-submodule of $\Theta_E(A)^n$ (VIII, p. 378, Proposition 2). Since $\mathscr{C}$ is hereditary, E is of type $\mathscr{C}$.

### 8. Cogebra Structure on the Restricted Dual

For any $a$ in A, we denote by $\eta (a)$ the linear form $f\mapsto f(a)$ on Θ(A). We thus define a K-linear mapping $\eta$ from A to the dual $\Theta (A)^*$ of the vector space Θ(A). Set $\varepsilon =\eta (1)$.

#### Proposition 8 {#alg-viii-s20-prop-8 .statement tag=00N1}

On the vector space Θ(A), there exists a unique cogebra structure (III, §11, No. 1, p. 574) such that the mapping $\eta : A\rightarrow \Theta (A)^*$ is a homomorphism from A to the dual algebra (III, §11, No. 2, p. 579) of Θ(A). The cogebra Θ(A) is coassociative and admits $\varepsilon$ as a counit.

For every integer $n\geqslant 1$, consider the K-linear mapping $j_n$ from $\Theta (A)^{\otimes n}$ to the dual of $A^{\otimes n}$ characterized by the formula

$$
\langle j_n(f_1\otimes  \cdots  \otimes f_n), a_1\otimes  \cdots  \otimes a_n\rangle =\prod_{i=1}^n\langle f_i, a_i\rangle \tag{13}
$$

for $(a_i)$ in $A^n$ and $(f_i)$ in $\Theta (A)^n$. By Proposition 16, (ii) of II, §7, No. 7, p. 308, the mapping $j_n$ is injective. Denote by $m_K: K\otimes K\rightarrow K$ and $m_A: A\otimes A\rightarrow A$ the mappings deduced from the multiplication in K and A, respectively. For $f, g\in \Theta (A)$ and $a, b\in A$, we have

$$
\langle j_2(f\otimes g), a\otimes b\rangle =m_K\circ (\eta (a)\otimes \eta (b))(f\otimes g)
$$

We therefore have

$$
\langle j_2(t), a\otimes b\rangle =m_K\circ (\eta (a)\otimes \eta (b))(t) \tag{14}
$$

for every $t\in \Theta (A)\otimes \Theta (A)$.

#### Lemma 2 {#alg-viii-s20-lem-2 .statement tag=00RS}

Let $c: \Theta (A)\rightarrow \Theta (A)\otimes \Theta (A)$ be a K-linear mapping. Then $\eta$ is a homomorphism from A to the dual algebra of the cogebra $(\Theta (A), c)$ if and only if the following diagram commutes:

Θ(A) $^c$ // $\Theta (A)\otimes \Theta (A)$

$$
j_{_1}j_{_2} \tag{15}
$$

$A_{*^t}^{m_A}$ // $(A\otimes A)_*$.

Indeed, $\eta$ is a homomorphism from A to the dual algebra of the cogebra $(\Theta (A), c)$ if and only if we have $\eta (ab) =m_K\circ (\eta (a)\otimes \eta (b))\circ c$ for all $a, b\in A$, that is

$$
\eta (ab)(f) =m_K\circ (\eta (a)\otimes \eta (b))(c(f))
$$

for $a, b\in A$ and $f\in \Theta (A)$. Now, we have

$$
\eta (ab)(f) =f(ab) =\langle^tm_A(j_1(f)), a\otimes b\rangle
$$

and, by (14),

$$
m_K\circ (\eta (a)\otimes \eta (b))(c(f)) =\langle j_2(c(f)), a\otimes b\rangle
$$

for all $a, b\in A$ and every $f\in \Theta (A)$. The lemma follows.

Since $j_2$ is injective, there exists at most one linear mapping $c$ that makes the diagram above commute. To prove its existence, we must prove that the image of $^tm\circ j_1$ is contained in that of $j_2$. In other words, we must prove that there exist, for every element $f$ of Θ(A), a natural number $n$ and elements $f'_1, . . . , f'_n, f''_1, . . . , f''_n$ of Θ(A) satisfying the relations

$$
f(ab) =\sum_{i=1}^nf'_i(a)f''_i(b) \tag{16}
$$

for $a, b\in A$. We will then have

$$
c(f) =\sum_{i=1}^nf'_i\otimes f''_i \tag{17}
$$

By the corollary of VIII, p. 379, there exists a left A-module E of finite dimension over K with $f$ as a coefficient. Let $(e_1, . . . , e_n)$ be a basis of E, $(e^*_1, . . . , e^*_n)$ the dual basis, $x$ an element of E, and $x^*$ an element of $E^*$ such that $f=c_E(x, x^*)$. Set $f'_i=c_E(e_i, x^*)$ and $f''_i=c_E(x, e^*_i)$ for $i\in [1, n]$; for $a, b$ in A, we have

$$
f(ab) =\langle x^*, abx\rangle =\langle x^*a, bx\rangle =\langle\sum_i\langle x^*a, e_i\rangle e^*_i, bx\rangle
$$

$$
=\sum_i\langle x^*a, e_i\rangle \langle e^*_i, bx\rangle =\sum_i\langle x^*, ae_i\rangle \langle e^*_i, bx\rangle =\sum_if'_i(a)f''_i(b)
$$

and therefore (16).

Let us prove the coassociativity of $c$. For this, consider the K-linear mappings

$c'=(c\otimes 1_{\Theta (A)})\circ c$ and $c''=(1_{\Theta (A)}\otimes c)\circ c$

from Θ(A) to $\Theta (A)^{\otimes 3}$. We have the relations

$$
\langle j_3(f\otimes c(g)), a\otimes b\otimes c\rangle =\langle f, a\rangle \langle j_2\circ c(g), b\otimes c\rangle
$$

$$
=\langle f, a\rangle \langle g, bc\rangle
$$

$$
=\langle j_2(f\otimes g), a\otimes bc\rangle
$$

$=\langle^t$(Id$_A\otimes m_A)\circ j_2(f\otimes g), a\otimes b\otimes c\rangle$

for $f, g\in \Theta (A)$ and $a, b, c\in A$. From this, we deduce that the following diagram commutes:

$\Theta (A)\otimes \Theta (A)^{Id_{\Theta (A)}\otimes c}/$/ $\Theta (A)\otimes \Theta (A)\otimes \Theta (A)$

(18)

$j_2j_3$

$(A\otimes A)_{*^t}^{(Id_A\otimes m_A)}$ // $(A\otimes A\otimes A)_*$.

Because of the commutativity of this diagram and that of (15), for $f\in \Theta (A)$ and $a,a',a''\in A$, we have

$$
\langle j_3\circ c'(f), a\otimes a'\otimes a''\rangle =\langle f,(aa')a''\rangle
$$

we can show the relation

$$
\langle j_3\circ c''(f), a\otimes a'\otimes a''\rangle =\langle f, a(a'a'')\rangle
$$

likewise. Since multiplication in A is associative, we have $j_3\circ c'=j_3\circ c''$, and therefore $c'=c''$ because $j_3$ is injective.

Finally, formulas (16) and (17) imply that Θ(A) admits $\varepsilon$ as a counit.

#### Remark 1 {#alg-viii-s20-n8-rem-1 .statement tag=00N2}

Let $(V, \pi )$ be a finite-dimensional linear representation of the algebra A. Let us introduce a basis $(e_1, . . . , e_n)$ of V and the dual basis $(e^*_1, . . . , e^*_n)$ of $V^*$. By the proof of Lemma 2, we have the relation

$$
c(c_{\pi}(x, x^*)) =\sum_{k=1}^nc_{\pi}(e_k, x^*)\otimes c_{\pi}(x, e^*_k) \tag{19}
$$

for $x\in V$ and $x^*\in V^*$. For $1\leqslant i, j\leqslant n$, set $\pi_{ij}=c_{\pi}(e_j, e^*_i)$. For every $a\in A$, the matrix of $\pi (a)$ with respect to the basis $(e_1, . . . , e_n)$ of V is equal to $(\pi_{ij}(a))$. For $1\leqslant i\leqslant n$ and $1\leqslant j\leqslant n$, we then have

$$
c(\pi_{ij}) =\sum_{k=1}^n\pi_{ik}\otimes \pi_{kj} \tag{20}
$$

#### Definition 3 {#alg-viii-s20-def-3 .statement tag=00N3}

Let C be a cogebra over the field K and $c$ its coproduct. A subcogebra of C is any linear subspace $C_1$ of C such that $c(C_1)$ is contained in the canonical image of $C_1\otimes_KC_1$ in $C\otimes_KC$.

Let $j$ be the canonical injection of $C_1$ into C. By this definition, there exists a unique linear mapping $c_1: C_1\rightarrow C_1\otimes_KC_1$ such that we have

$$
c\circ j= (j\otimes j)\circ c_1 \tag{21}
$$

this relation means that $j$ is a morphism of cogebras from $(C_1, c_1)$ to $(C, c)$ (III, §11, No. 1, p. 574).

If C is coassociative, then $C_1$ is coassociative. If C is cocommutative, then so is $C_1$. If C has a counit $\varepsilon$, then the restriction of $\varepsilon$ to $C_1$ is a counit of $C_1$.

#### Proposition 9 {#alg-viii-s20-prop-9 .statement tag=00N4}

Let Θ be a linear subspace of Θ(A). The following properties are equivalent:

(i) Θ is an $(A,A)$-sub-bimodule of Θ(A).

(ii) Θ is a subcogebra of Θ(A).

(iii) There exists a hereditary set $\mathscr{C}$ of classes of A-modules of finite dimension over K such that $\Theta  = \Theta_{\mathscr{C}}(A)$.

When these properties hold, the set $\mathscr{C}$ mentioned in (iii) is uniquely determined.

The last assertion follows from the corollary of VIII, p. 388: the set $\mathscr{C}$ consists of the classes of A-modules E of finite dimension over K such that $\Theta_E(A)$ is contained in Θ.

(iii) $\Rightarrow$ (ii): Let $\mathscr{C}$ be a hereditary set of classes of A-modules of finite dimension over K. Then $\Theta_{\mathscr{C}}(A)$ is the union of the directed family $(\Theta_E(A))_{E\in\mathscr{C}}$. Since $\Theta_E(A)$ is a subcogebra of Θ(A) for every $E\in \mathscr{C}$ (VIII, p. 390, formula (19)), the same holds for $\Theta_{\mathscr{C}}(A)$.

(ii) $\Rightarrow$ (i): Let $f\in \Theta (A)$. Let $f'_1, . . . , f'_n, f''_1, . . . , f''_n$ be elements of Θ(A) satisfying $c(f) =\sum f'_i\otimes f''_i$. For $a,b$ in A, we have $f(ab) =\sum f'_i(a)f''_i(b)$, and therefore

$$
bf=\sum_{i=1}^nf''_i(b)f'_i,f a=\sum_{i=1}^nf'_i(a)f''_i
$$

(VIII, p. 375, formulas (3) and (4)). Consequently, a subcogebra of Θ(A) is an $(A$, A)-sub-bimodule.

(i) $\Rightarrow$ (iii): Suppose that Θ is an $(A$, A)-sub-bimodule of Θ(A); let $\mathscr{C}$ be the set of classes of A-modules E of finite dimension over K such that $\Theta_E(A)$ is contained in Θ. The set $\mathscr{C}$ is hereditary (VIII, p. 377, Remark 2), and we have $\Theta_{\mathscr{C}}(A)\subset \Theta$ by construction. Let $f\in \Theta$ and $E = Af$. Then E is finite-dimensional over K. Consequently, every linear form on E is of the form $u_a:g\mapsto g(a)$ with $a$ in A (II, §7, No. 5, p. 302, Corollary 2). Now, for $a, b, x\in A$, we have

$$
c_E(af, u_b)(x) =\langle u_b, xaf\rangle =f(bxa) =af b(x)
$$

so that $c_E(af, u_b) =af b$. We therefore have $\Theta_E(A)\subset \Theta$. Consequently, the A-module E is of type $\mathscr{C}$, and $f$ is one of its coefficients. We therefore have $\Theta \subset \Theta_{\mathscr{C}}(A)$ and, finally, $\Theta  = \Theta_{\mathscr{C}}(A)$.

#### Remark 2 {#alg-viii-s20-n8-rem-2 .statement tag=00N5}

Let Θ be a subcogebra of Θ(A). We endow K with the discrete topology and the algebra A with the coarsest topology for which the mappings $f: A\rightarrow K$ for $f$ running through Θ are continuous (Gen. Top., I, §2, No. 2, p. 175). This topology endows A with the structure of a topological K-module. A two-sided ideal $\mathfrak{a}$ of A is open if and only if it has finite codimension and its orthogonal $\mathfrak{a}'$ is contained in Θ. By Proposition 3 of VIII, p. 379, the open two-sided ideals of A form a fundamental system of neighborhoods of 0 in A. The topology on A is therefore compatible with its ring structure.

Let $\mathscr{C}$ be the hereditary set of classes of A-modules of finite dimension over K such that $\Theta  = \Theta_{\mathscr{C}}$ (VIII, p. 391, Proposition 9). Let E be a left A-module of finite dimension over K. We endow it with the discrete topology. The following properties are equivalent:

(i) The A-module E is of type $\mathscr{C}$.

(ii) The annihilator of the A-module E is open in A.

(iii) The mapping $(a, x)\mapsto ax$ from $A\times E$ to E is continuous.

The last property means that E is a topological A-module.

Let $\Theta^*$ be the dual algebra of the cogebra Θ. We endow $\Theta^*$ with the coarsest topology for which the mappings $\varphi \mapsto \varphi (u)$ from $\Theta^*$ to K, for $u$ running through Θ, are continuous. The topology on the algebra $\Theta^*$ is compatible with the additive group structure on $\Theta^*$. The orthogonals in $\Theta^*$ of the sets of the form $\Theta_E$(A), where E is an A-module of type $\mathscr{C}$, form a fundamental system of neighborhoods of 0. Now, such a set is a subcogebra of Θ, so its orthogonal is an ideal of $\Theta^*$. The topology on $\Theta^*$ is therefore compatible with its ring structure. The canonical algebra homomorphism $\eta : A\rightarrow \Theta^*$ (that sends $a\in A$ to the linear form $f\mapsto f(a)$ on Θ) defines an isomorphism from the completed Hausdorff space $\widehat{A}$ of A (Gen. Top., II, §3, No. 7, p. 191) to $\Theta^*$.

### Exercises {#alg-viii-s20-exercises}

See the [exercises for § 20](exercises/s20/).
