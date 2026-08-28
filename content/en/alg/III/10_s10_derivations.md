---
book: alg
book_title: Algebra
chapter: III
chapter_title: TENSOR ALGEBRAS, EXTERIOR ALGEBRAS, SYMMETRIC ALGEBRAS
section: 10
section_title: Derivations
lang: en
source: alg-i-iii
source_edition: 1998, Springer
pdf_pages: 0574-0598, 0669-0670
extraction: ocr
subsections:
    - "no": 1
      title: COMMUTATION FACTORS
      page: 0
      pdf_page: 574
    - "no": 2
      title: GENERAL DEFINITION OF DERIVATIONS
      page: 0
      pdf_page: 575
    - "no": 3
      title: EXAMPLES OF DERIVATIONS
      page: 0
      pdf_page: 577
    - "no": 4
      title: COMPOSITION OF DERIVATIONS
      page: 0
      pdf_page: 578
    - "no": 5
      title: DERIVATIONS OF AN ALGEBRA A INTO AN A-MODULE
      page: 0
      pdf_page: 581
    - "no": 6
      title: DERIVATIONS OF AN ALGEBRA
      page: 0
      pdf_page: 583
    - "no": 7
      title: Functorial Properties
      page: 0
      pdf_page: 584
    - "no": 8
      title: RELATIONS BETWEEN DERIVATIONS AND ALGEBRA HOMOMORPHISMS
      page: 0
      pdf_page: 585
    - "no": 9
      title: EXTENSION OF DERIVATIONS
      page: 0
      pdf_page: 586
    - "no": 10
      title: UNIVERSAL PROBLEM FOR DERIVATIONS; NON-COMMUTATIVE CASE
      page: 0
      pdf_page: 591
    - "no": 11
      title: UNIVERSAL PROBLEM FOR DERIVATIONS; COMMUTATIVE CASE
      page: 0
      pdf_page: 592
    - "no": 12
      title: FUNCTIORIAL PROPERTIES OF K-DIFFERENTIALS
      page: 0
      pdf_page: 594
statements: 41
exercises: 5
content_sha256: 321a0214d9f86881e7cc2493bc5c6c5f347dd080ee2ae7987600113edd176f01
---

## § 10. DERIVATIONS

In this paragraph, and unless otherwise mentioned, the algebras considered are not assumed to be associative nor necessarily to possess a unit element; K denotes a commutative ring.

### 1. COMMUTATION FACTORS

When in this paragraph we speak of graduations without specifying them, we shall always mean graduations of type $\Delta$, where $\Delta$ is a commutative group written additively. In this paragraph, a commutation factor over $\Delta$ with values in $\mathbf{Z}$ is called a commutation factor over $\Delta$ (§ 4, no. 7, Definition 6). A commutation factor over $\Delta$ is therefore identified with a mapping $\varepsilon : (\alpha, \beta) \mapsto \varepsilon_{\alpha \beta} = \varepsilon(\alpha, \beta)$ of $\Delta \times \Delta$ into the multiplicative group $\{-1, 1\}$ such that for $\alpha, \alpha', \beta, \beta'$ in $\Delta$,

$$
\begin{cases}
\varepsilon(\alpha + \alpha', \beta) = \varepsilon(\alpha, \beta)\varepsilon(\alpha', \beta) \\
\varepsilon(\alpha, \beta + \beta') = \varepsilon(\alpha, \beta)\varepsilon(\alpha, \beta') \\
\varepsilon(\beta, \alpha) = \varepsilon(\alpha, \beta).
\end{cases}
$$

(1)

It follows that $\varepsilon(2\alpha, \beta) = \varepsilon(\alpha, 2\beta) = 1$.

When $\Delta = \mathbf{Z}$, every commutation factor $\varepsilon$ is determined by giving $\varepsilon(1, 1)$; there are therefore only *two* such factors, the first defined by

(2)
$$
\varepsilon(p, q) = 1 \quad \text{for } p, q \text{ in } \mathbf{Z}
$$
and the second by
(3)
$$
\varepsilon(p, q) = (-1)^{pq} \quad \text{for } p, q \text{ in } \mathbf{Z}.
$$

### 2. GENERAL DEFINITION OF DERIVATIONS

