---
book: ta
book_title: Topologie algébrique
chapter: IV
chapter_title: ESPACES DÉLAÇABLES
section: 3
section_title: Groupes de Poincaré des groupes topologiques
lang: fr
source: ta-i-iv-fr
book_pages: A IV.369-A IV.382, A IV.459-A IV.461
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
content_sha256: 51df0626d16b3013a47fe3c4250f6b85c9b95f0362cf3c12832cd75e24bf6b9e
---

## § 3. GROUPES DE POINCARÉ DES GROUPES TOPOLOGIQUES

### 1. Prolongement des homomorphismes locaux de groupes

#### Définition 1 {#ta-iv-s3-def-1 .statement tag=021M}

Étant donnés un groupe topologique G et un groupe $G'$, on appelle homomorphisme local de G dans $G'$ une application $f$ d’un voisinage V de l’élément neutre de G dans $G'$ telle que, pour tout couple de points $x,y$ de V tels que $xy\in V$, on ait $f(xy) =f(x)f(y)$.

Si $G'$ est un groupe topologique et si $f$ est une application continue, on dit que $f$ est un homomorphisme local continu (ou morphisme local de groupes topologiques).

Si G et $G'$ sont des groupes topologiques, on a défini (TG, III, p. 6, déf. 2) la notion d’isomorphisme local de G à $G'$. Un isomorphisme local de G à $G'$ est un homéomorphisme $f$ d’un voisinage V de l’élément neutre de G sur un voisinage $V'$ de l’élément neutre de $G'$ tel que $f$ et l’application réciproque de $f$ soient des homomorphismes locaux.

#### Proposition 1 {#ta-iv-s3-prop-1 .statement tag=021N}

Soient G et $G'$ des groupes topologiques et soit $p: G\rightarrow G'$ un homomorphisme de groupes. Pour que $p$ fasse de G un revêtement de $G'$, il faut et il suffit que la restriction de $p$ à un voisinage convenable de l’élément neutre de G soit un isomorphisme local de G à $G'$.

La condition est nécessaire d’après la proposition 3 de TG, III, p. 6. Inversement, supposons que $p$ induise un homéomorphisme d’un voisinage ouvert V de l’élément neutre $e$ de G sur un voisinage $V'$ de l’élément neutre de $G'$. L’application $p$ est alors continue (TG, III, p. 15, prop. 23) et ouverte (TG, III, p. 16, prop. 24). L’image H de $p$ est un sous-groupe de $G'$ contenant V, donc ouvert et fermé dans $G'$ (TG, III, p. 7, corollaire). Soit N le noyau de $p$; on a $N\cap V =\{e\}$, donc N est discret (loc. cit., prop. 5). Par suite, $p$ fait de G un revêtement de H, principal de groupe N (I, p. 100, cor. 3 du th. 1). Comme H est ouvert et fermé dans $G'$, le $G'$-espace $(G, p)$ est un revêtement.

#### Proposition 2 {#ta-iv-s3-prop-2 .statement tag=021O}

Soit G un groupe topologique connexe, soit $G'$ un groupe et soit $f: V\rightarrow G'$ un homomorphisme local de G dans $G'$, où V est un voisinage connexe de l’élément neutre de G. Il existe alors un groupe topologique connexe H, un morphisme de groupes topologiques $p: H\rightarrow G$ tel que $(H, p)$ soit un revêtement de G et un homomorphisme de groupes $\varphi : H\rightarrow G'$ tel que l’ensemble des $y\in \overset{-1}{p}(V)$ vérifiant $f(p(y)) =\varphi (y)$ soit un voisinage de l’élément neutre dans H.

Si $G'$ est un groupe topologique et si l’application $f$ est continue, un tel homomorphisme $\varphi$ est continu.

#### Lemme 1 {#ta-iv-s3-lem-1 .statement tag=021P}

Soit G un groupe topologique et soit V un voisinage connexe de l’élément neutre $e$ de G. Pour tout voisinage U de $e$ dans G et tout $x\in V$, il existe un entier $n\in \mathbf{N}$ et des éléments $u_1, . . . , u_n$ dans U tels que $u_1. . . u_n=x$ et $u_1. . . u_k\in V$ pour tout entier $k$ tel que $1\leqslant k\leqslant n$.

On peut supposer que U est ouvert et contenu dans V. Notons A l’ensemble des $x\in V$ satisfaisant la condition du lemme. Si $x\in A$ et si $y\in xU\cap V$, alors $y\in A$, d’où AU $\cap V\subset A$ ; cela montre que A est ouvert dans V. Soit $x\in V$ tel que $xU^{-1}\cap A=\not\emptyset$; on a alors $x\in$ AU$\cap V$, donc $x\in A$. Par conséquent, si $x\in V$ et $x\notin A,xU^{-1}\cap A =\emptyset$ et A est fermé dans V. Comme $e\in A$ et que V est connexe, il en résulte que A = V.

Démontrons maintenant la proposition. Notons $j$ l’application $g\mapsto$ $(g, f(g))$ de V dans $G\times G'$ et soit H le sous-groupe de $G\times G'$ engendré par $j(V)$.

Soit U un voisinage de $e$ dans G, contenu dans V. Soit $x\in V$ ; d’après le lemme 1, il existe $u_1, . . . , u_n\in U$ tels que $x=u_1. . . u_n$ et tels que $u_1. . . u_k\in V$ pour tout entier $k$ tel que $1\leqslant k\leqslant n$. Par récurrence, on a $f(u_1. . . u_k) =f(u_1). . . f(u_k)$ pour tout entier $k,1\leqslant k\leqslant n$. En particulier, $j(x)$ appartient au sous-groupe engendré par $j(U)$. Il en résulte que H est engendré par $j(U)$.

