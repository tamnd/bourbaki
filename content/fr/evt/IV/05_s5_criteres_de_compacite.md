---
book: evt
book_title: Topological Vector Spaces
chapter: IV
chapter_title: LA DUALITÉ DANS LES ESPACES VECTORIELS TOPOLOGIQUES
section: 5
section_title: Critères de compacité
lang: fr
source: evt-i-v-fr
book_pages: EVT IV.32-EVT IV.38, EVT IV.67-EVT IV.72
pdf_pages: 0218-0224, 0253-0258
extraction: ocr
subsections:
    - "no": 1
      title: Remarques générales
      page: 32
      pdf_page: 218
    - "no": 2
      title: Compacité simple des ensembles de fonctions continues
      page: 33
      pdf_page: 219
    - "no": 3
      title: Les théorèmes d’Eberlein et de Šmulian
      page: 35
      pdf_page: 221
    - "no": 4
      title: Cas des espaces de fonctions continues bornées
      page: 36
      pdf_page: 222
    - "no": 5
      title: Enveloppe convexe d’un ensemble faiblement compact
      page: 37
      pdf_page: 223
statements: 9
exercises: 18
content_sha256: 9873ff7226898a8c69fd60eeea44e8d751f30d44dbd066dbc07879165c475aa5
---

## § 5. CRITÈRES DE COMPACITÉ

### 1. Remarques générales

Soit A une partie d’un espace topologique E. Pour qu’une suite $(x_n)_{n \in \mathbf{N}}$ de points de A ait pour valeur d’adhérence un point $x$ de E, il faut et il suffit que la condition suivante soit satisfaite (TG, I, p. 48) :

(A) *Quels que soient l’entier $m \geq 0$ et le voisinage U de $x$, il existe un entier $n \geq m$ tel que $x_n \in U$*.

On appelle suite *extraite* de la suite $(x_n)_{n \in \mathbf{N}}$ toute suite de la forme $(y_k)_{k \in \mathbf{N}}$ avec $y_k = x_{n_k}$ pour une suite strictement croissante $(n_k)_{k \in \mathbf{N}}$ d’entiers positifs. S’il existe une suite extraite de la suite $(x_n)_{n \in \mathbf{N}}$ et convergeant vers $x$, alors $x$ est valeur d’adhérence de $(x_n)$; réciproquement, si $x$ admet un système fondamental *dénombrable* de voisinages, et que $x$ est valeur d’adhérence de la suite $(x_n)$, alors il existe une suite extraite de $(x_n)$ et convergeant vers $x$.

Compte tenu de TG, IX, p. 20, corollaire, on en conclut que, lorsque E est *métrisable*, les conditions suivantes sont équivalentes :

a) *l’ensemble A est relativement compact dans E* ;
b) *toute suite infinie de points de A a une valeur d’adhérence dans E* ;
c) *de toute suite infinie de points de A, on peut extraire une suite qui converge vers un point de E*.

Nous étendrons, dans ce paragraphe, ce critère à certains espaces vectoriels topologiques *non métrisables*. La proposition suivante permet dans de nombreux cas de ramener l’étude des ensembles compacts à celle des ensembles faiblement compacts.

#### Proposition 1 {#evt-iv-s5-prop-1 .statement}

*Soient E un espace localement convexe séparé et A une partie de E. On note $E_\sigma$ l’espace E muni de la topologie affaiblie.*

a) *Si toute suite infinie de points de A a une valeur d’adhérence dans E, alors A est précompacte dans E*.

b) *Pour que A soit relativement compacte dans E, il faut et il suffit qu’elle soit précompacte dans E et relativement compacte dans $E_\sigma$*.

Prouvons a) par l’absurde. Si A n’est pas précompacte, il résulte du th. 3 de TG, II, p. 29, qu’il existe un voisinage convexe symétrique V de 0 dans E tel que A ne possède aucun recouvrement fini par des translatés de V. Autrement dit, si $x_0, x_1, \ldots, x_{n-1}$ sont des points de A, on a $A \notin \bigcup_{0 \leq i < n} (x_i + V)$ et il existe donc un point $x_n$ de A tel que $x_n - x_i \notin V$ pour $0 \leq i < n$. On peut alors construire par récurrence une suite infinie $(x_n)_{n \in \mathbf{N}}$ de points de A telle que $x_n - x_m \notin V$ lorsque $n > m$; comme V est symétrique, on a aussi $x_m - x_n \notin V$ pour $m \neq n$ et les ensembles $x_n + \frac{1}{2}V$ sont deux à deux disjoints. Pour tout point $x$ de E, il existe au plus un entier $n \geq 0$ tel que $x_n \in x + \frac{1}{2}V$, donc la suite $(x_n)_{n \in \mathbf{N}}$ n’a aucune valeur d’adhérence. D’où a).

