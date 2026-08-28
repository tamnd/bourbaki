---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VI
chapter_title: Systèmes de racines
section: 3
section_title: Invariants exponentiels
lang: fr
source: lie-iv-vi-fr
pdf_pages: 0180-0187, 0227-0227
extraction: ocr
subsections:
    - "no": 1
      title: L’algèbre d’un groupe commutatif libre
      page: 0
      pdf_page: 180
    - "no": 2
      title: Cas du groupe des poids; termes maximaux
      page: 0
      pdf_page: 182
    - "no": 3
      title: Éléments anti-invariants
      page: 0
      pdf_page: 182
    - "no": 4
      title: Éléments invariants
      page: 0
      pdf_page: 185
statements: 15
exercises: 2
content_sha256: 49437c544b71618efc5dd3ff3097a1aad64022cb699760034bd6e58a21ac0971
---

## § 3. Invariants exponentiels

Dans ce paragraphe, la lettre $A$ désigne un anneau commutatif, ayant un élément unité, non réduit à 0.

### 1. L’algèbre d’un groupe commutatif libre

Soit $P$ un $\mathbf{Z}$-module libre de rang fini $l$. Nous noterons $A[P]$ l’algèbre du groupe additif $P$ sur $A$ (Alg., chap. III, 3e éd., § 2, no 6). Pour tout $p \in P$, notons $e^p$ l’élément correspondant de $A[P]$. Alors $(e^p)_{p \in P}$ est une base du $A$-module $A[P]$, et, quels que soient $p, p' \in P$, on a :

$$
e^p e^{p'} = e^{p+p'}, \qquad (e^p)^{-1} = e^{-p}, \qquad e^0 = 1.
$$

#### Lemme 1 {#lie-vi-s3-lem-1 .statement}

Supposons $A$ factoriel (Alg. comm., chap. VII, § 3, no 1, déf. 1).

(i) L’anneau $A[P]$ est factoriel.

(ii) Si $u, v$ sont des éléments non proportionnels de $P$, les éléments $1 - e^u, 1 - e^v$ de $A[P]$ sont étrangers.

Soient $(p_1, p_2, \ldots, p_l)$ une base de $P$, et $X_1, X_2, \ldots, X_l$ des indéterminées. L’application $A$-linéaire de $A[X_1, \ldots, X_l, X_1^{-1}, \ldots, X_l^{-1}]$ sur $A[P]$ qui transforme $X_1^{n_1} X_2^{n_2} \ldots X_l^{n_l}$ (où $n_1, n_2, \ldots, n_l \in \mathbf{Z}$) en $e^{n_1 p_1 + \cdots + n_l p_l}$ est un isomorphisme d’anneaux. Or $A[X_1, \ldots, X_l]$ est un anneau factoriel (Alg. comm., chap. VII, § 3, no 5), et $A[X_1, \ldots, X_l, X_1^{-1}, \ldots, X_l^{-1}]$ est un anneau de fractions de $A[X_1, \ldots, X_l]$, donc est factoriel.

Soit $P'$ (resp. $P''$) l’ensemble des éléments de $P$ dont un multiple appartient à $\mathbf{Z}u + \mathbf{Z}v$ (resp. à $\mathbf{Z}u$). Alors les groupes $P/P'$ et $P'/P''$ sont sans torsion, donc il existe un supplémentaire de $P''$ dans $P'$ et un supplémentaire de $P'$ dans $P$. Par suite, il existe une base $(z_1, z_2, \ldots, z_l)$ du $\mathbf{Z}$-module $P$ et des entiers rationnels $j, m, n$ tels que $u = jz_1, v = mz_1 + nz_2, j > 0, n > 0$. Posant $X_i = e^{z_i}$ pour $1 \leq i \leq l$, on a donc $1 - e^u = 1 - X_1^j, 1 - e^v = 1 - X_1^m X_2^n$. Soit $K$ une clôture algébrique du corps des fractions de $A$, de sorte que $A[P]$ s’identifie à un sous-anneau de l’anneau $B = K[X_1, \ldots, X_l, X_1^{-1}, \ldots, X_l^{-1}]$. Pour toute racine $j$-ème de l’unité $z$, $1 - z X_1$ est extrémal dans

