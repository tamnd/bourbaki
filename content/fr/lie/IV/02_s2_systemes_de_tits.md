---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IV
chapter_title: Groupes de Coxeter et systèmes de Tits
section: 2
section_title: Systèmes de Tits
lang: fr
source: lie-iv-vi-fr
pdf_pages: 0021-0031, 0045-0055
extraction: ocr
subsections:
    - "no": 1
      title: Définition et premières propriétés
      page: 0
      pdf_page: 21
    - "no": 2
      title: Un exemple
      page: 0
      pdf_page: 23
    - "no": 3
      title: Décomposition de $G$ en doubles classes
      page: 0
      pdf_page: 24
    - "no": 4
      title: Relations avec les systèmes de Coxeter
      page: 0
      pdf_page: 24
    - "no": 5
      title: Sous-groupes de $G$ contenant $B$
      page: 0
      pdf_page: 26
    - "no": 6
      title: Sous-groupes paraboliques
      page: 0
      pdf_page: 28
    - "no": 7
      title: Théorème de simplicité
      page: 0
      pdf_page: 29
statements: 31
exercises: 29
content_sha256: deb36ce1ee638d8755f25803d603187d1b22b18c6854e52925925f2e3c08cec9
---

## § 2. Systèmes de Tits

Dans ce paragraphe, les lettres G, B, N, S, T, W ont la signification indiquée au n° 1 ci-dessous.

### 1. Définition et premières propriétés

