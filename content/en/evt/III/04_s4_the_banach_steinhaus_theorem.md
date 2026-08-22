---
book: evt
book_title: Topological Vector Spaces
chapter: III
chapter_title: SPACES OF CONTINUOUS LINEAR MAPPINGS
section: 4
section_title: The Banach-Steinhaus theorem
lang: en
source: evt-i-v
book_pages: TVS III.23-TVS III.28, TVS III.43-TVS III.46
pdf_pages: 0155-0160, 0175-0178
extraction: ocr
subsections:
    - "no": 1
      title: Barrels and barrelled spaces
      page: 24
      pdf_page: 156
    - "no": 2
      title: The Banach-Steinhaus theorem
      page: 25
      pdf_page: 157
    - "no": 3
      title: '**Bounded subsets of $ \mathcal{L}(E; F) $ (quasi-complete case)'
      page: 27
      pdf_page: 159
statements: 18
exercises: 21
content_sha256: ff2f868ada1841e3392167da48fee371699c8ed3d6ed90405e76db6ebf5ffcef
---

## § 4. THE BANACH-STEINHAUS THEOREM

*In this paragraph E denotes a locally convex space and E' its dual. Whenever we talk of the weak topology on E', we shall mean $ \sigma(E', E) $.*

### 1. Barrels and barrelled spaces

Proposition 1. — Let T be a subset of E. The following conditions are equivalent:

(i) T is convex, balanced, closed and absorbent.

(ii) T is the polar of a convex, balanced and weakly bounded set M in E'.

(iii) There exists a lower semi-continuous semi-norm p on E, such that T is the set of all x ∈ E satisfying p(x) ≤ 1.

(i) ⇒ (ii) : under the hypothesis of (i), let M = T°; then M is convex and balanced in E'. For every x ∈ E, there exists a real number r > 0 such that rx ∈ T, hence |u(x)| ≤ $ \frac{1}{r} $ for all u ∈ M; in other words M is weakly bounded. From cor. 3 of II, p. 45, we have T = M°, hence T satisfies (ii).

(ii) ⇒ (iii) : under the hypothesis of (ii), let $ p(x) = \sup_{u \in M} |u(x)| $ for all x ∈ E. It is immediate that T = M° consists of all x ∈ E such that p(x) ≤ 1. The semi-norm p on E' is lower semi-continuous, being the superior envelope of a family of continuous functions (GT, IV, § 6, No. 2, corollary).

(iii) ⇒ (i) : this is clear.

Corollary. — The following conditions are equivalent:

(i) every weakly bounded subset of E' is equicontinuous;

(ii) every convex, balanced, closed and absorbent set in E is a neighbourhood of 0;

(iii) every lower semi-continuous semi-norm on E is continuous.

Definition 1. — A set T satisfying the equivalent conditions of prop. 1 is said to be a barrel in E.

Definition 2. — A space E is said to be barrelled if it satisfies the equivalent conditions of the corollary of prop. 1.

We know (III, p. 22, prop. 9) that every equicontinuous subset of the dual E' of E is strongly and weakly bounded. We can therefore restate the definition of barrelled spaces as follows:

#### Scholium {#evt-iii-s4-n1-sch-1 .statement}

— In the dual of a barrelled space, the class of equicontinuous sets, the class of strongly bounded sets, the class of weakly bounded sets and the class of relatively compact sets for the weak topology are all identical. If E is Hausdorff and barrelled, and if E'_b is its strong dual, the polars of the neighbourhoods of 0 in one of the spaces form a base of the canonical bornology of the other, and the polars of bounded subsets of one of the spaces form a base for the filter of neighbourhoods of 0 of the other space.

Proposition 2. — Every locally convex space E which is a Baire space (GT, IX, § 5, No. 3) is barrelled.

Let T be a barrel in E; since T is absorbent, E is the union of closed sets nT (n integer > 0); since E is a Baire space, at least one of these sets contains an interior point, hence T itself has an interior point x. If $ x \neq 0 $, since $-x \in T$, and 0 is a point of the open segment with extremities x and $-x$, 0 is an interior point of the convex set T (II, p. 14, prop. 16). Therefore T is a neighbourhood of 0.

#### Corollary {#evt-iii-s4-n1-cor-1 .statement}

— *Every Fréchet space (and in particular, every Banach space) is barrelled.* This follows from Baire’s theorem (GT, IX, § 5, No. 3, th. 1).

#### Proposition 3 {#evt-iii-s4-prop-3 .statement}

— *Let $(F_i)_{i \in I}$ be a family of barrelled spaces, and for every $i \in I$, let $f_i$ be a linear mapping from $F_i$ into a vector space E. The space E with the finest locally convex topology for which the $f_i$ are continuous (II, p. 27, prop. 5), is a barrelled space.*

Let T be a barrel in E. Since $f_i$ is continuous, $f_i^{-1}(T)$ is a convex, balanced, closed and absorbent set in $F_i$; in other words, a barrel in $F_i$; since $F_i$ is barrelled, $f_i^{-1}(T)$ is a neighbourhood of 0 in $F_i$, for all $i \in I$. This implies that T is a neighbourhood of 0 in E (II, p. 27, prop. 5).

#### Corollary 1 {#evt-iii-s4-prop-3-cor-1 .statement}

— *Every quotient space of a barrelled space is barrelled.*

#### Corollary 2 {#evt-iii-s4-prop-3-cor-2 .statement}

— *Let $(E_i)_{i \in I}$ be a family of locally convex spaces and let E be the topological direct sum of this family. For E to be barrelled, it is necessary and sufficient that each $E_i$ is barrelled.*

The condition is evidently sufficient by virtue of prop. 3; it is also necessary, by cor. 1, since each $E_i$ is isomorphic to a quotient space of E (II, p. 31, prop. 8).

#### Corollary 3 {#evt-iii-s4-prop-3-cor-3 .statement}

— *Every inductive limit of barrelled spaces is a barrelled space.*

We shall prove later (IV, p. 14, corollary) that every product of barrelled spaces is barrelled.

### 2. The Banach-Steinhaus theorem

#### Theorem 1 {#evt-iii-s4-thm-1 .statement}

— *Let E be a barrelled space, F a locally convex space. Every simply bounded subset H of $\mathcal{L}(E; F)$ is equicontinuous.*

For, let $p$ be a continuous semi-norm on F; let $q = \sup_{u \in H} (p \circ u)$. Since H is simply bounded, we have $q(x) < +\infty$ for all $x \in E$ and $q$ is a lower semi-continuous semi-norm, being the finite superior envelope of continuous semi-norms. Since E is barrelled, $q$ is a continuous semi-norm and therefore H is equicontinuous.

#### Corollary 1 {#evt-iii-s4-thm-1-cor-1 .statement}

— *Let E and F be two Banach spaces, H a family of continuous linear mapping from E into F; if, for all $x \in E$, we have $\sup_{u \in H} \|u(x)\| < +\infty$, we also have $\sup_{u \in H} \|u\| < +\infty$.*

In fact, the hypothesis says that H is simply bounded and the conclusion that it is equicontinuous. In addition, every Banach space is barrelled (III, p. 25).

#### Corollary 2 {#evt-iii-s4-thm-1-cor-2 .statement}

— (Banach-Steinhaus theorem). — *Let E be a barrelled space, F a locally convex Hausdorff space, and let $(u_n)$ be a sequence of continuous linear mappings* from E into F, which converges simply to a mapping u from E into F. Then $ u \in \mathcal{L}(E; F) $, and $ (u_n) $ converges to u uniformly on every precompact subset of E.

The sequence $ (u_n) $ is, in fact, simply bounded, hence equicontinuous, and the corollary follows from the cor. of prop. 5 of III, p. 18.

#### Remark {#evt-iii-s4-n2-rem-1 .statement}

— 1) The property expressed by cor. 2 does not imply that E is barrelled : we shall see later that the strong dual of a Fréchet space possesses this property, while not necessarily being barrelled (IV, p. 23, cor. to prop. 2 and p. 58, exerc.

2) Let E and F be two Banach spaces, and $ (u_n) $ a sequence of continuous linear mappings from E into F such that $ \sup \|u_n\| = + \infty $. Then the set X of all $ x \in E $ such that $ \sup \|u_n(x)\| = + \infty $ is dense in E and is the intersection of a sequence of open sets in E. For, let $ X_k $ denote the set of all $ x \in E $ such that $ \sup \|u_n(x)\| > k $ (for k integer $ > 0 $). Each $ X_k $ is open and X is the intersection of the $ X_k $. Since E is a Baire space, it is enough to show that each $ X_k $ is dense in E. But, if the complement of $ X_k $ contains a non-empty open set U, we would have $ \|u_n(x)\| \leq 2k $ for $ x \in U - U $ and, since $ U - U $ is a neighbourhood of 0, we would have $ \sup \|u_n\| < + \infty $.

