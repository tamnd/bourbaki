---
book: evt
book_title: Topological Vector Spaces
chapter: II
chapter_title: Ensembles convexes et espaces localement convexes
section: 4
section_title: Espaces localement convexes
lang: fr
source: evt-i-v-fr
book_pages: EVT II.25-EVT II.38, EVT II.78-EVT II.81
pdf_pages: 0060-0073, 0113-0116
extraction: ocr
subsections:
    - "no": 1
      title: Définition d’un espace localement convexe
      page: 25
      pdf_page: 60
    - "no": 2
      title: Exemples d’espaces localement convexes
      page: 27
      pdf_page: 62
    - "no": 3
      title: Topologies localement convexes initiales
      page: 29
      pdf_page: 64
    - "no": 4
      title: Topologies localement convexes finales
      page: 29
      pdf_page: 64
    - "no": 5
      title: Somme directe topologique d’une famille d’espaces localement convexes
      page: 32
      pdf_page: 67
    - "no": 6
      title: Limites inductives de suites d’espaces localement convexes
      page: 34
      pdf_page: 69
    - "no": 7
      title: Relèvements dans les espaces de Fréchet
      page: 37
      pdf_page: 72
statements: 35
exercises: 17
content_sha256: b6e1e96a22fcb48eb3f02ce6a319522f67049491fe2e51213d682bbe6c028932
---

## § 4. ESPACES LOCALEMENT CONVEXES

### 1. Définition d’un espace localement convexe

#### Définition 1 {#evt-ii-s4-def-1 .statement}

On dit qu’un espace vectoriel topologique est localement convexe (réel) s’il existe un système fondamental de voisinages de 0 formé d’ensembles convexes.

Si E est un tel espace, on dit pour abréger que E est un espace localement convexe. Une topologie d’espace localement convexe est appelée topologie localement convexe.

Les espaces vectoriels topologiques sur $\mathbf{R}$ que nous aurons à étudier dans la suite de ce Traité seront pour la plupart localement convexes.

Soit V un voisinage convexe de 0 dans un espace localement convexe E ; alors $V \cap (-V)$ est un voisinage convexe et symétrique de 0. Comme l’adhérence d’un ensemble convexe est convexe (II, p. 14, prop. 14), il résulte de I, p. 7, prop. 4 que, dans E, les voisinages de 0 qui sont convexes, symétriques et fermés forment un système fondamental de voisinages de 0, invariant par toute homothétie de centre 0 et de rapport $\neq 0$.

#### Proposition 1 {#evt-ii-s4-prop-1 .statement}

Soient E un espace vectoriel, $\mathfrak{S}$ une base de filtre sur E formée de parties convexes, symétriques et absorbantes. Alors l’ensemble $\mathfrak{B}$ des transformés des ensembles de $\mathfrak{S}$ par les homothéties de rapport $> 0$ est un système fondamental de voisinages de 0 pour une topologie localement convexe sur E.

En effet, il est clair que $\mathfrak{B}$ est une base de filtre et satisfait aux conditions (EV_I) et (EV_{II}) de I, p. 7, prop. 4 ; elle satisfait aussi à la condition (EV_{III}) puisque, pour tout ensemble $V \in \mathfrak{S}$, on a $\frac{1}{2}V + \frac{1}{2}V = V$.

On notera que si $\mathcal{T}$ est la topologie localement convexe sur E ayant $\mathfrak{B}$ pour système fondamental de voisinages de 0, les ensembles $(1/n)V$, où $n$ parcourt l’ensemble des entiers $> 0$ et V parcourt $\mathfrak{S}$, forment encore un système fondamental de voisinages de 0 pour $\mathcal{T}$. Pour que $\mathcal{T}$ soit séparée, il faut et il suffit que, pour tout $x \neq 0$ dans E, il existe un entier $n$ et un ensemble $V \in \mathfrak{S}$ tels que $nx \notin V$ ; si de plus $\mathfrak{S}$ est dénombrable, la topologie $\mathcal{T}$ est une topologie localement convexe métrisable. Inversement, il est clair que si $\mathcal{T}$ est une topologie localement convexe métrisable, il existe un système fondamental dénombrable de voisinages convexes symétriques et fermés de 0 pour $\mathcal{T}$.

#### Corollaire {#evt-ii-s4-n1-cor-1 .statement}

Pour que la topologie $\mathcal{T}$ d’un espace vectoriel topologique E soit définie par un ensemble de semi-normes (II, p. 3), il faut et il suffit que $\mathcal{T}$ soit localement convexe.

En effet, la condition est nécessaire, puisque toute semi-norme $p$ sur E est une fonction convexe, et par suite, pour $\alpha > 0$, l’ensemble des $x \in E$ tels que $p(x) \leq \alpha$ est convexe (II, p. 19, corollaire). Inversement, si V est un voisinage fermé, symétrique et convexe de 0 dans E, la jauge $p$ de V est une semi-norme sur E telle que V soit l’ensemble des $x \in E$ vérifiant $p(x) \leq 1$ (II, p. 22, prop. 23).

Ceci montre en outre qu’une topologie localement convexe $\mathcal{T}$ est définie par l’ensemble de toutes les semi-normes continues pour $\mathcal{T}$. De plus, si $\mathcal{T}$ est métrisable, elle est définie par un ensemble dénombrable de semi-normes.

Compte tenu du corollaire de la prop. 1, les résultats du § 1 sur les topologies définies par des ensembles de semi-normes s’appliquent en particulier aux topologies localement convexes sur les espaces vectoriels réels. Le complété $\hat{E}$ d’un espace localement convexe séparé E est donc un espace localement convexe. On appelle espace de Fréchet un espace localement convexe métrisable et complet ; tout espace de Banach est donc un espace de Fréchet.

#### Proposition 2 {#evt-ii-s4-prop-2 .statement}

Soient E un espace localement convexe, M un sous-espace vectoriel de E, f une forme linéaire définie et continue dans M ; il existe alors une forme linéaire continue h définie dans E et prolongeant f.

En effet, compte tenu de II, p. 26, corollaire et de II, p. 7, cor. 2, il existe une semi-norme $p$ continue sur E, et telle que $|f(y)| \leq p(y)$ pour tout $y \in M$. En vertu du th. de Hahn-Banach (II, p. 24, cor. 1), il existe une forme linéaire $h$ sur E prolongeant $f$ et telle que $|h(x)| \leq p(x)$ pour tout $x \in E$, ce qui entraîne que $h$ est continue (II, p. 7, prop. 5).

#### Remarque {#evt-ii-s4-n1-rem-1 .statement}

Si g est une application linéaire continue de M dans un espace produit $\mathbf{R}^l$, il existe une application linéaire continue $h$ de E dans $\mathbf{R}^l$ qui prolonge $g$ : en effet, on peut écrire $g = (g_i)$, où les $g_i$ sont des formes linéaires continues dans M ; si, pour tout $i \in I$, $h_i$ est une forme linéaire continue dans E et prolongeant $g_i$, l’application linéaire continue $h = (h_i)$ répond à la question.

On notera que si F est un espace localement convexe séparé quelconque et g une application linéaire continue de M dans F, il n’existe pas nécessairement d’application linéaire continue de E dans F qui prolonge g (IV, p. 55, exerc. 16, c)). Il existe toutefois un tel prolongement lorsque M est de dimension finie (cf. cor. 2 ci-dessous).

#### Corollaire 1 {#evt-ii-s4-prop-2-cor-1 .statement}

