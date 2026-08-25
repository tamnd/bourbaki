---
book: ac
book_title: Commutative Algebra
chapter: VI
chapter_title: VALUATIONS
section: 10
section_title: Extensions of a valuation to a transcendental extension
lang: en
source: ac-i-vii
book_pages: 434-440, 471-473
pdf_pages: 0452-0458, 0489-0491
extraction: ocr
subsections:
    - "no": 1
      title: THE CASE OF A MONOGENOUS TRANSCENDENTAL EXTENSION
      page: 434
      pdf_page: 452
    - "no": 2
      title: THE RATIONAL RANK OF A COMMUTATIVE GROUP
      page: 437
      pdf_page: 455
    - "no": 3
      title: THE CASE OF ANY TRANSCENDENTAL EXTENSION
      page: 438
      pdf_page: 456
statements: 14
exercises: 2
content_sha256: e3c861ffcd021309856ff685759ee07561069de46e3d425be802720ae6d29f75
---

## 10. EXTENSIONS OF A VALUATION TO A TRANSCENDENTAL EXTENSION

### 1. THE CASE OF A MONOGENOUS TRANSCENDENTAL EXTENSION

#### Lemma 1 {#ac-vi-s10-lem-1 .statement}

Let $K$ be *a field*, $v$ a valuation on $K$, $\Gamma$ *its* order group, $\Gamma'$ a totally ordered group containing $\Gamma$ and $\xi$ *an element of* $\Gamma'$. There exists *a* unique valuation w *on* $K(X)$ such *that*, *for* $P = \sum_j a_j X^j$ ($a_j \in K$), $w(P) = \inf_j (v(a_j) + j\xi)$.

By Proposition 4 of § 3, no. 2, it suffices to show that the formula

$$
w\left( \sum_j a_j X^j \right) = \inf_j (v(a_j) + j\xi)
$$

defines a valuation on the ring $K[X]$. As

$$
v(a_j + b_j) + j\xi \geq \inf(v(a_j), v(b_j)) + j\xi = \inf(v(a_j) + j\xi, v(b_j) + j\xi),
$$

it follows that

$$
w(P + Q) \geq \inf(w(P), w(Q))
$$

for $P, Q$ in $K[X]$, equality holding if $w(P) \neq w(Q)$. We show that

$$
w(PQ) = w(P) + w(Q)
$$

for $P = \sum a_j X^j$ and $Q = \sum b_j X^j$. Let $i$ (resp. $k$) be the least of the integers $j$ such that $v(a_j) + j\xi$ (resp. $v(b_j) + j\xi$) attains its minimum; let $a$ (resp. $\beta$) denote this minimum. For $j, j'$ in $\mathbf{N}$,

