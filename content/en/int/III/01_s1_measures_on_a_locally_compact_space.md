---
book: int
book_title: Integration
chapter: III
chapter_title: MEASURES ON LOCALLY COMPACT SPACES
section: 1
section_title: Measures on a locally compact space
lang: en
source: int-i-vi
pdf_pages: 0046-0068, 0100-0104
extraction: ocr
subsections:
    - "no": 1
      title: Continuous functions with compact support
      page: 0
      pdf_page: 46
    - "no": 2
      title: Approximation properties
      page: 4
      pdf_page: 49
    - "no": 3
      title: Definition of a measure
      page: 7
      pdf_page: 52
    - "no": 4
      title: Product of a measure by a continuous function
      page: 10
      pdf_page: 55
    - "no": 5
      title: Real measures. Positive measures
      page: 11
      pdf_page: 56
    - "no": 6
      title: Absolute value of a complex measure
      page: 13
      pdf_page: 58
    - "no": 7
      title: Definition of a measure by extension
      page: 15
      pdf_page: 60
    - "no": 8
      title: Bounded measures
      page: 16
      pdf_page: 61
    - "no": 9
      title: Vague topology on the space of measures
      page: 18
      pdf_page: 63
    - "no": 10
      title: Compact convergence in $ \mathcal{M}(X; \mathbf{C}) $
      page: 21
      pdf_page: 66
statements: 41
exercises: 18
content_sha256: bc8211586145aed194cdd73907ade3cd2ac5456da88b9bc1aea67c999d7f993a
---

## § 1. MEASURES ON A LOCALLY COMPACT SPACE

### 1. Continuous functions with compact support

#### Definition 1 {#int-iii-s1-def-1 .statement}

— Let X be a topological space, let E be either $ \overline{\mathbf{R}} $ or a vector space over $ \mathbf{R} $, and let f be a mapping of X into E. The smallest closed set S in X such that $ f(x) = 0 $ on $ X - S $ (in other words, the closure in X of the set of all $ x \in X $ such that $ f(x) \neq 0 $) is called the support of f and is denoted Supp(f).

Let X be a locally compact space, E a topological vector space over $ \mathbf{R} $ or $ \mathbf{C} $; recall that $ \mathcal{C}(X;E) $ denotes the vector space of continuous mappings of X into E; when $ E = \mathbf{R} $ or $ E = \mathbf{C} $, we will omit the mention of E in this notation if no confusion can result. We shall denote by $ \mathcal{K}(X;E) $ the subspace of $ \mathcal{C}(X;E) $ formed by the continuous mappings with compact support; for every subset A of X, we denote by $ \mathcal{C}(X,A;E) $ (resp. $ \mathcal{K}(X,A;E) $) the subspace of $ \mathcal{C}(X;E) $ (resp. $ \mathcal{K}(X;E) $) formed by the mappings f such that $ \operatorname{Supp}(f) \subset A $. If $ E = \mathbf{R} $ or $ E = \mathbf{C} $, we write $ \mathcal{K}(X) $ (resp. $ \mathcal{K}(X,A) $) instead of $ \mathcal{K}(X;\mathbf{R}) $ or $ \mathcal{K}(X;\mathbf{C}) $ (resp. $ \mathcal{K}(X,A;\mathbf{R}) $ or $ \mathcal{K}(X,A;\mathbf{C}) $), provided no confusion can result; we denote by $ \mathcal{K}_+(X) $ the pointed convex cone formed by the functions $ \geq 0 $ of $ \mathcal{K}(X;\mathbf{R}) $.

For every compact subset K of X, the space $ \mathcal{K}(X,K;E) $ may be identified with a subspace of the space of continuous functions $ \mathcal{C}(K;E) $ (namely, the subspace of continuous mappings of K into E that are zero on the boundary$^1$ of K). When $ \mathcal{C}(K;E) $ is equipped with the topology of uniform convergence in K, $ \mathcal{K}(X,K;E) $ is a closed subspace of $ \mathcal{C}(K;E) $. In particular, if E is a Fréchet space (resp. a Banach space), then so is $ \mathcal{K}(X,K;E) $, because if the topology of E is defined by the semi-norms $ p_n $ (resp. the norm $ x \mapsto \|x\| $) then the topology of $ \mathcal{K}(X,K;E) $ is defined

\footnotetext{1}{The original is frontière, also translated as 'frontier' (GT, I, §1, No. 6, Def. 11).}

by the semi-norms $ f \mapsto \sup_{x \in K} p_n(f(x)) $ (resp. the norm $ f \mapsto \sup_{x \in K} \|f(x)\| $, denoted $ \|f\| $).

The space $ \mathcal{K}(X; E) $ is the union of the increasing directed family of subspaces $ \mathcal{K}(X, K; E) $, where $ K $ runs over the set of compact subsets of $ X $; moreover, if $ K_1 \subset K_2 $ are two compact subsets of $ X $, the canonical injection $ \mathcal{K}(X, K_1; E) \to \mathcal{K}(X, K_2; E) $ is continuous for the topologies defined above. If $ E $ is *locally convex*, one can therefore define on $ \mathcal{K}(X; E) $ the *direct limit*² of the locally convex topologies of the $ \mathcal{K}(X, K; E) $ (TVS, II, §4, No. 4); unless expressly mentioned to the contrary, this will always be the topology in question when we regard $ \mathcal{K}(X; E) $ as a topological vector space.

#### Proposition 1 {#int-iii-s1-prop-1 .statement}

*Let $ X $ be a locally compact space, $ E $ a Hausdorff locally convex space.*

(i) *The locally convex space $ \mathcal{K}(X; E) $ is Hausdorff. For every compact subset $ K $ of $ X $, the topology on $ \mathcal{K}(X, K; E) $ induced by that of $ \mathcal{K}(X; E) $ is the topology of uniform convergence in $ K $, and each of the subspaces $ \mathcal{K}(X, K; E) $ is closed in $ \mathcal{K}(X; E) $.*

(ii) *If $ E $ is the product of a finite number of locally convex spaces $ E_i $ ($ 1 \leq i \leq n $), then the mapping $ f \mapsto (\mathrm{pr}_i \circ f) $ is an isomorphism of the space $ \mathcal{K}(X; E) $ onto the product space $ \prod_{1 \leq i \leq n} \mathcal{K}(X; E_i) $.*

(iii) *If $ X $ is the sum of a family $ (X_\lambda)_{\lambda \in L} $ of locally compact spaces, then the mapping $ f \mapsto (f|X_\lambda)_{\lambda \in L} $ is an isomorphism of the space $ \mathcal{K}(X; E) $ onto the topological direct sum space of the family $ (\mathcal{K}(X_\lambda; E))_{\lambda \in L} $.*

