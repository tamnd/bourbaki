---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 14
section_title: Transcendental extensions
lang: en
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A V.106-A V.118, A V.171-A V.175
pdf_pages: 0220-0232, 0285-0289
extraction: ocr
subsections:
    - "no": 1
      title: Algebraically free families. Pure extensions
      page: 106
      pdf_page: 220
    - "no": 2
      title: Transcendence bases
      page: 107
      pdf_page: 221
    - "no": 3
      title: The transcendence degree of an extension
      page: 110
      pdf_page: 224
    - "no": 4
      title: Extension of isomorphisms
      page: 111
      pdf_page: 225
    - "no": 5
      title: Algebraically disjoint extensions
      page: 112
      pdf_page: 226
    - "no": 6
      title: Algebraically free families of extensions
      page: 115
      pdf_page: 229
    - "no": 7
      title: Finitely generated extensions
      page: 117
      pdf_page: 231
statements: 49
exercises: 20
content_sha256: 02d06e928820ce550a2909d158a548fc78ae258e1f5e3e0ab01d1c328bcea79e
---

## § 14. TRANSCENDENTAL EXTENSIONS

### 1. Algebraically free families. Pure extensions

Let us recall (IV, p. 4) the following definition:

#### Definition 1 {#alg-v-s14-def-1 .statement}

*Let E be an extension of a field K; a family $ \mathbf{x} = (x_i)_{i \in I} $ of elements of E is said to be algebraically free over K if the monomials $ \mathbf{x}^a = \prod_{i \in I} x_i^{a_i} $ with respect to the $ x_i $ (for $ a = (\alpha_i)_{i \in I} $, in $ \mathbf{N}^{(1)} $) are linearly independent over K. In the contrary case the family is said to be algebraically related over K.*

Definition 1 may also be expressed as follows:

#### Proposition 1 {#alg-v-s14-prop-1 .statement}

*For a family $ (x_i)_{i \in I} $ of elements of an extension E of a field K to be algebraically free over K it is necessary and sufficient for the relation $ f((x_i)) = 0 $, where $ f $ is a polynomial in $ K[X_i]_{i \in I} $, to imply $ f = 0 $.*

#### Definition 2 {#alg-v-s14-def-2 .statement}

*Let E be an extension of a field K. A family $ (x_i)_{i \in I} $ of elements of E is called a pure basis of E (over K) if it is algebraically free and $ E = K(x_i)_{i \in I} $. The extension E of K is also called pure if it possesses a pure basis.*

The empty family is algebraically free, hence K is a pure extension of itself. With the notation of Def. 2, every element $ x_i $ is transcendental over K; if $ I $ is non-empty, E is thus a transcendental extension of K.

#### Proposition 2 {#alg-v-s14-prop-2 .statement}

*Let E and $ E' $ be two fields and u an isomorphism of a subfield K of E onto a subfield $ K' $ of $ E' $. Let $ \mathbf{x} = (x_i)_{i \in I} $ (resp. $ \mathbf{x}' = (x'_i)_{i \in I} $) be a family of elements of E (resp. $ E' $) which is algebraically free over K (resp. $ K' $). Then there exists a unique isomorphism $ v $ of $ L = K(x_i)_{i \in I} $ onto $ L' = K'(x'_i)_{i \in I} $, which induces $ u $ on $ K $ and maps $ x_i $ to $ x'_i $ for each $ i \in I $.

The uniqueness of $ v $ is clear. Let us put $ A = K[x_i]_{i \in I} $ and $ A' = K'[x'_i]_{i \in I} $. By hypothesis the monomials $ x'' = \prod_{i \in I} x_i^{\alpha_i} $ (for $ \alpha = (\alpha_i)_{i \in I} $, in $ \mathbf{N}^{(I)} $) form a basis of the vector K-space $ A $ and there is a similar property of $ A' $. Hence there exists a ring isomorphism $ w : A \to A' $ mapping each element $ \sum_{\alpha \in \mathbf{N}^{(I)}} c_\alpha x^\alpha $ to $ \sum_{\alpha \in \mathbf{N}^{(I)}} u(c_\alpha) x'^\alpha $. Since $ L $ is the field of fractions of $ A $ and $ L' $ that of $ A' $, the isomorphism $ w $ extends to an isomorphism $ v $ of the field $ L $ onto the field $ L' $.

#### Corollary {#alg-v-s14-n1-cor-1 .statement}

— *For an extension E of a field K to be pure it is necessary and sufficient for E to be K-isomorphic to a field of rational fractions over K. More precisely, if the family $ (x_i)_{i \in I} $ is a pure basis of E, then there exists a unique K-isomorphism of $ K(X_i)_{i \in I} $ onto E which maps $ X_i $ to $ x_i $ for each $ i \in I $.*

#### Remark {#alg-v-s14-n1-rem-1 .statement}

— It is clear that in an extension E of K an algebraically free family over K consists of *linearly independent* elements over $ K $ (hence pairwise distinct); in other words, it is also a free family for the *vector space* structure of $ E $ (with respect to K). But the converse is false, for if E is an algebraic extension of K, any non-empty family of elements of E (and *a fortiori* a non-empty family of linearly independent elements over K) is never algebraically free over K. When there is a risk of confusion, we shall say that a subset of an extension E of K which is free for the vector space structure of E with respect to K is *linearly free* over K.

Let E be an extension of a field K. A subset S of E is said to be *algebraically free* (over $ K $) if the family defined by the identity mapping of S onto itself is algebraically free. The elements of an algebraically free subset of E are also called *algebraically independent*. If a subset of E is not algebraically free, it is said to be *algebraically related* and that its elements are *algebraically dependent*. For a family $ (x_i)_{i \in I} $ of elements of E to be algebraically free it is necessary and sufficient that $ i \mapsto x_i $ should be a bijection of I onto an algebraically free subset of E.

Every subset of an algebraically free set is algebraically free. Furthermore:

#### Proposition 3 {#alg-v-s14-prop-3 .statement}

— *For a family $ (x_i)_{i \in I} $, of elements of an extension E of a field K to be algebraically free over K it is necessary and sufficient that every finite subfamily of $ (x_i)_{i \in I} $ should be algebraically free over K.*

This proposition follows immediately from Def. 1.

### 2. Transcendence bases

#### Proposition 4 {#alg-v-s14-prop-4 .statement}

— *Let E be an extension of a field K and S and T two subsets of E. Then the following properties are equivalent:
a) $ S \cup T $ is algebraically free over K and $ S \cap T = \varnothing $.*

