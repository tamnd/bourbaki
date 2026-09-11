---
book: top
book_title: General Topology
chapter: VI
chapter_title: ESPACES NUMÉRIQUES ET ESPACES PROJECTIFS
section: 2
section_title: Distance euclidienne ; boules et sphères
lang: fr
source: top-v-x-fr
book_pages: TG VI.7-TG VI.12, TG VI.23-TG VI.25
pdf_pages: 0035-0040, 0051-0053
extraction: ocr
subsections:
    - "no": 1
      title: Distance euclidienne dans $\mathbf{R}^n$
      page: 7
      pdf_page: 35
    - "no": 2
      title: Déplacements
      page: 8
      pdf_page: 36
    - "no": 3
      title: Boules et sphères euclidiennes
      page: 8
      pdf_page: 36
    - "no": 4
      title: Projection stéréographique
      page: 11
      pdf_page: 39
statements: 13
exercises: 14
content_sha256: ea12c7bf4654b75d8e680909f96842a8bbfba287bf97157b890d942ed1870162
---

## § 2. DISTANCE EUCLIDIENNE; BOULES ET SPHÈRES

### 1. Distance euclidienne dans $\mathbf{R}^n$

On appelle *distance euclidienne* de deux points $\mathbf{x} = (x_i), \mathbf{y} = (y_i)$ de $\mathbf{R}^n$ le nombre
$$
d(\mathbf{x}, \mathbf{y}) = \sqrt{\sum_{i=1}^n (x_i - y_i)^2} \geq 0;
$$
rappelons-en les principales propriétés (A, IX, §7, n° 1). La relation $d(\mathbf{x}, \mathbf{y}) = 0$ équivaut à $\mathbf{x} = \mathbf{y}$. On a $d(\mathbf{y}, \mathbf{x}) = d(\mathbf{x}, \mathbf{y})$; pour tout scalaire $t \in \mathbf{R}$, $d(t\mathbf{x}, t\mathbf{y}) = |t| d(\mathbf{x}, \mathbf{y})$; quel que soit $\mathbf{z} \in \mathbf{R}^n$,
$$
d(\mathbf{x} + \mathbf{z}, \mathbf{y} + \mathbf{z}) = d(\mathbf{x}, \mathbf{y}),
$$
autrement dit, la distance de deux points est *invariante par translation*. La distance $d(0, \mathbf{x})$ de l’origine 0 à un point $\mathbf{x}$ se note encore $||\mathbf{x}||$ et s’appelle *norme euclidienne* de $\mathbf{x}$ (ou simplement *norme* de $\mathbf{x}$, quand aucune confusion n’en résulte; cf. IX, p. 31); on a $d(\mathbf{x}, \mathbf{y}) = ||\mathbf{y} - \mathbf{x}||$.

Pour $n = 1$, la distance euclidienne des points $x, y$ de $\mathbf{R}$ se réduit à la longueur $|y - x|$ des intervalles d’extrémités $x, y$; pour $n$ quelconque, on dit encore que $d(\mathbf{x}, \mathbf{y}) = ||y - x||$ est la *longueur* des segments d’extrémités $\mathbf{x}, \mathbf{y}$.

La distance euclidienne satisfait à l’inégalité, dite *inégalité du triangle*,
$$
d(\mathbf{x}, \mathbf{y}) \leq d(\mathbf{x}, \mathbf{z}) + d(\mathbf{z}, \mathbf{y})
$$
quels que soient $\mathbf{x}, \mathbf{y}, \mathbf{z}$ dans $\mathbf{R}^n$.

La démonstration de la relation (1) se ramène à celle de l’inégalité
$$
\left( \sum_{i=1}^n (x_i + y_i)^2 \right)^{1/2} \leq \left( \sum_{i=1}^n x_i^2 \right)^{1/2} + \left( \sum_{i=1}^n y_i^2 \right)^{1/2};
$$
cette dernière est équivalente à l’inégalité de Cauchy-Schwarz
$$
\left( \sum_{i=1}^n x_i y_i \right)^2 \leq \left( \sum_{i=1}^n x_i^2 \right) \left( \sum_{i=1}^n y_i^2 \right),
$$
et cette inégalité est elle-même conséquence immédiate de l’identité de Lagrange
$$
\left( \sum_{i=1}^n x_i^2 \right) \left( \sum_{i=1}^n y_i^2 \right) - \left( \sum_{i=1}^n x_i y_i \right)^2 = \frac{1}{2} \sum_{i,j} (x_i y_j - x_j y_i)^2.
$$
Cette démonstration montre en même temps que les deux membres de (1) ne peuvent être égaux que si $\mathbf{z}$ est un point du segment d’extrémités $\mathbf{x}, \mathbf{y}$.

