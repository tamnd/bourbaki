---
book: evt
book_title: Topological Vector Spaces
chapter: III
chapter_title: ESPACES D’APPLICATIONS LINÉAIRES CONTINUES
section: 1
section_title: Bornologie dans un espace vectoriel topologique
lang: fr
source: evt-i-v-fr
pdf_pages: 0136-0146, 0173-0176
extraction: ocr
subsections:
    - "no": 1
      title: Bornologies
      page: 0
      pdf_page: 136
    - "no": 2
      title: Parties bornées d’un espace vectoriel topologique
      page: 2
      pdf_page: 137
    - "no": 3
      title: Image par une application continue
      page: 4
      pdf_page: 139
    - "no": 4
      title: Parties bornées dans certaines limites inductives
      page: 5
      pdf_page: 140
    - "no": 5
      title: Les espaces $E_A$ (A borné)
      page: 7
      pdf_page: 142
    - "no": 6
      title: Ensembles bornés complets et espaces quasi-complets
      page: 8
      pdf_page: 143
    - "no": 7
      title: Exemples
      page: 9
      pdf_page: 144
statements: 33
exercises: 18
content_sha256: 900d3937eb1e4c2f117534a53720212a89478b9c51cb019d016f7b23ede16893
---

## § 1. BORNOLOGIE DANS UN ESPACE VECTORIEL TOPOLOGIQUE

### 1. Bornologies

#### Définition 1 {#evt-iii-s1-def-1 .statement}

On appelle bornologie sur un ensemble E une partie $\mathcal{B}$ de l’ensemble des parties de E satisfaisant aux conditions suivantes (cf. TG, X, p. 3, Remarque 2) :
(B1) Toute partie d’un ensemble de $\mathcal{B}$ appartient à $\mathcal{B}$.
(B2) Toute réunion finie d’ensembles de $\mathcal{B}$ appartient à $\mathcal{B}$.

On dit que $\mathcal{B}$ est couvrante si toute partie à un élément de E appartient à $\mathcal{B}$, ou, ce qui revient au même, si $\mathcal{B}$ est un recouvrement de E.

#### Exemple {#evt-iii-s1-n1-exa-1 .statement}

Soit E un espace métrique ; l’ensemble des parties bornées de E (TG, IX, p. 14) est une bornologie couvrante sur E. Soit G le groupe des isométries de E ; l’ensemble des parties M de G telles que, quel que soit $x \in E$, l’ensemble $M.x$ est une partie bornée de E, est une bornologie couvrante sur G.

Si $\mathcal{B}$ est une bornologie sur un ensemble E, on appelle base de $\mathcal{B}$ une partie $\mathcal{B}_1$ de $\mathcal{B}$ telle que tout ensemble de $\mathcal{B}$ soit contenu dans un ensemble de $\mathcal{B}_1$.

