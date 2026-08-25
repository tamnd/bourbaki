---
book: int
book_title: Integration
chapter: V
chapter_title: INTEGRATION OF MEASURES
section: 7
section_title: Integration with respect to an induced measure
lang: en
source: int-i-vi
book_pages: INT V.74-INT V.78, INT V.112-INT V.114
pdf_pages: 0329-0333, 0367-0369
extraction: ocr
subsections:
    - "no": 1
      title: Integration with respect to an induced measure
      page: 74
      pdf_page: 329
    - "no": 2
      title: Properties of induced measures
      page: 77
      pdf_page: 332
statements: 20
exercises: 11
content_sha256: 4ecc2c2ebe5af11cad1fd2fc9b49c9e7ed029e1548c1c274e34065846fe89224
---

## § 7. INTEGRATION WITH RESPECT TO AN INDUCED MEASURE

### 1. Integration with respect to an induced measure

Let $X$ be a locally compact subspace of $T$, $\mu$ a positive measure on $T$, and $\mu_X$ the measure induced on $X$ by $\mu$ (Ch. IV, §5, No. 7). For every $t \in T$, let us define a measure $\lambda_t$ *on* $X$ in the following way: $\lambda_t = \varepsilon_t$ if $t \in X$, $\lambda_t = 0$ if $t \in \mathbf{C}X$. For every finite numerical function $g$ defined on $X$, $\int g(x) d\lambda_t(x) = g(t)$ if $t \in X$ and $\int g(x) d\lambda_t(x) = 0$ if $t \in \mathbf{C}X$. If $g$ is a function in $\mathcal{K}(X)$ we therefore have, by the definition of $\mu_X$,

$$
\mu_X(g) = \int \langle g, \lambda_t \rangle d\mu(t) .
$$

This means that one can write

$$
\mu_X = \int \lambda_t d\mu(t)
$$

(§3, No. 1).

Let us now define a mapping $\pi$ of T into X by setting $\pi(t) = t$ for $t \in X$, and $\pi(t) = t_0$ for $t \in \mathbf{C}X$, $t_0$ being an arbitrary point of X; one can write $\lambda_t = \varphi_X(t)\varepsilon_{\pi(t)}$ for every $t \in T$. The mapping $\pi$ is $\mu$-measurable, because its restrictions to X and $\mathbf{C}X$ are (Ch. IV, §5, No. 10, Prop. 16); it follows at once that the pair $(\pi, \varphi_X)$ is $\mu$-adapted (§4, No. 1). We therefore have the following results:

#### Proposition 1 {#int-v-s7-prop-1 .statement}

— *For every numerical function* $g \geqslant 0$ *defined on* X,

$$
\int^\bullet g\,d\mu_X = \int_X g\,d\mu
$$

(cf. §5, No. 3, *Example*, for the notation $\int_X^\bullet$).

Taking into account the preceding remarks and (2), the relation (3) follows from Th. 1 of §4.

#### Corollary 1 {#int-v-s7-prop-1-cor-1 .statement}

— *For every subset* B *of* X, $\mu_X^\bullet(B) = \mu^\bullet(B)$; *for* B *to be locally* $\mu_X$*-negligible, it is necessary and sufficient that* B *be locally* $\mu$*-negligible*.

#### Corollary 2 {#int-v-s7-prop-1-cor-2 .statement}

— *Let* M *be a subset of* T. *If* $\mu$ *is concentrated on* M, *then* $\mu_X$ *is concentrated on* $M \cap X$.

#### Corollary 3 {#int-v-s7-prop-1-cor-3 .statement}

— *For the measure* $\mu_X$ *to be zero, it is necessary and sufficient that* X *be locally* $\mu$*-negligible*.

#### Remark {#int-v-s7-n1-rem-1 .statement}

— If S is the support of $\mu$, then $S \cap X$ (which is closed in X) contains the support of $\mu_X$ by Cor. 2, but may be distinct from it. For example, if $\mu$ is a diffuse measure and X is a subspace reduced to a point, then the induced measure $\mu_X$ is zero, hence its support is empty. Note, however, that the support of $\mu_X$ is equal to $S \cap X$ if X is open in T.

#### Proposition 2 {#int-v-s7-prop-2 .statement}

— *For a mapping* g *of* X *into a topological space to be* $\mu_X$*-measurable, it is necessary and sufficient that* g *be* $\mu$*-measurable in* X *(§5, No. 3, *Example*)*.

This follows from Prop. 3 of §4.

#### Corollary {#int-v-s7-n1-cor-1 .statement}

