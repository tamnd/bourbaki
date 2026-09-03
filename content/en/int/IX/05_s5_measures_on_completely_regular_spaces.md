---
book: int
book_title: Integration
chapter: IX
chapter_title: MEASURES ON HAUSDORFF TOPOLOGICAL SPACES
section: 5
section_title: Measures on completely regular spaces
lang: en
source: int-vii-ix
book_pages: INT IX.56-INT IX.72, INT IX.113-INT IX.117
pdf_pages: 0238-0254, 0295-0299
extraction: ocr
subsections:
    - "no": 1
      title: Measures and bounded continuous functions
      page: 56
      pdf_page: 238
    - "no": 2
      title: Bounded measures and linear forms on $\mathcal{C}^b(T)$
      page: 59
      pdf_page: 241
    - "no": 3
      title: Tight convergence of bounded measures
      page: 60
      pdf_page: 242
    - "no": 4
      title: 'Application: topological properties of the space $\mathcal{M}_+^b(T)$'
      page: 63
      pdf_page: 245
    - "no": 5
      title: Compactness criterion for tight convergence
      page: 64
      pdf_page: 246
    - "no": 6
      title: Tight convergence of measures and compact convergence of functions
      page: 67
      pdf_page: 249
    - "no": 7
      title: 'Application: the Laplace transformation'
      page: 68
      pdf_page: 250
statements: 33
exercises: 13
content_sha256: 58103c2c457c58b000a2920115ae10c4f462f32dd4b4a8e8eb6d2753005ef40f
---

## § 5. MEASURES ON COMPLETELY REGULAR SPACES

If T is a topological space, and F is a Banach space, the notation $C^b(T; F)$ indicates the space of bounded continuous functions on T with values in F, equipped with the norm of uniform convergence. If $F = \mathbf{R}$, this notation is abbreviated to $C^b(T)$, or to $C^b$ if there is no ambiguity, and one denotes by $C^b_+(T)$ or $C^b_+$ the cone of positive functions in $C^b(T)$. The space of bounded complex measures on T will be denoted $M^b(T; \mathbf{C})$, the space of bounded real measures by $M^b(T)$ or $M^b$, and the cone of bounded positive measures by $M^b_+(T)$ or $M^b_+$.

### 1. Measures and bounded continuous functions

Recall (GT, IX, §1, No. 5, Def. 4) that a topological space T is said to be completely regular if it is uniformizable and Hausdorff. This is equivalent to saying (loc. cit., Prop. 3) that T is homeomorphic to a subspace of a compact space. If T is completely regular, then every positive lower semi-continuous function $f$ on T is the upper envelope of the increasing directed set of elements of $C^b_+(T)$ that are $\leq f$, and every positive and bounded upper semi-continuous function $g$ is the lower envelope of the decreasing directed set of elements of $C^b_+(T)$ that are $\geq g$ (loc. cit., §1, No. 6, Prop. 5). We shall need the following lemma:

#### Lemma {#int-ix-s5-n1-lem-1 .statement}

Let T be a completely regular space, K a compact subset of T, and U an open subset of T containing K.
a) There exists an open subset U' of T such that $K \subset U' \subset \overline{U'} \subset U$.
b) Let f be a continuous function defined on K with values in an interval I of $\mathbf{R}$ (resp. in $\mathbf{C}$). There exists a bounded continuous function $f'$ on T, with values in I (resp. in $\mathbf{C}$), that extends f and is zero on $T - U$.

It suffices to treat the case that T is a subspace of a compact space X. Let V be an open subset of X such that $V \cap T = U$; denote by $V'$ an open set in X containing K such that $\overline{V'} \subset V$, by g a continuous function on X with values in I (resp. in $\mathbf{C}$) extending f and zero on $X - V$ (GT, IX, §4, No. 1, Prop. 1). The condition a) is satisfied by taking $U' = V' \cap T$, and b) by taking $f'$ to be the restriction of g to T.

#### Proposition 1 {#int-ix-s5-prop-1 .statement}

— Let T be a completely regular space.
a) Let $\mu$ be a positive measure on T, and f a numerical function $\geq 0$ defined on T and lower semi-continuous (resp. upper semi-continuous ous, finite, with compact support). Then

(1) $\mu^\bullet(f) = \sup_{g \in I_f} \mu^\bullet(g)$ (resp. $\mu^\bullet(f) = \inf_{g \in S_f} \mu(g)$),

where $I_f$ (resp. $S_f$) denotes the set of bounded continuous functions $g$ such that $0 \leq g \leq f$ (resp. $g \geq f$).

b) Let $\theta$ be a complex measure on $T$, and $f$ a numerical function $\geq 0$ defined on $T$ and lower semi-continuous. Then

(2) $|\theta|^\bullet(f) = \sup_g |\theta(g)|$,

where $g$ runs over the set of bounded and $|\theta|$-integrable continuous complex functions such that $|g| \leq f$.

The first of the formulas (1) is obvious, because $I_f$ is an increasing directed set of continuous functions whose upper envelope is $f$, and one can apply Prop. 5 of §1, No. 6. The same proposition will imply the second formula, if we show that $S_f$ contains a $\mu$-integrable bounded continuous function. Thus, let $K$ be the support of $f$, and $M$ the supremum of $f$; since $K$ is compact, $M$ is finite (GT, IV, §6, No. 2, Th. 3). Let $U$ be an open set containing $K$ and such that $\mu^\bullet(U) < +\infty$; there exists (Lemma) a continuous function $g$ with values in $[0, M]$, equal to $M$ on $K$ and zero outside $U$; then $g \in S_f$ and $\mu^\bullet(g) \leq M \mu^\bullet(U) < +\infty$.

Let us pass to b). It clearly suffices to show that $|\theta|^\bullet(f) \leq \sup_g |\theta(g)|$.

Let $a$ and $b$ be two real numbers such that $a < b < |\theta|^\bullet(f)$. By (1), there exists a function $h \in \mathcal{C}_+^b(T)$ such that $h \leq f$ and $|\theta|^\bullet(h) > b$; denote by $M$ the supremum of $h$. By the definition of $|\theta|^\bullet$ (§1, No. 2, Def. 4), there exists a compact subset $K$ of $T$ such that $|\theta|_K^\bullet(h_K) > b$. There then exists a continuous complex function $j$ on $K$ such that $|j| \leq h_K$ and $|\theta_K(j)| > b$ (Ch. III, §1, No. 6). Let us choose an open set $U$ containing $K$ and such that $|\theta|^\bullet(U - K) \leq \frac{b - a}{M}$ (§1, No. 9, Props. 13 and 14); extend $j$ to a continuous complex function $k$ on $T$, zero outside $U$ (Lemma); for every $t \in T$, set

(3)
$$
g(t) = \begin{cases}
k(t) & \text{if } |k(t)| \leq h(t) \\
\frac{k(t)}{|k(t)|} h(t) & \text{if } |k(t)| > h(t)
\end{cases}
$$

Clearly $|g| \leq h \leq f$, and $g = j$ on $K$, therefore $||\theta_K(j)| - |\theta(g)|| = ||\theta(j^0)| - |\theta(g)|| \leq |\theta|^\bullet(|j^0 - g|) \leq M \cdot |\theta|^\bullet(U - K) \leq b - a$, consequently $|\theta(g)| > a$. Let us show on the other hand that $g$ is a continuous function:

since $a$ is subject to the sole condition $a < |\theta|^*(f)$, this will imply that the second member of (2) is $\geqslant$ the first, whence the proposition. Now, let F (resp. $F'$) be the set of $t \in T$ such that $|k(t)| \leq h(t)$ (resp. $|k(t)| \geq h(t)$). These sets being closed, and their union being T, it will suffice to show that $g_F$ and $g_{F'}$ are continuous: now, this property is obvious for $g_F = k_F$, and it is so for $g_{F'}$ at the points where $k(t) \neq 0$; on the other hand, if $t \in F'$ is such that $k(t) = 0$, then also $h(t) = 0$, and the inequality $|g| \leq h$ implies that $g$ is continuous at the point $t$.

#### Remark 1 {#int-ix-s5-n1-rem-1 .statement}

Let $f$ be a positive lower semi-continuous function, and let $J_f$ be the set of positive bounded continuous functions zero outside a $\mu$-integrable open set and bounded above by $f$. One can show that $f$ is the upper envelope of $J_f$ and that $\mu^*(f) = \sup_{g \in J_f} \mu(g)$.

#### Remark 2 {#int-ix-s5-n1-rem-2 .statement}

If the measure $\mu$ is bounded, the formula $\mu^*(f) = \inf_{g \in S_f} \mu(g)$ is obviously valid for every function $f$ that is upper semi-continuous, positive and bounded.

#### Proposition 2 {#int-ix-s5-prop-2 .statement}

— *Let $\eta$ and $\eta'$ be two complex measures on a completely regular space $T$, such that $\eta(f) = \eta'(f)$ for every function $f \in \mathcal{C}^b(T)$ that is integrable for $|\eta|$ and $|\eta'|$. Then $\eta = \eta'$.*

Let us take up again the proof of the second part of Proposition 1, on setting $\theta = \eta - \eta'$. We can require the open set U to be integrable for $|\eta|$ and $|\eta'|$. The function $g$ is then integrable for these two measures, and the relation $\theta(g) = 0$ implies $a < 0$; therefore $|\theta|^*(f) = 0$ for every positive lower semi-continuous function $f$, whence finally $|\theta| = 0$, on taking $f = +\infty$.

#### Proposition 3 {#int-ix-s5-prop-3 .statement}

— *Let $\mu$ be a positive measure on a completely regular space $T$, and let $p \in [1, +\infty[$. The space $\mathcal{H}$ of functions $f \in \mathcal{C}^b(T)$, whose support is contained in a $\mu$-integrable open set, is dense in $\mathcal{L}^p(\mu)$.*

By Prop. 15 of §1, No. 10, it suffices to show that if K is compact in T, and if $g$ is the extension to T by 0 of a function in $\mathcal{C}_+(K)$ between 0 and 1, then there exists a function $f \in \mathcal{C}_+^b(T)$, with support contained in a $\mu$-integrable open set, such that $\|f - g\|_p$ is arbitrarily small. Now, let $\varepsilon$ be a number $> 0$, U an open neighborhood of K such that $\mu^*(U - K) < \varepsilon$, V an open neighborhood of K such that $\overline{V} \subset U$, and $f$ a function with values in $[0, 1]$, continuous, equal to $g$ on K and to 0 outside V (Lemma). The function $|f - g|^p$ is then bounded above by $\varphi_{U-K}$; therefore $\|f - g\|_p \leq \varepsilon^{1/p}$, which establishes the proposition.

*Remark 3).* — There is an analogous statement for functions with values in a Banach space F: the subspace $\mathcal{H} \otimes F$ of $\mathcal{C}^b(T; F)$ is dense in $\mathcal{L}_F^p(\mu)$.

#### Proposition 4 {#int-ix-s5-prop-4 .statement}

— *In order that a bounded complex measure $\theta$ on a completely regular space $T$ be positive, it is necessary and sufficient that $\theta(f) \geq 0$ for every function $f \in \mathcal{C}_+^b(T)$.*

Necessity is obvious. To establish sufficiency, let us take up again the proof of the preceding proposition, on taking $p = 1$ and $\mu = |\theta|$; the notations being the same, the relation $\mu^*(|f - g|) \leq \varepsilon$ and the inequality $\theta(f) \geq 0$ imply $\theta_K(g_K) = \theta(g) \geq -\varepsilon$; since $g_K$ is an arbitrary element of $\mathcal{C}(K)$ between 0 and 1, the measure $\theta_K$ is positive; the compact set K being arbitrary, this means that $\theta$ is positive.

### 2. Bounded measures and linear forms on $\mathcal{C}^b(T)$

#### Proposition 5 {#int-ix-s5-prop-5 .statement}

— *Let T be a completely regular space, and I a continuous complex linear form on the normed space $\mathcal{C}^b(T; \mathbf{C})$. In order that there exist a bounded complex measure $\theta$ on T such that $\theta(f) = I(f)$ for all $f \in \mathcal{C}^b(T; \mathbf{C})$, it is necessary and sufficient that the following condition be satisfied:

(M) *For every number $\varepsilon > 0$, there exists a compact subset K of T such that the relations $g \in \mathcal{C}^b(T; \mathbf{C}), |g| \leq 1, g_K = 0$ imply $|I(g)| \leq \varepsilon$.

The measure $\theta$ is then unique.*

Uniqueness follows from Prop. 2 of No. 1. Let us show that the condition (M) is necessary. Let $\theta$ be a bounded complex measure; let K be a compact set such that $|\theta|^*(T - K) \leq \varepsilon$ (§ 1, No. 2, *Remark 3*). The hypotheses $|g| \leq 1, g_K = 0$ imply $|g| \leq \varphi_{\mathbf{C}_K}$, therefore $|\theta(g)| \leq |\theta|^*(\varphi_{\mathbf{C}_K}) \leq \varepsilon$.

Let us pass to the proof of sufficiency. Let X be the Stone–Čech compactification of T (GT, IX, § 1, Exer. 7; or TG, IX, § 1, No. 6). For every function $f \in \mathcal{C}(X; \mathbf{C})$, set $\nu(f) = I(f_T)$; we define in this way a continuous linear form on $\mathcal{C}(X; \mathbf{C})$, that is, a complex measure on the compact space X. Let $\varepsilon$ be a number $> 0$, K a compact set satisfying (M); the function $\varphi_{\mathbf{C}_K}$ being lower semi-continuous and positive on X, the formula (2) gives us the following relations, where $\mathcal{G}$ denotes the set of functions $g \in \mathcal{C}(X; \mathbf{C})$ such that $|g| \leq \varphi_{\mathbf{C}_K}$:

$$
|\nu|^*(X - K) = \sup_{g \in \mathcal{G}} |\nu(g)| = \sup_{g \in \mathcal{G}} |I(g_T)| \leq \varepsilon.
$$

Let $(K_n)_{n \geq 1}$ be a sequence of compact subsets of T, such that each $K_n$ satisfies (M) for $\varepsilon = 1/n$, and let $S = \bigcup K_n$; S is a Borel set in X, contained in T, and $|\nu|^*(X - T) \leq |\nu|^*(X - S) \leq |\nu|^*(X - K_n) \leq 1/n$ for all n, so that T is $\nu$-measurable and $\nu$ is concentrated on T. Let $f$ be a bounded continuous function on T; since X is the Stone–Čech compactification of T, $f$ may be extended by continuity to a function $g \in \mathcal{C}(X; \mathbf{C})$. Now let $\mu$ be the measure induced by $\nu$ on $T$; one has $\mu(f) = \nu(f^0)$. (1) Since $\nu$ is concentrated on $T$, the functions $f^0$ and $g$ are equal $\nu$-almost everywhere, therefore $\mu(f) = \nu(g) = I(g_T) = I(f)$, which completes the proof.

#### Corollary {#int-ix-s5-n2-cor-1 .statement}

— *With notations as in Prop. 5, suppose that there exists a bounded positive measure $\mu$ on $T$ such that $|I(f)| \leq \mu(|f|)$ for all $f \in \mathcal{C}^b(T; \mathbf{C})$; then there exists a complex measure $\theta$ on $T$ such that $\theta(f) = I(f)$ for all $f \in \mathcal{C}^b(T; \mathbf{C})$.

### 3. Tight convergence of bounded measures

Let $T$ be a completely regular space; the bilinear form
$$
(f, \mu) \mapsto \int f(t) \, d\mu(t)
$$
on $\mathcal{C}^b(T) \times \mathcal{M}^b(T)$ puts these two spaces in a separating duality. For, it is clear that the duality is separating in $\mathcal{C}^b(T)$ from the fact that the measures $\varepsilon_x \ (x \in T)$ belong to $\mathcal{M}^b(T)$; it is separating in $\mathcal{M}^b(T)$ by Prop. 2 of No. 1.

#### Definition 1 {#int-ix-s5-def-1 .statement}

*The weak topology on $\mathcal{M}^b(T)$ associated with the preceding duality between $\mathcal{C}^b(T)$ and $\mathcal{M}^b(T)$ is called the topology of tight convergence (or the tight topology) on $\mathcal{M}^b(T)$.*

The tight topology is Hausdorff, by the remarks preceding the definition. We shall often employ the adverb 'tightly' to mean 'in the sense of the tight topology'. Absent mention to the contrary, $\mathcal{M}^b(T)$ will be equipped with the tight topology throughout the rest of this section.

Every element of $\mathcal{C}^b(T)$ is a linear combination of elements of $\mathcal{C}_+^b(T)$. For a filter $\mathfrak{F}$ on $\mathcal{M}^b(T)$ to converge tightly to a bounded measure $\lambda$, it is necessary and sufficient that
$$
\lim_{\mu} \mu(f) = \lambda(f) \quad \text{with respect to } \mathfrak{F} \text{ for every } f \in \mathcal{C}_+^b(T).
$$

#### Remark 1 {#int-ix-s5-n3-rem-1 .statement}

If $T$ is locally compact, the tight topology is finer than the topology induced on $\mathcal{M}^b(T)$ by the vague topology, and these two topologies coincide only when $T$ is compact. For, if $T$ is not compact, the mapping $t \mapsto \varepsilon_t$ converges vaguely to 0 with respect to the filter of complements of relatively compact subsets of $T$, but does not converge tightly to 0, because the function 1 belongs to $\mathcal{C}^b(T)$ (for the relations between vague convergence and tight convergence, see Prop. 9).

(1) This relation was only established above (§ 2, No. 1, Prop. 1) in the case that $f$ and $\nu$ are positive. The extension to the present situation, where $f$ and $\nu$ are complex and bounded, is immediate by linearity.

#### Remark 2 {#int-ix-s5-n3-rem-2 .statement}

It follows at once from Prop. 4 that $\mathcal{M}_+^b(T)$ is closed in $\mathcal{M}^b(T)$.

#### Remark 3 {#int-ix-s5-n3-rem-3 .statement}

If T is completely regular, the mapping $t \mapsto \varepsilon_t$ of T into $\mathcal{M}^b(T)$ is a homeomorphism (GT, IX, §1, No. 5).

#### Proposition 6 {#int-ix-s5-prop-6 .statement}

— Let T be a completely regular space.

a) Let f be a lower semi-continuous numerical function $\geqslant 0$ defined on T; then the function $\mu \mapsto |\mu|^*(f)$ is lower semi-continuous on $\mathcal{M}^b(T)$.

b) Let f be an upper semi-continuous bounded function defined on T; then the function $\mu \mapsto \mu(f)$ is upper semi-continuous on $\mathcal{M}_+^b(T)$.

