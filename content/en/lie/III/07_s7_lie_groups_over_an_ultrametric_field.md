---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: III
chapter_title: LIE GROUPS
section: 7
section_title: Lie groups over an ultrametric field
lang: en
source: lie-i-iii
pdf_pages: 0344-0355, 0409-0413
extraction: ocr
subsections:
    - "no": 1
      title: PASSAGE FROM LIE ALGEBRAS TO LIE GROUPS
      page: 0
      pdf_page: 345
    - "no": 2
      title: EXPONENTIAL MAPPINGS
      page: 0
      pdf_page: 346
    - "no": 3
      title: STANDARD GROUPS†
      page: 0
      pdf_page: 346
    - "no": 4
      title: FILTRATION OF STANDARD GROUPS
      page: 0
      pdf_page: 348
    - "no": 5
      title: POWERS IN STANDARD GROUPS
      page: 0
      pdf_page: 349
    - "no": 6
      title: LOGARITHMIC MAPPING
      page: 0
      pdf_page: 351
statements: 26
exercises: 10
content_sha256: 0c680762cdc1f3ee887ddeb36734fc91db046db61ac47e4409f0c49baf665b4b
---

## § 7. LIE GROUPS OVER AN ULTRAMETRIC FIELD

In this paragraph, the valued field $K$ is assumed to be ultrametric and of characteristic 0. Let $A$ denote the valuation ring of $K$, $m$ the maximal ideal of $A$ and $p$ the characteristic of the residue field $A/m$. If $K$ is locally compact, then $p \neq 0$ (*Commutative Algebra*, Chapter VI, § 9, Theorem 1).

### 1. PASSAGE FROM LIE ALGEBRAS TO LIE GROUPS

#### Proposition 1 {#lie-iii-s7-prop-1 .statement}

Let G be a Lie group germ with identity element e. There exists a fundamental system of open neighbourhoods of e in G consisting of Lie subgroups of G.

Let L(G) be given a norm compatible with its topology and such that $\| [x, y] \| \leq \| x \| \| y \|$ for all x, y in L(G). Let G_1 be the Lie group defined by L(G). By § 4, no. 2, Theorem 2, G and G_1 are locally isomorphic. Then it suffices to apply § 4, no. 2, Lemma 3 (iii).

#### Theorem 1 {#lie-iii-s7-thm-1 .statement}

Let L be a complete normable Lie algebra. There exists a Lie group G such that L(G) is isomorphic to L. Two such groups are locally isomorphic.

The first assertion has been proved in § 4, no. 2, Lemma 3. The second is a special case of § 4, no. 2, Theorem 2.

#### Theorem 2 {#lie-iii-s7-thm-2 .statement}

Let G be a Lie group and h a Lie subalgebra of L(G) admitting a topological supplement. There exists a Lie subgroup H of G such that L(H) = h. If H_1 and H_2 are Lie subgroups of G such that L(H_1) = L(H_2) = h, then H_1 \cap H_2 is open in H_1 and H_2.

The first assertion follows from Proposition 1 and § 4, no. 2, Theorem 3. The second is a special case of § 4, no. 2, Theorem 3.

#### Theorem 3 {#lie-iii-s7-thm-3 .statement}

Let G and H be Lie groups and h a continuous morphism of L(G) into L(H).

(i) There exist an open subgroup G' of G and a Lie group morphism $\phi$ of G' into H such that $h = L(\phi)$.

(ii) Let G_1, G_2 be open subgroups of G and $\phi_i$ a morphism of G_i into H such that $h = L(\phi_i)$. Then $\phi_1$ and $\phi_2$ coincide on an open subgroup of G.

By Proposition 1, this follows from § 4, no. 1, Theorem 1.

#### Proposition 2 {#lie-iii-s7-prop-2 .statement}

Let G be a Lie group and h a Lie subalgebra of L(G) admitting a topological supplement. The following conditions are equivalent:

(i) There exist an open subgroup G' of G and a normal Lie subgroup H of G' such that L(H) = h.

(ii) h is an ideal of L(H).

