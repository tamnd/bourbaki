---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 13
section_title: Absolutely Semisimple Algebras
lang: en
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.229-A VIII.249
pdf_pages: 0246-0266
extraction: native
subsections:
    - "no": 1
      title: Absolutely Semisimple Modules
      page: 229
      pdf_page: 246
    - "no": 2
      title: Algebras over Separably Closed Fields
      page: 230
      pdf_page: 247
    - "no": 3
      title: Absolutely Semisimple Algebras
      page: 231
      pdf_page: 248
    - "no": 4
      title: Characterization of Absolutely Semisimple Modules
      page: 235
      pdf_page: 252
    - "no": 5
      title: Derivations on Semisimple Algebras
      page: 236
      pdf_page: 253
    - "no": 6
      title: Cohomology of Algebras
      page: 239
      pdf_page: 256
    - "no": 7
      title: Cohomology of Absolutely Semisimple Algebras
      page: 241
      pdf_page: 258
    - "no": 8
      title: The Splitting of Artinian Algebras
      page: 243
      pdf_page: 260
statements: 33
exercises: 12
content_sha256: 59ae315352da7756628996eb1d9ea3c29c736ace51438fd89f399e043fd09a4b
---

## § 13. ABSOLUTELY SEMISIMPLE ALGEBRAS

### 1. Absolutely Semisimple Modules

#### Definition 1 {#alg-viii-s13-def-1 .statement tag=00F9}

Let K be a commutative field and A a K-algebra. We call an A-module M absolutely semisimple if the $A_{(L)}$-module $M_{(L)}$ is semisimple for every extension L of K.

Every absolutely semisimple module is semisimple. Conversely, if the field K is perfect, then every semisimple A-module that is finite-dimensional over K is absolutely semisimple (VIII, p. 222, Corollary 1, a)) because every extension of a perfect field is separable (V, §7, No. 1, p. 36, Proposition 2).

#### Proposition 1 {#alg-viii-s13-prop-1 .statement tag=00FA}

Let K be a commutative field and A a K-algebra.

a) Every direct sum of absolutely semisimple A-modules is an absolutely semisimple A-module. Every submodule and quotient module of an absolutely semisimple module is absolutely semisimple.

b) Let M be an A-module and let L be an extension of the field K. The A-module M is absolutely semisimple if and only if the $A_{(L)}$-module $M_{(L)}$ is absolutely semisimple.

Assertion a) follows from the analogous assertion for semisimple modules (VIII, p. 56, Corollaries 1 and 3).

Suppose that the A-module M is absolutely semisimple, and let $L'$ be an extension of L. As an $A_{(L')}$-module, $L'\otimes_LM_{(L)}$ is isomorphic to $M_{(L')}$ (II, §5, No. 1, p. 273, Proposition 2); it is therefore a semisimple module. This proves that $M_{(L)}$ is absolutely semisimple.

Conversely, suppose that $M_{(L)}$ is absolutely semisimple. Let $L'$ be an extension of K. There exists a composite extension $(\Omega, u, v)$ of L and $L'$ (V, §2, No. 4, p. 13, Corollary); we identify L and $L'$ with subextensions of Ω. The $A_{(\Omega)}$-module $M_{(\Omega)}$ is isomorphic to $(M_{(L)})_{(\Omega)}$; it is therefore semisimple. But $M_{(\Omega)}$ is also isomorphic to $(M_{(L')})_{(\Omega)}$, and Proposition 8, a) of VIII, p. 222 implies that $M_{(L')}$ is semisimple. So M is absolutely semisimple.

#### Proposition 2 {#alg-viii-s13-prop-2 .statement tag=00FB}

Let K be a commutative field, A a K-algebra, and M an A-module that is finite-dimensional over K. The following properties are equivalent:

(i) The A-module M is absolutely semisimple.

(ii) There exists an extension P of K that is a perfect field such that the $A_{(P)}$-module $M_{(P)}$ is semisimple.

(iii) The A-module M is semisimple, and the center of its commutant is an étale algebra over the field K.

It is clear that (i) implies (ii). Assume that (ii) holds; then the $A_{(P)}$-module $M_{(P)}$ is absolutely semisimple by Corollary 1, a) of VIII, p. 222. By Proposition 1, b), M is then absolutely semisimple. Therefore, (ii) implies (i).

Suppose that M is semisimple. Let Z be the center of the commutant of M; it is a commutative algebra of finite degree over the field K. If L is an extension of K, then it follows from Proposition 8, b) of VIII, p. 222 that the $A_{(L)}$-module $M_{(L)}$ is semisimple if and only if the ring $Z_{(L)}$ is reduced. The equivalence of (i) and (iii) therefore follows from Theorem 4 of V, §6, No. 7, p. 34.

### 2. Algebras over Separably Closed Fields

#### Lemma 1 {#alg-viii-s13-lem-1 .statement tag=00FC}

Let D be a field and Z its center. Denote the characteristic exponent of Z by $p$. Suppose that for every element $a$ of D, there exists an integer $m\geqslant 0$ such that $a^{p^m}$ belongs to Z. Then the field D is commutative.

If $p= 1$, then D = Z. We therefore assume $p >1$.

Let us give a proof by contradiction and suppose that D is not commutative. Let $a$ be an element of D Z and $q$ a power of $p$ such that $a^q$ belongs to Z. Denote the identity mapping on D by I and the inner automorphism $x\mapsto axa^{-1}$ from D to D associated with $a$ by $\sigma$; we have $\sigma^q= I$ because $a^q$ belongs to Z. We have $\sigma -I\not= 0$ because $a$ does not belong to Z, and we have $(\sigma -I)^q=\sigma^q-I = 0$ because Z has characteristic $p$. Let $f$ be the greatest natural number such that $(\sigma -I)^f\not= 0$; we have $f\geqslant 1$. Choose an element $c$ of D such that $(\sigma -I)^f(c)\not= 0$, and set

$$
x= (\sigma -I)^{f-1}(c),y= (\sigma -I)(x) = (\sigma -I)^f(c)
$$

By construction, we have $y\not= 0$ and $\sigma (y) =y$; if we set $z=y^{-1}x$, then it follows that

$$
\sigma (z) =\sigma (y)^{-1}\sigma (x) =y^{-1}(y+x) = 1 +z
$$

and therefore $\sigma (z^{p^j}) = 1 +z^{p^j}$ for every natural number $j$. Choose an integer $m\geqslant 0$ such that $z^{p^m}$ belongs to the center Z of D; we have