b) $ S $ is algebraically free over $ K $ and $ T $ is algebraically free over $ K(S) $.
c) $ T $ is algebraically free over $ K $ and $ S $ is algebraically free over $ K(T) $.

Evidently it is enough to prove that $ a) $ and $ b) $ are equivalent.

$ a) \Rightarrow b) $: Suppose that $ a) $ holds. Since $ S $ is contained in $ S \cup T $, it is algebraically free over $ K $. If $ T $ is not algebraically free over $ K(S) $, there exists (Prop. 3) a finite family $ (y_j)_{1 \leq j \leq n} $ of distinct elements of $ T $ which is algebraically related over $ K(S) $. Hence there is a non-zero polynomial $ f $ in the ring $ K(S)[Y_1, ..., Y_n] $ such that $ f(y,, ..., y,) = 0 $; after multiplying $ f $ if necessary by a non-zero element of $ K[S] $ we may suppose that all the coefficients off belong to $ K[S] $. The coefficients of fare polynomials in a finite number of distinct elements $ x_i \ (1 \leq i \leq m ) $ of $ S $, with coefficients in $ K $. The elements $ x_1, ..., x,, y_1, ..., y, $ are pairwise distinct because $ S \cap T = (21 $. The relation $ f(y,, ..., y,) = 0 $ may thus be written

$$
g(x_1, ..., x_m ; y_1, ..., y_n) = 0 ,
$$

where $ g $ is a non-zero polynomial of $ K[X_1, ..., X_m, Y_1, ..., Y_n] $, and such a relation contradicts the hypothesis that $ S \cup T $ is algebraically free.

$ b) \Rightarrow a) $: Suppose that $ b) $ holds. In the first place it is clear that $ T \cap K(S) = \varnothing $ and $ a fortiori \ S \cap T = (21 $. It suffices to show that if $ x_i \ (1 \leq i \leq m ) $ are distinct elements of $ S $, finite in number, and $ y_j \ (1 \leq j \leq n ) $ distinct elements of $ T $ finite in number, then the set of the $ x_i $ and $ y, $ is algebraically free over $ K $ (Prop. 3). Consider a polynomial $ f \in K[X_1, ..., X,, Y_1, ..., Y_n] $ such that $ f(x_1, ..., x_m, y_1, ..., y,) = 0 $ and put $ f = \sum \varphi_\alpha Y_1^{\alpha_1} ... Y_n^{\alpha_n} $ with $ \varphi_\alpha \in K[X_1, ..., X_m] $ for all $ \alpha = (\alpha,, ..., \alpha_n) \in \mathbf{N}^n $. Let $ g = f(x,, ..., x,, Y_1, ..., Y,) $; then $ g $ is a polynomial in the ring $ K[S][Y_1, ..., Y,] $ and the relation $ f(x_1, ..., x_m, y_1, ..., y,) = 0 $ may be written $ g(y_1, ..., y,) = 0 $. Since $ T $ is algebraically free over $ K(S) $, each of the coefficients $ \varphi_\alpha(x_1, ..., x,) $ of $ g $ is zero; since $ S $ is algebraically free over $ K $, we have $ \varphi_\alpha = 0 $ for all $ \alpha \in \mathbf{N}^n $, and hence $ f = 0 $.

#### Corollary {#alg-v-s14-n2-cor-1 .statement}

— *Let E be an extension of a field K and S a subset of E which is algebraically free over K. If x \in E is transcendental over K(S), then S U {x} is algebraically free over K.*

#### Proposition 5 {#alg-v-s14-prop-5 .statement}

— *Let E be an extension of the field K. For a subset S of E to be algebraically free over K it is necessary and sufficient that for each x \in S, the element x should be transcendental over the field K(S - {x}).*

The condition is necessary by Prop. 4.

To prove the sufficiency it is enough (Prop. 3) to show that every finite sequence $ (x_1, ..., x,) $ of distinct elements of $ S $ is algebraically free. Now by hypothesis $ x_i $ is transcendental over $ K(x_1, ..., x_{i-1}) $ for $ 1 \leq i \leq n $, and now our assertion follows by induction on $ n $ from the Cor. to Prop. 4.

#### Proposition 6 {#alg-v-s14-prop-6 .statement}

— *Let E be an extension of a field K and X an algebraically free subset of E over K. If K' \subset E is an algebraic extension of K then X is algebraically free over K'.*

Arguing by contradiction, let us suppose that X is algebraically related over K'. By Prop. 5 there exists an element $ x \in X $ which is algebraic over the field $ K'(M) $, where $ M = X - \{x\} $. Since $ K'(M) = K(M)(K') $ and $ K' $ is algebraic over $ K $, Cor. 2 of V, p. 18 shows that $ K'(M) $ is algebraic over $ K(M) $; since $ x $ is algebraic over $ K'(M) $, it is therefore algebraic over $ K(M) = K(X - \{x\}) $, by Prop. 3 of V, p. 19. Now Prop. 5 shows X to be algebraically related over K and we have a contradiction.

