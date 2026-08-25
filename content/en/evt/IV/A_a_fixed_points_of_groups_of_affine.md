---
book: evt
book_title: Topological Vector Spaces
chapter: IV
chapter_title: DUALITY IN TOPOLOGICAL VECTOR SPACES
section: 0
section_title: Fixed points of groups of affine transformations
appendix: true
lang: en
source: evt-i-v
pdf_pages: 0221-0229, 0254-0258
extraction: ocr
subsections:
    - "no": 1
      title: The case of solvable groups
      page: 0
      pdf_page: 221
    - "no": 2
      title: Invariant means
      page: 40
      pdf_page: 222
    - "no": 3
      title: Ryll-Nardzewski theorem
      page: 41
      pdf_page: 223
    - "no": 4
      title: Applications.
      page: 44
      pdf_page: 226
statements: 10
exercises: 8
content_sha256: e69ea53271bb8075f8d762c7e9c446bf7e5efa0e0729c716a20cb05bccd07396
---

## APPENDIX
# Fixed points of groups of affine transformations

### 1. The case of solvable groups

Let E be a real vector space, and K a convex subset of E. A mapping $u : K \to K$ such that for $x, y$ in K and for every real number $t$ in $[0, 1]$, we have

$$
u(t x + (1 - t) y) = t u(x) + (1 - t) u(y)
$$

is said to be an affine transformation. From relation (1) we deduce that

$$
u \left( \sum_{i \in I} t_i x_i \right) = \sum_{i \in I} t_i u(x_i)
$$

for every finite set I, points $x_i$ in K and positive real numbers $t_i$ such that $\sum_{i \in I} t_i = 1$.

Let $u$ and $v$ be two affine transformations on K, then the mapping $u \circ v$ is an affine transformation on K. If $v : E \to E$ is a linear mapping such that $v(K) \subset K$, the mapping $u : K \to K$ which coincides with $v$ on K is an affine transformation.

#### Theorem 1 (Markoff-Kakutani) {#evt-iv-a0-thm-1 .statement}

— *Let E be a Hausdorff locally convex vector space over the field $\mathbf{R}$, and K a non-empty compact convex subset of E. Let $\Gamma$ be a set of continuous affine transformations on K, pairwise permutable. Then there exists a point a in K such that $u(a) = a$ for all $u \in \Gamma$.*

For every $u \in \Gamma$, let $K_u$ be the set of all $x \in K$ such that $u(x) = x$. We shall show that $K_u$ is non-empty. Let $x$ be a point of K; for every integer $n \geq 1$, let $x_n$ be the element $\frac{1}{n} \sum_{i=0}^{n-1} u^i(x)$ of E. Since K is convex and stable under $u$, the points $x_n$ belong to K and since K is compact, there exists a limit point $a$ of the sequence $(x_n)_{n \geq 1}$. The mapping $y \mapsto u(y) - y$ from K into E is continuous, hence $u(a) - a$ is a limit point of the sequence $(u(x_n) - x_n)_{n \geq 1}$. But we have $u(x_n) - x_n = \frac{1}{n} (u^n(x) - x)$.

Since K is compact, hence also bounded (III, p. 3, prop. 2), the sequence $(u^n(x) - x)_{n \geq 1}$ is bounded; consequently, the sequence $\left( \frac{1}{n}(u^n(x) - x) \right)_{n \geq 1}$ tends to 0 (III, p. 4, prop. 3), and since E is Hausdorff, we have $u(a) - a = 0$. Therefore $a \in K_u$.

Each of the sets $K_u$ is a closed and convex subset of the compact space K, and we shall prove that the intersection $\bigcap_{u \in \Gamma} K_u$ is non-empty. For this it is enough to prove that, for $n \geq 1$, and $u_1, ..., u_n$ in $\Gamma$, the set $K_{u_1} \cap ... \cap K_{u_n}$ is non-empty. The case $n = 1$ having been considered, we argue by induction on $n$. Suppose $n \geq 2$ and put $L = K_{u_1} \cap ... \cap K_{u_{n-1}}$. By the hypothesis of induction, L is a non-empty compact convex subset of E. Since $u_n$ commutes with $u_1, ..., u_{n-1}$, we have $u_n(L) \subset L$. Applying the first part of the proof to the affine transformation induced by $u_n$ on L, we conclude that there exists a point $a$ in L such that $u_n(a) = a$; then $a$ belongs to $K_{u_1} \cap ... \cap K_{u_n}$, which is then non-empty.

