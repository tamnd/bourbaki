---
book: int
book_title: Integration
chapter: V
chapter_title: INTEGRATION OF MEASURES
section: 5
section_title: Measures defined by numerical densities
lang: en
source: int-i-vi
book_pages: INT V.38-INT V.62, INT V.99-INT V.107
pdf_pages: 0293-0317, 0354-0362
extraction: ocr
subsections:
    - "no": 1
      title: Locally integrable functions
      page: 38
      pdf_page: 293
    - "no": 2
      title: Measures defined by numerical densities
      page: 40
      pdf_page: 295
    - "no": 3
      title: Integration with respect to a measure defined by a density
      page: 42
      pdf_page: 297
    - "no": 4
      title: Behavior of the product with respect to the usual operations
      page: 45
      pdf_page: 300
    - "no": 5
      title: Characterization of measures with base $\mu$
      page: 48
      pdf_page: 303
    - "no": 6
      title: Equivalent measures
      page: 52
      pdf_page: 307
    - "no": 7
      title: Alien measures
      page: 54
      pdf_page: 309
    - "no": 8
      title: 'Applications: I. Duality of the spaces $L^p$'
      page: 56
      pdf_page: 311
    - "no": 9
      title: 'Applications: II. Functions of measures'
      page: 60
      pdf_page: 315
    - "no": 10
      title: Diffuse measures; atomic measures
      page: 61
      pdf_page: 316
statements: 52
exercises: 31
content_sha256: 6a7503ac7070c09ee4ba4dc75d90e625e4265b85f43d14a0cdfa0ac09063fc13
---

## § 5. MEASURES DEFINED BY NUMERICAL DENSITIES

### 1. Locally integrable functions

#### Proposition 1 {#int-v-s5-prop-1 .statement}

*Let g be a function defined locally almost everywhere in T (for the positive measure $\mu$), with values in a Banach space F (resp. in $\overline{\mathbf{R}}$). The following properties are equivalent:*

a) *For every point $t \in T$, there exists a neighborhood V of t such that the function $g \varphi_V$ is $\mu$-integrable.*

b) *The function g is $\mu$-measurable and, for every compact set $K \subset T$, $\int^* |g|\varphi_K\,d\mu < +\infty$.*

c) *For every numerical function $h \in \mathcal{K}(T)$, $gh$ is $\mu$-integrable.*

Let us show that a) implies b); for, the function g is measurable by the principle of localization (Ch. IV, §5, No. 2, Prop. 4). On the other hand, for every $t \in K$ there exists, by hypothesis, a neighborhood $V_t$ of $t$ in $T$ such that $g \varphi_{V_t}$ is integrable; one can therefore cover $K$ by a finite number of neighborhoods $V_i$ ($1 \leq i \leq n$) such that the functions $g \varphi_{V_i}$ are integrable. Since $|g| \varphi_K \leq \sum_{i=1}^n |g| \varphi_{V_i}$, one has $\int^* |g| \varphi_K \, d\mu < +\infty$.

Secondly, b) implies c), because $gh$ is then measurable, and if $L$ is the compact support of $h$ then $|gh| \leq \|h\| \cdot |g| \varphi_L$, therefore $\int^* |gh| \, d\mu < +\infty$ by hypothesis; $gh$ is therefore integrable by the criterion for integrability (Ch. IV, §5, No. 6, Th. 5).

Finally, c) implies a). Indeed, for every $t \in T$ let $V$ be a compact neighborhood of $t$. There exists a continuous mapping $h$ of $T$ into $[0,1]$, equal to 1 on $V$ and with compact support (Ch. III, §1, No. 2, Lemma 1); by hypothesis $gh$ is integrable, therefore so is $g \varphi_V = (gh) \varphi_V$ (Ch. IV, §5, No. 6, Cor. 3 of Th. 5).

#### Definition 1 {#int-v-s5-def-1 .statement}

*A function* $g$, *defined locally almost everywhere in* $T$ (*for the positive measure* $\mu$), *with values in a Banach space* $F$ (*resp. in* $\overline{\mathbf{R}}$), *is said to be locally integrable for* $\mu$ (*or locally* $\mu$*-integrable*) *if it satisfies the conditions* a), b), c) *of Prop. 1.* *If* $\theta$ *is a complex measure, a function* $g$ *defined locally* $\theta$*-almost everywhere is said to be locally* $\theta$*-integrable if it is locally integrable for the positive measure* $|\theta|$.

If $g$ is locally $\theta$-integrable, then every function equal to $g$ locally almost everywhere is locally integrable. It is clear that the sum of two locally integrable functions is locally integrable. The functions with values in $F$, *everywhere defined* and locally integrable for $\theta$, form a vector space denoted $\mathcal{L}_{loc}^1(T, \theta; F)$; when $F = \mathbf{R}$ or $\mathbf{C}$, the mention of $F$ is often omitted if there is no ambiguity. This space will always be equipped (absent express mention to the contrary) with the topology defined by the semi-norms $g \mapsto \int |g \varphi_K| \, d|\theta|$, where $K$ runs over the set of compact subsets of $T$. The associated Hausdorff space, the quotient of $\mathcal{L}_{loc}^1(T, \theta; F)$ by the subspace $\mathcal{N}_F^\infty$ of mappings that are zero locally almost everywhere, is denoted $L_{loc}^1(T, \theta; F)$. The spaces $L_{loc}^1(T, \theta; F)$ and $L_{loc}^1(T, |\theta|; F)$ are identical.

It can be shown that the topological vector spaces just defined are *complete* (Exer. 31).

Every measurable function $g$, that is essentially bounded on every compact set, is locally integrable. For every number $p$ such that $1 \leq p \leq +\infty$, every function $g \in \mathcal{L}_F^p$ is locally integrable; indeed, for every function $h \in \mathcal{H}(T)$, $h$ belongs to $\mathcal{L}^q$ (where $q$ is the exponent conjugate to $p$), therefore $gh$ is integrable (Ch. IV, §6, No. 4, Cor. 4 of Th. 2).

Let $F, G, H$ be three Banach spaces, and $(u, v) \mapsto \Phi(u, v)$ a continuous bilinear mapping of $F \times G$ into $H$. If $f$ is locally integrable and takes its values in F, and if $g \in \mathcal{L}_G^\infty$, then $\Phi(f, g)$ is locally integrable (Ch. IV, §6, No. 4, Cor. 1 of Th. 2).

### 2. Measures defined by numerical densities

