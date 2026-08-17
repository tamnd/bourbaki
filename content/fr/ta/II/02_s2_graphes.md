---
book: ta
book_title: Topologie algébrique
chapter: II
chapter_title: GROUPOÏDES
section: 2
section_title: Graphes
lang: fr
source: ta-i-iv-fr
book_pages: TA II.155-TA II.159, TA II.219-TA II.223
pdf_pages: 0171-0175, 0235-0239
extraction: native
subsections:
    - "no": 1
      title: Définition d’un graphe
      page: 155
      pdf_page: 171
    - "no": 2
      title: Orientation d’un graphe
      page: 156
      pdf_page: 172
    - "no": 3
      title: Graphes orientés et carquois
      page: 156
      pdf_page: 172
    - "no": 4
      title: Arbres
      page: 157
      pdf_page: 173
statements: 5
exercises: 12
content_sha256: 7b11f57105325047d7638e4ccda232addd1076f464d3da18b009dc079cf93bf9
---

## § 2. GRAPHES

### 1. Définition d’un graphe

#### Définition 1 {#ta-ii-s2-def-1 .statement tag=01SU}

Un graphe[^1] est un carquois $(S,F, o, t)$ muni d’une involution de F, notée $f\mapsto \overline{f}$, sans point fixe et telle que $t(\overline{f}) =o(f)$ pour tout $f\in F$.

Le carquois $(S,F, o, t)$ est dit sous-jacent à ce graphe. Pour toute flèche $f$ de ce carquois, on a, par définition, $\overline{f}=f,\overline{f}=\not f$ et $t(\overline{f}) =$ $o(f)$. En appliquant cette dernière relation à la flèche $\overline{f}$, on obtient l’égalité $o(\overline{f}) =t(f)$. La flèche $\overline{f}$ s’appelle la flèche opposée à $f$.

Une paire de flèches opposées du graphe s’appelle une arête du graphe. Chacune des deux flèches appartenant à cette paire s’appelle une orientation de cette arête. Pour cette raison, les flèches d’un graphe sont également appelées les arêtes orientées du graphe.

Si G et $G'$ sont des graphes, un morphisme de graphes de G dans $G'$ est un morphisme de carquois $\varphi : G\rightarrow G'$ tel que $\varphi (f) =\varphi (\overline{f})$ pour toute flèche $f$ de G.

