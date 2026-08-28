---
book: top
book_title: General Topology
chapter: I
chapter_title: STRUCTURES TOPOLOGIQUES
section: 3
section_title: Sous-espaces; espaces quotients
lang: fr
source: top-i-iv-fr
book_pages: TG I.17-TG I.24
pdf_pages: 0029-0036, 0105-0106
extraction: ocr
subsections:
    - "no": 1
      title: Sous-espaces d’un espace topologique
      page: 17
      pdf_page: 29
    - "no": 2
      title: Continuité par rapport à un sous-espace
      page: 19
      pdf_page: 31
    - "no": 3
      title: Sous-espaces localement fermés
      page: 20
      pdf_page: 32
    - "no": 4
      title: Espaces quotients
      page: 20
      pdf_page: 32
    - "no": 5
      title: '**Décomposition canonique d’une application continue**'
      page: 21
      pdf_page: 33
    - "no": 6
      title: Espace quotient d’un sous-espace
      page: 23
      pdf_page: 35
statements: 23
exercises: 16
content_sha256: 8f3e8c51c65e8658f192fbec94abe7c09eee805e66a19ea2daa3243d1a0988ef
---

## § 3. SOUS-ESPACES; ESPACES QUOTIENTS

### 1. Sous-espaces d’un espace topologique

Soit $A$ une partie d’un espace topologique $X$. Nous avons défini la topologie induite sur $A$ par la topologie de $X$ comme l’image réciproque de cette dernière par l’injection canonique $A \to X$ (I, p. 13, Exemple I); il revient au même de poser la définition suivante :

#### Définition 1 {#top-i-s3-def-1 .statement}

Soit $A$ une partie d’un espace topologique $X$. On appelle topologie induite sur $A$ par la topologie de $X$ la topologie dont les ensembles ouverts sont les traces sur $A$ des ensembles ouverts de $X$. L’ensemble $A$, muni de cette topologie, est appelé un sous-espace de $X$.

#### Exemple {#top-i-s3-n1-exa-1 .statement}

Sur l’ensemble $\mathbf{Z}$ des entiers rationnels, la topologie induite par celle de la droite rationnelle est la topologie discrète, car la trace sur $\mathbf{Z}$ de l’intervalle ouvert $]n-\frac{1}{2},n+\frac{1}{2}[$ est l’ensemble $\{n\}$.

En vertu de la prop. 5 de I, p. 13 (ou directement à partir de la déf. 1), si $B \subset A \subset X$, le sous-espace $B$ de $X$ est identique au sous-espace $B$ du sous-espace $A$ de $X$ (transitivité des topologies induites). Si $\mathcal{G}$ est un système générateur (resp. une base) de la topologie de $X$ (I, p. 13, Exemple II), sa trace $\mathcal{G}_A$ sur $A$ est un système générateur (resp. une base) de la topologie induite sur $A$.

Dans toutes les questions où interviennent des éléments ou des parties de $A$, il faut soigneusement distinguer entre leurs propriétés en tant que points (resp.

parties) de l’espace X, et leurs propriétés en tant que points (resp. parties) du sous-espace A. On opérera cette distinction en utilisant les locutions « dans A », « par rapport à A », ou « relativement à A » pour préciser les propriétés de la seconde catégorie (éventuellement en les opposant aux locutions « dans X », « par rapport à X », « relativement à X »).

Un ensemble ouvert dans le sous-espace A n’est pas nécessairement ouvert dans X : pour que tout ensemble ouvert dans A soit ouvert dans X, il faut et il suffit que A soit ouvert dans X. En effet, la condition est nécessaire, puisque A est ouvert par rapport à A ; elle est suffisante en vertu de (O_{II}) et de la déf. 1.

Les ensembles fermés dans A sont les traces sur A des ensembles fermés dans X (I, p. 13, Exemple I) ; on voit comme ci-dessus que, pour que tout ensemble fermé dans A soit fermé dans X, il faut et il suffit que A soit fermé dans X.

Les voisinages d’un point $x \in A$ par rapport à A sont les traces sur A des voisinages de $x$ par rapport à X ; pour que tout voisinage de $x$ par rapport à A soit un voisinage de $x$ par rapport à X, il faut et il suffit que A soit un voisinage de $x$ dans X.

#### Proposition 1 {#top-i-s3-prop-1 .statement}

Si A et B sont deux parties d’un espace topologique X telles que B $\subset$ A, l’adhérence de B par rapport au sous-espace A est la trace sur A de l’adhérence $\overline{B}$ de B par rapport à X.

En effet, si $x \in A$, tout voisinage de $x$ par rapport à A est de la forme $V \cap A$, où V est un voisinage de $x$ dans X. Comme $V \cap B = (V \cap A) \cap B$, pour que $x$ soit adhérent à B par rapport à A, il faut et il suffit qu’il soit adhérent à B par rapport à X.

#### Corollaire {#top-i-s3-n1-cor-1 .statement}

Pour qu’une partie B de A soit dense par rapport à A, il faut et il suffit que $\overline{B} = \overline{A}$ dans X (ou, ce qui revient au même, que $A \subset \overline{B}$).

On en conclut que si A, B, C sont trois parties de X telles que $A \supset B \supset C$, et si B est dense par rapport à A et C dense par rapport à B, alors C est dense par rapport à A (transitivité de la densité) ; en effet, on a alors $\overline{A} = \overline{B} = \overline{C}$ dans X.

#### Proposition 2 {#top-i-s3-prop-2 .statement}

Soit A une partie partout dense d’un espace topologique X ; pour tout $x \in A$ et tout voisinage V de $x$ par rapport à A, l’adhérence $\overline{V}$ de V dans X est un voisinage de $x$ par rapport à X.

En effet, V contient la trace $U \cap A$ sur A d’un ensemble U ouvert dans X et contenant $x$, donc $\overline{V}$ contient $U \cap \overline{A} = U$ (I, p. 7, prop. 5).

#### Proposition 3 {#top-i-s3-prop-3 .statement}

Soit $(A_i)_{i \in I}$ une famille de parties d’un espace topologique X, ayant l’une des propriétés suivantes :
a) les intérieurs des $A_i$ forment un recouvrement de X ;
b) $(A_i)_{i \in I}$ est un recouvrement fermé localement fini (I, p. 6) de X.

