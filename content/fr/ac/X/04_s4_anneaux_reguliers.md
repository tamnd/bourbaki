---
book: ac
book_title: Commutative Algebra
chapter: X
chapter_title: Profondeur, régularité, dualité
section: 4
section_title: Anneaux réguliers
lang: fr
source: ac-x-fr
pdf_pages: 0052-0060, 0161-0164
extraction: ocr
subsections:
    - "no": 1
      title: Propriétés homologiques élémentaires des anneaux locaux réguliers
      page: 0
      pdf_page: 52
    - "no": 2
      title: Caractérisation homologique des anneaux noethériens réguliers
      page: 54
      pdf_page: 53
    - "no": 3
      title: Anneaux réguliers et algèbres finies
      page: 0
      pdf_page: 56
    - "no": 4
      title: Anneaux présentables
      page: 0
      pdf_page: 57
    - "no": 5
      title: Anneaux réguliers et extensions plates
      page: 59
      pdf_page: 58
statements: 25
exercises: 13
content_sha256: 627586783da1c4cf8e8ca211c55aa5bda2405916d81ceb5d4444b3de5b2c26b9
---

## § 4. ANNEAUX RÉGULIERS

### 1. Propriétés homologiques élémentaires des anneaux locaux réguliers

#### Proposition 1 {#ac-x-s4-prop-1 .statement}

Soient $A$ un anneau local noethérien régulier et $n$ sa dimension. On a $\mathrm{dh}(A) = n$ et, pour tout entier $i \geqslant 0$,

$$
[\mathrm{Ext}_A^i(\kappa_A, \kappa_A) : \kappa_A] = [\mathrm{Tor}_i^A(\kappa_A, \kappa_A) : \kappa_A] = \binom{n}{i}.
$$

Soit $x = (x_1, \ldots, x_n)$ un système de coordonnées de $A$ (VIII, § 5, n° 1, déf. 1). La suite $x$ engendre $m_A$ et est complètement sécante pour $A$ (loc. cit., n° 2, th. 1). Le complexe de Koszul $K_\bullet(x, A)$ est une résolution libre de $\kappa_A$ (A, X, p. 159, remarque 3), dont la différentielle est nulle modulo $m_A$. Pour tout entier $i \geqslant 0$, on a donc ($§ 3$, n° 3, formule (1))

$$
[\mathrm{Ext}_A^i(\kappa_A, \kappa_A) : \kappa_A] = [\mathrm{Tor}_i^A(\kappa_A, \kappa_A) : \kappa_A] = \mathrm{rg}_A(K_i(x, A)) = \binom{n}{i}.
$$

Il résulte alors du cor. 1 de la prop. 4 du n° 3, § 3 que $\mathrm{dh}(A) = n$.

#### Proposition 2 {#ac-x-s4-prop-2 .statement}

Un anneau local noethérien régulier est factoriel.

D’après la prop. 1, tout module de type fini sur un anneau local noethérien régulier admet une résolution projective de longueur finie par des modules projectifs de type fini, donc libres (II, § 3, n° 2, cor. 2 de la prop. 5). Il résulte alors de VII, § 4, n° 7, cor. 3 de la prop. 16 qu’un tel anneau est factoriel.

#### Proposition 3 {#ac-x-s4-prop-3 .statement}

Soient $A$ un anneau local noethérien régulier et $M$ un $A$-module non nul de type fini. Sa dimension projective est finie et l’on a

$$
\mathrm{dp}_A(M) + \mathrm{prof}_A(M) = \dim(A).
$$

En effet, $M$ est de dimension projective finie (prop. 1), et l’on a $\mathrm{prof}(A) = \dim(A)$ puisque $A$ est un anneau de Macaulay ($§ 2$, n° 5, exemple 7). On applique alors le th. 1 du § 3, n° 5.

Corollaire 1. On a $\mathrm{dp}_A(M) \geqslant \dim(A) - \dim(M)$; pour qu’il y ait égalité, il faut et il suffit que $M$ soit macaulayen.

#### Corollaire 2 {#ac-x-s4-prop-3-cor-2 .statement}

Pour que le $A$-module $M$ soit libre, il faut et il suffit qu’il soit macaulayen et de dimension $\dim(A)$, ou encore qu’il soit de profondeur $\geqslant \dim(A)$.

