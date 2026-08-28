---
book: top
book_title: General Topology
chapter: III
chapter_title: GROUPES TOPOLOGIQUES
section: 2
section_title: Sous-groupes; groupes quotients; homomorphismes; espaces homogènes; groupes produits
lang: fr
source: top-i-iv-fr
book_pages: TG III.6-TG III.19, TG III.67-TG III.72
pdf_pages: 0189-0202, 0250-0255
extraction: ocr
subsections:
    - "no": 1
      title: Sous-groupes d’un groupe topologique
      page: 6
      pdf_page: 189
    - "no": 2
      title: Composantes connexes d’un groupe topologique
      page: 8
      pdf_page: 191
    - "no": 3
      title: Sous-groupes partout denses
      page: 9
      pdf_page: 192
    - "no": 4
      title: Espaces à opérateurs
      page: 9
      pdf_page: 192
    - "no": 5
      title: Espaces homogènes
      page: 11
      pdf_page: 194
    - "no": 6
      title: Groupes quotients
      page: 13
      pdf_page: 196
    - "no": 7
      title: Sous-groupes et groupes quotients d’un groupe quotient
      page: 14
      pdf_page: 197
    - "no": 8
      title: Homomorphismes continus et morphismes stricts
      page: 15
      pdf_page: 198
    - "no": 9
      title: Produit de groupes topologiques
      page: 17
      pdf_page: 200
    - "no": 10
      title: Produits semi-directs de groupes topologiques
      page: 18
      pdf_page: 201
statements: 44
exercises: 31
content_sha256: 53dcee520db44f494dfad065c5f0a848807b61ba005df7a20c2e488bf6829ce6
---

## § 2. SOUS-GROUPES; GROUPES QUOTIENTS; HOMOMORPHISMES; ESPACES HOMOGÈNES; GROUPES PRODUITS

### 1. Sous-groupes d’un groupe topologique

Soient $G$ un groupe topologique, $H$ un sous-groupe de $G$. D’après (GT’), la topologie induite sur $H$ par celle de $G$ est compatible avec la structure de groupe de $H$; la structure de *groupe topologique* ainsi définie sur $H$ est dite *induite* par celle de G. Sauf mention expresse du contraire, quand on considérera un sous-groupe H de G comme un groupe topologique, c’est toujours de cette structure induite qu’il s’agira.

#### Proposition 1 {#top-iii-s2-prop-1 .statement}

L’adhérence $\overline{H}$ d’un sous-groupe H d’un groupe topologique G est un sous-groupe de G. Si H est un sous-groupe distingué, $\overline{H}$ est aussi un sous-groupe distingué.

En effet, si a et b sont adhérents à H, $ab^{-1}$ est adhérent à H, puisque l’application $(x, y) \mapsto xy^{-1}$ est continue dans $G \times G$, et transforme $H \times H$ en H (I, p. 9, th. 1). De la même manière, en vertu de la continuité de l’application $x \mapsto axa^{-1}$, on voit que si H est un sous-groupe distingué, il en est de même de $\overline{H}$.

En particulier, l’adhérence N de l’ensemble $\{e\}$ réduit à l’élément neutre de G, est un sous-groupe distingué de G; pour qu’il se réduise à e, il faut et il suffit (III, p. 5, prop. 2) que G soit séparé.

#### Proposition 2 {#top-iii-s2-prop-2 .statement}

Dans un groupe séparé G, l’adhérence d’un sous-groupe commutatif H est un sous-groupe commutatif.

On peut se borner au cas où H est partout dense dans G, en vertu de la prop. 1; les fonctions continues $xy$ et $yx$, étant égales dans $H \times H$, le sont alors aussi dans $G \times G$, en vertu du principe de prolongement des identités (I, p. 53, cor. 1).

#### Proposition 3 {#top-iii-s2-prop-3 .statement}

Dans un groupe séparé G, l’ensemble M’ des éléments permutables aux éléments d’une partie quelconque M de G est un sous-groupe fermé. En particulier, le centre de G est fermé dans G.

En effet, M’ est l’intersection des ensembles $F_m$ des $x \in G$ tels que $xm = mx$, lorsque m parcourt M; la proposition résulte de ce que les $F_m$ sont fermés (I, p. 53, prop. 2).

#### Proposition 4 {#top-iii-s2-prop-4 .statement}

Dans un groupe topologique G, tout sous-groupe H localement fermé en un point (I, p. 20, déf. 2) est fermé.

Par translation, H est localement fermé en chacun de ses points, autrement dit H est localement fermé dans G. Soit V un voisinage ouvert symétrique de e dans G tel que $V \cap H$ soit fermé dans V. Si $x \in \overline{H}$, on a $xV \cap H \neq \varnothing$; si $y \in xV \cap H$, on a $x \in yV$, et $y(V \cap H) = (yV) \cap H$ est fermé dans $yV$; comme x est adhérent à $(yV) \cap H$, on a bien $x \in H$.

#### Corollaire {#top-iii-s2-n1-cor-1 .statement}

Dans un groupe topologique, pour qu’un sous-groupe soit ouvert, il faut et il suffit qu’il ait un point intérieur. Tout sous-groupe ouvert est fermé.

La première partie est immédiate, car si un sous-groupe H a un point intérieur, on voit par translation que tous ses points sont intérieurs. La seconde assertion est un cas particulier de la prop. 4.

#### Proposition 5 {#top-iii-s2-prop-5 .statement}

Dans un groupe topologique G, pour qu’un sous-groupe H soit discret, il faut et il suffit qu’il ait un point isolé. Tout sous-groupe discret d’un groupe séparé est fermé.

Si H a un point isolé, on voit par translation que tous ses points sont isolés, donc H est discret. La seconde assertion est un cas particulier de la prop. 4, car si G est séparé, {e} est fermé dans G et a fortiori dans tout voisinage de e.

#### Remarque {#top-iii-s2-n1-rem-1 .statement}

