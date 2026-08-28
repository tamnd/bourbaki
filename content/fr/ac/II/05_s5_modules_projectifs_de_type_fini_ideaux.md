---
book: ac
book_title: Commutative Algebra
chapter: II
chapter_title: Localisation
section: 5
section_title: Modules projectifs de type fini. Idéaux fractionnaires inversibles
lang: fr
source: ac-i-iv-fr
pdf_pages: 0134-0149, 0174-0180
extraction: ocr
subsections:
    - "no": 1
      title: Localisation par rapport à un élément.
      page: 0
      pdf_page: 134
    - "no": 2
      title: Caractérisation locale des modules projectifs de type fini.
      page: 0
      pdf_page: 136
    - "no": 3
      title: Rangs des modules projectifs.
      page: 0
      pdf_page: 139
    - "no": 4
      title: Modules projectifs de rang 1.
      page: 0
      pdf_page: 141
    - "no": 5
      title: Sous-modules non dégénérés.
      page: 0
      pdf_page: 144
    - "no": 6
      title: Sous-modules inversibles.
      page: 0
      pdf_page: 145
    - "no": 7
      title: Le groupe des classes de modules inversibles.
      page: 0
      pdf_page: 148
statements: 33
exercises: 25
content_sha256: 0ff523e5d5f2c323ee054e42091efca38799fd9de2cd23436a9d309c54b3aa61
---

## § 5. Modules projectifs de type fini Idéaux fractionnaires inversibles

### 1. Localisation par rapport à un élément.

Soient $A$ un anneau, $M$ un $A$-module. Pour tout élément $f \in A$, nous poserons $A_f = A[f^{-1}]$, $M_f = M[f^{-1}] = M \otimes_A A[f^{-1}]$ ($\S$ 2, nos 1 et 2); si $S_f$ est l’ensemble des $f^n$ pour $n \geqslant 0$, on a donc $A_f = S_f^{-1}A$, $M_f = S_f^{-1}M$. Si $f$ est inversible dans $A$, $A_f$ (resp. $M_f$) s’identifie canoniquement à $A$ (resp. à $M$); si $f$ est nilpotent, on a $A_f = 0$ et $M_f = 0$. Pour tout homomorphisme $u : M \to N$ de $A$-modules, on écrira $u_f = u \otimes 1 : M_f \to N_f$.

Soit $g$ un second élément de $A$; $A_{fg}$ (resp. $M_{fg}$) s’identifie canoniquement à $(A_f)_{g/1}$ (resp. $(M_f)_{g/1}$), où $g/1$ est l’image de $g$ dans $A_f$, et $u_{fg}$ à $(u_f)_{g/1}$ ($\S$ 2, no 3, prop. 7).

#### Proposition 1 {#ac-ii-s5-prop-1 .statement}

Soit $f$ un élément d’un anneau $A$, et soit $\varphi : A \to A_f$ l’application canonique. L’application $^a\varphi : \mathrm{Spec}(A_f) \to \mathrm{Spec}(A)$ est un homéomorphisme de $\mathrm{Spec}(A_f)$ sur le sous-espace ouvert $X_f$ de $X = \mathrm{Spec}(A)$ ($\S$ 4, no 3).

C’est un cas particulier du $\S$ 4, no 3, cor. de la prop. 13.

#### Proposition 2 {#ac-ii-s5-prop-2 .statement}

Soient $A$ un anneau, $u : M \to N$ un homomorphisme de $A$-modules, et $p$ un idéal premier de $A$.

(i) Supposons que $u_p : M_p \to N_p$ soit surjectif et que $N$ soit de type fini. Il existe alors $f \in A - p$ tel que $u_f : M_f \to N_f$ soit surjectif.

(ii) Supposons que $u_p$ soit bijectif, que $M$ soit de type fini et $N$ de présentation finie. Il existe alors $f \in A - p$ tel que $u_f$ soit bijectif.