De (1) on déduit l’inégalité

(2)
$$
d(\mathbf{x}, \mathbf{y}) \geq |d(\mathbf{x}, \mathbf{z}) - d(\mathbf{y}, \mathbf{z})|.
$$

Enfin si $\mathbf{x} = (x_i), \mathbf{y} = (y_i)$, on a
(3)
$$
\sup_{1 \leq i \leq n} |x_i - y_i| \leq d(\mathbf{x}, \mathbf{y}) \leq \sqrt{n} \cdot \sup_{1 \leq i \leq n} |x_i - y_i|.
$$

On en conclut que, pour qu’une partie A de $\mathbf{R}^n$ soit bornée (VI, p. 2), il faut et il suffit que $\sup_{\mathbf{x} \in A} \| \mathbf{x} \| < +\infty$.

### 2. Déplacements

Rappelons encore (A, IX, § 6, no 6) que les transformations affines $f$ de $\mathbf{R}^n$ sur lui-même qui laissent invariant la distance de deux points quelconques (c’est-à-dire telles que $d(f(\mathbf{x}), f(\mathbf{y})) = d(\mathbf{x}, \mathbf{y})$ quels que soient $\mathbf{x}$ et $\mathbf{y}$) sont appelées déplacements euclidiens (ou simplement déplacements)[^1]; elles forment un groupe, dit groupe des déplacements de $\mathbf{R}^n$. Ce groupe opère transitiivement dans $\mathbf{R}^n$; plus généralement, si V et V’ sont deux variétés linéaires affines de $\mathbf{R}^n$ de même dimension, il existe toujours un déplacement transformant V en V’. Les déplacements laissant invariant l’origine, appelés transformations orthogonales, forment un sous-groupe du groupe des déplacements, dit groupe orthogonal à $n$ variables réelles (A, IX, § 6, no 2); les applications linéaires qui forment ce groupe sont caractérisées par la propriété de laisser invariant la norme $\| \mathbf{x} \|$ de tout point $\mathbf{x} \in \mathbf{R}^n$, ou, ce qui revient au même, la forme quadratique $\| \mathbf{x} \|^2 = \sum_{i=1}^n x_i^2$. On appelle produit scalaire de deux vecteurs $\mathbf{x} = (x_i)$ et $\mathbf{y} = (y_i)$ de $\mathbf{R}^n$, la valeur $\sum_{i=1}^n x_i y_i$ de la forme bilinéaire associée (A, IX, § 3, no 4) à la forme quadratique $\frac{1}{2} \sum_{i=1}^n x_i^2$; on le note $(\mathbf{x} \mid \mathbf{y})$, ou simplement $\mathbf{x} \mathbf{y}$ lorsque aucune confusion n’est à craindre; toute transformation orthogonale laisse invariant le produit scalaire. Deux vecteurs $\mathbf{x}, \mathbf{y}$ sont dits orthogonaux si $(\mathbf{x} \mid \mathbf{y}) = 0$; deux sous-espaces vectoriels V, V’ de $\mathbf{R}^n$ sont dits orthogonaux si tout $\mathbf{x} \in V$ est orthogonal à tout $\mathbf{y} \in V'$; deux variétés linéaires affines P, P’ sont dites orthogonales si les sous-espaces vectoriels respectivement parallèles à P et P’ sont orthogonaux.

### 3. Boules et sphères euclidiennes

Pour tout entier $p > 0$, désignons par $U_p$ l’ensemble des couples $(\mathbf{x}, \mathbf{y})$ de points de $\mathbf{R}^n$ tels que $d(\mathbf{x}, \mathbf{y}) < 1/p$; les inégalités (3) (VI, p. 8) montrent que les ensembles $U_p$ forment un système fondamental d’entourages de la structure uniforme de $\mathbf{R}^n$ (cf. IX, p. 12).

De ce fait, et de l’inégalité
$$
|d(\mathbf{x}, \mathbf{y}) - d(\mathbf{x}', \mathbf{y}')| \leq d(\mathbf{x}, \mathbf{x}') + d(\mathbf{y}, \mathbf{y}'),
$$
qui est une conséquence de (1) (VI, p. 7), on conclut que $d(\mathbf{x}, \mathbf{y})$ est uniformément continue dans $\mathbf{R}^n \times \mathbf{R}^n$; la norme $\| \mathbf{x} \| = d(0, \mathbf{x})$ est par suite uniformément continue dans $\mathbf{R}^n$.

