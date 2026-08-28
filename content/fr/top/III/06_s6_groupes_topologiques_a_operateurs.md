---
book: top
book_title: General Topology
chapter: III
chapter_title: GROUPES TOPOLOGIQUES
section: 6
section_title: Groupes topologiques à opérateurs ; anneaux topologiques ; corps topologiques
lang: fr
source: top-i-iv-fr
book_pages: TG III.45-TG III.56, TG III.79-TG III.85
pdf_pages: 0228-0239, 0262-0268
extraction: ocr
subsections:
    - "no": 1
      title: Groupes topologiques à opérateurs
      page: 45
      pdf_page: 228
    - "no": 2
      title: Somme directe topologique de sous-groupes stables
      page: 46
      pdf_page: 229
    - "no": 3
      title: Anneaux topologiques
      page: 48
      pdf_page: 231
    - "no": 4
      title: Sous-anneaux. Idéaux. Anneaux quotients. Produits d’anneaux
      page: 50
      pdf_page: 233
    - "no": 5
      title: Complétion d’un anneau topologique
      page: 50
      pdf_page: 233
    - "no": 6
      title: Modules topologiques
      page: 52
      pdf_page: 235
    - "no": 7
      title: Corps topologiques
      page: 54
      pdf_page: 237
    - "no": 8
      title: Structures uniformes d’un corps topologique
      page: 55
      pdf_page: 238
statements: 20
exercises: 29
content_sha256: d9372c11396f6f8af17b5a832d391657f022a49ad7fb9031449217f3aa3234c5
---

## § 6. GROUPES TOPOLOGIQUES À OPÉRATEURS; ANNEAUX TOPOLOGIQUES; CORPS TOPOLOGIQUES

### 1. Groupes topologiques à opérateurs

Sur un ensemble G, on dit qu’une structure de *groupe à opérateurs* (A, I, p. 29) et une topologie sont *compatibles* si la topologie et la structure de groupe de G sont compatibles (III, p. 1) et si en outre les endomorphismes de G définis par les opérateurs (A, I, p. 30) sont *continus*. On dit alors que G, muni de la structure de groupe à opérateurs et de la topologie données, est un *groupe topologique à opérateurs*.

Si H est un sous-groupe stable d’un groupe topologique à opérateurs G, la topologie induite sur H par celle de G est compatible avec la structure de groupe à opérateurs de H. En outre:

#### Proposition 1 {#top-iii-s6-prop-1 .statement}

*Si H est un sous-groupe stable d’un groupe topologique à opérateurs G, l’adhérence $\overline{H}$ de H dans G est un sous-groupe stable de G.*

On sait déjà que $\overline{H}$ est un sous-groupe de G (III, p. 7, prop. 1); en outre, pour tout opérateur $\alpha$ de G, l’image de H par l’application continue $x \mapsto x^\alpha$ est contenue dans H, donc l’image de $\overline{H}$ est contenue dans $\overline{H}$ (I, p. 9, th. 1).

Soit H un sous-groupe stable distingué d’un groupe topologique à opérateurs; pour tout opérateur $\alpha$ de G, l’application de G/H dans lui-même obtenue à partir de $x \mapsto x^\alpha$ par passage aux quotients est continue (III, p. 17, *Remarque 3*); la structure de groupe à opérateurs de G/H est donc compatible avec la topologie quotient de celle de G par H.

Soit $(G_t)_{t \in I}$ une famille de groupes topologiques à opérateurs, tous les $G_t$ étant supposés avoir le même ensemble d’opérateurs $\Omega$. Pour tout $\alpha \in \Omega$, l’application $x \mapsto ((\mathrm{pr}_t x)^\alpha)$ de $G = \prod_{t \in I} G_t$ dans lui-même est continue (I, p. 25, prop. 1); la structure de groupe à opérateurs de G est donc compatible avec la topologie produit des topologies des $G_i$.

Si G est un groupe topologique à opérateurs séparé, admettant un complété $\hat{G}$ (III, p. 24), tout endomorphisme $x \mapsto x^\alpha$ de G, défini par un opérateur de G, se prolonge par continuité en un endomorphisme de $\hat{G}$ (III, p. 22, prop. 5), donc $\hat{G}$ est ainsi muni d’une structure de groupe topologique à opérateurs, ayant même ensemble d’opérateurs que G.

### 2. Somme directe topologique de sous-groupes stables

Comme l’étude des groupes commutatifs à opérateurs est équivalente à celle des modules (A, III, p. 21) nous nous permettrons d’utiliser à l’occasion la terminologie propre à ces derniers pour les groupes commutatifs à opérateurs quelconques; c’est ainsi que nous parlerons d’applications linéaires au lieu d’homomorphismes de groupes commutatifs à opérateurs, et que nous appellerons encore projecteur un endomorphisme idempotent d’un groupe commutatif à opérateurs (A, II, p. 18).

Lorsqu’un groupe topologique commutatif à opérateurs E (noté additive-ment) est somme directe d’une famille finie $(M_i)_{1 \leq i \leq n}$ de sous-groupes stables, l’application canonique bijective $(x_i) \mapsto \sum_{i=1}^n x_i$ du groupe produit $\prod_{i=1}^n M_i$ sur E est continue, mais n’est pas nécessairement un homéomorphisme.

#### Définition 1 {#top-iii-s6-def-1 .statement}

