---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 12
section_title: Tensor Products of Semisimple Modules
lang: en
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.211-A VIII.228
pdf_pages: 0228-0245
extraction: native
subsections:
    - "no": 1
      title: Semisimple Modules over Tensor Products of Algebras
      page: 211
      pdf_page: 228
    - "no": 2
      title: Tensor Products of Simple Modules
      page: 213
      pdf_page: 230
    - "no": 3
      title: Tensor Products of Semisimple Commutative Algebras
      page: 215
      pdf_page: 232
    - "no": 4
      title: The Radical of a Tensor Product of Algebras
      page: 217
      pdf_page: 234
    - "no": 5
      title: Tensor Products of Semisimple Modules
      page: 218
      pdf_page: 235
    - "no": 6
      title: Tensor Products of Semisimple Algebras
      page: 221
      pdf_page: 238
    - "no": 7
      title: Extension of Scalars in Semisimple Modules
      page: 222
      pdf_page: 239
statements: 26
exercises: 17
content_sha256: 6020f3b61ff41b5f57b660b58845013a596e982f71800914a058f01fab507010
---

## § 12. TENSOR PRODUCTS OF SEMISIMPLE MODULES

In this section, the letter K denotes a commutative field. If E and F are vector spaces over K, then we denote the tensor product $E\otimes_KF$ by $E\otimes F$.

### 1. Semisimple Modules over Tensor Products of Algebras

In this subsection, we consider K-algebras $A_1$ and $A_2$; we denote the algebra $A_1\otimes A_2$ by A.

#### Proposition 1 {#alg-viii-s12-prop-1 .statement tag=00E6}

Let $M_1$ be an $A_1$-module and $M_2$ an $A_2$-module, neither reduced to 0. If the module $M = M_1\otimes M_2$ over the ring $A = A_1\otimes A_2$ is simple (resp. isotypical, semisimple), then the $A_1$-module $M_1$ and the $A_2$-module $M_2$ are simple (resp. isotypical, semisimple).

Suppose that M is a semisimple A-module. Let $N_1$ be an $A_1$-submodule of $M_1$. Denote the canonical image of $N_1\otimes M_2$ in the A-module M by N. By Corollary 2 of VIII, p. 56, there exists an A-linear projector $p$ in M with image N. By assumption, we have $M_2\not= 0$; we can therefore choose an element $m$ of $M_2$ and a linear form $\varphi$ on the K-vector space $M_2$ such that $\varphi (m) = 1$ (II, §7, No. 5, p. 302, Corollary 2). Let $u$ be the mapping from $M_1$ to M defined by $u(m_1) =m_1\otimes m$, and let $v$ be the K-linear mapping from M to $M_1$ characterized by $v(m_1\otimes m_2) =\varphi (m_2)m_1$. Set $q=v\circ p\circ u$. The mapping $q: M_1\rightarrow M_1$ is $A_1$-linear, its image is contained in $N_1$, and we have $q(n) =n$ for every $n\in N_1$. Consequently, $q$ is a projector in $M_1$ with image $N_1$. We have proved that $M_1$ is a semisimple $A_1$-module (VIII, p. 56, Corollary 2).

Suppose that M is simple and that $M_1$ is the direct sum of two $A_1$-submodules $M'_1$ and $M''_1$. Set $M'= M'_1\otimes M_2$ and $M''= M''_1\otimes M_2$; then M is the direct sum of the A-submodules $M'$ and $M''$. Since M is simple, $M'$ or $M''$ must be reduced to 0; as we have $M_2\not= 0$ by assumption, we have $M'_1= 0$ or $M''_1= 0$ (II, §3, No. 7, p. 256, Corollary 2). This proves that $M_1$ is a simple $A_1$-module.

Now suppose that M is an isotypical A-module. Let S and T be simple $A_1$-submodules of $M_1$. The A-modules $S\otimes M_2$ and $T\otimes M_2$ can then be identified with nonzero submodules of M. They are therefore isotypical of the same type as M. By Remark VIII, p. 61, there exists a nonzero A-linear mapping $f: S\otimes M_2\rightarrow T\otimes M_2$. The mapping $f$ is, in particular, $A_1$-linear. Since the $A_1$-modules $S\otimes M_2$ and $T\otimes M_2$ are nonzero and isotypical of type S and T, respectively, S and T are isomorphic. This proves that $M_1$ is an isotypical $A_1$-module.

#### Proposition 2 {#alg-viii-s12-prop-2 .statement tag=00E7}

Let S be a simple module over the ring $A = A_1\otimes A_2$, finite-dimensional over K. For $i\in  \{1,2\}$, there exists a simple $A_i$-module $S_i$ such that the $A_i$-module S is isotypical of type $S_i$. The A-module S is isomorphic to a quotient of the A-module $S_1\otimes S_2$.

Since S is a nonzero $A_1$-module that is finite-dimensional over K, it has finite length over $A_1$ and there exist a simple left $A_1$-module $S_1$ and a nonzero $A_1$-linear mapping from $S_1$ to S. We endow $M_2=$ Hom$_{A_1}(S_1,S)$ with a left $A_2$-module structure defined by the external law $(a_2, u)\mapsto (a_2)_S\circ u$. We have $M_2\not= 0$ by construction, and $M_2$ is finite-dimensional over K. We can therefore find a simple left $A_2$-module $S_2$ and a nonzero $A_2$-linear mapping $\varphi : S_2\rightarrow M_2$. We define a nonzero A-linear mapping $\psi$ from $S_1\otimes S_2$ to S by

$$
\psi (s_1\otimes s_2) =\varphi (s_2)(s_1) \tag{1}
$$

for every $s_1\in S_1$ and $s_2\in S_2$. Since S is a simple A-module and $\psi$ is not zero, $\psi$ is surjective and S is isomorphic to a quotient of $S_1\otimes S_2$. For $i\in  \{1,2\}$, the $A_i$-module $S_1\otimes S_2$ is isotypical of type $S_i$, and therefore so is the $A_i$-module S (VIII, p. 61, Proposition 2).

