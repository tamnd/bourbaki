---
book: alg
book_title: Algebra
chapter: I
chapter_title: STRUCTURES ALGÉBRIQUES
section: 8
section_title: Anneaux
lang: fr
source: alg-i-iii-fr
book_pages: A I.151-A I.153
pdf_pages: 0102-0118, 0161-0163
extraction: ocr
subsections:
    - "no": 1
      title: Anneaux
      page: 0
      pdf_page: 102
    - "no": 2
      title: Conséquences de la distributivité
      page: 93
      pdf_page: 103
    - "no": 3
      title: Exemples d’anneaux
      page: 96
      pdf_page: 106
    - "no": 4
      title: Homomorphismes d’anneaux
      page: 97
      pdf_page: 107
    - "no": 5
      title: Sous-anneaux
      page: 97
      pdf_page: 107
    - "no": 6
      title: Idéaux
      page: 98
      pdf_page: 108
    - "no": 7
      title: Anneaux quotients
      page: 100
      pdf_page: 110
    - "no": 8
      title: Sous-anneaux et idéaux dans un anneau quotient
      page: 101
      pdf_page: 111
    - "no": 9
      title: Multiplication des idéaux
      page: 0
      pdf_page: 112
    - "no": 10
      title: Produit d’anneaux
      page: 103
      pdf_page: 113
    - "no": 11
      title: Décomposition directe d’un anneau
      page: 104
      pdf_page: 114
    - "no": 12
      title: Anneaux de fractions
      page: 107
      pdf_page: 117
statements: 40
exercises: 16
content_sha256: bf3ea45c41f5440bd1c826701322175fa5fb68e476ae52dac742e21634f09164
---

## § 8. ANNEAUX

### 1. Anneaux

#### Définition 1 {#alg-i-s8-def-1 .statement}

On appelle anneau un ensemble $\mathbf{A}$ muni de deux lois de composition appelées respectivement addition et multiplication, satisfaisant aux axiomes suivants:

(AN I) Pour l’addition, $\mathbf{A}$ est un groupe commutatif.
(AN II) La multiplication est associative et possède un élément neutre.
(AN III) La multiplication est distributive par rapport à l’addition.

On dit que l’anneau $\mathbf{A}$ est commutatif si sa multiplication est commutative.

Dans la suite, on note $(x, y) \mapsto x + y$ l’addition et $(x, y) \mapsto xy$ la multiplication; on note 0 l’élément neutre de l’addition et 1 celui de la multiplication. Enfin, on note $-x$ l’opposé de $x$ pour l’addition. Les axiomes d’un anneau s’expriment donc par les identités suivantes:

(1) $x + (y + z) = (x + y) + z$ (associativité de l’addition)
(2) $x + y = y + x$ (commutativité de l’addition)
(3) $0 + x = x + 0 = x$ (zéro)
(4) $x + (-x) = (-x) + x = 0$ (opposé)
(5) $x(yz) = (xy)z$ (associativité de la multiplication)
(6) $x.1 = 1.x = x$ (élément unité)
(7) $(x + y).z = xz + yz$
(8) $x.(y + z) = xy + xz$ (distributivité)

Enfin l’anneau $\mathbf{A}$ est commutatif si l’on a $xy = yx$ pour $x, y$ dans $\mathbf{A}$.

Muni de la seule addition, $\mathbf{A}$ est un groupe commutatif qu’on appelle groupe additif de $\mathbf{A}$. Pour tout $x \in \mathbf{A}$, définissons l’homothétie à gauche $\gamma_x$ et l’homothétie à droite $\delta_x$ par $\gamma_x(y) = xy, \delta_x(y) = yx$. D’après les formules (7) et (8), $\gamma_x$ et $\delta_x$ sont des endomorphismes du groupe additif de $\mathbf{A}$, donc transforment zéro en zéro et opposé en opposé. Par suite, on a

(9) $x.0 = 0.x = 0$
(10) $x.(-y) = (-x).y = -xy;$
on en déduit $(-x)(-y) = -((-x).y) = -(-xy)$, d’où
(11) $(-x)(-y) = xy.$

Les formules (10) et (11) constituent la règle des signes. On en déduit $-x = (-1).x = x.(-1)$ et $(-1)(-1) = 1$.

De (11) on déduit par récurrence sur $n$ la relation

$$
(-x)^n = \begin{cases}
x^n & \text{si } n \text{ est pair} \\
-x^n & \text{si } n \text{ est impair.}
\end{cases}
$$

Lorsqu’on parle d’éléments simplifiables, d’éléments inversibles, d’éléments permutables, d’éléments centraux, de commutant ou de centre dans un anneau $\mathbf{A}$, toutes ces notions sont relatives à la multiplication dans A. Si $x \in A, y \in A$ et si $y$ est inversible, l’élément $xy^{-1}$ de A se note aussi $x/y$ lorsque A est commutatif. L’ensemble des éléments inversibles de A est stable pour la multiplication. Pour la loi induite par la multiplication, c’est un groupe appelé *groupe multiplicatif* de A, noté parfois $A^*$.

