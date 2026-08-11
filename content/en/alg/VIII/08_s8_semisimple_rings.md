---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 8
section_title: Semisimple Rings
lang: en
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.135-A VIII.150
pdf_pages: 0152-0167
extraction: native
subsections:
    - "no": 1
      title: Semisimple Rings
      page: 135
      pdf_page: 152
    - "no": 2
      title: Modules over a Semisimple Ring
      page: 138
      pdf_page: 155
    - "no": 3
      title: Factors of a Semisimple Ring
      page: 141
      pdf_page: 158
    - "no": 4
      title: Idempotents and Semisimple Rings
      page: 145
      pdf_page: 162
statements: 30
exercises: 6
content_sha256: 725b6017435a01db686f5e73f7d66e05ef0ab6eadd6ee9d5337a2b7642692bd6
---

## § 8. SEMISIMPLE RINGS

### 1. Semisimple Rings

#### Theorem 1 {#alg-viii-s8-thm-1 .statement tag=00S4}

Let A be a ring. The following properties are equivalent:

(i) The A-module $A_s$ is semisimple.

(ii) For every left ideal $\mathfrak{a}$ of A, there exists a left ideal $\mathfrak{b}$ of A such that $A_s$ is the direct sum of $\mathfrak{a}$ and $\mathfrak{b}$.

(iii) The ring A is left Artinian, and the $(A,A)$-bimodule $_sA_d$ is semisimple.

(iv) The ring A is isomorphic to the product of a finite family of simple rings.

(v) There exist an integer $s\geqslant$ 0, fields $D_1, . . . ,D_s$, and integers $r_1\geqslant 1, . . .,r_s\geqslant 1$ such that the ring A is isomorphic to the product of the matrix rings $\mathbf{M}_{r_i}(D_i)$.

(vi) The ring A is left Artinian, and there exists a faithful and semisimple left A-module.

The equivalence of (i) and (ii) follows from Corollary 2 of VIII, p. 56, and that of (iv) and (v) follows from Theorem 1 of VIII, p. 120.

The A-module $A_s$ is finitely generated. If it is semisimple, then it is left Artinian (VIII, p. 71, Proposition 10). Since the A-module $A_s$ is faithful, this proves that (i) implies (vi). Conversely, suppose that property (vi) holds; let M be a faithful semisimple A-module. There exists an integer $m\geqslant 1$ such that $A_s$ is isomorphic to a submodule of $M^m$ (VIII, p. 50, Proposition 5, a)); since M is semisimple, the same holds for $A_s$. We have therefore proved the equivalence of (i) and (vi).

Let us prove that (i) implies (iii). Suppose that the ring A has property (i); we have already observed that A is then left Artinian. Now, the endomorphisms of the left A-module $A_s$ are the right multiplications by the elements of A. That the $(A$, A)-bimodule $_sA_d$ is semisimple then follows from Proposition 6 of VIII, p. 86.

Let us show that (iii) implies (iv). Suppose that the $(A$, A)-bimodule $_sA_d$ is semisimple. It is finitely generated, so there exists a finite family $(\mathfrak{a}_i)_{i\in I}$ of simple $(A$, A)-sub-bimodules with direct sum $_sA_d$. In other words, the $\mathfrak{a}_i$ are nonzero two-sided ideals of A, the additive group of A is the direct sum of the $\mathfrak{a}_i$, and for every $i\in I$, every two-sided ideal of A contained in $\mathfrak{a}_i$ is equal to 0 or $\mathfrak{a}_i$. Set $\mathfrak{b}_i=\sum_{j\not=i}\mathfrak{a}_j$ for every $i\in I$; this is a two-sided ideal of A. The mapping $a\mapsto (a+\mathfrak{b}_i)_{i\in I}$ is an isomorphism from the ring A to the product of the rings $A/\mathfrak{b}_i$. The $(A$, A)-bimodules $\mathfrak{a}_i$ and $A/\mathfrak{b}_i$ are isomorphic, so every two-sided ideal of $A/\mathfrak{b}_i$ is equal to 0 or $A/\mathfrak{b}_i$. If the ring A is left Artinian, then the same holds for the rings $A/\mathfrak{b}_i$, which are therefore simple (VIII, p. 120, Definition 1).

Finally, let us prove that (iv) implies (i). Suppose that A is the product of a finite family $(A_i)_{i\in I}$ of simple rings. Denote by $\pi_i$ the projection with index $i$ from A to $A_i$ and by $M_i$ the A-module with underlying additive group $A_i$ and law of action $(a, x)\mapsto \pi_i(a)x$. Since the ring $A_i$ is simple, the $A_i$-module $(A_i)_s$ is semisimple, so the A-module $M_i$ is semisimple. Since the A-module $A_s$ is nothing but the product $\prod_{i\in I}M_i$, it is semisimple.

#### Definition 1 {#alg-viii-s8-def-1 .statement tag=0093}

We say that a ring A is semisimple if it has the equivalent properties (i) through (vi) of Theorem 1. An algebra A over a commutative ring $k$ is a semisimple algebra if the ring underlying A is semisimple.

#### Proposition 1 {#alg-viii-s8-prop-1 .statement tag=0094}

Let A be a semisimple ring. There exists a finite family $(\mathfrak{m}_i)_{i\in I}$ of minimal left ideals of A such that $A_s=\oplus_{i\in I}\mathfrak{m}_i$. If $(\mathfrak{m}_i)_{i\in I}$ is such a family, then every simple A-module is isomorphic to one of the $\mathfrak{m}_i$. The set of classes of simple A-modules is finite.

