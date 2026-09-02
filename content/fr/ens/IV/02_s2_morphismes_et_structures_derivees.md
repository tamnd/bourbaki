---
book: ens
book_title: Theory of Sets
chapter: IV
chapter_title: STRUCTURES
section: 2
section_title: Morphismes et structures dérivées
lang: fr
source: ens-i-iv-fr
source_edition: 2006, Springer
book_pages: E IV.11-E IV.22
pdf_pages: 0214-0225, 0231-0234
extraction: ocr
subsections:
    - "no": 1
      title: Morphismes
      page: 11
      pdf_page: 214
    - "no": 2
      title: Structures plus fines
      page: 12
      pdf_page: 215
    - "no": 3
      title: Structures initiales
      page: 14
      pdf_page: 217
    - "no": 4
      title: Exemples de structures initiales
      page: 15
      pdf_page: 218
    - "no": 5
      title: Structures finales
      page: 19
      pdf_page: 222
    - "no": 6
      title: Exemples de structures finales
      page: 21
      pdf_page: 224
statements: 12
exercises: 11
content_sha256: cbee7ac8bfe2385e96af2a4e38f0596ab864675d5768a0895ec35c072202c5da
---

## § 2. MORPHISMES ET STRUCTURES DÉRIVÉES

### 1. Morphismes

Pour simplifier, nous supposerons, dans ce paragraphe et le suivant, que les espèces de structure dont il est question ne comportent qu'un seul ensemble de base (nécessairement principal); le lecteur étendra sans peine les définitions et résultats au cas général.

Soient $\Sigma$ une espèce de structure dans une théorie $\mathcal{T}$ plus forte que la théorie des ensembles, $x, y, s, t$ quatre lettres distinctes entre elles et distinctes des constantes de $\Sigma$; rappelons que la notation $\mathcal{F}(x; y)$ désigne l'ensemble des applications de $x$ dans $y$ (II, p. 31). Supposons donné un terme $\sigma\{x, y, s, t\}$ de $\mathcal{T}$, vérifiant les conditions suivantes:

(MO_I) *La relation*
« $s$ est une structure d'espèce $\Sigma$ sur $x$ et $t$ est une structure d'espèce $\Sigma$ sur $y$ » entraîne, dans $\mathcal{T}$, la relation $\sigma\{x, y, s, t\} \subset \mathcal{F}(x; y)$.

(MO_{II}) *Si, dans une théorie $\mathcal{T}'$ plus forte que $\mathcal{T}$, $E, E', E''$ sont trois ensembles munis de structures $\mathcal{S}, \mathcal{S}', \mathcal{S}''$ d'espèce $\Sigma$, les relations $f \in \sigma\{E, E', \mathcal{S}, \mathcal{S}'\}$ et $g \in \sigma\{E', E'', \mathcal{S}', \mathcal{S}''\}$ entraînent la relation $g \circ f \in \sigma\{E, E'', \mathcal{S}, \mathcal{S}''\}$.

(MO_{III}) *Étant donnés, dans une théorie $\mathcal{T}'$ plus forte que $\mathcal{T}$, deux ensembles $E, E'$ munis de structures $\mathcal{S}, \mathcal{S}'$ d'espèce $\Sigma$, pour qu'une bijection $f$ de $E$ sur $E'$ soit un isomorphisme, il faut et il suffit que l'on ait $f \in \sigma\{E, E', \mathcal{S}, \mathcal{S}'\}$ et $f^{-1} \in \sigma\{E', E, \mathcal{S}', \mathcal{S}\}$.

