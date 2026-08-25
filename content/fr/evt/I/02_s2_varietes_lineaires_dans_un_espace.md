---
book: evt
book_title: Topological Vector Spaces
chapter: I
chapter_title: Espaces vectoriels topologiques sur un corps valué
section: 2
section_title: Variétés linéaires dans un espace vectoriel topologique
lang: fr
source: evt-i-v-fr
book_pages: EVT I.11-EVT I.16, EVT I.25-EVT I.28
pdf_pages: 0017-0022, 0031-0034
extraction: ocr
subsections:
    - "no": 1
      title: Adhérence d’une variété linéaire
      page: 11
      pdf_page: 17
    - "no": 2
      title: Droites et hyperplans fermés
      page: 13
      pdf_page: 19
    - "no": 3
      title: Sous-espaces vectoriels de dimension finie
      page: 14
      pdf_page: 20
    - "no": 4
      title: Espaces vectoriels topologiques localement compacts
      page: 15
      pdf_page: 21
statements: 27
exercises: 15
content_sha256: 17282e590bb755f6fa41762cabf7db35892d4909a26cc70d7142e328f29ef6d1
---

## § 2. VARIÉTÉS LINÉAIRES DANS UN ESPACE VECTORIEL TOPOLOGIQUE

### 1. Adhérence d’une variété linéaire

Rappelons (A, II, p. 128) que, dans un espace vectoriel E sur un corps K, une variété linéaire affine (appelée simplement « variété linéaire » quand il n’en résulte pas de confusion) est la transformée par une translation quelconque d’un sous-espace vectoriel de E.

#### Proposition 1 {#evt-i-s2-prop-1 .statement}

*Dans un espace vectoriel topologique E, l’adhérence d’une variété linéaire est une variété linéaire.*

En effet, toute translation étant un homéomorphisme de E, il suffit de démontrer la proposition pour un sous-espace vectoriel M de E, et dans ce cas, la proposition a été vue dans I, p. 4.

#### Corollaire {#evt-i-s2-n1-cor-1 .statement}

*Dans un espace vectoriel topologique E, tout hyperplan est fermé ou partout dense.*

En effet, l’adhérence d’un hyperplan homogène H ne peut être que H ou l’espace E tout entier, puisque c’est un sous-espace vectoriel contenant H (prop. 1).

On voit donc que, pour qu’un hyperplan H soit fermé dans E, il faut et il suffit que $\mathbf{C} \subset H$ contienne un point intérieur.

Étant donnée une partie A d’un espace vectoriel topologique E, rappelons que le sous-espace vectoriel M engendré par A est l’ensemble des combinaisons linéaires des éléments de A (A, II, p. 16, prop. 9) ; l’adhérence de M dans E est, en vertu de la prop. 1, le plus petit sous-espace vectoriel fermé contenant A ; on dit que c’est le sous-espace vectoriel fermé engendré par A.

#### Définition 1 {#evt-i-s2-def-1 .statement}

Dans un espace vectoriel topologique E, on dit qu’un ensemble A est total si le sous-espace vectoriel fermé engendré par A est identique à E (ou, en d’autres termes, si l’ensemble des combinaisons linéaires d’éléments de A est partout dense).

#### Exemple 1 {#evt-i-s2-n1-exa-1 .statement}

Dans l’espace normé $\mathcal{C}(I ; \mathbf{C})$ (sur le corps $\mathbf{C}$) des fonctions continues dans $I = \{0, 1\}$, à valeurs dans $\mathbf{C}$, les restrictions à I des monômes $x^n$ ($n \in \mathbf{N}$) forment un ensemble total, en vertu du th. de Weierstrass-Stone (TG, X, p. 36, th. 3). De même dans le sous-espace P de $\mathcal{C}(I ; \mathbf{C})$ formé des fonctions telles que $f(0) = f(1)$, les restrictions à I des fonctions $e^{2n\pi ix}$ ($n \in \mathbf{Z}$) forment un ensemble total (TG, X, p. 40, prop. 8).

#### Exemple 2 {#evt-i-s2-n1-exa-2 .statement}

Tout ensemble absorbant dans un espace vectoriel topologique E sur un corps valué non discret (et en particulier tout voisinage de 0 dans E) est un ensemble total puisqu’il engendre E (I, p. 7). On déduit de là qu’une variété linéaire qui n’est pas dense dans E est nécessairement un ensemble rare dans E (TG, IX, p. 52), puisque son adhérence ne peut contenir de point intérieur.

