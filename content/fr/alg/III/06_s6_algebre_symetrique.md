---
book: alg
book_title: Algebra
chapter: III
chapter_title: ALGÈBRES TENSORIELLES, ALGÈBRES EXTÉRIEURES, ALGÈBRES SYMÉTRIQUES
section: 6
section_title: Algèbre symétrique
lang: fr
source: alg-i-iii-fr
book_pages: A III.188-A III.189
pdf_pages: 0454-0463, 0575-0576
extraction: ocr
subsections:
    - "no": 1
      title: Définition de l’algèbre symétrique d’un module
      page: 0
      pdf_page: 454
    - "no": 2
      title: Propriétés fonctorielles de l’algèbre symétrique
      page: 68
      pdf_page: 455
    - "no": 3
      title: Puissance symétrique $n$-ème d’un module et applications multilinéaires symétriques
      page: 70
      pdf_page: 457
    - "no": 4
      title: Extension de l’anneau des scalaires
      page: 72
      pdf_page: 459
    - "no": 5
      title: Limite inductive d’algèbres symétriques
      page: 72
      pdf_page: 459
    - "no": 6
      title: Algèbre symétrique d’une somme directe. Algèbre symétrique d’un module libre. Algèbre symétrique d’un module gradué.
      page: 73
      pdf_page: 460
statements: 19
exercises: 5
content_sha256: 40f152bcd1e869e851df2deb19631a5d9be1b26d27d6a38bfc42fdabc3f51e63
---

## § 6. ALGÈBRE SYMÉTRIQUE

### 1. Définition de l’algèbre symétrique d’un module

#### Définition 1 {#alg-iii-s6-def-1 .statement}

Soient $A$ un anneau commutatif, $M$ un $A$-module. On appelle algèbre symétrique de $M$, et on note $S(M)$ ou $\mathrm{Sym}(M)$ ou $S_A(M)$, l’algèbre sur $A$ quotient de l’algèbre tensorielle $T(M)$ par l’idéal bilatère $\mathfrak{J}'$ (aussi noté $\mathfrak{J}_M$) engendré par les éléments $xy - yx = x \otimes y - y \otimes x$ de $T(M)$, où $x$ et $y$ parcourent $M$.

L’idéal $\mathfrak{J}'$ étant engendré par des éléments homogènes de degré 2, est un idéal gradué (II, p. 167, prop. 2); on pose $\mathfrak{J}'_n = \mathfrak{J}' \cap T^n(M)$; l’algèbre $S(M)$ est donc graduée par la graduation (dite canonique) formée des $S^n(M) = T^n(M)/\mathfrak{J}'_n$. On a $\mathfrak{J}'_0 = \mathfrak{J}'_1 = \{0\}$, donc $S^0(M)$ s’identifie canoniquement à $A$ et $S^1(M)$ à $T^1(M) = M$; nous ferons toujours par la suite ces identifications, et nous noterons $\varphi'$ ou $\varphi'_M$ l’injection canonique $M \to S(M)$.

#### Proposition 1 {#alg-iii-s6-prop-1 .statement}

L’algèbre $S(M)$ est commutative.

En effet, on a par définition $\varphi'(x)\varphi'(y) = \varphi'(y)\varphi'(x)$ pour $x, y$ dans $M$, et comme les éléments $\varphi'(x)$, où $x$ parcourt $M$, engendrent $S(M)$, la conclusion résulte de III, p. 11.

#### Proposition 2 {#alg-iii-s6-prop-2 .statement}

Soient $E$ une $A$-algèbre, $f : M \to E$ une application $A$-linéaire telle que
$$
f(x)f(y) = f(y)f(x) \text{ quels que soient } x, y \text{ dans } M.
$$

Il existe un homomorphisme et un seul de A-algèbres $g : S(M) \to E$ tel que $f = g \circ \varphi'$.

