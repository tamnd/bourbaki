---
book: ac
book_title: Commutative Algebra
chapter: III
chapter_title: GRADUATIONS. FILTRATIONS AND TOPOLOGIES
section: 2
section_title: General results on filtered rings and modules
lang: en
source: ac-i-vii
book_pages: 162-195, 233-245
pdf_pages: 0182-0215, 0253-0265
extraction: ocr
subsections:
    - "no": 1
      title: FILTERED RINGS AND MODULES
      page: 162
      pdf_page: 182
    - "no": 2
      title: THE ORDER FUNCTION
      page: 165
      pdf_page: 185
    - "no": 3
      title: THE GRADED MODULE ASSOCIATED WITH A FILTERED MODULE
      page: 165
      pdf_page: 185
    - "no": 4
      title: HOMOMORPHISMS COMPATIBLE WITH FILTRATIONS
      page: 169
      pdf_page: 189
    - "no": 5
      title: THE TOPOLOGY DEFINED BY A FILTRATION
      page: 170
      pdf_page: 190
    - "no": 6
      title: COMPLETE FILTERED MODULES
      page: 173
      pdf_page: 193
    - "no": 7
      title: LINEAR COMPACTNESS PROPERTIES OF COMPLETE FILTERED MODULES
      page: 176
      pdf_page: 196
    - "no": 8
      title: THE LIFT OF HOMOMORPHISMS OF ASSOCIATED GRADED MODULES
      page: 177
      pdf_page: 197
    - "no": 9
      title: THE LIFT OF FAMILIES OF ELEMENTS OF AN ASSOCIATED GRADED MODULE
      page: 179
      pdf_page: 199
    - "no": 10
      title: 'APPLICATION: EXAMPLES OF NOETHERIAN RINGS'
      page: 183
      pdf_page: 203
    - "no": 11
      title: COMPLETE m-ADIC RINGS AND INVERSE LIMITS
      page: 185
      pdf_page: 205
    - "no": 12
      title: THE HAUSDORFF COMPLETION OF A FILTERED MODULE
      page: 187
      pdf_page: 207
    - "no": 13
      title: THE HAUSDORFF COMPLETION OF A SEMI-LOCAL RING
      page: 192
      pdf_page: 212
statements: 57
exercises: 13
content_sha256: c26bf20a582aa742f29736d90586757c3c9eeda4b62c48ac6556a17b97892062
---

## § 2. GENERAL RESULTS ON FILTERED RINGS AND MODULES

### 1. FILTERED RINGS AND MODULES

#### Definition 1 {#ac-iii-s2-def-1 .statement}

An increasing (resp. decreasing) sequence $(G_n)_{n \in \mathbf{Z}}$ of subgroups of a group $G$ is called an increasing (resp. decreasing) filtration on $G$.
A group with a filtration is called a filtered group.

If $(G_n)_{n \in \mathbf{Z}}$ is an increasing (resp. decreasing) filtration on a group $G$ and we write $G'_n = G_{-n}$, clearly $(G'_n)_{n \in \mathbf{Z}}$ is a decreasing (resp. increasing) filtration on $G$. We may therefore restrict our study to decreasing filtrations and hence forth when we speak of a filtration, we shall mean a decreasing filtration, unless otherwise stated.

Given a decreasing filtration $(G_n)_{n \in \mathbf{Z}}$ on a group $G$, clearly $\bigcap_{n \in \mathbf{Z}} G_n$ and $\bigcup_{n \in \mathbf{Z}} G_n$ are subgroups of $G$; the filtration is called separated if $\bigcup_{n \in \mathbf{Z}} G_n$ is reduced to the identity element and exhaustive if $\bigcup_{n \in \mathbf{Z}} G_n = G$.

#### Definition 2 {#ac-iii-s2-def-2 .statement}

Given a ring $A$, a filtration $(A_n)_{n \in \mathbf{Z}}$ over the additive group $A$ is called compatible with the ring structure on $A$ if

(1)
$$
A_m A_n \subset A_{m+n} \quad \text{for} \quad m \in \mathbf{Z}, \quad n \in \mathbf{Z}
$$

(2)
$$
1 \in A_0.
$$
The ring $A$ with this filtration is then called a filtered ring.

Conditions (1) and (2) show that $A_n$ is a subring of $A$ and the $A_n$ (left and right) $A_0$-modules. The set $B = \bigcup_{n \in \mathbf{Z}} A_n$ is a subring of $A$ and the set $n = \bigcap_{n \in \mathbf{Z}} A_n$, a two-sided ideal of $B$; for if $x \in n$ and $a \in A_k$ for all $k \in \mathbf{Z}$, $x \in A_{k-p}$, whence $ax \in A$, and $xa \in A$, by (1); therefore $ax \in n$ and $xa \in n$.

An important particular case is that in which $A_n = A$; then $A_n = A$ for $n \leq 0$ and all the $A_n$ are two-sided ideals of $A$.

#### Definition 3 {#ac-iii-s2-def-3 .statement}

Let $A$ be a filtered ring, $(A_n)_{n \in \mathbf{Z}}$ its filtration and $E$ an $A$-module. A filtration $(E_n)_{n \in \mathbf{Z}}$ on $E$ is called compatible with its module structure over the filtered ring $A$ if
$$
A_m E_n \subset E_{m+n} \quad \text{for} \quad m \in \mathbf{Z}, \quad n \in \mathbf{Z}.
$$
The $A$-module $E$ with this filtration is called a filtered module.

The $E_n$ are all $A_n$-modules; if $B = \bigcup_{n \in \mathbf{Z}} A_n$, clearly $\bigcup_{n \in \mathbf{Z}} E_n$ is a $B$-module and so is $\bigcap_{n \in \mathbf{Z}} E_n$ by the same argument as above for $\bigcap_{n \in \mathbf{Z}} A_n$. If $A_n = A$, all the $E_n$ are submodules of $E$.

Examples

(1) Let $A$ be a graded ring of type $\mathbf{Z}$; for all $i \in \mathbf{Z}$, let $A_{(i)}$ be the subgroup of homogeneous elements of degree $i$ in $A$. Let us write $A_n = \sum_{i \geq n} A_{(i)}$; then it is immediate that $(A_n)$ is an exhaustive and separated decreasing filtration which is compatible with the ring structure on $A$; this filtration is said to be associated with the graduation $(A_{(i)})_{i \in \mathbf{Z}}$ and the filtered ring $A$ is said to be associated with the given graded ring $A$.

Now let $E$ be a graded module of type $\mathbf{Z}$ over the graded ring $A$ and for all $i \in \mathbf{Z}$ let $E_{(i)}$ be the subgroup of homogeneous elements of degree $i$ of $E$. Let us write $E_n = \sum_{i \geq n} E_{(i)}$; then $(E_n)$ is an exhaustive and separated decreasing filtration which is compatible with the module structure on $E$ over the filtered ring $A$; this filtration is said to be associated with the graduation $(E_{(i)})_{i \in \mathbf{Z}}$ and the filtered module $E$ is said to be associated with the given graded module $E$.

(2) Let $A$ be a filtered ring, $(A_n)_{n \in \mathbf{Z}}$ its filtration and $E$ an $A$-module. Let us write $E_n = A_n E$; it follows from (1) that
$$
A_m E_n = A_m A_n E \subset A_{m+n} E = E_{m+n},
$$
and from (2) that $E_0 = E$; then $(E_n)$ is an exhaustive filtration which is compatible with the $A$-module structure on $E$. This filtration is said to be derived from the given filtration $(A_n)$ on $A$; note that it is not necessarily separated,

(3) Let $A$ be a ring and $m$ a two-sided ideal of $A$. Let us write $A_n = m^n$ for $n \geq 0$, $A_n = A$ for $n < 0$; it is immediate that $(A_n)$ is an exhaustive filtration on $A$, called the $m$-adic filtration. Let $E$ be an $A$-module; the filtration $(E_n)$ derived from the $m$-adic filtration on $A$ is called the $m$-adic filtration on $E$; in other words, $E_n = m^n E$ for $n \geq 0$ and $E_n = E$ for $n < 0$.

If $A$ is commutative and $B$ is an $A$-algebra, $n = mB$ is a two-sided ideal of $B$ and, for every $B$-module $F$, $n^k F = m^k F$ and hence the $n$-adic filtration on $F$ coincides with the $m$-adic filtration (if $F$ is considered as an $A$-module).

(4) If $A$ is a filtered ring and $(A_n)$ its filtration, the left $A$-module $A_n$ is a filtered $A$-module with the filtration $(A_n)$. On the other hand, clearly $(A_n)$ is a filtration which is compatible with the ring structure on the opposite ring $A^0$ and $A_n$ is a filtered (left) $A^0$-module with the filtration $(A_n)$.

(5) On a ring $A$ the sets $A_n$ such that $A_n = 0$ for $n > 0$, $A_n = A$ for $n \leq 0$ form what is called a trivial filtration associated (Example 1) with the trivial graduation on $A$; on an $A$-module $E$, every filtration $(E_n)$ consisting of sub-$A$-modules is then compatible with the module structure on $E$ over the filtered ring $A$. Then it is possible to say that every filtered commutative group $G$ is a filtered $\mathbf{Z}$-module, if $\mathbf{Z}$ is given the trivial filtration.

Let $G$ be a filtered group and $(G_n)_{n \in \mathbf{Z}}$ its filtration; clearly, for every subgroup $H$ of $G$, $(H \cap G_n)_{n \in \mathbf{Z}}$ is a filtration said to be induced by that on $G$; it is exhaustive (resp. separated) if that on $G$ is. Similarly, if $H$ is a normal subgroup of $G$, the family $((H.G_n)/H)_{n \in \mathbf{Z}}$ is a filtration on the group $G/H$, called the quotient under $H$ of the filtration on $G$; it is exhaustive if $(G_n)$ is. If $G'$ is another filtered group and $(G'_n)_{n \in \mathbf{Z}}$ its filtration, $(G_n \times G'_n)$ is a filtration on $G \times G'$ called the product of the filtrations on $G$ and $G'$, which is exhaustive (resp. separated) if $(G_n)$ and $(G'_n)$ are.

Now let $A$ be a filtered ring and $(A_n)$ its filtration; on every subring $B$ of $A$, clearly the filtration induced by that on $A$ is compatible with the ring structure on $B$. If $b$ is a two-sided ideal of $A$, the quotient filtration on $A/b$ of that on $A$ is compatible with the structure of this ring, for
$$
(A_n + b)(A_m + b) \subset A_{n+m} + b.
$$
If $A'$ is another filtered ring, the product filtration on $A \times A'$ is compatible with the structure of this ring.

Finally let $E$ be a filtered $A$-module and $(E_n)$ its filtration; on every submodule $F$ of $E$, the filtration induced by that on $E$ is compatible with the $A$-module structure on $F$ and, on the quotient module $E/F$, the quotient filtration of that on $E$ is compatible with the $A$-module structure, as
$$
A_n(F + E_m) \subset F + A_n E_m \subset F + E_{m+n}.
$$

If E' is another filtered A-module, the product filtration on E × E' is compatible with its A-module structure. If the filtrations on E and E' are derived from that on A (Example 2), so is their product filtration.

### 2. THE ORDER FUNCTION

Let A be a filtered ring, E a filtered A-module and (E_n) the filtration of E. For all x ∈ E let v(x) denote the *least* upper bound in R of the set on integers n ∈ Z such that x ∈ E_n. Then the following equivalences hold:

$$
\begin{cases}
v(x) = -∞ \Leftrightarrow x \notin \bigcup_{n \in \mathbf{Z}} E_n \\
v(x) = p \Leftrightarrow x \in E_p \text{ and } x \notin E_{p+1} \\
v(x) = +∞ \Leftrightarrow x \in \bigcap_{n \in \mathbf{Z}} E_n
\end{cases}
$$

The mapping v : E → \overline{\mathbf{R}} is called the order function of the filtered module E. If v is known then so are the E_n, for E_n is the set of x ∈ E such that v(x) ≥ n; the fact that the E_n are additive subgroups of E implies the relation

$$
v(x - y) \geq \inf(v(x), v(y)).
$$

The above definition applies in particular to the filtered A-module A; let w be its order function. It follows from equation (3) of no. 1 that for a ∈ A and x ∈ E,

$$
v(ax) \geq w(a) + v(x)
$$
whenever the right-hand side is defined; in particular, for a ∈ A and b ∈ A,

$$
w(ab) \geq w(a) + w(b)
$$
whenever the right hand side is defined.

The *order function* is defined similarly on a filtered group G which is not necessarily commutative; the corresponding relation to (5) is then written

$$
v(yx^{-1}) = v(xy^{-1}) \geq \inf(v(x), v(y)).
$$

### 3. THE GRADED MODULE ASSOCIATED WITH A FILTERED MODULE

Let G be a commutative group (written additively) and (G_n) a filtration on G. Let us write

$$
\begin{align*}
\operatorname{gr}_n(G) &= G_n / G_{n+1} \quad \text{for } n \in \mathbf{Z} \\
\operatorname{gr}(G) &= \bigoplus_{n \in \mathbf{Z}} \operatorname{gr}_n(G).
\end{align*}
$$

The commutative group gr(G) is then a graded group of type $\mathbf{Z}$, called the *graded group associated* with the filtered group G, the homogeneous elements of degree $n$ of gr(G) being those of $\mathrm{gr}_n(G)$.

Now let A be a filtered ring, (A,) its filtration, E a filtered A-module and (E_n) its filtration. For all $p \in \mathbf{Z}$, $q \in \mathbf{Z}$, a mapping

$$
\mathrm{gr}_p(A) \times \mathrm{gr}_q(E) \to \mathrm{gr}_{p+q}(E)
$$

is defined as follows: given $a \in \mathrm{gr}_p(A)$, $\xi \in \mathrm{gr}_q(E)$, two representatives $a, a'$ of $a$ and two representatives $x, x'$ of $\xi$, $ax \in E_{p+q}$, $a'x' \in E_{p+q}$ and $ax \equiv a'x'$ (mod. $E_{p+q+1}$), for