(i) Note that, on $ \mathcal{K}(X; E) $, the topology of uniform convergence *in* $ X $ is compatible with the vector space structure of $ \mathcal{K}(X; E) $ because, for every $ f \in \mathcal{K}(X; E) $, with (compact) support $ S $, the set $ f(X) = f(S) \cup \{0\} $ is compact, hence bounded in $ E $ (TVS, III, §3, No. 1, Prop. 1). Since this topology $ \mathcal{T}_0 $ is locally convex and induces on each $ \mathcal{K}(X, K; E) $ the topology of uniform convergence in $ K $, the same is true of the direct limit topology $ \mathcal{T} $ on $ \mathcal{K}(X; E) $ (TVS, II, §4, No. 4, *Remark*); moreover, $ \mathcal{T} $ is finer than $ \mathcal{T}_0 $ and $ \mathcal{T}_0 $ is Hausdorff, therefore $ \mathcal{T} $ is Hausdorff. Finally, suppose that a function $ f \in \mathcal{K}(X; E) $ belongs to the closure of $ \mathcal{K}(X, K; E) $; by the definitions, there exists a compact subset $ K' \supset K $ of $ X $ such that $ f \in \mathcal{K}(X, K'; E) $. By the foregoing, $ f $ belongs to the closure of $ \mathcal{K}(X, K; E) $ in the space $ \mathcal{K}(X, K'; E) $, hence belongs to $ \mathcal{K}(X, K; E) $.

(ii) The criterion for continuity in a direct limit (TVS, II, §4, No. 4, Prop. 5) shows at once that the mapping $ f \mapsto (\mathrm{pr}_i \circ f) $ is continuous and that the same is true of the inverse mapping (for the latter, it suffices to note that if, for every function $ f_i \in \mathcal{K}(X; E_i) $, one denotes by $ f'_i $ the mapping

² *Limite inductive*, translated as "direct limit" in S, A and GT.

of X into E such that $ \mathrm{pr}_i \circ f'_i = f_i $ and $ \mathrm{pr}_j \circ f'_i = 0 $ for $ j \neq i $, then each of the mappings $ f_i \mapsto f'_i $ is continuous).

(iii) Each compact subset K of X intersects only the $ X_\lambda $ of a finite sub-family $ (X_\lambda)_{\lambda \in H} $ of $ (X_\lambda)_{\lambda \in L} $, and it is immediate that if one sets $ K_\lambda = K \cap X_\lambda $ for $ \lambda \in H $, the mapping $ f \mapsto (f|X_\lambda)_{\lambda \in H} $ is an isomorphism of $ \mathcal{K}(X, K; E) $ onto $ \prod_{\lambda \in H} \mathcal{K}(X_\lambda, K_\lambda; E) $. Conversely, for every function $ f_\lambda \in \mathcal{K}(X_\lambda; E) $, let $ f''_\lambda $ be the mapping of X into E such that $ f''_\lambda|X_\lambda = f_\lambda $ and $ f''_\lambda|X_\mu = 0 $ for $ \mu \neq \lambda $; it is immediate that the mapping $ f_\lambda \mapsto f''_\lambda $ of $ \mathcal{K}(X_\lambda; E) $ into $ \mathcal{K}(X; E) $ is continuous. The assertion (iii) follows from these remarks and the criterion for continuity in direct limits (TVS, II, §4, No. 4, Prop. 5).

#### Proposition 2 {#int-iii-s1-prop-2 .statement}

— *Let X be a locally compact space, E a Hausdorff locally convex space.*

(i) *If E is a Fréchet space, then the space $ \mathcal{K}(X; E) $ is barreled.*

(ii) *If X is paracompact then, for every bounded set B in $ \mathcal{K}(X; E) $, there exists a compact subset K of X such that $ B \subset \mathcal{K}(X, K; E) $.*

Suppose E is a Fréchet space. Then, for every compact subset K of X, $ \mathcal{K}(X, K; E) $ is a Fréchet space, hence is barreled, and one knows that a direct limit of barreled spaces is barreled (TVS, III, §4, No. 1, Cor. 3 of Prop. 3), whence (i).

If X is paracompact, one knows (GT, I, §9, No. 10, Th. 5) that X is the sum of a family $ (X_\lambda)_{\lambda \in L} $ of locally compact spaces that are *countable at infinity*; thus (Prop. 1, (iii)), $ \mathcal{K}(X; E) $ is the *topological direct sum* of the family of subspaces $ \mathcal{K}(X_\lambda; E) $ ($ \lambda \in L $). By virtue of the characterization of the bounded sets in a topological direct sum (TVS, III, §1, No. 4, Prop. 5), every bounded set in $ \mathcal{K}(X; E) $ is contained in the sum of a *finite* number of subspaces $ \mathcal{K}(X_\lambda; E) $, and it will suffice to prove that every bounded set in $ \mathcal{K}(X_\lambda; E) $ is contained in a subspace $ \mathcal{K}(X_\lambda, K_\lambda; E) $, with $ K_\lambda $ compact in $ X_\lambda $. We are thus reduced to the case that X is countable at infinity, in other words is the union of a sequence of relatively compact open sets $ U_n $ such that $ \overline{U}_n \subset U_{n+1} $ (GT, I, §9, No. 9, Prop. 15). But then $ \mathcal{K}(X; E) $ is the *strict* direct limit of the sequence of spaces $ \mathcal{K}(X, \overline{U}_n; E) $, whence the assertion (ii) (TVS, III, §1, No. 4, Prop. 6).

We shall say that a subset H of $ \mathcal{K}(X; E) $ is *strictly compact* if it is compact and if there exists a compact subset K of X such that $ H \subset \mathcal{K}(X, K; E) $. It follows at once from Proposition 2 that if X is a *paracompact* locally compact space and if E is Hausdorff, then *every compact set* in $ \mathcal{K}(X; E) $ is *strictly compact*. One can give examples of locally compact

3 *Dénombrable à l'infini*, also translated as "σ-compact" (GT, I, §9, No. 9, Def. 5).

spaces $ X $ (not paracompact) such that there exist sets in $ \mathcal{K}(X; \mathbf{R}) $ that are *compact but not strictly compact* (Exercises 3 and 4).

We recall that, by virtue of Ascoli’s theorem (GT, X, §2, No. 5, Cor. 3 of Th. 2), a strictly compact subset $ H $ of $ \mathcal{K}(X; E) $ contained in $ \mathcal{K}(X, K; E) $ is characterized by the following conditions: $ 1^\circ $ it is closed; $ 2^\circ $ it is equicontinuous; $ 3^\circ $ for every $ x \in K $, the set $ H(x) $ is relatively compact in $ E $.

#### Corollary {#int-iii-s1-n1-cor-1 .statement}

*Let $ X $ be a paracompact, locally compact space; if $ E $ is a quasi-complete locally convex space, then the space $ \mathcal{K}(X; E) $ is quasi-complete.*

It suffices, by virtue of Proposition 2, (ii), to note that for every compact subset $ K $ of $ X $, $ \mathcal{K}(X, K; E) $ is a closed subspace of $ C(K; E) $, which is quasi-complete since every bounded subset of $ C(K; E) $ consists of functions taking values in a same bounded subset of $ E $.

### 2. Approximation properties

#### Lemma 1 {#int-iii-s1-lem-1 .statement}

*Let $ X $ be a locally compact space, $ K $ a compact subset of $ X $, and $ (V_k)_{1 \leq k \leq n} $ a finite covering of $ K $ by open sets of $ X $. Then, there exist $ n $ continuous mappings $ f_k $ of $ X $ into $ [0, 1] $, such that the support of $ f_k $ is contained in $ V_k $ for $ 1 \leq k \leq n $ and such that $ \sum_{k=1}^n f_k(x) \leq 1 $ for all $ x \in X $ and $ \sum_{k=1}^n f_k(x) = 1 $ for all $ x \in K $.

For, let $ X' $ be the compact space obtained by adjoining to $ X $ a point at infinity $ \omega $ (GT, I, §9, No. 8, Th. 4); the sets $ V_0 = X' - K $ and $ V_k $ ($ 1 \leq k \leq n $) form an open covering of $ X' $. Let $ (f_k)_{0 \leq k \leq n} $ be a continuous partition of unity subordinate to this covering of $ X' $ (GT, IX, §4, No. 3, Prop. 3); the functions $ f_k $ with index $ k \geq 1 $ satisfy the conditions of the lemma.

#### Lemma 2 {#int-iii-s1-lem-2 .statement}

*Let $ X $ be a locally compact space, $ K $ a compact subset of $ X $, $ E $ a locally convex space, $ q $ a continuous semi-norm on $ E $, and $ \Phi $ an equicontinuous set of mappings of $ X $ into $ E $ whose supports are contained in $ K $. Then, for every $ \varepsilon > 0 $, there exists a continuous partition of unity $ (\varphi_j)_{0 \leq j \leq n} $ on $ X $ having the following properties:
(i) $ \operatorname{Supp}(\varphi_j) \subset K $ for $ 1 \leq j \leq n $.
(ii) *If, for $ 1 \leq j \leq n $, $ x_j $ is any point of $ \operatorname{Supp}(\varphi_j) $, then, for every function $ f \in \Phi $ and every $ x \in X $,
$$
q\left(f(x) - \sum_{j=1}^n \varphi_j(x) f(x_j)\right) \leq \varepsilon.
$$*

For every $ y $ belonging to the boundary of $ K $, one has $ f(y) = 0 $ for all $ f \in \Phi $, therefore there exists an open neighborhood $ V_y $ of $ y $ in $ X $ such that, for every $ z \in V_y $ and every $ f \in \Phi $, one has $ q(f(z)) \leq \varepsilon/2 $. Let $ K' $ be the set of points of $ K $ not belonging to any of the $ V_y $ as $ y $ runs over the boundary of $ K $; $ K' $ is compact and is contained in the interior of $ K $. The set $ \Phi $ is uniformly equicontinuous in $ K $; therefore, there exists a finite open covering $ (U_j)_{1 \leq j \leq n} $ of $ K' $ consisting of open sets in $ X $ contained in $ K $, such that for every pair of points $ x, y $ of a same $ U_j $, one has $ q(f(x) - f(y)) \leq \varepsilon/2 $ for every $ f \in \Phi $. By Lemma 1, there exist $ n $ continuous mappings $ \varphi_j $ of $ X $ into $[0, 1]$ ($ 1 \leq j \leq n $) such that $ \operatorname{Supp}(\varphi_j) \subset U_j $ and such that
$$
\sum_{j=1}^n \varphi_j(x) \leq 1 \text{ on } X \text{ and } \sum_{j=1}^n \varphi_j(x) = 1 \text{ on } K'.
$$
For $ x_j \in \operatorname{Supp}(\varphi_j) $ ($ 1 \leq j \leq n $) and $ f \in \Phi $, we therefore have, for all $ x \in U_j $,
$$
q(f(x)\varphi_j(x) - f(x_j)\varphi_j(x)) = \varphi_j(x)q(f(x) - f(x_j)) \leq \frac{\varepsilon}{2}\varphi_j(x),
$$
and this relation remains true if $ x \notin U_j $ since then $ \varphi_j(x) = 0 $. By addition we infer that, for every $ x \in X $,
$$
q\left(f(x)(1 - \varphi_0(x)) - \sum_{j=1}^n \varphi_j(x)f(x_j)\right) \leq \frac{\varepsilon}{2}(1 - \varphi_0(x)),
$$
where $ \varphi_0 = 1 - \sum_{j=1}^n \varphi_j $; whence (1) for $ x \in K' $, since then $ \varphi_0(x) = 0 $;
(1) also holds for $ x \notin K $, the first member then being zero. Finally, for $ x \in K - K' $ we have $ q(f(x)\varphi_0(x)) \leq \varepsilon/2 $ by the definition of $ K' $, therefore this relation and (2) again imply (1) in this case.

Let $ X $ be a locally compact space; for every Banach space $ E $ (real or complex) we denote by $ \mathcal{C}^b(X; E) $ the vector space of continuous and bounded mappings of $ X $ into $ E $; we know that the topology of uniform convergence in $ X $ is compatible with the vector space structure (real, resp. complex) of $ \mathcal{C}^b(X; E) $, and it is defined by the norm
$$
||f|| = \sup_{x \in X} ||f(x)||.
$$
Moreover, the normed space thus defined is a Banach space (GT, X, §3, No. 2, and No. 1, Cor. 2 of Prop. 2); the topology defined by this norm on $ \mathscr{K}(X; E) $ (in other words, the topology of uniform convergence in $ X $) is coarser than the direct limit topology on $ \mathscr{K}(X; E) $ defined in No. 1.

#### Proposition 3 {#int-iii-s1-prop-3 .statement}

— Let $ X $ be a locally compact space, $ X' $ the compact space obtained by adjoining to $ X $ a point at infinity $ \omega $ (GT, I, §9, No. 8,

Th. 4), and E a Banach space. The closure of $ \mathcal{K}(X;E) $ in the normed space $ C^b(X;E) $ is the vector space of continuous functions on X, with values in E and tending to 0 at the point $ \omega $.

Let $ f \in C^b(X;E) $ be a function in the closure of $ \mathcal{K}(X;E) $; for every $ \varepsilon > 0 $, there exists a function $ g \in \mathcal{K}(X;E) $ such that $ \|f(x) - g(x)\| \leq \varepsilon $ for all $ x \in X $; if K is the support of g, it follows that $ \|f(x)\| \leq \varepsilon $ for all $ x \in \mathbf{C}K $, thus $ f(x) $ tends to 0 as $ x $ tends to $ \omega $. Conversely, if f has this property then, for every $ \varepsilon > 0 $, there exists a compact set $ K \subset X $ such that $ \|f(x)\| \leq \varepsilon $ for all $ x \in \mathbf{C}K $. By Lemma 1 there exists a continuous mapping h of X into $[0,1]$, with compact support, equal to 1 on K; then $ \|f(x)h(x)\| \leq \varepsilon $ on $ \mathbf{C}K $ and $ f(x) = f(x)h(x) $ on K; since $ fh $ has compact support and $ \|f(x) - f(x)h(x)\| \leq 2\varepsilon $ for all $ x \in X $, the proposition is proved.

We shall denote by $ C^0(X;E) $ the subspace of $ C^b(X;E) $ formed by the functions tending to zero at the point at infinity $ \omega $; it is thus the completion of the normed space $ \mathcal{K}(X;E) $.

#### Proposition 4 {#int-iii-s1-prop-4 .statement}

— Let X be a locally compact space, E a locally convex space; then, the space $ \mathcal{K}(X;E) $ is dense in $ C(X;E) $ for the topology of compact convergence.

For every compact set $ K \subset X $, there exists a function $ h \in \mathcal{K}(X;\mathbf{R}) $ equal to 1 on K, by Lemma 1; for every function $ f \in C(X;E) $ the function $ hf $, which belongs to $ \mathcal{K}(X;E) $, is equal to f on K, whence our assertion.

#### Proposition 5 {#int-iii-s1-prop-5 .statement}

— Let X be a locally compact space, E a real (resp. complex) locally convex space. For every compact subset K of X, the vector space $ \mathcal{K}(X,K;\mathbf{R}) \otimes_{\mathbf{R}} E $ (resp. $ \mathcal{K}(X,K;\mathbf{C}) \otimes_{\mathbf{C}} E $) (identified with a set of mappings of X into E, cf. A, II, §7, No. 7, Cor. of Prop. 15) is dense in $ \mathcal{K}(X,K;E) $; the vector space $ \mathcal{K}(X;\mathbf{R}) \otimes_{\mathbf{R}} E $ (resp. $ \mathcal{K}(X;\mathbf{C}) \otimes_{\mathbf{C}} E $) is dense in $ \mathcal{K}(X;E) $.

As the second assertion is an obvious consequence of the first, it suffices to prove the latter. We apply Lemma 2 with $ \Phi $ reduced to a single element $ f $ of $ \mathcal{K}(X,K;E) $; then, for every $ x \in X $,

$$
q\left(f(x) - \sum_{j=1}^n \varphi_j(x)f(x_j)\right) \leq \varepsilon,
$$

where the $ \varphi_j $ belong to $ \mathcal{K}(X,K;\mathbf{R}) $; since the mapping $ x \mapsto \sum_{j=1}^n \varphi_j(x)f(x_j) $ may be canonically identified with the element $ \sum_{j=1}^n \varphi_j \otimes f(x_j) $, this proves the proposition, by the definition of the topology of $ \mathcal{K}(X,K;E) $.

### 3. Definition of a measure

#### Definition 2 {#int-iii-s1-def-2 .statement}

— *A continuous linear form on* $ \mathcal{K}(X; \mathbf{C}) $, *X a locally compact space*, *is called a measure* (or *complex measure*) *on X*.

If $ \mu $ is a measure on a locally compact space $ X $, the value of the measure for a function $ f \in \mathcal{K}(X; \mathbf{C}) $ is called the *integral of f with respect to* $ \mu $; besides the general notations $ \mu(f) $ and $ \langle f, \mu \rangle $, one also uses the notations $ \int f d\mu $, $ \int f \mu $, $ \int f(x) d\mu(x) $ and $ \int f(x) \mu(x) $ to denote it; as to the use of the letter $ x $, see S, I, §1, No. 1.

By virtue of the criterion for continuity in direct limits (TVS, Ch. II, §4, No. 4, Prop. 5), to say that $ \mu $ is a measure on $ X $ means that $ \mu $ is a linear form on $ \mathcal{K}(X; \mathbf{C}) $ satisfying the following condition: for every compact subset $ K $ of $ X $, there exists a number $ M_K $ such that, for every function $ f \in \mathcal{K}(X; \mathbf{C}) $ *whose support is contained in* $ K $,

$$
| \mu(f) | \leq M_K \cdot \| f \| \quad \text{(where } \| f \| = \sup_{x \in X} |f(x)| ).
$$

More generally:

#### Proposition 6 {#int-iii-s1-prop-6 .statement}

— *Let X be a locally compact space, ($ K_\alpha $) a family of compact subsets of X whose interiors $ \overset{\circ}{K}_\alpha $ form an open covering of X. For a linear form $ \mu $ on $ \mathcal{K}(X; \mathbf{C}) $ to be a measure on X, it is necessary and sufficient that, for every $ \alpha $, there exist a number $ M_\alpha $ such that*

$$
| \mu(f) | \leq M_\alpha \cdot \| f \|
$$

*for every function* $ f \in \mathcal{K}(X, K_\alpha; \mathbf{C}) $.

The condition being obviously necessary, it suffices to prove that (5) implies (4) for every compact subset $ K $ of $ X $. Now, $ K $ is covered by a finite number of open sets $ \overset{\circ}{K}_{\alpha_i} $ ($ 1 \leq i \leq n $); applying Lemma 1 of No. 2 to $ K $ and to the $ \overset{\circ}{K}_{\alpha_i} $, there exist continuous functions $ g_i \geq 0 $ on $ X $ such that $ \operatorname{Supp}(g_i) \subset K_{\alpha_i} $, $ 0 \leq \sum_{i=1}^n g_i(x) \leq 1 $ for all $ x \in X $ and $ \sum_{i=1}^n g_i(x) = 1 $ for $ x \in K $. For every function $ f \in \mathcal{K}(X, K; \mathbf{C}) $, we can therefore write $ f = \sum_{i=1}^n f g_i $ and we have $ f g_i \in \mathcal{K}(X, K_{\alpha_i}; \mathbf{C}) $ and $ \| f g_i \| \leq \| f \| $; if $ M_K = \sum_{i=1}^n M_{\alpha_i} $, we then have the relation (4).

We denote by $ \mathcal{M}(X; \mathbf{C}) $, or simply $ \mathcal{M}(X) $ if no confusion can result, the vector space of measures on $ X $, in other words, the *dual* of $ \mathcal{K}(X; \mathbf{C}) $.

One knows that for every set $\mathscr{S}$ of *bounded* subsets of $\mathscr{K}(X;\mathbf{C})$, there is defined on $\mathscr{M}(X;\mathbf{C})$ the $\mathscr{S}$-topology, which is locally convex (TVS, III, §3, No. 1, Cor. of Prop. 1). We denote the topological vector space, obtained by equipping $\mathscr{M}(X;\mathbf{C})$ with the $\mathscr{S}$-topology, by $\mathscr{M}_{\mathscr{S}}(X;\mathbf{C})$ or $\mathscr{M}_{\mathscr{S}}(X)$.

#### Proposition 7 {#int-iii-s1-prop-7 .statement}

*For every set $\mathscr{S}$ of bounded subsets of $\mathscr{K}(X;\mathbf{C})$ that is a covering of $\mathscr{K}(X;\mathbf{C})$, the space $\mathscr{M}_{\mathscr{S}}(X;\mathbf{C})$ is Hausdorff and quasi-complete.*

This results from the fact that $\mathscr{K}(X;\mathbf{C})$ is barreled (TVS, III, §4, No. 2, Cor. 4 of Th. 1).

*Examples of measures.* — I. *Atomic measures.* Let X be a locally compact space, $a$ a point of X; the mapping $f\mapsto f(a)$ of $\mathscr{K}(X;\mathbf{C})$ into $\mathbf{C}$ obviously satisfies the condition (4) with $M_K=1$ for every compact subset K of X containing $a$, hence is a measure on X, which is denoted by $\varepsilon_a$; it is called the *Dirac measure* at the point $a$, or the measure defined by a *unit mass placed at the point $a$.*

More generally, let $\alpha$ be a mapping of X into $\mathbf{C}$ such that, for every compact subset K of X,
$$
\sum_{x\in K}|\alpha(x)|<+\infty.
$$
Then, for every function $f\in\mathscr{K}(X,K;\mathbf{C})$, the sum
$$
\mu(f)=\sum_{x\in X}\alpha(x)f(x)
$$
is defined, being equal to
$$
\sum_{x\in K}\alpha(x)f(x);
$$
it is clear that $\mu$ is a linear form on $\mathscr{K}(X;\mathbf{C})$ and that, for $f\in\mathscr{K}(X,K;\mathbf{C})$,
$$
|\mu(f)|\leq\left(\sum_{x\in K}|\alpha(x)|\right)\cdot\|f\|,
$$
in other words the condition (4) is satisfied.

A measure $\mu$ on X is said to be *atomic* if there exists a mapping $\alpha$ of X into $\mathbf{C}$ such that
$$
\sum_{x\in K}|\alpha(x)|<+\infty
$$
for every compact subset K of X, and such that $\mu$ is equal to the measure defined as above. If N is the set of $x\in X$ such that $\alpha(x)\neq0$, the condition imposed on $\alpha$ implies that for every compact subset K of X, $K\cap N$ is *countable*. One also says that $\mu$ is defined by the *masses* $\alpha(x)$ *placed at the points* $x\in N$. If one assumes that $N\cap K$ is *finite* for every compact set $K\subset X$, then obviously
$$
\sum_{x\in K}|\alpha(x)|<+\infty;
$$
it comes to the same to say that N is a *closed* and *discrete* subspace of X, because then every point of X has a compact neighborhood containing only a finite number of points of N, and conversely, if this is the case, then every compact subset of X can be covered by a finite number of such neighborhoods. When N is closed and discrete, every atomic measure defined by a function $\alpha$ such that $\alpha(x)=0$ on $\mathbf C N$ is called a discrete measure on X (cf. §2, No. 5).

### II. *Lebesgue measure.* For every function $f\in\mathcal K(\mathbf R;\mathbf C)$, there exists a compact interval $[a,b]$ of $\mathbf R$ outside of which $f$ is zero. The integral

$$
\mathrm I(f)=\int_{-\infty}^{+\infty}f(x)\,dx=\int_a^b f(x)\,dx
$$

is therefore defined; moreover, by the theorem of the mean (FRV, II, §1, No. 5, Prop. 6), we have $|\mathrm I(f)|\leq(b-a)\|f\|$; this shows that $f\mapsto\mathrm I(f)$ is a measure on $\mathbf R$, which is called *Lebesgue measure*.

For every interval J (bounded or not) of $\mathbf R$, one similarly calls *Lebesgue measure on J* the measure $f\mapsto\int_Jf(x)\,dx$, a linear form on $\mathcal K(J;\mathbf C)$ (the integral having meaning since there exists a compact interval $[a,b]$ contained in J outside of which $f$ is zero).

### III. Let $g$ be a continuous mapping of a compact interval $I\subset\mathbf R$ into $\mathbf C$, having a continuous derivative in I. Let $\Gamma=g(I)$, which is a compact subspace of $\mathbf C$; the mapping

$$
f\mapsto\int_I f(g(t))g'(t)\,dt
$$

of $\mathcal C(\Gamma;\mathbf C)$ into $\mathbf C$ is a continuous linear form by virtue of the theorem of the mean, hence is a *complex measure on $\Gamma$*; the integral relative to this measure is also written $\int_\Gamma f(z)\,dz$, even though it depends not only on $\Gamma$ but also on $g$.

#### Remark {#int-iii-s1-n3-rem-1 .statement}

The giving of a measure $\mu$ on a locally compact space X defines on X (along with the topology of X) a structure $\mathscr S$. Let $X_1$ be a second set, $\varphi$ a bijective mapping of X onto $X_1$; in conformity with general definitions (S, R, §8), the structure $\mathscr S_1$ obtained by *transporting* to $X_1$ the structure $\mathscr S$ of X, by means of $\varphi$, is defined in the following way. The topology of X is transported to $X_1$ by $\varphi$; the functions of $\mathcal K(X_1;\mathbf C)$ are then the functions $f$ such that $f\circ\varphi$ belongs to $\mathcal K(X;\mathbf C)$, and the measure $\mu_1$ on $X_1$ is defined by $\mu_1(f)=\mu(f\circ\varphi)$.

In particular, an *automorphism* of the structure $\mathscr S$ is a homeomorphism $\sigma$ of X onto itself, such that

$$
\mu(f)=\mu(f\circ\sigma)
$$

for every function $f\in\mathcal K(X;\mathbf C)$; the measure $\mu$ is then also said to be *invariant under the homeomorphism* $\sigma$.

#### Example {#int-iii-s1-n3-exa-1 .statement}

Lebesgue measure on $ \mathbf{R} $ is invariant under every translation of the additive group $ \mathbf{R} $. Indeed, for every function $ f \in \mathcal{K}(\mathbf{R}; \mathbf{C}) $ and every real number $ a $, we have

$$
\int_{-\infty}^{+\infty} f(x + a)\, dx = \int_{-\infty}^{+\infty} f(t)\, dt
$$

by the change-of-variables formula (FRV, II, §2, No. 1, formula (1)). For a generalization, see Ch. VII, §1, No. 2, Th. 1.

### 4. Product of a measure by a continuous function

Let $ X $ be a locally compact space, $ g $ a continuous mapping of $ X $ into $ \mathbf{C} $. It is clear that $ f \mapsto gf $ is a linear mapping of $ \mathcal{K}(X; \mathbf{C}) $ into itself; let us show that this mapping is continuous. Indeed, for every compact subset $ K $ of $ X $, and for every function $ f \in \mathcal{K}(X, K; \mathbf{C}) $, we have $ gf \in \mathcal{K}(X, K; \mathbf{C}) $; moreover, if $ b_K = \sup_{x \in K} |g(x)| $ then $ \|gf\| \leq b_K \|f\| $, whence our assertion (TVS, II, §4, No. 4, Prop. 5). The transpose of this continuous linear mapping (TVS, II, §6, No. 4) is therefore a linear mapping of $ \mathcal{M}(X; \mathbf{C}) $ into itself, which is denoted $ \mu \mapsto g \cdot \mu $ (or $ \mu \mapsto g\mu $, if no confusion can result). If $ \nu = g \cdot \mu $ we therefore have, for every function $ f \in \mathcal{K}(X; \mathbf{C}) $,

$$
\langle f, \nu \rangle = \langle gf, \mu \rangle
$$

or again

$$
\int f(x)\, d\nu(x) = \int f(x)g(x)\, d\mu(x)
$$

(which is abbreviated in the form $ d\nu(x) = g(x)\, d\mu(x) $). One says that $ g \cdot \mu $ is the product of the measure $ \mu $ by the function $ g $, or also the measure with density $ g $ with respect to $ \mu $ (cf. Ch. V, §5, No. 2, Def. 2). If $ g_1, g_2 $ are two continuous mappings of $ X $ into $ \mathbf{C} $, and $ \mu_1, \mu_2 $ are two measures on $ X $, then

$$
(g_1 + g_2) \cdot \mu = g_1 \cdot \mu + g_2 \cdot \mu, \quad g \cdot (\mu_1 + \mu_2) = g \cdot \mu_1 + g \cdot \mu_2,
$$
$$
(g_1 g_2) \cdot \mu = g_1 \cdot (g_2 \cdot \mu).
$$

Moreover, $ 1 \cdot \mu = \mu $ (here 1 denotes the constant function equal to 1 on $ X $); the set $ \mathcal{M}(X; \mathbf{C}) $, equipped with the external law of composition $ (g, \mu) \mapsto g \cdot \mu $ and with its additive structure, is thus a module over the ring $ \mathcal{C}(X; \mathbf{C}) $.

### 5. Real measures. Positive measures

Let X be a locally compact space. The real vector space $ \mathcal{K}(X; \mathbf{R}) $ is a subspace of the real vector space underlying the complex vector space $ \mathcal{K}(X; \mathbf{C}) $; moreover, the mapping $ (f_1, f_2) \mapsto f_1 + i f_2 $ is an *isomorphism* of the product topological vector space $ \mathcal{K}(X; \mathbf{R}) \times \mathcal{K}(X; \mathbf{R}) $ onto the real topological vector space $ \mathcal{K}(X; \mathbf{C}) $ (No. 1, Prop. 1).

For every (complex) measure $ \mu \in \mathcal{M}(X; \mathbf{C}) $, the restriction $ \mu_0 $ of $ \mu $ to $ \mathcal{K}(X; \mathbf{R}) $ is a continuous $ \mathbf{R} $-linear mapping of $ \mathcal{K}(X; \mathbf{R}) $ into $ \mathbf{C} $; moreover, this restriction determines $ \mu $, since if $ f = f_1 + i f_2 $ with $ f_1, f_2 $ in $ \mathcal{K}(X; \mathbf{R}) $, then $ \mu(f) = \mu_0(f_1) + i \mu_0(f_2) $. Conversely, let $ \mu_0 $ be a continuous $ \mathbf{R} $-linear mapping of $ \mathcal{K}(X; \mathbf{R}) $ into $ \mathbf{C} $; it is clear that the mapping

$$
f_1 + i f_2 \mapsto \mu_0(f_1) + i \mu_0(f_2)
$$

is a (complex) measure on X. Thus, every measure on X may be identified with its restriction to $ \mathcal{K}(X; \mathbf{R}) $.

Let $ \mu $ be a measure on X. One calls *conjugate measure* of $ \mu $ the measure $ \overline{\mu} $ defined by $ \overline{\mu}(f) = \overline{\mu(\overline{f})} $ for every function $ f \in \mathcal{K}(X; \mathbf{C}) $; for, it is clear that $ \overline{\mu} $ is a C-linear form and that it is continuous on $ \mathcal{K}(X; \mathbf{C}) $; obviously $ \overline{\mu} = \mu $, and, for two measures $ \mu, \nu $ and two scalars $ \alpha, \beta $ in $ \mathbf{C} $,

$$
(\alpha \mu + \beta \nu) = \overline{\alpha} \cdot \overline{\mu} + \overline{\beta} \cdot \overline{\nu}.
$$

More generally, for every function $ g \in \mathcal{C}(X; \mathbf{C}) $ and every measure $ \mu $ on X,

$$
g \cdot \overline{\mu} = \overline{g} \cdot \overline{\mu},
$$

as is immediate from the definition (No. 4).

A measure $ \mu $ on X is said to be *real* if $ \overline{\mu} = \mu $; by the foregoing, it is the same to say that for every function $ f \in \mathcal{K}(X; \mathbf{R}) $, $ \mu(f) $ is a *real* number. If one identifies a real measure with its restriction to $ \mathcal{K}(X; \mathbf{R}) $, one can thus say that the set of real measures on X is the *dual* of the real locally convex space $ \mathcal{K}(X; \mathbf{R}) $; it is a real vector space that is denoted $ \mathcal{M}(X; \mathbf{R}) $ (or sometimes $ \mathcal{M}(X) $ if this does not cause any confusion). The Lebesgue measure on $ \mathbf{R} $ is a *real* measure, as is the Dirac measure $ \varepsilon_a $ for every point $ a \in X $. If $ g \in \mathcal{C}(X; \mathbf{R}) $ and if $ \mu $ is a real measure, then so is $ g \cdot \mu $ by virtue of (7).

Let $ \mu $ be a (complex) measure on X. It follows from the preceding definition that the measures $ \mu_1 = (\mu + \overline{\mu})/2 $ and $ \mu_2 = (\mu - \overline{\mu})/2i $ are *real*; they are called, respectively, the *real part* and the *imaginary part* of $ \mu $, and they are denoted by $ \mathcal{R}\mu $ and $ \mathcal{I}\mu $, respectively; these measures are also characterized by the fact that, for every function $ f \in \mathcal{K}(X; \mathbf{R}) $,

$$
\mu_1(f) = \mathcal{R}(\mu(f)) , \quad \mu_2(f) = \mathcal{I}(\mu(f)).
$$

Obviously
$$
\mu = \mu_1 + i \mu_2,\quad \overline{\mu} = \mu_1 - i \mu_2.
$$

The space $ \mathcal{K}(X; \mathbf{R}) $ of continuous real-valued functions on $ X $ with compact support is clearly a *Riesz space* for the order relation $ f \leq g $. We shall say that a real measure $ \mu $ on $ X $ is *positive* if $ \mu(f) \geq 0 $ for every function $ f \geq 0 $ belonging to $ \mathcal{K}(X; \mathbf{R}) $; it is thus a positive linear form on the Riesz space $ \mathcal{K}(X; \mathbf{R}) $ (Ch. II, §2, No. 1, Def. 1). Conversely:

#### Theorem 1 {#int-iii-s1-thm-1 .statement}

*Every positive linear form on the Riesz space $ \mathcal{K}(X; \mathbf{R}) $ is a (positive) real measure on $ X $.*

For, let $ \mu $ be a positive linear form on $ \mathcal{K}(X; \mathbf{R}) $ and let $ K $ be a compact subset of $ X $. There exists a continuous mapping $ f_0 $ of $ X $ into $[0, 1]$, with compact support, such that $ f_0(x) = 1 $ on $ K $ (No. 2, Lemma 1). For every function $ g \in \mathcal{K}(X, K; \mathbf{R}) $, we thus have $ -\|g\|f_0 \leq g \leq \|g\|f_0 $, consequently $ |\mu(g)| \leq \|g\| \cdot \mu(f_0) $, which proves the theorem.

We denote by $ \mathcal{M}_+(X) $ the pointed convex cone of positive measures on $ X $ (or, what amounts to the same thing, the cone of positive linear forms on the Riesz space $ \mathcal{K}(X; \mathbf{R}) $).

#### Theorem 2 {#int-iii-s1-thm-2 .statement}

*Every real measure on a locally compact space $ X $ is the difference of two positive measures.*

In view of Theorem 1 and Ch. II, §2, No. 2, Th. 1, it all comes down to proving that a real measure $ \mu $ on $ X $ is a *relatively bounded* linear form on the Riesz space $ \mathcal{K}(X; \mathbf{R}) $. Let $ f $ be a continuous function $ \geq 0 $ on $ X $, with compact support $ K $; the relation $ 0 \leq g \leq f $ in $ \mathcal{K}(X; \mathbf{R}) $ implies that $ \|g\| \leq \|f\| $ and that the support of $ g $ is contained in $ K $. By hypothesis, there exists a number $ M_K \geq 0 $ such that $ |\mu(h)| \leq M_K \cdot \|h\| $ for every function $ h \in \mathcal{K}(X, K; \mathbf{R}) $; therefore $ |\mu(g)| \leq M_K \cdot \|g\| \leq M_K \cdot \|f\| $, which proves the theorem.

The space $ \mathcal{M}(X; \mathbf{R}) $ of real measures on $ X $ is thus identical with the space of relatively bounded linear forms on the Riesz space $ \mathcal{K}(X; \mathbf{R}) $; we recall that in $ \mathcal{M}(X; \mathbf{R}) $, the order relation $ \mu \leq \nu $ signifies that $ \nu - \mu $ is a positive measure, or also that $ \mu(f) \leq \nu(f) $ for every function $ f \in \mathcal{K}_+(X) $.

#### Theorem 3 {#int-iii-s1-thm-3 .statement}

*The space $ \mathcal{M}(X; \mathbf{R}) $ of real measures on a locally compact space $ X $ is fully lattice-ordered.*

This follows from Ch. II, §2, No. 2, Th. 1.

In conformity with the notations of Ch. II, §1, we define, for every *real* measure $ \mu $ on $ X $,

$$
\mu^+ = \sup(\mu, 0),\quad \mu^- = \sup(-\mu, 0),\quad |\mu| = \sup(\mu, -\mu);
$$

then $ \mu = \mu^+ - \mu^-,\ |\mu| = \mu^+ + \mu^- $ and $ \inf(\mu^+, \mu^-) = 0 $. Moreover, for every function $ f \in \mathcal{K}_+(\mathrm{X}) $,

$$
\int f\, d\mu^+ = \sup_{0 \leq g \leq f,\ g \in \mathcal{K}(\mathrm{X})} \int g\, d\mu
$$

and

$$
\int f\, d|\mu| = \sup_{|g| \leq f,\ g \in \mathcal{K}(\mathrm{X})} \int g\, d\mu,
$$

whence, in particular,

$$
\left| \int f\, d\mu \right| \leq \int |f|\, d|\mu|
$$

for every function $ f \in \mathcal{K}(\mathrm{X}; \mathbf{R}) $.

This inequality is also true if $ f \in \mathcal{K}(\mathrm{X}; \mathbf{C}) $; for, on multiplying $ f $ by a complex number of absolute value 1 (which does not change either side of the inequality), one can suppose that $ \int f\, d\mu \geq 0 $. Then

$$
\left| \int f\, d\mu \right| = \int f\, d\mu = \int (\Re f)\, d\mu \leq \int |\Re f|\, d|\mu| \leq \int |f|\, d|\mu|.
$$

### 6. Absolute value of a complex measure

Let $ \mu $ be a complex measure on a locally compact space $ \mathrm{X} $; for every function $ f \in \mathcal{K}_+(\mathrm{X}) $, the positive real number

$$
L(f) = \sup_{|g| \leq f,\ g \in \mathcal{K}(\mathrm{X}; \mathbf{C})} \left| \int g\, d\mu \right|
$$

is finite, because the relation $ |g| \leq f $ implies that $ \operatorname{Supp}(g) \subset \operatorname{Supp}(f) $ and $ \|g\| \leq \|f\| $, thus our assertion follows from formula (4) of No. 3. Let us show that $ L $ can be extended, in only one way, to a positive measure on $ \mathrm{X} $; in view of No. 5, Th. 1 and Ch. II, §2, No. 1, Prop. 3, it will suffice to show that if $ f_1,\ f_2 $ are two functions in $ \mathcal{K}_+(\mathrm{X}) $, then $ L(f_1 + f_2) = L(f_1) + L(f_2) $. Now, if $ |g_1| \leq f_1 $ and $ |g_2| \leq f_2 $, where $ g_1 $ and $ g_2 $ are functions in $ \mathcal{K}(\mathrm{X}; \mathbf{C}) $, we have $ |g_1 + \zeta g_2| \leq f_1 + f_2 $ for any complex number $ \zeta $ of absolute value 1, therefore

$$
|\mu(g_1 + \zeta g_2)| = |\mu(g_1) + \zeta \mu(g_2)| \leq L(f_1 + f_2).
$$

Moreover, we can suppose $ \zeta $ so chosen that
$$
|\mu(g_1) + \zeta \mu(g_2)| = |\mu(g_1)| + |\mu(g_2)|;
$$
since $ |\mu(g_i)| $ is arbitrarily close to $ L(f_i) $ ($ i = 1, 2 $), this proves that $ L(f_1) + L(f_2) \leq L(f_1 + f_2) $. On the other hand, consider a function $ g \in \mathcal{K}(X; \mathbf{C}) $ such that $ |g| \leq f_1 + f_2 $. The function $ g_i $ equal to $ g f_i/(f_1 + f_2) $ at the points where $ f_1(x) + f_2(x) \neq 0 $, and to 0 elsewhere ($ i = 1, 2 $), is continuous on X because $ f_i/(f_1 + f_2) $ ($ i = 1, 2 $) is continuous at every point where $ f_1(x) + f_2(x) \neq 0 $ and we have $ |g_i(x)| \leq |g(x)| $ for every $ x \in X $, which proves the continuity of $ g_i $ at the points where $ f_1(x) + f_2(x) = 0 $ ($ i = 1, 2 $), since at these points we have also $ g(x) = 0 $. It is clear that $ |g_i| \leq f_i $ ($ i = 1, 2 $) and $ g = g_1 + g_2 $, therefore
$$
|\mu(g)| \leq |\mu(g_1)| + |\mu(g_2)| \leq L(f_1) + L(f_2);
$$
since $ |\mu(g)| $ is arbitrarily close to $ L(f_1 + f_2) $, we have
$$
L(f_1 + f_2) \leq L(f_1) + L(f_2),
$$
which completes the proof of our assertion.

When $ \mu $ is a real measure, it follows from formula (9) that $ |\mu| \leq L $; on the other hand, by virtue of the last part of No. 5, if $ g \in \mathcal{K}(X; \mathbf{C}) $ and $ |g| \leq f \in \mathcal{K}_+(X) $ then $ |\int g \, d\mu| \leq \int |g| \cdot d|\mu| \leq \int f \, d|\mu| $, therefore by definition $ L \leq |\mu| $, in other words $ L = |\mu| $.

We denote again by $ |\mu| $ the positive measure $ L $ for any complex measure $ \mu $, and we say that $ |\mu| $ is the absolute value of $ \mu $. The definition of $ |\mu| $ can therefore be written
$$
|\mu|(f) = \sup_{|g| \leq f,\ g \in \mathcal{K}(X; \mathbf{C})} |\mu(g)|,
$$
consequently, for every function $ g \in \mathcal{K}(X; \mathbf{C}) $,
$$
\left| \int g \, d\mu \right| \leq \int |g| \, d|\mu|.
$$

It is clear that for every scalar $ \alpha \in \mathbf{C} $ and every measure $ \mu $ on $ X $,
$$
|\alpha \mu| = |\alpha| \cdot |\mu|.
$$

On the other hand, if $ \mu $ and $ \nu $ are two measures on $ X $, $ f $ is a function in $ \mathcal{K}_+(X) $, and $ g $ is a function in $ \mathcal{K}(X; \mathbf{C}) $ such that $ |g| \leq f $, then
$$
\left| \int g \, d(\mu + \nu) \right| = \left| \int g \, d\mu + \int g \, d\nu \right| \leq \int f \, d|\mu| + \int f \, d|\nu|,
$$

whence

$$(15)$$
$$|\mu + \nu| \leq |\mu| + |\nu|.$$

With the same notations, the relations $|g| \leq f$ and $|\overline{g}| \leq f$ are equivalent, therefore

$$(16)$$
$$|\overline{\mu}| = |\mu|.$$

It follows from (14), (15) and (16) that

$$(17)$$
$$|\mathcal{R}\mu| \leq |\mu|,\quad |\mathcal{I}\mu| \leq |\mu|,\quad |\mu| \leq |\mathcal{R}\mu| + |\mathcal{I}\mu|.$$

#### Proposition 8 {#int-iii-s1-prop-8 .statement}

*If $\mu$ is a measure on $X$ then, for every function $h \in \mathcal{C}(X; \mathbf{C})$,*

$$(18)$$
$$|h \cdot \mu| \leq |h| \cdot |\mu|.$$

For, if $f \in \mathcal{K}_+(X)$ and if $g \in \mathcal{K}(X; \mathbf{C})$ is such that $|g| \leq f$, then, by (13), $|\int gh d\mu| \leq \int |gh| d|\mu| \leq \int f|h| d|\mu|$, which proves (18).

### 7. Definition of a measure by extension

Let $X$ be a locally compact space; if $V$ is a *dense* linear subspace of $\mathcal{K}(X; \mathbf{C})$, it is clear that two measures $\mu_1, \mu_2$ on $X$ that coincide on $V$ are equal, and that every linear form on $V$ that is continuous for the topology induced by that of $\mathcal{K}(X; \mathbf{C})$ may be extended (in only one way) to a measure on $X$. For positive measures, a convenient criterion is the following:

#### Proposition 9 {#int-iii-s1-prop-9 .statement}

*Let $V$ be a linear subspace of $\mathcal{K}(X; \mathbf{R})$ having the following property:
(P) For every compact subset $K$ of $X$, there exists a function $f \in V$ such that $f \geq 0$ and such that $f(x) > 0$ for all $x \in K$.
Under these conditions, every positive linear form on $V$ for the ordering induced by that of $\mathcal{K}(X; \mathbf{R})$ (Ch. II, §2, No. 1, Def. 1) may be extended to a positive measure on $X$ (which is unique when $V$ is dense in $\mathcal{K}(X; \mathbf{R})$).
For every function $f \in \mathcal{K}(X; \mathbf{R})$, with support $K$, there exists a function $g \in V$ such that $f \leq g$; for, there exists a function $h \geq 0$ in $V$ such that $h(x) > 0$ for all $x \in K$; setting $\alpha = \inf_{x \in K} h(x)$, we thus have $\alpha > 0$ and the function $g = (\alpha^{-1} \|f\|)h$ meets the requirements. It then suffices to apply Th. 1 of No. 5 and Prop. 1 of TVS, II, §3, No. 1.*

### 8. Bounded measures

Let X be a locally compact space. Since the topology on $ \mathcal{K}(X; \mathbf{C}) $ induced by that of $ \mathcal{C}^b(X; \mathbf{C}) $ is coarser than the direct limit topology on $ \mathcal{K}(X; \mathbf{C}) $, a measure on X is not necessarily continuous for the topology of uniform convergence in X.

#### Definition 3 {#int-iii-s1-def-3 .statement}

*A measure on a locally compact space X is said to be bounded if it is continuous on $ \mathcal{K}(X; \mathbf{C}) $ for the topology of uniform convergence.*

It comes to the same to say that there exists a finite number $ M \geq 0 $ such that, for every function $ f \in \mathcal{K}(X; \mathbf{C}) $,

$$
|\mu(f)| \leq M \|f\|
$$

(where $ \|f\| $ is defined by formula (3) of No. 2).

To say that $ \mu $ is a bounded measure thus signifies that $ \mu $ belongs to the dual of the space $ \mathcal{K}(X; \mathbf{C}) $ normed by $ \|f\| $; we shall denote this dual by $ \mathcal{M}^1(X; \mathbf{C}) $ (or simply $ \mathcal{M}^1(X) $ when no confusion can result). We know that $ \mathcal{M}^1(X; \mathbf{C}) $ is equipped with a norm, $ \|\mu\| $ being the smallest of the numbers $ M \geq 0 $ for which the inequality (19) holds for every function $ f \in \mathcal{K}(X; \mathbf{C}) $, or again,

$$
\|\mu\| = \sup_{\|f\| \leq 1,\ f \in \mathcal{K}(X; \mathbf{C})} |\mu(f)| .
$$

Equipped with this norm, $ \mathcal{M}^1(X; \mathbf{C}) $ is known to be a Banach space (TVS, III, §3, No. 8, Cor. 2 of Prop. 12).

The definition of $ \|\mu\| $ by the formula (20) may be extended to every measure $ \mu $ on X and, by an abuse of language, $ \|\mu\| $ is again said to be the norm of $ \mu $; for $ \mu $ to be bounded, it is necessary and sufficient that $ \|\mu\| $ be finite.

If X is compact, then every measure on X is bounded.

#### Example {#int-iii-s1-n8-exa-1 .statement}

— 1) The measure $ \varepsilon_a $ defined by a unit mass at a point $ a \in X $ is bounded, and $ \|\varepsilon_a\| = 1 $.

