---
book: int
book_title: Integration
chapter: VI
chapter_title: VECTORIAL INTEGRATION
section: 3
section_title: Disintegration of measures
lang: en
source: int-i-vi
book_pages: INT VI.40-INT VI.51, INT VI.69-INT VI.71
pdf_pages: 0431-0442, 0460-0462
extraction: ocr
subsections:
    - "no": 1
      title: Disintegration of a measure $\mu$ relative to a $\mu$-proper mapping
      page: 40
      pdf_page: 431
    - "no": 2
      title: Pseudo-image measures
      page: 44
      pdf_page: 435
    - "no": 3
      title: Disintegration of a measure $\mu$ relative to a pseudo-image of $\mu$
      page: 45
      pdf_page: 436
    - "no": 4
      title: Measurable equivalence relations
      page: 46
      pdf_page: 437
    - "no": 5
      title: Disintegration of a measure by a measurable equivalence relation
      page: 50
      pdf_page: 441
statements: 16
exercises: 12
content_sha256: 6c7c7d84bc3a47a89cf864e928daf459d8ae1ed8bb404a27eaa408e6c0c22b3a
---

## § 3. DISINTEGRATION OF MEASURES

### 1. Disintegration of a measure $\mu$ relative to a $\mu$-proper mapping

Let T be a locally compact space having a countable base (in other words, a locally compact Polish space (GT, IX, §6, No. 1). We know that for every positive measure on T, the concepts of integral and essential integral coincide (Ch. V, §1, No. 3, Cor. of Prop. 9). On the other hand, we have the following properties:

#### Lemma 1 {#int-vi-s3-lem-1 .statement}

*If Y is a locally compact space with a countable base, the space $\mathcal{H}(Y)$ contains a countable dense subset. More precisely, there exists in $\mathcal{H}(Y)$ a countable subset S consisting of functions $\geq 0$, such that, for every function $f \geq 0$ of $\mathcal{H}(Y)$, there exists a sequence of functions $f_n \in S$ ($n \geq 0$) that converges uniformly to $f$ and is such $f_n \leq f_0$ for all $n \geq 0$.

For, Y is the union of an increasing sequence $(U_n)$ of relatively compact open sets such that $\overline{U}_n \subset U_{n+1}$ for all $n$ (GT, I, §9, No. 9, Prop. 15); the space $\mathcal{H}(Y)$ is the union of the increasing sequence of Banach spaces $\mathcal{H}(Y, \overline{U}_n)$, and each of the latter is known to be separable (GT, Ch. X, §3, No. 3, Th. 1). Let $S'_n$ be a countable dense set in $\mathcal{H}(Y, \overline{U}_n)$, $S_n$ the set of functions $\varphi^+$ for $\varphi \in S'_n$, and $u_n$ a function in $\mathcal{H}(Y, \overline{U}_{n+1})$, with values in $[0, 1]$ and equal to 1 on $U_n$. We take for S the union of the $S_n$ and the set of $m u_n$ for $m$ and $n$ integers $\geq 0$. For every function $f \geq 0$ of $\mathcal{H}(Y)$, $f$ has support contained in one of the $U_n$, hence is the uniform limit of a sequence of functions $f_p \in S_n$ ($p \geq 1$). These functions $f_p$ are uniformly bounded by a positive integer $m$, and it suffices to take $f_0 = m u_n$.*

#### Lemma 2 {#int-vi-s3-lem-2 .statement}

*If T is a locally compact space with a countable base, then the Banach space $\mathcal{K}(Y)$ of continuous numerical functions tending to 0 at the point at infinity is separable.*

This lemma is none other than the Cor. to Th. 1 of GT, X, §3, No. 3. One may observe that it also follows from Lemma 1 and the fact that the topology of uniform convergence on $\mathcal{K}(Y)$ is coarser than the direct limit topology of the topologies of the subspaces $\mathcal{K}(Y, \overline{U}_n)$.

#### Lemma 3 {#int-vi-s3-lem-3 .statement}

— *Let T and X be two locally compact spaces with countable bases, $\mu$ a positive measure on T, and $t \mapsto \lambda_t$ ($t \in T$) a family of positive measures on X. If the mapping $t \mapsto \lambda_t$ is scalarly $\mu$-integrable (for the topology $\sigma(\mathcal{M}(X), \mathcal{K}(X))$), then the family $t \mapsto \lambda_t$ is $\mu$-adequate ($\S 1$, No. 1, Example).*

For, Lemma 1, applied to $\mathcal{K}(X)$, shows that the mapping $t \mapsto \lambda_t$ is vaguely $\mu$-measurable ($\S 1$, No. 5, Prop. 13).

#### Theorem 1 {#int-vi-s3-thm-1 .statement}

*Let T and B be two locally compact spaces having countable bases, $\mu$ a positive measure on T, p a $\mu$-proper mapping (Ch. V, §6, No. 1, Def. 1) of T into B, and $\nu = p(\mu)$ the image of $\mu$ under p. Then there exists a $\nu$-adequate family ($\S 1$, No. 1, Example) $b \mapsto \lambda_b$ ($b \in B$) of positive measures on T, having the following properties:

a) $\| \lambda_b \| = 1$ for all $b \in p(T)$;

