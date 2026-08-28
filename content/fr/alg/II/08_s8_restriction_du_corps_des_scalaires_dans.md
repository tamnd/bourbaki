---
book: alg
book_title: Algebra
chapter: II
chapter_title: ALGÈBRE LINÉAIRE
section: 8
section_title: Restriction du corps des scalaires dans les espaces vectoriels
lang: fr
source: alg-i-iii-fr
book_pages: A II.118-A II.126
pdf_pages: 0295-0303, 0376-0377
extraction: ocr
subsections:
    - "no": 1
      title: Définition des K'-structures
      page: 119
      pdf_page: 296
    - "no": 2
      title: Rationalité pour un sous-espace
      page: 120
      pdf_page: 297
    - "no": 3
      title: Rationalité pour une application linéaire
      page: 121
      pdf_page: 298
    - "no": 4
      title: Formes linéaires rationnelles
      page: 122
      pdf_page: 299
    - "no": 5
      title: Applications aux systèmes linéaires
      page: 123
      pdf_page: 300
    - "no": 6
      title: Plus petit corps de rationalité
      page: 0
      pdf_page: 301
    - "no": 7
      title: Critères de rationalité
      page: 125
      pdf_page: 302
statements: 17
exercises: 5
content_sha256: 4729d446b1507616c621f4747b8a2f39bd8ee7b4be4522eb01d76377e8bc1968
---

## § 8. RESTRICTION DU CORPS DES SCALAIRE S DANS LES ESPACES VECTORIELS

Dans tout ce paragraphe, $K$ désigne un corps, $K'$ un sous-corps de $K$. Sur un ensemble $V$, une structure d’espace vectoriel à droite (resp. à gauche) sur $K$ définit, par restriction des scalaires, une structure d’espace vectoriel à droite (resp. à gauche) sur $K'$.

### 1. Définition des K'-structures

#### Proposition 1 {#alg-ii-s8-prop-1 .statement}

Soient V un espace vectoriel à droite sur K, V' une partie de V qui soit un sous-espace vectoriel sur K'. Les conditions suivantes sont équivalentes ;
a) L’application K-linéaire $\lambda$ de $V'_{(K)} = V' \otimes_{K'} K$ dans V, telle que $\lambda(x' \otimes \xi) = x'\xi$ pour $x' \in V', \xi \in K$, est bijective.
b) Toute application K'-linéaire $f'$ de V' dans un K-espace vectoriel W se prolonge de manière unique en une application K-linéaire $f$ de V dans W.
c) Toute base de V' sur K' est une base de V sur K.
d) Il existe une base de V' sur K' qui soit aussi une base de V sur K.
e) Le K-espace vectoriel V est engendré par V', et toute partie de V' libre sur K' est libre sur K.

On sait (II, p. 81-82) que $V'_{(K)}$ est muni d’une structure de K-espace vectoriel à droite pour laquelle $(x' \otimes \xi)\eta = x' \otimes (\xi\eta)$ ($\xi, \eta$ dans K, $x' \in V'$), et que pour toute application K'-linéaire $f'$ de V' dans un K-espace vectoriel W, il existe une application K-linéaire $\tilde{f}'$ de $V'_{(K)}$ dans W et une seule telle que $\tilde{f}'(x' \otimes 1) = f'(x')$ pour $x' \in V'$. Si j est l’injection canonique de V' dans V, $\lambda$ n’est autre que l’application K-linéaire correspondante $\bar{j}$. Si $\lambda$ est bijective, alors, pour toute application K'-linéaire $f': V' \to W, \tilde{f}' \circ \lambda^{-1}$ est l’unique application K-linéaire de V dans W prolongeant $f'$; autrement dit, a) implique b). Inversement, si b) est vérifiée, il existe en particulier une application K-linéaire $\mu$ de V dans $V'_{(K)}$ telle que $\mu(x') = x' \otimes 1$ pour tout $x' \in V'$; il est immédiat que $\mu \circ \lambda = 1_{V'_{(K)}}$; d’autre part $\lambda(\mu(x')) = x'$ pour tout $x' \in V'$, et comme par hypothèse $j: V' \to V$ se prolonge d’une seule manière en un endomorphisme de V, on a nécessairement $\lambda \circ \mu = 1_V$, ce qui achève de prouver que a) et b) sont équivalentes.

Pour toute base B' de V' sur K', l’ensemble B des éléments $v' \otimes 1$ de $V'_{(K)}$, où $v'$ parcourt B', est une base de $V'_{(K)}$ sur K (II, p. 84, prop. 4), et $\lambda(B) = B'$. Pour que $\lambda$ soit bijective, il est nécessaire que l’image par $\lambda$ de toute base de $V'_{(K)}$ soit une base de V sur K, et il suffit qu’il en soit ainsi pour une seule base de $V'_{(K)}$ (II, p. 24, cor. 2). Ceci prouve l’équivalence de a), c) et d).

Comme toute partie de V' libre sur K' est contenue dans une base de V' sur K' (II, p. 95, th. 2), c) implique e). Enfin, supposons e) vérifiée; si B' est une base de V' sur K', c’est une partie de V libre sur K; d’autre part, B' engendre V' sur K', donc engendre V sur K par hypothèse; par suite B' est une base de V sur K, ce qui prouve que e) entraîne c).

