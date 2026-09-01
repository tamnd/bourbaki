---
book: top
book_title: General Topology
chapter: X
chapter_title: ESPACES FONCTIONNELS
section: 3
section_title: Espaces fonctionnels spéciaux
lang: fr
source: top-v-x-fr
book_pages: TG X.47-TG X.54
pdf_pages: 0268-0282, 0296-0303
extraction: ocr
subsections:
    - "no": 1
      title: Espaces d’applications dans un espace métrique
      page: 19
      pdf_page: 268
    - "no": 2
      title: Espaces d’applications dans un espace normé
      page: 21
      pdf_page: 270
    - "no": 3
      title: Propriétés de dénombrabilité des espaces de fonctions continues
      page: 24
      pdf_page: 273
    - "no": 4
      title: La topologie de la convergence compacte
      page: 25
      pdf_page: 274
    - "no": 5
      title: Topologies sur les groupes d’homéomorphismes
      page: 30
      pdf_page: 279
statements: 31
exercises: 16
content_sha256: f40b7900a3993ebb8d5376787a3b8a3c62cd01cc1494c9254ba4e11c97479b67
---

## § 3. ESPACES FONCTIONNELS SPÉCIAUX

### 1. Espaces d’applications dans un espace métrique

Soient $X$ un ensemble, $Y$ un espace uniforme, $(f_i)_{i \in I}$ une famille d’écarts définissant la structure uniforme de $Y$ (IX, p. 5), $\mathcal{S}$ un ensemble de parties de $X$. Pour tout $i \in I$ et tout ensemble $A \in \mathcal{S}$, posons, pour tout couple $(u, v)$ d’applications de $X$ dans $Y$,

$$
g_{i,A}(u, v) = \sup_{x \in A} f_i(u(x), v(x));
$$

il est immédiat que $g_{i,A}$ est un écart sur $\mathcal{F}(X; Y)$ et que, lorsque $i$ parcourt $I$ et $A$ parcourt $\mathcal{S}$, la famille d’écarts $(g_{i,A})$ définit la structure uniforme de la $\mathcal{S}$-convergence sur $\mathcal{F}(X; Y)$. En particulier:

#### Proposition 1 {#top-x-s3-prop-1 .statement}

Si $Y$ est un espace uniforme métrisable, la structure uniforme de la convergence uniforme sur $\mathcal{F}(X; Y)$ est métrisable.

En effet, si $d$ est une distance sur $Y$ compatible avec la structure uniforme de cet espace, la structure de la convergence uniforme sur $\mathcal{F}(X; Y)$ est définie par l’unique écart

$$
\delta(u, v) = \sup_{x \in X} d(u(x), v(x));
$$

en général cet écart n’est pas fini, mais il est équivalent à un écart fini (IX, p. 3), et comme la structure uniforme de la convergence uniforme est séparé (X, p. 3, prop. 1), elle est métrisable.

#### Corollaire {#top-x-s3-n1-cor-1 .statement}

Soient $X$ un espace topologique, $Y$ un espace uniforme métrisable; on suppose qu’il existe une suite $(K_n)$ de parties compactes de $X$ telle que toute partie compacte de $X$ soit contenue dans l’un des $K_n$. Alors, sur $\mathcal{F}(X; Y)$, la structure uniforme de la convergence compacte est métrisable.

En effet, comme les $K_n$ forment un recouvrement de $X$, $\mathcal{F}_c(X; Y)$ est isomorphe à un sous-espace uniforme de $\prod_n \mathcal{F}_u(K_n; Y)$ (X, p. 3, Remarque 3) et le corollaire résulte donc de la prop. 1 (IX, p. 15, cor. 2).

On notera que ce corollaire s’applique en particulier lorsque $X$ est un espace localement compact dénombrable à l’infini (I, p. 68, cor. 1).

Soit maintenant $Y$ un espace métrique, et soit $d$ sa distance. Étant donnés un ensemble $X$ et un ensemble $\mathcal{S}$ de parties de $X$, nous désignerons par $\mathcal{B}_{\mathcal{S}}(X; Y)$ l’ensemble des applications $u : X \to Y$ telles que $u(A)$ soit borné pour tout $A \in \mathcal{S}$; sauf mention du contraire, nous munirons $\mathcal{B}_{\mathcal{S}}(X; Y)$ de la structure uniforme de la $\mathcal{S}$-convergence; cette dernière est définie par la famille d’écarts sur $\mathcal{B}_{\mathcal{S}}(X; Y)$:

$$
d_A(u, v) = \sup_{x \in A} d(u(x), v(x)) \qquad (A \in \mathcal{S})
$$

qui sont finis par hypothèse. Lorsque $\mathcal{S} = \{X\}$, on écrit $\mathcal{B}(X; Y)$ au lieu de $\mathcal{B}_{\mathcal{S}}(X; Y)$; on dit qu’une application $u : X \to Y$ est bornée si elle appartient à $\mathcal{B}(X; Y)$, autrement dit si $u(X)$ est une partie bornée de $Y$.

#### Proposition 2 {#top-x-s3-prop-2 .statement}

Soient $X$ un ensemble, $Y$ un espace métrique. Dans l’espace $\mathcal{F}_u(X; Y)$, l’ensemble $\mathcal{B}(X; Y)$ des applications bornées est à la fois ouvert et fermé.

En effet, si $u$ est bornée, toute application $v : X \to Y$ telle que $d(u(x), v(x)) \leq 1$ pour tout $x \in X$ est bornée, puisque

$$
d(v(x), v(x_0)) \leq d(u(x), u(x_0)) + 2;
$$

donc $\mathcal{B}(X; Y)$ est ouvert. D’autre part, si $u$ est adhérent à $\mathcal{B}(X; Y)$ dans $\mathcal{F}_u(X; Y)$, il existe une application $u_0 \in \mathcal{B}(X; Y)$ telle que $d(u(x), u_0(x)) \leq 1$ pour tout $x \in X$; donc $u$ est bornée.

#### Corollaire 1 {#top-x-s3-prop-2-cor-1 .statement}

Soient $X$ un ensemble, $Y$ un espace métrique, $\mathfrak{S}$ un ensemble de parties de $X$. Alors l’ensemble $\mathcal{B}_{\mathfrak{S}}(X; Y)$ des applications de $X$ dans $Y$ transformant tout $A \in \mathfrak{S}$ en une partie bornée de $Y$ est fermé dans $\mathcal{F}_{\mathfrak{S}}(X; Y)$. En particulier, si $Y$ est complet, $\mathcal{B}_{\mathfrak{S}}(X; Y)$ est complet pour la structure uniforme de la $\mathfrak{S}$-convergence.

En effet, $\mathcal{B}_{\mathfrak{S}}(X; Y)$ est l’image réciproque de la partie $\prod_{A \in \mathfrak{S}} \mathcal{B}(A; Y)$ du produit $\prod_{A \in \mathfrak{S}} \mathcal{F}_u(A; Y)$ par l’application canonique de $\mathcal{F}_{\mathfrak{S}}(X; Y)$ dans $\prod_{A \in \mathfrak{S}} \mathcal{F}_u(X; Y)$; la première assertion résulte donc de la Remarque 3 de X, p. 3. La seconde s’en déduit, compte tenu de X, p. 7, th. 1.