Soit E un groupe topologique commutatif à opérateurs et soit $(M_i)_{1 \leq i \leq n}$ une famille finie de sous-groupes stables de E, telle que E soit somme directe des $M_i$. On dit que E est somme directe topologique des $M_i$ si l’application canonique $(x_i) \mapsto \sum_{i=1}^n x_i$ du groupe produit $\prod_{i=1}^n M_i$ sur E est un homéomorphisme (et par suite un isomorphisme de groupes topologiques à opérateurs).

#### Proposition 2 {#top-iii-s6-prop-2 .statement}

Soit E un groupe topologique commutatif à opérateurs somme directe des sous-groupes stables $M_i$ ($1 \leq i \leq n$); soit $(p_i)_{1 \leq i \leq n}$ la famille de projecteurs associée à la décomposition $E = \sum_{i=1}^n M_i$ (A, II, p. 18, prop. 12). Pour que E soit somme directe topologique des $M_i$, il faut et il suffit que les $p_i$ soient continus.

En effet, l’application $x \mapsto (p_i(x))$ est l’application réciproque de $(x_i) \mapsto \sum_{i=1}^n x_i$.

Comme $1_E = \sum_{i=1}^n p_i$ (1_E désignant l’application identique de E), il suffit que $n - 1$ des projecteurs $p_i$ soient continus pour que le n-ème le soit.

Lorsque E est somme directe topologique de deux sous-groupes stables M, N, on dit encore que N est un supplémentaire topologique de M dans E; pour qu’il en soit ainsi, il faut et il suffit que l’application canonique de E/M sur N (A, II, p. 20, prop. 13) soit un isomorphisme de groupes topologiques à opérateurs.

#### Corollaire {#top-iii-s6-n2-cor-1 .statement}

Soient E un groupe topologique commutatif à opérateurs, M un sous-groupe stable de E. Les conditions suivantes sont équivalentes:
a) M admet dans E un supplémentaire topologique.
b) Il existe un projecteur continu p de E dans E tel que p(E) = M.
c) L’application identique de M peut être prolongée en une application linéaire continue de E dans M.

Il résulte de la prop. 2 que a) entraîne b) et il est clair que b) entraîne c). Enfin, si p est une application linéaire continue de E dans M prolongeant l’application identique de M, p est un projecteur continu et les projecteurs p et $1_E - p$ sont associés à la décomposition en somme directe $E = M + N$, où $N = p^{-1}(0)$.

#### Remarque 1 {#top-iii-s6-n2-rem-1 .statement}

Pour éviter toute confusion, on dit parfois qu’un sous-groupe stable de E supplémentaire de M (au sens de la structure de groupe à opérateurs sans topologie) est un supplémentaire algébrique de M.
2) Lorsqu’un groupe topologique commutatif à opérateurs séparé E est somme directe topologique d’une famille $(M_i)_{1 \leq i \leq n}$ de sous-groupes stables, chacun des sous-groupes $M_i$ est fermé dans E, car c’est l’ensemble des $x \in E$ tels que $p_i(x) = x$ (I, p. 53, prop. 2).

#### Proposition 3 {#top-iii-s6-prop-3 .statement}

Soient E, F deux groupes topologiques commutatifs à opérateurs, u une application linéaire continue de E dans F. Pour qu’il existe une application linéaire continue v de F dans E telle que $u \circ v$ soit l’application identique de F (auquel cas on dit que u est inversible à droite et que v est inverse à droite de u), il faut et il suffit que u soit un morphisme strict (III, p. 16) de E sur F et que $u^{-1}(0)$ admette un supplémentaire topologique dans E.

Les conditions sont nécessaires. En effet, on a alors $u(v(F)) = F$ et a fortiori $u(E) = F$; en outre; si l’on pose $p = v \circ u$, p est une application linéaire continue de E dans lui-même telle que $p^2 = p$; par suite (III, p. 47, corollaire) $p(E) = v(u(E)) = v(F)$ admet dans E un supplémentaire topologique $p^{-1}(0)$; mais comme $u(p(x)) = u(x)$ par hypothèse, on a $u(0) = p^{-1}(0)$. Enfin l’application bijective de $E/u^{-1}(0)$ sur F, associée à u, est composée de l’application bijective de $E/p^{-1}(0)$ sur $v(F)$, associée à p, et de la restriction de u à $v(F)$; comme v est continue, ces deux applications sont des isomorphismes, donc u est un morphisme strict de E sur F.

Les conditions sont suffisantes. En effet, si $\varphi$ est l’homomorphisme canonique de E sur $E/u^{-1}(0)$, dire que $u^{-1}(0)$ admet un supplémentaire topologique M dans E signifie que la restriction de $\varphi$ à $M$ est un isomorphisme de $M$ sur $E / u^{-1}(0)$. Comme d’autre part $u = w \circ \varphi$, où $w$ est un isomorphisme de $E / u^{-1}(0)$ sur $E$, on voit que la restriction de $u$ à $M$ est un isomorphisme de $M$ sur $F$, et l’isomorphisme réciproque $v$ est donc tel que $u \circ v$ soit l’application identique de $F$ sur lui-même.

#### Proposition 4 {#top-iii-s6-prop-4 .statement}

*Soient* $E, F$ *deux groupes topologiques commutatifs à opérateurs*, $u$ *une application linéaire continue de* $E$ *dans* $F$. *Pour qu’il existe une application linéaire continue* $v$ *de* $F$ *dans* $E$ *telle que* $v \circ u$ *soit l’application identique de* $E$ *sur lui-même* (auquel cas on dit que $u$ est *inversible à gauche* et que $v$ est *inverse à gauche de* $u$), *il faut et il suffit que* $u$ *soit un isomorphisme (topologique)* *de* $E$ *sur* $u(E)$, *et que* $u(E)$ *admette un supplémentaire topologique dans* $F$.

