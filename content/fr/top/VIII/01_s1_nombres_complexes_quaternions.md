---
book: top
book_title: General Topology
chapter: VIII
chapter_title: NOMBRES COMPLEXES
section: 1
section_title: Nombres complexes; quaternions
lang: fr
source: top-v-x-fr
pdf_pages: 0087-0093, 0110-0111
extraction: ocr
subsections:
    - "no": 1
      title: Définition des nombres complexes
      page: 0
      pdf_page: 87
    - "no": 2
      title: Topologie de $\mathbf{C}$
      page: 3
      pdf_page: 89
    - "no": 3
      title: Le groupe multiplicatif $\mathbf{C}^*$
      page: 4
      pdf_page: 90
    - "no": 4
      title: Le corps des quaternions
      page: 4
      pdf_page: 90
statements: 13
exercises: 5
content_sha256: 7423e8afcdf0c3ecb02aebaa42b1b6a4f89c0fb5de51c49241b0acf5c00dec80
---

## § 1. NOMBRES COMPLEXES; QUATERNIONS

### 1. Définition des nombres complexes

Le polynôme $X^2 + 1$ n’a pas de racine dans $\mathbf{R}$, puisqu’on a $x^2 + 1 \geqslant 1$ quel que soit $x \in \mathbf{R}$; il est donc irréductible dans $\mathbf{R}$. C’est là d’ailleurs un cas particulier du résultat analogue qui s’applique à tout corps ordonné (A, VI, § 2).

#### Définition 1 {#top-viii-s1-def-1 .statement}

On appelle corps des nombres complexes, et on désigne par $\mathbf{C}$, le corps (commutatif) $\mathbf{R}[X]/(X^2 + 1)$; on désigne par $i$ l’image canonique de $X$ dans $\mathbf{C}$, de sorte que $\mathbf{C}$ est obtenu par adjonction algébrique au corps $\mathbf{R}$ de la racine $i$ du polynôme $X^2 + 1$; les éléments de $\mathbf{C}$ sont appelés nombres complexes.

Du point de vue algébrique, l’intérêt du corps $\mathbf{C}$ provient du théorème fondamental suivant:

#### Théorème 1 (théorème de d’Alembert-Gauss) {#top-viii-s1-thm-1 .statement}

Le corps $\mathbf{C}$ des nombres complexes est algébriquement clos.

Pour le démontrer, il suffit (A, VI, § 2, n° 6, th. 3) d’établir que: 1° tout élément $\geqslant 0$ a une racine carrée dans $\mathbf{R}$; 2° tout polynôme de degré impair à coefficients dans $\mathbf{R}$ possède au moins une racine dans $\mathbf{R}$. Nous avons déjà démontré la première de ces propositions (IV, p. 12). D’autre part, si $f(X) = a_0 X^n + a_1 X^1 + \cdots + a_n$ est un polynôme de degré $n$ impair ($a_0 \neq 0$) à coefficients réels, on peut écrire pour $x \neq 0$, $f(x) = a_0 x^n g(x)$, où $g(x) = 1 + a_1 / a_0 x + \cdots + a_n / a_0 x^n$ tend vers $+1$ lorsque $x$ tend vers $+\infty$ ou $-\infty$. Il existe donc un nombre $a > 0$ tel que $f(a)$ ait le signe de $a_0$ et $f(-a)$ le signe de $-a_0$; d’après le th. de Bolzano (IV, p. 28, th. 2), $f$ a au moins une racine dans $(-a, a)$.

#### Remarque 1 {#top-viii-s1-n1-rem-1 .statement}

On peut démontrer le th. I sans utiliser la théorie des corps ordonnés, en se servant des propriétés de la topologie du corps $\mathbf{C}$, qui va être définie ci-dessous (VIII, p. 3): voir VIII, p. 22, exerc. 2, et aussi la partie de ce Traité consacrée à la Topologie algébrique, où le théorème de d’Alembert-Gauss sera démontré comme conséquence de résultats sur le degré d’application.

#### Remarque 2 {#top-viii-s1-n1-rem-2 .statement}

Comme $\mathbf{C}$ est de degré 2 par rapport à $\mathbf{R}$, on voit que $\mathbf{C}$ est, à isomorphisme près, la seule extension algébrique de $\mathbf{R}$ distincte de $\mathbf{R}$, et qu’il n’existe pas de corps contenu dans $\mathbf{C}$ et contenant $\mathbf{R}$, distinct de $\mathbf{R}$ et de $\mathbf{C}$.

