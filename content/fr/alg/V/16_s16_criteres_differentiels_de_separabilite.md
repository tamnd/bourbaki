---
book: alg
book_title: Algebra
chapter: V
chapter_title: Corps commutatifs
section: 16
section_title: CRITÈRES DIFFÉRENTIELS DE SÉPARABILITÉ
lang: fr
source: alg-iv-vii-fr
book_pages: A V.166-A V.168
pdf_pages: 0225-0235, 0270-0272
extraction: ocr
subsections:
    - "no": 1
      title: 'Prolongement des dérivations : cas des anneaux'
      page: 121
      pdf_page: 225
    - "no": 2
      title: 'Prolongement des dérivations : cas des corps'
      page: 122
      pdf_page: 226
    - "no": 3
      title: Dérivations dans les corps de caractéristique 0
      page: 124
      pdf_page: 228
    - "no": 4
      title: Dérivations dans les extensions séparables
      page: 126
      pdf_page: 230
    - "no": 5
      title: Indice d’une application linéaire
      page: 126
      pdf_page: 230
    - "no": 6
      title: Propriétés différentielles des extensions de type fini
      page: 127
      pdf_page: 231
    - "no": 7
      title: Bases de transcendance séparantes
      page: 130
      pdf_page: 234
statements: 33
exercises: 9
content_sha256: 24bef2fb88c76b05fffbba9ea5ecdefa6b82d964fc8b6a9549b0bcd31289dacd
---

## § 16. CRITÈRES DIFFÉRENTIELS DE SÉPARABILITÉ

### 1. Prolongement des dérivations : cas des anneaux

Soient $K$ un anneau commutatif, $A$ une $K$-algèbre commutative et $x = (x_i)_{i \in I}$ une famille d’éléments de $A$. Soit par ailleurs $\Delta$ une dérivation de $K$ dans un $A$-module $M$, autrement dit (III, p. 118) une application $\mathbf{Z}$-linéaire de $K$ dans $M$ satisfaisant à la relation $\Delta(cc') = c.\Delta(c') + c'.\Delta(c)$ pour $c, c'$ dans $K$. Pour tout $i \in I$, soit $D_i$ la dérivation partielle par rapport à $X_i$ dans l’anneau de polynômes $K[X_i]_{i \in I}$; c’est l’unique dérivation de cet anneau dans lui-même qui est nulle sur $K$ et sur $X_j$ pour tout $j$ dans $I - \{i\}$, et qui prend la valeur 1 sur $X_i$ (IV, p. 6). Pour tout polynôme $f = \sum_{\alpha \in \mathbf{N}^{(I)}} c_\alpha X^\alpha$ dans $K[X_i]_{i \in I}$, on notera $f^\Delta(x)$ l’élément $\sum_{\alpha \in \mathbf{N}^{(I)}} x^\alpha . \Delta(c_\alpha)$ de $M$.

#### Proposition 1 {#alg-v-s16-prop-1 .statement}

*On suppose que la famille* $x = (x_i)_{i \in I}$ *engendre la* $K$*-algèbre* $A$. *Soient* $(m_i)_{i \in I}$ *une famille d’éléments de* $M$ *et* $(f_\lambda)_{\lambda \in \Lambda}$ *une famille de polynômes engendrant l’idéal* $a$ *des polynômes* $f \in K[X_i]_{i \in I}$ *tels que* $f(x) = 0$. *Pour qu’il existe une dérivation* $D$ *de* $A$ *dans* $M$ *telle que* $D(c.1) = \Delta(c)$ *pour tout* $c \in K$ *et* $D(x_i) = m_i$ *pour tout* $i \in I$, *il faut et il suffit que l’on ait*
$$
f_\lambda^\Delta(x) + \sum_{i \in I} D_i f_\lambda(x).m_i = 0 \quad \text{pour tout } \lambda \in \Lambda .
$$
*S’il en est ainsi, la dérivation* $D$ *est unique et satisfait à*
$$
D(f(x)) = f^\Delta(x) + \sum_{i \in I} D_i f(x).m_i \quad \text{pour tout } f \in K[X_i]_{i \in I} .
$$

Posons $E = K[X_i]_{i \in I}$ et notons $\varphi$ le $K$-homomorphisme de $E$ sur $A$ qui applique $X_i$ sur $x_i$ pour tout $i \in I$; on a donc $\varphi(f) = f(x)$ pour tout $f \in E$. Considérons $M$ comme un $E$-module au moyen de l’homomorphisme $\varphi : E \to A$ et définissons une application $D'$ de $E$ dans $M$ par $D'(f) = f^\Delta(x) + \sum_{i \in I} D_i f(x) \cdot m_i$ (remarquer que la famille $(D_i f)_{i \in I}$ est à support fini pour tout $f \in E$). Il est immédiat que $D'$ est l’unique dérivation de $E$ dans $M$, prolongeant $\Delta$ et appliquant $X_i$ sur $m_i$ pour tout $i \in I$.

Soit $D$ une dérivation de $A$ dans $M$ telle que $D(c.1) = \Delta(c)$ pour tout $c \in K$ et $D(x_i) = m_i$ pour tout $i \in I$. Alors $D \circ \varphi$ est une dérivation de $E$ dans $M$, prolongeant $\Delta$ et appliquant $X_i$ sur $m_i$ pour tout $i \in I$. On a donc $D \circ \varphi = D'$, c’est-à-dire la relation (2). Ceci démontre l’unicité de $D$; de plus, la formule (1) est conséquence de $f_\lambda(x) = 0$ et de (2).

