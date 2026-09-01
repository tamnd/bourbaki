---
book: top
book_title: General Topology
chapter: IX
chapter_title: UTILISATION DES NOMBRES RÉELS EN TOPOLOGIE GÉNÉRALE
section: 6
section_title: Espaces polonais ; espaces sousliniens ; ensembles boréliens
lang: fr
source: top-v-x-fr
book_pages: TG IX.117-TG IX.125
pdf_pages: 0177-0194, 0237-0245
extraction: ocr
subsections:
    - "no": 1
      title: Espaces polonais
      page: 0
      pdf_page: 177
    - "no": 2
      title: Espaces sousliniens
      page: 59
      pdf_page: 179
    - "no": 3
      title: Ensembles boréliens
      page: 60
      pdf_page: 180
    - "no": 4
      title: Espaces éparpillés et espaces lusiniens
      page: 62
      pdf_page: 182
    - "no": 5
      title: Cribles
      page: 63
      pdf_page: 183
    - "no": 6
      title: Séparation des ensembles sousliniens
      page: 65
      pdf_page: 185
    - "no": 7
      title: Espaces lusiniens et ensembles boréliens
      page: 66
      pdf_page: 186
    - "no": 8
      title: Le théorème du graphe souslinien
      page: 69
      pdf_page: 189
    - "no": 9
      title: Sections boréliennes
      page: 70
      pdf_page: 190
    - "no": 10
      title: Capacitabilité des ensembles sousliniens
      page: 72
      pdf_page: 192
statements: 61
exercises: 22
content_sha256: 40c1604d7c2b11988ff1aec3e8859fb7bb9f1bdf6357bf484c3494bbfd9d4487
---

## § 6. ESPACES POLONAIS ; ESPACES SOUSLINIENS ; ENSEMBLES BORÉLIENS

### 1. Espaces polonais

#### Définition 1 {#top-ix-s6-def-1 .statement}

On dit qu’un espace topologique $X$ est polonais s’il est métrisable de type dénombrable (IX, p. 18), et s’il existe une distance compatible avec la topologie de $X$, pour laquelle $X$ soit complet.

#### Proposition 1 {#top-ix-s6-prop-1 .statement}

a) Tout sous-espace fermé d’un espace polonais est polonais.
    b) Le produit d’une famille dénombrable d’espaces polonais est polonais.
    c) La somme d’une famille dénombrable d’espaces polonais est un espace polonais.

En effet, tout sous-espace d’un espace métrisable de type dénombrable est métrisable de type dénombrable, et tout sous-espace fermé d’un espace complet est complet (II, p. 16, prop. 8). Tout produit dénombrable d’espaces métrisables de type dénombrable est métrisable de type dénombrable (IX, p. 19), et tout produit dénombrable d’espaces métriques complets est un espace métrique complet pour une distance compatible avec sa topologie (II, p. 17, prop. 10 et IX, p. 15, cor. 2). Enfin, soit $(X_n)$ une suite d’espaces polonais non vides, et soit $X$ l’espace somme des $X_n$; on peut supposer la topologie de $X_n$ définie par une distance $d_n \leq 1$ pour laquelle $X_n$ est complet et de type dénombrable (IX, p. 3); on définit alors la topologie de $X$ par la distance $d$ telle que $d(x, y) = d_n(x, y)$ si $x$ et $y$ appartiennent à un même $X_n$, $d(x, y) = 1$ dans le cas contraire (IX, p. 16). On sait que $X$ est de type dénombrable (IX, p. 19, corollaire); il reste à prouver qu’il est complet pour $d$. Or, si $(x_m)$ est une suite de Cauchy dans $X$, il existe un $m_0$ tel que pour $p \geq m_0, q \geq m_0$, on ait $d(x_p, x_q) < 1$, donc tous les $x_m$ d’indice $m \geq m_0$ appartiennent à un même $X_n$; puisque $X_n$ est complet pour $d_n$, la suite $(x_m)$ est convergente.

#### Proposition 2 {#top-ix-s6-prop-2 .statement}

Tout sous-espace ouvert d’un espace polonais est polonais.

Soient $X$ un espace polonais, $d$ une distance compatible avec la topologie de $X$, $U$ une partie ouverte de $X$ distincte de $X$. Soit $V$ la partie du produit $\mathbf{R} \times X$ formée des points $(t, x)$ tels que $t \cdot d(x, X - U) = 1$; le sous-espace $V$ de $\mathbf{R} \times X$ est fermé (IX, p. 13, prop. 3), donc polonais (prop. 1). Comme la restriction à $V$ de la projection $\mathrm{pr}_2$ de $\mathbf{R} \times X$ sur $X$ est un homéomorphisme de $V$ sur $U$ (IX, p. 13, prop. 3), $U$ est un sous-espace polonais.

#### Corollaire {#top-ix-s6-n1-cor-1 .statement}

Tout espace $X$ localement compact, métrisable et dénombrable à l’infini, est polonais.

En effet, soit $X'$ l’espace compact obtenu par adjonction à $X$ d’un point à l’infini; on sait que $X'$ est métrisable et de type dénombrable (IX, p. 21, corollaire), et d’autre part $X'$ est complet pour son unique structure uniforme (II, p. 27, th. 1); l’espace $X'$ est donc polonais, et il en est de même de $X$ qui est un sous-espace ouvert de $X'$.

#### Proposition 3 {#top-ix-s6-prop-3 .statement}

Soit $X$ un espace topologique séparé; l’intersection d’une suite $(A_n)$ de sous-espaces polonais de $X$ est un sous-espace polonais.

Soit $f$ l’application diagonale de $X$ dans $X^\mathbf{N}$ (E, II, p. 33; on rappelle que $f(x) = (y_n)$, où $y_n = x$ pour tout $n$); nous utiliserons le lemme suivant:

#### Lemme 1 {#top-ix-s6-lem-1 .statement}

Soit $(A_n)$ une suite de parties de l’espace topologique séparé $X$; la restriction au sous-espace $\bigcap_n A_n$ de $X$ de l’application diagonale $f : X \to X^\mathbf{N}$ est un homéomorphisme de $\bigcap_n A_n$ sur un sous-espace fermé de $\prod_n A_n$.

En effet, cette image est l’intersection de $\prod_n A_n$ et de la diagonale $\Delta = f(X)$ qui est fermée dans $X^\mathbf{N}$ puisque $X$ est séparé (I, p. 52, prop. 1), et d’autre part $f$ est un homéomorphisme de $X$ sur $\Delta$.

Sous les hypothèses de la prop. 3, $\prod_n A_n$ est un espace polonais (IX, p. 57, prop. 1), donc $\bigcap_n A_n$ est un sous-espace polonais d’après le lemme 1 et la prop. 1 (IX, p. 57).

#### Corollaire {#top-ix-s6-n1-cor-2 .statement}

L’espace des nombres irrationnels, muni de la topologie induite par celle de la droite numérique $\mathbf{R}$, est polonais.

En effet, il est l’intersection d’une famille dénombrable d’ensembles ouverts dans $\mathbf{R}$, à savoir les complémentaires des ensembles réduits à un point rationnel.

#### Théorème 1 {#top-ix-s6-thm-1 .statement}

Pour qu’un sous-espace $Y$ d’un espace polonais $X$ soit polonais, il faut et il suffit que $Y$ soit intersection d’une famille dénombrable d’ensembles ouverts dans $X$.

Il résulte aussitôt des prop. 2 (IX, p. 57) et 3 que la condition est suffisante. Montrons qu’elle est nécessaire. Soit $d$ une distance compatible avec la topologie de $Y$, et pour laquelle $Y$ soit complet. Soit $\overline{Y}$ l’adhérence de $Y$ dans $X$. Pour chaque entier $n$, soit $Y_n$ l’ensemble des $x \in \overline{Y}$ qui possèdent un voisinage ouvert $U$ tel que le diamètre de $U \cap Y$ (pour la distance $d$) soit $\leqslant 1/n$. Il est clair que $Y_n$ est ouvert dans $\overline{Y}$ et contient $Y$. Soit $x$ un point de l’intersection des $Y_n$; $x$ est adhérent à $Y$ et la trace sur $Y$ du filtre des voisinages de $x$ dans $X$ est un filtre de Cauchy (pour la distance $d$); ce filtre converge donc vers un point de $Y$, et par suite $x \in Y$; autrement dit, on a $Y = \bigcap_n Y_n$. Pour tout $n$, soit $H_n$ un ensemble ouvert dans $X$ tel que $H_n \cap \overline{Y} = Y_n$; soit d’autre part $(U_m)$ une suite d’ensembles ouverts dans $X$ tels que $\overline{Y} = \bigcap_m U_m$ (IX, p. 16, prop. 7); alors $Y$ est l’intersection de la famille dénombrable d’ensembles ouverts $(H_n \cap U_m)$.

