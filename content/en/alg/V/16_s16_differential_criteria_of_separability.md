---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 16
section_title: Differential criteria of separability
lang: en
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A V.127-A V.137, A V.177-A V.180
pdf_pages: 0241-0251, 0291-0294
extraction: ocr
subsections:
    - "no": 1
      title: 'Extension of derivations : the case of rings'
      page: 127
      pdf_page: 241
    - "no": 2
      title: 'Extension of derivations: the case of fields'
      page: 0
      pdf_page: 242
    - "no": 3
      title: Derivations in fields of characteristic zero
      page: 130
      pdf_page: 244
    - "no": 4
      title: Derivations in separable extensions
      page: 131
      pdf_page: 245
    - "no": 5
      title: The index of a linear mapping
      page: 132
      pdf_page: 246
    - "no": 6
      title: Differential properties of finitely generated extensions
      page: 133
      pdf_page: 247
    - "no": 7
      title: Separating transcendence bases
      page: 136
      pdf_page: 250
statements: 30
exercises: 9
content_sha256: c7d8584db6076196d8d6db626c359cb6ebc98a83d1be313ebe821fe9f6d6d894
---

## § 16. DIFFERENTIAL CRITERIA OF SEPARABILITY

### 1. Extension of derivations : the case of rings

Let K be a commutative ring, A a commutative K-algebra and $ x = (x_i)_{i \in I} $, a family of elements of A. Further, let $ A $ be a derivation of K into an A-module M, in other words (III, p. 553) a Z-linear mapping of K into M satisfying the relation $ \Delta(cc') = c \cdot \Delta(c') + c' \cdot \Delta(c) $ for $ c, c' $ in K. For each $ i \in I $ let $ D_i $ be the partial derivation with respect to $ X_i $ in the polynomial ring $ K[X_i]_{i \in I} $; this is the unique derivation of that ring into itself which is zero on K and on $ X_j $ for $ j \in I - \{i\} $, and takes the value 1 on $ X_i $ (IV, p. 6). For every polynomial $ f = \sum_{a \in N^{(I)}} c_a \cdot X^\alpha $ in $ K[X_i]_{i \in I} $, we denote by $ f^\Delta(x) $ the element $ \sum_{a \in N^{(I)}} x^\alpha \cdot A(c,) $ of M.

#### Proposition 1 {#alg-v-s16-prop-1 .statement}

— Suppose that the family $ x = (x_i)_{i \in I} $, generates the K-algebra A. Let $ (m_i)_{i \in I} $, be a family of elements of M and $ (f_\lambda)_\lambda $, a family of polynomials generating the ideal $ a $ of all polynomials $ f \in K[X_i]_{i \in I} $ such that $ f(x) = 0 $. For a derivation D of A into M to exist such that $ D(c \cdot 1) = \Delta(c) $ for all $ c \in K $ and $ D(x_i) = m_i $ for all $ i \in I $ it is necessary and sufficient that

$$
f_\lambda^\Delta(x) + \sum_{i \in I} D_i f_\lambda(x) \cdot m_i = 0 \quad \text{for all} \quad \lambda \in A .
$$

If this is so, the derivation D is unique and satisfies

$$
D(f(x)) = f^\Delta(x) + \sum_{i \in I} D_i f(x) \cdot m_i \quad \text{for all} \quad f \in K[X_i]_{i \in I}
$$

Put $ E = K[X_i]_{i \in I} $ and write $ \varphi $ for the K-homomorphism of E onto A which maps $ X_i $ to $ x_i $ for all $ i \in I $; we thus have $ \varphi(f) = f(x) $ for all $ f \in E $. We consider M as an E-module by means of the homomorphism $ \varphi : E \to A $ and define a mapping $ D' $ of E into M by $ D'(f) = f^\Delta(x) + \sum_{i \in I} D_i f(x) \cdot m_i $ (note that the family $ (D_i f)_{i \in I} $ has finite support for each $ f \in E $). It is clear that $ D' $ is the unique derivation of E into M extending A and mapping $ X_i $ to $ m_i $ for each $ i \in I $.

Let D be a derivation of A into M such that $ D(c \cdot 1) = \Delta(c) $ for all $ c \in K $ and $ D(x_i) = m_i $ for all $ i \in I $. Then $ D \circ \varphi $ is a derivation of E into M extending A and mapping $ X_i $ to $ m_i $ for all $ i \in I $. We thus have $ D \circ \varphi = D' $, that is, the relation (2) holds. This proves the uniqueness of D ; moreover (1) is a consequence of $ f, (x) = 0 $ and (2).

Conversely assume that (1) holds; in other words, we have $ D'(f_\lambda) = 0 $ for all $ \lambda \in A $. Let $ f \in a $; there exists a family with finite support $ (q_\lambda)_{\lambda \in \Lambda} $ in $ E $ such that $ f = \sum_{\lambda \in \Lambda} q_\lambda \cdot f_\lambda $. We have
$$
D'(f) = \sum_{\lambda \in \Lambda} [f_\lambda(x) \cdot D'(q_\lambda) + q_\lambda(x) \cdot D'(f_\lambda)]
$$
whence $ D'(f) = 0 $ because $ f_\lambda(x) $ and $ D'(f_\lambda) $ are zero for all $ \lambda \in A $. Since $ D' $ vanishes on $ a $, there exists a $ Z $-linear mapping $ D $ of $ A $ into $ M $ such that $ D' = D \circ \varphi $; clearly $ D $ is the required derivation of $ A $ into $ M $.

