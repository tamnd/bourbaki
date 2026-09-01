---
book: alg
book_title: Algebra
chapter: IX
chapter_title: Formes sesquilinéaires et formes quadratiques
section: 8
section_title: Types de formes quadratiques
lang: fr
source: alg-ix-fr
pdf_pages: 0130-0137
extraction: ocr
subsections:
    - "no": 1
      title: Types de formes quadratiques.
      page: 0
      pdf_page: 130
    - "no": 2
      title: Groupe des types de formes quadratiques.
      page: 0
      pdf_page: 132
    - "no": 3
      title: Anneau des types de formes quadratiques.
      page: 0
      pdf_page: 135
statements: 10
exercises: 0
content_sha256: 41114d3659ba1c03e45fbacc1d14e1405e0ae472fba157d2ff91fc89f7b4d7b1
---

## § 8. Types de formes quadratiques

Dans ce paragraphe on suppose que A est un corps commutatif.

### 1. Types de formes quadratiques.

Étant donnée une forme quadratique Q ($§ 3, n° 4$) sur un espace vectoriel E sur A, nous dirons que E est l’espace de défini-

(*) Ces résultats (inédits) nous ont été communiqués par I. Kaplansky.

tion de Q et que dim(E) est la dimension de Q. Étant données deux formes quadratiques Q, Q' sur des espaces vectoriels E, E' sur A, nous noterons Q ⊕ Q' leur somme directe (§ 3, no 4). Rappelons que la somme directe de deux formes neutres est neutre (§ 4, no 2).

Introduisons la relation suivante :

« Q et Q' sont des formes quadratiques non dégénérées de dimensions finies sur A, et il existe des formes quadratiques neutres, N, N' telles que Q ⊕ N soit équivalente à Q' ⊕ N' ».

