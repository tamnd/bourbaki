---
book: var
book_title: Variétés différentielles et analytiques
chapter: "1"
chapter_title: VARIÉTÉS DIFFÉRENTIELLES ET ANALYTIQUES, FASCICULE DE RÉSULTATS
section: 1
section_title: Fonctions différentiables
lang: fr
source: var-fr
pdf_pages: 0009-0014
extraction: ocr
subsections:
    - "no": 1
      title: Ordre de contact de deux fonctions en un point
      page: 0
      pdf_page: 9
    - "no": 2
      title: Fonctions dérivables en un point
      page: 0
      pdf_page: 10
    - "no": 3
      title: Composition des fonctions dérivables
      page: 0
      pdf_page: 11
    - "no": 4
      title: Produit de fonctions dérivables
      page: 0
      pdf_page: 12
    - "no": 5
      title: Premières variantes du théorème des fonctions implicites
      page: 0
      pdf_page: 12
    - "no": 6
      title: Dérivées partielles
      page: 0
      pdf_page: 13
    - "no": 7
      title: Dérivées itérées
      page: 0
      pdf_page: 13
statements: 0
exercises: 0
content_sha256: 68a240194e02f682042deb25f428d16a60db5f87c651da158fc9feeead037a42
---

## § 1. Fonctions différentiables

Dans ce paragraphe, la lettre E désigne un espace vectoriel topologique normable sur K ; la lettre F désigne un espace polynormé séparé sur K.

### 1.1 Ordre de contact de deux fonctions en un point

1.1.1. Soient X un espace topologique et $\theta$ une fonction numérique positive définie dans un voisinage d’un point $x_0$ de X. On dit qu’une fonction $f$, définie dans un voisinage de $x_0$ et à valeurs dans F, est négligeable devant $\theta$ en $x_0$ si la condition suivante est satisfaite :

Pour tout $\varepsilon > 0$ et pour toute semi-norme $\gamma$ continue sur F, il existe un voisinage V de $x_0$ sur lequel $f$ et $\theta$ sont définies et tel que

$$
\| f(x) \|_{\gamma} \leq \varepsilon \theta(x) \quad \text{pour tout } x \in V.
$$

Pour que $f$ soit négligeable devant $\theta$, il suffit que cette condition soit satisfaite pour une famille de semi-normes $\gamma$ définissant la topologie de F. Le faite que $f$ soit négligeable ou non devant $\theta$ en $x_0$ ne dépend que des germes de $f$ et de $\theta$ en $x_0$. On désigne par $o_{x_0}(\theta)$ (ou $o(\theta)$ lorsqu’il n’y a pas d’ambiguïté sur $x_0$) l’ensemble des germes en $x_0$ de fonctions négligeables devant $\theta$ en $x_0$ : c’est un sous-espace vectoriel de l’espace des germes en $x_0$ d’applications à valeurs dans F. Si $f$ est négligeable devant $\theta$, on écrira par abus de notations, $f \in o_{x_0}(\theta)$ ou encore $f(x) \in o(\theta(x))$ lorsque $x$ tend vers $x_0$.

Si $f$ et $g$ sont deux applications d’un voisinage de $x_0$ dans F, on écrira encore $f \equiv g \mod o(\theta)$ si $f - g$ est négligeable devant $\theta$.

Supposons que K soit égal à $\mathbf{R}$ ou $\mathbf{C}$ et que $x_0$ soit adhérent à l’ensemble Y des points de X où $\theta$ est définie et non nulle. La relation $f \in o(\theta)$ signifie alors que $f(x)/\theta(x)$ tend vers 0 lorsque $x$ tend vers $x_0$ en restant dans Y, et que $\theta(x) = 0$ entraîne $f(x) = 0$.

1.1.2. Soient $f$ et $g$ deux fonctions à valeurs dans F, définies au voisinage d’un point $x_0$ de E. Si $m$ est un entier positif, on dit que $f$ et $g$ ont un contact d’ordre $\geq m$ en $x_0$ si l’on a :

$$
f(x) - g(x) \in o(\| x - x_0 \|^{m}) \quad \text{pour } x \text{ tendant vers } x_0
$$

