---
book: top
book_title: General Topology
chapter: X
chapter_title: Function spaces
section: 3
section_title: Special function spaces
lang: en
source: top-v-x
pdf_pages: 0299-0314, 0333-0343
extraction: ocr
subsections:
    - "no": 1
      title: SPACES OF MAPPINGS INTO A METRIC SPACE
      page: 0
      pdf_page: 299
    - "no": 2
      title: SPACES OF MAPPINGS INTO A NORMED SPACE
      page: 0
      pdf_page: 301
    - "no": 3
      title: COUNTABILITY PROPERTIES OF SPACES OF CONTINUOUS FUNCTIONS
      page: 0
      pdf_page: 304
    - "no": 4
      title: THE COMPACT-OPEN TOPOLOGY
      page: 0
      pdf_page: 306
    - "no": 5
      title: TOPOLOGIES ON GROUPS OF HOMEOMORPHISMS
      page: 0
      pdf_page: 311
statements: 31
exercises: 10
content_sha256: 8c336f07217cf44a6de968a95edd464d659eb2373e41275c9e54ee365c2c1d02
---

## 3. SPECIAL FUNCTION SPACES

### 1. SPACES OF MAPPINGS INTO A METRIC SPACE

Let $ X $ be a set, $ Y $ a uniform space, $ (f_i)_{i \in I} $ a family of pseudometrics defining the uniform structure of $ Y $ (Chapter IX, \S 1, no. 4), and let $ \mathcal{S} $ be a set of subsets of $ X $. For each $ i \in I $, each set $ A \in \mathcal{S} $, and each pair $ (u, v) $ of mappings of $ X $ into $ Y $, write

$$
g_{i, A}(u, v) = \sup_{x \in A} f_i(u(x), v(x));
$$

it follows immediately that $ g_{i, A} $ is a *pseudometric* on $ \mathcal{F}(X; Y) $ and that the family of pseudometrics $ (g_{i, A})_{i \in I, A \in \mathcal{S}} $ defines the uniformity of $ \mathcal{S}$-*convergence* on $ \mathcal{F}(X; Y) $. In particular:

#### Proposition 1 {#top-x-s3-prop-1 .statement}

*If $ Y $ is a metrizable uniform space, the uniformity of uniform convergence on $ \mathcal{F}(X; Y) $ is metrizable.*

For if $ d $ is a metric on $ Y $ compatible with its uniform structure, the structure of uniform convergence on $ \mathcal{F}(X; Y) $ is defined by the single pseudometric

$$
\varepsilon(u, v) = \sup_{x \in X} d(u(x), v(x));
$$

in general this pseudometric is not finite, but it is equivalent to a finite one (Chapter IX, § 1, no. 2), and since the uniformity of uniform convergence is Hausdorff (§ 1, no. 2, Proposition 1), it is metrizable.

#### Corollary {#top-x-s3-n1-cor-1 .statement}

Let $ X $ be a topological space and let $ Y $ be a metrizable uniform space. Suppose that there is a sequence $ (K_n) $ of compact subsets of $ X $ such that every compact subset of $ X $ is contained in some $ K_n $. Then the uniformity of compact convergence on $ \mathcal{F}(X; Y) $ is metrizable.

Since the $ K_n $ cover $ X $, $ \mathcal{F}_c(X; Y) $ is isomorphic to a uniform subspace of $ \prod_n \mathcal{F}_u(K_n; Y) $ ($ \S 1 $, no. 2, Remark 3), and the corollary therefore follows from Proposition 1 (Chapter IX, § 2, no. 4, Theorem 1, Corollary 2).

Note that this corollary applies in particular if $ X $ is *locally compact and σ-compact* (Chapter I, § 9, no. 9, Proposition 15, Corollary 1).

Now let $ Y $ be a metric space and let $ d $ be its metric. If $ X $ is any set and $ \mathcal{S} $ any set of subsets of $ X $, we shall denote by $ \mathcal{B}_{\mathcal{S}}(X; Y) $ the set of all mappings $ u : X \to Y $ such that $ u(A) $ is *bounded* for each $ A \in \mathcal{S} $. Unless the contrary is expressly stated we shall regard $ \mathcal{B}_{\mathcal{S}}(X; Y) $ as endowed with the uniformity of $ \mathcal{S} $-convergence, which is defined by the following family of pseudometrics on $ \mathcal{B}_{\mathcal{S}}(X; Y) $:

$$
d_A(u, v) = \sup_{x \in A} d(u(x), v(x)) \tag{A \in \mathcal{S}}
$$

which are *finite* by hypothesis. When $ \mathcal{S} = \{X\} $, we write $ \mathcal{B}(X; Y) $ in place of $ \mathcal{B}_{\mathcal{S}}(X; Y) $. A mapping $ u : X \to Y $ is said to be *bounded* if it belongs to $ \mathcal{B}(X; Y) $, i.e. if $ u(X) $ is a bounded subset of $ Y $.

#### Proposition 2 {#top-x-s3-prop-2 .statement}

Let $ X $ be a set and $ Y $ a metric space. The set $ \mathcal{B}(X; Y) $ of bounded mappings is both open and closed in the space $ \mathcal{F}_u(X; Y) $.

If $ u $ is bounded, then every mapping $ v : X \to Y $ such that for all $ x \in X $, we have $ d(u(x), v(x)) \leq 1 $ is bounded, because

$$
d(v(x), v(x_0)) \leq d(u(x), u(x_0)) + 2;
$$

hence $ \mathcal{B}(X; Y) $ is open. On the other hand, if $ u $ lies in the closure of $ \mathcal{B}(X; Y) $ in $ \mathcal{F}_u(X; Y) $, there is a mapping $ u_0 \in \mathcal{B}(X; Y) $ such that $ d(u(x), u_0(x)) \leq 1 $ for all $ x \in X $; hence $ u $ is bounded.

#### Corollary 1 {#top-x-s3-prop-2-cor-1 .statement}

Let $ X $ be a set and $ Y $ a metric space. Then $ \mathcal{B}_{\mathcal{S}}(X; Y) $ is closed in $ \mathcal{F}_{\mathcal{S}}(X; Y) $. In particular, if $ Y $ is complete then $ \mathcal{B}_{\mathcal{S}}(X; Y) $ is complete with respect to the uniformity of $ \mathcal{S} $-convergence.

For $ \mathcal{B}_\mathfrak{S}(X; Y) $ is the inverse image of the subset $ \prod_{A \in \mathfrak{S}} \mathcal{B}(A; Y) $ of the product $ \prod_{A \in \mathfrak{S}} \mathcal{F}_u(X; Y) $ under the canonical mapping of $ \mathcal{F}_\mathfrak{S}(X; Y) $ into $ \prod_{A \in \mathfrak{S}} \mathcal{F}_u(A; Y) $; the first assertion therefore follows from § 1, no. 2, Remark 3, and the second follows from the first, if we take account of Theorem 1 of § 1, no. 5.

#### Corollary 2 {#top-x-s3-prop-2-cor-2 .statement}

*Let X be a topological space and Y a metric space. Then the space of all bounded continuous mappings of X into Y is both open and closed in $ C_u(X; Y) $; it is complete if Y is complete.*

