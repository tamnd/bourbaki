---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 6
section_title: Morita Equivalence of Modules and Algebras
lang: en
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.95-A VIII.117
pdf_pages: 0112-0134
extraction: native
subsections:
    - "no": 1
      title: Commutant and Duality
      page: 95
      pdf_page: 112
    - "no": 2
      title: Generating Modules and Finitely Generated Projective Modules
      page: 98
      pdf_page: 115
    - "no": 3
      title: Invertible Bimodules and Morita Equivalence
      page: 100
      pdf_page: 117
    - "no": 4
      title: The Morita Correspondence of Modules
      page: 103
      pdf_page: 120
    - "no": 5
      title: Ordered Sets of Submodules
      page: 106
      pdf_page: 123
    - "no": 6
      title: Other Properties Preserved by the Morita Correspondence
      page: 109
      pdf_page: 126
    - "no": 7
      title: Morita Equivalence of Algebras
      page: 111
      pdf_page: 128
statements: 40
exercises: 8
content_sha256: 431acdaed1fd9c52d8990f2716b199da988387715e43e6ee6eb867dc198d231e
---

## § 6. MORITA EQUIVALENCE OF MODULES AND ALGEBRAS

In this section, $k$ denotes a commutative ring.

### 1. Commutant and Duality

Let A and B be $k$-algebras. Recall (III, §4, No. 3, p. 466) that a bimodule over the algebras A and B is an $(A$, B)-bimodule P on which the two $k$-module structures deduced from the A- and B-module structures coincide. To avoid any ambiguity, we say that P is an $(A,B)_k$-bimodule. Let P be an $(A,B)_k$-bimodule. We denote by $P^*$ the dual Hom$_A(P,A)$ of the left A-module underlying P. It is a $(B,A)_k$-bimodule (II, §1, No. 14, p. 226); for $a\in A$, $b\in B,x\in P$, and $x^*\in P^*$, we have (1) $\langle x, bx^*a\rangle =\langle xb, x^*\rangle a$.

We denote by $_sA_d$ the algebra A viewed as an $(A,A)_k$-bimodule (loc. cit.) and by $\Lambda : P\otimes_BP^*\rightarrow_sA_d$ the homomorphism of $(A,A)_k$-bimodules determined by (2) $\Lambda(x\otimes x^*) =\langle x, x^*\rangle$

for $x\in P$ and $x^*\in P^*$. We denote by $\widetilde{P}$ the dual Hom$_B(P,B)$ of the right B-module underlying P; it is a $(B,A)_k$-bimodule. We denote by $\widetilde{\Lambda} :\widetilde{P}\otimes_AP\rightarrow_sB_d$ the homomorphism of $(B,B)_k$-bimodules determined by (3) $\widetilde{\Lambda}(\widetilde{x}\otimes x) =\langle \widetilde{x}, x\rangle$

for $x\in P$ and $\widetilde{x}\in \widetilde{P}$.

Now, suppose that the mapping $b\mapsto b_P$ is a bijection from B to End$_A(P)$; it is then an isomorphism from B to the opposite algebra of End$_A(P)$. The canonical homomorphism of $\mathbf{Z}$-modules from $P^*\otimes_AP$ to End$_A(P)$ (II, §4, No. 2, p. 271) then determines a homomorphism of $\mathbf{Z}$-modules $\Theta : P^*\otimes_AP\rightarrow$ B defined by (4) $x\Theta(x^*\otimes y) =\langle x, x^*\rangle y$ for $x, y\in P$ and $x^*\in P^*$. Because of (1), this homomorphism is $(B$, B)-linear, and we have (5) $\Theta(x^*\otimes y)y^*=x^*\langle y, y^*\rangle$ for $y\in P$ and $x^*, y^*\in P^*$. From (4) and (5), we deduce the following equalities in the $(B,B)_k$-bimodule $P^*\otimes_AP:$

$$
(y^*\otimes x)\Theta(x^*\otimes y) =y^*\otimes  \langle x, x^*\rangle y=y^*\langle x, x^*\rangle  \otimes y= \Theta(y^*\otimes x)(x^*\otimes y)
$$

for $x, y\in P$ and $x^*, y^*\in P^*$, and therefore (6) $s\Theta(t) = \Theta(s)t$ for $s, t\in P^*\otimes_AP$. Likewise, for $x, y$ in P and $x^*, y^*$ in $P^*$, we deduce the following equalities in the $(A,A)_k$-bimodule $P\otimes_BP^*$ from (4) and (5):

$$
(x\otimes x^*)\langle y, y^*\rangle =x\otimes \Theta(x^*\otimes y)y^*=x\Theta(x^*\otimes y)\otimes y^*=\langle x, x^*\rangle (y\otimes y^*)
$$

and therefore (7) $u\Lambda(v) = \Lambda(u)v$ for $u, v\in P\otimes_BP^*$.

For any element $x^*$ of $P^*$, denote the B-linear mapping $x\mapsto \Theta(x^*\otimes x)$ from P to B by $\sigma (x^*)$. We thus define a mapping $\sigma$ from $P^*$ to $\widetilde{P}$ that is $(B$, A)-linear and satisfies, by definition, (8) $\Theta(x^*\otimes y) =\langle \sigma (x^*), y\rangle$ for $x^*\in P^*$ and $y\in P$. By the definition of $\widetilde{\Lambda}$, we therefore have (9) $\Theta =\widetilde{\Lambda}\circ (\sigma \otimes 1_P)$.

Suppose that the mapping $a\mapsto a_P$ from A to End$_B(P)$ is bijective; it is then an algebra isomorphism. Analogously, we define a homomorphism of $(A,A)_k$-bimodules $\widetilde{\Theta} : P\otimes_B\widetilde{P}\rightarrow_sA_d$ by setting (10) $\widetilde{\Theta}(x\otimes \widetilde{y})y=x\langle \widetilde{y}, y\rangle$ for $x, y\in P$ and $\widetilde{y}\in \widetilde{P}$. We also define a homomorphism of $(B,A)_k$-bimodules $\widetilde{\sigma}:\widetilde{P}\rightarrow P^*$ by setting (11) $\widetilde{\Theta}(x\otimes \widetilde{y}) =\langle x,\widetilde{\sigma}(\widetilde{y})\rangle$ for $x\in P,\widetilde{y}\in \widetilde{P}$. We have (12) $\widetilde{\Theta} = \Lambda\circ (1_P\otimes \widetilde{\sigma})$.

#### Proposition 1 {#alg-viii-s6-prop-1 .statement tag=006R}

Suppose that the mappings $b\mapsto b_P$ from B to End$_A(P)$ and $a\mapsto a_P$ from A to End$_B(P)$ are bijective. Then $\sigma$ and $\widetilde{\sigma}$ are inverse isomorphisms, and we have the relations (13) $\Lambda =\widetilde{\Theta}\circ (1_P\otimes \sigma )$, (14) $\widetilde{\Lambda} = \Theta\circ (\widetilde{\sigma}\otimes 1_P)$.

For $x\in P,x^*\in P^*$, and $y\in P$, by relations (4), (8), (10), and (11), we have $(15)\langle x, x^*\rangle y=x\Theta(x^*\otimes y) =x\langle \sigma (x^*), y\rangle =\widetilde{\Theta}(x\otimes \sigma (x^*))y=\langle x,\widetilde{\sigma}(\sigma (x^*))\rangle y$. Likewise, for $x\in P,\widetilde{y}\in \widetilde{P}$, and $y\in P$, we have (16) $x\langle \widetilde{y}, y\rangle =\widetilde{\Theta}(x\otimes \widetilde{y})y=\langle x,\widetilde{\sigma}(\widetilde{y})\rangle y=x\Theta (\widetilde{\sigma}(\widetilde{y})\otimes y) =x\langle \sigma (\widetilde{\sigma}(\widetilde{y})), y\rangle$.