#### Corollaire 3 {#ac-x-s4-prop-3-cor-3 .statement}

Tout module réflexif de type fini sur un anneau local noethérien régulier de dimension 2 est libre.

En effet, un anneau local noethérien régulier est intégralement clos (VIII, § 5, n° 2, cor. 1 du th. 1). Le corollaire 3 résulte donc du corollaire 2 et du § 1, n° 10, prop. 16.

#### Corollaire 4 {#ac-x-s4-prop-3-cor-4 .statement}

Soit $\rho : A \to B$ un homomorphisme local d’anneaux locaux noethériens. On suppose que $A$ est régulier et que $\rho$ fait de $B$ un $A$-module de type fini. On a alors $dp_A(B) \geq \dim(A) - \dim(B)$. Pour que $B$ soit un anneau de Macaulay, il faut et il suffit que l’on ait $dp_A(B) = \dim(A) - \dim(B)$. Pour que $B$ soit un anneau de Macaulay de dimension égale à $\dim(A)$, il faut et il suffit que le $A$-module $B$ soit libre.

En effet, on a $\dim(B) = \dim_A(B)$ (VIII, § 2, n° 3, th. 1) ; par ailleurs, $B$ est un anneau de Macaulay si et seulement si c’est un $A$-module de Macaulay (§ 2, n° 6, prop. 8). Il suffit donc d’appliquer les corollaires 1 et 2.

#### Remarque {#ac-x-s4-n1-rem-1 .statement}

Le corollaire 4 permet de caractériser les anneaux locaux de Macaulay dans plusieurs cas importants. Soit $A$ un anneau local noethérien ; c’est un anneau de Macaulay si et seulement s’il en est ainsi de $\hat{A}$ (§ 2, n° 7, cor. 4 de la prop. 9). Supposons désormais l’anneau local $A$ complet et posons $d = \dim(A)$.

a) Supposons que $A$ possède un sous-corps. Il possède alors un sous-corps de représentants $K$ (IX, § 3, n° 3), et il existe une algèbre de séries formelles $E = K[[T_1, \ldots, T_n]]$ et un homomorphisme surjectif de $K$-algèbres $E \to A$ (*loc. cit.*); il existe aussi une algèbre de séries formelles $E' = K[[T_1, \ldots, T_d]]$ et un homomorphisme local injectif de $K$-algèbres $E' \to A$ tel que $A$ soit une algèbre finie sur $E'$ (*loc. cit.*). Les propriétés suivantes sont équivalentes :

(i) $A$ est un anneau de Macaulay ;
(ii) on a $dp_E(A) = n - d$ ;
(iii) $A$ est un $E'$-module libre.

b) Supposons que le corps résiduel de $A$ soit de caractéristique $p > 0$. Il existe un $p$-anneau de longueur $+\infty$, de corps résiduel $\kappa_A$ (IX, § 2, n° 3, prop. 5). Soit $C$ un tel anneau ; il existe une algèbre de séries formelles $E = C[[T_1, \ldots, T_n]]$ et un homomorphisme surjectif $\rho : E \to A$ (IX, § 2, n° 5, th. 3). Les propriétés suivantes sont équivalentes :

(i) $A$ est un anneau de Macaulay ;
(ii) on a $dp_E(A) = n + 1 - d$.

Supposons de plus que $p1_A$ ne soit pas diviseur de zéro dans $A$ ; il existe alors une algèbre de séries formelles $E' = K[[T_1, \ldots, T_{d-1}]]$ et un homomorphisme local injectif de $K$-algèbres $E' \to A$ tel que $A$ soit une algèbre finie sur $E'$ (*loc. cit.*). L’anneau local $E'$ est régulier, de dimension $n + 1$ (VIII, § 5, n° 5, exemple 2). Les conditions précédentes équivalent aussi à

(iii) $A$ est un $E'$-module libre.

Pour des résultats analogues dans le cas des modules, voir le § 5, n° 5.

### 2. Caractérisation homologique des anneaux noethériens réguliers

#### Théorème 1 (Serre) {#ac-x-s4-thm-1 .statement}

Pour qu’un anneau local noethérien soit régulier, il faut et il suffit que sa dimension homologique soit finie.

