---
book: alg
book_title: Algebra
chapter: III
chapter_title: ALGÈBRES TENSORIELLES, ALGÈBRES EXTÉRIEURES, ALGÈBRES SYMÉTRIQUES
section: 7
section_title: Algèbre extérieure
lang: fr
source: alg-i-iii-fr
book_pages: A III.76-A III.90, A III.189-A III.191
pdf_pages: 0463-0477, 0576-0578
extraction: ocr
subsections:
    - "no": 1
      title: Définition de l’algèbre extérieure d’un module
      page: 76
      pdf_page: 463
    - "no": 2
      title: Propriétés fonctorielles de l’algèbre extérieure
      page: 77
      pdf_page: 464
    - "no": 3
      title: Anticommutativité de l’algèbre extérieure
      page: 79
      pdf_page: 466
    - "no": 4
      title: Puissance extérieure $n$-ème d’un module et applications multilinéaires alternées
      page: 80
      pdf_page: 467
    - "no": 5
      title: Extension de l’anneau des scalaires
      page: 82
      pdf_page: 469
    - "no": 6
      title: Limites inductives d’algèbres extérieures
      page: 83
      pdf_page: 470
    - "no": 7
      title: Algèbre extérieure d’une somme directe. Algèbre extérieure d’un module gradué
      page: 83
      pdf_page: 470
    - "no": 8
      title: Algèbre extérieure d’un module libre
      page: 86
      pdf_page: 473
    - "no": 9
      title: Critères d’indépendance linéaire
      page: 88
      pdf_page: 475
statements: 30
exercises: 15
content_sha256: 50eb4d0f6b35bf47dec4073c1ae82fe5673ae979ce273833b17ead7fdc947f74
---

## § 7. ALGÈBRE EXTÉRIEURE

### 1. Définition de l’algèbre extérieure d’un module

#### Définition 1 {#alg-iii-s7-def-1 .statement}

Soient $A$ un anneau commutatif, $M$ un $A$-module. On appelle algèbre extérieure de $M$, et on note $\wedge(M)$ ou $\mathrm{Alt}(M)$ ou $\wedge_A(M)$, l’algèbre sur $A$ quotient de l’algèbre tensorielle $T(M)$ par l’idéal bilatère $\mathfrak{I}''$ (aussi noté $\mathfrak{I}_{M}''$) engendré par les éléments $x \otimes x$, où $x$ parcourt $M$.

L’idéal $\mathfrak{I}''$ étant engendré par des éléments homogènes de degré 2, est un idéal gradué (II, p. 167, prop. 2); on pose $\mathfrak{I}_n'' = \mathfrak{I}'' \cap T^n(M)$; l’algèbre $\wedge(M)$ est donc graduée par la graduation (dite canonique) formée des $\wedge^n(M) = T^n(M)/\mathfrak{I}_n''$.

On a $\mathfrak{g}_0' = \mathfrak{g}_1'' = \{0\}$, donc $\wedge^0(M)$ s’identifie canoniquement à $A$ et $\wedge^1(M)$ à $T^1(M) = M$; nous ferons toujours par la suite ces identifications, et nous noterons $\varphi''$ ou $\varphi_M''$ l’injection canonique $M \to \wedge(M)$.

#### Proposition 1 {#alg-iii-s7-prop-1 .statement}

*Soient E une A-algèbre, $f : M \to E$ une application A-linéaire telle que*
$$
(f(x))^2 = 0 \quad \text{quel que soit } x \in M.
$$
*Il existe un homomorphisme et un seul de A-algèbres $g : \wedge(M) \to E$ tel que $f = g \circ \varphi''$.*

En d’autres termes, $(\wedge(M), \varphi'')$ est solution du *problème d’application universelle* (E, IV, p. 23), où $\Sigma$ est l’espèce de structure de A-algèbre, les $\alpha$-applications étant les applications linéaires du A-module $M$ dans une A-algèbre vérifiant (1).

L’unicité de $g$ résulte de ce que $\varphi''(M) = M$ engendre $\wedge(M)$. Pour prouver l’existence de $g$, notons qu’en vertu de III, p. 56, prop. 1, il existe un homomorphisme $g_1 : T(M) \to E$ de A-algèbres tel que $f = g_1 \circ \varphi$; tout revient à voir que $g_1$ s’annule dans l’idéal $\mathfrak{g}'$, car alors, si $p : T(M) \to \wedge(M) = T(M)/\mathfrak{g}'$ est l’homomorphisme canonique, on pourra écrire $g_1 = g \circ p$, où $g : \wedge(M) \to E$ est un homomorphisme d’algèbres, et la conclusion résultera de ce que $p \circ \varphi = \varphi''$. Or, le noyau de $g_1$ est un idéal bilatère qui, en vertu de (1) et de la relation $g_1 \circ \varphi = f$, contient les éléments $x \otimes x$ pour $x \in M$. Ceci termine la démonstration.

*Remarques. — 1) Supposons que E soit une A-algèbre *graduée* de type $\mathbf{Z}$, de graduation $(E_n)$, et supposons en outre que l’application linéaire $f$ (supposée vérifier (1)) soit telle que*
$$
f(M) \subset E_1.
$$
Alors la relation $g(x_1 x_2 \ldots x_p) = f(x_1) f(x_2) \ldots f(x_p)$ pour les $x_i \in M$ montre que $g(\wedge^p(M)) \subset E_p$ pour tout $p \geqslant 0$, donc $g$ est un homomorphisme d’*algèbres graduées*.

2) Pour éviter des confusions, on note le plus souvent le produit de deux éléments $u, v$ de l’algèbre extérieure $\wedge(M)$ par $u \wedge v$ et on dit qu’il est le *produit extérieur* de $u$ par $v$. Les éléments de $\wedge^n(M)$ sont donc les sommes d’éléments de la forme $x_1 \wedge x_2 \wedge \cdots \wedge x_n$ avec $x_i \in M$ pour $1 \leqslant i \leqslant n$ et sont souvent appelés *n-vecteurs*.

### 2. Propriétés fonctorielles de l’algèbre extérieure

#### Proposition 2 {#alg-iii-s7-prop-2 .statement}

*Soient A un anneau commutatif, M et N deux A-modules, $u : M \to N$ une application A-linéaire. Il existe un homomorphisme de A-algèbres et un seul,*
$$
u'' : \wedge(M) \to \wedge(N),
$$
*tel que le diagramme*
$$
\begin{array}{ccc}
M & \xrightarrow{u} & N \\
\downarrow{\varphi_M''} & & \downarrow{\varphi_N''} \\
\wedge(M) & \xrightarrow{u''} & \wedge(N)
\end{array}
$$
*soit commutatif. En outre, $u''$ est un homomorphisme d’algèbres graduées.*

L’existence et l’unicité de $u''$ résultent de III, p. 77, prop. 1, appliquée à l’algèbre $\wedge(\mathbf{N})$ et à $f = \varphi''_{\mathbf{N}} \circ u : \mathbf{M} \to \wedge(\mathbf{N})$; on a en effet $f(\mathbf{M}) \subset \mathbf{N}$, donc $f$ vérifie la condition (1) par définition de $\mathfrak{J}'_{\mathbf{N}}$; comme $f(\mathbf{M}) \subset \wedge^1(\mathbf{N}) = \mathbf{N}$, le fait que $u''$ soit un homomorphisme d’algèbres graduées résulte de la Remarque 1 de III, p. 77.