For, one sees by Prop. 1 b) of No. 1 that $\mu \mapsto |\mu|^*(f)$ is the upper envelope of a family of functions of the form $\mu \mapsto |\mu(g)|$ with $g \in \mathcal{C}^b(T)$, hence continuous for the tight topology. This establishes a). To prove b), it suffices to choose a constant upper bound C for f, and to write $\mu(f) = \mu(C) - \mu(C - f)$; the function $\mu \mapsto \mu(C)$ is continuous, and the function $\mu \mapsto \mu(C - f)$ is lower semi-continuous on $\mathcal{M}_+^b(T)$ by the foregoing.

#### Proposition 7 {#int-ix-s5-prop-7 .statement}

— Let T be a completely regular space. Let $\mu$ be a bounded positive measure on T, and let f be a bounded positive function on T, such that the set of points of T where f is not continuous is locally $\mu$-negligible. Then the mapping $\lambda \mapsto \lambda^*(f)$ of $\mathcal{M}_+^b(T)$ into $\mathbf{R}$ is continuous at the point $\mu$.

For every $t \in T$, set $f'(t) = \liminf_{s \to t} f(s)$, $f''(t) = \limsup_{s \to t} f(s)$. Obviously $f' \leqslant f \leqslant f''$, with equality at every point of T where f is continuous (hence $\mu$-almost everywhere). On the other hand, $f'$ is lower semi-continuous, $f''$ is upper semi-continuous and bounded (GT, IV, §6, No. 2, Prop. 4). We therefore have the following relations by Prop. 6,

$$
\mu^*(f') \leqslant \liminf_{\lambda \to \mu} \lambda^*(f') \leqslant \liminf_{\lambda \to \mu} \lambda^*(f) \leqslant \mu^*(f) \leqslant \limsup_{\lambda \to \mu} \lambda^*(f)
$$
$$
\leqslant \limsup_{\lambda \to \mu} \lambda^*(f'') \leqslant \mu^*(f'').
$$

One concludes by observing that $\mu^*(f') = \mu^*(f'')$, because $f'$ and $f''$ are equal locally $\mu$-almost everywhere.

#### Proposition 8 {#int-ix-s5-prop-8 .statement}

— Let X be a completely regular space, T a subspace of X, and i the canonical injection of T into X. Denote by W the set of bounded positive measures on X that are concentrated on T, equipped with the topology induced by $\mathcal{M}^b(X)$. Then the mapping $\mu \mapsto i(\mu)$ of $\mathcal{M}_+^b(T)$ into $\mathcal{M}^b(X)$ is a homeomorphism of $\mathcal{M}_+^b(T)$ onto W.

We denote again by i the mapping $\mu \mapsto i(\mu)$ of $\mathcal{M}_+^b(T)$ into $\mathcal{M}_+^b(X)$; i is injective (§2, No. 4, Prop. 8) and maps $\mathcal{M}_+^b(T)$ into W (§2, No. 3, Prop. 7). If $\lambda \in W$, then $\lambda = i(\lambda_T)$ (§2, No. 3, Prop. 7 b)). Consequently, i is a bijection of $\mathcal{M}_+^b(T)$ onto W, and the inverse bijection of i is the mapping $r : \lambda \mapsto \lambda_T$ on $W$. On the other hand, $i$ is continuous: for, if $f \in \mathcal{C}^b(X)$, then $\langle i(\mu), f \rangle = \langle \mu, f \circ i \rangle$, and $f \circ i$ belongs to $\mathcal{C}^b(T)$. Thus, everything comes down to showing that, for every measure $\mu \in W$ and every function $f \in \mathcal{C}^b_+(T)$, one has

