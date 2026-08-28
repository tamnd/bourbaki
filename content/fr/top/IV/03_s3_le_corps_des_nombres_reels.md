---
book: top
book_title: General Topology
chapter: IV
chapter_title: NOMBRES RÉELS
section: 3
section_title: Le corps des nombres réels
lang: fr
source: top-i-iv-fr
book_pages: TG IV.10-TG IV.12, TG IV.51-TG IV.52
pdf_pages: 0281-0283, 0322-0323
extraction: ocr
subsections:
    - "no": 1
      title: La multiplication dans $\mathbf{R}$
      page: 10
      pdf_page: 281
    - "no": 2
      title: Le groupe multiplicatif $\mathbf{R}^*$
      page: 11
      pdf_page: 282
    - "no": 3
      title: Racines n-ièmes
      page: 12
      pdf_page: 283
statements: 2
exercises: 3
content_sha256: 4129deba33be1efb7e47422fe54b0ec337320d02914e0b8adb5465c22b24ea28
---

## § 3. LE CORPS DES NOMBRES RÉELS

### 1. La multiplication dans $\mathbf{R}$

La topologie de la droite rationnelle $\mathbf{Q}$ est non seulement compatible avec la structure de *groupe additif* de $\mathbf{Q}$, mais aussi avec sa structure de *corps*. En effet, la fonction $xy$ est continue au point $(0, 0)$ de $\mathbf{Q} \times \mathbf{Q}$, car pour tout entier $n > 0$, les relations $|x| \leqslant 1/n, |y| \leqslant 1/n$ entraînent $|xy| \leqslant 1/n^2 \leqslant 1/n$; d’autre part, pour tout nombre rationnel $a \neq 0$, la fonction $ax$ est continue au point $x = 0$, car pour $n$ entier $> 0$, la relation $|x| \leqslant \frac{1}{n|a|}$ entraîne $|ax| \leqslant 1/n$. Cela montre que $xy$ est continue en tout point de $\mathbf{Q} \times \mathbf{Q}$ (III, p. 49).

Pour montrer que $1/x$ est continue dans $\mathbf{Q}^*$, on va établir, de façon plus précise, qu’elle est *uniformément continue* (pour la structure additive) dans le complémentaire d’un voisinage arbitraire V de 0. En effet, on a

$$
\left| \frac{1}{x} - \frac{1}{y} \right| = \frac{|x - y|}{|xy|}
$$

il existe un entier $m > 0$ tel que, pour tout $x \in \mathcal{CV}$, $|x| \geqslant 1/m$; si $x$ et $y$ sont deux points de $\mathcal{CV}$ tels que $|x - y| \leqslant 1/m^2 n$, on a donc $\left| \frac{1}{x} - \frac{1}{y} \right| \leqslant 1/n$.

L’image par la fonction $1/x$, de tout filtre de Cauchy sur $\mathbf{Q}^*$ (relatif à la structure uniforme additive) auquel 0 n’est pas adhérent, est encore un filtre de Cauchy (pour la structure uniforme additive). Donc (III, p. 56, prop. 7):

#### Proposition 1 {#top-iv-s3-prop-1 .statement}

Les fonctions xy et $1/x$, définies respectivement dans $\mathbf{Q} \times \mathbf{Q}$ et $\mathbf{Q}^*$, se prolongent par continuité à $\mathbf{R} \times \mathbf{R}$ et $\mathbf{R}^*$ respectivement, et définissent sur $\mathbf{R}$ une structure de corps topologique commutatif. Muni de cette structure, $\mathbf{R}$ est appelé le corps des nombres réels.

Toutes les propriétés des corps topologiques établies dans III, p. 54 à 56, sont naturellement applicables; en particulier, toute fonction rationnelle de n variables réelles, à coefficients réels, est continue en tout point de $\mathbf{R}^n$ où son dénominateur n’est pas nul.

### 2. Le groupe multiplicatif $\mathbf{R}^*$

On sait (III, p. 55) que la topologie induite sur $\mathbf{R}^*$ par celle de la droite numérique est compatible avec la structure de groupe multiplicatif de $\mathbf{R}^*$; comme $\mathbf{R}^*$ est ouvert dans l’espace localement compact $\mathbf{R}$, $\mathbf{R}^*$ est un groupe topologique localement compact (I, p. 66, prop. 13), donc complet (III, p. 22, cor. 1 ; cela résulte aussi de III, p. 56, prop. 8); bien entendu, cette dernière propriété se rapporte à la structure uniforme multiplicative de $\mathbf{R}^*$, et non à la structure uniforme induite sur $\mathbf{R}^*$ par la structure uniforme additive de $\mathbf{R}$.

La fonction $xy$ applique l’ensemble $\mathbf{Q}_+ \times \mathbf{Q}_+$ dans $\mathbf{Q}_+$, donc elle applique $\mathbf{R}_+ \times \mathbf{R}_+$ dans $\mathbf{R}_+$ (I, p. 9, th. 1); en d’autres termes, le produit de deux nombres réels positifs est positif. Les formules $(-x)y = -xy$, $(-x)(-y) = xy$ montrent alors que le produit d’un nombre positif et d’un nombre négatif est négatif, et que le produit de deux nombres négatifs est positif; on en tire la relation
$$
|xy| = |x| \cdot |y|
$$
(qu’on pourrait déduire par prolongement de la même relation dans $\mathbf{Q} \times \mathbf{Q}$).

Si $x > 0, y > 0$, on a $xy \neq 0$, donc $xy > 0$; de même, si $x < 0, y > 0$, $xy < 0$; si $x < 0, y < 0$, $xy > 0$. En particulier, si $x \neq 0, x^2 > 0$; une somme de carrés de nombres réels ne peut être nulle que si chacun de ces nombres est nul.

