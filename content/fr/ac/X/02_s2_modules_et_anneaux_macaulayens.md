---
book: ac
book_title: Commutative Algebra
chapter: X
chapter_title: Profondeur, régularité, dualité
section: 2
section_title: Modules et anneaux macaulayens
lang: fr
source: ac-x-fr
book_pages: AC X.154-AC X.157
pdf_pages: 0022-0035, 0153-0156
extraction: ocr
subsections:
    - "no": 1
      title: Modules macaulayens
      page: 0
      pdf_page: 22
    - "no": 2
      title: Support d’un module macaulayen
      page: 24
      pdf_page: 23
    - "no": 3
      title: Modules macaulayens sur un anneau local
      page: 26
      pdf_page: 25
    - "no": 4
      title: Parties fortement sécantes et quotients d’un module macaulayen
      page: 28
      pdf_page: 27
    - "no": 5
      title: Anneaux de Macaulay
      page: 30
      pdf_page: 29
    - "no": 6
      title: Modules macaulayens et algèbres finies
      page: 32
      pdf_page: 31
    - "no": 7
      title: Modules macaulayens et algèbres plates
      page: 0
      pdf_page: 33
statements: 46
exercises: 11
content_sha256: 650bbfdcc8ed4e299912939fbb5d1419edd5bfe730a6cdaaf497218c5852c4b7
---

## § 2. MODULES ET ANNEAUX MACAULAYENS

### 1. Modules macaulayens

Soient $A$ un anneau noethérien, $M$ un $A$-module de type fini et $p$ un idéal premier de $A$. Si $p \not\in \mathrm{Supp}(M)$, on a $M_p = 0$, donc $\mathrm{prof}_{A_p}(M_p) = +\infty$ et $\dim_{A_p}(M_p) = -\infty$. Si $p \in \mathrm{Supp}(M)$, on a $0 \leq \mathrm{prof}_{A_p}(M_p) \leq \dim_{A_p}(M_p) < +\infty$ ($§ 1$, n° 4, cor. 2 du th. 2).

#### Définition 1 {#ac-x-s2-def-1 .statement}

*Soient $A$ un anneau noethérien et $M$ un $A$-module de type fini. On dit que $M$ est macaulayen ou est un module de Macaulay si, pour tout idéal maximal $m \in \mathrm{Supp}(M)$, on a $\mathrm{prof}_{A_m}(M_m) = \dim_{A_m}(M_m)$.*

D’après ce qui précède, il revient au même de dire qu’on a $\mathrm{prof}_{A_m}(M_m) \geq \dim_{A_m}(M_m)$ pour tout idéal maximal $m$ de $A$. Soit $A$ un anneau local noethérien ; pour qu’un $A$-module non nul de type fini soit macaulayen, il faut et il suffit que sa profondeur soit égale à sa dimension.

#### Exemple 1 {#ac-x-s2-n1-exa-1 .statement}

Tout $A$-module de longueur finie est macaulayen.

#### Exemple 2 {#ac-x-s2-n1-exa-2 .statement}

Soit $M'$ un sous-module facteur direct d’un $A$-module de type fini macaulayen $M$. Alors $M'$ est macaulayen ; en effet, pour tout idéal maximal $m$ de $A$, le $A_m$-module $M'_m$ est facteur direct de $M_m$ et on a par conséquent
$$
\mathrm{prof}_{A_m}(M'_m) \geq \mathrm{prof}_{A_m}(M_m) \geq \dim_{A_m}(M_m) \geq \dim_{A_m}(M'_m),
$$
d’après la remarque 4 du $§ 1$, n° 1 ct VIII, $§ 1$, n° 4, prop. 9 c).

#### Exemple 3 {#ac-x-s2-n1-exa-3 .statement}

Soient $M$ un $A$-module de type fini et macaulayen et $(x_1, \ldots, x_n)$ une suite $M$-régulière d’éléments de $A$. Alors le $A$-module $\overline{M} = M/(x_1M + \cdots + x_nM)$ est macaulayen. Soit en effet $m$ un idéal maximal de $A$ appartenant au support de $\overline{M}$ ; on a $x_i \in m$ pour tout $i$ puisque $x_i$ annule $\overline{M}$, et les images canoniques des $x_i$ dans $A_m$ forment une suite $M_m$-régulière d’éléments de $mA_m$. On a par conséquent ($§ 1$, n° 4, prop. 7 et VIII, $§ 3$, n° 2, cor. de la prop. 3) les égalités
$$
\mathrm{prof}_{A_m}(\overline{M}_m) = \mathrm{prof}_{A_m}(M_m) - n,
$$
$$
\dim_{A_m}(\overline{M}_m) = \dim_{A_m}(M_m) - n,
$$
d’où notre assertion.

#### Exemple 4 {#ac-x-s2-n1-exa-4 .statement}

Soient $M$ un $A$-module de type fini, et $a$ un idéal de $A$ tel que $aM = 0$. Pour que le $A$-module $M$ soit macaulayen, il faut et il suffit qu’il soit macaulayen comme $(A/a)$-module. En effet, posons $B = A/a$ ; soient $n$ un idéal maximal de $B$ et $m$ son image réciproque dans $A$ ; on a $\dim_{A_m}(M_m) = \dim_{B_n}(M_n)$ et $\mathrm{prof}_{A_m}(M_m) = \mathrm{prof}_{B_n}(M_n)$ ($§ 1$, n° 3, cor. de la prop. 4).

#### Proposition 1 {#ac-x-s2-prop-1 .statement}

Soient $\Lambda$ un anneau noethérien, $M$ un $\Lambda$-module de type fini, $p$ et $q$ des idéaux premiers de $\mathrm{Supp}(M)$ tels que $p \subset q$. Supposons $\dim_{\Lambda_q}(M_q) = \mathrm{prof}_{\Lambda_q}(M_q)$. On a alors $\dim_{\Lambda_p}(M_p) = \mathrm{prof}_{\Lambda_p}(M_p)$ et
$$
\dim_{\Lambda_q}(M_q) = \dim_{\Lambda_p}(M_p) + \dim(\Lambda_q/\mathfrak{p}\Lambda_q) .
$$
Cela résulte directement du cor. 1 de la prop. 13 du § 1, n° 7.

#### Corollaire {#ac-x-s2-n1-cor-1 .statement}