$$
w(a_j b_{j'} X^{j+j'}) = v(a_j) + j\xi + v(b_{j'}) + j'\xi \geq a + \beta,
$$

whence $w(PQ) \geq a + \beta$ by (2). Consider now the term $c X^{i+k}$ of degree $i + k$ in $PQ$; then $c = \sum_{n \in \mathbf{Z}} a_{i+n} b_{k-n}$; by the choice of $i$ and $k$, the element

$$
w(a_{i+n} b_{k-n} X^{i+k}) = v(a_{i+n}) + (i+n)\xi + v(b_{k-n}) + (k-n)\xi
$$

takes its minimum value $a + \beta$ once and once only with $n = 0$; hence $w(c X^{i+k}) = a + \beta$, whence, by (1),

$$
w(PQ) = \alpha + \beta = w(P) + w(Q).
$$

#### Proposition 1 {#ac-vi-s10-prop-1 .statement}

Let $K$ be *a field*, $v$ *a valuation on* $K$, $\Gamma$ *its order group*, $\Gamma'$ *a totally ordered group containing* $\Gamma$ *and* $\xi$ *an element of* $\Gamma'$ *such that the relations* $n\xi \in \Gamma, n \in \mathbf{Z}$ *imply* $n = 0$. Then there exists *a* unique valuation w *on* $K(X)$ *with values in* $\Gamma'$ *and extending* $v$ *such that* $w(X) = \xi$. The *residue field of* w *is equal to that of* $v$ *and its order group is the subgroup* $\Gamma + \mathbf{Z}\xi$ *of* $\Gamma'$.

We show first the uniqueness of w. Let $P = \sum_j a_j X^j$ be an element of $K[X]$. Then $w(a_j X^j) = v(a_j) + j\xi$, which shows that the monomials $a_j X^j$ such that $a_j \neq 0$ have distinct values for w. It follows that $w(P) = \inf_j (v(a_j) + j\xi)$, which shows both the uniqueness of w on $K[X]$ (hence also on $K(X)$) and the fact that the order group of w is $\Gamma + \mathbf{Z}\xi$. It is further seen that, if $P \neq 0$, we may write $P = a X^n (1 + u)$, where $a \in K^*, n \in \mathbf{N}, u \in K(X)$ and $w(u) > 0$; every element $R \neq 0$ of $K(X)$ can therefore be written in the form
$$
R = b X^n (1 + u'),
$$
where $b \in K^*, n \in \mathbf{Z}, u' \in K(X)$ and $w(u') > 0$; then $w(R) = v(b) + n \xi$, hence $w(R) = 0$ if and only if $v(b) = 0$ and $n = 0$; thus, when $w(R) = 0$, $R$ and $b$ are congruent modulo the ideal of $w$, which shows that the residue field of $w$ is equal to that of $v$.

Finally the existence of $w$ follows from Lemma 1.

#### Proposition 2 {#ac-vi-s10-prop-2 .statement}

*Let $K$ be a field, $v$ a valuation on $K$, $\Gamma$ its order group and $k$ its residue field. There exists a unique valuation $w$ on $K(X)$ extending $v$ such that $w(X) = 0$ and the image $t$ of $X$ in the residue field $k'$ of $w$ is transcendental over $k$. The order group of $w$ is equal to that of $v$ and its residue field is $k(t)$.*

To show the uniqueness of $w$, it will suffice for us to show that, if $P = \sum_j a_j X^j$ is a non-zero element of $K[X]$, then
$$
w(P) = \inf_j (v(a_j)).
$$
We may divide $P$ by an element of $K^*$ and suppose that $v(a_j) \geq 0$ for all $j$ and that one of the $v(a_j)$ is zero. As $w(X) = 0$, $P$ then belongs to the ring of $w$; writing $\bar{a}_j$ for the canonical image of $a_j$ in $k$, the canonical image of $P$ in the residue field $k'$ is $\sum_j \bar{a}_j t^j$; as $t$ is transcendental over $k$ and one of the $\bar{a}_j$ is non-zero, this image is non-zero, whence
$$
w(P) = 0 = \inf_j (v(a_j)).
$$
We now show the existence of $w$. The formula $w(P) = \inf_j (v(a_j))$ (for $P = \sum_j a_j X^j$) defines a valuation $w$ on $K(X)$, by virtue of Lemma 1, and $w$ obviously has the same order group as $v$. Then $w(X) = 0$. We show that the canonical image $t$ of $X$ in the residue field $k'$ of $w$ is transcendental over $k$: if $\sum_j \bar{a}_j t^j = 0$, where $\bar{a}_j \in k$ for all $j$, then, denoting by $a$, a representative of $\bar{a}_j$ in the ring of $v$, $w \left( \sum_j a_j X^j \right) > 0$; whence $v(a_j) > 0$ for all $j$, hence $\bar{a}_j = 0$ for all $j$. We show finally that $k' = k(t)$: every element $R$ of $K(X)$ may be written $R = c \left( \sum_j a_j X^j \right) / \left( \sum_j b_j X^j \right)$, where $c, a_j, b_j$ are in $K$, $v(a_j) \geq 0$ and $v(b_j) \geq 0$ for all $j$, one of the $v(a_j)$ and one of the $v(b_j)$ being zero; then $w(R) \geq 0$ if and only if $v(c) \geq 0$; denoting by $f$ the canonical homomorphism of the ring of $w$ onto $k'$,
$$
f(R) = f(c) \left( \sum_j f(a_j) t^j \right) / \left( \sum_j f(b_j) t^j \right),
$$

which proves our assertion.

#### Remark {#ac-vi-s10-n1-rem-1 .statement}

It should not be thought that the two types of extensions of v to K(X) which we have just met are the only ones; there may exist a third type of extension, where $\Gamma'/\Gamma$ is a torsion group and $k'$ a (not necessarily finite) algebraic extension of $k$. This third type is not necessarily provided by the procedure described in Lemma 1 (cf. § 3, Exercise 1).

### 2. THE RATIONAL RANK OF A COMMUTATIVE GROUP

#### Definition 1 {#ac-vi-s10-def-1 .statement}

*The rational rank of a commutative group G is the dimension of the vector Q-space* $G \otimes_{\mathbf{Z}} \mathbf{Q}$.

This dimension may also be defined as the least upper bound (finite or infinite) of the cardinals $r$ such that there exist $r$ elements of G which are linearly independent over $\mathbf{Z}$ (*Algebra*, Chapter II, § 7, no. 10, Proposition 26). The rational rank of G is *zero* if and only if G is a torsion group. For a subgroup of an additive group $\mathbf{R}^n$, the notion of rational rank coincides with that defined in *General Topology*, Chapter VII, § 1.

In the rest of this paragraph, we shall denote by $r(G)$ the rational rank of the commutative group G. If $G'$ is a subgroup of G, then (since $\mathbf{Q}$ is a flat $\mathbf{Z}$-module) we have the additive equation

$$
r(G) = r(G') + r(G/G').
$$

#### Proposition 3 {#ac-vi-s10-prop-3 .statement}

*Let G be a totally ordered Commutative group and H a subgroup of G. If $h(G)$ and $h(H)$ denote the heights of G and H* ($\S 4$, no. 4), *then the inequality*

$$
h(G) \leq h(H) + r(G/H)
$$

*holds*.

In fact, let $G_0 \subset G_1 \subset \ldots \subset G_n$ be a strictly increasing sequence of isolated subgroups of G. It is necessary to establish the inequality

$$
n \leq h(H) + r(G/H).
$$

It is obvious for $n = 0$. Suppose $n \geq 1$ and let us argue by induction on $n$. Applying the induction hypothesis to the group $G_{n-1}$ and its subgroup $H \cap G_{n-1}$, we obtain

$$
n - 1 \leq h(H \cap G_{n-1}) + r(G_{n-1}/(H \cap G_{n-1})).
$$

Then we distinguish two cases:

(a) $H \cap G_{n-1} = H$, in other words $H \subset G_{n-1}$. Inequality (7) may be written

$$
n \leq h(H) + r(G_{n-1}/H) + 1.
$$

Now $G/G_{n-1}$ is a totally ordered group not reduced to 0; it is therefore not a torsion group and $r(G/G_{n-1}) \geq 1$. Whence by (4), $r(G/H) \geq r(G_{n-1}/H) + 1$. Substituting in (8), we certainly obtain the desired inequality (6).

(b) $H \cap G_{n-1} \neq H$. As $H \cap G_{n-1}$ is an isolated subgroup of $H$, we conclude that $h(H) > h(H \cap G_{n-1}) + 1$. On the other hand, obviously $r(G/H) \geq r(G_{n-1}/(H \cap G_{n-1}))$. Substituting in (7), we again obtain (6).

#### Corollary {#ac-vi-s10-n2-cor-1 .statement}

*For every totally ordered commutative group G, $h(G) \leq r(G)$.* We set $H = (0)$ in Proposition 3.

#### Proposition 4 {#ac-vi-s10-prop-4 .statement}

*Let G be a totally ordered commutative group. Suppose that G is finitely generated and that $h(G) = r(G)$. Then G is isomorphic to $\mathbf{Z}^{r(G)}$ ordered lexicographically.*

Let us write $r = r(G) = h(G)$. If $r = 0$, then $G = (0)$. If $r = 1$, the structure of finitely generated commutative groups shows that there is an isomorphism $j$ of G onto Z (*Algebra*, Chapter VII, § 4, no. 6, Theorem 3). Now Z has only two total orderings compatible with its group structure, namely the usual ordering and its opposite. Hence $j$ or $-j$ is an isomorphism of the ordered group G onto Z with the usual ordering.

Suppose now that $r \geq 2$ and let us argue by induction on $r$. Let H be an isolated subgroup of G of height $r - 1$. Then $r(H) + r(G/H) = r$ (formula (4)), $r(H) \geq h(H) = r - 1$ and $r(G/H) \geq h(G/H) = 1$ (Corollary to Proposition 3), whence $r(H) = r - 1$ and $r(G/H) = 1$. The induction hypothesis shows that H is isomorphic to $\mathbf{Z}^{r-1}$ ordered lexicographically and the case $r = 1$ shows that $G/H$ is isomorphic to Z. As Z is a free Z-module, H is a *direct factor* of G (*Algebra*, Chapter 11, § 1, no. 11, Proposition 21). The following lemma then shows that G is isomorphic (not canonically) to the lexicographical product $H \times (G/H)$, which completes the proof.

#### Lemma 2 {#ac-vi-s10-lem-2 .statement}

*Let H be an isolated subgroup of a totally ordered commutative group G. If H is a direct factor of G, the ordered group G is isomorphic to the group $(G/H) \times H$ ordered lexicographically.*

Let $j$ be an isomorphism of $(G/H) \times H$ onto G such that $j(0, x) = x$ for all $x \in H$ and $j(y, x)$ belongs to the coset of H. As $(G/H) \times H$ is totally ordered, it amounts to showing that $j$ is *increasing* (*Set Theory*, Chapter III, § 1, no. 12, Proposition 11). Let $(y, x)$ be an element $\geq 0$ of $(G/H) \times H$ ordered lexicographically. If $y > 0$, the coset of H containing $j(y, x)$ is an element $> 0$, whence $j(y, x) > 0$, for, otherwise, $y \leq 0$ (§ 4, no. 2, Proposition 3). If $y = 0$ and $x \geq 0$, then $j(y, x) = x \geq 0$. Hence $j$ is certainly increasing.

### 3. THE CASE OF ANY TRANSCENDENTAL EXTENSION

In this no. we shall use the following notation : $K$ is a field, $K'$ an extension of $K$, $v$ a valuation on $K$, $v'$ an extension of $v$ to $K$, $\Gamma$ and $k$ (resp. $\Gamma'$ and $k'$) the order group and residue field of $v$ (resp. $v'$). We shall write:

$$
d(K'/K) = \dim.\mathrm{al},\ K' = \text{transcendence degree of } K' \text{ over } K;
$$
$$
s(v'/v) = \dim.\mathrm{al},\ k' = \text{transcendence degree of } k' \text{ over } k;
$$
$$
r(v'/v) = r(\Gamma'/\Gamma) = \text{rational rank of } \Gamma'/\Gamma,
$$

if the right-hand sides are finite; otherwise, we shall make the convention that $d(K'/K) = +\infty$ (resp. $s(v'/v) = +\infty, r(v'/v) = +\infty$).

#### Theorem 1 {#ac-vi-s10-thm-1 .statement}

*Let $x_1, \ldots, x,$ be elements of the ring of $v'$ whose canonical images $\overline{x}_i$ in $k'$ are algebraically independent over $k$ and $y_1, \ldots, y_r$ elements of $K'$ such that the canonical images of the $v'(y_j)$ in $\Gamma'/\Gamma$ are linearly independent over $\mathbf{Z}$. Then the $r+s$ elements $x_1, \ldots, x, y_1, \ldots, y_r$ of $K'$ are algebraically independent over $K$; the restriction of $v'$ to $K(x_1, \ldots, x, y_1, \ldots, y_r)$ admits $k(\overline{x}_1, \ldots, \overline{x}_s)$ as residue field and*

$$
\Gamma + \mathbf{Z}v'(y_1) + \ldots + \mathbf{Z}v'(y_r)
$$

as *order group*.

Our assertion is obvious if $r+s = 0$. We argue by induction on $r+s$. If $r' \leq r, s' \leq s$ and $r'+s' < r+s$, the induction hypothesis shows that the hypotheses of Theorem 1 hold if $K$ is replaced by $K(x_1, \ldots, x_s, y_1, \ldots, y_{r'})$ and the families $(x_1, \ldots, x_s), (y_1, \ldots, y_r)$ by $(x_{s'+1}, \ldots, x_s), (y_{r'+1}, \ldots, y_r)$. The problem is therefore reduced to one of the two following cases:

(a) There is an element $x$ in the ring $v'$ such that $\overline{x}$ is transcendental over $k$; then it is necessary to show that $x$ is transcendental over $K$ and that the restriction of $v'$ to $K(x)$ admits $k(\overline{x})$ as residue field and $\Gamma$ as order group.

(b) There is an element $y$ in $K'$ such that the relations $nv'(y) \in \Gamma$ and $n \in \mathbf{Z}$ imply $n = 0$; it is necessary to show that $y$ is transcendental over $K$ and that the restriction of $v'$ to $K(y)$ admits $k$ as residue field and $\Gamma + \mathbf{Z}v'(y)$ as order group.

Now Proposition 1 of § 8, no. 1 shows that $x$ (resp. $y$) cannot be algebraic over $K$. The other assertions of (a) (resp. (b)) follow immediately by Proposition 2 (resp. Proposition 1) of no. 1.

#### Corollary 1 {#ac-vi-s10-thm-1-cor-1 .statement}

*The inequality*

$$
s(v'/v) + r(v'/v) \leq d(K'/K)
$$

*holds.*

*Further, if $K'$ is a finitely generated extension of $K$ and equality holds in (9), then $\Gamma'/\Gamma$ is a finitely generated $\mathbf{Z}$-module and $k'$ is a finitely generated extension of $k$.*

Let $r$ and $s$ be natural numbers such that $r \leq r(v'/v)$ and $s \leq s(v'/v)$; we show that $r+s \leq d(K'/K)$ and this will prove (9). By hypothesis there exist elements $x_1, \ldots, x, y_1, \ldots, y$, of $K'$ which satisfy the hypotheses of Theorem 1.

They are therefore algebraically independent over $K$, which shows the inequality $r + s < d(K'/K)$.

If $K'$ is a finitely generated extension of $K$, $d(K'/K)$ is finite, hence $s(v'/v)$ and $r(v'/v)$ are also finite; we denote them by $s$ and $r$. There exist elements $x_1, \ldots, x_s, y_1, \ldots, y_r$ of $K'$ which satisfy the hypotheses of Theorem 1. If $r + s = d(K'/K)$, these elements form a transcendence basis of $K'$ over $K$ and $K'$ is therefore a finite algebraic extension of $K'' = K(x_1, \ldots, y_r)$. Let $\Gamma''$ and $k''$ be the order group and residue field of the restriction of $v'$ to $K''$. By Theorem 1, $\Gamma''/\Gamma$ is a finitely generated $\mathbf{Z}$-module and $k''$ is a finitely generated pure extension of $k$. On the other hand, as $K'$ is a finite algebraic extension of $K$, $\Gamma'/\Gamma$ is a finite group and $k'$ is a finite algebraic extension of $k''$ (\S 8, no. 1, Lemma 2). This proves the corollary.

#### Corollary 2 {#ac-vi-s10-thm-1-cor-2 .statement}

*Let h and h' be the heights of v and v'. Then*
$$
s(v'/v) + h' \leq d(K'/K) + h.
$$
By Proposition 3, $h' \leq r(v'/v) + h$.

#### Corollary 3 {#ac-vi-s10-thm-1-cor-3 .statement}

*Suppose that $K'$ is a finitely generated extension of $K$, that $\Gamma$ is isomorphic to $\mathbf{Z}^{h'}$ (ordered lexicographically) and there is equality in formula (10). Then $\Gamma'$ is isomorphic to $\mathbf{Z}^{h'}$ (ordered lexicographically) and $k'$ is a finitely generated extension of $k$.*

If there is equality in (10), there is equality in (9), whence the fact that $k'$ is a finitely generated extension of $k$ and that $\Gamma''$ is a finitely generated $\mathbf{Z}$-module. Further, comparing (9) and (10), it is seen that $h' - h = r(\Gamma'/\Gamma)$, whence $h' = r(\Gamma')$ and Proposition 4 (no. 2) then shows that $\Gamma'$ is isomorphic to $\mathbf{Z}^{h'}$ ordered lexicographically.

#### Corollary 4 {#ac-vi-s10-thm-1-cor-4 .statement}

*Suppose that v is improper (in which case $k = K$). Then*
$$
h(\Gamma') + d(k'/K) \leq r(\Gamma') + D(k'/K) \leq d(K'/K).
$$
*If, in particular, v' is of height 1, then*
$$
d(k'/K) \leq d(K'/K) - 1;
$$
*further, if $K'$ is a finitely generated extension of $K$ and there is equality in (12), then $v'$ is a discrete valuation and $k'$ is a finitely generated extension of $K$.*

It is a series of special cases of Corollaries 1, 2, 3.

### Exercises {#ac-vi-s10-exercises}

See the [exercises for § 10](exercises/s10/).