C. Q. F. D.

#### Définition 1 {#alg-ii-s8-def-1 .statement}

Soient V un espace vectoriel à droite sur un corps K et K' un sous-corps de K. On appelle K'-structure sur V tout sous-K'-espace vectoriel V' de V qui vérifie les conditions équivalentes de la proposition 1.

#### Exemple {#alg-ii-s8-n1-exa-1 .statement}

Soit B une base de V sur K. Pour tout sous-corps K' de K, le sous-K'-espace vectoriel de V engendré par B admet B pour base sur K', donc est une

K'-structure sur V. *Par exemple, si K est commutatif, et si on prend pour V la K-algèbre de polynômes K[X_1, ..., X_n], alors, pour tout sous-corps K' de K, K'[X_1, ..., X_n] est une K'-structure sur V.*

### 2. Rationalité pour un sous-espace

#### Définition 2 {#alg-ii-s8-def-2 .statement}

Soient V un espace vectoriel à droite sur K, muni d’une K'-structure V'. On dit qu’un vecteur de V est rationnel sur K' s’il appartient à V'. On dit qu’un sous-K-espace vectoriel W de V est rationnel sur K' s’il est engendré (sur K) par des vecteurs rationnels sur K'.

Soit (v'_i)_{i \in I} une base de V' sur K', qui est donc aussi une base de V sur K (II, p. 119, prop. 1). Pour qu’un vecteur x = $\sum_i v'_i \xi_i$ de V soit rationnel sur K', il faut et il suffit que $\xi_i \in K'$ pour tout $i \in I$.

Si W est un sous-K-espace vectoriel de V, rationnel sur K', il résulte de la déf. 2 que W' = W \cap V' est un sous-K'-espace vectoriel de W, qui engendre W sur K; par ailleurs toute partie de W' libre sur K' est aussi libre sur K puisqu’elle est contenue dans V' (II, p. 119, prop. 1). Il en résulte (II, p. 119, prop. 1) que W' est une K'-structure sur W, dite induite par la K'-structure V' de V.

Pour tout sous-K'-espace vectoriel W' de V' nous noterons W'.K le sous-K-espace vectoriel de V formé des combinaisons linéaires d’éléments de W' à coefficients dans K.

#### Proposition 2 {#alg-ii-s8-prop-2 .statement}

Soient V un espace vectoriel à droite sur K, V' une K'-structure sur V. L’application W' \mapsto W'.K est une bijection de l’ensemble des sous-K'-espaces vectoriels de V' sur l’ensemble des sous-K-espaces vectoriels de V rationnels sur K', et la bijection réciproque est W \mapsto W \cap V'.

Il est clair en effet que la bijection $\lambda^{-1}: V \to V' \otimes_{K'} K$, réciproque de la bijection $\lambda$ définie dans II, p. 119, prop. 1, applique tout sous-K'-espace vectoriel W' de V' sur son image par l’injection canonique $x' \mapsto x' \otimes 1$, et W'.K sur W' $\otimes_{K'} K$; les assertions de la prop. 2 sont donc conséquences de la déf. 2 et de II, p. 113, prop. 19.

#### Corollaire 1 {#alg-ii-s8-prop-2-cor-1 .statement}

Toute somme et toute intersection de sous-K-espaces vectoriels de V, rationnels sur K', est un sous-espace rationnel sur K'.

