---
book: evt
book_title: Topological Vector Spaces
chapter: IV
chapter_title: DUALITY IN TOPOLOGICAL VECTOR SPACES
section: 3
section_title: Dual of a Fréchet space
lang: en
source: evt-i-v
book_pages: TVS IV.21-TVS IV.26, TVS IV.57-TVS IV.61
pdf_pages: 0203-0208, 0239-0243
extraction: ocr
subsections:
    - "no": 1
      title: Semi-barrelled spaces
      page: 21
      pdf_page: 203
    - "no": 2
      title: Dual of a locally convex metrizable space
      page: 22
      pdf_page: 204
    - "no": 3
      title: Bidual of a locally convex metrizable space
      page: 23
      pdf_page: 205
    - "no": 4
      title: Dual of a reflexive Fréchet space
      page: 23
      pdf_page: 205
    - "no": 5
      title: The topology of compact convergence on the dual of a Fréchet space
      page: 24
      pdf_page: 206
    - "no": 6
      title: Separately continuous bilinear mappings
      page: 26
      pdf_page: 208
statements: 15
exercises: 2
content_sha256: f4266311de13748ecb57cc35032fc0f86227db873b93678214776c3770519275
---

## § 3. DUAL OF A FRÉCHET SPACE

### 1. Semi-barrelled spaces

#### Proposition 1 {#evt-iv-s3-prop-1 .statement}

— Let E be a locally convex space. The following conditions are equivalent :

(i) Let U be a subset of E which absorbs every bounded subset of E, and which is the intersection of a sequence of convex, balanced and closed neighbourhoods of 0 in E. Then U is a neighbourhood of 0 in E.

(ii) For every locally convex space F, every bounded subset of $\mathcal{L}_b(E; F)$ which is the union of a countable family of equicontinuous subsets, is equicontinuous.

(iii) In the strong dual $E'_b$ of E, every bounded subset which is the union of a countable family of equicontinuous subsets, is equicontinuous.

It is clear that (iii) is a particular case of (ii).

(i) $\Rightarrow$ (ii) : let H be a bounded subset of $\mathcal{L}_b(E; F)$, and let $(H_n)$ be a sequence of equicontinuous subsets of $\mathcal{L}_b(E; F)$ such that $H = \bigcup H_n$. Let V be a convex, balanced and closed neighbourhood of 0 in F. For every $n$, the set $W_n = \bigcap_{u \in H_n} u^{-1}(V)$ is a convex, balanced and closed neighbourhood of 0 in E since $H_n$ is equicontinuous. The set $W = \bigcap_{u \in H} u^{-1}(V)$ absorbs every bounded subset of E, since H is bounded in $\mathcal{L}_b(E; F)$ (III, p. 22), and we have $W = \bigcap_n W_n$. If E satisfies (i), then the set W is a neighbourhood of 0 in E, hence H is equicontinuous.

(iii) $\Rightarrow$ (i) : let $(U_n)$ be a sequence of convex, balanced and closed neighbourhoods of 0 in E. We assume that the set $U = \bigcap_n U_n$ absorbs every bounded subset of E, hence that its polar $U^\circ$ is bounded in $E'_b$. Then the set $B = \bigcup_n U_n^\circ$ is contained in $U^\circ$, hence is bounded in $E'_b$. If E satisfies (iii), the set B is equicontinuous in $E'$; consequently, the polar $B^\circ = \bigcap_n (U_n^\circ)^\circ = \bigcap_n U_n = U$ of B in E is a neighbourhood of 0 in E.

#### Definition 1 {#evt-iv-s3-def-1 .statement}

— A locally convex space E is said to be semi-barrelled if it satisfies the equivalent conditions of prop. 1.

Every barrelled space is semi-barrelled. This is also true for every bornological space (III, p. 22, prop. 10).

### 2. Dual of a locally convex metrizable space

#### Proposition 2 {#evt-iv-s3-prop-2 .statement}

— Let E be a locally convex metrizable space and F its strong dual. The space F is complete, semi-barrelled and satisfies the following condition :
(DB) There exists a sequence $(A_n)_{n \in \mathbf{N}}$ of bounded subsets of F such that every bounded subset of F is contained in one of the $A_n$.

The space E is bornological (III, p. 12, prop. 2), hence its strong dual is complete (III, p. 23, cor. 1).

Let $(V_n)_{n \in \mathbf{N}}$ be a decreasing sequence of neighbourhoods of 0 in E, such that every neighbourhood of 0 in E contains one of the $V_n$. Let $A_n$ be the polar of $V_n$ in F. Since E is bornological, every bounded subset of F is equicontinuous (III, p. 22, prop. 10), therefore contained in one of the $A_n$. In other words, the space F satisfies the condition (DB).

We now show that F is semi-barrelled. Let $(U_n)_{n \in \mathbf{N}}$ be a sequence of convex, balanced and closed neighbourhoods of 0 in F. We assume that the set $U = \bigcap_n U_n$ absorbs every bounded subset of F. We shall prove that U is a neighbourhood of 0 in F. For this, we shall construct, by induction on the integer $n \geqslant 0$, real numbers $\lambda_n > 0$ and convex balanced neighbourhoods $W_n$ of 0 in F, whose which are closed for $\sigma(F, E)$, and satisfy the following relations

(1)
$$
\lambda_n A_n \subset \frac{1}{2} U \cap \left( \bigcap_{0 \leq i < n} W_i \right)
$$

