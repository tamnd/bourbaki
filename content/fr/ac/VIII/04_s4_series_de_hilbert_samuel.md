---
book: ac
book_title: Commutative Algebra
chapter: VIII
chapter_title: DIMENSION
section: 4
section_title: Séries de Hilbert-Samuel
lang: fr
source: ac-viii-ix-fr
book_pages: AC VIII.87-AC VIII.94
pdf_pages: 0041-0055, 0091-0098
extraction: ocr
subsections:
    - "no": 1
      title: L’anneau $\mathbf{Z}((T))$
      page: 0
      pdf_page: 41
    - "no": 2
      title: Série de Poincaré d’un module gradué sur un anneau de polynômes
      page: 39
      pdf_page: 43
    - "no": 3
      title: Série de Hilbert-Samuel d’un module bien filtré
      page: 43
      pdf_page: 47
    - "no": 4
      title: Degré de la fonction de Hilbert-Samuel
      page: 47
      pdf_page: 51
    - "no": 5
      title: Série de Hilbert-Samuel d’un module quotient
      page: 48
      pdf_page: 52
statements: 34
exercises: 12
content_sha256: 8a3e20284919ae10cbe7a7b0edf8a7928dc3eb483565302464487f21ad0e6563
---

## § 4. SÉRIES DE HILBERT-SAMUEL

### 1. L’anneau $\mathbf{Z}((T))$

Soit A un anneau. Munissons le A-module $A^\mathbf{Z}$ de la topologie produit des topologies discrètes. Les éléments $(a_n) \in A^\mathbf{Z}$ tels qu’il existe $n_0 \in \mathbf{Z}$ avec $a_n = 0$ pour $n < n_0$ forment un sous-module B de $A^\mathbf{Z}$. Si pour $a = (a_n) \in B, b \in (b_n) \in B$, on pose $ab = c$, avec $c_n = \sum_{i+j=n} a_i b_j$, on définit sur B une structure de A-algèbre. Soit T l’élément $(\theta_n)$ de B tel que $\theta_n = 0$ pour $n \neq 1$ et $\theta_1 = 1$. Alors T est inversible dans B ; pour tout élément $a = (a_n)$ de B, la famille $(a_n T^n)_{n \in \mathbf{Z}}$ est sommable dans $A^\mathbf{Z}$ et l’on a

$$
a = \sum_{n \in \mathbf{Z}} a_n T^n .
$$

Dans la suite de ce chapitre, on notera $A((T))$ la $A$-algèbre $B$; elle contient comme sous-algèbres l’algèbre $A[[T]]$ des séries formelles et l’algèbre $A[T, T^{-1}]$; leur intersection est l’algèbre $A[T]$ des polynômes.

#### Remarque {#ac-viii-s4-n1-rem-1 .statement}

L’anneau $A((T))$ s’identifie naturellement à l’anneau de fractions $A[[T]]_T$ de l’anneau $A[[T]]$ défini par la partie multiplicative formée des puissances de $T$.

Pour $n, p$ dans $\mathbf{Z}$, on définit l’entier naturel $\left[ \begin{array}{c} n \\ p \end{array} \right]$ par

$$
\left( \begin{array}{ll}
\left[ \begin{array}{c} n \\ p \end{array} \right] = 0 & \text{si } p < 0 \text{ ou } p > n, \\
\left[ \begin{array}{c} n \\ p \end{array} \right] = \binom{n}{p} = \frac{n(n-1)...(n-p+1)}{p!} & \text{si } 0 \leq p \leq n .
\end{array} \right.
$$

On a $\left[ \begin{array}{c} n \\ p \end{array} \right] = \left[ \begin{array}{c} n \\ n-p \end{array} \right]$ pour $n, p \in \mathbf{Z}$.

#### Lemme 1 {#ac-viii-s4-lem-1 .statement}

*L’élément $1 - T$ de $\mathbf{Z}((T))$ est inversible. Pour tout entier $r > 0$ on a*

$$
(1 - T)^{-r} = \sum_{n \in \mathbf{Z}} \left[ \begin{array}{c} n + r - 1 \\ r - 1 \end{array} \right] T^n = \sum_{n \in \mathbf{N}} \binom{n + r - 1}{r - 1} T^n .
$$

En effet, $1 - T$ est inversible dans l’anneau $\mathbf{Z}[[T]]$, d’inverse $\sum_{m \geq 0} T^m$; on a donc

$$
(1 - T)^{-r} = (\sum_{m \geq 0} T^m)^r = \sum_{m_1, ..., m_r \geq 0} T^{m_1 + m_2 + ... + m_r},
$$

et la formule annoncée résulte de E, III, p. 44, prop. 15.

Soient $Q(T) \in \mathbf{Z}[T, T^{-1}]$, $r$ un entier $> 0$, et $F = (1 - T)^{-r} Q \in \mathbf{Z}((T))$. Posons

$$
Q(T) = \sum_{i \in \mathbf{Z}} a_i T^i , \quad F = \sum_{n \in \mathbf{Z}} \alpha_n T^n .
$$

Alors, d’après le lemme 1, on a

$$
\alpha_n = \sum_{i \in \mathbf{Z}} a_i \left[ \begin{array}{c} n - i + r - 1 \\ r - 1 \end{array} \right] = \sum_{i \leq n} a_i \binom{n - i + r - 1}{r - 1}.
$$

Soit $n_1$ la borne supérieure dans $\overline{\mathbf{R}}$ de l’ensemble des entiers $i \in \mathbf{Z}$ tels que $a_i \neq 0$. Pour tout entier $n \geq n_1$, on a $\alpha_n = \tilde{\alpha}(n)$, où $\tilde{\alpha}$ est le polynôme de $\mathbf{Q}[X]$ défini par

$$
\tilde{\alpha}(X) = \frac{1}{(r-1)!} \sum_{i \in \mathbf{Z}} a_i \prod_{j=1}^{r-1} (X - i + j) .
$$

Si l’on pose $c = Q(1) = \sum_{i \in \mathbf{Z}} a_i$, on a $\tilde{\alpha}(X) = c X^{r-1}/(r-1)! + \theta(X)$, où $\theta$ est un polynôme de degré $\leq r-2$. Par conséquent, on a

$$
\alpha_n = c \frac{n^{r-1}}{(r-1)!} + \rho_n n^{r-2},
$$

où le nombre rationnel $\rho_n$ tend vers une limite lorsque $n$ augmente indéfiniment. On en déduit la relation

$$
Q(1) = (r-1)! \lim_{n \to \infty} n^{1-r} \alpha_n.
$$

Si $F = \sum_{n \in \mathbf{Z}} a_n T^n$ et $G = \sum_{n \in \mathbf{Z}} b_n T^n$ sont deux éléments de $\mathbf{Z}((T))$, on note « $F \leq G$ » la relation « $a_n \leq b_n$ pour tout $n \in \mathbf{Z}$ ». C’est une relation d’ordre compatible avec la structure d’anneau de $\mathbf{Z}((T))$ (A, VI, p. 18, déf. 1). On a $(1-T)^{-1} \geq 1$. Si $Q \in \mathbf{Z}[T, T^{-1}]$ est $\geq 0$, alors l’entier $Q(1)$ est positif.

**Lemme 2. — a)** Soit $F$ un élément non nul de $\mathbf{Z}((T))$ tel qu’il existe $r \in \mathbf{Z}$, avec $(1-T)^r F \in \mathbf{Z}[T, T^{-1}]$; alors $F$ s’écrit de manière unique sous la forme $F = (1-T)^{-d}.Q$, où $Q \in \mathbf{Z}[T, T^{-1}]$, $Q(1) \neq 0$ et $d \in \mathbf{Z}$. Si $F \geq 0$, alors on a $Q(1) > 0$ et $d \geq 0$.

