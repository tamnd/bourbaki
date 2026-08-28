---
book: ac
book_title: Commutative Algebra
chapter: III
chapter_title: Graduations, filtrations et topologies
section: 1
section_title: Algèbres graduées de type fini
lang: fr
source: ac-i-iv-fr
pdf_pages: 0181-0190, 0278-0279
extraction: ocr
subsections:
    - "no": 1
      title: Systèmes de générateurs d’une algèbre commutative.
      page: 0
      pdf_page: 181
    - "no": 2
      title: Critères de finitude pour les anneaux gradués.
      page: 0
      pdf_page: 183
    - "no": 3
      title: Propriétés de l’anneau $A^{(d)}$.
      page: 0
      pdf_page: 184
    - "no": 4
      title: Idéaux premiers gradués.
      page: 0
      pdf_page: 187
statements: 13
exercises: 3
content_sha256: cefdabf8444c22722d075e8e5b095d8320f52ed3cbb929bd8070daf4172e4127
---

## § 1. Algèbres graduées de type fini.

### 1. Systèmes de générateurs d’une algèbre commutative.

Soient A un anneau commutatif, B une A-algèbre commutative. Rappelons (Alg., chap. IV, § 2, n° 1) que si $x = (x_i)_{i \in I}$ est une famille d’éléments de B, l’application $f \to f(x)$ de l’algèbre de polynômes $A[X_i]_{i \in I}$ dans B est un homomorphisme de $A[X_i]_{i \in I}$ sur la sous-algèbre de B engendrée par les $x_i$, dont le noyau $\alpha$ est l’idéal des polynômes $f$ tels que $f(x) = 0$, appelé idéal des relations algébriques (à coefficients dans A) entre les $x_i$.

#### Définition 1 {#ac-iii-s1-def-1 .statement}

Dans une algèbre commutative B sur un anneau commutatif A, on dit qu’une famille $(x_i)_{i \in I}$ d’éléments de B

(*) Sauf au § 5, qui utilise les résultats du chap. I, § 4, et par suite l’algèbre homologique, il n’est fait, dans ce chapitre, aucun usage d’autres Livres de la Deuxième Partie.

est algébriquement libre sur $A$ (ou que les $x_i$ sont algébriquement indépendants sur $A$) si l’idéal des relations algébriques entre les $x_i$, à coefficients dans $A$, est réduit à 0. Une famille $(x_i)$ qui n’est pas algébriquement libre sur $A$ est encore dite algébriquement liée sur $A$ (et on dit aussi que ses éléments sont algébriquement dépendants sur $A$).

Cette définition généralise celle donnée en Alg., chap. V, § 5, no 1, déf. 1 pour les familles d’éléments d’un corps commutatif.

Dire que la famille $(x_i)_{i \in I}$ est algébriquement libre sur $A$ revient encore à dire que les monômes $\prod_i x_i^{n_i}$ par rapport aux $x_i$ sont linéairement indépendants sur $A$; en particulier les $x_i$ sont alors linéairement indépendants sur $A$.

#### Définition 2 {#ac-iii-s1-def-2 .statement}

On dit qu’une algèbre commutative $B$ sur un anneau commutatif $A$ est de type fini si elle est engendrée par une famille finie d’éléments.

Il revient au même de dire que $B$ est isomorphe à une $A$-algèbre de la forme $A[X_1, ..., X_n]/\alpha$ (où les $X_i$ sont des indéterminées et $\alpha$ un idéal de l’anneau de polynômes $A[X_1, ..., X_n]$).

Si la $A$-algèbre $B$ est un $A$-module de type fini, elle est évidemment une $A$-algèbre de type fini ; la réciproque est fausse, comme le montre l’exemple des algèbres de polynômes (cf. chap. V).

Si $B$ est une $A$-algèbre de type fini et $A'$ une $A$-algèbre commutative quelconque, $B_{(A')} = B \otimes_A A'$ est une $A'$-algèbre de type fini, car si $(x_i)_{i \in I}$ est un système de générateurs de la $A$-algèbre $B$, il est clair que les $x_i \otimes 1$ forment un système de générateurs de la $A'$-algèbre $B_{(A')}$.