Soient G un groupe et B un sous-groupe de G. On fait opérer le groupe $B \times B$ sur G par la loi $(b, b') . g = bgb'^{-1}$ pour $b, b' \in B$ et $g \in G$. Les orbites de $B \times B$ dans G sont les ensembles $BgB$, pour $g \in G$, qu’on appelle *doubles classes* de G suivant B. Elles forment une *partition* de G ; l’ensemble quotient correspondant se note $B \backslash G / B$. Si C et C’ sont deux doubles classes, CC’ est *réunion* de doubles classes.

#### Définition 1 {#lie-iv-s2-def-1 .statement}

*On appelle système de Tits un quadruplet* $(G, B, N, S)$, *où G est un groupe, B et N deux sous-groupes de G et S une partie de N/(B \cap N)*, *satisfaisant aux axiomes suivants* :

(T1) *L’ensemble* $B \cup N$ *engendre G et* $B \cap N$ *est un sous-groupe distingué de N*.
(T2) *L’ensemble* S *engendre le groupe* $W = N/(B \cap N)$ *et se compose d’éléments d’ordre 2*.
(T3) *On a* $sBw \subset BwB \cup BswB$ *pour* $s \in S$ *et* $w \in W$ (*).
(T4) *Pour tout* $s \in S$, *on a* $sBs \subset B$.

Le groupe $W = N/(B \cap N)$ est parfois appelé le *groupe de Weyl* du système de Tits $(G, B, N, S)$.

#### Remarque 1 {#lie-iv-s2-n1-rem-1 .statement}

On verra au n° 5 (cor. du th. 3) que, si $(G, B, N)$ sont donnés, il existe au plus une partie S de $N/(B \cap N)$ telle que $(G, B, N, S)$ soit un système de Tits.

(*) Tout élément de W est une classe modulo $B \cap N$, donc un sous-ensemble de G ; ceci donne un sens aux produits tels que $BwB$. Plus généralement, pour toute partie A de W, nous noterons BAB le sous-ensemble $\bigcup_{w \in A} BwB$.

n° 2.1.

#### Remarque 2 {#lie-iv-s2-n1-rem-2 .statement}

Soit (G, B, N, S) un système de Tits, et soit Z un sous-groupe distingué de G contenu dans B. Soient $G' = G/Z$, $B' = B/Z$, $N' = N/(Z \cap N)$, et soit $S'$ l’image de S dans $N'/(B' \cap N')$. Alors on voit aussitôt que $(G', B', N', S')$ est un système de Tits.

Dans tout ce paragraphe, (G, B, N, S) désigne un système de Tits, on pose $T = B \cap N$ et $W = N/T$. Par double classe, on entend une double classe de G suivant B. Pour tout $w \in W$, on pose $C(w) = BwB$; c’est une double classe.

Nous allons déduire quelques conséquences élémentaires des axiomes (T1) à (T4). On note $w, w', \ldots$ des éléments de W et $s, s', \ldots$ des éléments de S. On a les relations évidentes

(1) $C(1) = B, \quad C(ww') \subset C(w) \cdot C(w'), \quad C(w^{-1}) = C(w)^{-1}$.

L’axiome (T3) s’écrit aussi sous la forme

(2) $C(s) \cdot C(w) \subset C(w) \cup C(sw)$.

Comme on a par ailleurs $C(sw) \subset C(s) \cdot C(w)$ d’après (1) et que $C(s) \cdot C(w)$ est réunion de doubles classes, il n’y a que deux possibilités

#### Remarque 3 {#lie-iv-s2-n1-rem-3 .statement}

$C(s) \cdot C(w) = \begin{cases} C(sw) & \text{si } C(w) \not\subset C(s) \cdot C(w) \\ C(w) \cup C(sw) & \text{si } C(w) \subset C(s) \cdot C(w) . \end{cases}$

On a $B \neq C(s) \cdot C(s)$ d’après (T4); faisant $w = s$ dans (3) et utilisant la relation $s^2 = 1$, on obtient

#### Remarque 4 {#lie-iv-s2-n1-rem-4 .statement}

$C(s) \cdot C(s) = B \cup C(s)$.

Cette formule montre que $B \cup C(s)$ est un sous-groupe de G. Multiplions les deux membres de (4) à droite par $C(w)$, utilisons la formule (3) et la relation

$$ B \cdot C(w) = C(w); $$

on obtient

#### Remarque 5 {#lie-iv-s2-n1-rem-5 .statement}

$C(s) \cdot C(s) \cdot C(w) = C(w) \cup C(sw)$.

Si l’on prend les inverses des ensembles intervenant dans les formules (2), (3) et (5) et qu’on y remplace $w$ par $w^{-1}$, on obtient les formules

(2') $C(w) \cdot C(s) \subset C(w) \cup C(ws)$

(3') $C(w) \cdot C(s) = \begin{cases} C(ws) & \text{si } C(w) \not\subset C(w) \cdot C(s) \\ C(w) \cup C(ws) & \text{si } C(w) \subset C(w) \cdot C(s) . \end{cases}$

(5') $C(w) \cdot C(s) \cdot C(s) = C(w) \cup C(ws)$.

#### Lemme 1 {#lie-iv-s2-lem-1 .statement}

Soient $s_1, \ldots, s_q \in S$ et soit $w \in W$. On a

$$ C(s_1 \ldots s_q) \cdot C(w) \subset \bigcup_{(i_1, \ldots, i_p)} C(s_{i_1} \ldots s_{i_p} w), $$

où $(i_1, \ldots, i_p)$ décrit l’ensemble des suites strictement croissantes d’entiers de l’intervalle $[1, q]$.

On raisonne par récurrence sur $q$, le cas $q = 0$ étant trivial. Si $q \geqslant 1$, on a $\mathrm{C}(s_1 \ldots s_q) \cdot \mathrm{C}(w) \subset \mathrm{C}(s_1) \cdot \mathrm{C}(s_2 \ldots s_q) \cdot \mathrm{C}(w)$. D’après l’hypothèse de récurrence, $\mathrm{C}(s_2 \ldots s_q) \cdot \mathrm{C}(w)$ est contenu dans la réunion des $\mathrm{C}(s_{j_1} \ldots s_{j_p} w)$, où
$$
2 \leq j_1 < \cdots < j_p \leq q.
$$
D’après (T3), l’ensemble $\mathrm{C}(s_1) \cdot \mathrm{C}(s_{j_1} \ldots s_{j_p} w)$ est contenu dans la réunion de $\mathrm{C}(s_1 s_{j_1} \ldots s_{j_p} w)$ et de $\mathrm{C}(s_{j_1} \ldots s_{j_p} w)$. D’où le lemme.

### 2. Un exemple

Soient $k$ un corps, $n$ un entier $\geq 0$, et soit $(e_i)$ la base canonique de $k^n$. Soit $G = \mathbf{GL}(n, k)$, soit $B$ le sous-groupe trigonal large supérieur de $G$ (formé des matrices triangulaires supérieures), et soit $N$ le sous-groupe de $G$ formé des matrices n’ayant qu’un seul élément non nul dans chaque ligne et dans chaque colonne. Un élément de $N$ permutte les droites $ke_i$; on en déduit un homomorphisme surjectif $N \to \mathfrak{S}_n$ dont le noyau est le sous-groupe $T = B \cap N$ des matrices diagonales; cela permet d’identifier $W = N/T$ et $\mathfrak{S}_n$. On désigne par $s_j$ ($1 \leq j \leq n - 1$) l’élément de $W$ correspondant à la transposition de $j$ et $j + 1$; soit $S$ l’ensemble des $s_j$. *Le quadruplet* $(G, B, N, S)$ *est un système de Tits*. En effet :

L’axiome (T1) résulte du cor. 2 de la prop. 14 de *Alg.*, chap. II, 3e éd., § 10, no 13.

L’axiome (T2) est démontré dans *Alg.*, Chap. I, nouv. éd., Rectif. à la p. 97.

L’axiome (T4) est immédiat.

Reste à vérifier (T3), i.e.
$$
s_j B w \subset B w B \cup B s_j w B \quad \text{pour} \quad 1 \leq j \leq n - 1, w \in W
$$
ou, ce qui revient au même :
$$
s_j B \subset BB' \cup Bs_j B', \quad \text{avec} \quad B' = w B w^{-1}.
$$
Soit $G_j$ le sous-groupe de $G$ formé des éléments laissant fixes les $e_i$ pour $i \neq j, j + 1$ et laissant stable le plan engendré par $e_j$ et $e_{j+1}$; ce groupe est isomorphe à $\mathbf{GL}(2, k)$. On vérifie que $G_j B = BG_j$. Comme $s_j \in G_j$, on a $s_j B \subset BG_j$, et il suffit de prouver la formule
$$
G_j \subset (B \cap G_j)(B' \cap G_j) \cup (B \cap G_j)s_j(B' \cap G_j).
$$
Identifions $G_j$ à $\mathbf{GL}(2, k)$; le groupe $B \cap G_j$ s’identifie au sous-groupe trigonal large supérieur $B_2$ de $\mathbf{GL}(2, k)$; le groupe $B' \cap G_j$ s’identifie à $B_2$ lorsque $w(j) < w(j + 1)$, et au sous-groupe trigonal large inférieur $B_2^-$ sinon. Dans le premier cas, la formule à démontrer s’écrit
$$
\mathbf{GL}(2, k) = B_2 \cup B_2 s B_2 \quad \text{où} \quad s = \begin{pmatrix} 0 & 1 \\ 1 & 0 \end{pmatrix};
$$

n° 2.4.

elle résulte par exemple du fait que $B_2$ est le stabilisateur d’un point dans l’action de $\mathbf{GL}(2, k)$ sur la droite projective $\mathbf{P}_1(k)$, et opère transitiement sur le complémentaire de ce point. Dans le second cas, la formule à démontrer s’écrit

$$
\mathbf{GL}(2, k) = B_2 B_2^- \cup B_2 s B_2^-;
$$

comme $B_2^- = s B_2 s$, elle résulte de la précédente par multiplication à droite par $s$.

### 3. Décomposition de $G$ en doubles classes

#### Théorème 1 {#lie-iv-s2-thm-1 .statement}

On a $G = \mathrm{BWB}$. L’application $w \mapsto C(w)$ est une bijection de $W$ sur l’ensemble $B \backslash G / B$ des doubles classes de $G$ suivant $B$.

Il est clair que $\mathrm{BWB}$ est stable par $x \mapsto x^{-1}$, et le lemme 1 montre qu’il est stable par produit. Comme il contient $B$ et $N$, il est donc égal à $G$.

Il nous reste à prouver que $C(w) \neq C(w')$ si $w \neq w'$. Pour cela, nous démontrerons par récurrence sur l’entier $q$ l’assertion suivante :

(A_q) Étant donnés $w$ et $w'$ distincts dans $W$ tels que $l_s(w) \geq l_s(w') = q$, on a $C(w) \neq C(w')$.

(Pour la définition de $l_s(w)$, voir § 1, n° 1.)

Cette assertion est évidente pour $q = 0$, car on a alors $w' = 1$ et $w \neq 1$, d’où $C(w') = B$ et $C(w) \neq B$.

Supposons que $q \geq 1$ et que $w, w'$ vérifient les hypothèses de (A_q). Il existe $s \in S$ tel que $sw'$ soit de longueur $q - 1$. On a

(6)
$$
l_s(w) > l_s(sw')
$$
d’où $w \neq sw'$. De plus, on a $sw \neq sw'$; d’après la formule (3) du § 1, n° 1, on a

(7)
$$
l_s(sw) \geq l_s(w) - 1 \geq l_s(sw') = q - 1.
$$

Vu l’hypothèse de récurrence, $C(sw')$ est distinct de $C(w)$ et de $C(sw)$; de la formule (2), on déduit

(8)
$$
C(sw') \cap C(s) \cdot C(w) = \varnothing.
$$

Comme on a par ailleurs $C(sw') \subset C(s) \cdot C(w')$, on a finalement $C(w) \neq C(w')$.

#### Remarque {#lie-iv-s2-n3-rem-1 .statement}

L’axiome (T4) n’a pas été utilisé dans la démonstration précédente.

### 4. Relations avec les systèmes de Coxeter

#### Théorème 2 {#lie-iv-s2-thm-2 .statement}

Le couple $(W, S)$ est un système de Coxeter. De plus, pour $s \in S$ et $w \in W$, les relations $C(sw) = C(s) \cdot C(w)$ et $l_s(sw) > l_s(w)$ sont équivalentes.

Pour tout $s \in S$, soit $P_s$ l’ensemble des éléments $w \in W$ tels que

$$
C(s) \cdot C(w) = C(sw).
$$

La condition (A') est évidente.

Vérifions (B'). Si $P_s$ et $sP_s$ avaient un élément commun $w$, on aurait $w \in P_s$ et $sw \in P_s$ d’où

$$
C(s) \cdot C(w) = C(sw), \quad C(s) \cdot C(sw) = C(w).
$$

On en déduirait $C(s) \cdot C(s) \cdot C(w) = C(w)$ et, d’après la formule (5), ceci entraînerait $C(w) = C(sw)$, en contradiction avec le th. 1.

Vérifions (C). Soient $s, s' \in S$ et $w, w' \in W$ avec $w' = ws'$. On fait l’hypothèse que $w \in P_s$ et $w' \notin P_s$, d’où

(9) $$ C(sw) = C(s) \cdot C(w) $$
(10) $$ C(w') \subset C(s) \cdot C(w') $$

d’après (3).

De (9) et de la relation $w = w's'$, on déduit

(11) $$ C(s)w's'B = C(sw). $$

D’après la formule (2'), on a $C(w')C(s') \subset C(w') \cup C(w's')$, d’où immédiatement

(12) $$ C(w')s'B \subset C(ws') \cup C(w). $$

Comme $C(w')$ est réunion de classes à gauche $gB$ et que l’on a

$$
C(s)C(w') = C(s)w'B,
$$

la formule (10) montre que $C(s)w'$ rencontre $C(w')$ et *a fortiori* que $C(s)w's'B$ rencontre $C(w')s'B$. Il résulte alors des formules (11) et (12) que la double classe $C(sw)$ est égale à l’une des doubles classes $C(ws')$ et $C(w)$; comme on a $sw \neq w$, le th. 1 permet de conclure que $sw = ws'$.

#### Corollaire 1 {#lie-iv-s2-thm-2-cor-1 .statement}

*Soient* $w_1, \ldots, w_q \in W$ *et soit* $w = w_1 \ldots w_q$. *Si*

$$
l_s(w) = l_s(w_1) + \cdots + l_s(w_q),
$$

*on a*

$$
C(w) = C(w_1) \ldots C(w_q).
$$

En prenant des décompositions réduites des $w_i$, on se ramène au cas d’une décomposition réduite

$$
w = s_1 \ldots s_q, \quad \text{avec } s_i \in S.
$$

Si $u = s_2 \ldots s_q$, on a alors $w = s_1u$ et $l_s(s_1u) > l_s(u)$, d’où $C(w) = C(s_1) \cdot C(u)$ d’après le théorème; la formule cherchée s’en déduit par récurrence sur $q$.

n° 2.5.

#### Corollaire 2 {#lie-iv-s2-thm-2-cor-2 .statement}

Soit $w \in W$ et soit $T_w$ la partie de $W$ associée à $w$ par le procédé du lemme 2 du § 1, n° 4. Si $t \in T_w$, on a
$$
C(t) \subset C(w) \cdot C(w^{-1}).
$$
Si $t \in T_w$, il existe par définition des éléments $w', w'' \in W$ et $s \in S$ tels que
$$
w = w' s w'', \quad l_s(w) = l_s(w') + l_s(w'') + 1 \quad \text{et} \quad t = w' s w'^{-1}.
$$
D’après le cor. 1, on a
$$
C(w) \cdot C(w^{-1}) = C(w') \cdot C(s) \cdot C(w'') \cdot C(w''^{-1}) \cdot C(s) \cdot C(w'^{-1}).
$$
D’où :
$$
C(w) \cdot C(w^{-1}) \supset C(w') \cdot C(s) \cdot C(s) \cdot C(w'^{-1}).
$$
D’après (4), on a $C(s) \subset C(s) \cdot C(s)$. D’où :
$$
C(w) \cdot C(w^{-1}) \supset C(w') \cdot C(s) \cdot C(w'^{-1}) \supset C(t).
$$

#### Corollaire 3 {#lie-iv-s2-thm-2-cor-3 .statement}

Soit $w \in W$ et soit $H_w$ le sous-groupe de $G$ engendré par $C(w) \cdot C(w^{-1})$. Alors :
a) Pour toute décomposition réduite $(s_1, \ldots, s_q)$ de $w$, on a
$$
C(s_j) \subset H_w \quad \text{pour} \quad 1 \leq j \leq q.
$$
b) Le groupe $H_w$ contient $C(w)$ et est engendré par $C(w)$.
Démontrons a) par récurrence sur $j$. Supposons que $C(s_k)$ soit contenu dans $H_w$ pour $k < j$. Soit
$$
t = (s_1 \ldots s_{j-1}) s_j (s_1 \ldots s_{j-1})^{-1}.
$$
L’élément $t$ appartient à la partie $T_w$ de $W$ définie dans le lemme 2 du § 1, n° 4. D’après le cor. 2, on a $C(t) \subset H_w$, d’où $C(s_j) \subset H_w$.
Comme $C(w) = C(s_1) \ldots C(s_q)$, cf. cor. 1, on a $C(w) \subset H_w$, d’où b).

#### Exemple {#lie-iv-s2-n4-exa-1 .statement}

Le th. 2, appliqué au système de Tits décrit au n° 2, montre que le groupe symétrique $\mathfrak{S}_n$, muni de l’ensemble des transpositions d’éléments consécutifs, est un groupe de Coxeter.

### 5. Sous-groupes de $G$ contenant $B$

Pour toute partie $X$ de $S$, on note $W_X$ le sous-groupe de $W$ engendré par $X$ (cf. § 1, n° 8) et $G_X$ la réunion $BW_X B$ des doubles classes $C(w)$, $w \in W_X$. On a $G_\varnothing = B$, et $G_S = G$.

#### Théorème 3 {#lie-iv-s2-thm-3 .statement}

a) Pour toute partie $X$ de $S$, l’ensemble $G_X$ est un sous-groupe de $G$, engendré par $\bigcup_{s \in X} C(s)$.
b) L’application $X \mapsto G_X$ est une bijection de $\mathcal{P}(S)$ sur l’ensemble des sous-groupes de $G$ contenant $B$.

c) Soit $(X_i)_{i \in I}$ une famille de parties de $S$. Si $X = \bigcap_{i \in I} X_i$, on a $G_X = \bigcap_{i \in I} G_{X_i}$.

d) Soient $X$ et $Y$ deux parties de $S$. On a $G_X \subset G_Y$ (resp. $G_X = G_Y$) si et seulement si l’on a $X \subset Y$ (resp. $X = Y$).

Il est clair que $G_X = (G_X)^{-1}$; le lemme 1 du n° 1 montre que $G_X . G_X \subset G_X$; d’où a), compte tenu du cor. 1 du th. 2.

L’injectivité de $X \mapsto G_X$ résulte de celle de $X \mapsto W_X$ (\S 1, n° 8, th. 2). Soit d’autre part $H$ un sous-groupe de $G$ contenant $B$. Soit $U$ l’ensemble des $w \in W$ tels que $C(w) \subset H$. On a $H = BUB$ puisque $H$ est réunion de doubles classes. Soit $X = U \cap S$; montrons que $H = G_X$. On a évidemment $G_X \subset H$. D’autre part, soit $u \in U$, et soit $(s_1, \ldots, s_q)$ une décomposition réduite de $u$. Le cor. 3 du th. 2 entraîne $C(s_j) \subset H$, d’où $s_j \in X$ pour $1 \leq j \leq q$. On a donc $u \in W_X$, et comme $H$ est réunion des $C(u)$ pour $u \in U$, on a bien $H \subset G_X$, ce qui achève de prouver $(b)$.

Les assertions c) et d) résultent des propriétés analogues des groupes $W_X$ (\S 1, n° 8, th. 2).

#### Corollaire {#lie-iv-s2-n5-cor-1 .statement}

L’ensemble $S$ se compose des éléments $w \in W$ tels que $w \neq 1$ et que $B \cup C(w)$ soit un sous-groupe de $G$.

Les éléments $w \in W$ tels que $B \cup C(w)$ soit un sous-groupe de $G$ sont ceux pour lesquels il existe $X \subset S$ avec $W_X = \{1, w\}$. Si de plus $w \neq 1$, on a nécessairement $\operatorname{Card}(X) = 1$, i.e. $w \in S$.

Remarque 1). — Le corollaire ci-dessus montre que $S$ est déterminé par $(G, B, N)$; pour cette raison, on se permet parfois de dire que $(G, B, N)$ est un système de Tits, ou encore que $(B, N)$ est un système de Tits dans $G$.

#### Proposition 1 {#lie-iv-s2-prop-1 .statement}

Soient $X$ une partie de $S$, et $N'$ un sous-groupe de $N$ dont l’image dans $W$ soit égale à $W_X$. Alors $(G_X, B, N', X)$ est un système de Tits.

On a $G_X = BW_X B = BN'B$, ce qui prouve que $G_X$ est engendré par $B \cup N'$. La vérification des axiomes (T1) à (T4) est alors immédiate.

#### Proposition 2 {#lie-iv-s2-prop-2 .statement}

Soient $X, Y \subset S$ et $w \in W$. On a

$$
G_X w G_Y = BW_X w W_Y B.
$$

Soient $s_1, \ldots, s_q \in X$ et $t_1, \ldots, t_q \in Y$. Le lemme 1 montre que l’on a

$$
C(s_1 \ldots s_q) . C(w) . C(t_1 \ldots t_q) \subset BW_X w W_Y B,
$$

d’où

$$
G_X w G_Y \subset BW_X w W_Y B.
$$

L’inclusion opposée est évidente.

Remarque 2). — Notons $G_X|G/G_Y$ l’ensemble des parties de $G$ de la forme $G_X g G_Y$, $g \in G$; définissons de manière analogue $W_X|W/W_Y$. La proposition précédente montre que la bijection canonique $w \mapsto C(w)$ de $W$ sur $B|G/B$ définit par passage au quotient une bijection $W_X|W/W_Y \to G_X|G/G_Y$.

n° 2.6.

SYSTÈMES DE TITS

#### Proposition 3 {#lie-iv-s2-prop-3 .statement}

Soient $X \subset S$ et $g \in G$. La relation $g B g^{-1} \subset G_X$ entraîne $g \in G_X$.

Soit $w \in W$ tel que $g \in C(w)$. Comme $B$ est un sous-groupe de $G_X$, l’hypothèse $g B g^{-1} \subset G_X$ entraîne $C(w) . C(w^{-1}) \subset G_X$, d’où $C(w) \subset G_X$ d’après le cor. 3 du th. 2, et $g$ appartient à $G_X$.

### 6. Sous-groupes paraboliques

#### Définition 2 {#lie-iv-s2-def-2 .statement}

On dit qu’un sous-groupe de $G$ est parabolique s’il contient un conjugué de $B$.
Il est clair que tout sous-groupe qui contient un sous-groupe parabolique est parabolique.

#### Proposition 4 {#lie-iv-s2-prop-4 .statement}

Soit $P$ un sous-groupe de $G$.
a) Pour que $P$ soit parabolique, il faut et il suffit qu’il existe une partie $X$ de $S$ telle que $P$ soit conjugué de $G_X$ (cf. n° 5 pour la définition de $G_X$).
b) Soient $X, X' \subset S$ et $g, g' \in G$ tels que $P = g G_X g^{-1} = g' G_{X'} g'^{-1}$. On a alors $X = X'$ et $g' g^{-1} \in P$.
L’assertion a) résulte du th. 3, b).
Sous les hypothèses de b), on a
$$
g^{-1} g' B g'^{-1} g \subset g^{-1} g' G_{X'} g'^{-1} g = G_X,
$$
et la prop. 3 montre que $g^{-1} g' \in G_X$. D’où $G_{X'} = G_X$ et $X' = X$ d’après le th. 3, b). Enfin, on a :
$$
g' g^{-1} = g . g^{-1} g' . g^{-1} \in g G_X g^{-1},
$$
d’où b).
Si le sous-groupe parabolique $P$ est conjugué de $G_X$, avec $X \subset S$, on dit que $X$ est le type de $P$.