(2)
$$
\bigcup_{0 \leq i \leq n} \lambda_i A_i \subset W_n \subset U_n .
$$

Suppose that the numbers $\lambda_i$ and the sets $W_i$ have been constructed for $0 \leq i < n$. By the hypothesis, the set U absorbs the bounded subsets of F; moreover, for $0 \leq i < n$, $W_i$ is a neighbourhood of 0 in F, hence absorbs the bounded subsets of F. We can therefore find a number $\lambda_n > 0$ satisfying (1). Let C denote the closed convex balanced envelope, for $\sigma(F, E)$, of $\bigcup_{0 \leq i \leq n} \lambda_i A_i$; the set C is equicontinuous, hence compact for $\sigma(F, E)$ (III, p. 17, cor. 2). Since $U_n$ is a neighbourhood of 0 in F, there exists a bounded subset B of E such that $B^\circ \subset \frac{1}{2} U_n$. Put $W_n = C + B^\circ$. Since $B^\circ$ is a neighbourhood of 0 in F, we see that $W_n$ is a convex and balanced neighbourhood of 0 in F. In addition, C is compact and $B^\circ$ closed for $\sigma(F, E)$; by cor. 1 of GT, III, § 4, No. 1, $W_n$ is closed for $\sigma(F, E)$. Finally, we have $C \subset \frac{1}{2} U \subset \frac{1}{2} U_n$ and $B^\circ \subset \frac{1}{2} U_n$, hence $W_n \subset U_n$ since $U_n$ is convex. We have thus established (2).

Put $W = \bigcap_n W_n$, then $W \subset U$. By (1) and (2), we have $\lambda_i A_i \subset W_j$ for all $i$ and $j$ in $\mathbf{N}$, and so $\lambda_i A_i \subset W$ for all $i \in \mathbf{N}$. In particular, W is absorbent, hence is a barrel for $\sigma(F, E)$. By remark 3 of IV, p. 4, W is a neighbourhood of 0 in F. A fortiori, U is a neighbourhood of 0 in F, and F is semi-barrelled.

The following corollary extends the Banach-Steinhaus theorem to the dual of a Fréchet space (*cf.* III, p. 25, cor. 2).

#### Corollary {#evt-iv-s3-n2-cor-1 .statement}

— Let G be a Hausdorff locally convex space, and let $(u_n)$ be a sequence of linear mappings from F into G, converging simply to a mapping u from F into G. Then u is continuous, and the sequence $(u_n)$ converges to u uniformly on every precompact subset of F.

Since F is complete, the set of all $u_n$, which is bounded for the topology of simple convergence, is bounded in $\mathcal{L}_b(F; G)$ (III, p. 27, cor. 1). Since the space F is semi-barrelled (prop. 2), every countable and bounded subset of $\mathcal{L}_b(F; G)$ is equicontinuous by prop. 1 of IV, p. 21. Therefore the set of the $u_n$ is equicontinuous, and the corollary follows from III, p. 18, corollary.

### 3. Bidual of a locally convex metrizable space

#### Proposition 3 {#evt-iv-s3-prop-3 .statement}

— Let E be a locally convex metrizable space, $E'_b$ its strong dual and G a Fréchet space. The space $\mathcal{L}_b(E'_b ; G)$ is a Fréchet space.

By prop. 2 (IV, p. 22), there exists a sequence $(A_n)$ of bounded subsets of $E'_b$ such that every bounded subset of $E'_b$ is contained in one of the $A_n$. Let $(V_n)$ be a countable fundamental system of neighbourhoods of 0 in G. Let $H_{mn}$ be the set of linear mappings $u$ from $E'_b$ into G such that $u(A_m) \subset V_n$. Then $(H_{mn})$ is a fundamental system of neighbourhoods of 0 in $\mathcal{L}_b(E'_b ; G)$, and the latter space is then metrizable.

To show that $\mathcal{L}_b(E'_b ; G)$ is complete, it is enough to prove that every Cauchy sequence $(u_n)$ in this space is convergent; since G is complete, there exists a linear mapping $u : E'_b \to G$ such that $(u_n)$ converges simply to u. By IV, p. 23, corollary, we have $u \in \mathcal{L}_b(E'_b ; G)$. It then follows from prop. 5 of GT, X, § 1, No. 5, that $(u_n)$ converges to u in $\mathcal{L}_b(E'_b ; G)$.

#### Corollary {#evt-iv-s3-n3-cor-1 .statement}

— The bidual of a locally convex metrizable space is a Fréchet space.

### 4. Dual of a reflexive Fréchet space

#### Proposition 4 {#evt-iv-s3-prop-4 .statement}

— Let E be a reflexive Fréchet space. The strong dual $E'_b$ of E is the inductive limit of a sequence of Banach spaces.

Let $(V_n)_{n \in \mathbf{N}}$ be a decreasing sequence of convex, balanced and closed neighbourhoods of 0 in E, such that every neighbourhood of 0 in E contains one of the $V_n$. Let $A_n$ be the polar of $V_n$ in $E'$. Then $A_n$ is convex, balanced and compact for $\sigma(E', E)$; by III, p. 8, corollary the space $E'_{A_n}$ is a Banach space. We shall prove that $E'_b$ is the inductive limit of the spaces $E'_{A_n}$; in other words, that every convex and balanced subset U of $E'$ which absorbs each of the $A_n$ is a neighbourhood of 0 in $E'_b$. For every $n \in \mathbf{N}$, choose a real number $\lambda_n > 0$ such that $\lambda_n A_n \subset U$. Let $B_n$ be the convex envelope of the set $\bigcup_{0 \leq i \leq n} \lambda_i A_i$; put $V = \bigcup_n B_n$, then $V \subset U$. For every $n \in \mathbf{N}$, the set $B_n$ is convex, balanced and compact for $\sigma(E', E)$ (II, p. 14, prop. 15).