On sait (A, V, § 3) que $\mathbf{R}$ peut être identifié à un sous-corps de $\mathbf{C}$, et que tout élément $z \in \mathbf{C}$ peut se mettre d’une manière et d’une seule sous la forme $x + iy$, où $x$ et $y$ sont réels; $x$ est appelé partie réelle de $z$ et se note $\mathcal{R}(z)$, $y$ partie imaginaire de $z$ et se note $\mathcal{I}(z)$; les nombres complexes de la forme $iy$ ($y$ réels) sont dits imaginaires purs. La relation $x + iy = 0$ ($x$ et $y$ réels) est équivalente à « $x = 0$ et $y = 0$ ».

Comme $i^2 = -1$, les éléments de $\mathbf{C}$, donnés par leurs parties réelles et imaginaires, satisfont aux règles de calcul suivantes:

(1)
$$
(x + iy) + (x' + iy') = (x + x') + i(y + y'),
$$

(2)
$$
(x + iy)(x' + iy') = (xx' - yy') + i(xy' + yx').
$$

En particulier $(x + iy)(x - iy) = x^2 + y^2 \in \mathbf{R}$; d’où, si $x + iy \neq 0$,

(3)
$$
\frac{1}{x + iy} = \frac{x}{x^2 + y^2} - i \frac{y}{x^2 + y^2}.
$$

La seconde racine du polynôme $X^2 + 1$ dans $\mathbf{C}$ est $-i$; par suite (A, V, § 6, n° 2) le seul automorphisme de $\mathbf{C}$, distinct de l’application identique, et qui laisse invariants les nombres réels, est l’application faisant correspondre à tout nombre complexe $z = x + iy$ le nombre complexe $x - iy$, qu’on note $\overline{z}$, et qu’on appelle (conformément aux définitions générales) le nombre complexe conjugué de $z$. On a $\mathcal{R}(z) = \frac{1}{2}(z + \overline{z})$, $\mathcal{I}(z) = \frac{1}{2i}(z - \overline{z})$. En vertu de cet automorphisme, si $f(z)$ est un polynôme à coefficients réels, on a $f(\overline{z}) = \overline{f(z)}$ pour tout $z \in \mathbf{C}$.

Le nombre réel $z \overline{z} = x^2 + y^2$ s’appelle la norme algébrique de $z$ (ou simplement la norme de $z$ lorsque aucune confusion n’est possible); c’est un nombre $\geqslant 0$, qui n’est nul que si $z = 0$. Le nombre positif $\sqrt{z \overline{z}} = \sqrt{x^2 + y^2}$ se réduit à la valeur absolue de $z$ lorsque $z$ est réel; on l’appelle encore valeur absolue de $z$ et on le note $|z|$ lorsque $z$ est un nombre complexe quelconque (cf. A, VI, § 2, n° 6). La relation $|z| = 0$ équivaut à $z = 0$. Si $z$ et $z'$ sont deux nombres complexes, le conjugué de $zz'$ est $\overline{z}.\overline{z}'$, donc $|zz'|^2 = zz'\overline{z}\overline{z}' = |z|^2|z'|^2$, d’où $|zz'| = |z|.|z'|$: la valeur absolue d’un produit est le produit des valeurs absolues des facteurs. En particulier, si $z \neq 0$ et $z' = 1/z$, on a $|1/z| = 1/|z|$.

Enfin, quels que soient les nombres complexes $z, z'$, on a l’inégalité du triangle:

(4)
$$
|z + z'| \leqslant |z| + |z'|.
$$

### 2. Topologie de $\mathbf{C}$

L’application $(x, y) \mapsto x + iy$ du plan numérique $\mathbf{R}^2$ sur $\mathbf{C}$ est *bijective*; au moyen de cette application, on peut *transporter* à $\mathbf{C}$ la topologie de $\mathbf{R}^2$ (cf. VI, p. 1). La topologie ainsi définie sur $\mathbf{C}$ est *compatible* avec la structure de corps de $\mathbf{C}$ (III, p. 54), car elle est compatible avec sa structure d’anneau (VI, p. 6) et, d’après (3), $1/z$ est continue dans le complémentaire $\mathbf{C}^*$ du point 0 dans $\mathbf{C}$.

