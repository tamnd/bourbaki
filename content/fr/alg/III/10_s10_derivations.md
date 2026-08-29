---
book: alg
book_title: Algebra
chapter: III
chapter_title: ALGÈBRES TENSORIELLES, ALGÈBRES EXTÉRIEURES, ALGÈBRES SYMÉTRIQUES
section: 10
section_title: Dérivations
lang: fr
source: alg-i-iii-fr
book_pages: A III.116-A III.138, A III.196-A III.197
pdf_pages: 0503-0525, 0583-0584
extraction: ocr
subsections:
    - "no": 1
      title: Facteurs de commutation
      page: 116
      pdf_page: 503
    - "no": 2
      title: Définition générale des dérivations
      page: 117
      pdf_page: 504
    - "no": 3
      title: Exemples de dérivations
      page: 119
      pdf_page: 506
    - "no": 4
      title: Composition des dérivations
      page: 119
      pdf_page: 506
    - "no": 5
      title: Dérivations d'une algèbre A dans un A-bimodule
      page: 122
      pdf_page: 509
    - "no": 6
      title: Dérivations d’une algèbre
      page: 124
      pdf_page: 511
    - "no": 7
      title: Propriétés fonctorielles
      page: 125
      pdf_page: 512
    - "no": 8
      title: Relations entre dérivations et homomorphismes d’algèbres
      page: 127
      pdf_page: 514
    - "no": 9
      title: Prolongement de dérivations
      page: 128
      pdf_page: 515
    - "no": 10
      title: 'Problème universel pour les dérivations: cas non commutatif'
      page: 131
      pdf_page: 518
    - "no": 11
      title: 'Problème universel pour les dérivations : cas commutatif'
      page: 133
      pdf_page: 520
    - "no": 12
      title: Propriétés fonctorielles des K-différentielles
      page: 135
      pdf_page: 522
statements: 41
exercises: 5
content_sha256: 5967d5f78522738e08118204b3d8794c1c7b323d7f835110ffde11c6a5076c65
---

## § 10. DÉRIVATIONS

Dans ce paragraphe, et sauf mention expresse du contraire, les algèbres considérées ne sont pas supposées associatives et n’ont pas nécessairement d’élément unité; $K$ désigne un anneau commutatif.

### 1. Facteurs de commutation

Quand dans ce paragraphe, on parlera sans préciser de graduations, il s’agira de graduations de type $\Delta$, où $\Delta$ désigne un groupe commutatif noté additivement. Dans ce paragraphe, on appelle facteur de commutation sur $\Delta$ un facteur de commutation sur $\Delta$ à valeurs dans l’anneau $\mathbf{Z}$ (III, p. 46, déf. 6). Un facteur de commutation sur $\Delta$ s’identifie donc à une application $\varepsilon : (\alpha, \beta) \mapsto \varepsilon_{\alpha\beta} = \varepsilon(\alpha, \beta)$ de $\Delta \times \Delta$ dans le groupe multiplicatif $\{-1, 1\}$ telle que pour $\alpha, \alpha', \beta, \beta'$ dans $\Delta$, on ait
$$
\begin{cases}
\varepsilon(\alpha + \alpha', \beta) = \varepsilon(\alpha, \beta)\varepsilon(\alpha', \beta) \\
\varepsilon(\alpha, \beta + \beta') = \varepsilon(\alpha, \beta)\varepsilon(\alpha, \beta') \\
\varepsilon(\beta, \alpha) = \varepsilon(\alpha, \beta).
\end{cases}
$$
Il en résulte que $\varepsilon(2\alpha, \beta) = \varepsilon(\alpha, 2\beta) = 1$.

Lorsque $\Delta = \mathbf{Z}$, tout facteur de commutation $\varepsilon$ est déterminé par la donnée de $\varepsilon(1, 1)$; il n’y a donc que deux tels facteurs, le premier défini par
$$
\varepsilon(p, q) = 1 \quad \text{pour } p, q \text{ dans } \mathbf{Z}
$$
et le second par
$$
\varepsilon(p, q) = (-1)^{pq} \quad \text{pour } p, q \text{ dans } \mathbf{Z}.
$$

### 2. Définition générale des dérivations

Considérons un anneau commutatif K, six K-modules gradués de type $\Delta : A, A', A'', B, B', B''$, et trois applications K-bilinéaires

$$
\mu : A \times A' \to A'', \quad \lambda_1 : B \times A' \to B'', \quad \lambda_2 : A \times B' \to B''
$$

telles que les applications K-linéaires correspondantes

$$
A \otimes_K A' \to A'', \quad B \otimes_K A' \to B'', \quad A \otimes_K B' \to B''
$$