quelle que soit la norme choisie pour définir la topologie de E. Pour cela, il suffit que la relation précédente soit vérifiée pour une norme définissant la topologie de E. S’il en est ainsi, on a $f(x_0) = g(x_0)$.

Si $f$ et $g$ prennent la même valeur en $x_0$, on appelle ordre de contact de $f$ et $g$ en $x_0$ la borne supérieure (finie ou égale à $+\infty$) des entiers $m$ tels que $f$ et $g$ aient un contact d’ordre $\geq m$ en $x_0$.

1.1.3. L’ordre de contact de $f$ et $g$ en $x_0$ ne dépend que des germes de ces fonctions au point $x_0$. On peut donc parler de l’ordre de contact de deux germes $\varphi$ et $\psi$ d’applications de E dans F au point $x_0$. La relation « $\varphi$ et $\psi$ ont un contact d’ordre $\geq m$ » est une relation d’équivalence compatible avec la structure vectorielle.

### 1.2. Fonctions dérivables en un point

1.2.1. Soit $f$ une fonction définie dans un voisinage du point $x_0$ de E et à valeurs dans F. On dit que $f$ est dérivable en $x_0$ s’il existe une fonction affine continue $v$ de E dans F ayant en $x_0$ un contact d’ordre $\geq 1$ avec $f$. Cette application $v$ est unique; il existe une application linéaire continue et une seule, notée $Df(x_0)$, de E dans F telle que:

$$
v(x) = v(x_0) + Df(x_0) \cdot (x - x_0).
$$

Si l’on choisit une norme sur E, ceci équivaut à:

$$
f(x_0 + h) \equiv f(x_0) + Df(x_0) \cdot h \mod o(\|h\|) \quad \text{pour } h \text{ tendant vers } 0,
$$

ce que l’on peut encore écrire sous la forme:

$$
\lim_{h \to 0, h \neq 0} \frac{\| f(x_0 + h) - f(x_0) - Df(x_0) \cdot h \|_\gamma}{\| h \|} = 0
$$

pour toute semi-norme $\gamma$ continue sur F.

L’élément $Df(x_0)$ de $\mathcal{L}(E, F)$ s’appelle la dérivée de $f$ en $x_0$. On écrit parfois $D_h f(x_0)$ pour $Df(x_0) \cdot h$; c’est une élément de F défini par la relation:

$$
D_h f(x_0) = \lim_{t \to 0, t \neq 0} \frac{f(x_0 + th) - f(x_0)}{t}.
$$

1.2.2. On dit qu’une fonction $f$ est strictement dérivable en $x_0$ si elle est dérivable en $x_0$ et si l’on a, pour toute norme définissant la topologie de E, la relation:

$$
f(y) - f(z) \equiv Df(x_0) \cdot (y - z) \mod o(\| y - z \| )
$$

pour $(y, z)$ tendant vers $(x_0, x_0)$ dans $E \times E$. Pour cela, il suffit que cette condition soit satisfaite pour une norme définissant la topologie de E. Supposons de plus E et F normés; pour tout nombre $c > \| Df(x_0) \|$, il existe alors un voisinage V de $x_0$ tel que $\| f(y) - f(z) \| \leq c. \| y - z \|$ pour $y, z$ dans V ; ceci entraîne que $f$ est uniformément continue dans V.

1.2.3. Le fait pour une fonction $f$ d’être dérivable ou strictement dérivable en $x_0$ ne dépend que du germe de $f$ en $x_0$. Les germes de fonctions dérivables en $x_0$ forment un sous-espace vectoriel $\mathcal{V}$ de l’espace de tous les germes et l’application $f \mapsto Df(x_0)$ de $\mathcal{V}$ dans $\mathcal{L}(E; F)$ est linéaire. Les germes de fonctions strictement dérivables en $x_0$ forment un sous-espace vectoriel de $\mathcal{V}$.

1.2.4. Une fonction dérivable en $x_0$ est continue en $x_0$.

1.2.5. Lorsque $E = K$, l’application $u \mapsto u(1)$ est un isomorphisme de $\mathcal{L}(E; F)$ sur $F$; si la fonction $f$ est dérivable en $x_0$, l’élément

