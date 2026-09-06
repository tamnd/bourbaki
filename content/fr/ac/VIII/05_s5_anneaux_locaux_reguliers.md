---
book: ac
book_title: Commutative Algebra
chapter: VIII
chapter_title: DIMENSION
section: 5
section_title: Anneaux locaux réguliers
lang: fr
source: ac-viii-ix-fr
book_pages: AC VIII.51-AC VIII.62, AC VIII.94-AC VIII.99
pdf_pages: 0055-0066, 0098-0103
extraction: ocr
subsections:
    - "no": 1
      title: Définition des anneaux locaux réguliers
      page: 51
      pdf_page: 55
    - "no": 2
      title: Anneau gradué associé à un anneau local régulier
      page: 0
      pdf_page: 57
    - "no": 3
      title: Quotients d’anneaux locaux réguliers
      page: 55
      pdf_page: 59
    - "no": 4
      title: Polynômes d’Eisenstein
      page: 56
      pdf_page: 60
statements: 31
exercises: 32
content_sha256: 6ad3c554aa21f75c5b44d1656b413c9e3aa4fcc3784dcd6abbdea8c83ca23186
---

## § 5. ANNEAUX LOCAUX RÉGULIERS

### 1. Définition des anneaux locaux réguliers

Soit A un anneau local noethérien. Soit $(x_i)_{i \in I}$ une famille d’éléments de $m_A$. D’après le cor. 2 à la prop. 4 de II, § 3, no 2, il revient au même de supposer que la famille $(x_i)_{i \in I}$ engendre l’idéal $m_A$ de A, ou que les classes des $x_i$ modulo $m_A^2$ engendrent le $\kappa_A$-espace vectoriel $m_A/m_A^2$; s’il en est ainsi, on a $\dim(A) \leq \mathrm{Card}(I)$ d’après le scholie du § 3, no 2. On a donc l’inégalité

$$
\dim(A) \leq [m_A/m_A^2 : \kappa_A] \leq \mathrm{Card}(I)
$$

pour toute famille $(x_i)_{i \in I}$ engendrant l’idéal $m_A$ de A.

#### Définition 1 {#ac-viii-s5-def-1 .statement}

On dit que l’anneau local noethérien $A$ est régulier si l’on a $\dim(A) = [\mathfrak{m}_A/\mathfrak{m}_A^2 : \kappa_A]$. On appelle alors système de coordonnées de $A$ toute famille d’éléments de $\mathfrak{m}_A$ dont les classes modulo $\mathfrak{m}_A^2$ forment une base du $\kappa_A$-espace vectoriel $\mathfrak{m}_A/\mathfrak{m}_A^2$.

Un système de coordonnées dans un anneau local noethérien régulier $A$ est donc une famille finie $(x_i)_{i \in I}$ engendrant l’idéal $\mathfrak{m}_A$ de $A$ et telle que $\mathrm{Card}(I) = \dim(A)$. Réciproquement, si l’idéal $\mathfrak{m}_A$ d’un anneau local noethérien $A$ est engendré par $d$ éléments avec $d \leq \dim(A)$, l’anneau $A$ est régulier.

#### Exemple 1 {#ac-viii-s5-n1-exa-1 .statement}

Les anneaux locaux noethériens réguliers de dimension 0 (resp. 1) sont les corps (resp. les anneaux de valuation discrète) (VI, § 3, no 6, prop. 9 et cor. 1 du th. 1 ci-dessous). Soit $A$ un anneau de valuation discrète ; alors un élément $t$ de $\mathfrak{m}_A$ est une uniformisante si et seulement si $\{ t \}$ est un système de coordonnées de $A$.

#### Exemple 2 {#ac-viii-s5-n1-exa-2 .statement}

Soit $k$ un corps et soit $n$ un entier positif. L’anneau de séries formelles $k[[X_1, ..., X_n]]$ est un anneau local noethérien régulier de dimension $n$ (§ 3, no 4, cor. 3 à la prop. 8). Soient $F_1, ..., F_n$ des séries formelles sans terme constant dans $k[[X_1, ..., X_n]]$; pour que la suite $(F_1, ..., F_n)$ soit un système de coordonnées de $k[[X_1, ..., X_n]]$, il faut et il suffit que la matrice $\left( \frac{\partial F_i}{\partial X_j}(0, ..., 0) \right)$ soit inversible.

Plus généralement, soit $A$ un anneau local noethérien régulier de dimension $r$; alors $A[[X_1, ..., X_n]]$ est un anneau local noethérien régulier de dimension $r + n$. Si $(a_1, ..., a_r)$ est un système de coordonnées de $A$, alors $(a_1, ..., a_r, X_1, ..., X_n)$ est un système de coordonnées de $A[[X_1, ..., X_n]]$.

#### Exemple 3 {#ac-viii-s5-n1-exa-3 .statement}

Soit $A$ un anneau local noethérien régulier complet de dimension $r$. L’anneau $A \{ X_1, ..., X_n \}$ des séries formelles restreintes est local noethérien régulier de dimension $r + n$ (§ 3, no 4, remarque 1). Si $(a_1, ..., a_r)$ est un système de coordonnées de $A$, alors $(a_1, ..., a_r, X_1, ..., X_n)$ est un système de coordonnées de $A \{ X_1, ..., X_n \}$.

#### Exemple 4 {#ac-viii-s5-n1-exa-4 .statement}

\* Soit $k$ un corps valué complet non discret. L’anneau des séries formelles à $n$ variables qui convergent dans un voisinage de 0 dans $k^n$ est un anneau local noethérien régulier de dimension $n$ (§ 3, no 4, remarque 2).