#### Corollary 3 {#evt-iii-s4-thm-1-cor-3 .statement}

— *Let E be a barrelled space, F a locally convex Hausdorff space and $ \Phi $ a filter on $ \mathcal{L}(E; F) $ which converges simply in E to a mapping u from E into F. If $ \Phi $ contains a simply bounded subset of $ \mathcal{L}(E; F) $, or if $ \Phi $ has a countable base, then u is a continuous linear mapping from E into F and $ \Phi $ converges uniformly to u on every precompact subset of E.*

Suppose first that $ \Phi $ contains a simply bounded set H ; since H is equicontinuous (th. 1), the corollary follows from the corollary of prop. 5 (III, p. 18). If $ \Phi $ has a countable base, every elementary filter $ \Psi $ associated with a sequence $ u_n $ (GT, I, § 6, No. 8) which is finer than $ \Phi $ is then simply convergent to u in E and it follows from cor. 2 that u is a continuous linear mapping from E into F, and that $ \Psi $ converges to u for the topology of uniform convergence on precompact subsets of E. Consequently, the same holds for $ \Phi $, since the latter is the intersection of elementary filters, each finer than $ \Phi $ (GT, I, § 6, No. 8).

We observe that a filter on $ \mathcal{L}(E; F) $ which converges simply and has a countable base does not necessarily contain a simply bounded set : to see this consider the example of the filter of neighbourhoods of 0 in $ \mathcal{L}(K; F) $ when the topology of F is metrizable, but cannot be defined by a single norm.

