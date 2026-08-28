---
book: int
book_title: Integration
chapter: V
chapter_title: INTEGRATION OF MEASURES
section: 6
section_title: Images of a measure
lang: en
source: int-i-vi
book_pages: INT V.62-INT V.74, INT V.107-INT V.112
pdf_pages: 0317-0329, 0362-0367
extraction: ocr
subsections:
    - "no": 1
      title: Image of a positive measure
      page: 62
      pdf_page: 317
    - "no": 2
      title: Integration with respect to the image of a positive measure
      page: 64
      pdf_page: 319
    - "no": 3
      title: Properties of the image of a positive measure
      page: 65
      pdf_page: 320
    - "no": 4
      title: Image of a complex measure
      page: 68
      pdf_page: 323
    - "no": 5
      title: 'Application: change of variable in the Lebesgue integral'
      page: 69
      pdf_page: 324
    - "no": 6
      title: Decomposition into slices. Inverse image of a measure under a local homeomorphism
      page: 71
      pdf_page: 326
statements: 29
exercises: 22
content_sha256: a70560a7e81a1387fafead635105a8388c5e8d3f23436033725b34a2d8dcc990
---

## § 6. IMAGES OF A MEASURE

### 1. Image of a positive measure

Let $X$ be a locally compact space, $\pi$ a $\mu$-measurable mapping of $T$ into $X$. To say that the pair $(\pi, 1)$ is *$\mu$-adapted* (§4, No. 1) is equivalent to saying that for every function $f \in \mathcal{K}(X)$, the function $f \circ \pi$ is *essentially $\mu$-integrable*.

#### Proposition 1 {#int-v-s6-prop-1 .statement}

*Let $\pi$ be a $\mu$-measurable mapping of $T$ into a locally compact space $X$. The following two properties are equivalent:*

a) *for every function* $f \in \mathcal{K}(X)$, $f \circ \pi$ *is essentially* $\mu$-*integrable*.

b) *for every compact set* $K \subset X$, $\overline{\pi}^{-1}(K)$ *is essentially* $\mu$-*integrable*.

We have just observed that a) implies that the pair $(\pi, 1)$ is $\mu$-adapted. Consequently (§ 4, No. 4, Th. 2), for every compact set $K \subset X$, the function $\varphi_K \circ \pi = \varphi_A$, where $A = \overline{\pi}^{-1}(K)$, is essentially $\mu$-integrable, in other words, a) implies b).

Conversely, suppose that $\overline{\pi}^{-1}(K)$ is essentially $\mu$-integrable for every compact subset $K$ of $X$, and let us show that a) is verified. Indeed, let $S$ be the support of $f$; since $S$ is compact, setting $A = \overline{\pi}^{-1}(S)$ we have, by hypothesis,

$$
\int^\bullet |f(\pi(t))| \, d\mu(t) \leq \|f\| \int^\bullet \varphi_S(\pi(t)) \, d\mu(t) = \|f\| \int^\bullet \varphi_A(t) \, d\mu(t) < +\infty.
$$

Since $f \circ \pi$ is $\mu$-measurable (Ch. IV, § 5, No. 3, Th. 1), we see that $f \circ \pi$ is essentially $\mu$-integrable (§ 1, No. 3, Prop. 9).

Property b) is obviously equivalent to the following (which is therefore also equivalent to a)):

c) *For every point* $x$ *of* $X$, *there exists a neighborhood* $V$ *of* $x$ *such that* $\overline{\pi}^{-1}(V)$ *is essentially* $\mu$-*integrable*.

#### Definition 1 {#int-v-s6-def-1 .statement}

*Let* $\mu$ *be a positive measure on a locally compact space* $T$. *A mapping* $\pi$ *of* $T$ *into a locally compact space* $X$ *is said to be* $\mu$*-proper* (*or proper for the measure* $\mu$) *if the pair* $(\pi, 1)$ *is* $\mu$*-adapted*, *that is* (§ 4, No. 1), *if* $\pi$ *is* $\mu$*-measurable and satisfies the (equivalent) conditions of Prop. 1*. *The measure* $\int \varepsilon_{\pi(t)} \, d\mu(t)$ *on* $X$ *is then called the image of* $\mu$ *under* $\pi$ *and is denoted* $\pi(\mu)$.

Thus if $\nu = \pi(\mu)$ then, by definition, for $f \in \mathcal{K}(X)$ one has

$$
\int f(x) \, d\nu(x) = \int f(\pi(t)) \, d\mu(t).
$$

#### Remark {#int-v-s6-n1-rem-1 .statement}

— 1) If $\mu$ is *bounded* (in particular, if $\mu$ has compact support) then every $\mu$-measurable mapping of $T$ into $X$ is $\mu$-proper (Ch. IV, § 5, No. 3, Th. 1 and No. 6, Th. 5).