L’intersection d’une famille de bornologies sur E est une bornologie ; par suite pour toute partie $\mathcal{S}$ de $\mathfrak{P}(E)$, il existe une plus petite bornologie contenant $\mathcal{S}$ ; on dit qu’elle est engendrée par $\mathcal{S}$ ; elle admet pour base l’ensemble des réunions finies d’ensembles de $\mathcal{S}$. Si E et E’ sont deux ensembles, et $\mathcal{B}$ (resp. $\mathcal{B}'$) une bornologie sur E (resp. E’), on appelle bornologie produit la bornologie sur $E \times E'$ qui admet pour base l’ensemble des $M \times M'$ pour $M \in \mathcal{B}$ et $M' \in \mathcal{B}'$.

#### Définition 2 {#evt-iii-s1-def-2 .statement}

Soit E un espace vectoriel. On dit qu’une bornologie $\mathcal{B}$ sur E est convexe si, quels que soient $X \in \mathcal{B}$ et $t \in \mathbf{K}$, l’homothétique $tX$ et l’enveloppe convexe équilibrée $\Gamma(X)$ (II, p. 10) de X appartiennent à $\mathcal{B}$.

Si X et Y sont des parties de E, on a

$$
X + Y \subset 2\Gamma(X \cup Y)
$$
$$
\lambda X \subset t\Gamma(X) \quad \text{pour} \quad |\lambda| \leq t .
$$

Par suite, si $\mathcal{B}$ est une bornologie convexe sur E, si A est une partie bornée de K et si X, Y appartiennent à $\mathcal{B}$, alors on a $X + Y \in \mathcal{B}$ et $A.X \in \mathcal{B}$.

### 2. Parties bornées d’un espace vectoriel topologique

#### Définition 3 {#evt-iii-s1-def-3 .statement}

Soit E un espace vectoriel topologique. On dit qu’une partie A de E est bornée si elle est absorbée par tout voisinage de 0 dans E (I, p. 7, déf. 4).

Pour que A soit bornée, il suffit que A soit absorbée par tout voisinage d’un système fondamental de voisinages de 0. Comme il existe un système fondamental de voisinages équilibrés de 0 (I, p. 7, prop. 4), il revient au même de dire que, pour tout voisinage V de 0 dans E, il existe $\lambda \in \mathbf{K}$ tel que $A \subset \lambda V$.

Supposons que la topologie de E soit définie par un système fondamental $\Gamma$ de semi-normes (II, p. 3); pour qu’une partie A de E soit bornée, il faut et il suffit que toute semi-norme $p \in \Gamma$ soit bornée sur A.

En particulier si E est un espace semi-normé, pour qu’une partie A de E soit bornée, il faut et il suffit qu’elle soit contenue dans une boule. En d’autres termes, si E est normé, cela signifie que A est bornée pour la structure d’espace métrique de E (TG, IX, p. 14).

#### Remarque 1 {#evt-iii-s1-n2-rem-1 .statement}

Si E est un espace semi-normé, les boules forment un système fondamental de voisinages bornés de 0 dans E. Inversement, si E est un espace vectoriel topologique localement convexe et s’il existe un voisinage borné de 0 dans E, celui-ci contient un voisinage convexe équilibré W, et la jauge de W est alors une semi-norme qui définit la topologie de E.

Ainsi, si E est localement convexe et métrisable et si sa topologie ne peut pas être définie par une seule norme, il n’existe pas de distance sur E définissant sa topologie et pour laquelle les parties bornées (TG, IX, p. 14) soient les parties bornées de E. Plus précisément, pour toute distance d sur E, invariante par translation et définissant la topologie de E, les parties bornées de E sont bornées pour d (III, p. 39, exerc. 3) mais la réciproque est inexacte.

#### Remarque 2 {#evt-iii-s1-n2-rem-2 .statement}

Soit M un sous-espace vectoriel de E, muni de la topologie induite. Pour qu’une partie de M soit bornée dans M, il faut et il suffit qu’elle soit bornée dans E.

#### Remarque 3 {#evt-iii-s1-n2-rem-3 .statement}

Soit N l’intersection des voisinages de 0 dans E, de sorte que $\tilde{E} = E/N$ est l’espace vectoriel séparé associé à E. Alors N est bornée; si $\pi : E \to \tilde{E}$ est l’homomorphisme canonique, pour qu’une partie B de E soit bornée, il faut et il suffit que $\pi(B)$ le soit.

#### Remarque 4 {#evt-iii-s1-n2-rem-4 .statement}

Si E est un espace localement convexe séparé, pour tout $x \neq 0$ dans E, il existe une semi-norme continue $p$ telle que $p(x) \neq 0$; cette semi-norme n’est pas bornée sur la demi-droite réelle $\mathbf{R}_+ . x$ engendrée par x. Donc aucun sous-espace non nul de E n’est borné. En particulier, un sous-ensemble borné ne contient aucune droite.

#### Définition 4 {#evt-iii-s1-def-4 .statement}

Soit E un espace localement convexe. On dit qu’une bornologie $\mathcal{B}$ sur E est adaptée à E si elle est convexe, composée de parties bornées de E, et si l’adhérence de tout ensemble de $\mathcal{B}$ appartient à $\mathcal{B}$.

#### Proposition 1 {#evt-iii-s1-prop-1 .statement}

Soit E un espace localement convexe. L’ensemble des parties bornées de E est une bornologie adaptée.

Il s’agit d’établir les propriétés suivantes :
a) Si B est une partie bornée de E, toute partie de B est bornée.
b) La réunion de deux parties bornées est bornée.
c) Tout homothétique d’une partie bornée est bornée.
d) L’enveloppe fermée convexe équilibrée (II, p. 14) d’une partie bornée est bornée.

Si $p$ est une semi-norme continue sur E, les boules de $p$ sont convexes équilibrées fermées, et l’homothétique d’une boule est une boule. Donc, si $p$ est bornée sur deux parties X et Y de E, elle l’est aussi sur l’enveloppe fermée convexe équilibrée de $X \cup Y$, et sur les homothétiques de celle-ci. Ceci établit les propriétés b), c) et d), et a) est évidente.

#### Définition 5 {#evt-iii-s1-def-5 .statement}

Soit E un espace localement convexe. On appelle bornologie canonique de E l’ensemble des parties bornées de E.

Si $\mathcal{B}$ est un ensemble de parties bornées de E, il existe une plus petite bornologie $\tilde{\mathcal{B}}$ adaptée à E et contenant $\mathcal{B}$. Les ensembles de $\tilde{\mathcal{B}}$ sont ceux contenus dans un homothétique de l’enveloppe fermée convexe équilibrée d’une réunion finie d’ensembles de $\mathcal{B}$.

Toute bornologie adaptée est contenue dans la bornologie canonique.

#### Proposition 2 {#evt-iii-s1-prop-2 .statement}

Dans un espace localement convexe E, tout ensemble précompact est borné.

En effet, soient A une partie précompacte de E et V un voisinage convexe et équilibré de 0. Il existe une suite finie $(a_i)_{1 \leq i \leq n}$ de points de A telle que

$$
A \subset \bigcup_{1 \leq i \leq n} (a_i + V).
$$

Comme $B = \{a_1, ..., a_n\}$ est borné, il existe un scalaire $\lambda$ tel que $0 < \lambda < 1$ et $\lambda B \subset V$; on a $\lambda A \subset \lambda B + \lambda V \subset V + V$, d’où la proposition.

#### Corollaire {#evt-iii-s1-n2-cor-1 .statement}

