---
book: alg
book_title: Algebra
chapter: V
chapter_title: Corps commutatifs
section: 5
section_title: EXTENSIONS RADICIELLES
lang: fr
source: alg-iv-vii-fr
book_pages: A V.23-A V.25, A V.144
pdf_pages: 0127-0129, 0248-0248
extraction: ocr
subsections:
    - "no": 1
      title: Éléments radiciels
      page: 23
      pdf_page: 127
    - "no": 2
      title: Extensions radicielles
      page: 24
      pdf_page: 128
statements: 9
exercises: 3
content_sha256: e5aeb9cce45f7b1cbf9fb672ac8eaabd6a12d9a4d67808f1e02a277cfb3e60f8
---

## § 5. EXTENSIONS RADICIELLES

Dans tout ce paragraphe, la lettre p désigne un entier qui est, soit égal à 1, soit premier. Tous les corps considérés sont d’exposant caractéristique p. Tous les résultats énoncés dans ce paragraphe sont triviaux lorsque p = 1.

### 1. Éléments radiciels

#### Définition 1 {#alg-v-s5-def-1 .statement}

Soient K un corps et E une extension de K. On dit qu’un élément x de E est radiciel sur K s’il existe un entier m \geqslant 0 tel que x^{p^m} \in K ; le plus petit de ces entiers s’appelle la hauteur de x (sur K).

#### Proposition 1 {#alg-v-s5-prop-1 .statement}

Soient E une extension d’un corps K et x un élément radiciel de hauteur e sur K ; posons a = x^{p^e}. On a alors a \in K, et le polynôme minimal de x sur K est X^{p^e} - a. De plus, on a [K(x) : K] = p^e.
Il suffit évidemment de prouver que le polynôme X^{p^e} - a est irréductible dans K[X]. D’après la définition de la hauteur de x, on a a \notin K^p, de sorte que la proposition résulte du lemme suivant :

#### Lemme 1 {#alg-v-s5-lem-1 .statement}

Soient $K$ un corps et $a$ un élément de $K$ tel que $a \notin K^p$. Pour tout entier $e \geqslant 0$, le polynôme $f(X) = X^{p^e} - a$ est irréductible dans $K[X]$.

