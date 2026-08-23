---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 7
section_title: Separable algebraic extensions
lang: en
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A V.36-A V.47, A V.151-A V.153
pdf_pages: 0150-0161, 0265-0267
extraction: ocr
subsections:
    - "no": 1
      title: Separable algebraic extensions
      page: 36
      pdf_page: 150
    - "no": 2
      title: Separable polynomials
      page: 37
      pdf_page: 151
    - "no": 3
      title: Separable algebraic elements
      page: 39
      pdf_page: 153
    - "no": 4
      title: The theorem of the primitive element
      page: 40
      pdf_page: 154
    - "no": 5
      title: Stability properties of separable algebraic extensions
      page: 41
      pdf_page: 155
    - "no": 6
      title: A separability criterion
      page: 42
      pdf_page: 156
    - "no": 7
      title: The relative separable algebraic closure
      page: 43
      pdf_page: 157
    - "no": 8
      title: The separable closure of a field
      page: 45
      pdf_page: 159
    - "no": 9
      title: Separable and inseparable degrees of an extension of finite degree
      page: 46
      pdf_page: 160
statements: 38
exercises: 5
content_sha256: 6a1e194beb6491068e8402aa0b896f006bcab263c6ed8066c487c9e85dadddc0
---

## § 7. SEPARABLE ALGEBRAIC EXTENSIONS

Throughout this paragraph $ K $ denotes a field.

### 1. Separable algebraic extensions

#### Definition 1 {#alg-v-s7-def-1 .statement}

— *Let E be an algebraic extension of K; then E is said to be separable (over K) if every subextension F of E of finite degree over K is an etale algebra over K* ($ V $, p. 28, Def. 1).

Let E be an extension of finite degree of K. Since every subalgebra of an etale algebra is etale ($ V $, p. 30, Prop. 3), it comes to the same to suppose that E is a separable extension of $ K $, or that E is an etale algebra over $ K $.

#### Proposition 1 {#alg-v-s7-prop-1 .statement}

— *Let E be an algebraic extension of K. If E is separable, then every subextension $ E' $ of E is separable. Conversely, if every subextension of finite degree of E is separable then E is separable.*

This follows immediately from Definition 1.

#### Proposition 2 {#alg-v-s7-prop-2 .statement}

— *For a field K to be perfect it is necessary and sufficient that every algebraic extension of K should be separable.*

Suppose first that K is perfect. Since a field is a reduced ring, it follows from Lemma 5 ($ V $, p. 35) that every extension of finite degree of $ K $ is an etale algebra over $ K $; therefore every algebraic extension of $ K $ is separable.

Suppose now that $ K $ is an imperfect field of characteristic $ p \neq 0 $. Let $ \Omega $ be an algebraic closure of $ K $. Since $ K $ is imperfect, there exists $ b \in K $ not belonging to $ K^p $; put $ a = b^{1/p} $. Then the extension $ K(a) $ of $ K $ is p-radical of finite degree. By $ V $, p. 26, Prop. 3, there exists a single K-homomorphism of $ K(a) $ into $ \Omega $, and since $ [K(a):K] > 1 $, the algebra $ K(a) $ is not etale over $ K $ ($ V $, p. 32, Prop. 4). In other words, the extension $ K(a) $ of finite degree of $ K $ is not separable.

#### Corollary {#alg-v-s7-n1-cor-1 .statement}

— *Every algebraic extension of a field of characteristic 0, or of a finite field, is separable.*
    This follows from *V*, p. 7, Prop. 5.

### 2. Separable polynomials

#### Proposition 3 {#alg-v-s7-prop-3 .statement}

— *Let f be a non-zero polynomial in K[X] and let Ω be an algebraically closed extension of K. The following conditions are equivalent:*
    *a) The polynomial f is relatively prime to its derivative f' in K[X].*
    *b) Either deg(f) = 0, or deg(f) > 0 and dis(f) ≠ 0 (IV, p. 83).*
    *c) There exists an extension L of K such that f splits in L[X] into a product of distinct polynomials of degree ≤ 1.*
    *d) The roots off in Ω are simple.*
    *e) The K-algebra K[X]/(f) is etale (V, p. 28, Def. 1).*

*a) ⇒ d)*: Under the hypothesis *a*) there exist two polynomials g and h in K[X] such that fg + f'h = 1 (IV, p. 12). Let a be a root of fin Ω; we have
$$
f'(a)\ h(a) = f(a)\ g(a) + f'(a)\ h(a) = 1,
$$
whence $ f'(a) \neq 0 $; therefore $ a $ is a simple root of fin Ω (*IV*, p. 17, Prop. 7).

*d) ⇒ c)*: If *d*) holds, f splits in Ω[X] into a product of distinct factors of degree ≤ 1.