Soit H un sous-groupe quelconque d’un groupe topologique G. Pour tout $x \in \overline{H}$, on a $x\overline{H} = x.\overline{H} = \overline{H}$, puisque les translations sont des homéomorphismes de G sur lui-même. Autrement dit, pour tout $x \in \overline{H}$, $xH$ est dense dans $\overline{H}$. On en conclut que si H n’est pas fermé, $\overline{H} \cap GH$ est dense dans $\overline{H}$.

### 2. Composantes connexes d’un groupe topologique

Soit V un voisinage symétrique de e dans G; le sous-groupe engendré par V, qu’on note $V^\infty$ est formé, comme on sait, de tous les composés $\prod_{i=1}^n x_i$ de suites finies d’éléments de V; $V^\infty$ est ouvert, puisque e lui est intérieur; il est donc fermé d’après la prop. 4 de III, p. 7. On en conclut que:
Proposition 6. — Tout groupe connexe est engendré par chacun des voisinages de l’élément neutre.

La réciproque de cette proposition est inexacte en général, comme nous le verrons dans IV, p. 8. Si un groupe topologique G est engendré par chacun des voisinages de l’élément neutre, on peut seulement dire qu’il ne contient aucun sous-groupe ouvert distinct de G.

*Comme exemple de groupe G non connexe, contenant un sous-groupe ouvert distinct de G, citons le groupe multiplicatif $\mathbf{R}^*$ des nombres réels $\neq 0$, dans lequel le sous-groupe $\mathbf{R}_+^*$ des nombres $> 0$ est à la fois ouvert et fermé (voir IV, p. 12).*

#### Proposition 7 {#top-iii-s2-prop-7 .statement}

Soient G un groupe topologique, M une partie de G contenant l’élément neutre e, H le sous-groupe de G engendré par M. Si M est connexe, H est connexe.

