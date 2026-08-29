---
book: var
book_title: Variétés différentielles et analytiques
chapter: "1"
chapter_title: VARIÉTÉS DIFFÉRENTIELLES ET ANALYTIQUES, FASCICULE DE RÉSULTATS
section: 1
section_title: Fonctions différentiables
lang: en
source: var-fr
pdf_pages: 0009-0014
extraction: ocr
subsections:
    - "no": 1
      title: Ordre de contact de deux fonctions en un point
      page: 0
      pdf_page: 9
    - "no": 2
      title: Fonctions dérivables en un point
      page: 0
      pdf_page: 10
    - "no": 3
      title: Composition des fonctions dérivables
      page: 0
      pdf_page: 11
    - "no": 4
      title: Produit de fonctions dérivables
      page: 0
      pdf_page: 12
    - "no": 5
      title: Premières variantes du théorème des fonctions implicites
      page: 0
      pdf_page: 12
    - "no": 6
      title: Dérivées partielles
      page: 0
      pdf_page: 13
    - "no": 7
      title: Dérivées itérées
      page: 0
      pdf_page: 13
statements: 0
exercises: 0
content_sha256: 0bf1c162534d51cfbef5c8dce9da23d0a8b404d715eeb87130dd56ee29844bbe
translated_from: content/fr/var/1/01_s1_fonctions_differentiables.md
source_lang: fr
translation_method: machine
source_content_sha256: 68a240194e02f682042deb25f428d16a60db5f87c651da158fc9feeead037a42
translation_model: gpt-5.4
translation_run: translate-en-mt-0f096b99
glossary_version: 34
glossary_terms_sha256: e4f4c9df1df91eccea2fa0dfe437cb5556d45d9853d24811e7e8531064f784ed
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 1. Differentiable functions

In this paragraph, the letter E denotes a normable topological vector space over K; the letter F denotes a separated polynormed space over K.

### 1.1 Order of contact of two functions at a point

1.1.1. Let X be a topological space and $\theta$ a positive numerical function defined in a neighbourhood of a point $x_0$ of X. One says that a function $f$, defined in a neighbourhood of $x_0$ and with values in F, is negligible with respect to $\theta$ at $x_0$ if the following condition is satisfied:

For every $\varepsilon > 0$ and for every continuous seminorm $\gamma$ on F, there exists a neighbourhood V of $x_0$ on which $f$ and $\theta$ are defined and such that

$$
\| f(x) \|_{\gamma} \leq \varepsilon \theta(x) \quad \text{for all } x \in V.
$$

For $f$ to be negligible with respect to $\theta$, it is enough that this condition be satisfied for a family of seminorms $\gamma$ defining the topology of F. The fact that $f$ is or is not negligible with respect to $\theta$ at $x_0$ depends only on the germs of $f$ and of $\theta$ at $x_0$. One denotes by $o_{x_0}(\theta)$ (or $o(\theta)$ when there is no ambiguity about $x_0$) the set of germs at $x_0$ of functions negligible with respect to $\theta$ at $x_0$: it is a vector subspace of the space of germs at $x_0$ of mappings with values in F. If $f$ is negligible with respect to $\theta$, one writes, by abuse of notation, $f \in o_{x_0}(\theta)$ or again $f(x) \in o(\theta(x))$ when $x$ tends to $x_0$.

If $f$ and $g$ are two mappings from a neighbourhood of $x_0$ into F, one also writes $f \equiv g \mod o(\theta)$ if $f - g$ is negligible with respect to $\theta$.

Suppose that K is equal to $\mathbf{R}$ or $\mathbf{C}$ and that $x_0$ is adherent to the set Y of points of X where $\theta$ is defined and non-zero. The relation $f \in o(\theta)$ then means that $f(x)/\theta(x)$ tends to 0 when $x$ tends to $x_0$ while remaining in Y, and that $\theta(x) = 0$ implies $f(x) = 0$.