Soient $\Lambda$ un anneau noethérien et $M$ un $\Lambda$-module de type fini. Les conditions suivantes sont équivalentes :
(i) le $\Lambda$-module $M$ est macaulayen ;
(ii) on a $\mathrm{prof}_{\Lambda_p}(M_p) = \dim_{\Lambda_p}(M_p)$ pour tout $p \in \mathrm{Supp}(M)$ ;
(iii) on a $\mathrm{prof}_F(M) = \mathrm{codim}(\mathrm{Supp}(M) \cap F', \mathrm{Supp}(M))$ pour toute partie fermée $F$ de $\mathrm{Spec}(\Lambda)$ ;
(iv) on a $\mathrm{prof}_A(p; M) = \dim_{\Lambda_p}(M_p)$ pour tout $p \in \mathrm{Supp}(M)$.

(i) $\Rightarrow$ (ii) : cela résulte de la proposition 1.
(ii) $\Rightarrow$ (iii) : d’après la prop. 8 du § 1, n° 5, $\mathrm{prof}_F(M)$ est la borne inférieure des entiers $\mathrm{prof}(M_p)$ pour $p$ parcourant $\mathrm{Supp}(M) \cap F$. Si $M$ est macaulayen, on a pour un tel idéal $p$ les égalités $\mathrm{prof}(M_p) = \dim(M_p) = \mathrm{codim}(V(p), \mathrm{Supp}(M))$ (VIII, § 1, n° 4, prop. 9), d’où (iii).
(iii) $\Rightarrow$ (iv) : il suffit de prendre $F = V(p)$.
(iv) $\Rightarrow$ (i) : cela résulte des inégalités $\mathrm{prof}_A(p; M) \leq \mathrm{prof}(M_p) \leq \dim(M_p)$, valables pour tout $p \in \mathrm{Supp}(M)$ ($§ 1$, n° 5, remarque 3 et n° 4, cor. 2 du th. 2).

#### Remarque {#ac-x-s2-n1-rem-1 .statement}

Soient $S$ une partie multiplicative de $\Lambda$ et $M$ un $\Lambda$-module de type fini et macaulayen. Alors $S^{-1}M$ est un $S^{-1}\Lambda$-module macaulayen. En effet, soit $q \in \mathrm{Spec}(S^{-1}\Lambda)$ ; notons $i_A^S : \Lambda \to S^{-1}\Lambda$ l’homomorphisme canonique et $p = (i_A^S)^{-1}(q)$. L’anneau $(S^{-1}\Lambda)_q$ s’identifie à $A_p$ (II, § 2, n° 5, prop. 11), et le $A_p$-module $(S^{-1}M)_q$ au $A_p$-module $M_p$ (II, § 2, n° 7, prop. 20), qui est macaulayen d’après le corollaire.

### 2. Support d’un module macaulayen

#### Proposition 2 {#ac-x-s2-prop-2 .statement}

Soient $\Lambda$ un anneau noethérien et $M$ un $\Lambda$-module de type fini et macaulayen.
a) Le $\Lambda$-module $M$ n’a pas d’idéaux premiers associés immergés.\footnote{Rappelons (cf. IV, § 2, n° 3, remarque) qu’on dit qu’un idéal premier associé à $M$ est immergé s’il n’est pas un élément minimal de $\mathrm{Supp}(M)$. Dire que $M$ n’a pas d’idéaux premiers associés immergés signifie donc que les idéaux premiers associés de $M$ sont les éléments minimaux de $\mathrm{Supp}(M)$.}
b) Soient $X$ une partie fermée irréductible de $\mathrm{Supp}(M)$ et $Y$ une partie fermée de $X$. On a
$$
\mathrm{codim}(Y, X) + \mathrm{codim}(X, \mathrm{Supp}(M)) = \mathrm{codim}(Y, \mathrm{Supp}(M)) .
$$
c) L’espace topologique $\mathrm{Supp}(M)$ est caténaire (VIII, § 1, n° 2, déf. 4).

d) Soient $X_1$ et $X_2$ des composantes irréductibles de $\mathrm{Supp}(M)$ et $Y$ une partie fermée de $X_1 \cap X_2$. On a $\mathrm{codim}(Y, X_1) = \mathrm{codim}(Y, X_2)$.

a) Soit $\mathfrak{p} \in \mathrm{Ass}(M)$. On a $\mathrm{prof}_A(\mathfrak{p}; M) = 0$ ($\S$ 1, n° 1, remarque 2), donc $\dim(M_{\mathfrak{p}}) = 0$ (n° 1, cor. de la prop. 1), ce qui implique que $\mathfrak{p}$ est un élément minimal de $\mathrm{Supp}(M)$.

b) Supposons d’abord $Y$ irréductible. Soient $\mathfrak{p}$ et $\mathfrak{q}$ les idéaux premiers de $\mathrm{Supp}(M)$ tels qu’on ait $Y = V(\mathfrak{q})$ et $X = V(\mathfrak{p})$. Il résulte de la prop. 1 que l’on a

$$
\begin{align*}
\mathrm{codim}(Y, X) &= \dim(A_{\mathfrak{q}}/\mathfrak{p}A_{\mathfrak{q}}) = \dim(M_{\mathfrak{q}}) - \dim(M_{\mathfrak{p}}) \\
&= \mathrm{codim}(Y, \mathrm{Supp}(M)) - \mathrm{codim}(X, \mathrm{Supp}(M)) .
\end{align*}
$$

Le cas général résulte de VIII, $\S$ 1, n° 2, remarque 3.

c) Soient $X$, $Y$, $Z$ des parties fermées irréductibles de $\mathrm{Supp}(M)$ telles que $Z \subset Y \subset X$. La codimension de chacune de ces parties dans $\mathrm{Supp}(M)$ est finie (VIII, $\S$ 1, n° 4, prop. 9 et $\S$ 3, n° 1, cor. 1 de la prop. 2). On déduit alors de b) l’égalité

$$
\mathrm{codim}(Z, Y) + \mathrm{codim}(Y, X) = \mathrm{codim}(Z, X)
$$

qui entraîne c) (VIII, $\S$ 1, n° 2, prop. 4).

d) D’après b), on a $\mathrm{codim}(Y, X_1) = \mathrm{codim}(Y, \mathrm{Supp}(M)) = \mathrm{codim}(Y, X_2)$.

En particulier, s’il existe un $A$-module $M$ de type fini, macaulayen, de support égal à $\mathrm{Spec}(A)$, l’anneau $A$ est caténaire et par conséquent tout anneau de fractions ou tout anneau quotient de $A$ est caténaire (VIII, $\S$ 1, n° 3, remarque 2).

#### Remarque 1 {#ac-x-s2-n2-rem-1 .statement}

Sous les hypothèses de la prop. 2, il peut arriver que deux composantes irréductibles $X_1$ et $X_2$ de $\mathrm{Supp}(M)$ aient une intersection $Y$ réduite à un point et que l’on ait $\dim X_1 \neq \dim X_2$ et $\dim X_2 \neq \mathrm{codim}(Y, X_2)$ (cf. exercice 4). Cependant ceci ne peut arriver lorsque l’anneau $A$ est local, comme le montre le corollaire qui suit.

#### Corollaire {#ac-x-s2-n2-cor-1 .statement}

Soient $A$ un anneau local noethérien et $M$ un $A$-module de type fini non nul et macaulayen.

a) Toutes les chaînes maximales de parties fermées irréductibles de $\mathrm{Supp}(M)$ sont de longueur égale à $\dim(M)$.

b) Pour toute partie fermée $X$ de $\mathrm{Supp}(M)$, on a

$$
\mathrm{codim}(X, \mathrm{Supp}(M)) = \dim(\mathrm{Supp}(M)) - \dim(X) .
$$

c) Toutes les composantes irréductibles de $\mathrm{Supp}(M)$ ont la même dimension.

d) Pour tout idéal $J$ de $A$, on a

$$
\mathrm{prof}_A(J; M) = \dim(M) - \dim(M/JM) .
$$

a) Une chaîne maximale de parties fermées irréductibles de $\mathrm{Supp}(M)$ a pour plus petit élément $\{m_A\}$ et pour plus grand élément une composante irréductible $X$ de