For any K-algebra B, we denote by $\mathscr{S}_K(B)$ the set of classes of simple (VIII, p. 51) left B-modules that are finite-dimensional over K.

#### Theorem 1 {#alg-viii-s12-thm-1 .statement tag=00E8}

Suppose that the field K is algebraically closed.

a) Let $M_1$ be an $A_1$-module and $M_2$ an $A_2$-module, both simple (resp. semisimple) and finite-dimensional over K. Then $M_1\otimes M_2$ is a simple (resp. semisimple) module over the ring $A_1\otimes A_2$ and is finite-dimensional over K.

b) The mapping from $\mathscr{S}_K(A_1)\times \mathscr{S}_K(A_2)$ to $\mathscr{S}_K(A_1\otimes A_2)$ that sends (cl(S$_1)$, cl(S$_2))$ to cl(S$_1\otimes S_2)$, where $S_1($resp. $S_2)$ is a simple $A_1$-module (resp. $A_2$-module) that is finite-dimensional over K, is bijective.

To prove part a), it suffices to consider the case when $M_1$ and $M_2$ are simple. Let $M'$ be an A-submodule of $M = M_1\otimes M_2$; it is an $A_1$-submodule of $M_1\otimes M_2$, stable under the set of endomorphisms of the form $1_{M_1}\otimes u$, where $u$ runs through the set of homotheties of the $A_2$-module $M_2$. Since the field K is algebraically closed, Schur’s lemma (VIII, p. 47, Theorem 1) implies that the commutant End$_{A_1}(M_1)$ of $M_1$ is equal to K. By Corollary 2 of VIII, p. 63, the A-submodule $M'$ of $M_1\otimes M_2$ is of the form $M_1\otimes M'_2$, where $M'_2$ is an $A_2$-submodule of $M_2$. We have assumed that $M_2$ is simple; we therefore have $M'_2= 0$ or $M'_2= M_2$, that is, $M'= 0$ or $M'= M$. Consequently, M is simple.

If S is a simple module over $A_1\otimes A_2$ that is finite-dimensional over K, then it follows from Proposition 2 and part a) that S is isomorphic to a module of the form $S_1\otimes S_2$, where $S_1$ (resp. $S_2)$ is a simple $A_1$-module (resp. $A_2$-module). Moreover, as an $A_i$-module, S is isotypical of type $S_i$, so the class of $S_i$ only depends on that of S. This proves part b).

#### Remark 1 {#alg-viii-s12-n1-rem-1 .statement tag=00E9}

Assertion a) of Theorem 1 is no longer true when the field K is not assumed algebraically closed. We can give examples (VIII, p. 225, Exercise 4) where $M_i$ is a simple $A_i$-module that is finite-dimensional over K, for $i\in  \{1,2\}$, and where the A-module $M_1\otimes M_2$ is not semisimple or is semisimple but not simple.

#### Remark 2 {#alg-viii-s12-n1-rem-2 .statement tag=00EA}

There exists a homomorphism $\varphi$ from $R_K(A_1)\otimes_{\mathbf{Z}}R_K(A_2)$ to $R_K(A)$ characterized by the relation $\varphi ([M_1]\otimes [M_2]) = [M_1\otimes M_2]$. This can be proved in the same way as Proposition 9 of VIII, p. 196. If the field K is algebraically closed, then $\varphi$ is an isomorphism from $R_K(A_1)\otimes_ZR_K(A_2)$ to $R_K(A)$ by Theorem 1, b) because for every K-algebra B, the $\mathbf{Z}$-module $R_K(B)$ is free with basis the family $([S])_{S\in\mathscr{S}_K(B)}$ (VIII, p. 195).

### 2. Tensor Products of Simple Modules

Let $A_1$ and $A_2$ be algebras over the commutative field K. We denote the K-algebra $A_1\otimes A_2$ by A.

#### Lemma 1 {#alg-viii-s12-lem-1 .statement tag=00RB}

Let $M_1$ and $N_1$ be $A_1$-modules, and let $M_2$ and $N_2$ be $A_2$-modules. We make the following assumptions:

(i) The $A_1$-module $M_1$ is finitely generated.

(ii) The $A_2$-module $M_2$ is finitely generated, or $N_1$ is finite-dimensional over K.

Set $M = M_1\otimes M_2$ and $N = N_1\otimes N_2$, and view them as modules over the ring $A = A_1\otimes A_2$. The canonical homomorphism (II, §3, No. 5, p. 251)

$\lambda :$ Hom$_K(M_1,N_1)\otimes$ Hom$_K(M_2,N_2)\longrightarrow$ Hom$_K(M,N)$

then induces an isomorphism of K-vector spaces

$\varphi :$ Hom$_{A_1}(M_1,N_1)\otimes$ Hom$_{A_2}(M_2,N_2)\longrightarrow$ Hom$_A(M,N)$.