Now we shall show that $\frac{1}{2} V^{oo} \subset V$. Let $x \in E'_b - V$; for every $n \in \mathbf{N}$, we have $x \notin B_n$, and since $B_n$ is closed for $\sigma(E', E)$ there exists an element $y_n$ in $B_n^\circ$ such that \langle y_n, x \rangle = 1 (\text{II, p. 38, prop. 4}). Since E is reflexive, every bounded subset of E is relatively compact for $\sigma(E, E')$ (IV, p. 16, th. 2). By the definition of $B_n$, we have
$$
\lambda_i y_n \in V_i \quad \text{for all } n \geq i,
$$
hence the sequence $(y_n)$ is bounded. Let $y$ be a limit point of $(y_n)$ for the topology $\sigma(E, E')$. We have $y \in V^\circ = \bigcap_n B_n^\circ$ and $\langle y, x \rangle = 1$. Hence $x \notin \frac{1}{2}V^{\circ\circ}$, and so we have the inclusion $\frac{1}{2}V^{\circ\circ} \subset V$ and *a fortiori*, $\frac{1}{2}V^{\circ\circ} \subset U$.

Since every bounded subset of $E'_b$ is contained in one of the sets $A_n$, the set $V = \bigcup_n B_n$ absorbs every bounded subset of $E'_b$. Consequently, $V^\circ$ is bounded in E, hence $\frac{1}{2}V^{\circ\circ}$ is a neighbourhood of 0 in $E'_b$. *A fortiori*, U is a neighbourhood of in $E'_b$.

#### Corollary {#evt-iv-s3-n4-cor-1 .statement}

*The strong dual of a reflexive Fréchet space is bornological and barrelled.*

An inductive limit of Banach spaces is bornological by definition. Further, a Banach space is barrelled (III, p. 25, corollary) and every inductive limit of barrelled spaces is a barrelled space (III, p. 25, cor. 3).

### 5. The topology of compact convergence on the dual of a Fréchet space

#### Theorem 1 (Banach-Dieudonné) {#evt-iv-s3-thm-1 .statement}

— *Let E be a locally convex metrizable space. The following topologies coincide on the dual $E'$ of E :*

a) *the topology $\mathcal{T}_\mathfrak{N}$ of $\mathfrak{N}$-convergence, where $\mathfrak{N}$ is the family of subsets of E each consisting of points of a sequence converging to 0 ;*
b) *the topology $\mathcal{T}_c$ of uniform convergence on compact subsets of E ;*
c) *the topology $\mathcal{T}_{pc}$ of uniform convergence on precompact subsets of E ;*
d) *the topology $\mathcal{T}_f$ which is the finest topology inducing the same topology as $\sigma(E', E)$ on every equicontinuous subset of $E'$.*

First observe that *a subset A of $E'$ is closed for $\mathcal{T}_f$ if and only if $A \cap H$ is closed for $\sigma(E', E)$ for every subset H of $E'$ which is equicontinuous and closed for $\sigma(E', E)$.* The weak topology $\sigma(E', E)$ and $\mathcal{T}_{pc}$ induce the same topology on every equicontinuous subset of $E'$ (III, p. 17, prop. 5). Consequently each of the topologies $\mathcal{T}_\mathfrak{N}$, $\mathcal{T}_c$, $\mathcal{T}_{pc}$, $\mathcal{T}_f$ is coarser than the one following it. It is therefore enough to prove that $\mathcal{T}_\mathfrak{N}$ is finer than $\mathcal{T}_f$. Moreover, every translation in $E'$ is a homeomorphism for $\mathcal{T}_f$. Hence it is enough to prove that, if F is a subset of $E'$ which is closed for $\mathcal{T}_f$, and does not contain 0, then there exists a set $S \in \mathfrak{N}$ such that $S^\circ \cap F = \varnothing$.

Let $(U_n)_{n \geq 0}$ be a decreasing sequence of neighbourhoods of 0 in E forming a fundamental system of neighbourhoods of 0. We shall construct, by induction on $n \geq 0$, *finite* sets $X_n$ such that we have
$$
X_n \subset U_n
$$
$$
\left( \bigcup_{0 \leq p \leq n} X_p \right)^\circ \cap U_{n+1}^\circ \cap F = \varnothing
$$

for every integer $n \geqslant 0$. Let $m \geqslant 0$ be an integer such that $X_n$ has been constructed for $0 \leqslant n < m$ and satisfies (4) and (5) for $0 \leqslant n < m$. For every $x \in U_m$, put
$$
F_x = (\bigcup_{0 \leqslant p < m} X_p)^{\circ} \cap \{x\}^{\circ} \cap U_{m+1}^{\circ} \cap F.
$$
Formula (5) with $n = m - 1$ implies that $\bigcap_{x \in U_m} F_x = \varnothing$. Further, the set $U_{m+1}^{\circ}$ is equicontinuous, and compact for $\sigma(E', E)$. In view of the definition of $\mathcal{T}_f$, each of the sets $F_x$ is compact for $\sigma(E', E)$; therefore there exists a finite subset $X_m$ of $U_m$ such that $\bigcap_{x \in X_m} F_x = \varnothing$, *i.e.* relation (5) is satisfied for $n = m$.

Put $S = \bigcup_{n \geqslant 0} X_n$. We have $X_n \subset U_p$ for $n \geqslant p$, therefore $S$ is the set of points of a sequence which converges to 0 in $E$. From (5) we deduce that $S^{\circ} \cap U_{n+1}^{\circ} \cap F = \varnothing$, and since $E'$ is the union of the sequence of sets $U_{n+1}^{\circ}$, we get $S^{\circ} \cap F = \varnothing$.

#### Corollary 1 {#evt-iv-s3-thm-1-cor-1 .statement}

*Let $E$ be a locally convex metrizable space. Every precompact subset of $E$ is contained in the closed convex balanced envelope of the set of points of a sequence converging to 0.*

This follows from the fact that the topologies $\mathcal{T}_{pc}$ and $\mathcal{T}_{\mathfrak{H}}$ are identical, on account of prop. 2 of III, p. 15.

#### Corollary 2 {#evt-iv-s3-thm-1-cor-2 .statement}

*Let $E$ be a Fréchet space. In order that a convex subset $A$ of the dual $E'$ of $E$ be closed for $\sigma(E', E)$, it is necessary and sufficient that $A \cap U^{\circ}$ is closed for $\sigma(E', E)$ for every neighbourhood $U$ of 0 in $E$.*

Since $E$ is complete, the topology $\mathcal{T}_c$ on $E'$ is compatible with the duality between $E'$ and $E$ (IV, p. 3, *Example*); consequently the closed convex subsets in $E'$ are the same for $\mathcal{T}_c$ and $\sigma(E', E)$ (IV, p. 1, prop. 1). The corollary then follows from the identity of the topologies $\mathcal{T}_c$ and $\mathcal{T}_f$.