Supp(M). Sa longueur est égale à la codimension de $\{ m_A \}$ dans X (prop. 2, c)) ; d’après la prop. 2, b) appliquée aux parties fermées $\{ m_A \} \subset X$, celle-ci est égale à $\operatorname{codim}(\{ m_A \}, \operatorname{Supp}(M))$, c’est-à-dire à $\dim(M)$.

b) C’est une conséquence de a) lorsque la partie X est irréductible (VIII, § 1, n° 2, prop. 5) ; le cas général résulte de VIII, § 1, n° 1, prop. 1 et § 1, n° 2, remarque 4.

c) C’est une conséquence de b).

d) On a $\operatorname{prof}_A(J; M) = \operatorname{codim}(\operatorname{Supp}(M) \cap V(J), \operatorname{Supp}(M))$ d’après le cor. de la prop. 1 du n° 1. Il suffit alors d’appliquer b) avec $X = \operatorname{Supp}(M) \cap V(J) = \operatorname{Supp}(M/JM)$ (II, § 4, n° 4, cor. de la prop. 18).

#### Remarque 2 {#ac-x-s2-n2-rem-2 .statement}

Soient M un A-module de type fini et macaulayen, et $p$ un élément de $\operatorname{Supp}(M)$. Compte tenu du th. 2 du § 1, n° 4, on a $\operatorname{prof}_A(p; M) < +\infty$, et il existe une suite M-régulière de longueur $\operatorname{prof}_A(p; M)$ formée d’éléments de $p$. Notons J l’idéal de A engendré par une telle suite ; alors le A-module $M/JM$ est macaulayen (n° 1, exemple 3) et $p$ est un élément minimal de son support. En effet, $p$ contient J donc appartient au support de $M/JM$ (II, § 4, n° 4, cor. de la prop. 18) ; d’après le corollaire 1 du théorème 2 du § 1, n° 4, l’idéal $p$ est contenu dans un élément de $\operatorname{Ass}(M/JM)$, mais tout idéal premier associé à un module de type fini macaulayen est un élément minimal de son support (prop. 2).

### 3. Modules macaulayens sur un anneau local

#### Proposition 3 {#ac-x-s2-prop-3 .statement}

Soient A un anneau local noethérien, M un A-module non nul de type fini et d la dimension de M. Les conditions suivantes sont équivalentes :

(i) le A-module M est macaulayen ;
(ii) on a $\operatorname{prof}(M) = d$ ;
(iii) on a $\operatorname{Ext}_A^i(\kappa_A, M) = 0$ pour tout entier $i < d$ ;
(iv) on a $\operatorname{Ext}_A^i(N, M) = 0$ pour tout A-module N de longueur finie et tout entier $i < d$ ;
(v) on a $\operatorname{Ext}_A^i(N, M) = 0$ pour tout A-module N de type fini et tout entier $i < d - \dim(M \otimes_A N)$ ;
(vi) il existe une suite M-régulière d’éléments de $m_A$ de longueur d.

La condition (i) équivaut à l’égalité $\operatorname{prof}(M) = d$, c’est-à-dire à la condition (ii), ou encore à l’inégalité $\operatorname{prof}(M) \geq d$, c’est-à-dire à (iii) et à (vi) (§ 1, n° 4, th. 2). Les implications (v) $\Rightarrow$ (iv) et (iv) $\Rightarrow$ (iii) sont évidentes.

Enfin, supposons M macaulayen et soit N un A-module de type fini. Posons $F = \operatorname{Supp}(N)$ ; d’après II, § 4, n° 4, prop. 18, on a $\operatorname{Supp}(M) \cap F = \operatorname{Supp}(M \otimes_A N)$, de sorte que

$$
\operatorname{prof}_F(M) = \operatorname{codim}(\operatorname{Supp}(M) \cap F, \operatorname{Supp}(M)) = \dim M - \dim(M \otimes_A N)
$$

(n° 1, cor. de la prop. 1 et n° 2, cor. de la prop. 2). L’implication (i) $\Rightarrow$ (v) résulte alors de la remarque 1 du § 1, n° 5.

Nous dirons dans la suite de ce numéro qu’un module M de type fini sur un anneau local noethérien A est pur si, pour tout idéal premier p associé à M, on a dim(A/p) = dim(M). Cela signifie aussi que M n’a pas d’idéaux premiers associés immergés et que les composantes irréductibles du support de M ont toutes la même dimension. Tout module macaulayen sur un anneau local noethérien est pur (n° 2, prop. 2 et son corollaire).

Lemme 1:— Soient A un anneau local noethérien, M un A-module de type fini et pur, et x un élément de mA. Les conditions suivantes sont équivalentes :

(i) on a dim(M/xM) = dim(M) − 1 ;
(ii) l’homothétie xM est injective.

On peut supposer M non nul. L’assertion (i) équivaut au fait que x n’appartienne à aucun des éléments minimaux p de Supp(M) tels que dim(A/p) = dim(M) (VIII, § 3, n° 2, prop. 3) et l’assertion (ii) équivaut au fait que x n’appartienne à aucun des idéaux premiers associés à M (IV, § 1, n° 1, cor. 2 de la prop. 2). Puisque M est pur, ses idéaux premiers associés sont les éléments minimaux de Supp(M), donc (i) et (ii) sont équivalentes.

Soient A un anneau local noethérien et M un A-module non nul de type fini. Rappelons (VIII, § 3, n° 2) qu’une suite (x₁, ..., x_r) d’éléments de mA est dite sécante pour M si l’on a dim(M/(x₁M + ... + x_rM)) = dim(M) − r.

#### Proposition 4 {#ac-x-s2-prop-4 .statement}

Soient A un anneau local noethérien, M un A-module non nul de type fini et (x₁, ..., x_r) une suite d’éléments de mA sécante pour M. Les conditions suivantes sont équivalentes :

(i) le A-module M est macaulayen ;
(ii) la suite (x₁, ..., x_r) est M-régulière et le A-module M/(x₁M + ... + x_rM) est macaulayen.

Supposons que la suite (x₁, ..., x_r) soit M-régulière. On a alors

$$
\dim(M) = r + \dim(M/(x_1M + ... + x_rM))
$$
$$
\operatorname{prof}(M) = r + \operatorname{prof}(M/(x_1M + ... + x_rM))
$$

(§ 1, n° 4, prop. 7), d’où l’implication (ii) ⇒ (i).

Supposons le A-module M macaulayen et démontrons (ii) par récurrence sur r. L’assertion est évidente si r = 0. Si r ≥ 1, le A-module N = M/(x₁M + ... + x_{r−1}M) est macaulayen par l’hypothèse de récurrence et l’on a dim(N/x_rN) = dim(N) − 1 puisque la suite (x₁, ..., x_r) est sécante ; l’homothétie (x_r)_N est donc injective (lemme 1), et N/x_rN est macaulayen (n° 1, exemple 3), d’où (ii).

#### Théorème 1 {#ac-x-s2-thm-1 .statement}

Soient A un anneau local noethérien, M un A-module non nul de type fini, d la dimension de M, x = (x₁, ..., x_d) une suite d’éléments de mA sécante pour M, et J l’idéal qu’elle engendre. Les conditions suivantes sont équivalentes :

(i) le A-module M est macaulayen ;

