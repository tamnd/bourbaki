---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 7
section_title: Simple Rings
lang: en
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.119-A VIII.133
pdf_pages: 0136-0150
extraction: native
subsections:
    - "no": 1
      title: Simple Rings
      page: 119
      pdf_page: 136
    - "no": 2
      title: Modules over a Simple Ring
      page: 122
      pdf_page: 139
    - "no": 3
      title: Degrees
      page: 124
      pdf_page: 141
    - "no": 4
      title: Ideals of Simple Rings
      page: 126
      pdf_page: 143
statements: 24
exercises: 16
content_sha256: 13a105e1ae4a8f7b21014f593edf1d71da3a94fc4158a3550efe2776d02521b0
---

## § 7. SIMPLE RINGS

### 1. Simple Rings

#### Proposition 1 {#alg-viii-s7-prop-1 .statement tag=0081}

Let A be a nonzero ring. The following conditions are equivalent:

(i) The A-module $A_s$ is isotypical.

(ii) The ring A is left Artinian, and every two-sided ideal of A is equal to 0 or A.

(iii) The ring A is left Artinian, and there exists a left A-module S that is simple and faithful.

If these conditions are satisfied, then the A-module $A_s$ has finite length and is isotypical of type S, and every simple A-module is isomorphic to S.

Let us prove that (i) implies (ii). Assume that (i) is satisfied. Then the finitely generated A-module $A_s$ is semisimple, hence has finite length and is Artinian (VIII, p. 71, Proposition 10); consequently, the ring A is left Artinian. The endomorphisms of the left A-module $A_s$ are the right multiplications by the elements of A. Since the left A-module $A_s$ is isotypical, it follows from Proposition 6, b) of VIII, p. 86 that the $(A$, A)-bimodule $_sA_d$ is simple. The sub-bimodules of $_sA_d$ are the two-sided ideals of A, so (i) implies (ii).

Let us prove that (ii) implies (iii). The ring A is not reduced to 0; consequently, there exists a simple A-module S. The annihilator of S is a proper two-sided ideal of A. If we assume that (ii) is satisfied, then that annihilator is equal to 0. The A-module S is then faithful, and (ii) implies (iii).

Let us prove that (iii) implies (i). Assume that (iii) is satisfied. Then there exists an integer $m\geqslant 1$ such that $A_s$ is isomorphic to a submodule of $S^m$ (VIII, p. 50, Proposition 5, a)). Since $S^m$ is an isotypical A-module of type S, the same holds for $A_s$ (VIII, p. 61, Proposition 2); hence, (iii) implies (i).

Suppose that conditions (i) through (iii) are satisfied. We have seen above that the A-module $A_s$ has finite length and is isotypical of type S. Every simple left A-module is isomorphic to a quotient of $A_s$, hence to S.

#### Definition 1 {#alg-viii-s7-def-1 .statement tag=0082}

We say that a ring A is simple if it satisfies the equivalent conditions (i), (ii), and (iii) of Proposition 1. Let K be a commutative field; a K-algebra is called simple if its underlying ring is simple.

#### Remark 1 {#alg-viii-s7-n1-rem-1 .statement tag=0083}

Recall that by Theorem 1 of II, §9, No. 1, p. 115, the following properties are equivalent:

(i) The A-module $A_s$ is simple.

(ii) The ring A is not reduced to 0, and there are no left ideals of A distinct from 0 or A.

(iii) The ring A is a field.

Consequently, by Proposition 1 (condition (ii)), commutative simple rings are nothing but commutative fields.

#### Remark 2 {#alg-viii-s7-n1-rem-2 .statement tag=0084}

We sometimes say that a ring A is quasi-simple if it is not reduced to 0 and if its only two-sided ideals are 0 and A. We say that A is primitive if it admits a faithful simple module. By Proposition 1, every simple ring is quasi-simple. Since every nonzero ring admits a simple module and the annihilator of a simple module is a two-sided ideal, we see that every quasi-simple ring is primitive. However, there exist quasi-simple rings that are not simple and primitive rings that are not quasi-simple (VIII, p. 128, Exercise 2); such rings are not left Artinian.