Dans un espace localement convexe, l’ensemble des points d’une suite de Cauchy est borné.

En effet cet ensemble est précompact (TG, II, p. 29).

#### Remarque 5 {#evt-iii-s1-n2-rem-5 .statement}

En général, les parties bornées d’un espace localement convexe E ne sont pas toutes précompactes (par exemple, si E est un espace normé de dimension infinie, sa boule unité n’est pas précompacte (I, p. 15, th. 3)). Toutefois, il en est ainsi si E est un espace faible (II, p. 45) : en effet, l’espace vectoriel topologique séparé associé à E est alors isomorphe à un sous-espace d’un produit $K^l$ dont les parties bornées sont précompactes (cf. III, p. 4, cor. 2).
Pour d’autres exemples, voir IV, p. 18.

#### Proposition 3 {#evt-iii-s1-prop-3 .statement}

Soit A une partie d’un espace localement convexe E. Si A est bornée, pour toute suite $(x_n)$ de points de A et toute suite $(\lambda_n)$ de scalaires tendant vers 0, la suite $(\lambda_n x_n)$ tend vers 0. Inversement, s’il existe une suite $(\lambda_n)$ de scalaires non nuls telle que pour toute suite $(x_n)$ de points de A la suite $(\lambda_n x_n)$ soit bornée, alors A est bornée.

Supposons A bornée. Si $(\lambda_n)$ est une suite de scalaires qui tend vers 0, et V un voisinage de 0, on a $\lambda_n A \subset V$ dès que $n$ est assez grand, d’où la première assertion.

Inversement si A n’est pas bornée et si $(\lambda_n)$ est une suite de scalaires $\neq 0$, il existe une semi-norme continue $p$ et une suite $(x_n)$ de points de A tels que $p(x_n) \geq \frac{n}{|\lambda_n|}$. On a alors $p(\lambda_n x_n) \geq n$, et la suite $(\lambda_n x_n)$ n’est pas bornée.

#### Corollaire {#evt-iii-s1-n2-cor-2 .statement}

Pour qu’une partie A de E soit bornée, il faut et il suffit que toute partie dénombrable de A le soit.

### 3. Image par une application continue

#### Proposition 4 {#evt-iii-s1-prop-4 .statement}

Soient E et F deux espaces localement convexes, et $f : E \to F$ une application continue. On suppose que $f(0) = 0$ et qu’il existe un nombre réel $m \geq 0$ tel que $f(\lambda x) = \lambda^m f(x)$ pour tout $\lambda > 0$. Alors si A est une partie bornée de E, $f(A)$ est bornée dans F.

En effet, si V est un voisinage de 0 dans F, $f^{-1}(V)$ est un voisinage de 0 dans E. Si A est bornée dans E, il existe $\lambda > 0$ tel que $A \subset \lambda f^{-1}(V)$ et ceci implique $f(A) \subset \lambda^m V$.

#### Corollaire 1 {#evt-iii-s1-prop-4-cor-1 .statement}

Soient E et F deux espaces localement convexes, et $u : E \to F$ une application linéaire continue. Si A est une partie bornée de E, $u(A)$ est bornée dans F.

#### Corollaire 2 {#evt-iii-s1-prop-4-cor-2 .statement}

Soit $E = \prod_{i \in I} E_i$ le produit d’une famille d’espaces localement convexes. Pour qu’une partie de E soit bornée, il faut et il suffit que toutes ses projections le soient.

Plus généralement :

#### Corollaire 3 {#evt-iii-s1-prop-4-cor-3 .statement}

Soient E un espace vectoriel, $(F_i)_{i \in I}$ une famille d’espaces localement convexes et $f_i$ une application linéaire de E dans $F_i$ (pour $i \in I$). Munissons E de la topologie (localement convexe) la moins fine qui rende continues les $f_i$ (II, p. 29). Pour qu’une partie A de E soit bornée, il faut et il suffit que $f_i(A)$ soit bornée dans $F_i$ pour tout $i \in I$.

En effet, si A est bornée, les $f_i(A)$ le sont (cor. 1). Inversement, si les $f_i(A)$ sont bornées et si $p$ est une semi-norme continue sur E, il existe une partie finie J de I et une famille $(q_j)_{j \in J}$, où $q_j$ est une semi-norme continue sur $F_j$, telles que l’on ait $p \leq \sup_{j \in J} (q_j \circ f_j)$. Par suite, $p$ est bornée sur A.

#### Corollaire 4 {#evt-iii-s1-prop-4-cor-4 .statement}

Soient $E_i$ ($1 \leq i \leq n$) et $F$ des espaces localement convexes, et $f$ une application multilinéaire continue de $\prod_{i=1}^n E_i$ dans $F$. Si $B_i$ est une partie bornée de $E_i$ pour $1 \leq i \leq n$, alors $f(\prod_{i=1}^n B_i)$ est bornée dans $F$.

#### Corollaire 5 {#evt-iii-s1-prop-4-cor-5 .statement}

Soient $E$ et $F$ deux espaces localement convexes, et $u : E \to F$ une application polynomiale continue. Si $A$ est une partie bornée de $E$, $u(A)$ est bornée.

### 4. Parties bornées dans certaines limites inductives

#### Proposition 5 {#evt-iii-s1-prop-5 .statement}

