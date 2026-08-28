---
book: int
book_title: Integration
chapter: VI
chapter_title: VECTORIAL INTEGRATION
section: 2
section_title: Vectorial measures . "
lang: en
source: int-i-vi
book_pages: INT VI.18-INT VI.40, INT VI.62-INT VI.69
pdf_pages: 0409-0431, 0453-0460
extraction: ocr
subsections:
    - "no": 1
      title: Definition of a vectorial measure
      page: 18
      pdf_page: 409
    - "no": 2
      title: Integration with respect to a vectorial measure
      page: 20
      pdf_page: 411
    - "no": 3
      title: Majorizable vectorial measures
      page: 22
      pdf_page: 413
    - "no": 4
      title: Vectorial measures with base $\mu$
      page: 25
      pdf_page: 416
    - "no": 5
      title: The Dunford–Pettis theorem
      page: 27
      pdf_page: 418
    - "no": 6
      title: Dual of the space $L^1_F$ (F a separable Banach space)
      page: 32
      pdf_page: 423
    - "no": 7
      title: Integration of a vector-valued function with respect to a vectorial measure
      page: 33
      pdf_page: 424
    - "no": 8
      title: Complex measures
      page: 34
      pdf_page: 425
    - "no": 9
      title: Bounded complex measures⁶
      page: 37
      pdf_page: 428
    - "no": 10
      title: Image of a complex measure; induced complex measure; product of complex measures\footnote{Cf. Ch. V, §6, No. 4; Ch. IV, §5, No. 7 and Ch. V, §7; Ch. III, §4 and Ch. V, §8, Nos. 2–5.}
      page: 39
      pdf_page: 430
statements: 42
exercises: 18
content_sha256: a8aa27b4be882b310434bde98ac4fb834ca90937904a9e3a872c008cc7e64bb3
---

## § 2. VECTORIAL MEASURES

### 1. Definition of a vectorial measure

The definition of a measure given in Ch. III, §1, No. 3 may be generalized as follows:

#### Definition 1 {#int-vi-s2-def-1 .statement}

*Let F be a Hausdorff locally convex space over R. One calls vectorial measure on T with values in F every continuous linear mapping of the space $\mathcal{K}(T)$ into F.*

Def. 1 may also be expressed as follows: a vectorial measure on T with values in F is a linear mapping m of $\mathcal{K}(T)$ into F such that, for every compact subset K of T, the restriction of m to $\mathcal{K}(T, K)$ is continuous for the topology of uniform convergence. If $f \in \mathcal{K}(T)$, one also writes $\int f dm$ or $\int f(t)\,dm(t)$ instead of $m(f)$. The measures with values in $\mathbf{R}$ are sometimes called *real* measures (Ch. III, §1, No. 5) or *scalar* measures on T.

#### Example {#int-vi-s2-n1-exa-1 .statement}

— 1) The identity mapping of $\mathcal{K}(T)$ is a vectorial measure on T with values in $\mathcal{K}(T)$.

2) *Let H be a complex Hilbert space, $\mathcal{L}(H)$ the normed algebra of continuous endomorphisms of H. Let A be a subalgebra of $\mathcal{L}(H)$, commutative, closed, self-adjoint and containing the identity; one shows that there exist a compact space X and an isomorphism of the normed algebra A onto the algebra $\mathcal{K}_\mathbf{C}(X) = \mathcal{C}_\mathbf{C}(X)$ of continuous complex functions on X, equipped with the norm $\|f\| = \sup_{x \in X} |f(x)|$. The inverse isomorphism, restricted to $\mathcal{K}(X)$, is a vectorial measure m on X, with values in $\mathcal{L}(H)$, such that $m(fg) = m(f)m(g)$.*_

#### Remark {#int-vi-s2-n1-rem-1 .statement}

— 1) For a linear mapping m of $\mathcal{K}(T)$ into F to be a vectorial measure, it is necessary and sufficient that, for every compact subset K of T, the image under m of the unit ball $\|f\| \leq 1$ of $\mathcal{K}(T, K)$ be *bounded* in F. The notion of vectorial measure with values in F is therefore the same for all the Hausdorff locally convex topologies on F that admit the same bounded sets, and in particular for all the topologies compatible with the duality between F and F' (TVS, IV, §1, No. 1, Prop. 1).

2) Let $T_1$ be a locally compact space, $F_1$ a Hausdorff locally convex space over $\mathbf{R}$, u a continuous linear mapping of $\mathcal{K}(T_1)$ into $\mathcal{K}(T)$, and v a continuous linear mapping of F into $F_1$. If m is a vectorial measure on T with values in F, then $v \circ m \circ u$ is a vectorial measure on $T_1$ with values in $F_1$. In particular, if g is a continuous, finite numerical function on T, then $f \mapsto m(gf)$ is a vectorial measure on T with values in F, which is denoted $g \cdot m$; if h is a second continuous, finite numerical function on T, then $g \cdot (h \cdot m) = (gh) \cdot m$.

3) Since the space $\mathcal{K}(T)$ is the direct limit of the Banach spaces $\mathcal{K}(T, K)$, and is in particular barreled (TVS, III, §4, No. 1, Cor. of Prop. 2 and Cor. 3 of Prop. 3), in order that a linear mapping m of $\mathcal{K}(T)$ into F be a vectorial measure, it is necessary and sufficient that, for every $z' \in F'$, $z' \circ m$ be a scalar measure on T (TVS, II, §6, No. 4, Prop. 5 and IV, §1, No. 3, Prop. 7).

4) In view of Remark 1, Prop. 1 of Ch. III, §2, No. 1 and its proof are again valid for vectorial measures. One can therefore define the *support* of a vectorial measure m on T to be the complement of the largest open set $U \subset T$ such that the restriction of m to U is zero.

### 2. Integration with respect to a vectorial measure