— *For a subset* B *of* X *to be* $\mu_X$*-measurable, it is necessary and sufficient that* B *be* $\mu$*-measurable*.

#### Theorem 1 {#int-v-s7-thm-1 .statement}

— *Let* g *be a function defined on* X, *with values in* $\overline{\mathbf{R}}$ *or in a Banach space. For* g *to be essentially* $\mu_X$*-integrable, it is necessary* and sufficient that $g$ be essentially $\mu$-integrable in $X$ (\S 5, No. 3, Example), in which case

$$
\int g \, d\mu_X = \int_X g \, d\mu.
$$

This follows from Th. 2 of \S 4.

#### Corollary 1 {#int-v-s7-thm-1-cor-1 .statement}

*For a subset B of X to be essentially $\mu_X$-integrable, it is necessary and sufficient that it be essentially $\mu$-integrable, in which case $\mu_X(B) = \mu(B)$.*

#### Corollary 2 {#int-v-s7-thm-1-cor-2 .statement}

*Let g be a complex function defined on T and locally $\mu$-integrable; the restriction $g_X$ of g to X is then locally $\mu_X$-integrable, and*

$$
(g \cdot \mu)_X = g_X \cdot \mu_X.
$$

This follows at once from Th. 1, applied to the functions $fg_X$ ($f \in \mathcal{K}(X; \mathbf{C})$), and the definition of the measure induced on X by a complex measure (Ch. IV, \S 5, No. 7).

#### Corollary 3 {#int-v-s7-thm-1-cor-3 .statement}

*Let $\theta$ be a complex measure on T; then*

$$
|\theta|_X = |\theta_X|.
$$

Set $|\theta| = \mu$ and apply Cor. 2 on taking $g$ to be a complex function of absolute value 1 such that $\theta = g \cdot \mu$ (\S 5, No. 5, Cor. 3 of Th. 2); then $\theta_X = g_X \cdot \mu_X$; but $g_X$ is a function of absolute value 1, and the formula (6) follows from Prop. 2 of \S 5, No. 2.

#### Remark {#int-v-s7-n1-rem-2 .statement}

— a) Cor. 3 has already been proved by another method (Ch. IV, \S 5, No. 7, Lemma 3).
    b) By virtue of Cor. 3, the corollaries 1,2,3 of Prop. 1, Prop. 2, Theorem 1 and its corollaries 1,2 extend at once to a complex measure.

#### Scholium {#int-v-s7-n1-sch-1 .statement}

— For every function $f$ (resp. $g$) defined on $X$ (resp. $T$) with values in the Banach space $F$ or in $\overline{\mathbf{R}}$, let us denote by $\zeta(f)$ (resp. $\rho(g)$) the extension by 0 of $f$ to $T$ (resp. the restriction of $g$ to $X$). Then $\zeta(\rho(g)) = \varphi_X \cdot g$, $\rho(\zeta(f)) = f$. We denote by $\mu'$ the measure $\varphi_X \cdot \mu$ on $T$. For every $p \in [1, +\infty]$, Props. 1 and 2 imply that $\zeta$ maps $\mathcal{L}_F^p(X, \mu_X)$ into $\mathcal{L}_F^p(T, \mu')$, and that $\rho$ maps $\mathcal{L}_F^p(T, \mu')$ onto $\mathcal{L}_F^p(X, \mu_X)$, with preservation of norm in both cases, as well as of the integral when $p = 1$ (Th. 1); passing to the associated Hausdorff spaces, we obtain two isomorphisms inverse to each other. Similarly, if $\zeta$ and $\rho$ are applied to positive numerical functions, the essential upper integral is preserved (Prop. 1). Thus, if we agree to *identify* a function on $X$ with a function on T that is zero on X − T, and the measure $\mu_X$ with the measure $\mu'$, problems concerning induced measures are reduced to problems concerning measures defined by densities, treated in §5. This sort of reasoning is applicable to complex measures as well, by Cor. 3 of Th. 1.

### 2. Properties of induced measures

#### Proposition 3 {#int-v-s7-prop-3 .statement}

— Let X be a locally compact subspace of T, and $\lambda$ a complex measure on X. The following properties are equivalent:
a) the canonical injection $i : X \to T$ is $\lambda$-proper;
b) for every compact subset K of T, $K \cap X$ is essentially $\lambda$-integrable;
c) every point $t \in T$ admits a neighborhood V such that $V \cap X$ is essentially $\lambda$-integrable;
d) there exists a measure $\theta$ on T such that $\theta_X = \lambda$.
If these equivalent conditions are satisfied, we have, with notations as in d),