Let $g$ be a positive numerical function defined locally $\mu$-almost everywhere in T and locally $\mu$-integrable; the set of $t$ such that $g(t) = +\infty$ is then locally $\mu$-negligible, because $g \varphi_K$ is $\mu$-integrable for every compact set K (Ch. IV, §2, No. 3, Prop. 7). Now let $g'$ be a locally integrable function that is positive and finite, equal to $g$ locally $\mu$-almost everywhere; set $\lambda'_t = g'(t) \varepsilon_t$. The mapping $t \mapsto \lambda'_t$ of T into $\mathcal{M}_+(T)$ is vaguely $\mu$-measurable and scalarly essentially integrable (or again, the pair $(I, g')$, where I is the identity mapping of T, is $\mu$-adapted); the integral $\nu = \int \lambda'_t d\mu(t)$ does not depend on the particular function $g'$, locally almost everywhere equal to $g$, used in the definition of the measures $\lambda'_t$. This measure $\nu$ is determined by the condition

$$
\int f(t)\,d\nu(t) = \int f(t)g(t)\,d\mu(t) \quad \text{for } f \in \mathcal{K}(T).
$$

If now $\theta$ is a complex measure, and if $u$ is a complex function (or a function with values in $\overline{\mathbf{R}}$) defined locally $\theta$-almost everywhere and locally integrable for $\theta$, one can write

$$
\begin{align*}
u &= g_1 - g_2 + i(g_3 - g_4) \\
\theta &= \mu_1 - \mu_2 + i(\mu_3 - \mu_4)
\end{align*}
$$

where $\mu_1 = (\Re \theta)^+$, $\mu_2 = (\Re \theta)^-$, $\mu_3 = (\Im \theta)^+$, $\mu_4 = (\Im \theta)^-$ (Ch. III, §1, No. 5), and where $g_1, g_2, g_3, g_4$ have the analogous meanings; since $|u|$ is locally $|\theta|$-integrable, each of the positive functions $g_i$ ($i = 1, 2, 3, 4$) is locally integrable for each positive measure $\mu_j$ ($j = 1, 2, 3, 4$), so that the mapping

$$
f \mapsto \int f(t)u(t)\,d\theta(t)
$$

on $\mathcal{K}(T)$ is a complex measure.

#### Definition 2 {#int-v-s5-def-2 .statement}

*Let $\theta$ be a complex measure, and let $u$ be a complex function (or a function with values in $\overline{\mathbf{R}}$) defined locally $\theta$-almost everywhere and locally $\theta$-integrable. The complex measure $f \mapsto \int fu\,d\theta$ on T is said to be the product of the measure $\theta$ by the function $u$, or the measure with density $u$ with respect to $\theta$, and is denoted $u \cdot \theta$.*

Every complex measure that is the product of a positive measure $\mu$ by a locally $\mu$-integrable function is called a measure with base $\mu$.

The relation $\eta = u \cdot \theta$ is again, by convention, written

$$
d\eta(t) = u(t)\, d\theta(t).
$$

When $u$ is everywhere defined and continuous, one recovers the definition given in Ch. III, §1, No. 4. It is clear that if $u_1$ and $u_2$ are locally $\theta$-integrable, then $(u_1 + u_2) \cdot \theta = u_1 \cdot \theta + u_2 \cdot \theta$. Similarly, if $\theta_1$ and $\theta_2$ are two measures on $T$, and if $u$ is a function locally integrable for $\theta_1$ and $\theta_2$, then $u$ is locally integrable for $\theta_1 + \theta_2$ and one has $u \cdot (\theta_1 + \theta_2) = u \cdot \theta_1 + u \cdot \theta_2$.

We shall henceforth restrict ourselves to the case of functions defined everywhere; the extension to functions defined locally almost everywhere, which is always obvious, is left to the reader.

The following proposition permits, for the most part, reducing the case of complex measures to that of positive measures:

#### Proposition 2 {#int-v-s5-prop-2 .statement}

*Let $\theta$ be a complex measure, and $u$ a locally $\theta$-integrable complex function; then*

$$
|u \cdot \theta| = |u| \cdot |\theta|.
$$

We begin with an auxiliary result:

#### Lemma 1 {#int-v-s5-lem-1 .statement}

— *Let $\theta$ be a complex measure, and let $f$ be an element of $\overline{\mathcal{L}}^1_C(T, \theta)$. Then*

$$
\langle|\theta|, |f|\rangle = \sup_{c \in \mathcal{K}_1} |\langle\theta, cf\rangle| = \sup_{c \in \mathcal{B}_1} |\langle\theta, cf\rangle|,
$$

*where $\mathcal{K}_1$ (resp. $\mathcal{B}_1$) denotes the set of complex functions $c$, continuous with compact support (resp. Borel), such that $|c| \leq 1$.

Let us first treat the case that $f \in \mathcal{K}(T; \mathbf{C})$. Obviously

$$
\sup_{c \in \mathcal{K}_1} |\langle\theta, cf\rangle| \leq \sup_{c \in \mathcal{B}_1} |\langle\theta, cf\rangle| \leq \langle|\theta|, |f|\rangle
$$

(Ch. IV, §4, No. 2, Prop. 2). On the other hand, let $g$ be an element of $\mathcal{K}(T; \mathbf{C})$ such that $|g| \leq |f|$; $g$ is the uniform limit of a sequence $(g_n)$ of elements of $\mathcal{K}(T; \mathbf{C})$ whose supports are contained in the open set $U$ formed by the $t$ such that $f(t) \neq 0$, and one may clearly suppose that $|g_n| \leq |f|$ for every $n$. Set $c_n(t) = g_n(t)/f(t)$ for $t \in U$, $c_n(t) = 0$ for $t \notin U$; then $c_n \in \mathcal{K}_1$, $g = \lim_{n \to \infty} c_n f$, therefore $|\langle\theta, g\rangle| = \lim_{n \to \infty} |\langle\theta, c_n f\rangle|$, and finally

$$
\sup_{|g| \leq |f|, g \in \mathcal{K}(T; \mathbf{C})} |\langle\theta, g\rangle| \leq \sup_{c \in \mathcal{K}_1} |\langle\theta, cf\rangle|.
$$

One concludes by observing that the first member of this inequality is equal to $\langle |\theta|, |f| \rangle$ (Ch. III, §1, No. 6, formula (12)).

Next, denote by $f$ an element of $\overline{\mathcal{L}}_C^1(\theta)$, and let us show that (4) is again true: it suffices to verify that the three members of this relation depend continuously on $f$ for the topology of $\overline{\mathcal{L}}_C^1(\theta)$, since they coincide on the dense subspace $\mathcal{K}(T; \mathbf{C})$. This results at once from the following inequalities, where $f$ and $f'$ denote elements of $\overline{\mathcal{L}}_C^1(\theta)$:

$$
|\langle |\theta|, |f| \rangle - \langle |\theta|, |f'| \rangle| \leq \langle |\theta|, |f - f'| \rangle = \overline{N}_1(f - f')
$$
$$
|\langle \theta, cf \rangle - \langle \theta, cf' \rangle| \leq \langle |\theta|, |c||f - f'| \rangle \leq \overline{N}_1(f - f')
$$

for all $c \in \mathcal{B}_1$. The lemma is thus established.

Passing to the proof of Proposition 2, let us apply the lemma to the function $uh$, where $h$ belongs to $\mathcal{K}_+(T)$. This yields:

$$
\langle |\theta|, |uh| \rangle = \sup_{c \in \mathcal{K}_1} |\langle \theta, cuh \rangle| = \sup_{c \in \mathcal{K}_1} |\langle u \cdot \theta, ch \rangle| = \langle |u \cdot \theta|, h \rangle .
$$

However, the first member is also equal to

$$
\langle |\theta|, |u|h \rangle = \langle |u| \cdot |\theta|, h \rangle .
$$

The two measures $|u| \cdot |\theta|$ and $|u \cdot \theta|$ are therefore equal.

#### Corollary {#int-v-s5-n2-cor-1 .statement}

*Let $g_1$ and $g_2$ be two locally $\mu$-integrable numerical functions; then*

$$
\inf(g_1 \cdot \mu, g_2 \cdot \mu) = \inf(g_1, g_2) \cdot \mu ; \quad \sup(g_1 \cdot \mu, g_2 \cdot \mu) = \sup(g_1, g_2) \cdot \mu .
$$

*In particular, if $g$ is a locally $\mu$-integrable numerical function, then*

$$
(g \cdot \mu)^+ = g^+ \cdot \mu ; \quad (g \cdot \mu)^- = g^- \cdot \mu .
$$

This follows at once from Prop. 2 and the formulas (6) of Ch. II, §1, No. 1.

### 3. Integration with respect to a measure defined by a density

*In the statements of this subsection, $g$ denotes a positive numerical function, defined everywhere and locally $\mu$-integrable, $\theta$ denotes a complex measure, and $u$ a locally $\theta$-integrable complex function.*

The remarks in No. 2 show that the results of §4 are applicable to the measure $\nu = g \cdot \mu = \int g(t) \varepsilon_t \, d\mu(t)$ (even though the measure $g(t) \varepsilon_t$ is not defined unless $g(t) \neq +\infty$). We thus obtain the following statement:

#### Proposition 3 {#int-v-s5-prop-3 .statement}

*For every numerical function $f \geqslant 0$ defined on $T$,*

$$
\int^\bullet f \, d\nu = \int^\bullet (f g) \, d\mu .
$$

This follows from Th. 1 of §4, No. 2.

#### Corollary 1 {#int-v-s5-prop-3-cor-1 .statement}

*In order that a function $\mathbf{f}$, with values in a Banach space or in $\overline{\mathbf{R}}$, be locally negligible for the measure $u \cdot \theta$, it is necessary and sufficient that $u \mathbf{f}$ be locally negligible for $\theta$.*

To say that $\mathbf{f}$ (resp. $u \mathbf{f}$) is locally negligible for $u \cdot \theta$ (resp. for $\theta$) is equivalent to saying that $|\mathbf{f}|$ (resp. $|u| \cdot |\mathbf{f}|$) is locally negligible for $|u \cdot \theta|$ (resp. for $|\theta|$). We are thus reduced, in view of Prop. 2 of No. 2, to the case that $\mathbf{f}, u, \theta$ are positive; the statement then follows at once from Prop. 3.

#### Corollary 2 {#int-v-s5-prop-3-cor-2 .statement}

*Let $u_1$ and $u_2$ be two locally $\theta$-integrable complex functions. In order that $u_1 \cdot \theta = u_2 \cdot \theta$, it is necessary and sufficient that $u_1$ and $u_2$ be equal locally almost everywhere.*

One is immediately reduced to showing that $u \cdot \theta = 0$ implies that $u(t) = 0$ locally almost everywhere; but $u \cdot \theta = 0$ means that the function 1 is locally negligible for the measure $u \cdot \theta$. One then applies Corollary 1.

#### Corollary 3 {#int-v-s5-prop-3-cor-3 .statement}

*Let $u$ be a complex function that is locally integrable for the positive measure $\mu$. For $u \cdot \mu$ to be a positive measure, it is necessary and sufficient that $u(t) \geqslant 0$ locally almost everywhere.*

For, $u \cdot \mu$ is positive if and only if $u \cdot \mu = |u \cdot \mu| = |u| \cdot \mu$ (Prop. 2), and this is equivalent to $u = |u|$ locally almost everywhere (Cor. 2).

#### Proposition 4 {#int-v-s5-prop-4 .statement}

*For a mapping $f$ of $T$ into a topological space $G$ to be measurable for the measure $u \cdot \theta$, it is necessary and sufficient that the restriction of $f$, to the $\theta$-measurable set $S$ of the $t$ such that $u(t) \neq 0$, be $\theta$-measurable.*

When $u$ and $\theta$ are positive, this follows at once from Prop. 3 of §4, No. 3. The result then extends to the case that $u$ and $\theta$ are complex thanks to Prop. 2.

#### Corollary {#int-v-s5-n3-cor-1 .statement}

*Let $\mathbf{f}$ be a function defined on $T$, with values in a Banach space $F$ or in $\overline{\mathbf{R}}$. For $\mathbf{f}$ to be $(u \cdot \theta)$-measurable, it is necessary and sufficient that $u \mathbf{f}$ be $\theta$-measurable.*

For, $u \mathbf{f}$ is the extension by 0 of $(u \mathbf{f})|S$ to $T$.

#### Theorem 1 {#int-v-s5-thm-1 .statement}

*Let $\mathbf{f}$ be a function defined on $T$, with values in a Banach space $F$ or in $\overline{\mathbf{R}}$. In order that $\mathbf{f}$ be essentially integrable for* the measure $\eta = u \cdot \theta$, it is necessary and sufficient that $uf$ be essentially $\theta$-integrable, in which case

$$
\int f \, d\eta = \int (uf) \, d\theta .
$$

Suppose moreover that $u$ is continuous and that $u(t) \neq 0$ for all $t \in T$; then $f$ is integrable for the measure $\eta$ if and only if $uf$ is integrable for $\theta$.

The case that $u$ and $\theta$ are positive follows at once from Th. 2 of §4, No. 4. The first and the last assertion of the statement then follow immediately, because $f$ is essentially integrable (resp. integrable) with respect to $\eta = u \cdot \theta$ if and only if it is essentially integrable (resp. integrable) for $|\eta| = |u| \cdot |\theta|$. Finally, suppose that $f$ is essentially integrable for $\eta$ (hence for $|\eta|$); we make use of the decomposition (2): $f$ is essentially integrable for each of the measures $\eta_{ij} = g_i \cdot \mu_j$ ($i = 1, 2, 3, 4,\ j = 1, 2, 3, 4$), because these measures are $\leq |\eta|$. We have

$$
\int f \, d\eta_{ij} = \int g_i f \, d\mu_j .
$$

The formula (6) follows immediately from this.

#### Corollary {#int-v-s5-n3-cor-2 .statement}

For the measure $u \cdot \theta$ to be bounded, it is necessary and sufficient that $u$ be essentially $\theta$-integrable.

#### Example {#int-v-s5-n3-exa-1 .statement}

Let $A$ be a subset of $T$; for $\varphi_A$ to be locally $\mu$-integrable, it is necessary and sufficient that $A$ be $\mu$-measurable. Assuming the condition to be fulfilled, set $\nu = \varphi_A \cdot \mu$; for every numerical function $f \geq 0$ defined on $T$, we then have

$$
\int^\bullet f \, d\nu = \int^\bullet f \varphi_A \, d\mu ,
$$

a quantity that is also denoted by $\int_A^\bullet f \, d\mu$ (cf. Ch. IV, §5, No. 6). For a mapping $g$ of $T$ into a topological space $G$ to be $\nu$-measurable, it is necessary and sufficient that the restriction of $g$ to $A$ be $\mu$-measurable. For a mapping $f$ of $T$ into a Banach space $F$ or into $\overline{\mathbf{R}}$ to be essentially $\nu$-integrable, it is necessary and sufficient that $f \varphi_A$ be essentially $\mu$-integrable, in which case

$$
\int f \, d\nu = \int f \varphi_A \, d\mu ,
$$

an expression that is also denoted $\int_A f \, d\mu$. Note that if two mappings of $T$ into $G$ (resp. $F, \overline{\mathbf{R}}$) coincide on $A$, then for one of them to be $\nu$-measurable (resp. essentially $\nu$-integrable), it is necessary and sufficient that the other be so. If now $g$ is a mapping into $G$ of an arbitrary subset $B \supset A$ of $T$, one says that $g$ is $\mu$-measurable *on* $A$ if an arbitrary extension to $T$ of the restriction of $g$ to $A$ is $\nu$-measurable, which amounts to saying that the restriction of $g$ to $A$ is $\mu$-measurable. A mapping $f$ of $B$ into a Banach space $F$, or into $\overline{\mathbf{R}}$, is said to be *essentially* $\mu$-integrable *on* $A$ if some extension $\overline{f}$ to $T$ of the restriction of $f$ to $A$ is essentially $\nu$-integrable; one then sets
$$
\int_A f \, d\mu = \int_A \overline{f} \, d\mu = \int \overline{f} \varphi_A \, d\mu,
$$
and one says that $\int_A f \, d\mu$ is the *integral of* $f$ *on* $A$ (or *extended to* $A$). If $f$ is a numerical function $\geqslant 0$ defined on $B \supset A$, one defines similarly $\int_A^* f \, d\mu$ and $\int_A^\bullet f \, d\mu$. Finally, a numerical function $g$ defined on $B \supset A$ is said to be *locally* $\mu$-integrable *on* $A$ if some extension $\overline{g}$ to $T$ of the restriction of $g$ to $A$ is locally $\nu$-integrable: this is equivalent to saying that, for every compact subset $K$ of $T$, $\overline{g} \varphi_{K \cap A}$ is $\mu$-integrable.

### 4. Behavior of the product with respect to the usual operations

#### Proposition 5 {#int-v-s5-prop-5 .statement}

*Let* $(\lambda_\alpha)_{\alpha \in A}$ *be a family of positive measures on* $T$, *directed for the relation* $\leqslant$, *admitting in* $\mathcal{M}(T)$ *a supremum* $\lambda$. *For a positive numerical function* $g$ *to be locally* $\lambda$-*integrable, it is necessary and sufficient that* $g$ *be locally* $\lambda_\alpha$-*integrable for every* $\alpha \in A$ *and that the family* $(g \cdot \lambda_\alpha)$ *be bounded above in* $\mathcal{M}(T)$; *in this case,
$$
g \cdot \lambda = \sup_{\alpha \in A} g \cdot \lambda_\alpha.
$$
It is clear that the condition is necessary. Conversely, suppose that $g$ is locally integrable for each of the measures $\lambda_\alpha$ and that the family $(g \cdot \lambda_\alpha)_{\alpha \in A}$ is bounded above; denote its supremum by $\lambda'$. The function $g$ is then $\lambda$-measurable (\S 1, No. 4, Cor. 2 of Prop. 11); moreover, for every function $h \in \mathcal{K}_+(T)$,
$$
\int^\bullet (hg) \, d\lambda = \sup_{\alpha \in A} \int^\bullet (hg) \, d\lambda_\alpha = \sup_{\alpha \in A} \int^\bullet h \, d(g \cdot \lambda_\alpha) = \int^\bullet h \, d\lambda'
$$
(\S 1, No. 4, Prop. 11). This implies first of all that the first member is finite for any $h$, so that $g$ is locally $\lambda$-integrable; the symbol $\int^\bullet$ may therefore be replaced by $\int$, and the formula may be written $\int h \, d(g \cdot \lambda) = \int h \, d\lambda'$. It follows that $g \cdot \lambda = \lambda'$, and this completes the proof.

#### Corollary {#int-v-s5-n4-cor-1 .statement}

— Suppose that $\mu$ is the sum of a family $(\mu_\alpha)_{\alpha \in A}$ of measures on T. For a positive numerical function g defined on T to be locally $\mu$-integrable, it is necessary and sufficient that g be locally $\mu_\alpha$-integrable for every $\alpha \in A$ and that the family $(g \cdot \mu_\alpha)_{\alpha \in A}$ be summable. In this case,

$$
g \cdot \mu = \sum_{\alpha \in A} g \cdot \mu_\alpha.
$$

Let $(g_\alpha)_{\alpha \in A}$ be a family of $\mu$-measurable positive functions defined on T. Let $S_\alpha$ be the set of $t \in T$ such that $g_\alpha(t) \neq 0$. We shall say that the family $(g_\alpha)$ is *locally countable* if the family $(S_\alpha)$ is locally countable (Ch. IV, §5, No. 9); this amounts to saying that, for every compact set K in T, the set of $\alpha \in A$ such that $g_\alpha|K$ is not zero is countable.

#### Proposition 6 {#int-v-s5-prop-6 .statement}

— Let $(g_\alpha)_{\alpha \in A}$ be a locally countable family of locally $\mu$-integrable positive numerical functions defined on T. In order that the function $g = \sum_{\alpha \in A} g_\alpha$ be locally $\mu$-integrable, it is necessary and sufficient that the family of measures $(g_\alpha \cdot \mu)_{\alpha \in A}$ be summable, in which case

$$
g \cdot \mu = \sum_{\alpha \in A} g_\alpha \cdot \mu.
$$

It is clear that $g$ is $\mu$-measurable (Ch. IV, §5, No. 2, Prop. 4 and No. 4, Cor. 1 of Th. 2). For $g$ to be locally $\mu$-integrable, it is therefore necessary and sufficient that $\mu^\bullet(gf)$ be finite for every $f \in \mathcal{H}_+(T)$. Now, since the set of $\alpha \in A$ such that $g_\alpha f \neq 0$ is countable, we have $\mu^\bullet(gf) = \sum_{\alpha \in A} \mu^\bullet(g_\alpha f)$ (§1, No. 1, Cor. of Prop. 2). Set $\nu_\alpha = g_\alpha \cdot \mu$; the condition $\mu^\bullet(gf) < +\infty$ is equivalent to the condition $\sum_{\alpha \in A} \nu_\alpha(f) < +\infty$: in other words, $g$ is locally $\mu$-integrable if and only if the family $(\nu_\alpha)$ is summable. Denoting the sum of this family by $\nu$, the preceding calculation yields the equality $\nu(f) = \mu^\bullet(gf)$, which is equivalent to (8).

#### Corollary {#int-v-s5-n4-cor-2 .statement}

— Let $(g_\alpha)$ be a sequence of locally $\mu$-integrable numerical functions, such that the sequence of measures $g_n \cdot \mu$ is increasing. In order that this sequence have an upper bound in the ordered vector space $\mathcal{M}(T)$ of real measures on T, it is necessary and sufficient that the function $g = \sup g_n$ be locally $\mu$-integrable; the supremum in $\mathcal{M}(T)$ of the sequence $(g_n \cdot \mu)$ is then the measure $g \cdot \mu$.

It suffices to apply Prop. 6 to the functions (positive locally almost everywhere) $g'_n = g_{n+1} - g_n$.

#### Proposition 7 {#int-v-s5-prop-7 .statement}

— Let X be a locally compact space that is countable at infinity, and let $t \mapsto \lambda_t$ be a $\mu$-adequate mapping of T into $\mathcal{M}_+(X)$.

Let $g$ be a positive numerical function defined on $X$, locally integrable for the measure $\nu = \int \lambda_t d\mu(t)$. The set of $t \in T$ such that $g$ is not locally $\lambda_t$-integrable is then locally negligible for $\mu$, the mapping $t \mapsto g \cdot \lambda_t$ (defined locally $\mu$-almost everywhere) is $\mu$-adequate, and

$$
g \cdot \nu = \int (g \cdot \lambda_t) d\mu(t).
$$

Let $(K_n)_{n \in \mathbf{N}}$ be an increasing sequence of compact subsets of $X$ whose interiors cover $X$; if $\eta$ is any positive measure on $X$, to say that $g$ is locally $\eta$-integrable is equivalent to saying that $g \varphi_{K_n}$ is $\eta$-integrable for every $n$. Now let $H_n$ be the set of $t \in T$ such that $g \varphi_{K_n}$ is not $\lambda_t$-integrable, and let $H = \bigcup_n H_n$; since $H_n$ is locally $\mu$-negligible for all $n$ (\S 3, No. 3, Th. 1), the same is true of $H$, which establishes the first assertion of the statement. Replacing $\lambda_t$ by 0 for $t$ in $H$ (which does not change the measure $\nu$), we can suppose that $g$ is locally $\lambda_t$-integrable for every $t \in T$. For every $\nu$-measurable positive function $h$ defined on $X$, we have, by Prop. 3 and by Prop. 5 of \S 3, No. 2,

$$
\int^\bullet h d(g \cdot \nu) = \int^\bullet (gh) d\nu = \int^\bullet d\mu(t) \int^\bullet (gh) d\lambda_t = \int^\bullet d\mu(t) \int^\bullet h d(g \cdot \lambda_t).
$$

This formula and Prop. 5 of \S 3, No. 2 first show (on taking $h \in \mathcal{K}_+(X)$) that the mapping $t \mapsto g \cdot \lambda_t$ is scalarly essentially $\mu$-integrable, and that its integral is $g \cdot \nu$; in other words, the relation (9) holds. Next, let us replace $\mu$ by a positive measure $\mu' \leq \mu$, and let us take for $h$ a positive lower semi-continuous function: it follows at once from these relations that $t \mapsto g \cdot \lambda_t$ is $\mu$-adequate (\S 3, No. 1, Def. 1).

#### Proposition 8 {#int-v-s5-prop-8 .statement}

*Let $\theta$ be a complex measure on $T$, $g_1$ a locally $\theta$-integrable complex function, $\theta_1$ the measure $g_1 \cdot \theta$. For a complex function $g_2$ defined on $T$ to be locally $\theta_1$-integrable, it is necessary and sufficient that $g_2 g_1$ be locally $\theta$-integrable, in which case*

$$
g_2 \cdot \theta_1 = g_2 \cdot (g_1 \cdot \theta) = (g_2 g_1) \cdot \theta
$$
('associativity formula').

By the corollary of Prop. 4, to say that $g_2$ is $\theta_1$-measurable is equivalent to saying that $g_2 g_1$ is $\theta$-measurable. Let us suppose this condition to be satisfied. For every function $f \in \mathcal{K}_+(T)$ we have, by Propositions 2 and 3,

$$
\int^\bullet |g_2| f d|\theta_1| = \int^\bullet |g_2| f |g_1| d|\theta| = \int^\bullet |g_2 g_1| f d|\theta|.
$$

To say that $g_2$ is locally $\theta_1$-integrable is therefore equivalent to saying that $g_2 g_1$ is locally $\theta$-integrable. Assuming this condition to be satisfied, by Th. 1 we have

$$
\int f \, d(g_2 \cdot \theta_1) = \int f g_2 \, d\theta_1 = \int f g_2 g_1 \, d\theta = \int f \, d(g_2 g_1 \cdot \theta),
$$

a formula equivalent to (10).

### 5. Characterization of measures with base $\mu$

#### Theorem 2 (Lebesgue–Nikodym) {#int-v-s5-thm-2 .statement}

— *Let $\mu$ and $\nu$ be two positive measures on $T$. The following properties are equivalent:*

1) $\nu$ *is a measure with base $\mu$*.
2) *Every locally $\mu$-negligible set is locally $\nu$-negligible*.
3) *Every $\mu$-negligible compact set is $\nu$-negligible*.

It is clear that 1) implies 2) (Cor. 1 of Prop. 3), and that 2) implies 3). We are going to show that 3) implies 1). We first note that if the condition 3) is satisfied, then every set $A$ that is *universally measurable* and locally $\mu$-negligible is locally $\nu$-negligible; for, $\nu^\bullet(A) = \sup \nu(K)$, where $K$ runs over the set of compact sets contained in $A$ (\S 1, No. 3, Prop. 10, a) and Ch. IV, \S 4, No. 6, Cor. 2 of Th. 4). Next, we shall establish two lemmas.