Soit $M'$ l’ensemble $M \cup M^{-1}$; il est connexe, puisque $M^{-1}$, image de M par l’application continue $x \mapsto x^{-1}$, est connexe (I, p. 82, prop. 4); comme M et $M^{-1}$ contiennent e, $M'$ est connexe (I, p. 81, prop. 2). Les groupe H est alors réunion des ensembles ${M'}^n$ pour les entiers $n \geqslant 1$ (A, I, p. 32, prop. 2 et p. 7, prop. 2); or ${M'}^n$ est l’image de la partie $M' \times M' \times \cdots \times M'$ (n fois) de $G \times G \times \cdots \times G$ par l’application continue $(x_1, x_2, \ldots, x_n) \mapsto x_1 x_2 \ldots x_n$; donc ${M'}^n$ est connexe (I, p. 83, prop. 8, et p. 82, prop. 4); comme e appartient à tous les ${M'}^n$, H est connexe (I, p. 81, prop. 2).

#### Corollaire {#top-iii-s2-n2-cor-1 .statement}

Le groupe des commutateurs d’un groupe topologique connexe est connexe.

En effet, l’ensemble C des commutateurs est l’image de $G \times G$ par l’application continue $(x, y) \mapsto xyx^{-1}y^{-1}$, donc est connexe (I, p. 83, prop. 8 et p. 82, prop. 4); comme C contient évidemment e et engendre le groupe des commutateurs, cela prouve le corollaire.

#### Proposition 8 {#top-iii-s2-prop-8 .statement}

Dans un groupe topologique G, la composante connexe K de l’élément neutre $e$ est un sous-groupe distingué fermé; la composante connexe d’un point $x$ est la classe $x.K = K.x$.

En effet, si $a \in K$, $a^{-1}K$ est connexe et contient $e$; donc on a $K^{-1}K \subset K$, ce qui prouve que $K$ est un sous-groupe de $G$; ce sous-groupe est invariant par tout automorphisme de $G$, en particulier par tout automorphisme intérieur, donc $K$ est *distingué*; on sait en outre que $K$ est fermé (I, p. 84, prop. 9). Enfin, la translation à gauche $y \mapsto xy$ étant un homéomorphisme de $G$ qui transforme $e$ en $x$, la composante connexe de $x$ est $x.K$.

On dit que la composante connexe de l’élément neutre $e$ de $G$ est la *composante neutre* de $G$.

### 3. Sous-groupes partout denses

La proposition suivante généralise la prop. 1 de III, p. 7 et la prop. 6 de III, p. 8:

#### Proposition 9 {#top-iii-s2-prop-9 .statement}

(i) *Soit $H$ un sous-groupe partout dense d’un groupe topologique $G$; si $K$ est un sous-groupe distingué de $H$, l’adhérence $\overline{K}$ de $K$ dans $G$ est un sous-groupe distingué de $G$.*

(ii) *Soit $H$ un sous-groupe partout dense d’un groupe topologique $G$; si $H$ est engendré par chacun des voisinages de l’élément neutre dans $H$, $G$ est engendré par chacun des voisinages de l’élément neutre dans $G$.*

(i) L’application $(z, x) \mapsto zxz^{-1}$ est continue dans $G \times G$, et applique $H \times K$ dans $K$; donc (I, p. 9, th. 1), elle applique $G \times \overline{K} = \overline{H} \times \overline{K}$ dans $\overline{K}$.

(ii) Soit $V$ un voisinage symétrique quelconque de $e$ dans $G$; $V \cap H$ est un voisinage de l’élément neutre dans $H$, donc engendre $H$; par suite, $V$ engendre un sous-groupe $H'$ contenant $H$; mais $H'$ est ouvert et fermé (III, p. 7, corollaire), donc contient $\overline{H} = G$.

### 4. Espaces à opérateurs

Soient $E$ un espace topologique, $G$ un groupe topologique. On dit que $G$ *opère continûment* dans $E$ si les conditions suivantes sont vérifiées:
1° $G$ opère sur $E$, autrement dit (A, I, p. 50) $E$ est muni d’une loi de composition externe $(s, x) \mapsto s.x$ dont $G$ est l’ensemble d’opérateurs, et qui est telle que $s.(t.x) = (st).x$ et $e.x = x$ pour $s, t$ dans $G$ et $x \in E$.
2° L’application $(s, x) \mapsto s.x$ de $G \times E$ dans $E$ est *continue*.

#### Lemme 1 {#top-iii-s2-lem-1 .statement}

*Si un groupe topologique $G$ opère continûment dans un espace topologique $E$, alors, pour tout $s \in G$, l’application $x \mapsto s.x$ est un homéomorphisme de $E$ sur lui-même.*

En effet, cette application est une bijection continue dont la bijection réciproque $x \mapsto s^{-1}.x$ est aussi continue.

Rappelons (A, I, p. 54) que, pour tout $x \in E$, l’ensemble $G.x$ des transformés $s.x$ de $x$ par les éléments $s \in G$ est appelé l’orbite de $x$ (pour le groupe d’opérateurs $G$) ; l’ensemble des $s \in G$ tels que $s.x = x$ est un sous-groupe de $G$, appelé stabilisateur de $x$ (A, I, p. 52). La relation $R \{x, y\} : « y$ appartient à l’orbite de $x$ » est une relation d’équivalence dans $E$, dite définie par $G$; les classes d’équivalence pour cette relation sont les orbites des points de $E$. L’espace topologique $E/R$ est appelé l’espace des orbites du groupe $G$ dans $E$, ou encore l’espace quotient de $E$ par le groupe $G$, et on le note $E/G$; on dit aussi que la topologie de $E/G$ est la topologie quotient de celle de $E$ par $G$.

#### Lemme 2 {#top-iii-s2-lem-2 .statement}

Si un groupe topologique $G$ opère continûment dans un espace topologique $E$, la relation d’équivalence $R$ définie par $G$ est ouverte.

En effet, le saturé pour $R$ d’une partie ouverte $U$ de $E$ est l’ensemble $\bigcup_{s \in G} s.U$, et chacun des $s.U$ est ouvert (lemme 1).

#### Exemple 1 {#top-iii-s2-n4-exa-1 .statement}

Soit $H$ un sous-groupe d’un groupe topologique $G$; $H$ opère continûment dans $G$ par la loi externe $(s, x) \mapsto sx$. Il opère aussi continûment dans $G$ par la loi externe $(s, x) \mapsto sxs^{-1}$.

#### Exemple 2 {#top-iii-s2-n4-exa-2 .statement}

*Si $K$ est un corps topologique (III, p. 54), le groupe multiplicatif $K^*$ opère continûment dans $K$ par la loi externe $(s, x) \mapsto sx.*$

#### Exemple 3 {#top-iii-s2-n4-exa-3 .statement}

Soient $G$ un groupe topologique, $E$ un espace topologique; l’application $(s, x) \mapsto x$ de $G \times E$ dans $E$ est une loi externe sur $E$ et $G$ opère continûment dans $E$ pour cette loi; on dit alors que $G$ opère trivialement dans $E$.

#### Remarque {#top-iii-s2-n4-rem-1 .statement}

Au lieu de dire qu’un groupe topologique $G$ opère continûment dans un espace topologique $E$, on dit aussi parfois que $G$ opère continûment à gauche dans $E$. Lorsque le groupe topologique $G^0$ opposé à $G$ opère continûment dans $E$, on dit que $G$ opère continûment à droite dans $E$; il revient au même de dire que $E$ est muni d’une loi de composition externe continue $(s, x) \mapsto s.x$ ayant $G$ comme ensemble d’opérateurs et telle que $s.(t.x) = (ts).x$ et $e.x = x$. On note souvent une telle loi à droite: $(s, x) \mapsto x.s$ (d’où la terminologie), et on a alors $(x.t).s = x.(ts)$. Lorsque $G$ opère continûment à droite dans $E$ par la loi $(s, x) \mapsto x.s$, il opère aussi continûment à gauche dans $E$ par la nouvelle loi externe $(s, x) \mapsto x.s^{-1}$ en vertu de l’axiome (GTII).

Soient $E$ (resp. $E'$) un ensemble dans lequel opère un groupe $G$ (resp. $G'$), $f$ un homomorphisme de $G$ dans $G'$, $g$ une application de $E$ dans $E'$. On dit que $f$ et $g$ sont compatibles si l’on a $g(s.x) = f(s).g(x)$ pour tout $s \in G$ et tout $x \in E$. Si $E''$ est un troisième ensemble où opère un groupe $G''$, $f'$ un homomorphisme de $G'$ dans $G''$, $g'$ une application de $E'$ dans $E''$, et si $f'$ et $g'$ sont compatibles, alors $f' \circ f$ et $g' \circ g$ sont compatibles. Lorsque $E, E'$ sont des espaces topologiques, $G, G'$ des groupes topologiques opérant continûment dans $E, E'$ respectivement, on dit que $(f, g)$ est un morphisme de l’espace à opérateurs $E$ dans l’espace à opérateurs $E'$ lorsque $f$ et $g$ sont continues et compatibles. Par passage aux quotients, $g$ définit alors une application continue de $E/G$ dans $E'/G'$ (I, p. 21, corollaire).

Soient G un groupe topologique opérant continûment dans un espace topologique E, φ l’application canonique de E sur l’espace des orbites E/G. Soient A une partie quelconque de E, A’ le sous-espace de E saturé pour la relation d’équivalence R définie par G (réunion des orbites des points de A; on dit aussi que A’ est le saturé de A par G); G opère continûment dans A’ par la restriction de (s, x) ↦ s.x à G × A’. En outre, comme R est ouverte (lemme 2) et A’ saturé, la prop. 4 de I, p. 32, et la relation φ(A) = φ(A’), entraînent:

#### Proposition 10 {#top-iii-s2-prop-10 .statement}

*La bijection canonique du sous-espace φ(A) de E/G sur l’espace des orbites A’/G est un homéomorphisme.*

Soit maintenant S une relation d’équivalence dans E telle que, pour tout s ∈ G, l’application x ↦ s.x soit *compatible avec S* (autrement dit, telle que la relation x ≡ y (mod. S) entraîne s.x ≡ s.y (mod. S)); nous dirons pour abréger que la relation S est *compatible avec le groupe* G. Si ψ est l’application canonique de E sur E/S, et si on désigne par s.ψ(x) la classe mod. S de s.x, le groupe G opère dans l’espace E/S par (s, ψ(x)) ↦ s.ψ(x) = ψ(s.x). En outre:

#### Proposition 11 {#top-iii-s2-prop-11 .statement}

*Si la relation d’équivalence S dans E est ouverte et compatible avec G, G opère continûment dans E/S.*

Comme la relation d’égalité (resp. la relation S) est ouverte dans G (resp. dans E), tout revient à démontrer que l’application (s, x) ↦ s.ψ(x) = ψ(s.x) de G × E dans E/S est continue (I, p. 34, cor. de la prop. 8); or cela résulte du fait que ψ et (s, x) ↦ s.x sont continues.

#### Remarque {#top-iii-s2-n4-rem-2 .statement}

Soit G’ un second groupe topologique opérant continûment dans E, et supposons que l’on ait s.(s’.x) = s’.(s.x) quels que soient s ∈ G, s’ ∈ G’, x ∈ E; alors la relation d’équivalence S définie par G’ est compatible avec G, et comme elle est ouverte (III, p. 10, lemme 2), on voit que G opère continûment dans E/G’; de même, G’ opère alors continûment dans E/G. On dit dans ce cas que les deux groupes G, G’ opèrent dans E de manières *permutables*.

### 5. Espaces homogènes

Soient G un groupe topologique, H un sous-groupe de G. Le groupe H opère continûment à droite dans G par la loi externe (t, x) ↦ xt, l’orbite d’un point x ∈ G étant la classe à gauche xH suivant H. L’ensemble des orbites est donc ce que nous avons appelé en algèbre (A, I, p. 56) l’ensemble *homogène* G/H. Quand nous parlerons de G/H comme d’un espace topologique, il s’agira toujours, sauf mention expresse du contraire, de l’espace des orbites de G (pour H), autrement dit de l’espace quotient de G par la relation d’équivalence x^{-1}y ∈ H. Conformément aux définitions générales, nous dirons que la topologie de cet espace est la topologie *quotient de celle de G par* H et G/H, muni de sa topologie, sera appelé *espace homogène* des classes à gauche suivant H.

#### Proposition 12 {#top-iii-s2-prop-12 .statement}

Le groupe G opère continûment dans tout espace homogène G/H.

Comme la relation d’équivalence $x^{-1}y \in H$ est ouverte (III, p. 10, lemme 2), cet énoncé est un cas particulier de la prop. 11 de III, p. 11.

#### Proposition 13 {#top-iii-s2-prop-13 .statement}

Soient G un groupe topologique, H un sous-groupe de G. Pour que l’espace homogène G/H soit séparé, il faut et il suffit que H soit fermé dans G.

La condition est nécessaire, H étant une classe d’équivalence suivant la relation $x^{-1}y \in H$; inversement, si H est fermé, le graphe de cette relation est fermé dans $G \times G$, étant l’image réciproque de H par l’application continue $(x, y) \mapsto x^{-1}y$. Comme la relation d’équivalence $x^{-1}y \in H$ est ouverte, G/H est séparé (I, p. 55, prop. 8).

#### Proposition 14 {#top-iii-s2-prop-14 .statement}

Soient G un groupe topologique, H un sous-groupe de G. Pour que l’espace homogène G/H soit discret, il faut et il suffit que H soit ouvert dans G.

En effet, les images réciproques dans G des points de G/H par l’application canonique sont les classes $xH$ ($x \in G$); pour que ces ensembles soient ouverts dans G, il faut et il suffit que H soit ouvert dans G.

Soit E un espace topologique non vide dans lequel un groupe topologique G opère continûment et transitivement; E est alors (au sens algébrique) un G-ensemble homogène (A, I, p. 56). Soient $x$ un point de E, $H_x$ son stabilisateur. La surjection continue $s \mapsto s.x$ de G sur E se factorise canoniquement en

$$
G \xrightarrow{f_x} G/H_x \xrightarrow{g_x} E
$$

où $f_x$ est l’application canonique de G sur l’espace homogène $G/H_x$, et $g_x$ la bijection $s.H_x \mapsto s.x$ de $G/H_x$ sur E; on sait en outre (I, p. 21, prop. 6) que $g_x$ est une application continue. Mais $g_x$ n’est pas nécessairement un homéomorphisme de $G/H_x$ sur E (III, p. 72, exerc. 29). Lorsque, pour tout $x \in E$, $g_x$ est un homéomorphisme, on dit que E est un espace homogène topologique (correspondant au groupe topologique G); pour cela, il est nécessaire et suffisant que, pour tout $x \in E$, l’application $s \mapsto s.x$ de G dans E soit ouverte.

#### Proposition 15 {#top-iii-s2-prop-15 .statement}

Pour qu’un espace topologique E, dans lequel un groupe topologique G opère continûment et transitivement, soit un espace homogène topologique (relativement à G), il suffit que, pour un point $x_0 \in E$, l’application $s \mapsto s.x_0$ transforme tout voisinage de e dans G en un voisinage de $x_0$ dans E.

En effet, tout $x \in E$ s’écrit $x = t.x_0$ pour un $t \in G$; si V est un voisinage de e, $V.x = (Vt).x_0$ est un voisinage de $x$, car on peut écrire $(Vt).x_0 = t.((t^{-1}Vt).x_0)$ et la conclusion résulte de ce que $t^{-1}Vt$ est un voisinage de e dans G, et $y \mapsto t.y$ un homéomorphisme de E sur lui-même (III, p. 9, lemme 1). On en déduit que pour tout ensemble ouvert U dans G, et tout $x \in E$, $U.x$ est ouvert dans E; en effet, pour tout $t \in U$, $t^{-1}U$ est un voisinage de e, donc $(t^{-1}U).x$ est un voisinage de $x$, et $t.((t^{-1}U).x) = U.x$ est un voisinage de $t.x$, d’où notre assertion, qui achève de démontrer la proposition.

### 6. Groupes quotients

#### Proposition 16 {#top-iii-s2-prop-16 .statement}

Soient $G$ un groupe topologique, $H$ un sous-groupe distingué de $G$. La topologie quotient de celle de $G$ par $H$ est compatible avec la structure de groupe de $G/H$.

Si $x \mapsto \dot{x}$ est l’application canonique de $G$ sur $G/H$, il faut prouver que $(\dot{x}, \dot{y}) \mapsto \dot{x}\dot{y}^{-1}$ est une application continue de $(G/H) \times (G/H)$ dans $G/H$. Comme la relation d’équivalence $x^{-1}y \in H$ est ouverte (III, p. 10, lemme 2), il suffit de montrer que $(x, y) \mapsto \dot{x}\dot{y}^{-1}$ est une application continue de $G \times G$ dans $G/H$ (I, p. 34, cor. de la prop. 8 et I, p. 21, prop. 6). Mais cela résulte de ce que cette application est composée des applications continues $x \mapsto \dot{x}$ et $(x, y) \mapsto xy^{-1}$.

Lorsque nous parlerons désormais d’un groupe quotient $G/H$ d’un groupe topologique $G$ comme d’un groupe topologique, il faudra toujours entendre, sauf mention expresse du contraire, que sa topologie est la topologie quotient de celle de $G$ par $H$.

#### Proposition 17 {#top-iii-s2-prop-17 .statement}

Soit $\varphi$ l’application canonique d’un groupe topologique $G$ sur un groupe quotient $G/H$. Si $\mathfrak{V}$ est un système fondamental de voisinages de $e$ dans $G$, $\varphi(\mathfrak{V})$ est un système fondamental de voisinages de l’élément neutre $\varphi(e)$ de $G/H$.

C’est un cas particulier de la prop. 5 de I, p. 33.

Les prop. 13 et 14 (III, p. 12) donnent en particulier, pour les groupes quotients:

#### Proposition 18 {#top-iii-s2-prop-18 .statement}

Soient $G$ un groupe topologique, $H$ un sous-groupe distingué de $G$.
a) Pour que le groupe quotient $G/H$ soit séparé, il faut et il suffit que $H$ soit fermé dans $G$.
b) Pour que le groupe quotient $G/H$ soit discret, il faut et il suffit que $H$ soit ouvert dans $G$.