2) The Lebesgue measure on $ \mathbf{R} $ is not bounded; indeed, for every integer $ n > 0 $ there exists a function $ f \in \mathcal{K}(\mathbf{R}; \mathbf{C}) $ with values in $[0, 1]$ and equal to 1 on the interval $[ -n, n ]$ (No. 2, Lemma 1); thus $ \|f\| = 1 $ and

$$
\int_{-\infty}^{+\infty} f(x)\, dx \geq \int_{-n}^{n} f(x)\, dx = 2n ,
$$

which proves that there does not exist any finite number M satisfying the relation (19).

3) On the real line $ \mathbf{R} $, the mapping

$$
f \mapsto \int_{-\infty}^{+\infty} \frac{f(x)\,dx}{1 + x^2}
$$

is a bounded measure since, for every function $ f \in \mathcal{H}(\mathbf{R}; \mathbf{C}) $,

$$
\left| \int_{-\infty}^{+\infty} \frac{f(x)\,dx}{1 + x^2} \right| \leq \|f\| \int_{-\infty}^{+\infty} \frac{dx}{1 + x^2} = \pi \cdot \|f\|.
$$

Since the relations $ \|f\| \leq 1 $ and $ \|\overline{f}\| \leq 1 $ are equivalent, it follows from (20) that

