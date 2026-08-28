---
book: ta
book_title: Topologie algébrique
chapter: II
chapter_title: GROUPOÏDES
section: 3
section_title: Groupoïdes
lang: en
source: ta-i-iv-fr
book_pages: TA II.159-TA II.179, TA II.223-TA II.227
pdf_pages: 0175-0195, 0239-0243
extraction: native
subsections:
    - "no": 1
      title: Catégories
      page: 159
      pdf_page: 175
    - "no": 2
      title: Foncteurs
      page: 161
      pdf_page: 177
    - "no": 3
      title: Groupoïdes
      page: 162
      pdf_page: 178
    - "no": 4
      title: Orbites d’un groupoïde
      page: 162
      pdf_page: 178
    - "no": 5
      title: Exemples de groupoïdes
      page: 163
      pdf_page: 179
    - "no": 6
      title: Sous-groupoïdes
      page: 164
      pdf_page: 180
    - "no": 7
      title: Opérations d’un groupoïde
      page: 167
      pdf_page: 183
    - "no": 8
      title: Sous-groupoïdes distingués ; quotients de groupoïdes
      page: 168
      pdf_page: 184
    - "no": 9
      title: Groupoïde des classes de chemins d’un graphe
      page: 171
      pdf_page: 187
    - "no": 10
      title: Groupoïdes libres
      page: 174
      pdf_page: 190
    - "no": 11
      title: Contraction de flèches d’un groupoïde
      page: 175
      pdf_page: 191
    - "no": 12
      title: Groupe de Poincaré d’un graphe
      page: 178
      pdf_page: 194
statements: 40
exercises: 12
content_sha256: edbca22829fbf6d3252d8d0fe702290bb710700d90133cb8833f67e30b2d8f37
translated_from: content/fr/ta/II/03_s3_groupoides.md
source_lang: fr
translation_method: machine
source_content_sha256: 2be663e4fa5a1975e93b6923e713d80ef48c42134455ee9a9d72b45e4888dd98
translation_model: gpt-5.4
translation_run: translate-en-mt-ae9dec28
glossary_version: 34
glossary_terms_sha256: 0fa6a7928dd974ba673e7a92a8695ec134d9b3c41a6adae8a7e3b67f662682ea
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 3. GROUPOIDS

### 1. Categories

#### Definition 1 {#ta-ii-s3-def-1 .statement tag=01SZ}

Let C be a quiver. Let J denote the set of pairs $(f, g)$ of arrows of C such that $t(f) =o(g)$. A law of composition in C is a mapping $m: J\rightarrow$ Fl(C) such that, for every pair $(f, g)\in J$, the origin of the arrow $m(f, g)$ is that of $f$ and its end that of $g$.

Let C be a quiver endowed with a law of composition $m$. Two arrows $f$ and $g$ such that $t(f) =o(g)$ are said to be composable; the arrow $m(f, g)$ is called their composite, or their product, and is often denoted by $f\cdot g$, or even by $f g$.

For every vertex $a$ of C, the set $C_{a,a}$ = Fl$_{a,a}(C)$, endowed with the mapping deduced from $m$ by passing to subsets, is a magma (A, I, p. 1, Def. 1).

One says that a family $(f_i)_{i\in I}$ of arrows of C, indexed by a finite nonempty totally ordered set I, is composable if, for every pair $(i, j)$ of consecutive elements of I, the arrows $f_i$ and $f_j$ are composable. The product $\prod_{i\in I}f_i$ of such a family is defined by induction on the cardinal of I in the following way (cf. A, I, p. 3):

(i) if I has a single element $\omega ,\prod_{i\in I}f_i=f_{\omega}$;

(ii) if I has at least two elements and if $\omega$ is the smallest element of I, one sets $\prod_{i\in I}f_i=f_{\omega}\cdot \prod_{i\in I-\{\omega\}}f_i$.

The law of composition $m$ is said to be associative if one has $f\cdot (g\cdot h) =$ $(f\cdot g)\cdot h$ for every composable triple $(f, g, h)$ of arrows of C. When the law $m$ is associative, the product of a sequence $(f_1, . . . , f_n)$ of $n$ composable arrows, where $n$ is an integer $\geqslant 1$, is denoted by $f_1f_2. . . f_n$.

Let $a$ be a vertex of C. One says that an arrow $e\in C_{a,a}$ is an identity element of $m$ at $a$ if one has $ef=f$ for every arrow $f$ with origin $a$ and $ge=g$ for every arrow $g$ with end $a$. There exists at most one identity element of $m$ at $a:$ if $e$ and $e'$ are two such elements, one has $e'=ee'=e$. When such an identity element exists, it is often denoted by $e_a$; it is then an identity element of the magma $C_{a,a}$ (A, I, p. 12).

#### Definition 2 {#ta-ii-s3-def-2 .statement tag=01T0}

A category is a quiver endowed with an associative law of composition for which there exists at each vertex an identity element.

#### Example 1 {#ta-ii-s3-n1-exa-1 .statement tag=01T1}

Let C be a quiver. Let Ch(C) denote the set of paths in C and $o:$ Ch(C) $\rightarrow$ Som(C)$,t:$ Ch(C) $\rightarrow$ Som(C) the mappings which associate with a path its origin and its end. The quadruple $\Omega_C=$ (Som(C), Ch(C)$, o, t$) is a quiver. Endow it with the law of composition defined by juxtaposition of paths. This law of composition is associative; for every vertex $a$ of C, the constant loop $e_a= (a)$ of origin $a$ is an identity element at $a$. Thus, $\Omega_C$ is a category. It is said to be the category of paths of the quiver C.

#### Example 2 {#ta-ii-s3-n1-exa-2 .statement tag=01T2}

Let Σ be a Species of structures in a theory $\mathscr{T}$ stronger than set theory and let $\sigma (x, y, s, u)$ be a term of $\mathscr{T}$ satisfying conditions (MO$_I$), (MO$_{II}$) and (MO$_{III}$) of E, IV, p. 11. Let S be a set; suppose that every element of S is a pair $(x, s)$, where $x$ is a set and $s$ a structure of species Σ on $x$. Let F be the set of mappings $f$ such that there exist $(x, s)$ and $(y, t)$ in S such that $f$ is a $\sigma$-morphism of $x$, endowed with the structure $s$, into $y$, endowed with the structure $t$; one then sets $o(f) = (x, s)$ and $t(f) = (y, t)$. Endowed with the law of composition given by $m(f, g) =g\circ f$, the quiver $(S,F, o, t)$ is a category. In this context, the elements of S are rather called objects.

Let C be a category.

For every vertex $a$ of C, the set $C_{a,a}$, endowed with the law of composition $(f, g)\mapsto f g$, is a monoid with identity element $e_a$.

A map $f$ of C is said to be invertible if there exists a map $g$ of C such that $o(g) =t(f),t(g) =o(f)$ and such that $f g$ and $gf$ are identity elements at $o(f)$ and $t(f)$ respectively. Such a map $g$ is unique (if $f g=e_{o(f)}$ and $g'f=e_{t(f)}$, one has $g=e_{t(f)}g= (g'f)g=$ $g'(f g) =g'e_{o(f)}=g'$) and is called the inverse of $f$; the inverse of an invertible map $f$ is denoted by $f^{-1}$.

### 2. Functors

#### Definition 3 {#ta-ii-s3-def-3 .statement tag=01T3}

Let C and $C'$ be categories. A functor from C into $C'$ is a morphism of quivers $\varphi : C\rightarrow C'$ such that $\varphi (f g) =$ $\varphi (f)\varphi (g)$ for every pair $(f, g)$ of composable maps of C.

Let C and $C'$ be categories and let $\varphi : C\rightarrow C'$ be a functor. Let $f$ be an arrow of C$,a$ its origin and $b$ its end; then, $\varphi (f)$ is an arrow of $C'$ with origin $\varphi (a)$ and end $\varphi (b)$.