Soit $(E_i)_{i \in I}$ une famille d’espaces localement convexes séparés, et soit $E$ la somme directe topologique de cette famille (II, p. 32). Pour qu’une partie $B$ de $E$ soit bornée, il faut et il suffit qu’il existe une partie finie $J$ de $I$ telle que $\mathrm{pr}_i(B)$ soit bornée dans $E_i$ pour $i \in J$ et $\mathrm{pr}_i(B) \subset \{0\}$ pour $i \notin J$.

Soit $J$ une partie finie de $I$. Comme la topologie de $E$ induit sur $\prod_{j \in J} E_j$ la topologie produit (II, p. 33, prop. 7 et 8), il résulte de III, p. 4, cor. 2 que la condition est suffisante.

Inversement, soit $B$ une partie bornée de $E$. Alors $\mathrm{pr}_i(B)$ est bornée pour tout $i$ (III, p. 4, cor. 1). Il suffit donc de prouver qu’il existe une partie finie $J$ de $I$ telle que $\mathrm{pr}_i(B) \subset \{0\}$ pour $i \notin J$. Supposons le contraire : il existe alors une suite infinie $(i_n)$ d’éléments distincts de $I$ et une suite infinie $(x_n)$ d’éléments de $B$ telles que $\mathrm{pr}_{i_n}(x_n) \neq 0$. Comme $E_{i_n}$ est séparé, il existe une semi-norme continue $p_n$ sur $E_{i_n}$ telle que $p_n(\mathrm{pr}_{i_n}(x_n)) \geq n$. Alors $p = \sum_{n \geq 1} p_n \circ \mathrm{pr}_{i_n}$ est une semi-norme continue sur $E$ et $p$ n’est pas bornée sur $B$, ce qui est absurde.

#### Proposition 6 {#evt-iii-s1-prop-6 .statement}

Soit $E$ un espace localement convexe limite inductive stricte d’une suite croissante $(E_n)$ de sous-espaces vectoriels fermés de $E$ (II, p. 36). Pour qu’une partie $B$ de $E$ soit bornée, il faut et il suffit qu’elle soit contenue dans un des sous-espaces $E_n$, et bornée dans ce sous-espace.

La condition est suffisante, puisque la topologie induite sur $E_n$ par celle de $E$ est identique à la topologie donnée sur $E_n$ (II, p. 35, prop. 9). Pour voir que la condition est nécessaire, il suffit (III, p. 3, prop. 3) de prouver que si une suite $(x_m)$ de points de $E$ n’est contenue dans aucun des sous-espaces $E_n$, elle ne peut pas tendre vers 0. Quitte à extraire une suite partielle de la suite $(x_m)$, on peut supposer qu’il existe une suite strictement croissante $(n_k)$ d’entiers tels que, pour tout indice $k$, on ait $x_k \notin E_{n_k}$ et $x_k \in E_{n_{k+1}}$. Il existe alors (II, p. 35, lemme 2) une suite croissante $(V_k)$ d’ensembles convexes telle que $V_k$ soit un voisinage de 0 dans $E_{n_k}$, que $V_{k+1} \cap E_{n_k} = V_k$, et que $x_k \notin V_{k+1}$ pour tout indice $k$. La réunion $V$ des $V_k$ est alors un voisinage de 0 dans $E$, et l’on a $x_k \notin V$ pour tout $k$, ce qui prouve que la suite $(x_k)$ ne tend pas vers 0.

La conclusion de la prop. 6 n’est plus nécessairement vraie pour un espace E limite inductive d’un ensemble filtrant non dénombrable de sous-espaces fermés de E (cf. III, p. 39, exerc. 7).

#### Proposition 7 {#evt-iii-s1-prop-7 .statement}

Soit $(E_n)_{n \geq 0}$ une suite d’espaces localement convexes séparés, et pour chaque $n$, soit $u_n : E_n \to E_{n+1}$ une application linéaire injective compacte (i.e. telle qu’il existe un voisinage de 0 dans $E_n$ dont l’image par $u_n$ soit relativement compacte, ce qui entraîne que $u_n$ est continue). Soit E l’espace limite inductive du système $(E_n, u_n)$ (II, p. 31), et soit $v_n$ l’application canonique de $E_n$ dans E. L’espace localement convexe E est séparé. En outre, pour toute partie A de E, les conditions suivantes sont équivalentes :

(i) A est bornée ;
(ii) il existe un entier $n$ tel que A soit l’image par $v_n$ d’une partie bornée de $E_n$ ;
(iii) A est relativement compacte.

Identifions $E_n$ à un sous-espace vectoriel de E (muni d’une topologie plus fine que la topologie induite).

#### Lemme 1 {#evt-iii-s1-lem-1 .statement}

Sous les hypothèses de la prop. 7, la topologie de E est la plus fine rendant continues les applications $v_n : E_n \to E$.

