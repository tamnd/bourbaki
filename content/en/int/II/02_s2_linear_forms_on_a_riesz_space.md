---
book: int
book_title: Integration
chapter: II
chapter_title: RIESZ SPACES
section: 2
section_title: Linear forms on a Riesz space
lang: en
source: int-i-vi
book_pages: INT II.19-INT II.21
pdf_pages: 0033-0039, 0043-0045
extraction: ocr
subsections:
    - "no": 1
      title: Positive linear forms on a Riesz space
      page: 9
      pdf_page: 33
    - "no": 2
      title: Relatively bounded linear forms
      page: 10
      pdf_page: 34
statements: 13
exercises: 9
content_sha256: f261078ae1db1a985db1c8cbda6a7a6f980a9e5c399f533b3b3eabf7b1f185bd
---

## § 2. LINEAR FORMS ON A RIESZ SPACE

### 1. Positive linear forms on a Riesz space

We recall the following definition (TVS, II, §2, No. 5):

#### Definition 1 {#int-ii-s2-def-1 .statement}

Given an ordered vector space E, a linear form L on E is said to be positive if $L(x) \geq 0$ for every $x \geq 0$ in E.

Since $L(y) - L(x) = L(y - x)$, it is the same to say that the relation $x \leq y$ implies $L(x) \leq L(y)$, or again that $L$ is an increasing function on E.

#### Example 1 {#int-ii-s2-n1-exa-1 .statement}

Let A be any set, E a linear subspace of the space $\mathbf{R}^A$ of all real-valued functions defined on A. For every element $a \in A$, the mapping $x \mapsto x(a)$ is a positive linear form on E.

#### Example 2 {#int-ii-s2-n1-exa-2 .statement}

Let $I = [a, b]$ be a compact interval of $\mathbf{R}$, E the Riesz space formed by the regulated real-valued functions on I (FRV, II, §1, No. 3); the mapping $x \mapsto \int_a^b x(t) \, dt$ is a positive linear form on E.

#### Example 3 {#int-ii-s2-n1-exa-3 .statement}

Let F be any set, $\mathcal{U}$ an ultrafilter on F (GT, I, §6, No. 4), E the Riesz space $\mathscr{B}(F)$ of bounded real-valued functions on F. For every $x \in E$, $\lim_{\mathcal{U}} x(t)$ exists, because $x(\mathcal{U})$ is a base of an ultrafilter on the relatively compact set $x(F)$, hence is convergent. Moreover, if $x \geq 0$ then $\lim_{\mathcal{U}} x(t) \geq 0$ by the principle of extension of inequalities; the mapping $x \mapsto \lim_{\mathcal{U}} x$ is thus a positive linear form on E. If $\mathcal{U}$ is taken to be the ultrafilter formed by the sets containing an element $a \in F$, one recovers the positive linear form $x \mapsto x(a)$ (Example 1).

#### Proposition 1 {#int-ii-s2-prop-1 .statement}

Let E be an ordered vector space, L a mapping of E into $\mathbf{R}$ such that $L(x + y) = L(x) + L(y)$ and such that the relation $x \geq 0$ implies $L(x) \geq 0$; then $L(\lambda x) = \lambda L(x)$ for every scalar $\lambda$ and every $x \geq 0$.

Since $L(-x) = -L(x)$ ($L$ being a representation of the additive group E in $\mathbf{R}$), we can restrict ourselves to the case that $\lambda \geq 0$. For every integer $n \geq 0$, we have $L(nx) = nL(x)$, whence $L((1/n)x) = (1/n)L(x)$ and consequently $L(rx) = rL(x)$ for every rational number $r \geq 0$. On the other hand, $L$ is increasing in E; if $r$ and $r'$ are rational numbers such that $r \leq \lambda \leq r'$, it follows that $rL(x) \leq L(\lambda x) \leq r'L(x)$; since $rL(x)$ and $r'L(x)$ differ from $\lambda L(x)$ as little as we like, we have $L(\lambda x) = \lambda L(x)$.

#### Proposition 2 {#int-ii-s2-prop-2 .statement}

Let E be a real vector space, C a convex cone with vertex 0 in E such that $E = C - C$, and $x \mapsto M(x)$ a mapping of C into $\mathbf{R}$ such that $M(\lambda x + \mu y) = \lambda M(x) + \mu M(y)$ for all $x \in C$, $y \in C$, $\lambda \geq 0$, $\mu \geq 0$. Then, there exists one and only one linear form L that extends M to E.