Supposons que A soit précompacte dans E et contenue dans une partie compacte B de $E_\sigma$. Alors B est complète dans $E_\sigma$, donc *dans* E (IV, p. 5, *Remarque* 2). On a $\overline{A} \subset B$, donc A est relativement compacte dans E. La réciproque est évidente, d’où *b*).

### 2. Compacité simple des ensembles de fonctions continues

Dans ce numéro, on note X un espace *compact* et $\mathcal{C}_s(X)$ l’espace des fonctions continues sur X, à valeurs dans le corps K (égal à $\mathbf{R}$ ou $\mathbf{C}$), muni de la topologie de la convergence simple dans X.

#### Proposition 2 {#evt-iv-s5-prop-2 .statement}

*Soient D une partie dense de X et A une partie de l’espace $\mathcal{C}_s(X)$. Les conditions suivantes sont équivalentes :*
(i) *A est relativement compacte dans $\mathcal{C}_s(X)$.*
(ii) *De toute suite infinie d’éléments de A, on peut extraire une suite convergeant dans $\mathcal{C}_s(X)$.*
(iii) *Toute suite infinie d’éléments de A a une valeur d’adhérence dans $\mathcal{C}_s(X)$.*
(iv) *Soient $(f_n)_{n \in \mathbf{N}}$ une suite de fonctions appartenant à A et $(x_m)_{m \in \mathbf{N}}$ une suite de points de D. Si les limites itérées*

$$
\gamma = \lim_{m \to \infty} \lim_{n \to \infty} f_n(x_m), \quad \delta = \lim_{n \to \infty} \lim_{m \to \infty} f_n(x_m)
$$

*existent, elles sont égales. De plus, on a* $\sup_{f \in A} |f(x)| < +\infty$ *pour tout* $x \in X$.

(i) $\Rightarrow$ (ii) : soit $\overline{A}$ l’adhérence de A dans $\mathcal{C}_s(X)$. Supposons que $\overline{A}$ soit compacte, et considérons une suite de fonctions $f_n \in A$ (pour $n \in \mathbf{N}$). Soit $\varphi$ l’application continue $x \mapsto (f_n(x))_{n \in \mathbf{N}}$ de X dans l’espace métrisable $K^\mathbf{N}$. L’image $X'$ de X par $\varphi$ est un espace compact métrisable, puisque X est compact. Soit E le sous-espace fermé de $\mathcal{C}_s(X)$ formé des fonctions continues $f$ sur X telles que la relation $\varphi(x) = \varphi(y)$ entraîne $f(x) = f(y)$ pour tout couple de points $x, y$ de X. D’après le cor. 2 de TG, I, p. 63 et la prop. 3 de TG, I, p. 32, l’application $f' \mapsto f' \circ \varphi$ est un homéomorphisme $\varphi^*$ de $\mathcal{C}_s(X')$ sur E. L’ensemble $A' = (\varphi^*)^{-1}(\overline{A})$ est donc compact dans $\mathcal{C}_s(X')$, et il est clair qu’il existe des éléments $f'_n$ de $A'$ tels que $\varphi^*(f'_n) = f'_n \circ \varphi$ soit égal à $f_n$.

Comme $X'$ est un espace compact métrisable, il existe dans $X'$ une partie dénombrable dense $D'$ (TG, IX, p. 18, prop. 12, et p. 21, prop. 16). Soit $\mathcal{T}_1$ (resp. $\mathcal{T}_2$) la topologie sur $A'$ induite par la topologie de la convergence simple dans $D'$ (resp. $X'$). Alors $\mathcal{T}_1$ est métrisable, $\mathcal{T}_2$ est compacte et plus fine que $\mathcal{T}_1$, donc $\mathcal{T}_1$ et $\mathcal{T}_2$ coïncident ; autrement dit, $A'$ est un sous-espace compact *métrisable* de $\mathcal{C}_s(X')$. Il existe donc une suite $(f'_{n_k})$ extraite de $(f'_n)$ et convergeant vers un élément $f'$ de $\mathcal{C}_s(X')$. La suite $(f_{n_k})$ converge alors vers $f = f' \circ \varphi$ dans $\mathcal{C}_s(X)$.