Dans ces conditions, pour qu’une partie B de X soit ouverte (resp. fermée) dans X, il faut et il suffit que chacun des ensembles $B \cap A_i$ soit ouvert (resp. fermé) dans $A_i$.

La nécessité des conditions est évidente. Pour démontrer qu’elles sont suffisantes, plaçons-nous d’abord dans l’hypothèse a); comme

$$(\mathbf{CB}) \cap A_t = A_t - (B \cap A_t),$$

on peut, par dualité, se borner à considérer le cas où chacun des $B \cap A_t$ est ouvert par rapport à $A_t$; alors $B \cap \bar{A}_t$ est ouvert dans $\bar{A}_t$ pour tout $t \in I$, donc ouvert dans $X$, et comme $B = \bigcup_t (B \cap \bar{A}_t)$ par hypothèse, $B$ est ouvert dans $X$.

Plaçons-nous maintenant dans l’hypothèse b); par dualité, on peut encore se borner à considérer le cas où chacun des $B \cap A_t$ est fermé par rapport à $A_t$; alors $B \cap A_t$ est fermé dans $X$; comme la famille $(B \cap A_t)$ est localement finie, et que $B = \bigcup_t (B \cap A_t)$, $B$ est fermé dans $X$ en vertu de I, p. 6, prop. 4.

#### Remarque {#top-i-s3-n1-rem-1 .statement}

Soit $(U_t)_{t \in I}$ un recouvrement ouvert d’un espace topologique $X$, et pour tout $t \in I$, soit $\mathcal{B}_t$ une base de la topologie de sous-espace $U_t$ de $X$; il est clair que $\mathcal{B} = \bigcup_{t \in I} \mathcal{B}_t$ est une base de la topologie de $X$.

### 2. Continuité par rapport à un sous-espace

Soient $X, Y$ deux espaces topologiques, $f$ une application de $X$ dans $Y$, $B$ une partie de $Y$ contenant $f(X)$. La définition de la topologie induite comme topologie initiale (I, p. 12, prop. 4) montre que pour que $f$ soit continue en $x \in X$, il faut et il suffit que l’application de $X$ dans le sous-espace $B$ de $Y$, ayant même graphe que $f$, soit continue au point $x$.