2) If $\pi$ is $\mu$-measurable and if, for every compact subset $K$ of $X$, $\overline{\pi}^{-1}(K)$ is relatively compact, then $\pi$ is $\mu$-proper (Ch. IV, § 5, No. 5, Prop. 7 and No. 6, Th. 5); in particular, every *proper* continuous mapping of $T$ into $X$ (GT, I, § 10, No. 2, Th. 1) is $\mu$-proper for every positive measure $\mu$ on $T$. More particularly, this is true of every *homeomorphism* $\pi$ of $T$ onto X; the measure $\nu = \pi(\mu)$ is then none other than the measure on X that is the transport of $\mu$ by $\pi$ (Ch. III, §1, No. 3).

3) Suppose that the topology of X admits a countable base; then every mapping $\pi$ of T into X that satisfies condition b) of Prop. 1 is $\mu$-measurable, hence is $\mu$-proper. It suffices to apply Th. 4 of Ch. IV, §5, No. 5, on observing that X is then metrizable (GT, IX, §2, No. 9, Cor. of Prop. 16) and that, for any metric compatible with the topology of X, every closed ball is a countable union of compact sets.

### 2. Integration with respect to the image of a positive measure

Let $\pi$ be a $\mu$-proper mapping of T into X, and let $\nu = \pi(\mu)$. Applying the results of §4, one obtains the following statements:

#### Proposition 2 {#int-v-s6-prop-2 .statement}

— *For every numerical function* $f \geqslant 0$ *defined on* X,
$$
\int^\bullet f(x)\, d\nu(x) = \int^\bullet f(\pi(t))\, d\mu(t).
$$
(2)

This follows from Th. 1 of §4, No. 2.

#### Corollary 1 {#int-v-s6-prop-2-cor-1 .statement}

— *For every subset* A *of* X,
$$
\nu^\bullet(A) = \mu^\bullet(\pi^{-1}(A)).
$$

#### Corollary 2 {#int-v-s6-prop-2-cor-2 .statement}

— *For a subset* A *of* X *to be locally negligible for* $\nu$, *it is necessary and sufficient that* $\pi^{-1}(A)$ *be locally negligible for* $\mu$.

#### Corollary 3 {#int-v-s6-prop-2-cor-3 .statement}

— *If the measure* $\mu$ *is concentrated on a set* M, *then* $\pi(\mu)$ *is concentrated on* $\pi(M)$.

For, if $N = X - \pi(M)$ then $\pi^{-1}(N)$ does not intersect M, therefore is locally $\mu$-negligible, consequently (Cor. 2) N is locally $\nu$-negligible.

#### Corollary 4 {#int-v-s6-prop-2-cor-4 .statement}

— *Let* S *be the support of* $\mu$. *If* $\pi$ *is continuous, then the support of* $\pi(\mu)$ *is* $\pi(S)$.

For, it follows from Cor. 3 that $\pi(\mu)$ is concentrated on $\pi(S)$, therefore if $S'$ is the support of $\pi(\mu)$ then $S' \subset \pi(S)$. On the other hand, $\pi^{-1}(X - S')$ is a locally $\mu$-negligible open set (Cor. 2), hence is $\mu$-negligible (Ch. IV, §5, No. 2, Cor. 2 of Prop. 5). Therefore $\pi^{-1}(X - S') \subset T - S$, consequently $\pi(S) \subset S'$, which proves the corollary.

#### Proposition 3 {#int-v-s6-prop-3 .statement}

— *For a mapping* f *of* X *into a topological space* G *to be* $\nu$*-measurable, it is necessary and sufficient that* $f \circ \pi$ *be* $\mu$*-measurable.*

This is an immediate consequence of Prop. 3 of §4, No. 3.

#### Corollary {#int-v-s6-n2-cor-1 .statement}

— For a subset A of X to be $\nu$-measurable, is is necessary and sufficient that $\pi^{-1}(A)$ be $\mu$-measurable.

However, the image under $\pi$ of a $\mu$-measurable subset M of T is not necessarily $\nu$-measurable, even if $\pi$ is continuous and M is $\mu$-negligible (Exer. 7 and §8, Exer. 1).

#### Theorem 1 {#int-v-s6-thm-1 .statement}

— Let f be a function defined on X with values in $\overline{\mathbf{R}}$ or in a Banach space F. For f to be essentially $\nu$-integrable, it is necessary and sufficient that $f \circ \pi$ be essentially $\mu$-integrable, in which case

$$
\int f(x)\, d\nu(x) = \int f(\pi(t))\, d\mu(t).
$$

Suppose, moreover, that $\pi$ is continuous and proper. Then, for f to be $\nu$-integrable, it is necessary and sufficient that $f \circ \pi$ be $\mu$-integrable.

It suffices to apply Th. 2 of §4, No. 4.

#### Corollary {#int-v-s6-n2-cor-2 .statement}

— For a subset A of X to be essentially $\nu$-integrable, it is necessary and sufficient that $\pi^{-1}(A)$ be essentially $\mu$-integrable, in which case $\nu(A) = \mu(\pi^{-1}(A))$.

