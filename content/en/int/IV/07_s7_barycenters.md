---
book: int
book_title: Integration
chapter: IV
chapter_title: EXTENSION OF A MEASURE. LP SPACES
section: 7
section_title: Barycenters
lang: en
source: int-i-vi
book_pages: INT IV.142-INT IV.148
pdf_pages: 0208-0225, 0249-0255
extraction: ocr
subsections:
    - "no": 1
      title: Definition of barycenters
      page: 101
      pdf_page: 208
    - "no": 2
      title: Extremal points and barycenters
      page: 102
      pdf_page: 209
    - "no": 3
      title: 'Applications: I. Vector spaces of continuous real functions'
      page: 106
      pdf_page: 213
    - "no": 4
      title: 'Applications: II. Vector spaces of continuous complex functions'
      page: 110
      pdf_page: 217
    - "no": 5
      title: 'Applications: III. Algebras of continuous functions'
      page: 111
      pdf_page: 218
    - "no": 6
      title: Uniqueness of integral representations
      page: 115
      pdf_page: 222
statements: 31
exercises: 10
content_sha256: 0570767550afc4ec72a1bd2d57ff21259b2713160100ad0deff3ffd79e594e1a
---

## § 7. BARYCENTERS

### 1. Definition of barycenters

Let E be a Hausdorff locally convex space over $ \mathbf{R} $, $ E' $ its dual, and $ E'^* $ the algebraic dual of $ E' $, E being canonically identified with a linear subspace of $ E'^* $. Let K be a compact subset of E; the canonical injection of K into E being continuous with compact support, for every measure $ \mu $ on K the integral $ \int x\, d\mu(x) $ is therefore defined and is an element of $ E'^* $ (Ch. III, §3, No. 1). Moreover, on K, the topology induced by the weak topology $ \sigma(E'^*, E') $ is identical with the original topology. Finally, if C is the closed convex envelope of K in $ E'^* $ equipped with $ \sigma(E'^*, E') $, then $ C \cap E $ is the closed convex envelope of K in E for the original topology (or for the weakened topology $ \sigma(E, E') $).

#### Definition 1 {#int-iv-s7-def-1 .statement}

*Let K be a compact subset of a Hausdorff locally convex space E. For every positive measure $ \mu $ on K of total mass equal to 1, the vector $ b_\mu = \int x\, d\mu(x) $ (belonging to $ E'^* $) is called the barycenter of $ \mu $.*

#### Example {#int-iv-s7-n1-exa-1 .statement}

— Let $ \mu $ be a *discrete* measure on K, positive and of total mass 1; it is thus of the form $ \mu = \sum_{i=1}^n \lambda_i \varepsilon_{x_i} $, where $ x_i \in K $, and the $ \lambda_i $ are real numbers such that $ \lambda_i \geq 0 $ for all $ i $ and $ \sum_{i=1}^n \lambda_i = 1 $. Since $ \int x\, d\varepsilon_y(x) = y $ (Ch. III, §3, No. 1, *Example 3*), $ b_\mu = \int x\, d\mu(x) = \sum_i \lambda_i x_i $. In particular, for every $ x \in K $, x is the barycenter of the measure $ \varepsilon_x $.

#### Proposition 1 {#int-iv-s7-prop-1 .statement}

*Let E be a Hausdorff locally convex space, K a compact subset of E, and C the closed convex envelope of K in E. The set C then consists of the points of E that are barycenters of at least one positive measure of mass 1 on K.*

This is nothing more than Prop. 5 of Ch. III, §3, No. 2 applied to the canonical injection of K into E.

#### Corollary {#int-iv-s7-n1-cor-1 .statement}

*If the closed convex envelope C of K in E is compact, then the barycenter of every positive measure of total mass 1 on K belongs to E.*

For, C is then also the closed convex envelope of K in $ E'^* $ equipped with the weak topology $ \sigma(E', E') $, and it suffices to apply, to the canonical injection of K into E, Prop. 4 of Ch. III, §3, No. 2.

#### Remark {#int-iv-s7-n1-rem-1 .statement}

The Cor. of Prop. 1 is applicable in particular when K is convex or when E is quasi-complete.

#### Proposition 2 {#int-iv-s7-prop-2 .statement}

— Let K be a compact convex subset of a Hausdorff locally convex space E, $ \mu $ a positive measure of total mass 1 on K, $ b_\mu $ its barycenter. For every convex numerical function $ f \geq 0 $ that is lower semi-continuous on K,
$$
f(b_\mu) \leq \int^* f d\mu.
$$
It is known (TVS, II, §5, No. 4, Prop. 5) that $ f $ is the upper envelope of a family of restrictions to K of continuous affine linear functions $ h_\alpha : x \mapsto c_\alpha + \langle x, z'_\alpha \rangle $. Then
$$
\int h_\alpha(x) d\mu(x) \leq \int^* f(x) d\mu(x)
$$
for every $ \alpha $; now, $ \int h_\alpha(x) d\mu(x) = c_\alpha + \int \langle x, z'_\alpha \rangle d\mu(x) $ since $ \mu $ has total mass 1; but $ \int \langle x, z'_\alpha \rangle d\mu(x) = \langle b_\mu, z'_\alpha \rangle $ by the definition of barycenter. Therefore $ \sup_\alpha \int h_\alpha(x) d\mu(x) = \sup_\alpha h_\alpha(b_\mu) = f(b_\mu) $, whence the conclusion.

When $ \mu $ is a discrete positive measure on K of total mass 1, Prop. 2 yields anew the inequality that defines the convex functions on K.

#### Corollary {#int-iv-s7-n1-cor-2 .statement}

— For every convex numerical function function g on K that is bounded and lower semi-continuous, $ g(b_\mu) \leq \int g d\mu $.

It suffices to note that $ \inf_{x \in K} g(x) = a $ is finite and apply Prop. 2 to $ g - a $.

### 2. Extremal points and barycenters

#### Proposition 3 {#int-iv-s7-prop-3 .statement}

— Let K be a compact convex subset of a Hausdorff locally convex space E, x a point of K. Every measure $ \mu $ on K, positive, of total mass 1, and admitting x as barycenter, is in the vague closure of the set of discrete positive measures of total mass 1 that admit x as barycenter.

Let U be a neighborhood of $ \mu $ for the vague topology; we can suppose that U consists of the measures $ \nu $ on K such that
$$
|\mu(f_i) - \nu(f_i)| \leq \delta
$$
for a finite number of functions $ f_i \in \mathcal{C}(K; \mathbf{C}) $ ($ 1 \leq i \leq p $) and a number $ \delta > 0 $. For every point $ a \in K $, there exists a closed convex neighborhood $ V_a $ of 0 in E such that
$$
|f_i(y) - f_i(a)| \leq \delta/2
$$

for $ 1 \leq i \leq p $ and for every $ y \in W_a = K \cap (a + V_a) $. Since $ K $ is compact, there exists a finite number of points $ a_j $ ($ 1 \leq j \leq r $) of $ K $ such that the $ W_{a_j} $ form a covering of $ K $ ($ 1 \leq j \leq r $). Consider a continuous partition of unity $ (g_j)_{1 \leq j \leq r} $ on $ K $, subordinate to the covering $ (W_{a_j}) $, and set $ \alpha_j = \mu(g_j) $ for all $ j $; if $ \alpha_j \neq 0 $ set $ \mu_j = \alpha_j^{-1} g_j \cdot \mu $, and if $ \alpha_j = 0 $ set $ \mu_j = \varepsilon_{a_j} $. Each of the measures $ \mu_j $ is positive, of total mass 1, and its support is contained in the compact convex set $ W_{a_j} $; moreover, by definition,

$$
\mu = \sum_{j=1}^r \alpha_j \mu_j
$$

since $ g_j \cdot \mu = 0 $ if $ \mu(g_j) = 0 $; the $ \alpha_j $ are $ \geq 0 $ and

$$
\sum_{j=1}^r \alpha_j = \sum_{j=1}^r \mu(g_j) = \mu \left( \sum_{j=1}^r g_j \right) = \mu(1) = 1 .
$$

Let $ x_j $ be the barycenter of $ \mu_j $, which belongs to $ W_{a_j} $ (No. 1, Prop. 1), and consider the discrete measure $ \nu = \sum_{j=1}^r \alpha_j \varepsilon_{x_j} $; it is positive and of total mass 1, and its barycenter is $ \sum_{j=1}^r \alpha_j x_j $, which is also the barycenter of $ \mu $ by virtue of (3), thus is equal to $ x $. Moreover, by (2), $ |f_i(y) - f_i(a_j)| \leq \delta/2 $ for all $ y \in W_{a_j} $ and for all $ i $, whence, since $ \operatorname{Supp}(\mu_j) \subset W_{a_j} $, $ |\mu_j(f_i) - f_i(a_j)| \leq \delta/2 $ for $ 1 \leq i \leq p $. On the other hand, since $ x_j \in W_{a_j} $, one also has

$$
|\varepsilon_{x_j}(f_i) - f_i(a_j)| \leq \delta/2
$$

for $ 1 \leq i \leq p $, whence $ |\mu_j(f_i) - \varepsilon_{x_j}(f_i)| \leq \delta $ for all $ i $ and $ j $. Since the $ \alpha_j $ are $ \geq 0 $ and have sum 1, it follows from (3) and the definition of $ \nu $ that $ \nu $ satisfies the inequality (1).

Q.E.D.

#### Corollary {#int-iv-s7-n2-cor-1 .statement}

— *Let $ K' $ be a compact subset of $ K $ such that $ K $ is the closed convex envelope of $ K' $. In order that $ x \in K' $ be an extremal point of $ K $, it is necessary and sufficient that $ \varepsilon_x $ be the only positive measure on $ K' $, of total mass 1, having $ x $ as barycenter.*

Suppose $ x $ is an extremal point of $ K $; to prove that $ \varepsilon_x $ is the only positive measure on $ K' $, of total mass 1, having $ x $ as barycenter, it suffices, by Prop. 3, to see that the set of *discrete* measures $ \nu $ on $ K' $ that are positive, of total mass 1, and have $ x $ as barycenter, reduces to $ \varepsilon_x $. But such a measure $ \nu $ is of the form $ \sum_{i=1}^r \lambda_i \varepsilon_{x_i} $ with $ \lambda_i > 0 $ for $ 1 \leq i \leq r $ and $ \sum_{i=1}^{r} \lambda_i = 1 $, and the hypothesis that $ x $ is the barycenter of $ \nu $ may be written $ x = \sum_{i=1}^{r} \lambda_i x_i $. Since $ x $ is extremal, this implies that $ x_i = x $ for all $ i $, whence $ \nu = \varepsilon_x $.

Conversely, let us assume that $ \varepsilon_x $ is the only positive measure on $ K' $, of total mass 1, having $ x $ as barycenter, and let us show that $ x $ is extremal. In the contrary case, there would exist two distinct points $ x', x'' $ of $ K $ and a real number $ \lambda $ such that $ 0 < \lambda < 1 $ and $ x = \lambda x' + (1 - \lambda) x'' $. By Prop. 1, $ x' $ (resp. $ x'' $) is the barycenter of a positive measure $ \mu' $ (resp. $ \mu'' $) on $ K' $ of total mass 1. Then $ x $ is the barycenter of $ \lambda \mu' + (1 - \lambda) \mu'' $. Therefore $ \lambda \mu' + (1 - \lambda) \mu'' = \varepsilon_x $. Therefore $ \mu' $ and $ \mu'' $ are proportional to $ \varepsilon_x $, whence $ x' = x'' = x $, which is absurd.

#### Theorem 1 (Choquet) {#int-iv-s7-thm-1 .statement}

— *Let E be a Hausdorff locally convex space over $ \mathbf{R} $, K a metrizable compact convex subset of E, and M the set of extremal points of K. The set M is the intersection of a countable family of open sets in K, and every point of K is the barycenter of a measure $ \mu $ on K such that $ \mu(K - M) = 0 $.*

To prove the first assertion, denote by I the interval $[0, 1]$ of $ \mathbf{R} $; since K is compact and metrizable, so is $ K \times K \times I $; the subset U of $ K \times K \times I $ formed by the triples $(x, y, \lambda)$ such that $ x \neq y $ and $ 0 < \lambda < 1 $ is open in $ K \times K \times I $, therefore there exists a sequence $(F_n)$ of closed sets in $ K \times K \times I $ whose union is U (GT, IX, §2, No. 5, Prop. 7). The mapping $ q : K \times K \times I \to K $ defined by $ q(x, y, \lambda) = \lambda x + (1 - \lambda) y $ is continuous and, by the definition of extremal point, $ K - M = q(U) = \bigcup_n q(F_n) $; but $ F_n $ is compact since it is closed in $ K \times K \times I $, therefore $ q(F_n) $ is compact and therefore closed in K; the set $ U_n = K - q(F_n) $ is therefore open in K, and we have $ M = \bigcap_n U_n $.

In the continuation of the proof, we shall denote by $ u $ a continuous and *convex* numerical function on K, by $ G \subset E \times \mathbf{R} $ the graph of $ u $, and by S the *closed convex envelope* of G in $ E \times \mathbf{R} $.

#### Lemma 1 {#int-iv-s7-lem-1 .statement}

— *Let $ \overline{u} $ be the lower envelope of the continuous affine linear functions on E that are $ \geq u $ on K. Then S is the set of points $(a, b) \in E \times \mathbf{R}$ such that $ a \in K $ and $ u(a) \leq b \leq \overline{u}(a) $.*

By the Hahn-Banach theorem, for $(a, b)$ to belong to S, it is necessary and sufficient that $ h(a, b) \geq 0 $ for every continuous affine linear function $ h $ on $ E \times \mathbf{R} $ such that $ h(x, u(x)) \geq 0 $ for $ x \in K $. Setting $ h(x, t) = f(x) - \lambda t $, where $ f $ is a continuous affine linear function on E, we see that the relation $(a, b) \in S$ is equivalent to the following property: the relation

$$
f(x) \geq \lambda u(x) \quad \text{for all } x \in K
$$

implies

(5)
$$
f(a) \geq \lambda b .
$$

First set $ \lambda = 0 $; the fact that (4) implies (5) for every continuous affine linear function $ f $ on $ E $ is equivalent to the relation $ a \in K $ by the Hahn-Banach theorem. Next, set $ \lambda = -1 $ and replace $ f $ by $ -f $; then the relation $ f(x) \leq u(x) $ in $ K $ must imply $ f(a) \leq b $. But since $ u $ is convex and continuous on $ K $, $ u(a) $ is equal to the supremum of the $ f(a) $ for the continuous affine linear functions $ f $ on $ E $ such that $ f(x) \leq u(x) $ on $ K $ (TVS, II, §5, No. 4, Prop. 5); we thus obtain the relation $ b \geq u(a) $. Finally, set $ \lambda = 1 $; to say that (4) implies (5) then means, by definition, that $ b \leq \overline{u}(a) $. This proves the lemma, since the relation (4) (resp. (5)) is equivalent to the one obtained by multiplying both sides by a scalar $ > 0 $.

#### Lemma 2 {#int-iv-s7-lem-2 .statement}

*If $ u $ is strictly convex on $ K $, then $ u(x) < \overline{u}(x) $ for every non-extremal point $ x $ of $ K $.*

For, there then exist two distinct points $ y, z $ of $ K $ such that $ x = (y + z)/2 $, whence $ u(x) < (u(y) + u(z))/2 $ since $ u $ is strictly convex. If $ f $ is an affine linear function on $ E $, then $ f(x) = (f(y) + f(z))/2 $; applying this relation to the continuous affine linear functions $ f $ that are $ \geq u $ on $ K $, we obtain

$$
\overline{u}(x) \geq (\overline{u}(y) + \overline{u}(z))/2 \geq (u(y) + u(z))/2 > u(x) .
$$

These lemmas established, we therefore (Lemma 1) have $ (a, \overline{u}(a)) \in S $ for all $ a \in K $. Since $ G $ is compact, being the image of $ K $ under the continuous mapping $ x \mapsto (x, u(x)) $, there exists, by Prop. 1 of No. 1, a positive measure $ \nu $ on $ G $, of total mass 1 , having $ (a, \overline{u}(a)) $ as barycenter. Since the restriction of the projection $ pr_1 $ to $ G $ is a homeomorphism of $ G $ onto $ K $, the measure $ \nu $ may be transported by means of this homeomorphism, which yields a measure $ \mu $ on $ K $ (positive and of total mass 1 ) such that

(6)
$$
a = \int x \, d\mu(x) \quad \text{and} \quad \overline{u}(a) = \int u(x) \, d\mu(x) .
$$

The first of the relations (6) means that $ a $ is the barycenter of $ \mu $. The function $ \overline{u} $ is upper semi-continuous and bounded on $ K $, hence is $ \mu $-integrable (§4, No. 4, Cor. 1 of Prop. 5); moreover, since the function $ -\overline{u} $ is by definition convex, we have, by the Cor. of Prop. 2 of No. 1,

(7)
$$
\overline{u}(a) \geq \int \overline{u}(x) \, d\mu(x) ,
$$

whence, on comparing with the second of the formulas (6),

$$
\int u(\mathbf{x})\, d\mu(\mathbf{x}) \geq \int \overline{u}(\mathbf{x})\, d\mu(\mathbf{x}) .
$$

But since $ u(\mathbf{x}) \leq \overline{u}(\mathbf{x}) $ on K, the relation (8) implies that $ u(\mathbf{x}) = \overline{u}(\mathbf{x}) $ almost everywhere for $ \mu $. Taking into account Lemma 2, one sees that Theorem 1 will be proved once the following lemma has been established:

#### Lemma 3 {#int-iv-s7-lem-3 .statement}

*Let E be a Hausdorff locally convex space over $ \mathbf{R} $, and K a metrizable compact convex subset of E. Then, there exists a strictly convex numerical function on K.*

For, the Banach space $ \mathcal{C}(K; \mathbf{R}) $ is separable (GT, X, §3, No. 3, Th. 1), therefore so is the subspace $ \mathcal{A} $ of $ \mathcal{C}(K; \mathbf{R}) $ formed by the restrictions to K of the *continuous affine linear functions on* E. Thus let $ (h_n) $ be a sequence dense in $ \mathcal{A} $, and let $ \alpha_n > \sup_{\mathbf{x} \in K} |h_n(\mathbf{x})| $. Then each of the functions $ h_n^2 / n^2 \alpha_n^2 $ is convex in K (TVS, II, §2, No. 8, *Examples*), and the series with general term $ h_n^2 / n^2 \alpha_n^2 $ is normally convergent, therefore its sum $ u $ is continuous and convex in K. It remains to see that $ u $ is strictly convex, and for this it suffices to prove that for any two distinct points $ \mathbf{x}, \mathbf{x}' $ of K, there is an integer $ n $ such that the restriction of $ h_n^2 $ to the segment with endpoints $ \mathbf{x}, \mathbf{x}' $ is strictly convex; but for this it suffices that $ h_n(\mathbf{x}) \neq h_n(\mathbf{x}') $ (*loc. cit.*). Now, there exists a function $ h \in \mathcal{A} $ such that $ h(\mathbf{x}) \neq h(\mathbf{x}') $ (TVS, II, §4, No. 1, Cor. 1 of Prop. 2) and since the sequence $ (h_n) $ is dense in $ \mathcal{A} $, there exists an $ n $ such that $ h_n(\mathbf{x}) \neq h_n(\mathbf{x}') $.

Q.E.D.

#### Corollary {#int-iv-s7-n2-cor-2 .statement}

*Let E be a Hausdorff locally convex space over $ \mathbf{R} $, C a proper convex cone in E with vertex 0, that is complete and metrizable for the uniform structure induced by the weakened uniform structure of E. Let M be the union of the extremal generators of C. For every $ \mathbf{x} \in C $ there exist a compact convex subset K of C and a measure $ \lambda \geq 0 $ on K of total mass 1, such that $ K - (M \cap K) $ is $ \lambda $-negligible and the barycenter of $ \lambda $ is equal to $ \mathbf{x} $.

For, $ \mathbf{x} $ belongs to a cap K of C (TVS, II, §7, No. 2, Prop. 5), and $ M \cap K $ contains the set of extremal points of K (*loc. cit.*, Cor. 1 of Prop. 4). It then suffices to apply Th. 1.

### 3. Applications: I. Vector spaces of continuous real functions

Let X be a nonempty compact space, $ \mathcal{H} $ a linear subspace of the Banach space $ \mathcal{C}(X; \mathbf{R}) $ that contains the constants and *separates* the points of X (GT, X, §4, No. 1, Def. 1). We equip $ \mathcal{H} $ with the normed space topology induced by that of $ C(X; \mathbf{R}) $, and denote by $ \mathcal{H}' $ the dual of this normed space. For every $ x \in X $, the mapping $ f \mapsto f(x) $ is a continuous linear form on $ \mathcal{H} $ (the restriction to $ \mathcal{H} $ of the Dirac measure $ \varepsilon_x $), thus is an element of $ \mathcal{H}' $ that will be denoted $ i_{\mathcal{H}}(x) $, so that

$$
\langle f, i_{\mathcal{H}}(x) \rangle = f(x)
$$

for every function $ f \in \mathcal{H} $ and every $ x \in X $.

The mapping $ i_{\mathcal{H}} $ of X into $ \mathcal{H}' $ is injective and continuous when $ \mathcal{H}' $ is equipped with the weak topology $ \sigma(\mathcal{H}', \mathcal{H}) $; the second assertion follows at once from the definitions and (9); as for the first, note that if $ x, x' $ are two distinct points of X, by hypothesis there exists a function $ h \in \mathcal{H} $ such that $ h(x) \neq h(x') $, therefore, by (9), $ \langle h, i_{\mathcal{H}}(x) \rangle \neq \langle h, i_{\mathcal{H}}(x') \rangle $ and *a fortiori* $ i_{\mathcal{H}}(x) \neq i_{\mathcal{H}}(x') $. The image $ i_{\mathcal{H}}(X) $ is therefore a *compact* subset of $ \mathcal{H}' $ (for the weak topology), and $ i_{\mathcal{H}} $ is a *homeomorphism* of X onto $ i_{\mathcal{H}}(X) $.

#### Proposition 4 {#int-iv-s7-prop-4 .statement}

(i) *The closed convex envelope* C *of* $ i_{\mathcal{H}}(X) $ *in* $ \mathcal{H}' $ *(for the weak topology* $ \sigma(\mathcal{H}', \mathcal{H}) $) *is compact*.

(ii) *For a point* $ i_{\mathcal{H}}(x) $ *to be an extremal point of* C, *it is necessary and sufficient that the only positive measure* $ \lambda $ *on* X *such that*

$$
h(x) = \int h \, d\lambda
$$

*for every function* $ h \in \mathcal{H} $ (which implies in particular that $ \lambda $ has total mass 1, since $ 1 \in \mathcal{H} $) *be the Dirac measure* $ \varepsilon_x $.

It follows that, for each $ h \in \mathcal{H} $, the function $ z' \mapsto \langle h, z' \rangle $ on C attains its supremum at at least one extremal point of C (TVS, II, §7, No. 1, Prop. 1), and this point belongs to $ i_{\mathcal{H}}(X) $ (*loc. cit.*, Cor. of Prop. 2).

(i) By (9), $ \| i_{\mathcal{H}}(x) \| \leq 1 $ in the normed space $ \mathcal{H}' $, in other words $ i_{\mathcal{H}}(X) $ is bounded, and the assertion follows from the fact that $ \mathcal{H}' $, equipped with the weak topology $ \sigma(\mathcal{H}', \mathcal{H}) $, is *quasi-complete* (TVS, III, §4, No. 2, Cor. 5 of Th. 1).

(ii) Every positive measure $ \mu $ of mass 1 on $ i_{\mathcal{H}}(X) $ arises, by transport of structure by means of the homeomorphism $ i_{\mathcal{H}} $, from a positive measure $ \lambda $ of mass 1 on X, the Dirac measure $ \varepsilon_{i_{\mathcal{H}}(x)} $ arising from $ \varepsilon_x $. To say that $ \mu $ admits $ i_{\mathcal{H}}(x) $ as barycenter means, by definition, that

$$
\int_X \langle h, i_{\mathcal{H}}(z) \rangle \, d\lambda(z) = \langle h, i_{\mathcal{H}}(x) \rangle
$$

for every function $ h \in \mathcal{H} $. Taking (9) into account, the assertion (ii) is just the translation of the criterion of No. 2, Cor. of Prop. 3 for $ i_{\mathcal{H}}(x) $ to be an extremal point of C.

We shall say that a point $ x \in X $ satisfying condition (ii) of Prop. 4 is $ \mathcal{H} $-extremal; we denote by $ \mathrm{Ch}_{\mathcal{H}}(X) $ (or simply $ \mathrm{Ch}(X) $) the set of these points, and by $ \check{S}_{\mathcal{H}}(X) $ (or simply $ \check{S}(X) $) the closure of $ \mathrm{Ch}_{\mathcal{H}}(X) $ in $ X $.

#### Proposition 5 {#int-iv-s7-prop-5 .statement}

*Every function* $ h \in \mathcal{H} $ *attains its supremum at at least one* $ \mathcal{H} $*-extremal point*.

Let $ x $ be a point of $ X $, $ h $ a function in $ \mathcal{H} $. The relation $ h(z) \leq h(x) $ for all $ z \in X $ may be written $ \langle h, i_{\mathcal{H}}(z) \rangle \leq \langle h, i_{\mathcal{H}}(x) \rangle $ for all $ z \in X $, and therefore means that the weakly closed hyperplane of $ \mathcal{H}' $ with equation $ \langle h, t' \rangle = \langle h, i_{\mathcal{H}}(x) \rangle $ is a *support hyperplane* of $ i_{\mathcal{H}}(X) $. It is known (TVS, II, §7, No. 1, Cor. of Prop. 1) that such a hyperplane contains at least one extremal point of the closed convex envelope of $ i_{\mathcal{H}}(X) $, and such a point $ i_{\mathcal{H}}(y) $ is the image of an $ \mathcal{H} $-extremal point $ y $ by definition; $ h(y) $ is therefore equal to the supremum of $ h $ in $ X $.

#### Proposition 6 {#int-iv-s7-prop-6 .statement}

*For every point* $ x \in X $, *the following properties are equivalent*:

a) $ x $ *is* $ \mathcal{H} $*-extremal*.

b) *For every open neighborhood* $ U $ *of* $ x $ *in* $ X $ *and every* $ \varepsilon > 0 $, *there exists a function* $ h \geq 0 $ *in* $ \mathcal{H} $ *such that* $ h(x) \leq \varepsilon $ *and* $ h(y) \geq 1 $ *for every* $ y \in X - U $.

Let $ x $ be any point of $ X $, $ f $ a function in $ \mathcal{C}(X; \mathbf{R}) $; it is known (TVS, II, §3, No. 1, Prop. 1) that the infimum of the numbers $ \lambda(f) $, for all the positive measures on $ X $ such that $ \lambda(h) = h(x) $ for every function $ h \in \mathcal{H} $, is equal to the supremum of the numbers $ h(x) $, where $ h $ runs over the set of functions $ h \in \mathcal{H} $ such that $ h \leq f $. Suppose that $ x $ is $ \mathcal{H} $-extremal; it then follows from Prop. 4, (ii) that for every function $ f \in \mathcal{C}(X; \mathbf{R}) $,

$$
f(x) = \sup_{h \in \mathcal{H}, h \leq f} h(x).
$$

To show that *a)* implies *b)*, we take for $ f $ a continuous mapping of $ X $ into $[0, 1]$, with support contained in $ U $, such that $ f(x) = 1 $; then, by (11), there exists a function $ h' \in \mathcal{H} $ such that $ h' \leq f $ and $ h'(x) \geq 1 - \varepsilon $. Since $ 1 \in \mathcal{H} $, the function $ h = 1 - h' $ meets the conditions of *b)*.