Let C, $C',C''$ be categories and let $\varphi : C\rightarrow C'$ and $\varphi ': C'\rightarrow C''$ be functors. Then, $\varphi '\circ \varphi$ is a functor.

Let C be a category. Then the quiver morphism Id$_C$ is a functor.

Let $\varphi : C\rightarrow C'$ be a functor. In order that $\varphi$ be an isomorphism, it is necessary and sufficient that the mappings Som($\varphi$ ) and Fl($\varphi$ ) be bijective.

Thus, if one calls a category structure on sets S and F the data of a quiver structure on these sets and of an associative composition law for which there exists at each vertex an identity element, one can take the functors as morphisms of the category structure (E, IV, p. 11).

### 3. Groupoids

#### Definition 4 {#ta-ii-s3-def-4 .statement tag=01T4}

A groupoid is a category each arrow of which is invertible.

Let G be a groupoid and let $a$ be a vertex of G. The monoid $G_{a,a}$ is a group, denoted by $G_a$ and called the isotropy group of G at $a$.

Let $a,b$ be vertices of G and let $f\in G_{a,b}$ be an arrow joining $a$ to $b$. The mapping $g\mapsto f gf^{-1}$ is a group isomorphism of $G_b$ onto $G_a$, denoted by Int($f$). If $f$ and $f'$ are composable arrows of G, one has Int($f f'$) $=$ Int($f$)$\circ$ Int($f'$) ; the inverse of the isomorphism Int($f$) is the isomorphism Int($f^{-1}$).

A morphism of groupoids $\varphi : G\rightarrow G'$ is a morphism of categories. Moreover, $\varphi$ is an isomorphism of groupoids if and only if it is an isomorphism of categories.

Let $\varphi : G\rightarrow G'$ be a morphism of groupoids. For every vertex $a$ of G, the mapping $f\mapsto \varphi (f)$ of $G_a$ into $(G')_{\varphi(a)}$ is a group homomorphism denoted by $\varphi_a$. In particular, one has $\varphi (e_a) =e_{\varphi(a)}$.

For every arrow $f$ of G$,\varphi (f^{-1})$ is the inverse of $\varphi (f)$. If $f$ is an arrow of G joining a vertex $a$ to a vertex $b$, one thus has, for every element $g\in G_b$, the relation Int($\varphi (f)$)$(\varphi (g)) =\varphi$(Int($f$)$(g)$).

### 4. Orbits of a groupoid

Let G be a groupoid. The connected components of the underlying quiver of G are called the orbits of G. The set of the orbits of G is denoted by Orb(G); if $\varphi : G\rightarrow G'$ is a morphism of groupoids, the mapping $\pi_0(\varphi )$ deduced from $\varphi$ by passing to the connected components of the associated graphs is in general denoted by Orb($\varphi$ ) and called the mapping deduced from $\varphi$ by passing to the orbits.

A groupoid which has exactly one orbit is said to be transitive. If G is a transitive groupoid, the groups $G_a$, for $a\in$ Som(G), are isomorphic. One says that the groupoid G is simply transitive if it is transitive and if, moreover, the isotropy groups $G_a$ are all reduced to their identity element.

#### Proposition 1 {#ta-ii-s3-prop-1 .statement tag=01T5}

Let G be a groupoid. The relation "there exists an arrow of G joining $a$ to $b$" is an equivalence relation in the set of vertices of G whose equivalence classes are the orbits of G.

Let $a,b,c$ be vertices of G. One has $e_a\in G_{a,a}$; if $f\in G_{a,b}$, $f^{-1}\in G_{b,a}$; if $f\in G_{a,b}$ and $g\in G_{b,c}$, one has $f g\in G_{a,c}$. This shows that the indicated relation is reflexive, symmetric and transitive; it is therefore an equivalence relation. The second assertion then results from the definition of the connected components of a quiver.

### 5. Examples of groupoids

1) Let G be a group. Let us denote by $\mathscr{G}$ the quiver whose set of vertices is reduced to one element and whose set of arrows is G. Endowed with the law of composition induced by that of G$,\mathscr{G}$ is a groupoid, called the groupoid associated with the group G.

2) Let X be a set. Let G be the quiver $(X,X\times X$, pr$_1$, pr$_2)$; define a law of composition in G by putting $(x, x')\cdot (x', x'') = (x, x'')$, if $x, x', x''$ are elements of X. This law is associative; for every $x\in X$, $(x, x)$ is the identity element at $x$; the inverse of the arrow $(x, x')$ is the arrow $(x', x)$. The groupoid thus defined is called the groupoid of pairs of the set X. If X is not empty, it is simply transitive.

3) Let X and S be sets and let $p: X\rightarrow S$ be a mapping. For $a\in S$, let $X_a=\overset{-1}{p}(a)$. For $a$ and $b$ in S, let $G_{a,b}$ be the set $\mathscr{B}(X_a; X_b)$ of bijections from $X_a$ onto $X_b$ and let G be the sum of the sets $G_{a,b}$. Let $o$ and $t$ be the mappings from G into S such that $o(f) =a$ and $t(f) =b$ for every element $f\in G_{a,b}$. The quadruple $(S,G, o, t)$ is a quiver. Endow it with the law of composition defined by $m(f, g) =g\circ f$ if $f\in \mathscr{B}(X_a; X_b)$ and $g\in \mathscr{B}(X_b; X_c)$, where $a, b, c$ are points of S. It is a groupoid; it is denoted by $\mathscr{B}(X, p)$ and called the groupoid of permutations of X relative to $p$.

4) Let $(G_i)_{i\in I}$ be a family of groupoids. Let us denote by G the product quiver of the family of underlying quivers; for each $i\in I$, let pr$_i: G\rightarrow G_i$ be the canonical quiver morphism. There exists a unique law of composition on G for which G is a groupoid and such that, for each $i\in I$, pr$_i$ is a groupoid morphism. Let $f= (f_i)_{i\in I}$ and $g= (g_i)_{i\in I}$ be arrows of G; they are composable if and only if the arrows $f_i$ and $g_i$ are composable, for $i\in I$. One then has $f g= (f_ig_i)_{i\in I}$.

The quiver G, endowed with this law of composition, is called the product groupoid of the family $(G_i)_{i\in I}$. It satisfies the following universal property: for every groupoid $G'$ and every family $(\varphi_i)_{i\in I}$, where $\varphi_i$ is a groupoid morphism of $G'$ into $G_i$, there exists a unique groupoid morphism $\varphi : G'\rightarrow G$ such that $\varphi_i=$ pr$_i\circ \varphi$ for each $i\in I$.

5) Let $((G_i)_{i\in I},(\varphi_{i,j})_{i\prec j})$ be an inductive system of groupoids, indexed by a right filtering preordered set $(I,\prec )$, the $\varphi_{i,j}$ being groupoid morphisms. Let G be the quiver whose set of vertices is lim$\longrightarrow_i$ Som(G$_i$), whose set of arrows is lim$\longrightarrow_i$ Fl(G$_i$), the source and target mappings being the mappings lim$\longrightarrow_io_{G_i}$ and lim$\longrightarrow_it_{G_i}$ respectively. The laws of composition of the $G_i$ induce a law of composition on G which makes it a groupoid (cf. A, I, p. 114). The canonical mappings Som(G$_i$)$\rightarrow$ Som(G) and Fl(G$_i$)$\rightarrow$ Fl(G) define a groupoid morphism $\varphi_i$ of $G_i$ into G. If $i,j$ are elements of I such that $i\prec j$, one has $\varphi_j\circ \varphi_{i,j}=\varphi_i$. The groupoid G is called the inductive limit of the family of groupoids $G_i$ and is denoted by lim$\longrightarrow_iG_i$. It satisfies the following universal property: for every groupoid H and every family $(\psi_i)_{i\in I}$, where, for $i\in I,\psi_i: G_i\rightarrow H$ is a groupoid morphism, such that $\psi_j\circ \varphi_{i,j}=\psi_i$ for every pair $(i, j)$ of elements of I such that $i\prec j$, there exists a unique groupoid morphism $\psi : G\rightarrow H$ such that $\psi_i=\psi \circ \varphi_i$.