$$
\lim_{\lambda \to \mu, \lambda \in W} \lambda_T(f) = \mu_T(f),
$$

or again

$$
\lim_{\lambda \to \mu, \lambda \in W} \lambda(f^0) = \mu(f^0).
$$

Let $f^\infty$ be the function on $X$ that coincides with $f$ on $T$ and with $+\infty$ on $X - T$, and let $f'$ and $f''$ be, respectively, the upper semi-continuous regularization of $f^0$ and the lower semi-continuous regularization of $f^\infty$ (GT, IV, §6, No. 2). The relations

$$
f'(x) = \limsup_{y \to x} f^0(y), \quad f''(x) = \liminf_{y \to x} f^\infty(y)
$$

immediately imply that $f'$ and $f''$ both coincide with $f$ and $f^0$ on $T$. Prop. 6 then yields

$$
\mu^\bullet(f') \geq \limsup_{\lambda \to \mu, \lambda \in W} \lambda^\bullet(f'), \quad \mu^\bullet(f'') \leq \liminf_{\lambda \to \mu, \lambda \in W} \lambda^\bullet(f'').
$$

But one can replace $f'$ and $f''$ by $f^0$ in these two formulas, since the measures $\lambda$ and $\mu$ are carried by $T$; we have thus obtained the desired relation.

The statement of Prop. 8 is only valid for positive measures: the mapping $\mu \mapsto i(\mu)$ of $\mathcal{M}^b(T)$ into $\mathcal{M}^b(X)$ is injective and continuous, but is not in general a homeomorphism of $\mathcal{M}^b(T)$ onto its image. For example, take $X = \mathbf{R}$, $T = \mathbf{R} - \{0\}$; the measures $\lambda_t = \varepsilon_t - \varepsilon_{-t}$ ($t > 0$) converge tightly to 0 in $X$ as $t$ tends to 0, but do not converge tightly to 0 in $T$ (the characteristic function of $]0, +\infty[$ belongs to $\mathcal{C}^b(T)$) (cf. however the Cor. of Th. 1 of No. 5).

#### Proposition 9 {#int-ix-s5-prop-9 .statement}

— *Let T be a locally compact space, and let $\mathfrak{F}$ be a filter on $\mathcal{M}^b_+(T)$ that converges vaguely to a bounded measure $\mu$. For $\mathfrak{F}$ to converge tightly to $\mu$, it is necessary and sufficient that $\lim_{\lambda} \lambda(1) = \mu(1)$ with respect to $\mathfrak{F}$.*

The condition is obviously necessary. To show that it is sufficient, let us denote by $X$ the Alexandroff compactification of $T$ (GT, I, §9, No. 8) and by $i$ the canonical injection of $T$ into $X$. By Prop. 8, everything comes down to showing that $\lambda \mapsto i(\lambda)$ converges tightly to $i(\mu)$ in $\mathcal{M}^b(X)$ with respect to $\mathfrak{F}$. Since $\mu(1) < +\infty$, there exists a set $A \in \mathfrak{F}$ such that the total masses of the measures in $A$ are bounded by a number $M$; it therefore suffices to verify that

$$
\lim_{\lambda, \mathfrak{F}} \int_X g \, d(i(\lambda)) = \int_X g \, d(i(\mu))
$$

for functions $g \in \mathcal{C}^b(X)$ forming a total set in $\mathcal{C}^b(X)$. Now, this equality is satisfied when $g$ has compact support in $T$, because of the vague convergence of $\mathfrak{F}$ to $\mu$, and also when $g$ is a constant function on $X$, from the fact that $\lim_{\lambda, \mathfrak{F}} \lambda(1) = \mu(1)$. Since the functions of the preceding two types form a total set in $\mathcal{C}^b(X)$ (Ch. III, §1, No. 2, Prop. 3), this completes the proof.

### 4. Application: topological properties of the space $\mathcal{M}_+^b(T)$

We first observe that if $T$ is completely regular, then $\mathcal{M}^b(T)$ is a Hausdorff topological vector space, hence is completely regular. Consequently, $\mathcal{M}_+^b(T)$ is completely regular.

#### Proposition 10 {#int-ix-s5-prop-10 .statement}

*Let $T$ be a Polish space; the space $\mathcal{M}_+^b(T)$ is then Polish for the tight topology.*

We begin by treating the case that $T$ is Polish and *compact*. The set $U$ of positive measures with mass $\leq 1$ is then compact (Ch. III, §1, No. 9, Cor. 2 of Prop. 15), and the topology induced on $U$ by the tight topology (which here coincides with the vague topology) is also induced by the topology of pointwise convergence on a total subset of $\mathcal{C}(T)$ (*loc. cit.*, No. 10, Prop. 17). Now, there exists in $\mathcal{C}(T)$ a countable total set (GT, X, §3, No. 3, Th. 1); consequently, $U$ is a metrizable compact space. The set $V$ of positive measures of mass $< 1$ is open in $U$, hence is a Polish locally compact space. Now, the mapping $\mu \mapsto \frac{1}{1 + \mu(1)} \mu$ of $\mathcal{M}_+^b(T)$ onto $V$ is a homeomorphism, the mapping $\lambda \mapsto \frac{1}{1 - \lambda(1)} \lambda$ being the inverse homeomorphism.

Let us pass to the case that $T$ is Polish; we can suppose that $T$ is the intersection of a decreasing sequence $(G_n)$ of open sets in a metrizable compact space $X$ (GT, IX, §6, No. 1, Cor. 1 of Th. 1); the space $\mathcal{M}_+^b(T)$ is then homeomorphic to the subspace $W$ of $\mathcal{M}_+^b(X)$ consisting of the measures concentrated on $T$ (No. 3, Prop. 8), and it will suffice to show that $W$ is the intersection of a sequence of open sets in the Polish space $\mathcal{M}_+^b(X)$ (GT, *loc. cit.*, Th. 1). Now, let $W_n$ be the set of measures $\mu \in \mathcal{M}_+^b(X)$ concentrated on $G_n$; the mapping $h_n : \mu \mapsto \mu^*(X - G_n)$ on $\mathcal{M}_+^b(X)$ is upper semi-continuous (No. 3, Prop. 6), and the set $A_k^n$ of measures $\mu \in \mathcal{M}_+^b(X)$ such that $h_n(\mu) < 1/k$ is therefore open for every $k \geq 1$ and every $n \in \mathbf{N}$. The proof is completed by observing that $W = \bigcap_n W_n = \bigcap_{n,k} A_k^n$.

#### Corollary 1 {#int-ix-s5-prop-10-cor-1 .statement}

*If T is a metrizable space of countable type, then $\mathcal{M}_+^b(T)$ is metrizable of countable type for the tight topology.*

For, let $\hat{T}$ be the completion of T for a metric defining the topology of T; the space $\hat{T}$ is Polish, and $\mathcal{M}_+^b(T)$ is homeomorphic to the subspace of the Polish space $\mathcal{M}_+^b(\hat{T})$ consisting of the measures concentrated on T (No. 3, Prop. 8). But every subspace of a Polish space is metrizable of countable type (GT, IX, §2, No. 8).

