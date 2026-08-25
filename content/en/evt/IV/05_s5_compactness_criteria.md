---
book: evt
book_title: Topological Vector Spaces
chapter: IV
chapter_title: DUALITY IN TOPOLOGICAL VECTOR SPACES
section: 5
section_title: Compactness criteria
lang: en
source: evt-i-v
book_pages: TVS IV.32-TVS IV.38, TVS IV.67-TVS IV.71
pdf_pages: 0214-0220, 0249-0253
extraction: ocr
subsections:
    - "no": 1
      title: General remarks
      page: 32
      pdf_page: 214
    - "no": 2
      title: Simple compactness of sets of continuous functions
      page: 33
      pdf_page: 215
    - "no": 3
      title: The Eberlein and Šmulian theorems
      page: 35
      pdf_page: 217
    - "no": 4
      title: The case of spaces of bounded continuous functions*
      page: 36
      pdf_page: 218
    - "no": 5
      title: Convex envelope of a weakly compact set
      page: 37
      pdf_page: 219
statements: 8
exercises: 18
content_sha256: 74acd4eb366456136b6614676effa587ce4c4fa1a461711a3f53b2c158904c50
---

## § 5. COMPACTNESS CRITERIA

### 1. General remarks

Let A be a subset of a topological space E. For a sequence $(x_n)_{n \in \mathbf{N}}$ of points of A to have a point x of E as a limit point, it is necessary and sufficient that the following condition is satisfied (GT, I, § 7, No. 3) :

(A) For every integer $m \geq 0$ and every neighbourhood U of x, there exists an integer $n \geq m$ such that $x_n \in U$.

A sequence of the form $(y_k)_{k \in \mathbf{N}}$ with $y_k = x_{n_k}$ for a strictly increasing sequence $(n_k)_{k \in \mathbf{N}}$ of positive integers is called an extracted sequence of the sequence $(x_n)_{n \in \mathbf{N}}$. If there exists an extracted sequence of the sequence $(x_n)_{n \in \mathbf{N}}$ which converges to x, then x is a limit point of $(x_n)$; conversely, if x has a countable fundamental system of neighbourhoods, and x is the limit point of the sequence $(x_n)$, then there exists an extracted sequence of $(x_n)$ converging to x.

On account of GT, IX, § 2, No. 9, corollary, we conclude that when E is metrizable, the following conditions are equivalent :
a) the set A is relatively compact in E ;
b) every infinite sequence of points of A has a limit point in E ;
c) from every infinite sequence of points of A, we can extract a sequence which converges to a point of E.

In this section, we shall extend this criterion to certain non metrizable topological vector spaces. The following proposition enables us to reduce the study of compact sets to that of weakly compact sets in a number of cases.

#### Proposition 1 {#evt-iv-s5-prop-1 .statement}

— Let E be a Hausdorff locally convex space, and A a subset of E. Let $E_\sigma$ denote the space E with the weakened topology.
a) If every infinite sequence of points of A has a limit point in E, then A is precompact in E.
b) In order that A be relatively compact in E, it is necessary and sufficient that it is precompact in E and relatively compact in $E_\sigma$.

We shall prove a) by reductio ad absurdum. If A is not precompact, then by th. 3 of GT, II, § 3, No. 7, it follows that there exists a symmetric convex neighbourhood V of 0 in E such that A cannot be covered by a finite number of translates of V.

In other words, if $x_0, x_1, ..., x_{n-1}$ are points of A, then $A \notin \bigcup_{0 \leq i < n} (x_i + V)$ and so there exists a point $x_n$ of A such that $x_n - x_i \notin V$ for $0 \leq i < n$. Then, by induction on the integer $n$, we can construct an infinite sequence $(x_n)_{n \in \mathbf{N}}$ of points of A such that $x_n - x_m \notin V$ whenever $n > m$; since V is symmetric, we also have $x_m - x_n \notin V$ for $m \neq n$ and the sets $x_n + \frac{1}{2} V$ are disjoint. For every point $x$ in E, there exists at most one integer $n \geq 0$ such that $x_n \in x + \frac{1}{2} V$, hence the sequence $(x_n)_{n \in \mathbf{N}}$ does not have any limit point. This proves *a)*.

Now suppose that A is precompact in E and is contained in a compact subset B of $E_\sigma$. Then B is complete in $E_\sigma$, hence also in E (IV, p. 5, *Remark 2*). We have $\overline{A} \subset B$, hence A is relatively compact in E. The converse is evident and *b)* follows.