b) $\lambda_b$ is concentrated on the set $\overline{p}^{-1}(b)$ (Ch. V, §5, No. 7, Def. 4) for all $b \in B$; in particular, $\lambda_b = 0$ for $b \notin p(T)$;

c) $\mu = \int \lambda_b d\nu(b)$.

Moreover, if $b \mapsto \lambda'_b$ ($b \in B$) is a second $\nu$-adequate family of positive measures on T having the properties b) and c), then $\lambda'_b = \lambda_b$ almost everywhere in B for the measure $\nu$.

1) *Uniqueness.* For every function $f \in \mathcal{K}(B)$, $f \circ p$ is $\mu$-integrable since p is $\mu$-proper (Ch. V, §6, No. 2, Th. 1); for every function $g \in \mathcal{K}(T)$, the function $t \mapsto g(t)f(p(t))$ is therefore $\mu$-integrable. It follows (Ch. V, §3, No. 3, Th. 1) that for almost every $b \in B$, the function $t \mapsto g(t)f(p(t))$ is $\lambda_b$-integrable and that

$$
\int g(t)f(p(t)) d\mu(t) = \int d\nu(b) \int g(t)f(p(t)) d\lambda_b(t).
$$

But since $\lambda_b$ is concentrated on $\overline{p}^{-1}(b)$, we have, for every $b \in B$, $f(p(t)) = f(b)$ almost everywhere for $\lambda_b$, therefore the second member of (1) is equal to $\int f(b)\langle g, \lambda_b \rangle d\nu(b)$. The analogous formula for $\lambda'_b$ also holds; consequently $\int f(b)\langle g, \lambda_b \rangle d\nu(b) = \int f(b)\langle g, \lambda'_b \rangle d\nu(b)$ for all $f \in \mathcal{K}(B)$ and $g \in \mathcal{K}(T)$. In other words, the two mappings $b \mapsto \lambda_b$ and $b \mapsto \lambda'_b$ of B into $\mathcal{M}(T)$ are equal scalarly locally almost everywhere for $\nu$, hence equal almost everywhere for $\nu$ (Lemma 1 and §1, No. 1, Remark 2).

2) *Provisional definition of the family* $b \mapsto \lambda_b$. For every function $f \in \mathcal{L}^1(\nu)$, $f \circ p$ is $\mu$-integrable (Ch. V, §6, No. 2, Th. 1), therefore $(f \circ p) \cdot \mu$ is a bounded measure on T, and

$$
\|(f \circ p) \cdot \mu\| = \int |f \circ p| \, d\mu = \int |f| \, d\nu = N_1(f)
$$

(Ch. IV, §4, No. 7, Prop. 12; Ch. V, §5, No. 3, Th. 1 and §6, No. 2, Th. 1). It follows that $(f \circ p) \cdot \mu$ depends only on the class $\tilde{f}$ of $f$ in $L^1(\nu)$ and that $\tilde{f} \mapsto (f \circ p) \cdot \mu$ is an *isometric* linear mapping of $L^1(\nu)$ into the Banach space $\mathcal{M}^1(T)$ of bounded measures on T, the strong dual of the Banach space $\mathcal{K}(T)$, which is separable (Lemma 2). By the Dunford–Pettis theorem (§2, No. 5, Cor. 2 of Th. 1) there exists a mapping $b \mapsto \lambda_b$ of B into the unit ball of $\mathcal{M}^1(T)$, scalarly $\nu$-measurable (for the topology $\sigma(\mathcal{M}^1(T), \overline{\mathcal{K}(T)})$) and such that, for every function $f \in \mathcal{L}^1(\nu)$,

$$
(f \circ p) \cdot \mu = \int f(b) \lambda_b \, d\nu(b),
$$

which may also be written, for every function $g \in \overline{\mathcal{K}(T)}$

$$
\int g(t) f(p(t)) \, d\mu(t) = \int f(b) \, d\nu(b) \int g(t) \, d\lambda_b(t).
$$

If $f \geq 0$ and $g \geq 0$, the first member of (3) is $\geq 0$, which proves that for every function $g \geq 0$ in $\mathcal{K}(T)$, the measure $(\int g(t) \, d\lambda_b(t)) \cdot \nu$ is $\geq 0$, hence that $\int g(t) \, d\lambda_b(t) \geq 0$ except for $b$ belonging to a $\nu$-negligible set $N(g)$ (Ch. V, §5, No. 3, Cor. 3 of Prop. 3). Now, there exists a dense sequence $(g_n)$ in the space $\mathcal{K}_+(T)$ of functions $\geq 0$ of $\mathcal{K}(T)$ (Lemma 1). The union N of the $N(g_n)$ is $\nu$-negligible and, for $b \notin N$, we have $\int g_n(t) \, d\lambda_b(t) \geq 0$ for all $n$, therefore $\int g(t) \, d\lambda_b(t) \geq 0$ for every function $g \in \mathcal{K}_+(T)$, in other words $\lambda_b \geq 0$.

This being so, we may replace $\lambda_b$ by 0 for every $b \in N$ without altering the validity of (3); we can therefore assume this modification to have been made, so that $\lambda_b \geq 0$ for every $b \in B$.

3) *Extensions of the formula* (3).

