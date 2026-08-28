---
book: alg
book_title: Algebra
chapter: III
chapter_title: ALGÈBRES TENSORIELLES, ALGÈBRES EXTÉRIEURES, ALGÈBRES SYMÉTRIQUES
section: 11
section_title: Cogèbres, produits de formes multilinéaires, produits intérieurs et dualité
lang: fr
source: alg-i-iii-fr
book_pages: A III.138-A III.172, A III.198-A III.203
pdf_pages: 0525-0559, 0585-0590
extraction: ocr
subsections:
    - "no": 1
      title: Cogèbres
      page: 138
      pdf_page: 525
    - "no": 2
      title: Coassociativité, cocommutativité, coïunité
      page: 141
      pdf_page: 528
    - "no": 3
      title: Propriétés des cogèbres graduées de type N
      page: 147
      pdf_page: 534
    - "no": 4
      title: Bigèbres et bigèbres gauches
      page: 148
      pdf_page: 535
    - "no": 5
      title: Les duals gradués $T(M)^{*gr}$, $S(M)^{*gr}$ et $\wedge(M)^{*gr}$
      page: 150
      pdf_page: 537
    - "no": 6
      title: 'Produits intérieurs: cas des algèbres'
      page: 156
      pdf_page: 543
    - "no": 7
      title: 'Produits intérieurs: cas des cogèbres'
      page: 159
      pdf_page: 546
    - "no": 8
      title: 'Produits intérieurs : cas des bigèbres'
      page: 162
      pdf_page: 549
    - "no": 9
      title: Produits intérieurs entre $T(M)$ et $T(M^*)$, $S(M)$ et $S(M^*)$, $\wedge(M)$ et $\wedge(M^*)$
      page: 165
      pdf_page: 552
    - "no": 10
      title: Explication des produits intérieurs dans le cas d’un module libre de type fini
      page: 167
      pdf_page: 554
    - "no": 11
      title: Isomorphismes entre $\wedge^p(M)$ et $\wedge^{n-p}(M^*)$ pour un module libre $M$ de dimension $n$
      page: 168
      pdf_page: 555
    - "no": 12
      title: Application au sous-espace associé à un p-vecteur
      page: 169
      pdf_page: 556
    - "no": 13
      title: '*p*-vecteurs purs. Grassmanniennes'
      page: 170
      pdf_page: 557
statements: 52
exercises: 27
content_sha256: 2e16d6b059fe7ddf4bc94fb3442430c0dcddc9cf0b5661ae740053067d632525
---

## § 11. COGÈBRES, PRODUITS DE FORMES MULTILINÉAIRES, PRODUITS INTÉRIEURS ET DUALITÉ

Dans ce paragraphe, A est un anneau commutatif, muni de la graduation triviale. Pour un A-module gradué M de type N, nous noterons $M^{*gr}$ le A-module gradué de type N, dont les éléments homogènes de degré n sont les formes A-linéaires sur M, nulles sur $M_k$ pour tout $k \neq n$.

### 1. Cogèbres

#### Définition 1 {#alg-iii-s11-def-1 .statement}

*On appelle cogèbre sur A (ou A-cogèbre, ou simplement cogèbre si aucune confusion n’en résulte) un ensemble E muni d’une structure définie par les données suivantes:
1) une structure de A-module sur E;
2) une application A-linéaire $c : E \to E \otimes_A E$, dite coproduit de E.*

#### Définition 2 {#alg-iii-s11-def-2 .statement}

*Etant données deux cogèbres E, E', dont les coproduits sont notés respectivement c et c', on appelle morphisme de E dans E' une application A-linéaire $u : E \to E'$ telle que l’on ait*

$$(u \otimes u) \circ c = c' \circ u$$

autrement dit, rendant commutatif le diagramme d’applications A-linéaires

$$
\begin{array}{ccc}
E & \xrightarrow{u} & E' \\
c \downarrow & & \downarrow c' \\
E \otimes_A E & \xrightarrow{u \otimes u} & E' \otimes_A E'
\end{array}
$$

On vérifie immédiatement que l’application identique est un morphisme, que le composé de deux morphismes est un morphisme, et que tout morphisme bijectif est un isomorphisme.

#### Exemple 1 {#alg-iii-s11-n1-exa-1 .statement}

L’isomorphisme canonique $A \to A \otimes_A A$ (II, p. 56) définit sur $A$ une structure de $A$-cogèbre.

#### Exemple 2 {#alg-iii-s11-n1-exa-2 .statement}

Soient $E$ une cogèbre, $c$ son coproduit, $\sigma$ l’automorphisme canonique du $A$-module $E \otimes_A E$ tel que $\sigma(x \otimes y) = y \otimes x$ pour $x \in E,\ y \in E$; l’application $A$-linéaire $\sigma \circ c$ définit sur $E$ une nouvelle structure de cogèbre; muni de cette structure, $E$ est appelé la cogèbre *opposée* à la cogèbre $E$ donnée.

#### Exemple 3 {#alg-iii-s11-n1-exa-3 .statement}

Soit $B$ une *A-algèbre*, et soit $m : B \otimes_A B \to B$ l’application $A$-linéaire définissant la multiplication dans $B$ (III, p. 5). La transposée $^t m$ est donc une application $A$-linéaire du dual $B^*$ du $A$-module $B$ dans le dual $(B \otimes_A B)^*$ du $A$-module $B \otimes_A B$. Si de plus $B$ est un $A$-module *projectif de type fini*, l’application canonique $\mu : B^* \otimes_A B^* \to (B \otimes_A B)^*$ est un isomorphisme de $A$-modules (II, p. 80); l’application $c = \mu^{-1} \circ ^t m$ est alors un coproduit définissant sur le *dual* $B^*$ du $A$-module $B$ une structure de *cogèbre*.

#### Exemple 4 {#alg-iii-s11-n1-exa-4 .statement}

Soient $X$ un ensemble, $A^{(X)}$ le $A$-module des combinaisons linéaires formelles des éléments de $X$ à coefficients dans $A$ (II p. 25), $(e_x)_{x \in X}$ la base canonique de $A^{(X)}$. On définit une application $A$-linéaire $c : A^{(X)} \to A^{(X)} \otimes_A A^{(X)}$ par la condition $c(e_x) = e_x \otimes e_x$, et on obtient ainsi une structure canonique de cogèbre sur $A^{(X)}$.

#### Exemple 5 {#alg-iii-s11-n1-exa-5 .statement}

Soient $M$ un $A$-module, $T(M)$ l’algèbre tensorielle de $M$ (III, p. 56); d’après (II, p. 71) il existe une application $A$-linéaire et une seule $c$ du $A$-module $T(M)$ dans le $A$-module $T(M) \otimes_A T(M)$, telle que, pour tout $n \geq 0$,

$$
c(x_1 x_2 \ldots x_n) = \sum_{0 \leq p \leq n} (x_1 x_2 \ldots x_p) \otimes (x_{p+1} \cdots x_n)
$$

quels que soient les $x_i \in M$ ($x_1 x_2 \ldots x_n$ désigne le produit dans l’algèbre $T(M)$). On munit ainsi $T(M)$ d’une structure de *cogèbre*.

#### Exemple 6 {#alg-iii-s11-n1-exa-6 .statement}

Soient $M$ un $A$-module, $S(M)$ l’algèbre symétrique de $M$ (III, p. 67); l’application diagonale $\Delta : x \mapsto (x, x)$ de $M$ dans $M \times M$ est une application $A$-linéaire, à laquelle correspond donc canoniquement un homomorphisme $S(\Delta)$ de la $A$-algèbre $S(M)$ dans la $A$-algèbre $S(M \times M)$ (III, p. 68, prop. 3). D’autre part, on a défini dans III, p. 73, un isomorphisme canonique d’algèbres graduées, $h : S(M \times M) \to S(M) \otimes_A S(M)$; par composition on obtient donc un homomorphisme de *A-algèbres*, $c = h \circ S(\Delta) : S(M) \to S(M) \otimes_A S(M)$, définissant donc sur $S(M)$ une structure de *cogèbre*. Pour tout $x \in M$, on a par définition $S(\Delta)(x) = (x, x)$, et la définition de $h$ donnée dans III, p. 73 montre que $h((x, x)) = x \otimes 1 + 1 \otimes x$. Il en résulte que $c$ est l’unique homomorphisme d’algèbre tel que, pour tout $x \in M$, on ait

$$
c(x) = x \otimes 1 + 1 \otimes x.
$$

Comme $c$ est un homomorphisme d’algèbres, on en déduit que, pour toute suite $(x_i)_{1 \leq i \leq n}$ de $n$ éléments de $M$, on a

$$
c(x_1 x_2 \ldots x_n) = \prod_{i=1}^n (x_i \otimes 1 + 1 \otimes x_i) = \sum (x_{i_1} \ldots x_{i_p}) \otimes (x_{j_1} \ldots x_{j_{n-p}})
$$

la sommation du troisième membre de (5) étant étendue à tous les couples de suites strictement croissantes (éventuellement vides) $i_1 < i_2 < \cdots < i_p,\ j_1 < j_2 < \cdots < j_{n-p}$ d’éléments de $[1, n]$, dont les ensembles d’éléments sont complémentaires. L’élément $c(x_1 x_2 \ldots x_n)$ est un élément de *degré total* $n$ dans $S(M) \otimes_A S(M)$, et sa composante de bidegré $(p, n-p)$ est

$$
\sum_\sigma (x_{\sigma(1)} \ldots x_{\sigma(p)}) \otimes (x_{\sigma(p+1)} \ldots x_{\sigma(n)})
$$

où la sommation est étendue à toutes les permutations $\sigma \in \mathfrak{S}_n$ qui sont *croissantes* dans chacun des intervalles $[1, p]$ et $[p+1, n]$.

#### Exemple 7 {#alg-iii-s11-n1-exa-7 .statement}

Soit $M$ un $A$-module, et procédons pour l’algèbre extérieure $\wedge(M)$ de la même manière que pour $S(M)$ dans l’*Exemple* 6; l’application diagonale $\Delta : M \to M \times M$ définit cette fois un homomorphisme $\wedge(\Delta)$ de la $A$-algèbre $\wedge(M)$ dans la $A$-algèbre $\wedge(M \times M)$ (III, p. 77, prop. 2); on a d’autre part un isomorphisme canonique d’algèbres graduées

$$
h : \wedge(M \times M) \to \wedge(M)^g \otimes_A \wedge(M)
$$

(III, p. 84, prop. 10), d’où par composition un homomorphisme d’*algèbres* $c = h \circ \wedge(\Delta) : \wedge(M) \to \wedge(M)^g \otimes_A \wedge(M)$, que l’on peut considérer comme un homomorphisme de $A$-modules $\wedge(M) \to \wedge(M) \otimes_A \wedge(M)$ et qui définit donc sur $\wedge(M)$ une structure de *cogèbre*. On prouve comme dans l’*Exemple* 6 que $c$ est l’unique homomorphisme d’algèbres tel que pour tout $x \in M$, on a

$$
c(x) = x \otimes 1 + 1 \otimes x,
$$

d’où, pour toute suite $(x_i)_{1 \leq i \leq n}$ d’éléments de $M$

$$
c(x_1 \wedge x_2 \wedge \cdots \wedge x_n) = (x_1 \otimes 1 + 1 \otimes x_1) \wedge \cdots \wedge (x_n \otimes 1 + 1 \otimes x_n)
$$

où le produit du second membre est pris dans l’algèbre $\wedge(M)^g \otimes_A \wedge(M)$; pour calculer ce produit, on considère, pour tout couple de suites strictement croissantes $i_1 < i_2 < \cdots < i_p,\ j_1 < j_2 < \cdots < j_{n-p}$ d’éléments de $[1, n]$, dont les ensembles d’éléments sont complémentaires, le produit $y_1 y_2 \ldots y_n$, où $y_{i_h} = x_{i_h} \otimes 1$ ($1 \leq h \leq p$) et $y_{j_k} = 1 \otimes x_{j_k}$ ($1 \leq k \leq n-p$), et on fait la somme de tous ces produits. Comme l’algèbre graduée $\wedge(M)^g \otimes_A \wedge(M)$ est anticommutative et que les éléments $x_i \otimes 1$ et $1 \otimes x_i$ sont de degré total 1, on a, en vertu de III, p. 45, lemme 3 et de III, p. 44, lemme 1,

$$
c(x_1 \wedge x_2 \wedge \cdots \wedge x_n) = \sum (-1)^\nu (x_{i_1} \wedge \cdots \wedge x_{i_p}) \otimes (x_{j_1} \wedge \cdots \wedge x_{j_{n-p}})
$$

$\nu$ étant le nombre de couples $(h, k)$ tels que $j_k < i_h$, et la sommation étant étendue au même ensemble que dans (5) (III, p. 140). L’élément $c(x_1 \wedge \cdots \wedge x_n)$ est de degré total $n$ dans $\Lambda(M)^g \otimes_A \Lambda(M)$, et sa composante homogène de bidegré $(p, n-p)$ est égale à

$$
\sum_{\sigma} \varepsilon_{\sigma}(x_{\sigma(1)} \wedge \cdots \wedge x_{\sigma(p)}) \otimes (x_{\sigma(p+1)} \wedge \cdots \wedge x_{\sigma(n)})
$$

la sommation étant étendue aux permutations $\sigma \in S_n$ qui sont croissantes dans chacun des intervalles $[1, p]$ et $[p+1, n]$.

Quand on parlera par la suite de $A^{(\mathbf{x})}$, de $T(M)$, $S(M)$ ou $\Lambda(M)$ comme de cogèbres, il s’agira, sauf mention expresse du contraire, des structures de cogèbres définies dans les exemples 5, 6, 7 et 8 respectivement.

#### Exemple 8 {#alg-iii-s11-n1-exa-8 .statement}

