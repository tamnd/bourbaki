---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 5
section_title: Commutation
lang: en
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.77-A VIII.94
pdf_pages: 0094-0111
extraction: native
subsections:
    - "no": 1
      title: The Commutant and Bicommutant of a Module
      page: 77
      pdf_page: 94
    - "no": 2
      title: Generating Modules
      page: 79
      pdf_page: 96
    - "no": 3
      title: The Bicommutant of a Generating Module
      page: 82
      pdf_page: 99
    - "no": 4
      title: The Countermodule of a Semisimple Module
      page: 84
      pdf_page: 101
    - "no": 5
      title: Density Theorem
      page: 88
      pdf_page: 105
    - "no": 6
      title: Application to Field Theory
      page: 89
      pdf_page: 106
statements: 30
exercises: 19
content_sha256: 66b6ffbb6b84286a4e95ac9d19db760b048d32b7a64451a279c4a9abd3faa5b3
---

## § 5. COMMUTATION

### 1. The Commutant and Bicommutant of a Module

Let E be a ring and B a subset of E. The commutant (or centralizer) of B in E is the subring $B'$ of E consisting of the elements that commute with every element of B. The commutant $B''$ of $B'$ is called the bicommutant (or bicentralizer) of B. We have $B\subset B''$, and $B'$ coincides with its bicommutant (III, §1, No. 2, p. 429). The center of a subring B of E is $B\cap B'$; the common center of $B'$ and $B''$ is $B'\cap B''$. If B is a commutative subring of E, then we have $B\subset B'$, and $B''$ is the center of $B'$ (III, §1, No. 2, p. 430).

Let A be a ring and M a left (resp. right) A-module. Let us apply these definitions to the case when E is the endomorphism ring of the additive group of M and B the ring of homotheties $A_M$ of M. The commutant $A'_M$ of $A_M$ in E is called the commutant of M; it is the endomorphism ring of the A-module M. The bicommutant $A''_M$ of $A_M$ in E is called the bicommutant of M; it is the endomorphism ring of the countermodule of M (VIII, p. 8, Definition 3). We have $A_M\subset A''_M$, the ring $A_M\cap A'_M$ is the center of $A_M$, and $A'_M\cap A''_M$ is the common center of $A'_M$ and $A''_M$.

#### Definition 1 {#alg-viii-s5-def-1 .statement}

The A-module M is balanced if we have $A_M= A''_M$.

If the A-module M is balanced, then the rings $A_M$ and $A'_M$ have the same center $A_M\cap A'_M$. The module M is a balanced A-module if and only if it is a balanced $A_M$-module. The countermodule of an A-module M is faithful and balanced.

When the ring A is commutative, the bicommutant $A''_M$ of M is the center of $A'_M=$ End$_A(M)$; that M is balanced means that the center of End$_A(M)$ is reduced to the homotheties.

For any element $a$ of A, denote by $\boldsymbol{\delta }_a$ the right homothety $x\mapsto xa$ from A to A and by $\boldsymbol{\gamma }_a$ the left homothety $x\mapsto ax$ (I, §8, No. 1, p. 97). The map $a\mapsto \boldsymbol{\delta }_a$ is a ring isomorphism from $A^o$ to the commutant of the left A-module $A_s$ (cf. II, §10, No. 7, p. 349, applied to $I =\{1\})$. The map $a\mapsto \boldsymbol{\gamma }_a$ is a ring isomorphism from A to the commutant of the right A-module $A_d$ (loc. cit.). If we identify A with the commutant of $A_d$ through this map, then the countermodule of $A_d$ is identified with $A_s$; consequently, the A-module $A_d$ is balanced. Likewise, the A-module $A_s$ is balanced.

Let $n$ be an integer $\geqslant 1$. We view $A^n$ as a left $\mathbf{M}_n$(A)-module (loc. cit.). The mapping that sends $m\in \mathbf{M}_n(A)$ to the endomorphism $x\mapsto mx$ of the A-module $A^n_d$ is a ring isomorphism from $\mathbf{M}_n(A)$ to the commutant of the right A-module $A^n_d$ (loc. cit.).

#### Proposition 1 {#alg-viii-s5-prop-1 .statement}

Let $(A_i)_{i\in I}$ be a family of rings, and for every $i\in I$, let $M_i$ be an $A_i$-module. Set $A =\prod A_i,M =\prod M_i$, and $N =\bigoplus M_i$. Endow M with the structure of an A-module with law of action $((a_i),(x_i))\mapsto (a_ix_i)$. The set N is an A-submodule of M.

a) The mapping $(u_i)\mapsto \prod u_i$ from $\prod$ End$_{\mathbf{Z}}(M_i)$ to End$_{\mathbf{Z}}(M)$ (II, §1, No. 5, p. 200) restricts to ring isomorphisms from $\prod(A_i)_{M_i},\prod(A_i)'_{M_i}$, and $\prod(A_i)''_{M_i}$ to $A_M,A'_M$, and $A''_M$, respectively.

b) The mapping $(u_i)\mapsto \bigoplus u_i$ from $\prod$ End$_{\mathbf{Z}}(M_i)$ to End$_{\mathbf{Z}}(N)$ (II, §1, No. 6, p. 203) restricts to ring isomorphisms from $\prod(A_i)_{M_i},\prod(A_i)'_{M_i}$, and $\prod(A_i)''_{M_i}$ to $A_N,A'_N$, and $A''_N$, respectively.

The ring isomorphisms defined in Proposition 1 are called canonical. The product $\prod(A_i)_{M_i}$ is often identified with $A_M$, and $\prod(A_i)'_{M_i}$ with $A'_M$, etc., through these isomorphisms.