Soit maintenant $A$ une partie de $X$; si $f$ est continue au point $x \in A$ (resp. continue dans $X$), sa restriction $f|A$ est une application du sous-espace $A$ dans $Y$, qui est continue au point $x$ (resp. continue dans $A$), en vertu de I, p. 9, prop. 2: on dit parfois qu’une application $f : X \to Y$ est continue relativement à $A$ au point $x \in A$ (resp. continue relativement à $A$) si sa restriction $f|A$ est continue au point $x$ (resp. continue dans $A$).

On notera que $f|A$ peut être continue sans que $f$ soit continue en aucun point de $X$: un exemple en est fourni par la fonction caractéristique $\varphi_A$ d’une partie $A$ de $X$ partout dense dans $X$ ainsi que son complémentaire (I, p. 92, exerc. 11); si on considère $\varphi_A$ comme une application de $X$ dans l’espace discret $\{0, 1\}$, $\varphi_A$ n’est continue en aucun point de $X$, mais sa restriction à $A$ est constante, donc continue.

Si $A$ est un voisinage dans $X$ d’un point $x \in A$, et si $f : X \to Y$ est telle que $f|A$ soit continue au point $x$, alors $f$ est continue au point $x$, puisque tout voisinage de $x$ par rapport à $A$ est un voisinage de $x$ par rapport à $X$ (caractère local de la continuité).

#### Proposition 4 {#top-i-s3-prop-4 .statement}

Soit $(A_t)_{t \in I}$ une famille de parties d’un espace topologique $X$, dont les intérieurs forment un recouvrement ouvert de $X$, ou qui est un recouvrement fermé localement fini de X. Soit f une application de X dans un espace topologique X'. Si la restriction de f à chacun des sous-espaces A_i est continue, f est continue.

En effet, si F' est une partie fermée de X' et si on pose F = $\overline{f^{-1}(F')}$, F ∩ A_i est fermé dans A_i pour tout i ∈ I (I, p. 9, th. 1), donc F est fermé dans X en vertu de la prop. 3 de I, p. 11 ; la conclusion résulte du th. 1 de I, p. 9.

### 3. Sous-espaces localement fermés

#### Définition 2 {#top-i-s3-def-2 .statement}

On dit qu’une partie L d’un espace topologique X est localement fermée en un point x ∈ L s’il existe un voisinage V de x dans X tel que L ∩ V soit une partie fermée du sous-espace V. On dit que L est localement fermée dans X si elle est localement fermée en chacun de ses points.

#### Remarque {#top-i-s3-n3-rem-1 .statement}

Soit F une partie de X telle que pour tout point x de X, il y ait un voisinage V de x dans X tel que V ∩ F soit fermé dans le sous-espace V; il résulte alors de la prop. 3 de I, p. 18 que F est fermée dans X. Par contre, il résulte aussitôt de la prop. 5 ci-dessous qu’il existe en général des ensembles localement fermés et non fermés dans X.

#### Proposition 5 {#top-i-s3-prop-5 .statement}

Soit L une partie d’un espace topologique X. Les conditions suivantes sont équivalentes:
a) L est localement fermée;
b) L est une partie ouverte du sous-espace $\overline{L}$, adhérence de L dans E;
c) L est intersection d’une partie ouverte et d’une partie fermée de X.

Il est immédiat que b) implique c), L étant alors l’intersection de $\overline{L}$ et d’une partie ouverte de X; c) implique a) en vertu de la déf. 2. Enfin, a) implique b): en effet, pour tout x ∈ L, il existe alors un voisinage ouvert U de x tel que U ∩ L soit fermé dans U; donc U ∩ $\overline{L}$ = U ∩ L, ce qui montre que dans le sous-espace $\overline{L}$, x est intérieur à L, donc L est ouvert dans $\overline{L}$.

#### Corollaire {#top-i-s3-n3-cor-1 .statement}

Soit f : X → X' une application continue; pour toute partie localement fermée L' de X', $\overline{f^{-1}(L')}$ est localement fermée dans X.
Cela résulte aussitôt de la prop. 5 ci-dessus et de I, p. 9, th. 1.

### 4. Espaces quotients

#### Définition 3 {#top-i-s3-def-3 .statement}

Soient X un espace topologique, R une relation d’équivalence dans X. On appelle espace quotient de X par R l’ensemble quotient X/R, muni de la topologie quotient de la topologie de X par la relation R (I, p. 15, Exemple I).