#### Lemma 2 {#int-v-s5-lem-2 .statement}

— *Let $\alpha$ be a bounded positive measure on $T$, and $\beta$ a real measure on $T$ such that $|\beta| \leq M \alpha$, where $M$ is a positive constant. Then, there exists a real function $u$, $\alpha$-integrable, such that $\beta = u \cdot \alpha$*.

Let $g$ be an element of the space $\mathcal{L}_\mathbf{R}^2(T, \alpha)$; $g$ is $\beta$-measurable and $\int^\bullet |g|^2 \, d|\beta| \leq M \int^\bullet |g|^2 \, d\alpha < +\infty$. The function $g$ therefore belongs to $\mathcal{L}^2(T, |\beta|)$, and also to $\mathcal{L}^1(T, |\beta|)$ since $\beta$ is bounded. By the Cauchy–Schwarz inequality,

$$
|\beta(g)|^2 \leq \left( \int |g| \, d|\beta| \right)^2 \leq \left( \int d|\beta| \right) \left( \int |g|^2 \, d|\beta| \right) \leq M^2 \alpha(1) \, \alpha(|g|^2).
$$

The mapping $g \mapsto \beta(g)$ is thus a continuous linear form on $\mathcal{L}^2(T, \alpha)$. The Hausdorff space associated with $\mathcal{L}^2(T, \alpha)$ being a Hilbert space, there then exists (TVS, Ch. V, \S 1, No. 7, Th. 3) a real function $u \in \mathcal{L}^2(T, \alpha)$, therefore also belonging to $\mathcal{L}^1(T, \alpha)$, such that $\beta(g) = \alpha(ug)$ for every $g \in \mathcal{L}^2(T, \alpha)$. Applying this relation for $g \in \mathcal{K}(T)$, one sees that $\beta = u \cdot \alpha$.