The mapping $\varphi : (u_i)\mapsto \prod u_i$ from $\prod$ End$_{\mathbf{Z}}(M_i)$ to End$_{\mathbf{Z}}(M)$ is an injective ring homomorphism. By the definition of the A-module structure on M, we have $\varphi (\prod(A_i)_{M_i}) = A_M$. Let $u\in A'_M$. For every $i\in I$, denote by $h_i$ the element of A with all components equal to 1 except that of index $i$, which is equal to 0 . If $x$ is an element of M with component of index $i$ equal to 0, then we have $x=h_ix$, and therefore pr$_i(u(x)) =$ pr$_i(u(h_ix)) =$ pr$_i(h_iu(x)) = 0$. Consequently, there exists a unique group homomorphism $u_i: M_i\mapsto M_i$ such that pr$_i(u(y)) =u_i$(pr$_i(y))$ for every $y\in M$. We have $u=\prod u_i$. Since the mapping $u$ is A-linear, the mapping $u_i$ is $A_i$-linear for every $i\in I$. This proves that the image of $\prod(A_i)'_{M_i}$ under $\varphi$ contains $A'_M$; the reverse inclusion is obvious. By applying this to the countermodule of M, we deduce that $\varphi$ induces an isomorphism from $A''_M$ to $\prod_i(A_i)''_{M_i}$. This proves assertion a).

The proof of b) is the same as that of a) mutatis mutandis.

#### Proposition 2 {#alg-viii-s5-prop-2 .statement}

Let A be a ring, and let M be an A-module. Let I be a set. Then the bicommutant of the A-module $M^{(I)}$ coincides with the ring of homotheties of the $A''_M$-module $M^{(I)}$.

For $i\in I$, we denote the projection homomorphism from $M^{(I)}$ to M by $\pi_i: (x_j)_{j\in I}\mapsto x_i$ and the corresponding canonical injection (I, §4, No. 9, p. 47) by $\iota_i: M\rightarrow M^{(I)}$.

Let $u$ be an element of End$_A(M^{(I)})$. For all $i, j\in I$, the composition $u_{i,j}=\pi_j\circ u\circ \iota_i$ belongs to the commutant $A'_M$ of M. For every element $b$ of $A''_M$ and every $(x_i)\in M^{(I)}$, we have the relations

$$
bu(x_i)_{i\in I}=b\sum u_{i,j}(x_i)=\sum u_{i,j}(bx_i)=u b(x_i)_{i\in I}
$$

$$
j\in Ij\in I
$$

$i\in Ii\in I$

The homothety $b_{M^{(I)}}$ therefore belongs to the bicommutant of the A-module $M^{(I)}$.

Conversely, let $b$ be an element of the bicommutant of $M^{(I)}$. For $i, j\in I$, set $b_{i,j}=\pi_j\circ b\circ \iota_i$. Take $i, j\in I$ with $i\not=j$. Since $\iota_j\circ \pi_j$ belongs to the commutant of the A-module $M^{(I)}$, we have

$$
b_{i,j}=\pi_j\circ \iota_j\circ \pi_j\circ b\circ \iota_i=\pi_j\circ b\circ \iota_j\circ \pi_j\circ \iota_i= 0
$$

Likewise, we have

$$
b_{j,j}=\pi_j\circ b\circ \iota_j=\pi_i\circ \iota_i\circ \pi_j\circ b\circ \iota_j=\pi_i\circ b\circ \iota_i\circ \pi_j\circ \iota_j=b_{i,i}
$$

Moreover, $b_{i,i}$ belongs to $A''_M$. It follows that $b$ coincides with a homothety of the $A''_M$-module $M^{(I)}$.

### 2. Generating Modules

Let A be a ring.

#### Definition 2 {#alg-viii-s5-def-2 .statement}

An A-module M is called generating if every A-module N is generated by the images of the A-linear mappings from M to N.

Let M be a left A-module. We denote the dual of M by $M^*$ and the canonical bilinear form on $M\times M^*$ (II, §2, No. 3, p. 233) by

$$
(x, x^*)\mapsto  \langle x, x^*\rangle =x^*(x)
$$

We denote by $\tau (M)$ the set of elements of A of the form $\sum^n_{i=1}\langle x_i, x^*_i\rangle$, where $x_1, . . . , x_n$ are elements of M and $x^*_1, . . . , x^*_n$ are elements of $M^*$. It is a two-sided ideal of A, called the trace ideal of M. The trace ideal of the A-module $A_s$ is A. The trace ideal of a module that is the direct sum of a family $(M_i)_{i\in I}$ of A-modules is the ideal $\sum_{i\in I}\tau (M_i)$. If M is a projective A-module, then it follows from Proposition 12 of II, §2, No. 6, p. 238, that we have $M =\tau (M)M$.

#### Theorem 1 {#alg-viii-s5-thm-1 .statement}

Let M be a left A-module. The following properties are equivalent:

(i) The A-module M is generating.

(ii) For every A-module N, there exist a set I and a surjective A-linear mapping from $M^{(I)}$ to N.

(iii) There exist an integer $n\geqslant 0$ and a surjective A-linear mapping from $M^n$ to $A_s$.

(iv) There exists an integer $n\geqslant 0$ such that $A_s$ is isomorphic to a direct factor submodule of $M^n$.

(v) The trace ideal $\tau (M)$ is equal to A.