$$
z^{p^m}=az^{p^m}a^{-1}=\sigma (z^{p^m}) = 1 +z^{p^m}
$$

This contradiction implies Lemma 1.

#### Proposition 3 {#alg-viii-s13-prop-3 .statement tag=00FD}

Let K be a separably closed field (V, §7, No. 8, p. 45, Definition 4), and let D be an algebra of finite degree over K that is a field. Then D is commutative.

Denote the characteristic exponent of K by $p$. Let $a$ be an element of D. The ring $K[a]$ is an algebraic extension of K (V, §3, No. 1, p. 17, Corollary 1). Since the field K is separably closed, it follows from V, §7, No. 7, p. 44, Proposition 13 that the algebra $K[a]$ is a $p$-radical extension of K. Hence there exists an integer $m\geqslant 0$ such that $a^{p^m}$ belongs to K. By Lemma 1, the field D is consequently commutative.

#### Corollary {#alg-viii-s13-n2-cor-1 .statement tag=00FE}

Let K be a separably closed field and A a semisimple algebra of finite degree over K. Then there exist an integer $r\geqslant 0$, strictly positive integers $n_1, . . . , n_r$, and extensions $K_1, . . . ,K_r$ of K of finite degree such that A is isomorphic to the algebra $\prod_i^r_{=1}\mathbf{M}_{n_i}(K_i)$.

By the structure theorem for semisimple algebras (VIII, p. 135, Theorem 1), A is isomorphic to an algebra $\prod^r_{i=1}\mathbf{M}_{n_i}(D_i)$, where $r$ is an integer $\geqslant 0,n_1, . . . , n_r$ are strictly positive integers, and $D_1, . . . ,D_r$ are K-algebras of finite degree that are fields. Since the field K is separably closed, each field $D_i$ is commutative by Proposition 3; the corollary follows.

### 3. Absolutely Semisimple Algebras

#### Definition 2 {#alg-viii-s13-def-2 .statement tag=00FF}

Let K be a commutative field. We say that a K-algebra A is absolutely semisimple if the ring $A_{(L)}$ is semisimple for every extension L of K.

An absolutely semisimple algebra is semisimple. The K-algebra A is absolutely semisimple if and only if the A-module $A_s$ is absolutely semisimple. By Proposition 1 of VIII, p. 229, we therefore obtain the following result: if L is an extension of K, then the L-algebra $A_{(L)}$ is absolutely semisimple if and only if the K-algebra A is absolutely semisimple.

#### Theorem 1 {#alg-viii-s13-thm-1 .statement tag=00FG}

Let K be a commutative field and A a K-algebra. The following properties are equivalent:

(i) The K-algebra A is absolutely semisimple.

(ii) The algebra A has finite degree over K, and there exists an extension P of K that is a perfect field, for which the P-algebra $A_{(P)}$ is semisimple.

(iii) The K-algebra A is semisimple and has finite degree over K, and its center is an étale K-algebra.

(iv) There exists a finite family $(n_i,D_i)_{i\in I}$, where $n_i$ is a strictly positive integer and $D_i$ a K-algebra of finite degree that is a field, such that the center $Z_i$ of $D_i$ is a separable extension of K for every $i\in I$ and A is isomorphic to the product of the matrix rings $\mathbf{M}_{n_i}(D_i)$.

(v) There exist an extension L of K and a finite family of integers $(n_i)_{i\in I}$ such that the L-algebra $A_{(L)}$ is isomorphic to the algebra $\prod_{i\in I}\mathbf{M}_{n_i}(L)$.

(vi) There exist a Galois extension L of K of finite degree and a finite family of integers $(n_i)$ such that $A_{(L)}$ is isomorphic to the product of the matrix algebras $\mathbf{M}_{n_i}(L)$.

We first prove the implications (v) $\Rightarrow$ (iv) $\Rightarrow$ (iii) $\Rightarrow$ (ii) $\Rightarrow$ (i). Denote the center of A by Z.

If property (v) holds, then the L-algebra $A_{(L)}$ is semisimple and has finite degree over L, and its center (isomorphic to $Z_{(L)}$, III, p. 41, Corollary) is isomorphic to $L^r$ for some integer $r\geqslant 0$. By Corollary 2, a) of VIII, p. 222, the algebra A is semisimple and has finite degree over K. It is therefore isomorphic to a finite product of rings $\prod_{i\in I}\mathbf{M}_{n_i}(D_i)$ with $n_i\geqslant 1$ for every $i\in I$, where the field $D_i$ is an algebra of finite degree over K. The center $Z_i$ of $D_i$ is a commutative field that is an extension of K, and Z is isomorphic to $\prod_{i\in I}Z_i$. Therefore, $Z_{(L)}$ is isomorphic, on the one hand, to $\prod_{i\in I}(Z_i)_{(L)}$ and, on the other hand, to $L^r$. In other words, the algebra $\prod_{i\in I}Z_i$ is étale over the field K (V, §6, No. 3, p. 28, Definition 1), and each of the extensions $Z_i$ is separable over K (V, §6, No. 4, p. 31, Corollary, and V, §7, No. 1, p. 42). So (v) implies (iv).

If property (iv) holds, then it is clear that A is a semisimple algebra and has finite degree over K. Its center Z is isomorphic to the product $\prod_{i\in I}Z_i$ of separable extensions of K of finite degree; it is therefore an étale algebra (loc. cit.). So (iv) implies (iii).

The implications (iii) $\Rightarrow$ (ii) $\Rightarrow$ (i) follow from Proposition 2 of VIII, p. 230 applied to the A-module $A_s$.

#### Lemma 2 {#alg-viii-s13-lem-2 .statement tag=00FH}

Let L be an algebraically closed field and D a field containing L in its center. If D is distinct from L, then there exists an extension $L'$ of L such that the ring $D\otimes_LL'$ is not left Artinian.

Let $x$ be an element of D L; since L is algebraically closed, the extension $L'= L(x)$ of L is not algebraic and $x$ is transcendent over L. The ring $B = L'\otimes_LL'$ is then an integral domain by Proposition 5 of V, §17, No. 4, p. 141.

The element $y=x\otimes 1-1\otimes x$ of B is not zero, but if $\varphi$ is the homomorphism from B to $L'$ that sends $\xi \otimes \eta$ to $\xi \eta$, then we have $\varphi (y) = 0$, so $y$ is not invertible in B. We view the ring $C = D\otimes_LL'$ as a right module over its subring B; it is a free module because D is a right vector space over its subfield $L'$. Since $y$ is a nonzero and noninvertible element of the integral domain B, right multiplication by $y$ in C is a mapping $R_y$ that is injective but not bijective. Now, $R_y$ is an endomorphism of the left C-module $C_s$; consequently (VIII, p. 28, Corollary 1), the ring C is not left Artinian.