L’homomorphisme $u''$ de la prop. 2 sera désormais noté $\wedge(u)$. Si $\mathbf{P}$ est un A-module et $v : \mathbf{N} \to \mathbf{P}$ une application A-linéaire, on a
$$
\wedge(v \circ u) = \wedge(v) \circ \wedge(u)
$$
car $\wedge(v) \circ \wedge(u)$ est un homomorphisme d’algèbres qui rend commutatif le diagramme

$$
\begin{array}{ccc}
\mathbf{M} & \xrightarrow{v \circ u} & \mathbf{P} \\
\varphi''_{\mathbf{M}} \downarrow & & \downarrow \varphi''_{\mathbf{P}} \\
\wedge(\mathbf{M}) & \xrightarrow{\wedge(v) \circ \wedge(u)} & \wedge(\mathbf{P})
\end{array}
$$

Puisque $\wedge(\mathbf{M})$ contient $\mathbf{M} = \wedge^1(\mathbf{M})$, on dit parfois que $\wedge(u)$ est le prolongement canonique de $u$ à $\wedge(\mathbf{M})$. La restriction $\wedge^n(u) : \wedge^n(\mathbf{M}) \to \wedge^n(\mathbf{N})$ est telle que
$$
\wedge^n(u)(x_1 \wedge x_2 \wedge \cdots \wedge x_n) = u(x_1) \wedge u(x_2) \wedge \cdots \wedge u(x_n)
$$
pour les $x_i \in \mathbf{M}$, puisque $\wedge(u)$ est un homomorphisme d’algèbres et $\wedge^1(u) = u$; la restriction $\wedge^0(u)$ à $\mathbf{A}$ est l’application identique. On notera que $\wedge^n(u)$ provient de $\mathbf{T}^n(u) : \mathbf{T}^n(\mathbf{M}) \to \mathbf{T}^n(\mathbf{N})$ par passage aux quotients.

#### Proposition 3 {#alg-iii-s7-prop-3 .statement}

*Si $u : \mathbf{M} \to \mathbf{N}$ est une application A-linéaire surjective, l’homomorphisme $\wedge(u) : \wedge(\mathbf{M}) \to \wedge(\mathbf{N})$ est surjectif, et son noyau est l’idéal bilatère de $\wedge(\mathbf{M})$ engendré par le noyau $\mathbf{P} \subset \mathbf{M} \subset \wedge(\mathbf{M})$ de $u$.

La démonstration se déduit de celle de III, p. 69, prop. 4 en y remplaçant S par $\wedge$ et $\mathfrak{J}'$ par $\mathfrak{J}''$.

Si $u : \mathbf{M} \to \mathbf{N}$ est une application linéaire injective, il n’est pas toujours vrai que $\wedge(u)$ soit une application injective (III, p. 188, exerc. 3) (voir cependant plus loin III, p. 88, corollaire). Toutefois il en est ainsi lorsque $u$ est une injection telle que $u(\mathbf{M})$ soit facteur direct de $\mathbf{N}$, et alors l’image de $\wedge(u)$ (isomorphe à $\wedge(\mathbf{M})$) est facteur direct de $\wedge(\mathbf{N})$; la démonstration est la même que celle des assertions analogues pour $\mathbf{T}(u)$ (III, p. 58) en remplaçant $\mathbf{T}$ par $\wedge$.

#### Proposition 4 {#alg-iii-s7-prop-4 .statement}

*Soient $\mathbf{N}$ et $\mathbf{P}$ deux sous-modules d’un A-module $\mathbf{M}$, tels que leur somme $\mathbf{N} + \mathbf{P}$ soit facteur direct dans $\mathbf{M}$, et que leur intersection $\mathbf{N} \cap \mathbf{P}$ soit facteur direct dans $\mathbf{N}$ et dans $\mathbf{P}$. Alors les homomorphismes $\wedge(\mathbf{N}) \to \wedge(\mathbf{M}), \wedge(\mathbf{P}) \to \wedge(\mathbf{M})$ et $\wedge(\mathbf{N} \cap \mathbf{P}) \to \wedge(\mathbf{M})$ prolongements canoniques des injections canoniques, sont injectifs; si l’on identifie $\wedge(\mathbf{N}), \wedge(\mathbf{P}),$ et $\wedge(\mathbf{N} \cap \mathbf{P})$ à des sous-algèbres de $\wedge(\mathbf{M})$ au moyen de ces homomorphismes, on a*
$$
\wedge(\mathbf{N} \cap \mathbf{P}) = \wedge(\mathbf{N}) \cap \wedge(\mathbf{P}).
$$

La démonstration se déduit de celle de III, p. 58, prop. 4 en remplaçant partout T par $\wedge$. Les hypothèses de la prop. 4 sont toujours vérifiées pour des sous-modules quelconques N, P de M lorsque A est un corps.

#### Corollaire {#alg-iii-s7-n2-cor-1 .statement}

Soient K un corps commutatif, M un espace vectoriel sur K. Pour tout élément $z \in \wedge(M)$, il existe un plus petit sous-espace vectoriel N de M tel que $z \in \wedge(N)$, et N est de dimension finie.

La démonstration se déduit de celle de III, p. 59, corollaire, en remplaçant partout T par $\wedge$.

On dit que N est le sous-espace vectoriel de M associé à l’élément z de $\wedge(M)$.

### 3. Anticommutativité de l’algèbre extérieure

#### Proposition 5 {#alg-iii-s7-prop-5 .statement}

(i) Soit $(x_i)_{1 \leq i \leq n}$ une suite finie d’éléments du module M; pour toute permutation $\sigma$ du groupe symétrique $\mathfrak{S}_n$, on a

$$
x_{\sigma(1)} \wedge x_{\sigma(2)} \wedge \cdots \wedge x_{\sigma(n)} = \varepsilon_\sigma \cdot x_1 \wedge x_2 \wedge \cdots \wedge x_n
$$

$\varepsilon_\sigma$ désignant la signature de la permutation $\sigma$.

(ii) S’il existe deux indices distincts i, j tels que $x_i = x_j$, le produit

$$
x_1 \wedge x_2 \wedge \cdots \wedge x_n
$$

est nul.

(i) Tout d’abord, puisqu’on a $x \wedge x = 0$ quel que soit $x \in M$ par définition de l’idéal $\mathfrak{J}'$, on a aussi, pour $x, y$ dans M,

$$
x \wedge y + y \wedge x = (x + y) \wedge (x + y) - x \wedge x - y \wedge y = 0.
$$

Ceci établit (6) dans le cas où $n = 2$. Le cas général résulte alors de III, p. 45, lemme 3.

(ii) Sous les hypothèses de (ii), il existe une permutation $\sigma \in \mathfrak{S}_n$ telle que $\sigma(1) = i$ et $\sigma(2) = j$; alors le premier membre de (6) est nul pour cette permutation, donc il en est de même du second.