*c) ⇒ b)*: Under the hypothesis c) there exist an element $ A \neq 0 $ in L and *distinct* elements $ a_1, ..., a_n $ of L such that $ f(X) = \lambda (X - a_1) ... (X - a_n) $. If $ \deg(f) > 0 $, we have (*IV*, p. 83, Prop. 11),
$$
\operatorname{dis}(f) = \lambda^{2n-2} \prod_{i < j} (\alpha_i - \alpha_j)^2 \neq 0.
$$

*b) ⇒ a)*: Let c be the leading coefficient and D the discriminant of f; the resultant of $ f' $ and f is equal to ± cD (IV, p. 84, Formula (54)), hence is non-zero; therefore (*IV*, p. 78, Cor. 2) the polynomials f and $ f' $ are relatively prime in K[X].

*a) ⇒ e)*: Let A be the K-algebra K[X]/(f) and x the image of X in A; by III, p. 573, Prop. 22, the A-module $ \Omega_K(A) $ is generated by the elements $ dx $, subject to the single relation $ f'(x)\ dx = 0 $. By *V*, p. 33, Th. 3, the K-algebra A is thus etale if and only if $ f'(x) $ is an invertible element in A, which means that f and $ f' $ are relatively prime in K[X].

#### Definition 2 {#alg-v-s7-def-2 .statement}

— *A polynomial $ f \in K[X] $ is said to be separable if it is non-zero and satisfies the equivalent conditions a), b), c), d) and e) of Prop. 3.*

#### Remark {#alg-v-s7-n2-rem-1 .statement}

— 1) Let L be an extension of K and f a non-constant polynomial in K[X]. By *e)* of Prop. 3 and V, p. 32, Cor. 2 it comes to the same to suppose that f is separable, whether considered as element of K[X] or of L[X]. On the other hand, it may well happen that f is irreducible in K[X] but not in L[X].

2) Let $ f \in K[X] $; we know (IV, p. 13, Prop. 13) that there exist irreducible polynomials $ f_1, \ldots, f_m $ in $ K[X] $ such that $ f = f_1 \ldots f_m $. Let $ \Omega $ be an algebraic closure of $ K $; since an irreducible polynomial $ g \in K[X] $ is the minimal polynomial over $ K $ of each of its roots in $ \Omega $, two distinct irreducible polynomials in $ K[X] $ have no common root in $ \Omega $. Condition $ d) $ of Prop. 3 now shows that $ f $ is separable if and only if the polynomials $ f_1, \ldots, f_m $ are separable and pairwise distinct.

#### Proposition 4 {#alg-v-s7-prop-4 .statement}

— *Let $ f $ be an irreducible polynomial in $ K[X] $. Then the following conditions are equivalent*:

a) $ f $ is separable.
b) *There exists an extension $ L $ of $ K $ in which $ f $ has a simple root.*
c) *The derivative $ f' $ off is not zero.*
d) *The field $ K $ is of characteristic $ 0 $, or it is of characteristic $ p \neq 0 $ and $ f \not\in K[X^p] $*.

We note first that an irreducible polynomial in $ K[X] $ is not constant. It is clear that $ a) $ implies $ b) $ (take an algebraic closure of $ K $ for $ L $). If $ x $ is a simple root off in an extension $ L $ of $ K $, we have $ f'(x) \neq 0 $ (IV, p. 17, Prop. 7), so $ b) $ implies $ c) $, and the equivalence of $ c) $ and $ d) $ follows from V, p. 9, Cor.

Suppose finally that $ f \neq 0 $; let $ x $ be a root of $ f $ in an algebraically closed extension $ \Omega $ of $ K $. Since $ f $ is the minimal polynomial of $ x $ over $ K $ and $ \deg f' < \deg f $, we have $ f'(x) \neq 0 $, and so $ x $ is a simple root of $ f $ (IV, p. 17, Prop. 7). Therefore $ f $ is separable and we have shown that $ c) $ implies $ a) $.

#### Corollary 1 {#alg-v-s7-prop-4-cor-1 .statement}

— *For a field $ K $ to be perfect it is necessary and sufficient that every irreducible polynomial of $ K[X] $ should be separable*.

If the field $ K $ is of characteristic $ 0 $, $ K $ is perfect and every irreducible polynomial of $ K[X] $ is separable, by $ d) $ above. Suppose then that $ K $ has characteristic $ p \neq 0 $.

Suppose first that $ K $ is perfect. We have $ K[X^p] = K[X]^p $, hence there exists no irreducible polynomial of $ K[X] $ belonging to $ K[X^p] $. By Prop. 4, every irreducible polynomial of $ K[X] $ is then separable.

