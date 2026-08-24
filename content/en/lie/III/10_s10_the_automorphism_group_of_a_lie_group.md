---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: III
chapter_title: LIE GROUPS
section: 10
section_title: The automorphism group of a Lie group
lang: en
source: lie-i-iii
pdf_pages: 0377-0386, 0427-0481
extraction: ocr
subsections:
    - "no": 1
      title: INFINITESIMAL AUTOMORPHISMS
      page: 0
      pdf_page: 377
    - "no": 2
      title: THE AUTOMORPHISM GROUP OF A LIE GROUP (REAL OR COMPLEX CASE)
      page: 0
      pdf_page: 380
    - "no": 3
      title: THE AUTOMORPHISM GROUP OF A LIE GROUP (ULTRAMETRIC CASE)
      page: 0
      pdf_page: 385
statements: 13
exercises: 3
content_sha256: ce97d672d395324edaf19e576695e17d7e634e8c8ecae751b42c35b7ffc0b7a4
---

## § 10. THE AUTOMORPHISM GROUP OF A LIE GROUP

In this paragraph, K is assumed to be of characteristic zero.

### 1. INFINITESIMAL AUTOMORPHISMS

#### Lemma 1 {#lie-iii-s10-lem-1 .statement}

Let G be a Lie group and $ \alpha $ a vector field on G. For all $ g \in G $, let
$$
\beta(g) = \alpha(g)g^{-1} \in L(G).
$$
The following conditions are equivalent:
(i) $ \alpha $ is a homomorphism of the group G into the group T(G);
(ii) for all $ g, g' $ in G, $ \alpha(gg') = \alpha(g)g' + g\alpha(g') $;
(iii) for all $ g, g' $ in G, $ \beta(gg_1) = \beta(g) + (\mathrm{Ad}\,g)\beta(g') $.

