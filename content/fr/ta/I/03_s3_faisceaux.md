---
book: ta
book_title: Topologie algébrique
chapter: I
chapter_title: REVÊTEMENTS
section: 3
section_title: Faisceaux
lang: fr
source: ta-i-iv-fr
book_pages: TA I.42-TA I.67, TA I.141-TA I.145
pdf_pages: 0058-0083, 0157-0161
extraction: native
subsections:
    - "no": 1
      title: Faisceaux d’ensembles
      page: 42
      pdf_page: 58
    - "no": 2
      title: Sous-faisceaux d’un faisceau
      page: 44
      pdf_page: 60
    - "no": 3
      title: Exemples de faisceaux
      page: 44
      pdf_page: 60
    - "no": 4
      title: Morphismes de préfaisceaux
      page: 47
      pdf_page: 63
    - "no": 5
      title: Espace étalé associé à un préfaisceau
      page: 49
      pdf_page: 65
    - "no": 6
      title: Faisceau associé à un préfaisceau
      page: 53
      pdf_page: 69
    - "no": 7
      title: Image directe et image réciproque d’un faisceau
      page: 57
      pdf_page: 73
    - "no": 8
      title: Les homomorphismes $\alpha \mathbf{e}\mathbf{t}\beta$ ; adjonction
      page: 59
      pdf_page: 75
    - "no": 9
      title: Faisceaux mous
      page: 64
      pdf_page: 80
    - "no": 10
      title: Faisceaux de structures
      page: 66
      pdf_page: 82
statements: 35
exercises: 8
content_sha256: b1dbe3984831e516a2148fa2209ce4ed470ed4767346646462742a4b69914881
---

## § 3. FAISCEAUX

### 1. Faisceaux d’ensembles

Soit B un espace topologique.

#### Définition 1 {#ta-i-s3-def-1 .statement tag=01NS}

Un préfaisceau sur B, relatif à une base $\mathscr{B}$ de la topologie de B, est un système projectif d’ensembles, relatif à l’ensemble d’indices $\mathscr{B}$ ordonné par la relation d’inclusion.

Autrement dit (E, III, p. 52), un préfaisceau $\mathscr{F}$ sur B relatif à $\mathscr{B}$ est un couple $((\mathscr{F}(U))_{U\in\mathscr{B}},(f_{UV}))$, que l’on note aussi $(\mathscr{F}(U), f_{UV})$, où $((\mathscr{F}(U))_{U\in\mathscr{B}}$ est une famille d’ensembles ayant $\mathscr{B}$ pour ensemble d’indices et où pour chaque couple $(U,V)$ d’éléments de $\mathscr{B}$ tel que $U\subset V,f_{UV}$ est une application de $\mathscr{F}(V)$ dans $\mathscr{F}(U)$, ces applications vérifiant les conditions suivantes :

(PF$_1)$ Les relations $U\subset V\subset W$ entraînent $f_{UW}=f_{UV}\circ f_{VW}$;

(PF$_2)$ Pour tout ouvert U $\in \mathscr{B},f_{UU}$ est l’application identique de

$$
\mathscr{F}(U)
$$

Un préfaisceau sur B relatif à l’ensemble des parties ouvertes de B est simplement appelé préfaisceau sur B.

Soit $\mathscr{F}= (\mathscr{F}(U), f_{UV})$ un préfaisceau sur B, relatif à une base $\mathscr{B}$ de la topologie de B. Soit U un élément de la base $\mathscr{B}$. Les éléments de $\mathscr{F}(U)$ s’appellent les sections de $\mathscr{F}$ sur U. Si V est un élément de la base $\mathscr{B}$ contenant U et $s$ un élément de $\mathscr{F}(V)$, l’élément $f_{UV}(s)$ de $\mathscr{F}(U)$ s’appelle la restriction de $s$ à U. Si aucune ambiguïté n’est à craindre sur les applications $f_{UV}$, on notera $s|U$ la restriction de $s$ à U.

Soient $B'$ une partie ouverte de B et $\mathscr{B}'$ une base de la topologie de $B'$ telle que $\mathscr{B}'\subset \mathscr{B}$. On appelle préfaisceau sur $B'$, relatif à $\mathscr{B}'$, déduit de $\mathscr{F}$ par restriction, et on note $\mathscr{F}|\mathscr{B}'$, le système projectif $((\mathscr{F}(U))_{U\in\mathscr{B}'},(f_{UV}))$ déduit de $\mathscr{F}$ par restriction à $\mathscr{B}'$ de l’ensemble d’indices (loc. cit.). Lorsque $\mathscr{F}$ est un préfaisceau sur B et que $\mathscr{B}'$ est l’ensemble des parties ouvertes de $B'$, le préfaisceau $\mathscr{F}|\mathscr{B}'$ est aussi noté $\mathscr{F}|B'$ et appelé préfaisceau déduit de $\mathscr{F}$ par restriction à $B'$.

#### Définition 2 {#ta-i-s3-def-2 .statement tag=01NT}

Soit $\mathscr{F}= (\mathscr{F}(U), f_{UV})$ un préfaisceau sur B. On dit que $\mathscr{F}$ est un faisceau sur B si, pour toute partie ouverte U de B et toute famille $(U_i)_{i\in I}$ de parties ouvertes de B, de réunion U, les propriétés suivantes sont satisfaites :

$(F_1)$ L’application $(f_{U_iU})_{i\in I}:\mathscr{F}(U)\rightarrow \prod_{i\in I}\mathscr{F}(U_i)$ est injective ;

$(F_2)$ Pour toute famille $(s_i)\in \prod_{i\in I}\mathscr{F}(U_i)$ telle que $f_{(U_i\cap U_j)U_i}(s_i) =$

$f_{(U_i\cap U_j)U_j}(s_j)$ pour tout couple $(i, j)\in I\times I$, il existe un élément $s$

de $\mathscr{F}(U)$ tel que pour tout $i\in I$, on ait $f_{U_iU}(s) =s_i$.

#### Remarque {#ta-i-s3-n1-rem-1 .statement tag=01NU}

Soit $\mathscr{F}$ un préfaisceau sur B. Pour tout ouvert U de B, $f_{\emptyset U}$ est une application de $\mathscr{F}(U)$ dans $\mathscr{F}(\emptyset )$, donc $\mathscr{F}(\emptyset )$ n’est pas vide dès qu’il existe un ouvert U pour lequel $\mathscr{F}(U)$ n’est pas vide. Si $\mathscr{F}$ est un faisceau, $\mathscr{F}(\emptyset )$ est un ensemble à un élément ; on le voit en appliquant $(F_1)$ et $(F_2)$ au recouvrement de l’ensemble vide par la famille vide ($I =\emptyset$ ).

Soit $\mathscr{F}$ un faisceau sur B et soit $B'$ une partie ouverte de B ; le préfaisceau $\mathscr{F}|B'$ déduit de $\mathscr{F}$ par restriction à $B'$ est un faisceau, appelé le faisceau déduit de $\mathscr{F}$ par restriction à $B'$.

### 2. Sous-faisceaux d’un faisceau

Soit B un espace topologique. Soit $\mathscr{F}= (\mathscr{F}(U), f_{UV})$ un préfaisceau sur B, relatif à une base $\mathscr{B}$ de la topologie de B.

Supposons donné, pour tout ouvert $U\in \mathscr{B}$, un sous-ensemble $\mathscr{L}(U)$ de $\mathscr{F}(U)$. Si l’on a $f_{UV}(\mathscr{L}(V))\subset \mathscr{L}(U)$ pour tout couple $(U,V)$ d’éléments de $\mathscr{B}$ tel que $U\subset V$, le couple $\mathscr{L}= ((\mathscr{L}(U))_{U\in\mathscr{B}},(f'_{UV}))$, où $f'_{UV}:\mathscr{L}(V)\rightarrow \mathscr{L}(U)$ est l’application déduite de $f_{UV}$, est un préfaisceau. Un tel préfaisceau s’appelle un sous-préfaisceau de $\mathscr{F}$. Comme les applications $f'_{UV}$ sont déterminées par la donnée du préfaisceau $\mathscr{F}$ et de la famille $(\mathscr{L}(U))_{U\in\mathscr{B}}$, on dit aussi par abus de langage que la famille $(\mathscr{L}(U))_{U\in\mathscr{B}}$ est un sous-préfaisceau de $\mathscr{F}$.

Supposons maintenant que $\mathscr{F}$ soit un faisceau sur B et soit, pour toute partie ouverte U de B$,\mathscr{L}(U)$, un sous-ensemble de $\mathscr{F}(U)$. Pour que $(\mathscr{L}(U))_{U\in\mathscr{B}}$ soit un sous-préfaisceau de $\mathscr{F}$, et que ce préfaisceau soit un faisceau, il faut et il suffit que la condition suivante soit satisfaite :

(F) Soient $(U_i)_{i\in I}$ une famille d’ouverts de B, U sa réunion, et $s$ un

élément de $\mathscr{F}(U)$. Pour que $s$ appartienne à $\mathscr{L}(U)$, il faut et il

suffit que pour tout $i$ dans I$,f_{U_iU}(s)$ appartienne à $\mathscr{L}(U_i)$.

En effet, si la condition (F) est réalisée, on a $f_{UV}(\mathscr{L}(V))\subset \mathscr{L}(U)$ pour tout couple $(U,V)$ d’ouverts de B tels que $U\subset V$ et les propriétés $(F_1)$ et $(F_2)$ relatives au sous-préfaisceau $(\mathscr{L}(U))$ résultent des propriétés analogues relatives au faisceau $\mathscr{F}$. La réciproque est immédiate.

Lorsque la condition (F) est satisfaite, on dit que $(\mathscr{L}(U))$ est un sous-faisceau du faisceau $\mathscr{F}$.

### 3. Exemples de faisceaux

Soit B un espace topologique.

1) Faisceaux d’applications

Soit X un ensemble. Pour tout ouvert U de B, on note $\mathscr{F}(U; X)$ l’ensemble des applications de U dans X (E, II, p. 31). Pour tout couple $(U,V)$ d’ouverts de B tel que $U\subset V$, soit $r_{UV}:\mathscr{F}(V; X)\rightarrow$ $\mathscr{F}(U; X)$ l’application de restriction $f\mapsto f|U$. Il est clair que le couple $(\mathscr{F}(U; X), r_{UV})$ est un faisceau sur B. On l’appelle le faisceau sur B des applications à valeurs dans X, et on le note $\mathscr{F}(B; X)$.

2) Faisceaux d’applications continues

Soit X un espace topologique. Pour tout ouvert U de B, soit $\mathscr{C}(U; X)$ l’ensemble des applications continues de U dans X. Alors, $(\mathscr{C}(U; X))$ est un sous-faisceau du faisceau $\mathscr{F}(B; X)$ d’après la prop. 4 de TG, I, p. 19. Le faisceau ainsi obtenu est noté $\mathscr{C}(B; X)$ et appelé le faisceau sur B des applications continues à valeurs dans X. Dans le cas particulier où X est muni de la topologie discrète, le faisceau $\mathscr{C}(B; X)$ prend le nom de faisceau sur B des applications localement constantes à valeurs dans X.

3) Faisceaux de sections continues

Soit E un espace topologique et soit $p: E\rightarrow B$ une application continue. Pour tout ouvert U de B, on note $\mathscr{S}(U;p)$ (ou $\mathscr{S}(U; E)$ lorsqu’il n’y a pas de confusion possible) l’ensemble des sections continues de $p$ au-dessus de U. La famille $(\mathscr{S}(U;p))$ est un sous-faisceau du faisceau

$\mathscr{C}\mathscr{S}(E$(B; E)$(E), p)$. Nous verrons au net appelé le. Le faisceau ainsi obtenu est notéfaisceau sur$_o6$ ci-dessous que tout faisceau surB des sections continues du$\mathscr{S}(B; E)$ ou simplementBB-espaceest isomorphe au faisceau sur B des sections continues d’un B-espace étalé.

4) Faisceaux de B-morphismes

Soient $(E, p)$ et $(E', p')$ des B-espaces. Pour tout ouvert U de E, on note $\mathscr{C}_B(U; E')$ l’ensemble des B-morphismes de $(U, p|U)$ dans $(E', p')$. La famille $(\mathscr{C}_B(U; E'))$ est un sous-faisceau du faisceau $\mathscr{C}(E; E')$. Le faisceau ainsi obtenu est noté $\mathscr{C}_B(E; E')$ et appelé le faisceau sur E des B-morphismes à valeurs dans $(E', p')$. Lorsque $(E, p)$ est égal à $(B$, Id$_B)$, ce faisceau est le faisceau $\mathscr{S}(B; E)$ de l’exemple 3.