$\alpha)$ For every function $f \in \mathcal{L}^1(\nu)$, it follows from (3) that the mapping $b \mapsto \lambda_b$ of B into $\mathcal{M}(T)$ is scalarly integrable for the measure $|f \cdot \nu|$ and the topology $\sigma(\mathcal{M}(T), \mathcal{K}(T))$, therefore (Lemma 3) the family $b \mapsto \lambda_b$ is $|f \cdot \nu|$-*adequate*. Now let $g$ be a numerical function defined on T, integrable for the measure $|(f \circ p) \cdot \mu|$, that is (Ch. V, §5, No. 3, Th. 1), such that $t \mapsto g(t)f((p(t)))$ is $\mu$-integrable; it then follows from (2), from Th. 1 of Ch. V, §3, No. 3 and from Th. 1 of Ch. V, §5, No. 3 that, for almost every $b \in B$, $g$ is integrable for $\lambda_b$, that the function (defined almost everywhere) $b \mapsto \int g(t)\, d\lambda_b(t)$ is integrable for $|f \cdot \nu|$, and that the formula (3) is again valid.

$\beta)$ For every function $g \in \overline{\mathcal{K}(T)}$, it follows from (3), applied to $f \in \mathcal{K}(B)$, that the mapping $p$ is proper for the measure $|g \cdot \mu|$ (Ch. V, §6, No. 1, Def. 1) and the image under $p$ of the measure $g \cdot \mu$ is the measure with density $b \mapsto \int g(t)\, d\lambda_b(t)$ with respect to $\nu$. If $f$ is then taken to be a function such that $f \circ p$ is integrable for the measure $|g \cdot \mu|$, that is, such that $t \mapsto g(t)f(p(t))$ is $\mu$-integrable (Ch. V, §5, No. 3, Th. 1), the formula (3) is again valid (Ch. V, §6, No. 2, Th. 1).

4) *Properties of the family* $b \mapsto \lambda_b$. By the property $\beta)$, we can apply formula (3) by taking $f = 1,\ g \in \mathcal{K}(T)$; this proves that $b \mapsto \lambda_b$ is scalarly $\nu$-integrable (for the topology $\sigma(\mathcal{M}(T), \mathcal{K}(T))$), hence is $\nu$-*adequate* (Lemma 3), and that $\mu = \int \lambda_b\, d\nu(b)$.

Now let $\psi$ be any function in $\mathcal{K}(B)$; the conditions of property $\alpha)$ are fulfilled by taking $f \in \mathcal{K}(B)$ and $g = \psi \circ p$, because the function $\psi(p(t))f(p(t))$ is $\mu$-integrable since $f\psi$ belongs to $\mathcal{K}(B)$ and $p$ is $\mu$-proper. Then $\psi \circ p$ is $\lambda_b$-integrable for almost every $b \in B$, and

$$
\int f(p(t))\psi(p(t))\, d\mu(t) = \int f(b)\, d\nu(b) \int \psi(p(t))\, d\lambda_b(t);
$$

but the first member is by definition $\int f(b)\psi(b)\, d\nu(b)$. We therefore see that for every function $\psi \in \mathcal{K}(B)$, the measure $\psi \cdot \nu$ and the measure with density $b \mapsto \int \psi(p(t))\, d\lambda_b(t)$ are identical. Consequently (Ch. V, §5, No. 3, Cor. 2 of Prop. 3) there exists a $\nu$-negligible set $N'(\psi)$ such that, for every $b \notin N'(\psi)$, the function $\psi \circ p$ is $\lambda_b$-integrable and $\psi(b) = \int \psi(p(t))\, d\lambda_b(t)$.

Let S be a countable subset of $\mathcal{K}(B)$ having the properties stated in Lemma 1 (with $Y = B$), and let $N'$ be the $\nu$-negligible set that is the union of the $N'(\psi)$ for $\psi \in S$. Every function $\psi \geq 0$ of $\mathcal{K}(B)$ is the uniform limit of a sequence $(\psi_n)$ of elements of S with $\psi_n \leq \psi_0$. Consequently for $b \notin N'$, Lebesgue's theorem shows on the one hand that $\psi \circ p$ is $\lambda_b$-integrable, in other words that $p$ is $\lambda_b$-proper, and on the other hand that $\psi(b) = \int \psi(p(t))\, d\lambda_b(t)$. In other terms, the mappings $b \mapsto \varepsilon_b$ and $b \mapsto p(\lambda_b)$ of B into $\mathcal{M}(B)$ (the latter being defined almost everywhere) are scalarly almost everywhere equal for $\nu$ (and for the topology $\sigma(\mathcal{M}(B), \mathcal{K}(B))$); it follows that these mappings are equal almost everywhere for $\nu$ (Lemma 1 and §1, No. 1, *Remark* 2). Finally, if $p(\lambda_b) = \varepsilon_b$, the set $B - \{b\}$ is $\varepsilon_b$-negligible, therefore the set $T - \bar{p}^{-1}(B)$ is $\lambda_b$-negligible (Ch. V, §6, No. 2, Cor. 2 of Prop. 2), in other words $\lambda_b$ is concentrated on $\overline{p}^{-1}(b)$; and, on the other hand, $\| \lambda_b \| = \int d\lambda_b = \int d((p(\lambda_b))) = \| \varepsilon_b \| = 1$ (Ch. V, §6, No. 2, Th. 1).