Consider a commutative ring $K$, six graded $K$-modules of type $\Delta : A, A', A'', B, B', B''$, and three $K$-linear mappings
$$
\mu : A \times A' \to A'', \qquad \lambda_1 : B \times A' \to B'', \qquad \lambda_2 : A \times B' \to B''
$$
such that the corresponding $K$-linear mappings
$$
A \otimes_K A' \to A'', \qquad B \otimes_K A' \to B'', \qquad A \otimes_K B' \to B''
$$
are *graded of degree* 0. The image $\mu(a, a')$ for $a \in A, a' \in A'$ is simply denoted by $a.a'$ or even $aa'$, and similarly for the two other bilinear mappings. The *degree* of $a.a'$ is therefore the *sum* of the degrees of $a$ and $a'$.

#### Definition 1 {#alg-iii-s10-def-1 .statement}

*Given the above and a commutation factor $\varepsilon$ on $\Delta \times \Delta$, an $\varepsilon$-derivation (or $(K, \varepsilon)$-derivation) of degree $\delta \in \Delta$ of $(A, A', A'')$ into $(B, B', B'')$ is a triple of graded $K$-linear mappings of degree $\delta$:*
$$
d : A \to B, \qquad d' : A' \to B', \qquad d'' : A'' \to B''
$$
*such that, for every homogeneous element $a \in A$ and every element $a' \in A'$*
(4)
$$
d''(a.a') = (da).a' + \varepsilon_{\delta, \deg(a)}a.(d'a').
$$

It obviously suffices by linearity to verify relation (4) when $a$ and $a'$ run through respective generating systems of $A$ and $A'$.

It is often convenient to denote the three mappings $d, d', d''$ by the same letter $d$ (which can be justified by denoting equally by $d$ the graded $K$-linear mapping of degree $\delta$)

$$
(a, a', a'') \mapsto (da, d'a', d''a'')
$$

of $A \oplus A' \oplus A''$ into $B \oplus B' \oplus B''$). Relation (4) can then be written more simply
$$
d(a.a') = (da).a' + \varepsilon_{\delta,\deg(a)} a.(da').
$$
The $\varepsilon$-derivations of $(A, A', A'')$ into $(B, B', B'')$ of *given* degree form a sub-K-module of the K-module of graded linear mappings
$$
\operatorname{Hom}_{\mathbf{K}}(A \oplus A' \oplus A'', B \oplus B' \oplus B'').
$$
When $\varepsilon(\alpha, \beta) = 1$ for all $\alpha, \beta$ in $\Delta$, we say simply *derivation* (or *K-derivation*) instead of $\varepsilon$-derivation. Derivations form a sub-K-module of
$$
\operatorname{Hom}_{\mathbf{K}}(A \oplus A' \oplus A'', B \oplus B' \oplus B'').
$$
When $\Delta = \mathbf{Z}$ and $\varepsilon(p.q) = (-1)^{pq}$, every $\varepsilon$-derivation of *even* degree is a derivation; every $\varepsilon$-derivation of *odd* degree is often called an *antiderivation* (or *K-antiderivation*); an antiderivation $d$ therefore satisfies
$$
d(a.a') = (da).a' + (-1)^{\deg(a)} a.(da')
$$
for a *homogeneous* element $a \in A$.

#### Remark {#alg-iii-s10-n2-rem-1 .statement}

(1) The notion of *derivation* can be defined for non-graded modules by agreeing to give these modules the trivial graduation.

(2) If only $\varepsilon$-derivations of given degree $\delta$ are considered, the commutation factor $\varepsilon$ may be disposed of as follows: the bilinear mapping $\lambda_2 : A \times B' \to B''$ is modified by replacing it by the bilinear mapping $\lambda'_2 : A \times B' \to B''$ such that, for every *homogeneous* $a$ in $A$ and all $b' \in B'$,
$$
\lambda'_2(a, b') = \varepsilon_{\delta, \deg(a)} \lambda_2(a, b').
$$
Then $d$ is a derivation relative to the bilinear mappings $\mu, \lambda_1, \lambda'_2$.

The general definition of $\varepsilon$-derivations given above is especially used in two cases:

*Case (I)*: $A = B, A' = B', A'' = B''$ and the three bilinear mappings $\mu, \lambda_1, \lambda_2$ are equal to the *same* mapping.

*Case (II)*: $A = A' = A'', B = B' = B''$, so that (for $\mu$) $A$ is a *graded algebra* and the two K-bilinear mappings.
$$
\lambda_1 : B \times A \to B, \quad \lambda_2 : A \times B \to B
$$
are such that the corresponding K-linear mappings $B \otimes_K A \to B, A \otimes_K B \to B$ are graded of degree 0. An $\varepsilon$-derivation of degree $\delta$ of $A$ into $B$ is then a graded K-linear mapping $d : A \to B$ of degree $\delta$, such that for every homogeneous $x$ in $A$ and every $y \in A$, we have the relation
$$
d(xy) = (dx)y + \varepsilon_{\delta, \deg(a)} x(dy).
$$

Consider in particular in case (II) the case where A is a unital associative K-algebra and $\lambda_1$ and $\lambda_2$ are the external laws of an (A, A)-bimodule (§ 4, no. 3, Definition 3). This holds notably when A and B are two unital associative K-algebras, a unital homomorphism of graded K-algebras $\rho : A \to B$ is given and an (A, A)-bimodule structure is considered on B defined by the two external laws

$$
\lambda_1 : (b, a) \mapsto b \rho(a), \qquad \lambda_2 : (a, b) \mapsto \rho(a)b
$$

for $a \in A, b \in B$.

Cases (I) and (II) have the following case in common: consider a graded K-algebra A, take $B = A$, mappings (7) both being multiplication on A. We then speak of an $\varepsilon$-derivation (or (K, $\varepsilon$)-derivation) of the graded algebra A: it is a graded K-linear mapping of A into itself, of degree $\delta$, satisfying (8) for every homogeneous $x$ in A and all $y \in A$. In particular if A is a graded ring, considered as an (associative) $\mathbf{Z}$-algebra, we speak of the $\varepsilon$-derivation of the ring A.

Let A be a unital commutative associative K-algebra and B an A-module; when we speak of a derivation of A into B, it will always be understood that we mean with the A-bimodule structure on B derived from its A-module structure; then the formula

$$
d(xy) = x(dy) + y(dx) \quad \text{for} \quad x \in A, y \in A
$$

holds for such a derivation $d : A \to B$.

### 3. EXAMPLES OF DERIVATIONS

#### Example 1 {#alg-iii-s10-n3-exa-1 .statement}

Let A be an $\mathbf{R}$-algebra of differentiable mappings of $\mathbf{R}$ into $\mathbf{R}$ and let $x_0$ be a point of $\mathbf{R}$; $\mathbf{R}$ can be considered as an A-module with the external law $(f, a) \mapsto f(x_0)a$. Then the mapping $f \mapsto Df(x_0)$ is a derivation, since (Functions of a Real Variable, I, § 1, no. 3)

$$
(D(fg))(x_0) = (Df(x_0))g(x_0) + f(x_0)(Dg(x_0)).*
$$

#### Example 2 {#alg-iii-s10-n3-exa-2 .statement}

Let X be a differentiable manifold of class $C^\infty$ and let A be the graded $\mathbf{R}$-algebra of differential forms on X. The mapping which associates with every differential form $\omega$ on X its exterior differential $d\omega$ is an anti-derivation of degree +1 (Differentiable and Analytic Manifolds, R, § 8).*

#### Example 3 {#alg-iii-s10-n3-exa-3 .statement}

Let A be an associative K-algebra. For all $a \in A$, the mapping $x \mapsto ax - xa$ is a derivation of the algebra A (cf. no. 6).

#### Example 4 {#alg-iii-s10-n3-exa-4 .statement}

Let M be a K-module and A the exterior algebra $\bigwedge(M^*)$ with its usual graduation (§ 7, no. 1). *It will be seen in § 11, no. 9 that, for all $x \in M$, the right interior product $i(x)$ is an antiderivation of A of degree $-1$.*

#### Example 5 {#alg-iii-s10-n3-exa-5 .statement}

Returning to the general situation of Definition 1 of no. 2, let $\overline{K}$ be another commutative ring and $\rho : K \to \overline{K}$ a ring homomorphism; let $\overline{A}, \overline{A}', \overline{A}'', \overline{B}, \overline{B}', \overline{B}''$ denote the graded $\overline{K}$-modules obtained respectively from $A, A', A'', B, B', B''$ by extending the ring of scalars to $\overline{K}$ (II, § 11, no. 5); we derive from $\mu, \lambda_1$ and $\lambda_2$ $\overline{K}$-bilinear mappings
$$
\bar{\mu} : \overline{A} \times \overline{A}' \to \overline{A}'', \quad \bar{\lambda}_1 : \overline{B} \times \overline{A}' \to \overline{B}'', \quad \bar{\lambda}_2 : \overline{A} \times \overline{B}' \to \overline{B}''
$$
by considering the tensor products by $l_{\overline{K}}$ of the corresponding $K$-linear mappings to $\mu, \lambda_1$ and $\lambda_2$ (II, § 5, no. 1). Then, if $d$ is an $\varepsilon$-derivation of degree $\delta$ of $(A, A', A'')$ into $(B, B', B'')$, the mapping $\bar{d} = d \otimes l_{\overline{K}}$ of $\overline{A} \oplus \overline{A}' \oplus \overline{A}''$ into $\overline{B} \oplus \overline{B}' \oplus \overline{B}''$ is an $\varepsilon$-derivation of degree $\delta$ of $(\overline{A}, \overline{A}', \overline{A}'')$ into $(\overline{B}, \overline{B}', \overline{B}'')$.

#### Example 6 {#alg-iii-s10-n3-exa-6 .statement}

Let $A$ be a graded $K$-algebra of type $\mathbf{Z}$; a graded linear $K$-mapping of degree 0, $d : A \to A$, is defined by taking, for $x_n \in A_n (n \in \mathbf{Z})$, $d(x_n) = nx_n$. This mapping is a derivation of $A$, since, for $x_p \in A_p, x_q \in A_q$,
$$
d(x_p x_q) = (p + q)x_p x_q = d(x_p)x_q + x_p d(x_q).
$$

### 4. COMPOSITION OF DERIVATIONS

We suppose in this no. that case (I) of no. 2 holds, that is that $A, A', A''$ are three graded $K$-modules of type $\Delta$ and that we are given a $K$-bilinear mapping $\mu : A \times A' \to A''$ corresponding to a graded $K$-linear mapping of degree 0, $A \otimes_K A' \to A''$. The graded endomorphisms $f$ of $A \oplus A' \oplus A''$ such that $f(A) \subset A, f(A') \subset A'$ and $f(A'') \subset A''$ form a graded subalgebra of the graded associative algebra $\mathrm{Endgr}_K(A \oplus A' \oplus A'')$ (§ 3, no. 1, Example 2). In particular two $\varepsilon$-derivations of $(A, A', A'')$ can be composed, but it should not be thought that the composition of two $\varepsilon$-derivations is an $\varepsilon$-derivation.

On every graded algebra $B$ of type $\Delta$ is defined the $\varepsilon$-bracket (or simply bracket when $\varepsilon = 1$) of two homogeneous elements $u, v$, by the formula (10)
$$
[u, v]_\varepsilon = uv - \varepsilon_{\deg u, \deg v} vu \text{ (denoted simply by } [u, v] \text{ if } \varepsilon = 1).
$$
By extending this mapping by linearity, a $K$-bilinear mapping $(u, v) \mapsto [u, v]_\varepsilon$ of $B \times B$ into $B$ is obtained. Then, for homogeneous $u$ and $v$ in $B$
$$
[v, u]_\varepsilon = -\varepsilon_{\deg u, \deg v}[u, v]_\varepsilon.
$$
Applying this definition to the graded algebra $\mathrm{Endgr}_K(A \oplus A' \oplus A'')$, the $\varepsilon$-bracket of two graded endomorphisms is thus defined.

#### Proposition 1 {#alg-iii-s10-prop-1 .statement}

*Let $d_1, d_2$ be two $\varepsilon$-derivations of $(A, A', A'')$ of respective degrees $\delta_1, \delta_2$. Then the $\varepsilon$-bracket*
$$
[d_1, d_2]_\varepsilon = d_1 \circ d_2 - \varepsilon_{\delta_1, \delta_2} d_2 \circ d_1
$$
*is an $\varepsilon$-derivation of degree $\delta_1 + \delta_2$. Moreover, if $d$ is an $\varepsilon$-derivation of $(A, A', A'')$ of degree $\delta$ and if $\varepsilon_{\delta, \delta} = -1$, then $d^2 = d \circ d$ is a derivation.*

Suppose $x \in A$ is homogeneous of degree $\xi$; for all $y \in A'$,
$$
d_1(d_2(xy)) = ((d_1 d_2)(x))y + \varepsilon_{\delta_1, \delta_2 + \xi}(d_2 x)(d_1 y)
+ \varepsilon_{\delta_2, \xi}(d_1 x)(d_2 y) + \varepsilon_{\delta_1 + \delta_2, \xi} x((d_1 d_2)(y))
$$
taking account of formulae (1) of no. 1. Exchanging the roles of $d_1$ and $d_2$, we obtain, after simplifications again using (1) (no. 1),
$$
(d_1 d_2)(xy) - \varepsilon_{\delta_1, \delta_2}(d_2 d_1)(xy) = ((d_1 d_2)(x))y - \varepsilon_{\delta_1, \delta_2}((d_2 d_1)(x))y
+ \varepsilon_{\delta_1 + \delta_2, \xi} x((d_1 d_2)(y))
- \varepsilon_{\delta_1, \delta_2} \varepsilon_{\delta_1 + \delta_2, \xi} x((d_2 d_1)(y))
$$
that is, writing $d = [d_1, d_2]_\varepsilon$ and $\delta = \delta_1 + \delta_2$,
$$
d(xy) = (dx)y + \varepsilon_{\delta, \xi} x(dy)
$$
which proves that $d$ is an $\varepsilon$-derivation.

On the other hand, if, in (11), we let $d_1 = d_2 = d$, $\delta_1 = \delta_2 = \delta$ and $\varepsilon_{\delta, \delta} = -1$, we obtain, since then $\varepsilon_{\delta, \delta + \xi} = -\varepsilon_{\delta, \xi}$ by (1),
$$
d^2(xy) = (d^2 x)y + \varepsilon_{2\delta, \xi} x(d^2 y)
$$
and as $\varepsilon_{2\delta, \xi} = 1$ it is seen that $d^2$ is a derivation.

#### Corollary {#alg-iii-s10-n4-cor-1 .statement}

*Suppose that $\Delta = \mathbf{Z}$. Then:*
(i) *The square of an antiderivation is a derivation.*
(ii) *The bracket of two derivations is a derivation.*
(iii) *The bracket of an antiderivation and a derivation of even degree is an antiderivation.*
(iv) *If $d_1$ and $d_2$ are antiderivations, $d_1 d_2 + d_2 d_1$ is a derivation.*

Under the hypotheses of the beginning of this no., consider now a finite sequence $D = (d_i)_{1 \leq i \leq n}$ of *pairwise permutable derivations* of $(A, A', A'')$. For every polynomial $P(X_1, \ldots, X_n)$ in the algebra $K[X_1, \ldots, X_n]$, the element $P(d_1, \ldots, d_n)$ of $\mathrm{Endgr}_K(A \oplus A' \oplus A'')$ is then defined (§ 2, no. 9); its abbreviated notation is $P(D)$.

#### Proposition 2 {#alg-iii-s10-prop-2 .statement}

*With the above hypotheses and notation, consider 2n indeterminates $T_1, \ldots, T_n, T'_1, \ldots, T'_n$ and for every polynomial $F \in K[X_1, \ldots, X_n]$ write $F(T) = F(T_1, \ldots, T_n), F(T') = F(T'_1, \ldots, T'_n)$ and*
$$
F(T + T') = F(T_1 + T'_1, \ldots, T_n + T'_n).
$$
*Suppose that*
$$
P(T + T') = \sum_i Q_i(T) R_i(T')
$$
*where the $Q_i$ and $R_i$ belong to $K[X_1, \ldots, X_n]$. Then, for all $x \in A$ and $y \in A'$,*
$$
P(D)(xy) = \sum_i (Q_i(D)x)(R_i(D)y).
$$

We introduce $n$ other indeterminates $T_1'', \ldots, T_n''$ and consider the polynomial algebra $K[T_1, \ldots, T_n, T_1', \ldots, T_n', T_1'', \ldots, T_n''] = B$; on the other hand we consider the $K$-module $M$ of bilinear mappings of $A \times A'$ into $A''$; a $B$-module structure is defined on $M$ by writing, for every $K$-bilinear mapping $f \in M$ and $1 \leq i \leq n$,

$$
\begin{cases}
(T_i f)(a, a') = f(d_i a, a') \\
(T_i' f)(a, a') = f(a, d_i a') \\
(T_i'' f)(a, a') = d_i(f(a, a'))
\end{cases}
$$

Since the $d_i$ are permutable with one another, it is seen that, for every polynomial $F \in K[X_1, \ldots, X_n]$, $(F(T)f)(a, a') = f(F(D)a, a')$,

$$
(F(T')f)(a, a') = f(a, F(D)a')
$$

and $(F(T'')f) = F(D)(f(a, a'))$. Hence, to prove (12) it suffices to show that

$$
(P(T'') - \sum_i Q_i(T)R_i(T')).\mu = 0
$$

or also $(P(T'') - P(T + T')).\mu = 0$ in the $B$-module $M$. Now, the hypothesis that the $d_i$ are derivations can also be expressed by saying that, for $1 \leq i \leq n$,

$$
(T_i'' - T_i - T_i').\mu = 0
$$

in the $B$-module $M$. By considering successively the polynomials

$P(T_1'', T_2'', \ldots, T_n'') - P(T_1 + T_1', T_2'', \ldots, T_n'')$
$P(T_1 + T_1', T_2'', \ldots, T_n'') - P(T_1 + T_1', T_2 + T_2', \ldots, T_n'')$
$\ldots$
$P(T_1 + T_1', \ldots, T_{n-1} + T_{n-1}', T_n'') - P(T_1 + T_1', \ldots, T_{n-1} + T_{n-1}', T_n + T_n')$

it is seen that the difference $P(T'') - P(T + T')$ can be written in the form

$$
\sum_{i=1}^n (T_i'' - T_i - T_i') G_i(T, T', T'')
$$

where the $G_i$ are elements of $B$. Relation (14) is therefore an immediate consequence of relations (15).

#### Corollary (Leibniz's formula) {#alg-iii-s10-n4-cor-2 .statement}

*Let $d_i$ ($1 \leq i \leq n$) be $n$ derivations of $(A, A', A'')$ which are permutable with one another. For all $\alpha = (\alpha_1, \ldots, \alpha_n) \in \mathbf{N}^n$, we write*

$$
d^\alpha = d_1^{\alpha_1} d_2^{\alpha_2} \ldots d_n^{\alpha_n}.
$$

Then, for $x \in \mathbf{A}$ and $y \in \mathbf{A}'$,

$$
d^\alpha(xy) = \sum_{\beta + \gamma = \alpha} ((\beta, \gamma)) d^\beta(x)d^\gamma(y)
$$

where we have written (in the notation introduced at the beginning of the chapter)

$$
((\beta, \gamma)) = (\beta + \gamma)!/(\beta! \gamma!).
$$

This follows immediately from the multinomial formula (I, § 8, no. 2)

$$
(T + T')^\alpha = \sum_{\beta + \gamma = \alpha} ((\beta, \gamma)) T^\beta {T'}^\gamma
$$

and Proposition 2.

### 5. DERIVATIONS OF AN ALGEBRA A INTO AN A-MODULE

We suppose in this no. that Case (II) of no. 2 holds. Then there is a graded K-algebra A and a graded K-module E and also two K-linear mappings of degree 0

$$
E \otimes_K A \to E, \quad A \otimes_K E \to E
$$

denoted by

$$
x \otimes a \mapsto x.a \quad \text{and} \quad a \otimes x \mapsto a.x \quad \text{for } a \in A \text{ and } x \in E.
$$

#### Proposition 3 {#alg-iii-s10-prop-3 .statement}

Let $d : A \to E$ be an $\varepsilon$-derivation of degree $\delta$. Then $\mathrm{Ker}(d)$ is a graded subalgebra of A; if A admits a unit element, it belongs to $\mathrm{Ker}(d)$.

Clearly $\mathrm{Ker}(d)$ is a graded sub-K-module of A; further, relation (8) of no. 2 shows that, if $x$ and $y$ are two homogeneous elements belonging to $\mathrm{Ker}(d)$, then $d(xy) = 0$ and hence $xy \in \mathrm{Ker}(d)$. Finally, if A admits a unit element 1 (of degree 0, cf. § 3, no. 1), relation (8) of no. 2, where $x$ and $y$ are replaced by 1, gives $d(1) = d(1) + d(1)$ and hence $d(1) = 0$.

#### Corollary {#alg-iii-s10-n5-cor-1 .statement}

Let $d_1$ and $d_2$ be two $\varepsilon$-derivations from A to E of the same degree $\delta$. If $d_1$ and $d_2$ take the same values at each element of a generating system of the algebra A, then $d_1 = d_2$.

$d_1 - d_2$ is an $\varepsilon$-derivation of degree $\delta$, hence $\mathrm{Ker}(d_1 - d_2)$ is a subalgebra of A which contains a generating system of A and hence is equal to A.

#### Proposition 4 {#alg-iii-s10-prop-4 .statement}

Let $d : A \to E$ be an $\varepsilon$-derivation of degree $\delta$. Suppose that A has a unit element 1 and let $x$ be a homogeneous element of A with an inverse $x^{-1}$ in A. Then

$$
d(x^{-1}) = -\varepsilon_{\delta, \deg(x)} x^{-1}((dx)x^{-1}) = -\varepsilon_{\delta, \deg(x)} (x^{-1}(dx))x^{-1}.
$$

We have $d(xx^{-1}) = d(1) = 0$ (Proposition 3), whence
$$
(dx)x^{-1} + \varepsilon_{\delta, \deg(x)} x(d(x^{-1})) = 0
$$
which proves the first formula of (19). On the other hand, $x^{-1}$ is homogeneous of degree $-\deg(x)$ and $\varepsilon_{\delta, \deg(x)} = \varepsilon_{\delta, -\deg(x)}$ by formulae (1) of no. 1; writing $d(x^{-1}x) = 0$, the second formula of (19) is obtained similarly.

#### Proposition 5 {#alg-iii-s10-prop-5 .statement}

*Suppose that $\mathbf{A}$ is an integral domain and let $\mathbf{L}$ be its field of fractions. Every derivation of $\mathbf{A}$ into a vector space $\mathbf{E}$ over $\mathbf{L}$ (considered as an $\mathbf{A}$-module) can be extended uniquely to a derivation of $\mathbf{L}$ into $\mathbf{E}$.*

Let $d$ be a derivation of $\mathbf{A}$ into $\mathbf{E}$ and $\bar{d}$ a derivation of $\mathbf{L}$ into $\mathbf{E}$ extending $d$; then, for $u \in \mathbf{A}, v \in \mathbf{A}, v \neq 0$, of necessity, by virtue of (19),
$$
\bar{d}(u/v) = v^{-1}du - uv^{-2}dv
$$
which proves the uniqueness of $\bar{d}$. Conversely, we show that $\bar{d}$ can be defined by formula (20); it must first be verified that if $u/v = u'/v'$ the value of the right hand side of (20) does not change when $u$ is replaced by $u'$ and $v$ by $v'$. Now, $uv' = vu'$, hence $v'(du) + u(dv') = v(du') + u'(dv)$ and therefore $v'(du - uv^{-1}dv) = v(du' - u'{v'}^{-1}dv')$, since $uv'v^{-1} = u'$ and $u'{v'}^{-1}v = u$. Thus a mapping $\bar{d}: \mathbf{L} \to \mathbf{E}$ has been defined which extends $d$; it is immediately verified that it is $\mathbf{K}$-linear and a derivation.

#### Proposition 6 {#alg-iii-s10-prop-6 .statement}

*Suppose that $\mathbf{A}$ is a unital associative graded $\mathbf{K}$-algebra and $\mathbf{E}$ a graded $(\mathbf{A}, \mathbf{A})$-bimodule. If $d : \mathbf{A} \to \mathbf{E}$ is an $\varepsilon$-derivation of degree $\delta$, then, for every finite sequence $(x_i)_{1 \leq i \leq n}$ of homogeneous elements of $\mathbf{A}$, of respective degrees $\xi_i$ ($1 \leq i \leq n$),
$$
d(x_1 x_2 \ldots x_n) = \sum_{i=1}^n \varepsilon_{\delta, \xi_1 + \cdots + \xi_{i-1}} x_1 \cdots x_{i-1} (dx_i) x_{i+1} \cdots x_n.
$$
Formula (21) is trivial for $n = 0$ and is proved by induction on $n$, taking account of (4) (no. 2).

#### Corollary {#alg-iii-s10-n5-cor-2 .statement}

*Suppose that $\mathbf{A}$ is a unital commutative associative algebra and $\mathbf{E}$ an $\mathbf{A}$-module. If $d : \mathbf{A} \to \mathbf{E}$ is a derivation, then, for every integer $n \geq 0$,
$$
d(x^n) = nx^{n-1}(dx) \quad \text{for all } x \in \mathbf{A}.
$$
It suffices to give $\mathbf{A}$ the trivial graduation and apply (21) with all the $x_i$ equal to $x$.

We return to the general case of an $\varepsilon$-derivation $d : \mathbf{A} \to \mathbf{E}$ of degree $\delta$. Let $Z_\delta$ be the set of $a \in \mathbf{A}$ such that for every homogeneous component $a_\alpha$ of $a$ of degree $\alpha$, for every homogeneous $x$ in $\mathbf{E}$,
$$
xa_\alpha = \varepsilon_{\alpha, \deg(x)} a_\alpha x.
$$

If $A$ is a unital associative graded algebra and $E$ a graded $(A, A)$-bimodule it follows immediately from this definition that $Z_\varepsilon$ is a *graded subalgebra* of $A$ containing the unit element.

#### Proposition 7 {#alg-iii-s10-prop-7 .statement}

*Suppose that $A$ is a unital associative graded algebra and $E$ a graded $(A, A)$-bimodule. Let $d : A \to E$ be an $\varepsilon$-derivation of degree $\delta$ and $a$ a homogeneous element of $Z_\varepsilon$ of degree $\alpha$. Then the mapping $x \mapsto a(dx)$ is an $\varepsilon$-derivation of degree $\delta + \alpha$.*

We write $d'(x) = a(dx)$; for $x$ homogeneous of degree $\xi$ in $A$ and $y \in A$, by virtue of (23) and (1) (no. 1),

$$
d'(xy) = a((dx)y) + \varepsilon_{\delta, \xi} a(x(dy)) = (a(dx))y + \varepsilon_{\delta+\alpha, \xi}(xa)(dy)
= (d'x)y + \varepsilon_{\delta+\alpha, \xi} x(d'y).
$$

Proposition 7 says that the K-module of $\varepsilon$-derivations of $A$ into $E$ is a *graded $Z_\varepsilon$*-module of type $\Delta$.

### 6. DERIVATIONS OF AN ALGEBRA

Let $A$ be a graded K-algebra; for every *homogeneous* element $a \in A$, let $\mathrm{ad}_\varepsilon(a)$, or simply $\mathrm{ad}(a)$ if no confusion can arise, denote the K-linear mapping of $A$ into $A$

$$
x \mapsto [a, x]_\varepsilon
$$
(no. 4, formula (10)) which is *graded of degree* $\deg a$.

#### Proposition 8 {#alg-iii-s10-prop-8 .statement}

*Let $A$ be a graded K-algebra.*

(i) *For every $\varepsilon$*-derivation $d : A \to A$ and every homogeneous element $a$ of $A$,

$$(24)$$
$$
[d, \mathrm{ad}_\varepsilon(a)]_\varepsilon = \mathrm{ad}_\varepsilon(da).
$$

(ii) *If the algebra $A$ is associative, $\mathrm{ad}_\varepsilon(a)$ is an $\varepsilon$*-derivation of $A$ of degree $\deg(a)$.

(i) Suppose that $d$ is of degree $\delta$, let $\alpha = \deg a$ and write $f = [d, \mathrm{ad}_\varepsilon(a)]_\varepsilon$. For every homogeneous element $x \in A$ of degree $\xi$, we have, by (1) (no. 1),

$$
f(x) = d(ax - \varepsilon(\alpha, \xi) xa) - \varepsilon_{\delta, \alpha}(a(dx)) - \varepsilon_{\alpha, \delta+\xi}(dx)a \\
= (da)x + \varepsilon_{\delta, \alpha} a(dx) - \varepsilon_{\alpha, \xi}(dx)a - \varepsilon_{\delta+\alpha, \xi} x(da) \\
- \varepsilon_{\delta, \alpha} a(dx) + \varepsilon_{\alpha, \xi}(dx)a \\
= (da)x - \varepsilon_{\delta+\alpha, \xi} x(da) = [da, x]_\varepsilon.
$$

(ii) For all $x$ homogeneous of degree $\xi$ and all $y$ homogeneous of degree $\eta$ in $A$,

$$
\mathrm{ad}_\varepsilon(a)(xy) = a(xy) - \varepsilon_{\alpha, \xi+\eta}(xy)a \\
= (ax - \varepsilon_{\alpha, \xi} xa)y + \varepsilon_{\alpha, \xi} x(ay - \varepsilon_{\alpha, \eta} ya) \\
= \mathrm{ad}_\varepsilon(a)(x).y + \varepsilon_{\alpha, \xi} x.\mathrm{ad}_\varepsilon(a)(y)
$$
taking account of (1) and the associativity of $A$.

When $A$ is associative, $\mathrm{ad}_\varepsilon(a)$ is called the *inner $\varepsilon$-derivation* of $A$ defined by $a$.

#### Corollary {#alg-iii-s10-n6-cor-1 .statement}

*Let $A$ be an associative graded algebra. For two homogeneous elements, $a, b$ of $A$,*
$$
[\mathrm{ad}_\varepsilon(a), \mathrm{ad}_\varepsilon(b)]_\varepsilon = \mathrm{ad}_\varepsilon([a, b]_\varepsilon).
$$
(25)

It suffices to replace $d$ by $\mathrm{ad}_\varepsilon(a)$ and $\mathrm{ad}_\varepsilon(a)$ by $\mathrm{ad}_\varepsilon(b)$ in (24).

If $\deg a = \alpha, \deg b = \beta$, formula (25) is equivalent to the following relation for every homogeneous element $c \in A$ of degree $\gamma$
$$
\varepsilon_{\alpha, \gamma}[a, [b, c]_\varepsilon]_\varepsilon + \varepsilon_{\beta, \alpha}[b, [c, a]_\varepsilon]_\varepsilon + \varepsilon_{\gamma, \beta}[c, [a, b]_\varepsilon]_\varepsilon = 0
$$
called the *Jacobi identity*.

### 7. Functorial Properties

*In this no., all algebras are assumed to be associative and unital and every algebra homomorphism is assumed to be unital.*

#### Proposition 9 {#alg-iii-s10-prop-9 .statement}

*Let $A, B$ be two graded $K$-algebras, $E$ an $(A, A)$-bimodule and $F$ a graded $(B, B)$-bimodule; let $\rho : A \to B$ be a graded algebra homomorphism and $\theta : E \to F$ a graded $A$-homomorphism of $A$-bimodules (relative to $\rho$), of degree 0. Then:*

*(i)* *For every $\varepsilon$-derivation $d' : B \to F$, $d' \circ \rho : A \to \rho^*(F)$ is an $\varepsilon$-derivation of the same degree.*
*(ii)* *For every $\varepsilon$-derivation $d : A \to E$, $\theta \circ d : A \to \rho^*(F)$ is an $\varepsilon$-derivation of the same degree.*

The two assertions follow immediately from the relations
$$
d'(\rho(xy)) = d'(\rho(x)\rho(y)) = d'(\rho(x))\rho(y) + \varepsilon_{\delta', \xi}\rho(x)d'(\rho(y))
$$
$$
\theta(d(xy)) = \theta((dx)y + \varepsilon_{\delta, \xi}x(dy)) = \theta(dx)\rho(y) + \varepsilon_{\delta, \xi}\rho(x)\theta(dy)
$$
for $x \in A$ homogeneous of degree $\xi$ and $y \in A$, $\delta$ and $\delta'$ denoting the respective degrees of $d$ and $d'$.

#### Corollary {#alg-iii-s10-n7-cor-1 .statement}

*Let $S$ be a generating system of the algebra $A$. In order that $d' \circ \rho = \theta \circ d$, it is necessary and sufficient that $d'(\rho(x)) = \theta(d(x))$ for all $x \in S$.*

This is an immediate consequence of Proposition 9 and no. 5, Corollary to Proposition 3.

Under the conditions of Proposition 9, we know that $B$ has (by means of $\rho$) an $(A, A)$-bimodule structure (II, § 1, no. 14, *Example 1*).

#### Proposition 10 {#alg-iii-s10-prop-10 .statement}

*Under the conditions of Proposition 9, for an $\varepsilon$-derivation $d' : B \to F$ to be $A$-linear for the left (resp. right) $A$-module structures on $B$ and $\rho^*(F)$, it is necessary and sufficient that $d'$ be zero on the subalgebra $\rho(A)$ of $B$.*

We perform the proof for left A-module structures. For $a \in A, b \in B$,
$$
d'(\rho(a)b) = d'(\rho(a))b + \rho(a)d'b
$$
and hence if $d' \circ \rho = 0$, $d'$ is linear for the left A-module structures on B and $\rho^*(F)$. Conversely, if this is so, in particular
$$
d'(\rho(a)) = d'(\rho(a).1) = \rho(a)d'(1) = 0
$$
(no. 5, Proposition 3).

In particular let $D_K(B, F)$ denote the K-module of derivations of B into F (no. 2); those among these derivations which are A-linear, in other words those which are zero on $\rho(A)$, form a sub-K-module of $D_K(B, F)$, denoted by $D_{A,\rho}(B, F)$ or simply $D_A(B, F)$ (obviously $D_K(B, F) = D_{K,\phi}(B, F)$, where $\phi : K \to B$ is the homomorphism defining the K-algebra structure on B).

Now let A, B, C be three graded K-algebras, $\rho : A \to B, \sigma : B \to C$ two graded algebra homomorphisms and G a graded (C, C)-bimodule; if $D_A(B, G)$, $D_B(C, G)$ and $D_A(C, G)$ denote the respective K-modules $D_{A,\rho}(B, \sigma_*(G))$, $D_{B,\sigma}(C, G)$ and $D_{A,\sigma \circ \rho}(C, G)$, $D_B(C, G)$ is clearly a sub-K-module of $D_A(C, G)$ since $\sigma(\rho(A)) \subset \sigma(B)$.

#### Proposition 11 {#alg-iii-s10-prop-11 .statement}

*Under the above conditions, there is an exact sequence of K-homomorphisms*
$$
0 \to D_B(C, G) \xrightarrow{u} D_A(C, G) \xrightarrow{v} D_A(B, G)
$$
*where u is the canonical injection and v the homomorphism $d \mapsto d \circ \sigma$* (Proposition 9).

The kernel of v is the set of derivations $d : C \to G$ such that $d(\sigma(b)) = 0$ for all $b \in B$, which is precisely the image of u.

### 8. RELATIONS BETWEEN DERIVATIONS AND ALGEBRA HOMOMORPHISMS

We suppose again in this no. that *Case (II)* of no. 2 holds and the graded K-algebra A is not assumed to be associative. Given an element $\delta \in \Delta$, consider the graded K-module E($\delta$) (II, § 11, no. 2) such that
$$
(E(\delta))_\mu = E_{\mu+\delta}
$$
for all $\mu \in \Delta$. We define on the graded K-module $A \oplus E(\delta)$ a *graded K-algebra* structure by setting, for every homogeneous element $a \in A$ and arbitrary elements $a' \in A, x, x'$ in $E(\delta)$
$$
(a, x)(a', x') = (aa', x.a' + \varepsilon_{\delta, \deg(a)} a.x');
$$
the verification of the fact that this multiplication defines a graded ring structure is immediate.

The projection $p : (a, x) \mapsto a$ is called the augmentation of the algebra $A \oplus E(\delta)$ and is a graded algebra homomorphism. The graded K-linear mappings $g : A \to A \oplus E(\delta)$ of degree 0 such that the composition

$$
A \xrightarrow{g} A \oplus E(\delta) \xrightarrow{p} A
$$

is the identity $1_A$ are the mappings of the form $x \mapsto (x, f(x))$, where $f : A \to E$ is a graded K-linear mapping of degree $\delta$.

#### Proposition 12 {#alg-iii-s10-prop-12 .statement}

*For a graded K-linear mapping $f : A \to E$ of degree $\delta$ to be an $\varepsilon$-derivation, it is necessary and sufficient that the mapping $x \mapsto (x, f(x))$ of A into $A \oplus E(\delta)$ be a graded K-algebra homomorphism.*

Using the fact that for $x$ homogeneous in $A$ and $y \in A$

$$
(xy, f(xy)) = (x, f(x)).(y, f(y)),
$$

we obtain, taking account of (28), the equivalent relation

$$
f(xy) = f(x).y + \varepsilon_{\delta, \deg(x)} x.f(y),
$$

whence the proposition.

#### Proposition 13 {#alg-iii-s10-prop-13 .statement}

*For the algebra $A \oplus E(\delta)$ to be associative and unital, it is necessary and sufficient that $A$ be associative and unital, and that the mappings $(a, x) \mapsto a.x$ and $(a, x) \mapsto x.a$ define on $E$ an $(A, A)$-bimodule structure; the unit element of $A \oplus E(\delta)$ is then $(1, 0)$.*

If an element $(u, m) \in A \oplus E(\delta)$ is written as unit element of this algebra, it is immediately found that $u$ must be the unit element of $A$; writing $(u, m).(0, x) = (0, x).(u, m) = (0, x)$, we obtain $u.x = x.u = x$ for $x \in E$ and, writing $(u, m).(u, 0) = (u, 0).(u, m) = (u, 0)$, we obtain $m = 0$. The fact that $A$ is associative when $A \oplus E(\delta)$ is follows from the fact that the augmentation is a surjective homomorphism. The condition $(x.a').a'' = x.(a'.a'')$ is then equivalent to $((0, x)(a', 0))(a'', 0) = (0, x)((a', 0)(a'', 0))$ and similarly the condition $a.(a'.x) = (a.a').x$ is equivalent to

$$
(a, 0)((a', 0)(0, x)) = ((a, 0)(a', 0))(0, x);
$$

finally the condition $a.(x.a') = (a.x).a'$ is equivalent to

$$
(a, 0)((0, x)(a', 0)) = ((a, 0)(0, x))(a', 0).
$$

### 9. EXTENSION OF DERIVATIONS

#### Proposition 14 {#alg-iii-s10-prop-14 .statement}

*Let $A$ be a commutative ring, $M$ an $A$-module, $B$ the $A$-algebra $T(M)$ (resp. $S(M)$, resp. $\Lambda(M)$) and $E$ a $(B, B)$-bimodule. Let $d_0 : A \to E$ be a derivation of the ring $\mathbf{A}$ into the $\mathbf{A}$-module $\mathbf{E}$ and $d_1 : M \to \mathbf{E}$ an additive group homomorphism such that, for all $a \in \mathbf{A}$ and all $x \in M$,

$$
(29) \quad d_1(ax) = ad_1(x) + d_0(a) \cdot x,
$$

and further, when $B = S(M)$,

$$
(30) \quad x \cdot d_1(y) + d_1(x) \cdot y = y \cdot d_1(x) + d_1(y) \cdot x
$$

for all $x, y$ in $M$, and, when $B = \bigwedge(M)$,

$$
(31) \quad x \cdot d_1(x) + d_1(x) \cdot x = 0
$$

for all $x \in M$. Then there exists one and only one derivation $d$ of $B$ (considered as a $\mathbf{Z}$-algebra) into the $(B, B)$-bimodule $\mathbf{E}$ such that $d|_{\mathbf{A}} = d_0$ and $d|_{M} = d_1$.

We take on the $\mathbf{Z}$-module $B \oplus \mathbf{E}$ the associative $\mathbf{Z}$-algebra structure defined by

$$
(b, t)(b', t') = (bb', bt' + tb')
$$

which has $(1, 0)$ as unit element (no. 8, Proposition 13). Under the canonical injection $t \mapsto (0, t)$, $\mathbf{E}$ is identified with a two-sided ideal of $B \oplus \mathbf{E}$ such that $\mathbf{E}^2 = \{0\}$. On the other hand, the mapping $h_0 : B \oplus \mathbf{E}$ defined by $h_0(a) = (a, d_0(a))$ is a unital ring homomorphism (no. 8, Proposition 12); under this mapping, $B \oplus \mathbf{E}$ then becomes an $\mathbf{A}$-algebra. Moreover, if, for all $x \in M$, we write $h_1(x) = (x, d_1(x))$, it follows from the definition of $h_0$ and (29) that $h_1(ax) = h_0(a)h_1(x)$; in other words $h_1$ is an $\mathbf{A}$-linear mapping of $M$ into $B \oplus \mathbf{E}$. Then there exists one and only one $\mathbf{A}$-algebra homomorphism, $h : B \to B \oplus \mathbf{E}$ such that $h|_M = h_1$ (and necessarily $h|_{\mathbf{A}} = h_0$): for, if $B = T(M)$, this follows from $§ 5$, no. 1, Proposition 1; if $B = S(M)$, condition (30) shows that $h(x)h(y) = h(y)h(x)$ for all $x, y$ in $M$ and the conclusion follows from $§ 6$, no. 1, Proposition 2; finally if $B = \bigwedge(M)$, condition (31) shows that $(h(x))^2 = 0$ for all $x \in M$, since $x \wedge x = 0$ and the conclusion follows from $§ 7$, no. 1, Proposition 1. The homomorphism $h$ is such that the composition $p \circ h : B \to B$ with the augmentation $\rho : B \oplus \mathbf{E} \to B$ is the identity $l_B$, for $p \circ h$ and $l_B$ coincide by definition for the elements of $\mathbf{A}$ and those of $M$ and the set of these elements is a generating system of $B$. We can therefore write $h(b) = (b, d(b))$ for all $b \in B$ and the mapping $b \mapsto d(b)$ of $B$ into $\mathbf{E}$ is a derivation with the required properties, by virtue of Proposition 12 of no. 8.

#### Corollary {#alg-iii-s10-n9-cor-1 .statement}

*Let $M$ be a graded $K$-module of type $\Delta$; the $K$-algebras $T(M)$, $S(M)$ and $\bigwedge(M)$ are given the corresponding graduations of type $\Delta' = \Delta \times \mathbf{Z}$ ($§ 5$, no. 5, Proposition 7, $§ 6$, no. 6, Proposition 10 and $§ 7$, no. 7, Proposition 11). On the other hand $M$ is given the graduation of type $\Delta'$ such that $M_{\alpha, 1} = M_{\alpha}$ for all $\alpha \in \Delta$ and $M_{\alpha, n} = \{0\}$ for $\alpha \in \Delta$ and $n \neq 1$. Let $\varepsilon'$ be a commutation factor over $\Delta'$.*

(i) Let E be a graded (left and right) $\mathbf{T}(M)$-bimodule of type $\Delta'$; for all $\delta \in \Delta$ and every integer $n \in \mathbf{Z}$, every graded K-linear mapping $f : M \to E$ of degree $\delta_1' = (\delta, n)$ can be extended uniquely to an $\varepsilon'$-derivation $d : \mathbf{T}(M) \to E$ of degree $\delta'$.

(ii) Let E be a graded $S(M)$-module of type $\Delta'$; for a graded K-linear mapping $f : M \to E$ of degree $\delta'$ to be extendable to an $\varepsilon'$-derivation $d : S(M) \to E$ of degree $\delta'$, it is necessary and sufficient that, for every ordered pair $(x, y)$ of homogeneous elements of M,

$$
x . f(y) + \varepsilon_{\delta', (\deg(y), 1)} y . f(x) = y . f(x) + \varepsilon_{\delta', (\deg(x), 1)} x . f(y).
$$

The $\varepsilon'$-derivation d is then unique.

(iii) Let E be a graded (left and right) $\Lambda(M)$-bimodule of type $\Delta'$; for a graded K-linear mapping $f : M \to E$ of degree $\delta'$ to be extendable to an $\varepsilon'$-derivation

$$
d : \Lambda(M) \to E
$$

of degree $\delta'$, it is necessary and sufficient that, for every homogeneous element x of M,

$$
x . f(x) + \varepsilon_{\delta', (\deg(x), 1)} f(x) . x = 0.
$$

The $\varepsilon'$-derivation d is then unique.

Remark 2 of no. 2 is applied with one of the external B-module laws on E (with B equal to $\mathbf{T}(M)$, $S(M)$ or $\Lambda(M)$) modified; the external law thus modified is still, by (1) (no. 1), a B-module law and the B-module law thus obtained on E is still compatible with the other B-module structure. It then suffices to apply Proposition 14 with $A = K$ and $d_0 = 0$.

Example (1). In the application of Proposition 14 note that if $d_0 = 0$ condition (29) means simply that $d_1$ is A-linear. If we take in particular $E = B$ and the (B, B)-bimodule structure derived from the ring structure on B, conditions (30) and (31) are automatically satisfied when $d_1$ is taken to be the composition of an endomorphism s of M and the canonical injection $M \to B$; this is obvious for (30) since $S(M)$ is commutative and for (31) this follows from the fact that x and $s(x)$ are of degree 1 in $\Lambda(M)$. It is therefore seen that every endomorphism s of M can be extended uniquely to a derivation $D_s$ of $\mathbf{T}(M)$ (resp. $S(M)$, resp. $\Lambda(M)$), which is of degree 0. Moreover, for two endomorphisms s, t of M,

$$
[D_s, D_t] = D_{[s, t]}
$$

for both sides are derivations of $\mathbf{T}(M)$ (resp. $S(M)$, resp. $\Lambda(M)$) which are equal to $[s, t]$ on M.

The expression for $D_s$ is obtained using formula (21) of no. 5, which gives respectively, for $x_1, x_2, \ldots, x_n$ in $M$,

$$
\begin{cases}
D_s(x_1 \otimes x_2 \otimes \cdots \otimes x_n) \\
\phantom{D_s(x_1 \otimes x_2 \otimes \cdots \otimes x_n)} = \sum_{i=1}^n x_1 \otimes \cdots \otimes x_{i-1} \otimes s(x_i) \otimes x_{i+1} \otimes \cdots \otimes x_n \\
D_s(x_1 x_2 \ldots x_n) = \sum_{i=1}^n x_1 \ldots x_{i-1} s(x_i) x_{i+1} \ldots x_n \\
D_s(x_1 \wedge x_2 \wedge \cdots \wedge x_n) \\
\phantom{D_s(x_1 \wedge x_2 \wedge \cdots \wedge x_n)} = \sum_{i=1}^n x_1 \wedge \cdots \wedge x_{i-1} \wedge s(x_i) \wedge x_{i+1} \wedge \cdots \wedge x_n.
\end{cases}
$$

In the case of the algebra $\Lambda(M)$, there is the following interpretation of $D_s$:

#### Proposition 15 {#alg-iii-s10-prop-15 .statement}

*If $M$ is a free $K$-module of finite rank $n$, then, for every endomorphism $s$ of $M$, the restriction to $\Lambda^n(M)$ of the derivation $D_s$ is the homothety of ratio $\operatorname{Tr}(s)$.*

Let $(e_j)_{1 \leq j \leq n}$ be a basis of $M$ and write $e = e_1 \wedge e_2 \wedge \cdots \wedge e_n$. If
$$
s(e_j) = \sum_{k=1}^n \alpha_{jk} e_k,
$$
the third formula in (36) gives
$$
D_s(e) = \sum_{i=1}^n e_1 \wedge \cdots \wedge e_{i-1} \wedge s(e_i) \wedge e_{i+1} \wedge \cdots \wedge e_n = \left( \sum_{j=1}^n \alpha_{jj} \right) e.
$$

*Example (2).* In the Corollary to Proposition 14, part (iii), let $\Delta = \{0\}$, the graduation on $\Lambda(M)$ then being the usual graduation of type $\mathbf{Z}$; on the other hand take $\varepsilon(p, q) = (-1)^{pq}$. Then, for every linear form $x^* \in M^*$ on $M$, $x \mapsto \langle x, x^* \rangle$ is a graded $K$-linear mapping of degree $-1$ of $M$ into $\Lambda(M)$ satisfying relation (34); then there exists an *antiderivation* $i(x^*)$ of $\Lambda(M)$, of degree $-1$, such that (by virtue of formula (21) of no. 5)
$$
i(x^*)(x_1 \wedge \cdots \wedge x_n)
= \sum_{i=1}^n (-1)^{i-1} \langle x_i, x^* \rangle x_1 \wedge \cdots \wedge x_{i-1} \wedge x_{i+1} \wedge \cdots \wedge x_n
$$
and which is a special case of the inner product to be defined in § 11, no. 9, formula (68).

#### Proposition 16 {#alg-iii-s10-prop-16 .statement}

*Let $A$ be a commutative $K$-algebra, $M_i$ ($1 \leq i \leq n$) and $P$ $A$-modules and $H$ the $A$-module of $A$-multilinear mappings of $M_1 \times M_2 \times \cdots \times M_n$* into P. Suppose that there is given a K-derivation $d_0 : A \to A$ of the algebra A, for each i, a K-linear mapping $d_i : M_i \to M_i$ and a K-linear mapping $D : P \to P$, so that, for $1 \leq i \leq n$, $(d_0, d_i, d_i)$ is a K-derivation of $(A, M_i, M_i)$ into itself and $(d_0, D, D)$ is a K-derivation of $(A, P, P)$ into itself. Then there exists a K-linear mapping $D' : H \to H$ such that $(d_0, D', D')$ is a K-derivation of $(A, H, H)$ into itself and

(37) $D(f(x_1, \ldots, x_n))$

$$
= (D'f)(x_1, \ldots, x_n) + \sum_{i=1}^n f(x_1, \ldots, x_{i-1}, d_ix_i, x_{i+1}, \ldots, x_n)
$$

for all $x_i \in M_i$ for $1 \leq i \leq n$ and $f \in H$.

We show that for $f \in H$, the mapping $D'f$ of $M_1 \times M_2 \times \cdots \times M_n$ into P defined by (37) is A-multilinear. For $a \in A$,

$$
(D'f)(ax_1, x_2, \ldots, x_n) = D(af(x_1, \ldots, x_n)) - f(d_1(ax_1), x_2, \ldots, x_n)
$$
$$
-a \sum_{i=2}^n f(x_1, \ldots, x_{i-1}, d_ix_i, x_{i+1}, \ldots, x_n)
$$

and by hypothesis

$$
D(af(x_1, \ldots, x_n)) = (d_0a)f(x_1, \ldots, x_n) + aD(f(x_1, \ldots, x_n))
$$

and $d_1(ax_1) = (d_0a)x_1 + a.d_1x_1$, which gives

$$
(D'f)(ax_1, x_2, \ldots, x_n) = a.(D'f)(x_1, \ldots, x_n)
$$

and linearity in each of the $x_i$ is proved similarly. On the other hand,

$$
(D'(af))(x_1, \ldots, x_n) = D(af(x_1, \ldots, x_n))
$$
$$
- \sum_{i=1}^n af(x_1, \ldots, x_{i-1}, d_ix_i, x_{i+1}, \ldots, x_n)
$$
$$
= (d_0a)f(x_1, \ldots, x_n)) + aD(f(x_1, \ldots, x_n))
$$
$$
- \sum_{i=1}^n af(x_1, \ldots, x_{i-1}, d_ix_i, x_{i+1}, \ldots, x_n)
$$
$$
= (d_0a)f(x_1, \ldots, x_n) + a(D'f)(x_1, \ldots, x_n)
$$

in other words

$$
D'(af) = (d_0a)f + a(D'f)
$$

which establishes the proposition.

#### Example {#alg-iii-s10-n9-exa-1 .statement}

(3) Applying Proposition 16 to the case $n = 1$, $M_1 = M$, $P = A$, then $H = M^*$, the dual of M, and it is seen that for a K-derivation $(d_0, d, d')$ of $(A, M, M)$ is derived a K-derivation $(d_0, d^*, d^*)$ of $(A, M^*, M^*)$ such that

(38) $d_0\langle m, m^*\rangle = \langle dm, m^*\rangle + \langle m, d^*m^*\rangle$

for $m \in M$ and $m^* \in M^*$. The K-linear mapping of $M \oplus M^*$ into itself which is equal to $d$ on $M$ and to $d^*$ on $M^*$ then satisfies condition (29) and there is therefore a $K$-derivation $D$ of the $A$-algebra $T(M \oplus M^*)$, which reduces to $d_0$ on $A$, to $d$ on $M$ and to $d^*$ on $M^*$. The restriction $d_J^I$ of $D$ to the sub-$A$-module $T_J^I(M)$ of $T(M \oplus M^*)$ ($§ 5$, no. 6) is a $K$-endomorphism of $T_J^I(M)$ such that $(d_0, d_J^I, d_J^I)$ is a $K$-derivation of $(A, T_J^I(M), T_J^I(M))$. Moreover, for $i \in I, j \in J$, if we write $I' = I - \{i\}, J' = J - \{j\}$, it is immediately verified that for the contraction $c_j^i$ ($§ 5$, no. 6)

$$
c_j^i(d_J^I(z)) = d_{J'}^{I'}(c_j^i(z)) \quad \text{for all } z \in T_J^I(M).
$$

(4) Let $M_i$ ($1 \leq i \leq 3$) be three $A$-modules and, for each $i$, suppose that $(d_0, d_i, d_i)$ is a derivation of $(A, M_i, M_i)$; applying Proposition 16 again for $n = 1$, a derivation $(d_0, d_{ij}, d_{ij})$ of $(A, H_{ij}, H_{ij})$, where $H_{ij} = \operatorname{Hom}_A(M_i, M_j)$, is derived for each ordered pair $(i, j)$. With this notation, for $u \in \operatorname{Hom}_A(M_1, M_2)$ and $v \in \operatorname{Hom}_A(M_2, M_3)$,

$$
d_{13}(v \circ u) = (d_{23}v) \circ u + v \circ (d_{12}u)
$$
as is immediately verified from the definitions.

### 10. UNIVERSAL PROBLEM FOR DERIVATIONS; NON-COMMUTATIVE CASE

Throughout the rest of $§ 10$ all the algebras are assumed to be associative and unital and all the algebra homomorphisms are assumed to be unital.

Let $A$ be a $K$-algebra; the tensor product $A \otimes_K A$ has canonically an $(A, A)$-bimodule structure under which

$$
x . (u \otimes v) . y = (xu) \otimes (vy)
$$
for all $x, y, u, v$ in $A$ ($§ 4$, no. 3, Example 2). The $K$-linear mapping $m : A \otimes_K A \to A$ corresponding to multiplication in $A$ (and hence such that $m(x \otimes y) = xy$) is an $(A, A)$-bimodule homomorphism; its kernel $I$ is therefore a sub-bimodule of $A \otimes_K A$.

#### Lemma 1 {#alg-iii-s10-lem-1 .statement}

*The mapping $\delta_A : x \mapsto x \otimes 1 - 1 \otimes x$ is a $K$-derivation of $A$ into $I$ and $I$ is generated, as a left $A$-module, by the image of $\delta_A$.*

The first assertion follows from the fact that

$$
(xy) \otimes 1 - 1 \otimes (xy) = (x \otimes 1 - 1 \otimes x) . y + x . (y \otimes 1 - 1 \otimes y)
$$
by (40). On the other hand, if the element $\sum_i x_i \otimes y_i$ (for $x_i, y_i$ in $A$) belongs to $I$, by definition $\sum_i x_i y_i = 0$ and hence

$$
\sum_i (x_i \otimes y_i) = \sum_i x_i (1 \otimes y_i - y_i \otimes 1)
$$
by (40), which completes the proof of the lemma.

#### Proposition 17 {#alg-iii-s10-prop-17 .statement}

*The derivation* $\delta_A$ *has the following universal property*: for every $(A, A)$-bimodule $E$ and every $K$-derivation $d : A \to E$, there exists one and only one $(A, A)$-bimodule homomorphism $f : I \to E$ such that $d = f \circ \delta_A$.

Note first that, for every $(A, A)$-bimodule homomorphism $f : I \to E$, $f \circ \delta_A$ is a derivation (no. 7, Proposition 9). Conversely, let $d : A \to E$ be a K-derivation; then we prove first that if there exists an $(A, A)$-bimodule homomorphism $f : I \to E$ such that $d = f \circ \delta_A$, $f$ is *uniquely determined* by this condition for the definition of $\delta_A$ gives

$$
f(x \otimes 1 - 1 \otimes x) = dx
$$

and our assertion follows from the fact that the image of $\delta_A$ already generates I as a left A-module (Lemma 1): hence of necessity

$$
f\left( \sum_i x_i \otimes y_i \right) = \sum_i x_i \cdot f(1 \otimes y_i - y_i \otimes 1) = -\sum_i x_i \cdot dy_i.
$$

Conversely, as the mapping $(x, y) \mapsto -x \cdot dy$ of $A \times A$ into $E$ is $K$-bilinear, there exists one and only one $K$-linear mapping $g : A \otimes_K A \to E$ such that $g(x \otimes y) = -x \cdot dy$; it suffices to verify that the restriction $f$ of $g$ to $I$ is A-linear for the left and right A-module structures. The first assertion is obvious since $(xx') \cdot dy = x \cdot (x' \cdot dy)$; to prove the second, note that, if $\sum_i x_i \otimes y_i \in I$ and $x \in A$, then

$$
\sum_i x_i \cdot d(y_i x) = \sum_i x_i \cdot dy_i \cdot x + \sum_i (x_i y_i) \cdot dx
$$

but since $\sum_i x_i y_i = 0$ by definition of $I$, this completes the proof.

We have thus defined a *canonical* $K$-module *isomorphism* $f \mapsto f \circ \delta_A$

$$
\operatorname{Hom}_{(A, A)}(I, E) \to D_K(A, E)
$$

the left hand side being the $K$-module of $(A, A)$-bimodule homomorphisms of $A$ into $E$.

### 11. UNIVERSAL PROBLEM FOR DERIVATIONS; COMMUTATIVE CASE

Suppose now that $A$ is a *commutative* $K$-algebra and $E$ an $A$-*module*; $E$ can be considered as an $(A, A)$-bimodule whose two external laws are identical with the given $A$-module law. On the other hand the $(A, A)$-bimodule structure on $A \otimes_K A$ is identical with its $(A \otimes_K A)$-module structure arising from the *commutative ring* structure on $A \otimes_K A$, since in this case, for $x, y, u, v$ in $A$,

$$
x \cdot (u \otimes v) \cdot y = (xu) \otimes (vy) = (xu) \otimes (yv) = (x \otimes y)(u \otimes v).
$$

The kernel $\mathfrak{J}$ of $m$ is therefore in this case an *ideal* of the ring $A \otimes_K A$ and, as $m : A \otimes_K A \to A$ is surjective, $(A \otimes_K A)/\mathfrak{J}$ is isomorphic to $A$; if also $E$ is considered as an $(A \otimes_K A)$-module by means of $m$ (in other words the $(A \otimes_K A)$-module $m_*(E)$), the $(A, A)$-*bimodule* homomorphisms $\mathfrak{J} \to E$ are identified with the $(A \otimes_K A)$-*module* homomorphisms $\mathfrak{J} \to E$ (§ 4, no. 3), in other words there is a canonical $K$-module isomorphism.

$$
\operatorname{Hom}_{(A, A)}(\mathfrak{J}, E) \to \operatorname{Hom}_{A \otimes_K A}(\mathfrak{J}, E).
$$

On the other hand, $\mathfrak{J}E = \{0\}$, for the elements $1 \otimes x - x \otimes 1$ generate $\mathfrak{J}$ as an $(A \otimes_K A)$-module (no. 10, Lemma 1) and, for all $z \in E$,

$$
(1 \otimes x - x \otimes 1)z = 0
$$

by virtue of the definition of the $(A \otimes_K A)$-module structure on $E$. Since $\mathfrak{J}$ is contained in the annihilator of the $(A \otimes_K A)$-module $E$ and the $((A \otimes_K A)/\mathfrak{J})$-module structure on $E$ is by definition just the initial $A$-module structure given on $E$, there is, taking account of the canonical isomorphism of

$$
\mathfrak{J} \otimes_K ((A \otimes_K A)/\mathfrak{J})
$$

onto $\mathfrak{J}/\mathfrak{J}^2$ (§ 4, no. 1, Corollary 1 to Proposition 1), a canonical $K$-module isomorphism

$$
\operatorname{Hom}_{A \otimes_K A}(\mathfrak{J}, E) \to \operatorname{Hom}_A(\mathfrak{J}/\mathfrak{J}^2, E).
$$

Taking account of Proposition 17 of no. 10, it is seen that we have proved the following proposition:

#### Proposition 18 {#alg-iii-s10-prop-18 .statement}

*Let $A$ be a commutative $K$-algebra and $\mathfrak{J}$ the ideal the kernel of the surjective canonical homomorphism $m : A \otimes_K A \to A$, so that $A$ is isomorphic to $(A \otimes_K A)/\mathfrak{J}$ and $\mathfrak{J}/\mathfrak{J}^2$ has canonically an $A$-module structure. Let $d_{A/K} : A \to I/I^2$ be the $K$-linear mapping which associates with every $x \in A$ the class of $x \otimes 1 - 1 \otimes x$ modulo $\mathfrak{J}^2$. The mapping $d_{A/K}$ is a $K$-derivation and, for every $A$-module $E$ and every $K$-derivation $D : A \to E$, there exists one and only one $A$-linear mapping $g : \mathfrak{J}/\mathfrak{J}^2 \to E$ such that $D = g \circ d_{A/K}$.*

#### Example {#alg-iii-s10-n11-exa-1 .statement}

Let M be a K-module; it follows from Proposition 14 of no. 9 that for every S(M)-module E, the mapping D ↦ D | M defines an S(M)-module isomorphism of D_K(S(M), E) onto Hom_K(M, E); on the other hand, since E is an S(M)-module, Hom_K(M, E) is canonically isomorphic to

$$
\operatorname{Hom}_{S(M)}(M \otimes_K S(M), E),
$$

every K-homomorphism of M into E being uniquely expressible in the form $x \mapsto h(x \otimes 1)$, where

$$
h \in \operatorname{Hom}_{S(M)}(M \otimes_K S(M), E)
$$

(II, § 5, no. 1). Let D_0 be the K-derivation $S(M) \to M \otimes_K S(M)$ whose restriction to M is the canonical homomorphism $x \mapsto x \otimes 1$; every K-derivation D : S(M) → E can therefore be written uniquely as $h \circ D_0$ with

$$
h \in \operatorname{Hom}_{S(M)}(M \otimes_K S(M), E).
$$

By the uniqueness of a solution of a universal mapping problem, it is seen that there exists a unique S(M)-module isomorphism

$$
\omega : M \otimes_K S(M) \to \Omega_K(S(M))
$$

such that $D_0 \circ \omega = d_{S(M)/K}$; in other words, for all $x \in M$, $\omega(x \otimes 1) = dx$.

In particular, *if M is a free K-module with basis* $(e_\lambda)_{\lambda \in L}$, $\Omega_K(S(M))$ *is a free S(M)-module with basis the set of differentials* $de_\lambda$. Consider in particular the case where $L = \{1, n\}$, so that S(M) is identified with the polynomial algebra $K[X_1, \ldots, X_n]$ (§ 6, no. 6); for every polynomial $P \in K[X_1, \ldots, X_n]$, we can write uniquely

$$
dP = \sum_{i=1}^n D_i P . dX_i
$$

with $D_i P \in K[X_1, \ldots, X_n]$ and, by virtue of the above, the mappings $P \mapsto D_i P$ are the *K-derivations* of $K[X_1, \ldots, X_n]$ corresponding to the coordinate forms on $\Omega_K(S(M))$ for the basis $(dX_i)$; we also write $\frac{\partial P}{\partial X_i}$ instead of $D_i P$ and this is called the *partial derivative* of P with respect to $X_i$.

### 12. FUNCTIORIAL PROPERTIES OF K-DIFFERENTIALS

#### Proposition 19 {#alg-iii-s10-prop-19 .statement}

*Let*

$$
\begin{array}{ccc}
K & \xrightarrow{\rho} & K' \\
\downarrow \eta & & \downarrow \eta' \\
A & \xrightarrow{u} & A'
\end{array}
$$

*be a commutative diagram of commutative ring homomorphisms*, $\eta$ (resp. $\eta'$) *making*

A (resp. $A'$) into a $K$-algebra (resp. $K'$-algebra). There exists one and only one $A$-linear mapping $v : \Omega_K(A) \to \Omega_{K'}(A')$ rendering commutative the diagram

$$
\begin{array}{ccc}
A & \xrightarrow{u} & A' \\
d_{A/K} \downarrow & & d_{A'/K'} \downarrow \\
\Omega_K(A) & \xrightarrow{v} & \Omega_{K'}(A')
\end{array}
$$

$d_{A'/K'} \circ u$ is a $K$-derivation of $A$ with values in the $A$-module $\Omega_{K'}(A')$; the existence and uniqueness of $v$ then follow from Proposition 18 of no. 11.

The mapping $v$ of Proposition 19 will be denoted by $\Omega(u)$; if there is a commutative diagram of commutative ring homomorphisms

$$
\begin{array}{cccccc}
K & \xrightarrow{\sigma} & K' & \xrightarrow{\sigma'} & K'' \\
\eta \downarrow & & \eta' \downarrow & & \eta'' \downarrow \\
A & \xrightarrow{u} & A' & \xrightarrow{u'} & A''
\end{array}
$$

it follows immediately from the uniqueness property of Proposition 19 that

$$
\Omega(u' \circ u) = \Omega(u') \circ \Omega(u).
$$

Since $\Omega_{K'}(A')$ is an $A'$-module, from $\Omega(u)$ we derive canonically an $A'$-linear mapping

$$(41)$$
$$
\Omega_0(u) : \Omega_K(A) \otimes_A A' \to \Omega_{K'}(A')
$$

such that $\Omega(u)$ is the composition of $\Omega_0(u)$ and the canonical homomorphism $i_A : \Omega_K(A) \to \Omega_K(A) \otimes_A A'$. For every $A'$-module $E'$, there is a commutative diagram

$$
\begin{array}{ccc}
\operatorname{Hom}_{A'}(\Omega_{K'}(A'), E') & \xrightarrow{\operatorname{Hom}(\Omega_0(u), 1_{E'})} & \operatorname{Hom}_{A'}(\Omega_K(A) \otimes_A A', E') \\
\phi_{A'} \downarrow & & \phi_A \circ r_A \downarrow \\
D_{K'}(A', E') & \xrightarrow{C(u)} & D_K(A, E)
\end{array}
$$

where $C(u)$ is the mapping $D \mapsto D \circ u$ (no. 7, Proposition 9) and $r_A$ is the canonical isomorphism

$$
\operatorname{Hom}(i_A, 1_{E'}) : \operatorname{Hom}_{A'}(\Omega_K(A) \otimes_A A', E') \to \operatorname{Hom}_A(\Omega_K(A), E');
$$

this follows immediately from Proposition 19 and the definition of the isomorphisms $\phi_A$ and $\phi_{A'}$.

#### Proposition 20 {#alg-iii-s10-prop-20 .statement}

*Suppose that $A' = A \otimes_K K'$, with $\eta': K' \to A'$ and $u: A \to A'$ the canonical homomorphisms. Then the $A'$-linear mapping*

$$
\Omega_0(u): \Omega_K(A) \otimes_A A' \to \Omega_{K'}(A')
$$

*is an isomorphism.*

By virtue of the fact that in diagram (42) the vertical arrows are bijective, it reduces to proving that, for every $A'$-module $E'$, the homomorphism $C(u): D \mapsto D \circ u$ in diagram (42) is bijective (II, § 2, no. 1, Theorem 1). Now $\mathrm{Hom}(u, 1_{E'}): \mathrm{Hom}_{K'}(A \otimes_K K', E') \to \mathrm{Hom}_K(A, E')$ is an isomorphism (II, § 5, no. 1, Proposition 1) and $C(u)$ is its restriction to $D_{K'}(A', E')$ and hence is injective; moreover, if $f: A' \to E'$ is a $K'$-linear mapping such that

$$
f \circ u: A \to E'
$$

is a $K$-derivation, it follows immediately from the fact that $f$ is $K'$-linear and the fact that $f((x \otimes 1)(y \otimes 1)) = (y \otimes 1)f(x \otimes 1) + (x \otimes 1)f(y \otimes 1)$ for $x, y$ in $A$, that $f$ is a $K'$-*derivation*, the elements $x \otimes 1$ for $x \in A$ forming a generating system of the $K'$-module $A'$; this completes the proof that $C(u)$ is bijective.

From now on we confine our attention to the case where $\rho: K \to K'$ is the *identity mapping* of $K$; every $K$-algebra homomorphism $u: A \to B$ is therefore mapped to a $B$-linear mapping

$$
\Omega_0(u): \Omega_K(A) \otimes_K B \to \Omega_K(B).
$$

On the other hand, we can consider the $B$-module of $A$-*differentials* $\Omega_A(B)$ since $B$ is an $A$-algebra by means of $u$; the canonical derivation $d_{B/A}: B \to \Omega_A(B)$ being *a fortiori* a $K$-derivation, it factorizes uniquely into

$$
B \xrightarrow{d_{B/K}} \Omega_K(B) \xrightarrow{\Omega_u} \Omega_A(B)
$$

where $\Omega_u$ is a $B$-linear mapping (no. 11, Proposition 18). For every $B$-module $E$, there is a commutative diagram

$$
\begin{array}{ccc}
\mathrm{Hom}_B(\Omega_A(B), E) & \xrightarrow{\mathrm{Hom}(\Omega_u, 1_E)} & \mathrm{Hom}_B(\Omega_K(B), E) \\
\downarrow \phi_{A,B} & & \downarrow \phi_{K,B} \\
D_A(B, E) & \xrightarrow{j_u} & D_K(B, E)
\end{array}
$$

where $j_u$ is the canonical injection (no. 7); this follows immediately from Proposition 18 of no. 11.

#### Proposition 21 {#alg-iii-s10-prop-21 .statement}

*The sequence of $B$-linear mappings*

$$
\Omega_K(A) \otimes_A B \xrightarrow{\Omega_0(u)} \Omega_K(B) \xrightarrow{\Omega_u} \Omega_A(B) \to 0
$$

*is exact.*

It reduces to verifying that, for every B-module E, the sequence

$$
0 \to \operatorname{Hom}_B(\Omega_A(B), E) \xrightarrow{\operatorname{Hom}(\Omega_u, 1_E)} \operatorname{Hom}_B(\Omega_K(B), E) \xrightarrow{\operatorname{Hom}(\Omega_0(u), 1_E)} \operatorname{Hom}_B(\Omega_K(A) \otimes_A B, E)
$$

is exact (II, § 2, no. 1, Theorem 1); but by virtue of the fact that in the commutative diagrams (42) and (44) the vertical arrows are isomorphisms, it suffices to show that the sequence

$$
0 \longrightarrow D_A(B, E) \xrightarrow{j_u} D_K(B, E) \xrightarrow{C(u)} D_K(A, E)
$$

is exact, which is just Proposition 11 of no. 7.

We consider now the case where the K-algebra homomorphism $u : A \to B$ is surjective; if $\mathfrak{J}$ is its kernel, B is then isomorphic to $A/\mathfrak{J}$. We consider the restriction $d|_{\mathfrak{J}} : \mathfrak{J} \to \Omega_K(A)$ of the canonical derivation $d = d_{A/K}$ and the composite A-linear mapping

$$
d' : \mathfrak{J} \xrightarrow{d|_{\mathfrak{J}}} \Omega_K(A) \xrightarrow{i_A} \Omega_K(A) \otimes_A B.
$$

Then $d'(\mathfrak{J}^2) = 0$, since, for $x, y$ in $\mathfrak{J}$,

$$
d'(xy) = d(xy) \otimes 1 = (x.dy + y.dx) \otimes 1 = dy \otimes u(x) + dx \otimes u(y) = 0
$$

since $u(x) = u(y) = 0$. Hence we derive from $d'$, by passing to the quotient, an A-linear mapping

$$
\bar{d} : \mathfrak{J}/\mathfrak{J}^2 \to \Omega_K(A) \otimes_A B
$$

and as $\mathfrak{J}$ annihilates the A-module $\mathfrak{J}/\mathfrak{J}^2$, $\bar{d}$ is a B-linear mapping.

#### Proposition 22 {#alg-iii-s10-prop-22 .statement}

*Let $\mathfrak{J}$ be an ideal of the commutative K-algebra A, $B = A/\mathfrak{J}$ and $u : A \to B$ the canonical homomorphism. The sequence of B-linear mappings*

$$
\mathfrak{J}/\mathfrak{J}^2 \xrightarrow{\bar{d}} \Omega_K(A) \otimes_A B \xrightarrow{\Omega_0(u)} \Omega_K(B) \to 0
$$

*is then exact.*

Note that $\Omega_K(A) \otimes_A B$ is identified with $\Omega_K(A)/\mathfrak{J}\Omega_K(A)$ and that the image of $\bar{d}$ is the image of $d(\mathfrak{J})$ in this quotient module; the quotient of $\Omega_K(A) \otimes_A B$ by $\operatorname{Im}(\bar{d})$ is therefore identified with the quotient $\Omega_K(A)/N$, where N is the sub-A-module generated by $\mathfrak{J}\Omega_K(A)$ and $d(\mathfrak{J})$. Moreover, the composite mapping

$$
A \xrightarrow{d_{A/K}} \Omega_K(A) \longrightarrow \Omega_K(A)/N
$$

is a K-derivation (no. 7, Proposition 9) and, since it is zero on $\mathfrak{J}$ by definition of N, it defines, when passing to the quotient, a K-derivation $D_0 : B \to \Omega_K(A)/N$.

Taking account of the uniqueness of the solution of a universal mapping problem, it reduces to proving that, for every B-module E and every K-derivation D: B → E, there exists a unique B-linear mapping g: Ω_K(A)/N → E such that D = g ∘ D_0. But, the composite mapping D ∘ u: A → E is a K-derivation (no. 7, Proposition 9) and hence there exists one and only one A-linear mapping f: Ω_K(A) → E such that f ∘ d_{A/K} = D ∘ u. This relation shows already that f is zero on d(Σ); as also ΣE = {0} since E is a B-module, f is zero on ΣΩ_K(A); hence f is zero on N and defines, when passing to the quotient, a B-linear mapping g: Ω_K(A)/N → E such that g ∘ D_0 = D; the uniqueness of g follows from the uniqueness of f.

It must not be thought that, even if u: A → B is an injective homomorphism, Ω_0(u): Ω_K(A) ⊗_A B → Ω_K(B) is injective (Exercise 5). However we have the following proposition:

#### Proposition 23 {#alg-iii-s10-prop-23 .statement}

Let A be an integral K-algebra, B its field of fractions and u: A → B the canonical injection. Then Ω_0(u): Ω_K(A) ⊗_A B → Ω_K(B) is an isomorphism.

Using the fact that in diagram (42) the vertical arrows are bijective, it reduces to proving that, for every vector space E over B, the mapping C(u): D_K(B, E) → D_K(A, E) is bijective. But this follows from the fact that every K-derivation of A into E can be extended uniquely to a K-derivation of B into E (no. 5, Proposition 5).

### Exercises {#alg-iii-s10-exercises}

See the [exercises for § 10](exercises/s10/).
