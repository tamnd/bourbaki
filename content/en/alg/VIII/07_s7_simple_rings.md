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
statements: 22
exercises: 16
content_sha256: 0da21afb2047c710a88c4307d50227e4c1a9f5d69f32fc9b26289043e3c1a623
---

## § 7. SIMPLE RINGS

### 1. Simple Rings

#### Proposition 1 {#alg-viii-s7-prop-1 .statement}

Let A be a nonzero ring. The following conditions are equivalent:

(i) The A-module $A_s$ is isotypical.

(ii) The ring A is left Artinian, and every two-sided ideal of A is equal to 0 or A.

(iii) The ring A is left Artinian, and there exists a left A-module S that is simple and faithful. If these conditions are satisfied, then the A-module $A_s$ has finite length and is isotypical of type S, and every simple A-module is isomorphic to S.

Let us prove that (i) implies (ii). Assume that (i) is satisfied. Then the finitely generated A-module $A_s$ is semisimple, hence has finite length and is Artinian (VIII, p. 71, Proposition 10); consequently, the ring A is left Artinian. The endomorphisms of the left A-module $A_s$ are the right multiplications by the elements of A. Since the left A-module $A_s$ is isotypical, it follows from Proposition 6, b) of VIII, p. 86 that the $(A$, A)-bimodule $_sA_d$ is simple. The sub-bimodules of $_sA_d$ are the two-sided ideals of A, so (i) implies (ii).

Let us prove that (ii) implies (iii). The ring A is not reduced to 0; consequently, there exists a simple A-module S. The annihilator of S is a proper two-sided ideal of A. If we assume that (ii) is satisfied, then that annihilator is equal to 0. The A-module S is then faithful, and (ii) implies (iii).

Let us prove that (iii) implies (i). Assume that (iii) is satisfied. Then there exists an integer $m\geqslant 1$ such that $A_s$ is isomorphic to a submodule of $S^m$ (VIII, p. 50, Proposition 5, a)). Since $S^m$ is an isotypical A-module of type S, the same holds for $A_s$ (VIII, p. 61, Proposition 2); hence, (iii) implies (i).

Suppose that conditions (i) through (iii) are satisfied. We have seen above that the A-module $A_s$ has finite length and is isotypical of type S. Every simple left A-module is isomorphic to a quotient of $A_s$, hence to S.

#### Definition 1 {#alg-viii-s7-def-1 .statement}

We say that a ring A is simple if it satisfies the equivalent conditions (i), (ii), and (iii) of Proposition 1. Let K be a commutative field; a K-algebra is called simple if its underlying ring is simple.

#### Remark 1 {#alg-viii-s7-n1-rem-1 .statement}

Recall that by Theorem 1 of II, §9, No. 1, p. 115, the following properties are equivalent:

(i) The A-module $A_s$ is simple.

(ii) The ring A is not reduced to 0, and there are no left ideals of A distinct from 0 or A.

(iii) The ring A is a field. Consequently, by Proposition 1 (condition (ii)), commutative simple rings are nothing but commutative fields.

#### Remark 2 {#alg-viii-s7-n1-rem-2 .statement}

We sometimes say that a ring A is quasi-simple if it is not reduced to 0 and if its only two-sided ideals are 0 and A. We say that A is primitive if it admits a faithful simple module. By Proposition 1, every simple ring is quasi-simple. Since every nonzero ring admits a simple module and the annihilator of a simple module is a two-sided ideal, we see that every quasi-simple ring is primitive. However, there exist quasi-simple rings that are not simple and primitive rings that are not quasi-simple (VIII, p. 128, Exercise 2); such rings are not left Artinian.

Theorem 1 (Wedderburn). — A ring is simple if and only if it is isomorphic to a matrix ring $\mathbf{M}_r(D)$, where $r\geqslant 1$ is an integer and D a field.

#### Lemma 1 {#alg-viii-s7-lem-1 .statement}

Let A be a simple ring, S a simple left A-module, and D the opposite ring of the field End$_A(S)$. Then S is an invertible $(A,D)$-bimodule. It is also a finite-dimensional right vector space over D, and the mapping $a\mapsto a_S$ is a ring isomorphism from A to End$_D(S)$.

By Proposition 1, the A-module $A_s$ has finite length and is isotypical of type S. Hence, there exists an integer $m\geqslant 1$ such that the A-modules $A_s$ and $S^m$ are isomorphic. Then the A-module S is projective and finitely generated. It is generating (VIII, p. 80, Theorem 1), and Lemma 1 follows from Theorem 1 of VIII, p. 101, (ii)$\Rightarrow$(i) and (ii)$\Rightarrow$(iii) applied to the $(A,D)_{\mathbf{Z}}$-bimodule S. **Lemma 2.** — Let D be a field and V a right vector space of finite dimension $r\geqslant 1$ over D. Then V is a simple module over the ring E = End$_D(V)$, and its commutant is equal to $D_V$. The ring E is simple, and its left length is equal to $r$.