#### Corollary {#evt-iv-a0-n1-cor-1 .statement}

— *Let G be a solvable group of continuous affine transformations on K. Then there exists a point in K which is invariant under G.*

By the definition of a solvable group (A, I, § 6, No. 4) there exists a finite decreasing sequence $(G_i)_{0 \leq i \leq n}$ of distinct subgroups of G, such that $G_0 = G$, $G_n = \{e\}$ and such that the group $G_{i-1}/G_i$ is *commutative* for $1 \leq i \leq n$. Let $K_i$ denote the set of fixed points of $G_i$ in K. Then $K_n = K$. Moreover, for $1 \leq i \leq n$, every element of $G_i$ induces the identity transformation on $K_i$; we thus deduce an action of the abelian group $G_{i-1}/G_i$ on K if $K_i$ is non-empty; it follows from th. 1 that the set $K_{i-1}$ of fixed points of $G_{i-1}/G_i$ in $K_i$ is non-empty. By descending induction on $i$, we conclude that $K_0$ is non-empty, hence the corollary.

### 2. Invariant means

Let X be a topological space. Let $\mathcal{B}(X; \mathbf{R})$ denote the real vector space consisting of continuous bounded mappings from X into $\mathbf{R}$. Endowed with the norm $\|f\| = \sup_{x \in X} |f(x)|$, this is a Banach space (GT, X, § 3, No. 1); it is also an ordered vector space, where the relation $f \geq g$ means «$f(x) \geq g(x)$ for all $x \in X$».

#### Definition 1 {#evt-iv-a0-def-1 .statement}

*A positive linear form $\mu$ on the space $\mathcal{B}(X; \mathbf{R})$, where X is a topological space, for which $\|\mu\| = 1$, is called a mean on X.*

\* When X is compact, a mean on X is a positive measure on X such that $\mu(X) = 1$. \*

#### Lemma 1 {#evt-iv-a0-lem-1 .statement}

*The set K of means on X is the subset of the unit ball of the dual of the Banach space $E = \mathcal{B}(X; \mathbf{R})$ whose elements are the linear forms $\mu$ such that $\mu(1) = 1$. It is a subset of $E'$ which is convex and compact for $\sigma(E', E)$.*

Let $\mu$ be a linear form on E, such that $\mu(1) = 1$. For every function $f \in E$, we define the function $f' \in E$ by $f'(x) = \|f\| - f(x)$ ($x \in X$). First assume that $\mu$ is a mean; for every $f \in E$, we have $f' \geq 0$, hence $\mu(f') \geq 0$, *i.e.* $\mu(f) \leq \|f\|$; therefore $\|\mu\| \leq 1$.

Conversely, suppose $\mu$ belongs to $E'$, and that $\| \mu \| \leq 1$; for every positive function $f \in E$, we have $\mu(f') \leq \| f' \|$, hence