Because of the assumptions, P is faithful as an A-module and as a B-module. From relations (15) and (16), respectively, we deduce $\widetilde{\sigma}\circ \sigma = 1_{P^*}$ and $\sigma \circ \widetilde{\sigma}=$ $1_{\widetilde{P}}$. Relations (13) and (14) then follow from (12) and (9), respectively.

#### Remark 1 {#alg-viii-s6-n1-rem-1 .statement tag=006S}

Suppose that the mapping $b\mapsto b_P$ from B to End$_A(P)$ is bijective. Then

a) the B-module P can be identified with the countermodule of P; it is therefore faithful and balanced;

b) the mapping $a\mapsto a_P$ from A to End$_B(P)$ is bijective if and only if the A-module P is faithful and balanced.

#### Remark 2 {#alg-viii-s6-n1-rem-2 .statement tag=006T}

Under the assumptions of Proposition 1, the A-module P is balanced; since the rings $A_P$ and $A'_P$ have the same center (VIII, p. 77), there is an isomorphism $\varphi$ from the center Z(A) of the ring A to the center Z(B) of the ring B, determined by the relation $\varphi (z)_P=z_P$ for $z\in Z(A)$. Moreover, the endomorphisms of the $(A,B)_k$-bimodule P are the homotheties $z_P$ where $z$ runs through Z(A); the automorphisms of the $(A,B)_k$-bimodule P are the homotheties $z_P$ where $z$ is invertible in Z(A).

### 2. Generating Modules and Finitely Generated Projective Modules

#### Proposition 2 {#alg-viii-s6-prop-2 .statement tag=006U}

Let A and B be algebras over $k$, and let P be an $(A,B)_k$-bimodule. Suppose that the mapping $b\mapsto b_P$ from B to End$_A(P)$ is bijective. The following assertions are equivalent:

(i) The A-module P is projective and finitely generated.

(ii) The mapping Θ (VIII, p. 96) is an isomorphism of $(B,B)_k$-bimodules from $P^*\otimes_AP$ to $_sB_d$.

(iii) The image of Θ contains the unit element of B. If, moreover, the mapping $a\mapsto a_P$ from A to End$_B(P)$ is bijective, then the assertions above are equivalent to the following statement:

(iv) There exist a $(B,A)_k$-bimodule Q and a surjective homomorphism of $(B,B)_k$-bimodules from $Q\otimes_AP$ to $_sB_d$.

By the corollary of II, §4, No. 2, p. 271, assertion (i) implies (ii). Moreover, (iii) follows from (ii). Let $t\in B^*\otimes_AB$ be such that $\Theta(t) = 1$. Let $n$ be an integer, and let $(x_1, . . . , x_n)\in P^n$ and $(x^*_1, . . . , x^*_n)\in P^{*n}$ be such that $t=\sum^n_{i=1}x^*_i\otimes x_i$. For every $x$ belonging to P, the relation $x\Theta(t) =x$ can be written as

$$
\sum_{i=1}^n\langle x, x^*_i\rangle x_i=x
$$

It follows that the A-module P is finitely generated by the family $(x_i)_{1\leqslant i\leqslant n}$, and we conclude the proof of the implication (iii) $\Rightarrow$ (i) using Proposition 12 of II, §2, No. 6, p. 238.

We obviously have (ii) $\Rightarrow$ (iv). Let Q be a $(B,A)_k$-bimodule and $\theta$ a surjective homomorphism of $(B,B)_k$-bimodules from $Q\otimes_AP$ to $_sB_d$. In the notation of the previous subsection, there exists a homomorphism of $(B,A)_k$-bimodules $\zeta : Q\rightarrow \widetilde{P}$ such that $\theta (y\otimes x) =\langle \zeta (y), x\rangle$ for $x\in P$ and $y\in Q$, and we have $\theta =\widetilde{\Lambda}\circ (\zeta \otimes 1_P)$. Since $\theta$ is surjective, the same holds for $\widetilde{\Lambda}$. If the mapping $a\mapsto a_P$ from A to End$_B(P)$ is bijective, then Θ is surjective by relation (14) of Proposition 1 of VIII, p. 97; the implication (iv) $\Rightarrow$ (iii) follows.

#### Proposition 3 {#alg-viii-s6-prop-3 .statement tag=006V}

Let A and B be algebras over $k$ and P an $(A,B)_k$-bimodule. The following properties are equivalent:

(i) The A-module P is generating.

(ii) The image of the mapping Λ from $P\otimes_BP^*$ to $_sA_d$ (VIII, p. 95) contains the unit element.

(iii) There exist a $(B,A)_k$-bimodule Q and a surjective homomorphism of $(A,A)_k$-bimodules from $P\otimes_BQ$ to $_sA_d$. If, moreover, the mapping $b\mapsto b_P$ from B to End$_A(P)$ is bijective, then the assertions are equivalent to the following statement:

(iv) The mapping Λ is an isomorphism from $P\otimes_BP^*$ to $_sA_d$. (i) $\Leftrightarrow$ (ii): The image of Λ is the trace ideal $\tau (P)$ (VIII, p. 80). The equivalence of (i) and (ii) therefore follows from Theorem 1 of VIII, p. 80. (ii) $\Rightarrow$ (iii): It suffices to take $Q = P^*$. (iii) $\Rightarrow$ (ii): Let Q be a $(B,A)_k$-bimodule and $\psi$ a homomorphism of $(A,A)_k$-bimodules from $P\otimes_BQ$ to $_sA_d$. There exists a homomorphism of $(B,A)_k$-bimodules Ψ from Q to $P^*$ such that $\psi (x\otimes y) =\langle x,\Psi(y)\rangle$ for $x\in P$ and $y\in Q$, and we have the equality $\psi = \Lambda\circ (1_P\otimes \Psi)$. If $\psi$ is surjective, then so is Λ.

It is clear that (iv) implies (ii). Conversely, suppose that property (ii) holds and that the mapping $b\mapsto b_P$ from B to End$_A(P)$ is bijective. Let $e$ be an element of $P\otimes_BP^*$ such that $\Lambda(e) = 1$. By relation (7) of VIII, p. 96, we have $u= \Lambda(u)e$ for every $u$ in $P\otimes_BP^*$; the injectivity of Λ follows.

#### Proposition 4 {#alg-viii-s6-prop-4 .statement tag=006W}

Let A and B be $k$-algebras and P an $(A,B)_k$-bimodule. Suppose that the mapping $b\mapsto b_P$ from B to End$_A(P)$ is bijective.

a) If the A-module P is generating, then the right B-module P is projective and finitely generated.

b) If the A-module P is projective and finitely generated, then the right B-module P is generating.

Suppose that the A-module P is generating. It is then faithful and balanced (VIII, p. 82, Theorem 2), and consequently the mapping $a\mapsto a_P$ from A to End$_B(P)$ is bijective (VIII, p. 97, Remark 1). Moreover, the mapping $\Lambda : P\otimes_BP^*\rightarrow_sA_d$ is bijective (VIII, p. 98, Proposition 3). We view P as a $(B^o,A^o)_k$-bimodule. The mapping Λ induces a bijective mapping $P^*\otimes_{B^o}P\rightarrow A^o$; by Proposition 2 of VIII, p. 98, (iv) $\Rightarrow$ (i), the right B-module P is projective and finitely generated.

Now, suppose that the A-module P is projective and finitely generated. Then the mapping $\Theta : P^*\otimes_AP\rightarrow_sB_d$ is bijective (loc. cit., (i) $\Rightarrow$ (ii)). By the implication (iii) $\Rightarrow$ (i) of Proposition 3 above applied to the $(B^o,A^o)_k$-bimodule P, the right B-module P is generating.

#### Corollary 1 {#alg-viii-s6-prop-4-cor-1 .statement tag=006X}

