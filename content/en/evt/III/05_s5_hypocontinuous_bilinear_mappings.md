---
book: evt
book_title: Topological Vector Spaces
chapter: III
chapter_title: SPACES OF CONTINUOUS LINEAR MAPPINGS
section: 5
section_title: Hypocontinuous bilinear mappings
lang: en
source: evt-i-v
book_pages: TVS III.28-TVS III.33, TVS III.46-TVS III.49
pdf_pages: 0160-0165, 0178-0181
extraction: ocr
subsections:
    - "no": 1
      title: Separately continuous bilinear mappings
      page: 28
      pdf_page: 160
    - "no": 2
      title: Separately continuous bilinear mappings on a product of Fréchet spaces
      page: 29
      pdf_page: 161
    - "no": 3
      title: Hypocontinuous bilinear mappings
      page: 30
      pdf_page: 162
    - "no": 4
      title: Extension of a hypocontinuous bilinear mapping
      page: 32
      pdf_page: 164
    - "no": 5
      title: Hypocontinuity of the mapping $(u, v) \mapsto v \circ u$
      page: 32
      pdf_page: 164
statements: 11
exercises: 15
content_sha256: 4245718f16c815b97502b1ac288429946f7e3f9aa3b5136610d10239abd53e48
---

## § 5. HYPOCONTINUOUS BILINEAR MAPPINGS

### 1. Separately continuous bilinear mappings

Let $ E, F, G $ be three locally convex spaces. For every bilinear mapping $ u $ from $ E \times F $ into $ G $, and for every $ x \in E $ (resp. $ y \in F $), we denote by $ u(x, .) $ (resp. $ u(., y) $) the mapping $ y \mapsto u(x, y) $ (resp. $ x \mapsto u(x, y) $) from $ F $ into $ G $ (resp. from $ E $ into $ G $).

Definition 1. — *A bilinear mapping $ u $ from $ E \times F $ into $ G $ is said to be separately continuous if, for all $ x \in E $, the linear mapping $ u(x, .) $ from $ F $ into $ G $ is continuous, and for all $ y \in F $, the linear mapping $ u(., y) $ from $ E $ into $ G $ is continuous.*

The following proposition follows immediately from the definition.

Proposition 1. — *For a bilinear mapping $ u $ from $ E \times F $ into $ G $ to be separately continuous, it is necessary and sufficient that for all $ y \in F $, the linear mapping $ u(., y) $ from $ E $ into $ G $ is continuous and that the linear mapping $ y \mapsto u(., y) $ from $ F $ into $ \mathcal{L}_s(E; G) $ is continuous.*

We can also say that, to every linear mapping $ v \in \mathcal{L}(F; \mathcal{L}_s(E; G)) $ is associated the bilinear mapping $ (x, y) \mapsto v(y)(x) $, then we define a linear *bijection* from $ \mathcal{L}(F; \mathcal{L}_s(E; G)) $ onto the vector space of separately continuous bilinear mappings from $ E \times F $ into $ G $.

A separately continuous bilinear mapping from $ E \times F $ into $ G $ need not necessarily be continuous on $ E \times F $ (III, p. 47, exerc. 2; cf. however III, p. 30, and IV, p. 26, th. 2).

The notion of a separately continuous bilinear *form* on a product $ E_1 \times E_2 $ of two locally convex spaces is directly related to that of a continuous linear mapping when $ E_1 $ and $ E_2 $ are assigned the *weak* topologies (II, p. 42), Suppose that $ (E_1, F_1) $ and $ (E_2, F_2) $ are two pairs of real (resp. complex) vector spaces in separating duality (*loc. cit.*); we assign to $ E_i $ (resp. $ F_i $) the weak topology $ \sigma(E_i, F_i) $ (resp. $ \sigma(F_i, E_i) $) for $ i = 1, 2 $, and denote by $ B(E_1, E_2) $ the vector space of separately *continuous* bilinear forms on $ E_1 \times E_2 $. Applying prop. 1 to the case when $ G = K $, we see that, for every bilinear form $ \Phi \in B(E_1, E_2) $ and every $ x_2 \in E_2 $, the mapping $ x_1 \mapsto \Phi(x_1, x_2) $ is a continuous linear form on $ E_1 $, hence (II, p. 43, prop. 3) there exists one element, and only one $ ^d\Phi(x_2) \in F_1 $ such that