Réciproquement, supposons la relation (1) satisfaite ; autrement dit, on a $D'(f_\lambda) = 0$ pour tout $\lambda \in \Lambda$. Soit $f \in a$; il existe une famille à support fini $(q_\lambda)_{\lambda \in \Lambda}$ dans $E$ telle que $f = \sum_{\lambda \in \Lambda} q_\lambda \cdot f_\lambda$. On a
$$
D'(f) = \sum_{\lambda \in \Lambda} \left[ f_\lambda(x) \cdot D'(q_\lambda) + q_\lambda(x) \cdot D'(f_\lambda) \right]
$$
d’où $D'(f) = 0$ puisque $f_\lambda(x)$ et $D'(f_\lambda)$ sont nuls pour tout $\lambda \in \Lambda$. Comme $D'$ s’anule sur $a$, il existe une application $\mathbf{Z}$-linéaire $D$ de $A$ dans $M$ telle que $D' = D \circ \varphi$; il est immédiat que $D$ est la dérivation cherchée de $A$ dans $M$.

### 2. Prolongement des dérivations : cas des corps

Soient $K, L$ et $M$ des corps tels que $K \subset L \subset M$. D’après la prop. 21 (III, p. 136), on a une suite exacte de $M$-espaces vectoriels
$$
(E_{K,L,M}) \quad \Omega_K(L) \otimes_L M \xrightarrow{\alpha} \Omega_K(M) \xrightarrow{\beta} \Omega_L(M) \to 0 ;
$$
les applications $M$-linéaires $\alpha$ et $\beta$ sont caractérisées par les relations
(3) $$
\alpha(d_{L/K} x \otimes 1) = d_{M/K} x \quad \text{pour } x \in L
$$
(4) $$
\beta(d_{M/K} y) = d_{M/L} y \quad \text{pour } y \in M .
$$

Soit $V$ un $M$-espace vectoriel ; notons $D_K(M, V)$ l’espace vectoriel des $K$-dérivations de $M$ à valeurs dans $V$, et introduisons de même $D_K(L, V)$ et $D_L(M, V)$. D’après III, p. 135, diagramme (42) et III, p. 136, diagramme (44), on a un diagramme commutatif d’homomorphismes d’espaces vectoriels

$$
\begin{array}{ccccccccc}
0 & \to & \operatorname{Hom}_M(\Omega_L(M), V) & \xrightarrow{\operatorname{Hom}(\beta, 1)} & \operatorname{Hom}_M(\Omega_K(M), V) & \xrightarrow{\operatorname{Hom}(\alpha, 1)} & \operatorname{Hom}_M(\Omega_K(L) \otimes_L M, V) \\
& & \downarrow & & \downarrow & & \downarrow \\
0 & \to & \operatorname{Der}_L(M, V) & \xrightarrow{i_V} & \operatorname{Der}_K(M, V) & \xrightarrow{r_V} & \operatorname{Der}_K(L, V) ,
\end{array}
$$

où les flèches verticales sont des isomorphismes, où $i_V$ est l’injection canonique et $r_V$ l’application de restriction.

On déduit alors de II, p. 102, th. 5 et II, p. 104, prop. 10 la proposition suivante :

#### Proposition 2 {#alg-v-s16-prop-2 .statement}

*Les conditions suivantes sont équivalentes :*

a) *L’application $\alpha$ est injective.*
b) *Toute $K$-dérivation de $L$ dans $M$ se prolonge en une $K$-dérivation de $M$ dans $M$.*
c) *Toute $K$-dérivation de $L$ dans un $M$-espace vectoriel $V$ se prolonge en une $K$-dérivation de $M$ dans $V$.*

#### Proposition 3 {#alg-v-s16-prop-3 .statement}

*Soient $K$ un corps, $L$ une extension pure de $K$ et $(x_i)_{i \in I}$ une base pure de $L$* (V, p. 102, déf. 2).

a) *Soient $V$ un espace vectoriel sur $L$, $\Delta$ une dérivation de $K$ dans $V$ et $(v_i)_{i \in I}$ une famille d’éléments de $V$. Il existe une dérivation $D$ de $L$ dans $V$, et une seule, prolongeant $\Delta$ et telle que $D(x_i) = v_i$ pour tout $i \in I$.*
b) *Le $L$-espace vectoriel $\Omega_K(L)$ des $K$-différentielles de $L$ a pour base la famille $(dx_i)_{i \in I}$.*

L’assertion b) a été démontrée en IV, p. 22, et l’assertion a) s’en déduit aussitôt.

#### Corollaire {#alg-v-s16-n2-cor-1 .statement}

*Soit $P$ un sous-corps de $K$. L’application canonique $\alpha$ de $\Omega_P(K) \otimes_K L$ dans $\Omega_P(L)$ est injective, et la famille $(d_{L/P} x_i)_{i \in I}$ est une base (sur $L$) d’un sous-espace de $\Omega_P(L)$ supplémentaire de l’image de $\alpha : \Omega_P(K) \otimes_K L \to \Omega_P(L)$.*