Let us now prove that (i) implies (v). This is a consequence of the following lemma.

#### Lemma 3 {#alg-viii-s13-lem-3 .statement tag=00FI}

Let A be an absolutely semisimple K-algebra and L an algebraically closed extension of K. Then the algebra $A_{(L)}$ is isomorphic to a product of finitely many matrix algebras over L.

The L-algebra $A_{(L)}$ is semisimple; it is therefore isomorphic to a product of finitely many algebras of the form $\mathbf{M}_{n_i}(D_i)$, where $D_i$ is a field containing L in its center and $n_i$ an integer $\geqslant 1$ (VIII, p. 137, Remark 1).

Let $L'$ be an extension of L. Since the K-algebra A is absolutely semisimple, the ring $A_{(L')}$ is semisimple and therefore left Artinian. Now, the ring $A_{(L')}$ is isomorphic to $L'\otimes_LA_{(L)}$, hence to $\prod_{i\in I}\mathbf{M}_{n_i}(L'\otimes_LD_i)$; by Proposition 5 of VIII, p. 7, each of the rings $\mathbf{M}_{n_i}(L'\otimes_LD_i)$ is therefore left Artinian.

Let $n\geqslant 1$ be an integer and B a ring. Let $(\mathfrak{b}_r)_{r\geqslant 0}$ be a decreasing sequence of left ideals of B; denote by $\mathfrak{c}_r$ the set of square matrices of order $n$ with entries in $\mathfrak{b}_r$. Then $(\mathfrak{c}_r)_{r\geqslant 0}$ is a decreasing sequence of left ideals of $\mathbf{M}_n(B)$. In particular, if the ring $\mathbf{M}_n(B)$ is left Artinian, then so is B.

By the above, for every $i\in I$ and every extension $L'$ of L, the ring $D_i\otimes_LL'$ is left Artinian. By Lemma 2, we have $D_i= L$ for every $i\in I$, which implies Lemma 3.

We will use the following lemma to prove the implication (i)$\Rightarrow$(vi).

#### Lemma 4 {#alg-viii-s13-lem-4 .statement tag=00FJ}

Let A and B be algebras over the field K that have finite generating sets, and let $K'$ be an extension of K. If the $K'$-algebras $A_{(K')}$ and $B_{(K')}$ are isomorphic, then there exists a subextension L of $K'$, finitely generated over K, such that the L-algebras $A_{(L)}$ and $B_{(L)}$ are isomorphic.

Let $(e_i)_{i\in I}$ and $(f_j)_{j\in J}$ be finite generating sets for the algebras A and B, respectively. Let $u$ be an isomorphism from $A_{(K')}$ to $B_{(K')}$ and $v$ the inverse isomorphism; there exists a subextension L of $K'$, finitely generated over K, such that we have $u(1\otimes e_i)\in B_{(L)}$ for every $i\in I$ and $v(1\otimes f_j)\in A_{(L)}$ for every $j\in J$. Consequently, $u$ sends $A_{(L)}$ into $B_{(L)}$, and $v$ sends $B_{(L)}$ into $A_{(L)}$. The induced mappings $u': A_{(L)}\rightarrow B_{(L)}$ and $v': B_{(L)}\rightarrow A_{(L)}$ are ring homomorphisms; they are inverse bijections.

Let us complete the proof of the implication (i)$\Rightarrow$(vi). Let $K'$ be a separable closure of K (V, §7, No. 8, p. 45). Then $A_{(K')}$ is an absolutely semisimple algebra over $K'$. By the implication (i)$\Rightarrow$(iv), the $K'$-algebra $A_{(K')}$ is isomorphic to a product $\mathbf{M}_{n_1}(D_1)\times \cdots \times \mathbf{M}_{n_r}(D_r)$, where $D_i$ is a $K'$-algebra of finite degree that is a field whose center $Z_i$ is a separable extension of $K'$. Since $K'$ is separably closed, we have $Z_i= K'$. By Proposition 3 of VIII, p. 231, the field $D_i$ is commutative. We therefore have $D_i= K'$. We denote the K-algebra $\mathbf{M}_{n_1}(K)\times  \cdots  \times \mathbf{M}_{n_r}(K)$ by B. The $K'$-algebras $A_{(K')}$ and $B_{(K')}$ are isomorphic by the above. Every subextension of $K'$ that is finitely generated over K is separable and has finite degree over K, hence is contained in a subextension L of $K'$ that is Galois and of finite degree over K (V, §10, No. 1, p. 57, Proposition 2). The implication therefore follows from Lemma 4.

The implication (vi)$\Rightarrow$(v) is immediate.

#### Corollary 1 {#alg-viii-s13-lem-4-cor-1 .statement tag=00FK}

Let K be a commutative field, and let $A_1$ and $A_2$ be K-algebras. Suppose that $A_1$ is absolutely semisimple.

a) If $A_2$ is semisimple, then so is $A_1\otimes_KA_2$.

b) If $A_2$ is absolutely semisimple, then so is $A_1\otimes_KA_2$.

Denote the center of $A_1$ by $Z_1$ and that of $A_2$ by $Z_2$. The center Z of $A_1\otimes_KA_2$ is equal to $Z_1\otimes_KZ_2$ by the corollary of III, §4, No. 4, p. 468. Suppose that $A_2$ is semisimple; then $Z_2$ is a reduced algebra (VIII, p. 137, Propositions 2 and 3). By Theorem 1, $Z_1$ is an étale and therefore separable K-algebra. By Proposition 5 of V, §15, No. 2, p. 120, the ring $Z = Z_1\otimes_KZ_2$ is reduced; since $A_1$ has finite degree over K (Theorem 1), it follows from Proposition 7 of VIII, p. 221 that the ring $A_1\otimes_KA_2$ is semisimple.

Now suppose that $A_2$ is absolutely semisimple. Let L be an extension of K. Then the algebra $A_{1(L)}$ is absolutely semisimple, and the algebra $A_{2(L)}$ is semisimple. Therefore, by a), the algebra $A_1\otimes_KA_{2(L)}$ is semisimple.

#### Corollary 2 {#alg-viii-s13-lem-4-cor-2 .statement tag=00FL}