#### Definition 3 {#alg-v-s14-def-3 .statement}

*A subset B of an extension E of a field K is a transcendence basis of E (over K) if B is algebraically free over K and E is algebraic over K(B).*

#### Example {#alg-v-s14-n2-exa-1 .statement}

— *A pure basis is a transcendence basis. On the other hand, if E is a pure extension of K, a transcendence basis of E over K is not always a pure basis of E. For example, in $ K(X) $, $ \{X^2\} $ is a transcendence basis but does not generate $ K(X) $.*

#### Proposition 7 {#alg-v-s14-prop-7 .statement}

*Let E be an extension of a field K. Every transcendence basis of E is a maximal element of the set (ordered by inclusion) of subsets of E algebraically free over K. Conversely, if S is a subset of E such that E is algebraic over $ K(S) $, every maximal algebraically free subset of S is a transcendence basis of E.*

Let B be a transcendence basis of E over K and $ x \in E - B $. Then $ x $ is algebraic over $ K(B) $; by V, p. 107, Prop. 4, the subset $ B \cup \{x\} $ of E is not algebraically free over K, whence the first part of the proposition. Secondly, if E is algebraic over $ K(S) $ and B is a maximal algebraically free part of S, it follows from the Cor. of Prop. 4 that every $ x \in S $ is algebraic over $ K(B) $; hence (V, p. 18, Cor. 1) $ K(S) $ is algebraic over $ K(B) $, and so (V, p. 19, Prop. 3), E is algebraic over $ K(B) $.

#### Theorem 1 (Steinitz) {#alg-v-s14-thm-1 .statement}

— *Every extension E of a field K admits a transcendence basis over K. In other words, every extension of a field K is an algebraic extension of a pure extension of K.*

By contrast, an extension is not always a pure extension of an algebraic extension (V, p. 171, Ex. 2).

This theorem is a consequence of the following more precise result:

#### Theorem 2 {#alg-v-s14-thm-2 .statement}

*Let E be an extension of a field K, S a subset of E such that E is algebraic over $ K(S) $ and T a subset of S which is algebraically free over K; then there exists a transcendence basis B of E over K such that $ T \subset B \subset S $.*

For the set of algebraically free subsets of S, ordered by inclusion, is a set of finite character (E, III, p. 34) by Prop. 3. By Th. 1 of E, III, p. 35 it has a maximal element B containing T, and B is a transcendence basis of E over K, by Prop. 7.

#### Corollary (« Exchange Theorem ») {#alg-v-s14-n2-cor-2 .statement}

— Let E be an extension of K, S a subset of E such that E is algebraic over K(S), T a subset of E which is algebraically free over K; then there exists a subset S' of S such that T ∪ S' is a transcendence basis of E over K and T ∩ S' = ∅.

For E is algebraic over K(T U S) and we have T ⊂ T U S.

### 3. The transcendence degree of an extension

#### Theorem 3 {#alg-v-s14-thm-3 .statement}

— Let E be an extension of a field K. All transcendence bases of E over K have the same cardinal.

