---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: V
chapter_title: Groupes engendrés par des réflexions
section: 2
section_title: Réflexions
lang: fr
source: lie-iv-vi-fr
pdf_pages: 0065-0071, 0126-0126
extraction: ocr
subsections:
    - "no": 1
      title: Pseudo-réflexions
      page: 0
      pdf_page: 65
    - "no": 2
      title: Réflexions
      page: 0
      pdf_page: 66
    - "no": 3
      title: Réflexions orthogonales
      page: 0
      pdf_page: 67
    - "no": 4
      title: Réflexions orthogonales dans un espace affine euclidien
      page: 0
      pdf_page: 68
    - "no": 5
      title: Compléments sur les rotations planes
      page: 0
      pdf_page: 69
statements: 16
exercises: 3
content_sha256: f16537357b899952237ff7885a09e6217a02895a46b577fde6d07b82206db25b
---

## § 2. Réflexions

Dans ce paragraphe, on désigne par K un corps commutatif, supposé de caractéristique $\neq 2$ à partir du n° 2. On note V un espace vectoriel sur K.

### 1. Pseudo-réflexions

#### Définition 1 {#lie-v-s2-def-1 .statement}

On dit qu’un endomorphisme s de l’espace vectoriel V est une pseudo-réflexion si $1 - s$ est de rang 1.

Soit s une pseudo-réflexion dans V, et soit D l’image de $1 - s$. Par définition, D est de dimension 1 ; étant donné $a \neq 0$ dans D, il existe donc une forme linéaire non nulle $a^*$ sur V telle que $x - s(x) = \langle x, a^* \rangle . a$ pour tout x dans V.

Réciproquement, étant donnés $a \neq 0$ dans V et une forme linéaire $a^* \neq 0$ sur V, la formule

$$
s_{a, a^*}(x) = x - \langle x, a^* \rangle . a \quad (x \in V)
$$

définit une pseudo-réflexion $s_{a, a^*}$; l’image de $1 - s_{a, a^*}$ est engendrée par a et le noyau de $1 - s_{a, a^*}$ est l’hyperplan de V formé des x tels que $\langle x, a^* \rangle = 0$

Si V* est le dual de V, il est immédiat que l’endomorphisme $s_{a^*, a}$ de V* transposé de $s_{a, a^*}$ est la pseudo-réflexion définie par la formule :

$$
s_{a^*, a}(x^*) = x^* - \langle x^*, a \rangle . a^* \quad (x^* \in V^*).
$$

Si a est un vecteur non nul, on appelle pseudo-réflexion de vecteur a toute pseudo-réflexion s telle que a appartienne à l’image de $1 - s$. On appelle hyperplan d’une pseudo-réflexion s le noyau de $1 - s$, ensemble des vecteurs x tels que $s(x) = x$.

#### Proposition 1 {#lie-v-s2-prop-1 .statement}

Soient G un groupe et $\rho$ une représentation linéaire irréductible de G dans un espace vectoriel V ; on suppose qu’il existe un élément g de G tel que $\rho(g)$ soit une pseudo-réflexion.

(i) Tout endomorphisme de V commutant à $\rho(G)$ est une homothétie, et $\rho$ est absolument irréductible.

(ii) Supposons V de dimension finie. Soit B une forme bilinéaire non nulle sur V invariante par $\rho(G)$. Alors B est non dégénérée, symétrique ou antisymétrique, et toute forme bilinéaire sur V invariante par $\rho(G)$ est proportionnelle à B.

Soit u un endomorphisme de V commutant à $\rho(G)$. Soient par ailleurs g un élément de G tel que $\rho(g)$ soit une pseudo-réflexion, et D l’image de $1 - \rho(g)$. Comme D est de dimension 1 et que $u(D) \subset D$, il existe $\alpha$ dans K tel que $u - \alpha . 1$ s’annule sur D ; le noyau N de $u - \alpha . 1$ est alors un sous-espace vectoriel de V stable par $\rho(G)$, non nul puisqu’il contient D ; comme $\rho$ est irréductible, on a $N = V$ et $u = \alpha . 1$. La deuxième partie de (i) résulte de la première d’après Alg., chap. VIII, § 13, n° 4, cor. de la prop. 5.