b) Soient $Q, R$ dans $\mathbf{Z}[T, T^{-1}]$, $d, d'$ dans $\mathbf{Z}$ avec $Q(1) > 0$. Si

$$
(1-T)^{-d}.Q \leq (1-T)^{-d'}.R,
$$

alors, ou bien $d < d'$, ou bien $d = d'$ et $Q(1) \leq R(1)$.

a) On peut écrire $F = (1-T)^{-r} T^n P(T)$ avec $r, n \in \mathbf{Z}$ et $P(T) \in \mathbf{Z}[T]$. Par division euclidienne, on peut écrire $P(T) = (1-T)^p R(T)$ avec $R(T) \in \mathbf{Z}[T]$ et $R(1) \neq 0$. Donc $F = (1-T)^{-(r-p)} Q(T)$, où $Q(T) = T^n R(T) \in \mathbf{Z}[T, T^{-1}]$ et $Q(1) \neq 0$. Cela démontre l’existence de $d$ et $Q$. Par ailleurs, si $(1-T)^r Q(T) = (1-T)^s R(T)$ avec $r > s$ et $Q, R$ dans $\mathbf{Z}[T, T^{-1}]$, on a $R(T) = (1-T)^{r-s} Q(T)$, donc $R(1) = 0$; cela démontre l’unicité. Supposons que $F$ soit $\geq 0$; si on avait $d < 0$, alors on aurait $F(1) = 0$, ce qui est impossible puisque $F$ est non nul et que tous ses coefficients sont positifs ; on a donc $d \geq 0$. Si $d = 0$, alors $Q = F \geq 0$, donc $Q(1)$ est positif. Si $d \geq 1$, alors $Q(1)$ est positif d’après la formule (3). Cela démontre a).

b) Supposons $d \geq d'$. Alors $(1-T)^{-d} ((1-T)^{d-d'} R - Q) \geq 0$; comme $S(T) = (1-T)^{d-d'} R - Q$ appartient à $\mathbf{Z}[T, T^{-1}]$, cela implique $S(1) \geq 0$ d’après ce qui précède. Si $d > d'$, on a $S(1) = -Q(1) < 0$, d’où une contradiction ; si $d = d'$, on a $S(1) = R(1) - Q(1)$ d’où $Q(1) \leq R(1)$.

### 2. Série de Poincaré d’un module gradué sur un anneau de polynômes

Soient $H_0$ un anneau, $I$ un ensemble fini et $H$ l’anneau de polynômes $H_0[(X_i)_{i \in I}]$. Pour chaque $i \in I$, soit $d_i$ un entier $> 0$. Munissons $H$ de la structure d’anneau gradué de type $\mathbf{Z}$ telle que les éléments de $H_0$ soient homogènes de degré 0 et chaque $X_i$ homogène de degré $d_i$. Lorsque $d_i = 1$ pour tout $i$, on retrouve la graduation usuelle des anneaux de polynômes.

Soit $M$ un $H$-module gradué de *type fini* dont tous les composants homogènes sont des $H_0$-modules de longueur finie ; on appelle *série de Poincaré* de $M$ l’élément $P_M$ de $\mathbf{Z}((T))$ tel que $P_M = \sum_{n \in \mathbf{Z}} \operatorname{long}_{H_0}(M_n) \cdot T^n$, et l’on pose $Q_M = P_M \cdot \prod_{i \in I} (1 - T^{d_i})$.

#### Théorème 1 {#ac-viii-s4-thm-1 .statement}

*L’élément $Q_M$ de $\mathbf{Z}((T))$ appartient à $\mathbf{Z}[T, T^{-1}]$*.

Divisant $H_0$ par l’annulateur du $H_0$-module $M$, on se ramène au cas où $M$ est un $H_0$-module fidèle. Si $a, b \in \mathbf{Z}$ sont tels que $M$ soit engendré comme $H$-module par $M' = \sum_{a \leq i \leq b} M_i$, alors $M'$ est un $H_0$-module fidèle et de longueur finie ; par suite, l’anneau $H_0$ est artinien (A, VIII, § 1, no 3), donc noethérien (*loc. cit.*, § 9, no 1). L’anneau de polynômes $H$ est donc noethérien (*loc. cit.*, § 1, no 4). Si $I$ est vide, on a $H = H_0$, et la famille d’entiers $(\operatorname{long}_{H_0}(M_n))_{n \in \mathbf{Z}}$ est à support fini, puisque $M$ est un $H_0$-module de type fini ; d’où le théorème dans ce cas. Raisonnons alors par récurrence sur le cardinal de l’ensemble $I$, supposé non vide ; soient $j \in I$ et $J = I - \{j\}$. Notons $H'$ le sous-anneau gradué de $H$ engendré par $H_0$ et les $X_i$ pour $i$ dans $J$ ; considérons l’homothétie $(X_j)_M$ de rapport $X_j$ dans $M$, son noyau $R$, et son conoyau $S$. On a, pour chaque $n \in \mathbf{Z}$, une suite exacte de $H_0$-modules

$$
0 \to R_{n-d_j} \to M_{n-d_j} \to M_n \to S_n \to 0 ,
$$

donc $R_{n-d_j}$ et $S_n$ sont de longueur finie, et l’on a

$$
\operatorname{long}_{H_0}(M_n) - \operatorname{long}_{H_0}(M_{n-d_j}) = \operatorname{long}_{H_0}(S_n) - \operatorname{long}_{H_0}(R_{n-d_j}) .
$$

Puisque $M$ est un module de type fini sur l’anneau noethérien $H$, les $H$-modules $R$ et $S$ sont de type fini ; comme ils sont annulés par $X_j$, ce sont des $H'$-modules de type fini. D’après l’hypothèse de récurrence, les éléments $P_R \cdot \prod_{i \in J} (1 - T^{d_i})$ et $P_S \cdot \prod_{i \in J} (1 - T^{d_i})$ de $\mathbf{Z}((T))$ appartiennent donc à $\mathbf{Z}[T, T^{-1}]$; de (4), on tire

$$
P_M - T^{d_j} \cdot P_M = P_S - T^{d_j} \cdot P_R ,
$$

c’est-à-dire $(1 - T^{d_j}) \cdot P_M = P_S - T^{d_j} \cdot P_R$; on a donc

$$
P_M \cdot \prod_{i \in I} (1 - T^{d_i}) = P_S \cdot \prod_{i \in J} (1 - T^{d_i}) - T^{d_j} \cdot P_R \cdot \prod_{i \in J} (1 - T^{d_i}) ,
$$

d’où la conclusion.

#### Exemple 1 {#ac-viii-s4-n2-exa-1 .statement}

Supposons $H_0$ artinien et prenons $M = H$. Alors, avec les notations précédentes, on a $R = 0$ et $S = H'$, donc d’après (5), on a $Q_H = Q_{H'}$; comme on a $Q_{H_0} = \operatorname{long}(H_0)$, on en tire par récurrence $Q_H = \operatorname{long}(H_0)$, c’est-à-dire