#### Theorem 1 (Wedderburn) {#alg-viii-s7-thm-1 .statement tag=00S3}

A ring is simple if and only if it is isomorphic to a matrix ring $\mathbf{M}_r(D)$, where $r\geqslant 1$ is an integer and D a field.

#### Lemma 1 {#alg-viii-s7-lem-1 .statement tag=0085}

Let A be a simple ring, S a simple left A-module, and D the opposite ring of the field End$_A(S)$. Then S is an invertible $(A,D)$-bimodule. It is also a finite-dimensional right vector space over D, and the mapping $a\mapsto a_S$ is a ring isomorphism from A to End$_D(S)$.

By Proposition 1, the A-module $A_s$ has finite length and is isotypical of type S. Hence, there exists an integer $m\geqslant 1$ such that the A-modules $A_s$ and $S^m$ are isomorphic. Then the A-module S is projective and finitely generated. It is generating (VIII, p. 80, Theorem 1), and Lemma 1 follows from Theorem 1 of VIII, p. 101, (ii)$\Rightarrow$(i) and (ii)$\Rightarrow$(iii) applied to the $(A,D)_{\mathbf{Z}}$-bimodule S.

#### Lemma 2 {#alg-viii-s7-lem-2 .statement tag=00R7}

Let D be a field and V a right vector space of finite dimension $r\geqslant 1$ over D. Then V is a simple module over the ring E = End$_D(V)$, and its commutant is equal to $D_V$. The ring E is simple, and its left length is equal to $r$.

We know that V is a simple E-module (VIII, p. 45, Example 3) and that its commutant is equal to $D_V$ (VIII, p. 82, Corollary 1). Let $(x_i)_{1\leqslant i\leqslant r}$ be a basis of V over the field D. The mapping $u\mapsto (u(x_i))_{1\leqslant i\leqslant r}$ is an isomorphism from the E-module $E_s$ to the E-module $V^r$; consequently, the E-module $E_s$ is isotypical of length $r$, so the ring E is simple.

Let us now prove Theorem 1. Recall (II, §10, No. 7, p. 349) that the ring $\mathbf{M}_r(D)$ can be identified with the endomorphism ring of the right D-vector space $D^r_d$; moreover, every right vector space of finite dimension $r$ over a field D is isomorphic to $D^r_d$ (II, §7, No. 1, p. 292). Theorem 1 therefore follows from Lemmas 1 and 2.

#### Remark 3 {#alg-viii-s7-n1-rem-3 .statement tag=0086}

Let A be a simple ring, S a simple A-module, and D the opposite ring of the field End$_A(S)$. Then the A-module $A_s$ has finite length, and dim$_D(S)$ is equal to long(A). Indeed, by Lemma 1, the ring A is isomorphic to End$_D(S)$; we then apply Lemma 2.

#### Corollary 1 {#alg-viii-s7-lem-2-cor-1 .statement tag=0087}

a) The center of a simple ring is a field.

b) The opposite ring of a simple ring is simple.

c) The left length of a simple ring is equal to its right length.

Let D be a field, Z its center, and V a right vector space over D of finite dimension $r\geqslant 1$. We denote the endomorphism ring of V by E.

The mapping $z\mapsto z_V$ is an isomorphism from Z to the center of E by Corollary 2 of VIII, p. 83. Assertion a) follows. The dual $V^*$ of V is a right vector space over the opposite field $D^o$ of D, and its dimension is equal to $r$. The mapping $u\mapsto^tu$ is an isomorphism from the opposite ring $E^o$ of E to the ring End$_{D^o}(V^*)$. Consequently, the ring $E^o$ is simple, and the rings E and $E^o$ have the same left length, equal to $r$ (Lemma 2).

#### Corollary 2 {#alg-viii-s7-lem-2-cor-2 .statement tag=0088}

Let $r$ and $r'$ be strictly positive integers, and let D and $D'$ be fields. The rings $\mathbf{M}_r(D)$ and $\mathbf{M}_{r'}(D')$ are isomorphic if and only if we have $r=r'$ and the fields D and $D'$ are isomorphic.