Nous avons vu qu’un anneau local noethérien régulier est de dimension homologique finie (prop. 1).

Inversement, soit $A$ un anneau local noethérien de dimension homologique finie $n$; d’après le § 3, n° 3, cor. 2 de la prop. 4 et n° 5, th. 1, on a
$$
n = \mathrm{dh}(A) = \mathrm{dp}_A(\kappa_A) = \mathrm{prof}(A) .
$$
Si $n = 0$, le $A$-module $\kappa_A$ est libre, donc $m_A = 0$ et $A$ est un corps. Supposons $n > 0$ et raisonnons par récurrence sur $n$. Puisque $\mathrm{prof}(A) > 0$, l’idéal $m_A$ n’est pas associé à $A$ ($§ 1$, n° 1, remarque 2), donc n’est pas contenu dans la réunion de $m_A^2$ et des idéaux associés à $A$ (II, $§ 1$, n° 1, prop. 2). Par conséquent (IV, $§ 1$, n° 1, cor. 2 de la prop. 2), on peut trouver un élément $x$ de $m_A - m_A^2$ tel que l’homothétie $x_A$ soit injective. Notons $B$ l’anneau local noethérien $A/xA$ et considérons la suite de $A$-modules
$$
0 \to \kappa_A \xrightarrow{i} m_A/xm_A \xrightarrow{p} m_B \to 0
$$
où l’application $i$ est déduite par passage aux quotients de l’application $a \mapsto ax$ de $A$ dans $m_A$ et où $p$ est la surjection canonique ; elle est exacte. Puisque la classe de $x$ dans le $\kappa_A$-espace vectoriel $m_A/m_A^2$ n’est pas nulle, il existe une application $A$-linéaire $\phi : m_A \to \kappa_A$ avec $\phi(x) = 1$; par passage au quotient, on déduit de $\phi$ une rétraction de $i$, de sorte que la suite exacte précédente est scindée. Cela entraîne les relations
$$
\mathrm{dp}_B(m_B) \leq \mathrm{dp}_B(m_A/xm_A) = \mathrm{dp}_A(m_A) < +\infty
$$
(cor. 2 de la prop. 7 du $§ 3$, n° 4 et $\Lambda$, X, p. 135, cor. 1). Le cor. 2 de loc. cit. appliqué à la suite exacte de $B$-modules $0 \to m_B \to B \to \kappa_B \to 0$ entraîne $\mathrm{dp}_B(\kappa_B) < +\infty$. L’anneau $B$ est donc de dimension homologique finie ($§ 3$, n° 3, cor. 2 de la prop. 4), et de profondeur $n - 1$ ($§ 1$, n° 4, prop. 7 et n° 3, cor. de la prop. 4). Il résulte de l’hypothèse de récurrence que $B$ est régulier, donc que $A$ est régulier (VIII, $§ 5$, n° 3, cor. 1 de la prop. 2).

Par conséquent, si $A$ est un anneau local noethérien, il y a équivalence entre les trois propriétés suivantes :
(i) $A$ est régulier ;
(ii) le $A$-module $\kappa_A$ est de dimension projective finie ;
(iii) tout $A$-module de type fini est de dimension projective $< +\infty$.

#### Définition 1 {#ac-x-s4-def-1 .statement}

On dit qu’un anneau $A$ est régulier s’il est noethérien et que l’anneau local $A_m$ est régulier pour tout idéal maximal $m$ de $A$.

#### Proposition 4 {#ac-x-s4-prop-4 .statement}

Soit $A$ un anneau noethérien. Les conditions suivantes sont équivalentes :
(i) $A$ est régulier ;
(ii) tout $A$-module de type fini est de dimension projective $< +\infty$ ;
(iii) pour tout idéal maximal $m$ de $A$, la dimension projective de $A/m$ est finie ;
(iv) pour tout idéal premier $p$ de $A$, l’anneau local $A_p$ est régulier.

Prouvons que (i) implique (ii). Soit $M$ un $A$-module de type fini. Sous l’hypothèse (i), on a $\mathrm{dp}_{A_m}(M_m) \leq \mathrm{dh}(A_m) < +\infty$ pour tout idéal maximal $m$ de $A$ (n° 1, prop. 1) ; donc $M$ est de dimension projective $< +\infty$ ($§ 3$, n° 2, cor. 2 de la prop. 3), d’où (ii).

