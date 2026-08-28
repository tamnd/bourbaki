---
book: alg
book_title: Algebra
chapter: II
chapter_title: ALGÈBRE LINÉAIRE
section: 2
section_title: Modules d’applications linéaires. Dualité
lang: fr
source: alg-i-iii-fr
book_pages: A II.183-A II.189
pdf_pages: 0213-0227, 0360-0366
extraction: ocr
subsections:
    - "no": 1
      title: Propriétés de Hom_A(E, F) relatives aux suites exactes
      page: 0
      pdf_page: 213
    - "no": 2
      title: Modules projectifs
      page: 39
      pdf_page: 216
    - "no": 3
      title: Formes linéaires; dual d’un module
      page: 40
      pdf_page: 217
    - "no": 4
      title: Orthogonalité
      page: 41
      pdf_page: 218
    - "no": 5
      title: Transposée d’une application linéaire
      page: 42
      pdf_page: 219
    - "no": 6
      title: Dual d’un module quotient. Dual d’une somme directe. Bases duales
      page: 44
      pdf_page: 221
    - "no": 7
      title: Bidual
      page: 46
      pdf_page: 223
    - "no": 8
      title: Équations linéaires
      page: 48
      pdf_page: 225
statements: 43
exercises: 24
content_sha256: 6fdcfa5713a3f71bb37e31c09d327449f1f66ff64a8caee1f42d7e5c6821200b
---

## § 2. MODULES D’APPLICATIONS LINÉAIRES. DUALITÉ

### 1. Propriétés de Hom_A(E, F) relatives aux suites exactes

#### Théorème 1 {#alg-ii-s2-thm-1 .statement}

Soient A un anneau, E', E, E'' trois A-modules, u : E' → E, v : E → E'' deux homomorphismes. Pour que la suite

(1)
$$
E' \xrightarrow{u} E \xrightarrow{v} E'' \longrightarrow 0
$$
soit exacte, il faut et il suffit que, pour tout A-module F, la suite