The countermodule of a generating module is projective and finitely generated. The countermodule of a finitely generated projective module is generating.

Let A be a $k$-algebra, and let M be an A-module. We denote the opposite $k$-algebra of the algebra End$_A(M)$ by B. The corollary follows from Proposition 4 applied to the $(A,B)_k$-bimodule M.

#### Corollary 2 {#alg-viii-s6-prop-4-cor-2 .statement tag=006Y}

Let A and B be $k$-algebras and P an $(A,B)_k$-bimodule. The following properties are equivalent:

(i) The A-module P is generating, and the mapping $b\mapsto b_P$ from B to End$_A(P)$ is bijective.

(ii) The right B-module P is projective, finitely generated, faithful, and balanced, and the mapping $a\mapsto a_P$ from A to End$_B(P)$ is bijective.

The implication (i) $\Rightarrow$ (ii) follows from Proposition 4, a) and Remark 1 (VIII, p. 97). Assume that (ii) holds; then the A-module P is generating (Proposition 4, b) applied to the $(B^o,A^o)_k$-bimodule P). Since the B-module P is faithful and balanced, the second assertion of (i) is also satisfied (VIII, p. 97, Remark 1).

### 3. Invertible Bimodules and Morita Equivalence

#### Definition 1 {#alg-viii-s6-def-1 .statement tag=006Z}

Let A and B be $k$-algebras and P an $(A,B)_k$-bimodule. We say that P is invertible if there exists a $(B,A)_k$-bimodule Q such that $P\otimes_BQ$ is isomorphic to $_sA_d$ and $Q\otimes_AP$ to $_sB_d$. Such a bimodule Q is called an inverse of P.

Let A and B be $k$-algebras, and let P be an invertible $(A,B)_k$-bimodule. Let C be a $k$-algebra and $P'$ an invertible $(B,C)_k$-bimodule. Finally, let Q and $Q'$ be inverse bimodules of P and $P'$, respectively. By the associativity of the tensor product (II, §3, No. 8, p. 258, Proposition 8) and Proposition 4 of II, §3, No. 4, p. 249, the $(C,A)_k$-bimodule $Q'\otimes_BQ$ is an inverse of the $(A,C)_k$-bimodule $P\otimes_BP'$, so that $P\otimes_BP'$ is an invertible $(A,C)_k$-bimodule.

Hence, the relation “A and B are $k$-algebras, and there exists an invertible $(A,B)_k$-bimodule” is an equivalence relation.

#### Definition 2 {#alg-viii-s6-def-2 .statement tag=0070}

Two $k$-algebras A and B are called Morita equivalent if there exists an invertible $(A,B)_k$-bimodule. Rings A and B are called Morita equivalent if the $\mathbf{Z}$-algebras A and B are Morita equivalent.

Two isomorphic $k$-algebras are Morita equivalent. If two $k$-algebras are Morita equivalent, then their opposite algebras are Morita equivalent.

Let P be an invertible $(A,B)_k$-bimodule and Q an inverse of P. Then Q is an invertible $(B,A)_k$-bimodule, and it has P as inverse. Moreover, viewed as a $(B^o,A^o)_k$-bimodule, P is invertible and has the $(A^o,B^o)_k$-bimodule Q as inverse.

#### Lemma 1 {#alg-viii-s6-lem-1 .statement tag=0071}

Let A and B be $k$-algebras, P be an invertible $(A,B)_k$-bimodule, M and N be B-modules, and $u: M\rightarrow N$ be a B-linear mapping. If the mapping $1_P\otimes u: P\otimes_BM\rightarrow P\otimes_BN$ is zero (resp. bijective), then so is $u$.

Let Q be a bimodule inverse to P and $\theta : Q\otimes_AP\rightarrow_sB_d$ an isomorphism of $(B,B)_k$-bimodules. The lemma follows from the commutativity of the diagram

$Q\otimes_AP\otimes_BM^{1_Q\otimes 1_P\otimes u}/$/ $Q\otimes_AP\otimes_BN$

$\theta \otimes 1_M\theta \otimes 1_M$

M $u$ // N .

#### Theorem 1 {#alg-viii-s6-thm-1 .statement tag=0072}

Let A and B be $k$-algebras and P an $(A,B)_k$-bimodule. Denote the $(B,A)_k$-bimodule Hom$_A(P,A_s)$ by $P^*$. The following properties are equivalent:

(i) The $(A,B)_k$-bimodule P is invertible.

(ii) The A-module P is projective, finitely generated, and generating, and the mapping $b\mapsto b_P$ from B to End$_A(P)^o$ is a $k$-algebra isomorphism.

(iii) The right B-module P is projective, finitely generated, and generating, and the mapping $a\mapsto a_P$ from A to End$_B(P)$ is a $k$-algebra isomorphism. If these properties hold, then the homomorphisms

$\Theta : P^*\otimes P\rightarrow_sB_d$ and $\Lambda : P\otimes P^*\rightarrow_sA_d$

are isomorphisms, so that the $(B,A)_k$-bimodule $P^*$ is an inverse of P.

If property (ii) holds, then P is an invertible $(A,B)_k$-bimodule with inverse $P^*$ (VIII, p. 98, Proposition 2 and p. 98, Proposition 3). This proves that (ii) implies (i) and the last assertion.

Suppose that the $(A,B)_k$-bimodule P is invertible. Then the A-module P is generating (VIII, p. 98, Proposition 3, (iii) $\Rightarrow$ (i)). It is therefore faithful and balanced (VIII, p. 82, Theorem 2) and, consequently, the mapping $a\mapsto a_p$ from A to End$_B(P)$ is bijective.

Let us now prove that the mapping $b\mapsto b_P$ from B to End$_A(P)$ is bijective. Let Q be a $(B,A)_k$-bimodule, inverse to P. Let $u\in$ End$_A(P)$; then $1_Q\otimes u$ is an endomorphism of the left B-module $Q\otimes_AP$. Since the $(B,B)_k$-bimodule $Q\otimes_AP$ is isomorphic to $_sB_d$, there exists a unique element $b$ of B such that $1_Q\otimes u$ is the homothety with ratio $b$ of the right B-module $Q\otimes_AP$. Consequently, we have $1_Q\otimes (u-b_P) = 0$. Hence, $u=b_P$ by Lemma 1; this proves that the mapping $b\mapsto b_P$ from B to End$_A(P)$ is bijective.

By Proposition 2 of VIII, p. 98, the A-module P is then projective and finitely generated. We have therefore proved the equivalence of (i) and (ii).

By interchanging the roles of A and B, we obtain the equivalence of (i) and (iii), which concludes the proof of the proposition.

#### Corollary 1 {#alg-viii-s6-thm-1-cor-1 .statement tag=0073}

Let A and B be Morita equivalent $k$-algebras, and let P be an invertible $(A,B)_k$-bimodule. There exists an isomorphism $\varphi$ from the center Z(A) of A to the center of B determined by the relation $\varphi (z)_P=z_P$ for every $z\in Z(A)$. The automorphisms of the $(A,B)_k$-bimodule P are the homotheties $z_P$ where $z$ is an invertible element of Z(A).

Given Theorem 1, this follows from Remark 2 of VIII, p. 97.

#### Corollary 2 {#alg-viii-s6-thm-1-cor-2 .statement tag=0074}

Let A and B be Morita equivalent $k$-algebras, and let P be an invertible $(A,B)_k$-bimodule. Every $(B,A)_k$-bimodule inverse to P is isomorphic to the dual $P^*=$ Hom$_A(P,A)$ of P. More precisely, let Q be a $(B,A)_k$-bimodule that is an inverse of P, and let $\lambda : P\otimes_BQ\rightarrow_sA_d$ be an isomorphism of $(A,A)_k$-bimodules. There exists a unique mapping $\tau : Q\rightarrow P^*$ determined by the relation $\langle p, \tau (q)\rangle =\lambda (p\otimes q)$ for $p\in P$ and $q\in Q$, and $\tau$ is an isomorphism of $(B,A)_k$-bimodules.