#### Lemma 3 {#int-v-s5-lem-3 .statement}

— *Suppose that the positive measure $\nu$ is such that every $\mu$-negligible compact set is $\nu$-negligible. Let $\mathfrak{K}$ be the set of compact subsets $K$ of $T$ having the following property:*

(11) There exists a constant $M \geq 0$ such that $\varphi_K \cdot \nu \leq M \varphi_K \cdot \mu$.
The set $\mathcal{K}$ is then $\mu$-dense in $T$.

If $K$ satisfies (11), and if $A$ is a Borel set contained in $K$, it follows at once from Prop. 8 that $\varphi_A \cdot \nu \leq M \varphi_A \cdot \mu$; from this, one deduces that the union of two elements $K, K'$ of $\mathcal{K}$ belongs to $\mathcal{K}$ because $\varphi_{K \cup K'} = \varphi_K + \varphi_A$, where $A = K' \cap \complement K$. To establish the lemma, it remains to prove that every compact set $L$ such that $\mu(L) > 0$ contains a compact set $K \in \mathcal{K}$ such that $\mu(K) > 0$ (Ch. IV, §5, No. 8, Prop. 12). Choose a number $M > \nu(L)/\mu(L)$ and apply Lemma 1 to the bounded positive measure $\alpha = \varphi_L \cdot (\nu + M \mu)$ and the measure $\beta = \varphi_L \cdot (\nu - M \mu)$. Replacing if necessary the function $u$ such that $\beta = u \cdot \alpha$ by a function equal to it $\alpha$-almost everywhere, one can suppose that $u$ is universally measurable (§3, No. 4, Prop. 7) and is zero outside of $L$. The set $H$ of $t \in T$ such that $u(t) < 0$, which is contained in $L$, could not be $\mu$-negligible, for it would then be $\nu$-negligible (by the remark made at the beginning of the proof of Th. 2), hence $\alpha$-negligible, and one would have $\beta(L) > 0$, which contradicts the choice of $M$. Let $K$ be a compact set contained in $H$, such that $\mu(K) > 0$; let us show that $K \in \mathcal{K}$, which will establish the lemma. By Prop. 8,

$$
\varphi_K \cdot (\nu - M \mu) = \varphi_K \cdot \beta = \varphi_K \cdot (u \cdot \alpha) = (\varphi_K u) \cdot \alpha .
$$

The function $\varphi_K u$ is negative, therefore we indeed have $\varphi_K \cdot \nu \leq M \varphi_K \cdot \mu$.

Let us now complete the proof of Theorem 2. Assume that the condition 3) is verified and define $\mathcal{K}$ as in Lemma 3. Let $(K_\alpha)_{\alpha \in A}$ be a locally countable family of pairwise disjoint elements of $\mathcal{K}$, such that the set $N = T - \bigcup_{\alpha \in A} K_\alpha$ is locally $\mu$-negligible (Ch. IV, §5, No. 9, Prop. 14); the family $(K_\alpha)$ being locally countable, $N$ is universally measurable and therefore locally $\nu$-negligible. Set $\mu_\alpha = \varphi_{K_\alpha} \cdot \mu$, $\nu_\alpha = \varphi_{K_\alpha} \cdot \nu$; since the functions $\varphi_{K_\alpha}$ form a locally countable family, whose sum is equal to 1 locally almost everywhere for $\mu$ and for $\nu$, Proposition 6 implies that $\mu = \sum_{\alpha \in A} \mu_\alpha$, $\nu = \sum_{\alpha \in A} \nu_\alpha$. On the other hand, by the definition of $\mathcal{K}$, there exists for every $\alpha$ a constant $M_\alpha$ such that $\nu_\alpha \leq M_\alpha \mu_\alpha$; Lemma 2 therefore implies the existence of a function $g_\alpha$, which one can suppose to be zero outside of $K_\alpha$ and positive (Cor. 3 of Prop. 3), such that $\nu_\alpha = g_\alpha \cdot \mu_\alpha$. Therefore (No. 4, Prop. 8)

$$
\nu_\alpha = g_\alpha \cdot \mu_\alpha = g_\alpha \cdot (\varphi_{K_\alpha} \cdot \mu) = (g_\alpha \varphi_{K_\alpha}) \cdot \mu = g_\alpha \cdot \mu .
$$

Set $g = \sum_{\alpha \in A} g_\alpha$; since the family $(g_\alpha)$ is locally countable and the family $(\nu_\alpha)$ is summable, Proposition 6 implies that $g$ is locally $\mu$-integrable, and that $\nu = g \cdot \mu$, which establishes the theorem.

#### Corollary 1 {#int-v-s5-thm-2-cor-1 .statement}

— Let $\mathcal{N}$ be a set of positive measures with base $\mu$, admitting a supremum $\nu$ in $\mathcal{M}(T)$; then $\nu$ is a measure with base $\mu$.

The Cor. of Prop. 2 permits reduction to the case that $\mathcal{N}$ is an increasing directed set. For every locally $\mu$-negligible set $A$ one then has, by Prop. 11 of §1, No. 4,

$$
\nu^\bullet(A) = \sup_{\lambda \in \mathcal{N}} \lambda^\bullet(A) = 0.
$$

Theorem 2 therefore implies that $\nu$ is a measure with base $\mu$.

#### Corollary 2 {#int-v-s5-thm-2-cor-2 .statement}

— Let $\nu$ be a real measure on $T$. In order that $\nu$ belong to the band generated by $\mu$ in the fully lattice-ordered space $\mathcal{M}(T)$ (Ch. II, §1, No. 5), it is necessary and sufficient that $\nu$ be a measure with base $\mu$.

On considering $\nu^+$ and $\nu^-$, one is immediately reduced to the case of a positive measure $\nu$ (No. 2, Cor. of Prop. 2). Let us then set $\nu_n = \inf(n\mu, \nu)$; $\nu$ belongs to the band generated by $\mu$ if and only if $\nu = \sup_n \nu_n$ (Ch. II, §1, No. 5, Cor. of Prop. 6). Now $\nu_n$, being bounded above by $n\mu$, is a measure with base $\mu$ by Th. 2; the relation $\nu = \sup_n \nu_n$ therefore implies that $\nu$ is a measure with base $\mu$ (Cor. 1). Conversely, suppose that $\nu$ is a measure with base $\mu$: $\nu = g \cdot \mu$, where $g$ is locally $\mu$-integrable and positive. Then $\nu_n = \inf(g, n) \cdot \mu$ (Cor. of Prop. 2), and it follows at once from Lebesgue’s theorem (Ch. IV, §4, No. 3, Prop. 4) that $\nu = \sup_n \nu_n$.

#### Corollary 3 {#int-v-s5-thm-2-cor-3 .statement}

— Let $\theta$ be a complex measure; there exists a universally measurable function $v$, with $|v| = 1$, such that $\theta = v \cdot |\theta|$, $|\theta| = \overline{v} \cdot \theta$.

Write $\theta = \theta_1 - \theta_2 + i(\theta_3 - \theta_4)$, where $\theta_1 = (\Re \theta)^+$, $\theta_2 = (\Re \theta)^-$, $\theta_3 = (\Im \theta)^+$, $\theta_4 = (\Im \theta)^-$; the positive measures $\theta_i$ ($i = 1, 2, 3, 4$), being bounded above by $|\theta|$ (Ch. III, §1, No. 6, formula (17)), are measures with base $|\theta|$ by Theorem 2. It follows that there exists a locally $|\theta|$-integrable function $v$ such that $\theta = v \cdot |\theta|$. Proposition 2 then yields the relation $|\theta| = |v| \cdot |\theta|$, which implies that $|v| = 1$ locally $|\theta|$-almost everywhere (Cor. 2 of Prop. 3). Finally, by Prop. 8, $\overline{v} \cdot \theta = (v \overline{v}) \cdot |\theta| = |\theta|$. Since the function $v$ is defined only up to a locally $|\theta|$-negligible function, one can suppose that $v$ is universally measurable (§3, No. 4, Prop. 7) and that $|v| = 1$ everywhere.

#### Remark 1 {#int-v-s5-n5-rem-1 .statement}

Suppose that $\lambda$ is a positive measure, that $v$ is a $\lambda$-measurable function such that $|v| = 1$ locally $\lambda$-almost everywhere (which implies that $v$ is locally $\lambda$-integrable), and that $\theta = v \cdot \lambda$. Prop. 2 shows immediately that $\lambda = |\theta|$; in other words, the property of the preceding statement characterizes the positive measure $|\theta|$.