Il s’agit de prouver que, si U est une partie de E telle que $U \cap E_n$ soit ouvert dans $E_n$ pour tout $n$, alors U est ouvert dans E ; autrement dit, il faut montrer que, pour tout $x \in U$, il existe un ensemble *convexe équilibré* V tel que $x + V \subset U$ et que $V \cap E_n$ soit un voisinage de 0 dans $E_n$ pour tout $n$ assez grand (II, p. 29, prop. 5). Pour tout $n$, soit $W_n$ un voisinage convexe équilibré de 0 dans $E_n$ tel que l’adhérence $H_n$ de $W_n$ dans $E_{n+1}$ soit compacte. Soit $x \in U$ et soit $n_0$ un entier tel que $x \in E_{n_0}$. Nous allons construire par récurrence une suite $(\varepsilon_n)_{n \geq n_0}$ de scalaires $> 0$ telle que $x + \sum_{n_0 \leq i \leq n} \varepsilon_i H_i$ soit contenu dans U pour $n \geq n_0$. Supposons donc construits les $\varepsilon_i$ pour $i < n$. Si $n = n_0$, posons $V_{n-1} = \{0\}$; sinon, posons

$$
V_{n-1} = \sum_{n_0 \leq i \leq n-1} \varepsilon_i H_i.
$$

Alors $V_{n-1}$ est compact dans $E_n$ et à plus forte raison dans $E_{n+1}$. Comme $U \cap E_{n+1}$ est ouvert dans $E_{n+1}$, il existe un scalaire $\varepsilon_n > 0$ tel que $x + V_n = x + V_{n-1} + \varepsilon_n H_n$ soit contenu dans U (TG, II, p. 31, cor.). Posons $V = \bigcup_{n \geq n_0} V_n$. Alors V est convexe équilibré ; pour $n \geq n_0$, on a $V \cap E_n \supset \varepsilon_n H_n \cap E_n \supset \varepsilon_n W_n$, donc $V \cap E_n$ est un voisinage de 0 dans $E_n$. Ceci achève la démonstration du lemme.

L’ensemble $U = E - \{0\}$ est tel que l’ensemble $U \cap E_n = E_n - \{0\}$ soit ouvert dans $E_n$ pour tout $n$, donc U est ouvert dans E, ce qui prouve que E est séparé (TG, III, p. 5, prop. 2). Il est clair alors que la propriété (ii) de l’énoncé entraîne (iii) et que (iii) entraîne (i). Montrons enfin que (i) entraîne (ii). Il suffit de montrer que si une partie A de E n’est absorbée par aucun des ensembles $\sum_{0 \leq i \leq n} H_i$, alors A n’est pas bornée. Or, il existe alors une suite $(x_n)_{n \geq 1}$ de points de A telle que, pour tout $n$, on ait $x_n \notin n^2 \sum_{0 \leq i \leq n} H_i$. L’ensemble des $x_n / n$ est alors fermé en vertu du lemme 1, car son intersection avec $E_m$ est discrète pour tout entier $m$. Le complémentaire de l’ensemble des $x_n/n$ est donc un voisinage ouvert de 0 qui n’absorbe pas la suite $(x_n)$, et A n’est pas bornée.

#### Remarque 1 {#evt-iii-s1-n4-rem-1 .statement}

Avec les notations ci-dessus, soit $F_n$ l’espace vectoriel engendré par $H_n$, muni de la norme égale à la jauge de $H_n$. Nous verrons (III, p. 8, cor.) que $F_n$ est un espace de Banach ; l’injection de $F_n$ dans $E_{n+1}$ est compacte, donc aussi *a fortiori* l’injection $w_n$ de $F_n$ dans $F_{n+1}$. En outre, E est encore *limite inductive du système inductif* ($F_n, w_n$) *d’espaces de Banach*. En effet, un voisinage convexe équilibré V de 0 dans E est tel que $V \cap E_n$ absorbe $H_{n-1}$ pour tout $n \geq 1$, et inversement, si un ensemble convexe équilibré W dans E est tel que $W \cap E_n$ absorbe $H_{n-1}$, $W \cap E_{n-1}$ contient un homothétique de $W_{n-1}$ pour tout $n \geq 1$, donc W est un voisinage de 0 dans E.

#### Remarque 2 {#evt-iii-s1-n4-rem-2 .statement}

Soient F un espace localement convexe, $k$ un entier $\geq 0$ et $f : E^k \to F$ une application multilinéaire. Pour que $f$ soit continue, il faut et il suffit que la restriction de $f$ à $E_n^k$ soit continue, pour tout $n$. En effet, on vérifie aussitôt que $E^k$ a la topologie localement convexe finale pour la famille d’applications linéaires $v_n \times \cdots \times v_n : E_n \times \cdots \times E_n \to E \times \cdots \times E$ (II, p. 30, cor. 2 et p. 33, prop. 7) et que $u_n \times \cdots \times u_n$ est une application linéaire injective compacte de $(E_n)^k$ dans $(E_{n+1})^k$. Il suffit alors d’appliquer le lemme 1.

### 5. Les espaces $E_A$ (A borné)

Soit E un espace localement convexe et soit A une partie convexe équilibrée de E. Rappelons que $E_A$ désigne l’espace vectoriel engendré par A, muni de la semi-norme $p_A$ jauge de A (II, p. 28, *Exemple 3*). On vérifie immédiatement que l’injection canonique de $E_A$ dans E est continue si et seulement si A est bornée. Si de plus E est séparé, un ensemble borné A ne contient pas de droite (III, p. 2, *Remarque 4*) et $p_A$ est alors une norme (II, *loc. cit.*).