Soit E un espace localement convexe. Pour tout point $x_0$ non adhérent à 0 dans E, il existe une forme linéaire continue f définie dans E et telle que $f(x_0) \neq 0$.

Il suffit d’appliquer la prop. 2 au sous-espace vectoriel M de dimension 1 engendré par $x_0$ (qui est séparé) et à la forme linéaire $\xi x_0 \mapsto \xi$ définie dans M, qui est continue en vertu de I, p. 13, prop. 2.

#### Corollaire 2 {#evt-ii-s4-prop-2-cor-2 .statement}

Soient E un espace localement convexe séparé, M un sous-espace vectoriel de E de dimension finie. Il existe alors un sous-espace vectoriel fermé N de E, supplémentaire topologique de M dans E.

Pour qu’un sous-espace M de E admette un supplémentaire topologique, il faut et il suffit en effet que l’application identique de M sur lui-même se prolonge en une application linéaire continue u de E sur M, qui est alors nécessairement un projecteur continu (TG, III, p. 47, corollaire). Or, ceci résulte de la remarque (II, p. 26) puisque M est alors isomorphe à un espace $\mathbf{R}^n$ (I, p. 14, th. 2).

#### Proposition 3 {#evt-ii-s4-prop-3 .statement}

Dans un espace localement convexe E, l’enveloppe convexe équilibrée d’un ensemble précompact est un ensemble précompact.

Soit A un ensemble précompact dans E. Pour tout voisinage convexe équilibré V de 0 dans E, il existe un nombre fini de points $a_i \in A$ ($1 \leq i \leq n$) tels que A soit contenu dans la réunion S des voisinages $a_i + V$ ($1 \leq i \leq n$). L’enveloppe convexe équilibrée C de A est donc contenue dans l’enveloppe convexe équilibrée de S ; mais cette dernière est contenue dans B + V, où B est l’enveloppe convexe de l’ensemble fini formé des points $a_i$ et $-a_i$ ($1 \leq i \leq n$). Or, B est précompacte (II, p. 15, cor. 2) ; il existe par suite un nombre fini de points $b_k \in B$ ($1 \leq k \leq m$) tels que B soit contenue dans la réunion des voisinages $b_k + V$. Alors C est contenue dans la réunion des voisinages $b_k + 2V$, ce qui achève la démonstration.

On notera que, dans un espace localement convexe séparé de dimension infinie, l’enveloppe convexe d’un ensemble compact n’est pas nécessairement fermée (II, p. 79, exerc. 3).

#### Corollaire {#evt-ii-s4-n1-cor-2 .statement}

Dans un espace localement convexe séparé E, si un ensemble compact est contenu dans un ensemble convexe complet (pour la structure uniforme induite par celle de E), alors son enveloppe fermée convexe est compacte.

En effet, cette enveloppe est une partie fermée d’un espace complet, donc est un espace complet, et par ailleurs c’est un espace précompact et séparé.

Par contre, dans un espace localement convexe séparé non complet, l’enveloppe fermée convexe d’un ensemble compact peut être non compacte (II, p. 92, exerc. 2).

### 2. Exemples d’espaces localement convexes

1) L’espace $\mathbf{R}^n$ est localement convexe, puisque les cubes ouverts de centre 0 sont convexes (II, p. 9, prop. 6). Il en est donc de même de tout espace vectoriel topologique réel E de *dimension finie* ; en effet, cela résulte de ce qui précède et de I, p. 14, th. 2 si E est séparé ; sinon, l’espace séparé F associé à E est de dimension finie, donc localement convexe, et les images réciproques par l’application canonique $E \to F$ des voisinages convexes de 0 dans F sont convexes et forment un système fondamental de voisinages de 0 dans E.

2) Soit E un espace vectoriel sur $\mathbf{R}$, et soit $\mathfrak{B}$ l’ensemble de *toutes* les parties de E, convexes, symétriques et absorbantes. En vertu de la prop. 1 de II, p. 25, $\mathfrak{B}$ est un système fondamental de voisinages de 0 pour une topologie localement convexe \textit{T}_\omega sur E, qui est évidemment la plus fine de toutes les topologies localement convexes sur E. Cette topologie est séparée : en effet, soit $x \neq 0$ un point quelconque de E ; il existe une base $(e_i)_{i \in I}$ de E et un $\alpha \in I$ tels que $e_\alpha = x$ ; l’ensemble des $y = \sum_i y_i e_i$ tels que $|y_\alpha| < 1$ est un ensemble convexe, symétrique et absorbant auquel $x$ n’appartient pas. Il résulte aussitôt de II, p. 26, corollaire, que $\mathcal{T}_\omega$ est aussi la topologie définie par l’ensemble de toutes les semi-normes sur E, donc toute semi-norme est continue pour $\mathcal{T}_\omega$.

En particulier, si $u$ est une application linéaire de E dans un espace localement convexe quelconque F, l’image réciproque par $u$ de tout voisinage convexe de 0 dans F est un ensemble convexe absorbant dans E, donc un voisinage de 0 pour $\mathcal{T}_\omega$, et par suite $u$ est continue pour $\mathcal{T}_\omega$.

Étant donné un ensemble convexe C dans E, on dit qu’un point $a \in C$ est point interne de C si, pour toute droite D passant par $a$, $D \cap C$ contient un segment ouvert contenant $a$ ; il revient au même de dire que l’ensemble $-a + C$ est absorbant. Pour qu’un point $a$ d’une partie A de E soit intérieur à A pour $\mathcal{T}_\omega$, il faut et il suffit qu’il existe un ensemble convexe C tel que $a \in C \subset A$, et que $a$ soit point interne de C.

Plus généralement, soient V une variété linéaire affine dans E, C un ensemble convexe contenu dans V ; on dit qu’un point $a \in C$ est point interne de C relativement à V si, dans le sous-espace vectoriel $V_0 = -a + V$, le point 0 est point interne de l’ensemble $C_0 = -a + C$.

Lorsque E est de dimension finie, la topologie $\mathcal{T}_\omega$ n’est autre que la topologie canonique sur E (I, p. 14, th. 2) ; cela montre que pour tout ensemble convexe C dans E, tout point interne de C est intérieur à C pour la topologie canonique (cf. II, p. 79, exerc. 5).

3) Soient E un espace vectoriel sur $\mathbf{R}$, A un ensemble convexe symétrique. Le sous-espace vectoriel F engendré par A est aussi le cône convexe engendré par A, puisque $-A = A$, donc est l’ensemble des $\lambda x$, où $x \in A$ et $\lambda \in \mathbf{R}$ ; dans F, l’ensemble A est absorbant, et l’ensemble des $\lambda A$, où $\lambda > 0$, est un système fondamental de voisinages de 0 pour une topologie localement convexe sur F (dite définie par A), qui est définie par la semi-norme $p_A$, jauge de A (II, p. 21, prop. 22) ; on note $E_A$ l’espace localement convexe obtenu en munissant F de cette semi-norme. Pour que l’espace $E_A$ soit séparé, il faut et il suffit que $p_A$ soit une norme, ou encore que A ne contienne aucune droite. Si B est un second ensemble convexe symétrique dans E et si $A \subset B$, il est clair que l’on a $E_A \subset E_B$, et que l’injection canonique de $E_A$ dans $E_B$ est continue pour les topologies définies respectivement par A et B. D’autre part, si $f$ est une application linéaire de E dans un espace vectoriel réel $E'$, $f(A)$ est convexe et symétrique dans $E'$, et $f$ est une application linéaire continue de $E_A$ sur $E'_{f(A)}$.

