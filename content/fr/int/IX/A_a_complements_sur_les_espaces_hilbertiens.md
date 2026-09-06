---
book: int
book_title: Integration
chapter: IX
chapter_title: MESURES SUR LES ESPACES TOPOLOGIQUES SÉPARÉS
section: 0
section_title: Compléments sur les espaces hilbertiens
appendix: true
lang: fr
source: int-ix-fr
pdf_pages: 0094-0098, 0108-0110
extraction: ocr
subsections:
    - "no": 1
      title: Trace d'une forme quadratique par rapport à une autre
      page: 0
      pdf_page: 94
    - "no": 2
      title: Applications de Hilbert–Schmidt
      page: 0
      pdf_page: 96
statements: 5
exercises: 9
content_sha256: aced91e0475cbcf3beb48a3c7f719e9a57b6702f2fcd9454db892c456fc7358e
---

## ANNEXE

# COMPLÉMENTS SUR LES ESPACES HILBERTIENS

### 1. Trace d'une forme quadratique par rapport à une autre

Dans ce n°, on note E un espace vectoriel réel et Q, H deux formes quadratiques positives sur E. Il existe deux formes bilinéaires symétriques $(x, y) \mapsto (x|y)_Q$ et $(x, y) \mapsto (x|y)_H$ caractérisées par
$$
Q(x) = (x|x)_Q, \quad H(x) = (x|x)_H
$$
pour tout $x \in E$.

On appelle trace de Q par rapport à H, et l'on note $\operatorname{Tr}(Q/H)$ le nombre réel positif, fini ou non, défini comme suit:
a) S'il existe $x \in E$ avec $H(x) = 0$ et $Q(x) \neq 0$, on pose $\operatorname{Tr}(Q/H) = +\infty$.
b) Dans le cas contraire, $\operatorname{Tr}(Q/H)$ est la borne supérieure de l'ensemble des nombres de la forme $\sum_{i=1}^p Q(e_i)$ où $(e_1, \ldots, e_p)$ parcourt l'ensemble des suites finies d'éléments de E orthonormales pour H.

Soient E un espace hilbertien réel et Q une forme quadratique positive sur E. Posons $H(x) = \|x\|^2$ pour tout $x \in E$; alors H est une forme quadratique positive sur E. On dit que Q est nucléaire si $\operatorname{Tr}(Q/H)$ est fini. Pour tout $x \in E$ de norme 1, on a $Q(x) \leq \operatorname{Tr}(Q/H)$, d'où $Q \leq \operatorname{Tr}(Q/H).H$; en particulier toute forme nucléaire Q est continue.

#### Remarque 1 {#int-ix-a0-n1-rem-1 .statement}

Pour tout sous-espace F de E, notons $Q_F$ la restriction de Q à F et $H_F$ celle de H. On a $\operatorname{Tr}(Q_F/H_F) \leq \operatorname{Tr}(Q/H)$ et $\operatorname{Tr}(Q/H)$ est la borne supérieure des nombres $\operatorname{Tr}(Q_F/H_F)$ pour $F \subset E$ de dimension finie.

#### Remarque 2 {#int-ix-a0-n1-rem-2 .statement}

Soient $E_1$ un espace vectoriel réel, $Q_1$ et $H_1$ deux formes quadratiques positives sur $E_1$ et $\pi : E \to E_1$ une application linéaire surjective. Si $Q = Q_1 \circ \pi$ et $H = H_1 \circ \pi$, on a $\operatorname{Tr}(Q/H) = \operatorname{Tr}(Q_1/H_1)$.

#### Proposition 1 {#int-ix-a0-prop-1 .statement}

On suppose que E est de dimension finie et H non dégénérée.
a) Il existe un endomorphisme u de E caractérisé par $(x|y)_Q = (u(x)|y)_H$ pour $x, y$ dans E.
b) On a $\operatorname{Tr}(Q/H) = \operatorname{Tr}(u)$.
c) On a $\operatorname{Tr}(Q/H) = \sum_{i=1}^m Q(e_i)$ pour toute base $(e_1, \ldots, e_m)$ de E orthonormale pour H.