Suppose next that $ K $ is imperfect, whence $ K \neq K^p $. Let $ a $ be an element of $ K $ not belonging to $ K^p $; the polynomial $ X^p - a $ is irreducible in $ K[X] $ (V, p. 24, Lemma 1), and it belongs to $ K[X^p] $, and so is not separable.

#### Corollary 2 {#alg-v-s7-prop-4-cor-2 .statement}

— *Let $ f \in K[X] $ be a non-zero polynomial. For $ f $ to be separable it is necessary and sufficient that there should exist an extension $ L $ of $ K $ which is a perfect field and such that $ f $ has no repeated factor in $ L[X] $*.

Let $ \Omega $ be an algebraic closure of $ K $; iff is separable, $ f $ has no repeated factors in $ \Omega[X] $ (Prop. 3, $ d$) ). Conversely, if $ L $ is a perfect extension of $ K $ such that $ f $ has no repeated factor in $ L[X] $, then $ f $ is separable in $ L[X] $ (Cor. 1 and Remark 2), hence in $ K[X] $ (Remark 1).

### 3. Separable algebraic elements

#### Definition 3 {#alg-v-s7-def-3 .statement}

— Let E be an extension of K. An element x of E which is algebraic over K is said to be separable over K if the algebraic extension K(x) of K is separable.

#### Proposition 5 {#alg-v-s7-prop-5 .statement}

— Let E be an extension of K, x an element of E algebraic over K and f the minimal polynomial of x over K. Then the following conditions are equivalent:
a) x is separable over K;
b) the polynomial f is separable;
c) x is a simple root of f.
The equivalence of a) and b) follows from Prop. 3, that of b) and c) from Prop. 3 and 4 (cf. V, p. 37 and 38).

#### Corollary 1 {#alg-v-s7-prop-5-cor-1 .statement}

— If an element x of E is a simple root of a polynomial g of K[X], it is separable over K.
For the minimal polynomial f of x over K divides g in K[X] (V, p. 16, Th. 1), so x is a simple root of f.

#### Corollary 2 {#alg-v-s7-prop-5-cor-2 .statement}

— If an element x of E is algebraic and separable over K, it is algebraic and separable over every extension K' of K contained in E.
Let f be the minimal polynomial of x over K. Then x is a simple root of f by Prop. 5, and since f belongs to K'[X], the element x of E is separable over K' by Cor. 1.

#### Corollary 3 {#alg-v-s7-prop-5-cor-3 .statement}

— Suppose that K has characteristic $ p \neq 0 $. For an element x of E to belong to K it is necessary and sufficient for it to be both separable algebraic and p-radical over K.
The stated condition is clearly necessary. Conversely suppose that x is separable algebraic over K and p-radical of height e over K. Since x is separable over K, the minimal polynomial f of x over K does not belong to K[X^p] (Prop. 4 and 5); since x is p-radical of height e over K, we have $ f(X) = X^{p^e} - x^{p^e} $ (V, p. 24, Prop. 1); we conclude that $ e = 0 $, so $ x \in K $.

#### Proposition 6 {#alg-v-s7-prop-6 .statement}

— Let E be an extension of K.
a) If E is algebraic and separable over K, every element of E is algebraic and separable over K.
b) Conversely, let A be a set of elements of E, algebraic and separable over K and such that $ E = K(A) $; then E is algebraic and separable over K.
If E is algebraic and separable over K, the same is true of the extension K(x) of K for every $ x \in E $, whence a).
Under the hypothesis b), the extension E is algebraic over K (V, p. 18, Cor. 1).

Let F be a subextension of E of finite degree over K. By V, p. 11, Cor., there exist elements $ x_1, \ldots, x_m $ of A such that $ F \subset K(x_1, \ldots, x_r) $ and we have

$$
K(x_1, \ldots, x_m) = K[x_1, \ldots, x_m] \quad (\text{V, p. 18, Cor. 1}).
$$

By the hypothesis on A, the algebras $ K[x_1], \ldots, K[x_m] $ are etale over K; hence the same is true of $ K[x_1] \otimes \cdots \otimes K[x_m] $ (V, p. 32, Cor. 1). Now F is isomorphic to a subalgebra of a quotient algebra of $ K[x_1] \otimes \cdots \otimes K[x_m] $, and so is etale (V, p. 30, Prop. 3).

#### Corollary {#alg-v-s7-n3-cor-1 .statement}

— *For an algebraic extension E to be separable over K it is necessary and sufficient that every element of E should be a simple root of its minimal polynomial over K. It is enough to apply Prop. 5 and 6.*

### 4. The theorem of the primitive element

Let $ E $ be an extension of $ K $; an element $ x $ of $ E $ is said to be *primitive* if $ E = K[x] $. For the extension $ E $ to possess a primitive element it is necessary for $ [E : K] $ to be finite.

