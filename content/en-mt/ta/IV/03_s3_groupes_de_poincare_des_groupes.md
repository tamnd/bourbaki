---
book: ta
book_title: Topologie algébrique
chapter: IV
chapter_title: ESPACES DÉLAÇABLES
section: 3
section_title: Groupes de Poincaré des groupes topologiques
lang: en
source: ta-i-iv-fr
book_pages: TA IV.369-TA IV.382, TA IV.459-TA IV.461
pdf_pages: 0385-0398, 0475-0477
extraction: native
subsections:
    - "no": 1
      title: Prolongement des homomorphismes locaux de groupes
      page: 369
      pdf_page: 385
    - "no": 2
      title: Espaces de Hopf
      page: 373
      pdf_page: 389
    - "no": 3
      title: Groupe de Poincaré des groupes topologiques
      page: 375
      pdf_page: 391
    - "no": 4
      title: Revêtements des groupes topologiques
      page: 375
      pdf_page: 391
    - "no": 5
      title: Revêtement universel d’un groupe topologique délaçable
      page: 379
      pdf_page: 395
statements: 21
exercises: 10
content_sha256: db277372c3e796b13b34997012f2dcc46e40c38ba1cb2d96cac245fe466f7b8f
translated_from: content/fr/ta/IV/03_s3_groupes_de_poincare_des_groupes.md
source_lang: fr
translation_method: machine
source_content_sha256: 1169515dcc48f21c5184d88c376c4b8aa59faa45c9c75be74a8ecf51424e3584
translation_model: gpt-5.4
translation_run: translate-en-mt-7d47dc9a
glossary_version: 34
glossary_terms_sha256: 8e10dff88d24fff59f982950e17e98fed2ff8bb76496b5fddbdc879faa4ab702
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 3. POINCARÉ GROUPS OF TOPOLOGICAL GROUPS

### 1. Extension of local group homomorphisms

#### Definition 1 {#ta-iv-s3-def-1 .statement tag=021M}

Given a topological group G and a group $G'$, a local homomorphism of G into $G'$ means a mapping $f$ of a neighbourhood V of the identity element of G into $G'$ such that, for every pair of points $x,y$ of V such that $xy\in V$, one has $f(xy) =f(x)f(y)$.

If $G'$ is a topological group and if $f$ is a continuous mapping, one says that $f$ is a continuous local homomorphism (or local morphism of topological groups).

If G and $G'$ are topological groups, the notion of local isomorphism of G onto $G'$ has been defined (TG, III, p. 6, Def. 2). A local isomorphism of G onto $G'$ is a homeomorphism $f$ of a neighbourhood V of the identity element of G onto a neighbourhood $V'$ of the identity element of $G'$ such that $f$ and the inverse mapping of $f$ are local homomorphisms.

#### Proposition 1 {#ta-iv-s3-prop-1 .statement tag=021N}

Let G and $G'$ be topological groups and let $p: G\rightarrow G'$ be a group homomorphism. In order that $p$ should make G a covering of $G'$, it is necessary and sufficient that the restriction of $p$ to a suitable neighbourhood of the identity element of G should be a local isomorphism of G onto $G'$.

The condition is necessary by Proposition 3 of TG, III, p. 6. Conversely, suppose that $p$ induces a homeomorphism of an open neighbourhood V of the identity element $e$ of G onto a neighbourhood $V'$ of the identity element of $G'$. The mapping $p$ is then continuous (TG, III, p. 15, Prop. 23) and open (TG, III, p. 16, Prop. 24). The image H of $p$ is a subgroup of $G'$ containing V, hence open and closed in $G'$ (TG, III, p. 7, Corollary). Let N be the kernel of $p$; one has $N\cap V =\{e\}$, therefore N is discrete (loc. cit., Prop. 5). Consequently, $p$ makes G a principal covering of H, with group N (I, p. 100, Cor. 3 of Th. 1). Since H is open and closed in $G'$, the $G'$-space $(G, p)$ is a covering.

#### Proposition 2 {#ta-iv-s3-prop-2 .statement tag=021O}

Let G be a connected topological group, let $G'$ be a group and let $f: V\rightarrow G'$ be a local homomorphism of G into $G'$, where V is a connected neighbourhood of the identity element of G. Then there exist a connected topological group H, a morphism of topological groups $p: H\rightarrow G$ such that $(H, p)$ is a covering of G, and a group homomorphism $\varphi : H\rightarrow G'$ such that the set of $y\in \overset{-1}{p}(V)$ satisfying $f(p(y)) =\varphi (y)$ is a neighbourhood of the identity element in H.

If $G'$ is a topological group and if the mapping $f$ is continuous, such a homomorphism $\varphi$ is continuous.

#### Lemma 1 {#ta-iv-s3-lem-1 .statement tag=021P}

Let G be a topological group and let V be a connected neighbourhood of the identity element $e$ of G. For every neighbourhood U of $e$ in G and every $x\in V$, there exist an integer $n\in \mathbf{N}$ and elements $u_1, . . . , u_n$ in U such that $u_1. . . u_n=x$ and $u_1. . . u_k\in V$ for every integer $k$ such that $1\leqslant k\leqslant n$.

One may suppose that U is open and contained in V. Let A denote the set of $x\in V$ satisfying the condition of the lemma. If $x\in A$ and if $y\in xU\cap V$, then $y\in A$, whence AU $\cap V\subset A$; this shows that A is open in V. Let $x\in V$ be such that $xU^{-1}\cap A=\not\emptyset$; then one has $x\in$ AU$\cap V$, hence $x\in A$. Consequently, if $x\in V$ and $x\notin A,xU^{-1}\cap A =\emptyset$ and A is closed in V. Since $e\in A$ and V is connected, it follows that A = V.

