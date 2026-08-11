---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 14
section_title: Central Simple Algebras
lang: en
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.251-A VIII.276
pdf_pages: 0268-0293
extraction: native
subsections:
    - "no": 1
      title: Central Simple Algebras
      page: 251
      pdf_page: 268
    - "no": 2
      title: Two Lemmas on Bimodules
      page: 254
      pdf_page: 271
    - "no": 3
      title: Conjugacy Theorems
      page: 256
      pdf_page: 273
    - "no": 4
      title: Automorphisms of Semisimple Algebras
      page: 257
      pdf_page: 274
    - "no": 5
      title: Simple Subalgebras of Simple Algebras
      page: 259
      pdf_page: 276
    - "no": 6
      title: Maximal Commutative Subalgebras
      page: 261
      pdf_page: 278
    - "no": 7
      title: Maximal Étale Subalgebras
      page: 264
      pdf_page: 281
    - "no": 8
      title: Diagonalizable Subalgebras of Simple Algebras
      page: 266
      pdf_page: 283
statements: 34
exercises: 19
content_sha256: e2de6c11e8459b9d9147a7d38b4bcae31d2059b8a3f9bf692c5d5c7ea151503b
---

## § 14. CENTRAL SIMPLE ALGEBRAS

In this section, K is a commutative field.

### 1. Central Simple Algebras

#### Definition 1 {#alg-viii-s14-def-1 .statement}

We say that an algebra A over the field K is central if the mapping $\lambda \mapsto \lambda 1$ is a bijection from K to the center of A.

A central algebra is not reduced to 0. For every integer $n\geqslant 1$, the matrix K-algebra $\mathbf{M}_n(K)$ is central (VIII, p. 83, Corollary 2) and simple (VIII, p. 120, Theorem 1). More generally, let D be a central K-algebra of finite degree; then $\mathbf{M}_n(D)$ is also central. Let A be a simple ring; its center Z is a field (VIII, p. 121, Corollary 1), and A is therefore a central simple algebra over Z. If the field K is algebraically closed, then a simple algebra of finite degree over K is central (VIII, p. 122, Corollary 3). The opposite algebra of a central simple algebra is central simple.

#### Remark 1 {#alg-viii-s14-n1-rem-1 .statement}

Let A and B be K-algebras. If $A\otimes_KB$ is a central simple algebra, then so are A and B (III, §4, No. 4, p. 468, Corollary of Proposition 6 and VIII, p. 221, Proposition 6). Conversely, if A and B are central simple algebras and if one of them has finite degree over K, then $A\otimes_KB$ is a central simple algebra (III, §4, No. 4, p. 468, Corollary of Proposition 6 and VIII, p. 222, Corollary 2).

#### Remark 2 {#alg-viii-s14-n1-rem-2 .statement}

Let A be a K-algebra and L an extension of the field K. If the L-algebra $A_{(L)}$ is central simple, then the K-algebra A is central simple. Conversely, if one of the degrees [A : K] and [L : K] is finite and if A is a central simple K-algebra, then the L-algebra $A_{(L)}$ is central simple. This follows from Corollary 2 of VIII, p. 222.

#### Remark 3 {#alg-viii-s14-n1-rem-3 .statement}

Let A and B be Morita-equivalent K-algebras. The algebra A is central simple if and only if B is (VIII, p. 105, Proposition 6; p. 111, Corollary; and p. 102, Corollary 1).

#### Remark 4 {#alg-viii-s14-n1-rem-4 .statement}

In particular, if A is a central simple K-algebra and $n\geqslant 1$, then $\mathbf{M}_n(A)$ is a central simple K-algebra (VIII, p. 102, Example 1).

#### Theorem 1 {#alg-viii-s14-thm-1 .statement}

Let A be a K-algebra of finite degree. The following properties are equivalent:

(i) The algebra A is central simple.

(ii) The algebra A is central and without radical.

(iii) The canonical homomorphism from the K-algebra $A\otimes_KA^o$ to the K-algebra End$_K(A)$ that sends $a\otimes a'$ to the K-linear mapping $x\mapsto axa'$ from A to A is bijective.

(iv) There exist an extension L of the field K and an integer $n\geqslant 1$ such that the L-algebras $A_{(L)}$ and $\mathbf{M}_n(L)$ are isomorphic.