$$
K[X_1, \ldots, X_l];
$$

de plus l’idéal engendré par $1 - z X_1$ ne contient aucun monôme en les $X_i$. On en conclut que l’idéal $(1 - z X_1)B$ de $B$ est un idéal premier de hauteur 1 (Alg. comm., chap. VII, § 1, no 6), donc que $1 - z X_1$ est extrémal dans $B$. Les facteurs extrémaux de $1 - X_1^j$ dans $B$ sont donc de la forme $1 - z X_1$. Or aucun de ces facteurs ne divise $1 - X_1^m X_2^n$ dans $B$ (car l’homomorphisme $f$ de $B$ dans $B$ tel que $f(X_1) = z^{-1}, f(X_i) = X_i$ pour $i \geq 2$, vérifie

$$
f(1 - z X_1) = 0 \quad \text{et} \quad f(1 - X_1^m X_2^n) = 1 - z^{-m} X_2^n \neq 0).
$$

Ainsi, $1 - X_1^j$ et $1 - X_1^m X_2^n$ sont étrangers dans $B$. Par suite un diviseur commun de $1 - X_1^j$ et $1 - X_1^m X_2^n$ dans $A[P]$ est inversible dans $B$, donc, à la multiplication près par un élément de la forme $X_1^{k_1} X_2^{k_2} \ldots X_l^{k_l}$, est égal à un élément $a$ de $A$; en outre, $a$ doit diviser 1 dans $A$, donc être inversible dans $A$. En définitive, $1 - X_1^j$ et $1 - X_1^m X_2^n$ sont étrangers dans $A[P]$.

### 2. Cas du groupe des poids; termes maximaux

Gardons les notations du numéro précédent et soit R un système de racines réduit dans un espace vectoriel réel V. Dans la suite de ce paragraphe, nous prendrons pour P le groupe des poids de R (§ 1, no 9). Le groupe W = W(R) opère dans P, donc aussi dans l’algèbre A[P]; on a $w(e^p) = e^{w(p)}$ pour $w \in W$ et $p \in P$.

Soit C une chambre de R (§ 1, no 5) et soit B = $(\alpha_i)_{1 \leq i \leq l}$ la base correspondante de R. Nous munirons V (donc aussi P) de la structure d’ordre définie par C. Si $p, p' \in P$, on a $p \geq p'$ si et seulement si $p - p'$ est combinaison linéaire à coefficients positifs des $\alpha_i$.

#### Définition 1 {#lie-vi-s3-def-1 .statement}

Soit $x = \sum_{p \in P} x_p e^p$ un élément de A[P]. On appelle support de x l’ensemble S des $p \in P$ tels que $x_p \neq 0$ et support maximal de x l’ensemble X des éléments maximaux de S. On dit encore que le terme $x_p e^p$ pour $p \in X$ est un terme maximal de x.

#### Lemme 2 {#lie-vi-s3-lem-2 .statement}

Soit $x \in A[P]$ et soit $(x_p e^p)_{p \in X}$ la famille des termes maximaux de x. Soit $q \in P$ et soit $y \in A[P]$ tels que $e^q$ soit l’unique terme maximal de y. Alors, la famille des termes maximaux du produit xy est $(x_p e^{p+q})_{p \in X}$.

Posons $x = \sum_p x_p e^p, y = \sum_r y_r e^r$ et $xy = \sum_t z_t e^t$. On a $r \leq q$ pour tout $r \in P$ tel que $y_r \neq 0$ et $z_t = \sum_{p+r=t} x_p y_r$.

Si $t = p + q = p' + r$ avec $p \in X$ et $x_p y_r \neq 0$, on a $r \leq q$, d’où $p' \geq p$ et par suite $p' = p$. On a donc $z_{p+q} = x_p y_q = x_p \neq 0$. Ceci montre que $X + q$ est contenu dans le support du produit xy.

D’autre part, si $t = p' + r$ avec $x_p y_r \neq 0$, il existe $p \in X$ tel que $p' \leq p$ et on a $t \leq p + q$. Le support maximal de xy est donc contenu dans $X + q$. Comme deux éléments de $X + q$ ne sont pas comparables, il en résulte que $X + q$ est exactement le support maximal de xy et nous avons vu ci-dessus que $z_{p+q} = x_p$ pour $p \in X$, ce qui achève la démonstration du lemme.