#### Corollaire 1 {#alg-iii-s7-prop-5-cor-1 .statement}

Soient H, K deux parties complémentaires de l’intervalle $[1, n]$ de $\mathbf{N}$, et soient $(i_h)_{1 \leq h \leq p}$, $(j_k)_{1 \leq k \leq n-p}$ les suites des éléments de H et de K respectivement, rangées dans l’ordre croissant; posons

$$
x_H = x_{i_1} \wedge x_{i_2} \wedge \cdots \wedge x_{i_p}, \quad x_K = x_{j_1} \wedge x_{j_2} \wedge \cdots \wedge x_{j_{n-p}};
$$

alors on a

$$
x_H \wedge x_K = (-1)^{\nu} x_1 \wedge x_2 \wedge \cdots \wedge x_n
$$

où $\nu$ est le nombre des couples $(i, j) \in H \times K$ tels que $i > j$.

Compte tenu de la prop. 5, tout revient à prouver le

#### Lemme 1 {#alg-iii-s7-lem-1 .statement}

Si $\sigma \in \mathfrak{S}_n$ est la permutation telle que $\sigma(h) = i_h$ pour $1 \leq h \leq p$, $\sigma(h) = j_{h-p}$ pour $p + 1 \leq h \leq n$, on a $\varepsilon_\sigma = (-1)^{\nu}$.

En effet, pour $1 \leq h < h' \leq p$ ou $p + 1 \leq h < h' \leq n$, on a $\sigma(h') > \sigma(h)$, et le nombre des couples $(h, h')$ tels que $1 \leq h \leq p < h' \leq n$ et que $\sigma(h) > \sigma(h')$ est égal à $\nu$.

#### Corollaire 2 {#alg-iii-s7-lem-1-cor-2 .statement}

*L’algèbre graduée* $\wedge(M)$ *est alternée* (III, p. 53).
Il suffit en effet d’appliquer à $\wedge(M)$ la prop. 13 de III, p. 54, en prenant pour système générateur l’ensemble M et en utilisant la prop. 5 de III, p. 79.

#### Proposition 6 {#alg-iii-s7-prop-6 .statement}

*Si M est un A-module de type fini, $\wedge(M)$ est un A-module de type fini; de plus, si M admet un système générateur à n éléments, on a $\wedge^p(M) = \{0\}$ pour $p > n$.*
Soit en effet $(x_i)_{1 \leq i \leq n}$ un système générateur de M. Tout élément de $\wedge^p(M)$ est combinaison linéaire d’éléments de la forme
$$
x_{i_1} \wedge x_{i_2} \wedge \cdots \wedge x_{i_p}
$$
où les indices $i_k$ appartiennent à $\{1, n\}$; en vertu de la prop. 5 de III, p. 79, on peut supposer ces indices distincts (sinon l’élément correspondant est nul). Si $p > n$, il n’y a pas de telle suite d’indices, donc $\wedge^p(M) = \{0\}$. Si $p \leq n$, ces suites sont en nombre fini, ce qui achève la démonstration.

### 4. Puissance extérieure $n$-ème d’un module et applications multilinéaires alternées

Etant donnés deux modules M, N sur un anneau commutatif A, on appelle application *n-linéaire alternée* de $M^n$ dans N toute application *n-linéaire* $f : M^n \to N$ telle que l’on ait, pour tout $p \leq n - 2$.
(8)
$$
f(u_1, \ldots, u_p, x, x, v_1, \ldots, v_{n-p-2}) = 0
$$
quels que soient $x$, les $u_i$ ($1 \leq i \leq p$) et les $v_j$ ($1 \leq j \leq n - p - 2$) dans M.

#### Proposition 7 {#alg-iii-s7-prop-7 .statement}

*Soient A un anneau commutatif, M et N deux A-modules. Si, à toute application A-linéaire $g : \wedge^n(M) \to N$ ($n \geq 2$) on associe l’application n-linéaire*
(9)
$$
(x_1, x_2, \ldots, x_n) \mapsto g(x_1 \wedge x_2 \wedge \cdots \wedge x_n)
$$
*on obtient une application A-linéaire bijective du A-module* $\operatorname{Hom}_A(\wedge^n(M), N)$ *sur le A-module des applications n-linéaires alternées de* $M^n$ *dans N*.
Considérons en effet la bijection canonique de A-module $\operatorname{Hom}_A(T^n(M), N)$ sur le A-module $\mathcal{L}_n(M, \ldots, M; N)$ de *toutes* les applications *n*-linéaires de $M^n$ dans N, obtenu en associant à toute application A-linéaire $f : T^n(M) \to N$ l’application *n*-linéaire
$$
\tilde{f} : (x_1, \ldots, x_n) \mapsto f(x_1 \otimes x_2 \otimes \cdots \otimes x_n)
$$
(II, p. 71). D’autre part, les applications A-linéaires $g : \wedge^n(M) \to N$ correspondent biunivoquement aux applications A-linéaires $f : \mathbf{T}^n(\mathbf{M}) \to \mathbf{N}$ telles que $f$ s’annule dans $\mathfrak{S}_n''$, en associant à $g$ l’application $f = g \circ p_n$, où
$$
p_n : \mathbf{T}^n(\mathbf{M}) \to \wedge^n(\mathbf{M}) = \mathbf{T}^n(\mathbf{M})/\mathfrak{S}_n''
$$
est l’homomorphisme canonique (II, p. 36, th. 1). Mais comme $\mathfrak{S}_n''$ est combinai-son linéaire d’éléments de la forme
$$
(u_1 \otimes u_2 \otimes \cdots \otimes u_p) \otimes (x \otimes x) \otimes (v_1 \otimes \cdots \otimes v_{n-p-2})
$$
$(x, u_i, v_j$ dans $\mathbf{M}$), dire que $f$ est de la forme $g \circ p_n$ signifie que la fonction $n$-linéaire correspondante $\bar{f}$ vérifie (8), autrement dit est alternée.

On dit que le A-module $\wedge^n(\mathbf{M})$ est la puissance extérieure $n$-ème de $\mathbf{M}$. Pour tout homomorphisme de A-modules $u : \mathbf{M} \to \mathbf{N}$, l’application
$$
\wedge^n(u) : \wedge^n(\mathbf{M}) \to \wedge^n(\mathbf{N})
$$
qui coïncide avec $\wedge(u)$ dans $\wedge^n(\mathbf{M})$ s’appelle la puissance extérieure $n$-ème de $u$.

#### Corollaire 1 {#alg-iii-s7-prop-7-cor-1 .statement}

*Pour toute application n-linéaire alternée $g : \mathbf{M}^n \to \mathbf{N}$, on a, pour toute permutation $\sigma \in \mathfrak{S}_n$*,
$$
g(x_{\sigma(1)}, x_{\sigma(2)}, \ldots, x_{\sigma(n)}) = \varepsilon_\sigma g(x_1, x_2, \ldots, x_n)
$$
*quels que soient les $x_i \in \mathbf{M}$; en outre si $x_i = x_j$ pour deux indices $i, j$ distincts, on a*
$$
g(x_1, x_2, \ldots, x_n) = 0.
$$
C’est une conséquence évidente de la prop. 7 de III, p. 80 et de III, p. 79, prop. 5.