$$
\Phi(x_1, x_2) = \langle x_1, ^d\Phi(x_2) \rangle
$$

for every $ x_1 \in E_1 $ and $ x_2 \in E_2 $; moreover, the mapping $ ^d\Phi : E_2 \to F_1 $ is linear and *continuous* for the (weak) topologies of $ E_2 $ and of $ F_1 $.

Conversely, for every continuous linear mapping $ u : E_2 \to F_1 $ the mapping $(x_1, x_2) \mapsto \Phi(x_1, x_2) = \langle x_1, u(x_2) \rangle$ is a separately continuous bilinear form on $E_1 \times E_2$, and we have $u = {}^d \Phi$. Thus we have defined an isomorphism $d : \Phi \mapsto {}^d \Phi$ from $B(E_1, E_2)$ onto $\mathcal{L}(E_2; F_1)$, said to be *canonical*. Similarly the formula

$$
\Phi(x_1, x_2) = \langle {}^s \Phi(x_1), x_2 \rangle
$$

defines a *canonical* isomorphism $s : \Phi \to {}^s \Phi$ from $B(E_1, E_2)$ onto $\mathcal{L}(E_1, F_2)$; we have evidently the commutative diagram

$$
\begin{array}{ccc}
& B(E_1, E_2) & \\
s & / & d \\
\downarrow & & \downarrow \\
\mathcal{L}(E_1; F_2) & \leftrightarrow & \mathcal{L}(E_2; F_1)
\end{array}
$$

where $t$ is the isomorphism of transposition (II, p. 46, prop. 5 and corollary). In view of the definition of weak topologies on $F_1$ and $F_2$, it is immediate that when $B(E_1, E_2)$, $\mathcal{L}(E_1; E_2)$ and $\mathcal{L}(E_2; F_1)$ are assigned *the topology of simple convergence*, *the isomorphisms of diagram (3) are topological vector space isomorphisms*.

### 2. Separately continuous bilinear mappings on a product of Fréchet spaces

#### Proposition 2 {#evt-iii-s5-prop-2 .statement}

*Let E, F and G be three locally convex spaces. Suppose that E and F are metrizable and E is barrelled. Let H be a set of separately continuous bilinear mappings from E × F into G. Suppose that for every $x \in E$, the set of mappings $u(x, .)$ from F into G, where u runs through H, is equicontinuous. Then H is equicontinuous.*

Let $U_n$ (resp. $V_n$) be a fundamental sequence of neighbourhoods of 0 in E (resp. F). If H is not equicontinuous, there exists a closed, convex, balanced neighbourhood W of 0 in G such that for all $n$, $H(U_n \times V_n)$ is not contained in W. There exists then a sequence of pairs $(x_n, y_n) \in U_n \times V_n$, and a sequence $(u_n)$ of elements of H, such that $u_n(x_n, y_n) \notin W$. Let $p$ be the gauge of W. For every $y \in F$ and every $u \in H$, the mapping $u(., y)$ from E into G is continuous, hence $p \circ u(., y)$ is a continuous semi-norm on E. On the other hand, for every $x \in E$, the set of mappings $u(x, .)$ for $u \in H$ is equicontinuous; since the sequence $(y_n)$ tends to 0, it is bounded, and the set of all $u(x, y_n)$, for $n \geq 0$ and $u \in H$, is bounded (III, p. 22, prop. 9). It follows from this that the function $p'(x) = \sup_{\substack{u \in H \\ n \geq 0}} p(u(x, y_n))$ is a lower semi-continuous semi-norm (finite) on E. Since E is barrelled, $p'$ is continuous (III, p. 24, corollary). Since $(x_n)$ tends to 0 in E, $p'(x_n)$ tends to 0, so that we have $p'(x_n) \leq 1$ if $n$ is large enough; but then $p(u_n(x_n, y_n)) \leq p'(x_n) \leq 1$, hence $u_n(x_n, y_n) \in W$, which contradicts the hypothesis on $u_n, x_n, y_n$.

#### Corollary 1 {#evt-iii-s5-prop-2-cor-1 .statement}

— Let E and F be two Fréchet spaces, and G a locally convex space. Every separately continuous bilinear mapping from $ E \times F $ into G is continuous.