The space in question is $ \mathcal{B}(X; Y) \cap C_u(X; Y) $; the first assertion follows from Proposition 2; the second follows from the first ($ \S 1 $, no. 6, Theorem 2, Corollary 1).

### 2. SPACES OF MAPPINGS INTO A NORMED SPACE

Consider, more particularly, the situation in which Y is a *normed* vector space over a non-discrete valued division ring K (Chapter IX, § 3, no. 3). Let us denote by $ ||y|| $ the norm of $ y \in Y $. The set $ \mathcal{F}(X; Y) = Y^X $ is then canonically endowed with a K-vector space structure. A mapping $ u : X \to Y $ is bounded if and only if the real-valued function $ x \mapsto ||u(x)|| $ is bounded in X. If $ u, v $ are bounded mappings of X into Y, it is clear that $ u + v $ and $ \lambda u (\lambda \in K) $ are bounded; in other words, $ \mathcal{B}(X; Y) $ is a *vector subspace* of $ \mathcal{F}(X; Y) $. Moreover, $ ||u|| = \sup_{x \in X} ||u(x)|| $ is a *norm* on $ \mathcal{B}(X; Y) $; for it satisfies the triangle inequality and $ ||u|| = 0 $ implies $ u = 0 $, and for each $ \lambda \in K $ we have

$$
||\lambda u|| = \sup_{x \in X} ||\lambda u(x)|| = \sup_{x \in X} |\lambda| \cdot ||u(x)|| = |\lambda| \cdot \sup_{x \in X} ||u(x)|| = |\lambda| \cdot ||u||.
$$

Moreover, it is immediately verified that the uniformity on $ \mathcal{B}(X; Y) $ defined by this norm is the uniformity of uniform convergence. Unless the contrary is expressly stated, whenever $ \mathcal{B}(X; Y) $ is considered as a normed space, it is the norm defined above which is in question.

#### Proposition 3 {#top-x-s3-prop-3 .statement}

*If the normed space Y is complete, then every series $ (u_n) $ of bounded mappings of X into Y which is absolutely convergent in the normed space $ \mathcal{B}(X; Y) $ (i.e. which is such that $ \sum_{n=0}^\infty ||u_n|| < +\infty $; cf. Chapter IX, § 3, no. 6) is uniformly convergent in X.*

For since $ \mathcal{B}(X; Y) $ is complete (no. 1, Proposition 2, Corollary 1), the result follows from Chapter IX, § 3, no. 6, Proposition 11 and the definition of a uniformly convergent series.

#### Remark 1 {#top-x-s3-n2-rem-1 .statement}

If $ \sum_{n=0}^{\infty} \|u_n\| < +\infty $, then $ \sum_{n=0}^{\infty} |u_n(x)| \leq \sum_{n=0}^{\infty} |u_n| < +\infty $
for each $ x \in X $; in other words, for each $ x \in X $ the series with general term $ u_n(x) $ is absolutely convergent in the space $ Y $. The converse is false. To avoid all confusion we shall sometimes say that the series with general term $ u_n $ is *normally convergent*, meaning that the series with general term $ \|u_n\| $ is convergent. A series can be uniformly convergent in $ X $ without being normally convergent; this is the case, for example, for the series $ (u_n) $ in the space $ \mathcal{B}(\mathbf{R}, \mathbf{R}) $, defined as follows:
$ u_n(x) = (1/n) \sin x $ if $ x \in [n\pi, (n+1)\pi] $, $ u_n(x) = 0 $ otherwise.

When $ Y $ is a *normed algebra* (Chapter IX, § 3, no. 7) over a non-discrete valued field $ K $, then $ \mathcal{B}(X; Y) $ is a $ K $-algebra, and the norm $ \|u\| $ is compatible with the algebra structure, since
$$
\|uv\| = \sup_{x \in X} \|u(x)v(x)\| \leq \sup_{x \in X} \|u(x)\| \cdot \|v(x)\|
\leq \sup_{x \in X} \|u(x)\| \cdot \sup_{x \in X} \|v(x)\| = \|u\| \cdot \|v\|.
$$
Thus $ \mathcal{B}(X; Y) $ is now a *normed algebra* over $ K $.

#### Proposition 4 {#top-x-s3-prop-4 .statement}

*Let $ X_i $ ($ 1 \leq i \leq n $) and $ Y $ be normed vector spaces over a non-discrete valued division ring $ K $, and let $ X = \prod_{i=1}^n X_i $. Then the set of all multilinear mappings of $ X $ into $ Y $ is closed in the space $ \mathcal{F}_s(X; Y) $.*

