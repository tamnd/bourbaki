---
book: var
book_title: Variétés différentielles et analytiques
chapter: "1"
chapter_title: VARIÉTÉS DIFFÉRENTIELLES ET ANALYTIQUES, FASCICULE DE RÉSULTATS
section: 3
section_title: Fonctions analytiques réelles ou complexes
lang: en
source: var-fr
pdf_pages: 0020-0028
extraction: ocr
subsections:
    - "no": 1
      title: Séries convergentes
      page: 0
      pdf_page: 20
    - "no": 2
      title: Fonctions analytiques
      page: 0
      pdf_page: 24
    - "no": 3
      title: Fonctions holomorphes
      page: 0
      pdf_page: 26
    - "no": 4
      title: Fonctions analytiques réelles
      page: 0
      pdf_page: 28
statements: 0
exercises: 0
content_sha256: f57b08ffe64096e3070f1e8db29f0883cd9e1d33972479170757b88e14b6846d
translated_from: content/fr/var/1/03_s3_fonctions_analytiques_reelles_ou.md
source_lang: fr
translation_method: machine
source_content_sha256: cfe146e6a40be8be1b051f760f4e1533856f7696cddc3e4c6f58c02e159289ef
translation_model: gpt-5.4
translation_run: translate-en-mt-d0cc7d91
glossary_version: 34
glossary_terms_sha256: 76a7b1046cbc8c4d1c2ad090ce8cf993a6fb209c7da811852175f95ffcd4672c
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 3. Real or Complex Analytic Functions

In this paragraph, it is assumed that $K = \mathbf{R}$ or $\mathbf{C}$. Let $(E_i),\ 1 \leq i \leq n$, be a finite family of normed spaces over $K$, let $E$ be the product space of the $E_i$, and let $F$ be a separated locally convex topological vector space over $K$.

### 3.1. Convergent series

3.1.1. Let $f = \sum f_\alpha$ be a formal series belonging to $\hat{P}(E_1, \ldots, E_n; F)$ (App., No. A.5). If $\gamma$ is a continuous seminorm on $F$ and $R = (R_1, \ldots, R_n)$ a sequence of $n$ strictly positive real numbers, we set:

$$
\|f\|_{\gamma, R} = \sum_\alpha R^\alpha \|f_\alpha\|_\gamma.
$$

If $F$ is a normed space and if $\gamma$ is the norm of $F$, we write $\|f\|_R$ instead of $\|f\|_{\gamma, R}$.

The set $\mathcal{H}_R(E_1, \ldots, E_n; F)$ of the $f \in \hat{P}(E_1, \ldots, E_n; F)$ such that $\|f\|_{\gamma, R}$ is finite for every continuous seminorm $\gamma$ on $F$ is a vector subspace of $\hat{P}(E_1, \ldots, E_n; F)$. We have

