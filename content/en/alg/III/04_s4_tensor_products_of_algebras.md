---
book: alg
book_title: Algebra
chapter: III
chapter_title: TENSOR ALGEBRAS, EXTERIOR ALGEBRAS, SYMMETRIC ALGEBRAS
section: 4
section_title: Tensor products of algebras
lang: en
source: alg-i-iii
source_edition: 1998, Springer
pdf_pages: 0484-0508, 0650-0651
extraction: ocr
subsections:
    - "no": 1
      title: TENSOR PRODUCT OF A FINITE FAMILY OF ALGEBRAS
      page: 0
      pdf_page: 484
    - "no": 2
      title: UNIVERSAL CHARACTERIZATION OF TENSOR PRODUCTS OF ALGEBRAS
      page: 0
      pdf_page: 487
    - "no": 3
      title: MODULES AND MULTIMODULES OVER TENSOR PRODUCTS OF ALGEBRAS
      page: 0
      pdf_page: 489
    - "no": 4
      title: TENSOR PRODUCT OF ALGEBRAS OVER A FIELD
      page: 0
      pdf_page: 492
    - "no": 5
      title: TENSOR PRODUCT OF AN INFINITE FAMILY OF ALGEBRAS
      page: 0
      pdf_page: 494
    - "no": 6
      title: COMMUTATION LEMMAS
      page: 0
      pdf_page: 496
    - "no": 7
      title: TENSOR PRODUCT OF GRADED ALGEBRAS RELATIVE TO COMMUTATION FACTORS
      page: 0
      pdf_page: 498
    - "no": 8
      title: TENSOR PRODUCT OF GRADED ALGEBRAS OF THE SAME TYPES
      page: 0
      pdf_page: 504
    - "no": 9
      title: ANTICOMMUTATIVE ALGEBRAS AND ALTERNATING ALGEBRAS
      page: 0
      pdf_page: 506
statements: 43
exercises: 2
content_sha256: e2b0067020818d84b0b33e5febea1d4a9107e190bf3bc4bf6ffb9ec89a7d669b
---

## § 4. TENSOR PRODUCTS OF ALGEBRAS

From § 4 to § 8 inclusive, A denotes a commutative ring and, unless otherwise mentioned, the algebras considered are assumed to be associative and unital and the algebra homomorphisms are assumed to be unital.

### 1. TENSOR PRODUCT OF A FINITE FAMILY OF ALGEBRAS

A always denotes a commutative ring with unit element. Let (E_i)_{i \in I} be a finite family of A-algebras and let E = \bigotimes_{i \in I} E_i be the tensor product A-module of the A-modules E_i (II, § 3, no. 9). We shall define an A-algebra structure on E. Let m_i: E_i \otimes_A E_i \to E_i be the A-linear mapping defining the multiplication on E_i (§ 1, no. 3). Consider the A-linear mapping

$$
m' = \bigotimes_{i \in I} m_i: \bigotimes_{i \in I} (E_i \otimes_A E_i) \to \bigotimes_{i \in I} E_i = E;
$$

the composite mapping