$$
f'(x_0) = Df(x_0) \cdot 1
$$

n’est autre que la dérivée de $f$ en $x_0$ au sens donné dans Fonct. Var. Réelle, chap. I, § 1, n° 6, remarque 2.

### 1.3. Composition des fonctions dérivables

1.3.1. Supposons F normable. Soient $x_0 \in E$ et $y_0 \in F$, U un voisinage de $x_0$ et V un voisinage de $y_0$; enfin soit $f$ une application de U dans V, dérivable en $x_0$, avec $f(x_0) = y_0$. Si $g$ est une application de V dans un espace vectoriel polynormé séparé G, dérivable en $y_0$, l’application $g \circ f$ de U dans G est dérivable en $x_0$, et l’on a :

(1)
$$
D(g \circ f)(x_0) = Dg(y_0) \circ Df(x_0).
$$
Si $f$ et $g$ sont strictement dérivables, il en est de même de $g \circ f$.

1.3.2. Soit $f$ une application définie au voisinage d’un point $x_0$ de E et à valeurs dans F, dérivable en $x_0$; si $u$ est une application linéaire continue de F dans un espace polynormé séparé G, la fonction $u \circ f$ est dérivable en $x_0$ et l’on a :

(2)
$$
D(u \circ f)(x_0) = u \circ Df(x_0).
$$

1.3.3. Supposons que F soit produit d’une famille $(F_i)_{i \in I}$ d’espaces vectoriels polynormés séparés; pour tout $i$ dans I, soit $f_i$ une application définie dans un voisinage U d’un point $x_0$ de E et à valeurs dans F et soit $f = (f_i)_{i \in I}$. Pour que $f$ soit dérivable (resp. strictement dérivable) en $x_0$, il faut et il suffit que tous les $f_i$ le soient; on a :

(3)
$$
D_h f(x_0) = (D_h f_i(x_0))_{i \in I} \quad \text{pour tout } h \text{ dans } E.
$$

1.3.4. Si $E = K$, on peut remplacer $Df(x_0)$ par $f'(x_0)$ et $D_h f_i(x_0)$ par $f'_i(x_0)$ dans les formules (1) et (3).

### 1.4. Produit de fonctions dérivables

1.4.1. Soient $F_1, \ldots, F_m$ des espaces polynormés séparés et $u$ une application $m$-linéaire continue de $F_1 \times \cdots \times F_m$ dans $F$. Soit $U$ un voisinage d’un point $x_0$ de $E$, et soit $f_i$ une application de $U$ dans $F_i$ (pour $1 \leq i \leq m$). Si les $f_i$ sont dérivables (resp. strictement dérivables) en $x_0$, il en est de même de $u(f_1, \ldots, f_m) = g$ et l’on a:

(4) $D_hg(x_0) = \sum_{j=1}^m u(f_1(x_0), \ldots, D_hf_j(x_0), \ldots, f_m(x_0))$ pour $h$ dans $E$,

ce que l’on écrira plus succinctement :

(5) $Dg = \sum_{j=1}^m u(f_1, \ldots, Df_j, \ldots, f_m)$.

En particulier, pour $m = 2$, on a :

(6) $Du(f_1, f_2) = u(Df_1, f_2) + u(f_1, Df_2)$.

Pour $m = 1$, on retrouve 1.3.2.

1.4.2. Lorsque $E = K$, on peut remplacer $Dg$ par $g'$ et $Df_j$ par $f'_j$ dans les formules (4) à (6).

### 1.5. Premières variantes du théorème des fonctions implicites

Supposons que $E$ et $F$ sont des espaces de Banach et soient $x_0$ un point de $E$, $U$ un voisinage de $x_0$ et $f$ une application de $U$ dans $F$. On suppose de plus que $f$ est strictement dérivable en $x_0$.

1.5.1. Si $Df(x_0)$ est un isomorphisme de $E$ sur $F$, il existe un voisinage ouvert $U_0$ de $x_0$ contenu dans $U$ et un voisinage ouvert $V_0$ de $f(x_0)$ tels que $f|U_0$ soit un homéomorphisme de $U_0$ sur $V_0$. L’application $g : V_0 \to U_0$ réciproque de $f|U_0$ est strictement dérivable au point $f(x_0)$ et l’on a :

