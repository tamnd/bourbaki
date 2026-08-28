---
book: var
book_title: Variétés différentielles et analytiques
chapter: "1"
chapter_title: VARIÉTÉS DIFFÉRENTIELLES ET ANALYTIQUES, FASCICULE DE RÉSULTATS
section: 6
section_title: Fibrations
lang: fr
source: var-fr
pdf_pages: 0059-0067
extraction: ocr
subsections:
    - "no": 1
      title: Fibrations
      page: 0
      pdf_page: 59
    - "no": 2
      title: Fibrations principales
      page: 0
      pdf_page: 60
    - "no": 3
      title: Morphismes de fibrations principales
      page: 0
      pdf_page: 61
    - "no": 4
      title: Construction de fibrations principales au moyen de cocycles
      page: 0
      pdf_page: 63
    - "no": 5
      title: Espaces fibrés associés à une fibration principale
      page: 0
      pdf_page: 64
    - "no": 6
      title: Extension et restriction du groupe structural
      page: 0
      pdf_page: 66
    - "no": 7
      title: Changements de structure
      page: 0
      pdf_page: 67
statements: 0
exercises: 0
content_sha256: 041a801bb9638dc98ed267f9a74ade144cc09841cb4d2f742e4682ab57d1cafb
---

## § 6. Fibrations¹

### 6.1. Fibrations

6.1.1. On appelle fibration de classe $C'$, ou simplement fibration, un triplet $(X, B, \pi)$ où $B$ et $X$ sont des variétés de classe $C'$ et $\pi$ un morphisme de $X$ dans $B$, jouissant de la propriété suivante :

(F) Pour tout $x \in B$, il existe un voisinage ouvert $U$ de $x$, une variété $F$, et un isomorphisme $\varphi$ de $\pi^{-1}(U)$ sur $U \times F$ tel que $\pi(\varphi^{-1}(x, y)) = x$ pour tout $x \in U$ et tout $y \in F$.

Si $\lambda = (X, B, \pi)$ est une fibration, on appelle $X$ l’espace de $\lambda$, $B$ la base de $\lambda$, et $\pi$ la projection de $\lambda$. L’application $\pi$ est une submersion ; en particulier $\pi(X)$ est ouvert dans $B$, et si $R$ désigne la relation d’équivalence définie par $\pi$ dans $X$, l’application canonique de $X/R$ dans $\pi(X)$ est un isomorphisme. Pour tout $x \in B$, l’image réciproque $\pi^{-1}(x)$ est une sous-variété fermée de $X$, appelée la fibre de $x$, et notée $X_x$.

6.1.2. Exemples :
(a) Si $B$ et $F$ sont deux variétés, le triplet $(B \times F, B, pr_1)$ est une fibration dont les fibres sont canoniquement isomorphes à $F$.
(b) Si $\lambda = (X, B, \pi)$ et $\lambda' = (X', B', \pi')$ sont des fibrations,
$$
\lambda \times \lambda' = (X \times X', B \times B', \pi \times \pi')
$$
est une fibration ; on l’appelle le produit de $\lambda$ et de $\lambda'$.
(c) Si $\lambda = (X, B, \pi)$ et $\lambda' = (X', B, \pi')$ sont des fibrations de même base, $\lambda \times_B \lambda' = (X \times_B X', B, \pi \times_B \pi')$ est une fibration ; on l’appelle le produit de $\lambda$ et de $\lambda'$ au-dessus de $B$, ou encore le produit fibré de $\lambda$ et de $\lambda'$.

6.1.3. Soient $\lambda = (X, B, \pi)$ et $\lambda' = (X', B', \pi')$ deux fibrations. On appelle morphisme de $\lambda$ dans $\lambda'$ tout couple $(f, g)$, où $f$ est un morphisme de $B$ dans $B'$, et $g$ un morphisme de $X$ dans $X'$, tel que $\pi' \circ g = f \circ \pi$. Lorsque $B = B'$ et $f = \mathrm{Id}_B$, on dit que $g$ est un $B$-morphisme de $\lambda$ dans $\lambda'$; si $g$ est un isomorphisme de $X$ sur $X'$, $g^{-1}$ est un $B$-morphisme de $\lambda'$ dans $\lambda$, et l’on dit que $g$ est un $B$-isomorphisme de $\lambda$ sur $\lambda'$; pour qu’il en soit ainsi, il faut et il suffit que, pour tout $x \in B$, l’application $g_x : X_x \to X'_x$ induite par $g$ soit un isomorphisme.

