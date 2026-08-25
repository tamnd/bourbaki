---
book: int
book_title: Integration
chapter: V
chapter_title: INTEGRATION OF MEASURES
section: 4
section_title: Integration of positive point measures
lang: en
source: int-i-vi
book_pages: INT V.31-INT V.38, INT V.99
pdf_pages: 0286-0293, 0354-0354
extraction: ocr
subsections:
    - "no": 1
      title: Families of point measures
      page: 31
      pdf_page: 286
    - "no": 2
      title: Upper integrals of positive functions with respect to an integral of point measures
      page: 33
      pdf_page: 288
    - "no": 3
      title: Measurability with respect to an integral of point measures
      page: 35
      pdf_page: 290
    - "no": 4
      title: Integration of functions with values in a Banach space, with respect to an integral of point measures
      page: 37
      pdf_page: 292
statements: 10
exercises: 2
content_sha256: 430049d52ece7ec09ca13d7fcfbee0ced4d0c7ea802338d6a358ebe95493a050
---

## § 4. INTEGRATION OF POSITIVE POINT MEASURES

### 1. Families of point measures

Let X and T be two locally compact spaces, $\pi$ a mapping of T into X, and $g$ a finite numerical function $\geqslant 0$ defined on T; these two functions define a mapping $t \mapsto \lambda_t = g(t)\varepsilon_{\pi(t)}$ of T into the space $\mathcal{M}(X)$ of measures on X, such that for every $t \in T$, $\lambda_t$ is either a point measure (Ch. III, §2, No. 4) or is equal to 0. If $f$ is a numerical function $\geqslant 0$ defined on X, then $\int^* f(x) d\lambda_t(x) = \int^\bullet f(x) d\lambda_t(x) = f(\pi(t))g(t)$ (recall our convention of taking this product to be 0 when $g(t) = 0$ and $f(\pi(t)) = +\infty$). Every function (with values in a topological space) defined on X is $\lambda_t$-measurable for every $t \in T$. Every mapping $f$ of X into a Banach space F is $\lambda_t$-integrable for all $t \in T$, and $\int f(x) d\lambda_t(x) = f(\pi(t))g(t)$. Finally, if $f$ is an arbitrary numerical function defined on X, for $f$ to be $\lambda_t$-integrable it is necessary and sufficient that $f(\pi(t))g(t)$ be finite, in which case $\int f(x) d\lambda_t(x) = f(\pi(t))g(t)$.

#### Definition 1 {#int-v-s4-def-1 .statement}

Let $\mu$ be a positive measure on T. The pair $(\pi, g)$ is said to be $\mu$-adapted if the following conditions are satisfied:
1° The functions $\pi$ and $g$ are $\mu$-measurable.
2° For every function $f \in \mathcal{K}(X)$, the mapping $t \mapsto f(\pi(t))g(t)$ is essentially $\mu$-integrable.

#### Proposition 1 {#int-v-s4-prop-1 .statement}

If the pair $(\pi, g)$ is $\mu$-adapted, then the mapping $\Lambda : t \mapsto \lambda_t = g(t)\varepsilon_{\pi(t)}$ of T into $\mathcal{M}_+(X)$ is scalarly essentially $\mu$-integrable, vaguely $\mu$-measurable and $\mu$-adequate. Conversely, if $\Lambda$ is scalarly essentially $\mu$-integrable and vaguely $\mu$-measurable, then the function $g$ is $\mu$-measurable and the restriction of $\pi$ to the set $S$ of $t \in T$ such that $g(t) \neq 0$ is $\mu$-measurable.

Suppose that the pair $(\pi, g)$ is $\mu$-adapted; for every function $f \in \mathcal{K}(X)$, the function $t \mapsto \langle f, \lambda_t \rangle = f(\pi(t))g(t)$ is then essentially $\mu$-integrable. Let us show that $t \mapsto \lambda_t$ is vaguely $\mu$-measurable. For, we first note that if $\pi$ and $g$ are continuous, then the mapping $t \mapsto \lambda_t$ is vaguely continuous. In the general case, the set of compact subsets $K$ of $T$ such that the restrictions of $\pi$ and $g$ to $K$ are continuous is $\mu$-dense (Ch. IV, §5, No. 10, Prop. 15); if $K$ is such a set, then the restriction of $t \mapsto \lambda_t$ to $K$ is vaguely continuous, whence the first assertion of the statement. Prop. 2 of §3, No. 1 shows that $\Lambda$ is $\mu$-adequate.