Si $B$ est une $A$-algèbre de type fini, et $C$ une $B$-algèbre de type fini, alors $C$ est une $A$-algèbre de type fini ; en effet, il résulte aussitôt des définitions que si $(b_\lambda)_{\lambda \in L}$ est un système de générateurs de la $A$-algèbre $B$ et $(c_\mu)_{\mu \in M}$ un système de générateurs de la $B$-algèbre $C$, tout élément de $C$ est égal à un polynôme à coefficients dans $A$, par rapport aux $b_\lambda$ et aux $c_\mu$.

### 2. Critères de finitude pour les anneaux gradués.

Dans ce no et les suivants, toutes les graduations envisagées (Alg., chap. II, 3e éd., § 11) sont supposées de type $\mathbf{Z}$. Si A (resp. M) est un anneau gradué (resp. un module gradué), on note $A_i$ (resp. $M_i$) l’ensemble des éléments homogènes de degré i de A (resp. M).

Si $A_i = \{0\}$ (resp. $M_i = \{0\}$) pour $i < 0$, on dira, pour abréger, que A (resp. M) est un anneau (resp. un module) gradué à degrés positifs.

#### Proposition 1 {#ac-iii-s1-prop-1 .statement}

Soient $A = \bigoplus_{i \in \mathbf{Z}} A_i$ un anneau commutatif gradué à degrés positifs, m l’idéal gradué $\bigoplus_{i \geq 1} A_i$, $(x_\lambda)_{\lambda \in L}$ une famille d’éléments homogènes de A, de degrés $\geq 1$. Les conditions suivantes sont équivalentes :

a) L’idéal de A engendré par la famille $(x_\lambda)$ est égal à m.
b) La famille $(x_\lambda)$ est un système de générateurs de la $A_0$-algèbre A.
c) Pour tout $i \geq 0$, le $A_0$-module $A_i$ est engendré par les éléments de la forme $\prod_\lambda x_\lambda^{n_\lambda}$ qui sont de degré i dans A.

Il est clair que les conditions b) et c) sont équivalentes. Si elles sont vérifiées, tout élément de m est de la forme $f((x_\lambda))$ où $f$ est un polynôme de $A_0[X_\lambda]_{\lambda \in L}$ sans terme constant ; on a donc $m = \sum_{\lambda \in L} A x_\lambda$, ce qui prouve que c) entraîne a). Inversement, supposons vérifiée la condition a). Soit $A' = A_0[x_\lambda]_{\lambda \in L}$ la sous-$A_0$-algèbre de A engendrée par la famille $(x_\lambda)$, et montrons que $A' = A$. Pour cela, il suffit de montrer que $A_i \subset A'$ pour tout $i \geq 0$. Procédons par récurrence sur $i$, la propriété étant évidente pour $i = 0$. Soit donc $y \in A_i$ avec $i \geq 1$. Puisque $y \in m$, il existe une famille $(a_\lambda)_{\lambda \in L}$ d’éléments de A, de support fini, telle que $y = \sum_\lambda a_\lambda x_\lambda$, et on peut supposer chacun des $a_\lambda$ homogène et de degré $i - \deg(x_\lambda)$ (en le remplaçant au besoin par sa composante homogène de ce degré) ; comme $\deg(x_\lambda) > 0$, l’hypothèse de récurrence montre que l’on a $a_\lambda \in A'$ pour tout $\lambda \in L$, d’où $y \in A'$ et $A_i \subset A'$, ce qui achève de prouver que a) implique b).

#### Corollaire {#ac-iii-s1-n2-cor-1 .statement}

Soient $A = \bigoplus_{i \in \mathbf{Z}} A_i$ un anneau commutatif gradué à degrés positifs et $m$ l’idéal gradué $\bigoplus_{i \geq 1} A_i$.

(i) Les conditions suivantes sont équivalentes :
a) L’idéal $m$ est un $A$-module de type fini.
b) L’anneau $A$ est une $A_0$-algèbre de type fini.

(ii) Supposons vérifiées les conditions de (i) et soit $M = \bigoplus_{i \in \mathbf{Z}} M_i$ un $A$-module gradué de type fini. Alors, pour tout $i \in \mathbf{Z}$, $M_i$ est un $A_0$-module de type fini, et il existe $i_0$ tel que $M_i = \{ 0 \}$ pour $i < i_0$.

(i) Si une famille $(y_\mu)$ d’éléments de $A$ est un système de générateurs du $A$-module $m$ (resp. de la $A_0$-algèbre $A$), il en est de même de la famille formée des composantes homogènes des $y_\mu$; l’équivalence des conditions a) et b) résulte donc de la prop. 1.