### 2. Simple compactness of sets of continuous functions

In this section, X denotes a *compact* space and $\mathcal{C}_s(X)$ the space of continuous functions on X, with values in the field K (equal to $\mathbf{R}$ or $\mathbf{C}$). The space $\mathcal{C}_s(X)$ is assigned the topology of simple convergence on X.

#### Proposition 2 {#evt-iv-s5-prop-2 .statement}

*Let D be a dense subset of X and A a subset of the space $\mathcal{C}_s(X)$. The following conditions are equivalent :*
(i) *A is relatively compact in $\mathcal{C}_s(X)$.*
(ii) *From every infinite sequence of elements of A, we can extract a sequence converging in $\mathcal{C}_s(X)$.*
(iii) *Every infinite sequence of elements of A has a limit point in $\mathcal{C}_s(X)$.*
(iv) *Let $(f_n)_{n \in \mathbf{N}}$ be a sequence of functions belonging to A and $(x_m)_{m \in \mathbf{N}}$ a sequence of points of D. If the iterated limits*

$$
\gamma = \lim_{m \to \infty} \lim_{n \to \infty} f_n(x_m), \quad \delta = \lim_{n \to \infty} \lim_{m \to \infty} f_n(x_m)
$$

*exist, then they are equal. In addition, we have $\sup_{f \in A} |f(x)| < + \infty$ for all $x \in X$.*

(i) $\Rightarrow$ (ii) : let $\overline{A}$ be the closure of A in $\mathcal{C}_s(X)$. Assume that A is compact, and consider a sequence of functions $f_n \in A$ (for $n \in \mathbf{N}$). Let $\phi$ be the continuous mapping $x \mapsto (f_n(x))_{n \in \mathbf{N}}$ from X into the metrizable space $K^\mathbf{N}$. The image $X'$ of X under $\phi$ is a compact metrizable space, since X is compact. Let E be the closed subspace of $\mathcal{C}_s(X)$ consisting of continuous functions $f$ on X such that the relation $\phi(x) = \phi(y)$ implies $f(x) = f(y)$ for every pair of points $x, y$ in X. By cor. 2 of GT, I, § 9, No. 4 and prop. 3 of GT, I, § 5, No. 2, the mapping $f' \mapsto f' \circ \phi$ is a homeomorphism $\phi^*$ from $\mathcal{C}_s(X')$ onto E. Hence the set $A' = (\phi^*)^{-1}(\overline{A})$ is compact in $\mathcal{C}_s(X')$, and it is clear that there exist elements $f'_n$ in $A'$ such that $\phi^*(f'_n) = f'_n \circ \phi$ is equal to $f_n$.

Since $X'$ is a compact metrizable space, there exists a countable dense subset D' in $X'$ (GT, IX, § 2, No. 8, prop. 12 and § 2, No. 9, prop. 16). Let $\mathcal{T}_1$ (resp. $\mathcal{T}_2$) be the topology on $A'$ induced by the topology of simple convergence on D' (resp. $X'$). Then $\mathcal{T}_1$ is metrizable, $\mathcal{T}_2$ is compact and finer than $\mathcal{T}_1$, hence $\mathcal{T}_1$ and $\mathcal{T}_2$ coincide; in other words, $A'$ is a compact *metrizable* subspace of $\mathcal{C}_s(X')$. Therefore, there exists a sequence $(f'_{n_k})$ extracted from $(f'_n)$ and converging to an element $f'$ of $\mathcal{C}_s(X')$. Therefore, the sequence $(f_{n_k})$ converges to $f = f' \circ \phi$ in $\mathcal{C}_s(X)$.

(ii) $\Rightarrow$ (iii) : this is clear.

(iii) $\Rightarrow$ (iv) : suppose that every infinite sequence of elements of A has a limit point in $\mathcal{C}_s(X)$. Let $x \in X$. The mapping $\phi_x : f \mapsto f(x)$ from A into K is continuous. Consequently, every infinite sequence in $\phi_x(A)$ has a limit point; since the field K (equal to $\mathbf{R}$ or $\mathbf{C}$) is metrizable, the set $\phi_x(A)$ is relatively compact in K, hence bounded. In other words, we have $\sup_{f \in A} |f(x)| < \infty$.

