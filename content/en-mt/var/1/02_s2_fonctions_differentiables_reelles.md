---
book: var
book_title: Variétés différentielles et analytiques
chapter: "1"
chapter_title: VARIÉTÉS DIFFÉRENTIELLES ET ANALYTIQUES, FASCICULE DE RÉSULTATS
section: 2
section_title: Fonctions différentiables réelles
lang: en
source: var-fr
pdf_pages: 0015-0019
extraction: ocr
subsections:
    - "no": 1
      title: Fonctions dérivables en un point
      page: 0
      pdf_page: 15
    - "no": 2
      title: Le théorème des accroissements finis
      page: 0
      pdf_page: 15
    - "no": 3
      title: Fonctions de classe $C^r$ ($r \neq \omega$)
      page: 0
      pdf_page: 16
    - "no": 4
      title: Dérivées des fonctions de classe $C^r$
      page: 0
      pdf_page: 17
    - "no": 5
      title: Formule de Taylor
      page: 0
      pdf_page: 17
    - "no": 6
      title: Critères de dérivabilité
      page: 0
      pdf_page: 19
statements: 0
exercises: 0
content_sha256: df93b3eccc63eeaac231d190cc93798443c258ceb9af58b543930f3e95d373a4
translated_from: content/fr/var/1/02_s2_fonctions_differentiables_reelles.md
source_lang: fr
translation_method: machine
source_content_sha256: 751c6249671612296169a2ada973673daef293ce7e4ae1a9d165e88250336f6c
translation_model: gpt-5-6-mini, gpt-5-6
translation_run: translate-en-mt-8d0ab83f
glossary_version: 34
glossary_terms_sha256: a96ecfb5c3040e4392b3447675a022ec3add3cce250d4836f15a276ef5e89a94
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 2. Real differentiable functions

In this paragraph, it is assumed that K = R. The letter E denotes a normed vector space over R; the letter F denotes a separated locally convex topological vector space over R.

### 2.1. Differentiable functions at a point

2.1.1. Let f be a function defined in a neighbourhood of a point x_0 of E and with values in F. Let u be an element of the space $\mathcal{L}(E; F)$ of continuous linear mappings from E into F. In order that f be differentiable at x_0 and admit u there as derivative, it is necessary and sufficient that one have
$$
\lim_{h \to 0, h \neq 0} \frac{f(x_0 + h) - f(x_0) - u(h)}{\|h\|} = 0.
$$

2.1.2. In order that f be strictly differentiable at x_0, it is necessary and sufficient that one have
$$
\lim_{(h, k) \to (0, 0), h \neq k} \frac{f(x_0 + h) - f(x_0 + k) - Df(x_0) \cdot (h - k)}{\|h - k\|} = 0.
$$

2.1.3. Let F_1 and F_2 be two separated locally convex spaces and let u be a bilinear mapping from F_1 × F_2 into F, satisfying the following continuity condition:
(SC) If ((a_n, b_n)) is a sequence of elements of F_1 × F_2 converging to an element (a, b) ∈ F_1 × F_2, then the sequence (u(a_n, b_n)) converges to u(a, b) in F.

Let f_i (for i = 1, 2) be a mapping from a neighbourhood of a point x_0 of E into F_i. If f_1 and f_2 are differentiable at x_0, then u(f_1, f_2) is differentiable at x_0 and one has:
$$
D(u(f_1, f_2))(x_0) \cdot h = u(Df_1(x_0) \cdot h, f_2(x_0)) + u(f_1(x_0), Df_2(x_0) \cdot h)
$$
for every $h \in E$.

### 2.2. The mean value theorem

2.2.1. Let x, y be in E, and let [x, y] be the closed segment joining these two points. Let moreover f be a mapping from a neighbourhood of [x, y] into the space F, differentiable at every point of [x, y]. Then f(x) − f(y) belongs to the closed convex envelope of the set of points Df(z) · (x − y) for z in [x, y].

2.2.2. Let U be an open connected set of E, and let f be a mapping from U into

F, admitting a zero derivative at every point of U; then $f$ is constant in U.