#### Définition 2 {#evt-i-s2-def-2 .statement}

Dans un espace vectoriel topologique E, on dit qu’une famille $(a_\iota)_{\iota \in I}$ de points de E est topologiquement libre si, quel que soit $\kappa \in I$, le sous-espace vectoriel fermé engendré par les $a_\iota$ d’indice $\iota \neq \kappa$ ne contient pas $a_\kappa$.

#### Exemple 3 {#evt-i-s2-n1-exa-3 .statement}

Dans l’espace normé $\mathcal{C}(I ; \mathbf{C})$ des fonctions continues dans $I = \{0, 1\}$, les restrictions à I des fonctions $e^{2n\pi ix}$ ($n \in \mathbf{Z}$) forment une famille topologiquement libre. En effet, pour tout $n \in \mathbf{Z}$, si $f(x)$ est une combinaison linéaire $\sum_{k \neq n} c_k e^{2k\pi ix}$ (les $c_k$ étant nuls sauf un nombre fini d’entre eux), on a
$$
\int_0^1 |e^{2n\pi ix} - f(x)|^2 \, dx = 1 + \sum_{k \neq n} |c_k|^2 \geq 1
$$
et a fortiori, en vertu du th. de la moyenne
$$
\sup_{x \in I} |e^{2n\pi ix} - f(x)| \geq 1
$$
ce qui prouve que $e^{2n\pi ix}$ n’appartient pas au sous-espace vectoriel fermé de $\mathcal{C}(I ; \mathbf{C})$ engendré par les $e^{2k\pi ix}$ d’indice $k \neq n$.

L’ensemble des éléments d’une famille topologiquement libre est appelé partie topologiquement libre de E. Toute partie d’une partie topologiquement libre est topologiquement libre ; toute partie réduite à un point $x \neq 0$ est topologiquement libre si l’espace E est séparé.

Une famille topologiquement libre est libre (au sens algébrique ; cf. A, II, p. 96, Remarque) ; mais la réciproque est inexacte.

#### Exemple 4 {#evt-i-s2-n1-exa-4 .statement}

Dans l’espace normé $\mathcal{C}(I ; \mathbf{C})$ des fonctions continues dans $I = \{0, 1\}$, les restrictions à I des monômes $x^n$ ($n \in \mathbf{N}$) forment une famille libre au sens algébrique. Mais il existe une suite $(p_n)$ de polynômes telle que $p_n(x^2)$ converge uniformément vers x dans I (TG, X, p. 36, lemme 2), ce qui signifie que x appartient au sous-espace vectoriel fermé de $\mathcal{C}(I ; \mathbf{C})$ engendré par les monômes $x^{2^n}$ ($n \in \mathbf{N}$).

#### Remarque 1 {#evt-i-s2-n1-rem-1 .statement}

Contrairement à ce qui se passe en Algèbre pour les parties libres d’un espace vectoriel, l’ensemble des parties topologiquement libres d’un espace vectoriel topologique E n’est pas inductif en général pour la relation d’inclusion (I, p. 25, exerc. 2) ; en outre, il n’existe pas nécessairement dans E de partie topologiquement libre maximale (I, p. 25, exerc. 4), donc il n’existe pas nécessairement de partie topologiquement libre qui soit en même temps totale.

#### Remarque 2 {#evt-i-s2-n1-rem-2 .statement}

Soient M un sous-espace vectoriel fermé de E, et $(\dot{a}_i)_{i \in I}$ une famille topologiquement libre dans l’espace quotient $E/M$. Si $a_i$ est un élément quelconque de la classe $\dot{a}_i$, la famille $(a_i)_{i \in I}$ est topologiquement libre, comme il résulte de la déf. 2 et du fait que l’application canonique de E sur $E/M$ est continue. Mais on notera que si N est le sous-espace vectoriel fermé engendré par les $a_i$, on peut avoir $M \cap N \neq \{0\}$ (I, p. 25, exerc. 2) et par suite la somme $M + N$ n’est pas nécessairement directe au sens algébrique (ni *a fortiori* au sens topologique).

### 2. Droites et hyperplans fermés

#### Proposition 2 {#evt-i-s2-prop-2 .statement}