(2)
$$
0 \longrightarrow \operatorname{Hom}(E'', F) \xrightarrow{\bar{v}} \operatorname{Hom}(E, F) \xrightarrow{\bar{u}} \operatorname{Hom}(E', F)
$$
(où on a posé $\bar{u} = \operatorname{Hom}(u, 1_F)$ $\bar{v} = \operatorname{Hom}(v, 1_F)$) soit exacte.

Supposons la suite (1) exacte. Si $w \in \operatorname{Hom}(E'', F)$ et si $\bar{v}(w) = w \circ v = 0$, alors $w = 0$ puisque $v$ est surjectif. La suite (2) est donc exacte en $\operatorname{Hom}(E'', F)$. Montrons qu’elle est exacte en $\operatorname{Hom}(E, F)$. On a $\bar{u} \circ \bar{v} = \operatorname{Hom}(v \circ u, 1_F)$ (II, p. 6, formule (10)) et $v \circ u = 0$ puisque la suite (1) est exacte en E. Par conséquent $\bar{u} \circ \bar{v} = 0$, c’est-à-dire $\operatorname{Im}(\bar{v}) \subset \operatorname{Ker}(\bar{u})$. D’autre part, si $w \in \operatorname{Ker}(\bar{u})$, alors $w \circ u = 0$, donc $\operatorname{Ker}(w) \supset \operatorname{Im}(u)$. Mais comme la suite (1) est exacte en E, $\operatorname{Im}(u) = \operatorname{Ker}(v)$, donc $\operatorname{Ker}(w) \supset \operatorname{Ker}(v)$; comme $v$ est surjectif, il résulte de II, p. 7, Remarque qu’il existe un $w' \in \operatorname{Hom}(E'', F)$ tel que $w = w' \circ v = \bar{v}(w')$. Par conséquent $\operatorname{Ker}(\bar{u}) \subset \operatorname{Im}(\bar{v})$, ce qui achève de prouver que la suite (2) est exacte.

Inversement, supposons que (2) soit exacte pour tout A-module F. Comme $\bar{u} \circ \bar{v} = \operatorname{Hom}(v \circ u, 1_F) = 0$, on a $w \circ v \circ u = 0$ pour tout homomorphisme $w : E'' \to F$. Prenant $F = E''$ et $w = 1_{E''}$, on voit d’abord que $v \circ u = 0$, donc $u(E') \subset \operatorname{Ker}(v)$. Prenons ensuite $F = \operatorname{Coker}(u)$, et soit $\varphi : E \to F = E/u(E')$ l’application canonique. On a $\bar{u}(\varphi) = \varphi \circ u = 0$ par définition, donc il existe un $\psi \in \operatorname{Hom}(E'', F)$ tel que $\varphi = \bar{v}(\psi) = \psi \circ v$; cela entraîne évidemment $u(E') = \operatorname{Ker}(\varphi) \supset \operatorname{Ker}(v)$, ce qui prouve que la suite (1) est exacte en E. Enfin, soit $\theta$ l’homomorphisme canonique de $E''$ sur $F = E''/v(E)$; on a $\bar{v}(0) = \theta \circ v = 0$, donc $\theta = 0$; par suite, $F = \{0\}$ et $v$ est surjectif. La suite (1) est donc exacte en $E''$.

#### Corollaire {#alg-ii-s2-n1-cor-1 .statement}

Pour qu’une application A-linéaire $u : E \to F$ soit surjective (resp. bijective, resp. nulle), il faut et il suffit que, pour tout A-module G, l’application $\operatorname{Hom}(u, 1_G) : \operatorname{Hom}(F, G) \to \operatorname{Hom}(E, G)$ soit injective (resp. bijective, resp. nulle).

Il suffit d’appliquer le th. 1 au cas où $E'' = \{0\}$ (resp. $E' = \{0\}$, resp. $E'' = E$ et $v = 1_E$).

On notera que si l’on part d’une suite exacte
$$
0 \longrightarrow E' \xrightarrow{u} E \xrightarrow{v} E'' \longrightarrow 0
$$
la suite correspondante
$$
0 \longrightarrow \operatorname{Hom}(E'', F) \xrightarrow{\bar{v}} \operatorname{Hom}(E, F) \xrightarrow{\bar{u}} \operatorname{Hom}(E', F) \longrightarrow 0
$$

n’est pas nécessairement exacte, autrement dit, l’homomorphisme $\bar{u}$ n’est pas nécessairement surjectif. Si on identifie $E'$ à un sous-module de $E$, cela signifie qu’une application linéaire de $E'$ dans $F$ ne peut pas toujours se prolonger en une application linéaire de $E$ dans $F$ (II, p. 184–185, exerc. 11 et 12). Toutefois:

#### Proposition 1 {#alg-ii-s2-prop-1 .statement}

*Si la suite exacte d’applications linéaires*

$$
(3)\quad 0 \longrightarrow E' \xrightarrow{u} E \xrightarrow{v} E'' \longrightarrow 0
$$

*est scindée* (autrement dit, si $u(E')$ est *facteur direct* de $E$) *la suite*

$$
(4)\quad 0 \longrightarrow \mathrm{Hom}(E'', F) \xrightarrow{\bar{v}} \mathrm{Hom}(E, F) \xrightarrow{\bar{u}} \mathrm{Hom}(E', F) \longrightarrow 0
$$

*est exacte et scindée. Inversement, si, pour tout A-module F, la suite (4) est exacte, la suite (3) est scindée*.

Si la suite exacte (3) est scindée, il existe une rétraction linéaire $u': E \to E'$ associée à $u$ (II, p. 20, prop. 15); si

$$
\bar{u}' = \mathrm{Hom}(u', 1_F): \mathrm{Hom}(E', F) \to \mathrm{Hom}(E, F),
$$

le fait que $u' \circ u$ soit l’identité entraîne que $\bar{u} \circ \bar{u}'$ est l’identité (II, p. 6, formule (10)), donc la première assertion résulte de II, p. 20, prop. 15. Inversement, supposons la suite (4) exacte pour $F = E'$. Il existe alors un élément $f \in \mathrm{Hom}(E, E')$ tel que $f \circ u = 1_{E'}$, et la conclusion résulte de II, p. 20, prop. 15.

On notera que la première assertion de la prop. 1 peut aussi être considérée comme un cas particulier de II, p. 13, cor. 1, identifiant canoniquement $\mathrm{Hom}(E', F) \oplus \mathrm{Hom}(E'', F)$ à $\mathrm{Hom}(E' \oplus E'', F)$ au moyen de l’application $\mathbf{Z}$-linéaire $\mathrm{Hom}(p', 1_F) + \mathrm{Hom}(p'', 1_F)$, où $p': E' \oplus E'' \to E'$ et $p'': E' \oplus E'' \to E''$ sont les projections canoniques.

#### Théorème 2 {#alg-ii-s2-thm-2 .statement}

*Soient A un anneau, F', F, F'' trois A-modules, u: F' \to F, v: F \to F'' deux homomorphismes. Pour que la suite*

$$
(5)\quad 0 \longrightarrow F' \xrightarrow{u} F \xrightarrow{v} F''
$$

*soit exacte, il faut et il suffit que, pour tout A-module E, la suite*

$$
(6)\quad 0 \longrightarrow \mathrm{Hom}(E, F') \xrightarrow{\bar{u}} \mathrm{Hom}(E, F) \xrightarrow{\bar{v}} \mathrm{Hom}(E, F'')
$$

(où l’on a posé $\bar{u} = \mathrm{Hom}(1_E, u), \bar{v} = \mathrm{Hom}(1_E, v)$) *soit exacte*.

Supposons la suite (5) exacte. Notons d’abord que l’on a $\bar{v} \circ \bar{u} = \mathrm{Hom}(1_E, v \circ u) = 0$ (II, p. 6, formule (10)) puisque $v \circ u = 0$. L’image de $\mathrm{Hom}(E, F')$ par $\bar{u}$ est donc contenue dans le noyau N de $\bar{v}$; soit $f$ l’homomorphisme du $\mathbf{Z}$-module $\mathrm{Hom}(E, F')$ dans N dont le graphe est égal à celui de $\bar{u}$; il s’agit de prouver que $f$ est *bijective*, donc de définir une application $g: N \to \mathrm{Hom}(E, F')$ telle que $f \circ g$ et $g \circ f$ soient les applications identiques. Pour cela, soit $w$ un élément de N, c’est-à-dire une application linéaire $w: E \to F$ telle que $v \circ w = 0$. Cette dernière relation équivaut à $w(E) \subset \mathrm{Ker}(v) = u(F')$ par hypothèse, donc, puisque $u$ est injectif, il existe une application linéaire et une seule $w': E \to F'$ telle que $w = u \circ w'$, et on prend $g(w) = w'$; il est immédiat de vérifier que $g$ satisfait aux conditions voulues.

Inversement, supposons que la suite (6) soit exacte pour tout A-module E. Comme $\mathrm{Hom}(1_E, v \circ u) = \bar{v} \circ \bar{u} = 0$, on a $v \circ u \circ w = 0$ pour tout homomorphisme $w : E \to F'$. Prenant $E = F'$ et $w = 1_{F'}$, on voit d’abord que $v \circ u = 0$, donc $u(F') \subset \mathrm{Ker}(v)$. Prenons ensuite $E = \mathrm{Ker}(v)$ et soit $\varphi : E \to F$ l’injection canonique. On a $\bar{v}(\varphi) = v \circ \varphi = 0$ par définition, donc il existe un $\psi \in \mathrm{Hom}(E, F')$ tel que $\varphi = \bar{u}(\psi) = u \circ \psi$, ce qui entraîne évidemment $\mathrm{Ker}(v) \subset u(F')$ et achève la démonstration de l’exactitude de (5) en F. Enfin, si $\theta$ est l’application identique de $\mathrm{Ker}\, u$, on a $\bar{u}(\theta) = 0$, donc $\theta = 0$, et $\mathrm{Ker}\, u = \{0\}$, ce qui prouve l’exactitude de (5) en $F'$.

Remarque 1). — Le th. 2 permet, pour tout sous-module $F'$ de F, d’identifier $\mathrm{Hom}(E, F')$ à un sous-$\mathbf{Z}$-module de $\mathrm{Hom}(E, F)$. Lorsqu’on fait cette identification, on a, pour toute famille $(M_\lambda)$ de sous-modules de F
$$
\mathrm{Hom}(E, \bigcap_\lambda M_\lambda) = \bigcap_\lambda \mathrm{Hom}(E, M_\lambda)
$$
car si $u \in \mathrm{Hom}(E, F)$ appartient à chacun des $\mathrm{Hom}(E, M_\lambda)$, on a, pour tout $x \in E$, $u(x) \in M_\lambda$ pour tout $\lambda$, donc $u$ applique E dans $\bigcap_\lambda M_\lambda$.

#### Corollaire {#alg-ii-s2-n1-cor-2 .statement}

Pour qu’une application A-linéaire $u : E \to F$ soit injective, il faut et il suffit que pour tout A-module G, l’application $\mathrm{Hom}(1_G, u) : \mathrm{Hom}(G, E) \to \mathrm{Hom}(G, F)$ soit injective.

Il suffit d’appliquer le th. 2 au cas où $F' = \{0\}$.

Si l’on part d’une suite exacte
$$
0 \longrightarrow F' \xrightarrow{u} F \xrightarrow{v} F'' \longrightarrow 0
$$
la suite correspondante
$$
0 \longrightarrow \mathrm{Hom}(E, F') \xrightarrow{\bar{u}} \mathrm{Hom}(E, F) \xrightarrow{\bar{v}} \mathrm{Hom}(E, F'') \longrightarrow 0
$$
n’est pas nécessairement exacte, autrement dit $\bar{v}$ n’est pas nécessairement surjectif. Si on identifie $F'$ à un sous-module de F et $F''$ au module quotient $F/F'$, cela signifie qu’une application linéaire de E dans $F''$ n’est pas nécessairement de la forme $v \circ w$, où $w$ est une application linéaire de E dans F. Toutefois:

#### Proposition 2 {#alg-ii-s2-prop-2 .statement}

Si la suite exacte
$$
0 \longrightarrow F' \xrightarrow{u} F \xrightarrow{v} F'' \longrightarrow 0
$$
est scindée (autrement dit, si $u(F')$ est facteur direct de F), la suite
$$
0 \longrightarrow \mathrm{Hom}(E, F') \xrightarrow{\bar{u}} \mathrm{Hom}(E, F) \xrightarrow{\bar{v}} \mathrm{Hom}(E, F'') \longrightarrow 0
$$
est exacte et scindée. Inversement, si la suite (8) est exacte pour tout A-module E, la suite exacte (7) est scindée.

La première assertion résulte de ce que
$$
\mathrm{Hom}(E, F') \oplus \mathrm{Hom}(E, F'')
$$
s’identifie canoniquement à $\mathrm{Hom}(E, F' \oplus F'')$ au moyen de l’application $\mathbf{Z}$-linéaire $\operatorname{Hom}(l_E, j') + \operatorname{Hom}(l_E, j''),\ j': F' \to F' \oplus F''$ et $j'': F'' \to F' \oplus F''$ étant les injections canoniques (II, p. 13, cor. 1). Inversement, si la suite (8) est exacte pour $E = F''$, il y a un élément $g \in \operatorname{Hom}(F'', F)$ tel que $v \circ g = 1_{F''}$, et la conclusion résulte de II, p. 20, prop. 15.

Remarque 2). — Les résultats de ce n° sont valables sans modification pour tous les groupes commutatifs à opérateurs.

### 2. Modules projectifs

#### Définition 1 {#alg-ii-s2-def-1 .statement}

On dit qu’un A-module P est projectif si, pour toute suite exacte $F' \to F \to F''$ d’applications A-linéaires, la suite
$$
\operatorname{Hom}(P, F') \to \operatorname{Hom}(P, F) \to \operatorname{Hom}(P, F'')
$$
est exacte.

#### Proposition 3 {#alg-ii-s2-prop-3 .statement}

Pour qu’un A-module P, somme directe d’une famille de sous-modules $(M_i)$, soit projectif, il faut et il suffit que chacun des $M_i$ soit projectif.
En effet, pour tout homomorphisme $u : E \to F$ de A-modules,
$$
\operatorname{Hom}(1_P, u) : \operatorname{Hom}(P, E) \to \operatorname{Hom}(P, F)
$$
s’identifie à $\prod_i \operatorname{Hom}(1_{M_i}, u)$ (II, p. 13, cor. 1); la conclusion résulte donc de la déf. 1 et de II, p. 10, prop. 5(ii).

#### Corollaire {#alg-ii-s2-n2-cor-1 .statement}

Tout A-module libre est projectif.
Il suffit en effet, en vertu de la prop. 3, de montrer que $A_s$ est projectif, ce qui résulte aussitôt de la commutativité du diagramme (50) de II, p. 35.

#### Proposition 4 {#alg-ii-s2-prop-4 .statement}

Soit P un A-module. Les propriétés suivantes sont équivalentes:
a) P est projectif.
b) Pour toute suite exacte $0 \to F' \to F \to F'' \to 0$ d’applications A-linéaires, la suite
$$
0 \to \operatorname{Hom}(P, F') \to \operatorname{Hom}(P, F) \to \operatorname{Hom}(P, F'') \to 0
$$
est exacte.
c) Pour tout homomorphisme surjectif $u : E \to E''$ de A-modules et tout homomorphisme $f : P \to E''$, il existe un homomorphisme $g : P \to E$ tel que $f = u \circ g$ (on dit que $f$ « se relève » en un homomorphisme de P dans E).
d) Toute suite exacte $0 \to E' \to E \xrightarrow{v} P \to 0$ d’applications A-linéaires est scindée (et par suite P est isomorphe à un facteur direct de E).
e) P est isomorphe à un facteur direct d’un A-module libre.
Il est trivial que a) implique b). Pour voir que b) entraîne c), il suffit d’appliquer b) à la suite exacte $0 \to E' \to E \xrightarrow{u} E'' \to 0$ où $E' = \operatorname{Ker}(u)$, puisque c) exprime que
$$
\operatorname{Hom}(1_P, u) : \operatorname{Hom}(P, E) \to \operatorname{Hom}(P, E'')
$$

est surjectif. Pour voir que c) implique d), il suffit d’appliquer c) à l’homomorphisme surjectif $v : E \to P$ et à l’homomorphisme $1_P : P \to P$; l’existence d’un homomorphisme $g : P \to E$ tel que $1_P = v \circ g$ entraîne que la suite