Let K be a separably closed field, and let A be an absolutely semisimple K-algebra. Then there exist an integer $r\geqslant 0$ and strictly positive integers $n_1, . . . , n_r$ such that the algebra A is isomorphic to the algebra $\prod_i^r_{=1}\mathbf{M}_{n_i}(K)$.

By Theorem 1, A is isomorphic to an algebra of the form $\prod^r_{i=1}\mathbf{M}_{n_i}(D_i)$ for an integer $r\geqslant 0$, integers $n_1, . . . , n_r$, and K-algebras of finite degree $D_1, . . . ,D_r$ that are fields and whose centers are separable extensions of K and therefore equal to K. By Proposition 3 of VIII, p. 231, we have $D_i= K$ for $i\in [1, r]$.

#### Example {#alg-viii-s13-n3-exa-1 .statement tag=00FM}

A commutative K-algebra is absolutely semisimple if and only if it is étale: this follows from the definition (V, §6, No. 3, p. 28, Definition 1) and the equivalence of properties (i) and (v) of Theorem 1.

### 4. Characterization of Absolutely Semisimple Modules

#### Proposition 4 {#alg-viii-s13-prop-4 .statement tag=00FN}

Let K be a commutative field and A a K-algebra.

a) Let M be a semisimple A-module. The A-module M is absolutely semisimple if and only if every simple module belonging to the support of M is.

b) Let S be a simple A-module, and let D be its commutant. The following properties are equivalent:

(i) The A-module S is absolutely semisimple.

(ii) The K-algebra D is absolutely semisimple.

(iii) The K-algebra D is a field, has finite degree over K, and its

center is a separable extension of K.

Assertion a) follows from Proposition 1, a) of VIII, p. 229. Let S and D be as in b), and let L be an extension of K. The $A_{(L)}$-module $S_{(L)}$ is semisimple if and only if the ring $D_{(L)}$ is (VIII, p. 222, Proposition 8, c)). This proves the equivalence of (i) and (ii), and that of (ii) and (iii) follows from Theorem 1 because D is a field.

#### Corollary {#alg-viii-s13-n4-cor-1 .statement tag=00RF}

Let K be a commutative field, let $A_1$ and $A_2$ be K-algebras, and let $M_1$ be an absolutely semisimple $A_1$-module and $M_2$ a semisimple $A_2$-module. Then $M_1\otimes_KM_2$ is a semisimple module over the ring $A_1\otimes_KA_2$.

The module $M_1$ is the direct sum of absolutely semisimple simple $A_1$-modules (Proposition 4). It therefore suffices to prove the assertion in the case when the modules $M_1$ and $M_2$ are simple. Denote their commutants by $D_1$ and $D_2$. The K-algebra $D_1$ is absolutely semisimple (loc. cit.); by Corollary 1 of VIII, p. 234, the K-algebra $D_1\otimes_KD_2$ is semisimple. It then follows from Corollary 1 of VIII, p. 215 that the $(A_1\otimes_KA_2$)-module $M_1\otimes_KM_2$ is semisimple.

### 5. Derivations on Semisimple Algebras

In this subsection and the next ones, K is a commutative ring, A a K-algebra, B the K-algebra $A\otimes_KA^o$, and $\varepsilon$ the K-linear mapping from B to A defined by $\varepsilon (x\otimes y) =xy$ for $x, y$ in A.

Recall (III, §4, No. 3, p. 467) that every $(A$, A)-bimodule P can be viewed as a left B-module, with external law given by $(a\otimes a')p=apa'$ for $a, a'$ in A and $p$ in P. Conversely, every B-module can be viewed as an $(A,A)$-bimodule. We endow A with its canonical $(A$, A)-bimodule structure and with the corresponding B-module structure; we endow B with the $(A$, A)-bimodule structure corresponding to the B-module $B_s$. We therefore have

$$
a(x\otimes y)a'= (a\otimes a')(x\otimes y) =ax\otimes ya'
$$

for $a, a', x, y$ in A, where the product $ya'$ is calculated in the algebra A.

The K-linear mapping $\varepsilon$ is a homomorphism of $(A$, A)-bimodules.

#### Proposition 5 {#alg-viii-s13-prop-5 .statement tag=00FO}

The following properties are equivalent:

(i) The B-module A is projective.

(ii) There exists an element $e$ of the $(A,A)$-bimodule B satisfying the following two conditions: $\varepsilon (e) = 1$ and $ae=ea$ for every $a\in A$.

The mapping $\varepsilon : B\rightarrow A$ is surjective because we have $\varepsilon (a\otimes 1) =a$ for every $a\in A$; it is a homomorphism of $(A$, A)-modules, hence a B-linear mapping. If the B-module A is projective, then there exists a section $s$ of $\varepsilon$ (II, §2, No. 2, p. 231, Proposition 4); it is a homomorphism of $(A$, A)-bimodules from A to B. If we set $e=s$(1), then we have $\varepsilon (e) =\varepsilon (s(1)) = 1$ and $ae=s(a) =ea$ for every $a\in A$. So (i) implies (ii).

Conversely, let $e$ be an element of B satisfying the conditions in item (ii). Define a mapping $s$ from A to B by the formula

$$
s(a) =ae=ea \tag{1}
$$

It is a homomorphism of $(A$, A)-modules, and we have $\varepsilon \circ s= 1_A$; in other words, $s$ is a B-linear section of the surjective mapping $\varepsilon$. Consequently, the B-module A is isomorphic to the direct factor submodule $s(A)$ of $B_s$ (II, §1, No. 9, p. 211, Proposition 15) and is therefore projective (II, §2, No. 2, p. 231, Proposition 4). This proves that (ii) implies (i).

#### Remark 1 {#alg-viii-s13-n5-rem-1 .statement tag=00FP}

Let $e=\sum^r_{i=1}a_i\otimes a'_i$ be an element of B. The conditions in item (ii) of Proposition 5 translate to the formulas

$$
\sum_{i=1}^ra_ia'_i= 1 \tag{2}
$$

(3) $\sum_{i=1}^raa_i\otimes a'_i=\sum_{i=1}^ra_i\otimes a'_ia$ for every $a\in A$.

When they are satisfied, $e$ is an idempotent in B. Indeed, we then have the relations

$$
e^2=\sum_{i=1}^ra_iea'_i=\sum_{i=1}^rea_ia'_i=e
$$

#### Remark 2 {#alg-viii-s13-n5-rem-2 .statement tag=00FQ}

Let K be a commutative field, let A be a K-algebra, and let M be an A-module. The group End$_K(M)$ is endowed with an $(A$, A)-bimodule structure defined by

$$
aua'(x) =au(a'x)
$$

