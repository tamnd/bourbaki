---
book: ts
book_title: Théories spectrales
chapter: V
chapter_title: REPRÉSENTATIONS UNITAIRES
section: 1
section_title: Représentations unitaires
lang: fr
source: ts-iii-v-fr
book_pages: A V.373-A V.398, A V.483-A V.486
pdf_pages: 0386-0411, 0496-0499
extraction: native
subsections:
    - "no": 1
      title: Rappels concernant les représentations linéaires continues
      page: 374
      pdf_page: 387
    - "no": 2
      title: Un critère de continuité
      page: 377
      pdf_page: 390
    - "no": 3
      title: Représentations continues de dimension finie
      page: 378
      pdf_page: 391
    - "no": 4
      title: Représentations irréductibles
      page: 378
      pdf_page: 391
    - "no": 5
      title: Représentations unitaires
      page: 379
      pdf_page: 392
    - "no": 6
      title: Somme directe hilbertienne et produit tensoriel de repré- sentations unitaires
      page: 383
      pdf_page: 396
    - "no": 7
      title: Coefficients matriciels
      page: 385
      pdf_page: 398
    - "no": 8
      title: Le lemme de Schur
      page: 386
      pdf_page: 399
    - "no": 9
      title: Semi-simplicité
      page: 390
      pdf_page: 403
    - "no": 10
      title: Classes de représentations unitaires
      page: 392
      pdf_page: 405
    - "no": 11
      title: Composantes isotypiques
      page: 394
      pdf_page: 407
statements: 50
exercises: 7
content_sha256: 5053a4dc4e4e329edeb4e91a8697d86524dabbe10969a25702b4d92ba3c10685
---

## § 1. REPRÉSENTATIONS UNITAIRES

Dans ce paragraphe, les espaces vectoriels sont sur $K =\mathbf{R}$ ou $\mathbf{C}$.

Rappelons qu’une représentation linéaire d’un groupe G dans un K-espace vectoriel E est un homomorphisme $\varrho$ de G dans le groupe $\mathbf{G}\mathbf{L}(E)$ des automorphismes de E (A, VIII, p. 387, déf. 1). On dit que E est l’espace de la représentation $\varrho$, et que la dimension de E est la dimension de $\varrho$, que l’on note aussi dim($\varrho$ ).

On peut identifier une représentation de G dans un K-espace vectoriel à un K[G]-module (loc. cit.), et on utilisera la terminologie correspondante, par exemple concernant les sommes directes de représentations, les morphismes de représentations ou la représentation sur $\mathbf{C}$ obtenue à partir d’une représentation dans un $\mathbf{R}$-espace vectoriel par extension des scalaires.

Une représentation $\varrho : G\rightarrow \mathbf{G}\mathbf{L}(E)$ est dite fidèle si c’est un homomorphisme injectif.

On prendra garde que cela ne signifie pas que le K[G]-module associé à $\varrho$ est un K-module fidèle (A, II, p. 28).

Le caractère d’une représentation de G dans un K-espace vectoriel de dimension finie est l’application $\chi_{\varrho}$ de G dans K telle que $\chi_{\varrho}(g) =$ Tr($\varrho (g)$) pour tout $g\in G$, cf. A, VIII, p. 388.

### 1. Rappels concernant les représentations linéaires continues

Soit G un groupe topologique. On rappelle qu’une représentation linéaire continue de G dans un K-espace vectoriel topologique E est une représentation linéaire $\varrho$ de G dans E telle que l’application de $G\times E$ dans E définie par $(g, x)\mapsto \varrho (g)x$ est continue (INT, VIII, p. 128, § 2, n$^o1$, déf. 1). Cette application définit une action de G sur E et l’image de $\varrho$ est contenue dans $\mathscr{L}(E)$. On dit qu’une représentation continue $\varrho$ est bornée si son image est bornée dans l’espace $\mathscr{L}(E)$ muni de la topologie de la convergence bornée.

#### Remarque {#ts-v-s1-n1-rem-1 .statement tag=038J}

Si $K =\mathbf{R}$ et si $\varrho$ est une représentation linéaire continue de G dans un $\mathbf{R}$-espace vectoriel E, alors l’application $\varrho_{(\mathbf{C})}:g\mapsto 1\otimes \varrho (g)$ est une représentation linéaire continue de G dans $E_{(\mathbf{C})}$; si $\varrho$ est bornée, alors $\varrho_{(\mathbf{C})}$ est bornée.

Pour tout K-espace vectoriel topologique E, l’homomorphisme qui à tout $g\in G$ associe $1_E$ est une représentation linéaire continue de G dans E, appelée représentation triviale de G dans E.

Soit H un sous-groupe de G. La restriction de $\varrho$ à H est une représentation linéaire continue de H dans E, notée Res$^G_H(\varrho )$.

Soient $\varrho_1$ et $\varrho_2$ des représentations linéaires continues de G dans des K-espaces vectoriels topologiques $E_1$ et $E_2$. Un G-morphisme $u$ de $\varrho_1$ dans $\varrho_2$ est un morphisme de représentations linéaires qui est continu, c’est-à-dire une application linéaire continue $u: E_1\rightarrow E_2$ telle que $u\circ \varrho_1(g) =\varrho_2(g)\circ u$ pour tout $g\in G$. On note Hom$_G(\varrho_1, \varrho_2)$ l’espace vectoriel des G-morphismes de $\varrho_1$ dans $\varrho_2$. C’est un sous-espace fermé de l’espace $\mathscr{L}(E_1; E_2)$ muni de la topologie de la convergence simple.

Soit $\varrho$ une représentation linéaire continue d’un groupe G dans un K-espace vectoriel topologique E. L’application identique $1_E$ de E est un G-morphisme de $\varrho$ dans $\varrho$, qui est noté $1_{\varrho}$. Si $\varrho_1,\varrho_2$ et $\varrho_3$ sont des représentations linéaires continues de G dans des K-espaces vectoriels topologiques $E_1, E_2, E_3$ respectivement, et si $u: E_1\rightarrow E_2$ et $v: E_2\rightarrow E_3$ sont des G-morphismes, alors $v\circ u$ est un G-morphisme.

Un G-morphisme $u$ de $\varrho_1$ dans $\varrho_2$ est un G-isomorphisme s’il existe un G-morphisme $v$ de $\varrho_2$ dans $\varrho_1$ tel que $v\circ u= 1_{\varrho_1}$ et $u\circ v= 1_{\varrho_2}$. Il faut et il suffit pour cela que $u$ soit un G-morphisme et un isomorphisme d’espaces vectoriels topologiques de l’espace de $\varrho_1$ dans l’espace de $\varrho_2$; son inverse $v=u^{-1}$ est en effet alors un G-morphisme. S’il existe un G-isomorphisme de $\varrho_1$ dans $\varrho_2$, on dit que ces représentations sont isomorphes.

#### Définition 1 {#ts-v-s1-def-1 .statement tag=038K}

Soit $\varrho$ une représentation linéaire continue d’un groupe topologique G dans un espace vectoriel topologique E. Une représentation linéaire continue $\pi$ de G dans F est une sous-représentation de $\varrho$ si F est un sous-espace fermé de E et si, pour tout $g\in G$, l’espace F est stable par $\varrho (g)$ et $\pi (g)$ est l’endomorphisme de F déduit de $\varrho (g)$ par passage aux sous-espaces.

Soit $\varrho$ une représentation linéaire continue d’un groupe topologique G dans un espace vectoriel topologique E. L’adhérence de $\{0\}$ dans E est une sous-représentation de $\varrho$. Plus généralement, l’adhérence d’un sous-espace stable par les endomorphismes $\varrho (g)$ est une sous-représentation de $\varrho$.

Une sous-représentation $\pi$ de $\varrho$ est déterminée de manière unique par un sous-espace fermé F, stable par tous les endomorphismes $\varrho (g)$. Cette dernière condition sera souvent énoncée sous la forme « F est un sous-espace G-invariant de E ». On dira alors aussi que F définit une sous-représentation de $\varrho$, ou parfois, par abus de langage, que F est une sous-représentation de $\varrho$, ou de E.

Soit F un sous-espace de E définissant une sous-représentation $\pi$ de $\varrho$. Pour tout $g\in G$, l’application linéaire $\varrho (g)$ définit, par passage au quotient, un endomorphisme $\widetilde{\varrho}(g)$ de $E/F$. L’application $g\mapsto \widetilde{\varrho}(g)$ est une représentation linéaire continue de G dans $E/F$ et la projection canonique de E dans $E/F$ est un G-morphisme. On dit que $\widetilde{\varrho}$ est la représentation quotient de G sur $E/F$; on la note aussi $\varrho /\pi$.

Le sous-espace des éléments de E invariants par l’action de G est une sous-représentation triviale de $\varrho$. On la note $\varrho^G$ ou bien $E^G$.

Soit A un sous-ensemble de E. Le sous-espace fermé F engendré par les éléments $\varrho (g)x$, où $g\in G$ et $x\in A$, est une sous-représentation de $\varrho$, dite sous-représentation de $\varrho$ engendrée par A ; si F = E, on dit que A engendre $\varrho$. Si la sous-représentation F est de dimension finie, on dit que le sous-ensemble A est G-fini.

Supposons que A est réduit à un seul élément $x\in E$. Si A engendre $\varrho$, on dit que $x$ est un vecteur cyclique de $\varrho$ et que $\varrho$ est une représentation cyclique ; on dit que $x$ est un vecteur G-fini si A est G-fini.

L’ensemble des vecteurs G-finis de $\varrho$ est un sous-espace vectoriel de E stable par $\varrho$; il n’est pas nécessairement fermé.

Soit $(\varrho_i)_{i\in I}$ une famille de représentations linéaires continues de G dans des K-espaces vectoriels topologiques localement convexes $(E_i)_{i\in I}$. Soit E l’espace somme directe des espaces $E_i$. L’application $g\mapsto (\varrho_i(g))$ est une représentation linéaire de G dans E, dite somme, ou somme directe, des représentations $\varrho_i$. Si I est fini, elle est continue.

Si les représentations $\varrho_i$ sont égales à une représentation $\varrho$ pour tout $i\in I$, on dit que la somme directe des représentations $\varrho_i$ est la somme de Card(I) copies de la représentation $\varrho$, et on la note aussi $\varrho^{Card(I)}$, ou bien Card(I) $\varrho$.