The mapping $\lambda$ is injective (II, §7, No. 7, p. 308, Proposition 16) and sends the linear subspace Hom$_{A_1}(M_1,N_1)\otimes$ Hom$_{A_2}(M_2,N_2)$ to Hom$_A(M,N)$. It therefore suffices to prove that every A-linear mapping from M to N belongs to the image of Hom$_{A_1}(M_1,N_1)\otimes$ Hom$_{A_2}(M_2,N_2)$ by $\lambda$. Let $u: M\rightarrow N$ be an A-linear mapping. Let $x\in M_1$. Denote by $u_x$ the $A_2$-linear mapping $y\mapsto u(x\otimes y)$ from $M_2$ to $N_1\otimes N_2$. Set P = Hom$_{A_2}(M_2,N_2)$, and denote by $\nu$ the canonical homomorphism from $N_1\otimes P$ to Hom$_{A_2}(M_2,N_1\otimes N_2)$ (II, §4, No. 2, p. 269). This mapping is injective (II, §4, No. 2, p. 269, Proposition 2, (i) applied to the K-vector space $N_1)$. By assumption (ii), there exists a linear subspace $V_x$ of $N_1$, finite-dimensional over K, such that $u_x$ takes on values in $V_x\otimes N_2$. It follows that $u_x$ is the image by $\nu$ of a unique element $v_x$ of $N_1\otimes P$. The mapping $\widetilde{u}:x\mapsto v_x$ from $M_1$ to $N_1\otimes P$ is $A_1$-linear. By assumption (i), the $A_1$-module $M_1$ is finitely generated. A reasoning analogous to the above shows that $\widetilde{u}$ belongs to the image of Hom$_{A_1}(M_1,N_1)\otimes P$ in Hom$_{A_1}(M_1,N_1\otimes P)$. Lemma 1 follows.

#### Theorem 2 {#alg-viii-s12-thm-2 .statement tag=00EB}

Let $A_1$ and $A_2$ be algebras over the commutative field K; let $S_1$ be a simple $A_1$-module and $S_2$ a simple $A_2$-module. Let $D_1$ and $D_2$ be the respective commutants of $S_1$ and $S_2$. Set $M = S_1\otimes S_2,A = A_1\otimes A_2$, and $D = D_1\otimes D_2$. We view M as a left $(A,D)$-bimodule.

a) The commutant of the A-module M is equal to $D_M$.

b) The mapping $\mathfrak{a}\mapsto \mathfrak{a}M$ is an isomorphism from the set of right ideals of D, ordered by inclusion, to the set of A-submodules of M, ordered by inclusion. The inverse mapping sends a submodule N of M to the ideal of D consisting of the elements $d$ such that $dM\subset N$.

Assertion a) follows from Lemma 1 because a simple module is monogenous.

Let T be the $(A_1,D_2$)-bimodule $S_1\otimes (D_2)_d$. We identify $M = S_1\otimes S_2$ with $T\otimes_{D_2}S_2$ (II, §3, No. 8, p. 258); this identification is compatible with the structures of left modules over the ring $A = A_1\otimes A_2$.

Let N be an A-submodule of M; it is an $A_2$-submodule of $T\otimes_{D_2}S_2$, stable by the endomorphisms of the form $(a_1)_T\otimes 1_{S_2}$ for $a_1$ running through $A_1$. It follows from Corollary 2 of VIII, p. 63 that there exists a unique $(A_1,D_2)$-sub-bimodule V of T such that $N = V\otimes_{D_2}S_2$.

The isomorphism $u$ from $T = S_1\otimes (D_2)_d$ to $((D_1)_d\otimes (D_2)_d)\otimes_{D_1}S_1$ defined by $u(s\otimes d) = 1\otimes d\otimes s$ is $(A_1,D_2$)-linear. We identify these $(A_1,D_2)$-bimodules. A reasoning analogous to that given above proves the existence and uniqueness of a right $(D_1\otimes D_2$)-submodule $\mathfrak{a}$ of $D_1\otimes D_2$ such that $V =\mathfrak{a}\otimes_{D_1}S_1$. In view of the identifications made above, $\mathfrak{a}$ is the unique right ideal of $D = D_1\otimes D_2$ such that $N =\mathfrak{a}M$.

We have just proved that the mapping $\mathfrak{a}\mapsto \mathfrak{a}M$ is bijective; the last assertion follows.

#### Corollary 1 {#alg-viii-s12-thm-2-cor-1 .statement tag=00EC}

The module $S_1\otimes S_2$ over the ring $A_1\otimes A_2$ is semisimple (resp. isotypical, simple) if and only if the ring $D = D_1\otimes D_2$ is semisimple (resp. simple, a field). In particular, $S_1\otimes S_2$ is simple if the commutant of $S_1$ or $S_2$ is equal to K.

By Theorem 2, the module $S_1\otimes S_2$ over the ring $D_1\otimes D_2$ is semisimple (resp. isotypical, simple) if and only if the right D-module $(D_1\otimes D_2)_d$ is (VIII, p. 109, Proposition 10). Now the right D-module $D_d$ is simple if and and only if D is a field; it is isotypical (resp. semisimple) if and only if the ring D is simple (resp. semisimple) (VIII, p. 120, Definition 1; VIII, p. 121, Corollary 1; and VIII, p. 137, Proposition 2).

#### Corollary 2 {#alg-viii-s12-thm-2-cor-2 .statement tag=00ED}

We have $\mathfrak{R}_A(M) =\mathfrak{R}(D)M$. The A-module M is without radical if and only if the ring D is without radical.

This follows from Proposition 8 of VIII, p. 108 and Theorem 2, b).

### 3. Tensor Products of Semisimple Commutative Algebras

#### Theorem 3 {#alg-viii-s12-thm-3 .statement tag=00EE}

Let $Z_1$ and $Z_2$ be semisimple commutative algebras over K. The radical of the ring $Z_1\otimes Z_2$ is equal to the set of its nilpotent elements.

Let us first treat the case when $Z_1$ and $Z_2$ are extensions $L_1$ and $L_2$ of the field K. By interchanging $L_1$ and $L_2$ if necessary, we reduce to the case when the transcendent degree of $L_1$ over K is less than that of $L_2$ over K. Choose an algebraic closure Ω of $L_2$; by Corollary 1 of Theorem 5 of V, §14, No. 6, p. 114, we may assume that $L_1$ is a subextension of Ω.

