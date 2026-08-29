---
book: ac
book_title: Commutative Algebra
chapter: X
chapter_title: Profondeur, régularité, dualité
section: 6
section_title: Extension des scalaires dans les algèbres régulières
lang: fr
source: ac-x-fr
pdf_pages: 0070-0081, 0168-0169
extraction: ocr
subsections:
    - "no": 1
      title: Algèbres essentiellement de type fini
      page: 0
      pdf_page: 70
    - "no": 2
      title: Produits tensoriels d’algèbres de Macaulay ou de Gorenstein
      page: 72
      pdf_page: 71
    - "no": 3
      title: Extension séparable du corps de base dans les algèbres régulières¹ ou normales
      page: 74
      pdf_page: 73
    - "no": 4
      title: Algèbres absolument régulières ou absolument normales
      page: 75
      pdf_page: 74
    - "no": 5
      title: Caractérisations des algèbres absolument régulières
      page: 78
      pdf_page: 77
statements: 33
exercises: 7
content_sha256: 5ce020b594660b670473a0d1b1f4d34b94ffccaae815319291452fefe8423aae
---

## § 6. EXTENSION DES SCALAires DANS LES ALGÈBRES RÉGULIÈRES

### 1. Algèbres essentiellement de type fini

Soit $k$ un anneau. Soient $A$ une $k$-algèbre et $x = (x_i)_{i \in I}$ une famille d’éléments de $A$; notons $A'$ la sous-algèbre de $A$ engendrée par les $x_i$. Nous dirons que $x$ est une famille essentiellement génératrice de la $k$-algèbre $A$ si, pour tout élément $a$ de $A$, il existe un élément $s$ de $A'$, inversible dans $A$, tel que $sa$ appartienne à $A'$. Il revient au même de dire que, pour tout $a \in A$, il existe des polynômes $P$ et $Q$ de $k[(X_i)_{i \in I}]$ tels que $Q(x)$ soit inversible dans $A$ et que l’on ait $a = P(x)Q(x)^{-1}$.

Nous dirons qu’une $k$-algèbre $A$ est essentiellement de type fini si elle admet une famille essentiellement génératrice finie. Il revient au même de dire qu’il existe une $k$-algèbre $A'$ de type fini et une partie multiplicative $S$ de $A'$ telle que la $k$-algèbre $A$ soit isomorphe à $S^{-1}A'$.

#### Exemple 1 {#ac-x-s6-n1-exa-1 .statement}

Dire qu’une extension $L$ d’un corps $K$ est une $K$-algèbre essentiellement de type fini signifie que c’est une extension de type fini au sens de A, V, p. 11, déf. 2. La $K$-algèbre $L$ n’est de type fini que si c’est une extension de degré fini de $K$ (V, § 3, n° 4, cor. 3 du th. 3).

#### Exemple 2 {#ac-x-s6-n1-exa-2 .statement}

Pour qu’une $k$-algèbre locale soit essentiellement de type fini, il faut et il suffit qu’elle soit isomorphe à une $k$-algèbre de la forme $A_p$, où $A$ est une $k$-algèbre de type fini et $p$ un idéal premier de $A$ (cf. II, § 2, n° 5, prop. 11 (iii)).

#### Proposition 1 {#ac-x-s6-prop-1 .statement}

Si l’anneau $k$ est noethérien, toute $k$-algèbre essentiellement de type fini est un anneau noethérien.

Cela résulte de III, § 2, n° 10, cor. 3 du th. 2 et II, § 2, n° 4, cor. 2 de la prop. 10.

On déduit de la définition les propriétés suivantes :

#### Proposition 2 {#ac-x-s6-prop-2 .statement}

a) Toute algèbre quotient d’une $k$-algèbre essentiellement de type fini est essentiellement de type fini.

b) Tout anneau de fractions d’une $k$-algèbre essentiellement de type fini est une $k$-algèbre essentiellement de type fini.

c) La $k$-algèbre produit d’une famille finie de $k$-algèbres essentiellement de type fini est essentiellement de type fini.

d) Soit $k \to k'$ un homomorphisme d’anneaux ; pour toute $k$-algèbre $A$ essentiellement de type fini, la $k'$-algèbre $A_{(k')} = k' \otimes_k A$ est essentiellement de type fini.

#### Corollaire {#ac-x-s6-n1-cor-1 .statement}

Soient $A$ une $k$-algèbre essentiellement de type fini et $B$ une $k$-algèbre noethérienne. Alors l’anneau $A \otimes_k B$ est noethérien.

En effet, c’est une $B$-algèbre essentiellement de type fini (prop. 2, d)) et on applique la proposition 1.

#### Proposition 3 {#ac-x-s6-prop-3 .statement}

Soient $k$ un anneau, $A$ une $k$-algèbre et $B$ une $A$-algèbre. Si $A$ est essentiellement de type fini sur $k$ et $B$ essentiellement de type fini sur $A$, alors $B$ est essentiellement de type fini sur $k$.

Notons $\rho : A \to B$ l’application canonique. Soient $x = (x_i)_{i \in I}$ une famille essentiellement génératrice finie de la $k$-algèbre $A$ et $A'$ la sous-algèbre qu’elle engendre ; soit $y = (y_j)_{j \in J}$ une famille essentiellement génératrice finie de la $A$-algèbre $B$. Notons $B'$ la sous-$k$-algèbre de $B$ engendrée par les $\rho(x_i)$ et les $y_j$. Soit $b \in B$ ; par hypothèse il existe des polynômes $P$ et $Q$ dans $A[(Y_j)_{j \in J}]$ tels que $Q(y)$ soit inversible dans $B$ et que l’on ait $Q(y) b = P(y)$. Les coefficients non nuls de $P$ et $Q$ sont en nombre fini ; il existe un polynôme $R \in k[(X_i)_{i \in I}]$ tel que $R(x)$ soit inversible dans $A$ et que $R(x) P$ et $R(x) Q$ appartiennent à $A'[(Y_j)_{j \in J}]$. Alors $\rho(R(x)) Q(y)$ est inversible dans $B$, et l’on a

$$
\rho(R(x)) Q(y) b = \rho(R(x)) P(y) \in B'.
$$

Ainsi les éléments $\rho(x_i)$ pour $i \in I$ et $y_j$ pour $j \in J$ forment une famille essentiellement génératrice finie de la $k$-algèbre $B$.

#### Corollaire {#ac-x-s6-n1-cor-2 .statement}

Le produit tensoriel de deux $k$-algèbres essentiellement de type fini est une $k$-algèbre essentiellement de type fini.

Soient en effet $A$ et $B$ deux $k$-algèbres essentiellement de type fini. Alors $A \otimes_k B$ est essentiellement de type fini sur $A$ (prop. 2, d)) donc sur $k$ (prop. 3).