Lorsque $\Sigma$ et $\sigma$ sont donnés, on exprime la relation $f \in \sigma\{x, y, s, t\}$ en disant que $f$ est un morphisme (ou un $\sigma$-morphisme) de $x$, muni de $s$, dans $y$, muni de $t$; si (dans une théorie $\mathcal{T}'$ plus forte que $\mathcal{T}$) $E, E'$ sont deux ensembles munis de structures $\mathcal{S}, \mathcal{S}'$ d'espèce $\Sigma$, le terme $\sigma\{E, E', \mathcal{S}, \mathcal{S}'\}$ est l'ensemble des $\sigma$-morphismes de $E$ dans $E'$.

#### Exemple 1 {#ens-iv-s2-n1-exa-1 .statement tag=03VL}

Prenons pour $\Sigma$ l'espèce de structure d'ordre et pour $\sigma\{x, y, s, t\}$ l'ensemble des applications $f$ de $x$ dans $y$ telles que la relation $(u, v) \in s$ entraîne (f(u), f(v)) \in t. Avec les notations de III, p. 4, cela signifie encore que $u \leq v$ entraîne $f(u) \leq f(v)$, c'est-à-dire que $f$ est croissante (III, p. 7). La vérification des axiomes (MO_I), (MO_{II}) et (MO_{III}) est immédiate.

#### Exemple 2 {#ens-iv-s2-n1-exa-2 .statement tag=03VM}

Prenons pour $\Sigma$ une espèce de structure algébrique comportant une seule loi de composition (interne) (IV, p. 5, Exemple 2). Soient A, A' deux ensembles munis de structures d'espèce $\Sigma$, et soient $p, p'$ les lois de composition de ces deux structures. Considérons les applications $f$ de A dans A' telles que l'on ait $p'(f(x), f(y)) = f(p(x, y))$ pour $x \in A$ et $y \in A$; ces applications vérifient (MO_I), (MO_{II}) et (MO_{III}); on les appelle homomorphismes de A dans A'.

#### Exemple 3 {#ens-iv-s2-n1-exa-3 .statement tag=03VN}

Prenons pour $\Sigma$ l'espèce de structure topologique (IV, p. 5, Exemple 3). Soient A, A' deux ensembles munis de topologies V, V' respectivement; considérons les applications $f$ de A dans A' telles que la relation $X' \in V'$ entraîne $f^{-1}(X') \in V$ (autrement dit, l'image réciproque par $f$ de tout ensemble ouvert pour $V'$ doit être ouvert pour $V$); on dit que ces applications, qui satisfont à (MO_I), (MO_{II}) et (MO_{III}), sont les applications continues de A dans A' pour les topologies V et V', (cf. TG, I, § 2).

#### Remarque {#ens-iv-s2-n1-rem-1 .statement tag=03VO}

Pour une espèce de structure donnée $\Sigma$, on a souvent l'occasion de définir divers termes $\sigma x, y, s, t$ qui satisfont aux conditions (MO_I), (MO_{II}) et (MO_{III}). Par exemple, pour l'espèce $\Sigma$ de structure topologique, on dit (avec les notations de l'exemple précédent) qu'une application $f$ de A dans A' est ouverte si la relation $X \in V$ entraîne $f(X) \in V'$ (autrement dit, si l'image par $f$ de tout ensemble ouvert est un ensemble ouvert). On constate aisément que les applications ouvertes satisfont aussi aux conditions (MO_I), (MO_{II}) et (MO_{III}) pour l'espèce $\Sigma$; *en outre, on peut montrer qu'une application continue n'est pas nécessairement ouverte, et qu'une application ouverte n'est pas nécessairement continue.* La donnée d'une espèce de structure $n'implique donc pas$ une notion de morphisme bien déterminée.

Pour les structures d'ordre, les structures algébriques et les structures topologiques, il sera toujours sous-entendu que les morphismes sont ceux qui ont été définis dans les exemples ci-dessus, sauf mention expresse du contraire.

La condition (MO_{III}) et la caractérisation des bijections (II, p. 18, corollaire) entraînent le critère suivant:
CST8. Soient E, E' deux ensembles munis chacun d'une structure d'espèce $\Sigma$. Soit $f$ un $\sigma$-morphisme de E dans E', g un $\sigma$-morphisme de E' dans E. Si $g \circ f$ est l'application identique de E sur lui-même, et $f \circ g$ l'application identique de E' sur lui-même, $f$ est un isomorphisme de E sur E', et g est l'isomorphisme réciproque.

On notera qu'une bijection de E sur E' peut être un $\sigma$-morphisme sans que son application réciproque soit un $\sigma$-morphisme. *Par exemple, une application bijective d'un espace topologique A dans un espace topologique A' peut être continue sans que son application réciproque le soit (TG, I, § 2, n° 1, Remarque 3).*

#### Remarque {#ens-iv-s2-n1-rem-2 .statement tag=03VP}

Lorsqu'une espèce de structure $\Sigma$ comporte plusieurs ensembles de base principaux $x_1, \ldots, x_n$, et des ensembles de base auxiliaires $A_1, \ldots, A_m$, un $\sigma$-morphisme est un système $(f_1, \ldots, f_n)$, où $f_i$ est une application de $x_i$ dans $y_i$ ($1 \leq i \leq n$), ces systèmes d'applications vérifiant des conditions analogues à (MO_{II}) et (MO_{III}), que le lecteur énoncera aisément.

### 2. Structures plus fines

Dans tout le reste de ce paragraphe, nous supposerons données une espèce de structure $\Sigma$ et une notion de $\sigma$-morphisme relative à cette espèce de structure;

toutes les notions qui vont être introduites dépendent, non seulement de $\Sigma$, mais aussi de la notion de $\sigma$-morphisme envisagée. Nous dirons d’ordinaire « morphisme » pour « $\sigma$-morphisme ».

Soient E un ensemble, $\mathcal{S}_1$ et $\mathcal{S}_2$ deux structures d’espèce $\Sigma$ sur E. On dit que la structure $\mathcal{S}_1$ est plus fine que $\mathcal{S}_2$ (ou que $\mathcal{S}_2$ est moins fine que $\mathcal{S}_1$) si l’application identique de E, muni de $\mathcal{S}_1$, sur E, muni de $\mathcal{S}_2$, est un morphisme.

Si cela est nécessaire pour éviter des confusions, on dira que $\mathcal{S}_1$ est plus fine que $\mathcal{S}_2$ relativement à la notion de $\sigma$-morphisme considérée; de même pour toutes les notions qui vont être définies dans ce paragraphe.

Supposons que $\mathcal{S}_1$ soit plus fine que $\mathcal{S}_2$; si E′ est un ensemble muni d’une structure $\mathcal{S}'$ d’espèce $\Sigma$, et si f est un morphisme de E, muni de $\mathcal{S}_2$, dans E′, muni de $\mathcal{S}'$, alors f est aussi un morphisme de E, muni de $\mathcal{S}_1$, dans E′, muni de $\mathcal{S}'$: cela résulte de la définition précédente et de (MO$_{\text{II}}$). De même, si g est un morphisme de E′, muni de $\mathcal{S}'$, dans E, muni de $\mathcal{S}_1$, g est aussi un morphisme de E′, muni de $\mathcal{S}'$, dans E, muni de $\mathcal{S}_2$.

En termes plus imagés, plus une structure (d’espèce $\Sigma$) sur E est fine, plus il y a de morphismes dont E est l’ensemble de départ, et moins il y a de morphismes dont E est l’ensemble d’arrivée.

La relation « $\mathcal{S}_1$ est moins fine que $\mathcal{S}_2$ » est une relation d’ordre entre $\mathcal{S}_1$ et $\mathcal{S}_2$ dans l’ensemble des structures d’espèce $\Sigma$ sur E: elle est en effet réflexive d’après (MO$_{\text{III}}$), transitive d’après (MO$_{\text{II}}$), et si une structure d’espèce $\Sigma$ est à la fois plus fine et moins fine qu’une autre, elle lui est identique en vertu de (MO$_{\text{III}}$). Conformément aux définitions générales (III, p. 13), on dit que deux structures d’espèce $\Sigma$ sur E sont comparables si l’une est plus fine que l’autre; on dit qu’une structure est strictement plus fine (resp. strictement moins fine) qu’une autre si elle est plus fine (resp. moins fine) que cette dernière et en est distincte.

#### Exemple 1 {#ens-iv-s2-n2-exa-1 .statement tag=03VQ}

Pour qu’une structure d’ordre de graphe s sur un ensemble A soit plus fine qu’une structure d’ordre de graphe s′, il faut et il suffit que $s \subset s'$. Autrement dit, la relation $x \leq y$ pour s entraîne $x \leq y$ pour s′; on retrouve la définition donnée dans III, p. 6, Exemple 3.

#### Exemple 2 {#ens-iv-s2-n2-exa-2 .statement tag=03VR}

Considérons deux structures algébriques F, F′ de même espèce $\Sigma$ sur un ensemble A, F et F′ étant les graphes des lois de composition de ces deux structures. D’après la définition des morphismes dans ce cas (IV, p. 12, Exemple 2), dire que F est plus fine que F′ signifie que $F \subset F'$. Mais comme F et F′ sont des graphes fonctionnels ayant tous deux le même ensemble de définition $A \times A$, on a nécessairement $F = F'$. Autrement dit, deux structures comparables d’espèce $\Sigma$ sont nécessairement identiques.

#### Exemple 3 {#ens-iv-s2-n2-exa-3 .statement tag=03VS}

Soient V, V′ deux topologies sur un même ensemble A. Dire que V est plus fine que V′ signifie, en vertu de la définition des morphismes (IV, p. 12, Exemple 3) que $V' \subset V$; en d’autres termes, toute partie de A qui est un ensemble ouvert pour V′ est aussi un ensemble ouvert pour V (ou, de façon plus imagée, plus une topologie est fine, plus il y a d’ensembles ouverts).

#### Remarque {#ens-iv-s2-n2-rem-1 .statement tag=03VT}

Nous venons de voir un exemple (Exemple 2) où deux structures comparables de même espèce $\Sigma$ sont nécessairement identiques. On rencontre de nombreux exemples de telles structures: structures d’ordre total, *topologies d’espace compact, structures d’espace de Fréchet (les morphismes étant les applications linéaires continues), topologies définies par une valeur absolue (ou une valuation) sur un corps, etc.*

Pour une telle espèce de structure $\Sigma$, un morphisme $f$ de $E$ dans $E'$ qui est une application *bijective* est un *isomorphisme*: car en transportant par $f$ la structure $\mathcal{S}$ de $E$, on obtient une structure d’espèce $\Sigma$ plus fine que la structure $\mathcal{S}'$ de $E'$, donc qui est nécessairement identique à cette dernière.

### 3. Structures initiales

Considérons une famille $(A_i)_{i \in I}$ d’ensembles, dont chacun est muni d’une structure $\mathcal{S}_i$ d’espèce $\Sigma$. Soit d’autre part $E$ un ensemble, et, pour chaque $i \in I$, soit $f_i$ une application *de E dans $A_i$*. On dit qu’une structure $\mathcal{I}$ d’espèce $\Sigma$ sur $E$ est *structure initiale pour la famille* $(A_i, \mathcal{S}_i, f_i)_{i \in I}$ si elle possède la propriété suivante:

(IN) Quels que soient l’ensemble $E'$, la structure $\mathcal{S}'$ d’espèce $\Sigma$ sur $E'$ et l’application $g$ *de E' dans E*, la relation

« $g$ est un morphisme de $E'$ dans $E$ »

est *équivalente* à la relation

« quel que soit $i \in I$, $f_i \circ g$ est un morphisme de $E'$ dans $A_i$ ».

CST9. *S’il existe, sur E, une structure initiale pour la famille* $(A_i, \mathcal{S}_i, f_i)_{i \in I}$ *elle est la moins fine des structures d’espèce* $\Sigma$ *sur E pour lesquelles chacune des applications* $f_i$ *est un morphisme, et par suite est unique*.

En effet, soit $\mathcal{I}$ une structure initiale sur $E$, et $\mathcal{S}$ une structure d’espèce $\Sigma$ sur $E$, pour laquelle chacune des $f_i$ est un morphisme. Désignant par $i$ l’application identique de $E$, muni de $\mathcal{S}$, sur $E$, muni de $\mathcal{I}$, on peut encore dire que $f_i \circ i$ est un morphisme pour tout $i \in I$; la condition (IN) montre que $i$ est un morphisme, ce qui signifie (IV, p. 13) que $\mathcal{S}$ est *plus fine* que $\mathcal{I}$. D’autre part, en appliquant (IN) au cas où $g$ est l’application identique de $E$ (muni de $\mathcal{I}$) sur lui-même, on voit (en vertu de (MO$_{\text{III}}$)) que chacune des $f_i$ est un morphisme de $E$ dans $A_i$, ce qui prouve le critère.

Il peut se faire qu’il existe une structure d’espèce $\Sigma$ sur $E$ qui soit la moins fine de toutes les structures d’espèce $\Sigma$ pour lesquelles les $f_i$ sont des morphismes, mais que cette structure ne soit pas la structure initiale pour $(A_i, \mathcal{S}_i, f_i)$ (IV, p. 30, exerc. 6).

On a le *critère de transitivité* suivant:

CST10. *Soient E un ensemble, $(A_i)_{i \in I}$ une famille d’ensembles, et pour chaque* $i \in I$, *soit* $\mathcal{S}_i$ *une structure d’espèce* $\Sigma$ *sur* $A_i$. *Soit* $(J_\lambda)_{\lambda \in L}$ *une partition de* $I$, *et soit* $(B_\lambda)_{\lambda \in L}$ *une famille d’ensembles ayant* $L$ *comme ensemble d’indices*. *Enfin, pour tout* $\lambda \in L$, *soit* $h_\lambda$ *une application de* $E$ *dans* $B_\lambda$; *pour tout* $\lambda \in L$ *et tout* $i \in J_\lambda$, *soit* $g_{\lambda i}$ *une application de* $B_\lambda$ *dans* $A_i$; *on pose alors* $f_i = g_{\lambda i} \circ h_\lambda$ (fig. 1). *On suppose que, pour tout* $\lambda \in L$, *il existe une structure initiale* $\mathcal{S}'_\lambda$ *sur* $B_\lambda$, *pour la famille* $(A_i, \mathcal{S}_i, g_{\lambda i})_{i \in J_\lambda}$. *Dans ces conditions, les propositions suivantes sont équivalentes*:

a) *il existe une structure initiale* $\mathcal{I}$ *sur* $E$ *pour la famille* $(A_i, \mathcal{S}_i, f_i)_{i \in I}$;

b) il existe une structure initiale $\mathcal{J}'$ sur E pour la famille $(B_\lambda, \mathcal{S}'_\lambda, h_\lambda)_{\lambda \in L}$. En outre, ces propositions entraînent que $\mathcal{J} = \mathcal{J}'$.

En effet, soit F un ensemble muni d'une structure d'espèce $\Sigma$, et soit $u$ une application de F dans E. Remarquons que, par définition, la relation

« $h_\lambda \circ u$ est un morphisme de F dans $B_\lambda$ »

est équivalente à la relation

« quel que soit $t \in J_\lambda$, $g_{\lambda t} \circ h_\lambda \circ u = f_t \circ u$ est un morphisme de F dans $A_t$ ».

![Diagramme commutatif montrant les relations entre E, B_\lambda, A_t, et les morphismes h_\lambda, g_{\lambda t}, f_t](Fig. 1)

La relation
(1) « quel que soit $\lambda \in L$, $h_\lambda \circ u$ est un morphisme de F dans $B_\lambda$ »
est donc équivalente à la relation
(2) « quel que soit $t \in I$, $f_t \circ u$ est un morphisme de F dans $A_t$ ».
Or, dire que $\mathcal{J}'$ est structure initiale pour la famille $(B_\lambda, \mathcal{S}'_\lambda, h_\lambda)_{\lambda \in L}$ signifie que la relation (1) est équivalente à la relation