*Tout espace vectoriel topologique séparé E de dimension 1 sur un corps valué non discret K est isomorphe à $K_s$; de façon précise, pour tout $a \neq 0$ dans E, l’application $\xi \mapsto \xi a$ de $K_s$ sur E est un isomorphisme* (autrement dit, toute application linéaire de $K_s$ sur E est un isomorphisme).

Comme l’application $\xi \mapsto \xi a$ de $K_s$ sur E est bijective et continue (I, p. 1, déf. 1), il suffit de prouver qu’elle est bicontinue. Soit $\alpha$ un nombre réel $> 0$; on va montrer qu’il existe un voisinage V de 0 dans E tel que la relation $\xi a \in V$ entraîne $|\xi| < \alpha$. Comme K n’est pas discret, il existe un élément $\xi_0 \in K$ tel que $0 < |\xi_0| < \alpha$; d’autre part, E étant séparé, il existe dans E un voisinage V de 0 ne contenant pas $\xi_0 a$, et on peut supposer V équilibré (I, p. 7, prop. 4). Montrons que la relation $\xi a \in V$ entraîne $|\xi| < |\xi_0|$; sinon, on aurait $|\xi_0 \xi^{-1}| \leq 1$, donc $\xi_0 a = (\xi_0 \xi^{-1}) (\xi a) \in V$, contrairement à l’hypothèse, ce qui achève la démonstration.

#### Corollaire 1 {#evt-i-s2-prop-2-cor-1 .statement}

*Dans un espace vectoriel topologique séparé E sur un corps valué non discret K, tout sous-espace vectoriel D de dimension 1 est isomorphe à $K_s$*.

#### Corollaire 2 {#evt-i-s2-prop-2-cor-2 .statement}

*Soit E un espace vectoriel topologique sur un corps valué non discret. Tout sous-espace vectoriel D (de dimension 1) supplémentaire algébrique d’un hyperplan homogène fermé H est supplémentaire topologique de H*.

En effet, dans D, l’ensemble réduit à 0 est fermé, étant l’intersection de D et de l’ensemble fermé H ; D est donc séparé. Mais comme E/H est aussi séparé, l’application canonique de D sur E/H, qui est linéaire, est un isomorphisme en vertu de la prop. 2, d’où la conclusion (TG, III, p. 47).

#### Théorème 1 {#evt-i-s2-thm-1 .statement}

*Soit E un espace vectoriel topologique sur un corps valué non discret. Soit H un hyperplan dans E, défini par une équation $f(x) = \alpha$, où f est une forme linéaire non identiquement nulle. Pour que H soit fermé dans E, il faut et il suffit que f soit continue*.

La condition est évidemment suffisante (TG, I, p. 9, th. 1); montrons qu’elle est nécessaire. On peut supposer que H est un hyperplan fermé homogène, d’équation $f(x) = 0$; l’espace quotient $E/H$ est alors un espace vectoriel topologique séparé de dimension 1 sur K. On peut écrire $f = g \circ \varphi$, où $\varphi$ est l’application canonique de E sur $E/H$, et g une application linéaire de $E/H$ sur $K_s$; d’après la prop. 2, g est continue, donc il en est de même de f.

#### Corollaire {#evt-i-s2-n2-cor-1 .statement}

Toute forme linéaire continue et non nulle sur E est un morphisme strict de E sur $K_s$.

#### Remarque {#evt-i-s2-n2-rem-1 .statement}

On peut donner des exemples d’espaces vectoriels topologiques normés sur un corps valué non discret et complet, dans lesquels toute forme linéaire continue est identiquement nulle (I, p. 25, exerc. 4) ; dans un tel espace, tout hyperplan est donc partout dense (I, p. 11, corollaire).

### 3. Sous-espaces vectoriels de dimension finie

#### Théorème 2 {#evt-i-s2-thm-2 .statement}

Tout espace vectoriel topologique séparé E de dimension finie n sur un corps valué complet et non discret K, est isomorphe à $K_s^n$; de façon précise, pour toute base $(e_i)_{1 \leq i \leq n}$ de E sur K, l’application linéaire $(\xi_i) \mapsto \sum_{i=1}^n \xi_i e_i$ est un isomorphisme de $K_s^n$ sur E.

