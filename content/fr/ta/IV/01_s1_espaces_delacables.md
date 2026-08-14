---
book: ta
book_title: Topologie algébrique
chapter: IV
chapter_title: ESPACES DÉLAÇABLES
section: 1
section_title: Espaces délaçables
lang: fr
source: ta-i-iv-fr
book_pages: A IV.340-A IV.351
pdf_pages: 0356-0367
extraction: native
subsections:
    - "no": 1
      title: Espaces simplement connexes par arcs
      page: 340
      pdf_page: 356
    - "no": 2
      title: Espaces délaçables
      page: 340
      pdf_page: 356
    - "no": 3
      title: Revêtement universel d’un espace délaçable
      page: 342
      pdf_page: 358
    - "no": 4
      title: Exemples
      page: 346
      pdf_page: 362
statements: 20
exercises: 0
content_sha256: dc9fb068a5f23baf7703b844f8c6d79d0abb6cc37ee1c3e39a8d37360e346101
---

## § 1. ESPACES DÉLAÇABLES

### 1. Espaces simplement connexes par arcs

#### Définition 1 {#ta-iv-s1-def-1 .statement tag=0208}

On dit qu’un espace topologique X est simplement connexe par arcs s’il est connexe par arcs et si tout lacet dans X est strictement homotope à un lacet constant.

L’espace vide est simplement connexe par arcs. Pour qu’un espace connexe par arcs X soit simplement connexe par arcs, il faut et il suffit que le groupe $\pi_1(X, x)$ soit réduit à l’élément neutre pour tout point $x$ de X (III, p. 292, prop. 2). Il suffit qu’il en soit ainsi pour un point $x$ de X (loc. cit.).

Tout espace topologique homéotope à un espace simplement connexe par arcs est simplement connexe par arcs. En effet, il est connexe par arcs (III, p. 260) et, en tout point, son groupe de Poincaré est réduit à l’élément neutre (III, p. 296, cor. 2 de la prop. 6). En particulier, un espace topologique homéotope à un point est simplement connexe par arcs.

Un espace topologique simplement connexe par arcs et localement connexe par arcs est simplement connexe (III, p. 309, cor. 2 de la prop. 1).

### 2. Espaces délaçables

#### Définition 2 {#ta-iv-s1-def-2 .statement tag=0209}

On dit qu’un espace topologique B est délaçable s’il est localement connexe par arcs et si tout point $b$ de B possède un voisinage V tel que l’homomorphisme de $\pi_1(V, b)$ dans $\pi_1(B, b)$ déduit de l’injection canonique ait pour image l’élément neutre.

Un espace topologique localement connexe par arcs est délaçable si et seulement si chacune de ses composantes connexes l’est.

Soit B un espace topologique localement connexe par arcs. Supposons que tout point de B possède un voisinage V qui est délaçable. Alors, B est délaçable.

Tout espace topologique localement connexe par arcs et simplement connexe par arcs est délaçable. C’est en particulier le cas d’un espace localement connexe par arcs homéotope à un point.

#### Remarque 1 {#ta-iv-s1-n2-rem-1 .statement tag=020A}

Il existe des espaces topologiques B, connexes et localement connexes par arcs tels que certains points $a$ de B, mais pas tous, possèdent un voisinage V tel que l’homomorphisme de $\pi_1(V, a)$ dans $\pi_1(B, a)$ soit trivial (III, p. 336, exerc. 6).

#### Remarque 2 {#ta-iv-s1-n2-rem-2 .statement tag=020B}

Soit B un espace délaçable ; toute opération du groupoïde $\varpi (B)$ sur un B-espace est sans monodromie locale (cf. III, p. 313, remarque). En particulier, pour qu’une application $p: E\rightarrow B$ fasse de E un revêtement de B, il faut et il suffit qu’elle soit étale, séparée et qu’elle vérifie la propriété de relèvement des chemins (III, p. 315, corollaire 3).

#### Proposition 1 {#ta-iv-s1-prop-1 .statement tag=020C}

L’espace produit d’une famille finie d’espaces délaçables est délaçable.

Il suffit de démontrer que, si A et B sont deux espaces délaçables, il en est de même de leur produit $A\times B$. Sous ces conditions, l’espace $A\times B$ est en effet localement connexe par arcs (III, p. 261, prop. 9). Soit $(a, b)$ un point de $A\times B$. Il existe par hypothèse un voisinage U de $a$ (resp. un voisinage V de $b)$ tels que l’image de l’homomorphisme $i_*:\pi_1(U, a)\rightarrow \pi_1(A, a)$ déduit de l’injection canonique $i: U\rightarrow A$ (resp. de l’homomorphisme $j_*:\pi_1(V, b)\rightarrow \pi_1(B, b)$ déduit de l’injection canonique $j: V\rightarrow B$) soit réduite à l’élément neutre. Alors, $U\times V$ est un voisinage de $(a, b)$ dans $A\times B$. L’homomorphisme $\pi_1(U\times V,(a, b))\rightarrow \pi_1(A\times B,(a, b))$ s’identifie à l’homomorphisme $(i_*, j_*)$ (III, p. 297, corollaire de la prop. 4). Son image est donc réduite à l’élément neutre. Cela prouve que $A\times B$ est délaçable.

