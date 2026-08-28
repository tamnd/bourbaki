---
book: int
book_title: Integration
chapter: VII
chapter_title: HAAR MEASURE
section: 1
section_title: Construction of a Haar measure
lang: en
source: int-vii-ix
pdf_pages: 0007-0032, 0084-0093
extraction: ocr
subsections:
    - "no": 1
      title: Definitions and notations
      page: 0
      pdf_page: 7
    - "no": 2
      title: The existence and uniqueness theorem
      page: 6
      pdf_page: 12
    - "no": 3
      title: Modulus
      page: 10
      pdf_page: 16
    - "no": 4
      title: Modulus of an automorphism
      page: 13
      pdf_page: 19
    - "no": 5
      title: Haar measure of a product
      page: 14
      pdf_page: 20
    - "no": 6
      title: Haar measure of an inverse limit*
      page: 15
      pdf_page: 21
    - "no": 7
      title: Local definition of a Haar measure
      page: 18
      pdf_page: 24
    - "no": 8
      title: Relatively invariant measures
      page: 19
      pdf_page: 25
    - "no": 9
      title: Quasi-invariant measures
      page: 20
      pdf_page: 26
    - "no": 10
      title: Locally compact fields
      page: 21
      pdf_page: 27
    - "no": 11
      title: Finite-dimensional algebras over a locally compact field
      page: 25
      pdf_page: 31
statements: 42
exercises: 23
content_sha256: 419ab91b51b52ce173f1a3d494e9786a6b3f625f788e1e4f59833324cd27ed0e
---

## § 1. CONSTRUCTION OF A HAAR MEASURE

### 1. Definitions and notations

Let G be a topological group operating continuously on the left (GT, III, §2, No. 4) in a locally compact space X; for $s \in G$ and $x \in X$, let $sx$ be the transform of $x$ by $s$. We denote by $\gamma_X(s)$, or $\gamma(s)$, the homeomorphism of X onto X defined by

(1)
$$
\gamma(s)x = sx.
$$

We have

(2)
$$
\gamma(st) = \gamma(s)\gamma(t).
$$

If $f$ is a function defined on $X$, $\gamma(s)f$ will be defined by transport of structure, that is, by the formula $(\gamma(s)f)(\gamma(s)x) = f(x)$; in other words,

(3)
$$
(\gamma(s)f)(x) = f(s^{-1}x).
$$

If $\mu$ is a measure defined on $X$, $\gamma(s)\mu$ will also be defined by transport of structure, which leads to

(4)
$$
\langle f, \gamma(s)\mu \rangle = \langle \gamma(s^{-1})f, \mu \rangle \quad \text{for } f \in \mathcal{K}(X).
$$

In other words,

(5)
$$
\int_X f(x) d(\gamma(s)\mu)(x) = \int_X f(sx) d\mu(x).
$$

If $A$ is a $(\gamma(s)\mu)$-integrable set, then $s^{-1}A$ is $\mu$-integrable and

(6)
$$
(\gamma(s)\mu)(A) = \mu(s^{-1}A).
$$

The measure $\gamma(s)\mu$ may also be defined as the *image* of $\mu$ under $\gamma(s)$.

Instead of writing $d(\gamma(s)\mu)(x)$, it is sometimes useful to write $d\mu(s^{-1}x)$; the formula (5) then takes the following form:

$$
\int_X f(x) d\mu(s^{-1}x) = \int_X f(sx) d\mu(x);
$$

the expression on the right may then be deduced from that on the left by 'replacing $x$ by $sx$.'

#### Definition 1 {#int-vii-s1-def-1 .statement}

*Let $\mu$ be a measure on $X$.*
a) $\mu$ *is said to be invariant under $G$* if $\gamma(s)\mu = \mu$ *for every* $s \in G$.
b) $\mu$ *is said to be relatively invariant under $G$* if $\gamma(s)\mu$ *is proportional to* $\mu$ *for every* $s \in G$.
c) $\mu$ *is said to be quasi-invariant under $G$* if $\gamma(s)\mu$ *is equivalent to* $\mu$ *for every* $s \in G$.

#### Remark {#int-vii-s1-n1-rem-1 .statement}

— 1) Assume $\mu$ invariant. Then $|\mu|$, $\mathcal{R}(\mu)$, $\mathcal{I}(\mu)$ are invariant. If $\mu$ is real, then $\mu^+$ and $\mu^-$ are invariant.
2) Assume $\mu$ relatively invariant and nonzero. There exists, for every $s \in G$, a unique complex number $\chi(s)$ such that

(7)
$$
\gamma(s)\mu = \chi(s)^{-1}\mu,
$$

and the function $\chi$ on $G$ is a representation of $G$ in $\mathbf{C}^*$, called the *multiplier* of $\mu$. The formula (5) then gives

$$
(8) \quad \int_X f(sx)\, d\mu(x) = \chi(s)^{-1} \int_X f(x)\, d\mu(x),
$$

and formula (6) gives

$$
(9) \quad \mu(sA) = \chi(s) \mu(A).
$$

With the conventions made above, (7) may also be written

$$
(10) \quad d\mu(sx) = \chi(s)\, d\mu(x).
$$

3) Since $|\gamma(s)\mu| = \gamma(s)(|\mu|)$, to say that $\mu$ is quasi-invariant amounts to saying that $|\mu|$ is quasi-invariant.

If $\mu$ is quasi-invariant and $\mu'$ is another measure on $X$ equivalent to $\mu$, then $\gamma(s)\mu'$ is equivalent to $\gamma(s)\mu$, hence to $\mu$, hence to $\mu'$, and so $\mu'$ is quasi-invariant. To say that $\mu$ is quasi-invariant under $G$ therefore means that the *class* of $\mu$ is invariant under $G$.

For $\mu$ to be quasi-invariant, it is necessary and sufficient that the set of locally $\mu$-negligible subsets of $X$ be invariant under $G$ (Ch. V, §5, No. 5, Th. 2), or again that, for every $\mu$-negligible compact subset $K$ of $X$ and for every $s \in G$, $sK$ be $\mu$-negligible (*loc. cit.*, *Remark*).

If $\mu$ is quasi-invariant, then the support of $\mu$ is invariant under $G$. In particular if $G$ is *transitive* in $X$ (A, I, §5, No. 5, Def. 6), this support is either empty (if $\mu = 0$) or equal to $X$ (if $\mu \neq 0$).

#### Lemma 1 {#int-vii-s1-lem-1 .statement}

— *Let $X, Y, Z$ be three topological spaces, with $Y$ locally compact. Let $(x, y) \mapsto xy$ be a continuous mapping of $X \times Y$ into $Z$, which defines a mapping $x \mapsto u_x$ of $X$ into $\mathcal{F}(Y; Z)$ by the relation $u_x(y) = xy$. Let $f$ be a continuous function on $Z$ with values in $\mathbf{R}$ or in a Banach space, S the support of $f$, and $\mu$ a measure on $Y$. Assume that for every $x_0 \in X$, there exists a neighborhood $V$ of $x_0$ in $X$ such that $\bigcup_{x \in V} u_x^{-1}(S)$ is relatively compact in $Y$. Then:
a) for every $x \in X$, $f \circ u_x$ is continuous on $Y$, with compact support;
b) the mapping $x \mapsto \int_Y f(xy)\, d\mu(y)$, which is defined by a), is continuous on $X$.

The assertion a) is obvious. Let us prove b). Since continuity is a local property, we may reduce to the case that $\bigcup_{x \in X} u_x^{-1}(S)$ is contained in a compact subset $Y'$ of $Y$. Since the function $(x, y) \mapsto f(xy)$ is continuous on $X \times Y$, $f \circ u_x$ tends to $f \circ u_{x_0}$ uniformly on $Y'$ as $x$ tends to $x_0$

(GT, X, §3, No. 4, Th. 3), therefore $\mu(f \circ u_x)$ tends to $\mu(f \circ u_{x_0})$. Whence the lemma.

Let us now return to the previous notations.

#### Proposition 1 {#int-vii-s1-prop-1 .statement}

— *Assume that G is locally compact. Let $\mu$ be a nonzero relatively invariant measure on X. Then its multiplier $\chi$ is a continuous function on G.*

For, let $f \in \mathcal{K}(X)$, S the support of $f$, $s_0$ a point of G, and V a compact neighborhood of $s_0$ in G; then, the set

$$
\bigcup_{s \in V} \gamma(s)^{-1}(S) = V^{-1}S
$$

is compact in X; by Lemma 1 and formula (8), $\chi(s^{-1}) \langle \mu, f \rangle$ depends continuously on $s$; if $f$ is chosen so that $\langle \mu, f \rangle \neq 0$, one sees that $\chi$ is continuous.

Now let G be a topological group operating continuously on the right in a locally compact space X; for $s \in G$ and $x \in X$, let $xs$ be the transform of $x$ by $s$. We denote by $\delta_X(s)$, or $\delta(s)$, the homeomorphism of X defined by