In particular, for every compact set $K \subset X$, $\nu(K) = \mu(\pi^{-1}(K))$. It follows from this and Cor. 3 of Prop. 2 that if $\mu$ is atomic (§ 5, No. 10) then so is $\pi(\mu) = \nu$. For, let M be the set of $t \in T$ such that $\mu(\{t\}) \neq 0$; since $\mu$ is carried by M, $\nu$ is carried by $\pi(M)$; moreover, for every $x \in \pi(M)$ we have $\nu(\{x\}) = \mu(\pi^{-1}(x)) > 0$, since $\pi^{-1}(x)$ contains at least one point of M. Therefore $\nu$ is atomic (§ 5, No. 10, Prop. 15).

### 3. Properties of the image of a positive measure

#### Proposition 4 {#int-v-s6-prop-4 .statement}

— Let T, T', T'' be three locally compact spaces, $\mu$ a positive measure on T, $\pi$ a $\mu$-measurable mapping of T into T', $\pi'$ a mapping of T' into T'', and $\pi'' = \pi' \circ \pi$.

a) Suppose that $\pi$ is $\mu$-proper and let $\mu' = \pi(\mu)$. For $\pi'$ to be $\mu'$-proper, it is necessary and sufficient that $\pi''$ be $\mu$-proper, in which case $\pi''(\mu) = \pi'(\pi(\mu))$ ('transitivity of the image of a measure').

b) Suppose that $\pi'$ is continuous, and that $\pi''$ is $\mu$-proper; then $\pi$ is $\mu$-proper, $\pi'$ is $\pi(\mu)$-proper and $\pi''(\mu) = \pi'(\pi(\mu))$.