We know that V is a simple E-module (VIII, p. 45, Example 3) and that its commutant is equal to $D_V$ (VIII, p. 82, Corollary 1). Let $(x_i)_{1\leqslant i\leqslant r}$ be a basis of V over the field D. The mapping $u\mapsto (u(x_i))_{1\leqslant i\leqslant r}$ is an isomorphism from the E-module $E_s$ to the E-module $V^r$; consequently, the E-module $E_s$ is isotypical of length $r$, so the ring E is simple.

Let us now prove Theorem 1. Recall (II, §10, No. 7, p. 349) that the ring $\mathbf{M}_r(D)$ can be identified with the endomorphism ring of the right D-vector space $D^r_d$; moreover, every right vector space of finite dimension $r$ over a field D is isomorphic to $D^r_d$ (II, §7, No. 1, p. 292). Theorem 1 therefore follows from Lemmas 1 and 2.

#### Remark 3 {#alg-viii-s7-n1-rem-3 .statement}

Let A be a simple ring, S a simple A-module, and D the opposite ring of the field End$_A(S)$. Then the A-module $A_s$ has finite length, and dim$_D(S)$ is equal to long(A). Indeed, by Lemma 1, the ring A is isomorphic to End$_D(S)$; we then apply Lemma 2.

#### Corollary 1 {#alg-viii-s7-lem-1-cor-1 .statement}

a) The center of a simple ring is a field.

b) The opposite ring of a simple ring is simple.

c) The left length of a simple ring is equal to its right length.

Let D be a field, Z its center, and V a right vector space over D of finite dimension $r\geqslant 1$. We denote the endomorphism ring of V by E.

The mapping $z\mapsto z_V$ is an isomorphism from Z to the center of E by Corollary 2 of VIII, p. 83. Assertion a) follows. The dual $V^*$ of V is a right vector space over the opposite field $D^o$ of D, and its dimension is equal to $r$. The mapping $u\mapsto^tu$ is an isomorphism from the opposite ring $E^o$ of E to the ring End$_{D^o}(V^*)$. Consequently, the ring $E^o$ is simple, and the rings E and $E^o$ have the same left length, equal to $r$ (Lemma 2).

#### Corollary 2 {#alg-viii-s7-lem-1-cor-2 .statement}

Let $r$ and $r'$ be strictly positive integers, and let D and $D'$ be fields. The rings $\mathbf{M}_r(D)$ and $\mathbf{M}_{r'}(D')$ are isomorphic if and only if we have $r=r'$ and the fields D and $D'$ are isomorphic.

The condition is obviously sufficient.

Conversely, suppose that the rings $B =\mathbf{M}_r(D)$ and $B'=\mathbf{M}_{r'}(D')$ are isomorphic. Since $r$ is the length of $B_s$ and $r'$ that of $B'_s$ (Lemma 2), we have $r=r'$. Moreover, B is Morita equivalent to D and $B'$ to $D'$ (VIII, p. 102, Example 1). Consequently, the fields D and $D'$ are Morita equivalent, hence isomorphic (VIII, p. 111, Proposition 13, c)).

#### Corollary 3 {#alg-viii-s7-lem-1-cor-3 .statement}

Let K be a commutative field, and let A be a K-algebra of finite degree with simple underlying ring. There exist an integer $r$ and a K-algebra D of finite degree over K that is a field such that A is isomorphic to $M_r(D)$. In particular, if K is algebraically closed, then A is isomorphic to a matrix algebra over K.

Let S be a simple left A-module; it is a finite-dimensional K-vector space over K. Its commutant is therefore an algebra of finite degree over K. The first assertion then follows from Lemma 1. If K is algebraically closed, then D = K by Theorem 1 of VIII, p. 47.

#### Remark 4 {#alg-viii-s7-n1-rem-4 .statement}

Let K be an algebraically closed commutative field, and let A be an algebra of finite degree over K. The algebra A is simple if and only if there exists an integer $n\geqslant 1$ such that A is isomorphic to $M_n(K)$. Its center is then isomorphic to K.

### 2. Modules over a Simple Ring

#### Lemma 3 {#alg-viii-s7-lem-3 .statement}

Let A be a simple ring, and let S be a simple A-module. Denote the opposite field of the commutant of S by D. Every A-module is isomorphic to an A-module of the form $S\otimes_DV$, where V is a left vector space over the field D.

This follows from Lemma 1 of VIII, p. 120 and Morita’s theorem (VIII, p. 103).

#### Proposition 2 {#alg-viii-s7-prop-2 .statement}

Let A be a simple ring and S a simple A-module.

a) Every A-module is projective and isotypical of type S, hence semisimple. If it has length $\mathfrak{a}$, then it is isomorphic to $S^{(\mathfrak{a})}$.

b) Every nonzero A-module is generating.

c) Two A-modules are isomorphic if and only if they have the same length.

Denote the opposite field of the commutant of S by D. By Lemma 1 of VIII, p. 120, S is an invertible $(A$, D)-bimodule. Let M be an A-module; by Lemma 3, it is isomorphic to a module of the form $S\otimes_DV$, where V is a left vector space over the field D.

The D-module V is projective and isotypical of type $D_s$; it is generating if and only if it is not reduced to 0. Finally, the length of $S\otimes_DV$ is equal to the dimension of the D-vector space V, and two vector spaces are isomorphic if and only if they have the same dimension. Proposition 2 now follows in view of Propositions 10 of VIII, p. 109 and 12 of VIII, p. 110.