This set consists of all $ u \in F(X; Y) $ which satisfy all the relations
$$
\begin{align*}
u(x_1, \ldots, x_i' + x_i'', \ldots, x_n) &= u(x_1, \ldots, x_i', \ldots, x_n) \\
&\quad + u(x_1, \ldots, x_i'', \ldots, x_n), \\
u(x_1, \ldots, \lambda x_i, \ldots, x_n) &= \lambda u(x_1, \ldots, x_i, \ldots, x_n)
\end{align*}
$$
($ 1 \leq i \leq n,\ x_i,\ x_i',\ x_i'' $ arbitrary elements of $ X_i $, $ \lambda $ an arbitrary element of $ K $); since both sides of the relations (1) are continuous functions of $ u $ on $ \mathcal{F}_s(X; Y) $ (\S 1, no. 2, Remark 6), the result follows (Chapter I, § 8, no. 1, Proposition 2).

#### Proposition 5 {#top-x-s3-prop-5 .statement}

*Under the hypotheses of Proposition 4, the set $ \mathcal{L}(X_1, \ldots, X_n; Y) $ of continuous multilinear mappings of $ X $ into $ Y $ is closed in $ \mathcal{F}(X; Y) $ with respect to the topology of bounded convergence; it is complete with respect to the uniformity of bounded convergence if $ Y $ is complete.*

For if $ \mathcal{G} $ is the set of all bounded subsets of $ X $, $ \mathcal{L}(X_1, \ldots, X_n; Y) $ is the intersection of the set of all multilinear mappings of $ X $ into $ Y $ and the set $ \mathcal{B}_\mathcal{G}(X; Y) $ (Chapter IX, § 3, no. 5, Theorem 1); the result thus follows from Proposition 4 and Proposition 2, Corollary 1.

For the remainder of this subsection, $ K $ denotes a non-discrete valued field.

Then $ \mathcal{L}(X_1, \ldots, X_n; Y) $ is a vector subspace of $ \mathcal{F}(X; Y) $. Let $ B $ be the unit ball in $ X $, the set of all $ (x_i)_{1 \leq i \leq n} $ such that $ \sup_{1 \leq i \leq n} \|x_i\| \leq 1 $.

Then the mapping $ u \to u|B $ of $ \mathcal{L}(X_1, \ldots, X_n; Y) $ into $ \mathcal{B}(B; Y) $ is injective; moreover, the inverse image, under this mapping, of the uniformity of uniform convergence on $ \mathcal{B}(B; Y) $ is the uniformity of bounded convergence on $ \mathcal{L}(X_1, \ldots, X_n; Y) $. For every bounded subset of $ X $ is contained in a set of the form $ \mu B $ (for some $ \mu \in K^* $), and if $ u $ is an element of $ \mathcal{L}(X_1, \ldots, X_n; Y) $, to say that $ \|u(z)\| \leq a $ for all $ z \in \mu B $ is equivalent to saying that $ \|u(z)\| \leq a/|\mu|^n $ for all $ z \in B $. It is easily verified that the number
$$
\|u\| = \sup_{z \neq 0} \frac{\|u(z)\|}{\|z\|}
$$
is a norm on $ \mathcal{L}(X_1, \ldots, X_n; Y) $ and defines the uniformity of bounded convergence on this set, and clearly we have
$$
(2) \quad \|u(x_1, \ldots, x_n)\| \leq \|u\| \cdot \|x_1\| \cdots \|x_n\|.
$$

Unless the contrary is expressly stated, whenever $ \mathcal{L}(X_1, \ldots, X_n; Y) $ is considered as a normed space, it is the norm defined above which is in question.

#### Proposition 6 {#top-x-s3-prop-6 .statement}

*The multilinear mapping*
$$
(u, x_1, \ldots, x_n) \to u(x_1, \ldots, x_n)
$$
*of the normed space* $ \mathcal{L}(X_1, \ldots, X_n; Y) \times X_1 \times \cdots \times X_n $ *into* $ Y $ *is continuous*.

This is an immediate consequence of the inequality (2) (Chapter IX, § 3, no. 5, Theorem 1).

#### Proposition 7 {#top-x-s3-prop-7 .statement}

*Let* $ X, Y, Z $ *be three normed spaces over* $ K $. *The canonical mapping of the normed space* $ \mathcal{L}(X, Y; Z) $ *into the space of linear mappings of* $ X $ *into* $ \mathcal{L}(Y; Z) $ *which sends each* $ u \in \mathcal{L}(X, Y; Z) $ *to the mapping* $ x \to u(x, .) $ *is an isometry of* $ \mathcal{L}(X; Y; Z) $ *onto* $ \mathcal{L}(X; \mathcal{L}(Y; Z)) $.

This follows immediately from the definitions and the relation
$$
\sup_{\|x\| \leq 1} \left( \sup_{\|y\| \leq 1} \|u(x, y)\| \right) = \sup_{\|x\| \leq 1, \|y\| \leq 1} \|u(x, y)\|.
$$

#### Proposition 8 {#top-x-s3-prop-8 .statement}

Let $ X, Y, Z $ be three normed spaces over $ K $. The bilinear mapping $ (u, v) \to v \circ u $ of $ \mathcal{L}(X; Y) \times \mathcal{L}(Y; Z) $ into $ \mathcal{L}(X; Z) $ is continuous.

For if $ u \in \mathcal{L}(X; Y) $ and $ v \in \mathcal{L}(Y; Z) $ we have
$$
||v \circ u|| \leq ||u|| \cdot ||v||,
$$
since for all $ x \in X $ we have $ ||v(u(x))|| \leq ||v|| \cdot ||u(x)|| \leq ||v|| \cdot ||u|| \cdot ||x|| $ by reason of (2).

In particular, on the set $ \mathcal{L}(X) $ of continuous endomorphisms of a normed space $ X $ over $ K $, the norm $ ||u|| $ is compatible with the $ K $-algebra structure of $ \mathcal{L}(X) $.

#### Remark 2 {#top-x-s3-n2-rem-2 .statement}

The set $ \mathcal{L}(\mathbf{R}^m; \mathbf{R}^n) $ of linear (necessarily continuous) mappings of $ \mathbf{R}^m $ into $ \mathbf{R}^n $ can be identified with the set $ M_{n,m}(\mathbf{R}) $ of matrices with $ n $ rows and $ m $ columns with coefficients in $ \mathbf{R} $ and hence can be identified with $ \mathbf{R}^{mn} $; on $ \mathcal{L}(\mathbf{R}^m; \mathbf{R}^n) $, the uniformity of bounded convergence (with respect to the Euclidean metric on $ \mathbf{R}^m $), of compact convergence, and of pointwise convergence are then identified with the *additive* uniformity on $ \mathbf{R}^{mn} $. Take the norm of $ x = (x_i) \in \mathbf{R}^n $ to be
$$
||x|| = \sup_i |x_i|,
$$
and let $ (e_j) $ be the canonical basis of $ \mathbf{R}^m $; if $ u $ and $ v $ are two linear mappings of $ \mathbf{R}^m $ into $ \mathbf{R}^n $ such that $ \|u(e_j) - v(e_j)\| \leq \epsilon $ for $ 1 \leq j \leq m $, then we have $ |\alpha_{ij} - \beta_{ij}| \leq \epsilon $ for each pair $ (i, j) $ [$ U = (\alpha_{ij}) $ and $ V = (\beta_{ij}) $ being the matrices of $ u, v $ respectively]; and conversely, if these inequalities are satisfied, we have $ \|u(x) - v(x)\| \leq ma\epsilon $ for every point $ x $ of a cube of centre o and side $ a $ in $ \mathbf{R}^m $.

### 3. COUNTABILITY PROPERTIES OF SPACES OF CONTINUOUS FUNCTIONS

#### Theorem 1 {#top-x-s3-thm-1 .statement}

Let $ X $ be a compact space.
a) *If $ X $ is metrizable and if $ Y $ is any metrizable uniform space of countable type* (Chapter IX, § 2, no. 8), *then the metrizable space $ C_u(X; Y) $ of continuous mappings of $ X $ into $ Y $, endowed with the topology of uniform convergence, is of countable type*.
b) *Conversely, if the metrizable space $ C_u(X; \mathbf{R}) $ is of countable type, then $ X $ is metrizable*.

a) Let $ d $ (resp. $ d' $) be a metric compatible with the topology of $ X $ (resp. with the uniformity of $ Y $); then $ \delta(f, g) = \sup_{x \in X} d'(f(x), g(x)) $ is a metric defining the uniformity of uniform convergence on the space $ C(X; Y) $, the functions of $ C(X; Y) $ being bounded because $ X $ is compact (no. 1). For each pair of integers $ m > 0, n > 0 $, let $ G_{mn} $ be the set of functions $ f \in \mathcal{C}(X; Y) $ such that the relation $ d(x, x') \leq 1/m $ implies $ d(f(x), f(x')) \leq 1/n $. Every function $ f \in \mathcal{C}(X; Y) $ is uniformly continuous (Chapter II, § 4, no. 1, Theorem 2) and therefore, for each $ n > 0 $, $ \mathcal{C}(X; Y) $ is the union of the sets $ G_{mn} $ ($ m > 0 $). Let $ \{a_1, \ldots, a_{p(m)}\} $ be a finite subset of $ X $ such that the open balls with centres $ a_i $ and radii $ 1/m $ cover $ X $ ($ 1 \leq i \leq p(m) $); and let $ (b_r)_{r \in \mathbf{N}} $ be a countable sequence which is dense in $ Y $. For each mapping $ \varphi : [1, p(m)] \to \mathbf{N} $, let $ H_\varphi $ be the set of those $ f \in G_{mn} $ such that $ d'(f(a_k), b_{\varphi(k)}) \leq 1/n $ for $ 1 \leq k \leq p(m) $. By the definition of the $ b_r $, $ G_{mn} $ is the union of the sets $ H_\varphi $ for $ \varphi \in \mathbf{N}^{p(m)} $; let $ C_{mn} $ be the set of mappings $ \varphi \in \mathbf{N}^{p(m)} $ such that $ H_\varphi \neq \emptyset $, and for each $ \varphi \in C_{mn} $ let $ g_\varphi $ be an element of $ H_\varphi $; finally, let $ L_{mn} $ denote the countable set of $ g_\varphi $ for $ \varphi \in C_{mn} $. Let $ f \in G_{mn} $, and let $ \varphi $ be an element of $ C_{mn} $ such that $ f \in H_\varphi $; then it follows immediately from the definitions that we have $ d'(f(x), g_\varphi(x)) \leq 4/n $ for all $ x \in X $, i.e. $ \delta(f, g_\varphi) \leq 4/n $. Hence the union of the sets $ L_{mn} $ is dense in $ \mathcal{C}_u(X; Y) $, because for every integer $ n > 0 $ and every $ f \in \mathcal{C}(X; Y) $ there exists $ m $ such that $ f \in G_{mn} $, and we have just seen that the distance from $ f $ to $ L_{mn} $ is $ \leq 4/n $.

