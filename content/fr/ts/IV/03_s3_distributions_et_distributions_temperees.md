---
book: ts
book_title: Théories spectrales
chapter: IV
chapter_title: THÉORIE SPECTRALE HILBERTIENNE
section: 3
section_title: Distributions et distributions tempérées
lang: fr
source: ts-iii-v-fr
book_pages: A IV.196-A IV.223, A IV.330-A IV.344
pdf_pages: 0209-0236, 0343-0357
extraction: native
subsections:
    - "no": 1
      title: Dérivation sous le signe somme
      page: 197
      pdf_page: 210
    - "no": 2
      title: Critères d’intégrabilité dans R$^n$ et Z$^n$
      page: 199
      pdf_page: 212
    - "no": 3
      title: Fonctions test
      page: 200
      pdf_page: 213
    - "no": 4
      title: Distributions
      page: 203
      pdf_page: 216
    - "no": 5
      title: Interprétation de fonctions comme distributions
      page: 206
      pdf_page: 219
    - "no": 6
      title: Dérivation des distributions
      page: 208
      pdf_page: 221
    - "no": 7
      title: Fonctions de Schwartz
      page: 209
      pdf_page: 222
    - "no": 8
      title: Inclusions d’espaces fonctionnels dans l’espace des fonctions de Schwartz
      page: 212
      pdf_page: 225
    - "no": 9
      title: Fonctions à croissance polynomiale
      page: 214
      pdf_page: 227
    - "no": 10
      title: Distributions tempérées
      page: 214
      pdf_page: 227
    - "no": 11
      title: Interprétation de fonctions comme distributions tempé- rées
      page: 216
      pdf_page: 229
    - "no": 12
      title: Transformation de Fourier des distributions tempérées
      page: 217
      pdf_page: 230
    - "no": 13
      title: Distributions et distributions tempérées sur un espace vectoriel
      page: 221
      pdf_page: 234
    - "no": 14
      title: Espaces de Sobolev
      page: 221
      pdf_page: 234
statements: 46
exercises: 33
content_sha256: 7d66bcffa1460836b747007f8c6dfba03d2e4efa4d124f2a548123f68b9fbd89
---

## § 3. DISTRIBUTIONS ET DISTRIBUTIONS TEMPÉRÉES

Dans ce paragraphe, $n$ désigne un entier naturel. On notera $\mu$ la mesure de Lebesgue sur $\mathbf{R}^n$, ainsi que sa restriction à tout ensemble localement compact de $\mathbf{R}^n$.

On note

$$
x\cdot y=\sum_{i=1}^nx_iy_i
$$

le produit scalaire sur l’espace euclidien $\mathbf{R}^n$; la norme euclidienne est notée $x\mapsto  \|x\|$ (TG, VI, p. 7). On rappelle que le groupe $\mathbf{R}^n$ est en dualité avec lui-même relativement à l’application $(x, y)\mapsto$ exp(2$i\pi  x\cdot y)$ et que la mesure duale de la mesure de Lebesgue s’identifie alors avec la mesure de Lebesgue (corollaire 3 de II, p. 236). On note $\mathscr{F}$ (resp. $\mathscr{F})$ la transformation de Fourier (resp. la cotransformation de Fourier) de $\mathbf{R}^n$ (cf. n$^o9$ de II, p. 237).

Pour tout $\alpha = (\alpha_i)_{1\leqslant i\leqslant n}\in \mathbf{N}^n$, on notera $X^{\alpha}$ la fonction de $\mathbf{R}^n$

dans $\mathbf{R}$ définie par $x= (x_i)_{1\leqslant i\leqslant n}\mapsto x^{\alpha}=\prod_{i=1}^nx^{\alpha}_{i^i}$.

Soient $\alpha$ et $\beta$ des éléments de $\mathbf{N}^n$. On note

$$
^n(\alpha )^n(\alpha_i)
$$

$$
|\alpha |=\sum\alpha_i,=\prod
$$

$$
\beta \beta_i
$$

$i=1i=1$

#### Lemme 1 {#ts-iv-s3-lem-1 .statement tag=030C}

Soit U un ouvert de $\mathbf{R}^n$.

a) Soient K une partie compacte de U et V un voisinage ouvert de K dans U. Il existe une fonction $\varphi \in \mathscr{C}^{\infty}(U)$ à support compact contenu dans V telle que $0\leqslant \varphi \leqslant 1$ et telle que $\varphi (x) = 1$ pour tout $x\in K$;

b) Pour tout recouvrement ouvert localement fini de U, il existe une partition de l’unité formée de fonctions de classe $C^{\infty}$ qui lui est subordonnée.

Cela résulte de VAR, R1, p. 40, 5.3.6.

#### Proposition 1 {#ts-iv-s3-prop-1 .statement tag=030D}

Soient U un ouvert de $\mathbf{R}^n$ et $k\in \mathbf{N}$. Soient E, F et G des espaces vectoriels topologiques et $b: E\times F\rightarrow G$ une application bilinéaire continue. Soient $f$ et $g$ des fonctions de classe $C^k$ de U dans E et F respectivement. Alors l’application $h:x\mapsto b(f(x), g(x))$ est de classe $C^k$ dans U ; de plus, pour tout $\alpha \in \mathbf{N}^n$ tel que $|\alpha |\leqslant k$ et pour tout $x\in U$, on a

$$
\alpha (\alpha )\beta \alpha -\beta
$$

$$
\partial h(x) =\sum b \partial f(x), \partial g(x)
$$

$$
_{\beta\in\mathbf{N}^n}\beta
$$

$\beta \leqslant \alpha$

L’application $h$ est la composée de l’application $(f, g) : U\rightarrow E\times F$, qui est de classe $C^k$, et de l’application $b: E\times F\rightarrow G$ qui est de classe $C^{\infty}$. Elle est donc de classe $C^k$. L’expression pour ses dérivées partielles résulte de la formule de Leibniz (FVR, I, p. 28, prop. 2, cf. A, III, p. 122, corollaire).

On rappelle qu’un espace vectoriel topologique localement convexe séparé est un espace de Montel s’il est tonnelé et si toute partie bornée est relativement compacte (EVT, IV, p. 18, déf. 4).

On rappelle également que si E et F sont des espaces localement convexes, et si E est bornologique (EVT, III, p. 12, déf. 1), une application linéaire $u: E\rightarrow F$ est continue si et seulement si l’image par $u$ de toute partie bornée de E est bornée dans F (EVT, III, p. 11, prop. 1, (iiibis), lorsque F est semi-normé, le cas général en résultant de manière formelle, cf. EVT, II, p. 7, prop. 5, b)).

### 1. Dérivation sous le signe somme

On fixe un espace topologique localement compact X et une mesure $\nu$ sur X. Soit E un espace de Banach.

#### Proposition 2 {#ts-iv-s3-prop-2 .statement tag=030E}

Soient I un intervalle de $\mathbf{R}$ et $f$ une application de $X\times I$ dans E telle que

(i) Pour tout $t\in I$, l’application $x\mapsto f(x, t)$ de X dans E est $\nu$-intégrable ;

(ii) Pour tout $x\in X$, l’application $t\mapsto f(x, t)$ de I dans E admet une dérivée, notée $t\mapsto f'(x, t)$;

(iii) Il existe une fonction positive $\nu$-intégrable $g$ sur X telle que $\|f'(x, t)\|\leqslant g(x)$ pour tout $(x, t)\in X\times I$.

Alors l’application F de I dans E définie par

$$
F(t) =\int_Xf(x, t)d\nu (x)
$$

est dérivable dans I et pour tout $t\in I$, on a

$$
F'(t) =\int_Xf'(x, t)d\nu (x)
$$

Soit $t_0\in I$ et soit J un intervalle de $\mathbf{R}$ contenu dans I qui est un voisinage de $t_0$ dans I. Soit $h: X\times J\rightarrow E$ l’application définie par $(x, t)\mapsto (f(x, t)-f(x, t_0))/(t-t_0)$ pour $(x, t)\in X\times (J-\{t_0\})$ et $(x, t_0)\mapsto f'(x, t_0)$ pour $x\in X$. Soit $x\in X$. On a $\|h(x, t_0)\|\leqslant g(x)$ et, pour tout $t\not =t_0$, il vient $\|h(x, t)\|\leqslant g(x)$ par FVR, I, p. 23, th. 2. Par définition de la dérivée, la proposition se déduit du corollaire 1 de INT, IV, p. 144, § 4, n$^o3$, appliqué à l’application $h$.

Reprenons les notations de VAR, R1, 2.4, p. 19 concernant les dérivées partielles.

#### Corollaire 1 {#ts-iv-s3-prop-2-cor-1 .statement tag=030F}

Soit U un ouvert de $\mathbf{R}^n$. Soient $k\in \mathbf{N}$ et $f$ une application de $X\times U$ dans E qui vérifie les conditions suivantes :

(i) Pour tout $t\in U$, l’application $x\mapsto f(x, t)$ de X dans E est $\nu$-intégrable ;

(ii) Pour tout $x\in X$, l’application $t\mapsto f(x, t)$ de U dans E est de classe $C^k$, de dérivées partielles notées $\partial^{\alpha}f(x, t)$ pour tout $\alpha \in \mathbf{N}^n$ tel que $|\alpha |\leqslant k$;

(iii) Il existe une fonction $\nu$-intégrable $g$ sur X telle que pour tout $\alpha \in \mathbf{N}^n$ vérifiant $|\alpha |\leqslant k$ et pour tout $(x, t)\in X\times U$, on a $\|\partial^{\alpha}f(x, t)\|\leqslant g(x)$.

Alors l’application F de U dans E définie par

$$
F(t) =\int_Xf(x, t)d\nu (x)
$$

est de classe $C^k$ dans U et pour tout $\alpha \in \mathbf{N}^n$ vérifiant $|\alpha |\leqslant k$ et tout $t\in U$, on a

$$
\partial^{\alpha}F(t) =\int_X\partial^{\alpha}f(x, t)d\nu (x)
$$

Cela résulte de la proposition par récurrence sur $k$.

#### Corollaire 2 {#ts-iv-s3-prop-2-cor-2 .statement tag=030G}

Soit $k$ un entier naturel. Soient $f\in \mathscr{L}^1(\mathbf{R}^n, \mu)$ et $g\in \mathscr{C}^k(\mathbf{R}^n)$. On suppose que pour tout $\alpha \in \mathbf{N}^n$ tel que $|\alpha |\leqslant k$, la fonction $\partial^{\alpha}g$ est bornée. Alors le produit de convolution $f*g$ appartient à $\mathscr{C}^k(\mathbf{R}^n)$ et pour tout $\alpha$ tel que $|\alpha |\leqslant k$, on a $\partial^{\alpha}(f*g) =f*\partial^{\alpha}g$.

On peut appliquer le corollaire 1 à l’espace $X =\mathbf{R}^n$, à la mesure de Lebesgue et à l’application $h$ définie par $(x, t)\mapsto f(x)g(t-x)$ de $\mathbf{R}^n\times \mathbf{R}^n$ dans $\mathbf{C}$; en effet, pour tout $\alpha \in \mathbf{N}^n$ tel que $|\alpha |\leqslant k$, on a l’inégalité

$|\partial^{\alpha}h(x, t)|\leqslant$ sup sup $|\partial^{\beta}g(y)||f(x)|$

$|\beta |\leqslant ky\in \mathbf{R}^n$

dont le second membre est une fonction intégrable sur $\mathbf{R}^n$.

### 2. Critères d’intégrabilité dans R$^n$ et Z$^n$

#### Proposition 3 {#ts-iv-s3-prop-3 .statement tag=030H}

Soient N une norme sur $\mathbf{R}^n,r$ un nombre réel et $p\in [1,+\infty [$.

a) La fonction $(1 + N)^r$ appartient à $\mathscr{L}^p(\mathbf{R}^n, \mu)$ si et seulement si $rp <-n$;

a$')$ La restriction à $\mathbf{Z}^n$ de la fonction $(1 + N)^r$ appartient à $\ell^p(\mathbf{Z}^n)$ si et seulement si $rp <-n$;

b) Soit V un voisinage mesurable borné de 0 dans $\mathbf{R}^n$. La fonction $N^r$ appartient à $\mathscr{L}^p(\mathbf{R}^n-V, \mu)$ si et seulement si $rp <-n$.

En vertu de l’équivalence des normes sur $\mathbf{R}^n$ (EVT I, p. 14, th. 2 et TG, IX, p. 32, prop. 8), on peut supposer que la norme N est donnée par $N(x) =$ sup$|x_i|$ pour $x= (x_i)\in \mathbf{R}^n$. Notons B la boule unité de $\mathbf{R}^n$ pour cette norme.