By hypothesis, every $z \in E$ may be written $z = y - x$, where $x, y$ belong to C; moreover, if also $z = y' - x'$ with $x' \in C$, $y' \in C$, then

$M(y) - M(x) = M(y') - M(x')$; for, from the relation $y - x = y' - x'$ we infer $y + x' = x + y'$, consequently $M(y) + M(x') = M(x) + M(y')$. Let us denote by $L(z)$ the common value of $M(y) - M(x)$ for all expressions of $z$ as the difference $y - x$ of two elements of $C$; one verifies immediately that $L$ is a linear form on $E$ extending $M$; the uniqueness of $L$ results from the fact that $C$ generates the space $E$.

#### Proposition 3 {#int-ii-s2-prop-3 .statement}

*Let $E$ be a directed ordered vector space, $P$ the set of elements $\geqslant 0$ of $E$, and $x \mapsto M(x)$ a mapping of $P$ into $\mathbf{R}$, with values $\geqslant 0$, such that $M(x + y) = M(x) + M(y)$ for all $x, y$ in $P$. Then, there exists one and only one positive linear form $L$ that extends $M$ to $E$.*

Since $E = P - P$, the same reasoning as in Prop. 2 proves, first, the existence and uniqueness of an *additive* mapping $L$ of $E$ into $\mathbf{R}$ that extends $M$. Proposition 1 then shows that $L(\lambda x) = \lambda L(x)$ for all $\lambda \geqslant 0$ and all $x \in P$, from which it is immediate that $L$ is a linear form.

### 2. Relatively bounded linear forms

Let $E$ be a directed ordered vector space. Let $Q$ be the set of *positive* linear forms on $E$; it is a subset of the algebraic dual $E^*$ of $E$ (the space of all linear forms on $E$). It is immediate that $Q + Q \subset Q$ and $\lambda Q \subset Q$ for every scalar $\lambda > 0$ (in other words, $Q$ is a *convex cone* in $E^*$). Moreover, $Q \cap (-Q) = \{0\}$, because if $L$ and $-L$ are both positive linear forms, then $L(x) \geqslant 0$ and $L(x) \leqslant 0$ for all $x \geqslant 0$, whence $L(x) = 0$ for all $x \geqslant 0$ and therefore $L = 0$ (No. 1, Prop. 3). The set $Q$ thus defines on $E^*$ an *order relation* $L \leqslant M$, equivalent to « $M - L$ is a positive linear form on $E$ », or again to « for every $x \geqslant 0$, $L(x) \leqslant M(x)$ »; the elements $\geqslant 0$ of $E^*$ for this order structure are the positive linear forms (which justifies the terminology introduced). Let $\Omega$ be the linear subspace of $E^*$ generated by $Q$, that is, the set of linear forms on $E$ that are *differences of two positive linear forms*; we are going to give another characterization of the elements of $\Omega$ when $E$ is a Riesz space.

#### Definition 2 {#int-ii-s2-def-2 .statement}

*Given a Riesz space $E$, a linear form $L$ on $E$ is said to be relatively bounded if, for every $x \geqslant 0$ in $E$, $L$ is bounded on the set of $y \in E$ such that $|y| \leqslant x$.*

#### Theorem 1 {#int-ii-s2-thm-1 .statement}

1° *In order that a linear form $L$ on a Riesz space $E$ be relatively bounded, it is necessary and sufficient that it be the difference of two positive linear forms.*

2° *The ordered vector space $\Omega$ of relatively bounded linear forms on $E$ is a Riesz space that is fully lattice-ordered.*

If $L = U - V$, where $U$ and $V$ are positive linear forms on $E$, the relation $-x \leq y \leq x$ implies

$$
-U(x) \leq U(y) \leq U(x) \quad \text{and} \quad -V(x) \leq V(y) \leq V(x),
$$

whence it is immediate that $|L(y)| \leq U(x) + V(x)$; thus, $L$ is relatively bounded. Suppose, conversely, that $L$ is relatively bounded; it all comes down to proving that there exists a positive linear form $N$ such that $N(x) \geq L(x)$ for all $x \geq 0$, because $N - L$ will then be a positive linear form.

Now, if a positive linear form $N$ has this property then, for every $x \geq 0$ and for $0 \leq y \leq x$, we have $N(x) \geq N(y) \geq L(y)$, therefore $N(x) \geq \sup_{0 \leq y \leq x} L(y)$; if we prove that the real-valued function

$$
x \mapsto M(x) = \sup_{0 \leq y \leq x} L(y),
$$