It is enough to prove the inequality Card(B) ≥ Card(B'), when B and B' are two transcendence bases of E over K, and we may suppose that B' is not empty. We first suppose that B is finite and use induction on its cardinal n; for n = 0, E is algebraic over K and B' is empty. Suppose now that n ≥ 1; given x ∈ B', the exchange theorem provides a subset C of B such that x ∉ C and {x} U C is a transcendence basis of E over K; we have C ≠ B by Prop. 7 whence Card C < n. Put K_1 = K(x) and C' = B' - {x}; then C and C' are algebraically free over the field K_1 (V, p. 107, Prop. 4) and E is algebraic both over K_1(C) = K(C U {x})) and K_1(C') = K(B'). In other words, C and C' are two transcendence bases of E over K_1. Since Card(C) < n, the induction hypothesis implies the inequality Card(C') ≤ Card(C) ≤ n - 1, whence Card(B') ≤ n = Card(B).

Suppose now that B is infinite. Every x ∈ B is algebraic over K(B') and so there exists a finite subset S(x) of B' such that x is algebraic over K(S(x)). Write S = U_{x ∈ B} S(x), then S ⊂ B' and since B is infinite, we have Card(S) ≤ Card(B) (E, III, p. 49, Cor. 3). But since every element of B is algebraic over K(S) and E is algebraic over K(B), we conclude that E is algebraic over K(S) (V, p. 19, Prop. 3). Now Prop. 7 implies that S = B', whence the desired inequality Card(B') ≤ Card(B).

#### Definition 4 {#alg-v-s14-def-4 .statement}

— Let E be an extension of a field K. The cardinal of every transcendence basis of E over K is called the transcendence degree of E over K and written tr. deg_K E.

Th. 2 and 3 and Def. 4 imply the following corollaries, where E denotes an extension of a field K, of finite transcendence degree n.

#### Corollary 1 {#alg-v-s14-def-4-cor-1 .statement}

— Let S be a subset of E such that E is algebraic over K(S). Then Card(S) ≥ n; if the cardinal of S is equal to n, then S is algebraically free over K (hence it is then a transcendence basis of E over K).

#### Corollary 2 {#alg-v-s14-def-4-cor-2 .statement}

— Suppose that E = K(x_1, ..., x_m), then m ≥ n; if moreover m = n, then (x_1, ..., x_m) is a pure basis of E over K, and E is then a pure extension of K.

#### Corollary 3 {#alg-v-s14-def-4-cor-3 .statement}

— Every subset of $ E $ which is algebraically free over $ K $ has at most $ n $ elements, and if it has exactly $ n $ elements, it is a transcendence basis of $ E $ over $ K $.

#### Theorem 4 {#alg-v-s14-thm-4 .statement}

— Let $ K, E $ and $ F $ be three fields such that $ K \subset E \subset F $. If $ S $ is a transcendence basis of $ E $ over $ K $ and $ T $ a transcendence basis of $ F $ over $ E $, then $ S \cap T $ is empty and $ S \cup T $ is a transcendence basis of $ F $ over $ K $.

For $ F $ is algebraic over $ E(T) $; moreover, $ E(T) $ is algebraic over the field $ K(S \cup T) = K(S)(T) $, because $ E $ is algebraic over $ K(S) $ ($ V $, p. 18, Cor. 2); therefore ($ V $, p. 19, Prop. 3) $ F $ is algebraic over $ K(S \cup T) $. On the other hand, $ T $ being algebraically free over $ E $ is so $ a fortiori $ over $ K(S) $, hence ($ V $, p. 107, Prop. 4) $ S \cup T $ is algebraically free over $ K $ and $ S \cap T = \varnothing $.

#### Corollary {#alg-v-s14-n3-cor-1 .statement}

— Let $ K, E $ and $ F $ be three fields such that $ K \subset E \subset F $. Then we have
$$
\text{tr. deg}_K F = \text{tr. deg}_K E + \text{tr. deg}_E F
$$

### 4. Extension of isomorphisms

#### Proposition 8 {#alg-v-s14-prop-8 .statement}

— Let $ \Omega $ be an algebraically closed extension of a field $ K $, $ E $ and $ F $ two subextensions of $ \Omega $ and $ u $ a $ K $-isomorphism of $ E $ onto $ F $. For a $ K $-automorphism $ v $ of $ O $ to exist which extends $ u $, it is necessary and sufficient for $ \Omega $ to have the same transcendence degree over $ E $ and $ F $.

The condition is clearly necessary.

Suppose then that $ \Omega $ has the same transcendence degree over $ E $ and $ F $ and let us choose a transcendence basis $ B $ of $ \Omega $ over $ E $ and a transcendence basis $ C $ of $ \Omega $ over $ F $. Since $ B $ and $ C $ are equipotent, Prop. 2 ($ V $, p. 106) shows that $ u $ extends to a $ K $-isomorphism $ u' $ of $ E(B) $ onto $ F(C) $. Since $ C? $ is an algebraic closure of $ E(B) $ and $ F(C) $, the Cor. of $ V $, p. 23 shows that $ u' $ extends to an automorphism $ v $ of $ \Omega $.

#### Corollary 1 {#alg-v-s14-prop-8-cor-1 .statement}

— Let $ O $ be an algebraically closed extension of a field $ K $ and $ E $ a subextension of $ \Omega $. Every $ K $-automorphism of $ E $ extends to a $ K $-automorphism of $ \Omega $.

#### Corollary 2 {#alg-v-s14-prop-8-cor-2 .statement}

— Let $ \Omega $ be an algebraically closed extension of a field $ K $, $ E $ and $ F $ two subextensions of $ \Omega $ and $ u $ a $ K $-isomorphism of $ E $ onto $ F $. If the transcendence degree of $ E $ over $ K $ is finite (in particular if $ E $ is algebraic over $ K $) then there exists a $ K $-automorphism of $ \Omega $ extending $ u $.

Let us denote by $ n, d(E) $ and $ d(F) $ the transcendence degrees of $ E $ over $ K $, of $ O $ over $ E $ and of $ C? $ over $ F $ respectively. The existence of the $ K $-isomorphism $ u $ shows that the transcendence degree of $ F $ over $ K $ is equal to $ n $. By the Cor. of Th. 4 the transcendence degree of $ \Omega $ over $ K $ is equal to $ d(E) + n $ and also to $ d(F) + n $. Therefore ($ E $, III, p. 28, Prop. 8) we have $ d(E) = d(F) $ and we can apply Prop. 8.

#### Proposition 9 {#alg-v-s14-prop-9 .statement}

— Let K be a field and $ \Omega $ an algebraically closed extension of K. Suppose that $ \Omega $ is not algebraic over K; then the set of elements of $ \Omega $ which are transcendental over K is infinite. Moreover, if x and y are two elements of $ \Omega $ which are transcendental over K, then there exists an automorphism u of $ \Omega $ over K such that $ u(x) = y $.

Since $ \Omega $ is not algebraic over K, there exists an element x of $ \Omega $ transcendental over K; then the elements $ x^n $ ($ n \in \mathbf{N} $) are distinct and transcendental over K. Suppose that x and y are distinct and transcendental over K; by Prop. 2 (V, p. 106) there exists a K-isomorphism $ \tilde{u} $ of $ K(x) $ onto $ K(y) $ such that $ \tilde{u}(x) = y $; since $ K(x) $ is of transcendence degree 1 over K, Cor. 2 of Prop. 8 shows that $ \tilde{u} $ extends to a K-automorphism u of $ \Omega $.

#### Proposition 10 {#alg-v-s14-prop-10 .statement}

— Let K be a field, $ \Omega $ an algebraically closed extension of K and G the group of K-automorphisms of $ \Omega $. Let $ x \in \Omega $.

a) For x to be algebraic over K it is necessary and sufficient for the set of elements $ u(x) $ as u runs over G to be finite,

b) For x to be p-radical over K it is necessary and sufficient that $ u(x) = x $ for all $ u \in G $.

In particular if K is perfect, the set of invariants of the group G is equal to K.

Suppose first that x is transcendental. By Prop. 9 the set T of elements of $ \Omega $ transcendental over K is infinite, and for each $ y \in T $ there exists $ u \in G $ such that $ u(x) = y $. Hence the set of elements $ u(x) $ as u runs over G is infinite.

Suppose now that x is algebraic over K and denote by fits minimal polynomial over K; the set of roots of f in $ \Omega $ is finite and for each $ u \in G $ we have $ f(u(x)) = u(f(x)) = 0 $. Hence the set of elements $ u(x) $ as u runs over G is finite. This proves a).