Soit N (resp. N') le sous-espace de V formé des x tels que B(x, y) = 0 (resp. B(y, x) = 0) pour tout y dans V; comme B est invariante par ρ(G), les sous-espaces N et N' de V sont stables par ρ(G) et distincts de V puisque B ≠ 0. Puisque ρ est irréductible, on a N = N' = 0, et B est donc non dégénérée.

Comme V est de dimension finie, toute forme bilinéaire sur V est donnée par la formule

(3)
$$
B'(x, y) = B(u(x), y)
$$
où u est un endomorphisme convenable de V. Si B' est invariante par ρ(G), l’endomorphisme u commute à ρ(G). Soient en effet x, y dans V et g dans G; comme B et B' sont invariantes par ρ(G), on a
$$
\begin{align*}
B(u(\rho(g)(x)), y) &= B'(\rho(g)(x), y) = B'(x, \rho(g^{-1})(y)) \\
&= B(u(x), \rho(g^{-1})(y)) = B(\rho(g)(u(x)), y),
\end{align*}
$$
d’où $u(\rho(g)(x)) = \rho(g)(u(x))$ puisque B est non dégénérée. D’après (i), il existe α dans K avec $u = \alpha . 1$, d’où $B' = \alpha . B$.

Appliquons ceci en particulier à la forme bilinéaire $B'(x, y) = B(y, x)$; on a alors $B(y, x) = \alpha . B(x, y) = \alpha^2 . B(y, x)$ quels que soient x, y dans V, et comme B est non nulle, on a $\alpha^2 = 1$, d’où $\alpha = 1$ ou $\alpha = -1$. Donc B est symétrique ou antisymétrique.

### 2. Réflexions

On rappelle que sauf mention expresse du contraire, le corps K est désormais supposé de caractéristique différente de 2. On appellera réflexion dans V toute pseudo-réflexion s telle que $s^2 = 1$; si s est une réflexion, on notera $V_s^+$ le noyau de $s - 1$ et $V_s^-$ celui de $s + 1$.

#### Proposition 2 {#lie-v-s2-prop-2 .statement}

Soit s un endomorphisme de V.

(i) Si s est une réflexion, V est somme directe de l’hyperplan $V_s^+$ et de la droite $V_s$.

(ii) Réciproquement, supposons que V soit somme directe d’un hyperplan H et d’une droite D tels que $s(x) = x$ et $s(y) = -y$ pour $x \in H$ et $y \in D$. Alors s est une réflexion, et l’on a $H = V_s^+$ et $D = V_s^-$. Enfin, D est l’image de $1 - s$.

(i) Si s est une réflexion, $V_s^+$ est un hyperplan. Si x appartient à $V_s^+ \cap V_s^-$, on a $x = s(x) = -x$, d’où $x = 0$ puisque K est de caractéristique $\neq 2$. Enfin, pour tout x dans V, le vecteur $x' = s(x) + x$ (resp. $x'' = s(x) - x$) appartient à $V_s^+$ (resp. $V_s^-$) puisque $s^2 = 1$, et l’on a $2x = x' - x''$. Donc V est somme directe de $V_s^+$ et de $V_s^-$, et $V_s^-$ est nécessairement de dimension 1 puisque $V_s^+$ est un hyperplan.

(ii) Sous les hypothèses faites, tout élément de V s’écrit de manière unique sous la forme $v = x + y$ avec $x \in H$ et $y \in D$ et l’on a $s(v) = x - y$; l’assertion (ii) résulte immédiatement de là.

#### Corollaire {#lie-v-s2-n2-cor-1 .statement}

Si V est de dimension finie, toute réflexion est de déterminant — 1.

Soit s une réflexion dans V. La prop. 2, (i) montre qu’il existe une base $(e_1, \ldots, e_n)$ de V telle que $s(e_1) = e_1, \ldots, s(e_{n-1}) = e_{n-1}$ et $s(e_n) = -e_n$, d’où $\det s = -1$.

#### Proposition 3 {#lie-v-s2-prop-3 .statement}

*Soit s une réflexion dans V.*

(i) *Pour qu’un sous-espace $V'$ de V soit stable par s, il faut et il suffit que l’on ait $V_s^- \subset V'$ ou $V' \subset V_s^+$.*

(ii) *Pour qu’un endomorphisme u de V commute à s, il faut et il suffit que $V_s^+$ et $V_s^-$ soient stables par u.*

(i) Si $V' \subset V_s^+$, on a $s(x) = x$ pour tout $x$ dans $V'$, d’où $s(V') \subset V'$. Supposons $V_s^- \subset V'$; pour tout $x$ dans $V'$, on a $s(x) - x \in V_s^- \subset V'$, d’où $s(x) \in V'$; on a encore $s(V') \subset V'$. Réciproquement, supposons que l’on ait $s(V') \subset V'$; si l’on a $V' \not\subset V_s^+$, il existe $x$ dans $V'$ avec $s(x) \neq x$; le vecteur non nul $a = s(x) - x$ appartient à la droite $V_s^-$, donc engendre cet espace; comme on a $a \in V'$, on a $V_s^- \subset V'$.

(ii) Supposons d’abord que $u$ commute à $s$. Si $x$ est un vecteur tel que $s(x) = \varepsilon \cdot x$ (où $\varepsilon = \pm 1$), on a $s(u(x)) = u(s(x)) = \varepsilon \cdot u(x)$, donc $V_s^+$ et $V_s^-$ sont stables par $u$. Réciproquement, supposons $V_s^+$ et $V_s^-$ stables par $u$; il est clair que $us - su$ est nul dans $V_s^+$ et dans $V_s^-$, et comme $V$ est somme directe de $V_s^+$ et $V_s^-$, on a $us - su = 0$.

#### Corollaire {#lie-v-s2-n2-cor-2 .statement}

*Pour que deux réflexions distinctes s et u soient permutables, il faut et il suffit que l’on ait $V_s^- \subset V_u^+$ et $V_u^- \subset V_s^+$.*

Si l’on a $V_s^- \subset V_u^+$ et $V_u^- \subset V_s^+$, la prop. 3, (i) montre que $V_u^+$ et $V_u^-$ sont stables par $s$, d’où $su = us$ d’après la prop. 3, (ii).

Réciproquement, si l’on a $su = us$, le sous-espace $V_s^-$ est stable par $u$ d’après (ii); d’après (i), il y a donc deux cas possibles :

a) On a $V_u^- \subset V_s^-$: ces deux espaces étant de dimension 1 sont donc égaux, d’où $V_s^- \not\subset V_u^+$; comme $V_u^+$ est stable par $s$, on a donc $V_u^+ \subset V_s^+$, et ces deux hyperplans sont égaux. D’où $s = u$, ce qui est exclu.

b) On a $V_s^- \subset V_u^+$: l’image de $1 - s$ est donc contenue dans le noyau de $1 - u$, d’où $(1 - u)(1 - s) = 0$. Comme $u$ et $s$ commutent, on a aussi $(1 - s)(1 - u) = 0$, c’est-à-dire $V_u^- \subset V_s^+$.

#### Remarque {#lie-v-s2-n2-rem-1 .statement}

Soit $a \neq 0$ dans $V$ et soit $a^*$ une forme linéaire non nulle sur $V$: de la formule (1), on déduit

$$
s_a^{2}, a^*(x) = x + (\langle a, a^* \rangle - 2)\langle x, a^* \rangle \cdot a
$$

et par suite $s_a, a^*$ est une réflexion si et seulement si l’on a $\langle a, a^* \rangle = 2$. Dans ces conditions, on a alors $s_a, a^*(a) = -a$.

### 3. Réflexions orthogonales

Supposons V de dimension finie. Soit B une forme bilinéaire non dégénérée sur V. D’après Alg., chap. IX, § 6, no 3, prop. 4, pour qu’une réflexion s dans n° 2.4.

V laisse B invariante, il faut et il suffit que les sous-espaces $V_s^+$ et $V_s^-$ de V soient orthogonaux pour B; ils sont alors non isotropes. De plus, pour tout hyperplan non isotrope H dans V, il existe une réflexion s et une seule qui conserve B et induise l’identité sur H; c’est la symétrie par rapport à H, cf. Alg., chap. IX, § 6, n° 3. Si a est un vecteur non nul orthogonal à H, on a alors $B(a, a) \neq 0$, et la réflexion s est donnée par la formule

$$
s(x) = x - 2 \frac{B(x, a)}{B(a, a)} \cdot a \quad \text{pour tout } x \in V,
$$

d’après Alg., chap. IX, § 6, n° 4, formule (6). On dit aussi que s est la réflexion orthogonale par rapport à H.

#### Proposition 4 {#lie-v-s2-prop-4 .statement}

On suppose V de dimension finie. Soient B une forme bilinéaire symétrique non dégénérée sur V, X un sous-espace de V et $X^0$ l’orthogonal de X par rapport à B; enfin soit s la réflexion orthogonale par rapport à un hyperplan non isotrope H de V. Les conditions suivantes sont équivalentes :

(i) X est stable par s.
(ii) $X^0$ est stable par s.
(iii) H contient X ou $X^0$.

On a $V_s^+ = H$, et d’après ce qu’on a rappelé, $V_s^-$ est l’orthogonal $H^0$ de H par rapport à B. Pour que X soit stable par s, il faut et il suffit d’après la prop. 3, (i) que l’on ait $X \subset H$ ou $H^0 \subset X$; mais la relation $H^0 \subset X$ équivaut à $X^0 \subset H$ d’après Alg., chap. IX, § 1, n° 6, cor. 1 de la prop. 4. On a donc prouvé l’équivalence de (i) et (iii); celle de (ii) et (iii) s’en déduit en échangeant les rôles de X et $X^0$, car $(X^0)^0 = X$.

### 4. Réflexions orthogonales dans un espace affine euclidien

Conservons les notations du numéro précédent, et soit E un espace affine dont V est l’espace des translations. La donnée de la forme B sur V munit E d’une structure d’espace euclidien (Alg., chap. IX, § 6, n° 6).

Soit H un hyperplan non isotrope de E. La symétrie par rapport à H (Alg., chap. IX, § 6, n° 6) s’appelle aussi la réflexion orthogonale par rapport à H; on la note souvent $s_H$. On a $s_H^2 = 1$, et $s_H$ est l’unique déplacement (loc. cit., déf. 3) de E, distinct de l’identité, et laissant fixes les éléments de H. L’automorphisme de V associé à $s_H$ est la réflexion orthogonale par rapport à la direction de H (qui est un hyperplan non isotrope de V).

Tout $x \in E$ s’écrit de façon unique $x = h + v$, avec $h \in H$, et $v \in V$ orthogonal à H; on a

$$
s_H(h + v) = h - v.
$$

#### Proposition 5 {#lie-v-s2-prop-5 .statement}

Soient H et H’ deux hyperplans de E parallèles et non isotropes Il existe un unique vecteur $v \in V$, orthogonal à H, et tel que $H' = H + v$. Le déplacement $s_{H'} s_H$ est la translation de vecteur $2v$.

L’existence et l’unicité de $v$ sont immédiates. L’automorphisme de $V$ associé à $s_{H'} s_H$ est l’identité; donc $s_{H'} s_H$ est une translation. D’autre part, soit $a \in H'$; on a $a - v \in H$ et

$$
s_{H'} s_H (a - v) = s_{H'} (a - v) = a + v = (a - v) + 2v,
$$

ce qui montre que $s_{H'} s_H$ est la translation de vecteur $2v$.

#### Corollaire {#lie-v-s2-n4-cor-1 .statement}

*Soient $H$ et $H'$ deux hyperplans parallèles, distincts et non isotropes. Si $K$ est de caractéristique zéro (resp. $p > 0$, avec $p \neq 2$) le groupe de déplacements de $E$ engendré par $s_H$ et $s_{H'}$ est un groupe diédral infini* (resp. *d’ordre $2p$*).

En effet, d’après la prop. 2 du chap. IV, § 1, no 2, il suffit de vérifier que $s_{H'} s_H$ est d’ordre infini (resp. d’ordre $p$), ce qui est évident.

#### Remarque {#lie-v-s2-n4-rem-1 .statement}

Gardons les notations de la prop. 5 et supposons de plus que $K = \mathbf{R}$. Posons $s = s_H$ et $s' = s_{H'}$. Soit $H_n$ l’hyperplan $H + n.v$ et soit $C_n$ l’ensemble des points de $E$ de la forme $a + \xi .v$ avec $a \in H$ et $n < \xi < n + 1$. Les $C_n$ sont des ensembles ouverts connexes et ils forment une partition de $E - \bigcup_n H_n$. Ce sont donc les *chambres* définies par le système $H = (H_n)_{n \in \mathbf{Z}}$ dans $E$. La translation $(s's)^n$ transforme la chambre $C = C_0$ en la chambre $C_{2n}$, et comme $s(C_0) = C_{-1}$, on a $(s's)^n s(C) = C_{2n-1}$. Il en résulte que *le groupe diédral W engendré par s et s' permut de façon simplement transitive les chambres C_n*. De plus, montrons que, *si les chambres C et w(C) sont de part et d’autre de H* (pour $w \in W$), *on a* $l(sw) = l(w) - 1$ (les longueurs étant prises par rapport à $S = \{s, s'\}$ (chap. IV, § 1, no 1)). En effet, on a alors $w(C) = C_n$ avec $n < 0$. Si $n = -2k$, on a $w = (ss')^k$ et $sw = (s's)^{k-1}s'$, d’où $l(w) = 2k$ et $l(sw) = 2k - 1$ (chap. IV, § 1, no 2, *Remarque*). Si $n = -2k - 1$, on a $w = (ss')^k s$ et $sw = (s's)^k$, d’où $l(w) = 2k + 1$ et $l(sw) = 2k$.

### 5. Compléments sur les rotations planes

Dans ce no, on désigne par $V$ un espace vectoriel réel de dimension 2, muni d’un *produit scalaire* (c’est-à-dire d’une forme bilinéaire symétrique positive non dégénérée) et d’une *orientation*. Les mesures d’angles seront prises par rapport à la base $2\pi$; la mesure principale d’un angle de demi-droites (resp. de droites) est donc un nombre réel $\theta$ tel que $0 \leq \theta < 2\pi$ (resp. $0 \leq \theta < \pi$) (*Top. gén.*, chap. VIII, § 2, no 3 et no 6). Pour tout nombre réel $\theta$, on parlera par abus de langage de l’angle $\theta$ pour désigner un angle dont une mesure est $\theta$ et on note $\rho_\theta$ la rotation d’angle $\theta$ (*Alg.*, chap. IX, § 10, no 3).

#### Proposition 6 {#lie-v-s2-prop-6 .statement}

*Soit s la réflexion orthogonale par rapport à une droite D de V. Si $\Delta$ et $\Delta'$ sont deux demi-droites d’origine O (resp. deux droites passant par O) de V, on a*:

$$
(\overline{s(\Delta)}, \overline{s(\Delta')}) \equiv - (\overline{\Delta}, \overline{\Delta'}) \pmod{2\pi} \text{ (resp. } \pmod{\pi}\text{)}.
$$

Soit $u$ une rotation transformant $\Delta$ en $\Delta'$. Comme $su$ est une transformation orthogonale de V de déterminant — 1, c’est une réflexion et l’on a donc $(su)^2 = 1$. Par suite, $u^{-1} = sus^{-1}$ transforme $s(\Delta)$ en $s(\Delta')$, d’où la proposition.

#### Corollaire {#lie-v-s2-n5-cor-1 .statement}

Soient D et D' deux droites de V et soit $\theta$ une mesure de l’angle $(\overline{D}, \overline{D'})$. On a $s_D s_D = \rho_{2\theta}$.