#### Exemple 1 {#ac-x-s4-n2-exa-1 .statement}

Si l’anneau $A$ est régulier, l’anneau de fractions $S^{-1}A$ est régulier pour toute partie multiplicative $S$ de $A$ : cela résulte par exemple de la caractérisation (iii) ci-dessus.

#### Exemple 2 {#ac-x-s4-n2-exa-2 .statement}

Pour qu’un anneau soit régulier, il faut et il suffit qu’il soit isomorphe au produit d’une famille finie d’anneaux réguliers intègres ; cela résulte en effet de ce que tout anneau régulier est localement intègre ($§ 1$, n° 8), puisque les anneaux locaux réguliers sont intègres.

#### Exemple 3 {#ac-x-s4-n2-exa-3 .statement}

Les anneaux réguliers intègres de dimension $\leq 1$ sont les anneaux de Dedekind (VIII, $§ 5$, n° 1, exemple 1 et VII, $§ 2$, n° 2, théorème 1).

**Corollaire 1.** *Soit $A$ un anneau noethérien. Les conditions suivantes sont équivalentes* :

(i) *on a* $\mathrm{dh}(A) < +\infty$ ;
(ii) *$A$ est régulier et l’on a* $\dim(A) < +\infty$.

*Si ces conditions sont réalisées, on a* $\dim(A) = \mathrm{dh}(A)$.

Si l’anneau $A$ est régulier, on a pour tout idéal maximal $m$ de $A$ l’égalité $\dim(A_m) = \mathrm{dh}(A_m)$ (n° 1, prop. 1), et donc

$$
\mathrm{dh}(A) = \sup_m \mathrm{dh}(A_m) = \sup_m \dim(A_m) = \dim A
$$

($§ 3$, n° 2, prop. 3 et VIII, $§ 1$, n° 3, prop. 8). D’autre part, si $\mathrm{dh}(A) < +\infty$, l’anneau $A$ est régulier d’après la prop. 4. Le corollaire en résulte.

Il existe des anneaux noethériens réguliers de dimension infinie (VIII, $§ 5$, exerc. 6).

**Corollaire 2.** *Un anneau régulier est normal, de Gorenstein et de Macaulay.*

En effet, un anneau local régulier est intégralement clos (VIII, $§ 5$, n° 2, cor. 1 du th. 1), de Gorenstein ($§ 3$, n° 9, exemple 4) et de Macaulay ($§ 2$, n° 5, exemple 6).

**Corollaire 3.—** *Soient $A$ un anneau noethérien, $J$ un idéal de $A$ et $\hat{A}$ le séparé complété de $A$ pour la topologie $J$-adique.*

a) *Pour que l’anneau $\hat{A}$ soit régulier, il faut et il suffit que, pour tout idéal maximal $m$ de $A$ contenant $J$, l’anneau $A_m$ soit régulier.*

b) *Si l’anneau $A$ est régulier, l’anneau $\hat{A}$ est régulier. Si l’anneau $\hat{A}$ est régulier et l’idéal $J$ contenu dans le radical de $A$, l’anneau $\Lambda$ est régulier.*

#### Corollaire 4 {#ac-x-s4-prop-4-cor-4 .statement}

*Soient $A$ un anneau régulier et $P$ un $A$-module projectif de type fini. L’algèbre symétrique $S_A(P)$ est un anneau régulier.*

Soient $p$ un idéal premier de $S_A(P)$ et $q$ son image réciproque dans $A$. L’anneau local $S_A(P)_p$ est un anneau de fractions de l’anneau $S_A(P)_q$, qui est isomorphe à $S_{A_q}(P_q)$ (A, III, p. 72, prop. 7); il suffit de prouver que ce dernier est régulier. Cela nous ramène au cas où $A$ est local ; mais alors $P$ est libre de type fini. D’après la prop. 1 du n° 1 et A, X, p. 143, cor. 1, on a $dh(S_A(P)) = dh(A) + rg_A(P) < +\infty$, et $S_A(P)$ est régulier d’après la prop. 4.

#### Corollaire 5 {#ac-x-s4-prop-4-cor-5 .statement}