$$
\left( \bigotimes_{i \in I} E_i \right) \otimes_A \left( \bigotimes_{i \in I} E_i \right) \xrightarrow{\tau} \bigotimes_{i \in I} (E_i \otimes_A E_i) \xrightarrow{m'} \bigotimes_{i \in I} E_i
$$

where $ \tau $ is the associativity isomorphism (II, § 3, no. 9) is an A-linear mapping $ m : E \otimes_A E \to E $; we shall see that $ m $ defines an (associative and unital) algebra structure on $ E $. For, on explicitly performing the multiplication defined by $ m $, we obtain the formula

(1)
$$
\left( \bigotimes_{i \in I} x_i \right) \left( \bigotimes_{i \in I} y_i \right) = \bigotimes_{i \in I} (x_i y_i) \quad \text{for } x_i, y_i \text{ in } E_i \text{ and } i \in I.
$$

It is therefore seen already, by linearity, that if $ e_i $ is the unit element of $ E_i $, $ e = \bigotimes_{i \in I} e_i $ is unit element of $ E $. On the other hand, the associativity of each of the $ E_i $ implies the relation

$$
\left( \left( \bigotimes_{i \in I} x_i \right) \left( \bigotimes_{i \in I} y_i \right) \right) \left( \bigotimes_{i \in I} z_i \right) = \bigotimes_{i \in I} (x_i y_i z_i) = \left( \bigotimes_{i \in I} x_i \right) \left( \left( \bigotimes_{i \in I} y_i \right) \left( \bigotimes_{i \in I} z_i \right) \right)
$$

whence, by linearity, the relation $ x(yz) = (xy)z $ for all $ x, y, z $ in $ E $.

#### Definition 1 {#alg-iii-s4-def-1 .statement}

*Given a family* $ (E_i)_{i \in I} $ *of algebras over* $ A $, *the tensor product of this family*, denoted by $ \bigotimes_{i \in I} E_i $ (or, when $ I $ is the interval $ \{1, n\} $ of $ \mathbf{N} $, $ E_1 \otimes_A E_2 \otimes \cdots \otimes_A E_n $, or simply $ E_1 \otimes E_2 \otimes \cdots \otimes E_n $) *is the algebra obtained by giving the tensor product of the* $ A $*-modules* $ E_i $ *the multiplication defined by* (1).

Relation (1) shows that the tensor product $ \bigotimes_{i \in I} E_i^0 $ of the *opposite* algebras to the $ E_i $ is the opposite algebra to $ \bigotimes_{i \in I} E_i $; in particular, if the $ E_i $ are *commutative*, so is $ \bigotimes_{i \in I} E_i $.

Let $ (E_i)_{i \in I} $ and $ (F_i)_{i \in I} $ be two families of $ A $-algebras with the same finite indexing set $ I $. For each $ i \in I $, let $ f_i : E_i \to F_i $ be an $ A $-algebra homomorphism. Then the $ A $-linear mapping

$$
f = \bigotimes_{i \in I} f_i : \bigotimes_{i \in I} E_i \to \bigotimes_{i \in I} F_i
$$

is an *A-algebra homomorphism*, as follows from (1).

For every partition $ (I_j)_{j \in J} $ of $ I $, the associativity isomorphisms

$$
\bigotimes_{j \in J} \left( \bigotimes_{i \in I_j} E_i \right) \to \bigotimes_{i \in I} E_i
$$

(II, § 3, no. 9) are also *algebra* isomorphisms, as follows from (1) and their definitions.

When $ I $ is the interval $[1, n]$ of $ \mathbf{N} $ and all the algebras $ E_i $ are equal to the same algebra $ E $, the tensor product algebra $ \bigotimes_{i \in I} E_i $ is also denoted by $ E^{\otimes n} $.

We shall restrict our attention in the remainder of this no. to the properties of tensor products of two algebras, leaving to the reader the task of extending them to tensor products of arbitrary finite families.

Let $ E, F $ be two $ A $-algebras; if $ a $ (resp. $ b $) is a left ideal of $ E $ (resp. $ F $), the canonical image $ \operatorname{Im}(a \otimes b) $ of $ a \otimes_A b $ in $ E \otimes_A F $ is a left ideal of $ E \otimes_A F $; there are analogous results when "left ideal" is replaced by "right ideal" or "two-sided ideal". Moreover:

#### Proposition 1 {#alg-iii-s4-prop-1 .statement}

*Let $ E, F $ be two $ A $-algebras and $ a $ (resp. $ b $) a two-sided ideal of $ E $ (resp. $ F $). Then the canonical $ A $-module isomorphism*

$$
(E/a) \otimes (E/b) \to (E \otimes F)/(\operatorname{Im}(a \otimes F) + \operatorname{Im}(E \otimes b))
$$

(II, § 3, no. 6, Corollary 1 to Proposition 6) *is an algebra isomorphism*.

This follows from (1) and the definition given *loc. cit*.

#### Corollary 1 {#alg-iii-s4-prop-1-cor-1 .statement}

*Let $ E $ be an $ A $-algebra and $ a $ an ideal of $ A $. Then the $ A $-module $ aE $ is a two-sided ideal of $ E $ and the canonical $ (A/a) $-module isomorphism*

$$
(A/a) \otimes_A E \to E/aE
$$

*is an* $ (A/a) $*-algebra isomorphism*.

#### Corollary 2 {#alg-iii-s4-prop-1-cor-2 .statement}

*If $ a, b $ are two ideals of $ A $, $ (A/a) \otimes_A (A/b) $ is canonically isomorphic to $ A/(a + b) $*.

#### Corollary 3 {#alg-iii-s4-prop-1-cor-3 .statement}

*Let $ E, F $ be two $ A $-algebras and $ a $ an ideal of $ A $ contained in the annihilator of $ F $. Then the $ (A/a) $-algebra $ E \otimes_A F $ is canonically isomorphic to $ (E/aE) \otimes_{A/a} F $*.

#### Proposition 2 {#alg-iii-s4-prop-2 .statement}

*Let $ (E_\lambda)_{\lambda \in L} $ and $ (F_\mu)_{\mu \in M} $ be two families of $ A $-algebras. The canonical mapping* (II, § 3, no. 7)

$$
\left( \bigoplus_{\lambda \in L} E_\lambda \right) \otimes_A \left( \bigoplus_{\mu \in M} F_\mu \right) \to \bigoplus_{(\lambda, \mu) \in L \times M} (E_\lambda \otimes_A F_\mu)
$$

*is an algebra isomorphism*.

This follows immediately from II, § 3, no. 7, Proposition 7 and the definition of multiplication on $ E \otimes F $.

#### Proposition 3 {#alg-iii-s4-prop-3 .statement}

*Let $ A, B $ be two commutative rings, $ \varphi : A \to B $ a ring homomorphism and $ E, F $ two $ A $-algebras. Then the canonical $ B $-module isomorphism*

$$
\varphi^*(E) \otimes_B \varphi^*(F) \to \varphi^*(E \otimes_A F)
$$

(II, § 5, no. 1, Proposition 3) *is a $ B $-algebra isomorphism*.

#### Proposition 4 {#alg-iii-s4-prop-4 .statement}

Let $ A, B $ be two commutative rings, $ \rho : A \to B $ a ring homomorphism, $ E $ an $ A $-algebra and $ F $ a $ B $-algebra. Then the canonical $ A $-module isomorphism

$$
\rho_*(F) \otimes_A E \to \rho_*(F \otimes_B \rho^*(E))
$$

(II, § 5, no. 2, Proposition 6) is an $ A $-algebra isomorphism.

The verifications are trivial on account of § 1, no. 5.

In particular, the $ A $-algebra structure on $ B \otimes_A E $, obtained by restricting the ring $ B $ of scalars to $ A $, is identical with the structure of the algebra $ B \otimes_A E $, the tensor product of the $ A $-algebras $ B $ and $ E $.

Finally, if $ (A_i, \phi_{ji}) $ is a direct system of commutative rings, $ (E_i, f_{ji}) $ and $ (F_i, g_{ji}) $ two direct systems of $ A_i $-algebras ($ \S 1 $, no. 6) and $ A = \lim \rightarrow A_i $, the canonical $ A $-module isomorphism

$$
\lim \rightarrow (E_i \otimes_{A_i} F_i) \to (\lim \rightarrow E_i) \otimes_A (\lim \rightarrow F_i)
$$

(II, § 6, no. 3, Proposition 7) is also an $ A $-algebra isomorphism, as follows from the definitions.

Examples of tensor products of algebras. (1) Let $ A $ be a commutative ring and $ M, N $ two $ A $-modules; the canonical mapping

$$
\text{End}_A(M) \otimes_A \text{End}_A(N) \to \text{End}_A(M \otimes_A N)
$$

(II, § 4, no. 4) is an $ A $-algebra homomorphism, as follows from II, § 3, no. 2, formula (5). When $ M $ or $ N $ is a finitely generated projective $ A $-module, we know that this homomorphism is bijective (II, § 4, no. 4, Proposition 4). In particular we recover the definition of the tensor product of two square matrices.

(2) Let $ S, T $ be two monoids and $ A^{(S)} $ and $ A^{(T)} $ the algebras of the monoids $ S $ and $ T $ over the ring $ A $ (III, § 2, no. 6); then there is a canonical $ A $-algebra isomorphism

$$
A^{(S)} \otimes_A A^{(T)} \to A^{(S \times T)}.
$$

The elements $ e_s \otimes e_t $ (resp. $ e_{(s,t)} $), where $ s $ runs through $ S $ and $ t $ runs through $ T $, form a basis of $ A^{(S)} \otimes_A A^{(T)} $ by virtue of II, § 3, no. 7, Corollary 2 to Proposition 7 (resp. of $ A^{(S \times T)} $; the desired isomorphism is obtained by mapping $ e_s \otimes e_t $ to $ e_{(s,t)} $ and it follows from the definitions that this is indeed an algebra isomorphism.

### 2. UNIVERSAL CHARACTERIZATION OF TENSOR PRODUCTS OF ALGEBRAS

#### Proposition 5 {#alg-iii-s4-prop-5 .statement}

Let $ (E_i)_{i \in I} $ be a finite family of $ A $-algebras and, for each $ i \in I $, let $ e_i $ be the unit element of $ E_i $. For each $ i \in I $, let $ u_i : E_i \to E = \bigotimes_{i \in I} E_i $ be the $ A $-linear mapping defined by

$$
u_i(x_i) = \bigotimes_j x'_j \quad \text{with } x'_i = x_i \text{ and } x'_j = e_j \text{ for } j \neq i.
$$

(i) *The $ u_i $ are $ \mathbf{A} $-algebra isomorphisms; further, for $ i \neq j $, the elements $ u_i(x_i) $ and $ u_j(x_j) $ are permutable in $ \mathbf{E} $ for all $ x_i \in \mathbf{E}_i $ and $ x_j \in \mathbf{E}_j $ and $ \mathbf{E} $ is generated by the union of the subalgebras $ u_i(\mathbf{E}_i) $.

(ii) *Let $ \mathbf{F} $ be an $ \mathbf{A} $-algebra and, for all $ i \in \mathbf{I} $, let $ v_i : \mathbf{E}_i \to \mathbf{F} $ be an $ \mathbf{A} $-algebra homomorphism, where the $ v_i $ are such that, for $ i \neq j $, $ v_i(x_i) $ and $ v_j(x_j) $ are permutable in $ \mathbf{F} $ for all $ x_i \in \mathbf{E}_i $ and $ x_j \in \mathbf{E}_j $. Then there exists one and only one $ \mathbf{A} $-algebra homomorphism $ w : \mathbf{E} \to \mathbf{F} $ such that*

$$
v_i = w \circ u_i \quad \text{for all } i \in \mathbf{I}.
$$

(i) The mapping $ u_i $ is an algebra homomorphism by definition of the multiplication on $ \mathbf{E} $. If $ i \neq j $, $ x_i \in \mathbf{E}_i, x_j \in \mathbf{E}_j $, then

$$
u_i(x_i) = \bigotimes_k x'_k \quad \text{with } x'_i = x_i, x'_k = e_k \text{ for } k \neq i,
$$
$$
u_j(x_j) = \bigotimes_k x''_k \quad \text{with } x''_j = x_j, x''_k = e_k \text{ for } k \neq j.
$$

Clearly $ x'_k x''_k = x''_k x'_k $ for all $ k \in \mathbf{I} $ and hence $ u_i(x_i) $ and $ u_j(x_j) $ commute in $ \mathbf{E} $ by formula (1) (no. 1) defining the multiplication in $ \mathbf{E} $. The last assertion follows from the relation $ \bigotimes_i x_i = \prod_{i \in \mathbf{I}} u_i(x_i) $.

(ii) For each $ i \in \mathbf{I} $, let $ x_i $ be an element of $ \mathbf{E}_i $. The product $ \prod_{i \in \mathbf{I}} v_i(x_i) $ is then defined in $ \mathbf{F} $ independently of any ordering on $ \mathbf{I} $ since the algebra $ \mathbf{F} $ is associative and the elements $ v_i(x_i) $ are pairwise permutable. The mapping $ (x_i)_{i \in \mathbf{I}} \to \prod_{i \in \mathbf{I}} v_i(x_i) $ of $ \prod_{i \in \mathbf{I}} \mathbf{E}_i $ into $ \mathbf{F} $ is obviously $ \mathbf{A} $-multilinear and there therefore exists one and only one $ \mathbf{A} $-linear mapping $ w : \mathbf{E} \to \mathbf{F} $ such that

$$
w\left( \bigotimes_i x_i \right) = \prod_i v_i(x_i).
$$

Now, the desired $ \mathbf{A} $-algebra homomorphism $ w : \mathbf{E} \to \mathbf{F} $ must satisfy (5), which follows from (4) and the fact that $ \bigotimes_i x_i = \prod_{i \in \mathbf{I}} u_i(x_i) $. This proves the uniqueness of $ w $; it remains to show that the $ \mathbf{A} $-linear mapping $ w $ defined by (5) is an $ \mathbf{A} $-algebra homomorphism and satisfies (4). The fact that $ w $ satisfies (4) is obvious: it suffices to apply (5) to the case where $ x_j = e_j $ for $ j \neq i $ and we obtain $ w(u_i(x_i)) = v_i(x_i) $. Finally, $ w $ is an algebra homomorphism, for

$$
w\left( \left( \bigotimes_i x_i \right) \left( \bigotimes_i y_i \right) \right) = w\left( \bigotimes_i (x_i y_i) \right) = \prod_i v_i(x_i y_i)
$$
$$
= \prod_i (v_i(x_i) v_i(y_i)) = \left( \prod_i v_i(x_i) \right) \cdot \left( \prod_i v_i(y_i) \right)
$$

since $ v_i(x_i) $ commutes with $ v_j(y_j) $ for $ j \neq i $; hence

$$
w w \left( \left( \bigotimes_i x_i \right) \left( \bigotimes_i y_i \right) \right) = w \left( \bigotimes_i x_i \right) . w \left( \bigotimes_i y_i \right)
$$

which, by linearity, completes the proof.

The ordered pair consisting of E and the canonical mapping $ \phi : (x_i) \mapsto \bigotimes_i x_i $ of $ \prod_i E_i $ into E is a solution of the universal mapping problem (Set Theory, IV, § 3, no. 1) where $ \Sigma $ is the species of A-algebra structure, the morphisms being the A-algebra homomorphisms and the $ \alpha $-mappings the mappings $ \prod_i u_i $ of $ \prod_i E_i $ into an A-algebra such that the $ u_i $ are A-algebra homomorphisms and $ u_i(x_i) $ and $ u_j(x_j) $ commute for $ i \neq j $, for all $ x_i \in E_i $ and $ x_j \in E_j $.

#### Corollary {#alg-iii-s4-n2-cor-1 .statement}

*Let* $ (E_i)_{i \in I}, (F_i)_{i \in I} $ *be two finite families of A-algebras and, for all* $ i \in I $, *let* $ f_i : E_i \to F_i $ *be an algebra homomorphism. If* $ u_i : E_i \to \bigotimes_{j \in I} E_j, v_i : F_i \to \bigotimes_{j \in I} F_j $ *are the canonical homomorphisms, the mapping* $ f = \bigotimes_i f_i $ *(cf. no. 1)* *is the unique A-algebra homomorphism such that* $ f \circ u_i = v_i \circ f_i $ *for all* $ i \in I $.

It suffices to note that the homomorphisms $ g_i = v_i \circ f_i $ are such that $ g_i(x_i) = v_i(f_i(x_i)) $ and $ g_j(x_j) = v_j(f_j(x_j)) $ commute for $ i \neq j $, $ x_i \in E_i $ and $ x_j \in E_j $; then apply Proposition 5.

When, in Proposition 5, the algebra F is assumed to be *commutative*, the hypothesis that $ v_i(x_i) $ and $ v_j(x_j) $ are permutable for $ i \neq j $ is automatically satisfied. Hence, *when F is commutative*, there is a canonical bijection

$$
\text{Hom}_{A\text{-alg.}} \left( \bigotimes_i E_i, F \right) \to \prod_i \text{Hom}_{A\text{-alg.}} (E_i, F),
$$

namely the one which associates with every homomorphism $ w $ of $ \bigotimes_i E_i $ into F the family of $ w \circ u_i $.

Note that if E is a commutative A-algebra, the ring structure of $ E \otimes_A F $ is the same as that of $ F_{(E)} $ (\S 1, no. 5).

### 3. MODULES AND MULTIMODULES OVER TENSOR PRODUCTS OF ALGEBRAS

#### Definition 2 {#alg-iii-s4-def-2 .statement}

*Let E be a (unital) A-algebra. A left (resp. right) E-module is a left (resp. right) module over the underlying ring of E.*

Unless otherwise mentioned, all the modules and multimodules considered in this no. are left modules and multimodules.

If M is an E-module, the homomorphism $ \eta : A \to E $ (\S 1, no. 4) then defines on M an A-module structure, said to be underlying the E-module structure on M; for $ \alpha \in A, s \in E, x \in M $,

$$
\alpha(sx) = s(\alpha x) = (\alpha s)x,
$$

so that for all $ s \in E $, the homothety $ h_s : x \mapsto sx $ of M is an endomorphism of the underlying A-module structure. Conversely, being given an E-module structure on M is equivalent to being given an A-module structure on M and an A-algebra homomorphism $ s \mapsto h_s $ of E into $ \mathrm{End}_A(M) $.

#### Definition 3 {#alg-iii-s4-def-3 .statement}

*Let E and F be two (unital) A-algebras and M a set with an E-module structure and an F-module structure. M is called a (left) bimodule over the algebras E and F if:*

(1) *M is a bimodule over the underlying rings of E and F* (II, § 1, no. 14);
(2) *the two A-module structures underlying the E-module and F-module structures on M are identical*.

The latter condition says that if e and $ e' $ are the unit elements of E and F respectively, then

$$
(\alpha e)x = (\alpha e')x \quad \text{for } \alpha \in A, x \in M;
$$

then $ \alpha x $ is used to denote the common value of the two sides.

It can also be said that being given on M a bimodule structure over E and F is equivalent to being given an A-module structure on M and also two A-algebra homomorphisms $ s \mapsto h'_s $ of E into $ \mathrm{End}_A(M) $ and $ t \mapsto h''_t $ of F into $ \mathrm{End}_A(M) $ such that $ h'_s h''_t = h''_t h'_s $ for all $ s \in E $ and $ t \in F $. Consequently (no. 2, Proposition 5) an A-algebra homomorphism $ u \mapsto h_u $ of $ E \otimes_A F $ into $ \mathrm{End}_A(M) $ is canonically derived such that $ h_{s \otimes t} = h'_s h''_t = h''_t h'_s $ for $ s \in E $ and $ t \in F $. In other words, an $(E \otimes_A F)$-module structure is thus defined on M, which is said to be associated with the given bimodule structure over E and F and under which

$$
(s \otimes t).x = s(tx) = t(sx) \quad \text{for } s \in E, t \in F \text{ and } x \in M.
$$

The given E-module and F-module structures on M can be derived from this $(E \otimes_A F)$-module structure by restrictions of the ring of scalars, corresponding to the two canonical homomorphisms $ E \to E \otimes_A F $ and $ F \to E \otimes_A F $.

Conversely, if an $(E \otimes_A F)$-module structure is given on M, by means of the canonical homomorphisms $ E \to E \otimes_A F $ and $ F \to E \otimes_A F $ an E-module structure and an F-module structure on M and it is immediate that M is a *bimodule* over the algebras E and F with these two structures and that the given $(E \otimes_A F)$-module structure is associated with this bimodule structure.

Thus a one-to-one correspondence has been established between $(E \otimes_A F)$-module and bimodules over the algebras E and F. Clearly every sub-bimodule of M is a submodule for the associated $(E \otimes_A F)$-module structure and conversely. There are analogous results for quotients, products, direct sums and inverse and direct limits. Finally, if $ M' $ is another bimodule over the algebras E and F and $ f : M \to M' $ is a bimodule homomorphism, $ f $ is also an $ (E \otimes_A F) $-module homomorphism and conversely.

There are obviously corresponding statements for right bimodule structures, or when for example there is a left E-module structure and a right F-module structure; in this case we speak of an $ (E, F)$-bimodule and being given such a structure amounts to being given a left bimodule structure over E and $ F^o $.

#### Example {#alg-iii-s4-n3-exa-1 .statement}

(1) Let B be an A-algebra; the ring B has canonically a (B, B)-bimodule structure (II, § 1, no. 14, Example 1) and, if e is the unit element of B, then $ (\alpha e)x = x(\alpha e) = \alpha x $ for all $ x \in B $ and all $ \alpha \in A $; B can therefore be considered as a left bimodule over the algebras B and $ B^o $ (opposite to B); there is therefore associated with the (B, B)-bimodule structure on B a (B $ \otimes_A B^o $)-module structure such that, for $ b, x $ and $ b' $ in B,

$$
(b \otimes b').x = bx b'
$$

the right-hand side being the product in the ring B.

(2) Let E and F be two A-algebras, $ e, e' $ their respective unit elements, M an E-module and N an F-module; these module structures define on M a bimodule structure over the rings A and E and on N a bimodule structure over the rings A and F; from these is therefore derived a bimodule structure over the rings E and F on the tensor product $ M \otimes_A N $, defined by

$$
x.(m \otimes n) = (x.m) \otimes n, \quad y.(m \otimes n) = m \otimes (y.n)
$$

for $ x \in E, y \in F, m \in M, n \in N $ (II, § 3, no. 4); it is also seen that conditions (8) hold and hence the above bimodule structure is associated with an $ (E \otimes_A F) $-module structure on $ M \otimes_A N $, such that

$$
(x \otimes y).(m \otimes n) = (x.m) \otimes (y.n)
$$

for $ x \in E, y \in F, m \in M, n \in N $.

In particular, taking $ M = E_s, E_s \otimes_A N $ has canonically an $ (E \otimes_A F) $-module structure; on the other hand, $ E \otimes_A N $ is canonically identified with $ E \otimes_A (F_d \otimes_F N) = (E \otimes_A F) \otimes_F N $, where $ E \otimes_A F $ is considered as having its right F-module structure defined by the canonical homomorphism $ v : F \to E \otimes_A F $; for $ x, x' $ in E, $ y \in F, n \in N $, $ x' \otimes n $ is thus identified with $ (x' \otimes e') \otimes n $ and $ (x \otimes y).(x' \otimes n') = (xx') \otimes (y.n) $ with $ ((xx') \otimes y) \otimes n $. The $ (E \otimes_A F) $-module $ E_s \otimes_A N $ is thus identified with the $ (E \otimes_A F) $-module derived from N by extending the scalars to $ E \otimes_A F $ by means of the homomorphism $ v $ (II, § 5, no. 1). The canonical mapping $ n \mapsto e \otimes n $ of N into $ E_s \otimes_A N $ is identified with the canonical mapping $ n \mapsto (e \otimes e') \otimes n $ of N into $ (E \otimes_A F) \otimes_F N $; this is known to be an F-homomorphism.

With the same notation, let P be a right (E \otimes_A F)-module; then there is a canonical Z-module isomorphism

(11) $$ P \otimes_{E \otimes_A F} (E_s \otimes_A N) \to P \otimes_F N $$

where on the right-hand side P is considered as a right F-module by means of the canonical homomorphism $ v $. For P is canonically identified with $ P \otimes_{E \otimes_A F} (E \otimes_A F) $ and $ (E \otimes_A F) \otimes_F N $ with $ E \otimes_A (F \otimes_F N) $ and hence with $ E \otimes_A N $, which establishes the stated isomorphism (II, § 3, no. 8, Proposition 8 and II, § 3, no. 4, proposition 4).

All the above extends to *multimodules* (II, § 1, no. 14).

### 4. TENSOR PRODUCT OF ALGEBRAS OVER A FIELD

Let K be a commutative *field* and E, F two algebras over K whose respective unit elements $ e, e' $ are *non-zero*. Then the homomorphisms $ \eta_E : K \to E $ and $ \eta_F : K \to F $ (§ 1, no. 3) are injections which allow us to identify K with a subfield of E (resp. F). The canonical homomorphisms $ u : E \to E \otimes_K F $ and $ v : F \to E \otimes_K F $, defined by $ u(x) = x \otimes e' $ and $ v(y) = e \otimes y $ are *injective* (II, § 7, no. 9, Proposition 19) and allow us to identify E and F with *subalgebras* of $ E \otimes_K F $, both having as unit element the unit element $ e \otimes e' $ of $ E \otimes_K F $. In $ E \otimes_K F, E \cap F = K $ (II, § 7, no. 9, Proposition 19).

If E' and F' are subalgebras of E and F respectively, the canonical homomorphism $ E' \otimes_K F' \to E \otimes_K F $ is injective and allows us to identify $ E' \otimes_K F' $ with the subalgebra of $ E \otimes_K F $ generated by $ E' \cup F' $ (II, § 7, no. 7, Proposition 14).

#### Proposition 6 {#alg-iii-s4-prop-6 .statement}

*Let E, F be two non-zero algebras over a commutative field, K, C (resp. D) a subalgebra of E (resp. F) and C' (resp. D') the centralizer of C in E (resp. D in F). Then the centralizer of C \otimes_K D in E \otimes_K F is C' \otimes_K D'.*

It all reduces to verifying that an element $ z = \sum_i x_i \otimes y_i $ of the centralizer of $ C \otimes_K D $ ($ x_i \in F, y_i \in F $) belongs to $ C' \otimes_K D' $; we know that

$$
C' \otimes_K D' = (C' \otimes_K F) \cap (E \otimes_K D')
$$

(II, § 7, no. 7, Corollary to Proposition 14). The $ y_i $ may be assumed to be linearly independent over K; for all $ x \in C $, of necessity $ (x \otimes e')z = z(x \otimes e') $, that is $ \sum_i (xx_i - x_ix) \otimes y_i = 0 $, whence $ xx_i = x_ix $ for all $ i $ (II, § 3, no. 7, Corollary 1 to Proposition 7); hence of necessity $ x_i \in C' $ for all $ i $ and therefore $ z \in C' \otimes_K F $; it can similarly be shown that $ z \in E \otimes_K D' $, whence the proposition.

#### Corollary {#alg-iii-s4-n4-cor-1 .statement}

*If Z and Z' are the respective centres of E and F, the centre of E \otimes_K F is Z \otimes_K Z'*.

Let E and F be two subalgebras of an algebra G over a commutative field K; suppose that every element of E commutes with every element of F. Then the canonical injections $ i : E \to G, j : F \to G $ define a canonical homomorphism $ h = i \otimes j : E \otimes_K F \to G $ (no. 2, Proposition 5) such that
$$
(i \otimes j)(x \otimes y) = xy \quad \text{for } x \in E, y \in F.
$$

#### Definition 4 {#alg-iii-s4-def-4 .statement}

*Given an algebra G over a commutative field K, two subalgebras E, F of G are said to be linearly disjoint over K if they satisfy the following conditions:*
(1) *every element of E commutes with every element of F;*
(2) *the canonical homomorphism of $ E \otimes_K F $ into G is injective.*

#### Proposition 7 {#alg-iii-s4-prop-7 .statement}

*Let G be an algebra over a commutative field K and E, F two subalgebras of G such that every element of E commutes with every element of F. For E and F to be linearly disjoint over K, it is necessary and sufficient that there exist a basis of E over K which is a free subset of G for the right F-module structure on G. When this is so:*
(i) *the canonical homomorphism $ h : E \otimes_K F \to G $ is an isomorphism of $ E \otimes_K F $ onto the subalgebra of G generated by $ E \cup F $;*
(ii) $ E \cap F = K; $
(iii) *every free subset of E (resp. F) over K is a free subset of G with its right or left F-module (resp. E-module) structure.*

The condition of the statement is obviously necessary, since every basis of E over K is a basis of $ E \otimes_K F $ with its right F-module structure (II, § 3, no. 7, Corollary 1 to Proposition 7). To see that the condition is sufficient, note that the image H of $ E \otimes_K F $ under h is the set of sums $ \sum_i x_i y_i = \sum_i y_i x_i $ in G, with $ x_i \in E $ and $ y_i \in F $; if $ (a_\lambda) $ is a basis of E over K, H is therefore also the submodule of the (right or left) F-module G, generated by $ (a_\lambda) $. The condition of the statement therefore means that there exists a basis $ (a_\lambda) $ of E which is also a basis of the F-module H; it follows that h is injective. Assertion (iii) follows from the fact that every free subset of E is contained in a basis of E (II, § 7, no. 1, Theorem 2).

#### Corollary 1 {#alg-iii-s4-prop-7-cor-1 .statement}

*For the canonical homomorphism of $ E \otimes_K F $ into G to be bijective, it is necessary and sufficient that there exist a basis of E over K which is a basis of the (right or left) F-module G.*

#### Corollary 2 {#alg-iii-s4-prop-7-cor-2 .statement}

*Let E, F be two subalgebras of G, of finite rank over K and such that every element of E commutes with every element of F. For E and F to be linearly disjoint over K, it is necessary and sufficient that the subalgebra H of G generated by $ E \cup F $ be such that*
$$
[H : K] = [E : K] \cdot [F : K].
$$
This says that the rank over K of the surjective canonical homomorphism h : E \otimes_K F \to H is equal to the rank of E \otimes_K F over K, which is equivalent to saying that this homomorphism is bijective (II, § 7, No. 4, Proposition 9).

### 5. TENSOR PRODUCT OF AN INFINITE FAMILY OF ALGEBRAS

Let A be a commutative ring and (E_i)_{i \in I} an arbitrary family of (unital) A-algebras. For every finite subset J of I, let E_J denote the tensor product $ \bigotimes_{i \in J} E_i $ of the algebras E_i of index $ i \in J $; let $ e_i $ denote the unit element of E_i and $ e_J = \bigotimes_{i \in J} e_i $ the unit element of E_J; let $ f_{J,i} $ denote the canonical homomorphism $ E_i \to E_J $ for $ i \in J $ (no. 2, Proposition 5). If J, J' are two finite subsets of I such that $ J \subset J' $, a homomorphism $ f_{J'J} : E_J \to E_{J'} $ is canonically derived (no. 2, Proposition 5), by the condition $ f_{J'J} \circ f_{J,i} = f_{J',i} $ for all $ i \in J $. Moreover the uniqueness of $ f_{J'J} $ implies that if J, J', J'' are three finite subsets of I such that $ J \subset J' \subset J'' $, then $ f_{J''J} = f_{J''J'} \circ f_{J'J} $. In other words, $ (E_J, f_{J'J}) $ is a direct system of A-algebras whose indexing set is the right directed set $ \mathcal{F}(I) $ of finite subsets of I.

#### Definition 5 {#alg-iii-s4-def-5 .statement}

*The direct limit E of the direct system* $ (E_J, f_{J'J}) $ *is called the tensor product of the family of A-algebras* $ (E_i)_{i \in I} $.

If I is finite, E is identified with $ \bigotimes_{i \in I} E_i $. By an abuse of notation, E is also denoted by $ \bigotimes_{i \in I} E_i $ even if I is infinite.

For every finite subset J of I, let $ f_J $ denote the canonical homomorphism $ \bigotimes_{i \in J} E_i \to \bigotimes_{i \in I} E_i $ (writing $ f_i $ instead of $ f_{\{i\}} $); if e is the unit element of $ \bigotimes_{i \in I} E_i $, then $ f_J(e_J) = e $ for all $ J \in \mathcal{F}(I) $. It is immediate that if all the algebras E_i are commutative, so is $ \bigotimes_{i \in I} E_i $.

#### Proposition 8 {#alg-iii-s4-prop-8 .statement}

(i) *The homomorphisms* $ f_i : E_i \to E = \bigotimes_{k \in I} E_k $ *are such that for two indices* i, j *such that* $ i \neq j $, $ f_i(x_i) $ *and* $ f_j(x_j) $ *commute in* E *for all* $ x_i \in E_i $ *and* $ x_j \in E_j $; *further,* E *is generated by the union of the subalgebras* $ f_i(E_i) $.

(ii) *Let F be an A-algebra and, for all* $ i \in I $, *let* $ u_i : E_i \to F $ *be an A-algebra homomorphism such that, for* $ i \neq j $, $ u_i(x_i) $ *and* $ u_j(x_j) $ *commute in* F *for all* $ x_i \in E_i $ *and* $ x_j \in E_j $. *Then there exists one and only one A-algebra homomorphism* $ u : E \to F $ *such that* $ u_i = u \circ f_i $ *for all* $ i \in I $.

(i) As, for every finite subset J of I, $ f_i = f_J \circ f_{J,i} $, the first assertion in (i) follows from no. 2, Proposition 5, taking J containing i and j; the second also follows from no. 2, Proposition 5, taking account of the fact that E is the union of the $ f_J(E_J) $ when J runs through $ \mathcal{F}(I) $.

(ii) For every finite subset J of I, it follows from no. 2, Proposition 5 that there exists a unique homomorphism $ u_J : E_J \to F $ such that $ u_J \circ f_{J,i} = u_i $ for all $ i \in J $; it immediately follows from this uniqueness property that, for $ J \subset J' $, $ u_J = u_{J'} \circ f_{J'J} $; in other words, the $ u_J $ form a *direct system* of homomorphisms. Let $ u = \lim \to u_J : E \to F $; then by definition $ u_J = u \circ f_J $ for every finite subset $ J $ of $ I $ and in particular $ u_i = u \circ f_i $ for all $ i \in I $; the uniqueness of $ u $ follows from these relations and the fact that the $ f_i(E_i) $ generate the algebra $ E $.

#### Corollary {#alg-iii-s4-n5-cor-1 .statement}

*Let* $ (E_i)_{i \in I},\ (E'_i)_{i \in I} $ *be two families of* $ A $*-algebras with the same indexing set and, for all* $ i \in I $, *let* $ u_i : E_i \to E'_i $ *be an algebra homomorphism. Then there exists one and only one* $ A $*-algebra homomorphism* $ u : \bigotimes_{i \in I} E_i \to \bigotimes_{i \in I} E'_i $ *such that, for all* $ i \in I $, *the diagram*

$$
\begin{array}{ccc}
E_i & \xrightarrow{u_i} & E'_i \\
| & & | \\
\bigotimes_{i \in I} E_i & \xrightarrow{u} & \bigotimes_{i \in I} E'_i
\end{array}
$$

*is commutative*, $ f_i $ *and* $ f'_i $ *denoting the canonical homomorphisms*.

It suffices to apply Proposition 8 to the homomorphism $ f'_i \circ u_i $.

The homomorphism $ u $ defined in the Corollary to Proposition 8 is denoted by $ \bigotimes_{i \in I} u_i $. If $ J $ is any subset of $ I $, Proposition 8 can be applied to the family $ (f_i)_{i \in J} $ of canonical homomorphisms $ f_i : E_i \to \bigotimes_{i \in I} E_i = E $; a canonical homomorphism $ E_J \to E $ is derived which is also denoted by $ f_J $ and which, when $ J $ is *finite*, coincides with the homomorphism denoted thus above.

Now let $ (x_i)_{i \in I} $ be an element of $ \prod_{i \in I} E_i $ such that the family $ (x_i - e_i)_{i \in I} $ has *finite support* $ H $. It is immediate that, if $ J $ and $ J' $ are two finite subsets of $ I $ containing $ H $, then

$$
f_J((x_i)_{i \in J}) = f_{J'}((x_i)_{i \in J'}).
$$

The common value of the $ f_J((x_i)_{i \in J}) $ for the finite subsets $ J \supset H $ of $ I $ is denoted by $ \bigotimes_{i \in I} x_i $.

#### Proposition 9 {#alg-iii-s4-prop-9 .statement}

*Let* $ (E_i)_{i \in I} $ *be a family of* $ A $*-algebras and for each* $ i \in I $ *let* $ B_i $ *be a basis of* $ E_i $ *such that the unit element* $ e_i $ *belongs to* $ B_i $. *Let* $ B $ *be the set of elements of the form* $ \bigotimes_{i \in I} x_i $, *where* $ (x_i) $ *runs through the set of elements of* $ \prod_{i \in I} B_i $ *such that the family* $ (x_i - e_i) $ *has finite support*. *Then* $ B $ *is a basis of the algebra* $ \bigotimes_{i \in I} E_i $ *and this basis contains the unit element* $ e $.

For every finite subset $ J $ of $ I $, let $ B_J $ be the basis of $ E_J = \bigotimes_{i \in J} E_i $ the tensor product of the bases $ B_i $ for $ i \in J $ (II, § 3, no. 9). It follows immediately from the definitions that $ B $ is the union of the $ f_J(B_J) $ when $ J $ runs through $ \mathcal{F}(I) $ and that $ f_{J',J}(B_J) \subset B_{J'} $ when $ J \subset J' $; hence $ (B_J) $ is a direct system of subsets of the $ E_J $ and $ B = \lim \rightarrow B_J $; the conclusion then follows from II, § 6, no. 2, Corollary to Proposition 5.

The basis $ B $ is also called the *tensor product* of the bases $ B_i $ for $ i \in I $; when the conditions of Proposition 9 are fulfilled, the canonical homomorphisms $ f_J : E_J \to E = \bigotimes_{i \in I} E_i $ are *injective* for every subset $ J $ of $ I $, for if $ B_J $ is the basis of $ E_J $ the tensor product of the $ B_i $ for $ i \in J $, it is immediately verified that the restriction of $ f_J $ to $ B_J $ is injective and maps $ B_J $ onto a subset of $ B $.

### 6. COMMUTATION LEMMAS

#### Lemma 1 {#alg-iii-s4-lem-1 .statement}

*Let $ A $ be a commutative ring, $ E $ an $ A $-algebra, $ (x_i)_{1 \leq i \leq n} $ a finite sequence of elements of $ E $, $ (\lambda_i)_{1 \leq i \leq n} $ a finite sequence of elements of $ A $ and $ y $ an element of $ E $; suppose that*
$$
x_i y = \lambda_i y x_i \quad \text{for } 1 \leq i \leq n.
$$
*Then*
$$
(x_1 x_2 \ldots x_n) y = (\lambda_1 \lambda_2 \ldots \lambda_n) y (x_1 x_2 \ldots x_n).
$$

The lemma being trivial for $ n = 1 $, we argue by induction on $ n \geq 2 $. Now
$$
(x_1 x_2 \ldots x_n) y = (x_1 \ldots x_{n-1})(x_n y)
= (x_1 \ldots x_{n-1})(\lambda_n y x_n) = \lambda_n ((x_1 \ldots x_{n-1}) y) x_n,
$$
which, by the induction hypothesis, is equal to
$$
\lambda_n (\lambda_1 \ldots \lambda_{n-1}) y (x_1 \ldots x_{n-1}) x_n = (\lambda_1 \ldots \lambda_{n-1} \lambda_n) y (x_1 \ldots x_{n-1} x_n),
$$
whence the lemma.

#### Lemma 2 {#alg-iii-s4-lem-2 .statement}

*Let $ A $ be a commutative ring, $ E $ an $ A $-algebra and $ (x_i)_{1 \leq i \leq n} $ and $ (y_i)_{1 \leq i \leq n} $ two finite sequences of $ n $ elements of $ E $; suppose that for $ 1 \leq j \leq i \leq n $,*
$$
x_i y_j = \lambda_{ij} y_j x_i \quad \text{with } \lambda_{ij} \in A.
$$
*Then*
$$
(x_1 x_2 \ldots x_n)(y_1 y_2 \ldots y_n) = \left( \prod_{i > j} \lambda_{ij} \right) (x_1 y_1)(x_2 y_2) \ldots (x_n y_n).
$$

The lemma being trivial for $ n = 1 $, we again argue by induction on $ n $ for $ n \geq 2 $. By virtue of Lemma 1,
$$
(x_1 \ldots x_n)(y_1 \ldots y_n) = x_1 (x_2 \ldots x_n) y_1 (y_2 \ldots y_n)
= \left( \prod_{i > 1} \lambda_{i1} \right) (x_1 y_1)(x_2 \ldots x_n)(y_2 \ldots y_n)
$$
and it then suffices to apply the induction hypothesis to obtain (16).

For every family $ \lambda = (\lambda_{ij}) $ of elements of $ \mathbf{A} $, with $ 1 \leq j < i \leq n $, and for every permutation $ \sigma \in \mathfrak{S}_n $, we write

$$
\varepsilon_\sigma(\lambda) = \prod_{i > j,\ \sigma^{-1}(i) < \sigma^{-1}(j)} \lambda_{ij} = \prod_{i < j,\ \sigma(i) > \sigma(j)} \lambda_{\sigma(i),\ \sigma(j)}.
$$

Observe that, when $ \mathbf{A} = \mathbf{Z} $ and $ \lambda_{ij} = -1 $ for every ordered pair $ (i, j) $ such that $ 1 \leq j < i \leq n $, $ \varepsilon_\sigma(\lambda) $ is just the signature $ \varepsilon_\sigma $ of the permutation $ \sigma $ (I, § 5, no. 7).

#### Lemma 3 {#alg-iii-s4-lem-3 .statement}

*Let $ \mathbf{A} $ be a commutative ring, $ \mathbf{E} $ an $ \mathbf{A} $-algebra, $ (x_i)_{1 \leq i \leq n} $ a finite sequence of elements of $ \mathbf{E} $ and suppose that, for every ordered pair $ (i, j) $ of integers such that $ 1 \leq j < i \leq n $,*

$$
x_i x_j = \lambda_{ij} x_j x_i \quad \text{with } \lambda_{ij} \in \mathbf{A}.
$$

*Then, for every permutation $ \sigma \in \mathfrak{S}_n$,*

$$
x_{\sigma(1)} x_{\sigma(2)} \cdots x_{\sigma(n)} = \varepsilon_\sigma(\lambda) x_1 x_2 \cdots x_n.
$$

The lemma is trivial for $ n = 1 $ and $ n = 2 $; we proceed by induction on $ n $ for $ n \geq 3 $. If $ \sigma(n) = n $, relation (19) follows from the induction hypothesis. Suppose therefore that $ \sigma(n) = k, k \neq n $, and let $ \tau $ be the permutation of $ \{1, n\} $ defined by

$$
\begin{cases}
\tau(i) = i & \text{for } i < k \\
\tau(i) = i + 1 & \text{for } k \leq i < n \\
\tau(n) = k.
\end{cases}
$$

Let $ \pi = \tau^{-1} \circ \sigma $; the permutation $ \pi $ leaves $ n $ fixed; now $ \sigma = \tau \circ \pi $ and therefore, writing $ y_i = x_{\tau(i)},\ y_{\pi(i)} = x_{\sigma(i)} $. If $ i \neq n $ and $ j \neq n $, the relations $ \pi(i) > \pi(j) $ and $ \sigma(i) > \sigma(j) $ are equivalent (since $ \tau $ is a strictly increasing mapping of $ \{1, n-1\} $ into $ \{1, n\} $). For $ i \neq n, j \neq n $ and $ \sigma(i) > \sigma(j) $,

$$
y_{\pi(i)} y_{\pi(j)} = x_{\sigma(i)} x_{\sigma(j)} = \lambda_{\sigma(i),\ \sigma(j)} x_{\sigma(j)} x_{\sigma(i)} = \lambda_{\sigma(i),\ \sigma(j)} y_{\pi(j)} y_{\pi(i)}
$$

whence, by the induction hypothesis (using the fact that $ \pi(n) = n $):

$$
y_{\pi(1)} y_{\pi(2)} \cdots y_{\pi(n)} = \left( \prod_{i < j < n,\ \sigma(i) > \sigma(j)} \lambda_{\sigma(i),\ \sigma(j)} \right) y_1 y_2 \cdots y_n
$$

that is

$$
x_{\sigma(1)} x_{\sigma(2)} \cdots x_{\sigma(n)} = \left( \prod_{i < j < n,\ \sigma(i) > \sigma(j)} \lambda_{\sigma(i),\ \sigma(j)} \right) x_{\tau(1)} \cdots x_{\tau(n)}.
$$

Now

$$
x_{\tau(1)} \cdots x_{\tau(n)} = x_1 \cdots x_{k-1} x_{k+1} \cdots x_n x_k
$$

and this, by Lemma 1, is equal to

$$
\left( \prod_{j > k} \lambda_{jk} \right) x_1 \cdots x_n = \left( \prod_{\sigma(i) > \sigma(n)} \lambda_{\sigma(i),\ \sigma(n)} \right) x_1 \cdots x_n.
$$

Finally, (20) and (21) give

$$
x_{\sigma(1)} \cdots x_{\sigma(n)} = \alpha \cdot x_1 \cdots x_n
$$

with

$$
\alpha = \left( \prod_{i < j < n, \sigma(i) > \sigma(j)} \lambda_{\sigma(i), \sigma(j)} \right) \cdot \left( \prod_{i < n, \sigma(i) > \sigma(n)} \lambda_{\sigma(i), \sigma(n)} \right)
$$
$$
= \prod_{i < j, \sigma(i) > \sigma(j)} \lambda_{\sigma(i), \sigma(j)} = \varepsilon_\sigma(\lambda)
$$

which completes the proof of Lemma 3.

### 7. TENSOR PRODUCT OF GRADED ALGEBRAS RELATIVE TO COMMUTATION FACTORS

#### Definition 6 {#alg-iii-s4-def-6 .statement}

*Let* $(\Delta_i)_{i \in I}$ *be a finite family of commutative monoids written additively. A system of commutation factors over the* $\Delta_i$ *with values in a commutative ring* $\mathbf{A}$ *is a system of mappings* $\varepsilon_{ij}: \Delta_i \times \Delta_j \to \mathbf{A}$, *where* $i \in I$, $j \in I$, $i \neq j$ *satisfying the following conditions*:

(22)
$$
\varepsilon_{ij}(\alpha_i + \alpha'_i, \beta_j) = \varepsilon_{ij}(\alpha_i, \beta_j) \varepsilon_{ij}(\alpha'_i, \beta_j)
$$
(23)
$$
\varepsilon_{ij}(\alpha_i, \beta_j + \beta'_j) = \varepsilon_{ij}(\alpha_i, \beta_j) \varepsilon_{ij}(\alpha_i, \beta'_j)
$$
(24)
$$
\varepsilon_{ij}(\alpha_i, \beta_j) \varepsilon_{ji}(\beta_j, \alpha_i) = 1,
$$

*for all* $\alpha_i, \alpha'_i$ *in* $\Delta_i$, $\beta_j, \beta'_j$ *in* $\Delta_j$.

If I is given a total ordering and the $\Delta_i$ are groups, a system of commutation factors is defined over the $\Delta_i$ by taking for every ordered pair $(i, j)$ such that $i < j$ an arbitrary $\mathbf{Z}$-*bilinear* mapping of $\Delta_i \times \Delta_j$ into the (*multiplicative*) $\mathbf{Z}$-module $\mathbf{A}^*$ of *invertible* elements of the ring $\mathbf{A}$ and then writing

$$
\varepsilon_{ji}(\beta_j, \alpha_i) = (\varepsilon_{ij}(\alpha_i, \beta_j))^{-1}
$$

for $i < j$.

Note that, since the $\varepsilon_{ij}(\alpha_i, \beta_j)$ are invertible,

$$
\varepsilon_{ij}(0, \beta_j) = \varepsilon_{ij}(\alpha_i, 0) = 1,
$$

by virtue of (22) and (23).

#### Example {#alg-iii-s4-n7-exa-1 .statement}

(1) The *trivial* system of commutation factors consists of the $\varepsilon_{ij}$ such that $\varepsilon_{ij}(\alpha_i, \beta_j) = 1$ for all $i, j$, $\alpha_i \in \Delta_i$, $\beta_j \in \Delta_j$.

(2) If we take $\mathbf{A} = \mathbf{Z}$ and $\Delta_i = \mathbf{Z}$ for all $i \in I$, a system of commutation factors is obtained by taking $\varepsilon_{ij}(\alpha_i, \beta_j) = (-1)^{\alpha_i \beta_j}$. Note that this number depends only on the parities of $\alpha_i$ and $\beta_j$ and the $\varepsilon_{ij}$ can therefore be considered as commutation factors when certain of the $\Delta_i$ are equal to $\mathbf{Z}/2\mathbf{Z}$ and the others to $\mathbf{Z}$.

These two examples are the most frequent cases encountered in applications.

#### Proposition 10 {#alg-iii-s4-prop-10 .statement}

Let $ \mathbf{A} $ be a commutative ring and $ (\Delta_i)_{i \in I} $ a finite family of commutative monoids written additively; for each $ i \in I $ let $ E_i $ be a graded $ \mathbf{A} $-algebra of type $ \Delta_i $. Finally, let $ (\varepsilon_{ij}) $ be a system of commutation factors over the $ \Delta_i $ with values in $ \mathbf{A} $. Then there exist a graded $ \mathbf{A} $-algebra $ E $ of type $ \Delta = \prod_{i \in I} \Delta_i $ and for each $ i \in I $ an algebra homomorphism $ h_i : E_i \to E $, with the following properties:

(i) *If $ \phi_i : \Delta_i \to \Delta $ is the canonical homomorphism, then $ h_i $ is a graded homomorphism* (II, § 11, no. 2), in other words, $ h_i(E_i^{\alpha_i}) \subset E^{\phi_i(\alpha_i)} $, where $ (E_i^{\alpha_i}) $ and $ (E^{\alpha}) $ denote the respective graduations on $ E_i $ and $ E $.

(ii) *If $ i \neq j $ and $ x_i $ (resp. $ x_j $) is a homogeneous element of $ E_i $ (resp. $ E_j $) of degree $ \alpha_i \in \Delta_i $ (resp. $ \beta_j \in \Delta_j $), then*

$$
h_i(x_i) h_j(x_j) = \varepsilon_{ij}(\alpha_i, \beta_j) h_j(x_j) h_i(x_i).
$$

(iii) *For every $ \mathbf{A} $-algebra $ F $ and every system of homomorphisms $ f_i : E_i \to F $ satisfying the conditions*

$$
f_i(x_i) f_j(x_j) = \varepsilon_{ij}(\alpha_i, \beta_j) f_j(x_j) f_i(x_i),
$$

*where $ i, j, x_i, x_j, \alpha_i, \beta_j $ are as in (ii), then there exists one and only one algebra homomorphism $ f : E \to F $ such that $ f_i = f \circ h_i $ for all $ i \in I $. Moreover the underlying $ \mathbf{A} $-module of $ E $ is the tensor product $ \bigotimes_{i \in I} E_i $.*

Consider the $ \mathbf{A}\text{-module} $ $ E = \bigotimes_{i \in I} E_i $; it is identified with the direct sum of the submodules $ E^{\alpha} $, where, for each $ \alpha = (\alpha_i) \in \Delta $, we write $ E^{\alpha} = \bigotimes_{i \in I} E_i^{\alpha_i} $; the $ E^{\alpha} $ therefore form a graduation of type $ \Delta $ on the $ \mathbf{A} $-module $ E $. We shall define on $ E $ a *graded $ \mathbf{A} $-algebra* structure of type $ \Delta $. For this let $ I $ be given a total ordering; for every ordered pair of elements $ \alpha = (\alpha_i), \beta = (\beta_i) $ of $ \Delta $, we must first define an $ \mathbf{A} $-bilinear mapping of $ E^{\alpha} \times E^{\beta} $ into $ E^{\alpha + \beta} $, or alternatively an $ \mathbf{A} $-linear mapping $ m_{\alpha \beta} $ of $ E^{\alpha} \otimes_{\mathbf{A}} E^{\beta} $ into $ E^{\alpha + \beta} $. We shall define $ m_{\alpha \beta} $ by the condition

$$
m_{\alpha \beta} \left( \left( \bigotimes_{i \in I} x_i \right) \otimes \left( \bigotimes_{i \in I} y_i \right) \right) = \varepsilon(\alpha, \beta) \bigotimes_{i \in I} (x_i y_i)
$$

for $ x_i \in E_i^{\alpha_i}, y_i \in E_i^{\alpha_i} $, where

$$
\varepsilon(\alpha, \beta) = \prod_{i > j} \varepsilon_{ij}(\alpha_i, \beta_j).
$$

The right hand side of (27) obviously belongs to $ E^{\alpha + \beta} $ and the mapping $ (x_1, \ldots, x_n, y_1, \ldots, y_n) \mapsto \varepsilon(\alpha, \beta) \bigotimes_{i \in I} (x_i y_i) $ is $ \mathbf{A} $-multilinear in the product of the $ E_i^{\alpha_i} $ and the $ E_i^{\beta_i} $ ($ 1 \leq i \leq n $). Then it must be proved that the multiplication thus defined on E is associative; now, if $ \gamma = (\gamma_i) $ is a third element of $ \Delta $ and $ z_i \in E_i^{\gamma_i'} $ for $ 1 \leq i \leq n $, then

$$
\left( \left( \bigotimes_i x_i \right) \left( \bigotimes_i y_i \right) \right) \left( \bigotimes_i z_i \right) = \varepsilon(\alpha + \beta, \gamma) \varepsilon(\alpha, \beta) \bigotimes_i (x_i y_i z_i)
$$

$$
\left( \bigotimes_i x_i \right) \left( \left( \bigotimes_i y_i \right) \left( \bigotimes_i z_i \right) \right) = \varepsilon(\alpha, \beta + \gamma) \varepsilon(\beta, \gamma) \bigotimes_i (x_i y_i z_i)
$$

and it reduces to verifying the identity

$$
\varepsilon(\alpha + \beta, \gamma) \varepsilon(\alpha, \beta) = \varepsilon(\alpha, \beta + \gamma) \varepsilon(\beta, \gamma).
$$

But the latter follows immediately from the relations

$$
\varepsilon(\alpha + \beta, \gamma) = \varepsilon(\alpha, \beta) \varepsilon(\beta, \gamma)
$$
$$
\varepsilon(\alpha, \beta + \gamma) = \varepsilon(\alpha, \beta) \varepsilon(\alpha, \gamma)
$$

themselves immediate consequences of the definition (28) and (22) and (23).

If, for all $ i \in I $, $ e_i $ denotes the unit element of $ E_i $, we know that $ e_i $ is homogeneous of degree 0 (\S 3, no. 1), hence $ e = \bigotimes_{i \in I} e_i $ is homogeneous of degree 0 and it follows from (27), (28) and the relations

$$
\varepsilon_{ij}(\alpha_i, 0) = \varepsilon_{ij}(0, \beta_j) = 1
$$

that $ e $ is unit element of $ E $, which completes the definition on $ E $ of the desired graded A-algebra structure. Then take $ h_i(x_i) = x_i \otimes \bigotimes_{j \neq i} e_j $; to verify that $ h_i(x_i x_i') = h_i(x_i) h_i(x_i') $ for $ x_i, x_i' $ in $ E_i $, attention may be confined to the case where $ x_i $ and $ x_i' $ are homogeneous and then this relation follows immediately from (27) and the relations $ \varepsilon_{ij}(\alpha_i, 0) = \varepsilon_{ij}(0, \beta_j) = 1 $; the same relations and (24) prove also that the $ h_i $ satisfy conditions (i) and (ii) of the statement and that

$$
\bigotimes_{i \in I} x_i = \prod_{i \in I} h_i(x_i)
$$

where the right hand side is the product of the ordered sequence $ (h_i(x_i))_{i \in I} $ in E with the given total ordering on I (I, \S 1, no. 2) (it suffices to argue by induction on the number of $ x_i $ (assumed homogeneous) distinct from the $ e_i $).

It remains to prove condition (iii); note that the mapping

$$
(x_i)_{i \in I} \mapsto \prod_{i \in I} f_i(x_i),
$$

where the right hand side is the product of the ordered sequence $ (f_i(x_i))_{i \in I} $ with the given total ordering on $ I $, is A-multilinear. Then there exists one and only one A-linear mapping $ f : E \to F $ such that

$$
f\left( \bigotimes_{i \in I} x_i \right) = \prod_{i \in I} f_i(x_i).
$$

Clearly $ f(e) $ is the unit element of $ F $ and $ f \circ h_i = f_i $; to verify that $ f $ is an algebra homomorphism, in other words that $ f(x)f(y) = f(xy) $ for $ x, y $ in $ E $, attention may be confined, by linearity, to the case where $ x = \bigotimes_{i \in I} x_i $ and $ y = \bigotimes_{i \in I} y_i $, $ x_i $ (resp. $ y_i $) being homogeneous of degree $ \alpha_i $ (resp. $ \beta_i $) for all $ i \in I $. The relation to be verified then reduces, by (27), to

$$
\left( \prod_{i \in I} f_i(x_i) \right) \left( \prod_{i \in I} f_i(y_i) \right) = \varepsilon(\alpha, \beta) \prod_{i \in I} (f_i(x_i) f_i(y_i)).
$$

But, taking account of relations (26), this is a consequence of Lemma 2 of no. 6.

Clearly the algebra $ E $ and the canonical mapping $ \psi : \bigotimes_{i \in I} E_i \to E $ constitute a solution of the *universal mapping problem* (*Set Theory*, IV, § 3, no. 1), where $ \Sigma $ is the species of A-algebra structure and the $ \alpha $-mappings $ \prod_i f_i $ from $ \prod_i E_i $ to an A-algebra, satisfying conditions (26).

For a fixed total ordering on $ I $, the graded algebra $ E $ defined in the proof of Proposition 10 will be called a *graded tensor $ \varepsilon $-product of type* $ \Delta $ of the family $ (E_i)_{i \in I} $ of graded algebras of type $ \Delta_i $ and will be denoted by $ ^{\varepsilon} \bigotimes_{i \in I} E_i $ (if no confusion can arise over the ordering on $ I $); similarly, the homomorphism $ f : E \to F $ defined in the proof of Proposition 10 will be denoted by $ ^{\varepsilon} \bigotimes_{i \in I} f_i $. The homomorphisms $ h_i $ are called *canonical*. We also write $ ^{\varepsilon} G^{\otimes n} $ when $ I = \{1, n\} $ and all the $ E_i $ are equal to the same algebra $ G $.

#### Remark {#alg-iii-s4-n7-rem-1 .statement}

(1) We recover the tensor product of algebras defined in no. 1 (with moreover the graduation the tensor product of those of its factors) taking $ \varepsilon_{ij}(\alpha_i, \beta_j) = 1 $ for all $ i, j, \alpha_i $ and $ \beta_j $.

(2) Suppose that all the $ \Delta_i $ are equal to $ \mathbf{Z} $ and write $ \varepsilon_{ij}(\alpha_i, \beta_j) = (-1)^{\alpha_i \beta_j} $; the tensor $ \varepsilon $-product $ ^{\varepsilon} \bigotimes_{i \in I} E_i $ corresponding to this system of commutation factors is then called the *skew* tensor product of the graded algebras $ E_i $ of type $ \mathbf{Z} $ and denoted by $ ^{\varepsilon} \bigotimes_{i \in I} E_i $ (or $ E \ ^{\varepsilon} \otimes_A F $ for two algebras, or $ ^{\varepsilon} G^{\otimes n} $ instead of $ ^{\varepsilon} G^{\otimes n} $).

#### Corollary 1 {#alg-iii-s4-prop-10-cor-1 .statement}

In the notation of Proposition 10, suppose further that F is a graded A-algebra of type $ \Delta $ and that each $ f_i $ is a graded algebra homomorphism relative to $ \phi_i : \Delta_i \to \Delta $; then $ f = \varepsilon \bigotimes_i f_i $ is a graded algebra homomorphism.

This follows immediately from the definition of $ f $ and the fact that
$$
\sum_{i \in I} \phi_i(\alpha_i) = (\alpha_i)
$$
by definition of the $ \phi_i $.

It is therefore seen that $(E, \psi)$ is also a solution of another universal mapping problem, where this time $ \Sigma $ is the species of *graded A-algebra* structure *of type* $ \Delta $, the morphisms being graded algebra homomorphisms of type $ \Delta $ and the $ \alpha $-mappings the mappings $ \prod_i f_i $, where, in addition to conditions (26), it is assumed that $ f_i $ is a graded algebra homomorphism relative to $ \phi_i $.

#### Corollary 2 {#alg-iii-s4-prop-10-cor-2 .statement}

*Let* $(E_i)_{i \in I}, (F_i)_{i \in I}$ *be two finite families of* A*-algebras, with* $ E_i $ *and* $ F_i $ *graded of type* $ \Delta_i $ *for all* $ i \in I $. *For each* $ i \in I $, *let* $ g_i : E_i \to F_i $ *be a graded algebra homomorphism of type* $ \Delta_i $. *Then, if* $ h_i : E_i \to \varepsilon \bigotimes_{i \in I} E_i $ *and* $ h'_i : F_i \to \varepsilon \bigotimes_{i \in I} F_i $ *are the canonical homomorphisms, there exists one and only one homomorphism of graded* A*-algebras of type* $ \Delta $, $ g : \varepsilon \bigotimes_{i \in I} E_i \to \varepsilon \bigotimes_{i \in I} F_i $ *such that* $ g \circ h_i = h'_i \circ g_i $ *for all* $ i \in I $. *Also, if each* $ g_i $ *is bijective, so is* $ g $.

It suffices to apply Corollary 1 to $ f_i = h'_i \circ g_i $, noting that conditions (26) then follow from relations (25) applied to the $ h'_i $.

The homomorphism defined in Corollary 2 is also denoted by $ \varepsilon \bigotimes_i g_i $ (if no confusion can arise); if, for each $ i \in I $, $ G_i $ is a third graded A-algebra of type $ \Delta_i $ and $ g'_i : F_i \to G_i $ a graded algebra homomorphism, then
$$
\left( \varepsilon \bigotimes_i g'_i \right) \circ \left( \varepsilon \bigotimes_i g_i \right) = \varepsilon \bigotimes_i (g'_i \circ g_i),
$$
as follows immediately from (30).

In the case of a *skew* tensor product of graded algebras of type $ \mathbf{Z} $, we write $ \varepsilon \bigotimes_i f_i $ instead of $ \varepsilon \bigotimes_i f_i $ for homomorphisms $ f_i : E_i \to F_i $ of graded algebras of type $ \mathbf{Z} $; when $ I = \{1, 2\} $, this homomorphism is also denoted by $ f_1 \varepsilon \otimes f_2 $; when $ I = \{1, n\} $ and all the $ E_i $ (resp. $ F_i $) are equal and all the $ f_i $ equal to the same homomorphism $ f $, we write $ \varepsilon f^{\otimes n} $.

#### Remark {#alg-iii-s4-n7-rem-2 .statement}

In the proof of Proposition 10, a total ordering on $ I $ was used to define an *algebra* structure on the tensor product $ \bigotimes_{i \in I} E_i $ of the A-modules

E_i. If the ordering on I is changed, another multiplicative structure arises on $ \bigotimes_{i \in I} E_i $, but the new algebra thus obtained is canonically *isomorphic* to the above, since both are solutions of the same universal mapping problem. For example, when $ I = \{1, 2\} $, the canonical isomorphism of the algebra $ E_1 \overset{\varepsilon}{\otimes}_A E_2 $ onto the algebra $ E_2 \overset{\varepsilon}{\otimes}_A E_1 $ maps $ x_1 \otimes x_2 $ to $ \varepsilon_{2,1}(\alpha, \beta)x_2 \otimes x_1 $, where $ x_1 $ is homogeneous of degree $ \alpha $ and $ x_2 $ homogeneous of degree $ \beta $.

Let J be a subset of I and, for each $ i \in J $, consider the canonical homomorphism $ h_i : E_i \to \varepsilon \bigotimes_{i \in I} E_i = E $. By virtue of relations (25) a canonical homomorphism $ h : E' = \varepsilon \bigotimes_{i \in J} E_i \to E $ is derived canonically (by Proposition 10) from these homomorphisms, such that, for all $ i \in J $, $ h'_i = h \circ h_i $, $ h'_i $ being the canonical homomorphism $ E_i \to E' $. Taking the total ordering on J induced by that chosen on I, we obtain

$$
h\left( \bigotimes_{i \in J} x_i \right) = \prod_{i \in I} h_i(x_i) = \bigotimes_{i \in I} x'_i
$$

where the middle term is the product of the *ordered sequence* $ (h_i(x_i))_{i \in J} $ and where, in the right hand term, $ x'_i = x_i $ for $ i \in J $, $ x'_i = e_i $ for $ i \notin J $.

#### Proposition 11 {#alg-iii-s4-prop-11 .statement}

("associativity" of the tensor $ \varepsilon $-product). *In the notation of Proposition 10, let* $ (J_\lambda)_{\lambda \in L} $ *be a partition of I and write* $ \Delta'_\lambda = \prod_{i \in J_\lambda} \Delta_i $ *for all* $ \lambda \in L $. *Let* $ E'_\lambda $ *be a graded tensor $ \varepsilon $-product of type* $ \Delta'_\lambda $ *of the family* $ (E_i)_{i \in J_\lambda} $ *for some total ordering chosen on* $ J_\lambda $. *On the other hand, for* $ \lambda, \mu $ *in* $ L $ *and* $ \lambda \neq \mu $, *we write, for* $ \alpha'_\lambda = (\alpha_i)_{i \in J_\lambda} $, $ \beta'_\mu = (\beta_j)_{j \in J_\mu} $,

$$
\varepsilon'_{\lambda \mu}(\alpha'_\lambda, \beta'_\mu) = \prod_{i \in J_\lambda, j \in J_\mu} \varepsilon_{ij}(\alpha_i, \beta_j).
$$

*Then* $ (\varepsilon'_{\lambda \mu}) $ *is a system of commutation factors over the* $ \Delta'_\lambda $ *with values in* $ A $ *and there exists one and only one homomorphism of graded algebras of type* $ \Delta $, $ v : \varepsilon' \bigotimes_{\lambda \in L} E'_\lambda \to \varepsilon \bigotimes_{i \in I} E_i $, *such that*

$$
v\left( \bigotimes_{\lambda \in L} \left( \bigotimes_{i \in J_\lambda} x_i \right) \right) = \bigotimes_{i \in I} x_i
$$

*for all* $ (x_i) \in \prod_{i \in I} E_i $, *provided that the total ordering is taken on I which induces on each* $ J_\lambda $ *the chosen total ordering, and which is such that, for* $ \lambda < \mu $ *in* $ L $, $ i \in J_\lambda $ *and* $ j \in J_\mu $, $ i < j $.

The fact that the $ \varepsilon'_{\lambda \mu} $ form a system of commutation factors is trivial. Let $ h_{i,\lambda} : E_i \to E'_\lambda $, $ h'_\lambda : E'_\lambda \to \varepsilon' \bigotimes_{\lambda \in L} E'_\lambda $ *be the canonical homomorphisms* (for $ \lambda \in L $, $ i \in J_\lambda $) *and write* $ h''_i = h'_\lambda \circ h_{i,\lambda} $; *it will suffice by virtue of the uniqueness of* the solution of a universal mapping problem, to show that $ \varepsilon' \bigotimes_{\lambda \in L} E'_\lambda $ and the $ h''_i $ satisfy the conditions of Proposition 10. Now, for all $ \lambda \in L $, let $ f'_\lambda : E'_\lambda \to F $ be the unique algebra homomorphism such that $ f'_\lambda \circ h_{i,\lambda} = f_i $ for all $ i \in J_\lambda $. We show that, for $ \lambda \neq \mu $, $ \alpha'_\lambda = (\alpha_i)_{i \in J_\lambda}, \beta'_\mu = (\beta_j)_{j \in J_\mu} $,

$$
f'_\lambda(x'_\lambda)f'_\mu(x'_\mu) = \varepsilon'_{\lambda\mu}(\alpha'_\lambda, \beta'_\mu)f'_\mu(x'_\mu)f'_\lambda(x'_\lambda)
$$

for $ x'_\lambda \in E'_\lambda $ (resp. $ x'_\mu \in E'_\mu $) homogeneous of degree $ \alpha'_\lambda $ (resp. $ \beta'_\mu $); it suffices, by linearity, to verify it when $ x'_\mu = \bigotimes_{i \in J_\lambda} x_i, x'_\mu = \bigotimes_{j \in J_\mu} x_j, x_i $ (resp. $ x_j $) being homogeneous of degree $ \alpha_i $ (resp. $ \beta_j $) in $ E_i $ (resp. $ E_j $) for $ i \in J_\lambda, j \in J_\mu $. But this follows from formula (30) which defines the $ f'_\lambda $ and Lemma 3 of no. 6, taking account of hypothesis (26) and definition (32). There is therefore one and only one algebra homomorphism $ f : \varepsilon' \bigotimes_{\lambda \in L} E'_\lambda \to F $ such that $ f \circ h'_\lambda = f'_\lambda $ for all $ \lambda \in L $; whence $ f \circ h''_i = f_i $ for all $ i \in I $ and the uniqueness of $ f $ is trivial.

### 8. TENSOR PRODUCT OF GRADED ALGEBRAS OF THE SAME TYPES

Assuming the hypotheses of no. 7, Proposition 10 hold, suppose further that all the $ \Delta_i $ are equal to the *same commutative monoid* $ \Delta_0 $; we can then consider on the tensor $ \varepsilon $-product $ \varepsilon \bigotimes_{i \in I} E_i $ the *total graduation* of type $ \Delta_0 $, associated with the graduation of type $ \Delta = \Delta_0^I $ on this algebra (II, § 11, no. 1); we shall call $ \varepsilon \bigotimes_{i \in I} E_i $, with this graduation, a *graded tensor $ \varepsilon $-product of type* $ \Delta_0 $ of the family $ (E_i)_{i \in I} $ of graded algebras of type $ \Delta_0 $.

Always preserving the notation of Proposition 10 of no. 7, suppose that $ F $ is also a *graded A-algebra of type* $ \Delta_0 $ and that the $ f_i $ are *homomorphisms of graded algebras of type* $ \Delta_0 $. Then $ f : \varepsilon \bigotimes_{i \in I} E_i \to F $ is also a *homomorphism of graded algebras of type* $ \Delta_0 $: for it follows from formula (30) (no. 7) that if $ x_i $ is homogeneous and of degree $ \alpha_i \in \Delta_0, \bigotimes_{i \in I} x_i $ and $ \prod_{i \in I} f_i(x_i) $ are both homogeneous of degree $ \sum_{i \in I} \alpha_i \in \Delta_0 $.

It can therefore be said that $ \varepsilon \bigotimes_{i \in I} E_i $, with the total graduation of type $ \Delta_0 $, constitutes, together with the canonical mapping $ \psi $, a solution of a third universal mapping problem, where $ \Sigma $ is the species of *graded A-algebra of type* $ \Delta_0 $, the morphisms are homomorphisms of graded algebras of type $ \Delta_0 $ and the $ \alpha $-mappings are the mappings $ \prod_i f_i $, where, in addition to conditions (26) (of no. 7), it is assumed that each $ f_i $ is a homomorphism of graded algebras of type $ \Delta_0 $.

For every subset J of I, the canonical homomorphism $ \varepsilon \bigotimes_{i \in J} E_i \to \varepsilon \bigotimes_{i \in I} E_i $ (no. 7) is, in fact, a homomorphism of graded algebras of type $ \Delta_0 $, as follows immediately from the above.

#### Proposition 12 {#alg-iii-s4-prop-12 .statement}

("associativity" of the tensor $ \varepsilon $-product of graded algebras of the same types). *With the notation of Proposition 10 of no. 7, suppose that all the $ \Delta_i $ are equal to the same monoid $ \Delta_0 $; let $ (J_\lambda)_{\lambda \in L} $ be a partition of I. With the notation of Proposition 11 of no. 7, suppose that the right hand side of formula (32) (no. 7) depends only on the sums $ \alpha''_\lambda = \sum_{i \in J_\lambda} \alpha_i, \beta''_\mu = \sum_{j \in J_\mu} \beta_j $, for every ordered pair $ (\lambda, \mu) $ of distinct indices, all $ \alpha'_\lambda \in \Delta'_\lambda $ and all $ \beta'_\mu \in \Delta'_\mu $; let $ \varepsilon''_{\lambda \mu}(\alpha''_\lambda, \beta''_\mu) $ denote the right hand side of (32). *Then $ (\varepsilon''_{\lambda \mu}) $ is a system of commutation factors over the family $ (\Delta''_\lambda)_{\lambda \in L} $, where $ \Delta''_\lambda = \Delta_0 $ for all $ \lambda \in L $. *If $ E''_\lambda $ is the graded tensor $ \varepsilon $-product of type $ \Delta_0 $ of the family $ (E_i)_{i \in J_\lambda} $, there exists one and only one isomorphism of graded algebras of type $ \Delta_0 $, $ w : \varepsilon'' \bigotimes_{\lambda \in L} E''_\lambda \to \varepsilon \bigotimes_{i \in I} E_i $, such that

$$
w \left( \bigotimes_{\lambda \in L} \left( \bigotimes_{i \in J_\lambda} x_i \right) \right) = \bigotimes_{i \in I} x_i
$$

*provided that total orderings are chosen on the $ J_\lambda $ and on I as described in no. 7, Proposition 11.*

By the hypothesis, for $ \gamma, \delta $ in $ \Delta_0 $, $ \varepsilon''_{\lambda \mu}(\gamma, \delta) = \varepsilon_{i_0 j_0}(\gamma, \delta) $ for some $ i_0 \in J_\lambda $ and some $ j_0 \in J_\mu $, as is seen by considering the elements $ \alpha'_\lambda = (\alpha_i)_{i \in J_\lambda} $ and $ \beta'_\mu = (\beta_j)_{j \in J_\mu} $ such that $ \alpha_{i_0} = \gamma, \alpha_i = 0 $ for $ i \neq i_0 $, $ \beta_{j_0} = \delta, \beta_j = 0 $ for $ j \neq j_0 $; it follows immediately that the $ \varepsilon''_{\lambda \mu} $ form a system of commutation factors. The rest of the proof is then analogous to that of Proposition 11 (no. 7) and is left to the reader.

Note that the additional hypotheses of Proposition 12 are fulfilled when $ \Delta_0 = \mathbf{Z} $ and that $ (\varepsilon_{ij}) $ is, either the trivial system of factors $ (\varepsilon_{ij}(\alpha_i, \beta_j)) = 1 $ for all $ i, j $, or the system of factors defined by $ \varepsilon_{ij}(\alpha_i, \beta_j) = (-1)^{\alpha_i \beta_j} $; in the latter case, the right hand side of formula (32) is equal to $ (-1)^\gamma $, where

$$
\gamma = \sum_{i \in J_\lambda, j \in J_\mu} \alpha_i \beta_j = \left( \sum_{i \in J_\lambda} \alpha_i \right) \left( \sum_{j \in J_\mu} \beta_j \right).
$$

#### Remark {#alg-iii-s4-n8-rem-1 .statement}

(1) Let I be an infinite indexing set and $ \Delta_0 $ a commutative monoid; let $ (\Delta_i)_{i \in I} $ denote the family such that $ \Delta_i = \Delta_0 $ for all $ i $ and suppose given for every ordered pair of distinct indices $ (i, j) $ of I a mapping $ \varepsilon_{ij} : \Delta_i \times \Delta_j \to A $ satisfying conditions (22), (23) and (24) (no. 7); this will also be called a *system of commutation factors over the family* $ (\Delta_i) $. Consider a family $ (E_i)_{i \in I} $ of graded A-algebras of type $ \Delta_0 $; for each finite subset J of I, let $ E_J $ denote a *graded tensor $ \varepsilon $-product of type* $ \Delta_0 $ of the subfamily $ (E_i)_{i \in J} $ (with an arbitrary choice of a total ordering on J). If J, J' are two finite subsets of I such that $ J \subset J' $, a canonical homomorphism of graded algebras of type $ \Delta_0 $, h_{J'J}: E_J \to E_{J'}, has been defined above and the uniqueness properties of these homomorphisms show immediately that if J \subset J' \subset J'' are three finite subsets of I, then h_{J''J} = h_{J'J'} \circ h_{J'J}. Thus there is a direct system (E_J, h_{J'J}) of graded algebras of type $ \Delta_0 $ (\S 3, no. 3), whose indexing set is the right directed set $ \mathfrak{F}(I) $ of finite subsets of I. The graded algebra of type $ \Delta_0 $, the *direct limit* of this direct system (\S 3, no. 3), is called a *graded tensor $ \varepsilon $-product of type* $ \Delta_0 $ of the family $(E_i)_{i \in I}$; it is also denoted by $ \varepsilon \bigotimes_{i \in I} E_i $. When all the $ \Delta_i $ are equal to $ \mathbf{Z} $ and $ \varepsilon_{ij}(a_i, \beta_j) = (-1)^{\alpha_i \beta_j} $, the tensor product $ \varepsilon \bigotimes_{i \in I} E_i $ is also called the *skew* tensor product of the family $(E_i)_{i \in I}$ and is denoted by $ g \bigotimes_{i \in I} E_i $. We leave to the reader the task of formulating and proving the proposition which generalizes Proposition 10 of no. 7 to the case where I is infinite, as Proposition 8 of no. 5 generalizes Proposition 5 of no. 2 to the case where I is infinite. Note that the underlying A-module of $ \varepsilon \bigotimes_{i \in I} E_i $ is the same as that underlying the (non-graded) tensor product of the family $(E_i)_{i \in I}$ of non-graded algebras defined in no. 5.

(2) Let E be a graded A-algebra of type $ \Delta_0 $ (where $ \Delta_0 $ is a commutative monoid) and $ \rho : A \to B $ a ring homomorphism; the graduation on $ \rho^*(E) $ (II, \S 11, no. 5) is identical with the graduation on the graded tensor product $ B \otimes_A E $, where B has the trivial graduation.

### 9. ANTICOMMUTATIVE ALGEBRAS AND ALTERNATING ALGEBRAS

#### Definition 7 {#alg-iii-s4-def-7 .statement}

*A graded A-algebra E of type $ \mathbf{Z} $ is called anticommutative if for all non-zero homogeneous elements x, y of E*

$$
xy = (-1)^{\deg(x)\deg(y)} yx.
$$

*The algebra E is called alternating if it is anticommutative and also $ x^2 = 0 $ for every homogeneous element $ x \in E $ of odd degree.*

#### Remark {#alg-iii-s4-n9-rem-1 .statement}

(1) Let $ E^+ $ be the graded subalgebra of E the direct sum of the $ E_{2n} $ ($ n \in \mathbf{Z} $); it follows from Definition 7 that if E is anticommutative, $ E^+ $ is a *subalgebra contained in the centre of* E (and hence commutative).

(2) Suppose that 2 is not a divisor of 0 in E; then if E is anticommutative E is alternating, since for $ x \in E $ homogeneous and of odd degree, $ x^2 = -x^2 $ by (36), whence $ 2x^2 = 0 $ and $ x^2 = 0 $ by virtue of the hypothesis.

(3) We shall study in detail in \S 7 important examples of alternating algebras.

#### Lemma 4 {#alg-iii-s4-lem-4 .statement}

*Let E be a graded algebra of type $ \mathbf{Z} $ and S a set of homogeneous elements $ \neq 0 $; the set F of elements of E all of whose homogeneous components $ x \neq 0 $ satisfy relation (36) for all $ y \in S $ is a graded subalgebra of E.*

It suffices to note that: (1) if $ x', x'' $ are two homogeneous elements of the same degree $ p $, $ y $ a homogeneous element of degree $ q $ and $ x'y = (-1)^{pq}yx' $, $ x''y = (-1)^{pq}yx'' $, then also $ (x' + x'')y = (-1)^{pq}y(x' + x'') $; (2) if $ x', x'' $ are two homogeneous elements of respective degrees $ p', p'' $, $ y $ a homogeneous element of degree $ q $ and $ x'y = (-1)^{p'q}yx' $, $ x''y = (-1)^{p''q}yx'' $, then
$$
(x'x'')y = (-1)^{(p'+p'')q}y(x'x'').
$$

#### Proposition 13 {#alg-iii-s4-prop-13 .statement}

*Let E be a graded A-algebra of type $ \mathbf{Z} $ and S a generating system of the algebra E consisting of homogeneous elements $ \neq 0 $; for E to be anticommutative (resp. alternating), it is necessary and sufficient that (36) hold for all $ x \in S $ and $ y \in S $ (resp. that this condition hold and further that $ x^2 = 0 $ for all $ x $ homogeneous of odd degree belonging to S).*

We consider first the case of anticommutative algebras. By Lemma 4, the subalgebra F consisting of the elements all of whose homogeneous components $ x \neq 0 $ satisfy (36) for all $ y \in S $, contains all the elements of S and hence $ F = E $. If now $ F' $ is similarly the subalgebra of E consisting of the elements all of whose homogeneous components $ x \neq 0 $ satisfy (36) for every homogeneous element $ y \neq 0 $, it follows from the above that $ F' $ contains all the elements of S and hence $ F' = E $, which completes the proof of the proposition in this case.

To prove the proposition in the case of alternating algebras, it can be assumed that E is already anticommutative; it is then immediate that every homogeneous element of odd degree in E is of the form $ \sum_i z_ix_i $, where $ z_i \in E^+ $ and $ x_i \in S $ is of odd degree (using the fact that $ E^+ $ is contained in the centre of E); it follows that $ \left( \sum_i z_ix_i \right)^2 = \sum_i z_i^2x_i^2 + \sum_{i<j} z_i z_j (x_ix_j + x_jx_i) = 0 $ since $ x_i^2 = 0 $ by hypothesis and $ x_ix_j + x_jx_i = 0 $ by (36).

#### Proposition 14 {#alg-iii-s4-prop-14 .statement}

*Let E and F be two graded A-algebras of type $ \mathbf{Z} $, both anticommutative (resp. alternating). Then the skew tensor product $ E^g \otimes_A F $ (no. 7) is an anticommutative (resp. alternating) algebra.*

A generating system of $ E^g \otimes_A F $ consists of the $ x \otimes y $, where $ x $ (resp. $ y $) is a homogeneous element $ \neq 0 $ of E (resp. F). Consider two such elements $ x \otimes y, x' \otimes y' $, with $ \deg(x) = p, \deg(y) = q, \deg(x') = p', \deg(y') = q' $, so that $ x \otimes y $ is of degree $ p + q $ and $ x' \otimes y' $ of degree $ p' + q' $. Then by definition (no. 7, formula (27)) and by virtue of (36),
$$
\begin{align*}
(x \otimes y)(x' \otimes y') &= (-1)^{qp'}(xx') \otimes (yy') \\
(x' \otimes y')(x \otimes y) &= (-1)^{pq'}(x'x) \otimes (y'y) \\
&= (-1)^{pq'+pp'+qq'}(xx') \otimes (yy')
\end{align*}
$$
and the criterion of Proposition 13 shows that $ E^g \otimes_A F $ is anticommutative since $ pq' + pp' + qq' - qp' \equiv (p + q)(p' + q') $ (mod. 2). If further E and F are alternating and $ p + q $ is odd, one of the numbers $ p, q $ is necessarily odd, hence $ (x \otimes y)^2 = \pm (x^2) \otimes (y^2) = 0 $ and Proposition 13 shows that $ E^g \otimes_A F $ is alternating.

#### Corollary {#alg-iii-s4-n9-cor-1 .statement}

*Let E be an anticommutative* (resp. *alternating*) *graded A-algebra of type $ \mathbf{Z} $. Then for every ring homomorphism $ \rho : A \to B $, the graded B-algebra $ \rho^*(E) $ (no. 8, *Remark 2*) *is anticommutative* (resp. *alternating*).

The ring B with the trivial graduation can be considered as an alternating A-algebra and $ \rho^*(E) = E^g \otimes_A B $, hence Proposition 14 can be applied.

#### Remark {#alg-iii-s4-n9-rem-2 .statement}

Let E be an anticommutative graded A-algebra of type $ \mathbf{Z} $. Then the A-linear mapping of $ E \otimes_A E $ into E defined by multiplication of E ($ \S 1 $, no. 3) is a homomorphism of the graded A-algebra $ E^g \otimes_A E $ into E, for in the notation of Proposition 14, in the algebra E,
$$
(xy)(x'y') = (-1)^{qp'}(xx')(yy').
$$

### Exercises {#alg-iii-s4-exercises}

See the [exercises for § 4](exercises/s4/).