The existence and uniqueness of the mapping $\tau$ are clear. It is a homomorphism of $(B,A)_k$-bimodules, and we have $\lambda = \Lambda\circ (1_P\otimes \tau )$. Since $\lambda$ and Λ are isomorphisms of $(A,A)_k$-bimodules (VIII, p. 101, Theorem 1), so is $1_P\otimes \tau$. By Lemma 1, the mapping $\tau$ is bijective.

#### Remark {#alg-viii-s6-n3-rem-1 .statement tag=0075}

Under the assumptions of the corollary, let $q$ be an element of Q such that we have $\lambda (p\otimes q) = 0$ for every $p\in P$. We then have $\tau (q) = 0$, that is, $q= 0$. Likewise, if $p$ is an element of P such that we have $\lambda (p\otimes q) = 0$ for every $q\in Q$, then $p= 0$.

#### Example 1 {#alg-viii-s6-n3-exa-1 .statement tag=0076}

Let B be a $k$-algebra, $n$ an integer $\geqslant 1$, and A the $k$-algebra $\mathbf{M}_n(B)$. The right B-module $P = B^n_d$ is projective, finitely generated, and generating, and A can be identified with the endomorphism algebra of P (II, §10, No. 7, p. 349). By Theorem 1, the $(A,B)_k$-bimodule P is invertible. The algebras B and $\mathbf{M}_n(B)$ are therefore Morita equivalent.

$2)*$ Let A be a commutative $k$-algebra and P an A-module. We view P as an $(A,A)_k$-bimodule whose two laws of action are equal. If the $(A,A)_k$-bimodule P is invertible, then the A-module P is finitely generated (Theorem 1). By Theorem 3 of Comm. Alg., II, §5, No. 4, p. 114, the following properties are equivalent:

(i) The $(A,A)_k$-bimodule P is invertible.

(ii) There exists an A-module Q such that $P\otimes_AQ$ is isomorphic to A.

(iii) The A-module P is projective, finitely generated, and of rank $1.*$

### 4. The Morita Correspondence of Modules

In this subsection, the letters A and B denote Morita equivalent $k$-algebras and P an invertible $(A,B)_k$-bimodule. Choose a $(B,A)_k$-bimodule Q inverse to P and isomorphisms

$\lambda : P\otimes_BQ\rightarrow_sA_d$ and $\theta : Q\otimes_AP\rightarrow_sB_d$.

For any left B-module V, denote by $\theta_V$ the homomorphism of B-modules $\theta \otimes 1_V: Q\otimes_AP\otimes_BV\rightarrow V$; it is an isomorphism since $\theta$ is an isomorphism. Likewise, for every left A-module M, denote by $\lambda_M$ the homomorphism of A-modules $\lambda \otimes 1_M: P\otimes_BQ\otimes_AM\rightarrow M$; it is an isomorphism since $\lambda$ is an isomorphism.

#### Theorem 2 {#alg-viii-s6-thm-2 .statement tag=00S2}

a) Let V and W be left B-modules. The mapping $g\mapsto 1_P\otimes g$ is a bijection from Hom$_B(V,W)$ to Hom$_A(P\otimes_BV,P\otimes_BW)$. The inverse bijection sends an element $h$ of Hom$_A(P\otimes_BV,P\otimes_BW)$ to the element $\theta_W\circ (1_Q\otimes h)\circ \theta_V^{-1}$ of Hom$_B(V,W)$.

b) Every left A-module M is isomorphic to a module of the form $P\otimes_BV$, where V is a left B-module.

Let V and W be left B-modules. By Lemma 1 of VIII, p. 101, the mapping $\varphi :g\mapsto 1_P\otimes g$ from Hom$_B(V,W)$ to Hom$_A(P\otimes_BV,P\otimes_BW)$ is injective. By interchanging the roles of P and Q (and of A and B), we see that the mapping $\psi :h\mapsto 1_Q\otimes h$ from Hom$_A(P\otimes_BV,P\otimes_BW)$ to Hom$_A(Q\otimes_AP\otimes_BV,Q\otimes_AP\otimes_BW)$ is also injective. Now, the composition $\psi \circ \varphi$ is the mapping $g\mapsto \theta^-_W^1\circ g\circ \theta_V$. It is bijective, hence so is $\psi$. Consequently, $\varphi$ is bijective, and its inverse is the mapping $h\mapsto \theta_W\circ (1_Q\otimes h)\circ \theta^-_V^1$.

Assertion b) follows from the fact that $\lambda_M$ is an isomorphism from $P\otimes_B$ $\otimes_A\otimes M$ to M.

Let V be a left B-module and W a submodule of V. Since the B-module P is projective (VIII, p. 101, Theorem 1), the canonical mapping from $P\otimes_BW$ to $P\otimes_BV$ is injective. We identify $P\otimes_BW$ with its image in $P\otimes_BV$ through this mapping. We adopt the analogous conventions when P and B are replaced by Q and A.

#### Proposition 5 {#alg-viii-s6-prop-5 .statement tag=0077}

Let V be a left B-module. The mapping $W\mapsto P\otimes_BW$ is an isomorphism from the set of B-submodules of V, ordered by inclusion, to the set of A-submodules of $P\otimes_BV$, ordered by inclusion. The inverse isomorphism sends an A-submodule N of $P\otimes_BV$ to the image under $\theta_V$ of the B-submodule $Q\otimes_AN$ of $Q\otimes_AP\otimes_BV$.

Denote by $D_B(V)$ the set of B-submodules of V, ordered by inclusion, and define the sets $D_A(P\otimes_BV)$ and $D_B(Q\otimes_AP\otimes_BV)$ likewise. Let $\varphi : D_B(V)\rightarrow$ $D_A(P\otimes_BV)$ be the mapping $W\mapsto P\otimes_BW$ and $\psi$ the mapping from $D_A(P\otimes_BV)$ to $D_B(Q\otimes_AP\otimes_BV)$ given by $N\mapsto Q\otimes_AN$. These are increasing mappings, and the composition $\psi \circ \varphi$ is the mapping $W\mapsto \theta^-_V^1$(W), which is bijective. Consequently, $\varphi$ is injective, and $\psi$ is surjective. By replacing B with A and V with $P\otimes_BV$, we see that $\psi$ is also injective. Hence, $\varphi$ and $\psi$ are bijective, and the inverse mapping of $\varphi$ is indeed that described in the proposition.

#### Example 1 {#alg-viii-s6-n4-exa-1 .statement tag=0078}

Let us apply Proposition 5 of VIII, p. 104, to the specific case $V = B_s$.

a) The mapping $J\mapsto$ PJ is an isomorphism from the ordered set $D(B_s)$ of left ideals of B to the ordered set D(P) of A-submodules of P. The inverse mapping sends an A-submodule M of P to the left ideal J(M) of B consisting of the elements $b$ of B such that M contains $Pb$.

b) The mapping $K\mapsto$ KP is an isomorphism from the ordered set $D(A_d)$ of right ideals of A to the ordered set D(P) of B-submodules of P. The inverse mapping sends a B-submodule V of P to the right ideal K(V) of A consisting of the elements $a$ of A such that V contains $aP$.

Indeed, the A-module $P\otimes_BB_s$ can be canonically identified with P. If J is a left ideal of B, then the canonical image of $P\otimes_BJ$ in $P\otimes_BB_s$ corresponds to PJ through this identification. Consequently, the mapping $J\mapsto$ PJ is an isomorphism of ordered sets from $D(B_s)$ to D(P). Let $J\in D(B_s)$. Denote the set of elements $b$ of B such that PJ contains $Pb$ by $J'$. It is a left ideal of B that contains J, and we have PJ$'\subset$ PJ. Since the mapping $J\mapsto$ PJ is an isomorphism of ordered sets, we necessarily have PJ$'=$ PJ and $J = J'$. This proves a).