The first assertion follows from the fact that the A-module $A_s$ is semisimple and finitely generated. Every simple module is isomorphic to a quotient of $A_s$ (VIII, p. 46, Proposition 1). The second assertion then follows from Corollary 3 of VIII, p. 56, and the third assertion is an immediate consequence of the second.

#### Example {#alg-viii-s8-n1-exa-1 .statement tag=0095}

Let G be a finite group and K a commutative field. $*$We will see further on (VIII, p. 401, Corollary 1) that the algebra K[G] of the group G over the field K is a semisimple ring if and only if the characteristic exponent of K is prime to the order of $G.*$

#### Remark 1 {#alg-viii-s8-n1-rem-1 .statement tag=0096}

Let K be a commutative field, and let A be a semisimple algebra over K. Then there exist K-algebras $D_1, . . . ,D_s$ that are fields and integers $r_1\geqslant 1, . . . , r_s\geqslant 1$ such that the K-algebra A is isomorphic to the product $\prod^s_{i=1}\mathbf{M}_{r_i}(D_i)$.

#### Remark 2 {#alg-viii-s8-n1-rem-2 .statement tag=0097}

Let K be an algebraically closed field, and let A be an algebra of finite degree over K. By Remark 4 of VIII, p. 122, the algebra A is semisimple if and only if there exist integers $n_1\geqslant 1, . . . , n_r\geqslant 1$ such that A is isomorphic to the algebra $\mathbf{M}_{n_1}(K)\times  \cdots  \times \mathbf{M}_{n_r}(K)$.

#### Proposition 2 {#alg-viii-s8-prop-2 .statement tag=0098}

a) The center of a semisimple ring is semisimple.

b) The opposite ring of a semisimple ring is semisimple.

c) The quotient of a semisimple ring by a two-sided ideal is a semisimple ring.

d) The product of a finite family of semisimple rings is a semisimple ring.

Let A be a semisimple ring. It is isomorphic to the product of a finite family $(A_i)_{i\in I}$ of simple rings. The center of A is isomorphic to the product of the centers of the $A_i$, and $A^o$ is isomorphic to the product ring of the $A^o_i$. Assertions a) and b) therefore follow from Corollary 1 of VIII, p. 121.

Let $\mathfrak{a}$ be a two-sided ideal of A. The A-module $A_s/\mathfrak{a}$, quotient of the semisimple A-module $A_s$, is semisimple. The $(A/\mathfrak{a}$)-module $A_s/\mathfrak{a}$ is therefore semisimple; assertion c) follows.

A ring is semisimple if and only if it is isomorphic to the product of a finite family of simple rings; assertion d) follows.

#### Proposition 3 {#alg-viii-s8-prop-3 .statement tag=0099}

Let A be a commutative ring. The following properties are equivalent:

(i) The ring A is semisimple.

(ii) The ring A is Artinian and reduced (V, §6, No. 7, p. 34).

(iii) The ring A is isomorphic to the product of a finite family of commutative fields.

Commutative simple rings are commutative fields (VIII, p. 120, Remark 1). So (i) is equivalent to (iii).

It is clear that (iii) implies (ii). Conversely, suppose that the ring A is Artinian and reduced. The intersection of the set of prime ideals of A consists of the nilpotent elements of A (V, §15, No. 1, p. 118, Proposition 2), hence is reduced to 0 because A is reduced. By VIII, p. 2, there then exist distinct prime ideals $\mathfrak{p}_1, . . . ,\mathfrak{p}_r$ of A such that we have $\mathfrak{p}_1\cap  \cdots  \cap \mathfrak{p}_r= 0$. By the corollary of VIII, p. 8, each of the prime ideals $\mathfrak{p}_i$ of the Artinian ring A is maximal; we therefore have $\mathfrak{p}_i+\mathfrak{p}_j= A$ whenever $i$ and $j$ are distinct. By Proposition 9 of I, §8, No. 11, p. 110, the canonical homomorphism from A to the ring $\prod^r_{i=1}(A/\mathfrak{p}_i)$ is an isomorphism. The ring $A/\mathfrak{p}_i$ is a field for every $i$, and (ii) therefore implies (iii).

A commutative algebra of finite degree over a field is an Artinian commutative ring. Proposition 3 therefore generalizes Proposition 5 of V, §6, No. 7, p. 34.

### 2. Modules over a Semisimple Ring

#### Proposition 4 {#alg-viii-s8-prop-4 .statement tag=009A}

Let A be a ring. The following properties are equivalent:

(i) The ring A is semisimple.

(ii) Every A-module is semisimple.

(iii) There exists a generating and semisimple A-module.

(iv) There exists a faithful and semisimple A-module with finitely generated countermodule.

(v) Every A-module is projective.

(vi) Every monogenous A-module is projective.

$*$For other characterizations of semisimple rings, see Proposition 6 of X, §8, n$^o4$, p. $140.*$

Let us first prove that (i) implies (ii) and (v). Suppose that the ring A is semisimple, and consider a left A-module M. By assumption, the A-module $A_s$ is semisimple, so every free A-module is semisimple. By Proposition 20 of II, §1, No. 11, p. 218, there exist a free A-module L and a surjective A-linear mapping $u$ from L to M. Let N be the kernel of $u$. Since the A-module L is semisimple, there exists a semisimple submodule $N'$ supplementary to N in L (VIII, p. 56, Theorem 1). The A-module $N'$ is projective, and $u$ induces an isomorphism from $N'$ to M. Consequently, M is semisimple and projective.

(ii) $\Rightarrow$ (iii): If every A-module is semisimple, then the A-module $A_s$ is semisimple; it is moreover generating.