Let $r\geqslant 1$ be an integer. We say that a cardinal $\mathfrak{a}$ is divisible by $r$ if there exists a cardinal $\mathfrak{b}$ such that $\mathfrak{a}=r\mathfrak{b}$. This is the case if $\mathfrak{a}$ is infinite because we have $r\mathfrak{a}=\mathfrak{a}($Set Theory, III, §6, No. 3, p. 188, Corollary 3). It follows from this remark that if the cardinal $\mathfrak{a}$ is divisible by $r$, then there exists a unique cardinal $\mathfrak{b}$ such that $\mathfrak{a}=r\mathfrak{b}$.

#### Corollary {#alg-viii-s7-n2-cor-1 .statement}

Let $k$ be a commutative field, and let A be a simple $k$-algebra of finite degree over $k$. Every simple A-module is finite-dimensional over $k$. Two A-modules are isomorphic if and only if their dimensions over $k$ are equal.

Every simple A-module is isomorphic to a quotient of $A_s$, hence finite-dimensional over $k$. The corollary then follows from Proposition 2, c).

#### Proposition 3 {#alg-viii-s7-prop-3 .statement}

Let A be a simple ring. An A-module M is free if and only if its length is divisible by the length of A. If that is the case, then all bases of M have the same cardinal, denoted by dim$_A(M)$ (II, §7, No. 3, p. 294, Remark 2) and determined by the relation

(1) long$_A(M) =$ long(A) $\cdot$ dim$_A(M)$.

Suppose that M is free, and let $(e_i)_{i\in I}$ be a basis of M. The A-module M is the direct sum of the A-modules $Ae_i$, which are each isomorphic to $A_s$. Set $r=$ long$_A(A_s)$; this is an integer greater than or equal to 1 (VIII, p. 119, Proposition 1). We have long$_A(M) =r$ Card(I) by formula (13) of VIII, p. 73.

Conversely, suppose that the cardinal long$_A(M)$ is divisible by $r$. Let $\mathfrak{a}$ be the cardinal such that long$_A(M) =r\mathfrak{a}$. Then the A-module M has the same length as $A^(_s^{\mathfrak{a})}$, hence is isomorphic to it by Proposition 2. This proves that M is free.

#### Proposition 4 {#alg-viii-s7-prop-4 .statement}

Let A be a simple ring and M a nonzero A-module. Denote the endomorphism ring of the A-module M by B, and view M as a left B-module.

a) The mapping $a\mapsto a_M$ is an isomorphism from A to the endomorphism ring of the B-module M.

b) Suppose that M has finite length as an A-module. Then the ring B is simple, and we have

(2) long$_A(M) =$ long(B) and long$_B(M) =$ long(A) $$.

The A-module M is generating by Proposition 2 of VIII, p. 122. By definition, we have $B = A'_M$, and assertion a) therefore follows from Theorem 2 of VIII, p. 82.

Suppose that M is an A-module of finite length. Choose a simple A-module S, and let D be the opposite field of the endomorphism ring of S. By Lemma 3, the A-module M is isomorphic to a module of the form $S\otimes_DV$, where V is a left vector space over the field D. The vector space V is finite-dimensional. By Theorem 3 of VIII, p. 64, the ring B is isomorphic to End$_D(V)$; by Lemma 2 (VIII, p. 121), the ring B is therefore simple. Taking Remark 1 of VIII, p. 63 into account, we obtain the equalities

long(B) = dim$_D(V) =$ long$_A(M)$.

By Remarks 1 of VIII, p. 63 and 3 of VIII, p. 121, we have the relations

long$_B(M) =$ long$_{End_D(V)}(S\otimes_DV) =$ dim$_D(S) =$ long(A) $$,

which gives the last relation.

### 3. Degrees

Consider a ring B and a subring A of B. Endow B with the structure of an $(A$, A)-bimodule deduced by restriction of scalars from the $(B$, B)-bimodule structure on $_sB_d$.

#### Proposition 5 {#alg-viii-s7-prop-5 .statement}

Let B be a ring, A a simple subring of B, and S a simple left A-module. Then B is a free left A-module of dimension long$_A(B\otimes_AS)$.

Let $r$ be the length of A; the A-module $A_s$ is isomorphic to $S^r$. Now, the left A-module B is isomorphic to $B\otimes_AA_s$ (II, §3, No. 4, p. 249), hence to $(B\otimes_AS)^r$ (II, §3, No. 7, p. 255, Proposition 7). We therefore have long$_A(B) =r$ long$_A(B\otimes_AS)$, and Proposition 5 follows from Proposition 3 of VIII, p. 123.

#### Definition 2 {#alg-viii-s7-def-2 .statement}

Let B be a ring and A a simple subring of B. The dimension of the free left A-module B is called the (left) degree of B over A and is denoted by[^1] $[B : A]_s$.

By replacing A and B with the opposite rings, we deduce from the above that B is a free right A-module. We denote its dimension by $[B : A]_d$ and call it the right degree of B over A.

We can give an example of a field B and a subfield A such that the degrees $[B : A]_s$ and $[B : A]_d$ differ.[^2]