(v) For every separable closure $K'$ of K, there exists an integer $n\geqslant 1$ such that the $K'$-algebras $A_{(K')}$ and $\mathbf{M}_n(K')$ are isomorphic.

(vi) There exist a Galois extension L of the field K of finite degree and an integer $n\geqslant 1$ such that the L-algebras $A_{(L)}$ and $\mathbf{M}_n(L)$ are isomorphic.

(vii) There exist a K-algebra of finite degree D that is a field with center K and an integer $n\geqslant 1$ such that the algebra A is isomorphic to the algebra $\mathbf{M}_n(D)$.

A ring is simple if and only if it is semisimple and its center is a field (VIII, p. 143, Corollary of Proposition 10). Since A is an algebra of finite degree over the field K, it is a left Artinian ring; it is therefore semisimple if and only if it is without radical (VIII, p. 154, Proposition 4). The equivalence of (i) and (ii) follows.

Set $E = A\otimes_KA^o$ and F = End$_K(A)$; denote by $\varphi$ the canonical homomorphism from E to F defined by the relation $\varphi (a\otimes a')(x) =axa'$ for $x, a, a'$ in A. If the algebra A is central simple, then so are $A^o$ and, therefore, E (Remark 1), so $\varphi$ is injective. Now, we have $[E : K] = [A : K]^2= [F : K]$, so $\varphi$ is bijective. Conversely, suppose that $\varphi$ is bijective; since the algebra F is central simple (because it is isomorphic to a matrix algebra $\mathbf{M}_m$(K)), so is E, and therefore so is A (Remark 1). We have thus proved the equivalence of (i) and (iii).

By Remark 4, assertion (vii) implies assertion (i). The converse implication follows from Corollary 3 of VIII, p. 122 and Corollary 2 of VIII, p. 83.

It is clear that (vi) implies (iv), and (iv) implies (i) by Remark 2.

It remains to prove the implications (i)$\Rightarrow$(v)$\Rightarrow$(vi). Suppose that A is central simple, and let $K'$ be a separable closure of K (V, §7, No. 8, p. 45) . Then $A_{(K')}$ is a central simple algebra of finite degree over $K'$ (VIII, p. 251, Remark 2). By the corollary of VIII, p. 231, there consequently exist an integer $n\geqslant 1$ and an isomorphism of $K'$-algebras from $A_{(K')}$ to $\mathbf{M}_n(K')$; observe that the $K'$-algebras $\mathbf{M}_n(K')$ and $\mathbf{M}_n(K)_{(K')}$ are isomorphic. By Lemma 4 of VIII, p. 234, there exists a subextension L of $K'$, finitely generated over K, such that the L-algebras $A_{(L)}$ and $\mathbf{M}_n(K)_{(L)}$ are isomorphic. Then L is separable and of finite degree over K, so contained in a subextension $L'$ of $K'$ that is Galois and of finite degree over K (V, §10, No. 1, p. 57, Proposition 2). The $L'$-algebras $A_{(L')}$ and $\mathbf{M}_n(L')$ are then isomorphic.

#### Corollary 1 {#alg-viii-s14-thm-1-cor-1 .statement}

Let A be a central simple algebra of finite degree over a separably closed field K. There exists an integer $n\geqslant 1$ such that A is isomorphic to the matrix algebra $\mathbf{M}_n(K)$.

Indeed, every Galois extension of K is equal to K; it suffices to apply the equivalence of properties (i) and (v) of Theorem 1.

#### Corollary 2 {#alg-viii-s14-thm-1-cor-2 .statement}

Let A be a central simple algebra of finite degree over K (for example, a field of finite degree over K with center K). There exists an integer $n\geqslant 1$ such that $[A : K] =n^2$.

Let L be an extension of K and $n$ a strictly positive integer such that the L-algebras $A_{(L)}$ and $\mathbf{M}_n(L)$ are isomorphic. We have

$$
[A : K] = [A_{(L)}: L] = [\mathbf{M}_n(L) : L] =n^2
$$

In the notation of Corollary 2, the integer $n$ is called the reduced degree of A.

#### Remark 5 {#alg-viii-s14-n1-rem-5 .statement}

Let A be a central simple algebra of finite degree over K whose reduced degree is a prime number $`$. Then either A is a field, or A is isomorphic to $\mathbf{M}_`(K)$. Indeed, A is isomorphic to an algebra of the form $\mathbf{M}_n$(D), where D is a field with center K, and we have

$$
`^2= [A : K] =n^2[D : K]
$$

if A is not a field, then $n\not= 1$, so $n=`$ and D = K.

### 2. Two Lemmas on Bimodules

Let A and B be rings. For any homomorphism $f$ from B to A, we denote by $A^f$ the $(B$, A)-bimodule with underlying right A-module $A_d$ and external law for its left B-module structure given by $(b, a)\mapsto f(b)a$.

#### Lemma 1 {#alg-viii-s14-lem-1 .statement}

Let $f$ and $g$ be homomorphisms from B to A. The following conditions are equivalent:

(i) The $(B,A)$-bimodules $A^f$ and $A^g$ are isomorphic.

(ii) There exists an inner automorphism (I, §8, No. 4, p. 102, Example 2) $\theta$ of A such that $g=\theta \circ f$.

The automorphisms of the right A-module $A_d$ are the mappings $x\mapsto ax$, where $a$ is an invertible element of A. Such an automorphism is a B-linear mapping from $A^f$ to $A^g$ if and only if we have

$$
g(b)ax=af(b)x
$$

for every $x$ in A and every $b$ in B. This relation is equivalent to $g(b) =af(b)a^{-1}$ for every $b$ in B, that is, to $g=\theta \circ f$, where $\theta$ is the inner automorphism $x\mapsto axa^{-1}$ of A.

#### Lemma 2 {#alg-viii-s14-lem-2 .statement}

Suppose that B is a semisimple ring that is a finitely generated module over its center Z. Let M and N be $(B,A)$-bimodules. Suppose that they have finite length (which is, in particular, the case when they are right A-modules of finite length). If M and N are isomorphic as $(Z,A)$-bimodules, then they are isomorphic as $(B,A)$-bimodules.

A) First consider the case when B is the endomorphism ring of a vector space S of finite dimension $d$ over a commutative field L. We then have Z = L; we view S as a $(B$, Z)-bimodule. The ring B is simple, S is a simple B-module, and Z is the commutant of S; every B-module is isotypical of type S (VIII, p. 122, Proposition 2 a)). Let $(V, \alpha )$ (resp. $(W, \beta ))$ be a description of the B-module M (resp. N). The set V (resp. W) is endowed with a $(Z$, A)-bimodule structure such that $\alpha$ (resp. $\beta )$ is an isomorphism of $(B$, A)-bimodules (VIII, p. 64, Remark 2). As $(Z$, A)-bimodules, M is isomorphic to $V^d$ and N to $W^d$, and there exists an isomorphism from the set of $(Z$, A)-sub-bimodules of V, ordered by inclusion, to that of the $(B$, A)-sub-bimodules of M (loc. cit.). Hence V is a $(Z$, A)-bimodule of finite length, and so is W. Since the $(Z,A)$-bimodules $V^d$ and $W^d$ are isomorphic, the $(Z$, A)-bimodules V and W are isomorphic by Theorem 2, d) of VIII, p. 37 applied to the ring $Z\otimes_{\mathbf{Z}}A^o$. Finally, the $(B$, A)-bimodules M and N are isomorphic.