Let us now prove the proposition. Let $j$ be the mapping $g\mapsto$ $(g, f(g))$ of V into $G\times G'$ and let H be the subgroup of $G\times G'$ generated by $j(V)$.

Let U be a neighbourhood of $e$ in G, contained in V. Let $x\in V$; by lemma 1, there exist $u_1, . . . , u_n\in U$ such that $x=u_1. . . u_n$ and such that $u_1. . . u_k\in V$ for every integer $k$ such that $1\leqslant k\leqslant n$. By induction, one has $f(u_1. . . u_k) =f(u_1). . . f(u_k)$ for every integer $k,1\leqslant k\leqslant n$. In particular, $j(x)$ belongs to the subgroup generated by $j(U)$. It follows that H is generated by $j(U)$.

Let $\mathscr{B}$ be the set of subsets of H of the form $j(U)$, where U is a neighbourhood of $e$ in V. Let us show that there exists a unique topology on H, compatible with its group structure, for which $\mathscr{B}$ is a base of the filter of neighbourhoods of the identity element. For this, it is enough to prove that the set $\mathscr{B}$ satisfies conditions (GV$'_I$), (GV$'_{II}$) and (GV$'_{III}$) of III, p. 4.

Let therefore U be a neighbourhood of $e$ in G, contained in V; there exists a neighbourhood $U'$ of $e$ such that $U'\cdot U'\subset U$. For every pair $x, y$ of points of $U'$, one has $xy\in V$ and $f(xy) =f(x)f(y)$. Hence $j(U')\in \mathscr{B}$ and $j(U')\cdot j(U')\subset j(U)$. This shows that condition (GV$'_I$) is satisfied.

The set $U''= V\cap U^{-1}$ is then a neighbourhood of $e$ in V and, for $x\in U''$, one has $x^{-1}\in U$ and $f(x^{-1}) =f(x)^{-1}$. Hence $j(U'')^{-1}\subset j(U)$, which shows condition (GV$'_{II}$).

Finally, let us fix a neighbourhood U of $e$ in V such that $U = U^{-1}$ and $U^3\subset V$. Let W be a neighbourhood of $e$ in U and let $h= (g, f(g))$ be an element of $j(U)$. There exists a neighbourhood $W'$ of $e$ contained in W such that $gW'g^{-1}\subset W$. Then $j(W')\in \mathscr{B}$ and $hj(W')h^{-1}\subset j(W)$, for one has $f(gxg^{-1}) =f(g)f(x)f(g^{-1})$, for $x\in W'$.

Let $h\in H$. Since U is a neighbourhood of $e$ contained in V$,j(U)$ generates H; since U is symmetric, there exist elements $u_1, . . . , u_n$ in U such that $h=j(u_1). . . j(u_n)$. By induction on $n$, there exists a neighbourhood $W'$ of $e$ contained in W such that $hj(W')h^{-1}\subset j(W)$. Consequently, condition (GV$'_{III}$) is satisfied.

Let us then endow the group G with this topology.

Let us denote by $p: H\rightarrow$ G the restriction to H of the first projection $G\times G'\rightarrow G$. This is a group homomorphism. For every neighbourhood U of $e$ contained in V, the set $\overset{-1}{p}(U)$ contains the neighbourhood $j(U)$ of the identity element of H; hence $p$ is a continuous homomorphism of topological groups. For every neighbourhood U of $e$ contained in V, one has $p(j(U)) = U$, hence $p$ is an open mapping. Since G is connected, $p$ is surjective. Its kernel is discrete because it meets $j(V)$ only in the identity element. It then follows from Corollary 3 (I, p. 100) that the G-space $(H, p)$ is a covering.

Let $\varphi$ be the restriction to H of the second projection $G\times G'\rightarrow G'$. If $g\in V$, one has $(g, f(g)) =j(g)\in j(V)$ and $\varphi (g, f(g)) =f(g)$, so that $\varphi (y) =f(p(y))$ for $y\in j(V)$.

Suppose moreover that $G'$ is a topological group and that the mapping $f$ is continuous at $e$. Then the homomorphism $\varphi$ is continuous at the identity element of H, and hence is continuous (TG, III, p. 15, Prop. 23).

#### Corollary 1 {#ta-iv-s3-lem-1-cor-1 .statement tag=021Q}

Let G be a simply connected topological group and let $G'$ be a group. Let V be a connected neighbourhood of the identity element in G and let $f: V\rightarrow G'$ be a local homomorphism. There exists a unique group homomorphism $h: G\rightarrow G'$ extending $f$. If $G'$ is a topological group and if the mapping $f$ is continuous, the homomorphism $h$ is continuous.

The group G is connected. Let H$,\varphi$ and $p$ be as in proposition 2. Since G is simply connected, H is a trivializable covering of G (I, p. 124, def. 3); since H is connected and nonempty, the mapping $p$ is an isomorphism of topological groups. Put $h=\varphi \circ p^{-1}$; the mapping $h$ is a group homomorphism and there exists an open neighbourhood U of the identity element $e$ of G contained in V such that $f|U =h|U$. It follows from lemma 1 that $f$ and $h$ coincide on V. In other words, the mapping $h$ extends the mapping $f$.

If $G'$ is a topological group and if the mapping $f$ is continuous, the homomorphism $\varphi$ is continuous, hence so is $h$.

Let us prove the uniqueness of such an extension. The set of points of G where two homomorphisms of G into $G'$ coincide is a subgroup of G. Since the group G is connected, every subgroup of G containing a neighbourhood of the identity element is equal to G (TG, III, p. 8, prop. 6). The uniqueness of $h$ follows.

#### Remark 1 {#ta-iv-s3-n1-rem-1 .statement tag=021R}

When $G =\mathbf{R}$, this corollary follows from proposition 6 of TG, V, p. 3.

#### Corollary 2 {#ta-iv-s3-lem-1-cor-2 .statement tag=021S}

Two locally connected and simply connected topological groups which are locally isomorphic are isomorphic.

Let G and $G'$ be locally connected topological groups, let V and $V'$ be connected neighbourhoods of the identity element of G and of $G'$ respectively, and let $f: V\rightarrow V'$ be a homeomorphism which is a local isomorphism of G onto $G'$. By corollary 1, there exists a unique continuous group homomorphism $\varphi : G\rightarrow G'$ extending $f$ and a unique continuous group homomorphism $\varphi ': G'\rightarrow$ G extending $f^{-1}$. The homomorphisms $\varphi '\circ \varphi$ and Id$_G$ coincide on a neighbourhood of $e$ in G, hence are equal, since G is connected. Analogously, $\varphi \circ \varphi '=$ Id$_{G'}$, whence the corollary.

#### Corollary 3 {#ta-iv-s3-lem-1-cor-3 .statement tag=021T}

Let G be a simply connected topological group and let V be a connected neighbourhood of the identity element of G. One defines a presentation of G by taking as generator set the set V and as set $\mathbf{r}$ of relations the family of the $xyz^{-1}$, where $(x, y, z)$ runs through the triples of elements of V such that $xy=z$.

Let $F(V,\mathbf{r})$ be the quotient group of the free group F(V) by the smallest normal subgroup containing the elements $xyz^{-1}$, where $(x, y, z)\in V\times$ $V\times V$ and $xy=z$ (A, I, p. 86). Let us denote by $f: V\rightarrow F(V,\mathbf{r})$ and $g: F(V,\mathbf{r})\rightarrow G$ the canonical mappings. By construction, the mapping $f$ is a local homomorphism of G into $F(V,\mathbf{r})$. By corollary 1, there exists a unique group homomorphism $\overline{f}: G\rightarrow F(V,\mathbf{r})$ extending $f$. Since the group $F(V,\mathbf{r})$ is generated by $f(V)$, the homomorphism $\overline{f}$ is surjective. For $x\in V$, one has $g(\overline{f}(x)) =g(f(x)) =x$; since V generates G$,g\circ \overline{f}=$ Id$_G$, which proves that $\overline{f}$ is injective. It is therefore an isomorphism.

### 2. Hopf Spaces

#### Definition 2 {#ta-iv-s3-def-2 .statement tag=021U}

A pointed topological space $(X, e)$ endowed with a continuous law of composition $m: X\times X\rightarrow X$ is called a Hopf space, such that

(i) $m(e, e) =e$;

(ii) there exist homotopies pointed at $e$ connecting the mappings $x\mapsto m(x, e)$ and $x\mapsto m(e, x)$ with the mapping Id$_X$.

Properties (i) and (ii) are sometimes expressed by saying that $e$ is an identity element up to homotopy for the composition law $m$.

It should be noted that there may exist several identity elements up to homotopy for a continuous composition law $m$ on a topological space X. For example, for $X =\mathbf{R}$ and $m(x, y) = (x+y)/2$, every $x\in \mathbf{R}$ is an identity element up to homotopy.

#### Example 1 {#ta-iv-s3-n2-exa-1 .statement tag=021V}

Let G be a topological group and $m$ its composition law. The identity element $e$ of G is an identity element up to homotopy and $(G, e)$ is a Hopf space.

#### Example 2 {#ta-iv-s3-n2-exa-2 .statement tag=021W}

Let X be a topological space and $x$ a point of X. Endowed with the juxtaposition of loops at $x$, the pointed space $(\Omega_x(X), e_x)$ is a Hopf space. In fact, first one has $e_x*e_x=e_x$. On the other hand, let $\psi :\mathbf{I}\rightarrow \mathbf{I}$ be the function defined by $\psi (t) = 2t$ for $0\leqslant t\leqslant \frac{1}{2}$ and $\psi (t) = 1$ for $\frac{1}{2}\leqslant t\leqslant 1$ (cf. III, p. 291), and let $\sigma :\mathbf{I}\times \mathbf{I}\rightarrow \mathbf{I}$ be a strict homotopy connecting $\psi$ with Id$_{\mathbf{I}}($III, p. 289, example). Then, for every loop $c\in \Omega_x(X)$, the mapping $c\circ \sigma :\mathbf{I}\times \mathbf{I}\rightarrow X$ is a strict homotopy connecting $c*e_x$ with $c$ in $\Omega_x(X)$.

Let $\tau$ be the mapping $\Omega_x(X)\times \mathbf{I}\rightarrow \Omega_x(X)$ defined by $\tau (c, s)(t) =$ $c\circ \sigma (s, t)$. Let us now prove that $\tau$ is continuous. By proposition 1 of III, p. 257, it is enough to show that the mapping $(c, s, t)\mapsto c(\sigma (s, t))$ of $\Omega_x(X)\times \mathbf{I}\times \mathbf{I}$ into X is continuous, or again, since $\mathbf{I}\times \mathbf{I}$ is compact, that the mapping $c\mapsto c\circ \sigma$ of $\mathscr{C}_c(\mathbf{I}; X)$ into $\mathscr{C}_c(\mathbf{I}\times \mathbf{I}; X)$ is continuous. This last assertion then follows from the lemma, I, p. 132, b). Hence the mapping $\tau$ is a homotopy connecting the mapping $c\mapsto c*e_x$ with the identity mapping of $\Omega_x(X)$. One has $\tau (e_x, s)(t) =x$ for all $s,t\in \mathbf{I}$; therefore $\tau$ is a homotopy pointed at $e_x$. One reasons analogously for the mapping $c\mapsto e_x*c$.

#### Proposition 3 {#ta-iv-s3-prop-3 .statement tag=021X}

Let $(X, e)$ be a Hopf space and $m: X\times X\rightarrow X$ its composition law. For any loops $c,c'$ of X at $e$, one has:

$$
c'*c\sim c*c'\sim m\circ (c, c')
$$

where $\sim$ denotes the relation of strict homotopy. The law of composition of the group $\pi_1(X, e)$ is the homomorphism obtained by composing the canonical isomorphism $\pi_1(X, e)\times \pi_1(X, e)\rightarrow \pi_1(X\times X,(e, e))$ (III, p. 297, corollary) and the homomorphism $\pi_1(m,(e, e))$ of $\pi_1(X\times X,(e, e))$ into $\pi_1(X, e)$. The group $\pi_1(X, e)$ is commutative.

Let $\mu:\pi_1(X, e)\times \pi_1(X, e)\rightarrow \pi_1(X, e)$ be the group homomorphism obtained by composing the canonical isomorphism of $\pi_1(X, e)\times \pi_1(X, e)$ onto $\pi_1(X\times$ $X,(e, e))$ and the homomorphism $\pi_1(m,(e, e))$. It is to be proved that one has

$$
\mu(\gamma , \gamma ') =\gamma \gamma '=\gamma '\gamma \tag{1}
$$

for all $\gamma ,\gamma '\in \pi_1(X, e)$. Taking account of Remark 2 of III, p. 297, one has:

$$
\mu(\gamma , \gamma ') =\mu(\gamma , \varepsilon_e)\mu(\varepsilon_e, \gamma ') =\mu(\varepsilon_e, \gamma ')\mu(\gamma , \varepsilon_e) \tag{2}
$$

Let $c\in \Omega_e(X)$ be a loop of class $\gamma$; let us denote by $m_1: X\rightarrow X$ the mapping defined by $m_1(x) =m(x, e)$; then $\mu(\gamma , \varepsilon_e)$ is the class of $m_1\circ c$. By definition of a Hopf space, the mappings pointed at $e$, $m_1$ and Id$_X$, have the same pointed homotopy class at $e$. Hence the loops at $e$, $m_1\circ c$ and $c$, are strictly homotopic (III, p. 296, Cor. 1 of Prop. 3) and one has $\mu(\gamma , \varepsilon_e) =\gamma$. One proves analogously that one has $\mu(\varepsilon_e, \gamma ') =\gamma '$. Relation (1) then follows from relation (2).

#### Remark {#ta-iv-s3-n2-rem-1 .statement tag=021Y}

Let $(X, e)$ be a Hopf space. By Prop. 3, the mapping of composition of path classes, $\pi_1(X, e)\times \pi_1(X, e)\rightarrow$ $\pi_1(X, e)$ is continuous if $\pi_1(X, e)$ is endowed with the quotient topology of the topology of compact convergence on $\Lambda_e(X)$. It is in fact the composite of the continuous isomorphism $\pi_1(X, e)\times \pi_1(X, e)\rightarrow \pi_1(X\times X,(e, e))$ (III, p. 298, Remark 3) and the continuous mapping $m_*:\pi_1(X\times X,(e, e))\rightarrow$ $\pi_1(X, e)$ (III, p. 294, Remark 1).

### 3. Poincaré Group of Topological Groups

If G is a topological group, for every $g\in G$, the left translation $x\mapsto gx$ is a homeomorphism of G onto itself (TG, III, p. 2) and it induces an isomorphism of $\pi_1(G, e)$ onto $\pi_1(G, g)$.

Let G be a topological group, let $e$ be its identity element and let us denote by $G_0$ the path-connected component of $e$ in G. Let us denote by R the equivalence relation in G whose equivalence classes are the path-connected components of G, and let $p: G\rightarrow \pi_0(G)$ be the canonical mapping. Since every translation, on the left or on the right, is a homeomorphism of G, the relation R is compatible on the left and on the right with the group law of G. By Th. 2 of A, I, p. 35, the group $G_0$ is a normal subgroup of G, the quotient group $G/G_0$ is equal to $\pi_0(G)$ endowed with the quotient law of composition induced by that of G, and the mapping $p$ is a group homomorphism.

The group $\pi_1(G, e)$ is called the Poincaré group of G, and is denoted by $\pi_1(G)$. The canonical injection of $G_0$ into G induces an isomorphism of $\pi_1(G_0)$ onto $\pi_1(G)$ (III, p. 293, Remark 2).

Let $g$ be an element of G; the right translation $\boldsymbol{\delta }_g:x\mapsto xg$ induces an isomorphism $(\boldsymbol{\delta }_g)_*:\pi_1(G)\rightarrow \pi_1(G, g)$. Suppose that $g$ belongs to $G_0$ and let $b$ be a path joining $e$ to $g$. The mapping $\sigma : G\times \mathbf{I}\rightarrow G$ defined by $\sigma (x, t) =xb(t)$ is a homotopy joining Id$_G$ to $\boldsymbol{\delta }_g$. By prop. 3 of III, p. 295, one therefore has, for every $\alpha \in \pi_1(G)$, $(\boldsymbol{\delta }_g)_*(\alpha ) =$ $\beta^{-1}\alpha \beta$, where $\beta \in \varpi_{e,g}(G)$ is the class of the path $b$. If $\boldsymbol{\gamma }_g$ denotes the left translation, $x\mapsto gx$, one has analogously $(\boldsymbol{\gamma }_g)_*(\alpha ) =\beta^{-1}\alpha \beta$.

For every $g\in G$, the mapping Int($g$)$: G\rightarrow G$ induces an automorphism $\pi_1$(Int($g$)) of $\pi_1(G)$. One thus defines a law of operation of G on $\pi_1(G)$. For every $g\in G$, one has $\pi_1$(Int($g$)) $= (\boldsymbol{\gamma }_{g^{-1}})_*\circ (\boldsymbol{\delta }_g)_*$, so that the subgroup $G_0$ operates trivially; it follows that there is a law of operation of $\pi_0(G)$ on $\pi_1(G)$. When G is a commutative group, this operation is trivial, but this is not always the case (IV, p. 459, exerc. 1).

### 4. Coverings of Topological Groups

#### Proposition 4 {#ta-iv-s3-prop-4 .statement tag=021Z}

Let $(X, e)$ be a Hopf space (IV, p. 373, definition 2) and let $m: X\times X\rightarrow X$ be its law of composition. Assume that the space X is connected and locally arcwise connected. Let $X'$ be a connected covering of X; let $p$ denote its projection and let $e'$ be a point of the fibre $X'_e$.

a) The covering $X'$ is Galois and the group of its automorphisms is commutative.

b) There exists a continuous law of composition $m': X'\times X'\rightarrow X'$ and only one such that one has $p\circ m'=m\circ (p, p)$ and $m'(e', e') =e'$. Endowed with this law of composition, the pointed space $(X', e')$ is a Hopf space.

c) Endowed with the law of composition induced by $m'$, the fibre $X'_e$ is a group with identity element $e'$. The mapping of $\pi_1(X, x)$ into $X'_e$ given by $\gamma \mapsto e'\cdot \gamma$ is a surjective group homomorphism with kernel $p_*(\pi_1(X', e'))$. The mapping $g\mapsto g(e')$ is an isomorphism of the group Aut$_X(X')$ onto the group $X'_e$.

a) The group $\pi_1(X, e)$ is commutative (prop. 3). Since the covering $X'$ of X is connected, it is then a Galois covering and the group Aut$_X(X')$ is isomorphic to the quotient group $\pi_1(X, e)/p_*(\pi_1(X', e'))$ (III, p. 312, corollary 4 to proposition 2); this group is commutative.

b) Let us denote by $q: X'\times X'\rightarrow X$ the mapping $m\circ (p, p)$. The required mapping $m'$ is a continuous lifting of $q$ to $X'$ such that $m'(e', e') =e'$. The space $X'\times X'$ is locally arcwise connected; it is therefore enough, in order to prove the existence of such a continuous lifting, to verify that $q_*(\pi_1(X'\times X',(e', e')))$ is contained in $p_*(\pi_1(X', e'))$ (III, p. 308, prop. 1). By prop. 3, the mapping $\pi_1(m,(e, e))$ identifies with the law of composition of the group $\pi_1(X, e)$ when one identifies $\pi_1(X\times X,(e, e))$ with $\pi_1(X, e)\times \pi_1(X, e)$. The group $q_*(\pi_1(X'\times X',(e', e')))$ is therefore equal to the group $p_*(\pi_1(X', e'))$, whence the existence of $m'$. Since $X'\times X'$ is connected, the uniqueness of $m'$ follows from I, p. 34, corollary 1 of prop. 11.

