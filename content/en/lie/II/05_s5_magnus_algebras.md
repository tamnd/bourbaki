---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: II
chapter_title: FREE LIE ALGEBRAS
section: 5
section_title: Magnus algebras
lang: en
source: lie-i-iii
pdf_pages: 0167-0173, 0211-0219
extraction: ocr
subsections:
    - "no": 1
      title: MAGNUS ALGEBRAS
      page: 0
      pdf_page: 167
    - "no": 2
      title: MAGNUS GROUP
      page: 0
      pdf_page: 168
    - "no": 3
      title: MAGNUS GROUP AND FREE GROUP
      page: 0
      pdf_page: 169
    - "no": 4
      title: LOWER CENTRAL SERIES OF A FREE GROUP
      page: 0
      pdf_page: 170
    - "no": 5
      title: '*p*-Filtration of Free Groups'
      page: 0
      pdf_page: 172
statements: 14
exercises: 12
content_sha256: bad4e74403951e94fae22d37f0f1addf30ea18902739a7d9f01afac7e6586a5b
---

## § 5. MAGNUS ALGEBRAS

In this paragraph, X denotes a set, F(X) the free group constructed on X (Algebra, Chapter I, \S 7, no. 5) and A(X) the free associative algebra constructed on X with its total graduation $ (A^n(X))_{n \geq 0} $ (cf. Algebra, Chapter III, \S 3, no. 1, Example 3). X is identified with its images in F(X) and A(X).

### 1. MAGNUS ALGEBRAS

Let $ \hat{A}(X) $ be the product module $ \prod_{n \geq 0} A^n(X) $. We define on $ \hat{A}(X) $ a multiplication by the rule

$$
(a \cdot b)_n = \sum_{i=0}^n a_i \cdot b_{n-i}
$$

where $ a = (a_n) $ and $ b = (b_n) $ are in $ \hat{A}(X) $. We know (Commutative Algebra, Chapter III, \S 2, no. 12, Example 1) that $ \hat{A}(X) $ is an associative algebra and that $ A(X) $ is identified with the subalgebra of $ \hat{A}(X) $ consisting of the sequence all of whose terms are zero except for a finite number.

$ \hat{A}(X) $ is given the product topology of the discrete topologies on the factors

A^n(X); this topology makes $ \hat{A}(X) $ into a complete Hausdorff topological algebra, when the ring K has the discrete topology, and $ A(X) $ is dense in $ \hat{A}(X) $

Let $ a = (a_n) \in \hat{A}(X) $; the family $ (a_n)_{n \geq 0} $ is summable and $ a = \sum_{n \geq 0} a_n $.

For every integer $ m \geq 0 $, let $ \hat{A}_m(X) $ denote the ideal consisting of the series $ a = \sum_{n \geq m} a_n $ such that $ a_n \in A^n(X) $ for all $ n \geq m $. This sequence of ideals is a fundamental system of neighbourhoods of 0 in $ \hat{A}(X) $ and an integral filtration on $ \hat{A}(X) $. The order function associated with the above filtration is denoted by $ \omega $; then $ \omega(0) = +\infty $ and $ \omega(a) = m $ if $ a = \sum_{n \geq m} a_n $ with $ a_n \in A^n(X) $ for all $ n \geq m $ and $ a_m \neq 0 $ (\S 4, nos. 1 and 2).

$ \hat{A}(X) $ is called the *Magnus algebra* of the set X with coefficients in K. If there is any ambiguity over K we write $ \hat{A}_K(X) $.

#### Proposition 1 {#lie-ii-s5-prop-1 .statement}

*Let B be a unital associative algebra with a real filtration $ (B_\alpha)_{\alpha \in \mathbf{R}} $ such that B is Hausdorff and complete (\S 4, nos. 1 and 2). Let f be a mapping of X into B such that there exists $ \lambda > 0 $ for which $ f(X) \subset B_\lambda $. Then f can be extended in one and only one way to a continuous unital homomorphism $ \hat{f} $ of $ \hat{A}(X) $ into B.*

Let $ f' $ be the unique unital algebra homomorphism of $ A(X) $ into B extending $ f $ (*Algebra*, Chapter III, \S 2, no. 7, Proposition 7). We show that $ f' $ is *continuous*: $ f'(A^n(X)) \subset B_{n\lambda} $ whence $ f'(\hat{A}_n(X) \cap A(X)) \subset B_{n\lambda} $. Therefore $ f' $ can be extended in one and only one way by continuity to a homomorphism $ \hat{f} : \hat{A}(X) \to B $.