Pour tout ouvert U de B, soit $\mathscr{M}(U)$ l’ensemble des U-morphismes

de $\overset{-1}{p}(U)$ dans $(^-{p'}^1)(U)$. Pour tout couple $(U,V)$ d’ouverts de B tel que $U\subset V$, soit $m_{UV}:\mathscr{M}(V)\rightarrow \mathscr{M}(U)$ l’application qui à un V-morphisme

$f:\overset{-1}{p}(V)\rightarrow (^-{p'}^1)(V)$ associe le U-morphisme de $\overset{-1}{p}(U)$ dans $(^-{p'}^1)(U)$ déduit de $f$ par passage aux sous-ensembles. Alors $(\mathscr{M}(U), m_{UV})$ est un faisceau sur B. On le note $\mathscr{M}$or$_B(E; E')$ et on l’appelle le faisceau sur B des B-morphismes de $(E, p)$ dans $(E', p')$.

Pour tout ouvert U de B, soit $\mathscr{I}$s(U) le sous-ensemble de $\mathscr{M}(U)$

constitué des U-isomorphismes de $\overset{-1}{p}(U)$ dans $(^-{p'}^1)(U)$. La famille $(\mathscr{I}$s(U)) est un sous-faisceau du faisceau $\mathscr{M}$or$_B(E; E')$ des morphismes de $(E, p)$ dans $(E', p')$. Le faisceau ainsi obtenu est noté $\mathscr{I}$som$_B(E; E')$ et appelé faisceau sur B des B-isomorphismes de $(E, p)$ dans $(E', p')$.

5) Faisceaux d’applications de classe $C^r$

Soient X et Y des variétés de classe $C^r$ sur un corps K (les conventions sur K et $r$ étant celles de VAR, R). Pour tout ouvert U de X, soit $\mathscr{C}^r(U; Y)$ l’ensemble des morphismes de classe $C^r$ de U dans Y. La famille $(\mathscr{C}^r(U; Y))$ est un sous-faisceau du faisceau $\mathscr{C}(X; Y)$. Le faisceau ainsi obtenu est noté $\mathscr{C}^r(X; Y)$ et appelé le faisceau sur X des applications de classe $C^r$ à valeurs dans Y (cf. VAR, R, 5.4.2).

6) Faisceaux de sous-espaces

Si U et V sont des ouverts de B tels que $U\subset V$, notons $i_{UV}:\mathfrak{P}(V)\rightarrow$ $\mathfrak{P}(U)$ l’application qui, à une partie A de V, associe $A\cap U$. Le couple $(\mathfrak{P}(U), i_{UV})$ est un faisceau, appelé faisceau des sous-espaces de B et noté $\mathfrak{P}(B)$. En effet, si l’on note X l’ensemble $\{0; 1\}$, l’application qui à toute partie A de U associe sa fonction caractéristique $\varphi^U_A: U\rightarrow X$ est une bijection de $\mathfrak{P}(U)$ sur $\mathscr{F}(U; X)$ (E, III, p. 38) ; de plus, si U et V sont des ouverts tels que $U\subset V$, pour toute partie A de V$,\varphi^U_{A\cap U}$ est la restriction à U de $\varphi^V_A$ de sorte que $\mathfrak{P}(B)$ s’identifie au faisceau sur B des applications à valeurs dans X.

Soit, pour tout ouvert U de B$,\mathscr{L}(U)$ une partie de $\mathfrak{P}(U)$. Pour que $(\mathscr{L}(U))$ soit un sous-faisceau de $\mathfrak{P}(B)$, il faut et il suffit que la condition suivante soit satisfaite :

$(F')$ Soient $(U_i)_{i\in I}$ une famille d’ouverts de B, U sa réunion, et A un

sous-ensemble de U ; pour que A appartienne à $\mathscr{L}(U)$, il faut et

il suffit que pour tout $i$ dans I, $A\cap U_i$ appartienne à $\mathscr{L}(U_i)$.

Par exemple, si $\mathscr{L}(U)$ est l’ensemble des parties fermées de U, la condition $(F')$ est satisfaite.

7) Produits de faisceaux

Soit $\mathscr{B}$ une base de la topologie de B et soit I un ensemble. Pour tout $i\in I$, soit $\mathscr{F}_i= (\mathscr{F}_i(U), f_{i,UV})$ un préfaisceau sur B relatif à la base $\mathscr{B}$. Pour tout ouvert $U\in \mathscr{B}$, posons $\mathscr{F}(U) =\prod_{i\in I}\mathscr{F}_i(U)$, et pour tout couple $(U,V)$ d’éléments de $\mathscr{B}$ tel que $U\subset V$, notons $f_{UV}$ l’application $(f_{i,UV})_{i\in I}:\mathscr{F}(V)\rightarrow \mathscr{F}(U)$. Alors $(\mathscr{F}(U), f_{UV})$ est un préfaisceau sur B relatif à $\mathscr{B}$ appelé le préfaisceau produit de la famille $(\mathscr{F}_i)$ et noté $\prod_{i\in I}\mathscr{F}_i$. C’est un faisceau si pour tout $i\in I,\mathscr{F}_i$ est un faisceau.

### 4. Morphismes de préfaisceaux

#### Définition 3 {#ta-i-s3-def-3 .statement tag=01NV}

Soient B un espace topologique, $\mathscr{B}$ une base de la topologie de B$,\mathscr{F}= (\mathscr{F}(U), f_{UV})$ et $\mathscr{G}= (\mathscr{G}(U), g_{UV})$ des préfaisceaux sur B relatifs à $\mathscr{B}$. On appelle morphisme de préfaisceaux de $\mathscr{F}$ dans $\mathscr{G}$ un système projectif d’applications de $\mathscr{F}$ dans $\mathscr{G}$.

Autrement dit (E, III, p. 54), un morphisme de préfaisceaux de $\mathscr{F}$ dans $\mathscr{G}$ est une famille $(\varphi_U)_{U\in\mathscr{B}}$ telle que :

(MPF$_1)$ Pour tout ouvert U appartenant à $\mathscr{B},\varphi_U$ est une application

de $\mathscr{F}(U)$ dans $\mathscr{G}(U)$ ;

(MPF$_2)$ Pour tout couple $(U,V)$ d’ouverts appartenant à $\mathscr{B}$ tels que

$U\subset V$, on a $\varphi_U\circ f_{UV}=g_{UV}\circ \varphi_V$.

Lorsque $\mathscr{F}$ et $\mathscr{G}$ sont des faisceaux, un morphisme de préfaisceaux de $\mathscr{F}$ dans $\mathscr{G}$ est aussi appelé un morphisme de faisceaux. Si $\mathscr{F}$ et $\mathscr{G}$ sont des préfaisceaux sur B relatifs à $\mathscr{B}$, les morphismes de préfaisceaux de $\mathscr{F}$ dans $\mathscr{G}$ constituent un ensemble noté Mor($\mathscr{F};\mathscr{G}$). Au lieu de dire : « soit $\varphi$ un morphisme de préfaisceaux de $\mathscr{F}$ dans $\mathscr{G}$ », on dira souvent « soit $\varphi :\mathscr{F}\rightarrow \mathscr{G}$ un morphisme de préfaisceaux ».

Soient $\mathscr{F},\mathscr{G},\mathscr{H}$ des préfaisceaux sur B relatifs à $\mathscr{B}$ et $\varphi :\mathscr{F}\rightarrow \mathscr{G}$, $\psi :\mathscr{G}\rightarrow \mathscr{H}$ des morphismes de préfaisceaux. La famille $(\psi_U\circ \varphi_U)_{U\in\mathscr{B}}$ est un morphisme de préfaisceaux de $\mathscr{F}$ dans $\mathscr{H}$ que l’on note $\psi \circ \varphi$. La famille (Id$_{\mathscr{F}(U)})_{U\in\mathscr{B}}$ est un morphisme de préfaisceaux de $\mathscr{F}$ dans lui-même que l’on note Id$_{\mathscr{F}}$.

Pour qu’un morphisme de préfaisceaux $\varphi = (\varphi_U):\mathscr{F}\rightarrow \mathscr{G}$ soit un isomorphisme, il faut et il suffit que, pour tout ouvert U de $\mathscr{B},\varphi_U$ soit une bijection de $\mathscr{F}(U)$ sur $\mathscr{G}(U)$. Il est équivalent de dire qu’il existe un morphisme de préfaisceaux $\psi :\mathscr{G}\rightarrow \mathscr{F}$ tel que $\psi \circ \varphi =$ Id$_{\mathscr{F}}$ et $\varphi \circ \psi =$ Id$_{\mathscr{G}}$.

Soient $\mathscr{F}$ et $\mathscr{G}$ des préfaisceaux sur B, relatifs à une base $\mathscr{B}$ de la topologie de B, soit $B'$ une partie ouverte de B et soit $\mathscr{B}'$ une base de la topologie de $B'$ telle que $\mathscr{B}'\subset \mathscr{B}$. Soit $\varphi = (\varphi_U)_{U\in\mathscr{B}}$ un morphisme de préfaisceaux de $\mathscr{F}$ dans $\mathscr{G}$. Alors $(\varphi_U)_{U\in\mathscr{B}'}$ est un morphisme de préfaisceaux de $\mathscr{F}|\mathscr{B}'$ dans $\mathscr{G}|\mathscr{B}'$, que l’on note $\varphi |\mathscr{B}'$. Lorsque $\mathscr{B}$ est l’ensemble des parties ouvertes de B et $\mathscr{B}'$ l’ensemble des parties ouvertes de $B',\varphi |\mathscr{B}'$ est un morphisme de préfaisceaux de $\mathscr{F}|B'$ dans $\mathscr{G}|B'$ et est aussi noté $\varphi |B'$.

#### Exemple 1 {#ta-i-s3-n4-exa-1 .statement tag=01NW}

Soit B un espace topologique, soient $(E, p)$ et $(E', p')$ des B-espaces et soit $f: E\rightarrow E'$ un B-morphisme. Pour tout ouvert U de B, on définit l’application $f_U:\mathscr{S}(U; E)\rightarrow \mathscr{S}(U; E')$ par $f_U(s) =$ $f\circ s$. La famille $\mathscr{S}(f) = (f_U)$ est un morphisme de préfaisceaux de $\mathscr{S}(B; E)$ dans $\mathscr{S}(B; E')$. Si $(E'', p'')$ est un B-espace et $g: E'\rightarrow E''$ un B-morphisme, on a $\mathscr{S}(g\circ f) =\mathscr{S}(g)\circ \mathscr{S}(f)$.

#### Exemple 2 {#ta-i-s3-n4-exa-2 .statement tag=01NX}

Soient B un espace topologique, $\mathscr{B}$ une base de la topologie de B, $\mathscr{F}= (\mathscr{F}(U), f_{UV})$ un préfaisceau sur B relatif à $\mathscr{B}$ et $\mathscr{L}= (\mathscr{L}(U))$ un sous-préfaisceau de $\mathscr{F}$. Pour tout ouvert $U\in \mathscr{B}$, notons $i_U$ l’injection canonique de $\mathscr{L}(U)$ dans $\mathscr{F}(U)$. Alors $i= (i_U)_{U\in\mathscr{B}}$ est un morphisme de préfaisceaux de $\mathscr{L}$ dans $\mathscr{F}$. On dit que $i$ est le morphisme canonique de $\mathscr{L}$ dans $\mathscr{F}$.

#### Exemple 3 {#ta-i-s3-n4-exa-3 .statement tag=01NY}

Soient B un espace topologique, $\mathscr{B}$ une base de la topologie de B et I un ensemble. Pour tout $i\in I$, soit $\mathscr{F}_i= (\mathscr{F}_i(U), f_{i,UV})$ un préfaisceau sur B relatif à $\mathscr{B}$. Notons $\mathscr{F}$ le préfaisceau produit de la famille $(\mathscr{F}_i)_{i\in I}$. Pour tout ouvert $U\in \mathscr{B}$, on a $\mathscr{F}(U) =\prod_{i\in I}\mathscr{F}_i(U)$; pour tout $i\in I$, notons pr$_{i,U}:\mathscr{F}(U)\rightarrow \mathscr{F}_i(U)$ la projection d’indice $i$. Il résulte immédiatement de la définition du préfaisceau $\mathscr{F}$ que la famille pr$_i$ = (pr$_{i,U})_{U\in\mathscr{B}}$ est un morphisme de préfaisceaux de $\mathscr{F}$ dans $\mathscr{F}_i$. Le morphisme pr$_i$ est appelé le morphisme de projection d’indice $i$. Pour tout préfaisceau $\mathscr{F}'$ sur B relatif à $\mathscr{B}$ et toute famille $(\psi_i)_{i\in I}$, où $\psi_i$ est un morphisme de préfaisceaux de $\mathscr{F}'$ dans $\mathscr{F}_i$, il existe un unique morphisme de préfaisceaux $\psi :\mathscr{F}'\rightarrow \mathscr{F}$ tel que pour tout $i\in I$, pr$_i\circ \psi =\psi_i$.

#### Exemple 4 {#ta-i-s3-n4-exa-4 .statement tag=01NZ}

Soit X une variété différentielle de classe $C^{\infty}$ sur $\mathbf{R}$ et soit $\mathscr{C}^{\infty}(X;\mathbf{R})$ le faisceau sur X des fonctions numériques de classe $C^{\infty}$. Si P est un opérateur différentiel à coefficients $C^{\infty}$ sur X, la famille des restrictions de P aux ouverts de X est un morphisme du faisceau $\mathscr{C}^{\infty}(X;\mathbf{R})$ dans lui-même. On peut démontrer qu’inversement, tout morphisme $\mathbf{R}$-linéaire du faisceau $\mathscr{C}^{\infty}(X;\mathbf{R})$ dans lui-même est localement de cette forme (I, p. 142, exerc. 3).

### 5. Espace étalé associé à un préfaisceau

Soient B un espace topologique, $\mathscr{B}$ une base de la topologie de B et $\mathscr{F}= (\mathscr{F}(U), r_{UV})$ un préfaisceau sur B relatif à la base $\mathscr{B}$. Soit L l’ensemble des couples $(U, s)$ avec U $\in \mathscr{B}$ et $s\in \mathscr{F}(U)$. Notons $X_{\mathscr{F}}$ l’espace somme de la famille $(U)_{(U,s)\in L}$. Ainsi $X_{\mathscr{F}}$ est l’ensemble des triplets $(U, s, x)$ où $U\in \mathscr{B},s\in \mathscr{F}(U),x\in U$. Soit $R_{\mathscr{F}}$ la relation dans l’ensemble $X_{\mathscr{F}}$ définie par $R_{\mathscr{F}}((U, s, x),(U', s', x'))$ si et seulement si « $x$ = $x'$ et il existe W $\in \mathscr{B}$ tel que $x\in W$, W $\subset U\cap U'$ et $r_{WU}(s) =r_{WU'}(s')$ ». La relation $R_{\mathscr{F}}$ est une relation d’équivalence dans $X_{\mathscr{F}}:$ elle est, par définition, réflexive et symétrique ; démontrons qu’elle est transitive. Soient $\xi = (U, s, x),\xi '= (U', s', x')$ et $\xi ''$ = $(U'', s'', x'')$ des éléments de $X_{\mathscr{F}}$ tels que l’on ait $R_{\mathscr{F}}(\xi , \xi ')$ et $R_{\mathscr{F}}(\xi ', \xi '')$. On a alors $x=x'$ = $x''$ et il existe deux éléments $W'$ et $W''$ de $\mathscr{B}$ contenant $x$ tels que $W'\subset U\cap U',W''\subset U'\cap U'',r_{W'U}(s) =$ $r_{W'U'}(s'),r_{W''U'}(s') =r_{W''U''}(s'')$. Soit W un élément de $\mathscr{B}$ contenant $x$ et contenu dans $W'\cap W''$. On a alors $W\subset U\cap U''$,

$$
r_{WU}(s) =r_{WW'}\circ r_{W'U}(s) =r_{WW'}\circ r_{W'U'}(s') =r_{WU'}(s')
$$

et, de même, $r_{WU'}(s') =r_{WU''}(s'')$. Par conséquent, on a $R_{\mathscr{F}}(\xi , \xi '')$ et la relation $R_{\mathscr{F}}$ est transitive.

Notons $E_{\mathscr{F}}$ l’ensemble quotient $X_{\mathscr{F}}/R_{\mathscr{F}}$ et $[U, s, x]$ l’image canonique dans $E_{\mathscr{F}}$ d’un élément $(U, s, x)$ de $X_{\mathscr{F}}$. Pour $U\in \mathscr{B}$ et $s\in \mathscr{F}(U)$, notons $\sigma_{\mathscr{F}}(U, s): U\rightarrow E_{\mathscr{F}}$ l’application $x\mapsto [U, s, x]$. Munissons l’ensemble $E_{\mathscr{F}}$ de la topologie quotient, c’est-à-dire de la topologie la plus fine rendant continues les applications $\sigma_{\mathscr{F}}(U, s)$ pour $U\in \mathscr{B}$ et $s\in \mathscr{F}(U)$. L’application pr$_3: X_{\mathscr{F}}\rightarrow B$ définit par passage au quotient une application continue $p: E_{\mathscr{F}}\rightarrow B$ : on a $p([U, s, x]) =x$.

#### Proposition 1 {#ta-i-s3-prop-1 .statement tag=01O0}

L’application $p: E_{\mathscr{F}}\rightarrow$ B est étale. Pour tout ouvert $U\in \mathscr{B}$ et tout $s\in \mathscr{F}(U)$, l’application $\sigma_{\mathscr{F}}(U, s)$ est donc une section continue de $p$ au-dessus de U.

Soient $\lambda = (U, s)$ et $\mu= (U', s')$ des éléments de L. Par définition de la relation $R_{\mathscr{F}}$, l’ensemble $A_{\lambda \mu}$ des points $x$ de $U\cap U'$ en lesquels $\sigma_{\mathscr{F}}(U, s)$ et $\sigma_{\mathscr{F}}(U', s')$ coïncident est l’intérieur dans B, de l’ensemble des $x\in U\cap U'$ tels que $s(x) =s'(x)$. Il en résulte que $A_{\mu\lambda}= A_{\lambda \mu}$. On note alors $h_{\mu\lambda}: A_{\lambda \mu}\rightarrow A_{\mu\lambda}$ l’application Id$_{A_{\lambda \mu}}$. L’ensemble $E_{\mathscr{F}}$ est obtenu par recollement des ouverts U le long des $A_{\lambda \mu}$ au moyen des bijections $h_{\mu\lambda}$ (TG, I, p. 16). D’après la prop. 9 de TG, I, p. 17, l’application $\sigma_{\mathscr{F}}(U, s)$ induit un homéomorphisme de U sur une partie ouverte de $E_{\mathscr{F}}$. Cela prouve que l’application $p$ est étale (I, p. 33, prop 9).

Pour tout ouvert $U\in \mathscr{B}$ et tout $s\in \mathscr{F}(U)$, on a $\sigma_{\mathscr{F}}(U, s)(x) =$ $[U, s, x]$ pour tout $x\in U$. La seconde assertion découle donc de la définition de $p$.

#### Définition 4 {#ta-i-s3-def-4 .statement tag=01O1}

Le B-espace étalé $(E_{\mathscr{F}}, p)$ défini ci-dessus est appelé le B-espace étalé associé au préfaisceau $\mathscr{F}$. Pour $x\in B$, la fibre de $E_{\mathscr{F}}$ en $x$ est appelée la tige du préfaisceau $\mathscr{F}$ en $x$ et est notée $\mathscr{F}_x$. Pour tout ouvert $U\in \mathscr{B}$, toute section $s\in \mathscr{F}(U)$ de $\mathscr{F}$ sur U et tout point $x$ de U, l’élément $[U, s, x]$ de $E_{\mathscr{F}}$ est appelé le germe en $x$ de la section $s$.

Soit $a$ un point de B. L’ensemble $\mathscr{B}(a)$ des ouverts $U\in \mathscr{B}$ contenant $a$ et ordonné par la relation $\supset$ est filtrant. On déduit de $\mathscr{F}$, par restriction à $\mathscr{B}(a)$ de l’ensemble d’indices, un système inductif $((\mathscr{F}(U))_{U\in\mathscr{B}(a)},(r_{UV}))$. Par définition (E, III, p. 60), la limite inductive de ce système est le quotient de l’ensemble des couples $(U, s)$ tels que $a\in U$ et $s\in \mathscr{F}(U)$ par la relation d’équivalence R définie par $R((U, s),(U', s'))$ si et seulement s’il existe W $\in \mathscr{B}$ contenant $a$ et contenu dans $U\cap U'$ et tel que $r_{WU}(s) =r_{WU'}(s')$. Cette limite s’identifie donc à la tige $\mathscr{F}_a$ de $\mathscr{F}$ en $a$, par définition des limites inductives.

Soit $\mathscr{G}$ un préfaisceau sur B relatif à la base $\mathscr{B}$ et soit $\varphi = (\varphi_U)_{U\in\mathscr{B}}$ un morphisme de préfaisceaux de $\mathscr{F}$ dans $\mathscr{G}$. L’application $(U, s, x)\mapsto$ $(U, \varphi_U(s), x)$ de $X_{\mathscr{F}}$ dans $X_{\mathscr{G}}$ est compatible avec les relations d’équivalence $R_{\mathscr{F}}$ et $R_{\mathscr{G}}$, par définition d’un morphisme de préfaisceaux. Notons $E(\varphi ): E_{\mathscr{F}}\rightarrow E_{\mathscr{G}}$ l’application qui s’en déduit par passage aux quotients. Pour tout $U\in \mathscr{B}$ et tout $s\in \mathscr{F}(U)$, on a

$$
E(\varphi )\circ \sigma_{\mathscr{F}}(U, s) =\sigma_{\mathscr{G}}(U, \varphi_U(s))
$$

par suite, l’application $E(\varphi )$ est continue. L’application $E(\varphi )$ est un B-morphisme ; on dit que c’est le B-morphisme de $E_{\mathscr{F}}$ dans $E_{\mathscr{G}}$ associé au morphisme de préfaisceaux $\varphi$. Pour tout $a\in B$, $E(\varphi )$ définit par restrictions aux fibres en $a$ une application de la tige $\mathscr{F}_a$ de $\mathscr{F}$ dans la tige $\mathscr{G}_a$ de $\mathscr{G}$; on la note $\varphi_a$. C’est aussi la limite inductive des applications $\varphi_U$ (E, III, p. 63), où U parcourt l’ensemble $\mathscr{B}(a)$ des ouverts appartenant à la base $\mathscr{B}$ et qui contiennent $a$.

On a E(Id$_{\mathscr{F}}) =$ Id$_{E_{\mathscr{F}}}$.

Soit $\mathscr{H}$ un préfaisceau sur B relatif à $\mathscr{B}$ et soit $\psi = (\psi_U)$ un morphisme de préfaisceaux de $\mathscr{G}$ dans $\mathscr{H}$. Pour $[U, s, x]\in E_{\mathscr{F}}$, on a

$$
E(\psi \circ \varphi )([U, s, x]) = [U, \psi_U\circ \varphi_U(s), x]
$$

$$
= E(\psi )([U, \varphi_U(s), x])
$$

$$
= E(\psi )\circ E(\varphi )([U, s, x])
$$

Par suite, on a $E(\psi \circ \varphi ) = E(\psi )\circ E(\varphi )$. En particulier, si $a$ est un point de B, $(\psi \circ \varphi )_a=\psi_a\circ \varphi_a$.

Si $\varphi$ est un isomorphisme, Il en est de même de $E(\varphi )$.

#### Remarque {#ta-i-s3-n5-rem-1 .statement tag=01O2}

Soit $\mathscr{F}$ un faisceau sur B relatif à la base $\mathscr{B}$. Soit $B'$ une partie ouverte de B, soit $\mathscr{B}'$ une base de la topologie de $B'$ telle que $\mathscr{B}'\subset \mathscr{B}$. Soit $\mathscr{F}|\mathscr{B}'$ le préfaisceau sur $B'$ relatif à la base $\mathscr{B}'$ déduit de $\mathscr{F}$ par restriction.

1) L’ensemble $X_{\mathscr{F}|\mathscr{B}'}$ est alors un sous-ensemble de $X_{\mathscr{F}}$ et la relation d’équivalence $R_{\mathscr{F}}$ induit dans $X_{\mathscr{F}|\mathscr{B}'}$ la relation d’équivalence $R_{\mathscr{F}|\mathscr{B}'}$. On en déduit une injection canonique $i$ de $E_{\mathscr{F}|\mathscr{B}'}$ dans $E_{\mathscr{F}}$. Son image est $\overset{-1}{p}(B')$ car pour tout élément $[U, s, x]$ de $\overset{-1}{p}(B')$, il existe un élément V de $\mathscr{B}'$ tel que $x\in V$ et $V\subset U$, et l’on a $[U, s, x] =i([V, r_{VU}(s), x])$. L’application $i$ est continue car la topologie de $X_{\mathscr{F}|\mathscr{B}'}$ est la plus fine rendant continues les applications définies par $x\mapsto [U, s, x]$, pour $U\in \mathscr{B}'$ et $s\in \mathscr{F}(U)$. D’après le corollaire 2 de I, p. 30 de la proposition 6, l’injection canonique $i$ de $E_{\mathscr{F}|\mathscr{B}'}$ dans $E_{\mathscr{F}}$ induit un $B'$-isomorphisme de $E_{\mathscr{F}|\mathscr{B}'}$ sur $\overset{-1}{p}(B')$.

En particulier, lorsque $B'$ est égal à B$,i: E_{\mathscr{F}|\mathscr{B}'}\rightarrow E_{\mathscr{F}}$ est un B-isomorphisme d’espaces étalés.

2) Soit $\mathscr{G}$ un préfaisceau sur B relatif à la base $\mathscr{B}$ et soit $\varphi :\mathscr{F}\rightarrow \mathscr{G}$ un morphisme de préfaisceaux. La famille $\varphi '= (\varphi_U)_{U\in\mathscr{B}'}$ est un morphisme de préfaisceaux de $\mathscr{F}|\mathscr{B}'$ dans $\mathscr{G}|\mathscr{B}'$. Le diagramme

$$
E\mathscr{F}|\mathscr{B}'E(\varphi ')E\mathscr{G}|\mathscr{B}'
$$

$ii'$

$E_{\mathscr{F}}^{E(\varphi)}E_{\mathscr{G}}$ , où $i$ et $i'$ sont les injections canoniques, est commutatif.

#### Exemple 1 {#ta-i-s3-n5-exa-1 .statement tag=01O3}

Soient B un espace topologique, $\mathscr{B}$ une base de la topologie de B et F un ensemble. Prenons pour $\mathscr{F}$ le préfaisceau sur B relatif à $\mathscr{B}$ défini par $\mathscr{F}(U) = F$ pour tout $U\in \mathscr{B}$ et $r_{UV}$ = Id$_F$ pour tout couple $(U,V)$ d’éléments de $\mathscr{B}$ tel que $U\subset V$. L’application $[U, s, x]\mapsto (x, s(x))$ est un B-isomorphisme du B-espace $E_{\mathscr{F}}$ sur le B-espace $B\times F$ où F est muni de la topologie discrète. On notera que lorsque $\mathscr{B}$ est l’ensemble des parties ouvertes de B, le préfaisceau $\mathscr{F}$ sur B n’est un faisceau que si l’ensemble F est réduit à un point (cf. I, p. 43, remarque).

#### Exemple 2 {#ta-i-s3-n5-exa-2 .statement tag=01O4}

Soient B un espace topologique et $(E, p)$ un B-espace. Prenons pour $\mathscr{F}$ le faisceau sur B des sections continues de $(E, p)$. L’application $(U, s, x)\mapsto s(x)$ de $X_{\mathscr{F}}$ dans E est compatible avec la relation d’équivalence $R_{\mathscr{F}}$. L’application $e: E_{\mathscr{F}}\rightarrow E$ que l’on en déduit par passage au quotient est un B-morphisme ; le B-morphisme $e$ est dit canonique. L’image de $e$ est la réunion des images des sections continues de $p$ au-dessus des ouverts de B. L’application $e$ est donc surjective si $p$ est étale (I, p. 33, prop. 9). D’autre part, l’application $e$ est injective si et seulement si pour tout ouvert U de B et tout couple $(s, s')$ de sections continues de $p$ sur U, l’ensemble des points $x\in U$ tels que $s(x) =s'(x)$ est ouvert ; c’est en particulier le cas si $p$ est étale (I, p. 34, prop. 11, b)). Par conséquent, si $(E, p)$ est un B-espace étalé, l’application $e$ est un B-isomorphisme.

#### Exemple 3 {#ta-i-s3-n5-exa-3 .statement tag=01O5}

Soient B un espace topologique, $\mathscr{B}$ une base de la topologie de B$,\mathscr{F}$ un préfaisceau sur B relatif à $\mathscr{B}$ et $\mathscr{L}$ un sous-préfaisceau de $\mathscr{F}$. Alors, l’ensemble $X_{\mathscr{L}}$ est contenu dans l’ensemble $X_{\mathscr{F}}$ et la relation d’équivalence $R_{\mathscr{F}}$ induit dans $X_{\mathscr{L}}$ la relation d’équivalence $R_{\mathscr{L}}$. Le B-morphisme $E(i): E_{\mathscr{L}}\rightarrow E_{\mathscr{F}}$ associé au morphisme canonique $i:\mathscr{L}\rightarrow \mathscr{F}($I, p. 48, exemple 2) est donc injectif. Comme $E_{\mathscr{L}}$ et $E_{\mathscr{F}}$ sont des B-espaces étalés, l’application $E(i)$ est ouverte et même étale (I, p. 30, cor. 1), donc induit un homéomorphisme de $E_{\mathscr{L}}$ sur une partie ouverte de $E_{\mathscr{F}}$.

### 6. Faisceau associé à un préfaisceau

Conservons les notations du n$^o5$. On appelle faisceau associé au préfaisceau $\mathscr{F}$, et on note $\widetilde{\mathscr{F}}$ le faisceau $\mathscr{S}(B; E_{\mathscr{F}})$ des sections continues du B-espace étalé $E_{\mathscr{F}}$ associé au préfaisceau $\mathscr{F}$. Pour tout ensemble ouvert $U\in \mathscr{B}$, notons $\sigma_{\mathscr{F}}(U):\mathscr{F}(U)\rightarrow \widetilde{\mathscr{F}}(U)$ l’application qui, à $s\in \mathscr{F}(U)$, associe la section continue $\sigma_{\mathscr{F}}(U, s):x\mapsto [U, s, x]$ de $E_{\mathscr{F}}$ au-dessus de U. Par définition de la relation d’équivalence $R_{\mathscr{F}}$, la famille $\sigma_{\mathscr{F}}= (\sigma_{\mathscr{F}}(U))_{U\in\mathscr{B}}$ est un morphisme de préfaisceaux de $\mathscr{F}$ dans le préfaisceau $\widetilde{\mathscr{F}}|\mathscr{B}$. Le morphisme $\sigma_{\mathscr{F}}$ est appelé morphisme canonique de $\mathscr{F}$ dans $\widetilde{\mathscr{F}}|\mathscr{B}$.

Notons $j_{\mathscr{F}}: E_{\mathscr{F}}\rightarrow E_{\mathscr{F}}$ le B-morphisme composé du B-isomorphisme canonique $E_{\mathscr{F}|\mathscr{B}}\rightarrow E_{\mathscr{F}}\widetilde{(}I$, p. 51) et du B-morphisme $E(\sigma_{\mathscr{F}}): E_{\mathscr{F}}\rightarrow$ $E_{\widetilde{\mathscr{F}}|\mathscr{B}}$. Noton$\widetilde{s}$ d’autre part $e_{\mathscr{F}}:E_{\widetilde{\mathscr{F}}}\rightarrow E_{\mathscr{F}}$ le B-isomorphisme canonique (I, p. 52, exemple 2).

#### Proposition 2 {#ta-i-s3-prop-2 .statement tag=01O6}

L’application $j_{\mathscr{F}}$ est le B-isomorphisme réciproque de $e_{\mathscr{F}}$.

Pour $U\in \mathscr{B},s\in \mathscr{F}(U)$ et $x\in U$, on a par définition de $j_{\mathscr{F}}:$

$$
j_{\mathscr{F}}([U, s, x]) = [U, \sigma_{\mathscr{F}}(U, s), x]
$$

d’où $e_{\mathscr{F}}(j_{\mathscr{F}}([U, s, x])) =\sigma_{\mathscr{F}}(U, s)(x) = [U, s, x]$. Cela prouve la proposition.

#### Corollaire {#ta-i-s3-n6-cor-1 .statement tag=01O7}

Pour tout $a\in B$, l’application $(\sigma_{\mathscr{F}})_a:\mathscr{F}_a\rightarrow \widetilde{\mathscr{F}}_a$ est bijective.

Puisque $j_{\mathscr{F}}$ est un B-isomorphisme, il en est de même de $E(\sigma_{\mathscr{F}})$, et $(\sigma_{\mathscr{F}})_a$ s’en déduit par passage aux fibres en $a$.

Soient $\mathscr{G}$ un préfaisceau sur B relatif à $\mathscr{B}$ et $\varphi :\mathscr{F}\rightarrow \mathscr{G}$ un morphisme de préfaisceaux. On note $\widetilde{\varphi}:\widetilde{\mathscr{F}}\rightarrow \widetilde{\mathscr{G}}$ le morphisme de faisceaux $\mathscr{S}_{E(\varphi)}($I, p. 48, exemple 1), où $E(\varphi ): E_{\mathscr{F}}\rightarrow E_{\mathscr{G}}$ est le B-morphisme associé à $\varphi$. Pour tout ouvert $U\in \mathscr{B}$ et tout $s\in \mathscr{F}(U)$, on a, par définition,

$$
\widetilde{\varphi}_U(\sigma_{\mathscr{F}}(U, s)) = E(\varphi )\circ \sigma_{\mathscr{F}}(U, s) =\sigma_{\mathscr{G}}(U, \varphi_U(s))
$$

On a donc :

(1) $\widetilde{\varphi}_U\circ \sigma_{\mathscr{F}}(U) =\sigma_{\mathscr{G}}(U)\circ \varphi_U$, pour tout $U\in \mathscr{B}$. Autrement dit :

$$
\widetilde{\varphi}|\mathscr{B}\circ \sigma_{\mathscr{F}}=\sigma_{\mathscr{G}}\circ \varphi \tag{2}
$$

#### Proposition 3 {#ta-i-s3-prop-3 .statement tag=01O8}

Soit B un espace topologique, soit $\mathscr{B}$ une base de la topologie de B, soit $\mathscr{F}= (\mathscr{F}(U), f_{UV})$ un préfaisceau sur B relatif à $\mathscr{B}$, soit $\widetilde{\mathscr{F}}$ le faisceau associé et soit $\sigma_{\mathscr{F}}:\mathscr{F}\rightarrow \widetilde{\mathscr{F}}|\mathscr{B}$ le morphisme canonique. Étant donnés un faisceau $\mathscr{G}= (\mathscr{G}(U), g_{UV})$ sur B et un morphisme de préfaisceaux $\varphi :\mathscr{F}\rightarrow \mathscr{G}|\mathscr{B}$, il existe un unique morphisme de faisceaux $\psi :\widetilde{\mathscr{F}}\rightarrow \mathscr{G}$ tel que $\psi |\mathscr{B}\circ \sigma_{\mathscr{F}}=\varphi$.

#### Lemme {#ta-i-s3-n6-lem-1 .statement tag=01O9}

Soient U une partie ouverte de B et $s: U\rightarrow E_{\mathscr{F}}$ une section continue de $E_{\mathscr{F}}$ au-dessus de U. Pour tout point $a$ de U, il existe un ouvert $V\in \mathscr{B}$ tel que $a\in V$ et $V\subset U$ et un élément $v$ de $\mathscr{F}(V)$ tel que $s|V =\sigma_{\mathscr{F}}(V, v)$.

Soit $a\in U$. Par définition de l’espace $E_{\mathscr{F}}$, il existe un ouvert $V'\in \mathscr{B}$ tel que $a\in V'$ et un élément $t$ de $\mathscr{F}(V')$ tel que $s(a) = [V', t, a]$. Alors $s$ et $\sigma_{\mathscr{F}}(V', t)$ induisent par restriction deux sections continues de $E_{\mathscr{F}}$ au-dessus de $V'\cap U$ qui sont égales au point $a$. D’après la prop. 11, b) de I, p. 34, il existe un voisinage ouvert V de $a$, contenu dans $V'\cap U$, appartenant à $\mathscr{B}$, tel que $s$ et $\sigma_{\mathscr{F}}(V', t)$ soient égales en tout point de V. Si l’on pose $v=f_{VV'}(t)$, on a bien $s|V =\sigma_{\mathscr{F}}(V, v)$.

Démontrons la proposition. Pour tout ouvert U de B et toute section $s\in \widetilde{\mathscr{F}}(U)$, notons $D(U, s)$ l’ensemble des couples $(V, v)$ tels que $V\in \mathscr{B},V\subset U,v\in \mathscr{F}(U)$ et $s|V =\sigma_{\mathscr{F}}(V, v)$. Il résulte du lemme que ces ouverts V forment un recouvrement de U.

S’il existe un morphisme $\psi :\widetilde{\mathscr{F}}\rightarrow \mathscr{G}$ tel que $\psi |\mathscr{B}\circ \sigma_{\mathscr{F}}=\varphi$, alors, pour tout ouvert U de B, toute section $s\in \widetilde{\mathscr{F}}(U)$ et tout couple $(V, v)\in D(U, s)$, on a $g_{VU}(\psi_U(s)) =\psi_V(s|V) =\varphi_V(v)$. Cela prouve l’unicité de $\psi$ en vertu de la propriété $(F_1)$ des faisceaux.

Soient U un ouvert de B et $s$ un élément de $\widetilde{\mathscr{F}}(U)$. Soient $(V, v)$ et $(V', v')$ des éléments de $D(U, s)$. On a $s(a) = [V, v, a] = [V', v', a]$ pour tout point $a\in V\cap V'$. Il existe donc un couple $(W, w)\in D(V\cap V', s)$ tel que $a\in W$ et $f_{WV}(v) =f_{WV}(v') =w$. On a alors

$$
g_{W(V\cap V')}\circ g_{(V\cap V')V}(\varphi_V(v)) =g_{WV}(\varphi_V(v)) =\varphi_W(f_{WV}(v)) =\varphi_W(w)
$$

et de même,

$$
g_{W(V\cap V')}\circ g_{(V\cap V')V'}(\varphi_{V'}(v')) =\varphi_W(w)
$$

d’où

$$
g_{W(V\cap V')}\circ g_{(V\cap V')V}(\varphi_V(v)) =g_{W(V\cap V')}\circ g_{(V\cap V')V'}(\varphi_{V'}(v'))
$$

D’après la propriété $(F_1)$ des faisceaux, on a donc

$$
g_{(V\cap V')V}(\varphi_V(v)) =g_{(V\cap V')V'}(\varphi_{V'}(v'))
$$

D’après les propriétés $(F_1)$ et $(F_2)$ des faisceaux, il existe un unique élément $\psi_U(s)\in \mathscr{G}(U)$ tel que l’on ait :

(3) $g_{VU}(\psi_U(s)) =\varphi_V(v)$ pour tout $(V, v)\in D(u, s)$.

Soit $\psi_U:\widetilde{\mathscr{F}}(U)\rightarrow \mathscr{G}(U)$ l’application ainsi définie. Il résulte immédiatement de (3) que la famille $\psi = (\psi_U)$ est un morphisme de faisceaux et que l’on a $\varphi_V=\psi_V\circ \sigma_{\mathscr{F}}(V)$ pour tout $V\in \mathscr{B}$.

#### Corollaire 1 {#ta-i-s3-prop-3-cor-1 .statement tag=01OA}

Soient B un espace topologique, $\mathscr{F}$ un préfaisceau sur B$,\widetilde{\mathscr{F}}$ le faisceau associé et $\sigma_{\mathscr{F}}:\mathscr{F}\rightarrow \widetilde{\mathscr{F}}$ le morphisme canonique. Pour que $\mathscr{F}$ soit un faisceau, il faut et il suffit que $\sigma_{\mathscr{F}}$ soit un isomorphisme.

Si $\sigma_{\mathscr{F}}$ est un isomorphisme, $\mathscr{F}$ est un faisceau. Inversement, si $\mathscr{F}$ est un faisceau, il existe par la proposition 3 un morphisme $\varphi :\widetilde{\mathscr{F}}\rightarrow \mathscr{F}$ tel que $\varphi \circ \sigma_{\mathscr{F}}=$ Id$_{\mathscr{F}}$. Puisque Id$_{\mathscr{F}}$ est l’unique morphisme $\psi :\widetilde{\mathscr{F}}\rightarrow \widetilde{\mathscr{F}}$ tel que $\psi \circ \sigma_{\mathscr{F}}=\sigma_{\mathscr{F}}$, on a alors $\widetilde{\sigma}_{\mathscr{F}}\circ \varphi =$ Id$_{\widetilde{\mathscr{F}}}$.

#### Remarque {#ta-i-s3-n6-rem-1 .statement tag=01OB}

Soient B un espace topologique, $\mathscr{F}$ un préfaisceau sur B, $\mathscr{G}$ un faisceau sur B et $\varphi :\mathscr{F}\rightarrow \mathscr{G}$ un morphisme de préfaisceaux. Le morphisme canonique $\sigma_{\mathscr{G}}:\mathscr{G}\rightarrow \widetilde{\mathscr{G}}$ est un isomorphisme d’après le corollaire 1. D’après la relation (2) de I, p. 54, l’unique morphisme $\psi :\widetilde{\mathscr{F}}\rightarrow \mathscr{G}$ tel que $\psi \circ \sigma_{\mathscr{F}}=\varphi$ est donc $\sigma^{-1}_{\mathscr{G}}\circ \widetilde{\varphi}$.

#### Corollaire 2 {#ta-i-s3-prop-3-cor-2 .statement tag=01OC}

Soient B un espace topologique, $\mathscr{F}$ et $\mathscr{G}$ des faisceaux sur B et $\varphi$ un morphisme de faisceaux de $\mathscr{F}$ dans $\mathscr{G}$. Les assertions suivantes sont équivalentes :

(i) $\varphi$ est un isomorphisme ;

(ii) Il existe une base $\mathscr{B}$ de la topologie de B telle que pour tout $U\in \mathscr{B}$, l’application $\varphi_U$ soit bijective ;

(iii) Pour tout point $a$ de B, l’application $\varphi_a$ est une bijection de la tige $\mathscr{F}_a$ sur la tige $\mathscr{G}_a$.

L’implication (i)$\Rightarrow$(ii) est immédiate.

(ii)$\Rightarrow$(iii) : considérons le diagramme commutatif (I, p. 51)

$$
E\mathscr{F}|\mathscr{B}E(\varphi |\mathscr{B})E\mathscr{G}|\mathscr{B}
$$

$$
E_{\mathscr{F}}^{E(\varphi)}E_{\mathscr{G}}
$$

où les flèches verticales sont les B-isomorphismes canoniques. Si la condition (ii) est satisfaite, $E(\varphi |\mathscr{B})$ est un B-isomorphisme, donc $E(\varphi )$ en est un également. Les applications $\varphi_a$ se déduisent de $E(\varphi )$ par passage aux fibres et sont alors bijectives.

(iii)$\Rightarrow$(i) : sous l’hypothèse (iii), l’application $E(\varphi ): E_{\mathscr{F}}\rightarrow E_{\mathscr{G}}$ est un B-morphisme bijectif d’espaces étalés donc est un B-isomorphisme (I, p. 30, cor. 2 de la prop. 6). Par suite, le morphisme $\widetilde{\varphi}:\widetilde{\mathscr{F}}\rightarrow \widetilde{\mathscr{G}}$ est un isomorphisme. Comme $\mathscr{F}$ et $\mathscr{G}$ sont des faisceaux, les morphismes canoniques $\sigma_{\mathscr{F}}:\mathscr{F}\rightarrow \widetilde{\mathscr{F}}$ et $\sigma_{\mathscr{G}}:\mathscr{G}\rightarrow \widetilde{\mathscr{G}}$ sont des isomorphismes (corollaire 1) et l’on a $\widetilde{\varphi}\circ \sigma_{\mathscr{F}}=\sigma_{\mathscr{G}}\circ \varphi ($I, p. 54, relation (2)) donc $\varphi$ est un isomorphisme.

#### Scholie {#ta-i-s3-n6-sch-1 .statement tag=01OD}

Soit B un espace topologique. À tout faisceau $\mathscr{F}$ sur B, on associe un B-espace étalé $E_{\mathscr{F}}$ (I, p. 50, déf. 4). À tout B-espace étalé T, on associe le faisceau $\mathscr{S}(T)$ sur B de ses sections continues (I, p. 45, exemple 3). On a défini un isomorphisme canonique de faisceaux $\sigma_{\mathscr{F}}:\mathscr{F}\rightarrow \mathscr{S}(E_{\mathscr{F}})$ (I, p. 55, cor. 1) et un isomorphisme canonique de B-espaces étalés $e_T: E_{\mathscr{S}(T)}\rightarrow T$ (I, p. 52, exemple 2).

Pour tout couple $(\mathscr{F},\mathscr{G})$ de faisceaux sur B, on a défini (I, p. 50) une application $\varphi \mapsto E(\varphi )$ de l’ensemble des morphismes de faisceaux de $\mathscr{F}$ dans $\mathscr{G}$ dans l’ensemble des B-morphismes de $E_{\mathscr{F}}$ dans $E_{\mathscr{G}}$. On a les relations

E(Id$_{\mathscr{F}}) =$ Id$_{E_{\mathscr{F}}},E(\psi \circ \varphi ) = E(\psi )\circ E(\varphi )$.

Pour tout couple $(T,U)$ de B-espaces étalés, on a défini (I, p. 48, exemple 1) une application $f\mapsto \mathscr{S}(f)$ de l’ensemble des B-morphismes de T dans U dans l’ensemble des morphismes de faisceaux de $\mathscr{S}(T)$ dans $\mathscr{S}(U)$. On a les relations

$\mathscr{S}$ (Id$_T) =$ Id$_{\mathscr{S}(T)},\mathscr{S}(g\circ f) =\mathscr{S}(g)\circ \mathscr{S}(f)$.

Avec les notations précédentes, les diagrammes suivants sont commutatifs :

$$
\mathscr{F}^{\varphi}\mathscr{G}E_{\mathscr{S}(T)}^{E(\mathscr{S}(f))}E_{\mathscr{S}(U)}
$$

(4) $\sigma_{_{\mathscr{F}}}\sigma_{_{\mathscr{G}}}$ (5) $e_{_T}e_{_U}$

$\mathscr{S}(E_{\mathscr{F}})^{\mathscr{S}(E(\varphi))}\mathscr{S}(E_{\mathscr{G}})$, T $^fU$.

Cela résulte de I, p. 54, formule (2) pour le premier et c’est une conséquence immédiate des définitions pour le second. Cela implique que pour tout couple $(\mathscr{F},\mathscr{G})$ de faisceaux sur B et tout couple $(T,U)$ de B-espaces étalés, les applications $\varphi \mapsto E(\varphi )$ et $f\mapsto \mathscr{S}(f)$ considérées ci-dessus sont bijectives.

Ces résultats permettent de déduire un énoncé relatif aux B-espaces étalés d’un énoncé relatif aux faisceaux sur B, et réciproquement.

### 7. Image directe et image réciproque d’un faisceau

Soient A et B des espaces topologiques et $u: A\rightarrow B$ une application continue.

Soit $\mathscr{F}= (\mathscr{F}(U), f_{UV})$ un préfaisceau sur A. On définit un préfaisceau $\mathscr{F}'$ sur B de la façon suivante : pour tout ouvert U de B, posons $\mathscr{F}'(U) =\mathscr{F}(\overset{-1}{u}(U))$ et pour tout couple $(U,V)$ d’ouverts de B tel que U $\subset V$, posons $f'_{UV}=f_{\overset{-1}{u}(U)\overset{-1}{u}(V)}$. Alors $(\mathscr{F}'(U), f'_{UV})$ est un préfaisceau sur B. On le note $u_*(\mathscr{F})$ et on l’appelle le préfaisceau image directe du préfaisceau $\mathscr{F}$ par l’application $u$.

Si $(U_i)_{i\in I}$ est une famille d’ouverts de B, on a $\overset{-1}{u}(\bigcup_{i\in I}U_i) =$ $\bigcup_{i\in I}\overset{-1}{u}(U_i)$ et $\overset{-1}{u}(\bigcap_{i\in I}U_i) =\bigcap_{i\in I}\overset{-1}{u}(U_i)$ (E, II, p. 25, prop. 3 et 4). Il en résulte aussitôt que, si $\mathscr{F}$ jouit de la propriété $(F_1)$ (resp. $(F_2)$) des faisceaux (I, p. 43), il en est de même de $u_*(\mathscr{F})$. Par suite, l’image directe d’un faisceau est un faisceau.

Soient $\mathscr{F}_1$ et $\mathscr{F}_2$ des préfaisceaux sur A et soit $\varphi :\mathscr{F}_1\rightarrow \mathscr{F}_2$ un morphisme de préfaisceaux. Il existe alors un unique morphisme de préfaisceaux $u_*\varphi :u_*\mathscr{F}_1\rightarrow u_*\mathscr{F}_2$ tel que pour tout ouvert U de B, l’application $(u_*\varphi )(U): (u_*\mathscr{F}_1)(U)\rightarrow (u_*\mathscr{F}_2)(U)$ soit l’application $\varphi (\overset{-1}{u}(U)):\mathscr{F}_1(\overset{-1}{u}(U))\rightarrow \mathscr{F}_2(\overset{-1}{u}(U))$. Si $\mathscr{F}_3$ est un préfaisceau sur A et si $\psi :\mathscr{F}_2\rightarrow \mathscr{F}_3$ est un morphisme de préfaisceaux, on a $u_*(\psi \circ \varphi ) =u_*(\psi )\circ u_*(\varphi )$.

Soit C un espace topologique et soit $v: B\rightarrow$ C une application continue. Si $\mathscr{F}$ est un préfaisceau sur A, les préfaisceaux $v_*(u_*(\mathscr{F}))$ et $(v\circ u)_*(\mathscr{F})$ coïncident. Si $\varphi :\mathscr{F}_1\rightarrow \mathscr{F}_2$ est un morphisme de préfaisceaux sur A, on a l’égalité $v_*(u_*(\varphi )) = (v\circ u)_*(\varphi )$.

#### Exemple 1 {#ta-i-s3-n7-exa-1 .statement tag=01OE}

Soient B un espace topologique, A un sous-espace de B et $\mathscr{F}= (\mathscr{F}(U), f_{UV})$ un préfaisceau sur A. Notons $i: A\rightarrow B$ l’injection canonique. On a alors $i_*(\mathscr{F}) = (\mathscr{F}'(U), f'_{UV})$ où pour tout ouvert U de B$,\mathscr{F}'(U) =\mathscr{F}(U\cap A)$, et pour tout couple $(U,V)$ d’ouverts de B avec $U\subset V,f'_{UV}=f_{(U\cap A)(V\cap A)}$.

Soit maintenant $\mathscr{G}$ un préfaisceau sur B. On appelle image réciproque du préfaisceau $\mathscr{G}$ par $u$, et l’on note $u^*(\mathscr{G})$ le faisceau $\mathscr{C}_B(A; E_{\mathscr{G}})$ sur A des B-morphismes à valeurs dans le B-espace $E_{\mathscr{G}}($I, p. 45, exemple 4). Il est canoniquement isomorphe au faisceau sur A des sections du A-espace étalé $A\times_BE_{\mathscr{G}}$ (I, p. 9, prop. 3). On en déduit (I, p. 52, exemple 2) un isomorphisme canonique $\varphi$ de l’espace étalé associé à $u^*(\mathscr{G})$ sur le A-espace $A\times_BE_{\mathscr{G}}$. Si de plus $\mathscr{G}$ est un faisceau, on a pour tout point $a$ de A une bijection canonique $\psi_a:u^*(\mathscr{G})_a\rightarrow \mathscr{G}_{u(a)}:$ pour tout voisinage ouvert U de $a$ dans A et tout B-morphisme $f: U\rightarrow E_{\mathscr{G}}$, on a

$$
\varphi ([U, f, a]) = (a, f(a)),\psi_a([U, f, a]) =f(a)
$$

Soient $\mathscr{G}_1$ et $\mathscr{G}_2$ des préfaisceaux sur B et $\varphi :\mathscr{G}_1\rightarrow \mathscr{G}_2$ un morphisme de préfaisceaux. On déduit par changement de base du morphisme de B-espaces étalés $E(\varphi ): E_{\mathscr{G}_1}\rightarrow E_{\mathscr{G}_2}$ un morphisme de A-espaces étalés $A\times_BE_{\mathscr{G}_1}\rightarrow A\times_BE_{\mathscr{G}_2}$, d’où un morphisme de faisceaux sur A$,u^*(\varphi ):u^*(\mathscr{G}_1)\rightarrow u^*(\mathscr{G}_2)$. Soient $\mathscr{G}_3$ un préfaisceau sur B et $\psi :\mathscr{G}_2\rightarrow \mathscr{G}_3$ un morphisme de préfaisceaux. On a alors l’égalité $u^*(\psi \circ \varphi ) =u^*(\psi )\circ u^*(\varphi )$.

Soit C un espace topologique et soit $v: B\rightarrow$ C une application continue. Si $\mathscr{G}$ est un préfaisceau sur C, les faisceaux $u^*(v^*(\mathscr{G}))$ et $(v\circ u)^*(\mathscr{G})$ s’identifient canoniquement (I, p. 5). Si $\varphi :\mathscr{G}_1\rightarrow \mathscr{G}_2$ est un morphisme de préfaisceaux sur C, on a de plus $u^*(v^*(\varphi )) = (v\circ u)^*(\varphi )$.

#### Remarque {#ta-i-s3-n7-rem-1 .statement tag=01OF}

Le morphisme canonique $\sigma_{\mathscr{G}}:\mathscr{G}\rightarrow \widetilde{\mathscr{G}}$ de I, p. 53 correspond en termes d’espaces étalés à l’isomorphisme $j_{\mathscr{G}}$ de la proposition 2 de I, p. 53. Il en résulte que $u^*(\sigma_{\mathscr{G}})$ est un isomorphisme. En particulier si A = B et $u=$ Id$_A$, le préfaisceau $u^*(\mathscr{F})$ est le faisceau $\widetilde{\mathscr{F}}$.

#### Exemple 2 {#ta-i-s3-n7-exa-2 .statement tag=01OG}

Soient B un espace topologique et A un sous-espace de B. Notons $i: A\rightarrow B$ l’injection canonique. Pour tout faisceau $\mathscr{G}$ sur B, on note $\mathscr{G}_A$ le faisceau $i^*(\mathscr{G})$ et on dit que $\mathscr{G}_A$ est le faisceau sur A induit par le faisceau $\mathscr{G}$. Le faisceau $\mathscr{G}_A$ s’identifie au faisceau $\mathscr{S}(A; (E_{\mathscr{G}})_A)$ des sections du A-espace étalé induit par $E_{\mathscr{G}}$ au-dessus de A.

Supposons que A soit un sous-espace ouvert de B et soit $\mathscr{G}$ un faisceau sur B. Par définition, le faisceau $\mathscr{G}_A$ est le faisceau $\widetilde{\mathscr{G}}|A$ déduit de $\widetilde{\mathscr{G}}$ par restriction à l’ouvert A (I, p. 43). Soit $\sigma_{\mathscr{G}}:\mathscr{G}\rightarrow \widetilde{\mathscr{G}}$ l’isomorphisme canonique (I, p. 55, cor. 1). Alors, $\sigma_{\mathscr{G}}|A$ est un isomorphisme, dit canonique, du faisceau $\mathscr{G}|A$ sur le faisceau $\mathscr{G}_A$ que l’on appelle l’isomorphisme canonique de $\mathscr{G}|A$ sur $\mathscr{G}_A$.

### 8. Les homomorphismes $\alpha \mathbf{e}\mathbf{t}\beta$ ; adjonction

Soient A et B des espaces topologiques et soit $u: A\rightarrow B$ une application continue. Soit $\mathscr{G}$ un préfaisceau sur B. Par définition de l’image directe de préfaisceaux, une section du faisceau $u_*u^*\mathscr{G}$ au-dessus d’un ouvert U de B est une section du faisceau $u^*\mathscr{G}$ au-dessus de l’ouvert $\overset{-1}{u}(U)$ de A, c’est-à-dire un B-morphisme $\overset{-1}{u}(U)\rightarrow E_{\mathscr{G}}$. On définit ainsi un morphisme de faisceaux $\widetilde{\mathscr{G}}\rightarrow u_*u^*\mathscr{G}$ en associant à la section $s$ de $E_{\mathscr{G}}$ au-dessus d’un ouvert U de B la section $s\circ u$ de $E_{\mathscr{G}}$ au-dessus de $\overset{-1}{u}(U)$. La composition de ce morphisme et du morphisme canonique $\sigma_{\mathscr{G}}:\mathscr{G}\rightarrow \widetilde{\mathscr{G}}$ (I, p. 53) est un morphisme de préfaisceaux $\mathscr{G}\rightarrow u_*u^*\mathscr{G}$ que l’on notera $\beta_{\mathscr{G}}^u$, voire $\beta_{\mathscr{G}}$ s’il n’y a pas d’ambiguïté sur l’application $u$.

#### Remarque 1 {#ta-i-s3-n8-rem-1 .statement tag=01OH}

Soient A, B, C des espaces topologiques, soient $u: A\rightarrow B,v: B\rightarrow C$ des applications continues ; posons $w=v\circ u$. Soit $\mathscr{G}$ un préfaisceau sur C.

Soient U un ouvert de C et $s$ une section de $E_{\mathscr{G}}$ au-dessus de U. Alors, $\beta_{\mathscr{G}}^v(s)$ est la section $s\circ v$ de $E_{\mathscr{G}}$ au-dessus de $\overset{-1}{v}(U)$, et $v_*(\beta_{v^*\mathscr{G}}^u)(\beta^v_{\mathscr{G}}(s))$ est la section $s\circ v\circ u=s\circ w$ de $E_{\mathscr{G}}$ au-dessus de $\overset{-1}{u}(\overset{-1}{v}(U)) =\overset{-1}{w}(U)$.

Il en résulte l’égalité $\beta_{\mathscr{G}}^w=v_*(\beta_{v^*\mathscr{G}}^u)\circ \beta_{\mathscr{G}}^v$.

#### Remarque 2 {#ta-i-s3-n8-rem-2 .statement tag=01OI}

Si $\gamma :\mathscr{G}_1\rightarrow \mathscr{G}_2$ est un morphisme de préfaisceaux sur B, les morphismes de préfaisceaux $\beta_{\mathscr{G}_2}\circ \gamma$ et $u_*u^*(\gamma )\circ \beta_{\mathscr{G}_1}$ sont égaux. En effet, si V est un ouvert de B et $s\in \mathscr{G}_1(V),\beta_{\mathscr{G}_1}(s)$ est la section $t$ de $A\times_BE_{\mathscr{G}_1}$ au-dessus de $\overset{-1}{u}(V)$, définie par $x\mapsto (x,[V, s, u(x)])$. L’image de $t$ par $u^*(\gamma )$ est ainsi la section de $A\times_BE_{\mathscr{G}_2}$ au-dessus de $\overset{-1}{u}(V)$ donnée par $x\mapsto (x,[V, \gamma (s), u(x)])$. Il en résulte bien que $u_*u^*(\gamma )\circ \beta_{\mathscr{G}_1}(s) =\beta_{\mathscr{G}_2}(\gamma (s))$.

#### Proposition 4 {#ta-i-s3-prop-4 .statement tag=01OJ}

Soient A et B des espaces topologiques, $u: A\rightarrow B$ une application continue, $\mathscr{G}$ un préfaisceau sur B$,\mathscr{F}$ un faisceau sur A.

Pour tout morphisme de préfaisceaux $\varphi :\mathscr{G}\rightarrow u_*\mathscr{F}$, il existe un unique morphisme de faisceaux $\psi :u^*(\mathscr{G})\rightarrow \mathscr{F}$ tel que $\varphi =u_*(\psi )\circ \beta_{\mathscr{G}}$.

Autrement dit, l’application canonique

Mor($u^*(\mathscr{G}),\mathscr{F}$)$\rightarrow$ Mor($\mathscr{G}, u_*(\mathscr{F})$)$,\psi \mapsto u_*(\psi )\circ \beta_{\mathscr{G}}$

est une bijection.

Avec les notations de la proposition 4, on notera parfois $\psi =\varphi^{\sharp}$ et $\varphi =\psi^{\flat}$.

Démontrons la proposition 4. D’après la remarque 2 appliquée au morphisme $\sigma_{\mathscr{G}}:\mathscr{G}\rightarrow \widetilde{\mathscr{G}}$, le morphisme $\beta_{\mathscr{G}}$ est égal à la composition

$$
u_*(u^*(\sigma_{\mathscr{G}})^{-1})\circ \beta_{\widetilde{\mathscr{G}}}\circ \sigma_{\mathscr{G}}
$$

où $u^*(\sigma_{\mathscr{G}}):u^*(\mathscr{G})\rightarrow u^*(\widetilde{\mathscr{G}})$ est l’isomorphisme canonique de la remarque de I, p. 58. Soit $\widetilde{\varphi}:\widetilde{\mathscr{G}}\rightarrow u_*\mathscr{F}$ l’unique morphisme de faisceaux tel que $\widetilde{\varphi}\circ \sigma_{\mathscr{G}}=\varphi ($I, p. 54, prop. 3). Il suffit alors de montrer qu’il existe un unique morphisme de faisceaux $\widetilde{\psi}:u^*(\mathscr{G})\rightarrow \mathscr{F}$ tel que $u_*(\widetilde{\psi})\circ \beta_{\mathscr{G}}=\widetilde{\varphi}$.

Nous p$\widetilde{o}$uvons donc supposer que $\mathscr{G}$ est un faisceau. Pour qu’un morphisme de faisceaux $\psi :u^*(\mathscr{G})\rightarrow \mathscr{F}$ satisfasse à la conclusion de la proposition 4, il faut et il suffit que pour tout ouvert V de B et toute section $t$ de $E_{\mathscr{G}}$ au-dessus de V, on ait

$$
\varphi_V(t) =\psi_{\overset{-1}{u}(V)}(t\circ u|\overset{-1}{u}(V)) \tag{6}
$$

Soit $U_0$ un ouvert de A et $s_0$ un élément de $u^*(\mathscr{G})(U_0)$, autrement dit un B-morphisme de $U_0$ dans $E_{\mathscr{G}}$. Soit $S(U_0, s_0)$ l’ensemble des triplets $(U,V, t)$ où U est un ouvert de A contenu dans $U_0$, V est un ouvert de B tel que $u(U)\subset V$ et $t$ une section de $E_{\mathscr{G}}$ au-dessus de V telle que l’on ait

$$
t\circ u|U =s_0|U \tag{7}
$$

Si $U_1$ et $U_2$ sont des ouverts de A avec $U_1\subset U_2$, notons $f_{U_1U_2}$ l’application de restriction $\mathscr{F}(U_2)\rightarrow \mathscr{F}(U_1)$. Pour tout $(U,V, t)\in S(U_0, s_0)$, on a alors la relation

$$
f_{UU_0}(\psi_{U_0}(s_0)) =\psi_U(s_0|U)
$$

$$
=\psi_U(t\circ u|U)
$$

$$
=f_{U\overset{-1}{u}(V)}(\psi_{\overset{-1}{u}(V)}(t\circ u|\overset{-1}{u}(V)))
$$

Par suite, si $\psi :u^*(\mathscr{G})\rightarrow \mathscr{F}$ satisfait à (6), on a

$$
f_{UU_0}(\psi_{U_0}(s_0)) =f_{U\overset{-1}{u}(V)}(\varphi_V(t)) \tag{8}
$$

Démontrons que, pour tout point $a$ de $U_0$, il existe un triplet $(U,V, t)\in S(U_0, s_0)$ tel que $a\in U$. Soit en effet $a$ un point de $U_0$. Il existe un voisinage ouvert V de B contenant $u(a)$ et une section $t$ de l’espace étalé $E_{\mathscr{G}}$ au-dessus de V telle que $t(u(a)) =s_0(a)$ (I, p. 33, prop. 9). Soit $U_1=\overset{-1}{u}(V)\cap U_0$. Les sections $s_0|U_1$ et $t\circ u|U_1$ du $U_1$-espace étalé $E_{\mathscr{G}}\times_BU_1$ coïncident au point $a$. D’après la proposition 11, b) de I, p. 34, l’ensemble des points où elles coïncident est un ouvert U de $U_1$ qui contient $a$. Le triplet $(U,V, t)$ appartient alors à $S(U_0, s_0)$.

La formule (8) et la propriété $(F_1)$ des faisceaux (I, p. 43) entraînent alors l’unicité de $\psi$.

Soient $(U,V, t)$ et $(U',V', t')$ des éléments de $S(U_0, s_0)$. D’après la relation (7), les restrictions à $u(U\cap U')$ de $t$ et $t'$ coïncident. D’après la prop. 11, b) de I, p. 34, il existe un ouvert W de B tel que $u(U\cap U')\subset$ $W\subset V\cap V'$ et que $t|W =t'|W$. On a donc

$$
f_{\overset{-1}{u}(W)\overset{-1}{u}(V)}(\varphi_V(t)) =\varphi_W(t|W) =\varphi_W(t'|W) =f_{\overset{-1}{u}(W)\overset{-1}{u}(V')}(\varphi_{V'}(t'))
$$

d’où

$$
f_{(U\cap U')\overset{-1}{u}(V)}(\varphi_V(t)) =f_{(U\cap U')\overset{-1}{u}(V')}(\varphi_{V'}(t')) \tag{9}
$$

D’après les propriétés $(F_1)$ et $(F_2)$ pour le faisceau $\mathscr{F}$, il existe un unique élément $s'$ de $\mathscr{F}(U_0)$ tel que pour tout triplet $(U,V, t)$ de $S(U_0, s_0)$, on ait :

$$
f_{UU_0}(s') =f_{U\overset{-1}{u}(V)}(\varphi_V(t)) \tag{10}
$$

Notons $\psi_{U_0}(s_0)$ cet élément.

Soit $U_1$ un ouvert contenu dans $U_0$ et soit $s_1=s_0|U_1$. Si $(U,V, t)\in$ $S(U_1, s_1)$, U est un ouvert contenu dans $U_0$ et $t\circ u|U =s_1|U =s_0|U$, donc $(U, v, t)\in S(U_0, s_0)$ et la relation (10) entraîne alors que

$$
f_{UU_1}(f_{U_1U_0}(\psi_{U_0}(s_0))) =f_{UU_0}(\psi_{U_0}(s_0)) =f_{U\overset{-1}{u}(V)}(\varphi_V(t))
$$

Par définition de $\psi_{U_1}(s_1)$, on a donc $\psi_{U_1}(s_1) =f_{U_1U_0}(\psi_{U_0}(s_0))$. Cela prouve que la famille $\psi = (\psi_U)$ est un morphisme de faisceaux de $u^*(\mathscr{G})$ dans $\mathscr{F}$.

Démontrons que $\psi$ satisfait à la relation (6). Soient ainsi V un ouvert de B et $t$ une section de $E_{\mathscr{G}}$ au-dessus de V. Si U = $\overset{-1}{u}(V)$ et si $s=t\circ u|U$, le triplet $(U,V, t)$ appartient à $S(U, s)$ et la relation (6) est conséquence immédiate de la relation (10), appliquée à $U = U_0$.

#### Proposition 5 {#ta-i-s3-prop-5 .statement tag=01OK}

Soient A et B des espaces topologiques et soit $u: A\rightarrow B$ une application continue.

a) Soient $\mathscr{G}_1$ et $\mathscr{G}_2$ des préfaisceaux sur B et soit $\gamma :\mathscr{G}_1\rightarrow \mathscr{G}_2$ un morphisme de préfaisceaux. Soient encore $\mathscr{F}$ un faisceau sur A et $\varphi :\mathscr{G}_2\rightarrow u_*\mathscr{F}$ un morphisme de préfaisceaux. On a l’égalité

$$
(\varphi \circ \gamma )^{\sharp}=\varphi^{\sharp}\circ u^*(\gamma ) \tag{11}
$$

b) Soient $\mathscr{F}_1,\mathscr{F}_2$ des faisceaux sur A et soit $\mathscr{G}$ un préfaisceau sur B. Soit $\varphi :\mathscr{F}_1\rightarrow \mathscr{F}_2$ un morphisme de faisceaux et soit $\gamma :\mathscr{G}\rightarrow$ $u_*\mathscr{F}_1$ un morphisme de préfaisceaux. On a la relation

$$
(u_*(\varphi )\circ \gamma )^{\sharp}=\varphi \circ \gamma^{\sharp}
$$

a) Par définition de $\varphi^{\sharp}$ et la remarque 2 de I, p. 60, on a

$$
\varphi \circ \gamma =u_*(\varphi^{\sharp})\circ \beta_{\mathscr{G}_2}\circ \gamma =u_*(\varphi^{\sharp})\circ u_*u^*(\gamma )\circ \beta_{\mathscr{G}_1}
$$

Par suite, $\varphi \circ \gamma =u_*(\varphi^{\sharp}\circ u^*(\gamma ))\circ \beta_{\mathscr{G}_1}$, d’où la relation (11).

b) Par définition de $\gamma^{\sharp}$, on a