b) Let $ I = [0, 1] $. Since $ \mathcal{C}_u(X; I) $ is a uniform subspace of $ \mathcal{C}_u(X; \mathbf{R}) $, it is of countable type. Let $ (f_n) $ be a sequence which is dense in $ \mathcal{C}_u(X; I) $. Consider the product space $ K = \mathbf{N} $ and the mapping $ \psi : x \to (f_n(x)) $ of $ X $ into $ K $, which is obviously continuous. The mapping $ \psi $ is injective; for, by definition of the sequence $ (f_n) $, the relation $ f_n(x) = f_n(x') $ for all $ n $ implies, on passing to the limit, $ f(x) = f(x') $ for every function $ f \in \mathcal{C}(X; I) $; but this is impossible if $ x \neq x' $ by virtue of Axiom (OIV) applied to the point $ x $ and to a neighbourhood $ V $ of $ x $ which does not contain $ x' $ (Chapter IX, § 1, no. 5, Theorem 2). It follows that the compact space $ X $ is homeomorphic to the subspace $ \psi(X) $ of $ K $ (Chapter I, § 9, no. 4, Theorem 2, Corollary 2); since $ K $ is metrizable and of countable type, so is $ \psi(X) $ and therefore so is $ X $.

Q.E.D.

#### Corollary {#top-x-s3-n3-cor-1 .statement}

Let $ X $ be a locally compact space whose topology admits a countable base, and let $ Y $ be a metrizable uniform space of countable type.

a) The space $ \mathcal{L} $ of continuous mappings of $ X $ into $ Y $ which have a limit at infinity, endowed with the topology of uniform convergence in $ X $, is a metrizable space of countable type.

b) The space $ \mathcal{C}_c(X; Y) $ of continuous mappings of $ X $ into $ Y $, endowed with the topology of compact convergence, is a metrizable space of countable type.

a) Let $ X' $ be the compact space obtained by adjoining a point at infinity to $ X $ (Chapter I, § 9, no. 8, Theorem 4); by definition, every function $ f \in \mathcal{L} $ can be uniquely extended to a continuous function $ \overline{f} : X' \to Y $, and $ f \to \overline{f} $ is therefore a bijection of L onto $ C(X'; Y) $; and this bijection is a homeomorphism of the space L onto $ C_u(X'; Y) $ by Proposition 6 of § 1, no. 6. Since $ X' $ is metrizable (Chapter IX, § 2, no. 9, Proposition 16, Corollary) the result follows from Theorem 1, applied to $ X' $ and Y.

b) Let $ (U_n) $ be a covering of X by relatively compact open sets, such that every compact subset of X is contained in some $ U_n $ (Chapter I, § 9, no. 9, Proposition 15, Corollary 1). If $ S $ is the set of the $ \overline{U}_n $, the topology of compact convergence on $ C(X; Y) $ is the same as the topology of $ S $-convergence. Consequently ($ \S 1, $ no. 2, Remark 3) the space $ C_c(X; Y) $ is homeomorphic to a subspace of the product $ \prod_n C_u(\overline{U}_n; Y) $; since each of the compact spaces $ \overline{U}_n $ has a countable base, it is metrizable (Chapter IX, § 2, no. 9, Proposition 16); each of the $ C_u(\overline{U}_n; Y) $ is therefore metrizable and of countable type by Theorem 1, and hence so is $ C_c(X; Y) $.

Note that the space of all bounded continuous real-valued functions on $ \mathbf{R} $, endowed with the topology of uniform convergence, is not of countable type (Exercise 4).

### 4. THE COMPACT-OPEN TOPOLOGY

#### Theorem 2 {#top-x-s3-thm-2 .statement}

*Let X be a topological space, Y a uniform space. For each compact subset K of X and each open subset U of Y, let T(K, U) denote the set of all continuous mappings $ u : X \to Y $ such that $ u(K) \subset U $. Then the sets $ T(K, U) $ generate the topology of compact convergence on $ C(X; Y) $.*