We preserve the hypotheses and notation of Proposition 1 and let $ u \in \hat{A}(X) $. The element $ \hat{f}(u) $ is denoted by $ u((f(x))_{x \in X}) $ and called the *result of substituting the f(x) for the x in u*. In particular, $ u((x)_{x \in X}) = u $. Now let $ u = (u_y)_{y \in Y} $ be a family of elements of $ \hat{A}_1(X) $ and let $ v \in \hat{A}(Y) $. The above allows us to define the element $ v((u_y)_{y \in Y}) \in \hat{A}(X) $. It is denoted by $ v \circ u $. As $ u_y((f(x))) \in B_\lambda $, the elements $ u_y((f(x))) $ can be substituted for the y in v. The mappings $ v \mapsto (v \circ u)((f(x))) $ and $ v \mapsto v((u_y((f(x)))))) $ are then two continuous homomorphisms of unital algebras of $ \hat{A}(X) $ into B taking the same value $ u_y((f(x))) $ at the element $ y \in Y $. Therefore (Proposition 1)

$$
(v \circ u)((f(x))) = v((u_y((f(x))))))
$$

for all $ v \in \hat{A}(Y) $.

### 2. MAGNUS GROUP

For all $ a = (a_n)_{n \geq 0} $ in $ \hat{A}(X) $, the element $ a_0 $ of K will be called the *constant term* of a and denoted by $ \varepsilon(a) $. Formula (1) shows that $ \varepsilon $ is an algebra homomorphism of $ \hat{A}(X) $ into K.

#### Lemma 1 {#lie-ii-s5-lem-1 .statement}

*For an element a of $ \hat{A}(X) $ to be invertible, it is necessary and sufficient that its constant term be invertible in K.*

If $ a $ is invertible in $ \hat{\mathbf{A}}(\mathbf{X}) $, $ \varepsilon(a) $ is invertible in $ K $. Conversely, if $ \varepsilon(a) $ is invertible in $ K $, there exists $ u \in \hat{\mathbf{A}}_1(\mathbf{X}) $ such that $ a = \varepsilon(a)(1-u) $; we write $ b = \left( \sum_{n \geq 0} u^n \right) \varepsilon(a)^{-1} $. Then $ ab = ba = 1 $ and $ a $ is invertible.

The set of elements of $ \hat{\mathbf{A}}(\mathbf{X}) $ of constant term 1 is therefore a subgroup of the multiplicative monoid $ \hat{\mathbf{A}}(\mathbf{X}) $, called the *Magnus group* constructed on $ \mathbf{X} $ (relative to $ K $). In this chapter it will be denoted by $ \Gamma(\mathbf{X}) $ or simply $ \Gamma $. For every integer $ n \geq 1 $, we denote by $ \Gamma_n $ the set of $ a \in \Gamma $ such that $ \omega(a-1) \geq n $. By Proposition 2 of § 4, no. 5, the sequence $ (\Gamma_n)_{n \geq 1} $ is an *integral central filtration on $ \Gamma $*.

### 3. MAGNUS GROUP AND FREE GROUP

#### Theorem 1 {#lie-ii-s5-thm-1 .statement}

*Let $ r $ be a mapping of $ \mathbf{X} $ into $ \hat{\mathbf{A}}(\mathbf{X}) $ such that $ \omega(r(x)) \geq 2 $ for all $ x \in \mathbf{X} $. The unique homomorphism $ g $ of the free group $ F(\mathbf{X}) $ into the Magnus group $ \Gamma(\mathbf{X}) $ such that $ g(x) = 1 + x + r(x) $ for all $ x \in \mathbf{X} $ is injective.*

We first prove three lemmas.

#### Lemma 2 {#lie-ii-s5-lem-2 .statement}

*Let $ n $ be a non-zero rational integer. In the ring of formal power series $ K[[t]] $ we write $ (1+t)^n = \sum_{j \geq 0} c_{j,n} t^j $. There exists an integer $ j \geq 1 $ such that $ c_{j,n} \neq 0 $.

If $ n > 0 $, then $ c_{n,n} = 1 $ by the binomial formula.
Suppose that $ n < 0 $ and let $ m = -n $. If $ c_{j,n} = 0 $ for all $ j \geq 1 $, then $ (1+t)^n = 1 $, whence, taking the inverse, $ (1+t)^m = 1 $, which contradicts the formula $ c_{m,m} = 1 $.*