#### Corollaire 1 {#top-ix-s6-thm-1-cor-1 .statement}

Pour qu’un espace $X$ soit polonais, il faut et il suffit que $X$ soit homéomorphe à une intersection dénombrable d’ensembles ouverts du cube $\mathbf{I}^\mathbf{N}$ (où $I$ désigne l’intervalle $[0, 1]$ de $\mathbf{R}$).

La condition est évidemment suffisante; elle est nécessaire, parce que tout espace métrisable de type dénombrable est homéomorphe à un sous-espace de $\mathbf{I}^{\mathbf{N}}$ (IX, p. 18, prop. 12).

#### Corollaire 2 {#top-ix-s6-thm-1-cor-2 .statement}

Soient $X$ et $Y$ deux espaces polonais, $f$ une application continue de $X$ dans $Y$. Pour tout sous-espace polonais $Z$ de $Y$, $f^{-1}(Z)$ est un sous-espace polonais de $X$

En effet, on a $Z = \bigcap_n Z_n$, où les $Z_n$ sont ouverts dans $Y$, d’où $f^{-1}(Z) = \bigcap_n f^{-1}(Z_n)$, et les $f(Z_n)$ sont ouverts dans $X$.

### 2. Espaces sousliniens

#### Définition 2 {#top-ix-s6-def-2 .statement}

On dit qu’un espace topologique $X$ est un espace de Souslin, ou espace souslinien, s’il est séparé et s’il existe un espace polonais $P$ et une application continue de $P$ sur $X$. On dit qu’une partie $A$ d’un espace topologique $X$ est un ensemble souslinien si le sous-espace $A$ est souslinien.

#### Remarque {#top-ix-s6-n2-rem-1 .statement}

Il est clair que tout espace polonais est souslinien, et que l’image d’un espace souslinien $X$ par une application continue de $X$ dans un espace séparé $Y$ est un espace souslinien.

*Nous verrons plus loin que tout espace souslinien est un espace de Lindelöf (IX, p. 76, corollaire).*

#### Proposition 4 {#top-ix-s6-prop-4 .statement}

Dans tout espace souslinien $X$, il existe un ensemble dénombrable dense.

En effet, soient $P$ un espace polonais, $f$ une application continue de $P$ sur $X$; l’image par $f$ d’une partie dénombrable dense dans $P$ est une partie dénombrable dense.

#### Proposition 5 {#top-ix-s6-prop-5 .statement}

Tout sous-espace fermé (resp. ouvert) d’un espace souslinien $X$ est souslinien.

En effet, si $f$ est une application continue d’un espace polonais $P$ sur $X$, et $A$ une partie fermée (resp. ouverte) de $X$, $f^{-1}(A)$ est un sous-espace fermé (resp. ouvert) de $P$, donc un sous-espace polonais (IX, p. 57, prop. 1 et prop. 2), et la restriction de $f$ à $f^{-1}(A)$ est une application continue surjective de $f^{-1}(A)$ sur $A$.

#### Proposition 6 {#top-ix-s6-prop-6 .statement}

Soient $X$ un espace souslinien, $Y$ un espace séparé, $f$ une application continue de $X$ dans $Y$. L’image réciproque par $f$ d’un sous-espace souslinien $A$ de $Y$ est un sous-espace souslinien de $X$.

En effet, soient $P$, $Q$ des espaces polonais, $g$ une application continue de $P$ sur $X$, $h$ une application continue de $Q$ sur $A$. Soit $R$ l’ensemble des points $(x, y) \in P \times Q$ tels que $f(g(x)) = h(y)$; $R$ est fermé dans $P \times Q$, donc c’est un sous-espace polonais (IX, p. 57, prop. 1). Soit $\varphi$ la restriction à $\mathbf{R}$ de la projection $\mathrm{pr}_1$; le sous-espace $f^{-1}(A)$ de $X$ est alors l’image de $\mathbf{R}$ par l’application continue $g \circ \varphi$, et est par suite souslinien.

#### Proposition 7 {#top-ix-s6-prop-7 .statement}

*Le produit et la somme d’une famille dénombrable d’espaces sousliniens sont des espaces sousliniens.*

En effet, soient, pour tout entier $n$, $X_n$ un espace séparé, $P_n$ un espace polonais, $f_n$ une application continue de $P_n$ sur $X_n$. L’espace produit (resp. somme) des $P_n$ est polonais (IX, p. 57, prop. 1), et l’image de cet espace par l’application produit des $f_n$ (resp. l’application qui coïncide avec $f_n$ dans chaque $P_n$) est l’espace produit (resp. somme) des $X_n$; comme ce dernier est séparé, c’est un espace souslinien.

#### Proposition 8 {#top-ix-s6-prop-8 .statement}

*Soient $X$ un espace séparé, $(A_n)$ une suite de sous-espaces sousliniens de $X$. Alors la réunion et l’intersection des $A_n$ sont des sous-espaces sousliniens.*

En effet, ces sous-espaces sont séparés. L’existence de l’application canonique de l’espace somme des $A_n$ sur le sous-espace $\bigcup_n A_n$ de $X$ montre que ce dernier est souslinien (IX, p. 60, prop. 7); d’autre part, $\bigcap_n A_n$ est souslinien en vertu des prop. 5 et 7 (IX, p. 59 et 60) et du lemme 1 (IX, p. 58).

En général, même dans un espace polonais, le complémentaire d’un sous-espace souslinien n’est pas nécessairement souslinien (cf. IX, p. 120, exerc. 8); voir toutefois IX, p. 66, corollaire 1.

### 3. Ensembles boréliens

#### Définition 3 {#top-ix-s6-def-3 .statement}

*Soient $A$ un ensemble, $\Sigma$ un ensemble de parties de $A$. On dit que $\Sigma$ est une tribu sur $A$ si les conditions suivantes sont satisfaites:
a) le complémentaire de tout ensemble de $\Sigma$ appartient à $\Sigma$;
b) toute intersection dénombrable d’ensembles de $\Sigma$ appartient à $\Sigma$.*

Pour que $\Sigma$ soit une tribu, il faut et il suffit que la condition *a)* soit satisfaite, ainsi que la suivante:

*b')* toute réunion dénombrable d’ensembles de $\Sigma$ appartient à $\Sigma$.

L’ensemble $\mathcal{P}(A)$ de toutes les parties de $A$ est évidemment une tribu. Toute intersection de tribus sur $A$ est une tribu sur $A$. Pour toute partie $\mathcal{F}$ de $\mathcal{P}(A)$, il existe donc une *plus petite tribu* contenant $\mathcal{F}$; on l’appelle la tribu *engendrée* par $\mathcal{F}$.

#### Définition 4 {#top-ix-s6-def-4 .statement}

*On appelle tribu borélienne sur un espace topologique $X$ la tribu engendrée par l’ensemble des parties ouvertes de $X$; les ensembles de cette tribu sont appelés ensembles boréliens de $X$.*

Les parties fermées de $X$ sont donc des ensembles boréliens, engendrant la tribu borélienne. Si la topologie de $X$ admet une *base dénombrable* $\mathcal{B}$, les ensembles de $\mathcal{B}$ engendrant la tribu borélienne.

#### Définition 5 {#top-ix-s6-def-5 .statement}

Etant donnés deux espaces topologiques $X, Y$, on dit qu’une application $f : X \to Y$ est borélienne si, pour tout ensemble borélien $B$ de $Y$, $f^{-1}(B)$ est un ensemble borélien dans $X$.

Il résulte aussitôt de cette définition que si $f : X \to Y$ et $g : Y \to Z$ sont deux applications boréliennes, $g \circ f : X \to Z$ est borélienne.

#### Proposition 9 {#top-ix-s6-prop-9 .statement}

Soient $X, Y$ deux espaces topologiques, $\mathcal{F}$ une partie de $\mathfrak{P}(Y)$ engendrant la tribu borélienne de $Y$. Pour qu’une application $f : X \to Y$ soit borélienne, il faut et il suffit que $f^{-1}(\mathcal{F})$ soit contenu dans la tribu borélienne de $X$.

La condition est évidemment nécessaire. Inversement, si elle est vérifiée, considérons l’ensemble $\mathcal{L}$ des parties $B$ de $Y$ telles que $f^{-1}(B)$ soit borélien dans $X$. Il est immédiat que $\mathcal{L}$ est une tribu et contient $\mathcal{F}$; elle contient donc la tribu borélienne de $Y$, et par suite $f$ est borélienne.