1.1.2. Let $f$ and $g$ be two functions with values in F, defined in a neighbourhood of a point $x_0$ of E. If $m$ is a positive integer, one says that $f$ and $g$ have contact of order $\geq m$ at $x_0$ if one has:

$$
f(x) - g(x) \in o(\| x - x_0 \|^{m}) \quad \text{for } x \text{ tending to } x_0
$$

whatever norm be chosen to define the topology of E. For this, it is enough that the preceding relation be verified for a norm defining the topology of E. If this is so, one has $f(x_0) = g(x_0)$.

If $f$ and $g$ take the same value at $x_0$, the least upper bound (finite or equal to $+\infty$) of the integers $m$ such that $f$ and $g$ have contact of order $\geq m$ at $x_0$ is called the order of contact of $f$ and $g$ at $x_0$.

1.1.3. The order of contact of $f$ and $g$ at $x_0$ depends only on the germs of these functions at the point $x_0$. One can therefore speak of the order of contact of two germs $\varphi$ and $\psi$ of mappings of E into F at the point $x_0$. The relation “ $\varphi$ and $\psi$ have contact of order $\geq m$ ” is an equivalence relation compatible with the vector space structure.

### 1.2. Differentiable functions at a point

1.2.1. Let $f$ be a function defined in a neighbourhood of the point $x_0$ of E and with values in F. One says that $f$ is differentiable at $x_0$ if there exists a continuous affine function $v$ of E into F having contact of order $\geq 1$ with $f$ at $x_0$. This mapping $v$ is unique; there exists one and only one continuous linear mapping, denoted by $Df(x_0)$, of E into F such that:

$$
v(x) = v(x_0) + Df(x_0) \cdot (x - x_0).
$$

If one chooses a norm on E, this is equivalent to:

$$
f(x_0 + h) \equiv f(x_0) + Df(x_0) \cdot h \mod o(\|h\|) \quad \text{for } h \text{ tending to } 0,
$$

which may also be written in the form:

$$
\lim_{h \to 0, h \neq 0} \frac{\| f(x_0 + h) - f(x_0) - Df(x_0) \cdot h \|_\gamma}{\| h \|} = 0
$$

for every continuous seminorm $\gamma$ on F.

The element $Df(x_0)$ of $\mathcal{L}(E, F)$ is called the derivative of $f$ at $x_0$. One sometimes writes $D_h f(x_0)$ for $Df(x_0) \cdot h$; this is an element of F defined by the relation:

$$
D_h f(x_0) = \lim_{t \to 0, t \neq 0} \frac{f(x_0 + th) - f(x_0)}{t}.
$$

1.2.2. One says that a function $f$ is strictly differentiable at $x_0$ if it is differentiable at $x_0$ and if one has, for every norm defining the topology of E, the relation:

$$
f(y) - f(z) \equiv Df(x_0) \cdot (y - z) \mod o(\| y - z \| )
$$

for $(y, z)$ tending to $(x_0, x_0)$ in $E \times E$. For this, it is enough that this condition be satisfied for one norm defining the topology of E. Suppose moreover that E and F are normed; for every number $c > \| Df(x_0) \|$, there then exists a neighbourhood V of $x_0$ such that $\| f(y) - f(z) \| \leq c. \| y - z \|$ for $y, z$ in V; this implies that $f$ is uniformly continuous in V.

1.2.3. The fact that a function $f$ is differentiable or strictly differentiable at $x_0$ depends only on the germ of $f$ at $x_0$. The germs of functions differentiable at $x_0$ form a vector subspace $\mathcal{V}$ of the space of all germs, and the mapping $f \mapsto Df(x_0)$ of $\mathcal{V}$ into $\mathcal{L}(E; F)$ is linear. The germs of functions strictly differentiable at $x_0$ form a vector subspace of $\mathcal{V}$.

1.2.4. A function differentiable at $x_0$ is continuous at $x_0$.