Notons enfin que si E est muni d’une topologie $\mathcal{T}$ compatible avec sa structure d’espace vectoriel, et si V est un voisinage convexe et symétrique de 0 pour $\mathcal{T}$, l’espace vectoriel engendré par V est identique à E puisque V est absorbant, et l’application identique de E dans $E_V$ est continue.

### 3. Topologies localement convexes initiales

#### Proposition 4 {#evt-ii-s4-prop-4 .statement}

Soient E un espace vectoriel, $(E_i)_{i\in I}$ une famille d’espaces localement convexes, et pour chaque $i \in I$, soit $f_i$ une application linéaire de E dans $E_i$; alors la topologie $\mathcal{T}$ sur E définie comme la moins fine rendant continues toutes les applications $f_i$ est une topologie localement convexe.

En raison de II, p. 26, corollaire, cela est un cas particulier de la propriété correspondante pour les topologies définies par des semi-normes (II, p. 5).

En particulier, tout sous-espace vectoriel d’un espace localement convexe et tout espace produit d’espaces localement convexes sont des espaces localement convexes. Toute limite projective d’espaces localement convexes est localement convexe.

Tout produit dénombrable d’espaces de Fréchet (et en particulier tout produit dénombrable d’espaces de Banach) est un espace de Fréchet.

Tout espace localement convexe séparé E est isomorphe à un sous-espace d’un produit d’espaces de Banach, sous-espace qui est fermé si E est complet (II, p. 5, prop. 3). Tout espace de Fréchet est isomorphe à un sous-espace fermé d’un produit dénombrable d’espaces de Banach (*loc. cit.*).

### 4. Topologies localement convexes finales

#### Proposition 5 {#evt-ii-s4-prop-5 .statement}

Soient E un espace vectoriel, $(F_\alpha)_{\alpha \in A}$ une famille d’espaces vectoriels topologiques, et, pour tout $\alpha \in A$, soit $g_\alpha$ une application linéaire de $F_\alpha$ dans E.

(i) Soit $\mathcal{B}$ l’ensemble des parties convexes, symétriques et absorbantes V de E telles que $g_\alpha^{-1}(V)$ soit un voisinage de 0 dans $F_\alpha$ pour tout $\alpha$; l’ensemble $\mathcal{B}$ est un système fondamental de voisinages de 0 dans E pour une topologie $\mathcal{T}$ compatible avec la structure d’espace vectoriel.

(ii) Pour qu’une application linéaire $f$ de E dans un espace localement convexe G (resp. une semi-norme p sur E) soit continue pour $\mathcal{T}$, il faut et il suffit que, pour tout indice $\alpha$, $f \circ g_\alpha$ (resp. $p \circ g_\alpha$) soit continue dans $F_\alpha$.

(iii) La topologie $\mathcal{T}$ est la plus fine des topologies localement convexes sur E pour lesquelles les $g_\alpha$ sont continues.

En outre, la topologie $\mathcal{T}$ est la seule topologie localement convexe sur E vérifiant la condition (ii) pour les applications linéaires (resp. pour les semi-normes).

Comme $\mathcal{B}$ est une base de filtre invariante par les homothéties de rapport > 0, l’assertion (i) résulte aussitôt de II, p. 25, prop. 1. Par définition de $\mathcal{B}$, $\mathcal{T}$ est la plus fine des topologies localement convexes sur E rendant continues les $g_\alpha$, d’où (iii). Enfin, il est clair que si $f$ est continue, il en est de même des $f \circ g_\alpha$; réciproquement, si ces dernières sont continues pour tout $\alpha$, alors, pour tout voisinage convexe symétrique W de 0 dans G, $g_\alpha^{-1}(f^{-1}(W))$ est un voisinage de 0 dans $F_\alpha$ pour tout indice $\alpha$, et comme $f^{-1}(W)$ est convexe, symétrique et absorbant, cela prouve que $f^{-1}(W)$ est un voisinage de 0 pour $\mathcal{T}$, donc que $f$ est continue. De même, si une semi-norme $p$ sur $E$ est telle que $p \circ g_\alpha$ soit continue pour tout $\alpha$, et si $U$ est l’ensemble des $x \in E$ tels que $p(x) < 1$, alors, pour tout $\alpha$, $g_\alpha^{-1}(U)$ est un voisinage convexe de 0 dans $E_\alpha$, symétrique et absorbant ; donc $U$ est un voisinage de 0 dans $E$, et $p$ est continue (II, p. 2, prop. 1).

La dernière assertion résulte de E, IV, p. 19, critère CST 18.

On dit parfois que $\mathcal{T}$ est la topologie localement convexe finale de la famille des topologies $\mathcal{T}_\alpha$ des $F_\alpha$, pour la famille des applications linéaires $g_\alpha$.

Il peut se faire que $\mathcal{T}$ ne soit pas la plus fine des topologies sur $E$ compatibles avec la structure d’espace vectoriel et rendant continues les $f_\alpha$ (II, p. 80, exerc. 15 ; voir toutefois II, p. 80, exerc. 14).

Dans le cas (le plus important) où $E = \sum_{\alpha \in A} g_\alpha(F_\alpha)$ on obtient encore un système fondamental de voisinages de 0 pour $\mathcal{T}$ de la façon suivante : on considère toutes les familles $(V_\alpha)_{\alpha \in A}$ où, pour tout $\alpha \in A$, $V_\alpha$ est un voisinage symétrique de 0 pour $\mathcal{T}_\alpha$, et on prend l’enveloppe convexe dans $E$, $\Gamma((g_\alpha(V_\alpha)))$, de la réunion des $g_\alpha(V_\alpha)$. En effet, tout élément de $E$ étant de la forme $\sum_{\alpha \in J} x_\alpha$, où $J$ est une partie finie de $A$ et $x_\alpha \in g_\alpha(F_\alpha)$, il est immédiat que $\Gamma((g_\alpha(V_\alpha)))$ est un ensemble convexe symétrique et absorbant dans $E$ (chacun des $V_\alpha$ étant absorbant dans $F_\alpha$) ; comme $\Gamma((g_\alpha(V_\alpha)))$ contient tous les $g_\alpha(V_\alpha)$, c’est un voisinage de 0 pour $\mathcal{T}$. D’autre part, il est clair que pour tout voisinage convexe symétrique $V$ de 0 pour $\mathcal{T}$, on a $V \supset \Gamma((V \cap g_\alpha(F_\alpha)))$, d’où notre assertion.

#### Corollaire 1 {#evt-ii-s4-prop-5-cor-1 .statement}

Avec les notations de la prop. 5, soit $H$ un ensemble d’applications linéaires de $E$ dans un espace localement convexe $G$. Supposons que $E$ soit somme des sous-espaces $g_\alpha(F_\alpha)$ ; alors, pour que $H$ soit équicontinu pour $\mathcal{T}$, il faut et il suffit que, pour tout $\alpha$, l’ensemble des $f \circ g_\alpha$, où $f$ parcourt $H$, soit équicontinu dans $F_\alpha$.