(ii) On peut supposer $A$ engendré (en tant que $A_0$-algèbre) par des éléments homogènes $a_i$ ($1 \leq i \leq r$) de degrés $\geq 1$, et $M$ engendré (en tant que $A$-module) par des éléments homogènes $x_j$ ($1 \leq j \leq s$); soit $h_i = \deg(a_i)$, $k_j = \deg(x_j)$. Il est clair que $M_n$ est formé des combinaisons linéaires à coefficients dans $A_0$ des éléments $a_1^{\alpha_1} a_2^{\alpha_2} \ldots a_r^{\alpha_r} x_j$ tels que les $\alpha_i$ soient des entiers $\geq 0$ vérifiant la relation $k_j + \sum_{i=1}^r \alpha_i h_i = n$; pour chaque $n$ il n’y a qu’un nombre fini de familles $(\alpha_i)_{1 \leq i \leq r}$ vérifiant ces conditions, puisque $h_i \geq 1$ pour tout $i$; on en conclut que $M_n$ est un $A_0$-module de type fini, et en outre il est clair que $M_n = \{ 0 \}$ lorsque $n < \inf_j (k_j)$.

### 3. Propriétés de l’anneau $A^{(d)}$.

Soient $A = \bigoplus_{i \in \mathbf{Z}} A_i$ un anneau gradué, $M = \bigoplus_{i \in \mathbf{Z}} M_i$ un $A$-module gradué; pour tout couple d’entiers $(d, k)$ tel que $d \geq 1$, $0 \leq k \leq d-1$, posons

$$
A^{(d)} = \bigoplus_{i \in \mathbf{Z}} A_{id}, \quad M^{(d, k)} = \bigoplus_{i \in \mathbf{Z}} M_{id+k}.
$$

Il est clair que $A^{(d)}$ est un sous-anneau gradué de $A$ et $M^{(d, k)}$ un $A^{(d)}$-module gradué; en outre, si $N$ est un sous-module gradué de $M$, $N^{(d, k)}$ est un sous-$A^{(d)}$-module gradué de $M^{(d, k)}$. On écrira

$M^{(d)}$ au lieu de $M^{(d,0)}$; pour chaque $d \geqslant 1$, $M$ est somme directe des $A^{(d)}$-modules $M^{(d,k)}$ ($0 \leqslant k \leqslant d-1$).

#### Proposition 2 {#ac-iii-s1-prop-2 .statement}

Soient $A = \bigoplus_{i \in \mathbf{Z}} A_i$ un anneau commutatif gradué à degrés positifs, $M = \bigoplus_{i \in \mathbf{Z}} M_i$ un $A$-module gradué. On suppose que $A$ est une $A_0$-algèbre de type fini et $M$ un $A$-module de type fini. Alors, pour tout couple $(d, k)$ d'entiers tels que $d \geqslant 1$, $0 \leqslant k \leqslant d-1$ :
(i) $A^{(d)}$ est une $A_0$-algèbre de type fini.
(ii) $M^{(d,k)}$ est un $A^{(d)}$-module de type fini.

Montrons que $A$ est un $A^{(d)}$-module de type fini. Soit $(a_i)_{1 \leqslant i \leqslant s}$ un système de générateurs de la $A_0$-algèbre $A$ formé d'éléments homogènes. Les éléments de $A$ (en nombre fini) de la forme $a_1^{\alpha_1} a_2^{\alpha_2} \ldots a_s^{\alpha_s}$ tels que $0 \leqslant \alpha_i < d$ pour $1 \leqslant i \leqslant s$ constituent un système de générateurs du $A^{(d)}$-module $A$; en effet, pour tout système d'entiers $n_i \geqslant 0$ ($1 \leqslant i \leqslant s$), il y a des entiers positifs $q_i, r_i$ tels que $n_i = q_i d + r_i$ avec $r_i < d$ ($1 \leqslant i \leqslant s$); on a alors
$$
a_1^{n_1} a_2^{n_2} \ldots a_s^{n_s} = (a_1^{q_1} \ldots a_s^{q_s})^d (a_1^{r_1} \ldots a_s^{r_s})
$$
ce qui prouve notre assertion, car tout élément homogène $x \in A$ est tel que $x^d \in A^{(d)}$. Alors, si $M$ est un $A$-module de type fini, c'est aussi un $A^{(d)}$-module de type fini; comme $M$ est somme directe des $M^{(d,k)}$ ($0 \leqslant k \leqslant d-1$), chacun des $M^{(d,k)}$ est un $A^{(d)}$-module de type fini, ce qui prouve (ii).