B) Now consider the case when B is a simple ring that is finitely generated as a Z-module. Then Z is a field, and B is a central simple algebra of finite degree over the field Z. By Theorem 1 of VIII, p. 252, there exists an extension $Z'$ of Z of finite degree over Z such that the $Z'$-algebra $B'= B_{(Z')}$ is isomorphic to the endomorphism algebra of a finite-dimensional $Z'$-vector space. Set $M'= M_{(Z')}$ and $N'= N_{(Z')}$. Then $M'$ and $N'$ are $(B'$, A)-bimodules of finite length; viewed as $(Z'$, A)-bimodules, $M'$ and $N'$ are isomorphic. By the case treated in $A), M'$ and $N'$ are isomorphic as $(B'$, A)-bimodules and a fortiori as $(B$, A)-bimodules. Set $r= [Z': Z]$. The $(B$, A)-bimodule $M'= Z'\otimes_ZM$ is isomorphic to $M^r$, and, likewise, the $(B$, A)-bimodule $N'$ is isomorphic to $N^r$. Since M and N are $(B$, A)-bimodules of finite length, it follows from Theorem 2, d) of VIII, p. 37 that the $(B$, A)-bimodules M and N are isomorphic.

C) Finally, consider the general case, when B is a semisimple ring that is finitely generated as a Z-module. Let $\mathscr{S}$ be the set of classes of simple B-modules; it is finite (VIII, p. 136, Proposition 1). For any $\lambda \in \mathscr{S}$, denote by $M_{\lambda}$ (resp. $N_{\lambda})$ the isotypical component of type $\lambda$ of the B-module M (resp. N); it is a $(B$, A)-sub-bimodule of M (resp. N) (Remark, VIII, p. 67). For $\lambda \in \mathscr{S}$, denote the annihilator of the B-module $\lambda$ by $\mathfrak{b}_{\lambda}$, and set $B_{\lambda}= B/\mathfrak{b}_{\lambda}$; let $Z_{\lambda}$ be the center of $B_{\lambda}$. For $\lambda \in \mathscr{S}$, the $(B_{\lambda}$, A)-bimodules $M_{\lambda}$ and $N_{\lambda}$ have finite length. We can then identify B with the product of the simple rings $B_{\lambda}$ and Z with the product of the $Z_{\lambda}$ (VIII, p. 141, Proposition 8). Moreover, we can identify M with $\prod_{\lambda\in\mathscr{S}}M_{\lambda}$ and N with $\prod_{\lambda\in\mathscr{S}}N_{\lambda}$. By assumption, M and N are isomorphic as $(Z$, A)-bimodules; it follows that for $\lambda \in \mathscr{S}, M_{\lambda}$ and $N_{\lambda}$ are isomorphic $(Z_{\lambda}$, A)-bimodules. By the case treated in B), the $(B_{\lambda}$, A)-bimodules $M_{\lambda}$ and $N_{\lambda}$ are isomorphic, and so the $(B$, A)-bimodules M and N are isomorphic.

#### Remark {#alg-viii-s14-n2-rem-1 .statement}

It follows from the proof of Lemma 2 that M and N are $(Z,A)$-bimodules of finite length. Consequently, if B and A are two semisimple rings that are finitely generated modules over their respective centers Z(B) and Z(A), then two $(B$, A)-bimodules of finite length that are isomorphic as (Z(B),Z(A))-bimodules are isomorphic.

### 3. Conjugacy Theorems

#### Theorem 2 {#alg-viii-s14-thm-2 .statement}

Let B be a semisimple ring and Z its center; suppose that B is a finitely generated Z-module. Let A be a right Artinian ring, and let $f$ and $g$ be ring homomorphisms from B to A; write $f_Z$ and $g_Z$ for the restrictions of $f$ and $g$ to Z. The following properties are equivalent:

(i) There exists an inner automorphism $\theta$ of A such that $g=\theta \circ f$.

(ii) There exists an inner automorphism $\theta$ of A such that $g_Z=\theta \circ f_Z$.

Since the ring A is right Artinian, $A_d$ is a right A-module of finite length (VIII, p. 6, Theorem 1). Hence $A^f$ and $A^g$ are $(B$, A)-bimodules of finite length. By Lemma 1 (VIII, p. 254), assertion (i) means that $A^f$ and $A^g$ are isomorphic $(B$, A)-bimodules and assertion (ii) that they are isomorphic $(Z,A)$-bimodules. The equivalence of (i) and (ii) therefore follows from Lemma 2 (VIII, p. 254).

#### Corollary {#alg-viii-s14-n3-cor-1 .statement}

Let A and B be algebras over the field K. Suppose that B is central simple and of finite degree and that A is right Artinian. Let $f$ and $g$ be K-algebra homomorphisms from B to A. There exists an inner automorphism $\theta$ of A such that $g=\theta \circ f$.

In the notation of Theorem 2, we have Z = K and therefore $f_Z= 1_Z=g_Z$.

Theorem 3 (Skolem–Noether). — Let A and B be simple K-algebras and Z(A) and Z(B) their centers. Suppose that the algebra B has finite degree over K and that the algebra $Z(A)\otimes_KZ(B)$ is a field (which is, in particular, the case when A or B is central). Let $f$ and $g$ be K-algebra homomorphisms from B to A. There exists an inner automorphism $\theta$ of A such that $g=\theta \circ f$.

By Lemma 1 of VIII, p. 254, it suffices to prove that the $(B,A)$-bimodules $A^f$ and $A^g$ are isomorphic. Now, we can view $A^f$ and $A^g$ as left modules over the algebra $C = B\otimes_KA^o$, which is simple by Proposition 7 of VIII, p. 221. As right A-modules, $A^f$ and $A^g$ are isomorphic to $A_d$, hence have finite length because the ring A is simple (VIII, p. 121, Corollary 1). A fortiori, $A^f$ and $A^g$ are C-modules of finite length. Let S be a simple C-module; there exist strictly positive integers $m$ and $n$ such that $A^f$ is isomorphic to $S^m$ and $A^g$ to $S^n$. The right A-module S therefore has nonzero finite length. Since the right A-modules underlying $A^f$ and $A^g$ are isomorphic, they have the same length; we therefore have $m=n$, so that the C-modules $A^f$ and $A^g$ are isomorphic.

#### Corollary 1 {#alg-viii-s14-thm-2-cor-1 .statement}

Let A be a central simple algebra over K, and let L be an extension of K of finite degree. If $f$ and $g$ are K-algebra homomorphisms from L to A, then there exists an inner automorphism $\theta$ of A such that $g=\theta \circ f$.

#### Corollary 2 {#alg-viii-s14-thm-2-cor-2 .statement}

Let A be a central simple algebra over K, and let L be a subalgebra of A that is a field. Every K-algebra homomorphism from L to A extends to an inner automorphism of A.

#### Corollary 3 {#alg-viii-s14-thm-2-cor-3 .statement}

Let D be a field of finite degree over K with center K. Every element of D is algebraic over K. Let $x$ and $y$ be elements of D; there exists an element $a$ of $D^*$ such that $y=axa^{-1}$ if and only if $x$ and $y$ have the same minimal polynomial over K.

The first assertion follows from Corollary 1 of V, §3, No. 1, p. 17.

Suppose that there exists an element $a$ of $D^*$ such that $y=axa^{-1}$; for every polynomial P of K[X], we have $P(y) =aP(x)a^{-1}$, and, in particular, we have $P(x) = 0$ if and and only if $P(y) = 0$. Consequently, $x$ and $y$ have the same minimal polynomial over K (V, §3, No. 1, p. 16, Theorem 1).

Conversely, suppose that $x$ and $y$ have the same minimal polynomial. By loc. cit., there exists a K-isomorphism $u$ from $K[x]$ to $K[y]$ such that $u(x) =y$, and $K[x]$ is a field. By Corollary 2$,u$ extends to an inner automorphism $\theta :z\mapsto aza^{-1}$ of D, and we therefore have $y=\theta (x) =axa^{-1}$.

#### Proposition 1 {#alg-viii-s14-prop-1 .statement}

Let A be a central simple algebra of finite degree over K. Let B be a K-algebra, and let $f$ and $g$ be algebra homomorphisms from B to A. The following properties are equivalent:

(i) There exists an inner automorphism $\theta$ of A such that $g=\theta \circ f$.

(ii) As left B-modules, $A^f$ and $A^g$ are isomorphic.

By Lemma 1 (VIII, p. 254), property (i) is equivalent to the fact that $A^f$ and $A^g$ are isomorphic as $(B$, A)-bimodules. Since A is finite-dimensional over $K, A^f$ and $A^g$ are B-modules of finite length. Since the center of A is equal to K, the equivalence of (i) and (ii) follows from Lemma 2 of VIII, p. 254 applied to the $(A^o,B^o$)-bimodules $A^f$ and $A^g$.

### 4. Automorphisms of Semisimple Algebras

#### Theorem 4 {#alg-viii-s14-thm-4 .statement}

Let A be a semisimple ring, Z its center, and $u$ an automorphism of A. Suppose that A is a finitely generated Z-module and that we have $u(z) =z$ for every $z$ in Z. Then $u$ is an inner automorphism.

This follows from Theorem 2 of VIII, p. 256 applied with $f=$ Id$_A$ and $g=u$. **Example.** — Theorem 4 applies in the following two specific cases:

a) Let D be a field and Z its center. If D has finite degree over Z, then every automorphism of D that fixes the elements of Z is an inner automorphism. The assumption that D has finite degree over Z is essential (VIII, p. 269, Exercise 4).