#### Proposition 2 {#ta-iv-s1-prop-2 .statement tag=020D}

a) Tout revêtement d’un espace délaçable est délaçable.

b) Inversement, soit $p: E\rightarrow B$ une application étale et surjective et supposons que E soit un espace délaçable. Alors, B est délaçable.

a) Soit B un espace topologique délaçable et soit $(E, p)$ un revêtement de B. L’espace E est alors localement connexe par arcs. Soit $x$ un point de E, notons $b=p(x)$, et soit V un voisinage de $b$ dans B tel que l’homomorphisme canonique $\pi_1(V, b)\rightarrow \pi_1(B, b)$ soit trivial. Notons $i: V\rightarrow B$ et $j:^-p^1(V)\rightarrow E$ les injections canoniques. Par hypothèse, l’image de l’homomorphisme $\pi_1(i, b)$ est réduite à l’élément neutre. Puisque $p\circ i=j\circ p$ et que $\pi_1(p, x)$ est injectif, l’image de l’homomorphisme $\pi_1(j, x)$ est réduite à l’élément neutre. Cela prouve que E est délaçable.

b) L’espace B est localement connexe par arcs. Soit $b$ un point de B et soit $x$ un point de $E_b$. Comme $p$ est étale, il existe un voisinage U de $x$ dans E tel que $p$ induise un homéomorphisme de U sur $p(U)$. Soit V un voisinage de $x$ dans E contenu dans U tel que l’homomorphisme $\pi_1(j, x)$ soit trivial, où $j: V\rightarrow E$ désigne l’injection canonique. Notons $q: V\rightarrow p(V)$ l’application déduite de $p$ par passage aux sous-espaces ; c’est un homéomorphisme. Notons aussi $i$ l’injection canonique de $p(V)$ dans B. On a $p\circ j=i\circ q$, donc $\pi_1(i, b)\circ \pi_1(q, x) =\pi_1(p, x)\circ \pi_1(j, x)$ est l’homomorphisme trivial. Comme l’homomorphisme $\pi_1(q, x)$ est un isomorphisme, l’homomorphisme $\pi_1(i, b)$ est trivial. Il en résulte que l’espace B est délaçable.

#### Proposition 3 {#ta-iv-s1-prop-3 .statement tag=020E}

Soit B un espace topologique délaçable. Soit $(Y, q)$ un revêtement de B et soit $(Z, p)$ un revêtement de Y. L’espace topologique Z, muni de l’application $q\circ p$, est alors un revêtement de B.

En effet, l’application $q\circ p$ est étale ( I, p. 29, prop. 6) et séparée (I, p. 25, prop. 2). D’après la remarque 2 ci-dessus, il suffit donc de montrer qu’elle vérifie la propriété de relèvement des chemins. Soit $z$ un point de Z et soit $c:\mathbf{I}\rightarrow B$ un chemin dans B d’origine $q(p(z))$. Il existe un chemin $c'$ d’origine $p(z)$ dans Y qui relève $c$, car Y est un revêtement de B (III, p. 302, cor. 2). Comme Z est un revêtement de Y, il existe un chemin $c''$ d’origine $z$ dans Z qui relève $c'$; le chemin $c''$ relève $c$. Cela démontre la proposition.

### 3. Revêtement universel d’un espace délaçable

Soit B un espace topologique et soit $b$ un point de B. Rappelons que $\Lambda_b(B)$ désigne le sous-espace de $\mathscr{C}_c(\mathbf{I}; B)$ formé des chemins d’origine $b$, muni de la topologie quotient de la topologie de la convergence compacte. On note $e_B: \Lambda_b(B)\rightarrow$ B l’application qui, à un chemin, associe son terme ; elle est continue. Notons $\lambda_b(B)$ l’espace quotient de $\Lambda_b(B)$ pour la relation d’homotopie stricte et munissons-le de la topologie quotient. Comme deux chemins strictement homotopes ont même terme, l’application $e_B$ définit, par passage au quotient, une application continue $\varepsilon_B:\lambda_b(B)\rightarrow B$, dite application terme.

#### Théorème 1 {#ta-iv-s1-thm-1 .statement tag=020F}

Soit B un espace topologique connexe et localement connexe par arcs et soit $b$ un point de B. Les propriétés suivantes sont équivalentes :