Appliquons ce qui précède au $A$-module gradué $m = \bigoplus_{i \geqslant 1} A_i$, qui est de type fini en vertu du cor. de la prop. 1 du n° 2; on voit que $m^{(d)}$ est un $A^{(d)}$-module de type fini; par suite (n° 2, cor. de la prop. 1) $A^{(d)}$ est une $A_0$-algèbre de type fini.

#### Lemme 1 {#ac-iii-s1-lem-1 .statement}

Soient $A$ un anneau commutatif gradué tel que $A = A_0[A_1]$, $M$ un $A$-module gradué, $(y_\lambda)_{\lambda \in L}$ un système de générateurs homogènes de $M$ tels que $\deg(y_\lambda) \leqslant n_0$ pour tout $\lambda \in L$. Alors, pour tout $n \geqslant n_0$ et tout $k \geqslant 0$, on a $M_{n+k} = A_k \cdot M_n$.

Soit $n \geqslant n_0$ et soit $x \in M_{n+1}$. Puisque les $y_\lambda$ engendrent $M$, il existe une famille $(a_\lambda)_{\lambda \in L}$ d'éléments de $A$, de support fini, telle que $x = \sum_{\lambda} a_\lambda y_\lambda$; on peut en outre supposer chaque $a_\lambda$ homogène et de degré $n + 1 - \deg(y_\lambda)$ (en le remplaçant au besoin par sa composante homogène de ce degré). Comme $\mathbf{A} = \mathbf{A}_0[\mathbf{A}_1]$ et $\deg(a_\lambda) > 0$, chaque $a_\lambda$ est somme d’éléments de la forme $bb'$ avec $b \in \mathbf{A}_1, b' \in \mathbf{A}$, d’où $x \in \mathbf{A}_1\mathbf{M}_n$. On a donc $\mathbf{M}_{n+1} = \mathbf{A}_1\mathbf{M}_n$, d’où $\mathbf{M}_{n+k} = \mathbf{A}_k\mathbf{M}_n$ par récurrence sur $k$.

#### Lemme 2 {#ac-iii-s1-lem-2 .statement}

*Soit $\mathbf{A}$ un anneau commutatif gradué tel que $\mathbf{A} = \mathbf{A}_0[\mathbf{A}_1]$, et soit $S = \bigoplus_{i \geq 0} S_i$ une $\mathbf{A}$-algèbre commutative graduée à degrés positifs, qui soit un $\mathbf{A}$-module de type fini. Il existe alors un entier $n_0 \geq 0$ tel que :*

(i) *Pour $n \geq n_0$ et $k \geq 0$, $S_{n+k} = S_k.S_n$.*
(ii) *Pour $d \geq n_0$, $S^{(d)} = S_0[S_d]$.*

En vertu du lemme 1, il existe un entier $n_0 \geq 0$ tel que pour $n \geq n_0$ et $k \geq 0$ on ait $S_{n+k} = \mathbf{A}_k S_n$, d’où *a fortiori* $S_{n+k} = S_k S_n$, ce qui établit (i). Pour $d \geq n_0$ et $m > 0$, on a alors $S_{md} = (S_d)^m$ comme on le voit par récurrence sur $m$ en appliquant (i); ceci établit (ii).

#### Proposition 3 {#ac-iii-s1-prop-3 .statement}

*Soit $\mathbf{R} = \bigoplus_{i \geq 0} \mathbf{R}_i$ un anneau commutatif gradué à degrés positifs qui soit une $\mathbf{R}_0$-algèbre de type fini. Il existe un entier $e \geq 1$ tel que $\mathbf{R}^{(me)} = \mathbf{R}_0[\mathbf{R}_{me}]$ pour tout $m \geq 1$.*