Let B be a ring, A a simple subring of B, and S a simple left A-module. Let M be a left A-module and $\mathfrak{a}$ its length. The A-modules M and $S^{(\mathfrak{a})}$ are isomorphic (VIII, p. 122, Proposition 2), hence so are the B-modules $B\otimes_AM$ and $(B\otimes_AS)^{(\mathfrak{a})}$. The relation

(3) long$_A(B\otimes_AM) = [B : A]_s$ long$_A(M)$

follows from Proposition 5 and Definition 2.

#### Proposition 6 {#alg-viii-s7-prop-6 .statement}

Let C be a ring, B a simple subring of C, and A a simple subring of B. We then have $[C : A]_s= [C : B]_s[B : A]_s$.

Let us introduce a basis $(e_i)_{i\in I}$ of C viewed as a left B-module and a basis $(f_j)_{j\in J}$ of B viewed as a left A-module. Then the family $(f_je_i)_{j\in J,i\in I}$ is a basis of C viewed as a left A-module (II, §1, No. 13, p. 222, Proposition 25); Proposition 6 follows.

#### Remark 1 {#alg-viii-s7-n3-rem-1 .statement}

Suppose that A is a simple subring of a simple ring B and that the right degree $[B : A]_d$ is finite. Let C be the endomorphism ring of B viewed as a right A-module; it is a simple ring by Proposition 4, b) of VIII, p. 123. For any $b$ in B, let $\gamma (b)$ be the mapping $x\mapsto bx$ from B to B; then $\gamma :b\mapsto \gamma (b)$ is an isomorphism from B to a subring of C. Moreover, if $(x_1, . . . , x_m)$ is a basis of the right A-module B, then the morphism that sends $c$ to $(c(x_1), . . . , c(x_m))$ is an isomorphism of left B-modules from C to $B^m_s$; consequently, we have the relation

$$
[C :\gamma (B)]_s= [B : A]_d \tag{4}
$$

Taking into account relation (2) of VIII, p. 123 applied to the right A-module B, we see that

(5) long(C) $= [B : A]_d$ long(A) $$.

#### Remark 2 {#alg-viii-s7-n3-rem-2 .statement}

Let K be a commutative field. If A is a simple subalgebra of an algebra B of finite degree over K, then the left degree of B over A satisfies the relation $[B : A]_s[A : K] = [B : K]$ by Proposition 6 of VIII, p. 125. Likewise, we have $[B : A]_d[A : K] = [B : K]$. The equality $[B : A]_s= [B : A]_d$ follows.

### 4. Ideals of Simple Rings

Let D be a field and V a right vector space over D of finite dimension $n\geqslant 1$. Consider the simple ring A = End$_D(V)$. For any linear subspace W of V, we denote the set of elements $a$ of A satisfying $aW = 0$ (resp. $aV\subset W)$ by $\mathfrak{a}(W)$ (resp. $\mathfrak{b}(W))$.

#### Proposition 7 {#alg-viii-s7-prop-7 .statement}

a) The mapping $W\mapsto \mathfrak{a}(W)$ is a bijection from the set of linear subspaces of V to the set of left ideals of A.

b) The mapping $W\mapsto \mathfrak{b}(W)$ is a bijection from the set of linear subspaces of V to the set of right ideals of A.

c) Let $W_1$ and $W_2$ be linear subspaces of V. The relations $W_1\subset W_2$, $\mathfrak{a}(W_1)\supset \mathfrak{a}(W_2)$, and $\mathfrak{b}(W_1)\subset \mathfrak{b}(W_2)$ are equivalent.

Assertion b) follows from Example 1, b) of VIII, p. 104 applied to the invertible $(D^o,A^o$)-bimodule V, as does the equivalence of the relations $W_1\subset W_2$ and $\mathfrak{b}(W_1)\subset \mathfrak{b}(W_2)$.

Let $V^*$ be the dual of V, viewed as a right vector space over the opposite field $D^o$ of D. For any subspace W of V, denote the orthogonal of W in $V^*$ by $W'$. The mapping $W\mapsto W'$ is a bijection from the set of subspaces of V to the set of subspaces of $V^*$. If $W_1$ and $W_2$ are two subspaces of V, then the relations $W_1\subset W_2$ and $W'_1\supset W'_2$ are equivalent. Now, the mapping $u\mapsto^tu$ is an isomorphism from A to the opposite ring of End$_{D^o}(V^*)$; it transforms left ideals of A into right ideals of End$_{D^o}(V^*)$ and $\mathfrak{a}(W)$ into the set $\mathfrak{b}(W')$ of endomorphisms $h$ of $V^*$ such that $h(V^*)\subset W'$. Assertion a), as well as the equivalence of the relations $W_1\subset W_2$ and $\mathfrak{a}(W_1)\supset \mathfrak{a}(W_2)$, then follows from the assertion analogous to b) for the dual $V^*$ of V.

#### Corollary {#alg-viii-s7-n4-cor-1 .statement}

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

