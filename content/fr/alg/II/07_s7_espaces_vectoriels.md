---
book: alg
book_title: Algebra
chapter: II
chapter_title: ALGÈBRE LINÉAIRE
section: 7
section_title: Espaces vectoriels
lang: fr
source: alg-i-iii-fr
book_pages: A II.95-A II.118
pdf_pages: 0272-0295, 0369-0375
extraction: ocr
subsections:
    - "no": 1
      title: Bases d’un espace vectoriel
      page: 95
      pdf_page: 272
    - "no": 2
      title: Dimension des espaces vectoriels
      page: 96
      pdf_page: 273
    - "no": 3
      title: Dimension et codimension d’un sous-espace d’un espace vectoriel
      page: 98
      pdf_page: 275
    - "no": 4
      title: Rang d’une application linéaire
      page: 101
      pdf_page: 278
    - "no": 5
      title: Dual d’un espace vectoriel
      page: 102
      pdf_page: 279
    - "no": 6
      title: Equations linéaires dans les espaces vectoriels
      page: 106
      pdf_page: 283
    - "no": 7
      title: Produit tensoriel d’espaces vectoriels
      page: 108
      pdf_page: 285
    - "no": 8
      title: Rang d’un élément d’un produit tensoriel
      page: 111
      pdf_page: 288
    - "no": 9
      title: Extension des scalaires d’un espace vectoriel
      page: 113
      pdf_page: 290
    - "no": 10
      title: Modules sur les anneaux intègres
      page: 114
      pdf_page: 291
statements: 90
exercises: 39
content_sha256: b11e71e8b09f4551ae55f53e4c42181148c8ecfc4b718389cf2007b5f3dd33b3
---

## § 7. ESPACES VECTORIELS.

### 1. Bases d’un espace vectoriel

#### Théorème 1 {#alg-ii-s7-thm-1 .statement}

*Tout espace vectoriel sur un corps $K$ est un $K$-module libre.*

Il faut prouver que tout espace vectoriel admet une *base*; cela va résulter du théorème plus précis suivant:

#### Théorème 2 {#alg-ii-s7-thm-2 .statement}

*Étant donnés un système générateur $S$ d’un espace vectoriel $E$ sur un corps $K$, et une partie libre $L$ de $E$ contenue dans $S$, il existe une base $B$ de $E$ telle que $L \subset B \subset S$.

Le th. 1 résultera de cet énoncé en prenant $L = \varnothing$.

Pour prouver le th. 2, notons que l’ensemble $\mathcal{L}$ des parties libres de $E$ contenues dans $S$, ordonné par inclusion, est *un ensemble inductif* (E, III, p. 20), en vertu de II, p. 26; il en est de même de l’ensemble $\mathfrak{M}$ des parties libres contenant $L$ et contenues dans $S$. En vertu du th. de Zorn, $\mathfrak{M}$ admet un élément maximal $B$, et il suffit de prouver que le sous-espace vectoriel de $E$ engendré par $B$ est égal à $E$. Cela résulte aussitôt de la définition de $B$ et du lemme suivant:

#### Lemme 1 {#alg-ii-s7-lem-1 .statement}

*Soit $(a_i)_{i \in I}$ une famille libre d’éléments de $E$; si $b \in E$ n’appartient pas au sous-espace $F$ engendré par $(a_i)$, la partie de $E$ formée des $a_i$ et de $b$ est libre.*

Supposons que l’on ait une relation $\mu b + \sum_i \lambda_i a_i = 0$ avec $\mu \in K$ et $\lambda_i \in K$ pour tout $i \in I$, la famille $(\lambda_i)$ ayant un support fini; si on avait $\mu \neq 0$, on en déduirait $b = -\sum_i (\mu^{-1}\lambda_i)a_i$, donc $b \in F$ contrairement à l’hypothèse; on doit donc avoir $\mu = 0$, et il reste la relation $\sum_i \lambda_i a_i = 0$, qui entraîne $\lambda_i = 0$ pour tout $i \in I$ par hypothèse; d’où le lemme.

#### Corollaire {#alg-ii-s7-n1-cor-1 .statement}

*Pour une partie B d’un espace vectoriel E, les propriétés suivantes sont équivalentes*:
a) *B est une base de E.*
b) *B est une partie libre maximale de E.*
c) *B est un système générateur minimal de E.*
Cela résulte aussitôt du th. 2.

#### Exemple {#alg-ii-s7-n1-exa-1 .statement}

Étant donné un anneau A et un *sous-corps* K de A, A est un espace vectoriel (à droite ou à gauche) sur K, et admet donc une base; en particulier, tout *surcorps* d’un corps K possède une base en tant qu’espace vectoriel à gauche (resp. à droite) sur K. \* C’est ainsi que le corps R des nombres réels admet une base (infinie) en tant qu’espace vectoriel sur le corps Q des nombres rationnels; une telle base de R est dite *base de Hamel.* \*

#### Remarque {#alg-ii-s7-n1-rem-1 .statement}

Pour qu’une famille $(a_i)_{i \in I}$ d’éléments d’un espace vectoriel E sur un corps K soit *libre*, il faut et il suffit que, pour tout $\kappa \in I$, $a_\kappa$ n’appartienne pas au sous-espace de E engendré par les $a_i$ d’indice $i \neq \kappa$. On sait en effet que cette condition est nécessaire dans tout module (II, p. 26, *Remarque* 1). Elle est suffisante en vertu du lemme 1, comme on le voit aussitôt en raisonnant par l’absurde et considérant une sous-famille liée minimale de $(a_i)$.

### 2. Dimension des espaces vectoriels

#### Théorème 3 {#alg-ii-s7-thm-3 .statement}

*Deux bases d’un même espace vectoriel E sur un corps K sont équipotentes*.

Remarquons d’abord que si E admet une base *infinie* B, il résulte de II, p. 30, cor. 2 que toute autre base de E est équipotente à B. On peut donc se limiter au cas où E possède une base finie de $n$ éléments. Remarquons que tout espace vectoriel *monogène* sur K, non réduit à 0, est un K-module *simple* (I, p. 36, déf. 7), car il est engendré par chacun de ses éléments $\neq 0$, en vertu de la relation $\mu a = (\mu \lambda)(\lambda^{-1}a)$ pour $\mu \in K, \lambda \in K$ et $\lambda \neq 0$. Cela étant, si $(a_i)_{1 \leq i \leq n}$ est une base de E, on a $E = \bigoplus_{i=1}^n Ka_i$ à un isomorphisme près, et les sous-espaces $E_k = \bigoplus_{i=1}^k Ka_i$ pour $0 \leq k \leq n$ forment une *suite de Jordan-Hölder* de E, $E_k/E_{k-1}$ étant isomorphe à $Ka_k$. Le th. 3 résulte donc dans ce cas du th. de Jordan-Hölder (I, p. 41, th. 6).

On peut donner une démonstration indépendante du th. de Jordan-Hölder, en montrant par récurrence sur $n$ que si E admet une base B de $n$ éléments, toute autre base B’ a *au plus* $n$ éléments. La proposition est évidente pour $n = 0$. Si $n \geq 1$, B’ n’est pas vide; soit donc $a \in B'$. En vertu du th. 2 (II, p. 95), il existe une partie C de B telle que $\{a\} \cup C$ soit une base de E et que $a \notin C$, puisque $\{a\} \cup B$ est évidemment un système générateur de E. Comme B est une base de E, on ne peut avoir C = B (II, p. 96, corollaire), donc C a au plus $n - 1$ éléments. Soient V le sous-espace engendré par C, V' le sous-espace engendré par B' - {a}; V et V' sont tous deux supplémentaires du sous-espace Ka de E, donc sont isomorphes (II, p. 20, prop. 13). Comme V admet une base ayant au plus $n - 1$ éléments, B' - {a} a au plus $n - 1$ éléments en vertu de l’hypothèse de récurrence, donc B' a au plus $n$ éléments.

#### Définition 1 {#alg-ii-s7-def-1 .statement}

On appelle dimension d’un espace vectoriel E sur un corps K et on note $\dim_K E$ ou [E: K] (ou simplement dim E) le cardinal d’une quelconque des bases de E. Si M est une partie de E, on appelle rang de M (sur K) et l’on note rg M ou $\mathrm{rg}_K M$ la dimension du sous-espace vectoriel de E engendré par M.

Dire que E est de dimension finie équivaut à dire que E est un K-module de longueur finie et on a $\dim_K E = \mathrm{long}_K E$.

#### Corollaire {#alg-ii-s7-n2-cor-1 .statement}

Pour toute partie M de E, le rang de M est au plus égal à dim E.

En effet, si V est le sous-espace vectoriel de E engendré par M, M contient une base B' de V (II, p. 95, th. 2) et comme B' est une partie libre de E, elle est contenue dans une base B de E (II, p. 95, th. 2); on a Card(B') $\leqslant$ Card(B), d’où le corollaire.

Les th. 2 et 3 entraînent aussitôt la proposition suivante:

#### Proposition 1 {#alg-ii-s7-prop-1 .statement}

(i) Pour qu’un espace vectoriel à gauche sur K soit de dimension finie n, il faut et il suffit qu’il soit isomorphe à $K_s^n$.

(ii) Pour que deux espaces vectoriels $K_s^m$ et $K_s^n$ soient isomorphes (m et n entiers $\geqslant 0$) il faut et il suffit que $m = n$.

(iii) Dans un espace vectoriel E de dimension finie n, tout système générateur a au moins n éléments; un système générateur de E ayant n éléments est une base de E.

(iv) Dans un espace vectoriel E de dimension finie n, toute partie libre a au plus n éléments; une partie libre ayant n éléments est une base de E.

#### Proposition 2 {#alg-ii-s7-prop-2 .statement}

Soit $(E_t)_{t \in I}$ une famille d’espaces vectoriels sur K. On a

$$
\dim_K (\bigoplus_{t \in I} E_t) = \sum_{t \in I} \dim_K E_t.
$$

En effet, si on identifie canoniquement les $E_t$ à des sous-espaces de $E = \bigoplus_{t \in I} E_t$, et si $B_t$ est une base de $E_t$ ($t \in I$), alors $B = \bigcup_{t \in I} B_t$ est une base de E (II, p. 26, prop. 19); d’où la relation (1) puisque les $B_t$ sont deux à deux disjoints.

Remarque 1). — On peut donner des exemples de modules admettant deux bases finies n’ayant pas le même nombre d’éléments (II, p. 181, exerc. 16 c)). Toutefois:

#### Proposition 3 {#alg-ii-s7-prop-3 .statement}

Soient A un anneau, tel qu’il existe un homomorphisme $\rho$ de A dans un corps D; alors, pour tout A-module libre E, deux bases quelconques de E sont équipotentes.

Considérons en effet l’espace vectoriel $\rho^*(E) = D \otimes_A E$ sur D obtenu par extension à D de l’anneau des scalaires (II, p. 82), et soit $\varphi : x \mapsto 1 \otimes x$ l’application canonique de E dans $\rho^*(E)$; si $(a_\lambda)$ est une base de E, $(\varphi(a_\lambda))$ est une base de $\rho^*(E)$ (II, p. 84, prop. 4); la proposition résulte donc du th. 3 (II, p. 96).

#### Corollaire {#alg-ii-s7-n2-cor-2 .statement}

Si $A$ est un anneau commutatif $\neq 0$, $E$ un $A$-module libre, deux bases quelconques de $E$ sont équipotentes.

En effet, il existe dans $A$ au moins un idéal maximal $m$ (I, p. 99, th. 1), et comme $A/m$ est un corps, les conditions de la prop. 3 sont remplies.