#### Exemple 5 {#ac-viii-s5-n1-exa-5 .statement}

Soient $k$ un corps, $A$ une $k$-algèbre intègre de type fini et $m$ un idéal maximal de $A$. L’anneau local noethérien $A_m$ est régulier si et seulement si l’on a $\dim(A) = [m/m^2 : A/m]$ : en effet, on a $\dim(A_m) = \dim(A)$ (§ 2, no 4, cor. 2 au th. 3) et les espaces vectoriels $m/m^2$ et $mA_m/(mA_m)^2$ sur le corps $A/m$ sont isomorphes (II, § 3, no 3, prop. 9). En particulier, si $k$ est algébriquement clos, la condition énoncée équivaut à $\dim(A) = [m/m^2 : k]$ (V, § 3, no 3, prop. 1).

#### Exemple 6 {#ac-viii-s5-n1-exa-6 .statement}

\* Soit $X$ une variété algébrique sur un corps parfait $k$. Alors $X$ est non singulière en un point $x$ si et seulement si l’anneau local de $X$ en $x$ est régulier.

#### Exemple 7 {#ac-viii-s5-n1-exa-7 .statement}

\* Soit $A$ un anneau local noethérien régulier. On verra plus tard que l’anneau local noethérien $A_p$ est régulier pour tout idéal premier $p$ de $A$.

#### Proposition 1 {#ac-viii-s5-prop-1 .statement}

Soient $A$ et $B$ des anneaux locaux noethériens et $\rho : A \to B$ un homomorphisme local faisant de $B$ un $A$-module plat. On suppose que l’on a m_B = B.\rho(m_A). On a alors dim(A) = dim(B) et B est régulier si et seulement si A est régulier.

La première assertion résulte du cor. 1 de la prop. 7 du § 3, no 4. Comme B est plat sur A, on peut identifier m_B^k = B.\rho(m_A^k) à B \otimes_A m_A^k pour tout entier k \geqslant 0, donc m_B/m_B^2 à B \otimes_A (m_A/m_A^2) ou encore à \kappa_B \otimes_{\kappa_A} (m_A/m_A^2). On a donc

(2)
$$
[m_B/m_B^2 : \kappa_B] = [m_A/m_A^2 : \kappa_A],
$$
d’où aussitôt la proposition.

#### Corollaire {#ac-viii-s5-n1-cor-1 .statement}

Un anneau local noethérien A est régulier si et seulement si son complété $\hat{A}$ l’est.

En effet, $\hat{A}$ est plat sur A, et l’on a $m_{\hat{A}} = \hat{A}.m_A$ (III, § 3, no 4, th. 3 et § 2, no 12, cor. 2 à la prop. 16).

### 2. Anneau gradué associé à un anneau local régulier

#### Théorème 1 {#ac-viii-s5-thm-1 .statement}

Soit A un anneau local noethérien. Les conditions suivantes sont équivalentes :
(i) A est régulier.
(ii) L’idéal $m_A$ est engendré par une partie sécante pour A (§ 3, no 2, déf. 1).
(iii) L’idéal $m_A$ est engendré par une suite complètement sécante pour A (A, X, p. 157, déf. 2).
(iv) Soit S l’algèbre symétrique du $\kappa_A$-espace vectoriel $m_A/m_A^2$, et soit gr(A) = $\bigoplus_{n \geqslant 0} m_A^n/m_A^{n+1}$ l’anneau gradué associé à A. L’homomorphisme canonique $\gamma$ de S sur gr(A) est bijectif.
(v) Il existe un entier $r \geqslant 0$ tel que l’on ait $H_{A,m_A} = (1 - T)^{-r}$, c’est-à-dire $m_A = 0$ si $r = 0$ et $[m_A^n/m_A^{n+1} : \kappa_A] = \binom{n + r - 1}{r - 1}$ pour tout entier $n \geqslant 0$ si $r > 0$.
(vi) On a $H_{A,m_A} = (1 - T)^{-d}$ avec $d = \dim(A)$.

Si ces conditions sont remplies, tout système de coordonnées de A est une suite complètement sécante pour A.

(ii) \Rightarrow (i) : en effet, toute partie sécante a au plus $\dim(A)$ éléments (§ 3, no 2, th. 1).
(iii) \Rightarrow (ii) : en effet, toute suite complètement sécante est sécante (§ 3, no 2, corollaire de la prop. 3).
(iv) \Rightarrow (iii) : soit $(x_1, ..., x_r)$ une suite d’éléments de $m_A$ dont les classes modulo $m_A^2$ forment une base $(\xi_1, ..., \xi_r)$ de $m_A/m_A^2$ sur le corps $\kappa_A$. Si la propriété (iv) est satisfaite, gr(A) est l’algèbre de polynômes $\kappa_A[\xi_1, ..., \xi_r]$ et la suite $(x_1, ..., x_r)$ est complètement sécante (A, X, p. 160, th. 1). Ceci prouve aussi la dernière assertion du th. 1.
(i) \Rightarrow (iv) : posons $r = [m_A/m_A^2 : \kappa_A]$. D’après la formule (6) du § 4, no 2, la série de Poincaré de l’espace vectoriel gradué S sur le corps $\kappa_A$ est égale à

$$
P_S = \sum_{n \geqslant 0} [S^n(m_A/m_A^2) : \kappa_A] T^n = (1 - T)^{-r}.
$$

Supposons que l’homomorphisme canonique $\gamma : S \to \mathrm{gr}(A)$ ne soit pas bijectif. Comme $\gamma$ est surjectif, il existe un élément homogène $u$ de $S$, de degré $d > 0$, annulé par $\gamma$. On a alors