(iii) $\Rightarrow$ (iv): If M is a generating A-module, then it is faithful (VIII, p. 80, Corollary of Theorem 1), and its countermodule is finitely generated (VIII, p. 99, Corollary 1).

(iv) $\Rightarrow$ (i): Let M be a faithful and semisimple A-module with finitely generated countermodule. By Lemma 4 of VIII, p. 8, there exists a natural number $m$ such that $A_s$ is isomorphic to a submodule of $M^m$. The A-module $M^m$ is semisimple, and therefore so is $A_s$.

The implication (v) $\Rightarrow$ (vi) is immediate.

(vi) $\Rightarrow$ (i): Suppose that every monogenous A-module is projective. Let $\mathfrak{a}$ be a left ideal of A. Since the A-module $A_s/\mathfrak{a}$ is projective, there exists a left ideal $\mathfrak{b}$ of A such that $A_s$ is the direct sum of $\mathfrak{a}$ and $\mathfrak{b}$ (II, §2, No. 2, p. 231, Proposition 4). Consequently, the ring A is semisimple (VIII, p. 135, Theorem 1).

#### Lemma 1 {#alg-viii-s8-lem-1 .statement tag=009B}

Let A be a left Artinian ring, and let M be a simple A-module. Then the ring $A_M$ is simple.

Since the ring A is left Artinian, the same holds for the ring $A_M$, by Proposition 5 of VIII, p. 7. Now, M is a faithful and simple $A_M$-module, so the ring $A_M$ is simple (VIII, p. 119, Proposition 1).

#### Proposition 5 {#alg-viii-s8-prop-5 .statement tag=009C}

Suppose that the ring A is semisimple. Let M be a left A-module. The countermodule of M is finitely generated, and we have $A_M= A''_M$.

First consider the case when M is a simple A-module. By Lemma 1, the ring $A_M$ is simple. Proposition 5 then follows from Lemma 1 of VIII, p. 120.

Now consider the general case. The set $\mathscr{S}$ of classes of simple A-modules is finite (VIII, p. 136, Proposition 1). For every $\lambda \in \mathscr{S}$, choose an A-module $S_{\lambda}$ of class $\lambda$, and denote the opposite field of the commutant of $S_{\lambda}$ by $D_{\lambda}$. By Lemma 1 applied to the simple ring $A_{S_{\lambda}}, S_{\lambda}$ is a finite-dimensional vector space over the field $D_{\lambda}$; denote its dimension by $m(\lambda )$. Let B be the opposite ring of the endomorphism ring of M. We have seen in VIII, p. 84 that there exist $(D_{\lambda}$, B)-bimodules $V_{\lambda}$ that are simple as B-modules and an isomorphism of $(A$, B)-bimodules from M to $\oplus_{\lambda\in\mathscr{S}}S_{\lambda}\otimes_{D_{\lambda}}V_{\lambda}$. As a B-module, M is isomorphic to $\oplus_{\lambda\in\mathscr{S}}V^m_{\lambda}^{(\lambda)}$. Since $\mathscr{S}$ and the $m(\lambda )$ are finite, M is a finitely generated B-module.

The A-module M is semisimple, and its countermodule is finitely generated. We therefore have $A_M= A''_M$ by Proposition 4 of VIII, p. 83.

#### Proposition 6 {#alg-viii-s8-prop-6 .statement tag=009D}

Let M be a finitely generated semisimple A-module. Denote its support (VIII, p. 66) by $\mathscr{S}_M$ and its endomorphism ring by B. For every $\lambda \in \mathscr{S}_M$, choose a simple A-module $S_{\lambda}$ of class $\lambda$, and denote the left B-module Hom$_A(S_{\lambda},M)$ by $V_{\lambda}$.

a) The ring B is semisimple.

b) The mapping $\lambda \mapsto$ cl(V$_{\lambda})$ is a bijection from the support $\mathscr{S}_M$ of M to the set of classes of simple B-modules.

c) For every $\lambda \in \mathscr{S}_M$, the isotypical component of type $\lambda$ of the A-module M is equal to the isotypical component of type $V_{\lambda}$ of the B-module M.

Viewed as a B-module, M is semisimple (VIII, p. 85, Proposition 5) and faithful. Its countermodule is finitely generated because we have $A_M\subset$ End$_B(M)$. Hence, the ring B is semisimple (Proposition 4). If $(x_1, . . . , x_r)$ is a generating sequence of the A-module M, then the mapping $b\mapsto (bx_1, . . . , bx_r)$ from $B_s$ to $M^r$ is B-linear and injective. Every simple B-module is isomorphic to a submodule of $B_s$ (VIII, p. 136, Proposition 1), hence to a B-submodule of M. The proposition then follows immediately from Proposition 5 of VIII, p. 85.

#### Proposition 7 {#alg-viii-s8-prop-7 .statement tag=009E}

Let A be a semisimple ring.

a) Every finitely generated A-module is reflexive (II, §2, No. 7, p. 239).

b) For every simple left A-module S, the right A-module $S^*$ dual to S is simple, and the mapping $\lambda \mapsto$ cl($\lambda^*)$ defines a bijection from the set of classes of simple A-modules to the set of classes of simple right A-modules.

c) Let M be a finitely generated left A-module. The right A-module $M^*$ dual to M is finitely generated and has the same length as M. Moreover, we have $[M : S] = [M^*: S^*]$ for every simple A-module S.

Let M be a finitely generated A-module.

By Proposition 4 of VIII, p. 138, the A-module M is finitely generated and projective; it is therefore reflexive by Corollary 4 of II, §2, No. 7, p. 240. In particular, every simple A-module is reflexive. It also follows that two finitely generated left modules are isomorphic if and only if their duals are.