Soient $(\varrho_i)_{i\in I}$ et $(\pi_j)_{j\in J}$ des familles finies de représentations linéaires continues de G dans des K-espaces vectoriels topologiques $(E_i)_{i\in I}$ et $(F_j)_{j\in J}$, respectivement. L’isomorphisme canonique de K-espaces vectoriels

Hom$_K\bigoplus_{i\in I}E_i,\bigoplus_{j\in J}F_j\rightarrow \bigoplus_{(i,j)\in I\times J}$ Hom$_K(E_i,F_j)$ (A, II, p. 13, cor. 1) induit, par passage aux sous-espaces, un isomorphisme

(1) Hom$_G\bigoplus_{i\in I}\varrho_i,\bigoplus_{j\in J}\pi_j\rightarrow \bigoplus_{(i,j)\in I\times J}$ Hom$_G(\varrho_i, \pi_j)$

qui est également dit canonique.

Soient $\varrho_1$ et $\varrho_2$ des représentations linéaires de G dans des K-espaces vectoriels topologiques $E_1$ et $E_2$. Pour $u\in \mathscr{L}(E_1; E_2)$ et $g\in G$, on pose $\varrho (g)u=\varrho_2(g)\circ u\circ \varrho_1(g^{-1})$. L’application $g\mapsto \varrho (g)$ est une représentation linéaire de G dans $\mathscr{L}(E_1; E_2)$. L’espace des éléments invariants de cette représentation coïncide avec Hom$_G(\varrho_1, \varrho_2)$.

Soit $\varrho$ une représentation linéaire continue de G dans un espace localement convexe E. Rappelons (INT, VIII, p. 131, § 2, n$^o2)$ que la représentation contragrédiente $\breve{\varrho}$ de $\varrho$ est la représentation linéaire de G dans le dual $E'$ de E définie par $\breve{\varrho}(g) =^t\varrho (g^{-1})$.

### 2. Un critère de continuité

Le résultat suivant permet de vérifier que certaines représentations linéaires d’un produit direct de groupes topologiques sont continues.

#### Lemme 1 {#ts-v-s1-lem-1 .statement tag=038L}

Soient G et H des groupes topologiques et E un espace de Banach. Soient $\varrho$ une représentation bornée de G dans E et $\pi$ une représentation bornée de H dans E. Supposons que $\varrho (g)$ est permutable à $\pi (h)$ pour tout $(g, h)\in G\times H$. L’application $\varpi$ de $G\times H$ dans $\mathbf{G}\mathbf{L}(E)$ définie par $(g, h)\mapsto \varrho (g)\circ \pi (h)$ est une représentation linéaire continue et bornée de $G\times H$ dans E.

L’application $\varpi$ est une représentation linéaire de $G\times H$ dans E ; vérifions qu’elle est continue. Comme $\|\varpi (g, h)\|\leqslant \|\varrho (g)\|\|\pi (h)\|$ pour tout $(g, h)\in G\times H$, la représentation $\varpi$ est bornée, donc son image est équicontinue dans $\mathscr{L}(E)$. Il suffit alors de démontrer que, pour tout $x\in E$, l’application $(g, h)\mapsto \varpi (g, h)x$ est continue (remarque 2 de INT, VIII, p. 129, § 2, n$^o1)$. Soit $(g_0, h_0)\in G\times H$. Posons $y=\pi (h_0)x$. Pour tout $(g, h)\in G\times H$, il vient

$$
\|\varpi (g, h)x-\varpi (g_0, h_0)x\|\leqslant \|\varrho (g)(\pi (h)x-y)\|+\|\varrho (g)y-\varrho (g_0)y\|
$$

$$
\leqslant \|\varrho (g)\| \|\pi (h)x-y\|+\|\varrho (g)y-\varrho (g_0)y\|
$$

Puisque $\varrho$ est bornée et que $\varrho$ et $\pi$ sont continues, cela implique l’assertion.

### 3. Représentations continues de dimension finie

Soit $\varrho$ une représentation linéaire continue d’un groupe topologique G dans un K-espace vectoriel topologique séparé E de dimension finie. On munit $\mathscr{L}(E)$ de son unique structure d’espace vectoriel topologique séparé sur K ; le morphisme $\varrho : G\rightarrow \mathbf{G}\mathbf{L}(E)$ est alors continu puisque la topologie de $\mathbf{G}\mathbf{L}(E)$ est induite par la topologie de $\mathscr{L}$ (E), qui coïncide avec la topologie de la convergence simple (EVT, I, p. 14, th. 2). Par conséquent, le caractère de $\varrho$ est continu. Si G est un groupe de Lie réel, alors le caractère de $\varrho$ est une fonction analytique sur G (LIE, III, p. 225, § 8, n$^o1$, th. 1). La représentation contragrédiente est également continue lorsque $E'$ est muni de son unique topologie d’espace vectoriel topologique séparé sur K. De plus, pour tout entier $n\geqslant 0$, les représentations $\mathsf{T}^n(\varrho ),\mathsf{S}^n(\varrho )$ et $\wedge^n(\varrho ) ($loc. cit.) sont continues, lorsque les espaces correspondants sont munis de leurs topologies d’espaces vectoriels topologiques séparés sur K.

Soient $\varrho_1$ et $\varrho_2$ des représentations continues d’un groupe topologique G dans des espaces vectoriels topologiques séparés $E_1$ et $E_2$ de dimension finie. La représentation linéaire $\varrho_1\otimes \varrho_2$ de G dans $E_1\otimes E_2$ (LIE, III, p. 256, Appendice) est continue, l’espace $E_1\otimes E_2$ étant muni de sa topologie d’espace vectoriel topologique séparé sur K.

### 4. Représentations irréductibles

Dans ce numéro, G est un groupe topologique.

#### Définition 2 {#ts-v-s1-def-2 .statement tag=038M}

Une représentation $\varrho$ de G dans un K-espace vectoriel topologique E est dite irréductible si $\{0\}$ n’est pas dense dans E et si les seules sous-représentations de $\varrho$ sont $\varrho$ et la représentation dans l’adhérence de $\{0\}$.

Si $\varrho$ est une représentation irréductible de G dans un espace vectoriel topologique séparé E, alors tout élément non nul de E est un vecteur cyclique pour $\varrho$.

#### Lemme 2 {#ts-v-s1-lem-2 .statement tag=038N}

Soient $\pi$ et $\varrho$ des représentations linéaires continues de G dans des K-espaces vectoriels topologiques séparés. On suppose que $\pi$ est irréductible. Tout G-morphisme non nul de $\pi$ dans $\varrho$ est injectif et tout G-morphisme non nul de $\varrho$ dans $\pi$ est d’image dense.

En particulier, si $\pi$ et $\varrho$ sont irréductibles et de dimension finie, alors tout G-morphisme non nul de $\pi$ dans $\varrho$ est un isomorphisme.

Puisque l’espace de $\varrho$ est séparé, le noyau d’un G-morphisme $u$ de $\pi$ dans $\varrho$ est fermé, et induit une sous-représentation de $\pi$. Si le morphisme $u$ n’est pas nul, son noyau doit donc être réduit à 0, puisque $\pi$ est une représentation irréductible dans un espace vectoriel topologique séparé. Similairement, l’adhérence de l’image d’un G-morphisme non nul de $\varrho$ dans $\pi$ est une sous-représentation non nulle de $\pi$, donc est égale à l’espace de $\pi$.

La dernière assertion découle de ce qui précède.

#### Lemme 3 {#ts-v-s1-lem-3 .statement tag=038O}

Soit $\varrho$ une représentation linéaire continue de G dans un K-espace vectoriel topologique séparé E de dimension finie. Si E est non nul, alors il existe une sous-représentation irréductible de $\varrho$.

Puisque E est de dimension finie et non nul, il existe un sous-espace G-invariant F de E qui est non nul et de dimension minimale. Ce sous-espace est fermé dans E et définit une sous-représentation de E ; toute sous-représentation de F est aussi une sous-représentation de E, et la représentation F est donc irréductible par minimalité.

#### Remarque {#ts-v-s1-n4-rem-1 .statement tag=038P}

Une représentation non nulle E de G ne contient pas toujours de sous-représentation irréductible (cf. V, p. 426, remarque). On verra cependant que c’est le cas si G est compact et si $K =\mathbf{C}$ et si E est un espace localement convexe séparé quasi-complet et non nul sur K (prop. 7 de V, p. 464).

### 5. Représentations unitaires

#### Définition 3 {#ts-v-s1-def-3 .statement tag=038Q}

Soient G un groupe topologique et E un espace hilbertien sur K. Une représentation unitaire de G dans E est une représentation linéaire continue $\varrho$ de G dans E telle que, pour tout $g$ dans G, l’endomorphisme $\varrho (g)$ de E soit un endomorphisme unitaire (EVT, V, p. 40) de E.

Autrement dit, une représentation unitaire est une représentation isométrique dans un espace hilbertien. En particulier, une représentation unitaire est bornée.

La représentation triviale d’un groupe topologique dans un espace hilbertien est unitaire. Toute sous-représentation d’une représentation unitaire est unitaire. La restriction à un sous-groupe d’une représentation unitaire est unitaire.

#### Définition 4 {#ts-v-s1-def-4 .statement tag=038R}

Soit G un groupe topologique et soient $\varrho$ et $\pi$ des représentations unitaires de G dans des espaces hilbertiens E et F respectivement. Une forme sesquilinéaire G-invariante sur $E\times F$ est une forme sesquilinéaire continue $q$ sur $E\times F$ telle que

$$
q(x, y) =q(\varrho (g)x, \pi (g)y)
$$

pour tout $g\in G$ et tout $(x, y)\in E\times F$.

L’espace vectoriel des formes sesquilinéaires G-invariantes sur $E\times F$ est noté Sesq$_G(\varrho , \pi )$ ou Sesq$_G(E,F)$.

#### Exemple {#ts-v-s1-n5-exa-1 .statement tag=038S}

Soit G un groupe topologique et soit $\varrho$ une représentation unitaire de G dans E. Le produit scalaire $q$ sur E est une forme sesquilinéaire G-invariante sur $E\times E$.