A) Let us first prove that the radical of $L_1\otimes L_2$ is contained in that of $L_1\otimes \Omega$. Set $\mathfrak{a}=\mathfrak{R}(L_1\otimes L_2)(L_1\otimes \Omega)$; it is an ideal of the commutative ring $L_1\otimes \Omega$, and we must prove that $\mathfrak{a}$ is contained in the radical of $L_1\otimes \Omega$. In other words (VIII, p. 156, Theorem 1), we must prove that for $x\in \mathfrak{a}$, the element $1 +x$ is invertible in $L_1\otimes \Omega$. Now, since Ω is an algebraic extension of $L_2$, there exists an extension $L_3$ of $L_2$, of finite degree, such that $x$ belongs to $\mathfrak{R}(L_1\otimes L_2)(L_1\otimes L_3)$. It obviously suffices to prove that $1 +x$ is invertible in $L_1\otimes L_3$. Now, $C = L_1\otimes L_3$ is a finitely generated module over the ring $B = L_1\otimes L_2$. By the corollary of VIII, p. 175, we have $\mathfrak{R}(B)C\subset \mathfrak{R}$(C), so $x$ belongs to the radical of C and $1 +x$ is invertible in C.

B) Let us prove that the radical of $L_1\otimes \Omega$ consists of nilpotent elements. Denote the characteristic exponent of K by $p$ and the relative $p$-radical (that is, purely inseparable) closure of K in Ω (V, §5, No. 2, p. 25) by P; the field P is perfect. Since P is an algebraic extension of K, we have $L_1(P) = L_1[P]$ (V, §3, No. 2, p. 18, Corollary 1). Let $\mathfrak{b}$ be the kernel of the canonical homomorphism from $L_1\otimes P$ to the field $P_1= L_1[P]$. Let $x\in \mathfrak{b}$; there exist elements $y_1, . . . , y_n$ of $L_1$ and elements $z_1, . . . , z_n$ of P such that $x=\sum^n_{i=1}y_i\otimes z_i$ and $\sum_i^n_{=1}y_iz_i= 0$. Since P is $p$-radical over K, there exists a power $q$ of $p$ such that $z^q_1, . . . , z_n^q$ belong to K. We then have

$nnnq$

$$
x^q=\sum_{i=1}y^q_i\otimes z_i^q=\sum_{i=1}y^q_iz_i^q\otimes 1 =\sum_{i=1}y_iz_i\otimes 1 = 0
$$

So $\mathfrak{b}$ consists of nilpotent elements.

Set $\mathfrak{c}=\mathfrak{b}\otimes_P\Omega$; it is the kernel of the canonical homomorphism from $(L_1\otimes P)\otimes_P\Omega$ to $P_1\otimes_P\Omega$, and it consists of nilpotent elements by the above. Now, Ω is an algebraically closed extension of P, and $P_1$ is a subextension of Ω. Since the field P is perfect, $P_1$ is a separable extension of P (V, §15, No. 5, p. 125, Theorem 3). By Theorem 4 of V, p. 120, the intersection of the maximal ideals of the commutative ring $P_1\otimes_P\Omega$ is reduced to 0. In other words, the ring $P_1\otimes_P\Omega$, which is isomorphic to $((L_1\otimes P)\otimes_P\Omega)/\mathfrak{c}$, is without radical. This proves (VIII, p. 155, Proposition 5) that $\mathfrak{c}$ contains the radical of the ring $(L_1\otimes P)\otimes_P\Omega$. Now, this ring is isomorphic to $L_1\otimes \Omega$, and $\mathfrak{c}$ consists of nilpotent elements. Therefore, the radical of $L_1\otimes \Omega$ consists of nilpotent elements.

C) End of the proof in the specific case. By A) and B), the radical $\mathfrak{r}$ of $L_1\otimes L_2$ is contained in the set $\mathfrak{n}$ of nilpotent elements of this commutative ring. We moreover know that $\mathfrak{n}$ is contained in $\mathfrak{r}$ (VIII, p. 157, Remark 2).

Now consider the general case. Since a semisimple commutative K-algebra is the product of finitely many extensions of the field K (VIII, p. 137, Proposition 3) and the radical of a product of rings is the product of the radicals (VIII, p. 156, Corollary 3), the radical of $Z_1\otimes Z_2$ is the set of nilpotent elements of this ring.

### 4. The Radical of a Tensor Product of Algebras

Let $A_1$ and $A_2$ be K-algebras, and let $A = A_1\otimes A_2$.

#### Proposition 3 {#alg-viii-s12-prop-3 .statement tag=00EF}

Suppose that the algebras $A_1$ and $A_2$ are semisimple, with respective centers $Z_1$ and $Z_2$. Set $Z = Z_1\otimes Z_2$.

a) The mapping $\mathfrak{a}\mapsto \mathfrak{a}A$ is an isomorphism from the set of ideals of Z, ordered by inclusion, to the set of two-sided ideals of A, ordered by inclusion.

b) The radical of A is equal to the intersection of the maximal two-sided ideals of A and equals $\mathfrak{R}(Z)A$.

c) If one of the K-algebras $Z_1$ and $Z_2$ is separable, in particular if the field K is perfect, then the radicals of the rings Z and A are reduced to 0.

Each algebra $A_i$ is the product of finitely many simple algebras. Now, the center of a product of rings is the product of the centers, and we have the analogous assertions for radicals (VIII, p. 156, Corollary 3) and for two-sided ideals (I, §8, No. 10, p. 109, Proposition 8). It therefore suffices to prove Proposition 3 under the assumption that $A_1$ and $A_2$ are simple algebras.

For $i\in  \{1,2\}$, set $B_i= A_i\otimes A^o_i$, and view $A_i$ as a $B_i$-module, where the homotheties are given by the formula

$$
(x\otimes y)z=xzy
$$