Conversely, suppose that $\Lambda$ is scalarly essentially $\mu$-integrable and vaguely $\mu$-measurable; it is then $\mu$-adequate (§3, No. 1, Prop. 2). Since the function 1 is lower semi-continuous on $X$, the function $t \mapsto \lambda_t(1) = g(t)$ is $\mu$-measurable (§3, Def. 1). The set $S$ is therefore measurable (Ch. IV, §5, No. 5, Prop. 7). The set $\mathfrak{K}$ of compact sets $K \subset S$ such that $g|K$ is continuous and $\Lambda|K$ is vaguely continuous is $\mu$-dense in $S$ (Ch. IV, §5, No. 10, Prop. 15); if $K \in \mathfrak{K}$, then the restriction to $K$ of the mapping $t \mapsto \varepsilon_{\pi(t)} = \frac{1}{g(t)} \lambda_t$ is therefore vaguely continuous, and this implies the continuity of $\pi|K$ (Ch. III, §1, No. 9, Prop. 13). Since $\mathfrak{K}$ is $\mu$-dense in $S$, the restriction of $\pi$ to $S$ is $\mu$-measurable.

We shall make use of the following lemma:

#### Lemma {#int-v-s4-n1-lem-1 .statement}

*Let $T$ and $X$ be two topological spaces, $\pi$ a proper continuous mapping (GT, I, §10, No. 1, Def. 1) of $T$ into $X$. Let $g$ be a lower semi-continuous numerical function defined on $T$. For every $x \in X$, let $f(x)$ be the infimum of the function $g(t)$ in the set $\overline{\pi}^{-1}(x)$ (infimum equal to $+\infty$ if $\overline{\pi}^{-1}(x) = \varnothing$; cf. S, III, §1, No. 9). Then $f$ is lower semi-continuous on $X$.*

For every (finite) real number $a$, denote by $B_a$ the set of $x \in X$ such that $f(x) \leq a$, and by $A_a$ the set of $t \in T$ such that $g(t) \leq a$; it all comes down to showing that $B_a$ is closed (GT, IV, §6, No. 2, Prop. 1). Now, $A_a$ is closed (same ref.) and the proper mapping $\pi$ is closed (GT, I, §10, No. 1, Prop. 1); we are thus reduced to proving that $\pi(A_a) = B_a$. The obvious relation $f(\pi(t)) \leq g(t)$ for all $t \in T$ implies that $\pi(A_a) \subset B_a$. On the other hand, let $x \in B_a$; the set $\overline{\pi}^{-1}(x)$ is quasi-compact (GT, I, §10, No. 2, Th. 1) and nonempty, therefore there exists a $t \in \overline{\pi}^{-1}(x)$ such that

$$
g(t) = \inf_{u \in \pi^{-1}(x)} g(u) = f(x) \quad (\text{GT, IV, } \S 6, \text{ No. 2, Th. 3}); \text{ thus } t \in A_a \text{ and } \pi(t) = x.
$$

### 2. Upper integrals of positive functions with respect to an integral of point measures

We are going to see that, when $(\pi, g)$ is a $\mu$-adapted pair, one can sharpen the results obtained by applying the propositions of $\S 3$ to the family $t \mapsto \lambda_t = g(t)\varepsilon_{\pi(t)},$ which is $\mu$-adequate by Prop. 1.

#### Theorem 1 {#int-v-s4-thm-1 .statement}

*Let* $(\pi, g)$ *be a $\mu$-adapted pair, and let*
$$
\nu = \int g(t)\varepsilon_{\pi(t)}\, d\mu(t).
$$
*For every numerical function* $f \geq 0$ *defined on X,* (1)
$$
\int^\bullet f(x)\, d\nu(x) = \int^\bullet f(\pi(t))g(t)\, d\mu(t).
$$