Under the hypotheses of a), for $\pi''$ to be $\mu$-measurable it is necessary and sufficient that $\pi'$ be $\mu'$-measurable (No. 2, Prop. 3). On the other hand if $K$ is a compact subset of $T''$, then $\pi''(K) = \pi^{-1}(\pi'(K))$; for $\pi''(K)$ to be essentially $\mu$-integrable, it is necessary and sufficient that $\pi'(K)$ be essentially $\mu'$-integrable, by the Cor. of Th. 1. Finally, if $\pi''$ is $\mu$-proper then, setting $\mu'' = \pi''(\mu)$, we have, for every function $f \in \mathcal{H}(T'')$,

$$
\int f(t'')\, d\mu''(t'') = \int f(\pi''(t))\, d\mu(t)
$$
$$
= \int f\left(\pi'\left(\pi(t)\right)\right)\, d\mu(t) = \int f(\pi'(t'))\, d\mu'(t')
$$

by Th. 1 of No. 2, which completes the proof of a).

Under the hypotheses of b), let $K'$ be a compact subset of $T'$. Then $K'' = \pi'(K')$ is compact, therefore $\pi''(K'')$ is essentially $\mu$-integrable, therefore $\pi^{-1}(K') \subset \pi''(K'')$ is essentially $\mu$-integrable (Ch. IV, §5, No. 5, Prop. 7), so that $\pi$ is $\mu$-proper. The proof is then concluded by applying part a) of the statement.

#### Corollary {#int-v-s6-n3-cor-1 .statement}

*Let $T$ and $T'$ be two locally compact spaces, $\mu$ a positive measure on $T$, $\pi$ a bijective mapping of $T$ onto $T'$, and $\pi^{-1}$ the inverse mapping. Suppose that $\pi$ is $\mu$-proper, and let $\mu' = \pi(\mu)$. Then $\pi^{-1}$ is $\mu'$-proper and $\pi^{-1}(\pi(\mu)) = \mu$.*

#### Proposition 5 {#int-v-s6-prop-5 .statement}

*Let $T$ and $X$ be two locally compact spaces, $\mu$ a positive measure on $T$, $\pi$ a $\mu$-proper mapping of $T$ into $X$, $g$ a finite numerical function $\geqslant 0$, defined on $X$ and such that $g \circ \pi$ is locally integrable for $\mu$. In order that $g$ be locally integrable for $\pi(\mu)$, it is necessary and sufficient that $\pi$ be proper for the measure $(g \circ \pi) \cdot \mu$, in which case*

$$
\pi((g \circ \pi) \cdot \mu) = g \cdot \pi(\mu).
$$

Set $\nu = \pi(\mu)$. For $g$ to be locally $\nu$-integrable, it is necessary and sufficient that $gf$ be $\nu$-integrable for every function $f \in \mathcal{H}(X)$; since $gf$ has compact support, it comes to the same to say that $gf$ is essentially $\nu$-integrable, and this is equivalent to saying that $(g \circ \pi)(f \circ \pi)$ is essentially $\mu$-integrable (Th. 1). But, by Th. 1 of §5, No. 3, this signifies that $f \circ \pi$ is essentially integrable for $\rho = (g \circ \pi) \cdot \mu$, and, by definition, this says that $\pi$ is $\rho$-proper (since $\pi$ is obviously $\rho$-measurable). Moreover,

$$
\int fg\, d\nu = \int f(\pi(t))g(\pi(t))\, d\mu(t) = \int f(\pi(t))\, d\rho(t)
$$

(No. 2, Th. 1 and §5, Th. 1), which proves the relation (4).

#### Proposition 6 {#int-v-s6-prop-6 .statement}

— Let T and X be two locally compact spaces, $(\lambda_\alpha)_{\alpha \in A}$ a family of positive measures on T, directed for the relation $\leq$, admitting in $\mathcal{M}(T)$ a supremum $\mu$. In order that a mapping $\pi$ of T into X be $\mu$-proper, it is necessary and sufficient that it be $\lambda_\alpha$-proper for all $\alpha \in A$, and that the family $(\pi(\lambda_\alpha))_{\alpha \in A}$ be bounded above in $\mathcal{M}(X)$. In this case,

$$
\pi(\mu) = \sup_\alpha \pi(\lambda_\alpha).
$$

For $\pi$ to be $\mu$-measurable, it is necessary and sufficient that $\pi$ be $\lambda_\alpha$-measurable for all $\alpha \in A$ (§ 1, No. 4, Cor. 2 of Prop. 11). Suppose that this condition is satisfied; to say that $\pi$ is $\mu$-proper is then equivalent to saying that, for every function $f \in \mathcal{K}_+(X)$,

$$
\mu^\bullet(f \circ \pi) < +\infty.
$$

Now,

$$
\int^\bullet (f \circ \pi)\, d\mu = \sup_\alpha \int^\bullet (f \circ \pi)\, d\lambda_\alpha = \sup_\alpha \int^\bullet f\, d(\pi(\lambda_\alpha))
$$

(§ 1, No. 4, Prop. 11); the first member is thus finite for every $f \in \mathcal{K}_+(X)$ if and only if the family $(\pi(\lambda_\alpha))$ admits a supremum $\theta$ in $\mathcal{M}(X)$, in which case $\int (f \circ \pi)\, d\mu = \int f\, d\theta$, a relation equivalent to (5).

#### Corollary 1 {#int-v-s6-prop-6-cor-1 .statement}

— Let $(\mu_\alpha)_{\alpha \in A}$ be a summable family of positive measures on T, such that $\mu = \sum_{\alpha \in A} \mu_\alpha$; for a mapping $\pi$ of T into a locally compact space X to be $\mu$-proper, it is necessary and sufficient that it be $\mu_\alpha$-proper for every $\alpha \in A$, and that the family $(\pi(\mu_\alpha))_{\alpha \in A}$ be summable. In this case,

$$
\pi(\mu) = \sum_{\alpha \in A} \pi(\mu_\alpha).
$$

#### Corollary 2 {#int-v-s6-prop-6-cor-2 .statement}

— Let T and X be two locally compact spaces, $(\lambda_i)_{1 \leq i \leq n}$ a finite sequence of positive measures on T, and let $\mu = \sum_{i=1}^n \lambda_i$. For a mapping $\pi$ of T into X to be $\mu$-proper, it is necessary and sufficient that it be $\lambda_i$-proper for every index i, in which case

$$
\sum_{i=1}^n \pi(\lambda_i) = \pi\left( \sum_{i=1}^n \lambda_i \right).
$$

### 4. Image of a complex measure

Let $\theta$ be a complex measure on $T$, and let $\pi$ be a mapping of $T$ into a locally compact space $X$; suppose that $\pi$ is $\theta$-measurable, and that for each $f \in \mathcal{K}(X; \mathbf{C})$, $f \circ \pi$ is essentially $\theta$-integrable. Since it is equivalent to say that a function is measurable (resp. essentially integrable) with respect to $\theta$ or with respect to $|\theta|$, this means that $\pi$ is $|\theta|$-proper. If $f \in \mathcal{K}(X; \mathbf{C})$,

$$
\left| \int (f \circ \pi) \, d\theta \right| \leq \int (|f| \circ \pi) \, d|\theta| ;
$$

it follows at once that the linear form $f \mapsto \int (f \circ \pi) \, d\theta$ on $\mathcal{K}(X; \mathbf{C})$ is a *complex measure* on $X$ (Ch. III, §1, No. 3, Prop. 6), and one can make the following definition:

#### Definition 2 {#int-v-s6-def-2 .statement}

*Let $\theta$ be a complex measure on a locally compact space $T$. A mapping $\pi$ of $T$ into a locally compact space $X$ is said to be $\theta$-proper if it is $|\theta|$-proper. The measure $f \mapsto \int (f \circ \pi) \, d\theta$ is then called the image of $\theta$ under $\pi$ and is denoted $\pi(\theta)$.*.

The relation (7) may then be put in the following form:

$$
|\pi(\theta)| \leq \pi(|\theta|) .
$$

The measure $\pi(\theta)$ may be zero without $\theta$ being zero, as one sees immediately on taking for $T$ a space reduced to two points $a, b$, for $\theta$ the measure $\varepsilon_a - \varepsilon_b$, and for $\pi$ a constant mapping.

Let $\theta$ and $\theta'$ be two complex measures on $T$; if $\pi$ is $\theta$-proper and $\theta'$-proper, it follows from Cor. 2 of Prop. 6 that $\pi$ is $(\theta + \theta')$-proper since $|\theta + \theta'| \leq |\theta| + |\theta'|$, and obviously $\pi(\theta + \theta') = \pi(\theta) + \pi(\theta')$.

In particular, if $\theta$ is a real measure and $\pi$ is $\theta$-proper, then

$$
\pi(\theta) = \pi(\theta^+) - \pi(\theta^-) .
$$

Several results established earlier extend at once to complex measures; we cite the most important among them.

#### Proposition 7 {#int-v-s6-prop-7 .statement}

*Let $\theta$ be a complex measure on $T$, $\pi$ a $\theta$-proper mapping of $T$ into a locally compact space $X$, $\nu$ the image measure $\pi(\theta)$.

a) Let $A$ be a subset of $X$; if $\overline{\pi^{-1}}(A)$ is locally $\theta$-negligible, then $A$ is locally $\nu$-negligible.

b) Let $f$ be a mapping of $X$ into a topological space; if $f \circ \pi$ is $\theta$-measurable, then $f$ is $\nu$-measurable.*

c) Let $f$ be a function defined on $X$, with values in a Banach space $F$; if $f \circ \pi$ is essentially $\theta$-integrable, then $f$ is essentially $\nu$-integrable and

