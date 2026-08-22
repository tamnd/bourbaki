---
book: evt
book_title: Topological Vector Spaces
chapter: I
chapter_title: TOPOLOGICAL VECTOR SPACES OVER A VALUED DIVISION RING
section: 3
section_title: Metrisable topological vector spaces
lang: en
source: evt-i-v
book_pages: TVS I.28-TVS I.29
pdf_pages: 0024-0030, 0036-0037
extraction: ocr
subsections:
    - "no": 1
      title: Neighbourhoods of 0 in a metrisable topological vector space
      page: 16
      pdf_page: 24
    - "no": 2
      title: Properties of metrisable vector spaces
      page: 17
      pdf_page: 25
    - "no": 3
      title: Continuous linear functions in a metrisable vector space
      page: 17
      pdf_page: 25
statements: 11
exercises: 9
content_sha256: 3f9d6ffe144af4f7f06621a65e3c7b30c95b9f58e434288523f844d78845614d
---

## § 3. METRISABLE TOPOLOGICAL VECTOR SPACES

### 1. Neighbourhoods of 0 in a metrisable topological vector space

We say that a topological vector space E is *metrisable* if its topology is metrisable. Relative to the structure of its additive group and of its topology, E is, therefore, a metrisable group (GT, IX, § 3.1).

We know that, for a topological group to be metrisable, it is necessary and sufficient that there exists an enumerable fundamental system of neighbourhoods of the neutral element $ e $, whose intersection is the single element $ e $ (GT, IX, § 3.1, prop. 1).

Also we know that the uniform structure of a metrisable topological vector space E, can be defined by an *invariant distance* $ d(x, y) = |x - y| $, where $ x \mapsto |x| $ is a continuous mapping of E in $ \mathbf{R}_+ $ which satisfies the conditions : 1) $ |-x| = |x| $; 2) $ |x + y| \leq |x| + |y| $; 3) the relation $ |x| = 0 $ is equivalent to $ x = 0 $ (GT, IX, § 3.1, prop. 3).

We saw (GT, IX.§ 3.1, prop. 2) how such a distance d could be defined using a decreasing sequence $ (W_n) $ of neighbourhoods of 0 in E, forming a fundamental system of neighbourhoods and such that $ W_{n+1} + W_{n+1} + W_{n+1} \subset W_n $. When E is a metrisable vector space over a non-discrete valued division ring K, we can also suppose that the $ W_n $ are balanced (I, p. 7, prop. 4); if we revert to the process of definition of $ d $ (*loc. cit.*) we can see that the *relation* $ |\lambda| \leq 1 \implies |\lambda x| \leq |x| $. Further the conditions (EVT$_I$) and (EVT$_{II}$) of I, p. 2 imply both that $ |\lambda x_0| $ *tends to 0 as $ \lambda $ tends to 0 in K* for every $ x_0 \in E $, and that $ |\lambda_0 x| $ *tends to 0 as $ |x| $ tends to 0* for every $ \lambda_0 \in K $. Conversely, if the function $ |x| $ possesses all the preceding properties and if $ W_n $ is the set of $ x \in E $ such that $ |x| \leq 2^{-n} $, then the $ W_n $ form a fundamental system of balanced neighbourhoods of 0 for a metrisable topology on E that is compatible with the vector space structure of E.

#### Remark {#evt-i-s3-n1-rem-1 .statement}

— One of the most important classes of metrisable vector spaces are the normed spaces (I, p. 3). But it must be noted that there exist metrisable vector spaces whose topology cannot be defined by a norm (I, § 3, exerc. 1); we shall study important examples later.

### 2. Properties of metrisable vector spaces

Every vector subspace of a metrisable topological vector space E is metrisable; the same is true of every quotient space E/M of E by a closed vector subspace M (GT, IX, § 3.1, prop. 4). Every product of an enumerable family of metrisable topological vector spaces is metrisable (GT, IX, § 2.4, cor. 2). If K_0 is a complete valued division ring, and K is a subdivision ring everywhere dense in K_0, the completion $ \hat{E} $ of a metrisable vector space E over K is a metrisable vector space over K_0 (I, p. 6 and GT, IX, § 2, No. 1, prop. 1). Finally, if E is a metrisable vector space that is complete, then for every closed vector subspace M of E, the quotient space E/M is complete (GT, IX, § 3.1, prop. 4).

### 3. Continuous linear functions in a metrisable vector space

#### Theorem 1 (Banach) {#evt-i-s3-thm-1 .statement}

Let E and F be two metrisable vector spaces over a non-discrete valued division ring K, and let u be a continuous linear mapping of E in F. Suppose that E is complete. Then the following conditions are equivalent:
(i) u is a strict surjective morphism.
(ii) F is complete and u is surjective.
(iii) The image of u is not meagre in F (GT, IX, § 5.2).
(iv) For every neighbourhood V of 0 in E, the set $ \overline{u(V)} $ is a neighbourhood of 0 in F.