#### Corollary 2 {#int-ix-s5-prop-10-cor-2 .statement}

*If T is a completely regular Souslin (resp. Lusin) space, then the space $\mathcal{M}_+^b(T)$ is Souslin (resp. Lusin).*

For, consider a Polish space P and a continuous mapping $f$ of P onto T (GT, IX, §6, No. 2, Def. 2). Let $\tilde{f}$ be the continuous mapping $\mu \mapsto f(\mu)$ of $\mathcal{M}_+^b(P)$ into $\mathcal{M}_+^b(T)$; the space $\mathcal{M}_+^b(P)$ is Polish by Prop. 10, and $\tilde{f}$ is surjective (§2, No. 4, Prop. 9); the space $\mathcal{M}_+^b(T)$ is therefore Souslin. Similarly, if T is Lusin, then $f$ may be assumed to be injective (GT, *loc. cit.*, No. 4, Prop. 12); then $\tilde{f}$ is injective (§2, No. 4, Prop. 8), and so $\mathcal{M}_+^b(T)$ is Lusin (GT, *loc. cit.*, No. 4, Prop. 12).

Let T be a completely regular Souslin space (recall that for this, it suffices that T be Souslin and *regular* (TG, App. 1, Cor. of Prop. 2)), and let H be a compact subset of $\mathcal{M}_+^b(T)$; then H is compact and Souslin, hence *metrizable*, for the tight topology (*loc. cit.*, App. 1, Cor. 2 of Prop. 3).

### 5. Compactness criterion for tight convergence

#### Definition 2 {#int-ix-s5-def-2 .statement}

*Let T be a topological space, and let H be a subset of $\mathcal{M}^b(T)$; one says that H satisfies Prokhorov’s condition if*
    a) $\sup_{\mu \in H} |\mu|(1) < +\infty$;
    b) *for every number $\varepsilon > 0$, there exists a compact subset $K_\varepsilon$ of T such that*
    $$
    |\mu|(T - K_\varepsilon) \leq \varepsilon \quad \text{for every measure } \mu \in H.
    $$

It can be shown that if T is completely regular, the set of conditions *a)* and *b)* is equivalent to the following condition: there exists a real function $f \geq 1$ on T, such that the set of points t of T satisfying $f(t) \leq c$ is compact for every $c \in \mathbf{R}_+$ (which in particular implies that $f$ is lower semi-continuous), and such that $\sup_{\mu \in H} |\mu|(f) < +\infty$. Moreover, when T is locally compact, one obtains an equivalent statement by requiring f to be continuous (cf. Exer. 10).

#### Proposition 11 {#int-ix-s5-prop-11 .statement}

*Let T be a completely regular space, and let H be a subset of $\mathcal{M}^b(T)$ that satisfies Prokhorov’s condition; then its closure $\overline{H}$ in $\mathcal{M}^b(T)$ satisfies Prokhorov’s condition.*

For, the functions $\mu \mapsto |\mu|^*(1)$, $\mu \mapsto |\mu|^*(T - K_\varepsilon)$ are lower semi-continuous on $\mathcal{M}^b(T)$ by Prop. 6 of No. 3.

The interest of Prokhorov’s condition comes from the following theorem, whose converse will be studied later on (Th. 2).

**Theorem 1 (Prokhorov).** — *Let T be a completely regular space, and let H be a subset of $\mathcal{M}^b(T)$ that satisfies Prokhorov’s condition; then H is relatively compact in $\mathcal{M}^b(T)$ for the tight topology.*

We can suppose that T is a subspace of a compact space X; let i be the canonical injection of T into X. We can on the other hand suppose that H is *closed* in $\mathcal{M}^b(T)$, by Prop. 11. It will then suffice to show that every ultrafilter $\mathfrak{U}$ on H converges in $\mathcal{M}^b(T)$.

We shall begin with the case that $H \subset \mathcal{M}_+^b(T)$. The total masses of the measures $\mu \in H$ being bounded by hypothesis, $i(\mu)$ converges vaguely with respect to $\mathfrak{U}$, in $\mathcal{M}_+(X)$, to a measure $\nu \in \mathcal{M}_+(X)$ (Ch. III, §1, No. 9, Cor. 2 of Prop. 15); by Prop. 8 of No. 3, everything comes down to proving that $\nu$ is concentrated on T. Now, let $\varepsilon$ be a number $> 0$, and let $K_\varepsilon$ be a compact subset of T satisfying the formula (6). Since $X - K_\varepsilon$ is open in X, we have, by Prop. 6 of No. 3 applied in X, the inequalities

$$
\nu^*(X - T) \leq \nu^*(X - K_\varepsilon) \leq \liminf_{\mu, \mathfrak{U}} i(\mu)^*(X - K_\varepsilon)
= \liminf_{\mu, \mathfrak{U}} \mu^*(T - K_\varepsilon) \leq \varepsilon;
$$

since $\varepsilon > 0$ is arbitrary, the theorem is established in this special case.

Let us pass to the general case; for every measure $\mu$ on T, set

$$
a_1(\mu) = \Re(\mu)^+, \quad a_2(\mu) = \Re(\mu)^-, \quad a_3(\mu) = \Im(\mu)^+, \quad a_4(\mu) = \Im(\mu)^-;
$$

since $\mu = a_1(\mu) - a_2(\mu) + ia_3(\mu) - ia_4(\mu)$, it will suffice to show that the mappings $a_j$ ($j = 1, 2, 3, 4$) converge tightly with respect to $\mathfrak{U}$. But the set $H_j$ of measures $a_j(\mu)$, where $\mu$ runs over H, satisfies Prokhorov’s condition by virtue of the relation $|a_j(\mu)| \leq |\mu|$, and is contained in $\mathcal{M}_+^b(T)$; it is therefore relatively compact in $\mathcal{M}_+^b(T)$ by the special case, and the theorem then follows at once.

#### Corollary {#int-ix-s5-n5-cor-1 .statement}

— Let T be a subspace of a completely regular space X, and let H be a subset of $\mathcal{M}^b(T)$ that satisfies Prokhorov’s condition. If i denotes the canonical injection of T into X, then the restriction to H of the mapping $\mu \mapsto i(\mu)$ of $\mathcal{M}^b(T)$ into $\mathcal{M}^b(X)$ is a homeomorphism of H onto its image.

It suffices to treat the case that H is closed (Prop. 11), hence compact; the conclusion then follows from the fact that $\mu \mapsto i(\mu)$ is continuous and injective.

Recall that this result is also valid for an arbitrary subset of $\mathcal{M}_+^b(T)$ (No. 3, Prop. 8).

#### Theorem 2 {#int-ix-s5-thm-2 .statement}

— Let T be a locally compact space, or a Polish space, and let H be a relatively compact subset of $\mathcal{M}_+^b(T)$; then H satisfies Prokhorov’s condition.

We may restrict ourselves to the case that H is closed, hence compact. The total masses of the measures $\mu \in H$ are obviously bounded, because the mapping $\mu \mapsto \mu(1)$ is continuous, and everything comes down to proving the assertion b) of Def. 2.