For the existence of a groupoid satisfying this universal property when one does not suppose that the set I is right filtering, cf. II, p. 228, exerc. 3.

### 6. Subgroupoids

#### Definition 5 {#ta-ii-s3-def-5 .statement tag=01T6}

Let C be a category. A subcategory of C is a subquiver D of C satisfying the following conditions:

(i) For every vertex $a$ of D$,e_a$ is an arrow of D;

(ii) For every composable pair $(f, g)$ of arrows of C belonging to D, the product $f g$ is an arrow of D;

Let C be a category and let D be a subcategory of D; endowed with the law of composition deduced from that of C by passing to subsets, D is a category.

Every full subquiver of C is a subcategory of C. The intersection of a family of subcategories of C is a subcategory of C.

#### Definition 6 {#ta-ii-s3-def-6 .statement tag=01T7}

Let G be a groupoid. A subgroupoid of G is a subcategory H of G such that the inverse of every arrow of G belonging to H is an arrow of H.

Let G be a groupoid. Every subgroupoid of G is a groupoid. Every full subquiver of G is a subgroupoid of G. The intersection of a family of subgroupoids of G is a subgroupoid of G.

Let H be a subquiver of G. The intersection of the subgroupoids of G of which H is a subquiver is called the subgroupoid of G generated by H. The set of its vertices is equal to that of H and its orbits are the connected components of H.

#### Example 1 {#ta-ii-s3-n6-exa-1 .statement tag=01T8}

Let X be a set; let us denote by $X\times X$ the groupoid of pairs of X (II, p. 163, Example 2). Let R be an equivalence relation on X. The subquiver of the groupoid $X\times X$ whose set of vertices is X and whose set of arrows is the graph of the equivalence relation R is a subgroupoid of $X\times X$. Its orbits are the equivalence classes of the relation R.

Conversely, every subgroupoid of $X\times X$ whose set of vertices is X is of this form.

Let X and S be sets and let $p: X\rightarrow$ S be a mapping. The mapping $p$ defines an equivalence relation in X (E, II, p. 41). One denotes by $X\times_SX$ the subgroupoid of $X\times X$ defined by this equivalence relation, and one calls it the groupoid of pairs of $(X, p)$.

#### Example 2 {#ta-ii-s3-n6-exa-2 .statement tag=01T9}

Let G and $G'$ be groupoids, let $\varphi$ and $\psi$ be groupoid morphisms from G into $G'$. The equalizer of $\varphi$ and $\psi ($cf. II, p. 153) is a subgroupoid of G.

#### Example 3 {#ta-ii-s3-n6-exa-3 .statement tag=01TA}

Let X be a set and Γ a group. Denote by $X\times \Gamma \times X$ the graph whose set of vertices is X, whose set of arrows is $X\times \Gamma \times X$, the origin and end mappings being respectively pr$_1$ and pr$_3$. Endowed with the composition law $(x, \gamma , x')\cdot (x', \gamma ', x'') = (x, \gamma \gamma ', x'')$, it is a groupoid. It is moreover the groupoid deduced by transport of structure from the groupoid $(X\times X)\times \Gamma$, product of the groupoid of pairs $X\times X$ and of the groupoid associated with the group Γ (II, p. 163, example 1), by means of the bijection $(x, x', \gamma )\mapsto (x, \gamma , x')$ of $X\times X\times \Gamma$ onto $X\times \Gamma \times X$.