*Soient $A$ un anneau régulier, et $(T_i)_{i \in I}$ une famille finie d’indéterminées. L’anneau de polynômes $A[(T_i)_{i \in I}]$ et l’anneau de séries formelles $A[[T_i]_{i \in I}]$ sont réguliers.*

Cela résulte du cor. 4 et du cor. 3 b).

### 3. Anneaux réguliers et algèbres finies

#### Proposition 5 {#ac-x-s4-prop-5 .statement}

*Soient $\rho : A \to B$ un homomorphisme d’anneaux noethériens et $N$ un $B$-module. On suppose que
a) l’anneau $A$ est régulier,
b) $N$ est un $A$-module de type fini,
c) le $B$-module $N$ est macaulayen,
d) tout idéal premier minimal de $\mathrm{Supp}_B(N)$ est au-dessus d’un idéal premier minimal de $A$.
Alors $N$ est un $A$-module projectif (de type fini).*

Il s’agit de prouver que, pour tout idéal maximal $m$ de $A$, le $A_m$-module $N_m$ est libre (II, § 5, n° 2, th. 1). Le $A$-module $B/\mathrm{Ann}_B(N)$ est un sous-module du $A$-module de type fini $\mathrm{End}_A(N)$, donc est de type fini. Si l’on remplace $B$ par $B/\mathrm{Ann}_B(N)$, les hypothèses de la proposition sont encore vérifiées ($§ 2$, n° 1, exemple 5); on peut donc supposer que $B$ est un $A$-module de type fini et que $\mathrm{Supp}_B(N) = \mathrm{Spec}(B)$.

Soit $m$ un idéal maximal de $\mathrm{Supp}_A(N)$; posons $n = \dim(A_m)$. D’après le cor. 2 de la prop. 3 du n° 1, il suffit de prouver que $N_m$ est un $A_m$-module macaulayen de dimension $n$. Tout idéal maximal de $B_m$ est de la forme $nB_m$, où $n$ est un idéal premier de $B$ au-dessus de $m$ (V, § 2, n° 1, lemme 1 et prop. 1). Soit $p$ un idéal premier minimal de $\mathrm{Supp}_B(N)$, contenu dans $n$. La partie fermée $V(pB_n)$ de $\mathrm{Supp}_{B_n}(N_n)$ est alors de codimension nulle; le $B_n$-module $N_n$ étant macaulayen, le cor. de la prop. 2, § 2, n° 2 entraîne l’égalité $\dim_{B_n}(N_n) = \dim(B_n/pB_n)$. Mais $p$ est au-dessus d’un idéal premier minimal de $A$, contenu dans $m$, de sorte que

#### Corollaire {#ac-x-s4-n3-cor-1 .statement}

Soit B un anneau noethérien intègre et soit A un sous-anneau régulier de B. Supposons que le A-module B soit de type fini. Pour que l’anneau B soit de Macaulay, il faut et il suffit que le A-module B soit projectif.

Si l’anneau B est de Macaulay, le A-module B est projectif d’après la prop. 5.

Supposons inversement le A-module B projectif. Le A-module A est macaulayen (cor. 2 de la prop. 4) ; le A-module B est facteur direct dans un A-module libre de type fini, donc est macaulayen (§ 2, n° 1, exemple 2). On applique alors le cor. 1 de la prop. 8 du § 2, n° 6.

#### Exemple {#ac-x-s4-n3-exa-1 .statement}

Soit B une algèbre intègre non nulle de type fini sur un corps K. D’après VIII, § 2, n° 4, cor. 1 du th. 3, il existe une sous-algèbre A de B isomorphe à une algèbre de polynômes sur K et telle que B soit un A-module de type fini. Les propriétés suivantes sont équivalentes :

(i) l’anneau B est macaulayen ;
(ii) le A-module B est projectif ;
*(iii) le A-module B est libre.*

### 4. Anneaux présentables

On dit qu’un anneau A est présentable s’il existe un anneau régulier R et un homomorphisme surjectif de R dans A.

Par définition, les anneaux réguliers sont présentables.

#### Proposition 6 {#ac-x-s4-prop-6 .statement}

a) Tout anneau de fractions d’un anneau présentable est présentable. Toute algèbre de type fini sur un anneau présentable est un anneau présentable.