$$
0 \longrightarrow E' \longrightarrow E \xrightarrow{v} P \longrightarrow 0
$$

est scindée (II, p. 20, prop. 15). Comme pour tout A-module M, il existe un A-module libre L et une suite exacte $0 \to R \to L \to M \to 0$ (II, p. 27, prop. 20), il est clair que d) entraîne e). Enfin e) entraîne a) en vertu de la prop. 3 et de son corollaire.

#### Corollaire 1 {#alg-ii-s2-prop-4-cor-1 .statement}

*Pour qu’un A-module soit projectif et de type fini, il faut et il suffit qu’il soit facteur direct d’un A-module libre ayant une base finie.*

La condition est évidemment suffisante; inversement, un module projectif de type fini E est isomorphe à un quotient d’un module libre F ayant une base finie (II, p. 27) et E est isomorphe à un facteur direct de F en vertu de la prop. 4 d).

#### Corollaire 2 {#alg-ii-s2-prop-4-cor-2 .statement}

*Soient C un anneau commutatif, E, F deux C-modules projectifs de type fini; alors Hom_C(E, F) est un C-module projectif de type fini.*

En effet, on peut supposer qu’il y a deux C-modules libres de type fini M, N tels que $M = E \oplus E', \ N = F \oplus F'$; il résulte de II, p. 13, cor. 1 que $\mathrm{Hom}_C(M, N)$ est libre de type fini, et d’autre part que $\mathrm{Hom}_C(M, N)$ est isomorphe à $\mathrm{Hom}_C(E, F) \oplus \mathrm{Hom}_C(E', F) \oplus \mathrm{Hom}_C(E, F') \oplus \mathrm{Hom}_C(E', F')$, d’où le corollaire.

### 3. Formes linéaires; dual d’un module

Soit E un A-module *à gauche*. Comme A est un (A, A)-bimodule, $\mathrm{Hom}_A(E, A_s)$ est canoniquement muni d’une structure de A-module *à droite* (II, p. 35).

#### Définition 2 {#alg-ii-s2-def-2 .statement}

*Pour tout A-module à gauche E, le A-module à droite $\mathrm{Hom}_A(E, A_s)$ s’appelle le module dual de E (ou simplement le dual¹ de E) et ses éléments s’appellent les formes linéaires sur E.*

Si E est un A-module *à droite*, on appelle de même *dual* de E l’ensemble $\mathrm{Hom}_A(E, A_d)$ muni de sa structure canonique de A-module *à gauche*, et on appelle encore ses éléments *formes linéaires* sur E.