« $u$ est un morphisme de F dans E muni de $\mathcal{J}'$ »;

et dire que $\mathcal{J}$ est structure initiale pour la famille $(A_t, \mathcal{S}_t, f_t)_{t \in I}$ signifie que la relation (2) est équivalente à la relation

« $u$ est un morphisme de F dans E muni de $\mathcal{J}$ »;

d'où le critère, compte tenu de la propriété d'unicité de la structure initiale.

### 4. Exemples de structures initiales

I: Image réciproque d'une structure. — Lorsque I est un ensemble à un seul élément, la structure initiale pour le seul triplet $(A, \mathcal{S}, f)$ est appelée (lorsqu'elle existe) image réciproque par $f$ de la structure $\mathcal{S}$.

*Une topologie admet toujours une image réciproque par une application quelconque $f$; mais il n'en est pas ainsi pour une structure d'ordre ou une structure algébrique.*

II: Structure induite. — Soient A un ensemble muni d'une structure $\mathcal{S}$ d'espèce $\Sigma$, B une partie de A, $j$ l'injection canonique de B dans A. On appelle structure induite par $\mathcal{S}$ sur B l'image réciproque (si elle existe) de la structure $\mathcal{S}$ par l'injection $j$.

Une structure d'ordre induit une structure de même espèce sur toute partie de l'ensemble où elle est définie; il n'en est pas de même d'une structure d'ensemble ordonné filtrant. *Une topologie induit une topologie sur toute partie de l'ensemble où elle est définie; mais une topologie d'espace compact n'induit pas en général une topologie d'espace compact. Sur une partie quelconque B d'un ensemble A muni d'une structure algébrique, cette structure n'induit pas en général une structure de même espèce; lorsque la structure donnée sur A comporte des lois de composition, il est nécessaire que B soit stable pour chacune de ces lois, mais cette condition n'est pas toujours suffisante (cf. A, I, § 4, no 3).*