Assertion b) follows from assertion a) applied to the invertible $(B^o,A^o)_k$-bimodule P.

Note that the ring A is a field if and only if the B-module P is simple.

#### Example 2 {#alg-viii-s6-n4-exa-2 .statement tag=0079}

Denote by $\mathscr{B}_A,\mathscr{B}_B$, and $\mathscr{B}_P$ the sets of two-sided ideals of A, two-sided ideals of B, and $(A,B)_k$-sub-bimodules of P, respectively.

a) The mapping $\mathfrak{b}\mapsto P\mathfrak{b}$ is an isomorphism of ordered sets from $\mathscr{B}_B$ to $\mathscr{B}_P$; the inverse isomorphism sends an $(A,B)_k$-sub-bimodule $P'$ of P to the two-sided ideal of B consisting of the elements $b$ such that $Pb\subset P'$.

b) The mapping $\mathfrak{a}\mapsto \mathfrak{a}P$ is an isomorphism of ordered sets from $\mathscr{B}_A$ to $\mathscr{B}_P$; the inverse isomorphism sends an $(A,B)_k$-sub-bimodule $P'$ of P to the two-sided ideal of A consisting of the elements $a$ such that $aP\subset P'$.

Indeed, let J be a left ideal of B and $P'=$ PJ. Then $P'$ is an A-submodule of P and, by Example 1, the ideal J consists of the elements $b$ of B such that $Pb\subset P'$. Moreover, $P'$ is an $(A,B)_k$-sub-bimodule of P if and only if J is a two-sided ideal of B. Thus a) follows from loc. cit.

Assertion b) follows from assertion a) applied to the invertible $(B^o,A^o)_k$-bimodule P.

#### Proposition 6 {#alg-viii-s6-prop-6 .statement tag=007A}

Denote by $\mathscr{B}_A$ and $\mathscr{B}_B$ the sets of two-sided ideals of A and two-sided ideals of B.

a) There exists an isomorphism of ordered sets $f$ from $\mathscr{B}_A$ to $\mathscr{B}_B$ determined by the following property: if $\mathfrak{a}$ is a two-sided ideal of A and $\mathfrak{b}$ a two-sided ideal of B, then the relation $f(\mathfrak{a}) =\mathfrak{b}$ is equivalent to $\mathfrak{a}P = P\mathfrak{b}$.

b) Suppose that the ring A is commutative, so that A can be identified with the center of B (VIII, p. 102, Corollary 1). The isomorphism $f:\mathscr{B}_A\rightarrow$ $\mathscr{B}_B$ sends an ideal $\mathfrak{a}$ of A to the two-sided ideal $B\mathfrak{a}$ of B, and we have $\mathfrak{a}= A\cap B\mathfrak{a}$.

Assertion a) follows from Example 2.

Now, suppose that A is commutative, and identify A with the center of B. Let $\mathfrak{a}$ be an ideal of A. Then $B\mathfrak{a}$ is a two-sided ideal of B; we have PB$\mathfrak{a}=\mathfrak{a}P$ and therefore $f(\mathfrak{a}) = B\mathfrak{a}$. Let $\mathfrak{a}'$ be the ideal $A\cap B\mathfrak{a}$ of A; it is contained in $B\mathfrak{a}$ and contains $\mathfrak{a}$, so $B\mathfrak{a}'$ is equal to $B\mathfrak{a}$. Since $f$ is bijective, it follows that $\mathfrak{a}'=\mathfrak{a}$.

#### Example 3 {#alg-viii-s6-n4-exa-3 .statement tag=007B}

Let V be a left B-module. Then the correspondence given above sends the annihilator of the B-module V to the annihilator of the A-module $P\otimes_BV$. Indeed, denote the annihilator of the A-module $P\otimes_BV$ by $\mathfrak{a}$ and that of the B-module V by $\mathfrak{b}$. Let W be the $(A,B)_k$-sub-bimodule of P consisting of the elements such that $p\otimes v= 0$ for every element $v$ of V. We have the inclusion $P\mathfrak{b}\subset W$; conversely, for every $p\in W$ and $q\in Q$, we have that $\theta (q\otimes p)$ belongs to $\mathfrak{b}$. Hence, the element $\mathfrak{b}$ of $D(B_s)$ corresponds to the element W of D(P). Likewise, $\mathfrak{a}\in D(A_d)$ corresponds to W.

#### Example 4 {#alg-viii-s6-n4-exa-4 .statement tag=007C}

For any two-sided ideal $\mathfrak{a}$ of A, denote the subset of $\mathbf{M}_n(A)$ consisting of the matrices with entries in $\mathfrak{a}$ by $\mathbf{M}_n(\mathfrak{a})$. It is a two-sided ideal of $\mathbf{M}_n(A)$. We have $\mathbf{M}_n(\mathfrak{a})A^n=\mathfrak{a}^n= A^n\mathfrak{a}$. It follows from Proposition 6 that every two-sided ideal of $\mathbf{M}_n(A)$ is of the form $\mathbf{M}_n(\mathfrak{a})$, where $\mathfrak{a}$ is a two-sided ideal of A.

#### Remark {#alg-viii-s6-n4-rem-1 .statement tag=007D}

We keep the assumptions and notation above and suppose that the $(B,A)_k$-bimodule Q is the dual $P^*$ of the A-module P and that the isomorphisms $\lambda$ and $\theta$ are the canonical mappings $\Lambda : P\otimes_BP^*\rightarrow_sA_d$ and Θ : $P^*\otimes_AP\rightarrow_sB_d$ (VIII, p. 101, Theorem 1). Since the A-module P is projective and finitely generated, we have a canonical isomorphism $\vartheta_M: P^*\otimes_AM\rightarrow$ Hom$_A(P,M)$ for every A-module M (II, §4, No. 2, p. 271, Corollary). We leave it to the reader to reformulate the results of Subsections 3 and 4 by replacing the construction $M\mapsto Q\otimes_AM$ with the construction $M\mapsto$ Hom$_A(P,M)$.

### 5. Ordered Sets of Submodules

In this subsection, A and B are $k$-algebras, M is a left A-module, and V is a left B-module. We denote by D(M) (resp. D(V)) the set of submodules of M (resp. of V), ordered by inclusion. We assume given an isomorphism of ordered sets $\varphi : D(V)\rightarrow D(M)$.

By Morita’s theorem (VIII, p. 103, Theorem 2), we obtain such an isomorphism in the following situation: P is an invertible $(A,B)_k$-bimodule, M is the A-module $P\otimes_BV$, and for every submodule W of $V,\varphi (W)$ is the canonical image of $P\otimes_BW$ in M.

Some properties of the module M, or of its submodules, can be expressed in terms of the ordered set D(M): they are listed in Tables I and II.

The module M is the direct sum of a family $(M_i)_{i\in I}$ of submodules if and only if we have $M =\sum_{i\in I}M_i$ and $M_i\cap \sum_{j\not=i}M_j= 0$ for every $i\in I$. This remark and an examination of Table I give the following result.

#### Proposition 7 {#alg-viii-s6-prop-7 .statement tag=007E}

a) We have $\varphi (0) = 0$ and $\varphi (V) = M$.

b) Let $(V_i)_{i\in I}$ be a family of submodules of V. We have

$$
\varphi \sum_{i\in I}V_i=\sum_{i\in I}\varphi (V_i),\varphi \bigcap_{i\in I}V_i=\bigcap_{i\in I}\varphi (V_i)
$$

Submodules of M Ordered set D(M)