#### Lemme 4 {#ts-v-s1-lem-4 .statement tag=038T}

Soit G un groupe topologique et soit $\varrho$ un homomorphisme de G dans le groupe unitaire $\mathbf{U}(E)$ d’un espace hilbertien E. Alors $\varrho$ est une représentation unitaire de G si et seulement si $\varrho$ est continue en l’élément $e$ de G pour la topologie de la convergence simple sur $\mathbf{U}(E)$. Il suffit que cette propriété soit valide pour tout $x$ dans un sous-ensemble total de E.

La condition est évidemment nécessaire. Elle est suffisante d’après la remarque 2 de INT, VIII, p. 129, § 2, n$^o1$, puisque l’image de $\varrho$ est équicontinue dans $\mathscr{L}(E)$ et puisque la continuité de l’application $g\mapsto \varrho (g)x$ en $e$ implique sa continuité sur G.

Soit G un groupe topologique. Si $\varrho_1$ et $\varrho_2$ sont des représentations unitaires de G et si $u$ appartient à Hom$_G(\varrho_1, \varrho_2)$, alors $u^*$ appartient à Hom$_G(\varrho_2, \varrho_1)$. En effet, puisque $\varrho_1$ et $\varrho_2$ sont des représentations unitaires, on a pour tout $g\in G$

$$
u^*\circ \varrho_2(g) =u^*\circ \varrho_2(g^{-1})^*= (\varrho_2(g^{-1})\circ u)^*
$$

$$
= (u\circ \varrho_1(g^{-1}))^*=\varrho_1(g)\circ u^*
$$

#### Lemme 5 {#ts-v-s1-lem-5 .statement tag=038U}

Soit G un groupe topologique et soit $\varrho$ une représentation unitaire de G dans un espace hilbertien complexe E. L’espace Hom$_G(\varrho , \varrho )$ est une sous-algèbre stellaire unifère de $\mathscr{L}(E)$.

Ce qui précède montre que Hom$_G(\varrho , \varrho )$ est une sous-algèbre unifère et auto-adjointe de $\mathscr{L}(E)$. Puisqu’elle est fermée dans $\mathscr{L}$ (E), c’est une sous-algèbre stellaire de $\mathscr{L}(E)$.

#### Lemme 6 {#ts-v-s1-lem-6 .statement tag=038V}

Soient $\pi$ et $\varrho$ des représentations unitaires d’un groupe topologique G dans des espaces hilbertiens E et F respectivement. Soit D un sous-espace dense de E qui est stable par $\pi$. Soit $u$ un opérateur partiel fermé de E dans F de domaine D tel que $u\circ \pi (g) =\varrho (g)\circ u$ pour tout $g\in G$. Alors le domaine de $u^*$ est stable par $\varrho$ et on a la relation $u^*\circ \varrho (g) =\pi (g)\circ u^*$ pour tout $g\in G$.

Soient $g\in G$ et $x\in$ dom($u^*$). Pour tout $y\in$ dom($u$), on a

$$
\langle \varrho (g)x|u(y)\rangle =\langle x|\varrho (g^{-1})u(y)\rangle =\langle x|u(\pi (g^{-1})y)\rangle
$$

$$
=\langle u^*(x)|\pi (g^{-1})y\rangle =\langle \pi (g)(u^*(x))|y\rangle
$$

puisque $\varrho (g)^*=\varrho (g)^{-1}=\varrho (g^{-1})$. Cela démontre que $\varrho (g)x\in$ dom($u^*$) et que $u^*(\varrho (g)x) =\pi (g)(u^*(x))$. En particulier, le domaine de $u^*\circ \varrho (g)$ contient le domaine de $u^*$, et $\pi (g)\circ u^*\subset u^*\circ \varrho (g)$.

Mais de plus, si $x\in$ dom($u^*\circ \varrho (g)$), alors $x=\varrho (g^{-1})(\varrho (g)x)$ appartient à dom($u^*$) d’après ce qui précède appliqué à $g^{-1}$. On conclut que $u^*\circ \varrho (g) =\pi (g)\circ u^*$.

#### Proposition 1 {#ts-v-s1-prop-1 .statement tag=038W}

Soient $\varrho_1$ et $\varrho_2$ des représentations unitaires d’un groupe topologique G dans des espaces hilbertiens $E_1$ et $E_2$. L’application de Hom$_G(\varrho_1, \varrho_2)$ dans Sesq$_G(\varrho_2, \varrho_1)$ qui à $u$ associe la forme sesquilinéaire $q_u$ définie par $q_u(x, y) =\langle x|u(y)\rangle$ est un isomorphisme d’espaces vectoriels.

Si $u$ est un G-morphisme, alors on a

$$
q_u(\varrho_2(g)x, \varrho_1(g)y) =\langle \varrho_2(g)x|u(\varrho_1(g))y\rangle
$$

$$
=\langle \varrho_2(g)x|\varrho_2(g)u(y)\rangle =\langle x|u(y)\rangle =q_u(x, y)
$$

pour tout $g\in G$ et tout $(x, y)\in E_2\times E_1$, donc l’application indiquée est une application linéaire de Hom$_G(\varrho_1, \varrho_2)$ dans Sesq$_G(\varrho_2, \varrho_1)$. D’après EVT, V, p. 16, cor. 2, elle est injective.

Réciproquement, soient $q$ une forme sesquilinéaire G-invariante et $u$ l’unique application linéaire de $E_1$ dans $E_2$ telle que $q(x, y) =\langle x|u(y)\rangle$ pour tout $(x, y)\in E_2\times E_1($loc. cit.). Pour tout $g$ dans G et tout $(x, y)$ dans $E_2\times E_1$, on a

$$
\langle x|(\varrho_2(g)\circ u\circ \varrho_1(g^{-1}))(y)\rangle =\langle \varrho_2(g^{-1})x|u(\varrho_1(g^{-1})y)\rangle
$$

$$
=q(\varrho_2(g^{-1})x, \varrho_1(g^{-1})y) =q(x, y) =\langle x|u(y)\rangle
$$

donc $u=\varrho_2(g)\circ u\circ \varrho_1(g^{-1})$. Par conséquent, $u\in$ Hom$_G(\varrho_2, \varrho_1)$. La proposition en résulte.

Soit $\varrho$ une représentation unitaire d’un groupe topologique G dans un espace hilbertien E. Si $K =\mathbf{C}$, notons E l’espace conjugué de E (EVT, V, p. 6). Si $K =\mathbf{R}$, posons E = E. La représentation conjuguée $\overline{\varrho}$ est la représentation de G dans E définie par $\overline{\varrho}(g) =\varrho (g)$ pour tout $g\in G$. C’est une représentation unitaire de G ; par définition, un sous-espace de E est une sous-représentation de E si et seulement si c’est une sous-représentation de E.

#### Proposition 2 {#ts-v-s1-prop-2 .statement tag=038X}

Soit $\varrho$ une représentation unitaire d’un groupe topologique G dans un espace hilbertien E. Notons $u$ l’isomorphisme isométrique de $\overline{E}$ dans $E'$ qui à $x$ associe la forme linéaire $y\mapsto  \langle x|y\rangle$.

a) L’application $u$ est un isomorphisme de la représentation conjuguée $\overline{\varrho}$ dans la représentation contragrédiente $\breve{\varrho}$;

b) Munissons $E'$ de la structure d’espace hilbertien obtenue par transport de structure à l’aide de $u$; la représentation contragrédiente $\breve{\varrho}$ est une représentation unitaire de G dans $E'$.

D’après EVT, V, p. 15, th. 3 et remarque suivante, l’application $u$ est un isomorphisme isométrique.

Pour tout $g$ dans G, tout $x$ dans E et tout $y$ dans E, on a

$$
\langle y,( \breve{\varrho}(g)\circ u)(x)\rangle =\langle \varrho (g^{-1})y, u(x)\rangle
$$

$$
=\langle x|\varrho (g^{-1})y\rangle =\langle \varrho (g)x|y\rangle =\langle y, u(\overline{\varrho}(g)x)\rangle
$$

donc $\breve{\varrho}(g)\circ u=u\circ \overline{\varrho}(g)$, ce qui démontre a) ; l’assertion b) en découle aussitôt.

#### Corollaire {#ts-v-s1-n5-cor-1 .statement tag=038Y}

Soit $\varrho$ une représentation unitaire d’un groupe topologique G dans un espace hilbertien E. Les conditions suivantes sont équivalentes :

(i) La représentation $\varrho$ est irréductible ;

(ii) La représentation contragrédiente $\breve{\varrho}$ est irréductible ;

(iii) La représentation conjuguée $\overline{\varrho}$ est irréductible.

Cela résulte de la proposition 2, et de la remarque précédant celle-ci concernant les sous-représentations de E.

#### Proposition 3 {#ts-v-s1-prop-3 .statement tag=038Z}

Soit $\varrho$ une représentation unitaire d’un groupe topologique G dans un espace hilbertien E. Soit $\pi$ une sous-représentation de E et F l’espace de $\pi$. L’orthogonal $F^{\circ}$ de F dans E est une sous-représentation de E telle que $E = F\oplus F^{\circ}$ et $F^{\circ}$ est isomorphe à $E/F$.

L’espace $F^{\circ}$ est fermé. Pour tout $x\in F^{\circ}$, tout $g\in G$ et tout $y\in F$, on a $\langle \varrho (g)x|y\rangle =\langle x|\varrho (g^{-1})y\rangle = 0$ puisque $\varrho$ est unitaire et que F est une sous-représentation. Donc $\varrho (g)x\in F^{\circ}$.

La projection canonique de E sur $E/F$ est un G-morphisme, donc l’application de $F^{\circ}$ dans $E/F$ qui s’en déduit par passage au sous-espace est un G-morphisme de $F^{\circ}$ dans $E/F$; d’après EVT, V, p. 13, c’est un isomorphisme isométrique.

On notera également $\pi^{\circ}$ la représentation de G dans $F^{\circ}$.

#### Proposition 4 {#ts-v-s1-prop-4 .statement tag=0390}

Soit $\varrho$ une représentation unitaire d’un groupe topologique G dans un espace hilbertien E. Un sous-espace fermé F de E est une sous-représentation de $\varrho$ si et seulement si l’orthoprojecteur $p$ de E d’image F est un G-morphisme de $\varrho$ dans $\varrho$.

