---
book: alg
book_title: Algebra
chapter: III
chapter_title: ALGÈBRES TENSORIELLES, ALGÈBRES EXTÉRIEURES, ALGÈBRES SYMÉTRIQUES
section: 4
section_title: Produits tensoriels d’algèbres
lang: fr
source: alg-i-iii-fr
book_pages: A III.33-A III.55, A III.183-A III.184
pdf_pages: 0420-0442, 0570-0571
extraction: ocr
subsections:
    - "no": 1
      title: Produit tensoriel d’une famille finie d’algèbres
      page: 33
      pdf_page: 420
    - "no": 2
      title: Caractérisation universelle des produits tensoriels d’algèbres
      page: 36
      pdf_page: 423
    - "no": 3
      title: Modules et multimodules sur les produits tensoriels d’algèbres
      page: 38
      pdf_page: 425
    - "no": 4
      title: Produit tensoriel d’algèbres sur un corps
      page: 40
      pdf_page: 427
    - "no": 5
      title: Produit tensoriel d’une famille infinie d’algèbres.
      page: 42
      pdf_page: 429
    - "no": 6
      title: Lemmes de commutation
      page: 44
      pdf_page: 431
    - "no": 7
      title: Produit tensoriel d’algèbres graduées relativement à des facteurs de commutation
      page: 46
      pdf_page: 433
    - "no": 8
      title: Produit tensoriel d’algèbres graduées de mêmes types
      page: 51
      pdf_page: 438
    - "no": 9
      title: Algèbres anticommutatives et algèbres alternées
      page: 53
      pdf_page: 440
statements: 47
exercises: 2
content_sha256: 59645096ae90f853ea564641855a3e82cc91f3c460007a1723aae13682f0c924
---

## § 4. PRODUITS TENSORIELS D’ALGÈBRES

*Du § 4 au § 8 inclus, A désigne un anneau commutatif, et sauf mention expresse du contraire, les algèbres considérées sont supposées associatives et unifères, et les homomorphismes d’algèbres sont supposés unifères.*

### 1. Produit tensoriel d’une famille finie d’algèbres

On désigne toujours par A un anneau commutatif. Soit $(E_i)_{i \in I}$ une famille \emph{finie} de A-algèbres, et soit $E = \bigotimes_{i \in I} E_i$ le A-module produit tensoriel des A-modules $E_i$ (II, p. 71). On va définir sur E une structure de A-\emph{algèbre}. Soit $m_i : E_i \otimes_A E_i \to E_i$ l’application A-linéaire qui définit la multiplication dans $E_i$ (III, p. 5). Considérons l’application A-linéaire

$$
m' = \bigotimes_{i \in I} m_i : \bigotimes_{i \in I} (E_i \otimes_A E_i) \to \bigotimes_{i \in I} E_i = E;
$$

l’application composée

$$
(\bigotimes_{i \in I} E_i) \otimes_A (\bigotimes_{i \in I} E_i) \xrightarrow{\tau} \bigotimes_{i \in I} (E_i \otimes_A E_i) \xrightarrow{m'} \bigotimes_{i \in I} E_i
$$

où $\tau$ est l’isomorphisme d’associativité (II, p. 72) est une application A-linéaire $m : E \otimes_A E \to E$; nous allons voir que $m$ définit sur E une structure d’algèbre (associative et unifère). En effet, si on explicite la multiplication définie par $m$, on obtient la formule

(1)
$$
(\bigotimes_{i \in I} x_i)(\bigotimes_{i \in I} y_i) = \bigotimes_{i \in I} (x_i y_i) \quad \text{pour } x_i, y_i \text{ dans } E_i \text{ et } i \in I.
$$

On voit donc déjà, par linéarité, que si $e_i$ est l’élément unité de $E_i$, $e = \bigotimes_{i \in I} e_i$ est élément unité de E. D’autre part, l’associativité de chacune des $E_i$ entraîne la relation

$$
((\bigotimes_{i \in I} x_i)(\bigotimes_{i \in I} y_i))(\bigotimes_{i \in I} z_i) = \bigotimes_{i \in I} (x_i y_i z_i) = (\bigotimes_{i \in I} x_i)((\bigotimes_{i \in I} y_i)(\bigotimes_{i \in I} z_i))
$$

d’où, par linéarité, la relation $x(yz) = (xy)z$ quels que soient $x, y, z$ dans E.

#### Définition 1 {#alg-iii-s4-def-1 .statement}

Etant donnée une famille finie $(E_i)_{i \in I}$ d’algèbres sur $A$, on appelle produit tensoriel de cette famille, et on note $\bigotimes_{i \in I} E_i$ (ou, lorsque $I$ est l’intervalle $[1, n]$ de $\mathbf{N}$, $E_1 \otimes_A E_2 \otimes \cdots \otimes_A E_n$, ou simplement $E_1 \otimes E_2 \otimes \cdots \otimes E_n$) l’algèbre obtenue en munissant le produit tensoriel des $A$-modules $E_i$ de la multiplication définie par (1).

La relation (1) montre que le produit tensoriel $\bigotimes_{i \in I} E_i^0$ des algèbres opposées aux $E_i$ est l’algèbre opposée à $\bigotimes_{i \in I} E_i$; en particulier, si les $E_i$ sont commutatives, il en est de même de $\bigotimes_{i \in I} E_i$.

Soient $(E_i)_{i \in I}$ et $(F_i)_{i \in I}$ deux familles de $A$-algèbres ayant le même ensemble d’indices fini $I$. Soit, pour chaque $i \in I$, $f_i : E_i \to F_i$ un homomorphisme de $A$-algèbres. Alors l’application $A$-linéaire

$$
f = \bigotimes_{i \in I} f_i : \bigotimes_{i \in I} E_i \to \bigotimes_{i \in I} F_i
$$

est un homomorphisme de $A$-algèbres, comme il résulte de (1).

Pour toute partition $(I_j)_{j \in J}$ de $I$, les isomorphismes d’associativité

$$
\bigotimes_{j \in J} (\bigotimes_{i \in I_j} E_i) \to \bigotimes_{i \in I} E_i
$$

(II, p. 72) sont aussi des isomorphismes d’algèbres, comme il résulte de (1) et de leurs définitions.

Lorsque $I$ est l’intervalle $[1, n]$ de $\mathbf{N}$ et que toutes les algèbres $E_i$ sont égales à une même algèbre $E$, l’algèbre produit tensoriel $\bigotimes_{i \in I} E_i$ se note aussi $E^{\otimes n}$.

Nous nous bornerons dans le reste de ce $n^o$ aux propriétés des produits tensoriels de deux algèbres, laissant au lecteur le soin de les étendre aux produits tensoriels de familles finies quelconques.

Soient $E, F$ deux $A$-algèbres; si $a$ (resp. $b$) est un idéal à gauche de $E$ (resp. $F$), l’image canonique $\operatorname{Im}(a \otimes_A b)$ de $a \otimes_A b$ dans $E \otimes_A F$ est un idéal à gauche de $E \otimes_A F$; on a des énoncés analogues en remplaçant « idéal à gauche » par « idéal à droite » ou « idéal bilatère ». En outre:

#### Proposition 1 {#alg-iii-s4-prop-1 .statement}

Soient $E, F$ deux $A$-algèbres, $a$ (resp. $b$) un idéal bilatère de $E$ (resp. $F$). Alors l’isomorphisme canonique de $A$-modules

$$
(E/a) \otimes (F/b) \to (E \otimes F)/(\operatorname{Im}(a \otimes F) + \operatorname{Im}(E \otimes b))
$$

(II, p. 60, cor. 1) est un isomorphisme d’algèbres.

Cela résulte de (1) (III, p. 33) et de la définition donnée loc. cit.

#### Corollaire 1 {#alg-iii-s4-prop-1-cor-1 .statement}

Soient $E$ une $A$-algèbre, $a$ un idéal de $A$. Alors le $A$-module $aE$ est un idéal bilatère de $E$, et l’isomorphisme canonique de $(A/a)$-modules

$$
(A/a) \otimes_A E \to E/aE
$$

est un isomorphisme de $(A/a)$-algèbres.

#### Corollaire 2 {#alg-iii-s4-prop-1-cor-2 .statement}

Si $a, b$ sont deux idéaux de $A$, la $A$-algèbre $(A/a) \otimes_A (A/b)$ est canoniquement isomorphe à $A/(a + b)$.

#### Corollaire 3 {#alg-iii-s4-prop-1-cor-3 .statement}

Soient $E, F$ deux $A$-algèbres, $a$ un idéal de $A$ contenu dans l’annulateur de $F$. Alors la $(A/a)$-algèbre $E \otimes_A F$ est canoniquement isomorphe à $(E/aE) \otimes_{A/a} F$.

#### Proposition 2 {#alg-iii-s4-prop-2 .statement}

Soient $(E_\lambda)_{\lambda \in L}$ et $(F_\mu)_{\mu \in M}$ deux familles de $A$-algèbres. L’application canonique (II, p. 61)

$$
(\bigoplus_{\lambda \in L} E_\lambda) \otimes_A (\bigoplus_{\mu \in M} F_\mu) \to \bigoplus_{(\lambda, \mu) \in L \times M} (E_\lambda \otimes_A F_\mu)
$$

est un isomorphisme d’algèbres.

Cela résulte aussitôt de II, p. 61, prop. 7 et de la définition de la multiplication dans $E \otimes F$.

#### Proposition 3 {#alg-iii-s4-prop-3 .statement}

Soient $A, B$ deux anneaux commutatifs, $\varphi : A \to B$ un homomorphisme d’anneaux, $E, F$ deux $A$-algèbres. Alors l’isomorphisme canonique de $B$-modules

$$
\varphi^*(E) \otimes_B \varphi^*(F) \to \varphi^*(E \otimes_A F)
$$

(II, p. 83, prop. 3) est un isomorphisme de $B$-algèbres.

#### Proposition 4 {#alg-iii-s4-prop-4 .statement}

Soient $A, B$ deux anneaux commutatifs, $\varphi : A \to B$ un homomorphisme d’anneaux, $E$ une $A$-algèbre, $F$ une $B$-algèbre. Alors l’isomorphisme canonique de $A$-modules

$$
\varphi_*(F) \otimes_A E \to \varphi_*(F \otimes_B \varphi^*(E))
$$

(II, p. 85, prop. 6) est un isomorphisme de $A$-algèbres.

Les vérifications sont triviales, compte tenu de III, p. 7.

En particulier, la structure de $A$-algèbre de $B \otimes_A E$ obtenue par restriction à $A$ de l’anneau $B$ des scalaires, est identique à la structure de l’algèbre $B \otimes_A E$, produit tensoriel des $A$-algèbres $B$ et $E$.

Enfin, si $(A_i, \varphi_{ji})$ est un système inductif d’anneaux commutatifs, $(E_i, f_{ji})$ et $(F_i, g_{ji})$ deux systèmes inductifs de $A_i$-algèbres (III, p. 9), et $A = \lim \limits_{\longrightarrow} A_i$, l’isomorphisme canonique de $A$-modules

$$
\lim \limits_{\longrightarrow} (E_i \otimes_{A_i} F_i) \to (\lim \limits_{\longrightarrow} E_i) \otimes_A (\lim \limits_{\longrightarrow} F_i)
$$

(II, p. 93, prop. 7) est aussi un isomorphisme de $A$-algèbres, comme il résulte des définitions.

Exemples de produits tensoriels d’algèbres. — 1) Soient $A$ un anneau commutatif, $M, N$ deux $A$-modules ; l’application canonique

(2)
$$
\operatorname{End}_A(M) \otimes_A \operatorname{End}_A(N) \to \operatorname{End}_A(M \otimes_A N)
$$