### 2. Produits tensoriels d’algèbres de Macaulay ou de Gorenstein

#### Proposition 4 {#ac-x-s6-prop-4 .statement}

Soient $k$ un corps, $A$ une $k$-algèbre essentiellement de type fini et $B$ une $k$-algèbre.

a) Si $A$ et $B$ sont des anneaux de Macaulay, il en est de même de $A \otimes_k B$.

b) Si $A$ et $B$ sont des anneaux de Gorenstein, il en est de même de $A \otimes_k B$.

Supposons que $A$ et $B$ soient des anneaux de Macaulay (resp. de Gorenstein) et prouvons qu’il en est de même de $A \otimes_k B$. L’anneau $A \otimes_k B$ est noethérien (n° 1, cor. de la prop. 2). Le $A$-module $A \otimes_k B$ est libre, donc plat. D’après la prop. 10 du § 2, n° 7 (resp. le cor. 1 de la prop. 12 du § 3, n° 8), il nous suffit de prouver que $\kappa(p) \otimes_k B$ est un anneau de Macaulay (resp. de Gorenstein) pour tout idéal premier $p$ de $A$. L’extension $\kappa(p)$ de $k$ est de type fini (n° 1, prop. 2 et exemple 1) ; nous sommes donc ramenés à démontrer l’énoncé dans le cas où la $k$-algèbre $A$ est une extension de type fini $K$ de $k$.

L’anneau $K \otimes_k B$ est alors un $B$-module libre de rang fini, donc un $B$-module macaulayen. D’après le § 2, n° 6, cor. 1 de la prop. 8, c’est un anneau de Macaulay, ce qui prouve a). Supposons maintenant que $B$ soit un anneau de Gorenstein. Il existe des sous-extensions $K_i,\ 0 \leq i \leq m$, de $K$ avec

$$
k = K_0 \subset K_1 \subset \cdots \subset K_m = K
$$

telles que $K_i$ soit une $K_{i-1}$-algèbre monogène pour $i = 1, \ldots, m$, et cela nous permet de nous ramener au cas où l’extension $K$ de $k$ est monogène (de degré fini). L’homomorphisme canonique $B \to K \otimes_k B$ fait de $K \otimes_k B$ une $B$-algèbre plate et, pour tout $q \in \mathrm{Spec}(B)$, l’anneau $(K \otimes_k B) \otimes_B \kappa(q)$, isomorphe à $K \otimes_k \kappa(q)$, est une $\kappa(q)$-algèbre monogène, donc un anneau de Gorenstein ($§ 3$, n° 9, exemple 5). Ainsi $K \otimes_k B$ est un anneau de Gorenstein ($§ 3$, n° 8, cor. 1 de la prop. 12), ce qui achève de prouver b).

#### Corollaire 1 {#ac-x-s6-prop-4-cor-1 .statement}

Soient $k$ un corps, $K$ une extension de $k$ et $\Lambda$ une $k$-algèbre essentiellement de type fini. Pour que $A_{(K)}$ soit un anneau de Macaulay (resp. de Gorenstein), il faut et il suffit qu’il en soit de même de $A$.

Si $A$ est un anneau de Macaulay (resp. de Gorenstein), il en est de même de $A_{(K)}$ d’après la prop. 4. Puisque $A_{(K)}$ est un $A$-module fidèlement plat, la réciproque résulte de la prop. 10 du § 2, n° 7 (resp. du cor. 1 de la prop. 12 du § 3, n° 8).

#### Corollaire 2 {#ac-x-s6-prop-4-cor-2 .statement}

Soient $k$ un anneau noethérien, $A$ et $B$ des $k$-algèbres. On suppose que $A$ est plate et essentiellement de type fini sur $k$. Si $A$ et $B$ sont des anneaux de Macaulay (resp. de Gorenstein), alors $A \otimes_k B$ est un anneau de Macaulay (resp. de Gorenstein).

Supposons d’abord que $B$ soit un corps ; notons $\varphi$ l’homomorphisme canonique de $k$ dans $B$, et $r$ son noyau. L’homomorphisme $\varphi$ induit un homomorphisme du corps des fractions $\kappa(r)$ de $k/r$ dans $B$. Alors $A \otimes_k B$ s’identifie à $(A \otimes_k \kappa(r)) \otimes_{\kappa(r)} B$; comme $\varphi^{-1}(0) = r$, l’anneau $A \otimes_k \kappa(r)$ est un anneau de Macaulay (resp. de Gorenstein) d’après la prop. 10 du § 2, n° 7 (resp. le cor. 1 de la prop. 12 du § 3, n° 8). L’assertion résulte dans ce cas du cor. 1.

Passons au cas général. La $B$-algèbre $A \otimes_k B$ est plate, et noethérienne par le cor. de la prop. 2 du n° 1. Pour chaque idéal premier $q$ de $B$, l’anneau $(A \otimes_k B) \otimes_B \kappa(q)$, qui s’identifie à $A \otimes_k \kappa(q)$, est un anneau de Macaulay (resp. de Gorenstein) d’après ce qui précède. On conclut en appliquant la prop. 10 du § 2, n° 7 (resp. le cor. 1 de la prop. 12 du § 3, n° 8).

### 3. Extension séparable du corps de base dans les algèbres régulières¹ ou normales

#### Lemme 1 {#ac-x-s6-lem-1 .statement}

Soit $A$ un anneau noethérien, réunion d’une famille filtrante croissante $(A_\alpha)_{\alpha \in I}$ de sous-anneaux noethériens.

a) Si les anneaux $A_\alpha$ sont réguliers et si $A$ est un $A_\alpha$-module plat pour tout $\alpha \in I$, l’anneau $A$ est régulier.

b) Si les anneaux $A_\alpha$ sont normaux ($§ 1$, n° 8), $A$ est normal.