Nous dirons qu’un espace uniforme X est *semi-complet* si toute suite de Cauchy de X est convergente. Un espace uniforme complet est semi-complet, mais la réciproque est inexacte (TG, II, p. 37, exerc. 4) ; toutefois un espace métrisable semi-complet est complet (TG, IX, p. 17, prop. 9).

#### Proposition 8 {#evt-iii-s1-prop-8 .statement}

*Soit E un espace localement convexe séparé et soit A une partie convexe, équilibrée, bornée et fermée de E. Soit $(x_n)$ une suite de Cauchy de $E_A$. Pour qu’elle converge dans $E_A$, il faut et il suffit qu’elle converge dans E.*

L’injection canonique de $E_A$ dans E est continue. Par suite, si $(x_n)$ converge dans $E_A$, elle converge dans E. Inversement, supposons que $(x_n)$ converge vers y dans E. Il existe une suite croissante d’entiers $(n_k)$ telle que $p_A(x_m - x_n) \leq 2^{-k-1}$ si $m \geq n_k$ et $n \geq n_k$. La suite $(x_{n_k} + 2^{-k}A)$ est alors décroissante. Comme A est fermée dans E, on a $y \in \bigcap_k (x_{n_k} + 2^{-k}A)$, ce qui montre que $(x_{n_k})$, donc $(x_n)$, converge vers y dans $E_A$.

#### Corollaire {#evt-iii-s1-n5-cor-1 .statement}

Si $A$ est semi-complète (en particulier, complète), alors $E_A$ est un espace de Banach.
En effet, une suite de Cauchy de $E_A$ est aussi une suite de Cauchy pour la topologie de $E$ et est contenue dans un homothétique de $A$, donc converge dans $E$.

### 6. Ensembles bornés complets et espaces quasi-complets

#### Définition 6 {#evt-iii-s1-def-6 .statement}

On dit qu’un espace localement convexe $E$ est quasi-complet si toute partie bornée et fermée de $E$ est complète (pour la structure uniforme induite par celle de $E$).

Un espace localement convexe complet est quasi-complet, mais la réciproque est inexacte. \* Par exemple, si $E$ est un espace de Hilbert de dimension infinie, ou plus généralement un espace de Banach réflexif de dimension infinie, $E$ muni de sa topologie affaiblie est quasi-complet mais non complet (II, p. 54, prop. 9). \*
Un espace quasi-complet est semi-complet puisque toute suite de Cauchy est contenue dans une partie bornée et fermée (III, p. 3, corollaire et prop. 1). En particulier, un espace localement convexe métrisable et quasi-complet est complet.
Dans un espace quasi-complet séparé, l’adhérence et l’enveloppe fermée convexe équilibrée d’une partie précompacte sont compactes ; en effet, elles sont précompacts (II, p. 27, prop. 3), et complètes car fermées et bornées (III, p. 3, prop. 2).

#### Proposition 9 {#evt-iii-s1-prop-9 .statement}

(i) Un sous-espace vectoriel fermé d’un espace localement convexe quasi-complet est quasi-complet.
(ii) Un produit d’espaces localement convexes quasi-complets est quasi-complet.
(iii) Une somme directe topologique d’espaces localement convexes quasi-complets est quasi-complète.
(iv) Un espace localement convexe limite inductive stricte d’une suite de sous-espaces fermés quasi-complets est quasi-complet.
L’assertion (i) résulte de la Remarque 2 (III, p. 2), (ii) de III, p. 4, cor. 2, (iii) de la prop. 5 (III, p. 5) et (iv) de la prop. 6 (III, p. 5).

On notera qu’un espace quotient d’un espace localement convexe quasi-complet par un sous-espace vectoriel fermé n’est pas nécessairement quasi-complet (IV, p. 64, exerc. 10).

#### Proposition 10 {#evt-iii-s1-prop-10 .statement}

Soient $E$ un espace localement convexe, $M$ un sous-espace vectoriel de $E$ tel que tout point de $E$ soit adhérent à une partie bornée de $M$. Alors toute application linéaire continue $f$ de $M$ dans un espace localement convexe $F$, séparé et quasi-complet, se prolonge d’une seule manière en une application linéaire continue de $E$ dans $F$.
En effet, l’hypothèse entraîne que $M$ est dense dans $E$, donc $f$ se prolonge, d’une seule manière, en une application linéaire continue $\hat{f}$ de $E$ dans le complété $\hat{F}$ de $F$ (TG, III, p. 25, corollaire). Mais tout $x \in E$ est adhérent à une partie bornée $B$ de $M$; alors $\hat{f}(x)$ est adhérent à $f(B)$ dans $\hat{F}$. Or $f(B)$ est borné dans $F$, donc son adhérence dans $F$ est complète, et coïncide avec son adhérence dans $\hat{F}$, ce qui prouve qu’on a $f(x) \in F$.

### 7. Exemples