(II, p. 79) est un homomorphisme de $A$-algèbres, comme il résulte de II, p. 53, formule (5). Lorsque $M$ ou $N$ est un $A$-module projectif de type fini, on sait que cet homomorphisme est *bijectif* (II, p. 79, prop. 4). En particulier on retrouve la définition du produit tensoriel de deux matrices carrées.

2) Soient S, T deux monoïdes, $A^{(S)}$ et $A^{(T)}$ les algèbres des monoïdes S et T sur l’anneau A (III, p. 19); on a alors un isomorphisme canonique de A-algèbres

$$
A^{(S)} \otimes_A A^{(T)} \to A^{(S \times T)}
$$

En effet, les éléments $e_s \otimes e_t$ (resp. $e_{(s, t)}$), où s parcourt S et t parcourt T, forment une base de $A^{(S)} \otimes_A A^{(T)}$ en vertu de II, p. 62, cor. 2 (resp. de $A^{(S \times T)}$); l’isomorphisme cherché s’obtient en faisant correspondre $e_{(s, t)}$ à $e_s \otimes e_t$, et il résulte aussitôt des définitions que c’est bien un isomorphisme d’*algèbres*.

### 2. Caractérisation universelle des produits tensoriels d’algèbres

#### Proposition 5 {#alg-iii-s4-prop-5 .statement}

*Soit* $(E_i)_{i \in I}$ *une famille finie de A-algèbres*, *et, pour chaque* $i \in I$, *soit* $e_i$ *l’élément unité de* $E_i$. *Pour chaque* $i \in I$, *soit* $u_i : E_i \to E = \bigotimes_{k \in I} E_k$ *l’application A-linéaire défini par*

$$
u_i(x_i) = \bigotimes_j x'_j \quad \text{avec } x'_i = x_i \text{ et } x'_j = e_j \text{ pour } j \neq i.
$$

(i) *Les* $u_i$ *sont des homomorphismes de A-algèbres; de plus, pour* $i \neq j$, *les éléments* $u_i(x_i)$ *et* $u_j(x_j)$ *sont permutables dans* E *quels que soient* $x_i \in E_i$ *et* $x_j \in E_j$, *et* E *est engendrée par la réunion des sous-algèbres* $u_i(E_i)$.

(ii) *Soit* F *une A-algèbre, et, pour tout* $i \in I$, *soit* $v_i : E_i \to F$ *un homomorphisme de A-algèbres, les* $v_i$ *étant tels que, pour* $i \neq j$, $v_i(x_i)$ *et* $v_j(x_j)$ *soient permutables dans* F *quels que soient* $x_i \in E_i$ *et* $x_j \in E_j$. *Alors il existe un homomorphisme de A-algèbres* $w : E \to F$ *et un seul tel que*

$$
v_i = w \circ u_i \quad \text{pour tout } i \in I.
$$

(i) L’application $u_i$ est un homomorphisme d’algèbres par définition de la multiplication dans E. Si $i \neq j$, $x_i \in E_i$, $x_j \in E_j$, on a