Si $G$ est un groupe topologique, et $N$ l’adhérence de $\{e\}$ dans $G$, $N$ est un sous-groupe distingué fermé de $G$ (III, p. 7, prop. 1), donc $G/N$ est séparé; on dit que $G/N$ est le groupe séparé associé à $G$.

#### Proposition 19 {#top-iii-s2-prop-19 .statement}

Si $H$ est un sous-groupe distingué discret d’un groupe topologique $G$, $G/H$ est localement isomorphe (III, p. 6) à $G$.

En effet, soit $V$ un voisinage de $e$ dans $G$, ne contenant aucun point de $H$ autre que $e$, et soit $W$ un voisinage ouvert symétrique de $e$ dans $G$ tel que $W^2 \subset V$. La restriction à $W$ de l’application canonique $\varphi$ de $G$ sur $G/H$ est injective: en effet, la relation $\varphi(x) = \varphi(y)$ signifie que $x^{-1}y \in H$, et si $x \in W, y \in W$, on a $x^{-1}y \in W^2 \subset V$, d’où $x = y$. D’après la prop. 17, la restriction de $\varphi$ à $W$ est donc un homéomorphisme de $W$ sur $\varphi(W)$; comme en outre $\varphi(xy) = \varphi(x)\varphi(y)$ quels que soient $x, y$ dans $W$, $G$ et $G/H$ sont localement isomorphes (III, p. 6, prop. 3).

