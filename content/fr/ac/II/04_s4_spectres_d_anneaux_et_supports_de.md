---
book: ac
book_title: Commutative Algebra
chapter: II
chapter_title: Localisation
section: 4
section_title: Spectres d’anneaux et supports de modules
lang: fr
source: ac-i-iv-fr
pdf_pages: 0117-0134, 0168-0174
extraction: ocr
subsections:
    - "no": 1
      title: Espaces irréductibles.
      page: 0
      pdf_page: 117
    - "no": 2
      title: Espaces topologiques nœthériens
      page: 0
      pdf_page: 121
    - "no": 3
      title: Le spectre premier d’un anneau
      page: 0
      pdf_page: 122
    - "no": 4
      title: Support d’un module
      page: 0
      pdf_page: 130
statements: 51
exercises: 17
content_sha256: 09d8c983ce499791dac38520e1e02e0a00fce9a93da53ad207057672940643e7
---

## § 4. Spectres d’anneaux et supports de modules

### 1. Espaces irréductibles.

#### Définition 1 {#ac-ii-s4-def-1 .statement}

On dit qu’un espace topologique X est irréductible si toute intersection finie d’ensembles ouverts non vides de X est non vide.

En considérant la famille vide d’ensembles ouverts de X, on voit qu’un espace irréductible est non vide ; pour qu’un espace topologique X soit irréductible, il faut et il suffit qu’il soit non vide et que l’intersection de deux ensembles ouverts non vides de X soit toujours non vide (ou, ce qui revient au même, que la réunion de deux ensembles fermés distincts de X soit toujours distincte de X).

#### Proposition 1 {#ac-ii-s4-prop-1 .statement}

Soit X un espace topologique non vide. Les conditions suivantes sont équivalentes :
a) X est irréductible ;
b) tout ensemble ouvert non vide de X est dense dans X ;
c) tout ensemble ouvert de X est connexe.

Par définition, un ensemble dense dans X est un ensemble qui rencontre tout ensemble ouvert non vide, donc a) et b) sont équivalentes. Il est immédiat que c) entraîne a), car si U₁ et U₂ sont des ensembles ouverts non vides disjoints, U₁ ∪ U₂ est un ensemble ouvert non connexe. Montrons enfin que a) entraîne c) : si U est un ensemble ouvert non connexe, il est réunion de deux ensembles non vides disjoints U', U'' qui sont ouverts dans U, donc aussi ouverts dans X, ce qui implique que X n’est pas irréductible.

Un espace séparé n’est irréductible que s’il est réduit à un seul point.

On dit qu’une partie E d’un espace topologique X est un ensemble irréductible si le sous-espace E de X est irréductible. Pour qu’il en soit ainsi, il faut et il suffit que, pour tout couple d’ensembles U, V ouverts dans X et rencontrant E, U ∩ V rencontre aussi E, ou (ce qui revient au même) que, pour tout couple d’ensembles F, G fermés dans X et tels que E ⊂ F ∪ G, on ait E ⊂ F ou E ⊂ G. Par récurrence sur n, on en déduit que, si (F_i)_{1 \leq i \leq n} est une famille finie d’ensembles fermés dans X, tels que E ⊂ \bigcup_{i=1}^{n} F_i, il existe un indice i tel que E ⊂ F_i.

#### Proposition 2 {#ac-ii-s4-prop-2 .statement}

Dans un espace topologique X, pour qu’un ensemble E soit irréductible, il faut et il suffit que son adhérence \overline{E} le soit.

En effet, pour qu’un ensemble ouvert de X rencontre E, il faut et il suffit qu’il rencontre \overline{E}, et la proposition résulte des remarques précédentes.

#### Proposition 3 {#ac-ii-s4-prop-3 .statement}

(i) Si X est un espace irréductible, tout ensemble ouvert non vide de X est irréductible.

(ii) Soit (U_\alpha)_{\alpha \in A} un recouvrement non vide d’un espace topologique X, formé d’ensembles ouverts tels que U_\alpha \cap U_\beta \neq \emptyset pour tout couple d’indices (\alpha, \beta). Si les ensembles U_\alpha sont irréductibles, l’espace X est irréductible.

(i) Si X est irréductible, U ⊂ X ouvert non vide dans X et V ⊂ U ouvert non vide dans U, V est aussi ouvert dans X, donc dense dans X et a fortiori dans U. Donc U est irréductible (prop. 1).

(ii) Montrons que, pour tout ensemble V ouvert dans X et non vide, on a V \cap U_\alpha \neq \emptyset pour tout \alpha \in A : il en résultera que V \cap U_\alpha est dense dans U_\alpha par hypothèse, donc que V est dense dans X, et cela prouvera que X est irréductible (prop. 1). Or il existe au moins un indice \gamma tel que V \cap U_\gamma \neq \emptyset ; comme U_\alpha \cap U_\gamma \neq \emptyset pour tout \alpha, et que V \cap U_\gamma est dense dans U_\gamma, on a U_\alpha \cap U_\gamma \cap V \neq \emptyset et a fortiori U_\alpha \cap V \neq \emptyset, ce qui achève la démonstration de (ii).

#### Proposition 4 {#ac-ii-s4-prop-4 .statement}

Soient X et Y deux espaces topologiques, f une application continue de X dans Y. Pour toute partie irréductible E de X, f(E) est une partie irréductible de Y.

En effet, si U, V sont deux ensembles ouverts dans Y rencontrant f(E), f^{-1}(U) et f^{-1}(V) sont des ensembles ouverts dans X rencontrant E. Par suite $f^{-1}(U) \cap f^{-1}(V) = f^{-1}(U \cap V)$ rencontre E, ce qui entraîne que $U \cap V$ rencontre $f(E)$ et démontre la proposition.

#### Définition 2 {#ac-ii-s4-def-2 .statement}

On appelle composante irréductible d’un espace topologique X toute partie irréductible maximale de X.

Il résulte de la prop. 2 que toute composante irréductible de X est fermée dans X.

#### Proposition 5 {#ac-ii-s4-prop-5 .statement}

Soit X un espace topologique. Toute partie irréductible de X est contenue dans une composante irréductible de X, et X est réunion de ses composantes irréductibles.