#### Définition 1 {#top-vi-s2-def-1 .statement}

Étant donnés un point $\mathbf{x}_0 \in \mathbf{R}^n$, et un nombre $r > 0$, on appelle boule euclidienne ouverte (resp. fermée) à n dimensions de centre $\mathbf{x}_0$ et de rayon $r$, l’ensemble des points $\mathbf{x} \in \mathbf{R}^n$ tels que $d(\mathbf{x}_0, \mathbf{x}) < r$ (resp. $d(\mathbf{x}_0, \mathbf{x}) \leq r$); on appelle sphère euclidienne à $n - 1$ dimensions, de centre $\mathbf{x}_0$ et de rayon $r$, l’ensemble des points $\mathbf{x}$ tels que $d(\mathbf{x}_0, \mathbf{x}) = r$.

Lorsque aucune confusion n’est à craindre, on dit simplement « boule » (resp. « sphère ») pour « boule euclidienne » (resp. « sphère euclidienne »). Pour $n = 2$, on dit « disque » au lieu de « boule à 2 dimensions », et « cercle » au lieu de « sphère à 1 dimension ».

Pour $n = 1$, la boule ouverte (resp. fermée) de centre $x_0$ et de rayon $r$ est l’intervalle $]x_0 - r, x_0 + r[$ (resp. $[x_0 - r, x_0 + r]$); la sphère de centre $x_0$ et de rayon $r$ est l’ensemble des deux extrémités $x_0 - r, x_0 + r$ de ces intervalles. Pour $n = 0$, toute boule est réduite à 0, et toute sphère est vide.

D’après ce qui précède, les boules (ouvertes ou fermées) de centre $\mathbf{x}_0$ (ou seulement celles de rayon $1/p$, où $p$ parcourt l’ensemble des entiers $> 0$) forment un système fondamental de voisinages du point $\mathbf{x}_0$.

#### Proposition 1 {#top-vi-s2-prop-1 .statement}

Toute boule ouverte (resp. fermée) de $\mathbf{R}^n$ est un ensemble ouvert (resp. compact). L’adhérence d’une boule ouverte est la boule fermée de même centre et de même rayon ; l’intérieur d’une boule fermée est la boule ouverte de même centre et de même rayon.

La boule ouverte (resp. fermée) de centre $\mathbf{x}_0$ et de rayon $r$ est l’image réciproque de l’intervalle $]-\infty, r[$ (resp. $]-\infty, r]$) par la fonction continue $d(\mathbf{x}_0, \mathbf{x})$; c’est donc un ensemble ouvert (resp. fermé et borné, donc compact). Si $d(\mathbf{x}_0, \mathbf{x}) = r$, et si $\mathbf{y} = \mathbf{x}_0 + t(\mathbf{x} - \mathbf{x}_0)$ ($0 < t < 1$) est un point du segment ouvert d’extrémités $\mathbf{x}_0$ et $\mathbf{x}$, on a $d(\mathbf{x}_0, \mathbf{y}) = tr < r$, et $d(\mathbf{x}, \mathbf{y}) = (1 - t)r$ est aussi petit qu’on veut; donc $\mathbf{x}$ est adhérent à la boule ouverte de centre $\mathbf{x}_0$ et de rayon $r$. De même, si $\mathbf{z} = \mathbf{x} + t(\mathbf{x} - \mathbf{x}_0)$ ($t > 0$) est un point de la demi-droite ouverte d’origine $\mathbf{x}$ et de vecteur directeur $\mathbf{x} - \mathbf{x}_0$, on a
$$
d(\mathbf{x}_0, \mathbf{z}) = (1 + t)r > r,
$$
et $d(\mathbf{x}, \mathbf{z}) = tr$ est aussi petit qu’on veut; donc $\mathbf{x}$ n’est pas intérieur à la boule fermée de centre $\mathbf{x}_0$ et de rayon $r$.

#### Corollaire {#top-vi-s2-n3-cor-1 .statement}

Toute sphère euclidienne est un ensemble compact, frontière de la boule ouverte et de la boule fermée de même centre et de même rayon.