#### Corollaire 1 {#top-ix-s6-prop-9-cor-1 .statement}

Toute application continue est borélienne.

Il suffit d’appliquer la prop. 9 au cas où $\mathcal{F}$ est l’ensemble des parties ouvertes de $Y$.

#### Corollaire 2 {#top-ix-s6-prop-9-cor-2 .statement}

Soient $(X_n)$ une suite d’espaces topologiques, $X = \prod_n X_n$ leur produit. Si, pour chaque $n$, $A_n$ est une partie borélienne de $X_n$, alors $\prod_n A_n$ est une partie borélienne de $X$.

En effet, on a $\prod_n A_n = \bigcap_n \overline{\mathrm{pr}}_n^{-1}(A_n)$ et comme $\mathrm{pr}_n$ est continue, $\overline{\mathrm{pr}}_n^{-1}(A_n)$ est borélienne dans $X$ en vertu du cor. 1.

#### Remarque {#top-ix-s6-n3-rem-1 .statement}

Soint $Y$ un espace topologique, $X$ un sous-espace de $Y$; alors la tribu borélienne de $X$ est l’ensemble des parties de la forme $B \cap X$, où $B$ parcourt la tribu borélienne de $Y$. En effet, ces ensembles forment une tribu $\mathcal{L}$, à laquelle appartiennent les ouverts de $X$, donc $\mathcal{L}$ contient la tribu borélienne de $X$. Inversement, comme l’injection canonique $j : X \to Y$ est continue, pour tout ensemble borélien $B$ de $Y$, $j^{-1}(B) = B \cap X$ est un ensemble borélien dans $X$ (cor. 1 de la prop. 9), donc $\mathcal{L}$ est la tribu borélienne de $X$.

#### Proposition 10 {#top-ix-s6-prop-10 .statement}

Dans un espace souslinien $X$, tout ensemble borélien est souslinien.

En effet, soit $\mathcal{L}$ l’ensemble des parties $A$ de $X$ telles que $A$ et $\complement A$ soient sousliniens; la prop. 8 (IX, p. 60) montre que $\mathcal{L}$ est une tribu. Toute partie fermée $F$ de $X$ appartient à $\mathcal{L}$, car $F$ et $\complement F$ sont sousliniens (IX, p. 59, prop. 5); donc $\mathcal{L}$ contient tous les ensembles boréliens de $X$ (cf. IX, p. 66, corollaire 1).

#### Corollaire {#top-ix-s6-n3-cor-1 .statement}

Soit $f$ une application continue d’un espace souslinien $X$ dans un espace séparé $Y$. Pour tout sous-ensemble borélien $B$ de $X$, $f(B)$ est souslinien.

En effet, $B$ est souslinien, donc $f(B)$ est souslinien, d’après la Remarque de IX, p. 59.

Remarque. --- 2) Même lorsque X et Y sont polonais, il n’est pas vrai, en général, que l’image d’un ensemble borélien de X par une application continue de X dans Y soit un ensemble borélien de Y (cf. IX, p. 120, exerc. 8, et IX, p. 68, prop. 14).

### 4. Espaces éparpillés et espaces lusiniens

#### Définition 6 {#top-ix-s6-def-6 .statement}

On dit qu’un espace topologique est éparpillé s’il est séparé et si tout point possède un système fondamental de voisinages à la fois ouverts et fermés.

Tout espace éparpillé est totalement discontinu : car la composante connexe d’un point x est contenue dans tous les ensembles à la fois ouverts et fermés contenant x (I, p. 83), et l’intersection de ces ensembles se réduit à x si E est éparpillé.

Inversement, un espace localement compact totalement discontinu est éparpillé (II, p. 32, corollaire) ; mais il y a des espaces métrisables totalement discontinus qui ne sont pas éparpillés (IX, p. 119, exerc. 5 b).

Tout sous-espace d’un espace éparpillé est éparpillé ; tout produit (resp. toute somme) d’espaces éparpillés est un espace éparpillé.

#### Définition 7 {#top-ix-s6-def-7 .statement}

On dit qu’un espace topologique X est un espace de Lusin, ou un espace lusinien, s’il est séparé et s’il existe un espace polonais éparpillé P et une application continue bijective de P sur E.

Il est clair que tout espace lusinien est souslinien.

#### Proposition 11 {#top-ix-s6-prop-11 .statement}

Pour qu’un espace soit lusinien, il faut et il suffit qu’il existe un espace polonais P et une bijection continue de P sur X.

La condition étant évidemment nécessaire, tout revient à prouver qu’elle est suffisante. Si f est une application continue bijective d’une espace lusinien X sur un espace séparé Y, il résulte de la déf. 7 que Y est lusinien. Tout revient donc à prouver qu’un espace polonais est lusinien.

Notons en premier lieu que si X est un espace lusinien, tout sous-espace fermé (resp. ouvert) A de X est lusinien (cf. IX, p. 66, th. 3) ; en effet, si f est une application continue bijective d’un espace polonais éparpillé P sur X, f(A) est fermé (resp. ouvert) dans P, donc est un sous-espace polonais (IX, p. 57, prop. 1 et 2) et éparpillé, ce qui établit notre assertion.

Tout produit dénombrable d’espaces lusiniens est lusinien : cela résulte de la prop. 1 de IX, p. 57 et du fait que tout produit d’espaces éparpillés est éparpillé. Toute intersection dénombrable de sous-espaces lusiniens d’un espace topologique séparé est un sous-espace lusinien : cela résulte aussitôt des remarques précédentes et du lemme 1 de IX, p. 58. En outre :

#### Lemme 2 {#top-ix-s6-lem-2 .statement}

Si un espace séparé X est tel qu’il existe une partition dénombrable (A_n) de X formée de sous-espaces lusiniens, alors X est lusinien.

En effet, soient, pour tout entier n, P_n un espace polonais éparpillé et f_n une bijection continue de P_n sur A_n ; si P est l’espace somme des P_n, P est polonais

(IX, p. 57, prop. 1) et éparpillé, et l’application $f$ de $P$ dans $X$ qui coïncide avec $f_n$ dans chaque $P_n$ est une bijection continue de $P$ sur $X$, d’où le lemme.

Cela étant, montrons tout d’abord que l’intervalle $I = [0, 1]$ de $\overline{\mathbf{R}}$ est lusinien. Considérons en effet l’application surjective $f : \{0, 1\}^\mathbf{N} \to I$ qui, à tout point $(\varepsilon_n)_{n \geq 0}$ avec $\varepsilon_n = 0$ ou $\varepsilon_n = 1$, fait correspondre le nombre $\sum_{n=0}^\infty \varepsilon_n 2^{-n}$ ayant $(\varepsilon_n)$ pour développement dyadique (IV, p. 43). Soit $D$ l’ensemble dénombrable dans $\{0, 1\}^\mathbf{N}$ formé des suites autre que la suite 0, n’ayant qu’un nombre fini de termes $\neq 0$; $P = \{0, 1\}^\mathbf{N} - D$ est un espace polonais éparpillé (IX, p. 58, th. 1), et la restriction de $f$ à $P$ est une bijection continue de $P$ sur $I$ (IV, p. 42).

Soit enfin $P$ un espace polonais quelconque; d’après le cor. 1 de IX, p. 58, $P$ est homéomorphe à un sous-espace du cube $I^\mathbf{N}$, intersection dénombrable d’ensembles ouverts de $I^\mathbf{N}$; la proposition résulte donc du fait que $I$ est lusinien et des remarques faites au début de la démonstration.

#### Corollaire {#top-ix-s6-n4-cor-1 .statement}

*Toute limite projective dénombrable* (I, p. 28) *d’espaces lusiniens est un espace lusinien*.

En effet, une limite projective dénombrable d’espaces séparés est un sous-espace fermé du produit (dénombrable) de ces espaces; le corollaire résulte donc de ce qui a été prouvé au cours de la démonstration de la prop. 11.

*On peut montrer que les espaces de distributions $\mathcal{D}'(\Omega)$, $\mathcal{E}'(\Omega)$, etc. sur un ouvert $\Omega$ de $\mathbf{R}^n$, munis de la topologie forte, sont des espaces lusiniens.*

### 5. Cribles

#### Définition 8 {#top-ix-s6-def-8 .statement}

*On appelle crible une suite* $C = (C_n, p_n)_{n \geq 0}$ *telle que, pour tout* $n$, $C_n$ *soit un ensemble dénombrable et* $p_n$ *une surjection de* $C_{n+1}$ *sur* $C_n$.