$$
u_i(x_i) = \bigotimes_k x'_k \quad \text{avec } x'_i = x_i, x'_{k'} = e_k \text{ pour } k \neq i
$$
$$
u_j(x_j) = \bigotimes_k x''_k \quad \text{avec } x''_j = x_j, x''_{k'} = e_k \text{ pour } k \neq j.
$$

Il est clair que $x'_k x''_{k'} = x''_{k'} x'_k$ pour tout $k \in I$, donc $u_i(x_i)$ et $u_j(x_j)$ commutent dans E d’après la formule (1) (III, p. 33) définissant la multiplication dans E. La dernière assertion résulte de la relation $\bigotimes_i x_i = \prod_{i \in I} u_i(x_i)$.

(ii) Pour chaque $i \in I$, soit $x_i$ un élément de $E_i$. Le produit $\prod_{i \in I} v_i(x_i)$ est alors défini dans F indépendamment de toute structure d’ordre sur I, puisque l’algèbre

F est associative et que les éléments $v_i(x_i)$ sont deux à deux permutables. L’application $(x_i)_{i \in I} \to \prod_{i \in I} v_i(x_i)$ de $\prod_{i \in I} E_i$ dans F est évidemment A-multilinéaire, et il existe donc une application A-linéaire $w : E \to F$ et une seule, telle que

$$
w(\bigotimes_i x_i) = \prod_i v_i(x_i).
$$

Or, l’homomorphisme de A-algèbres $w : E \to F$ cherché doit satisfaire à (5), qui résulte de (4) et du fait que $\bigotimes_i x_i = \prod_{i \in I} u_i(x_i)$. Ceci prouve l’unicité de $w$; il reste à montrer que l’application A-linéaire $w$ définie par (5) est un homomorphisme de A-algèbres et vérifie (4). Le fait que $w$ vérifie (4) est évident : il suffit d’appliquer (5) au cas où $x_j = e_j$ pour $j \neq i$, et on obtient $w(u_i(x_i)) = v_i(x_i)$. Enfin, $w$ est un homomorphisme d’algèbres, car on a

$$
w((\bigotimes_i x_i)(\bigotimes_i y_i)) = w(\bigotimes_i (x_i y_i)) = \prod_i v_i(x_i y_i)
$$
$$
= \prod_i (v_i(x_i) v_i(y_i)) = (\prod_i v_i(x_i)) \cdot (\prod_i v_i(y_i))
$$

puisque $v_i(x_i)$ permute avec $v_j(y_j)$ pour $j \neq i$; on a donc bien

$$
w((\bigotimes_i x_i)(\bigotimes_i y_i)) = w(\bigotimes_i x_i) \cdot w(\bigotimes_i y_i)
$$

ce qui, par linéarité, achève la démonstration.

Le couple formé de E et de l’application canonique $\varphi : (x_i) \to \bigotimes_i x_i$ de $\prod_i E_i$ dans E est solution du *problème d’application universelle* (E, IV, p. 23) où $\Sigma$ est l’espèce de structure de A-algèbre, les morphismes étant les homomorphismes de A-algèbres, et les $\alpha$-applications les applications $\prod_i u_i$ de $\prod_i E_i$ dans une A-algèbre, telles que les $u_i$ soient des homomorphismes de A-algèbres, et que $u_i(x_i)$ et $u_j(x_j)$ permutent pour $i \neq j$, quels que soient $x_i \in E_i$ et $x_j \in E_j$.

#### Corollaire {#alg-iii-s4-n2-cor-1 .statement}

*Soient* $(E_i)_{i \in I}, (F_i)_{i \in I}$ *deux familles finies de A-algèbres*, et, *pour tout* $i \in I$, *soit* $f_i : E_i \to F_i$ *un homomorphisme d’algèbres*. *Si* $u_i : E_i \to \bigotimes_{j \in I} E_j, v_i : F_i \to \bigotimes_{j \in I} F_j$ *sont les homomorphismes canoniques*, *l’application* $f = \bigotimes_i f_i$ *(cf. III, p. 34)* *est l’unique homomorphisme de A-algèbres tel que* $f \circ u_i = v_i \circ f_i$ *pour tout* $i \in I$.

Il suffit de noter que les homomorphismes $g_i = v_i \circ f_i$ sont tels que $g_i(x_i) = v_i(f_i(x_i))$ et $g_j(x_j) = v_j(f_j(x_j))$ permutent pour $i \neq j, x_i \in E_i$ et $x_j \in E_j$; on applique alors la prop. 5 de III, p. 36.

Lorsque, dans la prop. 5 (III, p. 36), on suppose que l’algèbre F est *commutative*, l’hypothèse que $v_i(x_i)$ et $v_j(x_j)$ sont permutables pour $i \neq j$ est automatiquement vérifiée. Donc, lorsque $F$ est commutative, on a une bijection canonique

$$
\operatorname{Hom}_{A\text{-alg.}}(\bigotimes_i E_i, F) \to \prod_i \operatorname{Hom}_{A\text{-alg.}}(E_i, F),
$$

à savoir celle qui, à tout homomorphisme $w$ de $\bigotimes_i E_i$ dans $F$, associe la famille des $w \circ u_i$.

On notera que si $E$ est une $A$-algèbre commutative, la structure d’anneau de $E \otimes_A F$ est la même que celle de $F_{(E)}$ (III, p. 7).

### 3. Modules et multimodules sur les produits tensoriels d’algèbres

#### Définition 2 {#alg-iii-s4-def-2 .statement}

Soit $E$ une $A$-algèbre (unifère). On appelle $E$-module à gauche (resp. à droite) un module à gauche (resp. à droite) sur l’anneau sous-jacent à $E$.

Sauf mention expresse du contraire, tous les modules et multimodules considérés dans ce n° sont des modules et multimodules à gauche.

Si $M$ est un $E$-module, l’homomorphisme $\eta : A \to E$ (III, p. 6) définit alors sur $M$ une structure de $A$-module dite sous-jacente à la structure de $E$-module de $M$; pour $\alpha \in A, s \in E, x \in M$, on a

$$
\alpha(sx) = s(\alpha x) = (\alpha s)x,
$$

de sorte que pour tout $s \in E$, l’homothétie $h_s : x \mapsto sx$ de $M$ est un endomorphisme de la structure sous-jacente de $A$-module. Inversement, la donnée d’une structure de $E$-module sur $M$ équivaut à la donnée d’une structure de $A$-module sur $M$ et d’un homomorphisme de $A$-algèbres $s \mapsto h_s$ de $E$ dans $\operatorname{End}_A(M)$.

#### Définition 3 {#alg-iii-s4-def-3 .statement}

Soient $E$ et $F$ deux $A$-algèbres (unifères), $M$ un ensemble muni d’une structure de $E$-module et d’une structure de $F$-module. On dit que $M$ est un bimodule (à gauche) sur les algèbres $E$ et $F$ si ;
1° $M$ est un bimodule sur les anneaux sous-jacents à $E$ et $F$ (II, p. 33);
2° les deux structures de $A$-module sous-jacentes aux structures de $E$-module et de $F$-module de $M$ sont identiques.

Cette dernière condition exprime que, si $e$ et $e'$ sont les éléments unités de $E$ et $F$ respectivement, on a

$$
(\alpha e)x = (\alpha e')x \quad \text{pour } \alpha \in A, x \in M;
$$

on note alors $\alpha x$ la valeur commune des deux membres.

On peut encore dire que se donner sur $M$ une structure de bimodule sur $E$ et $F$ équivaut à se donner sur $M$ une structure de $A$-module, ainsi que deux homomorphismes de $A$-algèbres $s \mapsto h'_s$ de $E$ dans $\operatorname{End}_A(M)$ et $t \mapsto h''_t$ de $F$ dans $\operatorname{End}_A(M)$ tels que $h'_s h''_t = h''_t h'_s$ quels que soient $s \in E$ et $t \in F$. Par suite (III, p. 36, prop. 5) on en déduit canoniquement un homomorphisme de A-algèbres $u \mapsto h_u$ de $E \otimes_A F$ dans $\mathrm{End}_A(M)$ tel que $h_s \otimes t = h'_s h''_t = h''_t h'_s$ pour $s \in E$ et $t \in F$. Autrement dit, on définit ainsi sur $M$ une structure de $(E \otimes_A F)$-module, dite associée à la structure de bimodule sur $E$ et $F$ donnée, et pour laquelle on a
$$
(s \otimes t) \cdot x = s(tx) = t(sx) \quad \text{pour } s \in E, \ t \in F \text{ et } x \in M.
$$
Les structures de $E$-module et de $F$-module données sur $M$ se déduisent de cette structure de $(E \otimes_A F)$-module par restrictions de l’anneau des scalaires, correspondant aux deux homomorphismes canoniques $E \to E \otimes_A F$ et $F \to E \otimes_A F$.

Inversement, si on se donne sur $M$ une structure de $(E \otimes_A F)$-module, on en déduit au moyen des homomorphismes canoniques $E \to E \otimes_A F$ et $F \to E \otimes_A F$ une structure de $E$-module et une structure de $F$-module sur $M$, et il est immédiat que $M$ est un *bimodule* sur les algèbres $E$ et $F$ pour ces deux structures, et que la structure de $(E \otimes_A F)$-module donnée est associée à cette structure de bimodule.

On a ainsi établi une correspondance biunivoque entre les $(E \otimes_A F)$-modules et les bimodules sur les algèbres $E$ et $F$. Il est clair que tout sous-bimodule de $M$ est un sous-module pour la structure de $(E \otimes_A F)$-module associée, et réciproquement. On a des résultats analogues pour les quotients, produits, sommes directes, limites projectives et injectives. Enfin, si $M'$ est un second bimodule sur les algèbres $E$ et $F$, et si $f : M \to M'$ est un homomorphisme de bimodules, $f$ est aussi un homomorphisme de $(E \otimes_A F)$-modules, et réciproquement.

On a évidemment des énoncés correspondants pour les structures de bimodule à droite, ou lorsque par exemple il s’agit d’une structure de $E$-module à gauche et d’une structure de $F$-module à droite; on parle dans ce cas de $(E, F)$-*bimodule*, et la donnée d’une telle structure revient à celle d’une structure de *bimodule à gauche* sur $E$ et $F^\circ$.

#### Exemple 1 {#alg-iii-s4-n3-exa-1 .statement}

Soit $B$ une $A$-algèbre; l’anneau $B$ est canoniquement muni d’une structure de $(B, B)$-*bimodule* (II, p. 34, *Exemple* 1), et si $e$ est l’élément unité de $B$, on a $(\alpha e)x = x(\alpha e) = \alpha x$ pour tout $x \in B$ et tout $\alpha \in A$; on peut donc considérer $B$ comme un *bimodule à gauche* sur les algèbres $B$ et $B^\circ$ (opposée à $B$); à la structure de $(B, B)$-bimodule de $B$ est donc associée une structure de $(B \otimes_A B^\circ)$-*module* telle que, pour $b, x$ et $b'$ dans $B$, on ait
$$
(b \otimes b') \cdot x = bx b'
$$
le second membre étant le produit dans l’anneau $B$.

#### Exemple 2 {#alg-iii-s4-n3-exa-2 .statement}

Soient $E$ et $F$ deux $A$-algèbres, $e, e'$ leurs éléments unités respectifs, $M$ un $E$-module, $N$ un $F$-module; ces structures de module définissent sur $M$ une structure de bimodule sur les anneaux $A$ et $E$, et sur $N$ une structure de bimodule sur les anneaux $A$ et $F$; on en déduit donc sur le produit tensoriel $M \otimes_A N$ une structure de bimodule sur les anneaux $E$ et $F$, définie par
$$
x \cdot (m \otimes n) = (x \cdot m) \otimes n, \quad y \cdot (m \otimes n) = m \otimes (y \cdot n)
$$

pour $x \in E, y \in F, m \in M, n \in N$ (II, p. 54); on voit en outre que les conditions (8) de III, p. 38 sont vérifiées, donc la structure de bimodule précédente est associée à une structure de $(E \otimes_A F)$-module sur $M \otimes_A N$, telle que
$$(x \otimes y) . (m \otimes n) = (x.m) \otimes (y.n)$$
pour $x \in E, y \in F, m \in M, n \in N$.

Si on prend en particulier $M = E_s$, $E_s \otimes_A N$ se trouve muni canoniquement d’une structure de $(E \otimes_A F)$-module; d’ailleurs, $E \otimes_A N$ est canoniquement identifié à $E \otimes_A (F_d \otimes_F N) = (E \otimes_A F) \otimes_F N$, où $E \otimes_A F$ est considéré comme muni de sa structure de $F$-module à droite définie par l’homomorphisme canonique $v : F \to E \otimes_A F$; pour $x, x'$ dans $E, y \in F, n \in N$, $x' \otimes n$ est ainsi identifié à $(x' \otimes e') \otimes n$, et $(x \otimes y) . (x' \otimes n) = (xx') \otimes (y.n)$ à $((xx') \otimes y) \otimes n$. Le $(E \otimes_A F)$-module $E_s \otimes_A N$ est ainsi identifié au $(E \otimes_A F)$-module déduit de $N$ par extension des scalaires à $E \otimes_A F$ au moyen de l’homomorphisme $v$ (II, p. 82). L’application canonique $n \mapsto e \otimes n$ de $N$ dans $E_s \otimes_A N$ s’identifie à l’application canonique $n \mapsto (e \otimes e') \otimes n$ de $N$ dans $(E \otimes_A F) \otimes_F N$; on sait que c’est un $F$-homomorphisme.

Avec les mêmes notations, soit $P$ un $(E \otimes_A F)$-module à droite; alors on a un isomorphisme canonique de $\mathbf{Z}$-modules
$$P \otimes_{E \otimes_A F}(E_s \otimes_A N) \to P \otimes_F N$$
où au second membre $P$ est considéré comme $F$-module à droite au moyen de l’homomorphisme canonique $v$. En effet, $P$ s’identifie canoniquement à $P \otimes_{E \otimes_A F}(E \otimes_A F)$, et $(E \otimes_A F) \otimes_F N$ à $E \otimes_A (F \otimes_F N)$, donc à $E \otimes_A N$, ce qui établit l’isomorphisme annoncé (II, p. 64, prop. 8 et II, p. 55, prop. 4).

Tout ce qui précède s’étend aux *multimodules* (II, p. 33).

### 4. Produit tensoriel d’algèbres sur un corps

Soient $K$ un *corps* commutatif, $E$ et $F$ deux algèbres sur $K$, dont les éléments unités respectifs $e, e'$ sont *non nuls*. Alors les homomorphismes $\eta_E : K \to E$ et $\eta_F : K \to F$ (III, p. 6) sont des injections qui permettent d’identifier $K$ à un sous-corps de $E$ (resp. de $F$). Les homomorphismes canoniques $u : E \to E \otimes_K F$ et $v : F \to E \otimes_K F$, définis par $u(x) = x \otimes e'$ et $v(y) = e \otimes y$, sont *injectifs* (II, p. 113, prop. 19), et permettent d’identifier $E$ et $F$ à des *sous-algèbres* de $E \otimes_K F$, ayant toutes deux comme élément unité l’élément unité $e \otimes e'$ de $E \otimes_K F$. Dans $E \otimes_K F$, on a $E \cap F = K$ (II, p. 113, prop. 19).

Si $E'$ et $F'$ sont des sous-algèbres de $E$ et $F$ respectivement, l’homomorphisme canonique $E' \otimes_K F' \to E \otimes_K F$ est injectif, et permet d’identifier $E' \otimes_K F'$ à la sous-algèbre de $E \otimes_K F$ engendrée par $E' \cup F'$ (II, p. 108, prop. 14).

#### Proposition 6 {#alg-iii-s4-prop-6 .statement}

*Soient* $E, F$ *deux algèbres sur un corps commutatif* $K$, *non réduites à* $0$, $C$ (resp. $D$) *une sous-algèbre de* $E$ (resp. $F$), $C'$ (resp. $D'$) *la commutante de* $C$ *dans* $E$ (resp. *de* $D$ *dans* $F$). *Alors la commutante de* $C \otimes_K D$ *dans* $E \otimes_K F$ *est* $C' \otimes_K D'$.

Tout revient à voir qu’un élément $z = \sum_i x_i \otimes y_i$ de la commutante de $C \otimes_K D$ ($x_i \in E, y_i \in F$) appartient à $C' \otimes_K D'$; on sait que l’on a $C' \otimes_K D' = (C' \otimes_K F) \cap (E \otimes_K D')$ (II, p. 109, corollaire). On peut supposer les $y_i$ linéairement indépendants sur $K$; pour tout $x \in C$, on doit avoir $(x \otimes e')z = z(x \otimes e')$, c’est-à-dire $\sum_i (xx_i - x_ix) \otimes y_i = 0$, d’où $xx_i = x_ix$ pour tout $i$ (II, p. 62, cor. 1); on doit donc avoir $x_i \in C'$ pour tout $i$, et par suite $z \in C' \otimes_K F$; on montre de même que $z \in E \otimes_K D'$, d’où la proposition.

#### Corollaire {#alg-iii-s4-n4-cor-1 .statement}

*Si Z et Z' sont les centres respectifs de E et F, le centre de E $\otimes_K$ F est Z $\otimes_K$ Z'._

Soient E et F deux sous-algèbres d’une algèbre G sur un corps commutatif K; supposons que tout élément de E *commute* à tout élément de F. Alors les injections canoniques $i : E \to G,\ j : F \to G$ définissent un homomorphisme canonique $h = i \otimes j : E \otimes_K F \to G$ (III, p. 36, prop. 5) tel que $(i \otimes j)(x \otimes y) = xy$ pour $x \in E, y \in F$.

#### Définition 4 {#alg-iii-s4-def-4 .statement}

*Etant donnée une algèbre G sur un corps commutatif K, on dit que deux sous-algèbres E, F de G sont linéairement disjointes sur K si elles vérifient les conditions suivantes:
1° tout élément de E commute à tout élément de F;
2° l’homomorphisme canonique de E $\otimes_K$ F dans G est injectif.*

#### Proposition 7 {#alg-iii-s4-prop-7 .statement}

*Soient G une algèbre sur un corps commutatif K, E et F deux sous-algèbres de G telles que tout élément de E commute à tout élément de F. Pour que E et F soient linéairement disjointes sur K, il faut et il suffit qu’il existe une base de E sur K qui soit une partie libre de G pour la structure de F-module à droite de G. Lorsqu’il en est ainsi:
(i) l’homomorphisme canonique $h : E \otimes_K F \to G$ est un isomorphisme de E $\otimes_K$ F sur la sous-algèbre de G engendrée par $E \cup F$;
(ii) on a $E \cap F = K$;
(iii) toute partie libre de E (resp. F) sur K est une partie libre de G pour sa structure de F-module (resp. de E-module) à droite ou à gauche.
La condition de l’énoncé est évidemment nécessaire, toute base de E sur K étant une base de E $\otimes_K$ F pour sa structure de F-module à droite (II, p. 62, cor. 1). Pour voir que la condition est suffisante, remarquons que l’image H de E $\otimes_K$ F par $h$ est l’ensemble des sommes $\sum_i x_i y_i = \sum_i y_i x_i$ dans G, avec $x_i \in E$ et $y_i \in F$; si $(a_\lambda)$ est une base de E sur K, H est donc aussi le *sous-module* du F-module (à droite ou à gauche) G, engendré par $(a_\lambda)$. La condition de l’énoncé signifie donc qu’il existe une base $(a_\lambda)$ de E qui est aussi une base du F-module H; il en résulte que $h$ est injective. L’assertion (iii) résulte de ce que toute partie libre de E est contenue dans une base de E (II, p. 95, th. 2).

#### Corollaire 1 {#alg-iii-s4-prop-7-cor-1 .statement}

*Pour que l’homomorphisme canonique de E $\otimes_K$ F dans G soit bijectif,* il faut et il suffit qu’il existe une base de E sur K qui soit une base du F-module (à droite ou à gauche) G.

#### Corollaire 2 {#alg-iii-s4-prop-7-cor-2 .statement}

Soient E, F deux sous-algèbres de G, de rang fini sur K, telles que tout élément de E commute à tout élément de F. Pour que E et F soient linéairement disjointes sur K, il faut et il suffit que la sous-algèbre H de G engendrée par E ∪ F soit telle que

(12) $$ [H:K] = [E:K].[F:K]. $$

En effet, cela exprime que le rang sur K de l’homomorphisme canonique surjectif $h : E \otimes_K F \to H$ est égal au rang de $E \otimes_K F$ sur K, ce qui équivaut à dire que cet homomorphisme est bijectif (II, p. 101, prop. 9).

### 5. Produit tensoriel d’une famille infinie d’algèbres.

Soient A un anneau commutatif, et $(E_i)_{i \in I}$ une famille quelconque de A-algèbres (unifères). Pour toute partie finie J de I, notons $E_J$ le produit tensoriel $\bigotimes_{i \in J} E_i$ des algèbres $E_i$ d’indice $i \in J$; on note $e_i$ l’élément unité de $E_i$, et $e_J = \bigotimes_{i \in J} e_i$ l’élément unité de $E_J$; on note $f_{J,i}$ l’homomorphisme canonique $E_i \to E_J$ pour $i \in J$ (III, p. 36, prop. 5). Si J, J’ sont deux parties finies de I telles que $J \subset J'$, on en déduit canoniquement (III, p. 36, prop. 5) un homomorphisme $f_{J',J} : E_J \to E_{J'}$ par la condition $f_{J',J} \circ f_{J,i} = f_{J',i}$ pour tout $i \in J$. En outre l’unicité de $f_{J',J}$ entraîne que si J, J’, J'' sont trois parties finies de I telles que $J \subset J' \subset J''$, on a $f_{J'',J} = f_{J'',J'} \circ f_{J',J}$. Autrement dit, $(E_J, f_{J',J})$ est un système inductif de A-algèbres dont l’ensemble d’indices est l’ensemble filtrant croissant $\mathfrak{F}(I)$ des parties finies de I.