#### Remark 2 {#int-v-s5-n5-rem-2 .statement}

If $|\theta| \leq a \mu$, where $\mu$ is a positive measure and $a$ is a number $\geq 0$, then $\theta$ is a measure with base $\mu$.

#### Corollary 4 {#int-v-s5-thm-2-cor-4 .statement}

— Let $\rho$ and $\theta$ be two complex measures. In order that there exist a locally $\theta$-integrable function $u$ such that $\rho = u \cdot \theta$, it is necessary and sufficient that every $\theta$-negligible compact set be $\rho$-negligible.

The condition is obviously necessary. Conversely, suppose that every $\theta$-negligible compact set is $\rho$-negligible; Theorem 2 implies the existence of a locally $|\theta|$-integrable function $g$ such that $|\rho| = g \cdot |\theta|$. On the other hand, Cor. 3 implies the existence of a function $v_1$ (resp. $v_2$), of absolute value 1 and measurable for the measure $|\rho|$ (resp. $\theta$), such that $\rho = v_1 \cdot |\rho|$ (resp. $|\theta| = \overline{v_2} \cdot \theta$). Then, by Prop. 8, $\rho = u \cdot \theta$ with $u = v_1 g \overline{v_2}$.

#### Corollary 5 {#int-v-s5-thm-2-cor-5 .statement}

— Let $\mu$ and $\nu$ be two positive measures on T. The conditions 1), 2), 3) of Th. 2 are also equivalent to the following ones:

4) For every $\nu$-integrable numerical function $f \geq 0$ and for every number $\varepsilon > 0$, there exists a $\delta > 0$ such that the relations $0 \leq h \leq f$ and $\int^* h \, d\mu \leq \delta$ imply $\int^* h \, d\nu < \varepsilon$.

5) For every function $g \in \mathcal{K}_+(\mathrm{T})$ and every number $\varepsilon > 0$, there exists a $\delta > 0$ such that, for every $h \in \mathcal{K}_+(\mathrm{T})$ bounded above by $g$ and satisfying $\int h \, d\mu \leq \delta$, one has $\int h \, d\nu \leq \varepsilon$.

6) For every compact set $K \subset \mathrm{T}$ and every number $\varepsilon > 0$, there exists a $\delta > 0$ such that the relations $A \subset K$ and $\mu^*(A) \leq \delta$ imply $\nu^*(A) \leq \varepsilon$.

The implications 4) $\Rightarrow$ 6) $\Rightarrow$ 3) are obvious.

Suppose there exists a finite function $k \geq 0$, universally measurable and locally $\mu$-integrable, such that $\nu = k \cdot \mu$, and let us show that the condition 4) is satisfied. Let $f$ be a $\nu$-integrable function $\geq 0$, and let $\varepsilon > 0$. For every integer $n \geq 0$, let $A_n$ be the set of $t \in \mathrm{T}$ such that $k(t) \geq n$. The functions $f \varphi_{A_n}$ form a decreasing sequence, bounded above by $f$ and tending pointwise to 0, therefore there exists an $N$ such that $\int f \varphi_{A_N} \, d\nu \leq \varepsilon/2$ (Ch. IV, §4, No. 3, Prop. 4). If $h$ is a function on $\mathrm{T}$ satisfying $0 \leq h \leq f$ and $\int^* h \, d\mu \leq \varepsilon/2N$, then

$$
\nu^*(h) \leq \nu^*(h \varphi_{A_N}) + \nu^*(h(1 - \varphi_{A_N}))
$$
$$
\leq \nu^*(f \varphi_{A_N}) + \mu^*(h(1 - \varphi_{A_N})k)
$$
$$
\leq \frac{\varepsilon}{2} + N \mu^*(h) \leq \varepsilon.
$$

We have thus proved that the conditions 4) and 6) are equivalent to the conditions of Th. 2.

It is clear that 4) implies 5). Finally, if the condition 5) is satisfied, then $\nu$ belongs to the band generated by $\mu$ (Ch. II, §2, No. 2, Prop. 5), hence has base $\mu$ (Cor. 2).

#### Scholium {#int-v-s5-n5-sch-1 .statement}

For every $\dot{f} \in L^1_{\mathrm{loc}}(\mathrm{T}, \mu; \mathbf{R})$, set $\varphi(\dot{f}) = f \cdot \mu$, where $f \in \dot{f}$; the mapping $\varphi$ is linear, increasing and injective (Cor. 2 of Prop. 3), and its image in $\mathcal{M}(T)$ is the band B generated by $\mu$ (Cor. 2 of Th. 2). The mapping $\varphi$ therefore permits identifying $L^1_{\text{loc}}(T, \mu; \mathbf{R})$ with a space of real measures on T; since all of the spaces $L^p_R(T, \mu)$ are subspaces of $L^1_{\text{loc}}(T, \mu; \mathbf{R})$, they too may be identified with subspaces of $\mathcal{M}(T)$. Analogous considerations hold for complex-valued functions and measures. Note that the mapping $\varphi$ considered above is an isomorphism of the ordered vector space structures of $L^1_{\text{loc}}$ and B, but is obviously not an isomorphism for the *topological vector space* structures of these spaces.

Since every band in a fully lattice-ordered space is itself a fully lattice-ordered space (Ch. II, §1, No. 5), one sees that the space $L^1_{\text{loc}}$ is *fully lattice-ordered*; but it is worthwhile to recall that the supremum in $L^1_{\text{loc}}$ of an uncountable family $(\dot{f}_\alpha)$ of equivalence classes is not necessarily identical to the class of the upper envelope of the functions $f_\alpha$. However, we saw that for an *increasing sequence* $(f_n)$ of locally $\mu$-integrable functions whose upper envelope $f$ is locally $\mu$-integrable, $f \cdot \mu$ is the supremum of the sequence of measures $(f_n \cdot \mu)$ in $\mathcal{M}(T)$ (Cor. of Prop. 6).

Here is an interesting consequence of Corollary 3 of Th. 2:

#### Proposition 9 {#int-v-s5-prop-9 .statement}

*Let $\theta$ be a bounded complex measure; for $\theta$ to be a positive measure, it is necessary and sufficient that $\| \theta \| = \theta(1)$.*.

The condition is obviously necessary. Conversely, suppose that $\| \theta \| = \int d\theta$, and denote by $v$ a $|\theta|$-measurable function of absolute value 1 such that $\theta = v \cdot |\theta|$. Since $\| \theta \| = \int d|\theta|$ (Ch. IV, §4, No. 7, Prop. 12) and $\int d\theta = \int v \cdot d|\theta|$ (Th. 1), the hypothesis implies that $\int (1 - v) \, d|\theta| = 0$ and therefore $\int \mathcal{R}(1 - v) \, d|\theta| = 0$. The function $\mathcal{R}(1 - v)$, being positive, is therefore zero almost everywhere, which implies that $v = 1$ almost everywhere and completes the proof.

### 6. Equivalent measures

#### Proposition 10 {#int-v-s5-prop-10 .statement}

*Let $\mu$ and $\nu$ be two positive measures on T. The following conditions are equivalent:
a) The locally negligible sets are the same for $\mu$ and $\nu$.
b) The bands generated by $\mu$ and $\nu$ in $\mathcal{M}(T)$ are identical.
c) One has $\nu = g \cdot \mu$, where $g$ is locally $\mu$-integrable and $g(t) > 0$ locally almost everywhere for $\mu$.*

The conditions a) and b) are equivalent by Cor. 2 of Th. 2 of No. 5. If they are satisfied, then $\nu = g \cdot \mu$ and $\mu = h \cdot \nu$, where $g$ (resp. $h$) is positive and locally integrable for $\mu$ (resp. $\nu$). Therefore (No. 4, Prop. 8) $hg$ is locally $\mu$-integrable and $\mu = (hg) \cdot \mu$. It follows (No. 3, Cor. 2 of Prop. 3) that $hg$ is equal to 1 locally almost everywhere for $\mu$, so that $g(t) > 0$ and $h(t) = 1/g(t)$ locally almost everywhere for $\mu$. Conversely, suppose that $\nu = g \cdot \mu$ with $g(t) > 0$ locally almost everywhere for $\mu$;

since $(1/g)g$ is defined locally almost everywhere and is locally $\mu$-integrable, $1/g$ is locally $\nu$-integrable and $(1/g) \cdot \nu = \mu$ (No. 4, Prop. 8).

#### Definition 3 {#int-v-s5-def-3 .statement}

*Two complex measures $\theta, \theta'$ on a locally compact space $T$ are said to be equivalent if the measures $|\theta|$ and $|\theta'|$ satisfy the conditions a), b), c) of Prop. 10.*

For $\theta$ and $\theta'$ to be equivalent, it is therefore necessary and sufficient that $|\theta|$ and $|\theta'|$ be equivalent.

#### Remark {#int-v-s5-n6-rem-1 .statement}

— If $\mu$ and $\nu$ are two equivalent positive measures then the measurable functions defined on $T$, with values in any topological space $G$, are *the same* for $\mu$ and $\nu$, as follows at once from Prop. 4 of No. 3.

#### Proposition 11 {#int-v-s5-prop-11 .statement}

*Let $\mu$ be a positive measure on $T$. If $T$ is countable at infinity, then there exists a continuous function $h$ such that $h(t) > 0$ for all $t \in T$ and such that the measure $\nu = h \cdot \mu$ (equivalent to $\mu$) is bounded.*

Let $(K_n)$ be a sequence of compact sets forming a covering of $T$ and, for every $n$, let $f_n$ be a function in $\mathcal{H}(T)$ such that $0 \leq f_n \leq 1$ and $f_n(t) = 1$ on $K_n$ (Ch. III, §1, No. 2, Lemma 1). Let $(a_n)$ be a sequence of numbers $> 0$ such that $\sum_n a_n < +\infty$; the series $h = \sum_n a_n f_n$ is then normally convergent in $T$, consequently $h$ is a continuous function on $T$, such that $h(t) > 0$ for all $t \in T$, by construction. Setting $\nu = h \cdot \mu$, we then have (Prop. 3 and Ch. IV, §1, No. 3, Prop. 13)

$$
\nu^*(1) = \int^* h \, d\mu \leq \sum_n a_n \int f_n \, d\mu .
$$

On taking for example $a_n = 2^{-n} (\int f_n \, d\mu)^{-1}$ when $\int f_n \, d\mu > 1$, and $a_n = 2^{-n}$ otherwise, we have $\sum_n a_n < +\infty$ and $\nu^*(1) < +\infty$, which proves the proposition.

#### Proposition 12 {#int-v-s5-prop-12 .statement}