### 2. Extension of derivations: the case of fields

Let $ K, L $ and $ M $ be fields such that $ K \subset L \subset M $. By Prop. 21 (III, p. 572) we have an exact sequence of vector $ M $-spaces
$$
(\mathrm{E}_{K,L,M}) \quad \Omega_K(L) \otimes_L M \xrightarrow{\alpha} \Omega_K(M) \xrightarrow{\beta} \Omega_L(M) \to 0 ;
$$
the $ M $-linear mappings $ \alpha $ and $ \beta $ are characterized by the relations
$$
(3) \quad \alpha(d_{L/K} x \otimes 1) = d_{M/K} x \quad \text{for } x \in L \\
(4) \quad \beta(d_{M/K} y) = d_{M/L} y \quad \text{for } y \in M
$$

Let $ V $ be a vector $ M $-space, denote by $ D_K(M, V) $ the vector space of $ K $-derivations of $ M $ with values in $ V $ and similarly introduce $ D_K(L, V) $ and $ D_L(M, V) $. By III, p. 571, Diagram (42) and III, p. 572, Diagram (44), we have a commutative diagram of homomorphisms of vector spaces
$$
\begin{array}{ccccccccc}
0 \to \mathrm{Hom}_M(\Omega_L(M), V) & \xrightarrow{\mathrm{Hom}(\beta, 1)} & \mathrm{Hom}_M(\Omega_K(M), V) & \xrightarrow{\mathrm{Hom}(\alpha, 1)} & \mathrm{Hom}_M(\Omega_K(L) \otimes_L M, V) \\
\downarrow & & \downarrow & & \downarrow \\
0 \to \mathrm{Der}_L(M, V) & \xrightarrow{i_V} & \mathrm{Der}_K(M, V) & \xrightarrow{r_V} & \mathrm{Der}_K(L, V),
\end{array}
$$
where the vertical arrows are isomorphisms, $ i_V $ is the canonical injection and $ r_V $ the restriction mapping.

We thus obtain from II, p. 299, Th. 5 and II, p. 301, Prop. 10 the following proposition:

#### Proposition 2 {#alg-v-s16-prop-2 .statement}

— *The following conditions are equivalent*:
a) *The mapping $ \alpha $ is injective*.
b) *Every $ K $-derivation of $ L $ into $ M $ extends to a $ K $-derivation of $ M $ into $ M $*.
c) *Every $ K $-derivation of $ L $ into a vector $ M $-space $ V $ extends to a $ K $-derivation of $ M $ into $ V $*.

#### Proposition 3 {#alg-v-s16-prop-3 .statement}

— *Let $ K $ be a field, $ L $ a pure extension of $ K $ and $ (x_i)_{i \in I} $ a pure basis of $ L $* (V, p. 106, Def. 2).

a) Let $ V $ be a vector space over $ L $, $ A $ a derivation of $ K $ into $ V $ and $ (v_i)_{i \in I} $ a family of elements of $ V $. There exists a unique derivation $ D $ of $ L $ into $ V $, extending $ A $ and such that $ D(x_i) = v_i $ for all $ i \in I $.

b) The vector $ L $-space $ \Omega_K(L) $ of $ K $-differentials of $ L $ has the family $ (dx_i)_{i \in I} $ as basis.

Assertion b) has been proved in IV, p. 23 and Assertion a) follows directly from this.

#### Corollary {#alg-v-s16-n2-cor-1 .statement}

— Let $ P $ be a subfield of $ K $. The canonical mapping $ \alpha $ of $ \Omega_P(K) \otimes_K L $ into $ \Omega_P(L) $ is injective and the family $ (d_{L/P} x_i)_{i \in I} $, is a basis (over $ L $) of a subspace of $ \Omega_P(L) $ supplementary to the image of $ \alpha : \Omega_P(K) \otimes_K L \to \Omega_P(L) $.

Prop. 3, a) shows that every $ P $-derivation of $ K $ into a vector space $ V $ over $ L $ extends to a $ P $-derivation of $ L $ into $ V $; the injectivity of $ \alpha $ then follows by Prop. 2. The second assertion of the corollary follows from the exactness of the sequence $ (\mathbf{E}_{P,K,L}) $ and Prop. 3, b) (taking Formula (4) into account).

#### Proposition 4 {#alg-v-s16-prop-4 .statement}

— Let $ K $ be a field, $ L $ a separable algebraic extension of $ K $ and $ V $ a vector space over $ L $.

a) Every $ K $-derivation of $ L $ into $ V $ is zero.

b) If $ A $ is a derivation of $ K $ into $ V $, there exists a unique derivation $ D $ of $ L $ into $ V $ which extends $ A $.

