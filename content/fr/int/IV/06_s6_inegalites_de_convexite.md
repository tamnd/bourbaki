---
book: int
book_title: Integration
chapter: IV
chapter_title: Prolongement d'une mesure. Espaces $L^p$
section: 6
section_title: Inégalités de convexité
lang: fr
source: int-i-iv-fr
pdf_pages: 0207-0219, 0258-0267
extraction: ocr
subsections:
    - "no": 1
      title: Le théorème de convexité
      page: 0
      pdf_page: 207
    - "no": 2
      title: L’inégalité de la moyenne
      page: 0
      pdf_page: 208
    - "no": 3
      title: Les espaces $L_F^\infty$
      page: 0
      pdf_page: 210
    - "no": 4
      title: L’inégalité de Hölder
      page: 0
      pdf_page: 212
    - "no": 5
      title: 'Application: relations entre les espaces $L^p_F$ ($1 \leqslant p \leqslant +\infty$)'
      page: 0
      pdf_page: 217
statements: 23
exercises: 20
content_sha256: 30561cfafd43a04bc8339708f13a32de4e5f4653e5d9f7b6910a8e5bfa802234
---

## § 6. Inégalités de convexité

### 1. Le théorème de convexité

#### Théorème 1 {#int-iv-s6-thm-1 .statement}

Soient $X$ un espace localement compact, $\mu$ une mesure positive sur $X$, $F$ un espace de Banach réel, $D$ un ensemble convexe fermé dans $F$, $f$ une fonction sur $X$ telle que $f(X) \subset D$. Pour toute fonction numérique intégrable $g \geq 0$ non négligeable et telle que $fg$ soit intégrable, le point $\frac{\int fg\,d\mu}{\int g\,d\mu}$ appartient à $D$.

En effet, soit $F'$ le dual de $F$, et soit $\langle z, a' \rangle \leq \alpha$ ($a' \in F', \alpha \in \mathbf{R}$) une relation définissant un demi-espace fermé contenant $D$. Comme $fg$ est intégrable, il en est de même de la fonction numérique $\langle fg, a' \rangle = \langle f, a' \rangle g$, et on a $\int \langle fg, a' \rangle\,d\mu = \left\langle \int fg\,d\mu, a' \right\rangle$ ($§ 4$, n° 2, cor. 1 du th. 1); mais par hypothèse $\langle f(x), a' \rangle \leq \alpha$ pour tout $x \in X$, donc $\langle f(x)g(x), a' \rangle \leq \alpha g(x)$; en intégrant, il vient
$$
\left\langle \int fg\,d\mu, a' \right\rangle \leq \alpha \int g\,d\mu.
$$
Cela prouve que le point $\frac{\int fg\,d\mu}{\int g\,d\mu}$ appartient à tout demi-espace fermé contenant $D$; mais en vertu du th. de Hahn-Banach, $D$ est l’intersection des demi-espaces fermés qui le contiennent (*Esp. vect. top.*, chap. II, 2e éd., § 5, n° 3, cor. 1 de la prop. 4), d’où le théorème.

#### Corollaire {#int-iv-s6-n1-cor-1 .statement}

Si la mesure positive $\mu$ est de masse totale égale à 1, et si $f$ est intégrable, $\int f d\mu$ appartient à l’enveloppe fermée convexe de $f(X)$ dans $F$.

Il suffit de prendre pour fonction $g$ la constante 1.

### 2. L’inégalité de la moyenne

Nous allons préciser le th. 1 pour les fonctions mesurables numériques (finies ou non).

#### Définition 1 {#int-iv-s6-def-1 .statement}

Soient $X$ un espace localement compact, $\mu$ une mesure sur $X$. Etant donnée une fonction numérique $f$ (finie ou non), définie localement presque partout dans $X$, on appelle maximum en mesure, ou $\mu$-maximum (resp. minimum en mesure, ou $\mu$-minimum) de la fonction $f$, et on désigne par $M_\infty(f)$ (resp. $m_\infty(f)$) la borne inférieure (resp. supérieure) de l’ensemble des nombres $\alpha$ tels que l’on ait $f(x) \leq \alpha$ (resp. $f(x) \geq \alpha$) localement presque partout (pour $\mu$).

Il résulte aussitôt que la définition que $m_\infty(f) = -M_\infty(-f)$, donc de toute propriété du maximum en mesure on déduit une propriété correspondante du minimum en mesure.

Pour tout $\alpha > M_\infty(f)$, l’ensemble des $x \in X$ tels que $f(x) > \alpha$ est localement négligeable; or, l’ensemble des $x \in X$ tels que $f(x) > M_\infty(f)$ est réunion des ensembles où $f(x) > r_n$, $r_n$ parcourant l’ensemble des nombres rationnels $> M_\infty(f)$; on a donc $f(x) \leq M_\infty(f)$ localement presque partout (§ 5, n° 2). On a de même $f(x) \geq m_\infty(f)$ localement presque partout; on en déduit que $m_\infty(f) \leq M_\infty(f)$ si la mesure $\mu$ n’est pas nulle; en outre, la relation $m_\infty(f) = M_\infty(f)$ équivaut à dire que $f$ est localement presque partout égale à une constante. Il est clair que, si la mesure $\mu$ n’est pas nulle, on a

$$
\inf_{x \in X} f(x) \leq m_\infty(f) \leq M_\infty(f) \leq \sup_{x \in X} f(x).
$$

Si deux fonctions $f, g$ sont égales localement presque partout, on a $m_\infty(f) = m_\infty(g)$ et $M_\infty(f) = M_\infty(g)$.

