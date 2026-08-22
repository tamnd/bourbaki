---
book: evt
book_title: Topological Vector Spaces
chapter: I
chapter_title: TOPOLOGICAL VECTOR SPACES OVER A VALUED DIVISION RING
section: 1
section_title: Topological vector spaces
lang: en
source: evt-i-v
pdf_pages: 0009-0019, 0030-0033
extraction: ocr
subsections:
    - "no": 1
      title: Definition of a topological vector space
      page: 0
      pdf_page: 9
    - "no": 2
      title: Normed spaces on a valued division ring
      page: 3
      pdf_page: 11
    - "no": 3
      title: Vector subspaces and quotient spaces of a topological vector space; products of topological vector spaces; topological direct sums of subspaces
      page: 4
      pdf_page: 12
    - "no": 4
      title: Uniform structure and completion of a topological vector space
      page: 5
      pdf_page: 13
    - "no": 5
      title: Neighbourhoods of the origin in a topological vector space over a valued division ring
      page: 6
      pdf_page: 14
    - "no": 6
      title: Criteria of continuity and equicontinuity
      page: 8
      pdf_page: 16
    - "no": 7
      title: Initial topologies of vector spaces
      page: 9
      pdf_page: 17
statements: 23
exercises: 14
content_sha256: 1fa35c643923023134a74cbf1e3b29360774f343b752ec68611729b926b6618a
---

## § 1. TOPOLOGICAL VECTOR SPACES

### 1. Definition of a topological vector space

#### Definition 1 {#evt-i-s1-def-1 .statement}

— *Given a topological division ring* $ \mathbf{K} $ (GT, III, § 6.7) *and a set* $ E $ *such that* $ E $ *has*
$ 1^\circ $ *the structure of a left vector space on* $ \mathbf{K} $;
$ 2^\circ $ *a topology compatible with the structure of the additive group of* $ E $ (GT, III, § 1.1) *and satisfying in addition the following axiom :*
*(EVT)* *the mapping* $ (\lambda, x) \mapsto \lambda x $ *of* $ \mathbf{K} \times E $ *in* $ E $ *is continuous,* *then* $ E $ *is called a left topological vector space over* (or on) $ \mathbf{K} $.

It is equivalent to saying that $ E $ is a *topological left* $ \mathbf{K}\text{-module} $ (GT, III, § 6.6).
A left vector space structure relative to $ \mathbf{K} $ and a given topology on a set $ E $, are said to be *compatible* if the topology and the additive group structure of $ E $ are compatible and if, in addition, the axiom (EVT) is valid. This is the same as saying that the two mappings $ (x, y) \mapsto x + y $ and $ (\lambda, x) \mapsto \lambda x $ of $ E \times E $ and of $ \mathbf{K} \times E $, respectively, in $ E $ are continuous, for then the mapping $ x \mapsto -x = (-1)x $, is continuous and the topology of $ E $ is compatible with its additive group structure.

If $ E $ is a left topological vector space over $ \mathbf{K} $, we say that $ E $ provided only with its vector space structure, *underlies* the topological vector space $ E $.

#### Example {#evt-i-s1-n1-exa-1 .statement}

— 1) If $ E $ is a left vector space over a *discrete* topological division ring $ \mathbf{K} $, the *discrete* topology on $ E $ is compatible with the vector space structure of $ E $ (this is not so if $ \mathbf{K} $ is non-discrete and $ E $ is not the single point 0).
2) Let $ A $ be a topological ring (GT, III, § 6.3) and let $ \mathbf{K} $ be a subring of $ A $ that is also a division ring and such that the topology induced on $ \mathbf{K} $ by that of $ A $ is compatible with the division ring structure of $ \mathbf{K} $; then the topology of $ A $ is compatible with its left vector space structure on $ \mathbf{K} $.
3) Let $ \mathbf{K} $ be any topological division ring and $ I $ an arbitrary set. On the product vector space $ K_s^I(A, II, § 1.5) $, the product topology is compatible with the vector space structure (GT, III, § 6.4). Or we can say that the space $ K_s^I $ of mappings of $ I $ in $ \mathbf{K} $ with *pointwise* or *simple convergence* topology is a topological vector space on $ \mathbf{K} $ (TG, X, p. 4).
4) Let $ X $ be a topological space; on the set $ E = \mathcal{C}(X; \mathbf{R}) $ of finite real-valued *continuous* functions defined over $ X $, the *compact convergence* topology (GT, X, § 1.3) is compatible with the vector space structure of E on $ \mathbf{R} $. For, let $ u_0 $ be a point of E, let H be a compact subset of X and $ \varepsilon $ be an arbitrary strictly positive number. The real-valued function $ u_0 $ is bounded in H ; let $ a = \sup_{t \in H} |u_0(t)| $; if $ u $ is any point of E then for all $ t \in H $

$$
|\lambda u(t) - \lambda_0 u_0(t)| \leq |\lambda| \cdot |u(t) - u_0(t)| + a |\lambda - \lambda_0|.
$$

Hence, if $ |\lambda - \lambda_0| \leq \varepsilon $ and $ |u(t) - u_0(t)| \leq \varepsilon $ for all $ t \in H $, then for $ t \in H $,
$ |\lambda u(t) - \lambda_0 u_0(t)| \leq \varepsilon (\varepsilon + |\lambda_0| + a) $, which shows that the axiom (EVT) is satisfied ; similarly it can be verified that the compact convergence topology is compatible with the additive group structure of E.