Pour démontrer la première assertion, il suffit, en vertu du th. de Zorn, de prouver que l’ensemble $\mathfrak{J}$ des parties irréductibles de X est inductif. Soit $\mathfrak{G}$ une partie de $\mathfrak{J}$ totalement ordonnée par inclusion ; montrons que la réunion E des ensembles $F \in \mathfrak{G}$ est irréductible. Soient U, V deux ensembles ouverts dans X et rencontrant E ; comme $\mathfrak{G}$ est totalement ordonnée, il existe un ensemble $F \in \mathfrak{G}$ rencontrant U et V ; comme F est irréductible, $U \cap V$ rencontre F, donc aussi E, ce qui prouve que E est irréductible, donc que $\mathfrak{J}$ est inductif. La seconde assertion résulte de la première, car toute partie de X réduite à un seul point est irréductible.

#### Corollaire {#ac-ii-s4-n1-cor-1 .statement}

Toute composante connexe d’un espace topologique X est réunion de composantes irréductibles de X.

En effet, tout sous-espace irréductible de X est connexe en vertu de la prop. 1, donc contenu dans une composante connexe de X.

On notera que deux composantes irréductibles distinctes de X peuvent avoir des points communs (exerc. 11).

#### Proposition 6 {#ac-ii-s4-prop-6 .statement}

Soient X un espace topologique, $(P_i)_{1 \leq i \leq n}$ un recouvrement fini de X formé d’ensembles fermés irréductibles. Alors les composantes irréductibles de X sont les éléments maximaux (pour la relation d’inclusion) de l’ensemble des $P_i$.

On peut se borner au cas où les $P_i$ sont deux à deux incomparables. Si E est une partie irréductible de X, on a $E \subset \bigcup_{i=1}^{n} P_i$, donc E est contenu dans l’un des ensembles fermés $P_i$; cela prouve que les $P_i$ sont les seules parties irréductibles maximales de X.

#### Corollaire {#ac-ii-s4-n1-cor-2 .statement}

Soient X un espace topologique, E un sous-espace de X n’ayant qu’un nombre fini de composantes irréductibles distinctes $Q_i$ ($1 \leq i \leq n$); alors les composantes irréductibles de l’adhérence $\overline{E}$ dans X sont les adhérences $\overline{Q_i}$ des $Q_i$ ($1 \leq i \leq n$) et on a $\overline{Q_i} \neq \overline{Q_j}$ pour $i \neq j$.

En effet, $\overline{E}$ est la réunion des $\overline{Q_i}$, qui sont irréductibles (prop. 2); comme $Q_i$ est fermé dans E, on a $\overline{Q_i} \cap E = Q_i$; comme $Q_i \notin Q_j$ pour $i \neq j$, on a $\overline{Q_i} \notin \overline{Q_j}$, d’où le corollaire, en vertu de la prop. 6.

#### Remarque {#ac-ii-s4-n1-rem-1 .statement}

Supposons que X n’ait qu’un nombre fini de composantes irréductibles distinctes $X_i$ ($1 \leq i \leq n$); alors $U_i = \mathbf{C} \left( \bigcup_{j \neq i} X_j \right)$ est ouvert dans X et dense dans $X_i$ puisque $X_i \notin \bigcup_{j \neq i} X_j$; les $U_i$ ($1 \leq i \leq n$) sont donc des ouverts non vides de X, irréductibles (prop. 2), deux à deux disjoints, et dont la réunion est dense dans X.

#### Proposition 7 {#ac-ii-s4-prop-7 .statement}

Soit U une partie ouverte d’un espace topologique X. L’application $V \to \overline{V}$ (adhérence dans X) est une bijection de l’ensemble des parties irréductibles de U, fermées dans U, sur l’ensemble des parties irréductibles de X, fermées dans X et rencontrant U ; la bijection réciproque est $Z \to Z \cap U$. En particulier, cette bijection applique l’ensemble des composantes irréductibles de U sur l’ensemble des composantes irréductibles de X rencontrant U.

En effet, si V est fermée dans U et irréductible, $\overline{V}$ est irréductible (prop. 2) et l’on a $V = \overline{V} \cap U$. Inversement, si Z est irréductible, fermé dans X et rencontre U, $Z \cap U$ est un ouvert non vide dans Z, donc est irréductible (prop. 3), dense dans Z, et, comme Z est fermé, on a $Z = \overline{Z \cap U}$. Cela démontre la proposition.

### 2. Espaces topologiques nœthériens

#### Définition 3 {#ac-ii-s4-def-3 .statement}

On dit qu’un espace topologique X est nœthérien si tout ensemble non vide de parties fermées de X, ordonné par inclusion, possède un élément minimal.

Il revient au même de dire que tout ensemble non vide de parties ouvertes de X, ordonné par inclusion, possède un élément maximal, ou que toute suite décroissante (resp. croissante) d’ensembles fermés (resp. ouverts) est stationnaire (Ens., chap. III, § 6, no 5, prop. 6).

#### Proposition 8 {#ac-ii-s4-prop-8 .statement}

(i) Tout sous-espace d’un espace nœthérien est nœthérien.

(ii) Soit $(A_i)_{i \in I}$ un recouvrement fini d’un espace topologique X. Si les sous-espaces $A_i$ de X sont nœthériens, X est nœthérien.

(i) Soient X un espace nœthérien, A un sous-espace de X, $(F_n)$ une suite décroissante de parties de A, fermées dans A ; on a donc $F_n = \overline{F_n} \cap A$, et les adhérences $\overline{F_n}$ des $F_n$ dans X forment une suite décroissante de parties fermées de X. Comme cette suite est stationnaire, il en est de même de la suite $(F_n)$.

(ii) Soit $(G_n)_{n \geq 0}$ une suite décroissante de parties fermées de X ; par hypothèse, chacune des suites $(G_n \cap A_i)_{n \geq 0}$ est stationnaire. Comme I est fini, il y a un entier $n_0$ tel que, pour $n \geq n_0$, on ait $G_n \cap A_i = G_{n_0} \cap A_i$ pour tout $i \in I$. Mais $G_n = \bigcup_{i \in I} (G_n \cap A_i)$, donc la suite $(G_n)$ est stationnaire, et X est nœthérien.

#### Proposition 9 {#ac-ii-s4-prop-9 .statement}

Pour qu’un espace topologique X soit nœthérien, il faut et il suffit que tout ensemble ouvert dans X soit quasi-compact.