### 7. Sous-groupes et groupes quotients d’un groupe quotient

Soient G un groupe topologique, H un sous-groupe distingué de G, φ l’application canonique de G sur G/H. On sait (A, I, p. 37) que si A′ est un sous-groupe de G/H, φ(A′) est un sous-groupe de G contenant H. Réciproquement, si A est un sous-groupe de G, φ(A) est un sous-groupe de G/H; en outre, il existe une bijection canonique du groupe quotient A/(A ∩ H) sur le sous-groupe φ(A) de G/H et une bijection canonique de φ(A) sur le groupe quotient AH/H, et ces bijections sont des isomorphismes pour les structures de groupe.

#### Proposition 20 {#top-iii-s2-prop-20 .statement}

Soient A un sous-groupe d’un groupe topologique G, H un sous-groupe distingué de G, φ l’application canonique de G sur G/H. La bijection canonique de φ(A) sur AH/H est un isomorphisme de groupes topologiques.

Cela résulte des remarques qui précèdent, et de la prop. 10 de III, p. 11.

La bijection canonique de A/(A ∩ H) sur φ(A) est un homomorphisme continu, puisqu’elle provient par passage au quotient de la restriction de φ à A, mais en général les groupes topologiques A/(A ∩ H) et AH/H ne sont pas isomorphes (cf. III, p. 27, cor. 3).

*Par exemple, prenons pour G le groupe additif \mathbf{R} des nombres réels, pour H le groupe \mathbf{Z} des entiers, pour A le groupe θ\mathbf{Z} des multiples entiers d’un nombre irrationnel θ; on a A ∩ H = {0}, donc A/(A ∩ H) est un groupe discret, isomorphe à \mathbf{Z}; au contraire, A + H est partout dense dans \mathbf{R} (comme on le verra dans V, §1, prop. 1), donc (A + H)/H, qui est localement isomorphe à A + H (III, p. 13, prop. 19), n’est pas un groupe discret, et par suite n’est pas isomorphe à A/(A ∩ H).*

On a toutefois la proposition suivante:

#### Proposition 21 {#top-iii-s2-prop-21 .statement}

Soient G un groupe topologique, G_0 un sous-groupe partout dense, H_0 un sous-groupe distingué fermé de G_0, H son adhérence dans G, φ l’application canonique G → G/H; la bijection canonique G_0/H_0 → φ(G_0) est un isomorphisme du groupe topologique G_0/H_0 sur un sous-groupe partout dense de G/H.