On the other hand, if X is not compact, the *uniform convergence* topology (in X) is not necessarily compatible with the vector space structure of E ; for example if $ X = \mathbf{R} $ and if $ u_0 $ is an unbounded continuous function in $ \mathbf{R} $, then the mapping $ \lambda \mapsto \lambda u_0 $ of $ \mathbf{R} $ in E is not continuous in the uniform convergence topology on E.

5) Let E be a vector space of finite dimension $ n $ over a topological division ring K ; there exists an isomorphism $ u : K_s^n \to E $ of vector K-spaces and moreover, if $ v $ is a second isomorphism of $ K_s^n $ on E, then we can write $ v = u \circ f $, where $ f $ is an automorphism of the vector K-space $ K_s^n $. Consider, on $ K_s^n $, the *product* topology that is compatible with its vector space structure (*Example 3*) ; since every linear mapping of $ K_s^n $ in itself is continuous for this topology, every automorphism of the vector space $ K_s^n $ is *bicontinuous*. Hence, if we *transfer* the product topology of $ K_s^n $ to E, by means of any isomorphism whatever of $ K_s^n $ on E, the topology obtained on E is *independent* of the particular isomorphism used ; we call it the *canonical topology* on E ; we shall characterize it differently (I, § 1.3) when K is a non-discrete complete division ring with a valuation. Every linear mapping of E in a topological vector space over K is *continuous* for the canonical topology on E.

In the same way as in def. 1, a *right* topological vector space over K, a topological division ring, can be defined ; but every right vector space on K can be considered as a left vector space on the division ring $ K^0 $ opposite to K (A, II, § 1.1) and the topology of K is compatible with the structure of the division ring $ K^0 $. For this reason we usually consider only left topological vector spaces ; when we speak of « topological vector space » without qualification, it is to be understood that we refer to a left vector space.

If K' is a sub-division ring of K, and E a topological vector space over K, then it is clear that the topology of E is still compatible with the vector space structure of E relative to K', obtained by restricting the field of scalars to K' ; we say that the topological vector space on K', obtained by this procedure, *underlies* the topological vector space E on K.

In order that a topological vector space E be *Hausdorff*, it is necessary and sufficient that for all $ x \neq 0 $ of E, there exists a neighbourhood of 0 not containing $ x $ (GT, III, § 1.2).

Consider a topology, on a vector space E over a topological division ring K, that is compatible with the additive group structure of E. Because of the identity

$$
\lambda x - \lambda_0 x_0 = (\lambda - \lambda_0) x_0 + \lambda_0 (x - x_0) + (\lambda - \lambda_0) (x - x_0)
$$

axiom (EVT) is equivalent to the following system of three axioms.