Soit V un voisinage mesurable borné de 0 dans $\mathbf{R}^n$. La fonction $N^r$ est continue et bornée sur (B- $V)\cup (V$- B), ce qui montre que l’assertion b) est valide si et seulement si elle l’est lorsque V = B, ce qu’on supposera désormais. La fonction $(1 + N)^r$ étant continue et bornée sur B, et vérifiant l’encadrement $N^r\leqslant (1 + N)^r\leqslant 2^rN^r$ sur $\mathbf{R}^n-$ B, on constate que les assertions a) et b) sont équivalentes.

Démontrons b) lorsque V = B. On peut supposer que $p= 1$. Le cas où $r >0$ étant élémentaire, supposons que $r\leqslant 0$. Pour tout entier $j\geqslant 1$, l’ensemble intégrable

$$
C_j=\{x\in \mathbf{R}^n|2^{j-1}\leqslant N(x)<2^j\}
$$

est de mesure $2^{nj}(2^n-1)$. Les ensembles $(C_j)_{j\geqslant 1}$ forment une partition de $\mathbf{R}^n-$ B. D’après INT, V, p. 4, § 1, n$^o1$, cor., on a donc

$$
\int^*N^rd\mu=\sum\int^*N^rd\mu
$$

$\mathbf{R}^{n-}Bj\geqslant 1C^j$

$\leqslant \sum_{j\geqslant 1}2^{n+nj}2^{r(j-1)}= 2^{n-r}\sum_{j\geqslant 1}2^{(n+r)j}$ qui est finie si $r <-n$. D’autre part, on a (loc. cit.)

$$
\int^*N^rd\mu\geqslant \sum 2^{rj}2^{nj}(2^n-1) = (2^n-1)\sum 2^{(r+n)j}
$$

$\mathbf{R}^{n-}Bj\geqslant 1j\geqslant 1$

qui est infini si $r\geqslant -n$.

On démontre a$')$ de manière similaire en considérant les ensembles $C_j\cap \mathbf{Z}^n$ qui recouvrent $\mathbf{Z}^n-\{0\}$ et vérifient

Card(C$_j\cap \mathbf{Z}^n) = (2^{j+1}-1)^n-(2^j-1)^n$,

qui appartient à l’intervalle $[(1-2^{-n})(2^{j+1}-1)^n,2^{n(j+1)}]$.

### 3. Fonctions test

Dans ce numéro, U désigne un ouvert de $\mathbf{R}^n$. Pour $p\in [1,+\infty ]$, on écrira $\mathscr{L}^p(U)$ et $L^p(U)$ plutôt que $\mathscr{L}^p(U, \mu)$ et $L^p(U, \mu)$. On identifie les fonctions continues appartenant à $\mathscr{L}^p(U)$ à leur image dans $L^p(U)$.

Munissons l’espace $\mathscr{C}^{\infty}(U)$ des fonctions indéfiniment dérivables dans U à valeurs complexes de la topologie définie par la famille de semi-normes $p_{\alpha ,K}$ définies pour $\alpha \in \mathbf{N}^n$ et $K\subset U$ par

$p_{\alpha ,K}(\varphi ) =$ sup$|\partial^{\alpha}\varphi (x)|$.

$x\in K$

Cet espace est complet (cf. EVT, III, p. 9, exemple b)).

Pour toute partie compacte K de U, on note $\mathscr{C}_K^{\infty}(U)$ le sous-espace de $\mathscr{C}^{\infty}(U)$ formé des fonctions à support dans K. L’espace $\mathscr{C}_K^{\infty}(U)$ est muni de la topologie induite par celle de $\mathscr{C}^{\infty}(U)$. C’est un espace de Fréchet, une famille dénombrable de semi-normes qui en définit la topologie étant la famille $(p_{\alpha ,K})_{\alpha\in\mathbf{N}^n}$. En particulier, c’est un espace bornologique (EVT, III, p. 12, prop. 2).

On note $\mathscr{D}(U)$ l’espace vectoriel $\mathscr{K}(U)\cap \mathscr{C}^{\infty}(U)$ des fonctions de classe $C^{\infty}$ à support compact dans U. On dit que $\mathscr{D}(U)$ est l’espace des fonctions test dans U. L’espace $\mathscr{D}(U)$ est la limite inductive des espaces $\mathscr{C}_K^{\infty}(U)$ et il est muni de la topologie localement convexe limite inductive correspondante (EVT, II, p. 31).

Cet espace est noté $\mathscr{C}_{\circ}^{\infty}(U)$ dans EVT, III, p. 9.

Soit $(K_m)$ une suite croissante de parties compactes de U dont les intérieurs forment un recouvrement de U. L’espace $\mathscr{D}(U)$ est alors la limite inductive stricte des espaces $\mathscr{C}_K^{\infty_m}(U)$ (EVT, III, p. 9). C’est donc un espace complet (EVT, II, p. 35, prop. 9). Toute partie bornée de $\mathscr{D}(U)$ est contenue dans l’un des sous-espaces $\mathscr{C}_K^{\infty_m}(U)$ (EVT, III, p. 5, prop. 6). Cela signifie que $B\subset \mathscr{D}(U)$ est bornée si et seulement si il existe une partie compacte K de U et une famille $(M_{\alpha})_{\alpha\in\mathbf{N}^n}$ dans $\mathbf{R}_+$ telles que B est contenu dans l’ensemble des fonctions $\varphi \in \mathscr{C}_K^{\infty}(U)$ vérifiant

$$
p_{\alpha ,K}(\varphi )\leqslant M_{\alpha}
$$

pour tout $\alpha \in \mathbf{N}^n$.

L’espace $\mathscr{D}(U)$ est un espace bornologique (EVT, III, p. 12, exemple 3) et un espace de Montel (EVT, IV, p. 18, exemple 4).

Soit V un ouvert de $\mathbf{R}^n$ contenu dans U. Si $K\subset V$ est compact, alors la restriction des fonctions à V définit une application linéaire continue et surjective de $\mathscr{C}_K^{\infty}(U)$ sur $\mathscr{C}_K^{\infty}(V)$. L’extension par zéro d’une fonction définie sur V induit une application linéaire continue injective, dite canonique, de $\mathscr{D}(V)$ dans $\mathscr{D}(U)$.

#### Remarque {#ts-iv-s3-n3-rem-1 .statement tag=030I}

On définit de même l’espace $\mathscr{D}_{\mathbf{R}}(U)$ des fonctions test dans U à valeurs réelles. L’application linéaire telle que $z\otimes \varphi \mapsto z\varphi$ pour tout $z\in \mathbf{C}$ et tout $\varphi \in \mathscr{D}_{\mathbf{R}}(U)$ est un isomorphisme de $\mathbf{C}\otimes \mathscr{D}_{\mathbf{R}}(U)$ dans $\mathscr{D}(U)$.

#### Lemme 2 {#ts-iv-s3-lem-2 .statement tag=030J}

Soit $\mathscr{U}$ un recouvrement ouvert de U. Il existe un recouvrement ouvert localement fini de U plus fin que $\mathscr{U}$ et formé de parties relativement compactes.

Comme U est localement compact, il existe un recouvrement $\mathscr{V}$ de U plus fin que $\mathscr{U}$ constitué d’ouverts relativement compacts dans U. Puisque U est paracompact (TG, IX, p. 51, th. 4), il existe un recouvrement ouvert localement fini $\mathscr{W}$ plus fin que $\mathscr{V}$. Alors $\mathscr{W}$ est plus fin que $\mathscr{U}$ et est constitué d’ouverts relativement compacts.

#### Lemme 3 {#ts-iv-s3-lem-3 .statement tag=030K}

Soit $f\in \mathscr{K}(\mathbf{R}^n)$ et soit V un voisinage ouvert du support K de $f$. Il existe un entier $m_0\geqslant 1$ tel que, pour tout $x\in K$, l’ensemble V contient la boule de rayon $m^{-1}_0$ centrée en $x$. Pour tout entier $m > m_0$, soit $V_m$ la boule fermée de rayon $m^{-1}$ centrée en 0 dans $\mathbf{R}^n$ et soit $\varphi_m$ une fonction test à support dans $V_m$, positive et d’intégrale 1. Posons $f_m=\varphi_m*f$.

a) On a $f_m\in \mathscr{D}(\mathbf{R}^n)$ et le support de $f_m$ est contenu dans V ;

b) Soit $p\in [1,+\infty ]$. La suite $(f_m)_{m>m_0}$ converge vers $f$ dans $L^p(\mathbf{R}^n)$.

D’après TG, IX, p. 14, remarque, on a $d(K,\mathbf{R}^n-V)>0$. Soit $m_0\geqslant 1$ un entier tel que $m^{-1}_0< d(K,\mathbf{R}^n-$ V) ; il vérifie la condition demandée. Pour tout $m > m_0$, la fonction $f_m$ est continue (INT, VIII, p. 166, § 4, n$^o5$, prop. 11) et à support contenu dans $K + V_m$ (INT, VIII, p. 126, § 1, n$^o4$, prop. 5), donc dans V. D’après le corollaire 2 de IV, p. 198, on a $f_m\in \mathscr{D}(\mathbf{R}^n)$. Si $p\not = +\infty$, alors la suite $(f_m)$ converge vers $f$ dans $L^p(\mathbf{R}^n)$ (INT, VIII, p. 172, § 4, n$^o7$, prop. 20).[^1]

Supposons que $p= +\infty$. Soit $\varepsilon  >0$. La fonction $f$ est uniformément continue sur $\mathbf{R}^n$, donc il existe un entier $m_1> m_0$ tel que, pour tout $m\geqslant m_1$ et tous $x\in \mathbf{R}^n$ et $y\in V_m$, on ait $|f(x)-f(x-y)|< \varepsilon$.

Pour tout $m\geqslant m_1$, la fonction $\varphi_m$ est nulle en dehors de $V_m$, positive et d’intégrale 1. On en déduit donc l’inégalité

$$
|f(x)-f_m(x)|=\int_{\mathbf{R}^n}(f(x)-f(x-y))\varphi_m(y)d\mu(y)\leqslant \varepsilon
$$

pour tout $x\in \mathbf{R}^n$, d’où le résultat.

#### Proposition 4 {#ts-iv-s3-prop-4 .statement tag=030L}

a) L’injection canonique de $\mathscr{D}(U)$ dans $\mathscr{K}(U)$ est continue et $\mathscr{D}(U)$ est dense dans $\mathscr{K}(U)$;