(ii) la suite $x$ est M-régulière ;
(iii) la suite $x$ est complètement sécante pour $M$ (A, X, p. 157, déf. 2) ;
(iv) la multiplicité (VIII, § 7, n° 1, déf. 1) $e_J(M)$ de $M$ relativement à l’idéal $J$ est égale à la longueur du A-module $M/JM$ ;
(v) pour chaque entier $i$ tel que $1 \leq i \leq d$, le A-module $M/(x_1M + \ldots + x_{i-1}M)$ est pur.

L’équivalence de (ii) et (iii) résulte de A, X, p. 160, cor. 1 du th. 1. Le A-module $M/JM$ étant de longueur finie (VIII, § 3, n° 2, th. 1), l’équivalence de (iii) et (iv) résulte de VIII, § 4, n° 3, prop. 4 et n° 4, th. 3. Il reste à prouver l’équivalence de (i), (ii) et (v).

(i) $\Rightarrow$ (v) : si $M$ est macaulayen, chacun des modules $M/(x_1M + \ldots + x_{i-1}M)$ est macaulayen (prop. 4), donc pur.

(v) $\Rightarrow$ (ii) : cela résulte du lemme 1 appliqué à chacun des modules $M/(x_1M + \ldots + x_{i-1}M)$.

(ii) $\Rightarrow$ (i) : cela résulte de la prop. 4, puisque $M/JM$ est de longueur finie, donc macaulayen.

### 4. Parties fortement sécantes et quotients d’un module macaulayen

Soient $A$ un anneau noethérien, $M$ un A-module de type fini, et $S$ une partie de $A$. Conformément aux conventions du ch. VIII nous noterons $SM$ le sous-module $\sum_{s \in S} sM$ de $M$, et $\mathcal{G}$ l’idéal de $A$ engendré par $S$.

#### Lemme 2 {#ac-x-s2-lem-2 .statement}

Soit $\overline{\mathcal{G}}$ l’image de $\mathcal{G}$ dans $A/\mathrm{Ann}(M)$. On a
$$
\mathrm{ht}(\overline{\mathcal{G}}) = \mathrm{codim}(\mathrm{Supp}(M/SM), \mathrm{Supp}(M)) .
$$
Lorsque de plus $SM \neq M$, on a
$$
\mathrm{ht}(\overline{\mathcal{G}}) \leq \mathrm{Card}(S) .
$$

Notons $\alpha$ l’annulateur de $M$. D’après le cor. de la prop. 18 de II, § 4, n° 4, le support du A-module $M/SM$ est $V(\mathcal{G} + \alpha)$. Sa codimension dans $\mathrm{Supp}(M)$ est donc égale à la codimension de $V(\mathcal{G} + \alpha)$ dans $V(\alpha)$, soit encore à la codimension de $V((\mathcal{G} + \alpha)/\alpha)$ dans $\mathrm{Spec}(A/\alpha)$, qui n’est autre que la hauteur de $\overline{\mathcal{G}}$.

Supposons $SM \neq M$ ; l’inégalité $\mathrm{ht}(\overline{\mathcal{G}}) \leq \mathrm{Card}(S)$ est évidente lorsque $S$ est infinie, et résulte de la prop. 4 b) de VIII, § 3, n° 3 lorsque $S$ est finie.

#### Définition 2 {#ac-x-s2-def-2 .statement}

Soient $A$ un anneau noethérien, $M$ un A-module de type fini, et $S$ une partie finie de $A$. On dit que $S$ est fortement sécante pour $M$ si l’on a
$$
\mathrm{Card}(S) \leq \mathrm{codim}(\mathrm{Supp}(M/SM), \mathrm{Supp}(M)) .
$$

#### Remarque 1 {#ac-x-s2-n4-rem-1 .statement}

Toute partie finie S de A telle que SM = M est fortement sécante pour M. Lorsque SM ≠ M, il résulte du lemme 2 que pour que S soit fortement sécante pour M, il faut et il suffit qu’on ait Card(S) = codim(Supp(M/SM), Supp(M)), ou encore ht($\overline{\mathcal{G}}$) = Card(S).

#### Remarque 2 {#ac-x-s2-n4-rem-2 .statement}

Si l’anneau A est local et le module M non nul, toute partie S de $m_A$ fortement sécante pour M est sécante pour M. En effet, comme le $\Lambda$-module M/SM est non nul, on a

$$
\text{Card}(S) \leq \operatorname{codim}(\operatorname{Supp}(M/SM), \operatorname{Supp}(M)) \leq \dim(M) - \dim(M/SM)
$$

(VIII, § 1, n° 2, prop. 3 a)), d’où notre assertion.

#### Proposition 5 {#ac-x-s2-prop-5 .statement}

Soient A un anneau noethérien, M un A-module de type fini, et S une partie finie de A. Les conditions suivantes sont équivalentes :

(i) la partie S de A est fortement sécante pour M ;
(ii) pour tout élément $p$ de Supp(M/SM), l’application canonique $\Lambda \to A_p$ induit une bijection de S sur une partie de $pA_p$ sécante pour $M_p$.

(i) $\Rightarrow$ (ii) : Soit $p \in \operatorname{Supp}(M/SM)$ et soit $S'$ l’image de S dans $A_p$. L’ensemble $S'$ est contenu dans l’idéal maximal $pA_p$, et l’on a

$$
\dim(M_p/S'M_p) = \operatorname{codim}(V(p), \operatorname{Supp}(M/SM))
$$

(VIII, § 1, n° 4, prop. 9). L’inégalité Card(S) $\leq \operatorname{codim}(\operatorname{Supp}(M/SM), \operatorname{Supp}(M))$ et la prop. 3 b) de VIII, § 1, n° 2 entraînent les relations