Soient R et Q le noyau et le conoyau de u ; si g ∈ A, le noyau et le conoyau de u_g (resp. u_p) sont R_g et Q_g (resp. R_p et Q_p) (§ 2, n° 4, th. 1). On a donc Q_p = 0 ; comme N est de type fini, il en est de même de Q, de sorte qu’il existe g' ∈ A - p tel que g'Q = 0 (§ 2, n° 2, cor. 2 de la prop. 4), d’où Q_{g'} = 0. Sous les hypothèses de (ii), la suite 0 → R_{g'} → M_{g'} → N_{g'} → 0 est exacte, donc R_{g'} est de type fini (chap. I, § 2, n° 8, lemme 9). Or, on a (R_{g'})_{p_{R_{g'}}} = R_p = 0 ; donc il existe g_1 ∈ A_{g'} - pA_{g'} tel que g_1R_{g'} = 0 (§ 2, n° 2, cor. 2 de la prop. 4). On a g_1 = g''/g'^h, où g'' ∈ A - p ; comme g'/1 est inversible dans R_{g'}, on a (g''/1)R_{g'} = 0 d’où R_{g'g''} = (R_{g'})_{g''}/1 = 0. Si f = g'g'', on a f ∈ A - p, Q_f = 0 et R_f = 0, de sorte que u_f est bijectif.

#### Corollaire {#ac-ii-s5-n1-cor-1 .statement}

Si N est de présentation finie et si N_p est un A_p-module libre de rang p, il existe f ∈ A - p tel que N_f soit un A_f-module libre de rang p.

Il existe par hypothèse p éléments x_i ∈ N (1 ≤ i ≤ p) tels que les x_i/1 forment une base du A_p-module libre N_p. Considérons l’homomorphisme u : A^p → N tel que u(e_i) = x_i pour 1 ≤ i ≤ p, (e_i)_{1 ≤ i ≤ p} étant la base canonique de A^p. Comme u_p est bijectif par hypothèse, il existe f ∈ A - p tel que u_f soit bijectif, en vertu de la prop. 2.

#### Proposition 3 {#ac-ii-s5-prop-3 .statement}

Soit (f_i)_{i ∈ I} une famille finie d’éléments d’un anneau A, engendrant l’idéal A de A. L’anneau B = $\prod_{i ∈ I} A_{f_i}$ est alors un A-module fidèlement plat.

En vertu du § 2, n° 4, th. 1, chacun des A_{f_i} est un A-module plat, donc il en est de même de B (chap. I, § 2, n° 3, prop. 2). D’autre part, si p est un idéal premier de A, il existe un indice i tel que f_i ∉ p et p_{f_i} = pA_{f_i} est donc un idéal premier de A_{f_i}. On a alors pB ⊂ pA_{f_i} × $\prod_{j ≠ i} A_{f_j}$ ≠ B puisque pA_{f_i} ≠ A_{f_i} ; ceci suffit à entraîner que B est un A-module fidèlement plat (chap. I, § 3, n° 1, prop. 1).

#### Corollaire {#ac-ii-s5-n1-cor-2 .statement}

Sous les hypothèses de la prop. 3, pour qu’un A-module M soit de type fini (resp. de présentation finie), il faut et il suffit que, pour tout indice $i$, le $A_{f_i}$-module $M_{f_i}$ soit de type fini (resp. de présentation finie).

La condition est évidemment nécessaire ($\S 2$, no 4). Inversement, si tous les $M_{f_i}$ sont de type fini (resp. de présentation finie), $M' = \prod_{i \in I} M_{f_i}$ est un B-module de type fini (resp. de présentation finie, car on peut évidemment supposer que pour chaque $i$ il y a une suite exacte $A_{f_i}^m \to A_{f_i}^n \to M_{f_i} \to 0$, où $m$ et $n$ sont indépendants de $i$). Or, on a $M' = M \otimes_A B$. Le corollaire résulte alors de la prop. 3 et du chap. I, $\S 3$, no 6, prop. 11.

On notera que la condition sur les $f_i$ signifie que les ensembles ouverts $X_{f_i}$ forment un recouvrement de $\mathrm{Spec}(A)$ ($\S 4$, no 3, cor. 3 de la prop. 11).

### 2. Caractérisation locale des modules projectifs de type fini.

#### Théorème 1 {#ac-ii-s5-thm-1 .statement}

Soient $A$ un anneau, $P$ un $A$-module. Les propriétés suivantes sont équivalentes :
a) $P$ est un module projectif de type fini.
b) $P$ est un module de présentation finie, et pour tout idéal maximal $m$ de $A$, $P_m$ est un $A_m$-module libre.
c) $P$ est un module de type fini, pour tout $p \in \mathrm{Spec}(A)$, le $A_p$-module $P_p$ est libre, et si on désigne son rang par $r_p$, la fonction $p \to r_p$ est localement constante dans l’espace topologique $\mathrm{Spec}(A)$ (c’est-à-dire que tout point de $\mathrm{Spec}(A)$ admet un voisinage dans lequel cette fonction est constante).
d) Il existe une famille finie $(f_i)_{i \in I}$ d’éléments de $A$ engendrant l’idéal $A$, telle que, pour tout $i \in I$, le $A_{f_i}$-module $P_{f_i}$ soit libre de rang fini.
e) Pour tout idéal maximal $m$ de $A$, il existe $f \in A - m$ tel que $P_f$ soit un $A_f$-module libre de rang fini.

Nous démontrerons le théorème suivant le schéma logique

$$
\begin{array}{ccc}
a) & \Leftarrow & d) \\
\downarrow & & \uparrow \\
b) & \Rightarrow & e)
\end{array}
$$

$a) \Rightarrow b)$: On sait qu’un module projectif de type fini est de présentation finie (chap. I, $\S 2$, no 8, lemme 8, (iii)) ; si $P$ est un $A$-module projectif, $P_m = P \otimes_A A_m$ est un $A_m$-module projectif ($Alg.$, chap. II, 3e éd., § 5, no 1, cor. de la prop. 4); enfin, comme $A_m$ est un anneau local, tout $A_m$-module projectif de présentation finie est libre ($§ 3$, no 2, cor. 2 de la prop. 5).

$b) \Rightarrow e)$: Cela résulte du corollaire de la prop. 2 du no 1.

$c) \Rightarrow e)$: Soit $m$ un idéal maximal de $A$; posons $r_m = n$, et soit $(x_i)_1 \leq i \leq n$ une base de $P_m$. Quitte à multiplier les $x_i$ par un élément inversible de $A_m$, on peut supposer que les $x_i$ sont images canoniques d’éléments $p_i \in P$ ($1 \leq i \leq n$). Soit $(e_i)_1 \leq i \leq n$ la base canonique de $A^n$ et soit $u : A^n \to P$ l’homomorphisme tel que $u(e_i) = p_i$ pour $1 \leq i \leq n$. Comme $P$ est de type fini, il résulte de la prop. 2 du no 1 qu’il existe $f \in A - m$ tel que $u_f$ soit surjectif. On en conclut que $u_{f g}$ est aussi surjectif pour tout $g \in A - m$, et par hypothèse il existe $g \in A - m$ tel que $r_p = n$ pour $p \in X_g$. On peut donc, en remplaçant $f$ par $f g$, supposer que $r_p = n$ pour tout $p \in X_f$. Alors $u_p : A_p^n \to P_p$ est un homomorphisme surjectif et $P_p$ et $A_p$ sont deux $A_p$-modules libres de même rang; donc ($§ 3$, no 2, cor. de la prop. 6) $u_p$ est bijectif pour tout $p \in X_f$. Soit $p'$ un idéal premier de $A_f$, et soit $p$ son image réciproque dans $A$ par l’application canonique ; si on identifie $(A_f^n)_{p'}$ et $(P_f)_{p'}$ à $A_p^n$ et $P_p$ par les isomorphismes canoniques, $(u_f)_{p'}$ s’identifie à $u_p$ et est par suite bijectif. On en conclut que $u_f$ est bijectif ($§ 3$, no 3, th. 1), ce qui établit e).