(21)
$$
\|\overline{\mu}\| = \|\mu\|
$$
for every measure $ \mu $ on $ X $.

#### Proposition 10 {#int-iii-s1-prop-10 .statement}

— *For every measure $ \mu $ on $ X $*,

(22)
$$
\|\mu\| = \sup_{0 \leq f \leq 1,\ f \in \mathcal{H}(X; \mathbf{R})} |\mu|(f).
$$

For, taking into account the formula (12) that defines the absolute value of a measure, the second member of (22) may be written

$$
\sup_{0 \leq f \leq 1,\ f \in \mathcal{H}(X; \mathbf{R})} \left( \sup_{|g| \leq f,\ g \in \mathcal{H}(X; \mathbf{C})} |\mu(g)| \right) = \sup_{\|g\| \leq 1,\ g \in \mathcal{H}(X; \mathbf{C})} |\mu(g)|.
$$

#### Corollary 1 {#int-iii-s1-prop-10-cor-1 .statement}

— *For every measure $ \mu $ on $ X $, the norms of $ \mu $ and $ |\mu| $ are equal; $ \mu $ is bounded if and only if $ |\mu| $ is bounded.*

#### Corollary 2 {#int-iii-s1-prop-10-cor-2 .statement}

— *For every measure $ \mu $ on a compact space $ X $,*