$$
Dg(f(x_0)) = Df(x_0)^{-1}.
$$

1.5.2. Si $Df(x_0)$ est une application surjective de $E$ sur $F$, il existe un voisinage ouvert $U_0$ de $x_0$ contenu dans $U$, tel que $f|U_0$ soit une application ouverte.

1.5.3. Si $Df(x_0)$ est injective et d’image fermée, il existe un voisinage fermé $U_0$ de $x_0$ contenu dans $U$, tel que $f|U_0$ soit un homéomorphisme de $U_0$ sur une partie fermée de $F$.

### 1.6. Dérivées partielles

1.6.1. Soit $f$ une fonction définie dans un voisinage $U$ du point $x_0$ de $E$ et à valeurs dans $F$. Soient $X$ un sous-espace vectoriel de $E$ et $V$ l’ensemble des points $x$ de $X$, tels que $x_0 + x \in U$; posons $g(x) = f(x_0 + x)$ pour $x \in V$. On dit que $f$ admet une *dérivée partielle suivant* $X$ *en* $x_0$ si $g$ admet une dérivée en $0$; cette dérivée se note $D_X f(x_0)$; c’est une application linéaire continue de $X$ dans $F$. Si $f$ est dérivable en $x_0$, elle admet une dérivée partielle suivant $X$ en $x_0$ et cette dérivée partielle est la restriction de $Df(x_0)$ à $X$.

1.6.2. Supposons que $E$ soit produit d’une famille finie d’espaces vectoriels normés $E_i$ ($1 \leq i \leq n$) identifiés canoniquement à des sous-espaces de $E$; soit $x_0 = (x_0^1, \ldots, x_0^n)$ dans $E$ et soit $U$ un voisinage de $x_0$ dans $E$; enfin soit $f$ une application de $U$ dans $F$. On note $D_{i} f(x_0)$ la dérivée au point $x_0^i$, si elle existe, de l’application $z_i \mapsto f(x_0^1, \ldots, z_i, \ldots, x_0^n)$ définie au voisinage de $x_0^i$ dans $E_i$ et à valeurs dans $F$. C’est un élément de $\mathcal{L}(E_i; F)$ que l’on appelle la *i-ème dérivée partielle de* $f$ *en* $x_0$. Si $f$ est dérivable en $x_0$, les $n$ dérivées partielles existent, et déterminent $Df(x_0)$ par la formule :

$$
Df(x_0) \cdot h = \sum_{i=1}^{n} D_{i} f(x_0) \cdot h_i \quad \text{pour } h = (h_1, \ldots, h_n) \text{ dans } E.
$$

1.6.3. Plus particulièrement, soit $E = K^n$. Si les dérivées partielles de $f$ en $x_0$ existent, on note $\partial_{i} f(x_0)$ l’élément $D_{i} f(x_0) \cdot 1$ de $F$. L’écriture suivante est souvent usitée ; supposons qu’on ait choisi une notation pour les fonctions coordonnées sur $K^n$, par exemple $u_i$ désigne la $i$-ème projection de $K^n$ sur $K$. On écrit alors :

$$
\frac{\partial f}{\partial u_i}(x_0) \quad \text{ou} \quad \left. \frac{\partial f}{\partial u_i} \right|_{x = x_0}
$$

au lieu de $\partial_{i} f(x_0)$.

1.6.4. Soient $E = K^n$ et $F = K^m$; supposons que la fonction $f = (f_1, \ldots, f_m)$ à valeurs dans $F$ soit dérivable au point $x_0$ de $E$. Les dérivées partielles $a_{ji} = \partial_{i} f_j(x_0)$ existent alors (ce sont des éléments de $K$). La matrice à $m$ lignes et $n$ colonnes formée des $a_{ji}$ (élément de la ligne d’indice $j$ et de la colonne d’indice $i$) s’appelle la *matrice jacobienne* de $f$ en $x_0$; c’est la matrice de l’application linéaire $Df(x_0)$ de $K^n$ dans $K^m$ par rapport aux bases canoniques de ces espaces.