Compte tenu de I, p. 9, prop. 6, la démonstration suit la même marche que pour l’assertion (ii) de la prop. 5, en considérant un voisinage convexe symétrique $W$ de 0 dans $G$ et en notant que, si l’ensemble des $f \circ g_\alpha$ pour $f \in H$ est équicontinu dans $G$ et en notant que, si l’ensemble des $f \circ g_\alpha$ pour $f \in H$ est équicontinu dans $F_\alpha$, l’intersection $\bigcap_{f \in H} g_\alpha^{-1}(f^{-1}(W))$ est un voisinage convexe symétrique de 0 dans $F_\alpha$. Comme cette intersection est égale à $g_\alpha^{-1}(\bigcap_{f \in H} f^{-1}(W))$ et que l’ensemble $\bigcap_{f \in H} f^{-1}(W)$ est convexe et symétrique, tout revient à voir qu’il est aussi absorbant. Or, par hypothèse, tout $x \in E$ s’écrit sous la forme $\sum_{i=1}^n g_{\alpha_i}(z_{\alpha_i})$, où $z_{\alpha_i} \in F_{\alpha_i}$. Pour montrer qu’il existe $\lambda > 0$ tel que $f(\lambda x) \in W$ pour toute $f \in H$, il suffit donc de le faire lorsque $x$ est de la forme $g_\alpha(z_\alpha)$ avec $z_\alpha \in F_\alpha$ (car on passera de là au cas général en remplaçant $W$ par l’ensemble $W/n$). Mais alors la conclusion résulte de ce que l’ensemble $g_\alpha^{-1}(\bigcap_{f \in H} f^{-1}(W))$ est un voisinage de 0 dans $F_\alpha$.

#### Corollaire 2 {#evt-ii-s4-prop-5-cor-2 .statement}

Soient $E$ un espace vectoriel, $(G_\alpha)_{\alpha \in A}$ une famille d’espaces localement convexes, $(J_\lambda)_{\lambda \in L}$ une partition de $A$, et $(F_\lambda)_{\lambda \in L}$ une famille d’espaces vectoriels.

Pour tout $\lambda \in L$, soit $h_\lambda$ une application linéaire de $F_\lambda$ dans $E$; pour tout $\lambda \in L$ et tout $\alpha \in J_\lambda$, soit $g_{\lambda \alpha}$ une application linéaire de $G_\alpha$ dans $F_\lambda$; on pose alors $f_\alpha = h_\lambda \circ g_{\lambda \alpha}$. On munit chacun des $F_\lambda$ de la topologie localement convexe la plus fine rendant continues les $g_{\lambda \alpha}$ ($\alpha \in J_\lambda$); alors, sur $E$, la topologie localement convexe la plus fine rendant continues les $f_\alpha$ est identique à la topologie localement convexe la plus fine rendant continues les $h_\lambda$.

C’est un cas particulier de E, IV, p. 20, critère CST 19, et se démontre d’ailleurs aussitôt directement en utilisant la prop. 5.

Exemples de topologies localement convexes finales.

I. Espace quotient.
Soient $F$ un espace localement convexe, $M$ un sous-espace de $F$, $\varphi$ l’application canonique de $F$ sur $F/M$. Comme la topologie quotient sur $F/M$ est localement convexe et est la plus fine de toutes les topologies (localement convexes ou non) rendant continue $\varphi$, c’est la topologie localement convexe finale pour la famille réduite à $\varphi$.

II. Limites inductives d’espaces localement convexes.
Soient $A$ un ensemble ordonné filtrant à droite, $(E_\alpha, f_{\beta \alpha})$ un système inductif d’espaces vectoriels relatif à l’ensemble $A$ (A, II, p. 90); soit $E = \lim_{\longrightarrow} E_\alpha$ et soit $f_\alpha : E_\alpha \to E$ l’application linéaire canonique pour tout $\alpha \in A$. Supposons chaque $E_\alpha$ muni d’une topologie localement convexe $\mathcal{T}_\alpha$, et en outre, supposons que pour $\alpha \leq \beta$, $f_{\beta \alpha} : E_\alpha \to E_\beta$ soit continue. On dit alors que la topologie localement convexe finale $\mathcal{T}$ de la famille $(\mathcal{T}_\alpha)$ relativement aux applications linéaires $f_\alpha$ (resp. l’espace $E$ muni de $\mathcal{T}$) est la limite inductive de la famille $(\mathcal{T}_\alpha)$ (resp. l’espace limite inductive du système $(E_\alpha, f_{\beta \alpha})$), ou simplement des espaces localement convexes $E_\alpha$. Rappelons que $E$ est réunion des sous-espaces vectoriels $f_\alpha(E_\alpha)$ et que lorsque $\alpha \leq \beta$, on a $f_\alpha(E_\alpha) \subset f_\beta(E_\beta)$; si l’on munit $f_\alpha(E_\alpha)$ de la topologie finale pour l’application $f_\alpha$ (ce qui revient à identifier $f_\alpha(E_\alpha)$ à l’espace quotient $E_\alpha/f_\alpha^{-1}(0)$), la topologie $\mathcal{T}$ est aussi la topologie finale de la famille des topologies des $f_\alpha(E_\alpha)$, relativement aux injections canoniques (II, p. 30, cor. 2). En outre, la continuité de $f_{\beta \alpha}$ pour $\alpha \leq \beta$ entraîne que l’injection canonique $j_{\beta \alpha} : f_\alpha(E_\alpha) \to f_\beta(E_\beta)$ est continue, de sorte que $E$ est aussi l’espace limite inductive des $f_\alpha(E_\alpha)$ munis des topologies précédentes, relativement aux injections $j_{\beta \alpha}$.

#### Exemple {#evt-ii-s4-n4-exa-1 .statement}

Soient $X$ un espace localement compact, $E = \mathscr{K}(X; \mathbf{R})$ l’espace vectoriel des fonctions numériques finies $f$ continues dans $X$ à support compact. Pour toute partie compacte $K$ de $X$, soit $E_K$ le sous-espace vectoriel de $E$ formé des fonctions $f \in E$ nulles hors de $K$, et désignons par $\mathcal{T}_K$ la topologie induite sur $E_K$ par la topologie $\mathcal{T}_u$ de la convergence uniforme sur $X$. La limite inductive $\mathcal{T}$ des topologies $\mathcal{T}_K$ est plus fine que $\mathcal{T}_u$; on peut montrer que si $X$ est paracompact et non compact $\mathcal{T}$ est strictement plus fine que $\mathcal{T}_u$ (cf. INT, III, 2e éd., § 1, no 8). L’importance de la topologie $\mathcal{T}$ tient à ce que les formes linéaires sur $E$, continues pour $\mathcal{T}$, ne sont autres que les mesures (réelles) sur $X$ (INT, III, 2e éd., § 1, no 3).

#### Remarque {#evt-ii-s4-n4-rem-1 .statement}

Dans ce dernier exemple, la topologie induite par $\mathcal{T}$ sur $E_K$ est identique à $\mathcal{T}_K$, car elle est par définition moins fine que $\mathcal{T}_K$, et comme par ailleurs $\mathcal{T}$ est plus fine que $\mathcal{T}_u$, la topologie induite par $\mathcal{T}$ sur $E_K$ est plus fine que celle induite par $\mathcal{T}_u$, c’est-à-dire $\mathcal{T}_K$.

Ce raisonnement se généralise aussitôt à une limite inductive de topologies localement convexes ($\mathcal{T}_\alpha$) lorsqu’il existe sur $E$ une topologie localement convexe $\mathcal{T}'$ telle que $\mathcal{T}_\alpha$ soit la topologie induite sur $E_\alpha$ par $\mathcal{T}'$.