b) Let V be a finite-dimensional vector space over the field K. Every automorphism of the K-algebra End$_K(V)$ is an inner automorphism; this result extends to the case when the space V is not finite-dimensional over K (VIII, p. 272, Exercise 13).

In particular, every automorphism of a matrix algebra $\mathbf{M}_n(K)$ (with $n\geqslant$ 1) is an inner automorphism. This result admits the following generalization.

#### Proposition 2 {#alg-viii-s14-prop-2 .statement}

Let L be a commutative ring and V a free L-module of finite dimension $m$. Suppose that every L-module M such that $M^m$ is isomorphic to $L^m$ is isomorphic to L. Then every automorphism of the L-algebra End$_L(V)$ is an inner automorphism.

Set B = End$_L(V)$. Let $u$ be an automorphism of the L-algebra B. We view V as a left B-module; let $u_*(V)$ be the left B-module associated with $u$, with external law $(b, v)\mapsto u(b)(v)$ (II, §1, No. 13, p. 221). Let $(e_1, . . . , e_m)$ be a basis of the L-module V; given elements $v_1, . . . , v_m$ of V, there exists a unique element $b$ of B such that we have $b(e_i) =v_i$ for $1\leqslant i\leqslant m$. In other words, the element $e= (e_1, . . . , e_m)$ of $V^m$ provides a basis of the B-module $V^m$. Since $u$ is an automorphism, $e$ also gives a basis of the B-module $u_*(V^m) =u_*(V)^m$, which is therefore isomorphic to $V^m$. The $(B$, L)-bimodule V is invertible (VIII, p. 102, Example 1). By Theorem 2, b) of VIII, p. 103, there consequently exists an L-module M such that the B-module $u_*(V)$ is isomorphic to $V\otimes_LM$. The B-modules $V\otimes_LL^m$ and $V\otimes_LM^m$, respectively isomorphic to $V^m$ and $u_*(V)^m$, are therefore isomorphic. By loc. cit., the L-modules $L^m$ and $M^m$ are isomorphic. Given the assumption, M is isomorphic to L; consequently, the B-module $u_*$(V), which is isomorphic to $V\otimes_LM$, is isomorphic to V. Let $h$ be a B-module isomorphism from V to $u_*(V)$; it is, in particular, an automorphism of the L-module V, that is, an invertible element of B. For $b$ in B and $v$ in V, we have $h(b(v)) =u(b)(h(v))$ and therefore $u(b) =hbh^{-1}$.

The conditions of Proposition 2 are, in particular, satisfied when the commutative ring L is a principal ideal domain (VII, §3, p. 15, Corollary 3) or is Artinian (VIII, p. 37, Theorem 2, d)) or local (VIII, p. 36, Corollary 6).

### 5. Simple Subalgebras of Simple Algebras

#### Theorem 5 {#alg-viii-s14-thm-5 .statement}

Let A be a central simple K-algebra, and let B be a semisimple subalgebra of A of finite degree over K.

a) The commutant $B'$ of B in A is a simple subalgebra, and B is the commutant of $B'$ in A. Moreover, the algebra $B\cap B'$ is a semisimple commutative algebra of finite degree over K; it is the common center of B and $B'$.

b) Suppose that B is simple. Then $B'$ is simple, and we have the equalities