$$
\text{Card}(S) + \dim(M_p/S'M_p) \leq \operatorname{codim}(V(p), \operatorname{Supp}(M)) = \dim(M_p) .
$$

Comme $M_p$ n’est pas nul, on a d’autre part $\dim(M_p) \leq \text{Card}(S') + \dim(M_p/S'M_p)$ (VIII, § 3, n° 2, formule (8)). La condition (ii) découle alors de l’inégalité $\text{Card}(S') \leq \text{Card}(S)$.

(ii) $\Rightarrow$ (i) : On peut supposer SM $\neq$ M. Si la condition (ii) est satisfaite, on a pour tout idéal premier $p$ de Supp(M/SM)

$$
\text{Card}(S) = \text{Card}(S') \leq \dim(M_p) = \operatorname{codim}(V(p), \operatorname{Supp}(M)) ,
$$

ce qui entraîne (i) par passage à la borne inférieure.

#### Corollaire {#ac-x-s2-n4-cor-1 .statement}

Soient A un anneau noethérien et M un A-module de type fini. Toute suite M-régulière est fortement sécante pour M.

Soient x une suite M-régulière, et J l’idéal de A qu’elle engendre. Pour tout idéal premier $p \in \operatorname{Supp}(M/JM)$, l’image de x dans $A_p$ est une suite $M_p$-régulière d’éléments de $pA_p$, donc une suite sécante pour $M_p$ (VIII, § 3, n° 2, cor. de la prop. 3).

#### Proposition 6 {#ac-x-s2-prop-6 .statement}

Soient A un anneau noethérien, M un A-module macaulayen de type fini, et S une partie finie de A fortement sécante pour M. Alors le A-module M/SM est macaulayen.

Pour tout idéal maximal $m \in \mathrm{Supp}(M/SM)$, l’image de S dans $A_m$ est sécante pour $M_m$ (prop. 5). Puisque $M_m$ est un $A_m$-module macaulayen, il en est de même de $(M/SM)_m$ (prop. 4), d’où la proposition.

**Théorème 2 (Macaulay-Cohen).**— *Soient A un anneau noethérien et M un A-module de type fini. Les conditions suivantes sont équivalentes :*

(i) *le A-module M est macaulayen ;*

(ii) *pour tout idéal J de A engendré par une suite M-régulière d’éléments de A, le A-module M/JM n’a pas d’idéaux premiers associés immergés ;*

(iii) *pour toute partie finie S de A fortement sécante pour M, le A-module M/SM n’a pas d’idéaux premiers associés immergés.*

(i) $\Rightarrow$ (iii) : Soit S une partie finie de A fortement sécante pour M. Le A-module M/SM est macaulayen (prop. 6) et en particulier n’a pas d’idéaux premiers associés immergés (n° 2, prop. 2, a)).

(iii) $\Rightarrow$ (ii) : Cela résulte du cor. de la prop. 5.

(ii) $\Rightarrow$ (i) : Soit $p \in \mathrm{Supp}(M)$; démontrons que le $A_p$-module $M_p$ est macaulayen. Raisonnons par récurrence sur l’entier $\dim(M_p)$. Si $\dim(M_p)$ est nul, $M_p$ est un $A_p$-module de longueur finie, donc macaulayen (exemple 1, n° 1). Supposons que $\dim(M_p)$ soit non nul, c’est-à-dire que $p$ ne soit pas un élément minimal de $\mathrm{Supp}(M)$ (VIII, § 1, n° 4, prop. 9 a)). Comme M n’a pas d’idéaux premiers associés immergés, $p$ n’est contenu dans aucun idéal premier associé à M et il existe un élément $x$ de $p$ tel que l’homothétie $x_M$ soit injective ($§ 1$, remarque 2). L’homothétie $x_{M_p}$ est alors injective et l’on a $\dim(M_p/xM_p) < \dim(M_p)$ (VIII, § 3, n° 2, prop. 3). D’après l’hypothèse de récurrence appliquée au A-module $M/xM$ et à l’idéal premier $p$ de $\mathrm{Supp}(M/xM)$, le $A_p$-module $M_p/xM_p$ est macaulayen, ce qui entraîne que le $A_p$-module $M_p$ est macaulayen (n° 3, prop. 4).

### 5. Anneaux de Macaulay

#### Définition 3 {#ac-x-s2-def-3 .statement}

*On dit qu’un anneau $\Lambda$ est macaulayen, ou est un anneau de Macaulay, s’il est noethérien et que le A-module $\Lambda$ est macaulayen.*

#### Exemple 1 {#ac-x-s2-n5-exa-1 .statement}

Tout anneau artinien est un anneau de Macaulay (n° 1, exemple 1).

#### Exemple 2 {#ac-x-s2-n5-exa-2 .statement}

Un anneau de Macaulay ne possède pas d’idéaux premiers associés immergés (n° 2, prop. 2). Inversement, soit $A$ un anneau noethérien de dimension $\leqslant 1$ qui ne possède pas d’idéaux premiers associés immergés ; pour toute partie finie non vide fortement sécante S de A, le A-module $A/SA$ est de dimension $\leqslant 0$, donc macaulayen (n° 1, exemple 1) ; par suite A est un anneau de Macaulay (n° 4, th. 2). En particulier un anneau noethérien réduit de dimension $\leqslant 1$ est un anneau de Macaulay.

#### Exemple 3 {#ac-x-s2-n5-exa-3 .statement}

Un anneau noethérien normal de dimension $\leqslant 2$ est un anneau de Macaulay ($§ 1$, n° 10, texte précédant le th. 4). Inversement, soit $A$ un anneau de Macaulay dont l’anneau local $A_p$ en tout idéal premier $p$ de hauteur $\leqslant 1$ est intégralement clos ; alors A est normal ($§ 1$, n° 10, th. 4).

#### Exemple 4 {#ac-x-s2-n5-exa-4 .statement}

Si $A$ est un anneau de Macaulay, il en est de même de $S^{-1}A$ pour toute partie multiplicative $S$ de $A$ (n° 1, remarque). Inversement, si l’anneau $A_m$ est un anneau de Macaulay pour tout idéal maximal $m$ de $A$, alors l’anneau $A$ est de Macaulay (n° 1, déf. 1).

#### Exemple 5 {#ac-x-s2-n5-exa-5 .statement}

Soient $A$ un anneau noethérien et $J$ un idéal de $A$. Pour que $A/J$ soit un anneau de Macaulay, il faut et il suffit que ce soit un $\Lambda$-module macaulayen (n° 1, exemple 4).

#### Exemple 6 {#ac-x-s2-n5-exa-6 .statement}

Soient $A$ un anneau local noethérien et $J$ un idéal de $A$ engendré par une suite $A$-régulière. Pour que $A/J$ soit un anneau de Macaulay, il faut et il suffit que $A$ en soit un (exemple 5 et prop. 4 du n° 3).

#### Exemple 7 {#ac-x-s2-n5-exa-7 .statement}

Pour qu’un anneau local noethérien $A$ soit de Macaulay, il faut et il suffit qu’il possède un idéal de définition engendré par une suite $A$-régulière : cela résulte de la prop. 3 du n° 3, et du fait qu’une suite $A$-régulière d’éléments de $m_A$ engendre un idéal de définition si et seulement si elle est de longueur $\dim(A)$ (VIII, § 3, n° 2, th. 1 et cor. de la prop. 3). En particulier, tout anneau local noethérien régulier est un anneau de Macaulay (VIII, § 5, n° 2, th. 1). Plus généralement, le quotient d’un anneau local noethérien régulier $A$ par un idéal engendré par une suite $A$-régulière est un anneau de Macaulay (exemple 6).

#### Proposition 7 {#ac-x-s2-prop-7 .statement}

Soit $A$ un anneau noethérien. Les conditions suivantes sont équivalentes :

(i) $A$ est un anneau de Macaulay ;
(ii) pour toute partie fermée $F$ de $\mathrm{Spec}(A)$, on a $\mathrm{prof}_F(A) = \mathrm{codim}(F)$ ;
(iii) tout idéal $J$ de $A$ contient une suite $A$-régulière de longueur $\mathrm{ht}(J)$ ;
(iii') tout idéal maximal $m$ de $A$ contient une suite $A$-régulière de longueur $\mathrm{ht}(m)$ ;
(iv) pour tout idéal $J$ de $A$, on a $\mathrm{Ext}_A^i(A/J, A) = 0$ pour $i < \mathrm{ht}(J)$ ;
(iv') pour tout idéal maximal $m$ de $A$, on a $\mathrm{Ext}_A^i(A/m, A) = 0$ pour $i < \mathrm{ht}(m)$ ;
(v) pour tout idéal premier $p$ de $A$ et tout idéal $J$ de $A_p$ engendré par une suite sécante maximale pour $A_p$, on a $e_J(A_p) = \mathrm{long}(A_p/ JA_p)$ ;
(v') pour tout idéal maximal $m$ de $A$, il existe un idéal $J$ de $A_m$, engendré par une suite sécante maximale pour $A_m$, satisfaisant à $e_J(A_m) = \mathrm{long}(A_m/ JA_m)$ ;
(vi) (critère de Macaulay-Cohen) pour toute partie finie $S$ de $A$ telle que l’idéal $\mathfrak{S}$ engendré par $S$ soit de hauteur $\mathrm{Card}(S)$, le $A$-module $A/\mathfrak{S}$ n’a pas d’idéaux premiers associés immergés.

L’équivalence de (i) et (ii) résulte du n° 1, cor. de la prop. 1. D’après le th. 2 du § 1, n° 4, et la définition de la profondeur, les conditions (iii) et (iv) (resp. (iii') et (iv')) signifient qu’on a $\mathrm{prof}_A(J; A) \geq \mathrm{ht}(J)$ pour tout idéal (resp. tout idéal maximal) $J$ de $A$. On a donc

$$
(i) \Leftrightarrow (ii) \Rightarrow (iii) \Leftrightarrow (iv) \Rightarrow (iii') \Leftrightarrow (iv').
$$

Mais (iv') implique, pour tout idéal maximal $m$ de $A$, $\mathrm{Ext}_{A_m}^i(\kappa(m), A_m) = 0$ pour $i < \dim(A_m)$, d’où $\mathrm{prof}(A_m) \geq \dim(A_m)$, de sorte que $A$ est un anneau de Macaulay.

L’équivalence de (i), (v) et (v’) résulte du th. 1 du n° 3, et celle de (i) et (vi) du th. 2 du n° 4.

### 6. Modules macaulayens et algèbres finies

#### Remarque {#ac-x-s2-n6-rem-1 .statement}

Soit $\rho : A \to B$ un homomorphisme d’anneaux, et soit $p \in \mathrm{Spec}(A)$. Notons $\overline{B}$ l’anneau $\kappa(p) \otimes_A B$. Il s’identifie à $S^{-1}B/p(S^{-1}B)$, où $S$ est la partie multiplicative $\rho(A - p)$ de $B$; les idéaux premiers de $\overline{B}$ sont donc les idéaux $q\overline{B}$, où $q$ est un idéal premier de $B$ qui contient $pB$ et ne rencontre pas $S$, autrement dit un idéal premier de $B$ au-dessus de $p$. Pour un tel idéal $q$, on a $S \subset B - q$, donc l’anneau local de $\overline{B}$ en $q\overline{B}$ s’identifie à $B_q/pB_q$, c’est-à-dire encore à $\kappa(p) \otimes_A B_q$.

De même, si $N$ est un $B$-module, le $\overline{B}_{q\overline{B}}$-module $(\kappa(p) \otimes_A N)_{q\overline{B}}$ s’identifie à $\kappa(p) \otimes_A N_q$. Supposons de plus que le $B$-module $N$ soit de type fini ; d’après le lemme de Nakayama, la condition $\kappa(p) \otimes_A N_q = 0$ équivaut à $N_q = 0$. Ainsi le support du $\overline{B}$-module $\kappa(p) \otimes_A N$ est formé des idéaux $q\overline{B}$, où $q$ parcourt les idéaux premiers de $\mathrm{Supp}_B(N)$ au-dessus de $p$. En particulier, pour que le module $\kappa(p) \otimes_A N$ soit non nul, il faut et il suffit qu’il existe un idéal premier de $\mathrm{Supp}_B(N)$ au-dessus de $p$.

#### Proposition 8 {#ac-x-s2-prop-8 .statement}

Soit $\rho : A \to B$ un homomorphisme d’anneaux noethériens et soit $N$ un $B$-module qui est un $A$-module de type fini. Pour que le $A$-module $N$ soit macaulayen, il faut et il suffit que le $B$-module $N$ soit macaulayen et que, pour tout couple $(n, n')$ d’idéaux maximaux de $\mathrm{Supp}_B(N)$ tel que $\rho^{-1}(n) = \rho^{-1}(n')$, on ait $\dim_{B_n}(N_n) = \dim_{B'_n}(N'_n)$.

Le $A$-module $B/\mathrm{Ann}_B(N)$ est isomorphe à un sous-module du $A$-module de type fini $\mathrm{End}_A(N)$, donc est de type fini. Remplaçant $A$ par $A/\mathrm{Ann}_A(N)$ et $B$ par $B/\mathrm{Ann}_B(N)$, on se ramène au cas où $\rho$ est injectif et fait de $B$ une $A$-algèbre finie, et où l’on a $\mathrm{Supp}_A(N) = \mathrm{Spec}(A)$ et $\mathrm{Supp}_B(N) = \mathrm{Spec}(B)$. L’application $f : \mathrm{Spec}(B) \to \mathrm{Spec}(A)$ déduite de $\rho$ est alors surjective et un idéal premier $q$ de $B$ est maximal si et seulement si $f(q)$ est un idéal maximal de $A$ (V, § 2, n° 1, th. 1 et prop. 1).

Soit $m$ un idéal maximal de $A$. D’après la remarque ci-dessus, les idéaux premiers de l’anneau $B_m$ contenant $mB_m$ sont les idéaux de la forme $qB_m$ où $q \in \mathrm{Spec}(B)$ est un idéal de $B$ (nécessairement maximal) tel que $f(q) = m$. On a

$$
\mathrm{prof}_{A_m}(N_m) = \mathrm{prof}_{B_m}(mB_m; N_m) = \inf_{q \in f^{-1}(m)} (\mathrm{prof}_{B_q}(N_q))
$$

(§ 1, n° 3, prop. 4 et n° 5, prop. 8), et

$$
\dim_{A_m}(N_m) = \dim_{B_m}(N_m) = \sup_{q \in f^{-1}(m)} (\dim_{B_q}(N_q))
$$

(VIII, § 2, n° 3, th. 1 et § 1, n° 4, prop. 9). Comme on a $\mathrm{prof}_{B_q}(N_q) \leq \dim_{B_q}(N_q)$ pour tout $q \in f^{-1}(m)$, la proposition résulte de ces égalités.

#### Corollaire 1 {#ac-x-s2-prop-8-cor-1 .statement}

Soit $\rho : A \to B$ un homomorphisme d’anneaux noethériens. Si $B$ est une $A$-algèbre finie et un $A$-module macaulayen, c’est un anneau de Macaulay. Si de plus $\rho$ est injectif, on a $\mathrm{ht}(aB) = \mathrm{ht}(a)$ pour tout idéal $a$ de $A$, et $\mathrm{ht}(b) = \mathrm{ht}(\rho^{-1}(b))$ pour tout idéal $b$ de $B$.

La première assertion résulte de la prop. 8. Supposons $\rho$ injectif. Soit $a$ un idéal de $A$. On a $\mathrm{ht}(a) = \mathrm{prof}_A(a; B)$ puisque le $A$-module $B$ est macaulayen, de support égal à $\mathrm{Spec}(A)$ (n° 1, cor. de la prop. 1), $\mathrm{ht}(aB) = \mathrm{prof}_B(aB; B)$ (*loc. cit.*) et $\mathrm{prof}_A(a; B) = \mathrm{prof}_B(aB; B)$ ($§ 1$, n° 3, prop. 4), d’où $\mathrm{ht}(aB) = \mathrm{ht}(a)$. Soit $b$ un idéal de $B$. D’après ce qui précède, on a $\mathrm{ht}(\rho^{-1}(b)) = \mathrm{ht}(\rho^{-1}(b)B)$. Mais $\rho^{-1}(b)B$ est contenu dans $b$, donc de hauteur inférieure à $\mathrm{ht}(b)$ et on a $\mathrm{ht}(b) \leq \mathrm{ht}(\rho^{-1}(b))$ d’après VIII, $§ 2$, n° 3, th. 1, b).

#### Corollaire 2 {#ac-x-s2-prop-8-cor-2 .statement}

Soient $A$ un anneau noethérien intégralement clos et $B$ un anneau contenant $A$. On suppose que $B$ est un $A$-module sans torsion, de type fini. Si $B$ est un anneau de Macaulay, le $A$-module $B$ est macaulayen.

En effet, deux idéaux premiers de $B$ qui sont au-dessus du même idéal de $A$ ont la même hauteur (VIII, $§ 2$, n° 3, th. 2). On peut donc appliquer la prop. 8 avec $N = B$.

#### Corollaire 3 {#ac-x-s2-prop-8-cor-3 .statement}

Soient $A$ un anneau intégralement clos, $K$ son corps des fractions, $L$ une $K$-algèbre finie telle que $[L : K] 1_A$ soit inversible dans $A$, et $B$ une sous-$A$-algèbre de $L$, finie sur $A$.

a) *Le sous*-A*-module* $Al_B$ de $B$ est facteur direct.

b) *Pour tout idéal* $J$ *de* $A$, *on a l’inégalité* $\mathrm{prof}_A(J; A) \geq \mathrm{prof}_B(JB; B)$.

c) *Si* $B$ *est un anneau de Macaulay*, *il en est de même de* $A$.

L’application $K$-linéaire $\mathrm{Tr}_{L/K} : L \to K$ applique $B$ dans $A$ (V, $§ 1$, n° 6, cor. 2 de la prop. 17), donc définit par restriction une application $A$-linéaire $t : B \to A$. Pour tout $x \in A$, on a $t(xl_B) = [L : K] x$, d’où a).