Let $m$ be a vectorial measure on $T$, with values in $F$. For every $z' \in F'$, the mapping $z' \circ m$ is a scalar measure on $T$, depending linearly on $z'$. If $f$ is a numerical function defined on $T$, we shall say, by an abuse of language, that the pair $(f, m)$ has the property $P$ if, for every $z' \in F'$, the pair $(f, |z' \circ m|)$ has the property $P$. For example, we shall say that $f$ is *essentially integrable for* $m$ if, for every $z' \in F'$, the function $f$ is essentially integrable for $|z' \circ m|$. It comes to the same to say that $f$ is essentially integrable for each of the measures $(z' \circ m)^+$ and $(z' \circ m)^-$ (Ch. V, §2, No. 2, Cor. 2 of Prop. 3).

#### Proposition 1 {#int-vi-s2-prop-1 .statement}

*Let $m$ be a vectorial measure on $T$ with values in $F$, $f$ a numerical function on $T$ that is essentially integrable for $m$. The mapping*
$$
z' \mapsto \int f \, d(z' \circ m)^+ - \int f \, d(z' \circ m)^-
$$
*is a linear form on $F'$*.

Denoting this mapping by $\Phi$, it is immediate that $\Phi(\lambda z') = \lambda \Phi(z')$ for all $\lambda \in \mathbf{R}$. Everything comes down to showing that $\Phi(y' + z') = \Phi(y') + \Phi(z')$. Set $\mu = |y' \circ m| + |z' \circ m|$; by the Lebesgue–Nikodym theorem, one can then write $y' \circ m = g \cdot \mu$ and $z' \circ m = h \cdot \mu$, where $g$ and $h$ are two bounded and locally $\mu$-integrable numerical functions (Ch. V, §5, No. 5, Th. 2); moreover, $(y' \circ m)^+ = g^+ \cdot \mu$ and $(y' \circ m)^- = g^- \cdot \mu$, and the analogous relations hold with $y'$ replaced by $z'$ (resp. $y' + z'$) and $g$ by $h$ (resp. $g + h$). This being so, it is immediate that $f$ is essentially $\mu$-integrable (Ch. V, §2, No. 2, Cor. 1 of Prop. 3), and the relation to be proved reduces to $(g + h)^+ - (g + h)^- = (g^+ - g^-) + (h^+ - h^-)$, which is obvious.

#### Definition 2 {#int-vi-s2-def-2 .statement}

*Let $m$ be a vectorial measure on $T$ with values in $F$, $f$ a numerical function on $T$ that is essentially integrable for $m$. One calls integral of $f$ with respect to $m$, and denotes by $m(f)$ or $\int f \, dm$ or again $\int f(t) \, dm(t)$, the element of ${F'}^*$ defined by*

$$
\langle z', \int f \, dm \rangle = \int f \, d(z' \circ m)^+ - \int f \, d(z' \circ m)^-.
$$

We observe that if $f \in \mathcal{K}(T)$, the element $\int f \, dm$ so defined coincides with the element denoted likewise in No. 1, because the second member of (1) is then $\int f \, d(z' \circ m) = z'(m(f))$ by definition. Moreover, if in particular one applies Def. 2 to the case that $F = \mathbf{R}$, one sees that for every $z' \in F'$, f is essentially integrable for the real measure $z' \circ m$, and that the second member of (1) may be written $\int f d(z' \circ m)$.

Suppose now that $f$ is essentially integrable for $m$, and let $z' \in F'$. Set $\mu = |z' \circ m|$; by the Lebesgue–Nikodym theorem, one can write $z' \circ m = g \cdot \mu$, where $g$ is locally $\mu$-integrable and $\|g\| \leq 1$, and the proof of Prop. 1 shows that $\int f d(z' \circ m) = \int fg d\mu$. Consequently,

$$
\left| \int f d(z' \circ m) \right| \leq \int |f| d|z' \circ m|.
$$

It is clear that the set of finite numerical functions essentially integrable for $m$ is a vector space over $\mathbf{R}$; we shall denote by $\mathcal{L}(m)$ this space equipped with the coarsest locally convex topology making continuous all of the linear forms $f \mapsto \int f d(z' \circ m)$, where $z'$ runs over $F'$. Note that in general the locally convex space $\mathcal{L}(m)$ is *not Hausdorff*.

#### Example {#int-vi-s2-n2-exa-1 .statement}

— Let us take for $m$ the identity mapping of $\mathscr{K}(T)$ onto itself. Since the dual of $\mathscr{K}(T)$ is the space $\mathscr{M}(T)$ of scalar measures on $T$, the functions $f \in \mathcal{L}(m)$ are those that are essentially integrable for *every* scalar measure $\mu$ (cf. Exer. 1), and the integral $\int f dm$ is the linear form $\mu \mapsto \int f d\mu$ on $\mathscr{M}(T)$. One cannot have $\int f d\mu = 0$ for every measure $\mu \in \mathscr{M}(T)$ unless $f = 0$, as one sees on taking $\mu = \varepsilon_t$, where $t$ is arbitrary in $T$; in other words, the mapping $f \mapsto \int f dm$ is an *injection* of $\mathcal{L}(m)$ into the algebraic dual of $\mathscr{M}(T)$, which extends the identity mapping of $\mathscr{K}(T)$. The relation $\int f dm \in F = \mathscr{K}(T)$ is therefore equivalent to $f \in \mathscr{K}(T)$.

Let $u$ be a continuous linear mapping of $F$ into a Hausdorff locally convex space $G$, and let us denote again by $u$ its extension by bitransposition to a linear mapping of ${F'}^*$ into ${G'}^*$ (§ 1, No. 1). With this convention:

#### Proposition 2 {#int-vi-s2-prop-2 .statement}

*Every numerical function* $f$ *essentially integrable for* $m$ *is essentially integrable for* $u \circ m$, *and* $\int f d(u \circ m) = u(\int f dm)$.

The proposition is obvious, in view of the equality $y' \circ u \circ m = {}^t u(y') \circ m$ for all $y \in G'$.

In general, if $f \in \mathcal{L}(m)$, the integral $\int f dm$ belongs to ${F'}^*$ but not to $F$ (see the above *Example*). However:

#### Proposition 3 {#int-vi-s2-prop-3 .statement}

*If the image under* $m$ *of the set of* $f \in \mathscr{K}(T)$ *such that* $\sup_{t \in T} |f(t)| \leq 1$ *is weakly relatively compact in* $F$, *then* $\int f dm \in F$ *for every bounded numerical function* $f$ *essentially integrable for* $m$.

Let $A$ be the set of $f \in \mathcal{L}(m)$ such that $\sup_{t \in T} |f(t)| \leq 1$, and let $B = A \cap \mathscr{K}(T)$; by hypothesis, $m(B)$ is weakly relatively compact in $F$, therefore it suffices to show that $m(A)$ is contained in the closure (in ${F'}^*$) of $m(B)$ for the topology $\sigma({F'}^*, F')$; since $m(B)$ is convex and balanced, it suffices to prove that the polar of $m(B)$ in $F'$ is contained in that of $m(A)$ (TVS, II, §6, No. 3, Th. 1). Now, for a linear form $z' \in F'$ to belong to $(m(B))^\circ$, it is necessary and sufficient that $|\langle z', m(g)\rangle| = |\int g d(z'\circ m)| \leq 1$ for every function $g \in B$, which signifies that the scalar measure $|z'\circ m|$ is bounded and of norm $\leq 1$ (Ch. III, §1, No. 8); but by (2) the latter condition implies that $|\langle z', m(f)\rangle| \leq 1$ for every function $f \in A$, whence $z' \in (m(A))^\circ$.

#### Corollary 1 {#int-vi-s2-prop-3-cor-1 .statement}

*If, for every compact subset K of T, the image under m of the set of $f \in \mathcal{H}(T, K)$ such that $\sup_{t \in T} |f(t)| \leq 1$ is weakly relatively compact in F, then $\int f dm \in F$ for every function $f \in \mathcal{L}(m)$ that is bounded and has compact support, and $\int f dm \in F''$ for every function $f \in \mathcal{L}(m)$.*

The first assertion may be deduced immediately from Prop. 3: if $f$ is bounded and has compact support, and if U is a relatively compact open neighborhood of the support of $f$, then the restriction of $m$ to the subspace $\mathcal{H}(U)$ is a measure $m_U$ on U that satisfies the conditions of Prop. 3, and $\int f dm_U = \int f dm$ (Ch. V, §7, No. 1, Th. 1), therefore $\int f dm \in F$.

Now let $f$ be any element of $\mathcal{L}(m)$; for every compact subset K of T and every integer $n > 0$, let $f_{n,K}$ be the numerical function on T defined as follows: if $t \notin K$, $f_{n,K}(t) = 0$; if $t \in K$ and $|f(t)| \leq n$, $f_{n,K}(t) = f(t)$; finally, if $t \in K$ and $|f(t)| > n$, $f_{n,K}(t) = nf(t)/|f(t)|$. It is clear that for every $t \in T$, $f(t)$ is the limit of $f_{n,K}(t)$ with respect to the product filter of the Fréchet filter by the section filter of the (increasing directed) ordered set of compact subsets of T. Since $|f_{n,K}| \leq |f|$, it follows from Lebesgue’s theorem and Prop. 10 of Ch. V, §1, No. 3, applied to each scalar measure $|z'\circ m|$, that $f_{n,K}$ converges to $f$ in $\mathcal{L}(m)$ with respect to the preceding filter. Consequently, the integral $\int f dm$ is in the closure in ${F'}^*$ (for the topology $\sigma({F'}^*, F')$) of the set M of $m(f_{n,K})$. But the first part of the corollary shows that $M \subset F$, and, on the other hand, for every $z' \in F'$ one has $|\langle z', m(f_{n,K})\rangle| \leq \int |f| d|z'\circ m|$, which shows that M is bounded in $F_\sigma$, hence also in F (TVS, IV, §1, No. 1, Prop. 1). Lemma 1 of §1, No. 2 therefore shows that $\int f dm \in F''$.

#### Corollary 2 {#int-vi-s2-prop-3-cor-2 .statement}

*If F is semi-reflexive, then $\int f dm \in F$ for every numerical function $f$ essentially integrable for $m$.*

### 3. Majorizable vectorial measures

Let $q$ be a lower semi-continuous semi-norm on F. We shall denote by $A'_q$ the set of $z' \in F'$ such that $|\langle z', x\rangle| \leq q(x)$ for all $x \in F$. This is

the polar in $F'$ of the set of $x \in F$ such that $q(x) \leq 1$; for every $x \in F$,
$$
q(x) = \sup_{z' \in A'_q} |\langle x, z' \rangle|.
$$

#### Definition 3 {#int-vi-s2-def-3 .statement}

*Let $m$ be a vectorial measure on $T$ with values in $F$. If $q$ is a lower semi-continuous semi-norm on $F$, $m$ is said to be *q-majorizable* if there exists a positive measure $\mu$ such that $|z' \circ m| \leq \mu$ for every $z' \in A'_q$; the supremum of the measures $|z' \circ m|$ as $z'$ runs over $A'_q$ (Ch. III, §2, No. 4, Th. 3) is then denoted $q(m)$. One says that $m$ is *majorizable* if it is *q-majorizable* for every continuous semi-norm $q$ on $F$.

If $m$ and $m'$ are both *q-majorizable*, it is immediate that $m + m'$ is also *q-majorizable* and that
$$
q(m + m') \leq q(m) + q(m').
$$

When $F$ is a normed space, with norm denoted $|x|$, to say that $m$ is majorizable therefore means that the measures $|z' \circ m|$, where $|z'| \leq 1$, are bounded above$^1$ by a same positive measure; one then denotes by $|m|$ the supremum of this family of measures.

If $F = \mathbf{R}$, the measure $|m|$ corresponding to the Euclidean norm $|x|$ on $\mathbf{R}$ coincides with the measure denoted by $|m|$ in Ch. III, §1, No. 5.

#### Proposition 4 {#int-vi-s2-prop-4 .statement}

*Let* $(F_i)_{1 \leq i \leq n}$ *be a finite family of Hausdorff locally convex spaces, $F = \prod_{i=1}^n F_i$ their product, $q_i$ ($1 \leq i \leq n$) *a lower semi-continuous semi-norm* on $F_i$, *and* $q$ *the semi-norm on* $F$ *defined by* $q(x_1, \ldots, x_n) = \sum_{i=1}^n q_i(x_i)$. *If* $m_i$ ($1 \leq i \leq n$) *is a vectorial measure on* $T$ *with values in* $F_i$ *that is* $q_i$*-majorizable*, *then the measure* $m = (m_1, \ldots, m_n)$ *with values in* $F$ *is* *q-majorizable*.

For, the dual $F'$ may be identified with $\prod_{i=1}^n F_i'$, in such a way that if $x = (x_i) \in F$, $z' = (z_i') \in F'$, then $\langle x, z' \rangle = \sum_{i=1}^n \langle x_i, z_i' \rangle$. If $|\langle x, z' \rangle| \leq q(x)$ for every $x \in F$, then in particular $|\langle x_i, z_i' \rangle| \leq q_i(x_i)$ for $1 \leq i \leq n$, and the converse is obvious, which shows that the set $A'_q$ is the product of the $A'_{q_i}$. Since by hypothesis $|z_i' \circ m_i| \leq q_i(m_i)$ for $z_i' \in A'_{q_i}$, it follows that
$$
|z' \circ m| \leq \sum_{i=1}^n |z_i' \circ m_i| \leq \sum_{i=1}^n q_i(m_i)
$$
for every $z' \in A'_q$, which proves the proposition.

$^1$ Majorées.

#### Corollary {#int-vi-s2-n3-cor-1 .statement}

— *If the space F is finite-dimensional, then every vectorial measure m with values in F is majorizable. In order that a numerical function be essentially integrable for m, it is necessary and sufficient that it be essentially integrable for |m|* (where |x| denotes any norm on F).

#### Proposition 5 {#int-vi-s2-prop-5 .statement}

— *Let q be a lower semi-continuous semi-norm on F. Let m be a q-majorizable measure, and let f be a function essentially integrable for m and such that $\int f dm \in F$. Then*

$$
q\left( \int f dm \right) \leq \int^\bullet |f| dq(m).
$$

For,

$$
q\left( \int f dm \right) = \sup_{z' \in A'_q} \left| \langle z', \int f dm \rangle \right| \leq \sup_{z' \in A'_q} \int |f| d|z' \circ m| \leq \int^\bullet |f| dq(m)
$$

by virtue of (1) and the relation $|z' \circ m| \leq q(m)$ for $z' \in A'_q$.

#### Proposition 6 {#int-vi-s2-prop-6 .statement}

— *Let F be a quasi-complete, Hausdorff locally convex space, m a majorizable measure on T with values in F. If f is a numerical function essentially integrable for all of the measures q(m) (where q runs over the set of continuous semi-norms on F), then f is essentially integrable for m, and $\int f dm \in F$.

We shall make use of the following auxiliary result. Let $(\mu_\iota)_{\iota \in I}$ be an increasing directed family of positive measures on T. Let us denote by $\mathcal{L}^1((\mu_\iota)_{\iota \in I})$ the vector space of finite numerical functions on T, essentially $\mu_\iota$-integrable for every $\iota \in I$, equipped with the topology defined by the semi-norms $f \mapsto \mu_\iota(|f|)$ ($\iota \in I$). Let $\mathcal{L}_0$ be the linear subspace of $\mathcal{L}^1((\mu_\iota)_{\iota \in I})$ generated by the products $g \varphi_K$, where g runs over the set of continuous finite numerical functions on T, and K over the set of compact subsets of T.

#### Lemma 1 {#int-vi-s2-lem-1 .statement}

— *When $\mathcal{L}_0$ and $\mathcal{K}(T)$ are equipped with the topology induced by that of $\mathcal{L}^1((\mu_\iota)_{\iota \in I})$:
a) each element of $\mathcal{L}_0$ is in the closure of some bounded subset of $\mathcal{K}(T)$;
b) each element of $\mathcal{L}^1((\mu_\iota)_{\iota \in I})$ is in the closure of some bounded subset of $\mathcal{L}_0$.*

To prove a), we may restrict ourselves to the case of an element of the form $f = g \varphi_K$ ($g \in \mathcal{C}(T)$), K compact in T). It is immediate (by virtue of Urysohn’s theorem) that $f$ is in the closure of the set B of functions of the form $gh$, where h describes the set of continuous mappings of T into $[0,1]$ that are equal to 1 on K and to 0 on the complement of a fixed compact neighborhood H of K. Moreover, the set B is bounded, because $\mu_\iota(|gh|) \leq \mu_\iota(|f\varphi_H|)$ for every function h having the preceding properties.