Let S be a simple left A-module. Let $(T_i)_{i\in I}$ be a family of simple right A-modules with direct sum the dual $S^*$ of S. Since S is reflexive, it is isomorphic to $(S^*)^*$ and therefore to $\prod_{i\in I}T^*_i$. Each of the modules $T_i$ is reflexive; in particular, we have $T^*_i\not= 0$ for every $i\in I$. Since the simple module S is isomorphic to $\prod_{i\in I}T^*_i$, the set I has a single element, so $S^*$ is simple.

Since M is semisimple and finitely generated, it is the direct sum of simple submodules $S_1, . . . ,S_r$. Then $M^*$ is isomorphic to the direct sum of the family $S^*_1, . . . ,S^*_r$, and we have just seen that the modules $S^*_i$ are simple. Assertion c) follows immediately.

### 3. Factors of a Semisimple Ring

In this subsection, we consider a semisimple ring A.

We denote the set of classes of simple left A-modules by $\mathscr{S}$ (VIII, p. 51); it is finite (VIII, p. 136, Proposition 1). For every $\lambda \in \mathscr{S}$, we choose a simple A-module $S_{\lambda}$ of class $\lambda$. We denote its annihilator by $\mathfrak{b}_{\lambda}$ and the opposite field of its commutant End$_A(S_{\lambda})$ by $D_{\lambda}$.

#### Proposition 8 {#alg-viii-s8-prop-8 .statement tag=009F}

a) For every $\lambda \in \mathscr{S},S_{\lambda}$ is a finite-dimensional right vector space over the field $D_{\lambda}$. When passing to the quotient, the mapping $a\mapsto a_{S_{\lambda}}$ defines a ring isomorphism from $A/\mathfrak{b}_{\lambda}$ to End$_{D_{\lambda}}(S_{\lambda})$.

b) For every $\lambda \in \mathscr{S}$, the ring $A/\mathfrak{b}_{\lambda}$ is simple, and the canonical homomorphism $\psi$ from A to $\prod_{\lambda\in\mathscr{S}}A/\mathfrak{b}_{\lambda}$ is a ring isomorphism.

The ring $A/\mathfrak{b}_{\lambda}$ is isomorphic to $A_{S_{\lambda}}$. By Lemma 1 of VIII, p. 139, this ring is simple. The given mapping from $A/\mathfrak{b}_{\lambda}$ to End$_{D_{\lambda}}(S_{\lambda})$ can be identified with the mapping from $A_{S_{\lambda}}$ to $A''_{S_{\lambda}}$. By Proposition 5 of VIII, p. 139, it is an isomorphism.

The A-module $A_s$ is semisimple, faithful, and balanced. The homomorphism $\psi$ can be identified with the morphism from the bicommutant of $A_s$ to $\prod_{\lambda\in\mathscr{S}}$ End$_{D_{\lambda}}(S_{\lambda})$, which is an isomorphism (VIII, p. 86, Proposition 7, c)).

The simple ring $A/\mathfrak{b}_{\lambda}$ is called the simple factor of A of type $\lambda$.

#### Example {#alg-viii-s8-n3-exa-1 .statement tag=009G}

Let K be an algebraically closed commutative field, and let A be a semisimple algebra of finite degree over K. Let $(V_i)_{i\in I}$ be a family of simple A-modules such that every simple A-module is isomorphic to a unique $V_i$. Then I is a finite set (VIII, p. 136, Proposition 1), the vector spaces $V_i$ are finite-dimensional over the field K, the commutant of $V_i$ is equal to $K\cdot 1_{V_i}$ (VIII, p. 47, Theorem 1), and the mapping $a\mapsto (a_{V_i})_{i\in I}$ is an algebra isomorphism from A to $\prod_{i\in I}$ End$_K(V_i)$ (Proposition 8).

We have defined (VIII, p. 50) a minimal two-sided ideal as a minimal element of the set of nonzero two-sided ideals, ordered by inclusion. In other words, a minimal two-sided ideal $\mathfrak{a}$ of A is a simple $(A$, A)-sub-bimodule of $_sA_d$. Likewise, we define a maximal two-sided ideal of A as a maximal element of the set of proper two-sided ideals of A. A maximal two-sided ideal $\mathfrak{a}$ of A is simply a maximal $(A$, A)-sub-bimodule of $_sA_d$ (VIII, p. 48, Definition 2). If the ring A is simple, then the ideal 0 is a maximal two-sided ideal of A and A is a minimal two-sided ideal.

For any $\lambda \in \mathscr{S}$, we denote the isotypical component of type $\lambda$ of the A-module $A_s$ by $\mathfrak{a}_{\lambda}$. For any subset Λ of $\mathscr{S}$, we set $\mathfrak{a}_{\Lambda}=\sum_{\lambda\in\Lambda}\mathfrak{a}_{\lambda}$.

#### Proposition 9 {#alg-viii-s8-prop-9 .statement tag=009H}

a) Order the set $\mathfrak{P}(\mathscr{S})$ of subsets of $\mathscr{S}$ and the set $\mathscr{B}_A$ of two-sided ideals of A by inclusion. The mapping $\Lambda\mapsto \mathfrak{a}_{\Lambda}$ is an isomorphism of ordered sets from $\mathfrak{P}(\mathscr{S})$ to $\mathscr{B}_A$.

b) The minimal two-sided ideals of A are the ideals $\mathfrak{a}_{\lambda}$.

c) We have $\mathfrak{b}_{\lambda}=\mathfrak{a}_{\mathscr{S}\{\lambda\}}$ for every $\lambda \in \mathscr{S}$, and the ideals $\mathfrak{b}_{\lambda}$ are the maximal two-sided ideals of A.