Let us prove that the mapping $m'$ endows the pointed space $(X', e')$ with a structure of Hopf space. Let $m_1: X\rightarrow X$ be the mapping $g\mapsto m(g, e)$ and let $\sigma_1: X\times \mathbf{I}\rightarrow X$ be a homotopy pointed at $x$ joining $m_1$ to Id$_X$. Put $\tau =\sigma_1\circ (p$, Id$_{\mathbf{I}}): X'\times \mathbf{I}\rightarrow X$. The mapping $m'_1: X'\rightarrow X'$ defined by $h\mapsto m'(h, e')$ lifts the mapping $\tau (\cdot ,0)$; let $\tau ': X'\times \mathbf{I}\rightarrow X'$ be the lifting of $\tau$ which is a homotopy with origin $m'_1($III, p. 301, prop. 2). The mapping $t\mapsto \tau '(e', t)$ is a lifting to $X'$ of the constant mapping $t\mapsto e$; since $\tau '(e',0) =e'$, we therefore have $\tau '(e', t) =e'$ for every $t\in \mathbf{I}$. The mapping $\tau '(\cdot ,1)$ is then a lifting to $X'$ of the mapping $p$ which maps $e'$ to $e'$. Since $X'$ is connected, Id$_{X'}$ is the unique X-morphism of $X'$ into itself which fixes the point $e'$; we therefore have $\tau '(\cdot ,1) =$ Id$_{X'}$. This shows that $\tau '$ is a homotopy pointed at $e'$ which joins the mapping $m'_1$ to the mapping Id$_{X'}$. Analogously, there exists a homotopy pointed at $e'$ joining the mapping $m'_2:h\mapsto m'(e', h)$ to the mapping Id$_{X'}$. This proves that the pointed space $(X', e')$, endowed with the law of composition $m'$, is a Hopf space.

c) Since $X'$ is a connected covering of X, the orbital mapping of $e'$ induced by the operation of $\pi_1(X, e)$ on $X'_e$ is surjective and induces a bijection of $\pi_1(X, e)/p_*(\pi_1(X', e'))$ onto $X'_e($III, p. 305, Theorem 1).