(i) L’espace B est délaçable.

(ii) Il existe un revêtement non vide de B qui est simplement connexe par arcs.

(iii) L’espace $\lambda_b(B)$, muni de l’application terme, $\varepsilon_B:\lambda_b(B)\rightarrow B$, est un revêtement de B.

(iv) Le groupe $\pi_1(B, b)$ est discret pour la topologie admissible.

(v) Le groupe $\pi_1(B, b)$ est discret pour la topologie quotient de la topologie de la convergence compacte.

De plus, lorsque ces conditions sont satisfaites, l’espace $\lambda_b(B)$ est simplement connexe par arcs, simplement connexe, galoisien de groupe $\pi_1(B, b)^{\circ}$, et le revêtement pointé $(\lambda_b(B), \varepsilon_b)$ est un revêtement universel de l’espace pointé $(B, b)$.

Il résulte de la définition d’un espace délaçable que le sous-groupe de $\pi_1(B, b)$ réduit à l’élément neutre est admissible si et seulement si B est délaçable. Cela démontre l’équivalence (i$)\Leftrightarrow ($iv). Par ailleurs, l’équivalence des propriétés (iv) et (v) découle des remarques 4 et 5 de III, p. 320.

(iv$)\Rightarrow ($ii). D’après III, p. 316, prop. 5, il existe un revêtement $(E, p)$ de B et un point $x\in E_b$ tel que $p_*(\pi_1(E, x)) =\{e\}$; en particulier, $\pi_1(E, x)$ est réduit à l’élément neutre. La composante connexe par arcs de $x$ dans E est alors un revêtement non vide de B (I, p. 80, cor. 1 de la prop. 6), simplement connexe par arcs.

(ii$)\Rightarrow ($iii). Soit E un revêtement de B non vide et simplement connexe par arcs. Soit $x$ un point de $E_b$ (il en existe car B est connexe, I, p. 74, prop. 4). La projection $q: E\rightarrow$ B induit un homéomorphisme $\Lambda_x(E)\rightarrow \Lambda_b(B)$ (III, p. 302, cor. 2 de la prop. 3), d’où, par passage aux composantes connexes par arcs, un homéomorphisme $q_*:\lambda_x(E)\simeq \lambda_b(B)$. L’application terme $\Lambda_x(E)\rightarrow E$ est continue et ouverte, car E est localement connexe par arcs (III, p. 264, corollaire). L’application $\varepsilon_E:\lambda_x(E)\rightarrow E$ qu’elle définit par passage aux composantes connexes par arcs est donc continue et ouverte. L’application $\varepsilon_E\circ (q_*)^{-1}:\lambda_b(B)\rightarrow E$ est bijective, continue et ouverte. Cela démontre que l’espace topologique $\lambda_b(B)$, muni de la topologie de la convergence compacte et de l’application terme, est un revêtement de B.

(iii$)\Rightarrow ($v). En effet, l’ensemble $\pi_1(B, b)$, muni de la topologie quotient de la topologie de la convergence compacte s’identifie à la fibre du B-espace $\lambda_b(B)$ de B en la classe du lacet constant en $b$. Si $\lambda_b(B)$ est un revêtement de B, alors $\pi_1(B, b)$ est discret pour la topologie de la convergence compacte.

Supposons que ces assertions soient vérifiées. D’après ce qui précède, l’espace $\lambda_b(B)$ est alors un revêtement de B qui est simplement connexe par arcs, donc simplement connexe. L’espace pointé $(\lambda_b(B), \varepsilon_b)$ est par conséquent un revêtement universel de $(B, b)$ (I, p. 126, corollaire de la prop. 3) et le revêtement $\lambda_b(B)$ est un revêtement galoisien de B (I, p. 120, prop. 1). L’homomorphisme canonique $h_{(\lambda_b(B),\varepsilon_b)}:\pi_1(B, b)\rightarrow$ Aut$_B(\lambda_b(B))$ est alors un isomorphisme (III, p. 306, prop. 5).

#### Remarque 1 {#ta-iv-s1-n3-rem-1 .statement tag=020G}

Soit B un espace délaçable connexe et soit $b$ un point de B. Il résulte du théorème 1, (iv), que toute opération du groupe $\pi_1(B, b)$ est admissible. Par suite, tout $\pi_1(B, b)$-ensemble est isomorphe à un $\pi_1(B, b)$-ensemble $E_b$, où E est un revêtement de B (III, p. 318, prop. 7). Rappelons aussi ( III, p. 310, prop. 2) que si E et $E'$ sont des revêtements de B, l’application $f\mapsto f_b$ induit une bijection de l’ensemble des morphismes de B-espaces de E dans $E'$ sur l’ensemble des morphismes de $\pi_1(B, b)$-ensembles de $E_b$ dans $E'_b$.