Supposons que F est une sous-représentation de $\varrho$. Soit $x\in E$ et écrivons $x=p(x) +y$ où $y\in F^{\circ}$. Pour tout $g$ dans G, on a

$$
\varrho (g)x=\varrho (g)(p(x)) +\varrho (g)y
$$

et comme $\varrho (g)(p(x))$ appartient à F et $\varrho (g)y$ à $F^{\circ}$ (prop. 3), on a $p(\varrho (g)x) =\varrho (g)(p(x))$. Donc $p$ appartient à Hom$_G(\varrho , \varrho )$.

Réciproquement, si $p\in$ Hom$_G(\varrho , \varrho )$ alors $1_E-p$ est un G-morphisme, donc F = Ker(1$_E-p)$ est une sous-représentation de $\varrho$.

### 6. Somme directe hilbertienne et produit tensoriel de repré- sentations unitaires

Soit G un groupe topologique. Soit $(\varrho_i)_{i\in I}$ une famille de représentations unitaires de G dans des espaces hilbertiens $E_i$. Soit E l’espace somme hilbertienne externe des $E_i$ (EVT, V, p. 18, déf. 1). Pour tout $g$ dans G et pour tout $x= (x_i)_{i\in I}$ dans E, on a

$$
\sum_i\|\varrho_i(g)x_i\|^2=\sum_i\|x_i\|^2=\|x\|^2
$$

ce qui prouve que $(\varrho_i(g)x_i)_{i\in I}$ est dans E et a même norme que $x$. Ainsi l’élément $\varrho (g) : (x_i)_{i\in I}\mapsto (\varrho_i(g)x_i)_{i\in I}$ est un élément unitaire de $\mathscr{L}(E)$.

#### Lemme 7 {#ts-v-s1-lem-7 .statement tag=0391}

L’application $g\mapsto \varrho (g)$ est une représentation unitaire de G dans E.

D’après le lemme 4 de V, p. 380, il suffit de démontrer que pour tout $i$ dans I et tout $x$ dans $E_i$, l’application $g\mapsto \varrho (g)x$ est continue en l’élément neutre $e$ de G. Cette application est la composition de l’application continue $g\mapsto \varrho_i(g)x_i$ et de l’injection canonique de $E_i$ dans E. Elle est donc continue.

La représentation $\varrho$ est appelée somme hilbertienne des représentations unitaires $(\varrho_i)_{i\in I}$; on la note $\varrho =\bigoplus_{i\in I}\varrho_i$.

Soient G et H des groupes topologiques. Soit $\varrho_1$ (resp. $\varrho_2)$ une représentation unitaire de G (resp. H) dans un espace hilbertien $E_1$ (resp. $E_2)$. Soit $E = E_1\widehat{\otimes}_2E_2$ l’espace hilbertien produit tensoriel de $E_1$ et $E_2$ (EVT, V, p. 28, déf. 1). Pour $(g, h)\in G\times H$, soit $\varrho (g, h)$ l’endomorphisme continu $\varrho_1(g)\widehat{\otimes}_2\varrho_2(h)$ de E (EVT, V, p. 28) ; on le notera simplement $\varrho_1(g)\otimes \varrho_2(h)$ lorsqu’aucune ambiguïté ne sera à craindre.

#### Lemme 8 {#ts-v-s1-lem-8 .statement tag=0392}

a) L’application $\varrho : (g, h)\mapsto \varrho (g, h)$ est une représentation unitaire de $G\times H$ dans E ;

b) Pour toute base orthonormale $(e_i)_{i\in I}$ de $E_1$, l’application de la somme hilbertienne $\bigoplus_{i\in I}E_2$ dans E définie par $(y_i)_{i\in I}\mapsto \sum_{i\in I}e_i\otimes y_i$ est un H-isomorphisme isométrique de la somme hilbertienne $\bigoplus_{i\in I}\varrho_2$ dans Res$^{G\times H}_{\{e\}\times H}(\varrho )$;

c) Pour toute base orthonormale $(f_j)_{j\in J}$ de $E_2$, l’application de la somme hilbertienne $\bigoplus_{j\in J}E_1$ dans E définie par $(x_j)_{j\in J}\mapsto \sum_{j\in J}x_j\otimes f_j$ est un G-isomorphisme isométrique de la somme hilbertienne $\bigoplus_{j\in J}\varrho_1$ dans Res$^G_G^{\times}_{\times \{}^H_{e\}}(\varrho )$.

L’application $(g, h)\mapsto \varrho (g, h)$ est un homomorphisme de G dans $\mathbf{G}\mathbf{L}(E) ($cf. EVT, V, p. 28, n$^o2)$. Soit $(e_i)_{i\in I}$ une base orthonormale de $E_1$. D’après EVT, V, p. 29, prop. 3 et cor. 2, l’application

$$
u: (y_i)\mapsto \sum_{i\in I}e_i\otimes y_i
$$

est une isométrie de la somme hilbertienne $F_2=\bigoplus_{i\in I}E_2$ sur E. Par le truchement de cette isométrie, la représentation $\varrho_H:h\mapsto \varrho (e, h)$ de H dans E s’identifie à la représentation somme directe des représentations $(\varrho_2)_{i\in I}$ dans $F_2$. En particulier, c’est une représentation unitaire de H dans E (lemme 7). De même, l’homomorphisme $\varrho_G:g\mapsto \varrho (g, e)$ est une représentation unitaire de G dans E.

Soit $(g, h)\in G\times H$. On a $\varrho (g, h) =\varrho_G(g)\circ \varrho_H(h)$, donc $\varrho (g, h)$ est unitaire ; de plus, $\varrho_G(g)$ et $\varrho_H(h)$ sont permutables, donc le lemme 1 de V, p. 377 implique que $\varrho$ est une représentation unitaire de $G\times H$.

Enfin, les assertions concernant la restriction de $\varrho$ aux sous-groupes $\{e\} \times H$ et $G\times  \{e\}$ ont été obtenues au cours de l’argument précédent.

La représentation $(g, h)\mapsto \varrho_1(g)\otimes \varrho_2(h)$ de $G\times H$ est appelée produit tensoriel externe des représentations unitaires $\varrho_1$ et $\varrho_2$, et notée $\varrho_1\boxtimes \varrho_2$.

Soit $n\in \mathbf{N}$ et soit $(G_i)_{1\leqslant i\leqslant n}$ une famille finie de groupes topologiques. Soit $\varrho_i$ une représentation unitaire de $G_i$ dans un espace hilbertien $E_i$ pour $1\leqslant i\leqslant n$. On définit de même une représentation

$$
\varrho_1\boxtimes \cdots \boxtimes \varrho_n
$$

de $G_1\times  \cdots  \times G_n$ dans l’espace hilbertien $E = E_1\widehat{\otimes}_2\cdots \widehat{\otimes}_2E_n$ (EVT, V, p. 27).

Supposons que $G_i= G$ pour $1\leqslant i\leqslant n$. Soit $\Delta_n: G\rightarrow G^n$ l’homomorphisme défini par $g\mapsto (g, . . . , g)$ pour tout $g\in G$. On note $\varrho_1\otimes  \cdots  \otimes \varrho_n$ la représentation unitaire $(\varrho_1\boxtimes \cdots \boxtimes \varrho_n)\circ \Delta_n$ de G. On dit que c’est le produit tensoriel des représentations unitaires $\varrho_i$.

Pour toute permutation $\sigma$ de $\{1, . . . , n\}$, l’isomorphisme canonique

$$
E_1\widehat{\otimes}_2\cdots \widehat{\otimes}_2E_n\rightarrow E_{\sigma(1)}\widehat{\otimes}_2\cdots \widehat{\otimes}_2E_{\sigma(n)}
$$

(EVT, V, p. 28) est un isomorphisme isométrique

$$
\varrho_1\otimes  \cdots  \otimes \varrho_n\rightarrow \varrho_{\sigma(1)}\otimes  \cdots  \otimes \varrho_{\sigma(n)}
$$

de représentations de G.

Si $\varrho_i=\varrho$ pour $1\leqslant i\leqslant n$, où $\varrho$ est une représentation unitaire de G, on note aussi $\varrho^{\otimes n}$ la représentation produit tensoriel des $\varrho_i$, et on dit que c’est la $n^e$ puissance tensorielle de $\varrho$.

### 7. Coefficients matriciels

#### Définition 5 {#ts-v-s1-def-5 .statement tag=0393}

Soit G un groupe topologique et soit $\varrho$ une représentation unitaire de G dans un espace hilbertien E. Soient $x$ et $y$ des éléments de E. La fonction de G dans K donnée par $g\mapsto  \langle x|\varrho (g)y\rangle$ est appelée un coefficient matriciel de $\varrho$, ou une fonction représentative. Si $x=y$, on dit que c’est un coefficient matriciel diagonal. Si $\varrho$ est de dimension finie, on dit que c’est un coefficient matriciel de dimension finie.

Les coefficients matriciels de $\varrho$ sont des fonctions continues et bornées sur G. On note Υ(G) (resp. Θ(G)) l’ensemble des coefficients matriciels de représentations unitaires complexes (resp. complexes et de dimension finie) de G.

#### Proposition 5 {#ts-v-s1-prop-5 .statement tag=0394}

Soit G un groupe topologique. Les ensembles Θ(G) et Υ(G) sont des sous-algèbres involutives unifères de $\mathscr{C}_b(G)$.

La fonction constante 1 est un coefficient matriciel de la représentation triviale de G sur $\mathbf{C}$. Soit $\varrho$ une représentation unitaire de G et soient $x$ et $y$ des vecteurs de l’espace de $\varrho$. Pour tout $\lambda \in \mathbf{C}$ et tout $g\in G$, on a $\lambda \langle x|\varrho (g)y\rangle =\langle x|\varrho (g)(\lambda y)\rangle$. De plus, on a

$$
\langle x|\varrho (g)y\rangle =\langle \varrho (g^{-1})x|y\rangle =\overline{\langle y|\varrho(g^{-1})x\rangle}
$$

pour tout $g\in G$. Par conséquent, les ensembles Θ(G) et Υ(G) sont stables par multiplication par des scalaires et par conjugaison.