Enfin, si $f$ et $g$ sont deux fonctions telles que $f + g$ soit définie localement presque partout, on a

(1)
$$
M_\infty(f + g) \leq M_\infty(f) + M_\infty(g)
$$
si le second membre est défini, comme il résulte aussitôt de la déf. 1 ; de même si $f$ et $g$ sont toutes deux $\geqslant 0$, et telles que $fg$ soit définie localement presque partout, on a

(2)
$$
M_\infty(fg) \leq M_\infty(f)M_\infty(g)
$$
si le second membre est défini.

Lorsque $M_\infty(f) < +\infty$, on a $f(x) < +\infty$ localement presque partout, mais pas nécessairement presque partout. On dit qu’une fonction numérique $f$ est *bornée en mesure* (pour la mesure $\mu$) si elle est *définie et finie presque partout*, et si en outre les nombres $m_\infty(f)$ et $M_\infty(f)$ sont tous deux finis (cette dernière condition revenant à dire que $M_\infty(|f|) < +\infty$).

**Proposition 1** (inégalité de la moyenne). — *Soit $f$ une fonction numérique mesurable et bornée en mesure. Pour toute fonction numérique intégrable $g \geq 0$, la fonction $fg$ (définie presque partout) est intégrable et on a*

(3)
$$
m_\infty(f) \int |g|\,d|\mu| \leq \int |fg|\,d|\mu| \leq M_\infty(f) \int |g|\,d|\mu|.
$$

*En outre, deux des trois membres de l’inégalité (3) ne peuvent être égaux que si, dans l’ensemble des $x \in X$ où $g(x) \neq 0$, $f$ est presque partout égale à $M_\infty(f)$, ou presque partout égale à $m_\infty(f)$.

En effet, $fg$ est mesurable (§ 5, n° 3, cor. 5 du th. 1); en outre, on a l’inégalité $m_\infty(f)g(x) \leq f(x)g(x) \leq M_\infty(f)g(x)$, non seulement localement presque partout, mais même presque partout, car l’ensemble des points $x \in X$ où $g(x) \neq 0$ est réunion dénombrable d’ensembles intégrables (§ 5, n° 6, lemme 1). On en déduit que $fg$ est intégrable (§ 5, n° 6, th. 5) et on a l’inégalité (3). D’autre part, la fonction $M_\infty(f)g - fg$ est presque partout définie et égale à $(M_\infty(f) - f)g$; elle est donc presque partout $\geq 0$ dans $X$; comme la relation $M_\infty(f)\int |g|\,d|\mu| = \int |fg|\,d|\mu|$ est équivalente à $\int (M_\infty(f) - f)|g|\,d|\mu| = 0$, elle ne peut avoir lieu que si la fonction $(M_\infty(f) - f)g$ est négligeable, ce qui achève la démonstration.

En écartant le cas trivial où $\int g d|\mu| = 0$, l’inégalité (3) se déduit du th. 1 du n° 1 appliqué à l’intervalle $D = \{m_\infty(f), M_\infty(f)\}$. On peut apporter au th. 1 du n° 1 des compléments analogues à ceux de la prop. 1, qui précisent dans quel cas le point
$$
\left( \int fg\,d\mu \right) / \left( \int g\,d\mu \right)
$$
appartient à la frontière de $D$ (exerc. 2).

### 3. Les espaces $L_F^\infty$

#### Définition 2 {#int-iv-s6-def-2 .statement}

Pour toute application $f$ de $X$ dans un espace de Banach $F$, on pose $N_\infty(f) = M_\infty(|f|)$; on dit que $f$ est bornée en mesure (pour la mesure $\mu$) si $N_\infty(f)$ est fini. On désigne par $\mathcal{L}_F^\infty(X, \mu)$ (ou $\mathcal{L}_F^\infty(\mu)$, ou simplement $\mathcal{L}_F^\infty$) l’ensemble des applications mesurables et bornées en mesure de $X$ dans $F$.

Une fonction $f$ de $\mathcal{L}_F^\infty$ peut donc être caractérisée par le fait qu’il existe une fonction *mesurable et bornée* égale localement presque partout à $f$.

Il résulte aussitôt de (1) qu’on a
$$
N_\infty(f + g) \leq N_\infty(f) + N_\infty(g);
$$
d’autre part, on a $N_\infty(\alpha f) = |\alpha| N_\infty(f)$ pour tout scalaire $\alpha$. L’ensemble $\mathcal{L}_F^\infty$ est donc un *sous-espace vectoriel* de l’espace de toutes les applications de $X$ dans $F$, et $N_\infty(f)$ est une semi-norme sur cet espace vectoriel. Soit $(f_n)$ une suite de fonctions de $\mathcal{L}_F^\infty$, qui converge vers $f \in \mathcal{L}_F^\infty$ pour la topologie définie par la semi-norme $N_\infty(f)$; pour tout entier $m$, il existe un ensemble localement négligeable $H_m$ et un entier $n_0$ tels que, pour tout entier $n \geq n_0$ et tout $x \notin H_m$, on ait $|f(x) - f_n(x)| \leq 1/m$ (toute réunion dénombrable d’ensembles localement négligeables étant localement négligeable); la réunion $H$ des $H_m$ est localement négligeable, et on voit que $f_n(x)$ tend *uniformément* vers $f(x)$ dans le complémentaire de l’ensemble localement négligeable $H$; la réciproque est immédiate.