$e) \Rightarrow d)$: Soit $E$ l’ensemble des $f \in A$ tels que $P_f$ soit un $A_f$-module libre de type fini. L’hypothèse entraîne que $E$ n’est contenu dans aucun idéal maximal de $A$, donc $E$ engendre l’idéal $A$, et il existe par suite une famille finie $(f_i)_1 \leq i \leq n$ d’éléments de $E$ et des $a_i \in A$ ($1 \leq i \leq n$) tels que $1 = \sum_{i=1}^n a_i f_i$; d’où d).

$d) \Rightarrow c)$: Il résulte du no 1, cor. de la prop. 3, que $P$ est de type fini. D’autre part, pour tout idéal premier $p$ de $A$, il existe un indice $i$ tel que $p \in X_{f_i}$; si $p' = p_{f_i}$, on a $P_p = (P_{f_i})_{p'}$ ($§ 2$, no 5, prop. 10), donc par hypothèse $P_p$ est libre de même rang que $P_{f_i}$, ce qui prouve c).

$d) \Rightarrow a)$: Considérons l’anneau $B = \prod_{i \in I} A_{f_i}$ et le $B$-module $M = \prod_{i \in I} P_{f_i} = P \otimes_A B$. Pour chaque indice $i$, il y a un $A_{f_i}$-module libre $L_i$ tel que $P_{f_i}$ soit facteur direct de $L_i$, et on peut supposer que les $L_i$ ont tous même rang ; donc $L = \prod_{i \in I} L_i$ est un B-module libre, dont M est facteur direct, autrement dit M est un B-module projectif de type fini. Comme B est un A-module fidèlement plat (no 1, prop. 3), on en conclut que P est un A-module projectif de type fini (chap. I, § 3, no 6, prop. 12).

#### Corollaire 1 {#ac-ii-s5-thm-1-cor-1 .statement}

Supposons vérifiées les propriétés équivalentes de l’énoncé du th. 1. Soit m un entier $> 0$ tel que, pour toute famille $(x_i)_{1 \leq i \leq m}$ d’éléments de P, il existe une famille $(a_i)_{1 \leq i \leq m}$ d’éléments de A, non tous diviseurs de zéro, et pour lesquels $\sum_{i=1}^m a_i x_i = 0$. Alors, pour tout $p \in \mathrm{Spec}\,(A)$, on a $r_p \leq m$.

En effet, soit $p$ un idéal premier de A ; posons $r = r_p$ et soit $(y_j)_{1 \leq j \leq r}$ une base du $A_p$-module libre $P_p$. Il existe des éléments $x_j$ ($1 \leq j \leq r$) de P et un $s \in A - p$ tels que $y_j = x_j / s$ pour tout $j$. Pour toute famille $(a_j)_{1 \leq j \leq r}$ d’éléments de A tels que $\sum_{j=1}^r a_j x_j = 0$, on a alors $\sum_{j=1}^r (a_j / 1) y_j = 0$ dans $P_p$, d’où $a_j / 1 = 0$ pour $1 \leq j \leq r$. Comme $A - p$ ne contient pas 0, cela montre que les $a_j$ sont tous diviseurs de zéro dans A ($\S 2$, no 1, Remarque 3), donc on a nécessairement $r \leq m$.

#### Corollaire 2 {#ac-ii-s5-thm-1-cor-2 .statement}

Tout module plat de présentation finie est projectif.

En effet, si P est un A-module plat de présentation finie, et m un idéal maximal de A, le $A_m$-module $P_m$ est plat ($\S 3$, no 4, prop. 13) et de présentation finie ($\S 2$, no 4), donc libre ($\S 3$, no 2, cor. 2 de la prop. 5). La condition b) du th. 1 est donc vérifiée.

#### Remarque 1 {#ac-ii-s5-n2-rem-1 .statement}

Il existe des modules plats de type fini qui ne sont pas projectifs (exerc. 7).
2) Le cor. 2 du th. 1 s’étend aux modules sur un anneau non commutatif (chap. I, § 2, exerc. 15).

### 3. Rangs des modules projectifs.

#### Définition 1 {#ac-ii-s5-def-1 .statement}

Soit P un A-module projectif de type fini. Pour tout idéal premier $p$ de A, le rang du $A_p$-module libre $P_p$ s'appelle le rang de P en $p$ et se note $\mathrm{rg}_p(P)$.

En vertu du th. 1, la fonction $p \to \mathrm{rg}_p(P)$ à valeurs entières est localement constante dans $X = \mathrm{Spec}(A)$; elle est par suite constante si X est connexe, et en particulier lorsque l'anneau A est intègre ($\S 4$, no 3, cor. 2 de la prop. 15).

#### Définition 2 {#ac-ii-s5-def-2 .statement}

Soit n un entier $\geqslant 0$. On dit qu'un A-module projectif P est de rang n s'il est de type fini et si $\mathrm{rg}_p(P) = n$ pour tout idéal premier $p$ de A.

Il est clair que tout A-module libre de type fini L est de rang n au sens de la définition 2, n étant égal à la dimension (ou rang) de L définie en Alg., chap. II, 3e éd., § 7, no 2.