(ii) $\Rightarrow$ (iii) : c’est clair.

(iii) ⇒ (iv) : supposons que toute suite infinie d’éléments de A ait une valeur d’adhérence dans $\mathcal{C}_s(X)$. Soit $x \in X$. L’application $\varphi_x : f \mapsto f(x)$ de A dans K est continue. Par suite, dans $\varphi_x(A)$, toute suite infinie admet une valeur d’adhérence ; comme le corps K (égal à $\mathbf{R}$ ou $\mathbf{C}$) est métrisable, l’ensemble $\varphi_x(A)$ est relativement compact dans K, donc borné. Autrement dit, on a $\sup_{f \in A} |f(x)| < +\infty$.

Soient $f_n, x_m, \gamma$ et $\delta$ comme dans (iv). Soit $f$ une valeur d’adhérence de la suite $(f_n)$ dans $\mathcal{C}_s(X)$, et soit $x$ une valeur d’adhérence de la suite $(x_m)$ dans l’espace compact X. Pour tout $m$, l’application $h \mapsto h(x_m)$ de $\mathcal{C}_s(X)$ dans K est continue. Vu les hypothèses faites, on a donc $f(x_m) = \lim_{n \to \infty} f_n(x_m)$, d’où $\gamma = \lim_{m \to \infty} f(x_m)$; comme $f : X \to K$ est continue, et que $x$ est une valeur d’adhérence de la suite $(x_m)$, on a $\gamma = f(x)$. On prouve de manière analogue l’égalité $\delta = f(x)$, d’où $\gamma = \delta$.

(iv) ⇒ (i) : supposons que l’ensemble des nombres $f(x)$, pour $f$ parcourant A, soit borné dans K pour tout $x \in X$. Il revient au même de supposer que l’adhérence $\overline{A}$ de A dans l’espace produit $K^X$ est compacte (TG, I, p. 64). Supposons que A ne soit pas relativement compacte dans $\mathcal{C}_s(X)$. Cela signifie qu’il existe une fonction $u \in \overline{A}$ et un point $a \in X$ tels que $u$ ne soit pas continue en $a$. Il existe alors un nombre réel $\varepsilon > 0$ tel que, dans tout voisinage U de $a$, il existe un point $x$ avec $|u(x) - u(a)| \geq \varepsilon$.

Nous allons construire par récurrence une suite $(x_n)_{n \in \mathbf{N}}$ de points de D et une suite $(f_n)_{n \in \mathbf{N}}$ d’éléments de A, satisfaisant aux relations suivantes :

$$
(1)_m \quad |u(x_m) - u(a)| \geq \varepsilon \quad \text{pour } m \geq 1;
$$

$$
(2)_m \quad |u(x_i) - f_m(x_i)| \leq \frac{1}{m+1} \quad \text{pour } 0 \leq i \leq m-1;
$$

$$
(3)_{m,i} \quad |f_m(x_i) - f_m(a)| \leq \frac{1}{i+1} \quad \text{pour } 0 \leq m \leq i.
$$

On prend $x_0 = a$ avec $f_0$ arbitraire dans A (l’ensemble A n’est pas vide, sinon il serait relativement compact dans $\mathcal{C}_s(X)$). Soient $n \geq 1$ et $x_0, x_1, \ldots, x_{n-1}$, $f_0, f_1, \ldots, f_{n-1}$ satisfaisant aux relations (1)_m, (2)_m pour $1 \leq m < n$ et (3)_{m,i} pour $0 \leq m \leq i < n$. Comme $u$ appartient à $\overline{A}$, il existe $f_n \in A$ satisfaisant à (2)_n. Soit $V_n$ l’ensemble des $x \in X$ tels que l’on ait $|f_m(x) - f_m(a)| \leq \frac{1}{n+1}$ pour $0 \leq m \leq n$. C’est un voisinage de $a$ car $f_n$ est continue ; choisissons un point $x_n$ de $D \cap V_n$ tel que $|u(x_n) - u(a)| \geq \varepsilon$, donc (1)_n et (3)_{m,n} sont satisfaites. La construction peut donc se poursuivre.