#### Remarque 2 {#alg-ii-s7-n2-rem-2 .statement}

Lorsqu’un $A$-module libre $E$ est tel que deux bases quelconques de $E$ soient équipotentes, le cardinal d’une base quelconque de $E$ sur $A$ s’appelle encore la *dimension* ou le *rang* de $E$ et se note $\dim_A E$ ou $\dim E$.

#### Remarque 3 {#alg-ii-s7-n2-rem-3 .statement}

Soit $A$ un anneau tel que deux bases quelconques d’un $A$-module libre soient équipotentes, et soit $K$ un sous-corps de $A$, de sorte que $A$ peut être considéré comme *espace vectoriel à gauche* sur $K$ par restriction des scalaires. Tout $A$-module libre $E$ peut de même être considéré comme espace vectoriel à gauche sur $K$, et il résulte alors de II, p. 31, prop. 25, que l’on a

$$
\dim_K E = \dim_A E \cdot \dim_K A_s.
$$

#### Remarque 4 {#alg-ii-s7-n2-rem-4 .statement}

Nous verrons au chapitre VIII des exemples d’anneaux vérifiant la conclusion de la prop. 3, mais non l’hypothèse.

### 3. Dimension et codimension d’un sous-espace d’un espace vectoriel

#### Proposition 4 {#alg-ii-s7-prop-4 .statement}

*Tout sous-espace* $F$ *d’un espace vectoriel* $E$ *est facteur direct de* $E$, *et on a*

$$
\dim F + \dim(E/F) = \dim E.
$$

Comme l’espace vectoriel quotient $E/F$ est un module libre, on sait (II, p. 27, prop. 21) que $F$ est facteur direct de $E$; la relation (3) est alors un cas particulier de II, p. 97, formule (1).

#### Corollaire 1 {#alg-ii-s7-prop-4-cor-1 .statement}

*Si* $E, F, G$ *sont des espaces vectoriels sur un corps* $K$, *toute suite exacte d’applications linéaires* $0 \to E \to F \to G \to 0$ *est scindée*.

C’est une autre façon d’exprimer la prop. 4 (II, p. 21).

#### Corollaire 2 {#alg-ii-s7-prop-4-cor-2 .statement}

*Soit* $(E_i)_{0 \leq i \leq n}$ *une famille finie d’espaces vectoriels sur un corps* $K$. *S’il existe une suite exacte d’applications linéaires*

$$
0 \longrightarrow E_0 \xrightarrow{u_0} E_1 \xrightarrow{u_1} E_2 \longrightarrow \cdots \longrightarrow E_{n-1} \xrightarrow{u_{n-1}} E_n \xrightarrow{u_n} 0
$$

*on a la relation*

$$
\sum_{2k+1 \leq n} \dim E_{2k+1} = \sum_{2k \leq n} \dim E_{2k}
$$

*ou, si tous les espaces* $E_i$ *sont de dimension finie*

$$
\sum_{i=0}^n (-1)^i \dim E_i = 0.
$$

Soit $I_k = \operatorname{Im} u_k = \operatorname{Ker} u_{k+1}$ pour $0 \leq k \leq n-1$; $I_{k+1}$ est par suite isomorphe à $E_{k+1}/I_k$, donc (II, p. 98, formule (3)) $\dim I_k + \dim I_{k+1} = \dim E_{k+1}$ pour $0 \leq k \leq n-2$ et en outre $\dim I_0 = \dim E_0$ et $I_{n-1} = E_n$, donc $\dim I_{n-1} = \dim E_n$. Remplaçant $\dim E_i$ par son expression en fonction des $\dim I_k$ dans les deux membres de (5), on trouve de chaque côté $\sum_{k=0}^{n-1} \dim I_k$, d’où le corollaire.

#### Corollaire 3 {#alg-ii-s7-prop-4-cor-3 .statement}

*Si M et N sont deux sous-espaces d’un espace vectoriel E, on a*
$$
\dim(M + N) + \dim(M \cap N) = \dim M + \dim N.
$$
Il suffit d’appliquer le cor. 2 à la suite exacte
$$
0 \to M \cap N \to M \oplus N \to M + N \to 0
$$
(II, p. 17, prop. 10) en tenant compte de ce que
$$
\dim(M \oplus N) = \dim M + \dim N
$$
(II, p. 97, prop. 2).

#### Corollaire 4 {#alg-ii-s7-prop-4-cor-4 .statement}

*Pour tout sous-espace F d’un espace vectoriel E, on a $\dim F \leq \dim E$; si E est de dimension finie, la relation $\dim F = \dim E$ est équivalente à $F = E$.*
La première assertion est évidente d’après (3); en outre si $\dim E$ est finie, la relation $\dim F = \dim E$ entraîne $\dim(E/F) = 0$ d’après (3) (II, p. 98), et un espace vectoriel de dimension 0 est réduit à 0.

#### Corollaire 5 {#alg-ii-s7-prop-4-cor-5 .statement}

*Si un espace vectoriel E est somme d’une famille $(F_i)$ de sous-espaces vectoriels, on a*
$$
\dim E \leq \sum_i \dim F_i.
$$
*Si en outre $\dim E$ est fini, les deux membres de (8) sont égaux si et seulement si E est somme directe de la famille $(F_i)$.*
L’inégalité (8) résulte de (3) et du fait que E est isomorphe à un quotient de $\bigoplus_i F_i$ (II, p. 16, formule (28)). La seconde assertion est un cas particulier de II, p. 23, cor. 5, car l’égalité des deux membres de (8) implique que $\dim F_i = 0$ sauf pour un nombre fini d’indices (E, III, p. 27, cor. 2 et p. 49, cor. 4).

#### Définition 2 {#alg-ii-s7-def-2 .statement}

*Étant donné un espace vectoriel E, on appelle codimension (par rapport à E) d’un sous-espace F de E, et on note $\operatorname{codim}_E F$, ou simplement $\operatorname{codim} F$, la dimension de E/F (égale à celle d’un supplémentaire quelconque de F dans E).*
La relation (3) s’écrit donc encore
$$
\dim F + \operatorname{codim} F = \dim E.
$$

#### Proposition 5 {#alg-ii-s7-prop-5 .statement}

*Soient F, F' deux sous-espaces d’un espace vectoriel E, tels que $F \subset F'$. On a alors $\operatorname{codim}_E F' \leq \operatorname{codim}_E F \leq \dim E$. Si $\operatorname{codim}_E F$ est finie, la relation $\operatorname{codim}_E F' = \operatorname{codim}_E F$ entraîne $F = F'$.*

L’inégalité codim$_E$ F $\leqslant$ dim E est évidente en vertu de (9), et si dim E est finie la relation codim$_E$ F = dim E entraîne dim F = 0, donc F = {0}. Le reste de la proposition découle de là, car on a codim$_E$ F' = codim$_{E/F}$ (F'/F), puisque E/F' est canoniquement isomorphe à (E/F)/(F'/F) (I, p. 39, th. 4).

#### Proposition 6 {#alg-ii-s7-prop-6 .statement}

*Si M et N sont deux sous-espaces d’un espace vectoriel E, on a*
$$
\text{codim}(M + N) + \text{codim}(M \cap N) = \text{codim } M + \text{codim } N.
$$
(10)
Il suffit d’appliquer le cor. 2 de II, p. 98 à la suite exacte
$$
0 \to E/(M \cap N) \to (E/M) \oplus (E/N) \to E/(M + N) \to 0
$$
(II, p. 17, prop. 10) en tenant compte de II, p. 97, prop. 2.

On notera que si E est de dimension finie, (10) est conséquence de (7) et (9) (II, p. 99).

#### Proposition 7 {#alg-ii-s7-prop-7 .statement}

*Si $(F_i)$ est une famille finie de sous-espaces d’un espace vectoriel E, on a* $\text{codim}(\bigcap_i F_i) \leqslant \sum_i \text{codim } F_i$.

En effet, si $F = \bigcap_i F_i$, E/F est isomorphe à un sous-espace de la somme directe des E/F$_i$ (II, p. 15, formule (27)).

On donne souvent aux sous-espaces vectoriels de dimension 1 (resp. de dimension 2) d’un espace vectoriel E le nom de *droites passant par* 0 (resp. *plans passant par* 0) (ou simplement *droites* (resp. *plans*)) s’il n’en résulte pas de confusion (cf. II, p. 129), par analogie avec le langage de la Géométrie classique; on dit qu’un sous-espace de E est un *hyperplan passant par* 0 (ou simplement un *hyperplan*) s’il est de codimension 1. On peut encore définir les hyperplans comme les éléments *maximaux* de l’ensemble $\mathcal{S}$ des sous-espaces vectoriels de E *distincts de* E, ordonné par inclusion. En effet, il y a correspondance biunivoque entre les sous-espaces de E contenant un sous-espace H et les sous-espaces de E/H (I, p. 39, th. 4); si E est de dimension $\geqslant 1$, $\mathcal{S}$ est non vide, et dire que H est maximal dans $\mathcal{S}$ signifie que E/H ne contient aucun sous-espace distinct de {0} et de E/H, ce qui entraîne que E/H est engendré par un quelconque de ses éléments $\neq 0$, autrement dit est de dimension 1.

Dans un espace vectoriel de dimension finie $n \geqslant 1$, les hyperplans sont les sous-espaces *de dimension* $n - 1$, en vertu de II, p. 98, formule (3).

#### Proposition 8 {#alg-ii-s7-prop-8 .statement}

*Dans un espace vectoriel E sur un corps K, tout sous-espace vectoriel F est l’intersection des hyperplans qui le contiennent*.

Il suffit de montrer que pour tout $x \notin F$, il existe un hyperplan H contenant F et ne contenant pas x. On a par hypothèse $F \cap Kx = \{0\}$, donc la somme M de F et de Kx est directe. Soit N un supplémentaire de M dans E; E est alors somme directe de $H = F + N$ et de $Kx$, et H est donc un hyperplan répondant à la question.

#### Remarque {#alg-ii-s7-n3-rem-1 .statement}

La plupart des propriétés démontrées dans ce n° pour les sous-espaces d’un espace vectoriel ne subsistent plus pour les sous-modules d’un A-module libre dont la dimension (II, p. 98, Remarque 2) est définie. *Par exemple, un idéal d’un anneau commutatif n’admet pas nécessairement de base, car il y a des anneaux intègres A dans lesquels certains idéaux sont non principaux (VII, § 1, n°1) et deux éléments quelconques d’un tel anneau sont linéairement dépendants (II, p. 26, Remarque 1).* Un sous-module d’un A-module libre E peut être libre, distinct de E et avoir même dimension que E, comme le montrent les idéaux principaux dans un anneau intègre A; le même exemple prouve en outre qu’un sous-module libre d’un A-module libre n’admet pas nécessairement de supplémentaire.

### 4. Rang d’une application linéaire

#### Définition 3 {#alg-ii-s7-def-3 .statement}

Soient E, F deux espaces vectoriels sur un corps K. Pour toute application linéaire u de E dans F, on appelle rang de u et on note rg(u) la dimension du sous-espace u(E) de F.

Si N = Ker(u), E/N est isomorphe à u(E), d’où la relation
$$
\text{rg}(u) = \operatorname{codim}_E(\operatorname{Ker}(u))
$$
et par suite
$$
\text{rg}(u) + \dim(\operatorname{Ker}(u)) = \dim E.
$$
En outre, d’après II, p. 98, formule (3)
$$
\text{rg}(u) + \dim(\operatorname{Coker}(u)) = \dim F.
$$