Un module projectif de rang 0 est nul ($\S 3$, no 3, cor. 2 du th. 1). Si A n'est pas réduit à 0 et si un A-module projectif P est de rang n, l'entier n est déterminé de façon unique ; on le note alors $\mathrm{rg}(P)$.

#### Théorème 2 {#ac-ii-s5-thm-2 .statement}

Soient P un A-module et n un entier $\geqslant 0$. Les propriétés suivantes sont équivalentes :
a) P est projectif de rang n.
b) P est de type fini et, pour tout idéal maximal m de A, le $A_m$-module $P_m$ est libre de rang n.
c) P est de type fini et, pour tout idéal premier $p$ de A, le $A_p$-module $P_p$ est libre de rang n.
d) Pour tout idéal maximal m de A, il existe $f \in A - m$ tel que le $A_f$-module $P_f$ soit libre de rang n.

En vertu de la déf. 2 et du th. 1, a) et c) sont équivalentes ; b) implique c), car pour tout idéal premier $p$ de A, il existe un idéal maximal m contenant $p$, et si on pose $p' = p_m$, $P_p$ est isomorphe à $(P_m)_{p'}$ ($\S 2$, no 5, prop. 11) ; si $P_m$ est libre de rang n, il en est donc de même de $P_p$. La propriété c) implique d) en vertu du th. 1 et du fait que, si $f \in A - m$ et si $m' = m_f$, $P_m$ est isomorphe à $(P_f)_{m'}$, donc les rangs de $P_f$ et $P_m$ sont égaux. Enfin ce dernier raisonnement et le th. 1 montrent que d) implique b).

#### Remarque {#ac-ii-s5-n3-rem-1 .statement}

Si $A$ est un anneau intègre, un $A$-module projectif admet un rang bien défini (au sens de la déf. 2), comme on l’a observé plus haut ; en outre ce rang coïncide avec le rang défini en Alg., chap. II, 3e éd., § 7, no 2 ; il suffit en effet d’appliquer le th. 2 c) avec $p = (0)$.

Soient $E$ et $F$ deux $A$-modules projectifs de type fini. On sait (Alg., chap. II, 3e éd., §§ 2 et 3) que $E \times F, E \otimes_A F, \operatorname{Hom}_A(E, F)$ et le dual $E^*$ de $E$ sont projectifs de type fini ; il en est de même de la puissance extérieure $\wedge^k E$ pour tout entier $k > 0$ (Alg., chap. III, 3e éd.). De plus, on déduit immédiatement de la déf. 1 et du § 2, no 7, prop. 18 et 19, et no 8, que, pour tout idéal premier $p$ de $A$, on a :

(1) $\operatorname{rg}_p(E \times F) = \operatorname{rg}_p(E) + \operatorname{rg}_p(F)$
(2) $\operatorname{rg}_p(E \otimes_A F) = \operatorname{rg}_p(E) \cdot \operatorname{rg}_p(F)$
(3) $\operatorname{rg}_p(\operatorname{Hom}_A(E, F)) = \operatorname{rg}_p(E) \cdot \operatorname{rg}_p(F)$
(4) $\operatorname{rg}_p(E^*) = \operatorname{rg}_p(E)$
(5) $\operatorname{rg}_p(\wedge^k E) = \binom{\operatorname{rg}_p(E)}{k}$.

Lorsque les rangs de $E$ et de $F$ sont définis, il en est de même de ceux de $E \times F, E \otimes_A F, \operatorname{Hom}_A(E, F), E^*$ et $\wedge^k E$, et les formules ci-dessus sont encore valables en omettant l’indice $p$. En outre :

#### Corollaire {#ac-ii-s5-n3-cor-1 .statement}

Pour qu’un $A$-module projectif de type fini $P$ soit de rang $n$, il faut et il suffit que $\wedge^n P$ soit de rang 1.

#### Proposition 4 {#ac-ii-s5-prop-4 .statement}

Soient $B$ une $A$-algèbre commutative, $P$ un $A$-module projectif de rang $n$. Le $B$-module $P_{(B)} = B \otimes_A P$ est alors projectif de rang $n$.

On sait que $P_{(B)}$ est projectif de type fini (Alg., chap. II, 3e éd., § 5, no 1, cor. de la prop. 4). Si $q$ est un idéal premier de $B$ et $p$ son image réciproque dans $A$, on a $(P_{(B)})_q = (P \otimes_A B) \otimes_B B_q = P \otimes_A B_q =$

(P \otimes_A A_p) \otimes_{A_p} B_q, et comme, par hypothèse, P \otimes_A A_p est un A_p-module libre de rang n, (P_{(B)})_q est un B_q-module libre de rang n.

#### Proposition 5 {#ac-ii-s5-prop-5 .statement}

Soient A un anneau semi-local, P un A-module projectif de type fini. Si le rang de P est défini, P est un A-module libre.

Supposons d’abord que A soit isomorphe à un produit de corps K_i (1 \leq i \leq n). Les K_i s’identifient alors aux idéaux minimaux (Alg., chap. VIII, § 3, n° 1) de A, et, pour tout i, la somme p_i des K_j d’indice j \neq i est un idéal maximal de A, les p_i (1 \leq i \leq n) étant les seuls idéaux premiers de A. Tout A-module P de type fini est alors somme directe de ses composants isotypiques P_i (1 \leq i \leq n), P_i étant isomorphe à une somme directe d’un nombre fini r_i de A-modules isomorphes à K_i (Alg., chap. VIII, § 5, n° 1, prop. 1 et n° 3, prop. 11); l’anneau A_{p_i} s’identifie à K_i et annule les P_j d’indice j \neq i, donc r_i = \mathrm{rg}_{p_i}(P); si tous les r_i sont égaux à un même nombre r, P est isomorphe à A^r, d’où la proposition dans ce cas. Dans le cas général, soient R le radical de A, et B = A/R; comme B est un produit de corps, le B-module projectif P_{(B)} est libre d’après ce qui précède et la prop. 4. Par ailleurs P est un A-module plat, et la proposition résulte donc du § 3, n° 2, prop. 5.