Recall (I, p. 13) that the hyperplanes of $E'$ which are closed for $\sigma(E', E)$ are the kernels of linear forms on $E'$ associated with elements of $E$. Cor. 2 therefore gives another proof (for Fréchet spaces) of cor. 1 of III, p. 21.

#### Corollary 3 {#evt-iv-s3-thm-1-cor-3 .statement}

*Let $E$ be a Banach space and $M$ a vector subspace of the dual $E'$ of $E$. In order that $M$ be closed for the weak topology $\sigma(E', E)$, it is necessary and sufficient that its intersection with the unit ball (closed) in $E'$ be closed for $\sigma(E', E)$.*

#### Example {#evt-iv-s3-n5-exa-1 .statement}

— *Let $H$ be a hilbertian space satisfying the first axiom of countability; let $H_{\sigma}$ denote the space $H$ with the weakened topology assigned to it. Let $\mathcal{L}^1(H)$ be the Banach space of nuclear endomorphisms of $H$ (V, p. 51, and TS, V); the norm in $\mathcal{L}^1(H)$ is defined by $\|u\|_1 = \operatorname{Tr}((u^*u)^{1/2})$. We can identify $\mathcal{L}(H)$ with the dual of the Banach space $\mathcal{L}^1(H)$ by associating the linear form $\phi_u : v \mapsto \operatorname{Tr}(uv)$ on $\mathcal{L}^1(H)$ with every $u \in \mathcal{L}(H)$. Let $A$ be a sub-algebra of $\mathcal{L}(H)$, containing 1 and stable under $u \mapsto u^*$; this is a von Neumann algebra if and only if it is closed in $\mathcal{L}(H)$ for the weak topology $\sigma(\mathcal{L}(H), \mathcal{L}^1(H))$. From cor. 3, we deduce the following criterion : *for $A$ to be a von Neumann algebra, it is necessary and sufficient that if $(u_n)$ is any sequence of elements of $A$ with norm $\leqslant 1$ having a limit $u$ in the space $\mathcal{L}_s(H ; H_{\sigma})$, then $u$ belongs to $A$.*

### 6. Separately continuous bilinear mappings

#### Lemma 1 {#evt-iv-s3-lem-1 .statement}

Let E and F be two locally convex metrizable spaces, and u be a continuous linear mapping from $E'_b$ into F. Then there exists a neighbourhood U of 0 in $E'_b$ whose image under u is bounded in F.

Let $(U_n)_{n \in \mathbf{N}}$ (resp. $(V_n)_{n \in \mathbf{N}}$) be a fundamental system of neighbourhoods of 0 in E (resp. F). We assume that the sets $U_n$ are balanced and form a decreasing sequence. Since u is continuous, for every $n \in \mathbf{N}$, there exists a bounded set $B_n$ in E such that $u(B_n^\circ) \subset V_n$. Since $B_n$ is bounded, there exists a real number $\lambda_n > 0$ such that $\lambda_n B_n \subset U_n$. Put $B = \bigcup_{n \in \mathbf{N}} \lambda_n B_n$.

We shall prove that the set B is bounded in E, in other words that for every integer $m \geqslant 0$, there exists a real number $\mu > 0$ such that $\mu B \subset U_m$. Since the sets $B_n$ are bounded, there exists a real number $\mu$ such that $0 < \mu \leqslant 1$ and such that $\mu (\lambda_n B_n) \subset U_m$ for $0 \leqslant n \leqslant m$; we have also $\lambda_n B_n \subset U_n \subset U_m$ if $n > m$; hence $\mu B \subset U_m$ since $U_m$ is balanced.