Comme H_0 = H ∩ G_0, tout revient à prouver que si U_0 est un ensemble ouvert dans G_0, saturé pour la relation x^{-1}y ∈ H_0, il est la trace sur G_0 d’un ensemble ouvert dans G, saturé pour la relation x^{-1}y ∈ H (I, p. 23, prop. 10). Soit U un ensemble ouvert dans G tel que U_0 = U ∩ G_0; comme U_0 = U_0H_0, on vérifie aussitôt que l’on a U_0 = UH_0 ∩ G_0; comme UH_0 est ouvert dans G, on peut donc supposer que U = UH_0. Cela étant, l’ensemble UH est ouvert dans G et saturé pour la relation x^{-1}y ∈ H; montrons que UH ∩ G_0 = U_0, ce qui achèvera la démonstration. Or, si u ∈ U, h ∈ H sont tels que uh ∈ G_0, il y a un voisinage symétrique V de e dans G tel que uV ⊂ U; comme Vh est un voisinage de h dans G, il existe z ∈ V tel que zh ∈ H_0; mais alors uz^{-1} ∈ U et on a uh = (uz^{-1})(zh). On peut donc supposer que h ∈ H_0, et comme UH_0 = U, on a uh ∈ U_0.

Soit G un groupe topologique opérant continûment dans un espace topologique E, et soit K un sous-groupe distingué de G, contenu dans le stabilisateur de chacun des points de E. Pour tout x ∈ E, la relation s ≡ t (mod. K) entraîne donc s.x = t.x, et par passage au quotient on en déduit une application s ↦ s.x de G/K dans E; on vérifie immédiatement que pour la loi externe ainsi définie (s, x) ↦ s.x, G/K opère dans E. En outre, G/K opère continûment dans E pour cette loi: en effet, comme la relation d’égalité dans E et la relation s ≡ t (mod. K) dans G sont ouvertes, cela résulte de la continuité de l’application (s, x) ↦ s.x = s.x de G × E dans E (I, p. 34, cor. de la prop. 8 et I, p. 21, prop. 6).

Soient maintenant G un groupe topologique opérant continûment dans un espace topologique E, H un sous-groupe quelconque de G. Le groupe H opère continûment dans E; soit S la relation d’équivalence dans E définie par H, qui est ouverte (III, p. 10, lemme 2). La relation S est compatible avec le groupe G (III, p. 11); en effet, si y ≡ x (mod. S), il existe t ∈ H tel que y = t.x, d’où, pour tout s ∈ G, s.y = (sts^{-1}).(s.x), et comme H est distingué, sts^{-1} ∈ H, d’où notre assertion. Si ψ est l’application canonique de E sur E/S, le groupe G opère donc continûment dans E/S pour la loi externe (s, ψ(x)) ↦ ψ(s.x) (III, p. 11, prop. 11). En outre, le groupe H est contenu dans le stabilisateur de chacun des points de E/S; comme on l’a vu ci-dessus, G/H opère continûment dans E/S = E/H, pour la loi externe (s, ψ(x)) ↦ ψ(s.x). Si on désigne par R la relation d’équivalence dans E définie par G, la relation S entraîne R, et la relation d’équivalence R/S dans E/S est la relation définie par le groupe G/H. Par suite (I, p. 21, prop. 7):

#### Proposition 22 {#top-iii-s2-prop-22 .statement}

Soient G un groupe topologique opérant continûment dans un espace topologique E, H un sous-groupe distingué de G. La bijection canonique de E/G sur (E/H)/(G/H) est un homéomorphisme.

#### Corollaire {#top-iii-s2-n7-cor-1 .statement}

Soient G un groupe topologique, H un sous-groupe distingué de G, K un sous-groupe distingué de G contenant H; la bijection canonique de G/K sur (G/H)/(K/H) est un isomorphisme de groupes topologiques.

On sait déjà (A, I, p. 39) que cette bijection est un isomorphisme de groupes, et la prop. 22 (appliquée au groupe K opérant à droite dans G) achève d’établir le corollaire.

### 8. Homomorphismes continus et morphismes stricts

#### Proposition 23 {#top-iii-s2-prop-23 .statement}

Pour qu’un homomorphisme f d’un groupe topologique G dans un groupe topologique G' soit continu dans G, il faut et il suffit qu’il soit continu en un point.

La condition est évidemment nécessaire. Réciproquement, si f est continu au point a ∈ G et si V' est un voisinage de f(a), f^{-1}(V') = V est un voisinage de a; pour tout x ∈ G, on a f(xa^{-1}V) = f(x)(f(a))^{-1}f(V) ⊂ f(x)(f(a))^{-1}V', ce qui établit la continuité de f au point x.

Un homomorphisme continu d’un groupe topologique G dans un groupe topologique G' est encore appelé un morphisme de G dans G' pour les structures de groupe topologique (cf. E, IV, p. 11).

Soit f un homomorphisme continu d’un groupe topologique G dans un groupe topologique G'; l’image réciproque H = $\overline{f}(e')$ de l’élément neutre e' de G' est un sous-groupe distingué de G et $f(G)$ est un sous-groupe de G'. Considérons la factorisation canonique $f = \psi \circ \dot{f} \circ \varphi$, où $\varphi$ est l’application canonique $G \to G/H$, $\psi$ l’injection canonique $f(G) \to G'$, et enfin $\dot{f}$ un homomorphisme continu bijectif du groupe quotient G/H sur le sous-groupe $f(G)$ (I, p. 22); on dira que $\dot{f}$ est l’homomorphisme bijectif associé à f. En général, $\dot{f}$ n’est pas un isomorphisme de groupes topologiques.

Par exemple, soient G' un groupe topologique non discret, G le groupe topologique obtenu en munissant G' de la topologie discrète; l’application identique de G dans G' est un homomorphisme bijectif continu, mais non bicontinu.

#### Définition 1 {#top-iii-s2-def-1 .statement}

