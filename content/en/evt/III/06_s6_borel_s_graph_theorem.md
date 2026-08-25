---
book: evt
book_title: Topological Vector Spaces
chapter: III
chapter_title: SPACES OF CONTINUOUS LINEAR MAPPINGS
section: 6
section_title: Borel's graph theorem
lang: en
source: evt-i-v
book_pages: TVS III.49-TVS III.50
pdf_pages: 0166-0169, 0181-0182
extraction: ocr
subsections:
    - "no": 1
      title: Borel’s graph theorem
      page: 34
      pdf_page: 166
    - "no": 2
      title: Locally convex Lusin spaces
      page: 34
      pdf_page: 166
    - "no": 3
      title: Measurable linear mappings on a Banach space $^1$
      page: 36
      pdf_page: 168
statements: 8
exercises: 6
content_sha256: e379472db84810d5375451cb6502d4f3b37b304ba46555c234bad4be5f0f6752
---

## § 6. BOREL’S GRAPH THEOREM

### 1. Borel’s graph theorem

#### Theorem 1 {#evt-iii-s6-thm-1 .statement}

— Let E be a locally convex space which is the inductive limit of Banach spaces, F a Souslin locally convex space, for example a Lusin space (GT, IX, § 6, No. 2 and No. 4), and u a linear mapping from E into F. If the graph of u is a Borel subset of E × F, then u is continuous.

Let E_i be a family of Banach spaces, and (u_i) a family of continuous linear mappings u_i : E_i → E such that the topology of E is the finest locally convex topology for which the u_i are continuous. It is enough to prove that the composed mappings u ∘ u_i are continuous, or in fact (GT, IX, § 2, No. 6, prop. 10) that the restriction of u ∘ u_i to every closed subspace G of E_i satisfying the first axiom of countability is continuous. The graph of this restriction is the inverse image of the graph of u under the continuous mapping u_i × Id_F : G × F → E × F, hence is a Borel set in G × F. In addition, G × F is a Souslin space and every Borel subset of a Souslin space is a Souslin space (GT, IX, § 6, No. 3, prop. 10). Th. 1 then follows from th. 4, GT, IX, § 6, No. 8.

#### Remark {#evt-iii-s6-n1-rem-1 .statement}

Recall (III, p. 12) that every homological Hausdorff and semi-complete space, for example every Fréchet space, is the inductive limit of Banach spaces. \* This is also true for the strong dual of a reflexive Fréchet space (IV, p. 23, prop. 4). \*

### 2. Locally convex Lusin spaces

#### Proposition 1 {#evt-iii-s6-prop-1 .statement}

— Let E be a Hausdorff locally convex space. Suppose that there exists a sequence (E_n)_{n \in \mathbf{N}} of Fréchet spaces satisfying the first axiom of countability, and continuous linear mappings u_n : E_n → E such that E = \bigcup_{n \in \mathbf{N}} u_n(E_n). Then E is a Lusin space.

Let P_n be the kernel of u_n; then u_n defines a bijective continuous mapping from the quotient space E_n/P_n onto u_n(E_n). Since E_n/P_n is a Fréchet space satisfying the first axiom of countability (GT, IX, § 3, No. 1), hence a polish space (GT, IX, § 6, No. 1, def. 1), u_n(E_n) is a Lusin subspace of E (GT, IX, § 6, No. 4, prop. 11). Therefore by GT, IX, § 6, No. 7, cor. of th. 3, the space E, which is regular (GT, III, § 3, No. 1) is a Lusin space.

#### Example 1 {#evt-iii-s6-n2-exa-1 .statement}

Every Fréchet space satisfying the first axiom of countability is a polish space, hence a Lusin space. Consequently, so are the spaces $\mathcal{C}(X)$, where X is locally compact and has a countable base (the topology of $\mathcal{C}(X)$ being that of compact convergence, cf. GT, X, § 3, No. 3, corollary and § 1, No. 6, cor. 3); \* the spaces $\mathcal{C}_0^\infty(U)$, where U is an open subset of $\mathbf{R}^n$ (III, p. 9) and $\mathcal{H}(U)$, where U is an open subset of $\mathbf{C}^n$ (III, p. 10).

Prop. 1 shows that the spaces $\mathcal{C}_0^\infty(U)$, where U is an open set in $\mathbf{R}^n$, $\mathcal{G}_s(I)$, where I is a compact interval in $\mathbf{R}$ and $s \geq 1$, and $\mathcal{H}(K)$, where K is a compact subset of $\mathbf{C}^n$ are all Lusin spaces (III, p. 10). \*

#### Theorem 2 {#evt-iii-s6-thm-2 .statement}