Le critère général CST10 donne pour les structures induites le critère de transitivité:

CST11. Soient B une partie de A, C une partie de B, $\mathcal{S}$ une structure d'espèce $\Sigma$ sur A, induisant sur B une structure $\mathcal{S}'$ de même espèce. Pour que $\mathcal{S}$ induise sur C une structure d'espèce $\Sigma$, il faut et il suffit que $\mathcal{S}'$ induise sur C une structure d'espèce $\Sigma$, et les structures induites par $\mathcal{S}$ et $\mathcal{S}'$ sur C sont alors identiques.

CST12. Soient A, A' deux ensembles munis de structures $\mathcal{S}$, $\mathcal{S}'$ d'espèce $\Sigma$, B une partie de A, B' une partie de A'. On suppose que $\mathcal{S}$ (resp. $\mathcal{S}'$) induit une structure d'espèce $\Sigma$ sur B (resp. B'). Alors, si f est un morphisme de A dans A', tel que $f(B) \subset B'$, l'application g de B dans B', qui coïncide avec f dans B, est un morphisme (pour les structures induites par $\mathcal{S}$ et $\mathcal{S}'$).

En effet, soit $j$ (resp. $j'$) l'injection canonique de B (resp. B') dans A (resp. A'). Par définition, on a $f \circ j = j' \circ g$; comme $f$ et $j$ sont des morphismes, il en est de même de $f \circ j$ en vertu de (MO_{II}); mais alors, $j' \circ g$ étant un morphisme, il en est de même de $g$, par définition de la structure induite.

III: Structure produit. — Soit $(A_i)_{i \in I}$ une famille d'ensembles, et sur chaque ensemble $A_i$, soit $\mathcal{S}_i$ une structure d'espèce $\Sigma$; soit $E = \prod_{i \in I} A_i$ l'ensemble produit de la famille $(A_i)_{i \in I}$ (II, p. 32), et soit pr_i la projection de E sur $A_i$. On appelle structure produit des structures $\mathcal{S}_i$ la structure initiale (si elle existe) pour la famille $(A_i, \mathcal{S}_i, \mathrm{pr}_i)_{i \in I}$.

Une famille de structures d'ordre admet toujours une structure produit, mais non une famille de structures d'ordre total. *Une famille de structures de groupe admet toujours une structure produit, mais non une famille de structures de corps. Une famille de topologies admet toujours une structure produit, mais non une famille de topologies d'espace localement compact. Pour cette dernière espèce de structure, on notera qu'il y a une structure produit de même espèce sur tout produit d'une famille finie d'espaces localement compacts, mais pas toujours sur un produit d'une famille infinie de tels espaces (cf. TG, I, § 9, no 7, prop. 14).*

Le critère CST10 donne pour les structures produits le critère d'associativité:

CST13. Soit $(A_i)_{i \in I}$ une famille d'ensembles, et pour chaque $i \in I$, soit $\mathcal{S}_i$ une structure d'espèce $\Sigma$ sur $A_i$. Soit $(J_\lambda)_{\lambda \in L}$ une partition de $I$. On suppose que sur chaque produit partiel $B_\lambda = \prod_{i \in J_\lambda} A_i$ la famille $(\mathcal{S}_i)_{i \in J_\lambda}$ admette une structure produit $\mathcal{S}'_\lambda$. Alors, pour que la famille $(\mathcal{S}_i)_{i \in I}$ admette une structure produit $\mathcal{S}$, il faut et il suffit que la famille $(\mathcal{S}'_\lambda)_{\lambda \in L}$ admette une structure produit $\mathcal{S}'$, et l'application canonique de $E = \prod_{i \in I} A_i$ muni de $\mathcal{S}$, sur $F = \prod_{\lambda \in L} B_\lambda$ muni de $\mathcal{S}'$ (II, p. 35) est un isomorphisme.

Une autre application de CST10 donne le critère suivant, relatif aux structures induites par une structure produit:

CST14. Soit $(A_i)_{i \in I}$ une famille d'ensembles, et pour chaque $i \in I$, soit $\mathcal{S}_i$ une structure d'espèce $\Sigma$ sur $A_i$. Pour chaque $i \in I$, soit $B_i$ une partie de $A_i$. On suppose que chaque $\mathcal{S}_i$ induise sur $B_i$ une structure $\mathcal{S}'_i$ et que sur le produit $E = \prod_{i \in I} A_i$ il existe une structure $\mathcal{S}_0$ produit de la famille $(\mathcal{S}_i)$. Dans ces conditions, les propositions suivantes sont équivalentes:

a) sur l'ensemble $B = \prod_{i \in I} B_i \subset E$ il existe une structure $\mathcal{S}$ induite par $\mathcal{S}_0$;
b) sur l'ensemble $B$, il existe une structure $\mathcal{S}'$ produit de la famille de structures $(\mathcal{S}'_i)$.
En outre, ces propositions entraînent que $\mathcal{S} = \mathcal{S}'$.

En effet, soient $j_i$ l'injection canonique de $B_i$ dans $A_i$, $j$ l'injection canonique de $B$ dans $E$, $p_i$ la projection de $E$ sur $A_i$, $p'_i$ la projection de $B$ sur $B_i$; on a $p_i \circ j = j_i \circ p'_i$ pour tout $i \in I$. D'après CST10, $\mathcal{S}$ est la structure initiale pour la famille $(A_i, \mathcal{S}_i, p_i \circ j)_{i \in I}$ et $\mathcal{S}'$ est la structure initiale pour la famille $(A_i, \mathcal{S}_i, j_i \circ p'_i)_{i \in I}$. D'où le critère.

Les notions d'image réciproque et de structure produit sont liées par le critère suivant:

CST15. Soit $(A_i)_{i \in I}$ une famille d'ensembles, et pour chaque $i \in I$, soient $\mathcal{S}_i$ une structure d'espèce $\Sigma$ sur $A_i$, et $f_i$ une application d'un ensemble $E$ dans $A_i$. On suppose qu'il existe sur l'ensemble produit $A = \prod_{i \in I} A_i$ une structure produit $\mathcal{S}$ de la famille $(\mathcal{S}_i)$. Alors, pour qu'il existe une structure initiale pour la famille $(A_i, \mathcal{S}_i, f_i)_{i \in I}$, il faut et il suffit qu'il existe une structure image réciproque de $\mathcal{S}$ par l'application $x \mapsto f(x) = (f_i(x))$ de $E$ dans $A$, et ces deux structures sont identiques.

Comme $f_i = \mathrm{pr}_i \circ f$, ce critère est un cas particulier de CST10.

#### Remarque {#ens-iv-s2-n4-rem-1 .statement tag=03VU}

Soit $(\mathcal{S}_\lambda)_{\lambda \in L}$ une famille de structures d'espèce $\Sigma$ sur un même ensemble $A$; désignons par $A_\lambda$ l'ensemble $A$ muni de la structure $\mathcal{S}_\lambda$, et par $\mathrm{Id}_\lambda$ l'application identique de $A$ dans $A_\lambda$. Soient $B$ l'ensemble produit $A^L = \prod_{\lambda \in L} A_\lambda$, $\Delta$ la diagonale de ce produit (II, p. 33), et $h$ l'application diagonale de $A$ sur $\Delta$, $h(x)$ étant donc l'élément $(x_\lambda)_{\lambda \in L}$ tel que $x_\lambda = x$ pour tout $\lambda \in L$. Supposons qu'il existe sur $B$ la structure produit $\mathcal{S}'$ de la famille $(\mathcal{S}_\lambda)$; comme $h$ est injective, le critère CST15 montre que, pour qu'il existe une structure initiale $\mathcal{S}$ pour la famille $(A_\lambda, \mathcal{S}_\lambda, \mathrm{Id}_\lambda)_{\lambda \in L}$, il faut et il suffit qu'il existe sur $\Delta$ une structure $\mathcal{S}''$ induite par $\mathcal{S}'$; $\mathcal{S}''$ est alors transportée de $\mathcal{S}$ par $h$. En particulier, lorsque toutes les structures $\mathcal{S}_\lambda$ sont identiques, $h$ est un *isomorphisme* de $A$ (muni de cette structure) sur $\Delta$.

On a aussi le critère suivant:

**CST16.** *Soient* $(A_i)_{i \in I}, (B_i)_{i \in I}$ *deux familles d'ensembles ayant même ensemble d'indices. Pour tout* $i \in I$, *soient* $\mathcal{S}_i$ *une structure d'espèce* $\Sigma$ *sur* $A_i$, $\mathcal{S}'_i$ *une structure d'espèce* $\Sigma$ *sur* $B_i$. *Supposons qu'il existe sur* $A = \prod_{i \in I} A_i$ *(resp. $B = \prod_{i \in I} B_i$) la structure produit* $\mathcal{S}$ *(resp. $\mathcal{S}'$) de la famille* $(\mathcal{S}_i)$ *(resp. $(\mathcal{S}'_i)$). Enfin, pour tout* $i \in I$, *soit* $f_i$ *un morphisme de* $A_i$ *dans* $B_i$; *alors, l'application* $f = (f_i)_{i \in I}$ *est un morphisme de* $A$ *dans* $B$.

En effet, soit $p_i$ (resp. $q_i$) la projection de $A$ sur $A_i$ (resp. de $B$ sur $B_i$); on a $q_i \circ f = f_i \circ p_i$. Comme $f_i$ et $p_i$ sont des morphismes (critère CST9), il en est de même de $f_i \circ p_i$ d'après (MO$_{\text{II}}$), donc $f$ est un morphisme en vertu de la condition (IN).

#### Remarque {#ens-iv-s2-n4-rem-2 .statement tag=03VV}

Pour la plupart des structures usuelles, la condition énoncée dans CST16 est non seulement suffisante, mais aussi nécessaire pour que $f$ soit un morphisme (cf. IV, p. 30, exerc. 7). Il en est ainsi en particulier dans les circonstances suivantes (qui sont vérifiées, par exemple, lorsque $\Sigma$ est l'espèce de structure d'ordre, *ou l'espèce de structure de groupe ou l'espèce de structure topologique*, etc.; cf. IV, p. 30, exerc. 8):
Il existe une famille $(a_i)_{i \in I}$ telle que $a_i \in A_i$ pour tout $i \in I$ et telle que, si on pose $r_i(x_i) = (y_\kappa)$, avec $y_i = x_i, y_\kappa = a_\kappa$ pour $\kappa \neq i$, chacune des applications $r_i$ soit un *morphisme* de $A_i$ dans $A$.
En effet, si $f = (f_i)$ est un morphisme de $A$ dans $B$, on peut écrire $f_i = q_i \circ f \circ r_i$ pour tout $i \in I$, et il suffit d'appliquer (MO$_{\text{II}}$).
On notera que $r_i$ est un morphisme lorsque la condition suivante est vérifiée:
$a)$ Pour tout ensemble $E$ muni d'une structure d'espèce $\Sigma$, l'application constante $z \mapsto a_i$ est un morphisme de $E$ dans $A_i$. En effet, pour tout $\kappa \in I$, $p_\kappa \circ r_i$ est alors un morphisme de $A_i$ dans $A_\kappa$, puisque cette application est l'identité pour $\kappa = i$, et une application constante $z \mapsto a_\kappa$ pour $\kappa \neq i$; par définition de la structure produit, $r_i$ est donc un morphisme de $A_i$ dans $A$.
Les exemples cités ci-dessus vérifient, non seulement $a)$, mais aussi la condition:
$b)$ sur chaque ensemble $A'_i = A_i \times \prod_{\kappa \neq i} \{a_\kappa\}$, la structure $\mathcal{S}$ induit une structure d'espèce $\Sigma$.
Soit $p'_i$ la restriction de $p_i$ à $A'_i$; lorsque les conditions $a)$ et $b)$ sont vérifiées, $p'_i$ est un *isomorphisme* de $A'_i$ sur $A_i$. En effet, comme $p'_i = p_i \circ j_i$, où $j_i$ est l'injection canonique de $A'_i$ dans $A$, $p'_i$ est un morphisme en vertu de (MO$_{\text{II}}$). D'autre part, on a $r_i = j_i \circ p'_i$, donc $p'_i$ est un morphisme de $A_i$ dans $A'_i$ en vertu de la définition de la structure induite.