Soit $\mathscr{B}$ l’ensemble des parties de H de la forme $j(U)$, où U est un voisinage de $e$ dans V. Montrons qu’il existe une unique topologie sur H, compatible avec sa structure de groupe, pour laquelle $\mathscr{B}$ est une base du filtre des voisinages de l’élément neutre. Pour cela, il suffit de démontrer que l’ensemble $\mathscr{B}$ satisfait aux conditions (GV$'_I)$, (GV$'_{II})$ et (GV$'_{III})$ de III, p. 4.

Soit donc U un voisinage de $e$ dans G, contenu dans V ; il existe un voisinage $U'$ de $e$ tel que $U'\cdot U'\subset U$. Pour tout couple $x, y$ de points de $U'$, on a $xy\in V$ et $f(xy) =f(x)f(y)$. Par suite, $j(U')\in \mathscr{B}$ et $j(U')\cdot j(U')\subset j(U)$. Cela montre que la condition (GV$'_I)$ est vérifiée.

L’ensemble $U''= V\cap U^{-1}$ est alors un voisinage de $e$ dans V et, pour $x\in U''$, on a $x^{-1}\in U$ et $f(x^{-1}) =f(x)^{-1}$. Par suite, $j(U'')^{-1}\subset j(U)$, ce qui montre la condition (GV$'_{II})$.

Fixons enfin un voisinage U de $e$ dans V tel que $U = U^{-1}$ et $U^3\subset V$. Soit W un voisinage de $e$ dans U et soit $h= (g, f(g))$ un élément de $j(U)$. Il existe un voisinage $W'$ de $e$ contenu dans W tel que $gW'g^{-1}\subset W$. Alors, $j(W')\in \mathscr{B}$ et $hj(W')h^{-1}\subset j(W)$, car on a $f(gxg^{-1}) =f(g)f(x)f(g^{-1})$, pour $x\in W'$.

Soit $h\in H$. Comme U est un voisinage de $e$ contenu dans V$,j(U)$ engendre H ; puisque U est symétrique, il existe des éléments $u_1, . . . , u_n$ dans U tels que $h=j(u_1). . . j(u_n)$. Par récurrence sur $n$, il existe un voisinage $W'$ de $e$ contenu dans W tel que $hj(W')h^{-1}\subset j(W)$. Par suite, la condition (GV$'_{III})$ est vérifiée.

Munissons alors le groupe G de cette topologie.

Notons $p: H\rightarrow$ G la restriction à H de la première projection $G\times G'\rightarrow G$. C’est un homomorphisme de groupes. Pour tout voisinage U de $e$ contenu dans V, l’ensemble $\overset{-1}{p}(U)$ contient le voisinage $j(U)$ de l’élément neutre de H, donc $p$ est un homomorphisme continu de groupes topologiques. Pour tout voisinage U de $e$ contenu dans V, on a $p(j(U)) = U$, donc $p$ est une application ouverte. Comme G est connexe, $p$ est surjective. Son noyau est discret car il ne rencontre $j(V)$ qu’en l’élément neutre. Il résulte alors du corollaire 3 (I, p. 100) que le G-espace $(H, p)$ est un revêtement.

Soit $\varphi$ la restriction à H de la seconde projection $G\times G'\rightarrow G'$. Si $g\in V$, on a $(g, f(g)) =j(g)\in j(V)$ et $\varphi (g, f(g)) =f(g)$, si bien que $\varphi (y) =f(p(y))$ pour $y\in j(V)$.

Supposons de plus que $G'$ soit un groupe topologique et que l’application $f$ soit continue en $e$. Alors, l’homomorphisme $\varphi$ est continu en l’élément neutre de H, donc est continu (TG, III, p. 15, prop. 23).

#### Corollaire 1 {#ta-iv-s3-lem-1-cor-1 .statement tag=021Q}

Soit G un groupe topologique simplement connexe et soit $G'$ un groupe. Soit V un voisinage connexe de l’élément neutre dans G et soit $f: V\rightarrow G'$ un homomorphisme local. Il existe un unique homomorphisme de groupes $h: G\rightarrow G'$ prolongeant $f$. Si $G'$ est un groupe topologique et si l’application $f$ est continue, l’homomorphisme $h$ est continu.

Le groupe G est connexe. Soient H$,\varphi$ et $p$ comme dans la proposition 2. Comme G est simplement connexe, H est un revêtement trivialisable de G (I, p. 124, déf. 3) ; comme H est connexe et non vide, l’application $p$ est un isomorphisme de groupes topologiques. Posons $h=\varphi \circ p^{-1}$; l’application $h$ est un homomorphisme de groupes et il existe un voisinage ouvert U de l’élément neutre $e$ de G contenu dans V tel que $f|U =h|U$. Il résulte du lemme 1 que $f$ et $h$ coïncident sur V. Autrement dit, l’application $h$ prolonge l’application $f$.

Si $G'$ est un groupe topologique et si l’application $f$ est continue, l’homomorphisme $\varphi$ est continu donc $h$ l’est aussi.

Démontrons l’unicité d’un tel prolongement. L’ensemble des points de G où coïncident deux homomorphismes de G dans $G'$ est un sous-groupe de G. Comme le groupe G est connexe, tout sous-groupe de G contenant un voisinage de l’élément neutre est égal à G (TG, III, p. 8, prop. 6). L’unicité de $h$ en résulte.

#### Remarque 1 {#ta-iv-s3-n1-rem-1 .statement tag=021R}

Lorsque $G =\mathbf{R}$, ce corollaire résulte de la proposition 6 de TG, V, p. 3.

#### Corollaire 2 {#ta-iv-s3-lem-1-cor-2 .statement tag=021S}

Deux groupes topologiques localement connexes et simplement connexes qui sont localement isomorphes sont isomorphes.

Soient G et $G'$ des groupes topologiques localement connexes, soient V et $V'$ des voisinages connexes de l’élément neutre de G et de $G'$ respectivement et soit $f: V\rightarrow V'$ un homéomorphisme qui est un isomorphisme local de G à $G'$. D’après le corollaire 1, il existe un unique homomorphisme de groupes continu $\varphi : G\rightarrow G'$ qui prolonge $f$ et un unique homomorphisme de groupes continu $\varphi ': G'\rightarrow$ G qui prolonge $f^{-1}$. Les homomorphismes $\varphi '\circ \varphi$ et Id$_G$ coïncident sur un voisinage de $e$ dans G, donc sont égaux, car G est connexe. De même, $\varphi \circ \varphi '=$ Id$_{G'}$, d’où le corollaire.

#### Corollaire 3 {#ta-iv-s3-lem-1-cor-3 .statement tag=021T}

Soit G un groupe topologique simplement connexe et soit V un voisinage connexe de l’élément neutre de G. On définit une présentation de G en prenant pour ensemble générateur l’ensemble V et pour ensemble $\mathbf{r}$ de relateurs la famille des $xyz^{-1}$, où $(x, y, z)$ parcourt les triplets d’éléments de V tels que $xy=z$.

Soit $F(V,\mathbf{r})$ le groupe quotient du groupe libre F(V) par le plus petit sous-groupe distingué contenant les éléments $xyz^{-1}$, où $(x, y, z)\in V\times$ $V\times V$ et $xy=z$ (A, I, p. 86). Notons $f: V\rightarrow F(V,\mathbf{r})$ et $g: F(V,\mathbf{r})\rightarrow G$ les applications canoniques. Par construction, l’application $f$ est un homomorphisme local de G dans $F(V,\mathbf{r})$. D’après le corollaire 1, il existe un unique homomorphisme de groupes $\overline{f}: G\rightarrow F(V,\mathbf{r})$ prolongeant $f$. Comme le groupe $F(V,\mathbf{r})$ est engendré par $f(V)$, l’homomorphisme $\overline{f}$ est surjectif. Pour $x\in V$, on a $g(\overline{f}(x)) =g(f(x)) =x$; comme V engendre G$,g\circ \overline{f}=$ Id$_G$, ce qui démontre que $\overline{f}$ est injectif. C’est donc un isomorphisme.

### 2. Espaces de Hopf

#### Définition 2 {#ta-iv-s3-def-2 .statement tag=021U}

On appelle espace de Hopf un espace topologique pointé $(X, e)$ muni d’une loi de composition continue $m: X\times X\rightarrow X$ telle que

(i) $m(e, e) =e$;

(ii) il existe des homotopies pointées en $e$ reliant les applications $x\mapsto m(x, e)$ et $x\mapsto m(e, x)$ à l’application Id$_X$.

On exprime parfois les propriétés (i) et (ii) en disant que $e$ est un élément neutre à homotopie près pour la loi de composition $m$.

On notera qu’il peut exister plusieurs éléments neutres à homotopie près pour une loi de composition continue $m$ sur un espace topologique X. Par exemple, pour $X =\mathbf{R}$ et $m(x, y) = (x+y)/2$, tout $x\in \mathbf{R}$ est élément neutre à homotopie près.

#### Exemple 1 {#ta-iv-s3-n2-exa-1 .statement tag=021V}

Soient G un groupe topologique et $m$ sa loi de composition. L’élément neutre $e$ de G est élément neutre à homotopie près et $(G, e)$ est un espace de Hopf.

#### Exemple 2 {#ta-iv-s3-n2-exa-2 .statement tag=021W}

Soient X un espace topologique et $x$ un point de X. Muni de la juxtaposition des lacets en $x$, l’espace pointé $(\Omega_x(X), e_x)$ est un espace de Hopf. En effet, on a d’abord $e_x*e_x=e_x$. D’autre part, soit $\psi :\mathbf{I}\rightarrow \mathbf{I}$ la fonction définie par $\psi (t) = 2t$ pour $0\leqslant t\leqslant \frac{1}{2}$ et $\psi (t) = 1$ pour $\frac{1}{2}\leqslant t\leqslant 1$ (cf. III, p. 291) et soit $\sigma :\mathbf{I}\times \mathbf{I}\rightarrow \mathbf{I}$ une homotopie stricte reliant $\psi$ à Id$_{\mathbf{I}}($III, p. 289, exemple). Alors, pour tout lacet $c\in \Omega_x(X)$, l’application $c\circ \sigma :\mathbf{I}\times \mathbf{I}\rightarrow X$ est une homotopie stricte reliant $c*e_x$ à $c$ dans $\Omega_x(X)$.

Soit $\tau$ l’application $\Omega_x(X)\times \mathbf{I}\rightarrow \Omega_x(X)$ définie par $\tau (c, s)(t) =$ $c\circ \sigma (s, t)$. Démontrons que $\tau$ est continue. D’après la proposition 1 de III, p. 257, il suffit de montrer que l’application $(c, s, t)\mapsto c(\sigma (s, t))$ de $\Omega_x(X)\times \mathbf{I}\times \mathbf{I}$ dans X est continue, soit encore puisque $\mathbf{I}\times \mathbf{I}$ est compact, que l’application $c\mapsto c\circ \sigma$ de $\mathscr{C}_c(\mathbf{I}; X)$ dans $\mathscr{C}_c(\mathbf{I}\times \mathbf{I}; X)$ est continue. Cette dernière assertion résulte alors du lemme, I, p. 132, b). Par suite, l’application $\tau$ est une homotopie reliant l’application $c\mapsto c*e_x$ à l’application identique de $\Omega_x(X)$. On a $\tau (e_x, s)(t) =x$ pour tous $s,t\in \mathbf{I}$, donc $\tau$ est une homotopie pointée en $e_x$. On raisonne de même pour l’application $c\mapsto e_x*c$.

#### Proposition 3 {#ta-iv-s3-prop-3 .statement tag=021X}

Soient $(X, e)$ un espace de Hopf et $m: X\times X\rightarrow X$ sa loi de composition. Pour tous lacets $c,c'$ de X en $e$, on a :

$$
c'*c\sim c*c'\sim m\circ (c, c')
$$

où $\sim$ désigne la relation d’homotopie stricte. La loi de composition du groupe $\pi_1(X, e)$ est l’homomorphisme composé de l’isomorphisme canonique $\pi_1(X, e)\times \pi_1(X, e)\rightarrow \pi_1(X\times X,(e, e))$ (III, p. 297, corollaire) et de l’homomorphisme $\pi_1(m,(e, e))$ de $\pi_1(X\times X,(e, e))$ dans $\pi_1(X, e)$. Le groupe $\pi_1(X, e)$ est commutatif.

Soit $\mu:\pi_1(X, e)\times \pi_1(X, e)\rightarrow \pi_1(X, e)$ l’homomorphisme de groupes composé de l’isomorphisme canonique de $\pi_1(X, e)\times \pi_1(X, e)$ sur $\pi_1(X\times$ $X,(e, e))$ et de l’homomorphisme $\pi_1(m,(e, e))$. Il s’agit de démontrer que l’on a

$$
\mu(\gamma , \gamma ') =\gamma \gamma '=\gamma '\gamma \tag{1}
$$

pour tous $\gamma ,\gamma '\in \pi_1(X, e)$. Compte tenu de la remarque 2 de III, p. 297, on a :

$$
\mu(\gamma , \gamma ') =\mu(\gamma , \varepsilon_e)\mu(\varepsilon_e, \gamma ') =\mu(\varepsilon_e, \gamma ')\mu(\gamma , \varepsilon_e) \tag{2}
$$

Soit $c\in \Omega_e(X)$ un lacet de classe $\gamma$, notons $m_1: X\rightarrow X$ l’application définie par $m_1(x) =m(x, e)$ ; alors, $\mu(\gamma , \varepsilon_e)$ est la classe de $m_1\circ c$. Par définition d’un espace de Hopf, les applications pointées en $e,m_1$ et Id$_X$, ont même classe d’homotopie pointée en $e$. Par suite, les lacets en $e,m_1\circ c$ et $c$ sont strictement homotopes (III, p. 296, cor. 1 de la prop. 3) et l’on a $\mu(\gamma , \varepsilon_e) =\gamma$. On démontre de façon analogue que l’on a $\mu(\varepsilon_e, \gamma ') =\gamma '$. La relation (1) résulte alors de la relation (2).

#### Remarque {#ta-iv-s3-n2-rem-1 .statement tag=021Y}

Soit $(X, e)$ un espace de Hopf. D’après la prop. 3, l’application de composition des classes de chemins, $\pi_1(X, e)\times \pi_1(X, e)\rightarrow$ $\pi_1(X, e)$ est continue si $\pi_1(X, e)$ est muni de la topologie quotient de la topologie de la convergence compacte sur $\Lambda_e(X)$. C’est en effet la composée de l’isomorphisme continu $\pi_1(X, e)\times \pi_1(X, e)\rightarrow \pi_1(X\times X,(e, e))$ (III, p. 298, remarque 3) et de l’application continue $m_*:\pi_1(X\times X,(e, e))\rightarrow$ $\pi_1(X, e)$ (III, p. 294, remarque 1).

### 3. Groupe de Poincaré des groupes topologiques

Si G est un groupe topologique, pour tout $g\in G$, la translation à gauche $x\mapsto gx$ est un homéomorphisme de G sur lui-même (TG, III, p. 2) et elle induit un isomorphisme de $\pi_1(G, e)$ sur $\pi_1(G, g)$.

Soit G un groupe topologique, soit $e$ son élément neutre et notons $G_0$ la composante connexe par arcs de $e$ dans G. Notons R la relation d’équivalence dans G dont les classes d’équivalence sont les composantes connexes par arcs de G et soit $p: G\rightarrow \pi_0(G)$ l’application canonique. Puisque toute translation, à gauche ou à droite, est un homéomorphisme de G, la relation R est compatible à gauche et à droite avec la loi de groupe de G. D’après le th. 2 de A, I, p. 35, le groupe $G_0$ est un sous-groupe distingué de G, le groupe quotient $G/G_0$ est égal à $\pi_0(G)$ muni de la loi de composition quotient de celle de G et l’application $p$ est un homomorphisme de groupes.

On appelle groupe de Poincaré de G, et on note $\pi_1(G)$, le groupe $\pi_1(G, e)$. L’injection canonique de $G_0$ dans G induit un isomorphisme de $\pi_1(G_0)$ sur $\pi_1(G)$ (III, p. 293, remarque 2).

Soit $g$ un élément de G ; la translation à droite $\boldsymbol{\delta }_g:x\mapsto xg$ induit un isomorphisme $(\boldsymbol{\delta }_g)_*:\pi_1(G)\rightarrow \pi_1(G, g)$. Supposons que $g$ appartienne à $G_0$ et soit $b$ un chemin reliant $e$ à $g$. L’application $\sigma : G\times \mathbf{I}\rightarrow G$ définie par $\sigma (x, t) =xb(t)$ est une homotopie reliant Id$_G$ à $\boldsymbol{\delta }_g$. D’après la prop. 3 de III, p. 295, on a donc, pour tout $\alpha \in \pi_1(G)$, $(\boldsymbol{\delta }_g)_*(\alpha ) =$ $\beta^{-1}\alpha \beta$, où $\beta \in \varpi_{e,g}(G)$ est la classe du chemin $b$. Si l’on désigne par $\boldsymbol{\gamma }_g$ la translation à gauche, $x\mapsto gx$, on a de même $(\boldsymbol{\gamma }_g)_*(\alpha ) =\beta^{-1}\alpha \beta$.

Pour tout $g\in G$, l’application Int($g$)$: G\rightarrow G$ induit un automorphisme $\pi_1$(Int($g$)) de $\pi_1(G)$. On définit ainsi une loi d’opération de G sur $\pi_1(G)$. Pour tout $g\in G$, on a $\pi_1$(Int($g$)) $= (\boldsymbol{\gamma }_{g^{-1}})_*\circ (\boldsymbol{\delta }_g)_*$, si bien que le sous-groupe $G_0$ opère trivialement ; il en résulte une loi d’opération de $\pi_0(G)$ sur $\pi_1(G)$. Lorsque G est un groupe commutatif, cette opération est triviale, mais ce n’est pas toujours le cas (IV, p. 459, exerc. 1).

### 4. Revêtements des groupes topologiques

#### Proposition 4 {#ta-iv-s3-prop-4 .statement tag=021Z}

Soit $(X, e)$ un espace de Hopf (IV, p. 373, définition 2) et soit $m: X\times X\rightarrow X$ sa loi de composition. On suppose l’espace X connexe et localement connexe par arcs. Soit $X'$ un revêtement connexe de X ; notons $p$ sa projection et soit $e'$ un point de la fibre $X'_e$.

a) Le revêtement $X'$ est galoisien et le groupe de ses automorphismes est commutatif.

b) Il existe une loi de composition continue $m': X'\times X'\rightarrow X'$ et une seule telle que l’on ait $p\circ m'=m\circ (p, p)$ et $m'(e', e') =e'$. Muni de cette loi de composition, l’espace pointé $(X', e')$ est un espace de Hopf.

c) Munie de la loi de composition induite par $m'$, la fibre $X'_e$ est un groupe d’élément neutre $e'$. L’application de $\pi_1(X, x)$ dans $X'_e$ donnée par $\gamma \mapsto e'\cdot \gamma$ est un homorphisme de groupes surjectif de noyau $p_*(\pi_1(X', e'))$. L’application $g\mapsto g(e')$ est un isomorphisme du groupe Aut$_X(X')$ sur le groupe $X'_e$.

a) Le groupe $\pi_1(X, e)$ est commutatif (prop. 3). Comme le revêtement $X'$ de X est connexe, c’est alors un revêtement galoisien et le groupe Aut$_X(X')$ est isomorphe au groupe quotient $\pi_1(X, e)/p_*(\pi_1(X', e'))$ (III, p. 312, corollaire 4 de la proposition 2) ; ce groupe est commutatif.

b) Notons $q: X'\times X'\rightarrow X$ l’application $m\circ (p, p)$. L’application $m'$ requise est un relèvement continu de $q$ à $X'$ tel que $m'(e', e') =e'$. L’espace $X'\times X'$ est localement connexe par arcs ; il suffit donc, pour démontrer l’existence d’un tel relèvement continu, de vérifier que $q_*(\pi_1(X'\times X',(e', e')))$ est contenu dans $p_*(\pi_1(X', e'))$ (III, p. 308, prop. 1). D’après la prop. 3, l’application $\pi_1(m,(e, e))$ s’identifie à la loi de composition du groupe $\pi_1(X, e)$ lorsqu’on identifie $\pi_1(X\times X,(e, e))$ à $\pi_1(X, e)\times \pi_1(X, e)$. Le groupe $q_*(\pi_1(X'\times X',(e', e')))$ est donc égal au groupe $p_*(\pi_1(X', e'))$, d’où l’existence de $m'$. Comme $X'\times X'$ est connexe, l’unicité de $m'$ résulte de I, p. 34, corollaire 1 de la prop. 11.

