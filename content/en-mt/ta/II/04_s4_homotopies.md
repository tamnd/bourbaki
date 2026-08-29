---
book: ta
book_title: Topologie algébrique
chapter: II
chapter_title: GROUPOÏDES
section: 4
section_title: Homotopies
lang: en
source: ta-i-iv-fr
book_pages: TA II.180-TA II.196
pdf_pages: 0196-0212
extraction: native
subsections:
    - "no": 1
      title: Définition des homotopies
      page: 180
      pdf_page: 196
    - "no": 2
      title: Homotopismes de groupoïdes
      page: 181
      pdf_page: 197
    - "no": 3
      title: Cohomotopeur
      page: 184
      pdf_page: 200
    - "no": 4
      title: Comparaison de deux cohomotopeurs
      page: 187
      pdf_page: 203
    - "no": 5
      title: Groupes d’isotropie d’un cohomotopeur
      page: 192
      pdf_page: 208
statements: 15
exercises: 0
content_sha256: e32055ea451e7df87f25887fbf6aebc11fc734c7b092667a2f3abc000a796629
translated_from: content/fr/ta/II/04_s4_homotopies.md
source_lang: fr
translation_method: machine
source_content_sha256: 7c34529e46823508056b41a5c7a747e0356444b68c29c0a6cedd12b3172ae48c
translation_model: gpt-5.4
translation_run: translate-en-mt-21bd2be2
glossary_version: 34
glossary_terms_sha256: a385a8503f453217383a11d4003cb17c928f0479d52343f66d2fd506f0652078
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 4. HOMOTOPIES

### 1. Definition of homotopies

#### Definition 1 {#ta-ii-s4-def-1 .statement tag=01U3}

Let G be a groupoid, H a quiver, $\varphi$ and $\varphi '$ morphisms of quivers from H into G. A homotopy connecting $\varphi$ to $\varphi '$ is a mapping $h$ of the set of vertices of H into the set of arrows of G having the following properties:

(i) For every vertex $a$ of H, the arrow $h(a)$ has origin $\varphi (a)$ and end $\varphi '(a)$;

(ii) For every arrow $f$ of H, with origin $a$ and end $b$, one has $\varphi (f)h(b) =h(a)\varphi '(f)$.

One says that $\varphi$ and $\varphi '$ are homotopic if there exists a homotopy connecting $\varphi$ to $\varphi '$.

Let G be a groupoid, let H be a quiver and let $\varphi ,\varphi ',\varphi ''$ be morphisms of quivers from H into G. The mapping $a\mapsto e_{\varphi(a)}$ is a homotopy connecting $\varphi$ to $\varphi$. If $h$ is a homotopy connecting $\varphi$ to $\varphi '$, the mapping $a\mapsto h(a)^{-1}$ is a homotopy connecting $\varphi '$ to $\varphi$. Let $h$ and $h'$ be homotopies connecting $\varphi$ to $\varphi '$ and $\varphi '$ to $\varphi ''$ respectively. For every vertex $a$ of H, the arrows $h(a)$ and $h'(a)$ are composable. The mapping $a\mapsto h(a)h'(a)$ is a homotopy connecting $\varphi$ to $\varphi ''$.

It follows that the relation “ $\varphi$ is homotopic to $\varphi '$ ” is an equivalence relation on the set of morphisms of quivers from H into G.

Let G be a groupoid, H a quiver and $\varphi ,\varphi '$ morphisms of quivers from H into G which are homotopic. By condition (i) of Definition 1, for every vertex $a$ of H, the vertices $\varphi (a)$ and $\varphi '(a)$ belong to one and the same orbit of G.

Suppose moreover that H is a groupoid, and let $h$ be a homotopy joining $\varphi$ to $\varphi '$. The maps Orb($\varphi$ ) and Orb($\varphi '$) deduced from $\varphi$ and $\varphi '$ by passing to orbits are therefore equal. For every vertex $a$ of H and every arrow $f\in H_a$, one has $\varphi (f) =h(a)\varphi '(f)h(a)^{-1}=$ Int($h(a)$)$(\varphi '(f))$, by condition (ii) of Definition 1. In other words, the homomorphism $\varphi_a$ is equal to Int($h(a)$)$\circ \varphi '_a$. In particular, if the homomorphism $\varphi_a$ is injective (resp. bijective, resp. surjective), the same is true of the homomorphism $\varphi '_a$.

#### Remark 1 {#ta-ii-s4-n1-rem-1 .statement tag=01U4}

Let G, $G'$ be groupoids, H, $H'$ quivers, let $u: H'\rightarrow H$ be a morphism of quivers and $v: G\rightarrow G'$ a morphism of groupoids. If morphisms of quivers $\varphi ,\varphi '$ of H into G are homotopic, the morphisms of quivers $v\circ \varphi \circ u$ and $v\circ \varphi '\circ u$ of $H'$ into $G'$ are homotopic. More precisely, if $h$ is a homotopy joining $\varphi$ to $\varphi '$, the map Fl($v$)$\circ h\circ$ Som($u$) is a homotopy joining $v\circ \varphi \circ u$ to $v\circ \varphi '\circ u$.

#### Remark 2 {#ta-ii-s4-n1-rem-2 .statement tag=01U5}

Let G be a groupoid, let H be a quiver, and let $\varphi , \psi$ be morphisms of quivers of H into G. Let us denote by $j$ the canonical morphism of H into Grp(H), and let $\overline{\varphi}$ and $\overline{\psi}$ be the morphisms of groupoids of Grp(H) into G such that $\overline{\varphi}\circ j=\varphi$ and $\overline{\psi}\circ j=\psi$.

Recall that Som(H) = Som(Grp(H)).

A homotopy $h:$ Som(H) $\rightarrow$ Fl(G) joining $\varphi$ to $\psi$ is a homotopy joining $\overline{\varphi}$ to $\overline{\psi}$.

### 2. Homotopisms of groupoids

In this No$^o$, we shall use the notation $u\sim v$ to express that two morphisms of groupoids $u$ and $v$ are homotopic.

#### Definition 2 {#ta-ii-s4-def-2 .statement tag=01U6}

Let G, $G'$ be groupoids and let $\varphi$ be a morphism from G into $G'$. An inverse up to homotopy of $\varphi$ is a groupoid morphism $\psi$ from $G'$ into G such that the morphisms $\psi \circ \varphi$ and $\varphi \circ \psi$ are respectively homotopic to Id$_G$ and to Id$_{G'}$. One says that $\varphi$ is a homotopism if there exists an inverse of $\varphi$ up to homotopy.

An isomorphism of groupoids is a homotopism.