¹ Les définitions et la plus grande partie des résultats des §§ 6 et 7 s’appliquent aussi à la catégorie des espaces topologiques ; on doit alors remplacer les mots « variétés », « sous-variétés », « morphismes » et « variétés de groupes » par « espaces topologiques », « sous-espaces topologiques », « applications continues » et « groupes topologiques ». Font exception les résultats concernant les immersions, submersions, et relations d’équivalence régulières, ainsi que ceux des n°s 6.2.3 et 6.2.4 (a).

6.1.4. La fibration $(B \times F, B, pr_1)$ est appelée la fibration *triviale* de base $B$ et de fibre $F$. Un isomorphisme d'une fibration $\lambda$ sur une fibration triviale s'appelle une *trivialisation* de $\lambda$.

6.1.5. Soit $\lambda = (X, B, \pi)$ une fibration, et soit $f : B' \to B$ un morphisme. Soit $\pi'$ le morphisme canonique de $B' \times_B X$ dans $B'$. Le triplet $(B' \times_B X, B', \pi')$ est une fibration, appelée *l'image réciproque de $\lambda$ par $f'$* ou la fibration déduite de $\lambda$ par changement de base de $B$ à $B'$ suivant $f$, et notée $B' \times_B \lambda$, ou encore $f^*\lambda$. Si $f'$ désigne l'application canonique de $B' \times_B X$ dans $X$, le couple $(f, f')$ est un *morphisme* de $B' \times_B \lambda$ dans $\lambda$; il jouit de la propriété universelle suivante: si $(f, g)$ est un morphisme d'une fibration $\lambda'$ de base $B'$ dans la fibration $\lambda$, il existe un $B'$-morphismique unique $\varphi : \lambda' \to B' \times_B \lambda$ tel que $(f, g) = (f, f') \circ \varphi$.

Lorsque $B'$ est une sous-variété de $B$, et $f$ l'injection canonique de $B'$ dans $B$, $B' \times_B X$ s'identifie à la sous-variété $\pi^{-1}(B')$ de $X$, et $\pi'$ s'identifie à la restriction de $\pi$ à $\pi^{-1}(B')$; l'image réciproque de $\lambda$ par $f$ est alors appelée la *fibration induite par $\lambda$ sur $B'$*.

6.1.6. Si $\lambda = (X, B, \pi)$ est une fibration, on appelle *section morphique* (ou simplement *section*) de $\lambda$ tout morphisme $s : B \to X$ tel que $\pi \circ s = \mathrm{Id}_B$.

### 6.2. Fibrations principales

6.2.1. Soient $B$ une variété et $G$ une variété de groupe. On appelle *fibration principale de base $B$ et de groupe structural $G$* un quadruplet $\lambda = (P, G, B, \pi)$ où $P$ est une variété sur laquelle $G$ opère à droite par $(x, g) \mapsto x . g$ (cf. n° 5.12.5), et où $\pi$ est un morphisme de $P$ dans $B$, ces données étant assujetties à vérifier l'axiome suivant:

(P) Pour tout $b \in B$ il existe un voisinage ouvert $U$ de $b$ et un isomorphisme $f : U \times G \to \pi^{-1}(U)$ tels que l'on ait

$$
\pi(f(u, g)) = u \text{ et } f(u, gg') = f(u, g) \cdot g' \text{ si } u \in U \text{ et } g, g' \in G.
$$

6.2.2. Soit $\lambda = (P, G, B, \pi)$ une fibration principale. Le triplet $(P, B, \pi)$ est une fibration; on a $\pi(P) = B$. La relation d'équivalence $R$ définie par $\pi$ dans $P$ coïncide avec celle définie par $G$; son graphe n'est autre que le produit $P \times_B P$ (cf. n° 5.11.2); c'est une sous-variété de $P \times P$. L'application $(x, g) \mapsto (x, x . g)$ est un isomorphisme de $P \times G$ sur $P \times_B P$; l'application qui fait correspondre à tout $(x, y) \in P \times_B P$ l'unique élément $g \in G$ tel que $y = x . g$ est un morphisme de $P \times_B P$ dans $G$.

Le groupe $G$ opère *proprement et librement* sur $P$ (cf. Top. Gén., chap. III, 3e éd., § 4). Si $x \in P$ et si $b = \pi(x)$, l'application $g \mapsto x . g$ est un *isomorphisme de la variété $G$ sur la fibre de $b$*.

6.2.3. Inversement, soit $G$ une variété de groupe, et soit $P$ une variété sur laquelle $G$ opère à droite de façon à vérifier les deux conditions suivantes:
(a) $G$ opère proprement et librement sur $P$.
(b) Pour tout $x \in P$, l’application $g \mapsto x . g$ est une immersion de $G$ dans $P$.

Alors la relation d’équivalence définie par $G$ dans $P$ est régulière; si l’on note $P/G$ la variété quotient, et $\pi$ la projection canonique de $P$ sur $P/G$, le quadruplet $(P, G, P/G, \pi)$ est une fibration principale.
Lorsque $K$ est de caractéristique 0 et que $P$ est de dimension finie, la condition (b) ci-dessus est conséquence de la condition (a).

6.2.4. Les conditions du n° précédent sont vérifiées dans les deux cas suivants:
(a) $P$ est une variété de groupe et $G$ une sous-variété de groupe opérant sur $P$ par les translations à droite; la base de la fibration principale ainsi obtenue est l’espace homogène $P/G$.
(b) $G$ est un groupe discret opérant proprement et librement sur $P$. La projection $\pi : P \to P/G$ est alors un morphisme étale (n° 5.7.6).

6.2.5. Exemples:
(a) Soit $B$ une variété et soit $G$ une variété de groupe. Faisons opérer $G$ sur $B \times G$ par $(b, g) . g' = (b, gg')$. Le quadruplet $(B \times G, G, B, \mathrm{pr}_1)$ est une fibration principale.
(b) Soient $\lambda = (P, G, B, \pi)$ et $\lambda' = (P', G', B', \pi')$ deux fibrations principales. Faisons opérer $G \times G'$ sur $P \times P'$ par la formule:
$$
(x, x') . (g, g') = (x.g, x'.g'), \quad x \in P, x' \in P', g \in G, g' \in G'.
$$
Le quadruplet $\lambda \times \lambda' = (P \times P', G \times G', B \times B', \pi \times \pi')$ est une fibration principale; on l’appelle le produit de $\lambda$ et de $\lambda'$.
(c) Soient $\lambda = (P, G, B, \pi)$ et $\lambda' = (P', G', B, \pi')$ deux fibrations principales de même base. La sous-variété $P \times_B P'$ de $P \times P'$ est stable pour les opérations de $G \times G'$, et le quadruplet
$$
\lambda \times_B \lambda' = (P \times_B P', G \times G', B, \pi \times_B \pi')
$$
est une fibration principale; on l’appelle le produit de $\lambda$ et de $\lambda'$ au-dessus de $B$, ou encore le produit fibré de $\lambda$ et de $\lambda'$.

### 6.3. Morphismes de fibrations principales

6.3.1. Soient $\lambda = (P, G, B, \pi)$ et $\lambda' = (P', G', B', \pi')$ deux fibrations principales. On appelle morphisme de $\lambda$ dans $\lambda'$ tout triplet $(f, \varphi, h)$, où $f : P \to P'$ et $h : B \to B'$ sont des morphismes, $\varphi : G \to G'$ est un homomorphisme de variétés de groupes, et où $\pi' \circ f = h \circ \pi$ et $f(x . g) = f(x) . \varphi(g)$ pour $x \in P, g \in G$. On notera que $f$ détermine $h$; on dira souvent que $(f, \varphi)$, ou même simplement $f$, est un morphisme.

Lorsque $B = B'$ et $h = \mathrm{Id}_B$ (resp. lorsque $G = G'$ et $\varphi = \mathrm{Id}_G$), un morphisme est appelé un $B$-morphisme compatible avec $\varphi$ (resp. un $G$-morphisme compatible avec $h$). Un morphisme qui est à la fois un $B$-morphisme et un $G$-morphisme est appelé un $G$-$B$-morphisme (ici encore, on dit souvent « morphisme » lorsqu’il ne peut y avoir de confusion). Tout $G$-$B$-morphisme $f : P \to P'$ est un isomorphisme de la variété $P$ sur la variété $P'$; l’isomorphisme réciproque $f^{-1}$ est un $G$-$B$-morphisme : $f$ est un $G$-$B$-isomorphisme de $P$ sur $P'$.