Conversely, suppose that the condition *b)* is verified; this condition implies that $ 1 - h \leq \varphi_U $; for every positive measure $ \lambda $ on $ X $ satisfying the condition (10), we therefore have

$$
\lambda(U) = \lambda(\varphi_U) \geq \lambda(1 - h) = 1 - h(x) \geq 1 - \varepsilon.
$$

Since, by hypothesis, this relation holds for every $ \varepsilon > 0 $ and every open neighborhood $ U $ of $ x $, it follows that

$$
\lambda(\{x\}) = \inf_U \lambda(U) \geq 1 - \varepsilon
$$

for every $ \varepsilon > 0 $, therefore $ \lambda(\{x\}) = 1 $. Since $ \lambda $ is positive and of total mass 1, necessarily $ \lambda = \varepsilon_x $, which proves that $ x $ is $ \mathcal{H} $-extremal, by virtue of Prop. 4, (ii).

#### Proposition 7 {#int-iv-s7-prop-7 .statement}

*Let F be a closed subset of X. The following properties are equivalent:*

a) *F contains $ \check{S}_{\mathcal{H}}(X) $.*

b) *For every function $ h \in \mathcal{H} $, the set F intersects the set of points of X where h attains its supremum.*

c) *For every point $ x \in X $, there exists a positive measure $ \mu $ of total mass 1 on X, such that $ \operatorname{Supp}(\mu) \subset F $ and $ h(x) = \int h \, d\mu $ for every function $ h \in \mathcal{H} $.*