*Dans le langage des catégories, on dit que le foncteur qui, à un revêtement E de B, associe la fibre $E_b$ est une équivalence de catégories de la catégorie des revêtements de B dans la catégorie des $\pi_1(B, b)$-ensembles.*

#### Corollaire 1 {#ta-iv-s1-thm-1-cor-1 .statement tag=020H}

Soit B un espace topologique délaçable et soit $b$ un point de B. Soit E un revêtement connexe de B et soit $x$ un point de la fibre $E_b$. Les propriétés suivantes sont équivalentes :

(i) Le groupe $\pi_1(E, x)$ est trivial.

(ii) L’espace E est simplement connexe.

(iii) L’espace pointé $(E, x)$ est un revêtement universel de $(B, b)$.

L’implication (i)$\Rightarrow$(ii) a déjà été démontrée sous la seule hypothèse que l’espace B soit connexe et localement connexe par arcs ( III, p. 309, cor. 2 de la prop. 1) et l’implication (ii)$\Rightarrow$(iii) sans aucune hypothèse (I, p. 126, corollaire).

Démontrons (iii)$\Rightarrow$(i). D’après le théorème 1 de IV, p. 342, il existe un revêtement $E'$ de B et un point $x'$ de la fibre $E'_b$ tel que le groupe $\pi_1(E', x')$ soit réduit à l’élément neutre. Sous l’hypothèse (iii), il existe un B-morphisme pointé $f: (E, x)\rightarrow (E', x')$. Notons $p: E\rightarrow$ B et $p': E'\rightarrow B$ les projections des revêtements E et $E'$; on a $p=p'\circ f$ donc $\pi_1(p, x) =\pi_1(p', x')\circ \pi_1(f, x)$. Comme le groupe $\pi_1(E', x')$ est trivial, l’homomorphisme injectif $\pi_1(p, x)$ a pour image l’élément neutre. Cela prouve que le groupe $\pi_1(E, x)$ est réduit à l’élément neutre.

#### Corollaire 2 {#ta-iv-s1-thm-1-cor-2 .statement tag=020I}

Soit B un espace topologique délaçable et soit $b$ un point de B. Soit $(E, x)$ un revêtement universel de l’espace pointé $(B, b)$. Pour tout revêtement $E'$ de B et tout point $x'$ de $E'_b$, l’unique B-morphisme $f: E\rightarrow E'$ tel que $f(x) =x'$ fait de E un revêtement de $E'$. L’espace pointé $(E, x)$ est alors un revêtement universel de $(E', x')$.

D’après la prop. 7 de I, p. 81, l’espace E, muni de l’application $f$, est un revêtement de $E'$. La dernière assertion résulte alors du corollaire 1.

Soit B un espace topologique délaçable et soient $a,b$ deux points de B. L’espace topologique quotient $\varpi_{a,b}(B)$ est homéomorphe à l’espace $\pi_1(B, a)$, muni de la topologie quotient de la topologie de la convergence compacte (III, p. 293, remarque 3), donc est discret d’après le théorème 1 de IV, p. 342. Par suite, la classe d’homotopie stricte de tout chemin dans B joignant $a$ à $b$ est une partie ouverte de $\Lambda_{a,b}(B)$. Plus généralement :

#### Proposition 4 {#ta-iv-s1-prop-4 .statement tag=020J}

Soit B un espace topologique délaçable. La relation d’homotopie stricte est une relation d’équivalence ouverte dans l’espace topologique $\mathscr{C}_c(\mathbf{I}; B)$.

Supposons d’abord que l’espace B soit simplement connexe par arcs. Notons $\varphi : \Lambda (B)\rightarrow B\times B$ l’application qui, à un chemin $c$ dans B, associe le couple $(c(0), c(1))$ formé de son origine et de son terme. Pour que deux chemins dans B soient strictement homotopes, il faut et il suffit qu’ils aient même origine et même terme (III, p. 292, prop. 2). L’espace B étant connexe et localement connexe par arcs, l’application $\varphi$ est surjective, continue et ouverte (III, p. 262, prop. 10). La relation d’homotopie stricte est donc ouverte (TG, I, p. 32, prop. 3).

Dans le cas général, soit E un revêtement simplement connexe par arcs de B, non vide si B $=\not\emptyset$. Ce revêtement est surjectif car B est connexe (I, p. 74, prop. 4). Notons $p$ la projection du B-espace E et soit $\widetilde{p}: \Lambda (E)\rightarrow \Lambda (B)$ l’application qui, à un chemin $c$ dans E, associe le chemin $p\circ c$. Muni de l’application $\widetilde{p}$, Λ(E) est un revêtement de Λ(B) (III, p. 302, cor. 1 de la prop. 3). Pour que deux chemins dans B soient strictement homotopes, il faut et il suffit qu’ils soient les images par l’application $\widetilde{p}$ de deux chemins strictement homotopes dans E (III, p. 302, prop. 4). Soit U une partie ouverte de l’espace Λ(B). L’ensemble $(^-\widetilde{p}^1)(U)$ est ouvert dans Λ(E) ; d’après la première partie de la