On a enfin le critère suivant, qui caractérise les morphismes dans de nombreux cas:

**CST17.** *Soient* $A$ *et* $B$ *deux ensembles, munis de structures* $\mathcal{S}_A, \mathcal{S}_B$ *de même espèce* $\Sigma$. *On suppose qu'il existe sur* $A \times B$ *la structure* $\mathcal{S}_{A \times B}$, *produit de* $\mathcal{S}_A$ *et de* $\mathcal{S}_B$. *Soient* $f$ *une application de* $A$ *dans* $B$, $F$ *son graphe, $\pi$ l'application bijective* $x \mapsto (x, f(x))$ *de* $A$ *sur* $F$. *Pour que* $f$ *soit un morphisme de* $A$ *dans* $B$, *il faut et il suffit qu'il existe sur* $F$ *une structure d'espèce* $\Sigma$ *induite par* $\mathcal{S}_{A \times B}$, *et que lorsqu'on munit* $F$ *de cette structure, $\pi$ soit un isomorphisme de* $A$ *sur* $F$.

La condition est suffisante; en effet, si $j$ est l'injection canonique de $F$ dans $A \times B$, on peut écrire $f = pr_2 \circ j \circ \pi$, et $f$ est alors par hypothèse le composé de trois morphismes.

Montrons que la condition est nécessaire; désignons par $\mathcal{S}_F$ la structure d'espèce $\Sigma$ transportée de $\mathcal{S}_A$ par la bijection $\pi$ (IV, p. 7); tout revient à prouver que $\mathcal{S}_F$ est induite sur $F$ par $\mathcal{S}_{A \times B}$. Pour cela, remarquons d'abord que $j$ est un morphisme de $F$ dans $A \times B$: il suffit en effet, par définition de la structure $\mathcal{S}_F$, de prouver que $j \circ \pi$ est un morphisme de $A$ dans $A \times B$; mais $j \circ \pi$ n'est autre que l'application $x \mapsto (x, f(x))$ de $A$ dans $A \times B$, qui est un morphisme en vertu de l'hypothèse sur $f$ et de la définition de la structure produit. Reste à montrer que si $E$ est un ensemble muni d'une structure d'espèce $\Sigma$, $g$ une application de $E$ dans $F$ telle que $j \circ g$ soit un morphisme de $E$ dans $A \times B$, alors $g$ est un morphisme, ou, ce qui revient au même, que $g_1 = \pi^{-1} \circ g$ est un morphisme de $E$ dans $A$; mais comme $g_1 = pr_1 \circ (j \circ g)$, cela résulte de l'hypothèse et de la définition de la structure produit.