a) résulte de ce que la forme bilinéaire $(x, y) \mapsto (x|y)_\mathbf{H}$ est non dégénérée. Toute suite orthonormale pour $\mathbf{H}$ dans $E$ peut être complétée en une base de $E$ orthonormale pour $\mathbf{H}$. Par suite, $\operatorname{Tr}(Q/\mathbf{H})$ est la borne supérieure de l’ensemble des nombres de la forme $\sum_{i=1}^m Q(e_i)$ pour toutes les bases $(e_1, \ldots, e_m)$ de $E$ orthonormales pour $\mathbf{H}$. Pour prouver b) et c), il suffit de montrer que l’on a $\sum_{i=1}^m Q(e_i) = \operatorname{Tr}(u)$ pour toute base de cette sorte. Posons $a_{ij} = (u(e_i)|e_j)_\mathbf{H} = (e_i|e_j)_Q$ pour $1 \leq i, j \leq m$; on a $u(e_i) = \sum_{j=1}^m a_{ij} e_j$ pour $1 \leq i \leq m$, d’où

$$
\operatorname{Tr}(u) = \sum_{i=1}^m a_{ii} = \sum_{i=1}^m (e_i|e_i)_Q = \sum_{i=1}^m Q(e_i).
$$

C.Q.F.D.

#### Proposition 2 {#int-ix-a0-prop-2 .statement}

*On suppose que* $E$ *est de dimension finie. Il existe une base* $(e_1, \ldots, e_n)$ *de* $E$ *et un entier* $m$ *avec* $0 \leq m \leq n$ *tels que*

$$(1)$$
$$
\mathbf{H}\left( \sum_{i=1}^n t_i e_i \right) = \sum_{i=1}^m t_i^2
$$
*pour* $t_1, \ldots, t_n$ *réels. Si, de plus, la relation* $\mathbf{H}(x) = 0$ *entraîne* $Q(x) = 0$ *pour tout* $x \in E$, *on a* $\operatorname{Tr}(Q/\mathbf{H}) = \sum_{i=1}^m Q(e_i)$.

Il existe une base orthogonale $(e'_1, \ldots, e'_n)$ de $E$ pour $\mathbf{H}$. On peut supposer cette base numérotée de sorte que l’on ait $\mathbf{H}(e'_i) > 0$ pour $1 \leq i \leq m$ et $\mathbf{H}(e'_i) = 0$ pour $m < i \leq n$. On posera alors $e_i = e'_i / \mathbf{H}(e'_i)^{1/2}$ pour $1 \leq i \leq m$ et $e_i = e'_i$ pour $m < i \leq n$; la relation (1) est vérifiée.

Soit $F$ le sous-espace de $E$ engendré par $e'_{m+1}, \ldots, e'_n$; c’est l’ensemble des $x \in E$ tels que $\mathbf{H}(x) = 0$. On note $\pi$ l’application canonique de $E$ sur $E_1 = E/F$. Comme $Q$ et $\mathbf{H}$ sont nulles sur $F$, il existe deux formes quadratiques positives $Q_1$ et $\mathbf{H}_1$ sur $E_1$ telles que $Q = Q_1 \circ \pi$ et $\mathbf{H} = \mathbf{H}_1 \circ \pi$. De plus, $(\pi(e_1), \ldots, \pi(e_m))$ est une base de $E_1$, orthonormale pour $\mathbf{H}_1$ et $\mathbf{H}_1$ est donc non dégénérée.

D’après la prop. 1 et la *Remarque* 2, on a

$$
\operatorname{Tr}(Q/\mathbf{H}) = \operatorname{Tr}(Q_1/\mathbf{H}_1) = \sum_{i=1}^m Q_1(\pi(e_i)) = \sum_{i=1}^m Q(e_i).
$$

C.Q.F.D.

*Remarque 3).* — Supposons $E$ de dimension finie et $\mathbf{H}$ non dégénérée. Soit $(e_1, \ldots, e_n)$ une base de $E$. On pose $q = ((e_i|e_j)_Q)_{1 \leq i, j \leq n}$ et $h = ((e_i|e_j)_\mathbf{H})_{1 \leq i, j \leq n}$. Avec les notations de la prop. 1, la matrice de $u$ dans la base $(e_1, \ldots, e_n)$ de $E$ est égale à $h^{-1} q$, d’où

$$(2)$$
$$
\operatorname{Tr}(Q/\mathbf{H}) = \operatorname{Tr}(h^{-1} q) = \operatorname{Tr}(qh^{-1}).
$$

### 2. Applications de Hilbert–Schmidt

Soit E un espace hilbertien réel, dans lequel le produit scalaire est noté $(x|y)$. Il existe une isométrie $j_E$ de E sur son dual caractérisée par la formule

$$
(x|y) = \langle x, j_E(y) \rangle \quad \text{pour } x, y \text{ dans } E
$$

(Esp. vect. top., chap. V, § 1, n° 6, th. 3).