Let $f_n, x_m, \gamma$ and $\delta$ be as in (iv). Let $f$ be a limit point of the sequence $(f_n)$ in $\mathcal{C}_s(X)$, and let $x$ be a limit point of the sequence $(x_m)$ in the compact space X. For every $m$, the mapping $h \mapsto h(x_m)$ from $\mathcal{C}_s(X)$ into K is continuous. In view of the hypotheses, we have $f(x_m) = \lim_{n \to \infty} f_n(x_m)$, and hence $\gamma = \lim_{m \to \infty} f(x_m)$; since $f : X \to K$ is continuous and $x$ is a limit point of the sequence $(x_m)$, we get $\gamma = f(x)$. In an analogous way, we prove the equality $\delta = f(x)$, whence $\gamma = \delta$.

(iv) $\Rightarrow$ (i) : suppose that the set of numbers $f(x)$, as $f$ ranges over A, is bounded in K for all $x \in X$. This is equivalent to assuming that the closure $\overline{A}$ of A in the product space $K^X$ is compact (GT, I, § 9, No. 5). Suppose that A *is not relatively compact in* $\mathcal{C}_s(X)$. This means that there exists a function $u \in \overline{A}$ and a point $a \in X$ such that $u$ is not continuous at $a$. Hence there exists a real number $\varepsilon > 0$ such that in every neighbourhood U of $a$, there exists a point $x$ with $|u(x) - u(a)| \geq \varepsilon$.

We shall construct by induction a sequence $(x_n)_{n \in \mathbf{N}}$ of points in D and a sequence $(f_n)_{n \in \mathbf{N}}$ of elements of A, satisfying the following relations :

(1)$_m$ $$ |u(x_m) - u(a)| \geq \varepsilon \quad \text{for} \quad m \geq 1 ; $$

(2)$_m$ $$ |u(x_i) - f_m(x_i)| \leq \frac{1}{m + 1} \quad \text{for} \quad 0 \leq i \leq m - 1 ; $$

(3)$_{m,i}$ $$ |f_m(x_i) - f_m(a)| \leq \frac{1}{i + 1} \quad \text{for} \quad 0 \leq m \leq i . $$

We take $x_0 = a$ with $f_0$ arbitrary in A (the set A is not empty, otherwise it will be relatively compact in $\mathcal{C}_s(X)$). Let $n \geq 1$ and $x_0, x_1, ..., x_{n-1}, f_0, f_1, ..., f_{n-1}$ satisfy relations (1)$_m$, (2)$_m$ for $1 \leq m < n$ and (3)$_{m,i}$ for $0 \leq m \leq i < n$. Since $u$ belongs to $\overline{A}$, there exists $f_n \in A$ satisfying (2)$_n$. Let $V_n$ be the set of all $x \in X$ such that $|f_m(x) - f_m(a)| \leq \frac{1}{n + 1}$ for $0 \leq m \leq n$. Since $f_n$ is continuous, $V_n$ is a neighbourhood of $a$; choose a point $x_n$ in $D \cap V_n$ such that $|u(x_n) - u(a)| \geq \varepsilon$, hence (1)$_n$ and (3)$_{m,n}$ are satisfied. Therefore, the construction can be continued.

Since $u(X)$ is a compact subset of K, there exists a sequence $(y_k)$ extracted from $(x_m)$ and such that the limit $\gamma = \lim_{k \to \infty} u(y_k)$ exists. By (2)$_m$, we have $u(x_i) = \lim_{n \to \infty} f_n(x_i)$ for all $i \in \mathbf{N}$, hence

(4) $$
\gamma = \lim_{k \to \infty} \lim_{n \to \infty} f_n(y_k) .
$$

On the other hand we have $f_n(a) = \lim_{i \to \infty} f_n(x_i)$ by (3)$_{m,i}$ hence $f_n(a) = \lim_{k \to \infty} f_n(y_k)$. Since $x_0 = a$, we deduce from (2)$_m$ that $\lim_{n \to \infty} f_n(a) = u(a)$. Consequently,

$$
u(a) = \lim_{n \to \infty} \lim_{k \to \infty} f_n(y_k) .
$$

Finally, from (1)$_m$, we get $|\gamma - u(a)| \geq \varepsilon$, and so $\gamma \neq u(a)$. This contradicts assertion (iv); we have thus proved that (iv) implies (i).

### 3. The Eberlein and Šmulian theorems

#### Theorem 1 (Eberlein) {#evt-iv-s5-thm-1 .statement}

— *Let E be a Hausdorff and quasi-complete locally convex space, $\mathcal{T}$ a topology on E which is compatible with the duality between E and E' and A a subset of E. For A to be relatively compact for $\mathcal{T}$, it is necessary and sufficient that every infinite sequence of points of A has a limit point in E for $\mathcal{T}$.*