Démontrons que l’application $m'$ munit l’espace pointé $(X', e')$ d’une structure d’espace de Hopf. Soit $m_1: X\rightarrow X$ l’application $g\mapsto m(g, e)$ et soit $\sigma_1: X\times \mathbf{I}\rightarrow X$ une homotopie pointée en $x$ reliant $m_1$ à Id$_X$. Posons $\tau =\sigma_1\circ (p$, Id$_{\mathbf{I}}): X'\times \mathbf{I}\rightarrow X$. L’application $m'_1: X'\rightarrow X'$ définie par $h\mapsto m'(h, e')$ relève l’application $\tau (\cdot ,0)$; soit $\tau ': X'\times \mathbf{I}\rightarrow X'$ le relèvement de $\tau$ qui est une homotopie d’origine $m'_1($III, p. 301, prop. 2). L’application $t\mapsto \tau '(e', t)$ est un relèvement à $X'$ de l’application constante $t\mapsto e$; comme $\tau '(e',0) =e'$, on a donc $\tau '(e', t) =e'$ pour tout $t\in \mathbf{I}$. L’application $\tau '(\cdot ,1)$ est alors un relèvement à $X'$ de l’application $p$ qui applique $e'$ sur $e'$. Comme $X'$ est connexe, Id$_{X'}$ est l’unique X-morphisme de $X'$ dans lui-même qui fixe le point $e'$; on a donc $\tau '(\cdot ,1) =$ Id$_{X'}$. Cela montre que $\tau '$ est une homotopie pointée en $e'$ qui relie l’application $m'_1$ à l’application Id$_{X'}$. De même, il existe une homotopie pointée en $e'$ reliant l’application $m'_2:h\mapsto m'(e', h)$ à l’application Id$_{X'}$. Ceci prouve que l’espace pointé $(X', e')$, muni de la loi de composition $m'$, est un espace de Hopf.

c) Comme $X'$ est un revêtement connexe de X, l’application orbitale de $e'$ induite par l’opération de $\pi_1(X, e)$ sur $X'_e$ est surjective et induit une bijection de $\pi_1(X, e)/p_*(\pi_1(X', e'))$ sur $X'_e($III, p. 305, théorème 1).