Let U be the polar of B in $E'_b$. This is a neighbourhood of 0 in $E'_b$ and we have $\lambda_n B^\circ \subset B_n^\circ$, hence $\lambda_n u(U) \subset V_n$ for all $n \in \mathbf{N}$. Consequently $u(U)$ is bounded in F.

#### Theorem 2 {#evt-iv-s3-thm-2 .statement}

Let $E_1$ and $E_2$ be two reflexive Fréchet spaces, and G a locally convex Hausdorff space. For $i = 1, 2$, let $F_i$ be the strong dual of $E_i$. Then every separately continuous bilinear mapping $u : F_1 \times F_2 \to G$ is continuous.

The space G is isomorphic to a subspace of a product of Banach spaces (II, p. 5, prop. 3). Therefore it is enough to prove the theorem under the additional hypothesis that G is a Banach space. But $F_1$ is barrelled and $F_2$ bornological (IV, p. 24, corollary), and $\mathscr{L}_b(F_2 ; G)$ is a Fréchet space (IV, p. 23, prop. 3). Let v denote the linear mapping from $F_1$ into $\mathscr{L}_b(F_2 , G)$ associated with u by the relation

$$
u(x_1, x_2) = v(x_1)(x_2) \quad (x_1 \in F_1, x_2 \in F_2).
$$

Since $F_1$ is barrelled and u separately continuous, v is continuous (III, p. 31, prop. 6).

Since v is continuous, lemma 1 implies the existence of a neighbourhood $U_1$ of 0 in $F_1$ whose image under v is bounded in $\mathscr{L}_b(F_2 ; G)$. In other words, for every bounded subset $B_2$ in $F_2$, the set $u(U_1 \times B_2)$ is bounded in the Banach space G. Let $U_2$ be the set of all $x_2 \in F_2$ such that $\|u(x_1, x_2)\| \leqslant 1$ for all $x_1 \in U_1$. The set $U_2$ then absorbs every bounded subset; since $F_2$ is bornological, $U_2$ is a neighbourhood of 0 in $F_2$, and this proves that u is continuous.

### Exercises {#evt-iv-s3-exercises}

**T 1**) Let $E$ be a locally convex metrizable space, and $E'_b$ its strong dual. If $E'_b$ is metrizable, prove that the topology of $E$ can be defined by a single norm (use III, p. 37, exerc. 2 and p. 38, exerc. 5 and also the fact that $E$ is bornological).

**T 2**) An infra-barrelled space is semi-barrelled. A locally convex space is said to be a (DF) *space* if it is semi-barrelled and if the canonical bornology (III, p. 3, def. 5) has a countable base. Every normed space and every strict inductive limit of a sequence of normed spaces (II, p. 33) is a (DF) space. Every strong dual of a Fréchet space is a (DF) space.
*a*) The strong dual of a (DF) space is a Fréchet space.
*b*) Let $E$ be a (DF) space and let $(A_n)$ be an increasing sequence of bounded, convex, balanced and closed subsets of $E$ such that every bounded subset of $E$ is absorbed by one of the $A_n$.

Let U be the union of the $A_n$; show that the closure $\overline{U}$ of U in E is precisely the set of all $x \in E$ such that $\lambda x \in U$ for $0 \leq \lambda < 1$. (If $x \notin \lambda U$ for some $\lambda > 1$, then for every $n$, there exists a linear form $x'_n \in E'$ such that $x'_n \in A_n^\circ$ and $\langle x, x'_n \rangle = \lambda$, and the sequence $(x'_n)$ is equicontinuous, hence has a weak limit point.)
c) Show that if a (DF) space is barrelled, it is also bornological ($cf.$ III, p. 44, exerc. 13, b)). Give examples of (DF) spaces which are not ultrabornological, but are bornological and barrelled (III, p. 46, exerc. 22) and also of (DF) spaces which are not barrelled but are bornological.

¶ 3) Let E be a locally convex metrizable space, and $E'_b$ its strong dual.
a) Show that every convex balanced subset $V'$ of $E'_b$ which absorbs the strongly bounded subsets of $E'_b$ contains a barrel (for the strong topology) which absorbs the strongly bounded subsets of $E'_b$. (Let $(K'_n)$ be a countable base of the canonical bornology of $E'_b$ and let $\lambda_n$ be such that $\lambda_n K'_n \subset \frac{1}{2}V'$; apply exerc. 2, b) to the sequence $A'_n$, where $A'_n$ is the convex envelope of the union of the $\lambda_j K'_j$ for $j \leq n$.)
b) Deduce from a) that the following properties are equivalent :
$\alpha)$ E is distinguished (IV, p. 52, exerc. 4).
$\beta)$ $E'_b$ is infrabarrelled (III, p. 44, exerc. 7).
$\gamma)$ $E'_b$ is bornological.
$\delta)$ $E'_b$ is barrelled.
$\varepsilon)$ $E'_b$ is ultrabornological (III, p. 45, exerc. 19).
c) Show that if $E'_b$ is reflexive, then $\hat{E} = E''$ (which is obviously reflexive) ($cf.$ IV, p. 52, exerc. 4 and p. 53, exerc. 11).

