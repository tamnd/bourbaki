---
book: int
book_title: Integration
chapter: V
chapter_title: INTEGRATION OF MEASURES
section: 8
section_title: Products of measures
lang: en
source: int-i-vi
book_pages: INT V.114-INT V.122
pdf_pages: 0334-0349, 0369-0377
extraction: ocr
subsections:
    - "no": 1
      title: Interpretation of the product measure as an integral of measures
      page: 79
      pdf_page: 334
    - "no": 2
      title: Functions measurable with respect to a product of two measures
      page: 81
      pdf_page: 336
    - "no": 3
      title: Integration of positive functions
      page: 83
      pdf_page: 338
    - "no": 4
      title: Integration of functions with values in a Banach space
      page: 87
      pdf_page: 342
    - "no": 5
      title: Operations on the product of two measures
      page: 89
      pdf_page: 344
    - "no": 6
      title: Integration with respect to a finite product of measures
      page: 91
      pdf_page: 346
    - "no": 7
      title: 'Application: Measure of the Euclidean ball in $\mathbf{R}^n$'
      page: 93
      pdf_page: 348
statements: 31
exercises: 21
content_sha256: a3e06c32a25b00ebb1bdb33d080383d36bc6c9d36cba335c108b496f0c58c969
---

## § 8. PRODUCTS OF MEASURES

### 1. Interpretation of the product measure as an integral of measures

Throughout this section, T and T' denote two locally compact spaces, $\mu$ a positive measure on T, $\mu'$ a positive measure on T', and $\nu = \mu \otimes \mu'$ the product measure on $X = T \times T'$ (Ch. III, §4, No. 1).

For every $t \in T$, the mapping $t' \mapsto (t, t')$ of T' into X is continuous and proper. Let $\lambda'_t$ be the image of $\mu'$ under this mapping; $\lambda'_t$ is a positive measure on X, and if $f \in \mathcal{K}(X)$ then, denoting by $f_t$ the partial mapping $t' \mapsto f(t, t')$, we have

$$
\int f \, d\lambda'_t = \int f_t \, d\mu',
$$

which is also expressed by the relation $\lambda'_t = \varepsilon_t \otimes \mu'$.

Moreover, the mapping $t \mapsto \lambda'_t(f)$ is continuous, with compact support (Ch. III, §4, No. 1, Lemma 2), therefore the mapping $t \mapsto \lambda'_t$ of T into $\mathcal{M}(X)$ is vaguely continuous (and, *a fortiori*, vaguely $\mu$-measurable); consequently, the family of measures $t \mapsto \lambda'_t$ is $\mu$-adequate ($§ 3$, No. 1, Prop. 2a)). The integral of $f$ with respect to the measure $\int \lambda'_t \, d\mu(t)$ is by definition

$$
\int \langle f, \lambda'_t \rangle \, d\mu(t) = \int d\mu(t) \int f_t(t') \, d\mu'(t') = \int f(t, t') \, d\nu(t, t')
$$

(Ch. III, §4, No. 1, Th. 2); thus $\nu = \int \lambda'_t \, d\mu(t)$.

Similarly, for every element $t' \in T'$, let $\lambda_{t'}$ be the image of $\mu$ under the mapping $t \mapsto (t, t')$ of T into X. The mapping $t' \mapsto \lambda_{t'}$ is $\mu'$-adequate and vaguely continuous, and $\nu = \int \lambda_{t'} \, d\mu'(t')$. We shall need the following lemmas:

#### Lemma 1 {#int-v-s8-lem-1 .statement}

*For every numerical function $f \geqslant 0$ defined on X,*

$$
\int^* f_t \, d\mu' = \int^* f \, d\lambda'_t.
$$

Since $t' \mapsto (t, t')$ is a continuous and proper mapping, this follows from Prop. 2 of §4, No. 2.

#### Lemma 2 {#int-v-s8-lem-2 .statement}

Let $f$ be a mapping of $X$ into a topological space. For $f$ to be $\lambda'_t$-measurable, it is necessary and sufficient that $f_t$ be $\mu'$-measurable.
This is a consequence of Prop. 3 of §6, No. 2.

#### Lemma 3 {#int-v-s8-lem-3 .statement}

Let $f$ be a function defined on $X$, with values in $\overline{\mathbf{R}}$ or in a Banach space. For $f$ to be $\lambda'_t$-integrable, it is necessary and sufficient that $f_t$ be $\mu'$-integrable, in which case

$$
\int f_t \, d\mu' = \int f \, d\lambda'_t .
$$

This follows from Th. 2 of §4, No. 4, on taking into account the fact that $t' \mapsto (t, t')$ is continuous and proper.

#### Remark {#int-v-s8-n1-rem-1 .statement}

Lemmas 1,2,3 can be proved very simply without making use of the results of §§4 and 6, by a direct argument. For example, the relation (2) is obvious by definition if $f \in \mathcal{K}(T \times T')$. If $f$ is lower semi-continuous on $X = T \times T'$, it suffices to observe that $t' \mapsto f_t(t')$ is the upper envelope of the functions $t' \mapsto g_t(t') = g(t, t')$, where $g$ runs over the set of functions in $\mathcal{K}(X)$ such that $0 \leq g \leq f$. Finally, for arbitrary $f$, one notes that if $h \geq f$ is lower semi-continuous on $X$, then $t' \mapsto h(t, t')$ is lower semi-continuous on $T'$; and conversely, if $t' \mapsto u(t')$ is lower semi-continuous on $T'$ and is such that $u(t') \geq f(t, t')$ for all $t' \in T'$, then the function $h$ such that $h(t, t') = u(t')$, $h(t_1, t') = +\infty$ for $t_1 \neq t'$, is lower semi-continuous on $X$ and satisfies $h \geq f$. Once Lemma 1 is proved, one deduces from it that the set $(T - \{t\}) \times T'$ is $\lambda'_t$-negligible, and it is then every easy to prove Lemmas 2 and 3.