b) Soient A un anneau présentable et J un idéal de A. Le séparé complété $\widehat{A}$ de A pour la topologie J-adique est présentable.

c) Tout anneau local noethérien complet est présentable.

d) Soit A un anneau local présentable. Il existe un anneau local régulier R et un homomorphisme local surjectif de R dans A.

Soit A un anneau présentable ; choisissons un anneau régulier R et un homomorphisme surjectif $\rho : R \to A$.

a) Soit S une partie multiplicative de A ; posons T = $\rho^{-1}(S)$. L’homomorphisme $T^{-1}R \to S^{-1}A$ déduit de $\rho$ est surjectif et l’anneau $T^{-1}R$ est régulier (n° 3, exemple 1), donc $S^{-1}A$ est présentable.

Soit B une A-algèbre de type fini ; il existe un ensemble fini I et un homomorphisme surjectif $A[(T_i)_{i \in I}] \to B$, donc un homomorphisme surjectif $R[(T_i)_{i \in I}] \to B$. Comme l’anneau $R[(T_i)_{i \in I}]$ est régulier (n° 2, cor. 5 de la prop. 4), l’anneau B est présentable.

b) Posons $I = \rho^{-1}(J)$ et notons $\hat{R}$ le séparé complété de R pour la topologie I-adique ; pour chaque entier $n \geq 0$, l’application canonique $I^n/I^{n+1} \to J^n/J^{n+1}$ est surjective. Par conséquent, l’homomorphisme $\hat{R} \to \hat{A}$ déduit de $\rho$ est surjectif (III, § 2, n° 8, cor. 2 du th. 1) ; comme $\hat{R}$ est régulier (n° 2, cor. 3 de la prop. 4), l’anneau $\hat{A}$ est présentable.

c) Cela résulte de IX, § 2, n° 5, th. 3 a) et IX, § 3, n° 3, th. 2 a).

d) Soit $m_A$ l’idéal maximal de A ; alors $p = \rho^{-1}(m_A)$ est un idéal premier de R, l’anneau local $R_p$ est régulier et l’homomorphisme $R_p \to A$ déduit de $\rho$ est local et surjectif.

Puisque les corps et les anneaux de Dedekind sont réguliers, donc présentables, la proposition 6 implique que la plupart des anneaux rencontrés usuellement en géométrie algébrique sont présentables.

#### Proposition 7 {#ac-x-s4-prop-7 .statement}

Soit A un anneau présentable.

a) L’anneau $\Lambda$ est noethérien et caténaire.

b) Soit M un A-module de type fini. L’application
$$
p \mapsto \dim_{A_p}(M_p) - \operatorname{prof}_{A_p}(M_p)
$$
de $\operatorname{Spec}(A)$ dans $\mathbf{Z}$ est semi-continue supérieurement.

c) Soit M un $\Lambda$-module de type fini. L’ensemble des $p \in \operatorname{Spec}(A)$ tels que le $A_p$-module $M_p$ soit macaulayen est un ouvert dense. Son intersection avec $\operatorname{Supp}(M)$ est dense dans $\operatorname{Supp}(M)$.

Choisissons un anneau régulier R et un homomorphisme surjectif $R \to A$.

a) L’anneau R est de Macaulay (n° 2, cor. 2 de la prop. 4), donc A est caténaire ($§ 2$, n° 2, prop. 2 et VIII, § 1, n° 3, rem. 2).

b) Le R-module M est de type fini et de dimension projective $< +\infty$ (n° 1, prop. 1). Identifions $\operatorname{Spec}(A)$ à une partie fermée de $\operatorname{Spec}(R)$. Alors la fonction $p \mapsto \dim_{A_p}(M_p) - \operatorname{prof}_{A_p}(M_p)$ sur $\operatorname{Spec}(A)$ est la restriction de la fonction $q \mapsto \dim_{R_q}(M_q) - \operatorname{prof}_{R_q}(M_q)$ sur $\operatorname{Spec}(R)$ ; il suffit alors d’appliquer le cor. 4 du th. 1 du $§ 3$, n° 5.

c) Cela se démontre comme la partie c) de loc. cit.

### 5. Anneaux réguliers et extensions plates

#### Proposition 8 {#ac-x-s4-prop-8 .statement}