5) *Modifications of the family* $b \mapsto \lambda_b$. We have thus defined a $\nu$-adequate family $b \mapsto \lambda_b$ of measures $\geqslant 0$ on T, satisfying condition c) of the statement and such that, for almost every $b \in B$, $p$ is $\lambda_b$-proper, and $\lambda_b$ is concentrated on $\overline{p}^{-1}(b)$ and has norm 1. Let $N''$ be the $\nu$-negligible set of points $b \in B$ where one of the last three properties is not verified; we can then modify $\lambda_b$ in the following manner. If $b \in B - p(T)$, take $\lambda_b = 0$; if $b \in p(T) \cap N''$, take $\lambda_b = \varepsilon_{\xi(b)}$, where $\xi(b)$ is any point of $\overline{p}^{-1}(b)$. Since $B - p(T)$ is $\nu$-negligible (Ch. V, §6, No. 2, Cor. 3 of Prop. 2), we have only modified $\lambda_b$ at the points of a negligible set, consequently the family $b \mapsto \lambda_b$ is still $\nu$-adequate and has the property c); moreover, it now satisfies a) and b), which completes the proof.

Every $\nu$-adequate family $b \mapsto \lambda_b$ of positive measures on T, having the properties b) and c) of Th. 1, is said to be a *disintegration* of the measure $\mu$, relative to the $\mu$-proper mapping $p$.

### 2. Pseudo-image measures

#### Definition 1 {#int-vi-s3-def-1 .statement}

*Let T and B be two locally compact spaces, $\mu$ a positive measure on T, and p a $\mu$-measurable mapping of T into B. A positive measure $\nu$ on B is said to be a pseudo-image measure of $\mu$ under p if it satisfies the following condition: for a subset N of B to be locally $\nu$-negligible, it is necessary and sufficient that $\overline{p}^{-1}(N)$ be locally $\mu$-negligible.*

#### Example {#int-vi-s3-n2-exa-1 .statement}

— 1) If $p$ is $\mu$-proper and $\nu = p(\mu)$, then $\nu$ is a pseudo-image measure of $\mu$ under $p$ (Ch. V, §6, No. 2, Cor. 2 of Prop. 2).

2) Let $B'$ be a locally compact space, $\nu'$ a positive measure on $B'$; take for T the space $B \times B'$ and for $\mu$ the measure $\nu \otimes \nu'$; if $p$ is the projection of T onto B, then $\nu$ is a pseudo-image of $\mu$ under $p$ (Ch. V, §8, No. 2, Prop. 4 and No. 3, Cor. 1 of Prop. 7).

Note that if $\nu$ is a pseudo-image measure of $\mu$ under $p$, then $\nu$ is carried by $p(T)$.

If $\nu$ is a pseudo-image of $\mu$ under $p$, the set of measures that are pseudo-images of $\mu$ under $p$ is the class of positive measures equivalent to $\nu$, and every positive measure equivalent to $\mu$ admits the same pseudo-image measures under $p$. The class of $\nu$ is said to be the *pseudo-image class* of that of $\mu$ under $p$.

#### Proposition 1 {#int-vi-s3-prop-1 .statement}

— *Let T be a locally compact space countable at infinity, $\mu$ a positive measure on T, and $p$ a $\mu$-measurable mapping of T into a locally compact space B. Then there exists a pseudo-image measure of $\mu$ under $p$.*

For, there exists a *bounded* measure $\mu'$ on T equivalent to $\mu$ (Ch. V, §5, No. 6, Prop. 11); $p$ is then $\mu'$-proper.

### 3. Disintegration of a measure $\mu$ relative to a pseudo-image of $\mu$

#### Theorem 2 {#int-vi-s3-thm-2 .statement}

— *Let T and B be two locally compact spaces having countable bases, $\mu$ a positive measure on T, $p$ a $\mu$-measurable mapping of T into B, and $\nu$ a pseudo-image measure of $\mu$ under $p$. Then there exists a $\nu$-adequate family $b \mapsto \lambda_b$ ($b \in B$) of positive measures on T, having the following properties:
a) $\lambda_b \neq 0$ for $b \in p(T)$;
b) $\lambda_b$ is concentrated on the set $\overline{p^{-1}}(b)$ for every $b \in B$; in particular, $\lambda_b = 0$ for $b \notin p(T)$;
c) $\mu = \int \lambda_b \, d\nu(b)$.

Moreover, if $\nu' = r \cdot \nu$ is a second pseudo-image measure of $\mu$ under $p$, and if $b \mapsto \lambda'_b$ is a $\nu'$-adequate family of positive measures on T having the properties b) and c) with respect to $\nu'$, then $\lambda_b = r(b)\lambda'_b$ almost everywhere in B (*for $\nu$ or $\nu'$*).

There exists a continuous and finite numerical function $f$ defined on T, such that $f(t) > 0$ for every $t \in T$ and such that $\mu'' = f \cdot \mu$ is bounded (Ch. V, §5, No. 6, Prop. 11). Let $\nu'' = p(\mu'')$, which is equivalent to $\nu$, and write $\nu'' = g \cdot \nu$, with $g$ finite and locally $\nu$-integrable; one can suppose, moreover, that $g(b) > 0$ for all $b \in B$ (Ch. V, §5, No. 6, Prop. 10). Th. 1 of No. 1, applied to $\mu''$ and $\nu''$, shows that there exists a $\nu''$-adequate family $b \mapsto \lambda''_b$ ($b \in B$) of positive measures on T, such that:

1) $\| \lambda''_b \| = 1$ for $b \in p(T)$;
2) $\lambda''_b$ is concentrated on $\overline{p^{-1}}(b)$ for every $b \in B$;
3) $\mu'' = \int \lambda''_b \, d\nu''(b)$.

For every $b \in B$, let us define a positive measure $\lambda_b$ on T by the formula $\lambda_b = (1/f) \cdot (g(b)\lambda''_b)$. It is clear that the family $b \mapsto \lambda_b$ has the properties a) and b) of the statement. On the other hand, for every function $h \in \mathcal{K}(T)$, $h/f$ belongs to $\mathcal{K}(T)$, therefore

$$
\int h(t) \, d\mu(t) = \int (h(t)/f(t)) \, d\mu''(t) = \int d\nu''(b) \int (h(t)/f(t)) \, d\lambda''_b(t).
$$

But since the function $b \mapsto \int (h(t)/f(t)) \, d\lambda''_b(t)$ is $\nu''$-integrable, the function $b \mapsto g(b) \int (h(t)/f(t)) \, d\lambda''_b(t)$ is $\nu$-integrable (Ch. V, §5, No. 3, Th. 1).

By the definition of $\lambda_b$, this function is $b \mapsto \int h(t) d\lambda_b(t)$, whence (*loc. cit.*) $\int h(t) d\mu(t) = \int d\nu(b) \int h(t) d\lambda_b(t)$, which proves that $\mu = \int \lambda_b d\nu(b)$.

To establish the second part of the statement, we remark that one can suppose that $r(b) > 0$ for all $b \in B$ (Ch. V, §5, No. 6, Prop. 10); set $\lambda'''_b = f \cdot \left( (r(b)/g(b)) \lambda'_b \right)$; one shows, as above, that for every function $h \in \mathcal{K}(T)$, the relation

$$
\int h(t) d\mu(t) = \int d\nu'(b) \int h(t) d\lambda'_b(t)
$$

implies

$$
\int h(t) d\mu(t) = \int d\nu''(b) \int (h(t)/f(t)) d\lambda'''_b(t) .
$$