a) Soit $m$ un idéal maximal de $A$; pour tout $\alpha \in I$, notons $m_\alpha$ l’idéal $m \cap A_\alpha$ de $A_\alpha$. Puisque $A$ est noethérien, $m$ est de type fini et il existe un élément $\alpha$ de $I$ tel que $m = A m_\alpha$, de sorte que le $A$-module $(A_\alpha / m_\alpha) \otimes_{A_\alpha} A$ est isomorphe à $A / m$. Comme $A$ est plat sur $A_\alpha$, on a $\mathrm{dp}_A(A/m) \leq \mathrm{dp}_{A_\alpha}(A_\alpha / m_\alpha)$ (A, X, p. 141, lemme 2). Puisque les anneaux $A_\alpha$ sont réguliers, il en résulte que $A$ est régulier ($§ 4$, n° 2, prop. 4).

b) Puisque les $A_\alpha$ sont réduits, $A$ est réduit. Soient $a$ et $b$ des éléments de $A$ tels que $b$ ne soit pas diviseur de zéro et que l’élément $a/b$ de l’anneau total des fractions de $A$ soit entier sur $A$. Il existe un polynôme unitaire $P \in A[X]$ tel que $P(a/b) = 0$. Soit $\alpha$ un élément de $I$ tel que l’anneau $A_\alpha$ contienne $a$, $b$ et les coefficients de $P$. Puisque $A_\alpha$ est normal, il existe $c \in A_\alpha$ tel que $a = bc$. Ainsi $a/b = c$ appartient à $A$ et $A$ est normal.

#### Lemme 2 {#ac-x-s6-lem-2 .statement}

Soient $k$ un corps, $K$ et $L$ des extensions de $k$. On suppose que $K$ est de type fini et que l’une des extensions $K$ ou $L$ est séparable. Alors l’anneau $K \otimes_k L$ est régulier.

Notons $A$ l’anneau $K \otimes_k L$; il est noethérien d’après le cor. de la prop. 2 (n° 2). Supposons d’abord que l’extension $K$ soit séparable. D’après A, V, p. 130, corollaire; il existe une base de transcendance $t = (t_1, \ldots, t_n)$ de $K$ telle que $K$ soit une extension finie séparable de l’extension pure $k(t)$. L’anneau $E = k(t) \otimes_k L$, isomorphe à un anneau de fractions d’un anneau de polynômes sur $L$, est régulier ($§ 4$, n° 2, cor. 5 de la prop. 4); pour tout idéal premier $p$ de $E$, l’anneau $\kappa(p) \otimes_E A$ est isomorphe à $\kappa(p) \otimes_{k(t)} K$, donc à un produit fini de corps (A, V, p. 35, déf. 1, p. 34, th. 4, et p. 33, prop. 5). Puisque $A$ est un $E$-module libre, c’est un anneau régulier d’après le cor. de la prop. 9 du $§ 4$, n° 5.

Supposons maintenant que $L$ soit séparable sur $k$. D’après la première partie de la démonstration, l’anneau $K \otimes_k L'$ est régulier pour toute sous-extension de type fini $L'$ de $L$. On conclut en appliquant le lemme 1.

#### Proposition 5 {#ac-x-s6-prop-5 .statement}

Soient $k$ un corps, $A$ une $k$-algèbre et $K$ une extension de $k$. Supposons que $A$ soit essentiellement de type fini ou que l’extension $K$ soit de type fini.

¹ Dans ce numéro, une algèbre sur un corps $k$ est dite régulière si c’est un anneau régulier. En particulier, toute extension de $k$ est une algèbre régulière. On évitera de confondre cette notion avec celle d’extension régulière, introduite en A, V, p. 135, déf. 2, qui n’interviendra pas ici.

a) Si l’anneau $A_{(K)}$ est régulier (resp. normal), l’anneau $A$ est régulier (resp. normal).

b) Si l’anneau $A$ est régulier (resp. normal) et si l’extension $K$ de $k$ est séparable, l’anneau $A_{(K)}$ est régulier (resp. normal).

Le $A$-module $A_{(K)}$ est libre, donc fidèlement plat ; l’assertion a) résulte donc du cor. de la prop. 8 de I, § 3, n° 5 et de la prop. 8 du § 4, n° 5 (resp. du cor. 2 du th. 4 du § 1, n° 10). Sous les hypothèses de b), pour tout idéal premier $\mathfrak{p}$ de $A$, l’anneau $\kappa(\mathfrak{p}) \otimes_k K$ est régulier (lemme 2), et $a fortiori$ normal (§ 4, n° 2, cor. 2 de la prop. 4). L’assertion b) résulte donc du cor. de la prop. 9 du § 4, n° 5 (resp. du cor. 3 du th. 4 du § 1, n° 10).

### 4. Algèbres absolument régulières ou absolument normales

#### Définition 1 {#ac-x-s6-def-1 .statement}

Soient $k$ un corps et $A$ une $k$-algèbre. On dit que $A$ est absolument régulière (resp. absolument normale)$^1$ si l’anneau $A_{(k')}$ est régulier (resp. normal) pour toute extension $k'$ radicielle et de degré fini de $k$.

Toute $k$-algèbre absolument régulière (resp. absolument normale) est régulière (resp. normale), comme on le voit en prenant $k' = k$ dans la définition 1. Rappelons que les $k$-algèbres $A$ telles que l’anneau $A_{(k')}$ soit réduit pour toute extension $k'$ radicielle et de degré fini de $k$ sont les $k$-algèbres séparables (A, V, p. 117, th. 2).

#### Exemple 1 {#ac-x-s6-n4-exa-1 .statement}

Si $k$ est parfait, toute $k$-algèbre régulière (resp. normale) est absolument régulière (resp. absolument normale).

#### Exemple 2 {#ac-x-s6-n4-exa-2 .statement}

Soit $A$ une $k$-algèbre artinienne. Si $A$ est normale, elle est réduite, donc isomorphe à un produit fini d’extensions de $k$ (A, VIII, § 8, n° 1, prop. 2). Les conditions suivantes sont équivalentes :

A est séparable ;
— A est absolument régulière ;
— A est absolument normale.

En effet, si $A$ est absolument normale, elle est séparable ; si $A$ est séparable, pour toute extension finie $k'$ de $k$, l’anneau $A_{(k')}$ est réduit et artinien, donc isomorphe à un produit de corps, et par suite régulier, de sorte que $A$ est absolument régulière.

Si de plus la $k$-algèbre $A$ est de degré fini, les conditions précédentes équivalent encore à dire que $A$ est étale (A, V, p. 34, th. 4).