#### Théorème 4 {#lie-iv-s2-thm-4 .statement}

(i) Soient $P_1$ et $P_2$ deux sous-groupes paraboliques de $G$ dont l’intersection est parabolique et soit $g \in G$ tel que $g P_1 g^{-1} \subset P_2$. Alors $g \in P_2$ et $P_1 \subset P_2$.
(ii) Deux sous-groupes paraboliques distincts dont l’intersection est parabolique ne sont pas conjugués.
(iii) Soient $Q_1$ et $Q_2$ deux sous-groupes paraboliques de $G$ contenus dans un sous-groupe $Q$ de $G$. Tout $g \in G$ tel que $g Q_1 g^{-1} = Q_2$ appartient à $Q$.
(iv) Tout sous-groupe parabolique est son propre normalisateur (*).
L’assertion (i) résulte des prop. 3 et 4, et entraîne (ii). Sous les hypothèses de (iii), on a $g Q_1 g^{-1} \subset Q$, d’où $g \in Q$ d’après (i). Enfin (iv) résulte de (iii) en prenant $Q_1 = Q_2 = Q$.

#### Proposition 5 {#lie-iv-s2-prop-5 .statement}

Soient $P_1$ et $P_2$ deux sous-groupes paraboliques de $G$. Alors $P_1 \cap P_2$ contient un conjugué de $T$.