Let $ D $ be a $ K $-derivation of $ L $ into $ V $. If $ E $ is a subextension of $ L $ of finite degree over $ K $, then the $ K $-algebra $ E $ is etale, and so $ \Omega_K(E) = 0 $ ($ V $, p. 33, Th. 3), whence $ D|_E = 0 $ by the universal property of $ \Omega_K(E) $ (III, p. 569). Since $ L $ is the union of a family of subextensions of finite degree over $ K $, we have $ D = 0 $, whence $ a) $.

Let $ A $ be a derivation of $ K $ into $ V $. If $ D' $ and $ D'' $ are two extensions of $ A $ to a derivation of $ L $ into $ V $, then the difference $ D' - D'' $ is a $ K $-derivation of $ L $ into $ V $; hence it is zero by $ a) $ and so $ D' = D'' $.

It remains to prove the existence of an extension of $ A $. Zorn's Lemma (E, III, p. 20) implies the existence of a maximal extension $ D_0 $ of $ A $ to a derivation defined on a subfield $ L_0 $ of $ L $ containing $ K $.

Let $ x $ be in $ L $ and $ g $ the minimal polynomial of $ x $ over $ L_0 $. Since $ L $ is algebraic and separable over $ K $, $ x $ is algebraic and separable over $ L_0 $ ($ V $, p. 39, Prop. 6 and p. 39, Cor. 2); therefore $ x $ is a simple root of $ g $ ($ V $, p. 39, Prop. 5), whence $ g'(x) \neq 0 $ (IV, p. 17, Prop. 7). If we define $ g^{D_0}(x) $ as in $ V $, p. 127, there exists thus an element $ u $ of $ V $ such that $ g^{D_0}(x) + g'(x) \cdot u = 0 $; by Prop. 1 (V, p. 127) there exists a derivation $ D $ of $ L_0(x) $ into $ V $ extending $ D_0 $ and such that $ D(x) = u $. In view of the maximal character of $ (L_0, D_0) $ we thus have $ L_0(x) = L_0 $, whence $ x \in L_0 $. Since $ x $ was arbitrary we conclude that $ L_0 = L $.

#### Corollary 1 {#alg-v-s16-prop-4-cor-1 .statement}

— We have $ \Omega_K(L) = 0 $ if $ L $ is algebraic and separable over $ K $.

The corollary follows from Prop. 4, a) because the vector $ L $-space $ \Omega_K(L) $ is generated by the image of the canonical $ K $-derivation $ d_{L/K} : L \to \Omega_K(L) $.

#### Corollary 2 {#alg-v-s16-prop-4-cor-2 .statement}

— *If L is an algebraic and separable extension of a field K, the canonical mapping $ \alpha : \Omega_P(K) \otimes_K L \to \Omega_P(L) $ is an isomorphism for every subfield P of K.*

The mapping $ \alpha $ is injective by Prop. 2 (V, p. 128) and Prop. 4, *b*); since $ \Omega_K(L) $ reduces to 0 (Cor. 1) the exactness the sequence $ (E_{P.K.L}) $ implies that $ \alpha $ is surjective.

#### Corollary 3 {#alg-v-s16-prop-4-cor-3 .statement}

— *Let E be an extension of a field K and D a derivation of E into E, mapping K into K. If L is a subextension of E which is algebraic and separable over K, then $ D(L) \subset L $.*

Let A be the derivation of K into L which agrees with D on K. By Prop. 4 (V, p. 129) there exists a derivation D' of L into L extending A. Now we may consider D' and the restriction D'' of D to L as derivations of $ L $ into E ; since they agree on K, we have $ D' = D'' $ by Prop. 4, whence

$$
D(L) = D''(L) = D'(L) \subset L .
$$

#### Remark {#alg-v-s16-n2-rem-1 .statement}

— 1) Later (V, p. 131, Cor. 3 and p. 135, Cor. 2) we shall prove a converse to Cor. 1 of Prop. 4.

2) Every algebraic extension of a prime field is separable (V, p. 37, Cor.). Since every derivation of a prime field is zero, every derivation of an algebraic extension of a prime field is zero (Prop. 4).

### 3. Derivations in fields of characteristic zero

#### Theorem 1 {#alg-v-s16-thm-1 .statement}

— *Let K be a field of characteristic 0, L an extension of K and V a vector space over L. Let A be a derivation of K into V, $ (x_i)_{i \in I} $, a transcendence basis of L over K and $ (u_i)_{i \in I} $, a family of elements of V. Then there exists a unique derivation D of L into V extending A and such that $ D(x_i) = u_i $ for all $ i \in I $.*

Put $ E = K(x_i)_{i \in I} $; Prop. 3 (V, p. 128) shows that A extends to a unique derivation $ D_0 $ of E into V such that $ D_0(x_i) = u_i $ for all $ i \in I $. The field $ L $ is an algebraic extension of E and since L is of characteristic 0, L is separable over E (V, p. 37, Cor.). Therefore (V, p. 129, Prop. 4) $ D_0 $ extends to a unique derivation D of $ L $ into V.

#### Corollary 1 {#alg-v-s16-thm-1-cor-1 .statement}