Let $ Y' $ be the Hausdorff uniform space associated with Y (Chapter II, § 3, no. 8) and let $ i : Y \to Y' $ be the canonical mapping of Y onto $ Y' $. The topology of compact convergence is the coarsest topology for which the mappings $ u \to (i \circ u)|K $ of $ C(X; Y) $ into $ C_u(K; Y') $ are continuous, as K runs through the set of all compact subsets of X ($ \S 1, $ no. 4, Proposition 4). Hence we obtain a subbase of the topology of $ C_c(X; Y) $ by taking a subbase of the topology of $ C_c(K; Y') $ for each compact subset K of X and then taking the union [in $ \mathfrak{B}(C(X; Y)) $] of the inverse images of these subbases in $ C(X, Y) $. On the other hand, every open subset of Y is of the form $ \overline{i}^{-1}(U') $, where $ U' $ is open in $ Y' $ (Chapter II, § 3, no. 7, Proposition 12); hence, for each compact subset $ K' \supset K $, $ T(K, \overline{i}^{-1}(U')) $ is the inverse image of $ T(K, U') $ under the mapping

$$
C(X; Y) \to C_a(K'; Y').
$$

It thus remains for us to prove the theorem when X is *compact* and Y is *Hausdorff*; we shall make these assumptions from now on.

Let us first show that $ T(K, U) $ is open in $ C_c(X; Y) $. Let $ u_0 $ be a point of this set; since $ u_0(K) $ is compact (Chapter I, § 9, no. 4, Theorem 2, Corollary 1) and contained in the open set $ U $, there exists a symmetric entourage $ V $ of $ Y $ such that $ V(u_0(K)) \subset U $ (Chapter II, § 4, no. 3, Proposition 4, Corollary). Let $ W $ be the neighbourhood of $ u_0 $ in $ C_c(X; Y) $ consisting of all continuous mappings $ u : X \to Y $ such that $ (u(x), u_0(x)) \in V $ for all $ x \in K $. For such mappings we clearly have $ u(K) \subset V(u_0(K)) \subset U $; hence $ u \in T(K, U) $ and therefore $ W \subset T(K, U) $, which proves our assertion.

Conversely, if $ W $ is a neighbourhood of a point $ u_0 \in C_c(X; Y) $, let us show that $ W $ contains the intersection of a finite number of neighbourhoods of the form $ T(K, U) $. We may suppose that $ W $ is the set of all $ u \in C(X; Y) $ such that $ (u(x), u_0(x)) \in V $ for all $ x \in X $, $ V $ being a given entourage of $ Y $. Since $ u_0 $ is continuous on $ X $, it is uniformly continuous (Chapter II, § 4, no. 1, Theorem 2). Let $ V_1 $ be a symmetric entourage of $ Y $, open in $ Y \times Y $ and such that $ V_1^2 \subset V $. $ X $ can be covered by a finite number of compact sets $ K_i $ ($ 1 \leq i \leq n $) such that each $ u_0(K_i) $ is $ V_1 $-small ($ 1 \leq i \leq n $). Let $ U_i $ be the open set $ V_1(u_0(K_i)) $, and let $ u : X \to Y $ be a continuous mapping contained in the intersection of the $ n $ sets $ T(K_i, U_i) $ (which are neighbourhoods of $ u_0 $). Then, for every $ x \in K_i $, $ u(x) $ belongs to $ U_i $ and therefore $ u_0(x) $ and $ u(x) $ are $ V_1^2 $-close, hence $ V $-close. Since each $ x \in X $ belongs to some $ K_i $, we have $ u \in W $ and the proof is complete.

This result leads us to make the following definition:

#### Definition 1 {#top-x-s3-def-1 .statement}

*Let $ X, Y $ be two topological spaces, not necessarily uniformizable. For each compact subset $ K $ of $ X $ and each open subset $ U $ of $ Y $, let $ T(K, U) $ be the set of all $ u \in C(X; Y) $ such that $ u(K) \subset U $. The topology on $ C(X; Y) $ generated by the sets $ T(K, U) $ is called the topology of compact convergence or the compact-open topology; and we denote by $ C_c(X; Y) $ the topological space obtained by endowing $ C(X; Y) $ with this topology.*

If $ Y $ is a uniform space it follows from Theorem 2 that this definition agrees with that given in § 1, no. 3.

If $ H $ is a subset of $ C(X; Y) $ we shall say that the topology induced on $ H $ by that of $ C_c(X; Y) $ is the compact-open topology on $ H $.

#### Example {#top-x-s3-n4-exa-1 .statement}

Let $ I $ be the interval $[0, 1]$ in $ \mathbf{R} $. If $ Y $ is any topological space, the space $ C_c(I; Y) $ is called the *space of paths* in $ Y $. For each $ y \in Y $, the subspace $ \Omega_y(Y) $ of $ C_c(I; Y) $ consisting of paths $ u $ such that $ u(0) = u(1) = y $ is called the *space of loops* (in $ Y $) *at the point* $ y $.

#### Remark 1 {#top-x-s3-n4-rem-1 .statement}

Likewise, the topology induced on $ C(X; Y) $ by the product topology on $ Y^X = \mathcal{F}(X; Y) $ is called the *topology of pointwise convergence* ($ Y $ being not necessarily uniformizable); it is generated by sets of the form $ T(\{x\}, U) $ as $ x $ runs through $ X $ and $ U $ runs through the set of all open subsets of $ Y $, and it is therefore coarser than the compact-open topology. We deduce that, *if $ Y $ is Hausdorff, the space $ C_c(X; Y) $ is Hausdorff* (Chapter I, § 8, no. 1, Proposition 5, Corollary).

#### Remark 2 {#top-x-s3-n4-rem-2 .statement}

Let $ \mathcal{S} $ be a subbase of the topology of $ Y $, and let $ \mathcal{K} $ be a set of compact subsets of $ X $ with the following property:

(R) If $ L $ is any compact subset of $ X $ and $ V $ is any neighbourhood of $ L $, there exists a *finite* number of sets $ K_i \in \mathcal{K} $ such that $ L \subset \bigcup_i K_i \subset V $.

Then the sets $ T(K, U) $, where $ K \in \mathcal{K} $ and $ U \in \mathcal{S} $, form a *subbase* for the compact-open topology on $ C(X; Y) $. To prove this, we have to show that if $ L $ is any compact subset of $ X $ and $ V $ any open subset of $ Y $, and if $ u \in T(L, V) $, then there exists a finite number of pairs $ (K_i, U_i) $ such that $ K_i \in \mathcal{K} $, $ U_i \in \mathcal{S} $ and $ u \in \bigcap_i T(K_i, U_i) \subset T(L, V) $. Note first that for every finite sequence $ (s_k) $ of sets of $ \mathcal{S} $ and every compact subset $ M $ of $ X $, we have $ T\left(M, \bigcap_k S_k\right) = \bigcap_k T(M, S_k) $ by definition. We may therefore first of all replace $ \mathcal{S} $ by the set of finite intersections of sets of $ \mathcal{S} $, i.e. we may suppose that $ \mathcal{S} $ is a *base* of the topology of $ Y $. By hypothesis, $ u(L) $ is quasi-compact and contained in $ V $, hence there exists a finite number of sets $ U_i \in \mathcal{S} $ contained in $ V $ which cover $ u(L) $.

The sets $ \overline{u}^{-1}(U_i) $ are open in $ X $ and cover $ L $. For each $ x \in L $ there is therefore a compact neighbourhood $ N_x $ of $ x $ in $ L $, contained in some one of the $ \overline{u}^{-1}(U_i) $. We can cover $ L $ with a finite number of these sets $ N_{x_j} = L_j $; for each $ j $, let us denote by $ i(j) $ one of the indices $ i $ such that $ L_j \subset \overline{u}^{-1}(U_i) $. This being so, for each index $ j $ there exists [by (R)] a finite number of sets $ K_{jk} \subset \overline{u}^{-1}(U_{i(j)}) $, belonging to $ \mathcal{K} $, which cover $ L_j $. For each $ v \in \bigcap_{j,k} T(K_{jk}, U_{i(j)}) $ we have $ \bigcup_k v(K_{jk}) \subset U_{i(j)} $ and therefore $ v(L_j) \subset U_{i(j)} $, and $ v(L) = \bigcup_j v(L_j) \subset \bigcup_j U_{i(j)} \subset V $; thus our assertion is proved.

#### Theorem 3 {#top-x-s3-thm-3 .statement}

*Let $ X, Y, Z $ be three topological spaces and let $ f $ be a mapping of $ X \times Y $ into $ Z $. If $ f $ is continuous then $ \tilde{f}: x \to f(x, .) $ is a continuous mapping of $ X $ into $ C_c(Y; Z) $. The converse is true if $ Y $ is locally compact.*

Suppose that $ f $ is continuous. To show that $ \tilde{f} $ is continuous we have to prove that, for each compact subset $ K $ of $ Y $ and each open subset $ U $ of $ Z $, the inverse image $ V $ of $ T(K, U) $ under $ \tilde{f} $ is open in $ X $. Let $ x_0 \in V $; for each $ y \in K $, we have $ f(x_0, y) \in U $, and since $ f $ is continuous there is a neighbourhood $ V_y $ of $ x_0 $ in $ X $ and a neighbourhood $ W_y $ of $ y $ in $ Y $ such that $ f(V_y \times W_y) \subset U $. Since $ K $ is compact, there exists a finite number of points $ y_i \in K $ such that the sets $ W_{y_i} (1 \leq i \leq n) $ cover $ K $. Let $ V' $ be the intersection of the neighbourhoods $ V_{y_i} $ of $ x_0 $, which is a neighbourhood of $ x_0 $; if $ x \in V' $ and $ y \in K $, we have $ f(x, y) \in U $, since $ y $ is contained in some one of the $ W_{y_i} $ and $ x $ is contained in each $ V_{y_i} $; hence $ V' \subset V $, and therefore $ V $ is a neighbourhood of each of its points and consequently is open in $ X $.

Conversely, suppose that $ \tilde{f} $ is continuous and that $ Y $ is locally compact, and let us show that $ f $ is continuous. Let $ x_0 \in X $, let $ y_0 \in Y $ and let $ U $ be an open neighbourhood of $ f(x_0, y_0) $ in $ Z $; we shall show that there is a neighbourhood $ V $ of $ x_0 $ in $ X $ and a neighbourhood $ W $ of $ y_0 $ in $ Y $ such that $ f(V \times W) \subset U $. Since $ y \to f(x_0, y) $ is continuous, there is a *compact* neighbourhood $ W $ of $ y_0 $ such that $ f(\{x_0\} \times W) \subset U $. On the other hand, since $ \tilde{f} $ is continuous, the set $ V $ of $ x \in X $ such that $ f(x, .) \in T(W, U) $ [i.e. such that $ f(x, y) \in U $ for all $ y \in W $] is an open subset of $ X $ and therefore a neighbourhood of $ x_0 $; and we have $ f(V \times W) \subset U $.

Q.E.D.

#### Corollary 1 {#top-x-s3-thm-3-cor-1 .statement}

*Let $ X $ be a locally compact space, $ Y $ a topological space, $ H $ a subset of $ C(X; Y) $. Then the compact-open topology on $ H $ is the coarsest for which the mapping $ (u, x) \to u(x) $ of $ H \times X $ into $ Y $ is continuous.*

For, by Theorem 3, this mapping is continuous if and only if the canonical injection $ H \to C_c(X; Y) $ is continuous.

#### Remark 3 {#top-x-s3-n4-rem-3 .statement}

Let $ X $ be a locally compact space and $ Y $ a Hausdorff topological space. If $ \mathcal{T} $ is a topology on a subset $ H $ of $ C(X; Y) $ such that the mapping $ (u, x) \to u(x) $ is continuous on $ H \times X $ and if also $ H $ is *compact* with respect to $ \mathcal{T} $, then $ \mathcal{T} $ is the compact-open topology. For it is finer than the latter by Corollary 1, and since the compact-open topology is Hausdorff, the two topologies are identical. Note that if in addition $ Y $ is *completely regular*, then $ H $ is *equicontinuous* with respect to every uniformity compatible with the topology of $ Y $ (\S 2, no. 5, Theorem 2, Corollary 3), and for every compact subset $ K $ of $ X $ the set

$$
H(K) = \bigcup_{x \in K} H(x)
$$

is compact, since it is the image of $ H \times K $ under the continuous mapping $ (u, x) \to u(x) $.

#### Corollary 2 {#top-x-s3-thm-3-cor-2 .statement}

*Let $ X, Y, Z $ be three topological spaces such that $ X $ is Hausdorff and $ Y $ is locally compact. Then the restriction to $ C(X \times Y; Z) $ of the canonical bijection $ \mathcal{F}(X \times Y; Z) \to \mathcal{F}(X; \mathcal{F}(Y; Z)) $ (Set Theory, R, \S 4, no. 14) is a homeomorphism of $ C_c(X \times Y; Z) $ onto $ C_c(X; C_c(Y; Z)) $.*

This restriction is certainly a bijection

$$
\rho : \mathcal{C}(X \times Y; Z) \to \mathcal{C}(X; \mathcal{C}_c(Y; Z))
$$

by Theorem 3; it remains therefore to be shown that the compact-open topology on $ \mathcal{C}(X \times Y; Z) $ is the inverse image under $ \rho $ of the compact-open topology on $ \mathcal{C}(X; \mathcal{C}_c(Y; Z)) $. Since the sets $ T(K, U) $, where $ K $ is a compact subset of $ Y $ and $ U $ is an open subset of $ Z $, form a subbase of the topology of $ \mathcal{C}_c(Y; Z) $, it follows from Remark 2 that the topology of $ \mathcal{C}_c(X; \mathcal{C}_c(Y; Z)) $ is generated by the sets of the form $ T(J, T(K, U)) $, where $ K $ and $ U $ are as above and $ J $ is a compact subset of $ X $. Now the image of $ T(J, T(K, U)) $ under $ \rho $ is precisely $ T(J \times K, U) $, and is therefore an open set; so we have shown that $ \rho $ is continuous. To prove that $ \rho $ is a homeomorphism, we note first that the sets of the form $ J \times K $ in $ X \times Y $ (where $ J $ is a compact subset of $ X $, and $ K $ is a compact subset of $ Y $) satisfy the condition (R) of Remark 2: for if $ L $ is a compact subset of $ X \times Y $ and $ V $ is a neighbourhood of $ L $ in $ X \times Y $, the projections $ M = \operatorname{pr}_1(L) $, $ N = \operatorname{pr}_2(L) $ are compact, since $ X $ and $ Y $ are Hausdorff and $ V \cap (M \times N) $ is a neighbourhood of $ L $ in the compact space $ M \times N $, so that every point of $ L $ has a neighbourhood in $ M \times N $ of the form $ J \times K \subset V $, where $ J \subset M $ and $ K \subset N $ are compact; since $ L $ can be covered by a finite number of these neighbourhoods, the assertion is proved. Therefore sets of the form $ T(J \times K; U) $, where $ J $ is a compact subset of $ X $, $ K $ a compact subset of $ Y $ and $ U $ an open subset of $ Z $, generate the topology of $ \mathcal{C}_c(X \times Y; Z) $. But we have already seen that the image of $ T(J \times K, U) $ under $ \rho $ is the open set $ T(J, T(K, U)) $ in $ \mathcal{C}_c(X; \mathcal{C}_c(Y; Z)) $; hence $ \rho $ is a homeomorphism.

Note that if in addition $ Z $ is assumed to be uniformizable, Corollary 2 is a trivial consequence of § 1, no. 4, Proposition 2.

#### Proposition 9 {#top-x-s3-prop-9 .statement}

*Let $ X, Y, Z $ be three topological spaces, $ Y $ being locally compact. Then the mapping $ (u, v) \to v \circ u $ of $ \mathcal{C}_c(X; Y) \times \mathcal{C}_c(Y; Z) $ into $ \mathcal{C}_c(X; Z) $ is continuous.*

We have to show that, for every compact subset $ K $ of $ X $ and every open subset $ U $ of $ Z $, the set $ R $ of pairs $ (u, v) $ such that $ v(u(K)) \subset U $ is open in $ \mathcal{C}_c(X; Y) \times \mathcal{C}_c(Y; Z) $. Let $ (u_0, v_0) \in R $; then $ u_0(K) $ is a compact subset of the locally compact space $ Y $, contained in the open set $ \overline{v_0^{-1}}(U) $, and hence there is a compact neighbourhood $ L $ of $ u_0(K) $ contained in $ \overline{v_0^{-1}}(U) $ (Chapter I, § 9, no. 7, Proposition 10). The set $ V $ of all $ u \in \mathcal{C}_c(X; Y) $ such that $ u(K) \subset L $ is a neighbourhood of $ u_0 $, and the set $ W $ of all $ v \in \mathcal{C}_c(Y; Z) $ such that $ v(L) \subset U $ is a neighbourhood of $ v_0 $; furthermore, the relation $ (u, v) \in V \times W $ implies $ v(u(K)) \subset U $. Hence the result.

### 5. TOPOLOGIES ON GROUPS OF HOMEOMORPHISMS

#### Proposition 10 {#top-x-s3-prop-10 .statement}

Let $ X $ be a uniform space and let $ H $ be an equicontinuous set of homeomorphisms of $ X $ onto itself. If $ H $ and $ H^{-1} $ are endowed with the topology of pointwise convergence in $ X $, then the mapping $ u \to u^{-1} $ of $ H^{-1} $ onto $ H $ is continuous.

It is enough to show that, for each $ x_0 \in X $, the mapping $ u \to u^{-1}(x_0) $ of $ H^{-1} $ into $ X $ is continuous at every point $ u_0 \in H^{-1} $. Let $ V $ be a symmetric entourage of $ X $, and let $ y_0 = u_0^{-1}(x_0) $. By hypothesis there is a symmetric entourage $ U $ of $ X $ such that the relation $ (x, x_0) \in U $ implies $ (u^{-1}(x), u^{-1}(x_0)) \in V $ for all $ u \in H^{-1} $. Take an element $ u \in H^{-1} $ which is $ W(\{y_0\}, U) $-close to $ u_0 $; then we have $ (u(y_0), u_0(y_0)) \in U $, i.e. $ (u(y_0), x_0) \in U $. It follows that $ (y_0, u^{-1}(x_0)) \in V $, i.e. $ (u_0^{-1}(x_0), u^{-1}(x_0)) \in V $; this completes the proof.

#### Corollary {#top-x-s3-n5-cor-1 .statement}

Let $ X $ be a uniform space and let $ H $ be an equicontinuous group of homeomorphisms of $ X $ onto itself. Then the topology of pointwise convergence in $ X $ is compatible with the group structure of $ H $.

This is a consequence of Proposition 10, together with § 2, no. 1, Proposition 1, Corollary 5.

#### Proposition 11 {#top-x-s3-prop-11 .statement}

Let $ X $ be a compact space and let $ \Gamma $ be the group of all homeomorphisms of $ X $ onto itself. Then the topology of uniform convergence in $ X $ is compatible with the group structure of $ \Gamma $.

We know already (no. 4, Proposition 9) that the mapping $ (u, v) \to v \circ u $ of $ \Gamma \times \Gamma $ into $ \Gamma $ is continuous with respect to this topology; thus we have to show that $ u \to u^{-1} $ is continuous at every point $ u_0 $ of $ \Gamma $. Since $ u_0^{-1} $ is uniformly continuous on $ X $, given any symmetric entourage $ V $ of $ X $ there exists an entourage $ W $ of $ X $ such that the relation $ (x, x') \in W $ implies $ (u_0^{-1}(x), u_0^{-1}(x')) \in V $. Hence, if $ u \in \Gamma $ is such that $ (u_0(x), u(x)) \in W $ for all $ x \in X $, it follows that $ (x, u_0^{-1}(u(x))) \in V $ for all $ x \in X $, and therefore (as $ u $ is bijective) $ (u^{-1}(x), u_0^{-1}(x)) \in V $ for all $ x \in X $. This completes the proof.