Let G and $G'$ be groupoids. Let $\varphi ,\varphi '$ be groupoid morphisms from G into $G'$ which are homotopic. If $\varphi$ is a homotopism, the same is true of $\varphi '$. In fact, if $\psi$ denotes an inverse of $\varphi$ up to homotopy, one has $\psi \circ \varphi '\sim \psi \circ \varphi \sim$ Id$_G$ and $\varphi '\circ \psi \sim \varphi \circ \psi \sim$ Id$_{G'}$, which proves that $\psi$ is an inverse up to homotopy of $\varphi '$.

Let G, $G',G''$ be groupoids and let $\varphi : G\rightarrow G',\varphi ': G'\rightarrow G''$, $\psi : G'\rightarrow G,\psi ': G''\rightarrow G'$ be groupoid morphisms. Then, of the following conditions:

(i) $\psi$ is an inverse up to homotopy of $\varphi$;

(ii) $\psi '$ is an inverse up to homotopy of $\varphi '$;

(iii) $\psi \circ \psi '$ is an inverse up to homotopy of $\varphi '\circ \varphi$; any two imply the third. In fact, suppose first that (i) and (ii) are satisfied; one then has

$\psi \circ \psi '\circ \varphi '\circ \varphi \sim \psi \circ$ Id$_{G'}\circ \varphi \sim \psi \circ \varphi \sim$ Id$_G$

and, analogously, $\varphi '\circ \varphi \circ \psi \circ \psi '\sim$ Id$_{G'}$, whence (iii). If (i) and (iii) are satisfied,

$\varphi '\circ \psi '\sim \varphi '\circ \varphi \circ \psi \circ \psi '\sim$ Id$_{G''}$

and

$\psi '\circ \varphi '\sim (\varphi \circ \psi )\circ \psi '\circ \varphi '\circ (\varphi \circ \psi )\sim \varphi \circ \psi \sim$ Id$_{G'}$,

whence condition (ii). The proof that conditions (ii) and (iii) imply condition (i) is analogous.

In particular, if two of the morphisms $\varphi ,\varphi ',\varphi '\circ \varphi$ are homotopisms, the same is true of the third.

#### Proposition 1 {#ta-ii-s4-prop-1 .statement tag=01U7}

Let G, $G'$ be groupoids, let $\varphi$ be a morphism from G into $G'$, and let A be a subset of the set of vertices of G which meets every orbit of G. In order that $\varphi$ be a homotopism, it is necessary and sufficient that the following conditions be satisfied:

(i) the mapping Orb($\varphi$ ) from Orb(G) into Orb(G$'$), deduced from $\varphi$ by passing to orbits, is bijective;

(ii) for every $a\in A$, the homomorphism $\varphi_a: G_a\rightarrow G'_{\varphi(a)}$ is bijective.

Suppose first that $\varphi$ is a homotopism and let $\psi$ be an inverse of $\varphi$ up to homotopy. Then,

Orb($\psi$ )$\circ$ Orb($\varphi$ ) $=$ Orb($\psi \circ \varphi$ ) $=$ Orb(Id$_G$) $=$ Id$_{Orb(G)}$,

for two homotopic groupoid morphisms induce the same mapping by passing to orbits. Analogously, Orb($\varphi$ )$\circ$ Orb($\psi$ ) $=$ Id$_{Orb(G')}$. The mapping Orb($\varphi$ ) is therefore bijective, whence assertion (i). We also have, for every vertex $a$ of G,

$$
\psi_{\varphi(a)}\circ \varphi_a= (\psi \circ \varphi )_a
$$

since $\psi \circ \varphi$ is homotopic to Id$_G$, the homomorphism $(\psi \circ \varphi )_a$ is bijective (cf. p. 180), so that $\varphi_a$ is injective and $\psi_{\varphi(a)}$ is surjective. On interchanging the roles of $\varphi$ and $\psi$, we see that $\varphi_a$ is also surjective, whence condition (ii).

Suppose now that conditions (i) and (ii) are satisfied, and let us prove that $\varphi$ is a homotopism.

Let us first treat the case where each orbit of $G'$ is reduced to a point.

For each vertex $b$ of $G'$, choose a vertex $u(b)$ of G belonging to A and whose image under $\varphi$ is $b$. This is possible because the mapping Orb($\varphi$ ) is surjective and A meets each orbit of G. Let $f$ be an arrow of $G'$; we have $o(f) =t(f)$ by hypothesis; put $b=o(f)$ and $a=u(b)$. By condition (ii), there exists a unique arrow $v(f)\in G_a$ whose image under $\varphi$ is $f$. The pair $\psi = (u, v)$ is a groupoid morphism from $G'$ into G. Let us prove that $\psi$ is inverse to $\varphi$ up to homotopy. We already have $\varphi \circ \psi =$ Id$_{G'}$ by construction of $\psi$.

Let $x$ be a vertex of G. Put $a=\psi (\varphi (x))$; this is an element of A such that $\varphi (a) =\varphi (x)$. Since Orb($\varphi$ ) is injective, $a$ belongs to the orbit of $x$ in G and there exists an arrow $f$ in G joining $a$ to $x$. The arrow $h(x) =\psi (\varphi (f))^{-1}f$ then joins $a$ to $x$ and one has $\varphi (h(x)) =e_{\varphi(a)}$.

Let us show that the mapping $h:$ Som(G) $\rightarrow$ Fl(G) resulting is a homotopy joining $\psi \circ \varphi$ to Id$_G$. Condition (i) of definition 1 is satisfied, by construction. Let $f$ be an arrow of G$,x$ its origin and $y$ its term. One has $\varphi (x) =\varphi (y)$ ; put $a=\psi (\varphi (x)) =\psi (\varphi (y))$. The arrows $h(x)f h(y)^{-1}$ and $\psi \circ \varphi (f)$ belong to $G_a$ and both have image $\varphi (f)$ in $G'_{\varphi(a)}$. Since the mapping $\varphi_a$ is injective, one has $h(x)f h(y)^{-1}=\psi \circ \varphi (f)$. Condition (ii) of definition 1 is thus satisfied.

Let us now prove proposition 1 in the general case. Let X be a maximal oriented forest of $G'($II, p. 157, prop. 1). Let $G''$ be the groupoid deduced from $G'$ by contraction of the arrows of X and let $\varphi ': G'\rightarrow G''$ be the canonical morphism. The morphism $\varphi '$ satisfies the conditions of prop. 1 (II, p. 170, remark 1 and p. 178, cor. 2), and hence the same is true of the morphism $\varphi '\circ \varphi$.

Since the orbits of $G''$ are reduced to points, it follows from the special case already proved that $\varphi '$ and $\varphi '\circ \varphi$ are homotopisms, so that $\varphi$ is likewise one. This completes the proof of the proposition.

#### Corollary 1 {#ta-ii-s4-prop-1-cor-1 .statement tag=01U8}

Let G be a groupoid, let A be a set and let $f: A\rightarrow$ Som(G) be a mapping. If the image of $f$ meets each orbit of G, the canonical groupoid morphism $\varphi$ of $f^*G$ into G is a homotopism.

By definition of the inverse image groupoid (II, p. 166, example 4), A is the set of vertices of the groupoid $f^*G$ and one has Fl$_{a,b}(f^*G) =$ Fl$_{f(a),f(b)}(G)$ for every pair $(a, b)$ of elements of A. Moreover, one has Som($\varphi$ ) $=f$ and Fl($\varphi$ ) induces the identical mapping of Fl$_{a,b}(f^*G)$ into Fl$_{f(a),f(b)}(G)$. Consequently, the mapping Orb($\varphi$ ) is bijective and the homomorphism $\varphi_a: (f^*G)_a\rightarrow G_{f(a)}$ is an isomorphism, for every $a\in A$. The hypotheses of proposition 1 are therefore satisfied.

#### Corollary 2 {#ta-ii-s4-prop-1-cor-2 .statement tag=01U9}

Let G be a groupoid, let X be an oriented forest of G, let $G'$ be the groupoid deduced from G by contraction of the arrows of X. The canonical morphism of G into $G'$ is a homotopism.

It follows in fact from remark 1 of II, p. 170 and corollary 2 of II, p. 178 that the hypotheses of proposition 1 are satisfied.

### 3. Cohomotoper

Let H be a quiver, let G be a groupoid and let $\varphi$ and $\psi$ be quiver morphisms of H into G.

Let $G_1$ denote the quiver defined as follows: the vertices of $G_1$ are those of G; the arrows of $G_1$ are the elements of the sum of the sets Fl(G) and Som(H); the origin mapping of $G_1$ coincides with that of G on Fl(G) and with Som($\varphi$ ) on Som(H); the term mapping of $G_1$ coincides with that of G on Fl(G) and with Som($\psi$ ) on Som(H). Let $\alpha_1$ denote the quiver morphism from G into $G_1$ defined by the identity mapping of Som(G) and by the canonical injection of Fl(G) into Fl(G$_1$). Let $h_1$ denote the canonical injection Som(H) $\rightarrow$ Fl(G$_1$).

Consider the free groupoid Grp(G$_1$) constructed on $G_1($II, p. 174, def. 9), and let $\theta_1$ denote the canonical quiver morphism of $G_1$ into Grp(G$_1$). Lastly, denote by Coh($\varphi , \psi$ ) the groupoid deduced from Grp(G$_1$) by contraction of the loops (at the origin of $x$)

$$
\alpha_1(x)\alpha_1(y)\alpha_1(xy)^{-1} \tag{1}
$$

for every pair $(x, y)$ of composable arrows of G, as well as of the loops (at $\varphi (a)$)

$$
\alpha_1(\varphi (f))h_1(b)\alpha_1(\psi (f))^{-1}h_1(a)^{-1} \tag{2}
$$

for $a,b$ in Som(H) and $f\in$ Fl$_{ab}(H)$. Let $\pi :$ Grp(G$_1$)$\rightarrow$ Coh($\varphi , \psi$ ) denote the canonical morphism; let $\alpha$ = $\pi \circ \theta_1\circ \alpha_1$ and $h=$ Fl($\pi \circ \theta_1$)$\circ h_1$.

#### Proposition 2 {#ta-ii-s4-prop-2 .statement tag=01UA}

The groupoid Coh($\varphi , \psi$ ) is generated by the subquiver whose set of vertices is Som(G) and whose set of arrows is the union of the images of the mappings Fl($\alpha$ ) and $h$.

This subquiver being the image of the quiver $G_1$ under the quiver morphism $\pi \circ \theta_1$, the proposition follows at once from the construction of Coh($\varphi , \psi$ ).

#### Proposition 3 {#ta-ii-s4-prop-3 .statement tag=01UB}

The quiver morphism $\alpha$ is a groupoid morphism from G into Coh($\varphi , \psi$ ), and the mapping $h$ is a homotopy joining $\alpha \circ \varphi$ to $\alpha \circ \psi$.

The triple (Coh($\varphi , \psi$ )$, \alpha , h$) has the following universal property: if $G'$ is a groupoid, $\alpha '$ a morphism of groupoids from G into $G'$ and $h':$ Som(H) $\rightarrow$ Fl(G$'$) a homotopy joining $\alpha '\circ \varphi$ to $\alpha '\circ \psi$, there exists a unique morphism of groupoids $\eta :$ Coh($\varphi , \psi$ )$\rightarrow G'$ such that

(3) $\alpha '=\eta \circ \alpha$ and $h'=$ Fl($\eta$ )$\circ h$.

In view of the definition of the groupoid deduced by contraction of arrows, the contraction of the loops (1) implies that $\alpha$ is a morphism of groupoids, and the contraction of the loops (2) that $h$ is a homotopy joining $\alpha \circ \varphi$ to $\alpha \circ \psi$.

Let $G',\alpha ',h'$ be as in the statement. Let $\eta_1$ be the morphism of quivers from $G_1$ into $G'$ such that Som($\eta_1$) is equal to Som($\alpha '$) and such that Fl($\eta_1$) coincides with Fl($\alpha '$) on Fl(G) and with $h'$ on Som(H). There exists a unique morphism of groupoids $\eta_2:$ Grp(G$_1$)$\rightarrow G'$ such that $\eta_1=\eta_2\circ \theta_1$. Since $\alpha '$ is a morphism of groupoids and $h'$ is a homotopy joining $\alpha '\circ \varphi$ to $\alpha '\circ \psi ,\eta_2$ defines by passing to the quotient a morphism of groupoids $\eta$ from Coh($\varphi , \psi$ ) into $G'($II, p. 170, proposition 3). This morphism satisfies relations (3), and it is the only one (II, p. 185, proposition 2).

#### Definition 3 {#ta-ii-s4-def-3 .statement tag=01UC}

The groupoid Coh($\varphi , \psi$ ) is called the cohomotopizer of the pair $(\varphi , \psi )$. One says that $\alpha$ is the canonical morphism from G into Coh($\varphi , \psi$ ) and that $h$ is the canonical homotopy joining $\alpha \circ \varphi$ to $\alpha \circ \psi$.

The quiver whose set of vertices is the set of orbits of G, whose set of arrows is the set of connected components of H, and whose origin and end mappings are deduced from $\varphi$ and $\psi$ by passing to the quotients is called the framework of the pair $(\varphi , \psi )$.

#### Proposition 4 {#ta-ii-s4-prop-4 .statement tag=01UD}

The mapping Orb($\alpha$ )$:$ Orb(G) $\rightarrow$ Orb(Coh($\varphi , \psi$ )) is surjective; its fibres are the connected components of the framework of the pair $(\varphi , \psi )$.

The morphism $\alpha$ is the composite of the morphisms $\alpha_1: G\rightarrow G_1$, $\theta_1: G_1\rightarrow$ Grp(G$_1$) and $\pi :$ Grp(G$_1$)$\rightarrow$ Coh($\varphi , \psi$ ). The mapping $\theta_1$ induces a bijection of the set of connected components of the quiver $G_1$ onto the set of orbits of Grp(G$_1$), and the mapping Orb($\pi$ )$:$ Orb(Grp(G$_1$))$\rightarrow$ Orb(Coh($\varphi , \psi$ )) is bijective (II, p. 170, remark 1). It is therefore enough to prove that the mapping of Orb(G) into $\pi_0(G_1)$ deduced from $\alpha_1$ is surjective and that its fibres are the connected components of the framework of the pair $(\varphi , \psi )$. The surjectivity results from the fact that the mapping Som($\alpha_1$) is the identity mapping. The equivalence relation in Som(G) defined by “$a$ and $b$ are in the same connected component of $G_1$” is generated by the relations “there exists an arrow of G joining $a$ to $b$” and “there exists a vertex $h$ of H such that $\varphi (h) =a$ and $\psi (h) =b$”. This equivalence relation is compatible with the mapping of Som(G) into Orb(G), and the relation deduced from it in Orb(G) is generated by the relation “there exists an orbit $\eta$ of H such that Orb($\varphi$ )$(\eta ) =\alpha$ and Orb($\psi$ )$(\eta ) =\beta$”. It is therefore the relation “$\alpha$ and $\beta$ are in the same connected component of the framework of the pair $(\alpha , \beta )$”.

#### Proposition 5 {#ta-ii-s4-prop-5 .statement tag=01UE}

Let $G'$ be a groupoid, let $\eta ,\eta '$ be groupoid morphisms of Coh($\varphi , \psi$ ) into $G'$, and let $k$ be a mapping of Som(G) into Fl(G$'$). In order that $k$ be a homotopy joining $\eta$ to $\eta '$, it is necessary and sufficient that the following two conditions be satisfied:

(i) The mapping $k$ is a homotopy joining $\eta \circ \alpha$ to $\eta '\circ \alpha$;

(ii) For every vertex $a$ of H, one has

$$
\eta (h(a))k(\psi (a)) =k(\varphi (a))\eta '(h(a))
$$

By definition, in order that $k$ be a homotopy joining $\eta$ to $\eta '$, it is necessary and sufficient that the following two conditions be fulfilled (recall that Som(G) = Som(Coh($\varphi , \psi$ ))) :

a) For every vertex $x$ of Coh($\varphi , \psi$ )$,k(x)$ joins $\eta (x)$ to $\eta '(x)$ ;

b) For every pair $(x, y)$ of vertices of Coh($\varphi , \psi$ ) and every arrow $f\in$ Fl$_{x,y}$(Coh($\varphi , \psi$ )), one has $\eta (f)k(y) =k(x)\eta '(f)$.

By Prop. 2, it is enough to verify condition b) when $f$ belongs to the image of Fl($\alpha$ ) or to that of $h$, so that b) is equivalent to the conjunction of the two conditions c) and d) below:

c) For $x\in$ Som(G), $y\in$ Som(G) and $g\in$ Fl$_{x,y}(G)$, one has $\eta (\alpha (g))k(y) =k(x)\eta '(\alpha (g))$;

d) For every $a\in$ Som(H), one has $\eta (h(a))k(\psi (a)) =k(\varphi (a))\eta '(h(a))$. Condition (i) is equivalent to the conjunction of a) and c), and condition (ii) is condition d), whence the corollary.

### 4. Comparison of two cohomotopisers

Consider a diagram

H $^{\varphi}$ G

$$
u^{\psi}_v \tag{4}
$$

$$
{H'}^{\varphi'}_{\psi'}G'
$$

where H, $H'$, G, $G'$ are groupoids and $u,v,\varphi ,\psi ,\varphi ',\psi '$ are morphisms of groupoids such that $v\circ \varphi =\varphi '\circ u$ and $v\circ \psi =\psi '\circ u$.

Let $\alpha$ denote the canonical morphism of G into the cohomotopiser Coh($\varphi , \psi$ ) and $h$ the canonical homotopy joining $\alpha \circ \varphi$ to $\alpha \circ \psi$; define $\alpha '$ and $h'$ analogously. Then $\alpha '\circ v$ is a morphism of groupoids of G into Coh($\varphi ', \psi '$) and $h'\circ$ Som($u$) is a homotopy joining $\alpha '\circ \varphi '\circ u$ to $\alpha '\circ \psi '\circ u$, that is to say $\alpha '\circ v\circ \varphi$ to $\alpha '\circ v\circ \psi$. By the universal property of cohomotopisers (II, p. 185, Prop. 3), there exists a unique morphism of groupoids $w$ of Coh($\varphi , \psi$ ) into Coh($\varphi ', \psi '$) such that $w\circ \alpha =\alpha '\circ v$ and Fl($w$)$\circ h=h'\circ$ Som($u$). In particular, we have extended diagram (4) to a diagram

H $^{\varphi}$ G $^{\alpha}$ Coh($\varphi , \psi$ )

$$
u^{\psi}_vw \tag{5}
$$

${H'}^{\varphi'}_{\psi'}{G'}^{\alpha'}$ Coh($\varphi ', \psi '$)

in which the second square is commutative.

#### Theorem 1 {#ta-ii-s4-thm-1 .statement tag=01UF}

Make the following hypotheses:

(i) the morphism of groupoids $v$ is a homotopism;

(ii) the mapping Orb($u$)$:$ Orb(H) $\rightarrow$ Orb(H$'$), deduced from $u$ by passing to orbits, is bijective;

(iii) there exists in each orbit of H a point $a$ such that the homomorphism $u_a: H_a\rightarrow H'_{u(a)}$ is surjective.

Then, the groupoid morphism $w:$ Coh($\varphi , \psi$ )$\rightarrow$ Coh($\varphi ', \psi '$) is a homotopism.

Let $G''$ be the groupoid deduced from $G'$ by contraction of the arrows of a maximal oriented forest. The canonical morphism $v': G'\rightarrow G''$ is a homotopism (II, p. 184, corollary 2 of prop. 1). The two diagrams

H $^{\varphi}$ G ${H'}^{\varphi'}G'$

$u\psi v'\circ v$ et Id$_{H'}\psi 'v'$

$$
H'vv''\circ \circ \psi \varphi ''G'H'vv''\circ \circ \psi \varphi ''G''
$$

give rise to groupoid morphisms $w'_1:$ Coh($\varphi , \psi$ )$\rightarrow$ Coh($v'\circ \varphi ', v'\circ \psi '$) and $w'_2:$ Coh($\varphi ', \psi '$)$\rightarrow$ Coh($v'\circ \varphi ', v'\circ \psi '$) ; we have $w'_1=w'_2\circ w$. It is therefore enough to prove that $w'_1$ and $w'_2$ are homotopisms. Since the mappings Som($v'\circ v$)$:$ Som(G) $\rightarrow$ Som(G$''$) and Som($v'$)$:$ Som(G$'$)$\rightarrow$ Som(G$''$) are surjective, it is consequently enough to prove the theorem under the additional assumption that the mapping Som($v$) is surjective, an assumption that we shall make throughout the remainder of the proof.

Let us prove successively the following assertions:

– The mapping Orb($w$) is bijective;

– For every vertex $a$ of G, the homomorphism $w_a$ is surjective;

– For every vertex $a$ of G, the homomorphism $w_a$ is injective.

a) By assumption, the mapping Orb($u$) is bijective; the same is true of the mapping Orb($v$) by II, p. 182, prop. 1, since $v$ is a homotopism. The morphism of quivers from the framework of the pair $(\varphi , \psi )$ to that of the pair $(\varphi ', \psi ')$ defined by the mappings Orb($u$) and Orb($v$) is therefore an isomorphism. In particular, the mapping deduced from it by passing to connected components is bijective. Prop. 4 of II, p. 185 then implies that the mapping Orb($w$) is bijective.

(b) Let $f'$ be an arrow of $G'$, and let us denote by $a'$ its origin and by $b'$ its term. Since the mapping Som($v$) is surjective, there exist vertices $a$ and $b$ in G such that $a'=v(a)$ and $b'=v(b)$. Since the morphism $v$ is a homotopism, there exist an arrow $f$ of G joining $a$ to $b$ and an element $g\in G_a$ such that $v(g) =f'v(f)^{-1}($II, p. 182, prop. 1), whence $f'=v(gf)$. This proves that the mapping Fl($v$) is surjective.

Let us then prove that the mapping Fl($w$) is surjective. Its image contains that of Fl($\alpha '$), for one has $\alpha '\circ v=w\circ \alpha$ and the mapping Fl($v$) is surjective. Let $b$ be a vertex of $H'$; let $a$ be a vertex of H such that $b$ and $u(a)$ are in the same orbit of $H'$, and let $f$ be an arrow of $H'$ joining $u(a)$ to $b$. Then,

$$
h'(u(a))\cdot (\alpha '\circ \psi ')(f) = (\alpha '\circ \varphi ')(f)\cdot h'(b)
$$

since $h'$ is a homotopy joining $\alpha '\circ \varphi '$ to $\alpha '\circ \psi '$. The arrow $h'(u(a)) =$ $w(h(a))$ belong to the image of Fl($w$), and so do the two arrows $\alpha '(\psi '(f))$ and $\alpha '(\varphi '(f))$ by what precedes. It follows that the arrow $h'(b)$ belong to the image of Fl($w$), which proves that the image of Fl($w$) contains that of $h'$. By prop. 2 of II, p. 185, the mapping Fl($w$) is surjective.

Let $g'\in$ Coh($\varphi ', \psi '$)$_{u(a)}$. Let $g$ be an arrow of Coh($\varphi , \psi$ ) such that $w(g) =g'$. Let us denote by $x$ and $y$ the origin and the end of $g$; one has $u(x) =$ $u(y) =u(a)$. Let $g_1$ (resp. $g_2$) be an arrow of G joining $a$ to $x$ (resp. $a$ to $y$) whose image under $v$ is $e_{u(a)}$. Then, $\alpha (g_1)g\alpha (g_2)^{-1}$ is an element of Coh($\varphi , \psi$ )$_a$ whose image under $w_a$ is $g'$. Hence, for every vertex $a$ of G, the homomorphism $w_a$ is surjective.

c) Let us prove that, for every vertex $a$ of G, the homomorphism $w_a$ is injective. By considering successively the diagrams