(*) Si $H$ est un sous-groupe d’un groupe $G$, le normalisateur de $H$ dans $G$ est le sous-groupe $\mathcal{N}_G(H)$ formé des éléments $g$ de $G$ tels que $g H g^{-1} = H$. On dit que le sous-groupe $H'$ normalise $H$ si l’on a $H' \subset \mathcal{N}_G(H)$, auquel cas $H H' = H' H$ est un sous-groupe de $G$, dans lequel $H$ est distingué.

Quitte à transformer $P_1$ et $P_2$ par un automorphisme intérieur de $G$, on peut supposer que $B \subset P_1$. Soit $g \in G$ tel que $gB g^{-1} \subset P_2$. D’après le th. 1, il existe $n \in N$ et $b, b' \in B$ tels que $g = b n b'$. Comme $T$ est distingué dans $N$, on a
$$
P_2 \supset g B g^{-1} = b n B n^{-1} b^{-1} \supset b n T n^{-1} b^{-1} = b T b^{-1}
$$
et
$$
P_1 \supset B \supset b T b^{-1}
$$
d’où la proposition.

### 7. Théorème de simplicité

#### Lemme 2 {#lie-iv-s2-lem-2 .statement}

Soit $H$ un sous-groupe distingué de $G$. Il existe une partie $X$ de $S$ telle que $B H = G_X$ et tout élément de $X$ commute à tout élément de $S - X$.