En munissant l’ensemble $\mathbf{C}$ de cette topologie et de la structure de corps définie plus haut (VIII, p. 1), on définit donc sur $\mathbf{C}$ une structure de *corps topologique* (III, p. 54); quand nous parlerons de la topologie de $\mathbf{C}$, c’est toujours de la topologie précédente qu’il sera question.

Dans la suite, on *identifiera* le plus souvent les ensembles $\mathbf{C}$ et $\mathbf{R}^2$, considérés comme espaces topologiques; le sous-corps $\mathbf{R}$ de $\mathbf{C}$ se trouve alors identifié avec l’axe des abscisses de $\mathbf{R}^2$, qu’on appelle pour cette raison *axe réel*; on appelle de même *axe imaginaire* l’axe des ordonnées de $\mathbf{R}^2$ (on notera que ce n’est pas un sous-corps de $\mathbf{C}$). La demi-droite de paramètres $(1, 0)$ (identifiée à $\mathbf{R}_+$) est dite *demi-axe réel positif*; la demi-droite opposée, de paramètres $(-1, 0)$, *demi-axe réel négatif*.

Pour illustrer par des figures ce qui sera dit de $\mathbf{C}$ ou de $\mathbf{R}^2$, on utilisera la représentation (bien connue en géométrie élémentaire) de $\mathbf{R}^2$ par les points d’un plan où l’on a tracé deux axes de coordonnées rectangulaires, qui représentent respectivement l’axe réel et l’axe imaginaire de $\mathbf{C}$ (fig. 7).