$$\begin{array}{ccccccc} H & \underset{\psi}{\overset{\varphi}{\rightrightarrows}} & G & & H & \underset{v\circ\psi}{\overset{v\circ\varphi}{\rightrightarrows}} & G' \\ {\scriptstyle \mathrm{Id}_H}\big\downarrow & & \big\downarrow{\scriptstyle v} & \text{and} & {\scriptstyle u}\big\downarrow & & \big\downarrow{\scriptstyle \mathrm{Id}_{G'}} \\ H & \underset{v\circ\psi}{\overset{v\circ\varphi}{\rightrightarrows}} & G' & & H' & \underset{\psi'}{\overset{\varphi'}{\rightrightarrows}} & G' \end{array}$$

one is thus reduced to treating the two following cases: 1) One has $H'= H$ and $u=$ Id$_H; 2)$ One has $G'= G$ and $v=$ Id$_G$.

1) Suppose that one has $H'= H$ and $u=$ Id$_H$.

Consider a morphism of groupoids $v': G'\rightarrow G$ which is an inverse of $v$ up to homotopy and a homotopy $k:$ Som(G) $\rightarrow$ Fl(G) joining $v'\circ v$ to Id$_G$. By Remark 1 of II, p. 181, the mappings $\alpha \circ k\circ \varphi$ and $\alpha \circ k\circ \psi$ are homotopies joining respectively $\alpha \circ v'\circ \varphi '$ to $\alpha \circ \varphi$ and $\alpha \circ v'\circ \psi '$ to $\alpha \circ \psi$. Hence (cf. II, p. 180), the mapping

