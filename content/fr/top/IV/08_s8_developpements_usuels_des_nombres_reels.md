---
book: top
book_title: General Topology
chapter: IV
chapter_title: NOMBRES RÉELS
section: 8
section_title: Développements usuels des nombres réels
lang: fr
source: top-i-iv-fr
book_pages: TG IV.62-TG IV.64
pdf_pages: 0311-0316, 0333-0335
extraction: ocr
subsections:
    - "no": 1
      title: Valeurs approchées d’un nombre réel
      page: 40
      pdf_page: 311
    - "no": 2
      title: Développements des nombres réels relatifs à une suite de base
      page: 40
      pdf_page: 311
    - "no": 3
      title: Définition d’un nombre réel par son développement
      page: 41
      pdf_page: 312
    - "no": 4
      title: Comparaison des développements
      page: 42
      pdf_page: 313
    - "no": 5
      title: Développements de base a
      page: 43
      pdf_page: 314
    - "no": 6
      title: Cardinal de R
      page: 44
      pdf_page: 315
statements: 3
exercises: 17
content_sha256: c0e4c70a6e778ef71ceaffe15a445ecf38a19ce2a86aa00397867e1e26e55e37
---

## § 8. DÉVELOPPEMENTS USUELS DES NOMBRES RÉELS

### 1. Valeurs approchées d’un nombre réel

#### Définition 1 {#top-iv-s8-def-1 .statement}

Étant donné un nombre $\varepsilon > 0$, on dit qu’un nombre réel $r$ est valeur approchée à $\varepsilon$ près d’un nombre réel $x$, si $|x - r| \leq \varepsilon$; $r$ est dit valeur approchée par défaut si $r \leq x$, par excès si $r \geq x$.

