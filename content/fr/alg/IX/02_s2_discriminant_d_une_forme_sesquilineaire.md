---
book: alg
book_title: Algebra
chapter: IX
chapter_title: Formes sesquilinéaires et formes quadratiques
section: 2
section_title: Discriminant d'une forme sesquilinéaire
lang: fr
source: alg-ix-fr
pdf_pages: 0039-0047
extraction: ocr
statements: 12
exercises: 0
content_sha256: a03e917bbb712788678cb44f2f8c4eeb837bff91ffaff8fe794b3c2a69ffeff6
---

## § 2. DISCRIMINANT D’UNE FORME SESQUILINÉAIRE

par exemple $A = \mathbf{F}_p(X)$, où $p$ est premier ; $E'' = A'' \otimes_A E$ est alors un espace vectoriel de même dimension sur $A''$ que $E$ sur $A$; considérer l’application $M \to A'' \otimes_A M$.

c) On suppose $A' = A$. Soit $\omega$ une application bijective de $\mathfrak{F}(E)$ sur l’ensemble $\mathfrak{F}'(E')$ des sous-espaces de codimension finie de $E'$, telle que $\operatorname{codim} \omega(M) = \dim M$, et $\omega(M + N) = \omega(M) \cap \omega(N)$. Montrer qu’il existe une forme sesquilinéaire $\Phi$ sur $E \times E'$, non dégénérée à droite, et telle que $\omega(M) = M^0$ pour tout $M \in \mathfrak{F}(E)$. (Utiliser le th. 1 du chap. II, § 4, n° 6).

¶ 11) a) Soit $A$ un anneau artinien à gauche et à droite (chap. VIII, § 2, n° 3). Montrer que les conditions suivantes sont équivalentes : 1° l’annulateur à droite (resp. à gauche) de tout idéal à gauche (resp. à droite) $\neq A$ n’est pas réduit à 0 ; 2° le dual de tout $A$-module à gauche (resp. à droite) simple n’est pas réduit à 0 ; 3° le dual de tout $A$-module à gauche (resp. à droite) de type fini n’est pas réduit à 0. On dit qu’un anneau $A$ satisfait à la condition $(N_s)$ (resp. $(N_d)$) s’il vérifie ces conditions pour les $A$-modules à gauche (resp. à droite).

b) Soient $A$ un anneau artinien à gauche et à droite satisfaisant à la condition $(N_d)$, $E$ (resp. $F$) un $A$-module libre à gauche (resp. à droite), ayant une base dénombrable sur $A$, $\Phi$ une forme bilinéaire sur $E \times F$ telle que $s_\Phi$ soit injective. Soit $M$ un sous-module libre de $E$; montrer qu’il existe un sous-module libre $N$ de $F$ et une base $(e_n)$ (resp. $(f_n)$) de $M$ (resp. $N$) telles que $\Phi(e_i, f_j) = \delta_{ij}$; on peut en outre prendre pour $e_1$ un élément libre quelconque de $M$. (Remarquer que si $x$ est un élément libre de $M$, l’image de $F$ par l’application $y \to \Phi(x, y)$ est l’anneau $A$ tout entier ; procéder ensuite par récurrence pour construire les bases $(e_n)$ et $(f_n)$). En déduire que si la base $(e_n)$ de $M$ est finie, $E$ est somme directe de $M$ et de $N^0$, et que l’on a $M^{00} = M$.

c) On garde les hypothèses de b), et on suppose en outre que $A$ satisfait à la condition $(N_s)$ et que $d_\Phi$ est injective. Montrer alors qu’il existe une base $(e_n)$ dans $E$ et une base $(f_n)$ dans $F$ telles que $\Phi(e_i, f_j) = \delta_{ij}$. (Utiliser b) en déterminant par récurrence alternativement $e_n$ et $f_n$).