### 4. Modules projectifs de rang 1.

#### Théorème 3 {#ac-ii-s5-thm-3 .statement}

Soient A un anneau, M un A-module de type fini.

(i) S’il existe un A-module N tel que M \otimes_A N soit isomorphe à A, le module M est projectif de rang 1.

(ii) Réciproquement, si M est projectif de rang 1 et si M^* est le dual de M, l’homomorphisme canonique u : M \otimes_A M^* \to A correspondant à la forme bilinéaire canonique (x, x^*) \to \langle x, x^* \rangle sur M \times M^* (Alg., chap. II, 3e éd., § 2, n° 3) est bijectif.

(i) Il s’agit de prouver que, pour tout idéal maximal m de A, le A_m-module M_m est libre de rang 1 (th. 2 b)); quitte à remplacer A par A_m, on peut donc supposer que A est un anneau local (\S 2, n° 7, prop. 18). Soit k = A/m. L’isomorphisme \varphi : M \otimes_A N \to A définit un isomorphisme \varphi \otimes 1_k : (M/mM) \otimes_k (N/mN) \to k : comme le rang sur $k$ de $(M/mM) \otimes_k (N/mN)$ est le produit des rangs de $M/mM$ et $N/mN$, ces derniers sont nécessairement égaux à 1, autrement dit $M/mM$ est monogène. On en conclut que $M$ est monogène ($\S 3$, no 2, cor. 2 de la prop. 4); d'autre part, l'annulateur de $M$ annule aussi $M \otimes_A N$, donc est nul, ce qui prouve que $M$ est isomorphe à $A$.

(ii) Il suffit de prouver que, pour tout idéal maximal $m$ de $A$, $u_m$ est un isomorphisme ($\S 3$, no 3, th. 1). Comme $M$ est de présentation finie (chap. I, $\S 2$, no 8, lemme 8) $(M^*)_m$ s'identifie canoniquement au dual $(M_m)^*$ ($\S 2$, no 7, prop. 19) et comme $M_m$ est libre de rang 1 ainsi que son dual $(M_m)^*$, il est clair que l'homomorphisme canonique $u_m : (M_m) \otimes_{A_m} (M_m)^* \to A_m$ est bijectif, ce qui achève la démonstration.

Remarque 1). — Si $M$ est projectif de rang 1 et si $N$ est tel que $M \otimes_A N$ soit isomorphe à $A$, alors $N$ est isomorphe à $M^*$: en effet, on a des isomorphismes

$$
N \to N \otimes A \to N \otimes M \otimes M^* \to A \otimes M^* \to M^*.
$$

#### Proposition 6 {#ac-ii-s5-prop-6 .statement}

Soient $M$ et $N$ des $A$-modules projectifs de rang 1. Alors $M \otimes_A N$, $\mathrm{Hom}_A(M, N)$ et le dual $M^*$ de $M$ sont projectifs de rang 1.

Cela résulte aussitôt des formules (2), (3) et (4).

Notons maintenant que tout $A$-module de type fini est isomorphe à un module quotient de $L = A^{(\mathbf{N})}$; on peut donc parler de l'ensemble $F(A)$ des classes de $A$-modules de type fini pour la relation d'isomorphie (Ens., chap. I, 2e éd., $\S 6$, no 9); nous désignons par $P(A)$ la partie de $F(A)$ formée des classes de $A$-modules projectifs de rang 1, et par $\mathrm{cl}(M)$ l'image dans $P(A)$ d'un $A$-module projectif $M$ de rang 1. Il est immédiat que, pour deux $A$-modules projectifs $M, N$ de rang 1, $\mathrm{cl}(M \otimes_A N)$ ne dépend que de $\mathrm{cl}(M)$ et de $\mathrm{cl}(N)$; on pose par définition

$$
\mathrm{cl}(M) + \mathrm{cl}(N) = \mathrm{cl}(M \otimes_A N)
$$

et on définit ainsi une loi de composition interne dans $P(A)$.

#### Proposition 7 {#ac-ii-s5-prop-7 .statement}

L’ensemble $P(A)$ des classes de $A$-modules projectifs de rang 1, muni de la loi de composition (6), est un groupe commutatif. Si $M$ est un $A$-module projectif de rang 1 et $M^*$ son dual, on a

$$
\mathrm{cl}(M^*) = - \mathrm{cl}(M) \quad \text{et} \quad \mathrm{cl}(A) = 0.
$$

L’associativité et la commutativité du produit tensoriel montrent que la loi de composition (6) est associative et commutative ; l’isomorphie de $A \otimes_A M$ et de $M$ prouve que $\mathrm{cl}(A)$ est élément neutre pour cette loi, et on a, en vertu du th. 3, $\mathrm{cl}(M) + \mathrm{cl}(M^*) = \mathrm{cl}(A)$, d’où la proposition.

Soient $B$ une $A$-algèbre commutative, $M$ un $A$-module projectif de rang 1 ; alors $M_{(B)} = B \otimes_A M$ est un $B$-module projectif de rang 1 (n° 3, prop. 4). Il existe donc une application dite canonique $\varphi : P(A) \to P(B)$ telle que

$$
\varphi(\mathrm{cl}(M)) = \mathrm{cl}(M_{(B)}).
$$

La formule $M_{(B)} \otimes_B N_{(B)} = (M \otimes_A N)_{(B)}$ pour deux $A$-modules $M, N$ prouve que l’application $\varphi$ est un homomorphisme de groupes commutatifs.