#### Exemple 3 {#ac-x-s6-n4-exa-3 .statement}

Soit $A$ une $k$-algèbre locale régulière. Si l’extension $\kappa_A$ de $k$ est séparable, l’algèbre $A$ est absolument régulière. Soit en effet $k'$ une extension de degré fini de $k$. Le $A$-module $A_{(k')}$ est libre. Puisqu’il est de type fini, chaque idéal maximal de $A_{(k')}$ est au-dessus de $\mathfrak{m}_A$ (V, § 2, n° 1, prop. 1). L’anneau $\kappa_A \otimes_A A_{(k')}$, isomorphe à $\kappa_A \otimes_k k'$, est régulier (n° 3, lemme 2). D’après le cor. de la prop. 9 du § 4, n° 5, l’anneau $A_{(k')}$ est régulier, ce qui prouve que la $k$-algèbre $A$ est absolument régulière.

$^1$ Certains auteurs utilisent la terminologie « géométriquement régulière » (resp. « géométriquement normale ».

#### Proposition 6 {#ac-x-s6-prop-6 .statement}

Soient k un corps et A une k-algèbre noethérienne.

a) Si A est absolument régulière (resp. absolument normale, resp. séparable), il en est de même de S$^{-1}$A pour toute partie multiplicative S de A.

b) Si $A_m$ est absolument régulière (resp. absolument normale, resp. séparable), pour tout idéal maximal m de A, alors A est absolument régulière (resp. absolument normale, resp. séparable).

a) Cela résulte de ce que l’anneau $(S^{-1}A)_{(k')}$ est isomorphe à un anneau de fractions de l’anneau $A_{(k')}$ pour toute extension $k'$ de k.

b) Supposons que $A_m$ soit absolument régulière (resp. absolument normale, resp. séparable) pour tout idéal maximal m de A. Soit $k'$ une extension radicielle de k de degré fini et soit $m'$ un idéal maximal de $A_{(k')}$. Il s’agit de vérifier que l’anneau local $(A_{(k')})_{m'}$ est régulier (resp. normal, resp. réduit).

L’homomorphisme canonique $A \to A_{(k')}$ fait de $A_{(k')}$ une A-algèbre finie. L’idéal $m'$ est au-dessus d’un idéal maximal m de A (V, § 2, n° 1, prop. 1) et $(A_{(k')})_{m'}$ est isomorphe à un anneau de fractions de l’anneau régulier (resp. normal, resp. réduit) $(A_m)_{(k')}$, donc est régulier (resp. normal, resp. réduit).

#### Lemme 3 {#ac-x-s6-lem-3 .statement}

Soient k un corps et K une extension de type fini de k. Il existe une extension L de K, de degré fini, et une sous-k-extension $k'$ de L, radicielle et de degré fini sur k, telles que l’extension L de $k'$ soit séparable.

Choisissons une extension composée E de K et d’une clôture parfaite $\hat{k}$ de k, et des éléments $(t_1, \ldots, t_n)$ de E tels que E soit une extension algébrique séparable de $\hat{k}(t_1, \ldots, t_n)$ (A, V, p. 130, cor.). Soit I une partie génératrice finie de K sur k. Le corps $\hat{k}(t_1, \ldots, t_n)$ (resp. $\hat{k}K$) est réunion des sous-corps $k'(t_1, \ldots, t_n)$ (resp. $k'K$), où $k'$ parcourt l’ensemble des sous-extensions de $\hat{k}$ de degré fini sur k ; on peut donc trouver une telle sous-extension $k'$ telle que les éléments $t_1, \ldots, t_n$ de E = $\hat{k}K$ appartiennent à $k'K$ et que chaque élément de I soit algébrique et séparable sur $k'(t_1, \ldots, t_n)$. Alors L = $k'K$ est une extension séparable de $k'$, de degré fini sur K, et $k'$ est une extension radicielle de degré fini de k.

#### Proposition 7 {#ac-x-s6-prop-7 .statement}

Soient k un corps, A et B des k-algèbres dont l’une est essentiellement de type fini. Supposons que A soit absolument régulière (resp. absolument normale). Si l’anneau B est régulier (resp. normal), il en est de même de l’anneau $A \otimes_k B$.

Soit K une extension de type fini de k ; prouvons que l’anneau $A_{(K)}$ est régulier (resp. normal). Considérons en effet des extensions L et $k'$ ayant les propriétés du lemme 3. Alors l’anneau $A_{(k')}$ est régulier (resp. normal) par définition, et l’anneau $A_{(L)}$, qui s’identifie à $A_{(k')} \otimes_{k'} L$, est régulier (resp. normal) d’après la prop. 5, b) du n° 3. Par conséquent, $A_{(K)}$ est régulier (resp. normal) d’après la prop. 5, a).

Supposons l’anneau B régulier (resp. normal) et démontrons la proposition. L’homomorphisme canonique $B \to A \otimes_k B$ fait de $A \otimes_k B$ un B-module libre. Pour tout idéal premier $p$ de B, l’anneau $(A \otimes_k B) \otimes_B \kappa(p)$ s’identifie à $A \otimes_k \kappa(p)$ ; d’après le corollaire de la prop. 9 du § 4, n° 5 (resp. le cor. 3 du th. 4 du § 1, n° 10), il nous suffit de prouver que $A \otimes_k \kappa(p)$ est régulier (resp. normal) pour tout idéal premier $p$ de B.

Si la $k$-algèbre $B$ est essentiellement de type fini, l’extension $\kappa(p)$ de $k$ est de type fini et l’anneau $A \otimes_k \kappa(p)$ est régulier (resp. normal) d’après ce qu’on a vu plus haut. Supposons maintenant la $k$-algèbre $A$ essentiellement de type fini ; l’anneau $A \otimes_k \kappa(p)$ est noethérien et réunion de la famille filtrante croissante des sous-anneaux noethériens $\Lambda \otimes_k K$, où $K$ parcourt les sous-extensions de type fini de $\kappa(p)$. Ces derniers sont réguliers (resp. normaux), et on applique le lemme 1 du n° 3.

#### Corollaire 1 {#ac-x-s6-prop-7-cor-1 .statement}

Soit $k$ un corps. Le produit tensoriel de deux $k$-algèbres absolument régulières (resp. absolument normales) dont l’une est essentiellement de type fini, est une $k$-algèbre absolument régulière (resp. absolument normale).