Soient $E, F$ deux $A$-cogèbres, $c, c'$ leurs coproduits respectifs. Désignons par $\tau : (E \otimes_A E) \otimes_A (F \otimes_A F) \to (E \otimes_A F) \otimes_A (E \otimes_A F)$ l’isomorphisme d’associativité tel que $\tau((x \otimes x') \otimes (y \otimes y')) = (x \otimes y) \otimes (x' \otimes y')$ pour $x, x'$ dans $E$ et $y, y'$ dans $F$. Alors l’application linéaire composée

$$
E \otimes_A F \xrightarrow{c \otimes c'} (E \otimes_A E) \otimes_A (F \otimes_A F) \xrightarrow{\tau} (E \otimes_A F) \otimes_A (E \otimes_A F)
$$

définit sur le $A$-module $E \otimes_A F$ une structure de cogèbre, dite produit tensoriel des cogèbres $E$ et $F$.

Soient $E$ une cogèbre, $\Delta$ un monoïde commutatif. On dit qu’une graduation $(E_{\lambda})_{\lambda \in \Delta}$ sur le $A$-module $E$ est compatible avec le coproduit $c$ de $E$ si $c$ est un homomorphisme gradué de degré 0 du $A$-module gradué $E$ dans le $A$-module gradué (de type $\Delta$) $E \otimes_A E$, autrement dit (II, p. 173) si l’on a

$$
c(E_{\lambda}) \subset \sum_{\mu + \nu = \lambda} E_{\mu} \otimes_A E_{\nu}.
$$

Dans ce qui suit, nous nous limiterons le plus souvent aux graduations de type $\mathbf{N}$ compatibles avec le produit; une cogèbre munie d’une telle graduation sera encore appelée une cogèbre graduée. Si $F$ est une second cogèbre graduée, un morphisme de cogèbres graduées $\varphi : E \to F$ est par définition un morphisme de cogèbres (III, p. 138, déf. 2) qui est aussi un homomorphisme gradué de degré 0 de $A$-modules gradués.

#### Exemple 9 {#alg-iii-s11-n1-exa-9 .statement}

Il est immédiat que les cogèbres $T(M)$, $S(M)$, et $\Lambda(M)$ définies ci-dessus sont des cogèbres graduées.

### 2. Coassociativité, cocommutativité, coïunité

Soient $E$ une cogèbre, $c$ son coproduit, $N, N', N''$ trois $A$-modules, $m$ une application bilinéaire de $N \times N'$ dans $N''$. Notons $\tilde{m} : N \otimes_A N' \to N''$ l’application $A$-linéaire correspondant à $m$. Si $u : E \to N$, $v : E \to N'$ sont deux applications $A$-linéaires, on en déduit une application $A$-linéaire $u \otimes v : E \otimes_A E \to N \otimes_A N'$, et une application $A$-linéaire composée de $E$ dans $N''$:

$$
m(u, v) : E \xrightarrow{c} E \otimes_A E \xrightarrow{u \otimes v} N \otimes_A N' \xrightarrow{\tilde{m}} N''
$$

Il est clair que l’on a défini ainsi une application A-bilinéaire $(u, v) \mapsto m(u, v)$ de $\mathrm{Hom}_A(E, N) \times \mathrm{Hom}_A(E, N')$ dans $\mathrm{Hom}_A(E, N'')$.

Lorsque E est une cogèbre graduée, N, N', N'' des A-modules gradués de même type, $m$ un homomorphisme gradué de degré $k$ de $N \otimes_A N'$ dans $N''$, alors, si $u$ (resp. $v$) est un homomorphisme gradué de degré $p$ (resp. $q$), $m(u, v)$ est un homomorphisme gradué de degré $p + q + k$.

#### Exemple 1 {#alg-iii-s11-n2-exa-1 .statement}

Prenons pour E la cogèbre graduée $T(M)$ (III, p. 139), et supposons N, N', N'' munis de la graduation triviale. Un homomorphisme gradué de degré $-p$ de $T(M)$ dans N (resp. N', N'') correspond alors à une application multilinéaire de $M^p$ dans N (resp. N', N''). Etant donnée une application multilinéaire $u : M^p \to N$ et une application multilinéaire $v : M^q \to N'$, la méthode précédente permet d’en déduire une application multilinéaire $m(u, v) : M^{p+q} \to N''$, appelé *produit* (relativement à $m$) de $u$ et $v$. Les formules (3) (III, p. 139) et (11) (III, p. 141) montrent que l’on a, pour $x_1, \ldots, x_{p+q}$ dans M
$$
(m(u, v))(x_1, \ldots, x_{p+q}) = m(u(x_1, \ldots, x_p), v(x_{p+1}, \ldots, x_{p+q})).
$$

#### Exemple 2 {#alg-iii-s11-n2-exa-2 .statement}

Prenons pour E la cogèbre graduée $S(M)$ (III, p. 139), en conservant les mêmes hypothèses sur N, N', N''. Un homomorphisme gradué de degré $-p$ de $S(M)$ dans N correspond alors à une *application multilinéaire symétrique* de $M^p$ dans N (III, p. 70). On déduit donc d’une application multilinéaire symétrique $u : M^p \to N$ et d’une application multilinéaire symétrique $v : M^q \to N'$ une application multilinéaire symétrique $m(u, v) : M^{p+q} \to N''$, que l’on note encore (pour éviter des confusions) $u \cdot_m v$ (ou même $u.v$) et qu’on appelle *produit symétrique* (relativement à $m$) de $u$ et $v$. Les formules (6) (III, p. 140) et (11) (III, p. 141) montrent que l’on a, pour $x_1, \ldots, x_{p+q}$ dans M
$$
(u \cdot_m v)(x_1, \ldots, x_{p+q}) = \sum_\sigma m(u(x_{\sigma(1)}, \ldots, x_{\sigma(p)}), v(x_{\sigma(p+1)}, \ldots, x_{\sigma(p+q)}))
$$
la sommation étant étendue aux permutations $\sigma \in S_{p+q}$ croissantes dans chacun des intervalles $[1, p]$ et $[p+1, p+q]$.

#### Exemple 3 {#alg-iii-s11-n2-exa-3 .statement}

Prenons pour E la cogèbre graduée $\wedge(M)$ (III, p. 140). On déduit alors de la même manière, d’une application multilinéaire alternée $u : M^p \to N$ et d’une application multilinéaire alternée $v : M^q \to N'$, une application multilinéaire alternée $m(u, v) : M^{p+q} \to N''$, que l’on note encore $u \wedge_m v$ ou $u \wedge v$ et que l’on appelle *produit alterné* (relativement à $m$) de $u$ et $v$. Les formules (9) et (11) (III, p. 141) montrent ici que, pour $x_1, \ldots, x_{p+q}$ dans M, on a
$$
(u \wedge_m v)(x_1, \ldots, x_{p+q}) = \sum_\sigma \varepsilon_\sigma m(u(x_{\sigma(1)}, \ldots, x_{\sigma(p)}), v(x_{\sigma(p+1)}, \ldots, x_{\sigma(p+q)}))
$$
la sommation étant encore étendue aux permutations $\sigma \in S_{p+q}$ croissantes dans chacun des intervalles $[1, p]$ et $[p+1, p+q]$.

Revenons au cas où E est une cogèbre graduée quelconque (de type $\mathbf{N}$), et supposons que les trois modules N, N', N'' soient tous égaux au A-module sous-jacent à une A-algèbre graduée B de type $\mathbf{Z}$, l’application m étant le produit dans B, de sorte que $\tilde{m}: B \otimes_A B \to B$ est une application A-linéaire graduée de degré 0. On obtient donc sur le A-module gradué $\mathrm{Homgr}_A(E, B) = C$ une structure de A-algèbre graduée.

En particulier, on peut prendre $B = A$ (avec la graduation triviale), de sorte que $\mathrm{Homgr}_A(E, A)$ est le dual gradué $E^{*\mathrm{gr}}$, qui est ainsi muni d’une structure de A-algèbre graduée.

Soient F une seconde cogèbre graduée, $c'$ son coproduit, $\varphi : E \to F$ un morphisme de cogèbres graduées (III, p. 141); alors le morphisme gradué canonique $\tilde{\varphi} = \mathrm{Hom}(\varphi, 1_B) : \mathrm{Homgr}_A(F, B) \to \mathrm{Homgr}_A(E, B)$ est un homomorphisme d’algèbres graduées. En effet, pour $u, v$ dans $\mathrm{Homgr}_A(F, B)$ et $x \in E$, on a $(\tilde{\varphi}(uv))(x) = (uv)(\varphi(x)) = m((u \otimes v)(c'(\varphi(x))))$. Mais par hypothèse $c'(\varphi(x)) = (\varphi \otimes \varphi)(c(x))$ donc $(u \otimes v)(c'(\varphi(x))) = (\tilde{\varphi}(u) \otimes \tilde{\varphi}(v))(c(x))$, et par suite $\tilde{\varphi}(uv) = \tilde{\varphi}(u)\tilde{\varphi}(v)$, ce qui prouve notre assertion.

En particulier, le transposé gradué $^t\varphi : F^{*\mathrm{gr}} \to E^{*\mathrm{gr}}$ est un homomorphisme d’algèbres graduées.

#### Remarque {#alg-iii-s11-n2-rem-1 .statement}

Supposons que les $E_p$ soient des A-modules projectifs de type fini, de sorte que l’on peut identifier canoniquement les A-modules gradués $(E \otimes_A E)^{*\mathrm{gr}}$ et $E^{*\mathrm{gr}} \otimes_A E^{*\mathrm{gr}}$ (II, p. 80, cor. 1). Si de plus on identifie alors canoniquement les A-modules $A \otimes_A A$ et $A$ (II, p. 55), on peut dire que l’application linéaire $E^{*\mathrm{gr}} \otimes_A E^{*\mathrm{gr}} \to E^{*\mathrm{gr}}$ qui définit la multiplication dans $E^{*\mathrm{gr}}$ est la transposée graduée du coproduit $c$.

#### Proposition 1 {#alg-iii-s11-prop-1 .statement}

Soit E une cogèbre sur A. Afin que, pour toute A-algèbre associative B, la A-algèbre $\mathrm{Hom}_A(E, B)$ soit associative, il faut et il suffit que le coproduit $c : E \to E \otimes_A E$ soit tel que le diagramme

$$
\begin{array}{ccc}
E & \xrightarrow{c} & E \otimes_A E \\
\downarrow^c & & \downarrow^{1_E \otimes c} \\
E \otimes_A E & \xrightarrow{c \otimes 1_E} & E \otimes_A E \otimes_A E
\end{array}
$$

soit commutatif.

Soient B une A-algèbre associative, et $u, v, w$ trois éléments de $C = \mathrm{Hom}_A(E, B)$. Notons $m_3$ l’application A-linéaire $B \otimes_A B \otimes_A B \to B$ qui, à $b \otimes b' \otimes b''$, fait correspondre $bb'b''$. Par définition du produit dans l’algèbre C, $(uv)w$ est l’application composée

$$
E \xrightarrow{c} E \otimes E \xrightarrow{c \otimes 1_E} E \otimes E \otimes E \xrightarrow{u \otimes v \otimes w} B \otimes B \otimes B \xrightarrow{m_3} B
$$

tandis que $u(vw)$ est l’application composée

$$
E \xrightarrow{c} E \otimes E \xrightarrow{1_E \otimes c} E \otimes E \otimes E \xrightarrow{u \otimes v \otimes w} B \otimes B \otimes B \xrightarrow{m_3} B.
$$

Il en résulte que si le diagramme (12) est commutatif, l’algèbre $\mathrm{Hom}_A(E, B)$ est associative pour toute A-algèbre associative B. Pour établir la réciproque, il suffit de montrer qu’il existe une A-algèbre associative B et trois applications A-linéaires $u, v, w$ de E dans B telles que l’application $m_3 \circ (u \otimes v \otimes w)$ de $E \otimes E \otimes E$ dans B soit injective. Prenons pour B la A-algèbre $\mathcal{T}(E)$ et pour $u, v, w$ l’application canonique de E dans $\mathcal{T}(E)$. L’application $m_3 \circ (u \otimes v \otimes w)$ est alors l’application canonique $E \otimes E \otimes E = \mathcal{T}^3(E) \to \mathcal{T}(E)$ qui est injective.

Lorsque la cogèbre E vérifie la condition de la prop. 1, on dit qu’elle est coassociative.

#### Exemple 4 {#alg-iii-s11-n2-exa-4 .statement}

On vérifie aussitôt que la cogèbre A (III, p. 139, Exemple 1), la cogèbre $A^{(x)}$ (III, p. 139, Exemple 4) et la cogèbre $\mathcal{T}(M)$ (III, p. 139, Exemple 5) sont coassociatives. Si B est une A-algèbre associative qui est un A-module projectif de type fini, la cogèbre $B^*$ (III, p. 139, Exemple 3) est coassociative : en effet, la commutativité du diagramme (12) de III, p. 143, se déduit alors par transposition de celle du diagramme qui exprime l’associativité de B (III, p. 5). Réciproquement, le même raisonnement et l’identification canonique du A-module B avec son bidual (II, p. 47, cor. 4) montrent que si la cogèbre $B^*$ est coassociative, l’algèbre B est associative. Enfin, les cogèbres $S(M)$ et $\Lambda(M)$ (III, p. 139, Exemple 6 et p. 140, Exemple 7) sont coassociatives ; cela résulte de la commutativité du diagramme

$$
\begin{array}{ccc}
M & \xrightarrow{\Delta} & M \times M \\
\Delta \downarrow & & \downarrow 1_M \times \Delta \\
M \times M & \xrightarrow{\Delta \times 1_M} & M \times M \times M
\end{array}
$$

des propriétés fonctorielles de $S(M)$ (III, p. 69) et $\Lambda(M)$ (III, p. 78), qui donnent les diagrammes commutatifs correspondants

$$
\begin{array}{ccc}
S(M) & \xrightarrow{S(\Delta)} & S(M \times M) \\
S(\Delta) \downarrow & & \downarrow S(1_M \times \Delta) \\
S(M \times M) & \xrightarrow{S(\Delta \times 1_M)} & S(M \times M \times M)
\end{array}
$$
$$
\begin{array}{ccc}
\Lambda(M) & \xrightarrow{\Lambda(\Delta)} & \Lambda(M \times M) \\
\Lambda(\Delta) \downarrow & & \downarrow \Lambda(1_M \times \Delta) \\
\Lambda(M \times M) & \xrightarrow{\Lambda(\Delta \times 1_M)} & \Lambda(M \times M \times M)
\end{array}
$$

et de l’existence et de la fonctorialité des isomorphismes canoniques pour les algèbres symétrique et extérieure d’une somme directe (III, p. 73 et III, p. 84).

#### Proposition 2 {#alg-iii-s11-prop-2 .statement}

Soit E une cogèbre sur A. Afin que, pour toute A-algèbre commutative B, la A-algèbre $\mathrm{Hom}_A(E, B)$ soit commutative, il faut et il suffit que le coproduit $c : E \to E \otimes_A E$ soit tel que le diagramme

$$
\begin{array}{ccc}
E & & \\
/ & & \searrow \\
E \otimes_A E & \xrightarrow{\sigma} & E \otimes_A E
\end{array}
$$