(1')
$$
\delta(s)x = xs^{-1}.
$$

We have

(2')
$$
\delta(st) = \delta(s)\delta(t).
$$

By transport of structure, one defines the action of $\delta(s)$ on functions and measures on X:

(3')
$$
(\delta(s)f)(x) = f(xs)
$$
(4')
$$
\langle f, \delta(s)\mu \rangle = \langle \delta(s^{-1})f, \mu \rangle
$$
(5')
$$
\int_X f(x) d(\delta(s)\mu)(x) = \int_X f(xs^{-1}) d\mu(x)
$$
(6')
$$
(\delta(s)\mu)(A) = \mu(As).
$$

We agree to write $d\mu(xs)$ in place of $d(\delta(s)\mu)(x)$, and (5') then takes the form

$$
\int_X f(x) d\mu(xs) = \int_X f(xs^{-1}) d\mu(x).
$$

One defines in an analogous manner the measures on X invariant, relatively invariant and quasi-invariant under G. If $\mu$ is relatively invariant, its multiplier $\chi$ is defined by the formulas

$$
(7') \quad \delta(s)\mu = \chi(s)\mu
$$
$$
(8') \quad \int_X f(xs)\,d\mu(x) = \chi(s)^{-1} \int_X f(x)\,d\mu(x)
$$
$$
(9') \quad \mu(As) = \chi(s)\mu(A)
$$
$$
(10') \quad d\mu(xs) = \chi(s)\,d\mu(x).
$$

If one regards the group $G^0$ opposite to G as operating in X by $(x,s) \mapsto xs$, then $\mu$ is relatively invariant under $G^0$ with the same multiplier $\chi$.

Finally, let G be a locally compact group. It operates on itself by left and right translations, according to the formulas $\gamma(s)x = sx$, $\delta(s)x = xs^{-1}$. Then

$$
(11) \quad \gamma(s)\delta(t) = \delta(t)\gamma(s).
$$

All of the foregoing is applicable here, thus we have on G the concepts of measures that are *left-invariant*, *right-invariant*, *relatively left-invariant*, *relatively right-invariant*, *left quasi-invariant*, *right quasi-invariant* (however, see Nos. 8 and 9).

The mapping $x \mapsto x^{-1}$ is a homeomorphism of G onto G. For every function $f$ on G, we define the function $\check{f}$ on G by

$$
(12) \quad \check{f}(x) = f(x^{-1}).
$$

For every measure $\mu$ on G, we define the measure $\check{\mu}$ by

$$
(13) \quad \check{\mu}(f) = \mu(\check{f}) \quad \text{for } f \in \mathcal{K}(G).
$$

In other words,

$$
(14) \quad \int_G f(x)\,d\check{\mu}(x) = \int_G f(x^{-1})\,d\mu(x).
$$

If A is a $\check{\mu}$-integrable set, then $A^{-1}$ is $\mu$-integrable and

$$
(15) \quad \check{\mu}(A) = \mu(A^{-1}).
$$

We agree to write $d\mu(x^{-1})$ in place of $d\check{\mu}(x)$, and (14) then takes the form

$$
\int_G f(x)\, d\mu(x^{-1}) = \int_G f(x^{-1})\, d\mu(x).
$$

### 2. The existence and uniqueness theorem

#### Definition 2 {#int-vii-s1-def-2 .statement}

*Let G be a locally compact group. A nonzero positive measure on G that is left (resp. right) invariant is called a left (resp. right) Haar measure on G.*

#### Theorem 1 {#int-vii-s1-thm-1 .statement}

*On every locally compact group, there exists a left (resp. right) Haar measure, and, up to a constant factor, there exists only one.*

A) *Existence.* — Set $\mathcal{K}(G) = \mathcal{K}$, $\mathcal{K}_+(G) = \mathcal{K}_+$, $\mathcal{K}_+^* = \mathcal{K}_+ - \{0\}$. If C is a compact subset of G, we denote by $\mathcal{K}_+^*(C)$ the set of $f \in \mathcal{K}_+^*$ with support in C. For $f \in \mathcal{K}$ and $g \in \mathcal{K}_+^*$, there exist numbers $c_1, \ldots, c_n \geq 0$ and elements $s_1, \ldots, s_n$ of G such that $f \leq \sum_{i=1}^n c_i \gamma(s_i)g$: for, there exists a nonempty open set U in G such that $\inf_{s \in U} g(s) > 0$, and the support of $f$ can be covered by a finite number of left-translates of U. Let $(f : g)$ be the infimum of the numbers $\sum_{i=1}^n c_i$ for all systems $(c_1, \ldots, c_n, s_1, \ldots, s_n)$ of numbers $\geq 0$ and elements of G such that $f \leq \sum_{i=1}^n c_i \gamma(s_i)g$. Then:

(i) $(\gamma(s)f : g) = (f : g)$ for $f \in \mathcal{K}$, $g \in \mathcal{K}_+^*$, $s \in G$;
(ii) $(\lambda f : g) = \lambda(f : g)$ for $f \in \mathcal{K}$, $g \in \mathcal{K}_+^*$, $\lambda \geq 0$;
(iii) $((f + f') : g) \leq (f : g) + (f' : g)$ for $f \in \mathcal{K}$, $f' \in \mathcal{K}$, $g \in \mathcal{K}_+^*$;
(iv) $(f : g) \geq (\sup f)/(\sup g)$ for $f \in \mathcal{K}$, $g \in \mathcal{K}_+^*$;
(v) $(f : h) \leq (f : g)(g : h)$ for $f \in \mathcal{K}$, $g \in \mathcal{K}_+^*$, $h \in \mathcal{K}_+^*$;
(vi) $0 < \frac{1}{(f_0 : f)} \leq \frac{(f : g)}{(f_0 : g)} \leq (f : f_0)$ for $f, f_0, g$ in $\mathcal{K}_+^*$;
(vii) let $f, f', h$ be in $\mathcal{K}_+$ with $h(s) \geq 1$ on the support of $f + f'$, and let $\varepsilon > 0$; there exists a compact neighborhood V of e such that, for every $g \in \mathcal{K}_+^*(V)$,

$$
(f : g) + (f' : g) \leq ((f + f') : g) + \varepsilon(h : g).
$$

The properties (i), (ii), (iii) are obvious. Let $f \in \mathcal{K}$, $g \in \mathcal{K}_+^*$; if $f \leq \sum_{i=1}^n c_i \gamma(s_i)g$ with the $c_i \geq 0$, then $\sup f \leq \sum_{i=1}^n c_i g(s_i^{-1}s)$ for some s \in G, therefore $\sup f \leq (\sum_{i=1}^n c_i) \sup g$, whence (iv). Let us now prove (v); let $f \in \mathcal{K}$, $g, h$ in $\mathcal{K}_+^*$; if $f \leq \sum_{i=1}^n c_i \gamma(s_i)g$ and $g \leq \sum_{j=1}^p d_j \gamma(t_j)h$ ($c_i \geq 0, d_j \geq 0, s_i, t_j$ in $G$), then $f \leq \sum_{i,j} c_i d_j \gamma(s_i t_j)h$, therefore $(f : h) \leq \sum_{i,j} c_i d_j = (\sum_i c_i)(\sum_j d_j)$; thus $(f : h) \leq (f : g)(g : h)$. Applying (v) to $f_0, f, g$ on the one hand and to $f, f_0, g$ on the other, one obtains (vi). Finally, let $f, f', h$ be in $\mathcal{K}_+$ with $h(s) \geq 1$ on the support of $f + f'$, and let $\varepsilon > 0$. Set $F = f + f' + \frac{1}{2} \varepsilon h$; the functions $\varphi, \varphi'$, that coincide respectively with $f/F$ and $f'/F$ on the support of $f + f'$ and are zero outside it, belong to $\mathcal{K}_+$; for every $\eta > 0$, there exists a compact neighborhood $V$ of $e$ such that $|\varphi(s) - \varphi(t)| \leq \eta$ and $|\varphi'(s) - \varphi'(t)| \leq \eta$ for $s^{-1} t \in V$. Then let $g \in \mathcal{K}_+^*(V)$; for every $s \in G$,

$$
\varphi \cdot \gamma(s)g \leq (\varphi(s) + \eta) \cdot \gamma(s)g;
$$

for, this is obvious at the points where $\gamma(s)g$ is zero, therefore outside of $sV$; and in $sV$, $\varphi \leq \varphi(s) + \eta$; similarly, $\varphi' \cdot \gamma(s)g \leq (\varphi'(s) + \eta) \cdot \gamma(s)g$. This stated, let $c_1, \ldots, c_n$ be numbers $\geq 0$ and $s_1, \ldots, s_n$ elements of $G$ such that $F \leq \sum_{i=1}^n c_i \gamma(s_i)g$; then

$$
f = \varphi F \leq \sum_{i=1}^n c_i \varphi \cdot \gamma(s_i)g \leq \sum_{i=1}^n c_i (\varphi(s_i) + \eta) \cdot \gamma(s_i)g
$$

and similarly for $f'$; consequently

$$
(f : g) + (f' : g) \leq \sum_{i=1}^n c_i (\varphi(s_i) + \varphi'(s_i) + 2\eta) \leq (1 + 2\eta) \sum_{i=1}^n c_i
$$

since $\varphi + \varphi' \leq 1$. Applying the definition of $F$, then (ii), (iii) and (v), one infers that

$$
(f : g) + (f' : g) \leq (1 + 2\eta)(F : g) \leq
$$
$$
(1 + 2\eta)[((f + f') : g) + \frac{1}{2}\varepsilon(h : g)] \leq
$$
$$
(((f + f') : g) + \frac{1}{2}\varepsilon(h : g) + 2\eta((f + f') : h)(h : g) + \varepsilon\eta(h : g)
$$

and, if $\eta$ has been chosen so that $\eta[2((f + f') : h) + \varepsilon] \leq \frac{1}{2}\varepsilon$, one obtains (vii).

As V runs over the set of compact neighborhoods of e, the $\mathcal{K}_+^*(V)$ form a base of a filter $\mathcal{B}$ on $\mathcal{K}_+^*$. Let $\mathcal{F}$ be an ultrafilter on $\mathcal{K}_+^*$ finer than $\mathcal{B}$. On the other hand, let us fix $f_0 \in \mathcal{K}_+^*$ and let us set, for $f \in \mathcal{K}_+^*$ and $g \in \mathcal{K}_+^*$,

$$
I_g(f) = \frac{(f : g)}{(f_0 : g)}.
$$

By (vi), $\lim_{g,\mathcal{F}} I_g(f) = I(f)$ exists in the compact space $[1/(f_0 : f), (f : f_0)]$.

By (iii), $I(f + f') \leq I(f) + I(f')$. By (vii), $I(f) + I(f') \leq I(f + f') + \varepsilon I(h)$ for all $\varepsilon > 0$ provided $h$ is $\geq 1$ on the support of $f + f'$; it follows that $I(f + f') = I(f) + I(f')$. By Ch. II, §2, No. 1, Prop. 2, I is extendible to a linear form on $\mathcal{K}$; this linear form is a nonzero positive measure on G, left-invariant by (i); this is the sought-for left Haar measure. Passing to the opposite group, one deduces from this the existence of a right Haar measure.

B) *Uniqueness.* — Let $\mu$ be a left Haar measure, $\nu$ a right Haar measure. Then $\check{\nu}$ is a left Haar measure. We are going to show that $\mu$ and $\check{\nu}$ are proportional. This will prove that any two left Haar measures are indeed proportional.

Let $f \in \mathcal{K}$ be such that $\mu(f) \neq 0$. By Lemma 1, the function $D_f$ defined on G by the formula

$$
D_f(s) = \mu(f)^{-1} \int f(t^{-1}s) d\nu(t)
$$

is continuous on G. Let $g \in \mathcal{K}$. The function $(s, t) \mapsto f(s)g(ts)$ is continuous with compact support in $G \times G$. By Ch. III, §4, No. 1, Th. 2,

$$
\begin{align*}
\mu(f)\nu(g) &= \left( \int f(s) d\mu(s) \right) \left( \int g(t) d\nu(t) \right) \\
&= \int d\mu(s) \int f(s)g(ts) d\nu(t) = \int d\nu(t) \int f(s)g(ts) d\mu(s) \\
&= \int d\nu(t) \int f(t^{-1}s)g(s) d\mu(s) \\
&= \int g(s) \left[ \int f(t^{-1}s) d\nu(t) \right] d\mu(s) = \mu(g \cdot \mu(f) D_f),
\end{align*}
$$

whence

$$
\nu(g) = \mu(D_f \cdot g).
$$

This proves, first, that $D_f$ does not depend on $f$. For, if $f' \in \mathcal{K}$ is such that $\mu(f') \neq 0$, then $D_f \cdot \mu = D_{f'} \cdot \mu$, therefore $D_f = D_{f'}$ locally almost everywhere for $\mu$, hence everywhere, since $D_f$ and $D_{f'}$ are continuous and the support of $\mu$ is $G$. We may therefore write $D_f = D$. The formula (16) gives

$$
\mu(f)D(e) = \check{\nu}(f).
$$

The formula (19) may be extended by linearity to the functions $f \in \mathcal{K}$ such that $\mu(f) = 0$. We have $D(e) \neq 0$ since $\check{\nu} \neq 0$. This indeed establishes the proportionality of $\mu$ and $\check{\nu}$.

#### Corollary {#int-vii-s1-n2-cor-1 .statement}

— *Every left-invariant* (resp. *right-invariant*) *measure on* $G$ *is proportional to a left* (resp. *right*) *Haar measure*.

#### Example {#int-vii-s1-n2-exa-1 .statement}

— 1) On the additive group $\mathbf{R}$, the Lebesgue measure $dx$ is a Haar measure (Ch. III, §1, No. 3, *Example*).

2) For every function $f \in \mathcal{K}(\mathbf{R}_+^*)$, we have (FRV, II, §1, formula (12))

$$
\int_0^{+\infty} \frac{f(x)}{x} dx = \int_0^{+\infty} \frac{f(tx)}{tx} t dx = \int_0^{+\infty} \frac{f(tx)}{x} dx
$$

for all $t > 0$; the measure $x^{-1} dx$ is thus a Haar measure on the multiplicative group $\mathbf{R}_+^*$.

3) Let us take for $G$ the torus $T = \mathbf{R}/\mathbf{Z}$. Let $\varphi$ be the canonical mapping of $\mathbf{R}$ onto $T$. For $f \in \mathcal{K}(T)$, the function $f \circ \varphi$ is continuous and periodic with period 1 on $\mathbf{R}$, and the integral

$$
I(f) = \int_a^{a+1} f(\varphi(x)) dx
$$

is independent of the choice of $a \in \mathbf{R}$; it is immediate that it is invariant under translation; it therefore defines a Haar measure on $T$. By transport of structure, one deduces from this that $I(f) = \int_a^{a+1} f(e^{2\pi i t}) dt$ is a Haar measure on the multiplicative group $U$ of complex numbers of absolute value 1 (GT, VIII, §2, No. 1).

#### Proposition 2 {#int-vii-s1-prop-2 .statement}

— *Let* $G$ *be a locally compact group*, $\mu$ *a left or right Haar measure on* $G$. *For* $G$ *to be discrete, it is necessary and sufficient that* $\mu(\{e\}) > 0$. *For* $G$ *to be compact, it is necessary and sufficient that* $\mu^*(G) < +\infty$.

The conditions are obviously necessary. Let us show their sufficiency. Let $V$ be a compact neighborhood of $e$. If $\mu(\{e\}) > 0$, then $V$ is a finite set since $\mu(V) < +\infty$; since $G$ is Hausdorff, it is therefore discrete. Suppose $\mu^*(G) < +\infty$ and $\mu$ is, for example, left-invariant. Consider the set $\mathcal{E}$ of finite subsets $\{s_1, \ldots, s_n\}$ of $G$ such that $s_i V \cap s_j V = \varnothing$ for $i \neq j$; then

$$
n \mu(V) = \mu(s_1 V \cup \ldots \cup s_n V) \leq \mu^*(G),
$$

therefore $n \leq \mu^*(G)/\mu(V)$. We may therefore choose in $\mathcal{E}$ a maximal element $\{s_1, \ldots, s_n\}$. Then, for every $s \in G$, there exists an $i$ such that $s V \cap s_i V \neq \varnothing$, hence such that $s \in s_i V V^{-1}$. Thus $G$ is the union of the compact sets $s_i V V^{-1}$, hence is compact.

### 3. Modulus

Let $\mu$ be a left Haar measure on $G$. For every $s \in G$, $\delta(s)\mu$ is also left-invariant (No. 1, formula (11)), therefore (Th. 1) there exists a unique number $\Delta_G(s) > 0$ such that $\delta(s)\mu = \Delta_G(s)\mu$. By virtue of Th. 1, the number $\Delta_G(s)$ is independent of the choice of $\mu$.

#### Definition 3 {#int-vii-s1-def-3 .statement}

*The function $\Delta_G$ on $G$ is called the modulus (or modular function) of $G$. If $\Delta_G = 1$, the group $G$ is said to be unimodular.*

One can also say that $\mu$ is relatively right-invariant with multiplier $\Delta_G$. Thus $\Delta_G$ is a *continuous representation of $G$ in $\mathbf{R}_+^*$* (No. 1, Prop. 1).

#### Remark {#int-vii-s1-n3-rem-1 .statement}

— If $\varphi$ is an isomorphism of $G$ onto a locally compact group $G'$, then $\Delta_{G'} \circ \varphi = \Delta_G$. In particular:
1) Since $x \mapsto x^{-1}$ is an isomorphism of $G$ onto the opposite group $G^0$, one has $\Delta_{G^0} = \Delta_G^{-1}$.
2) If $\varphi$ is an automorphism of $G$, then $\Delta_G \circ \varphi = \Delta_G$.

Let $s \in G$. Then:

$$
\delta(s)(\Delta_G^{-1} \cdot \mu) = (\delta(s)\Delta_G^{-1}) \cdot (\delta(s)\mu) = (\Delta_G(s)^{-1}\Delta_G^{-1}) \cdot (\Delta_G(s)\mu) = \Delta_G^{-1} \cdot \mu,
$$

therefore $\Delta_G^{-1} \cdot \mu = \mu'$ is a right Haar measure. From this, one deduces that $\gamma(s)\mu' = (\gamma(s)\Delta_G^{-1}) \cdot \mu = \Delta_G(s)(\Delta_G^{-1} \cdot \mu) = \Delta_G(s)\mu'$, therefore, for every right Haar measure $\nu$, we have $\gamma(s)\nu = \Delta_G(s)\nu$. Since $\dot{\mu}$ is a right Haar measure, $\dot{\mu} = a \Delta_G^{-1} \cdot \mu$ with a constant $a > 0$; it follows that

$$
\mu = a(\Delta_G^{-1} \cdot \mu)^{\vee} = a \Delta_G \cdot \dot{\mu} = a^2 \mu,
$$

therefore $a = 1$ and finally $\dot{\mu} = \Delta_G^{-1} \cdot \mu$. One sees similarly that $\dot{\nu} = \Delta_G \cdot \nu$.

We therefore have the following results:

Formulary. — Let G be a locally compact group, $\Delta$ its modulus, $\mu$ a left Haar measure, and $\nu$ a right Haar measure.

1) One has

$$
\gamma(s)\mu = \mu \quad \delta(s)\mu = \Delta(s)\mu \quad \check{\mu} = \Delta^{-1} \cdot \mu .
$$

If $f$ is $\mu$-integrable on G, then the left and right translates of $f$ are $\mu$-integrable, and

$$
\int f(sx)\, d\mu(x) = \int f(x)\, d\mu(x)
$$
(21)
$$
\int f(xs)\, d\mu(x) = \Delta(s)^{-1} \int f(x)\, d\mu(x) .
$$

Moreover, $\check{f}$ is integrable for $\Delta^{-1} \cdot \mu$ and

$$
\int f(x^{-1})\Delta(x)^{-1}\, d\mu(x) = \int f(x)\, d\mu(x) .
$$
(22)

If A is a $\mu$-integrable subset of G, then sA and As are $\mu$-integrable and

$$
\mu(sA) = \mu(A) \qquad \mu(As) = \Delta(s)\mu(A) .
$$
(23)

2) One has

$$
\delta(s)\nu = \nu \quad \gamma(s)\nu = \Delta(s)\nu \quad \check{\nu} = \Delta \cdot \nu .
$$

If $f$ is $\nu$-integrable on G, then the left and right translates of $f$ are $\nu$-integrable and

$$
\int f(xs)\, d\nu(x) = \int f(x)\, d\nu(x)
$$
(25)
$$
\int f(xs)\, d\nu(x) = \Delta(s) \int f(x)\, d\nu(x) .
$$

Moreover, $\check{f}$ is integrable for $\Delta \cdot \nu$ and

$$
\int f(x^{-1})\Delta(x)\, d\nu(x) = \int f(x)\, d\nu(x) .
$$
(26)

If A is a $\nu$-integrable subset of G, then sA and As are $\nu$-integrable and

$$
\nu(As) = \nu(A) \qquad \nu(sA) = \Delta(s)^{-1} \nu(A) .
$$
(27)

3) $\nu$ is proportional to $\Delta^{-1} \cdot \mu$, and $\mu$ is proportional to $\Delta \cdot \nu$.

4) Suppose G is *unimodular*. Let $\mu$ be a Haar measure on G. Then:

$$
\gamma(s)\mu = \delta(s)\mu = \dot{\mu} = \mu .
$$

If $f$ is $\mu$-integrable on G, then the left and right translates of $f$ are $\mu$-integrable, as is $\check{f}$, and

$$
\int f(sx)\,d\mu(x) = \int f(xs)\,d\mu(x) = \int f(x^{-1})\,d\mu(x) = \int f(x)\,d\mu(x) .
$$

If A is a $\mu$-integrable subset of G, then sA, As and $A^{-1}$ are $\mu$-integrable and

$$
\mu(sA) = \mu(As) = \mu(A^{-1}) = \mu(A) .
$$

The analogous properties hold for the essential integral.

#### Proposition 3 {#int-vii-s1-prop-3 .statement}

*If there exists in G a compact neighborhood V of e invariant under the inner automorphisms, then G is unimodular.*

For, let $\mu$ be a left Haar measure on G. For every $s \in G$,

$$
\mu(V) = \mu(s^{-1}Vs) = \Delta_G(s)\mu(V) ,
$$

whence $\Delta_G(s) = 1$ since $0 < \mu(V) < +\infty$.

From this, one deduces immediately:

#### Corollary {#int-vii-s1-n3-cor-1 .statement}

*If G is discrete, or compact, or commutative, then G is unimodular.*

This is moreover trivial when G is *commutative*. Note also that if G is *discrete*, then the measure on G for which each point has mass 1 is obviously a left and right Haar measure on G, called the *normalized* Haar measure on G. If G is *compact*, there exists one and only one Haar measure on G such that $\mu(G) = 1$; it is called the *normalized* Haar measure of G. The preceding two conventions are not in accord when G is both discrete and compact, that is, finite; when we are in this case we shall always explicitly specify what is meant by normalized Haar measure.

Subgroups and quotient groups of a unimodular group are not always unimodular (\S 2, Exer. 5). See, however, Prop. 10 of \S 2, No. 7.

*We shall see later that semi-simple or nilpotent connected Lie groups are unimodular.*

### 4. Modulus of an automorphism

Let G be a locally compact group, $\varphi$ an automorphism of G, and $\mu$ a left Haar measure on G. It is clear that $\varphi^{-1}(\mu)$ is also a left Haar measure on G. Therefore there exists (No. 2, Th. 1) one and only one number $a > 0$ such that $\varphi^{-1}(\mu) = a \mu$. By No. 2, Th. 1, this number is independent of the choice of $\mu$. Note that if one had started with a right Haar measure, for example $\Delta_G^{-1} \cdot \mu$ (No. 3), one would have arrived at the same scalar $a$: for, since $\varphi^{-1}$ leaves $\Delta_G$ invariant (No. 3, Remark), one has $\varphi^{-1}(\Delta_G^{-1} \cdot \mu) = \Delta_G^{-1} \cdot \varphi^{-1}(\mu) = a \Delta_G^{-1} \cdot \mu$.

#### Definition 4 {#int-vii-s1-def-4 .statement}

*The number $a > 0$ such that $\varphi^{-1}(\mu) = a \mu$ is called the modulus of the automorphism $\varphi$ and is denoted $\operatorname{mod}_G \varphi$ or simply $\operatorname{mod} \varphi$.*

If $f$ is a $\mu$-integrable function on G, then

$$
\int f(\varphi^{-1}(x)) d\mu(x) = (\operatorname{mod} \varphi) \int f(x) d\mu(x).
$$

If A is a $\mu$-integrable subset of G, then

$$
\mu(\varphi(A)) = (\operatorname{mod} \varphi) \mu(A).
$$

In particular, for $s \in G$, let $i_s$ be the inner automorphism $x \mapsto s^{-1} x s$. Then $i_s^{-1} = \delta(s) \gamma(s)$, therefore

$$
i_s^{-1}(\mu) = \delta(s) \mu = \Delta_G(s) \mu,
$$

consequently

$$
\operatorname{mod} i_s = \Delta_G(s).
$$

If G is either discrete or compact, then its normalized Haar measure is transformed into itself by every automorphism $\varphi$ of G, as one sees immediately by transport of structure. Thus *an automorphism of a discrete or compact group has modulus 1*.

#### Proposition 4 {#int-vii-s1-prop-4 .statement}

*Let G be a locally compact group, $\Gamma$ a topological group, and $\gamma \mapsto u_\gamma$ a homomorphism of $\Gamma$ into the group $\mathcal{G}$ of automorphism of G, such that $(\gamma, x) \mapsto u_\gamma(x)$ is a continuous mapping of $\Gamma \times G$ into G. Then, the mapping $\gamma \mapsto \operatorname{mod}(u_\gamma)$ is a continuous representation of $\Gamma$ in $\mathbf{R}_+^*$.

This mapping is obviously a representation (algebraic) of $\Gamma$ in $\mathbf{R}_+^*$; it will suffice to prove its continuity. Let $f \in \mathcal{K}(G)$ and let S be its support.*

Let $\gamma_0 \in \Gamma$ and let $U$ be a relatively compact neighborhood of $u_{\gamma_0}^{-1}(S)$. The mapping $\gamma \mapsto u_\gamma$ is a continuous mapping of $\Gamma$ into $\mathcal{G}$ equipped with the topology of compact convergence (GT, X, §3, No. 4, Th. 3); therefore $u_\gamma^{-1}(S) \subset U$ for $\gamma$ sufficiently near $\gamma_0$. Lemma 1 of No. 1 then proves that $\int f(u_\gamma(x)) d\mu(x)$ (where $\mu$ denotes a left Haar measure of $G$) depends continuously on $\gamma$; whence the proposition.

### 5. Haar measure of a product

#### Proposition 5 {#int-vii-s1-prop-5 .statement}

— *Let* $(G_\iota)_{\iota \in I}$ *be a family of locally compact groups*. *For every* $\iota \in I$ *let* $\mu_\iota$ *be a left (resp. right) Haar measure on* $G_\iota$. *Assume that there exists a finite subset* $J$ *of* $I$ *such that, for every* $\iota \in I - J$, $G_\iota$ *is compact and* $\mu_\iota(G_\iota) = 1$. *Then the product measure* $\bigotimes_{\iota \in I} \mu_\iota$ *is a left (resp. right) Haar measure on* $G = \prod_{\iota \in I} G_\iota$. *If* $x = (x_\iota) \in G$ *then*
$$
\Delta_G(x) = \prod_{\iota \in I} \Delta_{G_\iota}(x_\iota).
$$
For every finite subset $J$ of $I$, $\bigotimes_{\iota \in J} \mu_\iota$ is a left (resp. right) Haar measure on $\prod_{\iota \in J} G_\iota$, as follows immediately from the definitions. Therefore $\bigotimes_{\iota \in I} \mu_\iota$ is a left (resp. right) Haar measure on $G$ (Ch. III, §4, No. 6, Prop. 9). On the other hand, if the $\mu_\iota$ are left Haar measures then
$$
\delta(x) \left( \bigotimes_{\iota \in I} \mu_\iota \right) = \bigotimes_{\iota \in I} \delta(x_\iota) \mu_\iota = \bigotimes_{\iota \in I} (\Delta_{G_\iota}(x_\iota) \mu_\iota) = \left( \prod_{\iota \in I} \Delta_{G_\iota}(x_\iota) \right) \bigotimes_{\iota \in I} \mu_\iota,
$$
whence $\Delta_G(x) = \prod_{\iota \in I} \Delta_{G_\iota}(x_\iota)$.

#### Example {#int-vii-s1-n5-exa-1 .statement}

— 1) Lebesgue measure on $\mathbf{R}^n$ is a Haar measure of the additive group $\mathbf{R}^n$.

2) The mapping $(r, u) \mapsto ru$ is an isomorphism of $\mathbf{R}_+^* \times \mathbf{U}$ onto $\mathbf{C}^*$ (GT, VIII, §1, No. 3). If $\mathbf{C}^*$ is identified with $\mathbf{R}_+^* \times \mathbf{U}$ by means of this isomorphism, and if $du$ denotes a Haar measure on $\mathbf{U}$, then $r^{-1} dr du$ is a Haar measure on $\mathbf{C}^*$ by Example 2 of No. 2. On the other hand, the bijection $\theta \mapsto e^{2i\pi \theta}$ of $[0, 1[$ onto $\mathbf{U}$ transforms the Lebesgue measure $d\theta$ on $[0, 1[$ into a Haar measure on $\mathbf{U}$ by Example 3 of No. 2. It follows that if $f \in \mathcal{H}(\mathbf{C}^*)$, the integral
$$
\int_0^{+\infty} \int_0^1 f(re^{2i\pi \theta}) r^{-1} dr\, d\theta
$$
defines a Haar measure on $\mathbf{C}^*$.

### 6. Haar measure of an inverse limit*

Let G be a locally compact group (hence complete). Let $(K_\alpha)_{\alpha \in A}$ be a decreasing directed family of compact normal subgroups of G, with intersection $\{e\}$ (so that the filter base formed by the $K_\alpha$ converges to e). Set $G_\alpha = G / K_\alpha$; let $\varphi_\alpha : G \to G_\alpha$ and $\varphi_{\beta \alpha} : G_\alpha \to G_\beta \ (\alpha \geq \beta)$ be the canonical homomorphisms. Then, the inverse limit of the inverse system $(G_\alpha, \varphi_{\beta \alpha})$ may be identified with G, and the canonical mapping of this inverse limit into $G_\alpha$ is identified with $\varphi_\alpha$ (GT, III, §7, No. 3, Prop. 2). The mappings $\varphi_\alpha$ and $\varphi_{\beta \alpha}$ are proper (*loc. cit.*, §4, No. 1, Cor. 2 of Prop. 1). These assumptions remain fixed throughout this subsection.

\* Lemma 2. — a) *Let $f \in \mathcal{K}_+(G)$, S a compact subset of G containing Supp $f$, U an open neighborhood of S in G, and $\varepsilon > 0$. There exist an $\alpha \in A$ and a function $g \in \mathcal{K}_+(G)$, zero outside U and constant on the cosets of $K_\alpha$, such that $|f - g| \leq \varepsilon$.

b) *Let $\mu$ and $\mu'$ be two measures on G such that $\varphi_\alpha(\mu) = \varphi_\alpha(\mu')$ for all $\alpha \in A$. Then $\mu = \mu'$.

There exists an $\alpha_1 \in A$ such that $K_{\alpha_1} S \cap K_{\alpha_1}(G - U) = \emptyset$ (GT, II, §4, No. 3, Prop. 4). Augmenting S and diminishing U, we may therefore assume that S and U are unions of cosets of $K_{\alpha_1}$. Consider the continuous numerical functions $h$ on S having the following property: there exists an $\alpha \geq \alpha_1$ such that $h$ is constant on the cosets of $K_\alpha$. These functions form a subalgebra of $\mathcal{K}(S)$ (because $(K_\alpha)$ is a decreasing directed family) that contains the constants and separates the points of S: for, let $x, y$ be two distinct points of S; since the intersection of the $K_\alpha$ is $\{e\}$, there exists an $\alpha \geq \alpha_1$ such that $\varphi_\alpha(x) \neq \varphi_\alpha(y)$, then a numerical function $u$ continuous on $\varphi_\alpha(S)$ such that $u(\varphi_\alpha(x)) \neq u(\varphi_\alpha(y))$. By the Stone–Weierstrass theorem, there exist an $\alpha \geq \alpha_1$ and a continuous function $h \geq 0$ on S, constant on the cosets of $K_\alpha$, such that $|f - h| \leq \frac{\varepsilon}{2}$ on S. For every $t \in \mathbf{R}$, set $\delta(t) = \left( t - \frac{\varepsilon}{2} \right)^+$, and set $h' = \delta \circ h$. Then $h'$ is a function $\geq 0$, continuous on S, constant on the cosets of $K_\alpha$, and $|h - h'| \leq \frac{\varepsilon}{2}$ on S, therefore $|f - h'| \leq \varepsilon$ on S. On the other hand, $h'(x) = 0$ if x belongs to the boundary of S in G, because then $h(x) \leq \frac{\varepsilon}{2}$. If $h'$ is extended by 0 on the complement of S, one obtains a function $g$ that meets the requirements, which proves a).

Now let $\mu, \mu'$ be two measures on G such that $\varphi_\alpha(\mu) = \varphi_\alpha(\mu')$ for all $\alpha \in A$. Let $v \in \mathcal{K}(G)$ be a function constant on the cosets of $K_\alpha$ for some $\alpha \in A$, so that we may write $v = w \circ \varphi_\alpha$ with $w \in \mathcal{K}(G_\alpha)$; then

\* Cf. Ch. III, §4, No. 5.

$$
\mu(v) = (\varphi_\alpha(\mu))(w) = (\varphi_\alpha(\mu'))(w) = \mu'(v); \text{ it follows that } \mu = \mu' \text{ by virtue of a)}.
$$

#### Proposition 6 {#int-vii-s1-prop-6 .statement}

*For every* $\alpha \in A$, *let* $\mu_\alpha$ *be a positive measure on* $G_\alpha$. *Suppose that* $\varphi_{\beta\alpha}(\mu_\alpha) = \mu_\beta$ *for* $\alpha \geq \beta$. *Then, there exists one and only one positive measure* $\mu$ *on* $G$ *such that* $\varphi_\alpha(\mu) = \mu_\alpha$ *for all* $\alpha \in A$.

Uniqueness follows immediately from Lemma 2 b). Let us prove the existence of $\mu$. Let $V$ be the vector space of functions belonging to $\mathcal{K}(G)$ and constant on the cosets of some $K_\alpha$ ($\alpha$ may depend on the function). It follows from Lemma 2 a) that $V$ satisfies the condition (P) of Ch. III, §1, No. 7, Prop. 9: for, let $K$ be a compact set in $G$ and choose $f \in \mathcal{K}_+(G)$ with $f(x) > 0$ for all $x \in K$; let $a > 0$ be the smallest value of $f$ on $K$; by Lemma 2 a), there exists a function $g \in V \cap \mathcal{K}_+(G)$ such that $|f - g| \leq a/2$, therefore $g(x) > 0$ for all $x \in K$, and condition (P) is verified. Let $f \in V$. There exists an $\alpha \in A$ such that $f$ is constant on the cosets of $K_\alpha$. By passage to the quotient, $f$ defines a function $f_\alpha \in \mathcal{K}(G_\alpha)$. The number $\mu(f) = \mu_\alpha(f_\alpha)$ does not depend on the choice of $\alpha$: for, let $\beta$ be any index such that $f$ is constant on the cosets of $K_\beta$; let $\gamma \in A$ be such that $\gamma \geq \alpha, \gamma \geq \beta$; then $f$ defines functions $f_\beta \in \mathcal{K}(G_\beta)$, $f_\gamma \in \mathcal{K}(G_\gamma)$ such that $f = f_\beta \circ \varphi_\beta = f_\gamma \circ \varphi_\gamma$; then $f_\alpha \circ \varphi_{\alpha\gamma} = f_\gamma$, therefore $\mu_\gamma(f_\gamma) = (\varphi_{\alpha\gamma}(\mu_\gamma))(f_\alpha) = \mu_\alpha(f_\alpha)$, and similarly $\mu_\gamma(f_\gamma) = \mu_\beta(f_\beta)$, whence our assertion. This established, it is clear that $\mu$ is a linear form on $V$ and that $\mu(f) \geq 0$ for $f \geq 0$. By Prop. 9 of Ch. III, §1, No. 7, $\mu$ may be extended to a positive measure on $G$, which we again denote by $\mu$. One has $\varphi_\alpha(\mu) = \mu_\alpha$ for all $\alpha \in A$ by the very construction of $\mu$.

#### Definition 5 {#int-vii-s1-def-5 .statement}

*The measure* $\mu$ *is said to be the inverse limit (or projective limit) of the* $\mu_\alpha$.

#### Proposition 7 {#int-vii-s1-prop-7 .statement}

*We retain the notations of Prop. 6. If each* $\mu_\alpha$ *is a left (resp. right) Haar measure on* $G_\alpha$, *then* $\mu$ *is a left (resp. right) Haar measure on* $G$.

Suppose, for example, that the $\mu_\alpha$ are left Haar measures. Let $s \in G$. For every $x \in G$,

$$
(\varphi_\alpha \circ \gamma(s))(x) = \varphi_\alpha(sx) = \varphi_\alpha(s)\varphi_\alpha(x) = (\gamma(\varphi_\alpha(s)) \circ \varphi_\alpha)(x);
$$

therefore $\varphi_\alpha(\gamma(s)\mu) = \gamma(\varphi_\alpha(s))\mu_\alpha = \mu_\alpha$. Therefore $\gamma(s)\mu = \mu$ by Lemma 2 b), thus $\mu$ is a left Haar measure.

We suppose henceforth the $K_\alpha$ to be not only compact, but open in $G$. The $G_\alpha$ are then discrete and, for $\beta \geq \alpha$, $K_\alpha/K_\beta$ is a compact and discrete group, hence is finite. The group $G$ is unimodular (Prop. 3).

#### Proposition 8 {#int-vii-s1-prop-8 .statement}

a) *Let* $\mu$ *and* $\mu'$ *be two positive measures on* $G$ *such that, for every* $\alpha$ *and for every coset* $C$ *of* $K_\alpha$, $\mu(C) = \mu'(C)$. *Then* $\mu = \mu'$.