Soient $c$ et $d$ des lacets de X en $e$, soient $\gamma$ et $\delta \in \pi_1(X, e)$ leurs classes. Soient $c'$ et $d'$ les chemins d’origine $e'$ dans $X'$ qui relèvent $c$ et $d$. On a $e'\cdot \gamma =c'(1)$ et $e'\cdot \delta =d'(1)$ (III, p. 304). D’après la proposition 3 de IV, p. 374, le lacet $m\circ (c, d)$ est strictement homotope au lacet $c*d$; on a donc $e'\cdot (\gamma \delta ) =e'\cdot (m\circ (c, d))$. Or, le chemin $m'\circ (c', d')$ est un relèvement d’origine $e'$ du chemin $m\circ (c, d)$ ; on a donc

$$
e'\cdot (\gamma \delta ) =m'(c'(1), d'(1)) =m'(e'\cdot \gamma , e'\cdot \delta )
$$

L’application $\gamma \mapsto e'\cdot \gamma$ est donc un homomorphisme de $\pi_1(X, e)$ dans l’ensemble $X'_e$ muni de la loi de composition induite par $m'$. Par suite, $X'_e$ est un groupe pour la loi de composition induite par $m'$ et l’application orbitale de $e'$ est un isomorphisme du groupe quotient sur $\pi_1(X, e)/p_*(\pi_1(X', e'))$ sur $X'_e$.