*12) Soient $E$ un espace hilbertien réel de type dénombrable, $\Phi(x, y)$ le produit scalaire dans $E$. Montrer qu’il n’existe pas de système de deux bases algébriques $(e_\lambda), (f_\mu)$ de l’espace vectoriel $E$ sur $\mathbf{R}$ telles que l’on ait $\Phi(e_\lambda, f_\mu) = \delta_{\lambda \mu}$ pour tout couple d’indices. (Remarquer d’abord que l’ensemble d’indices de ces bases aurait la puissance du continu ($Esp. vect. top.$, chap. II, § 3, exerc. 15)); considérer ensuite une base orthonormale (dénombrable) $(a_n)$ de $E$ et remarquer que le sous-espace engendré par les $a_n$ est contenu dans le sous-espace engendré par une sous-famille dénombrable de $(e_\lambda)$.*

#### Définition 1 {#alg-ix-s2-def-1 .statement}

Etant donnée une forme $\Phi$ sesquilinéaire pour $J$ sur $E$ et un système $S = (x_1, \ldots, x_n)$ de $n$ éléments de $E$, on appelle discriminant de $\Phi$ par rapport à ce système, et on note $D_\Phi(x_1, \ldots, x_n)$ ou $D_\Phi(S)$, l’élément $\det(\Phi(x_i, x_j))$ de $A$.

Si $(e_1, \ldots, e_n)$ est une base de $E$, le discriminant de $\Phi$ par rapport à cette base n’est autre que le déterminant de la matrice de $\Phi$ par rapport à cette base.

Il résulte de la définition de l’extension de $\Phi$ à $\wedge^n E$ ($§ 1$, no 9) que l’on a

$$
D_\Phi(x_1, \ldots, x_n) = \Phi_{(n)}(x_1 \wedge \ldots \wedge x_n, x_1 \wedge \ldots \wedge x_n),
$$

où $\Phi_{(n)}$ désigne l’extension de $\Phi$ à $\wedge^n E$. Pour toute permutation $\sigma \in \mathfrak{S}_n$, on a donc

$$
D_\Phi(x_{\sigma(1)}, \ldots, x_{\sigma(n)}) = D_\Phi(x_1, x_2, \ldots, x_n).
$$

#### Exemple {#alg-ix-s2-n0-exa-1 .statement}

Soit $B$ une algèbre sur l’anneau $A$, telle que $B$ soit un $A$-module libre de dimension finie $n$. Alors l’application $(x, y) \to \mathrm{Tr}_{B/A}(xy)$ (chap. VIII, § 12, no 2) est une forme bilinéaire sur $B$. Etant donné un système $(x_1, \ldots, x_n)$ de $n$ éléments de $B$, le discriminant de cette forme par rapport à ce système s’appelle le discriminant du système $(x_1, \ldots, x_n)$ sur $A$, et se note $D_{B/A}(x_1, \ldots, x_n)$. On a ainsi

$$
D_{B/A}(x_1, \ldots, x_n) = \det (\mathrm{Tr}_{B/A}(x_ix_j)).
$$

#### Remarque {#alg-ix-s2-n0-rem-1 .statement}

Soient $(e_1, \ldots, e_n)$ une base de $B$ sur $A$, et

$$
e_ie_j = \sum_{k=1}^n c_{ijk}e_k \quad (c_{ijk} \in A)
$$

(chap. II, § 7, no 2). Comme la matrice de l’endomorphisme $A$-linéaire $x \to e_kx$ de $B$ par rapport à $(e_r)$ est $(c_{ksr})$, on a $\mathrm{Tr}_{B/A}(e_k) = \sum_{r=1}^n c_{krr}$, d’où $\mathrm{Tr}_{B/A}(e_ie_j) = \sum_{k,r} c_{ijk}c_{krr}$. Il en résulte que l’on a

$$
D_{B/A}(e_1, \ldots, e_n) = \det_{i,j} (\sum_{k,r} c_{ijk}c_{krr}).
$$

#### Proposition 1 {#alg-ix-s2-prop-1 .statement}