Soient $\varrho_1$ et $\varrho_2$ des représentations unitaires de G ; soient $(x_1, y_1)$ des vecteurs de l’espace de $\varrho_1$ et $(x_2, y_2)$ des vecteurs de l’espace de $\varrho_2$. Pour tout $g\in G$, on a alors

$$
\langle x_1|\varrho_1(g)y_1\rangle +\langle x_2|\varrho_2(g)y_2\rangle =\langle (x_1, x_2)|(\varrho_1\oplus \varrho_2)(g)(y_1, y_2)\rangle
$$

$$
\langle x_1|\varrho_1(g)y_1\rangle \langle x_2|\varrho_2(g)y_2\rangle =\langle x_1\otimes x_2|(\varrho_1\otimes \varrho_2)(g)(y_1\otimes y_2)\rangle
$$

ce qui prouve que Θ(G) et Υ(G) sont stables par addition et par produit. La proposition en résulte.

### 8. Le lemme de Schur

Dans ce numéro, les espaces hilbertiens sont complexes.

#### Proposition 6 (Lemme de Schur) {#ts-v-s1-prop-6 .statement tag=0395}

Soit $\varrho$ une représentation unitaire d’un groupe topologique G dans un espace hilbertien non nul E. Alors $\varrho$ est irréductible si et seulement si Hom$_G(\varrho , \varrho )$ est égal à $\mathbf{C}\cdot 1_E$.

L’espace Hom$_G(\varrho , \varrho )$ est une sous-algèbre stellaire unifère de $\mathscr{L}(E)$ (lemme 5 de V, p. 380). Pour toute sous-représentation F de E, le projecteur orthogonal $p$ d’image F est un élément idempotent de l’algèbre stellaire Hom$_G(\varrho , \varrho )$ (prop. 4 de V, p. 383). Si celle-ci est égale à $\mathbf{C}\cdot 1_E$, cela signifie que $p= 0$ ou $p= 1_E$, ce qui veut dire que F = 0 ou F = E. Donc $\varrho$ est irréductible.

Réciproquement, supposons $\varrho$ irréductible. Soient $u$ et $v$ des éléments permutables de l’algèbre stellaire Hom$_G(\varrho , \varrho )$ tels que $uv= 0$. Supposons $u$ non nul. Le noyau F de $u$ définit alors une sous-représentation de $\varrho$ différente de E, donc F est réduit à 0 ; comme F contient l’image de $v$, on en déduit que $v= 0$. D’après la proposition 10 de I, p. 113, on a donc Hom$_G(\varrho , \varrho ) =\mathbf{C}\cdot 1_E$.

#### Corollaire 1 {#ts-v-s1-prop-6-cor-1 .statement tag=0396}

Soit $\pi$ une représentation unitaire irréductible d’un groupe topologique G dans un espace hilbertien E. Soit $u$ un opérateur partiel fermé sur E. On suppose que $u$ est à domaine dense, que dom($u$) est stable par $\pi$ et que $u\circ \pi (g) =\pi (g)\circ u$ pour tout $g\in G$. Alors dom($u$) $= E$ et $u$ est une homothétie.

L’opérateur partiel $u^*\circ u$ est un opérateur partiel auto-adjoint positif sur E (prop. 12 de IV, p. 241), il en est de même pour $v= 1_E+u^*\circ u$ et ce dernier est injectif puisque $-1\in /$ Sp($u^*\circ u$) (prop. 17 de IV, p. 248). On a $u^*\circ \pi (g) =\pi (g)\circ u^*$ pour tout $g\in G$ (lemme 6 de V, p. 381), d’où $v\circ \pi (g) =\pi (g)\circ v$ pour tout $g\in G$. Comme $v$ est injectif, il en résulte que $v^{-1}\circ \pi (g) =\pi (g)\circ v^{-1}$ pour tout $g\in G$. Mais $v^{-1}$ appartient à $\mathscr{L}$ (E), donc d’après la prop. 6, il existe $\lambda \in \mathbf{C}$ tel que $v^{-1}=\lambda 1_E$. On a nécessairement $\lambda \not = 0$, ce qui implique que E = Im($v^{-1}$) $=$ dom($v$)$\subset$ dom($u$), d’où dom($u$) $= E$. Comme $u$ est fermé, on a $u\in \mathscr{L}(E)$ (EVT, I, p. 19, cor. 5), donc $u\in$ Hom$_G(\pi , \pi )$ et $u$ est une homothétie d’après la prop. 6.

#### Corollaire 2 {#ts-v-s1-prop-6-cor-2 .statement tag=0397}

Soient $\varrho$ et $\pi$ des représentations unitaires irréductibles d’un groupe topologique G dans des espaces hilbertiens E et F respectivement. L’espace Hom$_G(\varrho , \pi )$ est de dimension 1 si $\varrho$ est isomorphe à $\pi$, et est nul sinon. En particulier, si $\varrho$ est isomorphe à $\pi$, tout G-morphisme non nul de $\varrho$ dans $\pi$ est un isomorphisme.

Supposons qu’il existe un G-morphisme non nul $u$ de $\varrho$ dans $\pi$. L’application linéaire $u^*\circ u$ est un élément de Hom$_G(\varrho , \varrho )$, donc il existe un nombre complexe $\lambda$ tel que $u^*\circ u=\lambda \cdot 1_E$ (prop. 6). On a alors

$$
\langle u(x)|u(y)\rangle =\langle x|u^*u(y)\rangle =\lambda \langle x|y\rangle
$$

pour tous $x$ et $y$ dans E. En particulier, $\lambda \not = 0$ puisque $u$ est non nul. Comme $\|u(x)\|=|\lambda |^{1/2}\|x\|$ pour tout $x\in E$, l’application linéaire $u$ est injective, et l’image de $u$ est fermée dans F (lemme 8 de I, p. 107) ; c’est alors une sous-représentation non nulle de la représentation irréductible $\pi$, d’où on déduit que $u$ est surjective. Ainsi, $u$ est un isomorphisme de $\varrho$ dans $\pi$. L’application $v\mapsto u^*\circ v$ est alors un isomorphisme de l’espace Hom$_G(\varrho , \pi )$ dans l’espace Hom$_G(\varrho , \varrho )$, qui est de dimension 1 (prop. 6).

#### Corollaire 3 {#ts-v-s1-prop-6-cor-3 .statement tag=0398}

Soit $\varrho$ une représentation unitaire d’un groupe topologique G dans un espace hilbertien E. La représentation $\varrho$ est irréductible si et seulement si l’espace Sesq$_G(\varrho , \varrho )$ est de dimension 1. Cet espace est alors engendré par le produit scalaire sur E.

Au vu de la prop. 1 de V, p. 381, cela résulte de la prop. 6.

#### Corollaire 4 {#ts-v-s1-prop-6-cor-4 .statement tag=0399}

Soient $\varrho_1$ et $\varrho_2$ des représentations unitaires irréductibles non isomorphes d’un groupe topologique G dans des espaces hilbertiens $E_1$ et $E_2$. L’espace Sesq$_G(\varrho_1, \varrho_2)$ est nul.

D’après la prop. 1 de V, p. 381, cela résulte du cor. 2.

#### Corollaire 5 {#ts-v-s1-prop-6-cor-5 .statement tag=039A}

Soit $\varrho$ une représentation unitaire d’un groupe topologique G dans un espace hilbertien E. Soit $\pi$ une représentation irréductible unitaire de G dans un espace hilbertien F.

a) Pour tout G-morphisme $u$ non nul de $\pi$ dans $\varrho$, il existe $\lambda \in \mathbf{R}^*_+$ tel que $\lambda u$ est isométrique ;

b) Tout G-morphisme $u$ de $\pi$ dans $\varrho$ a une image fermée ;

c) Tout G-morphisme non nul $v$ de $\varrho$ dans $\pi$ est surjectif.

Démontrons l’assertion a), qui implique l’assertion b) (lemme 8 de I, p. 107). Puisque le morphisme $u$ est non nul, il est injectif (lemme 2 de V, p. 378). La formule $q(x, y) =\langle u(x)|u(y)\rangle$ pour $x$ et $y$ dans F définit alors une forme sesquilinéaire continue sur F. Comme $u$ est un G-morphisme, on a $q(\pi (g)x, \pi (g)y) =q(x, y)$ pour tous $g$ dans G et $(x, y)\in F\times F$, donc $q$ est G-invariante. D’après le cor. 3, il existe $\alpha \in \mathbf{R}^*_+$ tel que

$$
q(x, y) =\langle u(x)|u(y)\rangle =\alpha \langle x|y\rangle
$$

pour tout $(x, y)\in F\times F$, et donc $\alpha^{-1/2}u$ est isométrique.

Démontrons enfin l’assertion c). Puisque $\pi$ est irréductible, l’image de $v$ est dense dans F (lemme 2 de V, p. 378), donc l’adjoint $v^*$ est injectif (EVT, V, p. 41, prop. 4). D’après b), l’image H de $v^*$ est un sous-espace fermé de E ; c’est donc une sous-représentation de $\varrho$, et $v^*$ induit par passage aux sous-espaces un G-isomorphisme de F dans H. La restriction $w$ de $v$ à H définit un G-morphisme de H dans F, qui est injectif car son noyau est l’intersection de H et de Ker($v$) $= H^{\circ}$ (loc. cit.). L’application $w$ est donc un isomorphisme (corollaire 2) ; en particulier, $v$ est surjectif.

#### Corollaire 6 {#ts-v-s1-prop-6-cor-6 .statement tag=039B}

Soient $G_1$ et $G_2$ des groupes topologiques. Soient $\varrho_1$ une représentation unitaire irréductible de $G_1$ dans un espace hilbertien $E_1$ et $\varrho_2$ une représentation unitaire irréductible de $G_2$ dans un espace hilbertien $E_2$. Le produit tensoriel externe $\varrho_1\boxtimes \varrho_2$ est une représentation unitaire irréductible de $G_1\times G_2$ dans $E_1\widehat{\otimes}_2E_2$.

Le produit tensoriel externe $\varrho =\varrho_1\boxtimes \varrho_2$ est une représentation unitaire de $G = G_1\times G_2$ dans l’espace $E = E_1\widehat{\otimes}_2E_2$ d’après le lemme 8 de V, p. 384.