Les conditions sont *suffisantes*, car si elles sont remplies, on obtient un inverse à gauche $v$ de $u$ en prenant le composé de l’isomorphisme de $u(E)$ sur $E$, réciproque de $u$, et d’un projecteur continu de $F$ sur $u(E)$.

Les conditions sont *nécessaires*. En effet, la relation $v(u(x)) = x$ montre que $u^{-1}(0)$ est réduit à $0$; $u$ est donc une bijection de $S$ sur $u(E)$, et comme la restriction de $v$ à $u(E)$ est continue, $u$ est un isomorphisme de $E$ sur $u(E)$. D’autre part, si l’on pose $q = u \circ v$, $q$ est une application linéaire continue de $F$ sur $u(E)$ telle que $q^2 = q$, ce qui prouve (III, p. 47, corollaire) que $u(E)$ admet un supplémentaire topologique dans $F$.

### 3. Anneaux topologiques

#### Définition 2 {#top-iii-s6-def-2 .statement}

*On appelle anneau topologique un ensemble* $A$ *muni d’une structure d’anneau et d’une topologie satisfaisant aux axiomes suivants*:

*(AT$_I$)*. *L’application* $(x, y) \mapsto x + y$ *de* $A \times A$ *dans* $A$ *est continue*.
*(AT$_{II}$)*. *L’application* $x \mapsto -x$ *de* $A$ *dans* $A$ *est continue*.
*(AT$_{III}$)*. *L’application* $(x, y) \mapsto xy$ *de* $A \times A$ *dans* $A$ *est continue*.

Les deux premiers axiomes expriment que la topologie de $A$ est compatible avec sa structure de *groupe additif* (III, p. 1).

Une structure d’anneau et une topologie étant données sur un ensemble $A$, on dit qu’elles sont *compatibles* si elles satisfont aux axiomes (AT$_I$), (AT$_{II}$) et (AT$_{III}$).

#### Exemple 1 {#top-iii-s6-n3-exa-1 .statement}

Sur un anneau $A$, la topologie *discrète* est compatible avec la structure d’anneau; un anneau topologique dont la topologie est discrète est dit anneau *discret*.
*2) On verra dans IV, p. 10 (resp. p. 11) que la topologie de la droite rationnelle $\mathbf{Q}$ (resp. de la droite numérique $\mathbf{R}$) est compatible avec la structure d’anneau de $\mathbf{Q}$ (resp. $\mathbf{R}$).*

Dans un anneau topologique, toute *homothétie* à gauche $x \mapsto ax$ (resp. toute homothétie à droite $x \mapsto xa$ est continue (et est un homéomorphisme si $a$ est inversible).

Soit $A$ un anneau topologique, et soit $G$ le groupe des éléments inversibles de $A$. Soit $\mathcal{T}$ la topologie la moins fine sur $G$ rendant continues les applications $x \mapsto x$ et $x \mapsto x^{-1}$ de $G$ dans $A$ (I, p. 12, prop. 4). Alors $\mathcal{T}$ est *compatible* avec la structure de groupe de $G$. En effet, il suffit de montrer que lorsque $G$ est muni de $\mathcal{T}$, les applications $(x, y) \mapsto xy^{-1}$ et $(x, y) \mapsto yx^{-1}$ de $G \times G$ dans $A$ sont continues (*loc. cit.*); or, par exemple, l’application $(x, y) \mapsto xy^{-1}$ de $G \times G$ dans $A$ est composée de l’application $(u, v) \mapsto uv$ de $A \times A$ dans $A$ et de l’application $(x, y) \mapsto (x, y^{-1})$ de $G \times G$ dans $A \times A$, et ces applications sont toutes deux continues par définition; on raisonne de même pour l’application $(x, y) \mapsto yx^{-1}$.

Comme on peut écrire identiquement
$$
xy - x_0y_0 = (x - x_0)(y - y_0) + (x - x_0)y_0 + x_0(y - y_0),
$$
l’axiome (AT$_{\text{III}}$) (compte tenu de (AT$_{\text{I}}$) et (AT$_{\text{II}}$)), est équivalent aux deux suivants:
(AT$_{\text{IIIa}}$) *Quel que soit* $x_0 \in A$, les *applications* $x \mapsto x_0x$ et $x \mapsto xx_0$ sont *continues au point* $x = 0$.
(AT$_{\text{IIIb}}$) *L’application* $(x, y) \mapsto xy$ de $A \times A$ dans $A$ est *continue au point* $(0, 0)$.

On en déduit un système de conditions nécessaires et suffisantes que doit vérifier le *filtre* $\mathcal{V}$ *des voisinages de* 0 dans un anneau $A$ pour définir sur $A$ une topologie compatible avec sa structure d’anneau: $\mathcal{V}$ doit satisfaire aux axiomes (GA$_{\text{I}}$) et (GA$_{\text{II}}$) de III, p. 4, et en outre aux deux axiomes suivants:
(AV$_{\text{I}}$) *Quels que soient* $x_0 \in A$ et $V \in \mathcal{V}$, *il existe* $W \in \mathcal{V}$ *tel que* $x_0W \subset V$ *et* $Wx_0 \subset V$.
(AV$_{\text{II}}$) *Quel que soit* $V \in \mathcal{V}$, *il existe* $W \in \mathcal{V}$ *tel que* $WW \subset V$.

#### Remarque {#top-iii-s6-n3-rem-1 .statement}

On rencontre assez souvent en Analyse des anneaux vérifiant les axiomes (AT$_{\text{I}}$), (AT$_{\text{II}}$) et (AT$_{\text{IIIa}}$), mais non (AT$_{\text{IIIb}}$). *Un exemple est l’anneau des mesures sur un groupe compact, où la loi multiplicative est la convolution, et la topologie est la topologie vague (INT, VIII).*.

*Exemple 3).* — Soit $\mathcal{B}$ une *base de filtre* sur un anneau $A$, formée d’*idéaux bilatères*; $\mathcal{B}$ est un système fondamental de voisinages de 0 pour une topologie compatible avec la structure de groupe additif de $A$; il résulte aussitôt de (AV$_{\text{I}}$) et (AV$_{\text{II}}$) que cette topologie est compatible avec la structure d’*anneau* de $A$.