#### Example {#evt-iii-s4-n2-exa-1 .statement}

— Let E be the Banach space (over $ \mathbf{C} $) consisting of continuous complex functions with period 1 in $ \mathbf{R} $, with the norm $ \|f\| = \sup_x |f(x)| $.

For every integer $ n \in \mathbf{Z} $ and every function $ f \in E $, let $ c_n(f) = \int_0^1 f(x) e^{-2i\pi nx} dx $ ($ n $-th Fourier coefficient of $ f $) ; each of the mappings $ f \mapsto c_n(f) $ is a continuous linear form on E. Let $ (\alpha_n) $ be a sequence of complex numbers such that, for every function $ f \in E $, the serie with the general term $ \alpha_n c_n(f) + \alpha_{-n} c_{-n}(f) $ is convergent. Under these conditions, the mapping $ u : f \mapsto \alpha_0 c_0(f) + \sum_{n \geq 1} [\alpha_n c_n(f) + \alpha_{-n} c_{-n}(f)] $ is a continuous linear form on E ; \* in other words, there exists a measure $ \mu $ on $[0, 1]$ such that $ u(f) = \int f(x) d\mu(x) $ for every function $ f \in E $, and $ \alpha_n $ is the $ n $-th Fourier coefficient of $ \mu $.* In fact, for every integer $ m > 0 $, the mapping $ f \mapsto \sum_{k = -m}^m \alpha_k c_k(f) $ is a continuous linear form $ u_m $ on E, and for all $ f \in E $, the sequence $ (u_m(f)) $ converges to $ u(f) $, by hypothesis. The assertion then follows from Banach-Steinhaus theorem, since E is barrelled.

#### Corollary 4 {#evt-iii-s4-thm-1-cor-4 .statement}