$$
\| f \| - \mu(f) = \mu(f') \leq \| f' \| \leq \| f \|,
$$

and finally $\mu(f) \geq 0$; consequently, $\mu$ is a mean.

It is clear that $K$ is convex; that it is compact for $\sigma(E', E)$ follows from cor. 3 of III, p. 17.

Q.E.D.

Let $\Gamma$ be a set of continuous mappings from $X$ into $X$ which commute pairwise. Let $\gamma \in \Gamma$. For every function $f \in E$, we have $f \circ \gamma \in E$; hence we can define an affine transformation $u_{\gamma}$ on the set $K$ of means on $X$, by

$$
u_{\gamma} \mu(f) = \mu(f \circ \gamma) \quad (\mu \in K, f \in E).
$$

If $K$ is assigned the topology induced by $\sigma(E', E)$, the mapping $u_{\gamma}$ is continuous. If $\gamma$ is a homeomorphism, $u_{\gamma} \mu$ can be deduced from $\mu$ by transport of structure. Finally, we have $u_{\gamma} u_{\gamma'} = u_{\gamma' \gamma} u_{\gamma}$ for all $\gamma, \gamma'$ in $\Gamma$. By the Markoff-Kakutani th. (IV, p. 39, th. 1), *there exists a mean $\mu$ on $X$, such that $u_{\gamma} \mu = \mu$ for all $\gamma \in \Gamma$; in other words*, $\mu$ satisfies the relation $\mu(f) = \mu(f \circ \gamma)$ for $f \in E$ and $\gamma \in \Gamma$.

In an analogous way, the corollary of th. 1 (IV, p. 40) implies the following result:

#### Proposition 1 {#evt-iv-a0-prop-1 .statement}

*Let $X$ be a topological space and $G$ a solvable group. We assume that $G$ operates on $X$ on the left, in such a way that for all $g \in G$, the mapping $x \mapsto g.x$ from $X$ into $X$ is continuous. Then there exists a mean on $X$ which is invariant under $G$.*

#### Corollary {#evt-iv-a0-n2-cor-1 .statement}

*Let $G$ be a solvable topological group. Then there exists a mean on $G$ which is invariant under the left and the right translations.*

It is enough to apply prop. 1 to the solvable group $G \times G$ acting on $G$ by $(g.g').x = {gxg'}^{-1}$.

### 3. Ryll-Nardzewski theorem

In this section, $E$ denotes a normed *space* over the field $\mathbf{R}$ and $\mathcal{T}$ a Hausdorff locally convex topology on $E$ for which the norm of $E$ is *lower semi-continuous*. These hypotheses are in particular satisfied in the following cases :

$a)$ $\mathcal{T}$ is the topology induced by the norm of the normed space $E$.
$b)$ $\mathcal{T}$ is the weakened topology $\sigma(E, E')$ of the normed space $E$.
$c)$ $E$ is the dual of a normed space $F$ and $\mathcal{T} = \sigma(F', F)$.
$d)$ There exist two normed spaces $F_1$ and $F_2$ such that $E = \mathscr{L}(F_1 ; F_2)$ and $\mathcal{T}$ is the topology of simple convergence.

*Unless otherwise expressly stated, the topological notions refer to the topology $\mathcal{T}$.*

Let $K$ be a convex subset of $E$. Suppose that $K$ is compact (for the topology $\mathcal{T}$), and that $K$ satisfies the first axiom of countability for the distance defined by the norm of $E$.

#### Lemma 2 {#evt-iv-a0-lem-2 .statement}

Suppose $K$ contains at least two points. For every $\varepsilon > 0$, there exists a partition of $K$ into two non-empty subsets $K_1$ and $K_2$, having the following properties :

a) $K_1$ is convex and compact ;
b) we have $\| x_1 - x_2 \| < \varepsilon$ for every $x_1$ and $x_2$ in $K_2$.

Let $L$ be the closure of the set of all extremal points of $K$. By the Krein-Milman th. (II, p. 55, th. 1), $K$ is the closed convex envelope of $L$. Since $K$ contains at least two points, so does $L$. For every $x \in L$, let $A_x$ be the set of all $y \in L$ such that $\| x - y \| \leq \varepsilon / 4$. By the hypothesis, on $K$, there exists a countable subset $D$ of $L$ such that $L = \bigcup_{x \in D} A_x$. Since the norm is lower semi-continuous, each of the sets $A_x$ is closed. Applying Baire’s th. (GT, IX, § 5, No. 3, th. 1) to the compact space $L$, we see that there exists a point $a$ in $D$ and an open subset $U$ in $E$ such that $L \cap U$ is non-empty and is contained in $A_a$. Since $L$ contains at least two points, and since $E$ is Hausdorff, we can choose $U$ in such a way that $L \notin U$.