Let us now prove b); we may restrict ourselves to the case of an element $f \geq 0$ of $\mathcal{L}^1((\mu_\iota)_\iota \in I)$. For every $\iota \in I$ and every $\varepsilon > 0$, there exists a compact subset $K(\iota, \varepsilon)$ of T such that the restriction of $f$ to $K(\iota, \varepsilon)$ is continuous and $|\mu_\iota(|f - f\varphi_{K(\iota, \varepsilon)}|)| \leq \varepsilon$. It is clear that $f$ is in the closure of the set C of $f\varphi_{K(\iota, \varepsilon)}$ (where $\iota \in I,\ \varepsilon > 0$). By virtue of Urysohn’s theorem, the set C in contained in $\mathcal{L}_0$; moreover, it is bounded, because $\mu_\kappa(f\varphi_{K(\iota, \varepsilon)}) \leq \mu_\kappa(f)$ for all $\iota \in I,\ \kappa \in I$ and $\varepsilon > 0$.

Let us now prove Prop. 6: for every function $g \in \mathscr{K}(T)$ and every continuous seminorm q on F, $q\left( \int g\,dm \right) \leq \int |g|\,d(q(m))$ (Prop. 5), which implies that the mapping $g \mapsto \int g\,dm$ of $\mathscr{K}(T)$ into F is continuous when $\mathscr{K}(T)$ is equipped with the topology induced by that of $\mathcal{L}^1((q(m))_{q \in Q})$ (Q the set of continuous semi-norms on F). Consequently, by the preceding lemma and Prop. 10 of TVS, III, §1, No. 6, this mapping may be extended by continuity, first to a continuous linear mapping $v_0$ of $\mathcal{L}_0$ into F, then to a continuous linear mapping $v$ of $\mathcal{L}^1((q(m))_{q \in Q})$ into F. Moreover, for every $z' \in F'$ the relation $\langle z', v(f) \rangle = \int f\,d(z' \circ m)$ holds, by the definition of $v$, for every $f \in \mathscr{K}(T)$; since $|z' \circ m| \leq q(m)$ for $q(z) = |\langle z', z \rangle|$, the mapping $f \mapsto \int f\,d(z' \circ m)$ is continuous on $\mathcal{L}^1((q(m))_{q \in Q})$, therefore again by continuity, the relation $\langle z', v(f) = \int f\,d(z' \circ m)$ holds for every function $f \in \mathcal{L}^1((q(m))_{q \in Q})$. It follows that $v(f) = \int f\,dm$, which completes the proof.

### 4. Vectorial measures with base $\mu$

#### Definition 4 {#int-vi-s2-def-4 .statement}

*Let $\mu$ be a positive measure on T. A vectorial measure $m$ on T, with values in F, is said to be a measure with base $\mu$ if there exists a mapping $f$ of T into F, scalarly locally $\mu$-integrable, such that $m(g) = \int gf\,d\mu$ for every function $g \in \mathscr{K}(T)$. One then says that $f$ is a density of $m$ with respect to $\mu$, and one writes $m = f \cdot \mu$.*

It is immediate that if $f_1$ and $f_2$ are two densities of $m$ with respect to $\mu$, then $f_1 - f_2$ is scalarly locally $\mu$-negligible (Ch. V, §5, No. 3, Cor. 2 of Prop. 3); recall that in general this does not imply that $f_1 - f_2$ is zero locally almost everywhere (cf. §1, Exer. 12 and No. 1, *Remark 2*).

Let $m$ be a measure with base $\mu$, of density $f$. For a numerical function $g$ to be essentially integrable for $m$, it is necessary and sufficient that $gf$ be scalarly essentially $\mu$-integrable (Ch. V, §5, No. 3, Th. 1).

#### Proposition 7 {#int-vi-s2-prop-7 .statement}

— Let $f$ be a mapping scalarly locally integrable with respect to a positive measure $\mu$ on $T$, such that, for every function $g \in \mathcal{K}(T)$, one has $\int gf\,d\mu \in F$. Then the mapping $g \mapsto \int gf\,d\mu$ of $\mathcal{K}(T)$ into $F$ is a vectorial measure on $T$, with base $\mu$ and density $f$ with respect to $\mu$.

For (No. 1, Remark 3), it suffices to show that, setting $m(g) = \int gf\,d\mu$, $z' \circ m$ is a scalar measure for every $z' \in F'$. But since $z'(m(g)) = \int g\langle z', f \rangle\,d\mu$, one has $z' \circ m = \langle z', f \rangle \cdot \mu$, whence our assertion.

#### Proposition 8 {#int-vi-s2-prop-8 .statement}

— Let $\mu$ be a positive measure on $T$, $m$ a measure on $T$ with values in $F$, with base $\mu$ and density $f$ with respect to $\mu$. Let $q$ be a lower semi-continuous semi-norm on $F$.

a) If, for every compact subset $K$ of $T$, the upper integral $\int_K^*(q \circ f)\,d\mu$ is finite, then $m$ is $q$-majorizable.

b) If $m$ is $q$-majorizable, then $q(m)$ has base $\mu$; if in addition $f$ is $\mu$-measurable as a mapping of $T$ into $F_\sigma$, then $q \circ f$ is locally $\mu$-integrable and $q(m) = (q \circ f) \cdot \mu$.

a) For every finite subset $J$ of $A'_q$, let us denote by $\lambda_J$ the supremum of the measures $|z' \circ m|$, where $z'$ runs over $J$; if $g_J = \sup_{z' \in J} |\langle z', f \rangle|$ then $\lambda_J = g_J \cdot \mu$ (Ch. V, §5, No. 2, Prop. 2). For every relatively compact open subset $U$ of $T$, let $\lambda_{J,U}$ be the restriction of $\lambda_J$ to $U$; let us first show that as $J$ runs over the directed set $\mathfrak{F}$ of finite subsets of $A'_q$, the family $(\lambda_{J,U})$ is bounded above in $\mathcal{M}(U)$. Indeed, for every function $h \geq 0$ in $K(U)$,

$$
\int h\,d\lambda_{J,U} = \int hg_J\,d\mu \leq \int^*(q \circ f)h\,d\mu \leq \|h\| \int_U^*(q \circ f)\,d\mu,
$$

whence our assertion (Ch. II, §2, No. 2). Let $\nu_U$ be the supremum of this family of measures in $\mathcal{M}(U)$. If $U'$ is a second relatively compact open subset of $T$ such that $U \subset U'$, then $\nu_U$ is the restriction of $\nu_{U'}$ to $U$, as follows immediately from the expression of the supremum of an increasing directed set of measures (Ch. II, §2, No. 2) and the fact that $\lambda_{J,U}$ is the restriction to $U$ of $\lambda_{J,U'}$. Thus there is one and only one positive measure $\nu$ whose restriction to each $U$ is $\nu_U$ (Ch. III, §2, No. 1, Prop. 1), and it is clear that $\nu = q(m)$.