$$
P_H = \operatorname{long}(H_0) \cdot \prod_{i \in I} (1 - T^{d_i})^{-1} .
$$

Supposons désormais H muni de la graduation usuelle, pour laquelle $d_i = 1$ pour tout $i \in I$, et posons $r = \mathrm{Card}(I)$; on a $P_M = Q_M(T).(1 - T)^{-r}$. Posons $c_M = Q_M(1)$. Alors, d’après la formule (2) du n° 1, on a :

#### Corollaire {#ac-viii-s4-n2-cor-1 .statement}

a) Si $r = 0$, alors on a $\mathrm{long}_{H_0}(M) = c_M$.

b) Si $r = 1$, alors on a $\mathrm{long}_{H_0}(M_n) = c_M$ pour $n$ assez grand.

c) Si $r > 1$, alors on a $\mathrm{long}_{H_0}(M_n) = c_M \frac{n^{r-1}}{(r-1)!} + \rho_n n^{r-2}$, où $\rho_n$ tend vers une limite dans $\mathbf{R}$ lorsque $n$ augmente indéfiniment.

#### Remarque 1 {#ac-viii-s4-n2-rem-1 .statement}

L’entier $c_M$ est positif d’après le lemme 2. On peut avoir $M \neq 0$ et $c_M = 0$ (cf. prop. 2).

#### Remarque 2 {#ac-viii-s4-n2-rem-2 .statement}

Soit $0 \to M' \to M \to M'' \to 0$ une suite exacte de H-modules gradués et d’homomorphismes de degré 0 telle que M soit de type fini sur H et $M_n$ de longueur finie sur $H_0$ pour chaque $n$. Alors, pour chaque $n \in \mathbf{Z}$, on a
$$
\mathrm{long}_{H_0}(M_n) = \mathrm{long}_{H_0}(M'_n) + \mathrm{long}_{H_0}(M''_n),
$$
donc $P_M = P_{M'} + P_{M''}$, $Q_M = Q_{M'} + Q_{M''}$ et $c_M = c_{M'} + c_{M''}$.

#### Remarque 3 {#ac-viii-s4-n2-rem-3 .statement}

Soit $M(p)$ le module déduit de M par décalage de $p$ de la graduation (A, II, p. 165, exemple 3). Comme on a $M(p)_n = M_{p+n}$, on a $P_{M(p)} = T^{-p}P_M$, $Q_{M(p)} = T^{-p}Q_M$ et $c_{M(p)} = c_M$.

#### Exemple 2 {#ac-viii-s4-n2-exa-2 .statement}

Supposons $H_0$ artinien, et soit M un H-module gradué libre engendré par s éléments homogènes, linéairement indépendants, de degrés respectifs $\delta_1, ..., \delta_s$. Alors M est isomorphe à $H(-\delta_1) \oplus \cdots \oplus H(-\delta_s)$. D’après les remarques 2 et 3 et l’exemple 1, on a donc
$$
P_M = \mathrm{long}(H_0)\left( \sum_{i=1}^s T^{\delta_i} \right)(1 - T)^{-r},
$$
$$
Q_M = \mathrm{long}(H_0)\left( \sum_{i=1}^s T^{\delta_i} \right),
$$
$$
c_M = s.\mathrm{long}(H_0).
$$

#### Exemple 3 {#ac-viii-s4-n2-exa-3 .statement}

Supposons toujours $H_0$ artinien ; soit M un H-module gradué, et supposons qu’il existe une suite exacte de H-modules gradués et d’homomorphismes de degré 0
$$
0 \to L_n \to L_{n-1} \to \cdots \to L_0 \to M \to 0,
$$
où, pour $k = 0, 1, ..., n$, $L_k$ est un H-module gradué libre engendré par des éléments homogènes linéairement indépendants, de degrés respectifs $\delta_{k,1}, ..., \delta_{k,m(k)}$. Alors, d’après la remarque 2 et l’exemple 2, on a
$$
Q_M = \mathrm{long}(H_0).\sum_{0 \leq k \leq n} \sum_{1 \leq j \leq m(k)} (-1)^k T^{\delta_{k,j}},
$$
$$
c_M = \mathrm{long}(H_0).\sum_{0 \leq k \leq n} (-1)^k m(k).
$$

#### Remarque 4 {#ac-viii-s4-n2-rem-4 .statement}

On peut prouver (p. 88, exerc. 4) que sous les hypothèses du th. 1, les $H_0$-modules $\mathrm{Tor}_j^H(H_0, M)$ sont de longueur finie, nuls pour $j > r$, et qu’on a
$$
c_M = \sum_{j=0}^r (-1)^j \mathrm{long}_{H_0}(\mathrm{Tor}_j^H(H_0, M)).
$$
Plus précisément, les $H$-modules $T_j = \mathrm{Tor}_j^H(H_0, M)$ sont munis naturellement de graduations et on a
$$
Q_M = \sum_{j=0}^r (-1)^j P_{T_j}.
$$

#### Proposition 1 {#ac-viii-s4-prop-1 .statement}

Soit $M$ un $H$-module gradué. On suppose que $M$ est engendré par $M_0$ et que $M_0$ est un $H_0$-module de longueur finie. Alors on a
$$
P_M \leq (1 - T)^{-r} \mathrm{long}_{H_0}(M_0), \quad c_M \leq \mathrm{long}_{H_0}(M_0).
$$
De plus, les conditions suivantes sont équivalentes :
(i) $c_M = \mathrm{long}_{H_0}(M_0)$;
(ii) $P_M = \mathrm{long}_{H_0}(M_0) \cdot (1 - T)^{-r}$, c’est-à-dire $M = M_0$ si $r = 0$ et
$$
\mathrm{long}_{H_0}(M_n) = \mathrm{long}_{H_0}(M_0) \binom{n + r - 1}{r - 1}
$$
pour $n \in \mathbf{N}$ si $r > 0$;
(iii) l’homomorphisme canonique de $H$-modules
$$
\varphi : H \otimes_{H_0} M_0 \to M
$$
est bijectif.

Notons $R$ le noyau de $\varphi$. Comme $\varphi$ est surjectif, on a
$$
P_M = P_{H \otimes M_0} - P_R = \mathrm{long}_{H_0}(M_0) (1 - T)^{-r} - P_R \quad \text{et} \quad c_M = \mathrm{long}_{H_0}(M_0) - c_R.
$$
Les conditions (i), (ii) et (iii) équivalent respectivement à $c_R = 0$, $P_R = 0$ et $R = 0$.
On a donc (iii) $\Rightarrow$ (ii) $\Rightarrow$ (i) et il suffit de prouver que $c_R = 0$ implique $R = 0$. Supposons $R \neq 0$ et soit $0 = N^h \subset N^{h-1} \subset ... \subset N^0 = M_0$ une suite de Jordan-Hölder du $H_0$-module $M_0$. Soit $R^m$ l’intersection de $R$ et de l’image de $H \otimes_{H_0} N^m$ dans $H \otimes_{H_0} M_0$; il existe un entier $m$ compris entre 1 et $h$ tel que $R^m \neq R^{m-1}$. Posons $L = R^{m-1}/R^m$; on a $0 \leq c_L \leq c_R$ et il suffit de prouver que $c_L \neq 0$. Or, si $k$ est le corps quotient de $H_0$ par l’idéal maximal annulateur de $N^{m-1}/N^m$, $L$ s’identifie à un sous-module gradué non nul de $k[(X_i)_{i \in I}]$. Donc $L$ contient un sous-module isomorphe à un module décalé de $k[(X_i)_{i \in I}]$; comme $c_{k[(X_i)_{i \in I}]} = 1$, on a donc $c_L \geq 1$ (remarques 2 et 3), ce qu’on voulait démontrer.

#### Remarque 5 {#ac-viii-s4-n2-rem-5 .statement}

D’après A, X, p. 160, th. 1, la condition (iii) signifie que $(X_1, ..., X_r)$ est une suite complètement sécante pour le $H$-module $M$.

#### Proposition 2 {#ac-viii-s4-prop-2 .statement}

Supposons que $H_0$ soit un corps, et soit $M$ un $H$-module gradué de type fini. Soit $K$ le corps des fractions de $H$. Alors $c_M$ est égal au rang du $H$-module $M$, c’est-à-dire à la dimension du $K$-espace vectoriel $M \otimes_H K$.

Cela est clair si $M = H$, puisque $c_H = 1$. Par ailleurs, soit $x \in H$, homogène de degré $d$, et non nul ; on a $(H/xH) \otimes_H K = 0$; de la suite exacte
$$
0 \to H(-d) \to H \to H/xH \to 0,
$$
et des remarques 2 et 3, on tire $c_{H/xH} = 0$. La proposition est donc vérifiée lorsque $M$ est engendré par un élément homogène. Le cas général s’en déduit, puisque tout $H$-module gradué de type fini possède une suite de composition dont les quotients sont de la forme précédente.

#### Remarque 6 {#ac-viii-s4-n2-rem-6 .statement}

Sous les hypothèses de la prop. 2, on a donc $c_M = 0$ si et seulement si $M$ est un $H$-module de torsion, ou encore si et seulement si $\dim_H(M) < r$ (§ 1, no 5, exemple 4).

### 3. Série de Hilbert-Samuel d’un module bien filtré

Dans la suite de ce paragraphe, nous utiliserons la notation suivante : si $G \in \mathbf{Z}((T))$ et si $r \in \mathbf{N}$, on pose $G^{(r)} = (1 - T)^{-r}G$; en particulier, si $G = \sum_{n \in \mathbf{Z}} a_n T^n$, alors
$$
G^{(1)} = \sum_{n \in \mathbf{Z}} \left( \sum_{i \leq n} a_i \right) T^n.
$$
Si $G \geq 0$, on a $G^{(r)} \geq 0$ pour tout $r \in \mathbf{N}$.

Soient $A$ un anneau noethérien, $q$ un idéal de $A$ et $M$ un $A$-module de type fini. Rappelons (III, § 3, no 1, déf. 1) qu’une filtration $q$-bonne sur $M$ est une application $F : n \mapsto F_n$ de $\mathbf{Z}$ dans l’ensemble des sous-modules de $M$ satisfaisant aux trois conditions suivantes :
a) on a $qF_n \subset F_{n+1} \subset F_n$ pour tout $n \in \mathbf{Z}$,
b) il existe $n_0 \in \mathbf{Z}$ tel que $qF_n = F_{n+1}$ pour $n \geq n_0$,
c) il existe $n_1 \in \mathbf{Z}$ tel que $F_{n_1} = M$.
Si $n_0$ et $n_1$ satisfont aux conditions précédentes, on a, pour tout $n \in \mathbf{Z}$,
$$
q^{n-n_1}M \subset F_n \subset q^{n-n_0}M
$$
(rappelons que l’on a posé $q^r = A$ pour $r \leq 0$, par convention).