La prop. 3, a) montre que toute $P$-dérivation de $K$ dans un espace vectoriel $V$ sur $L$ se prolonge en une $P$-dérivation de $L$ dans $V$; l’injectivité de $\alpha$ résulte alors de la prop. 2. La deuxième assertion du corollaire résulte de l’exactitude de la suite $(E_{P,K,L})$ et de la prop. 3, b) (compte tenu de la formule (4)).

#### Proposition 4 {#alg-v-s16-prop-4 .statement}

*Soient $K$ un corps, $L$ une extension algébrique et séparable de $K$ et $V$ un espace vectoriel sur $L$.*

a) *Toute $K$-dérivation de $L$ dans $V$ est nulle.*
b) *Si $\Delta$ est une dérivation de $K$ dans $V$, il existe une dérivation $D$ de $L$ dans $V$, et une seule, qui prolonge $\Delta$.*

Soit $D$ une $K$-dérivation de $L$ dans $V$. Si $E$ est une sous-extension de $L$, de degré fini sur $K$, la $K$-algèbre $E$ est étale, et l’on a donc $\Omega_K(E) = 0$ (V, p. 32, th. 3), d’où $D|E = 0$ par la propriété universelle de $\Omega_K(E)$ (III, p. 134). Comme $L$ est réunion d’une famille de sous-extensions de degré fini sur $K$, on a $D = 0$, d’où a).

Soit $\Delta$ une dérivation de $K$ dans $V$. Si $D'$ et $D''$ sont deux prolongements de $\Delta$ en une dérivation de $L$ dans $V$, la différence $D' - D''$ est une $K$-dérivation de $L$ dans $V$; elle est donc nulle d’après a), d’où $D' = D''$.

Il reste à prouver l’existence d’un prolongement de $\Delta$. Le théorème de Zorn (E, III, p. 20) entraîne l’existence d’un prolongement *maximal* $D_0$ de $\Delta$ en une dérivation définie dans un sous-corps $L_0$ de $L$ contenant $K$.

Soient $x$ dans $L$ et $g$ le polynôme minimal de $x$ sur $L_0$. Comme $L$ est algébrique et séparable sur $K$, $x$ est algébrique et séparable sur $L_0$ (V, p. 38, prop. 6 et p. 38, cor. 2); par suite, $x$ est une racine simple de $g$ (V, p. 38, prop. 5), d’où $g'(x) \neq 0$ (IV, p. 16, prop. 7). Si l’on définit $g^{D_0}(x)$ comme en V, p. 121, il existe donc un élément $u$ de $V$ tel que $g^{D_0}(x) + g'(x).u = 0$; d’après la prop. 1 (V, p. 121), il existe une dérivation $D$ de $L_0(x)$ dans $V$, prolongeant $D_0$ et telle que $D(x) = u$. Vu le caractère maximal de $(L_0, D_0)$, on a donc $L_0(x) = L_0$, d’où $x \in L_0$. Vu l’arbitraire de $x$, on a finalement $L_0 = L$.

#### Corollaire 1 {#alg-v-s16-prop-4-cor-1 .statement}

*On a* $\Omega_K(L) = 0$ *si* $L$ *est algébrique et séparable sur* $K$.
Le corollaire résulte de la prop. 4, *a)* car le $L$-espace vectoriel $\Omega_K(L)$ est engendré par l’image de la $K$-dérivation canonique $d_{L/K}: L \to \Omega_K(L)$.

#### Corollaire 2 {#alg-v-s16-prop-4-cor-2 .statement}

*Si* $L$ *est une extension algébrique et séparable d’un corps* $K$, *l’application canonique* $\alpha : \Omega_P(K) \otimes_K L \to \Omega_P(L)$ *est un isomorphisme pour tout sous-corps* $P$ *de* $K$.
L’application $\alpha$ est injective d’après la prop. 2 (V, p. 123) et la prop. 4, *b)* ; comme $\Omega_K(L)$ est réduit à 0 (cor. 1), l’exactitude de la suite $(E_{P,K,L})$ entraîne que $\alpha$ est surjective.

#### Corollaire 3 {#alg-v-s16-prop-4-cor-3 .statement}

*Soient* $E$ *une extension d’un corps* $K$ *et* $D$ *une dérivation de* $E$ *dans* $E$, *appliquant* $K$ *dans* $K$. *Si* $L$ *est une sous-extension de* $E$ *qui est algébrique et séparable sur* $K$, *on a* $D(L) \subset L$.
Soit $\Delta$ la dérivation de $K$ dans $L$ qui coïncide avec $D$ sur $K$. D’après la prop. 4 (V, p. 123), il existe une dérivation $D'$ de $L$ dans $L$ prolongeant $\Delta$. On peut considérer $D'$ et la restriction $D''$ de $D$ à $L$ comme des dérivations de $L$ dans $E$; comme elles coïncident sur $K$, on a $D' = D''$ d’après la prop. 4, d’où
$$
D(L) = D''(L) = D'(L) \subset L.
$$

#### Remarque 1 {#alg-v-s16-n2-rem-1 .statement}

Nous démontrerons plus loin (V, p. 125, cor. 3 et p. 129, cor. 2) une réciproque au cor. 1 de la prop. 4.

#### Remarque 2 {#alg-v-s16-n2-rem-2 .statement}

Toute extension algébrique d’un corps premier est séparable (V, p. 36, cor.). Comme toute dérivation d’un corps premier est nulle, toute dérivation d’une extension algébrique d’un corps premier est nulle (prop. 4).

### 3. Dérivations dans les corps de caractéristique 0