*(EVT$_1'$)* *For all* $ x_0 \in E $, *the mapping* $ \lambda \mapsto \lambda x_0 $ *is continuous at* $ \lambda = 0 $.

*(EVT$_2'$)* *For all* $ \lambda_0 \in K $, *the mapping* $ x \mapsto \lambda_0 x $ *is continuous at* $ x = 0 $.

*(EVT$_3'$)* *The mapping* $ (\lambda, x) \mapsto \lambda x $ *is continuous at* $ (0, 0) $.

In particular:

#### Proposition 1 {#evt-i-s1-prop-1 .statement}

— For all $ \alpha \in K $ and every point $ b \in E $, the mapping $ x \mapsto \alpha x + b $ of $ E $ in itself is continuous. Further, if $ \alpha \neq 0 $, this mapping is a homeomorphism of $ E $ on itself.

The second part of the proposition is a result of the fact that if $ \alpha \neq 0 $, then $ x \mapsto \alpha^{-1}x - \alpha^{-1}b $ is the inverse mapping of $ x \mapsto \alpha x + b $.

#### Corollary {#evt-i-s1-n1-cor-1 .statement}

— If $ A $ is an open (resp. closed) set in $ E $, then $ \alpha A $ is open (resp. closed) in $ E $ for every $ \alpha \neq 0 $ in $ K $.

Let $ E $ and $ F $ be two topological vector spaces on the same topological division ring $ K $. A bijection $ f $ of $ E $ on $ F $ is an isomorphism of the topological vector space $ E $ on the topological vector space $ F $ if and only if $ f $ is linear and bicontinuous. In particular, if $ \gamma \neq 0 $ belongs to the centre of $ K $, the homothety $ x \mapsto \gamma x $ is an automorphism of the topological vector space structure of $ E $.

### 2. Normed spaces on a valued division ring

Recall (GT, IX, § 3.2) that an absolute value on a division ring $ K $ is a mapping $ \xi \mapsto |\xi| $ of $ K $ in $ \mathbf{R}_+ $, such that $ |\xi| = 0 $ if, and only if, $ \xi = 0 $, and that $ |\xi \eta| = |\xi| \cdot |\eta| $, and $ |\xi + \eta| \leq |\xi| + |\eta| $; an absolute value defines a distance $ |\xi - \eta| $ on $ K $, and hence a Hausdorff topology compatible with the division ring structure of $ K $. If $ |\xi| = 1 $ for all $ \xi \neq 0 $, the absolute value is called improper, and the topology that it defines on $ K $ is the discrete topology; if, on the other hand, there exists $ \alpha \neq 0 $ in $ K $ such that $ |\alpha| \neq 1 $, then there exists $ \beta \neq 0 $ in $ K $ such that $ |\beta| < 1 $ (it is sufficient to take $ \beta = \alpha $ or $ \beta = \alpha^{-1} $), and the sequence $ (\beta^n)_{n \geq 1} $ converges to 0, thus the topology of $ K $ is not discrete.

We recall on the other hand (GT, IX, § 3.3) that if $ E $ is a vector space on a non-discrete valued division ring $ K $ then a norm on $ E $ is a mapping $ x \mapsto \|x\| $ of $ E $ in $ \mathbf{R}_+ $, such that $ \|x\| = 0 $ if, and only if, $ x = 0 $, and such that $ \|\lambda x\| = |\lambda| \cdot \|x\| $ for every scalar $ \lambda \in K $, and $ \|x + y\| \leq \|x\| + \|y\| $. A distance $ \|x - y\| $, is defined on $ E $ by the norm, and hence a topology that is compatible with the vector space structure of $ E $ (loc. cit.). Unless the contrary is expressly stated, a normed space is considered in terms of the structure of the topological vector space defined by its norm. The normed spaces are among the most important of topological vector spaces.

It is known (GT, IX, § 3.3) that two distinct norms on $ E $ can define the same topology on $ E $; for this it is necessary and sufficient that the two norms be equivalent (loc. cit.). The structure of normed spaces is thus richer than the structure of topological vector spaces; if $ E $ and $ F $ are two normed spaces one must be careful to distinguish between the idea of isomorphism of the normed space structure of $ E $ with that of $ F $, and the idea of isomorphism of the topological vector space structure of $ E $ with that of $ F $.

#### Example {#evt-i-s1-n2-exa-1 .statement}

— Let I be an arbitrary set of indices; it is known (GT, X, § 3.2) that a norm $ \|x\| $ can be defined, on the set of bounded mappings $ x = (\xi_i) $ of I in K, $ \mathcal{B}(I; K) $ (also written $ \mathcal{B}_K(I) $ or $ \ell_K^\infty(I) $), by $ \|x\| = \sup_{i \in I} |\xi_i| $. When I is a topological space, the set of bounded, continuous mappings of I in K is a closed subspace of the space $ \mathcal{B}(I; K) $ (GT, X, § 3.1, cor. 2). Another subspace of $ \mathcal{B}(I; K) $ is the set $ \ell_K^1(I) $ of absolutely summable families $ x = (\xi_i) $ (GT, X, § 3.6); we can define on this subspace another norm $ \|x\|_1 = \sum_{i \in I} |\xi_i| $, that in general is not equivalent to the norm $ \|x\| = \sup_{i \in I} |\xi_i| $ (I, p. 23, exerc. 6); when considering $ \ell_K^1(I) $ as a normed space, without specifying its norm, it is always the norm $ \|x\| $, that is meant. We write $ \mathcal{B}(I) $ and $ \ell^1(I) $ in place of $ \mathcal{B}(I; \mathbf{R}) $ and $ \ell_R^1(I) $.

### 3. Vector subspaces and quotient spaces of a topological vector space; products of topological vector spaces; topological direct sums of subspaces

Everything that has been said for topological modules (GT, III, § 6.6) applies in particular to topological vector spaces. If M is a vector subspace of a topological vector space E, the topology induced on M by that of E is compatible with the vector space structure of M, and the closure $ \overline{M} $ of M in E is a vector subspace of E. The quotient topology of that of E by M is compatible with the vector space structure of E/M.

If E is a topological vector space, the closure N of $ \{0\} $ in E (intersection of neighbourhoods of 0) is a closed vector subspace of E; the quotient vector subspace E/N, which is necessarily Hausdorff whether E is or not, is called the Hausdorff vector space associated with E.

Let $ (E_i)_{i \in I} $ be a family of topological vector spaces over the same topological division ring K, and let E be the product vector space of the $ E_i $. The product topology of the topologies of the $ E_i $ is compatible with the vector space structure of E. In the product space E, the subspace F, the direct sum of the $ E_i $ is everywhere dense (GT, III, § 2.9, prop. 25).

For certain types of topological vector spaces on the field $ \mathbf{R} $ or the field $ \mathbf{C} $ we define (in II, p. 29) a topology on the direct sum of a family $ (E_i) $ of topological vector spaces that is, in general, distinct from the topology induced by the product topology of the $ E_i $.

Everything that has been said on the finite direct sums of stable subgroups of topological groups with operators (GT, III, § 6.2) applies to topological vector spaces, replacing « stable subgroup » throughout by « vector subspace ».

#### Remark {#evt-i-s1-n3-rem-1 .statement}

— Given a closed vector subspace M of a Hausdorff topological vector space E, it is not necessarily the case that there exists an (algebraic) complementary vector subspace to M that is closed in E (even if E is a normed space; cf. IV, p. 55, exerc. 16 (c)); a fortiori there does not necessarily exist a topological complement of M in E (cf. I, p. 26, exerc. 8). However we shall see in § 2 that when K is a non-discrete valued division ring, then every closed subspace M of E, with finite codimension, does have a topological complement in E (I, p. 14, prop. 3).

### 4. Uniform structure and completion of a topological vector space

Since the topology of the topological vector space E is compatible with the additive group structure on E, it defines a uniform structure on E (GT, III, § 3); when we speak of the uniform structure of a topological vector space we always mean this structure unless the contrary is expressly stated. Every continuous linear mapping of a topological vector space E in a topological vector space F is uniformly continuous (GT, III, § 3.1, prop. 3); every mapping of E in itself of the form $ x \mapsto \alpha x + b $ is uniformly continuous. An equicontinuous set of linear mappings of E in F is uniformly equicontinuous (GT, X, § 2.2, prop. 5).

#### Remark {#evt-i-s1-n4-rem-1 .statement}

— 1) If B is a precompact set of K, then for every neighbourhood V of 0 in E, there is a neighbourhood U of 0 in E such that BU $ \subset $ V. For, if W is a neighbourhood of 0 in E such that W + W $ \subset $ V; then from (EVT$_{\text{III}}$) there is a neighbourhood T$_0$ of 0 in K and a neighbourhood U$_0$ of 0 in E such that T$_0$U$_0$ $ \subset $ W. As B is precompact, there are finitely many points $ \lambda_i \in B $ ($ 1 \leq i \leq n $) such that the $ \lambda_i + T_0 $ cover B; from (EVT$_{\text{II}}$) it follows that there is a neighbourhood U $ \subset $ U$_0$ of 0 in E, such that $ \lambda_i U \subset W $ for all $ i $; clearly U has the required properties. In a similar manner (using (EVT$_{\text{I}}$) instead of (EVT$_{\text{II}}$)) it can be shown that if H is a precompact set of E, then for every neighbourhood V of 0 in E, there exists a neighbourhood T of 0 in K such that TH $ \subset $ V.

2) From 1) it follows that, if B is a precompact set of K and H is a precompact set of E, then the mapping $ (\lambda, x) \mapsto \lambda x $ restricted to B $ \times $ H is uniformly continuous. For, if V is a neighbourhood of 0 in E then there are neighbourhoods T of 0 in K, and U of 0 in E such that TH + BU $ \subset $ V. Since we can write $ \lambda x - \lambda' x' = (\lambda - \lambda') x + \lambda'(x - x') $, we see that for $ \lambda, \lambda' $ in B, x, x' in H, $ \lambda - \lambda' \in T $ and $ x - x' \in U $, we have $ \lambda x - \lambda' x' \in V $, which proves our assertion.

A topological vector space is called complete if, considering its uniform structure, it is a complete uniform space.

Definition 2. — *A complete normed space on a non-discrete valued division ring is called a Banach space.*

#### Example {#evt-i-s1-n4-exa-1 .statement}

— If K is a non-discrete valued division ring then the space $ \mathscr{B}(I ; K) $ (I, p. 4, Example) is complete (GT, X, § 3.1, cor. 1). This is also true for the space $ \ell_K^1(I) $ (I, p. 4, Example) with the norm $ \|x\|_1 = \sum_{i \in I} |\xi_i| $: for, if $ x_n $ is a Cauchy sequence in this space and $ x_n = (\xi_{m_i})_{i \in I} $, then for all $ i \in I $

$$
|\xi_{m_i} - \xi_{n_i}| \leq \|x_m - x_n\|_1;
$$

thus, for each $ i \in I $, the sequence $ (\xi_{m_i})_{n \geq 1} $ converges to a limit $ \xi_i $ in K. Further, for each finite subset J of I

$$
\sum_{i \in J} |\xi_{m_i} - \xi_{n_i}| \leq \|x_m - x_n\|_1;
$$

and it follows immediately that there exists a constant $ a > 0 $, independent of J, m, n such that $ \sum_{i \in J} |\xi_{m_i} - \xi_{n_i}| \leq a $. Letting m tend to $ + \infty $, we deduce $ \sum_{i \in J} |\xi_i - \xi_{m_i}| \leq \varepsilon $ from which $ \sum_{i \in I} |\xi_i| \leq a + \|x_n\|_1 $, which shows that $ z = (\xi_i)_{i \in I} $ belongs to $ \ell_K^1(I) $; further, for all $ \varepsilon > 0 $, there exists $ n_0 $ such that for $ n \geq n_0 $ and for every finite set J of I, we have $ \sum_{i \in J} |\xi_i - \xi_{m_i}| \leq \varepsilon $; passing to the limit with respect to the directed set of finite subsets of I, we see that $ \|z - x_n\|_1 \leq \varepsilon $ for $ n \geq n_0 $, which shows that $ z $ is the limit of the sequence $ (x_n) $ in the normed space $ \ell_K^1(I) $.

Let $ K $ be a Hausdorff topological division ring, $ E $ a topological vector space on $ K $ and suppose that the completed ring $ \hat{K} $ is a *division ring* (this is so when $ K $ is a valued division ring, GT, IX, § 3.3) then the Hausdorff completion $ \hat{E} $ of $ E $ carries the structure of a *complete topological vector space* on $ \hat{K} $ (GT, III, § 6.5); we say that $ \hat{E} $, with this structure, is the *Hausdorff completion* of the topological vector space $ E $, or simply the *completion* of $ E $ when $ E $ is *Hausdorff*.

### 5. Neighbourhoods of the origin in a topological vector space over a valued division ring

#### Definition 3 {#evt-i-s1-def-3 .statement}

*Let $ K $ be a valued division ring and $ E $ a left vector space over $ K $; we say that a subset $ M $ of $ E $ is balanced if, for all $ x \in M $ and all $ \lambda \in K $ such that $ |\lambda| \leq 1 $, it is true that $ \lambda x \in M $ (or in other words if $ \lambda M \subset M $ when $ |\lambda| \leq 1 $).*

#### Proposition 2 {#evt-i-s1-prop-2 .statement}

*In a topological vector space $ E $ over a valued division ring $ K $, the closure of a balanced set $ M $, is a balanced set.*

If $ B $ is the set of $ \xi \in K $ with $ |\xi| \leq 1 $; then $ B $ is closed in $ K $. But $ B \times M $ is mapped into $ M $ by the continuous mapping $ (\lambda, x) \mapsto \lambda x $; and therefore $ B \times \overline{M} $ is mapped into $ \overline{M} $ (GT, I, § 2.1, th. 1) which proves that $ \overline{M} $ is balanced.

When $ M $ is an arbitrary set in the vector space $ E $ over a valued division ring $ K $, the set $ M_1 $ of the $ \lambda x $ with $ x \in M $ and $ \lambda \in K $ such that $ |\lambda| \leq 1 $, is clearly the smallest balanced set containing $ M $; $ M_1 $ is called the *balanced envelope* of $ M $.

#### Proposition 3 {#evt-i-s1-prop-3 .statement}

*Let $ K $ be a valued locally compact and non-discrete division ring and $ E $ be a Hausdorff topological vector space (resp. a topological vector space) over $ K $. For every compact (resp. precompact) set $ H $ in $ E $, the balanced envelope of $ H $ is compact (resp. precompact).

If $ B $ denotes the ball $ |\xi| \leq 1 $ in $ K $, the balanced envelope of $ H $ is $ H_1 $, the image of $ B \times H $ under the continuous mapping $ m : (\lambda, x) \mapsto \lambda x $. If $ E $ is Hausdorff, if $ B $ is compact and if $ H $ is compact then so is $ B \times H $ and therefore $ H_1 $. If $ H $ is precompact the restriction of $ m $ to $ B \times H $ is uniformly continuous (I, p. 5, *Remark* 2) and as $ B \times H $ is precompact, so also is its image under $ m $ (GT, II, § 4.2, prop. 2).

Note that the balanced envelope of a closed set is not necessarily closed. For example, in $ \mathbf{R}^2 $, the balanced envelope of the hyperbola defined by the equation $ xy = 1 $ is not closed.

The union of a family of balanced sets in $ E $ is balanced, which implies that for every set $ M $ of $ E $ there is a largest balanced subset $ N $ of $ M $ called the *balanced core of* $ M $; also $ N $ is not empty if and only if $ 0 \in M $. To say that $ x \in N $ means that for all $ \lambda \in K $ such that $ |\lambda| \leq 1 $, we have $ \lambda x \in M $, or again (if $ 0 \in M $) that, for all $ \mu \in K $ with |μ| ≥ 1, we have x ∈ μM. If 0 ∈ M, the balanced core N of M is therefore the intersection $ \bigcap_{|\mu| \geq 1} \mu M $. This shows in particular that if M is closed, so also is N.

#### Definition 4 {#evt-i-s1-def-4 .statement}

*Let K be a non-discrete valued division ring and E be a left vector space on K with two subsets A and B. We say that A absorbs B if there exists α > 0 such that λA ⊃ B for every λ ∈ K with |λ| ≥ α (or equivalently if μB ⊂ A for μ ≠ 0 and |μ| ≤ α⁻¹). A set A of E is called absorbent if it absorbs every set consisting of a single point.*

Let A be a balanced set of E; for it to absorb a set B of E it is sufficient that there exists λ ≠ 0 such that λA ⊃ B; in fact, for |μ| ≥ |λ|, we have λA = (λμ⁻¹) μA, and as μA is balanced and |λμ⁻¹| ≤ 1, it follows that λA ⊂ μA, and thus B ⊂ μA. In particular for a balanced set A of E to be absorbent, it is necessary and sufficient that for every x ∈ E, there exists λ ≠ 0 in K such that λx ∈ A. Every absorbent set of E generates the vector space E. Every finite intersection of absorbent sets is an absorbent set.

#### Proposition 4 {#evt-i-s1-prop-4 .statement}

*In a topological vector space E on a non-discrete valued division ring K there exists a fundamental system $ \mathfrak{B} $ of closed neighbourhoods of 0 such that :
*(EV₁)* Every set V ∈ $ \mathfrak{B} $ is balanced and absorbent.
*(EV₂)* For every V ∈ $ \mathfrak{B} $ and λ ≠ 0 in K, we have λV ∈ $ \mathfrak{B} $ (invariance of $ \mathfrak{B} $ under homotheties of non zero ratio).
*(EV₃)* For every V ∈ $ \mathfrak{B} $, there exists W ∈ $ \mathfrak{B} $ such that W + W ⊂ V.

Conversely, let E be a vector space on K, and let $ \mathfrak{B} $ be a filter base on E satisfying the conditions (EV₁), (EV₂) and (EV₃). Then there exists a topology (and it is unique) on E, compatible with the vector space structure of E, and for which $ \mathfrak{B} $ is a fundamental system of neighbourhoods of 0.

By axiom (EVT'₃) we show firstly that the *balanced core*, V₁, of V, a neighbourhood of 0, is itself a neighbourhood of 0. For there exist α > 0 and a neighbourhood W of 0 such that, if |λ| ≤ α and x ∈ W, then λx ∈ V. Since K is non-discrete, there exists μ ≠ 0 in K with |μ| ≤ α and μW is a neighbourhood of 0 for which μW ⊂ V. Also if v ∈ K and |v| ≤ 1 then |vμ| ≤ α and thus vμW ⊃ V. Hence μW ⊃ V₁ and V₁ is a neighbourhood of 0. Also as V is closed so also V₁ is closed. Thus the set $ \mathfrak{B} $ of *closed balanced* neighbourhoods of 0 form a fundamental system of neighbourhoods of 0 in E. By (EVT₁') every neighbourhood of 0 is *absorbent*; furthermore $ \mathfrak{B} $ satisfies (EV₂) (*cf.* I, p. 3, cor.); finally, because of the continuity of (x, y) ↦ x + y at the point (0, 0), every fundamental system of neighbourhoods of 0 in E satisfies (EV₃). The set $ \mathfrak{B} $ satisfies the conditions of the proposition.

Now let E be a vector space over K, and $ \mathfrak{B} $ be a filter base on E satisfying (EV₁), (EV₂) and (EV₃). The axiom (EV₁) shows firstly that for all V ∈ $ \mathfrak{B} $, we have −V = V and 0 ∈ V; these relations and the axiom (EV₃) show that $ \mathfrak{B} $ is a fundamental system of neighbourhoods of 0, for a topology on E compatible with the *additive group* structure of E (GT, III, § 1.2). On the other hand the axioms (EVT'_I), (EVT'_II) and (EVT'_III) are immediate consequences of (EV_I) and (EV_II), thus the topology defined above satisfies the axiom (EVT), and the proposition is proved.

#### Remark {#evt-i-s1-n5-rem-1 .statement}

— 1) In a normed space on a non-discrete valued division ring the set of open balls (resp. closed balls) with centre 0 is a fundamental system of neighbourhoods of 0 which satisfy the conditions (EV_I), (EV_II) and (EV_III).

2) When the division ring of scalars K is the field \mathbf{R} or the field \mathbf{C}, every filter base \mathfrak{B} on E which satisfies just the two axioms (EV_I) and (EV_III) is a fundamental system of neighbourhoods of 0 for a topology compatible with the vector space structure of E. In fact, we need only prove that, in these conditions, for every $ \lambda \neq 0 $ in K and every $ V \in \mathfrak{B} $ there exists $ W \in \mathfrak{B} $ such that $ \lambda W \subset V $. Now from (EV_III) there exists $ W_1 \in \mathfrak{B} $ with $ 2\,W_1 \subset V $, and we deduce, inductively, that for every positive integer $ n $, there exists $ W_n \in \mathfrak{B} $ such that $ 2^n W_n \subset V $. As V is balanced, if we take $ n $ so large that $ 2^n = |2^n| > |\lambda| $, then $ W = W_n $ satisfies the condition, as required.

This result does not hold for every non-discrete valued division ring K, for in such a division ring it is no longer necessarily true that $ |m\varepsilon| = m $ for every positive integer $ m $ ($ \varepsilon $ indicates the unit element of the division ring ; cf. I, p. 22, exerc. 1).

3) If K is a discrete division ring, conditions (EVT'_I) and (EVT'_III) are true for any topology on E. Arguing as in prop. 4, one easily sees that if E is a topological vector space on K, then there exists $ \mathfrak{B} $, a fundamental system of closed neighbourhoods of 0 in E satisfying conditions (EV_II) and (EV_III). Conversely, if a filter base $ \mathfrak{B} $ on a vector space E over K is such that 0 belongs to all the sets of $ \mathfrak{B} $ and (EV_II), (EV_III) are true, then $ \mathfrak{B} $ is a fundamental system of neighbourhoods of 0 in a topology compatible with the vector space structure of E.