Dans ce chapitre, nous désignerons par E* le dual d’un A-module E (à gauche ou à droite).

¹ Dans EVT, IV, nous définirons, pour des espaces vectoriels munis d’une *topologie*, une notion d’« espace dual » qui dépendra de cette topologie, et sera distincte de celle qui est définie ici. Le lecteur aura soin de ne pas appliquer inconsidérément à l’espace dual « topologique » les propriétés du dual « algébrique » qui sont établies dans ce paragraphe.

#### Exemple {#alg-ii-s2-n3-exa-1 .statement}

\* Sur l’espace vectoriel (par rapport au corps $\mathbf{R}$) des fonctions numériques continues dans un intervalle $[a, b]$ de $\mathbf{R}$, l’application $x \mapsto \int_a^b x(t)dt$ est une forme linéaire.*

Soient $E$ un $A$-module à gauche, $E^*$ son dual; pour tout couple d’éléments $x \in E,\ x^* \in E^*$, on désigne par $\langle x, x^* \rangle$ l’élément $x^*(x)$ de $A$. On a les relations

$$
\begin{align*}
(9)\qquad &\langle x + y, x^* \rangle = \langle x, x^* \rangle + \langle y, x^* \rangle \\
(10)\qquad &\langle x, x^* + y^* \rangle = \langle x, x^* \rangle + \langle x, y^* \rangle \\
(11)\qquad &\langle \alpha x, x^* \rangle = \alpha \langle x, x^* \rangle \\
(12)\qquad &\langle x, x^* \alpha \rangle = \langle x, x^* \rangle \alpha
\end{align*}
$$

pour $x, y$ dans $E,\ x^*, y^*$ dans $E^*$, et $\alpha \in A$. L’application $(x, x^*) \mapsto \langle x, x^* \rangle$ de $E \times E^*$ dans $A$ est appelée la *forme bilinéaire canonique* sur $E \times E^*$ (la notion de forme bilinéaire sera définie de façon générale dans IX, § 1). Toute forme linéaire $x^*$ sur $E$ peut être considérée comme l’application *partielle* $x \mapsto \langle x, x^* \rangle$ correspondant à la forme bilinéaire canonique.

Lorsque $E$ est un $A$-module *à droite*, la valeur $x^*(x)$ d’une forme linéaire $x^* \in E^*$ en un élément $x \in E$ se note $\langle x^*, x \rangle$, et les formules correspondant à (11) et (12) s’écrivent

$$
\begin{align*}
\langle x^*, x \alpha \rangle &= \langle x^*, x \rangle \alpha \\
\langle \alpha x^*, x \rangle &= \alpha \langle x^*, x \rangle.
\end{align*}
$$

Lorsque $A$ est commutatif, on peut indifféremment utiliser l’une ou l’autre notation.

#### Proposition 5 {#alg-ii-s2-prop-5 .statement}

*Pour tout anneau $A$, l’application qui, à tout $\xi \in A$, fait correspondre la forme linéaire $\eta \mapsto \eta \xi$ sur $A_s$, est un isomorphisme de $A_d$ sur le dual de $A_s$.*

C’est le cas particulier de l’isomorphisme canonique $E \to \mathrm{Hom}_A(A_s, E)$ de II, p. 35, *Remarque 2*, correspondant à $E = A_s$; la commutativité du diagramme (50) de II, p. 35, montre qu’il s’agit ici d’un isomorphisme de $A$-modules à droite.

Si on identifie $A_d$ au dual de $A_s$ au moyen de l’isomorphisme de la prop. 5, la forme bilinéaire canonique sur $A_s \times A_d$ s’explicite donc par

$$
\langle \xi, \xi^* \rangle = \xi \xi^* \qquad \text{pour } \xi, \xi^* \text{ dans } A.
$$

De même, le dual de $A_d$ s’identifie canoniquement à $A_s$, la forme bilinéaire canonique sur $A_d \times A_s$ s’explicitant par

$$
\langle \xi^*, \xi \rangle = \xi^* \xi \qquad \text{pour } \xi, \xi^* \text{ dans } A.
$$

### 4. Orthogonalité

#### Définition 3 {#alg-ii-s2-def-3 .statement}

*Soient $E$ un $A$-module, $E^*$ son dual; on dit qu’un élément $x \in E$ et un élément $x^* \in E^*$ sont orthogonaux si $\langle x, x^* \rangle = 0$.*

On dit qu’une partie $M$ de $E$ et une partie $M'$ de $E^*$ sont des *ensembles orthogonaux* si, quels que soient $x \in M,\ x^* \in M'$, $x$ et $x^*$ sont orthogonaux. En particulier, x^* \in E^* (\text{resp. } x \in E) \text{ est dit orthogonal à } M \text{ (resp. } M') \text{ s’il est orthogonal à tout élément de } M \text{ (resp. } M'). \text{ Si } x^* \text{ et } y^* \text{ sont orthogonaux à } M, \text{ il en est de même de } x^* + y^* \text{ et de } x^* \alpha \text{ pour tout } \alpha \in A \text{ en vertu de (10) et (12) (II, p. 40), ce qui justifie la définition suivante:}

#### Définition 4 {#alg-ii-s2-def-4 .statement}