Sauf mention expresse du contraire, quand nous considérerons désormais X/R comme un espace topologique, il sera sous-entendu qu’il s’agit de l’espace quotient de X par R. On dit souvent que cet espace topologique est l’espace obtenu en identifiant les points de X appartenant à une même classe d’équivalence suivant R.

Soit $\varphi$ l’application canonique $X \to X/R$. Par définition (I, p. 14, prop. 6 et corollaire) les ensembles *ouverts* (resp. *fermés*) dans $X/R$ sont les ensembles $A$ tels que $\varphi^{-1}(A)$ soit *ouvert* (resp. *fermé*) dans $X$; autrement dit, les ensembles ouverts (resp. fermés) dans $X/R$ sont en correspondance biunivoque canonique avec les ensembles ouverts (resp. fermés) dans $X$ *saturés* pour $R$, et sont les images canoniques de ces ensembles.

#### Proposition 6 {#top-i-s3-prop-6 .statement}

*Soient $X$ un espace topologique, $R$ une relation d’équivalence dans $X$, $\varphi$ l’application canonique de $X$ sur $X/R$; pour qu’une application $f$ de $X/R$ dans un espace topologique $Y$ soit continue, il faut et il suffit que $f \circ \varphi$ soit continue dans $X$.*

Ce n’est qu’un cas particulier de I, p. 14, prop. 6, exprimant que la topologie quotient est topologie *finale* pour l’application $\varphi$.

La prop. 6 montre qu’il existe une correspondance biunivoque canonique entre les applications continues de $X/R$ dans $Y$ et les applications continues de $X$ dans $Y$, *constantes dans toute classe d’équivalence suivant $R$*.

#### Exemple {#top-i-s3-n4-exa-1 .statement}

*Considérons, sur la droite numérique $\mathbf{R}$, la relation d’équivalence $x \equiv y$ (mod. 1); l’espace quotient de $\mathbf{R}$ par cette relation est appelé *tore à une dimension* et se désigne par $\mathbf{T}$. La classe d’équivalence d’un point $x \in \mathbf{R}$ se compose de tous les points $x + n$, où $n$ parcourt l’ensemble $\mathbf{Z}$ des entiers rationnels. D’après la prop. 6, il y a correspondance biunivoque entre les fonctions continues dans $\mathbf{T}$ et les fonctions *périodiques* de période 1, continues dans $\mathbf{R}$. Nous reviendrons dans V, §1, no 2 sur cet important exemple.*

#### Corollaire {#top-i-s3-n4-cor-1 .statement}

*Soient $X, Y$, deux espaces topologiques, $R$ (resp. $S$) une relation d’équivalence dans $X$ (resp. $Y$), $f : X \to Y$ une application continue compatible avec les relations d’équivalence $R$ et $S$ (E, II, p. 44); alors l’application $g : X/R \to Y/S$ déduite de $f$ par passage aux quotients (E, II, p. 45) est continue.*

C’est un cas particulier d’une propriété générale des structures quotients (E, IV, p. 21, critère CST 20).

**Proposition 7** (transitivité des espaces quotients). — *Soient $R$ et $S$ deux relations d’équivalence dans un espace topologique $X$, telles que $R$ entraîne $S$, et soit $S/R$ la relation d’équivalence quotient dans l’espace quotient $X/R$ (E, II, p. 46). L’application canonique bijective $(X/R)/(S/R) \to X/S$ est alors un homéomorphisme.*

C’est un cas particulier de la transitivité des topologies finales (I, p. 14, prop. 7; cf. E, II, p. 22, critère CST 21).

### 5. **Décomposition canonique d’une application continue**

Soient $X, Y$ deux espaces topologiques, $f : X \to Y$ une application continue, $R$ la relation d’équivalence $f(x) = f(y)$ dans $X$. Considérons la *décomposition canonique*:

$$
f : X \xrightarrow{\varphi} X/R \xrightarrow{g} f(X) \xrightarrow{\psi} Y
$$

où $\varphi$ est l’application canonique (surjective) de $X$ dans l’espace quotient $X/R$, $\psi$ l’injection canonique du sous-espace $f(X)$ dans $Y$ et $g$ la bijection associée à $f$ (E, II, p. 14). Il est immédiat que $g$ est continue (par la prop. 6 de I, p. 14) ce qui est d’ailleurs un cas particulier d’un résultat général sur les structures quotients (cf. E, IV, p. 21). Mais la bijection $g$ n’est pas nécessairement un homéomorphisme.