### 6. Criteria of continuity and equicontinuity

Let E and F be topological vector spaces over the same division ring K ; for a linear mapping $ f $ of E in F to be continuous, it is sufficient for it to be continuous at the origin (GT, III, § 2.8, prop. 23). This proposition generalizes as follows :

#### Proposition 5 {#evt-i-s1-prop-5 .statement}

— Let $ E_i (1 \leq i \leq n) $ and F be topological vector spaces on a non-discrete valued field K. In order that a multilinear mapping $ f $ of $ \prod_{i=1}^n E_i $ in F should be continuous in the product space $ \prod_{i=1}^n E_i $ it is sufficient for it to be continuous at $ (0, 0, ..., 0) $.

Let $ (a_1, a_2, ..., a_n) $ be an arbitrary point of $ \prod_{i=1}^n E_i $; we must show that for every neighbourhood W of 0 in F there exist neighbourhoods $ V_i $ of 0 in $ E_i $ ($ 1 \leq i \leq n $) such that the relations $ z_i \in V_i $ imply

$$
f(a_1 + z_1, a_2 + z_2, ..., a_n + z_n) - f(a_1, a_2, ..., a_n) \in W .
$$

Now, we can write

$$
f(a_1 + z_1, ..., a_n + z_n) - f(a_1, ..., a_n) = \sum_H u_H
$$