(23)
$$
\|\mu\| = |\mu|(1) = \int d|\mu|.
$$

This formula will be generalized in Ch. IV, §4, No. 7.

On a *compact* space $ X $, for every (complex) measure $ \mu $ on $ X $ the complex number $ \mu(1) $ is called the *total mass* of $ \mu $. When $ \mu $ is *positive*, its total mass is thus equal to its norm. When $ \mu $ is a positive measure on a *compact* space $ X $, of total mass equal to 1, one also says that its value $ \mu(f) $ for a continuous function $ f \in \mathcal{C}(X; \mathbf{C}) $ is the *mean* of $ f $ with respect to the measure $ \mu $.

#### Corollary 3 {#int-iii-s1-prop-10-cor-3 .statement}

— For every real measure $ \mu $ on a locally compact space $ X $,

$$
\| \mu \| = \sup_{\| f \| \leq 1,\ f \in \mathcal{K}(X; \mathbf{R})} | \mu(f) | .
$$

It suffices to make use of the formula (22) and the expression (9) for $ |\mu|(f) $ when $ \mu $ is a real measure and $ f \in \mathcal{K}_+(X) $.

The set of bounded real measures is therefore the dual of the normed space $ \mathcal{K}(X; \mathbf{R}) $; it is denoted $ \mathcal{M}^1(X, \mathbf{R}) $, or $ \mathcal{M}^1(X) $ if no confusion can result. The canonical injection $ \mathcal{M}^1(X, \mathbf{R}) \to \mathcal{M}^1(X; \mathbf{C}) $ is an isometry by virtue of (24).