Deux espaces fibrés principaux $P$ et $P'$ de même base $B$ et de même groupe structural $G$ sont dits $G$-$B$-isomorphes (ou simplement isomorphes) s’il existe un $G$-$B$-isomorphisme de $P$ sur $P'$.

6.3.2. La fibration principale $(B \times G, G, B, \mathrm{pr}_1)$ est appelée la fibration principale *triviale* de base $B$ et de groupe structural $G$. Un isomorphisme d’une fibration principale $\lambda = (P, G, B, \pi)$ sur la fibration principale triviale de base $B$ et de groupe structural $G$ est appelé une *trivialisation* de $\lambda$. Toute section $s$ de $\lambda$ définit une trivialisation $f_s$ de $\lambda$ par la formule :

$$
f_s^{-1}(b, g) = s(b) \cdot g \quad \text{pour } b \in B \text{ et } g \in G.
$$

On obtient ainsi une *bijection de l’ensemble des sections de $\lambda$ sur l’ensemble des trivialisations de $\lambda$*. De plus, si $s_0$ est une section de $\lambda$, toute section $s$ de $\lambda$ s’écrit de manière unique sous la forme $s(b) = s_0(b) \cdot r(b)$, où $r : B \to G$ est un morphisme.

6.3.3. Soit $\lambda = (P, G, B, \pi)$ une fibration principale, et soit $h : B' \to B$ un morphisme. Soit $\pi'$ (resp. $h'$) le morphisme canonique de $B' \times_B P$ dans $B'$ (resp. dans $P$). Faisons opérer $G$ sur $B' \times_B P$ par la formule

$$
(b', x) \cdot g = (b', x \cdot g), \quad (b', x) \in B' \times_B P, \quad g \in G.
$$

Le quadruplet $(B' \times_B P, G, B', \pi')$ est une fibration principale, appelée *l’image réciproque* de $\lambda$ par $h$, et notée $B' \times_B \lambda$ ou encore $h^* \lambda$. L’application $h' : B' \times_B P \to P$ est un $G$-morphisme compatible avec $h$; il jouit de la propriété universelle suivante : si $f$ est un $G$-morphisme compatible avec $h$ d’une fibration principale $\lambda'$ de base $B'$ dans la fibration $\lambda$, il existe un $G$-$B'$-isomorphisme unique $k : \lambda' \to B' \times_B \lambda$ tel que $f = h' \circ k$.

Lorsque $B'$ est une sous-variété de $B$, et $h$ l’injection canonique de $B'$ dans $B$, $B' \times_B P$ s’identifie à la sous-variété $\pi^{-1}(B')$ de $P$; on l’appelle *l’espace fibré principal induit par $P$ au-dessus de $B'$*, et on le note $\pi^{-1}(B')$, ou encore $P|B'$. Tout $x \in V$ a un voisinage ouvert $U$ tel que $P|U$ soit trivial.

### 6.4. Construction de fibrations principales au moyen de cocycles

Soient B une variété, G une variété de groupe et soit $\mathcal{U} = (U_i)_{i \in I}$ un recouvrement ouvert de B.

6.4.1. On appelle cocycle de classe $C^r$ sur B à valeurs dans G, subordonné à $\mathcal{U}$, une famille $(g_{i,j})_{(i,j) \in I \times I}$ possédant les deux propriétés suivantes:
(1) pour tout couple $(i,j) \in I \times I$, $g_{i,j}$ est une application de classe $C^r$ de l’ouvert $U_i \cap U_j$ de B dans G;
(2) pour tout triplet $(i,j,k) \in I^3$, on a
$$
g_{i,k}(x) = g_{i,j}(x) \cdot g_{j,k}(x) \quad \text{pour tout } x \in U_i \cap U_j \cap U_k.
$$
On dit que deux tels cocycles $(g_{i,j})$ et $(g'_{i,j})$ sont cohomologues s’il existe une famille $(h_i)_{i \in I}$ où, pour tout $i \in I$, $h_i$ est une application de classe $C^r$ de $U_i$ dans G, telle que:
(3)
$$
g'_{i,j}(x) = h_i(x)^{-1} \cdot g_{i,j}(x) \cdot h_j(x) \quad \text{pour tout } x \in U_i \cap U_j.
$$

6.4.2. Soit $\lambda = (P, G, B, \pi)$ une fibration principale. Donnons-nous pour tout $i \in I$ une section $s_i$ de $\lambda$ au dessus de $U_i$ (6.3.3). Pour tout couple $(i,j) \in I^2$, il existe alors un morphisme et un seul $g_{i,j}$ de $U_i \cap U_j$ dans G tel que:
(4)
$$
s_j(b) = s_i(b) \cdot g_{i,j}(b) \quad \text{pour tout } b \in U_i \cap U_j.
$$
La famille des $g_{i,j}$ est un cocycle sur B à valeurs dans G, subordonné au recouvrement ouvert $\mathcal{U}$. Ce cocycle est dit associé à l’objet $(\lambda, \mathcal{U}, (s_i)_{i \in I})$ et les applications $g_{i,j}$ sont appelées les fonctions de transition de cet objet.
Pour $i \in I$, soit $x \mapsto (\pi(x), f_i(x))$ la trivialisation définie par la section $s_i$ de $\lambda|U_i$ (6.3.2). Pour $x \in \pi^{-1}(U_i \cap U_j)$, on a:
(5)
$$
f_i(x) = g_{i,j}(\pi(x)) \cdot f_j(x).
$$

6.4.3. Inversement, soit $g = (g_{i,j})$ un cocycle sur B à valeurs dans G, subordonné au recouvrement $\mathcal{U}$. Il existe alors une fibration principale $\lambda = (P, G, B, \pi)$ et une famille de sections $(s_i)_{i \in I}$ de $\lambda$ au-dessus des $U_i$, telles que la relation (4) soit satisfaite. Il en est alors de même de (5). Si de plus $(\lambda', (s'_i))$ satisfait aux mêmes conditions, il existe un G-B-isomorphisme unique $f$ de $\lambda$ sur $\lambda'$ tel que $s'_i = f \circ s_i$ pour tout $i \in I$. On exprime ce résultat en disant que $(\lambda, (s_i))$ est déterminé à un isomorphisme unique près par le cocycle $g$.

6.4.4. Soient $\lambda = (P, G, B, \pi)$ et $\lambda' = (P', G, B, \pi')$ deux fibrations principales. Soient $(s_i)$ (resp. $(s'_i)$) une famille de sections de $\lambda$ (resp. $\lambda'$) au dessus des $U_i$ et soit $g$ (resp. $g'$) le cocycle associé à $(\lambda, \mathcal{U}, (s_i))$ (resp. $(\lambda', \mathcal{U}, (s'_i))$). Pour que $\lambda$ et $\lambda'$ soient G-B-isomorphes, il faut et il suffit que les cocycles $g$ et $g'$ soient cohomologues. Plus précisément, pour tout G-B-isomorphisme $f$ de $\lambda$ sur $\lambda'$, il existe une famille $(h_i)_{i \in I}$ de morphismes des $U_i$ dans $G$ et une seule telle que la relation (3) soit satisfaite et que l’on ait $f \circ (s'_i(x)) = s_i(x) \cdot h_i(x)$ pour tout $i \in I$ et tout $x \in U_i$, et l’on obtient ainsi une bijection de l’ensemble des G-B-isomorphismes de $\lambda$ sur $\lambda'$ sur l’ensemble des familles $(h_i)_{i \in I}$ satisfaisant à (3).