Pour tout couple d’entiers tels que $0 \leq m \leq n$, désignons par $p_{mn}$ l’application identique de $C_m$ sur lui-même si $m = n$, et la surjection $p_m \circ p_{m+1} \circ \cdots \circ p_{n-1}$ de $C_n$ sur $C_m$ si $m < n$. Il est clair que pour $m \leq n \leq q$, on a $p_{mq} = p_{mn} \circ p_{nq}$, et on peut donc considérer l’ensemble $L(C)$ *limite projective* de la famille $(C_n)$ pour la famille d’applications $(p_{mn})$ (E, III, p. 52); nous munirons cet ensemble. de la topologie *limite projective* des topologies discrètes sur les $C_n$ (I, p. 28). Il est clair que $L(C)$ est *fermé* dans l’espace produit $\prod_n C_n$; il en résulte aussitôt que $L(C)$ est un *espace polonais éparpillé* (IX, p. 62); nous dirons que $L(C)$ est l’espace topologique *associé* au crible $C$.

On appelle *criblage* d’un espace métrique $X$ la donnée d’un crible $C = (C_n, p_n)$ et, pour chaque entier $n \geq 0$, d’une application $\varphi_n$ de $C_n$ dans l’ensemble des parties *ouvertes non vides* de $X$ *de diamètre* $\leq 2^{-n}$, de manière que:

a) $X$ soit la réunion des $\varphi_0(c)$, lorsque $c$ parcourt $C_0$;
b) pour tout $n$ et tout $c \in C_n$, $\varphi_n(c)$ soit la réunion des $\varphi_{n+1}(c')$, où $c'$ parcourt $p_n^{-1}(c)$, et contienne les adhérences $\overline{\varphi_{n+1}(c')}$ de ces ensembles dans $X$.

On dit qu’un criblage est strict si en outre, pour tout n, les ensembles $\varphi_n(c)$ où c parcourt $C_n$, sont deux à deux disjoints. Ces ensembles sont alors à la fois ouverts et fermés dans X.

#### Lemme 3 {#top-ix-s6-lem-3 .statement}

Tout espace métrique de type dénombrable X possède un criblage. Si de plus X est éparpillé, X possède un criblage strict.

Observons d’abord que si U est un ensemble ouvert dans un espace métrique X de type dénombrable, et $\varepsilon$ un nombre > 0, il existe un recouvrement dénombrable de U par des ensembles ouverts de diamètre $\leq \varepsilon$, dont les adhérences dans X sont contenues dans U : il suffit en effet, pour tout $x \in U$, de considérer une boule ouverte $B_x$ de centre x et de rayon $\leq \varepsilon/2$, dont l’adhérence dans X soit contenue dans U, puis d’appliquer la prop. 13 de IX, p. 19 au recouvrement formé par les $B_x$. Si de plus X est éparpillé, il existe un tel recouvrement ($V_n$) formé d’ensembles à la fois ouverts et fermés dans X ; en désignant par $W_n$ l’intersection de $V_n$ et des $X - V_k$ pour $k < n$, on voit que les $W_n$ sont à la fois ouverts et fermés dans X, de diamètre $\leq \varepsilon$, deux à deux disjoints et recouvrent U.

Soit alors X un espace métrique de type dénombrable. Soit $C_0$ l’ensemble des indices d’un recouvrement dénombrable de X formé d’ensembles ouverts non vides de diamètre $\leq 1$, deux à deux disjoints si X est éparpillé ; $\varphi_0$ sera l’application qui, à chaque indice $c \in C_0$, associe l’ensemble correspondant du recouvrement. Supposons déjà définis les $C_i$ et les $\varphi_i$, ainsi que les surjections $p_i : C_{i+1} \to C_i$ pour $i \leq n$, de façon que la condition b) soit satisfaite pour ces indices. Si $c \in C_n$, $\varphi_n(c)$ est ouvert dans X, donc possède un recouvrement dénombrable par des ensembles ouverts non vides de diamètre $\leq 2^{-n-1}$, dont les adhérences dans X sont contenues dans $\varphi_n(c)$, et qui sont deux à deux disjoints lorsque X (donc $\varphi_n(c)$) est éparpillé ; si $I(c)$ est l’ensemble des indices de ce recouvrement, on prend pour $C_{n+1}$ l’ensemble somme des $I(c)$ lorsque $c$ parcourt $C_n$ ; pour tout $c' \in C_{n+1}$, on désigne par $p_n(c')$ l’unique élément $c \in C_n$ tel que $c' \in I(c)$, et par $\varphi_{n+1}(c')$ l’ensemble d’indice $c'$ du recouvrement considéré de $\varphi_n(c)$. Il est clair que l’on a ainsi défini par récurrence un criblage de X, et que ce criblage est strict si X est éparpillé, d’où le lemme.

Supposons maintenant que X soit un espace métrique complet de type dénombrable, et considérons un criblage de X par un crible C et des applications $\varphi_n$. Si $\gamma = (c_n)$ est un point de l’espace $L(C)$ associé à C, la suite $(\varphi_n(c_n))$ est une suite décroissante d’ensembles ouverts dans X, dont chacun contient l’adhérence du suivant dans X, et dont le diamètre tend vers 0 ; l’intersection de cette suite d’ensembles est donc réduite à un point (II, p. 15), qu’on notera $f(\gamma)$. On a ainsi défini une application $f$ de $L(C)$ dans X ; si deux points $\gamma, \gamma'$ de $L(C)$ ont mêmes coordonnées d’indice i pour $i \leq n$, il est clair que la distance de $f(\gamma)$ et de $f(\gamma')$ est $\leq 2^{-n}$, donc $f$ est continue en vertu de la définition de la topologie de $L(C)$. Pour tout $x \in X$, il résulte de la définition d’un criblage qu’on peut définir par récurrence sur $n$ une suite $\gamma = (c_n)$ telle que $x \in \varphi_n(c_n)$ pour tout $n \geq 0$ et $c_n = p_n(c_{n+1})$; on a par suite $x = f(\gamma)$, autrement dit $f$ est surjective. En outre, si le criblage est strict, la suite $\gamma = (c_n)$ telle que $x = f(\gamma)$ est unique, donc $f$ est bijective. On dira que $f$ est l’application déduite du criblage considéré.

#### Proposition 12 {#top-ix-s6-prop-12 .statement}

Pour tout espace lusinien (resp. souslinien) $X$, il existe un crible $C$ et une bijection (resp. surjection) continue de $L(C)$ sur $X$.

Compte tenu de la définition d’un espace lusinien (IX, p. 62, déf. 7) (resp. souslinien (IX, p. 59, déf. 2)), on se ramène au cas où $E$ est polonais et éparpillé (resp. polonais) et le raisonnement qui précède démontre alors la prop. 12.

### 6. Séparation des ensembles sousliniens

#### Théorème 2 {#top-ix-s6-thm-2 .statement}

Soit $X$ un espace séparé. Étant donnée une suite $(X_n)$ de sous-espaces sousliniens de $X$, deux à deux disjoints, il existe une suite $(B_n)$ d’ensembles boréliens de $X$, deux à deux disjoints, tels que $X_n \subset B_n$ pour tout $n$.

Nous établirons d’abord deux lemmes:

#### Lemme 4 {#top-ix-s6-lem-4 .statement}

Soient $(A_n), (A'_m)$ deux suites de parties d’un espace topologique $X$. Supposons que, pour tout couple $(A_n, A'_m)$, il existe un ensemble borélien $B_{nm}$ de $X$ tel que $B_{nm} \supset A_n$ et $B_{nm} \cap A'_m = \emptyset$. Alors il existe un ensemble borélien $B$ de $X$, qui contient $\bigcup_n A_n$ et ne rencontre pas $\bigcup_m A'_m$.

En effet, l’ensemble $B = \bigcup_n \left( \bigcap_m B_{nm} \right)$ répond à la question.

#### Lemme 5 {#top-ix-s6-lem-5 .statement}

Soient $X$ un espace séparé, $A, A'$ deux sous-espaces sousliniens de $X$ sans point commun. Il existe alors un ensemble borélien $B$ de $X$ tel que $B \supset A$ et $B \cap A' = \emptyset$.