1) Let D be a field, V a right vector space over D, and A the ring End$_D(V)$. For any linear subspace W of V, we denote the set of elements $a$ of A satisfying $aW = 0$ (resp. $aV\subset W)$ by $\mathfrak{a}(W)$ (resp. $\mathfrak{b}(W))$. a) Prove that the mapping $W\mapsto \mathfrak{a}(W)$ (resp. $W\mapsto \mathfrak{b}(W))$ is a decreasing (resp. increasing) bijection from the set of linear subspaces of V to the set of left (resp. right) ideals of A generated by an idempotent. b) The minimal left ideals of A are the ideals $\mathfrak{a}$(H), where H is a hyperplane in V. The minimal right ideals are the ideals $\mathfrak{b}$(D), where D is a line in V. Deduce the form of the left (resp. right) ideals of A of finite length. c) Let W and $W'$ be two subspaces of V such that $W\not= 0$ and $W'\not= V$. Prove that the intersection $\mathfrak{a}(W)\cap \mathfrak{b}(W')$ is not reduced to 0. d) The mapping $u\mapsto^tu$ defines a ring isomorphism from A to a subring B of End$_{D^o}(V^*)$. Show that the image of $\mathfrak{a}(W)$ (resp. $\mathfrak{b}(W))$ under this isomorphism is the trace on B of the ideal $\mathfrak{b}(W^o)$ (resp. $\mathfrak{a}(W^o))$, where $W^o$ denotes the orthogonal of W in $V^*$. e) Let $\mathfrak{F}$ be the set of linear subspaces of V. For any left ideal $\mathfrak{a}$ of A, denote by $\mathfrak{F}(\mathfrak{a})$ the subset of $\mathfrak{F}$ consisting of the subspaces Ker $u$ where $u$ runs through $\mathfrak{a}$. The set $\mathfrak{F}(\mathfrak{a})$ is stable under intersection, and every linear subspace of V containing an element of $\mathfrak{F}(\mathfrak{a})$ belongs to $\mathfrak{F}(\mathfrak{a})$. Prove that the mapping $\mathfrak{a}\mapsto \mathfrak{F}(\mathfrak{a})$ is a bijection from the set of left ideals of A to the set of subsets of $\mathfrak{F}$ with these two properties. f ) Suppose that the dimension of V is infinite, and denote it by $\mathfrak{c}$. Let $\mathfrak{m}$ be a maximal left ideal of A that is not of the form $\mathfrak{a}(D)$. Prove that the intersection of the subspaces $W\in \mathfrak{F}(\mathfrak{m})$ is reduced to 0, that each of these subspaces is infinite-dimensional, and that there exist such subspaces of codimension $\mathfrak{c}$.

$\P 2)$ Let D be a field, V a right vector space of infinite dimension $\mathfrak{c}$ over D, and A the ring End$_D(V)$. a) Let $u$ and $v$ be endomorphisms of V such that rg($u)\leqslant$ rg($v)$. Prove that there exist elements $a$ and $b$ of A such that $u=avb$. b) For any infinite cardinal $\mathfrak{n}\leqslant \mathfrak{c}$, denote the set of endomorphisms of V of rank $<\mathfrak{n}$ by $\mathfrak{A}_{\mathfrak{n}}$. Prove that $\mathfrak{A}_{\mathfrak{n}}$ is a two-sided ideal of A and that every two-sided ideal of A distinct from $\{0\}$ and A is one of the $\mathfrak{A}_{\mathfrak{n}}$ (use a)). In particular, the ideal of endomorphisms of finite rank is the smallest nonzero two-sided ideal of A, and the ideal $\mathfrak{A}_{\mathfrak{c}}=\mathfrak{T}$ of endomorphisms of rank $<\mathfrak{c}$ is the greatest two-sided ideal of A distinct from A. c) Let B be a basis of V and $\mathfrak{U}$ an ultrafilter on B that is finer than the filter $\mathfrak{G}$ of complements of subsets of B of cardinal $<\mathfrak{c}$. For any set U in $\mathfrak{U}$, denote by $e_U$ the projector of V with kernel generated by the vectors of U and image generated by the vectors of B U. Let $\mathfrak{a}_{\mathfrak{U}}$ be the left ideal of A generated by the $e_U$, where U runs through $\mathfrak{U}$. Prove that the ideal $\mathfrak{T}+\mathfrak{a}_{\mathfrak{U}}$ is distinct from A. Let $\mathfrak{V}$ be another ultrafilter on B containing $\mathfrak{G}$ and distinct from $\mathfrak{U}$. Prove that we have $\mathfrak{a}_{\mathfrak{U}}+\mathfrak{a}_{\mathfrak{V}}= A$. d) Prove that the cardinal of the set of ultrafilters on B containing $\mathfrak{G}$ is $2^{2^{\mathfrak{c}}}$. (Use the arguments of Exercises 6 of Gen. Top., I, §8, p. 135 and 5 of Gen. Top., I, §4, p. 126. Observe that in the latter exercise, the trace on F of every nonempty open subset of X has the same cardinal as F.) e) Suppose Card(D) $\leqslant 2^{\mathfrak{c}}$. Deduce from d) that the set of classes of simple $(A/\mathfrak{T})$-modules has cardinal $2^{2^{\mathfrak{c}}}$ (cf. VIII, p. 52, Exercise 5, d)). f ) Deduce from the above that the ring A is primitive but not quasi-simple and that the ring $A/\mathfrak{T}$ is quasi-simple but not simple (VIII, p. 120, Remark 2).