*Remarque 2). — La condition e) du th. 1 (équivalente au fait que $P$ est projectif de type fini) peut aussi s’exprimer en disant que le faisceau de modules $\tilde{P}$ sur $X = \mathrm{Spec}(A)$ associé (*) à $P$ est localement libre de type fini, et peut par suite s’interpréter comme le faisceau des sections d’un fibré vectoriel sur $X$. Inversement, tout fibré vectoriel sur $X$ provient d’un module projectif de type fini, déterminé à un isomorphisme unique près ; les modules projectifs de rang $n$ correspondent ainsi aux fibrés vectoriels dont toutes les fibres ont la dimension $n$. En particulier, les fibrés vectoriels de rang 1 correspondent aux modules projectifs de rang 1. Si l’on note $\mathcal{O}_X$ le faisceau structural $\tilde{A}$, et $\mathcal{O}_X^*$ le faisceau des unités de $\mathcal{O}_X$ (dont les sections sur un ouvert $U$ de $X$ sont les éléments inversibles de l’anneau des sections de $\mathcal{O}_X$ sur $U$), on en déduit que le

(*) Voir A. Grothendieck, Éléments de géométrie algébrique, I (§1) (Publ Math. I. H. E. S., n° 4, 1960).

groupe $P(A)$ est isomorphe au premier groupe de cohomologie $H^1(X, \mathcal{O}_X^*)$.*

### 5. Sous-modules non dégénérés.

Dans ce no et les deux suivants, on note $A$ un anneau, $S$ une partie multiplicative de $A$ formée d’éléments non diviseurs de zéro dans $A$, et $B$ l’anneau $S^{-1}A$; on identifie canoniquement $A$ à un sous-anneau de $B$ ($\S 2$, no 1, Remarque 3). Les éléments de $S$ sont alors inversibles dans $B$.

L’un des cas particuliers les plus importants pour les applications est celui où $A$ est intègre et $S$ l’ensemble des éléments $\neq 0$ de $A$; $B$ est alors le corps des fractions de $A$.

#### Définition 3 {#ac-ii-s5-def-3 .statement}

Soit $M$ un sous-A-module de $B$. On dit que $M$ est non dégénéré si $B.M = B$.

Lorsque $B$ est un corps, cette condition signifie simplement que $M$ n’est pas réduit à 0.

#### Proposition 8 {#ac-ii-s5-prop-8 .statement}

Soit $M$ un sous-A-module de $B$. Les conditions suivantes sont équivalentes :
a) $M$ est non dégénéré.
b) $M$ rencontre $S$.
c) Si $j : M \to B$ est l’injection canonique, l’homomorphisme $u = S^{-1}j : S^{-1}M \to B$ est bijectif.
   a) implique b), car si $B.M = B$, il existe $a \in A, s \in S$ et $x \in M$ tels que $(a/s)x = 1$, donc $ax = s$ appartient à $S \cap M$. Pour voir que b) implique c), remarquons déjà que $u$ est injectif ($\S 2$, no 4, th. 1) ; en outre si $x \in M \cap S$, l’image par $u$ de $x/x \in S^{-1}M$ dans $B$ est égale à 1, et $u$ est donc surjectif. Enfin, il est clair que c) entraîne a).

#### Corollaire {#ac-ii-s5-n5-cor-1 .statement}

Si $M$ et $N$ sont deux sous-A-modules non dégénérés de $B$, les A-modules $M + N, M.N$ et $M \cap N$ sont non dégénérés.
   L’assertion est triviale pour $M + N$; d’autre part, si $s \in S \cap M$ et $t \in S \cap N$, on a $st \in S \cap (M.N)$ et $st \in S \cap (M \cap N)$.

Étant donnés deux sous-A-modules M et N de B, désignons par N : M le sous-A-module de B formé des $b \in B$ tels que $bM \subset N$ (chap. I, § 2, no 10, Remarque). Si l’on fait correspondre à tout $b \in N : M$ l’homomorphisme $h_b : x \to bx$ de M dans N, on obtient un homomorphisme canonique $b \to h_b$ de N : M dans $\mathrm{Hom}_A(M, N)$.

#### Proposition 9 {#ac-ii-s5-prop-9 .statement}

Soient M, N deux sous-A-modules de B. Si M est non dégénéré, l’homomorphisme canonique de N : M dans $\mathrm{Hom}_A(M, N)$ est bijectif.

Soit $s \in S \cap M$. Si $b \in N : M$ est tel que $bx = 0$ pour tout $x \in M$, on a $bs = 0$, d’où $b = 0$ puisque s est non diviseur de 0 dans B. D’autre part, soit $f \in \mathrm{Hom}_A(M, N)$ et posons $b = f(s)/s$; pour tout $x \in M$, il existe $t \in S$ tel que $tx \in A$. On a donc

$$
f(x) = s^{-1}t^{-1}f(stx) = s^{-1}t^{-1}txf(s) = bx,
$$

d’où $b \in N : M$ et $f = h_b$, ce qui démontre la proposition.

#### Remarque {#ac-ii-s5-n5-rem-1 .statement}

En particulier, $A : M$ s’identifie canoniquement au dual $M^*$ de M, la forme bilinéaire canonique sur $M \times M^*$ s’identifiant à la restriction à $M \times (A : M)$ de la multiplication $B \times B \to B$.

### 6. Sous-modules inversibles.

(On conserve les notations du no 5.)

#### Définition 4 {#ac-ii-s5-def-4 .statement}

On dit qu’un sous-A-module M de B est inversible s’il existe un sous-A-module N de B tel que $M.N = A$.

Exemple : Si b est un élément inversible de B, le A-module Ab est inversible, comme on le voit en prenant $N = Ab^{-1}$.

#### Proposition 10 {#ac-ii-s5-prop-10 .statement}