D’après la prop. 4 du $§ 1$, n° 3, on a $\mathrm{prof}_A(J; B) = \mathrm{prof}_B(JB; B)$; mais d’après a) et la remarque 4 du $§ 1$, n° 1, on a $\mathrm{prof}_A(J; A) \geq \mathrm{prof}_A(J; B)$, d’où b).

Si l’anneau $B$ est noethérien, il en est de même de $A$ : en effet, on a d’après a) $aB \cap A = a$ pour tout idéal $a$ de $A$; ainsi toute suite croissante $(a_n)_{n \in \mathbf{N}}$ d’idéaux de $A$ est stationnaire puisque la suite $(a_nB)_{n \in \mathbf{N}}$ est stationnaire. Sous les hypothèses de c), le $A$-module $B$ est macaulayen (cor. 2), et il en est de même du $A$-module $A$ (n° 1, exemple 2).

#### Exemple {#ac-x-s2-n6-exa-1 .statement}

Le corollaire 3 s’applique notamment dans les deux situations suivantes :

a) On considère un anneau noethérien intégralement clos $A$, une extension séparable $L$ de son corps des fractions, de degré fini $n$ tel que $n1_A$ soit inversible dans $A$, et on prend pour $B$ la fermeture intégrale de $A$ dans $L$ (V, $§ 1$, n° 6, cor. 1 de la prop. 18).