b) *Fix an* $\alpha_0 \in A$. *For every* $\alpha \geq \alpha_0$ *let* $n_\alpha$ *be the number of elements of the finite group* $K_{\alpha_0}/K_\alpha$. *There exists one and only one positive measure* $\mu$ *on* $G$ *such that, for every* $\alpha \geq \alpha_0$, *each coset of* $K_\alpha$ *has measure* $n_\alpha^{-1}$. *Moreover, $\mu$ is a Haar measure on* $G$, *such that* $\mu(K_{\alpha_0}) = 1$.

Let $\mu$ and $\mu'$ be two positive measures on $G$ satisfying the condition a). The points of the discrete group $G_\alpha$ then have the same measure for $\varphi_\alpha(\mu)$ and $\varphi_\alpha(\mu')$, whence $\varphi_\alpha(\mu) = \varphi_\alpha(\mu')$, and this for all $\alpha$. Therefore $\mu = \mu'$ (Lemma 2 b)).

Let us prove b). For every $\alpha \geq \alpha_0$, let $\mu_\alpha$ be the Haar measure of the discrete group $G_\alpha$ such that every point has measure $n_\alpha^{-1}$. Let $\alpha, \beta$ be such that $\alpha \geq \beta \geq \alpha_0$. Then $K_\beta/K_\alpha$ has $n_\alpha/n_\beta$ elements. Therefore $\varphi_{\beta\alpha}(\mu_\alpha)$ is the measure on $G_\beta$ such that each point has measure $n_\alpha^{-1} \cdot \frac{n_\alpha}{n_\beta} = n_\beta^{-1}$; in other words, $\varphi_{\beta\alpha}(\mu_\alpha) = \mu_\beta$. It then suffices to apply Props. 6 and 7.