The relation (3) permits denoting its two members by $\int f(t, t') \, d\mu'(t')$ without risk of confusion. The analogous results obviously hold for the measures $\lambda_{t'} = \mu \otimes \varepsilon_{t'}$.

Instead of the notations

$$
\int^* f(t, t') \, d\nu(t, t'), \quad \int^\bullet f(t, t') \, d\nu(t, t'), \quad \int f(t, t') \, d\nu(t, t'),
$$

we shall employ the notations

$$
\iint^* f(t, t') \, d\mu(t) \, d\mu'(t'), \quad \iint^\bullet f(t, t') \, d\mu(t) \, d\mu'(t'), \quad \iint f(t, t') \, d\mu(t) \, d\mu'(t'),
$$

consistent with the notations adopted in Ch. III, §4, No. 1.

The interpretation of the measure $\nu$ as an integral $\int \lambda'_t \, d\mu(t)$ will allow us to translate the results of §3 into the language of product measures. On the other hand, the measure $\lambda'_t$ is carried by $\{t\} \times T' = \overline{\mathrm{pr}}_1^{-1}(t)$, so that this integral defines a decomposition of $\nu$ into slices, relative to the projection $\mathrm{pr}_1$ of $T \times T'$ onto $T$ (§6, No. 6). Before giving a list of the results so obtained, here is a useful property:

#### Proposition 1 {#int-v-s8-prop-1 .statement}

— Let $(\mu_\alpha)_{\alpha \in A}$ (resp. $(\mu'_\beta)_{\beta \in B}$) be a summable family of positive measures on T (resp. on T'), with sum denoted by $\mu$ (resp. by $\mu'$). The family $(\mu_\alpha \otimes \mu'_\beta)_{(\alpha, \beta) \in A \times B}$ is then summable on $T \times T'$, and

$$
\mu \times \mu' = \sum_{(\alpha, \beta) \in A \times B} \mu_\alpha \otimes \mu'_\beta.
$$

These properties are obvious when A and B are finite. It follows that if $A'$ (resp. $B'$) is a finite subset of A (resp. of B), then

$$
\sum_{(\alpha, \beta) \in A' \times B'} \mu_\alpha \otimes \mu'_\beta \leq \mu \otimes \mu'.
$$

The family $(\mu_\alpha \otimes \mu'_\beta)$ is therefore summable. To show that the two members of (4) are equal, it suffices to prove that the second member satisfies the characteristic property of product measures (Ch. III, §4, No. 1, Th. 1), which is shown by the following calculation.

Let $f$ be an element of $\mathcal{K}_+(T)$, $f'$ an element of $\mathcal{K}_+(T')$; recall that $f \otimes f'$ denotes the function $(t, t') \mapsto f(t)f'(t')$ on $T \times T'$, which belongs to $\mathcal{K}_+(T \times T')$ (A, II, §7, No. 7). Then, by the definition of product measures,

$$
\sum_{(\alpha, \beta) \in A \times B} \langle \mu_\alpha \otimes \mu'_\beta, f \otimes f' \rangle = \sum_{(\alpha, \beta) \in A \times B} (\langle \mu_\alpha, f \rangle \langle \mu'_\beta, f' \rangle)
= \left( \sum_{\alpha \in A} \langle \mu_\alpha, f \rangle \right) \left( \sum_{\beta \in B} \langle \mu'_\beta, f' \rangle \right)
= \langle \mu, f \rangle \langle \mu', f' \rangle
= \langle \mu \otimes \mu', f \otimes f' \rangle.
$$

### 2. Functions measurable with respect to a product of two measures

#### Proposition 2 {#int-v-s8-prop-2 .statement}

— Let $f$ be a $\nu$-measurable function defined on $T \times T'$, with values in a topological space G, and let M be the set of $t \in T$ such that the mapping $t' \mapsto f(t, t')$ is not $\mu'$-measurable.

a) If $f$ is constant on the complement of a $\nu$-moderated subset of $T \times T'$, then M is $\mu$-negligible.

b) If $\mu'$ is moderated, then M is $\mu$-negligible.

The assertion a) follows from Prop. 4b) of §3, No. 2 and the remarks of No. 1. To treat b), note that $\mu'$ is the sum of a sequence $\mu'_n$ of bounded measures (§2, No. 3, Prop. 4); $f$ is measurable with respect to $\mu \otimes \mu'_n \leq \nu$, and the set $M$ is the union of the sets $M_n$ associated with the measures $\mu'_n$ (§ 2, No. 2, Prop. 2). One is thus reduced to the case that $\mu'$ is bounded, which follows from Prop. 4c) of § 3, No. 2.

This statement extends immediately to complex measures (Ch. III, § 4, No. 2, Prop. 3).

#### Corollary {#int-v-s8-n2-cor-1 .statement}

— *Let A be a $\nu$-measurable subset of $T \times T'$, and let M be the set of $t \in T$ such that the section $A(t)$ of A at t is not $\mu'$-measurable.*

a) *If A is $\nu$-moderated, then M is $\mu$-negligible.*

b) *If the projection of A on $T'$ is $\mu'$-moderated, then M is locally $\mu$-negligible.*

The assertion a) follows immediately from Prop. 2. To establish b), denote by B a set, the union of a sequence of $\mu'$-integrable open sets in $T'$, that contains the projection of A on $T'$, and denote by $\mu'_1$ the moderated measure $\varphi_B \cdot \mu'$; since A is measurable with respect to $\mu \otimes \mu'_1 \leq \mu \otimes \mu'$, Prop. 2 implies that $A(t)$ is $\mu'_1$-measurable, except for $t$ forming a locally $\mu$-negligible set. But since $A(t) \subset B$, to say that $A(t)$ is $\mu'_1$-measurable is equivalent to saying that $A(t)$ is $\mu'$-measurable (§ 5, No. 3, Cor. of Prop. 4).

#### Proposition 3 {#int-v-s8-prop-3 .statement}