Il est clair que toute fonction égale localement presque partout à une fonction de $\mathcal{L}_F^\infty$ appartient à $\mathcal{L}_F^\infty$. En particulier, les fonctions *localement négligeables* définies dans $X$ et à valeurs dans $F$ forment un sous-espace vectoriel $\mathcal{N}_F^\infty$ de $\mathcal{L}_F^\infty$, caractérisé par la relation $N_\infty(f) = 0$ (adhérence de 0 pour la topologie définie par $N_\infty(f)$). On désigne par $L_F^\infty(X, \mu)$ (ou $L_F^\infty(\mu)$ ou $L_F^\infty$) l’espace séparé associé à $\mathcal{L}_F^\infty$, c’est-à-dire l’espace quotient $\mathcal{L}_F^\infty / \mathcal{N}_F^\infty$; sa topologie est définie par la *norme* déduite de $N_\infty$ par passage au quotient; la norme d’une classe $\dot{f} \in L_F^\infty$ s’écrit $N_\infty(\dot{f})$, ou encore $\| \dot{f} \|_\infty$. Lorsque $F = \mathbf{R}$ (resp. $\mathbf{C}$), on écrit $\mathcal{L}^\infty$ et $L^\infty$ au lieu de $\mathcal{L}_\mathbf{R}^\infty$ et $L_\mathbf{R}^\infty$ (resp. $\mathcal{L}_\mathbf{C}^\infty$ et $L_\mathbf{C}^\infty$) s’il n’en résulte pas de confusion.

#### Proposition 2 {#int-iv-s6-prop-2 .statement}

L’espace $\mathcal{L}_F^\infty$ est complet ; l’espace $L_F^\infty$ est un espace de Banach.

Soit en effet $(\mathbf{f}_n)$ une suite de Cauchy dans $\mathcal{L}_F^\infty$; pour tout entier $n$, il existe un entier $k_n$ tel que, pour $r \geq k_n$ et $s \geq k_n$, on ait $N_\infty(\mathbf{f}_r - \mathbf{f}_s) \leq 1/n$; il existe donc un ensemble localement négligeable $A_{rs}$ tel que l’on ait $|\mathbf{f}_r(x) - \mathbf{f}_s(x)| \leq 1/n$ pour tout $x \notin A_{rs}$. Si $A_n$ est la réunion des ensembles $A_{rs}$ (pour $r \geq k_n$ et $s \geq k_n$), $A_n$ est localement négligeable, et pour tout $x \notin A_n$, on a $|\mathbf{f}_r(x) - \mathbf{f}_s(x)| \leq 1/n$ pour tous les indices $r \geq k_n, s \geq k_n$. Soit $A$ l’ensemble localement négligeable réunion des $A_n$, et posons $g_n(x) = \mathbf{f}_n(x)$ pour $x \notin A$, $g_n(x) = 0$ pour $x \in A$; $g_n$ appartient à $\mathcal{L}_F^\infty$, et d’après la définition de $A$, la suite $(g_n)$ converge uniformément dans $X$ vers une fonction $g$. Il en résulte que la fonction $g$ est mesurable (§ 5, n° 4, th. 2); en outre, $g$ est bornée dans l’ensemble des $x \in X$ où $|g_{k_1}(x)| \leq N_\infty(g_{k_1})$, et comme le complémentaire de cet ensemble est localement négligeable, $g$ appartient à $\mathcal{L}_F^\infty$. Il est clair que dans $\mathcal{L}_F^\infty$, la suite $(g_n)$ a pour limite $g$, et il en est donc de même de la suite $(\mathbf{f}_n)$, puisque $N_\infty(\mathbf{f}_n - g_n) = 0$ pour tout $n$. La seconde partie de la proposition s’en déduit immédiatement.

#### Remarque 1 {#int-iv-s6-n3-rem-1 .statement}

Toute fonction $f$ continue et bornée dans $X$, à valeurs dans $F$, appartient à $\mathcal{L}_F^\infty$, et l’on a
$$
N_\infty(f) \leq \|f\| = \sup_{x \in X} |f(x)|.
$$
Pour que l’on ait $N_\infty(f) = \|f\|$ pour toute fonction continue et bornée $f$, il faut et il suffit que le support de la mesure $\mu$ soit égal à $X$. En effet, s’il existe une fonction continue $f$ à support compact négligeable et non identiquement nulle, on a $N_\infty(f) = 0$ et $\|f\| > 0$. Inversement, si le support de $\mu$ est égal à $X$, pour toute fonction continue et bornée $f$ et tout nombre $\alpha < \|f\|$, l’ensemble des $x \in X$ tels que $|f(x)| > \alpha$ est ouvert et non vide, donc de mesure extérieure $> 0$, ce qui montre que $N_\infty(f) = \|f\|$.

Lorsque le support de $\mu$ est égal à $X$, on peut donc identifier l’espace normé $C^b(X; F)$ des fonctions continues et bornées dans $X$, à valeurs dans $F$, avec un sous-espace de l’espace $\mathcal{L}_F^\infty$. Comme $\mathcal{L}_F^\infty$ n’est pas en général séparé, le sous-espace $C^b(X; F)$ n’est pas en général fermé dans $\mathcal{L}_F^\infty$, mais son image canonique dans $L_F^\infty$ est un sous-espace fermé de $L_F^\infty$ (qu’on peut d’ailleurs identifier à $C^b(X; F)$ dans le cas envisagé). En général, $C^b(X; F)$ est distinct de $L_F^\infty$, c’est-à-dire que, pour une fonction mesurable et bornée quelconque $f$, il n’existe pas en général de fonction $g$ continue et égale à $f$ localement presque partout (§ 5, exerc. 12). Cela entraîne que l’espace $\mathscr{K}(X; F)$ des applications de $X$ dans $F$, continues et à support compact, $n’est pas partout dense dans L_F^\infty$ en général, alors qu’il est partout dense dans chacun des espaces $L_F^p$ pour
$$
1 \leq p < +\infty
$$
(§ 3, n° 4, déf. 2).