#### Example {#int-vii-s1-n6-exa-1 .statement}

— Let $\mathbf{Q}_p$ be the $p$-adic field, the completion of $\mathbf{Q}$ for the $p$-adic absolute value $|x|_p = p^{-v_p(x)}$ (GT, IX, §3, No. 2, *Example 3*). The elements of $\mathbf{Q}_p$ are called *$p$*-*adic numbers*. We denote again by $|x|_p$ the continuous extension of the $p$-adic absolute value to $\mathbf{Q}_p$. One has

$$
|x + y|_p \leq \sup(|x|_p, |y|_p)
$$

for $x, y$ in $\mathbf{Q}$ (*loc. cit.*), hence for $x, y$ in $\mathbf{Q}_p$; moreover, if $|y|_p < |x|_p$ then $|x + y|_p = |x|_p$, because $|x|_p = |(x + y) - y|_p \leq \sup(|x + y|_p, |y|_p)$. If $(x_n)$ is a sequence of points of $\mathbf{Q}_p$ tending to $x \in \mathbf{Q}_p^*$, then $|x - x_n|_p < |x|_p$ and $|x - x_n|_p < |x_n|_p$ for $n$ sufficiently large, therefore $|x|_p = |x_n|_p$. This proves that, for every $x \in \mathbf{Q}_p^*$, $|x|_p$ is a power of $p$.