#### Théorème 1 {#alg-v-s16-thm-1 .statement}

*Soient* $K$ *un corps de caractéristique* 0, $L$ *une extension de* $K$ *et* $V$ *un espace vectoriel sur* $L$. *Soient* $\Delta$ *une dérivation de* $K$ *dans* $V$, $(x_i)_{i \in I}$ *une base de transcendance de* $L$ *sur* $K$ *et* $(u_i)_{i \in I}$ *une famille d’éléments de* $V$. *Il existe une dérivation* $D$ *de* $L$ *dans* $V$, *et une seule, prolongeant* $\Delta$ *et telle que* $D(x_i) = u_i$ *pour tout* $i \in I$.
Posons $E = K(x_i)_{i \in I}$. La prop. 3 (V, p. 123) montre que $\Delta$ se prolonge de manière unique en une dérivation $D_0$ de $E$ dans $V$ telle que $D_0(x_i) = u_i$ pour tout $i \in I$. Le corps $L$ est extension algébrique de $E$, et comme $L$ est de caractéristique 0, $L$ est séparable sur E (V, p. 36, cor.). Par suite (V, p. 123, prop. 4), D_0 se prolonge de manière unique en une dérivation D de L dans V.

#### Corollaire 1 {#alg-v-s16-thm-1-cor-1 .statement}

Toute dérivation de K dans V se prolonge en une dérivation de L dans V.

#### Corollaire 2 {#alg-v-s16-thm-1-cor-2 .statement}

Soient E une sous-extension de L et U le sous-L-espace vectoriel de $\Omega_K(L)$ engendré par les différentielles des éléments de E. Pour qu’un élément x de L soit algébrique sur E, il faut et il suffit que l’on ait $dx \in U$.

Pour tout $y \in L$, soit D(y) la classe de $dy$ modulo U. Alors D est une E-dérivation de L dans $\Omega_K(L)/U$. Comme K est de caractéristique 0, toute extension algébrique de E est séparable (V, p. 36, cor.) ; si $x \in L$ est algébrique sur E, on a $Dx = 0$ d’après la prop. 4 (V, p. 123), c’est-à-dire $dx \in U$.

Si $x \in L$ est transcendant sur E, il existe une E-dérivation $\Delta$ de E(x) dans L telle que $\Delta(x) = 1$ (V, p. 123, prop. 3) ; d’après le th. 1, $\Delta$ se prolonge en une E-dérivation D de L dans L. Soit $\varphi$ la forme linéaire sur $\Omega_K(L)$ telle que $D = \varphi \circ d$; on a $\varphi(dy) = 0$ pour $y \in E$ et $\varphi(x) = 1$, d’où $dx \notin U$.

#### Corollaire 3 {#alg-v-s16-thm-1-cor-3 .statement}

Pour qu’un élément x de L soit algébrique sur K, il faut et il suffit que l’on ait $dx = 0$ dans $\Omega_K(L)$. En particulier, pour que L soit une extension algébrique de K, il faut et il suffit que l’on ait $\Omega_K(L) = 0$.

Ce corollaire résulte immédiatement du cor. 2 où l’on fait $E = K$.

#### Corollaire 4 {#alg-v-s16-thm-1-cor-4 .statement}

Soient K, L et M des corps de caractéristique 0 tels que $K \subset L \subset M$; l’application canonique $\alpha : \Omega_K(L) \otimes_L M \to \Omega_K(M)$ est injective.

Ce corollaire résulte aussitôt du cor. 1 et de V, p. 122, prop. 2.

#### Théorème 2 {#alg-v-s16-thm-2 .statement}

Soient K un corps de caractéristique 0, L une extension de K et $(x_i)_{i \in I}$ une famille d’éléments de L.

a) Pour que $(x_i)_{i \in I}$ soit algébriquement libre sur K, il faut et il suffit que la famille des différentielles $dx_i$ (pour $i \in I$) dans $\Omega_K(L)$ soit linéairement libre sur L.

b) Pour que L soit algébrique sur $K(x_i)_{i \in I}$, il faut et il suffit que les différentielles $dx_i$ pour $i \in I$ engendrent l’espace vectoriel $\Omega_K(L)$ sur L.

c) Pour que $(x_i)_{i \in I}$ soit une base de transcendance de L sur K, il faut et il suffit que la famille $(dx_i)_{i \in I}$ soit une base de $\Omega_K(L)$ sur L.

Pour tout $i \in I$, soit $E_i$ le sous-corps $K(x_j)_{j \in I - \{i\}}$ de L. Pour que la famille $(x_i)_{i \in I}$ soit algébriquement libre sur K, il faut et il suffit (V, p. 104, prop. 5) que $x_i$ soit transcendant sur $E_i$ pour tout $i \in I$. D’après le cor. 2 du th. 1, ceci signifie que, pour tout $i \in I$, la différentielle $dx_i$ n’est pas combinaison linéaire à coefficients dans L des différentielles $dx_j$ pour $j \neq i$ dans I ; cette dernière condition signifie que la famille $(dx_i)_{i \in I}$ est libre sur L, d’où a).

L’assertion b) résulte aussitôt du cor. 2 du th. 1, et c) est conséquence de a) et b).

#### Corollaire {#alg-v-s16-n3-cor-1 .statement}

On a $[\Omega_K(L) : L] = \deg.\operatorname{tr}_K L$ lorsque K est de caractéristique 0.