Let $m: X\times \Gamma \rightarrow X$ be a right operation of the group Γ on X. The graph F of the mapping $m$, that is to say the set of triples $(x, \gamma , x')\in X\times \Gamma \times X$ such that $x'=x\gamma$, is the set of arrows of a unique subgroupoid G of $X\times \Gamma \times X$. The orbits of this groupoid are the orbits of Γ in X; if $x\in X$, the isotropy group of G at $x$ is the set of $(x, \gamma , x)$, where $\gamma$ runs through the stabilizer of $x$ in Γ.

Conversely, every subgroupoid G of the groupoid $X\times \Gamma \times X$ such that the mapping (pr$_1$, pr$_2$) of Fl(G) into $X\times \Gamma$ is a bijection is of this form.

#### Example 4 {#ta-ii-s3-n6-exa-4 .statement tag=01TB}

Let G be a groupoid, let X be a set and let $\varphi : X\rightarrow$ Som(G) be a mapping. Define a graph $G'$ in the following way. The set Som(G$'$) is the set X; for every pair $(x, y)$ of elements of X, the set Fl$_{x,y}(G')$ is the set of triples $(x, f, y)\in X\times$ Fl(G) $\times X$, where $f$ is an element of Fl$_{\varphi(x),\varphi(y)}(G)$. Let $x,y,z$ be elements of X$,f\in$ Fl$_{\varphi(x),\varphi(y)}(G)$ and $g\in$ Fl$_{\varphi(y),\varphi(z)}(G)$ arrows of G, and put $(x, f, y)\cdot (y, g, z) = (x, f g, z)$. This defines a composition law in the graph $G'$ which makes it a groupoid. It is called the inverse image groupoid of the groupoid G by the mapping $\varphi$ and is denoted by $\varphi^*(G)$.

The pair $(\varphi , \psi )$, where $\psi :$ Fl($\varphi^*(G)$)$\rightarrow$ Fl(G) is the mapping defined by $(x, f, y)\mapsto f$ is a groupoid morphism from $\varphi^*(G)$ into G, called the canonical morphism.

#### Example 5 {#ta-ii-s3-n6-exa-5 .statement tag=01TC}

Let $\varphi : G\rightarrow G'$ be a morphism of groupoids. Let H be the subquiver of G with set of vertices Som(G) and whose set of arrows consists of the $f\in$ Fl(G) such that $\varphi (f)$ is an identity element of $G'$. For every $a\in$ Som(G)$,e_a\in H_{a,a}$. For every $f\in$ Fl(H), $\varphi (f^{-1}) =\varphi (f)^{-1}$, hence $f^{-1}\in$ Fl(H). Further, if $f$ and $g$ are composable arrows of H, one has $\varphi (f g) =\varphi (f)\varphi (g) =e_{t(\varphi(f))}e_{o(\varphi(g))}=$ $e_{t(\varphi(f))}$, hence $f g$ is an arrow of H. This shows that H is a subgroupoid of G. It is called the kernel of $\varphi$ and is denoted by Ker($\varphi$ ).

#### Example 6 {#ta-ii-s3-n6-exa-6 .statement tag=01TD}

Let $\varphi : G\rightarrow G'$ be a morphism of groupoids. The quiver $\varphi (G)$ whose set of vertices is $\varphi$(Som(G)) and whose set of arrows is $\varphi$(Fl(G)) is not in general a subgroupoid of $G'$. This is nevertheless the case if the mapping Som($\varphi$ ) is injective (II, p. 225, exerc. 5).

### 7. Operations of a groupoid

Let G be a groupoid; let S denote the set of its vertices. Let X be a set and let $p: X\rightarrow S$ be a mapping. A (right) operation $\varphi$ of the groupoid G on the set X, relative to $p$, is a morphism of groupoids $\varphi$ from G into the groupoid $\mathscr{B}(X, p)$ of permutations of the set X relative to $p($II, p. 163) which induces the identity on the set of vertices. In other words, $\varphi$ consists, for each pair $(a, b)$ of points of S and for each arrow $g\in G$ joining $a$ to $b$, of a mapping $\varphi (g): X_a\rightarrow X_b$, such that, for every pair $(f, g)$ of composable arrows of G,

$$
\varphi (f g) =\varphi (g)\circ \varphi (f)
$$

and such that, for every $a\in S,\varphi (e_a)$ is the identity of $X_a$.

Let $\varphi$ and $\varphi '$ be operations of the groupoid G on a set X, relative to a mapping $p: X\rightarrow S$. In order that one have $\varphi =\varphi '$, it is enough that there exist a subquiver H of G, generating G, such that $\varphi (f) =\varphi '(f)$ for every $f\in$ Fl(H). In fact, the set of arrows $f$ of G such that $\varphi (f) =\varphi '(f)$ is the set of arrows of a subgroupoid of G, with set of vertices S.

Let G be a groupoid with set of vertices S, let X be a set, let $p: X\rightarrow S$ be a mapping, and let $\varphi$ be an operation of G on X relative to $p$. Let $G_{\varphi}$ be the subquiver of $p^*(G)$ whose set of vertices is X and whose set of arrows is the set of triples $(x, f, y)\in X\times$ Fl(G) $\times X$ such that $\varphi (f)(x) =y$. It is a subgroupoid of $p^*(G)$.

Conversely, let Γ be a subgroupoid of $p^*(G)$; suppose that the mapping $(x, f, y)\mapsto (x, f)$ of Fl(Γ) into $X\times$ Fl(G) is injective and that its image is the set of pairs $(x, f)$ such that $p(x) =o(f)$. Then there exists a unique operation $\varphi$ of the groupoid G on X such that $\Gamma  = G_{\varphi}$.

The orbits of the groupoid $G_{\varphi}$ are called the orbits of the operation of G on X. By definition, they are the equivalence classes of the relation in X defined by $R\{x, y\}$ if and only if there exists $f\in$ Fl(G) such that $\varphi (f)(x) =y$.

#### Example 1 {#ta-ii-s3-n7-exa-1 .statement tag=01TE}

Let G be a group, and let $\mathscr{G}$ be the groupoid associated with G (II, p. 163, Example 1). If X is a set, an operation (on the right) of the groupoid $\mathscr{G}$ on X is nothing other than an operation (on the right) of the group G on X. Moreover, the orbits of the operation of $\mathscr{G}$ coincide with those of the group G.

#### Example 2 {#ta-ii-s3-n7-exa-2 .statement tag=01TF}

Let $G = (S,F, o, t)$ be a groupoid. There exists a unique operation of G on the set S, relative to Id$_S$. It is given by $\varphi (f)(a) =b$ if $f\in G_{a,b}$. The orbits for this operation are the orbits of G in the sense defined on p. 162.

Let G be a groupoid, let S be the set of its vertices, let X be a set, and let $p: X\rightarrow S$ be a mapping. Let $\varphi$ be an operation of G on X relative to $p$. One says that the groupoid G operates without monodromy on X if, for every point $a\in S$ and every element $f\in G_a,\varphi (f)$ is the identity of $X_a$. If the groupoid G is transitive, it is enough that this be so for one point of S.

Let $a$ be a point of S and suppose that one has $\varphi (f) =$ Id$_{X_a}$ for every $f\in G_a$. Let $b$ be a point of S belonging to the orbit of $a$ and let $g$ be an arrow of G joining $a$ to $b$. For every $f\in G_b$, Int($g$)$(f) =gf g^{-1}$ is an element of $G_a$; hence one has Id$_{X_a}=\varphi (gf g^{-1}) =\varphi (g)\varphi (f)\varphi (g)^{-1}$, so that $\varphi (f) =$ Id$_{X_b}$. Let $b$ be a point of S belonging to the orbit of $a$ and let $g,g'$ be arrows of G joining $a$ to $b$; then $g'g^{-1}$ is a loop at $a$, whence $\varphi (g'g^{-1}) =$ Id$_{X_a}$ and $\varphi (g) =\varphi (g')$.

### 8. Normal Subgroupoids; Quotient Groupoids

#### Definition 7 {#ta-ii-s3-def-7 .statement tag=01TG}

Let G be a groupoid. One says that a subgroupoid H of G is normal if Som(H) = Som(G) and if for every pair $(a, b)$ of vertices of H and every arrow $f\in G_{a,b}$, one has Int($f$)$(H_b) = H_a$.

Let G be a groupoid and let H be a subgroupoid of G whose set of vertices is equal to Som(G). To verify that H is distinguished, it is enough to prove that $fH_bf^{-1}\subset H_a$ for every $a\in$ Som(G), every $b\in$ Som(G) and every $f\in G_{a,b}$. In fact, if this is so, one also has $f^{-1}H_af\subset H_b$ for every arrow $f\in G_{b,a}$, that is, $H_a\subset fH_bf^{-1}$, and consequently $fH_bf^{-1}= H_a$.

Let G be a groupoid and let H be a distinguished subgroupoid of G. For every vertex $a$ of G, the subgroup $H_a$ of $G_a$ is a distinguished subgroup of $G_a$.

Let $\varphi : G\rightarrow G'$ be a morphism of groupoids. The kernel of $\varphi ($II, p. 166, example 5) is a distinguished subgroupoid of G. In fact, let $f$ be an arrow in G joining $a$ to $b$ and let $g\in$ Ker($\varphi$ )$_b$; then one has $\varphi (f gf^{-1}) =\varphi (f)\varphi (g)\varphi (f^{-1}) =\varphi (f)e_{\varphi(b)}\varphi (f)^{-1}=e_{\varphi(a)}$, whence the inclusion $f$Ker($\varphi$ )$_bf^{-1}\subset$ Ker($\varphi$ )$_a$.

Let G be a groupoid. The groupoid G and the subgroupoid of G whose set of arrows is the set of identity elements of G are distinguished subgroupoids of G. The intersection of a family of distinguished subgroupoids of G is a distinguished subgroupoid of G. In particular, for every subset $F\subset$ Fl(G), there exists a smallest distinguished subgroupoid of G whose set of arrows contains F. It is called the distinguished subgroupoid generated by F.

Let H be a distinguished subgroupoid of G. Let $\mathscr{R}$ be the equivalence relation in Fl(G) defined by $\mathscr{R}\{f, g\}$ if and only if there exist arrows $x$ and $y$ in Fl(H) such that $f=xgy$. If $f$ and $g$ are arrows of G equivalent modulo $\mathscr{R}$, their origins (resp. their ends) belong to the same orbit of H. Put $F'=$ Fl(G)$/\mathscr{R}$ and denote by $o'$ and $t'$ the mappings of $F'$ into Orb(H) deduced from $o$ and $t$ by passing to the quotients. Denote by $G/H$ the quiver (Orb(H)$,F', o', t'$).

#### Lemma {#ta-ii-s3-n8-lem-1 .statement tag=01TH}

Given composable arrows $u$ and $v$ of $G/H$, one can choose representatives $f$ and $g$ of $u$ and $v$ in Fl(G) which are composable. The class modulo $\mathscr{R}$ of the product $f g$ does not depend on the choice of $f$ and $g$.

Let $f$ and $g$ be arbitrary representatives of $u$ and $v$ in Fl(G). The end of $f$ and the origin of $g$ belong to one and the same orbit of H, hence can be joined by an arrow $x$ of H (II, p. 162, prop. 1). The arrows $f x$ and $g$ are then representatives of $u$ and $v$ in F which are composable in G. This proves the first assertion.

Let now $f,g$ on the one hand, and $f',g'$ on the other hand, be representatives of $u$ and $v$ which are composable in G. By hypothesis, there exist arrows $x,y,z,t$ in H such that one has $f'=xf y$ and $g'=zgt$. Then one has $yz\in H_{t(f)}$ and $f'g'=xf yzgt=xf(yz)f^{-1}f gt$. Since H is a normal subgroupoid of G, the arrow $f(yz)f^{-1}$ is an arrow of H. The same is therefore true of the arrow $xf(yz)f^{-1}$, which proves that $f'g'$ and $f g$ are equivalent modulo $\mathscr{R}$.

By virtue of this lemma, there exists a unique law of composition $m$ in the quiver $G/H$ such that, for every pair $(u, v)$ of composable arrows, $m(u, v)$ is the class modulo $\mathscr{R}$ of the product $f g$, for every pair $(f, g)$ of composable arrows of G such that $u$ is the class of $f$ and $v$ that of $g$. Endowed with this law of composition, $G/H$ is a groupoid. Let $p_1:$ Som(G) $\rightarrow$ Som(G$/H$) and $p_2:$ Fl(G) $\rightarrow$ Fl(G$/H$) be the canonical surjections. The pair $p= (p_1, p_2)$ is a morphism of groupoids of G into $G/H$ whose kernel is the normal subgroupoid H.

#### Definition 8 {#ta-ii-s3-def-8 .statement tag=01TI}

One says that $G/H$ is the quotient groupoid of G by H and that $p: G\rightarrow G/H$ is the canonical morphism.

#### Remark 1 {#ta-ii-s3-n8-rem-1 .statement tag=01TJ}

The mapping Som($p$) defines, by passing to quotients, a bijection of the set of orbits of G onto the set of orbits of $G/H$. In particular, G is transitive if and only if $G/H$ is.

#### Remark 2 {#ta-ii-s3-n8-rem-2 .statement tag=01TK}

Let $a$ and $b$ be vertices of G. The mapping of $G_{a,b}$ into $(G/H)_{p(a),p(b)}$ deduced from $p$ is surjective. Let in fact $u$ be an arrow of $G/H$ joining $p(a)$ to $p(b)$; it is the class modulo $\mathscr{R}$ of an arrow $f$ of G. The origin $o(f)$ of $f$ belongs to the orbit of $a$ in H; hence there exists an arrow $x$ in H joining $a$ to $o(f)$. Analogously, there exists an arrow $y$ in H joining $t(f)$ to $b$. Then $f'=xf y$ is an element of $G_{a,b}$ whose class modulo $\mathscr{R}$ is $u$.

#### Proposition 2 {#ta-ii-s3-prop-2 .statement tag=01TL}

Let $a$ be a vertex of G. The group homomorphism $p_a: G_a\rightarrow (G/H)_{p(a)}$ deduced from $p$ by passing to the isotropy groups is surjective; its kernel is $H_a$.

The homomorphism $p_a$ is surjective by virtue of the preceding remark. Its kernel contains $H_a$ by construction of the groupoid $G/H$. Let $f$ be an element of $G_a$ such that $p_a(f) =e_{p(a)}$. This means that $f$ and $e_a$ are equivalent modulo $\mathscr{R}$; there then exist arrows $x$ and $y$ of H such that $f=xe_ay$. Necessarily, $x$ and $y$ belong to $H_a$, whence $f\in H_a$.

#### Proposition 3 {#ta-ii-s3-prop-3 .statement tag=01TM}

Let G be a groupoid, let H be a distinguished subgroupoid of G and let $p: G\rightarrow G/H$ be the canonical morphism. Let $\varphi : G\rightarrow G'$ be a groupoid morphism such that $H\subset$ Ker($\varphi$ ). There exists a unique groupoid morphism $\overline{\varphi}: G/H\rightarrow G'$ such that $\overline{\varphi}\circ p=\varphi$.

One says that $\overline{\varphi}$ is the groupoid morphism deduced from $\varphi$ by passing to the quotient.

The uniqueness of such a morphism is obvious, since the mappings Som($p$) and Fl($p$) are surjective.

Let $a$ and $b$ be vertices of G. If they are in the same orbit of H, there exists an arrow $f$ joining $a$ to $b$ in H, and one has $\varphi (f) =e_{\varphi(a)}$. In particular, $\varphi (a) =\varphi (b)$. Consequently, the mapping Som($\varphi$ ) defines, by passing to the quotient, a mapping $\overline{\varphi}_1:$ Orb(H) $\rightarrow$ Som(G$'$). Let $f$ and $g$ be arrows in G. If $f$ and $g$ are equivalent modulo $\mathscr{R}$, there exist arrows $x$ and $y$ in H such that $f$ = $xgy$. Consequently, $\varphi (f) =\varphi (x)\varphi (g)\varphi (y) =\varphi (g)$ since $\varphi (x)$ and $\varphi (y)$ are identity elements. The mapping Fl($\varphi$ ) therefore defines, by passing to the quotient, a mapping $\overline{\varphi}_2:$ Fl(G)$/\mathscr{R}\rightarrow$ Fl(G$'$).

Let $f$ and $g$ be composable arrows of G; let us denote by $u$ and $v$ their classes in Fl(G$/H$). One has $\overline{\varphi}_2(uv) =\varphi (f g) =\varphi (f)\varphi (g) =$ $\overline{\varphi}_2(u)\overline{\varphi}_2(v)$.

The pair $\overline{\varphi}= (\overline{\varphi}_1, \varphi_2)$ is a groupoid morphism from $G/H$ into $G'$ and one has $\overline{\varphi}\circ p=\varphi$.

### 9. Groupoid of classes of paths of a graph

Let G be a graph. Let us denote by $\Omega_G$ the category of paths of the underlying quiver of G (II, p. 160, example 1). Consider the finest equivalence relation $\mathscr{R}$ in Ch(G) such that one has:

(i) For every pair $(a, b)$ of vertices of G and every arrow $f$ in G joining $a$ to $b$, the paths $(a, f, b,\overline{f}, a)$ and $e_a$ are equivalent modulo $\mathscr{R}$;

(ii) If $(c, d)$ and $(c', d')$ are pairs of juxtaposed paths in G such that $\mathscr{R}\{c, c'\}$ and $\mathscr{R}\{d, d'\}$, the paths $c*d$ and $c'*d'$ are equivalent modulo $\mathscr{R}$.

Two paths equivalent modulo $\mathscr{R}$ have the same origin and the same end. The mappings $o$ and $t$ from Ch(G) into Som(G) define, by passing to the quotient, mappings $o'$ and $t'$ from Ch(G)$/\mathscr{R}$ into Som(G). Let us denote by $\varpi_G$ the quiver (Som(G), Ch(G)$/\mathscr{R}, o', t'$). The pair $\varphi$ formed by the identity mapping of Som(G) and the canonical projection of Ch(G) onto Ch(G)$/\mathscr{R}$ is a morphism of quivers from $\Omega_G$ into $\varpi_G$. The juxtaposition of paths in Ch(G) defines, by passing to the quotients, a law of composition in $\varpi_G$.

#### Proposition 4 {#ta-ii-s3-prop-4 .statement tag=01TN}

Endowed with this law of composition, $\varpi_G$ is a groupoid.

By construction, one has the relation $\varphi (cc') =\varphi (c)\varphi (c')$, for every pair of juxtaposed paths $(c, c')$ in G. Every arrow of $\varpi_G$ is of the form $\varphi (c)$, where $c$ is a path in G. It follows that the law of composition of $\varpi_G$ is associative and that $\varphi (e_a)$ is an identity element at $a$, for every vertex $a$ of $\varpi_G$. It remains to prove that every arrow of $\varpi_G$ is invertible. Let $c$ be a path in G, and let us prove by induction on the length of $c$ that one has $\varphi (c)\varphi (\overline{c}) =\varphi (e_{o(c)})$. This equality is true if $c$ is of length 0. If $c$ is of length $n\geqslant 1$, we may write $c=c_1c_2$, with $c_1$ of length 1 and $c_2$ of length $n-1$. Then, $\overline{c}=\overline{c_2}\overline{c_1}$ and one has

$$
\varphi (c)\varphi (\overline{c}) =\varphi (c_1)\varphi (c_2)\varphi (\overline{c_2})\varphi (\overline{c_1}) =\varphi (c_1)\varphi (e_{o(c_2)})\varphi (\overline{c_1}) =\varphi (c_1)\varphi (\overline{c_1})
$$

$$
=\varphi (c_1\overline{c_1}) =\varphi (e_{o(c_1)})
$$

by definition of the relation $\mathscr{R}$.

Applying this equality to the path $\overline{c}$, we see that $\varphi (\overline{c})\varphi (c) =$ $\varphi (e_{t(c)})$. Thus, $\varphi (c)$ is invertible, with inverse $\varphi (\overline{c})$.

The equivalence classes of the relation $\mathscr{R}$ are called the path classes in the graph G; the groupoid $\varpi_G$ is called the groupoid of path classes of the graph G. It has the same set of vertices as G, and its orbits are the connected components of the graph G.

Let us denote by $v$ the mapping which associates with an arrow $f$ of G the class of the path $(o(f), f, t(f))$ of G. The pair $j$ = (Id$_{Som(G)}, v$) is a morphism, called canonical, of quivers from G into $\varpi_G$. Its image generates $\varpi_G$; for every arrow $f$ of G, one has $j(\overline{f}) =j(f)^{-1}$.

Let G and $G'$ be graphs, let $\varphi : G\rightarrow G'$ be a graph morphism. Let us denote by $j: G\rightarrow \varpi_G$ and $j': G'\rightarrow \varpi_{G'}$ the canonical morphisms. If $c= (a_0, f_1, a_1, . . . , a_n)$ is a path in G, the class of the path $\varphi (c) = (\varphi (a_0), \varphi (f_1), \varphi (a_1), . . . , \varphi (a_n))$ depends only on the class of $c$. Thus, by passing to equivalence classes, one defines a quiver morphism $\varpi (\varphi ):\varpi_G\rightarrow \varpi_{G'}$ such that $\varpi (\varphi )\circ j=j'\circ \varphi$. It is a groupoid morphism.

#### Proposition 5 {#ta-ii-s3-prop-5 .statement tag=01TO}

Let G be a graph; let us denote by $j$ the canonical quiver morphism of G into $\varpi_G$. Let $\varphi$ be a quiver morphism of G into a groupoid $G'$ such that $\varphi (\overline{f}) =\varphi (f)^{-1}$ for every arrow $f$ of G. Then there exists a unique groupoid morphism $\varphi '$ of $\varpi_G$ into $G'$ such that $\varphi '\circ j=\varphi$.

One defines a mapping $u:$ Ch(G) $\rightarrow$ Fl(G$'$) by setting, for every path $c= (a_0, f_1, a_1, . . . , f_n, a_n)$ in G$,u(c) =e_{a_0}\varphi (f_1). . . \varphi (f_n)$. For every pair $(c, c')$ of composable paths in G, one has $u(cc') =$ $u(c)u(c')$. The mapping $u$ is compatible with the equivalence relation $\mathscr{R}$ defined above, whence, by passing to the quotient, a mapping $u':$ Ch(G)$/\mathscr{R}\rightarrow$ Fl(G$'$). Let us then set $\varphi '=$ (Som($\varphi$ )$, u'$). It is a groupoid morphism of $\varpi_G$ into $G'$ such that $\varphi '\circ j=\varphi$.

Let $\psi$ be a groupoid morphism of $\varpi_G$ into $G'$ such that $\psi \circ j=\varphi$. The equalizer of $\varphi '$ and $\psi$ is a subgroupoid of $\varpi_G$ which contains $j(G)$. Hence it is equal to $\varpi_G$, because $\varpi_G$ is generated by $j(G)$, and one has $\psi =\varphi '$.

#### Corollary 1 {#ta-ii-s3-prop-5-cor-1 .statement tag=01TP}

In a graph, every class of paths contains a unique path without retracing.

Let G be a graph. Let us denote by $j: G\rightarrow \varpi_G$ the canonical quiver morphism.

The existence, for every path $c$ of G, of an equivalent path without retracing is immediate by induction on the length of $c$ (cf. II, p. 157).

Let A be an orientation of G and let $G'$ be the groupoid associated with the free group F(A) constructed on A (II, p. 163, Example 1). Let $\psi$ be the morphism of quivers from G into $G'$ such that, for every $f\in A,\psi (f)$ is the element $f$ of F(A) and $\psi (\overline{f})$ is the element $f^{-1}$ of F(A). Let $\psi '$ be the unique morphism of groupoids from $\varpi_G$ into $G'$ such that $\psi '\circ j=\psi$.

Let $c,c'$ be paths without backtracking equivalent modulo $\mathscr{R}$. They have the same source and the same end. To prove that they are equal, it is enough to prove that the sequences $(f_1, . . . , f_n)$ and $(g_1, . . . , g_m)$ of their edges are equal. The image under $\psi '$ of the common class of $c$ and $c'$ is equal to $\psi (f_1). . . \psi (f_n)$ and to $\psi (g_1). . . \psi (g_m)$. Now the terms of the sequences $(\psi (f_1), . . . , \psi (f_n))$ and $(\psi (g_1), . . . , \psi (g_m))$ belong to the subset $A\cup A^{-1}$ of F(A) and two consecutive elements of these sequences are not inverses of one another. By A, I, p. 84, Prop. 7, these two sequences are equal. It follows that the sequences $(f_1, . . . , f_n)$ and $(g_1, . . . , g_m)$ are equal, and therefore that $c=c'$, whence uniqueness.

#### Corollary 2 {#ta-ii-s3-prop-5-cor-2 .statement tag=01TQ}

The canonical morphism from G into $\varpi_G$ is injective.

This results immediately from Corollary 1.

#### Corollary 3 {#ta-ii-s3-prop-5-cor-3 .statement tag=01TR}

Let $G'$ be a subgraph of G. The morphism from $\varpi_{G'}$ into $\varpi_G$ deduced from the injection of $G'$ into G is injective.