Soit $(x_j)_{1 \leq j \leq s}$ un système de générateurs homogènes de la $\mathbf{R}_0$-algèbre $\mathbf{R}$, dont les degrés soient $\geq 1$. Soit $h_j = \deg(x_j)$, soit $q$ un multiple commun des $h_j$ et posons $q_j = q/h_j$ pour $1 \leq j \leq s$; les éléments $x_j^{q_j}$ sont donc tous de degré $q$. Soit $\mathbf{B}$ la sous-$\mathbf{R}_0$-algèbre de $\mathbf{R}$ engendrée par les $x_j^{q_j}$; c’est une sous-algèbre graduée de $\mathbf{R}$, et l’on a $B_i = 0$ si $i$ n’est pas multiple de $q$. Soit $\mathbf{A}$ (resp. $S$) l’anneau gradué dont l’anneau sous-jacent est $\mathbf{B}$ (resp. $\mathbf{R}^{(q)}$) et la graduation formée des $A_i = B_{iq}$ (resp. $S_i = R_{iq}$). On a $\mathbf{A} = \mathbf{A}_0[\mathbf{A}_1]$ par définition de $\mathbf{B}$. Considérons les éléments de $\mathbf{R}$ (en nombre fini) de la forme $x_1^{\alpha_1} x_2^{\alpha_2} \ldots x_s^{\alpha_s}$, où $0 \leq \alpha_j < q_j$ et $\alpha_1 h_1 + \cdots + \alpha_s h_s \equiv 0$ (mod. $q$); montrons qu’ils engendrent le $\mathbf{B}$-module $\mathbf{R}^{(q)}$. Il suffit de prouver que tout élément de $\mathbf{R}^{(q)}$ de la forme $x_1^{n_1} x_2^{n_2} \ldots x_s^{n_s}$ est combinaison $\mathbf{B}$-linéaire des éléments précédents. Or, il existe des entiers positifs $k_j, r_j$ tels que $n_j = k_j q_j + r_j$ avec $r_j < q_j (1 \leq j \leq s)$; on a alors

$$
x_1^{n_1} x_2^{n_2} \ldots x_s^{n_s} = (x_1^{q_1})^{k_1} \ldots (x_s^{q_s})^{k_s} \cdot (x_1^{r_1} \ldots x_s^{r_s})
$$

et par hypothèse $\sum_{j=1} n_j h_j \equiv 0$ (mod. $q$), donc $\sum_{j=1} r_j h_j \equiv 0$ (mod. $q$) ; comme les $x_j^{q_i}$ appartiennent à B par définition, cela prouve notre assertion. Comme S est un A-module de type fini, on peut appliquer le lemme 2 : il existe $n_0$ tel que pour $d \geq n_0$, $S^{(d)} = S_0[S_d]$, donc $R^{(qd)} = R_0[R_{qd}]$ pour $d \geq n_0$. La proposition en résulte, avec $e = q n_0$.

### 4. Idéaux premiers gradués.

Soient $A = \bigoplus_{i \geq 0} A_i$ un anneau commutatif gradué à degrés positifs, m l’idéal gradué $\bigoplus_{i \geq 1} A_i$; nous dirons que deux idéaux gradués $a = \bigoplus_{i \geq 0} a_i, b = \bigoplus_{i \geq 0} b_i$ de A sont équivalents s’il existe un entier $n_0$ tel que $a_n = b_n$ pour $n \geq n_0$ (il est clair que c’est bien une relation d’équivalence). On dit qu’un idéal gradué est essentiel s’il n’est pas équivalent à m.

#### Proposition 4 {#ac-iii-s1-prop-4 .statement}

Soit $p = \bigoplus_{i \geq 0} p_i$ un idéal gradué de A ; pour que p soit premier, il faut et il suffit que si $x \in A_m, y \in A_n$ sont tels que $x \notin p$ et $y \notin p$, on ait $xy \notin p$.

La condition est évidemment nécessaire. Inversement, si elle est remplie, alors, dans l’anneau gradué $A/p = \bigoplus_{i \geq 0} A_i/p_i$, le produit de deux éléments homogènes $\neq 0$ est $\neq 0$, donc $A/p$ est intègre (Alg., chap. II, 3e éd., § 11, n° 4, prop. 7).

#### Proposition 5 {#ac-iii-s1-prop-5 .statement}

Soient $a = \bigoplus_{i \geq 0} a_i$ un idéal gradué de A, $n_0$ un entier $> 0$. Pour qu’il existe un idéal premier gradué $p = \bigoplus_{i \geq 0} p_i$ tel que $p_n = a_n$ pour $n \geq n_0$, il faut et il suffit que, pour tout couple d’éléments homogènes $x, y$ de degrés $\geq n_0$, la relation $xy \in a$ entraîne « $x \in a$ ou $y \in a$ ». S’il existe $n \geq n_0$ tel que $a_n \neq A_n$, l’idéal premier gradué vérifiant les conditions précédentes est unique.