Soient $E$ un espace topologique, $f$ et $g$ deux applications de $E$ dans un anneau topologique $A$; si $f$ et $g$ sont continues en un point $x_0 \in E$, $f + g$, $-f$ et $fg$ sont aussi continues en ce point. Il en résulte que les applications continues de $E$ dans $A$ forment un *sous-anneau* de l’anneau $A^E$ des applications de $E$ dans $A$. On voit aussi que, si $A$ est *commutatif*, tout *polynôme en n variables*, à coefficients dans $A$, et défini dans $A^n$, est *continu* dans $A^n$. De même, soient $f$ et $g$ deux applications d’un ensemble $E$ *filtré* par un filtre $\mathfrak{F}$, dans un anneau topologique *séparé* $A$; si $\lim_{\mathfrak{F}} f$ et $\lim_{\mathfrak{F}} g$ existent, il en est de même de $\lim_{\mathfrak{F}} (f + g)$, $\lim_{\mathfrak{F}} (-f)$ et $\lim_{\mathfrak{F}} (fg)$, et on a (I, p. 50, cor. 1 et I, p. 52, prop. 1)
$$
\begin{align*}
(1)\quad \lim_{\mathfrak{F}} (f + g) &= \lim_{\mathfrak{F}} f + \lim_{\mathfrak{F}} g \\
(2)\quad \lim_{\mathfrak{F}} (-f) &= -\lim_{\mathfrak{F}} f \\
(3)\quad \lim_{\mathfrak{F}} (fg) &= (\lim_{\mathfrak{F}} f)(\lim_{\mathfrak{F}} g).
\end{align*}
$$

### 4. Sous-anneaux. Idéaux. Anneaux quotients. Produits d’anneaux

Si H est un sous-anneau d’un anneau topologique A, la topologie induite sur H par celle de A est compatible avec la structure d’anneau de H; la structure d’anneau topologique ainsi définie sur H est dite induite par celle de A.

#### Proposition 5 {#top-iii-s6-prop-5 .statement}

Soit H un sous-anneau partout dense d’un anneau topologique A, et K un sous-anneau (resp. idéal à gauche, idéal à droite, idéal bilatère) de H. L’adhérence $\overline{K}$ de K dans A est un sous-anneau (resp. idéal à gauche, idéal à droite, idéal bilatère) de A.

Le raisonnement est le même que pour la prop. 9 de III, p. 9: si par exemple K est idéal à gauche dans H, l’application $(z, x) \mapsto zx$ est continue dans $A \times A$, et applique $H \times K$ dans K; elle applique donc $A \times \overline{K} = \overline{H} \times \overline{K}$ dans $\overline{K}$.

Soit H un idéal bilatère dans un anneau topologique A; par le même raisonnement que pour les groupes quotients (III, p. 13, prop. 16), on voit que la topologie quotient de celle de A par la relation $x - y \in H$ est compatible avec la structure d’anneau de A/H. En particulier, l’adhérence N de 0 dans A est un idéal bilatère fermé, d’après la prop. 5; l’anneau quotient A/N, qui est séparé (III, p. 12, prop. 13), est dit l’anneau séparé associé à A.

Soit $(A_i)_{i \in I}$ une famille d’anneaux topologiques. Sur l’ensemble produit $A = \prod_{i \in I} A_i$, la topologie produit des topologies des $A_i$ est compatible avec la structure d’anneau, produit des structures d’anneau des $A_i$ (même démonstration que pour les groupes produits); l’anneau topologique A ainsi défini est dit le produit des anneaux topologiques $A_i$.

### 5. Complétion d’un anneau topologique

Quand on parle de la structure uniforme d’un anneau topologique A, il s’agit toujours, sauf mention expresse du contraire, de la structure uniforme de son groupe additif; en particulier, on dit que A est un anneau complet si son groupe additif est complet.

Soit A un anneau topologique séparé: muni de sa structure de groupe additif, il peut être considéré comme sous-groupe partout dense d’un groupe commutatif séparé et complet $\hat{A}$, déterminé à une isomorphie près (III, p. 26, th. 2). Pour qu’on puisse considérer A comme un sous-anneau d’un anneau complet, il faut qu’on puisse prolonger par continuité la fonction $xy$ à l’espace $\hat{A} \times \hat{A}$. La possibilité de ce prolongement va résulter du théorème plus général suivant:

#### Théorème 1 {#top-iii-s6-thm-1 .statement}

Soient E, F, G trois groupes commutatifs séparés et complets, A un sous-groupe partout dense de E, B un sous-groupe partout dense de F. Si f est une application

**Z-bilinéaire**$^{1}$ continue de $A \times B$ dans $G$, $f$ peut être prolongée par continuité en une application **Z-bilinéaire continu** de $E \times F$ dans $G$.