(vi) There exist an integer $n\geqslant 0$, elements $x_1, . . . , x_n$ of M, and elements $x^*_1, . . . , x^*_n$ of $M^*$ satisfying $\sum^n_{i=1}\langle x_i, x^*_i\rangle = 1$.

(i) $\Rightarrow$ (ii): Suppose that M is generating, and let N be a left A-module. There exists a family $(u_i)_{i\in I}$ of A-linear mappings from M to N such that we have $N =\sum_{i\in I}u_i(M)$. The mapping $(x_i)\mapsto \sum_{i\in I}u_i(x_i)$ from $M^{(I)}$ to N is A-linear and surjective.

(ii) $\Rightarrow$ (iii): Assume that property (ii) holds, and take $N = A_s$. We then have a set I and a surjective linear mapping $u: M^{(I)}\rightarrow A_s$. Since $A_s$ is generated by the element 1, there exists a finite subset J of I such that $u(M^{(J)}) = A_s$, whence (iii).

(iii) $\Rightarrow$ (iv): This follows from Proposition 21 of II, §1, No. 12, p. 218.

(iv) $\Rightarrow$ (v): Let $n\geqslant 1$ be an integer such that $A_s$ is isomorphic to a direct factor submodule of M. We have $A =\tau (A_s)\subset \tau (M^n) =\tau (M)$ and therefore $\tau (M) = A$.

(v) $\Rightarrow$ (vi): This is clear.

(vi) $\Rightarrow$ (i): Let $n$ be an integer $\geqslant 0,x_1, . . . , x_n$ elements of M, and $x^*_1, . . . , x^*_n$ elements of $M^*$ satisfying $\sum^n_{i=1}\langle x_i, x^*_i\rangle = 1$. Let N be a left A-module and $y$ an element of N. The mappings $u_i:x\mapsto  \langle x, x^*_i\rangle y$ from M to N are A-linear, and we have $y=\sum^n_{i=1}u_i(x_i)$. This proves that M is a generating A-module. **Corollary.** — A generating A-module is faithful.

Let $a\in A$ satisfy $aM = 0$. Using the implication (i) $\Rightarrow$ (iv) of Theorem 1, we obtain $aA_s= 0$, and therefore $a= 0$. The corollary follows (II, §1, No. 12, p. 219).

#### Example 1 {#alg-viii-s5-n2-exa-1 .statement}

The A-module $A_s$ is generating.

#### Example 2 {#alg-viii-s5-n2-exa-2 .statement}

Every nonzero free A-module is generating. More generally, every module with a generating quotient is itself generating.

#### Example 3 {#alg-viii-s5-n2-exa-3 .statement}

Let M be a semisimple A-module whose countermodule is finitely generated. Then M is a generating $A_M$-module. Indeed, by Lemma 4 of VIII, p. 8, there exists a natural number $m$ such that $(A_M)_s$ is isomorphic to a submodule of $M^m$. Since $M^m$ is a semisimple $A_M$-module, $(A_M)_s$ is isomorphic to a direct factor submodule of $M^m$ and M is a generating $A_M$-module (Theorem 1).

#### Example 4 {#alg-viii-s5-n2-exa-4 .statement}

Let A be a principal ideal domain, and let P be a finitely generated A-module. There exist an integer $n\geqslant 1$ and an increasing sequence of ideals $(\mathfrak{a}_i)_{1\leqslant i\leqslant n}$ of A such that P is isomorphic to the direct sum of the $A/\mathfrak{a}_i$ (VII, §4, No. 4, p. 19, Theorem 2); the annihilator $\mathfrak{a}$ of P is equal to $\mathfrak{a}_1$. Then P is a generating module over the ring $A/\mathfrak{a}$. If P is not a torsion module, then we have $\mathfrak{a}= 0$ and P is a generating A-module.

#### Lemma 1 {#alg-viii-s5-lem-1 .statement}

Let A be a commutative ring, M a finitely generated A-module, and Ann(M) its annihilator. Let $\mathfrak{a}$ be an ideal of A. The following properties are equivalent:

(i) $\mathfrak{a}M = M$.

(ii) Ann(M) $+\mathfrak{a}= A$.

(iii) There exists an element $a$ of $\mathfrak{a}$ such that $am=m$ for every $m\in M$.

(i) $\Rightarrow$ (ii): Let $(x_1, . . . , x_n)$ be a generating family of the A-module M. If $\mathfrak{a}M = M$, then each $x_i$ can be written as $\sum^n_{j=1}c_{ij}x_j$, where the $c_{ij}$ belong to $\mathfrak{a}$. Denote the matrix $(c_{ij})$ by C and the column matrix with entries $x_1, . . . , x_n$ by X. We have ($I_n-C$)X = 0. Let $d$ be the determinant and V the cofactor matrix of the matrix $I_n-C$. By formula (26) of III, §8, No. 6, p. 532, we have $dX=^tV$($I_n-C$)X = 0, so that $d\in$ Ann(M). On the other hand, since the $c_{ij}$ belong to $\mathfrak{a}$, we have $d\equiv$ 1(mod $\mathfrak{a})$ (III, §8, No. 5, p. 529, (18)), and therefore $1\in$ Ann(M) $+\mathfrak{a}$.

(ii) $\Rightarrow$ (iii): Assuming that (ii) holds, there exist $a\in \mathfrak{a}$ and $b\in$ Ann(M) such that $a+b= 1$. We then have $am=m$ for every $m\in M$.

(iii) $\Rightarrow$ (i): This is clear. **Proposition 3.** — Let A be a commutative ring. Every finitely generated and faithful projective A-module is generating. More generally, a finitely generated projective A-module P is a generating $A_P$-module.