Suppose first that T is locally compact. Let $\varepsilon$ be a number > 0. Let us associate to every measure $\mu \in H$ a compact set $K_\mu$ in T such that $\mu^\bullet(T - K_\varepsilon) < \varepsilon$, then a relatively compact open neighborhood $U_\mu$ of $K_\mu$. The function $\lambda \mapsto \lambda^\bullet(T - U_\mu)$ being upper semi-continuous on $\mathcal{M}_+^b(T)$ (No. 3, Prop. 6), the set $V^\mu$ of measures $\lambda \in H$ such that $\lambda^\bullet(T - U_\mu) < \varepsilon$ is a neighborhood of $\mu$ in H. Therefore there exists a finite subset $H'$ of H such that the sets $V^\mu$ ($\mu \in H'$) cover H. Denoting by K the compact set $\bigcup_{\mu \in H'} \overline{U}_\mu$, we have $\lambda^\bullet(T - K) < \varepsilon$ for all $\lambda \in H$.

Suppose next that T is Polish. We do not restrict the generality by assuming that T is the intersection of a decreasing sequence $(T_p)_{p \geq 1}$ of open subsets of a compact space X (GT, IX, §6, No. 1, Cor. 1 of Th. 1). Let $i_p$ be the injection of T into $T_p$, and let $H_p$ be the set of measures of the form $i_p(\lambda)$ for $\lambda \in H$; since $H_p$ is compact in $\mathcal{M}_+^b(T_p)$, it follows that there exists a compact set $K_p \subset T_p$ such that $\nu^\bullet(T_p - K_p) \leq \varepsilon 2^{-p}$ for every measure $\nu \in H_p$, by the preceding result applied to the locally compact space $T_p$. Therefore also $\nu^\bullet(T - (T \cap K_p)) \leq \varepsilon 2^{-p}$, and finally $\lambda^\bullet(T - (T \cap K_p)) \leq \varepsilon 2^{-p}$ for every measure $\lambda \in H$. Now set $K = \bigcap_p K_p$; the set K is compact and is contained in T, and, for every measure $\lambda \in H$, we have $\lambda^\bullet(T - K) \leq \sum_p \lambda^\bullet(T - (T \cap K_p)) \leq \sum_p \varepsilon 2^{-p} = \varepsilon$. Prokhorov’s condition is thus verified.

### 6. Tight convergence of measures and compact convergence of functions

#### Proposition 12 {#int-ix-s5-prop-12 .statement}

— Let T be a completely regular space, and let B be the unit ball of the normed space $\mathcal{C}^b(T; \mathbf{C})$. Let I be a linear form on $\mathcal{C}^b(T; \mathbf{C})$. In order that there exist a bounded complex measure $\theta$ on T such that $I(f) = \theta(f)$ for all $f \in \mathcal{C}^b(T; \mathbf{C})$, it is necessary and sufficient that the restriction of I to B be continuous for the topology of compact convergence. The measure $\theta$ is then unique.

Let us show that the condition in the statement is necessary. Let $\theta$ be a bounded complex measure on T, $\varepsilon$ a number $> 0$, and K a compact subset of T such that $|\theta|^*(T - K) < \varepsilon$. Let $f \in B$; we denote by U the neighborhood of $f$ in B for the topology of compact convergence, formed by the functions $g \in B$ such that $\sup_{x \in K} |g(x) - f(x)| \leq \varepsilon$. Then, for every $g \in U$,

$$
|\theta(g) - \theta(f)| \leq \int_T |g - f| d|\theta| \leq \varepsilon |\theta|^*(K) + 2|\theta|^*(T - K) \leq (||\theta|| + 2)\varepsilon ,
$$

because $|g - f|$ is bounded above by $\varepsilon$ on K and by 2 on $T - K$.

Conversely, consider a linear form I on $\mathcal{C}^b(T; \mathbf{C})$ whose restriction to B is continuous for the topology of compact convergence. Then, for every number $\varepsilon > 0$, there exist a number $a > 0$ and a compact subset K of T such that the relations $f \in B, \sup_{x \in K} |f(x)| \leq a$ imply $|I(f)| \leq \varepsilon$. Prop. 5 of No. 2 then implies the existence of a unique bounded complex measure $\theta$ such that $I(f) = \theta(f)$ for all $f \in \mathcal{C}^b(T; \mathbf{C})$.

#### Proposition 13 {#int-ix-s5-prop-13 .statement}

— Let T be a locally compact space, and H a bounded subset of the normed space $\mathcal{C}^b(T; \mathbf{C})$. The mapping $(\mu, f) \mapsto \mu(f)$ of $\mathcal{M}_+^b(T) \times H$ into $\mathbf{C}$ is then continuous, when $\mathcal{M}_+^b(T)$ is equipped with the tight topology, and H with the topology of compact convergence.

Let $\mu \in \mathcal{M}_+^b(T), f \in H$, and let M be a real number such that $||\mu|| < M$, and $|g| \leq M$ for all $g \in H$. Let $\varepsilon$ be a number $> 0$ and choose a compact subset K of T such that $\mu^*(T - K) < \varepsilon$, then a relatively compact open neighborhood S of K. The set U of measures $\lambda \in \mathcal{M}_+^b(T)$ satisfying the inequalities

$$
\lambda^*(T) < M , \quad \lambda^*(T - S) < \varepsilon , \quad |\lambda(f) - \mu(f)| < \varepsilon
$$

is then a neighborhood of $\mu$ in $\mathcal{M}_+^b(T)$ (No. 3, Prop. 6). In addition, let V be the neighborhood of $f$ in H consisting of the functions $g \in H$ such that

$$
\sup_{x \in S} |g(x) - f(x)| < \varepsilon .
$$

Let $\lambda \in U$ and $g \in V$; since the function $|g - f|$ is bounded above by $\varepsilon$ in $S$, and by $2M$ in $T - S$, we have
$$
|\lambda(g) - \lambda(f)| \leq \int_T |g - f| d\lambda \leq \varepsilon \lambda^*(S) + 2M \lambda^*(T - S) \leq 3M \varepsilon,
$$
from which one deduces
$$
|\lambda(g) - \mu(f)| \leq |\lambda(g) - \lambda(f)| + |\lambda(f) - \mu(f)| \leq (3M + 1)\varepsilon.
$$
This proves the continuity of the mapping $(\lambda, g) \mapsto \lambda(g)$ at the point $(\mu, f)$ of $\mathcal{M}_+^b(T) \times H$.

#### Remark {#int-ix-s5-n6-rem-1 .statement}

Let $T$ be a completely regular space, $M$ a subset of $\mathcal{M}^b(T)$ that satisfies Prokhorov’s condition, $H$ a bounded subset of $C^b(T)$. An argument very close to the one just made may be used to prove that the mapping $(\lambda, g) \mapsto \lambda(g)$ of $M \times H$ into $\mathbf{C}$ is continuous when $M$ is equipped with the tight topology and $H$ with the topology of compact convergence.

#### Corollary {#int-ix-s5-n6-cor-1 .statement}

*Let $T$ be a completely regular space, $X$ a topological space, and $f$ a complex-valued function defined on $T \times X$, continuous and bounded. For every bounded measure $\mu$ on $T$, let $F_\mu$ be the function on $X$ defined by $F_\mu(x) = \int_T f(t, x) d\mu(t)$ for all $x \in X$.

a) The function $F_\mu$ is continuous and bounded for every bounded measure $\mu$.