— *Let f be a mapping of T into a topological space F. If f is $\mu$-measurable, then the mapping $(t, t') \mapsto f(t)$ is $\nu$-measurable. Conversely, if $\mu' \neq 0$, and if this mapping is $\nu$-measurable, then the function f is $\mu$-measurable.*

The first assertion follows from Cor. 1 of Prop. 10 of § 6, No. 6. Suppose that $\mu' \neq 0$, denote by $\mu'_1$ a nonzero measure with compact support that is bounded above by $\mu'$, by $\nu_1$ the measure $\mu \otimes \mu'_1$, and set $a = \| \mu'_1 \|$. The projection $\mathrm{pr}_1$ of $T \times T'$ onto T is then $\nu_1$-proper, and the image measure $\mathrm{pr}_1(\nu_1)$ is equal to $a \mu$ (§ 6, No. 6, Prop. 10). If $(t, t') \mapsto f(t)$ is $\nu$-measurable, then it is also $\nu_1$-measurable, therefore $f$ is measurable with respect to the measure $a \mu$ (§ 6, No. 2, Prop. 3), whence the result since $a \neq 0$.

The preceding statement extends immediately to complex measures (Ch. III, § 4, No. 2, Prop. 3), as do the following corollaries.

#### Corollary 1 {#int-v-s8-prop-3-cor-1 .statement}

— *Let F, F' and G be three topological spaces, and let u be a continuous mapping of $F \times F'$ into G. Let f (resp. $f'$) be a function defined on T (resp. $T'$) with values in F (resp. $F'$) and measurable for $\mu$ (resp. $\mu'$). Then the function $(t, t') \mapsto u(f(t), f'(t'))$ is measurable for $\mu \otimes \mu'$.*

The mappings $(t, t') \mapsto f(t)$, $(t, t') \mapsto f'(t')$ being $\nu$-measurable by Prop. 3, this follows from Th. 1 of Ch. IV, § 5, No. 3.

#### Corollary 2 {#int-v-s8-prop-3-cor-2 .statement}

— *If $A \subset T$ and $A' \subset T'$ are measurable (for $\mu$ and $\mu'$, respectively), then $A \times A'$ is measurable for $\mu \otimes \mu'$.*
This follows at once from Cor. 1.

#### Corollary 3 {#int-v-s8-prop-3-cor-3 .statement}

— *Consider two positive numerical (resp. complex-valued) functions $f$ defined on $T$ and $f'$ defined on $T'$. If these functions are measurable for $\mu$ and $\mu'$, respectively, then the function*

$$
f \otimes f' : (t, t') \mapsto f(t)f'(t')
$$

*is measurable for $\mu \otimes \mu'$.*

The case of complex functions, or of finite real functions, is an immediate consequence of Cor. 1. To treat the case of positive numerical functions, for every integer $n \geqslant 0$ we set $f_n = \inf(f, n)$, $f'_n = \inf(f', n)$, and we have (with the usual convention $0 \cdot (+\infty) = 0$) $f \otimes f' = \sup_n (f_n \otimes f'_n)$, whence the result.

#### Proposition 4 {#int-v-s8-prop-4 .statement}

— *Let $A$ be a subset of $T$. If $A$ is locally $\mu$-negligible, then $A \times T'$ is locally $\nu$-negligible. Conversely, if $A \times T'$ is locally $\nu$-negligible and if $\mu' \neq 0$, then $A$ is locally $\mu$-negligible.*

The first assertion follows from Cor. 1 of Prop. 10 of §6, No. 6. To establish the second assertion, let us take up again the notations in the proof of Prop. 3; $A \times T' = \mathrm{pr}_1^{-1}(A)$ is locally negligible for the measure $\nu_1$, therefore $A$ is locally negligible for $a\mu$ (§ 6, No. 2, Cor. of Prop. 2), whence the result since $a \neq 0$.

The preceding statement extends at once to the product of two complex measures (Ch. III, §4, No. 2, Prop. 3), as does the following corollary.

#### Corollary {#int-v-s8-n2-cor-2 .statement}

— *If the measure $\mu$ (resp. $\mu'$) is concentrated on $M$ (resp. $M'$), then $\mu \otimes \mu'$ is concentrated on $M \times M'$.*

For, $(T \times T') - (M \times M')$ is the union of the sets $(T - M) \times T'$ and $T \times (T' - M')$, which are locally negligible for $\mu \times \mu'$ by Prop. 4.

### 3. Integration of positive functions

Recall that we have agreed to define the product $0 \cdot (+\infty)$ to be equal to 0. This convention has in particular the following consequence: if $f$ is a numerical function $\geqslant 0$ defined on a locally compact space equipped with a positive measure $\lambda$, then $\lambda^*(af) = a \cdot \lambda^*(f)$ for every constant $a$ such that $0 \leqslant a \leqslant +\infty$. This is obvious if $a = 0$; if $a = +\infty$, then $\lambda^*(af) = a \cdot \lambda^*(f) = 0$ or $\lambda^*(af) = a \cdot \lambda^*(f) = +\infty$ according as $f$ is $\lambda$-negligible or not; finally, if $0 < a < +\infty$, one knows that $\lambda^*(af) = a \cdot \lambda^*(f)$.

#### Proposition 5 {#int-v-s8-prop-5 .statement}

— Let $f$ be a numerical function $\geqslant 0$, lower semi-continuous on $T \times T'$. Then, the function

$$
t \mapsto \int^* f(t, t') \, d\mu'(t')
$$

is lower semi-continuous on $T$, and

$$
\iint^* f(t, t') \, d\mu(t) \, d\mu'(t') = \int^* d\mu(t) \int^* f(t, t') \, d\mu'(t').
$$

This is a consequence of Prop. 2 of §3, No. 1, taking into account Lemma 1 of No. 1.

#### Corollary 1 {#int-v-s8-prop-5-cor-1 .statement}

— Let $f$ (resp. $f'$) be a lower semi-continuous function $\geqslant 0$ defined on $T$ (resp. $T'$); the function $f \otimes f' : (t, t') \mapsto f(t)f'(t')$ is then lower semi-continuous on $T \times T'$, and

$$
\iint^* f(t)f'(t') \, d\mu(t) \, d\mu'(t') = \left( \int^* f(t) \, d\mu(t) \right) \left( \int^* f'(t') \, d\mu'(t') \right).
$$