La prop. 2 de I, p. 13, entraîne que le th. 2 est vrai pour $n = 1$; raisonnons par récurrence sur n. Soit H le sous-espace vectoriel de E engendré par $e_1, e_2, \ldots, e_{n-1}$; l’hypothèse de récurrence montre que l’application $(\xi_i)_{1 \leq i \leq n-1} \mapsto \sum_{i=1}^{n-1} \xi_i e_i$ est un isomorphisme de $K_s^{n-1}$ sur H. Le sous-espace H, isomorphe à un produit d’espaces complets, est complet (TG, II, p. 17, prop. 10) ; par suite, il est fermé dans E (TG, II, p. 16, prop. 8). Soit D le sous-espace Ke_n supplémentaire de H dans E ; E est somme directe topologique de H et de D (I, p. 13, cor. 2), donc l’application

$$
(\xi_i)_{1 \leq i \leq n} \mapsto \sum_{i=1}^n \xi_i e_i \text{ de } K_s^{n-1} \times K_s
$$

sur E est un isomorphisme.

L’hypothèse que K est complet est essentielle pour la validité du th. 2 dès que $n > 1$. En effet, soit K un corps valué non complet, et soit $\hat{K}$ son complété : pour tout élément $a \neq 0$ de $\hat{K}$, $K.a$ est partout dense dans $\hat{K}$, puisque $x \mapsto xa$ est un homéomorphisme de $\hat{K}$ sur lui-même. Si $a \notin K$, le sous-espace $K + Ka$ de l’espace vectoriel topologique $\hat{K}$ sur K, est de dimension 2 sur K, mais il n’est pas isomorphe à $K_s^2$, puisque tout sous-espace de dimension 1 dans $K + Ka$ est dense dans $K + Ka$.

#### Corollaire 1 {#evt-i-s2-thm-2-cor-1 .statement}

Dans un espace vectoriel topologique séparé E sur un corps valué complet et non discret K, tout sous-espace vectoriel F de dimension finie est fermé dans E.

En effet, si F est de dimension n, il est isomorphe à $K_s^n$, donc complet, et par suite fermé dans E (TG, II, p. 16, prop. 8).

#### Corollaire 2 {#evt-i-s2-thm-2-cor-2 .statement}

Soient K un corps valué complet et non discret, E un espace vectoriel topologique séparé de dimension finie sur K, F un espace vectoriel topologique quelconque sur K ; toute application linéaire de E dans F est continue.

#### Corollaire 3 {#evt-i-s2-thm-2-cor-3 .statement}

Dans un espace vectoriel topologique séparé E sur un corps valué complet et non discret, toute partie libre finie est topologiquement libre.

#### Corollaire 4 {#evt-i-s2-thm-2-cor-4 .statement}

*Soit E un espace vectoriel topologique sur un corps valué complet non discret. Soient M un sous-espace vectoriel fermé de E, F un sous-espace vectoriel de dimension finie de E ; le sous-espace M + F est fermé dans E.*

En effet, l’espace quotient E/M est séparé ; soit $\varphi$ l’homomorphisme canonique de E sur E/M ; le sous-espace M + F est égal à $\varphi^{-1}(\varphi(F))$. Or, $\varphi(F)$ est de dimension finie dans E/M, donc (cor. 1) $\varphi(F)$ est fermé dans E/M, et par suite $\varphi^{-1}(\varphi(F))$ est fermé dans E.

On observera que, si M et N sont deux sous-espaces vectoriels fermés quelconques dans un espace vectoriel topologique séparé E, M + N n’est pas nécessairement fermé dans E, \* même si E est un espace hilbertien \* (cf. IV, p. 64, exerc. 13 d)).

#### Proposition 3 {#evt-i-s2-prop-3 .statement}

*Soit E un espace vectoriel topologique sur un corps valué complet et non discret K. Soit M un sous-espace vectoriel fermé de codimension finie n dans E. Tout sous-espace N supplémentaire algébrique de M dans E est supplémentaire topologique de M.*

En effet, dans N, l’ensemble réduit à 0 est fermé, étant l’intersection de N et de l’ensemble M fermé dans E ; N est donc séparé. Comme E/M est aussi séparé, l’application canonique de N sur E/M, qui est linéaire et bijective, est bicontinue (I, p. 14, cor. 2), d’où la proposition.

#### Corollaire {#evt-i-s2-n3-cor-1 .statement}

*Soient E et F deux espaces vectoriels topologiques sur un corps valué complet et non discret. Si F est séparé et de dimension finie, toute application linéaire continue de E sur F est un morphisme strict.*