for $x,y$, and $z$ in $A_i$. The commutant of the $B_i$-module $A_i$ is $(Z_i)_{A_i}$, the set of homotheties by elements of $Z_i$; we identify it with $Z_i$. Moreover, the $B_i$-submodules of $A_i$ are the two-sided ideals of $A_i$, and since the ring $A_i$ is simple, the only two-sided ideals are 0 and $A_i$. Hence $A_i$ is a simple $B_i$-module. Moreover, the $(B_1\otimes B_2$)-submodules of $A_1\otimes A_2$ are the two-sided ideals of the ring $A_1\otimes A_2$.

Assertion a) therefore follows from VIII, p. 214, Theorem 2, b) applied to the simple $B_1$-module $A_1$, with commutant $Z_1$, and to the simple $B_2$-module $A_2$, with commutant $Z_2$.

Let us prove assertion b). The intersection of the maximal two-sided ideals of A is the radical of the $(B_1\otimes B_2$)-module $A_1\otimes A_2$; by Corollary 2 of VIII, p. 215, this intersection coincides with $\mathfrak{R}(Z)A$. The algebras $Z_1$ and $Z_2$ are commutative and semisimple. The radical of the ring Z therefore consists of nilpotent elements (VIII, p. 215, Theorem 3), and the two-sided ideal $\mathfrak{R}(Z)A$ of the ring A is contained in the radical $\mathfrak{R}(A)$ (VIII, p. 157, Remark 1). However, the intersection of the maximal two-sided ideals of A contains $\mathfrak{R}(A)$ (VIII, p. 155, Proposition 5, d)). This proves assertion b).

The tensor product of a separable commutative algebra and a reduced commutative algebra is a reduced ring (V, §15, No. 2, p. 120, Proposition 5). The algebras $Z_1$ and $Z_2$ are commutative and semisimple, hence reduced. If one of the algebras $Z_1$ and $Z_2$ is separable, then the algebra Z is reduced; it is therefore without radical by Theorem 3 of VIII, p. 215, and we have $\mathfrak{R}(A) =\mathfrak{R}(Z)A = 0$. This is, in particular, the case when the field K is perfect because every reduced commutative algebra over a perfect field is separable (V, §15, No. 5, p. 125, Theorem 3).

#### Corollary {#alg-viii-s12-n4-cor-1 .statement tag=00EG}

Suppose that the algebras $A_1$ and $A_2$ are simple and that the center $Z_1$ of $A_1$ is reduced to K. Then the ring $A_1\otimes A_2$ has no other two-sided ideals than 0 and itself.

By assumption, we have $Z_1= K$, and since $A_2$ is simple, its center $Z_2$ is a field (VIII, p. 121, Corollary 1, a)). The ring $Z = Z_1\otimes Z_2$ is therefore a field, and the corollary follows from Proposition 3, a).

### 5. Tensor Products of Semisimple Modules

#### Proposition 4 {#alg-viii-s12-prop-4 .statement tag=00EH}

For $i\in  \{1,2\}$, let $A_i$ be a K-algebra, $M_i$ a semisimple $A_i$-module, and $Z_i$ the center of the commutant of $M_i$. Set $A = A_1\otimes A_2$, $M = M_1\otimes M_2$, and $Z = Z_1\otimes Z_2$. We have $\mathfrak{R}_A(M) =\mathfrak{R}(Z)M$. If one of the algebras $Z_1$ and $Z_2$ is separable over K, in particular if the field K is perfect, then the A-module M is without radical.

For $i\in  \{1,2\}$, let $S_i$ be a simple $A_i$-module, $D_i$ its commutant, and $I(i)$ a set. We begin by treating the case when $M_i$ is the $A_i$-module $S_i^{(I(i))}$. We identify the center $Z_i$ of its commutant with the center of $D_i$. Set $D = D_1\otimes D_2$. We have $\mathfrak{R}(D) =\mathfrak{R}(Z)D$ (Proposition 3 of VIII, p. 217) and $\mathfrak{R}_A(S_1\otimes S_2) =$ $\mathfrak{R}(D)(S_1\otimes S_2)$ (VIII, p. 215, Corollary 2), hence $\mathfrak{R}_A(S_1\otimes S_2) =\mathfrak{R}(Z)(S_1\otimes S_2)$. The A-module M is the direct sum of a family of A-modules isomorphic to $S_1\otimes S_2$, and the radical of the direct sum of a family of modules is the direct sum of the radicals (VIII, p. 152, Corollary 2). We therefore have $\mathfrak{R}_A(M) =\mathfrak{R}(Z)M$.

Now consider the general case. For $i\in  \{1,2\}$, denote the support of the $A_i$-module $M_i$ by $\mathscr{S}_{M_i}$. For $\lambda \in \mathscr{S}_{M_i}$, denote the isotypical component of $M_i$ of type $\lambda$ by $M_{i;\lambda}$ and the center of its commutant by $Z_{i;\lambda}$. We identify the ring $Z_i$ with the product of the rings $Z_{i;\lambda}$ for $\lambda \in \mathscr{S}_{M_i}$. Let $\lambda \in \mathscr{S}_{M_1}$ and $\mu\in \mathscr{S}_{M_2}$. Denote by $i_{\lambda}: Z_{1;\lambda}\rightarrow Z_1$ the unique K-linear mapping such that pr$_{\lambda}\circ i_{\lambda}$ is the identity mapping on $Z_{1;\lambda}$ and pr$_{\lambda'}\circ i_{\lambda}$ is the zero mapping for $\lambda '\in \mathscr{S}_{M_1}-\{\lambda \}$. Define $i_\mu: Z_{2;\mu}\rightarrow Z_2$ likewise. Set $Z_{\lambda ,\mu}= Z_{1;\lambda}\otimes Z_{2;\mu}$ and $i_{\lambda ,\mu}=i_{\lambda}\otimes i_\mu$, and denote the mapping pr$_{\lambda}\otimes$ pr$_\mu$ from Z to $Z_{\lambda ,\mu}$ by $\pi_{\lambda ,\mu}$. The mapping $\pi_{\lambda ,\mu}$ is a surjective ring homomorphism; we therefore have $\pi_{\lambda ,\mu}(\mathfrak{R}(Z))\subset \mathfrak{R}(Z_{\lambda ,\mu})$ (VIII, p. 155, Proposition 5, b)). Let us prove the reverse inclusion. Let $z$ be an element of $\mathfrak{R}(Z_{\lambda ,\mu})$; since $Z_{1;\lambda}$ and $Z_{2;\mu}$ are fields, $z$ is nilpotent (Theorem 3 of VIII, p. 215). We have $i_{\lambda ,\mu}(xy) =i_{\lambda ,\mu}(x)\cdot i_{\lambda ,\mu}(y)$ for $x, y$ in $Z_{\lambda ,\mu}$; consequently, $i_{\lambda ,\mu}(z)$ is nilpotent and therefore belongs to $\mathfrak{R}(Z)$. Since $\pi_{\lambda ,\mu}\circ i_{\lambda ,\mu}$ is the identity mapping on $Z_{\lambda ,\mu}$, the element $z$ belongs to $\pi_{\lambda ,\mu}(\mathfrak{R}(Z))$. We have thus proved the equality $\pi_{\lambda ,\mu}(\mathfrak{R}(Z)) =\mathfrak{R}(Z_{\lambda ,\mu})$.

