---
book: top
book_title: General Topology
chapter: VII
chapter_title: LES GROUPES ADDITIFS $\mathbf{R}^n$
section: 2
section_title: Homomorphismes continus de $\mathbf{R}^n$ et de ses groupes quotients
lang: fr
source: top-v-x-fr
book_pages: TG VII.11-TG VII.15
pdf_pages: 0069-0073, 0081-0083
extraction: ocr
subsections:
    - "no": 1
      title: Homomorphismes continus du groupe $\mathbf{R}^m$ dans le groupe $\mathbf{R}^n$
      page: 11
      pdf_page: 69
    - "no": 2
      title: Définition locale d’un homomorphisme continu de $\mathbf{R}^n$ dans un groupe topologique
      page: 11
      pdf_page: 69
    - "no": 3
      title: Homomorphismes continus de $\mathbf{R}^m$ dans $T^n$
      page: 13
      pdf_page: 71
    - "no": 4
      title: Automorphismes de $\mathbf{T}^n$
      page: 14
      pdf_page: 72
statements: 12
exercises: 7
content_sha256: 1ecb29f9c9ce268252169ba91c1887d162e07aba9ba86dc3ef66056bf668d2c7
---

## § 2. HOMOMORPHISMES CONTINUS DE $\mathbf{R}^n$ ET DE SES GROUPES QUOTIENTS

### 1. Homomorphismes continus du groupe $\mathbf{R}^m$ dans le groupe $\mathbf{R}^n$

Toute application linéaire de $\mathbf{R}^m$ dans $\mathbf{R}^n$ est évidemment un homomorphisme continu du groupe additif $\mathbf{R}^m$ dans le groupe additif $\mathbf{R}^n$. Réciproquement:

#### Proposition 1 {#top-vii-s2-prop-1 .statement}

Tout homomorphisme continu $f$ du groupe additif $\mathbf{R}^m$ dans le groupe additif $\mathbf{R}^n$ est une application linéaire de $\mathbf{R}^m$ dans $\mathbf{R}^n$.

Il suffit de montrer que, pour tout $x \in \mathbf{R}^m$ et tout $t \in \mathbf{R}$, on a $f(tx) = tf(x)$. Le raisonnement est le même que celui de la prop. 5 de V, p. 2 en remplaçant $x$ par $x$ et $\mathbf{R}$ par $\mathbf{R}^m$.

### 2. Définition locale d’un homomorphisme continu de $\mathbf{R}^n$ dans un groupe topologique

La prop. 6 de V, p. 3, se généralise à tous les groupes $\mathbf{R}^n$:

#### Proposition 2 {#top-vii-s2-prop-2 .statement}

Soit $A$ un parallélétope de $\mathbf{R}^n$ tel que $0 \in A$; soit $f$ une application continue de $A$ dans un groupe topologique $G$ (noté multiplicativement), telle que $f(x + y) = f(x)f(y)$ pour tout couple de points $x, y$ tels que $x \in A, y \in A, x + y \in A$. Il existe alors un homomorphisme continu et un seul de $\mathbf{R}^n$ dans $G$ qui prolonge $f$.

Par le même raisonnement que dans la prop. 6 de V, p. 3, on prouve d’abord que l’homomorphisme prolongeant $f$, s’il existe, est unique. D’autre part, le sous-groupe $G_1$ de $G$, engendré par $f(A)$, est commutatif; en effet, si $x$ et $y$ sont deux points quelconques de $A$, $\frac{1}{2}x$, $\frac{1}{2}y$ et $\frac{1}{2}(x + y)$ appartiennent à $A$, donc on a $f(\frac{1}{2}(x + y)) = f(\frac{1}{2}x)f(\frac{1}{2}y) = f(\frac{1}{2}y)f(\frac{1}{2}x)$, ce qui prouve que $f(\frac{1}{2}x)$ et $f(\frac{1}{2}y)$ sont permutables; il en est donc de même de $f(x) = (f(\frac{1}{2}x))^2$ et $f(y) = (f(\frac{1}{2}y))^2$, ce qui montre que deux éléments quelconques de $f(A)$ sont permutables.

Soient $a_1, a_2, \ldots, a_n$ $n$ vecteurs non nuls contenus dans $A$ et proportionnels aux vecteurs de base de ce parallélétope; pour chaque indice $i$, soit $D_i$ la droite passant par $0$ et $a_i$, ensemble des points $ta_i$ où $t$ parcourt $\mathbf{R}$. Soit $A_i$ l’ensemble des $t \in \mathbf{R}$ tels que $ta_i \in A$; $A_i$ est un intervalle contenant $(0, 1)$, et la fonction $f_i(t) = f(ta_i)$ est définie et continue dans $A_i$ et satisfait à la relation