Let $c$ and $d$ be loops in X at $e$, and let $\gamma$ and $\delta \in \pi_1(X, e)$ be their classes. Let $c'$ and $d'$ be the paths with origin $e'$ in $X'$ which lift $c$ and $d$. We have $e'\cdot \gamma =c'(1)$ and $e'\cdot \delta =d'(1)$ (III, p. 304). By Proposition 3 of IV, p. 374, the loop $m\circ (c, d)$ is strictly homotopic to the loop $c*d$; hence we have $e'\cdot (\gamma \delta ) =e'\cdot (m\circ (c, d))$. Now, the path $m'\circ (c', d')$ is a lift with origin $e'$ of the path $m\circ (c, d)$; hence we have

$$
e'\cdot (\gamma \delta ) =m'(c'(1), d'(1)) =m'(e'\cdot \gamma , e'\cdot \delta )
$$

The mapping $\gamma \mapsto e'\cdot \gamma$ is therefore a group homomorphism of $\pi_1(X, e)$ into the set $X'_e$ endowed with the law of composition induced by $m'$. Consequently, $X'_e$ is a group for the law of composition induced by $m'$, and the orbital mapping of $e'$ is an isomorphism of the quotient group $\pi_1(X, e)/p_*(\pi_1(X', e'))$ onto $X'_e$.