#### Proposition 9 {#alg-ii-s7-prop-9 .statement}

Soient E, F deux espaces vectoriels sur un corps K, u : E → F une application linéaire.
(i) On a \text{rg}(u) \leq \inf(\dim E, \dim F).
(ii) Supposons E de dimension finie; pour que \text{rg}(u) = \dim E, il faut et il suffit que u soit injective.
(iii) Supposons F de dimension finie; pour que \text{rg}(u) = \dim F, il faut et il suffit que u soit surjective.

Cela résulte aussitôt des relations (12) et (13).

#### Corollaire {#alg-ii-s7-n4-cor-1 .statement}

Soient E un espace vectoriel de dimension finie n, u un endomorphisme de E. Les propriétés suivantes sont équivalentes:
a) u est bijectif;
b) u est injectif;
c) u est surjectif;
d) u est inversible à droite;
e) u est inversible à gauche;
f) u est de rang n.

Si E est un espace vectoriel de dimension infinie, il y a des endomorphismes injectifs (resp. surjectifs) de E qui ne sont pas bijectifs (II, p. 194, exerc. 9).

Soient K, K' deux corps, $\sigma : K \to K'$ un isomorphisme de K sur K', E un K-espace vectoriel, E' un K'-espace vectoriel, $u : E \to E'$ une application semi-linéaire relative à $\sigma$ (II, p. 32); on appelle encore rang de $u$ la dimension du sous-espace $u(E)$ de E'. C’est aussi le rang de $u$ considéré comme application linéaire de E dans $\sigma_*(E')$, car toute base de $u(E)$ est aussi une base de $\sigma_*(u(E))$.

### 5. Dual d’un espace vectoriel

#### Théorème 4 {#alg-ii-s7-thm-4 .statement}

La dimension du dual $E^*$ d’un espace vectoriel E est au moins égale à la dimension de E. Pour que $E^*$ soit de dimension finie, il faut et il suffit que E le soit, et on a alors $\dim E^* = \dim E$.

Si K est le corps des scalaires de E, E est isomorphe à un espace $K_s^{(I)}$ et par suite $E^*$ est isomorphe à $K_d^{I}$ (II, p. 44, prop. 10). Comme $K_d^{(I)}$ est un sous-espace de $K_d^{I}$, on a $\dim E = \mathrm{Card}(I) \leq \dim E^*$ (II, p. 99, cor. 4); en outre, si I est fini, on a $K_d^{I} = K_d^{(I)}$ (cf. II, p. 192, exerc. 3d)).

#### Corollaire {#alg-ii-s7-n5-cor-1 .statement}

Pour un espace vectoriel E, les relations $E = \{0\}$ et $E^* = \{0\}$ sont équivalentes.

#### Théorème 5 {#alg-ii-s7-thm-5 .statement}

Étant données deux suites exactes d’espaces vectoriels (sur un même corps K) et d’applications linéaires

$$
\begin{array}{c}
0 \to E' \to E \to E'' \to 0 \\
0 \to F' \to F \to F'' \to 0
\end{array}
$$

et deux espaces vectoriels G, H sur K, les suites correspondantes

$$
\begin{array}{c}
0 \to \mathrm{Hom}(E'', G) \to \mathrm{Hom}(E, G) \to \mathrm{Hom}(E', G) \to 0 \\
0 \to \mathrm{Hom}(H, F') \to \mathrm{Hom}(H, F) \to \mathrm{Hom}(H, F'') \to 0
\end{array}
$$

sont exactes et scindées.

Cela résulte de ce que tout sous-espace vectoriel est facteur direct (II, p. 98, prop. 4) et de II, p. 37, prop. 1 et p. 38, prop. 2.

#### Corollaire {#alg-ii-s7-n5-cor-2 .statement}

Pour toute suite exacte

$$
0 \longrightarrow E' \xrightarrow{u} E \xrightarrow{v} E'' \longrightarrow 0
$$

d’espaces vectoriels sur un même corps K et d’applications linéaires, la suite

$$
0 \longrightarrow E''* \xrightarrow{t_v} E^* \xrightarrow{t_u} E'* \longrightarrow 0
$$

est exacte et scindée.

On en déduit en particulier que pour tout sous-espace vectoriel M de E, l’homomorphisme canonique $E^*/M' \to M^*$, où $M'$ est le sous-espace de $E^*$ orthogonal à M (II, p. 42), est bijectif.

#### Théorème 6 {#alg-ii-s7-thm-6 .statement}

Pour tout espace vectoriel E sur un corps K, l’application canonique $c_E : E \to E^{**}$ (II, p. 46) est injective; pour qu’elle soit bijective, il faut et il suffit que E soit de dimension finie.

La première assertion et le fait que si E est de dimension finie $c_E$ est bijective, sont des cas particuliers de II, p. 47, prop. 14. Supposons E de dimension infinie, de sorte que l’on peut supposer que $E = K_s^{(L)}$, où L est un ensemble infini, et par suite $E^* = K_d^L$. Soit $(e_\lambda)_{\lambda \in L}$ la base canonique de E, et soit $(e^*_\lambda)_{\lambda \in L}$ la famille correspondante des formes coordonnées dans $E^*$ (II, p. 45); le sous-espace vectoriel de $E^*$ engendré par les $e^*_\lambda$ n’est autre que la somme directe $F' = K_d^{(L)}$ et l’hypothèse que L est infini entraîne $F' \neq E^*$. Il existe donc un hyperplan $H'$ de $E^*$ contenant $F'$ (II, p. 100, prop. 8), et comme $E^*/H'$ n’est pas réduit à 0, il en est de même de son dual (II, p. 102, cor. du. th. 4), qui s’identifie à l’orthogonal $H''$ de $H'$ dans $E^{**}$ (II, p. 44, corollaire). Mais $H'' \cap c_E(E)$ est contenu dans l’image par $c_E$ de l’orthogonal de $F'$ dans E, qui par définition est réduit à 0; on ne peut donc avoir $c_E(E) = E^{**}$.

On identifiera d’ordinaire E au sous-espace de $E^{**}$ image de $c_E$.

Soient E, F deux espaces vectoriels sur un corps K, $u : E \to F$ une application linéaire. Nous allons définir des isomorphismes canoniques:

1° Du dual de $\operatorname{Im}(u) = u(E)$ sur $\operatorname{Im}(t^u) = t^u(F^*)$.
2° Du dual de $\operatorname{Ker}(u) = \overline{u}^{-1}(0)$ sur $\operatorname{Coker}(t^u) = E^*/t^u(F^*)$.
3° Du dual de $\operatorname{Coker}(u) = F/u(E)$ sur $\operatorname{Ker}(t^u) = t^u^{-1}(0)$.

Posons en effet $I = \operatorname{Im}(u)$, $N = \operatorname{Ker}(u)$, $C = \operatorname{Coker}(u)$; des suites exactes

$$
\begin{array}{ccccccccc}
0 & \longrightarrow & N & \longrightarrow & E & \overset{p}{\longrightarrow} & I & \longrightarrow & 0, \\
0 & \longrightarrow & I & \overset{j}{\longrightarrow} & F & \longrightarrow & C & \longrightarrow & 0
\end{array}
$$

on déduit, par transposition (II, p. 102, cor. du th. 5), les suites exactes

$$
\begin{array}{ccccccccc}
0 & \longrightarrow & I^* & \overset{t^p}{\longrightarrow} & E^* & \longrightarrow & N^* & \longrightarrow & 0, \\
0 & \longrightarrow & C^* & \longrightarrow & F^* & \overset{t^j}{\longrightarrow} & I^* & \longrightarrow & 0.
\end{array}
$$

En outre, comme $u = j \circ p$, on a $t^u = t^p \circ t^j$; les suites exactes (15) définissent donc des isomorphismes canoniques de $C^*$ sur $\operatorname{Ker}(t^u)$, de $I^*$ sur $\operatorname{Im}(t^u)$ et de $N^*$ sur $\operatorname{Coker}(t^u)$, puisque $t^p$ est injective et $t^j$ surjective. De façon plus précise, soient $y \in \operatorname{Im}(u)$, $z \in \operatorname{Ker}(u)$, $t \in \operatorname{Coker}(u)$, $y' \in \operatorname{Im}(t^u)$, $z' \in \operatorname{Coker}(t^u)$, $t' \in \operatorname{Ker}(t^u)$; lorsqu’on identifie canoniquement $y'$, $z'$, $t'$ à des formes linéaires sur $\operatorname{Im}(u)$, $\operatorname{Ker}(u)$ et $\operatorname{Coker}(u)$ respectivement, on a

$$
\begin{align*}
(16) \quad \langle y, y' \rangle &= \langle x, y' \rangle & \text{pour tout } x \in E \text{ tel que } u(x) = y; \\
(17) \quad \langle z, z' \rangle &= \langle z, x^* \rangle & \text{pour tout } x^* \in E^* \text{ dont la classe mod. } t^u(F^*) \text{ est égale à } z'; \\
(18) \quad \langle t, t' \rangle &= \langle s, t' \rangle & \text{pour tout } s \in F \text{ dont la classe mod. } u(E) \text{ est égale à } t.
\end{align*}
$$

On déduit en particulier de ces résultats:

#### Proposition 10 {#alg-ii-s7-prop-10 .statement}

Soient E, F deux espaces vectoriels sur un même corps K, u : E → F une application linéaire.

(i) Pour que u soit injective (resp. surjective), il faut et il suffit que $t^u$ soit surjective (resp. injective).

(ii) On a $\mathrm{rg}(u) \leq \mathrm{rg}(t^u)$, et $\mathrm{rg}(u) = \mathrm{rg}(t^u)$ si $\mathrm{rg}(u)$ est fini.

La seconde assertion résulte en effet de ce qui précède et du th. 4 (II, p. 102).

#### Théorème 7 {#alg-ii-s7-thm-7 .statement}

Soient E un espace vectoriel sur un corps K, F un sous-espace de E, F' l’orthogonal de F dans E*.

(i) On a $\dim F' \geq \mathrm{codim}_E F$; pour que $\dim F'$ soit fini, il faut et il suffit que $\mathrm{codim}_E F$ soit fini, et alors on a $\dim F' = \mathrm{codim}_E F$.

(ii) L’orthogonal de F' dans E est égal à F.

(iii) Tout sous-espace G' de E* de dimension finie est l’orthogonal d’un sous-espace de E, nécessairement égal à l’orthogonal de G' dans E et de codimension finie.

(i) On sait que F' est isomorphe au dual (E/F)* (II, p. 44, corollaire), donc l’assertion résulte de II, p. 102, th. 4, puisque $\dim(E/F) = \mathrm{codim}_E F$ par définition.

(ii) Soit $F_1$ l’orthogonal de F' dans E; il est clair que $F \subset F_1$ et que l’orthogonal $F'_1$ de $F_1$ est égal à $F'$ (II, p. 42); l’application linéaire canonique $(E/F_1)^* \to (E/F)^*$, transposée de $E/F \to E/F_1$, est donc bijective (II, p. 45, corollaire); il résulte alors de la prop. 10 que l’application canonique $E/F \to E/F_1$ est bijective, ce qui entraîne $F_1 = F$.

(iii) Soient G' un sous-espace de E* de dimension finie $p$ et soit F son orthogonal dans E; on a alors $\mathrm{codim}_E F \leq \dim G'$. En effet, si $(a_i^*)_{1 \leq i \leq p}$ est une base de G', F est le noyau de l’application linéaire $x \mapsto (\langle x, a_i^* \rangle)$ de E dans $K_s^p$, dont le rang est au plus $p$ (II, p. 101, prop. 9), d’où la conclusion (II, p. 101). Soit alors F' l’orthogonal de F dans E*; il résulte de (i) que $\dim F' \leq \dim G'$; mais d’autre part on a évidemment $G' \subset F'$, d’où $F' = G'$ (II, p. 99, cor. 4).

#### Remarque {#alg-ii-s7-n5-rem-1 .statement}

Un sous-espace G' de E* de dimension infinie n’est pas nécessairement l’orthogonal d’un sous-espace de E, autrement dit, si F est l’orthogonal de G' dans E, l’orthogonal F' de F dans E* peut être distinct de G' (II, p. 196, exerc. 20b))¹.

#### Corollaire 1 {#alg-ii-s7-thm-7-cor-1 .statement}

Soit $(x_i^*)_{1 \leq i \leq p}$ une suite finie de formes linéaires sur E, et soit F le sous-espace de E formé des x tels que

$$
\langle x, x_i^* \rangle = 0 \quad \text{pour } 1 \leq i \leq p.
$$

Alors $\mathrm{codim}_E F$ est égal au rang de l’ensemble des $x_i^*$, et toute forme linéaire sur E qui

¹ En munissant E et E* de topologies convenables, et en ne considérant dans E et E* que des sous-espaces fermés pour ces topologies, on peut rétablir une symétrie parfaite entre les propriétés de E et E* lorsque E est de dimension infinie (cf. EVT, II, § 6).

est nulle dans F est combinaison linéaire des $x_i^*$. On a $\operatorname{codim}_E F \leq p$, et pour que $\operatorname{codim}_E F = p$, il faut et il suffit que les $x_i^*$ soient linéairement indépendantes.

En effet, l’ensemble $G'$ des combinaisons linéaires des $x_i^*$ est un sous-espace de $E^*$ et $F$ est l’orthogonal de $G'$ dans $E$, donc $\operatorname{codim}_E F = \dim G'$ en vertu du th. 7; on a en outre $\dim G' \leq p$, et la relation $\dim G' = p$ signifie que $(x_i^*)$ est un système libre (II, p. 97, prop. 1); d’où le corollaire.

#### Corollaire 2 {#alg-ii-s7-thm-7-cor-2 .statement}

(i) Soit $(x_i^*)_{1 \leq i \leq p}$ une suite finie de formes linéaires sur $E$. Pour que $(x_i^*)$ soit un système libre, il faut et il suffit qu’il existe une suite $(x_i)_{1 \leq i \leq p}$ d’éléments de $E$ tels que $\langle x_i, x_j^* \rangle = \delta_{ij}$ (indice de Kronecker).

(ii) Soit $(x_i)_{1 \leq i \leq p}$ une suite finie d’éléments de $E$. Pour que $(x_i)$ soit un système libre, il faut et il suffit qu’il existe une suite $(x_i^*)_{1 \leq i \leq p}$ de formes linéaires sur $E$ telles que $\langle x_i, x_j^* \rangle = \delta_{ij}$.

Il est clair que (ii) se déduit de (i), en considérant $E$ comme identifié à un sous-espace de $E^{**}$ au moyen de $c_E$ (II, p. 103, th. 6). Soient $G'$ le sous-espace de $E^*$ engendré par les $x_i^*$, $F$ son orthogonal dans $E$; $E/F$ et $G'$ peuvent être chacun identifié canoniquement au dual de l’autre; si la famille $(x_i^*)$ est libre, il y a dans $E/F$ une base $(\dot{x}_i)$ duale de $(x_i^*)$ et tout système $(x_i)$ de représentants des classes $\dot{x}_i$ répond à la question. Inversement l’existence du système $(x_i)$ tel que $\langle x_i, x_j^* \rangle = \delta_{ij}$ entraîne que pour tout $i$ le sous-espace de $E^*$ orthogonal à $K.x_i$ contient les $x_j^*$ d’indice $j \neq i$ mais ne contient pas $x_i$, donc le système $(x_i^*)_{1 \leq i \leq p}$ est libre.

#### Corollaire 3 {#alg-ii-s7-thm-7-cor-3 .statement}

Soient $S$ un ensemble, $V$ un sous-espace vectoriel du $K$-espace vectoriel à droite $K_d^S$ des applications de $S$ dans $K$. Pour que $\dim V \geq p$ (où $p$ est un entier), il faut et il suffit qu’il existe $p$ éléments $s_i$ de $S$ et $p$ éléments $f_i$ de $V$ ($1 \leq i \leq p$) tels que l’on ait $f_i(s_j) = \delta_{ij}$.

L’espace $K_d^S$ est canoniquement identifié au dual de $E = K_s^{(S)}$, et on a $f(s) = \langle e_s, f \rangle$ pour $s \in S$ et $f \in K_d^S$, $(e_s)_{s \in S}$ étant la base canonique de $E$. Le cor. 2 montre donc que la condition est suffisante. Inversement, supposons que $\dim V \geq p$, de sorte qu’il existe un sous-espace $G'$ de $V$ de dimension $p$; soit $F$ l’orthogonal de $G'$ dans $E$, de sorte que $\dim(E/F) = p$. Il résulte de II, p. 95, th. 2 qu’il existe $p$ éléments $s_i \in S$ tels que les $e_{s_i}$ ($1 \leq i \leq p$) forment une base d’un supplémentaire de $F$ dans $E$ (en appliquant le th. 2 (II, p. 95) à une partie libre engendrant $F$ et au système générateur réunion de cette partie libre et de la base canonique de $E$); on prendra alors pour les $f_i$ les éléments d’une base de $G'$, duale de la base de $E/F$ formée des classes des $e_{s_i}$ mod. $F$.

#### Corollaire 4 {#alg-ii-s7-thm-7-cor-4 .statement}

Soient $E$ un espace vectoriel, $M, N$ deux sous-espaces de $E$, de codimensions finies; si $M', N'$ sont les orthogonaux de $M$ et $N$ dans $E^*$, l’orthogonal de $M \cap N$ dans $E^*$ est $M' + N'$.

En effet, comme $M$ (resp. $N$) est l’orthogonal de $M'$ (resp. $N'$) dans $E$ (II, p. 104, th. 7), $M \cap N$ est l’orthogonal de $M' + N'$ dans $E$, donc $M' + N'$ est l’orthogonal de $M \cap N$ dans $E^*$ (II, p. 104, th. 7, (iii)).