In fact, every Fréchet space is barrelled (III, p. 25, corollary).

Let E and F be two locally convex spaces. We use $ \mathcal{B}(E, F) $ to denote the space of continuous bilinear forms on $ E \times F $, with the topology of uniform convergence on sets of the form $ A \times B $, where A (resp. B) is bounded in E (resp. F). The formula
$$
u(x, y) = \langle y, \phi(u)(x) \rangle
$$
(for $ x \in E, y \in F $ and $ u \in \mathcal{B}(E, F) $) defines a continuous linear injective mapping $ \phi $ from $ \mathcal{B}(E, F) $ into $ \mathcal{L}_b(E; F'_b) $.

#### Corollary 2 {#evt-iii-s5-prop-2-cor-2 .statement}

— Suppose that E and F are metrizable and that E is barrelled. Then $ \phi $ is a topological vector space isomorphism from $ \mathcal{B}(E, F) $ onto $ \mathcal{L}_b(E; F'_b) $.

Let $ f \in \mathcal{L}_b(E; F'_b) $. Put $ u(x, y) = \langle y, f(x) \rangle $ for $ x \in E $ and $ y \in F $. The bilinear form $ u $ on $ E \times F $ is separately continuous; by prop. 2, it belongs to $ \mathcal{B}(E, F) $, and we have $ f = \phi(u) $. Hence $ \phi $ is a linear bijection from $ \mathcal{B}(E, F) $ onto $ \mathcal{L}_b(E; F'_b) $. It is immediate that $ \phi $ is bicontinuous, hence cor. 2 follows.

### 3. Hypocontinuous bilinear mappings

In what follows, we shall define a notion which is intermediate between that of a continuous bilinear mapping and that of a separately continuous bilinear mapping.

#### Proposition 3 {#evt-iii-s5-prop-3 .statement}

— Let E, F, G be three locally convex spaces, $ \mathfrak{S} $ a family of bounded subsets of E. Let u be a separately continuous bilinear mapping from $ E \times F $ into G. The following properties are equivalent :

a) For every neighbourhood W of 0 in G and every set $ M \in \mathfrak{S} $, there exists a neighbourhood V of 0 in F such that $ u(M \times V) \subset W $.

b) For every set $ M \in \mathfrak{S} $, the image of M under the mapping $ x \mapsto u(x, .) $ is an equicontinuous subset of $ \mathcal{L}(F; G) $.

c) The mapping $ y \mapsto u(., y) $ from F into $ \mathcal{L}_{\mathfrak{S}}(E; G) $ is continuous.

a) expresses that $ y \mapsto u(., y) $ is continuous at the point 0, on account of the definition of neighbourhoods of 0 in $ \mathcal{L}_{\mathfrak{S}}(E; G) $ (III, p. 13); likewise a) expresses that the image of M under the mapping $ x \mapsto u(x, .) $ is equicontinuous at the point 0 (III, p. 16).

#### Definition 2 {#evt-iii-s5-def-2 .statement}

— Let u be a bilinear mapping from $ E \times F $ into G. We say that u is $ \mathfrak{S}$-hypocontinuous if u is separately continuous and if it verifies one of the equivalent conditions a), b), c) of prop. 3.

The condition c) of prop. 3 shows that the notion of $ \mathfrak{S}$-hypocontinuous bilinear mapping depends on $ \mathfrak{S} $ only through the $ \mathfrak{S} $-topology on $ \mathcal{L}(E, G) $.

For every set $ \mathfrak{T} $ of bounded subsets of F, we define similarly the notion of $ \mathfrak{T}$-hypocontinuous mapping, by interchanging the roles of E and F in prop. 3. A separately continuous bilinear mapping u is said to be $ (\mathfrak{S}, \mathfrak{T}) $-hypocontinuous if it is both $ \mathfrak{S}$-hypocontinuous and $ \mathfrak{T}$-hypocontinuous.

Every *continuous* bilinear mapping from $ E \times F $ into $ G $ is $(\mathcal{S}, \mathcal{T})$-hypocontinuous for every pair $(\mathcal{S}, \mathcal{T})$ of sets of bounded subsets : for every neighbourhood $ W $ of 0 in $ G $, there exists a neighbourhood $ U $ of 0 in $ E $ and a neighbourhood $ V $ of 0 in $ F $ such that $ u(U \times V) \subset W $; since every set $ M \in \mathcal{S} $ is bounded, there exists $ \lambda > 0 $ such that $ \lambda M \subset V $, and so