a) Soit X un espace topologique. Soit $\mathcal{R}(X)$ l’espace vectoriel des fonctions numériques (finies) sur X, muni de la topologie de la convergence compacte (TG, X, p. 4) : c’est la topologie la moins fine rendant continues les applications de restriction $\mathcal{R}(X) \to \mathcal{R}(H)$ (où H décrit la famille des parties compactes de X et où $\mathcal{R}(H)$ est muni de la topologie de la convergence uniforme). Le cor. 3 de III, p. 4 montre qu’une partie A de $\mathcal{R}(X)$ est bornée si et seulement si, pour toute partie compacte H de X, l’ensemble des restrictions à H des fonctions appartenant à A est uniformément borné.

\* b) (Espaces de fonctions indéfiniment dérivables.) Soit $n \geqslant 1$ un entier. Pour tout ouvert U de $\mathbf{R}^n$, on note $\mathcal{C}^\infty(U)$ l’espace vectoriel des fonctions indéfiniment dérivables sur U (VAR, R, 2.3). Soit $f$ dans $\mathcal{C}^\infty(U)$. Pour tout multiindice $\alpha = (\alpha_1, \ldots, \alpha_n)$ dans $\mathbf{N}^n$, on note $\partial^\alpha f$ la dérivée partielle $\partial^{|\alpha|} f / \partial x_1^{\alpha_1} \cdots \partial x_n^{\alpha_n}$; c’est une fonction continue dans U (VAR, R, 2.3 et 2.4). Pour tout entier $m \geqslant 0$ et toute partie compacte H de U, posons

$$
p_{m,H}(f) = \sup_{\substack{|\alpha| \leqslant m \\ x \in H}} |\partial^\alpha f(x)| .
$$

Alors $p_{m,H}$ est une semi-norme sur $\mathcal{C}^\infty(U)$.

On munira $\mathcal{C}^\infty(U)$ de la topologie définie par les semi-normes $p_{m,H}$. C’est la moins fine des topologies rendant continues les applications $f \mapsto \partial^\alpha f$ de $\mathcal{C}^\infty(U)$ dans $\mathcal{R}(U)$, où ce dernier espace est muni de la topologie de la convergence compacte. Il existe une suite croissante de parties compactes $(H_n)_{n \geqslant 0}$ de U dont les intérieurs recouvrent U ; la famille des semi-normes $p_{m,H_n}$ définit la topologie de $\mathcal{C}^\infty(U)$, qui est donc un espace localement convexe métrisable. L’espace $\mathcal{C}^\infty(U)$ est complet, autrement dit, c’est un espace de Fréchet (II, p. 26) : en effet, soit $(f_k)$ une suite de Cauchy dans $\mathcal{C}^\infty(U)$; pour tout $\alpha \in \mathbf{N}^n$, la suite $(\partial^\alpha f_k)$ converge dans l’espace complet $\mathcal{R}(U)$ (TG, X, p. 7, th. 1) vers une fonction continue $g_\alpha$. Par récurrence sur $|\alpha|$, on déduit du th. 1 de FVR, II, p. 2, que l’on a $g_\alpha = \partial^\alpha g_0$ pour tout $\alpha \in \mathbf{N}^n$. Autrement dit, la suite $(f_k)$ converge vers $g_0$ dans $\mathcal{C}^\infty(U)$.

Soit A une partie de $\mathcal{C}^\infty(U)$. Pour que A soit bornée, il faut et il suffit que le nombre $\sup_{f \in A} p_{m,H}(f)$ soit fini quels que soient l’entier $m \geqslant 0$ et la partie compacte H de U ; cette condition signifie que, pour tout $\alpha \in \mathbf{N}^n$, l’ensemble des fonctions $\partial^\alpha f | H$ pour $f \in A$, est uniformément borné pour tout compact $H \subset U$.

Soit $H \subset U$ compact. On note $\mathcal{C}_H^\infty(U)$ le sous-espace de $\mathcal{C}^\infty(U)$ formé des fonctions à support dans H. L’espace $\mathcal{C}_c^\infty(U)$ des fonctions indéfiniment dérivables et à support compact dans U est réunion filtrante croissante des sous-espaces $\mathcal{C}_H^\infty(U)$ lorsque H parcourt l’ensemble des parties compactes de U. Chaque espace $\mathcal{C}_H^\infty(U)$ sera muni de la topologie induite par celle de $\mathcal{C}^\infty(U)$, et $\mathcal{C}_c^\infty(U)$ de la topologie limite inductive correspondante. Si les ensembles $H_n$ sont tels que les intérieurs des $H_n$ forment un recouvrement de U, l’espace $\mathcal{C}_c^\infty(U)$ est limite inductive stricte des espaces de

Fréchet $\mathcal{C}_{\mathbf{H}_n}^\infty(U)$; il est donc complet (II, p. 35, prop. 9), et toute partie bornée de $\mathcal{C}_c^\infty(U)$ est contenue dans l’un des sous-espaces $\mathcal{C}_{\mathbf{H}_n}^\infty(U)$ (III, p. 5, prop. 6). \*