Soient G et $G'$ des graphes ; on dit que $G'$ est un sous-graphe de G si c’en est un sous-carquois et si l’involution de Fl(G$')$ est la restriction de celle de Fl(G).

### 2. Orientation d’un graphe

Soit G un graphe. Une orientation de G est une partie A de l’ensemble des flèches de G telle que $A\cap A =\emptyset$ et $A\cup A =$ Fl(G).

Un graphe muni d’une orientation est appelé graphe orienté.

Soit G un graphe orienté et soit A son orientation ; un sous-graphe orienté de G est un sous-graphe $G'$ de G muni de l’orientation $A'=$ Fl(G$')\cap A$.

Soient $(G,A)$ et $(G',A')$ des graphes orientés. Un morphisme de graphes orientés de $(G,A)$ dans $(G',A')$ est un morphisme de graphes $\varphi : G\rightarrow G'$ tel que Fl($\varphi$ )$(A)\subset A'$.

### 3. Graphes orientés et carquois

Soient G un graphe, $(S,F, o, t)$ le carquois sous-jacent, et A une orientation de G. Alors, $(S,A, o|A, t|A)$ est un carquois, appelé le carquois associé au graphe orienté $(G,A)$.

Inversement, soit $C = (S,F, o, t)$ un carquois. Posons $\widetilde{F} = F\times \{-1,1\}$ et soient $\widetilde{o},\widetilde{t}$ les applications de $\widetilde{F}$ dans S définies par

$$
\widetilde{o}(f,1) =o(f)\widetilde{o}(f,-1) =t(f)
$$

$$
\widetilde{t}(f,1) =t(f)\widetilde{t}(f,-1) =o(f)
$$

pour $f\in F$. Alors, $\widetilde{C} = (S,\widetilde{F},\widetilde{o},\widetilde{t})$, muni de l’involution $(f, \varepsilon )\mapsto (f,-\varepsilon )$ de $\widetilde{F}$ est un graphe, appelé le graphe associé au carquois C. L’ensemble $A = F\times  \{1\}$ est une orientation de ce graphe. On dit que $(\widetilde{C},A)$ est le graphe orienté associé au carquois C.

Si $f$ est une flèche de C, on dit aussi que $(f,1)$ est l’arête orientée de $\widetilde{C}$ associée à $f$ et que la paire $\{(f,1),(f,-1)\}$ est l’arête de $\widetilde{C}$ associée à $f$.

Si $C'$ est un sous-carquois de C, le graphe orienté $\widetilde{C}'$ est un sous-graphe orienté de $\widetilde{C}$.

Il existe un unique morphisme de carquois $\varphi$ de C dans le carquois sous-jacent à $\widetilde{C}$ tel que $\varphi (f) = (f,1)$ pour toute flèche $f$ de G ; c’est un isomorphisme de C sur le carquois associé au graphe orienté $(\widetilde{C},A)$.

### 4. Arbres

Lorsqu’on parle de chemins, ou de composantes connexes, d’un graphe, il s’agit des chemins ou des composantes connexes du carquois sous-jacent. Deux sommets d’un graphe appartiennent à une même composante connexe si et seulement s’il existe un chemin qui les relie.

Soit G un graphe. Si $c= (a_0, f_1, a_1, . . . , f_n, a_n)$ est un chemin dans G, la suite $\overline{c}= (a_n, f_n, . . . , a_1, f_1, a_0)$ est un chemin dans G, appelé chemin opposé à $c$. Soient $c$ et $c'$ des chemins juxtaposables dans G ; alors, $\overline{c'}$ et $\overline{c}$ sont juxtaposables et l’on a $\overline{c*c'}=\overline{c'}*\overline{c}$.

Un chemin $c$ dans G est dit sans aller-retour s’il n’existe aucune paire de flèches consécutives de $c$ qui soient opposées. Soit $c= (a_0, f_1, . . . , f_n, a_n)$ un chemin dans G reliant $a_0$ et $a_n$. Si, pour un entier $i$ tel que $1\leqslant i < n$, les flèches $f_i$ et $f_{i+1}$ sont opposées, le chemin $(a_0, f_1, . . . , a_{i-1}, f_{i+2}, . . . , f_n, a_n)$ est un chemin dans G reliant $a_0$ à $a_n$ dont la longueur est strictement inférieure à celle du chemin $c$. Par récurrence, il existe donc un chemin sans aller-retour dans G qui relie $a_0$ à $a_n$.

#### Définition 2 {#ta-ii-s2-def-2 .statement tag=01SV}

Une forêt est un graphe dans lequel tout lacet sans aller-retour est un lacet constant. Un arbre est une forêt connexe.

#### Proposition 1 {#ta-ii-s2-prop-1 .statement tag=01SW}

Soit G un graphe. Toute forêt de G est contenue dans une forêt maximale de G ; en particulier, il existe une forêt maximale de G.

Pour qu’une forêt de G soit maximale, il faut et il suffit que l’ensemble de ses sommets soit égal à l’ensemble des sommets de G et que ses composantes connexes soient celles de G.

Soit $A_0$ une forêt de G. L’ensemble des forêts de G, muni de la relation d’ordre « A est un sous-graphe de B » est inductif. Il existe par conséquent une forêt maximale de G dont $A_0$ est un sous-graphe (E, III, p. 21, cor. 1).

Le sous-graphe de G dont l’ensemble des sommets est Som(G) et dont l’ensemble des flèches est vide est une forêt de G. Il existe donc une forêt maximale de G.

Soit A une forêt maximale de G. Démontrons que A et G ont même ensemble de sommets. Le sous-graphe de G dont l’ensemble des sommets est Som(G) et dont l’ensemble des flèches est Fl(A) est une forêt et A en est un sous-graphe. On a donc Som(A) = Som(G).

Démontrons maintenant que A et G ont mêmes composantes connexes. Comme une flèche de A est une flèche de G, toute composante connexe de A est contenue dans une composante connexe de G. Comme A et G ont même ensemble de sommets, il suffit de démontrer que deux sommets de G qui sont dans une même composante connexe de G sont dans une même composante connexe de A. Si ce n’est pas le cas, la relation $R_A$, « être dans la même composante connexe de A », est strictement plus fine que la relation $R_G$, et il existe deux sommets de G qui ne sont pas dans la même composante connexe de A mais qui sont néanmoins reliés par une flèche $f$ de G. Soit B le sous-graphe orienté de G dont l’ensemble des sommets est Som(G) et dont l’ensemble des flèches est Fl(A) $\cup  \{f, f\}$; démontrons que B est une forêt de G. Soit $c= (a_0, f_1, . . . , f_n, a_n)$ un lacet non constant sans aller-retour dans B de longueur minimale. Comme A est une forêt, le lacet $c$ n’est pas un lacet dans A. Soit $i$ (resp. $j)$ le plus petit (resp. le plus grand) entier de $\{0, . . . , n\}$ tel que $a_0$ et $a_i$ (resp. $a_j$ et $a_n)$ ne soient pas dans la même composante connexe de A. Cela signifie que les flèches $f_i$ et $f_{j+1}$ sont des flèches orientées de B associées à l’arête $\{f, f\}$ et qu’elles sont opposées. Comme le lacet $c$ est sans aller-retour, $f_{i+1}=\not\overline{f_i}$, donc $i=\not j$ et le chemin $(a_i, f_{i+1}, a_{i+1}, . . . , f_j, a_j)$ est un lacet sans aller-retour non constant dans B de longueur $< n$, contrairement à l’hypothèse que $c$ est de longueur minimale. Il en résulte que B est une forêt. Ceci contredit l’hypothèse que A est une forêt maximale de G.

Soit maintenant une forêt A de G telle que Som(A) = Som(G) et $\pi_0(A) =\pi_0(G)$; démontrons que c’est une forêt maximale de G. Il suffit de prouver que, si $f\notin$ Fl(A), le sous-graphe B de G d’ensemble de sommets Som(G) et d’ensemble de flèches Fl(A) $\cup  \{f, f\}$ n’est pas une forêt. Par hypothèse, les points $o(f)$ et $t(f)$ sont dans la même composante connexe de A ; il existe donc un chemin $c$ sans aller-retour dans A qui relie $o(f)$ à $t(f)$. Le chemin $c*\overline{f}$ est alors un lacet sans aller-retour et non constant dans B, ce qui montre que B n’est pas une forêt orientée.

#### Corollaire {#ta-ii-s2-n4-cor-1 .statement tag=01SX}

Une forêt maximale d’un graphe connexe en est un arbre maximal.

#### Remarque 1 {#ta-ii-s2-n4-rem-1 .statement tag=01SY}

On a défini dans LIE, IV, p. 33, annexe, la notion de graphe combinatoire comme un couple $(A,S)$, où S est un ensemble et A une partie de $\mathfrak{P}(S)$ formée d’ensembles à deux éléments ; les éléments de S s’appellent des sommets, ceux de A des arêtes, on dit que deux sommets $x$ et $y\in S$ sont liés si $\{x, y\}$ est une arête.

À un tel graphe combinatoire $\Gamma  = (A,S)$, on associe un graphe G dont l’ensemble des sommets est S et dont l’ensemble des flèches $\widetilde{A}$ est la partie de $S^2$ formée des couples de sommets liés, l’application origine et l’application terme coïncidant avec la première et la seconde projection de $S^2$ dans S, et l’involution $f\mapsto \overline{f}$ étant donnée par la restriction à $\widetilde{A}$ de l’application $(x, y)\mapsto (y, x)$ de $S^2$ dans lui-même. L’application qui à une arête $\{f, f\}$ de G associe l’ensemble $\{o(f), t(f)\}$ est une bijection de l’ensemble des arêtes de G sur celui des arêtes du graphe combinatoire Γ.

Inversement, tout graphe tel que l’origine et le terme de toute flèche soient distinctes, et tel qu’une flèche soit déterminée par son origine et son terme est de cette forme.

Le lecteur vérifiera que les notions de connexité, d’arbre, ou de forêt pour un graphe combinatoire coïncident avec les notions correspondantes pour le graphe qui lui est associé.

## EXERCICES {#ta-ii-s2-exercises}

See the [exercises for § 2](exercises/s2/).

[^1]: On prendra garde à ne pas confondre la notion de graphe introduite ici avec celle de E, II, §3, n$^o1$.