2.2.3. Let U be an open *convex* set of E, and let $f$ be a mapping from U into F, differentiable at every point of U. Given a continuous semi-norm $\gamma$ on F and a real number $M \geqslant 0$, the following conditions are equivalent:
    (i) For every $x$ in U, one has $\|Df(x)\|_{\gamma} \leqslant M$.
    (ii) For every $x$ and every $y$ in U, one has $\|f(x) - f(y)\|_{\gamma} \leqslant M \cdot \|x - y\|$.

2.2.4. Let U be a neighbourhood of a point $x_0$ of E and let $f$ be a function defined in the complement of $x_0$ in U, with values in F. Suppose that $f$ admits a derivative $Df(x)$ at every point $x$ of U, $x \neq x_0$, and that the function $x \mapsto Df(x)$ admits a limit $D_0$ when $x$ tends to $x_0$. Then, if $\dim(E) \geqslant 2$, $f$ has a limit at $x_0$ and the function $f$ extended by continuity to all of U is differentiable with derivative $D_0$ at $x_0$; the same holds if $\dim(E) = 1$ and it is assumed that $f$ has a limit at $x_0$.

### 2.3. Functions of class $C^r$ ($r \neq \omega$)

2.3.1. Let U be an open set of E and let $f$ be a mapping from U into F. We define the relation “$f$ is of class $C^r$” (for $r \in \mathbf{N}$) by induction on $r$ in the following manner:
    1) $f$ is of class $C^0$ if and only if it is continuous;
    2) if $r$ is an integer $\geqslant 1$, the function $f$ is of class $C^r$ if and only if it is differentiable at every point of U and if the derivative mapping $Df$ from U into $\mathcal{L}(E; F)$ is of class $C^{r-1}$.

Functions of class $C^r$ are also called *r times continuously differentiable functions*.

One says that $f$ is *of class $C^{\infty}$* (or *indefinitely differentiable*) if it is of class $C^r$ for every integer $r$.

If $f$ is of class $C^r$ in U, then $f$ is $p$ times differentiable for every integer $p \leqslant r$ and the function $D^p f$ is of class $C^{r-p}$.

2.3.2. The mappings of class $C^r$ from an open set U of E into F form a vector subspace $\mathcal{C}^r(U; F)$ of the space of all mappings from U into F. One has $\mathcal{C}^s(U; F) \subset \mathcal{C}^r(U; F)$ for $s \geqslant r$.

2.3.3. For a function $f$ to be of class $C^1$ in an open set U of E, it is necessary and sufficient that it be strictly differentiable at every point of U.

If E is a product of normed spaces $E_i$, a mapping $f$ from an open set V of E into F is of class $C^r$ if and only if $f$ possesses continuous iterated partial derivatives $D_{i_1} \ldots D_{i_m} f$ for every integer $m \leqslant r$.

2.3.4. Let G be a normed space and let U be an open set of E. Let V be an open set of G, $g \in \mathcal{C}^r(U; G)$ and $f \in \mathcal{C}^r(V; F)$. If $g(U) \subset V$, the mapping $f \circ g$ from U into F is of class $C^r$.

Let $F_1$ and $F_2$ be two separated locally convex spaces and let $u$ be a bilinear mapping from $F_1 \times F_2$ into F, hypocontinuous with respect to the set of bounded parts of $F_1$ (resp. $F_2$) (Esp. Vect. Top., ch. III, § 4, n° 2). Let U be an open set of E and $f_i \in \mathcal{C}^r(U; F_i)$ (for $i = 1, 2$). Then the function $u(f_1, f_2)$ belongs to $\mathcal{C}^r(U; F)$. If E is of finite dimension, it is sufficient to suppose that $u$ satisfies condition (SC) of n° 2.1.3.

2.3.5. If E is a product of normed spaces $E_i$ ($1 \leq i \leq n$) and if $f$ is a continuous $n$-linear mapping from E into F, then $f$ is of class $C^\infty$ and one has $D^p f = 0$ for $p \geq n + 1$.