b) Suppose that $T$ is locally compact. The mapping $\mu \mapsto F_\mu$ of $\mathcal{M}_+^b(T)$ into $C^b(X; \mathbf{C})$ is then continuous, if $\mathcal{M}_+^b(T)$ is equipped with the tight topology, and $C^b(X; \mathbf{C})$ with the topology of compact convergence.

For every $x \in X$, denote by $f_x$ the continuous and bounded function $t \mapsto f(t, x)$ on $T$; the mapping $x \mapsto f_x$ of $X$ into $C^b(T; \mathbf{C})$ has bounded image, and it is continuous if $C^b(T; \mathbf{C})$ is equipped with the topology of compact convergence (GT, X, §3, No. 4, Th. 3). Since $F_\mu(x) = \mu(f_x)$, the function $F_\mu$ is continuous by Prop. 12. Suppose $T$ is locally compact; Prop. 13 shows that the mapping $(\mu, x) \mapsto F_\mu(x)$ of $\mathcal{M}_+^b(T) \times X$ into $\mathbf{C}$ is continuous; the assertion b) follows from this (*loc. cit.*).

### 7. Application: the Laplace transformation

In this No., we denote by $M$ a commutative monoid, whose law of composition is written additively, equipped with the topology of a *locally compact* space, for which the mapping $(m, m') \mapsto m + m'$ of $M \times M$ into $M$ is continuous. The neutral element of $M$ is denoted by $0$. One calls *character* of $M$ every bounded continuous complex function $\chi$ on $M$ satisfying the relations
$$
\chi(m + m') = \chi(m) \cdot \chi(m'), \quad \chi(0) = 1, \quad |\chi(m)| \leq 1
$$

for $m, m'$ in $M$. If $\chi$ and $\chi'$ are characters, then so is $\chi \chi'$. The set of characters of $M$ is a monoid, denoted $X$; equip it with the topology of compact convergence, for which the mapping $(\chi, \chi') \mapsto \chi \chi'$ of $X \times X$ into $X$ is continuous. The neutral element of $X$ is the constant function 1.

For every bounded complex measure $\mu$ on $M$, one calls *Laplace transform* of $\mu$ the function $\mathcal{L}\mu$ on $X$ defined by

$$
(\mathcal{L}\mu)(\chi) = \int_M \chi(m)\, d\mu(m).
$$

By Th. 3 of GT, X, §3, No. 4, the mapping $(m, \chi) \mapsto \chi(m)$ of $M \times X$ into $\mathbf{C}$ is continuous and bounded. The corollary of Prop. 13 of No. 6 then implies the following result:

#### Proposition 14 {#int-ix-s5-prop-14 .statement}

*For every bounded complex measure $\mu$ on $M$, the function $\mathcal{L}\mu$ on $X$ is continuous and bounded. If $\mathcal{M}_+^b(M)$ is equipped with the tight topology and $\mathcal{C}^b(X; \mathbf{C})$ with the topology of compact convergence, the mapping $\mu \mapsto \mathcal{L}\mu$ of $\mathcal{M}_+^b(M)$ into $\mathcal{C}^b(X; \mathbf{C})$ is continuous.*

The set of characters of $M$ that tend to 0 at infinity will be denoted $X_0$; this set is stable under multiplication. We shall say that a submonoid$^{(1)}$ S of $X$ is *full* if S is stable for the mapping $\chi \mapsto \overline{\chi}$, $S \cap X_0$ separates the points of $M$ (GT, X, §4, No. 1, Def. 1) and if, given any $m \in M$, there exists an element $\chi$ of $S \cap X_0$ such that $\chi(m) \neq 0$.

Suppose in addition that $M$ is a noncompact abelian *group*. Let $f$ be a function on $M$ that tends to 0 at infinity; the same is then true of the function $x \mapsto f(x)f(-x)$ on $M$, whereas every character $\chi$ of $M$ satisfies $\chi(x)\chi(-x) = \chi(0) = 1$. It follows that $X_0$ is empty, and that $X$ does not contain any full submonoid. Thus, Theorem 3 below does not apply to locally compact groups that are not compact.

#### Theorem 3 {#int-ix-s5-thm-3 .statement}

*Let S be a full submonoid of X.*
a) *If $\mu$ and $\mu'$ are two bounded complex measures on $M$, such that $\mathcal{L}\mu$ and $\mathcal{L}\mu'$ have the same restriction to $S \cap X_0$, then $\mu = \mu'$.*
b) *Let $\mathfrak{F}$ be a filter on $\mathcal{M}_+^b(M)$, such that $\mathcal{L}\lambda(s)$ has a limit $\Phi(s) \in \mathbf{C}$ with respect to $\mathfrak{F}$ for every $s \in S$. Then the filter $\mathfrak{F}$ converges vaguely to a bounded positive measure $\mu$, and $\Phi(s) = \mathcal{L}\mu(s)$ for all $s \in S \cap X_0$.*
c) *Under the hypotheses of b), suppose in addition that the closure of $S \cap X_0$ contains 1, and that the function $\Phi$ on $S$ is continuous at the point 1. Then $\mathfrak{F}$ converges tightly to $\mu$, and $\Phi(s) = \mathcal{L}\mu(s)$ for all $s \in S$.*

We shall denote by E the algebra of continuous complex functions tending to 0 at infinity on $M$, and by $\mathfrak{A}$ the linear subspace of E generated

(1) Recall that a submonoid of a monoid A contains by definition the neutral element of A (A, I, §2, No. 1).

by $S \cap X_0$; then $\mathfrak{A}$ is a subalgebra of $E$ stable under the mapping $f \mapsto \overline{f}$; since $S$ is a full submonoid of $X$, Cor. 2 of Prop. 7 of GT, X, §4, No. 4 implies that $\mathfrak{A}$ is dense in $E$.

Let us prove a): by hypothesis, $\mu(f) = \mu'(f)$ for every $f \in \mathfrak{A}$; since $\mu$ and $\mu'$ are continuous linear forms on $E$, this implies that $\mu(f) = \mu'(f)$ for $f \in E$, and in particular for every continuous function $f$ with compact support, whence $\mu = \mu'$.

Let us place ourselves under the hypotheses of b). The number $\Phi(1) = \lim_{\lambda, \mathfrak{F}} \lambda(1)$ is real and positive; let there be given a real number $a > \Phi(1)$; since $\| \lambda \| = \mathcal{L} \lambda(1)$ for $\lambda \in \mathcal{M}_+^b(M)$, the relation $\lim_{\lambda, \mathfrak{F}} \mathcal{L} \lambda(1) = \Phi(1)$ implies that the set $H$ of measures $\lambda \in \mathcal{M}_+^b(M)$ such that $\| \lambda \| \leq a$ belongs to $\mathfrak{F}$. Since $\mathcal{M}^b(M; \mathbf{C})$ may be identified with the dual of the normed space $E$ (Ch. III, §1, No. 8 & §1, No. 2, Prop. 3), the space $H$ is compact for the topology $\sigma(\mathcal{M}^b(M; \mathbf{C}), E)$. On the other hand (TVS, III, §3, No. 4, Prop. 5), this topology coincides on $H$ with the topology of pointwise convergence in any total subset of $E$. In particular, since $\mathfrak{A}$ is dense in $E$, and the same is true of the space of continuous functions with compact support (Ch. III, §1, No. 2, Prop. 3), the topology of pointwise convergence in $S \cap X_0$ coincides on $H$ with the vague topology, and $H$ is compact for this topology. It follows at once that $\mathfrak{F}$ converges vaguely to a measure $\mu \in H$, and that $\mathcal{L} \mu(s) = \lim_{\lambda, \mathfrak{F}} \mathcal{L} \lambda(s)$ for all $s \in S \cap X_0$.

