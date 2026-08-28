---
book: int
book_title: Integration
chapter: I
chapter_title: Inégalités de convexité
section: 0
section_title: Inégalités de convexité
kind: front
lang: fr
source: int-i-iv-fr
pdf_pages: 0013-0018
extraction: ocr
subsections:
    - "no": 1
      title: L’inégalité fondamentale de convexité
      page: 0
      pdf_page: 13
    - "no": 2
      title: Les inégalités de Hölder et de Minkowski
      page: 0
      pdf_page: 15
    - "no": 3
      title: Les semi-normes $N_p$
      page: 0
      pdf_page: 16
statements: 0
exercises: 0
content_sha256: 750573dc1b78042da94b5170de3eeaa68556c47ddaef22f45ce3409e701e20d2
---

## CHAPITRE I

# INÉGALITÉS DE CONVEXITÉ

### 1. L’inégalité fondamentale de convexité

Soit X un ensemble; dans l’espace vectoriel $\mathbf{R}^X$ de toutes les fonctions numériques finies, définies dans X, soit P l’ensemble de toutes les fonctions numériques positives dans X. Soit d’autre part $M$ une fonction numérique finie ou non, à valeurs $\geqslant 0$, définie dans P, et telle que:

$1^\circ$ $M(0) = 0$, et $M$ est positivement homogène, c’est-à-dire que, pour tout nombre réel $\lambda$ fini et $> 0$, $M(\lambda f) = \lambda M(f)$.

$2^\circ$ $M$ est croissante dans P, autrement dit, la relation $f \leqslant g$ entraîne $M(f) \leqslant M(g)$.

$3^\circ$ $M$ est convexe dans P, autrement dit (\emph{Esp. vect. top.}, chap. II, 2e éd., § 2, n° 8) satisfait à la relation $M(f + g) \leqslant M(f) + M(g)$.

\emph{Exemple.} — Supposons que X soit un ensemble fini, par exemple l’intervalle $[1, n]$ de $\mathbf{N}$; en désignant par $x_i$ ($1 \leqslant i \leqslant n$) les coordonnées d’un vecteur $x \in \mathbf{R}^n$, les fonctions $M_1(x) = \sum_{i=1}^n x_i$ et $M_\infty(x) = \sup_{1 \leqslant i \leqslant n} x_i$ satisfont aux conditions précédentes dans l’ensemble P des x de coordonnées $\geqslant 0$.

\emph{Remarque.} — Soit S un cône convexe pointé contenu dans P (c’est-à-dire un ensemble tel que $S + S \subset S$ et $\lambda S \subset S$ pour $\lambda > 0$; cf. \emph{Esp. vect. top.}, chap. II, 2e éd., § 2, n° 4); soit $M$ une fonction numérique finie ou non, à valeurs $\geqslant 0$, définie dans S et satisfaisant dans S aux conditions $1^\circ$, $2^\circ$ et $3^\circ$ ci-dessus. On peut alors prolonger $M$ à l’ensemble P tout entier, de façon que la fonction prolongée (que nous noterons encore $M$) satisfasse aux mêmes conditions: il suffit, pour toute fonction $f \in P$, de poser $M(f) = +\infty$ s’il n’existe aucune fonction $g \in S$ telle que $f \leqslant g$, et $M(f) = \inf_{g \in S, f \leqslant g} M(g)$ dans le cas contraire. Ce procédé sera appliqué au chap. IV, § 1, pour définir l’intégrale supérieure d’une fonction positive.