#### Lemma 3 {#lie-ii-s5-lem-3 .statement}

*Let $ x_1, \ldots, x_s $ be elements of $ \mathbf{X} $ such that $ s \geq 1 $ and $ x_i \neq x_{i+1} $ for $ 1 \leq i \leq s-1 $; let $ n_1, \ldots, n_s $ be non-zero rational integers. Then the element $ \prod_{i=1}^s (1+x_i)^{n_i} $ of $ \hat{\mathbf{A}}(\mathbf{X}) $ is $ \neq 1 $.

Let $ m $ be a maximal ideal of $ K $ and $ k $ the field $ K/m $; let $ p : \hat{\mathbf{A}}_K(\mathbf{X}) \to \hat{\mathbf{A}}_k(\mathbf{X}) $ be the unique continuous homomorphism of unital $ K $-algebras such that $ p(x) = x $ for $ x \in \mathbf{X} $ (no. 1, Proposition 1). It suffices to prove that $ p\left( \prod_{i=1}^s (1+x_i)^{n_i} \right) \neq 1 $ and the problem is reduced to the case where $ K $ is a field.

In the notation of Lemma 2:

$$
\prod_{i=1}^s (1+x_i)^{n_i} = \sum_{b_1 \geq 0} \cdots \sum_{b_s \geq 0} c_{b_1, n_1} \cdots c_{b_s, n_s} x_1^{b_1} \cdots x_s^{b_s}.
$$

By Lemma 2, there exist integers $ a_i > 0 $ such that $ c_{a_i, n_i} \neq 0 $ ($ 1 \leq i \leq s $). By *Algebra*, Chapter I, § 7, no. 4, Proposition 6, no monomial $ x_1^{b_1} \cdots x_s^{b_s} $ such that $ b_i \geq 0 $ and $ (b_1, \ldots, b_s) \neq (a_1, \ldots, a_s) $ can be equal to $ x_1^{a_1} \ldots x_s^{a_s} $. It follows that the coefficient of $ x_1^{a_1} \ldots x_s^{a_s} $ in $ \prod_{i=1}^s (1 + x_i)^{n_i} $ is $ c_{a_1, n_1} \ldots c_{a_s, n_s} \neq 0 $, which implies the result.

#### Lemma 4 {#lie-ii-s5-lem-4 .statement}

*Let $ \sigma $ be the continuous endomorphism of $ \hat{A}(X) $ such that $ \sigma(x) = x + r(x) $ for $ x \in X $ (no. 1, Proposition 1). Then $ \sigma $ is an automorphism and $ \sigma(\hat{A}_m(X)) = \hat{A}_m(X) $ for all $ m \in \mathbf{N} $.

$ \sigma(x) \equiv x \mod \hat{A}_2(X) $ for $ x \in X $, whence, for $ n \geq 1 $ and $ x_1, \ldots, x_n $ in $ X $,
$$
\sigma(x_1) \ldots \sigma(x_n) \equiv x_1 \ldots x_n \mod \hat{A}_{n+1}(X);
$$
it follows by linearity that $ \sigma(a) \equiv a $ modulo $ \hat{A}_{n+1}(X) $ for all $ a \in A^n(X) $ and in particular $ \sigma(A^n(X)) \subset \hat{A}_n(X) $. It follows that $ \sigma(A^n(X)) \subset \hat{A}_n(X) $ for $ m \geq n $, whence $ \sigma(\hat{A}_n(X)) \subset \hat{A}_n(X) $. In other words, $ \sigma $ is compatible with the filtration $ (\hat{A}_m(X)) $ on $ A(X) $ and its restriction to the associated graded ring is the identity. Hence $ \sigma $ is bijective (*Commutative Algebra*, Chapter III, § 2, no. 8, Corollary 3 to Theorem 1).

Finally we prove Theorem 1. Let $ w \neq 1 $ be an element of $ F(X) $. By *Algebra*, Chapter I, § 7, no. 5, Proposition 7, there exist $ x_1, \ldots, x_s $ in $ X $ and non-zero rational integers $ n_1, \ldots, n_s $ such that $ s \geq 1 $, $ x_i \neq x_{i+1} $ ($ 1 \leq i \leq s-1 $) and
$$
w = x_1^{n_1} \ldots x_s^{n_s}.
$$
In the notation of Lemma 4,
$$
g(w) = \prod (1 + \sigma(x_i))^{n_i} = \sigma(\prod (1 + x_i)^{n_i}),
$$
hence $ g(w) \neq 1 $ by Lemmas 3 and 4.