Let $G$ (resp. $G'$) be the set of functions $g \in \mathcal{K}_+(T)$ (resp. $g' \in \mathcal{K}_+(T')$) such that $g \leqslant f$ (resp. $g' \leqslant f'$); then

$$
f \otimes f' = \sup_{g \in G,\ g' \in G'} g \otimes g'.
$$

Since the functions $g \otimes g'$ belong to $\mathcal{K}_+(T \times T')$, $f \otimes f'$ is indeed lower semi-continuous, and (6) follows at once from Prop. 5 (or directly by passage to the limit in the preceding formula).

#### Corollary 2 {#int-v-s8-prop-5-cor-2 .statement}

— Let $A$ be a $\mu$-moderated subset of $T$, and $A'$ a $\mu'$-moderated subset of $T'$; then $A \times A'$ is $\nu$-moderated in $T \times T'$.

In view of the definition of moderated set (§1, No. 2, Prop. 5), it suffices to show that if $B$ is an integrable open set in $T$, and $B'$ an integrable open set in $T'$, then the open set $B \times B'$ is integrable. This follows at once from Cor. 1.

#### Corollary 3 {#int-v-s8-prop-5-cor-3 .statement}

— Let $A$ be a $\mu$-negligible subset of $T$, and let $B'$ be a $\mu'$-moderated subset of $T'$; then $A \times B'$ is $\nu$-negligible.

For, $A \times B'$ is locally $\nu$-negligible (Prop. 4) and $\nu$-moderated (Cor. 2), hence is $\nu$-negligible (§1, No. 2, Cor. 1 of Prop. 7).

Cors. 2 and 3 may be extended to the product of two complex measures, on applying the statement to their absolute values (Ch. III, §4, No. 2, Prop. 3).

#### Proposition 6 {#int-v-s8-prop-6 .statement}

— Let $f$ be a numerical function $\geqslant 0$ defined on $T \times T'$. Then

$$
\iint^* f(t, t') d\mu(t) d\mu'(t') \geqslant \int^* d\mu(t) \int^* f(t, t') d\mu'(t').
$$

This follows from Prop. 3 of §3, No. 2, on taking (2) into account.

#### Proposition 7 {#int-v-s8-prop-7 .statement}

— Let $f$ be a $\nu$-measurable positive numerical function defined on $T \times T'$.

a) *If $f$ is $\nu$-moderated, then the functions* $t \mapsto \int^* f(t, t') d\mu'(t')$, $t' \mapsto \int^* f(t, t') d\mu(t)$ *are measurable and moderated for $\mu$ and $\mu'$, respectively, and*

$$
\iint^* f(t, t') d\mu(t) d\mu'(t') = \int^* d\mu(t) \int^* f(t, t') d\mu'(t')
$$
(7)
$$
= \int^* d\mu'(t') \int^* f(t, t') d\mu(t).
$$

b) *If the measure $\mu'$ is moderated, then the function* $t \mapsto \int^* f(t, t') d\mu'(t')$ *is $\mu$-measurable, and*

$$
\iint^* f(t, t') d\mu(t) d\mu'(t') = \int^* d\mu(t) \int^* f(t, t') d\mu'(t').
$$
(8)

The assertion a), as well as the assertion b) when $\mu'$ is bounded, are consequences of Prop. 5 of §3, No. 2. To treat the case that $\mu'$ is moderated, let us represent $\mu'$ as a sum $\sum_{n \in \mathbf{N}} \mu'_n$ of a sequence of bounded measures (§ 2, No. 3, Prop. 4). The function $t \mapsto \int^* f(t, t') d\mu'_n(t')$ is then $\mu$-measurable, and
$$
\iint^* f(t, t') d\mu(t) d\mu'_n(t') = \int^* d\mu(t) \int^* f(t, t') d\mu'_n(t').
$$
But $\mu \otimes \mu' = \sum_{n \in \mathbf{N}} (\mu \otimes \mu'_n)$ (Prop. 1); the assertion b) is then obtained by summing on $n$ (§ 2, No. 2, Prop. 1).

#### Corollary 1 {#int-v-s8-prop-7-cor-1 .statement}

— Let $H$ be a subset of $T \times T'$, and let $A$ be the set of $t \in T$ such that the section $H(t)$ of $H$ at $t$ is not $\mu'$-negligible.

a) *If $H$ is $\nu$-negligible then $A$ is $\mu$-negligible.*

b) *If $H$ is locally $\nu$-negligible and $\mu'$ is moderated, then $A$ is locally $\mu$-negligible.*

The property a) follows at once from Prop. 7 (or from Prop. 6). Under the hypotheses of b), it comes to the same to say that $H(t)$ is locally μ′-negligible or that it is μ′-negligible, since μ′ is moderated (§1, No. 2, Prop. 7). Thus property b) follows from the formula (8).

This corollary extends at once, by passage to absolute values, to the product of two complex measures. The same is true for the following corollary:

#### Corollary 2 {#int-v-s8-prop-7-cor-2 .statement}

— *If a set* $A \subset T \times T'$ *is ν-integrable, then the section* $A(t)$ *of* $A$ *at* $t$ *is μ′-integrable for almost every* $t \in T$, *the function* $t \mapsto \mu'(A(t))$ *is μ-integrable, and*

$$
\nu(A) = \int \mu'(A(t))\, d\mu(t).
$$

#### Proposition 8 {#int-v-s8-prop-8 .statement}

— *For every pair of numerical functions* $f \geq 0$, $f' \geq 0$ *defined on* $T$ *and* $T'$, *respectively,

$$
\iint^\bullet f(t)f'(t')\, d\mu(t)\, d\mu'(t') = \left( \int^\bullet f(t)\, d\mu(t) \right) \left( \int^\bullet f'(t')\, d\mu'(t') \right).
$$

We begin by treating the case that $\mu$ and $\mu'$ are measures *with compact support*; the same is then true of $\mu \otimes \mu'$, and all of the symbols $\int^\bullet$, $\iint^\bullet$ may be replaced by upper integrals. By Prop. 6,