— *Every derivation of K into V extends to a derivation of L into V*

#### Corollary 2 {#alg-v-s16-thm-1-cor-2 .statement}

— *Let E be a subextension of L and U the vector sub-L-space of $ \Omega_K(L) $ generated by the differentials of elements of E. For an element x to be algebraic over E it is necessary and sufficient that $ dx \in U $.*

For each $ y \in L $ let D(y) be the residue class of $ dy $ mod U. Then D is an E-derivation of L into $ \Omega_K(L)/U $. Since K is of characteristic 0, every algebraic extension of E is separable (V, p. 37, Cor.) ; if $ x \in L $ is algebraic over E, we have $ Dx = 0 $ by Prop. 4 (V, p. 129), that is, $ dx \in U $.

If $ x \in L $ is transcendental over $ E $, there exists an E-derivation $ A $ of $ E(x) $ into $ L $ such that $ \Delta(x) = 1 $ ($ V $, p. 128, Prop. 3); by Th. 1, $ A $ extends to an E-derivation D of $ L $ into L. Let $ \varphi $ be the linear form on $ \Omega_K(L) $ such that $ D = \varphi \circ d $; we have $ \varphi(dy) = 0 $ for $ y \in E $ and $ \varphi(x) = 1 $, whence $ dx \notin U $.

#### Corollary 3 {#alg-v-s16-thm-1-cor-3 .statement}

— *For an element x of L to be algebraic over K it is necessary and sufficient that $ dx = 0 $ in $ \Omega_K(L) $. In particular, for L to be an algebraic extension of K it is necessary and sufficient that $ \Omega_K(L) = 0 $.
This follows immediately from Cor. 2 on taking $ E = K $.

#### Corollary 4 {#alg-v-s16-thm-1-cor-4 .statement}

— *Let K, L and M be fields of characteristic 0 such that $ K \subset L \subset M $: then the canonical mapping $ a : \Omega_K(L) \otimes_L M \to \Omega_K(M) $ is injective.
This follows at once from Cor. 1 and $ V $, p. 128, Prop. 2.

#### Theorem 2 {#alg-v-s16-thm-2 .statement}

— *Let K be a field of characteristic 0, L an extension of K and $ (x_i)_{i \in I} $, a family of elements of L.
a) For $ (x_i)_{i \in I} $, to be algebraically free over K it is necessary and sufficient that the differentials $ dx_i $ (for $ i \in I $) in $ \Omega_K(L) $ should be linearly free over L.
b) For L to be algebraic over $ K(x_i)_{i \in I} $ it is necessary and sufficient that the differentials $ dx_i $, for $ i \in I $ generate the vector space $ \Omega_K(L) $ over L.
c) For $ (x_i)_{i \in I} $ to be a transcendence basis of L over K, it is necessary and sufficient that the family $ (dx_i)_{i \in I} $ should be a basis of $ \Omega_K(L) $ over L.
For every $ i \in I $ let $ E_i $ be the subfield $ K(x_j)_{j \in I, j \neq i} $ of L. For the family $ (x_i)_{i \in I} $, to be algebraically free over K it is necessary and sufficient ($ V $, p. 108, Prop. 5) that $ x_i $ should be transcendental over $ E_i $ for each $ i \in I $. By Cor. 2 of Th. 1 this means that for each $ i \in I $ the differential $ dx_i $ is not a linear combination with coefficients in L of the differentials $ dx_j $ with $ j \neq i $ in I; this latter condition just means that the family $ (dx_i)_{i \in I} $ is free over L, whence a).
Assertion b) follows at once from Cor. 2 of Th. 1 and c) is a consequence of a) and b).

#### Corollary {#alg-v-s16-n3-cor-1 .statement}

— *We have $ [\Omega_K(L) : L] = \operatorname{tr} \cdot \deg_K L $ when K is of characteristic 0.

### 4. Derivations in separable extensions

We have seen ($ V $, p. 122, Th. 1) that every extension $ L $ of a field $ K $ of characteristic 0 is separable; moreover, every derivation of K into a vector space over $ L $ extends then to a derivation of $ L $ ($ V $, p. 130, Cor. 1). More generally we have the following statement:

#### Theorem 3 {#alg-v-s16-thm-3 .statement}

— *Let K be a field and L an extension of K. For L to be separable over K it is necessary and sufficient that every derivation of K into a vector L-space should extend to a derivation of L.
We may assume that K has characteristic $ \neq 0 $. Suppose first that L is separable over K. Let $ V $ be a vector space over L and $ A $ a derivation of K into $ V $. By Mac

Lane's criterion (V, p. 124, Remark), the fields $ L^p $ and $ K $ are linearly disjoint over $ K^p $. Since $ A $ is a $ K^p $-linear mapping of $ K $ into $ V $, it extends in a unique way to an $ L^p $-linear mapping $ A' $ of $ K[L^p] = K(L^p) $ into $ V $. It is clear that $ A' $ is a derivation of $ K(L^p) $ into $ V $ which vanishes on $ L^p $; thus it extends (V, p. 103, Cor. 3) to a derivation of $ L $ into $ V $.