4) Let E be a locally convex Hausdorff space, E' its dual. If M is a closed vector subspace of E which is metrizable and distinguished (IV, p. 52, exerc. 4), then the strong topology $\beta(E'/M^\circ, M)$ is the quotient topology by $M^\circ$ of the strong topology $\beta(E', E)$ (use exerc. 3, b) and IV, p. 51, exerc. 22, b)).

¶ 5) For every integer $n > 0$, let $a^{(n)}$ be the double sequence $(a_{pq}^{(n)})$ ($p \in \mathbf{N}, q \in \mathbf{N}$) such that $a_{pq}^{(n)} = q$ if $p \leq n$ and $a_{pq}^{(n)} = 1$ if $p > n$. Let E be the vector space of all double sequences $x = (x_{pq})_{(p,q) \in \mathbf{N} \times \mathbf{N}}$ of real numbers such that, for every integer $n > 0$, the number $r_n(x) = \sum_{p,q} a_{pq}^{(n)} |x_{pq}|$ is finite. If E is assigned the topology defined by the semi-norms $r_n$, then E is a Fréchet space satisfying the first axiom of countability (IV, p. 47, exerc. 1, c)); the dual E' of E can be identified with the space of all double sequences $x' = (x'_{pq})$ of real numbers such that for at least one index $n$, there exists $k_n > 0$ such that $|x'_{pq}| \leq k_n a_{pq}^{(n)}$ for every pair $(p, q)$; and $\langle x, x' \rangle = \sum_{p,q} x_{pq} x'_{pq}$ (IV, p. 47, exerc. 1, c)).
For every integer $p_0 > 0$ and every sequence $(m_p)$ of integers $> 0$, let $J(p_0; (m_p))$ be the set of pairs of integers $p > 0, q > 0$ such that $p \geq p_0$ and $q \geq m_p$; let $\mathcal{B}$ be the filter base on $\mathbf{N} \times \mathbf{N}$ consisting of the sets $J(p_0; (m_p))$ and let $\mathfrak{F}$ be an ultrafilter which is finer than the filter with base $\mathcal{B}$.
a) Show that for all $x' = (x'_{pq}) \in E'$, the double sequence $(x'_{pq})$ has a limit $u(x')$ with respect to the ultrafilter $\mathfrak{F}$; if $V_n$ is a neighbourhood of 0 in E defined by $r_n(x) \leq 1$, then $|u(x')| \leq 1$ for all $x' \in V_n^\circ$.
b) Let $U'$ be a neighbourhood of 0 in $E'$, for the strong topology, which is convex, balanced and weakly closed, and for every $n$, let $\alpha_n > 0$ be such that $\alpha_n V_n^\circ \subset U'$. For every integer $p > 0$, let $m_p$ be an integer such that $2^{p+1} \leq \alpha_p m_p$, and let $x' = (x'_{pq})$ be the double sequence with $x'_{pq} = 0$ for $q < m_p$, $x'_{pq} = 2$ for $q \geq m_p$. Show that $x' \in U'$ but that $u(x') = 2$; deduce that $u$ is not strongly continuous in $E'$, while being bounded on every bounded subset of $E'$. Conclude (IV, p. 58, exerc. 3) that E is not distinguished, and consequently that the strong dual $E'_b$ is a non infra-barrelled (DF) space.
c) Using b) construct an example of a closed subspace M of a Fréchet space F such that the strong topology $\beta(F'/M^\circ, M)$ is distinct from the quotient topology by $M^\circ$ of the strong topology $\beta(F', F)$ (embed E in a countable product of Banach spaces).

**T 6) a)** Let E be a (DF) space (IV, p. 57, exerc. 2), and let U be a convex set such that for every bounded, convex and balanced subset A of E, $U \cap A$ is a neighbourhood of 0 for the topology induced on A by that of E. Show that U is a neighbourhood of 0 in A. (Let $(A_n)$ be a countable base for the canonical bornology of E (III, p. 3, def. 5). Show that, by induction we can define a sequence $(\lambda_n)$ of numbers $> 0$ and a sequence $(V_n)$ of closed, convex and balanced neighbourhoods of 0 in E such that $\lambda_n A_n \subset \frac{1}{3} U, \lambda_n A_n \subset \bigcap_{j=1}^\infty V_j, V_n \cap A_n \subset U$ for every $n$.

First show that if $\lambda_j$ and $V_j$ have been constructed for $j \leq n$, then we can find $\lambda_{n+1}$ such that $\lambda_{n+1} A_{n+1} \subset \frac{1}{3} U$ and $\lambda_{n+1} A_{n+1} \subset V_j$ for $j \leq n$. Next prove that we can find $V_{n+1}$ such that $\lambda_j A_j \subset V_{n+1}$ for $j \leq n + 1$ and $V_{n+1} \cap A_{n+1} \subset U$; for this, letting A denote the convex envelope of the $\lambda_j A_j$ for $j \leq n + 1$, show that we can take $V_{n+1} = \overline{A + V}$ for a suitable convex balanced neighbourhood V of 0; we remark that for this it is enough to show that, if $B = A_{n+1} \cap \complement U$, then 0 is not in the closure of the set $B + 2A$.
$b)$ Deduce from $a)$ that if $u$ is a linear mapping from E into a locally convex space F, such that the restriction of $u$ to every bounded subset of E is continuous, then $u$ is continuous ($cf.$ IV, p. 50, exerc. 15).