Si $x > 0$ et $y \leq z$ (resp. $y < z$), on a $xy \leq xz$ (resp. $xy < xz$); autrement dit, une homothétie de rapport $> 0$ conserve l’ordre dans $\mathbf{R}$; comme $(-x)y = -xy$, une homothétie de rapport $< 0$ change l’ordre de $\mathbf{R}$ en l’ordre opposé.

Si $x > 0, 1/x > 0$, car $x.(1/x) = 1 > 0$; si $0 < x < y$, on a $xy > 0$, puis $x.(1/xy) < y.(1/xy)$, c’est-à-dire $1/y < 1/x$; l’application $x \mapsto 1/x$ de l’ensemble $\mathbf{R}_+^*$ des nombres réels $> 0$ sur lui-même est strictement décroissante.

On voit de même que la fonction $1/x$ est strictement décroissante dans $]-\infty, 0[$, d’où résulte que la fonction $\frac{1}{x-a}$ est strictement décroissante dans chacun des intervalles $(a, \infty)$ et $(-\infty, a)$.

Il résulte de ce qui précède que $\mathbf{R}_+^*$ est un sous-groupe du groupe multiplicatif $\mathbf{R}^*$; en outre, la relation d’ordre $x \leq y$ est compatible avec la structure de groupe multiplicatif de $\mathbf{R}_+^*$, autrement dit ce dernier est un groupe totalement ordonné (A, VI, § 1).

Le fait que le produit de deux nombres réels positifs soit positif peut encore s’exprimer en disant que $\mathbf{R}$ est un corps ordonné (A, VI, § 2); et on a vu en Algèbre (loc. cit.) que toutes les propriétés qui précèdent sont communes aux corps ordonnés.

#### Proposition 2 {#top-iv-s3-prop-2 .statement}

*Le groupe multiplicatif $\mathbf{R}^*$ des nombres réels $\neq 0$ est un groupe topologique isomorphe au produit de ses sous-groupes $\mathbf{R}_+^*$ et $\mathbf{U}_0 = \{-1, +1\}$.*

Posons, pour $x \neq 0$, $\operatorname{sgn} x = \frac{x}{|x|}$ (*signe* de $x$); la fonction $\operatorname{sgn}$ est un homomorphisme de $\mathbf{R}^*$ sur $\mathbf{U}_0$; on a $x = |x| \cdot \operatorname{sgn} x$, et cette décomposition de $x$ en un produit d’un élément de $\mathbf{R}_+^*$ et d’un élément de $\mathbf{U}_0$ est unique; donc la structure de groupe de $\mathbf{R}^*$ est le produit de celles de $\mathbf{R}_+^*$ et de $\mathbf{U}_0$. D’autre part, l’application $x \mapsto |x|$ est continue, et il en est de même de $x \mapsto \operatorname{sgn} x = \frac{x}{|x|}$ puisque $x \neq 0$; d’où la proposition.

On étend la fonction $\operatorname{sgn}$ à $\mathbf{R}$ tout entier en posant $\operatorname{sgn} 0 = 0$.

On verra au chap. V (V, § 4, no 1, th. 1) que le groupe topologique $\mathbf{R}_+^*$ est *isomorphe* au groupe *additif* $\mathbf{R}$, ce qui achèvera de déterminer la structure du groupe topologique $\mathbf{R}^*$.

### 3. Racines n-ièmes

Soit $n$ un entier $> 0$ quelconque; de la relation $0 < x < y$, on déduit, par récurrence sur $n$, que $0 < x^n < y^n$; autrement dit, la fonction $x \mapsto x^n$ est *strictement croissante* pour $x \geqslant 0$; elle est évidemment *continue* en tout point, donc (IV, p. 9, th. 5) c’est un *homéomorphisme* de $\mathbf{R}_+$ sur un intervalle $I$; d’autre part, comme $x \geqslant 1$ entraîne $x^{n-1} \geqslant 1$, donc $x^n \geqslant x$, $I$ n’est pas borné, et par suite $I = \mathbf{R}_+$.

On désigne par $x^{1/n}$ ou $\sqrt[n]{x}$, et on appelle $x$ *puissance* $1/n$ ou *racine n-ième de* $x$, la valeur pour $x \geqslant 0$ de l’application *réciproque* de $x \mapsto x^n$ (pour $n = 2, 3$, on dit racine *carrée*, racine *cubique*; pour $n = 2$, on écrit $\sqrt{x}$ au lieu de $\sqrt[2]{x}$). Le nombre positif $x^{1/n}$ est donc défini comme l’unique solution positive de l’équation

$$
y^n = x \quad (x \geqslant 0).
$$

En particulier, on voit qu’il existe un nombre réel $x$ tel que $x^2 = 2$, alors qu’aucun nombre rationnel ne possède cette propriété; on retrouve donc de cette manière que la droite rationnelle $\mathbf{Q}$ n’est pas un espace complet.

L’application $x \mapsto x^{1/n}$ de $\mathbf{R}_+$ sur lui-même est *strictement croissante* et *continue*. D’après (2), on a $0^{1/n} = 0$, $1^{1/n} = 1$ et en outre

$$
(xy)^{1/n} = x^{1/n} y^{1/n},
$$

ce qui montre que $x \mapsto x^{1/n}$ est un *automorphisme* du groupe topologique $\mathbf{R}_+^*$.

Dans V, § 4, no 1, nous généraliserons ce résultat en obtenant *tous* les automorphismes du groupe multiplicatif $\mathbf{R}_+^*$.

## EXERCICES {#top-iv-s3-exercises}

See the [exercises for § 3](exercises/s3/).