$$
(i(\lambda))_X = \lambda \quad \text{and} \quad i(\lambda) = i(\theta_X) = \varphi_X \cdot \theta .
$$

The injection $i$ being continuous, the equivalence of the properties a), b) and c) follows from Prop. 1 of §6, and the remark that follows it, applied to the positive measure $|\lambda|$. If $\lambda$ is induced on X by a measure $\theta$ on T, then $|\lambda| = |\theta|_X$ (formula (6)), consequently $|\lambda|(K \cap X) = |\theta|(K \cap X) \leq |\theta|(K) < +\infty$ (Prop. 1) for every compact subset K of T, so that d) implies b). Suppose that a) is satisfied, and let us show that $(i(\lambda))_X = \lambda$, which will imply d). Let g be an element of $\mathcal{H}(X; \mathbf{C})$; denoting by $g'$ the extension by 0 of g to T we have, by the definition of induced measure and then by Prop. 7 of §6, No. 4,

$$
\int g \, d(i(\lambda))_X = \int g' \, d(i(\lambda)) = \int (g' \circ i) \, d\lambda = \int g \, d\lambda .
$$

This completes the proof of the equivalence of the four properties. If $\lambda = \theta_X$ and $g \in \mathcal{H}(T; \mathbf{C})$, then

$$
\int g \, d(i(\theta_X)) = \int (g \circ i) \, d(\theta_X) = \int g \varphi_X \, d\theta ,
$$

because $g \varphi_X$ is the extension by 0 of $g \circ i$ to T. This proves the second formula of (7).

#### Corollary 1 {#int-v-s7-prop-3-cor-1 .statement}

— If X is closed, then every complex measure $\lambda$ on X is induced by a measure on T.

For, if K is a compact set in T then K ∩ X is compact, hence λ-integrable.

#### Corollary 2 {#int-v-s7-prop-3-cor-2 .statement}

— Let θ be a complex measure on T, π a θ-proper mapping of T into a locally compact space Y, and π_X its restriction to X. Then π_X is θ_X-proper, and π_X(θ_X) = π(φ_X · θ).

For, π_X = π ∘ i, where i is the canonical injection X → T. When θ is positive the corollary may therefore be deduced from Prop. 3 and the transitivity of image measures (§6, No. 3, Prop. 4). The case of a non-positive complex measure then follows by linearity.

#### Proposition 4 {#int-v-s7-prop-4 .statement}

— Let X and Y be two locally compact subspaces of T such that Y ⊂ X. If θ is a complex measure on T, then the measure (θ_X)_Y induced by θ_X on Y is equal to θ_Y ('transitivity of induced measures').

It suffices to observe that if g is an element of $\mathcal{H}(Y; \mathbf{C})$, then the extension by 0 of g to T may be obtained by extending by 0 the extension by 0 of g to X, or again, making use of the identifications of the Scholium, that $φ_Y · θ = φ_Y(φ_X · θ)$ (§5, No. 4, Prop. 8).

#### Proposition 5 {#int-v-s7-prop-5 .statement}

— Let $(\lambda_α)_{α ∈ A}$ be an increasing directed family of positive measures on T, admitting a supremum λ, and let X be a locally compact subspace of T. The family of induced measures $λ_α|X$ is then bounded above in $\mathcal{M}(X)$, and

$$
\sup_{α ∈ A} (λ_α|X) = λ|X.
$$

In view of the identifications in the Scholium, this proposition is a special case of Prop. 5 of §5, No. 4.

#### Corollary {#int-v-s7-n2-cor-1 .statement}

— Let $(\mu_i)_{i ∈ I}$ be a summable family of positive measures on T, with sum μ. The family of induced measures $μ_i|X$ is then summable, and

$$
\sum_{i ∈ I} (μ_i|X) = μ|X.
$$

#### Proposition 6 {#int-v-s7-prop-6 .statement}

— Let $Λ : t ↦ λ_t$ be a μ-adequate mapping of T into $\mathcal{M}_+(X)$, where X is a locally compact space that is countable at infinity, and let Y be a locally compact subspace of X. Set $\int λ_t dμ(t) = ν$. The mapping $t ↦ λ_t|Y$ of T into $\mathcal{M}_+(Y)$ is then μ-adequate, and

$$
\int (λ_t|Y) dμ(t) = ν|Y.
$$

Taking into account the identifications in the Scholium, this proposition is a special case of Prop. 7 of §5, No. 4.

### Exercises {#int-v-s7-exercises}

See the [exercises for § 7](exercises/s7/).