#### Theorem 1 {#alg-v-s7-thm-1 .statement}

— *Let E be an extension of K. Then the following conditions are equivalent:
a) E possesses a primitive element;
b) there exist only a finite number of subextensions of E.
These conditions are satisfied when E is a separable extension of finite degree.*
Suppose first that $ E $ possesses a primitive element $ x $, and let $ f $ be the minimal polynomial of $ x $ over K. For each monic polynomial $ g \in E[X] $ dividing $ f $ in $ E[X] $ denote by $ E_g $ the subextension of $ E $ generated by the coefficients of g. Since the possible polynomials g are finite in number (if $ f $ splits in $ E[X] $ into a product of r monic irreducible polynomials, the number is bounded by $ 2^r $), the subextensions $ E_g $ are finite in number. To prove b) it is therefore enough to show that every subextension L of $ E $ is one of the $ E_g $. Now if $ L $ is a subextension of E, then we have $ L[x] = E $; if g is the minimal polynomial of $ x $ over L, we have $ [E : L] = \deg(g) $. Besides, g is a divisor off in $ L[X] $, hence in $ E[X] $; so we have $ E_g \subset L $ and $ E = E_g[x] $. Since $ g(x) = 0 $, we have $ [E : E_g] \leq \deg(g) $, therefore $ [E : E_g] \leq [E : L] $ and so $ L = E_g $ as we wished to show.

Next we observe that Condition b) implies that the extension E is of finite degree: by Remark 2 of V, p. 18 it suffices to prove that it is algebraic; now if z is an element of $ E $ transcendental over $ K $ then the subextensions $ K(z^n), n \in \mathbf{N} $ are pairwise distinct.

To show that b) $ \Rightarrow $ a) we now distinguish two cases:
A) If the field $ K $ is *finite*, the field $ E $ is a vector space of finite dimension over K and hence is a finite set. Therefore $ ^1 $ (V, p. 78, Lemma 1) there exists an element $ x $ of $ E $ generating the multiplicative group of $ E $, and we have $ E = K[x] $.

B) Suppose now that the field $ K $ is infinite. If $ b) $ holds, the extension $ E $ is of finite degree, so $ b) $ can also be expressed by saying that $ E $ possesses only a finite number of subalgebras. This being so, the implication $ b) \Rightarrow a) $ is a consequence of the following more general proposition (for which the hypothesis that the field $ K $ be infinite is indispensable, cf. V, p. 153, Ex. 5 of § 7):

#### Proposition 7 {#alg-v-s7-prop-7 .statement}

— *Suppose that $ K $ is infinite; let $ A $ be a commutative $ K $-algebra possessing only a finite number of sub-algebras (for example an etale $ K $-algebra, $ V $, p. 30, Prop. 3) and let $ V $ be a vector subspace of $ A $ generating $ A $. Then there exists $ x \in V $ such that $ A = K[x] $.*

Let $ A_1, \ldots, A_n $ be the subalgebras of $ A $ distinct from $ A $. If $ x \notin A_1 \cup \ldots \cup A_n $, then the sub-algebra $ K[x] $ cannot equal any of the $ A_i $ and so must coincide with $ A $. Further, since $ V $ generates $ A $, it is not contained in any of the subspaces $ A_i $. Prop. 7 is therefore a consequence of the following lemma:

*Lemma 1. — Let $ A $ be a vector $ K $-space, $ V, A_1, \ldots, A_n $ subspaces of $ A $. If $ \mathrm{Card}(K) \geq n $ and if $ V $ is not contained in any of the $ A_i $, then $ V $ is not contained in $ A_1 \cup \ldots \cup A_n $.*

Arguing by induction on $ n $, we need only prove that if $ V \subset A $, and $ V \subset A_1 \cup \ldots \cup A_n $, then $ V \subset A_1 \cup \ldots \cup A_{n-1} $. Let $ x \in V, x \notin A_n $, and let $ y $ be arbitrary in $ V $. If $ y \in Kx $, we have $ y \in A_1 \cup \ldots \cup A_{n-1} $; if not, then the elements $ x $ and $ y + \lambda x, \lambda \in K $ are strictly greater than $ n $ in number and belong to $ A_1 \cup \ldots \cup A_n $, so two of them belong to the same $ A_i $. Thus there exists $ i, 1 \leq i \leq n $ such that either $ x \in A_i $ and $ y + \lambda x \in A_i $ for some $ \lambda \in K $, or $ y + \mu x \in A_i $ and $ y + \mu x \in A_i $ for two distinct scalars $ \lambda, \mu \in K $. In both cases we conclude that $ x \in A_i $ and $ y \in A_i $; but this implies that $ i \neq n $, hence $ y \in A_1 \cup \ldots \cup A_{n-1} $, as we wished to show.