L’homéomorphisme affine $\mathbf{x} \mapsto (1/r)(\mathbf{x} - \mathbf{x}_0)$ transforme la sphère (resp. boule ouverte, boule fermée) de centre $\mathbf{x}_0$ et de rayon $r$ en la sphère (resp. boule ouverte, boule fermée) de centre 0 et de rayon 1 ; on désigne cette sphère par la notation $S_{n-1}$ et on l’appelle *sphère unité* dans $\mathbf{R}^n$; de même, on désigne par $B_n$, et on appelle *boule unité* dans $\mathbf{R}^n$, la boule *fermée* de centre 0 et de rayon 1. L’étude topologique d’une sphère à $n - 1$ dimensions (resp. d’une boule fermée à $n$ dimensions) est donc ramenée à celle de $S_{n-1}$ (resp. $B_n$). Quant aux boules ouvertes, on a la proposition suivante:

#### Proposition 2 {#top-vi-s2-prop-2 .statement}

*Toute boule ouverte à n dimensions est homéomorphe à $\mathbf{R}^n$.*

En effet, l’application $x \mapsto x/(1 + \|x\|)$ est continue dans $\mathbf{R}^n$ et applique $\mathbf{R}^n$ sur la boule ouverte de centre 0 et de rayon 1 ; en outre, de $y = x/(1 + \|x\|)$ on tire $x = y/(1 - \|y\|)$, donc l’application précédente est bijective et bicontinue.

Désignons par $R_n^*$ le complémentaire de 0 dans $\mathbf{R}^n$, et rappelons qu’on désigne par $\mathbf{R}^*$ l’ensemble des nombres réels $> 0$.

#### Proposition 3 {#top-vi-s2-prop-3 .statement}

*L’application $(t, z) \mapsto tz$ est un homéomorphisme de $\mathbf{R}^* \times S_{n-1}$ sur $R_n^*$.*

En effet, tout point $x \neq 0$ peut s’écrire d’une manière et d’une seule sous la forme $tz$, avec $t > 0$ et $\|z\| = 1$, car de la relation $x = tz$, on tire $t = \|x\|$, et $z = x/\|x\|$. Puisque $tz$ est continue dans le produit $\mathbf{R} \times \mathbf{R}^n$, donc *a fortiori* dans $\mathbf{R}^* \times S_{n-1}$, et que $\|x\|$ et $1/\|x\|$ sont continues dans $R_n^*$, la proposition est démontrée.

L’application $x \mapsto x/\|x\|$ est appelée *projection centrale* de $R_n^*$ sur $S_{n-1}$. On définit de même la *projection centrale* du complémentaire d’un point $a$ sur une sphère de centre $a$.

En particulier, pour $n = 1$, on a $S_{n-1} = \{-1, +1\}$, la projection centrale d’un nombre réel $x \neq 0$ est son signe $\operatorname{sgn} x$, et on retrouve ainsi la prop. 2 de IV, p. 12.

#### Corollaire 1 {#top-vi-s2-prop-3-cor-1 .statement}

*La sphère $S_{n-1}$ est homéomorphe à l’espace quotient de $R_n^*$ par la relation d’équivalence dont les classes sont les demi-droites ouvertes d’origine 0.*

Ces classes peuvent aussi être définies comme les orbites distinctes de $\{0\}$, du groupe des homothéties de rapport $> 0$.

#### Corollaire 2 {#top-vi-s2-prop-3-cor-2 .statement}

*L’espace $R_n^*$ est homéomorphe à $\mathbf{R} \times S_{n-1}$.*