$$
[A : B']_s= [B : K],[A : B]_s= [B': K],[A : K] = [B : K][B': K]
$$

(See VIII, p. 124, Definition 2 for the definition of the left degree $[A : B]_s.)$

The K-algebra $A^o$ is central simple, and the K-algebra B is semisimple and of finite degree. By Corollary 1 of VIII, p. 221, the algebra $C = B\otimes_KA^o$ is semisimple. Let M be the C-module with the same additive group as A and with external law given by the formula $(b\otimes a)a'=ba'a$ for $a, a'$ in A and $b$ in B. Let $u$ be an element of End$_{\mathbf{Z}}(A)$. Then $u$ belongs to the commutant $C'_M$ of the C-module M if and only if $u$ is right A-linear and left B-linear, in other words, if and only if $u$ belongs to the commutant of $B_M$ in the ring of homotheties of the A-module $A_s$. We consequently define an isomorphism $\gamma$ from $B'$ to $C'_M$ by the relation $\gamma (b')(x) =b'x$ for $b'$ in $B'$ and $x$ in M. Now, the ring C is semisimple, and the C-module M is generated by the element 1 of A. By Proposition 6 of VIII, p. 139, the ring $C'_M$ is semisimple, so the algebra $B'$ is semisimple.

Let $\varphi$ be the K-algebra homomorphism from $A\otimes_KA^o$ to End$_K(M)$ that sends $a\otimes a'$ to the K-linear mapping $x\mapsto axa'$ from M to M. Since the K-algebras A and $A^o$ are central simple, the only two-sided ideals of $A\otimes_KA^o$ are 0 and $A\otimes_KA^o$ (VIII, p. 218, Corollary). We have $C_M=\varphi (B\otimes A^o)$ and $C'_M=\varphi (B'\otimes K)$. The homomorphism $\varphi$ is not zero; it is therefore injective. Since the ring C is semisimple, we have $C''_M= C_M$ by Proposition 5 of VIII, p. 139. It follows that the subalgebra $B\otimes_KA^o$ of $A\otimes_KA^o$ is the commutant of the subalgebra $B'\otimes_KK$. The commutant of $B'\otimes_KK$ in $A\otimes_KK$ is therefore equal to $(B\otimes_KA^o)\cap (A\otimes_KK)$, that is, to $B\otimes K$ by Proposition 19 of II, §7, No. 9, p. 311. Hence the commutant of $B'$ in A is equal to B. The algebra $L = B\cap B'$ is the center of B. Since B is a semisimple algebra of finite degree over K, the algebra L is commutative and semisimple and has finite degree over K. Since B is the commutant of $B'$ in A, the center of $B'$ is also equal to $L = B\cap B'$ (VIII, p. 77). We have proved a).

Now suppose that the algebra B is simple. By Corollary 2 of VIII, p. 222, the ring C is simple. By Proposition 4 of VIII, p. 123 applied to the C-module M, whose commutant is isomorphic to $B'$, the ring $B'$ is simple and M is a $B'$-module of finite length. In other words, $B'$ is a simple subring of the simple ring A, and the left degree $[A : B']_s$ is an integer $m\geqslant 1$. Viewed as a left $B'$-module, A has a finite basis $(a_1, . . . , a_m)$. Moreover (loc. cit.), $\varphi$ induces by restriction an isomorphism from C to $C''_M=$ End$_{B'}$(A), and the mapping $c\mapsto (ca_1, . . . , ca_m)$ from C to $A^m$ is therefore bijective. Consequently, C is a free right A-module of dimension $m$. Now, we have $C = B\otimes A^o$, so C is a free right A-module of dimension [B : K]; it follows that $[A : B']_s=m= [B : K]$. From Proposition 6 of VIII, p. 125, we deduce

$$
[A : K] = [A : B']_s[B': K] = [B : K] [B': K]
$$

since we also have

$$
[A : K] = [A : B]_s[B : K]
$$

and [B : K] is finite and nonzero, we conclude that we have the equality $[A : B]_s= [B': K] ($Set Theory, III, §6, No. 3, p. 188, Corollary 3). We have proved b).

Let A be a central simple K-algebra of finite degree. There can exist semisimple commutative subalgebras B of A satisfying $[A : K]\not=$ $[B : K] [B': K]$ (Exercise 1 of VIII, p. 269).

#### Theorem 6 {#alg-viii-s14-thm-6 .statement}

Let A be a central simple K-algebra, B a subalgebra of A of finite degree, and $B'$ its commutant in A.

a) Suppose that B is central simple. Then $B'$ is central simple, and the K-algebra homomorphism $\theta : B\otimes_KB'\rightarrow A$ that sends $b\otimes b'$ to $bb'$ is an isomorphism.

b) Suppose that B is semisimple, and let $L = B\cap B'$. Then $B'$ is a semisimple algebra. The commutant $L'$ of L in A is a semisimple ring with center L, and the ring homomorphism $\psi : B\otimes_LB'\rightarrow L'$ that sends $b\otimes b'$ to $bb'$ is an isomorphism.

Let us prove a). If B is central simple, then $B'$ is central simple by Theorem 5 of VIII, p. 259. Hence the K-algebra $B\otimes_KB'$ is simple (VIII, p. 222, Corollary 2), and the homomorphism $\theta : B\otimes_KB'\rightarrow A$ is injective. Now, by the equality of $[A : B']_s$ and [B : K] (Theorem 5), the left $B'$-modules $B\otimes_KB'$ and A are free of the same finite dimension; they are therefore $B'$-modules of the same finite length. By Corollary 2 of II, §1, No. 10, p. $213,\theta$ is bijective.

Let us prove b). By Theorem 5, the algebra L is commutative, of finite degree over K, and semisimple. By loc. cit. applied to L, its commutant $L'$ in A is a semisimple algebra, and L is the commutant of $L'$ in A, so L is the center of $L'$. Since L is the center of the semisimple rings $L', B$, and $B'$, we can identify $L'$ with a finite product of simple rings $L'_i$ (for $i\in I)$, so that we have

$$
L =\prod_{i\in I}L_i,B =\prod_{i\in I}B_i,B'=\prod_{i\in I}B'_i
$$

where $L_i$ is the center of $L'_i$ and where $B_i$ and $B'_i$ are subalgebras of $L'_i$ with center $L_i$ that are each other’s commutants in $L'_i$. We view $L'_i$ as a central simple algebra over the commutative field $L_i$ and $B_i$ as a central simple $L_i$-algebra of finite degree. By assertion a), the canonical mapping $\psi_i: B_i\otimes_{L_i}B'_i\rightarrow L'_i$ that sends $b_i\otimes b'_i$ to $b_ib'_i$ is a ring isomorphism. Now, we can identify $B\otimes_LB'$ with $\prod_{i\in I}(B_i\otimes_{L_i}B'_i)$, so that $\psi$ is the product of the family of mappings $(\psi_i)_{i\in I}$. Therefore, $\psi$ is a ring isomorphism.

#### Corollary {#alg-viii-s14-n5-cor-1 .statement}

Suppose that the field K is algebraically closed and that A is a simple algebra of finite degree over K. Let B be a simple subalgebra of A, and let $B'$ be the commutant of B in A. Then $B'$ is a simple K-algebra, B is the commutant of $B'$, we have $[A : K] = [B : K][B': K]$, and the canonical homomorphism from $B\otimes_KB'$ to A is a K-algebra isomorphism.

Since every simple algebra of finite degree over K is central, the corollary follows from Theorems 5 and 6.

### 6. Maximal Commutative Subalgebras

We say that a subalgebra of a K-algebra A is a maximal commutative subalgebra of A if it is a maximal element of the set of commutative subalgebras of A.

#### Lemma 3 {#alg-viii-s14-lem-3 .statement}

Let A be a K-algebra and L a subalgebra of A.

a) The algebra L is a maximal commutative subalgebra of A if and only if L is equal to its commutant $L'$ in A.

b) Let $K'$ be a nonzero commutative K-algebra. Then L is a maximal commutative subalgebra of A if and only if $L_{(K')}$ is a maximal commutative subalgebra of $A_{(K')}$.

Let us prove a). First suppose that L is equal to $L'$. Then L is commutative; if M is a commutative subalgebra of A containing L, then we have $xy=yx$ for $x$ in L and $y$ in M, so $M\subset L'$ and therefore M = L. Consequently, L is a maximal commutative subalgebra of A.

Conversely, suppose that L is a maximal commutative subalgebra of A, and let $x$ be an element of $L'$. The subalgebra M of A generated by $L\cup  \{x\}$ is then commutative and contains L. Because L is maximal, we have M = L, and so $x\in L$ and finally $L = L'$, which gives a).