#### Corollaire 2 {#top-x-s3-prop-2-cor-2 .statement}

Soient $X$ un espace topologique, $Y$ un espace métrique. Alors l’espace des applications continues bornées de $X$ dans $Y$ est à fois ouvert et fermé dans l’espace $\mathcal{C}_u(X; Y)$; il est complet si en outre $Y$ est complet.

L’espace en question est en effet l’intersection

$$
\mathcal{B}(X; Y) \cap \mathcal{C}_u(X; Y);
$$

la première assertion résulte de la prop. 2, et la seconde s’en déduit, compte tenu de X, p. 9, cor. 1.

### 2. Espaces d’applications dans un espace normé

Considérons plus particulièrement le cas où $Y$ est un espace vectoriel normé sur un corps valué non discret $K$ (IX, p. 32), $\|y\|$ désignant la norme d’un élément $y \in Y$; l’ensemble $\mathcal{F}(X; Y) = Y^X$ est alors muni canoniquement d’une structure d’espace vectoriel sur $K$. Pour qu’une application $u : X \to Y$ soit bornée, il faut et il suffit que la fonction numérique $x \mapsto \|u(x)\|$ soit bornée dans $X$; si $u, v$ sont deux applications bornées de $X$ dans $Y$, il est clair que $u + v$ et $\lambda u$ ($\lambda \in K$) sont encore bornées; autrement dit, $\mathcal{B}(X; Y)$ est un sous-espace vectoriel de $\mathcal{F}(X; Y)$. En outre, $\|u\| = \sup_{x \in X} \|u(x)\|$ est une norme sur $\mathcal{B}(X; Y)$, car cette fonction satisfait à l’inégalité du triangle et $\|u\| = 0$ entraîne $u = 0$; enfin, on a, pour tout $\lambda \in K$,
$$
\|\lambda u\| = \sup_{x \in X} \|\lambda u(x)\| = \sup_{x \in X} |\lambda| \cdot \|u(x)\| = |\lambda| \cdot \sup_{x \in X} \|u(x)\| = |\lambda| \cdot \|u\|,
$$
notre assertion. Il est immédiat que la structure uniforme sur $\mathcal{B}(X; Y)$ définie par cette norme est la structure de la convergence uniforme. Sauf mention expresse du contraire, lorsque $\mathcal{B}(X; Y)$ sera considéré comme un espace normé, il s’agira toujours de la norme précédente.

#### Proposition 3 {#top-x-s3-prop-3 .statement}

Si l’espace normé $Y$ est complet, toute série $(u_n)$ d’applications bornées de $X$ dans $Y$, qui est absolument convergente dans l’espace normé $\mathcal{B}(X; Y)$ (c’est-à-dire telle que $\sum_{n=0}^{\infty} \|u_n\| < + \infty$; cf. IX, p. 36 et 37) est uniformément convergente dans $X$.

En effet, comme $\mathcal{B}(X; Y)$ est complet ($X$, p. 21, cor. 1), cela résulte de IX, p. 36, prop. 12 et de la définition d’une série uniformément convergente.

#### Remarque 1 {#top-x-s3-n2-rem-1 .statement}

Si $\sum_{n=0}^{\infty} \|u_n\| < +\infty$, on a pour tout $x \in X$,
$$
\sum_{n=0}^{\infty} \|u_n(x)\| \leq \sum_{n=0}^{\infty} \|u_n\| < +\infty;
$$
autrement dit, chacune des séries de terme général $u_n(x)$ ($x \in X$) est absolument convergente dans l’espace $Y$; la réciproque est inexacte. Pour éviter toute confusion, on exprime parfois que la série de terme général $\|u_n\|$ est convergente, en disant que la série de terme général $u_n$ est normalement convergente. Une série peut être uniformément convergente dans $X$ sans être normalement convergente; il en est ainsi, par exemple, de la série $(u_n)$ dans l’espace $\mathcal{B}(\mathbf{R}; \mathbf{R})$ définie de la façon suivante: $u_n(x) = (1/n) \sin x$ dans l’intervalle $[n\pi, (n+1)\pi]$, $u_n(x) = 0$ en dehors de cet intervalle.

Lorsque $Y$ est une algèbre normée (IX, p. 37) sur un corps valué commutatif non discret $K$, $\mathcal{B}(X; Y)$ est une algèbre sur $K$; en outre, la norme $\|u\|$ est alors compatible avec cette structure d’algèbre, car on a
$$
\|uv\| = \sup_{x \in X} |u(x)v(x)| \leq \sup_{x \in X} \|u(x)\| \cdot \|v(x)\|
\leq \sup_{x \in X} \|u(x)\| \cdot \sup_{x \in X} \|v(x)\| = \|u\| \cdot \|v\|.
$$
Autrement dit, $\mathcal{B}(X; Y)$ est alors une algèbre normée sur le corps $K$.

#### Proposition 4 {#top-x-s3-prop-4 .statement}

*Soient* $X_i$ ($1 \leq i \leq n$) *et* $Y$ *des espaces vectoriels normés sur un corps valué non discret* $K$, *et soit* $X = \prod_{i=1}^{n} X_i$. *L’ensemble de toutes les applications multilinéaires de* $X$ *dans* $Y$ *est fermé dans l’espace* $\mathcal{F}_s(X; Y)$.