#### Remarque {#evt-i-s2-n3-rem-1 .statement}

Les résultats des nos 2 et 3 ne sont plus valables lorsque K est *discret*. Par exemple, soit $K_1$ un corps valué non discret, et soit K le corps discret obtenu en munissant $K_1$ de la valeur absolue impropre ; $K_1$ est un espace vectoriel topologique de dimension 1 sur K, mais n’est pas isomorphe à $K_s$. Toutefois, on peut montrer que les résultats des nos 2 et 3 subsistent lorsque K est discret, pourvu qu’on impose aux espaces vectoriels topologiques considérés d’avoir un système fondamental de voisinages, *équilibrés* de 0 (c’est-à-dire ici de voisinages V tels que $K.V = V$) (I, p. 28, exerc. 14) ; cette condition (qui est toujours remplie lorsque K est un corps valué non discret, cf. I, p. 7, prop. 4) ne l’est plus ici pour tous les espaces vectoriels topologiques sur K, comme le montre l’exemple précédent.

### 4. Espaces vectoriels topologiques localement compacts

#### Théorème 3 {#evt-i-s2-thm-3 .statement}

*Soit K un corps valué complet non discret. Un espace vectoriel topologique séparé E sur K qui admet un voisinage de 0 précompact V est de dimension finie. Si E n’est pas réduit à 0, K et E sont alors localement compacts.*

Pour démontrer la première assertion, on peut se borner au cas où E est *complet*, car E est un sous-espace partout dense de son complété $\hat{E}$ et l’adhérence $\overline{V}$ de V dans $\hat{E}$ est compacte et est un voisinage de 0 dans $\hat{E}$ (TG, III, p. 24, prop. 7).

On peut donc supposer qu’il y a dans E un voisinage *compact* V de 0. Soit $\alpha \in K$ tel que $0 < |\alpha| < 1$ ; il y a donc des points $a_i \in V$ en nombre fini tels que

$$
V \subset \bigcup_i (a_i + \alpha V).
$$

Soit M le sous-espace (de dimension finie) de E engendré par les $a_i$; il est fermé dans E (I, p. 14, cor. 1); dans l’espace vectoriel topologique séparé E/M, l’image canonique de V est un voisinage compact W de 0 tel que $W \subset \alpha W$; ceci s’écrit encore $\alpha^{-1}W \subset W$, d’où par récurrence sur $n$, $\alpha^{-n}W \subset W$ pour tout entier positif $n$. Comme W est absorbant, on en déduit que $W = E/M$; autrement dit E/M est *compact*. Pour prouver la première assertion, il suffit donc de démontrer le lemme suivant :

#### Lemme 1 {#evt-i-s2-lem-1 .statement}

*Tout espace vectoriel topologique compact E sur un corps valué non discret est réduit à 0*.

En effet, comme E est complet, on peut supposer qu’il en est de même de K (I, p. 6). Si E n’était pas réduit à 0, il contiendrait une droite, fermée dans E, donc compacte, et isomorphe à $K_s$ (I, p. 14, cor. 1 et I, p. 13, prop. 2), et par suite K serait compact ; mais cela est absurde, car l’application $\xi \mapsto |\xi|$ de K dans $\mathbf{R}$ est continue, donc serait bornée, alors qu’il existe des $\gamma \in K$ tels que $|\gamma| > 1$, donc tels que $|\gamma^n| = |\gamma|^n$ soit arbitrairement grand.

Revenant au th. 3, on voit que si E admet un voisinage de 0 précompact et n’est pas réduit à 0, E est de dimension finie sur K, donc isomorphe à un espace $K_s^n$ avec $n > 0$; comme K est complet, il en est de même de E, qui est donc localement compact. Puisque $K_s$ est isomorphe à une droite de E (I, p. 13, prop. 2), nécessairement fermée dans E (I, p. 14, cor. 1), K est localement compact.

#### Remarque {#evt-i-s2-n4-rem-1 .statement}

La conclusion du th. 3 ne subsiste plus lorsque K est un corps discret, comme le montre l’exemple de $\mathbf{R}$ (muni de la topologie usuelle) considéré comme espace vectoriel topologique sur le corps $\mathbf{Q}$ discret.

## EXERCICES {#evt-i-s2-exercises}

See the [exercises for § 2](exercises/s2/).