b) Since the measures $\lambda_J$ have base $\mu$, so does their supremum $q(m)$ (Ch. V, §5, No. 5, Th. 2). If $f$ is $\mu$-measurable for the topology $\sigma(F, F')$ on $F$, it follows at once from the definitions that the mapping $g : t \mapsto (g_J(t))_{J \in \mathfrak{F}}$ of $T$ into the product space $\mathbf{R}^\mathfrak{F}$ is $\mu$-measurable. The restriction of $q \circ f = \sup_{J \in \mathfrak{F}} g_J$ to every compact subset of $T$ on which $g$ is continuous is lower semi-continuous; consequently $q \circ f$ is $\mu$-measurable (Ch. IV, §5, No. 5, Cor. of Prop. 8 and No. 10, Prop. 15). Let $K$ be a compact subset of T; it admits a partition consisting of a $\mu$-negligible set and a sequence $(K_n)$ of compact sets on which $g$ is continuous. Then $\int_{K_n}^*(q \circ f)\, d\mu = \sup_J \int_{K_n} g_J\, d\mu \leq \int_{K_n} dq(m)$ for all $n$ (Ch. IV, §1, No. 1, Th. 1 and Ch. V, §7, No. 1, Prop. 1), whence $\int_K^*(q \circ f)\, d\mu = \sum_n \int_{K_n}^*(q \circ f)\, d\mu \leq \int_K dq(m)$. But this proves that $q \circ f$ is locally $\mu$-integrable and that $\lambda_J \leq (q \circ f) \cdot \mu \leq q(m)$ for all $J \in \mathcal{F}$; whence, by definition, $q(m) = (q \circ f) \cdot \mu$.

#### Remark {#int-vi-s2-n4-rem-1 .statement}

Suppose that there exists in $A_q'$ a countable subset D that is dense for $\sigma(F', F)$; then, the function $q \circ f$ is always $\mu$-measurable, because $q(f(t)) = \sup_{z' \in D} |\langle z', f(t) \rangle|$ (Ch. IV, §5, No. 4, Cor. 1 of Th. 2). Then, for every compact subset K of T, $\int_K^*(q \circ f)\, d\mu = \sup_J \int_K g_J\, d\mu$, where J runs over the countable directed set of finite subsets of D (Ch. IV, §1, No. 1, Cor. of Th. 3); thus, one sees that in this case the condition that $\int_K^*(q \circ f)\, d\mu < +\infty$ for every compact subset K of T is necessary and sufficient for m to be $q$-majorizable.

#### Proposition 9 {#int-vi-s2-prop-9 .statement}

— *Let F be a finite-dimensional Banach space. Every measure m on T with values in F is a measure with base $|m|$. If $m = f \cdot |m|$, then $|f(t)| = 1$ locally almost everywhere for $|m|$. For m to have base $\mu$, it is necessary and sufficient that $|m|$ have base $\mu$, and if $m = g \cdot \mu$ then $|m| = |g| \cdot \mu$.

Let $(e_i)_{1 \leq i \leq n}$ and $(e'_i)_{1 \leq i \leq n}$ be dual bases of F and F' (A, II, §2, No. 6) with $|e'_i| = 1$ for all i. Then $|e'_i \circ m| \leq |m|$ for every index i, therefore (Ch. V, §5, No. 5, Th. 2) $e'_i \circ m = h_i \cdot |m|$, where $h_i$ is bounded and $|m|$-measurable. Setting $h = \sum_{i=1}^n h_i \cdot e_i$, we therefore have $m = h \cdot |m|$. If $m = f \cdot |m|$, Prop. 8 shows that $|m| = |f| \cdot |m|$, whence $|f(t)| = 1$ locally almost everywhere for $|m|$ (Ch. V, §5, No. 3, Cor. 2 of Prop. 3). The final assertion follows at once from Prop. 8.

#### Remark {#int-vi-s2-n4-rem-2 .statement}

If $z = \sum_{i=1}^n z_i e_i$ then $\psi(z_1, \ldots, z_n) = |z|$ is a positively homogeneous continuous function on $\mathbf{R}^n$. Setting $\mu_i = e'_i \circ m = h_i \cdot |m|$, by definition (Ch. V, §5, No. 9) $\psi(\mu_1, \ldots, \mu_n) = \psi(h_1, \ldots, h_n) \cdot |m| = |h| \cdot |m| = |m|$.

### 5. The Dunford–Pettis theorem

Let $\mu$ be a positive measure on T. A vectorial measure m on T, with values in F, is said to be *scalarly of base* $\mu$ (or to have base $\mu$ scalarly) if, for every $z' \in F'$, the scalar measure $z' \circ m$ has base $\mu$. If a vectorial measure $m$ with values in $F$ has base $\mu$, then it has base $\mu$ scalarly: for, if $m = f \cdot \mu$ then $z' \circ m = \langle z', f \rangle \cdot \mu$ for every $z' \in F'$. But there exist vectorial measures that are scalarly of base $\mu$ without having base $\mu$ (Exer. 17), and, on the other hand, there exist vectorial measures that are not scalarly of base $\nu$ for any positive measure $\nu$; note however that every *majorizable* measure $m$ with values in a *normed* space is scalarly of base $|m|$, by virtue of the Lebesgue–Nikodym theorem.

#### Example {#int-vi-s2-n5-exa-1 .statement}

— Let us take for $m$ the identity mapping of $\mathcal{H}(T)$. To say that $m$ is scalarly of base $\mu$ means that every real measure on $T$ has base $\mu$. In particular, the point measure $\varepsilon_t$ ($t \in T$) must have base $\mu$, which requires that $\mu(\{t\}) > 0$ for every $t \in T$, and implies in particular that every compact subset of $T$ is *countable*.

In this No. we are going to prove a result that generalizes one of the consequences of the Lebesgue–Nikodym theorem, namely, that the dual of $L^1(\mu)$ is $L^\infty(\mu)$ (Ch. V, §5, No. 8, Th. 4), and that gives a sufficient condition for a vectorial measure that is scalarly of base $\mu$ to have base $\mu$.

Let $\pi$ be the canonical mapping of $\mathcal{L}^\infty(\mu)$ onto $L^\infty(\mu)$. We shall say that a linear subspace $G$ of $L^\infty$ has the *lifting property* if there exists a linear mapping $\rho$ of $G$ into $\mathcal{L}^\infty(\mu)$ (called a *lifting* of $G$) such that $\pi \circ \rho$ is the identity on $G$ and $|\rho(f)(t)| \leq N_\infty(f)$ for all $t \in T$ and $f \in G$.

One proves that if $\mu$ is Lebesgue measure on $\mathbf{R}^n$, the entire space $L^\infty(\mathbf{R}^n, \mu)$ has the lifting property (Exer. 18).

#### Lemma 2 {#int-vi-s2-lem-2 .statement}

*Every separable subspace* $G$ *of the Banach space* $L^\infty(T, \mu)$ *has the lifting property*.

By the hypothesis, there exists a countable dense subset $H$ of $G$ that is a linear subspace with respect to the field $\mathbf{Q}$ of rational numbers; let $(h_n)$ be a (countable) basis of $H$ over $\mathbf{Q}$. For every integer $n$, let $h'_n$ be an element of $\mathcal{L}^\infty$ such that $\pi(h'_n) = h_n$, and let $\rho'$ be the $\mathbf{Q}$-linear mapping of $H$ into $\mathcal{L}^\infty$ defined by $\rho'(h_n) = h'_n$; it is clear that $\pi \circ \rho'$ is the identity on $H$. Moreover, for every $h \in H$ one has $|\rho'(h)(t)| \leq N_\infty(h)$ except at the points $t$ of a locally negligible set $A(h)$. Let $A$ be the union of the $A(h)$ for $h \in H$, which is also locally negligible. For every $h \in H$, denote by $\rho(h)$ the function $h'' \in \mathcal{L}^\infty$ such that $h''(t) = \rho'(h)(t)$ if $t \notin A$, and $h''(t) = 0$ if $t \in A$. It is clear that $\rho$ is a $\mathbf{Q}$-linear mapping of $H$ into the subspace $\mathcal{B}$ of bounded functions in $\mathcal{L}^\infty$, such that $\pi \circ \rho$ is the identity on $H$ and such that $|\rho(h)(t)| \leq N_\infty(h)$ for all $h \in H$ and $t \in T$. Since $\mathcal{B}$ is a Banach space for the norm $\|f\| = \sup_{t \in T} |f(t)|$ (Ch. IV, §5, No. 4, Th. 2), $\rho$ may be extended to a continuous $\mathbf{R}$-linear mapping, again denoted $\rho$, of $G$ into $\mathcal{B}$, which is obviously a lifting of $G$.

#### Definition 5 {#int-vi-s2-def-5 .statement}

— Let F be a Hausdorff locally convex space, $F'_s$ its dual equipped with the topology $\sigma(F', F)$. We denote by $\mathcal{L}_{F'_s}^\infty$ the vector space of mappings $f$ of T into $F'_s$, such that $f$ is scalarly $\mu$-measurable and is equal scalarly locally almost everywhere (for $\mu$) to a mapping of T into an equicontinuous subset of $F'$. We denote by $L_{F'_s}^\infty$ the quotient space of $\mathcal{L}_{F'_s}^\infty$ by the space of scalarly locally $\mu$-negligible mappings of T into $F'_s$.

When F satisfies the hypotheses of §1, No. 5, Prop. 13, the functions in $\mathcal{L}_{F'_s}^\infty$ are $\mu$-measurable for the weak topology $\sigma(F', F)$, but are not necessarily measurable for the strong topology on $F'$, even if F is a Banach space (§1, Exer. 17). Under the same conditions, the scalarly locally $\mu$-negligible mappings of T into $F'_s$ are identical to the locally $\mu$-negligible mappings of T into $F'_s$ (§1, No. 1, Remark 2).

When F is a separable normed space, the elements of $\mathcal{L}_{F'_s}^\infty$ are the mappings $f$ of T into $F'_s$ such that $f$ is scalarly $\mu$-measurable and $|f|$ is bounded in measure; one can then define a normed space structure on the space $L_{F'_s}^\infty$, by equipping it with the norm $N_\infty$ (Ch. IV, §6, No. 3).

#### Lemma 3 {#int-vi-s2-lem-3 .statement}

Let F be a Hausdorff locally convex space, $f$ an element of $\mathcal{L}_{F'_s}^\infty$. For every $z \in F$, one has $\langle z, f \rangle \in \mathcal{L}^\infty$, and the linear mapping $z \mapsto \pi(\langle z, f \rangle)$ of F into $L^\infty$ is continuous; if, moreover, F is a normed space, then $N_\infty(\langle z, f \rangle) \leq |z| \cdot \sup_{t \in T} |f(t)|$.

It is clear by definition that $\langle z, f \rangle$ is $\mu$-measurable and bounded in measure; replacing if necessary $f$ by a function belonging to the same class of $L_{F'_s}^\infty$, we can suppose in addition that $f(T) \subset V^\circ$, where V is a balanced convex neighborhood of 0 in F (which does not modify $\langle z, f \rangle$ except on a locally negligible set, depending on $z$). Then the relation $z \in V$ implies that $|\langle z, f(t) \rangle| \leq 1$ for all $t \in T$, which proves the continuity of $z \mapsto \pi(\langle z, f \rangle)$. The final assertion is obvious.

#### Lemma 4 {#int-vi-s2-lem-4 .statement}

Let F be a Hausdorff locally convex space, $f$ an element of $\mathcal{L}_{F'_s}^\infty$. For every numerical function $g \in \overline{\mathcal{L}}^1$, the function $gf$ is scalarly essentially $\mu$-integrable and $\int gf\, d\mu \in F'$.

For every $z \in F$, $\langle z, f \rangle$ belongs to $\mathcal{L}^\infty$, whence the first assertion. One can suppose moreover, without modifying $\int gf\, d\mu$, that $f(T) \subset V^\circ$, where V is a balanced convex neighborhood of 0 in F. Then the relation $z \in V$ implies $|\langle z, f(t) \rangle| \leq 1$ for all $t \in T$, whence $|\langle z, \int gf\, d\mu \rangle| = |\int \langle z, f \rangle g\, d\mu| \leq \overline{N}_1(g)$, which proves that $\int gf\, d\mu \in F'$.

#### Theorem 1 {#int-vi-s2-thm-1 .statement}

— Let F be a Hausdorff locally convex space that contains a countable dense subset. For every function $f \in \mathcal{L}_{F'_s}^\infty$ and every $z \in F$, let $v_f(z) = \pi(\langle z, f \rangle) \in L^\infty$; the mapping $f \mapsto v_f$ defines, by passage to the quotient, a linear bijection of $L_{F'}^\infty$ onto the space $\mathcal{L}(F; L^\infty)$ of continuous linear mappings of $F$ into $L^\infty$. *If $F$ is a normed space, this bijection is an isometry.*

In view of Lemma 3, the first assertion will be demonstrated if one proves that for every continuous mapping $u$ of $F$ into $L^\infty$, there exists a function $f \in \mathcal{L}_{F'}^\infty$ such that $\pi(\langle z, f \rangle) = u(z)$ for all $z \in F$, and that the class of $f$ in $L_{F'}^\infty$ is uniquely determined by this condition. The second point is immediate, because if $\pi(\langle z, f \rangle) = \pi(\langle z, f_1 \rangle)$ for all $z \in F$, then $f_1 - f$ is scalarly locally negligible. On the other hand, there exists a lifting $\rho$ of $u(F)$ into $\mathcal{L}^\infty$ (Lemma 2). For every $t \in T$, the mapping $z \mapsto \rho(u(z))(t)$ is a continuous linear form on $F$, that is, an element $f(t)$ of $F'$. The function $f$ is scalarly $\mu$-measurable since $\langle z, f \rangle = \rho(u(z)) \in \mathcal{L}^\infty$ for every $z \in F$; one has $\pi(\langle z, f \rangle) = u(z)$; finally, for every $t \in T$ and every $z$ belonging to the inverse image $V$ under $u$ of the unit ball of $L^\infty$,

$$
|\langle z, f(t) \rangle| = |\rho(u(z))(t)| \leq N_\infty(u(z)) \leq 1,
$$

which shows that $f(t) \in V^\circ$ for all $t \in T$.

If, moreover, $F$ is a normed space, the foregoing shows that

$$
\sup_{t \in T} |f(t)| \leq \|u\|.
$$

But on the other hand (Lemma 3), $N_\infty(u(z)) \leq |z| \cdot \sup_{t \in T} |f(t)|$, and this inequality continues to hold when $f$ is modified arbitrarily on a locally negligible set. It follows that $\|u\| = N_\infty(|f|)$.

#### Corollary 1 {#int-vi-s2-thm-1-cor-1 .statement}

*Let $F$ be a Hausdorff locally convex space containing a countable dense subset. For every function $f \in \mathcal{L}_{F'}^\infty$, every $z \in F$ and every function $g \in \mathcal{L}^1$, let $\Phi_f(z, \tilde{g}) = \int \langle z, f(t) \rangle g(t)\, d\mu(t)$. The mapping $f \mapsto \Phi_f$ defines, by passage to the quotient, a linear bijection of $L_{F'}^\infty$ onto the space $\mathcal{B}(F, L^1)$ of continuous bilinear forms on $F \times L^1$. *If $F$ is a normed space, this bijection is an isometry.*

One can suppose that $f(T)$ is an equicontinuous subset of $F'$. It is then clear that $\Phi_f$ is separately continuous, and, with the notations of Th. 1 and the Appendix, one has (taking into account the fact that $L^\infty$ is the dual of $L^1$ (Ch. V, §5, No. 8, Th. 4)) $^l \Phi_f = v_f$. The corollary then follows from Th. 1 above and from the Appendix, No. 1, Prop. 1 and its corollary.

#### Corollary 2 (Dunford–Pettis theorem) {#int-vi-s2-thm-1-cor-2 .statement}

— *Let $F$ be a Hausdorff locally convex space containing a countable dense subset. For every function $f \in \mathcal{L}_{F'}^\infty$ and every function $g \in \mathcal{L}^1$, let $w_f(\tilde{g}) = \int gf\, d\mu \in F'$ (Lemma 4). The mapping $f \mapsto w_f$ defines, by passage to the quotient, a linear bijection* of $L_{F_s}^\infty$ onto the space $\mathcal{R}(L^1, F')$ of linear mappings $u$ of $L^1$ into $F'$ such that the image under $u$ of the unit ball of $L^1$ is an equicontinuous subset of $F'$. *If $F$ is a normed space (in which case $\mathcal{R}(L^1, F')$ is the space of continuous linear mappings of $L^1$ into the strong dual of $F$), the bijection $f \mapsto w_f$ is an isometry.*

Taking into account the fact that $L^\infty$ is the dual of $L^1$, this follows from the preceding corollary and from the Appendix, No. 1, Prop. 1 and its corollary.

#### Remark {#int-vi-s2-n5-rem-1 .statement}

— It is clear that the mappings $u \in \mathcal{R}(L^1, F')$ are continuous for every $\mathcal{G}$-topology on $F'$ ($\mathcal{G}$ a covering of $F$ by bounded subsets). Conversely, if $F$ is assumed moreover to be *barreled*, then every continuous linear mapping of $L^1$ into $F'$ equipped with an $\mathcal{G}$-topology transforms the unit ball of $L^1$ into a bounded subset of $F'$, which is therefore equicontinuous (TVS, III, §4, No. 2, Th. 1).

#### Corollary 3 {#int-vi-s2-thm-1-cor-3 .statement}

*Let $F$ be a Hausdorff locally convex space containing a countable dense subset, $m$ a vectorial measure on $T$ with values in the weak dual $F'$ of $F$. If the image under $m$ of the set $B$ of functions $g$ in $\mathcal{K}(T)$ such that $\mu(|g|) \leq 1$ is contained in a closed and convex equicontinuous subset $H'$ of $F'$, then $m$ has base $\mu$ and there exists a density $f$ of $m$ with respect to $\mu$ such that $f(t) \in H'$ for all $t \in T$.*

The hypothesis implies that $m$ is continuous when $\mathcal{K}(T)$ is equipped with the topology induced by that of $\mathcal{L}^1(\mu)$ (defined by the semi-norm $N_1$); it may therefore be extended to a continuous linear mapping $u$ of $\mathcal{L}^1(\mu)$ into the completion $G$ of the weak dual of $F$; but since $H'$ is a compact subset of $G$ and the image under $u$ of the set $\overline{B}$ of $f \in \mathcal{L}^1$ such that $N_1(f) \leq 1$ is contained in the closure of $H'$ in $G$, one has $u(\overline{B}) \subset H'$, therefore $u$ maps $\mathcal{L}^1$ into $F'$. Since the relation $N_1(f) \leq \varepsilon$ implies that $u(f) \in \varepsilon H'$, one has $u(g) = 0$ if $g$ is $\mu$-negligible, and Cor. 2 may therefore be applied to the mapping of $L^1$ into $F'$ obtained from $u$ by passing to the quotient; whence the corollary.

#### Corollary 4 {#int-vi-s2-thm-1-cor-4 .statement}

*Let $F$ be a separable normed space, and $m$ a measure on $T$ with values in the strong dual $F'$, majorizable for the norm of $F'$. Then $m$ is a measure with base $|m|$, and if $m = f \cdot |m|$ then $|f(t)| = 1$ locally almost everywhere for $|m|$.*

By hypothesis, for every $z \in F$ such that $|z| \leq 1$, one has $|\langle z, m(g) \rangle| \leq |m|(|g|)$ for every function $g \in \mathcal{K}(T)$, consequently $|m(g)| \leq |m|(|g|)$ (TVS, IV, §2, No. 4, formula (1)). Since every ball in $F'$ is equicontinuous, Cor. 3 is applicable and shows that $m$ has base $|m|$; moreover, if $m = f \cdot |m|$ then $f$ is $|m|$-measurable for $\sigma(F', F)$ (§1, No. 5, Prop. 13) and $|m| = |f| \cdot |m|$ (No. 4, Prop. 8), which proves the corollary (Ch. V, §5, No. 3, Cor. 2 of Prop. 3).

If this corollary is applied to the case that $F$ if finite-dimensional, one recovers as a special case the first part of Prop. 9.

### 6. Dual of the space $L^1_F$ (F a separable Banach space)

#### Proposition 10 {#int-vi-s2-prop-10 .statement}

— *Let F be a separable Banach space. For every function $f \in \overline{\mathcal{L}}^1_F$ and every function $g \in \mathcal{L}_{F'_s}^\infty$, the numerical function $\langle f, g \rangle : t \mapsto \langle f(t), g(t) \rangle$ is essentially $\mu$-integrable, and*

$$
\left| \int \langle f, g \rangle \, d\mu \right| \leq \overline{N}_1(f) N_\infty(g) .
$$

*For every class $\dot{g} \in L_{F'_s}^\infty$, let $\theta(\dot{g})$ be the continuous linear form on $L^1_F$ deduced from the linear form $f \mapsto \int \langle f, g \rangle \, d\mu$ on $\overline{\mathcal{L}}^1_F$ by passage to the quotient; then $\theta$ is a linear isometry of $L_{F'_s}^\infty$ onto the strong dual $(L^1_F)'$ of the Banach space $L^1_F$.

For every compact subset K of T and every $\varepsilon > 0$, there exists a compact subset $K'$ of K such that $\mu(K - K') \leq \varepsilon$ and the restriction of $f$ (resp. $g$) to $K'$ is a continuous mapping of $K'$ into F (resp. into $F'_s$); consequently $g(K')$ is weakly compact, hence equicontinuous on $F'$ (TVS, III, §4, No. 2, Th. 1 or IV, §1, Exer. 10). Now, the restriction of the canonical bilinear form on $F \times F'$ to the product of F and an equicontinuous subset of $F'$ is continuous for the product topology of the topology of F and $\sigma(F', F)$ (GT, X, §2, No. 1, Cor. 4 of Prop. 1); it follows that the restriction of $\langle f, g \rangle$ to $K'$ is continuous, hence that $\langle f, g \rangle$ is $\mu$-measurable. Moreover,

$$
|\langle f(t), g(t) \rangle| \leq |f(t)| \cdot |g(t)| \leq |f(t)| N_\infty(g)
$$

locally almost everywhere, consequently $\langle f, g \rangle$ is essentially $\mu$-integrable and the inequality (3) holds (Ch. IV, §5, No. 6, Th. 5 and Ch. V, §1, No. 3, Lemma).

It remains to show that $\theta$ is a surjective isometry. Let $u$ be a continuous linear form on $L^1_F$. The mapping $(\tilde{h}, z) \mapsto u(\tilde{h}z)$ is a continuous bilinear form on $L^1 \times F$, because

$$
|u(\tilde{h}z)| \leq \|u\| \cdot N_1(hz) \leq \|u\| \cdot |z| \cdot N_1(h) .
$$

By Cor. 1 of Th. 1 of No. 5, there exists a mapping $g$ of T into $F'$, belonging to $\mathcal{L}_{F'_s}^\infty$, such that $|g(t)| \leq \|u\|$ for all $t \in T$ and such that $u(\tilde{h}z) = \int \langle hz, g \rangle \, d\mu$ for every function $h \in \mathcal{L}^1$ with class $\tilde{h}$ in $L^1$ and every $z \in F$. In other words, the linear forms $u$ and $\theta(\dot{g})$ coincide on the subspace of $L^1_F$ generated by the elements of the form $\tilde{h}z$ ($\tilde{h} \in L^1, z \in F$). Since this subspace is dense in $L^1_F$ (Ch. IV, §3, No. 5, Prop. 10), it follows that $u = \theta(\dot{g})$, which already proves that $\theta$ is surjective. Moreover, by (3), $\| \theta(\dot{g}) \| \leq N_\infty(g) \leq \| u \| = \| \theta(\dot{g}) \|$, whence $\| \theta(\dot{g}) \| = N_\infty(g)$, and this concludes the proof.

### 7. Integration of a vector-valued function with respect to a vectorial measure

#### Proposition 11 {#int-vi-s2-prop-11 .statement}

— *Let* $F, G, H$ *be three Banach spaces*, $\Phi$ *a continuous bilinear mapping of* $F \times G$ *into* $H$. *Let* $m$ *be a majorizable vectorial measure on* $T$, *with values in* $G$. *Then there exists one and only one continuous linear mapping* $I_{\Phi,m}$ *of* $\overline{\mathcal{L}}^1_F(|m|)$ *into* $H$ *such that, for every* $z \in F$ *and every numerical function* $h$ *integrable for* $|m|$, *one has* $I_{\Phi,m}(hz) = \Phi(z, \int h dm)$. *Moreover,

$$
|I_{\Phi,m}(f)| \leq \| \Phi \| \int |f| d|m|
$$

*for every function* $f \in \overline{\mathcal{L}}^1_F(|m|)$.

If there exists such a mapping, its value for a *step* function $f$ over the $|m|$-integrable sets is uniquely determined: for, it is known that one can then write $f = \sum_i a_i \varphi_{X_i}$, where the $X_i$ are $|m|$-integrable and disjoint, and the $a_i \in F$ (Ch. IV, §4, No. 9, Lemma). The value of $I_{\Phi,m}(f)$ must therefore be equal to $\sum_i \Phi(a_i, \int \varphi_{X_i} dm)$. Now, we have (No. 3, Prop. 5)

$$
\left| \sum_i \Phi \left( a_i, \int \varphi_{X_i} dm \right) \right| \leq \| \Phi \| \cdot \sum_i |a_i| \cdot |m|(X_i) = \| \Phi \| \int |f| d|m|,
$$

which shows first of all that the element $\sum_i \Phi(a_i, \int \varphi_{X_i} dm)$ of $H$ does not depend on the particular expression of $f$ in the form $\sum_i a_i \varphi_{X_i}$, hence that we may denote it by $I_{\Phi,m}(f)$. One verifies immediately that the mapping $I_{\Phi,m}$ so defined is linear on the space $\mathcal{E}_F$ of step functions over the $|m|$-integrable sets: for, it suffices to write two functions $f, g$ of $\mathcal{E}_F$ in the form $f = \sum_i a_i \varphi_{X_i}$ and $g = \sum_i b_i \varphi_{X_i}$ with the same finite family of pairwise disjoint $|m|$-integrable sets $X_i$ (which is possible by virtue of the Lemma of Ch. IV, §4, No. 9). The inequality (5) then shows that $I_{\Phi,m}$ is continuous on $\mathcal{E}_F$, and since this subspace is dense in $\overline{\mathcal{L}}^1_F$ (Ch. IV, §4, No. 10, Cor. 1 of Prop. 19 and Ch. V, §1, No. 3), one deduces from this the existence and uniqueness of $I_{\Phi,m}$, as well as the inequality (4).

One says that $I_{\Phi,m}(f)$ is the integral of $f$ *with respect to* $m$ (relative to the bilinear mapping $\Phi$); when the value of the bilinear mapping $\Phi$ at the point $(x,y)$ is denoted $xy$, we shall write $\int f\,dm$ instead of $I_{\Phi,m}(f)$.

With the notations of No. 6, the integral $\int \langle f, g \rangle\,d\mu$ is none other than $I_{\Phi,m}(f)$ with $\Phi(x,x') = \langle x, x' \rangle$ and $m = g \cdot \mu$.

#### Corollary {#int-vi-s2-n7-cor-1 .statement}

*If* $m$ *and* $m'$ *are two majorizable measures on* $T$, *with values in* $G$, *then* $I_{\Phi,m+m'} = I_{\Phi,m} + I_{\Phi,m'}$ *and* $I_{\Phi,\lambda m} = \lambda I_{\Phi,m}$ *for every scalar* $\lambda$.

The second assertion is immediate. The first signifies that for every function $f$ that is both $|m|$-integrable and $|m'|$-integrable,

$$
I_{\Phi,m+m'}(f) = I_{\Phi,m}(f) + I_{\Phi,m'}(f).
$$

The function $f$ is $(|m| + |m'|)$-integrable (Ch. V, §2, No. 2, Cor. 1 of Prop. 3), hence *a fortiori* $(|m + m'|)$-integrable, and the first member of (6) is indeed meaningful. To show (6), it suffices to do so for $f$ a step function over the $(|m| + |m'|)$-integrable sets, since the set of these functions is dense in $\mathcal{L}_F^1(|m| + |m'|)$ and the two members of (6) are continuous in the latter space, by virtue of (4). But for $f = a \varphi_X$, where $X$ is $(|m| + |m'|)$-integrable, the two members of (6) reduce to $\Phi(a, \int \varphi_X\,dm) + \Phi(a, \int \varphi_X\,dm')$, whence the corollary.

#### Remark {#int-vi-s2-n7-rem-1 .statement}

— When $m$ is of the form $b\mu$, where $b \in G$ and $\mu$ is a real measure on $T$,

$$
I_{\Phi,m}(f) = \int \Phi(f(t), b)\,d\mu(t)
$$

for every function $f \in \mathcal{L}_F^1(\mu)$, because both members are continuous on this space and coincide when $f$ is a step function over the $|\mu|$-integrable sets.

### 8. Complex measures

#### Definition 6 {#int-vi-s2-def-6 .statement}

*One calls complex measure on* $T$ *every continuous linear form on the complex vector space* $\mathscr{K}_C(T)$.\footnote{Cf. Ch. III, §1, No. 3, Def. 2.}

The space $\mathscr{M}_C(T)$ of complex measures on $T$ is thus the *dual* of the Hausdorff locally convex space $\mathscr{K}_C(T)$.

If $m$ is a complex measure on $T$, its restriction to $\mathscr{K}(T)$ is a vectorial measure on $T$ with values in $\mathbf{C}$ (regarded as a vector space over $\mathbf{R}$);

m is determined by this restriction, since if $f = f_1 + i f_2 \in \mathcal{H}_\mathbf{C}(T)$, the real part $f_1$ and the imaginary part $f_2$ of $f$ are in $\mathcal{H}(T)$, and $m(f) = m(f_1) + i m(f_2)$. Conversely, for every vectorial measure $m_0$ on T with values in $\mathbf{C}$, the formula $m(f) = m_0(f_1) + i m_0(f_2)$ defines a complex measure $m$, the only one on T whose restriction to $\mathcal{H}(T)$ is $m_0$. We shall therefore henceforth identify a complex measure with its restriction to $\mathcal{H}(T)$; such a measure $m$ is of the form $m = \mu_1 + i \mu_2$, where $\mu_1$ and $\mu_2$ are two real measures on T, which are called, respectively, the real part and the imaginary part of $m$. The support of $m$ is the union of the supports of $\mu_1$ and $\mu_2$. One knows that $m$ is majorizable (No. 3, Cor. of Prop. 4); we shall call absolute value of $m$ the positive measure $|m|$ corresponding to the absolute value $|x_1 + i x_2| = \sqrt{x_1^2 + x_2^2}$ on $\mathbf{C}$. One has $|m| = (\mu_1^2 + \mu_2^2)^{1/2}$ (No. 4, Remark following Prop. 9),$^3$ and $|\mu_1| \leq |m|$, $|\mu_2| \leq |m|$, $|m| \leq |\mu_1| + |\mu_2|$; moreover, $m$ is a measure with base $|m|$, and one can write $m = h \cdot |m|$, where $h \in \mathcal{L}_\mathbf{C}^\infty(|m|)$ and $|h(t)| = 1$ locally almost everywhere for $|m|$ (No. 4, Prop. 9).$^4$ The supports of $m$ and $|m|$ are the same.

For every mapping $f$ of T into a complex Banach space F, essentially integrable with respect to $|m|$, one can define (No. 7) the integral of $f$ with respect to $m$ (corresponding to the R-bilinear mapping $(x, \lambda) \mapsto \lambda x$ of $F \times \mathbf{C}$ into F), which will be denoted $\int f \, dm$; it follows at once from the uniqueness property of Prop. 11 that (with the preceding notations) $\int f \, dm = \int f \, d\mu_1 + i \int f \, d\mu_2 = \int f h \, d|m|$. We therefore have $m(f) = \int f \, dm$ for $f \in \mathcal{H}_\mathbf{C}(T)$. We say that $f$ is essentially integrable with respect to $m$ if it is so for $|m|$;$^5$ mappings that are $m$-integrable, $m$-measurable, locally $m$-integrable, $m$-negligible or locally $m$-negligible are defined similarly. We write
$$
\mathcal{L}_F^p(T, m) \quad \text{(resp. } \overline{\mathcal{L}}_F^p(T, m), \ L_F^p(T, m) \text{)}
$$
instead of $\mathcal{L}_F^p(T, |m|)$ (resp. $\overline{\mathcal{L}}_F^p(T, |m|), \ L_F^p(T, |m|)$); these are complex vector spaces.

For $f$ to be $m$-integrable (resp. essentially $m$-integrable), it is necessary and sufficient that $f$ be integrable (resp. essentially integrable) with respect to each of the four measures $\mu_1^+, \mu_1^-, \mu_2^+, \mu_2^-$, by virtue of the inequalities between $|m|, |\mu_1|, |\mu_2|$ and the relations $|\mu_k| = \mu_k^+ + \mu_k^-$ (Ch. V, §2, No. 2, Prop. 3 and its Cor. 1).

If $f$ is essentially $m$-integrable (resp. $m$-integrable), then $|f|$ is essen-

---
$^3$In particular, this definition of $|m|$ coincides with that in Ch. III, §1, No. 6 (cf. Ch. V, §5, No. 9).
$^4$Cf. Ch. V, §5, No. 5, Cor. 3 of Th. 2 for a sharper statement.
$^5$Cf. Ch. V, §1, remarks at the end of No. 3.

tially $|m|$-integrable (resp. $|m|$-integrable), and it follows from Prop. 11 that

$$
\left| \int \mathbf{f}\, dm \right| \leq \int |\mathbf{f}| \, d|m|.
$$

Let F and G be two complex Banach spaces, $u$ a continuous linear mapping of F into G. If $\mathbf{f}$ is an essentially $m$-integrable (resp. $m$-integrable) mapping of T into F, then $u \circ \mathbf{f}$ is essentially $m$-integrable (resp. $m$-integrable) and $\int (u \circ \mathbf{f})\, dm = u(\int \mathbf{f}\, dm)$; this follows at once from the foregoing and the analogous proposition for essentially $|m|$-integrable functions (Ch. IV, §4, No. 2, Th. 1 and Ch. V, §1, No. 3, Lemma and Def. 3).

Let $m$ be a complex measure on T and let $h$ be a locally $m$-integrable complex function. For every function $f \in \mathcal{K}_C(T)$, the function $fh$ is $m$-integrable and the mapping $f \mapsto \int fh\, dm$ is a complex measure, denoted $h \cdot m$ and called the measure *with density* $h$ with respect to $m$. If $m = g \cdot |m|$, it is clear that $h \cdot m = hg \cdot |m|$; since, moreover, $|g(t)| = 1$ locally almost everywhere for $|m|$, for $\mathbf{f}$ to be essentially integrable for $n = h \cdot m$ it is necessary and sufficient that $fh$ be essentially $m$-integrable, in which case $\int \mathbf{f}\, dn = \int (\mathbf{f}h)\, dm$. Moreover, $|h \cdot m| = |h| \cdot |m|$. We again say that every measure of the form $h \cdot m$ is a complex measure *with base* $m$; two complex measures $m, m'$ are said to be *equivalent* if each has a density with respect to the other, or, what amounts to the same, if $m' = h \cdot m$ with $h$ locally $m$-integrable and $h(t) \neq 0$ locally almost everywhere for $|m|$. It is clear that $m$ and $|m|$ are equivalent and that, for $m$ and $m'$ to be equivalent, it is necessary and sufficient that $|m|$ and $|m'|$ be so.

If $m$ and $m'$ are two complex measures on T, and $\mathbf{f}$ is a function with values in a complex Banach space F, essentially integrable (resp. integrable) for both $m$ and $m'$, then, for any complex numbers $\lambda$ and $\lambda'$, $\mathbf{f}$ is essentially integrable (resp. integrable) for $\lambda m + \lambda' m'$, and

$$
\int \mathbf{f}\, d(\lambda m + \lambda' m') = \lambda \int \mathbf{f}\, dm + \lambda' \int \mathbf{f}\, dm'.
$$

For, this follows from the Cor. of Prop. 11 of No. 7.

In addition, it follows from the definitions that

$$
|\lambda m + \lambda' m'| \leq |\lambda| \cdot |m| + |\lambda'| \cdot |m'|.
$$

One calls *conjugate measure* of a complex measure $m$ the complex measure $\overline{m}$ defined by $\overline{m}(f) = m(\overline{f})$ for $f \in \mathcal{K}_C(T)$. If $m = \mu_1 + i \mu_2$, where $\mu_1$ and $\mu_2$ are real measures, then $\overline{m} = \mu_1 - i \mu_2$ and $|\overline{m}| = |m|$; if $m = h \cdot |m|$ then $\overline{m} = \overline{h} \cdot |m|$. If $f$ is an essentially $m$-integrable (resp.

m-integrable) function with complex values, then $\overline{f}$ is essentially $\overline{m}$-integrable (resp. $\overline{m}$-integrable) and

$$
\int \overline{f}\, d\overline{m} = \overline{\int f\, dm}.
$$

#### Proposition 12 {#int-vi-s2-prop-12 .statement}

*Let m be a complex measure on T, p and q conjugate exponents (Ch. IV, §6, No. 4). The bilinear form $(f,g) \mapsto \int fg\, dm$ is defined and continuous on the product $\mathcal{L}_C^p(m) \times \mathcal{L}_C^q(m)$; the inequality $|\int fg\, dm| \leq N_p(f)N_q(g)$ holds, and $N_q(g)$ is the norm of the continuous linear form on $\mathcal{L}_C^p(m)$ deduced from the linear form $f \mapsto \int fg\, dm$ by passage to the quotient.

Moreover, if $1 \leq p < +\infty$, then every continuous linear form on the complex vector space $\mathcal{L}_C^p(m)$ is of the type $f \mapsto \int fg\, dm$, where $g$ is a function in $\mathcal{L}_C^q(m)$, whose class in $\mathcal{L}_C^q(m)$ is uniquely determined.

Since $m = h \cdot |m|$, where $|h(t)| = 1$ locally almost everywhere, the first assertion follows at once from Hölder’s inequality (Ch. IV, §6, No. 4, Th. 2); the second derives from Prop. 3 of Ch. IV, §6, No. 4. Finally, if $u$ is a continuous linear form on $\mathcal{L}_C^p$, its restriction to the (real) subspace $\mathcal{L}^p$ of $\mathcal{L}_C^p$ is a continuous $\mathbf{R}$-linear mapping of $\mathcal{L}^p$ into $\mathbf{C}$; if $1 \leq p < +\infty$, it is therefore of the type $f \mapsto \int fg_1\, d|m| + i \int fg_2\, d|m|$, where $g_1$ and $g_2$ belong to $\mathcal{L}^q$ (Ch. V, §5, No. 8, Th. 4); whence the final assertion, on setting $g = (g_1 + ig_2)h^{-1}$.

### 9. Bounded complex measures⁶

For every complex measure $m$ on $T$, one sets

$$
\|m\| = \sup_{\|f\| \leq 1,\, f \in \mathcal{H}_C(T)} |m(f)|.
$$

One says that $m$ is *bounded* if $\|m\| < +\infty$; it comes to the same to say that $m$ is continuous on $\mathcal{H}_C(T)$ equipped with the topology of uniform convergence, hence can be extended to a continuous linear form (of norm $\|m\|$) on the Banach space $\mathcal{H}_C(T)$ of continuous complex functions tending to 0 at infinity.

#### Lemma 5 {#int-vi-s2-lem-5 .statement}

*Let m be a complex measure on T, f an m-integrable complex function. Then $\int |f|\, d|m| = \sup |\int fh\, dm|$, as h runs over the set of functions in $\mathcal{H}_C(T)$ such that $|h(t)| \leq 1$ for all $t \in T$*.

⁶Cf. Ch. III, §1, No. 8.

If $m = g \cdot |m|$, then $\int |f| d|m| = \int |f g| d|m|$ and $\int f h \, dm = \int f g h \, d|m|$. Set $\zeta(t) = 0$ when $f(t)g(t) = 0$, and $\zeta(t) = \frac{f(t)g(t)}{|f(t)g(t)|}$ when $f(t)g(t) \neq 0$; $\zeta$ is $|m|$-measurable, thus for every $\varepsilon > 0$ there exists a compact subset K of T such that $\int_{T-K} |f| \, d|m| \leq \varepsilon$, the restriction of $\zeta$ to K is continuous, and $|\zeta(t)| = 1$ on K. Therefore, by virtue of Urysohn’s theorem, there exists a continuous function $\zeta_1$ defined on T, with complex values, such that $\zeta_1 = \zeta$ on K and such that $|\zeta_1(t)| \leq 2$ and $\zeta_1(t) \neq 0$ for every $t \in T$; setting $h(t) = \zeta_1(t)/|\zeta_1(t)|$, we see that $h$ is continuous on T, coincides with $\zeta$ on K, and is such that $|h(t)| = 1$ for all $t \in T$. Finally, let $u$ be a continuous mapping of T into $[0,1]$, equal to 1 on K and with compact support; setting $h_1 = h^{-1}u$, we have
$$
\left| \int f h_1 \, dm - \int |f| \, d|m| \right| \leq 2 \int_{T-K} |f| \, d|m| \leq 2\varepsilon ,
$$
which proves the lemma.

#### Proposition 13 {#int-vi-s2-prop-13 .statement}

— *Let m be a complex measure, and $\mu = |m|$. For m to be bounded, it is necessary and sufficient that $\mu$ be bounded, in which case $\|m\| = \|\mu\|$.*

We have $m = g \cdot \mu$, where $g$ is $\mu$-measurable and $|g(t)| = 1$ for all $t \in T$. If $\mu$ is bounded then, for every function $f \in \mathcal{K}_\mathbf{C}(T)$,
$$
|m(f)| = \left| \int f g \, d\mu \right| \leq N_\infty(fg)\|\mu\| = \|f\| \cdot \|\mu\|,
$$
therefore $m$ is bounded and $\|m\| \leq \|\mu\|$. If $m$ is bounded, then for every $f \in \mathcal{K}_\mathbf{C}(T)$ we have, on taking into account Lemma 5,
$$
|\mu(f)| \leq \|f\| \cdot \|m\|,
$$
therefore $\mu$ is bounded and $\|\mu\| \leq \|m\|$. Whence the proposition.

#### Corollary {#int-vi-s2-n9-cor-1 .statement}

— *Let m be a bounded complex measure. Every function $f \in \mathcal{L}_\mathbf{F}^\infty(m)$ is then m-integrable, and $\left| \int f \, dm \right| \leq N_\infty(f)\|m\|$.*

For, $f$ is $m$-measurable and, setting $\mu = |m|$, we have
$$
\int^* |f| \, d\mu \leq N_\infty(f)\|\mu\| = N_\infty(f)\|m\|,
$$
therefore $f$ is $|m|$-integrable (Ch. IV, §5, No. 6, Th. 5) and
$$
\left| \int f \, dm \right| \leq \int |f| \, d\mu \leq N_\infty(f)\|m\|.
$$

### 10. Image of a complex measure; induced complex measure; product of complex measures\footnote{Cf. Ch. V, §6, No. 4; Ch. IV, §5, No. 7 and Ch. V, §7; Ch. III, §4 and Ch. V, §8, Nos. 2–5.}

Let $m$ be a complex measure on $T$, and let $\pi$ be a mapping of $T$ into a locally compact space $X$. We shall say that $\pi$ is $m$-proper if $\pi$ is $|m|$-proper (Ch. V, §6, No. 1, Def. 1); it is then immediate that for every function $f \in \mathcal{H}_C(X)$, the function $f \circ \pi$ is essentially $m$-integrable and

$$
\left| \int (f \circ \pi)\, dm \right| \leq \int |f \circ \pi|\, d|m| = \int |f|\, d(\pi(|m|)),
$$

therefore the mapping $f \mapsto \int (f \circ \pi)\, dm$ is continuous on $\mathcal{H}_C(X)$, in other words is a complex measure on $X$, which is denoted $\pi(m)$ and called the *image* of $m$ under $\pi$. Moreover, it follows from (8) that $|\pi(m)| \leq \pi(|m|)$. If $m$ and $m'$ are two complex measures on $T$ and if $\pi$ is both $m$-proper and $m'$-proper, then $\pi$ is $(\lambda m + \lambda' m')$-proper for any complex scalars $\lambda, \lambda'$, and $\pi(\lambda m + \lambda' m') = \lambda \pi(m) + \lambda' \pi(m')$.

Let $Y$ be a locally compact subspace of $T$. For every function $f \in \mathcal{H}_C(Y)$, the function $f'$ on $T$, defined by $f'(t) = f(t)$ if $t \in Y$ and by $f'(t) = 0$ if $t \notin Y$, is $m$-integrable (Ch. IV, §5, No. 7); it is immediate that the mapping $f \mapsto \int f'\, dm$ is a complex measure on $Y$, called the measure *induced* on $Y$ by $m$ and denoted $m_Y$. If $m = g \cdot |m|$, it is clear that $m_Y = g_Y \cdot |m|_Y$, where $g_Y$ is the restriction to $Y$ of the function $g$, which is locally integrable for $|m|_Y$ (Ch. V, §7, No. 1); moreover, since $|g_Y| = 1$ locally almost everywhere for $|m|_Y$ (Ch. V, §7, No. 1, Cor. 1 of Prop. 1), we have $|m_Y| = |m|_Y$.\footnote{Cf. Ch. IV, §5, No. 7, Lemma 3.}

Let $T$ and $T'$ be two locally compact spaces, $m$ (resp. $m'$) a complex measure on $T$ (resp. $T'$). Write $m = g \cdot |m|$ and $m' = g' \cdot |m'|$. The function $g \otimes g'$ is locally integrable on $T \times T'$ for the positive measure $|m| \otimes |m'|$ (Ch. V, §8, No. 5, Prop. 10), and one verifies immediately that if $g$ (resp. $g'$) is replaced by a function $g_1$ (resp. $g'_1$) equal to $g$ (resp. $g'$) locally almost everywhere for $|m|$ (resp. $|m'|$), then $g_1 \otimes g'_1$ is equal to $g \otimes g'$ locally almost everywhere for $|m| \otimes |m'|$. The complex measure $(g \otimes g') \cdot (|m| \otimes |m'|)$ on $T \times T'$ therefore depends only on $m$ and $m'$; it is denoted $m \otimes m'$ and is called the *product* measure of $m$ and $m'$. Since $|g \otimes g'| = 1$ locally almost everywhere for $|m| \otimes |m'|$ (Ch. V, §8, No. 2, Prop. 4), we have $|m \otimes m'| = |m| \otimes |m'|$.\footnote{Cf. Ch. III, §4, No. 2, Prop. 3.}

The reader will easily verify that all of the propositions proved in Ch. V relative to the image of a positive measure, the measure induced by a positive measure, and the product of positive measures, except those in which upper integrals or essential upper integrals intervene, remain valid when the positive measures are replaced by arbitrary complex measures.

Finally, one defines as in §1 the concept of scalarly essentially m-integrable function for a complex measure m; for a function f to have this property, it is necessary and sufficient that f be scalarly essentially integrable with respect to $|\mu_1|$ and $|\mu_2|$, where $\mu_1$ and $\mu_2$ are the real and imaginary parts of $m$, in which case $\int f dm = \int f d\mu_1 + i \int f d\mu_2$. We leave to the reader the task of carrying over the results of §1 to complex measures.

### Exercises {#int-vi-s2-exercises}

See the [exercises for § 2](exercises/s2/).