A) Suppose first that the measure $\mu$ has compact support K and that the restrictions to K of the functions $g$ and $\pi$ are continuous. By formula (4) of $\S 3$, No. 1, $\nu^\bullet(1) = \int_K g(t)\, d\mu(t) < +\infty,$ so that all of the measures that figure in formula (1) are bounded. We may therefore replace $\int^\bullet$ by $\int^*$ in the first member. In view of formula (6) of $\S 3$, No. 2, it all comes down to proving that (2)
$$
\int^* f(x)\, d\nu(x) \leq \int^\bullet f(\pi(t))g(t)\, d\mu(t),
$$
where the symbol $\int^\bullet$ in the second member can in turn be replaced by $\int^*$. By the definition of upper integral, it suffices to verify the inequality (3)
$$
\int^* f(x)\, d\nu(x) \leq \int^* h(t)\, d\mu(t)
$$
for every lower semi-continuous function $h$ on T that is $\geq$ the function $t \mapsto f(\pi(t))g(t)$. Now, let $\varepsilon$ be a number $> 0$ and let $u$ be the function $(h + \varepsilon)/g,$ which is lower semi-continuous in K. If $t \in \pi^{-1}(\{x\}) \cap K,$ then $u(t) \geq f(x):$ this is obvious if $g(t) = 0,$ because then $u(t) = +\infty;$ if $g(t) > 0,$ then
$$
u(t)g(t) = h(t) + \varepsilon \geq f(\pi(t))g(t) = f(x)g(t),
$$

whence the asserted inequality. Under these conditions, for every $x \in X$ let $v(x)$ be the infimum of $u(t)$ for $t \in \pi^{-1}(\{x\}) \cap K$. The function $v$ is $\geq f$ by the foregoing, it is lower semi-continuous on $X$ by the Lemma (applied to the restriction of $\pi$ to $K$), and $v(\pi(t))g(t) \leq h(t) + \varepsilon$ for all $t \in K$ (recall that the first member is zero by convention if $g(t) = 0$). Let us then apply to $v$ the formula (4) of §3, No. 1. We obtain:

$$
\int^* f(x)\, d\nu(x) \leq \int^* v(x)\, d\nu(x)
$$
$$
= \int^* v(\pi(t))g(t)\, d\mu(t) \leq \int_K^* (h(t) + \varepsilon)\, d\mu(t)
$$
$$
= \int_K^* h(t)\, d\mu(t) + \varepsilon \mu(1).
$$

Since the measure $\mu$ is bounded and $\varepsilon$ is arbitrary, the inequality (3) follows.

B) Let us now pass to the general case. Since the mapping $t \mapsto (\pi(t), g(t))$ of $T$ into $X \times \mathbf{R}_+$ is $\mu$-measurable (Ch. IV, §5, No. 3, Th. 1), the set $\mathcal{K}$ of compact subsets $K$ of $T$ such that the restrictions of $\pi$ and $g$ to $K$ are continuous is $\mu$-dense (Ch. IV, §5, No. 10, Prop. 15). By Prop. 4 of §2, No. 3, $\mu$ is the sum of a summable family $(\mu_\alpha)_{\alpha \in A}$ of measures whose supports are elements of $\mathcal{K}$; the pair $(\pi, g)$ being $\mu_\alpha$-adapted for every $\alpha \in A$, let $\nu_\alpha$ be the measure $\int g(t) \varepsilon_{\pi(t)}\, d\mu_\alpha(t)$. Then by A),

$$
\int^* f(x)\, d\nu_\alpha(x) = \int^* f(\pi(t))g(t)\, d\mu_\alpha(t).
$$

But the $\nu_\alpha$ form a summable family whose sum is equal to $\nu$ (§3, No. 1, Cor. of Prop. 1). Therefore, by Prop. 1 of §2, No. 2,

$$
\int^* f(x)\, d\nu(x) = \sum_{\alpha \in A} \int^* f(x)\, d\nu_\alpha(x).
$$

One has an analogous relation for the second member of (5), and (1) therefore follows from (5) by summing over $\alpha$.

#### Corollary {#int-v-s4-n2-cor-1 .statement}