Plus généralement, on peut se demander si, lorsque l’on suppose que pour $E_\beta \subset E_\alpha$, $\mathcal{T}_\beta$ est égale à la topologie induite par $\mathcal{T}_\alpha$, alors $\mathcal{T}$ induit $\mathcal{T}_\alpha$ sur chacun des $E_\alpha$. La réponse à cette question est négative dans le cas général (II, p. 85, exerc. 26) ; mais nous allons voir dans les n°s suivants deux cas importants où elle est affirmative.

### 5. Somme directe topologique d’une famille d’espaces localement convexes

#### Définition 2 {#evt-ii-s4-def-2 .statement}

Soit $(E_i)_{i \in I}$ une famille d’espaces localement convexes, et soit $E$ l’espace vectoriel somme directe de la famille $(E_i)$ (A, II, p. 12). Pour tout $i \in I$, soit $f_i$ l’injection canonique de $E_i$ dans $E$. On appelle somme directe topologique de la famille $(E_i)$ l’espace $E$ muni de la topologie localement convexe la plus fine rendant continues les $f_i$ (topologie dite somme directe des topologies des $E_i$).

Dans toute la suite de ce n°, nous garderons (sauf mention expresse du contraire) les notations de la déf. 2 et nous identifierons canoniquement chaque $E_i$ à un sous-espace de $E$ au moyen de $f_i$.

En vertu de la description générale des voisinages d’une topologie localement convexe finale donnée dans II, p. 30, on obtient ici un système fondamental de voisinages de 0 dans $E$ pour la topologie somme directe de la façon suivante : pour toute famille $(V_i)_{i \in I}$, où $V_i$ est un voisinage convexe symétrique de 0 dans $E_i$, on considère l’enveloppe convexe $\Gamma((V_i))$ de la réunion des $V_i$; les $\Gamma((V_i))$, pour toutes les familles $(V_i)$ (ou seulement en prenant pour chaque $i$ les $V_i$ dans un système fondamental de voisinages de 0 dans $E_i$) forment un système fondamental de voisinages de 0 dans $E$.

#### Exemple {#evt-ii-s4-n5-exa-1 .statement}

Soient $E$ un espace vectoriel, $(a_i)_{i \in I}$ une base de $E$, et considérons sur chaque droite $Ra_i$ la topologie canonique (I, p. 2, Exemple 5) ; la topologie somme directe de ces topologies n’est autre que la topologie localement convexe la plus fine sur $E$ (II, p. 28) : en effet, si $V$ est un ensemble convexe, symétrique et absorbant dans $E$, $V_i = V \cap Ra_i$ est un voisinage de 0 dans $Ra_i$, et $V$ contient évidemment l’enveloppe convexe $\Gamma((V_i))$.

#### Proposition 6 {#evt-ii-s4-prop-6 .statement}

Pour qu’une topologie localement convexe $\mathcal{T}$ sur $E$ soit somme directe des topologies des $E_i$, il faut et il suffit qu’elle possède la propriété suivante : pour qu’une application linéaire $g$ de $E$ dans un espace localement convexe $G$ (resp. une semi-norme $p$ sur $E$) soit continue, il faut et il suffit que, pour tout $i \in I$, $g \circ f_i$ (resp. $p \circ f_i$) soit continue dans $E_i$.

C’est un cas particulier de la prop. 5 de II, p. 29.

Compte tenu de la définition de la somme directe d’une famille d’espaces vectoriels (A, II, p. 12, prop. 6), on peut encore dire que la topologie $\mathcal{T}$ est la seule pour laquelle l’application canonique $g \mapsto (g \circ f_i)$ soit une bijection

$$
\mathscr{L}(E; G) \to \prod_{i \in I} \mathscr{L}(E_i; G)
$$

pour tout espace localement convexe $G$.

#### Corollaire {#evt-ii-s4-n5-cor-1 .statement}

Les notations étant celles de la prop. 5 de II, p. 29, supposons que $E$ soit somme des $g_\alpha(F_\alpha)$. Soient $F$ l’espace somme directe topologique de la famille $(F_\alpha)_{\alpha \in A}$, $j_\alpha : F_\alpha \to F$ l’injection canonique, et soit $g : F \to E$ l’application linéaire telle que $g \circ j_\alpha = g_\alpha$ pour tout $\alpha \in A$. Si $N$ est le noyau de $g$, la bijection canonique $F/N \to E$ associée à $g$ est un isomorphisme topologique de $F/N$ sur $E$ muni de $\mathcal{T}$.

C’est un cas particulier de II, p. 30, cor. 2, compte tenu de II, p. 31, Exemple I.

#### Proposition 7 {#evt-ii-s4-prop-7 .statement}

L’injection canonique $j : E \to \prod_{i \in I} E_i$ est continue lorsqu’on munit $E$ de la topologie somme directe des topologies des $E_i$ et $\prod_{i \in I} E_i$ de la topologie produit. Lorsque $I$ est fini, cette application est un isomorphisme d’espaces vectoriels topologiques.

La première assertion résulte de ce que les injections canoniques $E_k \to \prod_{i \in I} E_i$ sont continues pour tout $k \in I$. Si $I$ est fini, $j$ est l’application identique, et il suffit de prouver que la topologie produit $\mathcal{T}'$ est plus fine que la topologie somme directe $\mathcal{T}$. Or, soit $V$ un voisinage convexe de 0 pour $\mathcal{T}$; chacun des $V \cap E_i$ est un voisinage convexe de 0 dans $E_i$; si $n$ est le nombre d’éléments de $I$, l’ensemble $V$ contient donc l’ensemble $\frac{1}{n} \sum_n (V \cap E_i)$, qui est un voisinage de 0 pour $\mathcal{T}'$, d’où la proposition.

Lorsque $I$ est infini, si, pour toute partie finie $J$ de $I$, on note $E_J$ l’espace $\prod_{i \in J} E_i$, muni de la topologie produit, $E$ est limite inductive des $E_J$ (identifiés à des sous-espaces de $E$).

#### Proposition 8 {#evt-ii-s4-prop-8 .statement}

Pour tout $i \in I$, soit $N_i$ un sous-espace de $E_i$.
(i) La topologie induite sur $N = \sum_i N_i$ par la topologie somme directe $\mathcal{T}$ sur $E$ est identique à la somme directe des topologies des $N_i$.
(ii) L’application canonique $h$ de l’espace somme directe topologique des $E_i/N_i$ sur $E/N$ (A, II, p. 14, formule (26)) est un isomorphisme d’espaces vectoriels topologiques.

(i) Avec les notations introduites plus haut, considérons un point $x = \sum_i \lambda_i x_i$ appartenant à $N \cap \Gamma((V_i))$ (($\lambda_i$) famille de nombres $\geq 0$ à support fini telle que $\sum_i \lambda_i = 1$, $x_i \in V_i$ pour tout $i \in I$). On a nécessairement, pour tout $i \in I$, $\lambda_i x_i \in N_i$, la somme des $N_i$ étant directe ; donc, pour tout $i$ tel que $\lambda_i > 0$, on a aussi $x_i \in N_i \cap V_i$, et $x$ appartient à l’enveloppe convexe $\Gamma((N_i \cap V_i))$, ce qui prouve (i).

(ii) Soient $f_i : E_i \to E, h_i : E_i/N_i \to E/N, p_i : E_i \to E_i/N_i$ et $p : E \to E/N$ les applications canoniques. On a $h_i \circ p_i = p \circ f_i$ pour tout $i \in I$, et la proposition résulte de II, p. 30, cor. 2 et p. 31, Exemple I.