### 5. Structures finales

Considérons une famille $(A_i)_{i \in I}$ d'ensembles, dont chacun est muni d'une structure $\mathcal{S}_i$ d'espèce $\Sigma$. Soit d'autre part $E$ un ensemble, et, pour chaque $i \in I$, soit $g_i$ une application de $A_i$ dans $E$. On dit qu'une structure $\mathcal{F}$ d'espèce $\Sigma$ sur $E$ est structure finale pour la famille $(A_i, \mathcal{S}_i, g_i)_{i \in I}$ si elle possède la propriété suivante:

(FI) Quels que soient l'ensemble $E'$, la structure $\mathcal{S}'$ d'espèce $\Sigma$ sur $E'$, et l'application $f$ de $E$ dans $E'$, la relation

« $f$ est un morphisme de $E$ dans $E'$ »

est équivalente à la relation

« quel que soit $i \in I$, $f \circ g_i$ est un morphisme de $A_i$ dans $E'$ ».

CST18. S'il existe sur $E$ une structure finale pour la famille $(A_i, \mathcal{S}_i, g_i)_{i \in I}$, elle est la plus fine des structures d'espèce $\Sigma$ sur $E$ pour lesquelles chacune des applications $g_i$ est un morphisme, et par suite est unique.

En effet, soient $\mathcal{F}$ une structure finale sur $E$, et $\mathcal{S}$ une structure d'espèce $\Sigma$ sur $E$, pour laquelle chacune des $g_i$ soit un morphisme. Désignant par $i$ l'application identique de $E$, muni de $\mathcal{F}$, sur $E$, muni de $\mathcal{S}$, on peut encore dire que $i \circ g_i$ est un morphisme pour tout $i \in I$; la condition (FI) montre que $i$ est un morphisme, ce qui signifie (IV, p. 13) que $\mathcal{S}$ est moins fine que $\mathcal{F}$. D'autre part, en appliquant (FI) au cas où $f$ est l'application identique de $E$ (muni de $\mathcal{F}$) sur lui-même, on voit (en vertu de (MOIII)) que chacune des $g_i$ est un morphisme de $A_i$ dans $E$, ce qui prouve le critère.