Let $ G = i_{\mathcal{H}}(F) $. The condition *a)* signifies that G contains the set of extremal points of C. The condition *b)* signifies that G meets the intersection of $ i_{\mathcal{H}}(X) $ with each of the closed support hyperplanes of $ i_{\mathcal{H}}(X) $. Finally, the condition *c)* signifies that every point of $ i_{\mathcal{H}}(X) $ is the barycenter of a measure with support contained in G; by No. 1, Prop. 1, this is also equivalent to saying that the closed convex envelope of $ i_{\mathcal{H}}(X) $ is equal to the closed convex envelope of G. The equivalence of the conditions *a)*, *b)* and *c)* therefore follows from TVS, II, §7, No. 1, Cor. of Prop. 2.

#### Proposition 8 {#int-iv-s7-prop-8 .statement}

*Suppose X is metrizable. Then the set $ \operatorname{Ch}_{\mathcal{H}}(X) $ of $ \mathcal{H} $-extremal points of X is the intersection of a countable family of open sets in X, and for every $ x \in X $, there exists a positive measure $ \mu $ of total mass 1 on X such that*

$$
\mu(X - \operatorname{Ch}_{\mathcal{H}}(X)) = 0 \quad \text{and} \quad \int h \, d\mu = h(x)
$$

*for every $ h \in \mathcal{H} $.*