$$
\iint^* f(t)f'(t')\, d\mu(t)\, d\mu'(t') \geq \int^* d\mu(t) \int^* f(t)f'(t')\, d\mu'(t')
$$
$$
= \left( \int^* f(t)\, d\mu(t) \right) \left( \int^* f'(t')\, d\mu'(t') \right).
$$

To establish the reverse inequality, let us choose a function $h \geq f$ (resp. $h' \geq f'$), the lower envelope of a sequence $(h_n)$ (resp. $(h'_n)$) of lower semi-continuous functions, such that

$$
\int^* h(t)\, d\mu(t) = \int^* f(t)\, d\mu(t)
$$

(resp. $\int^* h'(t')\, d\mu'(t') = \int^* f'(t')\, d\mu'(t')$); the existence of such functions follows immediately from the definition of upper integral (Ch. IV, §1, No. 3, Def. 3) and Lebesgue’s theorem. Applying Prop. 7 to the measurable function $h \otimes h'$, we have

$$
\iint^* f(t)f'(t')\, d\mu(t)\, d\mu'(t') \leq \iint^* h(t)h'(t')\, d\mu(t)\, d\mu'(t')
$$
$$
= \left( \int^* h(t)\, d\mu(t) \right) \left( \int^* h'(t')\, d\mu'(t') \right)
$$
$$
= \left( \int^* f(t)\, d\mu(t) \right) \left( \int^* f'(t')\, d\mu'(t') \right),
$$

which is the sought-for inequality. Thus the proposition is established when $\mu$ and $\mu'$ are measures with compact support. To treat the general case, it suffices to represent $\mu$ (resp. $\mu'$) as the sum of a family $(\mu_\alpha)_{\alpha \in A}$ (resp. $(\mu'_\beta)_{\beta \in B}$) of measures with compact support (§ 2, No. 3, Prop. 4), write the formula (10) for each measure $\mu_\alpha \otimes \mu'_\beta$, and sum on $(\alpha, \beta)$, taking into account Prop. 1 (§ 2, No. 2, Prop. 1).

#### Corollary 1 {#int-v-s8-prop-8-cor-1 .statement}

*With notations as in Prop. 8,

$$
\iint^* f(t)f'(t')\,d\mu(t)\,d\mu'(t') = \left( \int^* f(t)\,d\mu(t) \right) \left( \int^* f'(t')\,d\mu'(t') \right)
$$

except possibly when one of the factors of the second member is equal to 0 and the other is equal to $+\infty$.

When the two factors of the second member are finite, the functions $f$ and $f'$ are moderated (§ 1, No. 2, Prop. 7), therefore the function $f \otimes f'$ is moderated (Cor. 2 of Prop. 5); the above equality therefore reduces to the formula (10) (§ 1, No. 2, Prop. 7). When one of the factors of the second member has the value $+\infty$ and the other is not zero, then the second member has the value $+\infty$, and the above equality follows from Prop. 6.

#### Corollary 2 {#int-v-s8-prop-8-cor-2 .statement}

*Let $f$ and $f'$ be two functions with values in $\mathbf{C}$ or in $\overline{\mathbf{R}}$, defined on $T$ and $T'$, respectively, and essentially integrable (resp. integrable) for the measures $\mu$ and $\mu'$, respectively. The function $f \otimes f'$ is then essentially integrable (resp. integrable) for the measure $\mu \otimes \mu'$, and*

$$
\iint f(t)f'(t')\,d\mu(t)\,d\mu'(t') = \left( \int f(t)\,d\mu(t) \right) \left( \int f'(t')\,d\mu'(t') \right).
$$

When $f$ and $f'$ are positive, $f \otimes f'$ is measurable by Cor. 3 of Prop. 3, and the statement follows from formula (10) (resp. (11)) and the criterion for essential integrability (§ 1, No. 3, Prop. 9) (resp. the integrability criterion of Ch. IV, § 5, No. 6, Th. 5). The general case then follows immediately.

Corollary 2 extends at once to the product of two complex measures.

### 4. Integration of functions with values in a Banach space

#### Theorem 1 (Lebesgue–Fubini) {#int-v-s8-thm-1 .statement}

— *Let $f$ be a function defined on $T \times T'$, with values in a Banach space $F$ or in $\overline{\mathbf{R}}$; let $N$ be the set of $t \in T$ such that the function $t' \mapsto f(t,t')$ is not $\mu'$-integrable.

a) Suppose that $f$ is $\nu$-integrable; then $N$ is $\mu$-negligible, the function $t \mapsto \int f(t,t')\,d\mu'(t')$ (defined for $t \notin N$) is $\mu$-integrable, and*

$$
\iint f(t,t')\,d\mu(t)\,d\mu'(t') = \int d\mu(t) \int f(t,t')\,d\mu'(t').
$$

b) *Suppose that $f$ is essentially $\nu$-integrable, and that the measure $\mu'$ is moderated; then $N$ is locally $\mu$-negligible, the function $t \mapsto \int f(t, t')\, d\mu'(t')$ (defined for $t \notin N$) is essentially $\mu$-integrable, and (13) holds.*

The assertion a) follows at once from Th. 1 of §3, No. 3. To establish b), let us denote by $g$ a $\nu$-integrable function equal to $f$ locally almost everywhere, and by $H$ the set of $(t, t')$ such that $f(t, t') \neq g(t, t')$. By Cor. 1 of Prop. 7, the section $H(t)$ is $\mu'$-negligible, except for $t \in T$ forming a locally $\mu$-negligible set. The result pertaining to $f$ may then be deduced from the statement a) applied to $g$.

#### Scholium {#int-v-s8-n4-sch-1 .statement}

— *Let $f$ be a function defined on $T \times T'$, with values in $\overline{\mathbf{R}}$ or in a Banach space, that is $\nu$-measurable and $\nu$-moderated. For the three integrals*