Comme $u(X)$ est une partie compacte de K, il existe une suite $(y_k)$ extraite de $(x_m)$ et telle que la limite $\gamma = \lim_{k \to \infty} u(y_k)$ existe. D’après (2)_m, on a $u(x_i) = \lim_{n \to \infty} f_n(x_i)$ pour tout $i \in \mathbf{N}$, d’où

(4) $$
\gamma = \lim_{k \to \infty} \lim_{n \to \infty} f_n(y_k).
$$

Par ailleurs, on a $f_n(a) = \lim_{i \to \infty} f_n(x_i)$ d’après (3)$_{m,i}$ d’où $f_n(a) = \lim_{k \to \infty} f_n(y_k)$. Comme $x_0 = a$, on déduit $\lim_{n \to \infty} f_n(a) = u(a)$ de (2)$_m$. Par suite, on a

$$
u(a) = \lim_{n \to \infty} \lim_{k \to \infty} f_n(y_k).
$$

Enfin, d’après (1)$_m$, on a $|\gamma - u(a)| \geq \varepsilon$, d’où $\gamma \neq u(a)$. Ceci contredit l’assertion (iv) ; on a donc prouvé par l’absurde que (iv) implique (i).

### 3. Les théorèmes d’Eberlein et de Šmulian

#### Théorème 1 (Eberlein) {#evt-iv-s5-thm-1 .statement}

Soient E un espace localement convexe séparé et quasi-complet, $\mathcal{T}$ une topologie sur E compatible avec la dualité entre E et E', et A une partie de E. Pour que A soit relativement compacte pour $\mathcal{T}$, il faut et il suffit que toute suite infinie de points de A ait une valeur d’adhérence dans E pour $\mathcal{T}$.

La condition énoncée est évidemment nécessaire.