The last part of assertion c) then results from Corollary 3 of III, p. 311.

#### Proposition 5 {#ta-iv-s3-prop-5 .statement tag=0220}

Let us keep the notation and the hypotheses of Proposition 4.

a) If $m$ is an associative ( resp. commutative) law of composition, the same is true of $m'$.

b) If $e$ is a right-hand ( resp. left-hand) identity element for the law $m$, then $e'$ is a right-hand ( resp. left-hand) identity element for the law $m'$.

c) If X is a topological group, $m$ its law of composition and $e$ its identity element, the law of composition $m'$ endows $X'$ with a group structure compatible with the topology of $X'$, of which $e'$ is the identity element. The mapping $p: X'\rightarrow X$ is a group homomorphism whose kernel is discrete and contained in the center of $X'$.

a) Suppose that the law $m$ is associative. Then the mappings from $X'\times X'\times X'$ into X which map $(h_1, h_2, h_3)$ to $m(p(h_1), m(p(h_2), p(h_3)))$ and $m(m(p(h_1), p(h_2)), p(h_3))$ respectively are equal. The mappings $(h_1, h_2, h_3)\mapsto m'(h_1, m'(h_2, h_3))$ and $(h_1, h_2, h_3)\mapsto m'(m'(h_1, h_2), h_3)$ from $X'\times X'\times X'$ into $X'$ are continuous liftings of them which coincide at the point $(e', e', e')$. Since $X'\times X'\times X'$ is connected, they are equal (I, p. 34, Corollary 1 of Prop. 11), which shows that the law $m'$ is associative.

Suppose now that the law $m$ is commutative; the mappings $(h_1, h_2)\mapsto m'(h_1, h_2)$ and $(h_1, h_2)\mapsto m'(h_2, h_1)$ are continuous liftings to $X'$ of the mapping $(h_1, h_2)\mapsto m(p(h_1), p(h_2))$ which coincide at the point $(e', e')$. Since $X'\times X'$ is connected, they are equal (loc. cit.) and the law $m'$ is commutative.

If $e$ is a right (resp. left) identity element for the law $m$, the mapping $h\mapsto m'(h, e')$ (resp. $h\mapsto m'(e', h)$) from $X'$ into $X'$ is an X-morphism of coverings which coincides with Id$_{X'}$ at the point $e'$, hence at every point of $X'$, since $X'$ is connected (loc. cit.), whence b).