6.4.5. Reprenons les notations de 6.4.2. et soit $\mathcal{V} = (V_\alpha)_{\alpha \in A}$ un recouvrement ouvert plus fin que le recouvrement ouvert $\mathcal{U}$. Soit $\tau : A \to I$ une application telle que $V_\alpha \subset U_{\tau(\alpha)}$ pour tout $\alpha \in A$. Soit $s'_\alpha$ la restriction à $V_\alpha$ de la section $s_{\tau(\alpha)}$ et soit $g' = (g'_{\alpha,\beta})$ le cocycle subordonné au recouvrement ouvert $\mathcal{V}$ associé à $(\lambda, \mathcal{V}, (s'_\alpha))$. La fonction de transition $g'_{\alpha,\beta}$ est alors la restriction à $V_\alpha \cap V_\beta$ de la fonction de transition $g_{\tau(\alpha), \tau(\beta)}$.

### 6.5. Espaces fibrés associés à une fibration principale

6.5.1. Soit $\lambda = (P, G, B, \pi)$ une fibration principale. Soit F une variété sur laquelle le groupe G opère à gauche ; on note $(g, y) \mapsto g \cdot y$ la loi d’opération de G sur F. Le groupe G opère à droite sur $P \times F$ par la formule $(x, f) \cdot g = (x \cdot g, g^{-1} \cdot f)$; la relation d’équivalence définie par G dans $P \times F$ est régulière ; le quotient $P \times^G F = (P \times F)/G$ est muni d’une structure de variété.