Soient $\Phi$ une forme sesquilinéaire pour $J$ sur $E$, $(\tilde{x}_1, \ldots, x_n)$ un système de $n$ éléments de $E$, et $(a_{ij})_{(i,j = 1, \ldots, n)}$ une famille de $n^2$ éléments de $A$; posons $y_i = \sum_{i=1}^n a_{ji}x_i$. On a alors

$$
D_\Phi(y_1, \ldots, y_n) = \det (a_{ij}) \cdot \det (a_{ij})^j \cdot D_\Phi(x_1, \ldots, x_n).
$$

En effet, comme $\Phi$ est une forme sesquilinéaire, on a $\Phi(y_i, y_j) = \sum_{k,m} a_{ik} \Phi(x_k, x_m) a_{jm}^j$. Donc, si l’on note $A$ la matrice $(a_{ij})$, la matrice $(\Phi(y_i, y_j))$ est égale à $A . (\Phi(x_i, x_j)). {}^t A^j$. Comme $\det({}^t A) = \det(A)$, et que $\det(A^j) = \det(A)^j$, notre assertion est démontrée.

En particulier, si $(e_i)$ et $(e'_i)$ sont deux bases de $E, D$ et $D'$ les discriminants de $\Phi$ par rapport à ces bases, et $a$ le déterminant de la matrice de passage de la base $(e_i)$ à la base $(e'_i)$, on a
$$
(4) \qquad D' = aa^j D.
$$

Il résulte de la prop. 1 que, si $(e_i)$ est une base de $E$ et $(x_i)$ un système quelconque de $n$ éléments de $E$, $D_\Phi(e_1, \ldots, e_n)$ *divise* $D_\Phi(x_1, \ldots, x_n)$. En particulier les discriminants de $\Phi$ par rapport à deux bases quelconques de $E$ engendrent le même idéal principal de $A$.

Soient $(E_i)_{i \in I}$ une famille finie de $A$-modules libres de dimensions finies, $\Phi_i$ une forme sesquilinéaire pour $J$ sur $E_i$, et $B_i$ une base de $E_i$. Si $\Phi$ désigne la *somme directe* des $\Phi_i$ (§ 1, no 3) et $B$ la base de $\prod_{i \in I} E_i$ obtenue par réunion des $B_i$, on a évidemment
$$
(5) \qquad D_\Phi(B) = \prod_{i \in I} D_{\Phi_i}(B_i).
$$

Soient $\Phi$ une forme sesquilinéaire pour $J$ sur $E$, $h$ un homomorphisme de $A$ dans un anneau commutatif $A'$, $\Phi'$ la forme sesquilinéaire sur $A' \otimes_A E$ obtenue par extension de $\Phi$ (§ 1, no 4) et $(x_1, \ldots, x_n)$ un système quelconque d’éléments de $E$. Comme $A' \otimes_A E$ est un $A'$-module libre, $D_{\Phi'}(1 \otimes x_1, \ldots, 1 \otimes x_n)$ est défini, et on a évidemment
$$
(6) \qquad D_{\Phi'}(1 \otimes x_1, \ldots, 1 \otimes x_n) = h(D_\Phi(x_1, \ldots, x_n)).
$$

#### Exemple {#alg-ix-s2-n0-exa-2 .statement}

Soient $B$ une algèbre sur $A$ qui soit un $A$-module libre de dimension finie $n$, $(x_1, \ldots, x_n)$ une base de $B$ sur $A$, et $m$ un idéal de $A$. Si l’on note $h$ l’homomorphisme canonique de $B$ sur $B/mB$, $(h(x_1), \ldots, h(x_n))$ est une base de $B/mB$ sur $A/m$ (chap. I, § 6, no 5, prop. 5), et $B/mB$ est isomorphe à $(A/m) \otimes_A B$. On a donc
$$
D_{(B/mB)/(A/m)}(h(x_1), \ldots, h(x_n)) = h(D_{B/A}(x_1, \ldots, x_n)).
$$

#### Proposition 2 {#alg-ix-s2-prop-2 .statement}

On suppose que $A$ est intègre. Soient $\Phi$ une forme sesquilinéaire pour $J$ sur $E$ et $(e_1, \ldots, e_n)$ une base de $E$, telles que $D_\Phi(e_1, e_2, \ldots, e_n) \neq 0$.

a) Pour qu’un système $(x_1, \ldots, x_n)$ de $n$ éléments de $E$ soit libre, il faut et il suffit que $D_\Phi(x_1, \ldots, x_n)$ soit $\neq 0$.

b) Pour qu’un système $(x_1, \ldots, x_n)$ de $n$ éléments de $E$ soit une base de $E$, il faut et il suffit que $D_\Phi(x_1, \ldots, x_n)$ et $D_\Phi(e_1, \ldots, e_n)$ soient des éléments associés dans $A$ (cf. chap. VI, § 1, no 5).