The condition is obviously sufficient.

Conversely, suppose that the rings $B =\mathbf{M}_r(D)$ and $B'=\mathbf{M}_{r'}(D')$ are isomorphic. Since $r$ is the length of $B_s$ and $r'$ that of $B'_s$ (Lemma 2), we have $r=r'$. Moreover, B is Morita equivalent to D and $B'$ to $D'$ (VIII, p. 102, Example 1). Consequently, the fields D and $D'$ are Morita equivalent, hence isomorphic (VIII, p. 111, Proposition 13, c)).

#### Corollary 3 {#alg-viii-s7-lem-2-cor-3 .statement tag=0089}

Let K be a commutative field, and let A be a K-algebra of finite degree with simple underlying ring. There exist an integer $r$ and a K-algebra D of finite degree over K that is a field such that A is isomorphic to $M_r(D)$. In particular, if K is algebraically closed, then A is isomorphic to a matrix algebra over K.

Let S be a simple left A-module; it is a finite-dimensional K-vector space over K. Its commutant is therefore an algebra of finite degree over K. The first assertion then follows from Lemma 1. If K is algebraically closed, then D = K by Theorem 1 of VIII, p. 47.

#### Remark 4 {#alg-viii-s7-n1-rem-4 .statement tag=008A}

Let K be an algebraically closed commutative field, and let A be an algebra of finite degree over K. The algebra A is simple if and only if there exists an integer $n\geqslant 1$ such that A is isomorphic to $M_n(K)$. Its center is then isomorphic to K.

### 2. Modules over a Simple Ring

#### Lemma 3 {#alg-viii-s7-lem-3 .statement tag=008B}

Let A be a simple ring, and let S be a simple A-module. Denote the opposite field of the commutant of S by D. Every A-module is isomorphic to an A-module of the form $S\otimes_DV$, where V is a left vector space over the field D.

This follows from Lemma 1 of VIII, p. 120 and Morita’s theorem (VIII, p. 103).

#### Proposition 2 {#alg-viii-s7-prop-2 .statement tag=008C}

Let A be a simple ring and S a simple A-module.

a) Every A-module is projective and isotypical of type S, hence semisimple. If it has length $\mathfrak{a}$, then it is isomorphic to $S^{(\mathfrak{a})}$.

b) Every nonzero A-module is generating.

c) Two A-modules are isomorphic if and only if they have the same length.

Denote the opposite field of the commutant of S by D. By Lemma 1 of VIII, p. 120, S is an invertible $(A$, D)-bimodule. Let M be an A-module; by Lemma 3, it is isomorphic to a module of the form $S\otimes_DV$, where V is a left vector space over the field D.

The D-module V is projective and isotypical of type $D_s$; it is generating if and only if it is not reduced to 0. Finally, the length of $S\otimes_DV$ is equal to the dimension of the D-vector space V, and two vector spaces are isomorphic if and only if they have the same dimension. Proposition 2 now follows in view of Propositions 10 of VIII, p. 109 and 12 of VIII, p. 110.

Let $r\geqslant 1$ be an integer. We say that a cardinal $\mathfrak{a}$ is divisible by $r$ if there exists a cardinal $\mathfrak{b}$ such that $\mathfrak{a}=r\mathfrak{b}$. This is the case if $\mathfrak{a}$ is infinite because we have $r\mathfrak{a}=\mathfrak{a}($Set Theory, III, §6, No. 3, p. 188, Corollary 3). It follows from this remark that if the cardinal $\mathfrak{a}$ is divisible by $r$, then there exists a unique cardinal $\mathfrak{b}$ such that $\mathfrak{a}=r\mathfrak{b}$.

#### Corollary {#alg-viii-s7-n2-cor-1 .statement tag=008D}

Let $k$ be a commutative field, and let A be a simple $k$-algebra of finite degree over $k$. Every simple A-module is finite-dimensional over $k$. Two A-modules are isomorphic if and only if their dimensions over $k$ are equal.