b) On considère un anneau noethérien intégralement clos $B$ et un groupe fini $G$ d’automorphismes de $B$, tel que $\mathrm{Card}(G) 1_B$ soit inversible dans $B$. On prend pour $A$ l’anneau des éléments de $B$ invariants pour l’action de $G$. Vérifions que nous sommes dans un cas particulier de a). Le groupe $G$ opère sur le corps des

En particulier, si B est un anneau de Macaulay, il en est de même de A.

### 7. Modules macaulayens et algèbres plates

#### Proposition 9 {#ac-x-s2-prop-9 .statement}

Soient ρ : A → B un homomorphisme d’anneaux noethériens, M un A-module de type fini et N un B-module de type fini, plat sur A. Notons $^a\rho : \mathrm{Spec}(B) \longrightarrow \mathrm{Spec}(\Lambda)$ l’application associée à ρ. Les conditions suivantes sont équivalentes :

(i) le B-module $M \otimes_A N$ est macaulayen ;
(ii) le $(\kappa(p) \otimes_A B)$-module $\kappa(p) \otimes_A N$ est macaulayen pour tout $p \in \mathrm{Supp}_A(M)$, et le $A_p$-module $M_p$ est macaulayen pour tout $p \in ^a\rho(\mathrm{Supp}_B(N))$ ;
(iii) pour tout idéal maximal de $\mathrm{Supp}_B(N)$ dont l’image inverse $p$ dans A appartient à $\mathrm{Supp}_A(M)$, le $A_p$-module $M_p$ et le $(\kappa(p) \otimes_A B)$-module $\kappa(p) \otimes_A N$ sont macaulayens.

Si de plus le B-module N est fidèlement plat, ces conditions entraînent que le A-module M est macaulayen.

Soit q un idéal premier de B appartenant au support de $M \otimes_A N$. Posons $p = \rho^{-1}(q)$. Comme le module $(M \otimes_A N)_q$ s’identifie à $M_p \otimes_{A_p} N_q$, les modules $M_p$ et $N_q$ sont non nuls, et il en est de même de $\kappa(p) \otimes_A N_q$ (n° 6, remarque). Le $A_p$-module $N_q$, étant isomorphe à un module de fractions de $N_p$, est plat et on a les égalités

$$
\mathrm{prof}_{B_q}((M \otimes_A N)_q) = \mathrm{prof}_{A_p}(M_p) + \mathrm{prof}_{B_q}(\kappa(p) \otimes_A N_q)
$$
$$
\dim_{B_q}((M \otimes_A N)_q) = \dim_{A_p}(M_p) + \dim_{B_q}(\kappa(p) \otimes_A N_q)
$$

(§ 1, n° 6, prop. 11, b) et remarque), dans lesquelles chaque terme est un entier $\geq 0$. Compte tenu du fait que le $B_q$-module $\kappa(p) \otimes_A N_q$ est macaulayen si et seulement s’il l’est en tant que $(\kappa(p) \otimes_A B_q)$-module (n° 1, exemple 4), on en déduit l’équivalence des deux conditions suivantes :

(α) le $B_q$-module $(M \otimes_A N)_q$ est macaulayen ;
(β) le $A_p$-module $M_p$ et le $(\kappa(p) \otimes_A B_q)$-module $\kappa(p) \otimes_A N_q$ sont macaulayens.

Prouvons maintenant que (iii) implique (i). Soient n un idéal maximal de B appartenant au support de $M \otimes_A N$, et $p = \rho^{-1}(n)$. On a d’après ce qui précède $p \in \mathrm{Supp}_A(M) \cap ^a\rho(\mathrm{Supp}_B(N))$ ; la condition (iii) et la remarque du n° 6 entraînent que la condition (β) ci-dessus est satisfaite avec $q = n$. Il en résulte que le $B_n$-module $(M \otimes_A N)_n$ est macaulayen, d’où (i).