Soit E une variété. On dit que E est muni d’une structure d’espace fibré associé à $\lambda$ de fibre type F lorsqu’on s’est donné un morphisme $\rho : P \times F \to E$ jouissant de la propriété suivante :

(As) On a $\rho(x \cdot g, g^{-1}f) = \rho(x, f)$ pour $x \in P, f \in F, g \in G$, et l’application $\bar{\rho} : P \times^G F \to E$ déduite de $\rho$ par passage au quotient est un isomorphisme de variétés.

Il revient au même de dire que $(P \times F, G, E, \rho)$ est une fibration principale. L’application $\rho$ (ou parfois l’application $\bar{\rho}$) est appelée l’application repère de E, et notée $(x, f) \mapsto x \cdot f$; on a

$$
(x \cdot g) \cdot f = x \cdot (g \cdot f), \quad \text{pour } x \in P, g \in G \text{ et } f \in F.
$$

La donnée de $\lambda$ et de F détermine E à un isomorphisme unique près ; en particulier, on peut prendre pour E la variété $P \times^G F$ elle-même ; on dit que c’est l’espace fibré associé à $\lambda$ de fibre type F, et on le note $\lambda(F)$.

6.5.2. Soit E un espace fibré associé à $\lambda$ et de fibre type F. Il existe un morphisme unique $\pi_E$ de E dans B tel que $\pi_E(x \cdot f) = \pi(x)$ si $x \in P, f \in F$; le triplet $(E, B, \pi_E)$ est une fibration ; si B et F sont séparés, E est séparé.

