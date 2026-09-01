---
book: top
book_title: General Topology
chapter: IX
chapter_title: UTILISATION DES NOMBRES RÉELS EN TOPOLOGIE GÉNÉRALE
section: 5
section_title: Espaces de Baire
lang: fr
source: top-v-x-fr
book_pages: TG IX.52-TG IX.56, TG IX.111-TG IX.117
pdf_pages: 0172-0176, 0231-0237
extraction: ocr
subsections:
    - "no": 1
      title: Ensembles rares
      page: 52
      pdf_page: 172
    - "no": 2
      title: Ensembles maigres
      page: 53
      pdf_page: 173
    - "no": 3
      title: Espaces de Baire
      page: 54
      pdf_page: 174
    - "no": 4
      title: Fonctions semi-continues dans un espace de Baire
      page: 56
      pdf_page: 176
statements: 16
exercises: 7
content_sha256: e7f058030e9aa60229969b035e57617e41f974b7ae322db51d27e3faca3689ba
---

## § 5. ESPACES DE BAIRE

### 1. Ensembles rares

#### Définition 1 {#top-ix-s5-def-1 .statement}

On dit qu’une partie $A$ d’un espace topologique $X$ est rare si son adhérence n’a pas de point intérieur.

Il revient au même de dire que l’extérieur de $A$ est partout dense dans $X$.
Pour qu’un ensemble fermé $A$ soit rare, il faut et il suffit qu’il n’ait pas de point intérieur, ou, ce qui revient au même, qu’il soit identique à sa frontière. Pour qu’un ensemble quelconque soit rare, il faut et il suffit que son adhérence soit rare. Toute partie d’un ensemble rare est un ensemble rare.

#### Exemple 1 {#top-ix-s5-n1-exa-1 .statement}

La partie vide de $X$ est un ensemble rare. Dans un espace séparé, pour qu’un ensemble réduit à un point soit rare, il faut et il suffit que ce point ne soit pas isolé dans $X$. Un ensemble partout dense dans un espace non vide n’est jamais rare.
2) La frontière d’un ensemble fermé, ou d’un ensemble ouvert, est toujours un ensemble rare.
3) Dans l’espace numérique $\mathbf{R}^n$, toute variété linéaire affine de dimension $p < n$ est un ensemble rare (VI, p. 4, prop. 2).

#### Remarque {#top-ix-s5-n1-rem-1 .statement}

La frontière d’un ensemble quelconque n’est pas nécessairement un ensemble rare; par exemple, si $A$ et $\complement A$ sont tous deux partout denses, la frontière de $A$ est identique à l’espace $X$ tout entier.

#### Proposition 1 {#top-ix-s5-prop-1 .statement}

La réunion d’une famille localement finie d’ensembles rares est un ensemble rare.

La famille des adhérences des ensembles d’une famille localement finie étant localement finie, on peut se borner à prouver que si $(A_\alpha)$ est une famille localement finie d’ensembles fermés rares, l’intersection des ouverts $\complement A_\alpha$ est un ouvert partout dense. Or, pour tout $x \in X$, il y a un voisinage ouvert $U$ de $x$ ne rencontrant qu’un nombre fini d’ensembles $A_{\alpha_k}$ ($1 \leq k \leq n$). Prouvons par récurrence sur $h$ que l’intersection de $U$ et des $\complement A_{\alpha_k}$ pour $k \leq h$ est un ouvert non vide : il suffit de remarquer que $\complement A_{\alpha_n}$ est partout dense, donc son intersection avec l’ouvert non vide intersection de $U$ et des $\complement A_{\alpha_k}$ pour $1 \leq k \leq h - 1$ n’est pas vide.

Soit $Y$ un sous-espace de l’espace topologique $X$. Une partie $A$ de $Y$ est dite rare relativement à $Y$ si $A$ est un ensemble rare quand on le considère comme partie de l’espace topologique $Y$.

#### Proposition 2 {#top-ix-s5-prop-2 .statement}