where $ H $ varies over the $ 2^n - 1 $ subsets of the set of integers $ \{ 1, 2, ..., n \} $, excluding the set $ \{ 1, 2, ..., n \} $ itself, and where $ u_H = f(y_1, y_2, ..., y_n) $, with $ y_i = a_i $ if $ i \in H $ and $ y_i = z_i $ if $ i \notin H $. There exist $ 2^n - 1 $ balanced neighbourhoods $ W_H $ of 0 in $ F $ such that $ \sum_H W_H \subset W $; on the other hand as $ f $ is continuous at $ (0, 0, ..., 0) $ by hypothesis, there exists in each $ E_i $ a neighbourhood $ U_i $ of 0 ($ 1 \leq i \leq n $) such that the $ n $ relations $ x_i \in U_i $ imply that $ f(x_1, ..., x_n) \in \bigcap_H W_H $. As $ U_i $ is absorbent, there exists $ \lambda_i \neq 0 $ in $ K $ such that $ \lambda_i a_i \in U_i $. Let $ \lambda $ be an element of $ K $ such that $ |\lambda| \geq \prod_{i \in H} |\lambda_i|^{-1} $ for each subset $ H $; we show that the neighbourhoods $ V_i = \lambda^{-n} U_i $, fulfill the required condition. We can write $ u_H = \mu f(x_1, ..., x_n) $ where $ x_i \in U_i $ for $ 1 \leq i \leq n $ and $ \mu = \lambda^{-np} (\prod_{i \in H} \lambda_i^{-1}) $, $ p $ being the number of integers of $ \{ 1, 2, ..., n \} $ not in $ H $. From the above $ |\mu| \leq 1 $, hence $ u_H \in \mu W_H \subset W_H $ since $ W_H $ is balanced. The proposition is established.