d) For every $\lambda \in \mathscr{S}$, the canonical mapping from A to $A/\mathfrak{b}_{\lambda}$ induces an isomorphism of A-modules from $\mathfrak{a}_{\lambda}$ to $A/\mathfrak{b}_{\lambda}$.

Assertion a) follows from Proposition 8, d) of VIII, p. 87 applied to the A-module $A_s$. It follows that the minimal two-sided ideals of A are the $\mathfrak{a}_{\lambda}$ and that the maximal two-sided ideals are the ideals $\mathfrak{c}_{\lambda}=\mathfrak{a}_{\mathscr{S}\lambda}$ (for $\lambda \in \mathscr{S})$.

It remains to show the equality of $\mathfrak{b}_{\lambda}$ and $\mathfrak{c}_{\lambda}$ for every $\lambda \in \mathscr{S}$. Let $\lambda$ and $\mu$ be distinct in $\mathscr{S}$. The A-submodule $\mathfrak{a}_\mu S_{\lambda}$ of $S_{\lambda}$ is the union of the images of the linear mappings $a\mapsto ax$ from $\mathfrak{a}_\mu$ to $S_{\lambda}$ for $x\in S_{\lambda}$. Consequently, it is zero, and we have $\mathfrak{a}_\mu\subset \mathfrak{b}_{\lambda}$. We therefore have $\mathfrak{c}_{\lambda}\subset \mathfrak{b}_{\lambda}$, and finally $\mathfrak{c}_{\lambda}=\mathfrak{b}_{\lambda}$ because $\mathfrak{c}_{\lambda}$ is a maximal two-sided ideal of A and $\mathfrak{b}_{\lambda}$ is distinct from A.

#### Corollary {#alg-viii-s8-n3-cor-1 .statement tag=009I}

Let $(A_i)_{i\in I}$ be a finite family of simple rings and $f$ an isomorphism from A to $\prod_{i\in I}A_i$. For every $i\in I$, there exists a unique element $\varphi (i)$ of $\mathscr{S}$ such that the kernel of pr$_i\circ f$ is $\mathfrak{b}_{\varphi(i)}$. The mapping $\varphi$ is a bijection from I to $\mathscr{S}$; the mapping pr$_i\circ f$ induces an isomorphism $f_i$ from $A/\mathfrak{b}_{\varphi(i)}$ to $A_i$ for every $i\in I$.

Thus, $f$ is the composition of the canonical isomorphism from A to $\prod_{\lambda\in\mathscr{S}}A/\mathfrak{b}_{\lambda}$ and the isomorphism from $\prod_{\lambda\in\mathscr{S}}A/\mathfrak{b}_{\lambda}$ to $\prod_{i\in I}A_i$ deduced from the $f_i($“uniqueness of the decomposition of a semisimple ring into a product of simple rings”).

Let us prove the corollary. Let $i\in I$; denote the kernel of pr$_i\circ f$ by $\mathfrak{b}'_i$. Since the simple ring $A_i$ is isomorphic to $A/\mathfrak{b}'_i$, the two-sided ideal $\mathfrak{b}'_i$ of A is maximal. By Proposition 8, c), there consequently exists a unique element $\varphi (i)$ of $\mathscr{S}$ such that we have $\mathfrak{b}'_i=\mathfrak{b}_{\varphi(i)}$. When passing to the quotient, pr$_i\circ f$ defines an isomorphism $f_i$ from $A/\mathfrak{b}_{\varphi(i)}$ to $A_i$. Moreover, we have $\mathfrak{b}'_i+\mathfrak{b}'_j= A$ if $i\not=j$ and $\cap_{i\in I}\mathfrak{b}'_i= 0$ (cf. I, §8, No. 11, p. 110, Proposition 10). It follows from this and Proposition 8 that $\varphi$ is a bijection from I to $\mathscr{S}$.

#### Proposition 10 {#alg-viii-s8-prop-10 .statement tag=009J}

Denote the center of A by Z. For $\lambda \in \mathscr{S}$, let $Z_{\lambda}$ be the center of the field $D_{\lambda}$.

a) The mapping $z\mapsto (z_{S_{\lambda}})_{\lambda\in\mathscr{S}}$ is an isomorphism from the ring Z to the product $\prod_{\lambda\in\mathscr{S}}Z_{\lambda}$.

b) Order the set $\mathscr{I}_Z$ of ideals of Z and the set $\mathscr{B}_A$ of two-sided ideals of A by inclusion. The mapping $\mathfrak{a}\mapsto \mathfrak{a}A$ is an isomorphism of ordered sets from $\mathscr{I}_Z$ to $\mathscr{B}_A$. The inverse isomorphism sends a two-sided ideal $\mathfrak{b}$ of A to the ideal $\mathfrak{b}\cap Z$ of Z.

This proposition follows from Proposition 8 of VIII, p. 87 applied to the A-module $A_s$, whose bicommutant is A.

#### Corollary {#alg-viii-s8-n3-cor-2 .statement tag=009K}

Let B be a ring. The following properties are equivalent:

(i) The ring B is simple.

(ii) The ring B is semisimple, and its center is a field.

(iii) The ring B is semisimple, and there exists only one class of B-simple modules.

#### Proposition 11 {#alg-viii-s8-prop-11 .statement tag=009L}

Let $\lambda \in \mathscr{S}$. The isotypical component $\mathfrak{a}_{\lambda}$ of A is both the isotypical component of $A_s$ of type $S_{\lambda}$ and the isotypical component of $A_d$ of type $S^*_{\lambda}$. Moreover, we have