— Let E be a locally convex space, which is the inductive limit of an increasing sequence $(E_n)_{n \in \mathbf{N}}$ of subspaces of E, endowed with the topologies of Fréchet spaces satisfying the first axiom of countability. Suppose that every compact subset of E is contained in one of the $E_n$ and is compact in this space. Let F be a Fréchet space satisfying the first axiom of countability. Then the space $\mathcal{L}_c(E; F)$ is a Lusin space.

The space E is bornological (III, p. 12), hence the space $\mathcal{L}_c(E; F)$ is complete (III, p. 23, prop. 12). The linear mapping $j : f \mapsto (f|E_n)_{n \in \mathbf{N}}$ is an injection from $\mathcal{L}_c(E; F)$ into the product space $\prod_{n \in \mathbf{N}} \mathcal{L}_c(E_n; F)$; by virtue of the hypothesis on the compact subsets of E and the definition of the $\mathfrak{S}$-topologies, $j$ is an isomorphism from $\mathcal{L}_c(E; F)$ onto its image (endowed with the topology induced by the product topology); moreover, since $\mathcal{L}_c(E; F)$ is complete, this image is a closed subspace of $\prod_{n \in \mathbf{N}} \mathcal{L}_c(E_n; F)$ (GT, II, § 3, No. 4, prop. 8). By GT, IX, § 6, No. 4, it is therefore enough to prove that each of the spaces $\mathcal{L}_c(E; F)$ is a Lusin space. For the rest of the proof, we shall assume that E is a Fréchet space satisfying the first axiom of countability.

Since F is a Fréchet space satisfying the first axiom of countability, it is isomorphic to a closed subspace of a countable product of Banach spaces $F_n$, each of which is a quotient of F (II, p. 5), hence satisfies the first axiom of countability. The linear mapping $j' : f \mapsto (\mathrm{pr}_n \circ f)_{n \in \mathbf{N}}$ is an injection from $\mathcal{L}_c(E; F)$ into the product space $\prod_{n \in \mathbf{N}} \mathcal{L}_c(E; F_n)$, and by using the definition of the $\mathfrak{S}$-topologies and of the open sets in a product, $j'$ is an isomorphism from $\mathcal{L}_c(E; F)$ onto its image; moreover, since $\mathcal{L}_c(E; F)$ is complete, this image is a closed subspace of $\prod_{n \in \mathbf{N}} \mathcal{L}_c(E; F)$. Therefore it is enough to prove that each of the spaces $\mathcal{L}_c(E; F_n)$ is a Lusin space (GT, IX, § 6, No. 4), and consequently, we can assume that F is a Banach space satisfying the first axiom of countability.

The space $\mathcal{L}_c(E; F)$ is the union of a countable family of equicontinuous and closed subsets (III, p. 19, cor. 1 and GT, X, § 2, No. 3, prop. 6). But every equicontinuous subset H of $\mathcal{L}_c(E; F)$ is metrizable and satisfies the first axiom of countability (III, p. 18, prop. 6 and GT, X, § 2, No. 4, th. 1); if H is closed, then it is a complete space for the uniform structure induced by that of $\mathcal{L}_c(E; F)$, since the latter is complete In other words, H is a polish space, and *a fortiori* a Lusin space; consequently the regular space $\mathcal{L}_c(E; F)$ is a Lusin space (GT, IX, § 6, No. 7, cor. of th. 3).

#### Corollary {#evt-iii-s6-n2-cor-1 .statement}

— *The hypotheses on E being as in th. 2, assume, in addition that every bounded subset of E is relatively compact. Then the strong dual of E is a Lusin space.* *In particular, the strong dual of a Fréchet space satisfying the first axiom of countability, which is also a Montel space, is a Lusin space.*

\* Example 2. — Let U be an open subset of $\mathbf{R}^n$. The corollary applies in particular to the Fréchet space $E = \mathcal{C}_c^\infty(U)$; its dual $\mathcal{C}_c^{-\infty}(U)$ (the space of distributions with compact support on U) is then a Lusin space.

The space $\mathcal{C}_c^\infty(U)$ is a strict inductive limit of a sequence of Fréchet spaces $\mathcal{C}_{K_n}^\infty(U)$ satisfying the first axiom of countability (III, p. 9). We can show that each of the spaces $\mathcal{C}_{K_n}^\infty(U)$ is a Montel space; in addition, every bounded subset of $\mathcal{C}_c^\infty(U)$ is contained in one of the spaces $\mathcal{C}_{K_n}^\infty(U)$ (III, p. 5, prop. 6). We can then apply the corollary of th. 2. Then the dual $\mathcal{C}_c^{-\infty}(U)$ of $\mathcal{C}_c^\infty(U)$ (the space of distributions on U) is a Lusin space for the strong topology.