Firstly (i) implies (ii), for let u be a strict surjective morphism and N be the kernel of u. Then u induces an isomorphism of E/N on F. But E is metrisable and complete, hence E/N is complete (GT, IX, § 3.1, prop. 4), therefore F is complete.

Next (ii) implies (iii). Let F be complete and u be surjective. The image of u is precisely F and therefore not meagre in F from Baire’s theorem (GT, IX, § 5.3).

The following lemma shows that (iii) implies (iv).

#### Lemma 1 {#evt-i-s3-lem-1 .statement}

— Let E and F be two topological vector spaces over a non-discrete valued division ring K, and let u be a continuous linear mapping of E in F such that the image of E is not meagre. Then, for every neighbourhood V of 0 in E, the set $ \overline{u(V)} $ is a neighbourhood of 0 in F.

Let W be a balanced neighbourhood of 0 in E such that W + W ⊂ V (I, § 1.5, prop. 4). Let α be an element of K such that |α| > 1; then E is the union of the sets $ \alpha^n W $ where n varies in $ \mathbf{N} $; in fact, for all x ∈ E, there exists β ∈ K such that x ∈ βW (I, p. 7, prop. 4) and there exists an integer n ≥ 0 such that |β| < |α|^n, then x ∈ $ \alpha^n W $ since W is balanced. Hence, u(E) is the union of the sequence of sets $ u(\alpha^n W) = \alpha^n u(W) $, and as u(E) is not meagre in F, one at least of the sets $ \alpha^n \overline{u(W)} $ possesses an interior point (GT, IX, § 5.3, def. 2) and therefore $ \overline{u(W)} $ has an interior point.

Let $ y_0 $ be an interior point of $ \overline{u(W)} $; since $ -u(W) = u(W) $, and therefore $ -\overline{u(W)} = \overline{u(W)} $ it follows that $ 0 = y_0 + (-y_0) $ is an interior point of $ \overline{u(W)} + \overline{u(W)} $. As vector addition is a continuous mapping of $ F \times F $ in $ F $, the set $ \overline{u(W)} + \overline{u(W)} $ is contained in the closure of the set

$$
u(W) + u(W) = u(W + W) \subset u(V);
$$

hence $ \overline{u(V)} $ is a neighbourhood of 0 in $ F $.

Before proving that (iv) implies (i) we prove the following lemma, where we make the convention that, in all metric spaces, $ B_r(x) $ denotes the *closed* ball of centre $ x $ and radius $ r $.

#### Lemma 2 {#evt-i-s3-lem-2 .statement}

*Let E and F be two metric spaces, and suppose that E is also complete. Let u be a linear mapping of E in F having the following property: whatever the number $ r > 0 $, there exists a number $ \rho(r) > 0 $ such that, for all $ x \in E $, we have*

$$
B_{\rho(r)}(u(x)) \subset \overline{u(B_r(x))}.
$$

*In these conditions, for all $ a > r $, the image $ u(B_a(x)) $ contains the ball $ B_{\rho(r)}(u(x)) $.*

Let $ (r_n) $ be an infinite sequence of numbers $ > 0 $ such that $ r_1 = r $ and $ a = \sum_{n=1}^{\infty} r_n $. For each index $ n $ there exists a number $ \rho_n > 0 $ (with $ \rho_1 = \rho(r) $) such that

$$
B_{\rho_n}(u(x)) \subset \overline{u(B_{r_n}(x))}
$$

for all $ x \in E $; we can, and will, suppose that $ \lim_{n \to \infty} \rho_n = 0 $.

Let $ x_0 $ be a point of E, and $ y $ be a point of $ B_{\rho(r)}(u(x_0)) $. We shall show that $ y $ belongs to $ u(B_a(x_0)) $.

For this, a sequence $ (x_n)_{n>0} $ of points of E is defined inductively such that, for all $ n \geq 1 $, we have $ x_n \in B_{r_n}(x_{n-1}) $ and $ u(x_n) \in B_{\rho_{n+1}}(y) $. If the $ x_i $ have been defined for $ 0 \leq i \leq n-1 $ satisfying these relations, then we have $ y \in B_{\rho_n}(u(x_{n-1})) $; since

$$
B_{\rho_n}(u(x_{n-1})) \subset \overline{u(B_{r_n}(x_{n-1}))},
$$

there exists a point $ x_n \in B_{r_n}(x_{n-1}) $ whose image $ u(x_n) $ belongs to the neighbourhood $ B_{\rho_{n+1}}(y) $ of $ y $, which establishes the existence of the sequence $ (x_n) $.