#### Remarque 2 {#int-iv-s6-n3-rem-2 .statement}

Il est immédiat que la topologie définie par la semi-norme $N_\infty$ est plus fine que la topologie induite sur $\mathcal{L}_F^\infty$ par la topologie de la convergence en mesure ($§ 5, n° 11$).

### 4. L’inégalité de Hölder

Dans ce numéro, $p$ et $q$ désigneront deux nombres réels tels que $1 \leq p \leq +\infty, 1 \leq q \leq +\infty$, liés par la relation $1/p + 1/q = 1$; on a donc $q = p/(p - 1)$ si $1 < p < +\infty, \ q = +\infty$ si $p = 1$ et $q = 1$ si $p = +\infty$; $p$ et $q$ seront appelés des exposants conjugués. On remarquera que la relation $1 \leq p \leq 2$ équivaut à $2 \leq q \leq +\infty$; on n’a $p = q$ que lorsque $p$ et $q$ sont égaux à 2.

#### Théorème 2 (inégalité de Hölder) {#int-iv-s6-thm-2 .statement}

Soient $f$ et $g$ deux fonctions numériques finies presque partout et telles que $f$ soit égale presque partout à une fonction de $\mathcal{L}^p$ et $g$ à une fonction de $\mathcal{L}^q$. Alors la fonction $fg$ (définie presque partout) est intégrable, et on a

$$
N_1(fg) \leq N_p(f)N_q(g).
$$

Soit $f_1$ (resp. $g_1$) une fonction de $\mathcal{L}^p$ (resp. $\mathcal{L}^q$) à laquelle $f$ (resp. $g$) est presque partout égale; $fg$ est égale presque partout à la fonction $f_1g_1$ partout définie et finie, qui est mesurable comme produit de deux fonctions mesurables ($§ 5,$ th. 1 et 5). Si

$$
1 < p < +\infty,
$$

l’inégalité de Hölder pour l’intégrale supérieure (chap. I, n° 3, prop. 4) donne l’inégalité (4), et la relation $N_1(fg) < +\infty$ montre alors que $fg$ est intégrable ($§ 5,$ n° 6, th. 5). Si $p = 1, \ q = +\infty$, l’inégalité (4) et le fait que $fg$ soit intégrable sont des conséquences immédiates de l’inégalité de la moyenne (n° 2, prop. 1); le théorème est donc démontré dans tous les cas.

#### Corollaire 1 {#int-iv-s6-thm-2-cor-1 .statement}

Soient $F, G, H$ trois espaces de Banach, et $(\mathbf{u}, \mathbf{v}) \mapsto \Phi(\mathbf{u}, \mathbf{v})$ une application bilinéaire continue de $F \times G$ dans $H$, telle que $|\Phi(\mathbf{u}, \mathbf{v})| \leq |\mathbf{u}| \cdot |\mathbf{v}|$. Si $\mathbf{f} \in \mathcal{L}_F^p$ et $\mathbf{g} \in \mathcal{L}_G^q$, la fonction $\Phi(\mathbf{f}, \mathbf{g})$ est intégrable, et on a

$$
\left| \int \Phi(\mathbf{f}, \mathbf{g}) \, d\mu \right| \leq \int |\Phi(\mathbf{f}, \mathbf{g})| \, d|\mu| \leq N_p(\mathbf{f})N_q(\mathbf{g}).
$$

En effet, $\Phi(\mathbf{f}, \mathbf{g})$ est mesurable ($§ 5,$ n° 3, cor. 5 du th. 1); comme $|\Phi(\mathbf{f}, \mathbf{g})| \leq |\mathbf{f}| \cdot |\mathbf{g}|$, le corollaire résulte du th. 2 et du critère d’intégrabilité du $§ 5,$ n° 6, th. 5.

Deux cas particuliers du cor. 1 sont importants dans les applications :

#### Corollaire 2 {#int-iv-s6-thm-2-cor-2 .statement}