Every simple A-module is isomorphic to a quotient of $A_s$, hence finite-dimensional over $k$. The corollary then follows from Proposition 2, c).

#### Proposition 3 {#alg-viii-s7-prop-3 .statement tag=008E}

Let A be a simple ring. An A-module M is free if and only if its length is divisible by the length of A. If that is the case, then all bases of M have the same cardinal, denoted by dim$_A(M)$ (II, §7, No. 3, p. 294, Remark 2) and determined by the relation

(1) long$_A(M) =$ long(A) $\cdot$ dim$_A(M)$.

Suppose that M is free, and let $(e_i)_{i\in I}$ be a basis of M. The A-module M is the direct sum of the A-modules $Ae_i$, which are each isomorphic to $A_s$. Set $r=$ long$_A(A_s)$; this is an integer greater than or equal to 1 (VIII, p. 119, Proposition 1). We have long$_A(M) =r$ Card(I) by formula (13) of VIII, p. 73.

Conversely, suppose that the cardinal long$_A(M)$ is divisible by $r$. Let $\mathfrak{a}$ be the cardinal such that long$_A(M) =r\mathfrak{a}$. Then the A-module M has the same length as $A^{(\mathfrak{a})}_s$, hence is isomorphic to it by Proposition 2. This proves that M is free.

#### Proposition 4 {#alg-viii-s7-prop-4 .statement tag=008F}

Let A be a simple ring and M a nonzero A-module. Denote the endomorphism ring of the A-module M by B, and view M as a left B-module.

a) The mapping $a\mapsto a_M$ is an isomorphism from A to the endomorphism ring of the B-module M.

b) Suppose that M has finite length as an A-module. Then the ring B is simple, and we have

(2) long$_A(M) =$ long(B) and long$_B(M) =$ long(A).

The A-module M is generating by Proposition 2 of VIII, p. 122. By definition, we have $B = A'_M$, and assertion a) therefore follows from Theorem 2 of VIII, p. 82.

Suppose that M is an A-module of finite length. Choose a simple A-module S, and let D be the opposite field of the endomorphism ring of S. By Lemma 3, the A-module M is isomorphic to a module of the form $S\otimes_DV$, where V is a left vector space over the field D. The vector space V is finite-dimensional. By Theorem 3 of VIII, p. 64, the ring B is isomorphic to End$_D(V)$; by Lemma 2 (VIII, p. 121), the ring B is therefore simple. Taking Remark 1 of VIII, p. 63 into account, we obtain the equalities

long(B) = dim$_D(V) =$ long$_A(M)$.

By Remarks 1 of VIII, p. 63 and 3 of VIII, p. 121, we have the relations

long$_B(M) =$ long$_{End_D(V)}(S\otimes_DV) =$ dim$_D(S) =$ long(A),

which gives the last relation.

### 3. Degrees

Consider a ring B and a subring A of B. Endow B with the structure of an $(A$, A)-bimodule deduced by restriction of scalars from the $(B$, B)-bimodule structure on $_sB_d$.

#### Proposition 5 {#alg-viii-s7-prop-5 .statement tag=008G}

Let B be a ring, A a simple subring of B, and S a simple left A-module. Then B is a free left A-module of dimension long$_A(B\otimes_AS)$.

Let $r$ be the length of A; the A-module $A_s$ is isomorphic to $S^r$. Now, the left A-module B is isomorphic to $B\otimes_AA_s$ (II, §3, No. 4, p. 249), hence to $(B\otimes_AS)^r$ (II, §3, No. 7, p. 255, Proposition 7). We therefore have long$_A(B) =r$ long$_A(B\otimes_AS)$, and Proposition 5 follows from Proposition 3 of VIII, p. 123.

#### Definition 2 {#alg-viii-s7-def-2 .statement tag=008H}

Let B be a ring and A a simple subring of B. The dimension of the free left A-module B is called the (left) degree of B over A and is denoted by[^1] $[B : A]_s$.