Let $M$ be the closed convex envelope of $L \cap \complement U$. For every real number $t$ such that $0 < t < 1$, let $M_t$ be the set of all vectors of the form $tx_1 + (1 - t) x_2$ with $x_1 \in M$ and $x_2 \in K$; this is a non-empty, compact convex subset of $K$. We shall prove that $M_t \neq K$ by reductio ad absurdum. Suppose that $M_t = K$; then every extremal point $x$ in $K$ belongs to $M_t$, hence can be written in the form $x = tx_1 + (1 - t) x_2$ with $x_1 \in M$ and $x_2 \in K$. This implies that $x = x_1 = x_2$, and so $x \in M$. By Krein-Milman th. (II, p. 55, th. 1), we have $K = M$, and $K$ is the closed convex envelope of $L \cap \complement U$. By II, p. 56, corollary, this implies that $L \subset L \cap \complement U$, which contradicts the relation $L \cap U \neq \varnothing$.

Put $d = \sup_{x \in K, y \in K} \| x - y \|$ and choose a real number $t$ such that $0 < t < 1$ and $t < \varepsilon / 4d$. Put $K_1 = M_t$ and $K_2 = K - M_t$. By the preceding argument, the sets $K_1$ and $K_2$ are non-empty, and $K_1$ is convex and compact. Let $M'$ be the closed convex envelope of $L \cap U$. Since $K$ is the closed convex envelope of the set $L = (L \cap \complement U) \cup (L \cap U)$, it is also the closed convex envelope of $M \cup M'$. Let $x_1$ and $x_2$ be two points in $K_2$; for $i = 1, 2$, there exist $y_i \in M$, $z_i \in M'$ and a real number $\alpha_i$ such that $0 \leq \alpha_i \leq 1$ and $x_i = \alpha_i y_i + (1 - \alpha_i) z_i$. If $\alpha_i \geq t$, then
$$
x_i = t y_i + (1 - t) \left\{ \frac{\alpha_i - t}{1 - t} y_i + \frac{1 - \alpha_i}{1 - t} z_i \right\}
$$
; this contradicts the assumption that $x_i \notin M_i$. Hence $\alpha_i < t$, for $i = 1, 2$, and so
$$
\| x_i - z_i \| = \| \alpha_i (y_i - z_i) \| = \alpha_i \| y_i - z_i \| \leq \alpha_i d < dt < \varepsilon / 4 .
$$
For every point $z$ in $M'$, we have $\| z - a \| \leq \varepsilon / 4$, since $L \cap U \subset A_a$, and so, in particular $\| z_i - a \| \leq \varepsilon / 4$. Thus
$$
\| x_1 - x_2 \| \leq \sum_{i=1}^2 (\| x_i - z_i \| + \| z_i - a \|) < \varepsilon .
$$
This completes the proof.

#### Lemma 3 {#evt-iv-a0-lem-3 .statement}

Let G be a group of continuous (for $\mathcal{T}$) affine transformations on K. Suppose that K is non-empty and that $\|gx - gy\| = \|x - y\|$ for all x, y in K and all g in G. Then there exists a point in K which is invariant under G.

Let $\mathfrak{J}$ be the family of non-empty subsets of K which are closed convex and stable for G. If $(L_\alpha)_{\alpha \in I}$ is a family of elements of $\mathfrak{J}$ which is totally ordered by inclusion, then the set $L = \bigcap_{\alpha \in I} L_\alpha$ belongs to $\mathfrak{J}$. Consequently (S, III, § 3, No. 4, th. 2), there exists an element L in $\mathfrak{J}$ which is minimal for the relation of inclusion. We shall prove that L reduces to a point.

We argue by reductio ad absurdum, assuming that L contains at least two distinct points $x_1$ and $x_2$, put $x = (x_1 + x_2)/2$ and $\varepsilon = \|x_1 - x_2\|/2$. The convex and compact set L satisfies the first axiom of countability for the distance defined by the norm (GT, IX, § 2, No. 8). Hence we can apply lemma 2 and find a compact and convex subset $L_1$ of L, distinct from $\varnothing$ and from L, having the following property :

(A) *For every $y_1$ and $y_2$ in $L - L_1$, we have $\|y_1 - y_2\| < \varepsilon$.*