$$
u_*(\varphi )\circ \gamma =u_*(\varphi )\circ u_*(\gamma^{\sharp})\circ \beta_{\mathscr{G}}=u_*(\varphi \circ \gamma^{\sharp})\circ \beta_{\mathscr{G}}
$$

d’où la relation annoncée, compte tenu de la définition de $(u_*(\varphi )\circ \gamma )^{\sharp}$.

Posons $\alpha_{\mathscr{F}}$ = Id$^{\sharp}_{u_*(\mathscr{F})}$; c’est l’unique morphisme de faisceaux $\rho :u^*(u_*(\mathscr{F}))\rightarrow \mathscr{F}$ tel que

Id$_{u_*(\mathscr{F})}=u_*(\rho )\circ \beta_{u_*(\mathscr{F})}$.

La relation (11) appliquée à $\mathscr{G}_2=u_*(\mathscr{F})$ et au morphisme $\varphi =$ Id$_{u_*(\mathscr{F})}$ fournit pour tout morphisme de préfaisceaux de $\gamma :\mathscr{G}\rightarrow u_*(\mathscr{F})$ la factorisation

$$
\gamma^{\sharp}=\alpha_{\mathscr{F}}\circ u^*(\gamma )
$$

Il résulte alors de la proposition 4 que pour tout morphisme de faisceaux $\psi$ de $u^*(\mathscr{G})$ dans $\mathscr{F},\psi^{\flat}$ est l’unique morphisme $\varphi :\mathscr{G}\rightarrow u_*(\mathscr{F})$ tel que $\psi =\alpha_{\mathscr{F}}\circ u^*(\varphi )$.