Since the distance of $ x_n $ from $ x_{n+p} $ is less than $ r_{n+1} + r_{n+2} + \cdots + r_{n+p} $, which is arbitrarily small when $ n $ is large, the sequence $ (x_n) $ is a Cauchy sequence in E. As E is complete, the sequence $ (x_n) $ converges to a point $ x $ of E. The distance of $ x_0 $ from $ x $ is less than $ \sum_{n=1}^{\infty} r_n = a $, thus $ x \in B_a(x_0) $. But $ u $ is continuous, thus the sequence $ u(x_n) $ converges to $ u(x) $; also $ u(x_n) \in B_{\rho_{n+1}}(y) $, hence $ y = u(x) $, and the lemma is proved.

We return to the theorem and show that (iv) implies (i). Suppose that $ u $ satisfies condition (iv). For each of the spaces E and F, consider a distance that is invariant under translation and defines its topology (I, p. 16). By hypothesis, the set $ \overline{u(B_r(0))} $ is a neighbourhood of 0 in F for every $ r > 0 $, and thus there exists a number $ \rho(r) > 0 $ such that $ B_{\rho(r)}(0) \subset u(B_r(0)) $. By translation we conclude that $ B_{\rho(r)}(u(x)) \subset \overline{u(B_r(x))} $ for all $ r > 0 $ and all $ x \in E $. From lemma 2, for every pair of real positive numbers $ (a, r), a > r > 0 $, we have $ B_{\rho(r)}(0) \subset u(B_a(0)) $; thus $ u $ is a strict morphism of E on F. We have shown that (iv) implies (i) and the proof of the theorem is completed.

#### Corollary 1 {#evt-i-s3-lem-2-cor-1 .statement}

*If E and F are two complete metrisable vector spaces over a non-discrete valued division ring, then every bijective continuous linear mapping of E on F is an isomorphism.*

In particular, if E and F are two complete *normed* spaces, there exists a number $ a > 0 $ such that $ \|u(x)\| \geq a.\|x\| $ for all $ x \in E $.

#### Corollary 2 {#evt-i-s3-lem-2-cor-2 .statement}

*Let E be a vector space over a non-discrete valued division ring, let $ \mathcal{T}_1 $ and $ \mathcal{T}_2 $ be two topologies on E compatible with its vector space structure and for each of which E is metrisable and complete. Then, if $ \mathcal{T}_1 $ and $ \mathcal{T}_2 $ are comparable, they are identical.*

#### Corollary 3 {#evt-i-s3-lem-2-cor-3 .statement}

*Let E and F be two complete metrisable vector spaces over a non-discrete valued division ring. In order that a continuous linear mapping u of E in F should be a strict morphism, it is necessary and sufficient that $ u(E) $ be closed in F.*

The condition is necessary, because if $ u $ is a strict morphism, the image $ u(E) $, being isomorphic to the quotient $ E/u^{-1}(0) $, is complete (I, p. 17) and therefore closed in F. The condition is sufficient, since, if $ u(E) $ is closed in F, then $ u(E) $ must be a complete metrisable vector space and thus by theorem 1 $ u $ is a strict morphism of E on $ u(E) $.

#### Corollary 4 {#evt-i-s3-lem-2-cor-4 .statement}

*Let E be a complete metrisable vector space over a non-discrete valued division ring. If M and N are two closed vector subspaces, that are (algebraic) complements in E, then E is the direct topological sum of M and N.*

For $ M \times N $ is a complete metrisable vector space and the mapping $ (y, z) \mapsto y + z $ of $ M \times N $ on E is continuous and bijective, therefore an isomorphism (cor. 1).

#### Corollary 5 (The closed graph theorem) {#evt-i-s3-lem-2-cor-5 .statement}

— *Let E and F be two complete metrisable vector spaces over a non-discrete valued division ring. In order that a linear mapping u of E in F be continuous, it is necessary and sufficient that its graph, in the product space $ E \times F $, be closed.*

The condition is necessary since the graph of a continuous mapping into a Hausdorff space is closed (GT, I, § 8.1, cor. 2). To see that it is sufficient, note that it implies that the graph G of $ u $, which is a closed vector subspace of the complete metrisable space $ E \times F $, is itself metrisable and complete. The projection $ z \mapsto \mathrm{pr}_1(z) $ of G on E is a bijective, continuous linear mapping, therefore an isomorphism (cor. 1); since its inverse mapping is $ x \mapsto (x, u(x)) $, it follows that $ u $ is continuous in E.

We can express this corollary in the following form : $ u $ is continuous if the following situation holds : if the sequence $ (x_n) $ of points of E both converges to 0 and *is such that the sequence* $ (u(x_n)) $ *converges to* $ y $, then it is necessarily the case that $ y = 0 $.

#### Example {#evt-i-s3-n3-exa-1 .statement}