1.2.5. When $E = K$, the mapping $u \mapsto u(1)$ is an isomorphism of $\mathcal{L}(E; F)$ onto $F$; if the function $f$ is differentiable at $x_0$, the element

$$
f'(x_0) = Df(x_0) \cdot 1
$$

is none other than the derivative of $f$ at $x_0$ in the sense given in Fonct. Var. Réelle, chap. I, § 1, n° 6, remark 2.

### 1.3. Composition of differentiable mappings

1.3.1. Suppose that F is normable. Let $x_0 \in E$ and $y_0 \in F$, U a neighbourhood of $x_0$ and V a neighbourhood of $y_0$; finally, let $f$ be a mapping of U into V, differentiable at $x_0$, with $f(x_0) = y_0$. If $g$ is a mapping of V into a separated polynormed vector space G, differentiable at $y_0$, the mapping $g \circ f$ of U into G is differentiable at $x_0$, and one has:

(1)
$$
D(g \circ f)(x_0) = Dg(y_0) \circ Df(x_0).
$$
If $f$ and $g$ are strictly differentiable, the same is true of $g \circ f$.

1.3.2. Let $f$ be a mapping defined in a neighbourhood of a point $x_0$ of E and with values in F, differentiable at $x_0$; if $u$ is a continuous linear mapping of F into a separated polynormed space G, the function $u \circ f$ is differentiable at $x_0$ and one has:

(2)
$$
D(u \circ f)(x_0) = u \circ Df(x_0).
$$

1.3.3. Suppose that F is the product of a family $(F_i)_{i \in I}$ of separated polynormed vector spaces; for each $i$ in I, let $f_i$ be a mapping defined in a neighbourhood U of a point $x_0$ of E and with values in F and let $f = (f_i)_{i \in I}$. For $f$ to be differentiable (resp. strictly differentiable) at $x_0$, it is necessary and sufficient that all the $f_i$ should be so; one has:

(3)
$$
D_h f(x_0) = (D_h f_i(x_0))_{i \in I} \quad \text{for every } h \text{ in } E.
$$

1.3.4. If $E = K$, one may replace $Df(x_0)$ by $f'(x_0)$ and $D_h f_i(x_0)$ by $f'_i(x_0)$ in formulas (1) and (3).

### 1.4. Product of differentiable mappings

1.4.1. Let $F_1, \ldots, F_m$ be separated polynormed spaces and $u$ a continuous $m$-linear mapping of $F_1 \times \cdots \times F_m$ into $F$. Let $U$ be a neighbourhood of a point $x_0$ of $E$, and let $f_i$ be a mapping of $U$ into $F_i$ (for $1 \leq i \leq m$). If the $f_i$ are differentiable (resp. strictly differentiable) at $x_0$, the same is true of $u(f_1, \ldots, f_m) = g$, and one has:

(4) $D_hg(x_0) = \sum_{j=1}^m u(f_1(x_0), \ldots, D_hf_j(x_0), \ldots, f_m(x_0))$ for $h$ in $E$,

which will be written more succinctly:

(5) $Dg = \sum_{j=1}^m u(f_1, \ldots, Df_j, \ldots, f_m)$.

In particular, for $m = 2$, one has:

(6) $Du(f_1, f_2) = u(Df_1, f_2) + u(f_1, Df_2)$.

For $m = 1$, this gives again 1.3.2.

1.4.2. When $E = K$, one may replace $Dg$ by $g'$ and $Df_j$ by $f'_j$ in formulas (4) to (6).

### 1.5. First variants of the implicit function theorem

Suppose that $E$ and $F$ are Banach spaces, and let $x_0$ be a point of $E$, $U$ a neighbourhood of $x_0$ and $f$ a mapping of $U$ into $F$. Suppose further that $f$ is strictly differentiable at $x_0$.