$$
H_{A,m_A} = P_S - P_{\mathrm{Ker}(\gamma)} \leq P_S - P_{uS} = (1 - T^d)/(1 - T)^r =
$$
$$
= (1 + T + \cdots + T^{d-1})/(1 - T)^{r-1}.
$$

D’après le th. 3 du § 4, n° 4 et le lemme 2 du § 4, n° 1, on a donc $\dim(A) < r$, et A n’est pas régulier.

Prouvons enfin l’équivalence des conditions (iv) à (vi). Or (iv) signifie que l’on a $H_{A,m_A} = (1 - T)^{-s}$ avec $s = [m_A/m_A^2 : \kappa_A]$. Donc les conditions (iv), (v), (vi) signifient que l’on a $H_{A,m_A} = (1 - T)^{-m}$, avec respectivement $m = [m_A/m_A^2 : \kappa_A]$, $m \geq 0$, $m = \dim(A)$. Mais, si l’on a $H_{A,m_A} = (1 - T)^{-m}$, on a $\dim(A) = m$ d’après § 4, n° 4, th. 3 et $[m_A/m_A^2 : \kappa_A] = m$ (puisque $(1 - T)^{-m} = 1 + mT + \cdots$). L’équivalence des conditions (iv) à (vi) en résulte aussitôt.

#### Corollaire 1 {#ac-viii-s5-thm-1-cor-1 .statement}

Tout anneau local noethérien régulier est intégralement clos, et en particulier intègre.

Supposons A régulier. Alors $\mathrm{gr}(A)$ est isomorphe à une algèbre de polynômes en un nombre fini d’indéterminées sur un corps (th. 1, (iv)). Par suite, $\mathrm{gr}(A)$ est un anneau noethérien intégralement clos (V, § 1, n° 3, cor. 3 de la prop. 13), et A est donc intégralement clos (V, § 1, n° 4, prop. 15).

Nous verrons dans un chapitre ultérieur que tout anneau local noethérien régulier est factoriel.

#### Corollaire 2 {#ac-viii-s5-thm-1-cor-2 .statement}

Soient A et B des anneaux locaux noethériens et $\sigma$ un homomorphisme local de B dans A. On suppose A régulier et B complet. Pour que $\sigma$ soit bijectif, il faut et il suffit qu’il induise des bijections de $\kappa_B$ sur $\kappa_A$ et de $m_B/m_B^2$ sur $m_A/m_A^2$.

La condition énoncée est évidemment nécessaire.

Supposons inversement que $\sigma$ induise des isomorphismes de $\mathrm{gr}_0(B)$ sur $\mathrm{gr}_0(A)$ et de $\mathrm{gr}_1(B)$ sur $\mathrm{gr}_1(A)$. Comme l’anneau $\mathrm{gr}(B)$ est engendré par $\mathrm{gr}_0(B) \cup \mathrm{gr}_1(B)$ et que $\mathrm{gr}(A)$ est l’algèbre symétrique de l’espace vectoriel $\mathrm{gr}_1(A)$ sur le corps $\mathrm{gr}_0(A)$, l’homomorphisme $\mathrm{gr}(\sigma)$ est bijectif. Par suite, $\sigma$ est bijectif (III, § 2, n° 8, cor. 3 du th. 1).

#### Corollaire 3 {#ac-viii-s5-thm-1-cor-3 .statement}

Soient k un corps et A une k-algèbre locale noethérienne, dont le corps résiduel est égal à k. Pour que A soit régulière, il faut et il suffit que son complété $\hat{A}$ soit isomorphe à une k-algèbre de séries formelles $k[[X_1, ..., X_n]]$.

Cela résulte de l’équivalence de (i) et (iv) dans le th. 1, et de la prop. 11 de III, § 2, n° 9.

### 3. Quotients d’anneaux locaux réguliers

#### Proposition 2 {#ac-viii-s5-prop-2 .statement}

Soient $A$ un anneau local noethérien, $x = (x_1, ..., x_r)$ une suite d’éléments de $m_A$ et $x$ l’idéal engendré par $x$. Les conditions suivantes sont équivalentes :

(i) l’anneau $A$ est régulier, et $x$ fait partie d’un système de coordonnées de $A$;
(ii) l’anneau $A/x$ est régulier et $x$ est une suite sécante pour $A$;
(iii) l’anneau $A/x$ est régulier et $x$ est une suite complètement sécante pour $A$.

En outre, lorsque ces conditions sont satisfaites, $x$ est un idéal premier de $A$.

(iii) $\Rightarrow$ (ii) : cela résulte du corollaire de la prop. 3 du § 3, no 2.

(ii) $\Rightarrow$ (i) : supposons que $x$ soit une suite sécante pour $A$ et que l’anneau local noethérien $A/x$ soit régulier. Soit $(x_{r+1}, ..., x_d)$ une suite d’éléments de $A$, dont les classes modulo $x$ forment un système de coordonnées de $A/x$. Alors la suite $(x_1, ..., x_d)$ engendre l’idéal $m_A$ de $A$, et l’on a

$$
\dim(A) = r + \dim(A/x) = r + (d - r) = d .
$$

Par suite, $A$ est régulier et $(x_1, ..., x_d)$ est un système de coordonnées de $A$.

(i) $\Rightarrow$ (iii) : si la condition (i) est satisfaite, la suite $x$ est complètement sécante (no 2, th. 1), donc sécante d’après le corollaire de la prop. 3 du § 3, no 2. On a donc

(3)
$$
\dim(A/x) = \dim(A) - r ;
$$