Zero submodule Smallest element of D(M) Submodule M Greatest element of D(M) $\bigcap_{i\in I}M_i$ Greatest lower bound inf$_{i\in I}M_i$ $\sum_{i\in I}M_i$ Least upper bound sup$_{i\in I}M_i$ Supplementary submodules inf(M$',M'') = 0$, sup(M$',M'') = M$ Simple submodule of M Minimal element of D(M) $\{0\}$ Maximal submodule of M Maximal element of D(M) $\{M\}$ Socle $\mathscr{S}(M)$ of M Least upper bound in D(M) of the set of

minimal elements of D(M) $\{0\}$ $*$Radical $\mathfrak{R}(M)$ of M Greatest lower bound in D(M) of the set

$$
*
$$

(VIII, p. 151) of maximal elements of D(M) $\{M\}$

Table I.

Properties of the module M Properties of D(M)

M is Noetherian. The ordered set D(M) is Noetherian (Set

Theory, III, §6, No. 5, p. 190). M is Artinian. The set D(M), ordered by $\supset$, is

Noetherian. M is indecomposable. We have M $\not= 0$, and there are no

two nonzero elements $M'$ and $M''$ of

D(M) satisfying inf(M$',M'') = 0$,

sup(M$',M'') = M$. M is finitely generated. For every family $(M_i)_{i\in I}$ in D(M) with

upper bound M, there exists a finite

subset J of I such that M = sup$_{j\in I}M_j$. M is simple. Card(D(M)) = 2. M is semisimple. M is the least upper bound, in D(M),

of the set of minimal elements of

D(M) $\{0\}$.

Table II.

c) The B-module V is the direct sum of the family $(V_i)_{i\in I}$ of submodules if and only if M is the direct sum of the family $(\varphi (V_i))_{i\in I}$.

Let $V'$ and $V''$ be submodules of V such that $V'$ is contained in $V''$; set $M'=\varphi (V')$ and $M''=\varphi (V'')$, so that $M''$ contains $M'$. Denote by $[V',V'']$ the interval in D(V) consisting of the submodules W of V such that we have $V'\subset W\subset V''$, and define the interval $[M',M'']$ in D(M) likewise. The mapping $W\mapsto W/V'$ is an isomorphism of ordered sets from $[V',V'']$ to $D(V''/V')$; we define an isomorphism of ordered sets from $[M',M'']$ to $D(M''/M')$ likewise. Since $\varphi$ sends the interval $[V',V'']$ to $[M',M'']$, it defines an isomorphism $\varphi$ of ordered sets from $D(V''/V')$ to $D(M''/M')$. We deduce the following proposition from this and Tables I and II.

#### Proposition 8 {#alg-viii-s6-prop-8 .statement tag=007F}

a) Let $V'$ and $V''$ be submodules of V such that $V''$ contains $V'$. The B-module $V''/V'$ is simple if and only if the A-module $\varphi (V'')/\varphi (V')$ is simple.

b) If $V'$ is a simple submodule, maximal submodule, or direct factor of V, then $\varphi (V')$ is, respectively, a simple submodule, maximal submodule, or direct factor of M.

c) The isomorphism $\varphi$ transforms the socle $\mathscr{S}(V)$ of V into the socle $\mathscr{S}(M)$ of $M*$and the radical (VIII, p. 151, Definition 1$)\mathfrak{R}(V)$ of V into the radical $\mathfrak{R}(M)$ of M$.*$

d) Let $(V_i)_{0\leqslant i\leqslant n}$ be a finite sequence of submodules of V. It is a Jordan– Hölder series of V if and only if $(\varphi (V_i)_{0\leqslant i\leqslant n})$ is a Jordan–Hölder series of M.

#### Lemma 2 {#alg-viii-s6-lem-2 .statement tag=007G}

Let H and $H'$ be submodules of V such that $H\cap H'= 0$. The B-modules H and $H'$ are isomorphic if and only if the A-modules $\varphi (H)$ and $\varphi (H')$ are isomorphic.

We identify $H+H'$ with the product $H\times H'$. The graph of an isomorphism from H to $H'$ is a submodule $H''$ of V satisfying

$$
H\cap H''= H'\cap H''= 0,H + H'= H + H''= H'+ H'' \tag{17}
$$

conversely, every submodule that has these properties is the graph of an isomorphism from H to $H'$. By Proposition 7, the relation $H\cap H'= 0$ is equivalent to $\varphi (H)\cap \varphi (H') = 0$, and relations (17) are equivalent to the relations

$$
\varphi (H)\cap \varphi (H'') =\varphi (H')\cap \varphi (H'') = 0
$$

$$
\varphi (H) +\varphi (H') =\varphi (H) +\varphi (H'') =\varphi (H') +\varphi (H'')
$$

the lemma follows.

#### Proposition 9 {#alg-viii-s6-prop-9 .statement tag=00R6}

Let S be a simple submodule of V and T the simple submodule $\varphi (S)$ of M. If $V_S$ denotes the isotypical component of V of type S and $M_T$ the isotypical component of M of type T, then we have $\varphi (V_S) = M_T$.

Every simple submodule $S'$ of V distinct from S satisfies $S'\cap S = 0$. It is therefore isomorphic to S if and only if $\varphi (S')$ is isomorphic to T (Lemma 2). Now, $V_S$ is the sum of the simple submodules of V isomorphic to S, and $M_T$ is the sum of the simple submodules of M isomorphic to T. Proposition 9 therefore follows immediately from Propositions 7 and 8.

#### Proposition 10 {#alg-viii-s6-prop-10 .statement tag=007H}

a) The B-module V is Artinian (resp. Noetherian, indecomposable, simple, finitely generated) if and only if M is.

b) The B-module V has finite length if and only if the A-module M has finite length, and we then have long$_B(V) =$ long$_A(M)$.

c) The B-module V is semisimple (resp. isotypical) if and only if the A-module M is semisimple (resp. isotypical). If this is the case, then we have long$_B(V) =$ long$_A(M)$.

Assertion a) follows from the second property listed in Table II.

Assertion b) follows from Proposition 8, d).

The module V is semisimple if and only if it is equal to its socle $\mathscr{S}(V)$; it is isotypical if and only if there exists a simple submodule S of V such that $V = V_S$. Assertion c) therefore follows from Propositions 7, c), 8, c), and 9 (VIII, p. 106 and 109).

### 6. Other Properties Preserved by the Morita Correspondence

Let A and B be Morita equivalent $k$-algebras and P an invertible $(A,B)_k$-bimodule.

#### Proposition 11 {#alg-viii-s6-prop-11 .statement tag=007I}

Let

$$
(\mathscr{E})V'-\rightarrow^fV-\rightarrow^gV''
$$

be a diagram of B-modules and B-linear mappings, and let

$$
(P\otimes \mathscr{E})P\otimes_BV'\longrightarrow^{1_P\otimes f}P\otimes_BV\longrightarrow^{1_P\otimes g}P\otimes_BV''
$$

be the corresponding diagram of A-modules. Then $(\mathscr{E})$ is an exact sequence if and only if $(P\otimes \mathscr{E})$ is an exact sequence.

Suppose that the sequence $(\mathscr{E})$ is exact. Since the right B-module P is projective, the sequence $(P\otimes \mathscr{E})$ is exact (II, §3, No. 6, p. 251, Proposition 5 and II, §3, No. 7, p. 257, Corollary 6).

Conversely, suppose that the sequence $(P\otimes \mathscr{E})$ is exact. Let Q be a $(B,A)_k$-bimodule, inverse to P, and $\theta : Q\otimes_AP\rightarrow_sB_d$ an isomorphism. Consider the commutative diagram

$Q\otimes_AP\otimes_BV_'^{1_Q\otimes 1_P\otimes f}/$/ $Q\otimes_AP\otimes_BV^{1_Q\otimes 1_P\otimes g}/$/ $Q\otimes_AP\otimes_BV_{''}$