$$
\int f(\pi(t))\ d\theta(t) = \int f(x)\ d\nu(x).
$$

Taking into account formula (8), these results may be deduced from Cor. 2 of Prop. 2, from Prop. 3, and from Th. 1 of No. 2.

### 5. Application: change of variable in the Lebesgue integral

Let I be an interval (bounded or not) of $\mathbf{R}$, $a$ its left end-point and $b$ its right end-point in $\overline{\mathbf{R}}$, and $\mu$ the Lebesgue measure on I. For every $\mu$-integrable function $f$ and every interval $H \subset I$, with left end-point $\alpha$ and right end-point $\beta$, we write $\int_{\alpha}^{\beta} f(t)\ dt$ instead of $\int_H f(t)\ dt = \int_H f\ d\mu$, and we set $\int_{\beta}^{\alpha} f(t)\ dt = -\int_{\alpha}^{\beta} f(t)\ dt$; the meaning thus given to these symbols coincides with that attributed to them in FRV, II, §§1 and 2, when $f$ is a regulated function with compact support (Ch. IV, §4, No. 4, Example).

Let $g$ be a numerical function defined on I and *locally $\mu$*-integrable, $x_0$ a point of I; for every $x \in I$, set

$$
G(x) = c + \int_{x_0}^{x} g(t)\ dt \quad (c \text{ a constant}).
$$

The numerical function G is *continuous* on I; this follows at once from Lebesgue’s theorem (Ch. IV, §4, No. 3, Cor. 1 of Th. 2), since the product of $g$ and the characteristic function of the interval with end-points $x$ and $x+h$ tends to a negligible function as $h$ tends to 0. Therefore G(I) is an *interval* of $\mathbf{R}$. Throughout this No., we will regard G as a mapping of I onto the locally compact space G(I). We denote by $\lambda$ the measure $g \cdot \mu$ on I.

Suppose first that $g$ is $\mu$*-integrable*. Then, the same reasoning as above shows that the limits $G(a+)$ and $G(b-)$ exist and are *finite*; moreover, the measure $|\lambda|$ is *bounded* (§5, No. 3, Cor. of Th. 1), and the mapping G of I into G(I) is *$\lambda$*-proper.

#### Proposition 8 {#int-v-s6-prop-8 .statement}

*Suppose g is $\mu$*-integrable. If J denotes the open interval in $\mathbf{R}$ with end-points $G(a+)$ and $G(b-)$, the image under G of the measure $g \cdot \mu$ is the measure $\varphi_J \cdot \nu$ if $G(a+) \leq G(b-)$ and the measure $-\varphi_J \cdot \nu$ if $G(a+) \geq G(b-)$ (where $\nu$ denotes Lebesgue measure on G(I)).*

It suffices to prove that, for every function $f \in \mathcal{K}(G(I))$,

$$
\int_{G(a+)}^{G(b-)} f(\xi) d\xi = \int_a^b f(G(t))g(t)\,dt.
$$

Now, this formula has already been proved for $g \in \mathcal{K}(I)$ (FRV, II, §2, No. 1, formula (1)). Let us pass to the general case; there exists a sequence $(g_n)$ of functions in $\mathcal{K}(I)$ such that: $1^\circ$ the sequence $(g_n(t))$ tends to $g(t)$ almost everywhere in $I$; $2^\circ$ there exists a $\mu$-integrable function $h \geq 0$ such that $|g_n| \leq h$ for all $n$ (Ch. IV, §3, No. 4, Th. 3). It follows at once from Lebesgue’s theorem that, setting $G_n(x) = c + \int_{x_0}^x g_n(t)\,dt$, the sequence $(G_n)$ converges uniformly to $G$ on $I$, and that the numbers $G_n(a+)$ and $G_n(b-)$ tend respectively to $G(a+)$ and $G(b-)$. Let $f'$ be a function in $\mathcal{K}(\mathbf{R})$ that extends $f$; the foregoing proves that $f'(G_n(t))$ tends to $f'(G(t)) = f(G(t))$ for all $t \in I$; applying Lebesgue’s theorem, one sees that the formula (12) results from the formula