Let us denote by $i$ the inclusion morphism of $G'$ into G and by $\varpi (i)$ the morphism from $\varpi_{G'}$ into $\varpi_G$ deduced from it. The mappings Som($i$) and Som($\varpi (i)$) coincide. Moreover, if $c$ is a path without backtracking in $G'$, the path $i(c)$ is a path without backtracking in G. The assertion therefore results from Corollary 1.

#### Corollary 4 {#ta-ii-s3-prop-5-cor-4 .statement tag=01TS}

A nonempty graph G is a tree if and only if the groupoid $\varpi_G$ is simply transitive.

Let $a$ be a point of G. By Corollary 1, the following properties are equivalent:

(i) The isotropy group of $\varpi_G$ at $a$ is reduced to the identity element;

(ii) The only loop in G with origin $a$ which is without backtracking is the constant loop with origin $a$.

The groupoid $\varpi_G$ is simply transitive if and only if it is transitive and has property (i) for every $a$. The graph G is a tree if and only if it is connected and has property (ii) for every point $a$. Since the orbits of $\varpi_G$ are identified with the connected components of G, the corollary follows.

### 10. Free Groupoids

#### Definition 9 {#ta-ii-s3-def-9 .statement tag=01TT}

Let C be a quiver. The groupoid $\varpi_{\widetilde{C}}$ of classes of paths of the graph $\widetilde{C}$ associated with C is called the free groupoid constructed on C, and is denoted by Grp(C).