de plus, les classes de $x_1, ..., x_r$ modulo $m_A^2$ sont linéairement indépendantes sur le corps $\kappa_A$, et l’on a donc

(4)
$$
[m_A/(m_A^2 + x) : \kappa_A] = [m_A/m_A^2 : \kappa_A] - r .
$$

Les formules (3) et (4) montrent que $A/x$ est régulier.

Tout anneau local noethérien régulier est intègre d’après le cor. 1 du th. 1 du no 2. Par suite, $x$ est premier si $A/x$ est régulier.

#### Corollaire 1 {#ac-viii-s5-prop-2-cor-1 .statement}

Soient $A$ un anneau local noethérien, et $t$ un élément de $m_A$. Les conditions suivantes sont équivalentes :

(i) $A$ est régulier, et $t$ n’appartient pas à $m_A^2$;
(ii) $A/tA$ est régulier et $\dim(A/tA) < \dim(A)$;
(iii) $A/tA$ est régulier, et $t$ n’est pas diviseur de 0 dans $A$.

#### Corollaire 2 {#ac-viii-s5-prop-2-cor-2 .statement}

Soient $A$ un anneau local noethérien régulier, et $q$ un idéal de $A$. Alors $A/q$ est régulier si et seulement si $q$ est engendré par une partie d’un système de coordonnées de $A$.

La condition est suffisante d’après la prop. 2.

Supposons $A/q$ régulier, et soit $x = (x_1, ..., x_r)$ une suite d’éléments de $q$ dont les classes modulo $m_A^2$ forment une base de $(q + m_A^2)/m_A^2$ sur le corps $\kappa_A$. Soit $x$ l’idéal de $A$ engendré par $x$. On a donc $x \subset q$ et $x$ fait partie d’un système de coordonnées de $A$, donc l’anneau local noethérien $A/x$ est régulier (prop. 2); de plus, les espaces vectoriels $m_A/(q + m_A^2)$ et $m_A/(x + m_A^2)$ ont même dimension sur $\kappa_A$. Par suite, les anneaux locaux noethériens réguliers $A/q$ et $A/x$ ont même dimension. Comme les idéaux $q$ et $x$ sont premiers et que l’on a $x \subset q$, on a finalement $q = x$.

#### Exemple {#ac-viii-s5-n3-exa-1 .statement}

Soient $k$ un corps, $A = k[[X_1, ..., X_n]]$ et $q$ un idéal de $A$, distinct de $A$. Pour que $A/q$ soit régulier, il faut et il suffit qu’on puisse trouver un entier $r \geqslant 0$ et des éléments $F_1, ..., F_r$ de $A$, engendrant $q$, et tels que la matrice $\left( \frac{\partial F_i}{\partial X_j}(0, ..., 0) \right)$ soit de rang $r$ (« critère jacobien »). On a alors $\dim(A/q) = n - r$.

#### Remarque {#ac-viii-s5-n3-rem-1 .statement}

Soient $A$ un anneau local noethérien régulier et $q \subset m_A$ un idéal de $A$ tel que $A/q$ soit régulier. Soit $(x_1, ..., x_r)$ une suite d’éléments de $q$ dont les classes modulo $m_A^2$ engendrent l’espace vectoriel $(q + m_A^2)/m_A^2$ sur le corps $\kappa_A$. La démonstration du cor. 2 montre que l’idéal $q$ de $A$ est engendré par $(x_1, ..., x_r)$.

### 4. Polynômes d’Eisenstein

#### Définition 2 {#ac-viii-s5-def-2 .statement}

Soient $A$ un anneau, $p$ un idéal premier de $A$, et $P$ un polynôme de $A[T]$. On dit que $P$ est un polynôme d’Eisenstein pour $p$ s’il satisfait aux conditions suivantes :
a) $P$ est unitaire de degré $d \geqslant 1$;
b) on a $P(T) \equiv T^d \mod. pA[T]$;
c) on a $P(0) \notin p^2$.

Autrement dit, un polynôme d’Eisenstein pour $p$ est un polynôme de la forme $P(T) = T^d + \sum_{i=1}^d a_i T^{d-i}$, avec $d \geqslant 1$, où $a_1, ..., a_{d-1}$ appartiennent à $p$ et $a_d$ à $p - p^2$.

On dit que $P$ est un polynôme d’Eisenstein pour $pA_p$ si l’image canonique de $P$ dans l’anneau de polynômes $A_p[T]$ est un polynôme d’Eisenstein pour l’idéal $pA_p$; cela signifie aussi que $P$ est un polynôme d’Eisenstein pour $p$ et qu’il satisfait en outre à la condition suivante, plus forte que c) :
c’) tout élément $a$ de $A$ tel que $aP(0) \in p^2$ appartient à $p$.

#### Proposition 3 {#ac-viii-s5-prop-3 .statement}

Soient $A$ un anneau, $p$ un idéal premier de $A$ et $P \in A[T]$ un polynôme d’Eisenstein pour $p$.
a) Il n’existe pas de décomposition de la forme $P = P_1 P_2$ où $P_1$ et $P_2$ sont deux polynômes unitaires de $A[T]$ distincts de 1.
b) Supposons $A$ intégralement clos, de corps des fractions $K$. Alors $P$ est irréductible dans $K[T]$.