#### Proposition 11 {#int-iii-s1-prop-11 .statement}

— If $ \mu $ and $ \nu $ are two positive measures on $ X $, then $ \| \mu + \nu \| = \| \mu \| + \| \nu \| $.

For, the functions $ f \in \mathcal{K}(X; \mathbf{R}) $ such that $ 0 \leq f \leq 1 $ form a directed set $ S $ for the relation $ \leq $. For a positive measure $ \mu $ on $ X $, it therefore follows from (22) and the monotone limit theorem that $ \| \mu \| = \lim_{f \in S} \mu(f) $; the conclusion of the proposition then follows at once.

#### Corollary 1 {#int-iii-s1-prop-11-cor-1 .statement}

— If $ \mu $ and $ \nu $ are two positive measures on $ X $ such that $ \mu \leq \nu $, then $ \| \mu \| \leq \| \nu \| $; in particular, if $ \nu $ is bounded then so is $ \mu $.
Indeed, $ \| \nu \| = \| \mu \| + \| \nu - \mu \| $.

#### Corollary 2 {#int-iii-s1-prop-11-cor-2 .statement}

— For every real measure $ \mu $ on $ X $,

$$
\| \mu \| = \| \mu^+ \| + \| \mu^- \|.
$$

For (Cor. 1 of Prop. 10), the norm of $ \mu $ is equal to that of $ |\mu| = \mu^+ + \mu^- $.