#### Remarque {#lie-vi-s3-n2-rem-1 .statement}

Comme $x \neq 0$ signifie que le support maximal de x est non vide, le lemme 2 montre que $x \neq 0$ entraîne $xy \neq 0$, toutes les fois que y admet un unique terme maximal de la forme $e^q$.

### 3. Éléments anti-invariants

On conserve les notations du numéro précédent. On note $\varepsilon(w)$ le déterminant d’un élément $w \in W$. On a

$$
\varepsilon(w) = (-1)^{l(w)}
$$

la longueur $l(w)$ étant prise relativement à la famille des réflexions $s_{\alpha_i}$.

#### Définition 2 {#lie-vi-s3-def-2 .statement}

On dit qu’un élément $x \in A[P]$ est anti-invariant par $W$ si
$$
w(x) = \varepsilon(w) \cdot x
$$
pour tout $w \in W$.

Les éléments anti-invariants de $A[P]$ forment un sous-A-module de $A[P]$. Pour tout $x \in A[P]$, on pose :

(1)
$$
J(x) = \sum_{w \in W} \varepsilon(w) \cdot w(x).
$$

Pour $x \in A[P]$ et $w \in W$, on a :
$$
w(J(x)) = \sum_{v \in W} \varepsilon(v) \cdot wv(x) = \varepsilon(w) \sum_{v \in W} \varepsilon(v) \cdot v(x) = \varepsilon(w) \cdot J(x)
$$
et $J(x)$ est anti-invariant. D’autre part, soit $q = \mathrm{Card}(W)$. Pour tout élément anti-invariant $x$ de $A[P]$, on a $J(x) = q \cdot x$. Il en résulte que, si $q$ est inversible dans $A$, l’application $q^{-1}J$ est un projecteur de $A[P]$ sur le sous-module des éléments anti-invariants.

Soient $\varpi_1, \ldots, \varpi_l$ les poids fondamentaux correspondants à la chambre $C$. Les éléments de $P \cap \overline{C}$ (resp. $P \cap C$) sont les poids de la forme $n_1 \varpi_1 + \cdots + n_l \varpi_l$ avec $n_i \geqslant 0$ (resp. $n_i > 0$) pour $1 \leqslant i \leqslant l$ (§ 1, no 10). D’autre part,
$$
\rho = \varpi_1 + \cdots + \varpi_l
$$
est la demi-somme des racines positives (*loc. cit.*) et les éléments de $P \cap C$ sont encore les poids de la forme $\rho + p$ avec $p \in P \cap \overline{C}$. Enfin, si $p \in P \cap C$, on a $w(p) < p$ pour tout $w \neq 1$ (§ 1, no 6, cor. à la prop. 18) et $e^p$ est par suite l’unique terme maximal de $J(e^p)$.

#### Proposition 1 {#lie-vi-s3-prop-1 .statement}

Si 2 n’est pas diviseur de zéro dans $A$, les éléments $J(e^p)$ pour $p \in P \cap C$ forment une base du module des éléments anti-invariants de $A[P]$.

Les poids $w(p)$ pour $w \in W$ et $p \in P \cap C$ sont deux à deux distincts. Il en résulte que les $J(e^p)$ pour $p \in P \cap C$ sont linéairement indépendants.

Soit d’autre part $x = \sum_p x_p e^p$ un élément anti-invariant de $A[P]$. Si $p_0$ appartient à un mur, il est invariant par une réflexion $s \in W$ et l’on a
$$
x = \sum_p x_p e^p = -s(x) = -\sum_p x_p e^{s(p)}.
$$
On en déduit $2x_{p_0} = 0$, d’où $x_{p_0} = 0$. Comme tout élément n’appartenant à aucun mur s’écrit d’une façon unique sous la forme $w(p)$ avec $w \in W$ et $p \in P \cap C$, on a par suite :

(2)
$$
x = \sum_{p \in P \cap C} \sum_{w \in W} x_{w(p)} e^{w(p)}.
$$