Conversely, suppose that every derivation of $ K $ with values in $ L $ extends to a derivation of $ L $ into $ L $. Let $ B $ be a p-basis of $ K $ (V, p. 99) and let $ A $ be the set of families $ (\alpha_h)_{h \in R} $ with finite support consisting of integers between $ () $ and $ p - 1 $. For each $ b \in B $ there exists a derivation $ \Delta_b $ of $ K $ into $ K $ characterized by $ \Delta_b(b') = \delta_{bb'} $ (Kronecker symbol) for each $ b' \in B $ (V, p. 103). By hypothesis there exists for each $ b \in B $ a derivation $ D_b $ of $ L $ into $ L $ extending $ \Delta_b $. We have $ D_b(b') = \delta_{bb'} $ for $ b, b' $ in $ B $, which proves that in $ \Omega_{1/p}(L) $ the differentials $ db $ (for $ b \in B $) are linearly independent over $ L $. Therefore (V, p 102, Th. 1), $ B $ is p-free over $ L^p $. It follows (V, p. 98, Prop. 1 and p. 124, Remark) that the extension $ L $ of $ K $ is separable.

#### Corollary {#alg-v-s16-n4-cor-1 .statement}

— *If $ L $ is a separable extension of $ K $, the canonical mapping $ \alpha_p : \Omega_p(K) \otimes_K L \to \Omega_p(L) $ is injective for every subfield $ P $ of $ K $. Conversely, if there exists a perfect subfield $ P $ of $ K $ (for example the prime subfield of $ K $) such that the mapping $ \alpha_p $ is injective, then $ L $ is separable over $ K $.*

The first assertion follows from Prop. 2 (V, p. 128) and Th. 3. Conversely, let $ P $ be a perfect subfield of $ K $; we have $ P = P^p \subset K^p $, hence every derivation of $ K $ into a vector $ L $-space is a $ P $-derivation; the second assertion of the corollary now follows from Cor. 2 (V, p. 130) and Th. 3.

### 5. The index of a linear mapping

Let $ L $ be a field $ ^1 $, let $ U $ and $ V $ be two vector spaces $ ^2 $ over $ L $ and $ f : U \to V $ an $ L $-linear mapping; $ f $ is said to have *finite index* if the kernel $ N $ and cokernel $ C $ of $ f $ have finite dimension, and the integer

$$
\chi(f) = [C : L] - [N : L]
$$

is called the *index* of $ f $.

#### Lemma 1 {#alg-v-s16-lem-1 .statement}

— *Let $ U $ and $ V $ be two vector spaces of finite dimension over a field $ L $. Every linear mapping $ f : U \to V $ possesses an index equal to $ [V : L] - [U : L] $.*

Let $ N $ be the kernel, $ I $ the image and $ C $ the cokernel of $ f $. We have $ C = V/I $ and $ I $ is isomorphic to $ U/N $; thus we have $ [U : L] = [N : L] + [I : L] $ and $ [V : L] = [C : L] + [I : L] $, whence the result.

$ ^1 $ Not necessarily commutative.
$ ^2 $ On the left.

#### Lemma 2 {#alg-v-s16-lem-2 .statement}

— Let $ f : U \to V $ and $ g : V \to W $ be two L-linear mappings. Iff and g each have an index, the same is true of $ g \circ f $ and we have

$$
\chi(g \circ f) = \chi(f) + \chi(g).
$$

Put $ h = g \circ f $, and denote by N, N', N'' the kernels off, g, h respectively and by C, C', C'' their cokernels. We have $ N \subset N'' \subset U $ and $ f(N'') = f(U) \cap N' $; hence there exists a linear mapping $ \bar{f} : N'' \to N' $ agreeing with f on N'' and with kernel N. The canonical mapping $ \pi $ of V onto $ C = V / f(U) $ induces a mapping $ \pi' $ of N' into C whose kernel is $ f(U) \cap N' = \bar{f}(N'') $. By passage to quotients g defines a mapping $ \bar{g} $ of $ C = V/f(U) $ into $ C'' = W/g(f(U)) $ whose kernel is clearly $ (N' + f(U))/f(U) = \pi'(N') $. Finally the canonical mapping $ \rho $ of $ C'' = W/g(f(U)) $ onto $ C' = W/g(V) $ has the kernel $ g(V)/g(f(U)) = \bar{g}(C) $. To sum up, we have established the exactness of the sequence

$$
0 \to N \xrightarrow{i} N'' \xrightarrow{\bar{f}} N' \xrightarrow{\pi'} C \xrightarrow{\bar{g}} C'' \xrightarrow{\rho} C' \to 0
$$