$$
\iint f(t, t')\, d\mu(t)\, d\mu'(t'), \quad \int d\mu(t) \int f(t, t')\, d\mu'(t'), \quad \int d\mu'(t') \int f(t, t')\, d\mu(t)
$$

*to exist and be equal, it is necessary and sufficient that one of the two numbers*

$$
\int^* d\mu(t) \int^* |f(t, t')|\, d\mu'(t'), \quad \int^* d\mu'(t') \int^* |f(t, t')|\, d\mu(t)
$$

*be finite.*

This is an immediate consequence of Th. 1, Prop. 7 and the integrability criterion (Ch. IV, §5, No. 6, Th. 5).

#### Remark {#int-v-s8-n4-rem-1 .statement}

— 1) When the measure $\mu'$ is not moderated, it can happen that $f$ is essentially $\nu$-integrable and the function $t' \mapsto f(t, t')$ is not essentially $\mu'$-integrable for any value of $t \in T$ (§3, Exer. 4).

2) Let $\mu$ and $\mu'$ be two complex measures, and let $\nu = \mu \otimes \mu'$. If $f$ is $\nu$-integrable (in other words, $|\nu|$-integrable), then application of the theorem to the measures $|\mu|$ and $|\mu'|$, whose product is $|\nu|$ (Ch. III, §4, No. 2, Prop. 3), implies that $t' \mapsto f(t, t')$ is $\mu'$-integrable for $\mu$-almost every $t$. From this one deduces, on decomposing the measures $\mu$ and $\mu'$ as a linear combination of positive measures, that the statement of a) extends to complex measures. One can argue similarly for b).

#### Proposition 9 {#int-v-s8-prop-9 .statement}

*Let $F$, $F'$ and $G$ be three Banach spaces, and let $(x, y) \mapsto [x \cdot y]$ be a continuous bilinear mapping of $F \times F'$ into $G$. Let $f$ (resp. $f'$) be a function defined on $T$ (resp. $T'$) with values in $F$ (resp. $F'$) and essentially integrable for $\mu$ (resp. $\mu'$). Let $g$ be the function $(t, t') \mapsto [f(t) \cdot f'(t')]$; then $g$ is essentially integrable for $\mu \otimes \mu'$, and*

$$
\iint [f(t) \cdot f'(t')] \, d\mu(t)\, d\mu'(t') = \left[ \left( \int f\, d\mu(t) \right) \cdot \left( \int f'(t')\, d\mu'(t') \right) \right].
$$

*If, moreover, $f$ and $f'$ are integrable, then $g$ is integrable.*

The function $(t, t') \mapsto [\mathbf{f}(t) \cdot \mathbf{f}'(t')]$ is $(\mu \otimes \mu')$-measurable by Cor. 1 of Prop. 3. On the other hand, if $b$ denotes the norm of the bilinear mapping $(\mathbf{x}, \mathbf{y}) \mapsto [\mathbf{x} \cdot \mathbf{y}]$, then

$$
\iint^\bullet |[\mathbf{f}(t) \cdot \mathbf{f}'(t')]| d\mu(t) d\mu'(t') \leq b \iint^\bullet |\mathbf{f}(t)| \cdot |\mathbf{f}'(t')| d\mu(t) d\mu'(t')
$$
$$
= b \left( \int^\bullet |\mathbf{f}(t)| d\mu(t) \right) \left( \int^\bullet |\mathbf{f}'(t')| d\mu'(t') \right)
$$

by virtue of Prop. 8. This shows that $[\mathbf{f}(t) \cdot \mathbf{f}'(t')]$ is essentially integrable for $\mu \otimes \mu'$ (§ 1, No. 3, Prop. 9). Suppose that $\mathbf{f}$ and $\mathbf{f}'$ are integrable: then $\mathbf{f}$ and $\mathbf{f}'$ are moderated, and $\mathbf{g}$ is moderated (Cor. 2 of Prop. 5) therefore integrable (§ 1, No. 3, Cor. of Prop. 9). In this case the formula (14) follows from the Lebesgue–Fubini theorem and the linearity of the integral (Ch. IV, § 4, No. 2, Th. 1). To complete the treatment of the case that $\mathbf{f}$ and $\mathbf{f}'$ are essentially integrable, one then applies (14) to two integrable functions $\mathbf{f}_1$ and $\mathbf{f}_1'$, equal locally almost everywhere to $\mathbf{f}$ and $\mathbf{f}'$, on observing that $[\mathbf{f} \cdot \mathbf{f}'] = [\mathbf{f}_1 \cdot \mathbf{f}_1']$ locally almost everywhere in $T \times T'$ (Prop. 4).

This result extends to the product of complex measures.

### 5. Operations on the product of two measures

#### Proposition 10 {#int-v-s8-prop-10 .statement}

— Let $g$ (resp. $g'$) be a complex function (or a function with values in $\overline{\mathbf{R}}$) defined on $T$ (resp. $T'$).
a) If $g$ (resp. $g'$) is locally integrable for $\mu$ (resp. $\mu'$), then the function $g \otimes g': (t, t') \mapsto g(t)g'(t')$ is locally integrable for $\nu = \mu \otimes \mu'$, and

$$
(g \cdot \mu) \otimes (g' \cdot \mu') = (g \otimes g') \cdot (\mu \otimes \mu').
$$

b) Conversely, if $g \otimes g'$ is locally $\nu$-integrable, and if $g'$ is not locally $\mu'$-negligible, then $g$ is locally $\mu$-integrable.