#### Corollaire 5 {#alg-ii-s7-thm-7-cor-5 .statement}

Soit E un espace vectoriel de dimension finie n. Pour tout sous-espace F de E, de dimension p, l’orthogonal F’ de F dans E* est de dimension n − p. Pour tout sous-espace G’ de E*, de dimension q, l’orthogonal G de G’ dans E est de dimension n − q, et G’ est l’orthogonal de G dans E*.

Le th. 7 donne une autre caractérisation des hyperplans dans E:

#### Proposition 11 {#alg-ii-s7-prop-11 .statement}

Pour tout hyperplan H dans un espace vectoriel E, il existe une forme linéaire x_0^* sur E telle que H = x_0^{*-1}(0). Étant donnée une telle forme x_0^*, pour qu’une forme linéaire x* sur E soit telle que H = x^{*-1}(0), il faut et il suffit que x* = x_0^*\alpha, où α est un scalaire ≠ 0. Réciproquement, pour toute forme linéaire x* ≠ 0 sur E, le sous-espace x^{*-1}(0) est un hyperplan de E.

Cet énoncé ne fait que traduire le th. 7 de II, p. 104 pour les sous-espaces de E de codimension 1 et les sous-espaces de E* de dimension 1.

Si H est un hyperplan et x_0^* une forme linéaire telle que H = x_0^{*-1}(0), on dit que la relation

$$
\langle x, x_0^* \rangle = 0
$$

qui caractérise les éléments x ∈ H, est une équation de H.

Plus généralement, si (x_i^*) est une famille de formes linéaires sur E et si F désigne le sous-espace vectoriel intersection des hyperplans x_i^{*-1}(0), la relation « quel que soit i, ⟨x, x_i^*⟩ = 0 » caractérise les éléments x de F; on dit que les relations

$$
\langle x, x_i^* \rangle = 0 \quad \text{pour tout } i
$$

forment un système d’équations du sous-espace F. Le th. 7, (ii) (II, p. 104) exprime que tout sous-espace vectoriel de E peut être défini par un système d’équations.

Le th. 7, (i) et (ii), (II, p. 104) prouve en outre qu’un sous-espace F de codimension finie p peut être défini par un système de p équations

(19)
$$
\langle x, x_i^* \rangle = 0, \quad 1 \leq i \leq p,
$$

où les formes x_i^* sont linéairement indépendantes. Inversement, le cor. 1 de II, p. 104 montre qu’un sous-espace F défini par un système de p équations (19) est de codimension $\leq p$, et qu’il est de codimension p si et seulement si les x_i^* sont linéairement indépendantes; il revient au même de dire que F ne peut être défini par un système formé d’au plus $p - 1$ des équations (19).

### 6. Equations linéaires dans les espaces vectoriels

#### Proposition 12 {#alg-ii-s7-prop-12 .statement}

Soient E, F, deux espaces vectoriels sur un corps K, u : E → F une application linéaire. Pour que l’équation linéaire

(20)
$$
u(x) = y_0
$$

ait au moins une solution $x \in E$, il faut et il suffit que $y_0$ soit orthogonal au noyau de l’application transposée $^t u$.

En effet, l’orthogonal de $u(E)$ dans $F^*$ est $^t u^{-1}(0)$ (II, p. 43, corollaire), et l’orthogonal de $^t u^{-1}(0)$ dans $F$ est donc $u(E)$ (II, p. 104, th. 7 (ii)).

Nous allons obtenir un critère plus maniable pour les systèmes d’équations linéaires scalaires

$$(21)$$
$$
\langle x, x_i^* \rangle = \eta_i \quad (\iota \in I)
$$

où l’inconnue $x$ prend ses valeurs dans un espace vectoriel $E$ sur un corps $K$, les $x_i^*$ sont des formes linéaires sur $E$, et les seconds membres $\eta_i$ des éléments de $K$.

Si on considère une base $(a_\lambda)_{\lambda \in L}$ de $E$, le système (21) est équivalent au système d’équations

$$(22)$$
$$
\sum_{\lambda \in L} \xi_\lambda \langle a_\lambda, x_i^* \rangle = \eta_i \quad (\iota \in I)
$$

avec $x = \sum_{\lambda \in L} \xi_\lambda a_\lambda$, les solutions de (22) devant être des familles $(\xi_\lambda)$ d’éléments de $K$ à support fini.

#### Définition 4 {#alg-ii-s7-def-4 .statement}

On appelle rang du système (21) la dimension du sous-espace de $E^*$ engendré par la famille $(x_i^*)$.

#### Proposition 13 {#alg-ii-s7-prop-13 .statement}

Pour que le système (21) soit de rang fini $r$, il faut et il suffit que l’application linéaire $u : x \mapsto (\langle x, x_i^* \rangle)$ de $E$ dans $K_s^I$ soit de rang $r$.

En effet, si $F'$ est le sous-espace de $E^*$ engendré par les $x_i^*$, le noyau de $u$ est l’orthogonal $F$ de $F'$ dans $E$; si $F'$ est de dimension $r$, $F$ est de codimension $r$ et réciproquement (II, p. 104, th. 7), et on a $\mathrm{rg}(u) = \mathrm{codim}_E F$ (II, p. 101, formule (11)).