La dernière partie de l’assertion c) résulte alors du corollaire 3 de III, p. 311.

#### Proposition 5 {#ta-iv-s3-prop-5 .statement tag=0220}

Conservons les notations et les hypothèses de la proposition 4.

a) Si $m$ est une loi de composition associative ( resp. commutative), il en est de même de $m'$.

b) Si $e$ est élément neutre à droite ( resp. à gauche) pour la loi $m$, alors $e'$ est élément neutre à droite ( resp. à gauche) pour la loi $m'$.

c) Si X est un groupe topologique, $m$ sa loi de composition et $e$ son élément neutre, la loi de composition $m'$ munit $X'$ d’une structure de groupe compatible avec la topologie de $X'$ dont $e'$ est l’élément neutre. L’application $p: X'\rightarrow X$ est un homomorphisme de groupes dont le noyau est discret et contenu dans le centre de $X'$.

a) Supposons que la loi $m$ est associative. Alors les applications de $X'\times X'\times X'$ dans X qui appliquent $(h_1, h_2, h_3)$ sur $m(p(h_1), m(p(h_2), p(h_3)))$ et $m(m(p(h_1), p(h_2)), p(h_3))$ respectivement sont égales. Les applications $(h_1, h_2, h_3)\mapsto m'(h_1, m'(h_2, h_3))$ et $(h_1, h_2, h_3)\mapsto m'(m'(h_1, h_2), h_3)$ de $X'\times X'\times X'$ dans $X'$ en sont des relèvements continus qui coïncident au point $(e', e', e')$. Comme $X'\times X'\times X'$ est connexe, elles sont égales (I, p. 34, cor. 1 de la prop. 11), ce qui montre que la loi $m'$ est associative.

Supposons maintenant la loi $m$ commutative ; les applications $(h_1, h_2)\mapsto m'(h_1, h_2)$ et $(h_1, h_2)\mapsto m'(h_2, h_1)$ sont des relèvements continus à $X'$ de l’application $(h_1, h_2)\mapsto m(p(h_1), p(h_2))$ qui coïn-cident au point $(e', e')$. Comme $X'\times X'$ est connexe, elles sont égales (loc. cit.) et la loi $m'$ est commutative.

Si $e$ est élément neutre à droite (resp. à gauche) pour la loi $m$, l’application $h\mapsto m'(h, e')$ (resp. $h\mapsto m'(e', h)$) de $X'$ dans $X'$ est un X-morphisme de revêtements qui coïncide avec Id$_{X'}$ au point $e'$, donc en tout point de $X'$, puisque $X'$ est connexe (loc. cit.), d’où b).