Soit $\varphi$ l’homomorphisme canonique de $A$ dans le corps des fractions $k$ de $A/p$ et soit $\varphi': A[T] \to k[T]$ l’extension de $\varphi$ telle que $\varphi'(T) = T$. Supposons qu’on ait $P = P_1P_2$ où $P_1$ et $P_2$ sont deux polynômes unitaires de $A[T]$ distincts de 1. On a alors $T^d = \varphi'(P_1)\varphi'(P_2)$ dans $k[T]$, en notant $d$ le degré de $P$. Si $d_i$ est le degré de $P_i$, on a donc $\varphi'(P_i) = T^{d_i}$, c’est-à-dire $P_i(T) \equiv T^{d_i} \mod pA[T]$, et en particulier $P_i(0) \in p$. Mais alors $P(0) = P_1(0).P_2(0)$ appartient à $p^2$ contrairement aux hypothèses. Ceci prouve a).

L’assertion b) résulte de a) et de la prop. 11 de V, § 1, no 3.

Soient $A$ un anneau local noethérien et $P_1, ..., P_r$ des polynômes unitaires dans $A[T]$, de degré $\geq 2$. Soit $q$ l’idéal de $A[T_1, ..., T_r]$ engendré par $P_1(T_1), ..., P_r(T_r)$ et soit $B$ la $A$-algèbre quotient $A[T_1, ..., T_r]/q$. Pour $1 \leq i \leq r$, on note $d_i$ le degré de $P_i$, $t_i$ la classe de $T_i$ modulo $q$, et $\gamma_i$ la classe de $c_i = P_i(0)$ modulo $m_A^2$. On suppose que l’on a $P_i(T) \equiv T^{d_i} \mod m_A A[T]$ pour $1 \leq i \leq r$.

**Proposition 4. — a)** *L’anneau $B$ est local et noethérien, d’idéal maximal*

$$
m_B = Bm_A + \sum_{i=1}^r Bt_i.
$$

*On a $\dim(A) = \dim(B)$ et $[\kappa_B : \kappa_A] = 1$. Les monômes $t_1^{\alpha(1)} ... t_r^{\alpha(r)}$, avec $0 \leq \alpha(i) < d_i$ pour $1 \leq i \leq r$, forment une base du $A$-module $B$.*

*b) Soit $\lambda$ l’homomorphisme canonique de $m_A/m_A^2$ dans $m_B/m_B^2$. Alors le noyau de $\lambda$ est le $\kappa_A$-espace vectoriel engendré par $\gamma_1, ..., \gamma_r$. Les classes des éléments $t_1, ..., t_r$ forment une base sur $\kappa_A$ du conoyau de $\lambda$.*

*c) Pour que $B$ soit régulier, il faut et il suffit que $A$ soit régulier et que $\gamma_1, ..., \gamma_r$ soient linéairement indépendants dans le $\kappa_A$-espace vectoriel $m_A/m_A^2$.*

La $A$-algèbre $B$ est isomorphe au produit tensoriel $B_1 \otimes_A \cdots \otimes_A B_r$ avec $B_i = A[T]/(P_i)$ pour $1 \leq i \leq r$. Il en résulte que les monômes $t_1^{\alpha(1)} ... t_r^{\alpha(r)}$, avec $0 \leq \alpha(i) < d_i$ pour $1 \leq i \leq r$, forment une base du $A$-module $B$. En particulier, $B$ est entier sur $A$, donc $A$ et $B$ ont même dimension d’après le th. 1 du § 2, no 3.

D’après le cor. 3 de la prop. 9 de IV, § 2, no 5, l’anneau $B$ est noethérien, et tout idéal maximal de $B$ contient $B.m_A$. Par ailleurs, vu l’hypothèse faite sur $P_1, ..., P_r$ et la relation $P_i(t_i) = 0$, on a $t_i^{d_i} \in B.m_A$ pour $1 \leq i \leq r$. Donc tout idéal maximal de $B$ contient $t_1, ..., t_r$, donc aussi l’idéal $q' = B.m_A + Bt_1 + \cdots + Bt_r$. Or on a $m_A = A \cap q'$ et $B = A + q'$, donc $B/q'$ est isomorphe à $A/m_A$ et $q'$ est un idéal maximal de $B$; par suite, $B$ est local et l’on a $[\kappa_B : \kappa_A] = 1$. Ceci prouve a).

Posons $r = m_A^2 + \sum_{i=1}^r Ac_i$, et notons $\varphi$ l’homomorphisme canonique de $(A/m_A^2)[T_1, ..., T_r]$ sur $B/m_B^2$. Comme on a $m_B = B.m_A + \sum_{i=1}^r Bt_i$, le noyau $n$ de $\varphi$ est l’idéal engendré par les classes $\overline{P}_i(T_i)$ des polynômes $P_i(T_i)$ modulo $m_A^2.A[T_1, ..., T_r]$ et les monômes $T_iT_j$ et $xT_i$ pour $1 \leq i, j \leq r$ et $x$ dans $m_A/m_A^2$. D’après l’hypothèse faite sur $P_i$, à savoir $P_i(T) \equiv T^{d_i} \mod m_A.A[T]$, on peut remplacer $\overline{P}_i(T_i)$ par $\gamma_i$ dans cette description de $n$; par suite, l’anneau $B/m_B^2$ est isomorphe au quotient de $(A/r)[T_1, ..., T_r]$ par l’idéal gradué engendré par les monômes $T_i T_j$ et $x T_i$ pour $x$ dans $m_A / r$. Notons $\tau_i$ la classe de $t_i$ modulo $m_B^2$; on a donc

$$
B / m_B^2 = (A/r) \oplus \kappa_A \tau_1 \oplus \cdots \oplus \kappa_A \tau_r,
$$

d’où

$$
m_B / m_B^2 = (m_A / r) \oplus \kappa_A \tau_1 \oplus \cdots \oplus \kappa_A \tau_r.
$$