By Proposition 6 of III, §4, No. 4, p. 468, the commutant of $L_{(K')}$ in $A_{(K')}$ is $L'_{(K')}$. Since the equalities $L = L'$ and $L_{(K')}= L'_{(K')}$ are equivalent (II, §7, No. 9, p. 311, Proposition 19), assertion b) follows from a).

#### Proposition 3 {#alg-viii-s14-prop-3 .statement}

Let A be a central simple K-algebra of finite degree, and let L be a semisimple commutative subalgebra of A. The following properties are equivalent:

(i) The algebra L is a maximal commutative subalgebra of A.

(ii) The left L-module A is free, of dimension [L : K].

(iii) We have $[A : K] = [L : K]^2$. Suppose, moreover, that A is the algebra End$_K(V)$, where V is a vector space of nonzero finite dimension over K. Then the previous properties are also equivalent to the following:

(iv) V is a free L-module of dimension 1.

A) Suppose that A is of the form End$_K$(V), where V is a vector space of nonzero finite dimension over the field K. We will establish the equivalence of conditions (i) through (iv) following the diagram

(i) $=\Rightarrow$ (iv) $=\Rightarrow$ (ii) $=\Rightarrow$ (iii) $=\Rightarrow$ (i) .

Since L is a semisimple commutative algebra of finite degree over K, we can identify it with a finite product $\prod_{i\in I}L_i$ of extensions of K of finite degree (VIII, p. 137, Proposition 3). For every $i\in I$, let $V_i$ be the isotypical component of type $L_i$ of the L-module V; it is a vector space of nonzero finite dimension over $L_i$ because V is a faithful L-module (VIII, p. 144, Corollary). We can then identify V with $\prod_{i\in I}V_i$. Under these conditions, the commutant $L'$ of L in A, which is simply the algebra End$_L$(V), can be identified with the product $\prod_{i\in I}$ End$_{L_i}(V_i)$.

Suppose that L is a maximal commutative subalgebra of End$_K(V)$. By Lemma 3, a), we have $L = L'$, so $L'$ is commutative and we have dim$_{L_i}(V_i) = 1$ for every $i\in I$. So (i) implies (iv).

Suppose that the L-module V is free of dimension 1. Let $(e_1, . . . , e_r)$ be a basis of V over K. The mapping $a\mapsto (ae_1, . . . , ae_r)$ is an isomorphism of left A-modules and therefore of L-modules from A to $V^r$. Consequently, A is a free left L-module of dimension $r$, and we have $r=$ dim$_K(V) = [L : K]$. So (iv) implies (ii).

It is clear that (i) implies (iii).

Finally, suppose that we have $[A : K] = [L : K]^2$, in other words, dim$_K(V) = [L : K]$. We then have $\sum_i$ dim$_{L_i}(V_i)[L_i: K] =\sum_i[L_i: K]$, so that $V_i$ has dimension 1 over $L_i$ for every $i$. We then have End$_{L_i}(V_i) = L_i$ for every $i$, and so $L'= L$. By Lemma 3, a), L is a maximal commutative subalgebra of A. So (iii) implies (i).