![Figure 7](https://i.imgur.com/3Q5z5QG.png)

Figure 7

Comme dans tout corps topologique, toute *fonction rationnelle* de $n$ variables complexes, à coefficients complexes, est *continue* en tout point de $\mathbf{C}^n$ où son dénominateur n’est pas nul.

La permutation $z \mapsto \overline{z}$ de $\mathbf{C}$ est *continue*; c’est donc un *automorphisme* du corps topologique $\mathbf{C}$.

On peut d’ailleurs montrer que c’est le *seul* automorphisme du corps topologique $\mathbf{C}$, distinct de l’automorphisme identique (voir VIII, p. 25, exerc. 4).

Les fonctions $\Re(z), \mathcal{I}(z)$ ne sont autres que les fonctions *projections* dans $\mathbf{R}^2$; elles sont donc *continues*; il en est de même de la valeur absolue $|z|$, qui n’est autre que la *norme euclidienne* (VI, p. 7) du point $(x, y)$ dans $\mathbf{R}^2$.

Les propriétés de la valeur absolue permettent de donner une autre démonstration du fait que la topologie de $\mathbf{C}$ est compatible avec la structure de corps de $\mathbf{C}$.

(cf. IX, p. 28). En effet, la continuité de $z + z'$ résulte de l’inégalité du triangle
$$
|z + z'| \leq |z| + |z'|;
$$
la continuité de $zz'$ résulte de la relation
$$
|zz' - z_0 z'_0| = |z_0(z' - z'_0) + (z - z_0)z'_0 + (z - z_0)(z' - z'_0)| \\
\leq |z_0| \cdot |z' - z'_0| + |z'_0| \cdot |z - z_0| + |z - z_0| \cdot |z' - z'_0|.
$$
Enfin, la continuité de $z^{-1}$ résulte de la relation
$$
|z_0^{-1} - z^{-1}| = |z|^{-1} \cdot |z - z_0| \cdot |z_0|^{-1}.
$$

### 3. Le groupe multiplicatif $\mathbf{C}^*$

On sait (III, p. 55) que la topologie induite sur le groupe multiplicatif $\mathbf{C}^*$ des nombres complexes $\neq 0$ est compatible avec la structure de groupe de $\mathbf{C}^*$; comme $\mathbf{C}^*$ est ouvert dans $\mathbf{C}$, $\mathbf{C}^*$ est un groupe topologique *localement compact* (I, p. 66, prop. 13), donc *complet* (pour la structure uniforme multiplicative, bien entendu; cf. III, p. 56, prop. 8). Le groupe multiplicatif $\mathbf{R}_+^*$ des nombres réels $> 0$ est un *sous-groupe fermé* de $\mathbf{C}^*$. Un autre sous-groupe est formé de l’ensemble $\mathbf{U}$ des nombres complexes *de valeur absolue égale à* 1, qui est identifié avec le *cercle unité* $\mathbf{S}_1$ de $\mathbf{R}^2$, et est par suite un groupe *compact*. En outre:

#### Proposition 1 {#top-viii-s1-prop-1 .statement}

*Le groupe topologique* $\mathbf{C}^*$ *est le produit direct de ses sous-groupes* $\mathbf{R}_+^*$ *et* $\mathbf{U}$.

En effet, l’application $(t, u) \mapsto tu$ est un *homéomorphisme* de $\mathbf{R}_+^* \times \mathbf{U}$ sur $\mathbf{C}^*$ (VI, p. 10, prop. 3); il est immédiat d’autre part que c’est un isomorphisme du groupe produit $\mathbf{R}_+^* \times \mathbf{U}$ sur $\mathbf{C}^*$.

Nous savons que le groupe topologique $\mathbf{R}_+^*$ est isomorphe au groupe additif $\mathbf{R}$ (V, p. 11, th. 1); l’étude du groupe topologique $\mathbf{C}^*$ est donc ramenée à celle du groupe $\mathbf{U}$, que nous ferons au § 2.

### 4. Le corps des quaternions

On note $\mathbf{H}$ l’*algèbre des quaternions de Hamilton*, c’est-à-dire (A, III, p. 19) la $\mathbf{R}$-algèbre dont l’espace vectoriel sous-jacent est $\mathbf{R}^4$ et dont la table de multiplication de la base canonique (notée $(1, i, j, k)$), est donnée par les formules suivantes:
$$
\begin{align*}
1^2 &= 1, & 1i &= i1 = i, & 1j &= j1 = j, & 1k &= k1 = k, \\
i^2 &= j^2 = k^2 = -1, & ij &= -ji = k, & jk &= -kj = i, & ki &= -ik = j.
\end{align*}
$$
On identifie $\mathbf{R}$ au sous-corps $\mathbf{R}1$ de $\mathbf{H}$ et $\mathbf{C}$ au sous-corps de $\mathbf{H}$ formé des quaternions de la forme $a + bi$, pour $a, b$ dans $\mathbf{R}$. Tout quaternion $x \in \mathbf{H}$ s’écrit $x = x_0 + x_1 i + x_2 j + x_3 k = z_0 + z_1 j = z_0 + j \overline{z}_1$, avec $x_0, x_1, x_2, x_3$ dans $\mathbf{R}$, et $z_0, z_1$ dans $\mathbf{C}$; on pose
$$
\begin{align*}
\overline{x} &= x_0 - x_1 i - x_2 j - x_3 k = \overline{z}_0 - z_1 j, \\
T(x) &= x + \overline{x} = 2x_0 = z_0 + \overline{z}_0, \\
N(x) &= x \cdot \overline{x} = x_0^2 + x_1^2 + x_2^2 + x_3^2 = z_0 \overline{z}_0 + z_1 \overline{z}_1.
\end{align*}
$$

On dit que $N(\mathbf{x})$ est la norme (algébrique) de $\mathbf{x}$; c’est le carré de sa norme euclidienne $|\mathbf{x}|$ dans $\mathbf{R}^4$; on a $N(xy) = N(x)N(y)$. Il résulte de ce qui précède que $\mathbf{H}$ est un corps (non commutatif), l’inverse du quaternion non nul $\mathbf{x}$ étant $\overline{\mathbf{x}}/N(\mathbf{x})$. Le centre de $\mathbf{H}$ est $\mathbf{R}$, et il résulte de A, VIII, § 11, th. 2 que toute $\mathbf{R}$-algèbre de rang fini qui est un corps non commutatif est isomorphe à $\mathbf{H}$.

La topologie de $\mathbf{H} = \mathbf{R}^4$ est compatible avec sa structure de corps; elle est en effet compatible avec sa structure d’anneau d’après VI, p. 6, et les coordonnées de l’inverse $\mathbf{x}^{-1}$ d’un quaternion non nul $\mathbf{x}$ sont des fonctions rationnelles; donc continues, des coordonnées de $\mathbf{x}$.

Nous obtenons ainsi un troisième exemple de corps topologique localement compact et connexe, les deux autres étant $\mathbf{R}$ et $\mathbf{C}$; on peut montrer que ce sont, à isomorphisme près, les seuls corps topologiques ayant ces deux propriétés (AC, VI, § 9, n° 3, cor. du th. 1).

L’ensemble des quaternions de norme 1, identique à la sphère $\mathbf{S}_3$, est un sous-groupe compact du groupe multiplicatif $\mathbf{H}^*$ des quaternions non nuls.

#### Proposition 2 {#top-viii-s1-prop-2 .statement}

*Le groupe topologique $\mathbf{H}^*$ des quaternions $\neq 0$ est le produit direct de ses sous-groupes $\mathbf{R}_+^*$ et $\mathbf{S}_3$.*

En effet, l’application $(t, \mathbf{z}) \mapsto t\mathbf{z}$ de $\mathbf{R}_+^* \times \mathbf{S}_3$ dans $\mathbf{H}^*$ est un homéomorphisme d’après VI, p. 10, et c’est un homomorphisme de groupes.

Si $\mathbf{x} = z_0 + z_1 j \in \mathbf{H}$, avec $z_0, z_1$ dans $\mathbf{C}$, on a $N(\mathbf{x}) = z_0 \overline{z}_0 + z_1 \overline{z}_1$. Il s’ensuit que $N$ est une forme hermitienne positive non dégénérée sur le $\mathbf{C}$-espace vectoriel $\mathbf{H}$ (A, IX, §7, n° 1); notons $\mathbf{SU}(N)$ le groupe spécial unitaire correspondant. Si on identifie $\mathbf{H}$ à $\mathbf{C}^2$ à l’aide de la base $(1, j)$, le groupe $\mathbf{SU}(N)$ s’identifie alors au groupe $\mathbf{SU}(2, \mathbf{C})$.

#### Proposition 3 {#top-viii-s1-prop-3 .statement}

*L’application qui associe à chaque $\mathbf{q} \in \mathbf{S}_3$ l’endomorphisme*
$$
\mathbf{x} \mapsto \mathbf{xq}^{-1} = \mathbf{x}\overline{\mathbf{q}}
$$
*du $\mathbf{C}$-espace vectoriel $\mathbf{H}$ est un isomorphisme du groupe $\mathbf{S}_3$ sur le groupe spécial unitaire $\mathbf{SU}(N)$.*

Soit $\mathbf{q} \in \mathbf{S}_3$; posons $a_q(\mathbf{x}) = \mathbf{xq}^{-1}$ pour $\mathbf{x} \in \mathbf{H}$. Comme $N(a_q(\mathbf{x})) = N(\mathbf{x})$ pour $\mathbf{x} \in \mathbf{H}$, l’endomorphisme $a_q$ appartient au groupe unitaire $\mathbf{U}(N)$. D’autre part, d’après A, III, p. 111, ex. 2, le déterminant de $a_q$ est égal à 1, de sorte que $\mathbf{q} \mapsto a_q$ est un homomorphisme de groupes de $\mathbf{S}_3$ dans $\mathbf{SU}(N)$. Celui-ci est injectif, puisque $\mathbf{q} = a_q(1)^{-1}$. Soit enfin $u \in \mathbf{SU}(N)$; posons $\mathbf{q} = u(1)$. On a
$$
N(\mathbf{q}) = N(u(1)) = N(1) = 1,
$$
donc $\mathbf{q} \in \mathbf{S}_3$; posons $v = a_q^{-1} \circ u$. On a $v \in \mathbf{SU}(N)$ et $v(1) = 1$. Il s’ensuit que $v$ laisse stable l’orthogonal $\mathbf{C}j$ de 1 pour la forme $N$, donc que l’on a $v(j) = zj$ avec $z \in \mathbf{C}$; mais cela implique $z = \det(v) = 1$, soit $v = 1$, c’est-à-dire $u = a_q$.

Soit $\mathbf{H}_0$ le sous-$\mathbf{R}$-espace vectoriel de $\mathbf{H}$ formé des quaternions $\mathbf{x}$ *purs*, c’est-à-dire tels que $T(\mathbf{x}) = 0$. Notons $N_0$ la restriction à $\mathbf{H}_0$ de la forme quadratique $N$ et $\mathbf{SO}(N_0)$ le groupe spécial orthogonal correspondant (A, IX, §6, n° 2). Si on identifie $\mathbf{H}_0$ à $\mathbf{R}^3$ à l’aide de la base $(i, j, k)$, le groupe $\mathbf{SO}(N_0)$ s’identifie au groupe spécial orthogonal $\mathbf{SO}(3, \mathbf{R})$ de la forme quadratique

$$
(x_1, x_2, x_3) \mapsto x_1^2 + x_2^2 + x_3^2.
$$

Soit $q \in \mathbf{H}^*$ et $x \in \mathbf{H}$; d’après A, III, p. 16, formule (17), on a $T(qxq^{-1}) = T(x)$, de sorte que $qxq^{-1}$ est pur lorsque $x$ l’est.

#### Proposition 4 {#top-viii-s1-prop-4 .statement}

*L’application qui associe à chaque $q \in S_3$ l’endomorphisme $x \mapsto qxq^{-1} = q x \bar{q}$ de l’espace $\mathbf{H}_0$ des quaternions purs est un homomorphisme surjectif du groupe $S_3$ sur le groupe spécial orthogonal $\mathbf{SO}(N_0)$; son noyau est formé des quaternions $1$ et $-1$.*

Soit $q \in S_3$; posons $b_q(x) = qxq^{-1}$ pour $x \in \mathbf{H}_0$. Comme $N(b_q(x)) = N(x)$ pour $x \in \mathbf{H}_0$, l’endomorphisme $b_q$ de $\mathbf{H}_0$ appartient au groupe orthogonal $\mathbf{O}(N)$. D’autre part, l’espace vectoriel $\mathbf{H}$ est somme directe de $\mathbf{R}$ et de $\mathbf{H}_0$, et l’endomorphisme $x \mapsto qxq^{-1}$ de $\mathbf{H}$ est somme directe de $b_q$ et de l’automorphisme identique de $\mathbf{R}$; d’après A, III, p. 111, ex. 2, le déterminant de $b_q$ est donc égal à 1, et $q \mapsto b_q$ est un homomorphisme du groupe $S_3$ dans le groupe spécial orthogonal $\mathbf{SO}(N_0)$. Le noyau $K$ de cet homomorphisme est formé des éléments de $S_3$ qui commutent à tous les éléments de $\mathbf{H}_0$, donc qui appartiennent au centre de $\mathbf{H}$; comme ce centre est égal à $\mathbf{R}$, on a $K = S_3 \cap \mathbf{R} = \{-1, 1\}$.

Il nous reste à prouver que tout élément $u$ de $\mathbf{SO}(N_0)$ est de la forme $b_q$ pour un élément convenable $q$ de $S_3$. *Supposons d’abord que l’on ait $u(i) = i$.* Alors $u$ laisse stable l’orthogonal $Rj + Rk = Cj$ de $i$ et induit sur cet espace un élément $u$ du groupe spécial orthogonal de la forme induite par $N_0$, c’est-à-dire de la forme $zj \mapsto |z|^2$; il existe donc un élément $a \in U$ tel que $\bar{u}(zj) = azj$. Soit $q \in U$ tel que $q^2 = a$; on a

$$
b_q(zj) = qzjq^{-1} = qzj\bar{q} = qzqj = azj = \bar{u}(zj);
$$

comme $b_q(i) = i$, cela implique $u = b_q$. *Traitons maintenant le cas général.* On a $u(i)^2 = -1$, et $i$ et $u(i)$ engendrent deux sous-corps isomorphes de $\mathbf{H}$. D’après le théorème de Skolem-Noether (A, VIII, §10, n° 1, th. 1), il existe $q \in \mathbf{H}^*$ tel que $u(i) = qi\bar{q}^{-1}$; remplaçant $q$ par $q/|q|$, on peut supposer $q \in S_3$. D’après ce qui précède, il existe $q' \in S_3$ tel que $b_{q'}^{-1} \circ u = b_{q'}$, donc $u = b_{qq'}$, ce qui achève la démonstration.