Cette relation, que nous noterons Q ~ Q', est manifestement réflexive et symétrique. Elle est également transitive : en effet, si Q, Q', Q'' sont des formes quadratiques telles que Q ~ Q' et Q' ~ Q'', il existe des formes quadratiques neutres M, M', N, N' telles que Q ⊕ M soit équivalente à Q' ⊕ M' et Q' ⊕ N à Q'' ⊕ N' ; alors Q ⊕ (M ⊕ N) est équivalente à (Q ⊕ M) ⊕ N, donc à (Q' ⊕ M') ⊕ N, et aussi à (Q' ⊕ N) ⊕ M', donc encore à (Q'' ⊕ N') ⊕ M' et à Q'' ⊕ (N' ⊕ M') ; comme M ⊕ N et N' ⊕ M' sont neutres, on a bien Q ~ Q''. La relation Q ~ Q' est donc une relation d’équivalence entre Q et Q'. Il est clair que, si Q et Q' sont deux formes quadratiques non dégénérées de dimensions finies et équivalentes, on a Q ~ Q'.

Pour toute forme quadratique Q sur A, non dégénérée et de dimension finie, nous poserons

(1)
$$
\theta(Q) = \tau_x(X \sim Q),
$$
et nous dirons que $\theta(Q)$ est le type de Q. Si Q et Q' sont deux formes quadratiques sur A, non dégénérées et de dimensions finies, les relations Q ~ Q' et $\theta(Q) = \theta(Q')$ sont équivalentes.

#### Proposition 1 {#alg-ix-s8-prop-1 .statement}

Soient Q et Q' deux formes quadratiques sur A, non dégénérées et de dimensions finies. Pour que Q et Q' soient équivalentes, il faut et il suffit qu’elles aient même dimension et même type.

La condition est évidemment nécessaire. Supposons-la satisfaite. Il existe alors des formes neutres N, N' telles que Q ⊕ N et Q' ⊕ N' soient équivalentes. Comme ces deux formes ont même dimension, il en est de même de N et N', qui sont par suite équivalentes (§ 4, no 2, cor. 2 de la prop. 2). Donc Q et Q' sont équivalentes en vertu du th. de Witt (§ 4, no 3, cor. 1 du th. 1).

#### Proposition 2 {#alg-ix-s8-prop-2 .statement}

La relation « il existe une forme quadratique Q sur A, non dégénérée et de dimension finie, telle que X = θ(Q) » est collectivisante en X (Ens., chap. II, § 1, n° 4).

Soient en effet V un espace vectoriel de dimension infinie sur A, $\mathfrak{S}$ l’ensemble des formes quadratique non dégénérées définies sur les sous-espaces de dimensions finies de V, et $\mathfrak{W}$ l’ensemble des $\theta(Q)$ pour $Q \in \mathfrak{S}$. Il est clair que toute forme quadratique $Q'$ non dégénérée et de dimension finie sur A est équivalente à au moins un élément de $\mathfrak{S}$; d’où $\theta(Q') \in \mathfrak{W}$, ce qui démontre notre assertion.

### 2. Groupe des types de formes quadratiques.

Nous allons munir l’ensemble $\mathfrak{W}$ des types de formes quadratiques non dégénérées de dimensions finies sur A d’une structure de groupe commutatif. Nous définirons une addition dans $\mathfrak{W}$ par la formule

$$
T + T' = \theta(T \tau T') \tag{2}
$$

Cette addition est commutative puisque $T' \tau T$ est équivalente à $T \tau T'$. Elle est associative car, si $T, T'$ et $T''$ sont des éléments de $\mathfrak{W}$, on a

$$
(T + T') + T'' \sim (T + T') \tau T'' \sim (T \tau T') \tau T''
$$
$$
\sim T \tau (T' \tau T'') \sim T \tau (T' + T'') \sim T + (T' + T''),
$$
d’où $(T + T') + T'' = T + (T' + T'')$ puisque deux éléments de $\mathfrak{W}$ qui ont le même type sont égaux. De plus l’addition que l’on vient de définir possède un élément neutre : il est clair en effet que toutes les formes neutres ont le même type $T_0$, à savoir celui de la forme nulle de dimension nulle ; on voit aussitôt que $T_0$ est l’élément neutre cherché. Enfin l’existence, pour tout $T \in \mathfrak{W}$, d’un élément opposé à T résulte aussitôt de la proposition suivante :

#### Proposition 3 {#alg-ix-s8-prop-3 .statement}

Soit Q une forme quadratique non dégénérée et de dimension finie sur un espace vectoriel V sur A. Notons – Q la forme quadratique sur V définie par $(-Q)(x) = -Q(x)$ ($x \in V$). Alors la forme $Q \tau (-Q)$ est neutre.

En effet la restriction de $Q \tau (-Q)$ à la diagonale D de $V \times V$ est nulle. L’indice de cette forme est donc $\geqslant \frac{1}{2} \dim (V \times V)$ (§ 4, no 2, déf. 2), et par conséquent est égal à $\frac{1}{2} \dim (V \times V)$ (*ibid.*, formule (4)). Il en résulte que $Q \tau (-Q)$ est neutre (*ibid.*).

Ceci permet de poser la définition suivante :

#### Définition 1 {#alg-ix-s8-def-1 .statement}

*L’ensemble des types de formes quadratiques non dégénérées et de dimensions finies sur $A$, muni de l’addition définie par (2), s’appelle le groupe des types de formes quadratiques, ou groupe de Witt, de $A$.*

*Remarques. —* 1) Toute forme quadratique $Q$ non dégénérée et de dimension finie dont le type est nul (c’est-à-dire telle que $\theta(Q) = T_0$ avec les notations ci-dessus) est une forme neutre. Il existe en effet des formes neutres $N, N'$ telles que $Q \tau N$ soit équivalente à $N'$. Ceci montre que $Q$ est de dimension paire, donc qu’il existe une forme neutre $N_1$ de même dimension que $Q$. Comme $Q$ et $N_1$ ont même type, il résulte de la prop. 1 qu’elles sont équivalentes, donc que $Q$ est neutre.

2) Pour toute forme quadratique $Q$ de dimension finie sur $A$, notons $\delta(Q)$ la classe modulo 2 de la dimension de $Q$. On a
$$
\delta(Q \tau Q') = \delta(Q) + \delta(Q').
$$
Comme toute forme neutre $N$ est de dimension paire, on a $\delta(N) = 0$; la relation $Q \sim Q'$ entraîne donc $\delta(Q) = \delta(Q')$. Ainsi la restriction de $\delta$ au groupe $\mathfrak{W}$ des types de formes quadratiques sur $A$ est un homomorphisme de $\mathfrak{W}$ dans le groupe $\mathbf{Z}/(2)$. Cet homomorphisme est surjectif lorsque $A$ est de caractéristique $\neq 2$, mais ne l’est pas si $A$ est de caractéristique 2 car une forme quadratique de dimension impaire est alors dégénérée puisque sa forme bilinéaire associée est alternée (cf. § 5).