Soient $A$ et $B$ deux $k$-algèbres satisfaisant aux hypothèses du corollaire. Soit $k'$ une extension radicielle de $k$ de degré fini. L’anneau $B_{(k')}$ est régulier (resp. normal) ; l’anneau $A \otimes_k B_{(k')}$ est régulier (resp. normal) d’après la prop. 7, ainsi que l’anneau $(A \otimes_k B) \otimes_k k'$ qui lui est isomorphe.

#### Corollaire 2 {#ac-x-s6-prop-7-cor-2 .statement}

Soient $k$ un corps, $A$ une $k$-algèbre absolument régulière (resp. absolument normale) et $K$ une extension de $k$. Supposons que $A$ soit essentiellement de type fini ou que l’extension $K$ de $k$ soit de type fini.

a) L’anneau $\Lambda_{(K)}$ est régulier (resp. normal).

b) Si l’extension $K$ de $k$ est séparable, la $k$-algèbre $A_{(K)}$ est absolument régulière (resp. absolument normale).

L’assertion a) résulte de la proposition 7 ; l’assertion b) résulte du cor. 1 et de l’exemple 2.

#### Corollaire 3 {#ac-x-s6-prop-7-cor-3 .statement}

Soient $k$ un corps, $A$ une $k$-algèbre et $K$ une extension de $k$. Supposons que la $k$-algèbre $A$ soit essentiellement de type fini ou que l’extension $K$ de $k$ soit de type fini. Pour que la $k$-algèbre $A$ soit absolument régulière (resp. absolument normale), il faut et il suffit qu’il en soit ainsi de la $K$-algèbre $A_{(K)}$.

Supposons $A$ absolument régulière (resp. absolument normale) et soit $K'$ une extension radicielle de $K$ de degré fini. L’anneau $K' \otimes_K \Lambda_{(K)}$, isomorphe à $K' \otimes_k A$, est régulier (resp. normal) d’après le cor. 2.