démonstration, l’ensemble $U'$ saturé de $(^-\widetilde{p}^1)(U)$ pour la relation d’homotopie stricte est ouvert dans Λ(E). Comme Λ(E) est un revêtement de Λ(B), l’ensemble $\widetilde{p}(U')$ est ouvert dans Λ(B). Cela prouve la proposition, car $\widetilde{p}(U')$ est le saturé de U pour la relation d’homotopie stricte.

### 4. Exemples

1) Espaces localement contractiles

#### Définition 3 {#ta-iv-s1-def-3 .statement tag=020K}

On dit qu’un espace topologique B est localement contractile si tout point $b$ de B possède un voisinage V tel que l’espace pointé $(V, b)$ soit contractile (III, p. 234, exemple 3).

#### Proposition 5 {#ta-iv-s1-prop-5 .statement tag=020L}

Un espace topologique localement contractile est délaçable.

Soit B un espace localement contractile. Soit $b$ un point de B et soit V un voisinage de $b$ tel que $(V, b)$ soit un espace pointé contractile. L’espace V est homéotope à un point, donc $\pi_1(V, b) =\{\varepsilon_b\}($III, p. 296, corollaire 3).

Pour démontrer la proposition, il reste à démontrer que l’espace B est localement connexe par arcs. Soit $\sigma : V\times \mathbf{I}\rightarrow$ V une homotopie pointée en $b$ reliant l’application constante d’image $b$ à l’application Id$_V$. Pour tout voisinage W de $b$ contenu dans V, l’ensemble $\sigma (W\times \mathbf{I})$ est un voisinage de $b$ car il contient $W =\sigma (W\times  \{1\})$, et il est connexe par arcs car pour tout $(a, s)\in W\times \mathbf{I}$, l’application $t\mapsto \sigma (a, ts)$ est un chemin reliant $b=\sigma (a,0)$ à $\sigma (a, s)$ dans $\sigma (W\times \mathbf{I})$. Démontrons que les ensembles de la forme $\sigma (W\times \mathbf{I})$ forment un système fondamental de voisinages de $b$. Soit $V'$ un voisinage ouvert de $b$ dans B; alors, $^-\sigma^1(V')$ est un voisinage ouvert de $\{b\} \times \mathbf{I}$ dans $V\times \mathbf{I}$. Comme l’espace $\mathbf{I}$ est compact, la projection pr$_1: V\times \mathbf{I}\rightarrow V$ est propre (TG, I, p. 77, cor. 5) et pr$_1(\complement^-\sigma^1(V'))$ est une partie fermée de V ne contenant pas $b$. Son complémentaire W est ainsi un voisinage ouvert de $b$ dans V tel que $W\times \mathbf{I}\subset^-\sigma^1(V')$, d’où $\sigma (W\times \mathbf{I})\subset V'$.

Toute partie ouverte d’un espace numérique ou d’un espace projectif, réel ou complexe, à $n$ dimensions (cf. chapitres VI et VIII) est délaçable, de même que les sphères euclidiennes $\mathbf{S}_n$ (TG, VI, p. 11, prop. 4). Plus généralement, toute variété topologique (VAR R, seconde partie, p. 7, Notations et Conventions) est délaçable. En effet, ces espaces sont localement contractiles.

2) Groupe de Poincaré du cercle. — L’espace topologique $\mathbf{R}$ est homéotope à un point (III, p. 234, exemple 4), donc simplement connexe par arcs (IV, p. 340). La surjection canonique $p$ de $\mathbf{R}$ sur $\mathbf{T}=\mathbf{R}/\mathbf{Z}$ en fait un revêtement principal de groupe $\mathbf{Z}($I, p. 100, exemple 4). L’espace topologique $\mathbf{T}$ est délaçable et $(\mathbf{R},0)$ est un revêtement universel de $(\mathbf{T},0)$. On en déduit un isomorphisme canonique de groupes $\pi_1(\mathbf{T},0)\rightarrow \mathbf{Z}:$ il applique la classe du lacet $t\mapsto p(nt)$ en 0 sur l’élément $n$ de $\mathbf{Z}$. Compte tenu de l’exemple 6 (I, p. 101), on en déduit la proposition suivante.

#### Proposition 6 {#ta-iv-s1-prop-6 .statement tag=020M}