B) Let us continue with the general case. By Theorem 1 of VIII, p. 252, there exists a separable extension $K'$ of K of finite degree such that the $K'$-algebra $A_{(K')}$ is isomorphic to an algebra End$_{K'}(V')$, where $V'$ is a vector space of nonzero finite dimension over $K'$. Then the $K'$-algebra $L_{(K')}$ is commutative and semisimple (VIII, p. 222, Corollary 2). By the first part of the proof, the following properties are equivalent:

(i$')$ The algebra $L_{(K')}$ is a maximal commutative subalgebra of $A_{(K')}$.

(ii$')$ The left $L_{(K')}$-module $A_{(K')}$ is free, of dimension $[L_{(K')}: K']$.

(iii$')$ We have $[A_{(K')}: K'] = [L_{(K')}: K']^2$. By Lemma 3, b), properties (i) and (i’) are equivalent.

Set $n= [L : K]$; then $n= [L_{(K')}: K']$. Property (ii) means that the left L-modules A and $L^n$ are isomorphic; by Theorem 3 of VIII, p. 37, this is equivalent to the $L_{(K')}$-modules $A_{(K')}$ and $(L_{(K')})^n$ being isomorphic. The equivalence of (ii) and (ii$')$ follows.

Finally, we have $[A : K] = [A_{(K')}: K']$ and $[L : K] = [L_{(K')}: K']$, which give the equivalence of properties (iii) and (iii$')$. We have thus proved the equivalence of properties (i), (ii), and (iii).

#### Corollary {#alg-viii-s14-n6-cor-1 .statement}

Let A be a central simple algebra of finite degree over K, and let L be a semisimple commutative K-algebra such that [A : K] is equal to $[L : K]^2$. Let $f$ and $g$ be injective homomorphisms from L to A. There exists an inner automorphism $\theta$ of A such that $g=\theta \circ f$.

Set $n= [L : K]$. Viewed as a left module over the subring $f$(L), A is free of dimension $n$; this follows from the equivalence of properties (ii) and (iii) of Proposition 3. Since $f$ is an isomorphism from L to $f$(L), the left L-module $A^f$ (whose law of action is given by $(x, a)\mapsto f(x)a)$ is free of dimension $n$. The same holds for $A^g$, which is therefore isomorphic to $A^f$. We conclude using the equivalence of properties (i) and (ii) of Proposition 1 (VIII, p. 257).

Suppose that A is a central simple algebra of finite degree over K. There can exist maximal commutative subalgebras L of A that are not semisimple and for which $[A : K]\not= [L : K]^2$ (VIII, p. 270, Exercise 5).

### 7. Maximal Étale Subalgebras

#### Lemma 4 {#alg-viii-s14-lem-4 .statement}

Let A be a central simple algebra of finite degree over K, distinct from K. There exists an étale (V, §6, No. 3, p. 28, Definition 1) subalgebra of A distinct from K.

By Wedderburn’s theorem (VIII, p. 120, Theorem 1), we may assume that A is of the form $\mathbf{M}_n$(D), where $n$ is a strictly positive integer and D a field with center K.

Suppose $n >1$. The algebra of diagonal matrices with entries in K is an étale subalgebra of A distinct from K.

Suppose $n= 1$. Let $p$ be the characteristic exponent of D. By Lemma 1 of VIII, p. 230, there exists an element $a$ of D such that $a^{p^m}$ does not belong to K for any natural number $m$. So for $m$ sufficiently large, the element $x=a^{p^m}$ is separable over K (V, §7, No. 7, p. 44, Proposition 13), but it does not belong to K. The subalgebra $K(x)$ of A is a separable extension of the field K of finite degree, hence an étale subalgebra over K; it is distinct from K.

#### Proposition 4 {#alg-viii-s14-prop-4 .statement}

Let A be a central simple algebra of finite degree over K. Let L be a subalgebra of A, and let $L'$ be the commutant of L in A.

a) If L is maximal among the semisimple commutative subalgebras of A, then we have $L = L'$, and L is a maximal commutative subalgebra of A.

b) If L is maximal among the étale subalgebras of A, then we have $L = L'$, and L is a maximal commutative subalgebra of A.

We know that the relation $L = L'$ means that L is a maximal commutative subalgebra of A (VIII, p. 261, Lemma 3, a)). Suppose that L is semisimple, commutative, and distinct from $L'$. By Theorem 5 of VIII, p. 259$, L'$ is semisimple, and L is the commutant of $L'$ and therefore the center of $L'$; consequently, $L'$ is not commutative. It suffices to prove that there exists a semisimple commutative subalgebra M of A that is distinct from L and contains L and that is étale if L is étale.

By the structure theorem for semisimple rings (VIII, p. 135, Theorem 1), there exist simple rings $B_1, . . . ,B_r$ and an isomorphism $\varphi$ from $L'$ to $B_1\times  \cdots  \times B_r$. For $1\leqslant i\leqslant r$, denote the center of $B_i$ by $E_i$; we then have $\varphi (L) = E_1\times  \cdots  \times E_r$. Since $L'$ is not commutative, we may assume that $B_1$, for example, is not commutative; we therefore have $B_1\not= E_1$, and, by Lemma 4, there exists a subalgebra $M_1$ of $B_1$ that is commutative, distinct from $E_1$, and étale over $E_1$. Set $M =\varphi^{-1}(M_1\times E_2\times  \cdots  \times E_r)$; it is a semisimple commutative subalgebra of A containing L and distinct from L. Suppose that L is étale over K; let us prove that M is étale. The extensions $E_i$ of K are separable (V, §6, No. 4, p. 30, Proposition 3). Moreover, since the $E_1$-algebra $M_1$ and the K-algebra $E_1$ are étale, the K-algebra $M_1$ is also étale (V, §6, No. 5, p. 32, Corollary 2). Thus the K-algebra $M_1\times E_2\times  \cdots  \times E_r$ is étale, and therefore so is M.

Let A be a central simple algebra of finite degree over K. A subalgebra of A that is maximal among the semisimple commutative subalgebras of A is called a maximal semisimple commutative subalgebra of A. By Proposition 4, the term “maximal” refers to the property of being commutative or of being semisimple and commutative. A subalgebra of A that is maximal among the étale subalgebras of A is called a maximal étale subalgebra of A.

#### Corollary 1 {#alg-viii-s14-prop-4-cor-1 .statement}

Let A be a central simple K-algebra of finite degree. Every semisimple (resp. étale) commutative subalgebra of A is contained in a maximal commutative subalgebra of A that is semisimple (resp. étale).

#### Corollary 2 {#alg-viii-s14-prop-4-cor-2 .statement}

Let D be a field of finite degree over K with center K.

a) The maximal commutative subfields of D are the maximal commutative subalgebras of D and also the maximal semisimple commutative subalgebras of D. Every commutative subfield L of D is contained in a maximal commutative subfield.

b) Let L be a commutative subfield of D that is a separable extension of K; it is contained in a maximal commutative subfield of D that is a separable extension of K.

c) Let L be a commutative subfield of D. Then L is a maximal commutative subfield of D if and only if we have $[D : K] = [L : K]^2$.

A subalgebra of D is a field (V, §2, No. 2, p. 10, Proposition 1) and is therefore semisimple. Moreover, a maximal commutative subfield of D contains K. Assertions a) and b) then follow from Corollary 1 and assertion c) of Proposition 3 (VIII, p. 262).

#### Proposition 5 {#alg-viii-s14-prop-5 .statement}

Let A be a central simple algebra of finite degree over K. Let B be a semisimple subalgebra of A, and let $B'$ be the commutant of B.

a) The algebra B contains a maximal semisimple commutative subalgebra of A if and only if B contains $B'$.

b) Suppose that B contains $B'$, and let $g$ be a K-algebra homomorphism from B to A. There exists an inner automorphism $\theta$ of A that coincides with $g$ on B.

Let L be a maximal commutative subalgebra of A; by Lemma 3 of VIII, p. 261, L is equal to its commutant $L'$ in A. If B contains L, then its commutant $B'$ is contained in $L'$ and therefore in B.

Conversely, suppose that $B'$ is contained in B. Then $B'$ is the center of B, and it is a semisimple commutative algebra (VIII, p. 137, Proposition 2). By Corollary 1, there exists a maximal semisimple commutative subalgebra L of A containing $B'$. The commutant of L is L (VIII, p. 261, Lemma 3, a)), and that of $B'$ is equal to B (VIII, p. 259, Theorem 5). The relation $L\supset B'$ therefore implies $L\subset B$. We have proved a).

Let us prove b). Suppose that B contains $B'$, and choose a maximal semisimple commutative subalgebra L of A contained in B, which exists by a). Let $g$ be a homomorphism from B to A. By Proposition 3 of VIII, p. 262, we have the equality $[A : K] = [L : K]^2$; by the corollary of VIII, p. 263, there exists an inner automorphism $\theta_1$ of A that coincides with $g$ on L. If $f$ is the canonical injection of B into A, then the homomorphisms $g$ and $\theta_1\circ f$ have the same restriction to the center $B'$ of B because $B'$ is contained in L. By Theorem 2 of VIII, p. 256, there exists an inner automorphism $\theta$ of A such that $g=\theta \circ f$; in other words, $\theta$ extends $g$.

### 8. Diagonalizable Subalgebras of Simple Algebras

Let D be a K-algebra that is a field, and let V be a finite-dimensional right vector space over D. Let L be a K-subalgebra of End$_D(V)$ that is a diagonalizable K-algebra (V, §6, No. 3, p. 28). By definition, L has finite degree over K, and there exists a basis $(\varepsilon_i)_{i\in I}$ of L over K with the following properties:

$\varepsilon^2_i=\varepsilon_i, \varepsilon_i\varepsilon_j= 0$ if $i\not=j ,\sum_{i\in I}\varepsilon_i= 1$.