L’assertion b) résulte aussitôt de là.

D’après la formule (6) et la relation $[ \kappa_B : \kappa_A ] = 1$, on a

$$
[m_B / m_B^2 : \kappa_B] = [m_A / m^2 : \kappa_A] + \{ r - [r / m_A^2 : \kappa_A] \}.
$$

Or, le $\kappa_A$-espace vectoriel $r / m_A^2$ est engendré par $\gamma_1, ..., \gamma_r$ et l’on a

$$
\dim(B) = \dim(A) \leq [m_A / m_A^2 : \kappa_A].
$$

L’assertion c) résulte aussitôt des formules (7) et (8).

#### Corollaire {#ac-viii-s5-n4-cor-1 .statement}

*Soit A un anneau local noethérien régulier et soit P $\in A[T]$ un polynôme d’Eisenstein pour $m_A$. L’anneau $B = A[T]/(P)$ est local noethérien régulier, de même dimension que A, et l’on a $[ \kappa_A : \kappa_B ] = 1$. Enfin, on a $m_B = B.m_A + Bt$, où t est la classe de T modulo (P).*

Le cas où P est de degré $\geq 2$ résulte de la prop. 4, où l’on fait $r = 1$; lorsque P est de degré 1, c’est-à-dire de la forme $T - c$ avec $c \in m_A$, le corollaire est immédiat.

#### Proposition 5 {#ac-viii-s5-prop-5 .statement}

*Soit A un anneau intègre, de corps des fractions K, et soit L une extension algébrique de degré fini de K. On note B la fermeture intégrale de A dans L et p un idéal premier de A.

Supposons que l’anneau local $A_p$ soit noethérien et régulier ; soit t un élément de L tel que $L = K(t)$ et supposons qu’il existe dans $A[T]$ un élément P, polynôme d’Eisenstein pour $pA_p$, dont t soit racine.

a) Il existe dans B un unique idéal premier q au-dessus de p.
b) L’anneau local $B_q$ est noethérien et régulier, de même dimension que $A_p$.
c) On a $B_q = A_p[t]$.
d) L’homomorphisme canonique de $A/p$ dans $B/q$ induit un isomorphisme des corps des fractions de ces anneaux.*

Posons $C = A_p[t]$ et notons d le degré de P. D’après la prop. 3 appliquée à l’anneau $A_p$, le polynôme d’Eisenstein P est irréductible dans $K[T]$ et $(1, t, ..., t^{d-1})$ est une base de L sur K, donc de C sur $A_p$. Comme P est unitaire, le noyau de l’homomorphisme canonique de $A_p[T]$ sur C est égal à (P). D’après le corollaire de la prop. 4 ci-dessus, C est donc un anneau local noethérien régulier de même dimension que $A_p$, l’idéal maximal $m_C$ de C est engendré par $p \cup \{ t \}$ et le corps $\kappa_C$ est une extension triviale du corps des fractions de $A/p$. Pour prouver la prop. 5, il suffit donc de montrer qu’il existe un unique idéal premier q de B au-dessus de p, et qu’on a $C = B_q$.

Posons S = A − p. On sait (V, § 1, n° 5, prop. 16) que la fermeture intégrale de

#### Corollaire {#ac-viii-s5-n4-cor-2 .statement}

Supposons que A_p soit un anneau de valuation discrète. Alors B_q est un anneau de valuation discrète, t est une uniformisante de B_q, et l’on a

$$
f(B_q/A_p) = 1 , \quad e(B_q/A_p) = [L : K]
$$

(VI, § 8, n° 1).

En effet, les anneaux de valuation discrète sont les anneaux locaux noethériens réguliers de dimension 1 ; posant d = [L : K], on a t^d \in m_A - m_A^2, d’où d = e(B_q/A_p). On a [\kappa_B : \kappa_A] = 1, d’où f(B_q/A_p) = 1.

#### Exemple 1 {#ac-viii-s5-n4-exa-1 .statement}

Posons A = \mathbf{Z} et L = \mathbf{Q}(p^{1/d}), où p est un nombre premier et d un entier \geqslant 2. Notons B la fermeture intégrale de \mathbf{Z} dans L. Comme le polynôme T^d - p de \mathbf{Z}[T] est un polynôme d’Eisenstein pour p\mathbf{Z}_{(p)}, il existe un unique idéal premier q de B au-dessus de p\mathbf{Z}. Il existe donc une unique valuation discrète normalisée v du corps \mathbf{Q}(p^{1/d}) telle que v(p) > 0 ; on a [L : K] = v(p) = d, et B/q est un corps à p éléments. L’anneau B_q de la valuation v est égal à \mathbf{Z}_{(p)}[p^{1/d}].

#### Exemple 2 {#ac-viii-s5-n4-exa-2 .statement}

Posons A = \mathbf{Z} et L = R_{pf}(\mathbf{Q}) où p est un nombre premier et f un entier \geqslant 1 (cf. A, V, p. 78). On a donc L = \mathbf{Q}(\zeta) avec \zeta = \exp(2\pi i/p^f). Soient B la fermeture intégrale de \mathbf{Z} dans L et P le polynôme de \mathbf{Z}[T] tel que

$$
P(T - 1) = (T^{p^f} - 1)/(T^{p^{f-1}} - 1) .
$$

Posons d = p^f - p^{f-1}. On a P(\zeta - 1) = 0, P(0) = p et

$$
P(T - 1) \equiv (T - 1)^d \mod. p\mathbf{Z}[T] ,
$$