#### Corollaire 1 {#evt-ii-s4-prop-8-cor-1 .statement}

*Si, pour tout $i \in I, N_i$ est fermé dans $E_i$, alors $N = \sum N_i$ est fermé dans $E$.*

En effet, pour tout $i \in I$, la projection canonique $p_i : E \to E_i$ est continue (II, p. 32, prop. 6) ; par suite $p_i^{-1}(N_i)$ est fermé dans $E$, donc il en est de même de l’intersection $N = \bigcap_{i \in I} p_i^{-1}(N_i)$.

#### Corollaire 2 {#evt-ii-s4-prop-8-cor-2 .statement}

*Si chacun des $E_i$ est séparé, il en est de même de $E$, et chacun des $E_i$ est fermé dans $E$.*

Pour prouver la première assertion, il suffit d’appliquer le cor. 1 en prenant $N_i = \{0\}$ pour tout $i \in I$ ; pour prouver la seconde, il suffit d’appliquer le cor. 1 en prenant $N_i = E_i$ et $N_k = \{0\}$ pour tout $k \neq i$.

Nous montrerons au chap. III, p. 21, cor. 2 que si les $E_i$ sont séparés et *complets*, il en est de même de leur somme directe topologique $E$.

### 6. Limites inductives de suites d’espaces localement convexes

Dans ce n°, nous allons considérer une *suite croissante* ($E_n$) de sous-espaces vectoriels d’un espace vectoriel $E$, telle que $E$ soit *réunion* des $E_n$ ; nous supposerons chacun des $E_n$ muni d’une topologie localement convexe $\mathcal{T}_n$, telle que, pour tout $n$, la topologie induite sur $E_n$ par $\mathcal{T}_{n+1}$ soit *moins fine* que $\mathcal{T}_n$, et nous munirons $E$ de la topologie localement convexe $\mathcal{T}$ *limite inductive* de la suite $(\mathcal{T}_n)$ (II, p. 31, *Exemple II*) ; ces hypothèses et notations ne seront pas répétées dans ce n°.

Il peut se faire que les $\mathcal{T}_n$ soient toutes *séparées* sans que $\mathcal{T}$ le soit ; il peut se faire aussi que pour tout couple d’entiers $n, m$ tels que $n \leq m$, $E_n$ soit fermé (pour $\mathcal{T}_m$) dans $E_m$, sans que $E_n$ soit fermé dans $E$ pour $\mathcal{T}$ (II, p. 85, exerc. 26).

#### Lemme 1 {#evt-ii-s4-lem-1 .statement}

*Soit $\mathfrak{F}$ un filtre de Cauchy sur $E$ (pour $\mathcal{T}$) ; il existe un entier $k$ tel que, pour tout $N \in \mathfrak{F}$ et tout voisinage $V$ de 0 dans $E$, $E_k$ rencontre $N + V$.*

Raisonnons par l’absurde ; pour tout $k$, il existerait un voisinage convexe $V_k$ de 0 et un ensemble $M_k \in \mathfrak{F}$ tels que

$$
(E_k + V_k) \cap M_k = \varnothing .
$$

On peut évidemment supposer $V_{k+1} \subset V_k$ pour tout $k$. Soit $V$ l’enveloppe convexe de $\bigcup_k (E_k \cap V_k)$, qui est évidemment un voisinage de 0 pour $\mathcal{T}$. On a $V \subset V_n + E_n$ pour tout $n$ : en effet, tout $x \in V$ s’écrit $\sum_i \lambda_i x_i$ où $\lambda_i \geq 0$, $\sum_i \lambda_i = 1$ et $x_i \in V_i \cap E_i$ pour tout $i$ ; or, pour $i < n$, on a $x_i \in E_n$, donc $\sum_{i < n} \lambda_i x_i \in E_n$ ; et pour $i \geq n$, on a $x_i \in V_n$, donc

$$
\sum_{i \geq n} \lambda_i x_i \in V_n \text{ puisque } V_n \text{ est convexe et contient } 0, \text{ et } \sum_{i \geq n} \lambda_i \leq 1. \text{ On a par suite } V + E_n \subset V_n + E_n \text{ pour tout } n. \text{ Cela étant, soit } M \in \mathcal{F} \text{ un ensemble petit d'ordre } V. \text{ Il existe un entier } m \text{ tel que } E_m \cap M \text{ soit non vide ; on en conclut que l'on a}
$$
$$
M \subset E_m + V \subset E_m + V_m ;
$$
comme $\mathcal{F}$ est un filtre, l’ensemble $M_m$ rencontre $M$, donc $E_m + V_m$, et nous avons abouti à une contradiction, d’où le lemme.

#### Proposition 9 {#evt-ii-s4-prop-9 .statement}

*Supposons que, pour chaque entier n, la topologie induite sur $E_n$ par $\mathcal{T}_{n+1}$ soit identique à $\mathcal{T}_n$. Dans ces conditions :*
(i) *Pour tout n, la topologie induite par $\mathcal{T}$ sur $E_n$ est identique à $\mathcal{T}_n$; si les $\mathcal{T}_n$ sont séparées, $\mathcal{T}$ est séparée.*
(ii) *Supposons que pour tout n, $E_n$ soit fermé dans $E_{n+1}$ (pour $\mathcal{T}_{n+1}$). Alors, pour tout n, $E_n$ est fermé dans $E$ (pour $\mathcal{T}$).*
(iii) *Si chacun des $E_n$ est complet (pour $\mathcal{T}_n$), alors $E$ est complet pour $\mathcal{T}$.*

(i) Pour établir la première assertion, il suffit de prouver que la topologie $\mathcal{T}_n'$ induite par $\mathcal{T}$ sur $E_n$ est plus fine que $\mathcal{T}_n$. Pour cela, soit $V_n$ un voisinage convexe de 0 dans $E_n$ pour la topologie $\mathcal{T}_n$; nous allons construire une suite croissante $(V_{n+p})_{p \geq 1}$ telle que $V_{n+p}$ soit un voisinage convexe de 0 dans $E_{n+p}$ pour $\mathcal{T}_{n+p}$ et que l’on ait $V_{n+p} \cap E_n = V_n$ pour tout indice $p \geq 1$. Alors la réunion $V$ de la suite croissante $(V_{n+p})$ sera un ensemble convexe tel que, pour tout indice $k$, $V \cap E_k$ soit un voisinage de 0 pour $\mathcal{T}_k$, donc $V$ sera un voisinage de 0 pour $\mathcal{T}$, et comme $V \cap E_n = V_n$, on aura prouvé que $\mathcal{T}_n'$ est plus fine que $\mathcal{T}_n$.

Pour définir les $V_{n+p}$, il suffit de procéder par récurrence sur $p$, en utilisant le lemme suivant :

#### Lemme 2 {#evt-ii-s4-lem-2 .statement}

*Soient F un espace localement convexe, M un sous-espace vectoriel de F, V un voisinage convexe de 0 dans M. Il existe alors un voisinage convexe W de 0 dans F tel que $W \cap M = V$. En outre, si M est fermé dans F, alors, pour tout point $x_0 \in \mathbf{C} M$, il existe un voisinage convexe $W_0$ de 0 dans F tel que $W_0 \cap M = V$ et $x_0 \notin W_0$.*