Let us finally prove c). Suppose that X is a topological group. From the foregoing, the law $m'$ is associative and $e'$ is an identity element for it. Let $i: X\rightarrow X$ denote the mapping $g\mapsto g^{-1}$. It is continuous (TG, III, p. 1) and the homomorphism $\pi_1(i, e):\pi_1(X, e)\rightarrow \pi_1(X, e)$ is none other than the mapping $\gamma \mapsto \gamma^{-1}($IV, p. 374, prop. 3). Consequently, the subgroup $(i\circ p)_*(\pi_1(X', e'))$ is equal to $p_*(\pi_1(X', e'))$. By prop. 1 of III, p. 308, there therefore exists a continuous mapping $i': X'\rightarrow X'$ such that $p\circ i'=i\circ p$ and $i'(e') =e'$. The mappings $h\mapsto m'(h, i'(h))$ and $h\mapsto$ $m'(i'(h), h)$ of $X'$ into $X'$ are liftings to $X'$ of the constant mapping with image $e$ of $X'$ into X. They are therefore constant and their image is $e'=m'(e', e')$. Thus every element $h$ of $X'$ is invertible, with inverse $i'(h)$, which shows that $X'$, endowed with the composition law $m'$, is a group. By construction of the law $m'$, the mapping $p: X'\rightarrow X$ is a group homomorphism. Since the mappings $m'$ and $i'$ are continuous, the group structure of $X'$ is compatible with its topology (TG, III, p. 1). The fibre $\overset{-1}{p}(e)$ is a discrete subgroup of $X'$ which is contained in the center of $X'($I, p. 100, cor. 3) and X is isomorphic to the quotient topological group $X'/\overset{-1}{p}(e)$.

#### Corollary {#ta-iv-s3-n4-cor-1 .statement tag=0221}

Let G be a connected topological group and locally connected by arcs. Let $G'$ be a connected covering of G, let $p$ be its projection and let $e'$ be an element of the fibre N of the identity element $e$ of G. Endow $G'$ with the unique continuous composition law $m': G'\times G'\rightarrow G'$ such that $p\circ m'=m\circ (p, p)$ and $m'(e', e') =e'$. If $i: N\rightarrow G'$ denotes the canonical injection, $(G', p, i)$ is a central extension of G by N (A, I, p. 63).

### 5. Universal covering of a coverable topological group

Let G be a topological group locally connected by arcs. The translations of G are homeomorphisms (TG, III, p. 2). In order that the space G be coverable (IV, p. 340, def. 2), it is necessary and sufficient that G possess the following property:

There exists a neighbourhood V of the identity element $e$ of G such that the image of the homomorphism from $\pi_1(V, e)$ into $\pi_1(G, e)$ deduced from the canonical injection is reduced to the identity element.

#### Proposition 6 {#ta-iv-s3-prop-6 .statement tag=0222}

Let G be a connected and coverable topological group. There exist a topological group $\widetilde{G}$, with identity element $\widetilde{e}$, and a continuous homomorphism $p:\widetilde{G}\rightarrow G$ satisfying the following assertions:

a) The space $\widetilde{G}$ is simply connected and simply connected by arcs. Endowed with the mapping $p$, the pointed space $(\widetilde{G},\widetilde{e})$ is a universal covering of the pointed space $(G, e)$.

