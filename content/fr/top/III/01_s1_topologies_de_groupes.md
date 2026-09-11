---
book: top
book_title: General Topology
chapter: III
chapter_title: GROUPES TOPOLOGIQUES
section: 1
section_title: Topologies de groupes
lang: fr
source: top-i-iv-fr
pdf_pages: 0184-0189, 0249-0250
extraction: ocr
subsections:
    - "no": 1
      title: Groupes topologiques
      page: 0
      pdf_page: 184
    - "no": 2
      title: Voisinages d’un point dans un groupe topologique
      page: 3
      pdf_page: 186
    - "no": 3
      title: Isomorphismes et isomorphismes locaux
      page: 5
      pdf_page: 188
statements: 11
exercises: 9
content_sha256: 7776acd7bfae78ca9f67e9183ca719fdef316dd21713053f3630629a009ebb09
---

## § 1. TOPOLOGIES DE GROUPES

### 1. Groupes topologiques

#### Définition 1 {#top-iii-s1-def-1 .statement}

On appelle groupe topologique un ensemble G muni d’une structure de groupe et d’une topologie satisfaisant aux deux axiomes suivants :
(GT_I) L’application $(x, y) \mapsto xy$ de $G \times G$ dans $G$ est continue.
(GT_{II}) L’application $x \mapsto x^{-1}$ de $G$ dans $G$ (symétrie du groupe $G$) est continue.

Une structure de groupe et une structure topologique étant données sur un ensemble $G$, on dira qu’elles sont compatibles si elles satisfont à (GT_I) et (GT_{II}).

#### Exemple 1 {#top-iii-s1-n1-exa-1 .statement}

Sur un groupe $G$, la topologie discrète est compatible avec la structure du groupe ; un groupe topologique dont la topologie est discrète est appelé groupe discret.
De même, la topologie la moins fine (I, p. 11) sur $G$ est compatible avec la structure de groupe de $G$.

#### Exemple 2 {#top-iii-s1-n1-exa-2 .statement}

Au chap. IV, on verra que la topologie de la droite rationnelle $\mathbf{Q}$ (resp. de la droite numérique $\mathbf{R}$) est compatible avec la structure de groupe additif de $\mathbf{Q}$ (resp. $\mathbf{R}$).*

#### Exemple 3 {#top-iii-s1-n1-exa-3 .statement}

Si $G$ est un groupe topologique, sa topologie est compatible avec la structure du groupe $G^0$ opposé à $G$ (A, I, p. 2g) ; on dit que $G^0$, muni de cette topologie, est le groupe topologique opposé au groupe topologique $G$.