This is the translation of Th. 1 of No. 2, by transport of structure by means of the homeomorphism $ x \mapsto i_{\mathcal{H}}(x) $, as in Prop. 5.

A certain number of results of this No. may be extended when $ \mathcal{H} $ is replaced by a set $ \mathcal{P} $ of functions defined on X, with values in $ \mathbf{R} \cup \{+\infty\} $, that are lower semi-continuous, $ \mathcal{P} $ being assumed to contain the constants and to satisfy $ \mathcal{P} + \mathcal{P} \subset \mathcal{P} $ (Exer. 2).

#### Example {#int-iv-s7-n3-exa-1 .statement}

— Take X to be the unit ball $ \|x\| \leq 1 $ in $ \mathbf{R}^3 $, and let $ \mathcal{H} $ be a vector space of continuous functions on X, containing the restrictions to X of the affine linear functions on $ \mathbf{R}^3 $ and satisfying the *maximum principle*, that is, for every non-constant function $ h \in \mathcal{H} $, the set of points of X where h attains its supremum is contained in the sphere $ S_2 $. It then follows easily from Props. 5 and 7 that $ \operatorname{Ch}_{\mathcal{H}}(X) = \check{S}_{\mathcal{H}}(X) = S_2 $. An important example of a vector space $ \mathcal{H} $ satisfying the preceding conditions is the set of functions continuous on X and *harmonic* in the open ball $ \|x\| < 1 $. For these functions, one proves that the positive measure $ \mu $ of mass 1 such that $ \operatorname{Supp}(\mu) \subset S_2 $ and $ h(x) = \int h \, d\mu $ for all $ h \in \mathcal{H} $ is given, if $ \|x\| < 1 $, by Poisson’s formula