En effet cet ensemble est formé des $u \in \mathcal{F}(X; Y)$ vérifiant toutes les relations
$$
\begin{cases}
u(x_1, \ldots, x_i' + x_i'', \ldots, x_n) = u(x_1, \ldots, x_i', \ldots, x_n) + u(x_1, \ldots, x_i'', \ldots, x_n) \\
u(x_1, \ldots, \lambda x_i, \ldots, x_n) = \lambda u(x_1, \ldots, x_i, \ldots, x_n)
\end{cases}
$$
$(1 \leq i \leq n, x_i, x_i', x_i''$ arbitraires dans $X_i, \lambda$ arbitraire dans $K$); comme les deux membres des relations (1) sont fonctions continues de $u$ dans $\mathcal{F}_s(X; Y)$ ($X$, p. 4, *Remarque 6*), la proposition en résulte (I, p. 53, prop. 2).

#### Proposition 5 {#top-x-s3-prop-5 .statement}

*Sous les hypothèses de la prop.* 4, *l’ensemble* $\mathcal{L}(X_1, \ldots, X_n; Y)$ *des applications multilinéaires continues de* $X$ *dans* $Y$ *est fermé dans* $\mathcal{F}(X; Y)$ *muni de la topologie de la convergence bornée; il est complet pour la structure uniforme de la convergence bornée lorsque* $Y$ *est complet*.

En effet, si $\mathcal{S}$ est l’ensemble des parties bornées de $X$, $\mathcal{L}(X_1, \ldots, X_n; Y)$ est l’intersection de l’ensemble de toutes les applications multilinéaires de $X$ dans $Y$ et de l’ensemble $\mathcal{B}_{\mathcal{S}}(X; Y)$ (IX, p. 35, th. 1); la proposition résulte donc de la prop. 4 et de $X$, p. 21, cor 1.

Dans toute la fin de ce n°, nous supposerons que K désigne un corps valué non discret commutatif.

Alors $\mathcal{L}(X_1, \ldots, X_n; Y)$ est un sous-espace vectoriel de $\mathcal{F}(X; Y)$. Soit B la boule unité de X, ensemble des $(\mathbf{x}_i)_{1 \leq i \leq n}$ tels que $\sup_{1 \leq i \leq n} \| \mathbf{x}_i \| \leq 1$; l’application $u \mapsto u|B$ de $\mathcal{L}(X_1, \ldots, X_n; Y)$ dans $\mathcal{B}(B; Y)$ est injective; en outre l’image réciproque par cette application de la structure uniforme de la convergence uniforme sur $\mathcal{B}(B; Y)$ est la structure uniforme de la convergence bornée sur $\mathcal{L}(X_1, \ldots, X_n; Y)$. En effet, toute partie bornée de X est contenue dans un ensemble de la forme $\mu B$ (avec $\mu \in K^*$), et dire que, pour un élément $u \in \mathcal{L}(X_1, \ldots, X_n; Y)$, on a $\|u(\mathbf{z})\| \leq a$ pour tout $\mathbf{z} \in \mu B$, équivaut à dire que $\|u(\mathbf{z})\| \leq a/|\mu|^n$ pour tout $\mathbf{z} \in B$. On vérifie aussitôt que le nombre $\|u\| = \sup_{\mathbf{z} \neq 0} \|u(\mathbf{z})\|/\|\mathbf{z}\|$ est une norme sur $\mathcal{L}(X_1, \ldots, X_n; Y)$, définissant sur cet espace la structure uniforme de la convergence bornée, et l’on a évidemment

(2)
$$
\|u(x_1, \ldots, x_n)\| \leq \|u\| \cdot \|x_1\| \cdots \|x_n\|.
$$

Sauf mention expresse du contraire, lorsque $\mathcal{L}(X_1, \ldots, X_n; Y)$ sera considéré comme un espace normé, il s’agira toujours de la norme précédente. On peut encore dire que $\|u\|$ est le plus petit nombre $\geq 0$ vérifiant (2) pour toutes les valeurs des $x_i$.

#### Proposition 6 {#top-x-s3-prop-6 .statement}

*L’application multilinéaire*
$$
(u, x_1, \ldots, x_n) \to u(x_1, \ldots, x_n)
$$
*de l’espace normé $\mathcal{L}(X_1, \ldots, X_n; Y) \times X_1 \times \cdots \times X_n$ dans Y est continue.*

C’est une conséquence immédiate de l’inégalité (2) (IX, p. 35, th. 1).

#### Proposition 7 {#top-x-s3-prop-7 .statement}

*Soient X, Y, Z trois espaces normés sur K. L’application canonique de l’espace normé $\mathcal{L}(X, Y; Z)$ dans l’espace des applications linéaires de X dans $\mathcal{L}(Y; Z)$ qui, à tout $u \in \mathcal{L}(X, Y; Z)$, fait correspondre l’application $x \mapsto u(x, .)$, est une isométrie de $\mathcal{L}(X, Y; Z)$ sur $\mathcal{L}(X; \mathcal{L}(Y; Z))$.*

Cela résulte aussitôt des définitions et de la relation
$$
\sup_{\|x\| \leq b} (\sup_{\|y\| \leq c} \|u(x, y)\|) = \sup_{\|x\| \leq b, \|y\| \leq c} \|u(x, y)\|.
$$

#### Proposition 8 {#top-x-s3-prop-8 .statement}

*Soient X, Y, Z trois espaces normés sur K. L’application bilinéaire $(u, v) \mapsto v \circ u$ de $\mathcal{L}(X; Y) \times \mathcal{L}(Y; Z)$ dans $\mathcal{L}(X; Z)$ est continue.*

En effet, si $u \in \mathcal{L}(X; Y)$, $v \in \mathcal{L}(Y; Z)$, on a, de façon précise,
(3)
$$
\|v \circ u\| \leq \|u\| \cdot \|v\|
$$
car pour tout $x \in X$, $\|v(u(x))\| \leq \|v\| \cdot \|u(x)\| \leq \|v\| \cdot \|u\| \cdot \|x\|$ en vertu de (2).

En particulier, sur l’ensemble $\mathcal{L}(X)$ des *endomorphismes continus* d’un espace normé $X$ sur $K$, la norme $\|u\|$ est compatible avec la structure d’*algèbre* de $\mathcal{L}(X)$ sur $K$.

#### Remarque 2 {#top-x-s3-n2-rem-2 .statement}

L’ensemble $\mathcal{L}(\mathbf{R}^m; \mathbf{R}^n)$ des applications linéaires (nécessairement continues) de $\mathbf{R}^m$ dans $\mathbf{R}^n$ peut être identifié à l’ensemble $M_{n,m}(\mathbf{R})$ des matrices à $n$ lignes et $m$ colonnes sur $\mathbf{R}$, donc à $\mathbf{R}^{mn}$; sur $\mathcal{L}(\mathbf{R}^m; \mathbf{R}^n)$, la structure uniforme de la convergence bornée (pour la distance euclidienne sur $\mathbf{R}^m$), de la convergence compacte et de la convergence simple sont alors identifiées à la structure uniforme *additive* de $\mathbf{R}^{mn}$. En effet, prenons sur $\mathbf{R}^n$ la norme $\|x\| = \sup_i |x_i|$ pour $x = (x_i)$ et soit $(\mathbf{e}_j)$ la base canonique de $\mathbf{R}^m$; si $u$ et $v$ sont deux applications linéaires de $\mathbf{R}^m$ dans $\mathbf{R}^n$ telles que $\|u(\mathbf{e}_j) - v(\mathbf{e}_j)\| \leq \varepsilon$ pour $1 \leq j \leq m$, on a, pour les matrices $U = (\alpha_{ij})$, $V = (\beta_{ij})$ de ces applications, $|\alpha_{ij} - \beta_{ij}| \leq \varepsilon$ pour tout couple $(i, j)$; et inversement, si ces inégalités sont satisfaites, on a, pour tout point $x$ d’un cube de centre 0 et de côté $a$ dans $\mathbf{R}^m$, $\|u(x) - v(x)\| \leq ma\varepsilon$.

### 3. Propriétés de dénombrabilité des espaces de fonctions continues

#### Théorème 1 {#top-x-s3-thm-1 .statement}

*Soit $X$ un espace compact.*

a) *Si $X$ est métrisable, alors, pour tout espace uniforme métrisable $Y$ de type dénombrable* (IX, p. 18), *l’espace métrisable $C_u(X; Y)$ des applications continues de $X$ dans $Y$, muni de la topologie de la convergence uniforme, est de type dénombrable*.

b) *Réciproquement, si l’espace métrisable $C_u(X; \mathbf{R})$ est de type dénombrable, $X$ est métrisable*.