defined on the set $P$ of elements $\geq 0$ of $E$, may be extended to a positive linear form on $E$ (to be denoted $M$ as well), we will have demonstrated the first part of the theorem and will have proved, moreover, that $M$ is the supremum of $0$ and $L$ in $\Omega$. Since $M(x) \geq 0$ on $P$, it all comes down to proving that

$$
M(x + x') = M(x) + M(x')
$$

for every pair of elements $x \geq 0,\ x' \geq 0$ of $E$ (No. 1, Prop. 3). By definition,

$$
M(x) + M(x') = \sup_{0 \leq y \leq x} L(y) + \sup_{0 \leq y' \leq x'} L(y')
= \sup_{0 \leq y \leq x,\ 0 \leq y' \leq x'} L(y + y') \leq M(x + x').
$$

On the other hand, for every $z$ such that $0 \leq z \leq x + x'$, we have $x + x' = z + u$ with $u \geq 0$; by the decomposition lemma (§ 1, No. 1), there exist two elements $y,\ y'$ such that $0 \leq y \leq x,\ 0 \leq y' \leq x'$ and such that $z = y + y',\ u = (x - y) + (x' - y')$; then

$$
L(z) = L(y) + L(y') \leq M(x) + M(x'),
$$

therefore $M(x + x') = \sup_{0 \leq z \leq x + x'} L(z) \leq M(x) + M(x')$, which completes the proof of the first part of the theorem. Moreover, we have thus shown that $\Omega$ is a *Riesz space* and that, for every relatively bounded linear form $L$ on $E$ and for every $x \geq 0$,

(1)
$$
L^+(x) = \sup_{0 \leq y \leq x} L(y).
$$

It remains to see that $\Omega$ is fully lattice-ordered; for this, it suffices to show that any set $H$ of *positive* linear forms, bounded above and directed for the relation $\leqslant$, has a supremum in $\Omega$.

More generally, we have the following lemma:

#### Lemma {#int-ii-s2-n2-lem-1 .statement}

— *Let E be a directed ordered vector space, $E^*$ its dual, ordered by taking as positive elements the positive linear forms. Let $(u_\alpha)$ be an increasing directed family of elements of $E^*$. If, for every $x \geqslant 0$ in E, $\sup u_\alpha(x) < +\infty$, then the family $(u_\alpha)$ has a supremum $u$ in $E^*$ and, for all $x \geqslant 0$ in E,

$$
u(x) = \sup_{\alpha} u_\alpha(x).
$$

In the set P of all $x \geqslant 0$ in E, define the mapping $u$ by the formula (2); it is immediate that $u(\lambda x) = \lambda u(x)$ for all $\lambda \geqslant 0$ and $x \in P$; to prove the lemma it therefore suffices, by Prop. 2 of No. 1, to show that

$$
u(x + y) = u(x) + u(y)
$$

for $x, y$ in P. But this is immediate on observing that $u(x) = \lim u_\alpha(x)$ with respect to the directed set of indices (monotone limit theorem).

From the formula (1), one deduces immediately that if $L$ and $M$ are two relatively bounded linear forms on E then, for every $x \geqslant 0$,

$$
\begin{cases}
\sup(L, M)(x) = \sup_{y \geqslant 0,\ z \geqslant 0,\ y+z=x} (L(y) + M(z)) \\
\inf(L, M)(x) = \inf_{y \geqslant 0,\ z \geqslant 0,\ y+z=x} (L(y) + M(z)).
\end{cases}
$$

In particular if, in the first of these formulas, $M$ is replaced by $-L$, we get

$$
|L|(x) = \sup_{y \geqslant 0,\ z \geqslant 0,\ y+z=x} L(y - z).
$$

Now, if $x = y + z$, $y \geqslant 0$ and $z \geqslant 0$, then $-x \leqslant y - z \leqslant x$; conversely, the relation $|u| \leqslant x$ implies $L(u) \leqslant |L|(|u|) \leqslant |L|(x)$. From this we deduce the formula

$$
|L|(x) = \sup_{|y| \leqslant x} L(y) \quad \text{for } x \geqslant 0,
$$

whence, in particular,

$$
|L(x)| \leqslant |L|(|x|)
$$

for all $x \in E$.

#### Proposition 4 {#int-ii-s2-prop-4 .statement}

— In order that two positive linear forms $L, M$ on a Riesz space $E$ be alien to each other in the space $\Omega$, it is necessary and sufficient that, for every number $\varepsilon > 0$ and every $x \geq 0$ in $E$, there exist two elements $y \geq 0, z \geq 0$ of $E$ such that $x = y + z$ and $L(y) + M(z) \leq \varepsilon$.

Indeed, by the second formula of (3), this condition expresses that $\inf(L, M) = 0$.

#### Proposition 5 {#int-ii-s2-prop-5 .statement}

— Let $L$ be a positive linear form on a Riesz space $E$. In order that a positive linear form $M$ on $E$ belong to the band generated by $L$ in $\Omega$, it is necessary and sufficient that, for every $x \geq 0$ in $E$ and every number $\varepsilon > 0$, there exist a number $\delta > 0$ such that the relations $0 \leq y \leq x$ and $L(y) \leq \delta$ imply $M(y) \leq \varepsilon$.

Let us first show that the condition is necessary. If $M \geq 0$ belongs to the band generated by $L$ in $\Omega$, then (§ 1, No. 5, Cor. of Prop. 6)

$$
M = \sup_n \left( \inf(nL, M) \right).
$$

If one sets

$$
U_n = M - \inf(nL, M),
$$

$U_n$ is thus a positive linear form on $E$ and $\inf_n U_n = 0$ in $\Omega$; consequently (Lemma) $U_n(x)$ tends to 0 as $n$ tends to infinity, and there exists an $n$ such that $U_n(x) \leq \varepsilon/2$. Fixing such an $n$, we have $U_n(y) \leq \varepsilon/2$ for all $y$ such that $0 \leq y \leq x$, thus the relation $0 \leq y \leq x$ implies

$$
M(y) \leq \frac{\varepsilon}{2} + \inf(nL, M)(y) \leq \frac{\varepsilon}{2} + nL(y);
$$

if $y$ is such that $L(y) \leq \varepsilon/2n$ it follows that $M(y) \leq \varepsilon$, which establishes our assertion.

Let us now show that the condition is sufficient. For every positive linear form $M$ on $E$, one can write $M = U + V$, where $U$ belongs to the band generated by $L$ in $\Omega$ and where $V$ is alien to $L$, $U$ and $V$ being positive (§ 1, No. 5, Th. 1). If $M$ satisfies the condition of the statement then so does $V = M - U$, since $0 \leq V \leq M$. From this we will deduce that $V = 0$. For every $x \geq 0$ in $E$ and every number $\eta > 0$, there exist two elements $y \geq 0, z \geq 0$ of $E$ such that $x = y + z$ and $L(y) + V(z) \leq \eta$ (Prop. 4); given an arbitrary number $\varepsilon > 0$, choose $\eta \leq \varepsilon$ so that the relations $0 \leq u \leq x$ and $L(u) \leq \eta$ imply $V(u) \leq \varepsilon$; with $y$ and $z$ then determined as above, we have $L(y) \leq \eta$, therefore $V(y) \leq \varepsilon$ and so

$$
V(x) = V(y) + V(z) \leq \varepsilon + \eta \leq 2\varepsilon;
$$

since $\varepsilon$ is arbitrary, we have $V(x) = 0$ for every $x \geq 0$, that is, $V = 0$.

#### Example {#int-ii-s2-n2-exa-1 .statement}

Let E be a Riesz space equipped with a locally convex topology compatible with its ordered vector space structure (TVS, II, §2, No. 7). Let E' be the topological dual of E, and suppose in addition that the cone P of elements $\geqslant 0$ of E is *complete for the weakened topology* $\sigma(E, E')$. Then every continuous linear form $x' \in E'$ is *relatively bounded*, for one knows (TVS, II, §6, No. 8, Cor. 2 of Prop. 11) that under these conditions, for every $x \geqslant 0$ in E the set of $y \in E$ such that $|y| \leqslant x$ is *compact* for $\sigma(E, E')$. From this we deduce that E is then *fully lattice-ordered*; for ($§ 1$, No. 3, Prop. 2), it suffices to show that for every set $H \subset E$ that is bounded above and directed for $\leqslant$, the section filter $\mathcal{F}$ of H is *convergent in E for the topology* $\sigma(E, E')$ (the latter being compatible with the ordered vector space structure of E). By translation, we can suppose that $H \subset P$, and it then suffices to show that $\mathcal{F}$ is a *Cauchy filter* for $\sigma(E, E')$, or again that every continuous linear form $x' \in E'$ has a limit with respect to $\mathcal{F}$. But this follows at once from the monotone limit theorem when $x'$ is a *positive* linear form, and since every linear form $x' \in E'$ is the difference of two positive linear forms (Th. 1) our assertion is proved.

Exercises

### Exercises {#int-ii-s2-exercises}

See the [exercises for § 2](exercises/s2/).