Soit $b \in B$, et soit $F_b = \pi_E^{-1}(b)$; c’est une sous-variété fermée de E. Si $x \in P$ est tel que $\pi(x) = b$, soit $\theta_x : F \to F_b$ l’application définie par $\theta_x(f) = x \cdot f$; c’est un isomorphisme de variétés. De plus, pour tout $g \in G$, on a $\theta_{x \cdot g} = \theta_x \circ \rho_g$, où $\rho_g$ désigne l’automorphisme $f \mapsto g \cdot f$ de F. Supposons

F muni d'une structure s d'espèce quelconque Σ (cf. Ens., chap. IV, § 1, n° 4) et supposons que s soit invariante par G ; il existe alors sur F_b une structure s_b d'espèce Σ et une seule telle que les $\theta_x : F \to F_b$ soient des isomorphismes ; on l'obtient en transportant s au moyen de l'un des $\theta_x$ (loc. cit., n° 5).

Si s est une section de P au-dessus d'un ouvert U de B, l'application $(b, f) \mapsto s(b) . f$ est un isomorphisme de $U \times F$ sur $\pi_E^{-1}(U)$.

6.5.3. Exemples :
(a) Soit $\lambda = (B \times G, B, pr_1)$, soit $E = B \times F$, et soit
$$
\rho : (B \times G) \times F \to E
$$
l'application $(b, g, f) \mapsto (b, g . f)$. On obtient ainsi sur $B \times F$ une structure d'espace fibré associé à $\lambda$ de fibre type F, qui est dite triviale.