Soient $x, y$ dans A. On dit que $x$ est *multiple à gauche* (resp. *à droite*) de $y$ s’il existe $y' \in A$ tel que $x = y'y$ (resp. $x = yy'$); on dit encore que $y$ est *diviseur à droite* (resp. *à gauche*) de $x$. Lorsque A est commutatif, il est inutile de préciser « à gauche » ou « à droite ».

Conformément à la terminologie ci-dessus, tout élément $y \in A$ devrait être considéré comme un diviseur à droite et à gauche de 0; mais, par abus de langage, on réserve en général le nom de *diviseur à droite* (resp. *à gauche*) *de* 0 aux éléments $y$ tels qu’il existe $x \neq 0$ dans A satisfaisant à la relation $xy = 0$ (resp. $yx = 0$). Autrement dit, les diviseurs de zéro à droite (resp. à gauche) sont les éléments non simplifiables à droite (resp. à gauche).

Soit $x \in A$. On dit que $x$ est *nilpotent* s’il existe un entier $n > 0$ tel que $x^n = 0$. Alors l’élément $1 - x$ est inversible, d’inverse égal à $1 + x + x^2 + \cdots + x^{n-1}$.

Comme A est un groupe commutatif pour l’addition, on a défini (I, p. 23), l’élément $nx$ pour $n \in \mathbf{Z}$ et $x \in A$. Comme $\gamma_x$ et $\delta_x$ sont des endomorphismes du groupe additif A, on a $\gamma_x(ny) = n\gamma_x(y)$ et $\delta_y(nx) = n\delta_y(x)$, d’où
$$
x . (ny) = (nx) . y = n . (xy).
$$
En particulier, on a $nx = (n.1)x$.

On appelle *pseudo-anneau* un ensemble A muni d’une addition et d’une multiplication satisfaisant aux axiomes des anneaux, à l’exception de celui qui assure l’existence de l’élément neutre pour la multiplication.

### 2. Conséquences de la distributivité

La distributivité de la multiplication par rapport à l’addition permet d’appliquer la prop. 1 de I, p. 27, qui donne:

$$
\prod_{i=1}^n \left( \sum_{\lambda \in L_i} x_{i,\lambda} \right) = \sum_{(\alpha_1, \ldots, \alpha_n)} \prod_{i=1}^n x_{i, \alpha_i}
$$
somme étendue à toutes les suites $(\alpha_1, \ldots, \alpha_n)$ appartenant à $L_1 \times \cdots \times L_n$; on suppose que pour $i = 1, \ldots, n$, la famille $(x_{i, \lambda})_{\lambda \in L_i}$ d’éléments de l’anneau A est à support *fini*.

#### Proposition 1 {#alg-i-s8-prop-1 .statement}

*Soient A un anneau commutatif et* $(x_\lambda)_{\lambda \in L}$ *une famille finie d’éléments de A. Pour toute famille d’entiers positifs* $\beta = (\beta_\lambda)_{\lambda \in L}$, *posons* $|\beta| = \sum_{\lambda \in L} \beta_\lambda$. *On a*
$$
\left( \sum_{\lambda \in L} x_\lambda \right)^n = \sum_{|\beta|=n} \frac{n!}{\prod_{\lambda \in L} \beta_\lambda!} \prod_{\lambda \in L} x_\lambda^{\beta_\lambda}.
$$

Appliquons la formule (13) (I, p. 93) avec $L_i = L$ et $x_{i,\lambda} = x_\lambda$ pour $1 \leq i \leq n$. On a donc

$$
(\sum_{\lambda \in L} x_\lambda)^n = \sum_{\alpha_1, \ldots, \alpha_n} x_{\alpha_1} \cdots x_{\alpha_n},
$$

la somme étant étendue à toutes les suites $\alpha = (\alpha_1, \ldots, \alpha_n) \in L^n$.

Soit $\alpha$ dans $L^n$; pour tout $\lambda \in L$, on note $U^\alpha_\lambda$ l’ensemble des entiers $i$ tels que $1 \leq i \leq n$ et $\alpha_i = \lambda$, et l’on pose $\Phi(\alpha) = (U^\alpha_\lambda)_{\lambda \in L}$. Il est immédiat que $\Phi$ est une bijection de $L^n$ sur l’ensemble des partitions de $\{1, 2, \ldots, n\}$ indexées par $L$. Pour tout $\beta \in \mathbf{N}^L$ tel que $|\beta| = n$, on note $L^n_\beta$ l’ensemble des $\alpha \in L^n$ tels que Card $U^\alpha_\lambda = \beta_\lambda$ pour tout $\lambda \in L$. On en déduit que la famille $(L^n_\beta)_{|\beta|=n}$ est une partition de $L^n$ et que l’on a Card $L^n_\beta = \frac{n!}{\prod_{\lambda \in L} \beta_\lambda!}$ (I, p. 58).

Enfin, pour $\alpha \in L^n_\beta$, on a

$$
x_{\alpha_1} \cdots x_{\alpha_n} = \prod_{\lambda \in L} \prod_{i \in U^\alpha_\lambda} x_{\alpha_i} = \prod_{\lambda \in L} \prod_{i \in U^\alpha_\lambda} x_\lambda = \prod_{\lambda \in L} x_{\lambda}^{\beta_\lambda},
$$

d’où

$$
\sum_{(\alpha_1, \ldots, \alpha_n)} x_{\alpha_1} \cdots x_{\alpha_n} = \sum_{|\beta|=n} \sum_{\alpha \in L^n_\beta} x_{\alpha_1} \cdots x_{\alpha_n}
= \sum_{|\beta|=n} \sum_{\alpha \in L^n_\beta} \prod_{\lambda \in L} x_{\lambda}^{\beta_\lambda}
= \sum_{|\beta|=n} \frac{n!}{\prod_{\lambda \in L} \beta_\lambda!} \prod_{\lambda \in L} x_{\lambda}^{\beta_\lambda}
$$

et la formule (14) résulte donc de (15).

#### Corollaire 1 (formule du binôme) {#alg-i-s8-prop-1-cor-1 .statement}

Soient $x$ et $y$ deux éléments d’un anneau commutatif $A$. On a :

$$
(x + y)^n = \sum_{p=0}^n \binom{n}{p} x^p y^{n-p}.
$$

La formule (14) appliquée avec $L = \{1, 2\}$, $x_1 = x$ et $x_2 = y$ donne

$$
(x + y)^n = \sum_{p+q=n} \frac{n!}{p! q!} x^p y^q
$$

la sommation étant étendue aux couples d’entiers positifs $p, q$ avec $p + q = n$. La formule du binôme résulte immédiatement de là (E, III, p. 42).

#### Corollaire 2 {#alg-i-s8-prop-1-cor-2 .statement}

Soient $A$ un anneau commutatif, $X$ un ensemble, $\mathbf{u} = (u_x)_{x \in X}$ et $\mathbf{v} = (v_x)_{x \in X}$ deux familles d’éléments de $A$. Notons $\mathbf{u} + \mathbf{v}$ la famille $(u_x + v_x)_{x \in X}$.

Pour tout $\lambda \in \mathbf{N}^{(X)}$, posons $\lambda! = \prod_{x \in X} \lambda(x)!$. Alors, quel que soit $\alpha \in \mathbf{N}^{(X)}$, on a, avec les notations de I, p. 89,

$$
(u + v)^{\alpha} = \sum_{\beta + \gamma = \alpha} \frac{\alpha!}{\beta! \gamma!} u^{\beta} v^{\gamma}.
$$

En effet, pour $x \in X$, on a

$$
(u_x + v_x)^{\alpha(x)} = \sum_{m+n=\alpha(x)} \frac{\alpha(x)!}{m!n!} u_x^m v_x^n
$$

d’après le cor. 1. En faisant le produit de ces égalités pour $x \in X$, et en tenant compte de (13) (I, p. 93), on obtient le corollaire.

#### Corollaire 3 {#alg-i-s8-prop-1-cor-3 .statement}

Soient A un anneau, x et y des éléments nilpotents et permutables de A. Alors $x + y$ est nilpotent.

On se ramène aussitôt au cas où A est commutatif. Si $x^n = 0$ et $y^n = 0$, le cor. 1 entraîne que $(x + y)^{2n-1} = 0$.

#### Proposition 2 {#alg-i-s8-prop-2 .statement}

Soient A un anneau, $x_1, \ldots, x_n$ des éléments de A, et $I = \{1, 2, \ldots, n\}$.

Pour $H \subset I$, posons $x_H = \sum_{i \in H} x_i$. On a

$$
(-1)^n \sum_{\sigma \in S_n} x_{\sigma(1)} \cdots x_{\sigma(n)} = \sum_{H \subset I} (-1)^{\mathrm{Card}\ H}(x_H)^n.
$$

En particulier, si A est commutatif, on a

$$
(-1)^n n! x_1 x_2 \ldots x_n = \sum_{H \subset I} (-1)^{\mathrm{Card}\ H}(x_H)^n.
$$

Soit C l’ensemble des applications de I dans \{0, 1\}. Si à tout $H \subset I$, on fait correspondre sa fonction caractéristique, on obtient une bijection de $\mathcal{P}(I)$ sur C. Le second membre de (16) est donc égal à:

$$
\sum_{a \in C} (-1)^{a(1)+\ldots+a(n)} \left( \sum_{i \in I} a(i)x_i \right)^n
$$
$$
= \sum_{a \in C} (-1)^{a(1)+\ldots+a(n)} \sum_{(i_1, \ldots, i_n) \in I^n} a(i_1) \ldots a(i_n) x_{i_1} \ldots x_{i_n}
$$
$$
= \sum_{(i_1, \ldots, i_n) \in I^n} c_{i_1 \ldots i_n} x_{i_1} \ldots x_{i_n}
$$

avec

$$
c_{i_1 \ldots i_n} = \sum_{a \in C} (-1)^{a(1)+\ldots+a(n)} a(i_1) \ldots a(i_n).
$$

1) Supposons que $(i_1, \ldots, i_n)$ ne soit pas une permutation de I. Il existe un $j \in I$ distinct de $i_1, \ldots, i_n$. Soit C' l’ensemble des $a \in C$ tels que $a(j) = 0$. Pour tout $a \in C'$, soit $a^*$ la somme de $a$ et de la fonction caractéristique de $\{j\}$. On a $a^*(1) + \cdots + a^*(n) = a(1) + \cdots + a(n) + 1$, donc