#### Proposition 8 {#top-i-s3-prop-8 .statement}

Soient $f = \psi \circ g \circ \varphi$ la décomposition canonique d’une application continue $f : X \to Y$, $R$ la relation d’équivalence $f(x) = f(y)$. Les trois conditions suivantes sont équivalentes:
a) $g$ est un homéomorphisme de $X/R$ sur $f(X)$.
b) L’image par $f$ de tout ensemble ouvert saturé pour $R$ est un ensemble ouvert dans le sous-espace $f(X)$.
c) L’image par $f$ de tout ensemble fermé saturé pour $R$ est un ensemble fermé dans le sous-espace $f(X)$.

En effet, la condition b) (resp. c)) exprime que l’image par $g$ de tout ensemble ouvert (resp. fermé) dans $X/R$ est un ensemble ouvert (resp. fermé) dans $f(X)$.

#### Exemple {#top-i-s3-n5-exa-1 .statement}

Soient $X$ un espace topologique, $(X_t)_{t \in I}$ un recouvrement de $X$, $Y$ l’espace somme des sous-espaces $X_t$ de $X$; il y a donc une partition $(Y_t)_{t \in I}$ de $Y$ en sous-espaces à la fois ouverts et fermés, et pour chaque $t \in I$ un homéomorphisme $f_t : Y_t \to X_t$. Soit $f : Y \to X$ l’application continue qui coïncide avec $f_t$ dans $Y_t$ pour tout $t \in I$, et soit $R$ la relation d’équivalence $f(x) = f(y)$; l’espace quotient $Y/R$ est donc obtenu par « recollement » des $Y_t$ (I, p. 17). Considérons la bijection $g : Y/R \to X$, associée à $f$; en général $g$ n’est pas un homéomorphisme, comme le montre l’exemple où on prend tous les $X_t$ réduits à un point, $X$ étant supposé non discret. Toutefois, si les intérieurs des $X_t$ forment un recouvrement de $X$, ou si $(X_t)$ est un recouvrement fermé localement fini de $X$, $g$ est un homéomorphisme; en effet, pour toute partie ouverte $U$ de $Y$, saturée pour $R$, et pour tout $t \in I$, $f(U) \cap X_t = f_t(U \cap Y_t)$ est ouvert dans $X_t$, et la conclusion résulte de la prop. 3 de I. p. 18.

La proposition suivante donne une condition suffisante simple pour que $g$ soit un homéomorphisme:

#### Proposition 9 {#top-i-s3-prop-9 .statement}

Soient $f : X \to Y$ une application continue surjective, $R$ la relation d’équivalence $f(x) = f(y)$. S’il existe une section continue $s : Y \to X$ associée à $f$ (E, II, p. 18, déf. 11), l’application $g : X/R \to Y$ associée à $f$ est un homéomorphisme, et $s$ est un homéomorphisme de $Y$ sur le sous-espace $s(Y)$ de $X$.

En effet, si $\varphi : X \to X/R$ est l’application canonique, $g$ et $\varphi \circ s$ sont bijectives, continues et réciproques l’une de l’autre; de même $s$ et la restriction de $f$ à $s(Y)$ sont continues, bijectives et réciproques l’une de l’autre.

Lorsque $R$ est une relation d’équivalence dans un espace topologique $X$ et $\varphi : X \to X/R$ l’application canonique, toute section continue $s : X/R \to X$ associée à $\varphi$ est aussi appelée section continue de $X$ pour $R$ (cf. E, II, p. 42); le sous-espace $s(X/R)$ de $X$ est alors homéomorphe à $X/R$. On notera que la donnée de $s(X/R)$ détermine complètement $s$; aussi dit-on souvent par abus de langage que $s(X/R)$ est une section (continue) de $X$ pour $R$.

On notera qu’il n’existe pas nécessairement de section continue pour une relation d’équivalence dans un espace topologique (I, p. 94, exerc. 12).

### 6. Espace quotient d’un sous-espace