#### Définition 5 {#alg-iii-s4-def-5 .statement}

On appelle produit tensoriel de la famille de A-algèbres $(E_i)_{i \in I}$ la limite inductive E du système inductif $(E_J, f_{J',J})$.

Si I est fini, E s’identifie à $\bigotimes_{i \in I} E_i$. Par abus de notation, on désigne encore E par $\bigotimes_{i \in I} E_i$ même si I est infini.

Pour toute partie finie J de I, on notera $f_J$ l’homomorphisme canonique $\bigotimes_{i \in J} E_i \to \bigotimes_{i \in I} E_i$ (et on écrira $f_i$ au lieu de $f_{\{i\}}$); si $e$ est l’élément unité de $\bigotimes_{i \in I} E_i$, on a donc $f_J(e_J) = e$ pour tout $J \in \mathfrak{F}(I)$. Il est immédiat que si toutes les algèbres $E_i$ sont commutatives, il en est de même de $\bigotimes_{i \in I} E_i$.

#### Proposition 8 {#alg-iii-s4-prop-8 .statement}

(i) Les homomorphismes $f_i : E_i \to E = \bigotimes_{k \in I} E_k$ sont tels que pour deux indices $i, j$ tels que $i \neq j$, $f_i(x_i)$ et $f_j(x_j)$ commutent dans E quels que soient $x_i \in E_i$ et $x_j \in E_j$; en outre, E est engendrée par la réunion des sous-algèbres $f_i(E_i)$.

(ii) Soit F une A-algèbre, et, pour tout $i \in I$, soit $u_i : E_i \to F$ un homomorphisme de A-algèbres tel que, pour $i \neq j$, $u_i(x_i)$ et $u_j(x_j)$ commutent dans F quels que soient $x_i \in E_i$ et x_j \in E_j. Alors il existe un homomorphisme de A-algèbres u : E \to F et un seul tel que l’on ait $u_i = u \circ f_i$ quel que soit $i \in I$.

(i) Comme, pour toute partie finie J de I, on a $f_i = f_J \circ f_{J,i}$, la première assertion de (i) résulte de III, p. 36, prop. 5, en prenant J contenant i et j; la second résulte aussi de III, p. 36, prop. 5, en tenant compte de ce que E est réunion des $f_J(E_J)$ lorsque J parcourt $\mathcal{F}(I)$.

(ii) Pour toute partie finie J de I, il résulte de III, p. 36, prop. 5 qu’il existe un homomorphisme unique $u_J : E_J \to F$ tel que $u_J \circ f_{J,i} = u_i$ pour tout $i \in J$; on déduit aussitôt de cette propriété d’unicité que, pour $J \subset J'$, on a $u_J = u_{J'} \circ f_{J',J}$; autrement dit, les $u_J$ forment un système inductif d’homomorphismes. Soit $u = \lim_{\longrightarrow} u_J : E \to F$; on a par définition $u_J = u \circ f_J$ pour toute partie finie J de I, et en particulier $u_i = u \circ f_i$ pour tout $i \in I$; l’unicité de u résulte de ces relations et du fait que les $f_i(E_i)$ engendrent l’algèbre E.

#### Corollaire {#alg-iii-s4-n5-cor-1 .statement}

Soient $(E_i)_{i \in I}, (E'_i)_{i \in I}$ deux familles de A-algèbres ayant même ensemble d’indices, et, pour tout $i \in I$, soit $u_i : E_i \to E'_i$ un homomorphisme d’algèbres. Il existe alors un homomorphisme de A-algèbres et un seul $u : \bigotimes_{i \in I} E_i \to \bigotimes_{i \in I} E'_i$ tel que, pour tout $i \in I$, le diagramme

$$
\begin{array}{ccc}
E_i & \xrightarrow{u_i} & E'_i \\
f_i \downarrow & & \downarrow f'_i \\
\bigotimes_{i \in I} E_i & \xrightarrow{u} & \bigotimes_{i \in I} E'_i
\end{array}
$$

soit commutatif, $f_i$ et $f'_i$ désignant les homomorphismes canoniques.

Il suffit d’appliquer la prop. 8 aux homomorphismes $f'_i \circ u_i$.

L’homomorphisme u défini dans le cor. de la prop. 8 se note $\bigotimes_{i \in I} u_i$. Si J est une partie quelconque de I, on peut appliquer la prop. 8 à la famille $(f_i)_{i \in J}$ des homomorphismes canoniques $f_i : E_i \to \bigotimes_{i \in I} E_i = E$; on en déduit un homomorphisme canonique $E_J \to E$, que l’on note encore $f_J$ et qui, lorsque J est finie, coïncide avec l’homomorphisme noté de cette façon plus haut.

Soit maintenant $(x_i)_{i \in I}$ un élément de $\prod_{i \in I} E_i$ tel que la famille $(x_i - e_i)_{i \in I}$ ait un support fini H. Il est immédiat que, si J et J’ sont deux parties finies de I contenant H, on a

$$
f_J((x_i)_{i \in J}) = f_{J'}((x_i)_{i \in J'}).
$$

On désignera par $\bigotimes_{i \in I} x_i$ la valeur commune des $f_J((x_i)_{i \in J})$ pour les parties finies $J \supset H$ de I.

#### Proposition 9 {#alg-iii-s4-prop-9 .statement}

Soit $(E_i)_{i \in I}$ une famille de A-algèbres, et pour chaque $i \in I$, soit B une base de $E_i$ telle que l’élément unité $e_i$ appartienne à $B_i$. Soit $B$ l’ensemble des éléments de la forme $\bigotimes_{i \in I} x_i$, où $(x_i)$ parcourt l’ensemble des éléments de $\prod_{i \in I} B_i$ tels que la famille $(x_i - e_i)$ ait un support fini. Alors $B$ est une base de l’algèbre $\bigotimes_{i \in I} E_i$, et cette base contient l’élément unité $e$.

En effet, pour toute partie finie $J$ de $I$, soit $B_J$ la base de $E_J = \bigotimes_{i \in J} E_i$ produit tensoriel des bases $B_i$ pour $i \in J$ (II, p. 72). Il résulte aussitôt des définitions que $B$ est la réunion des $f_J(B_J)$ lorsque $J$ parcourt $F(I)$, et que l’on a $f_{J',J}(B_J) \subset B_{J'}$ lorsque $J \subset J'$; donc $(B_J)$ est un système inductif de parties des $E_J$ et $B = \varinjlim B_J$; la conclusion résulte donc de II, p. 92, corollaire.

On dit encore que la base $B$ est le produit tensoriel des bases $B_i$ pour $i \in I$; lorsque les conditions de la prop. 9 sont satisfaites, les homomorphismes canoniques $f_J : E_J \to E = \bigotimes_{i \in I} E_i$ sont injectifs pour toute partie $J$ de $I$, car si $B_J$ est la base de $E_J$ produit tensoriel des $B_i$ pour $i \in J$, on vérifie aussitôt que la restriction de $f_J$ à $B_J$ est injective et applique $B_J$ sur une partie de $B$.

### 6. Lemmes de commutation

#### Lemme 1 {#alg-iii-s4-lem-1 .statement}

Soient $A$ un anneau commutatif, $E$ une $A$-algèbre, $(x_i)_{1 \leq i \leq n}$ une suite finie d’éléments de $E$, $(\lambda_i)_{1 \leq i \leq n}$ une suite finie d’éléments de $A$, $y$ un élément de $E$; supposons que l’on ait
$$
x_i y = \lambda_i y x_i \quad \text{pour } 1 \leq i \leq n.
$$
Alors on a
$$
(x_1 x_2 \ldots x_n) y = (\lambda_1 \lambda_2 \ldots \lambda_n) y (x_1 x_2 \ldots x_n).
$$

Le lemme étant trivial pour $n = 1$, on raisonne par récurrence sur $n \geq 2$. On a
$$
(x_1 x_2 \ldots x_n) y = (x_1 \ldots x_{n-1}) (x_n y) = (x_1 \ldots x_{n-1}) (\lambda_n y x_n) = \lambda_n ((x_1 \ldots x_{n-1}) y) x_n
$$
ce qui, d’après l’hypothèse de récurrence, est égal à
$$
\lambda_n (\lambda_1 \ldots \lambda_{n-1}) y (x_1 \ldots x_{n-1}) x_n = (\lambda_1 \ldots \lambda_{n-1} \lambda_n) y (x_1 \ldots x_{n-1} x_n),
$$
d’où le lemme.

#### Lemme 2 {#alg-iii-s4-lem-2 .statement}

Soient $A$ un anneau commutatif, $E$ une $A$-algèbre, $(x_i)_{1 \leq i \leq n}$ et $(y_i)_{1 \leq i \leq n}$ deux suites finies de $n$ éléments de $E$; supposons que pour $1 \leq j < i \leq n$, on ait
$$
x_i y_j = \lambda_{ij} y_j x_i \quad \text{avec } \lambda_{ij} \in A.
$$
Alors on a
$$
(x_1 x_2 \ldots x_n) (y_1 y_2 \ldots y_n) = (\prod_{i > j} \lambda_{ij}) (x_1 y_1) (x_2 y_2) \ldots (x_n y_n).
$$

Le lemme étant trivial pour $n = 1$, on raisonne encore par récurrence sur $n$ pour $n \geqslant 2$. En vertu du lemme 1, on a
$$
(x_1 \ldots x_n)(y_1 \ldots y_n) = x_1(x_2 \ldots x_n)y_1(y_2 \ldots y_n) =
= (\prod_{i > 1} \lambda_{i1})(x_1y_1)(x_2 \ldots x_n)(y_2 \ldots y_n)
$$
et il suffit alors d’appliquer l’hypothèse de récurrence pour obtenir (16).

Pour toute famille $\lambda = (\lambda_{ij})$ d’éléments de $\mathbf{A}$, avec $1 \leq j < i \leq n$, et pour toute permutation $\sigma \in \mathfrak{S}_n$, on pose
$$
\varepsilon_\sigma(\lambda) = \prod_{i > j, \sigma^{-1}(i) < \sigma^{-1}(j)} \lambda_{ij} = \prod_{i < j, \sigma(i) > \sigma(j)} \lambda_{\sigma(i), \sigma(j)}.
$$
On observera que, lorsque $\mathbf{A} = \mathbf{Z}$ et $\lambda_{ij} = -1$ pour tout couple $(i, j)$ tel que $1 \leq j < i \leq n$, $\varepsilon_\sigma(\lambda)$ n’est autre que la signature $\varepsilon_\sigma$ de la permutation $\sigma$ (I, p. 62).

#### Lemme 3 {#alg-iii-s4-lem-3 .statement}

*Soient $\mathbf{A}$ un anneau commutatif, $\mathbf{E}$ une $\mathbf{A}$-algèbre, $(x_i)_{1 \leq i \leq n}$ une suite finie d’éléments de $\mathbf{E}$, et supposons que, pour tout couple $(i, j)$ d’entiers tel que $1 \leq j < i < n$, on ait*
$$
x_i x_j = \lambda_{ij} x_j x_i \qquad \text{avec } \lambda_{ij} \in \mathbf{A}.
$$
*Alors, pour toute permutation $\sigma \in \mathfrak{S}_n$, on a*
$$
x_{\sigma(1)} x_{\sigma(2)} \ldots x_{\sigma(n)} = \varepsilon_\sigma(\lambda) x_1 x_2 \ldots x_n.
$$
Le lemme est trivial pour $n = 1$ et $n = 2$; procédons par récurrence sur $n$ pour $n \geq 3$. Si $\sigma(n) = n$, la relation (19) résulte de l’hypothèse de récurrence. Supposons donc $\sigma(n) = k, k \neq n$, et soit $\tau$ la permutation de $\{1, n\}$ définie par
$$
\begin{cases}
\tau(i) = i & \text{pour } i < k \\
\tau(i) = i + 1 & \text{pour } k \leq i < n \\
\tau(n) = k.
\end{cases}
$$
Soit $\pi = \tau^{-1} \circ \sigma$; la permutation $\pi$ laisse fixe $n$; on a $\sigma = \tau \circ \pi$, et par suite, si on pose $y_i = x_{\tau(i)}$, on a $y_{\pi(i)} = x_{\sigma(i)}$. Si $i \neq n$ et $j \neq n$, les relations $\pi(i) > \pi(j)$ et $\sigma(i) > \sigma(j)$ sont équivalentes (puisque $\tau$ est une application strictement croissante de $\{1, n - 1\}$ dans $\{1, n\}$). Pour $i \neq n, j \neq n$ et $\sigma(i) > \sigma(j)$, on a
$$
y_{\pi(i)} y_{\pi(j)} = x_{\sigma(i)} x_{\sigma(j)} = \lambda_{\sigma(i), \sigma(j)} x_{\sigma(j)} x_{\sigma(i)} = \lambda_{\sigma(i), \sigma(j)} y_{\pi(j)} y_{\pi(i)}
$$
d’où, par l’hypothèse de récurrence (compte tenu du fait que $\pi(n) = n$) :
$$
y_{\pi(1)} y_{\pi(2)} \ldots y_{\pi(n)} = \left( \prod_{i < j < n, \sigma(i) > \sigma(j)} \lambda_{\sigma(i), \sigma(j)} \right) y_1 y_2 \ldots y_n
$$
c’est-à-dire
$$
x_{\sigma(1)} x_{\sigma(2)} \ldots x_{\sigma(n)} = \left( \prod_{i < j < n, \sigma(i) > \sigma(j)} \lambda_{\sigma(i), \sigma(j)} \right) x_{\tau(1)} \ldots x_{\tau(n)}.
$$

Or, on a

$$
x_{\tau(1)} \cdots x_{\tau(n)} = x_1 \cdots x_{k-1} x_{k+1} \cdots x_n x_k,
$$

et ceci, d’après le lemme 1 (III, p. 44), est égal à

$$(21)$$
$$
\left( \prod_{j > k} \lambda_{jk} \right) x_1 \ldots x_n = \left( \prod_{\sigma(i) > \sigma(n)} \lambda_{\sigma(i), \sigma(n)} \right) x_1 \ldots x_n.
$$

Finalement, (20) et (21) donnent

$$
x_{\sigma(1)} \cdots x_{\sigma(n)} = \alpha \cdot x_1 \ldots x_n
$$

avec

$$
\alpha = \left( \prod_{i < j < n, \sigma(i) > \sigma(j)} \lambda_{\sigma(i), \sigma(j)} \right) \cdot \left( \prod_{i < n, \sigma(i) > \sigma(n)} \lambda_{\sigma(i), \sigma(n)} \right)
$$
$$
= \prod_{i < j, \sigma(i) > \sigma(j)} \lambda_{\sigma(i), \sigma(j)} = \varepsilon_\sigma(\lambda)
$$

ce qui achève la démonstration du lemme 3.

### 7. Produit tensoriel d’algèbres graduées relativement à des facteurs de commutation

#### Définition 6 {#alg-iii-s4-def-6 .statement}

Soit $(\Delta_i)_{i \in I}$ une famille finie de monoïdes commutatifs, notés additives ment. On appelle système de facteurs de commutation sur les $\Delta_i$, à valeurs dans un anneau commutatif $\mathbf{A}$, un système d’applications $\varepsilon_{ij} : \Delta_i \times \Delta_j \to \mathbf{A}$, où $i \in I, j \in I, i \neq j$, vérifiant les conditions suivantes:

(22)
$$
\varepsilon_{ij}(\alpha_i + \alpha'_i, \beta_j) = \varepsilon_{ij}(\alpha_i, \beta_j) \varepsilon_{ij}(\alpha'_i, \beta_j)
$$
(23)
$$
\varepsilon_{ij}(\alpha_i, \beta_j + \beta'_j) = \varepsilon_{ij}(\alpha_i, \beta_j) \varepsilon_{ij}(\alpha_i, \beta'_j)
$$
(24)
$$
\varepsilon_{ij}(\alpha_i, \beta_j) \varepsilon_{ji}(\beta_j, \alpha_i) = 1,
$$

quels que soient $\alpha_i, \alpha'_i$ dans $\Delta_i$, $\beta_j, \beta'_j$ dans $\Delta_j$.

Si on munit I d’une structure d’ordre total et si les $\Delta_i$ sont des groupes, on définit un système de facteurs de commutation sur les $\Delta_i$ en prenant pour tout couple $(i, j)$ tel que $i < j$ une application $\mathbf{Z}$-bilinéaire quelconque $\varepsilon_{ij}$ de $\Delta_i \times \Delta_j$ dans le $\mathbf{Z}$-module (multiplicatif) $\mathbf{A}^*$ des éléments inversibles de l’anneau $\mathbf{A}$, puis en posant $\varepsilon_{ji}(\beta_j, \alpha_i) = (\varepsilon_{ij}(\alpha_i, \beta_j))^{-1}$ pour $i < j$.

On notera que, puisque les $\varepsilon_{ij}(\alpha_i, \beta_j)$ sont inversibles, on a

$$
\varepsilon_{ij}(0, \beta_j) = \varepsilon_{ij}(\alpha_i, 0) = 1,
$$

en vertu de (22) et (23).

#### Exemple 1 {#alg-iii-s4-n7-exa-1 .statement}

Le système de facteurs de commutation trivial est formé des $\varepsilon_{ij}$ tels que $\varepsilon_{ij}(\alpha_i, \beta_j) = 1$ quels que soient $i, j$, $\alpha_i \in \Delta_i$, $\beta_j \in \Delta_j$.

#### Exemple 2 {#alg-iii-s4-n7-exa-2 .statement}

Si on prend $\mathbf{A} = \mathbf{Z}$ et $\Delta_i = \mathbf{Z}$ pour tout $i \in I$, on a un système de facteurs de commutation en prenant $\varepsilon_{ij}(\alpha_i, \beta_j) = (-1)^{\alpha_i \beta_j}$. On notera que ce nombre ne dépend que des parités de $\alpha_i$ et $\beta_j$, et les $\varepsilon_{ij}$ peuvent donc être considérés comme un système de facteurs de commutation lorsque certains des $\Delta_i$ sont égaux à $\mathbf{Z}/2\mathbf{Z}$, les autres à $\mathbf{Z}$.

Ces deux exemples sont les cas les plus fréquents que l’on rencontre dans les applications.

#### Proposition 10 {#alg-iii-s4-prop-10 .statement}

*Soient A un anneau commutatif, $(\Delta_i)_{i \in I}$ une famille finie de monoïdes commutatifs, notés additivement; pour chaque $i \in I$, soit $E_i$ une A-algèbre graduée de type $\Delta_i$. Enfin, soit $(\varepsilon_{ij})$ un système de facteurs de commutation sur les $\Delta_i$, à valeurs dans A. Il existe alors une A-algèbre graduée E de type $\Delta = \prod_{i \in I} \Delta_i$ et, pour chaque $i \in I$, un homomorphisme d’algèbres $h_i : E_i \to E$, ayant les propriétés suivantes:

(i) Si $\varphi_i : \Delta_i \to \Delta$ est l’homomorphisme canonique, alors $h_i$ est un homomorphisme gradué (II, p. 166), autrement dit, on a $h_i(E_i^{\alpha_i}) \subset E^{\varphi_i(\alpha_i)}$, en notant $(E_i^{\alpha_i})$ et $(E^{\alpha})$ les graduations respectives de $E_i$ et de $E$.

(ii) Si $i \neq j$ et si $x_i$ (resp. $x_j$) est un élément de $E_i$ (resp. $E_j$) homogène de degré $\alpha_i \in \Delta_i$ (resp. $\beta_j \in \Delta_j$), alors on a

$$
h_i(x_i)h_j(x_j) = \varepsilon_{ij}(\alpha_i, \beta_j)h_j(x_j)h_i(x_i).
$$

(iii) Pour toute A-algèbre F et tout système d’homomorphismes $f_i : E_i \to F$ vérifiant les conditions

$$
f_i(x_i)f_j(x_j) = \varepsilon_{ij}(\alpha_i, \beta_j)f_j(x_j)f_i(x_i)
$$

lorsque $i, j, x_i, x_j, \alpha_i, \beta_j$ ont les mêmes significations que dans (ii), alors il existe un homomorphisme d’algèbres $f : E \to F$ et un seul, tel que $f_i = f \circ h_i$ pour tout $i \in I$. En outre, le A-module sous-jacent à E est le produit tensoriel $\bigotimes_{i \in I} E_i$.

Considérons le A-module $E = \bigotimes_{i \in I} E_i$; il s’identifie à la somme directe des sous-modules $E^{\alpha}$, où, pour tout $\alpha = (\alpha_i) \in \Delta$, on pose $E^{\alpha} = \bigotimes_{i \in I} E_i^{\alpha_i}$; les $E^{\alpha}$ forment donc sur le A-module E une graduation de type $\Delta$. Nous allons définir sur E une structure de A-algèbre graduée de type $\Delta$. Pour cela, munissons I d’une structure d’ordre total; pour tout couple d’éléments $\alpha = (\alpha_i), \beta = (\beta_i)$ de $\Delta$, il s’agit d’abord de définir une application A-bilinéaire de $E^{\alpha} \times E^{\beta}$ dans $E^{\alpha + \beta}$, ou encore une application A-linéaire $m_{\alpha \beta}$ de $E^{\alpha} \otimes_A E^{\beta}$ dans $E^{\alpha + \beta}$. Nous définirons $m_{\alpha \beta}$ par la condition

$$
m_{\alpha \beta}((\bigotimes_{i \in I} x_i) \otimes (\bigotimes_{i \in I} y_i)) = \varepsilon(\alpha, \beta) \bigotimes_{i \in I} (x_i y_i)
$$

pour $x_i \in E_i^{\alpha_i}, y_i \in E_i^{\beta_i}$, où l’on a posé

$$
\varepsilon(\alpha, \beta) = \prod_{i > j} \varepsilon_{ij}(\alpha_i, \beta_j).
$$

En effet, le second membre de (27) appartient évidemment à $E^{\alpha + \beta}$, et l’application $(x_1, \ldots, x_n, y_1, \ldots, y_n) \mapsto \varepsilon(\alpha, \beta) \bigotimes_{i \in I} (x_i y_i)$ est A-multilinéaire dans le produit des $E_i^{\alpha_i}$ et des $E_i^{\beta_i}$ ($1 \leq i \leq n$). Il s’agit ensuite de prouver que la multiplication ainsi définie sur $E$ est *associative*; or, si $\gamma = (\gamma_i)$ est un troisième élément de $\Delta$, et $z_i \in E_i^{\gamma_i}$ pour $1 \leq i \leq n$, on a
$$
((\bigotimes_i x_i)(\bigotimes_i y_i))(\bigotimes_i z_i) = \varepsilon(\alpha + \beta, \gamma) \varepsilon(\alpha, \beta) \bigotimes_i (x_i y_i z_i)
$$
$$
(\bigotimes_i x_i)((\bigotimes_i y_i)(\bigotimes_i z_i)) = \varepsilon(\alpha, \beta + \gamma) \varepsilon(\beta, \gamma) \bigotimes_i (x_i y_i z_i)
$$
et tout revient à vérifier l’identité
$$
\varepsilon(\alpha + \beta, \gamma) \varepsilon(\alpha, \beta) = \varepsilon(\alpha, \beta + \gamma) \varepsilon(\beta, \gamma).
$$
Mais cette dernière résulte aussitôt des relations
$$
\varepsilon(\alpha + \beta, \gamma) = \varepsilon(\alpha, \gamma) \varepsilon(\beta, \gamma)
$$
$$
\varepsilon(\alpha, \beta + \gamma) = \varepsilon(\alpha, \beta) \varepsilon(\alpha, \gamma)
$$
elles-mêmes conséquences immédiates de la définition (28) et de (22) et (23) (III, p. 46).

Si, pour tout $i \in I$, $e_i$ désigne l’élément unité de $E_i$, on sait que $e_i$ est homogène de degré 0 (III, p. 30), donc $e = \bigotimes_{i \in I} e_i$ est homogène de degré 0, et il résulte de (27), (28) (III, p. 47) et des relations $\varepsilon_{ij}(\alpha_i, 0) = \varepsilon_{ij}(0, \beta_j) = 1$ que $e$ est élément unité de $E$, ce qui achève de définir sur $E$ la structure de A-algèbre graduée cherchée. On prendra ensuite $h_i(x_i) = x_i \otimes \bigotimes_{j \neq i} e_j$; pour vérifier que $h_i(x_i x'_i) = h_i(x_i) h_i(x'_i)$ pour $x_i, x'_i$ dans $E_i$, on peut se borner au cas où $x_i$ et $x'_i$ sont homogènes, et alors cette relation découle aussitôt de (27) (III, p. 47) et des relations $\varepsilon_{ij}(\alpha_i, 0) = \varepsilon_{ij}(0, \beta_j) = 1$; ces mêmes relations et (24) (III, p. 46) prouvent en outre que les $h_i$ satisfont aux conditions (i) et (ii) de l’énoncé, et que l’on a
$$
\bigotimes_{i \in I} x_i = \prod_{i \in I} h_i(x_i)
$$
où le second membre est le produit de la *séquence* $(h_i(x_i))_{i \in I}$ dans $E$ pour la structure d’ordre total considérée sur $I$ (I, p. 3) (il suffit de raisonner par récurrence sur le nombre des $x_i$ (supposés homogènes) distincts des $e_i$).

Reste à vérifier la condition (iii); notons que l’application $(x_i)_{i \in I} \mapsto \prod_{i \in I} f_i(x_i)$, où le second membre est le produit de la *séquence* $(f_i(x_i))_{i \in I}$ pour l’ordre total choisi sur $I$, est A-multilinéaire. Il existe donc une application A-linéaire et une seule $f : E \to F$ telle que
$$
f(\bigotimes_{i \in I} x_i) = \prod_{i \in I} f_i(x_i).
$$
Il est clair que $f(e)$ est l’élément unité de $F$ et que $f \circ h_i = f_i$; pour voir que $f$ est un homomorphisme d’algèbres, autrement dit que $f(x)f(y) = f(xy)$ pour $x, y$ dans $E$, on peut se borner, par linéarité, au cas où $x = \bigotimes_{i \in I} x_i, y = \bigotimes_{i \in I} y_i, x_i$ (resp. $y_i$) étant homogène de degré $\alpha_i$ (resp. $\beta_i$) pour tout $i \in I$. La relation à vérifier se réduit alors, compte tenu de (27) (III, p. 47), à
$$
\left( \prod_{i \in I} f_i(x_i) \right) \left( \prod_{i \in I} f_i(y_i) \right) = \varepsilon(\alpha, \beta) \prod_{i \in I} (f_i(x_i) f_i(y_i)).
$$
Mais compte tenu des relations (26) (III, p. 47), cela est une conséquence du lemme 2 de III, p. 44.

Il est clair que l’algèbre $E$ et l’application canonique $\psi : \bigotimes_{i \in I} E_i \to E$ constituent une solution du *problème d’application universelle* (E, IV, p. 23), où $\Sigma$ est l’espèce de structure de A-algèbre, et les $\alpha$-applications les applications $\prod_i f_i$ de $\prod_i E_i$ dans une A-algèbre, vérifiant les conditions (26) de III, p. 47.

Pour un ordre total fixé sur $I$, nous dirons que l’algèbre graduée $E$ définie dans la démonstration de la prop. 10 est un $\varepsilon$-*produit tensoriel gradué de type* $\Delta$ de la famille $(E_i)_{i \in I}$ d’algèbres graduées de types $\Delta_i$, et nous le noterons $\varepsilon \bigotimes_{i \in I} E_i$ (s’il n’y a pas de confusion possible sur l’ordre de $I$); nous noterons de même $\varepsilon \bigotimes_{i \in I} f_i$ l’homomorphisme $f : E \to F$ défini dans la démonstration de la prop. 10. Les homomorphismes $h_i$ sont dits *canoniques*. On écrit aussi $^e G^{\otimes n}$ lorsque $I = \{1, n\}$ et que toutes les $E_i$ sont égales à une même algèbre $G$.

#### Remarque 1 {#alg-iii-s4-n7-rem-1 .statement}

On retrouve le produit tensoriel d’algèbres défini dans III, p. 34 (muni en outre de la graduation produit tensoriel de celles de ses facteurs) lorsque l’on prend $\varepsilon_{ij}(\alpha_i, \beta_j) = 1$ quels que soient $i, j, \alpha_i$ et $\beta_j$.
2) Supposons que tous les $\Delta_i$ soient égaux à $\mathbf{Z}$, et posons $\varepsilon_{ij}(\alpha_i, \beta_j) = (-1)^{\alpha_i \beta_j}$; le $\varepsilon$-produit tensoriel $\varepsilon \bigotimes_{i \in I} E_i$ correspondant à ce système de facteurs de commutation est alors appelé le produit tensoriel *gauche* des algèbres graduées $E_i$ de type $\mathbf{Z}$, et se note $^g \bigotimes_{i \in I} E_i$ (ou $E \ ^g \bigotimes_A F$ pour deux algèbres, ou $^g G^{\otimes n}$ au lieu de $^e G^{\otimes n}$).

#### Corollaire 1 {#alg-iii-s4-prop-10-cor-1 .statement}

*Avec les notations de la prop. 10 (III, p. 48), supposons en outre que F soit une A-algèbre graduée de type $\Delta$, et que chaque $f_i$ soit un homomorphisme d’algèbres graduées relatif à $\varphi_i : \Delta_i \to \Delta$; alors $f = \varepsilon \bigotimes_{i \in I} f_i$ est un homomorphisme d’algèbres graduées.*

Cela résulte aussitôt de la définition de $f$ et du fait que $\sum_{i \in I} \varphi_i(\alpha_i) = (\alpha_i)$ par définition des $\varphi_i$.

On voit donc que $(E, \psi)$ est *aussi* solution d’un second problème d’application universelle, où $\Sigma$ est cette fois l’espèce de structure de *A-algèbre graduée de type* $\Delta$, les morphismes étant les homomorphismes d’algèbres graduées de type $\Delta$, et les $\alpha$-applications les applications $\prod_i f_i$, où en plus des conditions (26) de III, p. 47, on suppose que $f_i$ est un homomorphisme d’algèbres graduées relatif à $\varphi_i$.

#### Corollaire 2 {#alg-iii-s4-prop-10-cor-2 .statement}

Soient $(E_i)_{i \in I}, (F_i)_{i \in I}$ deux familles finies de $A$-algèbres, $E_i$ et $F_i$ étant graduées de type $\Delta_i$ pour tout $i \in I$. Pour chaque $i \in I$, soit $g_i : E_i \to F_i$ un homomorphisme d’algèbres graduées de type $\Delta_i$. Alors, si $h_i : E_i \to \varepsilon \bigotimes_{i \in I} E_i$ et $h'_i : F_i \to \varepsilon \bigotimes_{i \in I} F_i$ sont les homomorphismes canoniques, il existe un homomorphisme de $A$-algèbres graduées de type $\Delta$ et un seul, $g : \varepsilon \bigotimes_{i \in I} E_i \to \varepsilon \bigotimes_{i \in I} F_i$ tel que $g \circ h_i = h'_i \circ g_i$ pour tout $i \in I$. En outre, si chaque $g_i$ est bijectif, il en est de même de $g$.

Il suffit d’appliquer le cor. 1 aux $f_i = h'_i \circ g_i$, en remarquant que les conditions (26) (III, p. 47) découlent alors des relations (25) (III, p. 47) appliquées aux $h'_i$.

On notera encore (si aucune confusion n’en résulte) $\varepsilon \bigotimes_i g_i$ l’homomorphisme défini dans le cor. 2; si pour chaque $i \in I$, $G_i$ est une troisième $A$-algèbre graduée de type $\Delta_i$, et $g'_i : F_i \to G_i$ un homomorphisme d’algèbres graduées, on a
$$
(\varepsilon \bigotimes_i g'_i) \circ (\varepsilon \bigotimes_i g_i) = \varepsilon \bigotimes_i (g'_i \circ g_i)
$$
comme il résulte aussitôt de (30) (III p. 48).

Lorsqu’il s’agit du produit tensoriel gauche d’algèbres graduées de type $\mathbf{Z}$, on écrit $\varepsilon \bigotimes_i f_i$ au lieu de $\varepsilon \bigotimes_i f_i$ pour des homomorphismes $f_i : E_i \to F_i$ d’algèbres graduées de type $\mathbf{Z}$; quand $I = \{1, 2\}$, on écrit aussi $f_1 \varepsilon \otimes f_2$ cet homomorphisme; quand $I = \{1, n\}$, que tous les $E_i$ (resp. $F_i$) sont égaux et tous les $f_i$ égaux à un même homomorphisme $f$, on écrit $\varepsilon f^{\otimes n}$.

#### Remarque {#alg-iii-s4-n7-rem-2 .statement}

Dans la démonstration de la prop. 10 (III, p. 47), on s’est servi d’une relation d’ordre total sur $I$ pour définir une structure d’algèbre sur le produit tensoriel $\bigotimes_{i \in I} E_i$ des $A$-modules $E_i$. Si l’on change la relation d’ordre sur $I$, on trouve une autre structure multiplicative sur $\bigotimes_{i \in I} E_i$, mais la nouvelle algèbre ainsi obtenue est canoniquement isomorphe à la précédente, puisque l’une et l’autre sont solutions du même problème d’application universelle. Par exemple, lorsque $I = \{1, 2\}$, l’isomorphisme canonique de l’algèbre $E_1 \varepsilon \otimes_A E_2$ sur l’algèbre $E_2 \varepsilon \otimes_A E_1$ transforme $x_1 \otimes x_2$ en $\varepsilon_{2,1}(\alpha, \beta)x_2 \otimes x_1$, pour $x_1$ homogène de degré $\alpha$ et $x_2$ homogène de degré $\beta$.

Soit $J$ une partie de $I$, et, pour chaque $i \in J$, considérons l’homomorphisme canonique $h_i : E_i \to \varepsilon \bigotimes_{i \in I} E_i = E$. En vertu des relations (25) de III, p. 47, on déduit canoniquement (par la prop. 10 de III, p. 47) de ces homomorphismes un homomorphisme canonique $h : E' = \varepsilon \bigotimes_{i \in J} E_i \to E$ tel que pour tout $i \in J$, $h'_i = h \circ h_i$, $h'_i$ étant l’homomorphisme canonique $E_i \to E'$. Si l’on prend sur $J$ l’ordre total induit par celui choisi sur $I$, on a
$$
h(\bigotimes_{i \in J} x_i) = \prod_{i \in I} h_i(x_i) = \bigotimes_{i \in I} x'_i
$$

où le second membre est le produit de la séquence $(h_i(x_i))_{i \in J}$, et où dans le troisième membre, $x'_i = x_i$ pour $i \in J$, $x'_i = e_i$ pour $i \notin J$.

**Proposition 11** (« associativité » du $\varepsilon$-produit tensoriel). — *Avec les notations de la prop. 10 (III, p. 47), soit $(J_\lambda)_{\lambda \in L}$ une partition de $I$, et posons $\Delta'_\lambda = \prod_{i \in J_\lambda} \Delta_i$ pour tout $\lambda \in L$. Soit $E'_\lambda$ un $\varepsilon$-produit tensoriel gradué de type $\Delta'_\lambda$ de la famille $(E_i)_{i \in J_\lambda}$ (pour un ordre total choisi sur $J_\lambda$). D’autre part, pour $\lambda, \mu$ dans $L$ et $\lambda \neq \mu$, posons, pour $\alpha'_\lambda = (\alpha_i)_{i \in J_\lambda}$, $\beta'_\mu = (\beta_j)_{j \in J_\mu}$,

$$
\varepsilon'_{\lambda \mu}(\alpha'_\lambda, \beta'_\mu) = \prod_{i \in J_\lambda, j \in J_\mu} \varepsilon_{ij}(\alpha_i, \beta_j).
$$

Alors $(\varepsilon'_{\lambda \mu})$ est un système de facteurs de commutation sur les $\Delta'_\lambda$ à valeurs dans $A$, et il existe un homomorphisme et un seul d’algèbres graduées de type $\Delta$, $v : \varepsilon' \bigotimes_{\lambda \in L} E'_\lambda \to \varepsilon \bigotimes_{i \in I} E_i$, tel que

$$
v\left( \bigotimes_{\lambda \in L} \left( \bigotimes_{i \in J_\lambda} x_i \right) \right) = \bigotimes_{i \in I} x_i
$$

pour tout $(x_i) \in \prod_{i \in I} E_i$, pourvu que l’on prenne sur $I$ l’ordre total qui induit sur chaque $J_\lambda$ l’ordre total choisi, et qui est tel que pour $\lambda < \mu$ dans $L$, $i \in J_\lambda$ et $j \in J_\mu$, on ait $i < j$.

Le fait que les $\varepsilon'_{\lambda \mu}$ forment un système de facteurs de commutation est trivial. Soient $h_{i,\lambda} : E_i \to E'_\lambda$, $h'_\lambda : E'_\lambda \to \varepsilon' \bigotimes_{\lambda \in L} E'_\lambda$ les homomorphismes canoniques (pour $\lambda \in L, i \in J_\lambda$), et posons $h''_i = h'_\lambda \circ h_{i,\lambda}$; il suffira, en vertu de l’unicité de la solution d’un problème d’application universelle, de montrer que $\varepsilon' \bigotimes_{\lambda \in L} E'_\lambda$ et les $h''_i$ vérifient les conditions de la prop. 10 (III, p. 47). Or, pour tout $\lambda \in L$, soit $f'_\lambda : E'_\lambda \to F$ l’unique homomorphisme d’algèbres tel que $f'_\lambda \circ h_{i,\lambda} = f_i$ pour tout $i \in J_\lambda$. Montrons que, pour $\lambda \neq \mu$, $\alpha'_\lambda = (\alpha_i)_{i \in J_\lambda}$, $\beta'_\mu = (\beta_j)_{j \in J_\mu}$, on a

$$
f'_\lambda(x'_\lambda) f'_\mu(x'_\mu) = \varepsilon'_{\lambda \mu}(\alpha'_\lambda, \beta'_\mu) f'_\mu(x'_\mu) f'_\lambda(x'_\lambda)
$$

pour $x'_\lambda \in E'_\lambda$ (resp. $x'_\mu \in E'_\mu$) homogène de degré $\alpha'_\lambda$ (resp. $\beta'_\mu$); il suffit, par linéarité, de le voir lorsque $x'_\lambda = \bigotimes_{i \in J_\lambda} x_i$, $x'_\mu = \bigotimes_{j \in J_\mu} x_j$, $x_i$ (resp. $x_j$) étant homogène de degré $\alpha_i$ (resp. $\beta_j$) dans $E_i$ (resp. $E_j$) pour $i \in J_\lambda, j \in J_\mu$. Mais cela résulte de la formule (30) (III, p. 48) qui définit les $f'_\lambda$, et du lemme 3 de III, p. 45, compte tenu de l’hypothèse (26) (III, p. 47) et de la définition (32). Il y a donc un homomorphisme d’algèbres et un seul $f : \varepsilon' \bigotimes_{\lambda \in L} E'_\lambda \to F$ tel que $f \circ h'_\lambda = f'_\lambda$ pour tout $\lambda \in L$; d’où $f \circ h''_i = f_i$ pour tout $i \in I$, et l’unicité de $f$ est triviale.

### 8. Produit tensoriel d’algèbres graduées de mêmes types

Les hypothèses de III, p. 47, prop. 10 étant supposées vérifiées, supposons en outre que tous les $\Delta_i$ soient égaux à un même monoïde commutatif $\Delta_0$; on peut alors considérer sur le $\varepsilon$-produit tensoriel $\varepsilon \bigotimes_{i \in I} E_i$ la graduation totale de type $\Delta_0$, associée à la graduation de type $\Delta = \Delta_0^I$ sur cette algèbre (II, p. 164); nous dirons que $\varepsilon \bigotimes_{i \in I} E_i$, munie de cette graduation, est un $\varepsilon$-produit tensoriel gradué de type $\Delta_0$ de la famille $(E_i)_{i \in I}$ d’algèbres graduées de type $\Delta_0$.

Conservant toujours les notations de la prop. 10 de III, p. 47, supposons que F soit aussi une A-algèbre graduée de type $\Delta_0$ et que les $f_i$ soient des homomorphismes d’algèbres graduées de type $\Delta_0$. Alors $f : \varepsilon \bigotimes_{i \in I} E_i \to F$ est aussi un homomorphisme d’algèbres graduées de type $\Delta_0$: il résulte en effet de la formule (30) (III, p. 48) que si $x_i$ est homogène et de degré $\alpha_i \in \Delta_0$, $\bigotimes_{i \in I} x_i$ et $\prod_{i \in I} f_i(x_i)$ sont tous deux homogènes de degré $\sum_{i \in I} \alpha_i \in \Delta_0$.

On peut donc dire que $\varepsilon \bigotimes_{i \in I} E_i$, muni de la graduation totale de type $\Delta_0$, constitue, avec l’application canonique $\psi$, une solution d’un troisième problème d’application universelle, où $\Sigma$ est l’espèce de structure de A-algèbre graduée de type $\Delta_0$, les morphismes les homomorphismes d’algèbres graduées de type $\Delta_0$, et les $\alpha$-applications les applications $\prod_i f_i$ où, en plus des conditions (26) (de III, p. 47), on suppose que chaque $f_i$ est un homomorphisme d’algèbres graduées de type $\Delta_0$.

Pour toute partie J de I, l’homomorphisme canonique $\varepsilon \bigotimes_{i \in J} E_i \to \varepsilon \bigotimes_{i \in I} E_i$ (III, p. 50) est, dans le cas actuel, un homomorphisme d’algèbres graduées de type $\Delta_0$, comme il résulte de ce qui précède.

#### Proposition 12 (« associativité » du $\varepsilon$-produit tensoriel d’algèbres graduées de mêmes types) {#alg-iii-s4-prop-12 .statement}

Avec les notations de III, p. 47, prop. 10, supposons que tous les $\Delta_i$ soient égaux à un même monoïde $\Delta_0$; soit $(J_\lambda)_{\lambda \in L}$ une partition de I. Avec les notations de la prop. 11 de III, p. 51, supposons que le second membre de la formule (32) (III, p. 51) ne dépende que des sommes $\alpha''_\lambda = \sum_{i \in J_\lambda} \alpha_i, \beta''_\mu = \sum_{j \in J_\mu} \beta_j$, pour tout couple $(\lambda, \mu)$ d’indices distincts, tout $\alpha'_\lambda \in \Delta'_\lambda$ et tout $\beta'_\mu \in \Delta'_\mu$; désignons par $\varepsilon''_{\lambda \mu}(\alpha''_\lambda, \beta''_\mu)$ le second membre de (32). Alors $(\varepsilon''_{\lambda \mu})$ est un système de facteurs de commutation sur la famille $(\Delta''_\lambda)_{\lambda \in L}$, où $\Delta''_\lambda = \Delta_0$ pour tout $\lambda \in L$. Si $E''_\lambda$ est le $\varepsilon$-produit tensoriel gradué de type $\Delta_0$ de la famille $(E_i)_{i \in J_\lambda}$, il existe un isomorphisme et un seul d’algèbres graduées de type $\Delta_0$, $w : \varepsilon'' \bigotimes_{\lambda \in L} E''_\lambda \to \varepsilon \bigotimes_{i \in I} E_i$, tel que
$$
w\left( \bigotimes_{\lambda \in L} \left( \bigotimes_{i \in J_\lambda} x_i \right) \right) = \bigotimes_{i \in I} x_i
$$
pourvu que l’on choisisse des ordres totaux sur les $J_\lambda$ et sur I de la façon décrite dans III, p. 51, prop. 11.

En vertu de l’hypothèse, pour $\gamma, \delta$ dans $\Delta_0$, on a $\varepsilon''_{\lambda \mu}(\gamma, \delta) = \varepsilon_{i_0 j_0}(\gamma, \delta)$ pour un $i_0 \in J_\lambda$ et un $j_0 \in J_\mu$, comme on le voit en considérant les éléments $\alpha'_\lambda = (\alpha_i)_{i \in J_\lambda}$ et $\beta'_\mu = (\beta_j)_{j \in J_\mu}$ tels que $\alpha_{i_0} = \gamma, \alpha_i = 0$ pour $i \neq i_0$, $\beta_{j_0} = \delta, \beta_j = 0$ pour $j \neq j_0$; il en résulte aussitôt que les $\varepsilon''_{\lambda \mu}$ forment un système de facteurs de commutation. Le reste de la démonstration est alors analogue à celle de la prop. 11 (III, p. 51), et est laissé au lecteur.

On notera que les hypothèses supplémentaires de la prop. 12 sont remplies lorsque $\Delta_0 = \mathbf{Z}$ et que $(\varepsilon_{ij})$ est, soit le système de facteurs trivial $(\varepsilon_{ij}(\alpha_i, \beta_j) = 1$ quels que soient $i, j$), soit le système de facteurs défini par $\varepsilon_{ij}(\alpha_i, \beta_j) = (-1)^{\alpha_i \beta_j}$; dans ce dernier cas, le second membre de la formule (32) est en effet égal à $(-1)^{\gamma}$, avec $\gamma = \sum_{i \in J_\lambda, j \in J_\mu} \alpha_i \beta_j = (\sum_{i \in J_\lambda} \alpha_i)(\sum_{j \in J_\mu} \beta_j)$.

#### Remarque 1 {#alg-iii-s4-n8-rem-1 .statement}

Soit I un ensemble infini d’indices, $\Delta_0$ un monoïde commutatif; désignons par $(\Delta_i)_{i \in I}$ la famille telle que $\Delta_i = \Delta_0$ pour tout $i$, et supposons donnée, pour tout couple d’indices distincts $(i, j)$ de I, une application $\varepsilon_{ij}: \Delta_i \times \Delta_j \to A$ vérifiant les conditions (22), (23) et (24) (III, p. 46); nous dirons encore que c’est un système de facteurs de commutation sur la famille $(\Delta_i)$. Considérons une famille $(E_i)_{i \in I}$ de A-algèbres graduées de type $\Delta_0$; pour chaque partie finie J de I, désignons par $E_J$ un $\varepsilon$-produit tensoriel gradué de type $\Delta_0$ de la sous-famille $(E_i)_{i \in J}$ (avec un choix arbitraire d’un ordre total sur J). Si J, J' sont deux parties finies de I telles que $J \subset J'$, on a défini ci-dessus un homomorphisme canonique d’algèbres graduées de type $\Delta_0$, $h_{J',J}: E_J \to E_{J'}$, et les propriétés d’unicité de ces homomorphismes montrent aussitôt que si $J \subset J' \subset J''$ sont trois parties finies de I, on a $h_{J'',J} = h_{J'',J'} \circ h_{J',J}$. On a donc un système inductif $(E_J, h_{J',J})$ d’algèbres graduées de type $\Delta_0$ (III, p. 32), dont l’ensemble d’indices est l’ensemble filtrant croissant $\mathcal{F}(I)$ des parties finies de I. L’algèbre graduée de type $\Delta_0$, limite inductive de ce système inductif (III, p. 33) est appelée un $\varepsilon$-produit tensoriel gradué de type $\Delta_0$ de la famille $(E_i)_{i \in I}$; on le note encore $\varepsilon \bigotimes_{i \in I} E_i$. Lorsque tous les $\Delta_i$ sont égaux à $\mathbf{Z}$ et $\varepsilon_{ij}(\alpha_i, \beta_j) = (-1)^{\alpha_i \beta_j}$, on dit encore que le produit tensoriel $\varepsilon \bigotimes_{i \in I} E_i$ est le produit tensoriel gauche de la famille $(E_i)_{i \in I}$ et on le note $^g \bigotimes_{i \in I} E_i$. Nous laissons au lecteur le soin de formuler et de démontrer la proposition qui généralise au cas où I est infini la prop. 10 de III, p. 47, comme la prop. 8 de III, p. 42 généralise au cas où I est infini la prop. 5 de III, p. 36. On notera que le A-module sous-jacent à $\varepsilon \bigotimes_{i \in I} E_i$ est le même que celui sous-jacent au produit tensoriel (non gradué) de la famille $(E_i)_{i \in I}$ d’algèbres non graduées, défini dans III, p. 42.