L’assertion relative à la somme est évidente. D’autre part, si $(W'_i)_{i \in I}$ est une famille de sous-K'-espaces vectoriels de V', on a $(\bigcap_{i \in I} W'_i) \otimes_{K'} K = \bigcap_{i \in I} (W'_i \otimes_{K'} K)$ (II, p. 109, cor. de la prop. 14), ce qui démontre le corollaire.

On dit qu’une base B de V sur K est rationnelle sur K' si elle est formée de vecteurs rationnels sur K'.

#### Corollaire 2 {#alg-ii-s8-prop-2-cor-2 .statement}

Toute base de V sur K, rationnelle sur K', est une base de V' sur K'.

En effet, si $W'$ est le sous-$K'$-espace vectoriel de $V'$ engendré par $B$, on a $W'.K = V = V'.K$, d’où $V' = W'$ en vertu de la prop. 2.

### 3. Rationalité pour une application linéaire

#### Définition 3 {#alg-ii-s8-def-3 .statement}

Soient $V_1, V_2$ deux espaces vectoriels à droite sur $K$, munis respectivement de $K'$-structures $V'_1, V'_2$. On dit qu’une application $K$-linéaire $f : V_1 \to V_2$ est rationnelle sur $K'$ si l’on a $f(V'_1) \subset V'_2$.

Si $V_3$ est un troisième espace vectoriel à droite sur $K$, muni d’une $K'$-structure $V'_3$, et si une application $K$-linéaire $g : V_2 \to V_3$ est rationnelle sur $K'$, il est clair que $g \circ f : V_1 \to V_3$ est rationnelle sur $K'$.

#### Proposition 3 {#alg-ii-s8-prop-3 .statement}

Soient $V_1, V_2$ deux espaces vectoriels à droite sur $K$, $V'_1, V'_2$ des $K'$-structures sur $V_1, V_2$ respectivement. On identifie canoniquement $V_1$ (resp. $V_2$) à $V'_1 \otimes_{K'} K$ (resp. $V'_2 \otimes_{K'} K$) (II, p. 119, prop. 1).

(i) L’application $f' \mapsto f' \otimes 1_K = f'_{(K)}$ est une bijection de $\mathrm{Hom}_{K'}(V'_1, V'_2)$ sur l’ensemble des applications $K$-linéaires de $V_1$ dans $V_2$, rationnelles sur $K'$; la bijection réciproque associe à toute application $K$-linéaire $f : V_1 \to V_2$, rationnelle sur $K'$, l’application $K'$-linéaire $f' : V'_1 \to V'_2$, ayant même graphe que la restriction de $f$ à $V'_1$.

(ii) Pour toute application $K$-linéaire $f : V_1 \to V_2$, rationnelle sur $K'$, on a $f(V'_1) = f(V_1) \cap V'_2$ et $f(V'_2) = V'_1 + \mathrm{Ker}(f)$.

(i) Il est clair qu’avec les identifications faites, si $f' : V'_1 \to V'_2$ est une application $K'$-linéaire, $f'_{(K)} = f' \otimes 1_K$ est rationnelle sur $K'$ et $f'$ est l’application ayant même graphe que la restriction de $f'_{(K)}$ à $V'_1$. Inversement, si $f : V_1 \to V_2$ est une application $K$-linéaire, rationnelle sur $K'$, et si $f' : V'_1 \to V'_2$ a même graphe que la restriction de $f$ à $V'_1$, $f$ et $f'_{(K)}$ coïncident dans $V'_1$, qui est un système générateur sur $K$ de $V_1$, donc $f = f'_{(K)}$.

(ii) Si $f = f' \otimes 1_K$, on a $f(V_1) = f(V'_1 \otimes_{K'} K) = f'(V'_1) \otimes_{K'} K$, et comme $f'(V'_1) \subset V'_2$, on a $f(V'_1) = f'(V'_1) = f(V_1) \cap V'_2$ (II, p. 113, prop. 19); la formule $f(V'_2) = V'_1 + \mathrm{Ker}(f)$ en résulte aussitôt.

#### Corollaire 1 {#alg-ii-s8-prop-3-cor-1 .statement}