Set $M_{\lambda ,\mu}= M_{1;\lambda}\otimes M_{2;\mu}$; this is a submodule of M that is stable under Z. For $z\in Z$ and $m\in M_{\lambda ,\mu}$, we have $zm=\pi_{\lambda ,\mu}(z)m$. Consequently, $\mathfrak{R}(Z)M_{\lambda ,\mu}$ is equal to $\mathfrak{R}(Z_{\lambda ,\mu})M_{\lambda ,\mu}$ and therefore to $\mathfrak{R}_A(M_{\lambda ,\mu})$ by the isotypical case. Since the radical of a direct sum is the direct sum of the radicals (VIII, p. 152, Corollary 2) and M is the direct sum of the submodules $M_{\lambda ,\mu}$ for $(\lambda , \mu)\in \mathscr{S}_{M_1}\times \mathscr{S}_{M_2}$, the equality $\mathfrak{R}_A(M) =\mathfrak{R}(Z)M$ is proved. The last assertion then follows from Proposition 3 of VIII, p. 217.

#### Lemma 2 {#alg-viii-s12-lem-2 .statement tag=00EI}

Let $A_1$ and $A_2$ be algebras over the commutative field K. Let $M_1$ be an $A_1$-module that is finite-dimensional over K and $M_2$ a $A_2$-module of finite length. Then the $A_1\otimes A_2$-module $M_1\otimes M_2$ has finite length.

Set $M = M_1\otimes M_2$. Let $(e_1, . . . , e_n)$ be a basis of $M_1$ over the field K. The mapping $(x_1, . . . , x_n)\mapsto \sum^n_{i=1}e_i\otimes x_i$ is an isomorphism from the $A_2$-module $M^n_2$ to the $A_2$-module M. Since $M_2$ is an $A_2$-module of finite length, so is M. Moreover, every A-submodule of M is an $A_2$-submodule; consequently, M is an A-module of finite length.

#### Proposition 5 {#alg-viii-s12-prop-5 .statement tag=00RC}

Let $A_1$ and $A_2$ be algebras over the commutative field K. Let $M_1$ be a semisimple $A_1$-module that is finite-dimensional over K and $M_2$ a semisimple $A_2$-module. For $i\in  \{1,2\}$, denote the commutant of the $A_i$-module $M_i$ by $D_i$ and the center of $D_i$ by $Z_i$. Set $A = A_1\otimes A_2$, M = $M_1\otimes M_2,D = D_1\otimes D_2$, and $Z = Z_1\otimes Z_2$.

a) The commutant of the A-module M can be identified with D, and its center is Z. If the $A_2$-module $M_2$ has finite length, then the A-module M has finite length, the ring D is right and left Artinian, and the ring Z is Artinian.

b) The following properties are equivalent:

(i) The A-module M is semisimple.

(ii) The ring Z is isomorphic to the product of a family of commutative fields.

(iii) The ring Z is reduced.

c) The following properties are equivalent:

(i) The A-module M is isotypical and not reduced to 0.

(ii) The ring Z is a field.

(iii) The ring Z is an integral domain.

By assumption, $M_1$ is finite-dimensional over K. The commutant of M can therefore be identified with D (VIII, p. 213, Lemma 1), and its center is Z (III, §4, No. 4, p. 468, Corollary). Suppose that the $A_2$-module $M_2$ has finite length. The A-module M has finite length by Lemma 2. Since $M_2$ is semisimple and finitely generated, the ring $D_2$ is semisimple (VIII, p. 139, Proposition 6), and its center $Z_2$ is the product of a finite family of commutative fields. Consequently, the $D_2$-module $(D_2)_s$ and the $Z_2$-module $(Z_2)_s$ each have finite length. Furthermore, since $M_1$ is finite-dimensional over K, so are $D_1$ and $Z_1$. By Lemma 2, the module $(D_1\otimes D_2)_s$ has finite length; therefore, the ring $D_1\otimes D_2$ is left Artinian. We prove likewise that the ring $D_1\otimes D_2$ is right Artinian and that the ring $Z_1\otimes Z_2$ is Artinian. Assertion a) follows.

Let us prove b). The center of the commutant of a semisimple module is isomorphic to the product of a family of commutative fields (VIII, p. 87, Proposition 8, a)); this proves that (i) implies (ii). The implication (ii) $\Rightarrow$ (iii) is clear.