a) Soit $d$ (resp. $d'$) une distance compatible avec la topologie de $X$ (resp. la structure uniforme de $Y$); on sait que $\delta(f, g) = \sup_{x \in X} d'(f(x), g(x))$ est une distance définissant la structure de la convergence uniforme sur $C(X; Y)$, les fonctions de $C(X; Y)$ étant bornées puisque $X$ est compact (X, p. 20). Pour tout couple d’entiers $m > 0, n > 0$, soit $G_{mn}$ l’ensemble des fonctions $f \in C(X; Y)$ telles que la relation $d(x, x') \leq 1/m$ entraîne $d'(f(x), f(x')) \leq 1/n$; toute fonction $f \in C(X; Y)$ est uniformément continue (II, p. 29, th. 2), donc, pour tout $n > 0$, $C(X; Y)$ est réunion des $G_{mn}$ ($m > 0$). Soit $\{a_1, \ldots, a_{p(m)}\}$ une partie finie de $X$ telle que les boules ouvertes de centre $a_i$ et de rayon $1/m$ forment un recouvrement de $X$ pour $1 \leq i \leq p(m)$; soit d’autre part $(b_r)_{r \in \mathbf{N}}$ une suite dénombrable dense dans $Y$. Pour toute application $\varphi$ de $\{1, p(m)\}$ dans $\mathbf{N}$, soit $H_\varphi$ l’ensemble des $f \in G_{mn}$ telles que $d'(f(a_k), b_{\varphi(k)}) \leq 1/n$ pour $1 \leq k \leq p(m)$. Par définition de $b_r$, $G_{mn}$ est réunion des $H_\varphi$ pour $\varphi \in \mathbf{N}^{p(m)}$; soit $C_{mn}$ l’ensemble des $\varphi \in \mathbf{N}^{p(m)}$ tels que $H_\varphi \neq \varnothing$, et pour chaque $\varphi \in C_{mn}$, soit $g_\varphi$ un élément de $H_\varphi$; enfin, désignons par $L_{mn}$ l’ensemble dénombrable des $g_\varphi$ pour $\varphi \in C_{mn}$. Soit $f \in G_{mn}$, et soit $\varphi$ un élément de $C_{mn}$ tel que $f \in H_\varphi$; il résulte aussitôt des définitions que l’on a $d'(f(x), g_\varphi(x)) \leq 4/n$ pour tout $x \in X$, autrement dit, $\delta(f, g_\varphi) \leq 4/n$. On en conclut que la réunion des $L_{mn}$ est partout dense dans $C_u(X; Y)$: en effet, pour tout entier $n > 0$ et tout $f \in C(X; Y)$, il existe $m$ tel que $f \in G_{mn}$, et on vient de voir que la distance de $f$ à $L_{mn}$ est $\leq 4/n$.

b) Soit $I = \{0, 1\}$; comme $\mathcal{C}_u(X; I)$ est un sous-espace uniforme de $\mathcal{C}_u(X; \mathbf{R})$, il est de type dénombrable; soit $(f_n)$ une suite partout dense dans cet espace. Considérons l’espace produit $K = I^\mathbf{N}$, et l’application $\psi : x \mapsto (f_n(x))$ de $X$ dans $K$ qui est évidemment continue. L’application $\psi$ est injective: en effet, par définition de la suite $(f_n)$, la relation $f_n(x) = f_n(x')$ pour tout $n$ entraîne, par passage à la limite, $f(x) = f(x')$ pour toute fonction $f \in \mathcal{C}(X; I)$; mais cela est impossible si $x \neq x'$, en vertu de l’axiome $(\mathrm{O}_{\mathrm{IV}})$ appliqué au point $x$ et à voisinage $V$ de $x$ ne contenant pas $x'$ (IX, p. 7, th. 2). On en conclut que l’espace compact $X$ est homéomorphe au sous-espace $\psi(X)$ de $K$ (I, p. 63, cor. 2); comme $K$ est métrisable et de type dénombrable, il en est de même de $\psi(X)$, donc de $X$.

C.Q.F.D.

#### Corollaire {#top-x-s3-n3-cor-1 .statement}

*Soient $X$ un espace localement compact dont la topologie admet une base dénombrable, $Y$ un espace uniforme métrisable de type dénombrable.*

*a) L’espace $\mathcal{L}$ des applications continues de $X$ dans $Y$, ayant une limite à l’infini, muni de la topologie de la convergence uniforme dans $X$, est un espace métrisable de type dénombrable.*

*b) L’espace $\mathcal{C}_c(X; Y)$ des applications continues de $X$ dans $Y$, muni de la topologie de la convergence compacte, est un espace métrisable de type dénombrable.*

*a) Soit $X'$ l’espace compact obtenu en adjoignant à $X$ un point à l’infini (I, p. 67, th. 4); par définition, toute fonction $f$ de $\mathcal{L}$ se prolonge de façon unique en une application continue $\tilde{f}$ de $X'$ dans $Y$, et $f \mapsto \tilde{f}$ est donc une bijection de $\mathcal{L}$ sur $\mathcal{C}(X'; Y)$; en outre cette bijection est un homéomorphisme de l’espace $\mathcal{L}$ sur $\mathcal{C}_u(X'; Y)$, en vertu de $X$, p. 7, prop. 6. Il suffit alors d’appliquer à $X'$ et $Y$ le th. 1, en observant que $X'$ est métrisable (IX, p. 21, corollaire).

*b) Soit $(U_n)$ un recouvrement de $X$ par des ensembles ouverts relativement compacts tel que toute partie compacte de $X$ soit contenue dans un $U_n$ (I, p. 68, cor. 1). Si $\mathfrak{S}$ est l’ensemble des $\overline{U}_n$, la topologie de la convergence compacte sur $\mathcal{C}(X; Y)$ est identique à la topologie de la $\mathfrak{S}$-convergence. Par suite (X, p. 3, Remarque 3) l’espace $\mathcal{C}_c(X; Y)$ est homéomorphe à un sous-espace du produit $\prod_n \mathcal{C}_u(\overline{U}_n; Y)$; comme chacun des espaces compacts $\overline{U}_n$ admet une base dénombrable, il est métrisable (IX, p. 21, prop. 16); chacun des $\mathcal{C}_u(\overline{U}_n; Y)$ est donc métrisable et de type dénombrable en vertu du th. 1 (X, p. 24) et par suite, il en est de même de $\mathcal{C}_c(X; Y)$.

On notera que l’espace des fonctions numériques continues bornées dans $\mathbf{R}$, muni de la topologie de la convergence uniforme, n’est pas de type dénombrable (X, p. 48, exerc. 4).

### 4. La topologie de la convergence compacte

#### Théorème 2 {#top-x-s3-thm-2 .statement}

*Soient $X$ un espace topologique, $Y$ un espace uniforme. Pour tout couple $(K, U)$ formé d’une partie compacte $K$ de $X$ et d’une partie ouverte $U$ de $Y$, soit $T(K, U)$* l’ensemble des applications continues $u : X \to Y$ telles que $u(K) \subset U$. Alors les ensembles de la forme $T(K, U)$ engendrent (I, p. 13) la topologie de la convergence compacte sur $C(X; Y)$.