Soient $(x_0, y_0)$ un point quelconque de $E \times F$, $\mathcal{U}$ et $\mathcal{V}$ les traces sur $A$ et $B$ respectivement, des filtres de voisinages de $x_0$ et $y_0$ ($\mathcal{U}$ et $\mathcal{V}$ sont des filtres par hypothèse); pour montrer que $f$ peut être prolongée par continuité, il suffit de voir que $f(\mathcal{U} \times \mathcal{V})$ est une *base de filtre de Cauchy* dans $G$ (II, p. 20, prop. 11). Partons de l’identité:

$$
f(x', y') - f(x, y) = f(x' - x, y_1) + f(x_1, y' - y)
+ f(x' - x, y' - y_1) + f(x - x_1, y' - y).
$$

Nous allons voir qu’en prenant $(x, y)$ et $(x', y')$ dans un ensemble assez petit de $\mathcal{U} \times \mathcal{V}$, et en choisissant convenablement $x_1$ et $y_1$, on peut rendre très petit chacun des termes du second membre. Soit $W$ un voisinage quelconque de 0 dans $G$; $f$ étant continue au point $(0, 0)$ de $A \times B$, il existe un ensemble $U \in \mathcal{U}$ et un ensemble $V \in \mathcal{V}$ tels que, pour $x \in U, x' \in U, y \in V, y' \in V$, on ait $f(x' - x, y' - y) \in W$. Prenons un point $x_1 \in U$, et un point $y_1 \in V$; quels que soient $x, x'$ dans $U$, et $y, y'$ dans $V$, on aura donc

$$
f(x' - x, y' - y_1) + f(x - x_1, y' - y) \in W + W.
$$

D’autre part, l’application partielle $x \mapsto f(x, y_1)$ est continue dans $A$; il existe donc un ensemble $U' \subset U$, appartenant à $\mathcal{U}$, et tel que, pour $x \in U'$ et $x' \in U'$, on ait $f(x' - x, y_1) \in W$. De même, il existe $V' \subset V$ et appartenant à $\mathcal{V}$ tel que, pour $y \in V'$ et $y' \in V'$, on ait $f(x_1, y' - y) \in W$. Par suite, si $(x, y)$ et $(x', y')$ sont deux points quelconques de $U' \times V'$, on a

$$
f(x', y') - f(x, y) \in W + W + W + W,
$$

ce qui démontre l’existence du prolongement $\bar{f}$ de $f$. Le fait que $\bar{f}$ est **Z-bilinéaire** est une conséquence immédiate du principe de prolongement des identités (I, p. 53, cor. 1).

C.Q.F.D.

Dans l’application de ce théorème à un anneau topologique séparé $A$, on a $E = F = G = \hat{A}, B = A$, et $f$ est l’application **Z-bilinéaire** $(x, y) \mapsto xy$, continue par hypothèse. On désignera encore par $xy$ la valeur de la fonction prolongée dans $\hat{A} \times \hat{A}$; cette fonction est une loi de composition dans $\hat{A}$, et dire qu’elle est **Z-bilinéaire** signifie qu’elle est *distributive* à droite et à gauche par rapport à l’addition; elle est d’autre part *associative* d’après le principe de prolongement des identités. Enfin, pour la même raison, l’élément unité de $A$ est aussi élément unité de $\hat{A}$. Par suite:

#### Proposition 6 {#top-iii-s6-prop-6 .statement}

*Un anneau topologique séparé $A$ est isomorphe à un sous-anneau partout*

$^{1}$ On rappelle (A, II, p. 50) que $f$ est dite **Z-bilinéaire** si, quels que soient les éléments $x, x'$ de $A$, et $y, y'$ de $B$, on a

$$
f(x + x', y) = f(x, y) + f(x', y) \quad \text{et} \quad f(x, y + y') = f(x, y) + f(x, y').
$$

dense d’un anneau séparé et complet $\hat{A}$, déterminé à une isomorphie près (et appelé l’anneau complété de A).

Si A est commutatif il en est de même de $\hat{A}$ (principe de prolongement des identités).

Soient A un anneau topologique non nécessairement séparé, N l’adhérence de 0 dans A, $A' = A/N$ l’anneau séparé associé à A ; l’anneau $\hat{A}'$ complété de A’ s’appelle l’anneau séparé complété de A et se note aussi $\hat{A}$. On démontre comme dans III, p. 25, prop. 8 que tout homomorphisme continu $u$ de A dans un anneau topologique séparé et complet C se factorise de façon unique en $u = v \circ \varphi$, où $v$ est un homomorphisme continu de $\hat{A}$ dans C et $\varphi$ l’application canonique de A dans $\hat{A}$. Si A, B sont deux anneaux topologiques, $u : A \to B$ un homomorphisme continu, il existe donc un homomorphisme continu et un seul $\hat{u} : \hat{A} \to \hat{B}$ tel que le diagramme

$$
\begin{array}{ccc}
A & \xrightarrow{u} & B \\
\downarrow \varphi & & \downarrow \psi \\
\hat{A} & \xrightarrow{\hat{u}} & \hat{B}
\end{array}
$$

soit commutatif ($\varphi$ et $\psi$ étant les applications canoniques) : il suffit en effet d’appliquer à $\psi \circ u$ le résultat précédent.

### 6. Modules topologiques

#### Définition 3 {#top-iii-s6-def-3 .statement}

Étant donné un anneau topologique A, on appelle module topologique à gauche sur A un ensemble E, muni :

1° d’une structure de A-module à gauche ;
2° d’une topologie compatible avec la structure de groupe additif de E et satisfaisant en outre à l’axiome suivant :
(MT) L’application $(\lambda, x) \mapsto \lambda x$ de $A \times E$ dans E est continue.

On définit de la même manière la notion de module topologique à droite sur un anneau topologique A ; comme tout module à droite sur A peut être considéré comme module à gauche sur l’anneau opposé $A^0$, et que la topologie de A est compatible avec la structure d’anneau de $A^0$, il n’y a pas lieu de distinguer les modules topologiques à droite sur A des modules topologiques à gauche sur $A^0$.

#### Exemple 1 {#top-iii-s6-n6-exa-1 .statement}

Un espace vectoriel topologique sur $\mathbf{R}$ (resp. $\mathbf{C}$) est un module topologique sur $\mathbf{R}$ (resp. $\mathbf{C}$) (cf. EVT, I, §1, n° 1).*
2) Soient A un anneau, $\mathcal{B}$ une base de filtre sur A formée d’idéaux bilatères de A, E un A-module à gauche. Si on munit A de la topologie (compatible avec sa structure d’anneau) pour laquelle $\mathcal{B}$ est un système fondamental de voisinages de 0 (III, p. 49, Exemple 3), et E de la topologie (compatible avec sa structure de groupe additif) dont les $aE$, où $a$ parcourt $\mathcal{B}$, forment un système fondamental de voisinages de 0 (III, p. 5, Exemple), on vérifie aussitôt que E est un module topologique sur A.

#### Remarque {#top-iii-s6-n6-rem-1 .statement}

Étant donné un anneau topologique A, considérons sur un A-module à gauche E une topologie compatible avec la structure de groupe additif de E. En vertu de l’identité

$$
\lambda x - \lambda_0 x_0 = (\lambda - \lambda_0)x_0 + \lambda_0(x - x_0) + (\lambda - \lambda_0)(x - x_0)
$$

l’axiome (MT) est équivalent au système des trois axiomes suivants:

(MT$_1'$) Quel que soit $x_0 \in E$, l’application $\lambda \mapsto \lambda x_0$ est continue au point $\lambda = 0$.
(MT$_2'$) Quel que soit $\lambda_0 \in A$, l’application $x \mapsto \lambda_0 x$ est continue au point $x = 0$.
(MT$_3'$) L’application $(\lambda, x) \mapsto \lambda x$ est continue au point $(0, 0)$.

On en déduit un système de conditions nécessaires et suffisantes que doit vérifier le filtre $\mathfrak{V}$ des voisinages de 0 dans un A-module E, pour définir sur E une topologie compatible avec sa structure de module; $\mathfrak{V}$ doit satisfaire aux axiomes (GA$_I$) et (GA$_II$) de III, p. 4, et en outre aux trois axiomes suivants:

(MV$_I$) Quels que soient $x_0 \in E$ et $V \in \mathfrak{V}$, il existe un voisinage S de 0 dans A tel que S.$x_0 \subset V$.
(MV$_II$) Quels que soient $\lambda_0 \in A$ et $V \in \mathfrak{V}$, il existe $W \in \mathfrak{V}$ tel que $\lambda_0 . W \subset V$.
(MV$_III$) Quel que soit $V \in \mathfrak{V}$, il existe $U \in \mathfrak{V}$ et un voisinage T de 0 dans A tels que T.$U \subset V$.

Toute groupe topologique commutatif est un $\mathbf{Z}$-module topologique lorsque l’anneau $\mathbf{Z}$ est muni de la topologie discrète.

Si M est un sous-module d’un module topologique E sur A, il est clair que la topologie induite sur M par celle de E est compatible avec la structure de module de M. En outre, sur le A-module quotient E/M, la topologie quotient de celle de E par M est compatible avec la structure de A-module. Il suffit en effet pour le voir de montrer que l’application $(\lambda, \dot{x}) \mapsto \lambda \dot{x}$ de $A \times (E/M)$ dans $E/M$ est continue (en désignant par $x \mapsto \dot{x}$ l’application canonique de E sur E/M). Or, comme on peut identifier les groupes topologiques additifs $A \times (E/M)$ et $(A \times E)/(\{0\} \times M)$ (III, p. 18, corollaire), il suffit de montrer que l’application $(\lambda, x) \mapsto \lambda \dot{x}$ de $A \times E$ dans $E/M$ est continue, ce qui est immédiat, cette application étant composée de $x \mapsto \dot{x}$ et de $(\lambda, x) \mapsto \lambda x$.

Soit $(E_i)_{i \in I}$ une famille quelconque de modules topologiques sur A, et soit $E = \prod_{i \in I} E_i$ le A-module produit des $E_i$. Sur E la topologie produit est compatible avec la structure de A-module: il suffit de voir que l’application

$$
(\lambda, x) \mapsto (\lambda . \mathrm{pr}_i x)_{i \in I}
$$

de $A \times E$ dans E est continue, ou encore (I, p. 25, prop. 1) que, pour tout indice $\kappa \in I$, $(\lambda, x) \mapsto \lambda . \mathrm{pr}_\kappa x$ est une application continue de $A \times E$ dans $E_\kappa$; or, cette application est composée des applications continues $(\lambda, x_\kappa) \mapsto \lambda x_\kappa$ et $(\lambda, x) \mapsto (\lambda, \mathrm{pr}_\kappa x)$.

Soient A un anneau topologique séparé, E un A-module topologique séparé. Soit $\hat{E}$ le groupe additif complété du groupe topologique commutatif E (III, p. 26, th. 2). L’application $\mathbf{Z}$-bilinéaire $(\lambda, x) \mapsto \lambda x$ du produit $A \times E$ des groupes additifs A, E dans le groupe additif E se prolonge par continuité en une application $\mathbf{Z}$-bilinéaire de $\hat{A} \times \hat{E}$ dans $\hat{E}$ (III, p. 50, th. 1), que nous désignerons encore par $(\lambda, x) \mapsto \lambda x$. En vertu du principe de prolongement des identités, on a encore $\lambda(\mu x) = (\lambda \mu)x$ pour $\lambda \in \hat{A}, \mu \in \hat{A}, x \in \hat{E}$ et $1 \cdot x = x$ pour $x \in \hat{E}$ (en désignant par 1 l’élément unité de $A$) ; la loi externe $(\lambda, x) \mapsto \lambda x$ définit donc sur $\hat{E}$ une structure de $\hat{A}$-module compatible avec la topologie de $\hat{E}$. Nous dirons que le module topologique $\hat{E}$ sur $\hat{A}$ ainsi défini est le complété du module topologique $E$ sur $A$.

Soit $E$ un module topologique sur un anneau topologique $A$, $A$ et $E$ n’étant pas nécessairement séparés. Soit $N$ (resp. $F$) l’adhérence de $\{0\}$ dans $A$ (resp. $E$) ; $N$ est un idéal bilatère de $A$ (III, p. 50, prop. 5) et $F$ un sous-A-module de $E$ (III, p. 45, prop. 1) ; en outre, on a par continuité $\lambda x \in F$ lorsque $\lambda \in N$ ou $x \in F$. On en déduit aussitôt, par passage aux quotients, une application $(\dot{\lambda}, \dot{x}) \mapsto \dot{\lambda} \dot{x}$ de $(A/N) \times (E/F)$ dans $E/F$, et on vérifie (grâce à III, p. 18, corollaire) que cette application est continue, et définit donc sur $E/F$ une structure de module topologique sur l’anneau topologique $A/N$. Si l’on pose $B = A/N, L = E/F$, on dit que le $B$-module $L$ est le module séparé associé à $E$; son complété $\hat{L}$ est un module topologique sur le séparé complété $\hat{A}$ (égal par définition à $\hat{B}$) de $A$ (III, p. 52), qu’on appelle le module séparé complété de $E$ et que l’on note $\hat{E}$. On voit comme dans III, p. 25, prop. 8 que tout homomorphisme continu $u : E \to G$ de $E$ dans un $\hat{A}$-module séparé et complet $G$ se factorise de façon unique en $u = v \circ \varphi$ où $v$ est un homomorphisme continu de $\hat{E}$ dans $G$ et $\varphi$ l’application canonique de $E$ dans $\hat{E}$. On en conclut que si $E, E'$ sont deux $A$-modules topologiques, $u : E \to E'$ un homomorphisme continu, il existe un homomorphisme continu et un seul $\hat{u} : \hat{E} \to \hat{E}'$ tel que le diagramme

$$
\begin{array}{ccc}
E & \xrightarrow{u} & E' \\
\downarrow \varphi & & \downarrow \varphi' \\
\hat{E} & \xrightarrow{\hat{u}} & \hat{E}'
\end{array}
$$

soit commutatif, $\varphi$ et $\varphi'$ étant les applications canoniques.

### 7. Corps topologiques

Dans ce qui suit, et dans les chapitres IV et V, lorsqu’on considérera un corps $K$, on désignera par $K^*$ le groupe multiplicatif des éléments $\neq 0$ de $K$.

#### Définition 4 {#top-iii-s6-def-4 .statement}

On appelle corps topologique un ensemble $K$ muni d’une structure de corps et d’une topologie compatible avec la structure d’anneau de $K$, et satisfaisant en outre à l’axiome suivant:

(KT) L’application $x \mapsto x^{-1}$ de $K^*$ dans $K^*$ est continue.

Une structure de corps et une topologie sur un ensemble $K$ sont dites compatibles, si la structure d’anneau correspondante et la topologie sont compatibles, et si en outre (KT) est vérifié.

#### Exemple 1 {#top-iii-s6-n7-exa-1 .statement}

Sur un corps K, la topologie discrète est compatible avec la structure de corps; un corps topologique dont la topologie est discrète est dit corps discret.
*2) La topologie de la droite rationnelle $\mathbf{Q}$ (resp. de la droite numérique $\mathbf{R}$) est compatible avec la structure de corps de $\mathbf{Q}$ (resp. $\mathbf{R}$; voir IV, p. 10, resp. p. 11).

La déf. 4 montre que, si K est un corps topologique, la topologie induite par celle de K sur le groupe multiplicatif $K^*$ est compatible avec la structure de ce groupe (cf. III, p. 49).

Si $a \neq 0$, les homothéties $x \mapsto ax$ et $x \mapsto xa$ sont des homéomorphismes de K sur lui-même; il en est de même de l’application $x \mapsto ax + b$ quel que soit $b \in K$. On notera que les homothéties $x \mapsto ax$ et $x \mapsto xa$ sont des automorphismes du groupe additif (topologique) de K lorsque $a \neq 0$. Si V est un voisinage quelconque de 0 dans K, $aV$ et $Va$ sont donc des voisinages de 0 quel que soit $a \neq 0$.

Soient E un espace topologique, et $f$ une application de E dans un corps topologique K; si, en un point $x_0 \in E, f$ est continue et $f(x_0) \neq 0, f^{-1}$ est continue en $x_0$. En particulier, si K est commutatif, toute fonction rationnelle de n variables, à coefficients dans K, est continue en tout point de $K^n$ où son dénominateur n’est pas nul.

De même, si $f$ est une application d’un ensemble E filtré par un filtre $\mathfrak{F}$, dans un corps topologique séparé K, et si $\lim_{\mathfrak{F}} f$ existe et est $\neq 0$, $\lim_{\mathfrak{F}} f^{-1}$ existe, et on a
$$
\lim_{\mathfrak{F}} f^{-1} = (\lim_{\mathfrak{F}} f)^{-1}.
$$

Si H est un sous-corps d’un corps topologique K, la topologie induite sur H par celle de K est compatible avec la structure de corps de H: la structure de corps topologique ainsi définie sur H est dite induite par celle de K. En outre, $\overline{H}$ est aussi un sous-corps de K (démonstration analogue à celle de III, p. 50, prop. 5).

Dans un corps topologique K, l’adhérence de l’ensemble réduit à 0 est un idéal bilatère, d’après III, p. 50, prop. 5, donc est nécessairement {0} ou K; autrement dit, si la topologie de K n’est pas la topologie la moins fine (I, p. 11), elle est séparée (III, p. 5, prop. 2).

### 8. Structures uniformes d’un corps topologique

Dans un corps topologique K, il faut distinguer:
1° La structure uniforme du groupe additif de K, définie sur K et dite structure uniforme additive de K.
2° Les structures uniformes droite et gauche du groupe multiplicatif $K^*$, définies sur $K^*$ et dites (par abus de langage) structures uniformes multiplicatives de K.
La structure induite sur $K^*$ par la structure uniforme additive de K est en général distincte des structures uniformes multiplicatives de K (voir III, p. 82, exerc. 17).
D’après la prop. 6 de III, p. 51, un corps topologique séparé K peut être considéré comme sous-anneau partout dense d’un anneau séparé et complet $\hat{K}$. Pour que $\hat{K}$ soit un corps topologique, il faut qu’on puisse prolonger par continuité l’application $x \mapsto x^{-1}$ à $(\hat{K})^*$; et cette condition nécessaire est aussi suffisante, car alors les fonctions $xx^{-1}, x^{-1}x$ et 1 sont égales dans $(\hat{K})^* \times (\hat{K})^*$ d’après le principe de prolongement des identités, ce qui prouve que la valeur, pour tout $x \neq 0$, de la fonction prolongée est bien l’inverse de $x$ dans $\hat{K}$. Autrement dit (cf. II, p. 20, prop. 11):

#### Proposition 7 {#top-iii-s6-prop-7 .statement}

*Pour que l’anneau complété $\hat{K}$ d’un corps topologique séparé $K$ soit un corps topologique, il faut et il suffit que l’image, par l’application $x \mapsto x^{-1}$, de tout filtre de Cauchy (pour la structure additive), auquel 0 n’est pas adhérent, soit encore un filtre de Cauchy (pour la structure additive).*

Il y a des corps topologiques où cette condition n’est pas vérifiée, et où l’anneau $\hat{K}$ admet des diviseurs de 0 (voir III, p. 85, exerc. 26). En outre, lorsque l’anneau complété $\hat{K}$ est un corps topologique, rien n’assure *a priori* que les structures *multiplicatives* de $\hat{K}$ soient des structures d’espace *complet*. Toutefois, il en sera ainsi pour les corps $K$ tels que $\hat{K}$ soit *localement compact* (voir I, p. 66, prop. 13, et III, p. 22, prop. 4), ou *commutatif*; en effet, pour ces derniers, on a la proposition suivante:

#### Proposition 8 {#top-iii-s6-prop-8 .statement}

*Si la structure uniforme additive d’un corps topologique commutatif $K$ est une structure d’espace séparé et complet, la structure multiplicative sur $K^*$ est une structure d’espace complet.*

Nous allons montrer que si $\mathcal{F}$ est un filtre de Cauchy pour la structure *multiplicative* sur $K^*, \mathcal{F}$ est une base de filtre de Cauchy pour la structure *additive* sur $K$, et ne converge pas vers 0, ce qui établira la proposition. Soit $U$ un voisinage quelconque de 0 dans $K$, $V$ un voisinage fermé de 0 tel que $V \subset U, VV \subset U$ (III, p. 49, axiome (AV$_{II}$)) et $-1 \notin V$; il existe par hypothèse un ensemble $A \in \mathcal{F}$ tel que, quels que soient $x \in A, y \in A, x^{-1}y \in 1 + V$. Soit $a$ un point de $A$; on a $A \subset a + aV$, et $a + aV$ est un ensemble fermé ne contenant pas 0, donc 0 n’est pas adhérent à $A$, ni par suite à $\mathcal{F}$. Soit $W$ un voisinage de 0 tel que $aW \subset V$ (III, p. 49, axiome (AV$_{I}$)); il existe par hypothèse un ensemble $B \in \mathcal{F}$ tel que $B \subset A$ et que, quels que soient $x \in B, y \in B$, on ait $x^{-1}y \in 1 + W$, d’où $y - x \subset xW \subset AW \subset aW + aVW$; comme $K$ est commutatif, $aVW = aWV \subset VW \subset U$, donc $y - x \in U + U$, ce qui démontre la proposition.

La même démonstration prouve que la prop. 8 s’étend au cas où tout filtre de Cauchy pour *l’une* des structures multiplicatives de $K$ est aussi un filtre de Cauchy pour l’autre structure multiplicative.

## EXERCICES {#top-iii-s6-exercises}

See the [exercises for § 6](exercises/s6/).