2.3.6. Suppose that E and F are Banach spaces. Let $f$ be a function of class $C^r$ (with $r \geq 1$) defined in a neighbourhood of a point $x_0$ of E and with values in F. Let $y_0 = f(x_0)$ and suppose that $Df(x_0)$ is an isomorphism of E onto F. Then $f$ induces a homeomorphism $g$ of a neighbourhood of $x_0$ onto a neighbourhood of $y_0$ (1.5) and the inverse mapping of $g$ is of class $C^r$ in a neighbourhood of $y_0$.

### 2.4. Derivatives of functions of class $C^r$

2.4.1. Let $f$ be a mapping of class $C^r$ of an open U of E into F. For every $x \in U$, and every integer $s$ with $s \leq r$, the multilinear mapping $D^s f(x)$ is symmetric.

2.4.2. Suppose in addition that E is finite-dimensional and let $(e_1, \ldots, e_n)$ be a basis of E. The partial derivatives $\partial_{i_1} \ldots \partial_{i_s} f$ depend symmetrically on the indices $i_1, \ldots, i_s$. Let $\alpha_k$ be the number of times that the index $k$ occurs in the sequence $i_1, \ldots, i_s$ and let $\alpha = (\alpha_1, \ldots, \alpha_n)$. We then put:

$$
\partial^{\alpha} f = \partial_1^{\alpha_1} \ldots \partial_n^{\alpha_n} f = \partial_{i_1} \ldots \partial_{i_s} f
$$

When the coordinates relative to the basis $(e_1, \ldots, e_n)$ are denoted by $x_1, \ldots, x_n$, we also write $\partial^{\alpha} f$ in the form:

$$
\frac{\partial^{|\alpha|} f}{\partial x_1^{\alpha_1} \ldots \partial x_n^{\alpha_n}}
$$

### 2.5. Taylor formula

2.5.1. Let $r$ be an integer $\geq 1$ and let $f$ be a mapping of class $C^r$ of an open U of E into F. For $x \in U$, $h \in E$ and $p \leq r$, let us agree to write $D^p f(x_0) \cdot h^p$ in place of $D^p f(x_0) \cdot (h, \ldots, h)$. If the segment $[x, x + h]$ is contained in $U$, we have the formula (“Taylor formula”):

$$
f(x + h) = \sum_{p=0}^{r-1} \frac{1}{p!} D^p f(x) \cdot h^p + v_r(x; h)
$$

where the “remainder” $v_r(x; h)$ is given by:

$$
v_r(x; h) = \int_0^1 \frac{(1-t)^{r-1}}{(r-1)!} D^r f(x + th) \cdot h^r \, dt
$$

We have:

$$
v_r(x; h) \equiv \frac{1}{r!} D^r f(x) \cdot h^r \quad \text{mod } o(\|h\|^r) \quad \text{when } h \text{ tends to } 0
$$

and

$$
f(x + h) \equiv \sum_{p=0}^r \frac{1}{p!} D^p f(x) \cdot h^p \quad \text{mod } o(\|h\|^r)
$$

when $h$ tends to zero.

2.5.2. Suppose moreover that $\gamma$ is a continuous seminorm on $F$; if one has $\|D^r f(z)\|_\gamma \leq M$ for every point $z$ of the segment $[x, x + h]$, then one has:

$$
\|v_r(x; h)\|_\gamma \leq \frac{M}{r!} \|h\|^r
$$

2.5.3. Suppose in addition that $E = \mathbf{R}^n$. One then has:

$$
f(x + h) \equiv \sum_{|\alpha| \leq r} \Delta^\alpha f(x) h^\alpha \quad \text{mod } o(\|h\|^r) \quad \text{when } h \text{ tends to } 0
$$

putting:

$$
\Delta^\alpha f(x) = \frac{1}{\alpha!} \partial^\alpha f(x)
$$