Let P be a finitely generated projective A-module. We have $\tau (P)P = P$ (VIII, p. 80).

If the A-module P is faithful, then the ideal $\tau (P)$ is equal to A (Lemma 1) and the A-module P is generating (Theorem 1); this leads to the first assertion. The second follows by Lemma 2 below.

#### Lemma 2 {#alg-viii-s5-lem-2 .statement}

Let A be a ring and M a projective A-module. The $A_M$-module M is projective.

Let $(x_i)_{i\in I}$ be a generating family of the A-module M. There exists a family $(x^*_i)_{i\in I}$ of linear forms on the A-module M such that for every $x\in M$, the family $(\langle x, x^*_i\rangle )_{i\in I}$ has finite support and $x=\sum_{i\in I}\langle x, x^*_i\rangle x_i$ (II, §2, No. 6, p. 238, Proposition 12). For every $i\in I$, the mapping $x\mapsto  \langle x, x^*_i\rangle_M$ is a linear form on the $A_M$-module M, and we have $x=\sum_{i\in I}\langle x, x^*_i\rangle_Mx_i$ for every $x\in M$. By loc. cit., M is a projective $A_M$-module.

### 3. The Bicommutant of a Generating Module

#### Theorem 2 {#alg-viii-s5-thm-2 .statement}

A generating module is balanced.

Let A be a ring, and let M be a generating A-module; by definition, there exist an integer $n\geqslant 0$, elements $x_1, . . . , x_n$ of M, and elements $x^*_1, . . . , x^*_n$ of the dual $M^*$ of M satisfying $\sum^n_{i=1}\langle x_i, x^*_i\rangle = 1$. Recall (II, §4, No. 2, p. 271) that we define a group homomorphism $\theta : M^*\otimes_AM\rightarrow$ End$_A(M)$ by the formula $\theta (x^*\otimes y)(x) =\langle x, x^*\rangle y$. If $u$ is an element of the bicommutant of M, then it commutes with End$_A(M)$; therefore, for every $y\in M$, we have

$$
u(y) =u\sum_{i=1}^n\langle x_i, x^*_i\rangle y=\sum_{i=1}^nu(\theta (x^*_i\otimes y)(x_i))
$$

$$
=\sum_{i=1}^n\theta (x^*_i\otimes y)(u(x_i)) =\sum_{i=1}^n\langle u(x_i), x^*_i\rangle y
$$

Consequently, $u$ belongs to $A_M$, and M is balanced.

#### Corollary 1 {#alg-viii-s5-thm-2-cor-1 .statement}

A free module is balanced.

This is clear if the module is zero, and a nonzero free module is generating (VIII, p. 81, Example 2). **Corollary 2.** — Let A be a ring, and let $n$ be an integer $\geqslant 0$. The center of $\mathbf{M}_n(A)$ consists of the scalar matrices with entries in the center of A. We view $A^n$ as a left $\mathbf{M}_n(A)$-module (II, §10, No. 7, p. 349). The endomorphisms of this module are the mappings $x\mapsto xa$, where $a$ runs through A.

Let M be the right A-module $A^n_d$. It is balanced by Corollary 1. Consequently, the centers of $A_M, A'_M$, and $A''_M$ coincide. Corollary 2 then follows from the fact that $A_M$ is identified with A and $A'_M$ with $\mathbf{M}_n(A)$.

#### Remark {#alg-viii-s5-n3-rem-1 .statement}

Let M be an A-module. If the $A_M$-module M is generating, then we have $A_M= A''_M$ by Theorem 2 applied to the $A_M$-module M, so that M is a balanced A-module.

#### Corollary 3 {#alg-viii-s5-thm-2-cor-3 .statement}

Every finitely generated projective module over a commutative ring is balanced.

Indeed, a finitely generated projective module M is a generating $A_M$-module by Proposition 3 of VIII, p. 82. The corollary therefore follows from the remark above.

#### Corollary 4 {#alg-viii-s5-thm-2-cor-4 .statement}

Every finitely generated module over a principal ideal domain is balanced.

Indeed, a finitely generated module M over a principal ideal domain A is a generating $A_M$-module (VIII, p. 81, Example 4).

#### Corollary 5 {#alg-viii-s5-thm-2-cor-5 .statement}

Let K be a commutative field, V a finite-dimensional vector space over K, and $u$ and $v$ endomorphisms of V. The following properties are equivalent:

(i) There exists a polynomial P in K[X] such that $v= P(u)$.

(ii) The endomorphism $v$ commutes with every endomorphism of V that commutes with $u$.

Take A to be the ring K[X] and M to be the K[X]-module deduced from V and $u$ (VII, §5, No. 1, p. 28). Assertion (i) means that $v\in K[X]_M$ and (ii) that $v\in K[X]''_M$. Corollary 5 is therefore a particular case of Corollary 4.

#### Proposition 4 {#alg-viii-s5-prop-4 .statement}

A semisimple module with finitely generated countermodule is balanced.

This follows from Example 3 of VIII, p. 81 and the remark.

#### Corollary 1 {#alg-viii-s5-prop-4-cor-1 .statement}

Let $(S_i)_{i\in I}$ be a finite family of pairwise nonisomorphic simple A-modules. For $i\in I$, denote by $D_i$ the opposite ring of the field of endomorphisms of $S_i$. Suppose that for every $i\in I$, the $D_i$-vector space $S_i$ is finite-dimensional. Then the mapping $a\mapsto (a_{S_i})_{i\in I}$ from A to $\prod_{i\in I}$ End$_{D_i}(S_i)$ is surjective.