Let $\mathbf{Z}_p$ be the closure of $\mathbf{Z}$ in $\mathbf{Q}_p$; this is a subring of $\mathbf{Q}_p$; its elements are called *$p$*-*adic integers*. One has $|x|_p \leq 1$ for every $x \in \mathbf{Z}_p$. Conversely, let $x$ be an element of $\mathbf{Q}_p$ such that $|x|_p \leq 1$, and let us show that $x \in \mathbf{Z}_p$; there exists a sequence $(x_n)$ of elements of $\mathbf{Q}$ tending to $x$, and $|x_n|_p \leq 1$ for $n$ sufficiently large by what we have seen above; it suffices to show that $x_n$ belongs to $\mathbf{Z}_p$ for $n$ sufficiently large; in other words, we are reduced to the case that $x \in \mathbf{Q}$; then $x = a/b$ with $b$ relatively prime to $p$; for every integer $n > 0$, there exist $b'_n \in \mathbf{Z}$ and $h_n \in \mathbf{Z}$ such that $bb'_n + h_n p^n = 1$, whence $x = \frac{abb'_n + ah_n p^n}{b} = ab'_n + \frac{ah_n p^n}{b}$ and $|x - ab'_n|_p \leq p^{-n}$, therefore $ab'_n$ tends to $x$.

From this, it follows that the closed ball with center 0 and radius $p^{-n}$, identical to the open ball with center 0 and radius $p^{-n+1}$, is $p^n \mathbf{Z}_p$. The topological space $\mathbf{Q}_p$ is therefore zero-dimensional, hence totally disconnected (GT, IX, §6, No. 4).

Let us show that the integers $0, 1, \ldots, p^n - 1$ constitute a system of representatives of $\mathbf{Z}_p$ modulo $p^n \mathbf{Z}_p$. First, $|k - k'|_p > p^{-n}$ for two such integers $k$ and $k'$, therefore the classes modulo $p^n \mathbf{Z}_p$ of these integers are distinct. On the other hand, let $x \in \mathbf{Z}_p$; there exists a $k \in \mathbf{Z}$ such that $|x - k|_p \leq p^{-n}$; adding a suitable multiple of $p^n$ to $k$, one can suppose that $k \in [0, p^n - 1]$, and $x$ is congruent to $k$ modulo $p^n \mathbf{Z}_p$. Whence our assertion. This shows that $\mathbf{Z}_p / p^n \mathbf{Z}_p$ is canonically isomorphic to $\mathbf{Z}/p^n \mathbf{Z}$. One sees, moreover, that $\mathbf{Z}_p$ is precompact, hence *compact* since it is complete. Since $\mathbf{Z}_p$ is an open subgroup of $\mathbf{Q}_p$, $\mathbf{Q}_p$ is *locally compact*. The topology of $\mathbf{Q}_p$ has a countable base (GT, IX, §2, No. 9, Cor. of Prop. 16). The additive group $\mathbf{Q}_p$ may be identified with the inverse limit of the discrete groups $\mathbf{Q}_p / p^n \mathbf{Z}_p$.

There exists one and only one Haar measure $\alpha$ on the additive group $\mathbf{Q}_p$ such that $\alpha(\mathbf{Z}_p) = 1$; it is called the *normalized Haar measure* on $\mathbf{Q}_p$. Since $\mathbf{Z}_p$ is the union of $p^n$ disjoint cosets of $p^n \mathbf{Z}_p$ ($n$ an integer $\geq 0$), one has $\alpha(p^n \mathbf{Z}_p) = p^{-n}$; similarly $\alpha(p^{-n} \mathbf{Z}_p) = p^n$, so that, finally, $\alpha(p^n \mathbf{Z}_p) = p^{-n}$ for every $n \in \mathbf{Z}$. By Prop. 8 b), $\alpha$ *is the only positive measure on* $\mathbf{Q}_p$ *such that every coset of* $p^n \mathbf{Z}_p$ (*n* *an integer* $\geq 0$) *has measure* $p^{-n}$.