#### Lemme 3 {#ac-viii-s4-lem-3 .statement}

Si $F$ et $F'$ sont deux filtrations $q$-bonnes sur $M$, il existe un entier $m$ tel que $F'_n \subset F_{n-m}$ pour tout $n \in \mathbf{Z}$.
En effet, il existe $n_2$ tel que $F'_n \subset q^{n-n_2}M$ pour tout $n$, donc $F'_n \subset F_{n-(n_2-n_1)}$ pour tout $n$.

#### Lemme 4 {#ac-viii-s4-lem-4 .statement}

Soit $F$ une filtration $q$-bonne sur $M$. Si $M/qM$ est de longueur finie, $M/F_{n+1}$ et $F_n/F_{n+1}$ sont de longueur finie pour tout $n \in \mathbf{Z}$.
Avec les notations de (7), on a $\operatorname{long}(M/F_{n+1}) \leq \operatorname{long}(M/q^{n-n_1+1}M)$ et il suffit de prouver que $q^nM/q^{n+1}M$ est de longueur finie pour tout $n$. On est donc ramené au cas de la filtration $q$-adique. Soit $(x_1, ..., x_r)$ un système générateur fini du $A$-module $q$, et soit $I$ l’ensemble fini des monômes de degré total $n$ en $r$ variables

X_1, ..., X_r. L’homomorphisme de (M/qM)^l dans q^nM/q^{n+1}M qui applique la famille (u_m)_{m\in I} sur l’élément $\sum m(x_1, ..., x_r)\ u_m$ est surjectif. Comme M/qM est de longueur finie, q^nM/q^{n+1}M l’est aussi.

Supposons désormais M/qM de longueur finie. Soit F une filtration q-bonne sur M. Il existe $n_1 \in \mathbf{Z}$ tel que $F_{n_1} = M$, donc $F_n = M$ pour $n \leq n_1$; on définit donc un élément $H_{M,F}$ de $\mathbf{Z}((T))$ en posant

(8)
$$
H_{M,F} = \sum_{n \in \mathbf{Z}} \operatorname{long}_{A/q}(F_n/F_{n+1}). T^n \in \mathbf{Z}((T)).
$$

#### Définition 1 {#ac-viii-s4-def-1 .statement}

On appelle $H_{M,F}$ la série de Hilbert-Samuel du A-module M (relativement à la filtration q-bonne F).

L’application $n \mapsto \operatorname{long}_A(F_n/F_{n+1})$ s’appelle souvent la fonction de Hilbert-Samuel de M (relativement à F).

Cela s’applique notamment au cas de la filtration q-adique ($F_n = q^nM$); on pose alors $H_{M,F} = H_{M,q}$. On a donc

(9)
$$
H_{M,q} = \sum_{n \in \mathbf{Z}} \operatorname{long}_{A/q}(q^nM/q^{n+1}M). T^n .
$$

#### Proposition 3 {#ac-viii-s4-prop-3 .statement}

a) Si F est une filtration q-bonne sur M, on a

(10)
$$
H_{M,F}^{(1)} = \sum_{n \in \mathbf{Z}} \operatorname{long}_A(M/F_{n+1}). T^n .
$$

b) Si F et F’ sont deux filtrations q-bonnes sur M, il existe un entier m tel que $H_{M,F'}^{(1)} \geq T^m H_{M,F}^{(1)}$.

La partie a) résulte aussitôt de la définition de $H_{M,F}^{(1)}$; la partie b) résulte de a) et du lemme 3.