Posons $x_j = \sum_{i=1}^n a_{ji} e_i$ ($a_{ji} \in A$). Démontrons d’abord a). Si $D_\Phi(x_1, \ldots, x_n) = 0$, on a $\det(a_{ji}) \cdot \det(a_{ji})' = 0$ (prop. 1) puisque $D_\Phi(e_1, \ldots, e_n) \neq 0$ et que $A$ est intègre ; on a donc $\det(a_{ji}) = 0$, et les vecteurs $x_j$ sont linéairement dépendants (chap. III, § 7, no 1, th. 1, appliqué à l’espace vectoriel $K \otimes_A E$, où $K$ désigne le corps des fractions de $A$). Réciproquement, si ces vecteurs sont linéairement dépendants on a $\det(a_{ji}) = 0$ (*ibid.*), d’où $D_\Phi(x_1, \ldots, x_n) = 0$ (prop. 1).

Démontrons maintenant b). Si $D_\Phi(x_1, \ldots, x_n)$ et $D_\Phi(e_1, \ldots, e_n)$ sont associés dans $A$, la prop. 1 montre que $\det(a_{ij}) \cdot \det(a_{ij})'$ est inversible dans $A$. Ainsi $\det(a_{ij})$ est lui aussi inversible dans $A$; donc la matrice $(a_{ij})$ sur $A$ est inversible (chap. III, § 6, no 5, th. 2), et l’endomorphisme $g$ de $E$ défini par $g(e_i) = x_i$ ($i = 1, \ldots, n$) est un automorphisme ; par conséquent $(x_1, \ldots, x_n)$ est une base de $E$. La réciproque résulte aussitôt de la prop. 1.

#### Proposition 3 {#alg-ix-s2-prop-3 .statement}

Soient $\Phi$ une forme sesquilinéaire pour $J$ sur $E$, et $S$ une base de $E$. Les conditions suivantes sont équivalentes :

a) L’application $s_\Phi$ de $E$ dans $E^*$ associée à $\Phi$ est bijective.

b) L’application $d_\Phi$ de $E$ dans $E^*$ associée à $\Phi$ est bijective.

c) L’élément $D_\Phi(S)$ est inversible dans $A$.

En effet la condition c) exprime que la matrice de $\Phi$ par rapport à $S$ est inversible (chap. III, § 6, no 5, th. 2). Donc c) est équivalente à a) ($§ 1,$ no 10) ; de même c) est équivalente à b).

#### Proposition 4 {#alg-ix-s2-prop-4 .statement}

On suppose $A$ intègre. Soit $S$ une base de $E$. Une condition nécessaire et suffisante pour qu’une forme sesquilinéaire $\Phi$ sur $E$ soit non dégénérée est que l’on ait $D_\Phi(S) \neq 0$.