$$
\int_{G_n(a+)}^{G_n(b-)} f'(\xi)\,d\xi = \int_a^b f'(G_n(t))g_n(t)\,dt
$$

by passage to the limit.

#### Corollary {#int-v-s6-n5-cor-1 .statement}

*If a function $\mathbf{f}$ defined on $G(I)$, with values in $\overline{\mathbf{R}}$ or in a Banach space, is such that the function $t \mapsto \mathbf{f}(G(t))g(t)$ is integrable on $I$ for Lebesgue measure, then $\mathbf{f}$ is integrable on $J$ for Lebesgue measure and*

$$
\int_{G(a+)}^{G(b-)} \mathbf{f}(\xi)\,d\xi = \int_a^b \mathbf{f}(G(t))g(t)\,dt
$$

(formula for change of variable in the Lebesgue integral).

For, $\mathbf{f}(G(t))$ is integrable for the measure $|g|\cdot\mu$, hence also for the measures $g^+\cdot\mu$ and $g^-\cdot\mu$; it follows from Th. 1 (No. 2) that $\mathbf{f}$ is integrable for the image measures $G(g^+\cdot\mu)$ and $G(g^-\cdot\mu)$, hence also for the measure $\varphi_J \cdot \nu$, and that (13) holds, on taking into account Prop. 8 and formula (9).

It can happen that $\mathbf{f}$ is integrable on $J$ for Lebesgue measure, but that $t \mapsto \mathbf{f}(G(t))g(t)$ is not integrable on $I$ for Lebesgue measure (Exer. 10).

Now suppose that $g$ maintains a *constant sign* almost everywhere (and is locally $\mu$-integrable); one may suppose for example that $g(t) \geq 0$ almost everywhere in $I$. Then $G$ is an increasing continuous function on $I$, therefore $G(a+)$ and $G(b-)$ exist (but may be infinite). Moreover, $G$ is a *$\lambda$-proper* mapping of $I$ into $G(I)$: for, if $G(b-) \in G(I)$, there is an x_1 \geq x_0 \text{ such that } G \text{ is constant for } x \geq x_1, \text{ and then the inverse image under } G \text{ of the compact interval } [G(x_0), G(b-)] \text{ is } \lambda\text{-integrable; if, on the contrary, } G(b-) \notin G(I), \text{ then the inverse image under } G \text{ of every compact interval with left end-point } G(x_0), \text{ contained in } G(I), \text{ differs from a compact interval by at most a } \lambda\text{-negligible interval. One argues similarly for the compact intervals with right end-point } G(x_0), \text{ whence our assertion. Moreover:}

#### Proposition 9 {#int-v-s6-prop-9 .statement}

*Suppose $g \geq 0$ and locally $\mu$-integrable. Then, the image under $G$ of the positive measure $g \cdot \mu$ is Lebesgue measure on $G(I)$. For a function $f$, defined on $G(I)$, with values in $\overline{\mathbf{R}}$ or in a Banach space, to be integrable on $G(I)$ for Lebesgue measure, it is necessary and sufficient that the function $t \mapsto f(G(t))g(t)$ be integrable on $I$ for Lebesgue measure, in which case the relation (13) holds.*

The first part of the statement follows from the fact that the formula (12) is valid for every function $f \in \mathcal{K}(G(I))$; for, the support of the function $t \mapsto f(G(t))$ is contained in an interval $K \subset I$ on which $g$ is integrable, by virtue of the above remarks, and it suffices to apply Prop. 8 to $K$. The second part is a consequence of Th. 1 of No. 2.

### 6. Decomposition into slices. Inverse image of a measure under a local homeomorphism

Let $X$ be a locally compact space, $\pi$ a mapping of $X$ into a locally compact space $T$, $\mu$ a positive measure on $T$, $\Lambda : t \mapsto \lambda_t$ a scalarly essentially $\mu$-integrable and vaguely $\mu$-measurable mapping of $T$ into $\mathcal{M}_+(X)$. Let $\nu = \int \lambda_t d\mu(t)$. If $\lambda_t$ is *carried by* $\overline{\pi}^{-1}(t)$ for every $t \in T$, the equality $\nu = \int \lambda_t d\mu(t)$ is said to be a *decomposition into slices* (or a *disintegration*) of $\nu$ relative to $\pi$. This concept will be studied in detail in Ch. VI.

#### Proposition 10 {#int-v-s6-prop-10 .statement}

*With the above notations, suppose that $\pi$ is $\nu$-measurable. Let $g$ be the function $t \mapsto \lambda_t^*(1)$ on $T$. For $\pi$ to be $\nu$-proper, it is necessary and sufficient that $g$ be locally $\mu$-integrable, in which case*

$$
\pi(\nu) = g \cdot \mu.
$$

We begin by arguing on the assumption that $g$ is finite locally $\mu$-almost everywhere; we will rid ourselves of this auxiliary hypothesis at the end of the proof. Since $\pi$ is by hypothesis $\nu$-measurable, to say that $\pi$ is $\nu$-proper is equivalent to saying that $\nu^*(f \circ \pi) < +\infty$ for every function $f \in \mathcal{K}_+(T)$; $g$ being finite locally almost everywhere, we are under the conditions for applying assertion c) of Prop. 5 of §3, No. 2. Therefore