#### Théorème 2 {#ac-viii-s4-thm-2 .statement}

Soient A un anneau noethérien, q un idéal de A, M un A-module de type fini tel que M/qM soit non nul et de longueur finie et F une filtration q-bonne sur M.

a) Il existe un entier d $\geq 0$, et un élément R de $\mathbf{Z}[T, T^{-1}]$, uniquement déterminés, tels que $R(1) > 0$ et $H_{M,F} = (1 - T)^{-d}R$.

b) Les entiers d et R(1) sont indépendants de la filtration q-bonne F choisie.

a) Considérons l’anneau gradué gr(A) tel que $\operatorname{gr}_n(A) = q^n/q^{n+1}$ et le gr(A)-module gradué gr(M) tel que $\operatorname{gr}_n(M) = F_n/F_{n+1}$. Puisque l’on a $F_{n_1} = M$ et $qF_n = F_{n+1}$ pour $n \geq n_0$, gr(M) est engendré par $\bigoplus_{n_1 \leq n \leq n_0} \operatorname{gr}_n(M)$, donc est de type fini. Par ailleurs, si $(x_1, ..., x_r)$ est un système générateur fini du A-module q, gr(A) est engendré par $\operatorname{gr}_0(A)$ et les classes des $x_i$ modulo $q^2$, donc est isomorphe à un anneau gradué quotient de $H = (A/q)[X_1, ..., X_r]$. D’après le th. 1 du n° 2, on a
$$
(1 - T)^r H_{M,F} \in \mathbf{Z}[T, T^{-1}] .
$$
On a $H_{M,F} \neq 0$ et il existe donc $d \in \mathbf{N}$ et $R \in \mathbf{Z}[T, T^{-1}]$ uniquement déterminés tels que $R(1) > 0$ et $H_{M,F} = (1 - T)^{-d}.R$ (lemme 2 du n° 1).

b) Soit $F'$ une autre filtration q-bonne et écrivons de même
$$
H_{M,F'} = (1 - T)^{-d'} R'.
$$
D’après la prop. 3, b), il existe un entier $m$ tel que $(1 - T)^{-d' - 1} R' \geq T^m (1 - T)^{-d - 1} R$.
D’après le lemme 2, b) du n° 1, cela implique $d' \geq d$ et, si $d' = d$, $R'(1) \geq R(1)$.
Échangeant les rôles de $F$ et $F'$, on obtient $d = d'$ et $R(1) = R'(1)$.

#### Remarque 1 {#ac-viii-s4-n3-rem-1 .statement}

Avec les notations de a), écrivons $R = \sum_{i \in \mathbf{Z}} a_i T^i$, et supposons $d > 0$.
D’après le n° 1, la relation $H_{M,F} = (1 - T)^{-d} R$ s’écrit aussi
$$
\text{(11)} \quad \operatorname{long}_A(F_n/F_{n+1}) = \sum_{i \in \mathbf{Z}} a_i \binom{n - i + d - 1}{d - 1} = \sum_{i \leq n} a_i \binom{n - i + d - 1}{d - 1}.
$$
De même, puisque $H^{(1)}_{M,F} = (1 - T)^{-d - 1} R$, on a
$$
\text{(12)} \quad \operatorname{long}_A(M/F_{n+1}) = \sum_{i \in \mathbf{Z}} a_i \binom{n - i + d}{d} = \sum_{i \leq n} a_i \binom{n - i + d}{d}.
$$

Soient $A$ un anneau noethérien, $q$ un idéal de $A$, $M$ un $A$-module de type fini tel que $M/qM$ soit de longueur finie. Si $M \neq qM$, il existe d’après le th. 2, b) des entiers $d_q(M) \geq 0$ et $e_q(M) > 0$ tels que, pour toute filtration q-bonne $F$ sur $M$, il existe $R \in \mathbf{Z}[T, T^{-1}]$ avec
$$
H_{M,F} = (1 - T)^{-d_q(M)} R , \quad R(1) = e_q(M) .
$$
Si $M = qM$, on pose par convention $d_q(M) = -\infty$, $e_q(M) = 0$.

#### Remarque 2 {#ac-viii-s4-n3-rem-2 .statement}

Dire que $M/qM$ est de longueur finie signifie que
$$
\operatorname{Supp}(M/qM) = \operatorname{Supp}(M) \cap V(q)
$$
est formé d’idéaux maximaux (IV, § 2, n° 5, prop. 7). Nous verrons ci-dessous (n° 4, corollaire au th. 3) que $d_q(M)$ est la borne supérieure des nombres $\dim_{A_m}(M_m)$, où $m$ parcourt l’ensemble $\operatorname{Supp}(M) \cap V(q)$.

#### Corollaire {#ac-viii-s4-n3-cor-1 .statement}

*Soient $A$ un anneau noethérien, $q$ un idéal de $A$, $M$ un $A$-module de type fini tel que $M/qM$ soit de longueur finie et $F$ une filtration q-bonne sur $M$.
a) Pour que l’on ait $d_q(M) \leq 0$, il faut et il suffit que la suite $(q^n M)$ soit stationnaire, ou encore que la suite $(F_n)$ soit stationnaire. On a alors, pour tout $n$ assez grand,
$$
\operatorname{long}(M/F_{n+1}) = \operatorname{long}(M/q^{n+1}M) = e_q(M) .
$$
b) Supposons que l’on ait $d_q(M) > 0$. On a alors
$$
\text{(13)} \quad \operatorname{long}_A(F_n/F_{n+1}) = e_q(M) n^{d_q(M) - 1}/(d_q(M) - 1)! + \rho_n n^{d_q(M) - 2},
$$
$$
\text{(14)} \quad \operatorname{long}_A(M/F_{n+1}) = e_q(M) n^{d_q(M)}/d_q(M)! + \sigma_n n^{d_q(M) - 1},
$$
où $\rho_n$ et $\sigma_n$ tendent vers une limite lorsque $n$ augmente indéfiniment.
Cela résulte aussitôt du th. 2 et de la formule (2) du n° 1.*

#### Remarque 3 {#ac-viii-s4-n3-rem-3 .statement}

Supposons q contenu dans le radical de A. Alors, d’après le lemme de Nakayama, la suite (q^nM) est stationnaire si et seulement si l’on a q^nM = 0 pour n assez grand. Il résulte alors de la partie a) du corollaire que l’on a d_q(M) \leq 0 si et seulement si M est de longueur finie et qu’on a alors e_q(M) = \operatorname{long}_A(M).

#### Proposition 4 {#ac-viii-s4-prop-4 .statement}

Soient A un anneau noethérien, x_1, ..., x_r des éléments de A, x l’idéal qu’ils engendrent et M un A-module de type fini tel que M/xM soit non nul et de longueur finie.
a) On a d_x(M) \leq r.
b) Si d_x(M) = r, alors e_x(M) \leq \operatorname{long}_A(M/xM).
c) Si la suite (x_1, ..., x_r) est complètement sécante pour M (A, X, p. 157), alors d_x(M) = r et e_x(M) = \operatorname{long}_A(M/xM). La réciproque est vraie si les x_i appartiennent au radical de A.