Puisque $B H$ est un sous-groupe de $G$ contenant $B$, il existe une unique partie $X$ de $S$ telle que $B H = G_X$ (th. 3).

Soient $s_1 \in X$ et $s_2 \in S - X$; soient $n_1$ et $n_2$ des représentants respectifs de $s_1$ et $s_2$ dans $N$. On a $n_1 \in G_X = B H$ et il existe $b \in B$ tel que $b n_1 \in H$. Comme $H$ est distingué dans $G$, l’élément $h = n_2 b n_1 n_2^{-1}$ de $G$ appartient à $H$. D’autre part
$$
h \in C(s_2) \cdot C(s_1) \cdot C(s_2).
$$
Si la longueur de $s_2 s_1 s_2$ est égale à 3, le cor. 1 du th. 2 entraîne
$$
C(s_2) \cdot C(s_1) \cdot C(s_2) = C(s_2 s_1 s_2),
$$
d’où $h \in H \cap C(s_2 s_1 s_2)$. Puisque $H \cap C(s_2 s_1 s_2)$ est non vide, on a $s_2 s_1 s_2 \in W_X$. Comme $(s_2, s_1, s_2)$ est une décomposition réduite, on en déduit $s_2 \in X$, contrairement à l’hypothèse ($\S 1$, no 8, cor. 1 de la prop. 7).