$$
d\mu(z) = \frac{1 - \|z\|^2}{\|z - x\|^3} d\sigma(z),
$$

where $ \sigma $ is the measure on $ S_2 $ invariant under the orthogonal group and such that $ \sigma(S_2) = 1 $ (Ch. VII, §3, Exer. 8).*

### 4. Applications: II. Vector spaces of continuous complex functions

Let $ X $ be a nonempty compact space, $ \mathcal{H} $ a linear subspace of the complex Banach space $ \mathcal{C}(X; \mathbf{C}) $ that contains the constants and separates the points of $ X $. The set of real parts $ \Re(f) $ of the functions $ f \in \mathcal{H} $ is a linear subspace $ \mathcal{H}_r $ of the real vector space $ \mathcal{C}(X; \mathbf{R}) $; for every $ f \in \mathcal{H} $, the set $ \mathcal{H}_r $ also contains $ \mathcal{I}(f) = \Re(-if) $; it follows that $ \mathcal{H}_r $ separates the points of $ X $, because the relation $ h(x) = h(y) $ for all $ h \in \mathcal{H}_r $ implies that $ \Re(f(x)) = \Re(f(y)) $ and $ \mathcal{I}(f(x)) = \mathcal{I}(f(y)) $ and so $ f(x) = f(y) $ for all $ f \in \mathcal{H} $. The $ \mathcal{H}_r $-extremal points in $ X $ are again called $ \mathcal{H} $-extremal, the set of them is denoted $ \mathrm{Ch}_{\mathcal{H}}(X) $, and the closure of the latter set is denoted $ \check{S}_{\mathcal{H}}(X) $. The analogues of Props. 5 and 7 are the following:

#### Proposition 9 {#int-iv-s7-prop-9 .statement}

*For every function $ f \in \mathcal{H} $, $ \mathrm{Ch}_{\mathcal{H}}(X) $ intersects the set of points where $ |f| $ attains its supremum.*

We may limit ourselves to the case that $ f $ is not the constant 0. Let $ a $ be a point of $ X $ where $ |f| $ attains its supremum, and set $ g = f/f(a) $; then $ g(a) = 1 $ and $ |g(x)| \leq 1 $ for all $ x \in X $, whence

$$
\Re(g(a)) = 1 \quad \text{and} \quad \Re(g(x)) \leq 1 \quad \text{for all } x \in X.
$$

By Prop. 5 of No. 3 applied to $ \mathcal{H}_r $, there exists $ b \in \mathrm{Ch}_{\mathcal{H}}(X) $ where $ \Re((g(x)) $ attains its supremum 1, whence $ |g(b)| = 1 $ since $ |g(b)| \leq 1 $; it follows that $ |f(b)| = |(f(a)| \geq |f(x)| $ for all $ x \in X $.

#### Proposition 10 {#int-iv-s7-prop-10 .statement}

*Let $ F $ be a closed subset of $ X $. The following properties are equivalent:
a) $ F $ contains $ \check{S}_{\mathcal{H}}(X) $.
b) For every function $ f \in \mathcal{H} $, $ F $ intersects the set of points of $ X $ where $ |f| $ attains its supremum.
c) For every point $ x \in X $, there exists a positive measure $ \mu $ of total mass 1 on $ X $ such that $ \mathrm{Supp}(\mu) \subset F $ and $ f(x) = \int f d\mu $ for every function $ f \in \mathcal{H} $.
Let us prove the equivalence of the conditions a) and c): let $ f = f_1 + i f_2 $ with $ f_1, f_2 $ in $ \mathcal{H}_r $; the relation $ f(x) = \int f d\mu $ is equivalent to the two relations $ f_1(x) = \int f_1 d\mu $ and $ f_2(x) = \int f_2 d\mu $; it thus suffices to apply to $ \mathcal{H}_r $ the equivalence of the conditions $ a) $ and $ c) $ of Prop. 7 of No. 3. The fact that $ a) $ implies $ b) $ follows from Prop. 9. Let us show that $ b) $ implies $ a) $; this is a matter of seeing that if $ b) $ is verified, then, for every $ h \in \mathcal{H}_r $, F intersects the set of points where $ h $ attains its infimum in X. The condition $ b) $ implies that F is nonempty; since F is compact, there exists $ a \in F $ such that $ h(a) \leq h(y) $ for all $ y \in F $. Let $ f \in \mathcal{H} $ be such that $ h = \mathcal{R}(f) $; for every $ \varepsilon > 0 $, the function $ g = f - h(a) + \varepsilon $ belongs to $ \mathcal{H} $, and
$$
\mathcal{R}(g(y)) = h(y) - h(a) + \varepsilon \geq \varepsilon
$$
for all $ y \in F $. Let $ c $ be the supremum of $ |g| $ in X, and set $ b = c^2 / 2\varepsilon $; for every $ y \in F $,
$$
|g(y) - b|^2 = |g(y)|^2 - 2b \mathcal{R}((g(y))) + b^2 \leq c^2 - 2b\varepsilon + b^2 = b^2,
$$
in other words, the supremum in F of the function $ |g - b| $ is $ \leq b $. Since $ g - b \in \mathcal{H} $, the hypothesis on F implies that $ |g - b| \leq b $, whence
$$
b^2 \geq |g - b|^2 = |g|^2 - 2b \mathcal{R}(g) + b^2
$$
and so $ \mathcal{R}(g) \geq |g|^2 / 2b \geq 0 $; since $ \mathcal{R}(g) = h - h(a) + \varepsilon $, and $ \varepsilon > 0 $ is arbitrary, we have $ h \geq h(a) $, and $ h(a) $ is the infimum of $ h $ in X, which completes the proof.

#### Remark {#int-iv-s7-n4-rem-1 .statement}

If $ f $ is a continuous real function, a point where $ |f| $ attains its supremum is a point where one of the functions $ f, -f $ attains its supremum. For a vector space $ \mathcal{H} $ of continuous real functions satisfying the hypotheses of No. 3, the Props. 9 and 10 are thus trivial corollaries of Props. 5 and 7, respectively.