Set $V_i=\varepsilon_i(V)$ for every $i$ in I; then $(V_i)_{i\in I}$ is a family of nonzero linear subspaces of V with direct sum V (II, §1, No. 8, p. 209, Proposition 12). Let $u$ be an endomorphism of V; then $u$ belongs to L if and and only if for every $i\in I$, there exists an element $\lambda_i$ of K such that $u(x) =\lambda_ix$ for every $x\in V_i$.

Conversely, suppose that V is the direct sum of a family $(V_i)_{i\in I}$ of nonzero linear subspaces. For any element $\boldsymbol{\lambda }= (\lambda_i)_{i\in I}$ of $K^I$, denote by $u_{\boldsymbol{\lambda }}$ the endomorphism of the D-vector space V such that $u_{\boldsymbol{\lambda }}(x) =\lambda_ix$ for $x\in V_i$. The set L of endomorphisms $u_{\boldsymbol{\lambda }}$ for $\boldsymbol{\lambda }\in K^I$ is a diagonalizable subalgebra of End$_D(V)$ having the family $(\varepsilon_i)_{i\in I}$ as basis, where $\varepsilon_i$ is the projector with image $V_i$ and kernel $\sum_{j\not=i}V_j$. We say that L is the diagonalizable subalgebra of End$_D(V)$ associated with the direct sum decomposition $V =\oplus_{i\in I}V_i$. We have [L : K] = Card(I) $\leqslant$ dim$_D(V)$.

#### Proposition 6 {#alg-viii-s14-prop-6 .statement}

Let L be the diagonalizable subalgebra of End$_D(V)$ associated with a direct sum decomposition $V =\oplus_{i\in I}V_i$.

a) The algebra L is maximal among the diagonalizable subalgebras of the K-algebra End$_D(V)$ if and only if every $V_i$ has dimension 1 over D.

b) The algebra L is a maximal commutative subalgebra of End$_D(V)$ if and only if we have D = K and every $V_i$ has dimension 1 over K.

If every vector space $V_i$ has dimension 1 over D, then we have

[L : K] = Card(I) = dim$_D(V)$,

so L is maximal among the diagonalizable subalgebras of End$_D(V)$. In the opposite case, there exists an index $j\in I$ such that dim$_D(V_j)\geqslant 2$. Choose two nonzero linear subspaces $V'_j$ and $V''_j$ of $V_j$ with direct sum $V_j$. The diagonalizable subalgebra of End$_D(V)$ associated with the direct sum decomposition $V = (\oplus_{i\in I\{j\}}V_i)\oplus V'_j\oplus V''_j$ contains L and is not equal to L; assertion a) follows.

The commutant $L'$ of L in End$_D(V)$ consists of the endomorphisms of the form $(x_i)\mapsto (u_i(x_i))$, with $(u_i)\in \prod_{i\in I}$ End$_D(V_i)$. The algebra L is a maximal commutative subalgebra of End$_D(V)$ if and only if we have $L = L'$ (VIII, p. 261, Lemma 3, a)). This relation is therefore equivalent to “End$_D(V_i) = K$ for every $i\in$ I”; assertion b) follows.

#### Proposition 7 {#alg-viii-s14-prop-7 .statement}

Let L be a commutative algebra of finite degree over K. The following properties are equivalent:

(i) The algebra L is étale.

(ii) There exists a separable extension of K of finite degree that diagonalizes K.

The implication (ii)$\Rightarrow$(i) follows from V, §6, No. 3, p. 29, Proposition 2.

Let us prove the implication (i)$\Rightarrow$(ii). Let Ω be a separable closure of K. By Theorem 4 of V, §6, No. 7, p. 34, there exist extensions $L_1, . . . ,L_n$ of K of finite degree, contained in Ω, such that L is isomorphic to the product $L_1\times  \cdots  \times L_n$. Let N be a Galois extension of K that contains the $L_i$ (V, §10, No. 1, p. 58), and let us prove that $L_{(N)}$ is diagonalizable. By the primitive element theorem (V, §7, No. 4, p. 40, Theorem 1), for every $i\in [1, n]$, there exists an irreducible separable polynomial $P_i\in K[X]$ such that $L_i$ is isomorphic to $K[X]/(P_i)$. Since N is a normal extension of K in which $P_i$ admits a root, the polynomial $P_i$ splits in N[X], with simple roots. Consequently, the N-algebra $L_{i(N)}$, which is isomorphic to $N[X]/(P_i)$, is isomorphic to $N^{[L_i:K]}$. Hence $L_{(N)}$ is diagonalizable.

#### Theorem 7 {#alg-viii-s14-thm-7 .statement}

Let A be a central simple K-algebra of finite degree and L a subalgebra of A. The following properties are equivalent:

(i) The algebra L is a maximal étale subalgebra of A.

(ii) There exist an extension $K'$ of K, an integer $n\geqslant 1$, and an isomorphism $\theta$ from $A_{(K')}$ to $\mathbf{M}_n(K')$ that sends $L_{(K')}$ to the set of diagonal matrices.

(iii) There exist $K',n$, and $\theta$ as in (ii), where the extension $K'$ is, moreover, assumed Galois and of finite degree.

It is clear that (iii) implies (ii).

If property (ii) holds, then $L_{(K')}$ is a maximal commutative subalgebra of $A_{(K')}$ (Proposition 6), and it is diagonalizable. The K-algebra L is then étale (V, §6, No. 3, p. 28, Definition 1), and it is a maximal commutative subalgebra of A (VIII, p. 261, Lemma 3, b)). We have proved that (ii) implies (i).

Suppose that property (i) holds. Since L is étale over K, by Proposition 7, there exists a Galois extension $K_1$ of K of finite degree such that the $K_1$-algebra $L_{(K_1)}$ is diagonalizable. The algebra A is central simple; by (VIII, p. 252, Theorem 1), there exist a Galois extension $K_2$, a vector space V of finite dimension $n$ over $K_2$, and an isomorphism $\theta$ from $A_{(K_2)}$ to End$_{K_2}(V)$. By Proposition 1 of V, p. 55, we may assume $K_1= K_2$. By Proposition 4, b) of VIII, p. 264 and Lemma 3, b) of VIII, p. 261$, L_{(K')}$ is a maximal commutative subalgebra of $A_{(K')}$, so $\theta (L_{(K')})$ is a maximal commutative subalgebra of End$_{K'}(V')$. Let us apply Proposition 6 to the diagonalizable algebra $\theta (L_{(K')}):$ there exists a basis $(e_1, . . . , e_n)$ of $V'$ over $K'$ such that $\theta (L_{(K')})$ consists of the endomorphisms of $V'$ with diagonal matrix with respect to this basis. So (i) implies (iii).

### Exercises {#alg-viii-s14-exercises}

See the [exercises for § 14](exercises/s14/).