Avec les notations de la prop. 3, on a
$\mathrm{Im}(f) = (\mathrm{Im}(f'))_{(K)}, \mathrm{Ker}(f) = (\mathrm{Ker}(f'))_{(K)}, \mathrm{Coker}(f) = (\mathrm{Coker}(f'))_{(K)}.$
En particulier, pour que $f$ soit injective (resp. surjective, nulle) il faut et il suffit que $f'$ le soit. Si $f$ est bijective, son application réciproque est rationnelle sur $K'$.
C’est un cas particulier de II, p. 113, cor. de la prop. 18.

#### Corollaire 2 {#alg-ii-s8-prop-3-cor-2 .statement}

Soit $f : V_1 \to V_2$ une application $K$-linéaire, rationnelle sur $K'$. Pour tout sous-$K$-espace vectoriel $W_1$ de $V_1$ (resp. $W_2$ de $V_2$) rationnel sur $K'$, $f(W_1)$ (resp. $f(W_2)$) est un sous-$K$-espace vectoriel de $V_2$ (resp. $V_1$) rationnel sur $K'$.
Avec les notations de la prop. 3, pour tout sous-$K'$-espace vectoriel $W'_1$ de $V'_1$, on a $f'_{(K)}(W'_1 \otimes_{K'} K) = f'(W'_1) \otimes_{K'} K$; d’où l’assertion relative à $W_1$ (II, p. 120, prop. 2). D’autre part, soit $W'_2$ un sous-$K'$-espace vectoriel de $V'_2$, et soit $g'$ l’application $K'$-linéaire canonique $V'_2 \to V'_2/W'_2$; on a $f^{-1}(W'_2) = \mathrm{Ker}(g' \circ f')$; en vertu du cor. 1, on a donc $f_{(K)}^{-1}(W'_2 \otimes_{K'} K) = f^{-1}(W'_2) \otimes_{K'} K$, d’où l’assertion relative à $W_2$.

Soient $V_1, V_2$ deux $K$-espaces vectoriels à droite, munis respectivement de $K'$-structures $V'_1, V'_2$. Il est immédiat que $V'_1 \times V'_2$ est une $K'$-structure sur $V_1 \times V_2$, dite *produit* des $K'$-structures $V'_1$ et $V'_2$.

#### Proposition 4 {#alg-ii-s8-prop-4 .statement}

*Pour qu’une application K-linéaire $f : V_1 \to V_2$ soit rationnelle sur $K'$, il faut et il suffit que son graphe $\Gamma$ soit rationnel sur $K'$ pour la $K'$-structure produit de $V_1 \times V_2$*.

Soit $g$ l’application $x_1 \mapsto (x_1, f(x_1))$ de $V_1$ dans $V_1 \times V_2$; c’est une application $K$-linéaire telle que $\Gamma = g(V_1)$; si $f$ est rationnelle sur $K'$, il en est de même de $\Gamma$ en vertu de II, p. 121, cor. 2. Inversement, supposons $\Gamma$ rationnel sur $K'$ et munissons-le de la $K'$-structure induite par celle de $V_1 \times V_2$; il résulte aussitôt des définitions que les restrictions $p_1, p_2$ à $\Gamma$ des projections $\mathrm{pr}_1, \mathrm{pr}_2$, sont des applications $K$-linéaires, rationnelles sur $K'$, de $\Gamma$ dans $V_1$ et $V_2$ respectivement. Comme $p_1$ est bijective, son application réciproque $q_1$ est rationnelle sur $K'$ (II, p. 121, cor. 1), donc il en est de même de $f = p_2 \circ q_1$.

### 4. Formes linéaires rationnelles