Soit $q$ une forme sesquilinéaire $(G_1\times G_2$)-invariante sur E. Pour tout couple $(x_1, y_1)\in E^2_1$, l’application $(x_2, y_2)\mapsto q(x_1\otimes x_2, y_1\otimes y_2)$ appartient à Sesq$_{G_2}(\varrho_2, \varrho_2)$. Notons $b(x_1, y_1)$ l’unique nombre complexe tel que

$$
q(x_1\otimes x_2, y_1\otimes y_2) =b(x_1, y_1)\langle x_2|y_2\rangle
$$

pour tout $(x_2, y_2)\in E^2_2$ (cor. 3). Soit $\varepsilon \in E_2$ de norme 1, de sorte que $b(x_1, y_1) =q(x_1\otimes \varepsilon , y_1\otimes \varepsilon )$ pour tout $(x_1, y_1)\in E^2_1$. Cette formule implique que l’application $b$ est sesquilinéaire sur $E_1$. De plus

$$
\|b(x_1, y_1)\|\leqslant \|q\| \|x_1\otimes \varepsilon \| \|y_1\otimes \varepsilon \|=\|q\| \|x_1\| \|y_1\|
$$

pour tout $(x_1, y_1)\in E^2_1$ (EVT, V, p. 26, formule (5)), donc $b$ est continue.

Soient $g\in G$ et $(x_1, y_1)\in E^2_1$. Puisque $\varrho_2$ est unitaire et que $q$ est invariante, il vient

$$
b(\varrho_1(g)x_1, \varrho_1(g)y_1) =q(x_1\otimes \varrho_2(g^{-1})\varepsilon , y_1\otimes \varrho_2(g^{-1})\varepsilon ) =b(x_1, y_1)
$$

de sorte que $b\in$ Sesq$_{G_1}(\varrho_1, \varrho_1)$. Il existe donc un unique $\lambda \in \mathbf{C}$ tel que $b(x_1, y_1) =\lambda \langle x_1|y_1\rangle$ pour tout $(x_1, y_1)\in E^2_1$ (cor. 3), c’est-à-dire

$$
q(x_1\otimes x_2, y_1\otimes y_2) =\lambda \langle x_1|y_1\rangle \langle x_2|y_2\rangle
$$

pour tout $(x_1, y_1, x_2, y_2)\in E^2_1\times E^2_2$. On en déduit que l’espace Sesq$_{G_1\times G_2}(\varrho , \varrho )$ est de dimension 1, ce qui implique que la représentation $\varrho =\varrho_1\boxtimes \varrho_2$ est irréductible (loc. cit.).

On rappelle que $\mathbf{U}$ désigne le groupe des nombres complexes de module 1.

#### Corollaire 7 {#ts-v-s1-prop-6-cor-7 .statement tag=039C}

Soit $\pi$ une représentation unitaire irréductible d’un groupe topologique G dans un espace hilbertien E. Il existe un homomorphisme continu $\chi$ du centre C de G dans $\mathbf{U}$ tel que $\pi (z) =\chi (z)\cdot 1_E$ pour tout $z\in C$. En particulier, si G est commutatif, on a dim(E) = 1.

Pour $z\in C$, l’application $\pi (z)$ appartient à Hom$_G(\pi , \pi )$; elle est donc de la forme $\chi (z)\cdot 1_E$ pour un certain nombre complexe $\chi (z)$ (prop. 6). Comme $\pi (z)$ est une application unitaire, on a $|\chi (z)|= 1$. De plus, comme $\pi$ est un homomorphisme, l’application $z\mapsto \chi (z)$ est un homomorphisme. Fixons $v\not = 0$ dans E ; l’application $z\mapsto \chi (z)v=\pi (z)v$ de C dans $\mathbf{U}$ est continue, et donc l’homomorphisme $\chi$ est continu.

Enfin, si G est commutatif, on a C = G, donc $\pi (g) =\chi (g)\cdot 1_E$ pour tout $g$ dans G ; tout sous-espace de dimension 1 de E est alors une sous-représentation de $\pi$, et puisque $\pi$ est irréductible, l’espace E doit être de dimension 1.

#### Définition 6 {#ts-v-s1-def-6 .statement tag=039D}

Soit $\pi$ une représentation unitaire irréductible d’un groupe topologique G dans un espace hilbertien E. L’homomorphisme $\chi$ du centre C de G dans $\mathbf{U}$ tel que $\pi (z) =\chi (z)\cdot 1_E$ pour tout $z$ dans C est appelé le caractère central de $\pi$.

#### Remarque {#ts-v-s1-n8-rem-1 .statement tag=039E}

Soit $\pi$ (resp. $\varrho )$ une représentation unitaire irréductible d’un groupe topologique G (resp. H) dans un espace hilbertien E (resp. F). Notons $\chi$ (resp. $\eta )$ le caractère central de $\pi$ (resp. $\varrho )$. Le caractère central de la représentation $\overline{\pi}$ est $\overline{\chi}$, et le caractère central de la représentation unitaire irréductible $\pi \boxtimes \varrho$ de $G\times H$ (cor. 6) est le caractère $\chi \boxtimes \eta : (g, h)\mapsto \chi (g)\eta (h)$ de $G\times H$.

### 9. Semi-simplicité

#### Définition 7 {#ts-v-s1-def-7 .statement tag=039F}

Soit $\varrho$ une représentation unitaire d’un groupe topologique G dans un espace hilbertien E. On dit que $\varrho$ est semi-simple s’il existe une famille $(F_i)_{i\in I}$ de sous-représentations irréductibles de $\varrho$ telle que E est la somme hilbertienne des sous-espaces $F_i$.

On dit parfois aussi qu’une représentation unitaire semi-simple admet une décomposition discrète ou est discrètement décomposable.

Si $(\varrho_i)_{i\in I}$ est une famille de représentations unitaires semi-simples d’un groupe topologique G, alors la somme hilbertienne des représentations $\varrho_i$ est semi-simple.

#### Proposition 7 {#ts-v-s1-prop-7 .statement tag=039G}

Soit G un groupe topologique et soit $\varrho$ une représentation unitaire de G dans un espace hilbertien complexe E. La représentation $\varrho$ est semi-simple si et seulement si toute sous-représentation non nulle de $\varrho$ contient une sous-représentation irréductible.

Supposons que $\varrho$ est semi-simple. Soit $(F_i)_{i\in I}$ une famille de sous-représentations irréductibles de $\varrho$ telle que E est la somme hilbertienne des sous-espaces $F_i$. Soit F une sous-représentation non nulle de E. Il existe $i\in I$ tel que la restriction à F de l’orthoprojecteur d’image $F_i$ n’est pas nulle. Cet orthoprojecteur définit alors par passage aux sous-espaces un G-morphisme non nul $p_i$ de F dans $F_i$ (prop. 4 de V, p. 383). D’après le lemme de Schur, le G-morphisme $p_i$ est surjectif (cor. 5 de V, p. 388). L’orthogonal dans F du noyau de $p_i$ est une sous-représentation de F isomorphe à $F_i$ (prop. 3 de V, p. 383), donc irréductible.

Démontrons l’assertion réciproque. Soit $\mathscr{F}$ l’ensemble des sous-espaces fermés F de E stables par G tels que la sous-représentation de $\varrho$ dans F est irréductible. Soit $\mathscr{O}$ l’ensemble des parties $\mathscr{G}$ de $\mathscr{F}$ telles que les sous-espaces appartenant à $\mathscr{G}$ soient deux à deux orthogonaux.

L’ensemble $\mathscr{O}$ est de caractère fini (E, III, p. 34, déf. 2). Soit alors $\mathscr{G}$ un élément maximal de $\mathscr{O}$ (E, III, p. 35, th. 1). Soit $E_1$ le sous-espace de E somme hilbertienne des sous-représentations irréductibles F de $\mathscr{G}$. Si on avait $E_1\not = E$, l’orthogonal de $E_1$ ne serait pas nul, et la sous-représentation de G dans $E^{\circ}_1$ contiendrait par hypothèse une sous-représentation irréductible. L’espace F de celle-ci serait orthogonal aux éléments de $\mathscr{G}$, de sorte que $\mathscr{G}\cup  \{F\} \in \mathscr{O}$; cela contredit la maximalité de $\mathscr{G}$, donc $E = E_1$, ce qui conclut la preuve.

#### Corollaire 1 {#ts-v-s1-prop-7-cor-1 .statement tag=039H}

Soit G un groupe topologique et soit $\varrho$ une représentation unitaire semi-simple de G dans un espace hilbertien complexe E. Toute sous-représentation de $\varrho ($resp. toute représentation quotient de $\varrho )$ est semi-simple.

Si $\varrho_1$ est une sous-représentation de $\varrho$, alors toute sous-représentation non nulle de $\varrho_1$ contient une sous-représentation irréductible (prop. 7), donc $\varrho_1$ est semi-simple (loc. cit.).

D’après la prop. 3 de V, p. 383, toute représentation quotient de $\varrho$ est isomorphe à une sous-représentation de $\varrho$, donc est semi-simple.

#### Corollaire 2 {#ts-v-s1-prop-7-cor-2 .statement tag=039I}

Toute représentation unitaire $\varrho$ de dimension finie d’un groupe topologique G est semi-simple.

Cela résulte de la prop. 7 et du lemme 3 de V, p. 379.

#### Corollaire 3 {#ts-v-s1-prop-7-cor-3 .statement tag=039J}

Soient $\varrho_1$ et $\varrho_2$ des représentations unitaires de dimension finie d’un groupe topologique G. Les représentations $\varrho_1$ et $\varrho_2$ sont isomorphes si et seulement si $\chi_{\varrho_1}=\chi_{\varrho_2}$.

Cela découle du corollaire 2 et de A, VIII, p. 389, prop. 1, b).

### 10. Classes de représentations unitaires

#### Lemme 9 {#ts-v-s1-lem-9 .statement tag=039K}

Soit E un espace hilbertien sur K. Soit $F\subset E$ un sous-espace vectoriel dense dans E. Alors la dimension hilbertienne de E est inférieure ou égale à la dimension de F.