Comme $w(x) = \sum_p x_p e^{w(p)} = \varepsilon(w) \sum_p x_p e^p$, on a $x_{w(p)} = \varepsilon(w)x_p$ et on déduit de (2) que
$$
x = \sum_{p \in P \cap C} x_p J(e^p),
$$
ce qui achève la démonstration.
Considérons maintenant l’élément $d$ de l’algèbre $A[\frac{1}{2} P]$ défini par
$$
(3)
\begin{align*}
d &= \prod_{\alpha \in \mathbf{R}, \alpha > 0} (e^{\alpha/2} - e^{-\alpha/2}) \\
&= e^\rho \cdot \prod_{\alpha \in \mathbf{R}, \alpha > 0} (1 - e^{-\alpha}) \\
&= e^{-\rho} \cdot \prod_{\alpha \in \mathbf{R}, \alpha > 0} (e^\alpha - 1).
\end{align*}
$$
Puisque $\rho \in P$, on a $d \in A[P]$.

#### Proposition 2 {#lie-vi-s3-prop-2 .statement}

(i) *L’élément d défini par (3) est un élément anti-invariant de A[P]; son unique terme maximal (n° 2, déf. 1) est $e^\rho$ et l’on a $d = J(e^\rho)$.*
(ii) *Pour tout $p \in P$, l’élément $J(e^p)$ est divisible de façon unique par d et le quotient $J(e^p)/d$ est un élément de A[P] invariant par W.*
(iii) *Si 2 n’est pas diviseur de zéro dans A, la multiplication par d est une bijection de l’ensemble des éléments de A[P] invariants par W sur l’ensemble des éléments anti-invariants de A[P].*

On sait que, pour $1 \leq i \leq l$, la réflexion $s_i = s_{\alpha_i}$ laisse stable l’ensemble des racines positives distinctes de $\alpha_i$ et que $s_i(\alpha_i) = -\alpha_i$ (§ 1, n° 6, cor. 1 de la prop. 17). On a donc
$$
s_i(d) = (e^{-x_i/2} - e^{x_i/2}) \cdot \sum_{\alpha \in \mathbf{R}, \alpha > 0, \alpha \neq \alpha_i} (e^{\alpha/2} - e^{-\alpha/2})
$$
$$
= -d = \varepsilon(s_i) \cdot d.
$$
Comme les $s_i$ engendrent W, ceci démontre la première assertion de (i). La deuxième assertion de (i) résulte aussitôt de (3) et du lemme 2, compte tenu de ce que 1 est l’unique terme maximal de $1 - e^{-\alpha}$ pour $\alpha \in \mathbf{R}, \alpha > 0$.

Supposons maintenant que $A = \mathbf{Z}$. D’après la prop. 1, on a:
$$
(4) \quad d = \sum_{p \in P \cap C} c_p J(e^p) \quad \text{avec} \quad c_p \in \mathbf{Z}.
$$
D’autre part, on vient de voir que
$$
(5) \quad d = e^\rho + \sum_{q < \rho} c_q' e^q.
$$
Si $p \in P \cap C$ avec $p \neq \rho$, on a $p > \rho$ et le coefficient de $e^p$ dans $d$ est nul d’après (5). On a donc $c_p = 0$. De plus, la comparaison des coefficients de $e^\rho$ dans (4) et (5) montre que $c_\rho = 1$ et par suite $d = J(e^\rho)$.

Supposons toujours $A = \mathbf{Z}$. Soient $p \in P, \alpha \in \mathbf{R}$ et M un système de représentants des classes à droite de W suivant le sous-groupe $\{1, s_\alpha\}$. On a:

$$
J(e^p) = \sum_{w \in M} \varepsilon(w) e^{w(p)} + \sum_{w \in M} \varepsilon(s_\alpha w) e^{s_\alpha w(p)}.
$$

Or $s_\alpha w(p) = w(p) - \langle \alpha^\vee, w(p) \rangle \alpha = w(p) + n_w \alpha$, avec $n_w \in \mathbf{Z}$. Donc

$$
J(e^p) = \sum_{w \in M} \varepsilon(w) e^{w(p)} (1 - e^{n_w \alpha}).
$$