for every $a, a'\in A$, every $u\in$ End$_K$(M), and every $x\in M$. We endow it with the associated B-module structure. Let $e=\sum^r_{i=1}a_i\otimes a'_i$ be an element of B satisfying the conditions in part (ii) of Proposition 5, so also relations (2) and (3). If $p\in$ End$_K(M)$ is a projector whose image N is an A-submodule of M, then $ep$ is an A-linear projector with the same image.

Indeed, the image of $ep$ is contained in N. If $x$ belongs to N, then so does $a'_ix$, so that we have $p(a'_ix) =a'_ix$ and

$$
ep(x) =\sum_{i=1}^ra_ia'_ix=x
$$

by formula (2). We deduce from formula (3) that $aep(x) =ep(ax)$ for every $a\in A$ and every $x\in M$, which proves that $ep$ is A-linear.

#### Theorem 2 {#alg-viii-s13-thm-2 .statement tag=00RG}

Let K be a commutative field and A a K-algebra. The following properties are equivalent:

(i) The K-algebra A is absolutely semisimple.

(ii) The K-algebra $B = A\otimes_KA^o$ is semisimple.

(iii) The B-module A is projective.

(iv) There exists an element $e$ of the $(A,A)$-bimodule B satisfying $\varepsilon (e) = 1$ and $ae=ea$ for every $a\in A$.

Suppose that the algebra A is absolutely semisimple, hence semisimple. Then the algebra $A^o$ is semisimple (VIII, p. 137, Proposition 2), and it follows from Corollary 1 of VIII, p. 234 that $B = A\otimes_KA^o$ is a semisimple K-algebra. Therefore, (i) implies (ii).

Since every module over a semisimple ring is projective (VIII, p. 138, Proposition 4), (ii) implies (iii).