Soit $A$ une partie partout dense de $\mathbf{R}$; pour tout $x \in \mathbf{R}$, et tout $\varepsilon > 0$, il existe une valeur approchée de $x$ à $\varepsilon$ près par défaut (resp. par excès) appartenant à $A$, car l’intervalle $]x - \varepsilon, x[$ (resp. $]x, x + \varepsilon[$) contient un point au moins de $A$. Si on considère maintenant une suite strictement décroissante donnée $(\varepsilon_n)$ de nombres $> 0$, tendant vers $0$, et si $r_n \in A$ est une valeur approchée de $x$ à $\varepsilon_n$ près, la suite $(r_n)$ a pour limite $x$ lorsque $n$ croît indéfiniment.

Dans le cas où $A$ est un sous-groupe du groupe additif $\mathbf{R}$, et qu’on astreint les $\varepsilon_n$ à appartenir à $A$, on peut définir canoniquement, pour tout $x \in \mathbf{R}$, une suite $(r_n)$ de valeurs approchées par défaut de $x$, appartenant à $A$.

En effet, d’après l’axiome d’Archimède (IV, p. 6, th. 1), l’ensemble des entiers $p$ tels que $p \varepsilon_n \leq x$ a un plus grand élément $p_n$; autrement dit, il existe un entier $p_n$ et un seul tel que

$$
p_n \varepsilon_n \leq x < (p_n + 1) \varepsilon_n.
$$

Comme $|x - p_n \varepsilon_n| \leq \varepsilon_n$, $p_n \varepsilon_n$ est une valeur approchée de $x$ à $\varepsilon_n$ près par défaut et appartient à $A$ d’après l’hypothèse; de même $(p_n + 1) \varepsilon_n$ est une valeur approchée de $x$ à $\varepsilon_n$ près par excès, appartenant à $A$, et les deux suites $(p_n \varepsilon_n)$ et $((p_n + 1) \varepsilon_n)$ ont pour limite $x$.

### 2. Développements des nombres réels relatifs à une suite de base

On va se borner à étudier le cas où $\varepsilon_n = \frac{1}{d_n}$, $(d_n)$ étant une suite strictement croissante d’entiers tels que $d_0 = 1$, et que $d_n$ soit un multiple de $d_{n-1}$ pour $n \geq 1$.

On posera $a_n = \frac{d_n}{d_{n-1}}$ ($n \geq 1$): c’est un entier $> 1$. Dans ce cas, la suite des valeurs approchées par défaut $r_n = \frac{p_n}{d_n}$ est croissante: en effet, $p_n$ est le plus grand entier tel que $\frac{p_n}{d_n} \leq x$; mais on a

$$
\frac{p_{n-1}}{d_{n-1}} = \frac{p_{n-1} a_n}{d_n} \leq x < \frac{p_{n-1} + 1}{d_{n-1}} = \frac{p_{n-1} a_n + a_n}{d_n}
$$

d’où $a_n p_{n-1} \leq p_n < a_n p_{n-1} + a_n$, et par suite $r_{n-1} \leq r_n \leq x$. On pose

$$
p_n = a_n p_{n-1} + u_n
$$

et on a $0 \leq u_n < a_n$, ce qui équivaut à $0 \leq u_n \leq a_n - 1$, puisque $u_n$ est entier.

On en tire

(3) $$
r_n = r_{n-1} + \frac{u_n}{d_n} = p_0 + \sum_{k=1}^n \frac{u_k}{d_k}
$$
et, comme $x = \lim_{n \to \infty} r_n$,

(4) $$
x = p_0 + \sum_{n=1}^\infty \frac{u_n}{d_n}.
$$

La série qui figure au second membre de (4) et dont $x$ est la somme, est appelée le *développement de x relatif à la suite de base* ($d_n$). Tous les coefficients $u_n$ sont $\geqslant 0$; $p_0$ est, par définition, le plus grand entier $p$ tel que $p \leqslant x$; on l’appelle *partie entière de x*, et on le désigne souvent par la notation $[x]$.

### 3. Définition d’un nombre réel par son développement

Réciproquement, donnons-nous un entier $q_0$, et une suite $(v_n)$ ($n \geqslant 1$) d’entiers tels que $0 \leqslant v_n \leqslant a_n - 1$, et cherchons s’il existe un nombre $x$ dont le développement (4) soit tel que $p_0 = q_0$, $u_n = v_n$ quel que soit $n$. Si ce nombre existe, il est *unique*, étant égal à $q_0 + \sum_{n=1}^\infty \frac{v_n}{d_n}$.

Pour tout entier $m > 0$, on a (principe de comparaison)

$$
\sum_{n=m+1}^\infty \frac{v_n}{d_n} \leqslant \sum_{n=m+1}^\infty \frac{a_n - 1}{d_n} = \sum_{n=m+1}^\infty \left( \frac{1}{d_{n-1}} - \frac{1}{d_n} \right) = \frac{1}{d_m}
$$

et les deux membres extrêmes ne sont égaux que si $v_n = a_n - 1$ pour tout $n > m$ (IV, p. 33, th. 2). Donc la série de terme général $\frac{v_n}{d_n}$ est convergente; en outre, si $x = q_0 + \sum_{n=1}^\infty \frac{v_n}{d_n}$, on a

$$
s_m = q_0 + \sum_{n=1}^m \frac{v_n}{d_n} \leqslant x \leqslant s_m + \frac{1}{d_m}
$$

et on ne peut avoir $x = s_m + \frac{1}{d_m}$ que si $v_n = a_n - 1$ quel que soit $n > m$. Comme $s_m$ est une fraction de dénominateur $d_m$, la valeur approchée $r_m$ de $x$ à $1/d_m$ près par défaut est égale à $s_m$ ou à $s_m + \frac{1}{d_m}$; et ce dernier cas ne peut se produire que si $v_n = a_n - 1$ pour tout $n > m$. Nous sommes ainsi amenés à distinguer deux cas:

1° Il existe une *infinité* de valeurs de $n$ telles que $v_n < a_n - 1$: la série $q_0 + \sum_{n=1}^\infty \frac{v_n}{d_n}$ est alors identique au développement de sa somme $x$.

2° Il existe un entier $m \geqslant 0$ tel que $v_n = a_n - 1$ pour $n > m$, et $v_m < a_m - 1$ (si $m > 0$) ; alors la somme $x$ de la série $q_0 + \sum_{n=1}^{\infty} \frac{v_n}{d_n}$ est égale au nombre rationnel

$$
q_0 + \sum_{n=1}^{m} \frac{v_n}{d_n} + \frac{1}{d_m}
$$

qui est de la forme $k/d_m$ ($k$ entier) ; le *développement* de $x$ est identique à la série (5), dont tous les termes d’indices $> m$ sont nuls ; on dit qu’un tel développement est *limité*. La série

$$
q_0 + \sum_{n=1}^{\infty} \frac{v_n}{d_n} = q_0 + \sum_{n=1}^{m} \frac{v_n}{d_n} + \sum_{n=m+1}^{\infty} \frac{a_n - 1}{d_n}
$$

est appelée le *développement impropre* du nombre $x$.

Inversement, soit $x$ un nombre rationnel qui peut se mettre sous forme d’une fraction de dénominateur $d_n$ pour une valeur de $n$; soit $m$ le plus petit entier tel que $x$ soit de la forme $k/d_m$ ($k$ entier) ; on a $r_n < x$ pour $n < m$, et $r_m = x$, donc le développement de $x$ est de la forme (5), et $x$ a un développement impropre, donné par la formule (6) ; ce développement impropre est d’ailleurs *unique*.

Pour qu’un nombre rationnel, mis sous forme irréductible $p/q$, soit égal à une fraction de dénominateur $d_m$, il faut et il suffit que $q$ *divise* $d_m$ (le nombre $m$ sera alors le plus petit entier $n$ tel que $q$ divise $d_n$). Il peut se faire que *tout nombre rationnel* ait cette propriété (pour un $n$ convenablement choisi) : il faut et il suffit pour cela que tout entier $> 0$ divise un $d_n$; ce sera par exemple le cas si $d_n = n!$. Si les $d_n$ ont cette propriété, pour qu’un nombre soit rationnel, il faut et il suffit que son développement relatif à la suite $(d_n)$ soit limité.

En résumé, à toute suite $s$ dont le premier terme $q_0$ est un entier quelconque, et dont le terme $v_n$ ($n \geqslant 1$) est tel que $0 \leqslant v_n \leqslant a_n - 1$, correspond un nombre réel égal à $q_0 + \sum_{n=1}^{\infty} \frac{v_n}{d_n}$; si $I_n$ désigne l’intervalle $(0, a_n - 1)$ de $\mathbf{N}$, on définit ainsi une application $\varphi$ de $E = \mathbf{Z} \times \prod_{n=1}^{\infty} I_n$ sur la droite numérique $\mathbf{R}$; en outre l’équation $\varphi(s) = x$, où $x \in \mathbf{R}$ est donné, a *une* solution si $x$ n’est pas une fraction de dénominateur $d_n$ (pour un $n$ convenable), et *deux* solutions dans le cas contraire.

### 4. Comparaison des développements

La connaissance des développements de deux nombres réels distincts $x, y$, permet de déterminer si $x < y$ ou si $x > y$.

En effet, soient $x = p_0 + \sum_{n=1}^{\infty} \frac{u_n}{d_n}$, $y = q_0 + \sum_{n=1}^{\infty} \frac{v_n}{d_n}$ les développements de $x$ et $y$. Si $p_0 < q_0$, on a $x < y$, car

$$
p_0 \leqslant x < p_0 + 1 \leqslant q_0 \leqslant y.
$$

Plus généralement, supposons que $p_0 = q_0$, et $u_n = v_n$ pour $1 \leq n < m$, mais que $u_m < v_m$; si

$$
r_n = p_0 + \sum_{k=1}^n \frac{u_k}{d_k}, \quad s_n = q_0 + \sum_{k=1}^n \frac{v_k}{d_k},
$$

on a $r_n = s_n$ pour $n < m$, et, comme $u_m + 1 \leq v_m$, $r_m + \frac{1}{d_m} \leq s_m$; mais $r_m \leq x < r_m + \frac{1}{d_m} \leq s_m \leq y$, donc on a encore $x < y$. Autrement dit, l’ordre de $x$ et $y$ est le même que celui des deux premiers termes distincts de leurs développements respectifs.

Il en résulte que, si $p_0 = q_0$ et $u_n = v_n$ pour $n < m$, les $m$ premiers termes du développement de tout nombre $z$ appartenant à l’intervalle fermé d’extrémités $x$ et $y$ sont les mêmes que ceux des développements de $x$ et $y$.

On remarquera aussi que, dans ce cas, on a $|y - x| \leq \frac{1}{d_{m-1}}$. Si on munit $\mathbf{Z}$ et les intervalles $I_n$ de la topologie discrète, on peut donc dire que l’application $\varphi$ définie ci-dessus est continue dans l’espace produit $E$.

### 5. Développements de base a

Les suites de base les plus importantes sont celles où $d_n = a^n$, $a$ étant un entier $> 1$; on dit alors que $a$ est le nombre de base (ou simplement la base) des développements correspondants. Pour les calculs numériques manuels, on emploie les développements de base 10, qui sont dits développements décimaux; dans les calculs sur ordinateurs, on utilise le plus souvent les développements de base 2 (dits développements dyadiques).

Pour représenter les valeurs approchées par défaut $r_n$ d’un nombre $x \geq 0$, dans son développement de base $a$, on se sert du symbolisme suivant: on désigne chaque entier $u$ tel que $0 \leq u \leq a - 1$ par un signe particulier; si

$$
r_n = p_0 + \sum_{k=1}^n \frac{u_k}{d_k},
$$

on écrit d’abord, à l’aide de ces signes, le développement de base $a$ de l’entier positif $p_0 = [x]$ (E, III, p. 40), puis on place une virgule, et on écrit ensuite successivement les signes représentant les nombres $u_1, u_2, \ldots, u_n$. Si S est le symbole ainsi obtenu, on écrit souvent, par abus de langage, $x = S \ldots$; il doit être entendu une fois pour toutes qu’une telle relation n’est qu’une manière abrégée d’indiquer que le second membre est la valeur approchée de $x$ à $1/a^n$ près par défaut.

Pour les nombres négatifs, l’usage établi est différent: on écrit, dans le symbolisme précédent, une valeur approchée de $x' = -x \geq 0$, en le faisant précéder du signe «−»; c’est donc en réalité une valeur approchée de $x$ par excès à $1/a^n$ près qu’on désigne ainsi.

Cette manière de faire ne laisse pas de présenter des inconvénients pour le calcul numérique; et pour la notation des logarithmes négatifs, on adopte le même symbolisme que pour les nombres positifs, en surlignant simplement la partie entière, pour indiquer qu’elle est égale à l’opposé du nombre écrit.

### 6. Cardinal de R

On a $\mathbf{R} = \bigcup_{n \in \mathbf{Z}} [n, n+1[$, et tous les intervalles $[n, n+1[$ sont équipotents à $[0, 1[$; comme $[0, 1[$ est un ensemble infini, on en conclut (E, III, p. 49, cor. 3) que $\mathbf{R}$ est équipotent à l’intervalle $[0, 1[$. En considérant le développement dyadique des nombres de l’intervalle $[0, 1[$, nous allons montrer que cet intervalle est équipotent à l’ensemble S de toutes les suites $(u_n)$ dont les termes sont égaux à 0 ou à 1.

Tout d’abord, il est équipotent au sous-ensemble S’ de S formé des suites $(u_n)$ telles que $u_n \neq 0$ pour une infinité de valeurs de $n$ (IV, p. 42). D’autre part, l’ensemble S” complémentaire de S’ dans S, est équipotent à l’ensemble des développements impropres des nombres rationnels égaux à une fraction de dénominateur $2^n$; comme ces nombres forment une partie de $\mathbf{Q}$, leur ensemble est dénombrable, donc aussi S”. Comme S’ est infini, il est équipotent à S (E, III, p. 49, cor. 4), d’où la proposition.

Remarquons maintenant que S est équipotent à $\mathfrak{P}(\mathbf{N})$; en effet, on définit une application bijective de $\mathfrak{P}(\mathbf{N})$ sur S, en faisant correspondre à toute partie X de $\mathbf{N}$ la suite $(u_n)$ telle que $u_n = 0$ pour $n \in X$, et $u_n = 1$ pour $n \notin X$.

Nous avons finalement démontré le théorème suivant:

#### Théorème 1 (Cantor) {#top-iv-s8-thm-1 .statement}

L’ensemble des nombres réels est équipotent à l’ensemble des parties d’un ensemble infini dénombrable.

#### Corollaire {#top-iv-s8-n6-cor-1 .statement}

L’ensemble des nombres réels a une puissance strictement supérieure à celle d’un ensemble dénombrable.

On dit qu’un ensemble équipotent à $\mathbf{R}$ a la puissance du continu. D’après la prop. 1 de IV, p. 13, tout intervalle non réduit à un point a la puissance du continu; le complémentaire d’une partie dénombrable de $\mathbf{R}$ a la puissance du continu (E, III, p. 49, cor. 4); en particulier, l’ensemble des nombres irrationnels a la puissance du continu.

Exercises

## EXERCICES {#top-iv-s8-exercises}

See the [exercises for § 8](exercises/s8/).