Supposons que toute suite infinie de points de A ait une valeur d’adhérence pour $\mathcal{T}$, donc aussi pour la topologie moins fine $\sigma(E, E')$. Alors A est précompacte pour $\mathcal{T}$ (IV, p. 32, prop. 1); pour que A soit relativement compacte pour $\mathcal{T}$, il faut et il suffit qu’elle le soit pour $\sigma(E, E')$ (loc. cit.). Il suffit donc de prouver le théorème lorsque $\mathcal{T}$ est la topologie affaiblie $\sigma(E, E')$.

Notons $\hat{E}$ le complété de E, que l’on identifie comme d’habitude à un sous-espace du dual algébrique ${E'}^*$ de E' (III, p. 21, th. 2). On note $E_\sigma$, $\hat{E}_\sigma$ et $E'_\sigma$ les espaces E, $\hat{E}$ et ${E'}^*$ munis respectivement des topologies $\sigma(E, E')$, $\sigma(\hat{E}, E')$ et $\sigma({E'}^*, E')$.

Soit $(x'_i)_{i \in I}$ une base de l’espace vectoriel E' sur le corps K. L’application $f \mapsto (f(x'_i))_{i \in I}$ est un homéomorphisme $\varphi$ de $E'_\sigma$ sur $K^I$; pour tout $i \in I$, l’image de A par l’application $x'_i$ de E dans K est relativement compacte : en effet, K est métrisable et toute suite infinie d’éléments de $x'_i(A)$ a une valeur d’adhérence. On en déduit que $\varphi(A)$ est relativement compacte dans $K^I$, donc que l’adhérence $\overline{A}$ de A dans $E'_\sigma$ est compacte.

Prouvons que $\overline{A}$ est contenue dans $\hat{E}$. Soit H une partie équicontinue de E' ; soit X son adhérence pour $\sigma(E', E)$; elle est compacte (III, p. 17, cor. 2). Pour tout $x \in {E'}^*$, soit $\varphi_x$ la restriction de $x' \mapsto \langle x, x' \rangle$ à X ; soit $\tilde{A} \subset \mathscr{C}_s(X)$ l’ensemble des fonctions $\varphi_x$ pour $x$ parcourant A. Vu l’hypothèse faite sur A, toute suite infinie d’éléments de $\tilde{A}$ a une valeur d’adhérence dans $\mathscr{C}_s(X)$; d’après la prop. 2 (IV, p. 33), l’ensemble $\tilde{A}$ est donc relativement compact dans $\mathscr{C}_s(X)$. Il en résulte que pour tout $a \in \overline{A}$, la fonction $\varphi_a$ sur X est continue. L’inclusion $\overline{A} \subset \hat{E}$ résulte alors du th. 2 de III, p. 21.

Montrons maintenant que $\overline{A}$ est contenue dans E. Comme A est précompacte dans $E_\sigma$ (IV, p. 32, prop. 1), elle est bornée dans $E_\sigma$ (III, p. 3, prop. 2), donc aussi dans E (IV, p. 1, prop. 1). Soit C l’enveloppe fermée convexe équilibrée de A dans E. Elle est bornée puisque A est bornée, donc complète puisque E est quasi-complet. Autrement dit, C est une partie convexe et fermée de $\hat{E}$, donc de $\hat{E}_\sigma$ (IV, p. 1, prop. 1). Comme on a $A \subset C$ et que la topologie de $\hat{E}_\sigma$ est induite par celle de ${E'_\sigma}^*$, on a donc $\overline{A} \subset C$, d’où $\overline{A} \subset E$.

Comme la topologie de $E_\sigma$ est induite par celle de ${E'_\sigma}^*$, la partie $\overline{A}$ de $E_\sigma$ est compacte, d’où le th. 1.

#### Théorème 2 (Šmulian) {#evt-iv-s5-thm-2 .statement}

Soient $E$ un espace de Fréchet et $A$ une partie de $E$. On note $E_\sigma$ l’espace $E$ muni de la topologie affaiblie. Les conditions suivantes sont équivalentes :

(i) $A$ est relativement compacte dans $E_\sigma$;
(ii) toute suite infinie de points de $A$ a une valeur d’adhérence dans $E_\sigma$;
(iii) de toute suite infinie de points de $A$, on peut extraire une suite qui converge dans $E_\sigma$.

L’équivalence de (i) et (ii) résulte du th. d’Eberlein, et (iii) entraîne évidemment (ii).

Montrons que (i) entraîne (iii). Supposons donc que l’adhérence $B$ de $A$ dans $E_\sigma$ soit compacte et que $(x_n)_{n \in \mathbf{N}}$ soit une suite de points de $A$. Notons $F$ le plus petit sous-espace vectoriel fermé de $E$ contenant les $x_n$; c’est un espace de Fréchet de type dénombrable. Comme $F$ est fermé dans $E_\sigma$ et que la topologie $\sigma(F, F')$ sur $F$ est induite par $\sigma(E, E')$, l’ensemble $B \cap F$ est compact pour $\sigma(F, F')$. Compte tenu des remarques de IV, p. 32, l’existence d’une suite extraite de $(x_n)_{n \in \mathbf{N}}$ convergeant pour $\sigma(E, E')$ (ou $\sigma(F, F')$, cela revient au même) est conséquence du lemme suivant :

#### Lemme 1 {#evt-iv-s5-lem-1 .statement}

Soit $F$ un espace de Fréchet de type dénombrable. Toute partie $C$ de $F$ qui est compacte pour la topologie $\mathcal{T}$ induite par $\sigma(F, F')$ est métrisable pour cette topologie.

Comme sur $F'$ la topologie de la convergence précompacte est plus fine que la topologie $\sigma(F', F)$, il existe dans $F'_s$ une partie dénombrable partout dense $D$ (III, p. 19, cor. 1). L’ensemble $C$ s’identifie donc à une partie de $K^D$, et la topologie induite sur $C$ par celle de $K^D$, qui est métrisable (TG, IX, p. 19, corollaire) est moins fine que la topologie induite par $\sigma(F, F')$, pour laquelle $C$ est compacte. Ces deux topologies sont donc identiques (TG, I, p. 63, cor. 3). C.Q.F.D.

Le th. de Šmulian peut s’étendre au cas où $E$ est limite inductive stricte d’une suite d’espaces de Fréchet (IV, p. 67, exerc. 2).

### \*4. Cas des espaces de fonctions continues bornées

Pour tout espace topologique $X$, nous noterons $\mathscr{C}^b(X)$ l’espace de Banach des applications continues et *bornées* de $X$ dans $K$, avec la norme définie par

$$
\| f \| = \sup_{x \in X} |f(x)|
$$

(TG, X, p. 21). Lorsque $X$ est compact, toute fonction continue sur $X$ est bornée (TG, IV, p. 28), et l’on écrit $\mathscr{C}(X)$ pour $\mathscr{C}^b(X)$.

Dans ce numéro et le suivant, nous ferons usage du lemme suivant, qui est un cas particulier du th. de Lebesgue (INT, IV, 2e éd., § 4, n° 3, th. 2), compte tenu de l’interprétation des éléments de $\mathcal{C}(X)'$ comme des mesures sur X.

#### Lemme 2 {#evt-iv-s5-lem-2 .statement}

Soit X un espace compact. Si une suite $(f_n)_{n \in \mathbf{N}}$ est bornée dans $\mathcal{C}(X)$ et converge simplement sur X vers une fonction continue f, on a $\mu(f) = \lim_{n \to \infty} \mu(f_n)$ pour tout $\mu$ dans $\mathcal{C}(X)'$.

#### Proposition 3 {#evt-iv-s5-prop-3 .statement}

Soit X un espace compact, et soit A une partie bornée de $\mathcal{C}(X)$. Pour que A soit relativement compacte pour la topologie de la convergence simple, il faut et il suffit qu’elle soit relativement compacte pour $\sigma(\mathcal{C}(X), \mathcal{C}(X)')$.

La topologie de la convergence simple est séparée et moins fine que $\sigma(\mathcal{C}(X), \mathcal{C}(X)')$, donc la condition énoncée est suffisante (TG, I, p. 63, cor. 3).

Supposons maintenant que A soit relativement compacte pour la topologie de la convergence simple. Soit $(f_n)_{n \in \mathbf{N}}$ une suite d’éléments de A. D’après la prop. 2 (IV, p. 33), il existe une suite $(f_{n_k})$ extraite de $(f_n)$ et convergeant simplement vers une fonction continue f. D’après le lemme 2, la suite bornée $(f_{n_k})$ tend vers f pour $\sigma(\mathcal{C}(X), \mathcal{C}(X)')$. Le th. de Šmulian (IV, p. 36, th. 2) montre alors que A est relativement compacte pour $\sigma(\mathcal{C}(X), \mathcal{C}(X)')$.

#### Corollaire {#evt-iv-s5-n4-cor-1 .statement}

Soient S un espace topologique et A une partie bornée de $\mathcal{C}^b(S)$. Les conditions suivantes sont équivalentes :

(i) A est relativement compacte pour $\sigma(\mathcal{C}^b(S), \mathcal{C}^b(S)')$;
(ii) si $(f_n)_{n \in \mathbf{N}}$ est une suite d’éléments de A et $(x_m)_{m \in \mathbf{N}}$ une suite de points de S telles que les limites itérées

$$
\gamma = \lim_{m \to \infty} \lim_{n \to \infty} f_n(x_m), \quad \delta = \lim_{n \to \infty} \lim_{m \to \infty} f_n(x_m)
$$

existent, on a $\gamma = \delta$.

Soient X le compactifié de Stone-Čech de S (TG, IX, p. 10) et $\alpha$ l’application canonique de S dans X. Posons D = $\alpha(S)$. L’application $\varphi : f \mapsto f \circ \alpha$ est un isomorphisme de l’espace normé $\mathcal{C}(X)$ sur l’espace normé $\mathcal{C}^b(S)$; posons $\tilde{A} = \varphi^{-1}(A)$. Comme X est compact et D dense dans X, la prop. 2 (IV, p. 33) montre que la condition (ii) équivaut à la compacité de $\tilde{A}$ pour la topologie de la convergence simple. L’équivalence de (i) et (ii) résulte donc de la prop. 3. \*

### \*5. Enveloppe convexe d’un ensemble faiblement compact

#### Théorème 3 (Krein) {#evt-iv-s5-thm-3 .statement}

Soit E un espace localement convexe séparé et quasi-complet, et soit $\mathcal{T}$ une topologie sur E compatible avec la dualité entre E et E'. Soit A une partie de E compacte pour $\mathcal{T}$. Alors l’enveloppe fermée convexe équilibrée C de A est compacte pour $\mathcal{T}$.

Faisons d’abord plusieurs réductions.

A) L’ensemble C est précompact pour $\mathcal{T}$ (II, p. 27, prop. 3), et A est compact pour $\sigma(E, E')$. Compte tenu de la prop. 1 (IV, p. 32), il s’agit de prouver que C est compact pour $\sigma(E, E')$, ce qui nous ramène au cas où $\mathcal{T} = \sigma(E, E')$.

B) Comme C est précompact et fermé pour $\sigma(E, E')$, il est borné et fermé pour la topologie initiale de E (III, p. 3, prop. 2 et IV, p. 1, prop. 1); il est donc complet puisque E est quasi-complet. Autrement dit, C est l’enveloppe fermée convexe équilibrée de A dans le complété $\hat{E}$ de E. Comme la topologie $\sigma(\hat{E}, E')$ induit $\sigma(E, E')$ sur E, on est ramené au cas où E est complet.

C) Soit $\Gamma$ l’enveloppe convexe équilibrée de A. Alors C est l’adhérence de $\Gamma$ pour $\sigma(E, E')$. D’après le th. d’Eberlein (IV, p. 35, th. 1), il s’agit de prouver que toute suite $(x_n)_{n \in \mathbf{N}}$ de points de $\Gamma$ a une valeur d’adhérence pour $\sigma(E, E')$ dans E. Or $x_n$ appartient à l’enveloppe convexe équilibrée d’une partie finie $B_n$ de A. Soit F le sous-espace vectoriel fermé de E engendré par l’ensemble dénombrable $B = \bigcup_n B_n$. Alors F est complet, la topologie $\sigma(F, F')$ sur F est induite par $\sigma(E, E')$ et l’on a $x_n \in F$ pour tout $n \in \mathbf{N}$. Il suffit donc de prouver que $(x_n)_{n \in \mathbf{N}}$ a une valeur d’adhérence pour $\sigma(F, F')$, ce qui nous ramène au cas où il existe dans E une partie dénombrable dense.

Munissons A de la topologie induite par $\sigma(E, E')$, qui en fait un espace compact. Définissons l’application linéaire $u : E' \to \mathscr{C}(A)$ par

$$
u(x')(a) = \langle a, x' \rangle \quad (a \in A, \ x' \in E')
$$

Soit $(x'_n)_{n \in \mathbf{N}}$ une suite équicontinue dans $E'$, convergeant vers 0 pour $\sigma(E', E)$. La suite des fonctions $u(x'_n)$ est alors bornée dans $\mathscr{C}(A)$ et converge simplement vers 0. Pour tout $\mu \in \mathscr{C}(A)'$, on a $\lim_{n \to \infty} \mu(u(x'_n)) = 0$ d’après le lemme 2 (IV, p. 37). D’après le critère fourni par la remarque de III, p. 21, la forme linéaire $\mu \circ u$ sur $E'$ est donc continue pour $\sigma(E', E)$ quelle que soit $\mu \in \mathscr{C}(A)'$. Il existe donc une application linéaire $v : \mathscr{C}(A)' \to E$ satisfaisant à la relation

$$
\langle u(x'), \mu \rangle = \langle v(\mu), x' \rangle \quad (x' \in E', \ \mu \in \mathscr{C}(A)')
$$

Il est clair que $v$ est continue si l’on munit $\mathscr{C}(A)'$ de la topologie $\sigma(\mathscr{C}(A)', \mathscr{C}(A))$ et E de la topologie $\sigma(E, E')$.

La boule unité (fermée) B de l’espace de Banach $\mathscr{C}(A)'$ est compacte pour la topologie $\sigma(\mathscr{C}(A)', \mathscr{C}(A))$ (III, p. 17, cor. 3). Par suite, $v(B)$ est une partie de E convexe, équilibrée et compacte pour $\sigma(E, E')$. Pour tout $a \in A$, la forme linéaire continue $\varepsilon_a : f \mapsto f(a)$ sur $\mathscr{C}(A)$ appartient à B, et l’on a $v(\varepsilon_a) = a$ d’après les formules (7) et (8). On a donc $A \subset v(B)$, d’où $C \subset v(B)$. Ceci prouve que C est compacte pour $\sigma(E, E')$.

C.Q.F.D. \*

## EXERCICES {#evt-iv-s5-exercises}

See the [exercises for § 5](exercises/s5/).