c) (Espaces de Gevrey.) Soit I un intervalle compact de $\mathbf{R}$. Pour tout entier $n \geqslant 0$, on note $D^n f$ la dérivée $n$-ième d’une fonction numérique $f$ définie dans I (lorsque cette dérivée existe). Soient $s \geqslant 1$ et $M \geqslant 0$ deux nombres réels. On note $\mathcal{G}_{s,M}(I)$ l’espace vectoriel des fonctions indéfiniment dérivables $f$ sur I (FVR, I, p. 28) telles que la suite $(|D^n f|/M^n(n!)^s)_{n \geqslant 0}$ soit bornée dans l’espace $\mathcal{C}(I)$ des fonctions continues sur I (muni de la topologie de la convergence uniforme). L’espace $\mathcal{G}_{s,M}(I)$ est un espace de Banach pour la norme

$$
\|f\|_{s,M} = \sup_{n \geqslant 0, x \in I} |D^n f(x)|/M^n(n!)^s .
$$

Pour $M \leqslant M'$, on a $\mathcal{G}_{s,M}(I) \subset \mathcal{G}_{s,M'}(I)$ et

$$
\|f\|_{s,M'} \leqslant \|f\|_{s,M}
$$

pour tout $f \in \mathcal{G}_{s,M}(I)$. On note $\mathcal{G}_s(I)$ la réunion des espaces $\mathcal{G}_{s,M}(I)$ et on le munit de la topologie limite inductive des topologies des $\mathcal{G}_{s,M}(I)$.

Soit $M < M'$ et soit B la boule unité (fermée) dans $\mathcal{G}_{s,M}(I)$. Nous allons montrer que B est une partie *compacte* de l’espace de Banach $\mathcal{G}_{s,M'}(I)$. Il est clair que B est fermée dans $\mathcal{G}_{s,M'}(I)$ et il suffit donc de prouver que B est précompacte dans $\mathcal{G}_{s,M'}(I)$. Soit $\varepsilon > 0$ et soit N un entier positif tel que $(M/M')^N \leqslant \varepsilon/2$. Soit k un entier positif ; l’ensemble des fonctions $D^{k+1} f$, pour $f$ parcourant B, est borné dans $\mathcal{C}(I)$, donc l’ensemble des fonctions $D^k f$, où $f$ parcourt B, est relativement compact dans $\mathcal{C}(I)$ : cela résulte du th. des accroissements finis (FVR, I, p. 23, cor. 1) et du th. d’Ascoli (TG, X, p. 17). Définissons une norme q sur $\mathcal{G}_{s,M}(I)$ par

$$
q(f) = \sup_{\substack{0 \leqslant n \leqslant N \\ x \in I}} |D^n f(x)|/M'^n(n!)^s .
$$

Ce qui précède montre que B est précompacte pour la topologie associée à la norme q ; autrement dit, il existe une partie finie C de B telle que, pour toute $f \in B$, il existe $g \in C$ pour laquelle $q(f - g) \leqslant \varepsilon$. Pour tout $n > N$, on a alors

$$
|D^n f(x) - D^n g(x)|/M'^n(n!)^s \leqslant 2(M/M')^n \leqslant \varepsilon ,
$$

d’où finalement $\|f - g\|_{s,M'} \leqslant \varepsilon$. Ceci prouve que B est précompacte dans $\mathcal{G}_{s,M'}(I)$.

L’espace $\mathcal{G}_s(I)$ est limite inductive des espaces $\mathcal{G}_{s,k}(I)$ où $k$ parcourt $\mathbf{N}$ ; d’après la prop. 7 (III, p. 6), toute partie bornée de $\mathcal{G}_s(I)$ est contenue dans l’un des espaces $\mathcal{G}_{s,k}(I)$ et elle est relativement compacte dans cet espace.

*d*) (Espaces de fonctions holomorphes.) Soit $n \geqslant 1$ un entier. Pour toute partie ouverte U de $\mathbf{C}^n$, on note $\mathcal{H}(U)$ l’espace des fonctions holomorphes dans U, muni de la topologie de la convergence compacte dans U. Pour toute partie compacte L de $\mathbf{C}^n$, on note $\mathcal{H}(L)$ l’espace des germes de fonctions holomorphes au voisinage de L ; on le munit de la topologie localement convexe la plus fine rendant continues les applications canoniques $\pi_U : \mathcal{H}(U) \to \mathcal{H}(L)$, où U parcourt l’ensemble des voisinages ouverts de L.

Pour tout entier $m \geqslant 1$, soit $U_m$ l’ensemble des points de $\mathbf{C}^n$ à distance $< 1/m$ de L. On peut montrer que l’application canonique $\pi_{U_m}$ de $\mathcal{H}(U_m)$ dans $\mathcal{H}(L)$ est injective, et que l’application de restriction de $\mathcal{H}(U_m)$ dans $\mathcal{H}(U_p)$ est compacte pour $p \geqslant m$. On peut donc appliquer la prop. 7 (III, p. 6). Soit A une partie bornée de $\mathcal{H}(L)$; il existe alors un entier $m \geqslant 1$ tel que A se compose des germes au voisinage de L des fonctions appartenant à un ensemble B borné dans $\mathcal{H}(U_m)$. De plus, pour qu’une application $\varphi$ de $\mathcal{H}(L)$ dans un espace topologique T soit continue, il faut et il suffit que l’application $\varphi \circ \pi_U$ de $\mathcal{H}(U)$ dans T soit continue pour tout voisinage ouvert U de L. \*

## EXERCICES {#evt-iii-s1-exercises}

See the [exercises for § 1](exercises/s1/).