This completes the proof of the equivalence of $ a) $ and $ b) $ in Th. 1. Finally if the extension $ E $ is separable and of finite degree, condition $ b) $ holds, by V, p. 30, Prop. 3.

### 5. Stability properties of separable algebraic extensions

#### Proposition 8 {#alg-v-s7-prop-8 .statement}

— *Let $ E $ be an extension of $ K $ and $ (E_i)_{i \in I} $ a family of subextensions of $ E $ such that $ E = K \left( \bigcup_{i \in I} E_i \right) $. If each extension $ E_i $ is algebraic and separable over $ K $, the same is true of $ E $.*

This follows at once from Prop. 6 (V, p. 39).

$ ^1 $ The reader may convince himself that Th. 1 is used nowhere before the proof of Lemma 1 of V, p. 78.

#### Proposition 9 {#alg-v-s7-prop-9 .statement}

— *Let F be an algebraic extension of K and E a subextension of F. For F to be separable over K it is necessary and sufficient that F should be separable over E and E separable over K.*

Suppose first that F is separable over K; then E is separable over K by Prop. 1 (V, p. 36). Moreover, every element of F is separable over K (V, p. 39, Prop. 6) hence over E (V, p. 39, Cor. 2) and so F is separable over E (V, p. 39, Prop. 6).

Conversely, suppose that F is separable over E and E separable over K. Denote by x an element of F and by $ f \in E[X] $ the minimal polynomial of x over E. Since E is algebraic over K, Th. 2 (V, p. 18) shows that there exists a subextension E' of E of finite degree over K such that $ f \in E'[X] $; then f is at the same time the minimal polynomial of x over E and over E', and since x is separable over E (V, p. 39, Prop. 6) it is so also over E' (V, p. 39, Prop. 5). Write $ F' = E'(x) $; then F is separable and of finite degree over E', and since E is separable over K, E' is separable and of finite degree over K (V, p. 36, Prop. 1). Hence F is separable and of finite degree over K, by V, p. 32, Cor. 2. Therefore (V, p. 39, Prop. 6) x is separable over K. We have now shown that every element of F is separable over K, hence F is separable over K (V, p. 39, Prop. 6).

#### Proposition 10 {#alg-v-s7-prop-10 .statement}

— *Let E and K' be two subextensions of the same extension of K and let $ E' = K'(E) $. Suppose that E is algebraic over K, hence E' algebraic over K' (V, p. 18, Cor. 2).

a) *If E is separable over K, then E' is separable over K'._

b) *Conversely if E' is separable over K' and E and K' are linearly disjoint over K, then E is separable over K._

Assertion *a)* follows directly from Prop. 6 (V, p. 39).

Under the hypothesis *b)*, let F be a subextension of E of finite degree over K. Then F and K' are linearly disjoint over K, hence the K'-algebra $ F_{(K')} = K' \otimes_K F $ is isomorphic to $ K'(F) $. Since $ K'(F) $ is a subextension of E' of finite degree over K' and E' is algebraic and separable over K', the K'-algebra $ K'(F) $ is etale. In other words, the K'-algebra $ F_{(K')} $ is etale, and now Cor. 2 of Prop. 4 (V, p. 32) shows that F is etale over K. Thus we have shown E to be separable over K.

### 6. A separability criterion

#### Proposition 11 {#alg-v-s7-prop-11 .statement}

— *Suppose that K is of characteristic exponent p, and let E be an algebraic extension of K, generated by a set S. If E is separable over K, then $ E = K(S^{p^n}) $ for all integers $ n \geq 0 $; conversely if E is of finite degree over K and $ E = K(S^p) $, then E is separable over K._

The case $ p = 1 $ is trivial by the Cor. of V, p. 37. Suppose from now on that $ p \neq 1 $.

By hypothesis E is algebraic over K and we have $ E = K(S) $, hence

$$
K(S^p) = K(E^p) = K[E^p] \quad \text{by V, p.18, Cor. 1.}
$$

If E is of finite degree over K, it is a separable extension of K if and only if it is an etale algebra over K; the Cor. of V, p. 35 shows that this happens if and only if $ E = K[E^p] $.