$$
f_i(t + t') = f_i(t)f_i(t')
$$

pour $t \in A_i, t' \in A_i$ et $t + t' \in A_i$. D’après la prop. 6 de V, p. 3, il existe un homomorphisme continu $\bar{f}_i$ de $\mathbf{R}$ dans $G$ qui prolonge $f_i$. Comme $\mathbf{R}^n$ est somme directe des sous-groupes $D_i$, on définit un homomorphisme $\bar{f}$ de $\mathbf{R}^n$ dans le groupe commutatif $G_1$ en posant, pour tout $x = \sum_{i=1}^n t_i a_i$, $\bar{f}(x) = \sum_{i=1}^n \bar{f}_i(t_i)$; $\bar{f}$ est un prolongement de $f$, puisque, si $x \in A$, tous les composants $x_i$ de $x$ sur les $D_i$ appartiennent aussi à $A$, d’après le choix des $a_i$; en outre, $\bar{f}$ est continu dans $\mathbf{R}^n$, puisqu’il est continu sur chacune des droites $D_i$, et que $t_i$ est fonction linéaire (donc continue) de $x$.

#### Corollaire 1 {#top-vii-s2-prop-2-cor-1 .statement}

*Soient $V$ un voisinage de $0$ dans $\mathbf{R}^n$, $f$ une application continue de $V$ dans un groupe topologique $G$, telle que $f(x + y) = f(x)f(y)$ pour tout couple de points $x, y$ tels que $x \in V, y \in V, x + y \in V$. Il existe un homomorphisme continu et un seul de $\mathbf{R}^n$ dans $G$, qui coïncide avec $f$ en tous les points d’un voisinage $W$ de $0$.*

Il suffit de prendre pour $W$ un pavé ouvert de centre $0$, contenu dans $V$, et de lui appliquer la prop. 2.

Nous verrons au chap. XI que cette propriété de $\mathbf{R}^n$ s’étend à une catégorie plus générale de groupes topologiques, les groupes « simplement connexes ».

#### Corollaire 2 {#top-vii-s2-prop-2-cor-2 .statement}

*Soit $f$ un isomorphisme local de $\mathbf{R}^n$ à un groupe topologique $G$; il existe un morphisme strict et un seul de $\mathbf{R}^n$ sur un sous-groupe ouvert de $G$, qui coïncide avec $f$ en tous les points d’un voisinage de $0$.*

En effet, soit $\bar{f}$ l’homomorphisme continu de $\mathbf{R}^n$ dans $G$ qui coïncide avec $f$ en tous les points d’un voisinage de $0$; $\bar{f}(\mathbf{R}^n)$ contient par hypothèse un voisinage de l’élément neutre de $G$, donc (III, p. 7, corollaire) est un sous-groupe ouvert de $G$; en outre, $\bar{f}$ est un morphisme strict de $\mathbf{R}^n$ sur $\bar{f}(\mathbf{R}^n)$, d’après III, p. 16, prop. 24.

#### Corollaire 3 {#top-vii-s2-prop-2-cor-3 .statement}

Lorsque $n \neq m$, $\mathbf{R}^n$ et $\mathbf{R}^m$ ne sont pas localement isomorphes.

Supposons $\mathbf{R}^n$ et $\mathbf{R}^m$ localement isomorphes. D’après le cor. 2 et la prop. 1 de VII, p. 11, il existe une application linéaire $f$ de $\mathbf{R}^m$ sur $\mathbf{R}^n$ qui est un isomorphisme local. Alors $f$ est injective, et par suite $m = n$.

Soit $G$ un groupe topologique. Le corollaire précédent montre qu’il existe au plus un entier $n$ tel que $G$ soit localement isomorphe à $\mathbf{R}^n$.

#### Théorème 1 {#top-vii-s2-thm-1 .statement}

Soit $G$ un groupe topologique connexe, localement isomorphe à $\mathbf{R}^n$; il est commutatif. Soit $K$ l’adhérence dans $G$ du sous-groupe de torsion de $G$ (A, II, p. 115). Alors $K$ est le plus grand sous-groupe compact de $G$; il est isomorphe à un tore $T^q$ ($0 \leq q \leq n$). De plus, il existe un sous-groupe fermé $V$ de $G$, isomorphe à $\mathbf{R}^{n-q}$, tel que le groupe topologique $G$ soit le produit direct de ses sous-groupes $K$ et $V$.