### 4. Dérivations dans les extensions séparables

On a vu (V, p. 117, th. 1) que toute extension L d’un corps K de caractéristique 0 est séparable ; de plus, toute dérivation de K dans un espace vectoriel sur L se prolonge alors en une dérivation de L (V, p. 125, cor. 1). On a plus généralement l’énoncé suivant :

#### Théorème 3 {#alg-v-s16-thm-3 .statement}

Soient K un corps et L une extension de K. Pour que L soit séparable sur K, il faut et il suffit que toute dérivation de K dans un L-espace vectoriel se prolonge en une dérivation de L.

On peut supposer K de caractéristique $p \neq 0$. Supposons d’abord que L soit séparable sur K. Soient V un espace vectoriel sur L et $\Delta$ une dérivation de K dans V. D’après le critère de MacLane (V, p. 119, remarque), les corps $L^p$ et K sont linéairement disjoints sur $K^p$. Comme $\Delta$ est une application $K^p$-linéaire de K dans V, elle se prolonge de manière unique en une application $L^p$-linéaire $\Delta'$ de $K[L^p] = K(L^p)$ dans V. Il est immédiat que $\Delta'$ est une dérivation de $K(L^p)$ dans V nulle sur $L^p$; elle se prolonge donc (V, p. 97, cor. 1) en une dérivation de L dans V.

Réciproquement, supposons que toute dérivation de K à valeurs dans L se prolonge en une dérivation de L dans L. Soit B une $p$-base de K (V, p. 95) et soit $\Lambda$ l’ensemble des familles $(\alpha_b)_{b \in B}$ à support fini formées d’entiers compris entre 0 et $p - 1$. Pour tout $b \in B$, il existe une dérivation $\Delta_b$ de K dans K caractérisée par $\Delta_b(b') = \delta_{bb'}$ (symbole de Kronecker) pour tout $b' \in B$ (V, p. 98). Par hypothèse, il existe pour chaque $b \in B$ une dérivation $D_b$ de L dans L prolongeant $\Delta_b$. On a $D_b(b') = \delta_{bb'}$ pour $b, b'$ dans B, ce qui prouve que, dans $\Omega_{L^p}(L)$, les différentielles $db$ (pour $b \in B$) sont linéairement indépendantes sur L. Par suite (V, p. 97, th. 1), B est $p$-libre sur $L^p$. Par suite (V, p. 94, prop. 1 et p. 119, remarque), l’extension L de K est séparable.

#### Corollaire {#alg-v-s16-n4-cor-1 .statement}

Si L est extension séparable de K, l’application canonique $\alpha_P : \Omega_P(K) \otimes_K L \to \Omega_P(L)$ est injective pour tout sous-corps P de K. Réciproquement, s’il existe un sous-corps parfait P de K (par exemple le sous-corps premier de K) tel que l’application $\alpha_P$ soit injective, alors L est séparable sur K.

La première assertion résulte de la prop. 2 (V, p. 123) et du th. 3. Réciproquement, soit P un sous-corps parfait de K ; on a $P = P^p \subset K^p$, donc toute dérivation de K dans un L-espace vectoriel est une P-dérivation ; la deuxième assertion du corollaire résulte alors de la prop. 2 (V, p. 123) et du th. 3.

### 5. Indice d’une application linéaire

Soit L un corps $^1$. Soient U et V deux espaces vectoriels $^2$ sur L et $f : U \to V$ une application L-linéaire ; on dit que $f$ possède un indice si le noyau N et le conoyau C de $f$ sont de dimension finie, et l’on appelle indice de $f$ l’entier
$$
\chi(f) = [C : L] - [N : L].
$$
$^1$ Non nécessairement commutatif.
$^2$ A gauche.

#### Lemme 1 {#alg-v-s16-lem-1 .statement}

Soient U et V deux espaces vectoriels de dimension finie sur un corps L. Toute application linéaire $f : U \to V$ possède un indice égal à $[V : L] - [U : L]$.

Soient N le noyau, I l’image et C le conoyau de $f$. On a $C = V/I$ et I est isomorphe à $U/N$; on a donc $[U : L] = [N : L] + [I : L]$ et $[V : L] = [C : L] + [I : L]$, d’où le lemme.

#### Lemme 2 {#alg-v-s16-lem-2 .statement}

Soient $f : U \to V$ et $g : V \to W$ des applications L-linéaires. Si $f$ et $g$ possèdent un indice, il en est de même de $g \circ f$ et l’on a :

$$
\chi(g \circ f) = \chi(f) + \chi(g).
$$

Posons $h = g \circ f$; notons respectivement N, N', N'' les noyaux de $f, g, h$ et C, C', C'' les conoyaux de ces applications. On a $N \subset N'' \subset U$ et $f(N'') = f(U) \cap N'$; par suite, il existe une application linéaire $\overline{f} : N'' \to N'$ coïncidant avec $f$ sur $N''$ et de noyau N. L’application canonique $\pi$ de V sur $C = V/f(U)$ induit une application $\pi'$ de $N'$ dans $C$ dont le noyau est $f(U) \cap N' = \overline{f}(N'')$. Par passage au quotient, $g$ définit une application $\overline{g}$ de $C = V/f(U)$ dans $C'' = W/g(f(U))$ dont le noyau est évidemment $(N' + f(U))/f(U) = \pi'(N')$. Enfin, l’application canonique $\rho$ de $C'' = W/g(f(U))$ sur $C' = W/g(V)$ a pour noyau $g(V)/g(f(U)) = \overline{g}(C)$. En résumé, on a établi l’exactitude de la suite