Soit en effet K le corps des fractions de A, et soit $\Phi'$ l’extension de $\Phi$ au K-espace vectoriel $K \otimes_A E$; identifions E à une partie de cet espace vectoriel. La relation $D_{\Phi}(S) \neq 0$ est alors équivalente à $D_{\Phi'}(S) \neq 0$ (formule (6)), qui elle-même exprime que $s_{\Phi'}$ est bijective (prop. 3), c’est-à-dire que $\Phi'$ est non dégénérée (§ 1, no 6, prop. 6). Or, pour tout $x \in K \otimes_A E$, il existe $a \in A$ tel que $ax \in E$; par suite, pour que $\Phi$ soit dégénérée, il faut et il suffit que $\Phi'$ le soit. Ceci démontre notre assertion.

#### Proposition 5 {#alg-ix-s2-prop-5 .statement}

*Soient A un corps, B une algèbre commutative de dimension finie n sur A, et S une base de B. Pour que B soit séparable (chap. VIII, § 7, no 5, déf. 1) il faut et il suffit que l’on ait* $D_{B/A}(S) \neq 0$.

Soient en effet $A'$ la clôture algébrique de A, et $B'$ l’algèbre $A' \otimes_A B$ sur $A'$. Si B est séparable, $B'$ est semi-simple (chap. VIII, § 7, no 5, cor. de la prop. 7) et est donc composée directe de n corps isomorphes à $A'$ (chap. VIII, § 6, no 4, cor. de la prop. 9). Si $S'$ désigne la base canonique de $B'$ (identifiée à ${A'}^n$), on a $D_{B'/A'}(S') = 1$, d’où $D_{B'/A'}(S) \neq 0$ (prop. 1) et $D_{B/A}(S) \neq 0$ (formule (6)).

Réciproquement supposons que l’on ait $D_{B/A}(S) \neq 0$. Pour montrer que B est séparable, il suffit de montrer que $B'$ est semi-simple, c’est-à-dire qu’elle n’admet pas d’élément nilpotent $\neq 0$. Or, si $x'$ était un élément nilpotent non nul de $B'$, on pourrait le prendre comme premier élément d’une base $S'$ de $B'$, et on aurait alors $\mathrm{Tr}_{B'/A'}(x'y') = 0$ pour tout $y' \in S'$ puisqu’un endomorphisme nilpotent a ses valeurs propres nulles (chap. VII, § 5, no 3, cor. 3 de la prop. 8), donc une trace nulle. Il en résulterait que $D_{B'/A'}(S') = 0$, d’où $D_{B'/A'}(S) = 0$ (prop. 1) et $D_{B/A}(S) = 0$ (formule (6)), contrairement à l’hypothèse.

#### Remarque {#alg-ix-s2-n0-rem-2 .statement}

Supposons que B soit un surcorps de A. Soient $S = (x_1, \ldots, x_n)$ une base de B, et $(s_1, \ldots, s_n)$ les A-isomorphismes de B dans la clôture algébrique $A'$ de A (chaque $s_j$ étant répété $[B : A]_i$ fois). Rappelons que, pour tout $z \in B$, on a $\mathrm{Tr}_{B/A}(z) = \sum_{j=1}^n s_j(z)$ (chap. VIII, § 12, no 2, prop. 4).

Il résulte alors de la formule de multiplication des déterminants que l’on a

$$(7)\quad (\det(s_j(x_i)))^2 = D_{B/A}(x_1, \ldots, x_n).$$

Cette formule montre que la proposition 5 généralise la condition de séparabilité donnée au chap. V, § 7, no 2, Remarque.

#### Proposition 6 {#alg-ix-s2-prop-6 .statement}

Soient $\Phi$ une forme A-bilinéaire sur E, et K un sous-anneau de A tel que A soit un K-module libre de dimension finie q. Si $(e_i)_{i=1,\ldots,n}$ est une base de E sur A et $(a_j)_{j=1,\ldots,q}$ une base de A sur K, alors $(a_j e_i)$ est une base de E sur K. L’application $\Phi'$ de $E \times E$ dans K définie par $\Phi'(x, y) = \mathrm{Tr}_{A/K}(\Phi(x, y))$ est une forme K-bilinéaire sur E, et on a

$$(8)\quad D_{\Phi'}(a_j e_i) = N_{A/K}(D_\Phi(e_1, \ldots, e_n)) \cdot (D_{A/K}(a_1, \ldots, a_q))^n.$$

Les deux premières assertions étant évidentes, il suffit de démontrer (7). Par définition le premier membre est le déterminant de l’endomorphisme K-linéaire $u$ de E défini par

$$u(a_j e_i) = \sum_{r,s} \mathrm{Tr}_{A/K}(a_j a_r \Phi(e_i, e_s)) a_r e_s.$$

Considérons l’endomorphisme A-linéaire $v$ de E défini par $v(e_i) = \sum_s \Phi(e_i, e_s) e_s$, et l’endomorphisme K-linéaire $w$ de E défini par $w(a_j e_i) = (\sum_r \mathrm{Tr}_{A/K}(a_j a_r) a_r) e_i$. On a

$$w(v(a_j e_i)) = w(\sum_s a_j \Phi(e_i, e_s) e_s) = \sum_{r,s} \mathrm{Tr}_{A/K}(a_j \Phi(e_i, e_s) a_r) a_r e_s$$

puisque $w(a e_s) = \sum_r \mathrm{Tr}_{A/K}(a a_r) a_r e_s$ pour tout $a \in A$; ainsi $u$ est l’application composée $w \circ v$. Donc, en notant $v_K$ l’application $v$ considérée comme application K-linéaire, on a $\det(u) = \det(v_K) \det(w)$. Or on a $\det(v_K) = N_{A/K}(\det(v))$ (chap. VIII, § 12, no 2, prop. 7), et il est clair que $\det(v) = D_\Phi(e_1, \ldots, e_n)$. D’autre part, comme chacun des A-modules $Ae_i (i = 1, \ldots, n)$ est stable pour $w$, et que le déterminant de la restriction de $w$ à $Ae_i$ est $\det(\mathrm{Tr}_{A/K}(a_j a_r)) = D_{A/K}(a_1, \ldots, a_q)$, on a $\det(w) = (D_{A/K}(a_1, \ldots, a_q))^n$. La formule (8) se réduit donc à $\det(u) = \det(v_K) \det(w)$, formule démontrée ci-dessus.

#### Corollaire (« Formule de transitivité des discriminants ») {#alg-ix-s2-n0-cor-1 .statement}

Soient K un anneau commutatif, A une algèbre commutative admettant une base finie $(a_j)_{j=1,\ldots,q}$ sur K, et E une algèbre sur A admettant une base finie $(e_i)_{i=1,\ldots,n}$. Alors $(a_j e_i)$ est une base de E sur K, et on a

$$
D_{E/K}(a_j e_i) = N_{A/K}(D_{E/A}(e_1, \ldots, e_n)) \cdot (D_{A/K}(a_1, \ldots, a_q))^n.
$$

En effet, si l’on pose $\Phi(x, y) = \operatorname{Tr}_{E/A}(xy)$, la forme K-bilinéaire $\Phi'$ de la prop. 6 est $\Phi'(x, y) = \operatorname{Tr}_{E/K}(xy)$ d’après la formule de transitivité des traces (Chap. VIII, § 12, n° 2, cor. de la prop. 7).

Exercices. — 1) Soit A une algèbre de rang fini sur un corps commutatif K, ayant un élément unité.
   a) Montrer que si le radical de A n’est pas nul, la forme bilinéaire $(x, y) \to \operatorname{Tr}_{A/K}(xy)$ sur A est dégénérée.
   b) On suppose que K est de caractéristique 0. Montrer que si A est une algèbre de matrices $M_n(K)$, S la base canonique de A sur K, on a $D_{A/K}(S) \neq 0$.
   c) Déduire de a) et b) que, pour qu’une algèbre A de rang fini sur un corps K de caractéristique 0 soit absolument semi-simple, il faut et il suffit que la forme bilinéaire $(x, y) \to \operatorname{Tr}_{A/K}(xy)$ soit non dégénérée (ou, ce qui revient au même, que $D_{A/K}(S) \neq 0$ pour toute base S de A sur K).