En effet, $\mathbf{R}^* = ]0, +\infty[$ est homéomorphe à $\mathbf{R}$ (IV, p. 13, prop. 1).

#### Remarque {#top-vi-s2-n3-rem-1 .statement}

Les propositions précédentes ne sont pas particulières aux boules euclidiennes, mais peuvent s’étendre à toute une catégorie de voisinages compacts de 0 dans $\mathbf{R}^n$ (voir VI, p. 24, exerc. 12).

Les ensembles $S_{n-1}$ et $B_n$ sont évidemment invariants par toute transformation orthogonale. Si $V$ est un sous-espace vectoriel à $p$ dimensions de $\mathbf{R}^n$, il existe une transformation orthogonale transformant $V$ en le sous-espace vectoriel de

R^n engendré par e_1, e_2, ..., e_p; on en conclut que V ∩ S_{n-1} (resp. V ∩ B_n) est homéomorphe à S_{p-1} (resp. B_p).

### 4. Projection stéréographique

Supposons n > 1 et considérons le point e_n = (0, ..., 0, 1) de S_{n-1}, et l’hyperplan H d’équation x_n = 0, orthogonal au vecteur e_n. À tout point x = (x_i) de S_{n-1}, distinct de e_n, faisons correspondre le point y où la droite passant par e_n et x rencontre l’hyperplan H (fig. 3).

![Figure 3](../images/figure_3.png)

On vérifie aisément qu’on a y = $\frac{1}{1 - x_n} (x - x_n e_n)$ et

$$
x = \frac{\|y\|^2 - 1}{\|y\|^2 + 1} e_n + \frac{2}{\|y\|^2 + 1} y.
$$

Si on désigne par A le complémentaire de {e_n} par rapport à S_{n-1}, ces formules prouvent qu’on a défini ainsi un homéomorphisme de A sur l’hyperplan H. Cet homéomorphisme est appelé projection stéréographique de A sur H, ou, par abus de langage, projection stéréographique de S_{n-1} sur H (cf. A, IX, § 10, exerc. 14); e_n est le point de vue de la projection, H l’hyperplan de projection. Plus généralement, si a est un point de S_{n-1} et H’ l’hyperplan passant par 0 et orthogonal à la droite passant par 0 et a, on définit de la même manière la projection stéréographique de point de vue a sur l’hyperplan de projection H’. Cette projection définit un homéomorphisme du complémentaire de a dans S_{n-1} sur H’, d’où:

#### Proposition 4 {#top-vi-s2-prop-4 .statement}

Pour n ≥ 1, le complémentaire d’un point dans la sphère euclidienne S_{n-1} est homéomorphe à l’espace numérique R^{n-1}.

#### Corollaire 1 {#top-vi-s2-prop-4-cor-1 .statement}

Pour n ≥ 1, la sphère S_{n-1} est homéomorphe à l’espace compact obtenu par adjonction à R^{n-1} d’un « point à l’infini » (I, p. 68).

Comme S_{n-1} est compact, cela résulte immédiatement de la prop. 4 et de loc. cit., th. 4.

#### Corollaire 2 {#top-vi-s2-prop-4-cor-2 .statement}

Pour n > 1, la sphère euclidienne S_{n-1} est un espace connexe et localement connexe dont tout point admet un voisinage ouvert homéomorphe à R^{n-1}.

En effet, la sphère étant un espace séparé, le complémentaire $U(a)$ d’un point $a$ de $S_{n-1}$ est ouvert dans $S_{n-1}$; si $n > 1$, l’espace $S_{n-1}$ est la réunion de deux parties connexes $U(a)$ et $U(-a)$ dont l’intersection est non vide, donc est connexe (I, p. 81, prop. 2).

#### Corollaire 3 {#top-vi-s2-prop-4-cor-3 .statement}

*Pour $n \geqslant 1$, la sphère $S_n$ est homéomorphe à l’espace quotient de la boule $B_n$, obtenu en identifiant tous les points de la sphère $S_{n-1}$.*

En effet, la boule $B_n$ est un espace *régulier* (I, p. 56); donc l’espace quotient F de $B_n$ obtenu en identifiant tous les points de $S_{n-1}$ est *séparé* (I, p. 58, prop. 15). Comme $B_n$ est un espace compact, F est compact, et est donc homéomorphe à l’espace compact déduit d’une boule ouverte à $n$ dimensions par adjonction d’un point à l’infini, en vertu du th. d’Alexandroff (I, p. 67, th. 4); les prop. 2 (VI, p. 10) et 4 entraînent donc le corollaire.

En particulier, pour $n = 1$, compte tenu de la prop. 4 de V, p. 2:

#### Corollaire 4 {#top-vi-s2-prop-4-cor-4 .statement}

*Le cercle $S_1$ est homéomorphe au tore $T$.*

Dans VIII, p. 4, nous retrouverons cette proposition comme conséquence d’un théorème plus précis.

On appelle *hémisphère fermé* (resp. *hémisphère ouvert*) de $S_{n-1}$ l’intersection de $S_{n-1}$ et d’un *demi-espace fermé* (resp. *ouvert*) déterminé par un hyperplan; par projection stéréographique sur un tel hyperplan, l’hémisphère fermé (resp. ouvert) ne contenant pas le point de vue, est appliqué sur une *boule fermée* (resp. *ouverte*) à $n - 1$ dimensions, à laquelle il est donc *homéomorphe*.

Pour $n = 2$, on dit « demi-cercle » au lieu d’« hémisphère ».

## EXERCICES {#top-vi-s2-exercises}

See the [exercises for § 2](exercises/s2/).

[^1]: La seule hypothèse que $d(f(\mathbf{x}), f(\mathbf{y})) = d(\mathbf{x}, \mathbf{y})$ quels que soient $\mathbf{x}, \mathbf{y}$ entraîne d’ailleurs que $f$ est linéaire affine, donc un déplacement (cf. A, IX, § 6, exerc. 21).