Soient $\Omega$ une clôture algébrique de $K$, et $b$ l’élément $a^{p^{-e}}$ de $\Omega$; on note $g$ le polynôme minimal de $b$ sur $K$. On a $f(X) = (X - b)^{p^e}$ et par suite tout polynôme irréductible dans $K[X]$ qui divise $f$ admet $b$ pour racine, donc est égal à $g$. Il existe donc (IV, p. 13, prop. 13) un entier $q \geqslant 1$ tel que $f = g^q$; comme $q$ divise le degré $p^e$ de $f$, il existe un entier $e'$ tel que $0 \leqslant e' \leqslant e$ et $q = p^{e'}$. Si $c$ est le terme constant de $g$, on a $-a = c^q$; comme on a supposé que $a$ n’appartient pas à $K^p$, on a donc $q = 1$, c’est-à-dire $f = g$. D’où le lemme.

### 2. Extensions radicielles

#### Définition 2 {#alg-v-s5-def-2 .statement}

Soit $E$ une extension d’un corps $K$. On dit que $E$ est radicielle (sur $K$) si tout élément de $E$ est radiciel sur $K$. S’il en est ainsi, on dit que $E$ est de hauteur finie si l’ensemble des hauteurs des éléments de $E$ est majoré, et on appelle hauteur de $E$ le maximum des hauteurs de ses éléments.

On notera que toute extension radicielle d’un corps parfait (en particulier d’un corps de caractéristique 0) est triviale.

Soit $K$ un corps. Les extensions radicielles de hauteur 0 de $K$ sont les extensions triviales. Toute extension radicielle de $K$ est algébrique. Si $E$ est une extension radicielle de $K$ et $F$ une extension radicielle de $E$, alors $F$ est une extension radicielle de $K$ : en effet, pour tout $x \in F$, il existe un entier $m \geqslant 0$ tel que $x^{p^m} \in E$, puis un entier $n \geqslant 0$ tel que $(x^{p^m})^{p^n} \in K$, c’est-à-dire $x^{p^{m+n}} \in K$.

#### Proposition 2 {#alg-v-s5-prop-2 .statement}

Soit $E$ une extension d’un corps $K$. Pour tout entier $n \geqslant 0$, soit $E_n$ l’ensemble des éléments de $E$ qui sont radiciels de hauteur $\leqslant n$ sur $K$, et soit $E_\infty$ l’ensemble des éléments de $E$ radiciels sur $K$. Alors $(E_n)_{n \geqslant 0}$ est une suite croissante de sous-extensions de $E$, de réunion $E_\infty$, et $E_\infty$ est la plus grande extension radicielle de $K$ contenue dans $E$.

Pour tout entier $n \geqslant 0$, l’ensemble $E_n$ se compose des éléments $x$ de $E$ tels que $x^{p^n} \in K$ ; comme l’application $x \mapsto x^{p^n}$ est un endomorphisme du corps $E$, on en conclut que $E_n$ est une sous-extension de $E$. La suite $(E_n)_{n \geqslant 0}$ est croissante, de réunion $E_\infty$, et par suite $E_\infty$ est une sous-extension de $E$ (V, p. 11, prop. 3). Il est clair que $E_\infty$ est une extension radicielle de $K$, et que $E_\infty$ contient toute sous-extension de $E$ qui est radicielle sur $K$.

#### Corollaire {#alg-v-s5-n2-cor-1 .statement}

Si une extension $E$ d’un corps $K$ est engendrée par un ensemble d’éléments radiciels sur $K$, elle est radicielle sur $K$.

En effet, $E_\infty$ est une sous-extension de $E$, et l’on a par hypothèse $E = K(E_\infty)$ d’où $E = E_\infty$; par suite, $E$ est une extension radicielle de $K$.

Sous les conditions de la proposition 2, on dit que $E_\infty$ est la fermeture radicielle de $K$ dans $E$.

Nous appliquerons surtout la prop. 2 au cas où E est une extension algébriquement close de K ; alors E est parfait et l’on a $E_n = K^{p^{-n}}$ pour tout $n \geq 0$. On note dans ce cas $K^{p^{-\infty}}$ l’ensemble des éléments de E radiciels sur K ; c’est le sous-corps de E réunion de la suite croissante $(K^{p^{-n}})_{n \geq 0}$ de sous-corps de E. D’après la prop. 2, $K^{p^{-\infty}}$ est la plus grande des sous-extensions de E qui sont radicielles sur K ; d’après la prop. 3 de V, p. 6, $K^{p^{-\infty}}$ est une clôture parfaite de K, et c’est aussi le plus petit sous-corps parfait de E contenant K. Lorsque K est parfait, on a évidemment $K = K^{p^{-n}} = K^{p^{-\infty}}$ pour tout $n$. Si K est imparfait, on a $K \neq K^p$, d’où

$$
K^{p^{-n}} \neq (K^p)^{p^{-n}} = K^{p^{-(n-1)}}
$$

pour $n \geq 1$ : les sous-corps $K^{p^{-n}}$ de E sont donc deux à deux distincts, et $K^{p^{-\infty}}$ est une extension algébrique de degré *infini* de K.

#### Proposition 3 {#alg-v-s5-prop-3 .statement}

*Soient K un corps, E un surcorps de K radiciel sur K et u un homomorphisme de K dans un corps parfait F. Il existe un homomorphisme v de E dans F prolongeant u, et un seul.*

Soit $E_n$ l’ensemble des éléments de E qui sont radiciels de hauteur $\leq n$ sur K. D’après la prop. 2, le corps E est réunion de la suite croissante $(E_n)_{n \geq 0}$ de sous-corps. Soit $v$ un homomorphisme de E dans F prolongeant $u$ ; pour tout $x \in E_n$, on a $x^{p^n} \in K$, d’où $v(x)^{p^n} = v(x^{p^n}) = u(x^{p^n})$ ; on a donc $v(x) = u(x^{p^n})^{p^{-n}}$ pour tout $n \geq 0$ et tout $x \in E_n$, d’où l’unicité d’un prolongement de $u$ à E.

Soit $n$ un entier positif ; pour tout $x \in E_n$, on a $x^{p^n} \in K$, et comme F est parfait, on définit un élément $v_n(x)$ de F par $v_n(x) = u(x^{p^n})^{p^{-n}}$. Il est immédiat que $v_n$ est un homomorphisme de $E_n$ dans F, qu’on a $v_0 = u$ et que $v_{n+1}$ induit $v_n$ sur $E_n$. Il existe donc un homomorphisme $v$ de E dans F induisant $v_n$ sur $E_n$ pour tout $n \geq 0$ et en particulier, coïncidant avec $v_0 = u$ sur $E_0 = K$.

#### Corollaire {#alg-v-s5-n2-cor-2 .statement}

*Pour qu’une extension E d’un corps K soit une clôture parfaite de K, il faut et il suffit que ce soit une extension radicielle de K et que le corps E soit parfait.*

Le corollaire est trivial lorsque $p = 1$ ; supposons donc $p \neq 1$. Les conditions énoncées sont nécessaires d’après V, p. 5, th. 3 ; elles sont suffisantes d’après la prop. 3.

#### Proposition 4 {#alg-v-s5-prop-4 .statement}

*Soit E une extension radicielle de degré fini d’un corps K. Alors [E : K] est une puissance de l’exposant caractéristique p de K.*

Comme E est une extension radicielle de degré fini de K, il existe des éléments $a_1, \ldots, a_m$ de E, radiciels sur K et tels que $E = K(a_1, \ldots, a_m)$. Soit $i$ compris entre 1 et $m$ ; comme $a_i$ est *a fortiori* radiciel sur $K(a_1, \ldots, a_{i-1})$, le degré

$$
n_i = [K(a_1, \ldots, a_i) : K(a_1, \ldots, a_{i-1})]
$$

est une puissance de $p$ (V, p. 23, prop. 1). On a $[E : K] = n_1 \ldots n_m$ d’après V, p. 17, th. 2, d’où la proposition.

## EXERCICES {#alg-v-s5-exercises}

See the [exercises for § 5](exercises/s5/).