Soit M un sous-A-module inversible de B. Alors :

(i) Il existe $s \in S$ tel que $As \subset M \subset As^{-1}$ (et en particulier M est non dégénéré).

(ii) $A : M$ est le seul sous-A-module N de B tel que $M.N = A$.
Si $M.N = A$, on a $B.M = B.(B.M) \supset B.(M.N) = B.A = B,$ donc M est non dégénéré. De même, N est non dégénéré. Si $t \in S \cap M$ et $u \in S \cap N$ (no 5, prop. 8), l’élément $s = tu$ appartient à $S \cap M \cap N$, d’où $Ms \subset M.N = A$, et par suite $As \subset M \subset As^{-1}$.

D’autre part, on a évidemment $N \subset A : M$, d’où

$$
A = M.N \subset M.(A : M) \subset A
$$

et $M.(A : M) = A$; multipliant les deux membres par $N$, on en déduit $A : M = N$, ce qui achève la démonstration.

**Théorème 4. — Soit M un sous-A-module non dégénéré de B. Les propriétés suivantes sont équivalentes :**

a) M est inversible.
b) M est projectif.
c) M est projectif de rang 1.
d) M est un A-module de type fini et, pour tout idéal maximal m de A, le $A_m$-module $M_m$ est monogène.

Montrons d’abord l’équivalence des propriétés a), b) et c). Si a) est vérifiée et si N est un sous-A-module de B tel que $M.N = A$, on a une relation

$$
\sum_{i=1}^p m_i n_i = 1 \quad (m_i \in M,\ n_i \in N \text{ pour tout } i).
$$

Pour tout $x \in M$, posons $\nu_i(x) = n_i x$; les $\nu_i$ sont des formes linéaires sur M et on a, en vertu de (9), $x = \sum_{i=1}^n m_i \nu_i(x)$ pour tout $x \in M$; cela prouve (Alg., chap. II, 3e éd., § 2, no 6, prop. 12) que M est projectif et engendré par les $m_i$; donc M est un module projectif de type fini.

Soit $m$ un idéal maximal de A; montrons que l’entier $r = \mathrm{rg}_m(M)$ est égal à 1. Soit S’ l’image de S dans $A_m$; comme les éléments de S sont non diviseurs de 0 dans A, ceux de S’ sont non diviseurs de 0 dans $A_m$, puisque $A_m$ est un A-module plat ($\S 2$, no 4, th. 1 et chap. I, § 2, no 4, prop. 3); on a donc $S'{}^{-1}A_m \neq 0$, et comme $M_m$ est un $A_m$-module libre de rang $r$, $S'{}^{-1}M_m$ est un $S'{}^{-1}A_m$-module libre de rang $r$. Mais si T’ est l’image de $A - m$ dans $S^{-1}A$, $S'{}^{-1}A_m$ (resp. $S'{}^{-1}M_m$) s’identifie canoniquement à $T'{}^{-1}(S^{-1}A)$ (resp. $T'{}^{-1}(S^{-1}M)$) ($\S 2$, no 3, prop. 7). Or $S^{-1}M = B$ (prop. 8 c)), donc T'−1(S−1M) est un module libre de rang 1 sur T'−1(S−1A), ce qui prouve que r = 1 et démontre l’implication a) ⇒ c).

L’implication c) ⇒ b) est triviale. Montrons que b) ⇒ a). Il existe par hypothèse une famille (non nécessairement finie) (fλ)λ∈L de formes linéaires sur M et une famille (mλ)λ∈L d’éléments de M tels que, pour tout x ∈ M, la famille (fλ(x)) ait un support fini et que l’on ait x = Σ λ mλfλ(x) (Alg., chap. II, 3e éd., § 2, n° 6, prop. 12).
Puisque M est non dégénéré, on a fλ(x) = nλx pour un nλ ∈ A : M en vertu de la prop. 9 du n° 5. Prenant pour x un élément de M ∩ S (n° 5, prop. 8), on voit qu’on a nécessairement nλ = 0 sauf pour un nombre fini d’indices, et Σ λ mλnλ = 1. Cela entraîne évidemment M.(A : M) = A, d’où a).

En vertu de la déf. 2 du n° 3, c) entraîne d). Démontrons la réciproque. Comme M est non dégénéré, son annulateur est nul, (prop. 8 b)), donc il en est de même de l’annulateur de Mm (§ 2, n° 4, formule (9)). Comme on suppose que Mm est un Am-module monogène, il est donc libre de rang 1 et il résulte alors du n° 3, th. 2, que M est projectif de rang 1.

#### Corollaire {#ac-ii-s5-n6-cor-1 .statement}

Tout sous-A-module inversible de B est plat et de présentation finie.
Cela résulte du th. 4 c).

#### Proposition 11 {#ac-ii-s5-prop-11 .statement}

Soient M, N deux sous-A-modules de B.
On suppose M inversible. Alors :
(i) L’homomorphisme canonique M ⊗A N → M.N est bijectif.
(ii) On a N : M = N.(A : M) et N = (N : M).M.
Soit j l’injection canonique N → B. Puisque M est un A-module plat (cor. du th. 4), 1 ⊗ j : M ⊗A N → M ⊗A B est injectif. Mais comme B = S−1A, le B-module M ⊗A B est égal à S−1M, donc s’identifie à B puisque M est non dégénéré (n° 5, prop. 8). Si l’on effectue cette identification, l’image de 1 ⊗ j est M.N, d’où (i).
Posons M′ = A : M. On a évidemment M′.N ⊂ N : M et M.(N : M) ⊂ N. D’autre part, puisque M.M′ = A (prop. 10), on a N : M = M′.M.(N : M) ⊂ M′.N et N = M.M′.N ⊂ M.(N : M), d’où (ii).