2.5.4. Let $f$ and $g$ be two functions of class $C^r$ on an open subset $U$ of $E$, with values in $F$. In order that $f$ and $g$ have at a point $x$ of $U$ a contact of order $\geq r$, it is necessary and sufficient that one have $D^p f(x) = D^p g(x)$ for every integer $p$ with $0 \leq p \leq r$. When $E$ is finite-dimensional, this amounts to saying that the iterated partial derivatives of order $\leq r$ of $f$ and $g$ (with respect to a basis of $E$) are equal at the point $x$.

2.5.5. Let $U$ be an open subset of $E \times \mathbf{R}^n$ of the form $V \times I_1 \times \cdots \times I_n$, where $V$ is an open subset of $E$ and $I_1, \ldots, I_n$ are open intervals of $\mathbf{R}$ containing 0. Put $U_0 = V$ and $U_j = V \times I_1 \times \cdots \times I_j$ for $1 \leq j \leq n$. Given a function $f \in \mathcal{C}^r(U; F)$ (with $1 \leq r \leq \infty$), there exists one and only one sequence of functions $f_j \in \mathcal{C}^{r-1}(U_j; F)$ (for $0 \leq j \leq n$) such that:

$$
f(x, t_1, \ldots, t_n) = f_0(x) + \sum_{j=1}^n t_j f_j(x, t_1, \ldots, t_j)
$$

for $x \in V$ and $t_j \in I_j$. One has:

$$
f_0(x) = f(x, 0, \ldots, 0)
$$
$$
f_j(x, t_1, \ldots, t_j) = \int_0^1 \partial_j f(x, t_1, \ldots, t_{j-1}, t_j u, 0, \ldots, 0) du
$$

for $1 \leq j \leq n$. In this last formula, $\partial_j f$ denotes the $j$-th partial derivative of the function $(t_1, \ldots, t_n) \mapsto f(x, t_1, \ldots, t_n)$.

### 2.6. Criteria of differentiability

2.6.1. Suppose that $F$, in addition to its topology $\mathcal{T}$, is endowed with a less fine topology $\mathcal{T}'$, which also makes $F$ a separated locally convex space. Suppose moreover that $\mathcal{T}$ and $\mathcal{T}'$ satisfy the following condition:
(S) For every neighbourhood $V$ of 0 for the topology $\mathcal{T}$, there exists a neighbourhood $W$ of 0 for $\mathcal{T}$ such that the $\mathcal{T}'$-closed convex envelope of every $\mathcal{T}$-compact subset of $W$ is contained in $V$.

Let $f$ be a mapping from an open set $U$ of $E$ into $F$. Suppose that $f$ is of class $C^r$ ($1 \leq r \leq \infty$) when $F$ is endowed with the topology $\mathcal{T}'$, that $D^m f(x)$ is, for every $x$ of $U$, and every integer $m \leq r$, a continuous multilinear mapping of $E^m$ into $F$ endowed with the topology $\mathcal{T}$ and that the mapping $x \mapsto D^m f(x)$ is continuous from $U$ into $\mathcal{L}_m(E; F)$ ($F$ being endowed with the topology $\mathcal{T}$). Then $f$ is of class $C^r$ when $F$ is endowed with the topology $\mathcal{T}$ and its derivatives $D^m f$ are the same for $\mathcal{T}$ and for $\mathcal{T}'$.

Condition (S) is in particular realized if there exists a fundamental system of neighbourhoods of 0 for the topology $\mathcal{T}$ which are closed for the topology $\mathcal{T}'$: this is the case if the dual of $F$ endowed with $\mathcal{T}$ is identical with the dual of $F$ endowed with $\mathcal{T}'$. Condition (S) is also realized if $F$ endowed with the topology $\mathcal{T}$ is quasi-complete (*Esp. Vect. Top.*, Ch. III, § 2, No. 5).

2.6.2. Let $f$ be a mapping from an open set $U$ of $E$ into $F$. If $f$ is of class $C^r$ (with $0 \leq r \leq \infty$), the scalar functions $u \circ f$ are of class $C^r$ for every continuous linear form $u$ on $F$. Conversely if $F$ is quasi-complete and if the functions $u \circ f$ are of class $C^{r+1}$ for every $u \in F'$, then $f$ is of class $C^r$.