*Soient $Y$ un sous-espace de $X$, et $A$ une partie de $Y$; si $A$ est rare relativement à $Y$, $A$ est rare relativement à $X$. Inversement, si $Y$ est ouvert dans $X$, et si $A$ est rare relativement à $X$, il est rare relativement à $Y$.*

Supposons $A$ rare relativement à $Y$; si l’adhérence $\overline{A}$ de $A$ relativement à $X$ contenait un ensemble ouvert non vide $U$, $U \cap A$ ne serait pas vide (par définition de l’adhérence), donc $U \cap Y$ serait un ensemble ouvert non vide par rapport à $Y$, et serait contenu dans l’adhérence $\overline{A} \cap Y$ de $A$ par rapport à $Y$, contrairement à l’hypothèse.

Supposons maintenant que $Y$ soit ouvert dans $X$, et que $A \subset Y$ soit rare relativement à $X$; si $U$ est un ensemble ouvert relativement à $Y$ et non vide, $U$ est ouvert relativement à $X$, donc contient un ensemble non vide $V$ ouvert par rapport à $X$ (et a fortiori par rapport à $Y$) et ne rencontrant pas $A$, ce qui montre que $A$ est rare relativement à $Y$.

La seconde partie de la prop. 2 est évidemment inexacte lorsque $Y$ n’est pas ouvert dans $X$: il suffit pour le voir de considérer le cas où $Y \neq \varnothing$ est rare relativement à $X$, et $A = Y$.

### 2. Ensembles maigres

#### Définition 2 {#top-ix-s5-def-2 .statement}

*On dit qu’une partie $A$ d’un espace topologique $X$ est maigre si elle est réunion d’une famille dénombrable d’ensembles rares.*

Il revient au même de dire que $A$ est contenu dans une réunion dénombrable d’ensembles fermés sans point intérieur.

Un ensemble maigre peut fort bien être *partout dense* dans $X$; l’espace $X$ tout entier peut même être un ensemble maigre.

Un exemple de ce dernier fait est fourni par tout espace séparé $X$ *dénombrable* et *sans point isolé*; la droite rationnelle $\mathbf{Q}$ est un espace de cette nature. Un espace topologique $X$ qui est un ensemble maigre dans $X$ n’est d’ailleurs pas nécessairement dénombrable (voir IX, p. 113, exerc. 9).

Toute partie d’un ensemble maigre dans un espace $X$ est un ensemble maigre; la réunion d’une famille *dénombrable* d’ensembles maigres est un ensemble maigre.

Soit Y un sous-espace de X ; on dit qu’une partie A de Y est maigre relativement à Y si A est un ensemble maigre quand on le considère comme partie de l’espace topologique Y. Il résulte de la prop. 2 de IX, p. 53 que si A est une partie de Y qui est maigre relativement à Y, A est maigre relativement à X ; si en outre Y est ouvert dans X, toute partie A de Y qui est maigre relativement à X est maigre relativement à Y.

### 3. Espaces de Baire

#### Définition 3 {#top-ix-s5-def-3 .statement}