Suppose that the ring Z is reduced. We then have $\mathfrak{R}(Z) = 0$ (VIII, p. 215, Theorem 3) and $\mathfrak{R}_A(M) = 0$ (VIII, p. 218, Proposition 4). Since the $A_2$-module $M_2$ is semisimple, there exist a family $(S_i)_{i\in I}$ of simple $A_2$-modules and an isomorphism from $M_2$ to $\bigoplus S_i$. Consequently, the A-module M is isomorphic to $\bigoplus M_1\otimes S_i$. For every $i\in I$, the A-module $M_1\otimes S_i$ is therefore without radical. By a), it has finite length; hence it is semisimple (VIII, p. 153, Proposition 3, b)). The A-module M is then the direct sum of a family of semisimple modules and is consequently semisimple. This proves that (iii) implies (i) and concludes the proof of b).

An A-module is isotypical and nonzero if and only if it is semisimple and the center of its commutant is a field (VIII, p. 87, Proposition 8, b)). So c) follows from b).

#### Corollary {#alg-viii-s12-n5-cor-1 .statement tag=00EJ}

If $Z_1$ or $Z_2$ is a separable algebra over the field K (which is, for example, the case when K is perfect), then the A-module $M_1\otimes M_2$ is semisimple.

The rings $Z_1$ and $Z_2$ are isomorphic to products of fields and are therefore reduced rings. In particular, if K is perfect, they are separable algebras over K (V, §15, No. 5, p. 125, Theorem 3). By Proposition 5 of V, §15, No. 2, p. 120, the tensor product of a separable algebra and a reduced algebra is reduced. So Z is a reduced ring, and the corollary follows from Proposition 5, b).

### 6. Tensor Products of Semisimple Algebras

#### Proposition 6 {#alg-viii-s12-prop-6 .statement tag=00EK}

Let $A_1$ and $A_2$ be nonzero K-algebras. If the ring $A_1\otimes A_2$ is simple (resp. semisimple), then the rings $A_1$ and $A_2$ are simple (resp. semisimple).

A ring B is semisimple (resp. simple) if and only if the B-module $B_s$ is semisimple (resp. isotypical and nonzero). The proposition therefore follows from Proposition 1 (VIII, p. 211).

#### Proposition 7 {#alg-viii-s12-prop-7 .statement tag=00EL}

Let $A_1$ and $A_2$ be semisimple K-algebras, with respective centers $Z_1$ and $Z_2$. Suppose that $A_1$ has finite degree over K. Then the ring $A_1\otimes A_2$ is left Artinian, as is its center $Z_1\otimes Z_2$. The ring $A_1\otimes A_2$ is simple (resp. semisimple) if and only if the ring $Z_1\otimes Z_2$ is a field (resp. a reduced ring).

This is the case $M_1= (A_1)_s, M_2= (A_2)_s$ of Proposition 5 of VIII, p. 219.

#### Corollary 1 {#alg-viii-s12-prop-7-cor-1 .statement tag=00EM}

Let $A_1$ and $A_2$ be semisimple K-algebras; suppose that $A_1$ is finite-dimensional over K. Suppose that the center of $A_1$ or $A_2$ is a separable algebra over K, which is, for example, the case when K is perfect. Then $A_1\otimes A_2$ is semisimple.

This is the case $M_1= (A_1)_s, M_2= (A_2)_s$ of the corollary of VIII, p. 221.

#### Corollary 2 {#alg-viii-s12-prop-7-cor-2 .statement tag=00RD}

Let $A_1$ and $A_2$ be simple K-algebras; suppose that $A_1$ is finite-dimensional over K. If the center of $A_1$ or $A_2$ is equal to K, then the algebra $A_1\otimes A_2$ is simple. This is, in particular, the case when K is algebraically closed.

The centers $Z_1$ and $Z_2$ of $A_1$ and $A_2$, respectively, are fields; if one of the rings $Z_1$ and $Z_2$ is equal to K, then the ring $Z_1\otimes Z_2$ is a field. It therefore suffices to apply Proposition 7.

If the field K is algebraically closed, then the center of $A_1$ is equal to K.

### 7. Extension of Scalars in Semisimple Modules

#### Proposition 8 {#alg-viii-s12-prop-8 .statement tag=00EN}

Let A be a K-algebra, M an A-module, and L an extension of the field K. Denote the commutant of M by D and the center of D by Z.

a) Suppose that the $A_{(L)}$-module $M_{(L)}$ is simple (resp. isotypical, semisimple). Then the A-module M is simple (resp. isotypical, semisimple).

b) Suppose that the A-module M is semisimple and that M or L is finite-dimensional over K. The $A_{(L)}$-module $M_{(L)}$ is semisimple if and only if the ring $Z_{(L)}$ is reduced. The $A_{(L)}$-module $M_{(L)}$ is isotypical and nonzero if and only if the ring $Z_{(L)}$ is an integral domain.

c) Suppose that the A-module M is simple. The $A_{(L)}$-module $M_{(L)}$ is semisimple (resp. isotypical, simple) if and only if the ring $D_{(L)}$ is semisimple (resp. simple, a field).

Assertion a) is a specific case of Proposition 1 (VIII, p. 211), assertion b) is a specific case of Proposition 5 (VIII, p. 219), and assertion c) is a specific case of Corollary 1 of VIII, p. 215.

#### Corollary 1 {#alg-viii-s12-prop-8-cor-1 .statement tag=00EO}

a) Suppose that the A-module M is semisimple, that the extension L of K is separable, and that M or L is finite-dimensional over K. Then the $A_{(L)}$-module $M_{(L)}$ is semisimple.

b) Suppose that the A-module M is simple and that its commutant is equal to K. Then the $A_{(L)}$-module $M_{(L)}$ is simple.

Assertion a) follows from Corollary VIII, p. 221. Assertion b) is a specific case of Proposition 8, c).

#### Corollary 2 {#alg-viii-s12-prop-8-cor-2 .statement tag=00RE}

Let L be an extension of the field K. Denote the center of the K-algebra A by Z.