Démontrons enfin c). Supposons que X soit un groupe topologique. D’après ce qui précède, la loi $m'$ est associative et $e'$ en est un élément neutre. Notons $i: X\rightarrow X$ l’application $g\mapsto g^{-1}$. Elle est continue (TG, III, p. 1) et l’homomorphisme $\pi_1(i, e):\pi_1(X, e)\rightarrow \pi_1(X, e)$ n’est autre que l’application $\gamma \mapsto \gamma^{-1}($IV, p. 374, prop. 3). Par suite, le sous-groupe $(i\circ p)_*(\pi_1(X', e'))$ est égal à $p_*(\pi_1(X', e'))$. D’après la prop. 1 de III, p. 308, il existe donc une application continue $i': X'\rightarrow X'$ telle que $p\circ i'=i\circ p$ et $i'(e') =e'$. Les applications $h\mapsto m'(h, i'(h))$ et $h\mapsto$ $m'(i'(h), h)$ de $X'$ dans $X'$ sont des relèvements à $X'$ de l’application constante d’image $e$ de $X'$ dans X. Elles sont donc constantes et leur image est $e'=m'(e', e')$. Ainsi, tout élément $h$ de $X'$ est inversible, d’inverse $i'(h)$, ce qui montre que $X'$, muni de la loi de composition $m'$, est un groupe. Par construction de la loi $m'$, l’application $p: X'\rightarrow X$ est un homomorphisme de groupes. Comme les applications $m'$ et $i'$ sont continues, la structure de groupe de $X'$ est compatible avec sa topologie (TG, III, p. 1). La fibre $\overset{-1}{p}(e)$ est un sous-groupe discret de $X'$ qui est contenu dans le centre de $X'($I, p. 100, cor. 3) et X est isomorphe au groupe topologique quotient $X'/\overset{-1}{p}(e)$.

#### Corollaire {#ta-iv-s3-n4-cor-1 .statement tag=0221}

Soit G un groupe topologique connexe et localement connexe par arcs. Soit $G'$ un revêtement connexe de G, soit $p$ sa projection et soit $e'$ un élément de la fibre N de l’élément neutre $e$ de G. Munissons $G'$ de l’unique loi de composition continue $m': G'\times G'\rightarrow G'$ telle que $p\circ m'=m\circ (p, p)$ et $m'(e', e') =e'$. Si $i: N\rightarrow G'$ désigne l’injection canonique, $(G', p, i)$ est une extension centrale de G par N (A, I, p. 63).

### 5. Revêtement universel d’un groupe topologique délaçable

Soit G un groupe topologique localement connexe par arcs. Les translations de G sont des homéomorphismes (TG, III, p. 2). Pour que l’espace G soit délaçable (IV, p. 340, déf. 2), il faut et il suffit que G possède la propriété suivante :

Il existe un voisinage V de l’élément neutre $e$ de G tel que l’image de l’homomorphisme de $\pi_1(V, e)$ dans $\pi_1(G, e)$ déduit de l’injection canonique soit réduite à l’élément neutre.

#### Proposition 6 {#ta-iv-s3-prop-6 .statement tag=0222}

Soit G un groupe topologique connexe et délaçable. Il existe un groupe topologique $\widetilde{G}$, d’élément neutre $\widetilde{e}$, et un homomorphisme continu $p:\widetilde{G}\rightarrow G$ qui vérifie les assertions suivantes :

a) L’espace $\widetilde{G}$ est simplement connexe et simplement connexe par arcs. Muni de l’application $p$, l’espace pointé $(\widetilde{G},\widetilde{e})$ est un revêtement universel de l’espace pointé $(G, e)$.