(b) Soient $\lambda = (P, G, B, \pi)$ et $\lambda' = (P', G', B', \pi')$ deux fibrations principales. Soit F (resp. F') une variété sur laquelle G (resp. G') opère à gauche ; et soit E (resp. E') un espace fibré associé à $\lambda$ (resp. à $\lambda'$) de fibre type F (resp. F'). Le groupe $G \times G'$ opère sur $F \times F'$ par $(g . g') . (f, f') = (g . f, g' . f')$. L'application $(P \times P') \times (F \times F') \to E \times E'$ produit des applications repères $P \times F \to E$ et $P' \times F' \to E'$ munit $E \times E'$ d'une structure d'espace fibré associé à $\lambda \times \lambda'$ de fibre type $F \times F'$.

(c) Avec les notations de (b), si l'on suppose que $B' = B$, on définit de même sur $E \times_B E'$ une structure d'espace fibré associé à $\lambda \times_{B'} \lambda'$ de fibre type $F \times F'$.

6.5.4. Les notations étant celles du n° 6.5.1, soit $h : B' \to B$ un morphisme, soit $\lambda' = B' \times_B \lambda$, et soit $E' = E' \times_B E$. Si $P' = B' \times_B P$, définissons une application $P' \times F \to E'$ en posant $(b', x) . f = (b', x . f)$; on munit ainsi $E'$ d'une structure d'espace fibré associé à $\lambda'$ de fibre type F ; on l'appelle l'image réciproque par $h$ de la structure donnée sur $E$.

6.5.5. Soit $\lambda = (P, G, B, \pi)$ une fibration principale, et soit E (resp. E') un espace fibré associé à $\lambda$ de fibre type F (resp. F'). Soit $u : F \to F'$ un morphisme compatible avec les opérations de G (c'est-à-dire tel que $u(g . f) = g . u(f)$ pour $f \in F, g \in G$). Il existe alors un morphisme $\bar{u} : E \to E'$ et un seul tel que l'on ait $\bar{u}(x . f) = x . u(f)$ pour $x \in P, f \in F$. Si $u$ est une immersion (resp. une submersion, une subimmersion), il en est de même de $\bar{u}$.

En particulier, supposons qu'une variété de groupe H opère à droite sur F de telle sorte que $g . (f . h) = (g . f) . h$ pour $g \in G, f \in F, h \in H$. Tout $h \in H$ définit alors un automorphisme $u_h$ de F compatible avec les opérations de G, d'où un automorphisme $\bar{u}_h$ de E ; le groupe H opère à droite sur E par $(y, h) \mapsto \bar{u}_h(y)$.

6.5.6. Soit $\lambda = (P, G, B, \pi)$ une fibration principale, et soit E un espace fibré associé à $\lambda$ de fibre type F. Soit $s : B \to E$ une section de E. Pour tout $x \in P$, il existe un élément unique $\sigma(x) \in F$ tel que $s(\pi(x)) = x . \sigma(x)$. L’application $\sigma : P \to F$ ainsi définie est un morphisme de variétés, et vérifie l’identité:

(*) $$
\sigma(x . g) = g^{-1} . \sigma(x).
$$

L’application $s \mapsto \sigma$ est une bijection de l’ensemble des sections de E sur l’ensemble des morphismes de P dans F qui vérifient l’identité (*).

6.5.7. Soient $\lambda = (P, G, B, \pi)$ et $\lambda' = (P', G, B, \pi')$ deux fibrations principales de même base B et de même groupe structural G. La fibration principale $\lambda \times_B \lambda' = (P \times_B P', G \times G, B, (\pi, \pi')_B)$ a pour groupe structural $G \times G$. Faisons opérer $G \times G$ à gauche sur G par la formule:

$$
(g, g') . g_1 = g . g_1 . {g'}^{-1},
$$

et soit E l’espace fibré associé à $\lambda \times_B \lambda'$ de fibre type G (muni de la loi d’opération définie ci-dessus). Alors les sections de E correspondent bijectivement aux isomorphismes de P sur P’. De façon précise, si s est une section de E correspondant (cf. n° 6.5.6) au morphisme $\sigma : P \times_B P' \to G$, il existe un G-B-isomorphisme $f_s : P \to P'$ et un seul tel que $\sigma(x, f_s(x)) = e$ pour tout $x \in P$; l’application $s \mapsto f_s$ est une bijection de l’ensemble des sections de E sur l’ensemble des G-B-isomorphismes de P sur P’.

### 6.6. Extension et restriction du groupe structural

6.6.1. Soit $\lambda = (P, G, B, \pi)$ une fibration principale, et soit $\varphi$ un homomorphisme de G dans une variété de groupe H. Faisons opérer G à gauche sur H par $g . h = \varphi(g) . h$ et soit $P \times^G H$ l’espace fibré associé à $\lambda$ de fibre type H. Comme les translations à droite dans H sont compatibles avec les opérations de G, le groupe H opère à droite sur $P \times^G H$ (cf. n° 6.5.5); si $\pi_H$ désigne la projection de $P \times^G H$ sur B, le quadruplet $(P \times^G H, H, B, \pi_H)$ est une fibration principale, notée $\varphi(\lambda)$; on dit qu’elle se déduit de $\lambda$ par l’homomorphisme $\varphi$.