a) If the L-algebra $A_{(L)}$ is semisimple, then the K-algebra A is semisimple.

b) Suppose that the K-algebra A is semisimple and that L or A is finite-dimensional over K. The L-algebra $A_{(L)}$ is semisimple if and only if the ring $Z_{(L)}$ is reduced; this is, in particular, the case when L is a separable extension of K. The L-algebra $A_{(L)}$ is simple if and only if the ring $Z_{(L)}$ is an integral domain; this is, in particular, the case when the center of A is equal to K.

Assertions a) and b) follow from Proposition 8, a) and b) applied to the A-module $A_s$.

#### Proposition 9 {#alg-viii-s12-prop-9 .statement tag=00EP}

Let A be a K-algebra and L a separable extension of K.

a) If M is an A-module without radical, then the $A_{(L)}$-module $M_{(L)}$ is without radical.

b) If the K-algebra A is without radical, then the L-algebra $A_{(L)}$ is without radical.

Let us prove assertion a). Let M be an A-module without radical. We identify M with its canonical image in $M_{(L)}$. Let N be a maximal submodule of M. Since the A-module $M/N$ is simple, it follows from Proposition 4 of VIII, p. 218 that the $A_{(L)}$-module $(M/N)_{(L)}= M_{(L)}/N_{(L)}$ is without radical and therefore $\mathfrak{R}_{A_{(L)}}(M_{(L)})\subset N_{(L)}$ by Corollary 1, c) of VIII, p. 152. Now, it follows from the corollary of Proposition 14 of II, §7, No. 7, p. 306 that the intersection of the $N_{(L)}$, where N runs through the set of maximal submodules of M, is reduced to 0. Consequently, the $A_{(L)}$-module $M_{(L)}$ is without radical.

Assertion b) follows from assertion a) applied to the A-module $A_s$.

#### Proposition 10 {#alg-viii-s12-prop-10 .statement tag=00EQ}

Let A be a K-algebra and L an extension of K. Let M be an A-module.

a) We make one of the following two assumptions:

(i) The A-module M is finitely generated and L is algebraic over K.

(ii) The ring A is left Artinian.

Then we have the inclusion

$$
\mathfrak{R}_A(M)_{(L)}\subset \mathfrak{R}_{A_{(L)}}(M_{(L)})
$$

b) If L is a separable extension of K, then we have the inclusion

$$
\mathfrak{R}_{A_{(L)}}(M_{(L)})\subset \mathfrak{R}_A(M)_{(L)}
$$

Let us prove assertion a). Consider case (i). First suppose that L has finite degree over K. Then the A-module $M_{(L)}$ is finitely generated. Denote the canonical homomorphism from A to $A_{(L)}$ by $f$; the ring $A_{(L)}$ is generated by the union of its center and $f(A)$. We can therefore apply Proposition 3 of VIII, p. 174 to the $A_{(L)}$-module $M_{(L)}$. This gives the inclusion $\mathfrak{R}_A(M_{(L)})\subset \mathfrak{R}_{A_{(L)}}(M_{(L)})$ and a fortiori $\mathfrak{R}_A(M)_{(L)}\subset \mathfrak{R}_{A_{(L)}}(M_{(L)})$ (VIII, p. 152, Corollary 1).

Let us now treat the general case. Let $x_1, . . . , x_n$ be elements that generate the A-module M and $x$ an element of $\mathfrak{R}_A(M)$. Let $a_1, . . . , a_n$ be elements of $A_{(L)}$; since L is algebraic over K, there exists a finite extension $L'$ of K contained in L such that the $a_i$ belong to $A_{(L')}$. By the above, $x$ belongs to the radical of the $A_{(L')}$-module $M_{(L')}$; it follows from the corollary of VIII, p. 153 that the elements $x_i+a_ix$ for $1\leqslant i\leqslant n$ generate the $A_{(L')}$-module $M_{(L')}$ and therefore the $A_{(L)}$-module $M_{(L)}$. By the same corollary, $x$ belongs to the radical of the $A_{(L)}$-module $M_{(L)}$.

Let us now consider case (ii). Let $\mathfrak{r}$ be the radical of A, so that the radical of the A-module M is equal to $\mathfrak{r}M$ (VIII, p. 174, Corollary). The radical $\mathfrak{r}$ of A is a nilpotent two-sided ideal of A (VIII, p. 173, Proposition 1); therefore, $\mathfrak{r}_{(L)}$ is a nilpotent two-sided ideal of $A_{(L)}$. It follows that $\mathfrak{r}_{(L)}\subset \mathfrak{R}(A_{(L)})$ (VIII, p. 156, Theorem 1), and Proposition 6 of VIII, p. 158 implies $\mathfrak{R}(A_{(L)})M_{(L)}\subset \mathfrak{R}_{A_{(L)}}(M_{(L)})$. We therefore have $\mathfrak{R}_A(M) =\mathfrak{r}M\subset$ $\mathfrak{R}_{A_{(L)}}(M_{(L)})$, which concludes the proof of assertion a).

The module $M/\mathfrak{R}_A(M)$ is without radical. If L is a separable extension of K, then it follows from Proposition 9 of VIII, p. 223 that the $A_{(L)}$-module $(M/\mathfrak{R}_A(M))_{(L)}$ is without radical. Consequently, we have the inclusion

$$
\mathfrak{R}_{A_{(L)}}(M_{(L)})\subset \mathfrak{R}_A(M)_{(L)}
$$

#### Corollary {#alg-viii-s12-n7-cor-1 .statement tag=00ER}

Let L be a separable extension of K. We have $\mathfrak{R}(A_{(L)}) =$ $\mathfrak{R}(A)_{(L)}$ if L is algebraic over K or if the ring A is left Artinian.

This is the case $M = A_s$ of Proposition 10.

### Exercises {#alg-viii-s12-exercises}

See the [exercises for § 12](exercises/s12/).