Si E est de dimension hilbertienne finie, celle-ci est égale à la dimension de E. Supposons que E est de dimension hilbertienne infinie. Le sous-espace F est alors de dimension infinie. Soit B une base orthonormale de E et soit $B'$ une base de F. Pour tout $x\in B$, il existe un élément $f(x)\in B'$ tel que $\langle x|f(x)\rangle  \not = 0$, puisque dans le cas contraire on aurait $x\in F^{\circ}=\{0\}$. On définit ainsi une application $f: B\rightarrow B'$.

$-1$

Pour tout $y\in B'$, l’ensemble $f(y)$ est contenu dans l’ensemble des $x\in B$ tels que $\langle x|y\rangle  \not = 0$, donc est dénombrable (EVT, V, p. 21, prop. 4). Par E, III, p. 50, prop. 4, on obtient Card(B) = Card($f(B)$)$\leqslant$ Card(B$')$.

Notons $Is_G(\pi_1, \pi_2)$ la relation

« G est un groupe topologique et $\pi_1,\pi_2$ sont des représentations

unitaires isomorphes de G dans des espaces hilbertiens sur K ».

Par rapport à $\pi_1$ et $\pi_2$, il s’agit d’une relation d’équivalence. Pour toute représentation unitaire $\pi$ de G dans un espace hilbertien sur K, on notera cl($\pi$ ) la classe d’équivalence de $\pi ($cf. E, II, p. 47) ; c’est donc une représentation unitaire de G isomorphe à $\pi$; on dit que cl($\pi$ ) est la classe de $\pi$. Des représentations unitaires $\pi_1$ et $\pi_2$ dans des espaces hilbertiens sur K sont isomorphes si et seulement si cl($\pi_1$) $=$ cl($\pi_2$).

Soit G un groupe topologique. Soit $\mathfrak{c}$ un cardinal. La relation

« $\lambda$ est une classe de représentation unitaire de G dans

un espace hilbertien complexe de dimension hilbertienne $\leqslant \mathfrak{c}$ »

est collectivisante en $\lambda$ (E, II, p. 3). En effet, tout espace hilbertien sur K de dimension $\leqslant \mathfrak{c}$ est isométriquement isomorphe à un sous-espace hilbertien de $\ell^2(\mathfrak{c})$ (EVT, V, p. 23, cor. 2), et l’assertion résulte alors de E, II, p. 47.

Soit $\pi$ une représentation unitaire irréductible de G dans un espace hilbertien E. Soit $x$ un élément non nul de E. Puisque $\pi$ est irréductible, le vecteur $x$ est un vecteur cyclique de $\pi$, ce qui implique que la dimension hilbertienne de E est $\leqslant$ Card(G) (lemme 9, appliqué au sous-espace dense engendré par les éléments $\pi (g)x$ pour $g\in G)$. Les classes des représentations unitaires irréductibles de G dans un espace hilbertien sur K appartiennent donc à l’ensemble des classes de représentations unitaires de G dans un espace hilbertien sur K de dimension hilbertienne $\leqslant$ Card(G) ; par conséquent, elles forment un ensemble.

#### Définition 8 {#ts-v-s1-def-8 .statement tag=039L}

On note $\widehat{G}$ l’ensemble des classes de représentations unitaires irréductibles de G dans un espace hilbertien complexe. On dit que $\widehat{G}$ est le dual unitaire de G.

Pour toute représentation unitaire irréductible $\pi$ de G dans un espace hilbertien complexe, on a donc cl($\pi$ )$\in \widehat{G}$.

#### Remarque 1 {#ts-v-s1-n10-rem-1 .statement tag=039M}

Supposons que G est un groupe commutatif. D’après le corollaire 7 de V, p. 390, toute représentation unitaire irréductible de G dans un espace hilbertien complexe est de dimension 1. Si G est localement compact, l’ensemble $\widehat{G}$ s’identifie à l’ensemble des caractères unitaires de G (déf. 1 de II, p. 201), et la notation $\widehat{G}$ est donc compatible avec celle introduite dans la déf. 2 de II, p. 201.

#### Remarque 2 {#ts-v-s1-n10-rem-2 .statement tag=039N}

Si G est fini, l’ensemble $\widehat{G}$ est en bijection avec l’ensemble des classes de $\mathbf{C}$[G]-modules simples (A, VIII, p. 47), qui est également noté $\widehat{G}$ dans A, VIII, p. 396.

#### Remarque 3 {#ts-v-s1-n10-rem-3 .statement tag=039O}

Pour $\pi \in \widehat{G}$, on identifiera $\overline{\pi}$ avec la classe dans $\widehat{G}$ de la représentation conjuguée de $\pi$.

#### Remarque 4 {#ts-v-s1-n10-rem-4 .statement tag=039P}

Si $\pi$ est une représentation unitaire irréductible de G dans un espace hilbertien complexe de dimension finie, son caractère $\chi_{\pi}$ ne dépend que de la classe de $\pi$. On peut donc parler de l’ensemble des caractères des représentations unitaires irréductibles complexes de dimension finie de G.

### 11. Composantes isotypiques

#### Définition 9 {#ts-v-s1-def-9 .statement tag=039Q}

Soit G un groupe topologique et soit $\pi$ une représentation continue irréductible de G. Soit $\varrho$ une représentation continue de G dans un espace localement convexe séparé E. On appelle composante $\pi$-isotypique de $\varrho$ l’adhérence dans E de la somme des espaces de toutes les sous-représentations de $\varrho$ isomorphes à $\pi$. On note $M_{\pi}(\varrho )$ ce sous-espace.

L’espace $M_{\pi}(\varrho )$ est un sous-espace fermé de E, qui définit une sous-représentation de $\varrho$. Cet espace ne dépend que de la classe de $\pi$ dans $\widehat{G}$.

#### Proposition 8 {#ts-v-s1-prop-8 .statement tag=039R}

Soit G un groupe topologique. Soit $\varrho$ une représentation unitaire de G dans un espace hilbertien complexe E.

a) Soient $\pi_1$ et $\pi_2$ des représentations unitaires irréductibles non isomorphes de G. Les sous-espaces $M_{\pi_1}(\varrho )$ et $M_{\pi_2}(\varrho )$ sont orthogonaux ;

b) Soient $\varrho '$ une représentation unitaire de G et $u$ un G-morphisme de $\varrho$ dans $\varrho '$. Pour toute représentation unitaire irréductible $\pi$ de G, on a $u(M_{\pi}(\varrho ))\subset M_{\pi}(\varrho ')$.

Soient $E_1$ et $E_2$ des sous-espaces de E définissant des sous-représentations isomorphes à $\pi_1$ et $\pi_2$ respectivement. L’orthoprojecteur de E d’image $E_2$ définit par passage aux sous-espaces un élément de Hom$_G(\pi_1, \pi_2)$, qui est nul (cor. 2 de V, p. 387), ce qui démontre que $E_2$ est orthogonal à $E_1$. Cela implique l’assertion a).

Pour l’assertion b), notons que $M_{\pi}(\varrho )$ est, par définition, l’adhérence dans E de l’espace engendré par les éléments $x\in E$ appartenant à un sous-espace fermé $F\subset E$ stable par $\varrho$ tel que la sous-représentation $\varrho_F$ de $\varrho$ dans F soit isomorphe à $\pi$. Il suffit donc de démontrer que, dans ce cas, on a $u(x)\in M_{\pi}(\varrho ')$. Soit $H =u(F)$; c’est un sous-espace fermé de l’espace de $\varrho '$ (cor. 5 de V, p. 388) stable par $\varrho '$ et $u$ induit par passage aux sous-espaces un G-morphisme surjectif de F dans H. Si H n’est pas nul, alors ce G-morphisme est un isomorphisme d’après le corollaire 2 de V, p. 387. La représentation de G sur H est donc alors isomorphe à $\pi$, d’où il résulte que $u(x)$ appartient à $M_{\pi}(\varrho ')$.

Pour tout espace vectoriel H et toute famille $(H_i)_{i\in I}$ de sous-espaces de H, on dit que les espaces $(H_i)_{i\in I}$ sont en somme directe si la famille $(H_i)_{i\in I}$ vérifie les conditions équivalentes de la prop. 11 de A, II, p. 18.

#### Proposition 9 {#ts-v-s1-prop-9 .statement tag=039S}

Soit G un groupe topologique et soit $\varrho$ une représentation unitaire de G dans un espace hilbertien complexe E. Soit $\pi$ une représentation unitaire irréductible de G dans un espace hilbertien complexe $E_{\pi}$. Notons $v$ l’application linéaire de Hom$_G(\pi , \varrho )\otimes E_{\pi}$ dans E telle que $v(u\otimes x) =u(x)$ pour tout $(u, x)\in$ Hom$_G(\pi , \varrho )\times E_{\pi}$.

L’application linéaire $v$ est injective et son image est la somme des espaces de toutes les sous-représentations de $\varrho$ qui sont isomorphes à $\pi$. En particulier, l’image de $v$ est dense dans $M_{\pi}(\varrho )$.

Le cor. 5 de V, p. 388 implique que l’image de $v$ est la somme des espaces de toutes les sous-représentations de $\varrho$ qui sont isomorphes à $\pi$.

Démontrons que $v$ est injective. Soit $(u_i)_{i\in I}$ une base de l’espace vectoriel Hom$_G(\pi , \varrho )$. Pour $i\in I$, notons $F_i$ l’image de $u_i$ et $\widetilde{u}_i: E_{\pi}\rightarrow F_i$ le G-isomorphisme déduit de $u_i$ par passage aux sous-espaces.

Démontrons d’abord, par récurrence sur le cardinal d’un sous-ensemble fini J de I, que les sous-espaces $(F_i)_{i\in J}$ sont en somme directe.

Le cas où J est vide est immédiat. Supposons que J n’est pas vide et que la propriété demandée vaut pour les sous-ensembles de I de cardinal au plus Card(J) $-1$.

Soit $j$ un élément fixé de J. L’hypothèse de récurrence implique que les sous-espaces $F_i$ pour $i\in J-\{j\}$ sont en somme directe. Soit $F'$ leur somme ; il suffit maintenant de démontrer que $F_j\cap F'=\{0\}$.