$$
c_{i_1 \ldots i_n} = \sum_{a \in C'} (-1)^{a(1)+\ldots+a(n)} a(i_1) \ldots a(i_n) + (-1)^{a^*(1)+\ldots+a^*(n)} a^*(i_1) \ldots a^*(i_n)
$$
$$
= \sum_{a \in C'} ((-1)^{a(1)+\ldots+a(n)} + (-1)^{a(1)+\ldots+a(n)+1}) a(i_1) \ldots a(i_n) = 0.
$$

2) Supposons qu’il existe $\sigma \in S_n$ tel que $i_1 = \sigma(1), \ldots, i_n = \sigma(n)$. Alors $a(i_1) \ldots a(i_n) = 0$ sauf si $a$ ne prend que la valeur 1. Donc $c_{i_1 \ldots i_n} = (-1)^n$.

### 3. Exemples d’anneaux

I. Anneau nul. Soit A un anneau. Pour qu’on ait $0 = 1$ dans A, il faut et il suffit que A soit réduit à un seul élément. En effet, la condition est évidemment suffisante. D’autre part, si $0 = 1$, on a, pour tout $x \in A$, $x = x.1 = x.0 = 0$. Un tel anneau s’appelle un anneau nul.

II. Anneau des entiers rationnels. Pour l’addition définie dans I, p. 20, et la multiplication définie dans I, p. 22, $\mathbf{Z}$ est un anneau commutatif. Les notations 0, 1, $-x$ sont en accord avec les notations introduites antérieurement.

*III. Anneau de fonctions réelles. Soit I un intervalle de l’ensemble $\mathbf{R}$ des nombres réels et soit A l’ensemble des fonctions continues définies dans I et à valeurs réelles. On définit la somme $f + g$ et le produit $f.g$ de deux fonctions $f$ et $g$ par

$$
(f + g)(t) = f(t) + g(t), \quad (fg)(t) = f(t)g(t) \qquad (t \in \mathbf{I}).
$$

On obtient un anneau commutatif dont l’élément unité est la constante 1.*

*IV. Pseudo-anneau de convolution. Soit E l’ensemble des fonctions continues à valeurs réelles définies dans $\mathbf{R}$, nulles en dehors d’un intervalle borné. La somme de deux fonctions est définie comme en III, mais le produit est maintenant défini par

$$
(fg)(t) = \int_{-\infty}^{\infty} f(s)g(t-s)\ ds
$$

(« produit de convolution »). On obtient ainsi un pseudo-anneau commutatif qui n’est pas un anneau (cf. INT, VIII, § 4).*

V. Anneau opposé d’un anneau A. Soit A un anneau. On note souvent $A^0$ l’ensemble A muni de la même addition que A et de la multiplication $(x, y) \mapsto yx$. C’est un anneau (appelé anneau opposé de A) qui admet même zéro et même unité que A, et qui coïncide avec A si et seulement si A est commutatif.

VI. Anneau des endomorphismes d’un groupe commutatif. Soit G un groupe commutatif, noté additivement. On note E l’ensemble des endomorphismes de G. Etant donnés $f$ et $g$ dans E, on définit les applications $f + g$ et $fg$ de G dans G par

$$
(f + g)(x) = f(x) + g(x), \qquad (fg)(x) = f(g(x)) \qquad (x \in \mathbf{G}).
$$

D’après I, p. 10, prop. 5, $f + g$ est un endomorphisme de G, et il en est évidemment de même de $fg = f \circ g$. D’après I, p. 43, E est un groupe (commutatif) pour l’addition. La multiplication est évidemment associative et admet l’élément neutre $\mathrm{Id}_G$. Par ailleurs, pour $f, g$ et $h$ dans E, posons $\varphi = f \cdot (g + h)$; pour tout $x \in \mathbf{G}$, on a

$$
\varphi(x) = f((g + h)(x)) = f(g(x) + h(x)) = f(g(x)) + f(h(x))
$$

car $f$ est un endomorphisme de $G$; on a donc $\varphi = fg + fh$, et il est clair que $(g + h)f = gf + hf$. Par suite, $E$ est un anneau (non commutatif en général) qu’on appelle *anneau des endomorphismes de* $G$.

VII. *Pseudo-anneau de carré nul.* Un pseudo-anneau $A$ est dit de carré nul si $xy = 0$ quels que soient $x, y$ dans $A$. Soit $G$ un groupe commutatif. Si l’on munit l’ensemble $G$ de l’addition du groupe $G$ et de la multiplication $(x, y) \mapsto 0$, on obtient un pseudo-anneau de carré nul. Ce n’est un anneau que si $G = \{0\}$, auquel cas c’est l’anneau nul.

### 4. Homomorphismes d’anneaux

#### Définition 2 {#alg-i-s8-def-2 .statement}

*Soient* $A$ *et* $B$ *deux anneaux*. *On appelle morphisme, ou homomorphisme, de* $A$ *dans* $B$ *toute application* $f$ *de* $A$ *dans* $B$ *satisfaisant aux relations*:

$$
f(x + y) = f(x) + f(y), \quad f(xy) = f(x) \cdot f(y), \quad f(1) = 1,
$$
*quels que soient* $x, y$ *dans* $A$.

Le composé de deux homomorphismes d’anneaux est un homomorphisme d’anneaux. Soient $A$ et $B$ deux anneaux et $f$ une application de $A$ dans $B$; pour que $f$ soit un isomorphisme, il faut et il suffit que ce soit un homomorphisme bijectif; dans ce cas, $f^{-1}$ est un homomorphisme de $B$ dans $A$. Un homomorphisme d’un anneau $A$ dans lui-même s’appelle un *endomorphisme* de $A$.

Soit $f : A \to B$ un homomorphisme d’anneaux. L’application $f$ est un homomorphisme du groupe additif de $A$ dans le groupe additif de $B$; en particulier, on a $f(0) = 0$ et $f(-x) = -f(x)$ pour tout $x \in A$. L’image par $f$ d’un élément inversible de $A$ est un élément inversible de $B$, et la restriction de $f$ au groupe multiplicatif de $A$ est un homomorphisme de ce groupe dans le groupe multiplicatif de $B$.

#### Exemple 1 {#alg-i-s8-n4-exa-1 .statement}

Soit $A$ un anneau. On voit immédiatement que l’application $n \mapsto n.1$ de $\mathbf{Z}$ dans $A$ est l’unique homomorphisme de $\mathbf{Z}$ dans $A$. En particulier, l’application identique de $\mathbf{Z}$ est l’unique endomorphisme de l’anneau $\mathbf{Z}$.

Prenons en particulier pour $A$ l’anneau des endomorphismes du groupe additif $\mathbf{Z}$ (I, p. 96, *Exemple VI*). L’application $n \mapsto n.1$ de $\mathbf{Z}$ dans $A$ est un isomorphisme de $\mathbf{Z}$ sur $A$ d’après la construction même de la multiplication dans $\mathbf{Z}$ (I, p. 22).

#### Exemple 2 {#alg-i-s8-n4-exa-2 .statement}

Soit $a$ un élément inversible d’un anneau $A$. L’application $x \mapsto axa^{-1}$ est un endomorphisme de $A$ car on a
$$
a(x + y)a^{-1} = axa^{-1} + aya^{-1},
$$
$$
a(xy)a^{-1} = (axa^{-1})(aya^{-1}).
$$
Elle est bijective, car la relation $x' = axa^{-1}$ équivaut à $x = a^{-1}x'a$. C’est donc un automorphisme de l’anneau $A$, appelé *automorphisme intérieur associé à* $a$.

### 5. Sous-anneaux

#### Définition 3 {#alg-i-s8-def-3 .statement}

*Soit* $A$ *un anneau*. *On appelle sous-anneau de* $A$ *toute partie* $B$ *de* $A$ *qui est un sous-groupe de* $A$ *pour l’addition, qui est stable pour la multiplication et contient l’unité de* $A$.

Les conditions précédentes peuvent s’écrire

$$
0 \in B, \quad B + B \subset B, \quad -B \subset B, \quad B.B \subset B, \quad 1 \in B.
$$

Si $B$ est un sous-anneau de $A$, on le munit de l’addition et de la multiplication induites par celles de $A$, qui en font un anneau. L’injection canonique de $B$ dans $A$ est un homomorphisme d’anneaux.

#### Exemple 1 {#alg-i-s8-n5-exa-1 .statement}

Tout sous-groupe du groupe additif $\mathbf{Z}$ qui contient 1 est égal à $\mathbf{Z}$. Donc $\mathbf{Z}$ est le seul sous-anneau de $\mathbf{Z}$.

#### Exemple 2 {#alg-i-s8-n5-exa-2 .statement}

Soient $A$ un anneau et $(A_t)_{t \in I}$ une famille de sous-anneaux de $A$; il est immédiat que $\bigcap_{t \in I} A_t$ est un sous-anneau de $A$. En particulier, l’intersection de tous les sous-anneaux de $A$ contenant une partie $X$ de $A$ est un sous-anneau qui est appelé le *sous-anneau de $A$ engendré par $X$*.

#### Exemple 3 {#alg-i-s8-n5-exa-3 .statement}

Soit $X$ une partie d’un anneau $A$. Le commutant de $X$ dans $A$ est un sous-anneau de $A$. En particulier, le centre de $A$ est un sous-anneau de $A$.

#### Exemple 4 {#alg-i-s8-n5-exa-4 .statement}

Soit $G$ un groupe commutatif à opérateurs; on note $\Omega$ l’ensemble d’opérateurs et $\alpha \mapsto f_\alpha$ l’action de $\Omega$ sur $G$. Soit $E$ l’anneau des endomorphismes du groupe sans opérateurs $G$ et $F$ l’ensemble des endomorphismes du groupe à opérateurs $G$. Par définition, $F$ se compose des endomorphismes $\varphi$ de $G$ tels que $\varphi \cdot f_\alpha = f_\alpha \cdot \varphi$ pour tout $\alpha \in \Omega$. Par suite, $F$ est un sous-anneau de l’anneau $E$. On appelle $F$ *l’anneau des endomorphismes du groupe à opérateurs $G$* (cf. II, p. 5). Soit $F_1$ le sous-anneau de $E$ engendré par les $f_\alpha$. Alors $F$ est le commutant de $F_1$ dans $E$.

### 6. Idéaux

#### Définition 4 {#alg-i-s8-def-4 .statement}

*Soit $A$ un anneau. On dit qu’une partie $a$ de $A$ est un idéal à gauche (resp. à droite) si $a$ est un sous-groupe du groupe additif de $A$ et si les relations $a \in A, x \in a$ entraînent $ax \in a$ (resp. $xa \in a$). On dit que $a$ est un idéal bilatère de $A$ si $a$ est à la fois un idéal à gauche et un idéal à droite de $A$.*

La définition d’un idéal à gauche se traduit par les relations

$$
0 \in a, \quad a + a \subset a, \quad A.a \subset a,
$$

la relation $-a \subset a$ résultant de la formule $(-1).x = -x$ et de $A.a \subset a$. Pour tout $x \in A$, soit $\gamma_x$ l’application $a \mapsto xa$ de $A$ dans $A$; l’action $x \mapsto \gamma_x$ munit le groupe additif $A^+$ de $A$ d’une structure de groupe à opérateurs ayant $A$ comme ensemble d’opérateurs. Les idéaux à gauche de $A$ ne sont autres que les sous-groupes de $A^+$ stables pour cette action.

Les idéaux à gauche dans l’anneau $A$ sont les idéaux à droite dans l’anneau opposé $A^0$. Dans un anneau commutatif, les trois espèces d’idéaux se confondent; on les appelle simplement *idéaux*.

#### Exemple 1 {#alg-i-s8-n6-exa-1 .statement}

Soit $A$ un anneau. L’ensemble $A$ est un idéal bilatère de $A$; il en est de même de l’ensemble réduit à 0, qu’on appelle l’idéal *nul* et qu’on écrit parfois 0 ou (0) au lieu de {0}.

#### Exemple 2 {#alg-i-s8-n6-exa-2 .statement}

Pour tout élément $a$ de $A$, l’ensemble $A.a$ des multiples à gauche de $a$ est un idéal à gauche; de même l’ensemble $a.A$ est un idéal à droite. Lorsque $a$ est dans le centre de $A$, on a $A.a = a.A$; cet idéal s’appelle *l’idéal principal* engendré par $a$ et se note $(a)$. On a $(a) = A$ si et seulement si $a$ est inversible.

#### Exemple 3 {#alg-i-s8-n6-exa-3 .statement}

Soit $M$ une partie de $A$. L’ensemble des éléments $x \in A$ tels que $xy = 0$ pour tout $y \in M$ est un idéal à gauche de $A$ qu’on appelle l’*annulateur à gauche* de $M$. On définit de manière analogue l’annulateur à droite de $M$.

#### Exemple 4 {#alg-i-s8-n6-exa-4 .statement}

Toute intersection d’idéaux à gauche (resp. à droite, bilatères) de $A$ est un idéal à gauche (resp. à droite, bilatère). Etant donnée une partie $X$ de $A$, il existe donc un plus petit idéal à gauche (resp. à droite, bilatère) contenant $X$; on l’appelle l’idéal à gauche (resp. à droite, bilatère) *engendré par* $X$.

Soit $a$ un idéal à gauche de $A$. Les conditions $1 \notin a, a \neq A$ sont évidemment équivalentes.

#### Définition 5 {#alg-i-s8-def-5 .statement}

*Soit $A$ un anneau. On dit, par abus de langage, qu’un idéal à gauche $a$ est maximal s’il est un élément maximal de l’ensemble des idéaux à gauche distincts de $A$.* Autrement dit, $a$ est maximal si $a \neq A$ et si les seuls idéaux à gauche de $A$ contenant $a$ sont $a$ et $A$.

#### Théorème 1 (Krull) {#alg-i-s8-thm-1 .statement}

*Soient $A$ un anneau et $a$ un idéal à gauche de $A$ distinct de $A$. Il existe un idéal à gauche maximal $m$ de $A$ contenant $a$.* Considérons $A$ comme opérant dans le groupe additif $A^+$ de $A$ par multiplication à gauche. Alors les idéaux à gauche de $A$ sont les sous-groupes stables de $A^+$. Le théorème résulte donc de I, p. 33, prop. 3, appliquée à la partie $P = \{1\}$ de $A^+$.

#### Proposition 3 {#alg-i-s8-prop-3 .statement}

*Soient $A$ un anneau, $(x_\lambda)_{\lambda \in L}$ une famille d’éléments de $A$, $a$ (resp. $b$) l’ensemble des sommes $\sum_{\lambda \in L} a_\lambda x_\lambda$ où $(a_\lambda)_{\lambda \in L}$ est une famille à support fini d’éléments de $A$ (resp. $\sum_{\lambda \in L} a_\lambda x_\lambda b_\lambda$ où $(a_\lambda)_{\lambda \in L}$, $(b_\lambda)_{\lambda \in L}$ sont des familles à support fini d’éléments de $A$). Alors $a$ (resp. $b$) est l’idéal à gauche (resp. bilatère) de $A$ engendré par l’ensemble des $x_\lambda$.

Les formules

(18) $$
0 = \sum_{\lambda \in L} 0.x_\lambda
$$
(19) $$
\sum_{\lambda \in L} a_\lambda x_\lambda + \sum_{\lambda \in L} a'_\lambda x_\lambda = \sum_{\lambda \in L} (a_\lambda + a'_\lambda)x_\lambda
$$
(20) $$
a.\sum_{\lambda \in L} a_\lambda x_\lambda = \sum_{\lambda \in L} (aa_\lambda)x_\lambda
$$