By replacing A and B with the opposite rings, we deduce from the above that B is a free right A-module. We denote its dimension by $[B : A]_d$ and call it the right degree of B over A.

We can give an example of a field B and a subfield A such that the degrees $[B : A]_s$ and $[B : A]_d$ differ.[^2]

Let B be a ring, A a simple subring of B, and S a simple left A-module. Let M be a left A-module and $\mathfrak{a}$ its length. The A-modules M and $S^{(\mathfrak{a})}$ are isomorphic (VIII, p. 122, Proposition 2), hence so are the B-modules $B\otimes_AM$ and $(B\otimes_AS)^{(\mathfrak{a})}$. The relation

(3) long$_A(B\otimes_AM) = [B : A]_s$ long$_A(M)$

follows from Proposition 5 and Definition 2.

#### Proposition 6 {#alg-viii-s7-prop-6 .statement tag=008I}

Let C be a ring, B a simple subring of C, and A a simple subring of B. We then have $[C : A]_s= [C : B]_s[B : A]_s$.

Let us introduce a basis $(e_i)_{i\in I}$ of C viewed as a left B-module and a basis $(f_j)_{j\in J}$ of B viewed as a left A-module. Then the family $(f_je_i)_{j\in J,i\in I}$ is a basis of C viewed as a left A-module (II, §1, No. 13, p. 222, Proposition 25); Proposition 6 follows.

#### Remark 1 {#alg-viii-s7-n3-rem-1 .statement tag=008J}

Suppose that A is a simple subring of a simple ring B and that the right degree $[B : A]_d$ is finite. Let C be the endomorphism ring of B viewed as a right A-module; it is a simple ring by Proposition 4, b) of VIII, p. 123. For any $b$ in B, let $\gamma (b)$ be the mapping $x\mapsto bx$ from B to B; then $\gamma :b\mapsto \gamma (b)$ is an isomorphism from B to a subring of C. Moreover, if $(x_1, . . . , x_m)$ is a basis of the right A-module B, then the morphism that sends $c$ to $(c(x_1), . . . , c(x_m))$ is an isomorphism of left B-modules from C to $B^m_s$; consequently, we have the relation

$$
[C :\gamma (B)]_s= [B : A]_d \tag{4}
$$

Taking into account relation (2) of VIII, p. 123 applied to the right A-module B, we see that

(5) long(C) $= [B : A]_d$ long(A).

#### Remark 2 {#alg-viii-s7-n3-rem-2 .statement tag=008K}

Let K be a commutative field. If A is a simple subalgebra of an algebra B of finite degree over K, then the left degree of B over A satisfies the relation $[B : A]_s[A : K] = [B : K]$ by Proposition 6 of VIII, p. 125. Likewise, we have $[B : A]_d[A : K] = [B : K]$. The equality $[B : A]_s= [B : A]_d$ follows.

### 4. Ideals of Simple Rings

Let D be a field and V a right vector space over D of finite dimension $n\geqslant 1$. Consider the simple ring A = End$_D(V)$. For any linear subspace W of V, we denote the set of elements $a$ of A satisfying $aW = 0$ (resp. $aV\subset W)$ by $\mathfrak{a}(W)$ (resp. $\mathfrak{b}(W))$.

#### Proposition 7 {#alg-viii-s7-prop-7 .statement tag=008L}

a) The mapping $W\mapsto \mathfrak{a}(W)$ is a bijection from the set of linear subspaces of V to the set of left ideals of A.

b) The mapping $W\mapsto \mathfrak{b}(W)$ is a bijection from the set of linear subspaces of V to the set of right ideals of A.

c) Let $W_1$ and $W_2$ be linear subspaces of V. The relations $W_1\subset W_2$, $\mathfrak{a}(W_1)\supset \mathfrak{a}(W_2)$, and $\mathfrak{b}(W_1)\subset \mathfrak{b}(W_2)$ are equivalent.

Assertion b) follows from Example 1, b) of VIII, p. 104 applied to the invertible $(D^o,A^o$)-bimodule V, as does the equivalence of the relations $W_1\subset W_2$ and $\mathfrak{b}(W_1)\subset \mathfrak{b}(W_2)$.