PROPOSITION 1. — Soit $\varphi(t_1, t_2, \ldots, t_n)$ une fonction numérique finie, définie et continue pour $t_i \geq 0$ ($1 \leq i \leq n$), et telle que :
1° les relations $t_i > 0$ ($1 \leq i \leq n$) entraînent $\varphi(t_1, t_2, \ldots, t_n) > 0$;
2° la fonction $\varphi$ est positivement homogène;
3° l’ensemble $K \subset \mathbf{R}^n$ défini par les relations $t_i \geq 0$ ($1 \leq i \leq n$), $\varphi(t_1, t_2, \ldots, t_n) \geq 1$, est convexe.
Dans ces conditions, si $f_1, f_2, \ldots, f_n$ sont $n$ fonctions finies et $\geq 0$, définies dans $X$, et telles que $M(f_i) < +\infty$ pour $1 \leq i \leq n$, on a
$$
M(\varphi(f_1, f_2, \ldots, f_n)) \leq \varphi(M(f_1), M(f_2), \ldots, M(f_n)).
$$
On sait en effet, en vertu du th. de Hahn-Banach (*Esp. vect. top.*, chap. II, 2e éd., § 5) que $K$ est l’intersection des $n$ demi-espaces $t_i \geq 0$ ($1 \leq i \leq n$) et d’une famille de demi-espaces fermés $(U_\iota)_{\iota \in I}$, $U_\iota$ étant défini par une relation de la forme
$$
\alpha_{\iota 1} t_1 + \alpha_{\iota 2} t_2 + \cdots + \alpha_{\iota n} t_n - \beta_\iota \geq 0
$$
où les $\alpha_{\iota k}$ ne sont pas tous nuls. Par hypothèse, si $t = (t_i)$ est tel que $t_i > 0$ pour $1 \leq i \leq n$, on a $\varphi(t_1, \ldots, t_n) > 0$, donc il existe $\lambda_0 > 0$ tel que la relation $\lambda \geq \lambda_0$ entraîne $\lambda t \in K$; cela montre que, pour chaque $\iota \in I$, les relations $t_i \geq 0$ ($1 \leq i \leq n$) entraînent $\alpha_{\iota 1} t_1 + \cdots + \alpha_{\iota n} t_n \geq 0$, et par suite qu’on a $\alpha_{\iota k} \geq 0$ pour $1 \leq k \leq n$; il est clair alors que $K$ est aussi l’intersection des demi-espaces $t_i \geq 0$ ($1 \leq i \leq n$) et des $U_\iota$ tels que $\beta_\iota \geq 0$; en outre, comme l’origine n’appartient pas à $K$, il existe au moins un indice $\iota$ tel que $\beta_\iota > 0$.
Soit alors $C$ le cône convexe dans $\mathbf{R}^{n+1}$ défini par les relations $t_i \geq 0$ ($1 \leq i \leq n+1$), $t_{n+1} \leq \varphi(t_1, t_2, \ldots, t_n)$ (adhérence du cône convexe engendré dans $\mathbf{R}^{n+1}$ par l’ensemble convexe $K \times \{1\}$); il est immédiat que $C$ est aussi défini par les relations $t_i \geq 0$ ($1 \leq i \leq n+1$) et
$$
\beta_\iota t_{n+1} \leq \alpha_{\iota 1} t_1 + \cdots + \alpha_{\iota n} t_n \quad (\iota \in I, \beta_\iota \geq 0).
$$
Pour tout $x \in E$, on a donc
$$
\beta_\iota \varphi(f_1(x), \ldots, f_n(x)) \leq \alpha_{\iota 1} f_1(x) + \cdots + \alpha_{\iota n} f_n(x)
$$
pour tout $\iota \in I$. Pour tout indice $\iota$ tel que $\beta_\iota > 0$, il résulte de (4) et des hypothèses sur $M$ que $M(\varphi(f_1, f_2, \ldots, f_n))$ est fini et qu’on a
$$
\beta_\iota M(\varphi(f_1, f_2, \ldots, f_n)) \leq \alpha_{\iota 1} M(f_1) + \alpha_{\iota 2} M(f_2) + \cdots + \alpha_{\iota n} M(f_n)
$$
et cette relation est aussi vérifiée de façon évidente si $\beta_\iota = 0$.
On voit donc que le point de coordonnées $M(f_1), M(f_2), \ldots, M(f_n), M(\varphi(f_1, f_2, \ldots, f_n))$ appartient à $C$, ce qui démontre la proposition.

### 2. Les inégalités de Hölder et de Minkowski