b) Le noyau N de $p$ est un sous-groupe discret de $\widetilde{G}$, contenu dans le centre de $\widetilde{G}$. L’homomorphisme $N\rightarrow$ Aut$_G(\widetilde{G})$ qui, à $n\in N$, associe la translation à droite dans $\widetilde{G}$, est un isomorphisme de groupes. L’homomorphisme de $\pi_1(G)$ dans N qui, à $\gamma \in \pi_1(G)$, associe l’unique élément $n$ de N tel que $\widetilde{e}\cdot \gamma =n$, est un isomorphisme de groupes.

c) Si $G'$ est un groupe topologique, d’élément neutre $e'$ et si $p': G'\rightarrow$ G est un homomorphisme de groupes qui fait de $G'$ un revêtement de G, l’unique application continue $u:\widetilde{G}\rightarrow G'$ telle que $u(\widetilde{e}) =e'$ et $p'\circ u=p$ est un homomorphisme de groupes. Muni de l’application $u,(\widetilde{G},\widetilde{e})$ est un revêtement universel de $(G', e')$.

D’après IV, p. 342, théorème 1, il existe un revêtement $(\widetilde{G}, p)$ de G, simplement connexe et simplement connexe par arcs, galoisien de groupe $\pi_1(G)^{\circ}$, et un point $\widetilde{e}$ de $\overset{-1}{p}(e)$ tel que le revêtement pointé $(\widetilde{G},\widetilde{e})$ soit un revêtement universel de $(G, e)$.

D’après IV, p. 375, prop. 4 et IV, p. 377, prop. 5, il existe sur l’espace $\widetilde{G}$ une unique structure de groupe compatible avec sa topologie pour laquelle $p$ soit un homomorphisme de groupes et $\widetilde{e}$ un élément neutre. Il résulte de la prop. 4 que le groupe $\widetilde{G}$ vérifie les assertions a) et b).

Démontrons l’assertion c). Soit $G'$ un groupe topologique et soit $p': G'\rightarrow G$ un homomorphisme de groupes qui fait de $G'$ un revêtement de G. Soit $e'$ l’élément neutre de $G'$. L’existence et l’unicité d’une application $u:\widetilde{G}\rightarrow G'$ telle que $p=p'\circ u$ et $u(\widetilde{e}) =e'$ résultent de ce que $(\widetilde{G},\widetilde{e})$ est un revêtement universel de l’espace pointé $(G, e)$. Comme les applications $p$ et $p'$ sont des homomorphismes de groupes surjectifs, $u$ est un homomorphisme de groupes. Muni de l’application $u,\widetilde{G}$ est un revêtement de $G'($I, p. 81, prop. 7), donc $(\widetilde{G},\widetilde{e})$ est un revêtement universel de $(G', e')$ (IV, p. 345, cor. 2 du th. 1).

Sous les hypothèses de la proposition, on dira, par abus, que $\widetilde{G}$ est un revêtement universel de G.

#### Exemple {#ta-iv-s3-n5-exa-1 .statement tag=0223}

La proposition 6 s’applique notamment lorsque G est un groupe de Lie connexe sur $\mathbf{R}$ ou $\mathbf{C}$. Il existe alors sur $\widetilde{G}$ une unique structure de variété analytique telle que la projection $p:\widetilde{G}\rightarrow G$ soit un morphisme étale de variétés analytiques (VAR R, §1, 5.8.2, p. 48). Pour cette structure de variété, $\widetilde{G}$ est un groupe de Lie (LIE, III, p. 113, corollaire).

#### Scholie {#ta-iv-s3-n5-sch-1 .statement tag=0224}

Soit G un groupe topologique connexe et délaçable, soit $e$ son élément neutre. Soit $\widetilde{G}$ un groupe topologique simplement connexe par arcs, d’élément neutre $\widetilde{e}$, et $p:\widetilde{G}\rightarrow G$ un homomorphisme de groupes qui fait de $\widetilde{G}$ un revêtement universel de G. Notons N le noyau de $p$.

La translation à droite $\boldsymbol{\delta }_h$ (resp. à gauche) par un élément $h\in N$ est un G-automorphisme du revêtement principal $\widetilde{G}$ et l’application $h\mapsto \boldsymbol{\delta }_h$ est un isomorphisme du groupe N sur le groupe des automorphismes de ce revêtement principal.

Pour tout sous-groupe K de N, l’application $p':\widetilde{G}/K\rightarrow$ G déduite de $p$ est un revêtement galoisien de G, et Aut$_G(G/K)$ s’identifie au groupe $N/K$. Lorsqu’on identifie comme ci-dessus les groupes N et $\pi_1(G)$, le groupe $p'_*(\pi_1(\widetilde{G}/K))$ s’identifie au sous-groupe K de N. En outre, $\widetilde{G}$ est un revêtement de $\widetilde{G}/K$, car G est localement connexe (I, p. 81, prop. 7).