Soit H l’anneau de polynômes (A/x)[X_1, ..., X_r]. Munissons G = \bigoplus_n x^nM/x^{n+1}M de la structure de H-module gradué pour laquelle (X_i)_G est la multiplication par la classe de x_i modulo x^2. Avec les notations P_G, Q_G, c_G du no 2, on a H_{M,x} = P_G, donc (1 - T)^{-d_x(M)}R = (1 - T)^{-r}Q_G, où R(1) = e_x(M) > 0 et Q_G(1) = c_G.

On a donc, soit d_x(M) < r et c_G = 0, soit d_x(M) = r et c_G = e_x(M). Par ailleurs, d’après la prop. 1 du no 2, on a c_G \leq \operatorname{long}(M/xM), et il y a égalité si et seulement si l’homomorphisme canonique A/x[X_1, ..., X_r] \otimes_{A/x} M/xM \to \bigoplus_n x^nM/x^{n+1}M est bijectif. Cela entraîne la proposition, compte tenu de A, X, p. 160, th. 1.

#### Proposition 5 {#ac-viii-s4-prop-5 .statement}

Soient 0 \to M' \to M \to M'' \to 0 une suite exacte de modules de type fini sur un anneau noethérien A, et q un idéal de A.
a) Pour que M/qM soit de longueur finie, il faut et il suffit qu’il en soit ainsi de M'/qM' et M''/qM''.
b) Supposons M/qM de longueur finie. Alors l’on est dans l’un des trois cas suivants :
1) d_q(M) = d_q(M') > d_q(M'') \text{ et } e_q(M) = e_q(M'),
2) d_q(M) = d_q(M'') > d_q(M') \text{ et } e_q(M) = e_q(M''),
3) d_q(M) = d_q(M') = d_q(M'') \text{ et } e_q(M) = e_q(M') + e_q(M'').
a) On a Supp(M) = Supp(M') \cup Supp(M'') et l’assertion résulte de la remarque 2.
b) Munissons M d’une filtration q-bonne F (par exemple la filtration q-adique), M'' de la filtration quotient F'', et M' de la filtration induite F'. Les filtrations F' et F'' sont q-bonnes (III, § 3, no 1, prop. 1). Alors on a pour chaque n une suite exacte de A-modules
$$
0 \to F'_n/F'_{n+1} \to F_n/F_{n+1} \to F''_n/F''_{n+1} \to 0
$$
(III, § 2, no 4, prop. 2), de sorte que l’on a H_{M,F} = H_{M',F'} + H_{M'',F''}, ou encore
$$
(1 - T)^{-d_q(M)}R = (1 - T)^{-d_q(M')}R' + (1 - T)^{-d_q(M'')}R''
$$
avec R, R', R'' \in \mathbf{Z}[T, T^{-1}], R(1) = e_q(M), R'(1) = e_q(M'), R''(1) = e_q(M''). L’assertion b) en résulte aussitôt.

### 4. Degré de la fonction de Hilbert-Samuel

#### Théorème 3 {#ac-viii-s4-thm-3 .statement}

Soient $A$ un anneau local noethérien, $q$ un idéal de $A$ distinct de $A$ et $M$ un $A$-module de type fini tel que $M/qM$ soit de longueur finie. Alors l’entier $d_q(M)$ est la dimension du $A$-module $M$ ($§ 1$, no 4, déf. 8).

On peut supposer $M \neq 0$. Démontrons l’inégalité $d_q(M) \leq \dim_A(M)$. D’après le cor. 2 à la prop. 9 du $§ 3$, no 5, il existe $x_1, ..., x_r \in q$, avec $r = \dim_A(M)$ et $\operatorname{long}(M / \sum_{i=1}^r x_i M) < +\infty$; posons $x = \sum_{i=1}^r x_i A$. D’après la prop. 4 du no 3, on a $d_x(M) \leq r$; on a $x \subset q$, d’où $H^{(1)}_{M,q} \leq H^{(1)}_{M,x}$ et donc (lemme 2 du no 1)

$$
d_q(M) \leq d_x(M) \leq r = \dim_A(M).
$$

Démontrons maintenant, par récurrence sur $\dim_A(M)$, l’inégalité $\dim_A(M) \leq d_q(M)$, évidente lorsque $\dim_A(M) = 0$.

Supposons qu’on ait $\dim_A(M) > 0$, et $\dim_A(N) \leq d_q(N)$ pour tout $A$-module de type fini $N$ tel que $\dim_A(N) < \dim_A(M)$. Si $0 = M_0 \subset M_1 \subset ... \subset M_n = M$ est une suite de composition de $M$, on a $\dim_A(M) = \sup(\dim_A(M_i/M_{i-1}))$ ($§ 1$, no 4, prop. 9) et $d_q(M) = \sup(d_q(M_i/M_{i-1}))$ (no 3, prop. 5). D’après IV, $§ 1$, no 4, th. 1, on peut donc supposer que $M$ est de la forme $A/p$, où $p$ est un idéal premier de $A$, et l’on a $p \neq m_A$ car $\dim_A(M) > 0$. Soit $x \in m_A - p$; l’homothétie $x_M$ de $M = A/p$ est injective, et l’on a la suite exacte

$$
0 \longrightarrow M \xrightarrow{x_M} M \longrightarrow M/xM \longrightarrow 0.
$$

D’après le $§ 3$, no 2, prop. 3, on a $\dim_A(M/xM) = \dim_A(M) - 1$; d’après la prop. 5 du no 3, et la suite exacte précédente, on a $d_q(M/xM) \leq d_q(M) - 1$. D’après l’hypothèse de récurrence, on a donc

$$
\dim_A(M) = \dim_A(M/xM) + 1 \leq d_q(M/xM) + 1 \leq d_q(M),
$$

ce qui achève la démonstration.

#### Corollaire {#ac-viii-s4-n4-cor-1 .statement}

Soient $A$ un anneau noethérien, $M$ un $A$-module de type fini et $q$ un idéal de $A$ tel que $M/qM$ soit de longueur finie. Alors $d_q(M)$ est la borne supérieure des dimensions $\dim_{A_m}(M_m)$, où $m$ parcourt l’ensemble fini $S = \operatorname{Supp}(M) \cap V(q)$, et $e_q(M)$ est la somme des $e_{q_m}(M_m)$ étendue à ceux des éléments $m$ de $S$ pour lesquels on a $\dim_{A_m}(M_m) = d_q(M)$.

Pour chaque entier $n$, la longueur de $M/q^nM$ est la somme des $\operatorname{long}_{A_m}(M_m/q^n_m M_m)$ (IV, $§ 2$, no 5, cor. 1 à la prop. 7 et corollaire à la prop. 8). Par conséquent, on a $H_{M,q} = \sum_{m \in S} H_{M_m,q_m}$, d’où le corollaire.

#### Remarque 1 {#ac-viii-s4-n4-rem-1 .statement}

On a aussi $d_q(M) = \sup_{m \in V(q)} \dim(M_m)$, c’est-à-dire $d_q(M) = \dim(\hat{M})$, où $\hat{M}$ est le complété de $M$ pour la topologie q-adique ($§ 3$, no 4, prop. 8).

#### Remarque 2 {#ac-viii-s4-n4-rem-2 .statement}

Supposons q contenu dans le radical de A ; alors $\dim(\hat{M}) = \dim(M)$ (*loc. cit.*, cor. 1), donc $d(M) = \dim(M)$.

### 5. Série de Hilbert-Samuel d’un module quotient

#### Lemme 5 {#ac-viii-s4-lem-5 .statement}

Soient A un anneau, M un A-module et $(P_n), (Q_n)$ deux filtrations décroissantes sur M formées de sous-modules. Supposons que l’on ait $P_n \supset Q_n$ et $\operatorname{long}_A(P_n/Q_n) < +\infty$ pour tout $n \in \mathbf{Z}$ et qu’il existe un entier $n_1$ tel que $Q_{n_1} = M$. Dans $\mathbf{Z}((T))$, on a les inégalités

$$
\sum_{n \in \mathbf{Z}} \operatorname{long}_A((P_{n+1} \cap Q_n)/Q_{n+1}).T^n \leq \sum_{n \in \mathbf{Z}} \operatorname{long}_A(P_{n+1}/Q_{n+1}).T^n \leq
$$
$$
\leq (1-T)^{-1} \sum_{n \in \mathbf{Z}} \operatorname{long}_A((P_{n+1} \cap Q_n)/Q_{n+1}).T^n .
$$

Il s’agit de prouver qu’on a les inégalités

(15) $\operatorname{long}((P_{n+1} \cap Q_n)/Q_{n+1}) \leq \operatorname{long}(P_{n+1}/Q_{n+1})$,
(16) $\operatorname{long}(P_{n+1}/Q_{n+1}) \leq \sum_{i \leq n} \operatorname{long}((P_{i+1} \cap Q_i)/Q_{i+1})$.

La première est évidente. D’autre part, on a $P_{n+1} \cap Q_i = P_{n+1}$ pour $i \leq n_1$ et $P_{n+1} \cap Q_{n+1} = Q_{n+1}$; on en déduit l’inégalité
$$
\operatorname{long}(P_{n+1}/Q_{n+1}) \leq \sum_{i \leq n} \operatorname{long}((P_{n+1} \cap Q_i)/(P_{n+1} \cap Q_{i+1})) .
$$

Mais le A-module $(P_{n+1} \cap Q_i)/(P_{n+1} \cap Q_{i+1})$ est isomorphe à un sous-module de $(P_{i+1} \cap Q_i)/Q_{i+1}$, et l’inégalité (16) en résulte.

#### Lemme 6 {#ac-viii-s4-lem-6 .statement}

Soient A un anneau, M un A-module et $(F_n)$ une filtration décroissante sur M formée de sous-modules ; on suppose qu’il existe un entier $n_1$ tel que $F_{n_1} = M$. Soient f un endomorphisme de M, $M'$ son noyau et $M''$ son conoyau. On munit $M'$ de la filtration $(F'_n)$ induite par $(F_n)$ et $M''$ de la filtration $(F''_n)$ quotient de $(F_n)$. On suppose que $F_n/F_{n+1}$ est de longueur finie pour tout $n \in \mathbf{Z}$ et qu’il existe un entier $\delta$ tel que $f(F_n) \subset F_{n+\delta}$. Soit $\varphi$ l’endomorphisme gradué de degré $\delta$ du module gradué $\mathrm{gr}(M) = \bigoplus_{n \in \mathbf{Z}} F_n/F_{n+1}$ qu’on déduit de f. Entre les éléments suivants de $\mathbf{Z}((T))$

$$
H_M = \sum_{n \in \mathbf{Z}} \operatorname{long}_A(F_n/F_{n+1}).T^n
$$
$$
H_{M'} = \sum_{n \in \mathbf{Z}} \operatorname{long}_A(F'_n/F'_{n+1}).T^n
$$
$$
H_{M''} = \sum_{n \in \mathbf{Z}} \operatorname{long}_A(F''_n/F''_{n+1}).T^n
$$
$$
P_{\mathrm{Ker}(\varphi)} = \sum_{n \in \mathbf{Z}} \operatorname{long}_A(\mathrm{Ker}(\varphi_n)).T^n ,
$$

on a les inégalités

(17) $H_{M'} \leq P_{\mathrm{Ker}(\varphi)}$

(18) $(1 - T^\delta).H_M^{(1)} + T^\delta.P_{\mathrm{Ker}(\varphi)} \leq H_{M''}^{(1)} \leq (1 - T^\delta).H_M^{(1)} + T^\delta.P_{\mathrm{Ker}(\varphi)}^{(1)}$.

La suite des sous-modules $G_n = f^{-1}(F_{n+\delta})$ de $M$ est une filtration décroissante, et l’on a $F_n \subset G_n$ pour tout entier $n$.
Par définition, on a $\mathrm{Ker}(\varphi_n) = (G_{n+1} \cap F_n)/F_{n+1}$, d’où

(19) $P_{\mathrm{Ker}(\varphi)} = \sum_{n \in \mathbf{Z}} \mathrm{long}_A((G_{n+1} \cap F_n)/F_{n+1}).T^n$.

Pour tout $n$, le A-module $(M' \cap F_n)/(M' \cap F_{n+1})$ s’identifie à un sous-module de $(G_{n+1} \cap F_n)/F_{n+1}$, et l’inégalité (17) résulte aussitôt de (19). D’après le lemme 5, on a par ailleurs

(20) $P_{\mathrm{Ker}(\varphi)} \leq \sum_{n \in \mathbf{Z}} \mathrm{long}_A(G_{n+1}/F_{n+1}).T^n \leq P_{\mathrm{Ker}(\varphi)}^{(1)}$.

Pour tout $n \in \mathbf{Z}$, on a une suite exacte de A-modules

$$ 0 \longrightarrow G_{n+1}/F_{n+1} \longrightarrow M/F_{n+1} \xrightarrow{f_n} M/F_{n+\delta+1} \longrightarrow M''/F''_{n+\delta+1} \longrightarrow 0, $$

où $f_n$ se déduit de $f$ par passage aux quotients. On a par conséquent

$\mathrm{long}_A(M''/F''_{n+\delta+1}) = \mathrm{long}_A(M/F_{n+\delta+1}) - \mathrm{long}_A(M/F_{n+1}) + \mathrm{long}_A(G_{n+1}/F_{n+1})$.

Multipliant par $T^{n+\delta}$ et sommant sur $n$, on obtient

(21) $H_{M''}^{(1)} = (1 - T^\delta)H_M^{(1)} + T^\delta.\sum_{n \in \mathbf{Z}} \mathrm{long}_A(G_{n+1}/F_{n+1}).T^n,$

et l’inégalité (18) résulte aussitôt de (20) et (21).

#### Lemme 7 {#ac-viii-s4-lem-7 .statement}

Conservons les notations du lemme 6.

a) On a l’inégalité $H_{M''}^{(1)} \geq \frac{1 - T^\delta}{1 - T} H_M$.

b) Pour que l’on ait égalité, il faut et il suffit que $\varphi$ soit injectif.

c) S’il en est ainsi, on a $M' \subset \bigcap_n F_n$, et la suite de A-modules

$$ 0 \longrightarrow \mathrm{gr}(M) \xrightarrow{\varphi} \mathrm{gr}(M) \xrightarrow{v} \mathrm{gr}(M'') \longrightarrow 0, $$

où $v$ est l’application canonique, est exacte.

Les assertions a) et b) résultent de la formule (18) du lemme 6, et de la définition $H_M^{(1)} = (1 - T)^{-1}.H_M$.

Supposons que $\varphi$ soit injectif. D’après III, § 2, no 8, th. 1, (i), on a

$$ \mathrm{Ker}(f) \subset f^{-1}(F_{n+\delta}) = F_n $$

pour tout $n$, d’où la première assertion de c). On a par ailleurs une suite exacte