#### Proposition 6 {#evt-i-s1-prop-6 .statement}

*With the same hypotheses on $ E_i (1 \leq i \leq n) $ and on $ F $ as in prop. 5, in order that a set $ \mathcal{E} $ of multilinear maps of $ \prod_{i=1}^n E_i $ in $ F $ be equicontinuous it is sufficient that the set be equicontinuous at $ (0, 0, ..., 0) $.*

For, in the demonstration of prop. 5 the $ U_i (1 \leq i \leq n) $ can be taken such that the relation $ x_i \in U_i (1 \leq i \leq n) $ imply $ f(x_1, ..., x_n) \in \bigcap_H W_H $ for *every* mapping $ f \in \mathcal{E} $.

### 7. Initial topologies of vector spaces

#### Proposition 7 {#evt-i-s1-prop-7 .statement}

*Let $ (E_v)_{v \in I} $ be a family of topological vector spaces on a topological division ring $ K $. Let $ E $ be a vector space on $ K $ and for each $ v \in I $, let $ f_v $ be a linear mapping of $ E $ in $ E_v $. Then the coarsest topology on $ E $ which makes each function $ f_v $ continuous, is a topology $ \mathcal{T} $ compatible with the vector space structure of $ E $. Further, if for every $ x \in E $, $ \phi(x) $ denotes the point $ (f_v(x)) $ of the product space $ F = \prod_{v \in I} E_v $, then the topology $ \mathcal{T} $ is the inverse image of the topology of the subspace $ \phi(E) $ of $ F $ under the linear mapping $ \phi $.*