$$
\int^\bullet (f \circ \pi)\, d\nu = \int^\bullet d\mu(t) \int^\bullet (f \circ \pi)\, d\lambda_t = \int^\bullet f(t)g(t)\, d\mu(t),
$$

from the fact that $\lambda_t$ is concentrated on $\overline{\pi}^{-1}(t)$. We know that $g$ is $\mu$-measurable, since $\Lambda$ is $\mu$-adequate (§ 3, No. 1, Def. 1). To say that the first member is finite for every $f \in \mathcal{K}_+(T)$ is therefore equivalent to saying that $g$ is locally $\mu$-integrable (§ 5, Prop. 1), and in this case (14) follows at once from the above relations.

It therefore only remains to eliminate the auxiliary hypothesis. If $g$ is locally $\mu$-integrable, then $g$ is finite locally $\mu$-almost everywhere, and the hypothesis is indeed satisfied. Let us assume that $\pi$ is $\nu$-proper, and let us show that $g$ is finite locally almost everywhere. Let $\mathfrak{K}$ be the $\mu$-dense set of compact sets $K$ such that $\Lambda|K$ is vaguely continuous; since $g$ is measurable, we are reduced to showing that every compact set $K \in \mathfrak{K}$ such that $g|K = +\infty$ is $\mu$-negligible. Now, let $\mathcal{H}$ be the set of functions $h \in \mathcal{K}_+(X)$ such that $h \leq 1$; set $g_h(t) = \lambda_t(h)$, denote by $\Lambda_h$ the $\mu$-adequate mapping $t \mapsto h \cdot \lambda_t$, by $\nu_h$ the integral of $\Lambda_h$, and by $f$ an element of $\mathcal{K}_+(T)$ such that $f \geq \varphi_K$. Applying formula (14) to $\Lambda_h$, which does satisfy the auxiliary hypothesis, we obtain:

$$
\int (f \circ \pi)\, d\nu \geq \int (f \circ \pi)\, d\nu_h = \int fg_h\, d\mu.
$$

But the functions $fg_h|K$ form an increasing directed set of continuous functions on $K$, whose upper envelope has the value $+\infty$; by Dini’s theorem (GT, X, §4, No. 1, Th. 1), one can choose $h$ so that $fg_h|K$ is greater than or equal to an arbitrary positive number $n$, and it follows that $\int (f \circ \pi)\, d\nu \geq n\, \mu(K)$. Since the first member is finite because $\pi$ is $\nu$-proper, it then follows that $\mu(K) = 0$.

#### Corollary 1 {#int-v-s6-prop-10-cor-1 .statement}

— *Suppose that $\pi$ is $\nu$-measurable.*

a) *If $N \subset T$ is locally $\mu$-negligible, then $\overline{\pi}^{-1}(N)$ is locally $\nu$-negligible.*
b) *If $f$ is a $\mu$-measurable mapping of $T$ into a topological space $G$, then $f \circ \pi$ is $\nu$-measurable.*

We take up again the notations $\Lambda_h$, $\nu_h$, $g_h$ of the end of the preceding proof: $\nu_h$ being a bounded measure for every $h \in \mathcal{H}$, $\pi$ is $\nu_h$-proper, $g_h$ is locally $\mu$-integrable, and $\pi(\nu_h) = g_h \cdot \mu$, a measure with base $\mu$. It follows that $N$ is locally negligible (resp. that $f$ is measurable) for the measure $\pi(\nu_h)$ (§ 5, No. 3, Cor. 1 of Prop. 3 and Prop. 4). Consequently $\overline{\pi}^{-1}(N)$ is locally negligible (resp. $f \circ \pi$ is measurable) for the measure $\nu_h$ (Cor. 2 of

Prop. 2, resp. Prop. 3). Finally, one notes that the measures $\nu_h$ form an increasing directed family of positive measures whose supremum is $\nu$, and one applies Cor. 1 (resp. Cor. 2) of Prop. 11 of §1, No. 4.

#### Corollary 2 {#int-v-s6-prop-10-cor-2 .statement}

*Suppose that $\pi$ is $\nu$-proper; let $f$ be a mapping defined on $T$, with values in a Banach space or in $\overline{\mathbf{R}}$. For $f \circ \pi$ to be essentially $\nu$-integrable, it is necessary and sufficient that $gf$ be essentially $\mu$-integrable.*

Taking into account Prop. 10, this follows immediately from Th. 1 of §5, No. 3 and Th. 1 of No. 2.

#### Example {#int-v-s6-n6-exa-1 .statement}