¶ 2) Soient B un anneau, A un sous-anneau de B contenant l’élément unité de B ; B est donc un (A, A)-bimodule ; on désigne par $^sB$ (resp. $^dB$) l’ensemble B considéré comme A-module à gauche (resp. à droite), par $^sB^*$ (resp. $^dB^*$) le A-module à droite (resp. à gauche) dual de $^sB$ (resp. $^dB$). Pour tout $x' \in ^sB^*$ et tout $b \in B$, $x \to \langle xb, x' \rangle$ est une forme A-linéaire sur $^sB$, donc un élément de $^sB^*$ qu’on désigne par $bx'$ ; l’application $(b, x') \to bx'$ définit sur $^sB^*$ une structure de B-module à gauche (cf. chap. III, 2e éd., App. II, n° 7).
   a) Soit $\varphi$ un homomorphisme du (A, A)-bimodule B dans le (A, A)-bimodule A ; pour que l’application A-bilinéaire $\Phi : (x, y) \to \varphi(xy)$ de $^sB \times ^dB$ dans A soit non dégénérée, il faut et il suffit que $\varphi(0)$ ne contienne aucun idéal (à gauche ou à droite) de B distinct de $\{0\}$. On dit alors que $\varphi$ est un homomorphisme frobeniusien de B dans A.
   b) Soit $\varphi$ un homomorphisme frobeniusien de B dans A ; montrer que l’application $d_\varphi$ associée à droite à $\Phi$ est un isomorphisme du B-module à gauche $B_s$ sur un sous-module du B-module à gauche $^sB^*$. Montrer que $d_\varphi$ est bijectif dans chacun des deux cas suivants : 1° A est un anneau artinien à gauche et à droite satisfaisant aux conditions (N_s) et (N_d) (§ 1, exerc. 11), et $^sB$ et $^dB$ sont des A-modules libres de longueurs finies (utiliser l’exerc. 11 b) du § 1) ; 2° A est un anneau artinien commutatif et involutif (chap. VIII, § 3, exerc. 11), contenu dans le centre de B, et $^sB$ est un A-module de longueur finie (utiliser l’exerc. 11 du chap. VIII, § 3).