If there exist G' and H with the properties of (i), then L(G') = L(G) and L(H) is an ideal of L(G') by § 3, no. 12, Proposition 47.

Suppose that h is an ideal of L(G). There exists a Lie group F such that L(F) = L(G)/h (Theorem 1). Let h be the canonical morphism of L(G) onto L(F). By Theorem 3 (i), there exist an open subgroup G' of G and a Lie group morphism $\phi$ of G' into F such that $L(\phi) = h$. By § 3, no. 8, the kernel H of $\phi$ is a Lie subgroup of G' and $L(H) = \mathrm{Ker}\ L(\phi) = \mathrm{Ker}\ h = h$. Finally, H is normal in G' since $H = \mathrm{Ker}\ \phi$.

### 2. EXPONENTIAL MAPPINGS

#### Proposition 3 {#lie-iii-s7-prop-3 .statement}

Let G be a Lie group. There exists an exponential mapping $\phi$ of G with the following properties:
(i) $\phi$ is defined on an open subgroup U of the additive group $L(G)$;
(ii) $\phi(U)$ is an open subgroup of G and $\phi$ is an isomorphism of the analytic manifold U onto the analytic manifold $\phi(U)$;
(iii) $\phi(nx) = \phi(x)^n$ for all $x \in U$ and all $n \in \mathbf{Z}$.

Let $L(G)$ be given a norm compatible with its topology and such that $\| [x, y] \| \leq \| x \| \| y \|$ for $x, y$ in $L(G)$. Let $G_1$ be the Lie group defined by $L(G)$. Let $\psi = \mathrm{Id}_{G_1}$, which is an exponential mapping of $G_1$. For all $\mu > 0$, let $L_\mu$ be the set of $x \in L(G)$ such that $\| x \| < \mu$. Then, for $\mu$ sufficiently small, $L_\mu$ is an open subgroup of the additive group $L(G)$, $\psi(L_\mu)$ is an open subgroup of $G_1$ (§ 4, no. 2, Lemma 3), $\psi|L_\mu$ is an isomorphism of analytic manifolds of $L_\mu$ onto $\psi(L_\mu)$ and $\psi(nx) = \psi(x)^n$ for all $x \in L_\mu$ and all $n \in \mathbf{Z}$. The $L_\mu$ form a fundamental system of neighbourhoods of 0 in $L(G)$. By Theorem 1, there exist $\mu$ and an open subgroup $G'$ of G such that $\psi(L_\mu)$ and $G'$ are isomorphic, whence the proposition.

#### Proposition 4 {#lie-iii-s7-prop-4 .statement}

Let G be a Lie group and $\phi$ an injective exponential mapping of G. Suppose that $p > 0$. For all $x, y$ in $L(G)$,

(1)
$$
x + y = \lim_{n \to +\infty} p^{-n} \phi^{-1}(\phi(p^n x) \phi(p^n y))
$$
(2)
$$
[x, y] = \lim_{n \to +\infty} p^{-2n} \phi^{-1}(\phi(p^n x) \phi(p^n y) \phi(-p^n x) \phi(-p^n y)).
$$

These are special cases of Proposition 4 of § 4, no. 3.

### 3. STANDARD GROUPS†

If $S(X_1, X_2, \ldots, X_n)$ is a formal power series with coefficients in $A$, then, for all $x_1, \ldots, x_r$ in m, the series $S(x_1, x_2, \ldots, x_r)$ is convergent. More precisely, $m \times m \times \cdots \times m$ is contained in the domain of absolute convergence of $S$ (Differentiable and Analytic Manifolds, R, 4.1.3).

#### Definition 1 {#lie-iii-s7-def-1 .statement}

Let r be an integer $\geq 0$. A standard group of dimension r over K is a Lie group G with the following properties:
(i) the underlying analytic manifold of G is $m \times m \times \cdots \times m$ (r factors);
(ii) there exists a formal power series F in 2r variables with coefficients in $A^r$, without constant term, such that $x.y = F(x, y)$ for all $x, y$ in G.

Then $0.0 = 0$ and hence the identity element of G is the origin of $m \times m \cdots \times m$.

† The results of nos. 3 and 4 and their proofs remain true when the characteristic of K is $> 0$.

L(G) will be identified with K'. By § 5, formula (13), the constants of structure of L(G) with respect to the canonical basis belong to A. We shall need, in the same proof to consider the elements of m × ... × m, now as elements of G, now as elements of L(G).

#### Example {#lie-iii-s7-n3-exa-1 .statement}

Let G = 1 + M_n(m), which is an open subset of M_n(K). If x ∈ G, then det x ∈ 1 + m and hence G ⊂ GL(n, K). Clearly GG ⊂ G. If x = 1 + y with y ∈ M_n(m), the calculation of the inverse of a matrix proves first that x^{-1} ∈ M_n(A); if we write x^{-1} = 1 + y', then y + y' + yy' = 0, hence y' ∈ M_n(m) and therefore x^{-1} ∈ G. Thus G is an open subgroup of GL(n, K). We identify G with m^{n^2} by means of the mapping (\delta_{ij} + y_{ij}) ↦ (y_{ij}). Clearly G is a standard group.

#### Theorem 4 {#lie-iii-s7-thm-4 .statement}

Let G be a finite-dimensional Lie group. There exists an open subgroup of G isomorphic to a standard group.

By replacing G by a group isomorphic to an open subgroup of G, the problem is reduced to the case where G is an open subset of K', with identity element 0 and where the coordinates of the product x.y and the inverse x^{[-1]} are given by formulae

(3) $$(x.y)_i = x_i + y_i + \sum_{|\alpha| \geq 1, |\beta| \geq 1} c_{\alpha \beta i} x^\alpha y^\beta \quad (i = 1, 2, \ldots, r)$$

(4) $$(x^{[-1]})_i = -x_i + \sum_{|\alpha| > 1} d_{\alpha i} x^\alpha \quad (i = 1, 2, \ldots, r)$$

where the series on the right hand side are convergent for x, y in G (§ 5, no. 1). Let λ ∈ K* and let the group law be transported from G to G' = λG by the homothety of ratio λ. For x', y' in G', the product x'.y' and the inverse x'^{[-1]} evaluated in G' have coordinates

$$(x'.y')_i = x'_i + y'_i + \sum_{|\alpha| \geq 1, |\beta| \geq 1} c'_{\alpha \beta i} {x'}^\alpha {y'}^\beta \quad (i = 1, 2, \ldots, r)$$

$$({x'}^{[-1]})_i = -x'_i + \sum_{|\alpha| > 1} d'_{\alpha i} {x'}^\alpha \quad (i = 1, 2, \ldots, r)$$

where

$$c'_{\alpha \beta i} = \lambda^{-|\alpha|-|\beta|+1} c_{\alpha \beta i}, \qquad d'_{\alpha i} = \lambda^{-|\alpha|+1} d_{\alpha i}.$$

As the series (3) and (4) are convergent, we see that, for |λ| sufficiently large, for all α, β, i,

$$|c'_{\alpha \beta i}| \leq 1, \qquad |d'_{\alpha i}| \leq 1$$

that is c'_{\alpha \beta i} ∈ A and d'_{\alpha i} ∈ A; and on the other hand G' ⊃ m × m × ... × m. Then m × m × ... × m is an open subgroup of G' and is a standard group.

### 4. FILTRATION OF STANDARD GROUPS

We again use the notation of Definition 1. We choose a number $a > 1$ and a real valuation $v$ of $K$ such that $|x| = a^{-v(x)}$ for all $x \in K$ (Commutative Algebra, Chapter VI, § 6, Proposition 3). If $a$ is a non-zero (and hence open) ideal of $A$ contained in $m$, let $G(a)$ denote the set of elements of $G$ whose coordinates belong to $a$. If $\lambda \in \mathbf{R}$, let $a_\lambda$ (resp. $a_\lambda^+$) denote the set of $x \in K$ such that $v(x) \geq \lambda$ (resp. $v(x) > \lambda$); then $a_0 = A$, $a_0^+ = m$. For $x = (x_1, \ldots, x_r) \in G$, we shall write

$$
\omega(x) = \inf(v(x_1), \ldots, v(x_r)).
$$

#### Proposition 5 {#lie-iii-s7-prop-5 .statement}

Let $G$ be a standard group.

(i) If $a$ is a non-zero ideal of $A$ contained in $m$, $G(a)$ is an open normal subgroup of $G$.

(ii) The $G(a_\lambda)$, for $\lambda > 0$, form a fundamental system of neighbourhoods of $e$ in $G$.

(iii) Suppose that $a_\lambda \subset a$ for $\lambda \geq \lambda_0$ and let the $G(a)/G(a_\lambda)$, for $\lambda \geq \lambda_0$, be given the discrete topology. Then the topological group $G(a)$ is the inverse limit of the groups $G(a)/G(a_\lambda)$.

(iv) Let $a, b$ be non-zero ideals of $A$ contained in $m$ such that $a \supset b \supset a^2$. The mapping $x \mapsto (x_1 \bmod b, \ldots, x_r \bmod b)$ of $G(a)$ into $(a/b) \times \cdots \times (a/b)$ defines on passing to the quotient an isomorphism of the group $G(a)/G(b)$ onto the additive group $(a/b) \times \cdots \times (a/b)$.

If $x \in G$ and $y \in G(a)$, the coordinates of $x$ and $x.y$ are equal modulo $a$. Hence, for $x', x''$ in $G$ and $y', y''$ in $G(a)$, the coordinates of $x'.x''$ and $(x'.y').(x''.y'')$ are equal modulo $a$. This proves (i).

(ii) is obvious.

(iii) follows from the above and General Topology, Chapter III, § 7, Proposition 2.

If $x \in G(a)$ and $y \in G(a)$, the coordinates of $x.y$ are congruent to those of $x + y$ modulo $G(a^2)$ by formula (4) of § 5. This proves (iv).

#### Corollary {#lie-iii-s7-n4-cor-1 .statement}

Suppose that $K$ is locally compact and let $q = \mathrm{Card}(A/m)$.

(i) If $a = m^a$ and $b = m^b$ with $b \geq a \geq 1$, $G(a)/G(b)$ is a $p$-group of cardinal $q^{r(b-a)}$.

(ii) $G(a)$ is an inverse limit of $p$-groups.

The number of elements in $G(a)/G(b)$ is $(\mathrm{Card}(a/b))^r$; if $b = a + 1$, $a/b$ is a 1-dimensional vector space over $A/m$, whence (i) in this case; the general case follows by induction on $b - a$. Assertion (ii) follows from (i) and Proposition 5 (iii).

#### Proposition 6 {#lie-iii-s7-prop-6 .statement}

Let $a, b, c, c'$ be non-zero ideals of $A$ contained in $m$ such that

$$
c' \subset c, \quad ab \subset c, \quad ab^2 \subset c', \quad a^2b \subset c'.
$$

If $x \in G(a)$ and $y \in G(b)$, then $x^{[-1]}y^{[-1]}x.y, x.y.x^{[-1]}y^{[-1]}$ and $[x,y]$ belong to $G(c')$ and are congruent modulo $G(c')$.

By § 5, no. 2, Proposition 1, there exist $c_{\alpha\beta} \in A'$ such that
$$
x^{[-1]}y^{[-1]}x.y - [x,y] = \sum_{|\alpha| + |\beta| \geq 3} c_{\alpha\beta} x^\alpha y^\beta.
$$
If $x = 0$ or $y = 0$, then $x^{[-1]}y^{[-1]}x.y - [x,y] = 0$; hence $c_{0\beta} = c_{\alpha 0} = 0$.
On the other hand, the conditions
$$
x \in G(a), \quad y \in G(b), \quad |\alpha| \geq 1, \quad |\beta| \geq 1, \quad |\alpha| + |\beta| \geq 3
$$
imply
$$
c_{\alpha\beta} x^\alpha y^\beta \in G(a^2 b + ab^2) \subset G(c')
$$
and hence $x^{[-1]}y^{[-1]}x.y - [x,y] \in G(c')$. We see similarly that
$$
x.y.x^{[-1]}y^{[-1]} - [x,y] \in G(c').
$$
Finally, by § 5, formula (13), $[x,y] \in G(ab) \subset G(c)$.

#### Proposition 7 {#lie-iii-s7-prop-7 .statement}

(i) *The family* $(G(a_\lambda))$ *is a central filtration on* $G$ *(Chapter II, § 4, no. 4, Definition 2)*.
(ii) *For* $\lambda \in \mathbf{R}_+^*$, $G(a_\lambda) = \{ x \in G | \omega(x) \geq \lambda \}$, $G(a_\lambda^+) = \{ x \in G | \omega(x) > \lambda \}$.
(ii) is obvious. We prove (i). Clearly $G(a_\lambda) = \bigcap_{\mu < \lambda} G(a_\mu)$ and $G = \bigcup_{\lambda > 0} G(a_\lambda)$.
On the other hand, if $x \in G(a_\lambda)$ and $y \in G(a_\mu)$, then
$$
x^{[-1]}y^{[-1]}x.y \in G(a_{\lambda+\mu})
$$
by Proposition 6 applied with $a = a_\lambda, b = a_\mu, c = c' = a_{\lambda+\mu}$.

By Chapter II, § 4, no. 4, we can form the group $\mathrm{gr}(G)$ associated with the group $G$, with the central filtration $(G(a_\lambda))$. Writing $G_\lambda = G(a_\lambda)/G(a_\lambda^+)$ for all $\lambda > 0$, we obtain $\mathrm{gr}(G) = \bigoplus_{\lambda > 0} G_\lambda$. Recall (*loc. cit.*, Proposition 1) that the commutator in $G$ allows us to define a bracket in $\mathrm{gr}(G)$ with which $\mathrm{gr}(G)$ is a Lie algebra, as follows: if $\bar{x} \in G_\lambda$ and $\bar{y} \in G_\mu$, choose a representative $x$ of $\bar{x}$ in $G(a_\lambda)$ and a representative $y$ of $\bar{y}$ in $G(a_\mu)$; then $[\bar{x}, \bar{y}]$ is the class of $x^{[-1]}y^{[-1]}x.y \in G(a_{\lambda+\mu})$ in $G_{\lambda+\mu}$. By Proposition 6, applied with $a = a_\lambda, b = a_\mu, c = a_{\lambda+\mu}, c' = a_{\lambda+\mu}^+$, we see that $[\bar{x}, \bar{y}]$ is also the class of $[x, y]$ in $G_{\lambda+\mu}$. Thus, when $G$ is considered as a Lie subalgebra of $L(G) = K^r$, filtered by the $G(a_\lambda)$, the associated graded Lie algebra (Chapter II, § 4, no. 3) is equal to $\mathrm{gr}(G)$.

### 5. POWERS IN STANDARD GROUPS

We preserve the notation of no. 4.

#### Proposition 8 {#lie-iii-s7-prop-8 .statement}

*Let* $n \in \mathbf{Z}$ *and* $h_n$ *be the mapping* $x \mapsto x^n$ *of* $G$ *into* $G$. *Let* $a$ *be a non-zero ideal of* $A$ *contained in* $m$, *such that* $n \notin a$. *Then* $h_n|G(a)$ *is an isomorphism of the analytic manifold* $G(a)$ *onto the analytic manifold* $G(na)$.

By definition of standard groups, $h_n$ is equal on the whole of $G$ to the sum of an integral series with coefficients in $A'$. By § 5, formula (4), this series is of the form
$$
h_n(x) = nx + \sum_{|\alpha| \geq 2} a_\alpha x^\alpha.
$$
Hence, for $x \in G$,
$$
\begin{align*}
h_n(nx) &= n^2 \left( x + \sum_{|\alpha| \geq 2} a_\alpha n^{|\alpha|-2} x^\alpha \right) \\
&= n^2 S(x)
\end{align*}
$$
where we write $S(x) = x + \sum_{|\alpha| \geq 2} a_\alpha n^{|\alpha|-2} x^\alpha$. This series $S(x)$ defines an analytic mapping, also denoted by $S$, of $G$ into $G$. By *Algebra*, Chapter IV, § 6, Proposition 8, there exists an integral series $S'$ in $r$ variables with coefficients in $A'$ such that $S'(S(X)) = S(S'(X)) = X$. Hence $S$ is an isomorphism of the analytic manifold $G$ onto itself and, for every non-zero ideal $b$ of $A$ contained in $m$, $S(G(b)) \subset G(b)$, $S'(G(b)) \subset G(b)$ and therefore
$$
S(G(b)) = G(b).
$$
As $h_n(y) = n^2 S \left( \frac{1}{n} y \right)$ for $y \in nG$, we see that $h_n|nG(b)$ is an isomorphism of the analytic manifold $nG(b)$ onto the analytic manifold $n^2 G(b)$. But, as $n \notin a$, $|n| > |\lambda|$ for all $\lambda \in a$, hence $n^{-1} a \subset m$ and hence $a$ is of the form $nb$ where $b$ is a non-zero ideal of $A$ contained in $m$.

#### Corollary {#lie-iii-s7-n5-cor-1 .statement}

*If $n$ is invertible in $A$, $h_n$ is an isomorphism of the analytic manifold $G$ onto itself. For every non-zero ideal $a$ of $A$ contained in $m$, $h_n(G(a)) = G(a)$. For all $x \in G$, $\omega(x^n) = \omega(x)$.*

This follows immediately from Proposition 8.

#### Proposition 9 {#lie-iii-s7-prop-9 .statement}

*Suppose that $p \neq 0$.
(i) Let $a, b$ be non-zero ideals of $A$ such that $b \subset a \subset m$. In the group $G(a)/G(b)$, every element has order a power of $p$.
(ii) Suppose that $v(p) = 1$. If $x \in G$ is such that $\omega(x) > \frac{1}{p-1}$, then*
$$
\omega(x^p) = \omega(x) + 1.
$$
By § 5, formula (4), for all $x \in G$,
$$
x^p = px + \sum_{|\alpha| \geq 2} c_\alpha x^\alpha
$$
where $c_\alpha \in A'$ for all $\alpha$. Even for proving (i) it can be assumed that $v(p) = 1$. Then if $\omega(x) \geq 1$, it follows that $\omega(x^p) \geq \omega(x) + 1$ and hence $\omega(x^{p^n})$ tends to $+\infty$ as $n$ tends to $+\infty$; this proves (i). As $\binom{p}{i}$ is divisible by $p$ for $1 \leq i \leq p - 1$, Proposition 2 of § 5, no. 3, proves that $c_\alpha \in pA'$ for
$$
2 \leq |\alpha| \leq p - 1
$$
and hence
$$
\omega(c_\alpha x^\alpha) > \omega(px) = \omega(x) + 1 \quad \text{for } 2 \leq |\alpha| \leq p - 1.
$$
On the other hand, if $|\alpha| \geq p$, $\omega(c_\alpha x^\alpha) \geq p \omega(x)$ and $p \omega(x) > \omega(x) + 1$ if $\omega(x) > \frac{1}{p - 1}$. This proves (ii).

### 6. LOGARITHMIC MAPPING

#### Lemma 1 {#lie-iii-s7-lem-1 .statement}

Suppose that $p \neq 0$. Let $G$ be a Lie group, $G_1$ an open subgroup of $G$ which is isomorphic to a standard group and $x \in G$. The following conditions are equivalent:
(i) there exists a power of $x$ which belongs to $G_1$;
(ii) there exists a strictly increasing sequence $(n_i)$ of integers such that $x^{n_i}$ tends to $e$ as $i$ tends to $+\infty$.
(ii) $\Rightarrow$ (i): obvious.
(i) $\Rightarrow$ (ii): suppose that $y = x^m \in G_1$. By Proposition 9 (i) of no. 5, $y^{p^n}$ tends to $e$ as $n$ tends to $+\infty$, in other words $x^{m p^n}$ tends to $e$ as $n$ tends to $+\infty$.

#### Proposition 10 {#lie-iii-s7-prop-10 .statement}

Suppose that $p \neq 0$. Let $G$ be a finite-dimensional Lie group. Let $G_f$ be the set of $x \in G$ for which there exists a strictly increasing sequence $(n_i)$ of integers such that $x^{n_i}$ tends to $e$ as $i$ tends to $+\infty$.
(i) $G_f$ is open in $G$.
(ii) There exists one and only one mapping $\psi$ of $G_f$ into $L(G)$ with the following properties:
(a) $\psi(x^n) = n \psi(x)$ for all $x \in G_f$ and all $n \in \mathbf{Z}$;
(b) there exists an open neighbourhood $V$ of $e$ in $G$ such that $\psi|V$ is the inverse mapping of an injective exponential mapping.
(iii) The mapping $\psi$ is analytic.

There exists an open subgroup of $G$ which is isomorphic to a standard group (no. 3, Theorem 4). Assertion (i) then follows from Lemma 1.

Let $U$ be an open subgroup of $L(G)$ and $\phi : U \to \phi(U)$ an exponential mapping of $G$ with the properties of Proposition 3 of no. 2. $U$ can be assumed to be small enough for $\phi(U) \subset G_f$. Let $x \in G_f$. There exists $m \in \mathbf{Z} - \{0\}$ such that $x^m \in \phi(U)$. The element $\frac{1}{m} \phi^{-1}(x^m)$ does not depend on the choice of $m$. For let $m' \in \mathbf{Z}$ be such that $x^{m'} \in \phi(U)$. Then $x^{m m'} \in \phi(U)$ and
$$
m' \phi^{-1}(x^m) = \phi^{-1}(x^{m m'}) = m \phi^{-1}(x^{m'})
$$
whence our assertion. Let $\psi(x) = \frac{1}{m} \phi^{-1}(x^m)$. Then $\psi|\phi(U) = \phi^{-1}$. On the other hand, if $n \in \mathbf{Z}$, then
$$
\psi(x^n) = \frac{1}{m} \phi^{-1}(x^{nm}) = \frac{n}{m} \phi^{-1}(x^m) = n \psi(x).
$$

Hence $\psi$ has properties (a) and (b) of the proposition. In a neighbourhood of $x$, $\psi$ is composed of the mappings $x \mapsto x^m$, $y \mapsto \phi^{-1}(y)$ and $z \mapsto \frac{1}{m} z$; hence $\psi$ is analytic on $G_f$.

Finally, let $\psi'$ be a mapping of $G_f$ into $L(G)$ and $V'$ a neighbourhood of $e$ in $G_f$ such that $\psi'(x^n) = n \psi'(x)$ for $x \in G_f$ and $n \in \mathbf{Z}$ and such that $\psi'|V'$ is the inverse mapping of an injective exponential mapping. Then $\psi$ and $\psi'$ coincide on a neighbourhood $W$ of $e$. If $x \in G_f$, there exists $n \in \mathbf{Z}$ such that $x^n \in W$. Then
$$
n \psi'(x) = \psi'(x^n) = \psi(x^n) = n \psi(x)
$$
and hence $\psi = \psi'$.

#### Definition 2 {#lie-iii-s7-def-2 .statement}

*The mapping $\psi$ of Proposition 10 is called the logarithmic mapping of of $G$ and is denoted by $\log_G$ or simply $\log$.*

#### Proposition 11 {#lie-iii-s7-prop-11 .statement}

*Suppose that $p \neq 0$. Let $x, y$ be two permutable elements of $G_f$. Then $xy \in G_f$ and $\log(xy) = \log x + \log y$.*

The fact that $xy \in G_f$ follows from Lemma 1. Let $U$ be an open subgroup of the additive group $L(G)$ and $\phi : U \to \phi(U)$ an exponential mapping of $G$ with the properties of Proposition 3 of no. 2; $U$ can be assumed to be small enough for $\log|\psi(U)|$ to be the inverse mapping of $\phi$. For $n \in \mathbf{Z} - \{0\}$ suitably chosen, $x^n \in \phi(U)$, $y^n \in \phi(U)$. Let $u = \log x^n$, $v = \log y^n$, whence $x^n = \phi(u)$, $y^n = \phi(v)$. By formula (2), $[u, v] = 0$. The Hausdorff formula proves then that $\phi(\lambda(u + v)) = \phi(\lambda u) \phi(\lambda v)$ for $|\lambda|$ sufficiently small; hence, for every sufficiently large integer $i$,
$$
\phi(p^i(u + v)) = \phi(p^i u) \phi(p^i v)
$$
that is
$$
p^i (\log x^n + \log y^n) = \log(x^{np^i} y^{np^i})
$$
or
$$
np^i (\log x + \log y) = np^i \log(xy).
$$

#### Proposition 12 {#lie-iii-s7-prop-12 .statement}

*Suppose that $p \neq 0$. Let $x \in G_f$. The following conditions are equivalent:
(i) $\log x = 0$;
(ii) $x$ is of finite order in $G$.*

If there exists an integer $n > 0$ such that $x^n = e$, it follows that
$$
n \log x = \log x^n = 0,
$$
whence $\log x = 0$. If $\log x = 0$, let $V$ be a neighbourhood of $e$ in $G_f$ such that $\log|V|$ is the inverse mapping of an injective exponential mapping. There exists an integer $n > 0$ such that $x^n \in V$; the equality $\log x^n = 0$ implies $x^n = e$.

#### Proposition 13 {#lie-iii-s7-prop-13 .statement}

*Suppose that $p \neq 0$. If $G$ is compact or standard, then $G_f = G$.*

If G is standard, it suffices to use Lemma 1. Suppose that G is compact. Let $x \in G$ and V be a neighbourhood of e in G. Let y be a limit point of the sequence $(x^n)_{n \geq 0}$. For all $n > 0$, there exist two integers $n_1, n_2$ such that $n_1 \geq 2n_2 \geq n$ and $x^{n_1} \in yV, x^{n_2} \in yV$, whence $x^{n_1 - n_2} \in V^{-1}V$ and $n_1 - n_2 \geq n$. Hence $x \in G_f$.

#### Corollary {#lie-iii-s7-n6-cor-1 .statement}

*Suppose that K is locally compact. Then $G_f$ is the union of the compact subgroups of G.*

Let $x \in G$. If x belongs to a compact subgroup of G, then $x \in G_f$ (Proposition 13). Suppose that $x \in G_f$. As K is locally compact, there exists an open subgroup $G_1$ of G which is compact. Then there exists an integer $m > 0$ such that $x^m \in G_1$. The closed subgroup $G_2$ generated by $x^m$ is contained in $G_1$ and is therefore compact. Then x commutes with the elements of $G_2$ and hence $G_2 \cup xG_2 \cup \cdots \cup x^{m-1}G_2$ is a compact subgroup of G which contains x.

#### Example {#lie-iii-s7-n6-exa-1 .statement}

Suppose that K is locally compact. Let U be the set of invertible elements of A; it is a compact open subgroup of the Lie group $K^*$. Then $U \subset (K^*)_f$ by Proposition 13; on the other hand, if $x \in K^*$ is such that $x \notin U$, either $x^n$ tends to 0 as n tends to $+\infty$, or $x^n$ tends to 0 as n tends to $-\infty$; hence $U = (K^*)_f$. The function $\log_{K^*}$ is defined and analytic on U, with values in $L(K^*) = K$, and such that $\log_{K^*}(xy) = \log_{K^*}(x) + \log_{K^*}(y)$ for all $x, y$ in U; the elements x of U such that $\log_{K^*}(x) = 0$ are the roots of unity of K.

We again use the notation of nos. 3, 4 and 5.

#### Proposition 14 {#lie-iii-s7-prop-14 .statement}

*Suppose that $p \neq 0$ and that v is chosen such that $v(p) = 1$. Let G be a standard group and E(X) (resp. L(X)) the expansion of the exponential function of G (resp. the logarithmic function of G) as an integral series about 0.*

(i) *The domain of absolute convergence* (Differentiable and Analytic Manifolds, R, 4.1.3) *of E contains the set $\Delta$ of $x \in G$ such that $\omega(x) > \frac{1}{p-1}$. Let $E'$ denote the mapping defined on $\Delta$ by this series. Then $E'$ is an exponential mapping of G and is an isomorphism of the manifold $\Delta$ onto itself.*

(ii) *The domain of absolute convergence of L contains G. Let $L'$ denote the mapping on G defined by this series. Then $L'$ is the logarithmic mapping of G and the restriction of $L'$ to $\Delta$ is the inverse mapping of $E'$.*

(iii) *The mapping $E'$ is an isomorphism of $\Delta$, with the Hausdorff law, onto the subgroup $\Delta$ of G.*

Using the notation of § 5, nos. 3 and 4, $E = \sum_{m \geq 1} \frac{\psi_{m,m}}{m!}$ ($§ 5$, no. 4, Proposition 3). As the coefficients $c_{\alpha \beta \gamma}$ belong to A, $\| \psi_{m,m} \| \leq 1$ (Differentiable and Analytic Manifolds, R, Appendix) $K^r$ is assumed to have the norm

$$
\| (\lambda_1, \ldots, \lambda_r ) \| = \sup(|\lambda_1|, \ldots, |\lambda_r|)
$$

By Chapter II, § 8, no. 1, Lemma 1, $v(m!) \leq \frac{m-1}{p-1}$. If $\omega(x) > \frac{1}{p-1}$, we see that $m \omega(x) - v(m!)$ tends to $+\infty$ with $m$, whence
$$
\left\| \frac{\psi_{m,m}}{m!} \right\| \|x\|^m \leq \frac{1}{|m!|} \|x\|^m
$$
which tends to 0 as $m$ tends to $+\infty$ and
$$
\omega\left( \frac{\psi_{m,m}(x)}{m!} \right) > \frac{m}{p-1} - \frac{m-1}{p-1} = \frac{1}{p-1} \quad \text{for } m \geq 1.
$$
Therefore $\Delta$ is contained in the domain of absolute convergence of $E$ and $E'(\Delta) \subset \Delta$. Clearly $E'$ is an exponential mapping.

If $L_m$ denotes the homogeneous component of $L$ of degree $m$, Proposition 3 of § 5, no. 4, proves that each coefficient of $L_m$ is of the form
$$
a_1 + \frac{1}{2} a_2 + \cdots + \frac{1}{m} a_m
$$
with $a_1, a_2, \ldots, a_m$ in $A$; but
$$
\inf \left( v(1), v\left( \frac{1}{2} \right), \ldots, v\left( \frac{1}{m} \right) \right) = o(\log m) \quad \text{as } m \text{ tends to } +\infty
$$
and
$$
\inf \left( v(1), v\left( \frac{1}{2} \right), \ldots, v\left( \frac{1}{m} \right) \right) \geq v\left( \frac{1}{m!} \right) \geq -\frac{m-1}{p-1}.
$$
Therefore, if $\omega(x) > 0$, $\|L_m\| \cdot \|x\|^m$ tends to 0 as $m$ tends to $+\infty$, so that $G$ is contained in the domain of absolute convergence of $L$. On the other hand, if $\omega(x) > \frac{m}{p-1}$, then $\omega(L_m(x)) > \frac{m}{p-1} - \frac{m-1}{p-1} = \frac{1}{p-1}$ for $m \geq 1$ and hence $L'(\Delta) \subset \Delta$.

As the formal power series $L(E(X))$ and $E(L(X))$ are equal to $X$, no. 4.1.5 of *Differentiable and Analytic Manifolds*, R, proves that
$$
L'(E'(x)) = E'(L'(x)) = x
$$
for $x \in \Delta$. Hence $E'$ is an isomorphism of the manifold $\Delta$ onto itself and the inverse isomorphism is the restriction of $L'$ to $\Delta$.

$L(X^{[n]}) = nL(X)$ for $n$ an integer $> 0$ (cf. § 5, no. 4). As $G$ is contained in the domain of absolute convergence of $L$ and $X^{[n]}$, therefore $L'(x^n) = nL'(x)$ for all $x \in G$. The relation $L'|_{\Delta} = {E'}^{-1}$ implies that $L'(x^n) = \log x^n$ for $n$ sufficiently large. Hence $L'(x) = \log x$. We have thus proved (i) and (ii).

Let $H = \sum_{r,s \geq 0} H_{r,s}$ be the Hausdorff formal power series and $h$ the Hausdorff function relative to $L(G)$. The domain of absolute convergence of $\tilde{H}$ contains $\Delta \times \Delta$ and $h$ is defined on $\Delta \times \Delta$ (Chapter II, § 8, Proposition 2). Then
$$
E'(x)E'(y) = E'(h(x, y))
$$
for $x, y$ sufficiently close to 0 ($§ 4$, Theorem 4 (v)). Hence, in the notation of no. 3, Definition 1, the formal power series $F(E(X), E(Y))$ and $E(H(X, Y))$ are equal. Let $x, y$ be elements of $\Delta$. Then
$$
\sup_m \left| \frac{\psi_{m,m}}{m!} \right| (\sup \|x\|, \|y\|)^m < 1 \\
\sup_{r,s} \|H_{r,s}\| \|x\|^r \|y\|^s < |\rho|^{1/(p-1)}
$$
by Chapter II, § 8, formula (14). By *Differentiable and Analytic Manifolds*, R, 4.1.5, $E'(x)E'(y)$ is obtained by substituting $x$ for $X$ and $y$ for $Y$ in
$$
F(E(X), E(Y))
$$
and $E'(h(x, y))$ is obtained by substituting $x$ for $X$ and $y$ for $Y$ in $E(H(X, Y))$. Hence $E'(x)E'(y) = E'(h(x, y))$.

### Exercises {#lie-iii-s7-exercises}

See the [exercises for § 7](exercises/s7/).