#### Théorème 8 {#alg-ii-s7-thm-8 .statement}

Soit

$$(21)$$
$$
\langle x, x_i^* \rangle = \eta_i \quad (\iota \in I)
$$

un système d’équations linéaires scalaires dans un espace vectoriel $E$ sur un corps $K$. Pour que ce système ait au moins une solution, il est nécessaire que pour toute famille $(\rho_i)$ de scalaires, de support fini, telle que $\sum_i x_i^* \rho_i = 0$, on ait $\sum_i \eta_i \rho_i = 0$. Si le rang du système (21) est fini, cette condition est aussi suffisante.

La condition est évidemment nécessaire. Elle exprime que, si $F'$ est le sous-espace de $E^*$ engendré par la famille $(x_i^*)$, il existe une application linéaire $f : F' \to K_d$, telle que $f(x_i^*) = \eta_i$ pour tout $\iota \in I$. Si $F'$ est de dimension finie $r$, $F'$ est l’orthogonal d’un sous-espace $F$ de $E$, de codimension $r$ (II, p. 104, th. 7), et $F'$ s’identifie au dual de $E/F$ (II, p. 44, corollaire); $f$ est donc un élément du bidual $(E/F)^{**}$. Comme $E/F$ est de dimension finie, il existe un élément $y \in E/F$ et un seul tel que $f(x^*) = \langle y, x^* \rangle$ pour tout $x^* \in F'$ (II, p. 103, th. 6). Les solutions de (21) sont alors les $x \in E$ dont $y$ est l’image canonique dans $E/F$.

#### Remarque {#alg-ii-s7-n6-rem-1 .statement}

Lorsque le rang du système (21) est infini, la condition du th. 8 n’est plus suffisante. Par exemple, supposons que les $x_i^*$ soient les formes coordonnées sur l’espace $E = K_s^{(I)}$, I étant infini (II, p. 45); comme les $x_i^*$ sont linéairement indépendantes, la condition du th. 8 est vérifiée par toute famille $(\eta_t)$, mais le système (21) n’a alors de solution que si la famille $(\eta_t)$ a un support fini.

Un système (21) est toujours de rang fini s’il n’a qu’un nombre fini d’équations, et son rang est alors au plus égal au nombre d’équations (II, p. 97, prop. 1). De même, si E est de dimension finie $n$ (ce qui, pour un système (22), correspond au cas où il n’y a qu’un nombre fini $n$ d’inconnues), son dual $E^*$ est de dimension $n$, donc le rang du système (21) est au plus égal à $n$ (II, p. 99, cor. 4). On déduit de là:

#### Corollaire 1 {#alg-ii-s7-thm-8-cor-1 .statement}

Un système d’équations linéaires scalaires dans un espace vectoriel, formé d’un nombre fini d’équations dont les premiers membres sont des formes linéairement indépendantes, admet toujours des solutions.

#### Corollaire 2 {#alg-ii-s7-thm-8-cor-2 .statement}

Pour qu’un système homogène (22) d’équations à $n$ inconnues, à coefficients dans un corps $K$, admette des solutions non banales formées d’éléments de $K$, il faut et il suffit que son rang soit $< n$.

Il en sera toujours ainsi si les équations sont en nombre fini $< n$.

#### Corollaire 3 {#alg-ii-s7-thm-8-cor-3 .statement}

Pour qu’un système linéaire (22) à coefficients et seconds membres dans un corps $K$, formé de $n$ équations à $n$ inconnues, ait une solution et une seule formée d’éléments de $K$, il faut et il suffit que le système homogène associé n’ait aucune solution non banale (ou, ce qui revient au même, que les premiers membres des équations de ce système soient des formes linéairement indépendantes).

### 7. Produit tensoriel d’espaces vectoriels

Les résultats des §§ 3, 4 et 5 relatifs aux modules libres ou projectifs s’appliquent en particulier aux espaces vectoriels et donnent les propositions suivantes:

#### Proposition 14 {#alg-ii-s7-prop-14 .statement}

Étant donnés une suite exacte

$$
0 \to E' \to E \to E'' \to 0
$$

d’espaces vectoriels à droite sur un corps $K$ et d’applications linéaires, et un espace vectoriel à gauche $F$ sur $K$, la suite correspondante d’applications $\mathbf{Z}$-linéaires

$$
0 \to E' \otimes_K F \to E \otimes_K F \to E'' \otimes_K F \to 0
$$

est exacte et scindée.

Comme la suite (23) est scindée, c’est là un cas particulier de II, p. 63, cor. 5 et II, p. 58, prop. 5.

En raison de la prop. 14, lorsque $E'$ est un sous-espace vectoriel de $E$, $j : E' \to E$ l’injection canonique, on identifie d’ordinaire $E' \otimes_K F$ à un sous-$\mathbf{Z}$-module de $E \otimes_K F$ au moyen de l’injection $j \otimes 1_F$. Avec cette convention:

#### Corollaire {#alg-ii-s7-n7-cor-1 .statement}

Soient K un corps, E un espace vectoriel à droite sur K, F un espace vectoriel à gauche sur K, $(M_\alpha)_{\alpha \in A}$ une famille de sous-espaces vectoriels de E, $(N_\beta)_{\beta \in B}$ une famille de sous-espaces vectoriels de F. On a alors

(24)
$$
(\bigcap_{\alpha \in A} M_\alpha) \otimes_K (\bigcap_{\beta \in B} N_\beta) = \bigcap_{(\alpha, \beta) \in A \times B} (M_\alpha \otimes_K N_\beta).
$$

Il suffit évidemment de démontrer le cas particulier

(25)
$$
(\bigcap_{\alpha \in A} M_\alpha) \otimes_K F = \bigcap_{\alpha \in A} (M_\alpha \otimes_K F).
$$

Il est clair que le premier membre de (25) est contenu dans le second. Pour prouver la réciproque, considérons une base $(f_\lambda)_{\lambda \in L}$ de F. Tout élément de $E \otimes_K F$ se met alors d’une seule manière sous la forme $\sum_{\lambda \in L} x_\lambda \otimes f_\lambda$, où $x_\lambda \in E$ (II, p. 62, cor. 1); si $E'$ est un sous-espace vectoriel de E, la relation $\sum_{\lambda \in L} x_\lambda \otimes f_\lambda \in E' \otimes_K F$ équivaut, en vertu de la prop. 14 (II, p. 108), à $x_\lambda \in E'$ pour tout $\lambda \in L$. Dire que $\sum_{\lambda \in L} x_\lambda \otimes f_\lambda$ appartient à chacun des $M_\alpha \otimes_K F$ signifie donc que pour tout $\lambda \in L$ et tout $\alpha \in A$, on a $x_\lambda \in M_\alpha$, c’est-à-dire $x_\lambda \in \bigcap_{\alpha \in A} M_\alpha$ pour tout $\lambda \in L$, ce qui prouve que le second membre de (25) est contenu dans le premier.

#### Proposition 15 {#alg-ii-s7-prop-15 .statement}

Si $(E_\lambda)_{\lambda \in L}$ est une famille d’espaces vectoriels à droite sur un corps K, $(F_\mu)_{\mu \in M}$ une famille d’espaces vectoriels à gauche sur K, l’application canonique

(26)
$$
\left( \prod_{\lambda \in L} E_\lambda \right) \otimes_K \left( \prod_{\mu \in M} F_\mu \right) \to \prod_{(\lambda, \mu) \in L \times M} (E_\lambda \otimes_K F_\mu)
$$
(II, p. 61, formule (22)) est injective.

Posons $F = \prod_{\mu \in M} F_\mu$; l’application (26) est composée des applications canoniques $(\prod_{\lambda \in L} E_\lambda) \otimes_K F \to \prod_{\lambda \in L} (E_\lambda \otimes_K F)$ et $\prod_{\lambda \in L} (E_\lambda \otimes_K F) \to \prod_{\lambda \in L} \left( \prod_{\mu \in M} (E_\lambda \otimes_K F_\mu) \right)$; comme F et les $E_\lambda$ sont des espaces vectoriels sur K, on est ramené à II, p. 63, cor. 3.

Lorsque les conditions de la prop. 15 sont remplies, on identifiera souvent le produit tensoriel $\left( \prod_{\lambda \in L} E_\lambda \right) \otimes_K \left( \prod_{\mu \in M} F_\mu \right)$ à son image canonique dans $\prod_{\lambda, \mu} (E_\lambda \otimes_K F_\mu)$. Avec cette convention:

#### Corollaire {#alg-ii-s7-n7-cor-2 .statement}

Soit F un espace vectoriel à gauche sur K; pour tout ensemble X, l’espace vectoriel à gauche $K_d^X \otimes_K F$ s’identifie au sous-espace de l’espace $F^X$ de toutes les applications de X dans F, formé des applications u telles que $u(X)$ soit de rang fini dans F.

En effet, si $(f_\lambda)$ est une base de F, l’élément $\sum_{\lambda \in L} v_\lambda \otimes f_\lambda$ de $K_d^X \otimes_K F$ s’identifie par (26) à l’application $x \mapsto \sum_\lambda v_\lambda(x)f_\lambda$. Comme $v_\lambda = 0$ sauf pour les indices $\lambda$ appartenant à une partie finie H de L, l’image de X par l’application précédente est contenue dans le sous-espace de F de dimension finie engendré par les $f_\lambda$ d’indices $\lambda \in H$. Inversement, soit $u : X \to F$ une application telle que $u(X)$ soit contenu dans un sous-espace G de F de dimension finie et soit $(b_i)_{1 \leq i \leq n}$ une base de G. Pour tout $x \in X$ on peut écrire $u(x) = \sum_{i=1}^n v_i(x) b_i$, où les $v_i(x)$ sont des éléments bien déterminés de K ; on définit ainsi n applications $v_i : X \to K$ et il est clair que $u$ est alors identifié à l’élément $\sum_{i=1}^n v_i \otimes b_i$.

De même, pour un espace vectoriel à droite E sur K et un ensemble Y, $E \otimes_K K_s^Y$ s’identifie au sous-espace de l’espace $E^Y$, formé des applications $v : Y \to E$ telles que $v(Y)$ soit de rang fini. Plus particulièrement, pour tout corps K, $K_d^X \otimes_K K_s^Y$ s’identifie à un sous-espace de l’espace $K^{X \times Y}$ des applications de $X \times Y$ dans K (K étant considéré comme (K, K)-bimodule) ; un élément $\sum_i u_i \otimes v_i$, où $u_i$ est une application de X dans K et $v_i$ une application de Y dans K, s’identifie à l’application $(x, y) \mapsto \sum_i u_i(x)v_i(y)$ de $X \times Y$ dans K.

#### Proposition 16 {#alg-ii-s7-prop-16 .statement}

(i) *Soient K, L deux corps, E un espace vectoriel à gauche sur K, F un espace vectoriel à gauche sur L, G un (K, L)-bimodule. Alors le $\mathbf{Z}$-homomorphisme canonique*
$$
\nu : \operatorname{Hom}_K(E, G) \otimes_L F \to \operatorname{Hom}_K(E, G \otimes_L F)
$$
*(II, p. 75, formule (7)) est injectif; il est bijectif lorsque l’un des espaces vectoriels E, F est de dimension finie.*

(ii) *Soient $E_1, E_2, F_1, F_2$ quatre espaces vectoriels sur un corps commutatif K; alors le K-homomorphisme canonique*
$$
\lambda : \operatorname{Hom}(E_1, F_1) \otimes \operatorname{Hom}(E_2, F_2) \to \operatorname{Hom}(E_1 \otimes E_2, F_1 \otimes F_2)
$$
*(II, p. 79, formule (21)) est injectif; il est bijectif si l’un des couples $(E_1, E_2), (E_1, F_1), (E_2, F_2)$ est formé d’espaces de dimension finie.*