The equivalence of (iii) and (iv) follows from Proposition 5. To complete the proof, let us show that (iv) implies (i). Let $e=\sum^r_{i=1}a_i\otimes a'_i$ be an element of B satisfying the conditions in item (ii) of Proposition 5. Let L be an extension of the field K; we must prove that the ring $A_{(L)}$ is semisimple or, equivalently, that every $A_{(L)}$-module is semisimple (VIII, p. 138, Proposition 4). Let M be an $A_{(L)}$-module, and let N be a submodule of M; we view M as a left $(A$, L)-bimodule and N as a sub-bimodule (III, §4, No. 3, p. 466). Since L is a field, there exists an L-linear projector $u$ in M with image N. Since the homotheties $a_M$ associated with the elements $a$ of A are L-linear, there exists a unique group homomorphism from $A\otimes_KA^o$ to End$_L(M)$ that sends an element $a\otimes a'$ to the L-linear mapping $x\mapsto au(a'x)$. We denote the image of $e$ by this homomorphism by $v$; it follows from Remark 2 that $v$ is an $A_{(L)}$-linear projector with image N. The kernel of $v$ is an $A_{(L)}$-submodule of M, supplementary to N. By Corollary 2 of VIII, p. 56, the $A_{(L)}$-module M is semisimple.

#### Remark 3 {#alg-viii-s13-n5-rem-3 .statement tag=00FR}

We know (VIII, p. 234, Corollary 1) that the tensor product of two absolutely semisimple algebras over a commutative field is absolutely semisimple. Consequently, if the algebra A is absolutely semisimple, then so is the algebra $B = A\otimes_KA^o$.

### 6. Cohomology of Algebras

In this subsection, K is a commutative ring, A a K-algebra, B the K-algebra $A\otimes_KA^o$, and $\varepsilon$ the K-linear mapping from B to A defined by $\varepsilon (x\otimes y) =$ $xy$ for $x, y$ in A. For $n\in \mathbf{N}$, we denote the tensor product over K of $n+ 2$ copies of the K-module A by $B_n$. We view it as an $(A$, A)-bimodule (and also as a B-module); we endow it with the structure of a left A-module deduced from the left A-module structure of the first factor of the tensor product and with the structure of a right A-module deduced from the right A-module structure of the last factor. In particular, $B_0$ is just the $(A$, A)-bimodule B.

For every integer $n\geqslant 1$, we define homomorphisms of bimodules $d_n^i$ for $i\in [0, n]$ and $d_n$ from $B_n$ to $B_{n-1}$ by the formulas (4) $d_n^i(x_0\otimes  \cdots  \otimes x_{n+1}) =x_0\otimes  \cdots  \otimes x_ix_{i+1}\otimes  \cdots  \otimes x_{n+1}$ for $i\in [0, n]$ and

$$
d_n=\sum_{i=0}^n(-1)^id_n^i \tag{5}
$$

We denote the mapping $\varepsilon : B_0\rightarrow A$ by $d_0=d^0_0$.

Let $n$ be an integer $\geqslant 1$. For $0\leqslant i < j\leqslant n$, we have (6) $d_n^i_{-1}\circ d_n^j=d_n^{j-}_-^1_1\circ d_n^i$, and from this we deduce

$$
d_{n-1}\circ d_n=\sum(-1)^{i+j}d_n^i_{-1}\circ d_n^j+\sum(-1)^{i+j}d_n^i_{-1}\circ d_n^j
$$

$$
=^0_0^{\leqslant}_{\leqslant}\sum^{i<j}_{i<j}^{\leqslant}_{\leqslant}^n_n(-1)^{i+j}d_n^{j-}_-^1_1\circ d_n^i+^0_0^{\leqslant}_{\leqslant}^j_j^{\leqslant}_{\leqslant}\sum^i_i^{\leqslant}_{\leqslant}^n_n^-_-^1_1(-1)^{i+j}d_n^i_{-1}\circ d_n^j
$$

and consequently (7) $d_{n-1}\circ d_n= 0$.

Let P be an $(A$, A)-bimodule. For any integer $n\geqslant 0$, we denote the K-module of K-multilinear mappings from $A^n$ to P by $C^n(A,P)$. The mapping $\alpha^n: C^n(A,P)\rightarrow$ Hom$_B(B_n,P)$ that sends $f\in C^n(A,P)$ to the homomorphism $\alpha^n(f)$ characterized by (8) $\alpha^n(f) (x_0\otimes  \cdots  \otimes x_{n+1}) =x_0f(x_1, . . . , x_n)x_{n+1}$ is an isomorphism of K-modules.

We denote by $\partial^n$ (for $n\geqslant 0)$ the unique K-linear mapping from $C^n(A,P)$ to $C^{n+1}(A,P)$ that makes the following diagram commutative:

$C_n(A,P)\partial^{^n}$ // $C_{n+1}(A,P)$

$\alpha^n\alpha^{n+1}$

Hom$_B(B_n,P)^{Hom(d_{n+1},1_P)}/$/ Hom$_B(B_{n+1},P)$.

By definition, we therefore have (9) $(\alpha^{n+1}\circ \partial^n)(f) =\alpha^n(f)\circ d_{n+1}$ for every $f\in C^n(A,P)$. In other words, we have

$$
\partial^n(f) (x_0, . . . , x_n) =\alpha^n(f) (d_{n+1}(1\otimes x_0\otimes  \cdots  \otimes x_n\otimes 1))
$$

for $x_0, . . . , x_n$ in A and $f$ in $C^n(A,P)$, that is,

$$
\partial^n(f)(x_0, . . . , x_n) =x_0f(x_1, . . . , x_n) \tag{10}
$$

$$
+^n\sum_{i=0}^{-1}(-1)^{i+1}f(x_0, . . . , x_{i-1}, x_ix_{i+1}, x_{i+2}, . . . , x_n)
$$

$$
+ (-1)^{n+1}f(x_0, . . . , x_{n-1})x_n
$$

By (7) and (9), we have (11) $\partial^{n+1}\circ \partial^n= 0$ for every $n\geqslant 0$.

We denote the K-module Ker $\partial^0$ by $H^0(A,P)$ and, for $n\geqslant 1$, the K-module Ker $\partial^n/$ Im $\partial^{n-1}$ by $H^n(A,P)$. We identify the K-module $C^0(A,P)$ with P, and we have $C^1(A,P) =$ Hom$_K(A,P)$. The mappings $\partial^n$ for $n\leqslant 2$ are given by the formulas (12) $\partial^0(p)(a) =ap-pa$ for every $p\in P$, (13) $\partial^1(f)(a, a') =af(a')-f(aa') +f(a)a'$ for $f\in C^1(A,P)$, (14) $\partial^2(f)(a, a', a'') =af(a', a'')-f(aa', a'') +f(a, a'a'')-f(a, a')a''$ for $f\in C^2(A,P)$.

So $H^0(A,P)$ is the K-submodule of P consisting of the elements $p$ such that $ap=pa$ for every $a\in A$, and $H^1(A,P)$ is the quotient of the K-module Der$_K(A,P)$ of K-derivations from A to P (III, §10, No. 2, p. 553) by the K-submodule consisting of the derivations of the form $a\mapsto ap-pa$ with $p\in P$ (called inner derivations).

### 7. Cohomology of Absolutely Semisimple Algebras

#### Proposition 6 {#alg-viii-s13-prop-6 .statement tag=00FS}

Let K be a commutative ring and A a K-algebra. Let $e=\sum^r_{i=1}a_i\otimes a'_i$ be an element of $B = A\otimes_KA^o$ satisfying the conditions in item (ii) of Proposition 5 of VIII, p. 236. For any integer $n\geqslant 1$ and any element $f$ of $C^n(A,P)$, we denote by $\gamma^n(f)$ the element of $C^{n-1}(A,P)$ defined by the formula

$$
\gamma^n(f)(x_1, . . . , x_{n-1}) =\sum_{i=1}^ra_if(a'_i, x_1. . . , x_{n-1}) \tag{15}
$$

We then have (16) $\partial^{n-1}(\gamma^n(f)) +\gamma^{n+1}(\partial^n(f)) =f$ for every integer $n\geqslant 1$ and every $f\in C^n(A,P)$.

#### Remark 1 {#alg-viii-s13-n7-rem-1 .statement tag=00SF}

$*$The morphisms $\partial_n: C_n(A,P)\rightarrow C_{n+1}(A,P)$ define a complex $(C(A,P), \partial )$ of K-modules (X, §2, n$^o1$, p. 24). The mapping $\gamma_n$ therefore defines a homotopy from this complex to itself linking 0 to Id$_{C(A,P)}$ (X, §2, n$^o4$, p. 32, définition $4).*$

We keep the notation of No.6. For every integer $n\geqslant 0$, we define a mapping $h_n: B_n\rightarrow B_{n+1}$ by the formula

$$
h_n(x) =d^1_{n+2}(e\otimes x) =\sum_{i=1}^ra_i\otimes a'_ix
$$

It is a homomorphism of $(A$, A)-bimodules (formula (3)).

#### Lemma 5 {#alg-viii-s13-lem-5 .statement tag=00FT}

We have the relation (17) $d_{n+1}\circ h_n+h_{n-1}\circ d_n= 1_{B_n}$ for every $n\geqslant 1$.

Let $x\in B_n$; we have

$$
(d_{n+1}\circ h_n)(x) = (d_{n+1}\circ d^1_{n+2})(e\otimes x)
$$

$$
= (d^0_{n+1}\circ d^1_{n+2})(e\otimes x)-^n\sum_{i=2}^{+2}(-1)^i(d_n^{i-}_{+1}^1\circ d^1_{n+2})(e\otimes x)
$$

so, by formula (6),

$$
(d_{n+1}\circ h_n)(x) = (d^0_{n+1}\circ d^0_{n+2})(e\otimes x)-^n\sum_{i=2}^{+2}(-1)^i(d^1_{n+1}\circ d_n^i_{+2})(e\otimes x)
$$

But we have

$$
(d^0_{n+1}\circ d^0_{n+2})(e\otimes x) =\varepsilon (e)x=x
$$

by property (ii) of Proposition 5 of VIII, p. 236 and, for $i\geqslant 2$,

$$
d^i_{n+2}(e\otimes x) =e\otimes d^i_n^{-2}(x)
$$

which gives

$$
(d_{n+1}\circ h_n)(x) =x-d^1_{n+1}(e\otimes d_n(x)) =x-h_{n-1}\circ d_n(x)
$$

and therefore formula (17).

We can finish the proof of Proposition 6 using Lemma 5. Let $n$ be an integer $\geqslant 1$ and $f$ an element of $C^n(A,P)$. By construction, we have

$$
\alpha^{n-1}(\gamma^n(f)) =\alpha^n(f)\circ h_{n-1} \tag{18}
$$

and, consequently, by formulas (9) and (18),

$$
\alpha^n(\partial^{n-1}(\gamma^n(f)) +\gamma^{n+1}(\partial^n(f))) =\alpha^{n-1}(\gamma^n(f))\circ d_n+\alpha^{n+1}(\partial^n(f))\circ h_n
$$

$$
=\alpha^n(f)\circ h_{n-1}\circ d_n+\alpha^n(f)\circ d_{n+1}\circ h_n
$$

$$
=\alpha^n(f)
$$

where the last equality follows from (17). Since $\alpha^n$ is bijective, the proposition follows.

#### Theorem 3 {#alg-viii-s13-thm-3 .statement tag=00FU}

Let K be a commutative ring, A a K-algebra, and P an $(A,A)$-bimodule. Suppose that the $(A\otimes_KA^o)$-module A is projective. We then have $H^n(A,P) = 0$ for every integer $n\geqslant 1$.

We must prove that for every integer $n\geqslant 1$, every element $f$ of $C^n(A,P)$ with $\partial^n(f) = 0$ is of the form $\partial^{n-1}(g)$ for an element $g$ of $C^{n-1}(A,P)$. By Proposition 5, this is an immediate consequence of Proposition 6.

#### Corollary {#alg-viii-s13-n7-cor-1 .statement tag=00FV}

Every K-derivation from A to P is inner.

This is a translation of the equality $H^1(A,P) = 0$.

#### Remark 2 {#alg-viii-s13-n7-rem-2 .statement tag=00FW}

The assumptions of Theorem 3 are, in particular, satisfied when K is a field and A an absolutely semisimple K-algebra (VIII, p. 238, Theorem 2).

#### Remark 3 {#alg-viii-s13-n7-rem-3 .statement tag=00FX}

Suppose that the K-module A is projective. Theorem 3 can also be proved as follows. The complex $(\bigoplus_{n\geqslant 0}B_n, d)$ and the homomorphism $\varepsilon : B_0\rightarrow A$ define a projective resolution of the B-module A; therefore, for every $n\geqslant 0$, the K-module $H^n(A,P)$ is isomorphic to Ext$^n_B(A,P)$ (X, §6, n$^o1$, p. 100, théorème 1). If the B-module A is projective, then the K-modules Ext$^n_B(A,P)$ are zero for $n\geqslant 1$ (X, §5, n$^o3$, p. 88, corollaire de la proposition 5), which implies that $H^n(A,P)$ is zero. Conversely, if $H^1(A,P)$ is zero for every $(A$, A)-bimodule P, then the B-module A is projective (X, §5, n$^o5$, p. 93, proposition $10).*$

### 8. The Splitting of Artinian Algebras

In this subsection, K is a commutative ring and A a K-algebra. Let $\mathfrak{r}$ be the radical of A. We denote the quotient algebra $A/\mathfrak{r}$ by A and the canonical mapping from A to A by $\pi$. We are interested in the subalgebras S of A such that $A = S\oplus \mathfrak{r}$.

We denote by Σ the set of K-linear sections $s$ of $\pi$ satisfying $s(\alpha \beta ) =$ $s(\alpha )s(\beta )$ for $\alpha , \beta$ in A. Note that such a section necessarily satisfies $s(1) = 1$ (in other words, $s$ is a ring homomorphism): we indeed have $s(1)^2=s$(1), and $s(1)$ is invertible because it belongs to $1 +\mathfrak{r}$ (VIII, p. 156, Theorem 1). If $s$ is an element of Σ, then the image S of $s$ is a subalgebra of A, and we have $A = S\oplus \mathfrak{r}$. Conversely, if S is a subalgebra of A such that $A = S\oplus \mathfrak{r}$, then the restriction of $\pi$ to S is bijective, and the inverse bijection defines an element of Σ with image S.

By Jacobson’s theorem (loc. cit.), every element of $1 +\mathfrak{r}$ is invertible in A. We call an inner automorphism of A of the form $a\mapsto xax^{-1}$ with $x\in 1 +\mathfrak{r}$ a special automorphism.

#### Proposition 7 {#alg-viii-s13-prop-7 .statement tag=00FY}

Suppose that the $(A\otimes_KA^o)$-module A is projective.

a) Let $S_1$ and $S_2$ be subalgebras of A satisfying $A = S_1\oplus \mathfrak{r}= S_2\oplus \mathfrak{r}$. There exists a special automorphism of A transforming $S_1$ into $S_2$.

b) Suppose that $\pi$ has a K-linear section and that the radical $\mathfrak{r}$ of A is nilpotent. Then there exists a subalgebra S of A satisfying $A = S\oplus \mathfrak{r}$.

Let $S_1$ and $S_2$ be as in a). Let $s_1$ and $s_2$ be the elements of the set Σ corresponding to the subalgebras $S_1$ and $S_2$. Let $\varepsilon$ be the K-linear mapping from $A\otimes_KA$ to A given by $\varepsilon (a\otimes b) =ab$. By Proposition 5 of VIII, p. 236 and Remark 1 of VIII, p. 237, there exists an element $e=\sum^r_{i=1}\alpha_i\otimes \alpha '_i$ of $A\otimes_KA$ satisfying $\sum^r_{i=1}\alpha_i\alpha '_i= 1$ and $\sum^r_{i=1}\alpha \alpha_i\otimes \alpha '_i=\sum^r_{i=1}\alpha_i\otimes \alpha '_i\alpha$ for every $\alpha \in A$. Set $x=\sum^r_{i=1}s_1(\alpha_i)s_2(\alpha '_i)$. We have $\pi (x) =\sum^r_{i=1}\alpha_i\alpha '_i= 1$ and therefore $x\in 1 +\mathfrak{r}$. Let $\alpha$ be an element of A. We have

$$
s_1(\alpha )x=\sum_{i=1}^rs_1(\alpha \alpha_i)s_2(\alpha '_i) = (\varepsilon \circ (s_1\otimes s_2))\sum_{i=1}^r\alpha \alpha_i\otimes \alpha '_i
$$

$$
= (\varepsilon \circ (s_1\otimes s_2))\sum_{i=1}^r\alpha_i\otimes \alpha '_i\alpha =\sum_{i=1}^rs_1(\alpha_i)s_2(\alpha_i'\alpha ) =xs_2(\alpha )
$$

The equality $x^{-1}S_1x= S_2$ follows, giving assertion a).

Under the assumptions of b), suppose furthermore that $\mathfrak{r}^2= 0$. In this case, the $(A$, A)-bimodule $\mathfrak{r}$ is annihilated by $\mathfrak{r}$, and we therefore view it as an $(A$, A)-bimodule. Choose a K-linear section $\sigma$ of $\pi$. We have (19) $\alpha x=\sigma (\alpha )x$ and $x\alpha =x\sigma (\alpha )$ for $\alpha \in A$ and $x\in \mathfrak{r}$. Set (20) $\varphi (\alpha , \beta ) =\sigma (\alpha \beta )-\sigma (\alpha )\sigma (\beta )$ for $\alpha , \beta \in A$. We have the relation $\pi (\varphi (\alpha , \beta )) =\alpha \beta -\alpha \beta = 0$ for $\alpha , \beta \in A$. Therefore, $\varphi$ defines an element of $C^2(A,\mathfrak{r})$. Let $\alpha , \beta , \gamma$ be elements of A; in view of (19), we have