Pour démontrer que la condition est nécessaire, il suffit, en vertu de la prop. 8, de prouver que tout espace nœthérien X est quasi-compact. Soit $(U_t)_{t \in I}$ un recouvrement ouvert de X ; l’ensemble des réunions finies d’ensembles U_t est non vide et admet donc un élément maximal $V = \bigcup_{t \in H} U_t$, où H est une partie finie de I. Par définition, on a $V \cup U_t = V$ pour tout $t \in I$, donc $V = X$.

Réciproquement, supposons que tout ensemble ouvert dans X soit quasi-compact, et soit $(U_n)$ une suite croissante de parties ouvertes de X. La réunion V des $U_n$ est ouverte, donc quasi-compacte ; comme $(U_n)$ est un recouvrement ouvert de V, il y a une sous-famille finie de $(U_n)$ qui est un recouvrement de V, donc $V = U_n$ pour un indice n, ce qui prouve que la suite $(U_n)$ est stationnaire.

#### Lemme 1 (« principe de récurrence nœthérienne ») {#ac-ii-s4-lem-1 .statement}

Soient E un ensemble ordonné dont toute partie non vide admet un élément minimal. Soit F une partie de E ayant la propriété suivante : si $a \in E$ est tel que la relation $x < a$ entraîne $x \in F$, alors $a \in F$. On a alors $F = E$.

En effet, supposons $F \neq E$; alors $\mathcal{C}F$ aurait un élément minimal b. Par définition, on a $x \in F$ pour tout $x < b$, ce qui entraîne $b \in F$, d’où contradiction.

#### Proposition 10 {#ac-ii-s4-prop-10 .statement}

Si X est un espace nœthérien, l’ensemble des composantes irréductibles de X (et a fortiori l’ensemble des composantes connexes de X) est fini.

Il suffit de prouver que X est réunion finie de parties fermées irréductibles (n° 1, prop. 6). Montrons qu’on peut appliquer le principe de récurrence nœthérienne en prenant pour E l’ensemble des parties fermées de X, ordonné par inclusion, pour F l’ensemble des réunions finies de parties fermées irréductibles. Soit Y une partie fermée de X telle que toute partie fermée $\neq Y$ de Y appartienne à F. Si Y est irréductible, on a $Y \in F$ par définition ; sinon, Y est réunion de deux parties fermées $Y_1, Y_2$ distinctes de Y. On a donc $Y_1 \in F$ et $Y_2 \in F$ par hypothèse, d’où $Y \in F$ par définition de F.

Il en résulte en particulier qu’un espace nœthérien séparé est nécessairement fini.

### 3. Le spectre premier d’un anneau

Soient A un anneau, X l’ensemble des idéaux premiers de A. Pour toute partie M de A, nous noterons V(M) l’ensemble des idéaux premiers de A contenant M ; il est clair que, si α est l’idéal de A engendré par M, on a V(M) = V(α) ; si M est réduit à un seul élément f, on écrira V(f) au lieu de V({f}), et on a V(f) = V(Af). L’application M → V(M) est décroissante pour les relations d’inclusion dans A et X. En outre, on a les formules suivantes :

(1) $V(0) = X, \quad V(1) = \varnothing;$

(2) $V\left( \bigcup_{i \in I} M_i \right) = V(\sum M_i) = \bigcap_{i \in I} V(M_i)$

pour toute famille $(M_i)_{i \in I}$ de parties de A ;