D’après le cor. 2 de la prop. 2, il existe un morphisme $f$ de $\mathbf{R}^n$ dans $G$, qui est un isomorphisme local, et qui se prolonge en un morphisme strict de $\mathbf{R}^n$ sur un sous-groupe ouvert de $G$. Comme $G$ est connexe, on a $f(\mathbf{R}^n) = G$; le noyau $H$ de $f$ est discret, puisque son intersection avec un voisinage convenable de 0 dans $\mathbf{R}^n$ est réduite à 0. Soient $W$ le sous-espace vectoriel de $\mathbf{R}^n$ engendré par $H$, $q$ sa dimension, et $V'$ un supplémentaire de $W$. D’après le th. 1 de VII, p. 4, le sous-groupe $K = f(W)$ de $G$ est isomorphe à $T^q$; le sous-groupe $V = f(V')$ de $G$ est isomorphe à $\mathbf{R}^{n-q}$, et le groupe topologique $G$ est le produit direct de ses sous-groupes $K$ et $V$ (III, p. 18, cor. de la prop. 26). Soit $u$ la projection de $G$ sur $V$, de noyau $K$, associée à cette décomposition; si $L$ est un sous-groupe compact de $G$, $u(L)$ est un sous-groupe compact de $V$ (I, p. 63, cor. 1 du th. 2), donc est réduit à 0 (VII, p. 6, cor. 2 du th. 2); on a donc $L \subset K$ et $K$ est bien le plus-grand sous-groupe compact de $G$. Enfin, tout élément de torsion de $G$ engendre un sous-groupe fini, donc appartient à $K$ d’après ce qui précède; le sous-groupe de torsion de $G$ est donc le sous-groupe de torsion de $K$; comme le sous-groupe de torsion de $T^q = (\mathbf{R}/\mathbf{Z})^q$ est $(\mathbf{Q}/\mathbf{Z})^q$, le groupe $K$ est l’adhérence de son sous-groupe de torsion, ce qui achève la démonstration.

#### Corollaire {#top-vii-s2-n2-cor-1 .statement}

Tout groupe connexe $G$, localement isomorphe à $\mathbf{R}^n$, est isomorphe à un groupe $\mathbf{R}^p \times T^{n-p}$ ($0 \leq p \leq n$).

### 3. Homomorphismes continus de $\mathbf{R}^m$ dans $T^n$

#### Proposition 3 {#top-vii-s2-prop-3 .statement}

Tout homomorphisme continu de $\mathbf{R}^m$ dans $T^n$ est de la forme $x \mapsto \varphi(u(x))$, où $\varphi$ est l’homomorphisme canonique de $\mathbf{R}^n$ sur $T^n$ (identifié à $\mathbf{R}^n/\mathbf{Z}^n$), et $u$ une application linéaire de $\mathbf{R}^m$ dans $\mathbf{R}^n$.

Soit $f$ un homomorphisme continu de $\mathbf{R}^m$ dans $T^n$; nous allons montrer qu’il existe une application linéaire $u$ de $\mathbf{R}^m$ dans $\mathbf{R}^n$ telle que les homomorphismes $x \mapsto f(x)$ et $x \mapsto \varphi(u(x))$ coïncident en tous les points d’un voisinage de 0 dans $\mathbf{R}^m$; la proposition à démontrer en résultera, d’après VII, p. 12, cor. 1. Or, soit $V$ un voisinage de 0 dans $\mathbf{R}^n$ tel que $\varphi$, restreint à $V$, soit un isomorphisme local de $\mathbf{R}^n$ à $\mathbf{T}^n$; soit $\psi$ l’isomorphisme local réciproque défini dans $\varphi(V)$. Comme $f$ est continue, $V' = f^{-1}(\varphi(V))$ est un voisinage de 0 dans $\mathbf{R}^m$; l’application $x \mapsto \psi(f(x))$ restreinte à $V'$, est une application continue de $V'$ dans $\mathbf{R}^n$, telle que

$$
\psi(f(x + y)) = \psi(f(x)) + \psi(f(y))
$$