L’implication (ii) ⇒ (iii) est claire ; prouvons que (i) implique (ii). Supposons le B-module M ⊗_A N macaulayen. Soit p un élément de Supp_A(M). On peut supposer que le (κ(p) ⊗_A B)-module κ(p) ⊗_A N est non nul, c’est-à-dire qu’il existe un idéal premier q de Supp_B(N) au-dessus de p (n° 6, remarque). Le B_q-module (M ⊗_A N)_q est macaulayen (n° 1, exemple 3) ; il résulte de l’implication (α) ⇒ (β) démontrée précédemment et de la remarque du n° 6 que le A_p-module M_p et le (κ(p) ⊗_A B)-module (κ(p) ⊗_A N) sont macaulayens, d’où (ii).

Si de plus N est fidèlement plat sur A, on a κ(p) ⊗_A N ≠ 0 pour tout p ∈ Spec(A), d’où a_p(Supp_B(N)) = Spec(A) (n° 6, remarque), de sorte que (ii) implique que M est macaulayen.

#### Corollaire 1 {#ac-x-s2-prop-9-cor-1 .statement}

Soient ρ : Λ → B un homomorphisme local d’anneaux locaux noethériens, M un A-module non nul de type fini et N un B-module non nul de type fini qui est un A-module plat. Pour que le B-module M ⊗_A N soit macaulayen, il faut et il suffit que le A-module M soit macaulayen et que le B/m_A B-module N/m_A N soit macaulayen.

En effet, N est un A-module fidèlement plat puisque N/m_A N est non nul (I, § 3, n° 1, définition 1).

#### Corollaire 2 {#ac-x-s2-prop-9-cor-2 .statement}

Soit ρ : A → B un homomorphisme d’anneaux noethériens faisant de B un A-module fidèlement plat et soit M un A-module de type fini. Pour que le B-module M ⊗_A B soit macaulayen, il faut et il suffit que le A-module M soit macaulayen et que κ(p) ⊗_Λ B soit un anneau de Macaulay pour tout p ∈ Supp(M).

#### Corollaire 3 {#ac-x-s2-prop-9-cor-3 .statement}

Soient A un anneau noethérien, B une Λ-algèbre finie et plate, M un A-module de type fini et macaulayen. Le B-module M ⊗_A B est macaulayen.

En effet, pour tout p ∈ Spec(A), l’anneau κ(p) ⊗_Λ B est une κ(p)-algèbre finie, donc est de Macaulay (n° 5, exemple 1), et on applique la prop. 9.

#### Corollaire 4 {#ac-x-s2-prop-9-cor-4 .statement}

Soient A un anneau noethérien, J un idéal de A et M un A-module de type fini. Notons Ā et Ĝ les séparés complétés de A et M pour la topologie J-adique, et S la partie multiplicative 1 + J de Λ. Considérons les conditions suivantes :

(i) le A-module M est macaulayen ;
(ii) le Ā-module Ĝ est macaulayen ;
(iii) le S^{-1}A-module S^{-1}M est macaulayen ;
(iv) pour tout idéal maximal m ∈ Supp(M) ∩ V(J), le A_m-module M_m est macaulayen ;
(v) pour tout idéal premier p ∈ Supp(M) tel que p + J ≠ A, le Λ_p-module M_p est macaulayen et l’anneau κ(p) ⊗_A Ā est de Macaulay.

Les conditions (ii) à (v) sont équivalentes, et sont entraînées par (i). Lorsque l’idéal J est contenu dans le radical de A, les conditions (i) à (v) sont équivalentes.

On sait que (i) implique (iii) (n° 1, exemple 3), et (iii) est identique à (i) lorsque J est contenu dans le radical de A (puisque les éléments de S sont alors inversibles).

Il est clair que (v) implique (iv) et que (iv) implique (i).

(i) $\Rightarrow$ (ii) : Soit $m$ un idéal maximal de $A$ ; alors $m\widehat{A}$ est un idéal maximal de $\widehat{A}$ au-dessus de $m$, et tout idéal maximal de $\widehat{A}$ est obtenu de cette façon (III, § 3, n° 4, prop. 8). L’anneau $\kappa(m) \otimes_A \widehat{A}$ est un corps, donc un anneau de Macaulay ; si le $A$-module $M$ est macaulayen, il en est de même du $\widehat{A}$-module $\widehat{M}$ d’après l’implication (iii) $\Rightarrow$ (i) de la prop. 9.

(ii) $\Rightarrow$ (v) : Le $\widehat{A}$-module $\widehat{M}$ est isomorphe à $M \otimes_A \widehat{A}$ (III, § 3, n° 4, th. 3) ; s’il est macaulayen, il résulte de la prop. 9, (i) $\Rightarrow$ (ii) que $\kappa(p) \otimes_A \widehat{A}$ est un anneau de Macaulay pour tout $p \in \mathrm{Supp}(M)$, et que le $A$-module $M$ est macaulayen.

#### Proposition 10 {#ac-x-s2-prop-10 .statement}

*Soit $\rho : A \to B$ un homomorphisme d’anneaux noethériens faisant de $B$ un $\Lambda$-module plat. Les conditions suivantes sont équivalentes :*

(i) $B$ est un anneau de Macaulay ;
(ii) pour tout idéal premier $q$ de $B$, les anneaux $A_{\rho^{-1}(q)}$ et $\kappa(\rho^{-1}(q)) \otimes_A B$ sont de Macaulay ;
(iii) pour tout idéal maximal $n$ de $B$, les anneaux $A_{\rho^{-1}(n)}$ et $\kappa(\rho^{-1}(n)) \otimes_A B$ sont de Macaulay.

*Si de plus $B$ est fidèlement plat sur $A$, ces conditions entraînent que $A$ est un anneau de Macaulay.*

C’est le cas particulier $M = A$, $N = B$ de la prop. 9.

#### Corollaire 1 {#ac-x-s2-prop-10-cor-1 .statement}

*Toute algèbre finie et plate sur un anneau de Macaulay est un anneau de Macaulay.*

#### Corollaire 2 {#ac-x-s2-prop-10-cor-2 .statement}

*Soient $A$ un anneau de Macaulay et $n$ un entier positif ; alors $A[X_1, \ldots, X_n]$ et $A[[X_1, \ldots, X_n]]$ sont des anneaux de Macaulay.*

Il suffit de traiter le cas $n = 1$. L’anneau $A[T]$ est noethérien (A, VIII, § 1, n° 4, cor. 1), et, pour tout corps $k$, l’anneau $k[T]$ est un anneau de Macaulay (n° 5, exemple 2) ; par conséquent, l’anneau $A[T]$ est de Macaulay (prop. 10) et l’anneau $A[[T]]$ est de Macaulay (cor. 4 de la prop. 9).

#### Corollaire 3 {#ac-x-s2-prop-10-cor-3 .statement}

*Toute algèbre de type fini sur un anneau noethérien de Macaulay est caténaire.*

En effet, une telle algèbre est un quotient d’un anneau de polynômes sur un anneau de Macaulay, donc un quotient d’un anneau de Macaulay (cor. 2), et par suite est caténaire (n° 2).

## EXERCICES {#ac-x-s2-exercises}

See the [exercises for § 2](exercises/s2/).