$$
\mathcal{H}_R(E_1, \ldots, E_n; F) \subset \mathcal{H}_{R'}(E_1, \ldots, E_n; F)
$$

whenever $R_i \geq R'_i$ for $1 \leq i \leq n$. The union of the

$$
\mathcal{H}_R(E_1, \ldots, E_n; F)
$$

is a vector subspace, denoted by $\mathcal{H}(E_1, \ldots, E_n; F)$, of $\hat{P}(E_1, \ldots, E_n; F)$, whose elements are called convergent series on the product of the $E_i$, with values in $F$. It depends only on the topology of the $E_i$ and not on their norms. One may therefore speak of the space $\mathcal{H}(E_1, \ldots, E_n; F)$ when the $E_i$ are normable spaces, without having to choose a norm on each $E_i$.

3.1.2. The mapping $f \mapsto \|f\|_{\gamma, R}$ is a seminorm on $\mathcal{H}_R(E_1, \ldots, E_n; F)$. The topology defined by these seminorms when $\gamma$ ranges over the set of continuous seminorms on $F$ (or simply a set of seminorms defining the topology of $F$) is separated. If $F$ is normable (resp. complete), the same is true of $\mathcal{H}_R(E_1, \ldots, E_n; F)$. The seminorms on $\mathcal{H}(E_1, \ldots, E_n; F)$ whose restriction to each $\mathcal{H}_R$ is continuous define a separated topology on $\mathcal{H}(E_1, \ldots, E_n; F)$, which depends only on the topologies of the $E_i$. The injection of $\mathcal{H}(E_1, \ldots, E_n; F)$ into $\hat{P}(E_1, \ldots, E_n; F)$ is continuous.

3.1.3. The canonical isomorphism of $\hat{P}(E; F)$ onto $\hat{P}(E_1, \ldots, E_n; F)$ yields by restriction an isomorphism of topological vector spaces of $\mathcal{H}(E; F)$ onto $\mathcal{H}(E_1, \ldots, E_n; F)$.

3.1.4. Let $f \in \mathcal{H}(E_1, \ldots, E_n; F)$ and let $J(f)$ be the set of $R \in (\mathbf{R}_+^*)^n$ such that $f \in \mathcal{H}_R(E_1, \ldots, E_n; F)$. The interior $I(f)$ of $J(f)$ is called the strict convergence indicatrix of $f$. It consists of the set of $R$ for which there exists an $R' \in J(f)$ with $0 < R_i < R'_i$ for $1 \leq i \leq n$. We denote by $\Omega(f)$ the set of points $(\log R_1, \ldots, \log R_n)$ of $\mathbf{R}^n$ for $R \in I(f)$: this is a convex subset of $\mathbf{R}^n$.

When $n = 1$, the set $I(f)$ is an interval $]0, \rho(f)[$ of $\mathbf{R}$, and $\rho(f)$ is called the strict radius of convergence of $f$. It is also the least upper bound (finite or $+\infty$) of the set of real numbers $R > 0$ such that for every continuous seminorm $\gamma$ on $F$, there exists a constant $M$ such that $\|f_m\|_{\gamma} \leq MR^{-m}$ (with $f = \sum f_m, f_m \in P_m(E; F)$) for every integer $m \geq 0$.

The set of points $x = (x_i) \in E_1 \times \cdots \times E_n$ such that there exists $R \in I(f)$ with $\|x_i\| \leq R_i$ for every $i$ is called the strict domain of convergence of $f$ and is denoted by $C(f)$. It is also the interior of the set of points $x$ for which there exists $R \in J(f)$ with $\|x_i\| < R_i$ for every $i$.

3.1.5. For $f_\alpha \in P_\alpha(E_1, \ldots, E_n; F)$ and for every continuous seminorm $\gamma$ on $F$, let us set:
$$
\|f_\alpha\|_{\gamma} = \sup_{\|x_i\| \leq 1} \|f_\alpha(x_1, \ldots, x_n)\|_{\gamma}.
$$
One then has the inequalities:
$$
\|f_\alpha\|_{\gamma} \leq \|f_\alpha\|_{\gamma'} \leq \frac{\alpha^\alpha}{\alpha!} \|f_\alpha\|_{\gamma}.
$$
For $f = \sum f_\alpha \in \hat{P}(E_1, \ldots, E_n; F)$ and $R \in (\mathbf{R}_+^*)^n$, let us set:
$$
\|f\|_{\gamma, R} = \sum_\alpha R^\alpha \|f_\alpha\|_{\gamma}
$$
and let $\tilde{\mathcal{H}}_R(E_1, \ldots, E_n; F)$ denote the vector subspace of $\hat{P}(E_1, \ldots, E_n; F)$
consisting of the $f$ such that $\|f\|_{\gamma, R}$ is finite for every $\gamma$, endowed with the topology defined by the seminorms $f \mapsto \|f\|_{\gamma, R}$. One has $\mathcal{H}_R \subset \tilde{\mathcal{H}}_R$ and the injection of $\mathcal{H}_R$ into $\tilde{\mathcal{H}}_R$ is continuous. The space $\mathcal{H}(E_1, \ldots, E_n; F)$ is the union of the $\tilde{\mathcal{H}}_R(E_1, \ldots, E_n; F)$ and its topology is the finest locally convex topology for which the injections of the $\mathcal{H}_R$ into $\mathcal{H}$ are continuous.

If $f \in \mathcal{H}(E_1, \ldots, E_n; F)$, the **indicator of convergence** is defined to be the interior $\tilde{I}(f)$ of the set $\tilde{J}(f)$ of the $R \in (\mathbf{R}_+^*)$ such that $f \in \tilde{\mathcal{H}}_R$. One has:
$$
e^{-1}\tilde{I}(f) \subset I(f) \subset \tilde{I}(f)
$$
(where $e$ is the base of the Naperian logarithms). From $\tilde{I}(f)$ one defines, as in 3.1.4., the domain of convergence $\tilde{C}(f)$ and, when $n = 1$, the radius of convergence $\tilde{\rho}(f)$. In particular, one has:
$$
e^{-1}\tilde{\rho}(f) \leq \rho(f) \leq \tilde{\rho}(f).
$$

3.1.6. For $R \in (\mathbf{R}_+^*)^n$, the (closed) polyball of center 0 and radius $R$ in $E$ is the set $B(R)$ of the $x \in E$ such that $\|x_i\| \leq R_i$ for every $i$. If $\dim E_i = 1$, one also says polydisc. If $f \in \mathcal{H}(E_1, \ldots, E_n; F)$, the domain of convergence (resp. strict domain of convergence) of $f$ is the union of the polyballs $B(R)$ for $R \in \tilde{I}(f)$ (resp. $R \in I(f)$).

3.1.7. Let $f \in \mathcal{H}(E_1, \ldots, E_n; F)$. Suppose that $F$ is quasi-complete. For every $x \in \tilde{C}(f)$, the family of the $f_a(x)$ is summable in $F$. Its sum, denoted by $\hat{f}(x)$ or simply $f(x)$, is a continuous function on $\tilde{C}(f)$. More precisely, for every $R$ such that $f \in \tilde{\mathcal{H}}_R$, the family of the $f_a(x)$ is uniformly summable for $x \in B(R)$. The mapping $f \mapsto \hat{f}$ is an injective continuous linear mapping of $\tilde{\mathcal{H}}_R$ into the space of bounded continuous functions on $B(R)$, endowed with the topology of uniform convergence.

3.1.8. Let $F_1, \ldots, F_m$ be separated polynormed spaces and let $u$ be a continuous $m$-linear mapping of $F_1 \times \cdots \times F_m$ into $F$. Let $f_i \in \mathcal{H}(E_1, \ldots, E_n; F_i)$ for $1 \leq i \leq m$. The formal series $u(f_1, \ldots, f_m)$ belongs to $\mathcal{H}(E_1, \ldots, E_n; F)$. We have:

$$
C(u(f_1, \ldots, f_m)) \supset \bigcap_i C(f_i)
$$
$$
\tilde{C}(u(f_1, \ldots, f_m)) \supset \bigcap_i \tilde{C}(f_i)
$$

and if $x \in \bigcap_i \tilde{C}(f_i)$, $F$ and the $F_i$ being quasi-complete, we have:
$$
u(f_1, \ldots, f_m)(x) = u(f_1(x), \ldots, f_m(x)).
$$

3.1.9. Let $F_1, \ldots, F_m$ be complete normed spaces and suppose that $F$ is quasi-complete. Let $f = (f_i)_{1 \leq i \leq m}$ with $f_i \in \mathcal{H}(E_1, \ldots, E_n; F_i)$ and $g \in \mathcal{H}(F_1, \ldots, F_m; F)$, such that $(f_i(0))_{1 \leq i \leq m}$ belongs to the strict domain of convergence of $g$. Then, for every $\alpha \in \mathbf{N}^m$, the formal series $g_\alpha \circ f$ belongs to $\mathcal{H}(E_1, \ldots, E_n; F)$ and the family of the $g_\alpha \circ f$ is summable in $\mathcal{H}(E_1, \ldots, E_n; F)$ and fortiori in $\hat{P}(E_1, \ldots, E_n; F)$. Its sum will be denoted by $g \circ f$.

More precisely, there exist $R \in \bigcap_i I(f_i)$ and $R' \in I(g)$ such that $\|f_i\|_R < R'_i$ for $1 \leq i \leq m$. Under these conditions, the formal series $g_\alpha \circ f$ belongs to $\mathcal{H}_R(E_1, \ldots, E_n; F)$, and the family of the $g_\alpha \circ f$ is summable in $\mathcal{H}_R(E_1, \ldots, E_n; F)$. Finally, if $x \in B(R)$, then $f(x) = (f_i(x))$ belongs to $B(R') \subset F_1 \times \cdots \times F_m$ and we have:
$$
g(f(x)) = (g \circ f)(x).
$$

3.1.10. Suppose that $E_i = K$ for $1 \leq i \leq n$. The space $\hat{P}(K^n; F)$ is then identified with the space of formal series in $n$ indeterminates $X_1, \ldots, X_n$ with coefficients in $F$, and an element of $\hat{P}(K^n; F)$ is written:

$$
f = \sum_{\alpha} X^\alpha c_\alpha \quad \text{with } c_\alpha \in F.
$$

If $R \in (\mathbf{R}_+^*)^n$ and if $\gamma$ is a continuous seminorm on $F$, one has:

$$
\| f \|_{\gamma, R} = \| f \|_{\gamma, R} = \sum_{\alpha} R^\alpha \| c_\alpha \|_\gamma
$$

One has $I(f) = \tilde{I}(f)$, $C(f) = \tilde{C}(f)$ and, when $n = 1$, $\rho(f) = \tilde{\rho}(f)$.

The space $\mathcal{H}(K^n; K)$ of convergent series with coefficients in $K$ is also denoted by $K\{(X_1, \ldots, X_n)\}$; it is a subalgebra of $K[[X_1, \ldots, X_n]]$. The space $\mathcal{H}(K^n; F)$ is a module over $K\{(X_1, \ldots, X_n)\}$ and if $F$ is finite-dimensional, this module is identified with $K\{(X_1, \ldots, X_n)\} \otimes_K F$.

3.1.11. Let $f \in \mathcal{H}(K^n; K^m)$, represented by a system of $m$ convergent series $f_j(X_1, \ldots, X_n)$, with coefficients in $K$. Let analogously $g \in \mathcal{H}(K^m; K^p)$, represented by a system of $p$ convergent series $g_k(Y_1, \ldots, Y_m) = \sum g_{k,\beta} Y^\beta$. The element $h = g \circ f$ of $\mathcal{H}(K^n; K^p)$ (cf. 3.1.9) is represented by $p$ formal series $h_k(X_1, \ldots, X_n)$, determined as follows: for $\alpha \in \mathbf{N}^n$ and $\beta \in \mathbf{N}^m$, let $c_{\alpha,\beta}$ be the coefficient of $X^\alpha$ in the formal series $f^\beta = \prod f_j^{\beta_j}$; then the family $(g_{k,\beta} c_{\alpha,\beta})_{\beta \in \mathbf{N}^m}$ is summable in $K$ and has as sum the coefficient of $X^\alpha$ in $h_k$.

3.1.12. Suppose $F$ quasi-complete and let $\hat{E}_i$ be the completion of $E_i$. Every continuous polynomial on $E_1 \times \cdots \times E_n$ with values in $F$ extends by continuity to a continuous polynomial on $\hat{E}_1 \times \cdots \times \hat{E}_n$, with values in $F$. One deduces from this a bijection $j$ of $\hat{P}(E_1, \ldots, E_n; F)$ onto $\hat{P}(\hat{E}_1, \ldots, \hat{E}_n; F)$. If $f \in \mathcal{H}(E_1, \ldots, E_n; F)$, then $j(f) \in \mathcal{H}(\hat{E}_1, \ldots, \hat{E}_n; F)$ and conversely. The strict convergence indicators of $f$ and of $j(f)$ are the same.

3.1.13. Suppose that $K = \mathbf{R}$, but that $F$ is endowed with a structure of complex vector space compatible with its structure of real vector space. Let $E_i^C = E_i \otimes_\mathbf{R} \mathbf{C}$. If $y \in E_i^C$, put

$$
y = \inf \sum_k |a_k| \cdot \| x_k \|,
$$

the greatest lower bound being taken over all finite families of pairs $(x_k, a_k) \in E_i \times \mathbf{C}$ such that $y = \sum_k x_k \otimes a_k$. In this way one obtains a norm on the complex vector space $E_i^C$; this norm extends the given norm on $E_i$ if one agrees to identify $x \in E_i$ with $x \otimes 1$. Let $h$ be an $\mathbf{R}$-polynomial-continuous mapping on $E_1 \times \cdots \times E_n$, with values in $F$, and homogeneous of multidegree $\alpha$; then there exists one and only one $\mathbf{C}$-polynomial-continuous mapping $\tilde{h}$ on $E_1^C \times \cdots \times E_n^C$, with values in $F$, extending $h$, and homogeneous of multidegree $\alpha$. One has

$$
\| \tilde{h} \|_\gamma = \| h \|_\gamma
$$

for every continuous seminorm $\gamma$ on the complex vector space $F$.

If $f = \sum_{\alpha} f_{\alpha} \in \mathcal{H}(E_1, \ldots, E_n; F)$, then $\tilde{f} = \sum_{\alpha} \tilde{f}_{\alpha} \in \mathcal{H}(E_1^c, \ldots, E_n^c; F)$. The series $f$ and $\tilde{f}$ have the same strict convergence indicatrix (and the same strict radius of convergence when $n = 1$).

Conversely, suppose $K = C$. Let $E_i^0$ and $F^0$ be the spaces over $\mathbf{R}$ obtained by restriction of scalars. If $f_{\alpha} \in P_{\alpha}(E_1, \ldots, E_n; F)$, then $f_{\alpha} \in P_{\alpha}(E_1^0, \ldots, E_n^0; F^0)$. If $f = \sum_{\alpha} f_{\alpha} \in \mathcal{H}(E_1, \ldots, E_n; F)$, then the formal series $f^0 = \sum_{\alpha} f_{\alpha} \in \hat{P}(E_1^0, \ldots, E_n^0; F^0)$ is a convergent series. The convergence indicatrices (resp. the strict convergence indicatrices) of $f$ and $f^0$ are identical and one has $f(x) = f^0(x)$ for every $x \in \bar{C}(f) = \bar{C}(f^0)$.

### 3.2. Analytic functions

3.2.1. Let $U$ be an open set of $E$ and $f$ a mapping of $U$ into $F$. One says that $f$ is *of class* $C^{\omega}$, or *K-analytic* (or simply *analytic*) in $U$ if, for every point $a$ of $U$, there exists a convergent series $f_{\alpha} \in \mathcal{H}(E; F)$ such that $f(a + x) = f_{\alpha}(x)$ for all $x$ in $E$ sufficiently near zero. If $K = \mathbf{R}$ (resp. $\mathbf{C}$), one also says that $f$ is *real analytic* (resp. *complex analytic* or *holomorphic*). The analytic mappings of $U$ into $F$ form a vector subspace, denoted by $\mathcal{C}^{\omega}(U; F)$, of the space of all mappings of $U$ into $F$.

For $a \in U$, the formal series $f_{\alpha}$ is unique: it is called the *power series expansion* of $f$ at the point $a$. If $f_{\alpha} = \sum_{\alpha} (f_{\alpha})_{\alpha}$ (with $(f_{\alpha})_{\alpha} \in P_{\alpha}(E_1, \ldots, E_n; F)$), one puts:

$$
\Delta^{\alpha} f(a) = (f_{\alpha})_{\alpha}.
$$

3.2.2. If $f \in \mathcal{C}^{\omega}(U; F)$, the map $\Delta^{\alpha} f : a \mapsto \Delta^{\alpha} f(a)$ of $U$ into

$$
P_{\alpha}(E_1, \ldots, E_n; F)
$$

is analytic. The map $\Delta^{\alpha} : f \mapsto \Delta^{\alpha} f$ is a $K$-linear map of $\mathcal{C}^{\omega}(U; F)$ into $\mathcal{C}^{\omega}(U; P_{\alpha}(E_1, \ldots, E_n; F))$. For $a \in U$, one has therefore, for $\alpha, \beta \in \mathbf{N}^n$, $\Delta^{\beta}(\Delta^{\alpha} f)(a) \in P_{\beta}(E_1, \ldots, E_n; P_{\alpha}(E_1, \ldots, E_n; F))$. If $x = (x_i) \in E$, one has therefore $(\Delta^{\beta}(\Delta^{\alpha} f)(a))(x) \in P_{\alpha}(E_1, \ldots, E_n; F)$ and $((\Delta^{\beta}(\Delta^{\alpha} f)(a))(x))(x) \in F$. This element of $F$ is equal to $((\alpha, \beta))(\Delta^{\alpha+\beta} f(a))(x)$. This is expressed by writing:

$$
\Delta^{\beta} \circ \Delta^{\alpha} = ((\alpha, \beta)) \Delta^{\alpha+\beta}.
$$

3.2.3. The strict convergence indicators (and the strict radii of convergence when $n = 1$) of the power series expansions of $f$ and of $\Delta^{\alpha} f$ at the same point $a$ of $U$ are identical.

3.2.4. Let $f \in \mathcal{C}^\omega(U; F)$. Then $f$ is strictly differentiable and indefinitely differentiable in $U$ (if $K = \mathbf{R}$, $f$ is of class $C^\infty$ in $U$). The iterated derivatives of $f$ are analytic, and their values at a point $a$ are symmetric multilinear mappings. One may then introduce the notation $D^\alpha f$ for the iterated partial derivatives as in No. 2.4.2. We have:

$$
\alpha! \Delta^\alpha f(a)(h) = D^\alpha f(a) . (h, \ldots, h)
$$

for all $a \in U$ and $h \in E$, which is written:

$$
\alpha! \Delta^\alpha f = D^\alpha f .
$$

3.2.5. Let $U$ be an open subset of $E$ and let $f, g$ be two analytic mappings of $U$ into $F$. Let $a \in U$. In order that $f$ and $g$ should have contact of order $\geq k$ at $a$, it is necessary and sufficient that $\Delta^\alpha f(a) = \Delta^\alpha g(a)$ for every $\alpha$ with $|\alpha| \leq k$. If $f$ and $g$ have contact of infinite order at $a$, they are equal in a neighbourhood of $a$. The set of points of $U$ at which $f$ and $g$ have contact of infinite order is open and closed.

In particular, if $U$ is connected and if there exists a nonempty open subset of $U$ on which $f$ and $g$ are equal, then $f = g$ ("principle of analytic continuation").

3.2.6. Let $U$ be an open subset of $E$ and let $f$ be an analytic mapping of $U$ into $F$. If the derivative $Df$ of $f$ is zero, $f$ is locally constant.

3.2.7. Suppose $F$ quasi-complete and let $G$ be a complete normed space. Let $g$ be an analytic mapping of an open set $U$ of $E$ into $G$ and let $f$ be an analytic mapping of an open set $V$ of $G$, containing $g(U)$, into $F$. The composite mapping $f \circ g$ is analytic in $U$. Suppose moreover that $0 \in U$ and that $g(0) = 0$. The expansion of $f \circ g$ into a power series at $0$ is then obtained by substituting, in the expansion of $f$ at $0$, the power series expansion of $g$ at $0$ (3.1.9).

3.2.8. Let $F_1, \ldots, F_m$ be separated polynormed spaces and $u$ a continuous multilinear mapping of $F_1 \times \cdots \times F_m$ into $F$. Let $U$ be an open set of $E$ and $f_i \in \mathcal{C}^\omega(U; F_i)$. The function $u(f_1, \ldots, f_m)$ is analytic, and its expansion into a power series at a point $a \in U$ is the series $u((f_1)_a, \ldots, (f_m)_a)$ (3.1.8).

3.2.9. Assume $F$ quasi-complete. Let $f \in \mathcal{H}(E_1, \ldots, E_n; F)$; the function $x \mapsto f(x)$ (3.1.7) is analytic in the open set $C(f)$, the domain of strict convergence of $f$. If $n = 1$ and if $\|a\| < \rho(f)$, the radius of strict convergence of the expansion of $f$ into a power series at $a$ is at least equal to $\rho(f) - \|a\|$. If $\rho(f) = + \infty$, one says that $f$ is an entire function.

3.2.10. Retain the hypotheses of 3.2.9. If $K = \mathbf{C}$, the results of 3.2.9 remain valid if one replaces $C(f)$ by $\tilde{C}(f)$ and $\rho(f)$ by $\tilde{\rho}(f)$ (for $n = 1$). If $K = \mathbf{R}$, the function $x \mapsto f(x)$ is analytic in $\tilde{C}(f)$.

3.2.11. Suppose that $E_i = K$ for $1 \leq i \leq n$. Let $U$ be an open set of $K^n$ and let $f \in \mathcal{C}^\omega(K^n; F)$. If $0 \in U$ and if $f_0 = \sum_\alpha X^\alpha c_\alpha$ is the power series expansion of $f$ at $0$, the power series expansion of $\Delta^\alpha f$ at $0$ is written (after identification of $P_\alpha(K^n; F)$ with $F$):

$$
(\Delta^\alpha f)_0 = \sum_\beta ((\alpha, \beta)) X^\beta c_{\alpha + \beta}.
$$

In particular, for $1 \leq i \leq n$ and for $x \in C(f_0)$, one has:

$$
\partial_i f(x) = \sum_\alpha (\alpha_i + 1) x^\alpha c_{\alpha + e_i}.
$$

### 3.3 Holomorphic Functions

In this No., it is supposed that $K = \mathbf{C}$.

3.3.1. Suppose $F$ quasi-complete. Let $U$ be an open set of $E$ and let $f$ be a mapping of $U$ into $F$. The following conditions are equivalent:
(i) $f$ is holomorphic;
(ii) $f$ is differentiable;
(iii) $f$ is locally bounded and, whatever $a \in U$ and $h \in E$ may be, the function $t \mapsto f(a + th)$, defined in an open neighbourhood of $0$ in $C$, is holomorphic;
(iv) $f$ is locally bounded and for every continuous linear form $u$ on $F$, the $\mathbf{C}$-valued function $u \circ f$ is holomorphic;
(v) $f$ is continuous and locally bounded and there exists a total set $H$ of the dual of $F$ such that $u \circ f$ is holomorphic for every $u \in H$.

When $E$ is finite-dimensional (resp. when $F$ is a Banach space), these conditions are still equivalent to conditions (iii'), (iv') or (v') (resp. (iv') or (v')) obtained from (iii), (iv) or (v) (resp. (iv) or (v)) by omitting the assumption "$f$ is locally bounded".

3.3.2. Suppose $F$ quasi-complete. Let $U$ be an open set of $E$ and $(f_n)$ a sequence of holomorphic mappings of $U$ into $F$, having the following property:
(W) Every point of $U$ possesses a neighbourhood in which the sequence $(f_n)$ converges uniformly.
Then the limit $f$ of the sequence $(f_n)$ is holomorphic, the sequence of derivatives $(Df_n)$ (with values in the quasi-complete space $\mathcal{L}(E; F)$) possesses property (W), and $Df$ is the limit of $(Df_n)$.

3.3.3. Let U be an open set of E and f a holomorphic mapping of U into F, assumed quasi-complete. Let $R = (R_i) \in (\mathbf{R}_+^*)^n$ and suppose that the polyball B(R) is contained in U and that f is bounded on B(R). Then, for every $α \in \mathbf{N}^n$ and every $x = (x_i) \in B(R)$:

$$
Δ^αf(0)(x) = \int_0^1 \cdots \int_0^1 f(e(\theta_1)x_1, \ldots, e(\theta_n)x_n)e(-α_1θ_1 - \cdots - α_nθ_n)\ dθ_1 \ldots dθ_n
$$

(where $e(θ) = \exp 2πi θ$).

Let moreover $γ$ be a continuous semi-norm on F and let M be the upper bound of $\|f(x)\|_γ$ for $\|x_i\| = R_i$. Then $\|Δ^αf(0)(x)\|_γ \leq M$ for every $x \in B(R)$ and $\|Δ^αf(0)\|_γ \leq MR^{-α}$. Finally, the domain of convergence of the series expansion of f at 0 contains the interior of the polyball B(R).

3.3.4. Let us retain the hypotheses of 3.3.3 and suppose moreover that $E_i = \mathbf{C}$. Let $\sum_{α} X^αc_α$ be the series expansion of f at 0. We have:

$$
c_α = R^{-α}\int_0^1 \cdots \int_0^1 f(e(\theta_1)R_1, \ldots, e(\theta_n)R_n)e(-α_1θ_1 - \cdots - α_nθ_n)\ dθ_1 \ldots dθ_n
$$

and:

$$
\|c_α\|_γ \leq R^{-α} \sup_{x \in B(R)} \|f(x)\|_γ
$$

(“Cauchy inequalities”). The strict domain of convergence of the series $\sum_{α} X^αc_α$ contains the interior of B(R).

3.3.5. Suppose E finite-dimensional and F quasi-complete. Let f be a holomorphic mapping of E into F. Then there exists in $\mathscr{H}(E; F)$ one and only one series $f_0$, of infinite radius of convergence (for every norm on E), such that $f(x) = f_0(x)$ for every $x \in E$.

3.3.6. If f is a holomorphic mapping of E into F such that $f(E)$ is bounded, then the function f is constant (“Liouville's theorem”).

3.3.7. We suppose that $E \neq 0$. Let f be a holomorphic mapping of an open set U of E into F. Let a be a point of U and $γ$ a continuous semi-norm on F. For every neighbourhood V of a, contained in U, there exists $x \in V, x \neq a$, such that:

$$
\|f(a)\|_γ \leq \|f(x)\|_γ.
$$

If moreover $F = \mathbf{C}$ and if f is not constant in a neighbourhood of a, we have $|f(a)| < \sup_{x \in V, x \neq a} |f(x)|$ and the mapping f is open in a neighbourhood of a.

Finally, let B be a bounded open set whose closure is contained in U and let B' be its boundary. We have:

$$
\sup_{x \in \overline{B}} |f(x)| = \sup_{x \in B'} |f(x)|
$$

(“maximum principle”).

3.3.8. Suppose E finite-dimensional. Let U be an open set of E, S a vector subspace of codimension $\geq 2$ of E and $f$ a holomorphic mapping of $U \cap (E - S)$ into F. Then $f$ extends by continuity to a holomorphic mapping of U into F.

3.3.9. Suppose that $E = \mathbf{C}$ and let $0 \leq \lambda < \mu \leq +\infty$. Let $f$ be a holomorphic mapping of the open set $U = \{ z \in \mathbf{C} | \lambda < |z| < \mu \}$ into F. There exists one and only one family $(a_n(f))_{n \in \mathbf{Z}}$ of elements of F such that, for every compact set H of U, the family $(a_n(f)z^n)_{n \in \mathbf{Z}}$ is uniformly summable with sum $f(z)$ for $z$ ranging over H (“Laurent expansion”).

Suppose moreover that $\lambda = 0$. The order of $f$ at the point $x = 0$ is defined to be the greatest lower bound (finite or infinite) of the set of integers $n$ such that $a_n(f) \neq 0$. If there exists a neighbourhood V of 0 such that $f$ is bounded in $V - \{0\}$, then $f$ is of order 0 at the point $x = 0$ and extends by continuity to a holomorphic function on the open set $|z| < \mu$. Let $p$ be an integer $> 0$; if $f$ is of order $-p$ at the point $x = 0$, one says that 0 is a pole of order $p$ of $f$.

3.3.10. Suppose that $E = \mathbf{C}$ and that F is normed. Let $f$ be a holomorphic mapping of the open unit disk U of E into F, such that $f(0) = 0$ and let $M = \sup_{z \in U} \|f(z)\|$. Then $\|f(z)\| \leq M \cdot |z|$ for all $z \in U$ ("Schwarz's lemma").

### 3.4. Real analytic functions

Suppose that $K = \mathbf{R}$.

3.4.1. Let U be an open set of E and $f$ a mapping of U into F, supposed quasi-complete.

The following conditions are equivalent:
(i) $f$ is analytic.
(ii) $f$ is of class $C^\infty$ and, for every $a \in U$, there exist a neighbourhood $V_a$ of $a$ and a real number $M$ such that, for every continuous semi-norm $\gamma$ on F, there exists a constant $A_\gamma$ such that one has
$$
\|\Delta^\alpha f(x)\|_\gamma \leq A_\gamma M^{|\alpha|} \quad \text{for all } x \in V_a \text{ and all } \alpha \in \mathbf{N}^n.
$$

3.4.2. Let U be an open set of E and $f$ a mapping of U into F. If F is quasi-complete, and if its strong dual $F'$ is a Baire space, then $f$ is analytic if and only if $u \circ f$ is analytic for all $u \in F'$.