Consider the A-module $M =\prod_{i\in I}S_i$. Since I is finite, we also have $M =\bigoplus_{i\in I}S_i$, and the image of $S_i$ in M is the isotypical component of M of type $S_i$. Consequently, the endomorphisms of the A-module M are the mappings $(s_i)\mapsto (s_id_i)$, where $(d_i)_{i\in I}$ runs through $\prod_{i\in I}D_i$ (VIII, p. 66, Proposition 5). Since I is finite and for every $i\in I$, the right $D_i$-vector space $S_i$ is finite-dimensional, the countermodule of M is finitely generated. By Proposition 4, the A-module M is balanced. Now, the bicommutant of the A-module M consists of elements of End$_{\mathbf{Z}}(M)$ of the form $\prod_{i\in I}u_i$, where $(u_i)\in \prod_{i\in I}$ End$_{D_i}(S_i)$ (VIII, p. 78, Proposition 1) because End$_{D_i}(S_i)$ is the bicommutant of $S_i$. The corollary follows from this.

This corollary applies, in particular, when A is an algebra over a commutative field K and each $S_i$ is a simple A-module that is finite-dimensional as a K-vector space: indeed, $D_i$ then contains the homotheties $\alpha_{S_i}$, where $\alpha$ runs through K, and $S_i$ is finite-dimensional over $D_i$ because it is so over K.

Corollary 2 (Burnside’s theorem). — Let A be an algebra over an algebraically closed commutative field K, and let S be a simple A-module that is finite-dimensional as a K-vector space. Then the mapping $a\mapsto a_S$ from A to End$_K(S)$ is surjective.

Indeed, the field of endomorphisms of the A-module S consists of the homotheties $\alpha_S$ with $\alpha \in K$ (VIII, p. 47, Theorem 1). We then apply Corollary 1 to the simple A-module S.

### 4. The Countermodule of a Semisimple Module

Let A be a ring. Denote the set of classes of simple A-modules by $\mathscr{S}$. For every $\lambda \in \mathscr{S}$, choose a simple A-module $S_{\lambda}$ of class $\lambda$, and denote the opposite ring of the field of endomorphisms of $S_{\lambda}$ by $D_{\lambda}$. We view $S_{\lambda}$ as an $(A,D_{\lambda}$)-bimodule.

Let M be a semisimple A-module, and let B be the endomorphism ring of M. Denote the bicommutant of M by C. For every $\lambda \in \mathscr{S}$, denote the left $(D_{\lambda}$, B)-bimodule Hom$_A(S_{\lambda},M)$ by $V_{\lambda}$. Finally, denote the support of the A-module M by $\mathscr{S}_M$ (VIII, p. 66); it is also the set of elements $\lambda$ of $\mathscr{S}$ such that $V_{\lambda}$ is nonzero. **Remark 1.** — The canonical description $\alpha_M$ of the A-module M is an isomorphism of left $(A$, B)-bimodules. By the corollary of Proposition 9, VIII, p. 71, the mapping $f\mapsto$ Hom(1$_{S_{\lambda}}, f)_{\lambda\in\mathscr{S}_M}$ from B to $\prod_{\lambda\in\mathscr{S}_M}$ End$_{D_{\lambda}}(V_{\lambda})$ is a ring isomorphism.

#### Proposition 5 {#alg-viii-s5-prop-5 .statement}

a) The countermodule of M is semisimple.

b) For every $\lambda \in \mathscr{S}_M$, the B-module $V_{\lambda}$ is simple, and its commutant is equal to $(D_{\lambda})_{V_{\lambda}}$.

c) The mapping $\lambda \mapsto$ cl(V$_{\lambda})$ is a bijection from the support of the A-module M to the support of its countermodule.

d) For every $\lambda \in \mathscr{S}_M$, the B-submodule $M_{\lambda}$ is the isotypical component of type $V_{\lambda}$ of the B-module M, and the multiplicity of $V_{\lambda}$ in M is equal to dim$_{D_{\lambda}}(S_{\lambda})$.

e) For $s\in S$, denote the mapping $\varphi \mapsto \varphi (s)$ from $V_{\lambda}=$ Hom$_A(S_{\lambda},M)$ to M by $\widetilde{s}$. It is B-linear. The resulting mapping $s\mapsto \widetilde{s}$ from $S_{\lambda}$ to Hom$_B(V_{\lambda},M)$ is an isomorphism of $(A,D_{\lambda})$-bimodules.

Let $\lambda \in \mathscr{S}_M$. Denote the ring End$_{D_{\lambda}}(V_{\lambda})$ by $E_{\lambda}$; since $V_{\lambda}$ is a nonzero $D_{\lambda}$-vector space, it is a simple $E_{\lambda}$-module, (VIII, p. 45, Example 3), and its commutant is equal to $(D_{\lambda})_{V_{\lambda}}$ (VIII, p. 82, Corollary 1 of Theorem 2). Since $E_{\lambda}$ is the ring of homotheties of the B-module $V_{\lambda}$ (VIII, p. 71, Corollary of Proposition 9), this proves b).

The canonical description $\alpha_M$ of M defines an isomorphism $\alpha_{\lambda}$ from $V_{\lambda}\otimes_{D^o}S_{\lambda}$ to $M_{\lambda}$. Since $V_{\lambda}$ is a simple B-module, the B-module $V_{\lambda}\otimes_{D^o}S_{\lambda}$

$\lambda \lambda$