3) Soit $a$ un élément $\neq 0$ de $A$. Si $N$ est une forme neutre, il en est de même de $aN$. Il en résulte que la relation $Q \sim Q'$ entraîne $aQ \sim aQ'$. Pour tout élément $T$ du groupe $\mathfrak{W}$, nous poserons
$$
a.T = \theta(aT).
$$
Nous obtenons ainsi une loi de composition externe entre le groupe $A^*$ des éléments non nuls de $A$ et le groupe $\mathfrak{W}$. Les formules suivantes résultent immédiatement de la définition :
$$
a.(T + T') = a.T + a.T', \quad ab.T = a.(b.T)
$$
$$
(a, b \text{ dans } A^*, \quad T, T' \text{ dans } \mathfrak{W}).
$$

Par contre, si $a, b$ et $a + b$ sont dans $A^*$, on n’a pas en général $(a + b).T = a.T + b.T$ ($T \in \mathfrak{W}$).

#### Proposition 4 {#alg-ix-s8-prop-4 .statement}

*Soit Q une forme quadratique non dégénérée sur un espace vectoriel E de dimension finie sur A. Supposons A de caractéristique $\neq 2$, et soit $(x_1, \ldots, x_n)$ une base orthogonale de V. Notons $T_1$ le type de la forme quadratique $Q_1$ définie sur l’espace vectoriel A et telle que $Q_1(1) = 1$. Le type de Q est alors $\sum_{i=1}^n Q(x_i) \cdot T_1$.

En effet la forme Q est équivalente à
$$(Q(x_1)Q_1) \tau \ldots \tau (Q(x_n)Q_1)$$

#### Corollaire {#alg-ix-s8-n2-cor-1 .statement}

*Les hypothèses et notations étant celles de la prop. 3, les éléments $a.T_1$ ($a \in A^*$) forment un ensemble de générateurs du groupe des types de formes quadratiques sur A.*

Chercher la structure du groupe des types de formes quadratiques sur A revient donc à chercher les relations $\mathbf{Z}$-linéaires qui existent entre les éléments de la forme $a.T_1$. Si $b \in A^*$, la forme $Q_1$ définie dans la prop. 4 est manifestement équivalente à $b^2Q_1$; on a donc $a.T_1 = ab^2.T_1$, ce qui montre que $a.T_1$ ne dépend que de la classe de $a$ modulo le sous-groupe $(A^*)^2$ des carrés d’éléments de $A^*$. Par ailleurs il résulte de la prop. 3 que l’on a $(-a).T_1 = -a.T_1$. Cependant il existe en général d’autres relations $\mathbf{Z}$-linéaires entre les $a.T_1$ que celles qui se déduisent des relations que nous venons d’indiquer.

#### Proposition 5 {#alg-ix-s8-prop-5 .statement}

*On suppose que A est un corps ordonné maximal. Soient Q une forme quadratique non dégénérée de dimension finie sur A, et $(s, t)$ sa signature ($§ 7$, no 2, déf. 2). Alors le type de Q est $(s - t).T_1$, et le groupe $\mathfrak{W}$ des types de formes quadratiques sur A est un groupe monogène infini engendré par $T_1$.

En effet, comme $A^*/(A^*)^2$ est d’ordre 2 et que $(-1).T_1 = -T_1$, $\mathfrak{W}$ est engendré par $T_1$ et est par suite monogène. Pour tout $n > 0$, $n.T_1$ est le type des formes quadratiques non dégénérées positives de dimension $n$; comme ces formes ne sont pas neutres, on a $n.T_1 \neq 0$, ce qui montre que $\mathfrak{W}$ est infini. Enfin une forme de signature $(s, t)$ est isomorphe, avec les notations de la prop. 4, à la somme directe de $s$ formes $Q_1$ et de $t$ formes $- Q_1$ (§ 7, n° 2, th. 1); il en résulte que son type est $(s - t). T_1$.

### 3. Anneau des types de formes quadratiques.

Nous supposerons, dans ce n°, que $A$ est un corps de caractéristique $\neq 2$.

Étant données deux formes quadratiques $Q, Q'$ sur des espaces vectoriels $V, V'$ sur $A$, nous appellerons produit tensoriel de $Q$ et $Q'$, et nous noterons $Q \otimes Q'$ la forme quadratique sur $V \otimes V'$ dont la forme bilinéaire associée est le produit tensoriel (§ 1, n° 9, déf. 11) des formes bilinéaires associées à $Q$ et $Q'$. On voit aisément que $Q \otimes Q'$ vérifie la relation

$$(5)$$
$$(Q \otimes Q')(x \otimes x') = Q(x)Q'(x') \quad (x \in V, x' \in V').$$

Si $Q$ et $Q'$ sont non dégénérées et de dimensions finies, il en est de même de $Q \otimes Q'$ (§ 1, n° 9, prop. 9).

Soient $Q, Q', Q''$ des formes quadratiques sur les espaces vectoriels $V, V', V''$. En faisant usage de l’isomorphisme canonique de $V \otimes V'$ sur $V' \otimes V$ (resp. de $(V \otimes V') \otimes V''$ sur $V \otimes (V' \otimes V'')$), de $(V \times V') \otimes V''$ sur $(V \otimes V'') \times (V' \otimes V'')$), on voit aussitôt que $Q \otimes Q'$ est équivalente à $Q' \otimes Q$ (resp. $(Q \otimes Q') \otimes Q''$ à $Q \otimes (Q' \otimes Q'')$, $(Q \tau Q') \otimes Q''$ à $(Q \otimes Q'') \tau (Q' \otimes Q'')$).