Supposons que l’intersection de $F_j$ et de $F'$ ne soit pas réduite à 0 ; cette intersection est une sous-représentation de $F_j$, et comme celle-ci est irréductible, on a donc $F_j\cap F'= F_j$, d’où $F_j\subset F'$.

Pour $i\in J-\{j\}$, notons pr$_i: F'\rightarrow F_i$ la projection et $\iota_i: F_i\rightarrow F'$ l’inclusion. On a un isomorphisme canonique

Hom$_G(F_j,F')\rightarrow \bigoplus_{i\in J-\{j\}}$ Hom$_G(F_j,F_i)$

(formule (1), p. 377) tel que $u: F_j\rightarrow F'$ a pour image la famille (pr$_i\circ u)_{i\in J-\{j\}}$ (A, II, p. 13, cor. 1). Le corollaire 2 de V, p. 387 implique que $\widetilde{u}_i\circ \widetilde{u}^{-1}_j$, qui est non nul, est une base de l’espace Hom$_G(F_j,F_i)$. Par conséquent, la famille des G-morphismes $(\iota_i\circ \widetilde{u}_i\circ \widetilde{u}^{-1}_j)_{i\in J-\{j\}}$ est une base de Hom$_G(F_j,F')$.

Notons $\iota$ l’inclusion de $F_j$ dans $F'$; c’est un élément de Hom$_G(F_j,F')$, donc c’est une combinaison linéaire des G-morphismes $\iota_i\circ \widetilde{u}_i\circ \widetilde{u}^{-1}_j$ pour $i\in J-\{j\}$. Il en résulte que $u_j$ est combinaison linéaire des applications $u_i$ pour $i\not =j$, ce qui contredit l’indépendance linéaire de la famille $(u_i)_{i\in I}$. L’assertion est donc démontrée par récurrence.

Démontrons maintenant que $v$ est injective. Soit $w$ un élément de Hom$_G(\pi , \varrho )\otimes E_{\pi}$. Il existe une unique famille $(x_i)_{i\in I}$ dans $E_{\pi}$ à support fini telle que

$$
w=\sum_{i\in I}u_i\otimes x_i
$$

(A, II, p. 62, cor. 1) et on a alors

$$
v(w) =\sum_{i\in I}u_i(x_i)
$$

D’après ce qui précède, la condition $v(w) = 0$ implique donc que $u_i(x_i) = 0$ pour tout $i\in I$, d’où $x_i= 0$ pour tout $i$ puisque $u_i$ est injectif, et donc $w= 0$.

#### Proposition 10 {#ts-v-s1-prop-10 .statement tag=039T}

Soit G un groupe topologique. Soit $\pi$ une représentation unitaire irréductible de G dans un espace hilbertien complexe $E_{\pi}$ et soit $\varrho$ une représentation unitaire de G dans un espace hilbertien complexe E.

Il existe des familles $(E_i)_{i\in I}$ de sous-espaces fermés invariants de E tels que la sous-représentation de $\varrho$ dans $E_i$ soit isomorphe à $\pi$ pour tout $i\in I$ et telle que $M_{\pi}(\varrho )$ soit la somme hilbertienne des espaces $E_i$. De plus, le cardinal de I est indépendant de la famille $(E_i)_{i\in I}$ vérifiant ces propriétés.

Démontrons l’existence de familles vérifiant les conditions indiquées. Soit $\mathscr{O}$ l’ensemble des parties C de Hom$_G(\pi , \varrho )-\{0\}$ telles que les sous-espaces $u(E_{\pi})$ pour $u\in C$ soient deux à deux orthogonaux. L’ensemble $\mathscr{O}$ est ordonné par l’inclusion. Il est non vide car la partie vide est en un élément, et il est de caractère fini (E, III, p. 34, déf. 2) puisque C appartient à $\mathscr{O}$ si et seulement si les ensembles contenant deux éléments de C appartiennent à $\mathscr{O}$. D’après E, III, p. 35, th. 1, il existe un élément maximal C de $\mathscr{O}$. Soit F l’adhérence du sous-espace engendré par les espaces $u(E_{\pi})$ pour $u\in C$; c’est la somme hilbertienne des espaces $u(E_{\pi})$ pour $u\in C$. Nous allons démontrer que $F = M_{\pi}(\varrho )$, ce qui démontrera que la famille $(u(E_{\pi}))_{\pi\in C}$ a les propriétés demandées.

Par définition, $u(E_{\pi})\subset M_{\pi}(\varrho )$ pour tout $u\in C$, donc F est contenu dans $M_{\pi}(\varrho )$. Pour démontrer l’inclusion réciproque, il suffit de démontrer que si $v$ est un G-morphisme de $\pi$ dans $\varrho$, alors son image est contenue dans F. Soit $p$ l’orthoprojecteur de E d’image $F^{\circ}$; c’est un G-morphisme, puisque F est une sous-représentation de E (prop. 4 de V, p. 383). L’image du G-morphisme $p\circ v$ est orthogonale à F ; elle est donc nulle (sinon $C\cup  \{p\circ v\} \in \mathscr{O}$, ce qui contredit la maximalité de C), et par conséquent l’image de $v$ est contenue dans F.

Soient maintenant $(E_i)_{i\in I}$ et $(F_j)_{j\in J})$ des familles de sous-espaces fermés invariants de E, deux à deux orthogonaux, tels que la sous-représentation de G dans $E_i$ (resp. dans $F_j)$ est isomorphe à $\pi$ pour tout $i\in I$ (resp. pour tout $j\in J)$, et telles que $M_{\pi}(\varrho )$ est somme hilbertienne de la famille $(E_i)_{i\in I}$ et de la famille $(F_j)_{j\in J}$.

Si I est fini, alors

dim Hom$_G(\pi ,M_{\pi}(\varrho )) =$ dim Hom$_GE_{\pi},\bigoplus_{i\in I}E_i$ = Card(I)

(formule (1) de V, p. 377 et cor. 2 de V, p. 387). Pour tout sous-ensemble fini L de J, on a alors

Card(L) = dim Hom$_GE_{\pi},\bigoplus_{i\in L}F_j$

$\leqslant$ dim Hom$_G(\pi ,M_{\pi}(\varrho )) =$ Card(I)

(loc. cit.). Cela démontre que J est alors fini et que Card(I) = Card(J), comme désiré. De même, si J est fini, alors I est fini et a le même cardinal.

Supposons maintenant que I et J sont infinis. Pour $j\in J$, notons $p_j$ l’orthoprojecteur de E d’image $F_j$. Pour $i\in I$, soit $x_i$ un élément non nul de $E_i$; c’est un vecteur cyclique de $E_i$. Observons que puisque $p_j$ induit par passage aux sous-espaces un G-morphisme de $E_i$ dans $F_j$, l’espace $p_j(E_i)$ est nul si et seulement si $p_j(x_i) = 0$ (en effet, l’espace $E_i\cap$Ker($p_j$) est soit nul, soit égal à $E_i)$.

Pour tout $j\in J$, il existe un élément $f(j)\in I$ tel que $p_j(E_{f(j)})$ ne soit pas réduit à 0 (dans le cas contraire, l’orthoprojecteur $p_j$ serait nul sur $M_{\pi}(\varrho ))$. On a ainsi défini une application $f$ de J dans I. Pour

$-1$

tout $i\in I$, l’ensemble $f(i)$ est dénombrable. En effet, cet ensemble est contenu dans l’ensemble des $j\in J$ tels que $p_j(E_i)$ est non nul, c’est-à-dire tels que $p_j(x_i)\not = 0$. Or (EVT, V, p. 20, cor. 2), on a

$$
\sum_{j\in J}\|p_j(x_i)\|^2=\|x_i\|^2
$$

donc l’ensemble des $j\in J$ tels que $p_j(x_i)\not = 0$ est dénombrable. D’après E, III, p. 50, prop. 4, on conclut que Card(J) = Card($f(J)$)$\leqslant$ Card(I). En inversant les rôles de I et J, on conclut que Card(I) = Card(J).

#### Corollaire {#ts-v-s1-n11-cor-1 .statement tag=039U}

Soient G un groupe topologique et $\varrho$ une représentation unitaire de G dans un espace hilbertien complexe E. La somme hilbertienne des composantes $\pi$-isotypiques de G pour $\pi \in \widehat{G}$ est la plus grande sous-représentation semi-simple de $\varrho$.

En effet, les composantes $\pi$-isotypiques de G pour $\pi \in \widehat{G}$ sont deux à deux orthogonales (prop. 8, a)), et chacune est semi-simple (prop. 10, a)), donc la somme hilbertienne F des espaces $M_{\pi}(\varrho )$ pour $\pi \in \widehat{G}$ définit une sous-représentation semi-simple de $\varrho$. Comme par ailleurs toute sous-représentation irréductible de $\varrho$ est une sous-représentation d’une composante isotypique de $\varrho$, le corollaire en résulte.

#### Définition 10 {#ts-v-s1-def-10 .statement tag=039V}

Soit G un groupe topologique. Soient $\varrho$ une représentation unitaire de G dans un espace hilbertien complexe E et $\pi$ une représentation unitaire irréductible de G dans un espace hilbertien complexe.

On appelle multiplicité de $\pi$ dans $\varrho$ le cardinal de l’ensemble I pour toute famille $(E_i)_{i\in I}$ de sous-espaces fermés de E stables par G tels que la sous-représentation de $\varrho$ induite dans $E_i$ soit isomorphe à $\pi$ pour tout I et telle que $M_{\pi}(\varrho )$ soit la somme hilbertienne des sous-espaces $E_i$.

Si la multiplicité de $\pi$ dans $\varrho$ est finie, alors elle est égale à la dimension de l’espace Hom$_G(\pi , \varrho )$ (resp. à la dimension de Hom$_G(\varrho , \pi ))$ d’après la formule (1) de V, p. 377 et le corollaire 2 de V, p. 387. Ce n’est pas toujours le cas en général.

#### Remarque {#ts-v-s1-n11-rem-1 .statement tag=039W}

Il est possible qu’une représentation unitaire $\varrho$ soit non nulle mais que toutes les composantes isotypiques de $\varrho$ relatives à toutes les représentations irréductibles de G soient nulles (cf. V, p. 426, remarque).

## EXERCICES {#ts-v-s1-exercises}

See the [exercises for § 1](exercises/s1/).