pour tout couple de points de $\mathbf{R}^m$ tels que $x \in V', \ y \in V', \ x + y \in V'$; donc (VII, p. 12, cor. 1), cette application coïncide avec un homomorphisme continu bien déterminé $u$ de $\mathbf{R}^m$ dans $\mathbf{R}^n$, en tous les points d’un voisinage $W$ de 0 dans $\mathbf{R}^m$; d’après la prop. 1 de VII, p. 11, $u$ est d’ailleurs une application linéaire de $\mathbf{R}^m$ dans $\mathbf{R}^n$; pour tout $x \in W$, on a donc $f(x) = \varphi(u(x))$, ce qui achève la démonstration.

#### Remarque {#top-vii-s2-n3-rem-1 .statement}

Le même raisonnement montre, plus généralement, que si $\varphi$ est un morphisme strict de $\mathbf{R}^n$ dans un groupe $G$, dont la restriction à un voisinage convenable de 0 est un isomorphisme local de $\mathbf{R}^n$ à $G$, tout homomorphisme continu de $\mathbf{R}^m$ dans $G$ est de la forme $x \mapsto \varphi(u(x))$, où $u$ est une application linéaire de $\mathbf{R}^m$ dans $\mathbf{R}^n$.

Dans le cas où $m = n = 1$, la prop. 3 donne la suivante:

#### Proposition 4 {#top-vii-s2-prop-4 .statement}

Si $\varphi$ est l’homomorphisme canonique de $\mathbf{R}$ sur $\mathbf{T}$, tout homomorphisme continu de $\mathbf{R}$ dans $\mathbf{T}$ est de la forme $x \mapsto \varphi(ax)$ où $a \in \mathbf{R}$; c’est un morphisme strict de $\mathbf{R}$ sur $\mathbf{T}$ si $a \neq 0$.

### 4. Automorphismes de $\mathbf{T}^n$

Soient $H$ un sous-groupe fermé de $\mathbf{R}^n$, $\varphi$ l’homomorphisme canonique de $\mathbf{R}^n$ sur le groupe quotient $\mathbf{R}^n/H$. Si $f$ est un homomorphisme continu de $\mathbf{R}^n/H$ dans un groupe topologique $G$, $\dot{f} = f \circ \varphi$ est un homomorphisme continu de $\mathbf{R}^n$ dans $G$, périodique, et ayant un groupe de périodes qui contient $H$; réciproquement, tout homomorphisme continu périodique de $\mathbf{R}^n$ dans $G$, dont le groupe de périodes contient $H$, est de cette forme.

Dans le cas où $H = \mathbf{Z}^n$, le groupe quotient $\mathbf{R}^n/\mathbf{Z}^n = \mathbf{T}^n$ est compact, donc tout homomorphisme continu $f$ de $\mathbf{T}^n$ dans un groupe topologique $G$ est un morphisme strict de $\mathbf{T}^n$ dans $G$ si $G$ est séparé (III, p. 16, Remarque 1), et $\dot{f} = f \circ \varphi$ est un morphisme strict de $\mathbf{R}^n$ dans $G$; en outre, $f(\mathbf{T}^n) = \dot{f}(\mathbf{R}^n)$ est un sous-groupe compact de $G$, isomorphe à un groupe $\mathbf{T}^p$ ($0 \leq p \leq n$).

On voit en particulier que le seul homomorphisme continu de $\mathbf{T}^n$ dans un groupe $\mathbf{R}^m$ est l’application identiquement nulle, puisque $\{0\}$ est le seul sous-groupe compact de $\mathbf{R}^m$.

Appliquons ce qui précède aux homomorphismes continus de $\mathbf{T}^n$ dans un groupe $\mathbf{T}^p$; si $f$ est un tel homomorphisme, $\varphi$ l’homomorphisme canonique de $\mathbf{R}^n$ sur $\mathbf{T}^n$, $f \circ \varphi$ est un homomorphisme continu de $\mathbf{R}^n$ dans $\mathbf{T}^p$; donc (VII, p. 13, prop. 3), si $\psi$ est l’homomorphisme canonique de $\mathbf{R}^p$ sur $\mathbf{T}^p$, il existe une application linéaire $u$ de $\mathbf{R}^n$ dans $\mathbf{R}^p$ telle que $f \circ \varphi = \psi \circ u$. Si $\mathbf{x} \in \mathbf{Z}^n$, $f(\varphi(\mathbf{x}))$ est l’élément neutre de $\mathbf{T}^p$, donc on a nécessairement $u(\mathbf{x}) \in \mathbf{Z}^p$, autrement dit, il faut que $u(\mathbf{Z}^n) \subset \mathbf{Z}^p$. Réciproquement, pour toute application linéaire $u$ de $\mathbf{R}^n$ dans $\mathbf{R}^p$ satisfaisant à cette condition, $\psi \circ u$ est un homomorphisme périodique continu de $\mathbf{R}^n$ dans $\mathbf{T}^p$, dont le groupe de périodes contient $\mathbf{Z}^n$; il définit donc un homomorphisme continu de $\mathbf{T}^n$ dans $\mathbf{T}^p$.