L’application $p:x\mapsto e^{2\pi ix}$ de $\mathbf{R}$ dans $\mathbf{S}_1$ fait de $(\mathbf{R},0)$ un revêtement universel de $(\mathbf{S}_1,1)$. Le groupe $\pi_1(\mathbf{S}_1,1)$ est isomorphe à $\mathbf{Z}$; la classe du lacet $t\mapsto e^{2\pi it}$ en est un générateur. Pour tout entier $n >0$, l’application $z\mapsto z^n$ fait de $\mathbf{S}_1$ un revêtement galoisien de groupe $\mathbf{Z}/n\mathbf{Z}$ de $\mathbf{S}_1$. Tout revêtement connexe et non vide de $\mathbf{S}_1$ est isomorphe à l’un de ces revêtements.

Seule la dernière assertion reste à démontrer. La fibre $E_1$ en 1 d’un revêtement connexe et non vide E de $\mathbf{S}_1$ est munie d’une opération transitive du groupe $\pi_1(§_1,1)$. Puisque les sous-groupes de $\mathbf{Z}$ sont les ensembles $n\mathbf{Z}$, pour $n\geqslant 0$, on constate que $E_1$ est isomorphe à l’un des ensembles homogènes associés aux revêtements décrits précédemment. Comme $\mathbf{S}_1$ est connexe et localement connexe par arcs, E est isomorphe à l’un de ces revêtements.

#### Corollaire {#ta-iv-s1-n4-cor-1 .statement tag=020N}

L’application $z\mapsto e^z$ de $\mathbf{C}$ dans $\mathbf{C}^*$ fait de $(\mathbf{C},0)$ un revêtement universel de $(\mathbf{C}^*,1)$. Le groupe $\pi_1(\mathbf{C}^*,1)$ est isomorphe à $\mathbf{Z}$; la classe du lacet $t\mapsto e^{2\pi it}$ en est un générateur. Pour tout entier $n >0$, l’application $z\mapsto z^n$ fait de $\mathbf{C}^*$ un revêtement galoisien de groupe $\mathbf{Z}/n\mathbf{Z}$ de $\mathbf{C}^*$. Tout revêtement connexe et non vide de $\mathbf{C}^*$ est isomorphe à l’un de ces revêtements.

L’application $z\mapsto (|z|, z/|z|)$ est un homéomorphisme de l’espace $\mathbf{C}^*$ sur l’espace $\mathbf{R}^*_+\times \mathbf{S}^1$ (TG, VI, p. 10, prop. 3) ; en particulier, $\mathbf{C}^*$ est connexe par arcs. Comme l’application $x\mapsto e^x$ de $\mathbf{R}$ dans $\mathbf{R}_+^*$ est un homéomorphisme, il résulte de la proposition 6 que l’application $(x, y)\mapsto e^xe^{2\pi iy}$ fait de $\mathbf{R}^2$ un revêtement de $\mathbf{C}^*$. En identifiant $\mathbf{R}^2$ à $\mathbf{C}$ par l’application $(x, y)\mapsto x+iy$, on en conclut que l’espace $\mathbf{C}$, muni de l’application $z\mapsto e^z$, est un revêtement de $\mathbf{C}^*$. Comme l’espace $\mathbf{C}$ est connexe et simplement connexe par arcs, le revêtement pointé $(\mathbf{C},0)$ est un revêtement universel de l’espace pointé $(\mathbf{C}^*,1)$.

Il découle aussi du corollaire, III, p. 297, que le groupe de Poincaré de $\mathbf{C}^*$ en 1 est isomorphe à $\mathbf{Z}$ et que la classe $\gamma$ du lacet $t\mapsto e^{2\pi it}$ en est un générateur.

Soit $n$ un entier $>0$. L’application $x\mapsto x^n$ de $\mathbf{R}^*_+$ dans lui-même est un homéomorphisme ; on en déduit comme précédemment que l’application $z\mapsto z^n$ fait de $\mathbf{C}^*$ un revêtement de degré $n$ de $\mathbf{C}^*$. Il est galoisien de groupe $\mathbf{Z}/n\mathbf{Z}$. La dernière assertion se démontre comme dans la preuve de la prop. 6.

Pour tout entier $n\geqslant 0$, le tore $(\mathbf{S}_1)^n$ est un espace délaçable (IV, p. 341, prop. 1) et son groupe de Poincaré en tout point est isomorphe à $\mathbf{Z}^n($III, p. 297, prop. 4).

Nous généraliserons ces résultats dans le paragraphe 3 consacré aux revêtements des groupes topologiques.