prouvent que $a$ est un idéal à gauche. Soit $a'$ un idéal à gauche tel que $x_\lambda \in a'$ pour tout $\lambda \in L$, et soit $(a_\lambda)_{\lambda \in L}$ une famille à support fini dans $A$. On a $a_\lambda x_\lambda \in a'$ pour tout $\lambda \in L$, d’où $\sum_{\lambda \in L} a_\lambda x_\lambda \in a'$; on a donc $a \subset a'$. Donc $a$ est l’idéal à gauche de $A$ engendré par les $x_\lambda$. On raisonne de façon analogue pour $b$.

#### Proposition 4 {#alg-i-s8-prop-4 .statement}

Soient $A$ un anneau et $(a_\lambda)_{\lambda \in L}$ une famille d’idéaux à gauche de $A$. L’idéal à gauche engendré par $\bigcup_{\lambda \in L} a_\lambda$ se compose des sommes $\sum_{\lambda \in L} y_\lambda$, où $(y_\lambda)_{\lambda \in L}$ est une famille à support fini telle que $y_\lambda \in a_\lambda$ pour tout $\lambda \in L$.

Soit $a$ l’ensemble des sommes $\sum_{\lambda \in L} y_\lambda$ avec $y_\lambda \in a_\lambda$ pour tout $\lambda \in L$. Les formules $\sum_{\lambda \in L} x_\lambda + \sum_{\lambda \in L} y_\lambda = \sum_{\lambda \in L} (x_\lambda + y_\lambda)$ et $a . \sum_{\lambda \in L} x_\lambda = \sum_{\lambda \in L} a x_\lambda$ montrent que $a$ est un idéal à gauche de $A$. Soient $\lambda \in L$ et $x \in a_\lambda$; posons $y_\lambda = x$ et $y_\mu = 0$ pour $\mu \neq \lambda$; on a $x = \sum_{\lambda \in L} y_\lambda$, d’où $x \in a$ et finalement $a_\lambda \subset a$. Si un idéal à gauche $a'$ contient $a_\lambda$ pour tout $\lambda \in L$, il contient évidemment $a$, donc $a$ est engendré par $\bigcup_{\lambda \in L} a_\lambda$.

On dit que l’idéal $a$ engendré par $\bigcup_{\lambda \in L} a_\lambda$ est la somme des idéaux à gauche $a_\lambda$ et on le note $\sum_{\lambda \in L} a_\lambda$ (cf. II, p. 16). En particulier, la somme $a_1 + a_2$ de deux idéaux à gauche se compose des sommes $a_1 + a_2$ avec $a_1 \in a_1$ et $a_2 \in a_2$.

### 7. Anneaux quotients