### 1.7. Dérivées itérées

1.7.1. Soit $f$ une fonction définie dans un voisinage d’un point $x_0$ de $E$, à valeurs dans $F$. Si $f$ est dérivable au voisinage de $x_0$, sa dérivée $Df$ est une application d’un voisinage de $x_0$ dans l’espace polynormé $\mathcal{L}(E; F)$ des applications linéaires continues de $E$ dans $F$. Soit $p$ un entier $\geq 2$:

on dit que $f$ est $p$ fois dérivable en $x_0$ si $f$ est dérivable au voisinage de $x_0$ et si sa dérivée $Df$ est $(p - 1)$ fois dérivable en $x_0$. On définit alors la dérivée $p$-ième de $f$ en $x_0$: c'est l'application $p$-linéaire continue $D^pf(x_0)$ de $E^p$ dans $F$, définie par:

$$
D^pf(x_0) . (h_1, \ldots, h_p) = (D(D^{p-1}f)(x_0) . h_1) . (h_2, \ldots, h_p).
$$

On pose aussi $D^0f = f$ et $D^1f = Df$. Si $f$ est $p$ fois dérivable en $x_0$ et si $q$ et $s$ sont deux entiers tels que $q + s = p$, avec $s > 0$, alors $f$ est $q$ fois dérivable au voisinage de $x_0$, la fonction $D^qf$ (à valeurs dans $\mathcal{L}_q(E; F)$) est $s$ fois dérivable en $x_0$, et on a:

$$
D^{q+s}f(x_0) . (h_1, \ldots, h_{q+s}) = (D^s(D^qf)(x_0) . (h_1, \ldots, h_s)) . (h_{s+1}, \ldots, h_{q+s})
$$

relation que l'on écrit par abus de notation sous la forme:

$$
D^{q+s}f = D^s D^qf.
$$

1.7.2. Soient $(E_i)_{1 \leq i \leq n}$ des sous-espaces vectoriels fermés de $E$, tels que $E$ soit somme directe topologique des $E_i$. On définit alors, quand elle existe, la dérivée partielle itérée $D_{i_1} \ldots D_{i_m}f$ d'une application $f$ d'un voisinage de $x_0 \in E$ dans $F$; c'est une application multilinéaire continue de

$$
E_{i_1} \times \cdots \times E_{i_m}
$$

dans $F$, définie par récurrence sur l'entier $m \geq 1$ comme suit : si $D_{i_2} \ldots D_{i_m}f(x)$ existe dans un voisinage de $x_0$ et possède une dérivée partielle suivant $E_{i_1}$, alors $D_{i_1} \ldots D_{i_m}f(x_0)$ est donnée par:

$$
D_{i_1} \ldots D_{i_m}f(x_0) . (h_1, \ldots, h_m) = (D_{i_1}(D_{i_2} \ldots D_{i_m}f)(x_0) . h_1) . (h_2, \ldots, h_m)
$$

pour $h_k \in E_{i_k}$.

Si $f$ est $m$ fois dérivable en $x_0$, alors la dérivée partielle $D_{i_1} \ldots D_{i_m}f(x_0)$ existe et est égale à la restriction de $D^m f(x_0)$ au sous-espace $E_{i_1} \times \cdots \times E_{i_m}$ de $E^m$. Par suite, $D^m f(x_0)$ est complètement déterminée par les dérivées partielles itérées d'ordre $m$ en $x_0$.

1.7.3. Supposons que $E$ soit de dimension finie et soit $(e_1, \ldots, e_n)$ une base de $E$. Posons $E_i = K e_i$ et soit $f$ une application d'un voisinage de $x_0$, à valeurs dans $F$. Si la dérivée partielle $D_{i_1} \ldots D_{i_m}f(x_0)$ (avec les notations de 1.7.2) existe, on pose:

$$
\partial_{i_1} \ldots \partial_{i_m} f(x_0) = D_{i_1} \ldots D_{i_m} f(x_0) . (e_{i_1}, \ldots, e_{i_m}).
$$