a) Let $K$ and $K'$ be two compact subsets of $T$ and $T'$, respectively; Cor. 2 of Prop. 8 shows that the function $(t, t') \mapsto g(t)g'(t')\varphi_{K \times K'}(t, t')$, equal to $(g\varphi_K) \otimes (g'\varphi_{K'})$, is $\nu$-integrable. Consequently, $g \otimes g'$ is locally $\nu$-integrable. One then verifies immediately that the second member of (15) satisfies the characteristic property of product measures (Ch. III, § 4, No. 1, Th. 1).

b) Now suppose that $g \otimes g'$ is locally $\nu$-integrable, and that $g'$ is not locally $\mu'$-negligible. Let $\mu_1$ be a positive measure with compact support such that $\mu_1 \leq \mu$; $g \otimes g'$ being $(\mu_1 \otimes \mu')$-measurable, $t \mapsto g(t)g'(t')$ is $\mu_1$-measurable except for a locally $\mu'$-negligible set of values of $t'$ (Prop. 2).

Since $g'$ is not zero locally $\mu'$-almost everywhere, from this we deduce that that $g$ is $\mu_1$-measurable, then $\mu$-measurable on decomposing $\mu$ into a sum of a family of measures with compact support (§ 2, No. 3, Prop. 4 and § 2, No. 2, Prop. 2). Having established this point, we may reduce to the case that $g$ and $g'$ are $\geqslant 0$, on replacing $g$ and $g'$ by their absolute values if necessary. Let $K$ be any compact subset of $T$, and let $K'$ be a compact subset of $T'$ such that $\int g' \varphi_{K'} d\mu' \neq 0$. By Prop. 8,

$$
\left( \int^\bullet g \varphi_K d\mu \right) \left( \int^\bullet g' \varphi_{K'} d\mu' \right) = \iiint^\bullet (g \otimes g') \varphi_{K \times K'} d\mu d\mu' < +\infty .
$$

The first factor of the first member is therefore finite, and this completes the proof.

This proposition extends to complex measures, thanks to Prop. 3 of Ch. III, § 4, No. 2.

#### Proposition 11 {#int-v-s8-prop-11 .statement}

*Let $\pi$ (resp. $\pi'$) be a mapping of $T$ (resp. $T'$) into a locally compact space $T_1$ (resp. $T'_1$).*

a) *If $\pi$ (resp. $\pi'$) is $\mu$-proper (resp. $\mu'$-proper), then the mapping $\pi \times \pi'$ is $(\mu \otimes \mu')$-proper and $(\pi \times \pi')(\mu \otimes \mu') = \pi(\mu) \otimes \pi'(\mu')$.*

b) *Conversely, if $\pi \times \pi'$ is $(\mu \otimes \mu')$-proper and $\mu' \neq 0$, then $\pi$ is $\mu$-proper.*