#### Remarque 2 {#alg-iii-s4-n8-rem-2 .statement}

Soient E une A-algèbre graduée de type $\Delta_0$ (où $\Delta_0$ est un monoïde commutatif), et $\rho: A \to B$ un homomorphisme d’anneaux; la graduation de $\rho^*(E)$ (II, p. 174) est identique à la graduation du produit tensoriel gradué $B \otimes_A E$, où B est muni de la graduation triviale.

### 9. Algèbres anticommutatives et algèbres alternées

#### Définition 7 {#alg-iii-s4-def-7 .statement}

On dit qu’une A-algèbre graduée E de type $\mathbf{Z}$ est anticommutative si, quels que soient les éléments homogènes non nuls x, y de E, on a

(36) $$ xy = (-1)^{\deg(x)\deg(y)} yx. $$

On dit que l’algèbre E est alternée si elle est anticommutative et si de plus $x^2 = 0$ pour tout élément homogène $x \in E$ de degré impair.

#### Remarque 1 {#alg-iii-s4-n9-rem-1 .statement}

Soit $E^+$ la sous-algèbre graduée de $E$ somme directe des $E_{2n}$ ($n \in \mathbf{Z}$); il résulte de la déf. 7 que si $E$ est anticommutative, $E^+$ est une sous-algèbre contenue dans le centre de $E$ (donc commutative).