(3) $V(\alpha \cap \alpha') = V(\alpha \alpha') = V(\alpha) \cup V(\alpha')$

pour tout couple d’idéaux $\alpha, \alpha'$ de A. En effet, les formules (1) et (2) sont évidentes ; d’autre part, la formule (3) signifie que, pour qu’un idéal premier p de A contienne l’un des idéaux $\alpha$ ou $\alpha'$, il faut et il suffit qu’il contienne $\alpha \alpha'$, ou qu’il contienne $\alpha \cap \alpha'$ ; elle résulte par suite du § 1, n° 1, prop. 1. La seconde formule (1) admet la réciproque suivante : si $\alpha$ est un idéal de A tel que $V(\alpha) = \varnothing$, alors $\alpha = A$, car il n’existe aucun idéal maximal de A contenant $\alpha$. Enfin, si $\alpha$ est un idéal de A et r($\alpha$) sa racine (\§ 2, n° 6, déf. 4), on a

(4) $V(\alpha) = V(r(\alpha))$

comme il résulte du § 2, n° 6, cor. 1 de la prop. 13.

Les formules (1) à (3) montrent que les parties $V(M)$ de X satisfont aux axiomes des ensembles fermés d’une topologie (Top, gén., chap. I, 3e éd., § 1, n° 4).

#### Définition 4 {#ac-ii-s4-def-4 .statement}

Soit A un anneau. On appelle spectre premier de A et on note Spec (A) l’ensemble X des idéaux premiers de A, muni de la topologie pour laquelle les ensembles fermés sont les ensembles $V(M)$ où M parcourt $\mathfrak{P}(A)$. La topologie ainsi définie s’appelle topologie spectrale ou topologie de Zariski sur X.

Il est clair que la relation Spec (A) = $\varnothing$ est équivalente à $A = \{0\}$.

Soit X le spectre premier d’un anneau A ; pour tout $f \in A$, notons $X_f$ l’ensemble des idéaux premiers de A ne contenant pas $f$ ;

on a $X_f = X - V(f)$, et $X_f$ est donc un ensemble ouvert. En vertu de (2), toute partie fermée de $X$ est intersection d'ensembles fermés de la forme $V(f)$, donc les $X_f$ forment une base de la topologie spectrale sur $X$. En outre, il résulte aussitôt des définitions que l'on a

$$
X_0 = \emptyset, \qquad X_1 = X,
$$

et plus généralement $X_f = X$ pour tout élément inversible $f$ de $A$;

$$
X_{fg} = X_f \cap X_g \text{ pour } f,\ g \text{ dans } A.
$$

Pour toute partie $Y$ de $X$, notons $\mathfrak{J}(Y)$ l'intersection des idéaux premiers de $A$ qui appartiennent à $Y$. Il est clair que $\mathfrak{J}(Y)$ est un idéal de $A$, et que l'application $Y \to \mathfrak{J}(Y)$ est décroissante pour les relations d'inclusion dans $X$ et dans $A$. On a évidemment les relations

$$
\mathfrak{J}(\emptyset) = A
$$
$$
\mathfrak{J}\left( \bigcup_{\lambda \in L} Y_\lambda \right) = \bigcap_{\lambda \in L} \mathfrak{J}(Y_\lambda)
$$

pour toute famille $(Y_\lambda)_{\lambda \in L}$ de parties de $X$. En outre :

#### Proposition 11 {#ac-ii-s4-prop-11 .statement}

*Soient A un anneau, a un idéal de A, Y une partie de X = Spec (A).*

(i) $V(a)$ est fermé dans $X$ et $\mathfrak{J}(Y)$ est un idéal de A égal à sa racine.

(ii) $\mathfrak{J}(V(a))$ est la racine de $a$, et $V(\mathfrak{J}(Y))$ est l'adhérence de $Y$ dans $X$.

(iii) *Les applications $\mathfrak{J}$ et $V$ définissent des bijections décroissantes réciproques l'une de l'autre, entre l'ensemble des parties fermées de X et l'ensemble des idéaux de A égaux à leurs racines.*

L'assertion (i) et la première assertion de (ii) résultent des définitions et du § 2, no 6, cor. 1 de la prop. 13. Si un ensemble fermé $V(M)$ (pour un $M \subset A$) contient $Y$, on a $M \subset p$ pour tout idéal premier $p \in Y$, d'où $M \subset \mathfrak{J}(Y)$ et par suite $V(M) \supset V(\mathfrak{J}(Y))$; comme on a $Y \subset V(\mathfrak{J}(Y))$, $V(\mathfrak{J}(Y))$ est le plus petit ensemble fermé de $X$ contenant $Y$, ce qui achève de prouver (ii). Enfin, il résulte de (ii) que, si $a$ est un idéal égal à sa racine, on a $\mathfrak{J}(V(a)) = a$ et que, si $Y$ est fermé dans $X$, $V(\mathfrak{J}(Y)) = Y$; ce qui démontre (iii).

On déduit aussitôt de la prop. 11 que, si M est une partie quelconque de A et Y une partie quelconque de X, on a V(M) = V(\mathfrak{J}(V(M))) et \mathfrak{J}(Y) = \mathfrak{J}(V(\mathfrak{J}(Y))).

#### Corollaire 1 {#ac-ii-s4-prop-11-cor-1 .statement}

Pour toute famille $(Y_\lambda)_{\lambda \in L}$ de parties fermées de X, $\mathfrak{J}(\bigcap_{\lambda \in L} Y_\lambda)$ est la racine de la somme des idéaux $\mathfrak{J}(Y_\lambda)$.

En effet, il résulte de la prop. 11, (iii), que $\mathfrak{J}(\bigcap_{\lambda \in L} Y_\lambda)$ est le plus petit idéal égal à sa racine et contenant tous les $\mathfrak{J}(Y_\lambda)$; cet idéal contient donc $\sum_{\lambda \in L} \mathfrak{J}(Y_\lambda)$ et par suite aussi la racine de $\sum_{\lambda \in L} \mathfrak{J}(Y_\lambda)$ (\S 2, n° 6, cor. 2 de la prop. 13), d’où le corollaire.

#### Corollaire 2 {#ac-ii-s4-prop-11-cor-2 .statement}

Désignons par $r(a)$ la racine d’un idéal a de A ; si a et b sont deux idéaux de A, la relation $V(a) \subset V(b)$ est équivalente à $b \subset r(a)$ et à $r(b) \subset r(a)$.

Il est immédiat que les relations $b \subset r(a)$ et $r(b) \subset r(a)$ sont équivalentes, et comme $V(a) = V(r(a))$, le corollaire résulte aussitôt de la prop. 11 ,(iii).

#### Corollaire 3 {#ac-ii-s4-prop-11-cor-3 .statement}

Soit $(f_\lambda)_{\lambda \in L}$ une famille d’éléments de A. Pour qu’un élément $g \in A$ soit tel que $X_g \subset \bigcup_{\lambda \in L} X_{f_\lambda}$, il faut et il suffit qu’il existe un entier $n > 0$ tel que $g^n$ appartienne à l’idéal engendré par les $f_\lambda$.

En effet, la relation $X_g \subset \bigcup_{\lambda \in L} X_{f_\lambda}$ équivaut à $V(g) \supset \bigcap_{\lambda \in L} V(f_\lambda)$, et il suffit d’appliquer le cor. 2.

#### Corollaire 4 {#ac-ii-s4-prop-11-cor-4 .statement}

Pour que deux éléments $f,\ g$ de A soient tels que $X_f = X_g$, il faut et il suffit qu’il existe deux entiers $m > 0,\ n > 0$ tels que $f^m \in Ag$ et $g^n \in Af$.

#### Corollaire 5 {#ac-ii-s4-prop-11-cor-5 .statement}

Pour que $f \in A$ soit tel que $X_f = \emptyset$, il faut et il suffit que f soit nilpotent.

Cela résulte aussitôt du cor. 4.

#### Corollaire 6 {#ac-ii-s4-prop-11-cor-6 .statement}

L’adhérence d’un ensemble réduit à un point $p \in X = \mathrm{Spec}(A)$ est l’ensemble $V(p)$ des idéaux premiers contenant $p$. Pour que l’ensemble $\{ p \}$ soit fermé dans $X$ (ou, comme on dit encore par abus de langage, pour que $p$ soit un point fermé de $X$), il faut et il suffit que $p$ soit maximal.

#### Corollaire 7 {#ac-ii-s4-prop-11-cor-7 .statement}

Si $A$ est un anneau noethérien, $X = \mathrm{Spec}(A)$ est un espace noethérien.

#### Proposition 12 {#ac-ii-s4-prop-12 .statement}

Pour tout $f \in A$, l’ensemble ouvert $X_f$ dans $X = \mathrm{Spec}(A)$ est quasi-compact ; en particulier, l’espace $X$ est quasi-compact.

Comme les $X_g$ forment une base de la topologie, il suffit de prouver que, si $(g_\lambda)_{\lambda \in L}$ est une famille d’éléments de $A$ telle que $X_f \subset \bigcup_{\lambda \in L} X_{g_\lambda}$, alors il existe une sous-famille finie $(g_\lambda)_{\lambda \in H}$ telle que $X_f \subset \bigcup_{\lambda \in H} X_{g_\lambda}$. Mais la relation $X_f \subset \bigcup_{\lambda \in L} X_{g_\lambda}$ signifie qu’il existe un entier $n > 0$ et une sous-famille finie $(g_\lambda)_{\lambda \in H}$ telle que $f^n$ appartienne à l’idéal engendré par cette sous-famille (cor. 3 de la prop. 11) ; d’où la proposition.

#### Proposition 13 {#ac-ii-s4-prop-13 .statement}

Soient $A, A'$ deux anneaux, $X = \mathrm{Spec}(A), X' = \mathrm{Spec}(A')$, $h$ un homomorphisme de $A$ dans $A'$ ; l’application $^a h : p' \to \overline{h}(p')$ de $X'$ dans $X$ est continue.

En effet, pour $M \subset A$, l’ensemble $(^a h)^{-1}(V(M))$ est l’ensemble des idéaux premiers $p'$ de $A'$ tels que $M \subset \overline{h}(p')$, ce qui équivaut à $h(M) \subset p'$ ; cet ensemble est donc égal à $V(h(M))$ et est par conséquent fermé.

On dit que $^a h$ est l’application associée à l’homomorphisme $h$.

#### Remarque {#ac-ii-s4-n3-rem-1 .statement}

Si $h$ est surjective et si $a$ est son noyau, il résulte de la définition de la topologie spectrale que $^a h$ est un homéomorphisme de $X'$ sur le sous-espace fermé $V(a)$ de $X$ ; en effet, pour qu’un idéal premier $p'$ de $A'$ contienne un idéal $b'$ de $A'$, il faut et il suffit que $\overline{h}(p')$ contienne $\overline{h}(b')$ ; on voit d’abord que $^a h$ est injective en prenant b’ premier ; en outre, pour tout idéal b’ de A’, l’image par $^a h$ de V(b’) est V($\overline{h}(b')$), d’où notre assertion, les idéaux de la forme $\overline{h}(b')$ étant tous les idéaux de A contenant $\alpha$.

#### Corollaire {#ac-ii-s4-n3-cor-1 .statement}

Soient S une partie multiplicative de A, $A' = S^{-1}A$, $h$ l’homomorphisme canonique $i_A^S$; alors $^a h$ est un homéomorphisme de $X' = \mathrm{Spec}(A')$ sur le sous-espace de $X = \mathrm{Spec}(A)$ formé des idéaux premiers de A ne rencontrant pas S.

En effet, soit $f' = f/s$ où $f \in A, s \in S$; on a $X_{f'} = X_{f/1}$ puisque $s/1$ est inversible dans $A'$. On sait déjà que $^a h$ est injective et que, pour tout $p' \in X'$, les relations $f/1 \in p'$ et $f \in \overline{h}(p') = ^a h(p')$ sont équivalentes, donc les conditions $p' \in X_{f/1}$ et $^a h(p') \in X_f$ sont équivalentes ; cela montre que $^a h(X_{f'})$ est égal à $X_f \cap ^a h(X')$, d’où la première assertion, puisque les $X_f$ (resp. $X_{f'}$) forment une base de la topologie de X (resp. X’). La seconde assertion résulte du § 2, n° 5, prop. 11, (ii).

#### Proposition 14 {#ac-ii-s4-prop-14 .statement}

Soit A un anneau. Pour qu’une partie Y de $X = \mathrm{Spec}(A)$ soit irréductible, il faut et il suffit que l’idéal $\mathfrak{J}(Y)$ soit premier.

Posons $p = \mathfrak{J}(Y)$, et notons que, pour un élément $f \in A$, la relation $f \in p$ est équivalente à $Y \subsetneq V(f)$. Supposons Y irréductible, et soient $f, g$ des éléments de A tels que $fg \in p$. On a donc

$$
Y \subset V(fg) = V(f) \cup V(g);
$$

comme Y est irréductible, $V(f)$ et $V(g)$ fermés, on a $Y \subset V(f)$ ou $Y \subset V(g)$, donc $f \in p$ ou $g \in p$, ce qui prouve que $p$ est premier.

Supposons maintenant $p$ premier ; on a $\overline{Y} = V(p)$ (prop. 11, (ii)), et comme $p$ est premier, $p = \mathfrak{J}(\{p\})$, d’où $\overline{Y} = V(\mathfrak{J}(\{p\})) = \{p\}$ (prop. 11, (ii)). Comme un ensemble réduit à un point est irréductible, Y est irréductible (n° 1, prop. 2).

#### Corollaire 1 {#ac-ii-s4-prop-14-cor-1 .statement}

Pour qu’un anneau A soit tel que $X = \mathrm{Spec}(A)$ soit irréductible, il faut et il suffit que le quotient de A par son nilradical $\mathfrak{N}$ soit intègre.

En effet (prop. 11, (i)), $\mathfrak{J}(X)$ est la racine de l’idéal (0), c’est-à-dire $\mathfrak{N}$.

#### Corollaire 2 {#ac-ii-s4-prop-14-cor-2 .statement}

L’application $p \to V(p)$ est une bijection de $X = \operatorname{Spec}(A)$ sur l’ensemble des parties fermées irréductibles de $X$; en particulier les composantes irréductibles d’une partie fermée $Y$ de $X$ sont les ensembles $V(p)$, où $p$ parcourt l’ensemble des éléments minimaux de l’ensemble des idéaux premiers de $A$ qui contiennent $\mathfrak{J}(Y)$.

Comme $\mathfrak{J}(V(p)) = p$ pour tout idéal premier $p$ de $A$, et $Y = V(\mathfrak{J}(Y))$ pour toute partie fermée $Y$ de $X$, la première assertion résulte de la prop. 14 ; d’autre part, pour que $Y \supset V(p)$, il faut et il suffit que $p = \mathfrak{J}(V(p)) \supset \mathfrak{J}(Y)$ (prop. 11), d’où la seconde assertion.

#### Corollaire 3 {#ac-ii-s4-prop-14-cor-3 .statement}

L’ensemble des idéaux premiers minimaux d’un anneau noethérien $A$ est fini.

En effet, $X = \operatorname{Spec}(A)$ n’a alors qu’un nombre fini de composantes irréductibles (cor. 7 de la prop. 11 et no 2, prop. 10) et le corollaire résulte du cor. 2 précédent.

#### Proposition 15 {#ac-ii-s4-prop-15 .statement}

Soient $A$ un anneau, $I$ un ensemble fini, $E$ l’ensemble des familles orthogonales $(e_i)_{i \in I}$ d’idempotents $e_i \neq 0$ de $A$, telles que $\sum_{i \in I} e_i = 1$. Pour tout $(e_i)_{i \in I} \in E$, posons $\varpi((e_i)_{i \in I}) = (V(A(1 - e_i)))_{i \in I}$, $\sigma((e_i)_{i \in I}) = (Ae_i)_{i \in I}$. Alors $\varpi$ est une bijection de $E$ sur l’ensemble $P$ des partitions $(U_i)_{i \in I}$ de $X = \operatorname{Spec}(A)$ en ensembles ouverts, et $\sigma$ est une bijection de $E$ sur l’ensemble $S$ des familles $(a_i)_{i \in I}$ d’idéaux $\neq 0$ de $A$ telles que $A$ soit somme directe des $a_i$.

Soit $(e_i)_{i \in I}$ un élément de $E$ et posons $Y_i = V(A(1 - e_i))$; si $i \neq j$, on a $1 = 1 - e_i + e_i(1 - e_j) \in A(1 - e_i) + A(1 - e_j)$, d’où $Y_i \cap Y_j = \emptyset$ (formules (1) et (2)). D’autre part,

$$
\bigcup_{i \in I} Y_i = V(\prod_{i \in I} A(1 - e_i)) \quad \text{(formule (3))};
$$

par hypothèse $\prod_{i \in I} (1 - e_i) = 1 - \sum_{i \in I} e_i = 0$, d’où $\bigcup_{i \in I} Y_i = X$ (formule (1)). Comme les $Y_i$ sont fermés, ils sont aussi ouverts, d’où $\varpi(E) \subset P$. Par ailleurs, on a évidemment $A = \sum_{i \in I} Ae_i$; si $0 = \sum_{i \in I} a_i e_i$ avec $a_i \in A$, on en tire, par multiplication par $e_i$, $0 = a_i e_i^2 = a_i e_i$ pour tout $i$; ceci prouve que $\sigma(E) \subset S$.

#### Lemme 2 {#ac-ii-s4-lem-2 .statement}

Si $e, f$ sont deux idempotents de $A$ tels que $Ae$ et $Af$ aient même racine, on a $e = f$.

En effet, il existe par hypothèse des entiers $m \geq 0,\ n \geq 0$ tels que $e = e^m \in Af$ et $f = f^n \in Ae$; soient $x, y$ des éléments de $A$ tels que $e = xf,\ f = ye$; on a $ef = x f^2 = x f = e$ et de même $ef = y e^2 = y e = f$, d’où $e = f$.

Le lemme 2 et le cor. 2 de la prop. 11 montrent que les applications $\varpi$ et $\sigma$ sont injectives.

Montrons que $\sigma$ est surjective. Si $(a_i)_{i \in I}$ est un élément de $S$, il y a des éléments $e_i \in a_i$ tels que $1 = \sum_{i \in I} e_i$; si $i \neq j$, on a $e_i e_j \in a_i \cap a_j = \{0\}$, d’où $e_i = \sum_{j \in I} e_i e_j = e_i^2$; enfin, on a $Ae_i \subset a_i$ pour tout $i \in I$ et $\sum_{i \in I} Ae_i = A$, d’où $Ae_i = a_i$.

Reste enfin à montrer que $\varpi$ est surjective. Soit $(U_i)_{i \in I}$ un élément de $P$ et posons $Z_i = \bigcup_{j \neq i} U_j$; comme $U_i$ et $Z_i$ sont fermés, il existe des idéaux $a_i,\ b_i$ de $A$ tels que $U_i = V(a_i)$, $Z_i = V(b_i)$. On va montrer qu’on peut de plus supposer que $a_i \cap b_i = 0$. On a $U_i \cap Z_i = \emptyset$, d’où $a_i + b_i = A$; soient $a_i \in a_i$, $b_i \in b_i$ tels que $a_i + b_i = 1$. On a $X = U_i \cup Z_i = V(a_i b_i)$ (formule (3)); tout élément de $a_i b_i$ est donc nilpotent (cor. 2 de la prop. 11); soit $p$ un entier tel que $a_i^p b_i^p = 0$. On a $U_i \subset V(A a_i) = V(A a_i^p),\ Z_i \subset V(A b_i) = V(A b_i^p)$ et $V(A a_i) \cap V(A b_i) = V(A a_i + A b_i) = \emptyset$, donc $U_i = V(A a_i^p)$ et $Z_i = V(A b_i^p)$, ce qui établit notre assertion en remplaçant $a_i$ par $A a_i^p$ et $b_i$ par $A b_i^p$. Les idéaux $a_i$ et $b_i$ étant ainsi choisis, il résulte de ce que $\sigma$ est bijective qu’il existe deux idempotents $f_i \in a_i,\ e_i \in b_i$ tels que $1 = e_i + f_i,\ e_i f_i = 0,\ a_i = A f_i,\ b_i = A e_i$. Si $i \neq j$, on a $X = Z_i \cup Z_j = V(A e_i e_j)$, et comme $e_i e_j$ est un idempotent, le lemme 2 montre que $e_i e_j = 0$. Enfin $e = \sum_{i \in I} e_i$ est idempotent et on a $e_i \in Ae$ pour tout $i \in I$, d’où $V(Ae) \subset Z_i$ pour tout $i$; il en résulte que $V(Ae) = \emptyset = V(A.1)$ et le lemme 2 montre encore que $e = 1$.

C. Q. F. D.

#### Corollaire 1 {#ac-ii-s4-lem-2-cor-1 .statement}

Soient $A$ un anneau, $\mathfrak{r}$ un nilidéal de $A$, $h : A \to A/\mathfrak{r}$ l’homomorphisme canonique. Pour toute famille orthogonale finie $(e'_i)_{i \in I}$ d’idempotents de $A/\mathfrak{r}$, telle que $\sum_{i \in I} e'_i = 1$, il existe une famille orthogonale finie $(e_i)_{i \in I}$ d’idempotents de $A$ telle que $\sum_{i \in I} e_i = 1$ et $h(e_i) = e'_i$ pour tout $i \in I$.

Posons $A' = A/\mathfrak{r}$. On sait (Remarque suivant la prop. 13) que
$$
a h : \operatorname{Spec}(A') \to \operatorname{Spec}(A)
$$
est un homéomorphisme bijectif, tout idéal premier de $A$ contenant $\mathfrak{r}$ par hypothèse. La prop. 15 montre qu’il existe dans $A$ une famille orthogonale finie $(e_i)_{i \in I}$ d’idempotents telle que $\sum_{i \in I} e_i = 1$ et que l’image par $a h$ de $V(A'(1 - e'_i))$ soit $V(A(1 - e_i))$. Mais il est clair que $V(A(1 - e_i))$ est aussi l’image par $a h$ de $V(A'(1 - h(e_i)))$; comme $1 - e'_i$ et $1 - h(e_i)$ sont des idempotents, le lemme 2 montre que $e'_i = h(e_i)$, d’où le corollaire.

#### Corollaire 2 {#ac-ii-s4-lem-2-cor-2 .statement}

Pour que le spectre premier $X = \operatorname{Spec}(A)$ d’un anneau $A$ soit connexe, il faut et il suffit qu’il n’existe dans $A$ aucun idempotent autre que $0$ et $1$.

Dire en effet que $X$ n’est pas connexe signifie qu’il existe dans $X$ un ensemble ouvert et fermé distinct de $\varnothing$ et de $X$.

### 4. Support d’un module

#### Définition 5 {#ac-ii-s4-def-5 .statement}

Soient $A$ un anneau, $M$ un $A$-module. On appelle support de $M$, et on note $\operatorname{Supp}(M)$, l’ensemble des idéaux premiers $\mathfrak{p}$ de $A$ tels que $M_{\mathfrak{p}} \neq 0$.

Comme tout idéal maximal de $A$ est premier, il résulte aussitôt du § 3, no 3, cor. 2 du th. 1, que, pour qu’un $A$-module $M$ soit réduit à $0$, il faut et il suffit que $\operatorname{Supp}(M) = \varnothing$.

#### Exemple {#ac-ii-s4-n4-exa-1 .statement}

Soit $a$ un idéal de $A$; avec les notations du no 3, on a
$$
V(a) = \operatorname{Supp}(A/a).
$$
En effet, si $\mathfrak{p}$ est un idéal premier de $A$ tel que $a \notin \mathfrak{p}$, on sait que $(A/a)_{\mathfrak{p}} = 0$ (\S 3, no 1, Remarque 3); si au contraire $a \subset \mathfrak{p}$, $aA_{\mathfrak{p}}$ est contenu dans l’idéal maximal $pA_p$ de $A_p$ et $(A/\alpha)_p$ est isomorphe à $A_p/\alpha A_p$, donc est $\neq 0$ ($\S 3$, n° 1, prop. 3); d’où notre assertion.
En particulier, on a $\mathrm{Supp}(A) = \mathrm{Spec}(A)$.

#### Proposition 16 {#ac-ii-s4-prop-16 .statement}

Soient $A$ un anneau, $M$ un $A$-module.
(i) Si $N$ est un sous-module de $M$, on a
$$
\mathrm{Supp}(M) = \mathrm{Supp}(N) \cup \mathrm{Supp}(M/N).
$$
(ii) Si $M$ est somme d’une famille $(N_i)_{i \in I}$ de sous-modules, on a
$$
\mathrm{Supp}(M) = \bigcup_{i \in I} \mathrm{Supp}(N_i).
$$
(i) De la suite exacte $0 \to N \to M \to M/N \to 0$, on déduit, pour tout idéal premier $p$ de $A$, la suite exacte
$$
0 \to N_p \to M_p \to (M/N)_p \to 0
$$
($\S 2$, n° 4, th. 1). Pour que $M_p$ soit réduit à $0$, il faut et il suffit donc qu’il en soit ainsi de $N_p$ et de $(M/N)_p$. Autrement dit, la relation $p \notin \mathrm{Supp}(M)$ équivaut à « $p \notin \mathrm{Supp}(N)$ et $p \notin \mathrm{Supp}(M/N)$ », ce qui prouve (i).
(ii) Pour tout idéal premier $p$ de $A$, $M_p$ est somme de la famille de sous-modules $(N_i)_p$ ($\S 2$, n° 4). Dire que $M_p \neq 0$ signifie qu’il existe $i \in I$ tel que $(N_i)_p \neq 0$, d’où (ii).

#### Corollaire {#ac-ii-s4-n4-cor-1 .statement}

Soient $A$ un anneau, $M$ un $A$-module, $(m_i)_{i \in I}$ un système de générateurs de $M$, et $a_i$ l’annulateur de $m_i$. On a alors
$$
\mathrm{Supp}(M) = \bigcup_{i \in I} V(a_i).
$$
En effet, $\mathrm{Supp}(M) = \bigcup_{i \in I} \mathrm{Supp}(Am_i)$ en vertu de la prop. 16, (ii). D’autre part, $Am_i$ est isomorphe au $A$-module $A/a_i$, et on a vu que $\mathrm{Supp}(A/a_i) = V(a_i)$ (*Exemple ci-dessus*).

#### Proposition 17 {#ac-ii-s4-prop-17 .statement}

Soient $\Lambda$ un anneau, $M$ un $A$-module, $a$ son annulateur ; si $M$ est de type fini, on a $\mathrm{Supp}(M) = V(a)$, et $\mathrm{Supp}(M)$ est donc fermé dans $\mathrm{Spec}(A)$.
Soit $(m_i)_{1 \leq i \leq n}$ un système de générateurs de $M$, et soit $a_i$ l’annulateur de $m_i$; on a $a = \bigcap_{i=1}^n a_i$, donc $V(a) = \bigcup_{i=1}^n V(a_i)$ (n° 3, formule (3)), et la proposition résulte du cor. de la prop. 16.

#### Corollaire 1 {#ac-ii-s4-prop-17-cor-1 .statement}

Soient $A$ un anneau, $M$ un $A$-module de type fini, $a$ un élément de $A$. Pour que $a$ appartienne à tout idéal premier du support de $M$, il faut et il suffit que l’homothétie de $M$, de rapport $a$, soit nilpotente.

En effet, il résulte de la prop. 17 que l’intersection des idéaux premiers appartenant à $\mathrm{Supp}(M)$ est la racine de l’annulateur $a$ de $M$ (n° 3, prop. 11, (ii)). Dire que $a$ appartient à cette racine équivaut à dire qu’il existe une puissance $a^k \in a$, donc que $a^k M = 0$.

#### Corollaire 2 {#ac-ii-s4-prop-17-cor-2 .statement}

Soient $A$ un anneau noethérien, $M$ un $A$-module de type fini, $a$ un idéal de $A$. Pour que $\mathrm{Supp}(M) \subset V(a)$, il faut et il suffit qu’il existe un entier $k$ tel que $a^k M = 0$.

En effet, si $b$ est l’annulateur de $M$, la relation $\mathrm{Supp}(M) \subset V(a)$ équivaut à $V(b) \subset V(a)$ d’après la prop. 17, donc à $a \subset r(b)$, où $r(b)$ est la racine de $b$ (n° 3, cor. 2 de la prop. 11). Puisque $A$ est noethérien, cette condition équivaut encore à l’existence d’un entier $k > 0$ tel que $a^k \subset b$ ($\S 2$, n° 6, prop. 15).

#### Proposition 18 {#ac-ii-s4-prop-18 .statement}

Soient $M, M'$ deux modules de type fini sur un anneau $A$; on a alors

$$
\mathrm{Supp}(M \otimes_A M') = \mathrm{Supp}(M) \cap \mathrm{Supp}(M').
$$

Il s’agit de prouver que, si $p$ est un idéal premier de $A$, les relations $(M \otimes_A M')_p \neq 0$ et « $M_p \neq 0$ et $M'_p \neq 0$ » sont équivalentes. Comme les $A_p$-modules $M_p \otimes_{A_p} M'_p$ et $(M \otimes_A M')_p$ sont isomorphes ($\S 2$, n° 7, prop. 18), notre assertion résulte du lemme suivant :

#### Lemme 3 {#ac-ii-s4-lem-3 .statement}

Soient $B$ un anneau local, $E$ et $E'$ deux $B$-modules de type fini. Si $E \neq 0$ et $E' \neq 0$, on a $E \otimes_B E' \neq 0$.

En effet, soit $k$ le corps résiduel de $B$. En vertu du $\S 3$, n° 2, prop. 4, on a $k \otimes_B E \neq 0$ et $k \otimes_B E' \neq 0$; on en déduit que $(k \otimes_B E) \otimes_k (k \otimes_B E') \neq 0$ (Alg., chap. II, 3e éd., $\S 3$, n° 7). Mais en vertu de l’associativité du produit tensoriel (loc. cit., $\S 3$, n° 8) ce produit tensoriel est isomorphe à $E \otimes_B ((k \otimes_k k) \otimes_B E') = E \otimes_B (k \otimes_B E')$ donc à $k \otimes_B (E \otimes_B E')$, d’où la conclusion.

#### Corollaire {#ac-ii-s4-n4-cor-2 .statement}

Soient M un A-module de type fini, n son annulateur. Pour tout idéal a de A, on a Supp (M/aM) = V(a) ∩ V(n) = V(a + n).

En effet, M/aM = M ⊗_A (A/a), et A/a est de type fini.

#### Proposition 19 {#ac-ii-s4-prop-19 .statement}

Soient A, B deux anneaux, φ : A → B un homomorphisme, aφ : Spec(B) → Spec(A) l’application continue associée à φ (prop. 13). Pour tout A-module M, on a Supp (M_B) ⊂ aφ^{-1}(Supp (M)) ; si en outre M est de type fini, on a Supp (M_B) = aφ^{-1}(Supp (M)).

Soit q un idéal premier de B et soit p = φ^{-1}(q). Supposons que q appartienne à Supp (M_B) ; on a M_B ⊗_B B_q = (M ⊗_A B) ⊗_B B_q = M ⊗_A B_q = (M ⊗_A A_p) ⊗_{A_p} B_q puisque l’homomorphisme A → B → B_q se factorise en A → A_p → B_q (§ 2, n° 1, prop. 2) ; l’hypothèse M_B ⊗_B B_q ≠ 0 entraîne donc M ⊗_A A_p ≠ 0, d’où la première assertion. Comme l’homomorphisme φ_q : A_p → B_q est local, la seconde assertion résulte du lemme suivant :

#### Lemme 4 {#ac-ii-s4-lem-4 .statement}

Soient A, B deux anneaux locaux, ρ : A → B un homomorphisme local, E un A-module de type fini. Si E ≠ 0, on a E_B ≠ 0.

En effet, soit m l’idéal maximal de A et soit k = A/m le corps résiduel ; l’hypothèse entraîne que B ⊗_A k = B/mB ≠ 0 ; en vertu de l’associativité du produit tensoriel, (E ⊗_A B) ⊗_A k est isomorphe à E ⊗_A (B ⊗_A k), donc aussi à E ⊗_A (k ⊗_k (B ⊗_A k)) et finalement à (E ⊗_A k) ⊗_k (B ⊗_A k) ; en vertu du § 3, n° 2, prop. 4, on a E ⊗_A k ≠ 0, donc (E ⊗_A B) ⊗_A k ≠ 0 (Alg., chap. II, 3e éd., § 3, n° 7) et a fortiori E ⊗_A B ≠ 0.

#### Proposition 20 {#ac-ii-s4-prop-20 .statement}

Soient A un anneau, M un A-module de type fini. Pour tout idéal premier p ∈ Supp (M), il existe un A-homomorphisme non nul ω : M → A/p.

Soit p ∈ Supp (M). Comme M est de type fini et M_p ≠ 0, on a M_p/pM_p = M_p ⊗_{A_p} (A_p/pA_p) ≠ 0 (§ 3, n° 2, prop. 4). Soit K = A_p/pA_p le corps des fractions de l’anneau intègre A/p ; puisque M_p/pM_p est un K-espace vectoriel non réduit à 0, il existe une forme linéaire non nulle u : M_p/pM_p → K. Si (x_i)_{1 ≤ i ≤ n} est un système de générateurs du A-module M, il existe un élément $\alpha \neq 0$ de $A/p$ tel que les images des $x_i$ par l’application A-linéaire composée
$$
\nu : M \to M_p \to M_p / pM_p \xrightarrow{\alpha u} K
$$
appartiennent à $A/p$. L’application $\nu$ induit alors une application A-linéaire non nulle $w$ de $M$ dans $A/p$.

## EXERCICES {#ac-ii-s4-exercises}

See the [exercises for § 4](exercises/s4/).