**T 7) a)** Let E be a (DF) space, U a convex, balanced and closed set in E, which absorbs the bounded subsets of E, and let $(x_n)$ be a sequence of points of $\complement U$. Show that there exists a neighbourhood V of 0 in E which does not contain any of the $x_n$. (Let $(A_n)$ be a countable base for the canonical bornology of E. Show that, by induction we can define a sequence $(\lambda_n)$ of numbers $> 0$ and a sequence $(V_n)$ of convex, balanced and closed neighbourhoods of 0 such that $\lambda_n A_n \subset \bigcap_{j=1}^\infty V_j, \lambda_n A_n \subset U$ and $x_n \in \complement V_n$ for all $n$. For this, if the $\lambda_j$ and $V_j$ have been constructed for $j \leq n$, take $\lambda_{n+1}$ such that $\lambda_{n+1} A_{n+1} \subset U$ and $\lambda_{n+1} A_{n+1} \subset V_j$ for all $j \leq n$, then take $V_{n+1}$ containing the closure of the convex envelope of the union of the $\lambda_j A_j$ for $j \leq n + 1$.
$b)$ Deduce from $a)$ that if M is a subset of E containing an everywhere dense countable set, then the topology induced on M by the strong topology of the bidual $E''$ of E is identical with the topology induced by that of E. In particular, the convergent sequences in E are the same for the topology of E and for the topology induced by the strong topology of $E''$; for every metrizable subset M of E, the topology induced on M by the topology of E is identical with the topology induced by the strong topology of $E''$.
$c)$ Deduce from $a)$ that if there exists a countable everywhere dense set in E, then E is infra-barrelled.
$d)$ Deduce from $b)$ and from exerc. 6 that if every bounded subset of E is metrizable for the topology induced by that of E, then E is infrabarrelled.

**T 8) Let E be a Fréchet space, $E'_b$ its strong dual. Suppose that there exists an everywhere dense sequence $(x'_n)$ in $E'_b$. Show that E satisfies the first axiom of countability. (Let $(K'_n)$ be a countable base for the canonical bornology of $E'_b$ consisting of closed convex balanced sets. For every system $\alpha$ consisting of a point $x'_n$, an arbitrary finite number of rational numbers $\lambda_k > 0 (1 \leq k \leq m)$ and m indices $n_k$ such that $x'_n \notin 2 \sum_{k=1}^m \lambda_k K'_{n_k} = 2H'_\alpha$, let $x_\alpha \in E$ be such that the hyperplane with equation $\langle x_\alpha, y' \rangle = 1$ strictly separates the two weakly compact sets $H'_\alpha$ and $x'_n + H'_\alpha$. Show that for every $x' \neq 0$ in $E'$, there exists a system $\alpha$ such that $\langle x_\alpha, x' \rangle \neq 0$. For this, consider a neighbourhood V' of 0 in $E'_b$ such that $V' \cap (x' + V') = \varnothing$, then for each integer $m$, take a rational number $\lambda_m > 0$ such that $\lambda_m K'_m \subset V'$; use the fact that the union $U' \subset V'$ of the $\lambda_m K'_m$ is a neighbourhood of 0 (exerc. 7, and IV, p. 58, exerc. 3, $b$)) and that there exists $n$ such that $x'_n \in x' + U'$.)

**T 9) a)** Let E be a Hausdorff semi-barrelled space, M a closed vector subspace of E and $E'$ the dual of E. Show that $E/M$ is semi-barrelled and that the strong topology $\beta(M^\circ, E/M)$ is identical with the topology induced on $M^\circ$ by the strong topology $\beta(E', E)$. (Note that it is enough to prove that a sequence $(x'_n)$ in $M^\circ$ which converges to 0 for $\beta(E', E)$ is bounded for $\beta(M^\circ, E/M)$.) Deduce that if E is a (DF) space, then so is $E/M$ ($cf.$ IV, p. 63, exerc. 8).

b) Let E be a locally convex Hausdorff space, M a (not-necessarily closed) vector subspace of E. Show that if M is a semi-barrelled space, then the strong topology $\beta(E'/M^\circ, M)$ is identical with the quotient topology by $M^\circ$ of the strong topology $\beta(E', E)$. (Argue as in a.)
c) Show that a Hausdorff and quasi-complete semi-barrelled space E is complete (use b) applied to E and $\hat{E}$). In particular, a semi-barrelled, semi-reflexive space is complete (*cf.* IV, p. 52, exerc. 6).
d) Show that the completion of a semi-barrelled (resp. (DF)) Hausdorff space is semi-barrelled (resp. a (DF) space).
e) Let $(E_n)$ be a sequence of semi-barrelled (resp. (DF)) spaces, E a vector space, and for each n, let $f_n$ be a linear mapping from $E_n$ into E. Suppose that E is the union of the $f_n(E_n)$; show that, E is semi-barrelled (resp. a (DF) space) for the finest locally convex topology for which all the $f_n$ are continuous (first examine the case where E is the topological direct sum of the $E_n$). If the $E_n$ are semi-reflexive (resp. reflexive) and if E is Hausdorff, then E is semi-reflexive (resp. reflexive).

10) Let E be a Fréchet space satisfying the first axiom of countability. Show that if in the dual $E'$ of E, every sequence which converges for the weak topology $\sigma(E', E)$ also converges for the strong topology $\beta(E', E)$, then E is a Montel space. (Show that every bounded subset of $E'$ is relatively compact for the strong topology; use GT, II, § 4, exerc. 6; then use IV, p. 53, exerc. 11, b).)