The restriction of $\alpha$ to $\mathbf{Z}_p$ is obviously a Haar measure on $\mathbf{Z}_p$.

### 7. Local definition of a Haar measure

#### Proposition 9 {#int-vii-s1-prop-9 .statement}

*Let G be a locally compact group, V an open subset of G, and $\mu$ a nonzero positive measure on V having the following property: if U is an open subset of V and if $s \in G$ is such that $sU \subset V$, then the image of the measure $\mu_U$ induced by $\mu$ on U, under the homeomorphism $x \mapsto sx$ of U onto sU, is $\mu_{sU}$. Then, there exists one and only one left Haar measure $\alpha$ on G that induces $\mu$ on V.*

For every $s \in G$, let $\mu_s$ be the image of $\mu$ under the homeomorphism $x \mapsto sx$ of V onto sV. The restriction of $\mu_s$ to $V \cap sV$ is the image of $\mu_{s^{-1}V \cap V}$ under the restriction of $x \mapsto sx$ to $s^{-1}V \cap V$; by hypothesis, this image is $\mu_{V \cap sV}$. By translation, one concludes from this that $\mu_s$ and $\mu_t$ have the same restriction to $sV \cap tV$ for any $s, t$. Therefore, by Prop. 1 of Ch. III, §2, No. 1, there exists a measure $\alpha$ on G that induces $\mu_s$ on sV for every $s$. It is clear that $\alpha$ is the unique left Haar measure on G inducing $\mu$ on V.

#### Corollary {#int-vii-s1-n7-cor-1 .statement}

*Let G, G' be two locally compact groups, V (resp. V') an open neighborhood of the neutral element of G (resp. G'), and $\varphi$ a local isomorphism of G' with G (GT, III, §1, No. 3, Def. 2) defined on V', such that $\varphi(V') = V$. Let $\alpha'$ be a left Haar measure on G', and $\alpha'_V$, its restriction to $V'$. Then $\varphi(\alpha'_{V'})$ is the restriction to $V$ of a unique left Haar measure $\alpha$ on $G$.

Let $V_1$ be an open neighborhood of $e$ in $G$ such that $V_1 V_1^{-1} \subset V$. Let $\mu$ be the restriction of $\varphi(\alpha'_{V'})$ to $V_1$. Let $U$ be an open subset of $V_1$ and let $s \in G$ be such that $sU \subset V_1$. Then $s \in V_1 V_1^{-1} \subset V$, therefore $s = \varphi(s')$ for some $s' \in V'$. Let $x \in U$. Then $x = \varphi(x')$ for some $x' \in V'$, therefore $sx = \varphi(s')\varphi(x') = \varphi(s'x')$ since $sx \in sU \subset V$. Since the left translations in $G'$ preserve $\alpha'$, one sees that $V_1$ and $\mu$ satisfy the conditions of Prop. 9. Let $\alpha$ be the left Haar measure on $G$ inducing $\mu$ on $V_1$. For every $t \in V$, there exists an open neighborhood $W$ of $e$ in $V_1$ such that $tW \subset V$. Then the restriction of $\varphi(\alpha'_{V'})$ to $tW$ may be deduced by translation from the restriction of $\mu$ to $W$, hence is the restriction of $\alpha$ to $tW$. Therefore $\varphi(\alpha'_{V'})$ is the restriction of $\alpha$ to $V$.

One says that $\alpha$ *is deduced from* $\alpha'$ *by means of the local isomorphism* $\varphi$.

#### Example {#int-vii-s1-n7-exa-1 .statement}

— The Haar measure on $T$ obtained in No. 2, *Example 3* may be deduced from the Lebesgue measure on $R$ by a local isomorphism of $R$ with $T$.

### 8. Relatively invariant measures

#### Proposition 10 {#int-vii-s1-prop-10 .statement}

*Let $G$ be a locally compact group, $\mu$ a relatively left-invariant measure on $G$ with multiplier $\chi$. If $\chi_1$ is a continuous representation of $G$ in $\mathbf{C}^*$, the measure $\chi_1 \cdot \mu$ is relatively left-invariant with multiplier $\chi_1 \chi$.*

For,

$$
\gamma(s)(\chi_1 \cdot \mu) = (\gamma(s)\chi_1) \cdot (\gamma(s)\mu) = (\chi_1(s^{-1})\chi_1) \cdot (\chi(s)^{-1}\mu)
= (\chi_1 \chi)(s)^{-1}(\chi_1 \cdot \mu).
$$

#### Corollary 1 {#int-vii-s1-prop-10-cor-1 .statement}

*Let $\mu$ be a left Haar measure on $G$. For a nonzero measure $\nu$ on $G$ to be relatively left-invariant, it is necessary and sufficient that it be of the form $a \chi \cdot \mu$, where $a \in \mathbf{C}^*$ and $\chi$ is a continuous representation of $G$ in $\mathbf{C}^*$; its multiplier is then $\chi$.*

The condition is sufficient (Prop. 10). On the other hand, if $\nu$ is a nonzero relatively left-invariant measure with multiplier $\chi$, then $\chi^{-1} \cdot \nu$ is left-invariant (Prop. 10) hence is of the form $a \mu$ with $a \in \mathbf{C}^*$ (No. 2, Cor. of Th. 1).

#### Corollary 2 {#int-vii-s1-prop-10-cor-2 .statement}

*Every relatively left-invariant measure is relatively right-invariant.*

For, with the notations of Cor. 1,

$$
\delta(s)(\chi \cdot \mu) = (\delta(s)\chi) \cdot (\delta(s)\mu) = (\chi(s)\chi) \cdot (\Delta_G(s)\mu)
= (\chi \Delta_G)(s)(\chi \cdot \mu).
$$

On account of Cor. 2, we shall henceforth speak of *relatively invariant measures on* G, without further specification. The relatively invariant measures admit as special cases the left Haar measures and the right Haar measures. Given a relatively invariant measure $\nu$ on G, it is convenient to distinguish between its *left multiplier* $\chi$ and its *right multiplier* $\chi'$, defined by $\gamma(s)\nu = \chi(s)^{-1}\nu$, $\delta(s)\nu = \chi'(s)\nu$. By (34), these multipliers satisfy the relation

$$
\chi' = \chi \Delta_G.
$$

Still denoting by $\mu$ a left Haar measure, we have

$$
\nu' = (\chi \cdot \mu)' = \dot{\chi} \cdot \dot{\mu} = (\chi^{-1} \Delta_G^{-1}) \cdot \mu,
$$

thus $\nu'$ is relatively invariant with left multiplier $\chi^{-1} \Delta_G^{-1}$ and right multiplier $\chi^{-1}$.

The concepts of negligible, locally negligible, measurable and locally integrable function are the same for every relatively invariant measure.

### 9. Quasi-invariant measures

#### Proposition 11 {#int-vii-s1-prop-11 .statement}

*Let G be a locally compact group, $\mu$ a left Haar measure on G. For a measure $\nu \neq 0$ on G to be left quasi-invariant, it is necessary and sufficient that $\nu$ be equivalent to $\mu$.*

Sufficiency is obvious. Let $\nu \neq 0$ be a left quasi-invariant measure, and let us show that $\nu$ is equivalent to $\mu$. We can restrict ourselves to the case that $\nu > 0$. Let A be a compact subset of G. We will show, as will establish the proposition, that the conditions $\mu(A) = 0$, $\nu(A) = 0$ are equivalent (Ch. V, §5, No. 5, Th. 2).

a) For every $f \in \mathcal{K}_+(G)$, the function $(x, y) \mapsto f(x)\varphi_A(xy)$ on $G \times G$ is $(\nu \otimes \mu)$-integrable, because it is upper semi-continuous, bounded, and its support is contained in the compact set $K \times K^{-1}A$ if one sets $K = \operatorname{Supp} f$. Therefore, by the Lebesgue–Fubini theorem,