d’où P(T) \equiv T^d. Par suite, P est un polynôme d’Eisenstein pour p\mathbf{Z}_{(p)}. Il y a donc un unique idéal premier q de B au-dessus de p\mathbf{Z}, et l’on a B_q = \mathbf{Z}_{(p)}[\zeta] ; de plus, \zeta - 1 est une uniformisante de B_q et l’on a

$$
[L : K] = d = p^f - p^{f-1} .
$$

Si v est l’unique valuation normalisée de \mathbf{Q}(\zeta) telle que v(p) > 0, on a v(p) = d. De plus, le corps B/q a p éléments. On peut prouver (cf. p. 96, exerc. 13) que B est égal à \mathbf{Z}[\zeta].

\* 5. Structure des anneaux locaux noethériens réguliers complets

Dans ce numéro, nous utilisons des définitions et des résultats du chapitre IX.

Soit A un anneau local noethérien régulier et complet ; notons $p$ la caractéristique de son corps résiduel $\kappa_A$, et distinguons deux cas.

A) $p = 0$. Alors (IX, § 3, no 3, th. 1), il existe un sous-corps K de A tel que la projection canonique de A sur $\kappa_A$ induise un isomorphisme de K sur $\kappa_A$. Appliquant alors le cor. 3 du th. 1 du no 2 à la K-algèbre A, on en déduit :

#### Proposition 6 {#ac-viii-s5-prop-6 .statement}

Soit A un anneau local noethérien régulier et complet, dont le corps résiduel $\kappa_A$ est de caractéristique 0. Posons $n = \dim(A)$. Alors A est isomorphe à l’anneau de séries formelles $\kappa_A[[X_1, ..., X_n]]$.

B) $p \neq 0$. On appelle sous-anneau de Cohen de A tout sous-anneau V de A qui est un $p$-anneau tel que $A = m_A + V$ (IX, § 2, no 2, déf. 2). L’anneau V est local ; son idéal maximal $m_V$ est engendré par $p.1_V$; par suite on a $m_A \cap V = m_V$ et l’injection canonique de V dans A définit par passage au quotient un isomorphisme du corps $\kappa_V$ sur le corps $\kappa_A$. Si $p.1_A = 0$, V est un corps de caractéristique $p$. Sinon V est un anneau de valuation discrète dont le corps des fractions est de caractéristique zéro (IX, § 2, no 1, cor. 1 à la prop. 1). On démontre (IX, no 2, th. 1) que A possède des sous-anneaux de Cohen.

#### Exemple 3 {#ac-viii-s5-n4-exa-3 .statement}

Soient k un corps de caractéristique $p \neq 0$ et $n$ un entier positif. L’anneau de séries formelles $k[[X_1, ..., X_n]]$ est local noethérien régulier complet, de dimension $n$ et k est un sous-anneau de Cohen de $k[[X_1, ..., X_n]]$.

#### Exemple 4 {#ac-viii-s5-n4-exa-4 .statement}

Soient V un anneau de valuation discrète complet et $n$ un entier positif. L’anneau de séries formelles $V_n = V[[X_1, ..., X_n]]$ est local noethérien régulier complet, de dimension $n + 1$, et V est un sous-anneau de Cohen de $V_n$.

#### Exemple 5 {#ac-viii-s5-n4-exa-5 .statement}

Gardons les notations précédentes. On dit qu’un polynôme P de $V_n[T]$ de degré $d \geq 2$ est spécial s’il est de la forme $T^d + \sum_{i=1}^d a_i T^{d-i}$, où $a_1, ..., a_{d-1}$ appartiennent à $m_{V_n}$, $a_d$ appartient à $m_V + m_{V_n}^2$ mais non à $m_{V_n}^2$. En particulier, P est un polynôme d’Eisenstein pour $m_{V_n}$. Posons $A = V_n[T]/(P)$. D’après le corollaire de la prop. 4 du no 4, l’anneau A est local noethérien régulier complet, de dimension $n + 1$. Si t est la classe de T modulo (P), la suite $(1, t, ..., t^{d-1})$ est une base du $V_n$-module A, et $(X_1, ..., X_n, t)$ est un système de coordonnées de A : en effet, il existe une uniformisante $\pi$ de V telle que $a_d \equiv \pi \mod. m_{V_n}^2$; comme on a aussi
$$
a_d = -t(t^{d-1} + a_1 t^{d-2} + \cdots + a_{d-1}),
$$
on a $\pi \in m_A^2$; comme $m_A$ est engendré par $\{\pi, X_1, ..., X_n, t\}$, cela prouve notre assertion. En outre, V est un sous-anneau de Cohen de A, car $\kappa_V$ s’identifie à $\kappa_{V_n}$, et $\kappa_{V_n}$ à $\kappa_A$ d’après le corollaire à la prop. 4 du no 4.

#### Théorème 2 {#ac-viii-s5-thm-2 .statement}

Soit $A$ un anneau local noethérien régulier et complet dont le corps résiduel est de caractéristique $\neq 0$, et soit $V$ un sous-anneau de Cohen de $A$. Posons $n = \dim(A)$.

a) Supposons que $V$ soit un corps. Alors la $V$-algèbre $A$ est isomorphe à l’algèbre de séries formelles $V[[X_1, ..., X_n]]$.

b) Supposons que $V$ soit un anneau de valuation discrète complet et que l’on ait $m_V \not\subset m_A^2$. Alors, la $V$-algèbre $A$ est isomorphe à l’algèbre de séries formelles $V[[X_1, ..., X_{n-1}]]$.

c) Supposons que $V$ soit un anneau de valuation discrète complet et que l’on ait $m_V \subset m_A^2$. Il existe alors un polynôme spécial $P$ dans $V[[X_1, ..., X_{n-1}]] [T]$ et un $V$-isomorphisme de $A$ sur $V[[X_1, ..., X_{n-1}]] [T]/(P)$.