Soit $\rho : A \to B$ un homomorphisme d’anneaux noethériens faisant de B un A-module fidèlement plat.

a) Pour tout A-module M de type fini, on a $dp_A(M) = dp_B(B \otimes_A M)$.

b) Si l’anneau B est régulier, l’anneau A est régulier.

$$
0 \to N \to L \to M \to 0
$$

où le $A$-module $L$ est libre de type fini. On a $dp_A(N) = dp_A(M) - 1$ (A, X, p. 135, cor. 2 de la prop. 1). Comme $B$ est plat sur $A$, la suite

$$
0 \to B \otimes_A N \to B \otimes_A L \to B \otimes_A M \to 0
$$

est exacte et on a $dp_B(B \otimes_A N) = dp_B(B \otimes_A M) - 1$. L’hypothèse de récurrence appliquée à $N$ permet de conclure. Cela prouve a) ; l’assertion b) résulte de a) et de la prop. 4 du n° 2.

#### Corollaire {#ac-x-s4-n5-cor-1 .statement}

*Soit $B$ un anneau régulier intègre et soit $A$ un sous-anneau noethérien de $B$ tel que $B$ soit un $A$-module de type fini. Les conditions suivantes sont équivalentes :*

(i) $A$ est régulier ;
(ii) $B$ est un $A$-module projectif ;
(iii) $B$ est un $A$-module plat ;
(iv) $B$ est un $A$-module fidèlement plat.

(i) $\Rightarrow$ (ii) : cela résulte du cor. de la prop. 5 du n° 3.
(ii) $\Rightarrow$ (iii) : cela résulte de I, § 3, n° 1, prop. 1.
(iii) $\Rightarrow$ (iv) : pour tout idéal premier $\mathfrak{p}$ de $A$, on a $\mathfrak{p}B \neq B$ (V, § 2, n° 1, cor. 1 du théorème 1). Il suffit alors d’appliquer I, § 3, n° 1, prop. 1.
(iv) $\Rightarrow$ (i) : cela résulte de la prop. 8, b).

Pour tout anneau local noethérien $A$, notons $\delta(A)$ l’entier

$$
\delta(A) = [\mathfrak{m}_A / \mathfrak{m}_A^2 : \kappa_A] - \dim(A)
$$

Rappelons (VIII, § 5, n° 1) que $\delta(A)$ est toujours positif et que son annulation caractérise les anneaux locaux réguliers.

Soit $\rho : A \to B$ un homomorphisme local d’anneaux locaux noethériens ; on déduit de $\rho$ un homomorphisme $\kappa_A$-linéaire $\mathfrak{m}_A / \mathfrak{m}_A^2 \to \mathfrak{m}_B / \mathfrak{m}_B^2$, d’où un homomorphisme $\kappa_B$-linéaire

$$
d\rho : \kappa_B \otimes_{\kappa_A} (\mathfrak{m}_A / \mathfrak{m}_A^2) \to \mathfrak{m}_B / \mathfrak{m}_B^2 .
$$

*Lemme 1.— On a*

$$
\delta(B) + [\mathrm{Ker}(d\rho) : \kappa_B] = \delta(A) + \delta(\kappa_A \otimes_A B) + (\dim(A) - \dim(B) + \dim(\kappa_A \otimes_A B)) .
$$

Notons $C$ l’anneau local $\kappa_A \otimes_A B$. Considérons la suite exacte de $B$-modules

$$
B \otimes_A \mathfrak{m}_A \to \mathfrak{m}_B \to \mathfrak{m}_C \to 0 ;
$$

par produit tensoriel avec $\kappa_B$, on obtient une suite exacte de $\kappa_{13}$-espaces vectoriels

$$
\kappa_B \otimes_{\kappa_A} (\mathfrak{m}_A/\mathfrak{m}_A^2) \xrightarrow{d\rho} \mathfrak{m}_B/\mathfrak{m}_B^2 \longrightarrow \mathfrak{m}_C/\mathfrak{m}_C^2 \to 0,
$$

d’où l’on déduit l’égalité