Let $V^*$ be the dual of V, viewed as a right vector space over the opposite field $D^o$ of D. For any subspace W of V, denote the orthogonal of W in $V^*$ by $W'$. The mapping $W\mapsto W'$ is a bijection from the set of subspaces of V to the set of subspaces of $V^*$. If $W_1$ and $W_2$ are two subspaces of V, then the relations $W_1\subset W_2$ and $W'_1\supset W'_2$ are equivalent. Now, the mapping $u\mapsto^tu$ is an isomorphism from A to the opposite ring of End$_{D^o}(V^*)$; it transforms left ideals of A into right ideals of End$_{D^o}(V^*)$ and $\mathfrak{a}(W)$ into the set $\mathfrak{b}(W')$ of endomorphisms $h$ of $V^*$ such that $h(V^*)\subset W'$. Assertion a), as well as the equivalence of the relations $W_1\subset W_2$ and $\mathfrak{a}(W_1)\supset \mathfrak{a}(W_2)$, then follows from the assertion analogous to b) for the dual $V^*$ of V.

#### Corollary {#alg-viii-s7-n4-cor-1 .statement tag=008M}

a) The minimal left ideals of A are the ideals $\mathfrak{a}(H)$, where H is a hyperplane in V. The maximal left ideals of A are the ideals $\mathfrak{a}(L)$, where L is a line in V.

b) The minimal right ideals of A are the ideals $\mathfrak{b}(L)$, where L is a line in V. The maximal right ideals of A are the ideals $\mathfrak{b}(H)$, where H is a hyperplane in V.

Let $(L_i)_{i\in I}$ be a family of lines with direct sum V. Let $(\varepsilon_i)_{i\in I}$ be the family of projectors associated with the decomposition $V =\oplus_{i\in I}L_i$. The $\varepsilon_i$ are idempotent in A, and we have $\varepsilon_i\varepsilon_j= 0$ for $i\not=j$ and $\sum_{i\in I}\varepsilon_i= 1$. Denote the hyperplane $\sum_{j\not=i}L_j$ by $H_i$; it is the kernel of $\varepsilon_i$. We then have

$$
\mathfrak{a}(H_i) = A\varepsilon_i,\mathfrak{b}(L_i) =\varepsilon_iA
$$

The A-module $A_s$ is the direct sum of the family $(\mathfrak{a}(H_i))_{i\in I}$ of minimal left ideals, and $A_d$ is the direct sum of the family $(\mathfrak{b}(L_i))_{i\in I}$ of minimal right ideals.

Consider the specific case $V = D^n_d$, and identify A with the matrix ring $\mathbf{M}_n(D)$. Denote the interval $[1, n]$ in $\mathbf{N}$ by I and the canonical basis of V by $(v_i)_{i\in I}$; set $L_i=v_iD$, and denote by $E_{ij}$ the matrix units (II, §10, No. 3, p. 341). We then have $\varepsilon_i= E_{ii}$. The left ideal AE$_{ii}$ is equal to DE$_{1i}+\cdots +$ DE$_{ni}$ and consists of the matrices with all columns except the $i$-th equal to zero. The right ideal $E_{ii}A$ is equal to DE$_{i1}+\cdots +$ DE$_{in}$ and consists of the matrices with all lines except the $i$th equal to zero. We also have the relation

$$
E_{ii}A E_{jj}= E_{ii}A\cap A E_{jj}= D E_{ij}
$$

for $i$ and $j$ between 1 and $n$.

### Exercises {#alg-viii-s7-exercises}

See the [exercises for § 7](exercises/s7/).

[^1]: If A and B are commutative fields, take care not to confuse the degree that is equal to [B : A] with the separable degree of the extension B of A, defined in V, §6, No. 5, p. 31 and also denoted by $[B : A]_s$.
[^2]: cf. A. H. Schofield, Artin’s problem for skew field extensions, Math. Proc. Cambridge Philos. Soc. **97** (1985), pp. 1–6.