Let L be the set of elements y of $ \Omega $ such that $ u(y) = y $ for all $ u \in G $, and let $ \bar{K} $ be the relative algebraic closure of K in $ \Omega $. By what has been said, L is a subextension of $ \bar{K} $ over K. Further (Cor. 1 to Prop. 8) every K-automorphism of $ \bar{K} $ is the restriction to $ \bar{K} $ of an element of G. Assertion b) of Prop. 10 now follows from Cor. 3 of V, p. 53.

### 5. Algebraically disjoint extensions

#### Definition 5 {#alg-v-s14-def-5 .statement}

— Let L be an extension of a field K, and E and F two subextensions of L. Then E and F are said to be algebraically disjoint (over K) and E is said to be algebraically disjoint from F over K, if for every subset A (resp. B) of E (resp. F) algebraically free over K, A and B are disjoint and $ A \cup B $ is algebraically free over K.

#### Remark {#alg-v-s14-n5-rem-1 .statement}

— 1) If E is a subextension of L which is algebraic over K, then it is algebraically disjoint from every subextension F of L. For an extension of K to be algebraic it is necessary and sufficient that it should be algebraically disjoint from itself.

2) It may happen that E is algebraically disjoint from F over K, but not over a subfield $ K_{\|} $ of K. \* For example C is algebraically disjoint from itself over R but not over $ \mathbf{Q} $. \*

3) It is clear that if E is algebraically disjoint from $ F $ over K, when E and F are considered as subextensions of L, the same is true when they are considered as subextensions of $ K(E \cup F) $ and conversely.

#### Proposition 11 {#alg-v-s14-prop-11 .statement}

— *If E and F are algebraically disjoint over K then* $ E \cap F $ *is algebraic over K*.

This follows from Def. 5.

#### Proposition 12 {#alg-v-s14-prop-12 .statement}

— *Let L be an extension of a field K and E, F subextensions of L. Then the following conditions are equivalent*:

a) *E and F are algebraically disjoint*;

b) *there exists a transcendence basis of E over K which is algebraically free over F*;

c) *every subset of E which is algebraically free over K is algebraically free over F*.

Let us introduce the following conditions:

$ b' $') *there exists a transcendence basis of F over K which is algebraically free over E*;

$ c' $') *every subset of F which is algebraically free over K is algebraically free over E*.

$ a) \Rightarrow b' $') : Suppose that E and F are algebraically disjoint. Let B (resp. C) be a transcendence basis of E (resp. $ F $) over K. Then $ B \cap C = \varnothing $ and $ B \cup C $ is algebraically free over K, hence C is algebraically free over $ K(B) $ (V, p. 107, Prop. 4); since E is algebraic over $ K(B) $, Prop. 6 of V, p. 108 shows C to be algebraically free over E.