(where i is the canonical injection of N in N").

![Diagram showing the relationships between N, N', N'', U, V, W, C, C', C'', with arrows indicating mappings and kernels](../images/fig_1.png)

Fig. 1

By hypothesis N, N', C and C' are of finite dimension; hence the same is true of N'' and C. By Cor. 2 (II, p. 295) we then have

$$
[N : L] - [N'' : L] + [N' : L] - [C : L] + [C'' : L] - [C' : L] = 0
$$

whence $ \chi(h) = \chi(f) + \chi(g) $.

### 6. Differential properties of finitely generated extensions

Theorem 4. — Let P be a perfect field, L an extension of P and K a subextension of L; we suppose that L is a finitely generated extension of K. Then the canonical L-linear mapping $ a : \Omega_p(K) \otimes_K L \to \Omega_p(L) $ has index equal to the transcendence degree of L over K.

If $ E $ and $ F $ are two subextensions of $ L $ such that $ E \subset F $, we denote by $ \alpha(F/E) $ the canonical $ F $-linear mapping of $ \Omega_p(E) \otimes_E F $ into $ \Omega_p(F) $ and when it is defined, the index of $ \alpha(F/E) $ will be written $ d(F/E) $. If $ E, F $ and $ G $ are three subextensions of $ L $ such that $ E \subset F \subset G $, we have a commutative diagram

$$
\begin{array}{ccc}
\Omega_p(F) \otimes_F G & \xrightarrow{\alpha(G/F)} & \Omega_p(G) \\
\uparrow \alpha(F/E) \otimes_F \mathrm{Id}_G & & \uparrow \alpha(G/E) \\
(\Omega_p(E) \otimes_E F) \otimes_F G & \xrightarrow{\beta} & \Omega_p(E) \otimes_E G
\end{array}
$$

where $ \beta $ is the canonical isomorphism defined in Prop. 2 (II, p. 278). Since the index is clearly invariant under extension by scalars and the index of an isomorphism is zero, Lemma 2 ($ V $, p. 133) shows that the index $ d(G/E) $ is defined when $ d(F/E) $ and $ d(G/F) $ are and then

$$
d(G/E) = d(G/F) + d(F/E).
$$

Since $ L $ is a finitely generated extension of $ K $, Formula (5) and the Cor. of $ V $, p. 111 shows that it is enough to consider the case where $ x $ exists such that $ L = K(x) $; further if $ x $ is algebraic over $ K $, there exists a power $ q $ of the characteristic exponent of $ L $ such that $ x^q $ is separable algebraic over $ K $ ($ V $, p. 44, Prop. 13). So it is enough to establish the equality $ d(L/K) = \operatorname{tr} . \deg_K L $ in the three special cases below:

$ a) $ $ x $ is transcendental over $ K $: then $ a $ is injective and its cokernel is of rank 1 over $ L $ ($ V $, p. 129, Cor.) ; so we have $ d(L/K) = 1 $ and also $ \operatorname{tr} . \deg_K L = 1 $.

$ b) $ $ x $ is separable algebraic over $ K $: then $ a $ is bijective ($ V $, p. 130, Cor. 2), whence $ d(L/K) = 0 $; clearly also $ \operatorname{tr} . \deg_K L = 0 $.

$ c) $ *The field $ L $ is of characteristic $ p \neq 0 $, $ x \notin K $ and $ x^p = a $ is in $ K $*: the cokernel $ C $ of $ a $ is isomorphic to $ \Omega_K(L) $, and since $ \{ x \} $ is a $ p $-basis of $ L $ over $ K $, the space $ C $ is of dimension 1 over $ L $ ($ V $, p. 102, Th. 1). Since $ a $ is a $ p $-th power in $ L $, we have $ d_{L/pa} = 0 $ and the kernel of $ a $ contains the subspace $ R $ of $ U = \Omega_p(K) \otimes_K L $ generated by $ d_{K/pa} \otimes 1 $. For each $ y \in K $ let $ \Delta(y) $ be the residue class of $ d_{K/p}y \otimes 1 $ mod $ R $; then $ A $ is a $ P $-derivation of $ K $ into $ U/R $ such that $ \Delta(a) = 0 $. Prop. 5 ($ V $, p. 101) shows that $ A $ extends to a $ P $-derivation $ D $ of $ L $ into $ U/R $. Hence there exists an $ L $-linear mapping $ \beta : \Omega_p(L) \to U/R $ such that $ D = \beta \circ d_{L/P} $ and $ \beta \circ a $ is the canonical mapping of $ U $ onto $ U/R $. This proves $ R $ to be the kernel of $ a $. Since $ P $ is perfect, we have $ P(K^P) = K^p $, whence $ a \notin P(K^P) $ and finally $ d_{K/pa} \neq 0 $ ($ V $, p. 103, Prop. 6). The kernel and cokernel of $ a $ are thus of dimension 1, whence $ d(L/K) = 0 $, and we also have $ \operatorname{tr} . \deg_K L = 0 $.

#### Corollary 1 {#alg-v-s16-lem-2-cor-1 .statement}

— *Let $ L $ be a finitely generated extension of a field $ K $ of transcendence degree $ s $. The vector space $ \Omega_K(L) $ is of dimension $ \geq s $ over $ L $, with equality if and only if $ L $ is separable over $ K $.*

Let P be the prime subfield of K. Let N be the kernel of α, then by exactness of the sequence $ (\mathbf{E}_{P,K,L}) $ (V, p. 128) and Th. 4, we have $[ \Omega_K(L) : L ] = s + [N : L]$; by V, p. 132, Cor., the extension L of K is separable if and only if $ N = 0 $. The corollary now follows.