— *In order that a subset N of X be locally negligible for $\nu$, it is necessary and sufficient that the intersection of $\pi^{-1}(N)$ with the set of points $t \in T$ where $g(t) > 0$ be locally negligible for $\mu$.*

#### Proposition 2 {#int-v-s4-prop-2 .statement}

— *Let $\pi$ be a proper continuous mapping (GT, I, §10, No. 1) of T into X, and let g be a continuous, finite numerical function on T such that $g(t) > 0$ for all $t \in T$. The pair $(\pi, g)$ is then $\mu$-adapted, and if one sets*
$$
\nu = \int g(t) \varepsilon_{\pi(t)}\, d\mu(t),
$$

then, for every numerical function $f \geq 0$ defined on $X$,

$$
\int^* f(x)\, d\nu(x) = \int^* f(\pi(t))g(t)\, d\mu(t).
$$

It is clear that $\pi$ and $g$ are $\mu$-measurable; moreover, for every function $\psi \in \mathcal{K}(X)$, $\psi \circ \pi$ is continuous with compact support, since $\pi$ is proper; the pair $(\pi, g)$ is therefore $\mu$-adapted and, moreover, the mapping $t \mapsto g(t)\varepsilon_{\pi(t)}$ is vaguely continuous.

Let $h$ be a lower semi-continuous function on $T$ such that

$$
f(\pi(t))g(t) \leq h(t) \quad \text{for all } t \in T.
$$

We are going to show that

$$
\int^* f(x)\, d\nu(x) \leq \int^* h(t)\, d\mu(t).
$$

By the definition of upper integral, this will imply the inequality

$$
\int^* f(x)\, d\nu(x) \leq \int^* f(\pi(t))g(t)\, d\mu(t),
$$

which, combined with the inequality (7) of §3, No. 2, will prove (7).

To prove (8), let us define a function $\overline{f}$ on $X$ in the following manner: $\overline{f}(x)$ is the infimum of $h(t)/g(t)$ in the set $\overline{\pi}^{-1}(x)$ (infimum equal to $+\infty$ if $\overline{\pi}^{-1}(x) = \varnothing$). The function $\overline{f}$ has the following properties:

$1^\circ$ $\overline{f}(x) \geq f(x)$ for all $x \in X$ (since $g(t) > 0$ for all $t \in T$).

$2^\circ$ $\overline{f}(\pi(t))g(t) \leq h(t)$ for all $t \in T$.

$3^\circ$ The function $\overline{f}$ is lower semi-continuous by virtue of the Lemma, the function $h/g$ being lower semi-continuous on $T$.

Consequently, in view of Prop. 2a) of §3, No. 1:

$$
\int^* f(x)\, d\nu(x) \leq \int^* \overline{f}(x)\, d\nu(x) = \int^* \overline{f}(\pi(t))g(t)\, d\mu(t) \leq \int^* h(t)\, d\mu(t),
$$

which establishes (8), and completes the proof.

### 3. Measurability with respect to an integral of point measures

#### Proposition 3 {#int-v-s4-prop-3 .statement}

— Let $(\pi, g)$ be a $\mu$-adapted pair, and let

$$
\nu = \int g(t)\varepsilon_{\pi(t)}\, d\mu(t).
$$

Let $f$ be a mapping of $X$ into a topological space $G$, and let $S$ be the ($\mu$-measurable) set of points $t \in T$ such that $g(t) > 0$. In order that $f$ be $\nu$-measurable, it is necessary and sufficient that the restriction of $f \circ \pi$ to $S$ be $\mu$-measurable.