soient *graduées de degré* 0. On notera simplement $a.a'$ ou même $aa'$ l’image $\mu(a, a')$ pour $a \in A, a' \in A'$, et de même pour les deux autres applications bilinéaires. Le *degré* de $a.a'$ est donc la *somme* des degrés de $a$ et de $a'$.

#### Définition 1 {#alg-iii-s10-def-1 .statement}

*Pour les données précédentes et pour un facteur de commutation $\varepsilon$ sur $\Delta \times \Delta$, on appelle $\varepsilon$-dérivation (ou (K, $\varepsilon$)-dérivation) de degré $\delta \in \Delta$ de (A, A', A'') dans (B, B', B'') un triplet d’applications K-linéaires graduées de degré $\delta$:*

$$
d : A \to B, \quad d' : A' \to B', \quad d'' : A'' \to B''
$$

*telles que, pour tout élément homogène $a \in A$ et tout élément $a' \in A'$ on ait*

(4)
$$
d''(a.a') = (da).a' + \varepsilon_{\delta, \deg(a)} a.(d'a').
$$

Il suffit évidemment, par linéarité, de vérifier la relation (4) lorsque $a$ et $a'$ parcourent des systèmes générateurs respectifs de A et A'.

Il est souvent commode de désigner par la même lettre $d$ les trois applications $d, d', d''$ (ce qu’on peut justifier en notant également $d$ l’application K-linéaire

$$
(a, a', a'') \mapsto (da, d'a', d''a'')
$$

de $A \oplus A' \oplus A''$ dans $B \oplus B' \oplus B''$). La relation (4) s’écrit alors plus simplement

(5)
$$
d(a.a') = (da).a' + \varepsilon_{\delta, \deg(a)} a.(da').
$$

Les $\varepsilon$-dérivations de (A, A', A'') dans (B, B', B'') de degré *donné* forment un sous-K-module du K-module des applications linéaires graduées

$$
\operatorname{Homgr}_K(A \oplus A' \oplus A'', B \oplus B' \oplus B'').
$$

Lorsque $\varepsilon(\alpha, \beta) = 1$ quels que soient $\alpha, \beta$ dans $\Delta$, on dit simplement *dérivation* (ou *K-dérivation*) au lieu de $\varepsilon$-dérivation. Les dérivations forment un sous-K-module de $\operatorname{Hom}_K(A \oplus A' \oplus A'', B \oplus B' \oplus B'')$.

Lorsque $\Delta = \mathbf{Z}$ et $\varepsilon(p, q) = (-1)^{pq}$, toute $\varepsilon$-dérivation de degré *pair* est une dérivation; une $\varepsilon$-dérivation de degré *impair* est souvent appelée *antidérivation* (ou *K-antidérivation*); une antidérivation $d$ satisfait donc à

(6)
$$
d(a.a') = (da).a' + (-1)^{\deg(a)} a.(da')
$$

pour un élément *homogène* $a \in A$.

#### Remarque 1 {#alg-iii-s10-n2-rem-1 .statement}

On peut définir la notion de dérivation pour des modules non gradués, en convenant de munir ces modules de la graduation triviale.

#### Remarque 2 {#alg-iii-s10-n2-rem-2 .statement}

Tant qu’on ne considère que des ε-dérivations d’un degré donné δ, on peut se débarrasser du facteur de commutation ε par le procédé suivant: on modifie l’application bilinéaire $\lambda_2 : A \times B' \to B''$ en la remplaçant par l’application bilinéaire $\lambda'_2 : A \times B' \to B''$ telle que pour tout $a$ homogène dans $A$ et tout $b' \in B'$, on ait

$$
\lambda'_2(a, b') = \varepsilon_{\delta, \deg(a)} \lambda_2(a, b').
$$

Alors $d$ est une dérivation relativement aux applications bilinéaires $\mu, \lambda_1, \lambda'_2$.

La définition générale des ε-dérivations donnée ci-dessus est surtout utilisée dans deux cas:

Cas I): on a $A = B, A' = B', A'' = B''$, et les trois applications bilinéaires $\mu, \lambda_1, \lambda_2$ sont égales à une même application.

Cas II): on a $A = A' = A'', B = B' = B''$, de sorte que (pour $\mu$) $A$ est une algèbre graduée, et que les deux applications K-bilinéaires

(7)
$$
\lambda_1 : B \times A \to B, \quad \lambda_2 : A \times B \to B
$$

sont telles que les applications K-linéaires correspondantes $B \otimes_K A \to B, A \otimes_K B \to B$ soient graduées de degré 0. Une ε-dérivation de degré δ de $A$ dans $B$ est alors une application K-linéaire graduée $d : A \to B$ de degré δ, telle que, pour tout $x$ homogène dans $A$ et tout $y \in A$, on ait la relation

(8)
$$
d(xy) = (dx)y + \varepsilon_{\delta, \deg(x)} x(dy).
$$

Rentre en particulier dans le cas II) le cas où $A$ est une K-algèbre associative unifière, et où $\lambda_1$ et $\lambda_2$ sont les lois d’action d’un (A, A)-bimodule (III, p. 39, déf. 3). Il en est ainsi notamment lorsque $A$ et $B$ sont deux K-algèbres associatives unifières, que l’on s’est donné un homomorphisme unifière de K-algèbres graduées $\rho : A \to B$ et que l’on considère sur $B$ la structure de (A, A)-bimodule définie par les deux lois d’action

$$
\lambda_1 : (b, a) \mapsto b\rho(a), \qquad \lambda_2 : (a, b) \mapsto \rho(a)b
$$

pour $a \in A, b \in B$.

Les cas I) et II) ont en commun le cas suivant: on considère une K-algèbre graduée $A$, on prend $B = A$, les applications (7) étant toutes deux la multiplication dans $A$. On parle alors de ε-dérivation (ou (K, ε)-dérivation) de l’algèbre graduée $A$: c’est une application K-linéaire graduée de $A$ dans elle-même, de degré δ, satisfaisant à (8) pour tout $x$ homogène dans $A$ et tout $y \in A$. En particulier, si $A$ est un anneau gradué, considéré comme une $\mathbf{Z}$-algèbre (associative), on parlera des ε-dérivations de l’anneau $A$.

Soient $A$ une K-algèbre associative, commutative et unifière, $B$ un A-module; lorsqu’on parlera de dérivation de $A$ dans $B$, il sera sous-entendu qu’il s’agit de la structure de A-bimodule de B déduite de sa structure de A-module; on a alors la formule
$$
d(xy) = x(dy) + y(dx)
$$
pour $x \in A, y \in A$
pour une telle dérivation $d : A \to B$.

### 3. Exemples de dérivations

#### Exemple 1 {#alg-iii-s10-n3-exa-1 .statement}

*Soit A la $\mathbf{R}$-algèbre des applications dérivables de $\mathbf{R}$ dans $\mathbf{R}$, et soit $x_0$ un point de $\mathbf{R}$; on peut considérer $\mathbf{R}$ comme A-module pour la loi d’action $(f, a) \mapsto f(x_0)a$. Alors l’application $f \mapsto Df(x_0)$ est une dérivation, puisque l’on a (FVR, I, § 1, no 3) $(D(fg))(x_0) = (Df(x_0))g(x_0) + f(x_0)(Dg(x_0)).*$

#### Exemple 2 {#alg-iii-s10-n3-exa-2 .statement}

*Soit X une variété différentielle de classe $C^\infty$, et soit A la $\mathbf{R}$-algèbre graduée des formes différentielles sur X, L’application qui à toute forme différentielle $\omega$ sur X associe sa différentielle extérieure $d\omega$ est une antidérivation de degré +1 (VAR. R, § 8).*

#### Exemple 3 {#alg-iii-s10-n3-exa-3 .statement}

Soit A une K-algèbre associative. Pour tout $a \in A$, l’application $x \mapsto ax - xa$ est une dérivation de l’algèbre A (cf. III, p. 124).

#### Exemple 4 {#alg-iii-s10-n3-exa-4 .statement}

Soient M un K-module, A l’algèbre extérieure $\wedge(M^*)$, munie de sa graduation usuelle (III, p. 76). *On verra dans III, p. 167 que, pour tout $x \in M$, le produit intérieur droit $i(x)$ est une antidérivation de degré −1 de A.*

#### Exemple 5 {#alg-iii-s10-n3-exa-5 .statement}

Reprenons la situation générale de la déf. 1 de III, p. 117, et soient $\overline{K}$ un second anneau commutatif, $\rho : K \to \overline{K}$ un homomorphisme d’anneaux; désignons par $\overline{A}, \overline{A}', \overline{A}'', \overline{B}, \overline{B}', \overline{B}''$ les $\overline{K}$-modules gradués obtenus respectivement à partir de A, A', A'', B, B', B'' par extension à $\overline{K}$ de l’anneau des scalaires (II, p. 174); on déduit de $\mu, \lambda_1$ et $\lambda_2$ des applications $\overline{K}$-bilinéaires
$$
\bar{\mu} : \overline{A} \times \overline{A}' \to \overline{A}'', \quad \bar{\lambda}_1 : \overline{B} \times \overline{A}' \to \overline{B}'', \quad \bar{\lambda}_2 : \overline{A} \times \overline{B}' \to \overline{B}''
$$
en considérant les produits tensoriels par $1_{\overline{K}}$ des applications K-linéaires correspondant à $\mu, \lambda_1$ et $\lambda_2$ (II, p. 82). Alors, si $d$ est une $\varepsilon$-dérivation de degré $\delta$ de (A, A', A'') dans (B, B', B''), l’application $\bar{d} = d \otimes 1_{\overline{K}}$ de $\overline{A} \oplus \overline{A}' \oplus \overline{A}''$ dans $\overline{B} \oplus \overline{B}' \oplus \overline{B}''$ est une $\varepsilon$-dérivation de degré $\delta$ de ($\overline{A}, \overline{A}', \overline{A}''$) dans ($\overline{B}, \overline{B}', \overline{B}''$).

#### Exemple 6 {#alg-iii-s10-n3-exa-6 .statement}

Soit A une K-algèbre graduée de type $\mathbf{Z}$; on définit une K-application linéaire graduée de degré 0, $d : A \to A$ en prenant, pour $x_n \in A_n$ ($n \in \mathbf{Z}$), $d(x_n) = nx_n$. Cette application est une dérivation de A, car pour $x_p \in A_p, x_q \in A_q$, on a $d(x_p x_q) = (p + q)x_p x_q = d(x_p) x_q + x_p d(x_q)$.

### 4. Composition des dérivations

Nous supposons dans ce n° que l’on se trouve dans le cas I) de III, p. 118, c’est-à-dire que A, A', A'' sont trois K-modules gradués de type $\Delta$, que l’on s’est donné une application K-bilinéaire $\mu : A \times A' \to A''$ correspondant à une application K-linéaire graduée de degré 0, $A \otimes_K A' \to A''$. Les endomorphismes gradués $f$ de $A \oplus A' \oplus A''$ tels que $f(A) \subset A, f(A') \subset A'$ et $f(A'') \subset A''$ forment une sous-algèbre graduée de l’algèbre associative graduée $\mathrm{Endgr}_K(A \oplus A' \oplus A'')$ (III, p. 31, Exemple 2). On peut en particulier composer deux $\varepsilon$-dérivations de $(A, A', A'')$, mais on se gardera de croire que le composé de deux $\varepsilon$-dérivations soit encore une $\varepsilon$-dérivation.

Dans toute algèbre graduée B de type $\Delta$, on définit le $\varepsilon$-crochet (ou simplement crochet lorsque $\varepsilon = 1$) de deux éléments homogènes $u, v$, par la formule

$$
[u, v]_\varepsilon = uv - \varepsilon_{\deg u, \deg v} vu \quad \text{(noté simplement } [u, v] \text{ si } \varepsilon = 1\text{)}.
$$

En prolongeant cette application par linéarité, on obtient une application K-bilinéaire $(u, v) \mapsto [u, v]_\varepsilon$ de $B \times B$ dans $B$. On a, pour $u$ et $v$ homogènes dans $B$

$$
[v, u]_\varepsilon = -\varepsilon_{\deg u, \deg v} [u, v]_\varepsilon.
$$

Appliquons cette définition à l’algèbre graduée $\mathrm{Endgr}_K(A \oplus A' \oplus A'')$ : on définit ainsi le $\varepsilon$-crochet de deux endomorphismes gradués.

#### Proposition 1 {#alg-iii-s10-prop-1 .statement}

*Soient $d_1, d_2$ deux $\varepsilon$-dérivations de $(A, A', A'')$, de degrés respectifs $\delta_1, \delta_2$. Alors le $\varepsilon$-crochet*

$$
[d_1, d_2]_\varepsilon = d_1 \circ d_2 - \varepsilon_{\delta_1, \delta_2} d_2 \circ d_1
$$

*est une $\varepsilon$-dérivation de degré $\delta_1 + \delta_2$. De plus, si $d$ est une $\varepsilon$-dérivation de degré $\delta$ de $(A, A', A'')$, et si $\varepsilon_{\delta, \delta} = -1$, alors $d^2 = d \circ d$ est une dérivation.*

Supposons $x \in A$ homogène de degré $\xi$; pour tout $y \in A'$, on a

$$
d_1(d_2(xy)) = ((d_1 d_2)(x))y + \varepsilon_{\delta_1, \delta_2 + \xi}(d_2 x)(d_1 y)
+ \varepsilon_{\delta_2, \xi}(d_1 x)(d_2 y) + \varepsilon_{\delta_1 + \delta_2, \xi} x((d_1 d_2)(y))
$$

compte tenu des formules (1) de III, p. 116. Echangeant les rôles de $d_1$ et $d_2$, on obtient, après simplifications utilisant de nouveau (1) (III, p. 116),

$$
(d_1 d_2)(xy) - \varepsilon_{\delta_1, \delta_2}(d_2 d_1)(xy) = ((d_1 d_2)(x))y - \varepsilon_{\delta_1, \delta_2}((d_2 d_1)(x))y
+ \varepsilon_{\delta_1 + \delta_2, \xi} x((d_1 d_2)(y)) - \varepsilon_{\delta_1, \delta_2} \varepsilon_{\delta_1 + \delta_2, \xi} x((d_2 d_1)(y))
$$

c’est-à-dire, en posant $d = [d_1, d_2]_\varepsilon$ et $\delta = \delta_1 + \delta_2$,

$$
d(xy) = (dx)y + \varepsilon_{\delta, \xi} x(dy)
$$

ce qui prouve que $d$ est une $\varepsilon$-dérivation.

D’autre part, si, dans (11), on fait $d_1 = d_2 = d, \delta_1 = \delta_2 = \delta$ et si $\varepsilon_{\delta, \delta} = -1$, on obtient, puisqu’alors $\varepsilon_{\delta, \delta + \xi} = -\varepsilon_{\delta, \xi}$ par (1),

$$
d^2(xy) = (d^2 x)y + \varepsilon_{2\delta, \xi} x(d^2 y)
$$

et comme $\varepsilon_{2\delta, \xi} = 1$, on voit que $d^2$ est bien une dérivation.

#### Corollaire {#alg-iii-s10-n4-cor-1 .statement}

Supposons $\Delta = \mathbf{Z}$. Alors:
    (i) Le carré d’une antidérivation est une dérivation.
    (ii) Le crochet de deux dérivations est une dérivation.
    (iii) Le crochet d’une antidérivation et d’une dérivation de degré pair est une antidérivation.
    (iv) Si $d_1$ et $d_2$ sont des antidérivations, $d_1 d_2 + d_2 d_1$ est une dérivation.

Sous les hypothèses du début de ce n° (III, p. 119,) considérons maintenant une suite finie $D = (d_i)_{i \leq i \leq n}$ de dérivations deux à deux permutables de $(A, A', A'')$. Pour tout polynôme $P(X_1, \ldots, X_n)$ de l’algèbre $K[X_1, \ldots, X_n]$, l’élément $P(d_1, \ldots, d_n)$ de $\mathrm{Endgr}_K(A \oplus A' \oplus A'')$ est donc défini (III, p. 26); on le notera en abrégé $P(D)$.

#### Proposition 2 {#alg-iii-s10-prop-2 .statement}

Avec les hypothèses et notations précédentes, considérons $2n$ indéterminées $T_1, \ldots, T_n, T'_1, \ldots, T'_n$, et pour tout polynôme $F \in K[X_1, \ldots, X_n]$, posons $F(T) = F(T_1, \ldots, T_n), F(T') = F(T'_1, \ldots, T'_n)$ et
$$
F(T + T') = F(T_1 + T'_1, \ldots, T_n + T'_n).
$$
Supposons que l’on ait
$$
P(T + T') = \sum_i Q_i(T) R_i(T')
$$
où les $Q_i$ et $R_i$ appartiennent à $K[X_1, \ldots, X_n]$. Alors, quels que soient $x \in A$ et $y \in A'$, on a
$$
(12) \quad P(D)(xy) = \sum_i (Q_i(D)x)(R_i(D)y).
$$

Introduisons $n$ autres indéterminées $T''_1, \ldots, T''_n$, et considérons l’algèbre de polynômes $K[T_1, \ldots, T_n, T'_1, \ldots, T'_n, T''_1, \ldots, T''_n] = B$; considérons d’autre part le $K$-module $M$ des applications bilinéaires de $A \times A'$ dans $A''$; on définit sur $M$ une structure de $B$-module en posant, pour toute application $K$-bilinéaire $f \in M$ et $1 \leq i \leq n$
$$
(13) \quad \begin{cases}
(T_i f)(a, a') = f(d_i a, a') \\
(T'_i f)(a, a') = f(a, d_i a') \\
(T''_i f)(a, a') = d_i(f(a, a'))
\end{cases}
$$

Puisque les $d_i$ sont deux à deux permutables, on voit que pour tout polynôme $F \in K[X_1, \ldots, X_n]$, on a $(F(T)f)(a, a') = f(F(D)a, a'), (F(T')f)(a, a') = f(a, F(D)a')$ et $(F(T'')f)(a, a') = F(D)(f(a, a'))$. Donc, pour prouver (12) il suffit de montrer que l’on a
$$
(14) \quad (P(T'') - \sum_i Q_i(T) R_i(T')) \cdot \mu = 0
$$
ou encore $(P(T'') - P(T + T')) \cdot \mu = 0$ dans le $B$-module $M$. Or, l’hypothèse que les $d_i$ sont des dérivations s'exprime encore en disant que l'on a, pour $1 \leqslant i \leqslant n$

(15) $(\mathrm{T}''_i - \mathrm{T}_i - \mathrm{T}'_i) . \mu = 0$

dans le B-module M. En considérant successivement les polynômes

$$
\begin{aligned}
&\mathrm{P}(\mathrm{T}''_1, \mathrm{T}''_2, \ldots, \mathrm{T}''_n) - \mathrm{P}(\mathrm{T}_1 + \mathrm{T}'_1, \mathrm{T}''_2, \ldots, \mathrm{T}''_n) \\
&\mathrm{P}(\mathrm{T}_1 + \mathrm{T}'_1, \mathrm{T}''_2, \ldots, \mathrm{T}''_n) - \mathrm{P}(\mathrm{T}_1 + \mathrm{T}'_1, \mathrm{T}_2 + \mathrm{T}'_2, \ldots, \mathrm{T}''_n) \\
&\qquad\qquad\qquad\qquad \cdots \\
&\mathrm{P}(\mathrm{T}_1 + \mathrm{T}'_1, \ldots, \mathrm{T}_{n-1} + \mathrm{T}'_{n-1}, \mathrm{T}''_n) - \mathrm{P}(\mathrm{T}_1 + \mathrm{T}'_1, \ldots, \mathrm{T}_{n-1} + \mathrm{T}'_{n-1}, \mathrm{T}_n + \mathrm{T}'_n)
\end{aligned}
$$

on voit que la différence $\mathrm{P}(\mathbf{T}'') - \mathrm{P}(\mathbf{T} + \mathbf{T}')$ s'écrit sous la forme

$$
\sum_{i=1}^{n} (\mathrm{T}''_i - \mathrm{T}_i - \mathrm{T}'_i) \mathrm{G}_i(\mathbf{T}, \mathbf{T}', \mathbf{T}'')
$$

où les $\mathrm{G}_i$ sont des éléments de B. La relation (14) est donc conséquence immédiate des relations (15).

#### Corollaire (formule de Leibniz) {#alg-iii-s10-n4-cor-2 .statement}

Soient $d_i$ ($1 \leqslant i \leqslant n$) $n$ dérivations de $(\mathrm{A}, \mathrm{A}', \mathrm{A}'')$, deux à deux permutables. Pour tout $\alpha = (\alpha_1, \ldots, \alpha_n) \in \mathbf{N}^n$ posons

(16) $d^\alpha = d_1^{\alpha_1} d_2^{\alpha_2} \ldots d_n^{\alpha_n}.$

Alors, pour $x \in \mathrm{A}$ et $y \in \mathrm{A}'$, on a

(17) $d^\alpha(xy) = \sum_{\beta + \gamma = \alpha} ((\beta, \gamma)) d^\beta(x) d^\gamma(y)$

où l'on a posé (avec les notations introduites au début du chapitre)

(18) $((\beta, \gamma)) = (\beta + \gamma)! / (\beta! \gamma!).$

Cela résulte aussitôt de la formule multinomiale (I, p. 95)

$$
(\mathbf{T} + \mathbf{T}')^\alpha = \sum_{\beta + \gamma = \alpha} ((\beta, \gamma)) \mathbf{T}^\beta \mathbf{{T}'}^\gamma
$$

et de la prop. 2.

### 5. Dérivations d'une algèbre A dans un A-bimodule

Nous supposons dans ce n° que l'on se trouve dans le cas II) de III, p. 118. On a donc une K-algèbre graduée A, et un K-module gradué E, ainsi que deux applications K-linéaires de degré 0

$$
\mathrm{E} \otimes_{\mathrm{K}} \mathrm{A} \to \mathrm{E}, \qquad \mathrm{A} \otimes_{\mathrm{K}} \mathrm{E} \to \mathrm{E}
$$

notées

$$
x \otimes a \mapsto x . a \quad \text{et} \quad a \otimes x \mapsto a . x \qquad \text{pour } a \in \mathrm{A} \text{ et } x \in \mathrm{E}.
$$

#### Proposition 3 {#alg-iii-s10-prop-3 .statement}

Soit $d : \mathrm{A} \to \mathrm{E}$ une $\varepsilon$-dérivation de degré $\delta$. Alors $\mathrm{Ker}(d)$ est une sous-algèbre graduée de A; si A admet un élément unité, il appartient à $\mathrm{Ker}(d)$.

Il est clair que $\mathrm{Ker}(d)$ est un sous-K-module gradué de A; de plus, la relation (8) de III, p. 118 montre que, si x et y sont deux éléments homogènes appartenant à Ker(d), on a d(xy) = 0, donc xy ∈ Ker(d). Enfin, si A admet un élément unité 1 (de degré 0, cf. III, p. 30), la relation (8) de III, p. 118, où on remplace x et y par 1, donne d(1) = d(1) + d(1), donc d(1) = 0.

#### Corollaire {#alg-iii-s10-n5-cor-1 .statement}

Soient d₁ et d₂ deux ε-dérivations de A dans E, de même degré δ. Si d₁ et d₂ prennent les mêmes valeurs en chaque élément d’un système générateur de l’algèbre A, on a d₁ = d₂.

En effet, d₁ − d₂ est une ε-dérivation de degré δ, donc Ker(d₁ − d₂) est une sous-algèbre de A qui contient un système générateur de A, donc est égale à A.

#### Proposition 4 {#alg-iii-s10-prop-4 .statement}

Soit d : A → E une ε-dérivation de degré δ. Supposons que A possède un élément unité 1, et soit x un élément homogène de A, ayant un inverse x⁻¹ dans A. Alors on a

$$
d(x^{-1}) = -\varepsilon_{\delta, \deg(x)} x^{-1}((dx)x^{-1}) = -\varepsilon_{\delta, \deg(x)} (x^{-1}(dx))x^{-1}.
$$

En effet, on a d(xx⁻¹) = d(1) = 0 (III, p. 122, prop. 3), d’où

$$(dx)x^{-1} + \varepsilon_{\delta, \deg(x)} x(d(x^{-1})) = 0$$

ce qui prouve la première formule (19). D’autre part, x⁻¹ est homogène de degré −deg(x) et $\varepsilon_{\delta, \deg(x)} = \varepsilon_{\delta, -\deg(x)}$ en vertu des formules (1) de III, p. 116; en écrivant que $d(x^{-1}x) = 0$, on obtient de même la seconde formule (19).

#### Proposition 5 {#alg-iii-s10-prop-5 .statement}

Supposons que A soit un anneau commutatif intègre, et soit L son corps des fractions. Toute dérivation de A dans un espace vectoriel E sur L (considéré comme A-module) se prolonge d’une seule manière en une dérivation de L dans E.

Soient d une dérivation de A dans E, $\overline{d}$ une dérivation de L dans E prolongeant d; alors, pour $u \in A, v \in A, v \neq 0$, on a nécessairement, en vertu de (19)

$$
\overline{d}(u/v) = v^{-1}du - uv^{-2}dv
$$

ce qui prouve l’unicité de $\overline{d}$. Inversement, montrons qu’on peut définir $\overline{d}$ par la formule (20); on doit d’abord vérifier que si $u/v = u'/v'$, la valeur du second membre de (20) ne change pas quand on remplace u par u’ et v par v’. Or, on a $uv' = vu'$, donc $v'(du) + u(dv') = v(du') + u'(dv)$, et par suite $v'(du - uv^{-1}dv) = v(du' - u'{v'}^{-1}dv')$, puisque $uv'v^{-1} = u'$ et $u'{v'}^{-1}v = u$. On a ainsi défini une application $\overline{d} : L \to E$, qui prolonge d; on vérifie aussitôt qu’elle est K-linéaire et est une dérivation.

#### Proposition 6 {#alg-iii-s10-prop-6 .statement}

Supposons que A soit une K-algèbre graduée associative unifère, E un (A, A)-bimodule gradué. Si d : A → E est une ε-dérivation de degré δ, on a, pour toute suite finie $(x_i)_{1 \leq i \leq n}$ d’éléments homogènes de A, de degrés respectifs $\xi_i$ (1 ≤ i ≤ n)

$$
d(x_1 x_2 \ldots x_n) = \sum_{i=1}^n \varepsilon_{\delta, \xi_1 + \ldots + \xi_{i-1}} x_1 \ldots x_{i-1} (dx_i) x_{i+1} \ldots x_n.
$$

La formule (21) est triviale pour $n = 0$ et se prouve par récurrence sur $n$, compte tenu de (4) (III, p. 117).

#### Corollaire {#alg-iii-s10-n5-cor-2 .statement}

Supposons que $A$ soit une algèbre associative unifère, commutative et ayant un élément unité, et $E$ un $A$-module. Si $d : A \to E$ est une dérivation, on $a$, pour tout entier $n \geqslant 0$,

$$
d(x^n) = nx^{n-1}(dx) \quad \text{pour tout } x \in A.
$$

Il suffit de munir $A$ de la graduation triviale et d’appliquer (21) avec tous les $x_i$ égaux à $x$.

Revenons au cas général d’une $\varepsilon$-dérivation $d : A \to E$ de degré $\delta$. Soit $Z_\varepsilon$ l’ensemble des $a \in A$ tels que pour tout composant homogène $a_\alpha$ de degré $\alpha$ de $a$, on ait, pour tout $x$ homogène dans $E$

$$
xa_\alpha = \varepsilon_{\delta, \deg(x)} a_\alpha x.
$$

Si $A$ est une algèbre graduée associative unifère, et $E$ un $(A, A)$-bimodule gradué, il résulte aussitôt de cette définition que $Z_\varepsilon$ est une sous-algèbre graduée de $A$ contenant l’élément unité.

#### Proposition 7 {#alg-iii-s10-prop-7 .statement}

Supposons que $A$ soit une algèbre graduée associative unifère et $E$ un $(A, A)$-bimodule gradué. Soit $d : A \to E$ une $\varepsilon$-dérivation de degré $\delta$, et $a$ un élément homogène de degré $\alpha$ de $Z_\varepsilon$. Alors l’application $x \mapsto a(dx)$ est une $\varepsilon$-dérivation de degré $\delta + \alpha$.

Posons en effet $d'(x) = a(dx)$; pour $x$ homogène de degré $\xi$ dans $A$, et $y \in A$, on a, en vertu de (23) et de (1) (III, p. 116),

$$
\begin{align*}
d'(xy) &= a((dx)y) + \varepsilon_{\delta, \xi} a(x(dy)) = (a(dx))y + \varepsilon_{\delta+\alpha, \xi} (xa)(dy) \\
&= (d'x)y + \varepsilon_{\delta+\alpha, \xi} x(d'y).
\end{align*}
$$

La prop. 7 exprime que le $K$-module des $\varepsilon$-dérivations de $A$ dans $E$ est un $Z_\varepsilon$-module gradué de type $\Delta$.

### 6. Dérivations d’une algèbre

Soit $A$ une $K$-algèbre graduée; pour tout élément homogène $a \in A$, on note $\mathrm{ad}_\varepsilon(a)$, ou simplement $\mathrm{ad}(a)$ si aucune confusion n’en résulte, l’application $K$-linéaire de $A$ dans $A$

$$
x \mapsto [a, x]_\varepsilon
$$

(III, p. 120, formule (10)) qui est graduée de degré $\deg a$.

#### Proposition 8 {#alg-iii-s10-prop-8 .statement}

Soit $A$ une $K$-algèbre graduée.

(i) Pour toute $\varepsilon$-dérivation $d : A \to A$ et tout élément homogène $a$ de $A$, on a

$$
[d, \mathrm{ad}_\varepsilon(a)]_\varepsilon = \mathrm{ad}_\varepsilon(da).
$$

(ii) Si l’algèbre $A$ est associative, $\mathrm{ad}_\varepsilon(a)$ est une $\varepsilon$-dérivation de $A$, de degré $\deg(a)$.

(i) En effet, supposons que $d$ soit de degré $\delta$, soit $\alpha = \deg a$, et posons $f = [d, \mathrm{ad}_\varepsilon(a)]_\varepsilon$. Pour tout élément homogène $x \in A$ de degré $\xi$, on a, compte tenu de (1), (III, p. 116)

$$
f(x) = d(ax - \varepsilon_{\alpha, \xi} xa) - \varepsilon_{\delta, \alpha}(a(dx)) - \varepsilon_{\alpha, \delta+\xi}(dx)a \\
= (da)x + \varepsilon_{\delta, \alpha}a(dx) - \varepsilon_{\alpha, \xi}(dx)a - \varepsilon_{\delta+\alpha, \xi}x(da) \\
- \varepsilon_{\delta, \alpha}a(dx) + \varepsilon_{\alpha, \xi}(dx)a \\
= (da)x - \varepsilon_{\delta+\alpha, \xi}x(da) = [da, x]_\varepsilon.
$$

(ii) Pour tout $x$ homogène de degré $\xi$ et tout $y$ homogène de degré $\eta$ dans $A$, on a

$$
\mathrm{ad}_\varepsilon(a)(xy) = a(xy) - \varepsilon_{\alpha, \xi+\eta}(xy)a \\
= (ax - \varepsilon_{\alpha, \xi}xa)y + \varepsilon_{\alpha, \xi}x(ay - \varepsilon_{\alpha, \eta}ya) \\
= \mathrm{ad}_\varepsilon(a)(x).y + \varepsilon_{\alpha, \xi}x.\mathrm{ad}_\varepsilon(a)(y)
$$

compte tenu de (1) et de l’associativité de $A$.

Lorsque $A$ est associative, on dit que $\mathrm{ad}_\varepsilon(a)$ est la $\varepsilon$-dérivation intérieure de $A$ définie par $a$.

#### Corollaire {#alg-iii-s10-n6-cor-1 .statement}

Soit $A$ une algèbre graduée associative. Pour deux éléments homogènes $a, b$ de $A$, on a

$$(25)$$
$$
[\mathrm{ad}_\varepsilon(a), \mathrm{ad}_\varepsilon(b)]_\varepsilon = \mathrm{ad}_\varepsilon([a, b]_\varepsilon).
$$

Il suffit de remplacer $d$ par $\mathrm{ad}_\varepsilon(a)$ et $\mathrm{ad}_\varepsilon(a)$ par $\mathrm{ad}_\varepsilon(b)$ dans (24).

Si $\deg a = \alpha$, $\deg b = \beta$, la formule (25) équivaut à la relation suivante, pour tout élément homogène $c \in A$ de degré $\gamma$

$$(26)$$
$$
\varepsilon_{\alpha, \gamma}[a, [b, c]_\varepsilon]_\varepsilon + \varepsilon_{\beta, \alpha}[b, [c, a]_\varepsilon]_\varepsilon + \varepsilon_{\gamma, \beta}[c, [a, b]_\varepsilon]_\varepsilon = 0
$$

dite identité de Jacobi.

### 7. Propriétés fonctorielles

Dans ce no, toutes les algèbres sont supposées associatives et unifères, et tout homomorphisme d’algèbres est supposé unifère.

#### Proposition 9 {#alg-iii-s10-prop-9 .statement}

Soient $A, B$ deux $K$-algèbres graduées, $E$ un $(A,A)$-bimodule gradué, $F$ un $(B,B)$-bimodule gradué; soient $\rho : A \to B$ un homomorphisme d’algèbres graduées, $\theta : E \to F$ un $A$-homomorphisme de $A$-bimodules (relatif à $\rho$), gradué et de degré 0. Alors:

(i) Pour toute $\varepsilon$-dérivation $d' : B \to F$, $d' \circ \rho : A \to \rho_*(F)$ est une $\varepsilon$-dérivation de même degré.

(ii) Pour toute $\varepsilon$-dérivation $d : A \to E$, $\theta \circ d : A \to \rho_*(F)$ est une $\varepsilon$-dérivation de même degré.

Les deux assertions découlent aussitôt des relations

$$
d'(\rho(xy)) = d'(\rho(x)\rho(y)) = d'(\rho(x))\rho(y) + \varepsilon_{\delta',\xi}\rho(x)d'(\rho(y))
$$
$$
\theta(d(xy)) = \theta((dx)y + \varepsilon_{\delta,\xi}x(dy)) = \theta(dx)\rho(y) + \varepsilon_{\delta,\xi}\rho(x)\theta(dy)
$$

pour $x \in A$ homogène de degré $\xi$ et $y \in A$, $\delta$ et $\delta'$ désignant les degrés respectifs de $d$ et $d'$.

#### Corollaire {#alg-iii-s10-n7-cor-1 .statement}

*Soit S un système générateur de l’algèbre A. Pour que $d'\circ\rho = \theta\circ d$, il faut et il suffit que $d'(\rho(x)) = \theta(d(x))$ pour tout $x \in S$.*

C’est une conséquence immédiate de la prop. 9 et de III, p. 123, corollaire.

Sous les conditions de la prop. 9, on sait que B est muni (au moyen de $\rho$) d’une structure de (A, A)-bimodule (II, p. 34, *Exemple 1*).

#### Proposition 10 {#alg-iii-s10-prop-10 .statement}

*Sous les conditions de la prop. 9, pour qu’une $\varepsilon$-dérivation $d' : B \to F$ soit A-linéaire pour les structures de A-module à gauche (resp. à droite) de B et de $\rho_*(F)$, il faut et il suffit que $d'$ s’annule dans la sous-algèbre $\rho(A)$ de B.*

Faisons la démonstration pour les structures de A-module à gauche. Pour $a \in A, b \in B$, on a
$$
d'(\rho(a)b) = d'(\rho(a))b + \rho(a)d'b,
$$
donc si $d' \circ \rho = 0$, $d'$ est linéaire pour les structures de A-module à gauche de B et de $\rho_*(F)$. Réciproquement, s’il en est ainsi, on a en particulier
$$
d'(\rho(a)) = d'(\rho(a).1) = \rho(a)d'(1) = 0
$$
(III, p. 122, prop. 3).

Notons en particulier $D_K(B,F)$ le K-module des *dérivations* de B dans F (III, p. 117); celles de ces dérivations qui sont A-*linéaires*, autrement dit qui s’annulent dans $\rho(A)$, forment un *sous-K-module* de $D_K(B,F)$, que l’on note $D_{A,\rho}(B,F)$ ou simplement $D_A(B,F)$ (on a évidemment $D_K(B,F) = D_{K,\varphi}(B,F)$, où $\varphi : K \to B$ est l’homomorphisme définissant la structure de K-algèbre de B).

Soient maintenant A, B, C trois K-algèbres graduées, $\rho : A \to B, \sigma : B \to C$ deux homomorphismes d’algèbres graduées, G un (C,C)-bimodule gradué; si l’on note $D_A(B,G), D_B(C,G)$ et $D_A(C,G)$ les K-modules respectifs $D_{A,\rho}(B, \sigma_*(G)), D_{B,\sigma}(C,G)$ et $D_{A,\sigma\circ\rho}(C,G)$, il est clair que $D_B(C,G)$ est un *sous-K-module* de $D_A(C,G)$ puisque $\sigma(\rho(A)) \subset \sigma(B)$.

#### Proposition 11 {#alg-iii-s10-prop-11 .statement}

*Sous les conditions précédentes, on a une suite exacte de K-homomorphismes*
$$
0 \longrightarrow D_B(C,G) \overset{u}{\longrightarrow} D_A(C,G) \overset{v}{\longrightarrow} D_A(B,G)
$$
*où u est l’injection canonique et v l’homomorphisme $d \mapsto d \circ \sigma$* (III, p. 125, prop. 9).

En effet, le noyau de $v$ est l’ensemble des dérivations $d : C \to G$ telles que $d(\sigma(b)) = 0$ pour tout $b \in B$, c’est-à-dire précisément l’image de $u$.

### 8. Relations entre dérivations et homomorphismes d’algèbres

Nous supposons de nouveau dans ce n° que l’on se trouve dans le cas II) de III, p. 118, la K-algèbre graduée A n’étant pas supposée associative. Etant donné un élément $\delta \in \Delta$, considérons le K-module gradué E($\delta$) (II, p. 165) tel que $(E(\delta))_{\mu} = E_{\mu + \delta}$ pour tout $\mu \in \Delta$. Définissons sur le K-module gradué $A \oplus E(\delta)$ une structure de K-\emph{algèbre graduée} en posant, pour tout élément homogène $a \in A$, et pour des éléments quelconques $a' \in A, x, x'$ dans $E(\delta)$,

$$(28)$$
$$(a, x)(a', x') = (aa', x.a' + \varepsilon_{\delta, \deg(a)} a.x');$$

la vérification du fait que cette multiplication définit une structure d’anneau gradué est en effet immédiate.

On appelle \emph{augmentation} de l’algèbre $A \oplus E(\delta)$ la projection $p : (a, x) \mapsto a$, qui est un homomorphisme d’algèbres graduées. Les applications K-linéaires $g : A \to A \oplus E(\delta)$ graduées \emph{de degré} 0 telles que la composée

$$
A \xrightarrow{g} A \oplus E(\delta) \xrightarrow{p} A
$$

soit l’identité $1_A$ sont les applications de la forme $x \mapsto (x, f(x))$, où $f : A \to E$ est une application K-linéaire graduée \emph{de degré} $\delta$.

#### Proposition 12 {#alg-iii-s10-prop-12 .statement}

*Pour qu’une application K-linéaire graduée $f : A \to E$ de degré $\delta$ soit une $\varepsilon$-dérivation, il faut et il suffit que l’application $x \mapsto (x, f(x))$ de $A$ dans $A \oplus E(\delta)$ soit un homomorphisme de K-algèbres graduées.*

En effet, si l’on écrit que pour $x$ homogène dans $A$ et $y \in A$, on a

$$(xy, f(xy)) = (x, f(x)).(y, f(y))$$

on obtient, compte tenu de (28), la relation équivalente

$$f(xy) = f(x).y + \varepsilon_{\delta, \deg(x)} x.f(y)$$

d’où la proposition.

#### Proposition 13 {#alg-iii-s10-prop-13 .statement}

*Pour que l’algèbre $A \oplus E(\delta)$ soit associative et unifère, il faut et il suffit que $A$ soit associative et unifère et que les applications $(a, x) \mapsto a.x$ et $(a, x) \mapsto x.a$ définissent sur $E$ une structure de $(A, A)$-bimodule ; l’élément unité de $A \oplus E(\delta)$ est alors $(1, 0)$.*

Si l’on écrit qu’un élément $(u, m) \in A \oplus E(\delta)$ est élément unité de cette algèbre, on trouve aussitôt que $u$ doit être élément unité de $A$; en écrivant que $(u, m).(0, x) = (0, x).(u, m) = (0, x)$, il vient $u.x = x.u = x$ pour $x \in E$, et en écrivant que $(u, m).(u, 0) = (u, 0).(u, m) = (u, 0)$ on obtient $m = 0$. Le fait que $A$ soit associative lorsque $A \oplus E(\delta)$ l’est résulte de ce que l’augmentation est un homomorphisme surjectif. La condition $(x.a').a'' = x.(a'a'')$ équivaut alors à $((0, x)(a', 0))(a'', 0) = (0, x)((a', 0), (a'', 0))$ et de même la condition $a.(a'.x) = (aa').x$ équivaut à $(a, 0)((a', 0)(0, x)) = ((a, 0)(a', 0))(0, x)$; enfin la condition $a.(x.a') = (a.x).a'$ équivaut à $(a, 0)((0, x)(a', 0)) = ((a, 0)(0, x))(a', 0)$.

### 9. Prolongement de dérivations

#### Proposition 14 {#alg-iii-s10-prop-14 .statement}

Soient $A$ un anneau commutatif, $M$ un $A$-module, $B$ la $A$-algèbre $T(M)$ (resp. $S(M)$, resp. $\wedge(M)$), $E$ un $(B,B)$-bimodule. Soient $d_0 : A \to E$ une dérivation de l’anneau $A$ dans le $A$-module $E$, $d_1 : M \to E$ un homomorphisme de groupes additifs tel que, pour tout $a \in A$ et tout $x \in M$, on ait
$$
d_1(ax) = ad_1(x) + d_0(a).x,
$$
et en outre, lorsque $B = S(M)$, que l’on ait
$$
x.d_1(y) + d_1(x).y = y.d_1(x) + d_1(y).x
$$
quels que soient $x, y$ dans $M$, et, lorsque $B = \wedge(M)$,
$$
x.d_1(x) + d_1(x).x = 0
$$
pour tout $x \in M$.

Alors il existe une dérivation et une seule $d$ de $B$ (considéré comme $\mathbf{Z}$-algèbre) dans le $(B, B)$-bimodule $E$ telle que $d | A = d_0$ et $d | M = d_1$.

Prenons sur le $\mathbf{Z}$-module $B \oplus E$ la structure de $\mathbf{Z}$-algèbre associative définie par
$$
(b, t)(b', t') = (bb', bt' + tb')
$$
dont $(1, 0)$ est l’élément unité (III, p. 127, prop. 13). Par l’injection canonique $t \mapsto (0, t)$, $E$ s’identifie à un idéal bilatère de $B \oplus E$ tel que $E^2 = \{0\}$. D’autre part, l’application $h_0 : A \to B \oplus E$ définie par $h_0(a) = (a, d_0(a))$ est un homomorphisme unifère d’anneaux (III, p. 127, prop. 12); par cette application, $B \oplus E$ devient donc une $A$-algèbre. En outre, si, pour tout $x \in M$, on pose $h_1(x) = (x, d_1(x))$, il résulte de la définition de $h_0$ et de (29) que l’on a $h_1(ax) = h_0(a)h_1(x)$; autrement dit $h_1$ est une application $A$-linéaire de $M$ dans $B \oplus E$. Il existe alors un homomorphisme de $A$-algèbres $h : B \to B \oplus E$ et un seul tel que $h | M = h_1$ (et nécessairement $h | A = h_0$) : en effet, si $B = T(M)$, cela résulte de III, p. 56, prop. 1; si $B = S(M)$, la condition (30) montre que $h(x)h(y) = h(y)h(x)$ quels que soient $x, y$ dans $M$, et la conclusion résulte de III, p. 67, prop. 2; enfin, si $B = \wedge(M)$, la condition (31) montre que $(h(x))^2 = 0$ quel que soit $x \in M$, puisque $x \wedge x = 0$, et la conclusion résulte de III, p. 77, prop. 1. L’homomorphisme $h$ est tel que le composé $p \circ h : B \to B$ avec l’augmentation $p : B \oplus E \to B$ soit l’identité $1_B$, car $p \circ h$ et $1_B$ coïncident par définition pour les éléments de $A$ et ceux de $M$, et l’ensemble de ces éléments est un système générateur de $B$. On peut par suite écrire $h(b) = (b, d(b))$ pour tout $b \in B$, et l’application $b \mapsto d(b)$ de $B$ dans $E$ est une dérivation répondant à la question, en vertu de la prop. 12 de III, p. 127.

#### Corollaire {#alg-iii-s10-n9-cor-1 .statement}

Soit $M$ un $K$-module gradué de type $\Delta$; on munit les $K$-algèbres $T(M)$, $S(M)$ et $\wedge(M)$ des graduations correspondantes de type $\Delta' = \Delta \times \mathbf{Z}$ (III, p. 62, prop. 7, III, p. 76, prop. 10 et III, p. 86, prop. 11). On munit d’autre part $M$ de la graduation de type $\Delta'$ telle que $M_{\alpha, 1} = M_\alpha$ pour tout $\alpha \in \Delta$ et $M_{\alpha, n} = \{0\}$ pour $\alpha \in \Delta$ et $n \neq 1$. Soit $\varepsilon'$ un facteur de commutation sur $\Delta'$.

(i) Soit $E$ un $T(M)$-bimodule (à droite et à gauche) gradué de type $\Delta'$; pour tout δ ∈ Δ et tout entier n ∈ Z, toute application K-linéaire f : M → E graduée de degré δ₁ = (δ, n) se prolonge d’une seule manière en une ε'-dérivation d : T(M) → E de degré δ'.

(ii) Soit E un S(M)-module gradué de type Δ'; pour qu’une application K-linéaire f : M → E, graduée de degré δ', se prolonge en une ε'-dérivation d : S(M) → E de degré δ', il faut et il suffit que, pour tout couple (x, y) d’éléments homogènes de M, on ait
(33) x . f(y) + ε'_{δ', (deg(y), 1)} y . f(x) = y . f(x) + ε'_{δ', (deg(x), 1)} x . f(y).
La ε'-dérivation d est alors unique.

(iii) Soit E un ∧(M)-bimodule (à gauche et à droite) gradué de type Δ'; pour qu’une application K-linéaire f : M → E graduée de degré δ', se prolonge en une ε'-dérivation d : ∧(M) → E de degré δ', il faut et il suffit que, pour tout élément homogène x de M, on ait
(34) x . f(x) + ε'_{δ', (deg(x), 1)} f(x) . x = 0.
La ε'-dérivation d est alors unique.

On applique la Remarque 2 de III, p. 118 en modifiant l’une des lois d’action de B-module de E (avec B égal à T(N), S(M) ou ∧(M)); la loi d’action ainsi modifiée est encore, en vertu de (1) (III, p. 116), une loi de B-module, et la structure de B-module ainsi obtenue sur E est encore compatible avec l’autre structure de B-module. Il suffit alors d’appliquer la prop. 14 (III, p. 128), avec A = K et d₀ = 0.

Exemple 1). — Dans l’application de la prop. 14, on notera que si d₀ = 0, la condition (29) (III, p. 128) signifie simplement que d₁ est A-linéaire. Si l’on prend en particulier E = B, et la structure de (B, B)-bimodule déduite de la structure d’anneau de B, les conditions (30) et (31) (III, p. 128) sont automatiquement vérifiées lorsqu’on prend pour d₁ la composée d’un endomorphisme s de M et de l’injection canonique M → B: c’est évident pour (30) puisque S(M) est commutative, et pour (31) cela résulte de ce que x et s(x) sont de degré 1 dans ∧(M). On voit donc que tout endomorphisme s de M se prolonge d’une seule manière en une dérivation Dₛ de T(M) (resp. de S(M), resp. de ∧(M)), qui est de degré 0. En outre, on a, pour deux endomorphismes s, t de M,
(35) [Dₛ, Dₜ] = D_{[s, t]}
car les deux membres sont des dérivations de T(M) (resp. S(M), resp. ∧(M)) qui sont égales à [s, t] dans M.

On obtiendra l’expression de Dₛ à l’aide de la formule (21) de III, p. 123, qui donne respectivement, pour x₁, x₂, ..., xₙ dans M
$$
\begin{cases}
Dₛ(x₁ \otimes x₂ \otimes \cdots \otimes xₙ) \\
= \sum_{i=1}^{n} x₁ \otimes \cdots \otimes x_{i-1} \otimes s(x_i) \otimes x_{i+1} \otimes \cdots \otimes xₙ \\
Dₛ(x₁x₂ \cdots xₙ) = \sum_{i=1}^{n} x₁ \cdots x_{i-1} s(x_i)x_{i+1} \cdots xₙ \\
Dₛ(x₁ \wedge x₂ \wedge \cdots \wedge xₙ) \\
= \sum_{i=1}^{n} x₁ \wedge \cdots \wedge x_{i-1} \wedge s(x_i) \wedge x_{i+1} \wedge \cdots \wedge xₙ.
\end{cases}
$$
(36)

Dans le cas de l’algèbre $\wedge (\mathbf{M})$, on a la propriété suivante de $D_s$:

#### Proposition 15 {#alg-iii-s10-prop-15 .statement}

*Si $\mathbf{M}$ est un $K$-module libre de rang fini $n$, alors, pour tout endomorphisme $s$ de $\mathbf{M}$, la restriction à $\wedge^n(\mathbf{M})$ de la dérivation $D_s$ est l’homothétie de rapport $\mathrm{Tr}(s)$.*

En effet, soit $(e_j)_{1 \leq j \leq n}$ une base de $\mathbf{M}$ et posons $e = e_1 \wedge e_2 \wedge \cdots \wedge e_n$. Si $s(e_j) = \sum_{i=1}^n \alpha_{jk} e_k$, la troisième formule (36) donne
$$
D_s(e) = \sum_{i=1}^n e_1 \wedge \cdots \wedge e_{i-1} \wedge s(e_i) \wedge e_{i+1} \wedge \cdots \wedge e_n = \left( \sum_{j=1}^n \alpha_{jj} \right) e.
$$

*Exemple.—*2) Dans III, p. 128–129, corollaire, (iii), prenons $\Delta = \{0\}$, la graduation sur $\wedge(\mathbf{M})$ étant donc la graduation usuelle de type $\mathbf{Z}$; prenons d’autre part $\varepsilon_{p,q} = (-1)^{pq}$. Alors, pour toute forme linéaire $x^* \in \mathbf{M}^*$ sur $\mathbf{M}$, $x \mapsto \langle x, x^* \rangle$ est une application $K$-linéaire graduée de degré $-1$ de $\mathbf{M}$ dans $\wedge(\mathbf{M})$ vérifiant la relation (34) de III, p. 129; il existe donc une *antidérivation* $i(x^*)$ de $\wedge(\mathbf{M})$, de degré $-1$, telle que (en vertu de la formule (21) de III, p. 123)
$$
i(x^*)(x_1 \wedge \ldots \wedge x_n) = \sum_{i=1}^n (-1)^{i-1} \langle x_i, x^* \rangle x_1 \wedge \cdots \wedge x_{i-1} \wedge x_{i+1} \wedge \ldots \wedge x_n
$$
et qui est un cas particulier du produit intérieur qui sera défini dans III, p. 166, formule (68).

#### Proposition 16 {#alg-iii-s10-prop-16 .statement}

*Soient $A$ une $K$-algèbre commutative, $M_i$ ($1 \leq i \leq n$) et $P$ des $A$-modules, $H$ le $A$-module des applications $A$-multilinéaires de $M_1 \times M_2 \times \cdots \times M_n$ dans $P$. On suppose donnée une $K$-dérivation $d_0 : A \to A$ de l’algèbre $A$, et pour chaque $i$, une application $K$-linéaire $d_i : M_i \to M_i$ et une application $K$-linéaire $D : P \to P$, de sorte que pour $1 \leq i \leq n$, $(d_0, d_i, d_i)$ soit une $K$-dérivation de $(A, M_i, M_i)$ dans lui-même et que $(d_0, D, D)$ soit une dérivation de $(A, P, P)$ dans lui-même. Alors il existe une application $K$-linéaire $D' : H \to H$ telle que $(d_0, D', D')$ soit une $K$-dérivation de $(A, H, H)$ dans lui-même et que l’on ait*
$$
(37)\quad D(f(x_1, \ldots, x_n)) = (D'f)(x_1, \ldots, x_n) + \sum_{i=1}^n f(x_1, \ldots, x_{i-1}, d_ix_i, x_{i+1}, \ldots, x_n)
$$
*quels que soient* $x_i \in M_i$ *pour* $1 \leq i \leq n$ *et* $f \in H$.

Montrons que pour $f \in H$, l’application $D'f$ de $M_1 \times M_2 \times \cdots \times M_n$ dans $P$ définie par (37) est $A$-multilinéaire. En effet, pour $a \in A$, on a
$$
(D'f)(ax_1, x_2, \ldots, x_n) = D(a f(x_1, \ldots, x_n)) - f(d_1(ax_1), x_2, \ldots, x_n)
$$
$$
- a \sum_{i=2}^n f(x_1, \ldots, x_{i-1}, d_ix_i, x_{i+1}, \ldots, x_n)
$$
et par hypothèse $D(a f(x_1, \ldots, x_n)) = (d_0a)f(x_1, \ldots, x_n) + aD(f(x_1, \ldots, x_n))$ et $d_1(ax_1) = (d_0a)x_1 + a.d_1x_1$, ce qui donne $(D'f)(ax_1, x_2, \ldots, x_n) =$ a. $(\mathrm{D}'f)(x_1, \ldots, x_n)$, et on prouve de même la linéarité en chacun des $x_i$. D’autre part, on a

$$
(\mathrm{D}'(af))(x_1, \ldots, x_n)
$$
$$
= \mathrm{D}(af(x_1, \ldots, x_n)) - \sum_{i=1}^m af(x_1, \ldots, x_{i-1}, d_ix_i, x_{i+1}, \ldots, x_n)
$$
$$
= (d_0a)f(x_1, \ldots, x_n) + a\mathrm{D}(f(x_1, \ldots, x_n))
$$
$$
- \sum_{i=1}^m af(x_1, \ldots, x_{i-1}, d_ix_i, x_{i+1}, \ldots, x_n)
$$
$$
= (d_0a)f(x_1, \ldots, x_n) + a(\mathrm{D}'f)(x_1, \ldots, x_n)
$$

autrement dit
$$
\mathrm{D}'(af) = (d_0a)f + a(\mathrm{D}'f)
$$
ce qui établit la proposition.

*Exemples. — 3*) Appliquant la prop. 16 (III, p. 130) au cas $n = 1$, $M_1 = M$, $P = A$, on a $H = M^*$, *dual* de $M$; on voit qu’on déduit d’une K-dérivation $(d_0, d, d)$ de $(A, M, M)$ une K-dérivation $(d_0, d^*, d^*)$ de $(A, M^*, M^*)$ telle que
$$
d_0\langle m, m^* \rangle = \langle dm, m^* \rangle + \langle m, d^*m^* \rangle
$$
pour $m \in M$ et $m^* \in M^*$. L’application K-linéaire de $M \oplus M^*$ dans lui-même qui est égale à $d$ dans $M$ et à $d^*$ dans $M^*$ vérifie alors la condition (29) de III, p. 128, et il y a par suite une K-*dérivation* $D$ de la A-algèbre $T(M \oplus M^*)$, qui se réduit à $d_0$ dans $A$, à $d$ dans $M$ et à $d^*$ dans $M^*$. La restriction $d_J^I$ de $D$ au sous-A-module $T_J^I(M)$ de $T(M \oplus M^*)$ (III, p. 63) est un K-endomorphisme de $T_J^I(M)$ tel que $(d_0, d_J^I, d_J^I)$ soit une K-*dérivation* de $(A, T_J^I(M), T_J^I(M))$. En outre, pour $i \in I, j \in J$, si l’on pose $I' = I - \{i\}, J' = J - \{j\}$, on vérifie aussitôt que l’on a pour la contraction $c_j^i$ (III, p. 64)
$$
c_j^i(d_J^I(z)) = d_{J'}^{I'}(c_j^i(z)) \quad \text{pour tout } z \in T_J^I(M).
$$

4) Soient $M_i$ ($1 \leq i \leq 3$) trois A-modules, et pour chaque $i$, supposons que $(d_0, d_i, d_i)$ soit une dérivation de $(A, M_i, M_i)$; appliquant de nouveau la prop. 16 (III, p. 130) pour $n = 1$, on en déduit pour tout couple $(i, j)$, une dérivation $(d_0, d_{ij}, d_{ij})$ de $(A, H_{ij}, H_{ij})$, où $H_{ij} = \mathrm{Hom}_A(M_i, M_j)$. Avec ces notations, a on, pour $u \in \mathrm{Hom}_A(M_1, M_2)$ et $v \in \mathrm{Hom}_A(M_2, M_3)$,
$$
d_{13}(v \circ u) = (d_{23}v) \circ u + v \circ (d_{12}u)
$$
comme on le vérifie aussitôt sur les définitions.

### 10. Problème universel pour les dérivations: cas non commutatif

Dans toute la fin du § 10, toutes les algèbres sont supposées associatives et unifères, et tout homomorphisme d’algèbres est supposé unifère.

Soit $A$ une $K$-algèbre; le produit tensoriel $A \otimes_K A$ est canoniquement muni d’une structure de $(A, A)$-bimodule pour laquelle
$$
x . (u \otimes v) . y = (xu) \otimes (vy)
$$
quels que soient $x, y, u, v$ dans $A$ (III, p. 39, Exemple 2). L’application $K$-linéaire $m : A \otimes_K A \to A$ correspondant à la multiplication dans $A$ (donc telle que $m(x \otimes y) = xy$) est un homomorphisme de $(A, A)$-bimodules; son noyau $I$ est donc un sous-bimodule de $A \otimes_K A$.

#### Lemme 1 {#alg-iii-s10-lem-1 .statement}

*L’application $\delta_A : x \mapsto x \otimes 1 - 1 \otimes x$ est une $K$-dérivation de $A$ dans $I$, et $I$ est engendré, en tant que $A$-module à gauche, par l’image de $\delta_A$.*

La première assertion résulte de ce que
$$
(xy) \otimes 1 - 1 \otimes (xy) = (x \otimes 1 - 1 \otimes x) . y + x . (y \otimes 1 - 1 \otimes y)
$$
en vertu de (40). D’autre part, si l’élément $\sum_i x_i \otimes y_i$ (pour les $x_i, y_i$ dans $A$) appartient à $I$, on a par définition $\sum_i x_i y_i = 0$, donc
$$
\sum_i (x_i \otimes y_i) = \sum_i x_i . (1 \otimes y_i - y_i \otimes 1)
$$
en vertu de (40), ce qui achève de prouver le lemme.

#### Proposition 17 {#alg-iii-s10-prop-17 .statement}

*La dérivation $\delta_A$ possède la propriété universelle suivante: pour toute $(A, A)$-bimodule $E$ et toute $K$-dérivation $d : A \to E$, il existe un homomorphisme de $(A, A)$-bimodules $f : I \to E$ et un seul tel que $d = f \circ \delta_A$.*

Notons d’abord que, pour tout homomorphisme $f : I \to E$ de $(A, A)$-bimodules, $f \circ \delta_A$ est une dérivation (III, p. 125, prop. 9). Inversement, soit $d : A \to E$ une $K$-dérivation, et prouvons d’abord que s’il existe un homomorphisme $f : I \to E$ de $(A, A)$-bimodules tel que $d = f \circ \delta_A$, $f$ est *uniquement déterminé* par cette condition; en effet, la définition de $\delta_A$ donne
$$
f(x \otimes 1 - 1 \otimes x) = dx
$$
et notre assertion résulte de ce que l’image de $\delta_A$ engendre $I$ comme $A$-module à gauche (lemme 1): on doit donc avoir
$$
f\left( \sum_i x_i \otimes y_i \right) = \sum_i x_i . f(1 \otimes y_i - y_i \otimes 1) = - \sum_i x_i . dy_i.
$$
Inversement, comme l’application $(x, y) \mapsto -x . dy$ de $A \times A$ dans $E$ est $K$-bilinéaire, il existe une application $K$-linéaire et une seule $g : A \otimes_K A \to E$ telle que $g(x \otimes y) = -x . dy$; il suffit de voir que la restriction $f$ de $g$ à $I$ est $A$-linéaire pour les structures de $A$-module à gauche et de $A$-module à droite. La première assertion est évidente puisque $(xx') . dy = x . (x' . dy)$; pour prouver la seconde, notons que si $\sum_i x_i \otimes y_i \in I$ et $x \in A$, on a
$$
\sum_i x_i . d(y_i x) = \sum_i x_i . dy_i . x + \sum_i (x_i y_i) . dx;
$$
mais, puisque $\sum_i x_i y_i = 0$ par définition de $I$, cela termine la démonstration.

On a ainsi défini un *isomorphisme canonique* $f \mapsto f \circ \delta_A$ de K-modules

$$
\operatorname{Hom}_{(A, A)}(I, E) \to D_K(A, E)
$$

le premier membre étant le K-module des homomorphismes de $(A, A)$-bimodules de $A$ dans $E$.

### 11. Problème universel pour les dérivations : cas commutatif

Supposons maintenant que $A$ soit une K-algèbre *commutative* et $E$ un *A-module*; $E$ peut être considéré comme un $(A, A)$-bimodule dont les deux lois externes sont identiques à la loi de $A$-module donnée. D’autre part la structure de $(A, A)$-bimodule de $A \otimes_K A$ s’identifie à sa structure de $(A \otimes_K A)$-module provenant de la structure d’anneau *commutatif* de $A \otimes_K A$, puisqu’on a ici pour $x, y, u, v$ dans $A$,

$$
x . (u \otimes v) . y = (xu) \otimes (vy) = (xu) \otimes (yv) = (x \otimes y)(u \otimes v).
$$

Le noyau $\mathfrak{J}$ de $m$ est donc ici un *idéal* de l’anneau $A \otimes_K A$ et comme $m : A \otimes_K A \to A$ est surjectif, $(A \otimes_K A)/\mathfrak{J}$ est isomorphe à $A$; si en outre on considère $E$ comme un $(A \otimes_K A)$-module au moyen de $m$ (autrement dit le $(A \otimes_K A)$-module $m_*(E)$), les homomorphismes $\mathfrak{J} \to E$ de $(A, A)$*-bimodules* s’identifient aux homomorphismes $\mathfrak{J} \to E$ de $(A \otimes_K A)$*-modules* (III, p. 39), autrement dit on a un isomorphisme canonique de K-modules

$$
\operatorname{Hom}_{(A, A)}(\mathfrak{J}, E) \to \operatorname{Hom}_{A \otimes_K A}(\mathfrak{J}, E).
$$

D’autre part, on a $\mathfrak{J}E = \{0\}$, car les éléments $1 \otimes x - x \otimes 1$ engendrent $\mathfrak{J}$ comme $(A \otimes_K A)$-module (III, p. 132, lemme 1) et on a, pour tout $z \in E$, $(1 \otimes x - x \otimes 1).z = 0$ en vertu de la définition de la structure de $(A \otimes_K A)$-module sur $E$. Puisque $\mathfrak{J}$ est contenu dans l’annulateur du $(A \otimes_K A)$-module $E$, et que la structure de $((A \otimes_K A)/\mathfrak{J})$-module de $E$ n’est autre par définition que la structure initiale de $A$-module donnée sur $E$, on a, compte tenu de l’isomorphisme canonique de $\mathfrak{J} \otimes_K ((A \otimes_K A)/\mathfrak{J})$ et de $\mathfrak{J}/\mathfrak{J}^2$ (III, p. 34, cor. 1), un isomorphisme canonique de K-modules

$$
\operatorname{Hom}_{A \otimes_K A}(\mathfrak{J}, E) \to \operatorname{Hom}_A(\mathfrak{J}/\mathfrak{J}^2, E).
$$

Compte tenu de la prop. 17 de III, p. 132, on voit que nous avons prouvé la proposition suivante:

#### Proposition 18 {#alg-iii-s10-prop-18 .statement}

*Soient $A$ une K-algèbre commutative, $\mathfrak{J}$ l’idéal noyau de l’homomorphisme canonique surjectif $m : A \otimes_K A \to A$, de sorte que $A$ est isomorphe à $(A \otimes_K A)/\mathfrak{J}$ et que $\mathfrak{J}/\mathfrak{J}^2$ est canoniquement muni d’une structure de $A$-module. Soit $d_{A/K} : A \to \mathfrak{J}/\mathfrak{J}^2$ l’application K-linéaire qui, à tout $x \in A$, fait correspondre la classe de $x \otimes 1 - 1 \otimes x$ modulo $\mathfrak{J}^2$. L’application $d_{A/K}$ est une K-dérivation, et pour tout $A$-module $E$, et toute

K-dérivation $D : A \to E$, il existe une application A-linéaire et une seule $g : \mathfrak{S}/\mathfrak{S}^2 \to E$ telle que $D = g \circ d_{A/K}$.

On dit que le A-module $\mathfrak{S}/\mathfrak{S}^2$ est le A-module des K-différentielles de A, et on le note $\Omega_K(A)$; pour tout $x \in A$, $d_{A/K}(x)$ (aussi noté $dx$) s’appelle la différentielle de $x$; on a vu (III, p. 132, lemme 1) que les éléments $d_{A/K}(x)$, pour $x \in A$, forment un système générateur du A-module $\Omega_K(A)$. La prop. 18 montre que l’application $g \mapsto g \circ d_{A/K}$ est un isomorphisme canonique de A-modules

$$
\varphi_A : \operatorname{Hom}_A(\Omega_K(A), E) \to D_K(A, E)
$$

(la structure de A-module de $D_K(A, E)$ étant définie par la prop. 7 de III, p. 124).

Le couple $(\Omega_K(A), d_{A/K})$ est donc solution du problème d’application universelle où $\Sigma$ est l’espèce de structure de A-module et les $\alpha$-applications les K-dérivations de A dans un A-module (E, IV, p. 23).

#### Exemple {#alg-iii-s10-n11-exa-1 .statement}

Soit M un K-module; il résulte de la prop. 14 de III, p. 128 que pour tout S(M)-module E, l’application $D \mapsto D|_M$ définit un isomorphisme de S(M)-modules de $D_K(S(M), E)$ sur $\operatorname{Hom}_K(M, E)$; d’autre part, puisque E est un S(M)-module, $\operatorname{Hom}_K(M, E)$ est canoniquement isomorphe à $\operatorname{Hom}_{S(M)}(M \otimes_K S(M), E)$, tout K-homomorphisme de M dans E s’écrivant d’une seule manière $x \mapsto h(x \otimes 1)$, où $h \in \operatorname{Hom}_{S(M)}(M \otimes_K S(M), E)$ (II, p. 82). Soit $D_0$ la K-dérivation $S(M) \to M \otimes_K S(M)$ dont la restriction à M est l’homomorphisme canonique $x \mapsto x \otimes 1$; toute K-dérivation $D : S(M) \to E$ s’écrit donc d’une seule manière $h \circ D_0$ avec $h \in \operatorname{Hom}_{S(M)}(M \otimes_K S(M), E)$. En vertu de l’unicité d’une solution d’un problème d’application universelle, on voit qu’il existe un unique isomorphisme de S(M)-modules

$$
\omega : M \otimes_K S(M) \to \Omega_K(S(M))
$$

tel que $D_0 \circ \omega = d_{S(M)/K}$; autrement dit, pour tout $x \in M$, on a $\omega(x \otimes 1) = dx$.

En particulier, si M est un K-module libre de base $(e_\lambda)_{\lambda \in L}$, $\Omega_K(S(M))$ est un S(M)-module libre ayant pour base l’ensemble des différentielles de $e_\lambda$. Considérons en particulier le cas où $L = \{1, n\}$, de sorte que S(M) s’identifie à l’algèbre de polynômes $K[X_1, \ldots, X_n]$ (III, p. 75); pour tout polynôme $P \in K[X_1, \ldots, X_n]$, on peut écrire d’une seule manière

$$
dP = \sum_{i=1}^n D_i P \cdot dX_i
$$

avec $D_i P \in K[X_1, \ldots, X_n]$, et en vertu de ce qui précède, les applications $P \mapsto D_i P$ sont les K-dérivations de $K[X_1, \ldots, X_n]$ correspondant aux formes coordonnées sur $\Omega_K(S(M))$ pour la base $(dX_i)$; on écrit aussi $\frac{\partial P}{\partial X_i}$ au lieu de $D_i P$, et on l’appelle la dérivée partielle de P par rapport à $X_i$.

### 12. Propriétés fonctorielles des K-différentielles

#### Proposition 19 {#alg-iii-s10-prop-19 .statement}

Soit

$$
\begin{array}{ccc}
K & \xrightarrow{\sigma} & K' \\
\eta \downarrow & & \eta' \downarrow \\
A & \xrightarrow{u} & A'
\end{array}
$$

un diagramme commutatif d’homomorphismes d’anneaux commutatifs, $\eta$ (resp. $\eta'$) faisant de $A$ (resp. $A'$) une $K$-algèbre (resp. $K'$-algèbre). Il existe une application $A$-linéaire et une seule $v : \Omega_K(A) \to \Omega_{K'}(A')$ rendant commutatif le diagramme

$$
\begin{array}{ccc}
A & \xrightarrow{u} & A' \\
d_{A/K} \downarrow & & d_{A'/K'} \downarrow \\
\Omega_K(A) & \xrightarrow{v} & \Omega_{K'}(A')
\end{array}
$$

En effet, $d_{A'/K'} \circ u$ est une $K$-dérivation de $A$ à valeurs dans le $A$-module $\Omega_{K'}(A')$; l’existence et l’unicité de $v$ résultent alors de la prop. 18 de III, p. 133.

L’application $v$ de la prop. 19 sera notée $\Omega(u)$; si l’on a un diagramme commutatif d’homomorphismes d’anneaux commutatifs

$$
\begin{array}{ccccc}
K & \xrightarrow{\sigma'} & K' & \xrightarrow{\sigma''} & K'' \\
\eta \downarrow & & \eta' \downarrow & & \eta'' \downarrow \\
A & \xrightarrow{u} & A' & \xrightarrow{u'} & A''
\end{array}
$$

il résulte aussitôt de la propriété d’unicité de la prop. 19 que

$$
\Omega(u' \circ u) = \Omega(u') \circ \Omega(u).
$$

Puisque $\Omega_{K'}(A')$ est un $A'$-module, on déduit canoniquement de $\Omega(u)$ une application $A'$-linéaire

$$
\Omega_0(u) : \Omega_K(A) \otimes_A A' \to \Omega_{K'}(A')
$$

telle que $\Omega(u)$ soit composée de $\Omega_0(u)$ et de l’homomorphisme canonique $i_A : \Omega_K(A) \to \Omega_K(A) \otimes_A A'$. Pour tout $A'$-module $E'$, on a un diagramme commutatif

$$
\begin{array}{ccc}
\operatorname{Hom}_{A'}(\Omega_{K'}(A'), E') & \xrightarrow{\operatorname{Hom}(\Omega_0(u), 1_{E'})} & \operatorname{Hom}_{A'}(\Omega_K(A) \otimes_A A', E') \\
\varphi_{A'} \downarrow & & \varphi_{A'} \circ r_A \downarrow \\
D_{K'}(A', E') & \xrightarrow{C(u)} & D_K(A, E)
\end{array}
$$

où $C(u)$ est l’application $D \mapsto D \circ u$ (III, p. 125, prop. 9) et $r_A$ l’isomorphisme canonique $\operatorname{Hom}(i_A, 1_{E'}) : \operatorname{Hom}_{A'}(\Omega_K(A) \otimes_A A', E') \to \operatorname{Hom}_A(\Omega_K(A), E')$; cela résulte aussitôt de la prop. 19 et de la définition des isomorphismes $\varphi_A$ et $\varphi_{A'}$.

#### Proposition 20 {#alg-iii-s10-prop-20 .statement}

Supposons que l’on ait $A' = A \otimes_K K'$, $\eta': K' \to A'$ et $u: A \to A'$ étant les homomorphismes canoniques. Alors l’application $A'$-linéaire

$$
\Omega_0(u): \Omega_K(A) \otimes_A A' \to \Omega_{K'}(A')
$$

est un isomorphisme.

En vertu du fait que dans le diagramme (42) de III, p. 135 les flèches verticales sont bijectives, tout revient à prouver que, pour tout $A'$-module $E'$, l’homomorphisme $C(u): D \mapsto D \circ u$ du diagramme (42) est bijectif (II, p. 36, th. 1). Or $\mathrm{Hom}(u, 1_{E'}): \mathrm{Hom}_{K'}(A \otimes_K K', E') \to \mathrm{Hom}_K(A, E')$ est un isomorphisme (II, p. 82, prop. 1) et $C(u)$ en est la restriction à $D_{K'}(A', E')$, donc est injectif; d’ailleurs, si $f: A' \to E'$ est une application $K'$-linéaire telle que $f \circ u: A \to E'$ soit une $K$-dérivation, on déduit aussitôt du fait que $f$ est $K'$-linéaire et de ce que $f((x \otimes 1)(y \otimes 1)) = (y \otimes 1)f(x \otimes 1) + (x \otimes 1)f(y \otimes 1)$ pour $x, y$ dans $A$, que $f$ est une $K'$-dérivation, les éléments $x \otimes 1$ pour $x \in A$ formant un système générateur du $K'$-module $A'$; ceci achève de montrer que $C(u)$ est bijectif.

Bornons-nous désormais au cas où $\rho: K \to K'$ est l’application identique de $K$; à tout homomorphisme de $K$-algèbres $u: A \to B$, on associe donc une application $B$-linéaire

$$
\Omega_0(u): \Omega_K(A) \otimes_A B \to \Omega_K(B).
$$

D’autre part, on peut considérer le $B$-module des $A$-différentielles $\Omega_A(B)$ puisque $B$ est une $A$-algèbre au moyen de $u$; la dérivation canonique $d_{B/A}: B \to \Omega_A(B)$ étant $a fortiori$ une $K$-dérivation, se factorise de façon unique en

$$
B \xrightarrow{d_{B/K}} \Omega_K(B) \xrightarrow{\Omega_u} \Omega_A(B)
$$

où $\Omega_u$ est une application $B$-linéaire (III, p. 133, prop. 18). Pour tout $B$-module $E$, on a un diagramme commutatif

$$
\begin{array}{ccc}
\mathrm{Hom}_B(\Omega_A(B), E) & \xrightarrow{\mathrm{Hom}(\Omega_u, 1_E)} & \mathrm{Hom}_B(\Omega_K(B), E) \\
\varphi_{A,B} \downarrow & & \varphi_{K,B} \downarrow \\
D_A(B, E) & \xrightarrow{j_u} & D_K(B, E)
\end{array}
$$

$j_u$ étant l’injection canonique (III, p. 126); cela résulte aussitôt de la prop. 18 de III, p. 133.

#### Proposition 21 {#alg-iii-s10-prop-21 .statement}

La suite d’applications $B$-linéaires

$$
\Omega_K(A) \otimes_A B \xrightarrow{\Omega_0(u)} \Omega_K(B) \xrightarrow{\Omega_u} \Omega_A(B) \longrightarrow 0
$$

est exacte.

Tout revient à voir que, pour tout $B$-module $E$, la suite

$$
0 \longrightarrow \mathrm{Hom}_B(\Omega_A(B), E) \xrightarrow{\mathrm{Hom}(\Omega_u, 1_E)} \mathrm{Hom}_B(\Omega_K(B), E) \xrightarrow{\mathrm{Hom}(\Omega_0(u), 1_E)} \mathrm{Hom}_B(\Omega_K(A) \otimes_A B, E)
$$

est exacte (II, p. 36, th. 1); mais en vertu du fait que dans les diagrammes commutatifs (42) (III, p. 135) et (44) (III, p. 136), les flèches verticales sont des isomorphismes, il suffit de montrer que la suite

$$
0 \longrightarrow D_A(B, E) \xrightarrow{j_u} D_K(B, E) \xrightarrow{C(u)} D_K(A, E)
$$

est exacte, ce qui n’est autre que la prop. 11 de III, p. 126.

Considérons maintenant le cas où l’homomorphisme de K-algèbres $u : A \to B$ est surjectif; si $\mathfrak{J}$ est son noyau, B est donc isomorphe à $A/\mathfrak{J}$. Considérons la restriction $d|_{\mathfrak{J}} : \mathfrak{J} \to \Omega_K(A)$ de la dérivation canonique $d = d_{A/K}$, et l’application A-linéaire composée

$$
d' : \mathfrak{J} \xrightarrow{d|_{\mathfrak{J}}} \Omega_K(A) \xrightarrow{i_A} \Omega_K(A) \otimes_A B.
$$

On a $d'(\mathfrak{J}^2) = 0$, car pour $x, y$ dans $\mathfrak{J}$, on a
$$
d'(xy) = d(xy) \otimes 1 = (x.dy + y.dx) \otimes 1 = dy \otimes u(x) + dx \otimes u(y) = 0
$$
puisque $u(x) = u(y) = 0$. On déduit donc de $d'$, par passage au quotient, une application A-linéaire

$$
\bar{d} : \mathfrak{J}/\mathfrak{J}^2 \to \Omega_K(A) \otimes_A B
$$

et comme $\mathfrak{J}$ annule le A-module $\mathfrak{J}/\mathfrak{J}^2$, $\bar{d}$ est en fait une application B-linéaire.

#### Proposition 22 {#alg-iii-s10-prop-22 .statement}

*Soient $\mathfrak{J}$ un idéal de la K-algèbre commutative $A, B = A/\mathfrak{J}$, et $u : A \to B$ l’homomorphisme canonique. La suite des applications B-linéaires*

$$
\mathfrak{J}/\mathfrak{J}^2 \xrightarrow{\bar{d}} \Omega_K(A) \otimes_A B \xrightarrow{\Omega_0(u)} \Omega_K(B) \longrightarrow 0
$$

*est alors exacte*.

Notons que $\Omega_K(A) \otimes_A B$ s’identifie à $\Omega_K(A)/\mathfrak{J}\Omega_K(A)$, et que l’image de $\bar{d}$ est l’image de $d(\mathfrak{J})$ dans ce module quotient; le quotient de $\Omega_K(A) \otimes_A B$ par $\operatorname{Im}(\bar{d})$ s’identifie donc au quotient $\Omega_K(A)/N$, où N est le sous-A-module engendré par $\mathfrak{J}\Omega_K(A)$ et $d(\mathfrak{J})$. En outre, l’application composée

$$
A \xrightarrow{d_{A/K}} \Omega_K(A) \longrightarrow \Omega_K(A)/N
$$

est une K-dérivation (III, p. 125, prop. 9), et puisqu’elle s’annule dans $\mathfrak{J}$ par définition de N, elle définit, par passage au quotient, une K-dérivation $D_0 : B \to \Omega_K(A)/N$. Compte tenu de l’unicité de la solution d’un problème d’application universelle, tout revient à prouver que, pour tout B-module E et toute K-dérivation $D : B \to E$, il existe une application B-linéaire unique $g : \Omega_K(A)/N \to E$ telle que $D = g \circ D_0$. Or, l’application composée $D \circ u : A \to E$ est une K-dérivation (III, p. 125, prop. 9), donc il existe une application A-linéaire $f : \Omega_K(A) \to E$ et une seule telle que $f \circ d_{A/K} = D \circ u$. Cette relation montre déjà que $f$ s’annule dans $d(\mathfrak{J})$; comme de plus $\mathfrak{J}E = \{0\}$ puisque E est un B-module, $f$ s’annule dans $\mathfrak{J}\Omega_K(A)$; donc $f$ s’annule dans N, et définit par passage au quotient, une application B-linéaire $g : \Omega_K(A)/N \to E$ telle que $g \circ D_0 = D$; l’unicité de $g$ résulte de l’unicité de $f$.

C. Q. F. D.

On se gardera de croire que, si $u : A \to B$ est un homomorphisme injectif, $\Omega_0(u) : \Omega_K(A) \otimes_A B \to \Omega_K(B)$ soit nécessairement injectif (III, p. 197, exerc. 5). Toutefois, on a la proposition suivante:

#### Proposition 23 {#alg-iii-s10-prop-23 .statement}

*Soient A une K-algèbre intègre, B son corps des fractions, u : A → B l’injection canonique. Alors $\Omega_0(u) : \Omega_K(A) \otimes_A B \to \Omega_K(B)$ est un isomorphisme.*

Compte tenu de ce que dans le diagramme (42) de III, p. 135, les flèches verticales sont bijectives, tout revient à prouver que pour tout espace vectoriel E sur B, l’application $C(u) : D_K(B, E) \to D_K(A, E)$ est bijective. Mais cela résulte de ce que toute K-dérivation de A dans E se prolonge d’une seule manière en une K-dérivation de B dans E (III, p. 123, prop. 5).

## EXERCICES {#alg-iii-s10-exercises}

See the [exercises for § 10](exercises/s10/).