(b) The kernel N of $p$ is a discrete subgroup of $\widetilde{G}$, contained in the center of $\widetilde{G}$. The group homomorphism $N\rightarrow$ Aut$_G(\widetilde{G})$ which, to $n\in N$, associates the right translation in $\widetilde{G}$, is a group isomorphism. The homomorphism of $\pi_1(G)$ into N which, to $\gamma \in \pi_1(G)$, associates the unique element $n$ of N such that $\widetilde{e}\cdot \gamma =n$, is a group isomorphism.

(c) If $G'$ is a topological group, with identity element $e'$, and if $p': G'\rightarrow$ G is a group homomorphism which makes $G'$ into a covering of G, the unique continuous mapping $u:\widetilde{G}\rightarrow G'$ such that $u(\widetilde{e}) =e'$ and $p'\circ u=p$ is a group homomorphism. Endowed with the mapping $u,(\widetilde{G},\widetilde{e})$ is a universal covering of $(G', e')$.

By IV, p. 342, Theorem 1, there exists a covering $(\widetilde{G}, p)$ of G, simply connected and simply connected by arcs, Galoisian with group $\pi_1(G)^{\circ}$, and a point $\widetilde{e}$ of $\overset{-1}{p}(e)$ such that the pointed covering $(\widetilde{G},\widetilde{e})$ is a universal covering of $(G, e)$.

By IV, p. 375, Prop. 4 and IV, p. 377, Prop. 5, there exists on the space $\widetilde{G}$ a unique group structure compatible with its topology for which $p$ is a group homomorphism and $\widetilde{e}$ an identity element. It follows from Prop. 4 that the group $\widetilde{G}$ satisfies assertions (a) and (b).

Let us prove assertion (c). Let $G'$ be a topological group and let $p': G'\rightarrow G$ be a group homomorphism which makes $G'$ into a covering of G. Let $e'$ be the identity element of $G'$. The existence and uniqueness of a mapping $u:\widetilde{G}\rightarrow G'$ such that $p=p'\circ u$ and $u(\widetilde{e}) =e'$ follow from the fact that $(\widetilde{G},\widetilde{e})$ is a universal covering of the pointed space $(G, e)$. Since the mappings $p$ and $p'$ are surjective group homomorphisms, $u$ is a group homomorphism. Endowed with the mapping $u,\widetilde{G}$ is a covering of $G'($I, p. 81, Prop. 7), hence $(\widetilde{G},\widetilde{e})$ is a universal covering of $(G', e')$ (IV, p. 345, Cor. 2 of Theorem 1).

Under the hypotheses of the proposition, we shall say, by abuse, that $\widetilde{G}$ is a universal covering of G.

#### Example {#ta-iv-s3-n5-exa-1 .statement tag=0223}

Proposition 6 applies in particular when G is a connected Lie group over $\mathbf{R}$ or $\mathbf{C}$. There then exists on $\widetilde{G}$ a unique structure of analytic manifold such that the projection $p:\widetilde{G}\rightarrow G$ is an étale morphism of analytic manifolds (VAR R, §1, 5.8.2, p. 48). For this manifold structure, $\widetilde{G}$ is a Lie group (LIE, III, p. 113, corollary).

#### Scholium {#ta-iv-s3-n5-sch-1 .statement tag=0224}

Let G be a connected and unknottable topological group, let $e$ be its identity element. Let $\widetilde{G}$ be a topological group simply connected by arcs, with identity element $\widetilde{e}$, and $p:\widetilde{G}\rightarrow G$ a group homomorphism which makes $\widetilde{G}$ into a universal covering of G. Let us denote by N the kernel of $p$.

The right translation $\boldsymbol{\delta }_h$ (resp. the left translation) by an element $h\in N$ is a G-automorphism of the principal covering $\widetilde{G}$, and the mapping $h\mapsto \boldsymbol{\delta }_h$ is an isomorphism of the group N onto the automorphism group of this principal covering.

For every subgroup K of N, the mapping $p':\widetilde{G}/K\rightarrow$ G deduced from $p$ is a Galois covering of G, and Aut$_G(G/K)$ is identified with the group $N/K$. When, as above, the groups N and $\pi_1(G)$ are identified, the group $p'_*(\pi_1(\widetilde{G}/K))$ is identified with the subgroup K of N. Moreover, $\widetilde{G}$ is a covering of $\widetilde{G}/K$, because G is locally connected (I, p. 81, prop. 7).