Soit $A$ un anneau. Si $a$ est un idéal bilatère de $A$, on dit que deux éléments $x$ et $y$ de $A$ sont congrus modulo $a$ et l’on écrit $x \equiv y$ (mod. $a$) ou $x \equiv y$ ($a$) si $x - y \in a$. On a là une relation d’équivalence dans $A$. Les relations $x \equiv y$ ($a$) et $x' \equiv y'$ ($a$) entraînent $x + x' \equiv y + y'$ ($a$), $x x' \equiv x y'$ ($a$), car $a$ est idéal à gauche, et $x y' \equiv y y'$ ($a$) car $a$ est idéal à droite, d’où $x x' \equiv y y'$ ($a$). Réciproquement, si $R$ est une relation d’équivalence sur $A$ compatible avec l’addition et la multiplication, l’ensemble $a$ des éléments $x$ tels que $x \equiv 0$ mod. $R$ est un idéal bilatère et la relation $x \equiv y$ mod. $R$ équivaut à $x \equiv y$ mod. $a$.

Soient $A$ un anneau et $a$ un idéal bilatère de $A$. On note $A/a$ l’ensemble quotient de $A$ par la relation d’équivalence $x \equiv y$ ($a$), muni de l’addition et de la multiplication quotients de celles de $A$ (I, p. 10, déf. 11). Montrons que $A/a$ est un anneau:
a) Pour l’addition, $A/a$ est le groupe commutatif quotient du groupe additif de $A$ par le sous-groupe $a$.
b) Pour la multiplication, $A/a$ est un monoïde (I, p. 13).
c) Soient $\xi, \eta, \zeta$ dans $A/a$ et soit $\pi : A \to A/a$ l’application canonique; considérons des éléments $x, y, z$ de $A$ tels que $\pi(x) = \xi, \pi(y) = \eta$ et $\pi(z) = \zeta$. On a
$$
\xi(\eta + \zeta) = \pi(x)\pi(y + z) = \pi(x(y + z)) = \pi(xy + xz) = \pi(x)\pi(y) + \pi(x)\pi(z)
= \xi\eta + \xi\zeta
$$
et l’on établit de manière analogue la relation $(\xi + \eta)\zeta = \xi\zeta + \eta\zeta$.

#### Définition 6 {#alg-i-s8-def-6 .statement}

Soient $A$ un anneau et $a$ un idéal bilatère de $A$. On appelle anneau quotient de $A$ par $a$ et l'on note $A/a$ l'ensemble quotient de $A$ par la relation d'équivalence $x \equiv y$ ($a$), muni de l'addition et de la multiplication quotients de celles de $A$.

L'anneau $A/\{0\}$ est isomorphe à $A$, et $A/A$ est un anneau nul.

#### Théorème 2 {#alg-i-s8-thm-2 .statement}

Soient $A$ un anneau et $a$ un idéal bilatère de $A$.
a) L'application canonique $\pi$ de $A$ sur $A/a$ est un homomorphisme d'anneaux.
b) Soient $B$ un anneau et $f$ un homomorphisme de $A$ dans $B$. Si $f(a) = \{0\}$, il existe un homomorphisme $\bar{f}$ de $A/a$ dans $B$ et un seul tel que $f = \bar{f} \circ \pi$.

Par construction, on a $\pi(x + y) = \pi(x) + \pi(y)$ et $\pi(xy) = \pi(x)\pi(y)$ pour $x, y$ dans $A$; on sait que $\pi(1)$ est l'unité $\varepsilon$ de $A/a$, d'où a).

Soient $A^+$ le groupe additif de $A$ et $B^+$ celui de $B$; comme $f$ est un homomorphisme de $A^+$ dans $B^+$, nul sur le sous-groupe $a$ de $A^+$, il existe (I, p. 35, prop. 5) un homomorphisme $\bar{f}$ et un seul de $A^+/a$ dans $B^+$ tel que $f = \bar{f} \circ \pi$. Soient $\xi, \eta$ dans $A/a$; soient $x, y$ dans $A$ tels que $\pi(x) = \xi$ et $\pi(y) = \eta$; on a $\xi \eta = \pi(xy)$ d'où

$$
\bar{f}(\xi \eta) = \bar{f}(\pi(xy)) = f(xy) = f(x) \cdot f(y) = \bar{f}(\xi) \cdot \bar{f}(\eta)
$$

et $\bar{f}(\varepsilon) = \bar{f}(\pi(1)) = f(1) = 1$, donc $\bar{f}$ est un homomorphisme d'anneaux.

#### Théorème 3 {#alg-i-s8-thm-3 .statement}

Soient $A$ et $B$ des anneaux, $f$ un homomorphisme de $A$ dans $B$.
a) Le noyau $a$ de $f$ est un idéal bilatère de $A$.
b) L'image $B' = f(A)$ de $f$ est un sous-anneau de $B$.
c) Soient $\pi : A \to A/a$ et $i : B' \to B$ les morphismes canoniques. Il existe un morphisme $f$ de $A/a$ dans $B'$ et un seul tel que $f = i \circ \bar{f} \circ \pi$, et $\bar{f}$ est un isomorphisme.

Comme $f$ est un morphisme du groupe additif de $A$ dans celui de $B$, $a$ est un sous-groupe de $A$. Si $x \in a$ et $a \in A$, on a $f(ax) = f(a)f(x) = 0$ donc $ax \in a$, et de même $xa \in a$; donc $a$ est un idéal bilatère de $A$. L'assertion b) est évidente. Comme $\bar{f}$ est nulle sur $a$, il existe un morphisme $\bar{f}$ de $A/a$ dans $B'$ tel que $f = i \circ \bar{f} \circ \pi$ (th. 2). L'unicité de $\bar{f}$, et le fait que $\bar{f}$ soit un isomorphisme, résultent de E, II, p. 44.

### 8. Sous-anneaux et idéaux dans un anneau quotient

#### Proposition 5 {#alg-i-s8-prop-5 .statement}

Soient $A$ et $A'$ deux anneaux, $f$ un homomorphisme de $A$ dans $A'$, et $a$ le noyau de $f$.
a) Soit $B'$ un sous-anneau de $A'$. Alors $B = f^{-1}(B')$ est un sous-anneau de $A$ contenant $a$. Si $f$ est surjectif, on a $f(B) = B'$, et $f|B$ définit par passage au quotient un isomorphisme de $B/a$ sur $B'$.
b) Soit $b'$ un idéal à gauche (resp. à droite, bilatère) de $A'$. Alors $b = f^{-1}(b')$ est un idéal à gauche (resp. à droite, bilatère) de $A$ contenant $a$.
c) Si $b'$ est un idéal bilatère de $A'$, l'application composée du morphisme canonique $A' \to A'/b'$ et de $f : A \to A'$ définit, par passage au quotient, un morphisme injectif $\bar{f}$ de $A/b$ dans $A'/b'$. Si $f$ est surjectif, $\bar{f}$ est un isomorphisme de $A/b$ sur $A'/b'$.

d) Supposons $f$ surjectif. Soit $\Phi$ l’ensemble des sous-anneaux (resp. idéaux à gauche, idéaux à droite, idéaux bilatères) de $A$ contenant $a$. Soit $\Phi'$ l’ensemble des sous-anneaux (resp. idéaux à gauche, idéaux à droite, idéaux bilatères) de $A'$. Les applications $B \mapsto f(B)$ et $B' \mapsto f^{-1}(B')$ sont des bijections réciproques de $\Phi$ sur $\Phi'$ et de $\Phi'$ sur $\Phi$.

a) et b) sont évidents, sauf la dernière assertion de a) qui résulte de I, p. 101, th. 3.

Le morphisme composé $g : A \to A' \to A'/b'$ considéré en c) a pour noyau $b$, donc $\bar{f}$ est un morphisme injectif de $A/b$ dans $A'/b'$ (I, p. 101, th. 3). Si $f$ est surjectif, $g$ est surjectif, donc $\bar{f}$ est surjectif.

Supposons $f$ surjectif. D’après ce qui précède, l’application $\theta : B' \mapsto f^{-1}(B')$ est une application de $\Phi'$ dans $\Phi$. Il est clair que l’application $\eta : B \mapsto f(B)$ est une application de $\Phi$ dans $\Phi'$. On a $\theta \circ \eta = \mathrm{Id}_{\Phi}, \eta \circ \theta = \mathrm{Id}_{\Phi'},$ d’où d).

#### Remarque {#alg-i-s8-n8-rem-1 .statement}

Avec les notations précédentes, $\theta$ et $\eta$ sont des isomorphismes d’ensembles ordonnés ($\Phi$ et $\Phi'$ étant ordonnés par inclusion).

#### Corollaire {#alg-i-s8-n8-cor-1 .statement}

Soient $A$ un anneau, $a$ un idéal bilatère de $A$.

a) Tout idéal à gauche (resp. à droite, bilatère) de $A/a$ s’écrit de manière unique sous la forme $b/a$, où $b$ est un idéal à gauche (resp. à droite, bilatère) de $A$ contenant $a$.

b) Si $b$ est bilatère, l’homomorphisme composé $A \to A/a \to (A/a)/(b/a)$ définit par passage au quotient un isomorphisme de $A/b$ sur $(A/a)(b/a)$.