### 4. LOWER CENTRAL SERIES OF A FREE GROUP

We shall prove the two following theorems:

#### Theorem 2 {#lie-ii-s5-thm-2 .statement}

*Suppose that in the ring $ K $ the relation $ n.1 = 0 $ implies $ n = 0 $ for every integer $ n $. Let $ r $ be a mapping of $ X $ into $ \hat{A}(X) $ such that $ \omega(r(x)) \geq 2 $ for $ x \in X $ and let $ g $ be the homomorphism of $ F(X) $ into the Magnus group $ \Gamma(X) $ such that $ g(x) = 1 + x + r(x) $ for $ x \in X $. For all $ n \geq 1 $, $ C^n F(X) $ is the inverse image under $ g $ of the subgroup $ 1 + \hat{A}_n(X) $ of $ \Gamma(X) $.*

#### Theorem 3 {#lie-ii-s5-thm-3 .statement}

*For all $ x \in X $, let $ c(x) $ be the canonical image of $ x $ in $ F(X)/(F(X), F(X)) $. Let $ g $ be the graded Lie $ \mathbf{Z} $-algebra associated with the filtration $ (C^n F(X))_{n \geq 1} $ of $ F(X) $ (§ 4, no. 6). The unique homomorphism of the free Lie $ \mathbf{Z} $-algebra $ L_\mathbf{Z}(X) $ into $ g $ which extends $ c $ is an isomorphism.*

Loosely speaking, the graded Lie $ \mathbf{Z} $-algebra associated with the free group $ F(X) $ (with the lower central series) is the free Lie $ \mathbf{Z} $-algebra $ L_\mathbf{Z}(X) $.

We write $ F(X) = F, \Gamma(X) = \Gamma, \hat{A}(X) = \hat{A}, \hat{A}_\mathbf{Z}(X) = \hat{A}_\mathbf{Z}, C^n F(X) = C^n, \Gamma_n = 1 + \hat{A}_n(X) $ and let $ \alpha : L_\mathbf{Z}(X) \to g $ be the homomorphism introduced in the statement of Theorem 3.

(A) Preliminary reductions.

Let $ \gamma $ denote the homomorphism of $ F $ into $ \Gamma $ defined by $ \gamma(x) = 1 + x $ for $ x \in X $. By Lemma 4 there exists an automorphism $ \sigma $ of the algebra $ \hat{A} $ compatible with the filtration on $ \hat{A} $ and such that $ \sigma(1 + x) = g(x) $ for all $ x \in X $; then $ \sigma(\Gamma_n) = \Gamma_n $ for all $ n $. As the homomorphisms $ g $ and $ \sigma \circ \gamma $ of $ F $ into $ \Gamma $ coincide on $ X, g = \sigma \circ \gamma $ and hence $ g^{-1}(\Gamma_n) = \gamma^{-1}(\Gamma_n) $. Under the hypotheses of Theorem 2, $ \mathbf{Z} $ can be identified with a subring of $ K $; the Magnus algebra $ \hat{A}_\mathbf{Z} $ is therefore identified with a subring of $ \hat{A} $ and the filtration on $ \hat{A}_\mathbf{Z} $ is induced by that on $ \hat{A} $. As $ \gamma $ maps $ F $ into $ \hat{A}_\mathbf{Z} $, we see that it suffices to prove Theorems 2 and 3 under the supplementary hypotheses $ K = \mathbf{Z}, r = 0 $ and hence $ g = \gamma $, hypotheses which we shall henceforth make.

(B) Surjectivity of $ \alpha $.

As $ X $ generates the group $ F = C^1 $, the set $ c(X) $ generates the $ \mathbf{Z} $-module $ g^1 = C^1/C^2 $. But $ g^1 $ generates the Lie $ \mathbf{Z} $-algebra $ g $ (\S 4, no. 6, Proposition 5) and hence $ c(X) $ generates $ g $, which proves that $ \alpha $ is surjective.