Suppose now that $ E $ is separable and of infinite degree over $ K $. Then $ K[E^p] $ is the union of the subrings $ K[E'^p] $ where $ E' $ ranges over the set of subextensions of $ E $ of finite degree over $ K $; but such an extension $ E' $ is separable over $ K $ ($ V $, p. 36, Prop. 1), whence $ E' = K[E'^p] \subset K[E^p] $ by what has been said; finally we have $ E = K[E^p] $. By induction on $ n \geq 0 $, the relation $ E = K[E^p] $ implies that $ E = K[E^{p^n}] $.

#### Corollary 1 {#alg-v-s7-prop-11-cor-1 .statement}

— *Every algebraic extension of a perfect field is a perfect field.*

Let $ K $ be a perfect field of characteristic exponent $ p $, and let $ E $ be an algebraic extension of $ K $. Then $ E $ is separable over $ K $ ($ V $, p. 36, Prop. 2) whence $ E = K(E^p) $ by Prop. 11; but we have $ K = K^p \subset E^p $, hence $ E = K(E^p) = E^p $, and so $ E $ is perfect.

#### Corollary 2 (Mac Lane) {#alg-v-s7-prop-11-cor-2 .statement}

— *Let $ K $ be an algebraic closure of $ K $ and $ K^{p^{-\infty}} $ the perfect closure of $ K $ in $ \overline{K} $. For a subextension $ E $ of $ \overline{K} $ to be separable over $ K $ it is necessary and sufficient that it should be linearly disjoint from $ K^{p^{-\infty}} $ over $ K $.*

We can immediately reduce to the case where $ [E : K] $ is finite. Let $ (x_i)_i $, be a basis of $ E $ over $ K $. For $ E $ to be linearly disjoint from $ K^{p^{-\infty}} $ it is necessary and sufficient that it should be so from $ K^{p^n} $ for all $ n \geq 0 $, and this just means that the relation $ \sum_{i \in I} x_i a_i^{p^{-n}} = 0 $ implies $ a_i = 0 $ for all $ i \in I $, for any family $ (a_i)_i $, of elements of $ K $. This in turn means that the family $ (x_i^{p^n})_{i \in I} $ is free over $ K $, or also that it is a basis of the vector space $ E $ over $ K $. Put differently, $ E $ is linearly disjoint from $ K^{p^{-n}} $ if and only if $ E = K(E^{p^n}) $. Now it suffices to apply Prop. 11.

#### Remark {#alg-v-s7-n6-rem-1 .statement}

— 1) When $ E $ is algebraic and of infinite degree over $ K $, the condition $ E = K(E^p) $ does not always ensure that $ E $ is separable over $ K $. For example, if $ K $ is imperfect and $ E $ is a perfect closure of $ K $, then we have $ E = K(E^p) $ but $ E $ is not a separable extension of $ K $ ($ V $, p. 39, Cor. 3).
2) Let $ E $ a separable algebraic extension of a field $ K $ of characteristic exponent $ p $. Then we have $ E^p \cap K = K^p $ (Cor. 2); therefore if $ E $ is perfect, the same is true of $ K $.

### 7. The relative separable algebraic closure

#### Proposition 12 {#alg-v-s7-prop-12 .statement}

— *Let $ E $ be an extension of $ K $ and $ E_s $, the set of elements of $ E $ which are algebraic and separable over $ K $. Then $ E_s $, is the largest subextension of $ E $ which is algebraic and separable over $ K $.*

By Prop. 6, *a*) ($ V $, p. 39) every subextension of $ E $ which is algebraic and separable over $ K $ is contained in $ E_s $. By Prop. 6, *b*) (*loc. cit.*) the extension $ K(E_s) $ of $ K $ is algebraic and separable, whence $ K(E_s) \subset E $, and so $ K(E_s) = E_s $.

With the notation of the preceding proposition, E, is called the relative separable (algebraic) closure of K in E. When K is perfect, E, is the relative algebraic closure of K in E (V, p. 36, Prop. 2).

#### Proposition 13 {#alg-v-s7-prop-13 .statement}

— Let E be an algebraic extension of K and let E,, be the relative separable algebraic closure of K in E.
a) E is a p-radical extension of E,.
b) If F is a subextension of E such that E is p-radical over F, then F ⊃ E,.
c) E, is the unique subextension of E which is separable over K and over which E is p-radical.
It suffices to prove a) in the case where K is of characteristic $ p \neq 0 $. Let x be an element of E and f its minimal polynomial over K. There exists an integer $ m \geq 0 $ such that f belongs to $ K[X^{p^m}] $ but not to $ K[X^{p^{m+1}}] $; in other words, we have $ f(X) = g(X^{p^m}) $ with $ g \in K[X] $, $ g \notin K[X^p] $. Since f is irreducible, the same is true of g, hence g is the minimal polynomial of $ x^{p^m} $ over K. By V, p. 38, Prop. 4 and p. 39, Prop. 5 we thus have $ x^{p^m} \in E_s $, so E is p-radical over E,.