Il suffit d’appliquer la prop. 5 au morphisme canonique de $A$ sur $A/a$.

### 9. Multiplication des idéaux

Soient $A$ un anneau, $a$ et $b$ des idéaux bilatères de $A$. L’ensemble des éléments de la forme $x_1 y_1 + \cdots + x_n y_n$ avec $n \geq 0$, $x_i \in a$ et $y_i \in b$ pour $1 \leq i \leq n$, est évidemment un idéal bilatère de $A$, qu’on note $ab$ et qu’on appelle le produit des idéaux bilatères $a$ et $b$. Pour cette multiplication, l’ensemble des idéaux bilatères de $A$ est un monoïde, ayant pour élément unité l’idéal bilatère $A$. Si $a, b, c$ sont des idéaux bilatères de $A$, on a $a(b+c) = ab + ac, (b+c)a = ba + ca$. Si $A$ est commutatif, la multiplication des idéaux est commutative.

On a $ab \subset aA \subset a$ et $ab \subset Ab \subset b$, donc
$$
ab \subset a \cap b.
$$
(21)

#### Proposition 6 {#alg-i-s8-prop-6 .statement}

Soient $a, b_1, \ldots, b_n$ des idéaux bilatères de $A$. Si $A = a + b_i$ pour tout $i$, on a $A = a + b_1 b_2 \ldots b_n = a + (b_1 \cap b_2 \cap \cdots \cap b_n)$.

D’après (21), il suffit de prouver que $A = a + b_1 b_2 \cdots b_n$. Par récurrence, il suffit d’envisager le cas où $n = 2$. Par hypothèse, il existe $a, a'$ dans $a, b_1 \in b_1, b_2 \in b_2$ tels que $1 = a + b_1 = a' + b_2$. Alors
$$
1 = a' + (a + b_1) b_2 = (a' + ab_2) + b_1 b_2 \in a + b_1 b_2,
$$
d’où $A = a + b_1 b_2$.

#### Proposition 7 {#alg-i-s8-prop-7 .statement}

Soient $b_1, \ldots, b_n$ des idéaux bilatères de $A$, tels que $b_i + b_j = A$ pour i ≠ j. Alors $b_1 \cap b_2 \cap \cdots \cap b_n = \sum_{\sigma \in S_n} b_{\sigma(1)} b_{\sigma(2)} \cdots b_{\sigma(n)}$. En particulier, si A est commutatif, $b_1 \cap b_2 \cap \cdots \cap b_n = b_1 b_2 \cdots b_n$ (cf. I, p. 151, exerc. 2).

Supposons d’abord $n = 2$. Il existe $a_1 \in b_1, a_2 \in b_2$ tels que $a_1 + a_2 = 1$. Si $x \in b_1 \cap b_2$, on a $x = x(a_1 + a_2) = xa_1 + xa_2 \in b_2 b_1 + b_1 b_2$. Donc $b_1 \cap b_2 = b_1 b_2 + b_2 b_1$.

Supposons maintenant l’égalité de la proposition établie pour les entiers <n. D’après la prop. 6 (I, p. 102), on a $b_n + (b_1 b_2 \cdots b_{n-1}) = A$, donc
$$
b_1 \cap b_2 \cap \cdots \cap b_n = (b_1 \cap b_2 \cap \cdots \cap b_{n-1}) b_n + b_n (b_1 \cap b_2 \cap \cdots \cap b_{n-1})
$$
$$
= \left( \sum_{\sigma \in S_{n-1}} b_{\sigma(1)} b_{\sigma(2)} \cdots b_{\sigma(n-1)} \right) b_n + b_n \left( \sum_{\sigma \in S_{n-1}} b_{\sigma(1)} b_{\sigma(2)} \cdots b_{\sigma(n-1)} \right)
$$
$$
\subset \sum_{\tau \in S} b_{\tau(1)} b_{\tau(2)} \cdots b_{\tau(n)} \subset b_1 \cap b_2 \cap \cdots \cap b_n.
$$

### 10. Produit d’anneaux

Soit $(A_i)_{i \in I}$ une famille d’anneaux. Soit A l’ensemble produit $\prod_{i \in I} A_i$. Sur A, on définit une addition et une multiplication par les formules
$$(22)\quad (x_i) + (y_i) = (x_i + y_i), \qquad (x_i)(y_i) = (x_i y_i).$$

On vérifie immédiatement que A est un anneau (dit produit des anneaux $A_i$) ayant pour zéro l’élément $0 = (0_i)_{i \in I}$ où $0_i$ est le zéro de $A_i$, et pour unité $1 = (1_i)_{i \in I}$ où $1_i$ est l’unité de $A_i$. Si les $A_i$ sont commutatifs, il en est de même de A. Si $C_i$ est le centre de $A_i$, le centre de A est $\prod_{i \in I} C_i$.

Pour tout $i \in I$, la projection $\mathrm{pr}_i$ de A sur $A_i$ est un homomorphisme d’anneaux. Si B est un anneau et $f_i : B \to A_i$ une famille d’homomorphismes, il existe un unique homomorphisme $f : B \to A$ tel que $f_i = \mathrm{pr}_i \circ f$ pour tout $i \in I$; il est donné par $f(b) = (f_i(b))_{i \in I}$.

Pour tout $i \in I$, soit $a_i$ un idéal à gauche de $A_i$. Alors $a = \prod_{i \in I} a_i$ est un idéal à gauche de A. On a un énoncé analogue pour les idéaux à droite, les idéaux bilatères et les sous-anneaux. Supposons que $a_i$ soit un idéal bilatère pour tout $i \in I$, et notons $f_i$ l’application canonique de $A_i$ sur $A_i / a_i$. Alors l’application $f : (x_i)_{i \in I} \mapsto (f_i(x_i))_{i \in I}$ de $\prod_{i \in I} A_i$ sur $\prod_{i \in I} (A_i / a_i)$ est un homomorphisme d’anneaux de noyau $\prod_{i \in I} a_i$, donc définit par passage au quotient un isomorphisme de $(\prod_{i \in I} A_i) / (\prod_{i \in I} a_i)$ sur $\prod_{i \in I} (A_i / a_i)$.

Soit $(I_\lambda)_{\lambda \in \Lambda}$ une partition de I. La bijection canonique de $\prod_{i \in I} A_i$ sur $\prod_{\lambda \in \Lambda} (\prod_{i \in I_\lambda} A_i)$ est un isomorphisme d’anneaux, par lequel on identifie ces deux anneaux.

Soit $J \subset I$. Notons $e_J$ l’élément $(x_i)_{i \in I}$ de $A$ défini par $x_i = 1_i$ pour $i \in J$, $x_i = 0_i$ pour $i \in I - J$. Alors $e_J$ est un idempotent central (I, p. 7) de $A$. On a aussitôt les formules suivantes:

$$
e_I = 1; \\
e_\varnothing = 0; \\
e_{J \cap K} = e_J e_K \quad \text{pour } J \subset I, K \subset I; \\
e_{J \cup K} = e_J + e_K \quad \text{pour } J \subset I, K \subset I, J \cap K = \varnothing; \\
\sum_\lambda e_{J_\lambda} = 1 \quad \text{si } (J_\lambda) \text{ est une partition finie de } I.
$$

Posons $A_J = \prod_{i \in J} A_i$. Soit $\eta_J$ la projection canonique de $A$ sur $A_J$. Pour $x = (x_i)_{i \in J} \in A_J$, soit $\varepsilon_J(x)$ l’élément $(y_i)_{i \in I}$ de $A$ défini par $y_i = x_i$ pour $i \in J$, $y_i = 0_i$ pour $i \in I - J$. Alors $\eta_J$ est un homomorphisme d’anneaux de $A$ sur $A_J$, $\varepsilon_J$ est un homomorphisme injectif de groupe additif de $A_J$ dans $A$, et, dans le diagramme

$$
A_J \xrightarrow{\varepsilon_J} A \xrightarrow{\eta_{I-J}} A_{I-J}
$$

le noyau $a_J$ de $\eta_{I-J}$ est égal à l’image de $\varepsilon_J$. On a $\varepsilon_J(xx') = \varepsilon_J(x)\varepsilon_J(x')$ quels que soient $x, x'$ dans $A_J$; mais $\varepsilon_J$ n’est pas en général un homomorphisme d’anneaux car $\varepsilon_J(1) = e_J$. Il est clair que $a_J = e_J A = A e_J$.