$$
\partial^2\varphi (\alpha , \beta , \gamma ) =\alpha \varphi (\beta , \gamma )-\varphi (\alpha \beta , \gamma ) +\varphi (\alpha , \beta \gamma )-\varphi (\alpha , \beta )\gamma
$$

$$
=\sigma (\alpha )\varphi (\beta , \gamma )-\varphi (\alpha \beta , \gamma ) +\varphi (\alpha , \beta \gamma )-\varphi (\alpha , \beta )\sigma (\gamma )
$$

$$
=\sigma (\alpha )(\sigma (\beta \gamma )-\sigma (\beta )\sigma (\gamma ))-\sigma (\alpha \beta \gamma ) +\sigma (\alpha \beta )\sigma (\gamma ) +\sigma (\alpha \beta \gamma )
$$

$$
-\sigma (\alpha )\sigma (\beta \gamma )-(\sigma (\alpha \beta )-\sigma (\alpha )\sigma (\beta ))\sigma (\gamma )
$$

$$
= 0
$$

By Theorem 3 of VIII, p. 242, the K-module $H^2(A,\mathfrak{r})$ is reduced to zero. Hence there exists an element $\psi$ of $C^1(A,\mathfrak{r})$ such that $\partial^1\psi =\varphi$, in other words, such that we have (21) $\varphi (\alpha , \beta ) =\alpha \psi (\beta )-\psi (\alpha \beta ) +\psi (\alpha )\beta$ for $\alpha , \beta$ in $A$. We have $\psi (\alpha )\psi (\beta ) = 0$ because $\mathfrak{r}^2$ is zero; from (19) and (20), we then deduce (22) $(\sigma +\psi )(\alpha \beta ) = (\sigma +\psi )(\alpha )(\sigma +\psi )(\beta )$, so that the K-linear section $\sigma +\psi$ of $\pi$ belongs to Σ. Its image is a subalgebra S of A such that $A = S +\mathfrak{r}$.