$$
0 \to N \xrightarrow{i} N'' \xrightarrow{\overline{f}} N' \xrightarrow{\pi'} C \xrightarrow{\overline{g}} C'' \xrightarrow{\rho} C' \to 0
$$

(où $i$ est l’injection canonique de N dans $N''$).

![Diagramme commutatif](fig1.png)

Par hypothèse, N, N', C et C' sont de dimension finie ; il en est donc de même de N'' et C''. D’après le cor. 2 (II, p. 98), on a alors

$$
[N : L] - [N'' : L] + [N' : L] - [C : L] + [C'' : L] - [C' : L] = 0
$$

d’où $\chi(h) = \chi(f) + \chi(g)$.

### 6. Propriétés différentielles des extensions de type fini

#### Théorème 4 {#alg-v-s16-thm-4 .statement}

Soient P un corps parfait, L une extension de P et K une sous-extension de L ; on suppose que L est une extension de type fini de K. Alors l’application L-linéaire canonique $\alpha : \Omega_p(K) \otimes_K L \to \Omega_p(L)$ a un indice égal au degré de transcendance de $L$ sur $K$.

Si $E$ et $F$ sont deux sous-extensions de $L$ telles que $E \subset F$, nous noterons $\alpha(F/E)$ l’application $F$-linéaire canonique de $\Omega_p(E) \otimes_E F$ dans $\Omega_p(F)$ et, lorsqu’il est défini, l’indice de $\alpha(F/E)$ sera noté $d(F/E)$. Si $E$, $F$ et $G$ sont trois sous-extensions de $L$ telles que $E \subset F \subset G$, on a un diagramme commutatif

$$
\begin{array}{ccc}
\Omega_p(F) \otimes_F G & \xrightarrow{\alpha(G/F)} & \Omega_p(G) \\
\uparrow \alpha(F/E) \otimes_F \mathrm{Id}_G & & \uparrow \alpha(G/E) \\
(\Omega_p(E) \otimes_E F) \otimes_F G & \xrightarrow{\beta} & \Omega_p(E) \otimes_E G
\end{array}
$$

où $\beta$ est l’isomorphisme canonique défini dans la prop. 2 (II, p. 83). Comme l’indice est évidemment invariant par extension des scalaires et que l’indice d’un isomorphisme est nul, le lemme 2 (V, p. 127) montre que l’indice $d(G/E)$ est défini lorsque $d(F/E)$ et $d(G/F)$ le sont et que l’on a alors

$$
d(G/E) = d(G/F) + d(F/E)
$$

Comme $L$ est une extension de type fini de $K$, la formule (5) et le cor. de V, p. 106 montrent qu’il suffit de considérer le cas où il existe $x$ tel que $L = K(x)$; de plus, si $x$ est algébrique sur $K$, il existe une puissance $q$ de l’exposant caractéristique de $L$ tel que $x^q$ soit algébrique et séparable sur $K$ (V, p. 42, prop. 13). Il suffit d’établir l’égalité $d(L/K) = \deg.\mathrm{tr}_K L$ dans les trois cas particuliers ci-dessous.

a) $x$ est transcendant sur $K$ : alors $\alpha$ est injectif et son conoyau est de rang 1 sur $L$ (V, p. 123, cor.) ; on a donc $d(L/K) = 1$ et aussi $\deg.\mathrm{tr}_K L = 1$.

b) $x$ est algébrique et séparable sur $K$ : alors $\alpha$ est bijectif (V, p. 124, cor. 2), d’où $d(L/K) = 0$; on a évidemment $\deg.\mathrm{tr}_K L = 0$.

c) *Le corps $L$ est de caractère $p \neq 0$, on a $x \notin K$ et $x^p = a$ appartient à $K$* : le conoyau $C$ de $\alpha$ est isomorphe à $\Omega_K(L)$, et comme $\{ x \}$ est une $p$-base de $L$ sur $K$, l’espace $C$ est donc de dimension 1 sur $L$ (V, p. 97, th. 1). Comme $a$ est une puissance $p$-ième dans $L$, on a $d_{L/p} a = 0$, et le noyau de $\alpha$ contient le sous-espace $R$ de $U = \Omega_p(K) \otimes_K L$ engendré par $d_{K/p} a \otimes 1$. Pour tout $y \in K$, soit $\Delta(y)$ la classe de $d_{K/p} y \otimes 1$ modulo $R$; alors $\Delta$ est une P-dérivation de $K$ dans $U/R$ telle que $\Delta(a) = 0$. La prop. 5 (V, p. 96) montre que $\Delta$ se prolonge en une P-dérivation $D$ de $L$ dans $U/R$. Il existe alors une application $L$-linéaire $\beta : \Omega_p(L) \to U/R$ telle que $D = \beta \circ d_{L/p}$, et $\beta \circ \alpha$ est l’application canonique de $U$ sur $U/R$. Ceci prouve que $R$ est le noyau de $\alpha$. Comme $P$ est parfait, on a $P(K^p) = K^p$, d’où $a \notin P(K^p)$ et finalement $d_{K/p} a \neq 0$ (V, p. 99, prop. 6). Le noyau et le conoyau de $\alpha$ sont donc de dimension 1, d’où $d(L/K) = 0$; on a aussi $\deg.\mathrm{tr}_K L = 0$.