Suppose first that $f$ is $\nu$-measurable. By hypothesis, the set $\mathcal{K}$ of compact subsets $K$ of $S$, such that the restriction of $\pi$ to $K$ is continuous, is $\mu$-dense in $S$ (Ch. IV, §5, No. 10, Prop. 15). To show that the restriction of $f \circ \pi$ to $S$ is $\mu$-measurable, it therefore suffices to prove that for every $K \in \mathcal{K}$, the set of compact subsets $H$ of $K$, such that the restriction of $f \circ \pi$ to $H$ is continuous, is $\mu$-dense in $K$ (Ch. IV, §5, No. 8, Prop. 13). But by hypothesis, there exists a partition of the compact set $\pi(K)$ formed by a $\nu$-negligible set $N$ and a sequence of compact sets $(C_n)$ such that the restriction of $f$ to each $C_n$ is continuous. Under these conditions, $K \cap \overline{\pi}(N)$ and the sets $K \cap \overline{\pi}(C_n)$ form a partition of $K$; but $K \cap \overline{\pi}(N)$ is $\mu$-negligible by virtue of the Cor. of Th. 1 of No. 2, the sets $K \cap \overline{\pi}(C_n)$ are compact, and the restriction of $f \circ \pi$ to each of the latter sets is continuous, which proves that the restriction of $f \circ \pi$ to $S$ is $\mu$-measurable.

Conversely, suppose this to be the case; to show that $f$ is $\nu$-measurable, it suffices to prove that the set $\mathcal{L}$ of compact subsets $L$ of $X$, such that the restriction of $f$ to $L$ is continuous, is $\nu$-dense (Ch. IV, §5, No. 10, Prop. 15). Let $N$ be a subset of $X$ such that $N \cap L$ is $\nu$-negligible for every $L \in \mathcal{L}$, and let us show that $N$ is locally $\nu$-negligible. For this, we must show that $\overline{\pi}(N) \cap S$ is locally $\mu$-negligible (Cor. of Th. 1 of No. 2). Now, the set $\mathcal{H}$ of compact subsets $H$ of $S$, such that the restrictions to $H$ of $\pi$ and $f \circ \pi$ are continuous, is by hypothesis $\mu$-dense in $S$ (Ch. IV, §5, No. 10, Prop. 15). It therefore suffices to prove that $\overline{\pi}(N) \cap H$ is $\mu$-negligible for every $H \in \mathcal{H}$. Now, $\pi(H)$ is compact and may be identified with the quotient space of $H$ by the equivalence relation $\pi(t) = \pi(t')$, $\pi$ being identified with the canonical mapping of $H$ onto this quotient space (GT, I, §5, No. 2, Prop. 3). Since the restriction of $f \circ \pi$ to $H$ is continuous, the restriction of $f$ to $\pi(H)$ is therefore continuous, in other words $\pi(H) \in \mathcal{L}$, consequently $N \cap \pi(H)$ is $\nu$-negligible. By the Cor. of Th. 1 of No. 2, $\overline{\pi}(N \cap \pi(H)) \cap S$ is locally $\mu$-negligible; the same is therefore true of the set

$$
H \cap \overline{\pi}(N) \subset \overline{\pi}(N \cap \pi(H)) \cap S;
$$

but since $H$ is compact, $H \cap \overline{\pi}(N)$ is $\mu$-negligible, which completes the proof.

#### Remark {#int-v-s4-n3-rem-1 .statement}

If $f$ is a mapping of $X$ into a Banach space $F$, it comes to the same to say that the restriction of $f \circ \pi$ to $S$ is $\mu$-measurable or to say that the function $(f \circ \pi)g$ (defined on $T$) is $\mu$-measurable, since $g$ is $\mu$-measurable, is not zero in $S$, and is zero on $T - S$ (Ch. IV, §5, No. 10, Prop. 15).

### 4. Integration of functions with values in a Banach space, with respect to an integral of point measures

#### Theorem 2 {#int-v-s4-thm-2 .statement}

*Let* $(\pi, g)$ *be a $\mu$-adapted pair, and let*
$$
\nu = \int g(t) \varepsilon_{\pi(t)} \, d\mu(t).
$$
*Let* $f$ *be a function defined on* $X$, *with values in a Banach space* $F$ *or in* $\overline{\mathbf{R}}$. *For* $f$ *to be essentially $\nu$-integrable, it is necessary and sufficient that* $t \mapsto f(\pi(t))g(t)$ *be essentially $\mu$-integrable, in which case*
$$
\int f(x) \, d\nu(x) = \int f(\pi(t))g(t) \, d\mu(t).
$$
*Suppose, moreover, that* $\pi$ *is continuous and proper, and that* $g$ *is continuous and such that* $g(t) > 0$ *for all* $t \in T$. *Then, for* $f$ *to be $\nu$-integrable, it is necessary and sufficient that* $t \mapsto f(\pi(t))g(t)$ *be $\mu$-integrable.*

A) We begin by treating the case that the measure $\mu$ has compact support $K$, on which $g$ is bounded. The measures $\mu$ and $\nu$ are then bounded, and one can replace 'essentially integrable' in the statement by 'integrable'. Suppose that $f$ is $\nu$-integrable: the function $f(\pi(t))g(t)$ is then $\mu$-integrable, and the relation (9) is verified, by Th. 1 of §3, No. 3. Conversely, suppose that $f(\pi(t))g(t)$ is $\mu$-integrable: $f$ is then $\nu$-measurable (No. 3, Prop. 3 and *Remark*), and
$$
\int^\bullet |f(x)| \, d\nu(x) = \int^\bullet |f(\pi(t))|g(t) \, d\mu(t) < +\infty
$$
(No. 2, Th. 1); $f$ is therefore essentially $\nu$-integrable (§1, No. 3, Prop. 9), hence $\nu$-integrable. Th. 1 of §3, No. 3 then implies (9).