Soit $V$ un espace vectoriel à droite sur $K$, muni d’une $K'$-structure $V'$. Comme $K'_d$ est une $K'$-structure sur le $K$-espace vectoriel à droite $K_d$, on peut définir les *formes linéaires* $x^* \in V^*$, *rationnelles sur $K'$*, comme les applications linéaires de $V$ dans $K_d$, rationnelles sur $K'$ pour les $K'$-structures de $V$ et de $K_d$. En vertu de II, p. 121, prop. 3, l’ensemble $R'$ de ces formes linéaires est l’image du dual ${V'}^*$ de $V'$ par l’application composée

$$
{V'}^* \xrightarrow{\varphi} K \otimes_{K'} {V'}^* \xrightarrow{\upsilon} V^*
$$

où $\varphi({x'}^*) = 1 \otimes {x'}^*$, et $\upsilon(\xi \otimes {x'}^*)$ est la forme linéaire $y^*$ sur $V$ telle que $y^*(x') = \xi \langle {x'}^*, x' \rangle$ pour tout $x' \in V'$ (II, p. 87). On sait que cette application est injective (II, p. 114, prop. 20 et p. 113, prop. 19) et il est clair que $R'$ est un sous-$K'$-espace vectoriel à gauche de $V^*$; en outre toute partie de $R'$ libre sur $K'$ est libre sur $K$. Mais en général $R'$ *n’engendre pas nécessairement* $V^*$ sur $K$ et ne définit donc pas une $K'$-structure sur $V^*$ (II, p. 199, exerc. 2). Toutefois, si $V$ est de dimension *finie* $n$ sur $K$, ${V'}^*$ est de dimension $n$ sur $K'$, et $R'$ définit alors canoniquement une $K'$-structure sur $V^*$.

#### Proposition 5 {#alg-ii-s8-prop-5 .statement}

*Soient $V$ un espace vectoriel à droite sur $K$, $V'$ une $K'$-structure sur $V$, $W$ un sous-K-espace vectoriel de $V$. Pour que $W$ soit rationnel sur $K'$, il faut et il suffit qu’il existe un ensemble $H \subset V^*$ de formes linéaires rationnelles sur $K'$, tel que $W$ soit l’orthogonal de $H$ dans $V$ (II, p. 42).

Soit $H$ une partie de $V^*$ dont les éléments sont des formes linéaires rationnelles sur $K'$. Pour tout $x^* \in H$, le noyau de $x^*$ est un sous-$K$-espace vectoriel de $V$, rationnel sur $K'$ (II, p. 121, cor. 2); l’intersection de ces noyaux est donc aussi un sous-$K$-espace vectoriel de $V$, rationnel sur $K'$ (II, p. 120, cor. 1).

Inversement, soit $W$ un sous-$K$-espace vectoriel de $V$, rationnel sur $K'$, de sorte que $W$ s’identifie à $W' \otimes_{K'} K$, où $W' = W \cap V'$ (II, p. 120, prop. 2). Pour qu’une forme linéaire ${x'}^* \in {V'}^*$ soit nulle dans $W'$, il faut et il suffit que la forme linéaire $x^* \in V^*$ qui lui correspond par (1) (II, p. 122) soit nulle dans $W$, car en vertu de II, p. 121, cor. 1, on a $\mathrm{Ker}(x^*) = (\mathrm{Ker}({x'}^*)) \otimes_{K'} K$, et $\mathrm{Ker}({x'}^*) = (\mathrm{Ker}(x^*)) \cap V'$. Soit $H'$ l’orthogonal de $W'$ dans ${V'}^*$; on sait (II, p. 104, th. 7) que $W'$ est l’orthogonal de $H'$ dans $V'$; si $H$ est l’image de $H'$ dans $V^*$ par l’application (1), il résulte de ce qui précède que $W$ est l’orthogonal de $H$ dans $V$, compte tenu de II, p. 109, cor. de la prop. 14.

### 5. Applications aux systèmes linéaires

#### Proposition 6 {#alg-ii-s8-prop-6 .statement}

(i) Étant donné un système d’équations linéaires homogènes

$$
\sum_{l \in I} \alpha_{\mu l} \xi_l = 0 \tag{2}
$$

dont les coefficients $\alpha_{\mu l}$ appartiennent à $K'$, toute solution $(\xi_l)$ de ce système formée d’éléments de $K$ est combinaison linéaire à coefficients dans $K$ de solutions $(\xi'_l)$ de (2) formées d’éléments de $K'$.

(ii) Étant donné un système d’équations linéaires

$$
\sum_{l \in I} \alpha_{\mu l} \xi_l = \beta_\mu \tag{3}
$$

dont les coefficients $\alpha_{\mu l}$ et les seconds membres $\beta_\mu$ appartiennent à $K'$, s’il existe une solution du système formée d’éléments de $K$, il existe aussi une solution formée d’éléments de $K'$.

(i) Pour tout ensemble $S$, munissons le $K$-espace vectoriel à droite $K_d^{(S)}$ de la $K'$-structure $K_d^{(S)}$. Soit $f$ l’application $K$-linéaire de $K_d^{(I)}$ dans $K_d^{(M)}$ faisant correspondre à tout vecteur $(\xi_l)_{l \in I}$ le vecteur $(\zeta_\mu)_{\mu \in M}$ défini par $\zeta_\mu = \sum_{l \in I} \alpha_{\mu l} \xi_l$ pour tout $\mu \in M$. Il est clair que $f$ est rationnelle sur $K'$; son noyau $V$, qui est l’ensemble des solutions dans $K$ du système (2), est un sous-espace de $K_d^{(I)}$ rationnel sur $K'$ (II, p. 121, cor. 2), donc engendré par les solutions de (2) dans $K'$.

(ii) Considérons $K$ comme $K'$-espace vectoriel à gauche; il existe un projecteur $K'$-linéaire $p$ de $K$ sur son sous-espace vectoriel $K'_s$ (II, p. 98, prop. 4); si $(\xi_l)$ est une solution de (3) dans $K$, on a $\sum_{l \in I} \alpha_{\mu l} p(\xi_l) = p \left( \sum_{l \in I} \alpha_{\mu l} \xi_l \right) = p(\beta_\mu) = \beta_\mu$, ce qui prouve que $(p(\xi_l))$ est une solution de (3) dans $K'$.

### 6. Plus petit corps de rationalité

Soit $V$ un $K$-espace vectoriel à droite, muni d’une $K'$-structure $V'$. Pour tout corps $L$ tel que $K' \subset L \subset K$, on posera $V_L = V'.L$; il est clair que toute base de $V'$ sur $K'$ est une base de $V$ sur $K$ et une base de $V_L$ sur $L$. Donc $V_L$ est une $L$-structure sur $V$, et $V'$ une $K'$-structure sur $V_L$.

#### Proposition 7 {#alg-ii-s8-prop-7 .statement}

(i) *Soit $V$ un $K$-espace vectoriel à droite muni d’une $K'$-structure $V'$. Pour tout vecteur $x \in V$ (resp. tout sous-$K$-espace vectoriel $W$ de $V$), l’ensemble des sous-corps $L$ de $K$ contenant $K'$ et tels que $x$ (resp. $W$) soit rationnel sur $L$, possède un plus petit élément $K'(x)$ (resp. $K'(W)$).*

(ii) *Soient $V_1, V_2$ deux $K$-espaces vectoriels à droite munis respectivement de $K'$-structures $V'_1, V'_2$. Pour toute application $K$-linéaire $f$ de $V_1$ dans $V_2$, l’ensemble des sous-corps $L$ de $K$ contenant $K'$ et tels que $f$ soit rationnel sur $L$, possède un plus petit élément $K'(f)$.*

Démontrons d’abord l’assertion de (i) relative à un vecteur $x \in V$. Soit $B$ une base de $V$ rationnelle sur $K'$; $B$ est une base de $V'$ sur $K'$ et une base de $V_L$ sur $L$ pour tout corps $L$ tel que $K' \subset L \subset K$; pour que $x = \sum_{b \in B} b \xi_b$ soit rationnel sur $L$, il faut et il suffit que les $\xi_b$ appartiennent à $L$ (II, p. 120), donc le plus petit corps $L$ ayant cette propriété est le sous-corps de $K$ *engendré* par $K'$ et les $\xi_b$ pour $b \in B$.

Démontrons ensuite (ii). Soient $B_1, B_2$ des bases de $V_1, V_2$ respectivement, rationnelles sur $K'$, et posons, pour tout $b_1 \in B_1$, $f(b_1) = \sum_{b_2 \in B_2} b_2 \alpha_{b_2 b_1}$ (*la famille $(\alpha_{b_2 b_1})$ n’est autre que la *matrice* de $f$ par rapport aux bases $B_1$ et $B_2$; cf. II, p. 144 *). Comme $B_1$ (resp. $B_2$) est une base de $(V_1)_L$ (resp. $(V_2)_L$) sur $L$ pour tout corps $L$ tel que $K' \subset L \subset K$, pour que $f$ soit rationnel sur $L$, il faut et il suffit que les $\alpha_{b_2 b_1}$ appartiennent à $L$; le plus petit corps ayant cette propriété est donc le corps *engendré* par $K'$ et les $\alpha_{b_2 b_1}$ pour $b_1 \in B_1, b_2 \in B_2$.

Enfin, pour établir l’assertion de (i) relative à un sous-espace $W$ de $V$, nous démontrerons d’abord le lemme suivant:

#### Lemme 1 {#alg-ii-s8-lem-1 .statement}

*Soient $V$ un $K$-espace vectoriel à droite muni d’une $K'$-structure $V'$, $W$ un sous-$K$-espace vectoriel de $V$. Il existe deux sous-$K$-espaces vectoriels $W_1, W_2$ de $V$, rationnels sur $K'$, tels que $V$ soit somme directe de $W_1$ et $W_2$ et que, si l’on identifie $V$ à $W_1 \times W_2$, $W$ soit le graphe d’une application $K$-linéaire $g$ de $W_1$ dans $W_2$.*

Soit $B$ une base de $V$ rationnelle sur $K'$. Appliquant le th. 2 de II, p. 95 à une base de $W$ sur $K$, considérée comme partie libre de $V$, et au système générateur réunion de cette partie libre et de $B$, on voit qu’il existe une partie $C$ de $B$ telle que $V$ soit somme directe de $W$ et du sous-espace $W_2$ de $V$ engendré par $C$. Soit par ailleurs $W_1$ le sous-espace de $V$ engendré par $B - C$. Comme $B \subset V'$, il est clair que $W_1$ et $W_2$ sont rationnels sur $K'$. En outre, pour tout $x \in W_1$, il existe un vecteur et un seul $g(x)$ de $W_2$ tel que $x + g(x) \in W$, puisque $V$ est somme directe de $W$ et $W_2$; alors $W$ est le graphe de $g$, et $g$ est $K$-linéaire puisque $W$ est un sous-$K$-espace vectoriel de $V$.

Ce lemme étant démontré, on sait que $W$ est rationnel sur un sous-corps $L$ de $K$ contenant $K'$ si et seulement si $g$ est rationnelle sur $L$ (II, p. 122, prop. 4). Le plus petit corps $K'(g)$ tel que $g$ soit rationnelle sur $K'(g)$ est donc aussi le plus petit corps sur lequel $W$ soit rationnel.

### 7. Critères de rationalité

Pour tout sous-corps $L$ de $K$, notons $\mathrm{End}_L(K)$ l’anneau des endomorphismes de $K$ considéré comme *espace vectoriel à gauche* sur $L$; si $L$ contient $K'$, $\mathrm{End}_L(K)$ est un sous-anneau de $\mathrm{End}_{K'}(K)$. Pour toute partie $\mathcal{M}$ de $\mathrm{End}_{K'}(K)$, il existe un *plus grand sous-corps* $L$ de $K$ contenant $K'$ et tel que $\mathcal{M}$ soit contenue dans $\mathrm{End}_L(K)$, à savoir l’ensemble des $\xi \in K$ tels que $\varphi(\xi \eta) = \xi \varphi(\eta)$ pour tout $\eta \in K$ et tout $\varphi \in \mathcal{M}$ (on vérifie aussitôt que cet ensemble est un sous-anneau, et d’autre part, en remplaçant $\eta$ par $\xi^{-1} \eta$ dans la relation précédente, il vient $\varphi(\xi^{-1} \eta) = \xi^{-1} \varphi(\eta)$ lorsque $\xi \neq 0$). Nous dirons que ce corps est le *commutant* de $\mathcal{M}$ dans $K$ et nous le noterons $\chi(\mathcal{M})$.

Soit maintenant $V$ un $K$-espace vectoriel à droite muni d’une $K'$-structure $V'$. Pour tout $\varphi \in \mathrm{End}_{K'}(K)$, il existe un endomorphisme $\varphi_V$ du $\mathbf{Z}$-module $V$ et un seul tel que l’on ait $\varphi_V(x'.\xi) = x'.\varphi(\xi)$ pour $x' \in V'$ et $\xi \in V$: en effet, on a défini dans II, p. 119 un $\mathbf{Z}$-isomorphisme $\lambda$ de $V' \otimes_{K'} K$ sur $V$ transformant $x' \otimes \xi$ en $x'.\xi$, et $\varphi_V$ est nécessairement égal à $\lambda \circ (1_{V'} \otimes \varphi) \circ \lambda^{-1}$.

#### Théorème 1 {#alg-ii-s8-thm-1 .statement}

*Soient $\mathcal{M}$ une partie de $\mathrm{End}_{K'}(K)$, $L = \chi(\mathcal{M})$ le sous-corps de $K$ commutant de $\mathcal{M}$.*

(i) *Soit $V$ un $K$-espace vectoriel à droite muni d’une $K'$-structure. Pour qu’un vecteur $x \in V$ soit rationnel sur $L$, il faut et il suffit que l’on ait $\varphi_V(x.\eta) = x.\varphi(\eta)$ pour tout $\varphi \in \mathcal{M}$ et tout $\eta \in K$. Pour qu’un sous-$K$-espace vectoriel $W$ de $V$ soit rationnel sur $L$, il faut et il suffit que l’on ait $\varphi_V(W) \subset W$ pour tout $\varphi \in \mathcal{M}$.*

(ii) *Soient $V_1, V_2$ deux $K$-espaces vectoriels à droite munis chacun d’une $K'$-structure. Pour qu’une application $K$-linéaire $f$ de $V_1$ dans $V_2$ soit rationnelle sur $L$, il faut et il suffit que l’on ait $f(\varphi_{V_1}(x_1)) = \varphi_{V_2}(f(x_1))$ pour tout $x_1 \in V_1$ et tout $\varphi \in \mathcal{M}$.*

Prouvons d’abord l’assertion de (i) relative à $x$. Soit $B$ une base de $V$ rationnelle sur $K'$, et posons $x = \sum_{b \in B} b.\xi_b$; pour $\varphi \in \mathcal{M}$ et $\eta \in K$, on a alors

$$
\varphi_V(x.\eta) - x.\varphi(\eta) = \sum_{b \in B} b.(\varphi(\xi_b \eta) - \xi_b \varphi(\eta))
$$

et par suite, les relations

« pour tout $\varphi \in \mathcal{M}$ et tout $\eta \in K$, $\varphi_v(x.\eta) = x.\varphi(\eta)$ »

et

« pour tout $\varphi \in \mathcal{M}$, tout $b \in B$ et tout $\eta \in K$, $\varphi(\xi_b\eta) = \xi_b\varphi(\eta)$ »

sont équivalentes. La seconde de ces relations signifie que pour tout $b \in B$, on a $\xi_b \in \chi(\mathcal{M})$, ce qui prouve la première assertion de (i).

Prouvons ensuite (ii). Pour que $f$ soit rationnelle sur $L$, il faut et il suffit que pour tout $x'_1 \in V_1$, rationnel sur $K'$, $f(x'_1)$ soit un vecteur de $V_2$ rationnel sur $L$; cela entraînera en effet que $f(x_1)$ est rationnel sur $L$ pour tout vecteur $x_1$ de $V_1$ rationnel sur $L$, un tel vecteur étant combinaison linéaire à coefficients dans $L$ de vecteurs rationnels sur $K'$. La condition précédente équivaut, d’après la première partie du raisonnement, à la relation

(4)
$$
f(x'_1).\varphi(\eta) = \varphi_{V_2}(f(x'_1).\eta) \quad \text{pour } \varphi \in \mathcal{M} \text{ et } \eta \in K
$$

ce qui s’écrit aussi

(5)
$$
f(\varphi_{V_1}(x'_1.\eta)) = \varphi_{V_2}(f(x'_1.\eta)) \quad \text{pour } \varphi \in \mathcal{M} \text{ et } \eta \in K.
$$

Comme tout élément de $V_1$ est combinaison linéaire à coefficients dans $K$ d’éléments de $V_1$ rationnels sur $K'$, la condition (5) équivaut à $f(\varphi_{V_1}(x_1)) = \varphi_{V_2}(f(x_1))$ pour tout $x_1 \in V_1$ et tout $\varphi \in \mathcal{M}$.

Enfin, pour prouver la seconde assertion de (i), utilisons le lemme 1 de II, p. 124: W est le graphe d’une application K-linéaire $g : W_1 \to W_2$ et W est rationnel sur $L$ si et seulement si l’application $g$ est rationnelle sur $L$ (II, p. 122, prop. 4). D’après (ii), pour que $g$ soit rationnelle sur $L$, il faut et il suffit que $g(\varphi_{W_1}(x_1)) = \varphi_{W_2}(g(x_1))$ pour tout $x_1 \in W_1$ et tout $\varphi \in \mathcal{M}$; comme $\varphi_v = \varphi_{W_1} \times \varphi_{W_2}$, la condition précédente signifie que le graphe W de $g$ est stable par $\varphi_v$ pour tout $\varphi \in \mathcal{M}$.

C. Q. F. D.

## EXERCICES {#alg-ii-s8-exercises}

See the [exercises for § 8](exercises/s8/).