3) Let D be a field, V a right vector space over D, and A a subring of the ring End$_D(V)$. a) Prove that the following conditions are equivalent:

(i) For every endomorphism $u$ of V and every finite sequence $x_1, . . . , x_n$ of vectors in V, there exists an element $a$ of A satisfying $u(x_i) =a(x_i)$ for $1\leqslant i\leqslant n$.

(ii) For every pair of elements $x, y$ of V with $x\not= 0$, there exists an $a\in A$ such that $a(x) =y$.

When these conditions are satisfied, we say that the subring A of End$_D(V)$ is dense. Assume from now on that A is dense. b) Prove that A is primitive (VIII, p. 120, Remark 2). Prove that, conversely, every primitive ring is isomorphic to a dense subring of the endomorphism ring of a vector space. c) Prove that the nonzero elements of the center of A are injective endomorphisms. In particular, the center of a primitive ring is an integral domain. d) Suppose that V is infinite-dimensional. For every integer $n >0$, prove that there exist a subring $A_n$ of A and a surjective homomorphism $A_n\rightarrow \mathbf{M}_n(D)$.

4) Let A be a primitive ring. a) If the ring A is commutative (resp. left Artinian), then it is a field (resp. a simple ring). b) Let $\mathfrak{a}$ and $\mathfrak{b}$ be nonzero left ideals of A. Prove that the ideal $\mathfrak{a}\mathfrak{b}$ is not zero.[^3] Deduce that the intersection of finitely many nonzero two-sided ideals of A is not reduced to 0. c) Prove that if for every $a\in A$, the element $1 +a^2$ is invertible in A, then A is a field (use Exercise 3, b)).

5) Let A be a ring. a) Let $e$ be an idempotent in A. Prove that if A is primitive (resp. quasi-simple), the same holds for the ring $eAe$ (use Exercise 3, b), Lemma 4 of VIII, p. 113, and Exercise 6, a) of VIII, p. 15). b) Let $n$ be an integer $\geqslant 1$. Prove that the matrix ring $\mathbf{M}_n(A)$ is primitive (resp. quasi-simple) if and only if A is primitive (resp. quasi-simple) (cf. VIII, p. 114, Example 2). c) Let B be a ring that is Morita equivalent to A; then B is primitive (resp. quasi-simple) if and only if A is.

6) Let A be a quasi-simple ring. a) An A-module is generating if and only if its dual is nonzero. b) Let $\mathfrak{a}$ be a left ideal of A, and let D be the ring End$_A(\mathfrak{a})$. Prove that $\mathfrak{a}$ is a finitely generated projective right D-module and that the mapping $a\mapsto a_{\mathfrak{a}}$ from A to End$_D(\mathfrak{a})$ is bijective. The ring D is quasi-simple if and only if the A-module $\mathfrak{a}$ is projective and finitely generated. c) Prove that a quasi-simple ring that contains a minimal left ideal is simple.

7) Let A be a ring. a) Let $\mathfrak{a}$ be a minimal left ideal of A. Prove that we have $\mathfrak{a}^2= 0$ or $\mathfrak{a}^2=\mathfrak{a}$. In the latter case, show that there exists an idempotent $e$ in $\mathfrak{a}$ such that $\mathfrak{a}= Ae$ (if $a\in A$ is such that $\mathfrak{a}a=\mathfrak{a}$, consider the automorphism $x\mapsto xa$ of $\mathfrak{a})$. b) Let $e$ be an idempotent in A. The ideal $Ae$ is minimal if and only if the ring $eAe$ is a field. c) Let $\mathfrak{a}$ and $\mathfrak{b}$ be two isomorphic left ideals of A. Prove that we have $\mathfrak{a}\mathfrak{b}=\mathfrak{b}$ if $\mathfrak{a}^2=\mathfrak{a}$, and $\mathfrak{a}\mathfrak{b}= 0$ if $\mathfrak{a}^2= 0$.

$\P 8)$ Let A be a ring. The left socle (or simply socle$)\mathfrak{s}$ of A is the socle of the A-module $A_s$, that is (VIII, p. 65), the sum of the minimal left ideals of A. It is a semisimple A-module, and its isotypical components are called its feet. Let $\mathfrak{a}$ be a foot of $\mathfrak{s}$. a) Prove that $\mathfrak{a}$ is a two-sided ideal and that the sum of the minimal ideals of square zero (Exercise 7) contained in $\mathfrak{a}$ is a two-sided ideal, namely the intersection of $\mathfrak{a}$ and its annihilator. b) Suppose that $\mathfrak{a}$ contains a minimal ideal with nonzero square. Prove that there are no nonzero elements $x$ of $\mathfrak{a}$ such that $\mathfrak{a}x= 0$ (use Exercise 7, c)). c) Under the assumption of b), prove that every left ideal of the pseudoring $\mathfrak{a}$ (I, §8, No. 1, p. 98) is an ideal of A (observe that the minimal ideals of $\mathfrak{a}$ are the minimal ideals of A contained in $\mathfrak{a})$. d) Suppose that the socle $\mathfrak{s}$ of A does not contain any minimal left ideals of square zero. Prove that every left ideal $\mathfrak{b}$ of A that has finite length as an A-module is contained in $\mathfrak{s}$ (use induction on the length of $\mathfrak{b}$ by observing that if $e$ is an idempotent in $\mathfrak{b}$, then $\mathfrak{b}e$ is a direct factor of $\mathfrak{b})$.