Posons $e_{\{i\}} = e_i$ et $a_i = a_{\{i\}} = e_i A = A e_i$ pour tout $i \in I$. On a $e_i^2 = e_i$, $e_i e_j = e_j e_i = 0$ pour $i \neq j$. Si $I$ est fini, on a $\sum_{i \in I} e_i = 1$, le groupe additif $A$ est somme directe des idéaux bilatères $a_i$, et, si $x \in A$, sa composante dans $a_i$ est $x e_i$. On en déduit aussitôt la proposition suivante:

#### Proposition 8 {#alg-i-s8-prop-8 .statement}

*Supposons I fini. Si b est un idéal à gauche ou à droite de A, b est somme directe des b ∩ a_i.*

### 11. Décomposition directe d’un anneau

Soient $A$ un anneau, $(b_i)_{i \in I}$ une famille d’idéaux bilatères de $A$. Nous appellerons homomorphisme canonique de $A$ dans $\prod_{i \in I} (A/b_i)$ l’homomorphisme

$$
x \mapsto (\varphi_i(x))_{i \in I},
$$

où $\varphi_i$ est l’homomorphisme canonique de $A$ sur $A/b_i$.

#### Proposition 9 {#alg-i-s8-prop-9 .statement}

*Soient A un anneau, $b_1, \ldots, b_n$ des idéaux bilatères de A tels que $b_i + b_j = A$ pour $i \neq j$. L’homomorphisme canonique de A dans $\prod_{i=1}^n (A/b_i)$ est surjectif, de noyau $\bigcap_{i=1}^n b_i = \sum_{\sigma \in S_n} b_{\sigma(1)} b_{\sigma(2)} \cdots b_{\sigma(n)}$.*

Il est clair que le noyau est $\bigcap_{i=1}^{n} b_i$. Pour prouver la surjectivité, il faut montrer que, pour toute famille $(x_i)_{1 \leq i \leq n}$ d’éléments de $A$, il existe $x \in A$ tel que $x \equiv x_i \ (b_i)$ pour $1 \leq i \leq n$. Prouvons cette assertion par récurrence sur $n$, le cas $n \leq 1$ étant trivial. D’après l’hypothèse de récurrence, il existe $y \in A$ tel que $y \equiv x_i \ (b_i)$ pour $1 \leq i \leq n - 1$. Cherchons $x$ sous la forme $y + z$ avec $z \in A$. On doit avoir $z \equiv 0 \ (b_i)$ pour $i < n$, c’est-à-dire $z \in b = \bigcap_{i=1}^{n-1} b_i$, et d’autre part $z \equiv x_n - y \ (b_n)$. Or $b_n + b = A$ d’après I, p. 102, prop. 6, d’où l’existence de $z$. Enfin, la deuxième expression du noyau résulte de I, p. 102, prop. 7.

#### Définition 7 {#alg-i-s8-def-7 .statement}

Soit $A$ un anneau. On appelle décomposition directe de $A$ une famille finie $(b_i)_{i \in I}$ d’idéaux bilatères de $A$ telle que l’homomorphisme canonique de $A$ dans $\prod_{i \in I} (A/b_i)$ soit un isomorphisme.

#### Proposition 10 {#alg-i-s8-prop-10 .statement}

Soient $A$ un anneau, $A'$ son centre, $(b_i)_{i \in I}$ une famille finie d’idéaux bilatères de $A$. Les conditions suivantes sont équivalentes:

a) la famille $(b_i)_{i \in I}$ est une décomposition directe de $A$;
b) il existe une famille $(e_i)_{i \in I}$ d’idempotents de $A'$ tels que $e_i e_j = 0$ pour $i \neq j$, $1 = \sum_{i \in I} e_i$, et $b_i = A(1 - e_i)$ pour $i \in I$;
c) on a $b_i + b_j = A$ pour $i \neq j$, et $\bigcap_{i \in I} b_i = \{0\}$;
d) on a $b_i + b_j = A$ pour $i \neq j$, et $\prod_{i \in I} b_i = \{0\}$ pour tout ordre total sur $I$;
e) il existe une décomposition directe $(b'_i)_{i \in I}$ de $A'$ telle que $b_i = A b'_i$ pour $i \in I$.

a) $\Rightarrow$ b). Si la condition a) est vérifiée, on peut identifier $A$ à l’anneau $\prod_{i \in I} (A/b_i)$, et $b_i$ au noyau de $\mathrm{pr}_i$. L’existence des $e_i$ avec les propriétés de b) résulte alors de I, p. 104.

b) $\Rightarrow$ d). Supposons qu’il existe des $e_i$ avec les propriétés de b). Pour $i \neq j$, on a $1 - e_i \in b_i, e_i = e_i(1 - e_j) \in b_j$, donc $1 \in b_i + b_j$ et $A = b_i + b_j$. D’autre part, si I est muni d’un ordre total et si $(x_i)_{i \in I}$ est une famille d’éléments de $A$, on a, puisque les $e_i$ sont centraux,

$$
\prod_{i \in I} x_i (1 - e_i) = (\prod_{i \in I} x_i)(\prod_{i \in I} (1 - e_i)) = (\prod_{i \in I} x_i)(1 - \sum_{i \in I} e_i) = 0
$$

donc $\prod_{i \in I} b_i = \{0\}$.

d) $\Rightarrow$ c). Cela résulte de I, p. 102, prop. 7.

c) $\Rightarrow$ a). Cela résulte de I, p. 104, prop. 9.

Ainsi, les conditions a), b), c) et d) sont équivalentes. Supposons-les vérifiées. Puisque b) $\Rightarrow$ a), la famille des $b'_i = A'(1 - e_i)$ est une décomposition directe de $A'$. On a $b_i = A(1 - e_i) = A b'_i$ pour tout $i \in I$. Donc la condition e) est vérifiée.

Enfin, supposons la condition e) vérifiée. Puisque a) $\Rightarrow$ b), il existe une famille (e_i)_{i \in I} d’idempotents de A’ tels que $e_i e_j = 0$ pour $i \neq j$, $1 = \sum_{i \in I} e_i$, et $b'_i = A'(1 - e_i)$ pour $i \in I$. Alors $b_i = Ab'_i = A(1 - e_i)$ pour $i \in I$, donc la condition b) est vérifiée.

#### Remarque {#alg-i-s8-n11-rem-1 .statement}

Soit A un anneau. Soit $(a_i)_{i \in I}$ une famille finie de sous-groupes du groupe additif $A^+$ de A, telle que $A^+$ soit somme directe des $a_i$. Supposons $a_i a_i \subset a_i$ pour $i \in I$, et $a_i a_j = \{0\}$ pour $i \neq j$. Alors $a_i$ est, pour tout $i \in I$, un idéal bilatère de A. Muni de l’addition et de la multiplication induites par celles de A, $a_i$ est un anneau admettant pour élément unité la composante de $1 \in A$ dans $a_i$.

Si $b_i = \sum_{j \neq i} a_j$, il est clair que les $b_i$ vérifient la condition c) de la prop. 10, donc $(b_i)_{i \in I}$ est une décomposition directe de A, qui est dite définie par $(a_i)_{i \in I}$.

Exemple: Idéaux et anneaux quotients de $\mathbf{Z}$
Un idéal de $\mathbf{Z}$ est un sous-groupe additif de $\mathbf{Z}$, donc de la forme $n.\mathbf{Z}$ avec $n \geqslant 0$; réciproquement, pour tout entier $n \geqslant 0$, l’ensemble $n.\mathbf{Z}$ est un idéal, l’idéal principal $(n)$. Donc tout idéal de $\mathbf{Z}$ est principal, et se représente de manière unique sous la forme $n\mathbf{Z}$ avec $n \geqslant 0$. L’idéal (1) est égal à $\mathbf{Z}$, l’idéal (0) est réduit à 0, et les idéaux distincts de $\mathbf{Z}$ et $\{0\}$ sont donc de la forme $n\mathbf{Z}$ avec $n > 1$. Si $m \geqslant 1$ et $n \geqslant 1$, on a $m\mathbf{Z} \supset n\mathbf{Z}$ si et seulement si $n \in m.\mathbf{Z}$, c’est-à-dire si $m$ divise $n$. Par suite, pour que l’idéal $n\mathbf{Z}$ soit maximal, il faut et il suffit qu’il n’existe aucun entier $m > 1$ distinct de $n$ divisant $n$; autrement dit, les idéaux maximaux de $\mathbf{Z}$ sont les idéaux de la forme $p\mathbf{Z}$ où $p$ est un nombre premier (I, p. 48, déf. 16).