On a donc $l_S(s_2 s_1 s_2) \leq 2$; si $l_S(s_1 s_2) = 1$, on a $s_1 s_2 \in S$, donc $(s_1 s_2)^2 = 1$, $s_1 s_2 = s_2 s_1$. Si $l_S(s_1 s_2) = 2$ la propriété (E) du $\S 1$, no 5 entraîne alors $s_2 s_1 = s_1 s_2$, car $s_1 \neq s_2$. C.Q.F.D.

Dans le th. 5 ci-dessous interviendra la propriété suivante d’un groupe $U$:
(R) Pour tout sous-groupe distingué $V$ de $U$, distinct de $U$, le groupe des commutateurs (cf. Alg., chap. I, $\S 6$, no 8) de $U/V$ est distinct de $U/V$.

Tout groupe résoluble vérifie (R); en particulier tout groupe commutatif vérifie (R); il en est de même de tout groupe simple non commutatif. On peut montrer que le groupe symétrique $\mathfrak{S}_n$ vérifie (R) pour tout $n$ (cf. exerc. 29).

#### Théorème 5 {#lie-iv-s2-thm-5 .statement}

Soit $Z$ l’intersection des conjugués de $B$, soit $U$ un sous-groupe de $B$ et soit $G_1$ le sous-groupe engendré par les conjugués de $U$ dans $G$. On fait les hypothèses suivantes :
(1) $U$ est distingué dans $B$ et $B = U T$.
(2) $U$ possède la propriété (R).
(3) $G_1$ est égal à son groupe des commutateurs.
(4) Le système de Coxeter $(W, S)$ est irréductible (cf. $\S 1$, no 9).
Alors tout sous-groupe $H$ de $G$ normalisé par $G_1$ est contenu dans $Z$ ou contient $G_1$.