#### Corollaire 1 {#alg-v-s16-thm-4-cor-1 .statement}

*Soit $L$ une extension de type fini d’un corps $K$, de degré de transcendance $s$. L’espace vectoriel $\Omega_K(L)$ est de dimension $\geq s$ sur $L$, et l’on a égalité si et seulement si $L$ est séparable sur $K$.*

Soit P le sous-corps premier de K. Soit N le noyau de $\alpha$; d’après l’exactitude de la suite $(E_{P,K,L})$ (V, p. 122) et le th. 4, on a $[ \Omega_K(L) : L ] = s + [N : L]$; d’après V, p. 126, cor., l’extension L de K est séparable si et seulement si $N = 0$. D’où le corollaire.

#### Corollaire 2 {#alg-v-s16-thm-4-cor-2 .statement}

*Soit L une extension de type fini d’un corps K. Pour que L soit algébrique et séparable sur K, il faut et il suffit que l’on ait $\Omega_K(L) = 0$*.

Cela résulte aussitôt du corollaire 1.

#### Corollaire 3 {#alg-v-s16-thm-4-cor-3 .statement}

*Soient K un corps de caractéristique $p \neq 0$ et L une extension de type fini de K, de degré de transcendance s. Si $[K : K^p]$ est fini, il en en est de même de $[L : L^p]$ et l’on a $[L : L^p] = p^s . [K : K^p]$*.

Soit P le sous-corps premier de K. Si $[K : K^p]$ est fini, l’espace vectoriel $\Omega_P(K) = \Omega_{K^p}(K)$ est de dimension finie m sur K, et l’on a $[K : K^p] = p^m$ (V, p. 98, th. 2); l’espace vectoriel $\Omega_P(K) \otimes_K L$ est alors de dimension finie m sur L. Par ailleurs, comme K est de degré fini sur $K^p$, le corps $K(L^p)$ est de degré fini sur $K^p(L^p) = L^p$; comme le corps L est une extension de type fini de K et qu’il est algébrique sur $K(L^p)$, c’est une extension de degré fini de $K(L^p)$ (V, p. 17, th. 2); on en conclut que L est de degré fini sur $L^p$ (V, p. 9, th. 1). Alors $\Omega_P(L)$ est un espace vectoriel de dimension finie n sur L, et l’on a $[L : L^p] = p^n$ (V, p. 98, th. 2). D’après le lemme 1 (V, p. 127), l’application L-linéaire $\alpha : \Omega_P(K) \otimes_K L \to \Omega_P(L)$ a donc un indice égal à $n - m$, d’où $n - m = s$ d’après le th. 4 (V, p. 127) et $p^n = p^s . p^m$.

#### Remarque 1 {#alg-v-s16-n6-rem-1 .statement}

Soient K un corps de caractéristique $p \neq 0$ et L une extension de K. On a $\Omega_K(L) = 0$ si et seulement si l’on a $L = K(L^p)$ (V, p. 99, prop. 6). Par suite, si L est de type fini sur K, c’est une extension algébrique et séparable si et seulement si l’on a $L = K(L^p)$. Lorsque L n’est pas de type fini sur K, ce résultat cesse d’être valable comme le montre le cas où L est la clôture parfaite de K.

#### Remarque 2 {#alg-v-s16-n6-rem-2 .statement}

Soient K un corps, $F_1, ..., F_m$ des polynômes de $K[X_1, ..., X_n]$, et L une extension de K engendrée par des éléments $x_1, ..., x_n$. On suppose que les polynômes $F_1, ..., F_m$ engendrent l’idéal de $K[X_1, ..., X_n]$ formé des polynômes F tels que $F(x_1, ..., x_n) = 0$. On déduit facilement de la prop. 1 (V, p. 121) et de la propriété universelle des modules de différentielles (III, p. 134) le résultat suivant : l’espace vectoriel $\Omega_K(L)$ sur L est engendré par $dx_1, ..., dx_n$; on a les relations

$$
\sum_{i=1}^n D_i F_j(x_1, ..., x_n) \cdot dx_i = 0 \quad (\text{pour } 1 \leq j \leq m);
$$

enfin, si $u_1, ..., u_n$ sont des éléments de L tels que $\sum_{i=1}^n u_i \cdot dx_i = 0$, il existe des éléments $v_1, ..., v_m$ de L tels que $u_i = \sum_{j=1}^m D_i F_j(x_1, ..., x_n) v_j$ pour $1 \leq i \leq n$. Notons r le rang de la matrice $(D_i F_j(x_1, ..., x_n))$ à n lignes et m colonnes; soit s le degré de transcendance de L sur K. On a alors $[ \Omega_K(L) : L ] = n - r$. Par suite, l’extension L de K est séparable si et seulement si l’on a $r + s = n$ (cor. 1), elle est algébrique et séparable si et seulement si l’on a $r = n$ (cor. 2).

### 7. Bases de transcendance séparantes

#### Définition 1 {#alg-v-s16-def-1 .statement}

Soit L une extension d’un corps K. On dit qu’une base de transcendance B de L sur K est séparante si l’extension algébrique L de K(B) est séparable.