Now let $ X $ be a locally compact space and let $ \Gamma $ be the group of all homeomorphisms of $ X $ onto itself. The topology of compact convergence in $ X $ is not necessarily compatible with the group structure of $ \Gamma $ (Exercise 17). Let $ X' $ denote the compact space obtained by adjoining a point at infinity $ \omega $ to $ X $. Every homeomorphism $ u $ of $ X $ onto itself extends uniquely to a homeomorphism $ u' $ of $ X' $ onto itself such that $ u'(\omega) = \omega $ (Chapter I, § 10, no. 3, Corollary to Proposition 7), so that $ \Gamma $ can be identified with the subgroup of the group $ \Gamma' $ of all homeomorphisms of $ X' $ onto itself, consisting of all homeomorphisms which leave $ \omega $ fixed. The topology induced on $ \Gamma $ by that of $ C_u(X'; X') $ is therefore compatible with the group structure of $ \Gamma' $ (Proposition 11), and $ \Gamma $ is closed in $ \Gamma' $ [with respect to the topology induced by that of $ C_u(X'; X') $] because it is defined by the equation $ u(\omega) = \omega $ (\S 1, no. 2, Remark 6). We denote by $ \mathcal{T}_\beta $ the group topology thus defined on $ \Gamma $; it is finer than the topology of compact convergence and can also (by virtue of \S 1, no. 6, Proposition 6) be defined as the topology of uniform convergence on $ X $, when $ X $ is endowed with the uniformity induced by the unique uniformity of $ X' $.