Finally, let us pass to c). Since the functions $\Phi$ and $\mathcal{L} \mu$ are continuous at the point $1 \in S$, and equal on $S \cap X_0$, and since $1$ is in the closure of $S \cap X_0$, we have $\Phi(1) = \mathcal{L} \mu(1)$. In other words, $\lim_{\lambda, \mathfrak{F}} \lambda(1) = \mu(1)$. Prop. 9 of No. 3 then shows that $\mu$ is the tight limit of the filter $\mathfrak{F}$. Every element of $S$ being a bounded continuous function on $M$, this implies that $\Phi(s) = \lim_{\lambda, \mathfrak{F}} \lambda(s) = \mu(s) = \mathcal{L} \mu(s)$ for all $s \in S$.

#### Corollary {#int-ix-s5-n7-cor-1 .statement}

— *Let $S$ be a full submonoid of $X$, such that the closure of $S \cap X_0$ contains 1. Let $L$ be the subset of $\mathcal{C}^b(S; \mathbf{C})$ consisting of the restrictions to $S$ of the Laplace transforms of the measures $\lambda \in \mathcal{M}_+^b(M)$.*

a) *The set $L$ is closed in the space $\mathcal{C}^b(S; \mathbf{C})$ equipped with the topology of pointwise convergence.*

b) *The mapping $\lambda \mapsto (\mathcal{L} \lambda)_S$ is a homeomorphism of $\mathcal{M}_+^b(M)$ onto $L$, if $\mathcal{M}_+^b(M)$ is equipped with the tight topology and $L$ with the topology of pointwise convergence.*

c) *The topology of pointwise convergence and the topology of compact convergence coincide on $L$.*

The assertions a) and b) are immediate consequences of Th. 3; the assertion c) follows from b) and Prop. 14, since the topology of compact convergence is finer than that of pointwise convergence.

One must be on guard that L is not closed in the set of all bounded complex functions on S, equipped with the topology of pointwise convergence. Assume for example the notations of Example 2 below (M = \mathbf{R}_+, S identified with \mathbf{R}_+). The Laplace transforms of the measures $\varepsilon_n$ ($n \in \mathbf{N}$) are the functions $t \mapsto e^{-nt}$ on $\mathbf{R}_+$; as $n$ tends to $+\infty$, these functions converge pointwise to the function equal to 1 for $t = 0$ and to 0 for $t \neq 0$, which does not belong to L.

*Example 1).* — Take for M the set N of positive integers, equipped with the law of addition and with the discrete topology. Let D be the unit disc of \mathbf{C} (the set of complex numbers of absolute value $\leq 1$) equipped with the topology induced by \mathbf{C} and with the law induced by multiplication. For every $z \in D$, let us denote by $f(z)$ the character $n \mapsto z^n$ of N. For every character $\chi$ of N, denote by $g(\chi)$ the complex number $\chi(1) \in D$. One verifies immediately that $f$ and $g$ are mutually inverse homeomorphisms between D and X, which will permit us, from now on, to *identify* X and D. The set of characters tending to 0 at infinity may then be identified with the set $D_0$ of complex numbers of absolute value < 1. Finally, the interval ]0, 1] of \mathbf{R} is a full submonoid of D, and 1 is in the closure of $]0, 1[ \cap D_0 = ]0, 1[$.

Every measure $\mu$ on N may be written in a unique way in the form $\mu = \sum_{n \in \mathbf{N}} u_n \cdot \varepsilon^n$, and $\mu$ is bounded if and only if $\sum_n |u_n| < +\infty$; one then has $\mathcal{L}\mu(z) = \sum_{n \in \mathbf{N}} u_n z^n$ for $z \in D$. This function is continuous on D; it is customary to call it the *generating function* of the summable sequence $(u_n)_{n \in \mathbf{N}}$. Transcribed into this language, Th. 3 yields the following result (taking into account Prop. 9 of No. 3):

#### Proposition 15 {#int-ix-s5-prop-15 .statement}

*Let A be a set equipped with a filter $\mathfrak{F}$. For every $\alpha \in A$, let $(u_{\alpha,n})_{n \in \mathbf{N}}$ be a summable sequence of positive numbers, and let $\Phi_\alpha$ be the function defined on the interval ]0, 1] of \mathbf{R} by $\Phi_\alpha(x) = \sum_{n \in \mathbf{N}} u_{\alpha,n} x^n$. In order that there exist a summable sequence $(u_n)_{n \in \mathbf{N}}$ of positive numbers such that*

$$
\lim_{\alpha, \mathfrak{F}} u_{\alpha,n} = u_n \quad \text{for all } n , \quad \lim_{\alpha, \mathfrak{F}} \sum_{n \in \mathbf{N}} u_{\alpha,n} = \sum_{n \in \mathbf{N}} u_n ,
$$

*it is necessary and sufficient that $\Phi_\alpha$ converge pointwise on ]0, 1[, with respect to $\mathfrak{F}$, to a function $\Phi$ continuous at the point 1. In this case, $\Phi(x) = \sum_{n \in \mathbf{N}} u_n x^n$ for all $x \in ]0, 1[$.*

Analogous results are obtained by taking M to be the monoid $\mathbf{N}^n$, where $n$ denotes an integer > 1; the space X may then be identified with $D^n$, and one can choose $]0, 1[^n$ as the full submonoid. We leave to the reader the task of transcribing Th. 3 in this case.

Example 2). — Let us take for M the set $\mathbf{R}_+$, equipped with the law of addition and with the usual topology. Let P be the set of complex numbers z with positive real part, equipped with the topology induced by C, and with the law induced by addition in C. For every $p \in P$, denote by $f(p)$ the character $x \mapsto e^{-px}$ of $\mathbf{R}_+$; it is easily verified that $f$ is an isomorphism of the topological monoid structure of P onto that of X; we shall identify X with P by means of $f$. It is clear that $\mathbf{R}_+$ is a full submonoid of P, and Th. 3 yields the following result:

#### Proposition 16 {#int-ix-s5-prop-16 .statement}

*Let A be a set equipped with a filter $\mathcal{F}$. For every $\alpha \in A$, let $\mu_\alpha$ be a bounded positive measure on $\mathbf{R}_+$, and let $\Phi_\alpha$ be the function defined on $\mathbf{R}_+$ by $\Phi_\alpha(p) = \int_0^{+\infty} e^{-px} d\mu_\alpha(x)$. In order that the mapping $\alpha \mapsto \mu_\alpha$ converge tightly with respect to $\mathcal{F}$ to a bounded positive measure $\mu$, it is necessary and sufficient that $\Phi_\alpha$ converge pointwise on $\mathbf{R}_+$, with respect to $\mathcal{F}$, to a function $\Phi$ continuous at the point 0. In this case, $\Phi(p) = \int_0^{+\infty} e^{-px} d\mu(x)$ for all $p \in \mathbf{R}_+$.*

There are analogous results for the additive monoids $\mathbf{R}_+^n$ ($n$ an integer $> 1$); we leave to the reader the transcription of Th. 3 in this case.

### Exercises {#int-ix-s5-exercises}

See the [exercises for § 5](exercises/s5/).