Assume now the hypothesis b) and let $ x \in E, $. Since x is separable over K, it is so also over F (V, p. 39, Cor. 2), but since E is p-radical over F, x is also p-radical over F, hence $ x \in F $ (V, p. 39, Cor. 3).

Finally c) follows from a) and b) and Prop. 12.

#### Corollary 1 {#alg-v-s7-prop-13-cor-1 .statement}

— Let E and K' be two extensions of K contained in the same extension of K. Suppose that E is algebraic over K and denote by E, the relative separable algebraic closure of K in E. Then $ K'(E_s) $ is the relative separable algebraic closure of K' in $ K'(E) $.

For $ K'(E_s) $ is a separable algebraic extension of K' by Prop. 10 (V, p. 42); since E is p-radical over E,, the extension $ K'(E) $ of $ K'(E_s) $ is p-radical (V, p. 25, Cor.). Now it suffices to apply Prop. 13.

#### Corollary 2 {#alg-v-s7-prop-13-cor-2 .statement}

— If E has finite degree over K, then $ E_s = \bigcap_{n \geq 0} K(E^{p^n}) $.

For each integer $ n \geq 0 $ denote by F, the subextension $ K(E^{p^n}) $ of E. The sequence $ (F_n)_{n \geq 0} $ of vector subspaces of E is descending and E is of finite dimension over K. Hence there exists an integer $ m \geq 0 $ such that $ F_m = F_n $ for all $ n \geq m $. We thus have $ K(F_m^p) = F_{m+1} = F_m $, hence $ F_m $ is a separable extension of K (V, p. 42, Prop. 11); it is clear that E is p-radical over F, and so Prop. 13 implies $ E_s = F_m = \bigcap_{n \geq 0} F_n $.

#### Remark {#alg-v-s7-n7-rem-1 .statement}

— Let E be an algebraic extension of K and E, the relative p-radical closure of E in K (V, p. 25). Then E, is the largest subextension of E which is p-radical over K (V, p. 25, Prop. 2). However, E is in general not separable over E, (V, p. 152, Ex. 2); for the case of quasi-Galois extensions see V, p. 76.

### 8. The separable closure of a field

#### Definition 4 {#alg-v-s7-def-4 .statement}

— *A field K is said to be separably closed if every separable algebraic extension of K is trivial.*

An algebraically closed field is separably closed. Conversely, if a perfect field K is separably closed, it is algebraically closed, because every algebraic extension of K is separable (*V*, p. 3 , Prop. 2).

#### Definition 5 {#alg-v-s7-def-5 .statement}

— *Let K be a field. By a separable algebraic closure, or (by abuse of language) separable closure of K we understand any extension E of K which is algebraic and separable over K, and such that the field E is separably closed.*

When K is perfect, there is complete identity between the notions of separable closure and algebraic closure of K (*V*, p. 36, Prop. 2 and p. 43, Cor. 1).

#### Proposition 14 {#alg-v-s7-prop-14 .statement}

— *Let Ω be an algebraically closed extension of K.*

a) *The relative separable algebraic closure Ω_s of K in Ω is a separable closure of K.*

b) *If E and E' are two separable closures of K, there exists a K-isomorphism of E onto E'._

Let F be a separable algebraic extension of Ω_s ; since Ω is algebraically closed, there exists an 0,-homomorphism u of F into Ω (*V*, p. 20, Th. 1). By Prop. 9 (V, p. 42) $ u(F) $ is separable over K, hence $ u(F) = \Omega_s $. Therefore F is a trivial extension of $ \Omega_s $ and so $ \Omega_s $ is separably closed, whence *a)*.

Let E be a separable closure of K. Since E is an algebraic extension of K, there exists a K-homomorphism v of E into Ω (*V*, p. 20, Th. 1). Hence $ v(E) $ is separable algebraic over K, whence $ v(E) \subset \Omega_s $. By *V*, p. 42, Prop. 9, $ \Omega_s $ is separable over $ v(E) $ and since the field $ v(E) $ is separably closed, we have $ v(E) = \Omega_s $. It follows that v is a K-isomorphism of E onto $ \Omega_s $. Now *b)* is an immediate consequence.

#### Corollary {#alg-v-s7-n8-cor-1 .statement}

— *Let E be a separably closed extension of K and F a separable algebraic extension of K ; then there exists a K-homomorphism of F into E._

Let Ω be an algebraic closure of E ; we have $ \Omega_s \subset E $ and it suffices to treat the case where $ E = \Omega_s $. Since F is an algebraic extension of K, there exists a K-homomorphism u of F into Ω (*V*, p. 20, Th. 1). Since the field $ u(F) $ is separable over K, we have $ u(F) \subset \Omega_s $ and u defines a K-homomorphism of F into $ \Omega_s = E $.

#### Remark {#alg-v-s7-n8-rem-1 .statement}