*Let $(\mu_n)$ be a sequence of bounded positive measures on $T$; there exists a bounded positive measure $\mu$ on $T$ such that the relation $\mu^*(N) = 0$ is equivalent to «$\mu_n^*(N) = 0$ for every $n$»; each of the measures $\mu_n$ has base $\mu$. Moreover, if $\mu'$ is a second positive measure on $T$ having this property, then $\mu$ and $\mu'$ are equivalent.*

The last part of the statement follows at once from Def. 3. To prove the existence of $\mu$, we can restrict ourselves to the case that $\mu_n \neq 0$ for every $n$; the family of measures $\mu_n / 2^n \| \mu_n \|$ is then summable in $\mathcal{M}(T)$, and its sum $\mu$ is such that $\| \mu \| \leq 1$. Moreover, since $\mu_n \leq 2^n \| \mu_n \| \cdot \mu$, the relation $\mu(N) = 0$ implies that $\mu_n(N) = 0$ for all $n$; conversely, if $N$ is a set that is negligible for all the $\mu_n$, then it is locally negligible for $\mu$

(§2, No. 2, Cor. 2 of Prop. 1), hence is $\mu$-negligible since $\mu$ is bounded (§1, No. 2, Cor. 2 of Prop. 7).

### 7. Alien measures

Given two real measures $\rho, \sigma$ on $T$, recall that $\rho$ and $\sigma$ are said to be alien (to each other) if $\inf(|\rho|, |\sigma|) = 0$ in $\mathcal{M}(T)$ (Ch. II, §1, No. 1). The real measures alien to a given measure are known to form a band (Ch. II, §1, No. 5, Th. 1). This definition may be extended immediately to the case of complex measures.

#### Definition 4 {#int-v-s5-def-4 .statement}

*One says that a complex measure $\theta$ on $T$ is concentrated on a subset $M$ of $T$, or that $M$ carries $\theta$, if $\mathbf{C}M$ is locally negligible for $\theta$.*

The set $M$ carries $\theta$ if and only if it carries $|\theta|$. It is equivalent to say that $M$ carries $\theta$, or that $M$ is $\theta$-measurable and $\theta = \varphi_M \cdot \theta$. If $\theta$ is concentrated on $M$, then every measure with base $|\theta|$ is concentrated on $M$.

#### Proposition 13 {#int-v-s5-prop-13 .statement}

*In order that two complex measures $\rho$ and $\sigma$ on $T$ be alien to each other, it is necessary and sufficient that there exist in $T$ two disjoint sets $R$ and $S$ such that $\rho$ is concentrated on $R$ and $\sigma$ on $S$; $R$ and $S$ may be taken to be universally measurable.*

Set $\mu = |\rho|$, $\nu = |\sigma|$, $\lambda = \mu + \nu$; since $\mu$ and $\nu$ are bounded above by $\lambda$, there exist two locally $\lambda$-integrable functions $u$ and $v$ (which one can suppose to be universally measurable by §3, No. 4, Prop. 7) such that $\mu = u \cdot \lambda$, $\nu = v \cdot \lambda$. Then

$$
\inf(|\rho|, |\sigma|) = \inf(\mu, \nu) = \inf(u, v) \cdot \lambda
$$

(No. 2, Cor. of Prop. 2). Let $A$ (resp. $B$) be the set of $t \in T$ such that $u(t) > 0$ and $v(t) = 0$ (resp. $u(t) = 0$ and $v(t) > 0$). If $\rho$ and $\sigma$ are alien, then $\inf(u, v) = 0$ locally $\lambda$-almost everywhere (No. 3, Cor. 2 of Prop. 3), so that the disjoint universally measurable sets $A$ and $B$ carry $\mu$ and $\nu$, respectively. Conversely, suppose that $\mu$ and $\nu$ are carried, respectively, by disjoint sets $R$ and $S$; $\varphi_R$ is measurable for the measure $\mu = u \cdot \lambda$, and $\mu = \varphi_R \cdot \mu$. By Prop. 8 of No. 4, the function $u' = u \varphi_R$ is $\lambda$-measurable, and $\mu = u' \cdot \lambda$. Similarly, if $v' = v \varphi_S$ then $\nu = v' \cdot \lambda$; one concludes by remarking that $\inf(u', v') = 0$ (No. 2, Cor. of Prop. 2).

#### Corollary 1 {#int-v-s5-prop-13-cor-1 .statement}

*For every real measure $\nu$ on $T$, there exist two disjoint sets $M, N$ carrying $\nu^+$ and $\nu^-$, respectively.*

One must take care not to confuse the notion of support of a measure $\nu$, and that of a set where $\nu$ is concentrated. The support S of $\nu$ is the smallest closed set carrying $\nu$ (Ch. III, § 2, No. 2, Prop. 2 and Ch. IV, §2, No. 2, Prop. 5). However, there may exist subsets of S that are distinct from S and carry $\nu$. More generally, one can have $\inf(\mu, \nu) = 0$ for two positive measures $\mu$ and $\nu$ having the same support (Exer. 5).

Note also that the intersection of the sets carrying $\nu$ is the set of points $t \in T$ such that $|\nu|(\{t\}) > 0$, and it can be empty (for example, in the case of Lebesgue measure); therefore, there is not in general a smallest set carrying $\nu$.

#### Corollary 2 {#int-v-s5-prop-13-cor-2 .statement}

— Let $\rho$ and $\sigma$ be two alien complex measures, and let $\rho'$ and $\sigma'$ be two complex measures admitting densities relative to $\rho$ and $\sigma$, respectively; then $\rho'$ and $\sigma'$ are alien.

#### Corollary 3 {#int-v-s5-prop-13-cor-3 .statement}

— Let $\rho$ and $\sigma$ be two alien complex measures; then $|\rho + \sigma| = |\rho| + |\sigma|$.

Denote by $v$ (resp. $w$) a universally measurable function of absolute value 1 such that $\rho = v \cdot |\rho|$ (resp. $\sigma = w \cdot |\sigma|$) (Cor. 3 of Th. 2), and by A a universally measurable set carrying $\rho$, such that $B = \mathbf{C}A$ carries $\sigma$ (Prop. 13); then also $\rho + \sigma = (v \varphi_A + w \varphi_B) \cdot (|\rho| + |\sigma|)$. Since the function $v \varphi_A + w \varphi_B$ has absolute value equal to 1, the corollary follows from Prop. 2.

#### Theorem 3 (Lebesgue) {#int-v-s5-thm-3 .statement}

— Every complex measure $\theta$ on T may be written in one and only one way in the form $\theta = g \cdot \mu + \theta'$, where $g$ is locally $\mu$-integrable and $\theta'$ is a measure alien to $\mu$. Then $|\theta| = |g| \cdot \mu + |\theta'|$.