(C) We identify the graded algebra $ \mathrm{gr}(\hat{A}) $ with $ A(X) $ under the canonical isomorphisms $ A^n(X) \to \hat{A}_n/\hat{A}_{n+1} $. For every integer $ n \geq 1 $, we write $ F^n = \gamma^{-1}(\Gamma_n) $; we know (\S 4, no. 5) that $ (F^n)_{n \geq 1} $ is an integral central filtration on $ F $. Let $ g' $ denote the associated graded Lie $ \mathbf{Z} $-algebra (\S 4, no. 4). Let $ f $ be the Lie algebra homomorphism of $ g' $ into $ A(X) $ associated with $ \gamma $ (\S 4, no. 5, Proposition 3). Now $ C^n \subset F^n $ for every integer $ n \geq 1 $ (\S 4, no. 6, Proposition 4) and hence there is a canonical homomorphism $ \varepsilon $ of $ g = \bigoplus_{n \geq 1} C^n/C^{n+1} $ into $ g' = \bigoplus_{n \geq 1} F^n/F^{n+1} $

$$
L_\mathbf{Z}(X) \xrightarrow{\alpha} g \xrightarrow{\varepsilon} g' \xrightarrow{f} A(X).
$$

We write $ \beta = f \circ \varepsilon $; we give $ \beta $ explicitly as follows: if $ u $ is the class modulo $ C^{n+1} $ of an element $ w $ of $ C^n $, then $ \gamma(w) - 1 $ is of order $ \geq n $ in $ \hat{A} $ and $ \beta(u) $ is the homogeneous component of $ \gamma(w) - 1 $ of degree $ n $. In particular,

$$
\beta(c(x)) = x \quad \text{for all } x \in X.
$$

(D) Proof of Theorems 2 and 3.

The Lie algebra homomorphism $ \beta \circ \alpha : L_\mathbf{Z}(X) \to A(X) $ restricted to $ X $ is the identity by (3) and hence is the canonical injection (\S 3, no. 1). Therefore $ \alpha $ is injective and hence bijective by (B); this proves Theorem 3. As $ \beta \circ \alpha = f \circ \varepsilon \circ \alpha $ is injective and $ \alpha $ is bijective, $ \varepsilon $ is injective. For all $ n \geq 1 $,

$$
\varepsilon_n : C^n/C^{n+1} \to F^n/F^{n+1}
$$

is injective and hence

$$
C^n \cap F^{n+1} = C^{n+1}.
$$

C^1 = F = F^1; if C^n = F^n, then C^n \cap F^{n+1} = F^{n+1} whence C^{n+1} = F^{n+1}
which proves Theorem 2 by induction on n \geqslant 1.

#### Corollary {#lie-ii-s5-n4-cor-1 .statement}

$$
\bigcap_{n \geqslant 1} C^n F(X) = \{e\}.
$$

Applying Theorem 2 with K = \mathbf{Z} and r = 0,
$$
\bigcap_{n \geqslant 1} C^n F(X) = \bigcap_{n \geqslant 1} g^{-1}(1 + \hat{A}_n(X)) = g^{-1}\left(\bigcap_{n \geqslant 1} (1 + \hat{A}_n(X))\right) = g^{-1}(1) = \{e\}.
$$

#### Remark {#lie-ii-s5-n4-rem-1 .statement}

Let H be a Hall set relative to X (\S 2, no. 10). Let M be the magma defined by the law of composition (x, y) \mapsto (x, y) = x^{-1}y^{-1}xy on F(X) and let $ \phi $ be the homomorphism of M(X) into M whose restriction to X is the identity. The elements of $ \phi(H) $ are called the *basic commutators* of F(X) associated with the Hall set H. For every integer n \geqslant 1, let H_n be the subset of H consisting of the elements of length n; we know (\S 2, no. 11, Theorem 1) that the canonical mapping of H_n into L_\mathbf{Z}(X) is a basis of the Abelian group L_\mathbf{Z}^n(X). Moreover, $ \phi(H_n) \subset C^n $; for all m \in H_n, let $ \phi_n(m) $ denote the class mod. C^{n+1} of $ \phi(m) \in C^n $. Theorem 3 then shows that $ \phi_n $ is *a bijection of H_n onto a basis of the Abelian group* C^n/C^{n+1}. It follows immediately that, for all w \in F(X) and all i \geqslant 1, there exists a unique element $ \alpha_i $ of $ \mathbf{Z}^{(H_i)} $ such that, for n \geqslant 1,

$$
w = \prod_{i=1}^n \prod_{m \in H_i} \phi(m)^{\alpha_i(m)} \mod. C^{n+1},
$$

where the product is calculated according to the total ordering given on H.

#### Example {#lie-ii-s5-n4-exa-1 .statement}