On dit qu’un espace topologique X est un espace de Baire si l’une des deux conditions suivantes (qui sont équivalentes) est remplie :
(EB) Toute intersection dénombrable d’ensembles ouverts partout denses dans X est partout dense dans X.
(EB') Toute réunion dénombrable d’ensembles fermés sans point intérieur dans X est sans point intérieur dans X.

L’axiome (EB) peut encore s’énoncer sous deux autres formes équivalentes :
(EB'') Tout ensemble ouvert non vide dans X est non maigre.
En effet, pour qu’un ensemble soit maigre, il faut et il suffit qu’il soit contenu dans une réunion dénombrable d’ensembles fermés sans point intérieur.
(EB''') Le complémentaire d’un ensemble maigre dans X est partout dense.
Cela signifie en effet qu’aucun ensemble maigre ne peut contenir d’ensemble ouvert non vide, et est donc équivalent à (EB''').

#### Proposition 3 {#top-ix-s5-prop-3 .statement}

Tout sous-espace ouvert Y d’un espace de Baire X est un espace de Baire.

Cela résulte de (EB'') puisque tout ensemble ouvert (resp. maigre) dans Y est ouvert (resp. maigre) dans X.

D’après cette proposition, tout point d’un espace de Baire admet un système fondamental de voisinages dont chacun est un espace de Baire. Réciproquement :

#### Proposition 4 {#top-ix-s5-prop-4 .statement}

Si tout point d’un espace topologique X possède un voisinage qui est un espace de Baire, X est un espace de Baire.

En effet, soient A un ensemble ouvert non vide dans X, x un point de A, V un voisinage ouvert de x qui soit un espace de Baire ; si A était maigre dans X, V ∩ A serait maigre dans V et ouvert dans V, contrairement à l’hypothèse.

#### Proposition 5 {#top-ix-s5-prop-5 .statement}

Dans un espace de Baire X, le complémentaire d’un ensemble maigre est un espace de Baire.

En effet, soit A un ensemble maigre dans X ; son complémentaire Y = C A par rapport à X est partout dense dans X. Soit B un ensemble maigre relativement à Y ; B est aussi maigre relativement à X, donc A ∪ B est maigre relativement à X. Le complémentaire de A ∪ B relativement à X, qui est aussi le complémentaire de B relativement à Y, est donc partout dense dans X, et a fortiori dans Y, ce qui démontre la proposition.

#### Théorème 1 (Baire) {#top-ix-s5-thm-1 .statement}

1° Tout espace localement compact X est un espace de Baire.
    2° Tout espace topologique X sur lequel existe une distance, compatible avec la topologie de X, et définissant sur X une structure d’espace métrique complet, est un espace de Baire.

Nous allons montrer que dans chacun des deux cas l’axiome (EB) est vérifié. Soit (A_n) une suite d’ensembles ouverts partout denses dans X, et soit G un ensemble ouvert non vide quelconque. On peut définir par récurrence une suite (G_n) d’ensembles ouverts non vides tels que G_1 = G et G_{n+1} \subset G_n \cap A_n; en effet, G_n n’étant pas vide par hypothèse, G_n \cap A_n est un ensemble ouvert non vide; comme X est régulier dans les deux cas envisagés, il existe un ensemble ouvert non vide G_{n+1} tel que \overline{G}_{n+1} \subset G_n \cap A_n. Cela étant l’ensemble $G \cap \bigcap_{n=1}^{\infty} A_n$ contient l’intersection des G_n, et cette dernière est identique à l’intersection des \overline{G}_n; tout revient à montrer que les ensembles \overline{G}_n ont une intersection non vide. Or, lorsque X est localement compact, on peut supposer \overline{G}_2 compact; dans l’espace compact \overline{G}_2, les \overline{G}_n (n \geq 2) forment une suite décroissante d’ensembles fermés non vides, et ont donc au moins un point commun d’après l’axiome (C''). Lorsque X est un espace métrique complet (pour une distance compatible avec sa topologie), on peut supposer \overline{G}_n choisi de sorte que son diamètre (relatif à cette distance) tende vers 0 lorsque n croît indéfiniment; les \overline{G}_n forment alors une base de filtre de Cauchy qui converge vers un point appartenant nécessairement à leur intersection.

#### Remarque {#top-ix-s5-n3-rem-1 .statement}

Il y a des espaces de Baire qui ne rentrent dans aucune des deux catégories précédentes, en particulier des espaces de Baire qui ne sont ni métrisables, ni localement compacts (IX, p. 113, exerc. 15); il y a aussi des espaces de Baire métrisables, mais pour lesquels il n’existe aucune structure d’espace métrique complet compatible avec leur topologie (IX, p. 113, exerc. 13).

#### Proposition 6 {#top-ix-s5-prop-6 .statement}

Soient G un groupe localement compact dénombrable à l’infini, M un espace de Baire séparé. Supposons que G opère à gauche continûment et transitivement dans M. Pour tout x \in M, soit H_x le stabilisateur de x dans G, de sorte que l’application s \mapsto s.x de G dans M définit par passage au quotient une bijection continue $\varphi_x : G/H_x \to M$ (III, p. 12). Alors $\varphi_x$ est un homéomorphisme de G/H_x sur M (autrement dit (III, p. 12), M est un espace homogène topologique de G).

Soit x_0 \in M. Il suffit de prouver (III, p. 12, prop. 15) que l’application s \mapsto s.x_0 transforme tout voisinage V de l’élément neutre dans G en un voisinage de x_0 dans M. Soit W un voisinage compact symétrique de e dans G tel que W^2 \subset V. Par hypothèse, G est réunion d’une suite d’ensembles compacts, donc d’une suite de translatés (s_nW) de W, tout compact pouvant être recouvert par un nombre fini de tels ensembles. Alors M est réunion de la suite des ensembles s_n W . x_0, qui sont compacts (donc fermés dans M) puisque M est séparé et s \mapsto s . x_0 continue. Comme M est un espace de Baire, il existe un indice n tel que s_n W . x_0 admette un point intérieur s_n w . x_0 avec w \in W. Par suite x_0 est point intérieur de

$$
w^{-1} s_n^{-1} . (s_n W . x_0) = w^{-1} W . x_0 \subset V . x_0
$$

(III, p. 9, lemme 1) de sorte que V . x_0 est un voisinage de x_0 dans M.

#### Corollaire {#top-ix-s5-n3-cor-1 .statement}

Soient G un groupe localement compact dénombrable à l’infini, G’ un groupe topologique séparé dont l’espace sous-jacent est un espace de Baire, f : G \to G’ un homomorphisme continu surjectif. Alors f est un morphisme strict surjectif (autrement dit, si H est le noyau de f, la bijection continue G/H \to G’ déduite de f est un isomorphisme de groupes topologiques).

En effet, on peut considérer G’ comme un espace où G opère continûment et transitivement par la loi (s, t’) \mapsto f(s)t’, et le stabilisateur de l’élément neutre e’ de G pour cette loi est H; il suffit donc d’appliquer la prop. 6.

### 4. Fonctions semi-continues dans un espace de Baire

#### Théorème 2 {#top-ix-s5-thm-2 .statement}

Soit X un espace de Baire, et soit (f_\alpha) une famille de fonctions numériques semi-continues inférieurement dans X, telles qu’en tout point x \in X, l’enveloppe supérieure \sup_\alpha f_\alpha(x) soit finie. Dans ces conditions, tout ensemble ouvert non vide contient un sous-ensemble ouvert non vide dans lequel la famille (f_\alpha) est uniformément majorée.

On peut encore énoncer le théorème en disant que l’ensemble des points au voisinage desquels la famille (f_\alpha) est uniformément majorée est un ensemble ouvert partout dense.

Soit f = \sup_\alpha f_\alpha l’enveloppe supérieure de la famille (f_\alpha); la fonction f est semi-continue inférieurement (IV, p. 30, th. 4) et finie en tout point de X. Il suffit donc de faire la démonstration lorsque la famille (f_\alpha) se réduit à une seule fonction f. Soit A_n l’ensemble des points x \in X tels que f(x) \leq n; A_n est fermé (IV, p. 29, prop. 1) et l’hypothèse entraîne que X est réunion des A_n, donc l’un au moins des A_n a un point intérieur, ce qui montre qu’il existe un ensemble ouvert non vide dans lequel f est majoré (par un entier n). Si on applique ce résultat à un sous-espace ouvert non vide quelconque de X (sous-espace qui est un espace de Baire d’après la prop. 3 de IX, p. 54), on obtient le théorème.

Les applications les plus fréquentes de ce théorème se rapportent au cas où les f_\alpha sont continues dans X.

#### Remarque {#top-ix-s5-n4-rem-1 .statement}

La conclusion du théorème peut être inexacte lorsqu’on ne suppose pas que X soit un espace de Baire. Par exemple, si pour tout nombre rationnel irréductible p/q, on pose f(p/q) = q, on définit sur la droite rationnelle \mathbf{Q} une fonction semi-continue inférieurement et finie en tout point (cf. IV, p. 29); mais il n’existe aucun ensemble ouvert non vide de \mathbf{Q} dans lequel f soit majorée.

## EXERCICES {#top-ix-s5-exercises}

See the [exercises for § 5](exercises/s5/).