The set of vertices of Grp(C) is equal to that of the vertices of C; the orbits of Grp(C) are the connected components of C.

Let C be a nonempty quiver. By Corollary 4, p. 174, the graph $\widetilde{C}$ associated with C is a tree if and only if the free groupoid Grp(C) constructed on C is simply transitive.

The composite of the canonical quiver morphisms $i: C\rightarrow \widetilde{C}$ and $j:\widetilde{C}\rightarrow \varpi_C$ is a quiver morphism from C into Grp(C) which is called the canonical morphism of C into Grp(C). Let us denote it by $\theta$. For every vertex $a$ of C, one has $\theta (a) =a$. If $f$ is an arrow of C$,\theta (f)$ is the class of the path $(o(f),(f,1), t(f))$ of $\widetilde{C}$. The morphism $\theta$ is injective (II, p. 174, Corollary 2) and its image generates the groupoid Grp(C).

Let $\varphi : C\rightarrow C'$ be a quiver morphism. Let us denote by $\theta_C$ (resp. $\theta_{C'}$) the canonical morphism of C into Grp(C) (resp. of $C'$ into Grp(C$'$)). The morphism $\varpi (\widetilde{\varphi})$ is the unique groupoid morphism $\psi$ from Grp(C) into Grp(C$'$) such that $\psi \circ \theta_C=\theta_{C'}\circ \varphi$.