#### Proposition 12 {#int-iii-s1-prop-12 .statement}

— If $ \mu $ is a bounded measure on $ X $ and if $ g $ is a bounded continuous mapping of $ X $ into $ \mathbf{C} $, then the measure $ g \cdot \mu $ is bounded and $ \| g \cdot \mu \| \leq \| g \| \cdot \| \mu \| $.

For every function $ f \in \mathcal{K}(X; \mathbf{C}) $,

$$
|\mu(fg)| \leq \| \mu \| \cdot \| fg \| \leq \| \mu \| \cdot \| g \| \cdot \| f \|.
$$

### 9. Vague topology on the space of measures

Let $ X $ be a locally compact space. On the space $ \mathcal{M}(X; \mathbf{C}) $, one can consider the topology of pointwise convergence in $ \mathcal{K}(X; \mathbf{C}) $, which we shall call the vague topology on $ \mathcal{M}(X; \mathbf{C}) $.

Since $ \mathcal{K}(X; \mathbf{C}) = \mathcal{K}(X; \mathbf{R}) + i \mathcal{K}(X; \mathbf{R}) $, the vague topology on $ \mathcal{M}(X; \mathbf{C}) $ is defined by the *semi-norms* $ \sup_{1 \leq i \leq n} |\mu(f_i)| $, where $ (f_i)_{1 \leq i \leq n} $ is any finite sequence of functions in $ \mathcal{K}(X; \mathbf{R}) $ (or in $ \mathcal{K}_+(X) $). To say that a filter $ \mathfrak{F} $ on $ \mathcal{M}(X; \mathbf{C}) $ *converges vaguely* to a measure $ \mu_0 $ signifies that

$$
\mu_0(f) = \lim_{\mu, \mathfrak{F}} \mu(f)
$$

for every function $ f \in \mathcal{K}(X; \mathbf{R}) $. For every function $ f \in \mathcal{K}(X; \mathbf{C}) $, the mapping $ \mu \mapsto \mu(f) $ is a *vaguely continuous* linear form on the space $ \mathcal{M}(X; \mathbf{C}) $.

#### Proposition 13 {#int-iii-s1-prop-13 .statement}

*Let X be a locally compact space and, for every $ x \in X $, let $ \varepsilon_x $ be the Dirac measure at the point x. The mapping $ x \mapsto \varepsilon_x $ is a homeomorphism of X onto a subspace of the space $ \mathcal{M}(X; \mathbf{C}) $ of measures on X, equipped with the vague topology. Moreover, if $ X' $ denotes the compact space obtained by adjoining to X a point at infinity $ \omega $, then $ \varepsilon_x $ tends to 0 as x tends to $ \omega $.*

For every function $ f \in \mathcal{K}(X; \mathbf{C}) $, $ \langle f, \varepsilon_x \rangle = f(x) $; since $ f $ is continuous, this proves that the mapping $ x \mapsto \varepsilon_x $ is continuous. If $ x, y $ are two distinct points of X, there exists a function $ f \in \mathcal{K}(X; \mathbf{C}) $ such that $ f(x) = 1, f(y) = 0 $ (No. 2, Lemma 1), which proves that $ \varepsilon_x \neq \varepsilon_y $; the mapping $ x \mapsto \varepsilon_x $ is therefore injective. Moreover, for every function $ f \in \mathcal{K}(X; \mathbf{C}) $, $ \langle f, \varepsilon_x \rangle $ tends to 0 by definition as $ x $ tends to $ \omega $, therefore $ x \mapsto \varepsilon_x $ may be extended by continuity to $ X' = X \cup \{ \omega \} $ by assigning to it the value 0 at the point $ \omega $. This extended mapping is also injective, since $ \varepsilon_x \neq 0 $ for all $ x \in X $. It is therefore a homeomorphism of the compact space $ X' $ onto a subspace of $ \mathcal{M}(X; \mathbf{C}) $, since $ \mathcal{M}(X; \mathbf{C}) $ is Hausdorff for the vague topology (GT, I, §9, No. 4, Cor. 2 of Th. 2).

#### Proposition 14 {#int-iii-s1-prop-14 .statement}

*In the space $ \mathcal{M}(X; \mathbf{C}) $ of measures on a locally compact space X, the cone $ \mathcal{M}_+(X) $ of positive measures is complete for the uniform structure deduced from the vague topology* (hence is *vaguely closed* in $ \mathcal{M}(X; \mathbf{C}) $).

For, consider a Cauchy filter $ \Phi $ for the vague uniform structure on $ \mathcal{M}_+(X) $; by definition, $ \mu_0(f) = \lim_{\mu, \Phi} \mu(f) $ exists for every function $ f \in \mathcal{K}(X; \mathbf{C}) $ and, by the principle of extension of inequalities, $ \mu_0(f) \geq 0 $ for every function $ f \in \mathcal{K}_+(X) $; it follows that $ \mu_0 $ is a positive measure on X (No. 5, Th. 1).

It should be noted that the space $ \mathcal{M}(X; \mathbf{C}) $ (or $ \mathcal{M}(X; \mathbf{R}) $) itself *is not necessarily complete* for the vague uniform structure (TVS, II, §6, No. 7).

#### Corollary {#int-iii-s1-n9-cor-1 .statement}

*If A and B are two vaguely closed subsets of $ \mathcal{M}_+(X) $, then $ A + B $ is vaguely closed in $ \mathcal{M}_+(X) $ (hence also in $ \mathcal{M}(X; \mathbf{C}) $).*

This is in fact a general property of weakly complete, proper cones in locally convex spaces (TVS, II, §6, No. 8, Cor. 2 of Prop. 11).

#### Proposition 15 {#int-iii-s1-prop-15 .statement}

— Let $ H $ be a subset of $ \mathcal{M}(X; \mathbf{C}) $. The following properties are equivalent:

a) $ H $ is vaguely bounded.
b) $ H $ is vaguely relatively compact.
c) $ H $ is equicontinuous.
d) For every compact subset $ K $ of $ X $, there exists a number $ M_K \geq 0 $ such that $ |\mu(f)| \leq M_K \|f\| $ for every measure $ \mu \in H $ and every function $ f \in \mathcal{K}(X, K; \mathbf{C}) $.

Since $ \mathcal{K}(X; \mathbf{C}) $ is a barreled space (No. 1, Prop. 2), the equivalence of properties a), b) and c) follows from TVS, III, §4, No. 1, Scholium.

It is clear that d) implies a). Finally, if $ H $ is equicontinuous then the set of restrictions of the measures $ \mu \in H $ to $ \mathcal{K}(X, K; \mathbf{C}) $ is also equicontinuous, whence the condition d), since $ \mathcal{K}(X, K; \mathbf{C}) $ is a normed space.