(où $\sigma$ est l’homomorphisme de symétrie, tel que $\sigma(x \otimes y) = y \otimes x$) soit commutatif (autrement dit, il faut et il suffit que la cogèbre $E$ soit identique à son opposée (III, p. 139, Exemple 2).

Soient $B$ une $A$-algèbre commutative, et $u, v$ deux éléments de $C = \mathrm{Hom}_A(E, B)$. Par définition du produit dans $C$, $uv$ et $vu$ sont respectivement égaux aux applications composées

$$
E \xrightarrow{c} E \otimes E \xrightarrow{u \otimes v} B \otimes B \xrightarrow{m} B
$$

et

$$
E \xrightarrow{c} E \otimes E \xrightarrow{v \otimes u} B \otimes B \xrightarrow{m} B.
$$

Il en résulte que si le diagramme (15) est commutatif, l’algèbre $\mathrm{Hom}_A(E, B)$ est commutative pour toute $A$-algèbre commutative $B$. Pour établir la réciproque, il suffit de montrer qu’il existe une $A$-algèbre commutative $B$ et deux applications $A$-linéaires $u, v$ de $E$ dans $B$ telles que $m \circ (u \otimes v) : E \otimes E \to B$ soit injective. Prenons pour $B$ l’algèbre $S(E \oplus E)$ et pour $u$ (resp. $v$) le composé de l’application canonique $E \oplus E \to S(E \oplus E)$ et de l’application $x \mapsto (x, 0)$ (resp. $x \mapsto (0, x)$) de $E$ dans $E \oplus E$. Si $h : S(E) \otimes S(E) \to S(E \oplus E)$ est l’isomorphisme canonique (III, p. 73, prop. 9) et si $\lambda : E \to S(E)$ est l’application canonique, on a $h^{-1} \circ m \circ (u \otimes v) = \lambda \otimes \lambda$. Or $\lambda \otimes \lambda$ est injectif, car $\lambda(E)$ est un facteur direct de $S(E)$ (II, p. 63, cor. 5).

Lorsque la cogèbre $E$ vérifie la condition de la prop. 2, on dit qu’elle est cocommutative.

#### Exemple 5 {#alg-iii-s11-n2-exa-5 .statement}

Il est immédiat que la cogèbre $A$ (III, p. 139, Exemple 1) et la cogèbre $A^{(x)}$ (III, p. 139, Exemple 4) sont cocommutatives. Il résulte de la formule (5) de III, p. 140, que la cogèbre $S(M)$ est cocommutative. Enfin, pour qu’une $A$-algèbre $B$, telle que le $A$-module $B$ soit projectif de type fini, ait la propriété que la cogèbre $B^*$ (III, p. 139, Exemple 3) soit cocommutative, il faut et il suffit que $B$ soit commutative; en effet (compte tenu de l’identification canonique du $A$-module $B$ et de son bidual (II, p. 47)), cela résulte de ce que la commutativité du diagramme (15) de III, p. 144, équivaut par transposition à celle du diagramme qui exprime la commutativité de $B$ (III, p. 5).

#### Proposition 3 {#alg-iii-s11-prop-3 .statement}

Soit $E$ une cogèbre sur $A$. Afin que, pour toute $A$-algèbre unifière $B$, la $A$-algèbre $\mathrm{Hom}_A(E, B)$ soit unifière, il faut et il suffit qu’il existe une forme linéaire $\gamma$ sur $E$ rendant commutatifs les diagrammes

$$
\begin{array}{ccc}
E & \xrightarrow{c} & E \otimes_A E \\
 & & \downarrow \gamma \otimes 1_E \\
 & & A \otimes_A E
\end{array}
$$
$$
\begin{array}{ccc}
E & \xrightarrow{c} & E \otimes_A E \\
 & & \downarrow 1_E \otimes \gamma \\
 & & E \otimes_A A
\end{array}
$$

où $c : E \to E \otimes_A E$ est le coproduit, $h'$ et $h''$ les isomorphismes canoniques (II, p. 55, prop. 4). L’unité de $\mathrm{Hom}_A(E, B)$ est alors l’application linéaire $x \mapsto \gamma(x)1$ (1 désignant l’élément unité de B).

Soit $\gamma$ une forme linéaire sur E qui rend commutatif le diagramme (16). Soient B une A-algèbre unifère d’élément unité 1, $\eta : A \to B$ l’application canonique, $v = \eta \circ \gamma$ l’élément de la A-algèbre $C = \mathrm{Hom}_A(E, B)$. Pour tout élément $u \in C$, $uv$ est l’application composée

$$
\text{(17)} \quad E \xrightarrow{c} E \otimes E \xrightarrow{1_E \otimes \gamma} E \otimes A \xrightarrow{u \otimes \eta} B \otimes B \xrightarrow{m} B.
$$

On a donc $uv = m \circ (u \otimes \eta) \circ h'' = u$. On prouve de même que l’on a $vu = u$, donc $v$ est élément unité de C. Inversement, munissons le A-module $A \oplus E$ de la structure d’algèbre unifère telle que $(a, x)(a', x') = (aa', ax' + a'x)$ pour $a, a'$ dans A et $x, x'$ dans E. Notons B la A-algèbre ainsi obtenue et soit C la A-algèbre $\mathrm{Hom}_A(E, B)$. Supposons C unifère et soit $e : x \mapsto (\gamma(x), \lambda(x))$ son élément unité (où $\gamma(x) \in A$ et $\lambda(x) \in E$). Soit d’autre part $f$ l’élément $x \mapsto (0, x)$ de C. Un calcul immédiat montre que $fe$ est l’élément

$$
x \mapsto (0, (h'')^{-1}((1_E \otimes \gamma)(c(x))))
$$

de C. La condition $fe = f$ entraîne la commutativité du second diagramme (16), et on voit de même que la condition $ef = f$ entraîne la commutativité du premier diagramme (16).

Une forme linéaire $\gamma$ sur E rendant commutatifs les diagrammes (16) de III, p. 145, est appelée une coïunité de la cogèbre E. Une cogèbre admet au plus une coïunité : en effet, c’est l’élément unité de l’algèbre $\mathrm{Hom}_A(E, A)$. Une cogèbre ayant une coïunité est dite coïunifère.

#### Exemple 6 {#alg-iii-s11-n2-exa-6 .statement}

L’application identique est la coïunité de la cogèbre A ; sur la cogèbre $A^{(X)}$ (III, p. 139, Exemple 4), la forme linéaire $\gamma$ telle que $\gamma(e_x) = 1$ pour tout $x \in X$ est la coïunité. Sur la cogèbre $T(M)$ (resp. $S(M)$, $\wedge(M)$) la forme linéaire $\gamma$ telle que $\gamma(1) = 1$ et $\gamma(z) = 0$ pour $z$ dans les $T^n(M)$ (resp. $S^n(M)$, $\wedge^n(M)$) pour $n \geqslant 1$, est la coïunité. Enfin, soit B une A-algèbre qui soit un A-module projectif de type fini, et qui possède un élément unité $e$; alors sur la cogèbre $B^*$ (III, p. 139, Exemple 3), la forme linéaire $\gamma : x^* \mapsto \langle e, x^* \rangle$ est la coïunité, car cette forme n’est autre que la transposée de l’application A-linéaire $\eta_e : \xi \mapsto \xi e$ de A dans B, et, par transposition, la commutativité des diagrammes (16) de III, p. 145, se déduit de celle des diagrammes qui expriment (à l’aide de $\eta_e$) que $e$ est élément unité de B (III, p. 6); le même raisonnement montre d’ailleurs qu’inversement, si la cogèbre $B^*$ admet une coïunité $\gamma$, la transposée de $\gamma$ définit un élément unité $e = {}^t\gamma(1)$ de B.

#### Proposition 4 {#alg-iii-s11-prop-4 .statement}

Soit E une cogèbre admettant une coïunité $\gamma$, et supposons qu’il existe dans $E$ un élément $e$ tel que $\gamma(e) = 1$; alors $E$ est somme directe des sous-A-modules $Ae$ et $E_\gamma = \mathrm{Ker}(\gamma)$, et l’on a

$$
(18) \quad \left\{ \begin{array}{l}
c(e) \equiv e \otimes e \ (\text{mod. } E_\gamma \otimes E_\gamma) \\
c(x) \equiv x \otimes e + e \otimes x \ (\text{mod. } E_\gamma \otimes E_\gamma) \text{ pour tout } x \in E_\gamma.
\end{array} \right.
$$

La première assertion est immédiate, car on a $\gamma(x - \gamma(x)e) = 0$ et la relation $\gamma(\alpha e) = 0$ entraîne $\alpha = 0$. Posons $c(e) = \sum_i s_i \otimes t_i$, de sorte que $e = \sum_i \gamma(s_i)t_i = \sum_i \gamma(t_i)s_i$ en vertu de (16) et que $1 = \gamma(e) = \sum_i \gamma(s_i)\gamma(t_i)$. On a par suite

$$
\sum_i (s_i - \gamma(s_i)e) \otimes (t_i - \gamma(t_i)e) = \sum_i s_i \otimes t_i - \sum_i e \otimes \gamma(s_i)t_i \\
\phantom{\sum_i (s_i - \gamma(s_i)e) \otimes (t_i - \gamma(t_i)e)} - \sum_i \gamma(t_i)s_i \otimes e + \sum_i \gamma(s_i)e \otimes \gamma(t_i)e
$$

élément qui, en vertu des relations antérieures, n’est autre que $c(e) - e \otimes e$; cela prouve par suite la première relation (18). D’autre part, la décomposition de $E \otimes E$ en somme directe

$$
A(e \otimes e) \oplus ((Ae) \otimes E_\gamma) \oplus (E_\gamma \otimes (Ae)) \oplus (E_\gamma \otimes E_\gamma)
$$

permet d’écrire, pour $x \in E_\gamma$, $c(x) = \lambda(e \otimes e) + (e \otimes y) + (z \otimes e) + u$ avec $u = \sum_j v_j \otimes w_j, y, z$ et les $v_j$ et $w_j$ appartenant à $E_\gamma$. La définition de la coïunité $\gamma$ donne alors $x = \lambda e + y = \lambda e + z$, et comme $\gamma(x) = 0$, on a nécessairement $\lambda = 0, x = y = z$, d’où la seconde relation (18).

#### Remarque {#alg-iii-s11-n2-rem-2 .statement}

Soient C une A-cogèbre coassociative et coünifère, B une A-algèbre associative unifère et M un B-module à gauche. L’application A-bilinéaire $(b, m) \mapsto bm$ de $B \times M$ dans $M$ définit une application A-bilinéaire

$$
\mathrm{Hom}_A(C, B) \times \mathrm{Hom}_A(C, M) \to \mathrm{Hom}_A(C, M)
$$

par le procédé général décrit au début de ce n°. On vérifie aussitôt que cette application définit sur $\mathrm{Hom}_A(C, M)$ une structure de module à gauche sur l’anneau $\mathrm{Hom}_A(C, B)$.

### 3. Propriétés des cogèbres graduées de type N

#### Proposition 5 {#alg-iii-s11-prop-5 .statement}

(i) Soit $E$ une cogèbre graduée admettant une coïunité $\gamma$; alors $\gamma$ est une forme linéaire homogène de degré 0.

(ii) Supposons de plus qu’il existe un élément $e \in E$ tel que $E_0 = Ae$ et $\gamma(e) = 1$. Alors le noyau $E_\gamma$ de $\gamma$ est égal à $E_+ = \sum_{n \geq 1} E_n$, on a $c(e) = e \otimes e$, et

$$
(19) \quad c(x) \equiv x \otimes e + e \otimes x \ (\text{mod. } E_+ \otimes E_+),
$$

pour tout $x \in E_+$.

(i) Il suffit de voir que $\gamma(x) = 0$ pour $x \in E_n$, pour tout $n \geq 1$. Puisque $c$ est un homomorphisme gradué de degré 0, on a
$$
c(x) = \sum_{0 \leq j \leq n} \left( \sum_i y_{ij} \otimes z_{i, n-j} \right)
$$
avec, pour tout $j$ tel que $0 \leq j \leq n$, $y_{ij}$ et $z_{ij}$ dans $E_j$; appliquant (16) (III, p. 145), il vient $x = \sum_{0 \leq j \leq n} \left( \sum_i \gamma(y_{ij}) z_{i, n-j} \right) = \sum_{0 \leq j \leq n} \left( \sum_i \gamma(z_{i, n-j}) y_{ij} \right)$, d’où, en égalant aux deux membres les composantes de degré 0 et de degré $n$
$$
x = \sum_i \gamma(y_{i0}) z_{in} = \sum_i \gamma(z_{i0}) y_{in}
$$
$$
0 = \sum_i \gamma(y_{in}) z_{i0} = \sum_i \gamma(z_{in}) y_{i0}
$$
et par suite $\gamma(x) = \sum_i \gamma(y_{in}) \gamma(z_{i0}) = \gamma(0) = 0$.

(ii) Puisque $\mathrm{Ker}(\gamma)$ et $E_+$ sont tous deux des sous-A-modules supplémentaires de $Ae = E_0$ et que $E_+ \subset \mathrm{Ker}(\gamma)$ par (i), on a $E_+ = \mathrm{Ker}(\gamma)$ (II, p. 18, Remarque 1); les autres assertions découlent de la prop. 4 de III, p. 146.

#### Proposition 6 {#alg-iii-s11-prop-6 .statement}

Soit $E$ une cogèbre graduée sur $A$. Afin que, pour toute $A$-algèbre commutative $B$, munie de la graduation triviale, la $A$-algèbre graduée de type $\mathbf{Z}$, $\mathrm{Homgr}_A(E, B)$ (III, p. 143) soit anticommutative (III, p. 53, déf. 7), il faut et il suffit que, si $\sigma_g$ désigne l’automorphisme du $A$-module $E \otimes_A E$ tel que $\sigma_g(x_p \otimes x_q) = (-1)^{pq} x_q \otimes x_p$ pour $x_p \in E_p, x_q \in E_q, p$ et $q$ quelconques dans $\mathbf{N}$, le diagramme
$$
\begin{array}{ccc}
E & & \\
& c & \\
E \otimes_A E & \xrightarrow{\sigma_g} & E \otimes_A E
\end{array}
$$
soit commutatif.

La démonstration est analogue à celle de la prop. 2 de III, p. 144.

Lorsque la cogèbre graduée $E$ vérifie la condition de la prop. 6, on dit qu’elle est anticommutative.

#### Exemple {#alg-iii-s11-n3-exa-1 .statement}

Il résulte aussitôt de la formule (8) de III, p. 140 que pour tout $A$-module $M$, la cogèbre graduée $\wedge(M)$ est anticommutative.

### 4. Bigèbres et bigèbres gauches

#### Définition 3 {#alg-iii-s11-def-3 .statement}

On appelle bigèbre graduée (resp. bigèbre graduée gauche) sur un anneau $A$ un ensemble $E$ muni d’une structure de $A$-algèbre graduée de type $\mathbf{N}$ et d’une structure de

A-cogèbre graduée de type $\mathbf{N}$, ayant même structure de $A$-module gradué sous-jacentes et telles que :

$1^\circ$ La $A$-algèbre $E$ est associative et unifère.
$2^\circ$ La $A$-cogèbre $E$ est coassociative et coünifère.
$3^\circ$ Le coproduit $c : E \to E \otimes_A E$ est un homomorphisme de l’algèbre graduée $E$ dans l’algèbre graduée $E \otimes_A E$ (resp. l’algèbre graduée $E^g \otimes_A E$ (cf. III, p. 49).
$4^\circ$ La coünité $\gamma$ de $E$ est un homomorphisme de l’algèbre graduée $E$ dans l’algèbre $A$ (munie de la graduation triviale) telle que si $e$ désigne l’élément unité de la $A$-algèbre $E$, $\gamma(e) = 1$.

Si $E$ est une bigèbre graduée dont la graduation est *triviale*, on dit simplement que $E$ est une *bigèbre*. On dit qu’une bigèbre graduée est commutative (resp. cocommutative) si l’algèbre sous-jacente est commutative (resp. si la cogèbre sous-jacente est cocommutative); on dit qu’une bigèbre graduée gauche est anticommutative (resp. anticocommutative) si l’algèbre graduée sous-jacente est anticommutative (resp. si la cogèbre graduée sous-jacente est anticocommutative).

Il résulte de la déf. 3, et de III, p. 147, prop. 5, que pour une bigèbre graduée ou une bigèbre graduée gauche $E$, on a

$$
(22)\quad \left\{\begin{array}{l}
c(e) = e \otimes e \\
c(x) \equiv x \otimes e + e \otimes x \pmod{E_+ \otimes E_+} \quad \text{pour } x \in E_+ = \bigoplus_{n \geq 1} E_n.
\end{array}\right.
$$

Si $E$ et $F$ sont deux bigèbres graduées (resp. deux bigèbres graduées gauches), on dit qu’une application $\varphi : E \to F$ est un *morphisme de bigèbres graduées* (resp. un *morphisme de bigèbres graduées gauches*) si : $1^\circ$ $\varphi$ est un morphisme d’algèbres graduées (transformant donc l’élément unité de $E$ en l’élément unité de $F$); $2^\circ$ $\varphi$ est un morphisme de cogèbres graduées tel que, si $\gamma$ et $\gamma'$ sont les coünités respectives de $E$ et $F$ on ait $\gamma = \gamma' \circ \varphi$.

#### Exemple 1 {#alg-iii-s11-n4-exa-1 .statement}

Soit $S$ un monoïde d’élément neutre $u$, de sorte que l’algèbre $E = A^{(S)}$ du monoïde $S$ sur $A$ admet l’élément unité $e_u$ (III, p. 19); on a vu d’autre part que $E$ est muni canoniquement d’une structure de $A$-cogèbre coassociative, cocommutative et ayant une coünité $\gamma$ telle que $\gamma(e_s) = 1$ pour tout $s \in S$ (III, p. 139, *Exemple 4* et III, p. 144, *Exemple 4*, p. 145, *Exemple 5* et p. 146, *Exemple 6*). La formule $c(e_s) = e_s \otimes e_s$ donnant le coproduit montre en outre aussitôt que $c$ est un homomorphisme d’algèbres. On a donc défini sur $E$ une structure de *bigèbre cocommutative* et $E$, muni de cette structure, est appelé la *bigèbre du monoïde $S$ sur $A$*.

Si $T$ est un second monoïde ayant un élément neutre $v$, $f : S \to T$ un homomorphisme tel que $f(u) = v$, $f_{(A)} : A^{(S)} \to A^{(T)}$ l’homomorphisme de $A$-algèbres déduit de $f$ (III, p. 20), on vérifie aussitôt que $f_{(A)}$ est un *homomorphisme de bigèbres*.

#### Exemple 2 {#alg-iii-s11-n4-exa-2 .statement}

Soit $M$ un $A$-module. Les structures de $A$-algèbre graduée (III, p. 67) et de $A$-cogèbre graduée (III, p. 139, *Exemple 6*) définies sur $S(M)$ définissent sur cet ensemble une structure de *bigèbre graduée commutative et cocommutative*; on a vu en effet (III, p. 139, *Exemple 6*) que le coproduit de $S(M)$ est un homomorphisme d’*algèbres*, et il résulte de la définition de la counité $\gamma$ (III, p. 146, *Exemple 6*) que $\gamma(1) = 1$ et que $\gamma$ est un homomorphisme d’algèbres de $E$ dans $A$.

#### Exemple 3 {#alg-iii-s11-n4-exa-3 .statement}

Soit $M$ un $A$-module. On voit comme dans l’*Exemple 2*) que sur $\wedge(M)$ les structures de $A$-algèbre graduée (III, p. 76) et de $A$-cogèbre graduée (III, p. 140, *Exemple 7*) définissent sur cet ensemble une structure de *bigèbre graduée gauche anticommutative et anticocommutative*.

#### Remarque {#alg-iii-s11-n4-rem-1 .statement}

Si $M$ est un $A$-module tel que $M \otimes_A M \neq \{0\}$, les structures de $A$-algèbre graduée (III, p. 56) et de $A$-cogèbre graduée (III, p. 139, *Exemple 5*) sur $T(M)$ *ne définissent pas* une structure de bigèbre, car en général on a
$$
c(x_1 x_2 y_1 y_2) \neq c(x_1 x_2) c(y_1 y_2)
$$
pour quatre éléments $x_1, x_2, y_1, y_2$ de $M$, comme le montre la formule (3) de III, p. 139.

### 5. Les duals gradués $T(M)^{*gr}$, $S(M)^{*gr}$ et $\wedge(M)^{*gr}$

Nous reprenons à partir de maintenant les conventions générales du chapitre sur les algèbres, qui seront donc supposées (*sauf mention expresse du contraire*) *associatives et unifères*.

Soit $M$ un $A$-module; les structures de $A$-cogèbre graduée définies sur $T(M)$ (III, p. 139, *Exemple 5*), $S(M)$ (III, p. 139, *Exemple 6*) et $\wedge(M)$ (III, p. 140, *Exemple 7*) permettent de définir canoniquement sur les duals gradués $T(M)^{*gr}$, $S(M)^{*gr}$ et $\wedge(M)^{*gr}$ des structures d’*algèbre graduée* de type $N$, en vertu de III, p. 143, prop. 1, p. 145, prop. 3 et p. 143, et de la convention faite sur la graduation du dual graduée d’un module gradué (III, p. 138). En outre, l’algèbre graduée $S(M)^{*gr}$ est *commutative* (III, p. 144, prop. 2 et p. 145, *Exemple 5*) et l’algèbre graduée $\wedge(M)^{*gr}$ est *anticommutative* (III, p. 148, prop. 6 et p. 148, *Exemple*). Dans $\wedge(M)^{*gr}$, *tout élément de degré 1 est de carré nul*; un tel élément s’identifie en effet à une forme linéaire $f$ sur $M$, et son carré à la forme bilinéaire alternée $f \wedge f$ sur $M^2$ telle que $(f \wedge f)(x, y) = f(x)f(y) - f(y)f(x)$ (III, p. 142, *Exemple 3*).

Soient $N$ un second $A$-module, $u$ une application $A$-linéaire de $M$ dans $N$. On sait que $u$ définit canoniquement des homomorphismes d’algèbres graduées
$$
\begin{cases}
T(u): T(M) \to T(N) \\
S(u): S(M) \to S(N) \\
\wedge(u): \wedge(M) \to \wedge(N)
\end{cases}
$$
(III, p. 57, III, p. 69, et III, p. 78). On vérifie aussitôt sur la formule (3) de III, p. 139 que $T(u)$ est aussi un *morphisme de cogèbres*. D’autre part, si $\Delta_M$ (resp. $\Delta_N$) désigne l’application diagonale $M \to M \times M$ (resp. $N \to N \times N$), on a la relation $(u \times u) \circ \Delta_M = \Delta_N \circ u$; on en déduit que $S(u \times u) \circ S(\Delta_M) = S(\Delta_N) \circ S(u)$ (resp. $\wedge (u \times u) \circ \wedge (\Delta_M) = \wedge (\Delta_N) \circ \wedge (u)$). Tenant compte de la définition du coproduit dans $S(M)$ et $\wedge (M)$ (III, p. 139, Exemple 6 et p. 140, Exemple 7) et du caractère fonctoriel des isomorphismes canoniques
$$
S(M \times M) \to S(M) \otimes_A S(M)
$$
et $\wedge (M \times M) \to \wedge (M)^{\mathrm{gr}} \otimes_A \wedge (M)$, on voit que $S(u)$ et $\wedge (u)$ sont aussi des morphismes de cogèbres¹ (donc ici des morphismes de bigèbres). Il en résulte aussitôt que les transposés gradués (II, p. 176) des homomorphismes (23) de III, p. 150
$$
\begin{align*}
tT(u) &: T(N)^{\mathrm{gr}} \to T(M)^{\mathrm{gr}} \\
tS(u) &: S(N)^{\mathrm{gr}} \to S(M)^{\mathrm{gr}} \\
t\wedge (u) &: \wedge (N)^{\mathrm{gr}} \to \wedge (M)^{\mathrm{gr}}
\end{align*}
$$
sont des homomorphismes d’algèbres graduées.

Remarquons maintenant que le dual $M^*$ de $M$ s’identifie au sous-module des éléments de degré 1 de $T(M)^{\mathrm{gr}}$ (resp. $S(M)^{\mathrm{gr}}, \wedge (M)^{\mathrm{gr}}$). Il résulte donc de la propriété universelle de l’algèbre tensorielle (III, p. 56) et de la propriété universelle de l’algèbre symétrique (III, p. 68) qu’il existe un homomorphisme et un seul d’algèbres graduées
$$
\theta_T : T(M^*) \to T(M)^{\mathrm{gr}}
$$
qui prolonge l’injection canonique $M^* \to T(M)^{\mathrm{gr}}$, et un homomorphisme et un seul d’algèbres graduées
$$
\theta_S : S(M^*) \to S(M)^{\mathrm{gr}}
$$
qui prolonge l’injection canonique $M^* \to S(M)^{\mathrm{gr}}$. D’autre part, l’injection canonique de $M^*$ dans l’algèbre opposée à $\wedge (M)^{\mathrm{gr}}$ est telle que le carré de tout élément de $M^*$ soit nul; donc (III, p. 77, prop. 1) il existe un homomorphisme et un seul d’algèbres graduées
$$
\theta_\wedge : \wedge (M^*) \to (\wedge (M)^{\mathrm{gr}})^0
$$
qui prolonge l’injection canonique $M^* \to \wedge (M)^{\mathrm{gr}}$.² Ces homomorphismes sont fonctoriels: par exemple, pour tout homomorphisme $u : M \to N$ de A-modules, le diagramme
$$
\begin{array}{ccc}
T(N^*) & \xrightarrow{T(t_u)} & T(M^*) \\
\theta_T \downarrow & & \downarrow \theta_T \\
T(N)^{\mathrm{gr}} & \xrightarrow{tT(u)} & T(M)^{\mathrm{gr}}
\end{array}
$$
est commutatif, comme il résulte aussitôt de la propriété universelle de l’algèbre tensorielle (III, p. 56); on a des diagrammes commutatifs analogues pour $\theta_S$ et $\theta_\wedge$.

¹ Cela résulte aussi des formules (5) de III, p. 140 et (9) de III, p. 141.
² On prolonge cette injection en un homomorphisme dans l’algèbre opposée à $\wedge (M)^{\mathrm{gr}}$ au lieu d’un homomorphisme dans $\wedge (M)^{\mathrm{gr}}$ pour des raisons de commodité dans les calculs.

Nous allons expliciter les homomorphismes $\theta_T, \theta_S$ et $\theta_\wedge$. Pour cela, considérons de façon plus générale une A-cogèbre coassociative E de coproduit c, et définissons par récurrence sur n, pour $n \geq 2$, l’application linéaire $c_n$ de E dans $E^{\otimes n}$ par $c_2 = c$, et
$$
c_n = (c_{n-1} \otimes 1_E) \circ c.
$$
Notons d’autre part $m_n : A^{\otimes n} \to A$ l’application linéaire canonique telle que $m_n(\xi_1 \otimes \xi_2 \otimes \cdots \otimes \xi_n) = \xi_1 \xi_2 \cdots \xi_n$, et remarquons que l’on a, pour $n \geq 2$
$$
m_n = m \circ (m_{n-1} \otimes 1_A)
$$
en posant $m = m_2$. Avec ces notations:

#### Lemme 1 {#alg-iii-s11-lem-1 .statement}

(i) *Dans l’algèbre associative* $E^* = \mathrm{Hom}_A(E, A)$, le produit de n éléments $u_1, u_2, \ldots, u_n$ est donné par
$$
u_1 u_2 \ldots u_n = m_n \circ (u_1 \otimes u_2 \otimes \cdots \otimes u_n) \circ c_n.
$$
(ii) *Supposons en outre la cogèbre* E *graduée*. Alors, dans l’algèbre associative graduée $E^{*\mathrm{gr}} = \mathrm{Homgr}_A(E, A)$, le produit de n éléments $u_1, u_2, \ldots, u_n$ de degré 1 est donné par
$$
u_1 u_2 \ldots u_n = m_n \circ (u_1 \otimes u_2 \otimes \cdots \otimes u_n) \circ \delta_n
$$
où $\delta_n : E \to E^{\otimes n}$ est l’application linéaire qui, à tout $x \in E$, fait correspondre la composante de multidegré $(1, 1, \ldots, 1)$ de $c_n(x)$.

La formule (26) n’est autre que la définition du produit dans $E^*$ pour $n = 2$; pour la démontrer par récurrence sur n, on observe que
$$
\begin{align*}
u_1 u_2 \ldots u_n &= m \circ ((u_1 u_2 \ldots u_{n-1}) \otimes u_n) \circ c \\
&= m \circ ((m_{n-1} \circ (u_1 \otimes u_2 \otimes \cdots \otimes u_{n-1}) \circ c_{n-1}) \otimes u_n) \circ c \\
&= m \circ (m_{n-1} \otimes 1_A) \circ (u_1 \otimes u_2 \otimes \cdots \otimes u_{n-1} \otimes u_n) \circ (c_{n-1} \otimes 1_E) \circ c \\
&= m_n \circ (u_1 \otimes u_2 \otimes \cdots \otimes u_n) \circ c_n
\end{align*}
$$
en vertu de (24), (25), de II, p. 53, formule (5) et de la relation $u_n = 1_A \circ u_n \circ 1_E$.

Lorsque E est graduée et les éléments $u_i \in E^{*\mathrm{gr}}$ homogènes de degré 1, on a par définition pour des éléments *homogènes* $x_i \in E$
$$
(u_1 \otimes u_2 \otimes \cdots \otimes u_n)(x_1 \otimes x_2 \otimes \cdots \otimes x_n) = 0
$$
sauf si tous les $x_i$ sont de degré 1, d’où la formule (27).

Il résulte des formules (3) de III, p. 139, (5) et (7) de III, p. 140 et de la formule (24) de III, p. 152 que lorsque l’on prend pour E l’une des trois cogèbres graduées $T(M)$, $S(M)$ et $\Lambda(M)$, on obtient respectivement par récurrence sur n (compte tenu de ce que le coproduit est un homomorphisme gradué de degré 0), pour $x_1, x_2, \ldots, x_n$ dans M:
lorsque $E = T(M)$,
$$
\delta_n(x_1 x_2 \ldots x_n) = x_1 \otimes x_2 \otimes \cdots \otimes x_n
$$
lorsque $E = S(M)$,
$$
\delta_n(x_1 x_2 \ldots x_n) = \sum_{\sigma \in \mathfrak{S}_n} x_{\sigma(1)} \otimes x_{\sigma(2)} \otimes \cdots \otimes x_{\sigma(n)}
$$
lorsque $E = \Lambda(M)$,
$$
\delta_n(x_1 x_2 \ldots x_n) = \sum_{\sigma \in \mathfrak{S}_n} \varepsilon_{\sigma} x_{\sigma(1)} \otimes x_{\sigma(2)} \otimes \cdots \otimes x_{\sigma(n)}
$$

Il suffit en effet de noter, par exemple lorsque $E = \wedge(M)$, que dans l’expression
$$
c_n(x_1 x_2 \ldots x_n) = (c_{n-1} \otimes 1_E) \left( \sum (-1)^v (x_{i_1} \ldots x_{i_p}) \otimes (x_{j_1} \ldots x_{j_{n-p}}) \right)
$$
provenant de la formule (8) de III, p. 140, les seuls termes pouvant donner un terme de multidegré $(1, 1, \ldots, 1)$ sont ceux pour lesquels $n - p = 1$, donc $\delta_n(x_1 x_2 \ldots x_n)$ est le terme de multidegré $(1, 1, \ldots, 1)$ dans la somme
$$
\sum_{i=1}^n (-1)^{n-i} c_{n-1}(x_1 \ldots x_{i-1} x_{i+1} \ldots x_n) \otimes x_i
$$
et ce terme est nécessairement égal à
$$
\sum_{i=1}^n (-1)^{n-i} \delta_{n-1}(x_1 \ldots x_{i-1} x_{i+1} \ldots x_n) \otimes x_i,
$$
d’où le résultat en vertu de l’hypothèse de récurrence.

Compte tenu du lemme 1 de III, p. 152, le produit dans $T(M)^{*gr}$ de $n$ formes linéaires $x_1^*, x_2^*, \ldots, x_n^*$ de $M^*$ est donné par
$$
\langle x_1^* x_2^* \ldots x_n^*, x_1 x_2 \ldots x_n \rangle = \prod_{i=1}^n \langle x_i^*, x_i \rangle
$$
pour $x_i \in M$ ($1 \leq i \leq n$); le produit de ces $n$ formes dans $S(M)^{*gr}$ est donné par
$$
\langle x_1^* x_2^* \ldots x_n^*, x_1 x_2 \ldots x_n \rangle = \sum_{\sigma \in S_n} \left( \prod_{i=1}^n \langle x_{\sigma(i)}^*, x_i \rangle \right);
$$
enfin, le produit de ces formes dans $\wedge(M)^{*gr}$ est donné par
$$
\langle x_1^* x_2^* \ldots x_n^*, x_1 x_2 \ldots x_n \rangle = \det(\langle x_i^*, x_j \rangle).
$$

Dans chacun de ces trois cas, on a respectivement
$$
\begin{align*}
\theta_T(x_1^* \otimes x_2^* \otimes \cdots \otimes x_n^*) &= x_1^* x_2^* \ldots x_n^* \\
\theta_S(x_1^* x_2^* \ldots x_n^*) &= x_1^* x_2^* \ldots x_n^* \\
\theta_\wedge(x_1^* \wedge x_2^* \wedge \cdots \wedge x_n^*) &= x_n^* x_{n-1}^* \ldots x_1^* = (-1)^{n(n-1)/2} x_1^* x_2^* \ldots x_n^*
\end{align*}
$$
donc on déduit de (28), (29) et (30) les relations
$$
\langle \theta_T(x_1^* \otimes x_2^* \otimes \cdots \otimes x_n^*), x_1 \otimes x_2 \otimes \cdots \otimes x_n \rangle = \prod_{i=1}^n \langle x_i^*, x_i \rangle
$$
(en d’autres termes, $\theta_T$ restreint à $T^2(M^*)$, n’est autre que l’homomorphisme canonique de II, p. 80)

$$
\langle \theta_S(x_1^* x_2^* \ldots x_n^*), x_1 x_2 \ldots x_n \rangle = \sum_{\sigma \in S_n} \left( \prod_{i=1}^n \langle x_{\sigma(i)}^*, x_i \rangle \right)
$$
$$
\langle \theta_\wedge(x_1^* \wedge x_2^* \wedge \cdots \wedge x_n^*), x_1 \wedge x_2 \wedge \cdots \wedge x_n \rangle = (-1)^{n(n-1)/2} \det(\langle x_i^*, x_j \rangle).
$$

#### Proposition 7 {#alg-iii-s11-prop-7 .statement}

Soit $M$ un $A$-module projectif de type fini. Alors les homomorphismes canoniques $\theta_T : T(M^*) \to T(M)^{*gr}$ et $\theta_\wedge : \wedge(M^*) \to (\wedge(M)^{*gr})^0$ sont bijectifs. En outre le dual gradué $\wedge(M)^{*gr}$ est alors égal au dual $\wedge(M)^*$ du $A$-module $\wedge(M)$.

Supposons d’abord que $M$ ait une base finie $(e_i)_{1 \leq i \leq m}$, et soit $(e_i^*)_{1 \leq i \leq m}$ la base duale de $M^*$ (II, p. 45). La formule (28 bis) de III, p. 153, montre que pour toute suite finie $s = (j_k)_{1 \leq k \leq n}$ de $n$ éléments de l’intervalle $[1, m]$ de $\mathbf{N}$, $\theta_T(e_{j_1}^* \otimes \cdots \otimes e_{j_n}^*)$ est l’élément d’indice $s$ de la base de $(T^n(M))^*$, *duale* de la base de $T^n(M)$ formée des $e_s = e_{j_1} \otimes \cdots \otimes e_{j_n}$ (III, p. 62, th. 1). Donc $\theta_T$ est bijectif.

De même, la formule (30 bis) de III, p. 153 montre que pour toute partie finie $H$ de $[1, m]$ ayant $n$ éléments, $(-1)^{n(n-1)/2} \theta_\wedge(e_H^*)$ (notation de III, p. 86, th. 1) est l’élément d’indice $H$ de la base de $(\wedge^n(M))^*$, *duale* de la base de $\wedge^n(M)$ formée des $e_H$. Donc $\theta_\wedge$ est bijectif.

Supposons seulement maintenant que $M$ soit projectif de type fini; alors $M$ est facteur direct d’un $A$-module libre de type fini $L$, de sorte qu’il existe deux applications $A$-linéaires $M \xrightarrow{j} L \xrightarrow{p} M$ dont le composé est l’identité $1_M$. On en déduit un diagramme commutatif

$$
\begin{array}{ccccc}
T(M^*) & \xrightarrow{T(t_j)} & T(L^*) & \xrightarrow{T(t_p)} & T(M^*) \\
\theta_T \downarrow & & \theta_T \downarrow & & \theta_T \downarrow \\
T(M)^{*gr} & \xrightarrow{t_{T(j)}} & T(L)^{*gr} & \xrightarrow{t_{T(p)}} & T(M)^{*gr}
\end{array}
$$

et un diagramme commutatif analogue où $T$ est remplacé par $\wedge$. La proposition résulte alors du lemme suivant:

#### Lemme 2 {#alg-iii-s11-lem-2 .statement}

Soit

$$
\begin{array}{ccccc}
X & \xrightarrow{u} & Y & \xrightarrow{v} & X \\
f \downarrow & & g \downarrow & & f \downarrow \\
X' & \xrightarrow{u'} & Y' & \xrightarrow{v'} & X'
\end{array}
$$

un diagramme commutatif d’ensembles et d’applications tel que $v \circ u$ et $v' \circ u'$ soient les applications identiques de $X$ et $X'$ respectivement. Alors, si $g$ est injective (resp. surjective, resp. bijective), il en est de même de $f$.

En effet, $u$ est injective puisque $v \circ u$ l’est; donc, si $g$ est injective, $u' \circ f = g \circ u$ est injective, et par suite $f$ est injective. De même $v'$ est surjective puisque $v' \circ u'$ l’est; donc, si $g$ est surjective, $f \circ v = v' \circ g$ est surjective et par suite $f$ est surjective.

La dernière assertion de la prop. 7 résulte de ce que $\wedge(M)$ est alors un $A$-module de type fini (III, p. 80, prop. 6 et II, p. 175, Remarque).

Examinons maintenant ce qu’on peut dire de l’homomorphisme $\theta_S$ lorsque $M$ est *projectif de type fini*. Supposons d’abord que $M$ admette une base finie $(e_i)_{1 \leq i \leq m}$. Avec les notations du début du chapitre, le $A$-module $S^n(M)$ admet pour base la famille des éléments $e^\alpha$ tels que $|\alpha| = n$. Notons $u_\alpha$ (pour $|\alpha| = n$) l’élément d’indice $\alpha$ dans la base de $(\mathbf{S}^n(\mathbf{M}))^*$ *duale* de $(e^\alpha)$. Les éléments $u_\alpha$, pour $\alpha \in \mathbf{N}^m$, forment donc une base de l’algèbre $\mathbf{S}(\mathbf{M})^{*\mathrm{gr}}$ et nous allons expliciter la table de multiplication de cette base. Posons

$$
u_\alpha u_\beta = \sum_{\gamma \in \mathbf{N}^m} a_{\alpha \beta \gamma} u_\gamma \quad \text{avec } a_{\alpha \beta \gamma} \in \mathbf{A}.
$$

On a par définition $a_{\alpha \beta \gamma} = \langle u_\alpha u_\beta, e^\gamma \rangle = m((u_\alpha \otimes u_\beta)(c(e^\gamma)))$, où $m : \mathbf{A} \otimes \mathbf{A} \to \mathbf{A}$ définit la multiplication dans $\mathbf{A}$ et $c$ est le coproduit de $\mathbf{S}(\mathbf{M})$. En d’autres termes, $a_{\alpha \beta \gamma}$ n’est autre que le coefficient de $e^\alpha \otimes e^\beta$ lorsque l’on écrit $c(e^\gamma)$ au moyen de la base de $\mathbf{S}(\mathbf{M}) \otimes \mathbf{S}(\mathbf{M})$ formée des $e^\xi \otimes e^n$, où $\xi$ et $\eta$ parcourent $\mathbf{N}^m$. Mais puisque $c$ est un homomorphisme d’algèbres, on a

$$
c(e^\gamma) = \prod_{i=1}^m (c(e_i))^{\gamma_i} = \prod_{i=1}^m (e_i \otimes 1 + 1 \otimes e_j)^{\gamma_i}
$$

en vertu du la formule (4) du n° 1 ; cela donne

$$(31)$$
$$
c(e^\gamma) = \sum_{\xi + \eta = \gamma} ((\xi, \eta)) e^\xi \otimes e^\eta
$$

où l’on pose

$$(32)$$
$$
((\xi, \eta)) = \prod_{i=1}^n \frac{(\xi_i + \eta_i)!}{\xi_i! \eta_i!} \quad \text{(cf. III, p. 122, formule (18))}.
$$

On obtient donc la table de multiplication

$$(33)$$
$$
u_\alpha u_\beta = ((\alpha, \beta)) u_{\alpha + \beta}.
$$

D’autre part, si $(e_i^*)_{1 \leq i \leq m}$ est la base de $\mathbf{M}^*$, duale de $(e_i)$, il résulte de la formule (29 bis) (III, p. 153) que l’on a, pour tout $\alpha \in \mathbf{N}^m$,

$$(34)$$
$$
\theta_S(e^{*\alpha}) = \alpha ! u_\alpha
$$

avec les notations de III, p. 75. L’homomorphisme $\theta_S$ est donc bijectif si et seulement si les $\alpha ! u_\alpha$ forment une *base* de $\mathbf{S}(\mathbf{M})^{*\mathrm{gr}}$, ou encore si les éléments $\alpha ! 1$ dans $\mathbf{A}$ sont *inversibles*.

#### Proposition 8 {#alg-iii-s11-prop-8 .statement}

*Supposons que l’anneau $\mathbf{A}$ soit une algèbre sur le corps $\mathbf{Q}$ des nombres rationnels ; alors, pour tout $\mathbf{A}$-module projectif de type fini $\mathbf{M}$, l’homomorphisme*

$$
\theta_S : \mathbf{S}(\mathbf{M}^*) \to \mathbf{S}(\mathbf{M})^{*\mathrm{gr}}
$$

*est bijectif*.

On vient en effet de le prouver lorsque $\mathbf{M}$ est libre de type fini ; on passe de là au cas général en utilisant le lemme 2 de III, p. 154, comme dans la démonstration de la prop. 7 de III, p. 154.

#### Remarque {#alg-iii-s11-n5-rem-1 .statement}

Soient M un A-module, $\rho : A \to B$ un homomorphisme d’anneaux commutatifs. On a alors un diagramme d’homomorphismes de B-algèbres graduées

$$
\begin{array}{ccc}
T((M^*)_{(B)}) & \longrightarrow & (T(M)^{*gr})_{(B)} \\
\downarrow T(\nu_M) & & \downarrow \nu_{T(M)} \\
T((M_{(B)})^*) & \xrightarrow{\theta_T} & T(M_{(B)})^{*gr}
\end{array}
$$

où la première ligne est l’homomorphisme composé de l’homomorphisme $\theta_T \otimes 1_B : T(M^*) \otimes_A B \to T(M)^{*gr} \otimes_A B$, et de l’isomorphisme canonique

$$
T((M^*)_{(B)}) \to T(M^*) \otimes_A B
$$

(III, p. 60, prop. 5). On vérifie aussitôt, compte tenu de la formule (28) et de la définition de l’homomorphisme $\nu_E$ (II, p. 87) que ce diagramme est *commutatif*. Lorsque M est un A-module *projectif de type fini*, $M_{(B)}$ est un B-module projectif de type fini (II, p. 84, corollaire), et tous les homomorphismes du diagramme précédent sont *bijectifs* (III, p. 154, prop. 7 et II, p. 88, prop. 8). On a des diagrammes commutatifs analogues en remplaçant T par S ou $\wedge$; le diagramme relatif à $\wedge$ est encore formé d’homomorphismes bijectifs lorsque M est projectif de type fini (III, p. 154, prop. 7); si de plus A est une algèbre sur $\mathbf{Q}$, le diagramme relatif à S est aussi formé d’homomorphismes bijectifs (III, p. 155, prop. 8).

### 6. Produits intérieurs: cas des algèbres

Soient $E = \bigoplus_{p \geq 0} E_p$ une *A-algèbre graduée* de type $\mathbf{N}$, P un A-module gradué de type $\mathbf{Z}$; pour tout élément *homogène* $x \in E_p$, la multiplication *à gauche* par x est une application A-linéaire $e(x)$ de E dans lui-même qui est *graduée de degré p*. Pour tout élément $u \in \mathrm{Homgr}_A(E, P)$, on appelle *produit intérieur droit de u par x* et on note $u \triangleleft x$ l’élément $u \circ e(x)$ de $\mathrm{Homgr}_A(E, P)$. On écrit aussi $(i(x))(u) = u \triangleleft x$, et on voit que $i(x)$ est un endomorphisme gradué de degré $p$ du A-module gradué $\mathrm{Homgr}_A(E, P)$. Si maintenant $x = \sum_{p \geq 0} x_p$ est un élément quelconque de E (avec $x_p \in E_p$ pour tout $p \geq 0$, $x_p = 0$ sauf pour un nombre fini de valeurs de $p$), on pose $i(x) = \sum_{p=0}^\infty i(x_p)$, qui est donc un endomorphisme du A-module $\mathrm{Homgr}_A(E, P)$.

Pour se souvenir de l’élément qui, dans l’expression $u \triangleleft x$, « opère » sur l’autre, on observera que l’élément x qui « opère » sur u est placé à l’extrémité libre du trait horizontal dans $\triangleleft$.

L’*associativité* de l’algèbre E se traduit par la relation $e(xy) = e(x) \circ e(y)$ pour $x, y$ homogènes; d’où, par définition de $i(x)$

$$
i(xy) = i(y) \circ i(x)
$$

d’abord pour $x, y$ homogènes, puis, par linéarité, pour $x, y$ quelconques dans $E$; cela s’écrit aussi
$$(36)$$
$$(u \llcorner x) \llcorner y = u \llcorner (xy)$$
pour $x, y$ dans $E$ et $u \in \mathrm{Homgr}_A(E, P)$; comme d’autre part il est clair que $i(1)$ est l’application identique (puisqu’il en est ainsi de $e(1) = 1_E$), et que $x \mapsto i(x)$ est $A$-linéaire, on voit que la loi d’action $(x, u) \mapsto u \llcorner x$ ($x \in E, u \in \mathrm{Homgr}_A(E, P)$) définit, avec l’addition, une structure de $E$-module à droite sur $\mathrm{Homgr}_A(E, P)$.

On aura en particulier à considérer le cas $P = A$, $\mathrm{Homgr}_A(E, P)$ étant dans ce cas le dual gradué $E^{*\mathrm{gr}}$ de $E$; $i(x)$ est alors la transposée graduée de l’application $A$-linéaire $e(x)$ (II, p. 176), autrement dit, quels que soient $x, y$ dans $E, u \in E^{*\mathrm{gr}}$, on a
$$(37)$$
$$\langle u \llcorner x, y \rangle = \langle u, xy \rangle.$$

Avec la convention du début du paragraphe, on notera que si $x \in E_p, i(x)$ est un endomorphisme de $E^{*\mathrm{gr}}$ de degré $-p$.

Pour tout élément homogène $x \in E_p$, on note de même $e'(x)$ la multiplication à droite par $x$, par $x \lrcorner u$ l’élément $u \circ e'(x)$ de $\mathrm{Homgr}_A(E, P)$, qu’on appelle le produit intérieur gauche de $u$ par $x$; on pose $i'(x)(u) = x \lrcorner u$, et $i'(x)$ est donc un endomorphisme gradué de degré $p$ de $\mathrm{Homgr}_A(E, P)$; on étend comme ci-dessus cette définition au cas où $x$ est un élément quelconque de $E$. Comme ici $e'(xy) = e'(y) \circ e'(x)$, on a
$$(38)$$
$$i'(xy) = i'(x) \circ i'(y)$$
qui s’écrit aussi
$$(39)$$
$$x \lrcorner (y \lrcorner u) = (xy) \lrcorner u$$
et montre que la loi d’action $(x, u) \mapsto x \lrcorner u$ définit, avec l’addition, une structure de $E$-module à gauche sur $\mathrm{Homgr}_A(E, P)$. L’associativité de $E$ entraîne d’autre part que $e(x) \circ e'(y) = e'(y) \circ e(x)$ pour $x, y$ homogènes dans $E$, d’où la relation
$$(40)$$
$$(y \lrcorner u) \llcorner x = y \lrcorner (u \llcorner x)$$
de sorte que les deux lois d’action sur $\mathrm{Homgr}_A(E, P)$ définissent sur cet ensemble une structure de $(E, E)$-bimodule (II, p. 33).

Lorsqu’on prend $P = A$, $i'(x)$ est la transposée graduée de $e'(x)$; autrement dit, quels que soient $x, y$ dans $E, u \in E^{*\mathrm{gr}}$, on a
$$(41)$$
$$\langle y, x \lrcorner u \rangle = \langle yx, u \rangle.$$

Lorsque l’algèbre graduée $E$ est commutative, on a évidemment $u \llcorner x = x \lrcorner u$. Lorsque $E$ est anticommutative et $P = A$, on a, pour $x \in E_p, y \in E_r$ et $u \in E_q^*$, $yx = (-1)^{pr} xy$, d’où par (37) et (41), $\langle u \llcorner x, y \rangle = (-1)^{pr} \langle y, x \lrcorner u \rangle$. Mais comme les deux membres de cette relation sont nuls sauf pour $r = q - p$, on a $x \lrcorner u = (-1)^{p(q-p)} u \llcorner x$.

Soient F une seconde A-algèbre graduée et $\varphi : E \to F$ un A-homomorphisme d’algèbres graduées; alors $\tilde{\varphi} = \mathrm{Hom}(\varphi, 1_P) : \mathrm{Homgr}_A(F, P) \to \mathrm{Homgr}_A(E, P)$ est un A-homomorphisme gradué de degré 0; par définition, pour $x, y$ dans E et $u \in \mathrm{Homgr}_A(F, P)$

$$
(\tilde{\varphi}(u \sqcup \varphi(x)))(y) = (u \sqcup \varphi(x))(\varphi(y))
= u(\varphi(x)\varphi(y)) = u(\varphi(xy)) = (\tilde{\varphi}(u))(xy) = (\tilde{\varphi}(u) \sqcup x)(y)
$$

ou encore

$$(42)$$
$$
\tilde{\varphi}(u \sqcup \varphi(x)) = \tilde{\varphi}(u) \sqcup x
$$

et on a de même

$$(43)$$
$$
\tilde{\varphi}(\varphi(x) \sqcup u) = x \sqcup \tilde{\varphi}(u).
$$

En d’autres termes, lorsque $\mathrm{Homgr}_A(F, P)$ est considéré comme un (E, E)-bimodule au moyen de l’homomorphisme d’anneaux $\varphi : E \to F$, on voit que $\tilde{\varphi}$ est un homomorphisme de (E, E)-bimodules (ou encore un E-homomorphisme du (F, F)-bimodule $\mathrm{Homgr}_A(F, P)$ dans le (E, E)-bimodule $\mathrm{Homgr}_A(E, P)$).

#### Exemple {#alg-iii-s11-n6-exa-1 .statement}

On peut en particulier appliquer ce qui précède lorsque E est l’une des algèbres graduées $T(M)$, $S(M)$ ou $\wedge(M)$ pour un A-module M, et P un A-module (muni de la graduation triviale). Pour expliciter les structures de bimodule ainsi obtenues, notons que les éléments de degré $-n$ de $\mathrm{Homgr}_A(T(M), P)$ (resp. $\mathrm{Homgr}_A(S(M), P)$, resp. $\mathrm{Homgr}_A(\wedge(M), P)$) sont identifiés aux *applications n-linéaires* (resp. aux *applications n-linéaires symétriques*, resp. aux *applications n-linéaires alternées*) de $M^n$ dans P. Il suffit d’exprimer les produits

$$
f \sqcup (x_1 \otimes x_2 \otimes \cdots \otimes x_p)
$$

(resp. $f \sqcup (x_1 x_2 \ldots x_p)$, resp. $f \sqcup (x_1 \wedge x_2 \wedge \cdots \wedge x_p)$) pour toute suite finie $(x_i)_{1 \leq i \leq p}$ d’éléments de M et les analogues pour le produit intérieur gauche. Il résulte aussitôt des définitions que l’on a

$$(44)$$
$$
f \sqcup (x_1 \otimes x_2 \otimes \cdots \otimes x_p) = (x_1 \otimes x_2 \otimes \cdots \otimes x_p) \sqcup f = 0 \quad \text{si } p > n
$$

et que, pour $p \leq n$, $f \sqcup (x_1 \otimes x_2 \otimes \cdots \otimes x_p)$ (resp. $(x_1 \otimes x_2 \otimes \cdots \otimes x_p) \sqcup f$) est l’*application* $(n - p)$*-linéaire* définie par

$$(45)$$
$$
\begin{cases}
(f \sqcup (x_1 \otimes x_2 \otimes \cdots \otimes x_p))(y_1, \ldots, y_{n-p}) = f(x_1, \ldots, x_p, y_1, \ldots, y_{n-p}) \\
((x_1 \otimes x_2 \otimes \cdots \otimes x_p) \sqcup f)(y_1, \ldots, y_{n-p}) = f(y_1, \ldots, y_{n-p}, x_1, \ldots, x_p)
\end{cases}
$$

Pour $p > n$, on a encore dans $\mathrm{Homgr}_A(S(M), P)$ (resp. $\mathrm{Homgr}_A(\wedge(M), P)$) les formules (44) en y remplaçant $x_1 \otimes x_2 \otimes \ldots \otimes x_p$ par $x_1 x_2 \ldots x_p$ (resp. $x_1 \wedge x_2 \wedge \cdots \wedge x_p$). Pour $p \leq n$, les mêmes substitutions dans (45) définissent les *applications* $(n - p)$*-linéaires symétriques* $f \sqcup (x_1 x_2 \ldots x_p)$ et $(x_1 x_2 \ldots x_p) \sqcup f$ (resp. les *applications* $(n - p)$*-linéaires alternées*

$$
f \sqcup (x_1 \wedge x_2 \wedge \cdots \wedge x_p) \text{ et } (x_1 \wedge x_2 \wedge \cdots \wedge x_p) \sqcup f.
$$

Lorsque $n = p$, les produits précédents sont égaux à la fonction constante sur M égale à $f(x_1, \ldots, x_p)$.

Si $u : M \to N$ est un homomorphisme de A-modules, $T(u) : T(M) \to T(N)$ est un homomorphisme de A-algèbres graduées, donc il résulte de ce qu’on a vu ci-dessus que $T(u))^\sim$ est un $T(M)$-homomorphisme du $(T(N), T(N))$-bimodule $\mathrm{Homgr}_A(T(N), P)$ dans le $(T(M), T(M))$-bimodule $\mathrm{Homgr}_A(T(M), P)$, relatif à l’homomorphisme d’anneaux $T(u)$. On a des résultats analogues pour $(S(u))^\sim$ et $(\wedge(u))^\sim$.

### 7. Produits intérieurs: cas des cogèbres

Soit $E = \bigoplus_{p \geq 0} E_p$ une cogèbre graduée coassociative et couinifère. On sait alors (III, p. 143, prop. 1 et p. 145, prop. 3) que le dual gradué $E^{*\mathrm{gr}}$ est muni (avec la convention de graduation faite au début du paragraphe) d’une structure d’algèbre graduée de type $\mathbf{N}$ sur $A$, le produit de deux éléments $u, v$ de cette algèbre étant défini par $uv = m \circ (u \otimes v) \circ c$, où $c : E \to E \otimes_A E$ est le coproduit et $m : A \otimes_A A \to A$ définit la multiplication. Autrement dit, si, pour $x \in E$, on a $c(x) = \sum_i y_i \otimes z_i$, on peut écrire (en identifiant canoniquement $A \otimes_A E$ et $E$)

$$
\langle x, uv \rangle = (uv)(x) = \sum_i u(y_i)v(z_i) = v\left( \sum_i u(y_i)z_i \right)
= v(((u \otimes 1_E) \circ c)(x)) = \langle ((u \otimes 1_E) \circ c)(x), v \rangle.
$$

Cela peut s’interpréter en disant que pour tout $u$ homogène de degré $p$ dans $E^{*\mathrm{gr}}$, la multiplication à gauche $e(u) : v \mapsto uv$ dans $E^{*\mathrm{gr}}$ est le transposé gradué de l’endomorphisme gradué de degré $-p$

$$(46)$$
$$
i(u) = (u \otimes 1_E) \circ c
$$

de $E$; avec les notations précédentes, on a donc

$$
(i(u))(x) = \sum_i u(y_i)z_i.
$$

La formule (46) définit d’ailleurs un élément $i(u) \in \mathrm{Endgr}_A(E)$ pour tout élément $u \in E^{*\mathrm{gr}}$; pour tout $x \in E$ et tout $u \in E^{*\mathrm{gr}}$, on pose

$$(47)$$
$$
x \prec u = (i(u))(x)
$$

de sorte que, pour $u$ et $v$ dans $E^{*\mathrm{gr}}$, on a

$$
\langle x, uv \rangle = \langle x \prec u, v \rangle.
$$

On dit que l’élément $x \prec u$ de $E$ est le produit intérieur droit de $x$ par $u$.

Ici encore, l’élément $u$ qui « opère » sur $x$ est placé à l’extrémité libre du trait horizontal dans $\prec$.

Pour deux éléments quelconques $u, v$ de $E^{*\mathrm{gr}}$, on a
$$
x \mathbin{\mathcal{L}} (uv) = (x \mathbin{\mathcal{L}} u) \mathbin{\mathcal{L}} v,
$$
autrement dit
$$
i(uv) = i(v) \circ i(u).
$$
En effet, posons comme ci-dessus $c(x) = \sum_i y_i \otimes z_i$, de sorte que $x \mathbin{\mathcal{L}} (uv) = \sum_i (uv)(y_i)z_i$. Si $c(y_i) = \sum_j y_{ij}' \otimes y_{ij}''$, on a donc
$$
x \mathbin{\mathcal{L}} (uv) = \sum_{i,j} u(y_{ij}')v(y_{ij}'')z_i.
$$
D’autre part, si $c(z_i) = \sum_k z_{ik}' \otimes z_{ik}''$, on a
$$
(x \mathbin{\mathcal{L}} u) \mathbin{\mathcal{L}} v = \sum_{i,k} u(y_i)v(z_{ik}')z_{ik}''.
$$
Or, la coassociativité de $E$ montre que l’on a (III, p. 143, prop. 1)
$$
\sum_{i,j} y_{ij}' \otimes y_{ij}'' \otimes z_i = \sum_{i,k} y_i \otimes z_{ik}' \otimes z_{ik}''
$$
et l’égalité des expressions (49) et (50) provient de ce que ce sont respectivement l’image du premier et du second membre de (51) par l’application linéaire $f$ de $E \otimes E \otimes E$ dans $A$ telle que $f(x \otimes y \otimes z) = u(x)v(y)z$.

Rappelons d’autre part (III, p. 145, prop. 3) que l’élément unité de l’algèbre $E^{*\mathrm{gr}}$ est la forme linéaire $e : x \mapsto \gamma(x).1$; on a donc
$$
x \mathbin{\mathcal{L}} e = \sum_i \gamma(y_i)z_i = x
$$
en vertu de la définition d’une coïunité. Comme l’application $u \mapsto i(u)$ est linéaire, on voit que sur $E$, la loi d’action $(u, x) \mapsto x \mathbin{\mathcal{L}} u$ définit une structure de $E^{*\mathrm{gr}}$-module à droite.

On définit de même, pour tout $u \in E^{*\mathrm{gr}}$, l’endomorphisme de $E$
$$
i'(u) = (1_E \otimes u) \circ c
$$
et, pour tout $x \in E$, on pose
$$
(i'(u))(x) = u \mathbin{\mathcal{L}} x
$$
et on dit que cet élément de $E$ est le produit intérieur gauche de $x$ par $u$. On voit comme ci-dessus que la loi d’action $(u, x) \mapsto u \mathbin{\mathcal{L}} x$ définit sur $E$ une structure de $E^{*\mathrm{gr}}$-module à gauche. En outre, ces deux structures sont compatibles, autrement dit, on a
$$
(u \mathbin{\mathcal{L}} x) \mathbin{\mathcal{L}} v = u \mathbin{\mathcal{L}} (x \mathbin{\mathcal{L}} v)
$$
pour $u, v$ dans $E^{*\mathrm{gr}}$ (II, p. 33). En effet, avec les mêmes notations que ci-dessus, le premier membre de (54) est $\sum_{i,j} u(z_i)v(y_{ij}')y_{ij}'$ et le second est $\sum_{i,k} v(y_i)u(z_{ik}')z_{ik}'$; leur égalité résulte de ce que ce sont les images respectives du premier et du second membre de (51) par l’application linéaire $g$ de $E \otimes E \otimes E$ dans $A$ telle que $g(x \otimes y \otimes z) = v(x)u(z)y$.

On voit donc que les deux lois d’action sur $E$ définissent sur cet ensemble une structure de $(E^{*gr}, E^{*gr})$-bimodule.

Lorsque la cogèbre $E$ est cocommutative, on a $u \lhd x = x \rhd u$ quels que soient $x \in E$ et $u \in E^{*gr}$; lorsqu’elle est anticocommutative (III, p. 53), et que $u \in E_p^*$ et $x \in E_q$, on peut écrire $c(x) = \sum_{0 \leq j \leq q} (\sum_i y_{ij} \otimes z_{i, q-j})$ avec $y_{ij}$ et $z_{ij}$ dans $E_j$ pour tout $j$, et l’on a par hypothèse

$$
\sum_i z_{ij} \otimes y_{i, q-j} = (-1)^{j(q-j)} \sum_i y_{ij} \otimes z_{i, q-j}.
$$

Par définition, on a $x \rhd u = \sum_{0 \leq j \leq q} (\sum_i u(y_{ij})z_{i, q-j})$ et

$$
u \lhd x = \sum_{0 \leq j \leq q} (\sum_i u(z_{i, q-j})y_{ij}).
$$

Comme $u(y_{ij}) = 0$ (resp. $u(z_{i, q-j}) = 0$) sauf si $j = p$ (resp. $q - j = p$), on voit d’après ce qui précède que l’on a $u \lhd x = (-1)^{p(q-p)}x \rhd u$.

Enfin, soit $\varphi : E \to F$ un morphisme de cogèbres graduées; on a vu alors (III, p. 143) que le transposé gradué $^t\varphi : F^{*gr} \to E^{*gr}$ est un homomorphisme d’algèbres graduées; on a par suite, pour $x \in E, u, v$ dans $F^{*gr}$,

$$
\langle \varphi(x \rhd ^t\varphi(u)), v \rangle = \langle x \rhd ^t\varphi(u), ^t\varphi(v) \rangle = \langle x, ^t\varphi(u)^t\varphi(v) \rangle = \langle x, ^t\varphi(uv) \rangle
$$
d’où
(55)
$$
\varphi(x) \rhd u = \varphi(x \rhd ^t\varphi(u));
$$
et de même
(56)
$$
u \lhd \varphi(x) = \varphi(^t\varphi(u) \lhd x).
$$

Autrement dit, $\varphi$ est un $F^{*gr}$-homomorphisme du $(E^{*gr}, E^{*gr})$-bimodule $E$ dans le $(F^{*gr}, F^{*gr})$-bimodule $F$, relatif à l’homomorphisme d’anneaux $^t\varphi : F^{*gr} \to E^{*gr}$.

#### Exemple {#alg-iii-s11-n7-exa-1 .statement}

On peut en particulier appliquer ce qui précède lorsque $E$ est l’une des cogèbres graduées $T(M), S(M)$ ou $\wedge(M)$ pour un $A$-module $M$ (III, p. 139–140, Exemples 5, 6 et 7). Pour expliciter les structures de bimodule ainsi obtenues, identifions encore un élément homogène $f$ de degré $n$ dans $T(M)^{*gr}$ (resp. $S(M)^{*gr}$, resp. $\wedge(M)^{*gr}$) à une forme $n$-linéaire (resp. une forme $n$-linéaire symétrique, resp. une forme n-linéaire alternée, dite aussi n-forme) sur $M^n$. Il suffit d’exprimer les produits $(x_1 \otimes x_2 \otimes \cdots \otimes x_p) \lhd f$ (resp. $(x_1 x_2 \ldots x_p) \lhd f$, resp. $(x_1 \wedge x_2 \wedge \cdots \wedge x_p) \lhd f$) pour toute suite finie $(x_i)_{1 \leq i \leq p}$ d’éléments de $M$ et les analogues pour le produit intérieur gauche. Or, les définitions (46) (III, p. 159) et (52) (III, p. 160) et les formules (3), (6) et (9) de III, p. 139–141, donnent respectivement

$$
(57)\quad \begin{cases}
(x_1 \otimes x_2 \otimes \cdots \otimes x_p) \lhd f = f \lhd (x_1 \otimes x_2 \otimes \cdots \otimes x_p) = 0 \\
(x_1 x_2 \ldots x_p) \lhd f = f \lhd (x_1 x_2 \ldots x_p) = 0 & \text{pour } p < n \\
(x_1 \wedge x_2 \wedge \cdots \wedge x_p) \lhd f = f \lhd (x_1 \wedge x_2 \wedge \cdots \wedge x_p) = 0
\end{cases}
$$

Pour $p \geq n$, on a respectivement

$$
(58)\quad (x_1 \otimes x_2 \otimes \cdots \otimes x_p) \lhd f = f(x_1, \ldots, x_n)x_{n+1} \otimes \cdots \otimes x_p
$$
$$
(59)\quad (x_1 x_2 \ldots x_p) \lhd f = \sum_\sigma f(x_{\sigma(1)}, \ldots, x_{\sigma(n)}) x_{\sigma(n+1)} \cdots x_{\sigma(p)}
$$
$$
(60)\quad (x_1 \wedge x_2 \wedge \cdots \wedge x_p) \lhd f = \sum_\sigma \varepsilon_\sigma f(x_{\sigma(1)}, \ldots, x_{\sigma(n)}) x_{\sigma(n+1)} \wedge \ldots \wedge x_{\sigma(p)}
$$

(où, dans (59) et (60), les sommations sont étendues aux permutations $\sigma \in \mathfrak{S}_p$ croissantes dans chacun des intervalles $[1, n]$ et $[n+1, p]$ de $\mathbf{N}$); et de même

$$
(61)\quad f \lhd (x_1 \otimes x_2 \otimes \cdots \otimes x_p) = f(x_{p-n+1}, \ldots, x_p)x_1 \otimes x_2 \otimes \cdots \otimes x_{p-n}
$$
$$
(62)\quad f \lhd (x_1 x_2 \ldots x_p) = \sum_\sigma f(x_{\sigma(p-n+1)}, \ldots, x_{\sigma(p)}) x_{\sigma(1)} \cdots x_{\sigma(p-n)}
$$
$$
(63)\quad f \lhd (x_1 \wedge x_2 \wedge \cdots \wedge x_p) =
\sum_\sigma \varepsilon_\sigma f(x_{\sigma(p-n+1)}, \ldots, x_{\sigma(p)}) x_{\sigma(1)} \wedge \ldots \wedge x_{\sigma(p-n)}
$$

(où, dans (62) et (63), les sommations sont étendues aux permutations $\sigma \in \mathfrak{S}_p$ croissantes dans chacun des intervalles $[1, p-n]$ et $[p-n+1, p]$ de $\mathbf{N}$).

### 8. Produits intérieurs : cas des bigèbres

Soit $E$ une bigèbre graduée (resp. une bigèbre graduée gauche) (III, p. 148, déf. 3); on peut alors appliquer les résultats des n°s 6 et 7 pour définir les produits intérieurs droits (resp. gauches) $x \lhd u \in E$ et $u \lhd x \in E^{*\mathrm{gr}}$ (resp. $u \lhd x \in E$ et $x \lhd u \in E^{*\mathrm{gr}}$) pour tout $x \in E$ et tout $u \in E^{*\mathrm{gr}}$. On obtient ainsi une structure de $(E, E)$-bimodule sur $E^{*\mathrm{gr}}$ et une structure de $(E^{*\mathrm{gr}}, E^{*\mathrm{gr}})$-bimodule sur $E$. De plus:

#### Proposition 9 {#alg-iii-s11-prop-9 .statement}

*Soit $E$ une bigèbre graduée (resp. une bigèbre graduée gauche). Pour tout élément $x$ de degré 1 dans $E$, les produits intérieurs gauche et droit par $x$ sont des dérivations (resp. des antidérivations) (III, p. 117–118) de l’algèbre $E^{*\mathrm{gr}}$.*

Les notations étant celles de III, p. 156, on a, pour tout élément $x$ homogène et de degré 1 dans une bigèbre graduée (resp. une bigèbre graduée gauche) $E$, c(x) = x \otimes 1 + 1 \otimes x, en vertu de la prop. 5 de III, p. 147 et du fait que c est un homomorphisme de degré 0. Supposons d’abord que E soit une bigèbre graduée. Pour tout $y \in E$, on a par définition

$$
\langle (uv) \llcorner x, y \rangle = \langle uv, xy \rangle = m((u \otimes v)(c(xy)))
$$

et puisque c est un homomorphisme d’algèbres, $c(xy) = c(x)c(y)$. Posons $c(y) = \sum_i s_i \otimes t_i$ avec $s_i$ et $t_i$ dans E; on a par suite

$$
c(xy) = \sum_i (xs_i) \otimes t_i + \sum_i s_i \otimes (xt_i).
$$

On a donc $\langle (uv) \llcorner x, y \rangle = \sum_i u(xs_i)v(t_i) + \sum_i u(s_i)v(xt_i)$. Mais on peut écrire

$$
\sum_i u(xs_i)v(t_i) = m(((u \llcorner x) \otimes v)(c(y))) = \langle (u \llcorner x)v, y \rangle,
$$

et de même

$$
\sum_i u(s_i)v(xt_i) = m((u \otimes (v \llcorner x))(c(y))) = \langle u(v \llcorner x), y \rangle,
$$

d’où, en revenant à la notation $i(x)$ pour le produit intérieur

(64)
$$
(i(x))(uv) = ((i(x))(u))v + u((i(x))(v))
$$

ce qui prouve que $i(x)$ est une *dérivation* dans $E^{*\mathrm{gr}}$.

Supposons maintenant que E soit une bigèbre graduée *gauche*, que $u \in E_p^*$, $v \in E_q^*$ et $y \in E_r$; on peut alors écrire

$$
c(y) = \sum_{0 \leq j \leq r} \left( \sum_i s_{ij} \otimes t_{i,r-j} \right)
$$

où les $s_{ij}$ et $t_{ij}$ appartiennent à $E_j$; par définition du produit dans $E^g \otimes_A E$, on a alors

$$
c(xy) = c(x)c(y) = \sum_{0 \leq j \leq r} \left( \sum_i (xs_{ij}) \otimes t_{i,r-j} + (-1)^j \sum_i s_{ij} \otimes (xt_{i,r-j}) \right)
$$

d’où cette fois

$$
\langle (uv) \llcorner x, y \rangle = \sum_{0 \leq j \leq r} \left( \sum_i u(xs_{ij})v(t_{i,r-j}) + (-1)^j \sum_i u(s_{ij})v(xt_{i,r-j}) \right)
$$

On a encore $\sum_{0 \leq j \leq r} (\sum_i u(xs_{ij})v(t_{i,r-j})) = \langle (u \llcorner x)v, y \rangle$. D’autre part, on a $u(s_{ij}) = 0$ sauf si $j = -p$, donc on peut aussi écrire

$$
\sum_{0 \leq j \leq r} (-1)^j (\sum_i u(s_{ij})v(xt_{i,r-j})) = (-1)^p \langle u(v \llcorner x), y \rangle.
$$

On conclut donc que l’on a

(65)
$$
(i(x))(uv) = ((i(x))(u))v + (-1)^p u((i(x))(v)),
$$

autrement dit $i(x)$ est une *antidérivation* dans $E^{*\mathrm{gr}}$. On prouve de même les assertions relatives au produit intérieur gauche par un élément $x$ de degré 1 dans E.

#### Remarque 1 {#alg-iii-s11-n8-rem-1 .statement}

Soient E une bigèbre graduée sur A et N, N', N'' trois A-modules gradués. Soit m une application A-bilinéaire de N × N' dans N''; pour u ∈ Homgr_A(E, N) et v ∈ Homgr_A(E, N'), notons u . v l’homomorphisme gradué m ◦ (u ⊗ v) ◦ c de E dans N''. D’autre part, notons i(x) le produit intérieur (droit ou gauche) par x ∈ E dans les A-modules Homgr_A(E, N), Homgr_A(E, N') et Homgr_A(E, N'') (III, p. 156). Alors, si x est de degré 1, on a

$$(i(x))(u . v) = ((i(x))(u)).v + u.((i(x))(v))$$

quels que soient u ∈ Homgr_A(E, N) et v ∈ Homgr_A(E, N').

Dans les mêmes conditions, si E est une bigèbre graduée gauche et si u est homogène de degré p, on a

$$(i(x))(u . v) = ((i(x))(u)).v + (-1)^p u.((i(x))(v)).$$

Les démonstrations sont les mêmes que dans la prop. 9.

#### Remarque 2 {#alg-iii-s11-n8-rem-2 .statement}

Le même raisonnement que dans la démonstration précédente prouve, plus généralement, que pour tout x ∈ E, si c(x) = $\sum_j x'_j \otimes x''_j$, on a, quels que soient u, v dans E*gr, la « formule de Leibniz »

$$(i(x))(uv) = \sum_j (i(x'_j))(u).(i(x''_j))(v).$$

En particulier, pour tout élément primitif d’une bigèbre graduée E, c’est-à-dire tel que c(x) = x ⊗ 1 + 1 ⊗ x, i(x) est une dérivation de E*gr.

#### Proposition 10 {#alg-iii-s11-prop-10 .statement}

Soit E une bigèbre graduée (resp. une bigèbre graduée gauche). Pour tout élément f de degré 1 dans E*gr, les produits intérieurs gauche et droit par f sont des dérivations (resp. des antidérivations) de l’algèbre E.

Soient x ∈ E_p, y ∈ E_q (p ≥ 1, q ≥ 1). En vertu de la prop. 5 de III, p. 147, on peut écrire

$$c(x) = x \otimes 1 + \sum_{1 \leq j \leq p-1} (\sum_i x'_{ij} \otimes x''_{i,p-j}) + 1 \otimes x$$
$$c(y) = y \otimes 1 + \sum_{1 \leq k \leq q-1} (\sum_i y'_{ik} \otimes y''_{i,q-k}) + 1 \otimes y$$

où x'_{ij} et x''_{ij} appartiennent à E_j, y'_{ik} et y''_{ik} à E_k. Si E est une bigèbre graduée, la composante de c(xy) = c(x)c(y) appartenant à E_1 ⊗ E, est égale à

$$\sum_i x'_{i,1} \otimes x''_{i,p-1}y + \sum_i y'_{i,1} \otimes xy''_{i,q-1}$$

donc on a par définition

$$(xy) \leftarrow f = \sum_i f(x'_{i,1})x''_{i,p-1}y + \sum_i f(y'_{i,1})xy''_{i,q-1}$$
$$(x \leftarrow f)y + x(y \leftarrow f)$$

et le produit intérieur droit par $f$ est bien une *dérivation*. Si au contraire E est une bigèbre graduée gauche, la composante de $c(xy)$ appartenant à $E_1 \otimes E$ est égale à
$$
\sum_i x_{i,1}' \otimes x_{i,p-1}'' y + (-1)^p \sum_i y_{i,1}' \otimes xy_{i,q-1}'
$$
et on obtient cette fois
$$
(xy) \lrcorner f = (x \lrcorner f)y + (-1)^p x(y \lrcorner f)
$$
ce qui montre que $i(f)$ est alors une *antidérivation*. On raisonne de même pour le produit intérieur gauche par $f$.

#### Exemple {#alg-iii-s11-n8-exa-1 .statement}

Les prop. 9 et 10 s’appliquent en particulier à la bigèbre graduée $S(M)$ et à la bigèbre graduée gauche $\wedge(M)$. Les produits intérieurs par des éléments de degré 1 de $S(M)$ (resp. $S(M)^{*gr}$) sont des *dérivations* qui *commutent deux à deux*, puisque $S(M)$ (resp. $S(M)^{*gr}$) est commutative.

De même, les produits intérieurs par des éléments de degré 1 de $\wedge(M)$ (resp. $\wedge(M)^{*gr}$) sont des *antidérivations*, qui sont de *carré nul*, car le carré d’un élément de degré 1 de l’algèbre $\wedge(M)$ (resp. $\wedge(M)^{*gr}$) est nul.

### 9. Produits intérieurs entre $T(M)$ et $T(M^*)$, $S(M)$ et $S(M^*)$, $\wedge(M)$ et $\wedge(M^*)$

Le produit intérieur droit définit sur $T(M)$ (resp. $S(M)$, resp. $\wedge(M)$) une structure de module à droite sur l’algèbre $T(M)^{*gr}$ (resp. $S(M)^{*gr}$, resp. $\wedge(M)^{*gr}$) (III, p. 161, *Exemples*). Utilisant les homomorphismes canoniques $\theta_T$ (resp. $\theta_S$, resp. $\theta_\wedge$) de III, p. 151, on en déduit
une structure de $T(M^*)$-module à droite sur $T(M)$
une structure de $S(M^*)$-module à droite sur $S(M)$
une structure de $\wedge(M^*)$-module à gauche sur $\wedge(M)$.

On notera encore $(z^*, t) \mapsto i(z^*) . t$ (par abus de langage) la loi d’action d’une quelconque de ces structures; on écrira aussi $t \lrcorner z^*$ au lieu de $i(z^*) . t$ lorsqu’il s’agit de $T(M)$ ou de $S(M)$; par contre, on écrira $z^* \lrcorner t$ lorsqu’il s’agit de $\wedge(M)$, et on dira qu’on a un produit intérieur *gauche* de $t$ par $z^*$, puisqu’on a alors une loi de $\wedge(M^*)$-module *à gauche*. Pour $z^*$ homogène de degré $n$ et $t$ homogène de degré $p$, on a $i(z^*) . t = 0$ si $p < n$, et, pour $x_i \in M$ ($1 \leq i \leq p$), $x_j^* \in M^*$ ($1 \leq j \leq n$) et $p \geq n$, on a, en vertu des formules (58), (59) et (60) de III, p. 162,

$$
\begin{align}
(66)\quad i(x_1^* \otimes x_2^* \otimes \cdots \otimes x_n^*) . (x_1 \otimes x_2 \otimes \cdots \otimes x_p) \\
&= \left( \prod_{j=1}^n \langle x_j^*, x_j \rangle \right) x_{n+1} \otimes \cdots \otimes x_p
\end{align}
$$

$$
\begin{align}
(67)\quad i(x_1^* x_2^* \cdots x_n^*) . (x_1 x_2 \cdots x_p) &= \sum_{\sigma} \left( \prod_{j=1}^n \langle x_j^*, x_{\sigma(j)} \rangle \right) x_{\sigma(n+1)} \cdots x_{\sigma(p)}
\end{align}
$$

(68) $$
i(x_1^* \wedge x_2^* \wedge \cdots \wedge x_n^*) \cdot (x_1 \wedge x_2 \wedge \cdots \wedge x_p)
= (-1)^{n(n-1)/2} \sum_{\sigma} \varepsilon_{\sigma} \left( \prod_{j=1}^n \langle x_j^*, x_{\sigma(j)} \rangle \right) x_{\sigma(n+1)} \wedge \cdots \wedge x_{\sigma(p)}
$$
où, dans les formules (67) et (68), $\sigma$ parcourt l’ensemble des permutations $\sigma \in \mathfrak{S}_p$ qui sont *croissantes* dans les intervalles $\{1, n\}$ et $\{n + 1, p\}$.

On peut encore écrire, avec les notations de produit intérieur,
$$
\begin{aligned}
\langle t \mathbin{\&} u^*, v^* \rangle &= \langle t, \theta_T(u^*v^*) \rangle &\text{pour } t \in T(M), u^*, v^* \text{ dans } T(M^*) \\
\langle t \mathbin{\&} u^*, v^* \rangle &= \langle t, \theta_S(u^*v^*) \rangle &\text{pour } t \in S(M), u^*, v^* \text{ dans } S(M^*) \\
\langle v^*, u^* \mathbin{\&} t \rangle &= \langle \theta_{\wedge}(u^* \wedge v^*), t \rangle &\text{pour } t \in \wedge(M), u^*, v^* \text{ dans } \wedge(M^*).
\end{aligned}
$$

Nous laissons au lecteur le soin d’expliciter les formules analogues pour les produits intérieurs gauches, utilisant cette fois les formules (61), (62) et (63) de III, p. 162.

On peut appliquer ce qui précède en remplaçant $M$ par son dual $M^*$; il faut alors remplacer $M^*$ par le bidual $M^{**}$ et $T(M^*)$, par exemple, est ainsi muni d’une structure de module à droite sur l’algèbre $T(M^{**})$. Mais l’application canonique $c_M : M \to M^{**}$ définit un homomorphisme d’algèbres $T(c_M) : T(M) \to T(M^{**})$, au moyen duquel $T(M^*)$ est muni d’une structure de $T(M)$-module *à droite*. On munit de même $S(M^*)$ (resp. $\wedge(M^*)$) d’une structure de $S(M)$-module *à droite* (resp. $\wedge(M)$-module *à gauche*). Les formules explicites donnant les lois externes de ces modules se déduisent aussitôt des précédentes en y échangeant les rôles de $M$ et de $M^*$. On remarquera que, pour tout $x \in M$, $i(x)$ est toujours une *dérivation* (resp. une *antidérivation de carré nul*) de l’algèbre graduée $S(M^*)$ (resp. $\wedge(M^*)$).

#### Proposition 11 {#alg-iii-s11-prop-11 .statement}

*L’homomorphisme canonique* $\theta_T : T(M^*) \to T(M)^{*gr}$ (resp. $\theta_S : S(M^*) \to S(M)^{*gr}$, resp. $\theta_{\wedge} : \wedge(M^*) \to \wedge(M)^{*gr}$) *est un homomorphisme de* $T(M)$-modules *à droite* (resp. *de* $S(M)$-modules *à droite*, resp. *de* $\wedge(M)$-modules *à gauche*).

Montrons en premier lieu que, pour $z^* \in T(M^*)$ et $t \in T(M)$, on a
$$
\theta_T(z^* \mathbin{\&} t) = \theta_T(z^*) \mathbin{\&} t.
$$
Puisque $M$ est un système générateur de l’algèbre $T(M)$, on peut se borner à prouver (69) lorsque $t = x \in M$; on peut en outre se borner au cas où $z^* = x_1^* \otimes x_2^* \otimes \cdots \otimes x_p^*$, avec les $x_j^* \in M^*$, et on a alors, d’après (66) (III, p. 165) où on a interverti les rôles de $M$ et $M^*$, $z^* \mathbin{\&} x = \langle x, x_1^* \rangle x_2^* \otimes \cdots \otimes x_p^*$. Par suite, quels que soient $y_2, \ldots, y_p$ dans $M$, on a
$$
\begin{aligned}
\langle \theta_T(z^* \mathbin{\&} x), y_2 \otimes y_3 \otimes \cdots \otimes y_p \rangle &= \langle x, x_1^* \rangle \prod_{j=2}^p \langle y_j, x_j^* \rangle \\
&= \langle \theta_T(z^*), x \otimes y_2 \otimes \cdots \otimes y_p \rangle = \langle \theta_T(z^*) \mathbin{\&} x, y_2 \otimes \cdots \otimes y_p \rangle
\end{aligned}
$$
d’où (69).

Prouvons en second lieu que pour $z^* \in S(M^*)$ et $t \in S(M)$, on a
$$
\theta_S(z^* \sqcup t) = \theta_S(z^*) \sqcup t.
$$
Comme ci-dessus, on peut se limiter au cas où $t = x \in M$. Mais en outre, ici $i(x)$ est une *dérivation* de $S(M^*)$ et une *dérivation* de $S(M)^{*gr}$. Par suite (III, p. 126, corollaire), il suffit de vérifier (70) pour $z^* = x^* \in M^*$, puisque $M^*$ est un système générateur de $S(M^*)$; mais cela est trivial, les deux membres étant alors égaux à $\langle x^*, x \rangle$. On raisonne de même pour prouver la relation
$$
\theta_\wedge(t \sqcup z^*) = t \sqcup \theta_\wedge(z^*)
$$
pour $z^* \in \wedge(M^*)$ et $t \in \wedge(M)$: on observe alors que pour $x \in M$, $i(x)$ est une *antidérivation* aussi bien dans $\wedge(M^*)$ que dans $\wedge(M)^{*gr}$ et on utilise III, p. 126, corollaire. On a un résultat analogue pour les produits intérieurs gauches.

### 10. Explication des produits intérieurs dans le cas d’un module libre de type fini

Soient $M$ un A-module libre de type fini, $(e_i)_{1 \leq i \leq n}$ une base de $M$, $(e_i^*)_{1 \leq i \leq n}$ la base duale de $M^*$. Pour toute suite finie $s = (i_1, \ldots, i_p)$ d’éléments de $\{1, n\}$, posons $e_s = e_{i_1} \otimes e_{i_2} \otimes \cdots \otimes e_{i_p}$ (resp. $e_s^* = e_{i_1}^* \otimes \cdots \otimes e_{i_p}^*$). On sait (III, p. 62, th. 1) que les $e_s$ forment une *base* du A-module $T(M)$ et les $e_s^*$ une *base* du A-module $T(M^*)$. Si $s, t$ sont deux suites finies d’éléments de $\{1, n\}$, nous noterons $s.t$ la suite obtenue de la façon suivante: si $s = (i_1, \ldots, i_p)$ et $t = (j_1, \ldots, j_q)$, $s.t$ est la suite $(i_1, \ldots, i_p, j_1, \ldots, j_q)$ à $p + q$ termes. On a donc $e_{s.t} = e_s \otimes e_t$. Il résulte alors de (66) que l’on a
$$
\begin{cases}
e_s \sqcup e_t^* = 0 & \text{si } s \text{ n’est pas de la forme } t.u \\
e_{t.u} \sqcup e_t^* = e_u
\end{cases}
$$

De même, l’algèbre symétrique $S(M)$ a pour base l’ensemble des monômes $e^\alpha$ pour $\alpha \in \mathbf{N}^n$ (III, p. 75, th. 1), et $S(M^*)$ l’ensemble des monômes $e^{*\alpha}$ pour $\alpha \in \mathbf{N}^n$; rappelons (III, p. 155) que l’on note $u_\alpha$, pour $|\alpha| = k$, les éléments de la base de $(S^k(M))^*$, duale de la base $(e^\alpha)_{|\alpha|=k}$ de $S^k(M)$; les $u_\alpha$, pour $\alpha \in \mathbf{N}^n$, forment donc une base de $S(M)^{*gr}$. La définition du produit intérieur droit par $e^\beta$ dans $S(M)^{*gr}$ comme transposée de la multiplication par $e^\beta$ dans $S(M)$ montre alors que l’on a
$$
\begin{cases}
u_\alpha \sqcup e^\beta = 0 & \text{si } \alpha \not\geq \beta \\
u_\alpha \sqcup e^\beta = u_{\alpha-\beta} & \text{si } \alpha \geq \beta
\end{cases}
$$

De même, puisque $S(M)$ s’identifie ici canoniquement au dual gradué de $S(M)^{*gr}$, $i(u_\beta)$ est le transposé gradué de la multiplication par $u_\beta$ dans $S(M)^{*gr}$, donc on déduit de la table de multiplication (33) (III, p. 155) de la base $(u_\alpha)$ que l’on a
$$
\begin{cases}
e^\alpha \sqcup u_\beta = 0 & \text{si } \alpha \not\geq \beta \\
e^\alpha \sqcup u_\beta = ((\beta, \alpha - \beta)) e^{\alpha-\beta} & \text{si } \alpha \geq \beta
\end{cases}
$$

Quant au produit intérieur droit d’un élément de $S(M)$ par un élément de $S(M^*)$, la définition de ce produit (III, p. 165) et la formule (34) de III, p. 155 permettent de déduire de (74) les formules

$$
(75)
\begin{cases}
e^\alpha \mathbin{\&} e^{*\beta} = 0 & \text{si } \alpha \not\geq \beta \\
e^\alpha \mathbin{\&} e^{*\beta} = \frac{\alpha!}{(\alpha - \beta)!} e^{\alpha-\beta} & \text{si } \alpha \geq \beta.
\end{cases}
$$

On a des formules analogues pour le produit intérieur d’un élément de $S(M^*)$ par un élément de $S(M)$ en échangeant les rôles de $M$ et $M^*$ (puisque $M^{**}$ s’identifie ici à $M$).

#### Remarque {#alg-iii-s11-n10-rem-1 .statement}

La donnée de la base $(e_i)_{1 \leq i \leq n}$ permet d’identifier l’algèbre $S(M)$ à l’algèbre de polynômes $A[X_1, \ldots, X_n]$ (III, p. 75); la formule (75) montre que le produit intérieur par $e^{*\alpha}$ n’est autre que l’opérateur différentiel $D^\alpha = D_1^{\alpha_1} D_2^{\alpha_2} \ldots D_n^{\alpha_n}$, où $D_i = \partial / \partial X_i$ pour $1 \leq i \leq n$ (III, p. 134, Exemple).

Considérons enfin l’algèbre extérieure $\wedge(M)$, qui a pour base l’ensemble des éléments $e_J$, où $J$ parcourt l’ensemble des parties de l’intervalle $\{1, n\}$ de $\mathbf{N}$ (III, p. 86, th. 1); de même $\wedge(M^*)$ a pour base les éléments $e_J^*$. Il résulte de la formule (68) de III, p. 166 que l’on a

$$
(76)
\begin{cases}
e_K^* \mathbin{\&} e_J = 0 & \text{si } K \notin J \\
e_K^* \mathbin{\&} e_J = (-1)^{p(p-1)/2} \rho_{K, J-K} e_{J-K} & \text{si } K \subset J \text{ et } p = \operatorname{Card}(K),
\end{cases}
$$

$\rho_{K, J-K}$ étant le nombre défini par la formule (19) de III, p. 87. On a des formules analogues en échangeant les rôles de $M$ et $M^*$.

### 11. Isomorphismes entre $\wedge^p(M)$ et $\wedge^{n-p}(M^*)$ pour un module libre $M$ de dimension $n$

#### Proposition 12 {#alg-iii-s11-prop-12 .statement}

Soit $M$ un $A$-module libre de dimension $n$; soit $e \in \wedge^n(M)$ un élément formant une base de $\wedge^n(M)$, et soit $e^*$ l’élément de $\wedge^n(M^*)$ tel que $\{(-1)^{n(n-1)/2} \theta_{\wedge}(e^*)\}$ soit la base duale de $\{e\}$ dans $(\wedge^n(M))^*$. Soit $\varphi : \wedge(M^*) \to \wedge(M)$ l’application $z \mapsto z \mathbin{\&} e^*$, et $\varphi' : \wedge(M^*) \to \wedge(M)$ l’application $z^* \mapsto z^* \mathbin{\&} e$. Soit $\varphi_p$ (resp. $\varphi'_p$) la restriction de $\varphi$ (resp. $\varphi'$) à $\wedge^p(M)$ (resp. $\wedge^p(M^*)$). Alors:

(i) L’application $\varphi$ est un isomorphisme de $\wedge(M)$-modules à gauche, et l’application $\varphi'$ un isomorphisme de $\wedge(M^*)$-modules à gauche; en outre les applications $\varphi$ et $\varphi'$ sont réciproques l’une de l’autre.

(ii) L’application $\varphi_p$ est un isomorphisme du $A$-module $\wedge^p(M)$ sur le $A$-module $\wedge^{n-p}(M^*)$ et l’application $\varphi'_p$ est un isomorphisme du $A$-module $\wedge^p(M^*)$ sur le $A$-module $\wedge^{n-p}(M)$.

(iii) Si l’on pose $B(u, v^*) = \langle u, \theta_{\wedge}(v^*) \rangle$ pour $u \in \wedge(M)$ et $v^* \in \wedge(M^*)$, on a, pour $u^* \in \wedge^p(M^*)$ et $v^* \in \wedge^{n-p}(M^*)$,

$$
(77) \quad B(\varphi'_p(u^*), v^*) = (-1)^{p(n-p)} B(u^*, \varphi'_{n-p}(v^*)).
$$

Le fait que $\varphi$ soit $\wedge(M)$-linéaire et que $\varphi'$ soit $\wedge(M^*)$-linéaire résulte des formules $(u \wedge v) \lrcorner e^* = u \lrcorner (v \lrcorner e^*)$ et $(u^* \wedge v^*) \lrcorner e = u^* \lrcorner (v^* \lrcorner e)$ (III, p. 157, formule (37)), compte tenu de ce que $\theta_\wedge$ est un isomorphisme de $\wedge(M^*)$ sur l’algèbre opposée à $\wedge(M)^*$). Il existe d’autre part une base $(e_i)_{1 \leq i \leq n}$ de $M$ telle que $e = e_1 \wedge e_2 \wedge \cdots \wedge e_n$ et $e^* = (-1)^{n(n-1)/2} e_1^* \wedge e_2^* \wedge \cdots \wedge e_n^*$, où $(e_i^*)$ est la base duale de $(e_i)$. Posons $I = \{1, n\}$; il résulte de (76) (III, p. 168) que l’on a, pour toute partie $J$ de $I$ à $p$ éléments

$$
\begin{cases}
\varphi(e_J) = (-1)^{\frac{n(n-1)}{2} + \frac{p(p-1)}{2}} \rho_{J, I-J} e_I^* \\
\varphi'(e_J^*) = (-1)^{p(p-1)/2} \rho_{J, I-J} e_I
\end{cases}
$$

Ceci prouve que $\varphi$ et $\varphi'$ sont bijectives; en outre, on a $\rho_{J, I-J} \rho_{I-J, J} = (-1)^{p(n-p)}$ (III, p. 87, formule (21)); comme le nombre

$$
\frac{n(n-1)}{2} + \frac{p(p-1)}{2} + \frac{(n-p)(n-p-1)}{2} + p(n-p) = n(n-1)
$$

est *pair*, on en conclut que $\varphi$ et $\varphi'$ sont réciproques l’une de l’autre. Enfin, pour prouver (77), il suffit de prendre $u^* = e_j^*$ et $v^* = e_{I-J}^*$; la vérification résulte encore de la définition de $\theta_\wedge$, des formules (78) et de la relation $\rho_{J, I-J} \rho_{I-J, J} = (-1)^{p(n-p)}$ (III, p. 87, formule (21)). On notera que pour $u^* \in \wedge^p(M^*)$ et $v^* \in \wedge^{n-p}(M^*)$, $B(\varphi_p(u^*), v^*)$ est, au signe près, le coefficient de $u^* \wedge v^*$ par rapport à la base $\{e^*\}$ de $\wedge^n(M^*)$.

#### Proposition 13 {#alg-iii-s11-prop-13 .statement}

*Avec les hypothèses et notations de la prop. 11, on a, pour tout endomorphisme g du A-module M*

$$
(\det g)\varphi = \wedge({}^t g) \circ \varphi \circ \wedge(g).
$$

Il est clair que l’on a $\wedge({}^t g) = \theta_\wedge^{-1} \circ ({}^t \wedge(g)) \circ \theta_\wedge$; puisque $\wedge(g)$ est un endomorphisme de l’algèbre $\wedge(M)$, et que par définition, on a, pour tout $z \in \wedge(M)$,
$\theta_\wedge(\wedge(g)(z) \lrcorner e^*) = \theta_\wedge(e^*) \llcorner \theta_\wedge(\wedge(g)(z))$, on déduit de la formule (42) de III, p. 158 que

$$
((\theta_\wedge^{-1} \circ ({}^t \wedge(g)) \circ \theta_\wedge) \circ \varphi \circ \wedge(g))(z) = \theta_\wedge^{-1}({}^t \wedge(g)(\theta_\wedge(e^*)) \llcorner z)
= z \lrcorner (\wedge({}^t g)(e^*)) = (\det g)(z \lrcorner e^*) = (\det g)\varphi(z)
$$

compte tenu de III, p. 95, prop. 8.

#### Corollaire {#alg-iii-s11-n11-cor-1 .statement}

*Pour tout automorphisme g de E, on a*

$$
\wedge({}^t g^{-1}) = (\det g)^{-1}\varphi \circ (\wedge(g)) \circ \varphi^{-1}
$$

### 12. Application au sous-espace associé à un p-vecteur

Soient $K$ un corps, $E$ un espace vectoriel sur $K$. Rappelons qu’à tout $p$-vecteur $z \in \wedge^p(E)$ on associe un sous-espace $M_z$ de $E$, de dimension finie, à savoir le plus petit sous-espace vectoriel $M$ de $E$ tel que $z \in \wedge^p(M)$ (III, p. 79, corollaire).

#### Proposition 14 {#alg-iii-s11-prop-14 .statement}

(i) *L’orthogonal de $M_z$ dans $E^*$ est l’ensemble des $x^* \in E^*$ tels que $x^* \perp z = 0$.*

(ii) *Le sous-espace $M_z$ associé à $z$ est l’image de $\wedge^{p-1}(E^*)$ par l’application $\lambda_z$: $u^* \mapsto u^* \perp z$ de $\wedge^{p-1}(E^*)$ dans $E$.*

Notons $N$ l’image de $\lambda_z$. Pour $x^* \in E^*$ et $u^* \in \wedge^{p-1}(E^*)$, on a
$$
\langle \theta_\wedge(x^*), u^* \perp z \rangle = \langle \theta_\wedge(u^* \wedge x^*), z \rangle = (-1)^{p-1} \langle \theta_\wedge(x^* \wedge u^*), z \rangle \\
= (-1)^{p-1} \langle \theta_\wedge(u^*), x^* \perp z \rangle.
$$
Par suite, pour que $x^*$ soit orthogonal à $N$, il faut et il suffit que $x^* \perp z$ soit orthogonal à $\theta_\wedge(\wedge(E^*))$. Or, cette dernière condition équivaut à dire que $x^* \perp z = 0$; en effet, soit $(e_\lambda)_{\lambda \in L}$ une base de $E$; en munissant $L$ d’une structure d’ordre total, on a vu (III, p. 86, th. 1) que les $e_J$, pour $J$ parcourant l’ensemble $\mathcal{F}(L)$ des parties finies de $L$, forment une base de $\wedge(E)$; il résulte alors de la formule (30) de III, p. 153 que les éléments $\theta_\wedge(e_J^*)$ sont, au signe près, les formes coordonnées sur $\wedge(E)$ relatives à la base $(e_J)$; d’où notre assertion.

L’orthogonal de $N$ est donc formé des $x^* \in E^*$ tels que $x^* \perp z = 0$ et la conclusion de (i) résultera donc de (ii).

Montrons d’abord que $N \subset M_z$. En effet, soit $M$ un sous-espace vectoriel de $E$ tel que $z \in \wedge(M)$, et soit $j : M \to E$ l’injection canonique; notons $\mu_z$ l’application $v^* \mapsto v^* \perp z$ de $\wedge^{p-1}(M^*)$ dans $M$; il résulte de la formule (60) de III, p. 162 que l’on a une factorisation canonique
$$
\lambda_z : \wedge^{p-1}(E^*) \xrightarrow{\wedge^{p-1}(t_j)} \wedge^{p-1}(M^*) \xrightarrow{\mu_z} M \xrightarrow{j} E
$$
ce qui prouve que $N \subset M$, donc $N \subset M_z$ par définition de $M_z$. Il reste à voir que $N = M_z$. Supposons le contraire: il existerait alors une base $(e_i)_{1 \leq i \leq n}$ de $M_z$ et un élément $x^* \in E^*$ tel que $\langle x^*, e_1 \rangle = 1, \langle x^*, e_j \rangle = 0$ pour $2 \leq j \leq n$, et tel que $x^*$ soit orthogonal à $N$, donc $x^* \perp z = 0$. Posons $z = \sum_H a_H e_H$, où la somme est étendue aux parties à $p$ éléments de $\{1, n\}$. En vertu de (68) (III, p. 166), on a
$$
\begin{align*}
x^* \perp e_H &= 0 & \text{si } 1 \notin H \\
x^* \perp e_{\{1\} \cup H} &= e_H & \text{si } H \subset \{2, n\}
\end{align*}
$$
ce qui montre que la relation $x^* \perp z = 0$ entraîne $a_H = 0$ pour $1 \in H$. Mais ceci est impossible, car $z$ appartiendrait alors à $\wedge^p(M')$, où $M'$ est le sous-espace de $M$ engendré par $e_2, \ldots, e_n$.

### 13. *p*-vecteurs purs. Grassmanniennes

Soient $K$ un corps, $E$ un espace vectoriel sur $K$. On dit qu’un *p*-vecteur $z \in \wedge^p(E)$ est *pur* (ou parfois *décomposable*) s’il est non nul et s’il existe des vecteurs $x_1, \ldots, x_p$ dans $E$ tels que $z = x_1 \wedge x_2 \wedge \cdots \wedge x_p$. Pour cela, il faut et il suffit que le sous-espace $M_z$ associé à $z$ (qui est toujours de dimension $\geq p$ pour $z \neq 0$) soit exactement de dimension $p$ (puisque $\wedge^p(M_z)$ est alors de dimension 1). En particulier, tout scalaire non nul, tout élément non nul de $E = \wedge^1(E)$, tout élément non nul de $\wedge^n(E)$ lorsque $E$ est de dimension $n$, est pur.

#### Proposition 15 {#alg-iii-s11-prop-15 .statement}

Soit $E$ un espace vectoriel de dimension $n$, et soit $e$ un élément $\neq 0$ de $\wedge^p(E)$ (formant donc une base de cet espace vectoriel). Soit $\varphi : \wedge(E) \to \wedge(E^*)$ l’isomorphisme d’espaces vectoriels associé à $e$ (III, p. 168, prop. 12). Si $z$ est un élément pur de $\wedge^p(E)$, alors $\varphi(z)$ est un élément pur de $\wedge^{n-p}(E^*)$, et les sous-espaces associés à $z$ et à $\varphi(z)$ sont orthogonaux.

Les cas $p = 0$ et $p = n$ sont triviaux. Supposons donc $1 \leq p \leq n - 1$ et soit $z = x_1 \wedge \cdots \wedge x_p \neq 0$. Il existe alors une base $(e_i)_{1 \leq i \leq n}$ de $E$ telle que $e_i = x_i$ pour $1 \leq i \leq p$, et $e = e_1 \wedge e_2 \wedge \cdots \wedge e_n$. On conclut alors de la formule (78) de III, p. 169 que l’on a $\varphi(z) = \pm e_{p+1}^* \wedge \cdots \wedge e_n^*$, d’où la proposition.

#### Corollaire {#alg-iii-s11-n13-cor-1 .statement}

Si $E$ est de dimension $n$, tout $(n-1)$-vecteur non nul sur $E$ est pur.

#### Proposition 16 {#alg-iii-s11-prop-16 .statement}

Pour qu’un élément $z \neq 0$ de $\wedge^p(E)$ soit pur, il faut et il suffit que l’on ait, pour tout $u^* \in \wedge^{p-1}(E^*)$

$$(u^* \perp z) \wedge z = 0.$$

Le cas $p = 0$ étant trivial, nous supposerons $p \geq 1$. Si $z = x_1 \wedge \cdots \wedge x_p$, la formule (68) (III, p. 166) avec $n = p - 1$ montre que $u^* \perp z$ est combinaison linéaire des $x_i$ ($1 \leq i \leq p$), d’où (81). Si au contraire le sous-espace $M_z$ associé à $z$ est de dimension $> p$, considérons une base $(e_j)_{1 \leq j \leq n}$ de ce sous-espace, avec $n > p$. Il résulte de la prop. 13 de III, p. 169 que chacun des $e_j$ est de la forme $u^* \perp z$ pour un $u \in \wedge^{p-1}(E^*)$, et la relation (81) entraîne donc $e_j \wedge z = 0$ pour $1 \leq j \leq n$. Il s’en suit que dans l’expression $z = \sum_H a_H e_H$ (où $H$ parcourt l’ensemble des parties à $p$ éléments de $\{1, n\}$) tous les coefficients $a_H$ sont nuls, d’où $z = 0$ contrairement à l’hypothèse.

Le critère de la prop. 16 équivaut à écrire les conditions (81) lorsque $u^*$ parcourt une base de $\wedge^{p-1}(E^*)$. En particulier, supposons que $E$ soit de dimension finie $n$, et soit $(e_i)_{1 \leq i \leq n}$ une base de $E$. Les conditions (81) sont alors équivalentes aux conditions

$$(82-(J, H)) \quad \langle e_J^*, (e_H^* \perp z) \wedge z \rangle = 0$$

quelles que soient les parties $J, H$ de $\{1, n\}$ telles que $\mathrm{Card}(J) = p + 1$ et $\mathrm{Card}(H) = p - 1$. Or, si $I$ et $I'$ sont deux parties à $p$ éléments de $\{1, n\}$, les formules (76) de III, p. 168 et la table de multiplication (20) de III, p. 87 montrent que l’on a $\langle e_J^*, (e_H^* \perp e_I) \wedge e_{I'} \rangle = 0$ sauf s’il existe un $i \in \{1, n\}$ tel que $I - H = \{i\}$, et $J - I' = \{i\}$, auquel cas on a

$$(83) \quad \langle e_J^*, (e_H^* \perp e_I) \wedge e_{I'} \rangle = (-1)^{(p-1)(p-2)/2} \varepsilon_{i, J, H}$$

où $\varepsilon_{i, J, H} = \rho_{\{i\}, H} \rho_{\{i\}, I'}$; on peut encore dire que pour $i \in J \cap \complement H$, $\varepsilon_{i, J, H}$ est égal à +1 si le nombre d’éléments de J qui sont <i et le nombre d’éléments de H qui sont <i ont même parité, et −1 dans le cas contraire.

Il en résulte aussitôt que si l’on pose $z = \sum_I a_I e_I$, où I parcourt l’ensemble des parties à $p$ éléments de $[1, n]$, la relation (82-(J, H)) est équivalente à la relation
(84-(J, H))
$$
\sum_{i \in J \cap G_H} \varepsilon_{i, J, H} a_{J-\{i\}} a_{H \cup \{i\}} = 0.
$$

Les relations (84) sont appelées les relations de Grassmann: ce sont donc des conditions nécessaires et suffisantes (lorsque J décrit l’ensemble des parties à $p + 1$ éléments et H l’ensemble des parties à $p - 1$ éléments de $[1, n]$) pour que l’élément $z \neq 0$ de $\wedge^p(E)$ soit pur.

On notera que les relations (84) ne sont pas indépendantes. Par exemple, pour $n = 4$ et $p = 2$, les relations de Grassmann se réduisent à l’unique relation
(85)
$$
a_{12} a_{34} - a_{13} a_{24} + a_{14} a_{23} = 0.
$$

Soit $D_p(E)$ le sous-ensemble de $\wedge^p(E)$ formé des $p$-vecteurs purs; il est clair que $D_p(E)$ est saturé pour la relation d’équivalence entre $u$ et $v$: «il existe $\lambda \in K^*$ tel que $v = \lambda u$», et que deux éléments $u, v$ de $D_p(E)$ sont équivalents pour cette relation si et seulement si les sous-espaces $M_u$ et $M_v$ de E qui leur sont associés sont les mêmes. On obtient donc ainsi une bijection canonique de l’ensemble des sous-espaces vectoriels de dimension $p$ de E sur l’image $G_p(E)$ de $D_p(E)$ dans l’espace projectif $P(\wedge^p(E))$ associé à $\wedge^p(E)$. Le sous-ensemble $G_p(E)$ de $P(\wedge^p(E))$ s’appelle la grassmannienne d’indice $p$ de l’espace vectoriel E. Lorsque E est de dimension finie et que $(e_i)_{1 \leq i \leq n}$ est une base de E, la grassmannienne d’indice $p$ est l’ensemble des points de $P(\wedge^p(E))$ dont un système de coordonnées homogènes $(a_I)$ (relativement à la base $(e_I)$ de $\wedge^p(E)$) vérifie les relations de Grassmann (84).

Lorsque $E = K^n$, on écrit parfois $G_{n,p}(K)$ au lieu de $G_p(K^n)$, de sorte que $G_{n,1}(K) = P_{n-1}(K)$. L’application $M \mapsto M^o$ qui, à tout sous-espace de dimension $p$ de $E = K^n$ fait correspondre le sous-espace orthogonal dans $E^*$ (identifié à $K^n$ par le choix de la base duale de la base canonique de $K^n$) définit donc une bijection canonique de $G_{n,p}(K)$ sur $G_{n,n-p}(K)$; la prop. 15 de III, p. 171, montre que cette bijection est la restriction à $G_{n,p}(K)$ d’un isomorphisme canonique de l’espace projectif $P(\wedge^p(K^n))$ sur l’espace projectif $P(\wedge^{n-p}(K^n))$.

## EXERCICES {#alg-iii-s11-exercises}

See the [exercises for § 11](exercises/s11/).