(1) $[A_s: S_{\lambda}] = [A_d: S^*_{\lambda}] =$ dim$_{D_{\lambda}}S_{\lambda}$

and

(2) long(A) = long(A$^o) =_{\lambda}\sum_{\in\mathscr{S}}$ dim$_{D_{\lambda}}S_{\lambda}$.

The first assertion is the specific case $M = A_s$ of Proposition 6, c) of VIII, p. 139. The equality $[A_s: S_{\lambda}] = [A_d: S^*_{\lambda}]$ follows from Proposition 7 of VIII, p. 140 because the dual of the left A-module $A_s$ is isomorphic to the right A-module $A_d$. By Propositions 8, a) and 9, c), the mapping $a\mapsto a_{S_{\lambda}}$ defines an isomorphism of left A-modules from $\mathfrak{a}_{\lambda}$ to End$_{D_{\lambda}}(S_{\lambda})$. Since $[A_s: S_{\lambda}]$ is, by definition, the length of the left A-module $\mathfrak{a}_{\lambda}$, the relation $[A_s: S_{\lambda}] =$ dim$_{D_{\lambda}}S_{\lambda}$ follows from Lemma 2 of VIII, p. 121. Finally, relation (2) is obtained from (1) by taking the sum over $\lambda$.

#### Scholium {#alg-viii-s8-n3-sch-1 .statement tag=009M}

Let A be a semisimple ring and Z its center. There exist canonical bijections between the following sets:

a) The set $\mathscr{S}(A)$ of classes of simple left A-modules

b) The set $\mathscr{S}(A^o)$ of classes of simple right A-modules

c) The set of minimal two-sided ideals of A

d) The set of maximal two-sided ideals of A

e) The set $\mathscr{S}(Z)$ of classes of simple Z-modules

f) The set of minimal ideals of Z

g) The set of maximal ideals of Z.

Thus, to every element $\lambda$ of $\mathscr{S}$ (A), there correspond the class $\lambda^*$ of the simple right A-module $S^*_{\lambda}$, dual of $S_{\lambda}$, the minimal two-sided ideal $\mathfrak{a}_{\lambda}$ of A (isotypical component of $A_s$ of type $\lambda )$, the maximal two-sided ideal $\mathfrak{b}_{\lambda}$ of A (annihilator of the simple module $S_{\lambda})$, the class of the simple Z-module $Z\cap \mathfrak{a}_{\lambda}$, the minimal ideal $Z\cap \mathfrak{a}_{\lambda}$ of Z, and the maximal ideal $Z\cap \mathfrak{b}_{\lambda}$ of Z.

#### Proposition 12 {#alg-viii-s8-prop-12 .statement tag=009N}

Let M be a module over the semisimple ring A and $\mathscr{S}_M\subset \mathscr{S}$ the support of M. Then the annihilator Ann(M) of M is the two-sided ideal $\sum_{\lambda\in\mathscr{S} \mathscr{S}_M}\mathfrak{a}_{\lambda}$, and the trace ideal $\tau (M)$ of M is the two-sided ideal $\sum_{\lambda\in\mathscr{S}_M}\mathfrak{a}_{\lambda}$. In particular, A is the direct sum of Ann(M) and $\tau (M)$.

By definition (VIII, p. 84$),\mathscr{S}_M$ consists of the classes of simple submodules of M. Since the module M is semisimple, the annihilator of M is the intersection of the annihilators $\mathfrak{b}_{\lambda}$ of the modules of class $\lambda$, for $\lambda$ running through $\mathscr{S}_M$. Now, we have $\mathfrak{b}_{\lambda}=\sum_{\mu\not=\lambda}\mathfrak{a}_\mu$ for every $\lambda \in \mathscr{S}$ (Proposition 9).

Since A is the direct sum of the family $(\mathfrak{a}_{\lambda})_{\lambda\in\mathscr{S}}$, the annihilator of M is indeed equal to $\sum_{\lambda\in\mathscr{S} \mathscr{S}_M}\mathfrak{a}_{\lambda}$.

By definition (VIII, p. 80), the trace ideal $\tau (M)$ is the A-submodule of $A_s$ generated by the images of the A-linear mappings from M to $A_s$. Because M is semisimple, it amounts to the same to say that $\tau (M)$ is generated by the simple submodules of $A_s$ with class belonging to $\mathscr{S}_M$. We therefore have

$$
\tau (M) =\sum_{\lambda\in\mathscr{S}_M}\mathfrak{a}_{\lambda}
$$

#### Corollary {#alg-viii-s8-n3-cor-3 .statement tag=009O}

Let M be a module over the semisimple ring A. The following properties are equivalent:

(i) The A-module M is faithful.

(ii) The support of M is equal to $\mathscr{S}$.

(iii) The A-module M is generating.

Indeed, saying that M is faithful means that its annihilator is reduced to 0, and M is generating if and only if its trace is equal to A (VIII, p. 80, Theorem 1).

### 4. Idempotents and Semisimple Rings

Let A be a ring. Recall that an element $e$ of A is called idempotent (I, §1, No. 4, p. 7) if we have $e^2=e$. It is then also an idempotent element of the opposite ring $A^o$ of A.

#### Proposition 13 {#alg-viii-s8-prop-13 .statement tag=009P}

a) A left ideal $\mathfrak{a}$ of A admits a supplement in $A_s$ if and only if there exists an idempotent $e$ in A such that $\mathfrak{a}= Ae$. The ideal $\mathfrak{a}$ then consists of the elements $x$ of A such that $x=xe$.