Inversement, tout revêtement connexe non vide E de G est G-isomorphe à un revêtement de ce type (I, p. 113, th. 3 et I, p. 111, prop. 10). Considérons en effet un point $x$ de la fibre $E_e$ et soit $f$ l’unique homomorphisme de $\widetilde{G}$ dans E qui applique $\widetilde{e}$ sur $x$. Muni de $f,\widetilde{G}$ est un revêtement galoisien de E ; le sous-groupe Aut$_E(\widetilde{G})$ de Aut$_G(\widetilde{G})$ s’identifie à $f^{-1}(x)$ qui est donc un sous-groupe de N. Par suite, $f$ induit un G-isomorphisme de $\widetilde{G}/f^{-1}(x)$ sur E. Par transport de structure, il en résulte une structure de groupe topologique sur E pour laquelle $x$ est élément neutre et pour laquelle l’application $f$ est un homomorphisme surjectif. La projection du G-espace E est alors un homomorphisme de groupes et la loi de composition de E est donc la loi de composition définie par la prop. 4 de IV, p. 375.

Soient $(E, q)$ et $(E', q')$ des revêtements connexes de G, soient $x$ un point de $E_e$ et $x'$ un point de $E'_e$. Pour qu’il existe un G-morphisme de E dans $E'$, il faut et il suffit que $p_*(\pi_1(E, x))$ soit contenu dans $p'_*(\pi_1(E', x'))$. Si cette condition est satisfaite, il existe alors un unique G-morphisme $f: E\rightarrow E'$ tel que $g(x) =x'($III, p. 311, cor. 2 de la prop. 1). Si l’on munit E et $E'$ des lois de composition de groupes pour lesquelles $q$ et $q'$ sont des homomorphismes et $x$ et $x'$ des éléments neutres, l’application $g$ est un homomorphisme de groupes. En effet, $g$ s’identifie à l’homomorphisme canonique $\widetilde{G}/p_*(\pi_1(E, x))\rightarrow$ $\widetilde{G}/p'_*(\pi_1(E', x'))$.

#### Proposition 7 {#ta-iv-s3-prop-7 .statement tag=0225}

Pour que deux groupes topologiques connexes et délaçables soient localement isomorphes, il faut et il suffit que leurs revêtements universels soient des groupes topologiques isomorphes.

Un groupe topologique connexe et délaçable est localement isomorphe à son revêtement universel (IV, p. 369, prop. 1) ; la condition est donc suffisante. Elle est nécessaire d’après le corollaire 2 de la proposition 2 (IV, p. 372), car le revêtement universel d’un groupe topologique connexe et délaçable est simplement connexe (IV, p. 379, prop. 6).

#### Proposition 8 {#ta-iv-s3-prop-8 .statement tag=0226}

Soit G un groupe topologique connexe et délaçable et soit $\widetilde{G}$ un revêtement universel de G. Soit V un voisinage ouvert connexe de l’élément neutre $e$ de G tel que l’image de l’homomorphisme canonique de $\pi_1(V\cdot V, e)$ dans $\pi_1(G, e)$ soit réduite à l’élément neutre. Notons $F(V,\mathbf{r})$ le groupe défini par l’ensemble générateur V et par l’ensemble $\mathbf{r}$ des relateurs $xyz^{-1}$, où $(x, y, z)$ parcourt l’ensemble des éléments de $V\times V\times V$ tels que $xy=z$. Notons $j: V\rightarrow F(V,\mathbf{r})$ l’application canonique.

Il existe un unique isomorphisme $f$ du groupe $F(V,\mathbf{r})$ sur $\widetilde{G}$ tel que $f\circ j$ soit un relèvement à $\widetilde{G}$ de l’injection canonique de V dans G.

L’ensemble $V\cdot V$ est connexe et ouvert, donc localement connexe par arcs. Soit $p$ la projection de $\widetilde{G}$. Il existe une section continue $s$ de $p$ au-dessus de $V\cdot V$ telle que $s(e) =\widetilde{e}$, où $\widetilde{e}$ désigne l’élément neutre de $\widetilde{G}($III, p. 308, prop. 1). Posons $\widetilde{V} =s(V)$ ; l’ensemble $\widetilde{V}$ est un voisinage ouvert connexe de $\widetilde{e}$ dans $\widetilde{G}$ et $s$ est un homéomorphisme de $V\cdot V$ sur $\widetilde{V}\cdot \widetilde{V}$. Les applications $(x, y)\mapsto s(x)s(y)$ et $(x, y)\mapsto s(xy)$ sont des relèvements à $\widetilde{G}$ de l’application $(x, y)\mapsto xy$ de $V\times V$ dans G qui coïncident en $(e, e)$ ; comme $V\times V$ est connexe, elles coïncident sur $V\times V$ (I, p. 34, cor. 1). En outre, si $(\widetilde{x},\widetilde{y},\widetilde{z})\in \widetilde{V}\times \widetilde{V}\times \widetilde{V}$, les conditions $\widetilde{x}\widetilde{y}=\widetilde{z}$ et $p(\widetilde{x})p(\widetilde{y}) =p(\widetilde{z})$ sont équivalentes. L’existence d’un isomorphisme $f: F(V,\mathbf{r})\rightarrow \widetilde{G}$ résulte alors du corollaire 3 (IV, p. 372) de la proposition 2.

Soit $g$ un isomorphisme de $F(V,\mathbf{r})$ vérifiant les conditions de la proposition. L’égalité $e\cdot e=e$ entraîne que $eee^{-1}\in \mathbf{r}$, si bien que $j(e)$ est l’élément neutre de $F(V,\mathbf{r})$. Comme V est connexe, $g\circ j$ est l’unique relèvement continu à $\widetilde{G}$ de l’injection canonique de V dans G. Par suite, $f$ et $g$ coïncident sur $j(V)$. Comme $j(V)$ engendre le groupe $F(V,\mathbf{r})$, $f=g$.

## EXERCICES {#ta-iv-s3-exercises}

See the [exercises for § 3](exercises/s3/).