*We shall prove by reductio ad absurdum that $gx \in L_1$ for all $g \in G$.* Let $g \in G$ be such that $gx \in L - L_1$ then we have

$$
\|gx_i - gx\| = \|x_i - x\| = \|x_1 - x_2\|/2 = \varepsilon ,
$$

for $i = 1, 2$. By property (A), we have $gx_i \in L_1$. Since $L_1$ is convex, we conclude that $gx = (gx_1 + gx_2)/2$ belongs to $L_1$, which contradicts the assumption.

Let $L'$ be the closed convex envelope of the orbit $Gx$ of x. The set $L'$ belongs to $\mathfrak{J}$. By the preceding argument, we have $L' \subset L_1$, hence $L' \subset L, L' \neq L$. This contradicts the minimal character of L and the proof is complete.

#### Theorem 2 (Ryll-Nardzewski) {#evt-iv-a0-thm-2 .statement}

— *Let E be a normed space and K a non-empty convex subset of E, which is compact for the weakened topology $\sigma(E, E')$. Let G be a group of isometric affine transformations of K. Then there exists a point in K which is invariant under G.*

For every $g \in G$, let $K_g$ denote the set of all points x in K such that $gx = x$; let K be assigned the weakened topology; each set $K_g$ is convex and closed in the compact space K. We shall prove that the intersection $\bigcap_{g \in G} K_g$ is non-empty; for this, it is enough to prove that the set $K_{g_1} \cap ... \cap K_{g_n}$ is non-empty for every $g_1, ..., g_n$ in G. Fix $g_1, ..., g_n$ and let H be the subgroup of G generated by $\{ g_1, ..., g_n \}$. Choose a point a in K and let L denote the closed convex envelope of the orbit Ha of a. Let D be the countable set of elements of the form $\lambda_1 h_1 a + \cdots + \lambda_m h_m a$, where $\lambda_1, ..., \lambda_m$ are positive rational numbers such that $\lambda_1 + \cdots + \lambda_m = 1$, and $h_1, ..., h_m$ are elements in H. The closure $\overline{D}$ of D for the strong topology, is convex, hence it is closed for $\sigma(E, E')$ (IV, p. 4, prop. 2); therefore $\overline{D} = L$ and this proves that L is a metric space satisfying the first axiom of countability for the distance $(x, y) \mapsto \|x - y\|$. We can now apply lemma 2. There exists a point b in L which is invariant under H, hence $b \in K_{g_1} \cap ... \cap K_{g_n}$.

#### Corollary {#evt-iv-a0-n3-cor-1 .statement}

— Let E be a reflexive Banach space, G a group of automorphisms of the normed space E, and K a subset of E. Suppose that K is non-empty, convex, closed, bounded and stable under G. Then there exists a point in K which is invariant under G.

Since E is reflexive, K is compact for $\sigma(E, E')$ (IV, p. 15, th. 1). Moreover, every element of G belongs to $\mathcal{L}(E)$.

### 4. Applications.

\* A) Unitary representations of groups :
Let E be a complex hilbertian space, G a group and $\pi$ a unitary representation of G on E, i.e. a homomorphism from G into the group of automorphisms of E. Let $E^G$ be the hilbertian subspace of E consisting of all vectors invariant under $\pi(G)$. For every $x \in E$, let $K_x$ be the closed convex envelope of the orbit of x. Fix a point x in E.

We shall show that there exists a unique point in $K_x$ which is invariant under $\pi(G)$, namely the projection of x on $E^G$. By IV, p. 44, corollary (applied to the underlying real vector space to E), there exists a point in $K_x$ which is invariant under $\pi(G)$; let a be such a point; then $a \in E^G$. Let P be the set of all $y \in E$ such that $y - x$ is orthogonal to $E^G$; we see immediately that P is closed, convex and invariant under $\pi(G)$; therefore $x \in P$, hence $K_x \subset P$ and finally $a \in P$. In other words, $a - x$ is orthogonal to $E^G$; consequently a is the projection of x onto $E^G$. \*

\* B) Trace of an operator in a hilbertian space :
Suppose that the representation $\pi$ is irreducible, that is, that there exists no hilbertian subspace of E, distinct from $\{0\}$ and from E, which is invariant under $\pi(G)$. Let $F = \mathcal{L}^2(E)$ be the hilbertian space of all Hilbert-Schmidt endomorphisms of E, with the scalar product $\langle u|v \rangle = \operatorname{Tr}(u^*v)$. We define a unitary representation $\lambda$ from G into F by the formula

$$
\lambda(g).u = \pi(g)\ u\pi(g)^{-1} \quad (u \in F,\ g \in G)
$$

The space $F^G$ of all elements of E invariant under $\lambda(G)$ consists of the Hilbert-Schmidt endomorphisms $u$ of E which commute with $\pi(g)$ for all $g \in G$. By Schur’s lemma, such a $u$ is a homothety. Hence we must consider two cases :
1) if E is infinite dimensional, then $F^G = \{0\}$;
2) if E is finite dimensional, then $F = \mathcal{L}(E)$ and $F^G = \mathbf{C}.1_E$.