La condition de l’énoncé est évidemment nécessaire. Si l’on a $a_n = A_n$ pour tout $n \geq n_0$, il est clair que tout idéal premier contenant m est gradué et répond à la question ; il peut donc y avoir plusieurs idéaux premiers gradués répondant à la question ; toutefois, deux quelconques de ces idéaux sont évidemment équivalents. Supposons donc qu’il existe un élément homogène $a \in A_d$ (avec $d \geq n_0$) n’appartenant pas à $a_d$. Soit $p$ l’ensemble des $x \in A$ tels que $ax \in a$. Il est clair que $p$ est un idéal de $A$; comme les composantes homogènes de $ax$ sont les produits par $a$ de celles de $x$, et que $a$ est un idéal gradué, $p$ est un idéal gradué ; en outre, on a $1 \notin p$, donc $p \neq A$. Pour prouver que $p$ est premier, il suffit de montrer que si $x \in A_m, y \in A_n$ sont tels que $x \notin p$ et $y \notin p$, alors on a $xy \in p$ (prop. 4). On a alors $ax \in a_{m+d}, ay \in a_{n+d}$, d’où par hypothèse $a^2xy \in a_{m+n+2d}$; on en conclut que $axy \in a_{m+n+d}$, puisque $xy \in p$. Enfin, si $n \geq n_0$ et $x \in A_n$, les conditions $x \in a_n$ et $ax \in a_{n+d}$ sont équivalentes par hypothèse, donc $p \cap A_n = a_n$, ce qui achève de prouver l’existence de l’idéal premier gradué $p$ répondant à la question. Si en outre $p'$ est un second idéal premier gradué de $A$ tel que $p' \cap A_n = a_n$ pour $n \geq n_0$, on a $a \notin p'$ et $ax \in p'$ pour tout $x \in p$, d’où $p \subset p'$ puisque $p'$ est premier. D’autre part, si $x$ est un élément homogène de degré $n \geq 0$ de $p'$, $ax$ est homogène de degré $n + d \geq n_0$ et appartient par suite à $p' \cap A_{n+d} = a_{n+d}$, d’où par définition $x \in p$, ce qui montre que $p' \subset p$, et finalement $p' = p$.

#### Proposition 6 {#ac-iii-s1-prop-6 .statement}

Soit $d$ un entier $\geq 1$.
(i) Pour tout idéal premier gradué essentiel $p$ de $A$, $p \cap A^{(d)}$ est un idéal premier gradué essentiel de $A^{(d)}$.
(ii) Inversement, pour tout idéal premier gradué essentiel $p'$ de $A^{(d)}$, il existe un idéal premier gradué (nécessairement essentiel) $p$ de $A$, et un seul, tel que $p \cap A^{(d)} = p'$.
(i) Si $a \in A_k$ n’appartient pas à $p_k$, $a^{kd}$ n’appartient pas à $p_{kd}$, donc $p \cap A^{(d)}$ est essentiel.
(ii) Pour tout $n \geq 0$, l’ensemble $p \cap A_n$ doit être égal à l’ensemble $a_n$ des $x \in A_n$ tels que $x^d \in p'$. Montrons que $a = \bigoplus_{n \geq 0} a_n$ est un idéal premier gradué ; comme $a_n = p'_n$ lorsque $n$ est multiple de $d$, puisque $p'$ est premier, cela prouvera l’existence et l’unicité de $p$. Or, si $x \in a_n, y \in a_n, (x - y)^{2d}$ est somme de termes dont chacun est produit de $x^d$ ou de $y^d$ par un élément homogène de degré $nd$, donc $(x - y)^{2d} \in p'$, et puisque $p'$ est premier, $(x - y)^d \in p'$, donc $a_n$ est un sous-groupe de $A$. Comme $p'$ est un idéal de $A^{(d)}$, $a$ est un idéal gradué de $A$; enfin, la relation $(xy)^d \in p'$ entraîne $x^d \in p'$ ou $y^d \in p'$, ce qui achève la démonstration en vertu de la prop. 4.