#### Corollaire 2 {#alg-iii-s7-prop-7-cor-2 .statement}

*Soit $(x_i)_{1 \leq i \leq n}$ une suite de n éléments de $\mathbf{M}$ telle que*
$$
x_1 \wedge x_2 \wedge \cdots \wedge x_n = 0;
$$
*alors, pour toute application n-linéaire alternée $g : \mathbf{M}^n \to \mathbf{N}$, on a* $g(x_1, \ldots, x_n) = 0$.

#### Corollaire 3 {#alg-iii-s7-prop-7-cor-3 .statement}

*Soit $f : \mathbf{M}^{n-1} \to \mathbf{A}$ une forme $(n-1)$-linéaire alternée. Si $(x_i)_{1 \leq i \leq n}$ est une suite de n éléments de $\mathbf{M}$ telle que $x_1 \wedge x_2 \wedge \cdots \wedge x_n = 0$, on a*
$$
\sum_{i=1}^n (-1)^i f(x_1, \ldots, \hat{x}_i, \ldots, x_n)x_i = 0
$$
*(où l’on pose $f(x_1, \ldots, \hat{x}_i, \ldots, x_n) = f(x_1, \ldots, x_{i-1}, x_{i+1}, \ldots, x_n)$ pour $1 \leq i \leq n$).*
Il suffit de prouver que l’application $n$-linéaire
$$
(x_1, \ldots, x_n) \mapsto \sum_{i=1}^n (-1)^i f(x_1, \ldots, \hat{x}_i, \ldots, x_n)x_i
$$
de $\mathbf{M}^n$ dans $\mathbf{M}$ est *alternée*. Or, si $x_i = x_{i+1}$, tous les termes de la somme du second membre ont des coefficients nuls sauf $x_i$ et $x_{i+1}$, puisque $f$ est alternée; d’autre part, le coefficient de $x_i$ est $(-1)^i f(x_1, \ldots, x_{i-1}, x_{i+1}, x_{i+2}, \ldots, x_n)$ et celui de $x_{i+1}$ est $(-1)^{i+1} f(x_1, \ldots, x_i, x_{i+2}, \ldots, x_n)$ et ils sont opposés par hypothèse.

#### Remarque {#alg-iii-s7-n4-rem-1 .statement}

On dit qu’un élément z de $T^n(M)$ est un tenseur antisymétrique (contravariant) d’ordre n si $\sigma.z = \varepsilon_\sigma z$ pour tout permutation $\sigma \in \mathfrak{S}_n$ (cf. III, p. 71, Remarque); ces éléments forment un sous-A-module $A'_n(M)$ de $T^n(M)$. Pour tout $z \in T^n(M)$, on pose $a.z = \sum_{\sigma \in \mathfrak{S}_n} \varepsilon_\sigma(\sigma.z)$ et on dit que $a.z$ est l’antisymétrisé de z; comme $\varepsilon_{\sigma\tau} = \varepsilon_\sigma \varepsilon_\tau$, on voit aussitôt que $a.z$ est un tenseur antisymétrique, et par suite $z \mapsto a.z$ est un endomorphisme de $T^n(M)$ dont l’image $A''_n(M)$ est contenue dans $A'_n(M)$; en général on a $A''_n(M) \neq A'_n(M)$ (III, p. 189, exerc. 8). Si $z$ est un tenseur antisymétrique, on a $a.z = n!z$; donc, lorsque $n!$ est inversible dans A, l’endomorphisme $z \mapsto (n!)^{-1}a.z$ est un projecteur dans $T^n(M)$ dont l’image est $A'_n(M) = A''_n(M)$. En outre le noyau de ce projecteur n’est autre que $\mathfrak{g}_n''$; en effet, on peut évidemment se borner au cas où $n \geqslant 2$, donc 2 (divisant $n!$) est inversible dans A et $x \otimes x = 2^{-1}(x \otimes x + x \otimes x)$; par suite $\mathfrak{g}_n''$ est engendré par les éléments $z + \rho.z$, où $\rho$ est une transposition échangeant deux nombres consécutifs dans $\{1, n\}$; en outre, pour deux permutations $\sigma, \tau$ de $\mathfrak{S}_n$, on peut écrire
$$
z - \varepsilon_{\sigma\tau}((\sigma\tau).z) = z - \varepsilon_\tau(\tau.z) + \varepsilon_\tau(\tau.z - \varepsilon_\sigma\sigma.(\tau.z)),
$$
d’où l’on déduit que $z - \varepsilon_\sigma(\sigma.z) \in \mathfrak{g}_n''$ quels que soient $z \in T^n(M)$ et $\sigma \in \mathfrak{S}_n$. Par suite (en supposant toujours $n!$ inversible dans A), on voit que $z - (n!)^{-1}a.z = \sum_{\sigma \in \mathfrak{S}_n} (n!)^{-1}(z - \varepsilon_\sigma(\sigma.z)) \in \mathfrak{g}_n''$ pour tout $z \in T^n(M)$, ce qui établit notre assertion.

Lorsque $n!$ est inversible dans A, les sous-modules $A'_n(M)$ et $\mathfrak{g}_n''$ de $T^n(M)$ sont donc supplémentaires, et la restriction à $A'_n(M)$ de l’homomorphisme canonique $T^n(M) \to \wedge^n(M) = T^n(M)/\mathfrak{g}_n''$ est un isomorphisme de A-modules, qui permet dans le cas envisagé d’identifier les tenseurs antisymétriques d’ordre n aux éléments de la puissance extérieure n-ème de M. On notera ici encore que cette identification n’est pas compatible avec la multiplication, le produit dans $T(M)$ de deux tenseurs antisymétriques n’étant pas antisymétrique en général.

### 5. Extension de l’anneau des scalaires