The last part of the proposition is a particular case of GT, I, § 4.1, prop. 3. The proposition then follows from the next lemma.

#### Lemma {#evt-i-s1-n7-lem-1 .statement}

— *Let $ M $ and $ N $ be two vector spaces, and $ g $ a linear mapping of $ M $ in $ N $. If $ \mathcal{T}_0 $ is a topology compatible with the vector space structure of $ N $, then the inverse image of $ \mathcal{T}_0 $ by $ g $ is compatible with the vector space structure of $ M $.*

We show, for example, that $ (\lambda, x) \mapsto \lambda x $ is continuous at each point $ (\lambda_0, x_0) $ of $ K \times M $. Put $ y_0 = g(x_0) $. Every neighbourhood of 0 in $ M $ contains a neighbourhood of the form $ g(U) $ where $ U $ is a neighbourhood of 0 in $ N $; by hypothesis there exists a neighbourhood $ V $ of 0 in $ K $ and a neighbourhood $ W $ of 0 in $ N $ such that the relations $ \lambda - \lambda_0 \in V $, and $ y - y_0 \in W $ imply $ \lambda y - \lambda_0 y_0 \in U $. Thus the relations $ \lambda - \lambda_0 \in V $, $ x - x_0 \in g(W) $ imply $ \lambda x - \lambda_0 x_0 \in g(U) $. We can show similarly that $ (x, y) \mapsto x - y $ is continuous in $ M \times M $.