Les axiomes (GT_I) et (GT_{II}) équivalent au suivant :
(GT'). L’application $(x, y) \mapsto xy^{-1}$ de $G \times G$ dans $G$ est continue.

En effet, $(\mathrm{GT}_I)$ et $(\mathrm{GT}_II)$ entraînent évidemment $(\mathrm{GT}')$. Réciproquement, $(\mathrm{GT}')$ entraîne $(\mathrm{GT}_II)$, car $x \mapsto ex^{-1} = x^{-1}$ est alors continue, et $(\mathrm{GT}')$ et $(\mathrm{GT}_II)$ entraînent $(\mathrm{GT}_I)$, car $(x, y) \mapsto x.(y^{-1})^{-1} = xy$ est alors continue.

Si $a$ est un élément quelconque de $G$, la translation à gauche $x \mapsto ax$ (resp. la translation à droite $x \mapsto xa$) est continue d’après $(\mathrm{GT}_I)$; c’est par suite un homéomorphisme de $G$ sur lui-même. Les applications $x \mapsto axb$ (où $a$ et $b$ parcourent $G$) forment donc un groupe d’homéomorphismes de $G$; les applications $x \mapsto axa^{-1}$ (resp. $x \mapsto ax,\ x \mapsto xa$) où $a$ parcourt $G$, un sous-groupe de ce groupe d’homéomorphismes. De même, comme la symétrie $x \mapsto x^{-1}$ est une permutation involutive de $G$, $(\mathrm{GT}_II)$ montre que cette application est un homéomorphisme de $G$ sur lui-même.

Si $A$ est un ensemble ouvert (resp. fermé) dans $G$, et $x$ un point quelconque de $G$, les ensembles $x.A,\ A.x$ et $A^{-1}$ sont ouverts (resp. fermés)\footnote{On rappelle que, si $A$ et $B$ sont deux parties d’un groupe $G$, $A.B$ ou $AB$ désigne l’ensemble des composés $xy$, où $x$ parcourt $A$ et $y$ parcourt $B$; $A^{-1}$ désigne l’ensemble des éléments $x^{-1}$, où $x$ parcourt $A$. Si $B$ se réduit à un seul élément $x$, on écrit $x.A$ ou $xA$ (resp. $A.x$ ou $Ax$) au lieu de $\{x\}.A$ (resp. $A.\{x\}$).}, car ils sont transformés de $A$ par un des homéomorphismes précédents. Si $A$ est ouvert et $B$ quelconque, $AB$ et $BA$ sont ouverts, comme réunions d’ensembles ouverts (axiome $(O_1)$). Si $V$ est un voisinage de $e$ dans $G$, et $A$ une partie non vide quelconque de $G$, $VA$ et $AV$ sont des voisinages de $A$; en effet, si $W$ est un voisinage ouvert de $e$ contenu dans $V$, $WA$ et $AW$ sont ouverts et contiennent $A$.

Par contre, $AB$ n’est pas nécessairement fermé lorsque $A$ est fermé, même si $B$ est fermé (cf. III, p. 28, cor. 1).

*Par exemple, dans le groupe additif $\mathbf{R}$ de la droite numérique, le sous-groupe $\mathbf{Z}$ des entiers rationnels est fermé, et il en est de même du sous-groupe $\theta\mathbf{Z}$ formé des multiples entiers $n\theta$ d’un nombre *irrationnel* $\theta$; mais le sous-groupe $\mathbf{Z} + \theta\mathbf{Z}$ de $\mathbf{R}$, qui est l’ensemble des nombres réels $m + n\theta$ (où $m$ et $n$ prennent toutes les valeurs entières) n’est pas fermé dans $\mathbf{R}$, comme nous le verrons dans V, §1, no 1.

De même, considérons, dans le groupe additif $\mathbf{R} \times \mathbf{R}$, l’ensemble $A$ des couples $(x, y)$ tels que $x \geq 0,\ 0 \leq y \leq 1 - \frac{1}{x+1}$, et l’ensemble $B$ des couples $(x, 0)$ ($x$ parcourant $\mathbf{R}$); ils sont fermés, mais $A + B$ est l’ensemble des couples $(x, y)$ tels que $0 \leq y < 1$, et n’est pas fermé dans $\mathbf{R} \times \mathbf{R}.*$

Soient $E$ un espace topologique, $f$ et $g$ deux applications de $E$ dans un groupe topologique $G$. Si $f$ et $g$ sont continues en un point $x_0 \in E$, il en est de même\footnote{On rappelle que $f^{-1}$ est l’application $x \mapsto (f(x))^{-1}, fg$ l’application $x \mapsto f(x)g(x)$; on aura soin de ne pas confondre ces applications avec $f^{-1}$ et $f \circ g$ (lorsque ces dernières sont définies) (E, II, p. 17 et p. 16).} de $f^{-1}$ et $fg$, d’après le théorème des fonctions composées (I, p. 10, th. 2); en particulier, les applications continues de $E$ dans $G$ forment un *sous-groupe* du groupe $G^E$ des applications de $E$ dans $G$.

De même, soient $f$ et $g$ deux applications d’un ensemble $E$ *filtré* par un filtre $\mathcal{F}$, dans un groupe topologique *séparé* $G$. Si $\lim_{\mathcal{F}} f$ et $\lim_{\mathcal{F}} g$ existent, il en est de même de $\lim_{\mathcal{F}} f^{-1}$ et $\lim_{\mathcal{F}} fg$, et l’on a (I, p. 50, cor. 1) (1) $\lim_{\mathfrak{F}} f^{-1} = (\lim_{\mathfrak{F}} f)^{-1}$

(2) $\lim_{\mathfrak{F}} fg = (\lim_{\mathfrak{F}} f)(\lim_{\mathfrak{F}} g).$

Lorsque G est un groupe *commutatif*, noté *additivement*, l’axiome (GT’) exprime que $(x, y) \mapsto x - y$ est une application continue. Si $f$ et $g$ sont des applications d’un espace topologique E dans G, continues en $x_0$, $f - g$ est donc continue en ce point. On transcrit de même les formules (1) et (2).

### 2. Voisinages d’un point dans un groupe topologique

Soit $\mathfrak{V}$ le filtre des voisinages de l’élément neutre $e$ dans un groupe topologique G, et soit $a$ un point quelconque de G; puisque $x \mapsto ax$ et $x \mapsto xa$ sont des homéomorphismes, le filtre des voisinages de $a$ est identique à la famille $a.\mathfrak{V}$ des ensembles $a.V$, où V parcourt $\mathfrak{V}$, et aussi à la famille $\mathfrak{V}.a$ des ensembles $V.a$. On connaît donc le filtre des voisinages d’un point *quelconque* d’un groupe topologique quand on connaît le filtre des voisinages de l’élément neutre $e$ du groupe.

Si on exprime que $xy$ et $x^{-1}$ sont continues pour $x = y = e$, on obtient (I, p. 8) les propriétés:

(GV_I) *Quel que soit* $U \in \mathfrak{V}$, *il existe* $V \in \mathfrak{V}$ *tel que* $V.V \subset U$.

(GV_{II}) *Quel que soit* $U \in \mathfrak{V}$, *on a* $U^{-1} \in \mathfrak{V}$.

Tout filtre $\mathfrak{V}$ sur G vérifiant (GV_I) et (GV_{II}) vérifie aussi
(GV_a) *Quel que soit* $U \in \mathfrak{V}$, *il existe* $V \in \mathfrak{V}$ *tel que* $V.V^{-1} \subset U$.
En effet, d’après (GV_I), il existe $W \in \mathfrak{V}$ tel que $W.W \subset U$, et d’après (GV_{II}), il existe $V \in \mathfrak{V}$ tel que $V \subset W \cap W^{-1}$, donc $V^{-1} \subset W$ et par suite
$$ V.V^{-1} \subset W.W \subset U. $$

Inversement, si un filtre $\mathfrak{V}$ sur G vérifie (GV_a) on en déduit en premier lieu que $e$ *appartient à tout ensemble* $U \in \mathfrak{V}$; car si $V \in \mathfrak{V}$ est tel que $V.V^{-1} \subset U$, comme V n’est pas vide, on a, pour tout $x \in V$, $x.x^{-1} = e \in U$. La condition (GV_a) entraîne alors que $V^{-1} \subset V.V^{-1} \subset U$, ce qui prouve que $U^{-1} \in \mathfrak{V}$ pour tout $U \in \mathfrak{V}$. Enfin si $V \in \mathfrak{V}$ est tel que $V.V^{-1} \subset U$, et $W \in \mathfrak{V}$ est tel que $W \subset V \cap V^{-1}$, on a $W.W \subset U$. On voit donc finalement que (GV_a) est *équivalent* à la conjonction de (GV_I) et (GV_{II}).

Enfin, comme $x \mapsto axa^{-1}$ est un homéomorphisme *conservant* $e$, $\mathfrak{V}$ possède la propriété suivante:
(GV_{III}) *Quels que soient* $a \in G$ *et* $V \in \mathfrak{V}$, $a.V.a^{-1} \in \mathfrak{V}$.

Ces trois propriétés du filtre $\mathfrak{V}$ sont caractéristiques. De façon précise:

#### Proposition 1 {#top-iii-s1-prop-1 .statement}

*Soient* G *un groupe*, et $\mathfrak{V}$ *un filtre sur* G *satisfaisant aux axiomes* (GV_I), (GV_{II}) *et* (GV_{III}). *Il existe une topologie et une seule compatible avec la structure de groupe de* G, *et pour laquelle* $\mathfrak{V}$ *est le filtre des voisinages de l’élément neutre* e. *Pour cette topologie, le filtre des voisinages d’un point quelconque* $a \in G$ *est identique à chacun des deux filtres* $a.\mathfrak{V}$ *et* $\mathfrak{V}.a$.

S’il existe une topologie répondant à la question, le filtre des voisinages de $a$ est identique à chacun des deux filtres $a.\mathfrak{V}$ et $\mathfrak{V}.a$ d’après ce qui précède, ce qui montre l’unicité de cette topologie. Son existence sera établie si nous prouvons : 1° que les filtres $a.\mathfrak{V}$ sont les filtres de voisinages d’une topologie sur $G$; 2° que cette topologie est compatible avec la structure de groupe de $G$.

1) Le filtre $a.\mathfrak{V}$ satisfait à l’axiome $(V_{\text{III}})$ (I, p. 3) d’après $(\mathrm{GV}_I)$ et $(\mathrm{GV}_{\text{II}})$, comme on l’a vu ci-dessus; pour voir que c’est le filtre des voisinages de $a$ dans une topologie sur $G$, il faut établir que l’axiome $(V_{\text{IV}})$ est vérifié. Soit donc $V$ un ensemble quelconque de $\mathfrak{V}$, et $W$ un ensemble de $\mathfrak{V}$ tel que $W.W \subset V$; quel que soit $x \in a.W$, on a $x.W \subset a.W.W \subset a.V$, autrement dit, $a.V$ appartient au filtre $x.\mathfrak{V}$, d’où $(V_{\text{IV}})$.

2) Montrons maintenant que la topologie définie par les filtres de voisinages $a.\mathfrak{V}$ satisfait à $(\mathrm{GT}')$. Soient $a$ et $b$ deux points quelconques de $G$; si on pose $x = au, y = bv$, il faut prouver que $xy^{-1}$ est aussi voisin qu’on veut de $ab^{-1}$ dès que $u$ et $v$ sont assez voisins de $e$. Or $(ab^{-1})^{-1}(xy^{-1}) = buv^{-1}b^{-1}$; donnons-nous arbitrairement un voisinage $U$ de $e$; on aura $buv^{-1}b^{-1} \in U$ si $uv^{-1} \in b^{-1}Ub = V$, et $V$ appartient à $\mathfrak{V}$ d’après $(\mathrm{GV}_{\text{III}})$; mais d’après $(\mathrm{GV}_I)$ et $(\mathrm{GV}_{\text{II}})$ il existe $W \in \mathfrak{V}$ tel que $W.W^{-1} \subset V$; il suffira donc de prendre $u \in W,\ v \in W$ pour avoir $xy^{-1} \in (ab^{-1})U$, ce qui achève la démonstration.

Un moyen fréquent de définir une topologie compatible avec une structure de groupe sur $G$ consistera à se donner un filtre satisfaisant aux axiomes $(\mathrm{GV}_I)$, $(\mathrm{GV}_{\text{II}})$ et $(\mathrm{GV}_{\text{III}})$; les conditions correspondantes pour une base de filtre $\mathfrak{B}$ sont les suivantes :

$(\mathrm{GV}'_I)$ *Quel que soit* $U \in \mathfrak{B}$, *il existe* $V \in \mathfrak{B}$ *tel que* $V.V \subset U$.
$(\mathrm{GV}'_{\text{II}})$ *Quel que soit* $U \in \mathfrak{B}$, *il existe* $V \in \mathfrak{B}$ *tel que* $V^{-1} \subset U$.
$(\mathrm{GV}'_{\text{III}})$ *Quels que soient* $a \in G$ *et* $U \in \mathfrak{B}$, *il existe* $V \in \mathfrak{B}$ *tel que* $V \subset a.U.a^{-1}$.

Tout voisinage de $e$ identique à son image par la symétrie $x \mapsto x^{-1}$ est dit *symétrique*; si $V$ est un voisinage quelconque de $e$, $V \cup V^{-1}, V \cap V^{-1}$ et $V.V^{-1}$ sont des voisinages symétriques; d’après $(\mathrm{GV}_{\text{II}})$, les voisinages symétriques forment un *système fondamental de voisinages* de $e$. De même, d’après $(\mathrm{GV}_I)$, lorsque $V$ parcourt un système fondamental de voisinages de $e$, les ensembles $V^n$ (*n* entier fixe $\neq 0$) forment un système fondamental de voisinages de $e$.

#### Remarque {#top-iii-s1-n2-rem-1 .statement}

Lorsque $G$ est *commutatif*, on a $x.A.x^{-1} = A$ pour toute partie $A$ et tout élément $x$ de $G$; la condition $(\mathrm{GV}_{\text{III}})$ (resp. $(\mathrm{GV}'_{\text{III}})$) est automatiquement vérifiée pour tout filtre (resp. toute base de filtre) sur $G$. Au contraire, si $G$ n’est pas commutatif, $(\mathrm{GV}_{\text{III}})$ n’est pas une conséquence de $(\mathrm{GV}_I)$ et $(\mathrm{GV}_{\text{II}})$ (voir III, p. 67, exerc. 5).

Pour un groupe commutatif $G$, écrit *additivement*, les axiomes caractérisant le filtre $\mathfrak{V}$ des voisinages de l’origine dans une topologie compatible avec la structure de groupe de $G$, sont donc les suivants :

$(\mathrm{GA}_I)$ *Quel que soit* $U \in \mathfrak{V}$, *il existe* $V \in \mathfrak{V}$ *tel que* $V + V \subset U$.
$(\mathrm{GA}_{\text{II}})$ *Quel que soit* $U \in \mathfrak{V}$, *on a* $-U \in \mathfrak{V}$.

#### Proposition 2 {#top-iii-s1-prop-2 .statement}

Pour qu’un groupe topologique G soit séparé, il faut et il suffit que l’ensemble {e} soit fermé.

La condition est évidemment nécessaire; inversement, si elle est satisfaite, la diagonale Δ de G × G, image réciproque de l’ensemble {e} par l’application continue (x, y) ↦ xy⁻¹, est un ensemble fermé, donc (I, p. 52, prop. 1) G est séparé.

#### Corollaire {#top-iii-s1-n2-cor-1 .statement}

Pour qu’un groupe topologique G soit séparé, il faut et il suffit que l’intersection des voisinages de e se réduise au point e.

La condition est évidemment nécessaire; inversement, si elle est satisfaite, l’ensemble {e} est fermé: en effet, si x ≠ e, il existe un voisinage V de e tel que x⁻¹ ∉ V, donc e ∉ xV, ce qui montre que x ne peut être adhérent à {e}.

#### Exemple {#top-iii-s1-n2-exa-1 .statement}

Définition d’une topologie de groupe par un ensemble de sous-groupes.

Si 𝒮 est une base de filtre sur un groupe G, formée de sous-groupes de G, il est immédiat qu’elle satisfait aux axiomes (GV₁) et (GV₂), car pour tout sous-groupe H de G, H.H⁻¹ = H. La base de filtre 𝒮 sera donc un système fondamental de voisinages de e dans une topologie compatible avec la structure de groupe de G, pourvu qu’elle satisfasse à (GV₃) (condition qui sera remplie en particulier si tous les sous-groupes de 𝒮 sont distingués, ce qui sera toujours le cas si G est commutatif). Pour que la topologie ainsi définie soit séparée, il faut et il suffit, d’après la prop. 2, que l’intersection des sous-groupes appartenant à 𝒮 se réduise à e. Les cas les plus intéressants sont ceux où le sous-groupe {e} n’appartient pas à 𝒮 (sinon la topologie définie par 𝒮 est la topologie discrète); si cette condition est remplie, la topologie définie par 𝒮 ne peut être séparée que si 𝒮 est un ensemble infini.

L’intersection de deux sous-groupes étant un sous-groupe, on peut définir une topologie de groupe sur G à partir d’un ensemble quelconque 𝒢 de sous-groupes de G; il suffit de considérer l’ensemble 𝒢 des sous-groupes a.H.a⁻¹, où H parcourt 𝒢 et a parcourt G, puis l’ensemble 𝒮 des intersections finies de sous-groupes appartenant à 𝒢; 𝒮 est une base de filtre, et satisfait à (GV₃).

En particulier, considérons le groupe additif d’un anneau A; tout ensemble 𝒢 d’idéaux de A (A, I, p. 98) définit une topologie compatible avec la structure de ce groupe additif; cette topologie est séparée si l’intersection des idéaux de 𝒢 est l’idéal nul; elle est distincte de la topologie discrète si aucune intersection finie d’idéaux de 𝒢 n’est l’idéal nul. Les topologies définies de cette manière jouent un grand rôle en Théorie des nombres (voir les exerc. des §§ 6 et 7 de ce chapitre).

### 3. Isomorphismes et isomorphismes locaux

Conformément aux définitions générales (E, IV, p. 6) un isomorphisme f d’un groupe topologique G sur un groupe topologique G’ est une application bijective de G sur G’ qui est à la fois un isomorphisme de la structure de groupe de G sur celle de G’, et un homéomorphisme de G sur G’. Autrement dit, pour que f soit un isomorphisme de G sur G’, il faut et il suffit que: 1° f soit bijective; 2° quels que soient les points x, y de G, f(xy) = f(x)f(y); 3° f soit bicontinue.

Par exemple, si a est un point quelconque de G, l’application x ↦ axa⁻¹ est un isomorphisme de G sur G, c’est-à-dire (loc. cit.) un automorphisme du groupe topologique G, qu’on appelle automorphisme intérieur.

Si une topologie $\mathcal{T}$ est compatible avec la structure de groupe d’un groupe $G$, et si $G^0$ désigne le groupe topologique obtenu en munissant le groupe opposé de $G$ de la topologie $\mathcal{T}$, la symétrie $x \mapsto x^{-1}$ est un *isomorphisme* du groupe topologique $G$ sur le groupe topologique $G^0$.

#### Définition 2 {#top-iii-s1-def-2 .statement}

*Étant donnés deux groupes topologiques* $G, G'$, *on appelle isomorphisme local de* $G$ *à* $G'$ *un homéomorphisme* $f$ *d’un voisinage* $V$ *de l’élément neutre de* $G$ *sur un voisinage* $V'$ *de l’élément neutre de* $G'$, *satisfaisant aux conditions suivantes*:

$1^\circ$ *Pour tout couple de points* $x, y$ *de* $V$ *tels que* $xy \in V, f(xy) = f(x)f(y)$.

$2^\circ$ *Si* $g$ *est l’application réciproque de* $f$, *pour tout couple de points* $x', y'$ *de* $V'$ *tels que* $x'y' \in V'$, $g(x'y') = g(x')g(y')$.

*L’application* $g$ *est alors un isomorphisme local de* $G'$ *à* $G$.

*On dit que deux groupes topologiques* $G, G'$ *sont localement isomorphes s’il existe un isomorphisme local de* $G$ *à* $G'$.

Deux groupes topologiques isomorphes sont évidemment localement isomorphes; la réciproque est inexacte.

*Par exemple, nous verrons (V, §1, n° 4), que les groupes topologiques* $\mathbf{R}$ *et* $\mathbf{T}$ *sont localement isomorphes, mais non isomorphes.*

Toute *restriction* à un voisinage de l’élément neutre de $G$ d’un isomorphisme local $f$ de $G$ à $G'$, est encore un isomorphisme local de $G$ à $G'$.

Un isomorphisme local de $G$ à $G$ s’appelle encore *automorphisme local* de $G$.

En général, si $f$ est un homéomorphisme d’un voisinage $V$ de l’élément neutre de $G$ sur un voisinage $V'$ de l’élément neutre de $G'$, satisfaisant à la condition $1^\circ$ de la déf. 2, il ne satisfait pas nécessairement à la condition $2^\circ$ (voir III, p. 67, exerc. 7). Toutefois, $G$ et $G'$ sont alors *localement isomorphes*; de façon précise:

#### Proposition 3 {#top-iii-s1-prop-3 .statement}

*Soient* $G$ *et* $G'$ *deux groupes topologiques, et* $f$ *un homéomorphisme d’un voisinage* $V$ *de l’élément neutre de* $G$ *sur un voisinage* $V'$ *de l’élément neutre de* $G'$, *satisfaisant à la condition* $1^\circ$ *de la définition* $2$; $f$ *est alors un prolongement d’un isomorphisme local de* $G$ *à* $G'$.

En effet, on voit sans peine que, si $W$ est un voisinage de l’élément neutre de $G$ tel que $W.W \subset V$, la restriction de $f$ à $W$ est un isomorphisme local de $G$ à $G'$.

## EXERCICES {#top-iii-s1-exercises}

See the [exercises for § 1](exercises/s1/).