Suppose that X is a set with two elements x, y and let H_1 = \{x, y\}, H_2 = \{xy\}. Every element w of F(X) can therefore be written
$$
w \equiv x^a y^b (x, y)^c \mod. C^3 \quad \text{with } a, b, c \text{ in } \mathbf{Z}.
$$
For w = (xy)^n, a = b = n and c = n(1 - n)/2 (cf. Exercise 9), whence
$$
(xy)^n \equiv x^n y^n (x, y)^{n(1-n)/2} \mod. C^3.
$$

### 5. *p*-Filtration of Free Groups

In this no., *p* denotes a prime number and we assume that K = \mathbf{F}_p. Let $ \gamma $ be the homomorphism of F(X) into $ \Gamma(X) $ defined by $ \gamma(x) = 1 + x $ for x in X; we write $ F_n^{(p)}(X) = \gamma^{-1}(1 + \hat{A}_n(X)) $. The sequence $ (F_n^{(p)}(X))_{n \geqslant 1} $ is an integral central filtration on F(X), which is *separated* since $ \gamma $ is injective (no. 3, Theorem 1). It is called the *p*-filtration on F(X).

#### Proposition 2 {#lie-ii-s5-prop-2 .statement}

*Suppose that X is finite. For every integer n \geqslant 1, the group F(X)/F_n^{(p)}(X) is a finite p-group of nilpotency class \leqslant n.*

Arguing by induction on $ n $, it suffices to prove that $ F_n^{(p)}(X)/F_{n+1}^{(p)}(X) $ is a finite commutative $ p $-group for all $ n \geqslant 1 $. For all $ w \in F_n^{(p)}(X) $, the element $ \gamma(w) - 1 $ of $ \hat{A}(X) $ is of order $ \geqslant n $; we denote by $ \delta_n(w) $ the homogeneous component of $ \gamma(w) - 1 $ of degree $ n $. The mapping $ \delta_n : F_n^{(p)}(X) \to A^n(X) $ is a homomorphism with kernel $ F_{n+1}^{(p)}(X) $ (\S 4, no. 5, Proposition 3) and hence $ F_n^{(p)}(X)/F_{n+1}^{(p)}(X) $ is isomorphic to a subgroup of $ A^n(X) $. Since $ X $ is finite, $ A^n(X) $ is a finite-dimensional vector space over $ \mathbf{F}_p $ and hence a finite commutative $ p $-group and so is $ F_n^{(p)}(X)/F_{n+1}^{(p)}(X) $.

#### Proposition 3 {#lie-ii-s5-prop-3 .statement}

*For all $ w \neq 1 $ in $ F(X) $, there exist a finite $ p $-group $ G $ and a homomorphism $ f $ of $ F(X) $ into $ G $ such that $ f(w) \neq 1 $.*

There exist elements $ x_1, \ldots, x_r $ of $ X $ and integers $ n_1, \ldots, n_r $ such that $ w = x_1^{n_1} \ldots x_r^{n_r} $. Let $ Y = \{x_1, \ldots, x_r\} $. The canonical injection of $ Y $ into $ X $ extends to a homomorphism $ \alpha : F(Y) \to F(X) $; on the other hand, let $ \beta $ be the homomorphism of $ F(X) $ into $ F(Y) $ whose restriction to $ Y $ is the identity and which maps $ X - Y $ to $ \{1\} $. Then $ \beta(\alpha(y)) = y $ for $ y \in Y $ and hence $ \beta \circ \alpha $ is the identity automorphism of $ F(Y) $. There obviously exists $ w' $ in $ F(Y) $ such that $ w = \alpha(w') $; then $ \beta(w) = w' \neq 1 $; now $ \bigcap_{n \geqslant 1} F_n^{(p)}(Y) = \{1\} $ and there therefore exists an integer $ n \geqslant 1 $ such that $ \beta(w) \notin F_n^{(p)}(Y) $. By Proposition 2, the group $ G = F(Y)/F_n^{(p)}(Y) $ is a finite $ p $-group. If $ f $ is the composition of $ \beta $ and the canonical homomorphism of $ F(Y) $ onto $ G $, then $ f(w) \neq 1 $.

#### Corollary {#lie-ii-s5-n5-cor-1 .statement}

*The intersection of the normal subgroups of finite index in $ F(X) $ is $ \{1\} $.*

### Exercises {#lie-ii-s5-exercises}

In the following exercises we assume the hypotheses and notation of § 5. $ F $ denotes the free group $ F(X) $ and $ g $ the unique homomorphism of $ F $ into the Magnus group $ \Gamma(X) $ such that $ g(x) = 1 + x $ for all $ x \in X $ (cf. Theorem 1).

See the [exercises for § 5](exercises/s5/).