* We shall see in Ch. IV, §4, No. 6 that the conditions of Proposition 15 are also equivalent to the condition that, for every compact subset $ K $ of $ X $, there exists a constant $ M_K $ such that $ |\mu|(K) \leq M_K $ for every measure $ \mu \in H $.*

#### Corollary 1 {#int-iii-s1-prop-15-cor-1 .statement}

— Let $ \nu $ be a positive measure on $ X $; the set of measures $ \mu $ such that $ |\mu| \leq \nu $ is vaguely compact.

#### Corollary 2 {#int-iii-s1-prop-15-cor-2 .statement}

— The set of measures $ \mu $ such that $ \|\mu\| \leq a $ ($ a $ any finite number $ > 0 $) is vaguely compact.

#### Corollary 3 {#int-iii-s1-prop-15-cor-3 .statement}

— If $ X $ is compact, the set of positive measures $ \mu $ on $ X $ such that $ \|\mu\| = 1 $ is vaguely compact.

For, it is the intersection of the vaguely compact set (Cor. 2) of measures such that $ \|\mu\| \leq 1 $ and the vaguely closed sets defined respectively by the relations $ \mu \geq 0 $ and $ \mu(1) = 1 $ (No. 8, Cor. 2 of Prop. 10).

#### Corollary 4 {#int-iii-s1-prop-15-cor-4 .statement}

— In the space $ \mathcal{M}(X; \mathbf{C}) $, the mapping $ \mu \mapsto \|\mu\| $ is lower semi-continuous for the vague topology.

This is an immediate consequence of Corollary 2.

It should be noted that the mapping $ \mu \mapsto |\mu| $ of $ \mathcal{M}(X; \mathbf{C}) $ into itself is not necessarily continuous for the vague topology (Exer. 9).

#### Proposition 16 {#int-iii-s1-prop-16 .statement}

— Let $ K $ be a compact subset of $ X $, $ H $ a vaguely bounded subset of $ \mathcal{M}(X; \mathbf{C}) $; then, the bilinear form $ (f, \mu) \mapsto \langle f, \mu \rangle $ is continuous on $ \mathcal{K}(X, K; \mathbf{C}) \times H $ when $ \mathcal{K}(X, K; \mathbf{C}) $ is equipped with the topology of uniform convergence and $ H $ with the vague topology.

For, there exists a number $ M \geqslant 0 $ such that
$$
|\mu(f)| \leqslant M \|f\|
$$
for every function $ f \in \mathcal{K}(X, K; \mathbf{C}) $ and every measure $ \mu \in H $ (Prop. 15). If $ \mu_0 $ and $ \mu $ are two measures belonging to $ H $, $ f_0 $ and $ f $ two functions in $ \mathcal{K}(X, K; \mathbf{C}) $, then
$$
|\mu(f) - \mu_0(f_0)| = |\mu(f - f_0) + \mu(f_0) - \mu_0(f_0)| \\
\leqslant M \|f - f_0\| + |\mu(f_0) - \mu_0(f_0)|,
$$
and the last quantity is arbitrarily small when $ \|f - f_0\| $ and $ |\mu(f_0) - \mu_0(f_0)| $ are, which proves the proposition.

### 10. Compact convergence in $ \mathcal{M}(X; \mathbf{C}) $

Recall that the topology of *compact convergence* on $ \mathcal{M}(X; \mathbf{C}) $ is the topology of uniform convergence in the compact subsets of $ \mathcal{K}(X; \mathbf{C}) $. We shall call *topology of strictly compact convergence* on $ \mathcal{M}(X; \mathbf{C}) $ the topology of uniform convergence in the strictly compact subsets (No. 1) of $ \mathcal{K}(X; \mathbf{C}) $.

#### Proposition 17 {#int-iii-s1-prop-17 .statement}

*On the space $ \mathcal{M}(X; \mathbf{C}) $, consider the following topologies:*
$ \mathcal{T}_1 $: *the topology of pointwise convergence in a total subset T of $ \mathcal{K}(X; \mathbf{C}) $;*
$ \mathcal{T}_2 $: *the vague topology;*
$ \mathcal{T}_3 $: *the topology of strictly compact convergence;*
$ \mathcal{T}_4 $: *the topology of compact convergence.*
*Each of these topologies is coarser than the next. Moreover:*
*(i)* *The bounded sets are the same for $ \mathcal{T}_2 $, $ \mathcal{T}_3 $ and $ \mathcal{T}_4 $.*
*(ii)* *If H is a vaguely bounded subset of $ \mathcal{M}(X; \mathbf{C}) $, the topologies induced on H by the topologies $ \mathcal{T}_1 $, $ \mathcal{T}_2 $, $ \mathcal{T}_3 $, $ \mathcal{T}_4 $ are identical.*

A vaguely bounded subset $ H $ of $ \mathcal{M}(X; \mathbf{C}) $ is equicontinuous (No. 9, Prop. 15), thus the first assertion follows from TVS, III, §3, No. 7, Prop. 9, and the second from GT, X, §2, No. 4, Th. 1.

Recall that when $ X $ is *paracompact*, the topology of strictly compact convergence coincides with the topology of compact convergence (No. 1, Prop. 2).

#### Proposition 18 {#int-iii-s1-prop-18 .statement}

*On the cone $ \mathcal{M}_+(X) $, the topologies induced by the following topologies coincide:*
$ \mathcal{T}_1 $: *the topology of pointwise convergence in a linear subspace V of $ \mathcal{K}(X; \mathbf{C}) $ that is dense in $ \mathcal{K}(X; \mathbf{C}) $ and satisfies the property (P) (No. 7, Prop. 9);*

\textit{\mathcal{T}_2: the vague topology;}

\textit{\mathcal{T}_3: the topology of strictly compact convergence.}

Since every filter is the intersection of the ultrafilters finer than it (GT, I, §6, No. 4, Prop. 7), it suffices to show that if $ \mathfrak{U} $ is an ultrafilter on $ \mathcal{M}_+(X) $ that converges to a measure $ \mu_0 $ for the topology $ \mathcal{T}_1 $, then it also converges to $ \mu_0 $ for $ \mathcal{T}_3 $. Let $ K $ be a compact subset of $ X $; by hypothesis, there exists a function $ h \in V $ that is $ \geqslant 0 $ on $ X $ and takes values $ > 0 $ on $ K $; it follows that every function $ f \in \mathcal{K}(X, K; \mathbf{C}) $ may be written $ f = gh $ with $ g \in \mathcal{K}(X, K; \mathbf{C}) $, and if $ c = \inf_{x \in K} h(x) > 0 $ then $ \|g\| \leqslant c^{-1}\|f\| $. By hypothesis, there exists a set $ H_0 \in \mathfrak{U} $ such that, for every measure $ \mu \in H_0 $,

$$
0 \leqslant \mu(h) \leqslant \mu_0(h) + 1 = b.
$$

Consequently, for every function $ f \in \mathcal{K}(X; \mathbf{C}) $,

$$
|\langle f, h \cdot \mu \rangle| = |\langle hf, \mu \rangle| \leqslant \|f\| \cdot \mu(h) \leqslant b \|f\|
$$

for every measure $ \mu \in H_0 $; this proves that the set $ H $ of measures $ h \cdot \mu $, where $ \mu $ runs over $ H_0 $, is \emph{vaguely bounded}. If $ \mathfrak{U}_0 $ is the ultrafilter induced by $ \mathfrak{U} $ on $ H_0 $, the image of $ \mathfrak{U}_0 $ under the mapping $ \mu \mapsto h \cdot \mu $ is the base of an ultrafilter $ \mathfrak{F} $ on $ H $, and since $ H $ is relatively compact for the topology of strictly compact convergence (Prop. 17 and No. 9, Prop. 15), $ \mathfrak{F} $ is convergent to a measure $ \nu_0 $ for this topology. In other words, for any $ \varepsilon > 0 $ and any compact subset $ L $ of $ \mathcal{K}(X, K; \mathbf{C}) $, there exists a subset $ N $ of $ H_0 $ belonging to $ \mathfrak{U} $ such that, for every function $ g \in L $ and every pair of measures $ \mu, \mu' $ belonging to $ N $, one has $ |\langle g, h \cdot \mu \rangle - \langle g, h \cdot \mu' \rangle| \leqslant \varepsilon $, that is,

$$
|\langle gh, \mu \rangle - \langle gh, \mu' \rangle| \leqslant \varepsilon.
$$

Now, we saw above that the mapping $ g \mapsto gh $ is an \emph{automorphism} of the Banach space $ \mathcal{K}(X, K; \mathbf{C}) $. We have thus shown that $ \mathfrak{U} $ is a \emph{Cauchy filter} on $ \mathcal{M}_+(X) $ for the topology of strictly compact convergence. \emph{A fortiori}, it is a Cauchy filter for vague convergence, and Prop. 14 of No. 9 shows that it is vaguely convergent to a measure $ \mu_1 $; moreover, since $ V $ is dense in $ \mathcal{K}(X; \mathbf{C}) $, the hypothesis implies that $ \mu_1 = \mu_0 $; finally, since $ \mathfrak{U} $ is a Cauchy filter for the topology of strictly compact convergence, it also converges to $ \mu_0 $ for this topology (GT, X, §1, No. 5, Prop. 5).

Q.E.D.

#### Corollary {#int-iii-s1-n10-cor-1 .statement}

— *If X is paracompact then the topologies induced on $ \mathcal{M}_+(X) $ by the vague topology and the topology of compact convergence coincide.*

However, the topologies induced on $ \mathcal{M}_+(X) $ by the topology of compact convergence and the topology of strictly compact convergence may be different when X is not paracompact (Exer. 3).

### Exercises {#int-iii-s1-exercises}

See the [exercises for § 1](exercises/s1/).