En effet, il existe par hypothèse un voisinage convexe U de 0 dans F tel que l’on ait $U \cap M \subset V$. L’enveloppe convexe W de $U \cup V$ dans F est évidemment un voisinage de 0 dans F ; montrons que $W \cap M = V$. En effet, tout point $z \in W$ est de la forme $\lambda x + (1 - \lambda) y$ avec $x \in V, y \in U$, et $0 \leq \lambda \leq 1$ (II, p. 10, prop. 8) ; si $z \in M$, on a nécessairement $y \in M$ si $\lambda \neq 1$, donc $y \in U \cap M \subset V$, et par suite $z \in V$ ; la conclusion subsiste évidemment encore si $\lambda = 1$. Si M est fermé dans F, l’espace F/M est séparé, donc il existe un voisinage convexe $U_0 \subset U$ de 0 dans F tel que $U_0$ ne rencontre pas $x_0 + M$ ; l’enveloppe convexe $W_0$ de $U_0 \cup V$ répond alors aux conditions de l’énoncé.

Pour achever de prouver (i), il suffit de remarquer que tout $x \in E$ appartient à un $E_n$ ; si $x \neq 0$ et si $\mathcal{T}_n$ est séparée, il y a un voisinage $V_n$ de 0 pour $\mathcal{T}_n$ ne contenant pas $x$, et nous venons de voir qu’il y a un voisinage V de 0 pour $\mathcal{T}$ tel que $V \cap E_n = V_n$, donc on a $x \notin V$, ce qui prouve que $\mathcal{T}$ est séparée.

(ii) Soit $x \in E - E_n$; il existe $m > n$ tel que $x \in E_m$, donc, comme $E_n$ est fermé dans $E_m$ pour $\mathcal{T}_m$ (en vertu de l’hypothèse que $\mathcal{T}_{n+1}$ induit $\mathcal{T}_n$ sur $E_n$ pour tout $n$), il existe pour $\mathcal{T}_m$ un voisinage convexe $V_m$ de 0 dans $E_m$ tel que $(x + V_m) \cap E_n = \varnothing$. Or, on a vu dans (i) qu’il existe un voisinage convexe $V$ de 0 pour $\mathcal{T}$ tel que l’on ait $V \cap E_m = V_m$; on a par suite $(x + V) \cap E_m = x + V_m$, donc $(x + V) \cap E_n = \varnothing$, ce qui démontre (ii).

(iii) Il résulte du lemme 1 que si $\mathfrak{F}$ est un filtre de Cauchy minimal pour $\mathcal{T}$ (TG, II, p. 14), il existe un indice $k$ tel que la trace de $\mathfrak{F}$ sur $E_k$ soit un filtre $\mathfrak{F}_k$; ce dernier est un filtre de Cauchy pour $\mathcal{T}_k$ d’après (i), et par suite $\mathfrak{F}_k$ converge dans $E_k$ par hypothèse ; mais comme le filtre sur $E$ engendré par $\mathfrak{F}_k$ est plus fin que $\mathfrak{F}$, $\mathfrak{F}$ admet un point adhérent pour $\mathcal{T}$, et par suite converge pour $\mathcal{T}$.

Lorsque pour tout $n$ la topologie induite sur $E_n$ par $\mathcal{T}_{n+1}$ est égale à $\mathcal{T}_n$, on dit que $\mathcal{T}$ est la limite inductive stricte de la suite $(\mathcal{T}_n)$, et que l’espace $E$, muni de $\mathcal{T}$, est limite inductive stricte de la suite des espaces localement convexes $E_n$.

#### Remarque 1 {#evt-ii-s4-n6-rem-1 .statement}

Supposons que $E$ soit réunion d’une famille filtrante croissante non dénombrable de sous-espaces $(E_\alpha)_{\alpha \in I}$, chaque $E_\alpha$ étant muni d’une topologie localement convexe $\mathcal{T}_\alpha$ telle que, pour $E_\alpha \subset E_\beta$, la topologie induite sur $E_\alpha$ par $\mathcal{T}_\beta$ soit égale à $\mathcal{T}_\alpha$. Il peut se faire alors que la topologie induite sur tout $E_\alpha$ par la topologie $\mathcal{T}$ soit égale à $\mathcal{T}_\alpha$, et que les $E_\alpha$ soient séparés et complets, sans que $E$ soit complet pour $\mathcal{T}$ (INT, III, 2e éd., § 1, exerc. 2).

#### Remarque 2 {#evt-ii-s4-n6-rem-2 .statement}

Soit $F$ un espace localement convexe, réunion d’une suite croissante $(F_n)$ de sous-espaces vectoriels, et pour chaque indice $n$, soit $\mathcal{T}_n$ la topologie induite sur $F_n$ par la topologie $\mathcal{T}$ de $F$. On se gardera de croire qu’en général $\mathcal{T}$ soit égale à la limite inductive des $\mathcal{T}_n$.

#### Remarque 3 {#evt-ii-s4-n6-rem-3 .statement}

Supposons que $E$ soit limite inductive stricte de la suite $(E_n)$; si $F$ est un sous-espace vectoriel fermé de $E$ (pour $\mathcal{T}$), il peut se faire que la limite inductive stricte des topologies induites par les $\mathcal{T}_n$ sur $F \cap E_n$ soit strictement plus fine que la topologie induite par $\mathcal{T}$ (IV, p. 64, exerc. 10).

#### Proposition 10 {#evt-ii-s4-prop-10 .statement}

Soient $E, F$ deux espaces localement convexes. On suppose que :

1) Il existe une famille $(E_\alpha)$ d’espaces de Fréchet et pour chaque $\alpha$ une application linéaire $g_\alpha : E_\alpha \to E$, telles que la topologie de $E$ soit la topologie localement convexe finale pour la famille $(g_\alpha)$.

2) Il existe une suite $(F_n)$ d’espaces de Fréchet, et pour chaque $n$ une injection linéaire continue $j_n : F_n \to F$ telles que $F = \bigcup_n j_n(F_n)$.

Alors toute application linéaire $u$ de $E$ dans $F$ dont le graphe est fermé dans $E \times F$ est continue.

Pour prouver que $u$ est continue, il suffit de voir que pour tout $\alpha$, $u \circ g_\alpha : E_\alpha \to F$ est continue (II, p. 29, prop. 5). Or, le graphe de $u \circ g_\alpha$ est l’image réciproque du graphe de $u$ par l’application continue $g_\alpha \times 1_F : E_\alpha \times F \to E \times F$, donc est fermé par hypothèse dans $E_\alpha \times F$. On peut ainsi se borner au cas où $E$ lui-même est un espace de Fréchet. Mais alors la proposition est un cas particulier de I, p. 20, prop. 1.

#### Corollaire {#evt-ii-s4-n6-cor-1 .statement}

Les hypothèses sur $E$ et $F$ étant les mêmes que dans la prop. 10, et $E$ étant supposé séparé, toute application continue surjective $v$ de $F$ dans $E$ est un morphisme strict.

Soit en effet N le noyau de v, et posons $N_n = j_n^{-1}(N)$; alors l’application $j'_n : F_n/N_n \to F/N$ déduite de $j_n$ par passage aux quotients est injective et continue, $F_n/N_n$ est un espace de Fréchet (puisque $N_n$ est fermé), et $F/N$ est réunion des images des $j'_n$. Par hypothèse, dans la factorisation canonique $v : F \to F/N \xrightarrow{w} E$, w est une application linéaire bijective et continue, dont le graphe dans $(F/N) \times E$ est donc fermé (TG, I, p. 53, cor. 2 de la prop. 2). En vertu des remarques du début et de la prop. 10, l’application réciproque $u$ de $w$ est donc continue, ce qui prouve le corollaire.