— Let $X$ and $T$ be two locally compact spaces, and let $\pi$ be a *local homeomorphism of $X$ into $T$*. In other words (GT, I, §11, Exer. 25), we assume that every point $x \in X$ admits a neighborhood $V$ such that $\pi|V$ is a homeomorphism of $V$ onto a neighborhood of $\pi(x)$; if necessary replacing $V$ by a relatively compact open neighborhood $W$ of $x$ such that $\overline{W} \subset V$, one deduces that the set $\mathcal{U}$ of relatively compact open subsets $U$ of $X$, such that $\pi|\overline{U}$ is a homeomorphism of $\overline{U}$ onto its image, is an *open covering* of $X$. Now let $\mu$ be a positive measure on $T$; if $U$ is an element of $\mathcal{U}$, then $\pi(U)$ is an open set in the compact space $\pi(\overline{U})$, therefore is a locally compact subspace of $T$, and one knows how to define the measure $\mu|\pi(U)$ induced by $\mu$ on $\pi(U)$ (Ch. IV, §5, No. 7). Let $\nu_U$ be the image of $\mu|\pi(U)$ under the homeomorphism inverse to $\pi|U$; we are going to show that there exists one and only one measure $\nu$ on $X$ that induces the measure $\nu_U$ on every open set $U \in \mathcal{U}$. This measure is called the *inverse image of $\mu$ under the local homeomorphism $\pi$*, and is denoted $\pi^{-1}(\mu)$.

The uniqueness of $\nu$ follows at once from the principle of localization (Ch. III, §2, No. 1, Cor. of Prop. 1). To establish existence, we note that if $t \in T$, then every point $x \in \pi^{-1}(t)$ admits a neighborhood that intersects $\pi^{-1}(t)$ only at the point $x$, so that $\pi^{-1}(t)$ is a *discrete* subspace of $X$, and that the family $(\varepsilon_x)_{x \in \pi^{-1}(t)}$ is summable; we denote its sum by $\lambda_t$. We next show that the mapping $t \mapsto \lambda_t$ is scalarly essentially $\mu$-integrable, and that its integral $\nu = \int \lambda_t d\mu(t)$ is the sought-for inverse image. This will result at once from the following lemma:

#### Lemma {#int-v-s6-n6-lem-1 .statement}

— a) *Let $f$ be an element of $\mathscr{K}_+(X)$; the function $t \mapsto \lambda_t(f)$ is positive, upper semi-continuous, with compact support, and its restriction to $\pi(X)$ is continuous.*

b) *Let $U$ be an element of $\mathcal{U}$, $\nu$ the integral of the scalarly essentially $\mu$-integrable function $t \mapsto \lambda_t$; the image of the measure $\nu|U$ under $\pi|U$ is equal to $\mu|\pi(U)$.*

To establish a), one may reduce by means of a partition of unity (Ch. III, §1, No. 2, Lemma 1) to the case that the support $S$ of $f$ is contained in an open set $U \in \mathcal{U}$. Let $g$ be the mapping $t \mapsto \lambda_t(f)$; $\pi|U$ being a homeomorphism, $g|\pi(U)$ belongs to $\mathcal{K}_+(\pi(U))$, consequently ($\pi(U)$ being an open set in $\pi(X)$) the restriction of $g$ to $\pi(X)$ is continuous. Since $g$ is positive and the restriction of $g$ to the compact set $\pi(S)$ is continuous, one sees that $g$ is upper semi-continuous on $T$. It follows that $g$ is $\mu$-integrable.

To establish b), denote by $g$ an element of $\mathcal{K}(\pi(U))$, by $g^\circ$ its extension by 0 to $T$, by $f$ the function $g \circ (\pi|U)$, and by $f^\circ$ the extension by 0 of $f$ to $X$. The assertion b) is equivalent to the equality $\int g^\circ d\mu = \int f^\circ d\nu$. But $f \in \mathcal{K}(U)$, therefore $f^\circ \in \mathcal{K}(X)$, and the second integral is therefore equal to $\int \lambda_t(f^\circ) d\mu(t)$. Finally $\lambda_t(f^\circ) = g^\circ(t)$, which completes the proof.

We now observe that $\pi(X)$ is *open* in $T$, hence is $\mu$-measurable; the mapping $\Lambda : t \mapsto \lambda_t$ is vaguely $\mu$-measurable, because its restriction to each of the sets $\pi(X)$ and $\mathbf{C}\pi(X)$ is vaguely continuous. Under these conditions, the formula $\overline{\pi}^{-1}(\mu) = \int \lambda_t d\mu(t)$ defines a decomposition into slices of $\overline{\pi}^{-1}(\mu)$ relative to $\pi$, and Prop. 10 yields the following result:

#### Proposition 11 {#int-v-s6-prop-11 .statement}

*Let $\pi$ be a local homeomorphism of a locally compact space $X$ into a locally compact space $T$, and let $\mu$ be a positive measure on $T$. Let $n$ be the numerical function that associates to every $t \in T$ the number of elements of $\overline{\pi}^{-1}(t)$ if this number is finite, and $+\infty$ in the contrary case. For $\pi$ to be $\overline{\pi}^{-1}(\mu)$-proper, it is necessary and sufficient that $n$ be locally $\mu$-integrable, in which case*

$$
\pi\left( \overline{\pi}^{-1}(\mu) \right) = n \cdot \mu .
$$

### Exercises {#int-v-s6-exercises}

See the [exercises for § 6](exercises/s6/).