b) Let $e$ and $f$ be idempotents in A. We have $Ae\subset Af$ if and only if we have $ef=e$.

c) Let M be an A-module. Then M is projective and monogenous if and only if there exists an idempotent $e$ in A such that M is isomorphic to $Ae$.

The endomorphisms of the A-module $A_s$ are the right multiplications by the elements of A. The projectors in the A-module $A_s$ are therefore the mappings $x\mapsto xe$ where $e$ is an idempotent in A. Moreover, the submodules of $A_s$ are the left ideals, and such a submodule admits a supplement if and only if it is the image of a projector (II, §1, No. 9, p. 211, Proposition 14). Assertion a) follows.

The relation $Ae\subset Af$ is equivalent to $e\in Af$. By a), it is therefore equivalent to $e=ef$; assertion b) follows.

If the A-module M is monogenous, there exists a surjective A-linear mapping $u: A_s\rightarrow M$. If, moreover, M is projective, then there exists a submodule $\mathfrak{a}$ of $A_s$ supplementary to the kernel of $u$. Then $u$ induces an isomorphism from $\mathfrak{a}$ to M. Conversely, if M is isomorphic to a direct factor of $A_s$, then it is monogenous and projective. Assertion c) therefore follows from a).

#### Remark 1 {#alg-viii-s8-n4-rem-1 .statement tag=009Q}

Let $\mathfrak{a}$ be a left ideal of A. By the proof above and the corollary of Proposition 12 of II, §1, No. 8, p. 209, the mapping $e\mapsto A(1-e)$ defines a bijection from the set of idempotents $e$ in A such that $\mathfrak{a}= Ae$ to the set of left ideals $\mathfrak{b}$ of A such that $A_s=\mathfrak{a}\oplus \mathfrak{b}$.

#### Remark 2 {#alg-viii-s8-n4-rem-2 .statement tag=009R}

Let $e$ and $f$ be idempotents in A. By Proposition 13, b), we have $Ae= Af$ if and and only if $ef=e$ and $f e=f$. Consequently, if the ring A is commutative, then the relation $Ae= Af$ is equivalent to $e=f$. This does not hold in general, as shown by the example $A =\mathbf{M}_2(\mathbf{Z}),e= (^{1 0}_{0 0})$, and $f= (^{1 0}_{1 0})$.

We say that idempotents $e$ and $e'$ in the ring A are orthogonal if $ee'=$ $e'e= 0$. Let $(e_i)_{i\in I}$ be a finite family of pairwise orthogonal idempotents in A. Since we have

$$
\sum_ie_i^2=\sum_ie^2_i+\sum_{i\not=j}e_ie_j=\sum_ie_i
$$

the element $\sum_{i\in I}e_i$ of A is idempotent.

A partition of an idempotent $e$ in A is a finite family $(e_i)_{i\in I}$ of pairwise orthogonal idempotents in A such that $e=\sum_{i\in I}e_i$. We say that an idempotent $e$ in A is decomposable if there exists a partition of $e$ consisting of pairwise orthogonal idempotents distinct from 0 and $e$; in the opposite case, we say that it is indecomposable. Observe that 0 is a decomposable idempotent.

#### Proposition 14 {#alg-viii-s8-prop-14 .statement tag=009S}

Let $e$ be an idempotent in A.

a) If $(e_i)_{i\in I}$ is a partition of $e$, then the A-module $Ae$ is the direct sum of the family $(Ae_i)_{i\in I}$.

b) Let $(\mathfrak{a}_i)_{i\in I}$ be a finite family of left ideals of A with direct sum $Ae$. For $i\in I$, denote the component of $e$ in $\mathfrak{a}_i$ by $e_i$. Then $(e_i)_{i\in I}$ is a partition of $e$, and we have $\mathfrak{a}_i= Ae_i$ for every $i\in I$.

c) The A-module $Ae$ is indecomposable if and only if the idempotent $e$ is indecomposable.

Let $(e_i)_{i\in I}$ be a partition of $e$. For every $i\in I$, we have

$$
e_ie=\sum_je_ie_j=e^2_i+\sum_{j\not=i}e_ie_j=e_i
$$

and therefore $Ae_i\subset Ae$. For every $i\in I$, we define an A-linear projector $p_i$ in $Ae$ by setting $p_i(x) =xe_i$. We have $p_ip_j= 0$ if $i\not=j$, and for every $x$ in $Ae$,

$$
x=xe=\sum_ixe_i=\sum_ip_i(x)
$$

Consequently (II, §1, No. 8, p. 20, Proposition $12), Ae$ is the direct sum of the images of the $p_i$. Now, we have $ee_i=e_ie=e_i$, so the image of $p_i$ is $Ae_i$. This proves a).

Take the notation and assumptions of b). Let $i\in I$. Since $e_i$ belongs to $Ae$, we have $e_i=e_ie=\sum_je_ie_j$. Since $Ae$ is the direct sum of the $\mathfrak{a}_j$ and $e_ie_j$ belongs to $\mathfrak{a}_j$ for every $j$, we have $e_i=e_ie_i$ and $e_ie_j= 0$ for $i\not=j$. In other words, $(e_i)_{i\in I}$ is a partition of the idempotent $e$. By a), $Ae$ is the direct sum of the $Ae_i$. By assumption, we have $Ae_i\subset \mathfrak{a}_i$, and $Ae$ is the direct sum of the $\mathfrak{a}_i$. We therefore have $Ae_i=\mathfrak{a}_i$ for every $i\in I$. We have proved b).

Finally, c) follows immediately from a) and b).

#### Remark 3 {#alg-viii-s8-n4-rem-3 .statement tag=00R8}