L’assertion a) résulte aussitôt du cor. 3 du th. 1 du no 2.

Prouvons b). Soit $(x_1, ..., x_m)$ une suite d’éléments de $m_A$, et soit $\varphi_0$ l’homomorphisme de $V[X_1, ..., X_m]$ dans $A$ qui coïncide avec l’identité sur $V$ et envoie $X_i$ sur $x_i$ pour $1 \leq i \leq m$. Si $a$ est l’idéal de $V[X_1, ..., X_m]$ engendré par $X_1, ..., X_m$, on a $\varphi_0(a) \subset m_A$, donc $\varphi_0$ se prolonge par continuité en un homomorphisme $\varphi$ de $V_m = V[[X_1, ..., X_m]]$ dans $A$. Soit $\pi$ une uniformisante de $V$. D’après le cor. 2 du th. 1 du no 2, $\varphi$ est un isomorphisme de $V_m$ sur $A$ si et seulement si $(\pi, x_1, ..., x_m)$ est un système de coordonnées de $A$. Mais l’application canonique de $m_V/m_V^2$ dans $m_A/m_A^2$ est injective, puisque l’on a $m_V \not\subset m_A^2$ et que $m_V/m_V^2$ est de rang 1 sur $\kappa_V$. Donc $m_A/(m_V + m_A^2)$ est de rang $n - 1$ et $(\pi, x_1, ..., x_m)$ est un système de coordonnées de $A$ si et seulement si les classes des $x_i$ forment une base de $m_A/(m_V + m_A^2)$ sur $\kappa_V$. D’où b).

Prouvons c). Soit $(y_1, ..., y_n)$ un système de coordonnées de $A$. Comme ci-dessus, posons $V_n = V[[Y_1, ..., Y_n]]$ et considérons l’homomorphisme $\varphi$ de $V_n$ dans $A$ qui coïncide avec l’identité sur $V$ et envoie $Y_i$ sur $y_i$ pour $1 \leq i \leq n$. Alors $\mathrm{gr}(\varphi)$ est surjectif, donc $\varphi$ est surjectif (III, § 2, no 8, cor. 2 du th. 1). Le noyau $p$ de $\varphi$ est un idéal premier de $V_n$; comme on a

$$
\dim(V_n) = n + 1 = \dim(V_n/p) + 1,
$$

l’idéal premier $p$ est de hauteur 1 (§ 1, no 3, prop. 8). Mais l’anneau $V_n$ est factoriel d’après la prop. 8 de VII, § 3, no 9 ; par suite, l’idéal $p$ est principal (VII, § 3, no 2, th. 1).

Soit $R$ un générateur de l’idéal $p$ de $V_n$. D’après le lemme 3 de VII, § 3, no 7, il existe des entiers $u(1), ..., u(n-1)$ au moins égaux à 1, et un isomorphisme $\sigma$ de $V[[X_1, ..., X_{n-1}, T]]$ sur $V_n$ tels que

$$
\begin{align*}
\sigma(X_i) &= Y_i + Y_n^{u(i)} \quad \text{pour } 1 \leq i < n \\
\sigma(T) &= Y_n
\end{align*}
$$

et que $\sigma^{-1}(R) = Q$ satisfasse à $Q(0, ..., 0, T) \neq 0$. De plus, d’après le théorème de préparation (VII, § 3, n° 8, prop. 6), il existe un polynôme P dans V[[X_1, ..., X_{n-1}]] [T] de la forme

$$
P = T^d + \sum_{i=1}^d a_i(X_1, ..., X_{n-1}) T^{d-i},
$$

engendrant le même idéal que Q dans V[[X_1, ..., X_{n-1}, T]], et tel que $a_i(0, ..., 0) \in m_V$ pour $1 \leq i \leq d$. On en déduit que A est V-isomorphe à V[[X_1, ..., X_{n-1}, T]]/(P). Mais V[[X_1, ..., X_{n-1}, T]] est somme directe de l’idéal (P) et du sous-V[[X_1, ..., X_{n-1}]]-module de base 1, T, ..., $T^{d-1}$ (VII, § 3, n° 8, prop. 5); par suite, A est V-isomorphe à V[[X_1, ..., X_{n-1}]] [T]/(P).

Posons C = V[[X_1, ..., X_{n-1}]] et notons α la classe de $a_d(X_1, ..., X_{n-1})$ modulo $m_C^2$. On a $\kappa_V = \kappa_C = \kappa_A$. D’après la prop. 4 du n° 4, le noyau de l’homomorphisme canonique de $m_C/m_C^2$ dans $m_A/m_A^2$ est égal à $\kappa_C \alpha$. Comme l’image de $m_V/m_V^2$ dans $m_A/m_A^2$ est nulle et que $m_V/m_V^2$ est de rang 1 sur $\kappa_C$, il en résulte que $a_d$ appartient à $m_V + m_C^2$, mais non à $m_C^2$. Par conséquent, le polynôme P est spécial, ce qu’on voulait démontrer.

\* Remarque. — Soient k un corps, A une k-algèbre noethérienne locale complète régulière. Lorsque $\kappa_A$ n’est pas une extension séparable de k, il n’est pas vrai en général que A soit isomorphe comme k-algèbre à $\kappa_A[[T_1, ..., T_n]]$ où $n = \dim(A)$ (p. 98, exerc. 29). \*

## EXERCICES {#ac-viii-s5-exercises}

See the [exercises for § 5](exercises/s5/).