$ b' $') $ \Rightarrow $ c) : Suppose that there exists a transcendence basis C of F over K which is algebraically free over E. Let A be a subset of E algebraically free over K. Then C is algebraically free over $ K(A) $, hence A is algebraically free over $ K(C) $ (V, p. 107, Prop. 4) and therefore over $ F $ (V, p. 108, Prop. 6), because F is algebraic over $ K(C) $.

c) $ \Rightarrow $ a) : This follows at once from Prop. 4 (V, p. 107).

The implications $ a) \Rightarrow b) \Rightarrow c' ) \Rightarrow a) $ may be proved in the same way.

#### Corollary {#alg-v-s14-n5-cor-1 .statement}

— *Let E and F be algebraically disjoint over K. Let E' be the relative algebraic closure of E in L and F' that of F* (V, p. 19). *Then* E' *and F'* *are algebraically disjoint over K*.

Let B be a transcendence basis of E over K; this is also a transcendence basis of E' over K. Since E is algebraically disjoint from F over K, B is algebraically free over F, hence over F' (V, p. 108, Prop. 6); now we can apply Prop. 12.

#### Proposition 13 {#alg-v-s14-prop-13 .statement}

— *Let L be an extension of a field K and E, F two subextensions of L*.

a) *We have* $ \operatorname{tr. deg}_L F(E) \leq \operatorname{tr. deg}_K E $. *When E and F are algebraically disjoint over K, then every transcendence basis of E over K is a transcendence basis of*

F(E) over F and we have tr . deg_F F(E) = tr . deg_K E. Conversely, this equality implies that E and F are algebraically disjoint over K when tr . deg_K E is finite.

b) We have tr . deg_K K(E U F) ≤ tr . deg_K E + tr . deg_K F. When E and F are algebraically disjoint over K, we have tr . deg_K K(E U F) = tr . deg_K E + tr . deg_K F. Conversely, this equality implies that E and F are algebraically disjoint over K when E and F are of finite transcendence degree over K.

a) Let B be a transcendence basis of E over K; then E is algebraic over K(B), and Cor. 2 of V, p. 18 shows that F(E) is algebraic over F(K(B)) = F(B). By Th. 2 (V, p. 109) B contains a transcendence basis of F(E) over F; when E is algebraically disjoint from F over K, B is algebraically free over F (Prop. 12) and this is then a transcendence basis of F(E) over F. The three first assertions of a) follow from this. Suppose now that E is of finite transcendence degree over K, equal to that of F(E) over F; since F(E) is algebraic over F(B) and Card B = tr . deg_F F(E), Cor. 1 of V, p. 110 shows B to be algebraically free over F, so E is algebraically disjoint from F over K (Prop. 12).

b) We have K(E U F) = F(E) and so the Cor. of V, p. 110 implies the equality:

$$
\text{tr . deg}_K K(E \cup F) = \text{tr . deg}_F F(E) + \text{tr . deg}_K F .
$$

Now b) follows at once from a) and this equality.

#### Proposition 14 {#alg-v-s14-prop-14 .statement}

— *Let L be an extension of a field K, E and F two subextensions of L and B a transcendence basis of E over K. For E and F to be algebraically disjoint over K it is necessary and sufficient that K(B) and F should be linearly disjoint over K.*

For E and F to be algebraically disjoint over K it is necessary and sufficient for B to be algebraically free over F (Prop. 12), that is, for the monomials in the elements of B to be linearly independent over F. Since these monomials form a basis of the vector K-space K[B], it comes to the same to say that K[B] and F are linearly disjoint over K. Finally, since K(B) is the field of fractions of K[B], Prop. 6 of V, p. 14 shows that K[B] and F are linearly disjoint if and only if this is so for K(B) and F.

#### Corollary 1 {#alg-v-s14-prop-14-cor-1 .statement}

— *If E and F are linearly disjoint, then E is algebraically disjoint from F over K. Conversely, if E is a pure extension of K and is algebraically disjoint from F over K, then E and F are linearly disjoint over K.*

#### Corollary 2 {#alg-v-s14-prop-14-cor-2 .statement}

— *Every pure extension of K is linearly disjoint from every algebraic extension of K; in particular, K is relatively algebraically closed in every pure extension of K.*

### 6. Algebraically free families of extensions

#### Definition 6 {#alg-v-s14-def-6 .statement}

— Let $ L $ be an extension of a field $ K $ and $ (E_i)_{i \in I} $ a family of subextensions of $ L $. The family $ (E_i)_{i \in I} $ is said to be algebraically free if the following condition is satisfied:

(AF) For each $ i \in I $ let $ A_i $ be a subset of $ E_i $ which is algebraically free over $ K $. Then $ A_i \cap A_j = \varnothing $ for $ i \neq j $ and $ \bigcup_{i \in I} A_i $ is algebraically free over $ K $.

#### Remark {#alg-v-s14-n6-rem-1 .statement}