Cherchons à quelle condition $f$ est un *isomorphisme* de $\mathbf{T}^n$ sur un sous-groupe de $\mathbf{T}^p$. Il faut d’abord que $u$ soit une application *injective* de $\mathbf{R}^n$ dans $\mathbf{R}^p$; sinon, le sous-espace vectoriel $u(0)^{-1}$ contiendrait des points $\mathbf{x} \neq 0$ arbitrairement voisins de 0, et en un tel point on aurait $f(\varphi(\mathbf{x})) = f(\varphi(0))$ et $\varphi(\mathbf{x}) \neq \varphi(0)$, contrairement à l’hypothèse. Cette condition entraîne donc en premier lieu $p \geq n$. L’image $u(\mathbf{Z}^n)$ est alors un sous-groupe discret de rang $n$ du groupe $\mathbf{Z}^p$; les *facteurs invariants* de $u(\mathbf{Z}^n)$ par rapport à $\mathbf{Z}^p$ (VII, p. 2 et A, VII, § 4, n° 2) doivent tous être égaux à *un*; sinon, il existerait un point $\mathbf{x} \in \mathbf{Z}^n$ et un entier $k > 1$ tel que $u\left(\frac{1}{k} \mathbf{x}\right) \in \mathbf{Z}^n$, et $\frac{1}{k} \mathbf{x} \notin \mathbf{Z}^n$, donc $f\left(\varphi\left(\frac{1}{k} \mathbf{x}\right)\right) = f(\varphi(0))$, et $\varphi\left(\frac{1}{k} \mathbf{x}\right) \neq \varphi(0)$ contrairement à l’hypothèse. Réciproquement, si cette condition est remplie, $u(\mathbf{R}^n) \cap \mathbf{Z}^n$ est identique à $u(\mathbf{Z}^n)$, et $f$ est un isomorphisme de $\mathbf{T}^n$ sur $u(\mathbf{R}^n)/u(\mathbf{Z}^n)$.

Si l’on applique ce raisonnement au cas où $p = n$, on a la proposition suivante:

#### Proposition 5 {#top-vii-s2-prop-5 .statement}

*Tout isomorphisme du groupe topologique* $\mathbf{T}^n$ *sur un de ses sous-groupes est un automorphisme de* $\mathbf{T}^n$, *qui s’obtient par passage aux quotients à partir d’une application linéaire* $u$ *de* $\mathbf{R}^n$ *sur lui-même, qui, restreinte à* $\mathbf{Z}^n$, *est un automorphisme de ce groupe*.

Il revient au même de dire (VII, p. 2) que, si $u(\mathbf{e}_i) = \sum_{j=1}^n a_{ij} \mathbf{e}_j$, les $a_{ij}$ doivent être des *entiers* tels que le déterminant $\det(a_{ij})$, soit égal à $+1$, ou à $-1$, autrement dit on doit avoir $(a_{ij}) \in \mathbf{GL}(n, \mathbf{Z})$.

On peut aussi présenter ce résultat de la manière suivante: à chaque matrice $(a_{ij}) \in \mathbf{GL}(n, \mathbf{Z})$, associons l’automorphisme $(u_j) \mapsto \left( \sum_i a_{ij} u_i \right)$ de $\mathbf{T}^n$. L’application de $\mathbf{GL}(n, \mathbf{Z})$ dans le groupe des automorphismes du groupe topologique $\mathbf{T}^n$ ainsi définie est un isomorphisme.

En particulier, pour $n = 1$:

#### Proposition 6 {#top-vii-s2-prop-6 .statement}

*Les seuls isomorphismes du groupe topologique* $\mathbf{T}$ *sur un de ses sous-groupes sont l’application identique et la symétrie* $x \mapsto -x$.

## EXERCICES {#top-vii-s2-exercises}

See the [exercises for § 2](exercises/s2/).