b) Pour tout $p\in [1,+\infty [$, l’injection canonique de $\mathscr{D}(U)$ dans $\mathscr{L}^p(U)$ est continue et $\mathscr{D}(U)$ est dense dans $L^p(U)$.

Toute semi-norme continue sur $\mathscr{K}(U)$ est continue sur $\mathscr{D}$(U), donc l’injection canonique de $\mathscr{D}(U)$ dans $\mathscr{K}(U)$ est continue.

Soit $f\in \mathscr{K}(U)$. Il existe une suite $(f_m)_{m\in\mathbf{N}}$ dans $\mathscr{D}(U)$ qui converge uniformément vers $f$ sur U et telle que les supports des $f_m$ soient contenus dans un voisinage relativement compact fixé du support de $f$ (lemme 3). La suite $(f_m)$ converge donc vers $f$ dans $\mathscr{K}(U)$. Cela conclut la preuve de a).

Soit $p\in [1,+\infty [$. Soit $f\in \mathscr{D}(U)$ et soit K le support de $f$. On a alors l’inégalité $N_p(f)\leqslant \mu(K)^{1/p}$ sup$_{x\in K}|f(x)|$, donc l’injection canonique de $\mathscr{D}(U)$ dans $\mathscr{L}^p(U)$ est continue. La dernière partie de l’assertion b) résulte alors de a).

Le produit de deux fonctions test étant encore une fonction test, la formule de Leibniz (FVR, I, p. 28, prop. 2) montre que l’espace $\mathscr{D}(U)$ est une algèbre topologique.

Plus généralement, soit $f\in \mathscr{C}^{\infty}(U)$. L’application linéaire $\varphi \mapsto f \varphi$ de $\mathscr{D}(U)$ dans $\mathscr{D}(U)$ est alors continue. En effet, pour toute partie compacte K de U et tout $\alpha \in \mathbf{N}^n$, on a

$$
(\alpha )
$$

$$
p_{\alpha ,K}(f \varphi )\leqslant \sum p_{\beta ,K}(f)p_{\alpha-\beta ,K}(\varphi )
$$

$$
\beta
$$

$0\leqslant \beta \leqslant \alpha$

(cf. loc. cit.).

### 4. Distributions

On conserve les notations du numéro précédent ; U désigne donc un ouvert de $\mathbf{R}^n$.

#### Définition 1 {#ts-iv-s3-def-1 .statement tag=030M}

L’espace dual de $\mathscr{D}(U)$, muni de la topologie de la convergence bornée, est appelé l’espace des distributions sur U. Il est noté $\mathscr{D}'(U)$.

Une distribution sur U est donc une forme linéaire continue sur $\mathscr{D}(U)$.

Si $f$ est une forme linéaire sur $\mathscr{D}(U)$ (et en particulier si $f$ est une distribution) et si $\varphi$ est dans $\mathscr{D}$(U), on notera $\langle f, \varphi \rangle$ l’évaluation de $f$ en $\varphi$.

Puisque $\mathscr{D}(U)$ est bornologique, l’espace $\mathscr{D}'(U)$ est complet (EVT, III, p. 24, cor. 1). Comme $\mathscr{D}(U)$ est un espace de Montel, il en est de même de $\mathscr{D}'(U)$ (EVT, IV, p. 19, prop. 9). En particulier, l’espace $\mathscr{D}'(U)$ est réflexif (EVT, IV, p. 16, th. 2).

#### Lemme 4 {#ts-iv-s3-lem-4 .statement tag=030N}

Soit $f$ une application linéaire de $\mathscr{D}(U)$ dans $\mathbf{C}$. Alors $f$ est une distribution si et seulement si, pour toute partie compacte K de U et pour toute famille $(M_{\alpha})_{\alpha\in\mathbf{N}^n}$ dans $\mathbf{R}_+$, la forme linéaire $f$ est bornée sur l’ensemble des fonctions $\varphi \in \mathscr{C}_K^{\infty}(U)$ telles que, pour tout $\alpha \in \mathbf{N}^n$, on a

sup$|\partial^{\alpha}\varphi (x)|\leqslant M_{\alpha}$.

$x\in K$

En effet, l’espace $\mathscr{D}(U)$ est bornologique et toute partie bornée de $\mathscr{D}(U)$ est contenue dans l’un des ensembles bornés décrits dans l’énoncé.

#### Lemme 5 {#ts-iv-s3-lem-5 .statement tag=030O}

Soit $\mathfrak{F}$ un filtre sur $\mathscr{D}'(U)$ ayant une base dénombrable ou contenant un ensemble simplement borné. Alors $\mathfrak{F}$ converge vers une distribution si et seulement si $\langle f, \varphi \rangle$ converge selon $\mathfrak{F}$ pour toute fonction test $\varphi$ sur U.

En particulier, une suite $(f_m)_{m\in\mathbf{N}}$ de distributions converge vers une distribution $f$ si et seulement si, pour tout $\varphi \in \mathscr{D}(U)$, la suite $(\langle f_m, \varphi \rangle )_{m\in\mathbf{N}}$ converge vers $\langle f, \varphi \rangle$.

Comme $\mathscr{D}'(U)$ est un espace de Montel, donc tonnelé, cela résulte du théorème de Banach–Steinhaus (EVT, III, p. 26, cor. 3 du th. 1).

Soit V un ouvert contenu dans U. La transposée de l’application linéaire canonique de $\mathscr{D}(V)$ dans $\mathscr{D}(U)$ est une application linéaire continue de $\mathscr{D}'(U)$ dans $\mathscr{D}'$(V), appelée restriction des distributions de U à V et notée $r_{VU}$, ou parfois $r_{V,U}$.

On a $r_{VV}= 1_{\mathscr{D}'(V)}$. Si $W\subset V\subset U$ sont des ouverts dans U, alors on a $r_{WV}\circ r_{VU}=r_{WU}$. Autrement dit, si $\mathscr{T}$ désigne la topologie sur U, le système projectif $\mathscr{D}'(U) = ((\mathscr{D}'(V))_{V\in\mathscr{T}},(r_{WV}))$ est un préfaisceau sur U à valeurs dans l’espèce de structure des espaces vectoriels topologiques localement convexes (TA, I, p. 42, déf. 1 et p. 66, §10).

#### Proposition 5 {#ts-iv-s3-prop-5 .statement tag=030P}

Le préfaisceau $\mathscr{D}'(U)$ est un faisceau.

Rappelons (TA, I, p. 43, déf. 2) que cela signifie que pour toute partie ouverte V de U et tout recouvrement ouvert $(V_i)_{i\in I}$ de V, les conditions suivantes sont satisfaites :

(i) L’application $(r_{V_iV})_{i\in I}:\mathscr{D}'(V)\rightarrow \prod_{i\in I}\mathscr{D}'(V_i)$ est injective ;

(ii) Pour toute famille $(f_i)\in \prod_{i\in I}\mathscr{D}'(V_i)$ telle que

$$
r_{(V_i\cap V_{i'})V_i}(f_i) =r_{(V_i\cap V_{i'})V_{i'}}(f_{i'})
$$

pour tout couple $(i, i')\in I\times I$, il existe une distribution $f\in \mathscr{D}'(V)$ telle que pour tout $i\in I$, on ait $r_{V_iV}(f) =f_i$.

Soient V un ouvert de U et $\mathscr{V}= (V_i)_{i\in I}$ un recouvrement ouvert de V. Soit $(W_j)_{j\in J}$ un recouvrement ouvert localement fini de V, plus fin que $\mathscr{V}$ et formé de parties relativement compactes (lemme 2 de IV, p. 201). Fixons une partition de l’unité $(\varphi_j)_{j\in J}$ subordonnée au recouvrement $(W_j)_{j\in J}$ telle que le support de $\varphi_j$ est contenu dans $W_j$ pour tout $j\in J$ (lemme 1 de IV, p. 196).

Soit $\varphi \in \mathscr{D}(V)$. Comme l’ensemble des $j\in J$ tels que $W_j$ rencontre le support de $\varphi$ est fini (TG, I, §9, n$^o1$, p. 59), on a

$$
\varphi =\sum_{j\in J}\varphi \varphi_j
$$

où la somme ne compte d’un nombre fini de termes non nuls.

Démontrons (i). Supposons que $f\in \mathscr{D}'(V)$ vérifie $r_{V_iV}(f) = 0$ pour tout $i\in I$. Cela signifie que $\langle f, \varphi \rangle = 0$ pour toute fonction test $\varphi$ dont le support est contenu dans l’un des ouverts $V_i$. C’est a fortiori vrai si le support de $\varphi$ est contenu dans l’un des ouverts $W_j$. Mais alors, pour tout $\varphi \in \mathscr{D}$(V), on a

$$
\langle f, \varphi \rangle =\langle f,\sum_{j\in J}\varphi \varphi_j\rangle =\sum_{j\in J}\langle f, \varphi \varphi_j\rangle = 0
$$

donc $f= 0$.

Démontrons (ii). Soit $(f_i)_{i\in I}$ une famille telle que $f_i\in \mathscr{D}'(V_i)$ pour tout $i\in I$ et $r_{V_i\cap V_{i'},V_i}(f_i) =r_{V_i\cap V_{i'},V_{i'}}(f_{i'})$ pour tous $i$ et $i'$ dans I. Soit $\iota : J\rightarrow I$ une application telle que $W_j\subset V_{\iota(j)}$ pour tout $j\in J$. Pour tout $j\in J$, posons $\widetilde{f}_j=r_{W_j,V_{\iota(j)}}(f_{\iota(j)})$. On a alors

$$
r_{W_j\cap W_{j'},W_j}(\widetilde{f}_j) =r_{W_j\cap W_{j'},W_j}(r_{W_j,V_{\iota(j)}}(f_{\iota(j)}))
$$

$$
=r_{W_j\cap W_{j'},V_{\iota(j)}}(f_{\iota(j)})
$$

$$
=r_{W_j\cap W_{j'},V_{\iota(j)}\cap V_{\iota(j')}}\circ r_{V_{\iota(j)}\cap V_{\iota(j')},V_{\iota(j)}}(f_{\iota(j)})
$$

En échangeant le rôle de $j$ et $j'$ et en notant que

$$
r_{V_{\iota(j)}\cap V_{\iota(j')},V_{\iota(j)}}(f_{\iota(j)}) =r_{V_{\iota(j)}\cap V_{\iota(j')},V_{\iota(j')}}(f_{\iota(j')})
$$

par hypothèse, on en déduit que

$$
r_{W_j\cap W_{j'},W_j}(\widetilde{f}_j) =r_{W_j\cap W_{j'},W_j}(\widetilde{f}_{j'}) \tag{1}
$$

pour tous $(j, j')\in J^2$.

Pour $\varphi \in \mathscr{D}$(V), posons

$$
\lambda (\varphi ) =\sum_{j\in J}\langle \widetilde{f}_j, \varphi \varphi_j|W_j\rangle
$$

où la somme est finie puisque seul un nombre fini de termes peuvent être non nuls.

L’application $\lambda$ est une forme linéaire sur $\mathscr{D}(V)$. Démontrons que c’est une distribution. Soit B une partie bornée de $\mathscr{D}(V)$ et soit K une partie compacte de V telle que $B\subset \mathscr{C}_K^{\infty}(V)$. D’après TG, I, §9, n$^o1$, p. 59, il existe un sous-ensemble fini $J'$ de J tel que

$$
\lambda (\varphi ) =\sum_{j\in J'}\langle \widetilde{f}_j, \varphi \varphi_j|W_j\rangle
$$

pour tout $\varphi \in B$. Puisque $\widetilde{f}_j$ est une distribution pour tout $j\in J'$ et que $\mathscr{D}(V)$ est une algèbre topologique, on en déduit que $\lambda$ est bornée sur B, d’où le résultat (lemme 4).

Soient $j\in J$ et $\varphi \in \mathscr{D}(V)$ dont le support est contenu dans $W_j$. On a alors

$$
\langle \lambda , \varphi \rangle =\sum_{j'\in J}\langle \widetilde{f}_{j'}, \varphi \varphi_{j'}|W_j\rangle =\sum_{j'\in J}\langle \widetilde{f}_j, \varphi \varphi_{j'}|W_j\rangle
$$

d’après (1), puisque $\varphi \varphi_{j'}$ a support contenu dans $W_j\cap W_{j'}$. Par conséquent

$$
\langle \lambda , \varphi \rangle =\langle \widetilde{f}_j,\sum_{j'\in J}\varphi \varphi_{j'}|W_j\rangle =\langle \widetilde{f}_j, \varphi |W_j\rangle
$$

d’où $r_{W_jV}(\lambda ) =\widetilde{f}_j$ pour tout $j\in J$.

Soit $i\in I$. Démontrons finalement que la restriction de $\lambda$ à $V_i$ coïncide avec $f_i$. D’après la condition (i), appliquée au recouvrement de $V_i$ par les ouverts $W_j$, il suffit de vérifier que pour tout $j\in J$, la restriction de $\lambda$ à $V_i\cap W_j$ coïncide avec celle de $f_i$. D’après ce qui précède, il s’agit de vérifier que la restriction de $f_i$ à $V_i\cap W_j$ est celle de $\widetilde{f}_j$. Or, on a

$$
r_{V_i\cap W_j,V_i}(f_i) =r_{V_i\cap W_j,V_i\cap V_{\iota(j)}}(r_{V_i\cap V_{\iota(j)},V_i}(f_i))
$$

$$
=r_{V_i\cap W_j,V_i\cap V_{\iota(j)}}(r_{V_i\cap V_{\iota(j)},V_{\iota(j)}}(f_{\iota(j)}) =r_{V_i\cap W_j,V_{\iota(j)}}(f_{\iota(j)})
$$

où on a utilisé l’hypothèse concernant la famille $(f_i)$. Mais alors

$$
r_{V_i\cap W_j,V_{\iota(j)}}(f_{\iota(j)}) =r_{V_i\cap W_j,W_j}(r_{W_j,V_{\iota(j)}}(f_{\iota(j)})) =r_{V_i\cap W_j,W_j}(\widetilde{f}_j)
$$

ce qui permet de conclure.

### 5. Interprétation de fonctions comme distributions

#### Proposition 6 {#ts-iv-s3-prop-6 .statement tag=030Q}

Soit $\nu$ une mesure sur U. La restriction de $\nu$ à $\mathscr{D}(U)$ est une distribution, qui est nulle si et seulement si la mesure $\nu$ est nulle.

Soit K une partie compacte de U. Pour toute fonction $\varphi \in \mathscr{C}_K^{\infty}$(U), on a $|\langle \nu , \varphi \rangle |\leqslant p_{0,K}(\varphi )|\nu |$(K), donc la restriction de $\nu$ à $\mathscr{D}(U)$ est continue. Puisque $\mathscr{D}(U)$ est dense dans $\mathscr{K}(U)$ (prop. 4, a) de IV, p. 202), la restriction de $\nu$ à $\mathscr{D}(U)$ est nulle si et seulement si $\nu$ est nulle.

On identifiera l’espace $\mathscr{M}(U;\mathbf{C})$ des mesures complexes sur U à un sous-espace de $\mathscr{D}'(U)$. On identifiera également l’espace $L^1_{loc}(U)$ à un sous-espace de $\mathscr{D}'(U)$ par l’application déduite par passage aux quotients de l’application qui associe à $f\in \mathscr{L}_{loc}^1(U)$ la mesure $f\cdot \mu$ (INT, V, p. 44, § 5, n$^o2$, déf. 2). En d’autres termes, pour $f\in L^1_{loc}(U)$ et $\varphi \in \mathscr{D}$(U), on a

$$
\langle f, \varphi \rangle =\int_Uf \varphi  d\mu
$$

En particulier, pour $p\in [1,+\infty ]$, cela permet d’identifier l’espace $L^p(U)$ à un sous-espace de $\mathscr{D}'(U) ($cf. INT, V, p. 43, § 5, n$^o1)$.

#### Proposition 7 {#ts-iv-s3-prop-7 .statement tag=030R}

Soit $p\in [1,+\infty ]$. L’injection de $L^p(U)$ dans $\mathscr{D}'(U)$ est continue.

Soit $f\in L^p(U)$. Soit K une partie compacte de U, dont on note $\varphi_K$ la fonction caractéristique. Pour toute fonction test $\varphi$ à support contenu dans K, l’inégalité de Hölder implique

$$
|\langle f, \varphi \rangle |=\int_Uf \varphi  d\mu\leqslant N_p(f)N_q(\varphi )\leqslant N_p(f)N_q(\varphi_K)p_{0,K}(\varphi )
$$

où $q$ est l’exposant conjugué de $p$.

On peut en particulier identifier $\mathscr{D}(U)$ à un sous-espace de $\mathscr{D}'(U)$.

#### Proposition 8 {#ts-iv-s3-prop-8 .statement tag=030S}

L’espace $\mathscr{D}(U)$ est dense dans $\mathscr{D}'(U)$.

Soit $\lambda$ une forme linéaire sur $\mathscr{D}'(U)$ nulle sur $\mathscr{D}(U)$. Puisque $\mathscr{D}(U)$ est réflexif, il existe une fonction test $\varphi \in \mathscr{D}(U)$ telle que $\lambda (f) =\langle f, \varphi \rangle$ pour tout $f\in \mathscr{D}'(U)$. Il vient

$$
0 =\lambda (\varphi ) =\langle \varphi , \varphi \rangle =\int_U|\varphi |^2d\mu
$$

d’où $\varphi = 0$. La proposition découle alors du théorème de Hahn–Banach (EVT, II, p. 49, cor. 3 (ii)).

Pour $h\in \mathscr{C}^{\infty}$(U), la transposée de l’application linéaire continue $\varphi \mapsto h\varphi$ de $\mathscr{D}(U)$ dans lui-même est une application linéaire continue de $\mathscr{D}'(U)$ dans lui-même, que l’on note $f\mapsto hf$. Cette définition est justifiée car si $f$ est la distribution associée à une mesure $\nu$ sur U, alors $hf$ est associée à la mesure $h\cdot \nu$. En effet, pour toute fonction test $\varphi \in \mathscr{D}$(U), on calcule

$$
\langle hf, \varphi \rangle =\langle f, h\varphi \rangle =\int_Uh\varphi d\nu =\int_U\varphi  d(h\cdot \nu )
$$

### 6. Dérivation des distributions

Soit $\alpha \in \mathbf{N}^n$. L’application linéaire $\varphi \mapsto \partial^{\alpha}\varphi$ est continue de $\mathscr{D}(U)$ dans $\mathscr{D}(U)$. Sa transposée $^t\partial^{\alpha}$ est une application linéaire continue de $\mathscr{D}'(U)$ dans $\mathscr{D}'(U)$ (EVT, IV, p. 6, cor., b)).

On note $\partial^{\alpha}$ l’application linéaire continue $(-1)^{|\alpha|t}\partial^{\alpha}$ de $\mathscr{D}'(U)$ dans lui-même.

#### Définition 2 {#ts-iv-s3-def-2 .statement tag=030T}

Si $f\in \mathscr{D}'(U)$ est une distribution, on dit que $\partial^{\alpha}f$ est la dérivée partielle itérée d’ordre $\alpha$ de $f$.

On a donc, par définition

$$
\langle \partial^{\alpha}f, \varphi \rangle = (-1)^{|\alpha|}\langle f, \partial^{\alpha}\varphi \rangle
$$

pour toute fonction $\varphi \in \mathscr{D}(U)$. On a $\partial^{\alpha+\beta}=\partial^{\alpha}\circ \partial^{\beta}$ pour tous $\alpha$ et $\beta$ dans $\mathbf{N}^n$.

Si $n= 1$, on notera aussi $f'$ la dérivée d’une distribution $f\in \mathscr{D}'(U)$.

La définition est justifiée par le lemme suivant.

#### Lemme 6 {#ts-iv-s3-lem-6 .statement tag=030U}

Soit $k$ un entier naturel. Soit $f\in \mathscr{C}^k(U)$ et soit $\lambda$ la distribution associée à $f$. Pour tout $\beta \in \mathbf{N}^n$ tel que $|\beta |\leqslant k$, la distribution $\partial^{\beta}\lambda$ est la distribution associée à la fonction $\partial^{\beta}f$.

Par récurrence sur $k$, il suffit de démontrer cette propriété lorsque $\beta$ vérifie $|\beta |= 1$, et on peut même supposer que $\beta = (0, . . . ,0,1)$. Puisque les distributions définissent un faisceau (prop. 5 de IV, p. 204), il suffit de vérifier l’assertion lorsqu’il existe un ouvert $V\subset \mathbf{R}^{n-1}$ et un intervalle ouvert $I\subset \mathbf{R}$ tels que $U = V\times I$.

Pour toute fonction test $\varphi \in \mathscr{D}$(U), on a par définition

$$
\langle \partial^{\beta}\lambda , \varphi \rangle =-\int_Uf(x)\partial^{\beta}\varphi (x)dx=-\int_V\int_If(y, t)\partial^{\beta}\varphi (y, t)dtdy
$$

d’après le théorème de Lebesgue–Fubini (INT, V, p. 96, § 8, n$^o4$, th. 1). Par intégration par parties (FVR, II, p. 10), on a

$$
-\int_If(y, t)\partial^{\beta}\varphi (y, t)dt=\int_I\partial^{\beta}f(y, t)\varphi (y, t)dt
$$

puisque $t\mapsto \varphi (y, t)$ est à support compact dans I. On obtient donc

$$
\langle \partial^{\beta}\lambda , \varphi \rangle =\int_V\int_I\partial^{\beta}f(y, t)\varphi (y, t)dtdy=\langle \partial^{\beta}f, \varphi \rangle
$$

#### Proposition 9 (Formule de Leibniz) {#ts-iv-s3-prop-9 .statement tag=030V}

Soient $f$ une distribution sur U et $g$ une fonction indéfiniment différentiable sur U. Soit $\alpha \in \mathbf{N}^n$. On a la relation

$$
\alpha (\alpha )\beta \alpha -\beta
$$

$$
\partial (f g) =\sum\partial f \partial g
$$

$$
\beta
$$

$\beta \leqslant \alpha$

En procédant par récurrence sur $|\alpha |$ comme dans la preuve de FVR, I, p. 28, prop. 2, il suffit de considérer le cas où $|\alpha |= 1$. Le résultat résulte alors du calcul

$$
\langle \partial^{\alpha}(f g), \varphi \rangle =\langle f g,-\partial^{\alpha}\varphi \rangle =\langle f,-g\partial^{\alpha}\varphi \rangle
$$

$$
=\langle f,-\partial^{\alpha}(g\varphi ) +\varphi \partial^{\alpha}g\rangle =\langle g\partial^{\alpha}f+f \partial^{\alpha}g, \varphi \rangle
$$

valide pour $\varphi \in \mathscr{D}(U)$.

### 7. Fonctions de Schwartz

On note $\mathscr{S}(\mathbf{R}^n)$ l’espace des fonctions indéfiniment dérivables $\varphi$ sur $\mathbf{R}^n$, à valeurs complexes, telles que, pour tous $\alpha$ et $\beta$ dans $\mathbf{N}^n$, la fonction $X^{\beta}\partial^{\alpha}\varphi$ est bornée sur $\mathbf{R}^n$. On munit $\mathscr{S}(\mathbf{R}^n)$ de la topologie localement convexe définie par la famille dénombrable de semi-normes $(q_{\alpha ,\beta})_{(\alpha ,\beta)\in\mathbf{N}^n\times\mathbf{N}^n}$, où $q_{\alpha ,\beta}$ est définie par

$q_{\alpha ,\beta}(\varphi ) =$ sup $|x^{\beta}\partial^{\alpha}\varphi (x)|=\|X^{\beta}\partial^{\alpha}\varphi \|_{\infty}$

$x\in \mathbf{R}^n$

pour $\varphi \in \mathscr{S}(\mathbf{R}^n)$. Cette topologie est séparée. Elle est également définie par les semi-normes $\widetilde{q}_{\alpha ,k}$ définies par

$\widetilde{q}_{\alpha ,k}(\varphi ) =$ sup $\|x\|^k|(\partial^{\alpha}\varphi )(x)|$.

$x\in \mathbf{R}^n$

pour tout $\varphi \in \mathscr{S}(\mathbf{R}^n)$, où $k\in \mathbf{N}$ et $\alpha \in \mathbf{N}^n$.

On dit que $\mathscr{S}(\mathbf{R}^n)$ est l’espace de Schwartz ou l’espace des fonctions de Schwartz sur $\mathbf{R}^n$.

#### Remarque {#ts-iv-s3-n7-rem-1 .statement tag=030W}

Soit $\varphi \in \mathscr{S}(\mathbf{R}^n)$. Pour tout $k\in \mathbf{N}$, on a

lim $\|x\|^k\varphi (x) = 0$,

$\|x\|\rightarrow +\infty$

puisque la fonction $x\mapsto  \|x\|^{k+1}\varphi (x)$ est bornée.

#### Exemple {#ts-iv-s3-n7-exa-1 .statement tag=030X}

La fonction $\gamma_n$ définie sur $\mathbf{R}^n$ par $\gamma_n(x) =$ exp($-\|x\|^2$) appartient à $\mathscr{S}(\mathbf{R}^n)$. En effet, on démontre par récurrence sur $k$ que, pour tout entier $k\in \mathbf{N}$, il existe un polynôme $P_k\in \mathbf{R}[X]$ tel que $\partial_k\gamma_1= P_k\gamma_1$.

Pour tous $\alpha = (\alpha_i)\in \mathbf{N}^n$ et $\beta = (\beta_i)\in \mathbf{N}^n$, et tout $x= (x_i)\in \mathbf{R}^n$, il vient alors

$$
|(X^{\beta}\partial^{\alpha}\gamma_n)(x)|=\prod_{i=1}^n|x_i|^{\beta_i}|P_{\alpha_i}(x_i)|\gamma_1(x_i)
$$

qui est une quantité bornée lorsque $x$ varie dans $\mathbf{R}^n$.

Soient $\alpha \in \mathbf{N}^n$ et $\beta \in \mathbf{N}^n$. Si $\varphi \in \mathscr{S}(\mathbf{R}^n)$, alors $X^{\beta}\partial^{\alpha}(\varphi )$ est encore une fonction de Schwartz ; l’application $\varphi \mapsto X^{\beta}\partial^{\alpha}\varphi$ ainsi définie de $\mathscr{S}(\mathbf{R}^n)$ dans lui-même est continue.

L’espace $\mathscr{S}(\mathbf{R}^n)$ est une algèbre topologique. Plus précisément, si $\varphi_1$ et $\varphi_2$ appartiennent à $\mathscr{S}(\mathbf{R}^n)$, alors $\varphi_1\varphi_2$ est une fonction de Schwartz telle que

$$
(\alpha )
$$

$$
q_{\alpha ,\beta}(\varphi_1\varphi_2)\leqslant \sum q_{\gamma ,\beta}(\varphi_1)q_{\alpha-\gamma ,0}(\varphi_2) \tag{2}
$$

$$
\gamma
$$

$0\leqslant \gamma \leqslant \alpha$

pour tous $\alpha$ et $\beta \in \mathbf{N}^n$ (prop. 1 de IV, p. 196).

L’inclusion canonique de $\mathscr{S}(\mathbf{R}^n)$ dans l’espace $\mathscr{C}^{\infty}(\mathbf{R}^n)$, muni de la topologie décrite dans le n$^o3$ de IV, p. 200, est continue, puisque

sup $|\partial^{\alpha}\varphi (x)|\leqslant q_{\alpha ,0}(\varphi )$

$x\in K$

pour toute partie compacte K de $\mathbf{R}^n$, tout $\alpha \in \mathbf{N}^n$ et toute fonction de Schwartz $\varphi$.

#### Lemme 7 {#ts-iv-s3-lem-7 .statement tag=030Y}

Soient $k\in \mathbf{N}$ et $\alpha \in \mathbf{N}^n$. Pour toute fonction $\varphi \in \mathscr{S}(\mathbf{R}^n)$ et tout nombre réel $T>0$, on a

$_k\alpha$ 1

(3) $\widetilde{q}_{\alpha ,k}(\varphi )\leqslant T$ sup $|\partial \varphi (x)|+\widetilde{q}_{\alpha ,k+1}(\varphi )$.

$\|x\|\leqslant T$ T En effet, on a

$\widetilde{q}_{\alpha ,k}(\varphi )\leqslant$ sup $\|x\|^k|\partial^{\alpha}\varphi (x)|+$ sup $\|x\|^k|\partial^{\alpha}\varphi (x)|$

$\|x\|\leqslant T\|x\|>T$

$k\alpha$ 1 $k+1\alpha$

$\leqslant T$ sup $|\partial \varphi (x)|+$ sup $\|x\||\partial \varphi (x)|$.

$$
\|x\|\leqslant TT\|x\|>T
$$

#### Proposition 10 {#ts-iv-s3-prop-10 .statement tag=030Z}

Soit B une partie bornée de $\mathscr{S}(\mathbf{R}^n)$. La topologie induite sur B par $\mathscr{S}(\mathbf{R}^n)$ coïncide avec la topologie induite par $\mathscr{C}^{\infty}(\mathbf{R}^n)$.

Comme l’inclusion de $\mathscr{S}(\mathbf{R}^n)$ dans $\mathscr{C}^{\infty}(\mathbf{R}^n)$ est continue, il suffit de démontrer que, pour toute partie ouverte V de $\mathscr{S}(\mathbf{R}^n)$, l’intersection $V\cap B$ est ouverte dans B pour la topologie induite par $\mathscr{C}^{\infty}(\mathbf{R}^n)$.

Soit V une partie ouverte de $\mathscr{S}(\mathbf{R}^n)$. Soit $\varphi_0\in V\cap B$. Il existe un ensemble fini I, une famille $(\alpha_i, k_i)_{i\in I}\in (\mathbf{N}^n\times \mathbf{N})^I$ et un nombre réel $\varepsilon  >0$ tels que V contient l’ensemble des $\varphi \in \mathscr{S}(\mathbf{R}^n)$ vérifiant

sup$_{i\in I}\widetilde{q}_{\alpha_i,k_i}(\varphi -\varphi_0)\leqslant \varepsilon$.

Puisque B est bornée dans $\mathscr{S}(\mathbf{R}^n)$, il existe $M>0$ tel que les semi-normes $\widetilde{q}_{\alpha_i,k_i+1}$ pour $i\in I$ sont bornées par M sur B. Soient $\delta  >0$ et $T>0$ des nombres réels. D’après l’inégalité (3), dès lors que $\varphi \in B$ vérifie la majoration

(4) sup sup $|\partial^{\alpha_i}(\varphi -\varphi_0)|\leqslant \delta$,

$i\in I\|x\|\leqslant T$

on a

$_k$ 2M

sup $\widetilde{q}_{\alpha_i,k_i}(\varphi -\varphi_0)\leqslant \delta T$ +.

$_{i\in I}$ T

Posons $T =^{4M}_{\varepsilon}$, puis $\delta =_{2T}^{\varepsilon_k}$. On constate que $V\cap B$ contient le voisinage de $\varphi_0$ dans B pour la topologie induite par $\mathscr{C}^{\infty}(\mathbf{R}^n)$ qui est défini par (4). Cela conclut la preuve.

#### Corollaire {#ts-iv-s3-n7-cor-1 .statement tag=0310}

Soit $(\varphi_m)_{m\in\mathbf{N}}$ une suite bornée dans $\mathscr{S}(\mathbf{R}^n)$. Pour toute fonction $\varphi \in \mathscr{S}(\mathbf{R}^n)$, les assertions suivantes sont équivalentes :

a) La suite $(\varphi_m)$ converge vers $\varphi$ dans $\mathscr{S}(\mathbf{R}^n)$;

b) La suite $(\varphi_m)$ converge vers $\varphi$ dans $\mathscr{C}^{\infty}(\mathbf{R}^n)$.

#### Remarque {#ts-iv-s3-n7-rem-2 .statement tag=0311}

Une suite $(\varphi_m)$ dans $\mathscr{C}^{\infty}(\mathbf{R}^n)$ converge si et seulement si, pour tout $\alpha \in \mathbf{N}^n$, la suite $(\partial^{\alpha}\varphi_m)$ converge vers une fonction $\varphi^{(\alpha)}$ dans $\mathscr{C}(\mathbf{R}^n)$ muni de la topologie de la convergence compacte. On a alors $\varphi^{(\alpha)}=\partial^{\alpha}\varphi$ et $(\varphi_m)$ converge vers $\varphi$[^0].

En effet, la condition est nécessaire. Réciproquement, si les suites $(\partial^{\alpha}\varphi_m)$ convergent vers des fonctions $\varphi^{(\alpha)}$ pour tout $\alpha \in \mathbf{N}^n$, alors il résulte de FVR, II, p. 2, th. 1, que $\varphi^{(\alpha)}=\partial^{\alpha}\varphi$[^0], ce qui signifie que la suite $(\varphi_m)$ converge vers $\varphi$[^0] dans $\mathscr{C}^{\infty}(\mathbf{R}^n)$.

#### Proposition 11 {#ts-iv-s3-prop-11 .statement tag=0312}

L’espace $\mathscr{S}(\mathbf{R}^n)$ est un espace de Fréchet et un espace de Montel.

Comme l’espace $\mathscr{C}^{\infty}(\mathbf{R}^n)$ est complet (EVT, III, p. 9, exemple b)), le corollaire de la proposition 10 implique que toute suite de Cauchy dans $\mathscr{S}(\mathbf{R}^n)$ converge dans $\mathscr{S}(\mathbf{R}^n)$ puisqu’elle est bornée et qu’elle converge dans $\mathscr{C}^{\infty}(\mathbf{R}^n)$.

L’espace $\mathscr{S}(\mathbf{R}^n)$ est donc un espace de Fréchet ; en particulier, il est tonnelé (EVT, III, p. 25, cor. de la prop. 2). Soit B une partie bornée de $\mathscr{S}(\mathbf{R}^n)$ et $(\varphi_m)_{m\in\mathbf{N}}$ une suite à valeurs dans B. Puisque $\mathscr{C}^{\infty}(\mathbf{R}^n)$ est un espace de Montel (EVT, IV, p. 18, exemple (4)), il existe une sous-suite de $(\varphi_m)_{m\in\mathbf{N}}$ qui converge dans $\mathscr{C}^{\infty}(\mathbf{R}^n)$, donc dans $\mathscr{S}(\mathbf{R}^n)$ (proposition 10). Donc B est relativement compacte dans $\mathscr{S}(\mathbf{R}^n)$. Il en résulte que $\mathscr{S}(\mathbf{R}^n)$ est un espace de Montel.

### 8. Inclusions d’espaces fonctionnels dans l’espace des fonctions de Schwartz

#### Proposition 12 {#ts-iv-s3-prop-12 .statement tag=0313}

L’espace $\mathscr{D}(\mathbf{R}^n)$ est contenu dans $\mathscr{S}(\mathbf{R}^n)$, et l’inclusion de $\mathscr{D}(\mathbf{R}^n)$ dans $\mathscr{S}(\mathbf{R}^n)$ est continue avec image dense.

Soit $B\subset \mathscr{D}(\mathbf{R}^n)$ une partie bornée, et soit K une partie compacte de $\mathbf{R}^n$ telle que $B\subset \mathscr{C}_K^{\infty}(\mathbf{R}^n)$. Soient $\alpha \in \mathbf{N}^n$ et $k\in \mathbf{N}$. Pour toute fonction $\varphi \in B$, il vient

$\widetilde{q}_{\alpha ,k}(\varphi )\leqslant$ sup$\|x\|^kp_{\alpha ,K}(\varphi )$,

$x\in K$

donc B est borné dans $\mathscr{S}(\mathbf{R}^n)$. La continuité de l’inclusion résulte alors du fait que les espaces $\mathscr{S}(\mathbf{R}^n)$ et $\mathscr{D}(\mathbf{R}^n)$ sont bornologiques.

Démontrons que $\mathscr{D}(\mathbf{R}^n)$ est dense dans $\mathscr{S}(\mathbf{R}^n)$. Soient B la boule unité de $\mathbf{R}^n$ et $\eta \in \mathscr{D}(\mathbf{R}^n)$ une fonction test à support contenu dans 2B telle que $0\leqslant \eta \leqslant 1$ et $\eta (x) = 1$ pour tout $x\in B$ (lemme 1, a) de IV, p. 196).

Soit $\varphi \in \mathscr{S}(\mathbf{R}^n)$. Pour tout entier $m\geqslant 1$ et tout $x\in \mathbf{R}^n$, posons $\eta_m(x) =\eta (x/m)$. Définissons enfin $\varphi_m=\eta_m\varphi$; on a $\varphi_m\in \mathscr{D}(\mathbf{R}^n)$. Comme $\partial^{\alpha}\eta_m=m^{-|\alpha|}(\partial^{\alpha}\eta )(x/m)$ pour tous $\alpha \in \mathbf{N}^n$ et $x\in \mathbf{R}^n$, on déduit de la formule (2) de IV, p. 210 que la suite $(\varphi_m)$ est bornée dans $\mathscr{S}(\mathbf{R}^n)$.

Soit C une partie compacte de $\mathbf{R}^n$. La suite $(\varphi_m)_{m\geqslant 1}$ converge vers $\varphi$ dans $\mathscr{C}_K^{\infty}(\mathbf{R}^n)$ puisque $\varphi_m$ coïncide avec $\varphi$ sur C pour tout $m$ suffisamment grand. Ainsi la suite $(\varphi_m)$ converge vers $\varphi$ dans $\mathscr{C}^{\infty}(\mathbf{R}^n)$, et le corollaire de la proposition 10 de IV, p. 211 permet de conclure que la suite $(\varphi_m)$ converge vers $\varphi$ dans $\mathscr{S}(\mathbf{R}^n)$.

#### Lemme 8 {#ts-iv-s3-lem-8 .statement tag=0314}

Soit B une partie bornée de $\mathscr{D}(\mathbf{R}^n)$. La topologie induite sur B par la topologie de $\mathscr{S}(\mathbf{R}^n)$ coïncide avec la topologie induite par $\mathscr{D}(\mathbf{R}^n)$.

Puisque l’inclusion de $\mathscr{D}(\mathbf{R}^n)$ dans $\mathscr{S}(\mathbf{R}^n)$ est continue, la topologie sur B induite par $\mathscr{D}(\mathbf{R}^n)$ est plus fine que celle induite par $\mathscr{S}(\mathbf{R}^n)$. Par ailleurs, il existe une partie compacte K de $\mathbf{R}^n$ telle que $B\subset \mathscr{C}_K^{\infty}(\mathbf{R}^n)$. Pour tout $\alpha \in \mathbf{N}^n$, on a alors $p_{\alpha ,K}(\varphi )\leqslant \widetilde{q}_{\alpha ,0}(\varphi )$, ce qui implique que la topologie induite par $\mathscr{S}(\mathbf{R}^n)$ est plus fine que celle induite par $\mathscr{D}(\mathbf{R}^n)$.

#### Proposition 13 {#ts-iv-s3-prop-13 .statement tag=0315}

Soit $p\in [1,+\infty ]$. L’espace $\mathscr{S}(\mathbf{R}^n)$ est contenu dans $\mathscr{L}^p(\mathbf{R}^n)$ et l’injection canonique de $\mathscr{S}(\mathbf{R}^n)$ dans $\mathscr{L}^p(\mathbf{R}^n)$ est continue. L’image de $\mathscr{S}(\mathbf{R}^n)$ dans $L^p(\mathbf{R}^n)$ est dense si $p\not = +\infty$.

La première assertion est immédiate pour $p= +\infty$. Supposons désormais que $p\in [1,+\infty [$. Soit $m$ un entier tel que $n+ 1< mp$. Pour tout $\varphi \in \mathscr{S}(\mathbf{R}^n)$ et $x\in \mathbf{R}^n$, on a

$$
\|x\|^{n+1}|\varphi (x)|^p\leqslant \widetilde{q}_{0,m}(\varphi )^p
$$

donc $\varphi \in \mathscr{L}^p(\mathbf{R}^n)$ d’après la prop. 3 de IV, p. 199. De plus, on obtient

$$
N_p(\varphi )\leqslant a^{1/p}_n\widetilde{q}_{0,0}(\varphi ) +b_n\widetilde{q}_{0,m}(\varphi )
$$

où

$\int\int$ 1

$$
a_n=d\mu(x),b_n=n_{+1}d\mu(x)
$$

$$
_{\|x\|\leqslant 1}\|_{x\|\geqslant 1}\|x\|
$$

donc l’injection de $\mathscr{S}(\mathbf{R}^n)$ dans $\mathscr{L}^p(\mathbf{R}^n)$ est continue.

Comme l’espace $\mathscr{D}(\mathbf{R}^n)$ est contenu dans $\mathscr{S}(\mathbf{R}^n)$, la proposition 4 de IV, p. 202 implique que $\mathscr{S}(\mathbf{R}^n)$ est dense dans $L^p(\mathbf{R}^n)$ si $p\not = +\infty$.

### 9. Fonctions à croissance polynomiale

#### Définition 3 {#ts-iv-s3-def-3 .statement tag=0316}

Une fonction $f:\mathbf{R}^n\rightarrow \mathbf{C}$ est à croissance polynomiale s’il existe un entier $k\geqslant 1$ tel que l’application définie par $x\mapsto (1 +\|x\|)^{-k}f(x)$ est bornée sur $\mathbf{R}^n$.

Toute fonction à croissance polynomiale est localement bornée. Toute fonction polynomiale sur $\mathbf{R}^n$ est à croissance polynomiale.

#### Proposition 14 {#ts-iv-s3-prop-14 .statement tag=0317}

Soit $f\in \mathscr{C}^{\infty}(\mathbf{R}^n)$. On suppose que pour tout $\alpha$ dans $\mathbf{N}^n$, la fonction $\partial^{\alpha}f$ est à croissance polynomiale. L’application linéaire de l’espace $\mathscr{S}(\mathbf{R}^n)$ dans lui-même définie par $\varphi \mapsto f \varphi$ est continue.

Pour tout $\varphi$ dans $\mathscr{S}(\mathbf{R}^n)$, la fonction $f \varphi$ appartient à $\mathscr{C}^{\infty}(\mathbf{R}^n)$. Par hypothèse, pour tout $\alpha \in \mathbf{N}^n$, il existe un entier $k_{\alpha}\geqslant 0$ et un réel $C_{\alpha}$ tel que $|\partial^{\alpha}f(x)|\leqslant C_{\alpha}(1 +\|x\|)^{k_{\alpha}}$ pour tout $x$ dans $\mathbf{R}^n$. Soit $\varphi \in \mathscr{S}(\mathbf{R}^n)$. Soient $\alpha \in \mathbf{N}^n$ et $k\in \mathbf{N}$. D’après la prop. 1 de IV, p. 196, il vient

$$
(\alpha )k\beta \alpha -\beta
$$

$\widetilde{q}_{\alpha ,k}(f \varphi )\leqslant \sum$ sup $\|x\||\partial f(x)\partial \varphi (x)|$

$$
\beta_{x\in\mathbf{R}^n}
$$

$0\leqslant \beta \leqslant \alpha$

$$
(\alpha )kk\alpha -\beta
$$

$\leqslant \sum C_{\beta}$ sup $\|x\|(1 +\|x\|)^{^{\beta}}|\partial \varphi (x)|$.

$$
\beta_{x\in\mathbf{R}^n}
$$

$0\leqslant \beta \leqslant \alpha$

Soit $\beta \in \mathbf{N}^n$ tel que $0\leqslant \beta \leqslant \alpha$. Pour tout $x\in \mathbf{R}^n$, on a

$\|x\|^k(1 +\|x\|)^{k_{\beta}}|\partial^{\alpha-\beta}\varphi (x)|\leqslant$ sup $2^{k_{\beta}}|\partial^{\alpha-\beta}\varphi (x)|$

$\|x\|\leqslant 1$

+ sup $2^{k_{\beta}}\|x\|^{k+k_{\beta}}|\partial^{\alpha-\beta}\varphi (x)|$

$x\in \mathbf{R}^n$

d’où finalement

$$
(\alpha )_k
$$

$$
\widetilde{q}_{\alpha ,k}(f \varphi )\leqslant \sum 2^{^{\beta}}C_{\beta}\widetilde{q}_{\alpha-\beta ,0}(\varphi ) +\widetilde{q}_{\alpha-\beta ,k+k_{\beta}}(\varphi )
$$

$$
\beta
$$

$0\leqslant \beta \leqslant \alpha$

ce qui implique la proposition.

### 10. Distributions tempérées

#### Définition 4 {#ts-iv-s3-def-4 .statement tag=0318}

On appelle espace des distributions tempérées sur $\mathbf{R}^n$ l’espace dual de $\mathscr{S}(\mathbf{R})$ muni de la topologie de la convergence bornée. On le note $\mathscr{S}'(\mathbf{R}^n)$.

Puisque $\mathscr{S}(\mathbf{R}^n)$ est bornologique, l’espace $\mathscr{S}'(\mathbf{R}^n)$ est complet (EVT, III, p. 24, cor. 1). Comme $\mathscr{S}(\mathbf{R}^n)$ est un espace de Montel, il en est de même de $\mathscr{S}'(\mathbf{R}^n)$ (EVT, IV, p. 19, prop. 9). L’espace $\mathscr{S}'(\mathbf{R}^n)$ est donc réflexif (EVT, IV, p. 16, th. 2).

#### Lemme 9 {#ts-iv-s3-lem-9 .statement tag=0319}

Une application linéaire $f$ de $\mathscr{S}(\mathbf{R}^n)$ dans $\mathbf{C}$ est une distribution tempérée si et seulement si pour toute famille $(M_{\alpha ,k})_{(\alpha ,k)\in\mathbf{N}^n\times\mathbf{N}}$ dans $\mathbf{R}_+$, la forme linéaire $f$ est bornée sur l’ensemble des fonctions $\varphi \in \mathscr{S}(\mathbf{R}^n)$ telles que $\widetilde{q}_{\alpha ,k}(\varphi )\leqslant M_{\alpha ,k}$ pour tout $(\alpha , k)\in \mathbf{N}^n\times \mathbf{N}$.

En effet, l’espace $\mathscr{S}(\mathbf{R}^n)$ est bornologique (EVT, III, p. 12, prop. 2) et toute partie bornée de $\mathscr{S}(\mathbf{R}^n)$ est contenue dans l’un des ensembles bornés décrits dans l’énoncé.

#### Lemme 10 {#ts-iv-s3-lem-10 .statement tag=031A}

Soit $\mathfrak{F}$ un filtre sur $\mathscr{S}'(\mathbf{R}^n)$ ayant une base dénombrable ou contenant un ensemble simplement borné. Alors $\mathfrak{F}$ converge vers une distribution tempérée si et seulement si $\langle f, \varphi \rangle$ converge selon $\mathfrak{F}$ pour toute fonction de Schwartz $\varphi$.

En particulier, une suite $(f_m)_{m\in\mathbf{N}}$ de distributions tempérées converge vers une distribution tempérée $f$ si et seulement si on a $\langle f_m, \varphi \rangle  \rightarrow  \langle f, \varphi \rangle$ pour tout $\varphi \in \mathscr{S}(\mathbf{R}^n)$.

Comme $\mathscr{S}'(\mathbf{R}^n)$ est un espace de Fréchet, donc tonnelé, (EVT, III, p. 25, cor. de la prop. 2) le lemme résulte du théorème de Banach– Steinhaus (EVT, III, p. 26, cor. 3 du th. 1).

L’injection canonique $j$ de $\mathscr{D}(\mathbf{R}^n)$ dans $\mathscr{S}(\mathbf{R}^n)$ est continue et son image est dense (lemme 12 de IV, p. 212), donc la transposée de $j$, qui est l’application de restriction des distributions tempérées au sous-espace $\mathscr{D}(\mathbf{R}^n)$, est une application linéaire injective continue de $\mathscr{S}'(\mathbf{R}^n)$ dans $\mathscr{D}'(\mathbf{R}^n)$. On identifiera $\mathscr{S}'(\mathbf{R}^n)$ à un sous-espace de $\mathscr{D}'(\mathbf{R}^n)$ par le biais de cette application.

Soit $\alpha \in \mathbf{N}^n$. L’application linéaire $\varphi \mapsto \partial^{\alpha}\varphi$ de $\mathscr{S}(\mathbf{R}^n)$ dans $\mathscr{S}(\mathbf{R}^n)$ est continue. Sa transposée est donc une application linéaire continue de $\mathscr{S}'(\mathbf{R}^n)$ dans $\mathscr{S}'(\mathbf{R}^n)$ (EVT, IV, p. 6, cor., b)). On note $\partial^{\alpha}$ l’application linéaire continue $(-1)^{|\alpha|t}\partial^{\alpha}$ de $\mathscr{S}'(\mathbf{R}^n)$ dans $\mathscr{S}'(\mathbf{R}^n)$. Cette définition est compatible avec la définition 2 de IV, p. 208 pour les distributions.

Soit $h\in \mathscr{C}^{\infty}(\mathbf{R}^n)$ une fonction telle que $\partial^{\alpha}h$ est à croissance polynomiale pour tout $\alpha \in \mathbf{N}^n$. La transposée de l’application linéaire continue $\varphi \mapsto h\varphi$ (prop. 14 de IV, p. 214) est une application linéaire continue sur $\mathscr{S}'(\mathbf{R}^n)$, notée $f\mapsto hf$.

### 11. Interprétation de fonctions comme distributions tempé- rées

#### Définition 5 {#ts-iv-s3-def-5 .statement tag=031B}

Une mesure $\nu$ sur $\mathbf{R}^n$ est dite tempérée s’il existe un entier $r\in \mathbf{N}$ tel que l’application continue $x\mapsto (1 +\|x\|)^{-r}$ est $\nu$-intégrable sur $\mathbf{R}^n$.

Autrement dit, une mesure $\nu$ est tempérée s’il existe $r\in \mathbf{N}$ tel que la fonction définie par $x\mapsto  \|x\|^{-r}$ est $\nu$-intégrable sur le complémentaire de la boule unité dans $\mathbf{R}^n$. En particulier, toute mesure bornée sur $\mathbf{R}^n$ est tempérée. Plus généralement, si $f$ est une fonction $\mu$-mesurable à croissance polynomiale et si $\nu$ est tempérée, alors la mesure $f\cdot \nu$ est tempérée.

L’ensemble $\mathscr{M}^t(\mathbf{R}^n)$ des mesures tempérées sur $\mathbf{R}^n$ est un sous-espace vectoriel de l’espace $\mathscr{M}(\mathbf{R}^n;\mathbf{C})$ des mesures complexes sur $\mathbf{R}^n$.

#### Proposition 15 {#ts-iv-s3-prop-15 .statement tag=031C}

Soit $\nu$ une mesure tempérée sur $\mathbf{R}^n$. La restriction de $\nu$ à $\mathscr{S}(\mathbf{R}^n)$ est une distribution tempérée. Elle est nulle si et seulement si la mesure $\nu$ est nulle.

Puisque $\nu$ est tempérée, il existe un entier positif $k$ tel que l’application $x\mapsto  \|x\|^{-k}$ est $\nu$-intégrable sur le complémentaire de la boule unité dans $\mathbf{R}^n$. Pour toute fonction de Schwartz $\varphi \in \mathscr{S}(\mathbf{R}^n)$, on a

$$
|\langle \nu , \varphi \rangle |\leqslant \int_{\|x\|\leqslant 1}d\nu \widetilde{q}_{0,0}(\varphi ) +\int_{\|x\|>1}\|x\|^{-k}d\nu \widetilde{q}_{0,k}(\varphi )
$$

donc la restriction de $\nu$ à $\mathscr{S}(\mathbf{R}^n)$ est une distribution tempérée.

La dernière assertion résulte de la prop. 6 de IV, p. 206 puisque $\mathscr{D}(\mathbf{R}^n)$ est contenu dans $\mathscr{S}(\mathbf{R}^n)$.

On identifiera l’espace $\mathscr{M}^t(\mathbf{R}^n)$ à un sous-espace de $\mathscr{S}'(\mathbf{R}^n)$.

#### Proposition 16 {#ts-iv-s3-prop-16 .statement tag=031D}

Soit $p\in [1,+\infty ]$ et $f\in \mathscr{L}^p(\mathbf{R}^n)$. Alors la mesure $f\cdot \mu$ de densité $f$ par rapport à la mesure de Lebesgue est tempérée. L’application $f\mapsto f\cdot \mu$ de $L^p(\mathbf{R}^n)$ dans $\mathscr{S}'(\mathbf{R}^n)$ ainsi définie est continue.

Soit $q$ l’exposant conjugué de $p$ et soit $r\geqslant 0$ tel que $rq > n$. Pour tout $x\in \mathbf{R}^n$, notons $g(x) = (1 +\|x\|)^{-r}$. La fonction $g$ appartient à $\mathscr{L}^q(\mathbf{R}^n)$ d’après la prop. 3 de IV, p. 199. D’après l’inégalité de Hölder, on a

$$
\int_{\mathbf{R}}^{*_n}(1 +\|x\|)^{-r}|f(x)|d\mu(x)\leqslant N_q(g)N_p(f)<+\infty
$$

donc la mesure $f\cdot \mu$ est tempérée.

Soit $f\in L^p(\mathbf{R}^n)$ et $\varphi \in \mathscr{S}(\mathbf{R}^n)$. L’inégalité de Hölder implique

$$
|\langle f\cdot \mu, \varphi \rangle |=\int_{\mathbf{R}^n}f(x)\varphi (x)d\mu(x)\leqslant \|f\|_p\|\varphi \|_q
$$

et la continuité de l’application $f\mapsto f\cdot \mu$ résulte alors de la prop. 13 de IV, p. 213.

Pour tout $p\in [1,+\infty ]$, on identifiera $L^p(\mathbf{R}^n)$ à un sous-espace de $\mathscr{S}'(\mathbf{R}^n)$ par l’application linéaire $f\mapsto f\cdot \mu$.

#### Proposition 17 {#ts-iv-s3-prop-17 .statement tag=031E}

Les espaces $\mathscr{D}(\mathbf{R}^n)$ et $\mathscr{S}(\mathbf{R}^n)$ sont denses dans $\mathscr{S}'(\mathbf{R}^n)$.

Il suffit de démontrer que $\mathscr{D}(\mathbf{R}^n)$ est dense dans $\mathscr{S}'(\mathbf{R}^n)$. Soit $\lambda$ une forme linéaire continue sur $\mathscr{S}'(\mathbf{R}^n)$ nulle sur $\mathscr{D}(\mathbf{R}^n)$. Comme l’espace $\mathscr{S}(\mathbf{R}^n)$ est réflexif, il existe une fonction $\varphi \in \mathscr{S}(\mathbf{R}^n)$ telle que $\lambda (f) =\langle f, \varphi \rangle$ pour tout $f\in \mathscr{S}'(\mathbf{R}^n)$. On a donc

$$
0 =\lambda (\psi ) =\langle \psi , \varphi \rangle =\int_{\mathbf{R}^n}\psi \varphi  d\mu
$$

pour tout $\psi \in \mathscr{D}(\mathbf{R}^n)$. La mesure $\varphi \cdot \mu$ sur $\mathbf{R}^n$ est donc nulle (prop. 6 de IV, p. 206), d’où $\varphi = 0$. La proposition découle alors du théorème de Hahn–Banach (EVT, II, p. 46, cor. 1).

### 12. Transformation de Fourier des distributions tempérées

Comme toute fonction de Schwartz $\varphi$ est intégrable sur $\mathbf{R}^n$ (prop. 13 de IV, p. 213), elle admet une transformée de Fourier $\mathscr{F}(\varphi )$ (resp. une cotransformée de Fourier $\mathscr{F}(\varphi ))$ qui s’identifie à la fonction continue et bornée sur $\mathbf{R}^n$ définie par

$y\mapsto \int\varphi (x)$ exp($-2i\pi  x\cdot y$)$d\mu(x)$

(resp. à la fonction $y\mapsto \int^{\mathbf{R}^n}_{\mathbf{R}^n}\varphi (x)$ exp(2$i\pi  x\cdot y)d\mu(x))$.

#### Lemme 11 {#ts-iv-s3-lem-11 .statement tag=031F}

Soit $\varphi \in \mathscr{S}(\mathbf{R}^n)$. La fonction $\mathscr{F}(\varphi )$ est indéfiniment dérivable sur $\mathbf{R}^n$ et on a

$$
\mathscr{F}(X^{\alpha}\varphi ) = (-2i\pi )^{-|\alpha|}\partial^{\alpha}(\mathscr{F}(\varphi ))
$$

$$
\mathscr{F}(\partial^{\alpha}\varphi ) = (2i\pi )^{|\alpha|}X^{\alpha}\mathscr{F}(\varphi )
$$

pour tout $\alpha$ dans $\mathbf{N}^n$.

On peut supposer que $n\geqslant 1$. Soit $\varphi \in \mathscr{S}(\mathbf{R}^n)$. La fonction définie par $(x, y)\mapsto \varphi (x)$ exp(2$i\pi x\cdot y)$ de $\mathbf{R}^n\times \mathbf{R}^n$ dans $\mathbf{C}$ vérifie les hypothèses du corollaire 1 de IV, p. 198 pour tout entier $k$. La transformée de Fourier de $\varphi$ est donc indéfiniment dérivable et vérifie

$\partial^{\alpha}(\mathscr{F}\varphi )(y) = (-2i\pi )^{|\alpha|}\int_{\mathbf{R}^n}x^{\alpha}\varphi (x)$ exp($-2i\pi x\cdot y$)$d\mu(x)$

pour tout $y\in \mathbf{R}^n$, ce qui implique la première formule.

Démontrons la seconde formule. Par récurrence sur $|\alpha |$, il suffit de le faire lorsque $|\alpha |= 1$, et on se ramène aisément au cas $\alpha = (1,0, . . . ,0)$. Écrivons tout $x\in \mathbf{R}^n$ sous la forme $x= (x_1, x')$ avec $x'\in \mathbf{R}^{n-1}$, et notons $\mu_1$ (resp. $\mu')$ la mesure de Lebesgue sur $\mathbf{R}^{n-1}$ (resp. $\mathbf{R})$. D’après le théorème de Lebesgue–Fubini (INT, V, p. 96, § 8, n$^o4$, th. 1), pour tout $y= (y_1, y')\in \mathbf{R}\times \mathbf{R}^{n-1}$, il vient

$\mathscr{F}(\partial_1\varphi )(y) =\int$ exp($-2i\pi  x'\cdot y'$)

$\times \int^{\mathbf{R}^{n-1}}_{\mathbf{R}}(\partial_1\varphi )(x_1, x')$ exp($-2i\pi  x_1y_1$)$d\mu_1(x_1)d\mu'(x')$.

Pour tout intervalle compact $[a, b]$ dans $\mathbf{R}$ et tout $x'\in \mathbf{R}^{n-1}$, on a

$\int_a^b(\partial_1\varphi )(x_1, x')$ exp($-2i\pi  x_1y_1$)$d\mu_1(x_1) =$

$\varphi (x_1, x')$ exp($-2i\pi  x_1y_1$)$^b_a$

$+ 2i\pi y_1\int_a^b\varphi (x_1, x')$ exp($-2i\pi x_1y_1$)$d\mu_1(x_1)$ par intégration par parties (FVR, II, p. 10, formule (10)). Lorsque $a$ tend vers $-\infty$ et $b$ tend vers $+\infty$, le premier terme du second membre converge vers 0 puisque $\varphi \in \mathscr{S}(\mathbf{R}^n)$. Le second terme converge d’après le théorème de Lebesgue (INT, IV, p. 137, § 3, n$^o7$, th. 6) vers

$2i\pi y_1\int_{\mathbf{R}}\varphi (x_1, x')$ exp($-2i\pi x_1y_1$)$d\mu_1(x_1)$,

puisque l’application $x_1\mapsto \varphi (x_1, x')$ est intégrable sur $\mathbf{R}$. Comme $x_1\mapsto \partial_1\varphi (x_1, x')$ est aussi intégrable sur $\mathbf{R}$, on en déduit que

$\int_{\mathbf{R}}\partial_1\varphi (x_1, x')$ exp($-2i\pi x_1y_1$)$d\mu_1(x_1)$

$= 2i\pi y_1\int_{\mathbf{R}}\varphi (x_1, x')$ exp($-2i\pi x_1y_1$)$d\mu_1(x_1)$ et finalement, en appliquant de nouveau le théorème de Lebesgue–Fubini on conclut que

$\mathscr{F}(\partial_1\varphi )(y) = 2i\pi y_1\int_{\mathbf{R}^n}\varphi (x)$ exp($-2i\pi  x\cdot y$)$d\mu(x)$,

comme désiré.

#### Proposition 18 {#ts-iv-s3-prop-18 .statement tag=031G}

La restriction à $\mathscr{S}(\mathbf{R}^n)$ de la transformation de Fourier est un automorphisme d’espaces vectoriels topologiques dont l’inverse est la restriction de la cotransformation de Fourier.

Soit $\varphi \in \mathscr{S}(\mathbf{R}^n)$. D’après le lemme précédent, la transformée de Fourier de $\varphi$ appartient à $\mathscr{C}^{\infty}(\mathbf{R}^n)$. De plus, pour $\alpha \in \mathbf{N}^n$ et $\beta \in \mathbf{N}^n$, on a

$$
X^{\beta}\partial^{\alpha}(\mathscr{F}(\varphi )) = (-2i\pi )^{|\alpha|}X^{\beta}\mathscr{F}(X^{\alpha}\varphi )
$$

$$
= (-1)^{|\alpha|}(2i\pi )^{|\alpha|-|\beta|}\mathscr{F}(\partial^{\beta}(X^{\alpha}\varphi ))
$$

En particulier, la fonction $X^{\beta}\partial^{\alpha}(\mathscr{F}(\varphi ))$ est bornée. Puisque $\alpha$ et $\beta$ sont arbitraires dans $\mathbf{N}^n$, cela signifie que $\mathscr{F}(\varphi )$ appartient à $\mathscr{S}(\mathbf{R}^n)$. De plus, ce calcul implique

$$
q_{\alpha ,\beta}(\mathscr{F}(\varphi ))\leqslant (2\pi )^{|\alpha|-|\beta|}\|\partial^{\beta}(X^{\alpha}\varphi )\|_1
$$

pour $(\alpha , \beta )\in \mathbf{N}^n\times \mathbf{N}^n$ et $\varphi \in \mathscr{S}(\mathbf{R}^n)$.

Comme l’inclusion de l’espace $\mathscr{S}(\mathbf{R}^n)$ dans $L^1(\mathbf{R}^n)$ est continue (prop. 13 de IV, p. 213), l’application $q_{\alpha ,\beta}\circ \mathscr{F}$ de $\mathscr{S}(\mathbf{R}^n)$ dans $\mathbf{R}$ est continue. Il en résulte que la transformation de Fourier est continue de l’espace $\mathscr{S}(\mathbf{R}^n)$ dans lui-même (cf. EVT, II, p. 7, prop. 5, c)). On vérifie de même que la cotransformation de Fourier est continue de l’espace $\mathscr{S}(\mathbf{R}^n)$ dans lui-même. D’après la formule d’inversion de Fourier (théorème 3 de II, p. 222), la transformation de Fourier et la cotransformation de Fourier sont des isomorphismes réciproques l’un de l’autre.

#### Définition 6 {#ts-iv-s3-def-6 .statement tag=031H}

On appelle transformation de Fourier (resp. cotransformation de Fourier) sur $\mathscr{S}'(\mathbf{R}^n)$ la transposée de la transformation de Fourier sur $\mathscr{S}(\mathbf{R}^n) ($resp. de la cotransformation de Fourier).

On note encore $\mathscr{F}$ (resp. $\mathscr{F})$ la transformation de Fourier (resp. la cotransformation de Fourier) sur $\mathscr{S}'(\mathbf{R}^n)$. La transformation de Fourier sur $\mathscr{S}'(\mathbf{R}^n)$ est donc un automorphisme d’espaces vectoriels topologiques dont l’inverse est la cotransformation de Fourier. Pour tout $f\in \mathscr{S}'(\mathbf{R}^n)$, la distribution tempérée $\mathscr{F}(f)$ (resp. $\mathscr{F}(f))$ est définie par la formule

$\langle \mathscr{F}(f), \varphi \rangle =\langle f,\mathscr{F}(\varphi )\rangle$ resp. $\langle \mathscr{F}(f), \varphi \rangle =\langle f,\mathscr{F}(\varphi )\rangle$

pour tout $\varphi \in \mathscr{S}(\mathbf{R}^n)$.

#### Proposition 19 {#ts-iv-s3-prop-19 .statement tag=031I}

Soit $f$ une distribution tempérée associée à une mesure bornée $\nu \in \mathscr{M}^1(\mathbf{R}^n) ($resp. à $g\in L^2(\mathbf{R}^n))$. La transformée de Fourier de $f$ dans $\mathscr{S}'(\mathbf{R}^n)$ est la distribution tempérée associée à la transformée de Fourier de la mesure $\nu ($resp. à la transformée de Fourier de $g)$.

Soit $\nu$ une mesure bornée sur $\mathbf{R}^n$ et $f$ la distribution tempérée associée à $\nu$. La transformée de Fourier $\mathscr{F}(\nu )$ est une fonction continue et bornée sur $\mathbf{R}^n$ (prop. 3 de II, p. 207). La distribution tempérée associée à cette fonction vérifie

$$
\langle \mathscr{F}(\nu ), \varphi \rangle =\int_{\mathbf{R}^n}\mathscr{F}(\nu )\varphi  d\mu=\int_{\mathbf{R}^n}\mathscr{F}(\varphi )d\nu =\langle f,\mathscr{F}(\varphi )\rangle =\langle \mathscr{F}(f), \varphi \rangle
$$

pour tout $\varphi \in \mathscr{S}(\mathbf{R}^n)$, où la seconde égalité est la prop. 13 de II, p. 221, qui est applicable ici puisque la mesure $\varphi \cdot \mu$ est bornée. La distribution tempérée associée à $\mathscr{F}(\nu )$ est donc $\mathscr{F}(f)$.

Lorsque $f$ est la distribution tempérée associée à $g\in L^2(\mathbf{R}^n)$, on suit une marche tout analogue en utilisant la formule (29) de II, p. 221.

Un énoncé similaire vaut également pour la cotransformation de Fourier.

#### Remarque {#ts-iv-s3-n12-rem-1 .statement tag=031J}

Les formules élémentaires concernant la transformation de Fourier des mesures restent valides pour la transformation de Fourier des distributions tempérées. Par exemple, pour $f\in \mathscr{S}'(\mathbf{R}^n)$ et $\alpha \in \mathbf{N}^n$, on a

$$
\mathscr{F}(\partial^{\alpha}f) = (2i\pi )^{|\alpha|}X^{\alpha}\mathscr{F}(f)
$$

$$
\mathscr{F}(X^{\alpha}f) = (-2i\pi )^{-|\alpha|}\partial^{\alpha}(\mathscr{F}(f))
$$

d’après le lemme 11.

### 13. Distributions et distributions tempérées sur un espace vectoriel

Soit $u$ une application linéaire bijective de $\mathbf{R}^n$ dans $\mathbf{R}^n$. L’application $\varphi \mapsto \varphi \circ u$ est un automorphisme de $\mathscr{S}(\mathbf{R}^n)$ (resp. de $\mathscr{D}(\mathbf{R}^n))$; sa transposée est un automorphisme de $\mathscr{S}'(\mathbf{R}^n)$ (resp. de $\mathscr{D}'(\mathbf{R}^n))$.

Soit E un espace vectoriel réel de dimension finie $n$. Soit $v:\mathbf{R}^n\rightarrow E$ un isomorphisme d’espaces vectoriels. On note $\mathscr{S}(E)$ (resp. $\mathscr{D}(E))$ l’ensemble des applications $\varphi : E\rightarrow \mathbf{C}$ telles que $\varphi \circ v\in \mathscr{S}(\mathbf{R}^n)$ (resp. telles que $\varphi \circ v\in \mathscr{D}(\mathbf{R}^n))$. D’après la remarque précédente, cet espace ne dépend pas du choix de $v$; il est isomorphe à $\mathscr{S}(\mathbf{R}^n)$ (resp. $\mathscr{D}(\mathbf{R}^n))$. On note $\mathscr{S}'(E)$ (resp. $\mathscr{D}'(E))$ le dual de $\mathscr{S}(E)$ (resp. de $\mathscr{D}(E))$ muni de la topologie de la convergence bornée. C’est un espace vectoriel topologique isomorphe à $\mathscr{S}'(\mathbf{R}^n)$ (resp. à $\mathscr{D}'(\mathbf{R}^n))$.

Soient E et F des espaces vectoriels réels de dimension $n$, en dualité relativement à une forme bilinéaire $b: E\times F\rightarrow \mathbf{R}$. Le groupe localement compact commutatif E est en dualité avec F relativement à l’application

$(x, y)\mapsto$ exp(2$i\pi b(x, y))$

de $E\times F$ dans $\mathbf{U}($cf. cor. 1 de II, p. 235). On munit E et F de mesures de Haar qui sont duales l’une de l’autre relativement à cette application.

L’espace $\mathscr{S}(E)$ est inclus dans $L^1(E)$; la transformation de Fourier de E induit, par passage aux sous-espaces et par dualité, un isomorphisme d’espaces vectoriels topologiques de $\mathscr{S}(E)$ dans $\mathscr{S}$ (F), dont la transposée est un isomorphisme d’espaces vectoriels topologiques de $\mathscr{S}'(F)$ dans $\mathscr{S}'(E)$.

### 14. Espaces de Sobolev

Soit U un ouvert de $\mathbf{R}^n$. Soient $p$ un nombre réel $\geqslant 1$ et $k$ un entier naturel. On note $W^{k,p}(U)$ l’espace des distributions $f\in \mathscr{D}'(U)$ telles que, pour tout $\alpha \in \mathbf{N}^n$ avec $|\alpha |\leqslant k$, la distribution $\partial^{\alpha}f$ est associée à un élément de $L^p(U)$.

En particulier, pour $U =\mathbf{R}^n$, les éléments de $W^{k,p}(U)$ sont des distributions tempérées. L’application de $W^{k,p}(u)$ dans $\mathbf{R}_+$ qui à $f\in W^{k,p}(U)$ associe

$1/p$

$$
\|f\|_{k,p}=(\sum_{|\alpha|\leqslant k}\|\partial^{\alpha}f\|^p_p
$$

est une norme sur $W^{k,p}(U)$. L’espace $W^{k,p}(U)$ sera toujours muni de cette norme ; cet espace normé est appelé espace de Sobolev d’indice $k$ et d’exposant $p$.

L’espace $\mathscr{D}(U)$ est contenu dans $W^{k,p}(U)$. On note $W^{k,p}_0$ (U) l’adhérence de $\mathscr{D}(U)$ dans $W^{k,p}(U)$. C’est un sous-espace fermé de $W^{k,p}(U)$.

On a $W^{k,p}_0(\mathbf{R}^n) = W^{k,p}(\mathbf{R}^n)$, mais les espaces $W^{k,p}(U)$ et $W^{k,p}_0$ (U) sont distincts en général (cf. exercices 12 de IV, p. 334 et 14 de IV, p. 334).

On note aussi $H^k(U) = W^{k,2}(U)$ et $H^k_0(U) = W^{k,2}_0(U)$.

La norme de $H^k(U)$ est une norme préhilbertienne, associée à la forme hermitienne positive sur $H^k(U)$ définie par

$$
(f_1, f_2)\mapsto \sum_{|\alpha|\leqslant}\int_{kU}\partial^{\alpha}f_1\partial^{\alpha}f_2d\mu
$$

L’espace hilbertien $H^k(U)$ coïncide avec l’espace noté $\mathscr{H}^k$ dans EVT, V, p. 6, exemple (3).

On a $W^{0,p}(U) = L^p(U)$ et $H^0(U) = L^2(U)$ par définition ; de plus $W^0_0^{,p}(U) = L^p(U)$ d’après la prop. 4, b) de IV, p. 202.

#### Proposition 20 {#ts-iv-s3-prop-20 .statement tag=031K}

Les espaces de Sobolev $W^{k,p}(U)$ et $W^{k,p}_0$ (U) sont des espaces de Banach de type dénombrable. En particulier, les espaces $H^k(U)$ et $H^k_0(U)$ sont des espaces hilbertiens de type dénombrable.

Il suffit de démontrer les assertions concernant $W^{k,p}(U)$.

Soit I l’ensemble des $\alpha \in \mathbf{N}^n$ tels que $|\alpha |\leqslant k$. L’application linéaire $u$ de $W^{k,p}(U)$ dans $L^p(U)^I$ qui associe à $f$ la famille $(\partial^{\alpha}f)_{\alpha\in I}$ est injective ; elle est continue et stricte par définition de la norme sur $W^{k,p}(U)$. Pour démontrer que $W^{k,p}(U)$ est complet, il suffit de démontrer que son image par $u$ est fermée. Or, soit $(f_n)_{n\in\mathbf{N}}$ une suite dans $W^{k,p}(U)$ telle que $(u(f_n))_{n\in\mathbf{N}}$ converge. Soit $(g_{\alpha})_{\alpha\in I}\in L^p(U)^I$ sa limite. Pour $\alpha \in I$, la suite $(\partial^{\alpha}f_n)_{n\in\mathbf{N}}$ converge dans $L^p(U)$ vers $g_{\alpha}$. A fortiori, la convergence a lieu dans $\mathscr{D}'(U)$. Posons $f=g_0$. Pour tout $\varphi \in \mathscr{D}$(U), il vient

$$
\langle \partial^{\alpha}f, \varphi \rangle = (-1)^{|\alpha|}\langle f, \partial^{\alpha}\varphi \rangle
$$

$=_{n\rightarrow}$lim$_{+\infty}(-1)^{|\alpha|}\langle f_n, \partial^{\alpha}\varphi \rangle =_{n\rightarrow}$lim$_{+\infty}\langle \partial^{\alpha}f_n, \varphi \rangle =\langle g_{\alpha}, \varphi \rangle$.

Cela démontre que $g_{\alpha}=\partial^{\alpha}f$ pour tout $\alpha \in I$, donc $(g_{\alpha})_{\alpha\in I}=u(f)$ appartient à l’image de $u$.

L’espace $W^{k,p}(U)$ s’identifie par $u$ à un sous-espace de l’espace $L^p(U)^I$; celui-ci est de type dénombrable (prop. 2 de IV, p. 180 et TG, IX, p. 19, cor., (ii))), donc il en est de même de $W^{k,p}(U) ($loc. cit., (i)).

#### Proposition 21 {#ts-iv-s3-prop-21 .statement tag=031L}

Soit N la norme euclidienne sur $\mathbf{R}^n$. Soit $k$ un entier $\geqslant 0$. L’espace de Sobolev $H^k(\mathbf{R}^n)$ est l’espace des $f\in \mathscr{S}'(\mathbf{R}^n)$ tel que $(1 + N^k)\mathscr{F}(f)$ appartient à $L^2(\mathbf{R}^n)$.

On procède par récurrence sur $k$. Lorsque $k= 0$, le résultat est une conséquence du théorème de Plancherel (II, p. 215, th. 1). Supposons que $k= 1$. Pour $f\in \mathscr{S}'(\mathbf{R}^n)$, on a $(1 + N)\mathscr{F}f\in L^2(\mathbf{R}^n)$ si et seulement si $f\in L^2(\mathbf{R}^n)$ et $N\mathscr{F}f\in L^2(\mathbf{R}^n)$. De plus, $N\mathscr{F}\in L^2(\mathbf{R}^n)$ si et seulement si, pour tout $\alpha \in \mathbf{N}^n$ tel que $|\alpha |= 1$, on a $X^{\alpha}\mathscr{F}f\in L^2(\mathbf{R}^n)$. Comme on a $\mathscr{F}(\partial^{\alpha}f) = 2i\pi X^{\alpha}\mathscr{F}f$, cette condition signifie que $\mathscr{F}(\partial^{\alpha}f)\in L^2(\mathbf{R}^n)$ pour tout $\alpha$ avec $|\alpha |= 1$, c’est-à-dire $\partial^{\alpha}f\in L^2(\mathbf{R}^n)$ pour tout $\alpha$ avec $|\alpha |= 1$. Il en résulte que l’assertion est vraie pour $k= 1$.

Supposons maintenant que $k\geqslant$ 2 et que l’assertion concernant $H^{\ell}(\mathbf{R}^n)$ est valide pour tout entier positif $\ell \leqslant k-1$. Soit $f\in \mathscr{S}'(\mathbf{R}^n)$. Par définition, on a $f\in H^k(\mathbf{R}^n)$ si et seulement si $f\in L^2(\mathbf{R}^n)$ et, pour tout $\beta \in \mathbf{N}^n$ tel que $|\beta |\leqslant 1$, la distribution $\partial^{\beta}f$ appartient à $H^{k-1}(\mathbf{R}^n)$. Cela équivaut, d’après l’hypothèse de récurrence, à $f\in L^2(\mathbf{R}^n)$ et $(1 + N^{k-1})\mathscr{F}(\partial^{\beta}f)\in L^2(\mathbf{R}^n)$ pour tout $\beta \in \mathbf{N}^n$ tel que $|\beta |\leqslant 1$. Comme $\mathscr{F}(\partial^{\beta}f) = (2i\pi X)^{|\beta|}\mathscr{F}(f)$, la condition $f\in H^k(\mathbf{R}^n)$ équivaut à dire que $\mathscr{F}f\in L^2(\mathbf{R}^n)$ et $(1 + N^{k-1})X^{\beta}\mathscr{F}f\in L^2(\mathbf{R}^n)$ pour $\beta \in \mathbf{N}^n$ tel que $|\beta |\leqslant 1$.

Les inégalités

$$
1 + N^k\leqslant 1 + N^{k-1}\sum_{\beta|\beta\in|\mathbf{N}\leqslant 1^n}|X^{\beta}|\leqslant 1 +n^{1/2}N^k\leqslant (1 +n^{1/2})(1 + N^k)
$$

impliquent alors que $f\in H^k(\mathbf{R}^n)$ si et seulement si $(1+N^k)\mathscr{F}\in L^2(\mathbf{R}^n)$.

## EXERCICES {#ts-iv-s3-exercises}

See the [exercises for § 3](exercises/s3/).

[^1]: Notons que c’est par erreur que l’énoncé de cette proposition inclut le cas $p= +\infty$.