$h_1:$ Som(H) $\rightarrow$ Fl(Coh($\varphi , \psi$ )),

$$
x\mapsto (\alpha \circ k\circ \varphi )(x)\cdot h(x)\cdot ((\alpha \circ k\circ \psi )(x))^{-1}
$$

is a homotopy joining $\alpha \circ v'\circ \varphi '$ to $\alpha \circ v'\circ \psi '$. By the universal property of cohomotopers (II, p. 185, prop. 3), there exists a unique groupoid morphism $w':$ Coh($\varphi ', \psi '$)$\rightarrow$ Coh($\varphi , \psi$ ) such that $\alpha \circ v'=$ $w'\circ \alpha '$ and $h_1=$ Fl($w'$)$\circ h'$.

H $^{\varphi}_{\psi}$ G $^{\alpha}$ Coh($\varphi , \psi$ )

Id$_Hvw$

H $^{\varphi'}_{\psi'}{G'}^{\alpha'}$ Coh($\varphi ', \psi '$)

Id$_Hv'w'$

H $^{\varphi}_{\psi}$ G $^{\alpha}$ Coh($\varphi , \psi$ ) .

In particular one has

$$
\alpha \circ v'\circ v=w'\circ \alpha '\circ v=w'\circ w\circ \alpha
$$

Since $k$ is a homotopy joining $v'\circ v$ to Id$_G,\alpha \circ k$ is a homotopy joining $w'\circ w\circ \alpha$ to $\alpha$. Since Fl($w'\circ w$)$\circ h=$ Fl($w'$)$\circ h'=h_1$, one has, for every vertex $x$ of H,

Fl($w'\circ w$)$\circ h(x)\cdot (\alpha \circ k\circ \psi )(x) =h_1(x)\cdot (\alpha \circ k\circ \psi )(x) = (\alpha \circ k\circ \varphi )(x)\cdot h(x)$,

by definition of $h_1$. By prop. 5 of II, p. 186, applied to the groupoid morphisms $w'\circ w$ and Id$_{Coh(\varphi ,\psi)}$, the mapping $\alpha \circ k$ is a homotopy joining $w'\circ w$ to Id$_G$. In particular, $w'\circ w$ is a homotopism.

For every vertex $a$ of G, the group homomorphism $(w'\circ w)_a$ is therefore bijective (II, p. 182, prop. 1). It follows that the homomorphism $w_a$ is injective, whence the result in case A).

2) Suppose that one has $G'= G$ and $v=$ Id$_G$.

Let $x$ be a vertex of $H'$. Since the mapping Orb($u$) is surjective, there exist a vertex $a$ of H and an arrow $f$ of $H'$ joining $u(a)$ to $x$. The arrows $\alpha (\varphi '(f))^{-1},h(a)$ and $\alpha (\psi '(f))$ join respectively $\varphi '(x)$ to $\varphi '(u(a)) =\varphi (a),\varphi (a)$ to $\psi (a)$ and $\psi '(u(a)) =\psi (a)$ to $\psi '(x)$, and therefore are composable in Coh($\varphi , \psi$ ). Put

$$
h_2(x) =\alpha (\varphi '(f))^{-1}\cdot h(a)\cdot \alpha (\psi '(f))
$$

Let us verify that the resulting arrow $h_2(x)$ does not depend on the chosen elements $a$ and $f$. Let $a'$ be a vertex of H and let $f'$ be an arrow of $H'$ joining $u(a')$ to $x$. Since the mapping Orb($u$) is injective, the vertices $a$ and $a'$ of H belong to the same orbit and there exists an arrow $c\in$ Fl(H) joining $a$ to $a'$. Then $u(c)f'f^{-1}$ is a loop at $u(a)$ in $H'$. By hypothesis (iii), there exists a vertex $b$ of H such that the homomorphism $u_b$ is surjective and an arrow $c'$ of H joining $b$ to $a$; then, Int($u(c')$)$(u(c)f'f^{-1})$ is a loop at $u(b)$ in H, and is therefore the image under $u_b$ of a loop $c''$ at $b$. Consequently, the arrow $g= (c'c)^{-1}c''c'$ of H joins the vertex $a'$ to the vertex $a$ and satisfies $f'=u(g)f$. We then have