L’assertion (i) est un cas particulier de II, p. 75, prop. 2. De même la seconde assertion de (ii) est un cas particulier de II, p. 79, prop. 4. Enfin, pour voir que l’homomorphisme (28) est toujours injectif, observons que $\operatorname{Hom}(E_i, F_i)$ est un sous-espace vectoriel de $F_i^{E_i}$ ($i = 1, 2$) et que $\operatorname{Hom}(E_1 \otimes E_2, F_1 \otimes F_2)$ s’identifie canoniquement à un sous-espace vectoriel de l’espace $(F_1 \otimes F_2)^{E_1 \times E_2}$ (II, p. 51, prop. 1); lorsqu’on fait ces identifications, et qu’on identifie en outre le premier membre de (28) à un sous-espace de $F_1^{E_1} \otimes F_2^{E_2}$ (II, p. 108, prop. 14), l’application canonique (28) devient la restriction à ce sous-espace de l’application canonique (26) (II, p. 109), et on a vu (II, p. 109, prop. 15) que cette dernière est injective.

#### Corollaire 1 {#alg-ii-s7-prop-16-cor-1 .statement}

*Soient E et F deux espaces vectoriels à gauche sur un corps K; l’application canonique*
$$
E^* \otimes_K F \to \operatorname{Hom}_K(E, F)
$$

(II, p. 77, formule (11)) est injective; elle est bijective lorsque E ou F est de dimension finie.
C’est un cas particulier de la prop. 16, (i).

#### Corollaire 2 {#alg-ii-s7-prop-16-cor-2 .statement}

Soient E un espace vectoriel à droite, F un espace vectoriel à gauche sur un même corps K ; l’application canonique
$$
E \otimes_K F \to \operatorname{Hom}_K(E^*, F)
$$
(II, p. 78, formule (15)) est injective; elle est bijective lorsque E est de dimension finie.
C’est un cas particulier de II, p. 77, Remarque 2.

#### Remarque 1 {#alg-ii-s7-n7-rem-1 .statement}

Soient K un corps commutatif, E, F deux espaces vectoriels sur K, $(a_\lambda)$ une base de E, $(b_\mu)$ une base de F; alors $(a_\lambda \otimes b_\mu)$ est une base du K-espace vectoriel $E \otimes_K F$ (II, p. 62, cor. 2), et par suite on a
$$
\dim_K(E \otimes_K F) = \dim_K E \cdot \dim_K F.
$$

#### Remarque 2 {#alg-ii-s7-n7-rem-2 .statement}

Soient K un corps commutatif, $E_1, E_2, F_1, F_2$ quatre espaces vectoriels sur K, $u : E_1 \to F_1, v : E_2 \to F_2$ deux applications linéaires; on a alors
$$
\operatorname{rg}(u \otimes v) = \operatorname{rg}(u) \cdot \operatorname{rg}(v).
$$
En effet, il est immédiat que $(u \otimes v)(E_1 \otimes E_2)$ est l’image canonique de $u(E_1) \otimes v(E_2)$ dans $F_1 \otimes F_2$, donc (II, p. 108, prop. 14) est isomorphe à $u(E_1) \otimes v(E_2)$; la conclusion résulte alors de (30).

#### Remarque 3 {#alg-ii-s7-n7-rem-3 .statement}

Sous les mêmes hypothèses que dans la Remarque 1, on a
$$
\dim_K(\operatorname{Hom}_K(E, F)) \geq \dim_K E \cdot \dim_K F.
$$
En effet, si E est isomorphe à $K^{(I)}$, $\operatorname{Hom}(E, F)$ est isomorphe à $(\operatorname{Hom}(K, F))^{I}$ (II, p. 13, cor. 1), donc à $F^{I}$ (II, p. 35); comme $F^{(I)}$ est un sous-espace de $F^{I}$ et que $\dim(F^{(I)}) = \operatorname{Card}(I) \cdot \dim F = \dim E \cdot \dim F$ (II, p. 97, prop. 2), l’inégalité (32) résulte de II, p. 99, cor. 4. Le même raisonnement montre que les deux membres de (32) sont égaux lorsque dim E est finie (cf. II, p. 142 et 144).

### 8. Rang d’un élément d’un produit tensoriel

Soient E un espace vectoriel à droite, F un espace vectoriel à gauche sur un même corps K; à tout élément $u \in E \otimes_K F$ il correspond canoniquement un homomorphisme $u_1 \in \operatorname{Hom}_K(E^*, F)$ par (29); si $u = \sum_i x_i \otimes y_i$, avec $x_i \in E$, $y_i \in F$, l’élément $u_1$ est l’application linéaire
$$
x^* \mapsto \sum_i \langle x^*, x_i \rangle y_i.
$$
D’autre part, $E \otimes_K F$ s’identifie canoniquement à $F \otimes_{K^0} E$, où E est considéré comme espace vectoriel à gauche et F comme espace vectoriel à droite sur le corps opposé $K^0$; il correspond donc canoniquement à $u$ un homomorphisme $u_2 \in \mathrm{Hom}_K(F^*, E)$, donné par

$$
y^* \mapsto \sum_i x_i \langle y_i, y^* \rangle;
$$

$u_1$ (resp. $u_2$), considérée comme application de $E^*$ dans $F^{**}$ (resp. de $F^*$ dans $E^{**}$), n’est autre que la *transposée* de $u_2$ (resp. $u_1$). Les *rangs* de $u_1$ et $u_2$ sont donc égaux à un même nombre *fini* $r$, dimension commune des sous-espaces $u_1(E^*)$ de $F$ et $u_2(F^*)$ de $E$, dont chacun est canoniquement isomorphe au dual de l’autre (II, p. 103); nous dirons que $r$ (noté $\mathrm{rg}(u)$) est le *rang* de l’élément $u$ de $E \otimes_K F$, et que $u_1(E^*)$ et $u_2(F^*)$ sont les sous-espaces (de $F$ et $E$ respectivement) *associés* à $u$.

#### Proposition 17 {#alg-ii-s7-prop-17 .statement}

*Soit* $u$ *un élément de* $E \otimes_K F$, $M \subset E$ *et* $N \subset F$ *ses sous-espaces associés.* *Pour toute expression* $u = \sum_{i=1}^s x_i \otimes y_i$ *de* $u$, *où* $x_i \in E$ *et* $y_i \in F$ *pour* $1 \leq i \leq s$, *le sous-espace* $M$ *(resp. N)* *est contenu dans le sous-espace de* $E$ *(resp. F)* *engendré par les* $x_i$ *(resp. les* $y_i$). *En outre, les propriétés suivantes sont équivalentes*:

a) *L’entier* $s$ *est égal au rang de* $u$.
b) *La famille* $(x_i)_{1 \leq i \leq s}$ *est une base de* $M$.
c) *La famille* $(y_i)_{1 \leq i \leq s}$ *est une base de* $N$.
d) *Les familles* $(x_i)_{1 \leq i \leq s}$ *et* $(y_i)_{1 \leq i \leq s}$ *sont toutes deux libres*.

D’après (33) (resp. 34)) chaque élément de $N = u_1(E^*)$ (resp. de $M = u_2(F^*)$) est combinaison linéaire des $y_i$ (resp. des $x_i$); d’où la première assertion. Si $s = r$, le sous-espace engendré par les $x_i$ (resp. $y_i$) ayant une dimension $\leq \dim M$ (resp. $\leq \dim N$) et contenant $M$ (resp. $N$) lui est identique, donc a) implique b) et c), et *a fortiori* d). Inversement, chacune des conditions b), c) implique a) par définition de $\mathrm{rg}(u)$. Enfin, si d) est vérifiée, il existe une famille $(x_i^*)_{1 \leq i \leq s}$ d’éléments de $E^*$ telle que $\langle x_i, x_j^* \rangle = \delta_{ij}$ (II, p. 104, cor. 1), donc il résulte de (33) que $(y_i)$ est une base de $N$, ce qui achève la démonstration.

#### Corollaire 1 {#alg-ii-s7-prop-17-cor-1 .statement}

*Le rang de* $u$ *est le plus petit entier* $s$ *tel qu’il existe une expression*
$$ u = \sum_{i=1}^s x_i \otimes y_i, \text{où } x_i \in E \text{ et } y_i \in F \text{ pour } 1 \leq i \leq s. $$
Cela résulte aussitôt de la prop. 17 et de II, p. 97, prop. 1.

#### Corollaire 2 {#alg-ii-s7-prop-17-cor-2 .statement}

*Soient* $K$ *un corps commutatif*, $E, F$ *deux espaces vectoriels sur* $K$, $L$ *un surcorps commutatif de* $K$. *Soient* $u$ *un élément de* $E \otimes_K F$, $M$ *et* $N$ *ses sous-espaces associés*, $u'$ *l’image canonique de* $u$ *dans* $(E \otimes_K F)_{(L)}$ *(identifié canoniquement à* $E_{(L)} \otimes_L F_{(L)}$, cf. II, p. 83, prop. 3); *alors on a* $\mathrm{rg}(u') = \mathrm{rg}(u)$, *et les sous-espaces associés à* $u'$ *s’identifient canoniquement à* $M_{(L)}$ *et* $N_{(L)}$.

En effet, si $u = \sum_{i=1}^r x_i \otimes y_i$, où les familles $(x_i)$ et $(y_i)$ sont libres, on a $u' =$

$$
\sum_{i=1}^{r} (1 \otimes x_i) \otimes (1 \otimes y_i),
$$
et les familles $(1 \otimes x_i)$ et $(1 \otimes y_i)$ sont libres dans $E_{(L)}$ et $F_{(L)}$ respectivement (II, p. 84, prop. 4).

### 9. Extension des scalaires d’un espace vectoriel

Rappelons (I, p. 110, th. 2) qu’un homomorphisme d’un corps $\mathbf{K}$ dans un anneau $A$ non réduit à 0 est nécessairement injectif.

#### Proposition 18 {#alg-ii-s7-prop-18 .statement}

Soit $\rho$ un homomorphisme d’un corps $\mathbf{K}$ dans un anneau $A$. Pour toute suite exacte de $\mathbf{K}$-espaces vectoriels et d’applications $\mathbf{K}$-linéaires

$$
E' \xrightarrow{u} E \xrightarrow{v} E''
$$

la suite

$$
E'_{(A)} \xrightarrow{u_{(A)}} E_{(A)} \xrightarrow{v_{(A)}} E''_{(A)}
$$

est exacte.

C’est un cas particulier de II, p. 108, prop. 14, compte tenu de II, p. 9, Remarque 4.

#### Corollaire {#alg-ii-s7-n9-cor-1 .statement}

Pour toute application $\mathbf{K}$-linéaire $f : E' \to E$, on a $\operatorname{Im}(f_{(A)}) = (\operatorname{Im}(f))_{(A)}$, $\operatorname{Ker}(f_{(A)}) = (\operatorname{Ker}(f))_{(A)}$, $\operatorname{Coker}(f_{(A)}) = (\operatorname{Coker}(f))_{(A)}$, à des isomorphismes canoniques près.

#### Proposition 19 {#alg-ii-s7-prop-19 .statement}