#### Exemple 1 {#ta-i-s3-n8-exa-1 .statement tag=01OL}

Considérons un espace topologique B, un sous-espace A de B, notons $i: A\rightarrow B$ l’injection canonique. Soient $(E, p)$

etp.vert45,(E$V', p$exemplede$')$ Bdeset toutB4-espaces. Prenons pour) et pourV-morphisme$\mathscr{F}$ le faisceau$f: E_V\mathscr{M}\mathscr{G}\rightarrow$orle faisceau${E'}^A_V(E$, posons$^A{; E'}^A\mathscr{M})$. Pour tout ou-$\varphi$or$_V(^Bf(E; E) =f'_V)_{\cap}(_AI$,, où $f_{V\cap A}$ est le $(V\cap A)$-morphisme de $E_{V\cap A}$ dans $E'_{V\cap A}$ induit par $f$. La famille $\varphi = (\varphi_V)$ ainsi définie est un morphisme de faisceaux de $\mathscr{G}$

dansfaisceaux(12) $i^*\mathscr{F}$. D’après la proposition$\psi :\mathscr{M}$or$_B\psi (E; E'_{V\cap A}()\sigma_{A\mathscr{G}}\rightarrow (V\mathscr{M}, f)$or$4|,_AV$il existe un unique morphisme de$(E\cap_AA) =; E'_A)f$tel que l’on ait$_{V\cap A}$

pour tout ouvert V de B et tout $f\in \mathscr{C}_V(E_V; E'_V)$. Le morphisme $\psi$ est appelé morphisme canonique de $\mathscr{M}$or$_B(E; E')_A$ dans $\mathscr{M}$or$_A(E_A; E'_A)$.

Si A est réduit à un point $a$, ce morphisme s’identifie au morphisme de la tige en $a$ du faisceau $\mathscr{M}$or$_B(E; E')$ sur l’ensemble $\mathscr{C}(E_a; E'_a)$.

Par passage aux sous-faisceaux, le morphisme $\psi$ induit un morphisme canonique de $\mathscr{I}$som$_B(E; E')_A$ dans $\mathscr{I}$som$_A(E_A; E'_A)$.

#### Exemple 2 {#ta-i-s3-n8-exa-2 .statement tag=01OM}

Soient A, B, C des espaces topologiques et soient $u: A\rightarrow B$, $v: B\rightarrow C$ des applications continues ; posons $w=v\circ u$. Soient E et $E'$ des C-espaces. Le morphisme canonique de $\mathscr{M}$or$_C(E; E')_A$

dans$\mathscr{M}$de$\mathscr{M}$oror$\mathscr{M}^C_B$or(E; E$(E\mathscr{M}^C_B$or$(E; E,\overset{A}{E'}){(E'_B}^A)')_A^A\rightarrow^B; E$dansdans${\mathscr{M}'}^A)$or$\mathscr{M}$est le morphisme composé du morphisme$\mathscr{M}^B$or(Eor$_A^{BB}(E$; E${(E'_A}^{BB},)$; E${E^A''_A}^B$déduit du morphisme canonique)). et du morphisme canonique de

### 9. Faisceaux mous

#### Définition 5 {#ta-i-s3-def-5 .statement tag=01ON}

Soit $p: E\rightarrow B$ une application étale. On dit que l’application $p$ est molle, ou que le B-espace étalé $(E, p)$ est mou si toute section continue de $p$ au-dessus d’un sous-espace fermé de B se prolonge en une section continue de $p$ au-dessus de B.

Soit $\mathscr{F}$ un faisceau sur B. On dit que $\mathscr{F}$ est un faisceau mou si l’espace étalé associé (I, p. 50, déf. 4) est mou.

Soit $\mathscr{F}$ un faisceau sur B. Le faisceau $\mathscr{F}$ est mou si et seulement si pour tout fermé Z de B, tout voisinage ouvert U de Z et tout $s\in \mathscr{F}(U)$, il existe $t\in \mathscr{F}(B)$ et un voisinage ouvert V de Z contenu dans U tel que $s|V =t|V$.

Si $\mathscr{F}$ est un faisceau mou, $\mathscr{F}(B)$ est non vide : en effet, l’unique section de l’espace étalé $E_{\mathscr{F}}$ associé à $\mathscr{F}$ au-dessus de $\emptyset$ se prolonge en une section continue de $E_{\mathscr{F}}$ au-dessus de B.

Soit $p: E\rightarrow B$ une application étale et soit A un sous-espace fermé de B. Si $p$ est molle, l’application $p_A:\overset{-1}{p}(A)\rightarrow A$ est molle. De façon équivalente, si $\mathscr{F}$ est un faisceau mou sur B, le faisceau induit sur un sous-espace fermé A est mou.

#### Proposition 6 {#ta-i-s3-prop-6 .statement tag=01OO}

Soient B un espace topologique, $\mathscr{F}$ un faisceau sur B et $(A_i)_{i\in I}$ un recouvrement fermé localement fini de B. Pour que le faisceau $\mathscr{F}$ soit mou, il faut et il suffit que, pour tout $i\in I$, le faisceau induit $\mathscr{F}_{A_i}$ soit mou.

La condition est évidemment nécessaire. Démontrons qu’elle est suffisante. Notons $p: E\rightarrow B$ le B-espace étalé $E_{\mathscr{F}}$ associé au faisceau $\mathscr{F}$. Soient A un sous-espace fermé de B et $s: A\rightarrow E$ une section continue de $p$ au-dessus de A ; il s’agit de démontrer que $s$ possède un prolongement continu à B. Pour tout sous-ensemble J de I, posons $A_J=\bigcup_{i\in J}A_i$; l’ensemble $A_J$ est fermé dans B (TG, I, p. 6, prop. 4).

Soit $\mathscr{S}$ l’ensemble des couples $(J, t)$ où J est une partie de I et $t$ une section continue de E au-dessus de $A_J$ qui coïncide avec $s$ dans $A\cap A_J$. Munissons $\mathscr{S}$ de la relation d’ordre notée $\leqslant$ pour laquelle $(J, t)\leqslant (J', t')$ si $J\subset J'$ et $t'|A_J=t$. Pour $\sigma = (J, t)\in \mathscr{S}$, on note $J_{\sigma}= J$ et $t_{\sigma}=t$. Démontrons que l’ensemble ordonné $\mathscr{S}$ est inductif. Soit S une partie totalement ordonnée de $\mathscr{S}$. Posons $J =\bigcup_{\sigma\in S}J_{\sigma}$; c’est une partie de I. On définit alors une section $t$ de E au-dessus de $A_J$ en posant $t(x) =t_{\sigma}(x)$, si $x\in A_{J_{\sigma}}$; on a donc $t|A\cap A_J=s$. Soit $j\in J$ et soit $\sigma \in S$ tel que $j\in J_{\sigma}$; comme $t|A_j=t_{\sigma}|A_j$, la restriction de $t$ à $A_j$ est continue. Il résulte alors de TG, I, p. 19, prop. 4 que $t$ est continue. Ainsi, $(J, t)$ est un élément de $\mathscr{S}$; par construction, c’est un majorant de S. Cela prouve que l’ensemble $\mathscr{S}$ est inductif. Il possède donc un élément maximal $(J, t)$ (E, III, p. 20, th. 2).

Raisonnons par l’absurde en supposant que J $= I\not$ . Soit $i$ un élément de I-J. Posons $A'= (A_i\cap A)\cup (A_i\cap A_J)$ et définissons une section $s'$ de E au-dessus de $A'$ par :

$'s(a)$ pour $a\in A_i\cap A$,

$$
s(a) =
$$

$t(a)$ pour $a\in A_i\cap A_J$,

ce qui est possible puisque $s$ et $t$ coïncident dans $A\cap A_J$. De plus, comme $A_i\cap A$ et $A_i\cap A_J$ sont fermés, la section $s'$ est continue (TG, I, p. 19, prop. 4). Par hypothèse, il existe une section continue $s_i: A_i\rightarrow E$ prolongeant $s'$. Comme les restrictions de $s_i$ et $t$ à $A_J\cap A_i$ sont égales, l’application $t': A_{J\cup \{i\}}\rightarrow E$ qui coïncide avec $t$ dans $A_J$ et avec $s_i$ dans $A_i$ est une section continue de $p$ au-dessus de $A_{J\cup \{i\}}$, prolongeant $s|A\cap A_{J\cup \{i\}}$. On a alors $(J, t)<(J\cup  \{i\}, t')$, ce qui contredit l’hypothèse que $(J, t)$ est maximal.

Ainsi, J = I, donc $A_J= B$ et $t$ est une section continue de E au-dessus de B prolongeant $s$.

#### Corollaire 1 {#ta-i-s3-prop-6-cor-1 .statement tag=01OP}

Soient B un espace paracompact, $\mathscr{F}$ un faisceau sur B et $(U_i)_{i\in I}$ un recouvrement ouvert de B. Si, pour tout $i\in I$, le faisceau induit $\mathscr{F}|U_i$ est mou, alors le faisceau $\mathscr{F}$ est mou.

Il existe en effet un recouvrement fermé localement fini $(F_j)_{j\in J}$ plus fin que le recouvrement $(U_i)_{i\in I}$ (TG, IX, p. 49, prop. 4 et p. 48, cor. 1). Par suite, pour tout $j\in J$, le faisceau $\mathscr{F}|F_j$ est mou et la proposition implique que le faisceau $\mathscr{F}$ est mou.

#### Corollaire 2 {#ta-i-s3-prop-6-cor-2 .statement tag=01OQ}

Soient B un espace paracompact, $\mathscr{F}$ un faisceau sur B et $(A_i)_{i\in I}$ un recouvrement fermé localement fini de B. Pour que le faisceau $\mathscr{F}$ soit mou, il faut et il suffit que la condition suivante soit satisfaite :

Pour tout $i\in I$, toute partie fermée A de $A_i$, tout ensemble ouvert V de B contenant A et tout élément $s$ de $\mathscr{F}(V)$, il existe un voisinage ouvert U de $A_i$ dans B, un élément $t$ de $\mathscr{F}(U)$ et un voisinage ouvert W de A dans B contenu dans $U\cap V$ tels que $t|W =s|W$.

Supposons que le faisceau $\mathscr{F}$ soit mou et montrons que la condition est satisfaite. Soit $i\in I$, soit A une partie fermée de $A_i$, soit V un ouvert de B contenant A et soit $s$ un élément de $\mathscr{F}(V)$. Posons $s_0=\sigma_{\mathscr{F}}(s)$. C’est une section continue au-dessus de V de l’espace étalé $E_{\mathscr{F}}$. Comme $A_i$ est fermé, A est fermé dans B et $s_0|A$ se prolonge en une section $t_0: B\rightarrow E_{\mathscr{F}}$, par définition d’un faisceau mou. Les sections $s_0$ et $t_0|V$ du V-espace étalé $E_{\mathscr{F}}\times_BV$ coïncident sur A, donc sur un voisinage W de A (I, p. 34, prop. 11, b)).

Réciproquement, supposons que la condition du corollaire soit satisfaite. D’après la proposition 6, il suffit de montrer que, pour tout $i\in I$, le faisceau $\mathscr{F}_{A_i}$ est mou. Soit A une partie fermée de $A_i$ et soit $s_0$ une section de l’espace étalé de $\mathscr{F}|A_i$ au-dessus de A, c’est-à-dire une section continue au-dessus de A de l’espace étalé $E_{\mathscr{F}}$. Comme A est fermé dans B et que B est paracompact, $s_0$ se prolonge en une section $s$ au-dessus d’un voisinage V de A dans B (I, p. 37, th. 2). Par hypothèse, il existe un voisinage ouvert U de $A_i$ dans B et une section $t$ de $E_{\mathscr{F}}$ au-dessus de U qui coïncide avec $s$ sur un voisinage de A. La restriction de $t$ à $A_i$ est une section de $\mathscr{F}_{A_i}$ qui prolonge $s_0$. Le faisceau $\mathscr{F}_{A_i}$ est donc mou. D’après la proposition 6, le faisceau $\mathscr{F}$ est mou.

### 10. Faisceaux de structures

Supposons données une espèce de structure Σ et une notion de $\sigma$-morphisme relative à cette espèce de structure.

Soit B un espace topologique.

On dit qu’un préfaisceau $\mathscr{F}$ sur B est à valeurs dans l’espèce de structure Σ si, pour tout ouvert U de B, l’ensemble $\mathscr{F}(U)$ est muni d’une structure d’espèce Σ et si les applications de restrictions sont des $\sigma$-morphismes.

On dira qu’un tel préfaisceau est un faisceau à valeurs dans l’espèce de structure Σ si, de plus, c’est un faisceau d’ensembles.

Si $\mathscr{F}$ et $\mathscr{G}$ sont des préfaisceaux à valeurs dans l’espèce de structure Σ, on dit qu’un morphisme $\varphi$ est un morphisme de préfaisceaux à valeurs dans Σ si, pour tout ouvert U, l’application $\varphi (U)$ est un $\sigma$-morphisme.

On parlera ainsi, par exemple, de faisceaux de groupes, de groupes abéliens, de $k$-modules (pour un anneau $k$ fixé), d’anneaux, de $k$-algèbres (pour un anneau commutatif $k$ fixé).

Le faisceau sur B des applications à valeurs dans un groupe (resp. un groupe abélien, resp. un $k$-module, resp. un anneau, resp. une $k$-algèbre) est naturellement muni d’une structure de faisceau de groupes (resp. de groupes abéliens, resp. de $k$-modules, resp. d’anneaux, resp. de $k$-algèbres). Si X est une variété différentielle de classe $C^r$ sur $\mathbf{R}$ le faisceau $\mathscr{C}^r(X;\mathbf{R})$ des fonctions numériques de classe $C^r$ est un faisceau de $\mathbf{R}$-algèbres, et le faisceau sur X des sections de classe $C^r$ d’un fibré vectoriel E sur X est un faisceau de $\mathbf{R}$-espaces vectoriels ; un opérateur différentiel définit un morphisme de faisceaux de $\mathbf{R}$-espaces vectoriels.

Pour ces espèces de structure Σ, il résulte de la construction que nous avons donnée que le faisceau $\widetilde{F}$ associé à un préfaisceau $\mathscr{F}$ à valeurs dans l’espèce de structure Σ (des groupes, des groupes abéliens, des $k$-modules, des anneaux, des $k$-algèbres) est un faisceau à valeurs dans cette espèce de structure, et que le morphisme canonique $j_{\mathscr{F}}:\mathscr{F}\rightarrow \widetilde{\mathscr{F}}$ est un morphisme de préfaisceaux à valeurs dans l’espèce de structure Σ.

Par exemple, le faisceau sur B des applications à valeurs dans un groupe est naturellement muni d’une structure de faisceau de groupes.

Soient A et B des espaces topologiques et soit $u: A\rightarrow B$ une application continue. Si $\mathscr{F}$ est un (pré)faisceau sur A à valeurs dans l’espèce de structure Σ, il en est de même du (pré)faisceau $u_*(\mathscr{F})$ image directe du (pré)faisceau $\mathscr{F}$ par $u$.

Supposons de plus que l’espèce de structure Σ soit celle des groupes, des groupes abéliens, des $k$-modules, des anneaux ou des $k$-algèbres. Si $\mathscr{G}$ est un (pré)faisceau sur B à valeurs dans l’espèce de structure Σ, alors le faisceau $u^*\mathscr{G}$ sur A, image réciproque du préfaisceau $\mathscr{G}$ par l’application $u$, est muni d’une structure de faisceau à valeurs dans Σ. Dans ce cas, les morphismes d’adjonction $\alpha$ et $\beta$ sont des morphismes de préfaisceaux à valeurs dans l’espèce de structure Σ. En particulier, si $\varphi :\mathscr{G}\rightarrow u_*\mathscr{F}$ est un morphisme de préfaisceaux à valeurs dans Σ, il en est de même du morphisme $\varphi^{\sharp}$; si $\psi :u^*(\mathscr{G})\rightarrow \mathscr{F}$ est un morphisme de préfaisceaux à valeurs dans Σ, il en est de même du morphisme $\psi^{\flat}$.

## EXERCICES {#ta-i-s3-exercises}

See the [exercises for § 3](exercises/s3/).