When $\theta$ is positive, this follows at once from the theorem of F. Riesz (Ch. II, §1, No. 5, Th. 1) applied to the fully lattice-ordered space $\mathcal{M}(T)$ of real measures on T, and to the band generated by $\mu$ in this space, on taking into account Cor. 2 of No. 5, Th. 2; moreover, $\theta'$ and $g \cdot \mu$ are then positive, which implies that $g$ is positive locally $\mu$-almost everywhere (Cor. 3 of Prop. 3). To treat the case that $\theta$ is not positive, set $\nu = |\theta|$, $\nu = f \cdot \mu + \nu'$ (where $f$ is positive and where $\nu'$ and $\mu$ are alien to each other), and $\theta = v \cdot \nu$, where $v$ is a universally measurable function of absolute value 1 (Cor. 3 of Th. 2). We then have (Prop. 8) $\theta = g \cdot \mu + \theta'$, with $g = v f$ (so that $|g| = f$) and $\theta' = v \cdot \nu'$ (so that $|\theta'| = \nu'$ by Prop. 2); the measures $\theta'$ and $\mu$ are alien to each other by Cor. 2 of Prop. 13. It only remains to establish the uniqueness of the decomposition. Thus, suppose that $\theta = g \cdot \mu + \theta' = g_1 \cdot \mu + \theta'_1$, where $\theta'$ and $\theta'_1$ are alien to $\mu$; $|\theta' - \theta'_1|$ is bounded above by $|\theta'| + |\theta'_1|$, therefore $\theta' - \theta'_1$ is alien to $\mu$, hence also to $(g_1 - g) \cdot \mu$. The relation $\theta' - \theta'_1 = (g_1 - g) \cdot \mu$ then implies that the two members are zero, which proves uniqueness.

Recall (No. 5, Th. 2 and Scholium) that the space $L^1_{loc}(T, \mu; \mathbf{C})$ may be identified (by means of the mapping $g \mapsto g \cdot \mu$) with a subspace of $\mathcal{M}_\mathbf{C}(T)$. With this convention, Theorem 3 takes the following form:

#### Corollary {#int-v-s5-n7-cor-1 .statement}

— *There exists a projector p of the space $\mathcal{M}_\mathbf{C}(T)$ onto the space $L^1_{\text{loc}}(T, \mu; \mathbf{C})$, whose kernel $\overline{p}^{-1}(0)$ is the set of complex measures alien to $\mu$, such that*

$$
|\theta| = |p(\theta)| + |\theta - p(\theta)|,\quad p(|\theta|) = |p(\theta)|
$$

*for every complex measure $\theta$.*

If $p$ is restricted to the set of bounded measures, one obtains a projector $p^1$ of the space $\mathcal{M}_\mathbf{C}^1(T)$ onto the space $L^1_\mathbf{C}(T, \mu)$; the relation $\| \theta \| = |\theta|(1)$ implies that $\| \theta \| = \| p^1(\theta) \| + \| \theta - p^1(\theta) \|$ for every bounded complex measure $\theta$.

### 8. Applications: I. Duality of the spaces $L^p$

We shall treat here only the case of the real spaces $L^p$.

Recall that two numbers $p, q$ such that $1 \leq p \leq +\infty$, $1 \leq q \leq +\infty$, $1/p + 1/q = 1$ are said to be *conjugate exponents* (Ch. IV, §6, No. 4). Every function $g \in \mathcal{L}^q$ defines a continuous linear form $\theta_g$ on $L^p$, obtained by passing to the quotient starting with the linear form $f \mapsto \int fg\,d\mu$ on $\mathcal{L}^p$, and one has $N_q(g) = \| \theta_g \|$ (Ch. IV, §6, No. 4, Cor. of Prop. 3). Passing to the quotient, one thus deduces from the mapping $g \mapsto \theta_g$ an isometric linear mapping $\varphi$ of $L^q$ into the dual $(L^p)'$ of $L^p$. We are going to show that, for $1 \leq p < +\infty$, $\varphi$ maps $L^q$ *onto* $(L^p)'$, so that we may henceforth identify the Banach space $L^q$ with the Banach space $(L^p)'$ by means of the isomorphism $\varphi$. Stated in other terms:

#### Theorem 4 {#int-v-s5-thm-4 .statement}

— *Let p and q be two conjugate exponents such that $1 \leq p < +\infty$. Every continuous linear form on $\mathcal{L}^p(T, \mu)$ is of the type $f \mapsto \int fg\,d\mu$, where g is a function in $\mathcal{L}^q(T, \mu)$ whose class in $L^q$ is well-defined.*

Let $\theta$ be a continuous linear form on $\mathcal{L}^p$; thus, there exists a number $a \geq 0$ such that $|\theta(f)| \leq a \cdot N_p(f)$ for every function $f \in \mathcal{L}^p$. Consider the restriction of $\theta$ to the space $\mathcal{K}(T)$ of continuous functions with compact support: for every compact subset K of T and every function $f \in \mathcal{K}(T, K)$ (the space of continuous functions with compact support contained in K), one has $N_p(f) \leq (\mu(K))^{1/p} \| f \|$; therefore the topology induced on $\mathcal{K}(T, K)$ by that of $\mathcal{L}^p$ is coarser than the topology of uniform convergence, and the restriction of $\theta$ to each $\mathcal{K}(T, K)$ is consequently continuous for the latter topology. This means that the restriction of $\theta$ to $\mathcal{K}(T)$ is a *real measure* $\nu$ (Ch. III, §1, No. 3, Def. 2).

Let us show that $|\nu|(|f|) \leq a \cdot N_p(f)$ for every function $f$ in $\mathcal{K}(T)$. It suffices to prove this formula for $f \geq 0$. Now, for every function $\psi$ in $\mathcal{K}(T)$ such that $|\psi| \leq f$, we have
$$
|\nu(\psi)| \leq a \cdot N_p(\psi) \leq a \cdot N_p(f);
$$
our assertion follows from the expression for the absolute value of a measure given in Ch. III, §1, No. 6, formula (12). The relation $|\nu|(|f|) \leq a (\mu(|f|^p))^{1/p}$ extends at once to the case that $f$ is the characteristic function of a compact set, by means of a passage to the lower envelope, and then implies that every $\mu$-negligible compact set is $\nu$-negligible, so that $\nu$ is a measure *with base* $\mu$ (No. 5, Th. 2).

Thus, there exists a locally $\mu$-integrable positive function $h_1$ such that $|\nu|(f) = \int f h_1 d\mu$ for every function $f \in \mathcal{K}(T)$. Let us show that $h_1$ is locally almost everywhere equal to a function in $\mathcal{L}^q$. If the function $f \geq 0$ in $\mathcal{K}(T)$ is such that $N_p(f) \leq 1$, then $\int f h_1 d\mu = |\nu|(f) \leq a$. For every continuous mapping $f_0$ of T into $[0,1]$ with compact support, we therefore have $\sup \int (f_0 h_1) f d\mu \leq a$ as $f$ runs over the set of functions $\geq 0$ in $\mathcal{K}(T)$ such that $N_p(f) \leq 1$. From this one deduces, by means of formula (11) of Chap. IV, §6, No. 4, that $N_q(f_0 h_1) \leq a$. It follows from this that $\sup_{K} N_q(\varphi_K h_1) \leq a$ as K runs over the set of compact subsets of T, and this proves our assertion (§1, Prop. 9).

Let $v$ be a universally measurable (real) function of absolute value 1 such that $\nu = v \cdot |\nu|$ (Cor. 3 of Th. 2) and let $g = v h_1$; then $\nu = g \cdot \mu$, and $g$ belongs to $\mathcal{L}^q$. For every function $f \in \mathcal{K}(T)$, we have $\theta(f) = \nu(f) = \int f g d\mu$. In other words, the continuous linear forms $\theta$ and $\theta_g$ coincide on $\mathcal{K}(T)$; they are therefore equal on $\mathcal{L}^p$, since $\mathcal{K}(T)$ is dense in $\mathcal{L}^p$, and this completes the proof.

#### Corollary {#int-v-s5-n8-cor-1 .statement}

— *For every number p such that $1 < p < +\infty$, the Banach space $L^p(T, \mu)$ is reflexive.*

In general, the dual of $L^\infty$ is not isomorphic to $L^1$, consequently $L^1$ and $L^\infty$ are not reflexive (Exer. 10). We are going to characterize the continuous linear forms on $L^\infty$ that arise, by passage to the quotient, from a linear form $g \mapsto \int f g d\mu$ on $\mathcal{L}^\infty$, where $g \in \mathcal{L}^1$.

The ordered vector space $L^\infty(T, \mu)$, which is a subspace of $L^1_{loc}(T, \mu)$, is *fully lattice-ordered*; for, if $(f_\alpha)$ is a family of positive functions in $\mathcal{L}^\infty$ whose set of classes $(\dot{f}_\alpha)$ is bounded above in $L^\infty$, there exists an $a \geq 0$ such that $N_\infty(f_\alpha) \leq a$ for all $\alpha$. Since $L^1_{loc}(T, \mu)$ is fully lattice-ordered, the family $(\dot{f}_\alpha)$ admits a supremum $\dot{h}$ in $L^1_{loc}(T, \mu)$; but since $\dot{a} \geq \dot{f}_\alpha$ for every $\alpha$, we have $\dot{h} \leq \dot{a}$, consequently $N_\infty(h) \leq a$, whence our assertion.

#### Proposition 14 {#int-v-s5-prop-14 .statement}

— *In order that a positive linear form $\theta$ on $\mathcal{L}^\infty$ be of the type $f \mapsto \int f g d\mu$, where $g \in \mathcal{L}^1$, it is necessary and sufficient that,* for every increasing directed family $(f_\alpha)_{\alpha \in A}$ of positive functions in $\mathcal{L}^\infty$ whose set of classes $(\dot{f}_\alpha)_{\alpha \in A}$ is bounded above in $L^\infty$ and admits $\dot{h}$ as its supremum in this space, one have

$$
\theta(h) = \sup_{\alpha \in A} \theta(f_\alpha).
$$

Let us first show that the condition is necessary. The measure $h \cdot \mu$ is the supremum in $\mathcal{M}(T)$ of the set of measures $f_\alpha \cdot \mu$ (No. 5, Scholium); therefore (Ch. II, §2, No. 2), for every function $\varphi \geq 0$ in $\mathcal{K}(T)$, we have $\int h \varphi \, d\mu = \sup_{\alpha \in A} \int f_\alpha \varphi \, d\mu$. If now $a$ is a number $\geq 0$ such that $N_\infty(f_\alpha) \leq a$ for all $\alpha \in A$ (which implies that $N_\infty(h) \leq a$), then for every $\varepsilon > 0$ there exists a $\varphi \in \mathcal{K}(T)$ such that $\varphi \geq 0$ and $N_1(g - \varphi) \leq \varepsilon$, from which we infer that $\int f_\alpha |g - \varphi| \, d\mu \leq a \varepsilon$ for all $\alpha \in A$, and $\int h |g - \varphi| \, d\mu \leq a \varepsilon$. Since $\sup_{\alpha \in A} \int f_\alpha g \, d\mu \leq \int h g \, d\mu$, this proves that the two members of this inequality are equal.

To establish that the condition is sufficient, we shall make use of the following lemma:

#### Lemma 4 {#int-v-s5-lem-4 .statement}

1° *Let $f$ be a lower semi-continuous and bounded positive function on $T$. Then its class $\dot{f}$ in $L^\infty$ is the supremum of the set of classes $\dot{\varphi}$, where $\varphi$ runs over the set of functions in $\mathcal{K}(T)$ such that $0 \leq \varphi \leq f$.*

2° *Let $f$ be a measurable and bounded positive function on $T$. Then its class $\dot{f}$ in $L^\infty$ is the infimum of the set of classes $\dot{\psi}$, where $\psi$ runs over the set of lower semi-continuous and bounded functions on $T$ that are $\geq f$.*

1° Let $f'$ be a function in $\mathcal{L}^\infty$ such that $\dot{f}'$ is the supremum in $L^\infty$ of the set of classes $\dot{\varphi}$ of the functions $\varphi$ in $\mathcal{K}(T)$ such that $0 \leq \varphi \leq f$; obviously $\dot{f}' \leq \dot{f}$. Let $U$ be a relatively compact open subset of $T$; for every function $h$ in $\mathcal{K}(T)$ such that $0 \leq h \leq f \varphi_U$ one has, by definition, $h(t) \leq f'(t)$ locally almost everywhere, therefore $h(t) \leq f'(t) \varphi_U(t)$ almost everywhere; it follows that $\int h \, d\mu \leq \int f' \varphi_U \, d\mu$. However, since $f \varphi_U$ is lower semi-continuous, $\int f \varphi_U \, d\mu = \sup \int h \, d\mu$, where $h$ runs over the set of functions in $\mathcal{K}(T)$ such that $0 \leq h \leq f \varphi_U$ (Ch. IV, §1, No. 1, Def. 1); therefore

$$
\int f \varphi_U \, d\mu \leq \int f' \varphi_U \, d\mu,
$$

and since $f' \varphi_U \leq f \varphi_U$ almost everywhere, necessarily $f \varphi_U = f' \varphi_U$ almost everywhere, whence $f = f'$ locally almost everywhere.

2° Let $f'$ be a function in $\mathcal{L}^\infty$ such that $\dot{f}'$ is the infimum in $L^\infty$ of the set of classes $\dot{\psi}$ of the lower semi-continuous functions $\psi$ that are bounded and $\geq f$; then $\dot{f}' \geq \dot{f}$. Let $K$ be a compact subset of $T$; for every lower semi-continuous function $h$ that is bounded and $\geq f \varphi_K$, let $\overline{h}$ be the function equal to $h$ on $K$ and to $\|f\| + \|h\|$ on $T - K$. Then $\overline{h}$ is lower semi-continuous and $\geq f$, therefore by definition $\overline{h}(t) \geq f'(t)$ locally almost everywhere; it follows that $h(t) \geq f'(t)\varphi_K(t)$ almost everywhere, whence $\int h d\mu \geq \int f'\varphi_K d\mu$. But $\int f\varphi_K d\mu = \inf \int h d\mu$, where $h$ runs over the set of lower semi-continuous functions that are bounded and $\geq f\varphi_K$ (Ch. IV, §1, No. 3, Def. 3); therefore

$$
\int f\varphi_K d\mu \geq \int f'\varphi_K d\mu,
$$

and since $f\varphi_K \leq f'\varphi_K$ almost everywhere, necessarily $f\varphi_K = f'\varphi_K$ almost everywhere, whence $f = f'$ locally almost everywhere.

The lemma having been proved, let $\theta$ be a positive linear form on $\mathcal{L}^\infty$ satisfying the condition in the statement of Prop. 14. The restriction of $\theta$ to the space $\mathcal{K}(T)$ is a positive measure $\nu$ on $T$. We are going to show that, for every positive function $f \in \mathcal{L}^\infty(T, \mu)$, one has $\theta(f) = \nu^*(f)$. Suppose first that $f$ is lower semi-continuous (and bounded); by Lemma 4, $f$ is the supremum of the increasing directed set of classes $\dot{\varphi}$, where $\varphi$ runs over the directed set $\Phi$ of functions in $\mathcal{K}(T)$ such that $0 \leq \varphi \leq f$. Since by hypothesis $\theta(f) = \sup_{\varphi \in \Phi} \theta(\varphi)$, and $\nu^*(f) = \sup_{\varphi \in \Phi} \nu(\varphi)$ by definition, our assertion is proved in this case. Secondly, suppose that $f$ is $\mu$-measurable and bounded; then, by definition, $\nu^*(f) = \inf_{\psi \in \Psi} \nu^*(\psi)$, where $\psi$ runs over the decreasing directed set $\Psi$ of lower semi-continuous functions that are bounded and $\geq f$. If $a \geq \|f\|$ then, applying the hypothesis of the statement to the increasing directed set of classes of the functions $a - \psi$, where $\psi \in \Psi$ and $\psi \leq a$, one sees, by virtue of the lemma, that $\theta(f) = \inf_{\psi \in \Psi} \theta(\psi)$, therefore indeed $\theta(f) = \nu^*(f)$. In particular, for every $\mu$-negligible function $f \geq 0$, one has $\theta(f) = 0$, therefore $\nu^*(f) = 0$ and consequently (No. 5, Th. 2) $\nu$ is a measure *with base* $\mu$; moreover, $\nu^*(1) = \theta(1) < +\infty$, consequently (Cor. of Th. 1) $\nu = g \cdot \mu$ with $g \in \mathcal{L}^1(T, \mu)$. Finally, since every $\mu$-measurable function is $\nu$-measurable, every positive function $f \in \mathcal{L}^\infty(T, \mu)$ is $\nu$-integrable and $\int fg d\mu = \nu^*(f) = \theta(f)$, which completes the proof.

One concludes from Prop. 14 that the linear forms on $\mathcal{L}^\infty$ of the type $f \mapsto \int fg d\mu$, where $g \in \mathcal{L}^1$, are the differences $\theta_1 - \theta_2$, where $\theta_1$ and $\theta_2$ are positive linear forms satisfying the condition of Prop. 14.

### 9. Applications: II. Functions of measures

Let $\mu_1, \mu_2, \ldots, \mu_n$ be real measures on T, and let $u(x_1, \ldots, x_n)$ be a finite numerical function, defined on $\mathbf{R}^n$, and positively homogeneous, that is (Ch. I, §1, No. 1), such that

$$
u(\alpha x_1, \ldots, \alpha x_n) = \alpha u(x_1, \ldots, x_n)
$$

for every scalar $\alpha \geqslant 0$. There exist positive measures $\lambda$ on T such that $|\mu_i| \leqslant \lambda$ for $1 \leqslant i \leqslant n$ (for example, the sum $\sum_{i=1}^n |\mu_i|$). Let $\lambda$ and $\lambda'$ be two such measures on T. One can write $\mu_i = f_i \cdot \lambda = f'_i \cdot \lambda'$, where $f_i$ (resp. $f'_i$) is measurable and essentially bounded for the measure $\lambda$ (resp. $\lambda'$) (No. 5, Th. 2). We are going to establish the following result: *in order that the numerical function $u(f_1, \ldots, f_n)$ be locally integrable for $\lambda$, it is necessary and sufficient that the function $u(f'_1, \ldots, f'_n)$ be locally integrable for $\lambda'$, in which case*

$$
u(f_1, \ldots, f_n) \cdot \lambda = u(f'_1, \ldots, f'_n) \cdot \lambda'.
$$

Since $|\mu_i| \leqslant \inf(\lambda, \lambda')$, we can restrict ourselves to the case that $\lambda \leqslant \lambda'$. Then $\lambda = g \cdot \lambda'$, where $g$ is a $\lambda'$-measurable function such that $0 \leqslant g \leqslant 1$ (No. 5, Th. 2); whence (No. 4, Prop. 8)

$$
\mu_i = f_i \cdot (g \cdot \lambda') = (f_i g) \cdot \lambda';
$$

it follows (No. 3, Cor. 2 of Prop. 3) that $f_i g$ is equal to $f'_i$ locally almost everywhere for $\lambda'$. Consequently, by (12),

$$
u(f'_1, \ldots, f'_n) = u(f_1 g, \ldots, f_n g) = u(f_1, \ldots, f_n) g
$$

locally almost everywhere for $\lambda'$. In order that $u(f'_1, \ldots, f'_n)$ be locally $\lambda'$-integrable, it is therefore necessary and sufficient that $u(f_1, \ldots, f_n) g$ be locally integrable for $\lambda'$, therefore (No. 4, Prop. 8) that $u(f_1, \ldots, f_n)$ be locally integrable for $\lambda$; and then (No. 4, Prop. 8)

$$
u(f'_1, \ldots, f'_n) \cdot \lambda' = (u(f_1, \ldots, f_n) g) \cdot \lambda' = u(f_1, \ldots, f_n) \cdot \lambda.
$$

Thus, the measure $u(f_1, \ldots, f_n) \cdot \lambda$ depends only on the measures $\mu_1, \ldots, \mu_n$ and the function $u$; it is also denoted $u(\mu_1, \ldots, \mu_n)$. This measure is therefore defined whenever $u$ is a positively homogeneous function such that, for a positive measure $\lambda$ that is an upper bound for all of the $|\mu_i|$, $u(f_1, \ldots, f_n)$ is locally $\lambda$-integrable, where $f_i$ denotes the density of $\mu_i$ with respect to $\lambda$. Note that this condition is fulfilled when $u$ is positively homogeneous and *continuous*: for, one then has
$$
|u(x_1, \ldots, x_n)| \leq a(|x_1| + |x_2| + \cdots + |x_n|)
$$
(*u* being bounded in a sufficiently small neighborhood of $(0, \ldots, 0)$)), and since $u(f_1, \ldots, f_n)$ is $\lambda$-measurable (Ch. IV, §5, No. 3, Th. 1), it is locally $\lambda$-integrable by virtue of the criterion for integrability (Ch. IV, §5, No. 6, Th. 5).

Let $u_1, \ldots, u_p$ be positively homogeneous numerical functions defined on $\mathbf{R}^n$, such that the $p$ functions $g_k = u_k(f_1, \ldots, f_n)$ $(1 \leq k \leq p)$ are locally $\lambda$-integrable. Let $v$ be a positively homogeneous numerical function defined on $\mathbf{R}^p$ such that $v(g_1, \ldots, g_p)$ is locally $\lambda$-integrable. Set
$$
w(x_1, \ldots, x_n) = v(u_1(x_1, \ldots, x_n), \ldots, u_p(x_1, \ldots, x_n)).
$$
Then, the function $w$ is positively homogeneous, $w(f_1, \ldots, f_n)$ is locally $\lambda$-integrable and, by definition,
$$
w(\mu_1, \ldots, \mu_n) = v(u_1(\mu_1, \ldots, \mu_n), \ldots, u_p(\mu_1, \ldots, \mu_n)).
$$

In the special case of the functions $x^+, x^-, |x|, x+y, \inf(x, y), \sup(x, y)$, the measures defined by the procedure just described coincide, respectively, with those that have been denoted $\mu^+, \mu^-, |\mu|, \mu+\nu, \inf(\mu, \nu), \sup(\mu, \nu)$; this follows at once from the Cor. of Prop. 2 of No. 2. If $\mu$ and $\nu$ are two real measures, and $\theta = \mu + i\nu$, then $|\theta| = \sqrt{\mu^2 + \nu^2}$; for, let $\lambda$ be a measure $\geq 0$ that is an upper bound for $|\mu|$ and $|\nu|$, and let $f, g$ be locally $\lambda$-integrable functions such that $\mu = f \cdot \lambda,\ \nu = g \cdot \lambda$; then
$$
\sqrt{\mu^2 + \nu^2} = \sqrt{f^2 + g^2} \cdot \lambda,
$$
$$
\theta = (f + ig) \cdot \lambda,\ \text{therefore (No. 2, Prop. 2)}\ |\theta| = \sqrt{f^2 + g^2} \cdot \lambda.
$$
This method can be applied to the positively homogeneous function $(x_1^2 + \ldots + x_n^2)^{1/2}$ to define the length of a curve in $\mathbf{R}^n$.

### 10. Diffuse measures; atomic measures

#### Definition 5 {#int-v-s5-def-5 .statement}

*A measure $\theta$ on T is said to be diffuse if* $|\theta|(\{t\}) = 0$ *for every* $t \in T$.

#### Example {#int-v-s5-n10-exa-1 .statement}

— Lebesgue measure on $\mathbf{R}$ is diffuse (Ch. IV, §1, No. 3, *Remark* 1).

To say that $\theta$ is a diffuse measure on $T$ amounts to saying that every set with finite complement carries $|\theta|$, or again that $|\theta|$ is alien to every point measure. The diffuse measures therefore form a band in $\mathcal{M}(T)$ (Ch. II, §1, No. 5, Th. 1).

Recall (Ch. III, §1, No. 3) that a complex measure $\rho$ on $T$ is said to be *atomic* if it is of the form $\sum_{t \in T} \alpha(t) \varepsilon_t$, where $\alpha$ is a complex function on $T$ such that $\sum_{t \in K} |\alpha(t)| < +\infty$ for every compact subset $K$ of $T$, which expresses that the family $(\alpha(t) \varepsilon_t)_{t \in T}$ is summable (§2, No. 1, Remark 2). It then follows from the remark following Cor. 3 of Th. 2 of No. 5 that $|\rho| = \sum_{t \in T} |\alpha(t)| \varepsilon_t$. The function $\alpha$ that occurs in these formulas is uniquely determined, because $\alpha(t) = \rho(\{t\})$. An atomic measure and a diffuse measure are alien to each other.

#### Proposition 15 {#int-v-s5-prop-15 .statement}

*Every complex measure $\sigma$ on $T$ may be written in one and only one way in the form $\rho + \theta$, where $\rho$ is an atomic measure and $\theta$ is a diffuse measure; one then has $|\sigma| = |\rho| + |\theta|$.*.

The uniqueness of the decomposition is obvious since, $\rho$ being atomic and $\theta$ diffuse, necessarily $\rho = \sum_{t \in T} \rho(\{t\}) \varepsilon_t = \sum_{t \in T} \sigma(\{t\}) \varepsilon_t$ and $\theta = \sigma - \rho$. To establish existence, it suffices to observe that $\sum_{t \in K} |\sigma(\{t\})| \leq |\sigma|(K) < +\infty$ for every compact set $K$, so that one can set $\sum_{t \in T} \sigma(\{t\}) \varepsilon_t = \rho$. The measure $\sigma - \rho$ is obviously diffuse, and the relation $|\sigma| = |\rho| + |\sigma - \rho|$ follows at once from Cor. 3 of Prop. 13 of No. 7.

One observes that this proof shows that if $\sigma$ is carried by a set $M$ and if $|\sigma|(\{t\}) > 0$ for every $t \in M$, then $\sigma$ is *atomic*.

### Exercises {#int-v-s5-exercises}

See the [exercises for § 5](exercises/s5/).