Soient X un espace topologique, A un sous-espace de X, R une relation d’équivalence dans X, f l’application canonique X → X/R, g sa restriction à A. La relation d’équivalence g(x) = g(y) dans A n’est autre que la relation R_A induite par R dans A (E, II, p. 45). Soit g = ψ ∘ h ∘ φ la décomposition canonique de g, de sorte que si j est l’injection canonique de A dans X, on a le diagramme commutatif¹

(1)

$$
\begin{array}{ccc}
A & \xrightarrow{\varphi} & A/R_A \\
& & \downarrow \\
& & X
\end{array}
$$

$$
\begin{array}{ccc}
A/R_A & \xrightarrow{k} & f(A) \\
& & \downarrow \\
f(A) & \xrightarrow{\psi} & X/R.
\end{array}
$$

#### Proposition 10 {#top-i-s3-prop-10 .statement}

*La bijection canonique h : A/R_A → f(A) est continue. En outre, les trois propriétés suivantes sont équivalentes*:

a) *h est un homéomorphisme*;
b) *tout ensemble ouvert dans A et saturé pour R_A est la trace sur A d’un ensemble ouvert dans X et saturé pour R*;
c) *tout ensemble fermé dans A et saturé pour R_A est la trace sur A d’un ensemble fermé dans X et saturé pour R*.

La première partie de la proposition est immédiate (I, p. 22). La seconde résulte de la prop. 8 de I, p. 22 : si B est un ensemble ouvert (resp. fermé) dans A et saturé pour R_A, et si g(B) = f(B) est la trace sur f(A) d’un ensemble C ouvert (resp. fermé) dans X/R, B est la trace sur A de l’ensemble ouvert (resp. fermé) $f^{-1}(C)$ saturé pour R ; et réciproquement, si B est la trace sur A d’un ensemble ouvert (resp. fermé) D saturé pour R, f(B) est la trace sur f(A) de f(D), qui est ouvert (resp. fermé) dans X/R.

#### Corollaire 1 {#top-i-s3-prop-10-cor-1 .statement}

*Si A est un ensemble saturé pour R et ouvert (resp. fermé) dans X, l’application canonique h : A/R_A → f(A) est un homéomorphisme*.

En effet, si A est ouvert (resp. fermé) et saturé pour R, et si B ⊂ A est ouvert (resp. fermé) dans A et saturé pour R_A, B est ouvert (resp. fermé) dans X et saturé pour R.

#### Corollaire 2 {#top-i-s3-prop-10-cor-2 .statement}

*S’il existe une application continue u : X → A telle que, pour tout x ∈ X, u(x) soit congru à x mod. R, alors f(A) = X/R et l’application canonique h : A/R_A → X/R est un homéomorphisme*.

En effet, comme toute classe d’équivalence suivant R rencontre A, l’image

¹ Cette expression signifie que l’on a $f \circ j = \psi \circ h \circ \varphi$.

canonique de $A / R_A$ dans $X / R$ est identique à $X / R$; d’autre part, si $U$ est ouvert dans $A$ et saturé pour $R_A$, il résulte de l’hypothèse que $u^{-1}(U)$ est identique à l’ensemble obtenu en saturant $U$ pour $R$; comme $u$ est continue, $u^{-1}(U)$ est ouvert dans $X$ (I, p. 9, th. 1) d’où le corollaire, en vertu de la prop. 10.

#### Exemple {#top-i-s3-n6-exa-1 .statement}

*Désignons par $R$ la relation d’équivalence $x \equiv y$ (mod. 1) dans la droite numérique $\mathbf{R}$ (I, p. 21, *Exemple*), par $A$ l’intervalle fermé $[0, 1]$; $A$ contient un point au moins de toute classe d’équivalence suivant $R$. L’application canonique de $A / R_A$ sur le tore $T$ est un homéomorphisme; en effet, soit $F$ un ensemble fermé dans $A$ (donc dans $\mathbf{R}$); pour saturer $F$ pour la relation $R$, il faut prendre la réunion des ensembles fermés $F + n$ (pour $n \in \mathbf{Z}$), qui forment évidemment une famille localement finie; leur réunion est donc fermée (I, p. 6, prop. 4), d’où notre assertion. On observera que $A / R_A$ s’obtient en identifiant dans $A$ les points 0 et 1.*

## EXERCICES {#top-i-s3-exercises}

See the [exercises for § 3](exercises/s3/).