— By Prop. 3 ($ V $, p. 107) it is enough to verify the condition (AF) for finite subsets $ A_i $. We thus obtain the following result : if $ (E_i)_{i \in I} $ is an algebraically free family, the same is true of $ (E'_i)_{i \in I} $ if $ E'_i $ is a subextension of $ E_i $ for each $ i \in I $; conversely, if every family $ (E'_i)_{i \in I} $, where $ E'_i $ is a finitely generated subextension of $ E $ for each $ i \in I $ is algebraically free, then $ (E_i)_{i \in I} $ is algebraically free. On the other hand, for $ (E_i)_{i \in I} $ to be algebraically free it is necessary and sufficient that $ (E_i)_{i \in J} $ should be algebraically free for every finite subset $ J $ of $ I $. Speaking intuitively we may say that the algebraic independence of extensions is a property « of finite character ».

#### Proposition 15 {#alg-v-s14-prop-15 .statement}

— Let $ (E_i)_{i \in I} $ be a family of subextensions of a given extension $ L $ of a field $ K $. Then the following conditions are equivalent :

a) The family $ (E_i)_{i \in I} $ is algebraically free.

b) For each $ i \in I $ the extension $ E_i $ is algebraically disjoint over $ K $ from the extension $ F_i $ generated by the $ E_j $ for $ j \neq i $.

c) There exists a family $ (B_i)_{i \in I} $ of disjoint subsets of $ L $, such that $ B_i $ is a transcendence basis of $ E_i $ over $ K $ for each $ i \in I $, and $ B = \bigcup_{i \in I} B_i $ is algebraically free over $ K $.

It is clear that $ a) $ implies $ c) $.

Assuming $ c) $, let us choose $ i $ in $ I $; put $ C_i = \bigcup_{j \neq i} B_j $. For each $ j \neq i $ every element of $ E_j $ is algebraic over $ K(B_j) $ and a fortiori over $ K(C_i) $. By Cor. 1 of $ V $, p. 18, the field $ F_i $ is therefore algebraic over $ K(C_i) $. Further, we have $ B_i \cap C_i = \varnothing $ and $ B - B_i \cup C_i $ is algebraically free over $ K $; therefore $ B_i $ is algebraically free over $ K(C_i) $ ($ V $, p. 107, Prop. 4), hence also over $ F_i $ (which is algebraic over $ K(C_i) $) by Prop. 6 of $ V $, p. 108. Thus we have proved that $ E_i $ is algebraically disjoint from $ F_i $ over $ K $ ($ V $, p. 113, Prop. 12), hence $ c) $ implies $ b) $.

Let us now assume $ b) $ and prove $ a) $. It is enough to show that if $ i_1, \ldots, i_n $ are distinct elements of $ I $, then the family of extensions $ (E_{i_1}, \ldots, E_{i_n}) $ is algebraically free; we argue by induction on $ n $, the case $ n = 1 $ being trivial. Suppose then that $ n > 1 $ and that the family $ (E_{i_1}, \ldots, E_{i_{n-1}}) $ is algebraically free; for $ 1 \leq k \leq n $ choose a subset $ A_k $ of $ E_{i_k} $ algebraically free over $ K $ and put

B = A, U ... U A_{n-1}. By the induction hypothesis the subsets A_1, ..., A_{n-1} are pairwise disjoint and B is algebraically free over K; by b) E_{i_n} is algebraically disjoint from F_i and since B is contained in F_{i_n} we have B \cap A_i = \varnothing and B \cup A_i = A, U ... U A_i is algebraically free over K. We have thus shown that the family (E_{i_1}, ..., E_{i_n}) is algebraically free.

The following proposition generalizes part b) of Prop. 13 (V, p. 113).

#### Proposition 16 {#alg-v-s14-prop-16 .statement}

— *Let* (E_i)_{i \in I} *be a family of subextensions of an extension of a field K*, and let E be the field generated by $ \bigcup_{i \in I} E_i $.

a) *We have* tr . deg_K E \leq \sum_{i \in I} \text{tr . deg}_K E_i, *with equality when the family* (E_i)_{i \in I} *is algebraically free over K*.

b) *Conversely, assume that* tr . deg_K E = \sum_{i \in I} \text{tr . deg}_K E_i *and that* tr . deg_K E *is finite; then the family* (E_i)_{i \in I}, *is algebraically free over K*.

For each $ i \in I $ let B_i be a transcendence basis of E_i over K and put $ B = \bigcup_{i \in I} B_i $. For each $ i \in I $, each element of E_i is algebraic over K(B_i), hence over K(B). Now Cor. 1 of V, p. 18 shows that E is algebraic over K(B); by V, p. 109, Th. 2, B thus contains a transcendence basis of E over K. If moreover the family (E_i)_{i \in I} is algebraically free over K, then the B_i are disjoint and the set B is algebraically free over K. This establishes a) (*Set Theory*, III, p. 160, Cor. of Prop. 4).

Under the hypotheses of b), E is algebraic over K(B) and of finite transcendence degree over K, and we have Card(B) \leq \text{tr . deg}_K E. By Cor. 1 of V, p. 110, B is algebraically free over K and the B_i are disjoint. Now Prop. 15 shows that the family (E_i)_{i \in I} is algebraically free over K.

Before stating the next theorem let us remark that there exist algebraically closed extensions of K of arbitrary transcendence degree, for example an algebraic closure of an appropriate field of rational fractions.

#### Theorem 5 {#alg-v-s14-thm-5 .statement}

— *Let* (E_i)_{i \in I}, *be a family of extensions of a field K and* \Omega *an algebraically closed extension of K*. *Suppose that the inequality*