$$
\alpha (\varphi '(f'))^{-1}h(a')\alpha (\psi '(f'))
$$

$$
=\alpha (\varphi '(f))^{-1}\alpha (\varphi '(u(g)))^{-1}h(a')\alpha (\psi '(u(g)))\alpha (\psi '(f))
$$

$$
=\alpha (\varphi '(f))^{-1}\alpha (\varphi (g))^{-1}h(a')\alpha (\psi (g))\alpha (\psi '(f))
$$

$$
=\alpha (\varphi '(f))^{-1}\cdot h(a)\cdot \alpha (\psi '(f))
$$

since $h$ is a homotopy joining $\alpha \circ \varphi$ to $\alpha \circ \psi$. This proves the announced independence.

By construction, we have $h_2(u(x)) =h(x)$ for all $x\in$ Som(H). Thus we have defined a mapping $h_2$ of Som(H$'$) into Fl(Coh($\varphi , \psi$ )). Let $c$ be an arrow of $H'$, and let $x$ denote its origin and $y$ its end. Let $a$ be a vertex of H and $f$ an arrow of $H'$ joining $u(a)$ to $x$. Then $f c$ is an arrow of $H'$ joining $u(a)$ to $y$. By definition of $h_2$, we thus have

$$
h_2(x)\alpha (\psi '(c)) =\alpha (\varphi '(f))^{-1}h(a)\alpha (\psi '(f))\alpha (\psi '(c))
$$

$$
=\alpha (\varphi '(c))\alpha (\varphi '(f c))^{-1}h(a)\alpha (\psi '(f c))
$$

$$
=\alpha (\varphi '(c))h_2(y)
$$

This proves that $h_2$ is a homotopy joining $\alpha \circ \varphi '$ to $\alpha \circ \psi '$.

By the universal property of cohomotopizers, there exists a unique morphism of groupoids $w':$ Coh($\varphi ', \psi '$)$\rightarrow$ Coh($\varphi , \psi$ ) such that $w'\circ \alpha '=\alpha$ and $h_2$ = Fl($w'$)$\circ h'$. We have $w'\circ w\circ \alpha =w'\circ \alpha '=\alpha$ and Fl($w'\circ w$)$\circ h=$ Fl($w'$)$\circ h'\circ$ Som($u$) $=h_2\circ u=h$ by definition of $h_2$. By the universal property of cohomotopizers, this implies that we have $w'\circ w=$ Id$_{Coh(\varphi ,\psi)}$. In particular, for every $a\in$ Som(G), the homomorphism $w_a$ is injective.

It then follows from Prop. 1 of II, p. 182 that the morphism $w$ is a homotopism, whence the theorem.

### 5. Isotropy Groups of a Cohomotopizer

Let G and H be groupoids, and let $\varphi ,\psi$ be morphisms of groupoids from H into G. The purpose of this n$^o$ is to calculate the isotropy groups of the cohomotopizer Coh($\varphi , \psi$ ). We again take up the notations $G_1, h_1, \theta_1, \alpha , h$ of n$^o3$.

Let $\Gamma_0$ denote the framework of the pair $(\varphi , \psi )$; let us recall (II, p. 185, Def. 3) that this is the quiver (Orb(G), Orb(H)$, \varphi_0, \psi_0$), where $\varphi_0$ and $\psi_0$ are the mappings of Orb(H) into Orb(G) deduced from the mappings $\varphi$ and $\psi$ by passing to orbits.

In all that follows in this No., we shall moreover suppose that the quiver $\Gamma_0$ is connected and nonempty; by II, p. 185, Prop. 4, this amounts to supposing that the groupoid Coh($\varphi , \psi$ ) is transitive, or again that the quiver $G_1$ is connected and nonempty (II, p. 185, Prop. 2).

#### Definition 4 {#ta-ii-s4-def-4 .statement tag=01UG}

An underlying equipment of the pair $(\varphi , \psi )$ is said to be given by the data:

(i) For every $i\in$ Orb(G), of a vertex $a(i)$ in the orbit $i$ of G;

(ii) For every $j\in$ Orb(H), of a vertex $b(j)$ in the orbit $j$ of H;

(iii) For every $j\in$ Orb(H), of arrows $c_1(j)$ and $c_2(j)$ of G joining respectively $\varphi (b(j))$ to $a(\varphi_0(j))$ and $\psi (b(j))$ to $a(\psi_0(j))$;

(iv) Of a subquiver T of the framework $\Gamma_0$ whose associated graph is a maximal tree of the graph $\widetilde{\Gamma}_0$;

(v) Of an orbit $i_0$ of G.

Let us choose an underlying equipment $(a, b, c_1, c_2,T, i_0)$ of the pair $(\varphi , \psi )$. We define a quiver morphism $\tau_1$ of $\Gamma_0$ into Grp(G$_1$) by setting $\tau_1(i) =a(i)$ for $i\in$ Som(Γ$_0$) $=$ Orb(G) and

$$
\tau_1(j) =c_1(j)^{-1}\cdot h_1(b(j))\cdot c_2(j)
$$

for $j\in$ Fl(Γ$_0$) $=$ Orb(H). We shall denote by $\tau_0$ the composite of $\tau_1$ and the canonical morphism $\theta_1$ of Grp(G$_1$) into Coh($\varphi , \psi$ ) ; it is a quiver morphism of $\Gamma_0$ into Coh($\varphi , \psi$ ).

For $i\in$ Orb(G), let us denote by $\alpha_i: G_{a(i)}\rightarrow$ Coh($\varphi , \psi$ )$_{a(i)}$ the group homomorphism deduced from the morphism $\alpha : G\rightarrow$ Coh($\varphi , \psi$ ) by restriction to the isotropy groups at $a(i)$.

For $j\in$ Orb(H), let us denote

$\varphi_j=$ Int($c_1(j)$)$^{-1}\circ \varphi_{b(j)}: H_{b(j)}\rightarrow G_{a(\varphi_0(j))}$

and

$\psi_j=$ Int($c_2(j)$)$^{-1}\circ \psi_{b(j)}: H_{b(j)}\rightarrow G_{a(\psi_0(j))}$,

so that one has, for every element $f$ of $H_{b(j)}$,

(6) $\varphi_j(f) =c_1(j)^{-1}\varphi (f)c_1(j)$ and $\psi_j(f) =c_2(j)^{-1}\psi (f)c_2(j)$.

For each vertex $i$ of $\Gamma_0$, let us again denote by $d_i$ the unique path class joining $i_0$ to $i$ in the tree $\widetilde{T}$; it is regarded as an arrow of Grp(Γ$_0$). Let us then denote by $\delta_i$ the arrow of Coh($\varphi , \psi$ ) which is the image of $d_i$ under the canonical morphism of Grp(Γ$_0$) into Coh($\varphi , \psi$ ) deduced from $\tau_0$; the origin of $\delta_i$ is $a(i_0)$, its end is $a(i)$.

The quiver morphism $\tau_0$, the group homomorphisms $\alpha_i$ (for $i\in$ Orb(G))$,\varphi_j$ and $\psi_j$ (for $j\in$ Orb(H)), and the arrows $\delta_i$ in Coh($\varphi , \psi$ ) (for $i\in$ Orb(G)) will be said to be deduced from the basic equipment.

If $(G_i)_{i\in I}$ is a family of groups, we denote by $_i*_{\in I}G_i$ their free product; the image of an element $g\in G_i$ under the canonical mapping of $G_i$ into $_i*_{\in I}G_i$ will be denoted by $[g]$, or even by $g$ if there is no possible confusion. If S is a set, we denote by F(S) the free group constructed on S (A, I, p. 84).

#### Proposition 6 {#ta-ii-s4-prop-6 .statement tag=01UH}

There exists a unique group homomorphism

$\Lambda :(*G_{a(i)})*$ F(Orb(H)) $\rightarrow$ Coh($\varphi , \psi$ )$_{a(i_0)}$

$i\in$Orb(G)

such that

(7) $\Lambda (f) =\delta_i\alpha_i(f)\delta_i^{-1}$ for $i\in$ Orb(G) and $f\in G_{a(i)}$,

(8) $\Lambda (j) =\delta_{\varphi_0(j)}\tau_0(j)\delta^{-1}_{\psi_0(j)}$ for $j\in$ Orb(H).

The homomorphism Λ is surjective; its kernel is the smallest normal subgroup of $(*_iG_{a(i)})*$ F(Orb(H)) containing the elements $j$ of Fl(T) and the elements $\varphi_j(f)j\psi_j(f)^{-1}j^{-1}$, for $j\in$ Orb(H) and $f\in H_{b(j)}$.

The existence and uniqueness of the homomorphism Λ result from the universal property of free products and free groups (A, I, p. 85, prop. 8).

Let A denote the set of the $a(i)$ for $i\in$ Orb(G) and $G_A$ the full subgroupoid of G whose set of vertices is A. For every $x\in$ Som(G), let $\overline{x}$ denote the orbit of $x$ in G and choose an arrow $d_x$ of G joining $x$ to $a(\overline{x})$. The pair $v$ formed by the mapping $x\mapsto a(\overline{x})$ of Som(G) into A and the mapping which to $f\in$ Fl$_{x,y}(G)$ associates the element $d^{-1}_xf d_y$ of Fl$_{a(\overline{x}),a(\overline{y})}(G_A)$ is a groupoid morphism. It follows from Proposition 1 of II, p. 182 that $v$ is a homotopism. Let $\varphi '=v\circ \varphi$ and $\psi '=v\circ \psi$, and then let $w$ be the canonical morphism of Coh($\varphi , \psi$ ) into Coh($\varphi ', \psi '$) ; it is a homotopism (II, p. 187, Theorem 1).

The orbits of $G_A$ are the sets $\{a\}$, for $a\in A$, and the injection $G_A\rightarrow G$ induces a bijection of Orb(G$_A$) onto Orb(G), by means of which we shall identify these two sets. One defines a basic equipment $(a', b', \beta '_1, \beta '_2,T', i_0)$ of the pair $(\varphi ', \psi ')$ by setting $a'(i) =a(i)$ for $i\in$ Orb(G)$,b'(j) =b(j),\beta '_1(j) =v(c_1(j)),\beta '_2(j) =v(c_2(j))$ for $j\in$ Orb(H) and $T'= T$. The group homomorphisms $\varphi '_j$ and $\psi '_j$ (for $j\in$ Orb(H)), the quiver morphism $\tau '_0$, the arrows $\delta '_i$ (for $i\in$ Orb(G)), and therefore the group homomorphism $\Lambda '$, deduced from this basic equipment, are the composites with $w$ of the corresponding homomorphisms $\varphi_j,\psi_j$, of the quiver morphism $\tau_0$, of the corresponding arrows $\delta_i$ and of the homomorphism Λ.

Let B be the set of the $b(j)$ for $j\in$ Orb(H), let $H_B$ be the full subgroupoid of H with set of vertices B; let us denote by $u: H_B\rightarrow H$ the canonical injection; put $\varphi ''=\varphi '\circ u$ and $\psi ''=\psi '\circ u$. The morphism $u$ induces a bijection B $\rightarrow$ Orb(H) by which we shall identify these two sets. From theorem 1 of II, p. 187 one further deduces a canonical homotopism $w':$ Coh($\varphi '', \psi ''$)$\rightarrow$ Coh($\varphi ', \psi '$). Moreover, the pair $(\varphi '', \psi '')$ is endowed with a base equipment $(a'', b'', \beta ''_1, \beta ''_2,T'', i_0)$, so that $\Lambda ', \varphi '_j, \psi '_j, \tau '_0, \delta '_i(i, i'\in$ Orb(G), $j\in$ Orb(H)) are the composites with $w'$ of $\Lambda '', \varphi ''_j, \psi ''_j, \tau ''_0, \delta ''_i$.

The various morphisms of groupoids introduced are summarized by the following diagram:

$H_{B\psi''}^{\varphi''}G_A^{\alpha''}$ Coh($\varphi '', \psi ''$)

$w'$

(9) H $^{\varphi'}G_A^{\alpha'}$ Coh($\varphi '', \psi ''$)

$\psi '$

$$
vw
$$

H $^{\varphi}_{\psi}$ G $^{\alpha}$ Coh($\varphi , \psi$ ) .

To prove the proposition, we may therefore suppose that A = Som(G) and B = Som(H), in other words that the canonical mappings Som(G) $\rightarrow$ Orb(G) and Som(H) $\rightarrow$ Orb(H) are bijective, hypotheses under which we shall place ourselves in the rest of the proof.

The quiver $G_1$ then has for set of vertices A and for arrows the sum set of the sets $G_a,a\in A$, and of the set B. The arrows of $G_a$ are loops at $a$; if $b\in B$, the arrow $b$ joins $\varphi (b)$ to $\psi (b)$, the arrows $c_1(b)$ and $c_2(b)$ are loops respectively at $\varphi (b)$ and $\psi (b)$. The quiver T will be identified with an oriented tree of $G_1$; it is a maximal oriented tree since the set of its vertices is equal to the set of vertices of $G_1($II, p. 157, prop. 1). We put $a_0=a(i_0)$. The set of arrows of the framework $\Gamma_0$ of the pair $(\varphi , \psi )$ being identified with B, the morphism of quivers $\tau_1: \Gamma_0\rightarrow$ Grp(G$_1$) associates to the arrow $b$ the class of paths $c_1(b)^{-1}bc_2(b)$ in the graph $\widetilde{G}_1$.

Recall that $\theta_1$ denotes the canonical morphism of quivers of $G_1$ into Grp(G$_1$). Let

$\lambda :_a*_{\in A}F(G_a)*F(B)\rightarrow$ Grp(G$_1$)$_{a_0}$

be the unique group homomorphism such that one has

$\lambda (f) =\tau_1(d_a)\theta_1(f)\tau_1(d_a)^{-1}$ if $a\in A$ and $f\in G_a$;

$\lambda (b) =\tau_1(d_{\varphi(b)})\tau_1(b)\tau_1(d_{\psi(b)})^{-1}$ if $b\in B$.

We thus have $\lambda =\lambda '\circ \varepsilon$, where $\lambda '$ denotes the canonical group homomorphism from $_a*_{\in A}F(G_a)*F(B)$ into Grp(G$_1$)$_{a_0}$ defined by the maximal oriented tree T (II, p. 179, prop. 9), and where $\varepsilon$ is the unique automorphism of the group $_a*_{\in A}F(G_a)*F(B)$ such that $\varepsilon (f) =f$ for $a\in A$ and $f\in G_a$, and $\varepsilon (b) =c_1(b)^{-1}h_1(b)c_2(b)$ for $b\in B$. According to remark 2 of II, p. 179, the homomorphism $\lambda$ is surjective and its kernel is the smallest normal subgroup of $_a*_{\in A}F(G_a)*F(B)$ containing the arrows of T.

Let us denote by $\pi :$ Grp(G$_1$)$\rightarrow$ Coh($\varphi , \psi$ ) the canonical groupoid morphism. According to II, p. 177, cor. 1 of prop. 8, the group homomorphism $\pi_{a_0}$ from Grp(G$_1$)$_{a_0}$ into Coh($\varphi , \psi$ )$_{a_0}$ is surjective, and its kernel is the smallest normal subgroup of Grp(G$_1$)$_{a_0}$ containing the loops Int($\tau_1(d_a)$)$(\alpha_1(f)\alpha_1(g)\alpha_1(f g)^{-1})$, for $a\in A$ and $f,g\in G_a$, and the loops Int($\tau_1(d_{\varphi(b)})$)$(\varphi (f)b\psi (f)^{-1}b^{-1})$, for $b\in B$ and $f\in H_b$.

If $p: F(\bigcup G_a\cup B)\rightarrow (_a*_{\in A}G_a)*F(B)$ denotes the canonical surjective homomorphism, we thus have $\Lambda \circ p=\pi_{a_0}\circ \lambda$. This formula implies that the homomorphism Λ is surjective; it remains to determine its kernel.

For $a\in A$ and $f\in G_a$, let us denote by $[f]$ the image of $f\in F(G_a)$ in the group $_a*_{\in A}F(G_a)*F(B)$. For $a\in A,f, g\in G_a$, we then have

Int($\tau_1(d_a)$)$(\alpha_1(f)\alpha_1(g)\alpha_1(f g)^{-1}) =\lambda ([f][g][f g]^{-1})$.

Analogously, for $b\in B$ and $f\in H_b$, the definition of the homomorphisms $\varphi_b$ and $\psi_b$ (formula (6) of II, p. 193) implies that one has

Int($\tau_1(d_{\varphi(b)})$)$(\varphi (f)h_1(b)\psi (f)^{-1}h_1(b)^{-1})$

$$
=\tau_1(d_{\varphi(b)})\varphi (f)(c_1(b)\tau_1(b)c_2(b)^{-1})\psi (f)^{-1}
$$

$$
(c_2(b)\tau_1(b)^{-1}c_1(b)^{-1})\tau_1(d_{\varphi(b)})^{-1}
$$

$$
=\tau_1(d_{\varphi(b)})c_1(b)\varphi_b(f)\tau_1(b)\psi_b(f)^{-1}\tau_1(b)^{-1}c_1(b)^{-1}\tau_1(d_{\varphi(b)})^{-1}
$$

$$
=\lambda (c_1(b))\lambda (\varphi_b(f)[b]\psi_b(f)^{-1}[b]^{-1})\lambda (c_1(b))^{-1}
$$

Consequently, the kernel of the homomorphism $\pi_{a_0}\circ \lambda$ is the smallest normal subgroup of $_a*_{\in A}F(G_a)*F(B)$ which contains the elements $[f][g][f g]^{-1}$ for $a\in A$ and $f,g\in G_a$, the elements $\varphi_b(f)[b]\psi_b(f)^{-1}[b]^{-1}$ for $b\in B$ and $f\in H_b$, and the elements $[b]$, for $b\in$ Fl(T).

Finally, the kernel of the homomorphism Λ is the smallest normal subgroup of $(_a*_{\in A}G_a)*F(B)$ which contains the images under $p$ of the preceding elements, in other words, the elements $[b]$, for $b\in$ Fl(T), and the elements $\varphi_b(f)[b]\psi_b(f)[b]^{-1}$, for $b\in B$ and $f\in H_b$. The proposition is thus proved.