$$
u(M \times \lambda V) = u(\lambda M \times V) \subset u(U \times V) \subset W .
$$

The converse is in general false (III, p. 47, exerc. 3).

#### Proposition 4 {#evt-iii-s5-prop-4 .statement}

*Let $ u $ be a $ \mathcal{S} $-hypocontinuous bilinear mapping from $ E \times F $ into $ G $. For every set $ M \in \mathcal{S} $, the restriction of $ u $ to $ M \times F $ is continuous, and $ u(M \times Q) $ is bounded in $ G $ for every bounded subset $ Q $ of $ F $.*

The first assertion follows from cor. 3 of GT, X, § 2, No. 1. Let $ W $ be a neighbourhood of 0 in $ G $; there exists, by hypothesis, a neighbourhood $ V $ of 0 in $ F $ such that $ u(M \times V) \subset W $. Since there exists $ \lambda \neq 0 $ such that $ \lambda Q \subset V $, we have $ \lambda u(M \times Q) = u(M \times \lambda Q) \subset W $, and this proves the second part of the proposition.

#### Proposition 5 {#evt-iii-s5-prop-5 .statement}

*Let $ u $ be a $(\mathcal{S}, \mathcal{T})$-hypocontinuous bilinear mapping from $ E \times F $ into $ G $. For every pair of sets $ M \in \mathcal{S} $, $ N \in \mathcal{T} $, $ u $ is uniformly continuous on $ M \times N $.*

The proposition follows immediately from prop. 2 of GT, X, § 2, No. 1 and prop. 5 of GT, X, § 2, No. 2.

#### Proposition 6 {#evt-iii-s5-prop-6 .statement}

*If $ F $ is a barrelled space, every separately continuous bilinear mapping $ u $ from $ E \times F $ into a locally convex space $ G $ is $ \mathcal{S} $-hypocontinuous for every set $ \mathcal{S} $ of bounded subsets of $ E $.*

In other words, the *linear mapping* $ y \mapsto u(., y) $ from $ F $ into $ \mathcal{L}_b(E; G) $ *is continuous*.

It is enough (III, p. 30, prop. 3) to prove that the image of every bounded subset $ M $ of $ E $ under $ x \mapsto u(x, .) $ is equicontinuous in $ \mathcal{L}(F; G) $. But, by virtue of prop. 1 (III, p. 28) this image is a simply bounded subset of $ \mathcal{L}(F; G) $, and since $ F $ is barrelled, every simply bounded subset of $ \mathcal{L}(F; G) $ is equicontinuous (III, p. 25, th. 1).

#### Remark {#evt-iii-s5-n3-rem-1 .statement}

— Suppose the topology of $ F $ is the finest locally convex topology on $ F $ for which the linear mappings $ h_\alpha : F_\alpha \to F $ are continuous (II, p. 27). Then condition *c)* of prop. 3 (III, p. 30) shows that if $ E $ and $ G $ are locally convex, then the bilinear mapping $ u : E \times F \to G $ is $ \mathcal{S} $-hypocontinuous if and only if each of the bilinear mappings

$$
(x, y_\alpha) \mapsto u(x, h_\alpha(y_\alpha))
$$

from $ E \times F_\alpha $ into $ G $ is $ \mathcal{S} $-hypocontinuous.

Now suppose that $ E $ is a locally convex space which is the *strict* inductive limit of an increasing sequence $ (E_n) $ of closed vector subspaces of $ E $ (II, p. 33); then every set $ M \in \mathcal{S} $ is contained in one of the $ E_n $ and is bounded in this subspace (III, p. 5, prop. 6). We denote by $ \mathcal{S}_n $ the family of all subsets belonging to $ \mathcal{S} $ contained in $ E_n $.

Condition $a)$ of prop. 3 (III, p. 30) shows that for a bilinear mapping $u : E \times F \to G$ to be $\mathfrak{S}$-hypocontinuous, it is necessary and sufficient that each of the restrictions $u_n : E_n \times F \to G$ of $u$ is $\mathfrak{S}_n$-hypocontinuous.