Montrons d’abord que $G = G_1 T$. Le groupe $G_1 T$ contient $B$, donc est son propre normalisateur (th. 4); comme $N$ normalise $G_1$ et $T$, il normalise aussi $G_1 T$, d’où $N \subset G_1 T$; puisque $G$ est engendré par $B$ et $N$, on a bien $G = G_1 T$.

Posons maintenant
$$
G' = G_1 H, \quad B' = B \cap G', \quad N' = N \cap G',
T' = T \cap G' = B' \cap N' \quad \text{et} \quad W' = N'/T'.
$$
On a $G = G'T$ puisque $G'$ contient $G_1$, d’où $N = N'T$. L’injection de $N'$ dans $N$ définit donc, par passage aux quotients, un isomorphisme $\alpha : W' \to W$. Soit $S' = \alpha^{-1}(S)$.

Montrons que $(G', B', N', S')$ est un système de Tits. Comme $G = BNB$ et $B = TU = UT$, on a $G = UNU$ et, puisque $U$ est un sous-groupe de $G'$, on en déduit $G' = UN'U$, d’où (T1) puisque $U \subset B'$. L’axiome (T2) est satisfait puisque $\alpha$ est un isomorphisme. Soit $w \in W$ et soit $w' = \alpha^{-1}(w)$ l’élément correspondant de $W'$. On a
$$
BwB = BwB' = Bw'B', \quad \text{puisque} \quad B = B'T.
$$
On en conclut que $G' \cap BwB = B'w'B'$, ou encore que l’injection de $G'$ dans $G$ définit par passage aux quotients une bijection de $B'\backslash G'/B'$ sur $B\backslash G/B$. L’axiome (T3) est alors immédiat. L’axiome (T4) résulte de $B = B'T$.