$$
ax - a'x' = (a - a')x + a'(x - x')
$$

and $a - a' \in A_{p+1}$ and $x - x' \in E_{q+1}$ and hence our assertion follows from formula (3) of no. 1. We may therefore denote by $\alpha\xi$ the class in

$$
E_{p+1}/E_{p+q+1} = \mathrm{gr}_{p+q}(E)
$$

of the product $ax$ of any representative $a \in a$ and any representative $x \in \xi$. It is immediate that the mapping (9) is *Z-bilinear*; by linearity, we derive a $\mathbf{Z}$-bilinear mapping

$$
\mathrm{gr}(A) \times \mathrm{gr}(E) \to \mathrm{gr}(E).
$$

If this definition is first applied to the case $E = A_0$, the mapping (10) is an internal law of composition on $\mathrm{gr}(A)$, which it is immediately verified is *associative* and has an identity element which is the canonical image in $\mathrm{gr}_0(A)$ of the unit element of A; it therefore defines on $\mathrm{gr}(A)$ a ring structure and the graduation $(\mathrm{gr}_n(A))_{n \in \mathbf{Z}}$ is by definition compatible with this structure. The graded ring $\mathrm{gr}(A)$ (of type $\mathbf{Z}$) thus defined is called the *graded ring associated* with the filtered ring A; it is obviously commutative if A is commutative; $\mathrm{gr}_0(A)$ is a subring of $\mathrm{gr}(A)$. The mapping (10) is on the other hand a $\mathrm{gr}(A)$-module external law on $\mathrm{gr}(E)$, the module axioms being trivially satisfied, and the graduation $(\mathrm{gr}_n(E))_{n \in \mathbf{Z}}$ on $\mathrm{gr}(E)$ is obviously compatible with this module structure. The graded $\mathrm{gr}(A)$-module $\mathrm{gr}(E)$ (of type $\mathbf{Z}$) thus defined is called the *graded module associated* with the filtered A-module E.

*Examples*

#### Example 1 {#ac-iii-s2-n3-exa-1 .statement}

Let A be a commutative ring and $t$ an element of A which is not a divisor of 0. Let us give A the *(t)*-*adic filtration* (no. 1, *Example 3*). Then the associated graded ring $\mathrm{gr}(A)$ is canonically isomorphic to the *polynomial ring* $(A/(t))[X]$. For $\mathrm{gr}_n(A) = 0$ for $n < 0$ and by definition the ring $\mathrm{gr}_0(A)$ is the ring $A/(t)$. We now note that by virtue of the hypothesis on $t$ the relation $at^n \equiv 0$ (mod. $t^{n+1}$) is equivalent to $a \equiv 0$ (mod. $t$); if $\tau$ is the canonical image of $t$ in $\mathrm{gr}_1(A)$, every element of $\mathrm{gr}_n(A)$ may then be written uniquely in the form $\alpha \tau^n$ where $\alpha \in \mathrm{gr}_0(A)$; whence our assertion.

#### Example 2 {#ac-iii-s2-n3-exa-2 .statement}

Let $K$ be a commutative ring, $A$ the ring of formal power series

$$
K[[X_1,\ldots,X_r]]
$$

(*Algebra, Chapter IV, § 5*) and $m$ the ideal of $A$ whose elements are the formal power series with no constant term. Let us give $A$ the $m$-adic *filtration* (no. 1, *Example 3*); if $M_1,\ldots,M_s$ are the distinct monomials in $X_1,\ldots,X_r$ of total degree $n-1$, clearly every formal power series $u$ of total order $\omega(u)\geq n$

*(loc. cit., no. 2)* may be written as $\displaystyle\sum_{k=1}^{s}u_kM_k$, where the $u_k$ belong to $m$; it is **seen** that $m^n$ is the set of formal power series $u$ such that $\omega(u)\geq n$, which shows that $\omega$ is the *orderfunction* for the $m$-adic filtration. Then clearly, for every formal power series $u\in m^n$, there exists a unique *homogeneous polynomial* of degree $n$ in the $X_i$ which is congruent to $u$ mod. $m^{n+1}$, namely the sum of terms of degree $n$ of $u$; we conclude that $\operatorname{gr}(A)$ is canonically isomorphic to the *polynomial ring* $K[X_1,\ldots,X_r]$.

#### Example 3 {#ac-iii-s2-n3-exa-3 .statement}

More generally, let $A$ be a commutative ring, $b$ an ideal of $A$ and $A$ be given the $b$-adic filtration. If we write $B=\operatorname{gr}_0(A)$, $F=\operatorname{gr}_1(A)=b/b^2$, we know (*Algebra, Chapter III*), that the identity mapping of the $B$-module $F$ onto itself can be extended uniquely to a homomorphism $u$ from the *symmetric algebra* $S(F)$ of $F$ to the $B$-algebra $\operatorname{gr}(A)$; it follows from the definition of $\operatorname{gr}(A)$ that $u$ is a *surjective homomorphism of graded algebras*; for $n\geq1$, every element of $\operatorname{gr}_n(A)$ is a sum of classes mod $b^{n+1}$ of elements of the form $y=x_1x_2\cdots x_n$, where $x_i\in b$ $(1\leq i\leq n)$; if $\xi_i$ is the class of $x_i$ mod. $b^2$, clearly the class of $y$ mod. $b^{n+1}$ is the element $u(\xi_1)\cdots u(\xi_n)$, whence our assertion. In particular, every system of generators of the $B$-module $F$ is a system of generators of the $B$-algebra $\operatorname{gr}(A)$.

If now $E$ is an $A$-module and $E$ is given the $b$-adic filtration, it is seen similarly that the graded $\operatorname{gr}(A)$-module $\operatorname{gr}(E)$ is *generated* by $\operatorname{gr}_0(E)=E/bE$. To be precise, the restriction $\phi$ to $\operatorname{gr}(A)\times\operatorname{gr}_0(E)$ of the external law on the $\operatorname{gr}(A)$-module $\operatorname{gr}(E)$ is a $\mathbf{Z}$-bilinear mapping of $\operatorname{gr}(A)\times\operatorname{gr}_0(E)$ to $\operatorname{gr}(E)$; moreover $\operatorname{gr}(A)$ is a $(\operatorname{gr}_0(A),\operatorname{gr}_0(A))$-bimodule and $\operatorname{gr}_0(E)$ a $\operatorname{gr}_0(A)$-module; it is immediately verified that, for $a\in\operatorname{gr}(A)$, $\alpha_0\in\operatorname{gr}_0(A)$, $\xi\in\operatorname{gr}_0(E)$,

$$
\phi(a\alpha_0,\xi)=\phi(a,\alpha_0\xi)
$$

and hence $\phi$ defines a *surjective* $\operatorname{gr}_1(A)$-linear mapping

(11)

$$
\gamma_E:\operatorname{gr}(A)\otimes_{\operatorname{gr}_0(A)}\operatorname{gr}_0(E)\longrightarrow\operatorname{gr}(E)
$$

which is called *canonical*.

#### Example 4 {#ac-iii-s2-n3-exa-4 .statement}

\* Let $K$ be a commutative ring, $\mathfrak g$ a Lie algebra over $K$ and $U$ the enveloping algebra of $\mathfrak g$. An *increasing filtration* $(U_n)_{n\in\mathbf{Z}}$ is defined on $U$ by taking $U_n=\{0\}$ for $n<0$ and denoting by $U_n$, for $n\geq0$ the set of elements of $U$ which can be expressed as a sum of products of at most $n$ elements of $\mathfrak g$, then

U_0 = K and gr(U) is a commutative K-algebra (Lie Groups and Lie Algebras, Chapter I, § 2, no. 6). The canonical mapping of g to gr_1(U) = U_1/U_0 can be extended uniquely to a homomorphism h of the symmetric algebra $S(g)$ of the K-module g to the K-algebra gr(U); the homomorphism h is surjective and, if the K-module g is free, h is bijective (loc. cit., no. 7, Theorem 1).

#### Example 5 {#ac-iii-s2-n3-exa-5 .statement}

Let A be a graded ring of type $\mathbf{Z}$ and E a graded A-module of type $\mathbf{Z}$; let $A_{(i)}$ (resp. $E_{(i)}$) be the subgroup of homogeneous elements of degree i of A (resp. E). Let A and E be given the filtrations associated with their graduations (no. 1, Example 1) and let A' and E' denote the filtered ring and filtered A-module thus obtained. Then it is immediate that the Z-linear mapping $A \to \mathrm{gr}(A')$ which maps an element of $A_{(n)}$ to its canonical image in
$$
\mathrm{gr}_n(A) = \left( \bigoplus_{i \geq n} A_{(i)} \right) / \left( \bigoplus_{i \geq n+1} A_{(i)} \right)
$$
is a graded ring isomorphism. A canonical graded A-module isomorphism $E \to \mathrm{gr}(E')$ is defined similarly.

#### Proposition 1 {#ac-iii-s2-prop-1 .statement}

Let A be a filtered ring, $(A_n)_{n \in \mathbf{Z}}$ its filtration and v its orderfunction. Suppose that $\mathrm{gr}(A)$ is a ring with no divisor of zero. Then, for every ordered pair of elements a, b of the ring $B = \bigcup_{n \in \mathbf{Z}} A_n$, $v(ab) = v(a) + v(b)$.

As $n = \bigcap_{n \in \mathbf{Z}} A_n$ is a two-sided ideal of the ring B, the formula holds if $v(a)$ or $v(b)$ is equal to $+\infty$. If not, $v(a) = r$ and $v(b) = s$ are integers; the classes $\alpha$ of a mod. A, +, and $\beta$ of b mod. A, +_1 are $\neq 0$ by definition, whence by hypothesis $\alpha \beta \neq 0$ in $\mathrm{gr}(A)$ and therefore $ab \notin A_{r+s+1}$, as $ab \in A_{r+s}$,
$$
v(ab) = v(a) + v(b).
$$

#### Corollary {#ac-iii-s2-n3-cor-1 .statement}

Let A be a filtered ring and $(A_n)_{n \in \mathbf{Z}}$ its filtration; let us set $B = \bigcup_{n \in \mathbf{Z}} A_n$, $n = \bigcap_{n \in \mathbf{Z}} A_n$. If the ring $\mathrm{gr}(A)$ has no divisors of zero, neither has the ring $B/n$.
If a and b are elements of B not belonging to n, then $v(a) \neq +\infty$ and $v(b) \neq +\infty$, whence $v(ab) \neq +\infty$ and therefore $ab \notin n$.

Note that the ring A can be an integral domain and the filtration (A,,) exhaustive and separated without $\mathrm{gr}(A)$ being an integral domain (Exercise 2).

#### Remark {#ac-iii-s2-n3-rem-1 .statement}

Let G be a group which is not necessarily commutative with a filtration $(G_n)_{n \in \mathbf{Z}}$ such that $G_{n+1}$ is normal in G, for all $n \in \mathbf{Z}$; again let $\mathrm{gr}_n(G) = G_n/G_{n+1}$. The restricted product of the family $(\mathrm{gr}_n(G))_{n \in \mathbf{Z}}$, that is the subgroup of the product $\prod_{n \in \mathbf{Z}} \mathrm{gr}_n(G)$ consisting of the elements $(\xi_n)$ all of whose components, except at most a finite number, are equal to the identity element, is also called the graded group associated with G and denoted by $\mathrm{gr}(G)$.

### 4. HOMOMORPHISMS COMPATIBLE WITH FILTRATIONS

Let G, G' be two commutative groups (written additively), (G,) a filtration on G and (G'_n) a filtration on G'; a homomorphism h : G → G' is called compatible with the filtrations on G and G' if h(G_n) ⊂ G'_n for all n ∈ Z. The composite homomorphism G, $\xrightarrow{h} G'_n \longrightarrow G'_n/G'_{n+1}$ is zero on G_{n+1} and hence defines by taking quotients a homomorphism h, : G_n/G_{n+1} → G'_n/G'_{n+1}; there is therefore a unique additive group homomorphism gr(h) : gr(G) → gr(G') such that, for all n ∈ Z, gr(h) coincides with h, on gr_n(G) = G_n/G_{n+1}. gr(h) is called the graded group homomorphism associated with h. If G'' is a third filtered group and h' : G' → G'' a homomorphism which is compatible with the filtrations, h' ∘ h is a homomorphism which is compatible with the filtrations and

(12)
$$
\operatorname{gr}(h' \circ h) = \operatorname{gr}(h') \circ \operatorname{gr}(h)
$$

#### Proposition 2 {#ac-iii-s2-prop-2 .statement}

Let G be a filtered commutative group and H a subgroup of G; let H be given the induced filtration and G/H the quotient filtration. If j : H → G is the canonical injection and p : G → G/H the canonical surjection, j and p are compatible with the filtrations and the sequence

(13)
$$
0 \longrightarrow \operatorname{gr}(H) \xrightarrow{\operatorname{gr}(j)} \operatorname{gr}(G) \xrightarrow{\operatorname{gr}(p)} \operatorname{gr}(G/H) \longrightarrow 0
$$
is exact.

The first assertion is obvious; if (G,,) is the filtration on G, then
$$
(H \cap G_n) \cap G_{n+1} = H \cap G_{n+1}
$$
and hence gr(j) is injective; moreover the canonical mapping
$$
G_n \to (H + G_n)/H
$$
is surjective, hence so is gr(p) and gr(p) ∘ gr(j) = 0 by (12). Finally, let $\xi \in G_n/G_{n+1}$ belong to the kernel of gr(p); then there exists x ∈ ξ such that x ∈ H + G_{n+1}; but as G_{n+1} ⊂ G,
$$
G_n \cap (H + G_{n+1}) = (H \cap G_n) + G_{n+1}
$$
and hence x = y + z where y ∈ H ∩ G, and z ∈ G, +_1; this proves that ξ is the class mod. G, +_1 of j(y), in other words it belongs to the image of gr(H) under gr(j).

Note that, given an exact sequence 0 → G' \xrightarrow{u} G \xrightarrow{v} G'' → 0 of filtered commutative groups, where u and v are compatible with the filtrations, the sequence 0 \longrightarrow \operatorname{gr}(G') \xrightarrow{\operatorname{gr}(u)} \operatorname{gr}(G) \xrightarrow{\operatorname{gr}(v)} \operatorname{gr}(G'') \longrightarrow 0 is not necessarily exact (Exercise 4).

If now A and B are two filtered rings and h: A → B a ring homomorphism which is compatible with the filtrations, it is immediately verified that the graded group homomorphism gr(h): gr(A) → gr(B) is also a ring homomorphism. In particular, if A' is a subring of A with the induced filtration, gr(A') is canonically identified with a graded subring of gr(A) (Proposition 2); if b is a two-sided ideal of A and A/b is given the quotient filtration, gr(A/b) is canonically identified with the quotient graded ring gr(A)/gr(b) (Proposition 2).

Finally, let A be a filtered ring, E, F two filtered A-modules and u : E → F an homomorphism compatible with the filtrations. Then it is immediate that gr(u) : gr(E) → gr(F) is a gr(A)-linear mapping and hence a homogeneous homomorphism of degree 0 of graded gr(A)-modules. Moreover, if u' : E → F is another A-homomorphism compatible with the filtrations, so is u + u' and

$$
\operatorname{gr}(u + u') = \operatorname{gr}(u) + \operatorname{gr}(u').
$$

Remarks

(1) Clearly filtered ring homomorphisms (resp. homomorphisms of filtered modules over a given filtered ring A) compatible with the filtrations can be taken as morphisms for the filtered ring structure (resp. filtered A-module structure) (Set Theory, Chapter IV, § 2, no. 1).

(2) Let E and F be two modules over a filtered ring A and let them have the filtrations derived from the filtration (A_n) on A (no. 1, Example 2). Then every A-linear mapping u : E → F is compatible with the filtrations, since

$$
u(A_nE) = A_nu(E) \subset A_nF.
$$

(3) Note that a filtered A-module homomorphism u : E → F which is compatible with the filtrations may satisfy gr(u) = 0 without being zero; this is so for example of the endomorphism x ↦ nx of the additive group $\mathbf{Z}$ with the (n)-adic filtration (for any integer n > 1). The relation gr(u) = gr(v) for two homomorphisms u, v of E to F, compatible with the filtrations, does not therefore imply necessarily u = u.