Soit $\rho$ un homomorphisme injectif d’un corps $\mathbf{K}$ dans un anneau $A$. Pour tout espace vectoriel à gauche $E$ sur $\mathbf{K}$, l’application canonique $\varphi : E \to \rho^*(E) = A \otimes_{\mathbf{K}} E$ est injective. En outre, pour tout sous-espace vectoriel $E'$ de $E$, $\rho^*(E') = A \otimes_{\mathbf{K}} E'$ s’identifie canoniquement à un sous-$A$-module facteur direct de $A \otimes_{\mathbf{K}} E$, et avec cette identification, on a

$$(35)\quad (A \otimes_{\mathbf{K}} E') \cap \varphi(E) = \varphi(E').$$

La première assertion est un cas particulier de II, p. 84, prop. 4; la seconde est un cas particulier de II, p. 108, prop. 14; enfin, pour démontrer (35), il suffit de prendre dans $A$ (considéré comme $\mathbf{K}$-module à droite) une base $(a_\lambda)_{\lambda \in L}$ telle que $a_{\lambda_0} = 1$ pour un indice $\lambda_0$ (II, p. 95, th. 2); les éléments de $A \otimes_{\mathbf{K}} E$ s’écrivent d’une seule manière $\sum_\lambda a_\lambda \otimes x_\lambda$ avec $x_\lambda \in E$, et pour qu’un tel élément appartienne à $A \otimes_{\mathbf{K}} E'$, il faut et il suffit que $x_\lambda \in E'$ pour tout $\lambda$. D’autre part, les éléments de $\varphi(E)$ sont ceux pour lesquels $x_\lambda = 0$ pour $\lambda \neq \lambda_0$; pour qu’un élément $\sum_\lambda a_\lambda \otimes x_\lambda$ appartienne à $(A \otimes_{\mathbf{K}} E') \cap \varphi(E)$, il faut et il suffit donc que $x_\lambda = 0$ pour $\lambda \neq \lambda_0$ et $x_{\lambda_0} \in E'$, d’où la conclusion.

#### Corollaire {#alg-ii-s7-n9-cor-2 .statement}

Soit $\rho$ un homomorphisme injectif d’un corps $\mathbf{K}$ dans un anneau $A$. Pour qu’une application $\mathbf{K}$-linéaire $f : E \to F$ (où $E$ et $F$ sont deux espaces vectoriels sur $\mathbf{K}$) soit injective (resp. surjective, nulle), il faut et il suffit que $f_{(A)} : E_{(A)} \to F_{(A)}$ soit injective (resp. surjective, nulle).

Cela résulte aussitôt de la prop. 19 et du cor. de la prop. 18.

#### Proposition 20 {#alg-ii-s7-prop-20 .statement}

*Soit $\rho$ un homomorphisme injectif d’un corps $K$ dans un anneau $A$. Pour tout espace vectoriel à gauche $E$ sur $K$, l’homomorphisme canonique de $A$-modules à droite*
$$
\upsilon : (E^*)_{(A)} \to (E_{(A)})^*
$$
*(II, p. 87)* est injectif; il est bijectif lorsque $E$ est de dimension finie.

La seconde assertion résulte de II, p. 88, prop. 8. Pour prouver la première, remarquons que tout élément de $(E^*)_{(A)}$ s’écrit $\sum_i x_i^* \otimes \alpha_i$, où $\alpha_i \in A$ et où $(x_i^*)_{1 \leq i \leq n}$ est une famille libre dans $E^*$; il lui correspond dans $(E_{(A)})^*$ la forme linéaire $y^*$ telle que $y^*(1 \otimes x) = \sum_i \rho(\langle x, x_i^* \rangle) \alpha_i$ pour tout $x \in E$. Or, il existe dans $E$ une famille $(x_i)_{1 \leq i \leq n}$ telle que $\langle x_i, x_j^* \rangle = \delta_{ij}$ (II, p. 105, cor. 2), d’où $y^*(1 \otimes x_i) = \alpha_i$; la relation $y^* = 0$ entraîne donc $\alpha_i = 0$ pour tout $i$, ce qui démontre notre assertion.

#### Proposition 21 {#alg-ii-s7-prop-21 .statement}

*Soient $K$ un corps, $L$ un surcorps de $K$.
(i) Pour tout espace vectoriel $E$ sur $K$, on a $\dim_L(E_{(L)}) = \dim_K E$.
(ii) Pour toute application $K$-linéaire $u : E \to F$, où $E$ et $F$ sont des espaces vectoriels sur $K$, on a $\mathrm{rg}(u_{(L)}) = \mathrm{rg}(u)$.

Si $(e_i)_{i \in I}$ est une base de $E$ sur $K$, $(1 \otimes e_i)_{i \in I}$ est une base de $E_{(L)}$ sur $L$ (II, p. 84, prop. 4), d’où la première assertion; la seconde résulte de la première et de ce que $u_{(L)}(E_{(L)})$ s’identifie canoniquement à $(u(E))_{(L)}$ en vertu de II, p. 113, corollaire de la prop. 18.*

#### Proposition 22 {#alg-ii-s7-prop-22 .statement}

*Soient $K$ un corps commutatif, $\rho : K \to A$ un homomorphisme central injectif, $E, F$ deux espaces vectoriels sur $K$. Alors l’homomorphisme canonique*
$$
\omega : A \otimes_K \mathrm{Hom}(E, F) \to \mathrm{Hom}_A(E_{(A)}, F_{(A)})
$$
*(II, p. 86, formule (17))* est injectif; il est bijectif si $A$ ou $E$ est un espace vectoriel sur $K$ de dimension finie.

C’est un cas particulier de II, p. 87, prop. 7.

### 10. Modules sur les anneaux intègres

#### Proposition 23 {#alg-ii-s7-prop-23 .statement}

*Dans un module $E$ sur un anneau intègre $A$, l’ensemble $T$ des éléments non libres est un sous-module de $E$.

En effet, si $x$ et $y$ sont non libres, il existe deux éléments $\alpha, \beta$ non nuls dans $A$ tels que $\alpha x = 0$ et $\beta y = 0$. On a $\alpha \beta \neq 0$ puisque $A$ est intègre, et $\alpha \beta (\lambda x + \mu y) = 0$ quels que soient $\lambda$ et $\mu$ dans $A$ puisque $A$ est commutatif, donc $\lambda x + \mu y$ est non libre.*

#### Remarque {#alg-ii-s7-n10-rem-1 .statement}

Soit E un module sur un anneau commutatif quelconque A. Si x est un élément non libre de E, tout élément du sous-module Ax est non libre. Par contre, si A contient des diviseurs de 0, la somme de deux éléments non libres de E peut être libre; par exemple, dans $\mathbf{Z}/6\mathbf{Z}$ considéré comme module sur lui-même, 3 et 4 sont non libres, mais $3 + 4 = 1$ est libre.

La prop. 23 conduit à poser la définition suivante:

#### Définition 5 {#alg-ii-s7-def-5 .statement}

Dans un module E sur un anneau intègre A, on appelle sous-module de torsion de E le sous-module de E formé des éléments non libres (aussi appelés éléments de torsion de E).

Lorsque E est égal à son sous-module de torsion (c’est-à-dire lorsque tout élément de E est annulé par un élément $\neq 0$ de A) on dit que E est un module de torsion. Lorsque le sous-module de torsion de E est réduit à 0 (c’est-à-dire que tout élément $\neq 0$ de E est libre) on dit (par abus de langage) que E est un module sans torsion.

Tout sous-module d’un A-module libre (et en particulier tout A-module projectif) est sans torsion. Le $\mathbf{Z}$-module $\mathbf{Q}$ est sans torsion.

#### Proposition 24 {#alg-ii-s7-prop-24 .statement}

Soit A un anneau intègre. Pour tout A-module E, notons T(E) le sous-module de torsion de E. Soit $f : E \to E'$ une application A-linéaire, E et E' étant des A-modules.
(i) On a $f(T(E)) \subset T(E')$.
(ii) Si f est injective, on a $f(T(E)) = T(E') \cap f(E)$.
(iii) Si f est surjective et si $\operatorname{Ker}(f) \subset T(E)$, alors $f(T(E)) = T(E')$.

Les assertions (i) et (ii) sont évidentes. D’autre part, si f est surjective et $x' \in T(E')$, on a $x' = f(x)$, où $x \in E$, et par hypothèse il existe $\alpha \neq 0$ dans A tel que $f(\alpha x) = \alpha x' = 0$; d’où $\alpha x \in \operatorname{Ker}(f)$, et en vertu de l’hypothèse, il existe $\beta \neq 0$ dans A tel que $\beta (\alpha x) = 0$; comme $\beta \alpha \neq 0$, on a bien $x \in T(E)$.

#### Corollaire 1 {#alg-ii-s7-prop-24-cor-1 .statement}

Pour tout A-module E, $E/T(E)$ est sans torsion.

Si $f : E \to E'$ est une application A-linéaire, notons $f_T$ l’application $T(E) \to T(E')$ qui a même graphe que la restriction de f à T(E). Avec cette notation:

#### Corollaire 2 {#alg-ii-s7-prop-24-cor-2 .statement}

Pour toute suite exacte de A-modules et d’applications A-linéaires

$$
0 \longrightarrow E' \xrightarrow{f} E \xrightarrow{g} E''
$$

la suite

$$
0 \longrightarrow T(E') \xrightarrow{f_T} T(E) \xrightarrow{g_T} T(E'')
$$

est exacte.

En effet,

$$
\operatorname{Ker}(g_T) = \operatorname{Ker}(g) \cap T(E) = f(E') \cap T(E) = f(T(E')) = \operatorname{Im}(f_T).
$$

#### Proposition 25 {#alg-ii-s7-prop-25 .statement}

*Soient A un anneau intègre, (E_i) une famille de A-modules; on a*
$$
T(\bigoplus_i E_i) = \bigoplus_i T(E_i).
$$
En effet, soit $(x_i)$ un élément de $\bigoplus_i E_i$ tel que $x_i \in T(E_i)$ pour tout $i$; alors chacun des $x_i$ est annulé par un élément $\alpha_i \neq 0$ de $A$, et on peut supposer que $\alpha_i = 1$ lorsque $x_i = 0$; comme la famille $(x_i)$ a un support fini, l’élément $\alpha = \prod_i \alpha_i$ de $A$ est défini et $\neq 0$; il annule évidemment $\bigoplus_i x_i$, donc $\bigoplus_i T(E_i) \subset T(\bigoplus_i E_i)$; la réciproque est immédiate.

Si $E$ et $F$ sont deux $A$-modules, il est clair que $T(E \otimes_A F)$ contient les images canoniques de $T(E) \otimes_A F$ et de $E \otimes_A T(F)$; mais on peut donner des exemples de $A$-modules *sans torsion*, $E$, $F$ tels que $T(E \otimes_A F) \neq 0$ (II, p. 197, exerc. 31).

On notera qu’un produit *infini* de modules de torsion n’est pas nécessairement un module de torsion; par exemple, dans le $\mathbf{Z}$-module $\prod_{i=1}^\infty (\mathbf{Z}/p^n\mathbf{Z})$ ($p$ entier $> 1$), l’élément dont toutes les coordonnées sont 1 est libre.

#### Proposition 26 {#alg-ii-s7-prop-26 .statement}

*Soient A un anneau intègre, K son corps des fractions, E un A-module, $E_{(K)} = K \otimes_A E$ l’espace vectoriel sur K obtenu par extension de l’anneau d’opérateurs; désignons par $\varphi$ l’application A-linéaire canonique $x \mapsto 1 \otimes x$ de E dans $E_{(K)}*.$

(i) *Tout élément de $E_{(K)}$ est de la forme $\lambda^{-1} \varphi(x)$ pour $\lambda \in A, \lambda \neq 0$ et $x \in E$.*

(ii) *Le noyau de $\varphi$ est le sous-module de torsion $T(E)$ de E.*

(i) Tout élément de $E_{(K)}$ est de la forme $z = \sum_{i=1}^n \xi_i \varphi(x_i)$ avec $\xi_i \in K$ et $x_i \in E$; pour tout $i$, il existe $\alpha_i \in A$ tel que $\alpha_i \neq 0$ et $\alpha_i \xi_i \in A$; si $\alpha = \prod_{i=1}^n \alpha_i$, on a donc $\alpha \neq 0$ et $\alpha \xi_i = \beta_i \in A$ pour tout $i$, d’où, dans $E_{(K)}$,
$$
z = \alpha^{-1}(\alpha z) = \alpha^{-1} \sum_{i=1}^n \beta_i \varphi(x_i) = \alpha^{-1} \varphi \left( \sum_{i=1}^n \beta_i x_i \right)
$$
puisque $\varphi$ est A-linéaire.

(ii) Si $x \neq 0$ n’est pas libre dans $E$, il existe $\alpha \neq 0$ dans $A$ tel que $\alpha x = 0$, d’où $\alpha \varphi(x) = \varphi(\alpha x) = 0$ dans $E_{(K)}$, ce qui entraîne $\varphi(x) = 0$. Réciproquement, supposons que pour un $x \in E$ on ait $1 \otimes x = 0$ dans $E_{(K)}$, et montrons que $x$ est un élément de torsion dans $E$. Considérons l’ensemble $\mathfrak{M}$ des sous-A-modules *monogènes* de $K$; c’est un ensemble filtrant croissant pour la relation d’inclusion, car deux éléments quelconques $\alpha, \beta$ de $K$ peuvent s’écrire $\alpha = \zeta^{-1} \xi$, $\beta = \zeta^{-1} \eta$, où $\xi, \eta, \zeta$ appartiennent à $A$ et $\zeta \neq 0$, donc $A.\alpha \subset A.\zeta^{-1}$ et $A.\beta \subset A.\zeta^{-1}$. En outre $K$ est réunion des modules $M \in \mathfrak{M}$, et peut donc être considéré comme la *limite inductive* du système inductif défini par les modules $M \in \mathfrak{M}$ et les injections canoniques (II, p. 93, *Remarque*). On a donc aussi, à un isomorphisme canonique près, $E_{(K)} = \lim_{\longrightarrow} (M \otimes_A E)$ (II, p. 93, prop. 7), et la relation $1 \otimes x = 0$ dans $E_{(K)}$ entraîne qu’il existe un $M \in \mathfrak{m}$ tel que $1 \in M$ et que l’on ait $1 \otimes x = 0$ dans le produit tensoriel $M \otimes_A E$ (E, III, p. 62, lemme 1). On peut d’ailleurs supposer (en remplaçant au besoin $M$ par un sous-module monogène $M' \supset M$ de $K$) que l’on a $M = A.\gamma^{-1}$, où $\gamma \in A$ et $\gamma \neq 0$. Or l’application $\xi \mapsto \gamma \xi$ est un isomorphisme de $M$ sur le $A$-module $A$; d’autre part, l’isomorphisme canonique $A \otimes_A E \to E$ (II, p. 55, prop. 4) fait correspondre à $\xi \otimes x$ l’élément $\xi x$ de $E$; il existe donc un isomorphisme $M \otimes_A E \to E$ qui, au produit tensoriel $\xi \otimes x$ fait correspondre l’élément $(\gamma \xi)x$ de $E$. L’hypothèse $1 \otimes x = 0$ dans $M \otimes_A E$ entraîne donc $\gamma x = 0$.

#### Remarque {#alg-ii-s7-n10-rem-2 .statement}

Soient $\alpha^{-1}\varphi(x), \beta^{-1}\varphi(y)$ deux éléments de $E_{(K)}$, avec $\alpha \in A, \beta \in A, x \in E, y \in E, \alpha \beta \neq 0$. Pour que $\alpha^{-1}\varphi(x) = \beta^{-1}\varphi(y)$ il faut et il suffit que $\beta x - \alpha y$ soit un élément de torsion de $E$, car cette relation équivaut à $\beta \varphi(x) = \alpha \varphi(y)$, ce qui s’écrit aussi $\varphi(\beta x - \alpha y) = 0$.

#### Corollaire 1 {#alg-ii-s7-prop-26-cor-1 .statement}

Si $E$ est un $A$-module sans torsion, l’application canonique $\varphi : E \to E_{(K)}$ est injective.

Rappelons (II, p. 82, prop. 1) que pour toute application $A$-linéaire $f$ de $E$ dans un espace vectoriel $F$ sur $K$, il existe une application $K$-linéaire et une seule $\bar{f} : E_{(K)} \to F$ telle que $f = \bar{f} \circ \varphi$; nous dirons que $\bar{f}$ est associée à $f$.

#### Corollaire 2 {#alg-ii-s7-prop-26-cor-2 .statement}

Soit $f$ une application $A$-linéaire de $E$ dans un espace vectoriel $F$ sur $K$; si l’on a $\operatorname{Ker}(f) \subset T(E)$, l’application $K$-linéaire $\bar{f}$ associée à $f$ est injective.

En effet, écrivons un élément de $\operatorname{Ker}(\bar{f})$ sous la forme $\lambda^{-1}\varphi(x)$, où $\lambda \in A, \lambda \neq 0, x \in E$; la relation $\bar{f}(\lambda^{-1}\varphi(x)) = 0$ équivaut à $\lambda^{-1}\bar{f}(\varphi(x)) = 0$ dans $F$, donc à $f(x) = \bar{f}(\varphi(x)) = 0$. Par hypothèse, cela entraîne $x \in T(E)$, donc $\varphi(x) = 0$, ce qui prouve le corollaire.

#### Corollaire 3 {#alg-ii-s7-prop-26-cor-3 .statement}

Soient $E$ un $A$-module, $g$ une application $A$-linéaire de $E$ dans un espace vectoriel $F$ sur $K$, telle que $g(E)$ engendre $F$ et que $\operatorname{Ker}(g) \subset T(E)$. Alors l’application $K$-linéaire $\bar{g}$ associée à $g$ est un isomorphisme de $E_{(K)}$ sur $F$.

En effet, $\bar{g}$ est injective en vertu du cor. 2, et l’hypothèse que $g(E)$ engendre $F$ entraîne que $\bar{g}$ est surjective.

Pour tout $A$-module $E$, on dit que l’espace vectoriel $E_{(K)}$ est associé à $E$. Pour toute partie $S$ de $E$, on appelle rang de $S$ sur $K$ (ou par abus de langage, rang de $S$) le rang de l’image canonique $\varphi(S)$ de $S$ dans $E_{(K)}$, autrement dit (II, p. 97, déf. 1) la dimension sur $K$ du sous-espace vectoriel de $E_{(K)}$ engendré par $\varphi(S)$.

Lorsque $E$ est un $A$-module sans torsion, on l’identifie d’ordinaire à son image canonique $\varphi(E)$ dans $E_{(K)}$. Avec cette convention, tout système générateur de $E$ contient une base de $E_{(K)}$ (II, p. 95, th. 2). En particulier:

#### Corollaire 4 {#alg-ii-s7-prop-26-cor-4 .statement}

Tout $A$-module de type fini est de rang fini.

On notera que la réciproque de ce corollaire n’est pas nécessairement exacte; par exemple $\mathbf{Q}$ est un $\mathbf{Z}$-module de rang 1 mais n’est pas de type fini sur $\mathbf{Z}$.

Rappelons (II, p. 83) que pour toute application linéaire $f : E \to E'$ (où $E$ et $E'$ sont des $A$-modules), on note $f_{(K)}$ l’application $K$-linéaire $1_K \otimes f : E_{(K)} \to E'_{(K)}$.

#### Proposition 27 {#alg-ii-s7-prop-27 .statement}

*Pour toute suite exacte*

$$
E' \xrightarrow{f} E \xrightarrow{g} E''
$$

*d’applications $A$-linéaires, la suite correspondante d’applications $K$-linéaires*

$$
E'_{(K)} \xrightarrow{f_{(K)}} E_{(K)} \xrightarrow{g_{(K)}} E''_{(K)}
$$

*est exacte*.

En effet, supposons que $g_{(K)}(\lambda^{-1} \otimes x) = 0$, avec $\lambda \in A, \lambda \neq 0, x \in E$; cela équivaut à $\lambda^{-1} \otimes g(x) = 0$ dans $E''_{(K)}$, donc aussi à $1 \otimes g(x) = \lambda(\lambda^{-1} \otimes g(x)) = 0$; en vertu de la prop. 26 (II, p. 116), il existe $\alpha \neq 0$ dans $A$ tel que $\alpha g(x) = 0$ dans $E''$, ou encore $g(\alpha x) = 0$. Par hypothèse, il y a donc un $x' \in E'$ tel que $\alpha x = f(x')$, et par suite $\lambda^{-1} \otimes x = f_{(K)}(\alpha^{-1}\lambda^{-1} \otimes x')$, ce qui démontre la proposition.

#### Corollaire 1 {#alg-ii-s7-prop-27-cor-1 .statement}

*Si $E'$ est un sous-module de $E$, $E'_{(K)}$ s’identifie canoniquement à un sous-espace vectoriel de $E_{(K)}$, et $(E/E')_{(K)}$ à $E_{(K)}/E'_{(K)}$.

Il suffit d’appliquer la prop. 27 à la suite exacte $0 \to E' \to E \to E/E' \to 0$.

#### Corollaire 2 {#alg-ii-s7-prop-27-cor-2 .statement}

*Pour toute application $A$-linéaire $f : E \to F$, on a $\mathrm{Ker}(f_{(K)}) = (\mathrm{Ker}(f))_{(K)}$, $\mathrm{Im}(f_{(K)}) = (\mathrm{Im}(f))_{(K)}$, $\mathrm{Coker}(f_{(K)}) = (\mathrm{Coker}(f))_{(K)}$ à des isomorphismes canoniques près. En particulier, pour que $f_{(K)}$ soit injective (resp. surjective, resp. nulle), il faut et il suffit que $\mathrm{Ker}(f) \subset T(E)$ (resp. que $\mathrm{Coker}(f)$ soit un module de torsion, resp. que $\mathrm{Im}(f) \subset T(F)$).

Cela résulte du cor. 1 et de la prop. 26 (II, p. 116).

#### Corollaire 3 {#alg-ii-s7-prop-27-cor-3 .statement}

*Soient $E$ un $A$-module, $(x_\lambda)_{\lambda \in L}$ une famille d’éléments de $E$. Pour que $(x_\lambda)$ soit une famille libre, il faut et il suffit que dans le $K$-espace vectoriel $E_{(K)}$, la famille $(1 \otimes x_\lambda)$ soit libre*.

En effet, la famille $(x_\lambda)$ définit une application $A$-linéaire $f : A^{(L)} \to E$ telle que $f(e_\lambda) = x_\lambda$ pour tout $\lambda \in L$ (($e_\lambda$) étant la base canonique de $A^{(L)}$), et dire que $(x_\lambda)$ est libre signifie que $f$ est injective. Il suffit d’appliquer le cor. 2 à $f$, en observant que $A^{(L)}$ est sans torsion (II, p. 116, prop. 25).

## EXERCICES {#alg-ii-s7-exercises}

See the [exercises for § 7](exercises/s7/).