— Let E be a vector subspace of the space of real-valued functions defined on $ I = [0, 1] $; let $ \| f \| $ be a norm on E, under which E is *complete*, and such that its topology is finer than the topology of simple convergence. Suppose further that E contains the set $ \mathcal{C}^\infty(I) $ of functions infinitely differentiable on I; we shall show that there exists an integer $ k \geq 0 $, such that E contains the set $ \mathcal{C}^k(I) $ of all functions with a continuous $ k $-th derivative in I.

For every pair of integers $ m > 0,\ n \geq 0 $, let $ V_{mn} $ be the set of functions $ f \in \mathcal{C}^\infty(I) $ such that $ |f^{(h)}(x)| \leq 1/m $ for $ 0 \leq h \leq n $ and for all $ x \in I $. The $ V_{m,n} $ form a fundamental system of neighbourhoods of 0 for a metrisable topology compatible with the vector space structure of $ \mathcal{C}^\infty(I) $, further $ \mathcal{C}^\infty(I) $ is *complete* in this topology (FVR, II, p. 2, th. 1). Let $ u $ be the canonical mapping of $ \mathcal{C}^\infty(I) $ in E; we show that $ u $ is *continuous*. From cor. 5 above it is sufficient to prove that if a sequence $ (f_n) $ converges to 0 in $ \mathcal{C}^\infty(I) $ and to a limit $ f $ in E then necessarily $ f = 0 $. But this is immediate since, by hypothesis, $ f $ is the simple convergence limit of $ (f_n) $. Hence there exists an integer $ k \geq 0 $ and a number $ a > 0 $ such that the relation

$$
p_k(f) = \sup_{\substack{x \in I \\ 0 \leq h \leq k}} |f^{(h)}(x)| \leq a
$$

implies $ \| f \| \leq 1 $ for all $ f \in \mathcal{C}^\infty(I) $.

But $ p_k $ is a norm on the space $ \mathcal{C}^k(I) $ and $ \mathcal{C}^\infty(I) $ is a subspace that is everywhere dense in $ \mathcal{C}^k(I) $ for this norm (the set of polynomials being already everywhere dense in $ \mathcal{C}^k(I) $, an immediate consequence of the Weierstrass-Stone theorem). By what has gone before, the identity mapping of $ \mathcal{C}^\infty(I) $ (carrying the norm $ p_k $) in E, is continuous, and so it can be extended continuously to the whole space $ \mathcal{C}^k(I) $ (since E is complete). This proves our assertion.

#### Proposition 1 {#evt-i-s3-prop-1 .statement}

*Let E, F be two topological vector spaces over a non-discrete valued division ring K. We suppose that :*

1) E *is metrisable and complete*.
2) *There exists a sequence* $ (F_n) $ *of complete metrisable vector spaces over K and, for each n, an injective continuous linear mapping* $ v_n $ *of* $ F_n $ *in F such that F is the union of the subspaces* $ v_n(F_n) $.

*Then let u be a linear mapping of E in F. If the graph of u is closed in* $ E \times F $, *then there exists an integer n and a continuous linear mapping* $ u_n $ *of E in* $ F_n $ *such that* $ u = v_n \circ u_n $ *(which implies that u is continuous and that* $ u(E) \subset v_n(F_n) $).*

Let G be the graph of $ u $ in $ E \times F $. For all $ n $, we consider the continuous linear mapping $ w_n : (x, y) \mapsto (x, v_n(y)) $ of $ E \times F_n $ in $ E \times F $; as G is closed, the set $ w_n^{-1}(G) = G_n $ is a closed vector subspace of $ E \times F_n $; if $ p_n $ is the restriction to $ G_n $ of the first projection $ \mathrm{pr}_1 $, we have $ p_n(G_n) = u^{-1}(v_n(F_n)) $. As $ p_n $ is continuous and $ G_n $ is complete (since $ G_n $ is closed in the complete space $ E \times F_n $), $ p_n(G_n) $ is, by theorem 1, either meagre in E or it is the whole of E. But, by hypothesis, E is the union of the $ p_n(G_n) $, and as E is complete, the $ p_n(G_n) $ cannot all be meagre in E by Baire’s theorem (GT, IX, § 5.3, th. 1). Therefore there exists an integer n such that $ p_n(G_n) = E $, or in other words $ u(E) \subset v_n(F_n) $. Further, as $ v_n $ is injective, $ G_n $ is the graph of a linear mapping $ u_n $ of E in $ F_n $, and by the closed graph theorem (I, p. 19, cor. 5) $ u_n $ is *continuous*; it follows then from the definitions that $ u = v_n \circ u_n $.

Exercises

### Exercises {#evt-i-s3-exercises}

See the [exercises for § 3](exercises/s3/).
