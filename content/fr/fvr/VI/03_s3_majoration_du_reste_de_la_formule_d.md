---
book: fvr
book_title: Functions of a Real Variable
chapter: VI
chapter_title: DÉVELOPPEMENTS TAYLORIENS GÉNÉRALISÉS. FORMULE SOMMATOIRE D’EULER–MACLAURIN
section: 3
section_title: Majoration du reste de la formule d’Euler–Maclaurin
lang: fr
source: fvr-i-vii-fr
book_pages: FVR VI.26
pdf_pages: 0280-0282, 0286-0286
extraction: ocr
subsections:
    - "no": 1
      title: Majoration du reste de la formule d’Euler–Maclaurin
      page: 20
      pdf_page: 280
    - "no": 2
      title: Application aux développements asymptotiques
      page: 20
      pdf_page: 280
statements: 0
exercises: 3
content_sha256: cf6bce0365e084335231f835eaf827d46a43dbe46a488847490d0657f983578f
---

## § 3. MAJORATION DU RESTE DE LA FORMULE D’EULER–MACLAURIN

### 1. Majoration du reste de la formule d’Euler–Maclaurin

La majoration obtenue dans (16) pour les polynômes de Bernoulli dans l’intervalle $[0, 1]$ permet de majorer aisément le reste $T_p(x, n)$ de la formule d’Euler–Maclaurin (IV, p. 14, formule (39))

$$
\left\{
\begin{aligned}
f(x) + f(x+1) + \cdots + f(x+n) \\
= \int_x^{x+n+1} f(t)\, dt - \frac{1}{2}(f(x+n+1) - f(x)) \\
+ \sum_{k=1}^p \frac{b_{2k}}{(2k)!} (f^{(2k-1)}(x+n+1) - f^{(2k-1)}(x)) + T_p(x, n)
\end{aligned}
\right.
$$

On a en effet (VI, p. 14, formule (41))

$$
T_p(x, n) = -\frac{1}{(2p+1)!} \int_0^{n+1} \overline{B}_{2p+1}(1-s) f^{(2p+1)}(x+s)\, ds
$$

où $\overline{B}_{2p+1}(t)$ est la fonction périodique de période 1 égale à $B_{2p+1}(t)$ dans l’intervalle $[0, 1[$. La formule (16) de VI, p. 19, montre que

$$
|\overline{B}_{2p+1}(t)| \leq 4e^{2\pi} \frac{(2p+1)!}{(2\pi)^{2p+1}}
$$

pour tout $t \in \mathbf{R}$, et l’application de la formule de la moyenne donne pour $T_p(x, n)$ la majoration

$$
|T_p(x, n)| \leq \frac{4e^{2\pi}}{(2\pi)^{2p+1}} \int_x^{x+n+1} |f^{(2p+1)}(t)|\, dt.
$$

### 2. Application aux développements asymptotiques

La formule d’Euler–Maclaurin permet de donner une solution plus complète (dans les cas les plus importants) au problème traité dans V, p. 28 à 32, consistant à obtenir un développement asymptotique de la somme partielle $s_n = \sum_{m=0}^n g(m)$ (resp. du reste $r_n = \sum_{m=n+1}^\infty g(m)$), où $g$ est une fonction numérique $> 0$ et monotone définie dans un intervalle $[x_0, +\infty[$. Nous allons nous borner au cas où $g$ est une fonction (H) (V, p. 41), d’ordre 0 par rapport à $e^x$; autrement dit, on a la relation $g' \ll g$; de cette relation, on déduit $g^{(k+1)} \ll g^{(k)}$ pour tout entier $k > 0$ tel qu’aucune des dérivées $g^{(h)}$ d’ordre $h \leq k$ ne soit équivalente à une constante

(V, p. 22, prop. 7). Soit $p$ un entier tel qu’aucune des dérivées $g^{(h)}$ d’ordre $h \leq 2p$ ne soit équivalente à une constante. Supposons d’abord que la série de terme général $g(n)$ ait une somme infinie, et distinguons plusieurs cas:

1° $|g^{(2p-1)}(n)|$ tend vers $+\infty$ avec $n$; il en est de même, en vertu de l’hypothèse, de $|g^{(2k-1)}(n)|$ pour $1 \leq k \leq p$; en outre comme $g^{(2p+1)}$ est monotone au voisinage de $+\infty$, la formule (4) de VI, p. 20, donne $T_p(0, n) = O(g^{(2p)}(n + 1)) = o(g^{(2p-1)}(n + 1))$; la formule d’Euler-Maclaurin, appliquée pour $x = 0$, montre que

$$
s_n = \sum_{m=0}^n g(m) = \int_0^{n+1} g(t)\, dt - \frac{1}{2}g(n+1)
$$
$$
+ \sum_{k=1}^p \frac{b_{2k}}{(2k)!} g^{(2k-1)}(n+1) + o(g^{(2p-1)}(n+1))
$$

chacun des termes de cette somme étant négligeable devant le précédent; en développant chacun d’eux par rapport à une échelle de comparaison $\mathscr{E}$, on aura donc un développement asymptotique de $s_n$.

2° Supposons maintenant que pour un indice $q$ tel que $1 \leq q < p$, $|g^{(2q-1)}(n)|$ tend vers $+\infty$ avec $n$, mais que $g^{(2k-1)}(n)$ tende vers 0 pour $k > q$. Comme $g^{(2p+1)}$ est monotone au voisinage de $+\infty$, l’intégrale $\int_0^\infty |g^{(2p+1)}(u)| du$ est convergente, et on peut alors écrire

$$
s_n = \sum_{m=0}^n g(m) = \int_0^{n+1} g(t)\, dt - \frac{1}{2}g(n+1) + \sum_{k=1}^q \frac{b_{2k}}{(2k)!} g^{(2k-1)}(n+1) + C
$$
$$
+ \sum_{k=q+1}^p \frac{b_{2k}}{(2k)!} g^{(2k-1)}(n+1) + o(g^{(2p-1)}(n+1))
$$

où $C$ est une constante: on a en effet

$$
\int_{n+1}^\infty |g^{(2p+1)}(u)| du = O(g^{(2p)}(n+1)) = o(g^{(2p-1)}(n+1)).
$$

La même formule est valable lorsque $g(n)$ elle-même tend vers 0. Enfin, lorsque la série de terme général $g(n)$ est convergente, on a, pour le reste

$r_n = \sum_{m=n+1}^\infty g(m)$, le développement

$$
r_n = \sum_{m=n+1}^\infty g(m) = \int_{n+1}^\infty g(t)\, dt + \frac{1}{2}g(n+1)
$$
$$
- \sum_{k=1}^p \frac{b_{2k}}{(2k)!} g^{(2k-1)}(n+1) + o(g^{(2p-1)}(n+1)).
$$

Exercices

## EXERCICES {#fvr-vi-s3-exercises}

See the [exercises for § 3](exercises/s3/).