En effet, d’après IX, p. 65, prop. 12, il existe deux cribles $C, C'$, une application continue $f$ de $L(C)$ sur $A$ et une application continue $f'$ de $L(C')$ sur $A'$, définies suivant le procédé décrit dans IX, p. 64. Pour tout $n \geq 0$ et tout $c \in C_n$, notons $q_n(c)$ le sous-espace de $L(C)$ formé des suites $(c_k)_{k \geq 0}$ telles que $c_n = c$; c’est un sous-espace fermé de $L(C)$. Pour tout $\gamma = (c_n) \in L(C)$, la suite des ensembles fermés $q_n(c_n)$ est décroissante et constitue une base de filtre ayant pour limite $\gamma$. En outre, pour tout $c \in C_n$, les ensembles $q_{n+i}(d)$, où $d$ parcourt l’ensemble $p_n^{-1}(c)$ dans $C_{n+i}$, forment une partition de $q_n(c)$. Notations analogues pour le crible $C'$.

Cela étant, on va raisonner par l’absurde, en supposant que tout ensemble borélien contenant $A$ rencontre $A'$. En premier lieu, il résulte du lemme 4 (IX, p. 65) et de la définition d’un criblage qu’il existe $c_0 \in C_0$ et $c'_0 \in C'_0$ tels que tout ensemble borélien contenant $f(q_0(c_0))$ rencontre $f'(q'_0(c'_0))$. On va alors définir par récurrence sur $n$ deux éléments $\gamma = (c_n) \in L(C), \gamma' = (c'_n) \in L(C')$ de la façon suivante: supposons déjà définis les $c_i$ et $c'_i$ pour $i < n$, de manière que, pour chaque indice $i < n$, tout ensemble borélien contenant $f(q_i(c_i))$ rencontre $f'(q'_i(c'_i))$; en appliquant le lemme 4 et la définition d’un criblage aux ensembles $f(q_{n-i}(c_{n-i}))$ et $f'(q'_{n-i}(c'_{n-i}))$, on voit qu’il existe $c_n \in C_n$ et $c'_n \in C'_n$ tels que $p_{n-i}(c_n) = c_{n-i}$, $p'_{n-i}(c'_n) = c'_{n-i}$ et que tout ensemble borélien contenant $f(q_n(c_n))$ rencontre $f'(q'_n(c'_n))$. Or, la suite des $f(q_n(c_n))$ converge vers un point $a = f(\gamma) \in A$, et la base de filtre des $f'(q'_n(c'_n))$ converge vers un point $a' = f'(\gamma') \in A'$. Comme $A \cap A' = \varnothing$ et que $X$ est séparé, il existe un voisinage fermé $V$ de $a$ ne contenant pas $a'$; pour $n$ assez grand, $V$ contient $f(q_n(c_n))$ et ne rencontre pas $f'(q'_n(c'_n))$, d’où contradiction puisque $V$ est borélien.