11) Let $(c_{mn})$ be a double sequence of numbers $> 0$ such that $c_{m,n} \leq c_{m+1,n}$ and let E be the space of all sequences $x = (x_n)$ of real numbers such that $p_m(x) = \sum_n c_{mn} |x_n| < +\infty$ for every integer m. We endow E with the topology defined by the semi-norms $p_m$ and for this topology E is a Fréchet space satisfying the first axiom of countability; the dual $E'$ of E can be identified with the space of all sequences $x' = (x'_n)$ such that $\sup_n c_{mn}^{-1} |x'_n| < +\infty$ for at least one m, the canonical bilinear form $\langle x, x' \rangle$ being identified with $\sum_n x_n x'_n$ (IV, p. 47, exerc. 1, c)). Suppose that there does not exist any subsequence $(n_k)$ for which there is a sequence $(a_m)$ of numbers $\geq 0$ and an index $m_0$ such that $c_{m,n_k} \leq a_m c_{m_0,n_k}$ for all $m \geq m_0$ and for all k. Under these conditions, every weakly convergent sequence in $E'$ is strongly convergent and consequently (IV, p. 60, exerc. 10) E is a Montel space. (Argue by *reductio ad absurdum*; if necessary make a transformation of the form $(x_n) \mapsto (a_n x_n)$ to reduce to the case where $c_{m_0 n} = 1$ for all n and some $m_0$, and where there exists a sequence $(x^{(p)})_{p \geq 0}$ which converges weakly to 0 in E', and is such that $|x^{(p)}_n| \leq 1$ for every pair $(p, n)$, and also that there exists a bounded set B in E, defined by $p_m(x) \leq b_m$ for all $m \geq 0$ and such that $\sup_{x \in B} |\langle x, x^{(p)} \rangle| \geq 2\delta > 0$ for every integer p. Under these hypothesis, prove that there exists a strictly increasing sequence $(r_q)$ of integers, and a sequence $(x^{(q)})$ of points of B such that

$$
\sum_{k=r_q+1}^{r_q+1} |x^{(q)}_k| > \delta
$$

for each index q. Then show, by *reductio ad absurdum*, that for every q, there exists at least one index $s_q$ such that $r_q < s_q \leq r_{q+1}$ and that for every integer m, we have $c_{m,s_q} \leq b_m 2^{m+2}/\delta$, which contradicts the hypothesis.)

12) a) Let F be a Hausdorff (DF) space, and $F'_b$ its strong dual. Show that if $F'_b$ is reflexive, then the completion $\hat{F}$ of F is reflexive and is equal to the bidual $F''$ of F (*cf.* IV, p. 52, exerc. 4 and p. 53, exerc. 11).
b) Let E be a Fréchet space. Show that if the bidual $E''$ of E is reflexive, then E is reflexive.

13) a) Let E, F be two Fréchet spaces, G a locally convex Hausdorff space and E', F', G' the duals of E, F, G respectively. Let $u$ be a bilinear mapping from $E' \times F'$ into $G'$, which is separately continuous (III, p. 28) when E', F', G' are assigned the weak topologies $\sigma(E', E)$, $\sigma(F', F)$ and $\sigma(G', G)$. Show that under these conditions, $u$ is a continuous mapping from $E' \times F'$ into $G'$ when E', F' and G' are assigned the strong topologies. (For $z \in G$, put \langle z, u(x', y') \rangle = \langle v_z(x'), y' \rangle \text{ where } v_z(x') \in F. \text{ First show that if } E' \text{ is assigned the strong topology and } F \text{ the initial topology, then the set of all } v_z, \text{ as } z \text{ ranges over a bounded set } C \text{ in } G, \text{ is equicontinuous; for this use IV, p. 51, exerc. 19, } d). \text{ Next show that there exists a neighbourhood } V' \text{ of } 0 \text{ for the strong topology of } E' \text{ such that the union of the sets } v_z(V') \text{ as } z \text{ ranges over } C \text{ is bounded in } F; \text{ for this use III, p. 47, exerc. 5.)}
b) Give an example to show that the conclusion of $a)$ does not hold if we assume that $E$ is a Fréchet space and $F$ a strict inductive limit of Fréchet spaces (III, p. 47, exerc. 3).

14) $a)$ Let $E$ be a Fréchet space, $E'$ its dual. Show that $E'$, endowed with the topology of compact convergence or with a finer $\mathcal{S}$-topology, is complete ($cf.$ III, p. 22, *Remark* 1). If $E$ is not reflexive, show that $E'$ is not infrabarrelled for any $\mathcal{S}$-topology which is finer than the topology of compact convergence and coarser than $\tau(E', E)$.
$b)$ Let $(E_\alpha)_{\alpha \in A}$ be a family of Fréchet spaces, $E$ a vector space and for every $\alpha \in A$, let $h_\alpha$ be a linear mapping from $E_\alpha$ into $E$. Suppose that $E$, endowed with the finest locally convex topology for which the $h_\alpha$ are continuous (II, p. 27) is Hausdorff. Prove that the dual $E'$ of $E$, endowed with the topology of compact convergence or with any finer $\mathcal{S}$-topology, is complete ($cf.$ III, p. 20, th.

See the [exercises for § 3](exercises/s3/).