Si $n_w \geq 0$, il est clair que $1 - e^{n_w \alpha}$ est divisible par $1 - e^\alpha$ et ceci est encore vrai pour $n_w < 0$ puisque $1 - e^{n_w \alpha} = -e^{n_w \alpha} (1 - e^{-n_w \alpha})$. Par suite, $J(e^p)$ est divisible par $1 - e^\alpha$ dans $\mathbf{Z}[P]$.

D'après le lemme 1, $\mathbf{Z}[P]$ est factoriel et les éléments $1 - e^\alpha$ pour $\alpha \in \mathbf{R}$ et $\alpha > 0$ sont deux à deux étrangers. Il s'ensuit que $J(e^p)$ est divisible dans $\mathbf{Z}[P]$ par le produit $\prod_{\alpha > 0} (1 - e^\alpha)$, donc aussi par $d = e^{-\rho} \prod_{\alpha > 0} (e^\alpha - 1)$.

Revenons maintenant au cas général : par extension des scalaires de $\mathbf{Z}$ à $A$, on déduit de ce qui précède que $d = J(e^\rho)$ et que tout élément $J(e^p)$ est divisible par $d$. Comme $d$ admet $e^\rho$ comme unique terme maximal, la Remarque du no 2 montre qu'il existe un seul élément $y \in A[P]$ tel que $J(e^p) = dy$ et il en résulte aussitôt que $y$ est invariant par $W$, puisque $d$ et $J(e^p)$ sont anti-invariants. Ceci démontre (i) et (ii).

Enfin, si 2 n'est pas diviseur de zéro dans $A$, la Remarque du no 2 et la prop. 1 entraînent (iii).

#### Remarque 1 {#lie-vi-s3-n3-rem-1 .statement}

Si 2 n'est pas diviseur de zéro dans $A$, on vérifie aisément que $d$ est l'unique élément anti-invariant de $A[P]$ admettant $e^\rho$ comme terme maximal.

#### Remarque 2 {#lie-vi-s3-n3-rem-2 .statement}

Le lemme 2 du no 2 montre que l'unique terme maximal du quotient $J(e^p)/d$ (pour $p \in P \cap C$) est $e^{p-\rho}$.

### 4. Éléments invariants

Soit $A[P]^W$ la sous-algèbre de $A[P]$ formée des éléments invariants par $W$. Pour $p \in P$, notons $W.p$ l'orbite de $p$ par $W$, et soit $S(e^p) = \sum_{q \in W.p} e^q$ la somme des différents transformés de $e^p$ par $W$; c'est un élément invariant par $W$. Si $p \in P \cap \overline{C}$, on a $w(p) \leq p$ pour tout $w \in W$ ($§ 1$, no 6, prop. 18) et $e^p$ est l'unique terme maximal de $S(e^p)$.

Soit $x = \sum_p x_p e^p \in A[P]^W$; on a $x_{w(p)} = x_p$ pour tout $p \in P$ et tout $w \in W$. D'autre part, toute orbite de $W$ dans $P$ rencontre $P \cap \overline{C}$ en un point et un seul ($§ 1$, no 5, th. 2). Par suite, on a :

$$
x = \sum_{p \in P \cap \overline{C}} x_p S(e^p).
$$

On en déduit :

#### Lemme 3 {#lie-vi-s3-lem-3 .statement}

Le A-module $A[P]^{\mathrm{w}}$ admet pour base la famille des $S(e^p)$ pour $p \in P \cap \overline{C}$.

Plus généralement :

#### Proposition 3 {#lie-vi-s3-prop-3 .statement}

Pour tout $p \in P \cap \overline{C}$, soit $x_p$ un élément de $A[P]^{\mathrm{w}}$ ayant pour unique terme maximal $e^p$. La famille $(x_p)_{p \in P \cap \overline{C}}$ est une base du A-module $A[P]^{\mathrm{w}}$.

Démontrons tout d’abord un lemme :

#### Lemme 4 {#lie-vi-s3-lem-4 .statement}

Soit I un ensemble ordonné vérifiant la condition suivante :
(MIN) Toute partie non vide de I contient un élément minimal.
Soient E un A-module, $(e_i)_{i \in I}$ une base de E et $(x_i)_{i \in I}$ une famille d’éléments de E telle que
$$
x_i = e_i + \sum_{j < i} a_{ij} e_j,
$$
pour tout $i \in I$ (avec $a_{ij} \in A$, le support de la famille $(a_{ij})$ étant fini pour tout $i$). Alors $(x_i)_{i \in I}$ est une base de E.