is isotypical of type $V_{\lambda}$ (VIII, p. 61, Proposition 1); the same therefore holds for the B-module $M_{\lambda}$, which proves a).

By Remark 1 above, there exist elements $e_{\lambda}$ of B, for $\lambda$ running through $\mathscr{S}_M$, such that $(e_{\lambda})_{V_{\lambda}}= 1_{V_{\lambda}}$ and $(e_{\lambda})_{V_µ}$ = 0 for $µ\in \mathscr{S}_M$ with $µ\not=\lambda$. The simple B-modules $V_{\lambda}$ are therefore pairwise nonisomorphic, which proves c) and the first assertion of d). The B-module $M_{\lambda}$ is isomorphic to $V_{\lambda}\otimes_{D^o_{\lambda}}S_{\lambda}$, so dim$_{D_{\lambda}}(S_{\lambda})$ is the multiplicity of $V_{\lambda}$ in M (II, §3, No. 7, p. 255, Corollary 1).

The mapping $\sum_{\lambda\in\mathscr{S}_M}\alpha_{\lambda}$ from $\bigoplus_{\lambda\in\mathscr{S}_M}V_{\lambda}\otimes_{D^o_{\lambda}}S_{\lambda}$ to M provides a description (VIII, p. 69, Definition 5) of the semisimple B-module M. By VIII, p. 70, Proposition 8, b), for every $\lambda \in \mathscr{S}_M$, the mapping from $S_{\lambda}$ to Hom$_B(V_{\lambda},M)$ described in e) is bijective and $D_{\lambda}$-linear. Since it is obviously A-linear, this proves e). **Remark 2.** — It follows from the proof that the mapping

$$
\sum V_{\lambda}\otimes_{D^o}S_{\lambda}\longrightarrow M
$$

$\lambda$

$\lambda \in \mathscr{S}_M$

induced by the canonical description of M is a description of the countermodule of M.

#### Proposition 6 {#alg-viii-s5-prop-6 .statement}

a) Viewed as an $(A,B^o)$-bimodule, M is semisimple.

b) For every $\lambda \in \mathscr{S}_M,M_{\lambda}$ is a simple $(A,B^o)$-sub-bimodule of M.

c) For every $(A,B^o)$-sub-bimodule N of M, there exists a unique subset Λ of $\mathscr{S}_M$ such that N is equal to $\oplus_{\lambda\in\Lambda}M_{\lambda}$.

Let $\lambda$ be in $\mathscr{S}_M$. The left A-module $S_{\lambda}$ and the right B-module $V_{\lambda}$ are simple, and $D_{\lambda}$ is the opposite ring of the field of endomorphisms of $S_{\lambda}$. By Corollary 2 of VIII, p. 63, the $(A,B^o$)-bimodule $S_{\lambda}\otimes_{D_{\lambda}}V_{\lambda}$ is simple, and the same holds for $M_{\lambda}$, which is isomorphic to it. This proves b), and a) follows.

If $\lambda$ and $µ$ are distinct in $\mathscr{S}_M$, then $M_{\lambda}$ and $M_µ$ are not isomorphic as A-modules, nor a fortiori as $(A,B^o$)-bimodules. Assertion c) follows by Corollary 2 of VIII, p. 68.

#### Proposition 7 {#alg-viii-s5-prop-7 .statement}

a) For every element $c$ of the bicommutant C of M and every $\lambda \in \mathscr{S}_M$, there exists a unique element $c_{\lambda}$ of End$_{D_{\lambda}}(S_{\lambda})$ such that for every $\varphi \in$ Hom$_A(S_{\lambda},M)$ and every $s\in S_{\lambda}$, we have $c\varphi (s) =\varphi (c_{\lambda}s)$.

b) Endow the $S_{\lambda}$, for $\lambda$ running through $\mathscr{S}_M$, with the C-module structure defined by a). Then the canonical mapping $\alpha_M$ from $\bigoplus_{\lambda\in\mathscr{S}_M}S_{\lambda}\otimes_{D_{\lambda}}V_{\lambda}$ to M is an isomorphism of $(C,B^o)$-bimodules.

c) The mapping $c\mapsto (c_{\lambda})_{\lambda\in\mathscr{S}_M}$ is an isomorphism from C to $\prod_{\lambda\in\mathscr{S}_M}$ End$_{D_{\lambda}}(S_{\lambda})$.

Assertions a) and c) follow from VIII, p. 71, Proposition 9 because the canonical mapping $\alpha_M$ from $\bigoplus_{\lambda\in\mathscr{S}}(S_{\lambda}\otimes_{D_{\lambda}}W_{\lambda})$ to M provides a description of the B-module M (Remark 2). Moreover, $\alpha_M$ is $(C,B^o$)-linear, which proves b).

#### Remark 3 {#alg-viii-s5-n4-rem-3 .statement}

Endow $S_{\lambda}$, for $\lambda \in \mathscr{S}_M$, with the C-module structure given by Proposition 7, a). If we replace A with B and B with C in Proposition 5 (VIII, p. 85), then we see that for every $\lambda \in \mathscr{S}_M$, the left C-module $S_{\lambda}$ is simple, with commutant $D_{\lambda}$, that the isotypical component of type $S_{\lambda}$ of the C-module M is equal to $M_{\lambda}$, and that the mapping $\lambda \mapsto$ cl$_C(S_{\lambda})$ is a bijection from the support of the A-module M to the support of the C-module M. Finally, observe that the A-linear mappings and C-linear mappings from $S_{\lambda}$ to M are identical, as are the A-submodules and C-submodules of M, and that the rings End$_A(M)$ and End$_C(M)$ are equal.