Soient A, A’ deux anneaux commutatifs, $\rho : A \to A'$ un homomorphisme d’anneaux, M un A-module, M’ un A’-module, $f : M \to M'$ un A-homomorphisme (relatif à $\rho$) de M dans M’. L’application composée $M \xrightarrow{f} M' \xrightarrow{\varphi''_{M'}} \wedge_{A'}(M')$ est une application A-linéaire de M dans la A-algèbre $\wedge_{A'}(M')$, et comme les éléments de $f(M) \subset M'$ sont de carré nul dans $\wedge_{A'}(M')$, il existe (III, p. 77, prop. 1) un A-homomorphisme d’algèbres et un seul $f'' : \wedge_A(M) \to \wedge_{A'}(M')$ rendant commutatif le diagramme

$$
\begin{array}{ccc}
M & \xrightarrow{f} & M' \\
\varphi''_M \downarrow & & \downarrow \varphi''_{M'} \\
\wedge_A(M) & \xrightarrow{f''} & \wedge_{A'}(M')
\end{array}
$$

(12) et $f''$ est un homomorphisme d’algèbres graduées. On en déduit aussitôt que si $\sigma : A' \to A''$ est un second homomorphisme d’anneaux, $M''$ un $A''$-module, $g : M' \to M''$ un $A'$-homomorphisme (relatif à $\sigma$), $g'' : \wedge_{A'}(M') \to \wedge_{A''}(M'')$ le $A''$-homomorphisme d’algèbres correspondant, alors le $A$-homomorphisme d’algèbres composé

$$
\wedge_A(M) \xrightarrow{f''} \wedge_{A'}(M') \xrightarrow{g''} \wedge_{A''}(M'')
$$

correspond au $A$-homomorphisme composé $g \circ f : M \to M''$ (relatif à $\sigma \circ \rho$).

#### Proposition 8 {#alg-iii-s7-prop-8 .statement}

*Soient $A, B$ deux anneaux commutatifs, $\rho : A \to B$ un homomorphisme d’anneaux, $M$ un $A$-module. Le prolongement canonique*

$$
\psi : \wedge_B(B \otimes_A M) \to B \otimes_A \wedge_A(M)
$$

*de l’application B-linéaire $l_B \otimes \varphi_M'' : B \otimes_A M \to B \otimes_A \wedge_A(M)$, est un isomorphisme de B-algèbres graduées.*

La démonstration se déduit de celle de III, p. 60, prop. 5 en y remplaçant $T$ par $\wedge$ et $\varphi_M$ par $\varphi_M''$.

### 6. Limites inductives d’algèbres extérieures

Soient $(A_\alpha, \varphi_{\beta \alpha})$ un système inductif filtrant d’anneaux commutatifs, $(M_\alpha, f_{\beta \alpha})$ un système inductif de $A_\alpha$-modules, $A = \lim \longrightarrow A_\alpha, M = \lim \longrightarrow M_\alpha$. Pour $\alpha \leq \beta$, on déduit canoniquement du $A_\alpha$-homomorphisme $f_{\beta \alpha} : M_\alpha \to M_\beta$ un homomorphisme de $A_\alpha$-algèbres (III, p. 82, formule (12)) $f_{\beta \alpha}' : \wedge_{A_\alpha}(M_\alpha) \to \wedge_{A_\beta}(M_\beta)$ et il résulte de (13) que $(\wedge_{A_\alpha}(M_\alpha), f_{\beta \alpha}')$ est un *système inductif de A-algèbres graduées*. Soit d’autre part $f_\alpha : M_\alpha \to M$ le $A_\alpha$-homomorphisme canonique; on en déduit (III, p. 82, formule (12)) un homomorphisme de $A_\alpha$-algèbres graduées, $f_\alpha'' : \wedge_{A_\alpha}(M_\alpha) \to \wedge_A(M)$, et il résulte encore de (13) que les $f_\alpha''$ constituent un système inductif de $A_\alpha$-homomorphismes.

#### Proposition 9 {#alg-iii-s7-prop-9 .statement}

*Le $A$-homomorphisme $f'' = \lim \longrightarrow f_\alpha'' : \lim \longrightarrow \wedge_{A_\alpha}(M_\alpha) \to \wedge_A(M)$ est un isomorphisme d’algèbres graduées.*

La démonstration est la même que celle de III, p. 61, prop. 6, en y remplaçant partout $T$ par $\wedge$ et $\varphi$ et $\varphi''$, et tenant compte du fait qu’une limite inductive d’algèbres alternées est alternée.

### 7. Algèbre extérieure d’une somme directe. Algèbre extérieure d’un module gradué

Soient $A$ un anneau commutatif, $M = \bigoplus_{\lambda \in L} M_\lambda$ la somme directe d’une famille de $A$-modules, $j_\lambda : M_\lambda \to M$ l’injection canonique; on en déduit un $A$-homomorphisme d’algèbres graduées $\wedge(j_\lambda) : \wedge(M_\lambda) \to \wedge(M)$. Puisque $\wedge(M)$ est anti-commutative, on peut appliquer aux homomorphismes $\wedge(j_\lambda)$ la prop. 10 de III, p. 47 (éventuellement généralisée au cas où L est infini, cf. III, p. 53, Remarque); il existe donc un unique homomorphisme d’algèbres

(14)
$$
g : \bigotimes_{\lambda \in L}^{\mathfrak{g}} \wedge (M_\lambda) \to \wedge (M)
$$
(aussi noté $g_M$) tel que $\wedge (j_\lambda) = g \circ f_\lambda$, en désignant par
$$
f_\lambda : \wedge (M_\lambda) \to \bigotimes_{\lambda \in L}^{\mathfrak{g}} \wedge (M_\lambda)
$$
l’homomorphisme canonique.

#### Proposition 10 {#alg-iii-s7-prop-10 .statement}

*L’homomorphisme canonique g (formule (14)) est un isomorphisme d’algèbres graduées.*
Pour prouver que $g$ est bijectif, on définit un homomorphisme d’algèbres graduées
(15)
$$
h : \wedge (M) \to \bigotimes_{\lambda \in L}^{\mathfrak{g}} \wedge (M_\lambda)
$$
tel que $g \circ h$ et $h \circ g$ soient respectivement les applications identiques de $\wedge (M)$ et de $\bigotimes_{\lambda \in L}^{\mathfrak{g}} \wedge (M_\lambda)$. Pour chaque $\lambda \in L$, on considère l’application linéaire composée
$$
u_\lambda : M_\lambda \xrightarrow{\varphi''_{M_\lambda}} \wedge (M_\lambda) \xrightarrow{f_\lambda} \bigotimes_{\lambda \in L}^{\mathfrak{g}} \wedge (M_\lambda).
$$
Il existe une application A-linéaire et une seule $u : M \to \bigotimes_{\lambda \in L}^{\mathfrak{g}} \wedge (M_\lambda)$ telle que $u \circ j_\lambda = u_\lambda$ pour tout $\lambda \in L$. Le produit tensoriel gauche $\bigotimes_{\lambda \in L}^{\mathfrak{g}} \wedge (M_\lambda)$ est une algèbre *alternée*: en effet, pour L fini cela résulte de III, p. 54, prop. 14, et pour L quelconque, cela résulte de la définition de ce produit donnée dans III, p. 53, *Remarque* et du fait qu’une limite inductive d’algèbres graduées alternées est alternée. Comme en outre $u(M)$ est contenu dans le sous-module des éléments de degré 1 de l’algèbre graduée $\bigotimes_{\lambda \in L}^{\mathfrak{g}} \wedge (M_\lambda)$, il résulte de III, p. 77, prop. 1 et *Remarque* 1, qu’il existe un homomorphisme unique d’algèbres graduées
$$
h : \wedge (M) \to \bigotimes_{\lambda \in L}^{\mathfrak{g}} \wedge (M_\lambda)
$$
tel que $h \circ \varphi''_M = u$. La vérification du fait que $g \circ h$ et $h \circ g$ sont les applications identiques se fait alors comme dans III, p. 73, prop. 9 en remplaçant S par $\wedge$, et $\varphi'$ par $\varphi''$.

#### Remarque {#alg-iii-s7-n7-rem-1 .statement}

Soit $N = \bigoplus_{\lambda \in L} N_\lambda$ la somme directe d’une seconde famille de A-modules ayant L pour ensemble d’indices, et, pour tout $\lambda \in L$, soit $v_\lambda : M_\lambda \to N_\lambda$ une application A-linéaire, d’où une application A-linéaire $v = \bigoplus_{\lambda} v_{\lambda} : M \to N$ (II, p. 13, prop. 7). Alors le diagramme

$$
\begin{array}{ccc}
g \bigotimes_{\lambda \in L} \wedge (M_{\lambda}) & \xrightarrow{g_M} & \wedge (M) \\
\downarrow \wedge (v_{\lambda}) & & \downarrow \wedge (v) \\
g \bigotimes_{\lambda \in L} \wedge (N_{\lambda}) & \xrightarrow{g_N} & \wedge (N)
\end{array}
$$

est commutatif (cf. III, p. 43, corollaire).

On peut décrire de façon plus précise le sous-A-module de $g \bigotimes_{\lambda \in L} \wedge (M_{\lambda})$ auquel $\wedge^n(M)$ s’identifie au moyen de l’isomorphisme $g$. Pour toute partie finie $J$ de $L$, posons $E_J = g \bigotimes_{\lambda \in J} \wedge (M_{\lambda})$, de sorte que $g \bigotimes_{\lambda \in L} \wedge (M_{\lambda}) = \varprojlim E_J$ suivant l’ensemble filtrant $\mathcal{F}(L)$ des parties finies de $L$, par définition (III, p. 53, Remarque). Pour toute famille $\nu = (n_{\lambda}) \in \mathbf{N}^{(L)}$ (ayant donc un support fini) telle que $\sum_{\lambda \in L} n_{\lambda} = n$, et toute partie finie $J$ de $L$ contenant le support de la famille $\nu$, posons

$$(16)$$
$$
\wedge^{J,\nu}(M) = \bigotimes_{\lambda \in J} \wedge^{n_{\lambda}}(M_{\lambda})
$$

de sorte que le sous-module $E_{J,n}$ des éléments de degré $n$ de $E_J$ est la somme directe des $\wedge^{J,\nu}(M)$ pour toutes les familles $\nu$ de support contenu dans $J$ et telles que $\sum_{\lambda \in L} n_{\lambda} = n$ (III, p. 47, prop. 10 et p. 52). Posons par convention $\wedge^{J,\nu}(M) = \{0\}$ pour les familles $\nu$ dont le support n’est pas contenu dans $J$; alors on peut encore dire que $E_{J,n}$ est somme directe de tous les $\wedge^{J,\nu}(M)$, où $\nu$ parcourt l’ensemble $H_n$ de toutes les familles $\nu = (n_{\lambda})_{\lambda \in L}$ telles que $\sum_{\lambda \in L} n_{\lambda} = n$. Puisque $\wedge^0(M_{\lambda})$ s’identifie à $A$, il est clair en outre que pour deux parties finies $J \subset J'$ de $L$ et une famille $\nu$ de support contenu dans $J$, l’application canonique $\wedge^{J,\nu}(M) \to \wedge^{J',\nu}(M)$ (restriction à $\wedge^{J,\nu}(M)$ de l’application canonique $E_J \to E_{J'}$) est bijective. Si l’on pose, pour tout $\nu \in H_n$,

$$(17)$$
$$
\wedge^{\nu}(M) = \varprojlim \wedge^{J,\nu}(M)
$$

on voit donc que l’on a, compte tenu de II, p. 91, prop. 5:

#### Corollaire {#alg-iii-s7-n7-cor-1 .statement}

*Le A-module $\wedge^n(M)$ est l’image par l’isomorphisme (14) (III, p. 84) du sous-module de $g \bigotimes_{\lambda \in L} \wedge (M_{\lambda})$ somme directe des sous-modules $\wedge^{\nu}(M)$ pour toutes les familles $\nu = (n_{\lambda}) \in \mathbf{N}^{(L)}$ telles que $\sum_{\lambda \in L} n_{\lambda} = n$; si $J$ est le support de $\nu$, $\wedge^{\nu}(M)$ est canoniquement isomorphe à $\bigotimes_{\lambda \in J} \wedge^{n_{\lambda}}(M_{\lambda})$.*

On identifiera en général $\wedge^{\nu}(M)$, $\bigotimes_{\lambda \in J} \wedge^{n_{\lambda}}(M_{\lambda})$ et leur image dans $\wedge^n(M)$. Avec cette convention:

#### Proposition 11 {#alg-iii-s7-prop-11 .statement}

Soient $\Delta$ un monoïde commutatif à élément neutre, $M$ un $A$-module gradué de type $\Delta$, $(M_\alpha)_{\alpha \in \Delta}$ sa graduation. Pour tout couple $(\alpha, n) \in \Delta \times \mathbf{N}$, soit $\wedge^{\alpha, n}(M)$ le sous-module de $\wedge^n(M)$ somme directe des sous-modules $\bigotimes_{\lambda \in J} \wedge^{n_\lambda}(M_{\alpha_\lambda})$, où $(n_\lambda)_{\lambda \in L}$ parcourt l’ensemble des familles d’entiers $\geqslant 0$ telles que $\sum_{\lambda \in L} n_\lambda = n$, $J$ est son support et, pour chaque $(n_\lambda), (\alpha_\lambda)_{\lambda \in J}$ parcourt l’ensemble des familles de $\Delta^J$ telles que $\sum_{\lambda \in J} \alpha_\lambda = \alpha$. Alors $(\wedge^{\alpha, n}(M))_{(\alpha, n) \in \Delta \times \mathbf{N}}$ est la seule graduation de type $\Delta \times \mathbf{N}$ compatible avec la structure d’algèbre de $\wedge(M)$ et qui induise sur $M = \wedge^1(M)$ la graduation donnée.

Le fait que $\wedge(M)$ soit somme directe des $\wedge^{\alpha, n}(M)$ résulte de III, p. 85, corollaire; le reste de la démonstration est identique à la fin de la démonstration de III, p. 62, prop. 7.

### 8. Algèbre extérieure d’un module libre

#### Théorème 1 {#alg-iii-s7-thm-1 .statement}

Soit $M$ un $A$-module ayant une base $(e_\lambda)_{\lambda \in L}$. Munissons $L$ d’une structure d’ensemble totalement ordonné (E, III, p. 20, th. 1), et, pour toute partie finie $J$ de $L$, posons

$$
e_J = e_{\lambda_1} \wedge e_{\lambda_2} \wedge \cdots \wedge e_{\lambda_n}
$$

où $(\lambda_k)_{1 \leq k \leq n}$ est la suite des éléments de $J$ rangés dans l’ordre croissant (E, III, p. 38, prop. 6); on convient que $e_\varnothing = 1$, élément unité de $A$. Alors les $e_J$, où $J$ parcourt l’ensemble $\mathcal{F}(L)$ des parties finies de $L$, forment une base de l’algèbre extérieure $\wedge(M)$.

Puisque les $e_\lambda$ engendrent le $A$-module $M$, tout élément de $\wedge(M)$ est combinaison linéaire de produits d’éléments $e_\lambda$ en nombre fini, donc (compte tenu de III, p. 79, prop. 5) est une combinaison linéaire d’un nombre fini d’éléments $e_J$ pour $J \in \mathcal{F}(L)$. Tout revient à prouver que les $e_J$ sont linéairement indépendants sur $A$. Sinon, il existerait entre ces éléments une relation linéaire à coefficients non tous nuls; la réunion des parties $J$ qui correspondent aux $e_J$ dont le coefficient dans cette relation est $\neq 0$ est une partie finie $K$ de $L$ (puisque’il n’y a qu’un nombre fini de coefficients $\neq 0$). Soit $N$ le sous-module de $M$ engendré par les $e_\lambda$ tels que $\lambda \in K$; $N$ est facteur direct dans $M$, donc (III, p. 78) $\wedge(N)$ s’identifie à une sous-algèbre de $\wedge(M)$, et si nous montrons que les $e_J$, pour $J \subset K$, forment une base de $\wedge(N)$, nous arriverons à la contradiction cherchée.

Tout revient donc à prouver le th. 1 lorsque la base de $M$ est finie; on peut donc supposer que $L = \{1, m\} \subset \mathbf{N}$. Pour chaque $i \in L$, soit $M_i$ le sous-module libre $Ae_i$ de $M$; $M$ est somme directe des $M_i$, et $\wedge(M_i)$ est somme directe de $\wedge^0(M_i) = A$ et de $\wedge^1(M_i) = M_i$ (III, p. 80, prop. 6). Identifions canoniquement $\wedge(M)$ au $A$-module produit tensoriel des $\wedge(M_i)$ (III, p. 84, prop. 10); ce dernier a pour base le produit tensoriel des bases $(1, e_i)$ des $\wedge(M_i)$ (II, p. 62, cor. 2); on obtient ainsi tous les éléments

$$
u_1 \otimes u_2 \otimes \cdots \otimes u_m
$$

où l’on a, soit $u_i = 1$, soit $u_i = e_i$; si $J$ est l’ensemble des indices $i$ tels que $u_i = e_i$, $u_1 \otimes u_2 \otimes \cdots \otimes u_m$ est identifié à $e_J$, ce qui termine la démonstration.

#### Corollaire 1 {#alg-iii-s7-thm-1-cor-1 .statement}

*Supposons que $L = \{1, m\}$; alors la base $(e_J)_{J \in \mathcal{B}(L)}$ de $\wedge(M)$ a $2^m$ éléments. Pour $p > m$, on a $\wedge^p(M) = \{0\}$; $\wedge^m(M)$ a une base formée d’un seul élément $e_L$; pour $0 \leq p \leq m$, le nombre d’éléments de la base $(e_J)$ de $\wedge^p(M)$ formée des $e_J$ tels que $\mathrm{Card}(J) = p$, est $\binom{m}{p} = \frac{m!}{p!(m-p)!}$.

Cela résulte de E, III, p. 29, prop. 12 et E, III, p. 42, cor. 1.

Revenons au cas où l’ensemble $L$ du th. 1 est quelconque, et explicitons la *table de multiplication* (III, p. 10) de la base $(e_J)$. Etant données deux parties finies $J, K$ de l’ensemble totalement ordonné $L$, posons

$$
\begin{cases}
\rho_{J, K} = 0 & \text{si } J \cap K \neq \varnothing \\
\rho_{J, K} = (-1)^v & \text{si } J \cap K = \varnothing
\end{cases}
$$

en désignant dans ce dernier cas par $v$ le nombre des couples $(\lambda, \mu) \in J \times K$ tels que $\lambda > \mu$. Alors le cor. 1 de III, p. 79 entraîne aussitôt la relation

$$
e_J \wedge e_K = \rho_{J, K} e_{J \cup K}.
$$

On notera la formule

$$
\rho_{J, K} \rho_{K, J} = (-1)^{jk}
$$

lorsque $J \cap K = \varnothing$, $j = \mathrm{Card}(J)$ et $k = \mathrm{Card}(K)$ (III, p. 80, cor. 2).

#### Corollaire 2 {#alg-iii-s7-thm-1-cor-2 .statement}

*Si $M$ est un $A$-module projectif, $\wedge(M)$ est un $A$-module projectif.*

La démonstration est la même que celle de III, p. 62, corollaire, en remplaçant $T$ par $\wedge$.

#### Corollaire 3 {#alg-iii-s7-thm-1-cor-3 .statement}

*Soient $M$ un $A$-module projectif, $(x_i)_{1 \leq i \leq n}$ une suite finie d’éléments de $M$. Pour qu’il existe sur $M$ une forme $n$-linéaire alternée $f$ telle que $f(x_1, x_2, \ldots, x_n) \neq 0$, il faut et il suffit que $x_1 \wedge x_2 \wedge \cdots \wedge x_n \neq 0$.

On sait déjà (sans hypothèse sur $M$) que la condition est nécessaire (III, p. 80, prop. 7). Supposons maintenant que $M$ soit projectif et que

$$
x_1 \wedge x_2 \wedge \cdots \wedge x_n \neq 0.
$$

Alors $\wedge^n(M)$ est projectif (cor. 2), donc l’application canonique

$$
\wedge^n(M) \to (\wedge^n(M))^**
$$

est injective (II, p. 47, cor. 4); on en conclut qu’il existe une forme linéaire $g : \wedge^n(M) \to A$ telle que $g(x_1 \wedge x_2 \wedge \cdots \wedge x_n) \neq 0$. Si $f$ est la forme $n$-linéaire alternée correspondant à $g$ (III, p. 80, prop. 7), on a donc $f(x_1, \ldots, x_n) \neq 0$.

### 9. Critères d’indépendance linéaire

#### Proposition 12 {#alg-iii-s7-prop-12 .statement}

Soit M un A-module projectif. Pour que des éléments $x_1, x_2, \ldots, x_n$ de M soient linéairement dépendants, il faut et il suffit qu’il existe $\lambda \neq 0$ dans A tel que
$$
\lambda x_1 \wedge x_2 \wedge \cdots \wedge x_n = 0.
$$
La condition est nécessaire (sans hypothèse sur M), car si, par exemple, $\lambda x_1$ (avec $\lambda \neq 0$) est combinaison linéaire de $x_2, \ldots, x_n$, la relation (22) a lieu (III, p. 79, prop. 5). Montrons que la condition est suffisante par récurrence sur n; pour $n = 1$, c’est une conséquence triviale de la définition. Supposons donc $n > 1$ et la condition (22) vérifiée pour un $\lambda \neq 0$. Si $\lambda x_2 \wedge x_3 \wedge \cdots \wedge x_n = 0$, alors l’hypothèse de récurrence entraîne que $x_2, \ldots, x_n$ sont linéairement dépendants, donc a fortiori $x_1, x_2, \ldots, x_n$ le sont. Si $\lambda x_2 \wedge x_3 \wedge \cdots \wedge x_n \neq 0$, il résulte de III, p. 87, cor. 3, qu’il existe une forme $(m - 1)$-linéaire alternée $f$ telle que $f(\lambda x_2 \wedge x_3 \wedge \cdots \wedge x_n) = \mu \neq 0$. Puisque l’on a
$$
x_1 \wedge (\lambda x_2) \wedge \cdots \wedge x_n = 0,
$$
il résulte de III, p. 87, cor. 3, que $\mu x_1$ est combinaison linéaire de $\lambda x_2, x_3, \ldots, x_n$; donc $x_1, x_2, \ldots, x_n$ sont linéairement dépendants.

#### Corollaire {#alg-iii-s7-n9-cor-1 .statement}

Soient M et N deux A-modules projectifs, et soit $f : M \to N$ une application A-linéaire. Si f est injective, alors $\wedge(f) : \wedge(M) \to \wedge(N)$ est injective.

Démontrons-le d’abord en supposant que M soit libre; soit $(e_\lambda)_{\lambda \in L}$ une base de M, de sorte que $(e_J)_{J \in \mathfrak{F}(L)}$ (formule (18)) est une base de $\wedge(M)$. Supposons que le noyau de $\wedge(f)$ contienne un élément $u = \sum_J \alpha_J e_J \neq 0$. Soit K un élément minimal parmi les parties finies J telles que $\alpha_J \neq 0$, et soit H une partie finie de L, disjointe de K et telle que $K \cup H$ contienne tous les J (en nombre fini) tels que $\alpha_J \neq 0$; pour tout $J \neq K$ tel que $\alpha_J \neq 0$, on a donc par définition $J \cap H \neq \varnothing$, et par suite (III, p. 87, formule (20))
$$
u \wedge e_H = \pm \alpha_K e_{K \cup H}
$$
appartient à l’idéal bilatère de $\wedge(M)$, noyau de $\wedge(f)$. Posons $e_{K \cup H} = e_{\lambda_1} \wedge e_{\lambda_2} \wedge \cdots \wedge e_{\lambda_n}$; on a donc $\alpha_K f(e_{\lambda_1}) \wedge f(e_{\lambda_2}) \wedge \cdots \wedge f(e_{\lambda_n}) = 0$; en vertu de la prop. 12, les éléments $f(e_{\lambda_i})$ ($1 \leq i \leq n$) de N sont linéairement dépendants. Mais ceci contredit l’hypothèse que f est injectif (II, p. 25, cor. 3).

Abordons maintenant le cas général, et soit $M'$ un A-module tel que $M \oplus M' = P$ soit libre (II, p. 39, prop. 4). Considérons l’application linéaire $g : M \oplus M' \to N \oplus M \oplus M'$ telle que $g(x, y) = (f(x), 0, y)$, de sorte qu’on a le diagramme commutatif

$$
\begin{array}{ccc}
M & \xrightarrow{f} & N \\
\downarrow & & \downarrow \\
P & \xrightarrow{g} & N \oplus P
\end{array}
$$

où les flèches verticales sont les injections canoniques. Puisque $g$ est injective et $P$ libre, $\wedge(g)$ est un homomorphisme injectif comme on l’a vu plus haut. Or, $\wedge(j): \wedge(M) \to \wedge(P)$ est un homomorphisme injectif puisque $M$ est facteur direct dans $P$ (III, p. 78). L’homomorphisme composé
$$
\wedge(M) \xrightarrow{\wedge(j)} \wedge(P) \xrightarrow{\wedge(g)} \wedge(N \oplus P)
$$
est donc injectif, et comme il est aussi égal, à l’homomorphisme composé
$$
\wedge(M) \xrightarrow{\wedge(f)} \wedge(N) \xrightarrow{\wedge(g')} \wedge(N \oplus P)
$$
on en conclut que $\wedge(f)$ est injectif.

#### Proposition 13 {#alg-iii-s7-prop-13 .statement}

*Soient $M$ un $A$-module, $N$ un sous-module facteur direct de $M$ qui est libre de dimension $p$, $\{u\}$ une base de $\wedge^p(N)$. Pour qu’un élément $x \in M$ appartienne à $N$, il faut et il suffit que $u \wedge x = 0$.*

Soit $P$ un sous-module de $M$ supplémentaire de $N$, et soient $y \in N$, $z \in P$ tels que $x = y + z$. Alors $u \wedge x = u \wedge z$. Comme $\wedge^p(N)$ est libre de dimension 1, l’application $\varphi : P \to P \otimes \wedge^p(N)$ telle que $\varphi(p) = p \otimes u$ est bijective (II, p. 55, prop. 4). D’autre part (III, p. 84, prop. 10), le composé des homomorphismes canoniques
$$
\psi : P \otimes \wedge^p(N) \to \wedge(P) \otimes \wedge(N) \to \wedge(M)
$$
est injectif. L’application $\psi \circ \varphi$ est donc injective, d’où la proposition.

#### Théorème 2 {#alg-iii-s7-thm-2 .statement}

*Soit $M$ un $A$-module ayant une base finie $(e_i)_{1 \leq i \leq n}$. Pour qu’une suite $(x_i)_{1 \leq i \leq n}$ de $n$ éléments de $M$ forme une base de $M$, il faut et il suffit que l’élément $\lambda \in A$ tel que*
$$
x_1 \wedge x_2 \wedge \cdots \wedge x_n = \lambda \cdot e_1 \wedge e_2 \wedge \cdots \wedge e_n
$$
*soit inversible dans $A$.*

Rappelons que $e_1 \wedge e_2 \wedge \cdots \wedge e_n$ est l’unique élément d’une base de $\wedge^n(M)$ (III, p. 87, cor. 1) de sorte que l’élément $\lambda \in A$ vérifiant (23) est déterminé de façon unique. Si $(x_i)_{1 \leq i \leq n}$ est une base de $M$, $x_1 \wedge x_2 \wedge \cdots \wedge x_n$ est l’unique élément d’une base de $\wedge^n(M)$ (III, p. 87), donc $\lambda$ est inversible. Réciproquement, supposons $\lambda$ inversible; alors la forme $n$-linéaire alternée $f$ correspondant à l’application linéaire $g : \wedge^n(M) \to A$ telle que $g(e_1 \wedge e_2 \wedge \cdots \wedge e_n) = \lambda^{-1}$, est telle que $f(x_1, x_2, \ldots, x_n) = 1$. Pour tout $x \in M$, on a évidemment
$$
x \wedge x_1 \wedge \cdots \wedge x_n = 0
$$
(III, p. 80, prop. 6); appliquant III, p. 87, cor. 3, on obtient
$$
f(x_1, x_2, \ldots, x_n)x = \sum_{i=1}^n (-1)^{i-1} f(x, x_1, \ldots, \hat{x}_i, \ldots, x_n)x_i.
$$
Comme $f(x_1, \ldots, x_n) = 1$, cela montre que tout $x \in M$ est combinaison linéaire de $x_1, x_2, \ldots, x_n$, et comme ces derniers sont linéairement indépendants (puisque $x_1 \wedge x_2 \wedge \cdots \wedge x_n \neq 0$), ils forment une base de $M$.

## EXERCICES {#alg-iii-s7-exercises}

See the [exercises for § 7](exercises/s7/).