Le sous-groupe $H$ est distingué dans $G'$. D’après le lemme 2 appliqué à $(G', B', N', S')$, il existe une partie $X'$ de $S'$ telle que $B'H = G'_X$ et tout élément de $S' - X'$ commute à tout élément de $X'$. Vu l’hypothèse (4), deux cas seulement sont possibles :

a) $X' = \varnothing$, i.e. $B'H = B'$, et $H \subset B' \subset B$. Si $g \in G$, on a $g = g_1 t$, avec $g_1 \in G_1, t \in T$ et $H \subset g_1 Bg_1^{-1}$ puisque $G_1$ normalise $H$. D’où $H \subset gBg^{-1}$; comme $Z$ est l’intersection des $gBg^{-1}$, on a $H \subset Z$.

b) $X' = S'$, i.e. $B'H = G'$; comme $G = G'T$, on a
$$
G = B'HT = HB'T = HB.
$$
Comme $B$ normalise $U$, tout conjugué de $U$ est de la forme $hUh^{-1}$, avec $h \in H$. Un tel sous-groupe est contenu dans le groupe $UH$, d’où $G_1 \subset UH$, par définition de $G_1$. On a alors les isomorphismes
$$
U/(U \cap H) \simeq UH/H = G_1 H/H \simeq G_1/(G_1 \cap H).
$$
D’après l’hypothèse (3), $G_1/(G_1 \cap H)$ est égal à son groupe des commutateurs. L’hypothèse (2) montre alors que le groupe $U/(U \cap H)$, isomorphe à $G_1/(G_1 \cap H)$, est réduit à l’élément neutre. D’où $G_1 \cap H = G_1$ et $G_1 \subset H$, ce qui achève la démonstration.

#### Corollaire {#lie-iv-s2-n7-cor-1 .statement}

Sous les hypothèses du th. 5, le groupe $G_1/(G_1 \cap Z)$ est simple non commutatif, ou réduit à l’élément neutre.

Le th. 5 montre que $G_1/(G_1 \cap Z)$ est simple ou réduit à l’élément neutre; d’autre part l’hypothèse (3) entraîne qu’il est égal à son groupe des commutateurs; d’où le corollaire.

#### Remarque 1 {#lie-iv-s2-n7-rem-1 .statement}

Les hypothèses (2), (3), (4) n’ont pas été utilisées pour démontrer que $(G', B', N', S')$ est un système de Tits.

#### Remarque 2 {#lie-iv-s2-n7-rem-2 .statement}

Supposons que $Z \cap U = \{1\}$. Comme $Z$ et $U$ sont distingués dans $B$, il en résulte que tout élément de $Z$ commute à tout élément de $U$, donc à tout élément de $G_1$. Vu le corollaire ci-dessus, il s’ensuit que $G_1 \cap Z$ est le centre de $G_1$.

#### Remarque 3 {#lie-iv-s2-n7-rem-3 .statement}

L’hypothèse (3) est entraînée par la condition suivante:
(3’) $U$ est engendré par les commutateurs $b^{-1}u^{-1}bu$, avec $u \in U$ et $b \in B \cap G_1$.

#### Exemple 1 {#lie-iv-s2-n7-exa-1 .statement}

Soient $k$ un corps, $n$ un entier $\geqslant 0$, $G = \mathbf{GL}(n, k)$, et soit $(G, B, N, S)$ le système de Tits décrit au no 2. Soit $U$ le groupe trigonal strict supérieur, i.e. le sous-groupe de $B$ formé des matrices dont les éléments diagonaux sont égaux à 1. La condition (1) du th. 5 se vérifie immédiatement; il en est de même de (2) puisque $U$ est résoluble; la condition (4) est vérifiée si $n \geqslant 2$. On peut prouver (cf. Alg., Chap. II, 3e éd., § 10, exerc. 13) que (3) est vérifiée si $n \geqslant 3$ ou si $n = 2$ et $\mathrm{Card}(k) \geqslant 4$. Sous ces conditions, on en conclut que $G_1/(G_1 \cap Z)$ est simple et que $G_1 \cap Z$ est le centre de $G_1$ (cf. Remarque 2).

Lorsque $k$ est commutatif, on a $G_1 = \mathbf{SL}(n, k)$, cf. Alg., Chap. III, 3e éd., § 8, no 9.

#### Exemple 2 {#lie-iv-s2-n7-exa-2 .statement}

Soit $g$ une algèbre de Lie simple sur $\mathbf{C}$, et soit $G$ le groupe adjoint de $g$ (cf. chap. III). On peut montrer, en utilisant le théorème 5, que $G$ est simple non abélien.*

## EXERCICES {#lie-iv-s2-exercises}

See the [exercises for § 2](exercises/s2/).