Applying the result of A) to the unitary representation $\lambda$, we obtain the following theorem :

Let $u \in \mathcal{L}^2(E)$, and let $A_u$ be the closed convex envelope in $\mathcal{L}^2(E)$ of the set of endomorphisms $\pi(g)\ u\pi(g)^{-1}$ of E, where g runs through G. If E is infinite dimensional, we have $0 \in A_u$. If E is finite dimensional with dimension d, there exists a unique homothety in $A_u$, namely the projection $\frac{1}{d}\ \operatorname{Tr}(u).\ 1_E$ of u onto the subspace $\mathbf{C}.1_E$ of $\mathcal{L}^2(E)$. \*

C) Haar measure of a compact group:

Let G be a compact group and let E = $\mathcal{C}(G, \mathbf{R})$ be the Banach space of all real valued continuous functions on G, endowed with the norm

$$
\| f \| = \sup_{x \in G} |f(x)| .
$$

For all $x \in G$, we define the automorphisms $\gamma_x$ and $\delta_x$ of E by the formulas

$$
\gamma_x f(y) = f(x^{-1}y) , \quad \delta_x f(y) = f(yx)
$$

(for $y \in G,\ f \in E$).

*Let $f \in E$, let $\Gamma_f$ (resp. $\Delta_f$) denote the closed convex envelope i. E, of the set of all functions $\gamma_x f$ (resp. $\delta_x f$) as x ranges over G. We shall prove that there exists a unique constant function $\mu(f)$ belonging to $\Gamma_f$, a unique constant function $\mu'(f)$ belonging to $\Delta_f$, and that these constants are equal.*