Il peut se faire qu'il existe une structure d'espèce $\Sigma$ sur $E$ qui soit la plus fine de toutes les structures d'espèce $\Sigma$ pour lesquelles les $g_i$ sont des morphismes, mais que cette structure ne soit pas structure finale pour $(A_i, \mathcal{S}_i, g_i)$ (IV, p. 30, exerc. 6).

On a le critère de transitivité suivant:

CST19. Soient E un ensemble, $(A_i)_{i \in I}$ une famille d'ensembles, et pour chaque $i \in I$, soit $\mathcal{S}_i$ une structure d'espèce $\Sigma$ sur $A_i$. Soit $(J_\lambda)_{\lambda \in L}$ une partition de $I$, et soit $(B_\lambda)_{\lambda \in L}$ une famille d'ensembles ayant $L$ comme ensemble d'indices. Enfin, pour tout $\lambda \in L$, soit $h_\lambda$ une application de $B_\lambda$ dans $E$; pour tout $\lambda \in L$ et tout $i \in J_\lambda$, soit $g_{i\lambda}$ une application de $A_i$ dans $B_\lambda$; on pose alors $f_i = h_\lambda \circ g_{i\lambda}$ (fig. 2). On suppose que, pour tout $\lambda \in L$, il existe une structure finale $\mathcal{S}'_\lambda$ sur $B_\lambda$, pour la famille $(A_i, \mathcal{S}_i, g_{i\lambda})_{i \in J_\lambda}$. Dans ces conditions, les propositions suivantes sont équivalentes:
a) il existe une structure finale $\mathcal{F}$ sur $E$ pour la famille $(A_i, \mathcal{S}_i, f_i)_{i \in I}$;
b) il existe une structure finale $\mathcal{F}'$ sur $E$ pour la famille $(B_\lambda, \mathcal{S}'_\lambda, h_\lambda)_{\lambda \in L}$.
En outre, ces propositions entraînent que $\mathcal{F} = \mathcal{F}'$.

![Diagramme montrant les applications entre ensembles et structures](../images/structure_transitivite.png)

Fig. 2

En effet, soit $F$ un ensemble muni d'une structure d'espèce $\Sigma$, et soit $u$ une application de $E$ dans $F$. Par définition, la relation

« $u \circ h_\lambda$ est un morphisme de $B_\lambda$ dans $F$ »

est équivalente à la relation

« quel que soit $i \in J_\lambda$, $u \circ h_\lambda \circ g_{i\lambda} = u \circ f_i$ est un morphisme de $A_i$ dans $F$ ».

La relation

(3) « quel que soit $\lambda \in L$, $u \circ h_\lambda$ est un morphisme de $B_\lambda$ dans $F$ »

est donc équivalente à la relation

(4) « quel que soit $i \in I$, $u \circ f_i$ est un morphisme de $A_i$ dans $F$ ».

Or, dire que $\mathcal{F}'$ est structure finale pour la famille $(B_\lambda, \mathcal{S}'_\lambda, h_\lambda)_{\lambda \in L}$ signifie que la relation (3) est équivalente à la relation