#### Corollary 2 {#alg-v-s16-lem-2-cor-2 .statement}

— *Let L be a finitely generated extension of a field K. For L to be algebraic and separable over K it is necessary and sufficient that $ \Omega_K(L) = 0 $.* This follows immediately from Cor. 1.

#### Corollary 3 {#alg-v-s16-lem-2-cor-3 .statement}

— *Let K be a field of characteristic $ p \neq 0 $ and L a finitely generated extension of K of transcendence degree s. If $[K : K^p]$ is finite, the same is true of $[L : L^p]$ and we have $[L : L^p] = p^s$. $[K : K^p]$.* Let P be the prime subfield of K. If $[K : K^p]$ is finite, then the vector space $ \Omega_P(K) = \Omega_{K^p}(K) $ is of finite dimension m over K, and we have $[K : K^p] = p^m$ (V, p. 103, Th. 2); the vector space $ \Omega_P(K) \otimes_K L $ is then of finite dimension m over L. Further, since K is of finite degree over $ K^p $, the field $ K(L^p) $ is of finite degree over $ K^p(L^p) = L^p $; since the field L is a finitely generated extension of K and is algebraic over $ K(L^p) $, it is an extension of finite degree of $ K(L^p) $ (V, p. 18, Th. 2); we thus conclude that L is of finite degree over $ L^p $ (V, p. 10, Th. 1). Then $ \Omega_P(L) $ is a vector space of finite dimension n over L and we have $[L : L^p] = p^n$ (V, p. 103, Th. 2). By Lemma 1 (V, p. 132) the L-linear mapping $ \alpha : \Omega_P(K) \otimes_K L \to \Omega_P(L) $ therefore has index $ n - m $, whence $ n - m = s $ by Th. 4 (V, p. 133) and $ p^n = p^s \cdot p^m $.

#### Remark {#alg-v-s16-n6-rem-1 .statement}

— 1) Let K be a field of characteristic $ p \neq 0 $ and L an extension of K. We have $ \Omega_K(L) = 0 $ if and only $ L = K(L^p) $ (V, p. 103, Prop. 6). Therefore if L is finitely generated over K, then it is an algebraic and separable extension if and only if we have $ L = K(L^p) $. When L is not finitely generated over K, this result no longer holds generally as is shown by the case where L is the perfect closure of K.

2) Let K be a field, $ F_1, \ldots, F_m $ polynomials in $ K[X_1, \ldots, X_n] $ and L an extension of K generated by the elements $ x_1, \ldots, x_n $. Suppose that the polynomials $ F_1, \ldots, F_m $ generate the ideal of $ K[X_1, \ldots, X_n] $ consisting of all polynomials F such that $ F(x_1, \ldots, x_n) = 0 $. From Prop. 1 (V, p. 127) and the universal property of the module of differentials (III, p. 569) we easily deduce the following result: the vector space $ \Omega_K(L) $ over L is generated by $ dx_1, \ldots, dx_n $; we have the relations

$$
\sum_{i=1}^n D_i F_j(x_1, \ldots, x_n) \cdot dx_i = 0 \quad \text{(for } 1 \leq j \leq m \text{)} ;
$$

finally if $ u_1, \ldots, u_n $ are elements of L such that $ \sum_{i=1}^n u_i \cdot dx_i = 0 $, there exist elements $ v_1, \ldots, v_m $ of L such that $ u_i = \sum_{j=1}^m D_i F_j(x_1, \ldots, x_n) \ v_j $ for $ 1 \leq i \leq n $. Let us denote by r the rank of the matrix $ (D_i F_j(x_1, \ldots, x_n)) $ with n rows and m columns; let s be the transcendence degree of $ L $ over $ K $. Then we have $[ \Omega_K(L) : L ] = n - r $. Therefore the extension $ L $ of $ K $ is separable if and only if $ r + s = n $ (Cor. 1). and it is algebraic and separable if and only if $ r = n $ (Cor. 2).

### 7. Separating transcendence bases

#### Definition 1 {#alg-v-s16-def-1 .statement}

*Let $ L $ be an extension of a field $ K $. A transcendence basis $ B $ of $ L $ over $ K $ is said to be separating if the algebraic extension $ L $ of $ K(B) $ is separable.*

If $ K $ has characteristic 0, every transcendence basis of $ L $ over $ K $ is separating because every algebraic extension of a field of characteristic 0 is separable ($ V $, p. 37, Cor.). If an extension admits a separating transcendence basis, it is separable ($ V $, p. 121, Prop. 6 and p. 122, Prop. 9). The following theorem shows that every *finitely generated* separable extension admits a separating transcendence basis; this restriction is essential ($ V $, p. 177, Ex. 1).

#### Theorem 5 {#alg-v-s16-thm-5 .statement}