Soient $Y'$ l’espace uniforme séparé associé à $Y$ (II, p. 24), $i : Y \to Y'$ l’application canonique de $Y$ sur $Y'$. La topologie de la convergence compacte est la topologie la moins fine rendant continues les applications $u \mapsto (i \circ u) \mid K$ de $C(X; Y)$ dans $C_u(K; Y')$, $K$ parcourant l’ensemble des parties compactes de $X$ (X, p. 5, prop. 4). On obtient donc un système générateur de la topologie de $C_c(X; Y)$ en prenant, pour chaque partie compacte $K$ de $X$, un système générateur de la topologie de $C_u(K; Y')$ et son image réciproque dans $C(X; Y)$, et en considérant la réunion dans $\mathcal{P}(C(X; Y))$ de tous les ensembles de parties ainsi obtenus.

D’autre part, toute partie ouverte de $Y$ est de la forme $i^{-1}(U')$, où $U'$ est ouvert dans $Y'$ (II, p. 23, prop. 12); donc, pour toute partie compacte $K' \supset K$, $T(K, i^{-1}(U'))$ est l’image réciproque de $T(K, U')$ par l’application $C(X; Y) \to C_u(K'; Y')$, et on est ainsi ramené à démontrer le théorème lorsque $X$ est *compact* et $Y$ *séparé*, ce que nous supposerons désormais.

Montrons d’abord que $T(K, U)$ est *ouvert* dans $C_c(X; Y)$. Soit $u_0$ un point de cet ensemble; comme $u_0(K)$ est compact (I, p. 63, cor. 1) et contenu dans l’ensemble ouvert $U$, il existe un entourage symétrique $V$ de $Y$ tel que $V(u_0(K)) \subset U$ (II, p. 31, corollaire). Soit $W$ le voisinage de $u_0$ dans $C_c(X; Y)$ formé des applications continues $u : X \to Y$ telles que $(u(x), u_0(x)) \in V$ pour tout $x \in K$. Pour ces applications, on a évidemment $u(K) \subset V(u_0(K)) \subset U$, donc $u \in T(K, U)$ et par suite $W \subset T(K, U)$, ce qui prouve notre assertion.

Inversement, si $W$ est un voisinage d’un point $u_0 \in C_0(X; Y)$, montrons que $W$ contient l’intersection d’un nombre fini de voisinages de $u_0$ de la forme $T(K, U)$. On peut supposer que $W$ est l’ensemble des $u \in C(X; Y)$ tels que $(u(x), u_0(x)) \in V$ pour tout $x \in X$, $V$ étant un entourage donné de $Y$. Comme $u_0$ est continue dans $X$, elle est uniformément continue (II, p. 29, th. 2); soit $V_1$ un entourage symétrique de $Y$, ouvert dans $Y \times Y$, tel que $\overline{V}_1 \subset V$. Il existe un recouvrement de $X$ par un nombre fini d’ensembles compacts $K_i$ ($1 \leq i \leq n$) tels que $u_0(K_i)$ soit petit d’ordre $V_1$ pour $1 \leq i \leq n$. Soit $U_i$ l’ensemble ouvert $V_1(u_0(K_i))$, et soit $u$ une application continue de $X$ dans $Y$ appartenant à l’intersection des $n$ ensembles $T(K_i, U_i)$ (qui sont des voisinages de $u_0$). Alors, pour tout $x \in K_i$, $u(x)$ appartient à $U_i$, donc $u_0(x)$ et $u(x)$ sont voisins d’ordre $\overline{V}_1$, donc voisins d’ordre $V$. Puisque tout $x \in X$ appartient à un des $K_i$ au moins, on a bien $u \in W$, ce qui achève la démonstration.

Ce résultat conduit à poser la définition suivante:

#### Définition 1 {#top-x-s3-def-1 .statement}

*Soient* $X, Y$ *deux espaces topologiques* (non nécessairement uniformisables). *Pour tout couple* $(K, U)$ *formé d’une partie compacte* $K$ *de* $X$ *et d’une partie ouverte*

U de Y, soit $T(K, U)$ l’ensemble des $u \in C(X; Y)$ telles que $u(K) \subset U$. On appelle topologie de la convergence compacte sur $C(X; Y)$ la topologie engendrée par l’ensemble des parties de la forme $T(K, U)$; on désigne par $C_c(X; Y)$ l’espace topologique obtenu en munissant $C(X; Y)$ de cette topologie.

Lorsque Y est un espace uniforme, il résulte du th. 2 (X, p. 25) que cette définition coïncide avec celle qui a été donnée dans X, p. 4.

Si H est une partie de $C(X; Y)$, nous dirons encore que la topologie induite sur H par celle de $C_c(X; Y)$ est la topologie de la convergence compacte.

#### Exemple {#top-x-s3-n4-exa-1 .statement}

Soit I l’intervalle $[0, 1]$ dans $\mathbf{R}$; pour tout espace topologique Y, l’espace $C_c(I; Y)$ est appelé l’espace des chemins dans Y; pour tout $y \in Y$, le sous-espace $\Omega_y(Y)$ de $C_c(I; Y)$ formé des chemins $u$ tels que $u(0) = u(1) = y$ est appelé l’espace des lacets (dans H) au point y.

#### Remarque 1 {#top-x-s3-n4-rem-1 .statement}

On dit de même que la topologie induite sur $C(X; Y)$ par la topologie produit sur $Y^X = F(X; Y)$ est la topologie de la convergence simple (Y n’étant pas nécessairement uniformisable); elle est engendrée par les ensembles de la forme $T(\{x\}, U)$ pour $x \in X$, U ouvert dans Y et est par suite moins fine que la topologie de la convergence compacte. On en déduit que si Y est séparé, l’espace $C_c(X; Y)$ est séparé (I, p. 54, corollaire).

#### Remarque 2 {#top-x-s3-n4-rem-2 .statement}

Soient $\mathfrak{S}$ un système générateur de la topologie de Y, $\mathfrak{R}$ un ensemble de parties compactes de X ayant la propriété suivante:
(R) Pour toute partie compacte L de X et tout voisinage V de L, il existe un nombre fini d’ensembles $K_i \in \mathfrak{R}$ tels que $L \subset \bigcup_i K_i \subset V$.

Alors les ensembles $T(K, U)$ où $K \in \mathfrak{R}$ et $U \in \mathfrak{S}$ forment un système générateur de la topologie de la convergence compacte sur $C(X; Y)$. En effet, il faut prouver que pour toute partie compacte L de X, toute partie ouverte V de Y, et tout $u \in T(L, V)$, il existe un nombre fini de couples $(K_i, U_i)$ tels que $K_i \in \mathfrak{R}$, $U_i \in \mathfrak{S}$ et $u \in \bigcap_i T(K_i, U_i) \subset T(L, V)$. Notons d’abord que pour toute suite finie $(S_k)$ d’ensembles de $\mathfrak{S}$ et toute partie compacte M de X, on a

$$
T(M, \bigcap_k S_k) = \bigcap_k T(M, S_k)
$$

par définition. On peut donc remplacer tout d’abord $\mathfrak{S}$ par l’ensemble des intersections finies d’ensembles de $\mathfrak{S}$, autrement dit supposer que $\mathfrak{S}$ est une base de la topologie de Y. Par hypothèse, $u(L)$ est quasi-compact et contenu dans V, donc il existe un nombre fini d’ensembles $U_i \in \mathfrak{S}$ contenus dans V et formant un recouvrement de $u(L)$. Les ensembles $u^{-1}(U_i)$ sont ouverts dans X et forment un recouvrement de L. Pour tout $x \in L$, il y a donc un voisinage compact $N_x$ de $x$ dans L, contenu dans un des $u^{-1}(U_i)$; on peut recouvrir L par un nombre fini de ces ensembles $N_{x_j} = L_j$; pour tout j, nous désignerons par $i(j)$ un des indices i tels que $L_j \subset u^{-1}(U_t)$. Cela étant, pour chaque indice $j$, il existe d’après (R) un nombre fini d’ensembles $K_{j,k} \subset u^{-1}(U_{t(j)})$ appartenant à $\mathcal{K}$ et formant un recouvrement de $L_j$. Pour tout $v \in \bigcap_{j,k} T(K_{j,k}, U_{t(j)})$, on a $\bigcup_k v(K_{j,k}) \subset U_{t(j)}$, donc $v(L_j) \subset U_{t(j)}$, et $v(L) = \bigcup_j v(L_j) \subset \bigcup_j U_{t(j)} \subset V$, ce qui achève de prouver notre assertion.

#### Théorème 3 {#top-x-s3-thm-3 .statement}

*Soient X, Y, Z trois espaces topologiques, f une application de $X \times Y$ dans Z. Si f est continue, $\tilde{f}: x \mapsto f(x,.)$ est une application continue de X dans $\mathcal{C}_c(Y; Z)$. La réciproque est vraie si Y est localement compact.*

Supposons $f$ continue et montrons que $\tilde{f}$ l’est : il faut prouver que pour toute partie compacte K de Y et toute partie ouverte U de Z, l’image réciproque V de $T(K, U)$ par $\tilde{f}$ est ouverte dans X. Soit donc $x_0 \in V$. Pour tout $y \in K$, on a $f(x_0, y) \in U$ et, comme $f$ est continue, il y a un voisinage $V_y$ de $x_0$ dans X et un voisinage $W_y$ de $y$ dans Y tels que $f(V_y \times W_y) \subset U$. Comme K est compact, il existe un nombre fini de points $y_i \in K$ tels que les ensembles $W_{y_i}$ recouvrent K ($1 \leq i \leq n$). Soit $V'$ l’intersection des voisinages $V_{y_i}$ de $x_0$, qui est un voisinage de $x_0$; pour $x \in V', y \in K$, on a $f(x, y) \in U$ puisque $y$ est contenu dans l’un des $W_{y_i}$ et que $x \in V_{y_i}$ pour tout $i$; on a donc bien $V' \subset V$, et comme V est un voisinage de chacun de ses points, il est ouvert dans X.

Réciproquement, supposons $\tilde{f}$ continue et Y localement compact, et montrons que $f$ est continue. Soient $x_0 \in X, y_0 \in Y, U$ un voisinage ouvert de $f(x_0, y_0)$ dans Z ; prouvons qu’il existe un voisinage V de $x_0$ dans X et un voisinage W de $y_0$ dans Y tels que $f(V \times W) \subset U$. Comme $y \mapsto f(x_0, y)$ est continue, il existe un voisinage *compact* W de $y_0$ tel que $f(\{x_0\} \times W) \subset U$. D’autre part, puisque $\tilde{f}$ est continue, l’ensemble V des $x \in X$ tels que $f(x,.) \in T(W, U)$ (c’est-à-dire tels que $f(x, y) \in U$ pour tout $y \in W$) est une partie ouverte de X, donc un voisinage de $x_0$. On a bien alors $f(V \times W) \subset U$.

C.Q.F.D.

#### Corollaire 1 {#top-x-s3-thm-3-cor-1 .statement}

*Soient X un espace localement compact, Y un espace topologique, H une partie de $\mathcal{C}(X; Y)$. Alors, sur H, la topologie de la convergence compacte est la moins fine pour laquelle l’application $(u, x) \mapsto u(x)$ de $H \times X$ dans Y est continue.*

En effet, en vertu du th. 3, dire que cette application est continue signifie que l’injection canonique $H \to \mathcal{C}_c(X; Y)$ est continue.

#### Remarque 3 {#top-x-s3-n4-rem-3 .statement}

Soient X un espace localement compact, Y un espace topologique séparé. Si $\mathcal{T}$ est une topologie sur une partie H de $\mathcal{C}(X; Y)$ telle que l’application $(u, x) \mapsto u(x)$ soit continue dans $H \times X$ et si en outre H est *compact* pour cette topologie, alors $\mathcal{T}$ est identique à la topologie de la convergence compacte : elle est en effet plus fine que cette dernière en vertu du cor. 1, et comme la topologie de la convergence compacte est séparée, ces deux topologies sont identiques. On notera que si en outre Y est *complètement régulier*, H est *équicontinu* pour toute structure uniforme compatible avec la topologie de Y (X, p. 19, cor. 3), et pour toute partie compacte K de X, l’ensemble $H(K) = \bigcup_{x \in K} H(x)$ est *compact*, étant l’image de $H \times K$ par l’application continue $(u, x) \mapsto u(x)$.

#### Corollaire 2 {#top-x-s3-thm-3-cor-2 .statement}

*Soient X, Y, Z trois espaces topologiques, X étant supposé séparé et Y localement compact. Alors, la restriction à $C(X \times Y; Z)$ de la bijection canonique $F(X \times Y; Z) \to F(X; F(Y; Z))$ (E, II, p. 31) est un homéomorphisme de $C_c(X \times Y; Z)$ sur $C_c(X; C_c(Y; Z))$.

Cette restriction est bien une bijection

$$
\rho : C(X \times Y; Z) \to C(X; C_c(Y; Z))
$$

en vertu du th. 3 (X, p. 28); reste à voir que la topologie de la convergence compacte sur $C(X \times Y; Z)$ est bien l’image réciproque par $\rho$ de la topologie de la convergence compacte sur $C(X; C_c(Y; Z))$. Comme un système générateur de la topologie de $C_c(Y; Z)$ est formé par les $T(K, U)$, où K est une partie compacte de Y et U une partie ouverte de Z, il résulte de la *Remarque 2* (X, p. 27) que la topologie de $C_c(X; C_c(Y; Z))$ est engendrée par les ensembles de la forme $T(J, T(K, U))$, K et U étant comme ci-dessus et J une partie compacte de X.

Or, l’image de $T(J, T(K, U))$ par $\rho^{-1}$ n’est autre que $T(J \times K, U)$, donc est un ensemble ouvert, et cela montre déjà que $\rho$ est continue. Inversement, remarquons que les ensembles de la forme $J \times K$ dans $X \times Y$ (J partie compacte de X, K partie compacte de Y) vérifient la condition (R) de la *Remarque 2* (X, p. 27): en effet, si L est une partie compacte de $X \times Y$ et V un voisinage de L dans $X \times Y$, les projections $M = pr_1(L)$, $N = pr_2(L)$ sont compactes, X et Y étant séparés, et $V \cap (M \times N)$ est un voisinage de L dans l’espace compact $M \times N$; donc tout point de L admet dans $M \times N$ un voisinage de la forme $J \times K \subset V$, où $J \subset M$ et $K \subset N$ sont compacts; comme on peut recouvrir L par un nombre fini de ces voisinages, notre assertion en résulte. Les ensembles de la forme $T(J \times K; U)$ (U ouvert dans Z, J (resp. K) compact dans X (resp. Y)) engendrent donc la topologie de $C_c(X \times Y; Z)$; comme nous avons vu que l’image de $T(J \times K, U)$ par $\rho$ est l’ensemble ouvert $T(J, T(K, U))$ dans $C_c(X; C_c(Y; Z))$, cela achève de prouver que $\rho$ est un homéomorphisme.

On notera que lorsque Z est en outre supposé uniformisable, le cor. 2 est une conséquence triviale de X, p. 5, prop. 2.

#### Proposition 9 {#top-x-s3-prop-9 .statement}

*Soient X, Y, Z trois espaces topologiques, Y étant localement compact. Alors l’application $(u, v) \mapsto v \circ u$ de $C_c(X; Y) \times C_c(Y; Z)$ dans $C_c(X; Z)$ est continue.*

Il faut prouver que pour toute partie compacte K de X et toute partie ouverte U de Z, l’ensemble R des couples $(u, v)$ tels que $v(u(K)) \subset U$ est ouvert dans $C_c(X; Y) \times C_c(Y; Z)$. Soit $(u_0, v_0)$ un élément de R. Alors $u_0(K)$ est une partie compacte de l’espace localement compact Y, contenue dans l’ensemble ouvert $v_0^{-1}(U)$, donc il existe un voisinage compact L de $u_0(K)$ contenu dans $v_0^{-1}(U)$ (I, p. 65, prop. 10). L’ensemble V des $u \in C_c(X; Y)$ tels que $u(K) \subset \hat{L}$ est un voisinage de $u_0$, et l’ensemble W des $v \in C_c(Y; Z)$ tels que $v(L) \subset U$ est un voisinage de $v_0$; en outre, la relation $(u, v) \in V \times W$ implique $v(u(K)) \subset U$, d’où la proposition.

### 5. Topologies sur les groupes d’homéomorphismes

#### Proposition 10 {#top-x-s3-prop-10 .statement}

Soient X un espace uniforme, H un ensemble équicontinu d’homéomorphismes de X sur lui-même. Si on munit H et $H^{-1}$ de la topologie de la convergence simple dans X, l’application $u \mapsto u^{-1}$ de $H^{-1}$ sur H est continue.

Il suffit de prouver que, pour tout $x_0 \in X$, l’application $u \mapsto u^{-1}(x_0)$ de $H^{-1}$ dans X est continue en tout point $u_0 \in H^{-1}$. Soit V un entourage symétrique de X, et posons $y_0 = u_0^{-1}(x_0)$. Par hypothèse, il existe un entourage symétrique U de X tel que la relation $(x, x_0) \in U$ implique $(u^{-1}(x), u^{-1}(x_0)) \in V$ pour tout $u \in H^{-1}$. Prenons $u \in H^{-1}$ voisin d’ordre $W(\{y_0\}, U)$ de $u_0$; on a donc

$$(u(y_0), u_0(y_0)) \in U,$$

c’est-à-dire $(u(y_0), x_0) \in U$. On en déduit $(y_0, u^{-1}(x_0)) \in V$, c’est-à-dire $(u_0^{-1}(x_0), u^{-1}(x_0)) \in V$, ce qui achève la démonstration.

#### Corollaire {#top-x-s3-n5-cor-1 .statement}

Soient X un espace uniforme, H un groupe équicontinu d’homéomorphismes de X sur lui-même. Alors la topologie de la convergence simple dans X est compatible (III, p. 1) avec la structure de groupe de H.

Cela résulte de la prop. 10, ainsi que de X, p. 13, cor. 5.

#### Proposition 11 {#top-x-s3-prop-11 .statement}

Soient X un espace compact, Γ le groupe de tous les homéomorphismes de X sur lui-même. Alors la topologie de la convergence uniforme dans X est compatible (III, p. 1) avec la structure de groupe de Γ.

On sait déjà (X, p. 29, prop. 9) que l’application $(u, v) \mapsto v \circ u$ de $\Gamma \times \Gamma$ dans Γ est continue pour cette topologie, et tout revient donc à prouver que $u \mapsto u^{-1}$ est continue en tout point $u_0 \in \Gamma$. Comme $u_0^{-1}$ est uniformément continue dans X, pour tout entourage symétrique V de X il existe un entourage W de X tel que la relation $(x, x') \in W$ entraîne $(u_0^{-1}(x), u_0^{-1}(x')) \in V$. Cela étant, si $u \in \Gamma$ est tel que $(u_0(x), u(x)) \in W$ pour tout $x \in X$, on en conclut d’après ce qui précède $(x, u_0^{-1}(u(x))) \in V$ pour tout $x \in X$, d’où, puisque $u$ est bijective, $(u^{-1}(x), u_0^{-1}(x)) \in V$ pour tout $x \in X$, ce qui achève la démonstration.

Soit maintenant X un espace localement compact et soit Γ le groupe des homéomorphismes de X sur lui-même; la topologie de la convergence compacte dans X n’est pas nécessairement compatible avec la structure de groupe de Γ (X, p. 51, exerc. 17). Désignons par X’ l’espace compact obtenu par adjonction à X d’un point à l’infini $\omega$; tout homéomorphisme $u$ de $X$ sur lui-même se prolonge d’une seule manière en un homéomorphisme $u'$ de $X'$ sur lui-même tel que $u'(\omega) = \omega$ (I, p. 67, th. 4), de sorte que $\Gamma$ s’identifie au sous-groupe du groupe $\Gamma'$ de tous les homéomorphismes de $X'$, formé des homéomorphismes laissant $\omega$ invariant. Sur $\Gamma$, la topologie induite par celle de $C_u(X'; X')$ est donc compatible avec la structure de groupe (prop. 11), et $\Gamma$ est fermé dans $\Gamma'$ (pour la topologie induite par celle de $C_u(X'; X')$) puisqu’il est défini par l’équation $u'(\omega) = \omega$ (X, p. 4, Remarque 6). Nous noterons $\mathcal{T}_\beta$ la topologie de groupe ainsi définie sur $\Gamma$; elle est plus fine que la topologie de la convergence compacte, et peut aussi (en vertu de X, p. 7, prop. 6) être définie comme la topologie de la convergence uniforme dans $X$, quand on munit $X$ de la structure uniforme induite par l’unique structure uniforme de $X'$.

La topologie $\mathcal{T}_\beta$ peut être caractérisée de la façon suivante:

#### Proposition 12 {#top-x-s3-prop-12 .statement}

*Sur le groupe $\Gamma$ des homéomorphismes d’un espace localement compact $X$, la topologie $\mathcal{T}_\beta$ est la moins fine rendant continues les deux applications $u \mapsto u$ et $u \mapsto u^{-1}$ de $\Gamma$ dans l’espace $C_c(X; X)$.*

Désignons pour un moment par $\mathcal{T}'$ cette dernière topologie. Comme $u \mapsto u^{-1}$ est continue pour $\mathcal{T}_\beta$ et que $\mathcal{T}_\beta$ est plus fine que la topologie de la convergence compacte, il est clair que $\mathcal{T}_\beta$ est plus fine que $\mathcal{T}'$. Pour démontrer la réciproque, munissons $X'$ de son unique structure uniforme; soit $u_0 \in \Gamma$ et soit $V$ un entourage de $X'$; il faut prouver qu’il existe une partie compacte $K$ de $X$ et un entourage symétrique $W$ de $X'$ tels que les relations

$$
u \in \Gamma,\ (u_0(x), u(x)) \in W \text{ et } (u_0^{-1}(x), u^{-1}(x)) \in W \text{ pour tout } x \in K
$$

entraînent $(u_0(x), u(x)) \in V$ pour tout $x \in X$. Soit $V_1$ un entourage symétrique ouvert de $X'$ tel que $V_1^2 \subset V$; alors $K_1 = X' - V_1(\omega)$ est une partie compacte de $X$. Prenons l’entourage ouvert symétrique $W$ de $X'$ tel que $W \subset V$ et que l’on ait $W(\omega) \cap W(u_0^{-1}(K_1)) = \varnothing$, ce qui est possible en vertu de II, p. 31, prop. 4; soit $K_2 = X' - W(\omega)$, qui est une partie compacte de $X$; nous allons voir que $W$ et l’ensemble compact $K = K_1 \cup K_2$ répondent à la question. Puisque $W \subset V$, il suffit en effet de prouver que la relation $(u_0^{-1}(x), u^{-1}(x)) \in W$ pour tout $x \in K_1$ (avec $u \in \Gamma$) implique que, pour tout $y \in W(\omega)$, on a $(u(y), \omega) \in V_1$; on aura alors aussi $(u_0(y), \omega) \in V_1$, donc $(u_0(y), u(y)) \in V_1^2 \subset V$ pour tout $y \in W(\omega) = X' - K_2$. Or, si on avait $y \in W(\omega)$ et $u(y) \in X' - V_1(\omega) = K_1$, on en conclurait $y \in u^{-1}(K_1) \subset W(u_0^{-1}(K_1))$, contrairement au choix de $W$, ce qui termine la démonstration.

En général, le groupe $\Gamma$, muni de $\mathcal{T}_\beta$, n’est pas localement compact (X, p. 50, exerc. 16 b)); mais on a le critère suivant:

#### Théorème 4 {#top-x-s3-thm-4 .statement}

Soit G un sous-groupe du groupe Γ des homéomorphismes d’un espace localement compact X. Supposons qu’il existe, dans l’espace $C_c(X; X)$, un voisinage V de l’application identique e tel que $V \cap G = H$ soit symétrique dans G et relativement compact dans $C_c(X; X)$. Alors l’adhérence $\overline{G}$ de G dans Γ pour la topologie $\mathcal{T}_\beta$ est un groupe localement compact pour la topologie induite par $\mathcal{T}_\beta$; cette topologie induite sur $\overline{G}$ est d’ailleurs identique à la topologie de la convergence compacte, et l’adhérence $\overline{H}$ de H dans $C_c(X; X)$ est un voisinage de e dans $\overline{G}$ pour cette topologie.

Montrons d’abord que $\overline{H}$ est contenu dans Γ et que sur $\overline{H}$, la topologie induite par $\mathcal{T}_\beta$ est identique à la topologie de la convergence compacte. Soit $u_0 \in \overline{H}$, qui est donc limite, dans $C_c(X; X)$, d’un ultrafiltre $\Phi$ sur H; comme $\Phi^{-1}$ (image de $\Phi$ par $u \mapsto u^{-1}$) est une base d’ultrafiltre sur $H \subset \overline{H}$, il converge dans le sous-espace compact $\overline{H}$ de $C_c(X; X)$ vers un élément $v_0$. L’application $(u, v) \mapsto uv$ converge vers $u_0v_0$ suivant $\Phi \times \Phi^{-1}$ (X, p. 29, prop. 9); a fortiori, $u \mapsto uu^{-1} = e$ converge vers $u_0v_0$ suivant $\Phi$, donc $u_0v_0 = e$ puisque $C_c(X; X)$ est séparé; on voit de même que $v_0u_0 = e$, ce qui prouve que $u_0$ et $v_0$ sont des bijections réciproques de X, d’où la première assertion. En outre, ce raisonnement montre que $\overline{H}^{-1} = \overline{H}$ et que pour tout ultrafiltre $\Phi$ sur $\overline{H}$ qui converge vers $u_0$, $\Phi^{-1}$ converge dans $C_c(X; X)$ vers $u_0^{-1}$; donc l’application $u \mapsto u^{-1}$ de $\overline{H}$ dans $C_c(X; X)$ est continue lorsque $\overline{H}$ est muni de la topologie de la convergence compacte (I, p. 50, cor. 1). La prop. 12 (X, p. 31) prouve alors que sur $\overline{H}$, la topologie de la convergence compacte est identique à la topologie induite par $\mathcal{T}_\beta$.

En outre, comme sur Γ la topologie $\mathcal{T}_\beta$ est plus fine que la topologie de la convergence compacte, $\overline{H}$ est aussi l’adhérence de H pour $\mathcal{T}_\beta$; or, H est un voisinage de e dans G pour la topologie de la convergence compacte, et a fortiori pour la topologie induite par $\mathcal{T}_\beta$; on en déduit (I, p. 18, prop. 2) que $\overline{H}$ est un voisinage de e dans $\overline{G}$ pour la topologie induite par $\mathcal{T}_\beta$, ce qui prouve que $\overline{G}$ est localement compact pour cette topologie. En outre, si W est l’intérieur de V pour la topologie de la convergence compacte, $W \cap \Gamma$ est ouvert pour $\mathcal{T}_\beta$, donc $W \cap \overline{G}$ est contenu dans l’adhérence de $H = V \cap G$ pour $\mathcal{T}_\beta$ (I, p. 7, prop. 5), ce qui prouve que $\overline{H}$ est aussi un voisinage de e dans $\overline{G}$ pour la topologie de la convergence compacte. Enfin, pour tout $u_0 \in \Gamma$, les bijections réciproques $v \mapsto u_0 \circ v$ et $v \mapsto u_0^{-1} \circ v$ de $C_c(X; X)$ sur lui-même sont continues (X, p. 29, prop. 9), donc, pour $u_0 \in \overline{G}$, $u_0 \overline{H}$ est un voisinage de $u_0$ dans $\overline{G}$ pour la topologie de la convergence compacte, ce qui achève la démonstration.

#### Corollaire {#top-x-s3-n5-cor-2 .statement}

Soit G un groupe d’homéomorphismes d’un espace localement compact X. Si l’adhérence $\overline{G}$ de G dans $C_c(X; X)$ est compacte, $\overline{G}$ est un groupe d’homéomorphismes de X, et la topologie de la convergence compacte est compatible avec la structure de groupe de $\overline{G}$, qui est donc un groupe compact.

Un groupe d’homéomorphismes d’un espace localement compact X qui est localement compact (non compact) pour la topologie de la convergence compacte, est localement fermé dans $C_c(X; X)$ en vertu de I, p. 66, prop. 12, mais n’est pas nécessairement fermé.

Par exemple dans l’anneau $\mathcal{L}(\mathbf{R}^n)$ des endomorphismes de $\mathbf{R}^n$, identifié à l’anneau $\mathbf{M}_n(\mathbf{R})$ des matrices carrées d’ordre n sur $\mathbf{R}$, et muni de la topologie de la convergence compacte, le groupe $\mathbf{GL}(n, \mathbf{R})$, identifié au groupe des matrices inversibles, est localement compact, mais partout dense (VI, p. 6, prop. 6).

## EXERCICES {#top-x-s3-exercises}

See the [exercises for § 3](exercises/s3/).