Dans ce numéro et le suivant, X et P ont la même signification que dans le n° 1, et $M$ désigne une fonction définie dans P et satisfaisant aux conditions énumérées au n° 1.

PROPOSITION 2. — Soient $\alpha$ et $\beta$ deux nombres tels que $0 < \alpha < 1,\ 0 < \beta < 1,\ \alpha + \beta = 1$. Si $f$ et $g$ sont deux fonctions finies et $\geqslant 0$, définies dans X, et si $M(f)$ et $M(g)$ sont finis, on a
$$
M(f^\alpha g^\beta) \leqslant (M(f))^\alpha (M(g))^\beta
$$
(inégalité de Hölder).

D’après la prop. 1, tout revient à prouver que, dans $\mathbf{R}^2$, l’ensemble défini par les relations $t_1 \geqslant 0,\ t_2 \geqslant 0,\ t_1^\alpha t_2^\beta \geqslant 1$ est convexe, ou encore (Fonct. var. réelle, chap. I, §4, n° 1, déf. 1) que la fonction $u(t) = t^{-\alpha/\beta}$ est convexe pour $0 < t < +\infty$. Or, en posant $r = \alpha/\beta$, on a $D^2u(t) = r(r+1)t^{-r-2}$, et comme $r > 0,\ D^2u(t) > 0$ dans $]0, +\infty[$, ce que démontre la proposition (Fonct. var. réelle, chap. I, § 4, n° 4, cor. de la prop. 8).

COROLLAIRE. — Soient $\alpha_i$ ($1 \leqslant i \leqslant n$) n nombres $\geqslant 0$ tels que $\sum_{i=1}^n \alpha_i = 1,\ f_i$ ($1 \leqslant i \leqslant n$) n fonctions finies et $\geqslant 0$, définies dans X et telles que $M(f_i)$ soit fini pour $1 \leqslant i \leqslant n$. Dans ces conditions, on a
$$
M(f_1^{\alpha_1} f_2^{\alpha_2} \ldots f_n^{\alpha_n}) \leqslant (M(f_1))^{\alpha_1} (M(f_2))^{\alpha_2} \ldots (M(f_n))^{\alpha_n}.
$$
On peut se borner au cas où $\alpha_i > 0$ pour tout $i$. Il suffit de raisonner par récurrence sur $n$, en appliquant l’inégalité (5) aux nombres $\alpha = \alpha_1$ et $\beta = \sum_{i=2}^n \alpha_i$, et aux fonctions
$$
f = f_1,\quad g = (f_2^{\alpha_2} f_3^{\alpha_3} \ldots f_n^{\alpha_n})^{1/\beta}.
$$

PROPOSITION 3. — Soit $p$ un nombre fini et $\geqslant 1$. Si $f$ et $g$ sont deux fonctions finies et $\geqslant 0$, définies dans X, on a
$$
(M((f + g)^p))^{1/p} \leqslant (M(f^p))^{1/p} + (M(g^p))^{1/p}
$$
(inégalité de Minkowski).

On peut se borner au cas où $M(f^p)$ et $M(g^p)$ sont finis. D’après la prop. 1, tout revient à prouver que, dans $\mathbf{R}^2$, l’ensemble défini par les relations $t_1 \geqslant 0,\ t_2 \geqslant 0,\ t_1^{1/p} + t_2^{1/p} \geqslant 1$ est convexe, ou encore que la fonction $u(t) = (1 - t^{1/p})^p$ est convexe pour $0 \leq t \leq 1$. Or, on a
$$
D^2 u(t) = \left(1 - \frac{1}{p}\right)t^{1/p-2} \left(1 - t^{1/p}\right)^{p-2} \geq 0
$$
pour $0 < t \leq 1$, d’où la proposition.

### 3. Les semi-normes $N_p$

Soit $p$ un nombre réel fini et $\geq 1$, et soit $\mathcal{F}^p(X, M)$ l’ensemble des fonctions numériques finies $f$, définies dans $X$ et telles que $M(|f|^p)$ soit *fini*. Il est évident que, si $g$ est une fonction appartenant à $\mathcal{F}^p(X, M)$, et si $|f| \leq |g|$, $f$ appartient aussi à $\mathcal{F}^p(X, M)$; cette remarque et l’inégalité de Minkowski montrent que la somme de deux fonctions de $\mathcal{F}^p(X, M)$ appartient encore à cet ensemble ; compte tenu du fait que $M$ est positivement homogène on voit donc que $\mathcal{F}^p(X, M)$ est un *sous-espace vectoriel* de l’espace $\mathbf{R}^X$ de toutes les fonctions numérique finies définies dans $X$.

Pour tout nombre $p > 0$ et toute fonction numérique finie $f$ définie dans $X$, on pose
$$
N_p(f) = (M(|f|^p))^{1/p};
$$
on a $N_p(\lambda f) = |\lambda| N_p(f)$ pour tout scalaire $\lambda$; en outre, si $p \geq 1$, on a, d’après (7)
$$
N_p(f + g) \leq N_p(f) + N_p(g)
$$
ce qui prouve que $N_p$ est une *semi-norme* sur l’espace vectoriel $\mathcal{F}^p(X, M)$ (*Esp. vect. top.*, chap. II, 2e éd., § 1).

**Proposition 4.** — *Soient* $p$ *et* $q$ *deux nombres finis et* $> 0$, *et posons* $1/r = 1/p + 1/q$. *Quelles que soient les fonctions numériques finies* $f, g$ *définies dans* $X$, *on a*
$$
N_r(fg) \leq N_p(f) N_q(g),
$$
*si* $N_p(f)$ *et* $N_q(g)$ *sont finis*.

En effet, la relation (9) s’écrit
$$
M(|f|^r |g|^r) \leq (M(|f|^p))^{r/p} (M(|g|^q))^{r/q}
$$
et n’est autre que l’inégalité de Hölder (5) appliquée aux nombres $\alpha = r/p$ et $\beta = r/q$ et aux fonctions $|f|^p$ et $|g|^q$.

COROLLAIRE. — *On suppose que* $M(1) = 1$; *alors, pour toute fonction numérique finie* $f$, *définie dans* $X$, *l’application* $p \mapsto N_p(f)$ *est croissante dans* $]0, +\infty[$.

En effet, en appliquant l’inégalité (9) au cas où $g = 1$, on voit que $N_r(f) \leq N_p(f)$ quel que soit $q > 0$; comme le nombre $r$ défini par $1/r = 1/p + 1/q$ parcourt l’ensemble des nombres tels que $0 < r < p$ lorsque $q$ parcourt l’ensemble des nombres $> 0$, le corollaire est démontré.

PROPOSITION 5. — *Pour toute fonction numérique finie* $f$ *définie dans* $X$, *l’ensemble* $I$ *des valeurs de* $1/p$ ($p > 0$) *telles que* $N_p(f)$ *soit fini est vide ou est un intervalle ; si* $I$ *n’est pas réduit à un point, l’application* $\alpha \mapsto \log N_{1/\alpha}(f)$ *est convexe dans* $I$, *ou égale à* $-\infty$ *dans l’intérieur de* $I$.

Soient $r$ et $s$ deux nombres $> 0$ distincts et tels que $1/r$ et $1/s$ appartiennent à $I$; tout revient à prouver que, si

$$
\frac{1}{p} = \frac{t}{r} + \frac{1-t}{s},
$$

avec $0 < t < 1$, on a

$$
\log N_p(f) \leq t \cdot \log N_r(f) + (1-t) \log N_s(f)
$$

ou, ce qui revient au même,

$$
N_p(f) \leq (N_r(f))^t (N_s(f))^{1-t}
$$

relation qui s’écrit, d’après la définition de $N_p$,

$$
M(|f|^p) \leq (M(|f|^r))^{tp/r} (M(|f|^s))^{(1-t)p/s}.
$$

Si on pose $\alpha = tp/r$, on a $1-\alpha = (1-t)p/s$, d’après la relation qui définit $p$ en fonction de $t, r, s$; d’où $p = \alpha r + (1-\alpha)s$. Or, l’inégalité de Hölder donne

$$
M(|f|^{r\alpha}|f|^{s(1-\alpha)}) \leq (M(|f|^r))^\alpha (M(|f|^s))^{1-\alpha}
$$

ce qui n’est autre que l’inégalité (12).

EXERCICES

1) Avec les hypothèses du n° 1, montrer que l’ensemble des fonctions bornées dans $X$ et telles que $M(|f|)$ soit fini, est une sous-algèbre $A$ de $\mathbf{R}^X$, et que l’ensemble des fonctions bornées dans $X$ et telles que $M(|f|) = 0$ est un idéal dans $A$. Si en outre $M(1)$ est fini, montrer que l’application $f \mapsto M(f)$ est continue quand on munit $A$ de la topologie de la convergence uniforme dans $X$.