c) Réciproquement, montrer que si $B_s$ et $^sB^*$ sont isomorphes, il existe un homomorphisme frobeniusien de B dans A lorsqu’on est dans l’un des deux cas considérés dans b) et que $^sB$ et $^dB$ ont même longueur (utiliser l’exerc. 11 b) du § 1).

d) Avec les hypothèses et notations de a), montrer que l’annulateur à droite (resp. à gauche) d’un idéal à gauche I (resp. d’un idéal à droite r) de B, est l’orthogonal $l^0$ (resp. $r^0$) pour la forme $\Phi$ du sous-module I (resp. r) de $^sB$ (resp. $^dB$).

e) Soit $\varphi$ un homomorphisme frobeniusien de B dans A. Montrer que si A est un anneau artinien involutif (chap. VIII, § 3, exerc. 11) il en est de même de B, lorsqu’on suppose en outre que l’une ou l’autre des conditions de b) est vérifiée (utiliser b) et d)).

¶ 3) Soient A un corps commutatif, B une algèbre de rang fini sur A, ayant un élément unité.

a) Pour que B soit une algèbre frobeniusienne, il faut et il suffit qu’il existe un homomorphisme frobeniusien de B dans A (exerc. 2). (Utiliser l’exerc. 2 c) et e) ci-dessus, et l’exerc. 6 b) du chap. VIII, § 13).