#### Proposition 6 {#ta-ii-s3-prop-6 .statement tag=01TU}

Let C be a quiver, let G be a groupoid, and let $\varphi$ be a quiver morphism from C into G. There exists a unique groupoid morphism $\varphi '$ from Grp(C) into G such that $\varphi '\circ \theta_C=\varphi$.

Let $\psi$ be the quiver morphism from $\widetilde{C}$ into G such that $\psi (a) =\varphi (a)$ for every vertex $a$ of C and $\psi (f, \varepsilon ) =\varphi (f)^{\varepsilon}$ for every arrow $f$ of C and every $\varepsilon \in  \{-1,1\}$. One has $\psi \circ i=\varphi$. By Proposition 5, p. 173, there exists a morphism $\varphi '$ from Grp(C) $=\varpi_C$ into G such that $\varphi '\circ j=\psi$. One then has $\varphi '\circ \theta_C=\varphi '\circ j\circ i=\psi \circ i\widetilde{=}\varphi$. As in the proof of Prop. 5, the uniqueness of $\varphi '$ results from the fact that $\theta_C(C)$ generates the groupoid Grp(C).

Under the hypotheses of Prop. 6, one sometimes says that $\varphi '$ is the groupoid morphism from Grp(C) into G extending the quiver morphism $\varphi$.

#### Example {#ta-ii-s3-n10-exa-1 .statement tag=01TV}

Let C be a quiver having a unique vertex $s$ and let A be the set of its arrows. The groupoid Grp(C) is then the groupoid associated with the free group F(A) constructed on A. In fact, it has a unique vertex $s$ and it results immediately from Prop. 6 that the canonical mapping from A into Grp(C)$_s$ deduced from the canonical morphism of C into Grp(C) satisfies the universal property of free groups (A, I, p. 85, Prop. 8).

### 11. Contraction of arrows of a groupoid

Let G be a groupoid and let F be a subset of the set of arrows of G. Let H be the normal subgroupoid of G generated by F. The groupoid $G/H$ is called the groupoid deduced from G by contraction of the set of arrows F and is denoted by $G/F$. If $p$ denotes the canonical morphism from G into $G/F$, one has $p(o(f)) =p(t(f))$ and $p(f) =e_{p(o(f))}$ for every arrow $f\in F$.

This morphism satisfies the following universal property.

#### Proposition 7 {#ta-ii-s3-prop-7 .statement tag=01TW}

For every groupoid morphism $\varphi : G\rightarrow G'$ which maps every arrow belonging to F onto an identity element of $G'$, there exists a unique groupoid morphism $\varphi ': G/F\rightarrow G'$ such that $\varphi '\circ p=\varphi$.

The kernel of $\varphi$ is a normal subgroupoid of G and the set of its arrows contains F. By definition, H is the smallest normal subgroupoid of G whose set of arrows contains F; it is therefore contained in the kernel of $\varphi$. The proposition then results from II, p. 170, Prop. 3.

Let us denote by Γ the subquiver of G whose set of vertices is Som(G) and whose set of arrows is F. The orbits of H are identified with the connected components of the quiver Γ. By definition of the quotient of a groupoid by a normal subgroupoid, the set of vertices of $G/F$ is identified with the set of connected components of Γ; in other words, it is the quotient set of Som(G) by the finest equivalence relation such that $o(f)$ is equivalent to $t(f)$ for every arrow $f\in F$.

The mapping $p$ induces, by passing to quotients, a bijection of the set of orbits of G onto the set of orbits of $G/F$ (II, p. 170, remark 1).

The purpose of this No$^o$ is to calculate the homomorphisms induced by $p$ by passing to the isotropy groups, which amounts, according to prop. 2 (II, p. 170), to calculating the isotropy groups of the subgroupoid H.

#### Proposition 8 {#ta-ii-s3-prop-8 .statement tag=01TX}

Let $\delta$ be the canonical morphism of the free groupoid Grp(Γ) into G extending the canonical injective morphism of Γ into G. Let $a$ be a vertex of G and let A be the orbit of $a$ in G. For every $b\in A$, let $f_{ab}$ be an arrow of G joining $a$ to $b$. The isotropy group $H_a$ is the distinguished subgroup of $G_a$ generated by the elements Int($f_{ab}$)$(\delta (c))$, where $b$ runs through the set A and $c$ runs through the elements of Grp(Γ)$_b$.

If $x$ and $y$ are vertices of G belonging to the same orbit, with $x=\not a$, let us moreover fix an arrow $f_{xy}$ of G joining $x$ to $y$. For every point $x$ of G, let $N_x$ be the distinguished subgroup of $G_x$ generated by the elements Int($f_{xy}$)$(\delta (c))$, where $y$ runs through the orbit of $x$ in G and $c$ runs through the group Grp(Γ)$_y$. For every $f\in G_{xy}$ and every $g\in N_y$, one has $f gf^{-1}\in N_x$. Let $x\in$ Som(G). One has $\delta$(Grp(Γ)$_x$)$\subset N_x$, by definition of $N_x$. By definition of the groupoid H$,\delta (f)$ is an arrow of H for every arrow $f$ of Grp(Γ) ; consequently, $\delta$(Grp(Γ)$_x$) is contained in $H_x$. Since H is a distinguished subgroupoid of G, one then has

Int($f_{xy}$)$(\delta (c))\in$ Int($f_{xy}$)$(N_y)\subset$ Int($f_{xy}$)$(H_y)\subset H_x$

for every $y\in$ Som(G), and hence $N_x\subset H_x$.

Let $x$ and $y$ be vertices of Γ. Put $N_{x,y}=\emptyset$ if $x$ and $y$ do not belong to the same connected component of Γ. In the contrary case, let $c$ and $c'$ be classes of paths joining $x$ to $y$ in the quiver $\widetilde{\Gamma}$ associated with Γ. Let $z$ be a vertex of G belonging to the orbit of $y$ and let $\ell$ be an element of Grp(Γ)$_z$; in the group $G_x$, we have the equality:

$$
\delta (c)f_{yz}\delta (\ell )f_{yz}^{-1}\delta (c')^{-1}
$$

$$
=\delta (c)f_{yz}f_{xz}^{-1}(f_{xz}\delta (\ell )f_{xz}^{-1})f_{xz}f_{yz}^{-1}\delta (c)^{-1}\delta (c(c')^{-1})
$$

The arrow $\delta (c(c')^{-1})$ is the class of a loop at $x$ in the quiver Γ, hence belongs to $N_x$, as does the arrow $f_{xz}\delta (\ell )f_{xz}^{-1}$. Since $\delta (c)f_{yz}f_{xz}^{-1}$ belongs to $G_x$ and $N_x$ is a distinguished subgroup of $G_x$, it follows that $\delta (c)f_{yz}\delta (\ell )f_{yz}^{-1}\delta (c')^{-1}$ belongs to $N_x$. Consequently, $\delta (c)N_y\subset N_x\delta (c')$. By symmetry, we have $\delta (c)N_y= N_x\delta (c')$. This implies that this set does not depend on the choice of $c$ and $c'$; we denote it by $N_{x,y}$.

Let N be the subquiver of G whose set of vertices is Som(G) and whose set of arrows joining $x$ to $y$ is equal to $N_{x,y}$ for every pair $(x, y)$ of vertices of G. It is a distinguished subgroupoid of G whose set of arrows contains F; hence H is a subgroupoid of N. In particular, $H_a\subset N_a$, whence the equality.

#### Corollary 1 {#ta-ii-s3-prop-8-cor-1 .statement tag=01TY}

Suppose further that, for every arrow $f$ of F, we have $o(f) =t(f)$. Then the origin and the end of every path in the quiver Γ coincide. Let $a$ be a vertex of G and let A be its orbit in G. For every element $c$ of F whose origin $b$ belongs to A, let us fix an arrow $f_c$ of G joining $a$ to $b$ and put $\kappa (c) =$ Int($f_c$)$(\delta (c)) =$ $f_c\delta (c)f_c^{-1}$.

The group $H_a$ is then the distinguished subgroup of $G_a$ generated by the arrows $\kappa (c)$.

By Prop. 8, the arrows $\kappa (c)$ are contained in the group $H_a$. Let $N_a$ denote the smallest normal subgroup of $G_a$ containing them. By that proposition, it is enough to prove that, for every vertex $b$ of G belonging to A, every arrow $f_{ab}$ joining $a$ to $b$ in G, and every element $c$ of Grp(Γ)$_b$, Int($f_{ab}$)$(\delta (c))$ belongs to $N_a$. Since the origin and the term of every element of F are equal, a loop at a vertex $b$ in the graph $\widetilde{\Gamma}$ is of the form $(b,(f_1, \varepsilon_1), b, . . . ,(f_n, \varepsilon_n), b)$, where for every $i\in  \{1, . . . , n\},f_i$ is an element of F with origin $b$ and $\varepsilon_i\in  \{-1,1\}$. We have

Int($f_{ab}$)$(\delta (c)) =f_{ab}f_c^{-1}\kappa (f_1)^{\varepsilon_1}. . . \kappa (f_n)^{\varepsilon_n}f_cf_{ab}^{-1}$.

Since $f_{ab}f_c^{-1}\in G_a$, it follows that Int($f_{ab}$)$(\delta (c))$ belongs to $N_a$.

#### Corollary 2 {#ta-ii-s3-prop-8-cor-2 .statement tag=01TZ}

If the graph associated with the quiver Γ is a forest, the homomorphism $p_a$ of $G_a$ into $(G/F)_{p(a)}$ is bijective, for every vertex $a$ of G.

In fact, under this assumption, one has Grp(Γ)$_b=\{e_b\}$ for every vertex $b$ of G (Corollary 1 of II, p. 173). It then follows from Proposition 8 that, for every vertex $a$ of G, the group $H_a$ reduces to the identity element.

### 12. Poincaré Group of a Graph

Let G be a graph. Let $a$ be a vertex of G; the isotropy group at $a$ of the groupoid Grp(G) is called the Poincaré group of G at $a$ and is denoted by $\pi_1(G, a)$. Let $c$ be a class of paths in G, and let $a$ be its origin and $b$ its term. The map Int($c$)$:\pi_1(G, b)\rightarrow \pi_1(G, a)$ defined by $c'\mapsto cc'c^{-1}$ is a group isomorphism. Let $\varphi : G\rightarrow H$ be a graph morphism. Let $\theta_G: G\rightarrow$ Grp(G) and $\theta_H: H\rightarrow$ Grp(H) denote the canonical morphisms. If $\overline{\varphi}$ denotes the unique groupoid morphism Grp(G) $\rightarrow$ Grp(H) such that $\overline{\varphi}\circ \theta_G=\theta_H\circ \varphi$, the group homomorphism $\overline{\varphi}_a:\pi_1(G, a)\rightarrow \pi_1(H, \varphi (a))$ is denoted by $\pi_1(\varphi , a)$.

Let G be a connected graph, let S be an orientation of G and let A be a maximal oriented tree of G (II, p. 157, prop. 1). Given vertices $a$ and $b$ of G, there exists a unique class of paths $\gamma_{a,b}$ in the graph $\widetilde{A}$ associated with A which joins $a$ to $b($II, p. 174, cor. 4 of prop. 5). If $a$, $b$ and $c$ are vertices of G, one has $\gamma_{a,b}\gamma_{b,c}=\gamma_{a,c}$, these two classes of paths being equal to the unique class of paths joining $a$ to $c$ in $\widetilde{A}$.

#### Proposition 9 {#ta-ii-s3-prop-9 .statement tag=01U0}

Let $a$ be a vertex of G. There exists a unique homomorphism $\lambda$ of the free group F(S-Fl(A)) into $\pi_1(G, a)$ such that

$$
\lambda (f) =\gamma_{a,o(f)}\cdot f\cdot \gamma_{t(f),a} \tag{1}
$$

for $f\in S$ - Fl(A). The homomorphism $\lambda$ is a group isomorphism.

Let us denote by L the group F(S-Fl(A)). The existence and uniqueness of the homomorphism $\lambda : L\rightarrow \pi_1(G, a)$ satisfying relations (1) follows from A, I, p. 85, prop. 8. Let $\mathscr{L}$ be the groupoid associated with the group L (II, p. 163, example 1); let us denote by $s$ its unique vertex. There exists a unique groupoid morphism $\mu:$ Grp(G) $\rightarrow \mathscr{L}$ such that $\mu(\theta_G(f)) =f$ for every arrow $f\in$ S-Fl(A) and $\mu(\theta_G(f)) =e_s$ for every arrow $f\in$ Fl(A) (II, p. 173, prop. 5). For $f\in$ S-Fl(A), one has $\mu(\theta_G(f)) =f$; the homomorphism $\mu_a\circ \lambda$ is therefore the identity isomorphism of the group L (A, I, p. 85, prop. 8). It follows that $\lambda$ is injective.

Let $\varpi_G/A$ be the groupoid deduced from $\varpi_G$ by contraction of the arrows of A and let $p:\varpi_G\rightarrow \varpi_G/A$ be the canonical groupoid morphism. It is surjective and the group homomorphism $p_a$ deduced from $p$ by passing to the isotropy groups is an isomorphism (II, p. 178, cor. 2 of prop. 8). Since the graph G is assumed connected and A is a maximal tree in it, the groupoid $\varpi_G/A$ has a unique vertex (II, p. 176). Moreover, $\varpi_G$ is generated by $\theta_G(G)$; consequently, $\varpi_G/A$ is generated by the loops $p(f)$, for $f\in S$, and the group $(\varpi_G/A)_{p(a)}$ is generated by the elements of the form $p(\theta_G(f))$, for $f\in$ S-Fl(A). The homomorphism $p_a\circ \lambda$ is therefore surjective. Consequently, $\lambda$ is surjective.

#### Remark 1 {#ta-ii-s3-n12-rem-1 .statement tag=01U1}

The homomorphism $\mu_a$ is the inverse isomorphism of $\lambda$.

#### Remark 2 {#ta-ii-s3-n12-rem-2 .statement tag=01U2}

There exists a unique homomorphism $\lambda :$ F(Fl(G)) $\rightarrow \pi_1(G, a)$ defined by relations (1) for every $f\in$ Fl(G). It follows from proposition 8 that the homomorphism $\lambda$ is surjective and that its kernel is the smallest normal subgroup of F(Fl(G)) containing the elements $f$, for $f\in$ Fl(A), and the elements $f\cdot \overline{f}$, for $f\in$ Fl(G).

## EXERCISES {#ta-ii-s3-exercises}

See the [exercises for § 3](exercises/s3/).