2) Soient X l’intervalle $[0, +\infty[$ de $\mathbf{R}$, S le cône convexe formé des fonctions définies dans X et telles que $0 \leq f(x) \leq kx$ dans X (pour un nombre fini $k > 0$ dépendant de $f$). On pose $M(f) = 0$ pour $f \in S$, et $M(f) = +\infty$ pour toute fonction positive $f$ définie dans X et n’appartenant pas à S. Montrer que $M$ satisfait aux conditions du n° 1, et qu’on a $M(x) = 0$, et $M(x^r) = +\infty$ pour tout nombre $r > 0$ distinct de 1.

3) Donner un exemple où X est un ensemble de deux éléments, où $N_p(x)$ est fini pour tout $p > 0$ et tout $x \in \mathbf{R}^2$, mais où il existe des valeurs de $p$ telles que l’application $p \mapsto N_p(x)$ ne soit pas dérivable en ces points.

4) Déduire l’inégalité (6) de l’inégalité de la moyenne géométrique
$$
z_1^{\alpha_1} z_2^{\alpha_2} \cdots z_n^{\alpha_n} \leq \alpha_1 z_1 + \cdots + \alpha_n z_n \quad (\text{où } \sum_{i=1}^n \alpha_i = 1)
$$
(Fonct. var. réelle, chap. III, §1, n° 1, prop. 2) (se ramener au cas où $M(f_i) = 1$ pour $1 \leq i \leq n$).