Soient $Q$ et $Q'$ deux formes quadratiques non dégénérées de dimensions finies. Si $Q$ est neutre, il en est de même de $Q \otimes Q'$. Soient en effet $V, V'$ les espaces de définition de $Q, Q'$, $2n$ et $n'$ leurs dimensions, et $W$ un sous-espace totalement singulier de dimension $n$ de $V$ (§ 4, n° 2); alors, $W \otimes V'$ est un sous-espace totalement singulier, et sa dimension est la moitié de celle de $V \otimes V'$; on en déduit, comme dans la prop. 3, que $Q \otimes Q'$ est neutre. De même $Q \otimes Q'$ est neutre toutes les fois que $Q'$ est neutre.

On déduit de là que, si $Q, Q', Q_1, Q'_1$ sont des formes quadratiques non dégénérées et de dimensions finies sur $A$, et si l’on suppose que l’on a $\theta(Q_1) = \theta(Q)$ et $\theta(Q'_1) = \theta(Q')$, alors on a $\theta(Q_1 \otimes Q'_1) = \theta(Q \otimes Q')$. Il suffit en effet de vérifier ceci dans le cas où $Q_1 = Q \tau N$ et $Q'_1 = Q' \tau N'$, $N$ et $N'$ étant des formes neutres ; dans ce cas $Q_1 \otimes Q'_1$ est équivalente à

$$
(Q \otimes Q') \tau (Q \otimes N' \tau Q' \otimes N \tau N \otimes N')
$$

et la seconde parenthèse désigne une forme neutre ; ceci démontre notre assertion.

Soit maintenant $\mathfrak{B}$ le groupe des types de formes quadratiques sur $A$. Définissons, sur l’ensemble $\mathfrak{B}$, une seconde loi de composition, notée multiplicativement, par la formule

(6)
$$
TT' = \theta(T \otimes T') \qquad (T, T' \text{ dans } \mathfrak{B}).
$$

Il résulte aussitôt de ce que nous venons de voir que cette loi de composition est commutative, associative et distributive par rapport à l’addition. Elle admet un élément unité, à savoir le type $T_1$ de la forme quadratique $Q_1$ définie sur l’espace vectoriel $A$ et telle que $Q_1(1) = 1$ : on a en effet, d’après (5), $Q_1 \otimes Q = Q$ pour toute forme quadratique $Q$. Le groupe additif $\mathfrak{B}$, muni de la multiplication que nous venons de définir, est donc un anneau commutatif à élément unité ; on l’appelle *anneau des types de formes quadratiques* de $A$ (ou *anneau de Witt* de $A$, lorsqu’aucune confusion n’est à craindre).

#### Remarque 1 {#alg-ix-s8-n3-rem-1 .statement}

Il est clair que, si $a$ est un élément de $A^*$, on a

(7)
$$
a . (TT') = (a . T)T' = T(a . T')
$$

quels que soient les éléments $T, T'$ de $\mathfrak{B}$. On remarquera d’ailleurs que l’on a $a . T = T_a T$, en notant $T_a$ le type de la forme quadratique $aQ_1$ sur $A$.

#### Remarque 2 {#alg-ix-s8-n3-rem-2 .statement}

Puisque $A$ est de caractéristique $\neq 2$, tout élément $T$ de $\mathfrak{B}$ se met sous la forme $\sum_{i=1}^n a_i . T_1$ où $a_i \in A^*$ (no 2, prop. 4). On a

(8)
$$
(\sum_{i=1}^n a_i . T_1)(\sum_{j=1}^q b_j . T_1) = \sum_{i,j} a_i b_j . T_1 \qquad (a_i, b_j \text{ dans } A^*).
$$

#### Remarque 3 {#alg-ix-s8-n3-rem-3 .statement}

Supposons que $A$ soit un *corps ordonné maximal*. Alors l’anneau $\mathfrak{B}$ est isomorphe à $\mathbf{Z}$ (prop. 5), l’entier correspondant au type d’une forme de signature $(s,\ t)$ étant $s - t$ (*ibid.*). Comme le produit tensoriel de deux formes $Q$, $Q'$ de signatures $(s,\ t)$, $(s',\ t')$ est une forme de dimension $(s + t)\,(s' + t')$, il en résulte, au moyen d’un calcul élémentaire, que la signature de $Q \otimes Q'$ est $(ss' + tt',\ st' + ts')$.