1.5.1. If $Df(x_0)$ is an isomorphism of $E$ onto $F$, there exists an open neighbourhood $U_0$ of $x_0$ contained in $U$ and an open neighbourhood $V_0$ of $f(x_0)$ such that $f|U_0$ is a homeomorphism of $U_0$ onto $V_0$. The mapping $g : V_0 \to U_0$ inverse to $f|U_0$ is strictly differentiable at the point $f(x_0)$, and one has:

$$
Dg(f(x_0)) = Df(x_0)^{-1}.
$$

1.5.2. If $Df(x_0)$ is a surjective mapping of $E$ onto $F$, there exists an open neighbourhood $U_0$ of $x_0$ contained in $U$, such that $f|U_0$ is an open mapping.

1.5.3. If $Df(x_0)$ is injective and has closed image, there exists a closed neighbourhood $U_0$ of $x_0$ contained in $U$, such that $f|U_0$ is a homeomorphism of $U_0$ onto a closed subset of $F$.

### 1.6. Partial derivatives

1.6.1. Let $f$ be a function defined in a neighbourhood $U$ of the point $x_0$ of $E$ and with values in $F$. Let $X$ be a vector space and $V$ the set of points $x$ of $X$ such that $x_0 + x \in U$; let us put $g(x) = f(x_0 + x)$ for $x \in V$. One says that $f$ admits a *partial derivative with respect to* $X$ *at* $x_0$ if $g$ admits a derivative at $0$; this derivative is denoted by $D_X f(x_0)$; it is a continuous linear mapping of $X$ into $F$. If $f$ is differentiable at $x_0$, it admits a partial derivative with respect to $X$ at $x_0$, and this partial derivative is the restriction of $Df(x_0)$ to $X$.

1.6.2. Suppose that $E$ is the product of a finite family of normed vector spaces $E_i$ ($1 \leq i \leq n$) canonically identified with subspaces of $E$; let $x_0 = (x_0^1, \ldots, x_0^n)$ in $E$ and let $U$ be a neighbourhood of $x_0$ in $E$; finally let $f$ be a mapping of $U$ into $F$. One denotes by $D_{i} f(x_0)$ the derivative at the point $x_0^i$, if it exists, of the mapping $z_i \mapsto f(x_0^1, \ldots, z_i, \ldots, x_0^n)$ defined in a neighbourhood of $x_0^i$ in $E_i$ and with values in $F$. It is an element of $\mathcal{L}(E_i; F)$ which is called the *$i$-th partial derivative of* $f$ *at* $x_0$. If $f$ is differentiable at $x_0$, the $n$ partial derivatives exist, and determine $Df(x_0)$ by the formula:

$$
Df(x_0) \cdot h = \sum_{i=1}^{n} D_{i} f(x_0) \cdot h_i \quad \text{for } h = (h_1, \ldots, h_n) \text{ in } E.
$$

1.6.3. More particularly, let $E = K^n$. If the partial derivatives of $f$ at $x_0$ exist, one denotes by $\partial_{i} f(x_0)$ the element $D_{i} f(x_0) \cdot 1$ of $F$. The following notation is often used; suppose that a notation has been chosen for the coordinate functions on $K^n$, for example $u_i$ denotes the $i$-th projection of $K^n$ onto $K$. One then writes:

$$
\frac{\partial f}{\partial u_i}(x_0) \quad \text{or} \quad \left. \frac{\partial f}{\partial u_i} \right|_{x = x_0}
$$

instead of $\partial_{i} f(x_0)$.

1.6.4. Let $E = K^n$ and $F = K^m$; suppose that the function $f = (f_1, \ldots, f_m)$ with values in $F$ is differentiable at the point $x_0$ of $E$. Then the partial derivatives $a_{ji} = \partial_{i} f_j(x_0)$ exist (they are elements of $K$). The matrix with $m$ rows and $n$ columns formed by the $a_{ji}$ (element of the row of index $j$ and of the column of index $i$) is called the *Jacobian matrix* of $f$ at $x_0$; it is the matrix of the linear mapping $Df(x_0)$ of $K^n$ into $K^m$ relative to the canonical bases of these spaces.