$$
\int d\nu(y) \int \varphi_A(xy)f(x)\,d\mu(x) = \int f(x)\,d\mu(x) \int \varphi_A(xy)\,d\nu(y).
$$

b) Suppose $\nu(A) = 0$. By hypothesis, $\nu(xA) = 0$ for all $x \in G$, therefore the right side of (36) is zero. Therefore there exists a $\nu$-negligible set $N_f$ such that, for $y \notin N_f$,

$$
(37) \quad 0 = \int \varphi_A(xy)f(x)\,d\mu(x) = \Delta_G(y)^{-1} \int \varphi_A(x)f(xy^{-1})\,d\mu(x).
$$

Let B be a compact subset of G such that $\nu(B) \neq 0$, and take for $f$ a function in $\mathcal{K}_+(G)$ equal to 1 on $AB^{-1}$. There then exists a $y \in B$ such that (37) is verified. But since $\varphi_A(x)f(xy^{-1}) = \varphi_A(x)$ for $y \in B$, this proves that $\mu(A) = 0$.

c) Suppose $\mu(A) = 0$. Then, for every $f \in \mathcal{K}_+(G)$, the left side of (36) is zero, hence also the right side. Consequently, there exists a locally $\mu$-negligible set M such that $\int \varphi_A(xy)\,d\nu(y) = 0$ for $x \notin M$. Since $\mu \neq 0$, it follows that $\nu(xA) = 0$ for some $x \in G$, whence $\nu(A) = 0$.

Applying Prop. 11 to $G^0$, one sees that the right quasi-invariant measures are identical with the left quasi-invariant measures. They are called simply quasi-invariant measures on G.

### 10. Locally compact fields

#### Definition 6 {#int-vii-s1-def-6 .statement}

— *Let K be a locally compact field*$^{(1)}$. *For $a \in K^*$, one calls modulus of a*, and denotes by $\mathrm{mod}_K(a)$ or simply $\mathrm{mod}(a)$, *the modulus of the automorphism* $x \mapsto ax$ *of the additive group* $K^+$ *underlying K; one sets* $\mathrm{mod}(0) = 0$.

#### Example {#int-vii-s1-n10-exa-1 .statement}

— 1) Let $K = \mathbf{R}$. If $s > 0$ then $s \cdot [0,1] = [0,s]$; if $s < 0$, $s \cdot [0,1] = [s,0]$. Thus $\mathrm{mod}_\mathbf{R} t = |t|$ for all $t \in \mathbf{R}$.

2) Let $K = \mathbf{Q}_p$. If $s \in \mathbf{Q}_p^*$ is such that $|s|_p = p^{-n}$, then $s \mathbf{Z}_p$ is the set of $x \in \mathbf{Q}_p$ such that $|x|_p \leq p^{-n}$; therefore, if $\mu$ denotes the normalized Haar measure on $\mathbf{Q}_p$, then $\mu(s \mathbf{Z}_p) = p^{-n}$. Thus $\mathrm{mod}_{\mathbf{Q}_p} t = |t|_p$ for all $t \in \mathbf{Q}_p$.

#### Proposition 12 {#int-vii-s1-prop-12 .statement}

— *The function mod is continuous on K, and* $\mathrm{mod}(ab) = \mathrm{mod}(a)\mathrm{mod}(b)$ *for all* $a, b$ *in K*.

The last assertion is obvious. Prop. 4 of No. 4 shows that the function mod is continuous at every point of $K^*$. It remains only to show its continuity at 0. This is obvious for discrete K; we shall therefore assume K nondiscrete. Let $\alpha$ be a Haar measure on $K^+$ and let C be a compact subset of K such that $\alpha(C) > 0$; for $a \in K^*$, we have $\alpha(aC) = \mathrm{mod}(a)\alpha(C)$.

(1) Corps (A, I, §9, No. 1), also translated as "division ring" (GT, III, §6, No. 7).

Since K is not discrete, $\alpha(\{0\}) = 0$ (No. 2, Prop. 2); therefore, for every $\varepsilon > 0$ there exists an open neighborhood U of 0 such that $\alpha(U) \leq \varepsilon$. Since the product in K is continuous, $aC \subset U$ for $a$ sufficiently near 0, and then $\mathrm{mod}(a) \leq \varepsilon / \alpha(C)$.

#### Proposition 13 {#int-vii-s1-prop-13 .statement}

— *For every* $M > 0$, *let* $V_M$ *be the set of* $x \in K$ *such that* $\mathrm{mod}(x) \leq M$. *If* K *is nondiscrete, the* $V_M$ *form a fundamental system of compact neighborhoods of* 0 *in* K.

The $V_M$ are closed neighborhoods of 0 by Prop. 12. Let us show that they are compact. Let U be a compact neighborhood of 0. There exists an $r \neq 0$ in K such that $\mathrm{mod}(r) < 1$ and $r^n \in U$ for all $n > 0$: for, let W be a neighborhood of 0 such that $WU \subset U$; by Prop. 12, there exists an $r \neq 0$ in K such that $\mathrm{mod}(r) < 1$ and $r \in U \cap W$; then $r^2 \in WU \subset U$, and $r^n \in U$ for all $n > 0$ by induction on $n$. We are going to show that $V_M$ is contained in a finite union of sets $r^{-q}U$ ($q$ an integer $\geq 0$), which will prove that the $V_M$ are indeed compact. If $x$ is a cluster point of the sequence $(r^n)$, then $\mathrm{mod}(x)$ is a cluster point of the sequence $(\mathrm{mod}(r)^n)$, therefore $\mathrm{mod}(x) = 0$, $x = 0$; since U is compact, it follows (GT, I, §9, No. 1, Cor. of Th. 1) that $\lim_{n \to \infty} r^n = 0$. Now let $a \in V_M$. Since the sequence $(r^n a)_{n \geq 0}$ tends to 0, there exists a smallest integer $n \geq 0$ such that $r^n a \in U$. If $n > 0$ then $r^{n-1} a \notin U$, therefore $r^n a \in U \cap C(rU)$; the closure X of $U \cap C(rU)$ is compact since U is compact, and it does not contain 0 since $rU$ is a neighborhood of 0; therefore, in X, $\mathrm{mod}(x)$ is bounded below by a number $m > 0$. Thus, if $n > 0$, we have $m \leq \mathrm{mod}(r^n a)$, whence $\mathrm{mod}(r^{-1})^n \leq M/m$. Since $\mathrm{mod}(r^{-1}) > 1$, the integer $n$ can only take on a finite number of values, a number not depending on $a$, which completes the proof of our assertion.

This being so, since the intersection of the $V_M$ reduces to $\{0\}$ the $V_M$ form a fundamental system of neighborhoods of 0 (GT, I, §9, No. 2, Prop. 1).

#### Corollary {#int-vii-s1-n10-cor-1 .statement}

— *The topology of a nondiscrete locally compact field admits a countable base.*

For, K is the union of compact sets $V_1, V_2, \ldots$. On the other hand, K is metrizable by Prop. 1 of GT, IX, §3, No. 1. Therefore the topology of K admits a countable base (*loc. cit.*, §2, No. 9, Cor. of Prop. 16).

#### Proposition 14 {#int-vii-s1-prop-14 .statement}

— *Let* $\alpha$ *be a Haar measure on* $K^+$. *Then the measure* $\beta = (\mathrm{mod}_K)^{-1} \cdot \alpha$ *on* $K^*$ *is a left Haar measure on the multiplicative group* $K^*$.

For, if $b \in K^*$, the mapping $a \mapsto b^{-1} a$ of K into K transforms $\alpha$ into $(\mathrm{mod}_K b) \alpha$, hence $(\mathrm{mod}_K)^{-1} \cdot \alpha$ into itself, whence the proposition.

#### Corollary {#int-vii-s1-n10-cor-2 .statement}

— *Let* f *be a function defined on* $K^*$, *with values in* $\overline{\mathbf{R}}$ *or in a Banach space. For* f *to be* $\beta$-*integrable, it is necessary and sufficient* that $(\mathrm{mod}_K)^{-1} f$ be $\alpha$-integrable, in which case

$$
\int_{K^*} f(x) d\beta(x) = \int_{K^+} (\mathrm{mod}_K(x))^{-1} f(x) d\alpha(x).
$$

This follows from Prop. 14, the Cor. of Prop. 13, and Ch. V, §5, No. 3, Th. 1.

#### Proposition 15 {#int-vii-s1-prop-15 .statement}

— *Assume K to be commutative. Let u be an automorphism of the vector space E = K^n. Then*

$$
\mathrm{mod}_E u = \mathrm{mod}_K(\det u).
$$

It suffices to verify the formula when $u$ runs over a system of generators of $\mathbf{GL}(E)$. Now, $\mathbf{GL}(E)$ is generated by the following elements (A, II, §10, No. 13, Cor. 2 of Prop. 14):
(a) The elements $u_1$ of the form

$$
(x_1, \ldots, x_n) \mapsto (x_{\sigma(1)}, \ldots, x_{\sigma(n)}),
$$

where $\sigma \in \mathfrak{S}_n$;
(b) the elements $u_2$ of the form

$$
(x_1, \ldots, x_n) \mapsto (ax_1, x_2, \ldots, x_n)
$$

with $a \in K^*$;
(c) the elements $u_3$ of the form

$$
(x_1, \ldots, x_n) \mapsto (x_1 + \sum_{i=2}^n c_i x_i, x_2, \ldots, x_n).
$$

If $f \in \mathcal{H}(E)$ then, denoting by $\alpha$ a Haar measure on $K^+$,

$$
\int \cdots \int_{K^n} f(x_1 + \sum_{i=2}^n c_i x_i, x_2, \ldots, x_n) d\alpha(x_1) d\alpha(x_2) \ldots d\alpha(x_n)
$$
$$
= \int \cdots \int_{K^{n-1}} d\alpha(x_2) \ldots d\alpha(x_n) \int_K f(x_1 + \sum_{i=2}^n c_i x_i, x_2, \ldots, x_n) d\alpha(x_1)
$$
$$
= \int \cdots \int_{K^{n-1}} d\alpha(x_2) \ldots d\alpha(x_n) \int_K f(x_1, x_2, \ldots, x_n) d\alpha(x_1)
$$
$$
= \int \cdots \int_{K^n} f(x_1, \ldots, x_n) d\alpha(x_1) \ldots d\alpha(x_n),
$$