L’application f de P dans $P \times^G H$ qui associe à $x \in P$ la classe de $(x, e)$ est un B-morphisme de P dans $P \times^G H$ compatible avec $\varphi$ (cf. n° 6.3.1). De plus, si $f'$ est un B-morphisme de P dans un espace fibré principal $P'$ de groupe structural H, et si $f'$ est compatible avec $\varphi$, il existe un H-B-isomorphisme unique $\theta$ de $P \times^G H$ sur $P'$ tel que $f' = \theta \circ f$.

6.6.2. Supposons que $\lambda$ soit définie au moyen d’un recouvrement ouvert $\mathcal{V} = (U_i)$ de B et d’un cocycle $(g_{ij})$ (6.4.2). Alors $\varphi(\lambda)$ peut être défini au moyen du même recouvrement et du cocycle $(h_{ij})$, avec $h_{ij} = \varphi \circ g_{ij}$.

6.6.3. Soit F une variété sur laquelle le groupe H opère à gauche; on note $(h, y) \mapsto h . y$ la loi d’opération de H sur F. Le groupe G opère sur F par $(g, y) \mapsto \varphi(g) . y$. Soit E un espace fibré associé à $\varphi(\lambda)$ de fibre type F. L’application $(x, y) \mapsto f(x) . y$ de $P \times F$ dans E (l’application $f$ étant celle définie au n° 6.6.1) munit E d’une structure d’espace fibré associé à $\lambda$ de fibre type F. En particulier, $(P \times^G H) \times^H F$ s’identifie à $P \times^G F$.

6.6.4. Supposons que G soit une sous-variété de groupe de H, et que $\varphi : G \to H$ soit l’injection canonique de G dans H. On dit alors que $\varphi(\lambda)$ se déduit de $\lambda$ par extension à H du groupe structural. Le morphisme $f : P \to P \times^G H$ du n° 6.6.1 est un isomorphisme de P sur une sous-variété fermée de $P \times^G H$ (égale à $P \times^G H$ si $G = H$); cet isomorphisme est compatible avec les opérations de G (noter que G opère sur $P \times^G H$ comme sous-groupe de H).

6.6.5. Supposons encore que G soit une sous-variété de groupe de H, et soit $\mu = (Q, H, B, \pi)$ une fibration principale de groupe structural H et de base B, et soit E un espace fibré associé à $\mu$ de fibre type $H/G$. Si $\gamma$ désigne la projection canonique de H sur $H/G$, posons $\delta(y) = y . \gamma(e)$, pour $y \in Q$ (où $e$ désigne l’élément neutre de H); on obtient ainsi un morphisme $\delta : Q \to E$ et le quadruplet $(Q, G, E, \delta)$ est une fibration principale. En particulier, $Q/G$ s’identifie canoniquement à E, lui-même isomorphe à $Q \times^H H/G$ $^{1}$.

Soit maintenant $s : B \to E$ une section de E, et soit $\lambda_s$ l’image réciproque par $s$ de la fibration $(Q, G, E, \delta)$ que l’on vient de définir. C’est une fibration principale, de base B et de groupe structural G et son extension à H est isomorphe à $\mu$; tout fibration jouissant de ces propriétés peut être obtenue ainsi, à un isomorphisme près; deux sections $s_1$ et $s_2$ de E définissent des fibrations isomorphes si et seulement si elles sont transformées l’une de l’autre par un H-B-automorphisme de $\mu$.

### 6.7. Changements de structure

Les structures et opérations décrites dans ce paragraphe sont compatibles avec les changements de structure décrits aux numéros 5.13 et 5.14.

$^1$ Dans le cas topologique (cf. note $^1$, page 61), il est nécessaire de supposer que les translations à droite par les éléments de G font de H un espace fibré principal de groupe structural G, de base $H/G$; cela revient à dire qu’il y a un ouvert non vide de $H/G$ au-dessus duquel la projection $H \to H/G$ admet une section continue. Dans la catégorie des variétés, la condition analogue est toujours satisfaite (cf. n° 6.2.4).