### 5. Applications: III. Algebras of continuous functions

#### Lemma 4 {#int-iv-s7-lem-4 .statement}

Let X be a compact space, $ \mathcal{H} $ a closed linear subspace of the Banach space $ \mathcal{C}(X; \mathbf{C}) $ (resp. $ \mathcal{C}(X; \mathbf{R}) $). Let a be a point of X admitting a countable fundamental system of neighborhoods; assume that, for any numbers c and d such that $ 0 < c < d < 1 $ and any open neighborhood U of a, there exists an $ f \in \mathcal{H} $ such that
$$
|f| \leq 1,\quad |f(a)| \geq d,\quad |f(x)| \leq c \text{ for all } x \in X - U.
$$
Then there exists a function $ u \in \mathcal{H} $ such that $ |u(x)| < |u(a)| $ for all $ x \neq a $.

Let $ (V_n) $ ($ n \geq 1 $) be a fundamental system of neighborhoods of $ a $, and let $ \lambda, \mu, \varepsilon $ be numbers such that
$$
0 < \lambda < 1,\quad 1 < \mu < \mu + \varepsilon \leq 1 + \lambda.
$$
Thus $ 0 < \lambda / \mu < 1 / \mu < 1 $. We are going to define, by induction on $ n $ ($ n \geq 1 $), a decreasing sequence $ (U_n) $ of open neighborhoods of $ a $ such that $ U_n \subset V_n $ for all $ n $, and a sequence $ (h_n) $ of functions in $ \mathcal{H} $ satisfying the relations
$$
\begin{align*}
(13_n) &\quad |h_n(x)| \leq \mu \quad \text{for all } x \in X \\
(14_n) &\quad h_n(a) = 1 \\
(15_n) &\quad |h_n(x)| \leq \lambda \quad \text{for all } x \in X - U_n \\
(16_n) &\quad \left| \sum_{j=1}^n \lambda^j h_j(y) \right| < \sum_{j=1}^{n+1} \lambda^j \quad \text{for all } y \in X.
\end{align*}
$$
Assume $ h_m $ and $ U_m $ defined for $ 1 \leq m < n $, satisfying the four preceding conditions (with $ n $ replaced by $ m $); on the other hand, set $ U_0 = X $.
The function $ \sum_{j=1}^{n-1} \lambda^j h_j $ (equal to 0 if $ n = 1 $) is continuous and takes the value $ \sum_{j=1}^{n-1} \lambda^j $ at the point $ a $; therefore there exists an open neighborhood $ U_n $ of $ a $, contained in $ U_{n-1} \cap V_n $, such that
$$
\left| \sum_{j=1}^{n-1} \lambda^j h_j(y) \right| < \sum_{j=1}^{n-1} \lambda^j + \varepsilon \lambda^n \quad \text{for all } y \in U_n.
$$
By hypothesis there exists a function $ f \in \mathcal{H} $ such that
$$
\begin{align*}
|f(x)| &\leq 1 \quad \text{for all } x \in X , \quad |f(a)| \geq 1 / \mu , \\
|f(x)| &\leq \lambda / \mu \quad \text{for } x \in X - U_n .
\end{align*}
$$
Set $ h_n = f / f(a) $; the relations $ (13_n) $, $ (14_n) $ and $ (15_n) $ then hold; set
$$
g = \sum_{j=1}^n \lambda^j h_j = \sum_{j=1}^{n-1} \lambda^j h_j + \lambda^n h_n .
$$
By (17) and $ (13_n) $, for $ y \in U_n $ we have
$$
|g(y)| < \sum_{j=1}^{n-1} \lambda^j + \varepsilon \lambda^n + \mu \lambda^n \leq \sum_{j=1}^{n+1} \lambda^j ,
$$

since $ \varepsilon + \mu \leq 1 + \lambda $; for $ x \in X - U_n $, we have $ |h_p(x)| \leq \lambda $ for $ 1 \leq p \leq n $, whence also
$$
|g(x)| \leq \sum_{j=2}^{n+1} \lambda^j < \sum_{j=1}^{n+1} \lambda^j,
$$
which completes the proof of $(16_n)$.

This being so, the series $ \sum_{n=1}^{\infty} \lambda^n h_n $ is normally convergent in $ X $ since $ \lambda < 1 $ and $ |h_n(x)| \leq \mu $ for all $ n $ and all $ x \in X $; let $ u $ be its sum, which belongs to $ \mathcal{H} $ since $ \mathcal{H} $ is closed. By the relation $(14_n)$, we have $ u(a) = \sum_{n=1}^{\infty} \lambda^n $; on the other hand if $ x \neq a $, there exists an integer $ n $ such that $ x \notin U_{n+1} $; therefore $ |h_{n+k}(x)| \leq \lambda $ for all $ k \geq 1 $ by the relation $(15_n)$; it follows, using $(16_n)$, that
$$
|u(x)| \leq \left| \sum_{j=1}^n \lambda^j h_j(x) \right| + \left| \sum_{j=n+1}^{\infty} \lambda^j h_j(x) \right| < \sum_{j=1}^{n+1} \lambda^j + \lambda \sum_{j=n+1}^{\infty} \lambda^j
$$
$$
= \sum_{j=1}^{\infty} \lambda^j = |u(a)|.
$$

#### Theorem 2 (E. Bishop) {#int-iv-s7-thm-2 .statement}

— *Let $ X $ be a compact space, $ \mathcal{A} $ a closed subalgebra of the complex Banach algebra $ \mathcal{C}(X; \mathbf{C}) $. Assume that $ \mathcal{A} $ contains the constants and separates the points of $ X $. Let $ a $ be a point of $ X $; the following conditions are equivalent:

a) There exists a function $ f \in \mathcal{A} $ such that $ |f(x)| < |f(a)| $ for all $ x \neq a $.

b) The point $ a $ is $ \mathcal{A} $-extremal and admits a countable fundamental system of neighborhoods.

a) $ \Rightarrow $ b): Let $ f \in \mathcal{A} $ be such that $ |f(a)| > |f(x)| $ for $ x \neq a $; by Prop. 9 of No. 4, $ a $ is an $ \mathcal{A} $-extremal point. On the other hand, if $ U_n $ is the set of $ x \in X $ such that $ |f(x)| > |f(a)| - 1/n $, then $ U_n $ is an open neighborhood of $ a $, and the intersection of the $ U_n $ reduces to $ a $; since $ X $ is compact, the $ U_n $ form a fundamental system of neighborhoods of $ a $ (GT, I, §9, No. 1, Th. 1).

b) $ \Rightarrow $ a): It suffices to verify that b) implies the hypotheses of Lemma 4. With the notations of that lemma, set $ \varepsilon = \log d / \log c $; thus $ 0 < \varepsilon < 1 $. Since $ a $ is an $ \mathcal{A}_r $-extremal point, there exists a function $ g \in \mathcal{A} $ such that
$$
\mathcal{R}(g) \geq 0,\quad \mathcal{R}(g(a)) \leq \varepsilon,\quad \mathcal{R}(g(x)) \geq 1 \text{ for } x \in X - U
$$

(No. 3, Prop. 6, b)). Set $ f = c^g $; since $ f $ is the sum of the normally convergent series $ \sum_{n=0}^{\infty} (\log c)^n g^n / n! $, we have $ f \in \mathcal{A} $ and

$$
|f| \leq 1,\quad |f(a)| \geq c^{\varepsilon} = d,\quad |f(x)| \leq c \text{ for } x \in X - U.
$$

Q.E.D.

#### Corollary {#int-iv-s7-n5-cor-1 .statement}

— *Suppose in addition that $ X $ is metrizable. Then the following properties are equivalent*:

a) *$ a $ is an $ \mathcal{A} $-extremal point of $ X $*.