Soit F un espace de Banach réel (resp. complexe), F' son dual fort (Esp. vect. top., chap. IV, § 3), et soit (z, z') \mapsto \langle z, z' \rangle la forme bilinéaire canonique sur F × F'. Si f \in \mathcal{L}_F^p et g \in \mathcal{L}_{F'}^q, la fonction numérique (resp. complexe) $\langle f, g \rangle$ est intégrable, et on a

$$
\left| \int \langle f, g \rangle \, d\mu \right| \leq \int \left| \langle f, g \rangle \right| \, d|\mu| \leq N_p(f)N_q(g).
$$

En effet, on a $|\langle z, z' \rangle| \leq |z| \cdot |z'|$.

Lorsque F est un espace hilbertien réel ou complexe, on sait qu’on peut l’identifier canoniquement à son dual F' (Esp. vect. top., chap. V, § 1, n° 6). Comme l’espace L_F^2 est complet, on a le résultat suivant :

#### Corollaire 3 {#int-iv-s6-thm-2-cor-3 .statement}

Soient $\mu$ une mesure positive sur X, F un espace hilbertien réel (resp. complexe). Sur l’espace L_F^2, la forme symétrique (resp. hermitienne)

$$
(\tilde{f}, \tilde{g}) \mapsto \int \langle f, g \rangle \, d\mu
$$

définit une structure d’espace hilbertien, pour laquelle la norme est égale à $\| \tilde{f} \|_2$.

#### Corollaire 4 {#int-iv-s6-thm-2-cor-4 .statement}

Soient F un espace de Banach, f une fonction de $\mathcal{L}_F^p$, g une fonction numérique appartenant à $\mathcal{L}^q$; la fonction fg est intégrable et on a

$$
\left| \int fg \, d\mu \right| \leq \int |fg| \, d|\mu| \leq N_p(f)N_q(g).
$$

#### Corollaire 5 {#int-iv-s6-thm-2-cor-5 .statement}

Soient $f_1, f_2, \ldots, f_n$ n fonctions positives intégrables, $\alpha_1, \alpha_2, \ldots, \alpha_n$ n nombres > 0 tels que $\sum_{i=1}^n \alpha_i = 1$; dans ces conditions, la fonction $f_1^{\alpha_1} f_2^{\alpha_2} \ldots f_n^{\alpha_n}$ est intégrable, et on a

$$
\int f_1^{\alpha_1} f_2^{\alpha_2} \ldots f_n^{\alpha_n} \, d|\mu| \leq \left( \int f_1 \, d|\mu| \right)^{\alpha_1} \left( \int f_2 \, d|\mu| \right)^{\alpha_2} \ldots \left( \int f_n \, d|\mu| \right)^{\alpha_n}.
$$

En effet, le produit $f_1^{\alpha_1} f_2^{\alpha_2} \ldots f_n^{\alpha_n}$ est mesurable, comme produit de fonctions mesurables (§ 5, th. 5 et th. 1); l’inégalité (8) étant vraie pour les intégrales supérieures (chap. I, n° 2, cor. de la prop. 2) la fonction $f_1^{\alpha_1} f_2^{\alpha_2} \ldots f_n^{\alpha_n}$ est intégrable (§ 5, n° 6, th. 5), d’où le corollaire.

Le cor. 2 du th. 2 se précise par la proposition suivante:

#### Proposition 3 {#int-iv-s6-prop-3 .statement}

*Soient $\mu$ une mesure positive sur $X$, $F$ un espace de Banach réel ou complexe, $F'$ son dual fort, $(z, z') \mapsto \langle z, z' \rangle$ la forme bilinéaire canonique sur $F \times F'$.

1° *Pour toute fonction* $f \in \mathcal{L}_F^p (1 \leq p \leq +\infty)$, *on a*
$$
N_p(f) = \sup \left| \int \langle f, g \rangle \, d\mu \right|
$$
*lorsque* $g$ *parcourt l’ensemble des fonctions de* $\mathcal{L}_F^q$, *telles que* $N_q(g) \leq 1$.

2° *Pour toute fonction* $g \in \mathcal{L}_F^q$ (*$1 \leq q \leq +\infty$*), *on a*
$$
N_q(g) = \sup \left| \int \langle f, g \rangle \, d\mu \right|
$$
*lorsque* $f$ *parcourt l’ensemble des fonctions de* $\mathcal{L}_F^p$ *telles que* $N_p(f) \leq 1$.

Démontrons d’abord la relation (9); nous distinguerons deux cas.

1° $1 \leq p < +\infty$. La relation (9) étant triviale lorsque $N_p(f) = 0$ (car alors $f$ et $\langle f, g \rangle$ sont négligeables), on peut toujours, en multipliant $f$ par un scalaire, supposer que $N_p(f) = 1$. Supposons en premier lieu que $f$ soit une fonction *étagée* intégrable, $f = \sum_{k=1}^n a_k \varphi_{A_k}$ où les $A_k$ sont deux à deux sans point commun (§ 4, n° 8, lemme 1). On a donc par hypothèse $\sum_{k=1}^n |a_k|^p \mu(A_k) = 1$. Pour tout $\varepsilon > 0$, il existe (pour tout indice $k$) un vecteur $a'_k \in F'$ tel que $|a'_k|^q = |a_k|^p$ si $p > 1$ (resp. $|a'_k| = 1$ si $p = 1$) et $\langle a_k, a'_k \rangle \geq (1 - \varepsilon)|a_k| \cdot |a'_k|$ (*Esp. vect. top.*, chap. IV, § 5, n° 1). Si on pose $g = \sum_{k=1}^n a'_k \varphi_{A_k}$, on a
$$
\sum_{k=1}^n |a'_k|^q \mu(A_k) = 1 \text{ si } p > 1 \text{ (resp. } \sup_{1 \leq k \leq n} |a'_k| = 1 \text{ si } p = 1),
$$
donc $N_q(g) = 1$; d’autre part
$$
\int \langle f, g \rangle \, d\mu = \sum_{k=1}^n \langle a_k, a'_k \rangle \mu(A_k) \geq (1 - \varepsilon) \sum_{k=1}^n |a_k| \cdot |a'_k| \mu(A_k)
$$

et comme $|a'_k| = |a_k|^{p/q} = |a_k|^{p-1}$ si $p > 1$ (resp. $|a'_k| = 1$ si $p = 1$), on a

$$
\int \langle f, g \rangle d\mu \geq (1 - \varepsilon) \sum_{k=1}^n |a_k|^p \mu(A_k) = (1 - \varepsilon) N_p(f) = 1 - \varepsilon
$$

ce qui démontre dans ce cas la relation (9).