For each index $ i \in I $, let $ \mathcal{B}_i $ be a fundamental system of neighbourhoods of 0 in $ E_i $. From the definition of the topology $ \mathcal{T} $, the filter of neighbourhoods of 0 for this topology is generated by unions of sets of the families $ f_i^{-1}(\mathcal{B}_i) $; in other words, the sets of the form $ \bigcap_k f_{i_k}^{-1}(V_{i_k}) $ form a fundamental system of neighbourhoods of 0 for $ \mathcal{T} $, the $ (i_k)_{1 \leq k \leq n} $ being any finite sequence of indices of I, and, for each index $ k $, $ V_{i_k} $ any set of $ \mathcal{B}_{i_k} $.

#### Corollary 1 {#evt-i-s1-prop-7-cor-1 .statement}

*Let G be a topological vector space on K. In order that a set H of mappings of G in E be equicontinuous, it is necessary and sufficient that, for all $ i \in I $, the set $ f_i \circ u $ where u varies in H should be equicontinuous.*

This is a particular case of GT, X, § 2.2, prop. 3.

#### Corollary 2 {#evt-i-s1-prop-7-cor-2 .statement}

*If the spaces $ E_i $ are Hausdorff, then in order that $ \mathcal{T} $ be Hausdorff, it is necessary and sufficient that, for every $ x \neq 0 $ in E, there should exist an index $ i \in I $, such that $ f_i(x) \neq 0 $.*

For $ \phi(E) $ is then a Hausdorff space, and in order that $ \mathcal{T} $ be Hausdorff, it is evidently necessary and sufficient that $ \phi $ be injective; note that we can then identify E (with $ \mathcal{T} $) with the subspace $ \phi(E) $ of $ \prod_{i \in I} E_i $ by the mapping $ \phi $.

#### Corollary 3 {#evt-i-s1-prop-7-cor-3 .statement}

*Suppose the $ E_i $ are complete and $ \phi(E) $ is closed in $ F = \prod_{i \in I} E_i $. Then E is complete in the topology $ \mathcal{T} $.*

For the subspace $ \phi(E) $ of F is then complete (GT, II, § 3.4, prop. 8 and § 3.5, prop. 10), therefore the same is true of E in the inverse image topology (GT, I, § 7.6, prop. 10 and GT, II, § 3.1, prop. 4).

#### Example {#evt-i-s1-n7-exa-1 .statement}

— Let $ \mathcal{D}'(\mathbf{R}) $ be the space of distributions on $ \mathbf{R} $; for $ p $ a number such that $ 1 \leq p \leq +\infty $, let $ j : L^p(\mathbf{R}) \to \mathcal{D}'(\mathbf{R}) $ be the canonical injection, which is continuous (when $ L^p(\mathbf{R}) $ carries its normed space topology and $ \mathcal{D}'(\mathbf{R}) $ the strong topology). For every distribution $ f \in \mathcal{D}'(\mathbf{R}) $, denote the derivative of $ f $ by $ D(f) $; recall that $ f \mapsto D(f) $ is a continuous endomorphism of $ \mathcal{D}'(\mathbf{R}) $. Then let E be the vector subspace of $ L^p(\mathbf{R}) $ formed from those $ f \in L^p(\mathbf{R}) $ for which $ D(f) \in L^p(\mathbf{R}) $, and confer on E the coarsest topology making the canonical injection $ i : E \to L^p(\mathbf{R}) $ and the mapping $ D : E \to L^p(\mathbf{R}) $ continuous ($ L^p(\mathbf{R}) $ carries its normed space topology). For this topology, the space E is *complete*. For, the image of E in $ F = L^p(\mathbf{R}) \times L^p(\mathbf{R}) $ by the mapping $ \phi : f \mapsto (f, D(f)) $ is *closed*, since it is the trace on $ L^p(\mathbf{R}) \times L^p(\mathbf{R}) $ of the image G of $ \mathcal{D}'(\mathbf{R}) $ in $ \mathcal{D}'(\mathbf{R}) \times \mathcal{D}'(\mathbf{R}) $ by the mapping

$$
\phi_0 : f \mapsto (f, D(f));
$$

now G is the graph of $ \phi_0 $, therefore closed in $ \mathcal{D}'(\mathbf{R}) \times \mathcal{D}'(\mathbf{R}) $ (GT, I, § 8.1, cor. 2 of prop. 2), and as $ \phi(E) $ is the inverse image of G by $ i \times i $, which is continuous, we see that $ \phi(E) $ is closed in F. \*

#### Corollary 4 {#evt-i-s1-prop-7-cor-4 .statement}

*Let E be a vector space over a topological division ring K, and let $ (\mathcal{T}_i)_{i \in I} $ be a family of topologies compatible with the vector space structure of E; then the upper bound $ \mathcal{T} $ of the topologies $ \mathcal{T}_i $ is compatible with the vector space structure of E.*

For, if $ E_t $ denotes the topological vector space obtained from $ E $ by the topology $ \mathcal{T}_t $, and $ f_t $ the identity map of $ E $ on $ E_t $, then $ \mathcal{T} $ is the coarsest topology making the $ f_t $ continuous.

### Exercises {#evt-i-s1-exercises}

See the [exercises for § 1](exercises/s1/).