#### Remarque {#ac-ii-s5-n6-rem-1 .statement}

La démonstration de (i) dans la prop. 11 utilise seulement le fait que M est plat et non dégénéré.

### 7. Le groupe des classes de modules inversibles.

(On conserve les notations des nos 5 et 6.)

Pour la multiplication, les sous-A-modules de B forment un monoïde commutatif $\mathfrak{M}$, admettant A pour élément neutre. Les modules inversibles sont donc les éléments inversibles de $\mathfrak{M}$, et forment par suite un groupe commutatif $\mathfrak{J}$. On a vu (no 6, prop. 10) que l’inverse de $M \in \mathfrak{J}$ est $A : M$.

Soit $A^*$ (resp. $B^*$) le groupe multiplicatif des éléments inversibles de A (resp. B), et notons $u$ l’injection canonique $A \to B$. Pour tout $b \in B^*$, $\theta(b) = bA$ est un sous-A-module inversible. L’application $\theta : B^* \to \mathfrak{J}$ est un homomorphisme dont le noyau est $u(A^*)$; son conoyau sera noté $\mathfrak{C}$ ou $\mathfrak{C}(A)$. On dit que le groupe $\mathfrak{C}$ est le groupe des classes de sous-A-modules inversibles de B. On a par construction la suite exacte

$$
(10) \quad (1) \to A^* \xrightarrow{u} B^* \xrightarrow{\theta} \mathfrak{J} \xrightarrow{\rho} \mathfrak{C} \to (1)
$$

où (1) désigne un groupe réduit à l’élément neutre, et $\rho$ est l’application canonique $\mathfrak{J} \to \mathfrak{C} = \mathfrak{J}/\theta(B^*)$.

Comme tout sous-A-module inversible M de B est projectif de rang 1 (no 6, th. 4), l’élément $cl(M) \in P(A)$ est défini (no 4).

#### Proposition 12 {#ac-ii-s5-prop-12 .statement}

L’application $cl : \mathfrak{J} \to P(A)$ définit, par passage au quotient, un isomorphisme de $\mathfrak{C} = \mathfrak{J}/\theta(B^*)$ sur le noyau de l’homomorphisme canonique $\varphi : P(A) \to P(B)$ (no 4).

En d’autres termes, on a une suite exacte

$$
(11) \quad (1) \to A^* \xrightarrow{u} B^* \xrightarrow{\theta} \mathfrak{J} \xrightarrow{cl} P(A) \xrightarrow{\varphi} P(B).
$$

Il résulte de la prop. 11 du no 6, et de la définition de l’addition dans $P(A)$ que l’on a $cl(M.N) = cl(M) + cl(N)$ pour M, N dans $\mathfrak{J}$, ce qui montre que cl est un homomorphisme. Si $M \in \mathfrak{J}$ est isomorphe à A, il existe $b \in B$ tel que $M = Ab$, et comme M est inversible, il existe $b' \in B$ tel que $b'b = 1$, autrement dit $b$ est inversible dans B ; la réciproque est immédiate. Donc le noyau de cl dans $\mathfrak{J}$ est $\theta(B^*)$.

Déterminons maintenant l’image de cl. Si $M \in \mathfrak{J}$, on a $M \otimes_A B = S^{-1}M = B$ (n° 5, prop. 8 c)), d’où $cl(M) \in \mathrm{Ker}(\varphi)$. Réciproquement, soit P un A-module projectif de rang 1 tel que $P_{(B)} = P \otimes_A B$ soit B-isomorphe à B. Comme P est un A-module plat, l’injection $u : A \to B$ définit une injection $u \otimes 1 : P \to P_{(B)} = B$ et P se trouve ainsi identifié à un sous-A-module de B ; en vertu de la prop. 8 c) du n° 5, P est non dégénéré, et le th. 4 du n° 6 montre que P est inversible. Le noyau de $\varphi$ est donc bien égal à l’image de cl : $\mathfrak{J} \to \mathbf{P}(A)$.

#### Corollaire 1 {#ac-ii-s5-prop-12-cor-1 .statement}

Pour que deux sous-A-modules inversibles de B aient même image dans $\mathfrak{C}$, il faut et il suffit qu’ils soient isomorphes.

#### Corollaire 2 {#ac-ii-s5-prop-12-cor-2 .statement}

Si l’anneau B est semi-local, le groupe $\mathfrak{C}$ des classes de sous-A-modules inversibles de B s’identifie canoniquement au groupe $\mathbf{P}(A)$ des classes de A-modules projectifs de rang 1.

En effet, on a alors $\mathbf{P}(B) = 0$ (n° 3, prop. 5).

#### Remarque {#ac-ii-s5-n7-rem-1 .statement}

L’hypothèse du cor. 2 est remplie dans les deux cas suivants :

1) A est intègre et S est l’ensemble des éléments $\neq 0$ de A, B étant donc le corps des fractions de A. Les sous-A-modules inversibles de B sont aussi appelés dans ce cas idéaux fractionnaires inversibles ; ceux qui sont des A-modules libres monogènes $Ab$ ($b \neq 0$ dans B) ne sont autres que les idéaux principaux fractionnaires définis dans Alg., chap. VI, § 1, n° 5.

*2) L’anneau A est nœthérien et S est l’ensemble des éléments de A qui ne sont pas diviseurs de 0, de sorte que B est l’anneau total des fractions de A. En effet, on a alors $S = A - \bigcup_i p_i$, où les $p_i$ sont les éléments (en nombre fini) de Ass (A) (chap. IV, § 1), donc B est semi-local (§ 3, n° 5, prop. 17).*

## EXERCICES {#ac-ii-s5-exercises}

See the [exercises for § 5](exercises/s5/).