$\theta \otimes 1_{V'}\theta \otimes 1_V\theta \otimes 1_{V''}$

$V_'f$ // V $g$ // $V_{''}$.

Since Q is a projective A-module and the sequence $(P\otimes \mathscr{E})$ is exact, the first line of this diagram is an exact sequence. Since the vertical arrows are isomorphisms, the second line is also exact.

#### Corollary {#alg-viii-s6-n6-cor-1 .statement tag=007J}

Let $f: V\rightarrow W$ be a B-linear mapping. Then $f$ is injective (resp. surjective) if and only if $1_P\otimes f$ is.

#### Proposition 12 {#alg-viii-s6-prop-12 .statement tag=007K}

Let V be a left B-module. The B-module V is projective (resp. generating, faithful, $*$injective, finitely presented ) if and only if the

$$
*
$$

A-module $P\otimes_BV$ is.

a) Suppose that V is projective. There exists a set I such that V is isomorphic to a direct factor submodule of $B^{(I)}_s$ . The A-module $P\otimes_BV$ is then isomorphic to a direct factor submodule of $P^{(I)}$; since P is a projective A-module, the same holds for $P\otimes_BV$.

b) Suppose that the B-module V is generating. Let M be an A-module. There exists a B-module W such that M is isomorphic to $P\otimes_BW$. By Theorem 1 of VIII, p. 80, there exist a set I and a surjection $\varphi : V^{(I)}\rightarrow W$. By the corollary, the mapping $1_P\otimes \varphi$ from $P\otimes (V^{(I})$ to $P\otimes_AW$ is surjective, which gives a surjection $(P\otimes V)^{(I)}\rightarrow M$. By Theorem 1 of VIII, p. 80, $P\otimes V$ is a generating A-module.

c) The B-module V is faithful if and only if its annihilator is reduced to 0. Assertion c) therefore follows from Example 3 of VIII, p. 105.

$*$d) Suppose that V is injective. By the remark of VIII, p. 106, the A-module $P\otimes_BV$ is isomorphic to Hom$_B(Q,V)$, where Q is a $(B,A)_k$-bimodule inverse to A. Since the A-module Q is projective, hence flat (X, §1, n$^o3$, p. 9, exemple 1), the A-module Hom$_B(Q,V)$ is injective by X, §1, n$^o8$, p. 18, proposition 11.

e) Suppose that V admits a finite presentation $L_1\rightarrow L_0\rightarrow V\rightarrow 0$ (X, §1, n$^o4$, p. 10). By taking the tensor product with P, we deduce an exact sequence of A-modules $N'_1-\rightarrow^uN'_0\rightarrow P\otimes_BV\rightarrow 0$, where $N'_1$ and $N'_0$ are projective and finitely generated (Proposition 11 and a)). Let $N''_0$ be a finitely generated A-module such that the module $N_0= N'_0\oplus N''_0$ is free and finitely generated, and let $u': N'_1\oplus N''_0\rightarrow N_0$ be the homomorphism $(u,1_{N''})$;

0

then $P\otimes_BV$ can be identified with the cokernel of $u'$. Let $N_1$ be a finitely generated free A-module and $p: N_1\rightarrow N'_1\oplus N''_0$ a surjective homomorphism; the sequence $N_1\longrightarrow^{u'\circ p}N_0\rightarrow P\otimes_BV\rightarrow 0$ is a finite presentation of the A-module $P\otimes_BV.*$

f) Suppose that the A-module $P\otimes_BV$ is projective (resp. generating, faithful, $*$injective, finitely presented ). By applying the above (interchanging

$$
*
$$

the roles of A and B and of P and Q), we see that the B-module $Q\otimes_AP\otimes_BV$ also has this property. The same is therefore true for the B-module V, which is isomorphic to it.

#### Corollary {#alg-viii-s6-n6-cor-2 .statement tag=007L}

The ring A is left Artinian (resp. left Noetherian) if and only if the ring B is.

Because of the isomorphism between the ordered set of left ideals of B and the set of A-submodules of P, the ring B is left Artinian (resp. left Noetherian) if and only if the A-module P is Artinian (resp. Noetherian). However, by Theorem 1 of VIII, p. 101, the A-module P is generating and finitely generated; in particular, $A_s$ is isomorphic to a direct factor of $P^n$ for an integer $n\geqslant 1$. Consequently, P is Artinian (resp. Noetherian) if and only if A is left Artinian (resp. left Noetherian).

### 7. Morita Equivalence of Algebras

#### Proposition 13 {#alg-viii-s6-prop-13 .statement tag=007M}

a) If two $k$-algebras are Morita equivalent, then their centers are isomorphic $k$-algebras.

b) Two commutative $k$-algebras are Morita equivalent if and only if they are isomorphic.

c) Two $k$-algebras that are fields are Morita equivalent if and only if they are isomorphic.

d) For $i= 1,2$, let $A_i$ and $B_i$ be Morita equivalent $k$-algebras and $P_i$ an invertible $(A_i,B_i)_k$-bimodule. Set $A = A_1\otimes_kA_2,B = B_1\otimes_kB_2$, and $P = P_1\otimes_kP_2$. The $k$-algebras A and B are Morita equivalent, and P is an invertible $(A,B)_k$-bimodule.

e) If A and B are Morita equivalent $k$-algebras and $k'$ is a commutative $k$-algebra, then the $k'$-algebras $A_{(k')}$ and $B_{(k')}$ are Morita equivalent.

Assertion a) follows from Corollary 1 of VIII, p. 102, and implies b).

Let K and L be $k$-algebras that are fields, and let P be an invertible $(K,L)_k$-bimodule. The right L-vector space P is a simple module (VIII, p. 104), hence of dimension 1, so the $k$-algebras End$_L(P)$ and L are isomorphic. By VIII, p. 101, Theorem 1, the mapping $a\mapsto a_P$ from K to End$_L(P)$ is an isomorphism. Therefore, the fields K and L are isomorphic over $k$; assertion c) follows.

Under the assumptions of d), let $Q_i(i= 1,2)$ be a $(B_i,A_i)_k$-bimodule inverse to $P_i$. Denote the $(B,A)_k$-bimodule $Q_1\otimes_kQ_2$ by Q. Consider the canonical $k$-linear isomorphism $(P_1\otimes_kP_2)\otimes_k(Q_1\otimes_kQ_2)\rightarrow (P_1\otimes_kQ_1)\otimes_k$ $(P_2\otimes_kQ_2)$; when passing to the quotient, it defines a morphism

$$
(P_1\otimes_kP_2)\otimes_B(Q_1\otimes_kQ_2)\rightarrow (P_1\otimes_{B_1}Q_1)\otimes_k(P_2\otimes_{B_2}Q_2)
$$

that is $(A$, A)-linear. Conversely, the inverse isomorphism $(P_1\otimes_kQ_1)\otimes_k(P_2\otimes_k$ $Q_2)\rightarrow (P_1\otimes_kP_2)\otimes_k(Q_1\otimes_kQ_2)$ defines an $(A$, A)-linear morphism $(P_1\otimes_{B_1}$ $Q_1)\otimes_k(P_2\otimes_{B_2}Q_2)\rightarrow (P_1\otimes_kP_2)\otimes_B(Q_1\otimes_kQ_2)$. These two morphisms are each other’s inverses and are thus isomorphisms. Since the $(A_i,A_i$)-bimodule $P_i\otimes_{B_i}Q_i$ is isomorphic to $A_i$, we obtain an $(A$, A)-linear isomorphism $P\otimes_B$ $Q\rightarrow A$. We likewise obtain a $(B$, B)-linear isomorphism $Q\otimes_AP\rightarrow B$, which completes the proof of d).