Therefore Th. 1 of No. 1, applied to $\mu''$ and $\nu''$, implies that for almost every $b \in B$, $\lambda'''_b = \lambda''_b$, whence $\lambda_b = r(b)\lambda'_b$.

#### Definition 2 {#int-vi-s3-def-2 .statement}

*Let T and B be two Polish locally compact spaces. Given a positive measure $\mu$ on T, a $\mu$-measurable mapping p of T into B, and a pseudo-image measure $\nu$ of $\mu$ under p, every $\nu$-adequate family $b \mapsto \lambda_b$ ($b \in B$) of positive measures on T having the properties b) and c) of Th. 2 is called a disintegration of $\mu$ relative to $\nu$.*

When $p$ is $\mu$-proper and $\nu = p(\mu)$, the concept of disintegration relative to $p$ thus coincides with the concept of disintegration relative to $\nu$. Under the hypotheses of Th. 2, two disintegrations of $\mu$ relative to the same pseudo-image measure $\nu$ are equal almost everywhere for $\nu$.

#### Remark {#int-vi-s3-n3-rem-1 .statement}

— Th. 1 of Ch. V, §3, No. 4 shows (taking into account the fact that T and B have countable bases) that for every function $f$ defined on T, with values in $\overline{\mathbf{R}}$ or in a Banach space F and $\mu$-integrable, the set of $b \in B$ such that $f$ is not $\lambda_b$-integrable is $\nu$-negligible, the function $b \mapsto \int f(t) d\lambda_b(t)$, defined almost everywhere, is $\nu$-integrable, and

$$
\int f(t) d\mu(t) = \int d\nu(b) \int f(t) d\lambda_b(t) .
$$

An analogous result holds for scalarly $\mu$-integrable functions, on applying Prop. 3 of §1, No. 1.

### 4. Measurable equivalence relations

Given a topological space X and an equivalence relation R in X, we shall say that R is *Hausdorff* if the quotient space X/R is Hausdorff.

Recall (GT, I, §8, No. 3, Prop. 8) that when R is an open equivalence relation, it comes to the same to say that the graph of R in X × X is closed.

Let p be a mapping of X into a Hausdorff topological space B, and let R be the equivalence relation $p(x) = p(y)$ in X; if K is a compact subset of X such that the restriction of p to K is continuous, then the relation $R_K$ induced by R on K is Hausdorff, because the quotient space $K / R_K$ is homeomorphic to the space $p(K)$, which is compact (GT, I, §9, No. 4, Th. 2 and its Cor. 2). If T is a locally compact space, $\mu$ is a positive measure on T, and p is a $\mu$-measurable mapping of T into a Hausdorff topological space B, one thus sees that there exists a $\mu$-dense set (Ch. IV, §5, No. 8) of compact subsets K of T for which the relation $R_K$ is Hausdorff. We are thus led to make the following definition:

#### Definition 3 {#int-vi-s3-def-3 .statement}

*Let T be a locally compact space, $\mu$ a positive measure on T. An equivalence relation R in T is said to be $\mu$-measurable if there exists a $\mu$-dense set of compact subsets K of T for which the relation $R_K$ is Hausdorff.*

If R is Hausdorff then R is $\mu$-measurable, because if $\varphi$ is the canonical mapping of T onto the Hausdorff topological space T/R, $\varphi$ is continuous and R is equivalent to $\varphi(x) = \varphi(y)$. Similarly, if R is such that the saturation for R of every compact subset of T is closed (in particular, if R is a closed equivalence relation), then R is $\mu$-measurable, because for every compact subset K of T, the relation $R_K$ is closed, hence Hausdorff (GT, I, §10, No. 4, Prop. 8).

Note that if R is $\mu$-measurable, then R is also measurable for every measure on T with base $\mu$.

#### Proposition 2 {#int-vi-s3-prop-2 .statement}

*Let T be a locally compact space countable at infinity, $\mu$ a positive measure on T.

1) For every $\mu$-measurable equivalence relation R in T, there exist a locally compact space B and a $\mu$-measurable mapping p of T into B such that R is equivalent to the relation $p(x) = p(y)$.

2) If, moreover, T admits a countable base, one can suppose that B admits a countable base.*

Since T is countable at infinity, there exists an increasing sequence $(K_n)_{n \geq 1}$ of compact subsets of T such that T is the union of the $K_n$ and a $\mu$-negligible set N, and such that each of the relations $R_{K_n}$ is Hausdorff. Let $B_n$ be the quotient space $K_n / R_{K_n}$, which is compact, and let $B'_n$ be the compact space that is the topological sum of $B_n$ and a point $a_n$. Let $q_n$ be the canonical mapping of $K_n$ onto $B_n$; we extend $q_n$ to a mapping $p_n$ of T into $B'_n$ in the following manner: if $x \in T$ is equivalent mod R to an element $y \in K_n$, set $p_n(x) = q_n(y)$; in the contrary case, set $p_n(x) = a_n$.

Let $B'$ be the product space $\prod_{n=1}^{\infty} B'_n$, which is compact, and let $p'$ be the mapping $x \mapsto (p_n(x))$ of T into B'. Let us show that $p'$ is $\mu$-measurable: it suffices (Ch. IV, §5, No. 3, Th. 1) to prove that each of the mappings $p_n$ is measurable, and for this it suffices that the restriction of $p_n$ to each $K_m$ be measurable. Now, this is obvious if $m \leq n$; if, on the contrary, $m > n$, let $K_{nm}$ be the saturation of $K_n$ for $R_{K_m}$, which is a compact subset of $K_m$ (GT, I, §9, No. 4, Th. 2); since $p_n$ is constant on $K_m - K_{nm}$, it suffices to prove that the restriction of $p_n$ to $K_{nm}$ is continuous, which is obvious on account of the canonical isomorphism between $K_{nm}/R_{K_{nm}}$ and $K_n/R_{K_n}$ (GT, I, §9, No. 4, Cor. 4 of Th. 2).

Let A be the saturation of $\bigcup_n K_n$ for the relation R, and let $N' = T - A \subset N$. We shall see that the relation $p'(x) = p'(y)$ is equivalent to the relation «$R\{x, y\}$ or $(x, y) \in N' \times N'$ ». For, if $R\{x, y\}$ then $p_n(x) = p_n(y)$ for all $n$, therefore $p'(x) = p'(y)$; and if $x \in N'$, $y \in N'$ then $p_n(x) = p_n(y) = a_n$ for all $n$, therefore $p'(x) = p'(y)$. If on the other hand $x$ and $y$ are in A and are not equivalent mod R, then there exist an integer $n$, an element $x' \in K_n$ (resp. $y' \in K_n$) equivalent mod R to $x$ (resp. $y$) such that $x'$ is not equivalent to $y'$ mod $R_{K_n}$; therefore $p_n(x) \neq p_n(y)$, consequently $p'(x) \neq p'(y)$. Finally, if $x \in N'$ and $y \in A$, then $p_n(y) \in B_n$ for $n$ sufficiently large and $p_n(x) = a_n$ for all $n$, therefore $p'(x) \neq p'(y)$, which establishes our assertion.

Consider then the quotient set $B_0 = N'/R_{N'}$; let $q_0$ be the canonical mapping of $N'$ onto $B_0$, $s_0$ a section of $q_0$. Set $p_0(x) = s_0(q_0(x))$ for $x \in N'$ and extend $p_0$ to T by taking $p_0$ to be constant on A equal to an element of T. Then $p = (p', p_0)$ is a $\mu$-measurable mapping of T into the locally compact space $B = B' \times T$; it is immediate that if $x \in N'$, $y \in N'$, the relation $p_0(x) = p_0(y)$ implies $R\{x, y\}$; thus $p$ meets the requirements. Moreover, if T admits a countable base, then so do each of the quotient spaces $B_n$ (GT, IX, §2, No. 10, Prop. 17), therefore B' admits a countable base, hence so does B.

#### Proposition 3 {#int-vi-s3-prop-3 .statement}

— *Let T be a Polish locally compact space, $\mu$ a positive measure on T, and R an equivalence relation in T. The following properties are equivalent:*

a) $R$ is $\mu$-measurable.

b) *There exists a sequence of mappings $p_n : T \to F_n$ into Hausdorff topological spaces, such that each $p_n$ is $\mu$-measurable and such that the relation $R\{x, y\}$ is equivalent to «for all $n$, $p_n(x) = p_n(y)$».*

c) *There exists a sequence $(A_n)$ of $\mu$-measurable sets, saturated for R, such that for every $x \in T$ the class of x with respect to R is the intersection of those $A_n$ that contain x.*

With notations as in the statement of b), set $p(x) = (p_n(x))$; the property b) means that the mapping $p$ of T into the product space $\prod F_n$ is measurable (Ch. IV, §5, No. 3, Th. 1) and that the relation $R\{x, y\}$ is equivalent to $p(x) = p(y)$; thus b) implies a).

Next let us show that c) implies b). Suppose c) verified; then the characteristic functions $\varphi_{A_n}$ are $\mu$-measurable, and the hypothesis c) means that the relation $R\{x, y\}$ is equivalent to «for every $n$, $\varphi_{A_n}(x) = \varphi_{A_n}(y)$».

Finally, let us show that a) implies c). By Prop. 2, there exist a locally compact space B with a countable base, and a $\mu$-measurable mapping $p$ of T into B, such that the relation $R\{x, y\}$ is equivalent to $p(x) = p(y)$. Let $(U_n)$ be a countable base for the topology of B. The sets $A_n = \overline{p^{-1}(U_n)}$ are $\mu$-measurable (Ch. IV, §5, No. 5, Prop. 7) and saturated for R; and if $x, y$ are points of T such that $p(x) \neq p(y)$, there exists an index $n$ such that $p(x) \in U_n$ and $p(y) \notin U_n$, which means that $x \in A_n$ and $y \notin A_n$.

#### Remark {#int-vi-s3-n4-rem-1 .statement}

If R is a $\mu$-measurable equivalence relation in T, the saturation for R of a compact subset of T is not necessarily $\mu$-measurable (Exer. 5).

#### Theorem 3 {#int-vi-s3-thm-3 .statement}

— *Let T be a locally compact space with a countable base, $\mu$ a positive measure on T, and R a $\mu$-measurable equivalence relation in T. Then, there exists a $\mu$-measurable subset S of T that intersects each class with respect to R at one and only one point (a 'measurable section' for R).*

We may clearly suppose that the measure $\mu$ is bounded and that $\mu(T) \leq 1$ (Ch. V, §5, No. 6, Prop. 11). We are going to define a sequence $(S_n)$ of *Borel* subsets (GT, IX, §6, No. 3) such that each equivalence class with respect to R intersects the union $S'$ of the $S_n$ in at most one point, that for every $n$ the saturation $T_n$ of the union of the $S_p$ with index $p \leq n$ is $\mu$-measurable, and that $\mu(T - T_n) \leq 1/2^n$. The saturation $T'$ of $S'$ will therefore be $\mu$-measurable and $N = T - T'$ will have measure zero. If $S''$ is any section of N for the relation $R_N$, $S = S' \cup S''$ will meet the requirements, since $S'$, being a Borel set, is $\mu$-measurable (Ch. IV, §5, No. 4, Cor. 3 of Th. 2), and $S''$ has measure zero.

By Prop. 2, $R\{x, y\}$ is equivalent to the relation $p(x) = p(y)$, where $p$ is a $\mu$-measurable mapping of T into a locally compact space F. Suppose the $S_k$ defined for $k \leq n$. Since $T - T_n$ is $\mu$-measurable and of measure $\leq 1/2^n$, there exists a compact subset K of $T - T_n$ such that $\mu(T - (T_n \cup K)) \leq 1/2^{n+1}$ and such that the restriction of $p$ to K is continuous. Since the induced relation $R_K$ is closed and K is metrizable, we know that there exists a Borel subset $S_{n+1}$ of K such that, in K, each point is equivalent (mod R) to one and only one point of $S_{n+1}$ (GT, IX, §6, No. 8, Th.4). Therefore $p(S_{n+1}) = p(K)$, which is a compact set in F; the saturation of $S_{n+1}$ for R is the inverse image $\overline{p^{-1}(p(K))}$, which is therefore μ-measurable (Ch. IV, §5, No. 5, Prop. 7); it is clear that this set contains K, therefore the union T_{n+1} of T_n and $\overline{p}^{-1}(p(K))$ is μ-measurable, saturated for R, and is such that $\mu(T - T_{n+1}) \leq 1/2^{n+1}$, which completes the proof.

### 5. Disintegration of a measure by a measurable equivalence relation

Let T be a Polish locally compact space, $\mu$ a positive measure on T, and R a $\mu$-measurable equivalence relation in T. Then, there exist (No. 4, Prop. 2) a Polish locally compact space B and a $\mu$-measurable mapping p of T into B, such that the relation $p(x) = p(y)$ is equivalent to R$\{x, y\}$. Every measure $\nu$ that is a pseudo-image of $\mu$ under p (No. 2) will be called a *quotient measure of $\mu$ by the relation* R; if $b \mapsto \lambda_b$ is a disintegration of $\mu$ relative to the measure $\nu$, we shall say that $b \mapsto \lambda_b$ is a *disintegration of $\mu$ by the relation* R. By virtue of the properties of p and the $\lambda_b$, each of the measures $\lambda_b$ is concentrated on an equivalence class with respect to R, and if $b \neq c$, the measures $\lambda_b$ and $\lambda_c$ are concentrated on distinct classes.

The space B, the mapping p and the pseudo-image measure $\nu$ on B can in general be chosen in infinitely many ways. Nevertheless, the various disintegrations of $\mu$ by R can all be deduced from one among them, as a consequence of the following theorem:

#### Theorem 4 {#int-vi-s3-thm-4 .statement}

*Let T be a Polish locally compact space, $\mu$ a positive measure on T, and R a $\mu$-measurable equivalence relation in T. Let B, B' be two Polish locally compact spaces, p, p' two $\mu$-measurable mappings of T into B, B' respectively, such that R$\{x, y\}$ is equivalent to $p(x) = p(y)$ and to $p'(x) = p'(y)$. Let $\nu, \nu'$ be pseudo-image measures of $\mu$ under p, p' respectively; let $b \mapsto \lambda_b, b' \mapsto \lambda_{b'}$ be disintegrations of $\mu$ relative to $\nu, \nu'$ respectively.*

*Under these conditions, there exist in B (resp. B') a set N (resp. N') negligible for $\nu$ (resp. $\nu'$) and a bijection f of B - N onto B' - N', having the following properties:*

a) *The mapping f (defined almost everywhere in B) is $\nu$-measurable and its inverse mapping $f'$ is $\nu'$-measurable; every pseudo-image measure of $\nu$ (resp. $\nu'$) under f (resp. $f'$) is equivalent to $\nu'$ (resp. $\nu$).*

b) *For every $b \in B - N$, the measure $\lambda'_{f(b)}$ on T is of the form $r(b)\lambda_b$, where $r(b) \neq 0$ and r is locally $\nu$-integrable.*

To establish a), we may limit ourselves to the case that $\nu$ and $\nu'$ are *bounded* measures (Ch. V, §5, No. 6, Prop. 11). Let $N_0 = B - p(T)$, $N'_0 = B' - p'(T)$; we know that $N_0$ (resp. $N'_0$) is negligible for $\nu$ (resp. $\nu'$) (No. 2). There exists a bijection f of B - $N_0$ onto B' - $N'_0$ defined by $f(p(t)) = p'(t)$ for all $t \in T$; let $f'$ be the inverse mapping of $f$, so that $f'(p'(t)) = p(t)$. For every subset M of B, the relation « M is $\nu$-measurable » is equivalent to « $\overline{p}^{-1}(M)$ is $\mu$-measurable », that is, to « $p'(f(M))$ is $\mu$-measurable », thus finally to « $f(M)$ is $\nu'$-measurable » (Ch. V, §6, No. 2, Cor. of Prop. 3). We thus see that $f$ (resp. $f'$) transforms every $\nu$-measurable (resp. $\nu'$-measurable) set into a $\nu'$-measurable (resp. $\nu$-measurable) set; since B and $B'$ are metrizable and have countable bases, it follows that $f$ and $f'$ are measurable (Ch. IV, §5, No. 5, Th. 4). Moreover, if $M \subset B$ is $\nu$-negligible then $\overline{p}^{-1}(M) = p'(f(M))$ is $\mu$-negligible, therefore $f(M)$ is $\nu'$-negligible (Ch. V, §6, No. 2, Cor. 2 of Prop. 2); similarly, $f'$ transforms every $\nu'$-negligible set into a $\nu$-negligible set. Consequently, the image of $\nu$ under $f$ (which is defined since $\nu$ is bounded, which implies that $f$ is $\nu$-proper) is equivalent to $\nu'$, and the image of $\nu'$ under $f'$ is equivalent to $\nu$ (Ch. V, §5, No. 6, Prop. 10). It remains to prove b). By virtue of Th. 2 of No. 3, we can restrict ourselves to the case that $\nu' = f(\nu)$. Since $\mu = \int \lambda_{b'}' d\nu'(b')$, we have, for every function $h \in \mathcal{K}(T)$,

$$
\int h(t) d\mu(t) = \int d\nu'(b') \int h(t) d\lambda_{b'}'(t) = \int d\nu(b) \int h(t) d\lambda_{f(b)}'(t)
$$

(Ch. V, §3, No. 4, Th. 1 and §6, No. 2, Th. 1); in other words, $\mu = \int \lambda_{f(b)}' d\nu(b)$. But since also $\mu = \int \lambda_b d\nu(b)$ and since, for every $b \in B - N_0$, $\lambda_b$ and $\lambda_{f(b)}'$ are carried by $\overline{p}^{-1}(b)$, Th. 2 of No. 3 implies that $\lambda_b = \lambda_{f(b)}'$ for almost every $b \in B - N_0$, hence for almost every $b \in B$. The conditions of Th. 4 are therefore verified by taking for N the union of $N_0$ and the set of $b \in B$ such that $\lambda_b \neq \lambda_{f(b)}'$.

### Exercises {#int-vi-s3-exercises}

See the [exercises for § 3](exercises/s3/).