— 1) Let E and E' be two separable closures of K. If K is not separably closed, there exist several K-isomorphisms of E onto E'. \* For E is then a non-trivial Galois extension of K, and so there exist K-automorphisms of E distinct from the identity (*V*, p. 56, Th. 1).
\* 2) Let E be an algebraic and separable extension of K. If every algebraic and separable extension of K is isomorphic to a subextension of E, then E is a separable closure of K. For if E' is a separable closure of K, then each of the extensions E and E' is isomorphic to a subextension of the other; hence E and E' are isomorphic extensions of K (V, p. 52, Prop. 1, a)).

### 9. Separable and inseparable degrees of an extension of finite degree

Let E be an extension of finite degree of K and $ \Omega $ an algebraic closure of K. Recall (V, p. 31) that by the *separable degree* of E over K, written $[E : K]_s$, we understand the number of K-homomorphisms of E into $ \Omega $.

#### Proposition 15 {#alg-v-s7-prop-15 .statement}

*Let E, be the relative separable closure of K in E; then* $[E : K]_s = [E_s : K]$.

The field $ \Omega $ is perfect and E is p-radical over $ E_s $, by V, p. 44, Prop. 13; therefore Prop. 3 (V, p. 26) shows that every K-homomorphism of E, into $ \Omega $ extends in a unique fashion to a K-homomorphism of E into $ \Omega $; we thus have $[E : K]_s = [E_s : K]$. Since E, is a separable extension of finite degree of K, it is an etale algebra over K; so we have $[E_s : K]_s = [E_s : K]$ by V, p. 32, Prop. 4, and the result follows.

With the preceding notation, the degree of E over $ E_s $ is called the *inseparable degree* of E over K and is denoted by $[E : K]_i$. We thus have

(1)
$$
[E : K] = [E : K]_s \cdot [E : K]_i
$$
by Prop. 15.

When K is of characteristic 0, then $ E = E_s $, and so $[E : K]_s = [E : K]$ and $[E : K]_i = 1$. If K is of characteristic $ p \neq 0 $, the number $[E : K]_i$ is a power of p because E is p-radical over $ E_s $ (V, p. 44, Prop. 13 and p. 26, Prop. 4). It should be noted that $[E : K]_i$ is not necessarily equal to the highest power of $ p $ dividing $[E : K]_s$, nor equal to the degree $[E_s : K]$ of the relativep-radical closure of E in K (V, p. 152, Ex. 3 and 2).

#### Proposition 16 {#alg-v-s7-prop-16 .statement}

*Let $ \Omega $ be an extension of K and E, F two subextensions of $ \Omega $, of finite degree over K.*

a) *If $ E \subset F $, then* $[F : K]_s = [F : E]_s \cdot [E : K]_s$, *and* $[F : K]_i = [F : E]_i \cdot [E : K]_i$.

b) *Let $ K' $ be a subextension of $ \Omega $; then we have*
$$
[K'(E) : K']_s \leq [E : K]_s \quad \text{and} \quad [K'(E) : K']_i \leq [E : K]_i,
$$
*and equality holds if $ K' $ is linearly disjoint from E over K.*

c) *We have* $[K(E \cup F) : K]_s \leq [E : K]_s \cdot [F : K]_s$, *and* $[K(E \cup F) : K]_i \leq [E : K]_i \cdot [F : K]_i$, *and equality holds if E and F are linearly disjoint over K*.

The assertion about the separable degrees in a) follows from (9) (V, p. 32). Since $[F : K] = [F : E] \cdot [E : K]$, the assertion about the inseparable degrees follows from this and (1).

By Cor. 1 of Prop. 13 (V, p. 44) and Prop. 15, we have

(2) $$ [K'(E) : K']_s = [K'(E_s) : K'] , \quad [K'(E) : K']_i = [F'(E) : K'(E_s)] ; $$

when K' is linearly disjoint from E over K, then E, is linearly disjoint from K' over K and E is linearly disjoint from K'(E_s) over E_s (V, p. 15, Prop. 8). Assertion b) now follows from Prop. 5 (V, p. 14).

By a) we have $$ [K(E \cup F) : K] = [F(E) : F] . [F : K]_s ; $$ by b) we have $$ [F(E) : F] , \leq [E : K] , \text{ with equality if } E \text{ and } F \text{ are linearly disjoint over } K. $$ Hence we obtain the inequality $$ [K(E \cup F) : K] , \leq [E : K] , . [F : K] , \text{ with equality if } E \text{ and } F \text{ are linearly disjoint over } K. $$ The assertion of c) about the inseparable degrees is proved in a similar fashion.

### Exercises {#alg-v-s7-exercises}

See the [exercises for § 7](exercises/s7/).