(4) The definitions at the beginning of this no. extend immediately to two groups G, G', which are not necessarily commutative and are filtered by subgroups $G_n, G'_n$ such that $G_{n+1}$ (resp. $G'_{n+1}$) is normal in G, (resp. $G'_n$). Proposition 2 is also valid with the same hypotheses on the G, and assuming that H is invariant in G, the proof remaining unchanged except for notation.

### 5. THE TOPOLOGY DEFINED BY A FILTRATION

Let G be a group filtered by a family $(G_n)_{n \in \mathbf{Z}}$ of normal subgroups of G. There exists a unique topology on G which is compatible with the group structure and for which the G, constitute a fundamental system of neighbourhoods of the identity element e of G (General Topology, Chapter III, § 1, no. 2, Example); it is called the topology on G defined by the filtration (G,). When we use topological notions concerning a filtered group, we shall mean, unless otherwise stated, with the topology defined by the filtration. Note that the G,, being subgroups of G, are both open and closed (General Topology, Chapter III, § 2, no. 1, Corollary to Proposition 4).

As each G, is normal in G, the entourages of the left and right uniformities on G coincide; we deduce that G admits a Hausdorff completion group $\hat{G}$ (General Topology, Chapter III, § 3, no. 4, Theorem 1 and no. 1, Proposition 2).

For every subset M of G, the closure of M in G is equal to

$$
\bigcap_{n \in \mathbf{Z}} (M . G_n) = \bigcap_{n \in \mathbf{Z}} (G_n . M)
$$

(General Topology, Chapter III, § 3, no. 1, formula (1)); in particular $\bigcap_{n \in \mathbf{Z}} G$, is the closure of $\{e\}$; thus it is seen that for the topology on G to be Hausdorff it is necessary and sufficient that the filtration (G,) be separated. For the topology on G to be discrete, it is necessary and sufficient that there exist $n \in \mathbf{Z}$ such that $G_+ = \{e\}$ (in which case $G_m = \{e\}$ for $m \geq n$); then the filtration (G,) is called discrete.

Since the Hausdorff group associated with G is $H = G / \left( \bigcap_{n \in \mathbf{Z}} G_n \right)$, the associated graded groups gr(G) and gr(H) (if H is given the quotient filtration) are canonically identified.

Not let G' be another filtered group and $u : G \to G'$ a homomorphism compatible with the filtrations; the definition of the topologies on G and G' shows immediately that $u$ is continuous (*). If H is a subgroup (resp. normal subgroup) of G, the topology induced on H by that on G (resp. the quotient topology with respect to H of that on G) is the topology on H (resp. G/H) defined by the filtration induced by that on G (resp. quotient topology of that on G). The product topology of those on G and G' is the topology defined by the product of filtrations on G and G'.