En d’autres termes, $(S(M), \varphi')$ est solution du problème d’application universelle (E, IV, p. 23), où $\Sigma$ est l’espèce de structure de A-algèbre, les $\alpha$-applications étant les applications linéaires du A-module M dans une A-algèbre vérifiant (1).

L’unicité de $g$ résulte de ce que $\varphi'(M) = M$ engendre $S(M)$. Pour prouver l’existence de $g$, notons qu’en vertu de III, p. 56, prop. 1, il existe un homomorphisme $g_1 : T(M) \to E$ de A-algèbres tel que $f = g_1 \circ \varphi$; tout revient à voir que $g_1$ s’annule dans l’idéal $\mathfrak{J}'$, car alors, si $p : T(M) \to S(M) = T(M)/\mathfrak{J}'$ est l’homomorphisme canonique, on pourra écrire $g_1 = g \circ p$, où $g : S(M) \to E$ est un homomorphisme d’algèbres, et la conclusion résultera de ce que $p \circ \varphi = \varphi'$. Or le noyau de $g_1$ est un idéal bilatère qui, en vertu de (1) et de la relation $g_1 \circ \varphi = f$, contient les éléments $x \otimes y - y \otimes x$ pour $x, y$ dans M. Ceci termine la démonstration.

#### Remarque 1 {#alg-iii-s6-n1-rem-1 .statement}

Supposons que E soit une A-algèbre graduée de type $\mathbf{Z}$, de graduation $(E_n)$, et supposons en outre que l’application linéaire $f$ (supposée vérifier (1)) soit telle que
$$
f(M) \subset E_1.
$$
Alors la relation $g(x_1 x_2 \ldots x_p) = f(x_1) f(x_2) \ldots f(x_p)$ pour les $x_i \in M$ montre que $g(S^p(M)) \subset E_p$ pour tout $p \geq 0$, donc $g$ est un homomorphisme d’algèbres graduées.

#### Remarque 2 {#alg-iii-s6-n1-rem-2 .statement}

Tout élément de $S(M)$ est somme de produits de la forme $x_1 x_2 \ldots x_n$, où les $x_i$ appartiennent à M; on aura soin de ne pas confondre de tels produits pris dans $S(M)$ et les produits analogues pris dans $T(M)$.

#### Remarque 3 {#alg-iii-s6-n1-rem-3 .statement}

Si $n! . 1$ est inversible dans A, le A-module $S^n(M)$ est engendré par les éléments de la forme $x^n$, où $x \in M$; cela résulte de la remarque précédente et de (I, p. 95, prop. 2).

### 2. Propriétés fonctorielles de l’algèbre symétrique

#### Proposition 3 {#alg-iii-s6-prop-3 .statement}

Soient A un anneau commutatif, M et N deux A-modules, $u : M \to N$ une application A-linéaire. Il existe un homomorphisme de A-algèbres et un seul, $u' : S(M) \to S(N)$, tel que le diagramme

$$
\begin{array}{ccc}
M & \xrightarrow{u} & N \\
\varphi'_M \downarrow & & \varphi'_N \downarrow \\
S(M) & \xrightarrow{u'} & S(N)
\end{array}
$$

soit commutatif. En outre, $u'$ est un homomorphisme d’algèbres graduées.

L’existence et l’unicité de $u'$ résultent de III, p. 67, prop. 2, appliquée à l’algèbre commutative $S(N)$ et à $f = \varphi'_N \circ u : M \to S(N)$; comme
$$
f(M) \subset S^1(N) = N,
$$

le fait que $u'$ soit un homomorphisme d’algèbres graduées résulte de III, p. 68, Remarque 1.

L’homomorphisme $u'$ de la prop. 3 sera désormais noté $S(u)$. Si P est un A-module et $v : N \to P$ une application A-linéaire, on a
$$
S(v \circ u) = S(v) \circ S(u)
$$
car $S(v) \circ S(u)$ est un homomorphisme d’algèbres qui rend commutatif le diagramme

$$
\begin{array}{ccc}
M & \xrightarrow{v \circ u} & P \\
\downarrow \varphi'_M & & \downarrow \varphi'_P \\
S(M) & \xrightarrow{S(v) \circ S(u)} & S(P)
\end{array}
$$

Comme $S(M)$ contient $M = S^1(M)$, on dit parfois que $S(u)$ est le prolongement canonique de $u$ à $S(M)$. La restriction $S^n(u) : S^n(M) \to S^n(N)$ est telle que
$$
S^n(u)(x_1 x_2 \ldots x_n) = u(x_1) u(x_2) \ldots u(x_n)
$$
pour les $x_i \in M$, puisque $S(u)$ est un homomorphisme d’algèbres et $S^1(u) = u$; la restriction $S^0(u)$ à $A$ est l’application identique. On notera que $S^n(u)$ provient de $T^n(u) : T^n(M) \to T^n(N)$ par passage aux quotients.

#### Proposition 4 {#alg-iii-s6-prop-4 .statement}

*Si $u : M \to N$ est une application A-linéaire surjective, l’homomorphisme $S(u) : S(M) \to S(N)$ est surjectif, et son noyau est l’idéal de $S(M)$ engendré par le noyau $P \subset M \subset S(M)$ de $u$.

Posons $v = T(u) : T(M) \to T(N)$; on sait (III, p. 57, prop. 3) que $v$ est surjective, donc il résulte des définitions que l’on a $v(\mathfrak{J}'_M) = \mathfrak{J}'_N$; si $\mathfrak{R}$ est le noyau de $v$, on a par suite $v^{-1}(\mathfrak{J}'_N) = \mathfrak{R} + \mathfrak{J}'_M$. Comme $S(u) : T(M)/\mathfrak{J}'_M \to T(N)/\mathfrak{J}'_N$ se déduit de $v$ par passage aux quotients, c’est un homomorphisme surjectif dont le noyau est $\mathfrak{R}' = (\mathfrak{R} + \mathfrak{J}'_M)/\mathfrak{J}'_M$. Comme $\mathfrak{R}$ est engendré par le noyau $P$ de $u$ (III, p. 57), il en est de même de $\mathfrak{R}'$.

Si $u : M \to N$ est une application linéaire injective, il n’est pas toujours vrai que $S(u)$ soit une application injective (III, p. 187, exerc. 1). Toutefois il en est ainsi lorsque $u$ est une injection telle que $u(M)$ soit facteur direct de $N$, et alors l’image de $S(u)$ (isomorphe à $S(M)$) est facteur direct de $S(N)$; la démonstration est la même que celle des assertions analogues pour $T(u)$ (III, p. 58) en remplaçant $T$ par $S$.

#### Proposition 5 {#alg-iii-s6-prop-5 .statement}

*Soient $N$ et $P$ deux sous-modules d’un A-module $M$, tels que leur somme $N + P$ soit facteur direct dans $M$, et que leur intersection $N \cap P$ soit facteur direct dans $N$ et dans $P$. Alors les homomorphismes $S(N) \to S(M)$, $S(P) \to S(M)$ et $S(N \cap P) \to S(M)$ prolongements canoniques des injections canoniques, sont injectifs; si l’on identifie $S(N)$, $S(P)$ et $S(N \cap P)$ à des sous-algèbres de $S(M)$ au moyen de ces homomorphismes, on a*
$$
S(N \cap P) = S(N) \cap S(P).
$$

La démonstration se déduit de celle de III, p. 58–59, prop. 4, en remplaçant partout $T$ par $S$. Les hypothèses de la prop. 5 sont toujours vérifiées pour des sous-modules quelconques $N, P$ de $M$ lorsque $A$ est un corps.

#### Corollaire {#alg-iii-s6-n2-cor-1 .statement}

Soient $K$ un corps commutatif, $M$ un espace vectoriel sur $K$. Pour tout élément $z \in S(M)$, il existe un plus petit sous-espace vectoriel $N$ de $M$ tel que $z \in S(N)$, et $N$ est de dimension finie.

La démonstration se déduit de celle de III, p. 59, corollaire, en remplaçant partout $T$ par $S$.

On dit que $N$ est le sous-espace vectoriel de $M$ associé à $z$.

### 3. Puissance symétrique $n$-ème d’un module et applications multilinéaires symétriques

Soient $X, Y$ deux ensembles, $n$ un entier $\geqslant 1$. On appelle application symétrique de $X^n$ dans $Y$ toute application $f : X^n \to Y$ telle que, pour toute permutation $\sigma \in \mathfrak{S}_n$ et tout élément $(x_i) \in X^n$, on ait
$$
f(x_{\sigma(1)}, x_{\sigma(2)}, \ldots, x_{\sigma(n)}) = f(x_1, x_2, \ldots, x_n).
$$
Comme les transpositions échangeant deux entiers consécutifs engendrent le groupe $\mathfrak{S}_n$ (I, p. 61), il suffit que la condition (5) soit vérifiée lorsque $\sigma$ est une telle transposition.

Lorsque $Y$ est un module sur un anneau commutatif $A$, il est clair que l’ensemble des applications symétriques de $X^n$ dans $Y$ est un sous-module du $A$-module $Y^{X^n}$ de toutes les applications de $X^n$ dans $Y$.

#### Proposition 6 {#alg-iii-s6-prop-6 .statement}

Soient $A$ un anneau commutatif, $M$ et $N$ deux $A$-modules. Si, à toute application $A$-linéaire $g : S^n(M) \to N$ ($n \geqslant 1$) on associe l’application $n$-linéaire
$$
(x_1, x_2, \ldots, x_n) \mapsto g(x_1 x_2 \ldots x_n)
$$
(où au second membre le produit est pris dans l’algèbre $S(M)$), on obtient une application $A$-linéaire bijective du $A$-module $\mathrm{Hom}_A(S^n(M), N)$ sur le $A$-module des applications $n$-linéaires symétriques de $M^n$ dans $N$.

Rappelons (II, p. 71) qu’on a une bijection canonique du $A$-module $\mathrm{Hom}_A(T^n(M), N)$ sur le $A$-module $\mathcal{L}_n(M, \ldots, M; N)$ de toutes les applications $n$-linéaires de $M^n$ dans $N$, en associant à toute application $A$-linéaire $f : T^n(M) \to N$ l’application $n$-linéaire
$$
\bar{f} : (x_1, x_2, \ldots, x_n) \mapsto f(x_1 \otimes x_2 \otimes \cdots \otimes x_n).
$$

D’autre part, les applications $A$-linéaires $g : S^n(M) \to N$ correspondent bi-univoquement aux applications $A$-linéaires $f : T^n(M) \to N$ telles que $f$ s’annule dans $\mathfrak{S}_n'$, en associant à $g$ l’application $f = g \circ p_n$, où $p_n : T^n(M) \to S^n(M) = T^n(M)/\mathfrak{S}_n'$ est l’homomorphisme canonique (II, p. 36, th. 1). Mais comme $\mathfrak{S}_n'$ est combinaison linéaire d’éléments de la forme
$$
(u_1 \otimes u_2 \otimes \cdots \otimes u_p) \otimes (x \otimes y - y \otimes x) \otimes (v_1 \otimes \cdots \otimes v_{n-p-2})
$$

(x, y, u_i, v_j dans M), dire que la fonction $f$ est de la forme $g \circ p_n$ signifie que la fonction $n$-linéaire correspondante $\bar{f}$ vérifie la relation

$$
\bar{f}(u_1, \ldots, u_p, x, y, v_1, \ldots, v_{n-p-2}) = \bar{f}(u_1, \ldots, u_p, y, x, v_1, \ldots, v_{n-p-2});
$$

autrement dit, d’après ce qu’on a vu plus haut, cela signifie que $\bar{f}$ est symétrique; d’où la proposition, compte tenu de ce que $p_n(x_1 \otimes x_2 \otimes \cdots \otimes x_n) = x_1 x_2 \cdots x_n$ pour les $x_i \in M$.

On dit que le A-module $S^n(M)$ est la puissance symétrique $n$-ème de M. Pour tout homomorphisme de A-modules $u : M \to N$, l’application $S^n(u) : S^n(M) \to S^n(N)$ qui coïncide avec $S(u)$ dans $S^n(M)$ s’appelle la puissance symétrique $n$-ème de $u$.

#### Remarque {#alg-iii-s6-n3-rem-1 .statement}

Soit $\sigma$ une permutation de $\mathfrak{S}_n$; comme l’application

$$
(x_1, x_2, \ldots, x_n) \mapsto x_{\sigma^{-1}(1)} \otimes x_{\sigma^{-1}(2)} \otimes \cdots \otimes x_{\sigma^{-1}(n)}
$$

de $M^n$ dans $T^n(M)$ est A-multilinéaire, elle s’écrit d’une seule manière

$$
(x_1, \ldots, x_n) \mapsto u_\sigma(x_1 \otimes x_2 \otimes \cdots \otimes x_n),
$$

où $u_\sigma$ est un endomorphisme du A-module $T^n(M)$, qu’on écrit aussi $z \mapsto \sigma . z$. Il est clair que si $\sigma$ est l’élément neutre de $\mathfrak{S}_n$, $u_\sigma$ est l’identité; d’autre part, lorsqu’on pose $y_i = x_{\sigma^{-1}(i)}$, on a, pour toute permutation $\tau \in \mathfrak{S}_n$, $y_{\tau^{-1}(i)} = x_{\sigma^{-1}(\tau^{-1}(i))}$, donc $\tau . (\sigma . z) = (\tau \sigma) . z$; autrement dit, le A-module $T^n(M)$ est un $\mathfrak{S}_n$-ensemble à gauche pour l’opération $(\sigma, z) \mapsto \sigma . z$ (I, p. 50). Les éléments de $T^n(M)$ tels que $\sigma . z = z$ pour tout $\sigma \in \mathfrak{S}_n$, sont appelés tenseurs symétriques (contravariants) d’ordre $n$; ils forment un sous-A-module $S'_n(M)$ de $T^n(M)$.

Pour tout $z \in T^n(M)$, on pose $s . z = \sum_{\sigma \in \mathfrak{S}_n} \sigma . z$, et on dit que $s . z$ est le symétrisé du tenseur $z$; il est clair que $s . z$ est un tenseur symétrique, et par suite $z \mapsto s . z$ est un endomorphisme de $T^n(M)$ dont l’image $S''_n(M)$ est contenue dans $S'_n(M)$; en général, on a $S''_n(M) \neq S'_n(M)$ (III, p. 188, exerc. 5). Si $z$ est un tenseur symétrique, on a $s . z = n! z$; on en conclut que lorsque $n!$ est inversible dans A, l’endomorphisme $z \mapsto (n!)^{-1} s . z$ est un projecteur dans $T^n(M)$ (II, p. 18), dont l’image est $S'_n(M) = S''_n(M)$; en outre le noyau de ce projecteur n’est autre que $\mathfrak{J}'_n$. En effet, on a évidemment $\sigma(\mathfrak{J}'_n) \subset \mathfrak{J}'_n$ pour tout $\sigma \in \mathfrak{S}_n$, et $\mathfrak{J}'_n$ est par définition engendré par les tenseurs $z - \rho . z$, où $\rho$ est une transposition échangeant deux nombres consécutifs dans $\{1, n\}$; en outre, si $\sigma, \tau$ sont deux permutations de $\mathfrak{S}_n$, on a $z - (\sigma \tau) . z = z - \sigma . z + \sigma . (z - \tau . z)$, d’où l’on déduit (puisque toute permutation de $\mathfrak{S}_n$ est produit de transpositions échangeant deux nombres consécutifs) que $z - \sigma . z \in \mathfrak{J}'_n$ quels que soient $z \in T^n(M)$ et $\sigma \in \mathfrak{S}_n$. Par suite (toujours en supposant $n!$ inversible dans A), on voit que $z - (n!)^{-1} s . z = \sum_{\sigma \in \mathfrak{S}_n} (n!)^{-1} (z - \sigma . z) \in \mathfrak{J}'_n$ pour tout $z \in T^n(M)$, ce qui démontre notre assertion.

Lorsque $n!$ est inversible dans A, les sous-modules $S'_n(M)$ et $\mathfrak{J}'_n$ de $T^n(M)$ sont donc supplémentaires, et la restriction à $S'_n(M)$ de l’homomorphisme canonique $T^n(M) \to S^n(M) = T^n(M)/\mathfrak{J}'_n$ est un isomorphisme de $A$-modules, qui permet dans le cas envisagé d’identifier les tenseurs symétriques d’ordre $n$ aux éléments de la puissance symétrique $n$-ème de $M$. On notera toutefois que cette identification n’est pas compatible avec la multiplication, le produit (dans $T(M)$) de deux tenseurs symétriques n’étant pas symétrique en général, et n’ayant donc pas pour image dans $S(M)$ le produit des images des tenseurs symétriques considérés.

### 4. Extension de l’anneau des scalaires

Soient $A, A'$ deux anneaux commutatifs, $\rho : A \to A'$ un homomorphisme d’anneaux, $M$ un $A$-module, $M'$ un $A'$-module, $f : M \to M'$ un $A$-homomorphisme (relatif à $\rho$) de $M$ dans $M'$. L’application composée $M \xrightarrow{f} M' \xrightarrow{\varphi'_{M'}} S_{A'}(M')$ est une application $A$-linéaire de $M$ dans la $A$-algèbre commutative $\rho_* (S_{A'}(M'))$; il existe donc (III, p. 67, prop. 2) un $A$-homomorphisme d’algèbres et un seul $f' : S_A(M) \to S_{A'}(M')$ rendant commutatif le diagramme

$$
\begin{array}{ccc}
M & \xrightarrow{f} & M' \\
\varphi'_M \downarrow & & \downarrow \varphi'_{M'} \\
S_A(M) & \xrightarrow{f'} & S_{A'}(M')
\end{array}
$$

On en déduit aussitôt que si $\sigma : A' \to A''$ est un second homomorphisme d’anneaux, $M''$ un $A''$-module, $g : M' \to M''$ un $A'$-homomorphisme (relatif à $\sigma$), $g' : S_{A'}(M') \to S_{A''}(M'')$ le $A'$-homomorphisme d’algèbres correspondant, alors le $A$-homomorphisme d’algèbres composé

$$
S_A(M) \xrightarrow{f'} S_{A'}(M') \xrightarrow{g'} S_{A''}(M'')
$$

correspond au $A$-homomorphisme composé $g \circ f : M \to M''$ (relatif à $\sigma \circ \rho$).

#### Proposition 7 {#alg-iii-s6-prop-7 .statement}

Soient $A, B$ deux anneaux commutatifs, $\rho : A \to B$ un homomorphisme d’anneaux, $M$ un $A$-module. Le prolongement canonique

$$
\psi : S_B(B \otimes_A M) \to B \otimes_A S_A(M)
$$

de l’application $B$-linéaire $1_B \otimes \varphi'_M : B \otimes_A M \to B \otimes_A S_A(M)$, est un isomorphisme de $B$-algèbres graduées.

La démonstration se déduit de celle de III, p. 60, prop. 5 en y remplaçant $T$ par $S$ et $\varphi_M$ par $\varphi'_M$.

### 5. Limite inductive d’algèbres symétriques

Soient $(A_\alpha, \varphi_{\beta \alpha})$ un système inductif filtrant d’anneaux commutatifs, $(M_\alpha, f_{\beta \alpha})$ un système inductif de $A_\alpha$-modules, $A = \lim \to A_\alpha, M = \lim \to M_\alpha$. Pour $\alpha \leq \beta$, on déduit canoniquement du $A_\alpha$-homomorphisme $f_{\beta \alpha}: M_\alpha \to M_\beta$ un homomorphisme de $A_\alpha$-algèbres (III, p. 72, formule (8)), $f'_{\beta \alpha}: S_{A_\alpha}(M_\alpha) \to S_{A_\beta}(M_\beta)$ et il résulte de (9) (III, p. 72) que $(S_{A_\alpha}(M_\alpha), f'_{\beta \alpha})$ est un *système inductif de $A_\alpha$-algèbres*. Soit d’autre part $f_\alpha: M_\alpha \to M$ le $A_\alpha$-homomorphisme canonique; on en déduit (III, p. 72, formule (8)) un homomorphisme de $A_\alpha$-algèbres, $f'_\alpha: S_{A_\alpha}(M_\alpha) \to S_A(M)$, et il résulte encore de (9) que les $f'_\alpha$ constituent un système inductif de $A_\alpha$-homomorphismes.

#### Proposition 8 {#alg-iii-s6-prop-8 .statement}

*Le A-homomorphisme* $f' = \varprojlim f'_\alpha : \varprojlim S_{A_\alpha}(M_\alpha) \to S_A(M)$ *est un isomorphisme d’algèbres graduées*.

La démonstration est la même que celle de III, p. 61, prop. 6, en y remplaçant partout $T$ par $S$ et $\varphi$ et $\varphi'$, et tenant compte du fait qu’une limite inductive d’algèbres commutatives est commutative.

### 6. Algèbre symétrique d’une somme directe. Algèbre symétrique d’un module libre. Algèbre symétrique d’un module gradué.

Soient $A$ un anneau commutatif, $M = \bigoplus_{\lambda \in L} M_\lambda$ la somme directe d’une famille de $A$-modules, $j_\lambda: M_\lambda \to M$ l’injection canonique; on en déduit un $A$-homomorphisme d’algèbres $S(j_\lambda): S(M_\lambda) \to S(M)$. Puisque $S(M)$ est commutative, on peut appliquer aux homomorphismes $S(j_\lambda)$ la prop. 8 de III, p. 42, et il existe donc un unique homomorphisme d’algèbres

$$
g : \bigotimes_{\lambda \in L} S(M_\lambda) \to S(M),
$$

(aussi noté $g_M$) tel que $S(j_\lambda) = g \circ f_\lambda$ pour tout $\lambda \in L$, en désignant par

$$
f_\lambda : S(M_\lambda) \to \bigotimes_{\lambda \in L} S(M_\lambda)
$$

l’homomorphisme canonique.

#### Proposition 9 {#alg-iii-s6-prop-9 .statement}

*L’homomorphisme canonique* $g$ (*formule (10)*) *est un isomorphisme d’algèbres graduées* (cf. III, p. 53, *Remarque 1*).

Pour prouver que $g$ est bijectif, on va définir un homomorphisme d’algèbres

$$
h : S(M) \to \bigotimes_{\lambda \in L} S(M_\lambda)
$$

tel que $g \circ h$ et $h \circ g$ soient respectivement les applications identiques de $S(M)$ et de $\bigotimes_{\lambda \in L} S(M_\lambda)$. Pour chaque $\lambda \in L$, soit $u_\lambda$ l’application linéaire composée

$$
M_\lambda \xrightarrow{\varphi'_{M_\lambda}} S(M_\lambda) \xrightarrow{f_\lambda} \bigotimes_{\lambda \in L} S(M_\lambda).
$$

Il existe une application $A$-linéaire et une seule $u: M \to \bigotimes_{\lambda \in L} S(M_\lambda)$ telle que $u \circ j_\lambda = u_\lambda$ pour tout $\lambda \in L$. Comme les $S(M_\lambda)$ sont commutatives, il en est de même de leur produit tensoriel (III, p. 42), donc (III, p. 67, prop. 2) il existe un homomorphisme unique d’algèbres $h : S(M) \to \bigotimes_{\lambda \in L} S(M_\lambda)$, tel que $h \circ \varphi'_M = u$; d’ailleurs, il est immédiat que $u(M)$ est contenu dans le sous-module des éléments de degré 1 de l’algèbre graduée $\bigotimes_{\lambda \in L} S(M_\lambda)$, donc $h$ est un homomorphisme d’algèbres graduées. Pour $x_\lambda \in M_\lambda$, on a $h(g(u_\lambda(x_\lambda))) = h(g(f_\lambda(\varphi'_{M_\lambda}(x_\lambda)))) = h(S(j_\lambda)(\varphi'_{M_\lambda}(x_\lambda))) = h(\varphi'_M(j_\lambda(x_\lambda))) = u_\lambda(x_\lambda)$; comme les $u_\lambda(x_\lambda)$ engendrent l’algèbre $\bigotimes_{\lambda \in L} S(M_\lambda)$ (III, p. 42, prop. 8), $h \circ g$ est bien l’application identique. De même,

$$ g(h(\varphi'_M(j_\lambda(x_\lambda)))) = g(u_\lambda(x_\lambda)) = g(f_\lambda(\varphi'_{M_\lambda}(x_\lambda))) = S(j_\lambda)(\varphi'_{M_\lambda}(x_\lambda)) = \varphi'_M(j_\lambda(x_\lambda)), $$

et comme les éléments $\varphi'_M(j_\lambda(x_\lambda))$ engendrent l’algèbre $S(M)$, $g \circ h$ est bien l’application identique.

*Remarque 1).* — Soit $N = \bigoplus_{\lambda \in L} N_\lambda$ la somme directe d’une seconde famille de A-modules ayant $L$ pour ensemble d’indices, et, pour tout $\lambda \in L$, soit $v_\lambda : M_\lambda \to N_\lambda$ une application A-linéaire, d’où une application A-linéaire $v = \bigoplus_{\lambda} v_\lambda : M \to N$ (II, p. 12, prop. 6). Alors le diagramme

$$
\begin{array}{ccc}
\bigotimes_{\lambda \in L} S(M_\lambda) & \xrightarrow{g_M} & S(M) \\
\downarrow & & \downarrow S(v) \\
\bigotimes_{\lambda \in L} S(N_\lambda) & \xrightarrow{g_N} & S(N)
\end{array}
$$

est commutatif, comme il résulte des définitions (III, p. 43, corollaire).

On peut décrire de façon plus précise le sous-A-module de $\bigotimes_{\lambda \in L} S(M_\lambda)$ auquel $S^n(M)$ s’identifie au moyen de l’isomorphisme $g$. Pour toute partie finie $J$ de $L$, posons $E_J = \bigotimes_{\lambda \in J} S(M_\lambda)$, de sorte que $\bigotimes_{\lambda \in L} S(M_\lambda) = \lim_{\longrightarrow} E_J$ suivant l’ensemble filtrant $\mathcal{F}(L)$ des parties finies de $L$, par définition (III, p. 42). Pour toute famille $\nu = (n_\lambda) \in \mathbf{N}^{(L)}$ (ayant donc un support *fini*) telle que $\sum_{\lambda \in L} n_\lambda = n$, et toute partie finie $J$ de $L$ contenant le support de la famille $\nu$, posons

$$
S^{J,\nu}(M) = \bigotimes_{\lambda \in J} S^{n_\lambda}(M_\lambda)
$$

de sorte que le sous-module $E_{J,n}$ des éléments de degré $n$ de $E_J$ est la *somme directe* des $S^{J,\nu}(M)$ pour toutes les familles $\nu$ de support contenu dans $J$ et telles que $\sum_{\lambda \in L} n_\lambda = n$ (III, p. 47, prop. 10 et III, p. 53). Posons par convention $S^{J,\nu}(M) = \{0\}$ pour les familles $\nu$ dont le support n’est pas contenu dans $J$; alors on peut encore dire que $E_{J,n}$ est *somme directe* de *tous* les $S^{J,\nu}(M)$, où $\nu$ parcourt l’ensemble $H_n$ de toutes les familles $\nu = (n_\lambda)_{\lambda \in L}$ telles que $\sum_{\lambda \in L} n_\lambda = n$. Puisque $S^0(M_\lambda)$ s’identifie à $A$, il est clair en outre que pour deux parties finies $J \subset J'$ de $L$ et une famille $\nu$ de support contenu dans $J$, l’application canonique $S^{J', \nu}(M) \to S^{J', \nu}(M)$ (restriction à $S^{J', \nu}(M)$ de l’application canonique $E_J \to E_{J'}$) est bijective. Si l’on pose, pour tout $\nu \in H_n$,
$$
S^\nu(M) = \lim_{\longrightarrow} S^{J', \nu}(M)
$$
on voit donc que l’on a, compte tenu de II, p. 91, prop. 5:

#### Corollaire {#alg-iii-s6-n6-cor-1 .statement}

*Le A-module* $S^n(M)$ *est l’image par l’isomorphisme* (10) (III, p. 74) *du sous-module de* $\bigotimes_{\lambda \in L} S(M_\lambda)$ *somme directe des sous-modules* $S^\nu(M)$ *pour toutes les familles* $\nu = (n_\lambda) \in \mathbf{N}^{(L)}$ *telles que* $\sum_{\lambda \in L} n_\lambda = n$; *si* $J$ *est le support de* $\nu$, $S^\nu(M)$ *est canoniquement isomorphe à* $\bigotimes_{\lambda \in J} S^{n_\lambda}(M_\lambda)$.

On identifiera en général $S^\nu(M)$, $\bigotimes_{\lambda \in J} S^{n_\lambda}(M_\lambda)$ et leur image dans $S^n(M)$.

#### Théorème 1 {#alg-iii-s6-thm-1 .statement}

*Soient* $A$ *un anneau commutatif*, $M$ *un A-module libre ayant une base* $(e_\lambda)_{\lambda \in L}$. *Pour toute application* $\alpha : L \to N$, *de support fini*, *posons*
$$
e^\alpha = \prod_{\lambda \in L} e_{\lambda}^{\alpha(\lambda)}
$$
*(produit dans l’algèbre commutative* $S(M)$). *Alors, lorsque* $\alpha$ *parcourt l’ensemble* $\mathbf{N}^{(L)}$ *des applications de* $L$ *dans* $N$, *de support fini*, *les* $e^\alpha$ *forment une base du A-module* $S(M)$.

Comme $M$ est somme directe des $M_\lambda = Ae_\lambda$, il suffit de démontrer le théorème lorsque $L$ est réduit à un seul élément et d’appliquer ensuite III, p. 73, prop. 9. Mais lorsque $M = Ae$ (*e* élément libre), on a $x \otimes y - y \otimes x = 0$ quels que soient $x, y$ dans $M$; l’idéal $\mathfrak{J}'$ est donc nul, d’où $T(Ae) = S(Ae)$ et le théorème résulte alors de III, p. 62, th. 1.

La table de multiplication de la base (14) est donnée par
$$
e^\alpha e^\beta = e^{\alpha + \beta}
$$
où $\alpha + \beta$ est l’application $\lambda \mapsto \alpha(\lambda) + \beta(\lambda)$ de $L$ dans $N$. En d’autres termes, la base $(e^\alpha)$ de $S(M)$, munie de la loi multiplicative (15), est canoniquement isomorphe au monoïde commutatif libre $\mathbf{N}^{(L)}$ déduit de $L$; on en conclut (III, p. 25) que *l’algèbre symétrique* $S(M)$ *d’un module libre* $M$ *ayant une base dont* $L$ *est l’ensemble d’indices, est canoniquement isomorphe à l’algèbre des polynômes* $A[(X_\lambda)_{\lambda \in L}]$, *l’isomorphisme canonique s’obtenant en faisant correspondre* $X_\lambda$ *à* $e_\lambda$. En particulier (III, p. 22, prop. 7), pour toute application $f : L \to E$ de $L$ dans une A-algèbre *commutative* $E$, il existe un homomorphisme $f : S(M) \to E$ de A-algèbres et un seul tel que $f(e_\lambda) = f(\lambda)$.

Remarque 2). — Les résultats précédents peuvent également s’obtenir comme conséquence des propriétés universelles des algèbres de polynômes et des algèbres symétriques, compte tenu de (II, p. 25, cor. 3).

#### Corollaire {#alg-iii-s6-n6-cor-2 .statement}

Si $M$ est un $A$-module projectif, $S(M)$ est un $A$-module projectif.

La démonstration est la même que celle de III, p. 62, corollaire, en remplaçant $T$ par $S$.

#### Proposition 10 {#alg-iii-s6-prop-10 .statement}

Soient $\Delta$ un monoïde commutatif à élément neutre, $M$ un $A$-module gradué de type $\Delta$, $(M_{\alpha})_{\alpha \in \Delta}$ sa graduation. Pour tout couple $(\alpha, n) \in \Delta \times \mathbf{N}$, soit $S^{\alpha, n}(M)$ le sous-module de $S^n(M)$ somme directe des sous-modules $\bigotimes_{\lambda \in J} S^{n_{\lambda}}(M_{\alpha_{\lambda}})$, où $(n_{\lambda})_{\lambda \in L}$ parcourt l’ensemble des familles d’entiers $\geqslant 0$ telles que $\sum_{\lambda \in L} n_{\lambda} = n$, $J$ est son support et, pour chaque $(n_{\lambda})$, $(\alpha_{\lambda})_{\lambda \in J}$ parcourt l’ensemble des familles de $\Delta^J$ telles que $\sum_{\lambda \in J} \alpha_{\lambda} = \alpha$. Alors $(S^{\alpha, n}(M))_{(\alpha, n) \in \Delta \times \mathbf{N}}$ est la seule graduation de type $\Delta \times \mathbf{N}$ compatible avec la structure d’algèbre de $S(M)$, et qui induise sur $M = S^1(M)$ la graduation donnée.

Le fait que $S(M)$ soit somme directe des $S^{\alpha, n}(M)$ résulte du cor. de la prop. 9; le reste de la démonstration est identique à la fin de la démonstration de III, p. 62, prop. 7.

Supposons plus particulièrement que $\Delta = \mathbf{Z}$, et munissons $S(M)$ de la graduation totale (de type $\mathbf{Z}$) (II, p. 164) correspondant à la graduation de type $\mathbf{Z} \times \mathbf{N}$ (donc aussi de type $\mathbf{Z} \times \mathbf{Z}$) définie ci-dessus; les éléments homogènes de degré $n \in \mathbf{Z}$ pour cette graduation sont donc ceux de la somme directe des $S^{q, m}(M)$ pour $q + m = n$. Soit $f$ une application linéaire homogène de degré 0 du $A$-module gradué $M$ dans une $A$-algèbre graduée commutative $F$ de type $\mathbf{Z}$; alors l’homomorphisme d’algèbres $g : S(M) \to F$ tel que $f = g \circ \varphi_M'$ est un homomorphisme d’algèbres graduées de type $\mathbf{Z}$, comme il résulte de la formule $g(x_1 x_2 \ldots x_n) = f(x_1) f(x_2) \ldots f(x_n)$ pour des $x_i$ homogènes dans $M$, de l’hypothèse sur $f$, et de la définition de la graduation de type $\mathbf{Z}$ sur $S(M)$.

## EXERCICES {#alg-iii-s6-exercises}

See the [exercises for § 6](exercises/s6/).