#### Corollaire {#top-viii-s1-n4-cor-1 .statement}

*L’application qui associe à chaque $(q, q') \in S_3 \times S_3$ l’endomorphisme $x \mapsto qx{q'}^{-1} = qx\bar{q}'$ du $\mathbf{R}$-espace vectoriel $\mathbf{H}$ est un homomorphisme surjectif du groupe produit $S_3 \times S_3$ sur le groupe spécial orthogonal $\mathbf{SO}(4, \mathbf{R})$ de la forme quadratique $N$; son noyau est formé des couples $(1, 1)$ et $(-1, -1)$.*

Soit $(q, q') \in S_3 \times S_3$; posons $c_{q,q'}(x) = qx{q'}^{-1}$ pour $x \in \mathbf{H}$. On voit comme ci-dessus que $(q, q') \mapsto c_{q,q'}$ est un homomorphisme du groupe produit $S_3 \times S_3$ dans le groupe spécial orthogonal $\mathbf{SO}(N)$. Si $c_{q,q'} = 1$, on a en particulier $c_{q,q'}(1) = 1$, donc $q = q'$, et la restriction de $c_{q,q'}$ à $\mathbf{H}_0$ est l’endomorphisme $b_q$; on a $b_q = 1$, donc $q = 1$ ou $q = -1$. Il reste à prouver que tout élément $u$ de $\mathbf{SO}(N)$ est de la forme $c_{q,q'}$. Supposons d’abord que $u(1) = 1$; alors $u$ laisse stable l’orthogonal $\mathbf{H}_0$ de 1 et induit sur $\mathbf{H}_0$ un élément de $\mathbf{SO}(N_0)$; d’après la proposition 4, il existe donc $q \in S_3$ tel que $u = c_{q,q}$. Dans le cas général, posons $v = c_{1,u(1)^{-1}} \circ u$; on a $v(1) = 1$; il existe donc $q \in S_3$ tel que $v = c_{q,q}$, et on a $u = c_{q,u(1)q}$.

#### Remarque 1 {#top-viii-s1-n4-rem-1 .statement}

A l’aide des relations $\| x + y \| \leq \| x \| + \| y \|$ et $\| xy \| = \| x \| . \| y \|$, on peut démontrer directement, comme plus haut pour le corps des nombres complexes, que la topologie de $\mathbf{R}^4$ est compatible avec la structure de corps de $\mathbf{H}$ (cf. IX, p. 28).

#### Remarque 2 {#top-viii-s1-n4-rem-2 .statement}

Sur les sphères $S_0, S_1$ et $S_3$, il existe, d’après ce qui précède, une structure de groupe compatible avec leur topologie. Inversement, on peut montrer que tout groupe topologique homéomorphe à une sphère $S_n$ est isomorphe à l’un des groupes topologiques $S_0, S_1$ ou $S_3$.

#### Remarque 3 {#top-viii-s1-n4-rem-3 .statement}

Tout point du groupe $S_3$ possède un voisinage homéomorphe à $\mathbf{R}^3$ (VI, p. 11, cor. 2), mais $S_3$ n’est pas localement isomorphe au groupe $\mathbf{R}^3$, sans quoi, étant connexe, il serait commutatif (VII, p. 13, th. 1), ce qui n’est pas le cas puisque $i$ et $j$ appartiennent à $S_3$ et que $ij \neq ji$.

#### Remarque 4 {#top-viii-s1-n4-rem-4 .statement}

Si l’on munit les groupes $\mathbf{SU}(N), \mathbf{SO}(N_0)$ et $\mathbf{SO}(N)$ des topologies induites par celle du groupe linéaire $\mathbf{GL}(4, \mathbf{R})$, et les groupes
$$
S_3/\{1, -1\} \quad \text{et} \quad (S_3 \times S_3)/\{(1, 1), (-1, -1)\}
$$
des topologies quotients, les isomorphismes de groupes
$$
\begin{align*}
S_3 &\to \mathbf{SU}(N), \\
S_3/\{1, -1\} &\to \mathbf{SO}(N_0), \\
(S_3 \times S_3)/\{(1, 1), (-1, -1)\} &\to \mathbf{SO}(N)
\end{align*}
$$
définis ci-dessus sont continus. Comme ils sont définis sur des espaces compacts et à valeurs dans des espaces séparés, ce sont des homéomorphismes, donc des isomorphismes de groupes topologiques.

## EXERCICES {#top-viii-s1-exercises}

See the [exercises for § 1](exercises/s1/).