Passons au cas où $f$ est un élément quelconque de $\mathcal{L}_F^p$ tel que $N_p(f) = 1$. Pour tout $\varepsilon > 0$, il existe une fonction étagée $f_1 \in \mathcal{L}_F^p$ telle que $N_p(f - f_1) \leq \varepsilon$ (§ 4, n° 10, cor. 1 de la prop. 19). D’après ce que nous venons de voir, il existe une fonction $g \in \mathcal{L}_F^q$, telle que $N_q(g) = 1$ et que $\int \langle f_1, g \rangle d\mu \geq N_p(f_1) - \varepsilon \geq 1 - 2\varepsilon$. Or, on a

$$
\int \langle f, g \rangle d\mu = \int \langle f_1, g \rangle d\mu + \int \langle f - f_1, g \rangle d\mu
$$

et d’après (6),

$$
\left| \int \langle f - f_1, g \rangle d\mu \right| \leq N_p(f - f_1) N_q(g)
$$

d’où

$$
\left| \int \langle f, g \rangle d\mu \right| \geq 1 - 3\varepsilon,
$$

ce qui démontre (9).

$2^\circ$ $p = +\infty$. On peut encore se borner au cas où $N_\infty(f) > 0$. Soit $\alpha$ un nombre quelconque tel que $0 < \alpha < N_\infty(f)$; par hypothèse, l’ensemble des $x \in X$ tels que $|f(x)| > \alpha$ est mesurable et n’est pas localement négligeable, donc il contient un ensemble compact $K$ de mesure $> 0$. Comme $f$ est mesurable, il existe un ensemble compact $K_1 \subset K$, de mesure $> 0$, et tel que la restriction de $f$ à $K_1$ soit continue. Il en résulte que, pour tout $\varepsilon > 0$, il existe une partition de $K_1$ en un nombre fini d’ensembles intégrables, dans chacun desquels l’oscillation de $f$ est $\leq \varepsilon$; un au moins de ces ensembles $A$ a une mesure $> 0$. Soit $a$ une des valeurs de $f$ dans $A$; on a $|a| > \alpha$, et $|f(x) - a| \leq \varepsilon$ pour tout $x \in A$. Il existe un vecteur $a' \in F'$ tel que $|a'| = 1$ et $|\langle a, a' \rangle| \geq |a| - \varepsilon$; la fonction $g = \varphi_A \cdot a'/\mu(A)$ est intégrable et on a $N_1(g) = 1$; d’autre part, on a

$$
\int \langle f, g \rangle d\mu = \frac{1}{\mu(A)} \int \langle f, a' \rangle \varphi_A d\mu.
$$

Or, on peut écrire

$$
\int \langle f, a' \rangle \varphi_A d\mu = \langle a, a' \rangle \mu(A) + \int \langle f - a, a' \rangle \varphi_A d\mu,
$$

et comme
$$
|\langle f - a, a' \rangle \varphi_A| \leq \varepsilon \varphi_A,
$$
on voit que
$$
\left| \int \langle f, g \rangle d\mu \right| \geq |\langle a, a' \rangle| - \varepsilon \geq |a| - 2\varepsilon > \alpha - 2\varepsilon;
$$
comme $\varepsilon$ est arbitraire et $\alpha$ un nombre quelconque < $N_\infty(f)$, la relation (9) est encore démontrée dans ce cas.

On raisonne exactement de la même manière pour démontrer la relation (10), en considérant séparément le cas $1 \leq q < +\infty$, et le cas $q = +\infty$, et en utilisant le fait que, pour tout $z' \in F'$, on a $|z'| = \sup_{|z| \leq 1} |\langle z, z' \rangle|$ par définition de la norme dans $F'$.

#### Remarque 1 {#int-iv-s6-n4-rem-1 .statement}

Soit $\mathcal{E}$ un sous-espace vectoriel partout dense de $\mathcal{L}_{F'}^q$; alors la formule (9) subsiste lorsque $g$ parcourt l’intersection de $\mathcal{E}$ avec l’ensemble $B$ des fonctions de $\mathcal{L}_{F'}^q$, telles que $N_q(g) \leq 1$. Il suffit en effet de remarquer que l’intérieur $\dot{B}$ de $B$ est dense par rapport à $B$, et que $\dot{B} \cap \mathcal{E}$ est dense par rapport à $\dot{B}$, puisque $\dot{B}$ est ouvert. Cette remarque s’applique en particulier à l’ensemble $\mathcal{E} = \mathscr{K}(X; F')$ des fonctions continues à support compact (à valeurs dans $F'$) lorsque $1 \leq q < +\infty$, c’est-à-dire $1 < p \leq +\infty$. Mais dans ce cas, la formule (9) est vraie lorsque $g$ parcourt $B \cap \mathscr{K}(X; F')$, même pour $p = 1$. En effet, on peut comme ci-dessus se borner au cas où $f$ est étagée. On a vu alors que si $N_1(f) = 1$, pour tout $\varepsilon > 0$, il existe une fonction étagée $g \in \mathcal{L}_{F'}^\infty$ telle que $|g(x)| \leq 1$ pour tout $x \in X$ et que $|\int \langle f, g \rangle d\mu| \geq 1 - \varepsilon$. Il existe un nombre fini d’ensembles compacts $K_i$ deux à deux sans point commun, tels que $g$ ait une valeur constante $a'_i$ dans chacun des $K_i$ et que, si $K$ est la réunion des $K_i$, on ait $\int |f| \varphi_{CK} d\mu \leq \varepsilon$. Soit $U_i$ un voisinage de $K_i$ tel que les ensembles $U_i$ soient deux à deux sans point commun, et soit $h_i$ une application continue de $X$ dans $\{0, 1\}$, de support contenu dans $U_i$ et égale à 1 dans $K_i$. Si on pose $h = \sum a'_i h_i$, on a $h(x) = g(x)$ dans $K$ et $|h(x)| \leq 1$ dans $X$, donc
$$
\int |\langle f, h \rangle| \varphi_{CK} d\mu \leq \varepsilon
$$
et par suite $|\int \langle f, h \rangle d\mu| \geq 1 - 3\varepsilon$, ce qui prouve notre assertion. On peut faire des remarques analogues pour la formule (10).