$\P 9)$ Let D be a field, V a right vector space over D, and A a dense subring of the ring End$_D(V)$ (Exercise 3). a) The subring A contains a nonzero endomorphism of finite rank if and only if the socle $\mathfrak{s}$ of A is nonzero (use Exercises 4, a) and 7, b) to prove that a minimal ideal of A is generated by an idempotent and then that this idempotent has rank 1). The socle of A then has a single foot (Exercise 4, a)). b) From now on, assume $\mathfrak{s}\not= 0$. Let $\mathfrak{a}$ be a minimal left ideal of A. Prove that there exists an element $`$ of the dual $V^*$ of V such that $\mathfrak{a}$ consists of the endomorphisms $z\mapsto v `(z)$ with $v\in V$. Let $V'$ be the set of linear forms $`\in V^*$ such that the endomorphism $z\mapsto v `(z)$ belongs to A for every $v\in V$. Prove that $V'$ is a $(D,A)$-sub-bimodule of $V^*$ and that $\mathfrak{s}$ is the set of endomorphisms of V of finite rank whose kernel can be written as Ker $`_1\cap  \cdots  \cap$ Ker$`_n$ with $`_1, . . . , `_n$ in $V'$. We can only have $\mathfrak{s}= A$ if the vector space V is finite-dimensional and A = End$_D(V)$. c) Let $\mathfrak{b}$ be a minimal right ideal of A. Prove that there exists a vector $v\in V$ such that $\mathfrak{b}$ consists of the endomorphisms $z\mapsto v `(z)$ with $`\in V'$. Deduce that the right socle of A is equal to its left socle $\mathfrak{s}$. d) Prove that $\mathfrak{s}$ is, moreover, the smallest nonzero two-sided ideal of A. e) Deduce from b) that a (left or right) Noetherian primitive ring with nonzero socle is simple (prove that V is necessarily finite-dimensional by considering the ideals contained in $\mathfrak{s})$. f ) Let M be a finite-dimensional subspace of V. Prove that $\mathfrak{s}$ contains a projector $e_M$ of V with image M. (Let $N'\subset V'$ be a supplementary subspace of the orthogonal of M. Prove that there exist bases $(v_j)_{1\leqslant j\leqslant k}$ of M and $(`_i)_{1\leqslant i\leqslant k}$ of $N'$ such that $`_i(v_j) =\delta_{ij}$, and consider the endomorphism $x\mapsto \sum_iv_i`_i(x).)$ Let N be the kernel of $e_M$. Prove that every endomorphism $u$ of V such that $u(M)\subset M$ and $u(N) = 0$ belongs to $\mathfrak{s}$. g) Let J be a finite subset of A. Prove that there exists a decomposition $V = M\oplus N$, where M is a finite-dimensional subspace and N is the orthogonal of a finite subset of $V'$, such that the ring of endomorphisms $u$ of V such that $u(M)\subset M$ and $u(N) = 0$ is contained in A and contains J. (Let $M_1=\sum_{u\in J}$ Im$u$ and $N_1=\cap_{u\in J}$ Ker $u$, apply f) to a subspace M containing $M_1$ and such that $M + N_1= V$, and then take N contained in $N_1.)$

10) Let A be a primitive ring with nonzero socle $\mathfrak{s}$, and let M be an A-module. Then M is faithful and isotypical if and only if we have $\mathfrak{s}M = M$ (use Proposition 4 of VIII, p. 50). Deduce that if $0\rightarrow M'\rightarrow M\rightarrow M''\rightarrow 0$ is an exact sequence of A-modules and $M'$ and $M''$ are faithful and isotypical, then the same holds for M.

11) Let K be a commutative field and V a vector space over K admitting a basis $(e_n)_{n\geqslant 1}$. Let $u$ and $v$ be the endomorphisms of V defined by $u(e_1) = 0,u(e_p) =e_{p-1}$ for $p >1$, and $v(e_p) =e_{p+1}$ for $p\geqslant 1$, and let A be the K-subalgebra of End$_K(V)$ generated by $1,u$, and $v$. We have $uv= 1_V$ and $vu\not= 1_V$. a) Prove that the elements $v^iu^j(i\geqslant 0, j\geqslant 0)$ form a basis of A over K. b) Prove that the ring A is primitive and that its socle $\mathfrak{s}$ is the set of endomorphisms $w$ of V such that the sequence $(w(e_p))_{p\geqslant 1}$ has finite support (observe that $\mathfrak{s}$ is the smallest two-sided ideal of A containing $1_V-vu)$. Prove that the K-algebra $A/\mathfrak{s}$ is isomorphic to $K[X,X^{-1}]$.

$\P 12)$ Let A be a ring and $d$ a derivation of A. Denote the ring $A[D]_{1,d}$ (VIII, p. 11) simply by A[D]. Every element $P\not= 0$ of A[D] can be written uniquely as $\sum^m_{k=0}a_kD^k$ with $a_k\in A$ and $a_m\not= 0$; we call $m$ the degree of P and $a_m$ its leading coefficient. a) Let $\mathfrak{b}$ be a two-sided ideal of A[D], and let $n$ be the minimum of the degrees of the nonzero elements of $\mathfrak{b}$. Prove that the set consisting of 0 and the leading coefficients of the elements of $\mathfrak{b}$ of degree $n$ is a two-sided ideal of A. b) Suppose that the ring A is quasi-simple, that A is a $\mathbf{Q}$-algebra, and that the derivation $d$ is not an inner derivation (III, §10, No. 6, p. 560). Prove that the ring A[D] is quasi-simple. c) Suppose that A is a commutative field of characteristic zero and that $d\not= 0$. Prove that every (left or right) ideal of A[D] is monogenous (consider an element of minimal degree in such an ideal). Deduce that A[D] is left and right Noetherian, quasi-simple, and without zero divisor but does not contain any minimal right or left ideals.

13) Let K be a commutative field of characteristic zero, and let A be the ring K[T]. Let $d$ be the derivation $_d^d_T$. Prove that the ring A[D] (Exercise 12) is quasi-simple. (Determine the derivations ad(D) and ad(T), and deduce that every nonzero two-sided ideal contains an invertible element.)

$\P 14)$ Let K be a commutative field. Let M be the free monoid generated by two elements $x$ and $y$, and let A be the algebra of the monoid M over K. Let V be a vector space over K admitting a basis $(e_n)_{n\geqslant 1}$. a) We define the structure of an A-module on V by setting $xe_1= 0,xe_p=e_{p-1}$ for $p >1$, and $ye_p=e_{2^p}$ for $p\geqslant 1$. Prove that V is a simple A-module. b) Prove that the A-module V is faithful. (Let $z\in M$. For $n\in \mathbf{N}$, denote the integer $s$ such that $e_s=ze_n$ by $P_z(n)$. Observe that we have $P_{zt}= P_z\circ P_t$ for $z, t$ in M. Deduce by induction on the length of $z$ and $t$ that if $z\not=t$, the set of integers $n$ such that $P_z(n) = P_t(n)$ is finite.) c) Likewise, for every integer $r >2$, prove that by setting $xe_1= 0,xe_p=e_{p-1}$ for $p >1$, and $ye_p=e_{r^p}$ for $p\geqslant 1$, we define the structure of a simple and faithful A-module on V. Prove that these structures are pairwise nonisomorphic.

15) Let A be a ring. A two-sided ideal $\mathfrak{p}$ of A is called prime if for any two-sided ideals $\mathfrak{a}$ and $\mathfrak{b}$ of A, the relation $\mathfrak{a}\mathfrak{b}\subset \mathfrak{p}$ implies $\mathfrak{a}\subset \mathfrak{p}$ or $\mathfrak{b}\subset \mathfrak{p}$. a) Prove that when A is commutative, this definition coincides with that given in I, §9, No. 3, p. 117. b) A two-sided ideal $\mathfrak{p}$ of A is prime if and only if for all elements $a$ and $b$ of $A-\mathfrak{p}$, there exists an $x\in A$ such that $axb /\in \mathfrak{p}$.

16) Let A be a ring. A two-sided ideal $\mathfrak{p}$ of A is called primitive if the quotient ring $A/\mathfrak{p}$ is primitive. a) Prove that the primitive ideals are the annihilators of the simple A-modules. In particular, the primitive ideals of a commutative ring are its maximal ideals. b) A two-sided maximal ideal is primitive; a primitive ideal is prime (Exercise 15). c) An element $x$ of A is invertible if and only if its image in every quotient of A by a primitive ideal is invertible (prove that if this is the case, $x$ is not contained in any maximal left ideals). d) Let $\mathfrak{a}$ be a left ideal of A. Prove that if $\mathfrak{a}+\mathfrak{p}= A$ for every primitive ideal $\mathfrak{p}$ of A, we have $\mathfrak{a}= A$. e) Let M be a finitely generated A-module such that $\mathfrak{p}M = M$ for every primitive ideal $\mathfrak{p}$ of A. Prove that M is zero (by induction on the smallest number of generators of M, using d)). f ) Let M be a Noetherian A-module. Prove that the intersection of the submodules $\mathfrak{a}M$, where $\mathfrak{a}$ runs through the set of finite products of primitive ideals, is reduced to 0 (use e)).

[^1]: If A and B are commutative fields, take care not to confuse the degree that is equal to [B : A] with the separable degree of the extension B of A, defined in V, §6, No. 5, p. 31 and also denoted by $[B : A]_s$.
[^2]: cf. A. H. Schofield, Artin’s problem for skew field extensions, Math. Proc. Cambridge Philos. Soc. **97** (1985), pp. 1–6.
[^3]: In this exercise and the next, if $\mathfrak{a}$ and $\mathfrak{b}$ are left ideals of A, we denote by $\mathfrak{a}\mathfrak{b}$ the left ideal generated by the products $ab$ for $a\in \mathfrak{a}$ and $b\in \mathfrak{b}$.