Soient $A$ un anneau commutatif gradué à degrés positifs, $p$ un idéal premier gradué essentiel de $A$. L’ensemble $S$ des éléments homogènes de $A$ n’appartenant pas à $p$ est multiplicatif, et l’anneau de fractions $S^{-1}A$ est donc gradué de façon canonique (chap. II, § 2, n° 9) (on notera qu’il y aura en général des éléments homogènes $\neq 0$ de degré négatif pour cette graduation). Nous désignerons par $A_{(p)}$ le sous-anneau de $S^{-1}A$ formé des éléments homogènes de degré 0, autrement dit l’ensemble des fractions $x/s$, où $x$ et $s$ sont homogènes de même degré dans $A$ et $s \notin p$. De même, pour tout $A$-module gradué $M$, $S^{-1}M$ est gradué de façon canonique (*loc. cit.*) et nous désignerons par $M_{(p)}$ le sous-groupe des éléments homogènes de degré 0, qui est évidemment un $A_{(p)}$-module.

#### Proposition 7 {#ac-iii-s1-prop-7 .statement}

*Soient $p$ un idéal premier gradué de $A$, $d$ un entier $\geqslant 1$, $p'$ l’idéal premier gradué $p \cap A^{(d)}$ de $A^{(d)}$; pour tout $A$-module gradué $M$, l’homomorphisme $(M^{(d)})_{(p')} \to M_{(p)}$ déduit de l’injection canonique $M^{(d)} \to M$ est bijectif.*

Si $S$ est l’ensemble des éléments homogènes de $A$ n’appartenant pas à $p$, et $S' = S \cap A^{(d)}$, l’homomorphisme canonique $\varphi : {S'}^{-1}M^{(d)} \to S^{-1}M$ est un homomorphisme homogène de degré 0, et il est injectif, car si $x \in M_{nd}$ est tel que $sx = 0$ pour $s \in A_m, s \notin p$, on a aussi $s^d x = 0$, et $s^d \in A_{md}, s^d \notin p'$. Reste à voir que l’image par $\varphi$ de $(M^{(d)})_{(p')}$ est $M_{(p)}$ tout entier ; mais si $x \in M_n, s \in A_n$ et $s \notin p$, on a aussi $x/s = (xs^{d-1})/s^d$ avec $xs^{d-1} \in A_{nd}, s^d \in A_{nd}$ et $s^d \notin p'$, d’où notre assertion.

#### Proposition 8 {#ac-iii-s1-prop-8 .statement}

*Soit $m = \bigoplus_{t \geqslant 1} A_t$; soient $(p^{(k)})_{1 \leqslant k \leqslant n}$ une famille finie d’idéaux premiers gradués de $A$ et $a$ un idéal gradué de $A$ tel que $a \cap m \notin p^{(k)}$ pour tout $k$; alors il existe un élément homogène $z \in a \cap m$ n’appartenant à aucun des $p^{(k)}$.*

Raisonnons par récurrence sur $n$, la proposition étant triviale pour $n = 1$. S’il existe un indice $j$ tel que $a \cap m \cap p^{(j)}$ soit contenu dans un des $p^{(k)}$ d’indice $k \neq j$, il résulte de l’hypothèse de récurrence qu’il y a un élément homogène $z' \in a \cap m$ n’appartenant à aucun des $p^{(k)}$ pour $k \neq j$, donc n’appartenant pas non plus à $p^{(j)}$, et cet élément répond à la question. Supposons donc que pour tout indice $j$, $a \cap m \cap p^{(j)}$ ne soit contenu dans aucun des $p^{(k)}$ d’indice $k \neq j$; l’hypothèse de récurrence entraîne donc l’existence d’un élément homogène $y_j \in a \cap m \cap p^{(j)}$ n’appartenant à aucun des $p^{(k)}$ d’indice $k \neq j$; comme les $y_j$ sont tous de degrés $\geq 1$, on peut en les remplaçant par des puissances convenables (puisque les $p^{(k)}$ sont premiers) supposer que $y_1$ et $\prod_{j=2}^n y_j$ sont de même degré. Alors $z = y_1 + \prod_{j=2}^n y_j$ est homogène de degré $\geq 1$ et le même raisonnement que dans le chap. II, § 1, no 1, prop. 2 montre que $z$ répond à la question.

## EXERCICES {#ac-iii-s1-exercises}

See the [exercises for § 1](exercises/s1/).