Supposons inversement la $K$-algèbre $A_{(K)}$ absolument régulière (resp. absolument normale) et soit $k'$ une extension radicielle de $k$ de degré fini. Soit $L$ une extension composée de $k'$ et de $K$ ; alors l’anneau $A_{(L)}$ s’identifie à $L \otimes_K \Lambda_{(K)}$, donc est régulier (resp. normal) ; par suite, l’anneau $A_{(k')}$ est régulier (resp. normal) d’après la prop. 5, a) du n° 3.

#### Corollaire 4 {#ac-x-s6-prop-7-cor-4 .statement}

Soient $k$ un corps, $A$ une $k$-algèbre essentiellement de type fini et $K$ une extension de $k$ qui soit un corps parfait. Pour que $A$ soit absolument régulière (resp. absolument normale), il faut et il suffit que l’anneau $A_{(K)}$ soit régulier (resp. normal).

Cela résulte du cor. 3 et de l’exemple 1.

### 5. Caractérisations des algèbres absolument régulières

#### Proposition 8 {#ac-x-s6-prop-8 .statement}

Soient k un corps et A une k-algèbre essentiellement de type fini. Notons I le noyau de l’homomorphisme de k-algèbres $\mu : A \otimes_k A \to A$ tel que $\mu(x \otimes y) = xy$ pour x et y dans A. Les conditions suivantes sont équivalentes :

(i) la k-algèbre A est absolument régulière ;
(ii) pour toute k-algèbre régulière C, l’anneau $A \otimes_k C$ est régulier ;
(iii) l’anneau $A \otimes_k A$ est régulier ;
(iv) l’idéal I de $A \otimes_k A$ est complètement sécant ($§ 5$, n° 1, déf. 1).

Notons B l’anneau $A \otimes_k A$ et munissons-le de la structure de A-algèbre déduite de l’homomorphisme $\rho : A \to A \otimes_k A$ tel que $\rho(x) = x \otimes 1$; alors $\mu$ est un homomorphisme de A-algèbres, et induit par passage au quotient un isomorphisme de $B/I$ sur A.

(i) $\Rightarrow$ (ii) : cela résulte de la prop. 7.
(ii) $\Rightarrow$ (iii) : il suffit d’appliquer (ii) avec $C = k$, puis avec $C = \Lambda$.
(iii) $\Rightarrow$ (iv) : le A-module B est libre, donc fidèlement plat. Si l’anneau B est régulier, A est régulier ($§ 4$, n° 5, prop. 8) ; l’idéal I est alors complètement sécant ($§ 5$, n° 3, prop. 2).
(iv) $\Rightarrow$ (i) : supposons l’idéal I complètement sécant et prouvons d’abord que A est régulier. Soit m un idéal maximal de A et soit $\nu : (A/m) \otimes_k A \to A/m$ l’homomorphisme déduit de $\mu$. L’idéal maximal $n = \mathrm{Ker}\,\nu$ est égal à $1((A/m) \otimes_k \Lambda)$; appliquant la prop. 6 du $§ 5$, n° 6 à la A-algèbre $A' = A/m$, on voit que l’idéal n est complètement sécant dans $(\Lambda/m) \otimes_k \Lambda$. Par conséquent ($§ 5$, n° 3, prop. 3) l’anneau local $((A/m) \otimes_k \Lambda)_n$ est régulier. Notons $j : \Lambda \to (A/m) \otimes_k A$ l’homomorphisme $x \mapsto 1 \otimes x$; puisque $\nu \circ j$ est l’homomorphisme canonique de A dans $A/m$, on a $j^{-1}(n) = m$. Ainsi j se prolonge en un homomorphisme local d’anneaux locaux de $A_m$ dans $((A/m) \otimes_k A)_n$, qui fait de ce dernier un $A_m$-module fidèlement plat. D’après la prop. 8 du $§ 4$, n° 5, l’anneau $A_m$ est donc régulier. Nous avons ainsi prouvé que A est régulier.

Soit maintenant $k'$ une extension de k. Le noyau de l’application $\mu' : A_{(k')} \otimes_{k'} \Lambda_{(k')} \to A_{(k')}$ déduite de la multiplication de $A_{(k')}$ n’est autre que $IA_{(k')}$; il est donc complètement sécant dans $A_{(k')}$ ($§ 5$, n° 6, prop. 6). La $k'$-algèbre $A_{(k')}$ satisfait donc à la condition (iv) ; d’après ce qu’on vient de voir, elle est régulière, et cela prouve (i).

Rappelons (A, III, p. 133-134) que le quotient $I/I^2$ muni de la structure de A-module déduite de $\rho$ est noté $\Omega_k(A)$ et appelé le module des k-différentielles de A. Lorsque la k-algèbre A est essentiellement de type fini, l’anneau $A \otimes_k A$ est noethérien, de sorte que le A-module $\Omega_k(A)$ est de type fini.

On note $d_{A/k}$ ou simplement d l’application k-linéaire de A dans $\Omega_k(A)$ qui associe à un élément x de A la classe de $x \otimes 1 - 1 \otimes x$ dans $\Omega_k(A)$. L’application d est une k-dérivation ; pour tout A-module M et toute k-dérivation D : A $\to$ M, il existe une unique application A-linéaire $g : \Omega_k(\Lambda) \to M$ telle que $D = g \circ d$ (loc. cit., prop. 18).

Si S est une partie multiplicative de A, l’application S^{-1}A-linéaire canonique (loc. cit., p. 136)
$$
S^{-1}\Omega_k(A) \to \Omega_k(S^{-1}A)
$$
est bijective : en effet, il suffit de vérifier que, pour tout S^{-1}A-module M, toute k-dérivation D : A \to M se prolonge de manière unique en une k-dérivation D : S^{-1}A \to M ; or cela résulte du raisonnement de loc. cit., p. 123, prop. 5.

Soient k un corps et A une k-algèbre locale essentiellement de type fini. Posons n = \dim(A) + \deg.\mathrm{tr}_k(\kappa_A). Soient B une k-algèbre de type fini et q un idéal premier de B tels que la k-algèbre A soit isomorphe à B_q (cf. n° 1, exemple 2) ; on a n = \dim_q(B) (VIII, § 2, n° 4, cor. 5 du th. 3). D’après loc. cit., th. 3, c) et cor. 5, on a aussi
$$
n = \sup \deg.\mathrm{tr}_k(\kappa(\mathfrak{p}))
$$
où \mathfrak{p} parcourt la famille (finie) des idéaux premiers minimaux de A. Si A est intègre, n est donc le degré de transcendance du corps des fractions de A.

#### Théorème 1 {#ac-x-s6-thm-1 .statement}

*Soient k un corps et A une k-algèbre locale essentiellement de type fini. Posons n = \dim(A) + \deg.\mathrm{tr}_k(\kappa_A).*

a) *On a [\kappa_A \otimes_A \Omega_k(A) : \kappa_A] \geq n.*

b) *Les conditions suivantes sont équivalentes :*
(i) *la k-algèbre A est absolument régulière ;*
(ii) *le A-module \Omega_k(A) est libre de rang n ;*
(iii) *on a [\kappa_A \otimes_A \Omega_k(A) : \kappa_A] = n.*

Considérons l’assertion
(iii') *on a [\kappa_A \otimes_A \Omega_k(A) : \kappa_A] \leq n ;*
il est clair que (ii) implique (iii) et que (iii) implique (iii'). Pour démontrer le théorème il suffit de prouver les implications (i) \Rightarrow (ii) et (iii') \Rightarrow (i).

Choisissons une k-algèbre de type fini B et un idéal premier q de B tels que A soit isomorphe à B_q (n° 1, exemple 2). On a \dim_q(B) = n ; remplaçant B par un anneau B_f , avec f \in B - q, on peut imposer que le spectre de B est connexe et de dimension n, ce que nous supposerons désormais.

(i) \Rightarrow (ii) : Supposons la k-algèbre A absolument régulière. Comme dans la démonstration de la prop. 8, notons \mu : A \otimes_k A \to A et \nu : \kappa_A \otimes_k A \to \kappa_A les homomorphismes déduits de la multiplication de A ; posons I = \mathrm{Ker}(\mu) et n = \mathrm{Ker}(\nu). L’idéal I est complètement sécant ; l’idéal n est maximal et l’anneau local (\kappa_A \otimes_k A)_n est régulier (loc. cit.). D’après le théorème 1 du § 5, n° 2, le A-module de type fini I/I^2, qui n’est autre que \Omega_k(A), est projectif, donc libre. Mais d’après la remarque du § 5, n° 6, l’idéal n s’identifie à \kappa_A \otimes_A 1, de sorte que n/n^2 est isomorphe à \kappa_A \otimes_A \Omega_k(A). On a donc
$$
\mathrm{rg}(\Omega_k(A)) = [\kappa_A \otimes_k \Omega_k(A) : \kappa_A] = [n/n^2 : \kappa_A] = \dim(\kappa_A \otimes_k A)_n .
$$

Désignons par B' l’anneau \kappa_A \otimes_k B, et par S l’image dans B' de B - q. L’anneau \kappa_A \otimes_k A s’identifie à B' \otimes_B B_q, c’est-à-dire à S^{-1}B'. Il existe donc un idéal maximal q' de B' ne rencontrant pas S tcl que l’on ait n = S^{-1}q' ; l’anneau (\kappa_A \otimes_k A)_n est alors isomorphe à B'_{q'} , et l’on a

$$
\dim(\kappa_A \otimes_k A)_n = \dim(\kappa_A \otimes_k B)_{q'} = \dim_{q'}(\kappa_A \otimes_k B)
$$

Comme n contient \kappa_A \otimes_k qB_q , q' contient l’idéal \kappa_A \otimes q de B' , donc son image réciproque dans B contient q ; elle est égale à q puisque q' ne rencontre pas S . D’après VIII, § 2, n° 4, cor. de la prop. 5, on a

$$
\dim_{q'}(\kappa_A \otimes_k B) = \dim_q(B) = n ,
$$

ce qui prouve (ii).

(iii') \Rightarrow (i) : Supposons que l’on ait [\kappa_A \otimes_A \Omega_k(\Lambda) : \kappa_A] \leq n , c’est-à-dire [\kappa(q) \otimes_B \Omega_k(B) : \kappa(q)] \leq n , et prouvons que la k-algèbre B est absolument régulière. Soit (x_1, \ldots , x_n) une suite d’éléments de B telle que 1 \otimes dx_1, \ldots , 1 \otimes dx_n engendrent le \kappa(q)-espace vectoriel \kappa(q) \otimes_B \Omega_k(B) . Remplaçant B par B_f , pour un élément f convenable de B - q , on peut supposer que dx_1, \ldots , dx_n engendrent le B-module \Omega_k(B) (lemme de Nakayama et II, § 5, n° 1, prop. 2). Soit \bar{k} une extension algébriquement close de k . Il nous suffit de prouver que la \bar{k}-algèbre B_{(\bar{k})} est régulière, puisque cela impliquera que B est absolument régulière (cor. 4 de la prop. 7 du n° 4). Pour tout composant canonique C de B_{(k)} , les différentielles d(1 \otimes x_i) engendrent le C-module \Omega_{\bar{k}}(C) (A, III, § 10, n° 12, prop. 20). Le théorème résulte donc des deux lemmes suivants :

#### Lemme 4 {#ac-x-s6-lem-4 .statement}

Soient k un corps, K une extension algébrique de k , B une k-algèbre dont le spectre est connexe. Pour tout composant canonique C de B_{(K)} , on a \dim(C) = \dim(B) .

Traitons d’abord le cas où l’extension K est de degré fini sur k . Le B-module C est facteur direct d’un module libre, donc projectif de type fini. Comme la fonction p \mapsto \mathrm{rg}_p C est constante sur Spec(B) (II, § 5, n° 3), le support du B-module C est égal à Spec(B) , de sorte que le B-module C est fidèlement plat. Cela entraîne \dim(C) \geq \dim(B) (VIII, § 2, n° 1, prop. 2), d’où l’égalité cherchée puisqu’on a \dim(C) \leq \dim(B_{(K)}) = \dim(B) (VIII, § 2, n° 4, cor. de la prop. 5).

Passons au cas général. Soit e l’élément idempotent de B_{(K)} tel que C = B_{(K)}/B_{(K)}e . Il existe une sous-extension K' de K de degré fini tel que e soit l’image d’un élément idempotent e' de B_{(K')} . Posons C' = B_{(K')}/B_{(K')}e' . L’anneau C' \otimes_{K'} K s’identifie à C , et C' est un composant canonique de B_{(K')} . On a \dim(C') = \dim(B) d’après le cas déjà traité, et \dim(C') = \dim(C) d’après loc. cit. , d’où le lemme.

#### Lemme 5 {#ac-x-s6-lem-5 .statement}

Soient k un corps algébriquement clos, A une k-algèbre de type fini dont le spectre est connexe, n un entier et (x_1, \ldots , x_n) une suite finie d’éléments de A . On suppose que A est de dimension n et que les différentielles dx_1, \ldots , dx_n engendrent le A-module \Omega_k(A) . Alors l’anneau A est intègre et régulier et le A-module \Omega_k(A) est libre de base (dx_1, \ldots , dx_n) .

Soit m un idéal maximal de A tel que \dim(A_m) = n . On a [A/m : k] = 1 (V, § 3, n° 3, prop. 1 (iii)), donc A = m \oplus k1_A . Notons p et q les projecteurs correspondants. Pour $a$ et $b$ dans $\Lambda$, on a
$$
ab = (p(a)q(b) + q(a)p(b) + p(a)p(b), q(a)q(b)) ,
$$
d’où $p(ab) \equiv p(a)q(b) + q(a)p(b) \pmod{\mathfrak{m}^2}$. Par conséquent l’application $\delta : \Lambda \to \mathfrak{m}/\mathfrak{m}^2$ qui associe à chaque élément $x$ de $\Lambda$ la classe de $p(x)$ modulo $\mathfrak{m}^2$ est une $k$-dérivation de $\Lambda$ dans le $k$-espace vectoriel $\mathfrak{m}/\mathfrak{m}^2$. Il existe donc une application $\Lambda$-linéaire $\phi : \Omega_k(\Lambda) \to \mathfrak{m}/\mathfrak{m}^2$ telle que $\delta(x) = \phi(dx)$ pour tout $x \in \Lambda$. Puisque $\delta$ est surjective, les $\phi(dx_i)$ engendrent le $\Lambda/\mathfrak{m}$-espace vectoriel $\mathfrak{m}/\mathfrak{m}^2$, et on a $[\mathfrak{m}/\mathfrak{m}^2 : \Lambda/\mathfrak{m}] \leq n = \dim(A_{\mathfrak{m}})$. Il en résulte que $A_{\mathfrak{m}}$ est régulier et que les images des $dx_i$ forment une base du $\Lambda/\mathfrak{m}$-espace vectoriel $\Lambda/\mathfrak{m} \otimes_A \Omega_k(\Lambda)$.

Prouvons maintenant que l’anneau $\Lambda$ est intègre et régulier. Il existe un idéal premier minimal $\mathfrak{q}$ de $\Lambda$ tel que $\dim(\Lambda/\mathfrak{q}) = n$. Pour tout idéal maximal $\mathfrak{m}$ de $\Lambda$ contenant $\mathfrak{q}$, on a $\dim(A_{\mathfrak{m}}) = n$ (VIII, § 2, n° 4, cor. 2 du th. 3), de sorte que $A_{\mathfrak{m}}$ est régulier d’après ce que nous venons de voir. En particulier $A_{\mathfrak{m}}$ est intègre, ce qui impose $\mathfrak{q}A_{\mathfrak{m}} = 0$. Comme cela a lieu pour tous les idéaux maximaux $\mathfrak{m}$ de $V(\mathfrak{q})$, on en déduit qu’on a $\operatorname{Supp}(\mathfrak{q}) \cap V(\mathfrak{q}) = \varnothing$. Mais $\operatorname{Spec}(\Lambda)$ est connexe, $V(\mathfrak{q})$ est non vide et l’on a $\operatorname{Supp}(\mathfrak{q}) \cup V(\mathfrak{q}) = \operatorname{Spec}(\Lambda)$ (II, § 4, n° 4, prop. 16). On en déduit $\operatorname{Supp}(\mathfrak{q}) = \varnothing$, d’où $\mathfrak{q} = 0$, ce qui signifie que $\Lambda$ est intègre. On a alors $\dim(A_{\mathfrak{m}}) = n$ pour tout idéal maximal $\mathfrak{m}$ de $\Lambda$; appliquant la première partie de la démonstration, on en déduit que $\Lambda$ est régulier.

Enfin, soit $\sum_{i=1}^n a_i dx_i = 0$ une relation linéaire entre les $dx_i$ à coefficients dans $\Lambda$. Si les $a_i$ ne sont pas tous nuls, il existe un indice $i$ et un idéal maximal $\mathfrak{m}$ de $\Lambda$ tel que $a_i$ n’appartienne pas à $\mathfrak{m}$ (V, § 3, n° 3, prop. 1, (iii) et (iv)) ; mais cela contredit le fait démontré plus haut que les classes des $dx_i$ dans $(\Lambda/\mathfrak{m}) \otimes_A \Omega_k(\Lambda)$ sont linéairement indépendantes.

#### Exemple {#ac-x-s6-n5-exa-1 .statement}

Lorsque $\Lambda$ est une extension de type fini de $k$, le théorème 1 redonne le cor. 1 de A, V, p. 128, compte tenu de l’exemple 2 du n° 4.

#### Corollaire 1 {#ac-x-s6-lem-5-cor-1 .statement}

*Soient $k$ un corps et $\Lambda$ une $k$-algèbre essentiellement de type fini. L’ensemble des éléments $\mathfrak{p}$ de $\operatorname{Spec}(\Lambda)$ tels que la $k$-algèbre $\Lambda_{\mathfrak{p}}$ soit absolument régulière est ouvert dans $\operatorname{Spec}(\Lambda)$.*

On peut supposer que la $k$-algèbre $\Lambda$ est de type fini. L’ensemble considéré est alors formé des idéaux premiers $\mathfrak{p}$ tels que $[\kappa(\mathfrak{p}) \otimes_k \Omega_k(\Lambda) : \kappa(\mathfrak{p})] \leq \dim_{\mathfrak{p}}(\Lambda)$. Or la fonction $\mathfrak{p} \mapsto \dim_{\mathfrak{p}}(\Lambda)$ est semi-continue inférieurement par définition, et la fonction $\mathfrak{p} \mapsto [\kappa(\mathfrak{p}) \otimes_k \Omega_k(\Lambda) : \kappa(\mathfrak{p})]$ est semi-continue supérieurement (lemme de Nakayama et II, § 5, n° 1, prop. 2).

Nous verrons plus loin (§ 7, n° 9, cor. 4 du th. 3) que sous les hypothèses du cor. 1, l’ensemble des idéaux premiers $\mathfrak{p}$ de $\Lambda$ tels que l’anneau $\Lambda_{\mathfrak{p}}$ soit régulier est ouvert dans $\operatorname{Spec}(\Lambda)$.

#### Corollaire 2 {#ac-x-s6-lem-5-cor-2 .statement}

*Soient $k$ un corps et $\Lambda$ une $k$-algèbre essentiellement de type fini. Pour que $\Lambda$ soit absolument régulière, il faut et il suffit que le $\Lambda$-module $\Omega_k(\Lambda)$ soit projectif et que pour tout idéal premier minimal $\mathfrak{q}$ de $\Lambda$, la $k$-algèbre $\Lambda_{\mathfrak{q}}$ soit séparable.*

Inversement, supposons que le $A$-module $\Omega_k(A)$ soit projectif et que la $k$-algèbre $A_q$ soit séparable pour tout idéal premier minimal $q$ de $A$. Soient $p$ un idéal premier de $A$, et $q$ un idéal premier minimal de $A$ contenu dans $p$. Puisque le $A_p$-module $\Omega_k(A)_p$ est libre (II, § 3, n° 2, cor. 2 de la prop. 5), on a

$$
[\kappa(p) \otimes_A \Omega_k(A) : \kappa(p)] = [\kappa(q) \otimes_A \Omega_k(A) : \kappa(q)] .
$$

La $k$-algèbre $A_q$ est artinienne et séparable, donc absolument régulière (n° 4, exemple 2). Le th. 1 entraîne

$$
[\kappa(q) \otimes_A \Omega_k(A) : \kappa(q)] = \deg.\operatorname{tr}_k(\kappa(q)) .
$$

Il résulte alors du th. 1 que la $k$-algèbre $A_p$ est absolument régulière, d’où le corollaire.

#### Remarque {#ac-x-s6-n5-rem-1 .statement}

Supposons la $k$-algèbre $A$ absolument régulière. Alors l’anneau total des fractions $F$ de $A$ s’identifie au produit des $A_q$, où $q$ parcourt l’ensemble des idéaux premiers minimaux de $A$ (IV, § 2, n° 5, prop. 10); c’est donc une $k$-algèbre séparable. Supposons inversement que $F$ soit une $k$-algèbre séparable; pour tout idéal premier minimal $q$ de $A$, la $k$-algèbre $A_q$ est un anneau de fractions de $F$ (IV, § 1, n° 1, cor. 3 de la prop. 2 et n° 3, cor. 1 de la prop. 7), donc une $k$-algèbre séparable (n° 4, prop. 6). Si en outre le $A$-module $\Omega_k(A)$ est projectif, il résulte du cor. 2 que la $k$-algèbre $A$ est absolument régulière.

#### Corollaire 3 {#ac-x-s6-lem-5-cor-3 .statement}

Soient $k$ un corps de caractéristique 0 et $A$ une $k$-algèbre essentiellement de type fini. Pour que $A$ soit régulière, il faut et il suffit que le $A$-module $\Omega_k(A)$ soit projectif.

D’après le corollaire 2, il suffit de prouver qu’une $k$-algèbre locale artinienne $A$ telle que $\Omega_k(A)$ soit un $A$-module libre est un corps. Or, d’après IX, § 3, n° 3, th. 1, il existe un sous-corps $K$ de $A$ tel que $A = K \oplus m_A$. Soit $\delta : A \to m_A/m_A^2$ l’application composée de la projection de $A$ sur $m_A$ et de l’application canonique $m_A \to m_A/m_A^2$. On vérifie comme dans la démonstration du lemme 4 que $\delta$ est une $k$-dérivation. Mais toute $k$-dérivation de $A$ dans un $A$-module annule $m_A$: soient en effet $x \in m_A$, et $n$ un entier $\geq 1$ tel qu’on ait $x^{n-1} \neq 0,\ x^n = 0$. Cela implique dans le $A$-module $\Omega_k(A)$ la relation $nx^{n-1} dx = 0$, donc $dx = 0$ puisque $nx^{n-1} \neq 0$. Ainsi $\delta(m_A) = 0$, donc $m_A = m_A^2$, et en définitive $m_A = \{0\}$.

## EXERCICES {#ac-x-s6-exercises}

See the [exercises for § 6](exercises/s6/).