The condition stated is obviously necessary.

Suppose now that every infinite sequence of points of A has a limit point for $\mathcal{T}$, hence also for the coarser topology $\sigma(E, E')$. Then A is precompact for $\mathcal{T}$ (IV, p. 32, prop. 1); in order that A be relatively compact for $\mathcal{T}$, it is necessary and sufficient that it be so for $\sigma(E, E')$ (*loc. cit.*). Therefore it is enough to prove the theorem when $\mathcal{T}$ is the weakened topology $\sigma(E, E')$.

Let $\hat{E}$ denote the completion of E, which we shall identify as usual with a subspace of the algebraic dual ${E'}^*$ of E' (III, p. 21, th. 2). Let $E_\sigma$, $\hat{E}_\sigma$ and $E_{\sigma'}^*$ denote the spaces E, $\hat{E}$ and ${E'}^*$ endowed with the topologies $\sigma(E, E')$, $\sigma(\hat{E}, E')$ and $\sigma({E'}^*, E')$ respectively.

Let $(x'_i)_{i \in I}$ be a basis of the vector space E' over the field K. The mapping $f \mapsto (f(x'_i))_{i \in I}$ is a homeomorphism $\phi$ from $E_{\sigma'}^*$ onto $K^I$; for every $i \in I$, the image of A under the mapping $x'_i$ from E into K is relatively compact : for, K is metrizable and every infinite sequence of elements of $x'_i(A)$ has a limit point. It follows that $\phi(A)$ is relatively compact in $K^I$, hence that the closure $\overline{A}$ of A in $E_{\sigma'}^*$ is compact.

*Next we shall prove that $\overline{A}$ is contained in $\hat{E}$.* Let H be an equicontinuous subset of E'; let X be its closure for $\sigma(E', E)$; X is compact (III, p. 17, cor. 2). For every $x \in {E'}^*$, let $\phi_x$ be the restriction of $x' \mapsto \langle x, x' \rangle$ to X; let $\tilde{A} \subset \mathscr{C}_s(X)$ be the set of functions $\phi_x$ as x ranges over A. In view of the hypothesis on A, every infinite sequence of elements of $\tilde{A}$ has a limit point in $\mathscr{C}_s(X)$; by prop. 2 (IV, p. 33), the set $\tilde{A}$ is therefore relatively compact in $\mathscr{C}_s(X)$. *It follows that for every $a \in \overline{A}$, the function $\phi_a$ on X is continuous.* The inclusion $\overline{A} \subset \hat{E}$ then follows from th. 2 of III, p. 21.

*Now we shall show that $\overline{A}$ is contained in E.* Since A is precompact in $E_\sigma$ (IV, p. 32, prop. 1), it is bounded in $E_\sigma$ (III, p. 3, prop. 2), hence also in E (IV, p. 1, prop. 1). Let C be the closed convex balanced envelope of A in E. Then C is bounded since A is bounded, hence complete since E is quasi-complete. In other words, C is a convex and closed subset of $\hat{E}$, so also of $\hat{E}_\sigma$ (IV, p. 1, prop. 1). Since $A \subset C$ and the topology of $\hat{E}_\sigma$ is induced by that of $E_{\sigma'}^*$, we have $\overline{A} \subset C$, and hence $\overline{A} \subset E$.

Since the topology of $E_\sigma$ is induced by that of ${E'_\sigma}^*$, the subset $\overline{A}$ of $E_\sigma$ is compact, and th. 1 follows.

**Theorem 2 (Šmulian).** — *Let E be a Fréchet space and A a subset of E. Let $E_\sigma$ denote the space E endowed with the weakened topology. The following conditions are equivalent* :

(i) *A is relatively compact in $E_\sigma$;*
(ii) *every infinite sequence of points of A has a limit point in $E_\sigma$;*
(iii) *from every infinite sequence of points of A, we can extract a sequence which converges in $E_\sigma$.*

The equivalence of (i) and (ii) follows from Eberlein’s theorem and (iii) obviously implies (ii).

We shall prove that (i) implies (iii). Suppose that the closure B of A in $E_\sigma$ is compact and that $(x_n)_{n \in \mathbf{N}}$ is a sequence of points of A. Let F denote the smallest closed vector subspace of E containing the $x_n$, this is a Fréchet space satisfying the first axiom of countability. Since F is closed in $E_\sigma$ and the topology $\sigma(F, F')$ on F is induced by $\sigma(E, E')$, the set $B \cap F$ is compact for $\sigma(F, F')$. On account of the remarks in IV, p. 32, the existence of a sequence extracted from $(x_n)_{n \in \mathbf{N}}$ converging for $\sigma(E, E')$ (or, which is the same, for $\sigma(F, F')$) is a consequence of the following lemma :

#### Lemma 1 {#evt-iv-s5-lem-1 .statement}

— *Let F be a Fréchet space satisfying the first axiom of countability. Every subset C of F which is compact for the topology $\mathcal{T}$ induced by $\sigma(F, F')$ is metrizable for this topology.*

Since the topology of precompact convergence on $F'$ is finer than the topology $\sigma(F', F)$, there exists an everywhere dense countable subset in $F'_s$ (III, p. 18, cor. 1). Hence the set C can be identified with a subset of $K^D$, and the topology induced on C by that of $K^D$, which is metrizable (GT, IX, § 2, No. 8) is coarser than the topology induced by $\sigma(F, F')$, for which C is compact. Hence these two topologies are identical (GT, I, § 9, No. 4, cor. 3).

Šmulian’s theorem can be extended to the case where E is the strict inductive limit of a sequence of Fréchet spaces (IV, p. 67, exerc. 2).

### *4. The case of spaces of bounded continuous functions*

For every topological space X, let $\mathscr{C}^b(X)$ denote the Banach space of all continuous and *bounded* mappings from X into K, with the norm defined by

$$
\| f \| = \sup_{x \in X} |f(x)|
$$

(GT, X, § 3, No. 2). When X is compact, every continuous function on X is bounded (GT, IV, § 6, No. 1), and we write $\mathscr{C}(X)$ for $\mathscr{C}^b(X)$.

In this and the following section, we shall use the following lemma, which is a particular case of Lebesgue’s theorem (INT, IV, 2nd ed. § 4, No. 3, th. 2) on account of the interpretation of the elements of $\mathscr{C}(X)'$ as measures on X.

#### Lemma 2 {#evt-iv-s5-lem-2 .statement}

Let X be a compact space. If a sequence $(f_n)_{n \in \mathbf{N}}$ is bounded in $C(X)$ and converges simply on X to a continuous function f, then $\mu(f) = \lim_{n \to \infty} \mu(f_n)$ for every $\mu$ in $C(X)'$.

#### Proposition 3 {#evt-iv-s5-prop-3 .statement}

Let X be a compact space, and let A be a bounded subset of $C(X)$. For A to be relatively compact for the topology of simple convergence, it is necessary and sufficient that it is relatively compact for $\sigma(C(X), C(X)')$.

The topology of simple convergence is Hausdorff and coarser than $\sigma(C(X), C(X)')$, hence the condition stated is sufficient (GT, I, § 9, No. 4, cor. 3).

Now suppose that A is relatively compact for the topology of simple convergence. Let $(f_n)_{n \in \mathbf{N}}$ be a sequence of elements of A. By prop. 2 (IV, p. 33), there exists a sequence $(f_{n_k})$ extracted from $(f_n)$ and converging simply to a continuous function f. By lemma 2, the bounded sequence $(f_{n_k})$ tends to f for $\sigma(C(X), C(X)')$. Then Šmulian’s theorem (IV, p. 36, th. 2) shows that A is relatively compact for $\sigma(C(X), C(X)')$.

#### Corollary {#evt-iv-s5-n4-cor-1 .statement}

Let S be a topological space and A a bounded subset of $C^b(S)$. The following conditions are equivalent :
(i) A is relatively compact for $\sigma(C^b(S), C^b(S'))$;
(ii) if $(f_n)_{n \in \mathbf{N}}$ is a sequence of elements of A and $(x_m)_{m \in \mathbf{N}}$ is a sequence of points of S such that the iterated limits
$$
\gamma = \lim_{m \to \infty} \lim_{n \to \infty} f_n(x_m), \quad \delta = \lim_{n \to \infty} \lim_{m \to \infty} f_n(x_m)
$$
exist, then $\gamma = \delta$.

Let X be the Stone-Čech compactification of S (GT, IX, § 1, No. 6) and $\alpha$ the canonical mapping from S into X. Put D = $\alpha(S)$. The mapping $\phi : f \mapsto f \circ \alpha$ is an isomorphism from the normed space $C(X)$ onto the normed space $C^b(S)$; put $\tilde{A} = \phi^{-1}(A)$. Since X is compact and D is dense in X, the prop. 2 (IV, p. 33) shows that condition (ii) is equivalent to the compactness of $\tilde{A}$ for the topology of simple convergence. The equivalence of (i) and (ii) then follows from prop. 3. *

### *5. Convex envelope of a weakly compact set

#### Theorem 3 (Krein) {#evt-iv-s5-thm-3 .statement}

Let E be a Hausdorff and quasi-complete locally convex space, and let $\mathcal{T}$ be a topology on E compatible with the duality between E and E'. Let A be a subset of E which is compact for $\mathcal{T}$. Then the closed convex balanced envelope C of A is compact for $\mathcal{T}$.

We shall first make several reductions.
A) The set C is precompact for $\mathcal{T}$ (II, p. 25, prop. 3), and A is compact for $\sigma(E, E')$. On account of prop. 1 (IV, p. 32), it is enough to prove that C is compact for $\sigma(E, E')$, and so we have reduced to the case where $\mathcal{T} = \sigma(E, E')$.
B) Since C is precompact and closed for $\sigma(E, E')$, it is bounded and closed for the initial topology of E (III, p. 3, prop. 2 and IV, p. 1, prop. 1); hence it is complete since E is quasi-complete. In other words, C is the closed convex balanced envelope of $A$ in the completion $\hat{E}$ of $E$. Since the topology $\sigma(\hat{E}, E')$ induces $\sigma(E, E')$ on $E$, we have reduced *to the case when $E$ is complete*.

C) Let $\Gamma$ be the convex balanced envelope of $A$. Then $C$ is the closure of $\Gamma$ for $\sigma(E, E')$. By Eberlein’s theorem (IV, p. 35, th. 1), it is enough to prove that every sequence $(x_n)_{n \in \mathbf{N}}$ of points of $\Gamma$ has a limit point for $\sigma(E, E')$ in $E$. But $x_n$ belongs to the convex balanced envelope of a finite subset $B_n$ of $A$. Let $F$ be the closed vector subspace of $E$ generated by the countable set $B = \bigcup_n B_n$. Then $F$ is complete, the topology $\sigma(F, F')$ on $F$ is induced by $\sigma(E, E')$ and we have $x_n \in F$ for all $n \in \mathbf{N}$. Hence it is enough to prove that $(x_n)_{n \in \mathbf{N}}$ has a limit point for $\sigma(F, F')$, which gives the reduction to *the case when there exists a countable dense set in $E$*.

Let $A$ be assigned the topology induced by $\sigma(E, E')$, which makes it a compact space. We define a linear mapping $u : E' \to \mathcal{C}(A)$ by

$$
u(x')(a) = \langle a, x' \rangle \quad (a \in A, x' \in E') .
$$

Let $(x'_n)_{n \in \mathbf{N}}$ be an equicontinuous sequence in $E'$, converging to 0 for $\sigma(E', E)$. Then the sequence of functions $u(x'_n)$ is bounded in $\mathcal{C}(A)$ and converges simply to 0. For every $\mu \in \mathcal{C}(A)'$, we have $\lim_{n \to \infty} \mu(u(x'_n)) = 0$ by lemma 2 (IV, p. 37). By the criterion given in the remark in III, p. 21, the linear form $\mu \circ u$ on $E'$ is then continuous for $\sigma(E', E)$ for every $\mu \in \mathcal{C}(A)'$. Hence there exists a linear mapping $v : \mathcal{C}(A)' \to E$ satisfying the relation

$$
\langle u(x'), \mu \rangle = \langle v(\mu), x' \rangle \quad (x' \in E', \mu \in \mathcal{C}(A)') .
$$

It is clear that $v$ is continuous if $\mathcal{C}(A)'$ is assigned the topology $\sigma(\mathcal{C}(A)', \mathcal{C}(A))$ and $E$ the topology $\sigma(E, E')$.

The unit ball (closed) $B$ of the Banach space $\mathcal{C}(A)$ is compact for the topology $\sigma(\mathcal{C}(A)', \mathcal{C}(A))$ (III, p. 17, cor. 3). Consequently, $v(B)$ is a convex balanced and compact subset of $E$ for $\sigma(E, E')$. For every $a \in A$, the continuous linear form $\varepsilon_a : f \mapsto f(a)$ on $\mathcal{C}(A)$ belongs to $B$, and we have $v(\varepsilon_a) = a$ by formulas (7) and (8). Hence, $A \subset v(B)$, and so $C \subset v(B)$. This proves that $C$ is compact for $\sigma(E, E')$.

Q.E.D.

### Exercises {#evt-iv-s5-exercises}

See the [exercises for § 5](exercises/s5/).