*Let $ K $ be a field, $ L $ an extension of $ K $ and $ (x_i)_{i \in I} $, a family of elements of $ L $. If the family $ (x_i)_{i \in I} $, is a separating transcendence basis of $ L $ over $ K $, then the family $ (dx_i)_{i \in I} $, is a basis of the vector space $ \Omega_K(L) $ over $ L $. The converse holds if $ L $ is a finitely generated separable extension of $ K $.

Put $ M = K(x_i)_{i \in I} $, and denote by $ \alpha $ the canonical mapping of $ \Omega_K(M) \otimes_M L $ into $ \Omega_K(L) $. If $ (x_i)_{i \in I} $ is a separating transcendence basis of $ L $ over $ K $, the family $ (d_{M/K} x_i)_{i \in I} $, is a basis of the vector $ M $-space $ \Omega_K(M) $ ($ V $, p. 128, Prop. 3) and $ \alpha $ is an isomorphism of vector $ L $-spaces since $ L $ is algebraic and separable over $ M $ ($ V $, p. 130, Cor. 2). Since $ \alpha(d_{M/K} x_i \otimes 1) = d_{L/K} x_i $, the family $ (d_{L/K} x_i)_{i \in I} $ is thus a basis of $ \Omega_K(L) $ over $ L $.

Conversely, suppose that $ L $ is a separable finitely generated extension of $ K $ and that the family $ (d_{L/K} x_i)_{i \in I} $ is a basis of the vector space $ \Omega_K(L) $ over $ L $. By Cor. 1 of $ V $, p. 134, the transcendence degree of $ L $ over $ K $ is equal to the dimension of $ \Omega_K(L) $ over $ L $, hence to the cardinal of $ I $. From the exact sequence $ (E_{K,M,L}) $ ($ V $, p. 128) we have $ \Omega_M(L) = 0 $; since $ L $ is a finitely generated extension of $ M $, Cor. 2 of $ V $, p. 135 shows that $ L $ is algebraic and separable over $ M = K(x_i)_{i \in I} $; since the transcendence degree of $ L $ over $ K $ is finite and equal to the cardinal of $ I $, the family $ (x_i)_{i \in I} $ is a transcendence basis of $ L $ over $ K $ ($ V $, p. 110, Cor. 1).

#### Corollary {#alg-v-s16-n7-cor-1 .statement}

*Let $ L $ be a separable finitely generated extension of $ K $ and let $ S $ be a subset of $ L $ such that $ L = K(S) $. Then there exists a separating transcendence basis $ B $ of $ L $ over $ K $, contained in $ S $.

Since $ \Omega_K(L) $ is generated by the differentials of the elements of $ S $, there exist $ s $ elements $ x_1, \ldots, x_s $ of $ S $ such that $ (dx_1, \ldots, dx_s) $ is a basis of $ \Omega_K(L) $ over $ L $. Now it suffices to apply Th. 5.

#### Remark {#alg-v-s16-n7-rem-1 .statement}

— Let $ L $ be a separable finitely generated extension of a field $ K $ of characteristic $ p \neq 0 $; there may exist transcendence bases of $ L $ which are not separating. It is enough to observe that $ \{X^p\} $ is a transcendence basis of $ K(X) $ but $ K(X) $ is a p-radical extension of degree $ p $ of $ K(X^p) $.

#### Proposition 5 {#alg-v-s16-prop-5 .statement}

— *Let L and M be two extensions of a field K contained in a given extension and algebraically disjoint over K. If M is separable over K, then L(M) is separable over L.*

It is enough to show that for every finite subset S of M, $ L(S) $ is separable over L (V, p. 122, Prop. 8). Let S be a finite subset of M. Since the field $ K(S) $ is separable over K, it has a separating transcendence basis B (Cor. of Th. 5). Since L and M are algebraically disjoint over K, B is a transcendence basis of $ L(B) $ over L (V, p. 113, Prop. 12). Further, every element of S is algebraic and separable over $ K(B) $, hence over $ L(B) $ (V, p. 39, Cor. 2). We deduce (V, p. 39, Prop. 6) that $ L(S) = L(B)(S) $ is algebraic and separable over $ L(B) $, hence $ L(S) $, is separable over L.

#### Corollary {#alg-v-s16-n7-cor-2 .statement}

— *If L and M are separable extensions, algebraically disjoint over K, then the field $ K(L \cup M) $ is separable over K.*

For $ K(L \cup M) = L(M) $ is separable over L by Prop. 5 (because M is separable over K) and L is separable over K, whence the corollary (V, p. 122, Prop. 9).

The hypothesis that the extensions L and M are algebraically disjoint is indispensable in Prop. 5 and its corollary. For let K be an imperfect field of characteristic $ p \neq 0 $ and E an extension of the form $ K(x, a) $ with x transcendental over K and a p-radical of height 1 over K ; put $ L = K(x) $ and $ M = K(x + a) $. Then $ x + a $ is transcendental over K (if not, $ x = (x + a) - a $ would be algebraic over K) and the fields L and M are separable over K. However, $ K(L \cup M) = K(x, a) $ is p-radical of degree $ p $ over $ L = K(x) $ and is not separable over L, nor over K.

### Exercises {#alg-v-s16-exercises}

See the [exercises for § 16](exercises/s16/).