$$
[\mathfrak{m}_B/\mathfrak{m}_B^2 : \kappa_B] + [\mathrm{Ker}(d\rho) : \kappa_B] = [\mathfrak{m}_A/\mathfrak{m}_A^2 : \kappa_A] + [\mathfrak{m}_C/\mathfrak{m}_C^2 : \kappa_C],
$$

qui entraîne le lemme.

#### Proposition 9 {#ac-x-s4-prop-9 .statement}

*Soit $\rho : A \to B$ un homomorphisme local d’anneaux locaux noethériens. Les conditions suivantes sont équivalentes :

(i) l’anneau $B$ est régulier et l’application $\kappa_B$-linéaire

$$
d\rho : \kappa_B \otimes_{\kappa_A} (\mathfrak{m}_A/\mathfrak{m}_A^2) \longrightarrow \mathfrak{m}_B/\mathfrak{m}_B^2
$$

est injective ;
(ii) les anneaux $B$ et $\kappa_A \otimes_A B$ sont réguliers et le $A$-module $B$ est plat ;
(iii) les anneaux $A$ et $\kappa_A \otimes_A B$ sont réguliers et le $A$-module $B$ est plat ;
(iv) les anneaux $A$ et $\kappa_A \otimes_A B$ sont réguliers, et l’on a

$$
\dim(B) = \dim(A) + \dim(\kappa_A \otimes_A B).
$$

On a $\dim(B) \leq \dim(A) + \dim(\kappa_A \otimes_A B)$ (VIII, § 3, n° 4, cor. 1 de la prop. 7) ; l’équivalence de (i) et (iv) résulte donc du lemme 1. Sous l’hypothèse (ii), le $A$-module $B$ est fidèlement plat puisqu’on a $\mathfrak{m}_A B \subset \mathfrak{m}_B \neq B$ (I, § 3, n° 1, prop. 1), ce qui entraîne (iii) d’après la prop. 8. L’implication (iii) $\Rightarrow$ (iv) résulte de VIII, *loc. cit*.

Il nous suffit maintenant de prouver que lorsque les conditions équivalentes (i) et (iv) sont satisfaites, le $A$-module $B$ est plat. Soit $x$ un système de coordonnées de $A$. Puisque $d\rho$ est injective, l’image par $\rho$ de cette suite fait partie d’un système de coordonnées de $B$. Ainsi la suite $x$ est complètement sécante pour $A$ et pour $B$ (VIII, § 5, n° 3, prop. 2), et engendre l’idéal $\mathfrak{m}_A$ de $A$. D’après la remarque 3 de A, X, p. 159, le $A$-module $\mathrm{Tor}_1^A(\kappa_A, B)$ est isomorphe à $H_1(x, B)$, donc est nul ; il en résulte que $B$ est plat sur $A$ (III, § 5, n° 2, th. 1 et n° 4, prop. 2).

#### Exemple {#ac-x-s4-n5-exa-1 .statement}

*Soient $X$, $Y$ deux variétés analytiques complexes, localement de dimension finie, $f$ un morphisme de $X$ dans $Y$, et $x$ un point de $X$. Considérons l’homomorphisme local $\rho : \mathcal{O}_{Y, f(x)} \to \mathcal{O}_{X, x}$ associé à $f$. L’application $d\rho$ est la transposée de l’application tangente $T_x(f) : T_x(X) \to T_{f(x)}(Y)$. Les conditions (i) à (iv) de la proposition 9 équivalent donc dans ce cas au fait que $f$ soit une submersion en $x$ (VAR, R, 5.9.1).*

#### Corollaire {#ac-x-s4-n5-cor-2 .statement}

*Soit $\rho : \Lambda \to B$ un homomorphisme d’anneaux noethériens faisant de $B$ un $A$-module plat. Si $A$ est régulier et si $\kappa(\rho^{-1}(\mathfrak{n})) \otimes_{\Lambda} B$ est régulier pour tout idéal maximal $\mathfrak{n}$ de $B$, l’anneau $B$ est régulier.

En effet pour tout idéal maximal $\mathfrak{n}$ de $B$ le $A_{\rho^{-1}(\mathfrak{n})}$-module $B_n$ est plat (II, § 3, n° 4, prop. 15), de sorte que l’anneau $B_n$ est régulier d’après la prop. 9.

## EXERCICES {#ac-x-s4-exercises}

See the [exercises for § 4](exercises/s4/).