### 4. Extension of a hypocontinuous bilinear mapping

Proposition 7. — *Let* $E, F, G$ *be three locally convex spaces*, $G$ *being assumed Hausdorff*; *let* $E_0$ *(resp. $F_0$) be a dense vector subspace of* $E$ *(resp. $F$). Let* $u$ *be a separately continuous bilinear mapping from* $E \times F$ *into* $G$.

1) *If* $u(E_0 \times F_0) = \{0\}$, *then* $u = 0$.

2) *Let* $\mathfrak{S}_0$ *be a family of bounded subsets of* $E_0$; *if the restriction of* $u$ *to* $E_0 \times F_0$ *is* $\mathfrak{S}_0$*-hypocontinuous then so is* $u$.

1) By hypothesis, for all $x \in E_0$, the continuous linear mapping $u(x, .)$ is null on $F_0$, hence on $F$: therefore for all $y \in F$, the continuous linear mapping $u(., y)$ is null on $E_0$, hence on $E$. This proves that $u = 0$.

2) For every closed neighbourhood $W$ of 0 in $G$ and for every set $M \in \mathfrak{S}_0$, there exists, by hypothesis, a neighbourhood $V$ of 0 in $F_0$ such that $u(M \times V) \subset W$. But $\overline{V}$ is a neighbourhood of 0 in $F$; for every $x \in M$, the relation $u(\{x\} \times V) \subset W$ implies that $u(\{x\} \times \overline{V}) \subset W$, since $u(x, .)$ is continuous and $W$ is closed; therefore $u(M \times \overline{V}) \subset W$, which proves that $u$ is $\mathfrak{S}_0$*-hypocontinuous.

Proposition 8. — *Let* $E, F, G$ *be three locally convex spaces*; *assume that* $G$ *is Hausdorff and quasi-complete*. *Let* $E_0$ *(resp. $F_0$) be a dense vector subspace of* $E$ *(resp. $F$), $\mathfrak{S}_0$ *(resp. $\mathfrak{T}_0$) a family of bounded subsets of* $E_0$ *(resp. $F_0$) such that every point of* $E$ *(resp. $F$) is in the closure of an element of* $\mathfrak{S}_0$ *(resp. $\mathfrak{T}_0$). Then every* $(\mathfrak{S}_0, \mathfrak{T}_0)$*-hypocontinuous bilinear mapping* $u$ *from* $E_0 \times F_0$ *into* $G$ *extends uniquely to a separately continuous bilinear mapping* $\overline{u}$ *from* $E \times F$ *into* $G$ *and* $\overline{u}$ *is* $(\mathfrak{S}_0, \mathfrak{T}_0)$*-hypocontinuous*.