b) *There exists $ u \in \mathcal{A} $ such that $ |u(x)| < |u(a)| $ for all $ x \neq a $*.

c) *Let $ \mathfrak{M} $ be the set of subsets $ M $ of $ X $ such that for every function $ f \in \mathcal{A} $, $ |f| $ attains its supremum in $ X $ at at least one point of $ M $. Then $ a $ belongs to all of the sets $ M \in \mathfrak{M} $*.

d) *Let $ \mathfrak{N} $ be the set of subsets $ N $ of $ X $ such that, for every function $ f \in \mathcal{A} $, $ \mathcal{R}(f) $ attains its supremum in $ X $ at at least one point of $ N $. Then $ a $ belongs to all of the sets $ N \in \mathfrak{N} $*.

*In other words*,

$$
\mathrm{Ch}_{\mathcal{A}}(X) = \bigcap_{M \in \mathfrak{M}} M = \bigcap_{N \in \mathfrak{N}} N.
$$

Since, in a metrizable space, every point admits a countable fundamental system of neighborhoods, the equivalence of $ a) $ and $ b) $ follows from Th. 2. Let us show that $ b) $ implies $ c) $: indeed, $ a $ is the unique point where $ |u| $ attains its supremum; on the other hand, $ c) $ implies $ a) $ because, for every $ f \in \mathcal{A} $, $ \mathrm{Ch}_{\mathcal{A}}(X) $ intersects the set of points where $ |f| $ attains its supremum (No. 4, Prop. 9). The same reasoning, using Prop. 5 of No. 3, shows that $ d) $ implies $ a) $. Finally, to see that $ b) $ implies $ d) $, we can restrict ourselves to the case that $ X $ does not reduce to the single point $ a $, therefore $ u(a) \neq 0 $; the function $ v = u/u(a) $ then belongs to $ \mathcal{A} $, and we have $ v(a) = 1 $ and $ |v(x)| < 1 $ for $ x \neq a $, whence $ \mathcal{R}(v(a)) = 1 $ and $ \mathcal{R}(v(x)) < 1 $ for $ x \neq a $. Since the function $ \mathcal{R}(v) $ attains its supremum only at the point $ a $, we have indeed $ a \in N $ for every $ N \in \mathfrak{N} $.

#### Example {#int-iv-s7-n5-exa-1 .statement}

— Let $ X_1 $ be the set of points $ (z_1, z_2) \in \mathbf{C}^2 $ such that $ |z_1|^2 + |z_2|^2 \leq 1 $ (the unit ball in $ \mathbf{R}^4 $) and let $ \mathcal{A}_1' $ be the set of restrictions to $ X_1 $ of the holomorphic functions, with values in $ \mathbf{C} $, defined in a neighborhood of $ X_1 $ in $ \mathbf{C}^2 $ (the neighborhood depending on the function considered); let $ \mathcal{A}_1 $ be the closure of $ \mathcal{A}_1' $ in $ \mathcal{C}(X_1; \mathbf{C}) $, which is obviously a closed complex subalgebra of $ \mathcal{C}(X_1; \mathbf{C}) $ and separates the points of $ X_1 $. Application of the 'maximum principle' for holomorphic functions shows that $ \mathrm{Ch}_{\mathcal{A}_1}(X_1) $ is the sphere $ S_3 $.

In the preceding definition, let us replace $ X_1 $ by the 'polydisk' $ X_2 $ defined by the relations $ |z_1| \leq 1 $ and $ |z_2| \leq 1 $, which yields subalgebras $ \mathcal{A}_2' $ and $ \mathcal{A}_2 $ (the closure of $ \mathcal{A}_2' $ of $ \mathcal{C}(X_2; \mathbf{C}) $. Here, the maximum principle shows that $ \mathrm{Ch}_{\mathcal{A}_2}(X_2) $ is the 'torus' defined by the relations $ |z_1| = 1 $ and $ |z_2| = 1 $.

From these results, one deduces that there does not exist an *analytic isomorphism* of an open neighborhood of $ X_1 $ onto an open neighborhood of $ X_2 $ that *transforms* $ X_1 $ *into* $ X_2 $; for, if $ v $ were the restriction to $ X_1 $ of such a mapping, one would have $ \mathcal{A}_2 = v \mathcal{A}_1 v^{-1} $ and so $ v $ would transform $ S_3 $ into a space homeomorphic to $ T^2 $, which is absurd since $ S_3 $ is simply connected but $ T^2 $ is not. One will observe, however, that the spaces $ X_1 $ and $ X_2 $ are *homeomorphic*, both being bounded convex sets in $ \mathbf{R}^4 $ with nonempty interior.*

### 6. Uniqueness of integral representations

Let E be a Hausdorff weak locally convex space (TVS, II, §6, No. 2), C a proper pointed convex cone in E. One knows that C is the set of elements $ \geqslant 0 $ of E for an order relation compatible with the vector space structure of E. When C is said to be lattice-ordered, it is of course the order induced on C by that of E that is understood.

#### Lemma 5 {#int-iv-s7-lem-5 .statement}

*Assume that C is weakly complete. Let $ \mathcal{A} $ be the set of restrictions to C of the continuous linear forms on E. Let $ (f_\lambda)_{\lambda \in \Lambda} $ be a finite family of elements of $ \mathcal{A} $, and $ f = \sup(f_\lambda) $. For every $ x \in C $, define*

$$
\overline{f}(x) = \sup \left( f(x_1) + f(x_2) + \cdots + f(x_n) \right),
$$

*the supremum being taken over the set $ S_x $ of sequences $ (x_1, x_2, \ldots, x_n) $ of elements of C such that $ x_1 + x_2 + \cdots + x_n = x $. Let $ \mathrm{Card}\, \Lambda = p $. Then there exists $ (y_1, \ldots, y_p) \in S_x $ such that $ \overline{f}(x) = f(y_1) + \cdots + f(y_p) $.

Denote by $ f_1, f_2, \ldots, f_p $ the elements of the family $ (f_\lambda) $. For $ k = 1, 2, \ldots, p $, let $ C_k $ be the set of $ y \in C $ such that

$$
f_1(y) < f(y),\ f_2(y) < f(y),\ \ldots,\ f_{k-1}(y) < f(y),\ f_k(y) = f(y).
$$

The $ C_k $ are disjoint convex cones with union C. Let $ x_1, x_2, \ldots, x_n $ in C be such that $ x_1 + x_2 + \cdots + x_n = x $. Let $ y_k $ be the sum of the $ x_i $ that belong to $ C_k $. Then $ y_1 + y_2 + \cdots + y_p = x $. Since $ f $ is affine on $ C_k $, $ f(y_1) + \cdots + f(y_p) = f(x_1) + \cdots + f(x_n) $. Therefore

$$
f(x) = \sup \left( f(y_1) + \cdots + f(y_p) \right),
$$

where $ (y_1, y_2, \ldots, y_p) $ runs over the set of sequences of $ p $ points of C such that $ y_1 + y_2 + \cdots + y_p = x $. Set $ D = C \cap (x - C) $. Since D is compact (TVS, II, §6, No. 8, Cor. 2 of Prop. 11), so is the set of elements $ (y_1, \ldots, y_p) $ of $ D^p $ such that $ y_1 + \cdots + y_p = x $, thus the supremum (19) is attained.

#### Lemma 6 {#int-iv-s7-lem-6 .statement}

We maintain the hypotheses and notations of Lemma 5, and assume the $ f_\lambda $ to be positive. The function $ \overline{f} $ is positively homogeneous, concave and upper semi-continuous in $ C $. It is affine if $ C $ is lattice-ordered.