Conversely, every nonempty connected covering E of G is G-isomorphic to a covering of this type (I, p. 113, th. 3 and I, p. 111, prop. 10). Consider in fact a point $x$ of the fibre $E_e$ and let $f$ be the unique homomorphism of $\widetilde{G}$ into E which maps $\widetilde{e}$ to $x$. Endowed with $f,\widetilde{G}$ is a Galois covering of E; the subgroup Aut$_E(\widetilde{G})$ of Aut$_G(\widetilde{G})$ is identified with $f^{-1}(x)$ and is therefore a subgroup of N. It follows that $f$ induces a G-isomorphism of $\widetilde{G}/f^{-1}(x)$ onto E. By transport of structure, there results a topological group structure on E for which $x$ is the identity element and for which the mapping $f$ is a surjective homomorphism. The projection of the G-space E is then a group homomorphism, and the composition law of E is therefore the composition law defined by prop. 4 of IV, p. 375.

Let $(E, q)$ and $(E', q')$ be connected coverings of G, let $x$ be a point of $E_e$ and $x'$ a point of $E'_e$. In order that there exist a G-morphism of E into $E'$, it is necessary and sufficient that $p_*(\pi_1(E, x))$ be contained in $p'_*(\pi_1(E', x'))$. If this condition is satisfied, there then exists a unique G-morphism $f: E\rightarrow E'$ such that $g(x) =x'($III, p. 311, cor. 2 of prop. 1). If E and $E'$ are endowed with the group composition laws for which $q$ and $q'$ are homomorphisms and $x$ and $x'$ identity elements, the mapping $g$ is a group homomorphism. In fact, $g$ is identified with the canonical homomorphism $\widetilde{G}/p_*(\pi_1(E, x))\rightarrow$ $\widetilde{G}/p'_*(\pi_1(E', x'))$.

#### Proposition 7 {#ta-iv-s3-prop-7 .statement tag=0225}

In order that two connected unrollable topological groups be locally isomorphic, it is necessary and sufficient that their universal coverings be isomorphic topological groups.

A connected unrollable topological group is locally isomorphic to its universal covering (IV, p. 369, prop. 1); the condition is therefore sufficient. It is necessary by corollary 2 of proposition 2 (IV, p. 372), since the universal covering of a connected unrollable topological group is simply connected (IV, p. 379, prop. 6).

#### Proposition 8 {#ta-iv-s3-prop-8 .statement tag=0226}

Let G be a connected unrollable topological group and let $\widetilde{G}$ be a universal covering of G. Let V be a connected open neighbourhood of the identity element $e$ of G such that the image of the canonical homomorphism of $\pi_1(V\cdot V, e)$ into $\pi_1(G, e)$ is reduced to the identity element. Let $F(V,\mathbf{r})$ denote the group defined by the generating set V and by the set $\mathbf{r}$ of relators $xyz^{-1}$, where $(x, y, z)$ runs through the set of elements of $V\times V\times V$ such that $xy=z$. Let $j: V\rightarrow F(V,\mathbf{r})$ denote the canonical mapping.

There exists a unique isomorphism $f$ of the group $F(V,\mathbf{r})$ onto $\widetilde{G}$ such that $f\circ j$ is a lifting to $\widetilde{G}$ of the canonical injection of V into G.

The set $V\cdot V$ is connected and open, hence locally arcwise connected. Let $p$ be the projection of $\widetilde{G}$. There exists a continuous section $s$ of $p$ over $V\cdot V$ such that $s(e) =\widetilde{e}$, where $\widetilde{e}$ denotes the identity element of $\widetilde{G}($III, p. 308, prop. 1). Put $\widetilde{V} =s(V)$; the set $\widetilde{V}$ is a connected open neighbourhood of $\widetilde{e}$ in $\widetilde{G}$, and $s$ is a homeomorphism of $V\cdot V$ onto $\widetilde{V}\cdot \widetilde{V}$. The mappings $(x, y)\mapsto s(x)s(y)$ and $(x, y)\mapsto s(xy)$ are liftings to $\widetilde{G}$ of the mapping $(x, y)\mapsto xy$ of $V\times V$ into G which coincide at $(e, e)$; since $V\times V$ is connected, they coincide on $V\times V$ (I, p. 34, cor. 1). Moreover, if $(\widetilde{x},\widetilde{y},\widetilde{z})\in \widetilde{V}\times \widetilde{V}\times \widetilde{V}$, the conditions $\widetilde{x}\widetilde{y}=\widetilde{z}$ and $p(\widetilde{x})p(\widetilde{y}) =p(\widetilde{z})$ are equivalent. The existence of an isomorphism $f: F(V,\mathbf{r})\rightarrow \widetilde{G}$ then follows from corollary 3 (IV, p. 372) of proposition 2.

Let $g$ be an isomorphism of $F(V,\mathbf{r})$ satisfying the conditions of the proposition. The equality $e\cdot e=e$ implies that $eee^{-1}\in \mathbf{r}$, so that $j(e)$ is the identity element of $F(V,\mathbf{r})$. Since V is connected, $g\circ j$ is the unique continuous lifting to $\widetilde{G}$ of the canonical injection of V into G. Consequently, $f$ and $g$ coincide on $j(V)$. Since $j(V)$ generates the group $F(V,\mathbf{r})$, $f=g$.

## EXERCISES {#ta-iv-s3-exercises}

See the [exercises for § 3](exercises/s3/).