#### Remarque 2 {#int-iv-s6-n4-rem-2 .statement}

Soient $\mu$ une mesure positive sur $X$, $f$ une fonction mesurable $\geq 0$ (finie ou non), dont le support est contenu dans une réunion dénombrable d’ensembles compacts $K_n$. On a alors, pour tout $p$ tel que $1 \leq p \leq +\infty$,
$$
N_p(f) = \sup \int^* |f g| d\mu
$$
lorsque $g$ parcourt l’ensemble des fonctions de $\mathscr{K}(X; \mathbf{R})$ telles que

N_q(g) \leq 1. En effet, la formule (11) est un cas particulier de (9) lorsque N_p(f) < +\infty, puisque alors f est équivalente à une fonction de $\mathcal{L}^p$ (§ 5, n° 6, th. 5). Si N_p(f) = +\infty, posons, pour tout entier n > 0, $f_n = \inf(n, f \varphi_{K_n})$. On a

$$
N_p(f_n) = \sup \int^* |f_n g| d\mu \leq \sup \int^* |f g| d\mu,
$$

d’où, en passant à la limite (§ 1, n° 3, th. 3), $\sup \int^* |f g| d\mu = +\infty$.

#### Corollaire {#int-iv-s6-n4-cor-1 .statement}

Soient $\mu$ une mesure positive sur X, F un espace de Banach, F' son dual fort, g une fonction quelconque de $\mathcal{L}^q_{F'}$. La forme linéaire sur $L^p_F$, déduite par passage au quotient de la forme linéaire $f \mapsto \int \langle f, g \rangle d\mu$ sur $\mathcal{L}^p_F$, est continue et a pour norme $N_q(g)$.

### 5. Application: relations entre les espaces $L^p_F$ ($1 \leqslant p \leqslant +\infty$)

#### Proposition 4 {#int-iv-s6-prop-4 .statement}

Soit f une fonction mesurable à valeurs dans un espace de Banach F; l’ensemble I des nombres p tels que 1 \leq p \leq +\infty et que N_p(f) soit finie, est vide ou est un intervalle de $\bar{\mathbf{R}}$. Si I n’est pas vide, la restriction à I de l’application p \mapsto N_p(f) est continue; en outre, si f n’est pas négligeable, log N_p(f) est une fonction convexe de 1/p dans $\bar{I}$.

Nous savons déjà (chap. I, n° 3, prop. 5) que l’ensemble J des nombres p \geq 1 finis tels que N_p(f) < +\infty est vide ou est un intervalle, et que log N_p(f) est fonction convexe de 1/p dans J (lorsque f n’est pas négligeable); cela entraîne bien entendu la continuité de p \mapsto N_p(f) dans J.

Si J est vide, on a I = \emptyset ou I = {+\infty}, et la proposition est évidente dans ce cas; on suppose désormais J non vide. La proposition est aussi évidente si f est négligeable; on suppose désormais f non négligeable. Si s \in J, on a, pour tout nombre fini p > s, $|f|^p = |f|^s |f|^{p-s}$, et l’inégalité de la moyenne montre que

(12)
$$
N_p(f) \leq (N_s(f))^{s/p}(N_\infty(f))^{(p-s)/p}.
$$

En faisant tendre p vers +\infty, il vient

(13)
$$
\lim_{p \to +\infty} \sup N_p(f) \leq N_\infty(f).
$$

Ceci prouve que, si +\infty \in I, J contient des nombres arbitrairement grands; donc I est bien un intervalle de $\bar{\mathbf{R}}$, et l’on a $\bar{I} = \bar{J}$. La proposition sera démontrée si nous prouvons que p \mapsto N_p(f) est continue dans $\bar{J}$, et il suffit de l’établir aux extrémités de J. On peut en outre supposer que J n’est pas réduit à un point. Soient r et s l’origine et l’extrémité de J ($r < s \leq +\infty$). Soit A l’ensemble (mesurable) des $x \in X$ tels que $|f(x)| \geq 1$; on a
$$
\int |f|^p d|\mu| = \int |f|^p \varphi_A d|\mu| + \int |f|^p \varphi_{\overline{C}A} d|\mu|.
$$
Lorsque $p \in J$ tend vers r, $|f|^p \varphi_A$ tend vers $|f|^r \varphi_A$ en décroissant, $|f|^p \varphi_{\overline{C}A}$ tend vers $|f|^r \varphi_{\overline{C}A}$ en croissant. Donc $\int |f|^p \varphi_{\overline{C}A} d|\mu|$ tend vers $\int^* |f|^r \varphi_{\overline{C}A} d|\mu|$ ($§ 1$, no 3, th. 3). D’autre part, $|f|^p \varphi_A$ est intégrable pour $p \in J$, et $\int |f|^p \varphi_A d|\mu|$ tend vers $\int |f|^r \varphi_A d|\mu|$ ($§ 4$, no 3, prop. 4). Donc $\int |f|^p d|\mu|$ tend vers $\int^* |f|^r d|\mu|$, ce qui prouve la continuité de $p \mapsto N_p(f)$ en r.