It is clear that a continuous function on G is invariant under the automorphisms $\gamma_x$ (resp. $\delta_x$) of E if and only if it is constant. Now the set of all functions $\gamma_x f$ (resp. $\delta_x f$) for x in G, is compact in E, since the mapping $x \mapsto \gamma_x f$ (resp. $x \mapsto \delta_x f$) from G into E is continuous (GT, X, § 3, No. 4, th. 3). It follows (II, p. 25, prop. 3) that $\Gamma_f$ (resp. $\Delta_f$) is a compact set in E for the topology defined by the norm, hence for $\sigma(E, E')$. By the Ryll-Nardzewski th. (IV, p. 43, th. 2), there exist constant functions in $\Gamma_f$ and $\Delta_f$. It remains to prove that if $c_1 \in \Gamma_f$ and $c_2 \in \Delta_f$ are constants, then $c_1 = c_2$.

Let $\varepsilon > 0$. By the hypothesis there exist points $x_1, ..., x_n,\ y_1, ..., y_n$ in G and positive real numbers $\lambda_1, ..., \lambda_n,\ \mu_1, ..., \mu_m$ such that

$$
\lambda_1 + \cdots + \lambda_n = \mu_1 + \cdots + \mu_m = 1 .
$$
$$
\sup_{x \in G} \left| \sum_{i=1}^n \lambda_i f(x_i x) - c_1 \right| \leq \varepsilon ,
$$
$$
\sup_{x \in G} \left| \sum_{j=1}^m \mu_j f(xy_j) - c_2 \right| \leq \varepsilon .
$$

Put $r = \sum_{i,j} \lambda_i \mu_j f(x_i y_j)$. Then $r - c_1 = \sum_{j=1}^m \mu_j a_j$ with $a_j = \sum_{i=1}^n \lambda_i f(x_i y_j) - c_1$; by (7), we have $|a_j| \leq \varepsilon$ for $1 \leq j \leq m$, hence $|r - c_1| \leq \varepsilon$. Similarly, we prove the inequality $|r - c_2| \leq \varepsilon$, hence $|c_1 - c_2| \leq 2\varepsilon$. Since $\varepsilon$ is arbitrary, we get $c_1 = c_2$, as asserted.

By the definition of $\mu(f)$, for every $\varepsilon > 0$ we can find positive numbers $\lambda_1, ..., \lambda_n$ with sum 1 and elements $x_1, ..., x_n$ in G such that $\left| \sum_{i=1}^n \lambda_i f(x_i x) - \mu(f) \right| \leq \varepsilon$ for all $x \in G$.

It is immediate that for $f, g$ in E and for every scalar $\lambda$, we have $\Gamma_{f+g} \subset \Gamma_f + \Gamma_g$ and $\Gamma_{\gamma f} = \lambda \Gamma_f$, hence we have the relations $\mu(f+g) = \mu(f) + \mu(g)$ and $\mu(\lambda f) = \lambda \mu(f)$. Therefore, the mapping $\mu : f \mapsto \mu(f)$ from E into $\mathbf{R}$ is a mean on the compact space G (IV, p. 40); *in other words $\mu$ is a positive measure on G such that $\mu(G) = 1$*.

It is immediate that $\mu$ is invariant under the left translations of $G$, and the equality $\mu(f) = \mu'(f)$ implies that $\mu$ is also invariant under right translations. \* In other words, $\mu$ is a left and a right measure on $G$ (INT, VII, § 1, No. 2, def. 2). \*

*D) Existence of invariant measures :

Let $X$ be a Hausdorff topological space, $\mu$ a positive bounded measure on $X$, and $G$ a group of homeomorphisms of $X$. Suppose that for all $g \in G$, the measure $g.\mu$, the image of $\mu$ under the mapping $g : X \to X$ is of base $\mu$. Let $u_g$ be a positive $\mu$-integrable function on $X$ such that $g.\mu = u_g.\mu$. Suppose also that there exist two positive $\mu$ integrable functions $\phi$ and $\psi$ on $X$, which are not $\mu$-null and are such that $\phi \leq u_g \leq \psi$ $\mu$-almost everywhere for all $g \in G$. We shall prove that there exists a positive bounded measure $\nu \neq 0$ on $X$, with base $\mu$, and invariant under $G$.

Let $P$ be the subset of the Banach space $E = L^1(X, \mu)$ consisting of classes of functions $f$ such that $\phi \leq f \leq \psi$ $\mu$-almost everywhere. Then $P$ is compact for the weakened topology $\sigma(E, E')$. The mapping $h \mapsto h.\mu$ from $P$ into the Banach space $F = \mathcal{M}^b(X)$ of bounded real measures on $X$, is a bijection from $P$ onto a subset $P_1$ of $E$ which is convex and compact for the topology $\sigma(F, F')$. By hypothesis, $g.\mu \in P_1$ for all $g \in G$. Let $K$ be the closed convex envelope of the set of all measures $g.\mu$. For all $g \in G$, the mapping $\nu \mapsto g.\nu$ is an isometric affine transformation of $K$. By the Ryll-Nardzewski th. (IV, p. 43, th. 2), there exists a measure $\nu \in K$ which is invariant under $G$. We have $\phi.\mu \leq \nu$, hence $\nu \neq 0$. \*

Exercises

### Exercises {#evt-iv-a0-exercises}

See the [exercises for Appendix 0](exercises/a0/).