$$
0 \longrightarrow M/M' \xrightarrow{f'} M \longrightarrow M/f(M) \longrightarrow 0,
$$

où $f'$ est déduit de $f$ par passage au quotient. Si $\varphi$ est injectif, on a comme ci-dessus ${f'}^{-1}(F_n) = F_{n-\delta}/M'$. Par suite la filtration sur $M/M'$ déduite par image réciproque par $f'$ de la filtration $F$ sur $M$ est la filtration $n \mapsto F_{n-\delta}/M'$; le gradué associé est $\mathrm{gr}(M)(-\delta)$ et on a une suite exacte de modules gradués (III, § 2, no 4, prop. 2)

$$
0 \longrightarrow \mathrm{gr}(M)(-\delta) \xrightarrow{\varphi'} \mathrm{gr}(M) \longrightarrow \mathrm{gr}(M'') \longrightarrow 0,
$$

où $\varphi'_n = \varphi_{n-\delta}$ pour tout $n$. Cela achève de démontrer c).

#### Proposition 6 {#ac-viii-s4-prop-6 .statement}

*Soient A un anneau noethérien, M un A-module de type fini et q un idéal de A tels que M/qM soit de longueur finie. Soit F une filtration q-bonne de M, et soit $\mathrm{gr}(A) = \bigoplus_{n \geq 0} (q^n/q^{n+1})$ l’anneau gradué associé à A pour la filtration q-adique.*

*Soient $(x_1, ..., x_s)$ une suite d’éléments de A, $(\delta_1, ..., \delta_s)$ une suite d’entiers strictement positifs telle que $x_i \in q^{\delta_i}$ pour $1 \leq i \leq s$, et soit $\xi_i$ la classe de $x_i$ dans $\mathrm{gr}_{\delta_i}(A) = q^{\delta_i}/q^{\delta_i+1}$.*

a) Munissons le A-module $\overline{M} = M/(x_1M + \cdots + x_sM)$ de la filtration q-bonne $\overline{F}$ quotient de F. On a alors dans $\mathbf{Z}((T))$ l’inégalité