*Étant donnée une partie M de E* (resp. *une partie M' de E*), on appelle sous-module totalement orthogonal à M (resp. M') (ou simplement sous-module orthogonal à M (resp. M') si aucune confusion n’en résulte) *l’ensemble des* $x^* \in E^*$ (resp. *l’ensemble des* $x \in E$) *qui sont orthogonaux à M* (resp. M').

Par définition d’une forme linéaire, le sous-module de E* orthogonal à E se réduit à 0; le sous-module de E* orthogonal à {0} est identique à E*.

#### Proposition 6 {#alg-ii-s2-prop-6 .statement}

*Soient M, N deux parties de E telles que M \subset N; si M' et N' sont les sous-modules de E* orthogonaux à M et N respectivement, on a N' \subset M'.*

#### Proposition 7 {#alg-ii-s2-prop-7 .statement}

*Soit (M_i) une famille de parties de E; le sous-module orthogonal à la réunion des M_i est l’intersection des sous-modules M'_i respectivement orthogonaux aux M_i; ce sous-module est aussi le sous-module orthogonal au sous-module de E engendré par la réunion des M_i.*

Ces résultats sont des conséquences immédiates des définitions.

On a une proposition analogue (que nous laissons au lecteur le soin d’énoncer) pour les sous-modules de E orthogonaux aux parties de E*.

Si M est un sous-module de E, M' le sous-module de E* orthogonal à M, M'' le sous-module de E orthogonal à M', on a $M \subset M''$ mais on peut avoir $M \neq M''$ (II, p. 184, exerc. 9). Notons toutefois que si M'' est l’orthogonal de M'' dans E*, on a $M''' = M'$; en effet, on a $M' \subset M''$ et d’autre part la relation $M \subset M''$ entraîne $M'' \subset M'$.

### 5. Transposée d’une application linéaire

Soient E, F deux A-modules à gauche; pour toute application linéaire $u : E \to F$, l’application $\mathrm{Hom}(u, 1_{A_s})$ est une application linéaire du A-module à droite F* dans le A-module à droite E* (II, p. 6), dite *transposée* de u.

En d’autres termes:

#### Définition 5 {#alg-ii-s2-def-5 .statement}

*Pour toute application linéaire u d’un A-module E dans un A-module F, on appelle transposée de u et on note $^t u$ l’application linéaire $y^* \mapsto y^* \circ u$ du dual F* de F dans le dual E* de E.*

La transposée $^t u$ est donc définie par la relation

$$
\langle u(x), y^* \rangle = \langle x, ^t u(y^*) \rangle \quad \text{pour tout } x \in E \text{ et tout } y^* \in F^*.
$$

La définition 5 s’applique sans changement pour des A-modules à *droite* et équivaut alors à la relation

$$
\langle y^*, u(x) \rangle = \langle ^t u(y^*), x \rangle \quad \text{pour tout } x \in E \text{ et tout } y^* \in F^*.
$$

Les formules (9) et (10) de II, p. 6 donnent ici

(16) $$ t(u_1 + u_2) = t u_1 + t u_2 $$

pour deux éléments $u_1, u_2$ de $\mathrm{Hom}_A(E, F)$, et

(17) $$ t(v \circ u) = t u \circ t v $$

pour $u \in \mathrm{Hom}_A(E, F)$ et $v \in \mathrm{Hom}_A(F, G)$, $G$ étant un troisième A-module; enfin il est clair que

(18) $$ t 1_E = 1_{E^*}. $$

#### Remarque {#alg-ii-s2-n5-rem-1 .statement}

On déduit de (17) et (18) que si $u$ est *inversible à gauche* (resp. *à droite*), $t u$ est *inversible à droite* (resp. *à gauche*).

#### Proposition 8 {#alg-ii-s2-prop-8 .statement}

Soient $u : E \to F$ une application A-linéaire, $M$ un sous-module de $E$, $M'$ l’orthogonal de $M$ dans $E^*$; l’orthogonal de $u(M)$ dans $F^*$ est l’image réciproque $t u^{-1}(M')$.

Cela résulte aussitôt de (15).

#### Corollaire {#alg-ii-s2-n5-cor-1 .statement}

L’orthogonal de l’image $u(E)$ dans $F^*$ est le noyau $t u^{-1}(0)$ de $t u$.

En effet, l’orthogonal de $E$ dans $E^*$ est réduit à 0.

Si $u : E \to F$ est un isomorphisme, $t u : F^* \to E^*$ est un isomorphisme et si $v : F \to E$ est l’isomorphisme réciproque de $u$, $t v$ est l’isomorphisme réciproque de $t u$ (formules (17) et (18)).

#### Définition 6 {#alg-ii-s2-def-6 .statement}

Étant donné un isomorphisme $u$ d’un A-module $E$ sur un A-module $F$, on appelle isomorphisme contragrédient de $u$ et on note $\check{u}$ le transposé de l’isomorphisme réciproque de $u$ (égal à l’isomorphisme réciproque du transposé de $u$).

L’isomorphisme $\check{u}$ est donc caractérisé par la relation

(19) $$ \langle u(x), \check{u}(x^*) \rangle = \langle x, x^* \rangle \quad \text{pour } x \in E, \ x^* \in E^*. $$

Si $v : F \to G$ est un isomorphisme, l’isomorphisme contragrédient de $v \circ u$ est $\check{v} \circ \check{u}$.

En particulier, l’application $u \mapsto \check{u}$ est un *isomorphisme* du groupe linéaire $\mathbf{GL}(E)$ sur un sous-groupe du groupe linéaire $\mathbf{GL}(E^*)$.

Soient $\sigma : A \to B$ un *isomorphisme* d’un anneau $A$ sur un anneau $B$, $E$ un A-module à gauche, $F$ un B-module à gauche, $u : E \to F$ une application *semi-linéaire* (II, p. 32) *relative à* $\sigma$. Soit $\sigma^{-1}$ l’isomorphisme réciproque de $\sigma$; pour tout $y^* \in F^*$, l’application $x \mapsto \langle u(x), y^* \rangle^{\sigma^{-1}}$ de $E$ dans $A$ est une *forme linéaire*; si on la désigne encore par $t u(y^*)$, on définit une application $t u : F^* \to E^*$, qu’on appelle encore la *transposée* de l’application semi-linéaire $u$; elle est donc caractérisée par l’identité

(20) $$ \langle u(x), y^* \rangle = \langle x, t u(y^*) \rangle^\sigma $$

pour $x \in E, y^* \in F^*$. On vérifie immédiatement que $^t u$ est une application semi-linéaire relativement à $\sigma^{-1}$. Si $v$ désigne l’application $u$ considérée comme application A-linéaire de $E$ dans $\sigma_*(F)$ (II, p. 32), on peut écrire $u = \varphi \circ v$, où $\varphi$ est l’application identique $\sigma_*(F) \to F$, considérée comme application semi-linéaire relative à $\sigma$. Il est immédiat que l’on a $^t u = ^t v \circ ^t \varphi$, et $(^t \varphi, \sigma^{-1})$ est un di-isomorphisme de $F_*$ sur $(\sigma_*(F))^*$, relatif à l’isomorphisme $\sigma^{-1}$; cette relation permet d’étendre aussitôt aux transposées d’applications semi-linéaires les propriétés des transposées d’applications linéaires.

### 6. Dual d’un module quotient. Dual d’une somme directe. Bases duales

Appliquons le th. 1 de II, p. 36 au cas où $F = A_s$:

#### Proposition 9 {#alg-ii-s2-prop-9 .statement}

*Soient $E', E, E''$ des A-modules,*

$$(21)$$
$$
E' \xrightarrow{u} E \xrightarrow{v} E'' \longrightarrow 0
$$
*une suite exacte d’applications linéaires.* *Alors la suite des applications transposées*
$$
0 \longrightarrow {E''}^* \xrightarrow{^t v} E^* \xrightarrow{^t u} {E'}^*
$$
*est exacte.*

#### Corollaire {#alg-ii-s2-n6-cor-1 .statement}

*Soient $M$ un sous-module d’un A-module $E$, $\varphi : E \to E/M$ l’homomorphisme canonique. Alors $^t \varphi$ est un isomorphisme du dual de $E/M$ sur le sous-module $M'$ de $E^*$ orthogonal à $M$.*

En effet, si $j : M \to E$ est l’injection canonique, le noyau de $^t j$ est par définition l’orthogonal de $M$ dans $E^*$.

En outre, avec les notations du corollaire, on obtient par passage au quotient à partir de $^t j$ un homomorphisme *injectif* $E^*/M' \to M^*$.

#### Proposition 10 {#alg-ii-s2-prop-10 .statement}

*Soit $(E_i)_{i \in I}$ une famille de A-modules, et pour tout $i \in I$, soit $j_i : E_i \to E = \bigoplus_{i \in I} E_i$ l’injection canonique. Alors l’application produit $x^* \mapsto (j_i(x^*))$ est un isomorphisme du dual $E^*$ de $E$ sur le produit $\prod_{i \in I} E_i^*$.*

C’est un cas particulier de II, p. 13, cor. 1, appliqué au cas où $\prod_\lambda F_\lambda = A_s$.

Si, au moyen des injections canoniques $j_i$, on identifie les $E_i$ à des sous-modules de leur somme directe $E$, et si, au moyen de l’application produit $x^* \mapsto (j_i(x^*))$, on identifie $E^*$ à $\prod_{i \in I} E_i^*$, on peut donc dire que $\prod_{i \in I} E_i^*$ est *le dual de* $\bigoplus_{i \in I} E_i$, la forme bilinéaire canonique étant donnée par

$$(22)$$
$$
\langle (x_i), (x_i^*) \rangle = \sum_{i \in I} \langle x_i, x_i^* \rangle.
$$

#### Corollaire {#alg-ii-s2-n6-cor-2 .statement}

Soient M, N deux sous-modules supplémentaires dans un A-module E, $p : E \to M, q : E \to N$ les projecteurs correspondants; alors $^t p + ^t q : M^* \oplus N^* \to E^*$ est un isomorphisme, et $^t p$ (resp. $^t q$) est un isomorphisme de $M^*$ (resp. $N^*$) sur le sous-module de $E^*$ orthogonal à N (resp. M). En outre, si $i : M \to E$ et $j : N \to E$ sont les injections canoniques, $^t p \circ ^t i$ et $^t q \circ ^t j$ sont les projecteurs $E^* \to ^t p(M^*)$, $E^* \to ^t q(N^*)$ correspondant à la décomposition de $E^*$ en somme directe de $^t p(M^*)$ et $^t q(N^*)$.

On a en effet $p \circ i = 1_M$, $q \circ j = 1_N$, $p \circ j = q \circ i = 0$, $i \circ p + j \circ q = 1_E$, d’où, par transposition (II, p. 43, formules (16), (17) et (18)), $^t i \circ ^t p = 1_{M^*}$, $^t j \circ ^t q = 1_{N^*}$, $^t j \circ ^t p = ^t i \circ ^t q = 0$, $^t p \circ ^t i + ^t q \circ ^t j = 1_{E^*}$, et la proposition résulte de II, p. 13, cor. 2.

Sous les hypothèses du corollaire, on identifie souvent $M^*$ (resp. $N^*$) à l’orthogonal $^t p(M^*)$ (resp. $^t q(N^*)$) de N (resp. M) dans $E^*$, en identifiant donc toute forme linéaire $u$ sur M (resp. N) à la forme linéaire sur E prolongeant $u$ et qui s’annule dans N (resp. M).

Lorsqu’un A-module E admet une base $(e_t)_{t \in T}$, on a vu que la donnée de cette base définit canoniquement un isomorphisme $u : A_s^{(T)} \to E$. En vertu de la prop. 10 et de II, p. 41, prop. 5, le dual de $A_s^{(T)}$ s’identifie canoniquement au produit $A_d^T$; considérons l’isomorphisme contragrédient $\tilde{u} : A_d^T \to E^*$. Si, pour tout $t \in T$, $f_t$ est l’élément de $A_d^T$ dont toutes les projections sont nulles sauf celle d’indice $t$, qui est égale à 1, et si on pose $e_t^* = \tilde{u}(f_t)$, les éléments $e_t^*$ de $E^*$ sont, en vertu de (19) (II, p. 43) et (22) (II, p. 44), caractérisés par les relations

$$
\langle e_t, e_{t'}^* \rangle = \begin{cases}
0 & \text{pour } t' \neq t. \\
1 & \text{pour } t' = t.
\end{cases}
$$

Il revient au même de dire que, pour tout $x = \sum_{t \in T} \xi_t e_t \in E$, on a $e_t^*(x) = \xi_t$; aussi dit-on que $e_t^*$ est la forme coordonnée d’indice $t$ sur E. Il résulte de (23) que $(e_t^*)$ est un système libre dans $E^*$.

En particulier, si T est fini, les $e_t^*$ forment une base de $E^*$, les $f_t$ formant alors la base canonique de $A_d^T$. Donc:
PROPOSITION 11. — Le dual d’un module libre ayant une base de n éléments est un module libre ayant une base de n éléments.

On notera que le dual d’un module libre ayant une base infinie n’est pas nécessairement un module libre (VII, § 3, exerc. 10).

#### Définition 7 {#alg-ii-s2-def-7 .statement}

Si E est un module libre ayant une base finie $(e_t)$, on appelle base duale de $(e_t)$ la base $(e_t^*)$ du dual $E^*$ de E définie par les relations (23).

On écrit aussi les relations (23) sous la forme
$$
\langle e_t, e_{t'}^* \rangle = \delta_{tt'}
$$
où $\delta_{tt'}$ est le symbole de Kronecker sur $T \times T$.

On notera que si T est fini et $(e_t^*)$ la base duale de $(e_t)$, on a, pour $x = \sum_{t \in T} \xi_t e_t \in E$, $x^* = \sum_{t \in T} \xi_t^* e_t^* \in E^*$,

$$
\langle x, x^* \rangle = \sum_{t \in T} \xi_t \xi_t^*.
$$

On définit bien entendu de la même manière la base duale d’une base finie d’un A-module à droite.

#### Corollaire {#alg-ii-s2-n6-cor-3 .statement}

*Le dual d’un module projectif de type fini est un module projectif de type fini.*

En effet, un A-module à gauche projectif de type fini peut être identifié à un facteur direct M d’un A-module libre $A_s^n$ ayant une base finie (II, p. 40, cor. 1). Alors (II, p. 45, prop. 11 et corollaire) M* est isomorphe à un facteur direct de $A_d^n$, d’où le corollaire.

#### Proposition 12 {#alg-ii-s2-prop-12 .statement}

*Soient E un A-module, $(a_t)_{t \in T}$ un système générateur de E. Les conditions suivantes sont équivalentes*:

a) *E est un A-module projectif*.

b) *Il existe une famille $(a_t^*)_{t \in T}$ de formes linéaires sur E telles que, pour tout $x \in E$, la famille $(\langle x, a_t^* \rangle)_{t \in T}$ ait un support fini et que l’on ait*

$$
x = \sum_{t \in T} \langle x, a_t^* \rangle a_t.
$$

Il existe un homomorphisme surjectif $u : L \to E$ où $L = A_s^{(T)}$, tel que, si $(e_t)_{t \in T}$ est la base canonique de L, on ait $u(e_t) = a_t$ (II, p. 24, prop. 17); pour que E soit projectif, il faut et il suffit qu’il existe une application linéaire $v : E \to L$ telle que $u \circ v = 1_E$ (II, p. 39, prop. 4 et II, p. 20, prop. 15). Si une telle application existe et si l’on pose $^t v(e_t^*) = a_t^*$, on a $\langle x, a_t^* \rangle = \langle x, ^t v(e_t^*) \rangle = \langle v(x), e_t^* \rangle$, donc la famille $(\langle x, a_t^* \rangle)$ a un support fini et l’on a $x = u \left( \sum_{t \in T} \langle v(x), e_t^* \rangle e_t \right) = \sum_{t \in T} \langle x, a_t^* \rangle a_t$ pour tout $x \in E$. Inversement, si la condition b) de l’énoncé est remplie, la somme $\sum_{t \in T} \langle x, a_t^* \rangle e_t$ est définie pour tout $x \in E$, et $x \mapsto \sum_{t \in T} \langle x, a_t^* \rangle e_t$ est une application linéaire $v : E \to L$ telle que $u \circ v = 1_E$.

### 7. Bidual

Soit E un A-module à gauche. Le dual E** du dual E* de E est appelé le *bidual* de E; c’est encore un A-module à gauche (II, p. 40). Pour tout $x \in E$, il résulte de II, p. 41, formules (10) et (12), que l’application $x^* \mapsto \langle x, x^* \rangle$ est une *forme linéaire* sur le A-module à droite E*, autrement dit un élément du bidual E**, que nous noterons $\tilde{x}$; en outre, on déduit aussitôt de (9) et (11) (II, p. 41) que l’application $c_E : x \mapsto \tilde{x}$ de E dans E** est *linéaire*; cette application sera dite canonique; en général, elle n’est ni injective ni surjective, même lorsque E est de type fini (cf. II, p. 184, exerc. 9e) et II, p. 103, th. 6).

On dit qu’un A-module E est réflexif si l’homomorphisme canonique $c_E : E \to E^{**}$ est bijectif.

Soit F un second A-module à gauche; pour toute application linéaire $u : E \to F$, l’application $^t(tu) : E^{**} \to F^{**}$, que nous écrirons aussi $^{tt}u$, est linéaire, et le diagramme

$$
\begin{array}{ccc}
E & \xrightarrow{u} & F \\
c_E \downarrow & & \downarrow c_F \\
E^{**} & \xrightarrow{^{tt}u} & F^{**}
\end{array}
$$

est commutatif, comme il résulte aussitôt des définitions et de la formule (15) (II, p. 42) donnant la transposée d’une application linéaire.

#### Proposition 13 {#alg-ii-s2-prop-13 .statement}

*Si E est un module libre* (resp. *un module libre ayant une base finie*), *l’application canonique* $c_E : E \to E^{**}$ *est injective* (resp. *bijective*).

En effet, soit $(e_t)_{t \in T}$ une base de E, et soit $(e_t^*)$ la famille des formes coordonnées correspondantes; par définition, si $x \in E$ est tel que $\tilde{x} = 0$, on a $\langle x, e_t^* \rangle = 0$ pour tout $t \in T$, autrement dit, toutes les coordonnées de $x$ sont nulles, donc $x = 0$. Supposons de plus T fini; puisque $\langle \tilde{e}_t, e_{t'}^* \rangle = \delta_{tt'}$, $(\tilde{e}_t)$ est la base duale de $(e_t^*)$ dans $E^{**}$, et comme $c_E$ transforme une base de E en une base de $E^{**}$, $c_E$ est bijective (II, p. 25, cor. 3). On a en outre prouvé:

#### Corollaire 1 {#alg-ii-s2-prop-13-cor-1 .statement}

*Soit E un A-module libre ayant une base finie; pour toute base* $(e_t)$ *de E, $(c_E(e_t))$ est la base duale de la base* $(e_t^*)$ *de* $E^*$, *duale de* $(e_t)$.

On dit dans ce cas que $(e_t)$ et $(e_t^*)$ sont deux bases *duales l’une de l’autre*.

#### Corollaire 2 {#alg-ii-s2-prop-13-cor-2 .statement}

*Si E est un A-module libre ayant une base finie, toute base finie de* $E^*$ *est la base duale d’une base de* E.

Il suffit en effet de considérer dans $E^{**}$ la base duale de la base donnée et d’identifier canoniquement E et $E^{**}$.

#### Corollaire 3 {#alg-ii-s2-prop-13-cor-3 .statement}

*Soient E, F deux A-modules ayant chacun une base finie, E (resp. F) étant canoniquement identifié à son bidual* $E^{**}$ *resp. F**). *Pour toute application linéaire* $u : E \to F$, *on a alors* $^{tt}u = u$.

Cela résulte aussitôt de la commutativité du diagramme (27).

#### Corollaire 4 {#alg-ii-s2-prop-13-cor-4 .statement}

*Si P est un module projectif* (resp. *un module projectif de type fini*) *l’application canonique* $c_P : P \to P^{**}$ *est injective* (resp. *bijective*).

Nous utiliserons le lemme suivant:

#### Lemme 1 {#alg-ii-s2-lem-1 .statement}

*Soient M, N deux sous-modules supplémentaires dans un A-module* E, $i : M \to E, j : N \to E$ *les injections canoniques. Alors le diagramme* (28)

$$
\begin{array}{ccc}
M \oplus N & \xrightarrow{c_M \oplus c_N} & M^{**} \oplus N^{**} \\
i+j \downarrow & & \downarrow tti + ttj \\
E & \xrightarrow{c_E} & E^{**}
\end{array}
$$

est commutatif.

En effet, par définition, pour $x \in M, y \in N, z^* \in E^*$

$$
\begin{align*}
\langle c_E(i(x) + j(y)), z^* \rangle &= \langle i(x) + j(y), z^* \rangle \\
&= \langle i(x), z^* \rangle + \langle j(y), z^* \rangle \\
&= \langle x, {}^t i(z^*) \rangle + \langle y, {}^t j(z^*) \rangle \\
&= \langle c_M(x), {}^t i(z^*) \rangle + \langle c_N(y), {}^t j(z^*) \rangle \\
&= \langle {}^{tt} i(c_M(x)) + {}^{tt} j(c_N(y)), z^* \rangle.
\end{align*}
$$

Cela étant, si E est un module libre (resp. un module libre ayant une base finie), $c_E$ est injectif (resp. bijectif); d’autre part, il résulte de II, p. 44, prop. 10, que ${}^{tt} i \oplus {}^{tt} j$ est bijectif; la commutativité du diagramme (28) entraîne alors que $c_M \oplus c_N$ est injectif (resp. bijectif), et il en est donc de même de $c_M$ et $c_N$ (II, p. 14, cor. 1), d’où le corollaire, compte tenu de II, p. 39, prop. 4.

### 8. Équations linéaires

Soient E, F deux A-modules. Toute équation de la forme $u(x) = y_0$, où $u : E \to F$ est une application linéaire donnée, $y_0$ un élément donné de F et où l’inconnue $x$ est assujettie à prendre ses valeurs dans E, s’appelle équation linéaire; on dit que $y_0$ est le second membre de l’équation; si $y_0 = 0$, l’équation est dite linéaire et homogène.

Tout élément $x_0 \in E$ tel que $u(x_0) = y_0$ est appelé solution de l’équation linéaire $u(x) = y_0$.¹

On dit souvent, de façon imagée, qu’un problème est linéaire s’il est équivalent à la détermination des solutions d’une équation linéaire.

Étant donnée une équation linéaire $u(x) = y_0$, l’équation $u(x) = 0$ est appelée l’équation linéaire et homogène associée à $u(x) = y_0$.

#### Proposition 14 {#alg-ii-s2-prop-14 .statement}

Si $x_0$ est une solution de l’équation linéaire $u(x) = y_0$, l’ensemble des solutions de cette équation est égal à l’ensemble des éléments $x_0 + z$, où $z$ parcourt l’ensemble des solutions de l’équation homogène associée $u(x) = 0$.

En effet, la relation $u(x) = y_0$ s’écrit $u(x) = u(x_0)$, équivalente à $u(x - x_0) = 0$.

¹ Il s’agit en fait d’un abus de langage; du point du vue logique, nous ne définissons pas ici le mot « solution », mais simplement la phrase « $x_0$ est solution de l’équation $u(x) = y_0$ » comme équivalente à la relation « $x_0 \in E$ et $u(x_0) = y_0$ ». On observera que dans une théorie mathématique $\mathcal{T}$ où la relation « A est un anneau, E et F des A-modules, u un homomorphisme de E dans F, $y_0$ un élément de F » est un théorème, tout terme $T$ de $\mathcal{T}$ tel que la relation « $T \in E$ et $u(T) = y_0$ » soit vraie dans $\mathcal{T}$ est une solution de l’équation $u(x) = y_0$ au sens de E, I, p. 40; ce qui justifie l’abus de langage précédent.

Autrement dit, si l’équation $u(x) = y_0$ a au moins une solution $x_0$, l’ensemble de ses solutions est l’ensemble $x_0 + \overline{u}^1(0)$, obtenu par translation à partir du noyau $\overline{u}^1(0)$ de $u$. On observera que $\overline{u}^1(0)$, étant un sous-module, n’est jamais vide, puisqu’il contient 0 (appelé la solution nulle, ou solution banale, de l’équation homogène $u(x) = 0$).

En vertu de la prop. 14, pour qu’une équation $u(x) = y_0$ ait exactement une solution, il faut et il suffit qu’elle ait au moins une solution, et que l’on ait $\overline{u}^1(0) = \{0\}$ (autrement dit, que l’équation homogène associée n’ait pas de solution non nulle, ou encore que $u$ soit injective); dans ce cas, pour tout $y \in F$, l’équation $u(x) = y$ a au plus une solution.

#### Proposition 15 {#alg-ii-s2-prop-15 .statement}

*Soit u une application linéaire d’un module E dans un module F. Si l’équation $u(x) = y_0$ a au moins une solution, $y_0$ est orthogonal au noyau de $^t u$.*

En effet, dire que $u(x) = y_0$ admet une solution signifie que $y_0 \in u(E)$ et la proposition résulte de II, p. 43, corollaire.

On observera que le critère nécessaire d’existence d’une solution de $u(x) = y_0$, donné par la prop. 15, est suffisant lorsque A est un corps (II, p. 106, prop. 12) mais *non en général* (II, p. 184, exerc. 10).

#### Remarque 1 {#alg-ii-s2-n8-rem-1 .statement}

Soient E un A-module, $(F_i)_{i \in I}$ une famille de A-modules, et pour tout $i \in I$, soit $u_i : E \to F_i$ une application linéaire. Tout système d’équations linéaires
$$
u_i(x) = y_i \quad (i \in I)
$$
où les $y_i \in F_i$ sont donnés, est équivalent à *une seule* équation linéaire $u(x) = y$, où $u$ est l’application $x \mapsto (u_i(x))$ de E dans $F = \prod_{i \in I} F_i$, et $y = (y_i)$. On dit que le système (29) est *homogène* si $y_i = 0$ pour tout $i \in I$.

#### Remarque 2 {#alg-ii-s2-n8-rem-2 .statement}

Supposons que E admette une *base* $(a_\lambda)_{\lambda \in L}$; si on pose $u(a_\lambda) = b_\lambda$ pour tout $\lambda \in L$, dire que $x = \sum_{\lambda \in L} \xi_\lambda a_\lambda$ vérifie l’équation $u(x) = y_0$ équivaut à dire que la famille (de support fini) $(\xi_\lambda)_{\lambda \in L}$ d’éléments de A vérifie la relation
$$
\sum_{\lambda \in L} \xi_\lambda b_\lambda = y_0.
$$
Inversement, la recherche des familles $(\xi_\lambda)_{\lambda \in L}$ d’éléments de A, de support fini, vérifiant (30), équivaut à la résolution de l’équation linéaire $u(x) = y_0$, où $u$ est l’unique application linéaire de E dans F telle que $u(a_\lambda) = b_\lambda$ pour tout $\lambda \in L$ (II, p. 25, cor. 3).

#### Remarque 3 {#alg-ii-s2-n8-rem-3 .statement}

Une équation linéaire $u(x) = y_0$ est dite *scalaire* lorsque $F = A_s$, et par suite $u$ est une *forme linéaire* sur E et $y_0$ un *scalaire*. Si E admet une base $(a_\lambda)_{\lambda \in L}$, il résulte de la *Remarque 2*) qu’une telle équation s’écrit aussi
$$
\sum_{\lambda \in L} \xi_\lambda \alpha_\lambda = y_0 \in A
$$
où la famille de scalaires $(\alpha_\lambda)$ est arbitraire, et où il est sous-entendu que la famille $(\xi_\lambda)$ doit avoir un support fini. De façon générale, par *solution* (dans A) d’un système d’équations linéaires scalaires
$$
\sum_{\lambda \in L} \xi_\lambda \alpha_{\lambda i} = \eta_i \quad (i \in I)
$$
où $\alpha_{\lambda i} \in A$ et $\eta_i \in A$ sont arbitraires, on entend une famille $(\xi_\lambda)_{\lambda \in L}$ d’éléments de A, de support *fini*, et vérifiant (32); les $\alpha_{\lambda i}$ sont dits les *coefficients* du système d’équations, et les $\eta_l$ les seconds membres. La résolution d’un tel système est équivalente à celle de l’équation $u(x) = y$, où $y = (\eta_l)$ et $u : A_s^{(L)} \to A_s^l$ est l’application linéaire
$$
(\xi_\lambda) \mapsto \left( \sum_{\lambda \in L} \xi_\lambda \alpha_{\lambda l} \right).
$$

#### Remarque 4 {#alg-ii-s2-n8-rem-4 .statement}

Un système linéaire (32) est encore appelé système d’équations linéaires scalaires à gauche lorsqu’il y a lieu d’éviter des confusions. Un système d’équations
$$
\sum_{\lambda \in L} \alpha_{\lambda l} \xi_\lambda = \eta_l \qquad (l \in I)
$$
est de même appelé système d’équations linéaires scalaires à droite; un tel système se ramène aussitôt à un système (32) en considérant les $\xi_\lambda, \eta_l$ et $\alpha_{\lambda l}$ comme appartenant à l’anneau $A^0$ opposé à $A$.

## EXERCICES {#alg-ii-s2-exercises}

See the [exercises for § 2](exercises/s2/).