B) Let us pass to the general case. Let $\mathcal{K}$ be the set of compact subsets $K$ of $T$ such that $g|K$ is continuous: $\mathcal{K}$ is $\mu$-dense (Ch. IV, §5, No. 10, Prop. 15), therefore the measure $\mu$ is the sum of a family $(\mu_\alpha)_{\alpha \in A}$ of measures whose supports are elements of $\mathcal{K}$ (§2, No. 3, Prop. 4). The pair $(g, \pi)$ is obviously $\mu_\alpha$-adapted for every $\alpha \in A$, and the measure $\nu$ is the sum of the family of measures $\nu_\alpha = \int \varepsilon_{\pi(t)}g(t) \, d\mu_\alpha(t)$ (§3, No. 1, Cor. of Prop. 1). Since the argument of A) may be applied to the measures $\mu_\alpha, \nu_\alpha$, the first part of the statement then follows from Prop. 3 of §2, No. 2.

For the function $f$ (resp. $t \mapsto f(\pi(t))g(t)$) to be integrable for $\nu$ (resp. for $\mu$), it is necessary and sufficient that it be essentially integrable and that

$$
\int^* |f(x)| d\nu(x) < +\infty \quad (\text{resp. } \int^* |f(\pi(t))|g(t)\,d\mu(t) < +\infty ).
$$

The second part of the statement therefore follows from the first part and Proposition 2.

#### Remark {#int-v-s4-n4-rem-1 .statement}

— Let $(\pi, g)$ be a $\mu$-adapted pair, $\pi'$ a mapping of T into X, and $g'$ a finite numerical function $\geq 0$ defined on T, such that $\pi'$ (resp. $g'$) is equal to $\pi$ (resp. $g$) locally almost everywhere for $\mu$. Then the pair $(\pi', g')$ is $\mu$-adapted, the measures $\lambda_t = g(t)\varepsilon_{\pi(t)}$ and $\lambda'_t = g'(t)\varepsilon_{\pi'(t)}$ are equal locally almost everywhere, and $\int g(t)\varepsilon_{\pi(t)}\,d\mu(t) = \int g'(t)\varepsilon_{\pi'(t)}\,d\mu(t)$. If now $\pi'$ and $g'$ are only defined locally almost everywhere (for $\mu$) and if there exists a $\mu$-adapted pair $(\pi, g)$ such that $\pi'$ (resp. $g'$) is equal to $\pi$ (resp. $g$) locally almost everywhere, one again says that the pair $(\pi', g')$ is $\mu$-adapted and one sets

$$
\int g'(t)\varepsilon_{\pi'(t)}\,d\mu(t) = \int g(t)\varepsilon_{\pi(t)}\,d\mu(t)
$$

(cf. §3, No. 3, *Remark*). The statements of Ths. 1 and 2 and of Prop. 3 remain valid when $\pi$ and $g$ are only assumed to be defined locally almost everywhere.

### Exercises {#int-v-s4-exercises}

See the [exercises for § 4](exercises/s4/).