On dit qu’un homomorphisme continu f d’un groupe topologique G dans un groupe topologique G' est un morphisme strict de G dans G', si l’homomorphisme bijectif $\dot{f}$ de $G/\overline{f}(e')$ sur $f(G)$, associé à f, est un isomorphisme de groupes topologiques (autrement dit, si $\dot{f}$ est bicontinu).

Un isomorphisme d’un groupe topologique G sur un groupe topologique G' est donc un morphisme strict bijectif de G dans G'.

#### Proposition 24 {#top-iii-s2-prop-24 .statement}

Soit f un homomorphisme continu d’un groupe topologique G dans un groupe topologique G'; les trois propositions suivantes sont équivalentes:
a) f est un morphisme strict;
b) l’image par f de tout ensemble ouvert dans G est un ensemble ouvert dans b(G);
c) l’image par f de tout voisinage de l’élément neutre dans G est un voisinage de l’élément neutre dans $f(G)$.

Compte tenu du lemme 2 de III, p. 10, l’équivalence de a) et b) résulte aussitôt des définitions (I, p. 33, prop. 5). L’équivalence de b) et c) est un cas particulier de la prop. 15 de III, p. 12, si l’on observe que G opère continûment dans $f(G)$ par la loi externe $(s, f(t)) \mapsto f(st)$.

#### Remarque 1 {#top-iii-s2-n8-rem-1 .statement}

D’après la condition b) de la prop. 24, tout homomorphisme continu d’un groupe topologique dans un groupe discret est un morphisme strict.

Si le groupe G est compact et $f(G)$ séparé, l’homomorphisme bijectif $\dot{f}$ associé à f est bicontinu (I, p. 76, cor 2, et I, p. 74, cor. 4); donc, tout homomorphisme continu d’un groupe compact dans un groupe séparé est un morphisme strict.

#### Remarque 2 {#top-iii-s2-n8-rem-2 .statement}

Soient f un morphisme strict de G dans G', g un morphisme strict de G' dans G"; si f est surjectif, ou si g est injectif, il résulte aussitôt de la prop. 24 que $g \circ f$ est un morphisme strict de G dans G". Par contre, cette conclusion n’est plus nécessairement valable si aucune des deux hypothèses précédentes n’est satisfaite, même si f est injectif et g surjectif (III, p. 70, exerc. 19).

#### Remarque 3 {#top-iii-s2-n8-rem-3 .statement}