Similarly we prove that for every open subset U of $\mathbf{C}^n$, and for every compact subset K of $\mathbf{C}^n$, the strong dual of $\mathcal{H}(U)$ and the strong dual of $\mathcal{H}(K)$ are Lusin spaces. \*

#### Remark {#evt-iii-s6-n2-rem-1 .statement}

— Let E be as in th. 2; let F be a Hausdorff locally convex space which is the union of the images of a sequence of continuous linear mappings $u_n : F_n \to F$, where each $F_n$ is a Fréchet space satisfying the first axiom of countability; then $\mathcal{L}_c(E ; F)$ is a Lusin space. As in prop. 1, we first reduce to the case where each $u_n$ is injective; then, as in the proof of th. 2, we can assume that E is a Fréchet space satisfying the first axiom of countability. Then, by I, p. 20, prop. 1, $\mathcal{L}(E ; F)$ is the union of the $\mathcal{L}(E ; F_n)$; moreover, the canonical injection $\mathcal{L}_c(E ; F_n) \to \mathcal{L}_c(E ; F)$ is continuous (GT, X, § 1, No. 4, prop. 3). Since each of the spaces $\mathcal{L}_c(E ; F_n)$ is a Lusin space by th. 2, $\mathcal{L}(E ; F_n)$ is also a Lusin space for the topology induced by that of $\mathcal{L}_c(E ; F)$ (GT, IX, § 6, No. 4, prop. 11); consequently $\mathcal{L}_c(E ; F)$ is a Lusin space by virtue of GT, IX, § 6, No. 7, corollary of th. 3.

### \*3. Measurable linear mappings on a Banach space $^1$

#### Proposition 2 {#evt-iii-s6-prop-2 .statement}

— *Let E be a Banach space, F a locally convex space and u a linear mapping from E into F. Assume that for every closed subset B of F, every compact subset X of E and every measure $\mu$ on X, the intersection $X \cap u^{-1}(B)$ is $\mu$-measurable. Then u is continuous.*

First assume that F is the base field. For every compact subset X of E and every measure $\mu$ on X, the restriction of $u$ to X is $\mu$-measurable (INT, IV). Suppose that $u$ is not continuous. Then we can find a sequence of points $(x_n)$ in E such that $\sum_n \| x_n \| < \infty$ and $|u(x_n)| \geq n$ for every integer $n$. Consider the mapping $g : (t_n) \mapsto \sum_n t_n x_n$ from the cube $C = [0, 1]^{\mathbf{N}}$ into E; it is clear that $g$ is continuous. Hence $f = u \circ g$ is measurable for every measure on C (INT, V); in particular for the measure $\mu$ which is the product of Lebesgue measures on the factors of C. Hence there exists a compact subset D of C such that $\mu(D) > \frac{1}{2}$ and such that the restriction of $f$ to D is continuous, hence also bounded. Let M be the upper bound of $|f|$ on D and let $p \in \mathbf{N}$ be such that $p \geq 4M$. Let $s = (s_n)$ and $t = (t_n)$ be two points of D such that $s_n = t_n$ for all $n \neq p$. Then

$$
f(s) - f(t) = u(\sum_n s_n x_n - \sum_n t_n x_n) = (s_p - t_p) u(x_p) .
$$

Since $|f(s) - f(t)| \leq 2M$ and $|u(x_p)| \geq p \leq 4M$, we get

$$
|s_p - t_p| \leq \frac{1}{2} .
$$

The Lebesgue-Fubini theorem (INT, V, 2nd ed., § 8, No. 3, cor. 2 of prop. 7) implies that $\mu(D) \leq \frac{1}{2}$; this gives a contradiction. Hence $u$ is continuous.

In the general case, for every $v \in F'$, the linear form $v \circ u$ is continuous, by the preceding argument. Let $(x_n)_{n \in \mathbf{N}}$ be a sequence of points of E tending to 0; then the sequence $(u(x_n))_{n \in \mathbf{N}}$ tends to 0 in F, if F is assigned the topology $\sigma(F, F')$; hence this sequence is bounded for $\sigma(F, F')$ and so it is bounded in F (III, p. 27, cor. 3). Since E is bornological (III, p. 12, prop. 2); the linear mapping $u : E \to F$ is continuous. \*

$^1$ The results of this section depend on the book of Integration.

Exercises

### Exercises {#evt-iii-s6-exercises}

See the [exercises for § 6](exercises/s6/).