\* La prop. 10 et son corollaire s’appliqueront en particulier lorsque E est un espace bornologique (III, p. 12) complet, et F une limite inductive d’une suite d’espaces de Fréchet. \*

### 7. Relèvements dans les espaces de Fréchet

Nous allons préciser dans le cas des espaces localement convexes la prop. 2 de TG, IX, p. 24.

#### Proposition 11 {#evt-ii-s4-prop-11 .statement}

Soit E un espace localement convexe métrisable. Il existe dans E une distance invariante par translation, définissant la topologie de E, et pour laquelle les boules ouvertes soient convexes.

Soit $(p_n)_{n \in \mathbf{N}}$ une suite de semi-normes définissant la topologie de E. Soit $d_n$ l’écart sur E défini par $d_n(x, y) = \inf(p_n(x - y), 1/n)$ pour $x, y$ dans E ; il est invariant par translation. Pour tout entier $n \geq 0$ et tout nombre réel $R \geq 0$, soit $B_{n,R}$ l’ensemble des $x \in E$ tels que $d_n(x, 0) < R$. Si $R \geq 1/n$, on a $B_{n,R} = E$, et dans le cas contraire, $B_{n,R}$ se compose des $x \in E$ tels que $p_n(x) < R$ ; dans tous les cas, l’ensemble $B_{n,R}$ est convexe.

Pour $x, y$ dans E, posons $d(x, y) = \sup_{n \in \mathbf{N}} d_n(x, y)$. On voit aussitôt que $d$ est une distance invariante par translation sur E, définissant sa topologie. Soient $x_0 \in E$ et $R \geq 0$ ; la boule ouverte de centre $x_0$ et de rayon R (pour la distance $d$) est égale à $\bigcap_{n \in \mathbf{N}} (x_0 + B_{n,R})$, donc elle est convexe.

#### Proposition 12 {#evt-ii-s4-prop-12 .statement}

Soient E et F des espaces de Fréchet et u une application linéaire continue de E sur F. Il existe une section continue, non nécessairement linéaire, de u.

Soit $d$ une distance sur E, définissant la topologie de E, invariante par translation, et dont les boules ouvertes soient convexes (prop. 11). Étant donnés $y$ et $y'$ dans F, soit $\delta(y, y')$ la distance des deux ensembles fermés $u^{-1}(y)$ et $u^{-1}(y')$ dans E. Comme $u$ est un morphisme strict (I, p. 17, th. 1), la remarque de TG, IX, p. 27 montre que $\delta$ est une distance sur F, définissant la topologie de F. Nous allons construire par récurrence une suite $(s_n)_{n \in \mathbf{N}}$ d’applications continues de F dans E satisfaisant aux inégalités suivantes pour tout $y \in F$ :

(2) $$
\delta(y, u(s_n(y))) < 2^{-n}
$$

(3) $$
d(s_n(y), s_{n-1}(y)) < 2^{-n+1} \quad (\text{seulement si } n \geq 1)
$$

Supposons que l’on ait $n = 0$, ou bien $n \geqslant 1$ mais que $s_{n-1}$ soit déjà construite. Soit $y_0 \in F$; comme $u$ est surjective, l’ensemble $u^{-1}(y_0)$ est non vide et, pour $n \geqslant 1$, on a $d(u^{-1}(y_0), s_{n-1}(y_0)) < 2^{-n+1}$ d’après l’hypothèse de récurrence. Il existe donc un point $x_0$ de $E$ tel que $u(x_0) = y_0$ et que, pour $n \geqslant 1$, $d(x_0, s_{n-1}(y_0)) < 2^{-n+1}$. Comme l’application $s_{n-1}$ est continue, l’ensemble des points $y$ de $F$ satisfaisant aux inégalités $\delta(y, y_0) < 2^{-n}$ et $d(x_0, s_{n-1}(y)) < 2^{-n+1}$ est un voisinage ouvert de $y_0$. Il existe donc un recouvrement ouvert $(V_i)_{i \in I}$ de $F$, et des applications constantes $s_{n,i}$ de $F$ dans $E$ qui satisfont *dans* $V_i$ aux inégalités (2) et (3) où l’on remplace $s_n$ par $s_{n,i}$. Comme l’espace $F$ est métrisable, il existe une partition continue de l’unité $(f_i)_{i \in I}$, localement finie et subordonnée au recouvrement $(V_i)_{i \in I}$ (TG, IX, p. 51, prop. 6 et p. 46, prop. 3). Pour tout $y \in F$, posons $s_n(y) = \sum_{i \in I} f_i(y) \cdot s_{n,i}(y)$. L’application $s_n$ de $F$ dans $E$ est continue ; comme les boules ouvertes sont convexes dans $E$ et dans $F$, l’application $s_n$ satisfait aux inégalités (2) et (3) pour tout $y \in F$.

Les applications $s_n : F \to E$ forment une suite de Cauchy pour la convergence uniforme d’après l’inégalité (3). Comme $E$ est complet, la suite $(s_n)_{n \in \mathbf{N}}$ converge uniformément vers une application continue $s : F \to E$ (TG, X, p. 9) ; la formule (2) montre que $u \circ s$ est l’application identique de $F$, donc $s$ est une section continue de $u$.

#### Corollaire {#evt-ii-s4-n7-cor-1 .statement}

*Si $L$ est une partie compacte de $F$, il existe une partie compacte $K$ de $E$ telle que $u(K) = L$.* Il suffit de poser $K = s(L)$, où $s$ est une section continue de $u$.

#### Remarque 1 {#evt-ii-s4-n7-rem-1 .statement}

Le corollaire de la prop. 12 peut aussi se déduire du th. 1 de I, p. 17 et de la prop. 18 de TG, IX, p. 22.
2) Conservons les notations de la prop. 12. Soit $p$ une semi-norme continue sur $E$ ; pour tout $y \in F$, posons $q(y) = \inf_{u(x) = y} p(x)$, de sorte que $q$ est une semi-norme continue sur $F$ (II, p. 4). Soit $\varphi$ une application semi-continue inférieurement de $F$ dans l’intervalle $]0, +\infty[$ de $\overline{\mathbf{R}}$. Montrons qu’il existe une section continue $s$ de $u$ telle que $p \circ s < q + \varphi$.

Soient $s_0$ une section continue de $u$ (prop. 12) et $N$ le noyau de $u$. Soit $y_0 \in F$; il existe $z_0 \in N$ tel que $p(s_0(y_0) + z_0) < q(y_0) + \varphi(y_0)$. Il existe un voisinage ouvert $W$ de $y_0$ dans $F$ tel que $p(s_0(y) + z_0) < q(y) + \varphi(y)$ pour tout $y \in W$. Par suite, il existe un recouvrement ouvert $(W_i)_{i \in I}$ de $F$ et des applications constantes $t_i : F \to N$ telles que $p(s_0(y) + t_i(y)) < q(y) + \varphi(y)$ pour tout $y \in W_i$. Comme $F$ est métrisable, il existe une partition continue localement finie de l’unité subordonnée au recouvrement $(W_i)_{i \in I}$, soit $(g_i)_{i \in I}$ (TG, IX, p. 51, prop. 6 et p. 46, prop. 3). L’application $s$ de $F$ dans $E$ définie par $s(y) = s_0(y) + \sum_{i \in I} g_i(y) \cdot t_i(y)$ répond aux conditions exigées.

## EXERCICES {#evt-ii-s4-exercises}

See the [exercises for § 4](exercises/s4/).