Ces lemmes étant démontrés, pour tout entier $n$, désignons par $F_n$ la réunion des ensembles $X_i$ tels que $i \neq n$; $F_n$ est un sous-espace souslinien (IX, p. 60, prop. 8). Pour chaque indice $n$, il existe, en vertu du lemme 5, un ensemble borélien $B'_n$ qui contient $X_n$ et ne rencontre pas $F_n$. Soit $B_n$ l’intersection de $B'_n$ et de $\bigcap_{i < n} (X - B')$. Les $B_n$ sont boréliens, deux à deux disjoints, et l’on a $B_n \supset X_n$ pour tout $n$, ce qui achève la démonstration du th. 2.

#### Corollaire 1 {#top-ix-s6-lem-5-cor-1 .statement}

Si une partition dénombrable d’un espace séparé est formée d’ensembles sousliniens, ces ensembles sont boréliens. En particulier, dans un espace séparé, tout ensemble souslinien dont le complémentaire est souslinien est un ensemble borélien.

#### Corollaire 2 {#top-ix-s6-lem-5-cor-2 .statement}

Soient $E$ et $F$ deux espaces sousliniens et $f : E \to F$ une application continue surjective. Pour qu’un sous-ensemble $B$ de $F$ soit borélien, il faut et il suffit que $f^{-1}(B)$ soit borélien dans $E$.

Le cor. 1 de la prop. 9 montre que la condition est nécessaire. D’autre part, si $f^{-1}(B)$ est borélien, $B = f(f^{-1}(B))$ et $F - B = f(E - f^{-1}(B))$ sont sousliniens (cor. de la prop. 10), donc boréliens (cor. 1).

### 7. Espaces lusiniens et ensembles boréliens

#### Théorème 3 {#top-ix-s6-thm-3 .statement}

Soit $X$ un espace lusinien régulier. Pour qu’un sous-espace de $X$ soit lusinien, il faut et il suffit qu’il soit borélien dans $X$.

Cela va résulter des deux lemmes suivants:

#### Lemme 6 {#top-ix-s6-lem-6 .statement}

Dans un espace lusinien $X$, tout ensemble borélien est un sous-espace lusinien de $X$.

(En d’autres termes, pour toute partie borélienne $B$ de $X$, il existe un espace polonais éparpillé $P$ et une application continue injective $f : P \to E$ telle que $f(P) = B$).

Soit $\mathfrak{S}$ l’ensemble des parties $A$ de $X$ telles que les sous-espaces $A$ et $\complement A$ soient lusiniens. Tout ensemble fermé et tout ensemble ouvert dans $X$ étant un sous-espace lusinien (IX, p. 62), $\mathfrak{S}$ contient tous les ensembles fermés de $X$. Le lemme sera donc établi si on prouve que $\mathfrak{L}$ est une tribu. Il suffit pour cela de montrer que si $(A_n)$ est une suite d’ensembles de $\mathfrak{L}$, les sous-espaces $\bigcap_n A_n$ et $\bigcup_n A_n$ sont lusiniens. Or, on a vu (IX, p. 62) que toute intersection dénombrable de sous-espaces lusiniens est un sous-espace lusinien. D’autre part, si $B_n$ est l’intersection de $A_n$ et de $\bigcap_{i < n} CA_i$, il résulte de l’hypothèse et de la remarque précédente que $B_n$ est un sous-espace lusinien; comme on a $\bigcup_n A_n = \bigcup_n B_n$, le sous-espace $\bigcup_n A_n$ est lusinien en vertu du lemme 2 (IX, p. 62).

#### Lemme 7 {#top-ix-s6-lem-7 .statement}

*Tout sous-espace lusinien $A$ d’un espace régulier $X$ est un ensemble borélien dans $X$.*

D’après la prop. 12 (IX, p. 65), il existe un crible $C$ et une *bijection continue* $f$ de $L(C)$ sur $A$. Avec les notations du lemme 5 (IX, p. 65), pour tout entier $n$ et tout $c \in C_n$, notons $g_n(c)$ le sous-espace $f(q_n(c))$ de $X$; c’est un sous-espace lusinien de $X$, donc un sous-espace souslinien. Lorsque $c$ parcourt $C_n$, les ensembles $g_n(c)$ sont deux à deux disjoints, puisque $f$ est bijective; en vertu du th. 2 (IX, p. 65), il existe donc une famille $c \mapsto g'_n(c)$ ($c \in C_n$) d’ensembles boréliens dans $X$, deux à deux disjoints et tels que $g'_n(c) \supseteq g_n(c)$ pour tout $c \in C_n$. Quitte à remplacer $g'_n(c)$ par son intersection avec l’adhérence $\overline{g_n(c)}$ de $g_n(c)$ dans $X$, on peut supposer que $g'_n(c) \subset \overline{g_n(c)}$. Désignons par $c_{n-i}, c_{n-2}, \ldots, c_0$ les images de $c$ dans $C_{n-i}, C_{n-2}, \ldots C_0$ par les surjections

$$
p_{n-i,n} = p_{n-i},\ p_{n-2,n} = p_{n-2} \circ p_{n-i},\ \ldots,\ p_{0n} = p_0 \circ p_i \circ \cdots \circ p_{n-i}
$$

respectivement; notons $h_n(c)$ l’intersection des ensembles

$$
g'_n(c),\ g'_{n-i}(c_{n-i}),\ \ldots,\ g'_0(c_0).
$$

Comme $q_i(c_i) \supset q_n(c)$ pour $0 \leq i \leq n-1$, $h_n(c)$ contient $g_n(c)$; il est clair en outre que $h_n(c)$ est borélien et contenu dans $\overline{g_n(c)}$, et que lorsque $c$ parcourt $C_n$, les $h_n(c)$ sont deux à deux disjoints; enfin, par construction, pour tout $c' \in C_{n+i}$, on a $h_{n+i}(c') \subset h_n(p_n(c'))$. Soit alors $B_n$ la réunion des $h_n(c)$ pour $c \in C_n$; $B_n$ est borélien, et $B_{n+i} \subset B_n$; de plus, $B_n$ contient la réunion des $g_n(c)$ (où $c \in C_n$), réunion qui n’est autre que $A$. Soit $B$ l’intersection de la suite décroissante des $B_n$; l’ensemble $B$ est borélien et contient $A$. On va montrer que $B = A$, ce qui achèvera la démonstration.

Soit $x$ un point de $B$; pour chaque entier $n$, il existe un $c \in C_n$ et un seul tel que $x \in h_n(c)$: notons-le $c_n(x)$; alors la suite $(c_n(x))_{n \geq 0}$ appartient à $L(C)$. La suite décroissante $(g_n(c_n(x)))$ converge par définition vers un point $a \in A$; la suite des adhérences de ces ensembles converge aussi vers $a$ dans $X$, puisque $X$ est *régulier*, et il en est de même *a fortiori* de la suite $(h_n(c_n(x)))$. Or, $x$ appartient à tous les ensembles $h_n(c_n(x))$, donc $x = a \in A$ et le théorème est démontré.

#### Corollaire {#top-ix-s6-n7-cor-1 .statement}

Soit $(A_n)$ une suite de sous-espaces lusiniens d’un espace topologique séparé E. La réunion des $A_n$ est un sous-espace lusinien de E.

Pour $i < n$, posons $A_{n,i} = A_n \cap A_i$; c’est un sous-espace lusinien, donc borélien, de $A_n$. Par suite, l’intersection $B_n$ des $A_n - A_{n,i}$ ($i < n$) est un sous-ensemble borélien de $A_n$, donc lusinien. Comme les $B_n$ sont deux à deux disjoints, et que leur réunion est égale à celle des $A_n$, cette dernière est un espace lusinien d’après le lemme 2 de IX, p. 62.

#### Proposition 13 {#top-ix-s6-prop-13 .statement}

Soit $(X_n)_{n \in \mathbf{N}}$ une suite d’espaces lusiniens réguliers, $X = \prod_n X_n$ leur produit. Alors la tribu borélienne sur $X$ est engendrée par les ensembles de la forme $\prod_n A_n$, où $A_n$ est borélien dans $X_n$ pour tout $n$.

On sait déjà que les ensembles $\prod_n A_n$ sont boréliens (IX, p. 61, cor. 2); il suffit de voir que la tribu $\mathfrak{S}$ engendrée par ces ensembles contient tout ensemble ouvert U de X. Or, pour tout $n$, soient $P_n$ un espace polonais, $f_n : P_n \to X_n$ une bijection continue de $P_n$ sur $X_n$, $f = (f_n) : \prod_n P_n \to X$ la bijection correspondante de $\prod_n P_n$ sur X. Chaque $P_n$ admet une base dénombrable d’ouverts $\mathfrak{B}_n$ et P admet donc comme base dénombrable d’ouverts $\mathfrak{B}$ les ensembles élémentaires $\prod_n B_n$, où $B_n = X_n$ sauf pour un nombre fini d’indices, et $B_n \in \mathfrak{B}_n$ pour chacun de ces derniers. Comme $f^{-1}(U)$ est ouvert, il est borélien et on en conclut que U appartient à la tribu engendrée par les images

$$
f\left(\prod_n B_n\right) = \prod_n f_n(B_n)
$$

des ensembles de $\mathfrak{B}$. Mais comme tout $B_n \in \mathfrak{B}_n$ est un espace polonais (IX, p. 57, prop. 2), $f_n(B_n)$ est lusinien (IX, p. 62, prop. 11), donc borélien en vertu du th. 3 (IX, p. 66), ce qui achève la démonstration.

#### Corollaire {#top-ix-s6-n7-cor-2 .statement}

Soient Y un espace topologique, $(X_n)_{n \in \mathbf{N}}$ une suite d’espaces lusiniens réguliers, et pour tout $n$, soit $f_n : Y \to X_n$ une application borélienne. Alors l’application $f = (f_n) : Y \to \prod_n X_n$ est borélienne.

Avec les notations de la prop. 13, il suffit de montrer que pour toute famille $(A_n)$, où $A_n$ est borélien dans $X_n$, $f^{-1}\left(\prod_n A_n\right) = \bigcap_n f_n^{-1}(A_n)$ est borélien dans Y, ce qui résulte de l’hypothèse.

#### Proposition 14 {#top-ix-s6-prop-14 .statement}

Soient X, Y des espaces lusiniens, Y étant de plus supposé régulier. Si f est une application borélienne injective de X dans Y, alors, pour tout ensemble borélien A dans X, $f(A)$ est un ensemble borélien dans Y.

Le sous-espace A de X est lusinien (IX, p. 66, lemme 6); d’autre part, l’injection canonique $j : A \to X$ est continue, donc borélienne et par suite, $f \circ j$ est borélienne; on peut donc se borner au cas où $A = X$. Soit $g = f \times id_Y : X \times Y \to Y \times Y$; d’après le cor. de la prop. 13, $g$ est borélienne. Comme la diagonale $\Delta$ de $Y \times Y$ est fermée (I, p. 52, prop. 1), le graphe $\Gamma_f$ de $f$, égal à $-1_g(\Delta)$, est borélien dans $X \times Y$, donc un sous-espace lusinien de $X \times Y$ (IX, p. 66, lemme 6). La restriction $h$ de $pr_2$ à $\Gamma_f$ est par hypothèse une bijection continue de $\Gamma_f$ sur le sous-espace $f(X)$ de $Y$; comme il existe une bijection continue $u$ d’un espace polonais éparpillé $P$ sur $\Gamma_f$, $h \circ u$ est une bijection continue de $P$ sur $f(X)$ qui est par suite un sous-espace lusinien de $Y$. Mais comme $Y$ est lusinien et régulier, le th. 3 (IX, p. 66) prouve que $f(X)$ est borélien dans $Y$.

### 8. Le théorème du graphe souslinien

#### Théorème 4 {#top-ix-s6-thm-4 .statement}

Soient G et H deux groupes topologiques séparés et u un homomorphisme de groupes de G dans H. On suppose que G est un espace de Baire et que le graphe $\Gamma$ de u est un sous-espace souslinien de $G \times H$. Alors u est continu.

Nous démontrerons d’abord deux lemmes. Disons qu’une partie X d’un espace topologique E est approchable s’il existe un ouvert U de E tel $U \cap \mathcal{C}X$ et $X \cap \mathcal{C}U$ soient maigres dans E (cf. IX, p. 112, exerc. 6).

#### Lemme 8 {#top-ix-s6-lem-8 .statement}

Toute partie borélienne d’un espace topologique E est approchable.

Il suffit de montrer que l’ensemble $\mathfrak{E}$ des parties approchables de E est une tribu. Si $(X_n)$ et $(Y_n)$ sont deux suites de parties de E, on a
$$
(\bigcup X_n) \cap \mathcal{C} (\bigcup Y_n) \subset \bigcup (X_n \cap \mathcal{C} Y_n)
$$
ce qui entraîne aussitôt que toute réunion dénombrable d’ensembles de $\mathfrak{E}$ appartient à $\mathfrak{E}$. Soit d’autre part $X \in \mathfrak{E}$ et soit U un ouvert tel que $X \cap \mathcal{C}U$ et $U \cap \mathcal{C}X$ soient maigres. Soit V l’intérieur de $\mathcal{C}U$; alors $\mathcal{C}U \cap \mathcal{C}V$ est fermé d’intérieur vide, donc maigre. De plus. $V \cap X \subset \mathcal{C}U \cap X$ et
$$
\mathcal{C}X \cap \mathcal{C}V \subset (\mathcal{C}X \cap U) \cup (\mathcal{C}U \cap \mathcal{C}V)
$$
sont maigres. Par suite, $\mathcal{C}X \in \mathfrak{E}$ et $\mathfrak{E}$ est bien une tribu.

#### Remarque {#top-ix-s6-n8-rem-1 .statement}

On peut montrer que toute partie souslinienne d’un espace séparé E est approchable (exerc. 14).

#### Lemme 9 {#top-ix-s6-lem-9 .statement}

Soit G un groupe topologique et soit B une partie borélienne non maigre de G. Si G est un espace de Baire, $BB^{-1}$ est un voisinage de e.

Soit U un ouvert de G tel que $U \cap \mathcal{C}B$ et $B \cap \mathcal{C}U$ soient maigres (lemme 8). Alors U n’est pas maigre, donc est non vide. Par suite, il suffit de montrer que

UU^{-1} \subset BB^{-1}. Soit x \in UU^{-1}; l’ouvert U \cap xU n’est pas vide, donc est non maigre puisque G est un espace de Baire. Posons:

$$
Z = (U \cap xU) \cap (\mathbf{C} (B \cap xB))
$$

On a $Z \subset (U \cap \mathbf{C} B) \cup x(U \cap \mathbf{C} B)$, et Z est maigre. Par suite, $U \cap xU$ n’est pas contenu dans Z, et l’on a $B \cap xB \neq \varnothing$, i.e. $x \in BB^{-1}$, ce qui montre bien que $BB^{-1}$ est un voisinage de e.

Démontrons maintenant le th. 4. Comme $u(G) = pr_2(\Gamma)$ et que H est séparé, $u(G)$ est souslinien, donc possède une partie dénombrable dense D (IX, p. 59, prop. 4). Soit W un voisinage de e dans H. Montrons que $\bar{u}^1(W)$ n’est pas maigre. En effet, si $\bar{u}^1(W)$ était maigre, il en serait de même de chacun de ses translatés. Mais on a $u(G) \subset \bigcup_{x \in D} xW$ et G est donc réunion d’une famille dénombrable de translatés de $\bar{u}^1(W)$, ce qui contredit le fait que G est un espace de Baire.

Soit maintenant V un voisinage de e dans H, et soit W un voisinage ouvert de e tel que WW^{-1} \subset V. L’intersection $\bar{pr}_2^1(W) \cap \Gamma$ est ouverte dans $\Gamma$. Comme la restriction de $pr_1$ à $\Gamma$ est une application continue bijective de $\Gamma$ sur G, il résulte du cor. 2 du th. 2 de IX, p. 66 que $\bar{u}^1(W) = pr_1(\bar{pr}_2^1(W) \cap \Gamma)$ est un sous-ensemble borélien de G. Le lemme 9 montre alors que $\bar{u}^1(V)$, qui contient $\bar{u}^1(W) . \bar{u}^1(W)^{-1}$, est un voisinage de e, ce qui entraîne que $u$ est continue.

### 9. Sections boréliennes

#### Théorème 5 {#top-ix-s6-thm-5 .statement}

Soient X un espace polonais, R une relation d’équivalence dans X; supposons que les classes d’équivalence suivant R soient fermées dans X, et que le saturé pour R de tout ensemble ouvert soit borélien. Alors il existe un ensemble borélien dans X qui rencontre chaque classe d’équivalence suivant R en un point et un seul.

Considérons sur X une distance compatible avec la topologie et pour laquelle X soit complet. D’après le lemme 3 (IX, p. 64), il existe un criblage de X, défini par un crible C = (C_n, p_n) et une suite d’applications ($\varphi_n$). Pour chaque $c \in C_n$, soit $g_n(c)$ le saturé pour R de l’ensemble ouvert $\varphi_n(c)$; par hypothèse, $g_n(c)$ est borélien dans E.

Puisque chaque ensemble C_n est dénombrable, nous pouvons munir C_n, d’une relation d’ordre total pour laquelle l’ensemble des éléments plus petits qu’un élément donné soit fini. Par récurrence sur n, définissons, pour tout $c \in C_n$, un ensemble $h_n(c)$ de la façon suivante. En premier lieu, pour $c \in C_0$, $h_0(c)$ est l’intersection de $\varphi_0(c)$ et des ensembles $X - g_0(c')$, où $c' \in C_0$ et $c' < c$. Pour $c \in C_{n+1}$, $h_{n+1}(c)$ est l’intersection de $\varphi_{n+1}(c)$, de $h_n(p_n(c))$ et des ensembles $X - g_{n+1}(c')$ pour $c' \in C_{n+1}$, $p_n(c') = p_n(c)$ et $c' < c$. Il est clair que les $h_n(c)$ sont des ensembles boréliens.

Nous allons démontrer l’assertion suivante: pour tout entier $n \geqslant 0$ et toute classe d’équivalence $H$ suivant $R$, il existe un élément et un seul $c \in C_n$ tel que $h_n(c)$ rencontre $H$, et l’on a

$$
h_n(c) \cap H = \varphi_n(c) \cap H.
$$

Pour $n = 0$, considérons le plus petit élément $c \in C_0$ tel que $\varphi_0(c)$ rencontre $H$; alors $\varphi_0(c) \cap H$ ne rencontre aucun des $g_0(c')$ relatifs aux éléments $c' \in C_0$ tels que $c' < c$, donc est contenu dans $h_0(c) \cap H$, et par suite égal à cet ensemble; de plus, on a $H \subset g_0(c)$ et par suite, pour $c' \in C_0$ et $c' > c$, $h_0(c') \cap H$ est vide, et l’assertion est démontrée pour $n = 0$. Raisonnons par récurrence sur $n$; s’il existe $c \in C_{n+1}$ tel que $h_{n+1}(c)$ rencontre $H$, il résulte de la relation $h_{n+1}(c) \subset h_n(p_n(c))$ et de l’hypothèse de récurrence que $p_n(c)$ est l’unique élément $d \in C_n$ tel que $h_n(d)$ rencontre $H$. Observons que $h_n(d)$, qui est contenu dans $\varphi_n(d)$, est contenu dans la réunion des $\varphi_{n+1}(c)$ relatifs aux éléments $c \in p_n^{-1}(d)$, par définition d’un criblage; il y a donc un plus petit élément $c \in p_n^{-1}(d)$ tel que $\varphi_{n+1}(c)$ rencontre $H$. On a alors

$$
\varphi_{n+1}(c) \cap H \subset \varphi_n(d) \cap H = h_n(d) \cap H
$$

en vertu de l’hypothèse de récurrence. Donc

$$
\varphi_{n+1}(c) \cap H \subset \varphi_{n+1}(c) \cap h_n(d),
$$

et comme par définition $\varphi_{n+1}(c) \cap H$ ne rencontre aucun des ensembles $g_{n+1}(c')$ relatifs aux $c' \in p_n^{-1}(d)$ tels que $c' < c$, il s’ensuit par définition de $h_{n+1}(c)$ que $\varphi_{n+1}(c) \cap H = h_{n+1}(c) \cap H$. De plus, on a $H \subset g_{n+1}(c)$ et par suite, si $c' \in p_n^{-1}(d)$ et tel que $c' > c$, $h_{n+1}(c') \cap H$ est vide. Ainsi notre assertion est démontrée pour tout $n$.

Pour tout entier $n$, soit alors $S_n$ la réunion des ensembles $h_n(c)$, où $c$ parcourt $C_n$; l’ensemble $S_n$ est borélien, et on a $S_{n+1} \subset S_n$. Soit $S$ l’intersection des $S_n$, qui est un ensemble borélien dans $X$; on va voir que $S$ rencontre en un point et un seul toute classe d’équivalence $H$ suivant $R$. En effet, pour tout $n$, soit $c_n(H)$ l’unique élément $c \in C_n$ tel que $h_n(c)$ rencontre $H$; alors $S_n \cap H = \varphi_n(c_n(H)) \cap H$, et $S \cap H$ est l’intersection des $\varphi_n(c_n(H)) \cap H$. Comme la suite $(c_n(H))$ appartient à $L(C)$, chacun des ensembles $\varphi_n(c_n(H))$ contient l’adhérence dans $X$ de $\varphi_{n+1}(c_{n+1}(H))$ et le diamètre de $\varphi_n(c_n(H))$ tend vers 0, donc chacun des ensembles $\varphi_n(c_n(H)) \cap H$ contient l’adhérence dans $H$ de $\varphi_{n+1}(c_{n+1}(H)) \cap H$, et son diamètre tend vers 0; comme $H$ est fermé dans l’espace complet $X$, l’intersection des $\varphi_n(c_n(H)) \cap H$ est réduite à un point, ce qui achève de prouver le théorème.

#### Corollaire 1 {#top-ix-s6-thm-5-cor-1 .statement}

*La conclusion du th. 5 est encore valable lorsque le saturé pour R de tout ensemble fermé est borélien.*

En effet, comme un ensemble ouvert U de X est réunion dénombrable d’ensembles fermés F_n (IX, p. 16, prop. 7), le saturé de U est réunion des saturés des F_n, donc est borélien, et on peut appliquer le th. 5.

#### Corollaire 2 {#top-ix-s6-thm-5-cor-2 .statement}

Soit G un groupe topologique dont l’espace sous-jacent est polonais. Pour tout sous-groupe fermé H de G, il existe un ensemble borélien dans G qui rencontre toute classe à gauche xH dans G en un point et un seul.

En effet, la relation d’équivalence $x^{-1}y \in H$ est ouverte et séparée dans G (III, p. 10 et 12).

#### Remarque 1 {#top-ix-s6-n9-rem-1 .statement}

Dans l’énoncé du th. 5, on peut remplacer la tribu borélienne par une tribu quelconque contenant les ensembles ouverts de X; la démonstration est inchangée.

#### Remarque 2 {#top-ix-s6-n9-rem-2 .statement}

Lorsque X est un espace compact métrisable, le cor. 1 du th. 5 s’applique à toute relation d’équivalence séparée R dans X, puisqu’on sait qu’une telle relation est fermée (I, p. 63, corollaire 2).

### 10. Capacitabilité des ensembles sousliniens

#### Définition 9 {#top-ix-s6-def-9 .statement}

Soit X un espace topologique séparé. On appelle capacité sur X une application f de l’ensemble des parties $\mathfrak{P}(X)$ dans la droite numérique achevée $\overline{\mathbf{R}}$, qui satisfait aux conditions suivantes:

(CA_I) La relation $A \subset B$ entraîne $f(A) \leq f(B)$.

(CA_{II}) Pour toute suite croissante $(A_n)$ de parties de X, on a $f\left( \bigcup_n A_n \right) = \lim_{n \to \infty} f(A_n)$.

On dit qu’une capacité f est continue à droite si elle vérifie la condition:
(CA_{III}) Pour toute partie compacte K de X et tout nombre $a > f(K)$, il existe un ensemble ouvert U contenant K et tel que $f(U) < a$.

#### Exemple {#top-ix-s6-n10-exa-1 .statement}

*Soit $\mu$ une mesure positive sur un espace séparé X; la mesure extérieure $\mu^*$ et la mesure extérieure essentielle $\mu^*$ sont alors des capacités continues à droite sur X (voir INT, IX, § 1, n° 2 et n° 9, prop. 12, 13). On démontre que dans un espace $\mathbf{R}^n (n \geq 3)$, la « capacité extérieure newtonienne » est une capacité continue à droite au sens de la déf. 9.*¹

#### Remarque {#top-ix-s6-n10-rem-1 .statement}

Soit f une capacité continue à droite sur X, et soit $(K_n)$ une suite décroissante de parties compactes de X; si $K = \bigcap_n K_n$, tout ouvert U contenant K contient les $K_n$ à partir d’un certain rang (I, p. 60, th. 1 appliqué à l’espace $K_1$). Il résulte alors aussitôt de (CA_I) et (CA_{III}) que l’on a
$$
f(K) = \inf_n f(K_n).
$$

¹ Voir M. Brelot, Éléments de la théorie classique du potentiel, Centre de Documentation Universitaire, Paris, 1969, 4e édition.

#### Définition 10 {#top-ix-s6-def-10 .statement}

Soit $f$ une capacité sur $X$; on dit qu’une partie $A$ de $X$ est capacitable (pour $f$) si $f(A) = \sup_K f(K)$, où $K$ parcourt l’ensemble des parties compactes de $A$.

*Par exemple, si $\mu$ est une mesure sur $X$, et si $f$ est la mesure extérieure essentielle $\mu^*$, tout ensemble $\mu$-mesurable est capacitable (INT, IX, § 1).*

#### Théorème 6 {#top-ix-s6-thm-6 .statement}

Soient $X$ un espace séparé, $f$ une capacité continue à droite sur $X$. Tout sous-espace souslinien $Y$ de $X$ est alors capacitable pour $f$.

Considérons un espace polonais $P$ et une application continue $p$ de $P$ dans $X$ telle que $p(P) = Y$. En vertu de IX, p. 58, cor. 1, on peut supposer que $P$ est l’intersection d’une suite $(G_n)$ d’ensembles ouverts dans un espace compact métrisable $M$, telle que $G_0 = M$. Chaque ensemble $G_n$ est alors réunion d’une suite croissante $(K_{nm})_{m \geq 1}$ d’ensembles compacts dans $M$ (IX, p. 16, prop. 7).

Il est clair que $Y$ est capacitable si $f(Y) = -\infty$. Supposons donc $f(Y) > -\infty$, et soit $a$ un nombre réel tel que $f(Y) > a$. Tout revient à prouver qu’il existe un ensemble compact $K \subset Y$ tel que $f(K) > a$. À cet effet, nous allons construire par récurrence une suite décroissante $(T_n)$ de parties compactes de $M$, telles que l’on ait

(1) $T_n \subset G_n$ et $f(p(P \cap T_n)) > a$ pour tout $n$.

Nous prendrons $T_0 = M$. Supposons faite la construction de $T_n$; les ensembles compacts $K_{n+1,m}$ (pour $m \geq 1$) forment un recouvrement de $G_{n+1}$, donc aussi de $P \cap T_n$; l’ensemble $P \cap T_n$ est donc réunion croissante des

$$
P \cap T_n \cap K_{n+1,m} (m \geq 1);
$$

en vertu de (CA$_{\Pi}$) et de (1), il existe un entier $k$ tel que

$$
f(p(P \cap T_n \cap K_{n+1,k})) > a;
$$

il suffit alors de poser $T_{n+1} = T_n \cap K_{n+1,k}$ pour satisfaire à (1) où $n$ est remplacé par $n + 1$, et la récurrence peut se poursuivre.

Posons $T = \bigcap_n T_n$; l’ensemble compact $T$ est contenu dans $\bigcap_n G_n = P$, et $K = p(T)$ est donc un ensemble compact contenu dans $Y$. Soit $U$ un ensemble ouvert dans $X$ et contenant $K$; l’ensemble $V = p^{-1}(U)$ est ouvert dans $P$ et contient $T$, et il existe un ensemble $V'$ ouvert dans $M$ et tel que $P \cap V' = V$. Comme $V'$ contient $T$, il existe $n_0$ tel que $T_n \subset V'$ pour $n \geq n_0$ (I, p. 60, th. 1 appliqué à $T_1$), donc $V$ contient $P \cap T_n$ et $U$ contient alors $p(P \cap T_n)$. Il en résulte en particulier que $f(U) > a$; comme $U$ est un ouvert quelconque contenant $K$, la condition (CA$_{\mathrm{III}}$) entraîne $f(K) \geq a$.

C.Q.F.D.

#### Proposition 15 {#top-ix-s6-prop-15 .statement}

Soient $X$ un espace séparé, $f$ une capacité sur $X$ (non nécessairement continue à droite), $Y$ un sous-espace souslinien de $X$. Alors $Y$ est capacitable pour $f$ lorsque l’une des hypothèses suivantes est vérifiée:

(i) Pour toute suite décroissante $(H_n)$ de parties fermées de $X$, on a
$$
f\left(\bigcap_n H_n\right) = \inf_n f(H_n).
$$
(ii) Pour toute suite décroissante $(K_n)$ de parties compactes de $X$, on a
$$
f\left(\bigcap_n K_n\right) = \inf_n f(K_n),
$$
et $Y$ est contenu dans une réunion dénombrable de parties compactes de $X$.

Plaçons-nous d’abord dans l’hypothèse (i), et reprenons les notations de la démonstration du th. 6. Soit $x$ un point de $X$ n’appartenant pas à l’ensemble compact $K = p(T)$. Comme $X$ est séparé, l’intersection des voisinages fermés de $x$ dans $X$ est réduite à $x$ (I, p. 52, prop. 1), donc les traces de ces voisinages sur $K$ forment une base de filtre dont l’intersection est vide; l’un d’eux est donc vide (I, p. 59, axiome $(C'')$), autrement dit il existe un ensemble ouvert $U$ contenant $K$ et tel que $x \notin U$. Or, on a vu dans la démonstration du th. 6 que $U$ contient $p(P \cap T_n)$ dès que $n$ est assez grand. On a donc $x \notin \overline{p(P \cap T_n)}$. Autrement dit, les ensembles $\overline{p(P \cap T_n)}$ forment une suite décroissante d’ensembles fermés dont l’intersection est $K$; on en conclut par l’hypothèse (i) que
$$
f(K) = \inf_n f(\overline{p(P \cap T_n)}) \geq a,
$$
ce qu’il fallait démontrer.

Plaçons-nous maintenant dans l’hypothèse (ii); soit $(L_m)$ une suite croissante d’ensembles compacts telle que $Y \subset \bigcup_m L_m$, et posons $Y_m = Y \cap L_m$. Soit $a < f(Y)$; d’après $(CA_{II})$, on a $f(Y_m) > a$ dès que $m$ est assez grand. L’entier $m$ étant fixé de cette façon, on définit sur l’espace compact $L_m$ une capacité $g$ en posant $g(A) = f(A)$ pour $A \in \mathcal{P}(L_m)$; les axiomes $(CA_I)$ et $(CA_{II})$ sont en effet trivialement vérifiés. En outre, cette capacité vérifie cette fois l’hypothèse (i), en raison de l’hypothèse (ii) sur $f$; il existe par suite un ensemble compact $K \subset Y_m$ tel que $g(K) = f(K) \geq a$, ce qui achève de démontrer la proposition.

## EXERCICES {#top-ix-s6-exercises}

See the [exercises for § 6](exercises/s6/).