and on the other hand $\mathrm{mod}_K(\det u_3) = \mathrm{mod}_K(1) = 1$, whence the result for $u_3$. It is established in an analogous manner for $u_1$ and $u_2$.

Let K be a commutative locally compact field, E a vector space of finite dimension n over K. If $\varphi$ is an isomorphism of the vector space $K^n$ onto the vector space E, $\varphi$ transforms the topology of $K^n$ into a topology on E that makes E a locally compact vector space. This topology (called canonical) is independent of $\varphi$ since every automorphism of the vector space $K^n$ is bicontinuous. Absent express mention to the contrary, when we speak of E as a topological vector space, the topology will always be understood to be the one just defined. Every automorphism u of the vector space E is bicontinuous, therefore $\mathrm{mod}_E u$ is defined. If, on the other hand, u is a noninvertible endomorphism of E, one sets $\mathrm{mod}_E u = 0$. Then:

#### Corollary 1 {#int-vii-s1-prop-15-cor-1 .statement}

— *Let K be a commutative locally compact field, E a finite-dimensional vector space over K, and u an endomorphism of the vector space E. Then* $\mathrm{mod}_E(u) = \mathrm{mod}_K(\det u)$.

If u is invertible, this follows from Prop. 15. If u is not invertible then $\det u = 0$, therefore $\mathrm{mod}_K(\det u) = 0 = \mathrm{mod}_E u$.

#### Corollary 2 {#int-vii-s1-prop-15-cor-2 .statement}

— *Let E be a real vector space of finite dimension n, $(e_1, e_2, \ldots, e_n)$ a basis of E, P the set of* $x = \sum_{i=1}^n \xi_i e_i \in E$ *such that* $0 \leq \xi_i \leq 1$ *for all i*, and $\mu$ *the unique Haar measure on the additive group E such that* $\mu(P) = 1$. *Let* $x_1, \ldots, x_n$ *be points of E, S the closed convex envelope in E of the set* $\{0, x_1, \ldots, x_n\}$. *Writing* $x_i = \sum_{j=1}^n \alpha_{ij} e_j$, *one has*

$$
\mu(S) = \mu(\dot{S}) = \frac{1}{n!} |\det(\alpha_{ij})|.
$$

We shall identify E with $\mathbf{R}^n$ by means of the isomorphism that transforms $(e_i)$ into the canonical basis of $\mathbf{R}^n$. Then $\mu$ is identified with the Lebesgue measure $\mu_n$ on $\mathbf{R}^n$.

Suppose first that $x_i = e_i$ for all i. Then S is the set $S_n$ of $x = (\xi_i)$ in $\mathbf{R}^n$ such that

$$
\xi_i \geq 0 \text{ for all } i \quad \text{and} \quad \xi_1 + \cdots + \xi_n \leq 1.
$$

Set $\mu_n(S_n) = a_n$. Let $\lambda \in \mathbf{R}$. Identifying $\mathbf{R}^n$ with $\mathbf{R}^{n-1} \times \mathbf{R}$, we may consider the section $C_\lambda$ of $S_n$ at $\lambda$. This section is empty if $\lambda < 0$ or $\lambda > 1$; if $0 \leq \lambda \leq 1$, $C_\lambda$ is the set of $(\xi_1, \ldots, \xi_{n-1}) \in \mathbf{R}^{n-1}$ such that

$$
\xi_1 \geq 0, \ldots, \xi_{n-1} \geq 0, \quad \xi_1 + \cdots + \xi_{n-1} \leq 1 - \lambda,
$$

hence may be deduced from $S_{n-1}$ by a homothety of ratio $1 - \lambda$, so that $\mu_{n-1}(C_\lambda) = (1 - \lambda)^{n-1} a_{n-1}$. By the Lebesgue–Fubini theorem,

$$
a_n = \int_0^1 (1 - \lambda)^{n-1} a_{n-1} d\lambda = \frac{1}{n} a_{n-1}.
$$

Since $a_1 = 1$, one sees that $a_n = \frac{1}{n!}$.

Let us return to the general case of the corollary. Let $u$ be the endomorphism of $\mathbf{R}^n$ such that $u(e_i) = x_i$ for all $i$. One has $u(S_n) = S$. If $u$ is invertible, Prop. 15 proves that

$$
\mu_n(S) = \frac{1}{n!} |\det u| = \frac{1}{n!} |\det(\alpha_{ij})|.
$$

Since $S - \overset{\circ}{S}$ is contained in a finite number of hyperplanes, $\mu(\overset{\circ}{S}) = \mu(S)$. Finally, if $u$ is not invertible, then $S$ is contained in a hyperplane, so that $\mu(S) = 0 = \det(\alpha_{ij})$.

### 11. Finite-dimensional algebras over a locally compact field

Let $K$ be a commutative field, $A$ a $K$-algebra of finite rank with unity element. For every $a \in A$, let $L_a, R_a$ be the endomorphisms $x \mapsto ax$, $x \mapsto xa$ of the vector space $A$, and let $N_{A/K}(a) \in K$, $N_{A^0/K}(a) \in K$ be the norms of $a$ in the regular representations of $A$ and the opposite algebra $A^0$; recall that $N_{A/K}(a) = \det(L_a)$, $N_{A^0/K}(a) = \det(R_a)$ (A, III, §9, No. 3). The following conditions are equivalent: $a$ invertible, $L_a$ invertible in $\mathrm{Hom}_K(A, A)$, $R_a$ invertible in $\mathrm{Hom}_K(A, A)$, $N_{A/K}(a) \neq 0$, $N_{A^0/K}(a) \neq 0$. We denote by $A^*$ the set of invertible elements of $A$.

Now assume the field $K$ to be locally compact, hence the algebra $A$ to be locally compact. Then $N_{A/K}$ and $N_{A^0/K}$ are continuous mappings of $A$ into $K$, therefore $A^*$ is open in $A$. By Cor. 1 of Prop. 15 of No. 10,

$$
\mathrm{mod}_A L_a = \mathrm{mod}_K N_{A/K}(a), \quad \mathrm{mod}_A R_a = \mathrm{mod}_K N_{A^0/K}(a).
$$

#### Proposition 16 {#int-vii-s1-prop-16 .statement}

— *Let $\alpha$ be a Haar measure of the additive group of $A$. The measures*

$$
(\mathrm{mod}_K N_{A/K}(a))^{-1} d\alpha(a), \quad (\mathrm{mod}_K N_{A^0/K}(a))^{-1} d\alpha(a)
$$

*on $A^*$ are, respectively, left and right Haar measures of the multiplicative group $A^*$.*

Let $\alpha'$ be the restriction of $\alpha$ to the open set $A^*$. For $a \in A^*$, one has $L_a(\alpha') = (\mathrm{mod}_K N_{A/K}(a))^{-1} \alpha'$, therefore $(\mathrm{mod}_K N_{A/K}(a))^{-1} d\alpha'(a)$ is a left Haar measure on $A^*$ (No. 8, Cor. 1 of Prop. 10). Passing to the opposite algebra, one sees that $(\mathrm{mod}_K N_{A^0/K}(a))^{-1} d\alpha'(a)$ is a right Haar measure on $A^*$.

#### Proposition 17 {#int-vii-s1-prop-17 .statement}

— *Suppose A is a field (locally compact). For every $a \in A$, $\mathrm{mod}_A(a) = \mathrm{mod}_K N_{A/K}(a)$.*

This is a translation of the first formula of (38).

#### Example {#int-vii-s1-n11-exa-1 .statement}

— 1) Take $K = \mathbf{R}$, $A = \mathbf{C}$. Taking into account *Alg.*, chap. VIII, §12, n° 2, prop. 4, we obtain $\mathrm{mod}_\mathbf{C}(z) = |z|^2$ for all $z \in \mathbf{C}$. (2)

2) Take $K = \mathbf{R}$, and for A the *quaternion field* $\mathbf{H}$ (GT, VIII, §1, No. 4). Consider the following elements of $\mathbf{M}_2(\mathbf{C})$:

$$
X_1 = \begin{pmatrix} 0 & i \\ i & 0 \end{pmatrix} \quad X_2 = \begin{pmatrix} 0 & -1 \\ 1 & 0 \end{pmatrix} \quad X_3 = \begin{pmatrix} i & 0 \\ 0 & -i \end{pmatrix}
$$

which, together with $I_2$, form a basis of $\mathbf{M}_2(\mathbf{C})$ over $\mathbf{C}$. One verifies easily that

$$
X_1^2 = X_2^2 = X_3^2 = -I_2, \qquad X_1 X_2 = -X_2 X_1 = X_3,
$$
$$
X_2 X_3 = -X_3 X_2 = X_1, \qquad X_3 X_1 = -X_1 X_3 = X_2.
$$

The mapping $a + b i + c j + d k \mapsto a I_2 + b X_1 + c X_2 + d X_3$ may therefore be extended to a $\mathbf{C}$-isomorphism of the algebra $\mathbf{C} \otimes_\mathbf{R} \mathbf{H}$ onto the algebra $\mathbf{M}_2(\mathbf{C})$. Since $[\mathbf{H} : \mathbf{R}] = 4$, $\mathbf{C}$ is a neutralizing field of $\mathbf{H}$ (*Alg.*, chap. VIII, §10, n° 5), and the reduced norm of $q = a + b i + c j + d k \in \mathbf{H}$ is

$$
\mathrm{Nrd}(q) = \det(a I_2 + b X_1 + c X_2 + d X_3)
$$
$$
= \det \begin{pmatrix} a + i d & -c + i b \\ c + i b & a - i d \end{pmatrix} = a^2 + b^2 + c^2 + d^2 = \|q\|^2.
$$

By *Alg.*, chap. VIII, §12, n° 3, prop. 8, one has

$$
\mathrm{N}_{\mathbf{H}/\mathbf{R}}(q) = (\mathrm{Nrd}_{\mathbf{H}/\mathbf{R}}(q))^2 = \|q\|^4.
$$

This stated, Prop. 17 shows that

$$
\mathrm{mod}_\mathbf{H}(q) = \|q\|^4.
$$

A deeper study of the structure of locally compact fields will be made in CA, VI, §9.

(2) This also follows from Cor. 1 of Prop. 15 and the fact that left-multiplication by $z = a + i b$ has matrix $\begin{pmatrix} a & -b \\ b & a \end{pmatrix}$ with respect to the canonical basis $1, i$ of $\mathbf{C}$ over $\mathbf{R}$.

### Exercises {#int-vii-s1-exercises}

See the [exercises for § 1](exercises/s1/).