Soient $m$ et $n$ deux entiers $\geqslant 1$. L’idéal $m\mathbf{Z} + n\mathbf{Z}$ est principal, d’où l’existence d’un entier $d \geqslant 1$ caractérisé par $d\mathbf{Z} = m\mathbf{Z} + n\mathbf{Z}$; pour tout entier $r \geqslant 1$, la relation «$r$ divise $d$» équivaut à $r\mathbf{Z} \supset d\mathbf{Z}$, donc à «$r\mathbf{Z} \supset m\mathbf{Z}$ et $r\mathbf{Z} \supset n\mathbf{Z}$» c’est-à-dire à «$r$ divise $m$ et $n$». On voit donc que les diviseurs communs à $m$ et $n$ sont les diviseurs de $d$ et que $d$ est par suite le plus grand des diviseurs $\geqslant 1$ communs à $m$ et $n$; on appelle $d$ le plus grand commun diviseur (en abrégé p.g.c.d.) de $m$ et $n$. Comme $d\mathbf{Z} = m\mathbf{Z} + n\mathbf{Z}$, il existe deux entiers $x$ et $y$ tels que $d = mx + ny$. On dit que $m$ et $n$ sont étrangers (ou premiers entre eux) si leur p.g.c.d. est égal à 1. Il revient au même de supposer qu’il existe des entiers $x$ et $y$ tels que $mx + ny = 1$.

L’intersection des idéaux $m\mathbf{Z}$ et $n\mathbf{Z}$ n’est pas nulle car elle contient $mn$, donc est de la forme $r\mathbf{Z}$ avec $r \geqslant 1$. En raisonnant comme précédemment, on voit que les multiples de $r$ sont les multiples communs à $m$ et $n$, et que $r$ est le plus petit des entiers $\geqslant 1$ multiples communs de $m$ et $n$; on l’appelle le plus petit commun multiple (p.p.c.m.) de $m$ et $n$.

Le produit des idéaux $m\mathbf{Z}$ et $n\mathbf{Z}$ est l’ensemble des $\sum_{i=1}^r mx_i ny_i = mn (\sum_{i=1}^r x_i y_i)$ pour $x_1, \ldots, y_r$ dans $\mathbf{Z}$, donc est égal à $mn\mathbf{Z}$.

Pour tout entier $n \geqslant 1$, l’anneau quotient $\mathbf{Z}/n\mathbf{Z}$ s’appelle l’anneau des entiers modulo $n$; il a $n$ éléments, qui sont les classes modulo $n$ des entiers $0, 1, 2, \ldots, n-1$. Pour $n = 1$, on obtient un anneau nul.

#### Proposition 11 {#alg-i-s8-prop-11 .statement}

Soient $n_1, \ldots, n_r$ des entiers $\geqslant 1$, étrangers deux à deux, et $n = n_1 \ldots n_r$. L’homomorphisme canonique de $\mathbf{Z}$ dans l’anneau produit $\prod_{i=1}^r (\mathbf{Z}/n_i\mathbf{Z})$ est surjectif, de noyau $n\mathbf{Z}$, et définit un isomorphisme d’anneaux de $\mathbf{Z}/n\mathbf{Z}$ sur $\prod_{i=1}^r (\mathbf{Z}/n_i\mathbf{Z})$.

Posons $a_i = n_i\mathbf{Z}$ pour $i = 1, \ldots, r$. Par hypothèse, on a $a_i + a_j = \mathbf{Z}$ pour $i \neq j$. La prop. résulte alors de I, p. 104, prop. 9.

Les résultats précédents, ainsi que ceux relatifs à la décomposition en facteurs premiers, seront généralisés au chap. VII, § 1, consacré à l’étude des anneaux principaux et en Alg. comm., chap. VII, § 3, consacré à l’étude des anneaux factoriels.

### 12. Anneaux de fractions

#### Théorème 4 {#alg-i-s8-thm-4 .statement}

Soient $A$ un anneau commutatif et $S$ une partie de $A$. Soit $A_S$ le monoïde des fractions de $A$ (muni de la seule multiplication) à dénominateurs dans $S$ (I, p. 17). Soit $\varepsilon : A \to A_S$ le morphisme canonique. Il existe sur $A_S$ une addition et une seule satisfaisant aux conditions suivantes:
a) $A_S$, muni de cette addition et de sa multiplication, est un anneau commutatif;
b) $\varepsilon$ est un homomorphisme d’anneaux.

Supposons trouvée sur $A_S$ une addition satisfaisant aux conditions a) et b). Soient $x, y$ dans $A_S$. Soit $S'$ le sous-monoïde multiplicatif de $A$ engendré par $S$. Il existe $a, b$ dans $A$ et $p, q$ dans $S'$ tels que $x = a/p, y = b/q$. On a $x = \varepsilon(aq)\varepsilon(pq)^{-1}$, $y = \varepsilon(bp)\varepsilon(pq)^{-1}$, d’où
$$
x + y = (\varepsilon(aq) + \varepsilon(bp))\varepsilon(pq)^{-1}
= \varepsilon(aq + bp)\varepsilon(pq)^{-1}
= (aq + bp)/pq.
$$
(23)

Cela prouve l’unicité de l’addition.

Définissons maintenant une addition dans $A_S$ en posant $x + y = (aq + bp)/pq$. Il faut montrer que cette définition ne dépend pas du choix de $a, b, p, q$. Or, si $a', b'$ dans $A$, $p', q'$ dans $S'$ sont tels que $x = a'/p', y = b'/q'$, il existe $s$ et $t$ dans $S'$ tels que $ap's = a'ps, bq't = b'qt$, d’où
$$(aq + bp)(p'q')(st) = (a'q' + b'p')(pq)(st)$$
et donc
$$(aq + bp)/pq = (a'q' + b'p')/p'q'.$$

On vérifie facilement que l’addition dans $A_S$ est associative et commutative, que $0/1$ est élément neutre pour l’addition, que $(-a)/p$ est opposé de $a/p$, et que $x(y + z) = xy + xz$ quels que soient $x, y, z \in A_S$. Si $a, b \in A$, on a
$$\varepsilon(a + b) = (a + b)/1 = a/1 + b/1 = \varepsilon(a) + \varepsilon(b)$$
donc $\varepsilon$ est un homomorphisme d’anneaux.

#### Définition 8 {#alg-i-s8-def-8 .statement}

L’anneau défini au th. 4 s’appelle l’anneau des fractions de A associé à S, ou à dénominateurs dans S, et se note $A[S^{-1}]$.

Le zéro $A[S^{-1}]$ est 0/1, l’unité de $A[S^{-1}]$ est 1/1.
On reviendra sur les propriétés de $A[S^{-1}]$ en Alg. comm., chap. II, § 2.
Si S est l’ensemble des éléments simplifiables de A, l’anneau $A[S^{-1}]$ s’appelle l’anneau total des fractions de A. On identifie alors A à un sous-anneau de A $[S^{-1}]$ grâce à l’application $\varepsilon$, qui est alors injective (I, p. 18, prop. 6).

#### Théorème 5 {#alg-i-s8-thm-5 .statement}

Soient A un anneau commutatif, S une partie de A, B un anneau, f un homomorphisme de A dans B tel que tout élément de $f(S)$ soit inversible. Il existe un homomorphisme $\bar{f}$ de $A[S^{-1}]$ dans B et un seul tel que $f = \bar{f} \circ \varepsilon$.

On sait (I, p. 18, th. 1) qu’il existe un morphisme $\bar{f}$ et un seul du monoïde multiplicatif $A[S^{-1}]$ dans le monoïde multiplicatif B tel que $f = \bar{f} \circ \varepsilon$. Soient $a, b$ dans A, $p, q$ dans $S'$ (sous-monoïde multiplicatif de A engendré par S). Comme les éléments de $f(A)$ commutent deux à deux, on a
$$
\begin{align*}
\bar{f}(a/p + b/q) &= \bar{f}((aq + bp)/pq) = f(aq + bp)f(pq)^{-1} \\
&= (f(a)f(q) + f(b)f(p))f(p)^{-1}f(q)^{-1} \\
&= f(a)f(p)^{-1} + f(b)f(q)^{-1} \\
&= \bar{f}(a/p) + \bar{f}(b/q).
\end{align*}
$$
Donc $\bar{f}$ est un homomorphisme d’anneaux.

## EXERCICES {#alg-i-s8-exercises}

See the [exercises for § 8](exercises/s8/).