Pour toute partie J de I, soit $E_J$ le sous-module de E de base $(e_i)_{i \in J}$. Soit $\mathcal{S}$ l’ensemble des parties J de I possédant les deux propriétés suivantes :
(a) Si $i' \leq i$ et $i \in J$, on a $i' \in J$;
(b) $(x_i)_{i \in J}$ est une base de $E_J$.

On vérifie immédiatement que $\mathcal{S}$, ordonné par inclusion, est inductif et non vide. Il possède donc un élément maximal J. Si $J \neq I$, soit $i_0$ un élément minimal de $I - J$ et posons $J' = J \cup \{i_0\}$. Tout élément $i \in I$ tel que $i < i_0$ appartient alors à J : on en déduit que $J'$ satisfait à (a). D’autre part, $J'$ satisfait aussi à (b); en effet, on a
$$
e_{i_0} = x_{i_0} - \sum_{j < i_0} a_{i_0 j} e_j
$$
d’où (b). Par suite $J' \in \mathcal{S}$, d’où une contradiction. On a donc $J = I$, ce qui démontre le lemme.

Démontrons maintenant la prop. 3. Nous allons appliquer le lemme 4, avec $I = P \cap \overline{C}$. Soit $q \in I$, et soit $I_q$ l’ensemble des $p \in I$ tels que $p \leq q$. Si $p \in I_q$, les relations
$$
q - p \geq 0, \quad p \in \overline{C}, \quad q \in \overline{C}
$$
entraînent
$$
(q - p|p) \geq 0 \quad \text{et} \quad (q - p|q) \geq 0,
$$
d’où
$$
(p|p) \leq (p|q) \leq (q|q).
$$

L’ensemble $I_q$ est donc borné. Comme I est discret, il s’ensuit que $I_q$ est fini, et il est clair que I satisfait à la condition (MIN). D’autre part, pour tout $p \in I$, on a
$$
x_p = e^p + \sum_{q < p} c_{pq} e^q
$$

d’où aussi d’après (6)

$$
x_p = S(e^p) + \sum_{q < p,\ q \in I} c_{pq} S(e^q).
$$

La proposition résulte alors des lemmes 3 et 4.

#### Théorème 1 {#lie-vi-s3-thm-1 .statement}

Soient $\omega_1, \ldots, \omega_l$ les poids fondamentaux correspondant à la chambre $C$ et, pour $1 \leq i \leq l$, soit $x_i$ un élément de $A[P]^w$ admettant $e^{\omega_i}$ pour unique terme maximal. Soit

$$
\varphi : A[X_1, \ldots, X_l] \to A[P]^w
$$

l’homomorphisme de l’algèbre de polynômes $A[X_1, \ldots, X_l]$ dans $A[P]^w$ qui applique $X_i$ sur $x_i$. L’application $\varphi$ est un isomorphisme.

Le lemme 2 entraîne que l’image par $\varphi$ du monôme $X_1^{n_1} \cdots X_l^{n_l}$ est un élément admettant comme unique terme maximal $e^{n_1 \omega_1 + \cdots + n_l \omega_l}$. Comme tout élément de $P \cap \overline{C}$ s’écrit de façon unique sous la forme $n_1 \omega_1 + \cdots + n_l \omega_l$, la prop. 3 montre que les images par $\varphi$ des monômes $X_1^{n_1} \cdots X_l^{n_l}$ forment une base de $A[P]^w$, d’où le théorème.

#### Exemple 1 {#lie-vi-s3-n4-exa-1 .statement}

On peut prendre $x_i = S(e^{\omega_i})$.

#### Exemple 2 {#lie-vi-s3-n4-exa-2 .statement}

D’après la Remarque 2 du no 3, on peut prendre $x_i = J(e^p + \omega_i)/d$ (avec les notations du no 3).

## EXERCICES {#lie-vi-s3-exercises}

Les notations et hypothèses sont celles des n° 2, 3, 4.

See the [exercises for § 3](exercises/s3/).