### 1.7. Iterated Derivatives

1.7.1. Let $f$ be a function defined in a neighbourhood of a point $x_0$ of $E$, with values in $F$. If $f$ is differentiable in a neighbourhood of $x_0$, its derivative $Df$ is a mapping of a neighbourhood of $x_0$ into the polynormed space $\mathcal{L}(E; F)$ of continuous linear mappings of $E$ into $F$. Let $p$ be an integer $\geq 2$:

one says that $f$ is $p$ times differentiable at $x_0$ if $f$ is differentiable in a neighbourhood of $x_0$ and if its derivative $Df$ is $(p - 1)$ times differentiable at $x_0$. One then defines the $p$-th derivative of $f$ at $x_0$: it is the continuous $p$-linear mapping $D^pf(x_0)$ of $E^p$ into $F$, defined by:

$$
D^pf(x_0) . (h_1, \ldots, h_p) = (D(D^{p-1}f)(x_0) . h_1) . (h_2, \ldots, h_p).
$$

We also set $D^0f = f$ and $D^1f = Df$. If $f$ is $p$ times differentiable at $x_0$ and if $q$ and $s$ are two integers such that $q + s = p$, with $s > 0$, then $f$ is $q$ times differentiable in a neighbourhood of $x_0$, the function $D^qf$ (with values in $\mathcal{L}_q(E; F)$) is $s$ times differentiable at $x_0$, and one has:

$$
D^{q+s}f(x_0) . (h_1, \ldots, h_{q+s}) = (D^s(D^qf)(x_0) . (h_1, \ldots, h_s)) . (h_{s+1}, \ldots, h_{q+s})
$$

a relation which, by abuse of notation, is written in the form:

$$
D^{q+s}f = D^s D^qf.
$$

1.7.2. Let $(E_i)_{1 \leq i \leq n}$ be closed vector subspaces of $E$, such that $E$ is the topological direct sum of the $E_i$. One then defines, when it exists, the iterated partial derivative $D_{i_1} \ldots D_{i_m}f$ of a mapping $f$ from a neighbourhood of $x_0 \in E$ into $F$; it is a continuous multilinear mapping from

$$
E_{i_1} \times \cdots \times E_{i_m}
$$

into $F$, defined by induction on the integer $m \geq 1$ as follows: if $D_{i_2} \ldots D_{i_m}f(x)$ exists in a neighbourhood of $x_0$ and has a partial derivative with respect to $E_{i_1}$, then $D_{i_1} \ldots D_{i_m}f(x_0)$ is given by:

$$
D_{i_1} \ldots D_{i_m}f(x_0) . (h_1, \ldots, h_m) = (D_{i_1}(D_{i_2} \ldots D_{i_m}f)(x_0) . h_1) . (h_2, \ldots, h_m)
$$

for $h_k \in E_{i_k}$.

If $f$ is $m$ times differentiable at $x_0$, then the partial derivative $D_{i_1} \ldots D_{i_m}f(x_0)$ exists and is equal to the restriction of $D^m f(x_0)$ to the subspace $E_{i_1} \times \cdots \times E_{i_m}$ of $E^m$. Consequently, $D^m f(x_0)$ is completely determined by the iterated partial derivatives of order $m$ at $x_0$.

1.7.3. Suppose that $E$ is finite-dimensional and let $(e_1, \ldots, e_n)$ be a basis of $E$. Put $E_i = K e_i$ and let $f$ be a mapping from a neighbourhood of $x_0$, with values in $F$. If the partial derivative $D_{i_1} \ldots D_{i_m}f(x_0)$ (with the notations of 1.7.2) exists, one puts:

$$
\partial_{i_1} \ldots \partial_{i_m} f(x_0) = D_{i_1} \ldots D_{i_m} f(x_0) . (e_{i_1}, \ldots, e_{i_m}).
$$