Le même raisonnement s’applique au point s si $s < +\infty$. Supposons enfin $s = +\infty$. Compte tenu de (13), il suffit de prouver que $\liminf_{p \to +\infty} N_p(f) \geq N_\infty(f)$. Or, soit $a$ un nombre tel que $0 < a < N_\infty(f)$. Comme par hypothèse il existe des valeurs finies de $p$ telles que $N_p(f) < +\infty$, l’ensemble A des $x \in X$ tels que $|f(x)| \geq a$, qui est mesurable et non négligeable, est intégrable en raison de l’inégalité $\varphi_A \leq (|f|/a)^p$; en outre, on tire de cette inégalité que $N_p(f) \geq a . (|\mu|(A))^{1/p}$; faisant tendre $p$ vers $+\infty$, il vient $\liminf_{p \to +\infty} N_p(f) \geq a$, ce qui achève la démonstration.

#### Corollaire {#int-iv-s6-n5-cor-1 .statement}

Si $r, s, p$ sont trois nombres tels que $1 \leq r < p < s \leq +\infty$, l’intersection $\mathcal{L}_F^r \cap \mathcal{L}_F^s$ est contenue dans $\mathcal{L}_F^p$.

On notera qu’en général, les topologies induites sur l’intersection $\mathcal{L}_F^r \cap \mathcal{L}_F^s$ par les topologies des $\mathcal{L}_F^p$ ($r < p < s$) sont distinctes. Si on ne fait aucune hypothèse supplémentaire sur $\mu$, les topologies induites sur $\mathcal{L}_F^r \cap \mathcal{L}_F^s$ par celles de $\mathcal{L}_F^r$ et de $\mathcal{L}_F^s$ sont en général non comparables (en d’autres termes, le rapport $N_r(f)/N_s(f)$ peut prendre des valeurs arbitrairement grandes et des valeurs arbitrairement petites dans $\mathcal{L}_F^r \cap \mathcal{L}_F^s$; cf. exerc. 8).

La prop. 4 peut être précisée lorsque $\mu$ est une mesure bornée :

#### Proposition 5 {#int-iv-s6-prop-5 .statement}

Soit $\mu$ une mesure bornée, et soit $f$ une fonction $\mu$-mesurable à valeurs dans un espace de Banach F. L’ensemble I des nombres $p$ tels que $1 \leq p \leq +\infty$ et que $N_p(f)$ soit finie, est vide ou est un intervalle d’origine $p = 1$ et contenant ce point; en outre, $(\mu(X))^{-1/p} N_p(f)$ est fonction croissante de $p$ dans I.

BARYCENTRES

C’est une conséquence immédiate de la prop. 4 ci-dessus, et du cor. de la prop. 4 du chap. I, n° 3.

#### Corollaire {#int-iv-s6-n5-cor-2 .statement}

Si la mesure $\mu$ est bornée, la relation $r < s$ entraîne $\mathcal{L}_F^s \subset \mathcal{L}_F^r$; en outre, la topologie de la convergence en moyenne d’ordre $s$ est plus fine que la topologie de la convergence en moyenne d’ordre $r$ (sur $\mathcal{L}_F^s$).

On peut montrer qu’en général la topologie de la convergence en moyenne d’ordre $s$ est strictement plus fine que la topologie de la convergence en moyenne d’ordre $r$ (exerc. 8).

#### Proposition 6 {#int-iv-s6-prop-6 .statement}

Soient $X$ un espace discret, $\mu$ la mesure sur $X$ définie par la masse $+1$ placée en chaque point de $X$. Si $f$ est une application de $X$ dans l’espace de Banach $F$, l’ensemble $I$ des nombres $p$ tels que $1 \leq p \leq +\infty$ et que $N_p(f)$ soit finie, est vide ou est un intervalle d’extrémité $+\infty$ et contenant ce point ; en outre, $N_p(f)$ est fonction décroissante de $p$ dans $I$.

En effet, on a $\mu^*(|f|) = \sum_{x \in X} |f(x)|$ pour toute fonction $f$ (§ 1, n° 1, Exemple), et $N_\infty(f) = \|f\| = \sup_{x \in X} |f(x)|$; s’il existe un nombre $\alpha > 0$ tel que l’on ait $|f(x)| \geq \alpha$ pour une infinité de valeurs de $x \in X$, on a $N_p(f) = +\infty$ pour tout $p$ fini ; dans le cas contraire il existe un $x_0 \in X$ tel que $|f(x_0)| = \|f\|$, d’où
$$
N_\infty(f) = |f(x_0)| \leq N_p(f)
$$
pour tout $p$ fini. Comme la fonction $\log N_p(f)$ est convexe par rapport à $1/p$ et prend sa plus petite valeur au point $+\infty$, elle est nécessairement fonction décroissante de $p$ dans $I$ (Fonct. var. réelle, chap. I, §4, n° 3, prop. 5), ce qui achève la démonstration.

#### Corollaire {#int-iv-s6-n5-cor-3 .statement}

Si $X$ est discret et si la mesure $\mu$ est définie par la masse $+1$ en chaque point de $X$, la relation $r < s$ entraîne $\mathcal{L}_F^r \subset \mathcal{L}_F^s$; en outre, la topologie de la convergence en moyenne d’ordre $r$ est plus fine que la topologie de la convergence en moyenne d’ordre $s$ (sur $\mathcal{L}_F^r$).

## EXERCICES {#int-iv-s6-exercises}

See the [exercises for § 6](exercises/s6/).