Let us now prove the existence of S in the general case. We reason by induction on the least integer $p\geqslant 1$ such that $\mathfrak{r}^p= 0$; the case $p= 1$ is trivial. Suppose $p\geqslant 2$, and set $A'= A/\mathfrak{r}^{p-1}$. The radical $\mathfrak{r}'$ of $A'$ is equal to $\mathfrak{r}/\mathfrak{r}^{p-1}$ (Proposition 5 of VIII, p. 155), so satisfies $\mathfrak{r}'^{p-1}= 0$, and the algebra $A'/\mathfrak{r}'$ is isomorphic to $A = A/\mathfrak{r}$ and is therefore absolutely semisimple. By the induction hypothesis, there exists a subalgebra $S'$ of $A'$ such that $A'= S'\oplus \mathfrak{r}'$. Then $S'$ is of the form $A''/\mathfrak{r}^{p-1}$, where $A''$ is a subalgebra of A containing $\mathfrak{r}^{p-1}$, and we have (23) $A = A''+\mathfrak{r},\mathfrak{r}^{p-1}= A''\cap \mathfrak{r}$.

The algebra $A''/\mathfrak{r}^{p-1}$ is isomorphic to $A'/\mathfrak{r}'$; we have $(\mathfrak{r}^{p-1})^2= 0$, so $\mathfrak{r}^{p-1}$ is the radical of $A''$. By the case we just treated, there exists a subalgebra S of $A''$ such that $A''= S\oplus \mathfrak{r}^{p-1}$; we deduce the relation $A = S\oplus \mathfrak{r}$ from (23).

#### Corollary 1 {#alg-viii-s13-prop-7-cor-1 .statement tag=00S8}

Let K be a commutative field, A a K-algebra, and $\mathfrak{r}$ the radical of A. Suppose that the K-algebra $A/\mathfrak{r}$ is absolutely semisimple.

a) Let $S_1$ and $S_2$ be subalgebras of A satisfying $A = S_1\oplus \mathfrak{r}= S_2\oplus \mathfrak{r}$. There exists a special automorphism of A transforming $S_1$ into $S_2$.

b) If $\mathfrak{r}$ is nilpotent, then there exists a subalgebra S of A satisfying A = $S\oplus \mathfrak{r}$.

This follows from Proposition 7 and Theorem 2 of VIII, p. 238.

#### Corollary 2 {#alg-viii-s13-prop-7-cor-2 .statement tag=00FZ}

Let A be a commutative algebra of finite degree over a perfect field K, and let $\mathfrak{r}$ be its radical. There exists a unique subalgebra S of A such that $A = S\oplus \mathfrak{r}$. Moreover, S is isomorphic to a product of finitely many extensions of K of finite degree.

The K-algebra $A/\mathfrak{r}$ is semisimple (VIII, p. 173, Proposition 1) and has finite degree; it is absolutely semisimple because the field K is perfect (VIII, p. 232, Theorem 1). Since the ideal $\mathfrak{r}$ is nilpotent and A is commutative, the existence and uniqueness of S then follow from Corollary 1. Since S is semisimple and commutative and has finite degree, the last assertion is a consequence of Proposition 3 of VIII, p. 137.

#### Remark 1 {#alg-viii-s13-n8-rem-1 .statement tag=00G0}

The assumption that $A/\mathfrak{r}$ is absolutely semisimple is essential in Corollary 1 (VIII, p. 246, Exercise 4).

#### Remark 2 {#alg-viii-s13-n8-rem-2 .statement tag=00G1}

Suppose that A is an Artinian algebra over the field K. If A is commutative, then we can show (VIII, p. 180, Exercise 9) that A is isomorphic to a product of algebras $A_1\times  \cdots  \times A_n$ such that $A_i/\mathfrak{R}(A_i)$ is a field for every $i$. Conversely, if A is not commutative, then A may not be isomorphic to a product of algebras $A_1\times  \cdots  \times A_n$ such that $A_i/\mathfrak{R}(A_i)$ is a simple ring for every $i$ (VIII, p. 247, Exercise 5).

### Exercises {#alg-viii-s13-exercises}

See the [exercises for § 13](exercises/s13/).