Let M be a semisimple A-module. Denote by Z the center of the bicommutant C of the A-module M; it is also the center of the commutant B of M. Endow M and the $S_{\lambda}$, for $\lambda \in \mathscr{S}_M$, with Z-module structures deduced by restriction of scalars from the C-module structures. For every $\lambda \in \mathscr{S}_M$, denote the center of the field $D_{\lambda}$ by $Z_{\lambda}$.

#### Proposition 8 {#alg-viii-s5-prop-8 .statement}

a) The mapping $z\mapsto (z_{S_{\lambda}})_{\lambda\in\mathscr{S}_M}$ is an isomorphism from Z to the product of the fields $Z_{\lambda}$.

b) The A-module M is isotypical and nonzero if and only if Z is a field.

c) Let Λ be a subset of $\mathscr{S}_M$. Denote by $e_{\Lambda}$ the unique element of Z such that $(e_{\Lambda})_{S_{\lambda}}= 1_{S_{\lambda}}$ for $\lambda \in Λ$ and $(e_{\Lambda})_{S_{\lambda}}= 0$ for $\lambda \in \mathscr{S}_M$ Λ. We have $(e_{\Lambda})_{M_{\lambda}}= 1_{M_{\lambda}}$ for $\lambda \in Λ$ and $(e_{\Lambda})_{M_{\lambda}}= 0$ for $\lambda \in \mathscr{S}_M$ Λ.

d) If the support $\mathscr{S}_M$ of M is finite, then the mapping $Λ\mapsto e_{\Lambda}Z$ is a bijection from the set of subsets of $\mathscr{S}_M$ to the set of ideals of Z, and the mapping $\mathfrak{a}\mapsto \mathfrak{a}M$ is a bijection from the set of ideals of Z to the set of $(A,B^o)$-sub-bimodules of M. These bijections are isomorphisms of ordered sets. The reverse bijection sends an $(A,B^o)$-sub-bimodule N of M to the ideal consisting of the elements $z$ of Z that send N into M.

For $\lambda \in \mathscr{S}_M, Z_{\lambda}$ is the common center of the commutant $D_{\lambda}$ and the bicommutant $C_{\lambda}$ of the A-module $S_{\lambda}$. By Proposition 7, c) above, the mapping $c\mapsto (c_{\lambda})_{\lambda\in\mathscr{S}_M}$ is an isomorphism from C to $\prod_{\lambda\in\mathscr{S}_M}C_{\lambda}$. By restriction to the centers, we obtain the isomorphism $z\mapsto (z_{S_{\lambda}})_{\lambda\in\mathscr{S}_M}$ from Z to $\prod_{\lambda\in\mathscr{S}_M}Z_{\lambda}$, whence a).

The ring $\prod_{\lambda\in\mathscr{S}_M}Z_{\lambda}$ is a field if and only if the set $\mathscr{S}_M$ has a single element, whence b).

Assertion c) follows from Proposition 7, a). Suppose that $\mathscr{S}_M$ is finite. It follows from a) and Proposition 8 of I, §8, No. 10, p. 109, that the mapping $Λ\mapsto e_{\Lambda}Z$ is an isomorphism of ordered sets from $\mathfrak{P}(\mathscr{S}_M)$ to the set of ideals of Z. Let Λ be a subset of $\mathscr{S}_M$. By c), we have the relation $e_{\Lambda}$ZM $=e_{\Lambda}M =$ $\bigoplus_{\lambda\in\Lambda}M_{\lambda}$; because of Proposition 6, c) of VIII, p. 86, it remains to describe the inverse bijection. But $z\in Z$ sends M into $\bigoplus_{\lambda\in\Lambda}M_{\lambda}$ if and only if $z=e_{\Lambda}z$, that is, $z\in e_{\Lambda}Z$.

#### Corollary {#alg-viii-s5-n4-cor-1 .statement}

Suppose that A is an algebra over an algebraically closed commutative field K and that M is a semisimple A-module that is finite-dimensional as a vector space over K. For every $\lambda$ in $\mathscr{S}_M$, denote by $e_{\lambda}$ the projector of M with image $M_{\lambda}$ and kernel $\oplus_{\lambda\not=µ}M_µ$. Then $(e_{\lambda})_{\lambda\in\mathscr{S}_M}$ is a basis of the vector space Z over K.

Since M is a finite-dimensional vector space over K that is the direct sum of the family of nonzero submodules $(M_{\lambda})_{\lambda\in\mathscr{S}_M}$, the set $\mathscr{S}_M$ is finite, and each of the spaces $S_{\lambda}$, for $\lambda \in \mathscr{S}_M$, is finite-dimensional over K. Since the field K is algebraically closed, we have $D_{\lambda}= Z_{\lambda}= K$ (VIII, p. 47, Theorem 1), and the mapping $z\mapsto (z_{S_{\lambda}})_{\lambda\in\mathscr{S}_M}$ is an isomorphism from Z to $K_{\mathscr{S}_M}$ (Proposition 8, a)). The corollary then follows from part c) of Proposition 8.

### 5. Density Theorem

Theorem 3 (Jacobson). — Let M be a semisimple A-module, and let $c$ be an endomorphism of the additive group M. Then $c$ belongs to the bicommutant $A''_M$ of M if and only if it satisfies the following condition:

(D) For every finite subset F of M, there exists an element $a$ of A such that $c$ coincides with $a_M$ on F.