Soient $E_1$ et $E_2$ deux espaces hilbertiens réels et $u$ une application linéaire continue de $E_1$ dans $E_2$. On appelle adjointe de $u$ l’application linéaire continue $u^* = j_{E_1}^{-1} \circ {}^t u \circ j_{E_2}$ de $E_2$ dans $E_1$. L’application $u^*$ est caractérisée par la relation

$$
(u(x_1)|x_2) = (x_1|u^*(x_2)) \quad \text{pour } x_1 \in E_1, \quad x_2 \in E_2.
$$

Si $v$ est une application linéaire continue de $E_2$ dans un espace de Hilbert $E_3$, on a $(v \circ u)^* = u^* \circ v^*$.

Soient $E_1$ et $E_2$ deux espaces hilbertiens réels et $u$ une application linéaire de $E_1$ dans $E_2$. On définit sur $E_1$ deux formes quadratiques positives $H$ et $Q$ par les formules

$$
H(x) = \|x\|^2, \qquad Q(x) = \|u(x)\|^2 \qquad (x \in E_1).
$$

#### Proposition 3 {#int-ix-a0-prop-3 .statement}

*Supposons u continue. Soient $(e_i)_{i \in I}$ une base orthonormale de $E_1$ et $(f_j)_{j \in J}$ une base orthonormale de $E_2$. On a*

$$
\operatorname{Tr}(Q/H) = \sum_{i \in I} \|u(e_i)\|^2 = \sum_{j \in J} \|u^*(f_j)\|^2 = \sum_{i \in I} \sum_{j \in J} (u(e_i)|f_j)^2.
$$

Pour tout $x \in E_1$, on a $\|x\|^2 = \sum_{i \in I} (x|e_i)^2$ et de même $\|y\|^2 = \sum_{j \in J} (y|f_j)^2$ pour tout $y \in E_2$. Par suite, on a

$$
\sum_{i \in I} \|u(e_i)\|^2 = \sum_{i \in I} \sum_{j \in J} (u(e_i)|f_j)^2 \\
= \sum_{j \in J} \sum_{i \in I} (e_i|u^*(f_j))^2 \\
= \sum_{j \in J} \|u^*(f_j)\|^2.
$$

En particulier, le nombre $\sum_{i \in I} \|u(e_i)\|^2$ ne dépend pas de la base orthonormale $(e_i)_{i \in I}$ de $E_1$.

Posons $t = \operatorname{Tr}(Q/H)$. Pour toute partie finie $I'$ de $I$, on a par définition

$$
\sum_{i \in I'} \|u(e_i)\|^2 = \sum_{i \in I'} Q(e_i) \leq t,
$$

d’où $\sum_{i \in I} \|u(e_i)\|^2 \leq t$. Soit $(e'_1, \ldots, e'_p)$ une suite orthonormale finie dans E. On peut compléter cette suite en une base orthonormale $(e'_\alpha)_{\alpha \in A}$ de $E_1$. On a alors

$$
\sum_{\alpha = 1}^p \|u(e'_\alpha)\|^2 \leq \sum_{\alpha \in A} \|u(e'_\alpha)\|^2 = \sum_{i \in I} \|u(e_i)\|^2
$$

et, en passant à la borne supérieure sur $(e'_1, \ldots, e'_p)$, on trouve l’inégalité $t \leq \sum_{i \in I} \|u(e_i)\|^2$. On a donc établi l’égalité $t = \sum_{i \in I} \|u(e_i)\|^2$.

C.Q.F.D.

On dira que $u$ est une *application de Hilbert–Schmidt* de $E_1$ dans $E_2$ si la forme quadratique positive $Q : x \mapsto \|u(x)\|^2$ sur $E_1$ est nucléaire. S’il en est ainsi, on a $Q \leq \operatorname{Tr}(Q/H) \cdot H$, donc $u$ est continue et l’on a

$$
\|u\| \leq \operatorname{Tr}(Q/H)^{\frac{1}{2}}.
$$

Soit $u : E_1 \to E_2$ une application linéaire continue. D’après la prop. 3, $u$ est une application de Hilbert–Schmidt si et seulement s’il existe une base orthonormale $(e_i)_{i \in I}$ de $E_1$ telle que $\sum_{i \in I} \|u(e_i)\|^2 < +\infty$. S’il en est ainsi, toute base orthonormale de $E_1$ a la même propriété. De plus, si $u$ est une application de Hilbert–Schmidt, il en est de même de son adjointe $u^*$ en vertu de la formule $\sum_{i \in I} \|u(e_i)\|^2 = \sum_{j \in J} \|u^*(f_j)\|^2$ (prop. 3).

Exercises

## EXERCICES {#int-ix-a0-exercises}

See the [exercises for Appendix 0](exercises/a0/).