a) For, $\pi \times \pi'$ is $(\mu \times \mu')$-measurable by Cor. 1 of Prop. 3 of No. 2. On the other hand, if $K$ (resp. $K'$) is a compact subset of $T_1$ (resp. $T'_1$), then $\pi^{-1}(K)$ and ${\pi'}^{-1}(K')$ are essentially integrable for $\mu$ and $\mu'$, respectively, therefore $\pi^{-1}(K) \times {\pi'}^{-1}(K')$ is essentially integrable for $\mu \otimes \mu'$ (Cor. 2 of Prop. 8). This proves that $\pi \times \pi'$ is $(\mu \times \mu')$-proper. Now let $\mu_1 = \pi(\mu)$, $\mu'_1 = \pi'(\mu')$, $\nu_1 = (\pi \times \pi')(\mu \otimes \mu')$; for $f \in \mathcal{K}(T_1)$ and $f' \in \mathcal{K}(T'_1)$, we have

$$
\iint f(\pi(t)) f'(\pi'(t')) d\mu(t) d\mu'(t')
$$
$$
= \left( \int f(\pi(t)) d\mu(t) \right) \left( \int f'(\pi'(t')) d\mu'(t') \right)
$$

(Cor. 2 of Prop. 8), which proves that $\nu_1 = \mu_1 \otimes \mu'_1$ (Ch. III, § 4, No. 1, Th. 1).

b) Now suppose that $\pi \times \pi'$ is $\mu \otimes \mu'$-proper and that $\mu' \neq 0$. Let $\mu_1$ be a measure $\leq \mu$ with compact support. The function $\pi \times \pi'$ being measurable for $\mu_1 \otimes \mu'$, the mapping $t \mapsto (\pi(t), \pi'(t'))$ is $\mu$-measurable except for $t'$ forming a locally $\mu'$-negligible set (No. 2, Prop. 2). Since $\mu' \neq 0$, it follows that $\pi$ is $\mu_1$-measurable, and finally that $\pi$ is $\mu$-measurable

(§2, No. 3, Prop. 4 and §2, No. 2, Prop. 2). It remains to show that $\mu^\bullet(f \circ \pi) < +\infty$ for every function $f \in \mathcal{K}_+(\mathrm{T}_1)$. If $\mu$ is zero, this property is obvious. If $\mu$ is not zero, then neither is $\mu \otimes \mu'$, consequently $(\pi \times \pi')(\mu \otimes \mu') \neq 0$ (§6, No. 2, Cor. 1 of Prop. 2). By Lemma 1 of Ch. III, §4, No. 1, there exist two functions $g \in \mathcal{K}_+(\mathrm{T}_1)$, $g' \in \mathcal{K}_+(\mathrm{T}'_1)$ such that

$$
\langle (\pi \times \pi')(\mu \otimes \mu'), g \otimes g' \rangle \neq 0.
$$

This expression being equal to $\langle \mu \otimes \mu', (g \circ \pi) \otimes (g' \circ \pi') \rangle$ by the definition of image measures, Prop. 8 implies that ${\mu''}^\bullet(g' \circ \pi') \neq 0$. We then have, by Prop. 8 and by Prop. 2 of §6, No. 2,

$$
\left( \int^\bullet (f \circ \pi) d\mu \right) \left( \int^\bullet (g' \circ \pi') d\mu' \right) = \iint^\bullet (f \circ \pi) \otimes (g' \circ \pi') d\mu d\mu'
$$
$$
= \iint^\bullet (f \otimes g') d((\pi \times \pi')(\mu \otimes \mu')) < +\infty.
$$

The first integral in the first member is therefore finite, which completes the proof.

This result extends at once to the product of two complex measures (apply the statement to their absolute values). The same is true for the following proposition.

#### Proposition 12 {#int-v-s8-prop-12 .statement}

— Let X (resp. X') be a locally compact subspace of T (resp. T'). Then, the induced measure $(\mu \otimes \mu')_{X \times X'}$ on the locally compact subspace $X \times X'$ of $T \times T'$ is equal to the product $\mu_X \otimes \mu'_{X'}$ of the measures induced on X and X' by $\mu$ and $\mu'$, respectively.

For, if $f \in \mathcal{K}(X)$ and $f' \in \mathcal{K}(X')$, then

$$
\iint_{X \times X'} f(t)f'(t') d\mu(t) d\mu'(t') = \left( \int_X f(t) d\mu(t) \right) \left( \int_{X'} f'(t') d\mu'(t') \right)
$$

by Cor. 2 of Prop. 8, which proves, by the definition of induced measures (Ch. IV, §5, No. 7) that

$$
(\mu \otimes \mu')_{X \times X'} = \mu_X \otimes \mu'_{X'}
$$

(Ch. III, §4, No. 1, Th. 1).

### 6. Integration with respect to a finite product of measures

The preceding results may be extended without difficulty to a product of a finite number of measures. For example, let $T_1, T_2, T_3$ be three locally compact spaces, $\mu_i$ a positive measure on $T_i$ ($i = 1, 2, 3$), and let ν = μ₁ ⊗ μ₂ ⊗ μ₃ be the product measure on T = T₁ × T₂ × T₃. Let f be a ν-integrable function with values in $\overline{\mathbf{R}}$ or in a Banach space; a first application of the Lebesgue–Fubini theorem shows that, except at points $(t₁, t₂) ∈ T₁ × T₂$ forming a negligible set (for $μ₁ ⊗ μ₂$), the function $t₃ ↦ f(t₁, t₂, t₃)$ is $μ₃$-integrable, the function

$$
(t₁, t₂) ↦ \int f(t₁, t₂, t₃) \, dμ₃(t₃),
$$

defined almost everywhere in $T₁ × T₂$, is $(μ₁ ⊗ μ₂)$-integrable, and

$$
\iiint f(t₁, t₂, t₃) \, dν(t₁, t₂, t₃) = \iint dμ₁(t₁) \, dμ₂(t₂) \int f(t₁, t₂, t₃) \, dμ₃(t₃).
$$

A second application of the same theorem shows that, for almost every $t₁ ∈ T₁$, the function $t₂ ↦ \int f(t₁, t₂, t₃) \, dμ₃(t₃)$ is defined almost everywhere in $T₂$ and is $μ₂$-integrable; moreover, the function

$$
t₁ ↦ \int dμ₂(t₂) \int f(t₁, t₂, t₃) \, dμ₃(t₃),
$$

defined almost everywhere in $T₁$, is $μ₁$-integrable, and

$$
\iiint f(t₁, t₂, t₃) \, dν(t₁, t₂, t₃) = \int dμ₁(t₁) \int dμ₂(t₂) \int f(t₁, t₂, t₃) \, dμ₃(t₃).
$$

One proves similarly that, for almost every $t₁ ∈ T₁$, the function $(t₂, t₃) ↦ f(t₁, t₂, t₃)$ is $(μ₂ ⊗ μ₃)$-integrable, that the function

$$
t₁ ↦ \iint f(t₁, t₂, t₃) \, dμ₂(t₂) \, dμ₃(t₃),
$$

defined almost everywhere, is $μ₁$-integrable, and that

$$
\iiint f(t₁, t₂, t₃) \, dν(t₁, t₂, t₃) = \int dμ₁(t₁) \iint f(t₁, t₂, t₃) \, dμ₂(t₂) \, dμ₃(t₃).
$$

We leave to the reader the task of generalizing in the same way the other results proved above for the product of two measures.

### 7. Application: Measure of the Euclidean ball in $\mathbf{R}^n$

Let $\mu$ be Lebesgue measure on $\mathbf{R}$, and $\mu_n$ Lebesgue measure on $\mathbf{R}^n$, the product of $n$ factors equal to $\mu$. We propose to calculate the measure $V_n = \mu_n(\mathbf{B}_n)$ of the Euclidean unit ball. By Cor. 2 of Prop. 7,

$$
V_n = \int_{-1}^{+1} \mu_{n-1}(\mathbf{B}_n(z_n)) dz_n .
$$

Now, the section $\mathbf{B}_n(z_n)$ is the subset of $\mathbf{R}^{n-1}$ defined by the relation $\sum_{i=1}^{n-1} z_i^2 \leq 1 - z_n^2$, in other words, it is the transform of the ball $\mathbf{B}_{n-1}$ by the homothety with ratio $\sqrt{1 - z_n^2}$. But it follows immediately from Prop. 11 and the formula

$$
\alpha \int_{-\infty}^{+\infty} f(\alpha x) dx = \int_{-\infty}^{+\infty} f(z) dz
$$

for $f \in \mathcal{K}(\mathbf{R})$, that the image of $\mu_{n-1}$ under the homothety $\mathbf{x} \mapsto \alpha \mathbf{x}$ is the measure $\alpha^{1-n} \mu_{n-1}$. Therefore

$$
\mu_{n-1}(\mathbf{B}_n(z_n)) = \left( \sqrt{1 - z_n^2} \right)^{n-1} V_{n-1} .
$$

Substitution in (16), and making the change of variable $z_n = \sin \varphi$ (with $-\frac{\pi}{2} \leq \varphi \leq \frac{\pi}{2}$), yields

$$
V_n = V_{n-1} \int_{-\frac{\pi}{2}}^{+\frac{\pi}{2}} \cos^n \varphi d\varphi = 2 V_{n-1} \int_0^{\frac{\pi}{2}} \cos^n \varphi d\varphi .
$$

But (FRV, Ch. VII, §1, No. 3, formula (20))

$$
\int_0^{\frac{\pi}{2}} \cos^m \varphi d\varphi = \frac{1}{2} \frac{\Gamma \left( \frac{1}{2} \right) \Gamma \left( \frac{m+1}{2} \right)}{\Gamma \left( \frac{m+2}{2} \right)}
$$

and on substituting in the relation (17) and taking into account the expression for $\Gamma \left( \frac{1}{2} \right)$ (FRV, VII, §1, No. 3, formula (21)), one obtains finally

$$
V_n = \frac{\pi^{n/2}}{\Gamma \left( \frac{n}{2} + 1 \right)} .
$$

Exercises

### Exercises {#int-v-s8-exercises}

See the [exercises for § 8](exercises/s8/).