Condition (i) means that, for all $ g, g' $ in G, we have in the group T(G):
$$
\beta(g)g\beta(g')g' = \beta(gg')gg'
$$
or
$$
\beta(g)((\mathrm{Ad}\,g)\beta(g'))gg' = \beta(gg')gg'.
$$
But the product of $ \beta(g) $ and $ (\mathrm{Ad}\,g)\beta(g') $ in T(G) is just the sum of $ \beta(g) $ and $ (\mathrm{Ad}\,g)\beta(g') $ in $ L(G) $ (\S 2, no. 1, Proposition 2). Hence (i) $ \Leftrightarrow $ (iii). On the other hand, condition (ii) may be written $ \beta(gg')gg' = \beta(g)gg' + g\beta(g')g' $, or
$$
\beta(gg') = \beta(g) + (\mathrm{Ad}\,g)\beta(g')
$$
and hence (ii) $ \Leftrightarrow $ (iii).

#### Definition 1 {#lie-iii-s10-def-1 .statement}

Let G be a Lie group. An infinitesimal automorphism of G is any analytic vector field on G satisfying the conditions of Lemma 1.

#### Lemma 2 {#lie-iii-s10-lem-2 .statement}

Let $ K' $ be a non-discrete closed subfield of K, A a $ K' $-manifold, B and C $ K $-manifolds and $ f $ a $ K' $-analytic mapping of $ A \times B $ into C. Suppose that, for all

LIE GROUPS

$a \in A$, *the mapping* $b \mapsto f(a, b)$ *of* B *into* C *is* K-*analytic*. *Then, for all* $t \in TA$, *the mapping* $u \mapsto (Tf)(t, u)$ *of* TB *into* TC *is* K-*analytic*.

We fix $t \in TA$ and write $g(u) = (Tf)(t, u)$. Clearly $g$ is K'-analytic. By *Differentiable and Analytic Manifolds*, R, 5.14.6, it suffices to prove that the tangent mappings to $g$ are K-linear. It can be assumed that A, B, C are open neighbourhoods of 0 in complete normable spaces E, F, G over K', K, K and that $t$ is tangent to A at 0. We identify TA, TB, TC, with $A \times E, B \times F, C \times G$ and $t$ with an element of E. Then for all $(x, y) \in TB = B \times F$.

$$
g(x, y) = (f(0, x), (D_1f)(0, x)(t) + (D_2f)(0, x)(y)).
$$

We identify $T(B \times F)$ with $(B \times F) \times (F \times F)$ and $T(C \times G)$ with $(C \times G) \times (G \times G)$. Then, for all

$$
((x, y), (h, k)) \in T(B \times F) = (B \times F) \times (F \times F),
$$

$(Tg)((x, y), (h, k)) = ((a, b), (c, d))$, where

$$
\begin{align*}
a &= f(0, x), \\
b &= (D_1f)(0, x)(t) + (D_2f)(0, x)(y), \quad c = (D_2f)(0, x)(h), \\
d &= (D_2D_1f)(0, x)(t, h) + (D_2D_2f)(0, x)(y, h) + (D_2f)(0, x)(k).
\end{align*}
$$

We now fix $(x, y) \in B \times F$. We need to prove that the mapping $(h, k) \mapsto (c, d)$ of $F \times F$ into $G \times G$ is K-linear. As the mapping $x \mapsto f(0, x)$ of B into C is K-analytic, the mappings

$$
(h, k) \mapsto (D_2f)(0, x)(h), \quad (h, k) \mapsto (D_2D_2f)(0, x)(y, h),
$$
$$(h, k) \mapsto (D_2f)(0, x)(k)$$

are K-linear. On the other hand

$$
(D_2D_1f)(0, x)(t, h) = \lim_{\lambda \in K', \lambda \to 0} \lambda^{-1}((D_2f)(\lambda t, x)(h) - (D_2f)(0, x)(h))
$$

and, for fixed $\lambda$, the mapping $x \mapsto f(\lambda t, x)$ is K-analytic, so that the mapping $h \mapsto (D_2f)(\lambda t, x)(h)$ is K-linear.

#### Proposition 1 {#lie-iii-s10-prop-1 .statement}

*Let* K' *be a non-discrete closed subfield of* K, G *a Lie group over* K, V *a manifold over* K' *and* $(v, g) \mapsto vg$ *a* K'-*analytic mapping of* V $\times$ G *into* G. *Suppose that, for all* $v \in V$, *the mapping* $g \mapsto vg$ *of* G *into* G *is an automorphism of* G. *Let* $\varepsilon$ *be an element of* V *such that* $\varepsilon g = g$ *for all* $g \in G$ *and* $a \in T_\varepsilon(V)$. *Then the vector field* $g \mapsto ag$ *on* G *is an infinitesimal automorphism of* G.

For $v \in V,\ g_1 \in G,\ g_2 \in G,\ v(g_1g_2) = (vg_1)(vg_2)$. Hence, for $u_1 \in TG,\ u_2 \in TG,\ a(u_1u_2) = (au_1)(au_2)$ (\S 2, no. 1, Proposition 3). In particular, the mapping $g \mapsto ag$ of G into TG is a group homomorphism. On the other hand, this mapping is analytic by Lemma 2.

#### Proposition 2 {#lie-iii-s10-prop-2 .statement}

*Let* G *be a real or complex Lie group and* $\alpha$ *an infinitesimal automorphism of G. There exists a law of analytic operation $(\lambda, g) \mapsto \phi_\lambda(g)$ of K on G with the following properties:
(1) if D is the associated law of infinitesimal operation, then $D(1) = \alpha$;
(2) for all $\lambda \in K$, $\phi_\lambda \in \mathrm{Aut}\, G$.
(a) For all $\mu > 0$, let $K_\mu$ be the open ball of centre 0 and radius $\mu$ in K. For all $g \in G$, let $\mathcal{F}_g$ be the set of analytic integral curves $f$ of $\alpha$ defined in a ball $K_\mu$ and such that $f(0) = g$. By Differentiable and Analytic Manifolds, R, 9.1.3 and 9.1.5, $\mathcal{F}_g$ is non-empty and two elements of $\mathcal{F}_g$ coincide on the intersection of their domains of definition; let $\mu(g)$ be the least upper bound of the numbers $\mu$ such that there exists an element of $\mathcal{F}_g$ defined in $K_\mu$; there exists a unique element of $\mathcal{F}_g$ defined in $K_{\mu(g)}$; we denote it by $f_g$.
(b) Let $g_1, g_2$ be in G, $f_1 \in \mathcal{F}_{g_1}, f_2 \in \mathcal{F}_{g_2}$ with $f_1$ and $f_2$ defined on the same ball $K_\mu$. Then $f_1 f_2 : K_\mu \to G$ is analytic and $(f_1 f_2)(0) = g_1 g_2$. On the other hand, for all $\lambda \in K_\mu$,

$$
(T_\lambda(f_1 f_2))1 = (T_\lambda f_1)1 \cdot f_2(\lambda) + f_1(\lambda) \cdot (T_\lambda f_2)1 \quad (\S\ 2,\ \text{Proposition 7})
$$
$$
= \alpha(f_1(\lambda)) f_2(\lambda) + f_1(\lambda) \alpha(f_2(\lambda))
$$
$$
= \alpha((f_1 f_2)(\lambda)) \tag{\text{Lemma 1}}
$$

and hence $f_1 f_2 \in \mathcal{F}_{g_1 g_2}$. This proves that $\mu(g_1 g_2) \geq \inf_{g \in V} (\mu(g_1), \mu(g_2))$.
(c) By Differentiable and Analytic Manifolds, R, 9.1.4 and 9.1.5, there exists a neighbourhood V of e in G such that $\sigma = \inf_{g \in V} \mu(g) > 0$. Let $h \in G$ and C be its connected component. For all $h' \in C$, $\mu(h') \geq \inf(\sigma, \mu(h)) > 0$ by (b). On the other hand, the functions $f_{h'}$, where $h' \in C$, take their values in C. By Differentiable and Analytic Manifolds, R, 9.1.4 and 9.1.5, $\mu = +\infty$ in C and finally $\mu = +\infty$ in G. Then let $f_g(\lambda) = \phi_\lambda(g)$ for all $g \in G$ and all $\lambda \in K$. By Differentiable and Analytic Manifolds, R, 9.1.4 and 9.1.5, the mapping $(\lambda, g) \mapsto \phi_\lambda(g)$ is a law of analytic operation of K on G. Clearly, if D is the associated law of infinitesimal operation, $D(1) = \alpha$. By (b),

$$
\phi_\lambda(g_1 g_2) = \phi_\lambda(g_1) \phi_\lambda(g_2)
$$

for all $\lambda \in K, g_1 \in G, g_1 \in G$.

#### Proposition 3 {#lie-iii-s10-prop-3 .statement}

Suppose that K is ultrametric. Let G be a compact Lie group and $\alpha$ an infinitesimal automorphism of G. There exist an open subgroup I of K and a law of analytic operation $(\lambda, g) \mapsto \phi_\lambda(g)$ of I on G with the following properties:
(1) if D is the associated law of infinitesimal operation, then $D(1) = \alpha$;
(2) for all $\lambda \in I, \phi_\lambda \in \mathrm{Aut}\, G$.
As G is compact, there exist an open subgroup I' of K and a law of analytic operation $(\lambda, g) \mapsto \phi_\lambda(g)$ of I' on G with property (1) of the proposition (§ 4, no. 7, Corollary 2 to Theorem 6). We write $ \phi_\lambda(g) = f_g(\lambda) $ for $ \lambda \in I' $ and $ g \in G $. Then, for $ g_1, g_2 $ in $ G $ and $ \lambda \in I' $,

$$
(T_\lambda(f_{g_1}f_{g_2}))1 = (T_\lambda f_{g_1})1 \cdot f_{g_2}(\lambda) + f_{g_1}(\lambda) \cdot (T_\lambda f_{g_2})1 \\
= \alpha(f_{g_1}(\lambda)) f_{g_2}(\lambda) + f_{g_1}(\lambda) \alpha(f_{g_2}(\lambda)) \\
= \alpha(f_{g_1}(\lambda) f_{g_2}(\lambda))
$$

and $ (f_{g_1}f_{g_2})(0) = g_1 g_2 = f_{g_1g_2}(0) $. Hence $ f_{g_1'g_2'}(\lambda) = f_{g_1'}(\lambda) f_{g_2'}(\lambda) $ for $ (g_1', g_2', \lambda) $

in a neighbourhood of $ (g_1, g_2, 0) $ (Differentiable and Analytic Manifolds, R, 9.1.8). As $ G $ is compact, there exists an open subgroup $ I $ of $ I' $ such that $ f_{g_1g_2}(\lambda) = f_{g_1}(\lambda) f_{g_2}(\lambda) $ for all $ g_1 \in G, g_2 \in G, \lambda \in I $. In other words, $ \phi_\lambda \in \mathrm{Aut}\, G $ for $ \lambda \in I $.

#### Lemma 3 {#lie-iii-s10-lem-3 .statement}

Let $ G $ and $ G' $ be Lie groups and $ \phi $ a homomorphism of $ G $ into $ \mathrm{Aut}(G') $. Let $ f(g, g') = (\phi(g))(g') $ for $ g \in G, g' \in G' $. Consider the following conditions:
(i) $ f $ is analytic;
(ii) $ f $ is analytic in a neighbourhood of $ (e_G, e_{G'}) $;
(iii) for all $ g' \in G' $, the mapping $ g \mapsto f(g, g') $ is analytic.
Then (i) $ \Leftrightarrow $ ((ii) and (iii)). If $ G $ is connected, (i) $ \Leftrightarrow $ (ii).
Clearly (i) implies (ii) and (iii). Let $ g_0 \in G, g_0' \in G' $. For all $ g \in G, g' \in G' $,

$$
f(gg_0, g'g_0') = (\phi(g)\phi(g_0))(g'g_0') = \phi(g)(\phi(g_0)g').\phi(g)(\phi(g_0)g_0').
$$

This proves the implication ((ii) and (iii)) $ \Rightarrow $ (i). Finally, if $ G' $ is connected, $ G' $ is generated by every neighbourhood of $ e_{G'} $ and hence (ii) $ \Rightarrow $ (iii).

### 2. THE AUTOMORPHISM GROUP OF A LIE GROUP (REAL OR COMPLEX CASE)

In this no., we assume that $ K = \mathbf{R} $ or $ \mathbf{C} $.

#### Lemma 4 {#lie-iii-s10-lem-4 .statement}

Let $ H $ be a finite-dimensional simply connected Lie group.
(i) For all $ u \in \mathrm{Aut}\, L(H) $, let $ \theta(u) $ be the unique automorphism of $ H $ such that $ L(\theta(u)) = u $. Then the mapping $ (u, g) \mapsto \theta(u)g $ of $ (\mathrm{Aut}\, L(H)) \times H $ into $ H $ is analytic.
(ii) Let $ N $ be a Lie subgroup of $ H $ and $ \mathrm{Aut}(H, N) $ the set of $ v \in \mathrm{Aut}\, H $ such that $ v(N) = N $. Then $ 0^{-1}(\mathrm{Aut}(H, N)) $ is a Lie subgroup of $ \mathrm{Aut}\, L(H) $.
(iii) Suppose that $ N $ is discrete and normal, so that the Lie algebra of $ G = H/N $ is identified with $ L(H) $. For all $ w \in \mathrm{Aut}\, G $, let $ \eta(w) $ be the unique automorphism of $ H $ such that $ L(\eta(w)) = L(w) $. Then the mapping $ \eta $ is an isomorphism of the group $ \mathrm{Aut}\, G $ onto the group $ \mathrm{Aut}(H, N) $.
To prove (i), it suffices, by Lemma 3 of no. 1, to verify that the mapping $ (u, g) \mapsto \theta(u)g $ is analytic in a neighbourhood of $ (\mathrm{Id}_{L(H)}, e) $. There exists an open neighbourhood B of 0 in $ L(H) $ such that $ \psi = \exp_H|B $ is an analytic isomorphism of B onto an open neighbourhood of e in H. There exist an open neighbourhood U of $ \mathrm{Id}_{L(H)} $ in Aut $ L(H) $ and an open neighbourhood $ B' $ of 0 in $ L(H) $ such that $ U(B') \subset B $. Then the mapping $ (u, g) \mapsto \theta(u)g $ of $ U \times \psi(B') $ into H is composed of the following mappings:

the mapping $ (u, g) \mapsto (u, \psi^{-1}(g)) $ of $ U \times \psi(B') $ into $ U \times B' $;
the mapping $ (u, x) \mapsto u(x) $ of $ U \times B' $ into $ B $;
the mapping $ y \mapsto \psi(y) $ of $ B $ into $ G $.

Hence this mapping is analytic.

Let $ p $ be the canonical mapping of H into the homogeneous space $ H/N $. Then $ \theta^{-1}(\mathrm{Aut}(H, N)) $ is the set of $ u \in \mathrm{Aut}\ L(H) $ such that
$$
p(\theta(u)g) = p(e), \quad p(\theta(u^{-1})g) = p(e)
$$
for all $ g \in N $. By § 8, no. 2, Theorem 2 and Corollary 2 to Theorem 2, this proves (ii).

Suppose that N is discrete and normal. Let $ w \in \mathrm{Aut}\ G $. Then
$$
L(p \circ \eta(w)) = L(\eta(w)) = L(w) = L(w \circ p)
$$
hence $ p \circ \eta(w) = w \circ p $ and therefore $ \eta(w) \in \mathrm{Aut}(H, N) $. Clearly the mapping $ \eta $ of $ \mathrm{Aut}\ G $ into $ \mathrm{Aut}(H, N) $ is an injective homomorphism. This homomorphism is surjective because $ p : H \to G $ is a submersion.

Let G be a locally compact group and $ \Gamma $ the automorphism group of G. Recall that a topology $ \mathcal{T}_\beta $ has been defined on $ \Gamma $ (General Topology, Chapter X, § 3, no. 5). It is the coarsest topology for which the mappings $ v \mapsto v $ and $ v \mapsto v^{-1} $ of $ \Gamma $ into $ C_c(G; G) $ (space of continuous mappings of G into G with the compact convergence topology) are continuous. The topology $ \mathcal{T}_\beta $ is compatible with the group structure on $ \Gamma $ (loc. cit.). For every compact subset L of G and every neighbourhood U of $ e_G $ in G, let $ N(L, U) $ be the set of $ \phi \in \Gamma $ such that $ \phi(g) \in gU $ and $ \phi^{-1}(g) \in gU $ for all $ g \in L $; then the $ N(L, U) $ form a fundamental system of neighbourhoods of $ e_\Gamma $. If G is generated by a compact subset C, the topology $ \mathcal{T}_\beta $ is also the coarsest topology for which the mappings $ v \mapsto v|C $ and $ v \mapsto v^{-1}|C $ of $ \Gamma $ into $ C_u(C; G) $ are continuous (for every compact subset of G is contained in $ (C \cup C^{-1})^n $ for sufficiently large n). If K is locally compact and V is a finite-dimensional vector space over K, the topology $ \mathcal{T}_\beta $ on $ \mathbf{GL}(V) $ is just the usual topology.

#### Theorem 1 {#lie-iii-s10-thm-1 .statement}

Let G be a finite-dimensional Lie group and $ G_0 $ its identity component. Suppose that G is generated by $ G_0 $ and a finite number of elements.

(i) There exists on $ \mathrm{Aut}\ G $ one and only one analytic manifold structure satisfying the following condition:
(AUT) for every analytic manifold M and every mapping f of M into $ \mathrm{Aut}\ G $, f is analytic if and only if the mapping $ (m, g) \mapsto f(m)g $ of $ M \times G $ into G is analytic.

Suppose in the rest of the statement that Aut G has this structure.
(ii) Aut G is a finite-dimensional Lie group.
(iii) The morphism $ \phi : u \mapsto L(u) $ of Aut G into Aut L(G) is analytic.
(iv) If G is connected, $ \phi $ is an isomorphism of the Lie group Aut G onto a Lie subgroup of Aut L(G); this Lie subgroup is equal to Aut L(G) if G is simply connected.
(v) Let $ a $ be the set of infinitesimal automorphisms of G. Then $ a $ is a Lie algebra of vector fields and the law of infinitesimal operation associated with the mapping $ (u, g) \mapsto u(g) $ of (Aut G) $ \times $ G into G is an isomorphism of L(Aut G) onto $ a $.
(vi) The topology of the Lie group Aut G is the topology $ \mathcal{T}_\beta $.
(a) The uniqueness of the analytic structure considered in (i) is obvious.
(b) Suppose that G is connected. Let H be the universal covering space of G, $ p $ the canonical morphism of H onto G and N = Ker $ p $. We introduce the notation $ \theta $, $ \eta $ and Aut(H, N) of Lemma 4. We transport the Lie group structure of Aut L(G) to Aut H by means of $ \theta $. Then Aut H becomes a finite-dimensional Lie group and Aut(H, N) a Lie subgroup of Aut H (Lemma 4 (ii)). We transport the Lie group structure of Aut(H, N) to Aut G by means of $ \eta^{-1} $. Then Aut G becomes a finite-dimensional Lie group. Properties (ii), (iii) and (iv) of the theorem are satisfied and the mapping $ (u, g) \mapsto u(g) $ of (Aut G) $ \times $ G into G is analytic (Lemma 4 (i)). Let M be an analytic manifold, $ f $ a mapping of M into Aut G and $ \phi $ the mapping $ (m, g) \mapsto f(m)g $ of M $ \times $ G into G. Clearly, if $ f $ is analytic, $ \phi $ is analytic. Suppose that $ \phi $ is analytic. Then the T$ \phi $: TM $ \times $ TG $ \to $ TG is analytic; its restriction to M $ \times $ L(G), that is the mapping $ (m, x) \mapsto L(f(m))x $ of M $ \times $ L(G) into L(G) is therefore analytic; as L(G) is finite-dimensional, it follows that the mapping $ m \mapsto L(f(m)) $ of M into Aut L(G) is analytic and hence that $ f $ is analytic. Thus (i) holds.

Let L(G) be given a norm. For all $ \lambda > 0 $, let B_\lambda be the open ball of centre 0 and radius $ \lambda $ in L(G). We choose $ \lambda > 0 $ sufficiently small for $ \psi = \exp_G|_{B_\lambda} $ to be an isomorphism of the analytic manifold B_\lambda onto the open submanifold $ \psi(B_\lambda) $ of G. Let $ \Phi $ be a filter on Aut G. For $ \Phi $ to converge to Id_G in Aut G, it is necessary and sufficient that L($ \Phi $) converge to Id_{L(G)} in Aut L(G) and hence that L($ \Phi $)|_{B_{\lambda/2}} and L($ \Phi $)^{-1}|_{B_{\lambda/2}} converge uniformly to Id_{B_{\lambda/2}}. This condition implies that $ \Phi|\psi(B_{\lambda/2}) $ and $ \Phi^{-1}|\psi(B_{\lambda/2}) $ converge uniformly to Id_{$ \psi(B_{\lambda/2}) $}. Conversely, suppose that $ \Phi|\psi(B_{\lambda/2}) $ converges uniformly to Id_{$ \psi(B_{\lambda/2}) $}. There exists M $ \in \Phi $ such that, if $ u \in M $, then $ u(\psi(B_{\lambda/2})) \subset \psi(B_{2\lambda/3}) $; then L(u)(B_{\lambda/2}) is a connected subset of L(G) whose image under $ \exp_G $ is contained in $ \psi(B_{2\lambda/3}) $, hence L(u)(B_{\lambda/2}) does not meet $ B_\lambda - B_{2\lambda/3} $ and therefore L(u)(B_{\lambda/2}) $ \subset $ B_\lambda; then the hypothesis that $ \Phi|\psi(B_{\lambda/2}) $ converges uniformly to Id_{$ \psi(B_{\lambda/2}) $} implies that L($ \Phi $)|_{B_{\lambda/2}} converges uniformly to Id_{B_{\lambda/2}}. It then follows that:

$$
(\Phi \text{ converges to } \mathrm{Id}_G \text{ in Aut } G) \iff (\Phi \text{ converges to } \mathrm{Id}_G \text{ under } \mathcal{T}_\beta).
$$

This proves (vi).

Let D be the law of infinitesimal operation associated with the law of left operation of Aut(G) on G. By Propositions 1 and 2 of no. 1, $ D(L(\text{Aut } G)) = a $. Hence a is a Lie algebra of vector fields and D is a morphism of $ L(\text{Aut } G) $ onto a. Let $ x_1 $ and $ x_2 $ be elements of $ L(\text{Aut } G) $ such that $ D(x_1) = D(x_2) $. Then the laws of operation $ (\lambda, g) \mapsto (\exp \lambda x_1)g $ and $ (\lambda, g) \mapsto (\exp \lambda x_2)g $ of K on G have the same associated law of infinitesimal operation; hence, for $ |\lambda| $ sufficiently small, $ \exp \lambda x_1 $ and $ \exp \lambda x_2 $ coincide on a neighbourhood of e ($ \S 4 $, no. 7, Theorem 6), whence $ \exp \lambda x_1 = \exp \lambda x_2 $. It follows that $ x_1 = x_2 $ and hence D is an isomorphism of $ L(\text{Aut } G) $ onto a.

The theorem has thus been completely proved for G connected.

(c) We pass to the general case. By hypothesis, G is generated by $ G_0 $ and a finite number of elements $ x_1, x_2, \ldots, x_n $. Every $ u \in \text{Aut } G $ leaves $ G_0 $ stable. Let $ \text{Aut}_1 G $ be the set of $ u \in \text{Aut } G $ which, on passing to the quotient, give the identity automorphism of $ G/G_0 $. This is a normal subgroup of $ \text{Aut } G $. By part (b) of the proof, $ \text{Aut } G_0 $ has a canonical Lie group structure and the mapping $ (g_1, g_2, \ldots, g_n, u) \mapsto (ug_1, ug_2, \ldots, ug_n) $ of $ G_0^n \times \text{Aut } G_0 $ into $ G_0^n $ is analytic. Let P be the corresponding semidirect product of $ \text{Aut } G_0 $ by $ G_0^n $; it is a finite-dimensional Lie group ($ \S 1 $, no. 4, Proposition 7).

If $ w \in \text{Aut}_1 G $, we write
$$
w_0 = w|G_0 \in \text{Aut } G_0 \\
w_i = x_i^{-1}w(x_i) \in G_0 \quad (1 \leq i \leq n) \\
\zeta(w) = ((w_1, \ldots, w_n), w_0) \in P.
$$
For all $ w, w' $ in $ \text{Aut}_1 G $,
$$
\begin{align*}
\zeta(w)\zeta(w') &= ((w_1, \ldots, w_n)(w_0(w'_1), \ldots, w_0(w'_n)), w_0w'_0) \\
&= ((w_1w_0(w'_1), \ldots, w_nw_0(w'_n)), w_0w'_0) \\
&= ((x^{-1}w(x_1)w(x_1^{-1}w'(x_1)), \ldots, x_n^{-1}w(x_n)w(x_n^{-1}w'(x_n))), w_0w'_0) \\
&= (((ww')_1, \ldots, (ww')_n), (ww')_0) \\
&= \zeta(ww')
\end{align*}
$$
and hence $ \zeta $ is a homomorphism of $ \text{Aut}_1 G $ into P. This homomorphism is obviously injective.

We show that $ \zeta(\text{Aut}_1 G) $ is closed in P. Let $ \Phi $ be a filter on $ \text{Aut}_1 G $ such that $ \zeta(\Phi) $ converges to a point $ ((w_1, \ldots, w_n), w_0) $ of P. Then $ \Phi $ converges pointwise to a mapping v of G into G. Clearly v is an endomorphism of the group G. Moreover, v leaves each coset modulo $ G_0 $ stable and $ v|G_0 = w_0 $. It follows that $ v \in \text{Aut}_1 G $. As $ \zeta(v) = ((w_1, \ldots, w_n), w_0) $, we have shown that $ \zeta(\text{Aut}_1 G) $ is closed in P.

(d) In part (d) of the proof we assume that $ K = \mathbf{R} $. By $ \S 8 $, no. 2, Theorem 2, $ \zeta(\text{Aut}_1 G) $ is a Lie subgroup of P. We transport the real Lie group structure on $ \zeta(\text{Aut}_1 G) $ to $ \text{Aut}_1 G $ by means of $ \zeta^{-1} $. Thus $ \text{Aut}_1 G $ becomes a finite-dimensional Lie group.

Let M be an analytic manifold, f a mapping of M into Aut_1G and φ the mapping (m, g) ↦ f(m)g of M × G into G. We have the following equivalences:

f analytic
⇔ the mappings m: ↦ (f(m))_i, where 0 ≤ i ≤ n, are analytic
⇔ {the mappings m ↦ f(m)x_i of M into G, for 1 ≤ i ≤ n, are analytic
and
the mapping (m, g) ↦ f(m)g of M × G_0 into G is analytic
⇔ φ is analytic.

For w ∈ Aut_1G, L(w) = L(w_0) and hence the morphism w ↦ L(w) of Aut_1G into Aut L(G) is analytic. We see as in (b) that the law of infinitesimal operation associated with the law of operation of Aut_1G on G is an isomorphism of L(Aut_1G) onto a.

Let C be a compact subset of G_0 generating G_0. For a filter Φ to converge to Id_G on Aut_1G, it is necessary and sufficient that Φ|(C ∪ {x_1} ∪ ... ∪ {x_n}) and Φ^{-1}|(C ∪ {x_1} ∪ ... ∪ {x_n}) converge uniformly to

Id_a|(C ∪ {x_1} ∪ ... ∪ {x_n}).

The topology of Aut_1G is therefore the topology $ \mathcal{T}_\beta $.

Clearly Aut_1G is open in Aut G with the topology $ \mathcal{T}_\beta $. There exists on Aut G a Lie group structure compatible with this topology and inducing on Aut_1G the structure constructed above (\S 8, no. 1, Corollary 2 to Theorem 1). The fact that the Lie group Aut G has the properties of the theorem follows from the corresponding properties for Aut_1G.

(e) In part (e) of the proof we assume that K = C. By (c) and Theorem 2 of \S 8, no. 2, there exists on Aut_1G a real Lie group structure such that ζ is an isomorphism of Aut_1G onto a real Lie subgroup of P.

The law of operation (w, g) ↦ wg of (Aut_1G) × G on G is real analytic. Let D be the associated law of infinitesimal operation. By Propositions 1 and 2 of no. 1, D(L(Aut_1G)) = a.

For all α ∈ a, let α_0 denote the restriction of α to G_0; it is an infinitesimal automorphism of G_0 which we identify, because of part (b) of the proof, with an element of L(Aut G_0). For 1 ≤ i ≤ n, we write

$$ \alpha_i = x_i^{-1} \alpha(x_i) \in L(G) = L(G_0). $$

Finally, we write $ f(\alpha) = ((\alpha_1, ..., \alpha_n), \alpha_0) \in L(P) $. Then f is a C-linear mapping of a into L(P).

On the other hand, clearly $ L(\zeta) = f \circ D $. Hence $ L(\zeta)(L(Aut_1G)) = f(a) $ is a complex vector subspace of L(P). By Proposition 2 of \S 4, no. 2, $ \zeta(Aut_1G) $ is a complex Lie subgroup of P and we can proceed exactly as in (d): we transport the complex Lie group structure on $ \zeta(Aut_1G) $ to Aut_1G by means of $ \zeta^{-1} $ and we see as in (d) that Aut_1G has the properties analogous to properties (i), (ii), (iii), (v) and (vi) of the theorem.

Clearly Aut₁G is open in Aut G with the topology $ \mathcal{T}_\beta $. Let $ w \in \mathrm{Aut}\ G $. Let $ \sigma $ be the automorphism $ v \mapsto wvw^{-1} $ of Aut₁G. It is real analytic ($ \S 8 $, no. 1, Theorem 1), $ L(\sigma) $ is an $ \mathbf{R} $-automorphism of $ L(\mathrm{Aut}_1 G) $ and

$$
D \circ L(\mathrm{Aut}_1 G) \circ D^{-1}
$$

is an $ \mathbf{R} $-automorphism of $ a $. This automorphism is also the automorphism of $ a $ derived from $ w $ by transport of structure; as $ w $ is K-analytic, we see that $ L(\sigma) $ is K-linear. Hence $ \sigma $ is K-analytic ($ \S 3 $, no. 8, Proposition 32). By $ \S 1 $, no. 9, Proposition 18, there exists on Aut G one and only one Lie K-group structure such that $ \mathrm{Aut}_1 G $ is an open Lie subgroup of Aut G. The fact that this structure has the properties of the theorem follows from the corresponding properties for $ \mathrm{Aut}_1 G $.

#### Corollary 1 {#lie-iii-s10-thm-1-cor-1 .statement}

*Let G be a finite-dimensional real Lie group and $ G_0 $ its identity component. Suppose that G is generated by $ G_0 $ and a finite number of elements. Then Aut G has the topology $ \mathcal{T}_\beta $ and is a finite-dimensional real Lie group.*

#### Corollary 2 {#lie-iii-s10-thm-1-cor-2 .statement}

*Let G be a semi-simple connected real or complex Lie group. The group Int G is the identity component of Aut G.*

The mapping $ u \mapsto L(u) $ is an isomorphism of Aut G onto a Lie subgroup of Aut $ L(G) $ (Theorem 1). The image of Int G under this isomorphism is Ad G. But Ad G is the identity component of Aut $ L(G) $ ($ \S 9 $, no. 8, Proposition 30 (ii)).

### 3. THE AUTOMORPHISM GROUP OF A LIE GROUP (ULTRAMETRIC CASE)

#### Theorem 2 {#lie-iii-s10-thm-2 .statement}

*When K is ultrametric and locally compact and G is a compact Lie group, assertions (i), (ii), (iii), (v) and (vi) of Theorem 1 are true.*
(a) The uniqueness of the analytic structure considered in (i) is obvious.
(b) Suppose that G is the Lie group defined by the normable Lie algebra L. Then G is an open and closed ball in L. Let $ w \in \mathrm{Aut}\ G $. Then $ L(w) $ coincides with $ w $ in a neighbourhood of 0. Let $ x \in G $. Let $ p $ be the characteristic of the residue field. Then $ p^n x $ tends to 0 as $ n $ tends to $ +\infty $. There therefore exists $ n $ such that $ w(p^n x) = L(w)(p^n x) $. Therefore

$$
p^n w(x) = w(x)^{p^n} = w(x^{p^n}) = w(p^n x)
= L(w)(p^n x) = p^n L(w)(x)
$$

whence $ w(x) = L(w)(x) $. Thus, $ w = L(w)|G $.

Let $ \Gamma $ be the set of $ \gamma \in \mathrm{Aut}\ L(G) $ such that $ \gamma(G) = G $. As G is open and compact in $ L(G) $, $ \Gamma $ is an open subgroup of $ \mathrm{Aut}\ L(G) $. By the above, Aut G is identified with $ \Gamma $, whence there is a Lie group structure on Aut G, with which properties (i), (ii), (iii) and (vi) of Theorem 1 are obvious. Property (v) follows from Propositions 1 and 3 of no. 1.

(c) We pass to the general case. By § 7, no. 1, Proposition 1, there exists an open compact subgroup G_0 of G which is of the type considered in (b). Then G is generated by G_0 and a finite number of elements x_1, x_2, ..., x_n. Let Aut_1G be the set of u ∈ Aut G such that u(G_0) = G_0 and u(x_iG_0) = x_iG_0 for 1 ≤ i ≤ n. We define as in the proof of Theorem 1, part (c), a semi-direct product P of Aut G_0 by G_0^n and an injective homomorphism ζ of Aut_1G into P, whose image is closed in P.

(d), (e): the argument is exactly as in parts (d), (e) of the proof of Theorem 1 with R replaced by Q_p and using Proposition 3 instead of Proposition 2.

#### Remark {#lie-iii-s10-n3-rem-1 .statement}

If K = Q_p, and the Lie group G is generated by a compact subset (cf. Exercise 2), assertions (i), (ii), (iii) and (vi) of Theorem 1 are still true, but not (v) (Exercise 3).

### Exercises {#lie-iii-s10-exercises}

See the [exercises for § 10](exercises/s10/).