It is clear that $ \overline{f} $ is positively homogeneous. Let $ x, y $ belong to $ C $. If $ x_1, \ldots, x_m, y_1, \ldots, y_n $ in $ C $ are such that $ x_1 + \cdots + x_m = x,\ y_1 + \cdots + y_n = y $, then $ x_1 + \cdots + x_m + y_1 + \cdots + y_n = x + y $, therefore

$$
f(x_1) + \cdots + f(x_m) + f(y_1) + \cdots + f(y_n) \leq \overline{f}(x + y);
$$

it follows that $ \overline{f}(x) + \overline{f}(y) \leq \overline{f}(x + y) $, therefore $ \overline{f} $ is concave. Let $ L $ (resp. $ L_\lambda $) be the set of $ (t, x) \in \mathbf{R} \times E $ such that $ x \in C $ and $ 0 \leq t \leq \overline{f}(x) $ (resp. $ 0 \leq t \leq f_\lambda(x) $). Each of the $ L_\lambda $ is closed in the weakly complete proper convex cone $ \mathbf{R}_+ \times C $, therefore the sum $ \sum_{\lambda \in \Lambda} L_\lambda $ is closed (TVS, II, §6, No. 8, Cor. 2 of Prop. 11). By Lemma 5, this sum is equal to $ L $. Therefore $ L $ is closed, which proves that $ \overline{f} $ is upper semi-continuous. Finally, assume $ C $ is lattice-ordered, and let us prove that $ \overline{f} $ is convex. Let $ x, y $ belong to $ C $ and let $ \varepsilon > 0 $. There exist $ z_1, z_2, \ldots, z_n $ in $ C $ such that $ f(z_1) + \cdots + f(z_n) \geq \overline{f}(x + y) - \varepsilon $ and $ z_1 + \cdots + z_n = x + y $. The vector space $ C - C $ is lattice-ordered for the order induced by that of $ E $ (A, VI, §1, No. 9, Prop. 8). By the decomposition theorem (*loc. cit.*, No. 10, Th. 1), there exist $ x_1, \ldots, x_n, y_1, \ldots, y_n $ in $ C $ such that

$$
x_1 + y_1 = z_1,\ \ldots,\ x_n + y_n = z_n,\ x_1 + \cdots + x_n = x,\ y_1 + \cdots + y_n = y.
$$

Then, since $ f $ is positively homogeneous and convex,

$$
\begin{align*}
\overline{f}(x + y) &\leq \varepsilon + f(z_1) + \cdots + f(z_n) \\
&\leq \varepsilon + f(x_1) + f(y_1) + \cdots + f(x_n) + f(y_n) \\
&\leq \varepsilon + \overline{f}(x) + \overline{f}(y).
\end{align*}
$$

Since $ \varepsilon $ is an arbitrary number $ > 0 $, we have proved that $ \overline{f} $ is indeed convex.

#### Theorem 3 (Choquet) {#int-iv-s7-thm-3 .statement}

*Let $ E $ be a Hausdorff weak locally convex space, $ C $ a weakly complete proper convex cone with vertex 0 in $ E $, $ G $ the union of the extremal generators of $ C $, $ K $ a compact convex subset of $ C $, $ \lambda $ and $ \lambda' $ positive measures of mass 1 on $ K $, admitting the same barycenter, such that $ \lambda^*(K - (K \cap G)) = \lambda'^*(K - (K \cap G)) = 0 $. Assume that $ C $ is lattice-ordered. Then, for every lower semi-continuous, positively homogeneous convex function $ f \geq 0 $ on $ C $, $ \lambda^*(f|K) = \lambda'^*(f|K) $.*

Let $ \mathcal{A} $ (resp. $ \mathcal{A}' $) be the set of restrictions to $ C $ of the continuous linear forms (resp. affine functions) on $ E $. We know (TVS, II, §5, No. 4, Remark 2) that $ f $ is the upper envelope of the set of elements of $ \mathcal{A} $ that are $ \leq f $. The set of functions of the form $ \sup(f_1, \ldots, f_p) $, where $ f_1, \ldots, f_p $ belong to $ \mathcal{A} $, $ f_1 \geq 0, \ldots, f_p \geq 0 $, is an increasing directed set and has $ f $ as its upper envelope. Taking into account §1, No. 1, Th. 1, it suffices to verify the equality $ \lambda(f|K) = \lambda'(f|K) $ when $ f $ is of the preceding form.

Define $ \overline{f} $ as in Lemma 5. It is clear that $ \overline{f}(y) = f(y) $ if $ y \in G $. Since $ \lambda^*(K - (K \cap G)) = 0 $, we have $ \lambda(f|K) = \lambda(\overline{f}|K) $. By Lemma 6, $ \overline{f} $ is affine and upper semi-continuous. Therefore $ \overline{f}|K $ is the lower envelope of a decreasing directed set of restrictions of elements of $ \mathcal{A}' $ to K (TVS, II, §5, No. 4, Prop. 6). Let $ x \in K $ be the barycenter of $ \lambda $. If $ g \in \mathcal{A} $ then $ \lambda(g|K) = g(x) $. Therefore $ \lambda(\overline{f}|K) = \overline{f}(x) $ (\S4, No. 4, Cor. 2 of Prop. 5). Thus $ \lambda(f|K) = \overline{f}(x) $, and one sees similarly that $ \lambda'(f|K) = \overline{f}(x) $.

#### Corollary {#int-iv-s7-n6-cor-1 .statement}

*Let E be a Hausdorff locally convex space, C a proper convex cone with vertex 0 in E, admitting a compact sole M, and let G be the union of the extremal generators of C. Let $ x \in M $. If C is lattice-ordered, then there exists at most one positive measure $ \lambda $ of mass 1 on M, such that $ \lambda^*(M - (G \cap M)) = 0 $, and admitting x as barycenter.*

Replacing the topology of E by the weakened topology (which does not change the topology of M), one can suppose E to be a weak space. Let $ \lambda $ and $ \lambda' $ be two measures on M having the stated properties, and let h be a continuous linear form on E such that M is the intersection of C and the hyperplane with equation $ h(x) = 1 $. Let $ \mathcal{S} $ be the subset of $ \mathcal{C}(M) $ consisting of the restrictions to M of the positively homogeneous and continuous convex functions $ \geq 0 $ on C. The cone C is weakly complete (TVS, II, §7, No. 3). By Th. 3, $ \lambda(f) = \lambda'(f) $ for every $ f \in \mathcal{S} $.

If $ f_1, f_2, f_3, f_4 $ belong to $ \mathcal{S} $, then
$$
\begin{align*}
\sup(f_1 - f_2, f_3 - f_4) &= \sup(f_1 + f_4, f_3 + f_2) - (f_2 + f_4) \in \mathcal{S} - \mathcal{S} \\
\inf(f_1 - f_2, f_3 - f_4) &= -\sup(f_2 - f_1, f_4 - f_3) \in \mathcal{S} - \mathcal{S}.
\end{align*}
$$
Since $ h|M \in \mathcal{S} $, $ \mathcal{S} - \mathcal{S} $ contains the constant functions. If x and y are two distinct points of M, there exists a continuous linear form on E that separates x and y, and this form is the difference of two continuous linear forms that are positive on C (TVS, II, §6, No. 8, Lemma 1). It follows from the foregoing that for $ \alpha, \beta $ real, there exists $ f \in \mathcal{S} - \mathcal{S} $ such that $ f(x) = \alpha, f(y) = \beta $. Then $ \mathcal{S} - \mathcal{S} $ is dense in $ \mathcal{C}(M) $ for the topology of uniform convergence (GT, X, §4, No. 1, Cor. of Prop. 2). Since $ \lambda $ and $ \lambda' $ coincide on $ \mathcal{S} - \mathcal{S} $, we have $ \lambda = \lambda' $.

Exercises

### Exercises {#int-iv-s7-exercises}

See the [exercises for § 7](exercises/s7/).