The topology $ \mathcal{T}_\beta $ can be characterized as follows:

#### Proposition 12 {#top-x-s3-prop-12 .statement}

*On the group $ \Gamma $ of all homeomorphisms of a locally compact space $ X $, the topology $ \mathcal{T}_\beta $ is the coarsest for which the mappings $ u \to u $ and $ u \to u^{-1} $ of $ \Gamma $ into $ C_c(X; X) $ are continuous.*

Let us denote the latter topology for the moment by $ \mathcal{C}' $. Since $ u \to u^{-1} $ is continuous with respect to $ \mathcal{T}_\beta $ and since $ \mathcal{T}_\beta $ is finer than the topology of compact convergence, it is clear that $ \mathcal{T}_\beta $ is finer than $ \mathcal{C}' $. To prove the converse, endow $ X' $ with its unique uniformity; let $ u_0 \in \Gamma $ and let $ V $ be an entourage of $ X' $; then we have to prove that there is a compact subset $ K $ of $ X $ and a symmetric entourage $ W $ of $ X' $ such that the relations

$$
u \in \Gamma, \ (u_0(x), u(x)) \in W \text{ and } (u_0^{-1}(x), u^{-1}(x)) \in W \text{ for all } x \in K
$$

imply

$$
(u_0(x), u(x)) \in V \text{ for all } x \in X.
$$