#### Remarque 2 {#alg-iii-s4-n9-rem-2 .statement}

Supposons que 2 ne soit pas diviseur de 0 dans $E$; alors si $E$ est anticommutative, $E$ est alternée, car pour $x \in E$ homogène et de degré impair, on a $x^2 = -x^2$ d’après (36), d’où $2x^2 = 0$, et $x^2 = 0$ en vertu de l’hypothèse.

#### Remarque 3 {#alg-iii-s4-n9-rem-3 .statement}

Nous étudierons en détail dans III, p. 76 à 90, des exemples importants d’algèbres alternées.

#### Lemme 4 {#alg-iii-s4-lem-4 .statement}

Soient $E$ une algèbre graduée du type $\mathbf{Z}$, $S$ un ensemble d’éléments homogènes $\neq 0$; l’ensemble $F$ des éléments de $E$ dont toutes les composantes homogènes $x \neq 0$ satisfont à la relation (36) (III, p. 53) pour tout $y \in S$, est une sous-algèbre graduée de $E$.

Il suffit de noter que: 1° si $x', x''$ sont deux éléments homogènes de même degré $p$, $y$ un élément homogène de degré $q$, et si $x'y = (-1)^{pq}yx'$, $x''y = (-1)^{pq}yx''$, on a aussi $(x' + x'')y = (-1)^{pq}y(x' + x'')$; 2° si $x', x''$ sont deux éléments homogènes de degrés respectifs $p', p''$, $y$ un élément homogène de degré $q$, et si $x'y = (-1)^{p'q}yx'$, $x''y = (-1)^{p''q}yx''$, on a $(x'x'')y = (-1)^{(p' + p'')q}y(x'x'')$.

#### Proposition 13 {#alg-iii-s4-prop-13 .statement}

Soient $E$ une $A$-algèbre graduée de type $\mathbf{Z}$, $S$ un système générateur de l’algèbre $E$ formé d’éléments homogènes $\neq 0$; pour que $E$ soit anticommutative (resp. alternée), il faut et il suffit que (36) (III, p. 53) soit vérifiée, quels que soient $x \in S$ et $y \in S$ (resp. que cette condition soit vérifiée et en outre que $x^2 = 0$ pour tout $x$ homogène de degré impair appartenant à $S$).

Considérons d’abord le cas des algèbres anticommutatives. En vertu du lemme 4, la sous-algèbre $F$ formée des éléments dont toute les composantes homogènes $x \neq 0$ satisfont à (36) (III, p. 53) pour tout $y \in S$, contient tous les éléments de $S$, donc $F = E$. Si maintenant $F'$ est de même la sous-algèbre de $E$ formée des éléments dont toutes les composantes homogènes $x \neq 0$ satisfont à (36) pour tout élément homogène $y \neq 0$ de $E$, il résulte de ce qui précède que $F'$ contient tous les éléments de $S$, donc $F' = E$, ce qui prouve la proposition dans ce cas.

Pour prouver la proposition dans le cas des algèbres alternées, on peut déjà supposer $E$ anticommutative; il est immédiat alors que tout élément homogène de degré impair de $E$ est de la forme $\sum_i z_i x_i$, où $z_i \in E^+$ et $x_i \in S$ est de degré impair (utilisant le fait que $E^+$ est contenu dans le centre de $E$); on en déduit $\left( \sum_i z_i x_i \right)^2 = \sum_i z_i^2 x_i^2 + \sum_{i < j} z_i z_j (x_i x_j + x_j x_i) = 0$ puisque $x_i^2 = 0$ par hypothèse et $x_i x_j + x_j x_i = 0$ en vertu de (36).

#### Proposition 14 {#alg-iii-s4-prop-14 .statement}

Soient $E$ et $F$ deux $A$-algèbres graduées de type $\mathbf{Z}$, toutes deux anticommutatives (resp. alternées). Alors le produit tensoriel gauche $E \mathop{\otimes}\limits_A F$ (III, p. 49) est (une algèbre) anticommutative (resp. alternée).

En effet, un système générateur de $E \mathop{\otimes}\limits_A F$ est formé des $x \otimes y$, où $x$ (resp. $y$) est un élément homogène $\neq 0$ de $E$ (resp. $F$). Considérons deux tels éléments $x \otimes y, x' \otimes y'$, avec $\deg(x) = p, \deg(y) = q, \deg(x') = p', \deg(y') = q'$, de sorte que $x \otimes y$ est de degré $p + q$ et $x' \otimes y'$ de degré $p' + q'$. On a par définition (III, p. 47, formule (27)), et en vertu de (36) (III, p. 53)

$$
\begin{align*}
(x \otimes y)(x' \otimes y') &= (-1)^{qp'}(xx') \otimes (yy') \\
(x' \otimes y')(x \otimes y) &= (-1)^{pq'}(x'x) \otimes (y'y) \\
&= (-1)^{pq' + pp' + qq'}(xx') \otimes (yy')
\end{align*}
$$

et le critère de la prop. 13 (III, p. 54) montre que $E^g \otimes_A F$ est anticommutative puisque $pq' + pp' + qq' - qp' \equiv (p + q)(p' + q')$ (mod. 2). Si de plus E et F sont alternées et $p + q$ impair, un des nombres $p, q$ est nécessairement impair, donc $(x \otimes y)^2 = \pm (x^2) \otimes (y^2) = 0$, et la prop. 13 montre que $E^g \otimes_A F$ est alternée.

#### Corollaire {#alg-iii-s4-n9-cor-1 .statement}

*Soit E une A-algèbre graduée de type $\mathbf{Z}$, anticommutative (resp. alternée). Alors, pour tout homomorphisme d’anneaux $\rho : A \to B$, la B-algèbre graduée $\rho^*(E)$ (III, p. 53, Remarque 2) est anticommutative (resp. alternée)*.

En effet, l’anneau B, muni de la graduation triviale, peut être considéré comme une A-algèbre alternée, et $\rho^*(E) = E^g \otimes_A B$, donc on peut appliquer la prop. 14.

#### Remarque {#alg-iii-s4-n9-rem-4 .statement}

Soit E une A-algèbre graduée de type $\mathbf{Z}$ anticommutative. Alors l’application A-linéaire de $E \otimes_A E$ dans E définie par la multiplication de E (III, p. 5) est un homomorphisme de la A-algèbre graduée $E^g \otimes_A E$ dans E, car avec les notations de la prop. 14, on a, dans l’algèbre E, $(xy)(x'y') = (-1)^{qp'}(xx')(yy')$.

## EXERCICES {#alg-iii-s4-exercises}

See the [exercises for § 4](exercises/s4/).