— *Let E and F be two locally convex spaces, $ \mathfrak{S} $ a cover of E consisting of bounded subsets. If E is barrelled and F Hausdorff and quasi-complete, the space $ \mathcal{L}_{\mathfrak{S}}(E; F) $ is Hausdorff and quasi-complete.*

In fact, every bounded and closed subset of $ \mathcal{L}_{\mathfrak{S}}(E; F) $ is simply bounded (because $ \mathfrak{S} $ is a cover of E), hence equicontinuous (III, p. 25, th. 1) and consequently is a complete subspace of $ \mathcal{L}_{\mathfrak{S}}(E; F) $ because of prop. 11 (III, p. 22).

#### Corollary 5 {#evt-iii-s4-thm-1-cor-5 .statement}

— *The strong dual and the weak dual of a barrelled space are quasi-complete.*

### 3. **Bounded subsets of $ \mathcal{L}(E; F) $ (quasi-complete case)

#### Theorem 2 {#evt-iii-s4-thm-2 .statement}

— *Let E be a locally convex Hausdorff space, F a locally convex space and $ \mathfrak{S} $ a family of closed, convex, balanced, bounded and semi-complete subsets of E (III, p. 7). Every simply bounded subset H of $ \mathcal{L}(E; F) $ is bounded for the $ \mathfrak{S} $-topology.*

Let $ A \in \mathfrak{S} $. The space $ E_A $ is then a Banach space (III, p. 8, corollary), hence barrelled. On the other hand, the canonical image of H in $ \mathcal{L}(E_A; F) $ is simply bounded, hence equicontinuous (III, p. 25, th. 1). Consequently, the set of all $ u(x) $ for $ u \in H $ and $ x \in A $, is bounded in F, which proves that H is bounded for the $ \mathfrak{S} $-topology.

#### Corollary 1 {#evt-iii-s4-thm-2-cor-1 .statement}

— *Let E be a locally convex Hausdorff space, F a locally convex space, and $ \mathfrak{S} $ a family of bounded subsets of E. If E is semi-complete, then every simply bounded subset of $ \mathcal{L}(E; F) $ is bounded for the $ \mathfrak{S} $-topology.*

It is enough to apply th. 2, after replacing the sets of $ \mathfrak{S} $ by their closed, convex, balanced envelopes, since this does not change the $ \mathfrak{S} $-topology.

When E is semi-complete (for example quasi-complete), we can talk of the *bounded subsets* of $ \mathcal{L}(E; F) $ without specifying the $ \mathfrak{S} $-topology, since these are the same for all the $ \mathfrak{S} $-topologies whenever $ \mathfrak{S} $ is a cover of E.

#### Corollary 2 {#evt-iii-s4-thm-2-cor-2 .statement}

— *Every semi-complete bornological space is barrelled.*

Every simply bounded subset of the dual of such a space is strongly bounded (cor. 1), hence equicontinuous (III, p. 22, prop. 10).

#### Corollary 3 {#evt-iii-s4-thm-2-cor-3 .statement}

— *Let E be a locally convex space. Every subset of E which is bounded for $ \sigma(E, E') $ is bounded.*

Let A be a subset of E. Saying that A is bounded for $ \sigma(E, E') $ means that every continuous linear form on E is bounded on A ; Saying that A is bounded means that every continuous semi-norm on E is bounded on A. Let N be the closure of 0 in E and $ \pi $ the canonical mapping from E onto E/N. The continuous linear forms on E are the mappings of the form $ f \circ \pi $ with $ f \in (E/N)' $ and we have an analogous characterization of continuous semi-norms on E. Replacing E by E/N and A by $ \pi(A) $ we can thus limit ourselves to the case where E is Hausdorff.

Let $ \mathfrak{S} $ be the set of equicontinuous subsets of $ E' $; when $ E' $ is assigned the topology $ \sigma(E', E) $, $ E $ can be identified with $ (E')_{\mathfrak{S}}' $ (III, p. 19, cor. 1). Every closed equicontinuous subset of $ E' $ is compact for $ \sigma(E', E) $ (III, p. 17, cor. 2), hence complete for $ \sigma(E', E) $. It is now enough to apply th. 2.

### Exercises {#evt-iii-s4-exercises}

See the [exercises for § 4](exercises/s4/).