Si K est de caractéristique 0, toute base de transcendance de L sur K est séparante puisque toute extension algébrique d’un corps de caractéristique 0 est séparable (V, p. 36, cor.). Si une extension admet une base de transcendance séparante, elle est séparable (V, p. 116, prop. 6 et p. 117, prop. 9). Le théorème suivant montre que toute extension séparable de type fini admet une base de transcendance séparante ; cette restriction est essentielle (V, p. 166, exerc. 1).

#### Théorème 5 {#alg-v-s16-thm-5 .statement}

Soient K un corps, L une extension de K et $(x_i)_{i \in I}$ une famille d’éléments de L. Si la famille $(x_i)_{i \in I}$ est une base de transcendance séparante de L sur K, la famille $(dx_i)_{i \in I}$ est une base de l’espace vectoriel $\Omega_K(L)$ sur L. La réciproque est vraie si L est une extension séparable de type fini de K.

Posons $M = K(x_i)_{i \in I}$ et notons $a$ l’application canonique de $\Omega_K(M) \otimes_M L$ dans $\Omega_K(L)$. Si $(x_i)_{i \in I}$ est une base de transcendance séparante de L sur K, la famille $(d_{M/K} x_i)_{i \in I}$ est une base du M-espace vectoriel $\Omega_K(M)$ (V, p. 123, prop. 3) et $a$ est un isomorphisme de L-espaces vectoriels puisque L est algébrique et séparable sur M (V, p. 124, cor. 2). Comme on a $a(d_{M/K} x_i \otimes 1) = d_{L/K} x_i$, la famille $(d_{L/K} x_i)_{i \in I}$ est donc une base de $\Omega_K(L)$ sur L.

Réciproquement, supposons que L soit une extension séparable de type fini de K, et que la famille $(d_{L/K} x_i)_{i \in I}$ soit une base de l’espace vectoriel $\Omega_K(L)$ sur L. D’après le cor. 1 de V, p. 128, le degré de transcendance de L sur K est égal à la dimension de $\Omega_K(L)$ sur L, donc au cardinal de I. D’après la suite exacte $(E_{K,M,L})$ (V, p. 122), on a $\Omega_M(L) = 0$; comme L est une extension de type fini de M, le cor. 2 de V, p. 129, montre que L est algébrique et séparable sur $M = K(x_i)_{i \in I}$; comme le degré de transcendance de L sur K est fini et égal au cardinal de I, la famille $(x_i)_{i \in I}$ est une base de transcendance de L sur K (V, p. 106, cor. 1).

#### Corollaire {#alg-v-s16-n7-cor-1 .statement}

Soit L une extension séparable de type fini de K, et soit S une partie de L telle que $L = K(S)$. Il existe alors une base de transcendance séparante B de L sur K, contenue dans S.

Comme $\Omega_K(L)$ est engendré par les différentielles des éléments de S, il existe s éléments $x_1, ..., x_s$ de S tels que $(dx_1, ..., dx_s)$ soit une base de $\Omega_K(L)$ sur L. Il suffit alors d’appliquer le th. 5.

#### Remarque {#alg-v-s16-n7-rem-1 .statement}

Soit L une extension séparable de type fini d’un corps K de caractéristique $p \neq 0$; il peut exister des bases de transcendance de L qui ne sont pas séparantes. Il suffit de noter que $\{X^p\}$ est une base de transcendance de K(X) mais que K(X) est une extension radicielle de degré $p$ de K$(X^p)$.

#### Proposition 5 {#alg-v-s16-prop-5 .statement}

Soient L et M deux extensions d’un corps K, contenues dans une même extension et algébriquement disjointes sur K. Si M est séparable sur K, alors L(M) est séparable sur L.

Il suffit de montrer que, pour toute partie finie S de M, L(S) est séparable sur L (V, p. 116, prop. 8). Soit S une partie finie de M. Comme le corps K(S) est séparable sur K, il possède une base de transcendance séparante B (cor. du th. 5). Comme L et M sont algébriquement disjointes sur K, B est une base de transcendance de L(B) sur L (V, p. 108, prop. 12). De plus, tout élément de S est algébrique et séparable sur K(B), donc sur L(B) (V, p. 38, cor. 2). On en conclut (V, p. 38, prop. 6) que L(S) = L(B) (S) est algébrique et séparable sur L(B), donc L(S) est séparable sur L.

#### Corollaire {#alg-v-s16-n7-cor-2 .statement}

Si L et M sont des extensions séparables et algébriquement disjointes de K, le corps K(L ∪ M) est séparable sur K.

En effet, K(L ∪ M) = L(M) est séparable sur L d’après la prop. 5 (car M est séparable sur K) et L est séparable sur K, d’où le corollaire (V, p. 117, prop. 9).

L’hypothèse que les extensions L et M sont algébriquement disjointes est indispensable dans la prop. 5 et son corollaire. En effet, soient K un corps imparfait de caractéristique $p \neq 0$, et E une extension de la forme $K(x, a)$ avec x transcendant sur K et a radiciel de hauteur 1 sur K ; on pose $L = K(x)$ et $M = K(x + a)$. Alors $x + a$ est transcendant sur K (sinon $x = (x + a) - a$ serait algébrique sur K) et les corps L et M sont séparables sur K. Pourtant $K(L \cup M) = K(x, a)$ est radiciel de degré $p$ sur $L = K(x)$ et n’est séparable ni sur L, ni sur K.

## EXERCICES {#alg-v-s16-exercises}

See the [exercises for § 16](exercises/s16/).