First, suppose that $c$ satisfies condition (D). Let $u$ be an element of $A'_M$. Let $x$ be an element of M, and apply condition (D) to the subset $F =\{x, u(x)\}$. There exists an element $a$ of A such that $c(x) =ax$ and $c(u(x)) =au(x)$, so that $u(c(x)) =u(ax) =au(x) =c(u(x))$. Since $x$ is arbitrary, we have $cu=uc$; as this holds for all $u$, we have $c\in A''_M$.

For the converse, we use the following lemma.

#### Lemma 3 {#alg-viii-s5-lem-3 .statement}

Let M be a semisimple A-module. Let B be the bicommutant of the A-module M. Then every A-submodule of M is a B-submodule of M.

Let N be an A-submodule of M. By Corollary 2 of VIII, p. 56, there exists a projector $p$ of the A-module M with image N; it belongs to $A'_M$. Since we have the relation $pb=bp$ for every $b\in B$, we obtain that N is a B-submodule of M.

Let us conclude the proof of Theorem 3. Suppose that $c$ belongs to $A''_M$, and let F = $\{x_1, . . . , x_n\}$ be a finite subset of M. Denote the element $(x_1, . . . , x_n)$ of $M^n$ by $x$. The A-module $M^n$ is semisimple and, by Proposition 2 of VIII, p. 79, its bicommutant coincides with the homotheties of the $A''_M$-module $M^n$. By Lemma 3, the A-submodule $Ax$ of $M^n$ is an $A''_M$-submodule of $M^n$. Let $a\in A$ be such that $(cx_1, . . . , cx_n)$ is equal to $ax$. Then $c$ coincides with $a_M$ on $\{x_1, . . . , x_n\}$, which implies condition (D).

#### Remark {#alg-viii-s5-n5-rem-1 .statement}

Denote the endomorphism ring of the additive group of M by E. Endow M with the discrete topology; the ring E consists of mappings from M to M, and we can endow it with the topology induced by the product topology on $M^M$ (“topology of simple convergence in M”, Gen. Top., I, §2, No. 3, p. 31). The topology on E is Hausdorff and compatible with the additive group structure on E. For every $f$ in E, the mappings $g\mapsto f\circ g$ and $g\mapsto g\circ f$ from E to E are continuous. Consequently, the commutant of every subset of E is closed in E. Theorem 3 therefore implies that $A''_M$ is the closure of $A_M$ in E.

### 6. Application to Field Theory

#### Proposition 9 {#alg-viii-s5-prop-9 .statement}

Let L be a field and E a subring of End$_{\mathbf{Z}}(L)$ that contains the mapping $\boldsymbol{\gamma }_a:x\mapsto ax$ for every $a\in L$. Denote by K the set of elements $a$ of L such that $u(xa) =u(x)a$ for every $x$ in L and every $u$ in E; it is a subfield of L.

Let V be a finite-dimensional linear subspace of the right K-vector space L, and let $h$ be a K-linear mapping from V to L. There exists an element of E that coincides with $h$ on V.

We view L as a left E-module. Since E contains the left multiplications $\boldsymbol{\gamma }_a$, every E-submodule of L is a left ideal of the field L; the E-module L is therefore simple. Every endomorphism of the additive group of L that commutes with the $\boldsymbol{\gamma }_a$ is of the form $\boldsymbol{\delta }_b:x\mapsto xb$ with $b$ in L. Consequently, $b\mapsto \boldsymbol{\delta }_b$ is an isomorphism from K to the opposite ring of End$_E$(L), which is a field.

The bicommutant $E''$ of the E-module L therefore consists of the endomorphisms of the right K-vector space L. Let $v$ be an endomorphism of the K-vector space L whose restriction to V coincides with $h$; it is an element of $E''$. Let $(x_i)_{i\in I}$ be a basis of V over K; by Theorem 3 (VIII, p. 88), there exists an element $u$ of E such that $u(x_i) =v(x_i) =h(x_i)$ for $i\in I$. By linearity, it follows that $u(x) =h(x)$ for every $x$ in V.

#### Corollary {#alg-viii-s5-n6-cor-1 .statement}

Let L be a field. Let Γ be a subgroup of the automorphism group of the field L, and let K be the field of invariants of Γ. Let V be a right K-linear subspace of L of finite dimension $n$ over K. Then there exist elements $\sigma_1, . . . , \sigma_n$ of Γ with the following property: for every K-linear mapping $u$ from V to L, there exist elements $a_1, . . . , a_n$ of L such that we have $u(x) =\sum_i^n_{=1}a_i\sigma_i(x)$ for every $x$ in V.

Denote by E the set of mappings from L to L of the form $x\mapsto$ $Σ_{\sigma\in\Gamma}a_{\sigma}\sigma (x)$, where $(a_{\sigma})_{\sigma\in\Gamma}$ is a family of elements of L with finite support. We have $\boldsymbol{\gamma }_a\in E$ for every $a$ in L, and E is a subring of the endomorphism ring of the additive group of L. Moreover, the field K consists of the elements $a$ of L such that $u(xa) =u(x)a$ for every $x$ in L and every $u$ in E.

Let H be the left L-vector space Hom$_K(V,L)$; it has dimension $n$. By Proposition 9, it is generated by the restrictions of the elements of Γ to V. There exist $n$ elements $\sigma_1, . . . , \sigma_n$ of Γ whose restrictions to V form a basis of H over L. The corollary follows from this.

#### Remark {#alg-viii-s5-n6-rem-1 .statement}

When the field L is commutative, this corollary reduces to Artin’s theorem (V, §10, No. 6, p. 65).

### Exercises {#alg-viii-s5-exercises}

See the [exercises for § 5](exercises/s5/).