« $u$ est un morphisme de $E$ (muni de $\mathcal{F}'$) dans $F$ » et dire que $\mathcal{F}$ est structure finale pour la famille $(A_i, \mathcal{S}_i, f_i)_{i \in I}$ signifie que la relation (4) est équivalente à la relation

« $u$ est un morphisme de $E$ (muni de $\mathcal{F}$) dans $F$ »;

d’où le critère, compte tenu de la propriété d’unicité de la structure finale.

### 6. Exemples de structures finales

I : Image directe d’une structure. — Lorsque $I$ est un ensemble à un seul élément, la structure finale pour le seul triplet $(A, \mathcal{S}, f)$ est appelée (lorsqu’elle existe) image directe par $f$ de la structure $\mathcal{S}$.

II : Structure quotient. — Soient $A$ un ensemble muni d’une structure $\mathcal{S}$ d’espèce $\Sigma$, $R$ une relation d’équivalence dans $A$, et soit $\varphi$ l’application canonique de $A$ sur l’ensemble quotient $E = A/R$ (II, p. 41). On appelle structure quotient de $\mathcal{S}$ par la relation $R$ l’image directe (si elle existe) de la structure $\mathcal{S}$ par l’application $\varphi$.

\* En général, une structure d’ordre ou une structure algébrique n’admettent pas de structure quotient pour une relation d’équivalence quelconque (cf. III, p. 69, exerc. 2). Par contre une topologie admet toujours une structure quotient pour une relation d’équivalence arbitraire, mais il n’en est pas de même d’une structure d’espace topologique séparé.*

Soient $A, B$ deux ensembles munis respectivement de structures $\mathcal{S}, \mathcal{S}'$ d’espèce $\Sigma$, et soit $f$ un morphisme de $A$ dans $B$. Soient $R$ la relation d’équivalence $f(x) = f(y)$, $\varphi$ l’application canonique de $A$ sur $A/R$, et $j$ l’injection canonique de $f(A)$ dans $B$. Supposons que $\mathcal{S}$ admette une structure quotient $\mathcal{S}_0$ par $R$, et que $\mathcal{S}'$ induise une structure $\mathcal{S}'_0$ sur $f(A)$. Alors, dans la décomposition canonique $f = j \circ g \circ \varphi$ de $f$ (II, p. 44), la bijection $g$ de $A/R$ sur $f(A)$, associée à $f$, est un morphisme (mais non nécessairement un isomorphisme), lorsqu’on munit $A/R$ de $\mathcal{S}_0$ et $f(A)$ de $\mathcal{S}'_0$. En effet, $j \circ g$ est un morphisme de $A/R$ dans $B$, par définition de la structure quotient, et $g$ un morphisme de $A/R$ sur $f(A)$, par définition de la structure induite.

CST20. Soient $A, A'$ deux ensembles munis de structures $\mathcal{S}, \mathcal{S}'$ d’espèce $\Sigma$, $R$ une relation d’équivalence dans $A$, $R'$ une relation d’équivalence dans $A'$. On suppose qu’il existe une structure quotient $\mathcal{S}_0$ de $\mathcal{S}$ par $R$, et une structure quotient $\mathcal{S}'_0$ de $\mathcal{S}'$ par $R'$. Alors, si $f$ est un morphisme de $A$ dans $A'$, compatible avec les relations $R$ et $R'$ (II, p. 44), et $g$ l’application obtenue par passage aux quotients, $g$ est un morphisme de $A/R$ dans $A'/R'$.

En effet, si $\varphi$ est l’application canonique de $A$ sur $A/R$, $\varphi'$ l’application canonique de $A'$ sur $A'/R'$, on a $g \circ \varphi = \varphi' \circ f$; comme $\varphi'$ et $f$ sont des morphismes, il en est de même de $\varphi' \circ f$ en vertu de (MO$_{\text{II}}$); mais alors, $g \circ \varphi$ étant un morphisme, il en est de même de $g$, par définition de la structure quotient.

Le critère de transitivité CST19 donne en particulier le critère suivant:

CST21. Soient $A$ un ensemble muni d'une structure $\mathcal{S}$ d'espèce $\Sigma$, $R$ une relation d'équivalence dans $A$, telle qu'il existe sur $A/R$ une structure quotient $\mathcal{S}'$ de $\mathcal{S}$ par $R$. Soit $S$ une relation d'équivalence dans $A$, moins fine que $R$, et soit $S/R$ la relation d'équivalence dans $A/R$, quotient de $S$ par $R$ (II, p. 46). Pour qu'il existe sur $(A/R)/(S/R)$ une structure quotient $\mathcal{S}''$ de $\mathcal{S}'$ par $S/R$, il faut et il suffit qu'il existe sur $A/S$ une structure quotient $\mathcal{S}_0$ de $\mathcal{S}$ par $S$, et l'application canonique de $A/S$ (muni de $\mathcal{S}_0$) sur $(A/R)(S/R)$ (muni de $\mathcal{S}''$) est alors un isomorphisme.

En effet, soient $\varphi$ l'application canonique de $A$ sur $A/R$, $\psi$ celle de $A/R$ sur $(A/R)/(S/R)$. En vertu de CST19, dire que $\mathcal{S}''$ est structure quotient de $\mathcal{S}'$ par $S/R$ équivaut à dire que $\mathcal{S}''$ est structure finale pour le triplet $(A, \mathcal{S}, \psi \circ \varphi)$. Le critère résulte alors de ce que la relation $\psi(\varphi(x)) = \psi(\varphi(y))$ est équivalente à $S$.

#### Remarque {#ens-iv-s2-n6-rem-1 .statement tag=03VW}

Soient $A$ un ensemble muni d'une structure $\mathcal{S}$ d'espèce $\Sigma$, $R$ une relation d'équivalence dans $A$ telle qu'il existe sur $E = A/R$ une structure quotient $\mathcal{S}'$ de $\mathcal{S}$ par $R$. Soit $\varphi$ l'application canonique de $A$ sur $E$; en général, il n'existe pas de section $s$ associée à $\varphi$ (II, p. 18) qui soit un morphisme de $E$ dans $A$. Supposons qu'une telle section $s$ existe, et en outre qu'il existe une structure $\mathcal{S}''$ induite par $\mathcal{S}$ sur $s(E)$; alors, en désignant par $j$ l'injection canonique de $s(E)$ dans $A$, et en posant $s = j \circ f$, l'application bijective $f$ est un isomorphisme de $E$ sur $s(E)$. En effet, $f$ est un morphisme par définition de la structure induite, et $g = \varphi \circ j$ est un morphisme de $s(E)$ sur $E$ en raison de (MO_{II}); comme $g \circ f$ est l'application identique de $E$ et $f \circ g$ l'application identique de $s(E)$, la conclusion résulte du critère CST8.

## EXERCICES {#ens-iv-s2-exercises}

See the [exercises for § 2](exercises/s2/).