The uniqueness and hypocontinuity of $\overline{u}$ follows from prop. 7; it remains to prove the existence of $\overline{u}$. For every $y' \in F_0$, the continuous linear mapping $x' \mapsto u(x', y')$ from $E_0$ into $G$ extends uniquely to a continuous linear mapping $x \mapsto u_1(x, y')$ from $E$ into $G$ (III, p. 8, prop. 10). It follows immediately that for every $x \in E$, the mapping $y' \mapsto u_1(x, y')$ from $F_0$ into $G$ is linear; and we shall show that it is continuous. By hypothesis, there exists $M \in \mathfrak{S}_0$, such that $x \in \overline{M}$. For every closed neighbourhood $W$ of 0 in $G$, there exists, by hypothesis, a neighbourhood $V$ of 0 in $F_0$ such that $u(M \times V) \subset W$; since $x \mapsto u_1(x, y')$ is continuous, we deduce that $u_1(\overline{M} \times V) \subset W$, and in particular $u_1(x, y') \in W$ for all $y' \in V$. This establishes our assertion. By virtue of prop. 7, the bilinear map $u_1$ from $E \times F_0$ into $G$ is $(\mathfrak{S}_0, \mathfrak{T}_0)$*-hypocontinuous. We end the proof by interchanging the roles of $E$ and $F$ in the first part of the proof, applied to $u_1$.

### 5. Hypocontinuity of the mapping $(u, v) \mapsto v \circ u$

Proposition 9. — *Let* $R, S, T$ *be three locally convex Hausdorff spaces*. *Suppose that the spaces* $\mathcal{L}(R; S), \mathcal{L}(S; T), \mathcal{L}(R; T)$ *are each assigned the topology of simple* (resp. *compact*, *bounded*) convergence. *Then the bilinear mapping* $(u, v) \mapsto v \circ u$ *from* $\mathcal{L}(R; S) \times \mathcal{L}(S; T)$ *into* $\mathcal{L}(R; T)$ *is* $(\mathfrak{S}, \mathfrak{T})$-*hypocontinuous*, *where* $\mathfrak{T}$ *is the family of equicontinuous subsets of* $\mathcal{L}(S; T)$, *and* $\mathfrak{S}$ *the family of finite* (resp. *compact, bounded*) *subsets of* $\mathcal{L}(R; S)$.

We first prove that $(u, v) \mapsto v \circ u$ is $\mathfrak{T}$-hypocontinuous. Let H be an equicontinuous set in $\mathcal{L}(S; T)$, let W be a neighbourhood of 0 in T and let M be a finite (resp. compact, bounded) subset of R. We must show that there exists a neighbourhood V of 0 in S such that if $u(M) \subset V$ and $v \in H$, then $v(u(M)) \subset W$. But for this, it is enough to have $v(V) \subset W$ for all $v \in H$, and the existence of such a neighbourhood follows from the equicontinuity of H.

To see that $(u, v) \mapsto v \circ u$ is $\mathfrak{S}$-hypocontinuous, we shall prove that, for every neighbourhood W of 0 in T, every finite (resp. compact, bounded) subset M of R and every finite (resp. compact, bounded) subset L of $\mathcal{L}(R; S)$ there exists a finite (resp. compact, bounded) subset N of S such that the relations $v(N) \subset W$ and $u \in L$ imply that $v(u(M)) \subset W$. Evidently it is enough to show that we can take $N = \bigcup_{u \in L} u(M)$, *i.e.* that the set N is finite (resp. compact, bounded) whenever L and M are. This is immediate if L and M are finite, or if M is bounded in R and L is bounded in $\mathcal{L}(R; S)$ (for the topology of bounded convergence, *cf.* III, p. 22). Finally, we show that if M is compact in R and L is compact in $\mathcal{L}(R; S)$ for the topology of compact convergence, then N is compact in S. But if $u_M$ is the restriction to M of $u \in L$, the mapping $u \mapsto u_M$ from L into the space $\mathcal{C}(M; S)$ of all continuous mappings from M into S, with the topology of uniform convergence, is continuous; hence the image of L under this mapping is compact, and our assertion then follows from the continuity of the map $(w, x) \mapsto w(x)$ from $\mathcal{C}(M; S) \times M$ into S (GT, X, § 1, No. 6, prop. 9).

In the two corollaries that follow, we assume as in prop. 9, that the spaces $\mathcal{L}(R; S)$, $\mathcal{L}(S; T)$, $\mathcal{L}(R; T)$ are *all three* assigned the topology of simple convergence, or all three the topology of compact convergence, or all three that of bounded convergence.

#### Corollary 1 {#evt-iii-s5-prop-6-cor-1 .statement}

*For every equicontinuous subset H of* $\mathcal{L}(S; T)$ *the map* $(u, v) \mapsto v \circ u$ *from* $\mathcal{L}(R; S) \times H$ *into* $\mathcal{L}(R; T)$ *is continuous*.

This follows immediately from prop. 9 (III, p. 32) and 4 (III, p. 31).

#### Corollary 2 {#evt-iii-s5-prop-6-cor-2 .statement}

*Suppose S is barrelled. If the sequence* $(u_n)$ *tends to u in* $\mathcal{L}(R; S)$ *and the sequence* $(v_n)$ *to v in* $\mathcal{L}(S, T)$, *then the sequence* $(v_n \circ u_n)$ *tends to* $v \circ u$ *in* $\mathcal{L}(R; T)$.

In fact, the sequence $(v_n)$, being simply bounded in $\mathcal{L}(S; T)$ is equicontinuous, since S is barrelled (III, p. 25, th. 1); the corollary is then a consequence of cor. 1.

### Exercises {#evt-iii-s5-exercises}

See the [exercises for § 5](exercises/s5/).