3) Espaces projectifs réels. — Soit $n$ un entier $>0$. Les espaces $\mathbf{S}_n$ et $\mathbf{P}_n(\mathbf{R})$ sont connexes, non vides et l’application canonique (TG, VI, p. $13)\varphi :\mathbf{S}_n\rightarrow \mathbf{P}_n(\mathbf{R})$ fait de $\mathbf{S}_n$ un revêtement principal de $\mathbf{P}_n(\mathbf{R})$ de groupe $\{+1,-1\}($I, p. 99, exemple 1). Pour $n\geqslant 2$, la sphère $\mathbf{S}_n$ est simplement connexe (I, p. 127, exemple 3) et délaçable, donc simplement connexe par arcs (IV, p. 344, corollaire 1). Pour $n= 1$, l’application $z\mapsto z^2$ de $\mathbf{S}_1$ dans $\mathbf{S}_1$ définit une relation d’équivalence dans $\mathbf{S}_1$ dont les classes sont les couples de points opposés de $\mathbf{S}_1$. L’application $\varphi :\mathbf{S}_1\rightarrow \mathbf{P}_1(\mathbf{R})$ définit par passage au quotient une bijection continue $\psi :\mathbf{S}_1\rightarrow \mathbf{P}_1(\mathbf{R})$ telle que $\psi (z^2) =\varphi (z)$. Comme $\mathbf{S}_1$ est un espace compact, l’application $\psi$ est un homéomorphisme (TG, I, p. 63, cor. 2).

#### Proposition 7 {#ta-iv-s1-prop-7 .statement tag=020O}

L’application $x\mapsto \varphi (e^{2\pi ix})$ de $\mathbf{R}$ sur $\mathbf{P}_1(\mathbf{R})$ fait de $(\mathbf{R},0)$ un revêtement universel de $(\mathbf{P}_1(\mathbf{R}), \varphi (1))$. Soit $c:\mathbf{I}\rightarrow \mathbf{S}_1$ le chemin $t\mapsto e^{\pi it}$; la classe de $\varphi (c)$ est un générateur du groupe $\pi_1(\mathbf{P}_1(\mathbf{R}), \varphi (1))$ qui est isomorphe à $\mathbf{Z}$.

Pour tout entier $n\geqslant$ 2 et tout point $x$ de $\mathbf{S}_n$, l’application canonique $\varphi :\mathbf{S}_n\rightarrow \mathbf{P}_n(\mathbf{R})$ fait de $(\mathbf{S}_n, x)$ un revêtement universel de $(\mathbf{P}_n(\mathbf{R}), \varphi (x))$. Pour tout chemin $c$ dans $\mathbf{S}_n$ reliant $x$ à $-x$, la classe de $\varphi \circ c$ engendre le groupe $\pi_1(\mathbf{P}_n(\mathbf{R}), \varphi (x))$ qui est isomorphe à $\mathbf{Z}/2\mathbf{Z}$.

4) Quotient d’un espace par l’opération propre d’un groupe discret

#### Lemme 1 {#ta-iv-s1-lem-1 .statement tag=020P}

Soit X un espace topologique, soit G un groupe discret opérant proprement dans X et soit $p$ la projection canonique de X sur $X/G$.

Soit $x$ un point de X, soit $K_x$ son fixateur dans G. Soit $U_1$ un voisinage de $x$ dans X ; il existe un voisinage U de $x$ dans X, stable par $K_x$ et contenu dans $U_1$ tel que $g\cdot U\cap U =\emptyset$ si $g\notin K_x$ et tel que l’application canonique $p$ induise un homéomorphisme de $U/K_x$ sur un voisinage V de $p(x)$ dans $X/G$.

D’après la prop. 8 de TG, III, p. 32, il existe un voisinage $U_2$ de $x$ dans X, stable par $K_x$, tel que $g\cdot U_2\cap U_2=\emptyset$ si $g\notin K_x$ et tel que l’application canonique $p$ induise un homéomorphisme de $U_2/K_x$ sur un voisinage de $p(x)$ dans $X/G$.

Comme l’application canonique $U_2\rightarrow U_2/K_x$ est fermée (TG, III, p. 28, prop. 2), il existe un voisinage ouvert U de $x$ contenu dans $U_1\cap U_2$ qui est stable par $K_x($I, p. 75, lemme). La relation d’équivalence dans $U_2$ définie par $K_x$ est aussi ouverte (TG, III, p. 10, lemme 2). Il résulte alors de TG, I, p. 32, prop. 4, que l’application canonique induit un homéomorphisme de $U/K_x$ sur un voisinage ouvert de $p(x)$ dans $X/G$, d’où le lemme.

#### Proposition 8 {#ta-iv-s1-prop-8 .statement tag=020Q}

Soit X un espace topologique et soit G un groupe discret opérant proprement dans X. Notons $p$ la projection canonique de X sur $X/G$.

a) Supposons que X soit connexe par arcs et que le groupe G soit engendré par les fixateurs des points de X. Alors, l’homomorphisme canonique $\pi_1(X, x)\rightarrow \pi_1(X/G, p(x))$ est surjectif pour tout point $x$ de X. En particulier, $X/G$ est simplement connexe par arcs si X l’est.