$$
H_{\overline{M}, \overline{F}}^{(s)} \geq \left( \prod_{i=1}^s \frac{1 - T^{\delta_i}}{1 - T} \right) \cdot H_{M, F}.
$$

b) *Pour qu’il y ait égalité dans (22), il faut et il suffit que la suite $(\xi_1, ..., \xi_s)$ d’éléments de l’anneau $\mathrm{gr}(A)$ soit complètement sécante pour le module $\mathrm{gr}(M) = \bigoplus_{n} (F_n/F_{n+1})$.*

*En ce cas, l’homomorphisme canonique de $\mathrm{gr}(M)/\sum_{i=1}^s \xi_i \cdot \mathrm{gr}(M)$ dans $\mathrm{gr}(\overline{M}) = \bigoplus (\overline{F}_n/\overline{F}_{n+1})$ est un isomorphisme.*

c) *Supposons les conditions de b) satisfaites, et que chacun des A-modules $M_i = M/(x_1M + \cdots + x_iM)$ ($0 \leq i < s$) soit séparé pour la topologie q-adique¹. Alors la suite $(x_1, ..., x_s)$ est complètement sécante pour le A-module M.*

Lorsque $s = 1$, on a $\bigcap_n F_n = \bigcap_n q^nM$ et la suite $\{ \xi_1 \}$ est complètement sécante pour $\mathrm{gr}(M)$ si et seulement si l’homothétie de rapport $\xi_1$ dans $\mathrm{gr}(M)$ est injective. La prop. 6 résulte alors aussitôt du lemme 7 appliqué à l’homothétie $f = (x_1)_M$ dans M.

Supposons que l’on ait $s \geq 2$ et raisonnons par récurrence sur s. L’hypothèse de récurrence appliquée au A-module $M_1 = M/x_1M$ muni de la filtration G quotient de F, et à la suite $(x_2, ..., x_s)$ fournit l’inégalité

$$
H_{M_1, G}^{(s-1)} \geq \left( \prod_{i=2}^s \frac{1 - T^{\delta_i}}{1 - T} \right) \cdot H_{M_1, G};
$$

¹ Ceci se produit en particulier si q est contenu dans le radical de A (III, § 3, no 3, prop. 6).

il y a égalité si et seulement si la suite $(\xi_2, ..., \xi_s)$ est complètement sécante pour le gr(A)-module $gr(M_1) = \bigoplus_n G_n/G_{n+1}$. Comme les éléments $\frac{1 - T^{\delta_i}}{1 - T}$ de $\mathbf{Z}((T))$ sont positifs, le cas $s = 1$ déjà traité et la formule (23) fournissent les inégalités

$$
H^{(s)}_{M,F} \geq \left( \prod_{i=2}^s \frac{1 - T^{\delta_i}}{1 - T} \right) \cdot H^{(1)}_{M_1,G} \geq \left( \prod_{i=1}^s \frac{1 - T^{\delta_i}}{1 - T} \right) \cdot H_{M,F}.
$$

Ceci prouve *a*).

On ne peut avoir égalité dans (22) que si l’on a simultanément l’égalité dans (23) et l’égalité

$$
H^{(1)}_{M_1,G} = \left( \frac{1 - T^{\delta_1}}{1 - T} \right) \cdot H_{M,F}.
$$

Cette dernière relation signifie que $\{\xi_1\}$ est complètement sécante pour gr(M) et implique que l’homomorphisme canonique de gr(M)/$\xi_1\cdot$gr(M) dans gr(M_1) est un isomorphisme. Autrement dit, on a égalité dans (22) si et seulement si $\{\xi_1\}$ est complètement sécante pour gr(M) et $\{\xi_2, ..., \xi_s\}$ complètement sécante pour gr(M)/$\xi_1\cdot$gr(M). Ceci signifie que $\{\xi_1, ..., \xi_s\}$ est complètement sécante pour gr(M) (A, X, p. 160, cor. 2). On a ainsi démontré l’équivalence des deux conditions de *b*). Supposons-les satisfaites ; alors, d’après l’hypothèse de récurrence gr(M) s’identifie à $gr(M_1)/\sum_{i=2}^s \xi_i \cdot gr(M_1)$; comme par ailleurs gr(M_1) s’identifie à gr(M)/$\xi_1\cdot$gr(M), la dernière assertion de *b*) est ainsi satisfaite.

Supposons maintenant que $\{\xi_1, ..., \xi_s\}$ soit complètement sécante pour gr(M) et M_i séparé pour la topologie q-adique (pour $0 \leq i < s$). D’après ce qui précède et l’hypothèse de récurrence, la suite $(x_2, ..., x_s)$ est complètement sécante pour M_1 ; comme on a $M_1 = M/x_1M$ et que $\{x_1\}$ est complètement sécante pour M, la suite $(x_1, x_2, ..., x_s)$ est complètement sécante pour M (A, X, p. 160, th. 1).

## EXERCICES {#ac-viii-s4-exercises}

See the [exercises for § 4](exercises/s4/).