5) Soit $\alpha$ un nombre réel $> 1$, et soit $\beta = 1 - \alpha < 0$. Soit g une fonction finie, définie dans X, telle que $g(x) > 0$ pour tout $x \in X$ et que $M(g) > 0$; montrer que pour toute fonction $f$ finie et $\geq 0$ définie dans X, et telle que $M(f)$ soit fini, on a
$$
M(f^\alpha g^\beta) \geq (M(f))^\alpha (M(g))^\beta
$$
(appliquer convenablement l’inégalité de Hölder).

6) Déduire l’inégalité de Minkowski de l’inégalité de Hölder (majorer $M(f(f+g)^{p-1})$ à l’aide de l’inégalité de Hölder). Si l’on suppose que $M(f+g) = M(f) + M(g)$ pour tout couple de fonctions $f, g$, définies et $\geq 0$ dans X, déduire de même de l’exerc. 5 l’inégalité
$$
(M((f+g)^p))^{1/p} \geq (M(f^p))^{1/p} + (M(g^p))^{1/p}
$$
dans les cas suivants: a) $0 < p < 1$, $f$ et $g$ fonctions finies et $\geq 0$ définies dans X, telles que $f(x) + g(x) > 0$ pour tout $x \in X$ et que $M(f^p)$ et $M(g^p)$ soient finis; b) $p < 0$, $f$ et $g$ fonctions finies, définies dans X, telles que $f(x) > 0$ et $g(x) > 0$ pour tout $x \in X$, que $M(f^p)$ et $M(g^p)$ soient finis et $M((f+g)^p) > 0$.