b) Si l’espace X est délaçable, l’espace $X/G$ est délaçable.

a) L’ensemble N des éléments $g\in G$ pour lesquels il existe un chemin $c_g:\mathbf{I}\rightarrow X$ tel que $c_g(0) =x,c_g(1) =g\cdot x$ et tel que le lacet $p\circ c_g$ dans $X/G$ soit strictement homotope à un lacet constant est un sous-groupe de G. Si $g\in G$ et s’il existe un point $y$ de X tel que $g\cdot y=y$, choisissons un chemin $c:\mathbf{I}\rightarrow X$ reliant $x$ à $y$; alors le chemin $c'=c*$ $(g\cdot c)$ vérifie $c'(0) =x,c'(1) =g\cdot x$ et $[p\circ c'] = [p\circ c][p\circ (g\cdot c)]^{-1}=e_{p(x)}$, donc $p\circ c'$ est strictement homotope à un lacet constant. Comme G est engendré par les fixateurs des points de X, il en résulte que N = G.

Soit $c$ un lacet dans $X/G$ en $p(x)$. D’après le théorème 4 de III, p. 287, il existe un chemin $\widetilde{c}:\mathbf{I}\rightarrow X$ relevant $c$ tel que $\widetilde{c}(0) =x$. Comme $p(\widetilde{c}(1)) =c(1) =p(x)$, il existe $g\in G$ tel que $\widetilde{c}(1) =g\cdot x$. Choisissons un chemin $c_g:\mathbf{I}\rightarrow X$ reliant $x$ à $g\cdot x$ et tel que $p\circ c_g$ soit strictement homotope à un lacet constant. Alors, le chemin $c'=\widetilde{c}*c_g$ est un lacet en $x$ dans X tel que $[p\circ c'] = [c]$. Cela montre que l’homomorphisme $\pi_1(X, x)\rightarrow \pi_1(X/G, p(x))$ est surjectif. L’autre assertion en découle immédiatement.

Démontrons maintenant l’assertion b). L’espace $X/G$ est localement connexe par arcs (III, p. 261, prop. 8).

Soit $x$ un point de X et soit $K_x$ son fixateur dans G. Soit $U_1$ un voisinage ouvert de $x$, contenu dans U, tel que l’image de l’homomorphisme canonique $\pi_1(U_1, x)\rightarrow \pi_1(X, x)$ soit réduite à l’élément neutre. D’après le lemme 1 (IV, p. 349), il existe un voisinage U de $x$ dans X, contenu dans $U_1$, stable par $K_x$, tel que $g\cdot U\cap U =\emptyset$ si $g\notin K_x$ et tel que l’application canonique $p$ induise un homéomorphisme de $U/K_x$ sur un voisinage V de $p(x)$ dans $X/G$.

Soit $c$ un lacet en $x$ dans V ; d’après le théorème 4 (III, p. 287), appliqué à l’espace topologique U et au groupe $K_x$, il existe un chemin $\widetilde{c}:\mathbf{I}\rightarrow U$ tel que $\widetilde{c}(0) =x$ et qui relève $c$. On a nécessairement $\widetilde{c}(1) =x$, si bien que $\widetilde{c}$ est un lacet en $x$ dans U. Par hypothèse, $\widetilde{c}$ est strictement homotope à un lacet constant dans X ; par suite, il en est de même de $c$ et l’homomorphisme canonique $\pi_1(V, p(x))\rightarrow \pi_1(X/G, p(x))$ est trivial. Cela démontre que $X/G$ est délaçable si X l’est.

5) Dans le plan euclidien $\mathbf{R}^2$, soit P l’espace topologique réunion des cercles de centre $(1/n,0)$ passant par l’origine (pour $n\in \mathbf{N}^*)$. L’espace P est compact, connexe et localement connexe par arcs, mais n’est pas délaçable. Le groupe $\pi_1(P,0)$, muni de la topologie admissible, est séparé et non discret (III, p. 337, exerc. 7).

#### Remarque 1 {#ta-iv-s1-n4-rem-1 .statement tag=020R}

Le théorème 4 de III, p. 287 et la prop. 8 (IV, p. 349) restent valables sous l’hypothèse plus générale que G est un groupe de Lie de dimension finie sur $\mathbf{R}$ opérant proprement dans X. Pour plus de détails, cf. D. Montgomery et C. T. Yang, « The existence of a slice », Annals of mathematics 65 (1957), p. 108–116 ; R. Palais, « On the existence of slices for actions of non-compact Lie groups », Annals of mathematics 73 (1961), p. 295–323 ; et G. Bredon, Introduction to compact transformation groups, Academic Press, 1972.