On sait que $s_D s_D$ est une rotation puisque son déterminant vaut 1. Soient $\Delta$ et $\Delta'$ des demi-droites d’origine 0 portées par D et D'. On a:

$$
\begin{align*}
(\Delta, s_D s_D(\Delta)) &\equiv (\Delta, s_{D'}(\Delta)) \equiv (\overline{\Delta}, \overline{\Delta'}) + (\overline{\Delta'}, s_{D'}(\overline{\Delta})) \\
&\equiv (\overline{\Delta}, \overline{\Delta'}) + (s_{D'}(\overline{\Delta'}), s_{D'}(\overline{\Delta})) \\
&\equiv (\overline{\Delta}, \overline{\Delta'}) - (\overline{\Delta'}, \overline{\Delta}) \equiv 2(\overline{\Delta}, \overline{\Delta'}) \pmod{2\pi}
\end{align*}
$$

d’où le corollaire.

Soient maintenant $\Delta$ et $\Delta'$ deux demi-droites de V telles que

$$
\Delta \neq \Delta' \quad \text{et} \quad \Delta \neq -\Delta',
$$

et soient $s$ et $s'$ les réflexions orthogonales par rapport aux droites D et D' contenant $\Delta$ et $\Delta'$. Soit $\theta$ la mesure principale de l’angle $(\overline{D}, \overline{D'})$. Si $\theta \in \pi \mathbf{Q}$, on désigne par $m$ le plus petit entier $\geq 1$ tel que $m\theta \in \pi \mathbf{Z}$. Si $\theta \notin \pi \mathbf{Q}$, on pose $m = \infty$. Soit W le groupe engendré par $s$ et $s'$.

#### Proposition 7 {#lie-v-s2-prop-7 .statement}

Le groupe W est un groupe diédral (chap. IV, § 1, no 2) d’ordre $2m$. Il se compose des rotations $\rho_{2n\theta}$ et des produits $\rho_{2n\theta}s$ pour $n \in \mathbf{Z}$. Les transformées de D et D' par les éléments de W sont les transformées de D par les rotations $\rho_{n\theta}$ pour $n \in \mathbf{Z}$.

Le cor. de la prop. 6 montre que $s's$ est d’ordre $m$, d’où la première assertion. Les éléments de W sont donc de la forme $(s's)^n = \rho_{2n\theta}$ ou $(s's)^n s = \rho_{2n\theta}s$; la dernière assertion en résulte, puisque $D' = \rho_\theta(D)$.

#### Corollaire {#lie-v-s2-n5-cor-2 .statement}

Soit C le secteur angulaire ouvert réunion des demi-droites ouvertes $\Delta_1$ d’origine 0 telles que $0 < (\overline{\Delta}, \overline{\Delta_1}) < \theta$. Pour qu’aucune transformée de D ou de D' par un élément de W ne rencontre C, il faut et il suffit que m soit fini et que

$$
\theta = \pi/m.
$$

Si $m = \infty$, l’image de l’ensemble des $n\theta$ ($n \in \mathbf{Z}$) est dense dans $\mathbf{R}/2\pi \mathbf{Z}$ (Top. gén., chap. VII, § 1, cor. de la prop. 11); la réunion des transformées de D par les éléments de W est donc dense dans V et rencontre C. Si $m$ est fini et si $\theta = k\pi/m$, avec $1 < k < m$, les entiers $k$ et $m$ étant étrangers, il existe un entier $h$ tel que $hk \equiv 1 \bmod{m}$; on a alors $(\overline{D}, \rho_{h\theta}(\overline{D})) \equiv \pi/m$ (mod. $\pi$), et $\rho_{h\theta}(D)$ rencontre C. Ceci montre que la condition est nécessaire. La réciproque est immédiate.

#### Remarque {#lie-v-s2-n5-rem-1 .statement}

Supposons $m$ fini et $\theta = \pi/m$. Si $n \in \mathbf{Z}$, soit $C_n$ la réunion des demi-droites ouvertes $\Delta_1$ d’origine 0 telles que

$$
n\theta < (\overline{\Delta}, \overline{\Delta_1}) < (n+1)\theta.
$$

Les $C_n$ pour $-m \leq n < m$ sont des ouverts connexes et forment une partition de $E - \bigcup_n D_n$ (en posant $D_n = \rho_{n\theta}(D)$). Ce sont donc les *chambres* déterminées dans $E$ par le système des $m$ droites $D_n$ ($1 \leq n \leq m$). On a $C_{2k} = \rho_{2k\theta}(C)$ et $C_{2k-1} = \rho_{2k\theta s}(C)$. De plus, on a $C_n = C$ si et seulement si $n \in 2m\mathbf{Z}$. Par suite, *le groupe W permuté de façon simplement transitive les chambres* $C_n$.

Montrons enfin que, *si $w \in W$ est tel que les chambres* $C$ *et* $w(C)$ *soient de part et d’autre de la droite* $D$, *on a* $l(sw) = l(w) - 1$ (les longueurs étant prises par rapport à $S = \{s, s'\}$). En effet, on a alors $w(C) = C_n$, avec $-m \leq n < 0$. Si $n = -2k$, on a $w = (ss')^k$ et $sw = s'(ss')^{k-1}$, d’où $l(w) = 2k$ et $l(sw) = 2k - 1$ (chap. IV, § 1, no 2, *Remarque*). Si $n = -2k + 1$, on a

$$
w = (ss')^{k-1}s \quad \text{et} \quad sw = (s's)^{k-1},
$$

d’où $l(w) = 2k - 1$ et $l(sw) = 2k - 2$. C.Q.F.D.

## EXERCICES {#lie-v-s2-exercises}

See the [exercises for § 2](exercises/s2/).