Let $ V_1 $ be a symmetric open entourage of $ X' $ such that $ \overset{2}{V}_1 \subset V $; then $ K_1 = X' - V_1(\omega) $ is a compact subset of $ X $. Choose a symmetric open entourage $ W $ of $ X' $ such that $ W \subset V $ and $ W(\omega) \cap W(u_0^{-1}(K_1)) = \emptyset $; this is possible by Proposition 4 of Chapter II, \S 4, no. 3. Let $ K_2 = X' - W(\omega) $, which is a compact subset of $ X $. We shall see that $ W $ and the compact set $ K = K_1 \cup K_2 $ do what is required. Since $ W \subset V $, it is enough to show that the relation

$$
(u_0^{-1}(x), u^{-1}(x)) \in W \text{ for all } x \in K_1 \quad (u \in \Gamma)
$$

implies that

$$
(u(y), \omega) \in V_1 \text{ for all } y \in W(\omega);
$$

for we shall then also have $ (u_0(y), \omega) \in V_1 $ and thence

$$
(u_0(y), u(y)) \in \overset{2}{V}_1 \subset V
$$

for all $ y \in W(\omega) = X' - K_2 $. Now if we had $ y \in W(\omega) $ and

$$
u(y) \in X' - V_1(\omega) = K_1,
$$

it would follow that $ y \in u^{-1}(K_1) \subset W(u_0^{-1}(K_1)) $, contrary to the choice of $ W $; the proof is therefore complete.

In general the group $ \Gamma $, endowed with $ \mathcal{T}_\beta $, is not locally compact; but we have the following criterion:

#### Theorem 4 {#top-x-s3-thm-4 .statement}

*Let $ G $ be a subgroup of the group $ \Gamma $ of all homeomorphisms of a locally compact space $ X $. Suppose that, in the space $ C_c(X; X) $, there is a neighbourhood $ V $ of the identity mapping $ e $ such that $ V \cap G = H $ is symmetric in $ G $ and relatively compact in $ C_c(X; X) $. Then the closure $ \overline{G} $ of $ G $ in $ \Gamma $ with respect to the topology $ \mathcal{T}_\beta $ is a locally compact group with respect to the topology induced by $ \mathcal{T}_\beta $; this topology induced on $ \overline{G} $ is the same as the topology of compact convergence, and the closure $ \overline{H} $ of $ H $ in $ C_c(X; X) $ is a neighbourhood of $ e $ in $ \overline{G} $ with respect to this topology.*

Let us show first that $ \overline{H} $ is contained in $ \Gamma $ and that the topology induced on $ \overline{H} $ by $ \mathcal{T}_\beta $ is *the same as the topology of compact convergence*. Let $ u_0 \in \overline{H} $; $ u_0 $ is therefore the limit, in $ C_c(X; X) $, of an ultrafilter $ \Phi $ on $ H $. Since $ \Phi^{-1} $ (the image of $ \Phi $ under $ u \to u^{-1} $) is an ultrafilter base on $ H \subset \overline{H} $, it converges in the compact subspace $ \overline{H} $ of $ C_c(X; X) $ to an element $ v_0 $. The mapping $ (u, v) \to uv $ converges to $ u_0 v_0 $ with respect to $ \Phi \times \Phi^{-1} $ (no. 4, Proposition 9); *a fortiori*, $ u \to uu^{-1} = e $ converges to $ u_0 v_0 $ with respect to $ \Phi $, hence $ u_0 v_0 = e $ since $ C_c(X; X) $ is Hausdorff. Similarly $ v_0 u_0 = e $; hence $ u_0 $ is a homeomorphism of $ X $, i.e., $ u_0 \in \Gamma $. Thus $ \overline{H} $ is contained in $ \Gamma $. Moreover, this argument shows that $ \overline{H}^{-1} = \overline{H} $ and that, for every ultrafilter $ \Phi $ on $ \overline{H} $ which converges to $ u_0 $, $ \Phi^{-1} $ converges in $ C_c(X; X) $ to $ u_0^{-1} $; hence the mapping $ u \to u^{-1} $ of $ \overline{H} $ into $ C_c(X; X) $ is continuous when $ \overline{H} $ carries the topology of compact convergence (Chapter I, § 7, no. 4, Proposition 9, Corollary 1). Proposition 12 then shows that, on $ \overline{H} $, the topology of compact convergence is the same as the topology induced by $ \mathcal{T}_\beta $.

Furthermore, since the topology $ \mathcal{T}_\beta $ on $ \Gamma $ is finer than the topology of compact convergence, $ \overline{H} $ is also the closure of $ H $ with respect to $ \mathcal{T}_\beta $. But $ H $ is a neighbourhood of $ e $ in $ G $ with respect to the topology of compact convergence, and *a fortiori* with respect to the topology induced by $ \mathcal{T}_\beta $; it follows (Chapter I, § 3, no. 1, Proposition 2) that $ \overline{H} $ is a neighbourhood of $ e $ in $ \overline{G} $ with respect to the topology induced by $ \mathcal{T}_\beta $, and hence $ \overline{G} $ is locally compact in this topology. If $ W $ is the interior of $ V $ with respect to the topology of compact convergence, then $ W \cap \Gamma $ is open in $ \mathcal{T}_\beta $, hence $ W \cap \overline{G} $ is contained in the closure of $ H = V \cap G $ with respect to $ \mathcal{T}_\beta $ (Chapter I, § 1, no. 6, Proposition 5); this shows that $ \overline{H} $ is also a neighbourhood of $ e $ in $ \overline{G} $ with respect to the topology of compact convergence. Finally, for each $ u_0 \in \Gamma $, the bijections $ v \to u_0 \circ v $ and $ v \to u_0^{-1} \circ v $ of $ C_c(X; X) $ onto itself are continuous (no. 4, Proposition 9), and hence, if $ u_0 \in \overline{G} $, $ u_0 \overline{H} $ is a neighbourhood of $ u_0 $ in $ \overline{G} $ with respect to the topology of compact convergence. This completes the proof.

#### Corollary {#top-x-s3-n5-cor-2 .statement}

*Let $ G $ be a group of homeomorphisms of a locally compact space $ X $. If the closure $ \overline{G} $ of $ G $ in $ C_c(X; X) $ is compact, then $ \overline{G} $ is a group of homeomorphisms of $ X $, and the topology of compact convergence is compatible with the group structure of $ \overline{G} $, which is therefore a compact topological group.*

A group of homeomorphisms of a locally compact space $ X $ which is locally compact but not compact with respect to the topology of compact convergence is *locally closed* in $ C_c(X; X) $ by virtue of Chapter I, § 9, no. 7, Proposition 12, *but is not necessarily closed*.

For example, in the ring $ \mathcal{L}(\mathbf{R}^n) $ of endomorphisms of $ \mathbf{R}^n $, identified with the ring $ M_n(\mathbf{R}) $ of square $ n \times n $ matrices over $ \mathbf{R} $ and endowed with the topology of compact convergence, the group $ GL(n, \mathbf{R}) $, identified with the group of non-singular matrices, is locally compact but dense (Chapter VI, § 1, no. 6, Proposition 6).

### Exercises {#top-x-s3-exercises}

See the [exercises for § 3](exercises/s3/).