Soit $f$ un homomorphisme continu d’un groupe topologique $G$ dans un groupe topologique $G'$, et soit $H$ un sous-groupe distingué de $G$; par passage aux quotients, on déduit de $f$ un homomorphisme $g$ du groupe $G/H$ sur le groupe quotient $f(G)/f(H)$. Cet homomorphisme est *continu* (I, p. 21, corollaire). En outre, si $f$ est un *morphisme strict* de $G$ dans $G'$, $g$ est un *morphisme strict* de $G/H$ sur $f(G)/f(H)$: en effet, si $U$ est ouvert dans $G/H$, et si on désigne par $\varphi$ (resp. $\varphi'$) l’application canonique de $G$ sur $G/H$ (resp. de $f(G)$ sur $f(G)/f(H)$), on a $g(U) = \varphi'(f(\varphi^{-1}(U)))$, et comme $\varphi^{-1}(U)$ est ouvert dans $G$, $g(U)$ est ouvert dans $f(G)/f(H)$, d’où notre assertion.

### 9. Produit de groupes topologiques

Soit $(G_i)_{i \in I}$ une famille de groupes topologiques. On sait (A, I, p. 43) qu’on définit sur l’ensemble produit $G = \prod_{i \in I} G_i$ une structure de groupe (dite *produit* des structures de groupes des $G_i$) en posant $(x_i).(y_i) = (x_i y_i)$; si $e_i$ est l’élément neutre de $G_i$, $e = (e_i)$ est l’élément neutre de $G$, et on a $(x_i)^{-1} = (x_i^{-1})$. La *topologie produit* (I, p. 14) des topologies des $G_i$ est *compatible* avec la structure de groupe précédente. En effet, l’application $((x_i), (y_i)) \mapsto (x_i y_i^{-1})$ de $G \times G$ dans $G$ est composée de l’application $((x_i, y_i)) \mapsto (x_i y_i^{-1})$ de $\prod_{i \in I} (G_i \times G_i)$ dans $G$, et de l’application canonique $((x_i), (y_i)) \mapsto ((x_i, y_i))$ de $G \times G$ sur $\prod_{i \in I} (G_i \times G_i)$; et ces applications sont continues (I, p. 25, cor. 1 et prop. 2).

#### Définition 2 {#top-iii-s2-def-2 .statement}

*On dit que le groupe topologique obtenu en munissant l’ensemble produit $G = \prod_{i \in I} G_i$ de la structure de groupe produit des structures de groupe des $G_i$, et de la topologie produit des topologies des $G_i$, est le produit des groupes topologiques $G_i$.*.

Si $(J_k)_{k \in K}$ est une *partition* de $I$, $G$ est isomorphe au produit des groupes topologiques $\prod_{i \in J_k} G_i$ (associativité du produit).

Si $H_i$ est un sous-groupe de $G_i$, le produit des groupes topologiques $H_i$ est isomorphe au sous-groupe $\prod_i H_i$ de $\prod_i G_i$. En particulier, soit $J$ une partie quelconque de $I$, et $J' = \complement J$; le groupe topologique $\prod_{i \in J} G_i$ est isomorphe au sous-groupe distingué $G'_J = (\prod_{i \in J} G_i) \times (\prod_{i \in J'} \{e_i\})$ de $G$. Comme la projection de tout ensemble ouvert est un ensemble ouvert, la projection $\mathrm{pr}_J$ de $G$ sur $\prod_{i \in J} G_i$ est un *morphisme strict*; par suite, le groupe quotient $G/G'_J$ est isomorphe à $G'_{J'}$: $G$ est isomorphe au produit $G'_J \times (G/G'_J)$.

#### Proposition 25 {#top-iii-s2-prop-25 .statement}

*Soit $(G_i)_{i \in I}$ une famille de groupes topologiques, et soit $H$ le sous-* groupe distingué de $G = \prod_{i \in I} G_i$ formé des $x = (x_i)$ tels que les $x_i$ soient égaux à l’élément neutre $e_i$ de $G_i$ sauf pour un nombre fini d’indices. Le sous-groupe $H$ est partout dense dans $G$.

C’est un cas particulier de I, p. 28, prop. 8.

Soit $(E_i)_{i \in I}$ une famille d’espaces topologiques, et pour chaque $i \in I$, soit $G_i$ un groupe topologique opérant continûment dans $E_i$. Il est clair que le groupe produit $G = \prod_{i \in I} G_i$ opère continûment dans l’espace produit $E = \prod_{i \in I} E_i$ pour la loi externe $((s_i), (x_i)) \mapsto (s_i \cdot x_i)$ (I, p. 25, cor. 1 et prop. 2); en outre l’orbite pour $G$ d’un point $x = (x_i)$ de $E$ est le produit des orbites des $x_i$ (pour les $G_i$). Soit $\varphi_i$ l’application canonique de $E_i$ sur $E_i / G_i$, et soit $\varphi = (\varphi_i)$ l’application produit de $E$ sur $\prod_{i \in I} (E_i / G_i)$; la remarque précédente montre que la bijection canoniquement associée à $\varphi$ applique l’espace des orbites $E/G$ sur $\prod_{i \in I} (E_i / G_i)$. En outre:

#### Proposition 26 {#top-iii-s2-prop-26 .statement}

*La bijection de $E/G$ sur $\prod_{i \in I} (E_i / G_i)$ canoniquement associée à $(\varphi_i)$ est un homéomorphisme.*

En effet, comme les $\varphi_i$ sont surjectives et ouvertes, $\varphi = (\varphi_i)$ est ouverte (I, p. 34, cor. de la prop. 8).

#### Corollaire {#top-iii-s2-n9-cor-1 .statement}

*Soit $(G_i)_{i \in I}$ une famille de groupes topologiques, et pour chaque $i \in I$, soit $H_i$ un sous-groupe distingué de $G_i$; on désigne par $\varphi_i$ l’application canonique de $G_i$ sur $G_i / H_i$. Posons $G = \prod_{i \in I} G_i$, $H = \prod_{i \in I} H_i$. L’homomorphisme bijectif de $G/H$ sur $\prod_{i \in I} (G_i / H_i)$ associé à l’homomorphisme continu $(x_i) \mapsto (\varphi_i(x_i))$ est un isomorphisme de groupes topologiques.*

En effet, cet homomorphisme est un isomorphisme pour les structures de groupe.

#### Remarque {#top-iii-s2-n9-rem-1 .statement}

Si $G$ est un groupe topologique *commutatif* noté additivement, l’application $(x, y) \mapsto x + y$ de $G \times G$ sur $G$ est un *morphisme strict*; c’est en effet un homomorphisme de $G \times G$ sur $G$, puisque $(x + x') + (y + y') = (x + y) + (x' + y')$; il est continu, et enfin l’image du voisinage $V \times V$ de l’origine dans $G \times G$, par cet homomorphisme, est le voisinage $V + V$ de l’origine dans $G$.

### 10. Produits semi-directs de groupes topologiques

#### Proposition 27 {#top-iii-s2-prop-27 .statement}

*Soient $L, N$ deux groupes topologiques, $y \mapsto \sigma_y$ un homomorphisme de $L$ dans le groupe des automorphismes $\Gamma$ de la structure de groupe (non topologique) de $N$. On suppose que l’application $(x, y) \mapsto \sigma_y(x)$ de $N \times L$ dans $N$ est continue. Alors:
1° Sur le produit semi-direct externe $S$ de $N$ et de $L$, relatif à $\sigma$ (A, I, p. 64, déf. 2), la topologie produit de celles de $N$ et de $L$ est compatible avec la structure de groupe; les injections canoniques $j_1 : N \to S, j_2 : L \to S$ sont des isomorphismes respectifs des groupes* topologiques $N$ et $L$ sur les sous-groupes $j_1(N)$ et $j_2(L)$ du groupe topologique $S$, et $pr_2$ est un morphisme strict de $S$ sur $L$.

$2^\circ$ Soient $f : N \to G,\ g : L \to G$ deux homomorphismes continus dans un groupe topologique $G$, vérifiant la relation $f(\sigma_y(x)) = g(y)f(x)g(y^{-1})$; alors l’homomorphisme associé : $(x, y) \mapsto f(x)g(y)$ de $S$ dans $G$ est continue.

La proposition résulte aussitôt des définitions et des propriétés de la topologie produit.

On dit que le groupe topologique $S$ ainsi défini est le *produit semi-direct topologique externe* de $N$ et de $L$ (relatif à $\sigma$); on observera que la condition imposée à $\sigma$ implique que $L$ *opère continûment à gauche* dans $N$ pour la loi externe $(x, y) \mapsto \sigma_y(x)$ (III, p. 10).

Soient maintenant $G$ un groupe topologique, $N, L$ deux sous-groupes de $G$ tels que $G$ soit, en tant que groupe non muni d’une topologie, le *produit semi-direct* de $N$ et de $L$ (A, I, p. 65); il est clair alors que l’application $(x, y) \mapsto \sigma_y(x)$ est *continue* dans $N \times L$, et l’homomorphisme canonique bijectif $h : (x, y) \mapsto xy$ de $S$ dans $G$ *continu*. Mais ce dernier homomorphisme n’est pas nécessairement *bicontinu*; lorsqu’il est bicontinu, on dit que $G$ est *produit semi-direct topologique* de $N$ et de $L$. Pour qu’il en soit ainsi, il faut et il suffit que, si $p : G \to N,\ q : G \to L$ sont les applications faisant correspondre à $z \in G$ les éléments uniques $p(z) \in N,\ q(z) \in L$ tels que $z = p(z)q(z)$, l’une des applications $p,\ q$ soit *continue* (auquel cas toutes deux le sont). Il revient au même de dire que la restriction à $L$ de l’application canonique $G \to G/N$ est un isomorphisme du groupe topologique $L$ sur le groupe topologique $G/N$.

## EXERCICES {#top-iii-s2-exercises}

See the [exercises for § 2](exercises/s2/).