Applying the previous results to the opposite ring of A, we see, in particular, that a monogenous right A-module M is projective if and only if there exists an idempotent $e$ in A such that M is isomorphic to $eA$. Moreover, $eA$ is an indecomposable right module if and only if $e$ is indecomposable.

Now suppose that the ring A is semisimple, and denote the set of classes of simple left A-modules by $\mathscr{S}$. The A-module $A_s$ is semisimple, and every submodule of $A_s$ is a direct factor. Let $\mathfrak{a}$ be a left ideal of A. By the above, there exists an idempotent $e$ in A such that $\mathfrak{a}= Ae$, and the A-module $\mathfrak{a}$ is simple if and only if it is indecomposable, that is, if and only if $e$ is indecomposable.

Let $(\mathfrak{m}_i)_{i\in I}$ be a family of minimal left ideals of A such that we have $A_s=\oplus_{i\in I}\mathfrak{m}_i$. By Proposition 14, there exists a partition $(\varepsilon_i)_{i\in I}$ of 1 consisting of indecomposable idempotents such that $\mathfrak{m}_i= A\varepsilon_i$ for every $i\in I$.

For every $\lambda \in \mathscr{S}$, let $S_{\lambda}$ be an A-module of class $\lambda$, and let $\mathfrak{a}_{\lambda}$ be the isotypical component of type $\lambda$ of the A-module $A_s$. Since A is the direct sum of the family $(\mathfrak{a}_{\lambda})_{\lambda\in\mathscr{S}}$, there exists a partition $(e_{\lambda})_{\lambda\in\mathscr{S}}$ of 1 such that $\mathfrak{a}_{\lambda}= Ae_{\lambda}$ for every $\lambda \in \mathscr{S}$. For $\lambda \in \mathscr{S}$, denote by $I(\lambda )$ the set of indices $i\in I$ such that the simple A-module $\mathfrak{m}_i$ is of type $\lambda$. By Proposition 4, b) of VIII, p. 65, we have

$$
\mathfrak{a}_{\lambda}=_{i\in}\bigoplus_{I(\lambda)}\mathfrak{m}_i \tag{3}
$$

The idempotent $e_{\lambda}$ is the component of 1 in $\mathfrak{a}_{\lambda}$, so $e_{\lambda}=\sum_{i\in I(\lambda)}\varepsilon_i$.

#### Proposition 15 {#alg-viii-s8-prop-15 .statement tag=009T}

Suppose that the ring A is semisimple.

a) For every $\lambda \in \mathscr{S},e_{\lambda}$ is the unique element of the center Z of A satisfying the relations $(e_{\lambda})_{S_{\lambda}}= 1_{S_{\lambda}}$ and $(e_{\lambda})_{S_\mu}= 0$ for $\mu\not=\lambda$.

b) The indecomposable idempotents in the ring Z are the $e_{\lambda}$, and the minimal ideals of Z are the $Ze_{\lambda}$ for $\lambda \in \mathscr{S}$.

c) Let M be an A-module and $(M_{\lambda})_{\lambda\in\mathscr{S}}$ the family of its isotypical components. The family of projectors associated with the decomposition of M into the direct sum of the $M_{\lambda}$ (VIII, p. 65) is $((e_{\lambda})_M)_{\lambda\in\mathscr{S}}$, and we have $M_{\lambda}=\mathfrak{a}_{\lambda}M$ for every $\lambda \in \mathscr{S}$.

Let $\lambda$ and $\mu$ be distinct in $\mathscr{S}$. We have $e_{\lambda}\in \mathfrak{a}_{\lambda}$, and $\mathfrak{a}_{\lambda}$ is contained in the annihilator $\mathfrak{b}_\mu$ of the A-module $S_\mu$ (VIII, p. 142, Proposition 9). We therefore have $(e_{\lambda})_{S_\mu}= 0$. The relation $(e_{\lambda})_{S_{\lambda}}= 1_{S_{\lambda}}$ follows because we have $1 =\sum_{\nu\in\mathscr{S}}e_{\nu}$. Assertion a) is then a consequence of Proposition 8 of VIII, p. 141.

Let $\lambda$ be in $\mathscr{S}$. The two-sided ideal $\mathfrak{a}_{\lambda}$ of A consists of the elements $x$ such that $x=xe_{\lambda}$; we therefore have $Z\cap \mathfrak{a}_{\lambda}= Ze_{\lambda}$, and therefore b) by Proposition 10, b).

Let us prove c). Let $x$ be an element of M. We have $e_{\lambda}\in \mathfrak{a}_{\lambda}$ for every $\lambda \in \mathscr{S}$. Since the mapping $a\mapsto ax$ from $A_s$ to M is A-linear, we have $\mathfrak{a}_{\lambda}x\subset M_{\lambda}$ (VIII, p. 66, Proposition 5) and, in particular, $e_{\lambda}x\in M_{\lambda}$. We have $1 =\sum_{\lambda\in\mathscr{S}}e_{\lambda}$, hence $x=\sum_{\lambda\in\mathscr{S}}e_{\lambda}x$. Consequently, $e_{\lambda}x$ is the component of $x$ in $M_{\lambda}$.

#### Remark 4 {#alg-viii-s8-n4-rem-4 .statement tag=009U}

Suppose that the ring A is semisimple. Let $(e_i)_{i\in I}$ be a partition of 1 consisting of nonzero idempotents in the center Z of A. If Card(I) = Card($\mathscr{S})$, then the $e_i$ are the indecomposable idempotents in Z.

### Exercises {#alg-viii-s8-exercises}

See the [exercises for § 8](exercises/s8/).