$$
\text{tr . deg}_K \Omega \geq \sum_{i \in I} \text{tr . deg}_K E_i
$$

*holds. Then there exists an algebraically free family* (F_i)_{i \in I}, *of subextensions of* \Omega *such that* F_i *is K-isomorphic to* E_i *for all* i \in I.

For each $ i \in I $ let B_i be a transcendence basis of E_i over K. Let B be a transcendence basis of \Omega over K. By (2) we have Card B \geq \sum_{i \in I} \text{Card} B_i; *hence* there exists a family (B'_i)_{i \in I}, *of pairwise disjoint subsets of B and bijections* u_i : B_i \to B'_i *for* i \in I. *By Prop. 2 of V, p. 106, u, extends to a K-isomorphism* v_i *of* K(B_i) *onto* K(B'_i); *since* \Omega *is algebraically closed and* E_i *algebraic over*

K(B_i), the Cor. (V, p. 23) shows that $ v_i $ extends to a K-isomorphism of $ E_i $ onto a subextension $ F_i $ of $ \Omega $. By construction $ B'_i $ is a transcendence basis of $ F_i $ over K, and Prop. 15 (V, p. 115) shows that the family $ (F_i)_{i \in I} $ of subextensions of $ \Omega $ is algebraically free over K.

#### Corollary 1 {#alg-v-s14-thm-5-cor-1 .statement}

— *Let E and R be two extensions of a field K. Suppose that $ \Omega $ is algebraically closed, of transcendence degree at least equal to that of E. Then E is K-isomorphic to a subextension of R.*

#### Corollary 2 {#alg-v-s14-thm-5-cor-2 .statement}

— *Let R be an algebraically closed field of infinite transcendence degree over its prime subfield. Then every field of the same characteristic as $ \Omega $ is the ascending directed union of fields isomorphic to subfields of R.*

For each field is the ascending directed union of finitely generated subfields over its prime field, and now it is enough to apply Cor. 1.
\* Example. — This applies particularly in characteristic 0 in taking $ \Omega = \mathbf{C} $ (« Lefschetz' principle »). \*

### 7. Finitely generated extensions

#### Proposition 17 {#alg-v-s14-prop-17 .statement}

— *Let E be an extension of a field K and B a transcendence basis of E over K. For E to be finitely generated over K (V, p. 11, Def. 2) it is necessary and sufficient that B be finite and that the degree $[E : K(B)]$ be finite.*

Suppose that E is finitely generated over K and let S be a finite subset of E such that $ E = K(S) $. By Th. 2 (V, p. 109) S contains a transcendence basis $ B' $ of E over K and this has the same cardinal as B (V, p. 110, Th. 3). Therefore B is finite. Put $ K' = K(B) $; then E is algebraic over $ K' $ and we have $ E = K'(S) $; since S is finite, Th. 2 of V, p. 18 shows that $[E : K']$ is finite.

Conversely, suppose that B is finite and $[E : K(B)]$ is finite. If C is a (finite) basis of the vector space E over $ K(B) $, we have $ E = K(B)(C) = K(B \cup C) $ and so E is a finitely generated extension of K.

#### Corollary 1 {#alg-v-s14-prop-17-cor-1 .statement}

— *Suppose that E is a finitely generated extension of K, and let $ K' $ be the relative algebraic closure of K in E (V, p. 19). Then $ K' $ is of finite degree over K.*

Let B be a transcendence basis of E over K. By Cor. 2 of V, p. 114, $ K' $ is linearly disjoint from $ K(B) $ over K, whence $[K' : K] = [K'(B) : K(B)] \leq [E : K(B)]$ and now the finiteness of $[K' : K]$ follows from that of $[E : K(B)]$.

#### Corollary 2 {#alg-v-s14-prop-17-cor-2 .statement}

— *A field that is finitely generated over its prime subfield contains only finitely many roots of unity.*

By Cor. 1 we are reduced to proving that a field L which is an extension of finite degree of its prime subfield possesses only a finite number of roots of unity. This is clear when L is of characteristic $ \neq 0 $ because it is then finite. If L is of characteristic 0 and contains infinitely many roots of unity, then it contains primitive roots of unity of arbitrarily high order. By V, p. 84, Th. 2 there exist therefore an infinity of integers $ n > 0 $ such that $ \varphi(n) \leq [L : \mathbf{Q}] $, which is absurd (V, p. 80, Formulae (2) and (3)).

#### Corollary 3 {#alg-v-s14-prop-17-cor-3 .statement}

— *If E is a finitely generated extension of a field K, then every subextension E' of E is finitely generated.*

Let B' be a transcendence basis of E' over K. By V, p. 109, Th. 2, B' is contained in a transcendence basis B of E over K and so is finite, by Prop. 17. Since E' is algebraic over K(B') and E is a finitely generated extension of K(B'). Cor. 1 shows $[E' : K(B')]$ to be finite. Now Prop. 17 shows that E' is finitely generated over K.

Prop. 17 may be paraphrased by saying that a finitely generated extension of K is an algebraic extension of finite degree of a purely transcendental extension $ K(x_1, \ldots, x_n) $.

### Exercises {#alg-v-s14-exercises}

See the [exercises for § 14](exercises/s14/).