b) Soit $\varphi$ un homomorphisme frobeniusien de B dans A ; toute forme A-linéaire sur B peut alors s’écrire d’une seule manière $x \to \varphi(b'x)$ (resp. $x \to \varphi(xb'')$) où $b'$ et $b''$ appartiennent à B ; pour que cette forme soit un homomorphisme frobeniusien, il faut et il suffit que $b'$ (resp. $b''$) soit inversible dans B.

c) Pour tout $x \in B$, soit $x^\sigma$ l’unique élément (cf. b)) tel que $\varphi(xy) = \varphi(yx^\sigma)$ pour tout $y \in B$. Montrer que $x \to x^\sigma$ est un A-automorphisme de B. On dit que l’algèbre frobeniusienne B est symétrique si $\sigma$ est un automorphisme intérieur de B ; il y a alors un homomorphisme frobeniusien de B dans A pour lequel $\sigma$ est l’identité (cf. b)). Il revient au même de dire que les (B, B)-bimodules B et $^sB^* = ^dB^*$ (qu’on écrit B*) sont isomorphes (exerc. 2 c)).

d) Soient E un B-module à gauche de longueur finie, E’ son dual, E’* le dual de E’ considéré comme espace vectoriel sur A ; E’* est muni d’une structure de B-module à gauche en posant, pour $x' \in E'$, $x'' \in {E'}^*$, $b \in B$, $\langle x', bx'' \rangle = \langle x'b, x'' \rangle$ (chap. III, 2e éd., App. II, n° 7). Pour tout $x \in E$, soit $f_E(x)$ (ou simplement $f(x)$) l’élément de E’*tel que $\langle x', f(x) \rangle = \varphi(\langle x, x' \rangle)$ pour tout $x' \in E'$; montrer que $f$ est une bijection semi-linéaire pour l’automorphisme $\sigma$, du B-module à gauche E sur le B-module à gauche E’* (utiliser l’exerc. 10 du chap. VIII, § 4). Pour $E = B_s$, on a (avec les notations de l’exerc. 2 b)) $d_\Phi(x^\sigma) = f_{B_s}(x)$ pour tout $x \in B$.

4) a) Soit G un groupe fini. Montrer que l’algèbre B du groupe G sur un corps commutatif quelconque A est une algèbre frobeniusienne symétrique (exerc. 3). (Considérer l’application $\varphi$ de B dans A qui, à tout élément $x = \sum_{s \in G} \xi_s . s$, associe $\varphi(x) = \xi_e$, e désignant l’élément neutre de G).

b) Soient E un espace vectoriel de dimension finie $n$ sur un corps commutatif A, et B l’algèbre extérieure $\wedge E$. Montrer que B est une algèbre frobeniusienne. (Si $(e_i)_{1 \leq i \leq n}$ est une base de E, considérer l’application qui à tout élément $x$ de B associe le coefficient de $e_1 \wedge e_2 \wedge \ldots \wedge e_n$ dans l’expression de $x$ à l’aide de la base de B correspondant à $(e_i)$). Pour que l’algèbre frobeniusienne B soit symétrique, il faut et il suffit que $n$ soit pair ou A de caractéristique 2.

¶ 5) a) Montrer que le produit tensoriel de deux algèbres frobeniusiennes (resp. frobeniusiennes et symétriques) de rang fini sur un corps commutatif K est une algèbre frobeniusienne (resp. frobeniusienne et symétrique) (cf. § 1, n° 9, prop. 9).

b) Soient B une algèbre de rang fini sur K, L une extension de K de degré fini sur K. Montrer que si l’algèbre $B_{(L)} = B \otimes_K L$ sur L est frobeniusienne (resp. frobeniusienne et symétrique), il en est de même de B. (Utiliser les exerc. 2 c) et 3 c) ci-dessus et l’exerc. 2 du chap. VIII, § 2).

6) Montrer que toute algèbre absolument semi-simple B de rang fini sur un corps commutatif A est une algèbre frobeniusienne symétrique. (Se ramener au cas où B est simple ; utiliser l’exerc. 5 b) ci-dessus, ainsi que la prop. 9 du chap. VIII, § 12, n° 3).