Let v be the order function (no. 2) on G. The hypothesis on the G, implies that $v(xy x^{-1}) = v(y)$ and hence $v(xy^{-1}) = v(yx^{-1}) = v(x^{-1}y) = v(y^{-1}x)$ for all x, y in G. Let $\rho$ be a real number such that $0 < \rho < 1$ (for example take

(*) Throughout this chapter we shall use the words "continuous homomorphism" in the sense of what is called "continuous representation" in General Topology, Chapter III, § 2, no. 8; the word "homomorphism" will never be used in the sense of General Topology, Chapter III, § 2, no. 8, Definition 1; for this notion we shall always use the term "strict morphism" in order to avoid any confusion.

$\rho = 1/e$ and let $d(x, y) = \rho^{v(xy^{-1})}$ for all $x, y$ in G. Then $d(x, x) = 0, d(x, y) = d(y, x)$ and inequality (5') of no. 2 gives

$$
(15) \quad d(x, y) \leq \sup(d(x, z), d(y, z))
$$

for all $x, y, z$ in G, which implies the triangle inequality

$$
d(x, y) \leq d(x, z) + d(y, z).
$$

Thus $d$ is a *pseudometric* on G which is invariant under left and right translations and G, is the set of $x \in G$ such that $d(e, x) < \rho^n$; the uniform structure defined by $d$ is then the uniform structure on the topological group G. If G is Hausdorff, G is a *zero-dimensional* metrizable topological space (*General Topology*, Chapter IX, § 6, no. 4); $d$ is a *distance* on G if also the filtration (G,) is exhaustive.

Given a topological ring A, recall that a *left topological A-module* is an A-module E with a topology compatible with its additive group structure and such that the mapping $(a, x) \mapsto ax$ from $A \times E$ to E is continuous (*General Topology*, Chapter III, § 6, no. 6).

#### Proposition 3 {#ac-iii-s2-prop-3 .statement}

*Let A be ajiltered ring, (A,) itsjiltration, B the subring $\bigcup_{n \in \mathbf{Z}} A_n$ of A, E ajiltered B-module, (E_n) itsjiltration and F the sub-B-module $\bigcup_{n \in \mathbf{Z}} E_n$ of E. Then the mapping $(a, x) \mapsto ax$ from $B \times F$ to F is continuous.*

Let $a, \in B, x_0 \in F$; there exists by hypothesis integers $r, s$ such that $a_0 \in A_r$ and $x_0 \in E_s$. The relation

$$
ax - a_0x_0 = (a - a_0)x_0 + a_0(x - x_0) + (a - a_0)(x - x_0)
$$

shows that if $a - a_0 \in A_i$ and $x - x_0 \in E_j$, $ax - a_0x_0$ belongs to

$$
E_{i+s} + E_{j+r} + E_{i+j}.
$$

Then, given an integer $n$, $ax - a_0x_0 \in E_n$ provided $i \geq n - s, j \geq n - r$ and $i + j \geq n$, that is so long as $i$ and $j$ are sufficiently large.

#### Corollary {#ac-iii-s2-n5-cor-1 .statement}

*The ring B is a topological ring and the B-module F a topological B-module.*

The first assertion is obtained by applying Proposition 3 to $F = B$.

It is seen in particular that a filtered ring A whose filtration is *exhaustive* is a topological ring; if this is so every filtered A-module whose filtration is *exhaustive* is a topological A-module.

#### Proposition 4 {#ac-iii-s2-prop-4 .statement}

*Let A be a commutative ringjiltered by an exhaustivejiltration (A,) and p an ideal of A. Suppose that the ideal $\operatorname{gr}(p) = \bigoplus_{n \in \mathbf{Z}} (p \cap A_n)/(p \cap A_{n+1})$ of the ring $\operatorname{gr}(A)$ is prime. Then the closure of p in A is a prime ideal.*

We know that gr(A/p) is isomorphic to gr(A)/gr(p) (no. 4, Proposition 2) and hence an integral domain; we conclude that $A / \bigcap_{n \in \mathbf{Z}} (p + A_n)$ is an integral domain (no. 3, Corollary to Proposition 1). Then the closure $\bigcap_{n \in \mathbf{Z}} (p + A_n)$ of $p$ is a prime ideal.

Let $A$ be a ring and $m$ a two-sided ideal of $A$; the topology defined on $A$ by the $m$-adic filtration (no. 1, Example 3) is called the *m-adic topology*; as the *m*-adic filtration is exhaustive, $A$ is a topological ring with this topology (Corollary to Proposition 3). Similarly, for every $A$-module $E$, the topology defined by the $m$-adic filtration is called the *m-adic topology* on $E$; $E$ is a topological $A$-module under this topology.

Let $m'$ be another two-sided ideal of $A$; for the $m'$-adic topology on $A$ to be *finer* than the $m$-adic topology, it is necessary and sufficient that there exist an integer $n > 0$ such that ${m'}^n \subset m$; the condition is necessary and, if it is fulfilled, ${m'}^{hn} \subset m^h$ for all $h > 0$ and hence the condition is sufficient. If $A$ is a *commutative Noetherian ring*, it amounts to the same to say that $V(m) \subset V(m')$ in the prime spectrum of $A$ (Chapter II, § 4, no. 3, Corollary 2 to Proposition 11 and § 2, no. 6, Proposition 15).

### 6. COMPLETE FILTERED MODULES

#### Proposition 5 {#ac-iii-s2-prop-5 .statement}

*Let $G$ be a filtered group whose filtration $(G,)$ consists of invariant subgroups of $G$. The following conditions are equivalent:*

(a) $G$ is a complete topological group.

(b) *The associated Hausdorff group* $G' = G / (\bigcap_{n \in \mathbf{Z}} G_n)$ *is complete*.

(c) *Every Cauchy sequence in $G$ is convergent*.

*If $G$ is commutative and written additively, these conditions are also equivalent to the following:*

(d) *Every family* $(x_\lambda)_{\lambda \in L}$ *of elements of $G'$ which converges to 0 with respect to the filter $\mathcal{F}$ of complements of finite subsets of $L$ is summable in $G'$*.

For a filter on $G$ to be a Cauchy filter (resp. a convergent filter), it is necessary and sufficient that its image under the canonical mapping $G \to G'$ be a Cauchy (resp. convergent) filter (*General Topology*, Chapter II, § 3, no. 1, Proposition 4); whence first of all the equivalence of (a) and (b); on the other hand, as $G'$ is metrizable, the equivalence of (b) and (c) follows from Proposition 9 of *General Topology*, Chapter IX, § 2, no. 6.

Suppose now that $G$ is commutative. Suppose that $G'$ is complete and let $(x_\lambda)_{\lambda \in L}$ be a family of elements of $G'$ which converge to 0 with respect to $\mathcal{F}$. For every neighbourhood $V'$ of 0 in $G$ which is a subgroup of $G'$, there exists a finite subset $J$ of $L$ such that the condition $\lambda \in L - J$ implies $x_\lambda \in V'$; then $\sum_{\lambda \in H} x_\lambda \in V'$ for every finite subset $H$ of $L$ not meeting $J$, which shows that the family $(x_\lambda)_{\lambda \in L}$ is summable (*General Topology*, Chapter III, § 5, no. 2, Theorem 1).

Conversely, suppose that condition (d) holds and let $(x_n)$ be a Cauchy sequence on $G'$; the family $(x_{n+1} - x_n)$ is then summable and in particular the series with general term $x_{n+1} - x_n$ is convergent and hence the sequence $(x_n)$ is convergent.

Let $G$ be a filtered group whose filtration $(G_r)$ consists of normal subgroups of $G$; the quotient groups $G/G_n$ are *discrete* and hence complete, since the $G_r$ are open in $G$. Let $f_n$ be the canonical mapping $G \to G/G_n$ and for $m \leq n$ let $f_{mn}$ be the canonical mapping $G/G_n \to G/G_m$; $(G/G_n, f_{mn})$ is an inverse system of discrete groups with $\mathbf{Z}$ as indexing set (*General Topology*, Chapter III, § 7, no. 3). Let $\tilde{G}$ be the topological group the inverse limit of this inverse system and for all $n$ let $g_n : \tilde{G} \to G/G_n$ be the canonical mapping; let $f : G \to \tilde{G}$ be the inverse limit of the inverse system of mappings $(f_n)$ such that $f_n = g_n \circ f$ for all $n$; finally, let $j$ be the canonical mapping of $G$ to its Hausdorff completion $\hat{G}$; as the $G/G_n$ are complete, there exists a unique topological group isomorphism $i : \hat{G} \to \tilde{G}$ such that $f = i \circ j$ (*loc. cit.*, Corollary 1 to Proposition 2); we shall call it the *canonical* isomorphism of $\hat{G}$ onto $\tilde{G}$.

Let $H$ be another filtered group whose filtration $(H_r)$ consists of normal subgroups of $H$ and let $u : G \to H$ be a homomorphism compatible with the filtrations (no. 4). Set $\tilde{H} = \lim H/H_n$; for all $n$, $u$ defines by taking quotients a homomorphism $u_n : G/G_n \to H/H_n$ and the $u_n$ obviously form an inverse system of mappings; set $\tilde{u} = \lim u_n$. Moreover let $\hat{H}$ be the Hausdorff completion of $H$ and $ti : \hat{G} \to H$ the homomorphism derived from $u$ by passing to the Hausdorff completions (*General Topology*, Chapter II, § 3, no. 7, Proposition 15). It follows immediately from the definitions that if $\hat{G}$ is identified with $\tilde{G}$ and $\hat{H}$ with $\tilde{H}$ by means of the canonical isomorphisms, $ti$ is identified with $\tilde{u}$. We conclude in particular that, if, for all $n$, $u_n$ is an isomorphism, then $ti$ is an isomorphism of topological groups.

*Examples of complete filtered groups and rings*

#### Example 1 {#ac-iii-s2-n6-exa-1 .statement}

Let $G$ be a complete filtered group. Every *closed* subgroup of $G$ with the induced filtration is complete (*General Topology*, Chapter II, § 3, no. 4, Proposition 8). Every quotient group of $G$ with the quotient filtration is complete (*General Topology*, Chapter IX, § 3, no. 1, *Remark* 1).

#### Example 2 {#ac-iii-s2-n6-exa-2 .statement}

Let $A$ be a filtered commutative ring whose filtration we denote by $(a_n)_{n \in \mathbf{Z}}$; let $A'$ be the ring of formal power series $A[[X_1, \ldots, X_s]]$. For all $e = (e_1, \ldots, e_s) \in \mathbf{N}^s$, we write $|e| = \sum_{i=1}^s e_i$, $X^e = \prod_{i=1}^s X_i^{e_i}$ so that every element $P \in A'$ can be written uniquely $P = \sum_{e \in \mathbf{N}^s} \alpha_{e,P} X^e$ where $\alpha_{e,P} \in A$. For all $n \in \mathbf{Z}$, let $a'_n$ denote the set of $P \in A'$ such that $\alpha_{e,P} \in a_{n-|e|}$ for all $e \in \mathbf{N}^s$; we show that $a'_n$ is an *ideal* of $A'$. Clearly $a'_n$ is an additive subgroup of $A'$; on the other hand, if $P \in a'_n$ and $Q \in A'$, then, for all $e \in \mathbf{N}^s$, $\alpha_{e,PQ} = \sum_{e'+e''=e} \alpha_{e',Q}\alpha_{e'',P}$; as the relation $e' + e'' = e$ implies $|e''| \leq |e|$, $PQ \in a'_n$. Moreover, if $Q \in a'_m$, then, for $e' + e'' = e$, $\alpha_{e',Q}\alpha_{e'',P} \in a_{m-|e'|}a_{n-|e''|} \subset a_{m+n-|e|}$, which proves that $(a'_n)_{n \in \mathbf{Z}}$ is a *filtration* compatible with the ring structure on $A'$ (for obviously $1 \in a'_0$). When in future we speak of $A'$ as a filtered ring, we shall mean, unless otherwise stated, with the filtration (ah). Clearly $\bigcap_{n \in \mathbf{Z}} a'_n$ is the set of formal power series all of whose coefficients belong to $\bigcap_{n \in \mathbf{Z}} a_n$; then, if $A$ is Hausdorff, so is $A'$. If $a_0 = A$, then $a'_0 = A'$.

#### Proposition 6 {#ac-iii-s2-prop-6 .statement}

*With the above notation, suppose that $a_0 = A$ and let $h$ denote the mapping $P \mapsto (\alpha_{e,P})_{e \in \mathbf{N}^s}$. Then $h$ is an isomorphism of the additive topological group $A$ onto the additive topological group $A^{\mathbf{N}^s}$. The polynomial ring $A[X_1, \ldots, X_s]$ is dense in $A'$; if $A$ is complete, so is $A'$.*

Clearly $h$ is bijective; $V_n = h(a'_n)$ is the set of $(a_e) \in A^{\mathbf{N}^s}$ such that $a_e \in a_{n-|e|}$ for all $e \in \mathbf{N}^s$ such that $|e| \leq n$; as these elements $e$ are finite in number, $V_n$ is a neighbourhood of 0 in $A^{\mathbf{N}^s}$. Conversely, if $V$ is a neighbourhood of 0 in $A^{\mathbf{N}^s}$, there is a finite subset $E$ of $\mathbf{N}^s$ and an integer $v$ such that the conditions $a_e \in a_v$ for all $e \in E$ imply $(a_e) \in V$; if then $n$ is the greatest of the integers $v + |e|$ for $e \in E$, then $h(a'_n) \subset V$, which proves the first assertion of Proposition 6.

Moreover, with $n$ and $E$ defined as above, $h(P - \sum_{e \in E} \alpha_{e,P}X^e) \in V$ for all $P \in A'$, which shows that $A[X_1, \ldots, X_s]$ is dense in $A'$. The last assertion follows from the first and the fact that a product of complete spaces is complete.

Let $m$ be an ideal of $A$ and suppose that $(a_i)$ is the $m$-adic filtration; then, if $n$ is the ideal of $A'$ generated by $m$ and the $X_i$ ($1 \leq i \leq s$), the filtration $(a_i)$ is the $n$-adic filtration. For clearly, for all $k \geq 0$, $n^k$ is generated by the elements $aX^e$ such that $a \in m^{k-|e|}$ for all $e \in \mathbf{N}^s$ such that $|e| \leq k$, whence $n^k \subset a \&$. Let us prove conversely that $a'_k \subset n^k$. For all $P \in a'_k$, $P = P' + P''$, where $P' = \sum_{|e| < k} \alpha_{e,P}X^e$, $P'' = \sum_{|e| \geq k} \alpha_{e,P}X^e$. Clearly it is possible to write $P'' = \sum_{|e|=k} X^e Q_e$, where the $Q_e$ are elements of $A'$, whence $P'' \in n^k$; on the other hand, clearly $\alpha_{e,P}X^e \in n^k$ for all $e \in \mathbf{N}^s$, whence $P' \in n^k$. Then $n^k = a'_k$.

#### Corollary {#ac-iii-s2-n6-cor-1 .statement}

*Let $A$ be a commutative ring,

$$
A' = A[[X_1, \ldots, X_s]]
$$

*the ring of formal power series in $s$ indeterminates over $A$ and $n$ the ideal of $A'$ consisting of the formal power series with no constant term. The ring $A'$ is Hausdorff and complete* with the n-adic topology and the polynomial ring $A[X_1, \ldots, X_s]$ is everywhere dense in $A'$.

It is sufficient to apply what has just been said to the case $m = \{0\}$.

### 7. LINEAR COMPACTNESS PROPERTIES OF COMPLETE FILTERED MODULES

Recall that, if E is an A-module, an affine subset (or an affine linear variety) of E is any subset F which is empty or of the form $a + M$, where $a \in E$ and M is a submodule of E called the direction of F (Algebra, Chapter II, § 9, nos. 1 and 3).

#### Proposition 7 {#ac-iii-s2-prop-7 .statement}

Let A be a filtered ring, E a filtered A-module and $(E_n)$ filtration of E; suppose that $E_0 = E$, that the $E_n$ are submodules of E, that the A-modules $E/E_n$ are Artinian and finally that the topological group E is Hausdorff and complete. Then the intersection of a decreasing sequence of non-empty closed affine subsets of E is non-empty.

We have seen in no. 6 that, since E is Hausdorff and complete, it is identified with $\tilde{E} = \lim_{\leftarrow} E/E_n$. Let $(W_p)$ be a decreasing sequence of non-empty closed affine subsets of E and, for all $n \geq 0$, let $W_{p,n}$ be the canonical image of $W_p$ in $E/E_n$; we are going to construct a sequence $x = (x_n) \in \tilde{E}$ such that $x_n \in W_{p,n}$ for all $p$ and all $n$; hence $x \in W_p + E_n$ for all $p$ and all $n$ and, as the $W_p$ are closed, $x \in W_p$ for all $p$ (no. 5), which will prove the proposition.

As $E/E_0 = 0$, we shall take $x_0 = 0$. Suppose that the $x_i$ are defined for $0 \leq i \leq n - 1$ and let $W'_{p,n}$ be the set of elements of $W_{p,n}$ whose canonical image in $E/E_{n-1}$ is $x_{n-1}$; as $x_{n-1} \in W_{p,n-1}$ and $W_{p,n-1}$ is the canonical image of $W_{p,n}$, $W'_{p,n}$ is non-empty and is obviously an affine subset of $E/E_n$; moreover the sequence $(W'_{p,n})_{p \in \mathbf{N}}$ is decreasing. As $E/E_n$ is Artinian, this sequence is stationary (otherwise the sequence of submodules of $E/E_n$ which are the directions of the $W'_{p,n}$ would be strictly decreasing, which is absurd). It is sufficient then to take $x_n$ to be an element of $\bigcap_{p \in \mathbf{N}} W'_{p,n}$ and the construction of $(x_n)$ can then be performed by induction.

#### Proposition 8 {#ac-iii-s2-prop-8 .statement}

Suppose that A and E satisfy the hypotheses of Proposition 7. Let $(F_p)$ be a decreasing sequence of closed submodules of E such that $\bigcap F_p = 0$. Then, for every neighbourhood V of 0 in E, there exists $p$ such that $F_p \subset V$ (in other words, the base of the filter $(F_p)$ converges to 0).

We may assume that V is one of the $E_n$, in which case $E/V$ is Artinian. Let us write $F'_p = (F_p + V)/V$; as the $F'_p$ form a decreasing sequence of submodules of $E/V$, there exists an integer $j$ such that $F'_p = F'_j$ for all $p > j$. We shall see that $F'_j = \{0\}$, which will complete the proof. Let $x \in F'_j$ and let W, be the set of elements of F, whose image in $E/V$ is $x$ ($p \geq j$); by definition of j, the W, are non-empty closed affine subsets of E and obviously $W_{p+1} \subset W$;

then it follows from Proposition 7 that there exists an element y belonging to all the W,. As W, $\subset F,$ and $\bigcap_{p \in \mathbf{N}} F_p = \{0\}, y = 0$; since x is the canonical image of y in E/V, $x = 0$ (cf. Exercises 15 to 21).

### 8. THE LIFT OF HOMOMORPHISMS OF ASSOCIATED GRADED MODULES

#### Theorem 1 {#ac-iii-s2-thm-1 .statement}

Let X, Y be two filtered groups whose filtrations $(X_n), (Y_n)$ consist of normal subgroups; let $u : X \to Y$ be a homomorphism compatible with the filtrations.

(i) Suppose that the filtration $(X_n)$ is exhaustive. For $\mathrm{gr}(u)$ to be injective, it is necessary and sufficient that $\bar{u}^{-1}(Y_n) = X_n$ for all $n \in \mathbf{Z}$.

(ii) Suppose that one of the following hypotheses holds: (α) X is complete and Y Hausdorff; (β) Y is discrete. Then, for $\mathrm{gr}(u)$ to be surjective, it is necessary and sufficient that $Y_n = u(X_n)$ for all $n \in \mathbf{Z}$.

(i) To say that the mapping $\mathrm{gr}_n(u)$ is injective means that
$$
X_n \cap \bar{u}^{-1}(Y_{n+1}) \subset X_{n+1}.
$$
This is obviously the case if $(Y_{n+1}) = X_{n+1}$. Conversely, if
$$
X_n \cap \bar{u}^{-1}(Y_{n+1}) \subset X_{n+1}
$$
for all $n$, we deduce by induction on $k$ that $X_{n-k} \cap \bar{u}^{-1}(Y_{n+1}) \subset X_{n+1}$ for all $n \in \mathbf{Z}$ and all $k \geq 0$. As the filtration $(X_n)$ is exhaustive, we see that, for all $n$, $X_n$ is the union of the $X_{n-k}$ ($k \geq 0$), hence $\bar{u}^{-1}(Y_{n+1}) \subset X_{n+1}$ for all $n$ and therefore $X_{n+1} \subset \bar{u}^{-1}(Y_{n+1})$, which completes the proof.

(ii) To say that the mapping $\mathrm{gr}_n(u)$ is surjective means that
$$
Y_n = u(X_n)Y_{n+1}.
$$
This is obviously the case if $Y_n = u(X_n)Y_{n+1}$ for all $n \in \mathbf{Z}$. Let $n$ be an integer and $y$ an element of $Y_n$; we shall define a sequence $(x_k)_{k \geq 0}$ of elements of $X_n$ such that $x_k \in X_n$, $x_{k+1} \equiv x_k \pmod{X_{n+k}}$ and $u(x_k) \equiv y \pmod{Y_{n+k}}$ for all $k \geq 0$. We shall take $x_0$ equal to the identity element of X, which certainly gives $u(x_0) \equiv y \pmod{Y_n}$. Suppose that an $x_k \in X_n$ has been constructed such that $u(x_k) \equiv y \pmod{Y_{n+k}}$; then $(u(x_k))^{-1}y \in Y_{n+k}$; the hypothesis implies that there exists $t \in X_{n+k}$ such that $u(t) \equiv (u(x_k))^{-1}y \pmod{Y_{n+k+1}}$ and hence $u(x_k t) \equiv y \pmod{Y_{n+k+1}}$; it is sufficient to take $x_{k+1} = x_k t$ to carry out the induction. This being so, if Y is discrete, there exists $k \geq 0$ such that $Y_{n+k} = \{e'\}$ (the identity element of Y), whence $u(x_k) = y$ and hence in this case it has been proved that $u(X_n) = Y$, for all $n$. Suppose now that X is complete and Y Hausdorff. As $x_h^{-1} x_k \in X_{n+k}$ for $h \geq k \geq 0$, $(x_k)$ is a Cauchy sequence in $X_n$; as

X_n is closed in X and hence complete, this sequence has at least one limit x in X_n. By virtue of the continuity of u, u(x) is the unique limit of the sequence (u(x_k)) in Y, Y being Hausdorff. But the relations u(x_k) \equiv y (\text{mod. } Y_{n+k+1}) show that y is also a limit of this sequence, whence $u(x) = y$ and it has also been proved that $u(X_n) = Y_n$.

#### Corollary 1 {#ac-iii-s2-thm-1-cor-1 .statement}

*Suppose that X is Hausdorff and its filtration exhaustive. Then, if gr(u) is injective, u is injective.*

Let e, e' be the identity elements of X and Y respectively. Then
$$
\bar{u}^{-1}(e') \subset \bigcap_n \bar{u}^{-1}(Y_n) = \bigcap_n X_n = \{e\}
$$
by hypothesis, whence the corollary.

#### Corollary 2 {#ac-iii-s2-thm-1-cor-2 .statement}

*Suppose that one of the following hypotheses holds :*
$(\alpha)$ *X is complete, Y is Hausdorff and its filtration is exhaustive;*
$(\beta)$ *Y is discrete and its filtration is exhaustive.*
*Then, if gr(u) is surjective, u is surjective.*

In this case $Y = \bigcup_n Y_n = \bigcup_n u(X_n) \subset u(X)$.

#### Corollary 3 {#ac-iii-s2-thm-1-cor-3 .statement}

*Suppose that X and Y are Hausdorff, the filtrations of X and Y exhaustive and X complete. Then, if gr(u) is bijective, u is bijective.*

Let A be a local ring, m its maximal ideal and M an A-module; let A and M be given the *m-adic* filtrations and let gr(A) and gr(M) be the graded ring and the graded gr(A)-module associated with A and M. We have seen (no. 3, Example 3) that the canonical mapping (11) is always *surjective*; we are going to consider the following property of M:
*(GR)* *The canonical mapping*
$$
\gamma_M : \operatorname{gr}(A) \otimes_{\operatorname{gr}_0(A)} \operatorname{gr}_0(M) \to \operatorname{gr}(M)
$$
*is bijective*.

#### Proposition 9 {#ac-iii-s2-prop-9 .statement}

*Let A be a local ring, m its maximal ideal, M, N two A-modules and u : N \to M an A-homomorphism. M and N are given the m-adic filtrations and suppose that: (1) M satisfies property (GR); (2) \operatorname{gr}_0(u) : \operatorname{gr}_0(N) \to \operatorname{gr}_0(M) is injective. Then \operatorname{gr}(u) : \operatorname{gr}(N) \to \operatorname{gr}(M) is injective, N and P = \operatorname{Coker}(u) satisfy property (GR) and $m^n N = \bar{u}^{-1}(m^n M)$ for every integer $n > 0$.*

It is immediately verified that the diagram
$$
\begin{array}{ccc}
\operatorname{gr}(A) \otimes_{\operatorname{gr}_0(A)} \operatorname{gr}_0(N) & \xrightarrow{1 \otimes \operatorname{gr}_0(u)} & \operatorname{gr}(A) \otimes_{\operatorname{gr}_0(A)} \operatorname{gr}_0(M) \\
\downarrow \gamma_N & & \downarrow \gamma_M \\
\operatorname{gr}(N) & \xrightarrow{\operatorname{gr}(u)} & \operatorname{gr}(M)
\end{array}
$$

is commutative. As $\mathrm{gr}_0(A) = A/m$ is a field, the hypothesis implies that $1 \otimes \mathrm{gr}_0(u)$ is injective; as by hypothesis $\gamma_M$ is injective, so is $\gamma_M \circ (1 \otimes \mathrm{gr}_0(u))$. This implies first that $\gamma_N$ is injective and hence bijective and therefore that $\mathrm{gr}(u)$ is injective. The formula $\tilde{u}^1(m^nM) = m^nN$ is then a consequence of Theorem 1 (i).

Also, let us write $N' = u(N)$ and let $j : N' \to M$ be the canonical injection. If $p : M \to P = M/N'$ is the canonical homomorphism, then in the commutative diagram

$$
\begin{array}{ccccccccc}
\mathrm{gr}(A) \otimes \mathrm{gr}_0(N') & \xrightarrow{1 \otimes \mathrm{gr}_0(j)} & \mathrm{gr}(A) \otimes \mathrm{gr}_0(M) & \xrightarrow{1 \otimes \mathrm{gr}_0(p)} & \mathrm{gr}(A) \otimes \mathrm{gr}_0(P) & \to & 0 \\
\downarrow \gamma_{N'} & & \downarrow \gamma_M & & \downarrow \gamma_P & & \\
\mathrm{gr}(N') & \xrightarrow{\mathrm{gr}(j)} & \mathrm{gr}(M) & \xrightarrow{\mathrm{gr}(p)} & \mathrm{gr}(P) & \to & 0
\end{array}
$$

the lower row is exact (no. 4, Proposition 2) and so is the upper row by virtue of Proposition 2 of no. 4 and the fact that $\mathrm{gr}_0(A)$ is a field. Moreover, $\mathrm{gr}(j)$ is injective (no. 4, Proposition 2) and hence $\mathrm{gr}_0(j)$ is injective, The first part of the argument applied to $j$ shows that $\gamma_{N'}$ is bijective; as $\gamma_M$ is also bijective by hypothesis, we conclude that $\gamma_P$ is bijective (Chapter I, § 1, no. 4, Corollary 2 to Proposition 2).

#### Corollary {#ac-iii-s2-n8-cor-1 .statement}

Under the hypotheses of Proposition 9, if we assume also that $N$ is Hausdorf with the $m$-adic filtration, then $u$ is injective.

This follows from the fact that $\mathrm{gr}(u)$ is injective (Corollary 1 to Theorem 1).

\* Remark. Suppose that the hypotheses of Proposition 9 hold and also one of the following conditions:
(1) $m$ is nilpotent;
(2) $A$ is Noetherian and $P$ is ideally Hausdorff (cf. § 5, no. 1);
then $P$ is a flat $A$-module. This follows from the fact that $\gamma_P$ is bijective and § 5, no. 2, Theorem 1 (iv), since $A/m$ is a field. \*

### 9. THE LIFT OF FAMILIES OF ELEMENTS OF AN ASSOCIATED GRADED MODULE

Let $A$ be a filtered commutative ring, $(A_n)_{n \in \mathbf{Z}}$ its filtration and $C$ a subring of $A$, such that $C \cap A_1 = \{0\}$. The restriction to $C$ of the canonical mapping $A_0 \to A_0/A_1 = \mathrm{gr}_0(A)$ is then injective, which allows us to identify $C$ with a submodule of $\mathrm{gr}_0(A)$; this is what we shall usually do in similar cases. If $A_1 \neq A$, and $K$ is any subfield of $A$, then $K \cap A_1 = (0)$ since $K \cap A_1$ is an ideal of $K$ not containing 1 ; then $K$ may be identified with a subfield of $\mathrm{gr}_0(A)$.

#### Proposition 10 {#ac-iii-s2-prop-10 .statement}

Let $A$ be a filtered commutative ring and $(A_n)$ its filtration; suppose that there exists a subring $C$ of $A_0$ such that $C \cap A_n = \{0\}$ and $C$ is identified with a subring of $\mathrm{gr}_0(A)$. Let $(x_i)_{1 \leq i \leq q}$ be a finite family of elements of $A$; suppose that $x_i \in A_n$, for $1 \leq i \leq q$ and let $\xi_i$ be the class of $x_i$ in $\mathrm{gr}_{n_i}(A)$ for $1 \leq i \leq q$.

(i) If the family $(\xi_i)$ of elements of $\mathrm{gr}(A)$ is algebraically free over $C$, the family $(x_i)$ is algebraically free over $C$.

(ii) If the filtration on $A$ is exhaustive and discrete and $(\xi_i)$ is a system of generators of the $C$-algebra $\mathrm{gr}(A)$, then $(x_i)$ is a system of generators of the $C$-algebra $A$.

Let $A'$ be the polynomial algebra $\mathbf{C}[X_1, \ldots, X_q]$ over $\mathbf{C}$; let $A'$ be given the graduation $(A'_n)$ of type $\mathbf{Z}$ where $A_n$ is the set of $\mathbf{C}$-linear combinations of the monomials $X_1^{s(1)} \ldots X_q^{s(q)}$ such that $\sum_{i=1}^q n_i s(i) = n$. Let $u$ be the homomorphism $f \mapsto f(x_1, \ldots, x_q)$ from the $\mathbf{C}$-algebra $A'$ to the $\mathbf{C}$-algebra $A$; by definition, $u(A'_n) \subset A_n$ for all $n \in \mathbf{Z}$ and hence $u$ is compatible with the filtrations $(A')$ being given its filtered ring structure associated with its graded ring structure, cf. no. 1, Example 1). This being so, the hypothesis of (i) means that

$$
\mathrm{gr}(u): A' = \mathrm{gr}(A') \to \mathrm{gr}(A)
$$

is injective; as the filtration on $A'$ is exhaustive and separated, Corollary 1 to Theorem 1 of no. 8 may be applied and $u$ is injective, which proves the conclusion of (i). Similarly, the hypothesis (ii) on the (\&) means that $\mathrm{gr}(u)$ is surjective; as $A$ is discrete and its filtration is exhaustive, Corollary 2 to Theorem 1 of no. 8 may be applied and $u$ is surjective, which proves the conclusion of (ii).

#### Proposition 11 {#ac-iii-s2-prop-11 .statement}

Let $A$ be a complete Hausdorff filtered commutative ring, $C$ a subring of $A_0$ such that $C \cap A_n = 0$ and $(x_i)_{1 \leq i \leq q}$ a finite family of elements of $A$ such that $x_i \in A_{n_i}$ where $n_i > 0$ for $1 \leq i \leq q$; let $\xi_i$ be the class of $x_i$ in $\mathrm{gr}_{n_i}(A)$ for $1 \leq i \leq q$.

(i) There exists a unique $C$-homomorphism $v$ from the algebra of formal power series $A'' = \mathbf{C}[[X_1, \ldots, X_q]]$ to $A$ such that $v(X_i) = x_i$ for $1 \leq i \leq q$.

(ii) If the family $(\xi_i)$ is algebraically free over $C$, the homomorphism $v$ is injective.

(iii) If the filtration on $A$ is exhaustive and the family $(\xi_i)$ is a system of generators of the $C$-algebra $\mathrm{gr}(A)$, the homomorphism $v$ is surjective.

As $n_i \geq 1$ for all $i$, $\sum_{i=1}^q n_i s(i) \geq \sum_{i=1}^q s(i)$ for every monomial $X_1^{s(1)} \ldots X_q^{s(q)}$ and on the other hand $\sum_{i=1}^q n_i s(i) \leq r \cdot \sum_{i=1}^q s(i)$ if $r$ is the greatest of the $n_i$. If $A''_n$ denotes the set of formal power series whose non-zero terms $a_s X_1^{s(1)} \ldots X_q^{s(q)}$ satisfy $\sum_{i=1}^q n_i s(i) \geq n$, it follows from no. 6, Corollary to Proposition 6 that $A''$ is Hausdorff and complete with the exhaustive filtration $(A''_n)$ and that

$$
A' = \mathbf{C}[X_1, \ldots, X_q]
$$

is dense in $A''$; moreover the homomorphism $u$ defined in the proof of Proposition 10 is continuous on $A'$ and can be extended uniquely to a continuous homomorphism $v : A \to A$, since $A$ is Hausdorff and complete (General Topology, Chapter III, § 3, no. 3, Proposition 5), which proves (i); also, $\mathrm{gr}(A'') = \mathrm{gr}(A')$ and $\mathrm{gr}(v) = \mathrm{gr}(u)$; (ii) and (iii) then follow respectively from Corollaries 1 and 2 to Theorem 1 of no. 8 in view of the hypotheses on $A$.

The conclusion of (ii) (resp. (iii)) of the proposition is sometimes expressed by saying that the family $(x_i)$ is formally free over $C$ (resp. a formal system of generators of $A$).

#### Proposition 12 {#ac-iii-s2-prop-12 .statement}

Let $A$ be a filtered ring, $E$ a filtered $A$-module and $(A_n)$ and $(E_n)$ the respective filtrations on $A$ and $E$. Suppose that $A$ is complete and the filtration $(E_n)$ is exhaustive and separated. Let $(x_i)_{i \in I}$ be a finite family of elements of $E$ and for $i \in I$ let $n(i)$ be an integer such that $x_i \in E_{n(i)}$; finally let $\xi_i$ be the class of $x_i$ in $\mathrm{gr}_{n(i)}(E)$. Then, if $(\xi_i)$ is a system of generators of the $\mathrm{gr}(A)$-module $\mathrm{gr}(E)$, $(x_i)$ is a system of generators of the $A$-module $E$.

In the $A$-module $L = A'$, let $L_0$ denote the set $(a_i)$ such that $a_i \in A_{n - n(i)}$ for all $i \in I$; if $p$ and $q$ are the least and greatest of the $n(i)$, then $A^I_{n-q} \supset L_0 \supset A^I_{n-p}$ and the topology defined on $L$ by the definition $(L_n)$ is the same as the product topology; hence $L$ is a complete filtered $A$-module. As $L$ is free, there exists an $A$-linear mapping $u : L \to E$ such that $u((a_i)) = \sum_{i \in I} a_i x_i$ and it is obviously compatible with the filtrations; we must prove that $u$ is surjective and for this it is sufficient, by virtue of Corollary 2 to Theorem 1, no. 8, to show that

$$
\mathrm{gr}(u) : \mathrm{gr}(L) \to \mathrm{gr}(E)
$$

is surjective or also that, for all $x \in E_n$, there exist a family $(a_i)$ such that $a_i \in A_{n-n(i)}$ for all $i \in I$ and $x \equiv \sum_{i \in I} a_i x_i \pmod{E_{n+1}}$. Let $\xi$ be the class of $x$ in $\mathrm{gr}_n(E)$; since the $\xi_i$ generate the $\mathrm{gr}(A)$-module $\mathrm{gr}(E)$, there exist $\alpha_i \in \mathrm{gr}(A)$ such that $\xi = \sum_{i \in I} \alpha_i \xi_i$ and we may assume that $\alpha_i \in \mathrm{gr}_{n-n(i)}(A)$ by replacing if need be $\alpha_i$ by its homogeneous component of degree $n - n(i)$. Then $\alpha_i$ is the image of an element $a_i \in A_{n-n(i)}$ and the family $(a_i)$ has the required property.

#### Corollary 1 {#ac-iii-s2-prop-12-cor-1 .statement}

Let $A$ be a complete filtered ring and $E$ a filtered $A$-module whose filtration is exhaustive and separated. If $\mathrm{gr}(E)$ is a finitely generated (resp. Noetherian) $\mathrm{gr}(A)$-module, then $E$ is a finitely generated (resp. Noetherian) $A$-module.

If $\mathrm{gr}(E)$ is finitely generated, there is a finite system of homogeneous generators and Proposition 12 shows that $E$ is finitely generated. Suppose now that $\mathrm{gr}(E)$ is Noetherian and let $F$ be a submodule of $E$; the filtration induced on $F$ by that on $E$ is exhaustive and separated and $\mathrm{gr}(F)$ is identified with a sub-gr(A)-module of gr(E) (no. 4, Proposition 2) and hence is finitely generated by hypothesis; we conclude that F is a finitely generated A-module and hence E is Noetherian.

#### Corollary 2 {#ac-iii-s2-prop-12-cor-2 .statement}

Let A be a complete Hausdorff filtered ring whose filtration is exhaustive. If gr(A) is a left Noetherian ring, so is A.

It is sufficient to apply Corollary 1 with E = A.

#### Corollary 3 {#ac-iii-s2-prop-12-cor-3 .statement}

Let A be a complete filtered ring, (A,) its filtration, E a Hausdorff filtered A-module, (E_n) its filtration and F a finitely generated submodule of E; suppose that A_∞ = A and E_0 = E.

(i) If, for all k ≥ 0, E_k = E_{k+1} + A_k F, then F = E.
(ii) If it is further supposed that the filtration on E is derived from that on A (no. 1, Example 2), the relation E = E_1 + F implies F = E.

Let ξ_i (1 ≤ i ≤ n) be the classes mod. E_1 of a finite system of generators of F. It follows from the given hypothesis that for all k ≥ 0 every element of gr_k(E) can be expressed in the form $\sum_{i=1}^n \alpha_i \xi_i$ where $\alpha_i \in \mathrm{gr}(A)$; the $\xi_i$ therefore generate the gr(A)-module gr(E), which proves (i) by virtue of Proposition 12. If the filtration on E is derived from that on A, the relation E = E_1 + F implies

$$
E_k = A_k E = A_k E_1 + A_k F = A_k A_1 E + A_k F \subset A_{k+1} E + A_k F \\
= E_{k+1} + A_k F \subset E_k,
$$

whence (ii).

#### Proposition 13 {#ac-iii-s2-prop-13 .statement}

Let A be a ring, m a two-sided ideal of A contained in the Jacobson radical of A and E an A-module. Let A and E be given the m-adic filtrations (no. 1, Example 3). Suppose that one of the following conditions holds:
(a) E is a finitely generated A-module and A is Hausdorff;
(b) m is nilpotent.

For E to be a free A-module, it is necessary and sufficient that E/mE be a free (A/m)-module and that E satisfy property (GR) (no. 8).

If E is a free A-module and $(e_\lambda)$ a basis of E, $m^k E$ is the direct sum of the submodules $m^k e_\lambda$ of E for all $k > 0$ (Algebra, Chapter II, § 3, no. 7, Remark); then $m^k E / m^{k+1} E$ is identified with the direct sum of the $m^k e_\lambda / m^{k+1} e_\lambda$ (Algebra, Chapter 11, § 1, no. 6, Proposition 7). We deduce first (for $k = 0$) that the classes $1 \otimes e_\lambda$ of the $e_\lambda$ in $E / mE = (A / m) \otimes_A E$ form a basis of the (A/m)-module $E / mE$, since the canonical mapping

$$
(m^k / m^{k+1}) \otimes_A (E / mE) \to m^k E / m^{k+1} E
$$

is bijective for all $k \geq 0$; hence $\gamma_E$ is bijective. Note that this part of the proof uses neither condition (a) nor condition (b).

Suppose conversely that the conditions of the statement hold and let $(x_i)_{i \in I}$ be a family of elements of E whose classes mod. $mE$ form a basis of the $(A/m)$-module $E/mE$; let L be the free A-module $A_s^{(I)}$, $(f_i)_{i \in I}$ its canonical basis and $u : L \to E$ the A-linear mapping such that $u(f_i) = x_i$ for all $i \in I$. The hypotheses already imply that $u$ is surjective (Chapter II, § 3, no. 2, Corollary 1 to Proposition 4) and it remains to prove that $u$ is injective. Now, each of the hypotheses (a) and (b) implies that A is Hausdorff and hence so is L with the m-adic filtration, since $m^kL = (m^k)^{(I)}$ (Algebra, Chapter II, § 3, no. 7, Remark) and $\operatorname{gr}(L)$ is identified with $\operatorname{gr}(A) \otimes_{A/m} (L/mL)$ from the first part of the proof; the homomorphism $u$ is compatible with the filtrations and it is possible to write $\operatorname{gr}(u) = \gamma_E \circ v$ where $v$ is the bijection of $\operatorname{gr}(L)$ onto
$$
\operatorname{gr}(A) \otimes_{A/m} (E/mE)
$$
mapping the class off, mod. mM onto $1 \otimes \bar{x}_i$, where $\bar{x}_i$ is the class of $x_i$ mod. $mE$. The hypothesis then implies that $\operatorname{gr}(u)$ is injective and the conclusion follows with the aid of Corollary 1 to Theorem 1, no. 8.

### 10. APPLICATION: EXAMPLES OF NOETHERIAN RINGS

#### Lemma 1 {#ac-iii-s2-lem-1 .statement}

Let A be a graded ring of type $\mathbf{Z}$, whose graduation $(A_n)$ is such that $A_n = 0$ for all $n < 0$ or $A_n = 0$ for all $n > 0$. Let M be a graded A-module of type $\mathbf{Z}$. For M to be a Noetherian A-module, it is necessary and sufficient that every graded submodule of M be finitely generated.

As $n \mapsto -n$ is an automorphism of the group $\mathbf{Z}$, we may restrict our attention to the case $A_n = 0$ for all $n > 0$. Let A' and M' denote the ring A and the module M with the filtrations associated with their respective graduations (no. 1, Example 1), which are exhaustive and separated; the hypothesis on A implies that A' is discrete and hence complete. If E is a sub-A-module of M, the filtered A'-module E' obtained by giving E the induced filtration is Hausdorff and its filtration is exhaustive; moreover $\operatorname{gr}(E')$ is identified with a graded sub-A-module of $M = \operatorname{gr}(M')$ and hence is finitely generated by hypothesis. The conclusion then follows from Corollary 1 to Proposition 12 of no. 9.

#### Theorem 2 {#ac-iii-s2-thm-2 .statement}

Let A be a graded ring of type $\mathbf{N}$, M a graded A-module of type $\mathbf{N}$ and $(A_n)$ and $(M_n)$ their respective graduations. Suppose that there exists an element $a \in A_0$ such that $A_n = A_0 a^n$ and $M_n = a^n M_0$ for all $n > 0$. Then, if M, is a Noetherian $A_0$-module, M is a Noetherian A-module.

By virtue of Lemma 1 it is sufficient to prove that every graded submodule N of M is finitely generated. For all $r \geq 0$, let $N_r = N \cap M_r$ and let L_r be the set of $m \in M_0$ such that $a^r m \in N_r$. As
$$
a^r A_0 \subset A_r = A_0 a^r, \quad a^r A_0 L_r \subset A_0 a^r L_r \subset A_0 N_r \subset N_r
$$

and hence the L, are sub-A,-modules of M,; moreover,

$$
aN_r \subset N \cap aM_r = N \cap M_{r+1} = N_{r+1}
$$

and hence the sequence $(L_r)_{r \geq 0}$ is increasing. The hypothesis implies that there exists an integer $n \geq 0$ such that $L_r = L_n$ for $r \geq n$. For each $r \leq n$, let $(m_{r,s})_{1 \leq s \leq k_r}$ be a system of generators of the A,-module $L_r$. We shall show that the elements $a^r m_{r,s}$ for $1 \leq s \leq k_r$, $0 \leq r \leq n$ form a system of generators of the A-module N. As $M_r = a^r M_0$ for all $r$, $N_r = a^r L_r$ for all $r$ by definition of $L_r$. Then, for $r \leq n$,

$$
N_r = a^r L_r = \sum_{s=1}^{k_r} a^r A_0 m_{r,s} \subset \sum_{s=1}^{k_r} A_0 a^r m_{rs},
$$

and, for $r > n$,

$$
N_r = a^r L_n = \sum_{s=1}^{k_n} a^r A_0 m_{n,s} \subset \sum_{s=1}^{k_n} A_0 a^r m_{n,s} \subset \sum_{s=1}^{k_n} A_0 a^{r-n} \cdot (a^n m_{n,s})
$$

which completes the proof (cf. Exercise 10).

#### Corollary 1 (Hilbert’s Theorem) {#ac-iii-s2-thm-2-cor-1 .statement}

*For every commutative Noetherian ring C, the polynomial ring C[X] is Noetherian* (cf. Exercise 10).

#### Corollary 2 {#ac-iii-s2-thm-2-cor-2 .statement}

*For every commutative Noetherian ring C and every integer $n > 0$, the polynomial ring C[X_1, ..., X_n] is Noetherian.*

This follows from Corollary 1 by induction on $n$.

#### Corollary 3 {#ac-iii-s2-thm-2-cor-3 .statement}

*If C is a commutative Noetherian ring, every finitely generated commutative C-algebra is a Noetherian ring.*

Such an algebra is isomorphic to a quotient of a polynomial algebra C[X_1, ..., X_n] (§ 1, no. 1).

#### Corollary 4 {#ac-iii-s2-thm-2-cor-4 .statement}

*Let A be a graded commutative ring of type $\mathbf{N}$ and let $(A_n)$ be its graduation. For A to be Noetherian, it is necessary and sufficient that $A_n$ be Noetherian and that A be ajinitely generated A,-algebra.*

The condition is sufficient by Corollary 3. Conversely, suppose A is Noetherian; $m = \sum_{n \geq 1} A_n$ which is an ideal of A, is then finitely generated; then A is a finitely generated A,-algebra (§ 1, no. 2, Corollary to Proposition 1); on the other hand $A_n$, which is isomorphic to $A/m$, is a Noetherian ring.

#### Corollary 5 {#ac-iii-s2-thm-2-cor-5 .statement}

*Let A be a commutative ring and m an ideal of A such that $A/m$ is Noetherian, $m/m^2$ is ajinitely generated $(A/m)$-module and A is Hausdorff and complete with the m-adic topology. Then gr(A) and A are Noetherian.*

gr(A) is an $(A/m)$-module generated by $m/m^2$ (no. 3, Example 3) and hence the ring gr(A) is Noetherian by Corollary 3. From this we deduce that A itself is Noetherian (no. 9, Corollary 2 to Proposition 12).

#### Corollary 6 {#ac-iii-s2-thm-2-cor-6 .statement}

For every commutative Noetherian ring C and every integer n > 0, the ring of formal power series $\mathbf{C}[[X_1, \ldots, X_n]]$ is Noetherian.

This follows from Corollary 5 and no. 6, Corollary to Proposition 6, for if m is the ideal of $A = \mathbf{C}[[X_1, \ldots, X_n]]$ consisting of the formal power series with no constant term, $A/m$ is isomorphic to C and $m/m^2$ to the C-module $\mathbf{C}"$.

Remarks

(1) Corollaries 2, 3 and 6 apply in particular if C is a commutative field.

\* (2) Let g be a Lie algebra over a commutative Noetherian ring C and suppose that g is a finitely generated C-module. Let the enveloping algebra U of g be given the increasing filtration $(U_n)$ defined in no. 3, Example 4. With the corresponding topology, U is discrete and hence Hausdorff and complete; the associated graded ring gr(U) is a finitely generated C-algebra, being a quotient of the symmetric algebra $\mathcal{S}(g)$, hence gr(U) is a Noetherian ring (Corollary 3) and we deduce that U is a left and right Noetherian ring (no. 9, Corollary 2 to Proposition 12). \*

### 11. COMPLETE m-ADIC RINGS AND INVERSE LIMITS

We have seen in no. 6 that, if A is a commutative ring and m an ideal of A such that A is Hausdorf and complete with the m-adic topology, then the topological ring $A$ is canonically identified with the inverse limit of the discrete rings $A_i = A/m^{i+1} \ (i \in \mathbf{N})$ with respect to the canonical mappings

$$
h_{ij}: A/m^{j+1} \to A/m^{i+1} \quad (i \leq j);
$$

note that $h_{ij}$ is surjective and that, if $n_{ij}$ is its kernel, then

$$
n_{ij} = m^{i+1}/m^{j+1} = (m/m^{j+1})^{i+1} =
$$

in particular $(n_{0j})^{j+1} = 0$. Conversely:

#### Proposition 14 {#ac-iii-s2-prop-14 .statement}

Let $(A,, h_{ij})$ be an inverse system of discrete commutative rings, whose indexing set is $\mathbf{N}$ and let $(M_i, u_{ij})$ be an inverse system of modules over the inverse system of rings $(A_i, h_{ij})$. Let $n_j$ denote the kernel of $h_{0j}: A \to A$, and set $A = \lim A_i$, $M = \lim M_i$. Suppose that

(a) for all $i \in \mathbf{N}$, $h_{ii}$ is the identity mapping on A, and, for $i \leq j$, $h_{ij}$ and $u_{ij}$ are surjective;
(b) for $i \leq j$, the kernels of $h_{ij}$ and $u_{ij}$ are $n_j^{i+1}$ and $n_j^{i+1} M_j$ respectively.

Then:
(i) $A$ is a complete Hausdorff topological ring, $M$ is a complete Hausdorff topological A-module and the canonical mappings $h,: A \to A,, u_i: M \to M_i$ are surjective.
(ii) If $M_0$ is a finitely generated A,-module, $M$ is a finitely generated A-module;

to be precise, every finite subset S of M such that $u_0(S)$ generates M, is a system of generators of M.

The assertions in (i) follow from General Topology, Chapter II, § 3, no. 5, Corollary to Proposition 10 and Corollary 1 to Theorem 1.

For all $i \in \mathbf{N}$, let us write $m_{i+1} = \mathrm{Ker}(h_i), N_{i+1} = \mathrm{Ker}(u_i)$; then

$$
m_{i+1} = \lim_{k \geq 0} h_{i,t+k}^{-1}(0) = \lim_{\leftarrow} n_{i+1}^{t+k}
$$

and $N_{i+1} = \lim_{\leftarrow} n_{i+k}^{t+1} M_{i+k}$; as $h_{i+k}$ and $u_{i+k}$ are surjective,

$$
h_{i+k}(m_{i+1}) = n_{i+k}^{t+1}, \quad u_{i+k}(N_{i+1}) = n_{i+k}^{t+1} M_{i+k}.
$$

Let us show that $m_i N_j \subset N_{i+j}$ for $i \geq 1$ and $j \geq 1$, which amounts to proving that $u_{i+j-1}(m_i N_j) = 0$; now

$$
u_{i+j-1}(m_i N_j) = h_{i+j-1}(m_i) u_{i+j-1}(N_j)
$$

is equal to $n_{i+j-1}^{t'}(n_{i+j-1}^{t'} M_{i+j-1}) = 0$, as, for all $k \geq 0$, $n_k^{k+1}$, which is the kernel of $h_{kk}$, is equal to 0. We see similarly that $m_i m_j \subset m_{i+j}$. If for $i \leq 0$ we set $m_i = A$ and $N_i = M$, $(m_i)_{i \in \mathbf{Z}}$ is a filtration of A and $(N_i)_{i \in \mathbf{Z}}$ a filtration of M compatible with the filtration on A; the topologies on A and M are obviously those defined by these filtrations. This being so, let $a$ be an ideal of A such that $h_1(a) = n_1$ and $M'$ the submodule of M generated by S; we are going to prove that

$$
N_i = a^i M' + N_{i+1} \quad \text{for } i \geq 0.
$$

Let us write $a_i = h_i(a), M'_i = u_i(M')$; it is sufficient to show that

$$
u_i(N_i) = a_i^i M'_i.
$$

This is true if $i = 0$, for $N_0 = M$ and $M'_0 = M$, by hypothesis. If $i \geq 1$, then $u_i(N_i) = n_i^i M_i$ by (16). As $h_{1i}$ is surjective and $h_{0i} = h_{01} \circ h_{1i}$, $h_{1i}$ maps the kernel $n_i$ of $h_i$, onto the kernel $n_1$ of $h_1$, and $n_i = h_{1i}(n_1)$; then

$$
h_{1i}(a_i) = h_1(a) = n_1 = h_{1i}(n_i)
$$

and, as the kernel of $h_{1i}$ is $n_i^2$, $n_i \subset a_i + n_i^2$ and $a_i \subset n_i$, whence $n_i = a_i + n_i^2$. Moreover $u_{0i}(M'_i) = u_0(M') = M, = u_{0i}(M_i)$ and, as $\mathrm{Ker}(u_{0i}) = n_i M_i$, $M_i = M'_i + n_i M_i$; whence

$$
n_i^i M_i = (a_i + n_i^2)^i (M'_i + n_i M_i).
$$

Now, $a_i^k n_i^{i+1-k} \subset n_i^{i+1} = 0$ for $0 \leq k \leq i$; then it certainly follows that $u_i(N_i) = n_i M_i = a_i^i M'_i$, which proves (17).

Moreover $m_1 = h_1(n_1)$, whence $a \subset m_1$ and therefore $a^i \subset m_1^i \subset m_i$, whence

$N_i \subset m_i M' + N_{i+1}$; on the other hand obviously $m_i M \subset N_i$ and hence $N_i = m_i M' + N_{i+1}$ for all $i \geq 0$; then it follows from Corollary 3 to Proposition 12 of no. 9 that $M' = M$, which completes the proof.

#### Corollary 1 {#ac-iii-s2-prop-14-cor-1 .statement}

*With the notation and hypotheses of Proposition 14 suppose further that $M_0$ is a finitely generated $A$-module and that the ideal $n_1$ of $A$, is finitely generated. Let $m_1$ be the kernel of $h_1$; the topologies on $A$ and $M$ are then the $m_1$-adic topologies on this ring and this module respectively; to be precise, for all $i \geq 0$, the kernels of $h_i$ and $u_i$ are $m_1^{i+1}$ and $m_1^{i+1} M$ respectively; further $m_1 / m_1^2$ is a finitely generated $A$-module.*

We preserve the notation of the proof of Proposition 14; the hypotheses here allow us to assume that the ideal $a$ is finitely generated. Let $i \geq 0$ be any integer; for all $j \geq 0$, by (17), $N_{i+j} = a^j(a^i M) + N_{i+j+1} \subset m_j(a^i M) + N_{i+j+1}$; conversely, $m_j(a^i M) \subset m_j m_i M \subset m_{i+j} M \subset N_{i+j}$, whence

$$
N_{i+j} = m_j(a^i M) + N_{i+j+1}.
$$

As $a$ and $M$ are finitely generated $A$-modules, so is $a^i M$. Applying Corollary 3 to Proposition 12 of no. 9 to the module $N_i$ with the filtration $(N_{ij})_{j \in \mathbf{Z}}$ defined by $N_{ij} = N_i$, if $j < 0$, $N_{ij} = N_{i+j}$ if $j \geq 0$, we obtain $N_i = a^i M$, whence $N_i \subset m_1^i M$. But also $m_1^i M \subset m_i M \subset N_i$, whence $N_i = m_1^i M$. Applying this to the case where $M = A$, $u_{ij} = h_{ij}$, we obtain $m_i = m_1^i$. Moreover, $m_1 = a + m_1^2$ by (17), which proves the last assertion of the corollary.

#### Corollary 2 {#ac-iii-s2-prop-14-cor-2 .statement}

*Under the hypotheses of Corollary 1, for $A$ to be Noetherian, it is necessary and sufficient that $A$, be so.*

The condition is necessary since $A$, is isomorphic to a quotient of $A$; it is sufficient by virtue of no. 10, Corollary 5 to Theorem 2.

### 12. THE HAUSDORFF COMPLETION OF A FILTERED MODULE

Let $G$ be a filtered group whose filtration $(G,)$ consists of normal subgroups of $G$; we have already recalled (no. 6) that the *Hausdorff completion* $\hat{G}$ of the topological group $G$ is canonically identified with the inverse limit $\lim \leftarrow G/G_n$ of the *discrete* groups $G/G_n$, the canonical homomorphism $i : G \to \hat{G}$ having image the Hausdorff group associated with $G$ (everywhere dense in $\hat{G}$) and kernel the closure $\bigcap G$, of $\{0\}$ in $G$. The Hausdorff completion $\hat{G}_n$ of the subgroup $G$, of $G$ is identified with the closure of $i(G_n)$ in $\hat{G}$ (*General Topology*, Chapter II, § 3, no. 9, Corollary 1 to Proposition 18) and, since $G$, is closed in $\hat{G}$,

$$
G, = i^{-1}(\hat{G}_n) = i^{-1}(\hat{G}_n \cap i(G)).
$$

Moreover, the $\hat{G}_n$ form a fundamental system of neighbourhoods of 0 in $\hat{G}$ (*General Topology*, Chapter 111, § 3, no. 4, Proposition 7) and are therefore normal open subgroups of $\hat{G}$ (General Topology, Chapter 111, § 2, no. 3, Proposition 8); the topology on $\hat{G}$ is defined by the filtration $(\hat{G}_n)$, which is always separated by definition. As $i(G)$ is dense in $\hat{G}$ and $\hat{G}_n$ is open,

$$
\hat{G} = i(G) \cdot \hat{G}_n
$$

and similarly

$$
= i(G_{n-1}) \cdot \hat{G}_n.
$$

We deduce from (18) and (19) that the filtration $(\hat{G}_n)$ is exhaustive if and only if $(G,)$ is.

The second isomorphism theorem (Algebra, Chapter I, § 6, no. 13, Theorem 6 (d)) and equations (18), (19) and (20) show that the canonical homomorphisms

$$
G_{n-1}/G_n \to \hat{G}_{n-1}/\hat{G}_n, \quad G/G_n \to \hat{G}/\hat{G}_n,
$$

are bijective and hence so is the canonical homomorphism

$$
\operatorname{gr}(G) \to \operatorname{gr}(\hat{G}).
$$

Now let $A$ be a filtered ring, $E$ a filtered $A$-module and $(A_n)$ and $(E_n)$ the respective filtrations of $A$ and $E$; we shall assume that these filtrations are exhaustive so that for the corresponding topologies $A$ is a topological ring and $E$ a topological $A$-module (no. 5, Proposition 3). Then we have defined (General Topology, Chapter 111, §6, nos. 5 and 6) $\hat{A}$ as a topological ring and $\hat{E}$ as a topological $\hat{A}$-module. If $i : A \to \hat{A}$ is the canonical homomorphism, then $i(A_m)i(A_n) \subset i(A_{m+n})$, whence by the continuity of multiplication in $A$,

$$
\hat{A}_m \hat{A}_n \subset \hat{A}_{m+n}
$$

since $A_n$ is the closure of $i(A_n)$ in $\hat{A}$. It can be similarly shown that

$$
\hat{A}_m \hat{E}_n \subset \hat{E}_{m+n};
$$

in other words:

#### Proposition 15 {#ac-iii-s2-prop-15 .statement}

Let $A$ be a filtered ring and $E$ a filtered $A$-module, the respective filtrations $(A_n), (E_n)$ of $A$ and $E$ being exhaustive. Then $(\hat{A}_n)$ is a filtration compatible with the ring structure on $\hat{A}$ and $(\hat{E}_n)$ a filtration compatible with the module structure on $\hat{E}$ over the filtered ring $\hat{A}$; moreover these filtrations are exhaustive and define respectively the topologies on $\hat{A}$ and $\hat{E}$. Finally, the canonical mappings $\operatorname{gr}(A) \to \operatorname{gr}(\hat{A})$ and $\operatorname{gr}(E) \to \operatorname{gr}(\hat{E})$ of graded $\mathbf{Z}$-modules are respectively a graded ring isomorphism and a graded $\operatorname{gr}(A)$-module isomorphism.

In what follows, for every uniform space $X$, $j_X$ will denote the canonical mapping from $X$ to its Hausdorff completion $\hat{X}$ and $X_0 = j_X(X)$ the uniform subspace of $\hat{X}$, which is the Hausdorff space associated with $X$. Recall that the topology on $X$ is the inverse image under $j_X$ of that on $X_0$ (General Topology,

Chapter II, § 3, no. 7, Proposition 12). Recall also that, for every uniformly continuous mapping $f : X \to Y$, $\hat{f}$ denotes the uniformly continuous mapping from $\hat{X}$ to $\hat{Y}$ such that $\hat{f} \circ j_X = j_Y \circ f$ (loc. cit., Proposition 15); if $X$ is a uniform subspace of $Y$ and $\mathcal{E}$ the canonical injection, $\hat{X}$ is identified with a uniform subspace of $\hat{Y}$ and $\hat{f}$ is the canonical injection of $X$ into $\hat{Y}$ (loc. cit., no. 9. Corollary 1 to Proposition 18).

#### Lemma 2 {#ac-iii-s2-lem-2 .statement}

*Let $X \xrightarrow{f} Y \xrightarrow{g} Z$ be an exact sequence of strict morphisms of topological groups (Algebra, Chapter II, § 1, no. 4, Remark). Suppose that $X, Y, Z$ admit Hausdorff completion groups and that the identity elements $\mathcal{E} X, Y, Z$ admit countable fundamental systems of neighbourhoods. Then $\hat{X} \xrightarrow{\hat{f}} \hat{Y} \xrightarrow{\hat{g}} \hat{Z}$ is an exact sequence of strict morphisms.*

Let $N_1, N_g$ be the respective kernels off and $g$; let us write

$$
f = f_3 \circ f_2 \circ f_1
$$

where $f_1$ is the canonical mapping $X \to X/N_f$, $f_2$ is an isomorphism of $X/N_f$ onto $N$, and $f_3$ is the canonical injection $N \to Y$. We already know that $f_2$ is an isomorphism of $(X/N_f)^*$ onto $\hat{N}_g$ and we have just recalled that $f_1$ is an injective strict morphism of $N$, to $\hat{Y}$; if we show that $\hat{f}_1$ is a surjective strict morphism, it will follow that $\hat{f}$ is a strict morphism (General Topology, Chapter III, § 2, no. 8, Remark 2). Let $g_1$ be the canonical mapping $Y \to Y/N_g$; if we show that $\hat{g}_1$ is a surjective strict morphism of the kernel $\hat{N}_g$, we shall see as above that $\hat{g}$ is a strict morphism and the sequence $\hat{X} \xrightarrow{\hat{f}} \hat{Y} \xrightarrow{\hat{g}} \hat{Z}$ will be exact. Thus we have reduced the problem to proving that, if $Y = X/N$ (where $N$ is a normal subgroup of $X$) and $f : X \to Y$ is the canonical mapping, $\hat{f}$ is a *surjective strict morphism with kernel* $\hat{N}$.

Let $f_0 : X_0 \to Y_0$ be the mapping which coincides with $f$ on $X_0$; as $j_X$ (resp. $j_Y$) is a surjective strict morphism of $X$ onto $X$, (resp. $Y$ onto $Y_0$), $f_0$ is a surjective strict morphism (General Topology, Chapter III, § 2, no. 8, Remark 3). Now $X_0$ and $Y_0$ are metrizable (General Topology, Chapter IX, § 3, no. 1, Proposition 1); then it follows from General Topology, Chapter IX, § 3, no. 1, Corollary 1 to Proposition 4 and Lemma 1, that $\hat{f}_0 = \hat{f}$ is a surjective strict morphism and has kernel the closure $\hat{N}_0'$ *in* $X$ of the kernel $N_0'$ of $f_0$. Then it will be sufficient for us to prove that $\hat{N}_0' = \hat{N}$. Now $N_0'$ obviously contains $N_0 = j_X(N)$; it will be sufficient to show that $N_0'$ is contained in the closure $\overline{N}_0$ of $N_0$ *in* $X$. Now,

$$
u = j_X^{-1}(X_0 - \overline{N}_0) = X - j_X^{-1}(\overline{N}_0)
$$

is an open set in $X$ which does not meet $N$; as $f$ is a surjective strict morphism, $V = f(U)$ is an open set in $Y$ not containing the identity element $e'$ of $Y$ and hence not meeting the closure of $e'$; then $j_Y(V)$ does not contain the identity element of $Y_0$. But $j_Y(V) = f_0(X_0 - \overline{N}_0)$ and hence $N'_0 \subset \overline{N}_0$, which complete the proof of Lemma 2.

#### Proposition 16 {#ac-iii-s2-prop-16 .statement}

*Let $A$ be a filtered ring, ($A,$) its filtration, $E$ an $A$-module and ($E_n$) the filtration on $E$ derived from that on $A$ consisting of the $E_n = A_n E$. Suppose that the filtration ($A,$) is exhaustive and the module $E$ is finitely generated. If $i : E \to \hat{E}$ is the canonical mapping, then, for all $n \in \mathbf{Z}$,*
$$
8_n = \hat{A}_n \hat{E} = \hat{A}_n i(E) \quad \text{and} \quad \hat{E} = \hat{A}.i(E).
$$
*In particular $\hat{E}$ is a finitely generated $\hat{A}$-module.*

The equation $A_n E = E_n$ implies, by virtue of the continuity of the external law on the $A$-module $8, \hat{A}_n \hat{E} \subset 8$, and obviously $\hat{A}_n \hat{E} \supset \hat{A}_n i(E)$. By hypothesis there exists a surjective homomorphism $u : L \to E$, where $L = A_s^I$, $I$ being a finite set; let $L$ be given the product filtration, consisting of the $L_n = A_n^I$, which define on $L$ the product topology; then $\hat{L} = \hat{A}_s^I$ and $\hat{L}_n = \hat{A}_n^I$ (*General Topology*, Chapter II, § 3, no. 9, Corollary 2 to Proposition 18). Let $j : L \to \hat{L}$ be the canonical mapping and $(e_i)_{i \in I}$ the canonical basis of $L$; for an element $\sum_{i \in I} a_{ij}(e_i)$ (where $a_i \in \hat{A}$ for all $i \in I$) to belong to $\hat{L}_n$, it is necessary and sufficient that $a_i \in \hat{A}_n$ for all $i$; then $\hat{L}_n = \hat{A}_n . j(L)$. This being so, by definition $u(\hat{L}_n) = A_n E = E_n$ and hence $u$ is a *strict morphism* of $L$ onto $E$ (*General Topology*, Chapter III, § 2, no. 8, Proposition 24). Lemma 2 then shows that $\hat{u} : \hat{L} \to \hat{E}$ is a *surjective strict morphism*. As $\hat{L}_n$ is an open subgroup off, $\hat{u}(\hat{L}_n)$ is an open (and therefore closed) subgroup of $\hat{E}$; but $\hat{u}(\hat{L}_n) = \hat{A}_n \hat{u}(j(L)) = \hat{A}_n i(E)$ and, as $i(E_n) \subset A_n i(E) \subset \hat{A}_n i(E)$, finally $\hat{E}_n \subset \hat{A}_n i(E) \subset \hat{A}_n \hat{E} \subset \hat{E}_n$ and therefore $\hat{E}_n = \hat{A}_n \hat{E} = \hat{A}_n i(E)$; setting $n = 0$, we obtain the second formula of (25).

#### Corollary 1 {#ac-iii-s2-prop-16-cor-1 .statement}

*Under the conditions of Proposition 16, if $A$ is complete, so is $E$.*

As the canonical mapping $A \to \hat{A}$ is then surjective (no. 6, Proposition 5), $\hat{E} = i(E)$ by (25) and the conclusion follows by Proposition 5 of no. 6.

#### Corollary 2 {#ac-iii-s2-prop-16-cor-2 .statement}

*Let $A$ be a commutative ring, $m$ a finitely generated ideal of $A$ and $\hat{A}$ the Hausdorff completion of $A$ with respect to the $m$-adic topology. Then $\hat{m}^n = (\hat{m})^n = m^n . \hat{A}$ for every integer $n > 0$ and the topology on $\hat{A}$ is the $\hat{m}$-adic topology.*

Let us write $A_n = m^n$, which is a finitely generated ideal of $A$. The formula $m^p A_n = m^{n+p}$ shows that the topology induced on $A$, by the $m$-adic topology coincides with the $m$-adic topology on the $A$-module $A_n$ (no. 1, *Example 3*).

By Proposition 16 applied to $E = A_n$, $\hat{A}_n = \hat{A}.A_n$ in other words $\hat{m}^n = m^n . \hat{A}$. In particular $m = m . \hat{A}$, whence
$$
(\hat{m})^n = m^n . \hat{A} = \hat{A}.A_n
$$
(cf. Exercise 12).

Examples of Hausdorff completions of filtered rings

(1) Let $A$ be a graded ring of type $\mathbf{N}$ and let $(A_n)_{n \geq 0}$ be its graduation; let it be given the associated filtration which is separated and exhaustive (no. 1, Example 1). The additive group $A$ is canonically identified with a subgroup of $B = \prod_{n \in \mathbf{N}} A_n$; if $B$ is given the topology the product of the discrete topologies, the topology induced on $A$ is the topology defined by the filtration on $A$; also $B$ is a complete topological group and $A$ is dense in $B$ (General Topology, Chapter III, §2, no. 9, Proposition 25). The additive topological group $B$ is then identified with the completion $\hat{A}$ of the Hausdorff additive group $A$ and it follows from Proposition 15 that it has a unique ring structure which makes it the completion of the topological ring $A$. To define multiplication in this ring, note that, if we write $A'_n = \sum_{i > n} A_i$, the closure in $B$ of the two-sided ideal $A'_n$ is the set $B$, of $x = (x_i) \in B$ such that $x_i = 0$ for $i \leq n$. Then let $x = (x_i), y = (y_i)$ be two elements of $B$ and $z = (z_i)$ their product. Then, for all $n > 0$, $x \equiv x'_n$ (mod. $B_n$), $y \equiv y'_n$ (mod. $B_n$), where $x'_n = (x_i)_{0 \leq i \leq n}$, $y'_n = (y_i)_{0 \leq i \leq n}$, whence $z \equiv x'_n y'_n$ (mod. $B_n$). But $x'_n$ and $y'_n$ belong to $A$ and it is therefore seen that, for all $n \in \mathbf{N}$,

$$
z_n = \sum_{j=0}^n x_j y_{n-j}.
$$

In particular, we again obtain the Corollary to Proposition 6 of no. 6 : if $C$ is a commutative ring, the completion of the polynomial ring $C[X_1, \ldots, X_r]$, with the filtration associated with its usual graduation (by total degree) is canonically identified with the ring of formal power series $C[[X_1, \ldots, X_r]]$ (cf. Algebra, Chapter IV, §5, no. 10).

*(2) Let $K$ be a complete commutative field with a valuation. The completion of the ring of convergent series in $r$ variables over $K$ is canonically identified with the ring of formal power series $K[[X_1, \ldots, X_r]]$. \*

(3) Let $a$ be a non-zero non-invertible element of a principal ideal domain; the (a)-adic topology on $A$ is also called the $a$-adic topology; it is Hausdorff, for the intersection of the ideals $(a^n)$ reduces to 0 (Algebra, Chapter VII, §1, no. 3). Note that the completion of $A$ with respect to this topology is not necessarily an integral domain (cf. no. 13, Remark 3). The associated graded ring $\mathrm{gr}(A) = \mathrm{gr}(\hat{A})$ is canonically isomorphic to $(A/a)[X]$ (no. 3, Example 1). If $A = \mathbf{Z}$, the completion of $\mathbf{Z}$ with respect to the n-adic topology ($n > 1$) is denoted by $\mathbf{Z}_n$ and its elements are called $n$-adic integers.

Every element of $\mathbf{Z}/n^k \mathbf{Z}$ admits a unique representative of the form $\sum_{i=0}^{k-1} a_i n^i$ where $0 \leq a_i \leq n - 1$ for all $i$; moreover, its canonical image in $\mathbf{Z}/n^{k-1} \mathbf{Z}$ is the class of $\sum_{i=0}^{k-2} a_i n^i$. These remarks and the fact that $Z$, is canonically identified with the inverse limit $\lim_{\leftarrow} \mathbf{Z}/n^k \mathbf{Z}$ show immediately that every element of $Z$, can be written uniquely in the form $\sum_{i=0}^{\infty} a_i n^i$ where $0 \leq a_i < n$ and conversely that such a series is convergent in $\mathbf{Z}$.

### 13. THE HAUSDORFF COMPLETION OF A SEMI-LOCAL RING

#### Proposition 17 {#ac-iii-s2-prop-17 .statement}

Let $A$ be a commutative ring and $(m_{\lambda})_{\lambda \in L}$ a family of ideals of $A$, distinct from $A$, such that $m_{\lambda}$ and $m_{\mu}$ are relatively prime for $\lambda \neq \mu$. For every family $s = (s(\lambda))_{\lambda \in L}$ of integers $\geq 0$, of finite support, set $a_s = \bigcap_{\lambda \in L} m_{\lambda}^{s(\lambda)}$ (equal to the product of the $m_{\lambda}^{s(\lambda)}$ for the $\lambda$ such that $s(\lambda) \neq 0$; cf. Chapter 11, § 1, no. 2, Propositions 3 and 5); the $a_s$ form a fundamental system of neighbourhoods of 0 with respect to a topology $\mathcal{T}$ compatible with the ring structure on $A$; let $\hat{A}$ be the Hausdorff completion of $A$ with respect to this topology. On the other hand, for all $\lambda \in L$, let $A_{\lambda}$ be the ring $A$ with the $m_{\lambda}$-adic topology and let $\hat{A}_{\lambda}$ be its Hausdorff completion. If $u : A \to \prod_{\lambda \in L} A_{\lambda}$ denotes the diagonal homomorphism, $u$ is continuous and the corresponding homomorphism $\hat{u} :$

$$
\hat{A} \to \left( \prod_{\lambda \in L} A_{\lambda} \right)^{\hat{}} = \prod_{\lambda \in L} \hat{A}_{\lambda}
$$

(General Topology, Chapter III, § 6, no. 5 and Chapter II, § 3, no. 9, Corollary 2 to Proposition 18) is a topological ring isomorphism.

The first assertion follows from General Topology, Chapter III, § 6, no. 3, Example 3. Let us set $B = \prod_{\lambda \in L} A_{\lambda}$; as the topology on $A$ is finer than each of the $m_{\lambda}$-adic topologies, the mappings $\mathrm{pr}_{\lambda} \circ u$ are continuous and hence $u$ is continuous. Also, $u(a_s)$ is the intersection of the diagonal $A$ of $B$ and the open set $\bigcap_{\lambda \in L} \mathrm{pr}_{\lambda}^{-1}(m_{\lambda}^{s(\lambda)})$ of $B$; it follows that $u$ is a strict morphism from the additive group $A$ to $B$ with image $A$. Now $\Delta$ is dense in $B$. For let $b = (a_{\lambda})_{\lambda \in L}$ be an element of $B$; every neighbourhood of $b$ in $B$ contains a set of the form $b + V$, where $V = \bigcap_{\lambda \in L} \mathrm{pr}_{\lambda}^{-1}(m_{\lambda}^{s(\lambda)})$ for a family $s = (s(\lambda))_{\lambda \in L}$ with finite support of integers $\geq 0$. As the $m_{\lambda}^{s(\lambda)}$ are relatively prime in pairs (Chapter II, § 1, no. 2, Proposition 3), there exists $x \in A$ such that $x \equiv a_{\lambda} \pmod{m_{\lambda}^{s(\lambda)}}$ for all $\lambda$ (loc. cit., Proposition 5) and hence $(b + V) \cap A \neq \varnothing$. The Hausdorff completion of the group $B/\Delta$ is then $\{0\}$; applying Lemma 2 of no. 12 to the exact sequences $0 \to A \xrightarrow{u} B, A \xrightarrow{u} B \to B/\Delta$, we see that $\hat{u}$ is an isomorphism of $\hat{A}$ onto $\hat{B}$.

#### Corollary {#ac-iii-s2-n13-cor-1 .statement}

Let $A$ be a principal ideal domain and $P$ a representative system of extremal elements of $A$ (Algebra, Chapter VII, § 1, no. 3). The topology on $A$ with respect to which the ideals $\neq 0$ of $\mathbf{A}$ form a fundamental system of neighbourhoods of 0, which is compatible with the ring structure on $\mathbf{A}$, is Hausdorff and the completion of $\mathbf{A}$ with this topology is canonically isomorphic to the product of the completions of $\mathbf{A}$ with respect to the $x$-adic topologies, where $x$ runs through $P$.

The principal ideals $(x)$ where $\pi \in P$ are maximal and distinct and hence relatively prime, we have already seen (no. 12, Example 3) that the $x$-adic topologies are Hausdorff and hence so is the topology defined in the statement of Proposition 17, which is finer than each of the $x$-adic topologies.

If the Corollary to Proposition 17 is applied when $\mathbf{A} = \mathbf{Z}$, we denote by $\hat{\mathbf{Z}}$ the completion of $\mathbf{Z}$ with respect to the topology for which all the ideals $\neq 0$ of $\mathbf{Z}$ form a fundamental system of neighbourhoods of 0, the ring isomorphic to the product $\prod_{p \in P} \mathbf{Z}_p$ of the rings of $p$-adic integers (P being the set of prime numbers).

Remarks

(1) Clearly, under the conditions of Proposition 17, the topology $\mathcal{T}$ is the least upper bound of the $m_\lambda$-adic topologies on $\mathbf{A}$.

(2) Every closed ideal $a$ of $\prod_{\lambda \in L} \hat{A}_\lambda$ is identical with the product of its projections $a_\lambda = \mathrm{pr}_\lambda(a)$, which are closed ideals in the $A_\lambda$; for $\hat{A}_\lambda$ is canonically identified with a closed ideal $A'_\lambda$ of $\prod_{\lambda} \hat{A}_\lambda$ and $a_\lambda$ with $a \cap A'_\lambda$ (Algebra, Chapter I, §8, no. 10, Proposition 6), the sum of the $a_\lambda$ is dense in the product $\prod_\lambda a_\lambda$ (General Topology, Chapter III, §2, no. 9, Proposition 25) and the latter is closed in $\prod_\lambda \hat{A}_\lambda$, whence our assertion.

#### Proposition 18 {#ac-iii-s2-prop-18 .statement}

Let $\mathbf{A}$ be a commutative ring, $(m_i)_{1 \leq i \leq q}$ a finite family of distinct maximal ideals of $\mathbf{A}$, t the product ideal $m_1 m_2 \ldots m_q = m_1 \cap m_2 \cap \ldots \cap m_q$ and $S$ the multiplicative subset $\bigcap_{i=1}^q (\mathbf{A} - m_i)$. Let $\mathbf{A}$ be given the $r$-adic topology, the ring $B = S^{-1} \mathbf{A}$ the $rB$-adic topology and each of the local rings $A_n$ the $(m_i A_{m_i})$-adic topology. Let $u : \mathbf{A} \to B$, $v_i : B \to A_{m_i}$ be the canonical homomorphism (Chapter II, §2, no.1, Corollary 2 to Proposition 2) and $v$ the homomorphism $(v_i) : B \to \prod_{i=1}^q A_n$. The homomorphisms $u$ and $v$ are continuous and the corresponding homomorphism $\hat{u} : \hat{\mathbf{A}} \to$ and $\hat{v} : \hat{B} \to \prod_{n} (A_n)^*$ are topological ring isomorphisms.

$m_i \cap S = \varnothing$ for $1 \leq i \leq q$, hence the ideal $m'_i = m_i B$ of $B$ is maximal (Chapter II, §2, no. 5, Proposition 11) and
$$
rB = m'_1 \cap m'_2 \cap \cdots \cap m'_q
$$

(Chapter II, § 2, no. 4); finally, $B_{m'_i} = A_i$, up to a canonical isomorphism (Chapter 11, § 2, no. 5, Proposition 11). As $\bar{u}^1(rB) = r$ and $\bar{v}_i^1(m_iA_{m_i}) \supset rB$, $u$ and $v$ are continuous. Then it is sufficient to prove that,

$$
w = v \circ u : A \to \prod_{i=1}^4 A_{m_i},
$$

$\hat{w}$ is an isomorphism of $\hat{A}$ onto $\prod_{i=1}^q \hat{A}_{m_i}$, for this result applied to $B$ and the $m'_i$ will show that $\hat{v}$ is an isomorphism and therefore also $\hat{u}$. Note that every product of powers of the $m_i$ contains a power of $c$ and hence the $r$-adic topology is the least upper bound of the $m_i$-adic topologies; moreover, if $A_i$ denotes the ring $A$ with the $m_i$-adic topology and $\phi : A \to \prod_{i=1}^q A$, the diagonal mapping, $\hat{\phi} : \hat{A} \to \prod_{i=1}^4 \hat{A}_i$ is an isomorphism (Proposition 17). Then it all amounts to proving that, if $u_i : A_i \to A_{m_i}$ is the canonical mapping, $\hat{u}_i : \hat{A}_i \to \hat{A}_{m_i}$ is an isomorphism. Now, for all $n$, the mapping

$$
u_{i,n} : A/m_i^n \to A_{m_i}/m_i^n A_{m_i}
$$

derived from $u_i$ by taking quotients is an isomorphism (Chapter II, §3, no. 3, Proposition 9); our assertion follows from the fact that $\hat{A}_i$ (resp. $\hat{A}_{m_i}$) is the inverse limit of the discrete rings $A/m_i^n$ (resp. $A_{m_i}/m_i^n A_{m_i}$) (cf. no. 6).

Remark (3). We see that an integral domain $A$ can be such that its Hausdorff completion $\hat{A}$ admits non-zero divisors of zero.

#### Proposition 19 {#ac-iii-s2-prop-19 .statement}

Let $A$ be a commutative ring and $m$ a maximal ideal of $A$. The Hausdorff completion $\hat{A}$ of $A$ with respect to the $m$-adic topology is a local ring whose maximal ideal is $m$.

If $a = \bigcap_{k \geq 1} m^k$, $\hat{A}$ is the completion of the Hausdorff ring $A/a$ associated with $A$ and, as $m/a$ is maximal in $A/a$, we may assume that $A$ is Hausdorff with respect to the $m$-adic topology. As $A/m$ and $\hat{A}/\hat{m}$ are isomorphic rings (no. 12, formula (21)), $m$ is maximal in $\hat{A}$. As the topology on $\hat{A}$ is defined by the filtration $(m^n)^*$ (no. 12), the proposition will be a consequence of the following lemma:

#### Lemma 3 {#ac-iii-s2-lem-3 .statement}

Let $A$ be a complete Hausdorf topological ring, in which there exists a fundamental system $\mathcal{G}$ of neighbourhoods of 0 consisting of additive subgroups of $A$.
(i) For all $x \in A$ such that $\lim_{n \to m} x^n = 0$, $1 - x$ is invertible in $A$ and its inverse is equal to $\sum_{n=0}^\infty x^n$.
(ii) Let $a$ be a two-sided ideal of $A$ such that $\lim_{n \to \infty} x^n = 0$ for all $x \in a$. For an element y of $\mathbf{A}$ to be invertible, it is necessary and sufficient that its class mod. a be invertible in $\mathbf{A}/a$; in particular a is contained in the Jacobson radical of $\mathbf{A}$.

(i) As

$$
(1 - x)(1 + x + \cdots + x^n) = (1 + x + \cdots + x^n)(1 - x) = 1 - x^{n+1},
$$

it all amounts to proving that the series with general term $x^n$ is convergent in $\mathbf{A}$; now, by hypothesis, for every neighbourhood $V \in \mathfrak{S}$ of 0 in $\mathbf{A}$, there exists an integer $p > 0$ such that $x^n \in V$ for all $n \geq p$. We conclude that

$$
x^p + x^{p+1} + \ldots + x^q \in V
$$

for all $q \geq p$ and our assertion then follows from Cauchy's criterion (*General Topology*, Chapter III, § 5, no. 2, Theorem 1).

(ii) Suppose that there exists $y' \in \mathbf{A}$ such that $yy' \equiv 1$ (mod. a) and $y'y \equiv 1$ (mod. a). The hypothesis on a implies, by (i), that $yy'$ and $y'y$ are invertible in $\mathbf{A}$ and hence $y$ is invertible in $\mathbf{A}$. In particular, every $x \in a$ is such that $1 - x$ is invertible in $\mathbf{A}$ and, as a is a two-sided ideal of $\mathbf{A}$, it is contained in the Jacobson radical of $\mathbf{A}$ (*Algebra*, Chapter VIII, § 6, no. 3, Theorem 1).

Having established this lemma, it is sufficient to apply it to the topological ring $\hat{\mathbf{A}}$ and the ideal $\hat{\mathfrak{m}}$, as, for all $x \in \hat{\mathfrak{m}}$, $x^n \in (\hat{\mathfrak{m}})^n \subset (\mathfrak{m}^n)^{\wedge}$ and the sequence $(x^n)$ therefore tends to 0.

If we take $\mathbf{A} = \mathbf{Z}$, every maximal ideal of $\mathbf{Z}$ is of the form $p\mathbf{Z}$ where $p$ is prime. The ring of $p$-adic numbers $\mathbf{Z}_p$ is then a local ring of which $p\mathbf{Z}_p$ is the maximal ideal (Corollary 2 to Proposition 16) and whose residue field is isomorphic to $\mathbf{Z}/p\mathbf{Z} = \mathbf{F}_p$, and $\mathbf{Z}_{(p)}$ with the $p\mathbf{Z}_{(p)}$-adic topology is identified with a topological subring of $\mathbf{Z}$, containing $\mathbf{Z}$.

#### Corollary {#ac-iii-s2-n13-cor-2 .statement}

Let $\mathbf{A}$ be a semi-local ring (Chapter II, § 3, no. 5), $m_i$ its distinct maximal ideals $(1 \leq i \leq q)$ and

$$
r = m_1 \cap m_2 \cap \cdots \cap m_q
$$

its Jacobson radical. The Hausdorff completion $\hat{\mathbf{A}}$ of $\mathbf{A}$ with respect to the r-adic topology is a semi-local ring, canonically isomorphic to the product $\prod_{i=1}^q \hat{\mathbf{A}}_{m_i}$, where $\hat{\mathbf{A}}_{m_i}$ is the Hausdorff completion ring of the local ring $\mathbf{A}_{m_i}$ with respect to the $(m_i \mathbf{A}_{m_i})$-adic topology.

### Exercises {#ac-iii-s2-exercises}

See the [exercises for § 2](exercises/s2/).