Under the assumptions of e), let P be an invertible $(A,B)_k$-bimodule; then $P_{(k')}$ is an invertible $(A_{(k')},B_{(k')})_{k'}$-bimodule.

Let A be a $k$-algebra, and let $e$ be an idempotent in A. The set $eAe$, endowed with the addition, multiplication, and action of $k$ induced by those of A, is a $k$-algebra with unit element $e$.

#### Proposition 14 {#alg-viii-s6-prop-14 .statement tag=007N}

Let A and B be $k$-algebras. Then A and B are Morita equivalent if and only if there exist an integer $n\geqslant 1$ and a square matrix $e= (e_{ij})$ in $\mathbf{M}_n(B)$ satisfying the following conditions:

(i) We have $e^2=e$.

(ii) The two-sided ideal of B generated by the elements $e_{ij}$ is equal to B.

(iii) The $k$-algebra A is isomorphic to $e\mathbf{M}_n(B)e$. If conditions (i) and (ii) are satisfied, then the $(e\mathbf{M}_n(B)e,B)_k$-bimodule $eB^n_d$ is invertible.

In view of Theorem 1 (VIII, p. 101), the $k$-algebra A is Morita equivalent to B if and only if it is isomorphic to the endomorphism algebra of a projective, finitely generated, and generating right B-module. The proposition therefore follows from Lemmas 3 and 4 below.

#### Lemma 3 {#alg-viii-s6-lem-3 .statement tag=007O}

A right B-module P is projective, finitely generated, and generating if and only if there exist an integer $n\geqslant 0$ and an idempotent $e= (e_{ij})$ in $\mathbf{M}_n(B)$ with the following properties:

(i) The B-module P is isomorphic to $eB^n_d$.

(ii) The two-sided ideal of B generated by the elements $e_{ij}$ is equal to B.

Let P be a right B-module. Then P is projective and finitely generated if and only if it is isomorphic to a direct factor submodule of a B-module of the form $B^n_d$, where $n$ is an integer $\geqslant 0$ (II, §2, No. 2, p. 232, Corollary 1). If we identify the $k$-algebras $\mathbf{M}_n(B)$ and End(B$^n_d)$, then this means that there exists an idempotent $e$ in $\mathbf{M}_n(B)$ such that P is isomorphic to $eB^n_d$.

The B-module P is generating if and only if its trace ideal $\tau (P)$ is equal to B, that is, $\tau (eB^n_d) = B$ (VIII, p. 80, Theorem 1). Let $x_1, . . . , x_n$ be the elements of $B^n_d$ corresponding to the columns of the matrix $e$, and let $x^*_i$ (for $1\leqslant i\leqslant n)$ be the linear form $(b_1, . . . , b_n)\mapsto b_i$ on $eB^n_d$. The family $(x_1, . . . , x_n)$ generates the B-module $eB^n_d$, and the family $(x^*_1, . . . , x^*_n)$ generates its dual. Now, we have $\langle x^*_i, x_j\rangle =e_{ij}$, so $\tau (eB^n_d)$ is the two-sided ideal of B generated by the $e_{ij}$. This proves Lemma 3.

#### Lemma 4 {#alg-viii-s6-lem-4 .statement tag=007P}

Let V be a B-module and E the endomorphism $k$-algebra of V. Let $e$ be a projector of V and P the image of $e$. The mapping that sends $v\in eEe$ to the endomorphism $x\mapsto v(x)$ of the B-module P is an isomorphism of $k$-algebras from $eEe$ to End$_B(P)$.

Denote the mapping described in the statement by $\varphi :eEe\rightarrow$ End$_B(P)$; it is a homomorphism of $k$-algebras. Let $u\in$ End$_B(P)$. Denote by $v$ the endomorphism of V defined by $v(x) =u(e(x))$ for $x\in V$. We have $(eve)(x) =$ $u(x)$ for $x\in P$, that is, $\varphi (eve) =u$. Consequently, $\varphi$ is surjective. Let $w$ be an element of the kernel of $\varphi$; the restrictions of $w$ to the kernel and to the image of $e$ are zero, so $w$ is zero, which proves that $\varphi$ is injective.

#### Example 1 {#alg-viii-s6-n7-exa-1 .statement tag=007Q}

Let A be a $k$-algebra and $e$ an idempotent in A such that $AeA = A$. The $k$-algebra $eAe$ can be identified with the endomorphism $k$-algebra of the submodule $eA_d$ of $A_d$ (Lemma 4). Since $AeA = A$, it follows from Proposition 14 that $eA_d$ is an invertible $(eAe,A)_k$-bimodule, so that the $k$-algebras $eAe$ and A are Morita equivalent. Moreover, Morita’s theorem (VIII, p. 103) implies the following results:

a) Let M and N be left A-modules. Every $eAe$-linear mapping from $eM$ to $eN$ extends uniquely to an A-linear mapping from M to N.

b) Every left module over the $k$-algebra $eAe$ is isomorphic to a module of the form $eM$, where M is a left A-module.

#### Example 2 {#alg-viii-s6-n7-exa-2 .statement tag=007R}

Let A be a $k$-algebra and $n\geqslant 1$ an integer. We identify the matrix algebra $\mathbf{M}_n(A)$ with the endomorphism algebra of the right A-module $A^n_d$. We have seen that A and $\mathbf{M}_n(A)$ are Morita equivalent. For every left A-module M, identify $A^n_d\otimes_AM$ with $M^n$. The algebra $\mathbf{M}_n(A)$ then has a left action on $M^n$, and we have

$$
(a\cdot m)_i=\sum_{j=1}^na_{ij}m_j
$$

for $a= (a_{ij})$ in $\mathbf{M}_n(A)$ and $m= (m_i)$ in $M^n$. Morita’s theorem implies the following results:

a) Every left module over the algebra $\mathbf{M}_n(A)$ is isomorphic to a module of the form $M^n$, where M is a left A-module.

b) Let M be a left A-module. The mapping $N\mapsto N^n$ is a bijection from the set of A-submodules of M to the set of $\mathbf{M}_n$(A)-submodules of $M^n$.

c) Let M and N be left A-modules. For an A-linear mapping $g: M\rightarrow N$, let $g_n$ be the mapping $(m_i)\mapsto (g(m_i))$ from $M^n$ to $N^n$. Then the mapping $g\mapsto g_n$ is a bijection from Hom$_A(M,N)$ to Hom$_{\mathbf{M}_n(A)}(M^n,N^n)$.

d) Let M be a left A-module. The module $M^n$ over the ring $\mathbf{M}_n(A)$ is indecomposable (resp. semisimple, simple, Artinian, Noetherian, finitely generated) if and only if the A-module M is.

#### Example 3 {#alg-viii-s6-n7-exa-3 .statement tag=007S}

Let A be a principal ideal domain and L a nonzero, finitely generated, free A-module. Let B be the endomorphism ring of L; then L is an invertible $(A,B)_{\mathbf{Z}}$-bimodule, and the rings A and B are Morita equivalent. By Morita’s theorem, Proposition 10, a) (VIII, p. 109), and the structure theorem for finitely generated A-modules (VII, §4, No. 4, p. 19, Theorem 2), every finitely generated B-module is isomorphic to $\oplus^m_{i=1}(L/\mathfrak{a}_iL)$, where $m$ is a natural number and the $\mathfrak{a}_i$ are ideals of A satisfying $\mathfrak{a}_1\subset \mathfrak{a}_2\subset  \cdots  \subset \mathfrak{a}_m$ and $\mathfrak{a}_m\not= A$; the integer $m$ and the ideals $\mathfrak{a}_i$ are uniquely determined. By Proposition 6 of VIII, p. 105, every two-sided ideal of B is of the form $dB$, where $d$ is an element of A.

### Exercises {#alg-viii-s6-exercises}

See the [exercises for § 6](exercises/s6/).
