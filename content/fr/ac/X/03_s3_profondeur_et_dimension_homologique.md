---
book: ac
book_title: Commutative Algebra
chapter: X
chapter_title: Profondeur, régularité, dualité
section: 3
section_title: Profondeur et dimension homologique
lang: fr
source: ac-x-fr
pdf_pages: 0036-0051, 0156-0161
extraction: ocr
subsections:
    - "no": 1
      title: Dimension projective, dimension injective, dimension homologique
      page: 0
      pdf_page: 36
    - "no": 2
      title: Localisation de la dimension homologique
      page: 38
      pdf_page: 37
    - "no": 3
      title: Dimension homologique des anneaux noethériens
      page: 0
      pdf_page: 38
    - "no": 4
      title: Quotient par un élément simplifiable
      page: 43
      pdf_page: 42
    - "no": 5
      title: Profondeur et dimension projective
      page: 45
      pdf_page: 44
    - "no": 6
      title: Profondeur et dimension injective
      page: 0
      pdf_page: 46
    - "no": 7
      title: Anneaux de Gorenstein
      page: 48
      pdf_page: 47
    - "no": 8
      title: Anneaux de Gorenstein et algèbres plates
      page: 51
      pdf_page: 50
statements: 26
exercises: 16
content_sha256: 368543644bd264c2543c7fe61456948403e44a81447152dff4e406a7c7ea5786
---

## § 3. PROFONDEUR ET DIMENSION HOMOLOGIQUE

### 1. Dimension projective, dimension injective, dimension homologique

Soient A un anneau, M un A-module. Rappelons (A, X, p. 134, déf. 1) que la dimension projective de M, notée dp_A(M), est la borne inférieure (dans $\overline{\mathbf{Z}}$) de l’ensemble des longueurs des résolutions projectives de M. On a dp_A(0) = -∞ et dp_A(M) ≥ 0 si M est non nul. Pour que M soit projectif, il faut et il suffit que l’on ait dp_A(M) ≤ 0.

#### Exemple {#ac-x-s3-n1-exa-1 .statement}

Soit J un idéal de A engendré par une suite A-régulière $x = (x_1, \ldots, x_r)$. On a dp_A(A/J) ≤ r. En effet, c’est clair si A est nul ; dans le cas contraire, le complexe de Koszul $K_\bullet(x, A)$ est une résolution libre de A/J de longueur r (loc. cit., p. 159, remarque 3). De plus, pour tout A-module N, les A-modules Ext_A^r(A/J, N) et N/JN sont isomorphes (loc. cit.) ; par suite, pour qu’on ait dp_A(A/J) = r, il faut et il suffit que J soit distinct de A (loc. cit., p. 134, prop. 1).

On définit de même la dimension injective de M, que l’on note di_A(M), comme la borne inférieure de l’ensemble des longueurs des résolutions injectives de M. On a di_A(0) = -∞, et di_A(M)_0 si M ≠ 0. Pour que M soit injectif, il faut et il suffit que l’on ait di_A(M) ≤ 0.

#### Proposition 1 {#ac-x-s3-prop-1 .statement}

Soient A un anneau, M un A-module et n un entier ≥ 0. Les conditions suivantes sont équivalentes :

(i) on a di_A(M) ≤ n (autrement dit, M possède une résolution injective de longueur ≤ n) ;
(ii) pour tout A-module N et tout entier i > n, on a Ext_A^i(N, M) = 0 ;
(iii) pour tout idéal a de A, on a Ext_A^{n+1}(A/a, M) = 0 ;
(iv) pour toute suite exacte de A-modules

$$
0 \to M \to I^0 \to I^1 \to \ldots \to I^{n-1} \to Q \to 0,
$$

où les $I^i$ sont injectifs, le A-module Q est injectif.

(i) ⇒ (ii) : cela résulte de A, X, p. 100, th. 1.
(ii) ⇒ (iii) : c’est clair.
(iii) ⇒ (iv) : dans la situation de (iv), on a pour tout A-module N un isomorphisme de Ext_A^1(N, Q) sur Ext_A^{n+1}(N, M) (A, X, p. 128, cor. 4) ; sous l’hypothèse (iii), le A-module Ext_A^1(A/a, Q) est nul pour tout idéal a de A et Q est injectif (A, X, p. 93, prop. 11).
(iv) ⇒ (i) : considérons la suite exacte (A, X, p. 52)

$$
0 \to M \to I^0(M) \to \ldots \to I^{n-1}(M) \to K^{n-1}(M) \to 0;
$$

si la condition (iv) est satisfaite, le A-module $K^{n-1}(M)$ est injectif, d’où (i).

Rappelons (A, X, p. 138, déf. 2) que la dimension homologique de l’anneau $A$, notée $\mathrm{dh}(A)$, est la borne supérieure dans $\overline{\mathbf{Z}}$ de l’ensemble des entiers $n$ pour lesquels il existe deux $A$-modules $M$ et $N$ tels que $\mathrm{Ext}^n_A(M, N)$ soit non nul. C’est donc aussi la borne supérieure de l’ensemble des dimensions projectives (ou injectives) de tous les $A$-modules ; lorsque $A$ est noethérien, on peut se borner aux $A$-modules de type fini (A, X, p. 139, cor.).

### 2. Localisation de la dimension homologique

#### Proposition 2 {#ac-x-s3-prop-2 .statement}

Soient $A$ un anneau, $M$ et $N$ des $A$-modules, $i$ un entier et $S$ une partie multiplicative de $\Lambda$. On a un isomorphisme canonique de $S^{-1}A$-modules

$$
S^{-1} \mathrm{Tor}_i^\Lambda(M, N) \longrightarrow \mathrm{Tor}_i^{S^{-1}\Lambda}(S^{-1}M, S^{-1}N) .
$$

Si l’anneau $A$ est noethérien et le $A$-module $M$ de type fini, on a un isomorphisme canonique de $S^{-1}\Lambda$-modules

$$
S^{-1} \mathrm{Ext}_\Lambda^i(M, N) \longrightarrow \mathrm{Ext}_{S^{-1}\Lambda}^i(S^{-1}M, S^{-1}N) .
$$

Comme le $A$-module $S^{-1}A$ est plat, cela résulte de A, X, p. 110, prop. 9 et p. 111, prop. 10.

#### Corollaire {#ac-x-s3-n2-cor-1 .statement}

Soient $A$ un anneau, $M$ et $N$ des $\Lambda$-modules, $i$ un entier.

a) Le support de $\mathrm{Tor}_i^\Lambda(M, N)$ est contenu dans $\mathrm{Supp}(M) \cap \mathrm{Supp}(N)$, et il en est de même du support de $\mathrm{Ext}_\Lambda^i(M, N)$ si $A$ est noethérien et $M$ de type fini.

b) Supposons $A$ noethérien, les modules $M$ et $N$ de type fini ; si le $\Lambda$-module $M \otimes_A N$ est de longueur finie, il en est de même de $\mathrm{Tor}_i^\Lambda(M, N)$ et de $\mathrm{Ext}_\Lambda^i(M, N)$.

Si $p$ est un idéal premier de $A$ n’appartenant pas à $\mathrm{Supp}(M) \cap \mathrm{Supp}(N)$, l’un des modules $M_p$ ou $N_p$ est nul, ce qui implique a) compte tenu de la prop. 2.

Pour qu’un module de type fini sur un anneau noethérien soit de longueur finie, il faut et il suffit que son support soit formé d’idéaux maximaux (IV, § 2, n° 5, prop. 7). Sous l’hypothèse b), les $A$-modules $\mathrm{Tor}_i^\Lambda(M, N)$ et $\mathrm{Ext}_\Lambda^i(M, N)$ sont de type fini (A, X, p. 108, cor.) ; l’assertion b) résulte donc de a).

#### Proposition 3 {#ac-x-s3-prop-3 .statement}

Soient $A$ un anneau noethérien, $M$ un $A$-module de type fini et $N$ un $A$-module.

a) On a

$$
\mathrm{dp}_A(M) = \sup_p \mathrm{dp}_{A_p}(M_p) , \quad \mathrm{di}_A(N) = \sup_p \mathrm{di}_{A_p}(N_p) , \quad \mathrm{dh}(A) = \sup_p \mathrm{dh}(A_p) ,
$$

où $p$ parcourt l’ensemble des idéaux premiers (resp. maximaux) de $A$.

b) L’application $p \mapsto \mathrm{dp}_{A_p}(M_p)$ de $\mathrm{Spec}(A)$ dans $\overline{\mathbf{Z}}$ est semi-continue supérieurement.

Prouvons a). Soit $n$ un entier $\geqslant 0$. Supposons qu’on ait $\mathrm{dp}_A(M) < n$. Pour tout idéal premier $p$ de $A$ et tout $A_p$-module $Q$, le $A_p$-module $\mathrm{Ext}_A^n(M_p, Q)$ est isomorphe à $(\mathrm{Ext}_A^n(M, Q))_p$ (prop. 2), donc est nul ; on en déduit l’inégalité

Prouvons b). Soient p un idéal premier de A et n = dp_{A_p}(M_p). Démontrons qu’il existe un voisinage U de p dans Spec(A) tel que l’on ait dp_{A_q}(M_q) \leq n pour tout q \in U. C’est clair si n = +\infty ; si n = -\infty , cela résulte du fait que le support de M est fermé. Supposons maintenant n fini et choisissons une suite exacte de A-modules
$$
P_{n-1} \xrightarrow{d_{n-1}} P_{n-2} \longrightarrow \ldots \longrightarrow P_0 \xrightarrow{d_0} M \to 0 ,
$$
où les P_i sont libres de type fini (A, X, p. 53, prop. 6). Posons P = Ker d_{n-1} ; c’est un module de présentation finie. Le A_p-module P_p est projectif (A, X, p. 134, prop. 1), donc libre (II, § 3, n° 2, cor. 2 de la prop. 5). D’après II, § 5, n° 1, cor. de la prop. 2, il existe un élément f de A - p tel que le A_f-module P_f soit libre ; le A_q-module P_q est alors libre pour tout élément q de l’ouvert U de Spec(A) formé des idéaux premiers ne contenant pas f . Cela prouve b).

#### Corollaire 1 {#ac-x-s3-prop-3-cor-1 .statement}

Pour toute partie multiplicative S de A , on a
$$
\mathrm{dp}_{S^{-1}A}(S^{-1}M) \leq \mathrm{dp}_A(M) \quad , \quad \mathrm{di}_{S^{-1}A}(S^{-1}N) \leq \mathrm{di}_A(N) \quad , \quad \mathrm{dh}(S^{-1}A) \leq \mathrm{dh}(A) .
$$

#### Corollaire 2 {#ac-x-s3-prop-3-cor-2 .statement}

Si on a dp_{A_m}(M_m) < +\infty pour tout idéal maximal m de Supp(M) , on a dp_A(M) < +\infty .

En effet, le sous-espace X de Supp(M) formé des idéaux maximaux est quasi-compact (II, § 4, n° 2, prop. 8 et 9 et n° 3, cor. 7 de la prop. 11) ; l’application m \mapsto dp_{A_m}(M_m) de X dans \overline{\mathbf{R}} est semi-continue supérieurement (prop. 3), donc bornée (TG, IV, p. 30, cor. du th. 3).

#### Remarque {#ac-x-s3-n2-rem-1 .statement}

Soit A un anneau noethérien régulier de dimension infinie (VIII, § 5, exerc. 6 c)). Nous verrons ci-dessous (n° 7, th. 2 et § 4, n° 1, prop. 1) qu’on a di_{A_m}(A_m) = dh(A_m) < +\infty pour tout idéal maximal m de A ; la prop. 3 entraîne donc di_A(A) = dh(A) = +\infty . Par conséquent, les fonctions p \mapsto di_{A_p}(N_p) et p \mapsto dh(A_p) ne sont pas en général semi-continues supérieurement.

### 3. Dimension homologique des anneaux noethériens

Soient A un anneau local noethérien, M un A-module de type fini. Rappelons (A, X, § 3, n° 6) qu’une résolution
$$
\ldots \longrightarrow L_n \xrightarrow{d_n} L_{n-1} \longrightarrow \ldots \longrightarrow L_0 \xrightarrow{d_0} M \to 0
$$
de M est une résolution projective minimale si chacun des modules L_i est libre de type fini, et si le complexe $\kappa_A \otimes_A L$ est à différentielle nulle. Pour tout entier $i \geq 0$, on a alors

(1) $$ \operatorname{Ext}_A^i(M, \kappa_A) : \kappa_A ] = [\operatorname{Tor}_i^A(M, \kappa_A) : \kappa_A ] = \operatorname{rg}_A(L_i) $$

(A, X, p. 103, exemple 3). Tout A-module de type fini admet une telle résolution (A, X, p. 56, prop. 10).

**Proposition 4.** *Soient A un anneau local noethérien, M un A-module de type fini et n un entier $\geq 0$. Les conditions suivantes sont équivalentes* :

(i) *on a* $\operatorname{dp}_A(M) < n$ ;
(ii) *on a* $\operatorname{Tor}_n^A(M, \kappa_A) = 0$ ;
(iii) *on a* $\operatorname{Ext}_A^n(M, \kappa_A) = 0$ ;
(iv) *toute résolution projective minimale de M est de longueur* $< n$.

Les assertions (i) $\Rightarrow$ (ii) et (i) $\Rightarrow$ (iii) sont immédiates (A, X, p. 100, th. 1). Soit L une résolution projective minimale de M ; si (ii) ou (iii) est vérifié, on a $L_n = 0$ d’après (1). Comme toute résolution projective minimale de M est isomorphe à L (A, X, p. 54, prop. 8), on en déduit (iv). L’implication (iv) $\Rightarrow$ (i) est triviale.

**Corollaire 1.—** *Soient A un anneau local noethérien et n un entier $\geq 0$. Les conditions suivantes sont équivalentes* :

(i) *on a* $\operatorname{dh}(A) < n$ ;
(ii) *on a* $\operatorname{Ext}_A^i(M, N) = 0$ *et* $\operatorname{Tor}_i^A(M, N) = 0$ *pour tout couple* $(M, N)$ *de A-modules et tout entier* $i \geq n$ ;
(iii) *on a* $\operatorname{Tor}_n^A(\kappa_A, \kappa_A) = 0$ ;
(iv) *on a* $\operatorname{Ext}_A^n(\kappa_A, \kappa_A) = 0$ ;
(v) *on a* $\operatorname{dp}_A(\kappa_A) < n$.

Il est clair que (i) implique (ii) et que (ii) implique (iii) et (iv). D’après la prop. 4 appliquée au A-module $\kappa_A$, chacune des conditions (iii) et (iv) implique (v). Prouvons que (v) implique (i) : si $\operatorname{dp}_A(\kappa_A) < n$, on a $\operatorname{Tor}_n^A(M, \kappa_A) = 0$ pour tout A-module M ; par suite tout A-module de type fini est de dimension projective $< n$ (prop. 4), ce qui entraîne $\operatorname{dh}(A) < n$ (A, X, p. 138, prop. 4).

**Corollaire 2.—** *On a* $\operatorname{dh}(A) = \operatorname{dp}_A(\kappa_A)$.

*Remarques.* 1) Soit A un anneau local. Le A-module $\operatorname{Tor}_1^A(\kappa_A, \kappa_A)$ est isomorphe à $\mathfrak{m}_A / \mathfrak{m}_A^2$ (A, X, p. 72, exemple). Par suite lorsque A est noethérien, pour que $\operatorname{Tor}_1^A(\kappa_A, \kappa_A)$ soit nul, il faut et il suffit que $\mathfrak{m}_A$ soit nul, c’est-à-dire que A soit un corps. Le cor. 1 entraîne donc qu’un anneau local noethérien de dimension homologique 0 est un corps.

2) Soient A un anneau local noethérien, M un A-module de type fini et de dimension projective finie $n$, N un A-module non nul de type fini. *Le A-module* $\operatorname{Ext}_A^n(M, N)$ *n’est pas nul* : soient en effet L une résolution projective minimale de M, et d sa différentielle. On a une suite exacte

$$
\operatorname{Hom}_A(L_{n-1}, N) \xrightarrow{\operatorname{Hom}(d_n, 1)} \operatorname{Hom}_A(L_n, N) \longrightarrow \operatorname{Ext}_A^n(M, N) \to 0 .
$$

Comme $d_n \otimes 1_{\kappa_A}$ est nulle, on en déduit par produit tensoriel avec $\kappa_A$ un isomorphisme $\kappa_A \otimes_A \mathrm{Hom}_A(L_n, N) \longrightarrow \kappa_A \otimes_A \mathrm{Ext}_A^n(M, N)$, d’où compte tenu de la formule (1) ci-dessus,

$$
[\kappa_A \otimes_A \mathrm{Ext}_A^n(M, N) : \kappa_A] = [\mathrm{Ext}_A^n(M, \kappa_A) : \kappa_A][\kappa_A \otimes_A N : \kappa_A],
$$

qui est non nul par la prop. 4 et le lemme de Nakayama. Par conséquent, la dimension projective de M est le plus grand entier $i$ tel que $\mathrm{Ext}_A^i(M, N)$ soit non nul.

3) Soient $A$ un anneau noethérien, $M$ un $A$-module de type fini et de dimension projective finie, $N$ un $A$-module de type fini dont le support est égal à $\mathrm{Spec}(A)$. D’après la remarque précédente et les prop. 2 et 3 du n° 2, la dimension projective $n$ de $M$ est le plus grand entier $i$ tel que $\mathrm{Ext}_A^i(M, N)$ soit non nul ; le support du $A$-module $\mathrm{Ext}_A^n(M, N)$ est l’ensemble des éléments $p$ de $\mathrm{Spec}(A)$ tels que $\mathrm{dp}_{A_p}(M_p) = n$.

Il peut exister des $A$-modules $M$ de type fini, de dimension projective $+\infty$, satisfaisant à $\mathrm{Ext}_A^i(M, A) = 0$ pour $i$ assez grand : *c’est le cas par exemple du $A$-module $\kappa_A$ lorsque $A$ est un anneau local de Gorenstein qui n’est pas régulier*.

#### Proposition 5 {#ac-x-s3-prop-5 .statement}

*Soient $A$ un anneau noethérien, $M$ un $A$-module de type fini et $n$ un entier $\geqslant 0$. Les conditions suivantes sont équivalentes :

(i) *on a* $\mathrm{dp}_A(M) < n$ ;
(ii) *pour tout idéal maximal* $m$ *de* $A$, *on a* $\mathrm{Ext}_A^n(M, A/m) = 0$ (resp. *on a* $\mathrm{Tor}_n^A(M, A/m) = 0$) ;
(iii) *pour tout idéal maximal* $m$ *de* $A$, *on a* $\mathrm{Ext}_{A_m}^n(M_m, A/m) = 0$ (resp. *on a* $\mathrm{Tor}_n^{A_m}(M_m, A/m) = 0$).

(i) $\Rightarrow$ (ii) : c’est clair.
(ii) $\Rightarrow$ (iii) : cela résulte de la prop. 2 du n° 2.
(iii) $\Rightarrow$ (i) : d’après la prop. 4, la condition (iii) implique l’inégalité $\mathrm{dp}_{A_m}(M_m) < n$ pour tout idéal maximal $m$ de $A$, et on conclut grâce à la prop. 3.

#### Remarque 4 {#ac-x-s3-n3-rem-4 .statement}

Soient $A$ un anneau noethérien et $n$ un entier $\geqslant 0$. Si $m$ et $m'$ sont deux idéaux maximaux de $A$ distincts, les $A$-modules $\mathrm{Ext}_A^n(A/m, A/m')$ et $\mathrm{Tor}_n^A(A/m, A/m')$ sont annulés par $m + m'$, donc sont nuls. Par une démonstration analogue à celle du cor. 1 de la prop. 4, on déduit de la prop. 5 l’équivalence des conditions suivantes :

(i) *on a* $\mathrm{dh}(A) < n$ ;
(ii) *on a* $\mathrm{Ext}_A^i(M, N) = 0$ *et* $\mathrm{Tor}_i^A(M, N) = 0$ *pour tout couple* $(M, N)$ *de* $A$-modules *et tout entier* $i \geqslant n$ ;
(iii) *on a* $\mathrm{Tor}_n^A(A/m, A/m) = 0$ *pour tout idéal maximal* $m$ *de* $A$ ;
(iv) *on a* $\mathrm{Ext}_A^n(A/m, A/m) = 0$ *pour tout idéal maximal* $m$ *de* $A$ ;
(v) *on a* $\mathrm{dp}_A(A/m) < n$ *pour tout idéal maximal* $m$ *de* $A$.

On a en particulier $\mathrm{dh}(A) = \sup_m \mathrm{dp}_A(A/m)$, où $m$ parcourt l’ensemble des idéaux maximaux de $A$.

PROPOSITION 6. Soient $A$ un anneau noethérien, $N$ un $A$-module, $n$ un entier $\geqslant 0$. Les conditions suivantes sont équivalentes :

(i) on a $\operatorname{di}_A(N) < n$ ;
(ii) pour tout idéal premier $p$ de $\Lambda$, on a $\operatorname{Ext}_A^n(\Lambda/p, N) = 0$ ;
(iii) pour tout idéal premier $p$ de $A$, on a $\operatorname{Ext}_{A_p}^n(\kappa(p), N_p) = 0$.

Si de plus le $A$-module $N$ est de type fini, ces conditions équivalent à :

(iv) pour tout idéal maximal $m$ de $A$, on a $\operatorname{Ext}_A^i(A/m, N) = 0$ pour $n \leqslant i \leqslant n + \operatorname{ht}(m)$.

Observons que la condition (iii) équivaut à

(iii') pour tout idéal premier $p$ de $A$, on a $\operatorname{Ext}_A^n(A/p, N) \otimes_A \kappa(p) = 0$.

En effet, comme $\operatorname{Ext}_A^n(A/p, N)$ est annulé par $p$, le $A$-module $\operatorname{Ext}_A^n(A/p, N) \otimes_A \kappa(p)$ est isomorphe à $\operatorname{Ext}_A^n(A/p, N) \otimes_A A_p$, donc à $\operatorname{Ext}_{A_p}^n(\kappa(p), N_p)$ (n° 2, prop. 2).

Les implications (i) $\Rightarrow$ (ii) et (i) $\Rightarrow$ (iv) résultent de la prop. 1 du n° 1, et l’implication (ii) $\Rightarrow$ (iii') est claire.

(iii) $\Rightarrow$ (i) : pour tout $A$-module $M$, posons $T(M) = \operatorname{Ext}_A^n(M, N)$. Supposons que (i) ne soit pas vérifiée. Il existe alors (n° 1, prop. 1) un idéal $a$ de $A$ tel que $T(A/a) \neq 0$. Soit $p$ un idéal de $A$ maximal parmi les idéaux possédant cette propriété ; prouvons que $p$ est premier. D’après IV, § 1, n° 4, th. 1 et th. 2, il existe une suite de composition $(M_i)_{0 \leqslant i \leqslant m}$ de $A/p$ tel que chaque quotient $M_i/M_{i+1}$ soit isomorphe à un module $A/p_i$, où $p_i$ ($0 \leqslant i \leqslant m-1$) est un idéal premier contenant $p$. Si $T(A/p_i)$ était nul pour tout $i$, on déduirait par récurrence sur $i$ des suites exactes

$$
T(M_0/M_i) \longrightarrow T(M_0/M_{i+1}) \longrightarrow T(M_i/M_{i+1})
$$

que $T(M_0/M_m) = T(A/p)$ est nul, ce qui n’est pas. Il existe donc un indice $i$ tel que $T(A/p_i) \neq 0$. Vu le caractère maximal de $p$, on a $p = p_i$, de sorte que $p$ est premier.

Soit $x$ un élément de $A - p$ ; on déduit de la suite exacte

$$
0 \to A/p \xrightarrow{x_{A/p}} A/p \to A/(p + xA) \to 0
$$

une suite exacte

$$
T(A/(p + xA)) \longrightarrow T(A/p) \xrightarrow{u} T(A/p),
$$

où $u = \operatorname{Ext}_A^n(x_A, 1_N) = x_{T(A/p)}$ (A, X, p. 89, prop. 6). À cause du caractère maximal de $p$, on a $T(A/(p + xA)) = 0$, de sorte que l’homomorphisme $u$ est injectif. Le $A/p$-module non nul $T(A/p)$ est donc sans torsion. Cela implique que $T(A/p) \otimes_A \kappa(p)$ n’est pas nul (A, II, p. 117, cor. 1), ce qui contredit (iii').

Supposons le $A$-module $N$ de type fini, et prouvons que (iv) implique (iii). Soient $p$ un idéal premier de $A$ et $m$ un idéal maximal de $A$ contenant $p$. Il existe une chaîne saturée d’idéaux premiers de $A$ d’extrémités $\mathfrak{p}$ et $\mathfrak{m}$. La longueur $r$ de cette chaîne est inférieure à $\mathrm{ht}(\mathfrak{m})$; sous l’hypothèse (iv), on a donc
$$
\mathrm{Ext}_{A_{\mathfrak{m}}}^{n+r}(\kappa(\mathfrak{m}), N_{\mathfrak{m}}) = \mathrm{Ext}_{A}^{n+r}(A/\mathfrak{m}, N) \otimes_{A} A_{\mathfrak{m}} = 0 .
$$
Il résulte alors du lemme 3 du § 1, n° 7 qu’on a $\mathrm{Ext}_{A_{\mathfrak{p}}}^{n}(\kappa(\mathfrak{p}), N_{\mathfrak{p}}) = 0$, ce qui prouve (iii).

#### Remarque 5 {#ac-x-s3-n3-rem-5 .statement}

Soit $N$ un $A$-module de type fini ; la condition $\mathrm{Ext}_{A}^{n}(A/\mathfrak{m}, N) = 0$ pour tout idéal maximal $\mathfrak{m}$ de $A$ n’entraîne pas nécessairement $\mathrm{di}_{A}(N) < n$. Si par exemple l’anneau $A$ est local et n’est pas un anneau de Gorenstein (n° 7, déf. 1), on a $\mathrm{Ext}_{A}^{n}(A/\mathfrak{m}, A) = 0$ pour $n < \mathrm{prof}(A)$ mais $\mathrm{di}_{A}(A) = +\infty$.

### 4. Quotient par un élément simplifiable

Dans ce numéro, $A$ désigne un anneau et $x$ un élément de $A$ *simplifiable*.

Soient $M$ un $A$-module et $p : P \to M$ une résolution projective de $M$. D’après A, X, p. 101, cor. du th. 1, $H_{n}(P/xP)$ s’identifie à $\mathrm{Tor}_{n}^{A}(M, A/xA)$, donc est isomorphe à $M/xM$ si $n = 0$, à $\mathrm{Ker}(x_{M})$ si $n = 1$, et est nul sinon (*loc. cit.*, p. 102, exemple 1). Considérons les complexes de $(A/xA)$-modules $R$ et $R'$ tels que
$$
\begin{aligned}
R_{n} & = P_{n}/xP_{n} & R'_{n} & = 0 & \text{pour } n \geqslant 2, \\
R_{1} & = Z_{1}(P/xP) & R'_{1} & = (P_{1}/xP_{1})/R_{1}, \\
R_{n} & = 0 & R'_{n} & = P_{n}/xP_{n} & \text{pour } n \leqslant 0,
\end{aligned}
$$
et dont les différentielles se déduisent de celle de $P$. Les complexes $R(1)$ et $R'$ sont des résolutions gauches de $\mathrm{Ker}(x_{M})$ et $M/xM$ respectivement et on a une suite exacte de complexes
$$
0 \to R \to P/xP \to R' \to 0 .
$$

De manière analogue, soit $e : M \to E$ une résolution injective de $M$; notons $K$ le complexe $\mathrm{Ker}(x_{E})$. D’après A, X, p. 101, cor. du th. 1, $H_{n}(K)$ s’identifie à $\mathrm{Ext}_{A}^{n}(A/xA, M)$, donc est isomorphe à $\mathrm{Ker}(x_{M})$ si $n = 0$, à $M/xM$ si $n = 1$, et est nul sinon (*loc. cit.*, p. 102, exemple 1). On déduit de $E$ des complexes de $(A/xA)$-modules $S$ et $S'$ tels que
$$
\begin{aligned}
S^{n} & = K^{n} & {S'}^{n} & = 0 & \text{pour } n \leqslant 0, \\
S^{1} & = B^{1}(K) & {S'}^{1} & = K^{1}/S^{1}, \\
S^{n} & = 0 & {S'}^{n} & = K^{n} & \text{pour } n \geqslant 2.
\end{aligned}
$$
Les complexes $S$ et $S'(-1)$ sont des résolutions droites de $\mathrm{Ker}(x_{M})$ et $M/xM$ respectivement, et on a une suite exacte de complexes
$$
0 \to S \to \mathrm{Ker}(x_{E}) \to S' \to 0 .
$$

Soient $N$ un $(A/xA)$-module, et $e' : N \to E'$ une résolution injective de $N$. On déduit de la suite exacte (2) une suite exacte de complexes de $(A/xA)$-modules
$$
0 \to \mathrm{Homgr}_{A/xA}(R', E') \to \mathrm{Homgr}_{A/xA}(P/xP, E') \to \mathrm{Homgr}_{A/xA}(R, E') \to 0 .
$$

Considérons la suite exacte d’homologie associée à cette suite exacte. D’après A, X, p. 100, th. 1, on a pour tout entier $n \geqslant 0$ des isomorphismes

$$
H^n(\mathrm{Homgr}_{\Lambda/xA}(R', E')) \longrightarrow \mathrm{Ext}^n_{A/xA}(M/xM, N)
$$
$$
H^n(\mathrm{Homgr}_{\Lambda/xA}(P/xP, E')) \longrightarrow H^n(\mathrm{Homgr}_A(P, E')) \longrightarrow \mathrm{Ext}^n_A(M, N)
$$
$$
H^n(\mathrm{Homgr}_{A/xA}(R, E')) = H^{n-1}(\mathrm{Homgr}_{A/xA}(R(1), E')) \longrightarrow \mathrm{Ext}^{n-1}_{A/xA}(\mathrm{Ker}(x_M), N)
$$

on en déduit une suite exacte longue de $(A/xA)$-modules

$$
\ldots \longrightarrow \mathrm{Ext}^n_{A/xA}(M/xM, N) \longrightarrow \mathrm{Ext}^n_A(M, N) \longrightarrow \mathrm{Ext}^{n-1}_{A/xA}(\mathrm{Ker}(x_M), N)
$$
$$
\longrightarrow \mathrm{Ext}^{n+1}_{A/xA}(M/xM, N) \longrightarrow \mathrm{Ext}^{n+1}_A(M, N) \longrightarrow \ldots
$$

(4)

De même, soit $p' : P' \to N$ une résolution projective du $(\Lambda/xA)$-module $N$. On déduit de la suite exacte (3) une suite exacte de complexes de $(A/xA)$-modules

$0 \to \mathrm{Homgr}_{A/xA}(P', S) \longrightarrow \mathrm{Homgr}_{A/xA}(P', \mathrm{Ker}(x_E)) \longrightarrow \mathrm{Homgr}_{A/xA}(P', S') \to 0$.

Compte tenu de l’isomorphisme $\mathrm{Homgr}_{A/xA}(P', \mathrm{Ker}(x_E)) \longrightarrow \mathrm{Homgr}_A(P', E)$, la suite exacte d’homologie associée s’écrit

$$
\ldots \longrightarrow \mathrm{Ext}^n_{A/xA}(N, \mathrm{Ker}(x_M)) \longrightarrow \mathrm{Ext}^n_A(N, M) \longrightarrow \mathrm{Ext}^{n-1}_{A/xA}(N, M/xM)
$$
$$
\longrightarrow \mathrm{Ext}^{n+1}_{A/xA}(N, \mathrm{Ker}(x_M)) \longrightarrow \mathrm{Ext}^{n+1}_A(N, M) \longrightarrow \ldots
$$

(5)

Considérons enfin la suite exacte de complexes de $(A/xA)$-modules

$0 \to R \otimes_{A/xA} P' \longrightarrow (P/xP) \otimes_{A/xA} P' \longrightarrow R' \otimes_{A/xA} P' \to 0$

déduite de la suite exacte (2) ; compte tenu de l’isomorphisme $P \otimes_A P' \longrightarrow (P/xP) \otimes_{A/xA} P'$, la suite exacte d’homologie associée s’écrit

$$
\ldots \longrightarrow \mathrm{Tor}^A_n(M, N) \longrightarrow \mathrm{Tor}^{A/xA}_n(M/xM, N) \longrightarrow \mathrm{Tor}^{A/xA}_{n-2}(\mathrm{Ker}\ x_M, N)
$$
$$
\longrightarrow \mathrm{Tor}^A_{n-1}(M, N) \longrightarrow \mathrm{Tor}^{A/xA}_{n-1}(M/xM, N) \longrightarrow \ldots
$$

(6)

**Proposition 7.-** *Soient $A$ un anneau, $x$ un élément simplifiable de $A$, $M$ un $A$-module tel que l’homothétie $x_M$ soit injective, $N$ un $A$-module annulé par $x$, $n$ un entier. Les homomorphismes canoniques de $(A/xA)$-modules*

$$
\mathrm{Ext}^n_{A/xA}(M/xM, N) \longrightarrow \mathrm{Ext}^n_A(M, N),
$$
$$
\mathrm{Ext}^n_A(N, M) \longrightarrow \mathrm{Ext}^{n-1}_{A/xA}(N, M/xM),
$$
$$
\mathrm{Tor}^A_n(M, N) \longrightarrow \mathrm{Tor}^{A/xA}_n(M/xM, N)
$$

déduits des suites exactes (4), (5) et (6) sont des isomorphismes.

#### Corollaire {#ac-x-s3-n4-cor-1 .statement}

Soient $A$ un anneau local noethérien, $M$ un $A$-module de type fini et $J$ un idéal de $A$ engendré par une suite $(x_1, \ldots, x_r)$ d’éléments de $m_A$ qui est à la fois $A$-régulière et $M$-régulière. On a $\mathrm{dp}_{A/J}(M/JM) = \mathrm{dp}_A(M)$ et $\mathrm{di}_{A/J}(M/JM) = \mathrm{di}_A(M) - r$.

Il suffit de traiter le cas $r = 1$. Posons alors $x = x_1$. Les $A$-modules $\mathrm{Ext}^n_{A/xA}(M/xM, \kappa_A)$ et $\mathrm{Ext}^n_A(M, \kappa_A)$ sont isomorphes pour tout entier $n$ (prop. 7) ; l’égalité $\mathrm{dp}_{A/xA}(M/xM) = \mathrm{dp}_A(M)$ résulte de la prop. 4 du n° 3. De même, les $A$-modules $\mathrm{Ext}^{n-1}_{A/xA}(\kappa_A, M/xM)$ et $\mathrm{Ext}^n_A(\kappa_A, M)$ sont isomorphes pour tout entier $n$, et l’égalité $\mathrm{di}_{A/xA}(M/xM) = \mathrm{di}_A(M) - 1$ résulte de la prop. 6 du n° 3.

### 5. Profondeur et dimension projective

#### Théorème 1 (Auslander-Buchsbaum) {#ac-x-s3-thm-1 .statement}

Soient $A$ un anneau local noethérien et $M$ un $A$-module de type fini et de dimension projective finie. On a l’égalité

$$
\mathrm{dp}_A(M) + \mathrm{prof}_A(M) = \mathrm{prof}(A)
$$

Raisonnons par récurrence sur $\mathrm{dp}_A(M)$.

a) Si $\mathrm{dp}_A(M)$ est nul, $M$ est un $A$-module libre de type fini non nul ; sa profondeur est égale à $\mathrm{prof}(A)$ (§ 1, n° 1, remarque 4).

b) Supposons $\mathrm{dp}_A(M) = 1$ et choisissons une résolution projective minimale

$$
0 \to L_1 \xrightarrow{d_1} L_0 \xrightarrow{d_0} M \to 0
$$

de $M$ (n° 3, prop. 4, (iv)). Les $A$-modules $L_0$ et $L_1$ sont libres de type fini et non nuls, donc de profondeur $\mathrm{prof}(A)$ (§ 1, n° 1, remarque 4). L’application $1_{\kappa_A} \otimes d_1 : \kappa_A \otimes_A L_1 \to \kappa_A \otimes_A L_0$ est nulle, ce qui entraîne que $d_1$ appartient à $m_A \mathrm{Hom}_A(L_1, L_0)$. D’après la remarque 5 du § 1, n° 1, on a $\mathrm{prof}_A(M) = \mathrm{prof}(A) - 1$.

c) Supposons $\mathrm{dp}_A(M) > 1$. Choisissons une suite exacte

$$
0 \to N \to L \to M \to 0
$$

où $L$ est un $A$-module libre de type fini. On a alors $\mathrm{prof}_A(L) = \mathrm{prof}(A)$ (§ 1, n° 1, remarque 4), $\mathrm{dp}_A(N) = \mathrm{dp}_A(M) - 1$ (A, X, p. 135, cor. 2 c)), d’où $\mathrm{prof}_A(N) = \mathrm{prof}(A) - \mathrm{dp}_A(N)$ (hypothèse de récurrence), et en particulier $\mathrm{prof}_A(N) < \mathrm{prof}_A(L)$. D’après la prop. 1 du § 1, n° 1, on a alors $\mathrm{prof}_A(M) = \mathrm{prof}_A(N) - 1$, ce qui achève la démonstration.

Remarque. Compte tenu du cor. 2 de la prop. 4 (n° 3), le th. 1 appliqué au $A$-module $\kappa_A$ entraîne que l’on est dans l’un ou l’autre des cas suivants :

(i) on a $\mathrm{dp}_A(\kappa_A) = \mathrm{dh}(A) = +\infty$ ;
(ii) on a $\mathrm{dp}_A(\kappa_A) = \mathrm{dh}(A) = \mathrm{prof}(A) < +\infty$.

Nous verrons ultérieurement (§ 4, n° 2) que (ii) caractérise les anneaux locaux réguliers.

#### Corollaire 1 {#ac-x-s3-thm-1-cor-1 .statement}

Conservons les hypothèses du théorème 1.

a) On a $dp_A(M) \leq \operatorname{prof}(\Lambda)$. Pour qu’il y ait égalité, il faut et il suffit que l’idéal maximal $m_A$ soit associé à $M$.

b) On a $\operatorname{prof}_A(M) \leq \operatorname{prof}(\Lambda)$. Pour qu’il y ait égalité, il faut et il suffit que $M$ soit libre.

a) En effet, « $\operatorname{prof}_A(M) = 0$ » équivaut à « $m_A \in \operatorname{Ass}(A)$ » ($§ 1$, n° 1, remarque 2).

b) En effet, « $dp_A(M) = 0$ » équivaut à « $M$ est libre ».

COROLLAIRE 2.: Conservons les hypothèses du théorème 1 et supposons de plus que $A$ soit un anneau de Macaulay. Alors $dp_A(M)$ est la somme des deux entiers positifs $\dim(A) - \dim_A(M)$ et $\dim_A(M) - \operatorname{prof}(M)$.

En particulier, $dp_A(M)$ est alors supérieur à $\dim(A) - \dim_A(M)$, et il y a égalité si et seulement si $M$ est macaulayen.

COROLLAIRE 3. Soient $A$ un anneau noethérien, $M$ un $A$-module de type fini et de dimension projective finie, $i$ un entier $\geq 0$, $N$ un $A$-module de type fini et $F$ le support du $A$-module $\operatorname{Ext}_A^i(M, N)$ (resp. $\operatorname{Tor}_i^\Lambda(M, N)$). On a alors $\operatorname{prof}_F(\Lambda) \geq i$.

En effet, soit $p \in F$. On a $\operatorname{Ext}_A^i(M_p, N_p) \neq 0$ (resp. $\operatorname{Tor}_i^\Lambda(M_p, N_p) \neq 0$) d’après la prop. 2 du n° 2, donc $i \leq dp_{A_p}(M_p) \leq dp_A(M) < +\infty$ (n° 2, prop. 3). Le th. 1 entraîne $\operatorname{prof}(A_p) \geq i$. Par suite ($§ 1$, n° 5, prop. 8)

$$
\operatorname{prof}_F(\Lambda) = \inf_{p \in F} \operatorname{prof}(A_p) \geq i .
$$

Avec la terminologie du $§ 1$, n° 5, remarque 4, la conclusion du cor. 3 signifie que les modules $\operatorname{Ext}_\Lambda^i(M, N)$ et $\operatorname{Tor}_i^\Lambda(M, N)$ sont de grade $\geq i$. Elle entraîne que la codimension de leur support dans $\operatorname{Spec}(A)$ est $\geq i$ ($§ 1$, n° 7, prop. 12).

#### Corollaire 4 {#ac-x-s3-thm-1-cor-4 .statement}

Soient $A$ un anneau noethérien de Macaulay et $M$ un $A$-module de type fini et de dimension projective finie.

a) Soit $p \in \operatorname{Spec}(\Lambda)$; notons $\mathscr{C}(p)$ l’ensemble des composantes irréductibles de $\operatorname{Supp}(M)$ contenant $p$. On a

$$
\dim_{A_p}(M_p) - \operatorname{prof}_{A_p}(M_p) = dp_{A_p}(M_p) - \inf_{X \in \mathscr{C}(p)} \operatorname{codim}(X, \operatorname{Spec}(A)) .
$$

b) L’application $p \mapsto \dim_{A_p}(M_p) - \operatorname{prof}_{A_p}(M_p)$ de $\operatorname{Spec}(A)$ dans $\overline{\mathbf{Z}}$ est semi-continue supérieurement.

c) L’ensemble des idéaux premiers $p$ de $\Lambda$ tels que le $A_p$-module $M_p$ soit macaulayen est ouvert et dense dans $\operatorname{Spec}(\Lambda)$. Son intersection avec $\operatorname{Supp}(M)$ est dense dans $\operatorname{Supp}(M)$.

a) On peut supposer $p \in \operatorname{Supp}(M)$. Posons $\varphi(p) = \dim(A_p) - \dim_{A_p}(M_p)$. D’après le cor. 2 ci-dessus, on a

$$
\dim_{A_p}(M_p) - \operatorname{prof}_{A_p}(M_p) = dp_{A_p}(M_p) - \varphi(p) .
$$

Puisque $A$ est un anneau de Macaulay, on a

$$
\dim(A_p) = \operatorname{codim}(V(p), \operatorname{Spec}(A)) = \operatorname{codim}(V(p), X) + \operatorname{codim}(X, \operatorname{Spec}(A))
$$

$$
\dim_{\Lambda_p}(M_p) = \operatorname{codim}(V(p), \operatorname{Supp}(M)) = \sup_{X \in \mathcal{C}(p)} \operatorname{codim}(V(p), X)
$$

et par suite

$$
\varphi(p) = \inf_{X \in \mathcal{C}(p)} \operatorname{codim}(X, \operatorname{Spec}(A)) .
$$

b) Soit $p \in \operatorname{Spec}(A)$, et soit $F$ la réunion des composantes irréductibles de $\operatorname{Supp}(M)$ qui ne contiennent pas $p$. Pour tout élément $q$ de $\operatorname{Spec}(A) - F$, on a $\mathcal{C}(q) \subset \mathcal{C}(p)$, d’où $\varphi(q) \geq \varphi(p)$ d’après la formule ci-dessus. Par conséquent la fonction $\varphi$ est semi-continue inférieurement ; l’assertion b) résulte alors de la prop. 3 du n° 2.

c) Soit $U$ l’ensemble des éléments $p$ de $\operatorname{Spec}(A)$ tels que $M_p$ soit macaulayen. La condition $p \in U$ équivaut à $\dim(M_p) - \operatorname{prof}(M_p) \leq 0$, de sorte que $U$ est ouvert d’après b). Comme $U$ contient $\operatorname{Spec}(A) - \operatorname{Supp}(M)$, il suffit de prouver que $U \cap \operatorname{Supp}(M)$ est dense dans $\operatorname{Supp}(M)$. Pour tout idéal premier minimal $p$ de $\operatorname{Supp}(M)$, le $A_p$-module $M_p$ est de longueur finie (IV, § 2, n° 5, cor. 2 de la prop. 7 et § 1, n° 3, cor. 1 de la prop. 7), donc macaulayen ; par conséquent $U$ rencontre toutes les composantes irréductibles de $\operatorname{Supp}(M)$. On conclut à l’aide de la prop. 1 de II, § 4, n° 1.

### 6. Profondeur et dimension injective

#### Proposition 8 {#ac-x-s3-prop-8 .statement}

Soient $A$ un anneau noethérien, $M$ un $A$-module de type fini. On a $\dim_A(M) \leq \operatorname{di}_A(M)$.

Soit $r$ un entier positif inférieur à $\dim_A(M)$. Il existe une chaîne saturée d’idéaux premiers $p \subset p_1 \subset \ldots \subset p_{r-1} \subset q$ telle que $p$ soit un élément minimal du support de $M$; le $A_p$-module $M_p$ est alors de longueur finie, de sorte qu’on a $\operatorname{Hom}_{A_p}(\kappa(p), M_p) \neq 0$, donc $\operatorname{Ext}^r_{A_q}(\kappa(q), M_q) \neq 0$ (§ 1, n° 7, lemme 3), ce qui implique $\operatorname{di}_A(M) \geq r$ (n° 3, prop. 6).

#### Proposition 9 {#ac-x-s3-prop-9 .statement}

Soient $A$ un anneau local noethérien et $M$ un $A$-module non nul de type fini et de dimension injective finie. On a $\operatorname{di}_A(M) = \operatorname{prof}(A)$.

Posons $r = \operatorname{di}_A(M)$. On a $\operatorname{Ext}^i_A(\kappa_A, M) = 0$ pour $i > r$, donc $\operatorname{Ext}^r_A(\kappa_A, M) \neq 0$ d’après la prop. 6 du n° 3, (iv) $\Rightarrow$ (i). Soit $s$ la profondeur de $A$ et soit $(x_1, \ldots, x_s)$ une suite $A$-régulière d’éléments de $\mathfrak{m}_A$ (§ 1, n° 4, th. 2); posons $N = A/(x_1A + \ldots + x_sA)$. D’après l’exemple du n° 1, on a $\operatorname{dp}_A(N) = s$ et $\operatorname{Ext}^s_A(N, M) \neq 0$, donc $s \leq \operatorname{di}_A(M) = r$. Mais $N$ est de profondeur 0 (§ 1, n° 4, prop. 7), donc il existe une suite exacte de $A$-modules

$$
0 \to \kappa_A \to N \to N' \to 0 .
$$

On en déduit une suite exacte de modules d’extensions

$$
\operatorname{Ext}^r_A(N, M) \to \operatorname{Ext}^r_A(\kappa_A, M) \to \operatorname{Ext}^{r+1}_A(N', M) ;
$$

comme on a $\operatorname{Ext}^{r+1}_A(N', M) = 0$ et $\operatorname{Ext}^r_A(\kappa_A, M) \neq 0$, on obtient $\operatorname{Ext}^r_A(N, M) \neq 0$, d’où $r \leq \operatorname{dp}_A(N) = s$. En définitive, on a $r = s$, ce qui achève la démonstration.

### 7. Anneaux de Gorenstein

#### Définition 1 {#ac-x-s3-def-1 .statement}

On dit qu’un anneau $A$ est un anneau de Gorenstein s’il est noethérien et que le $A_m$-module $A_m$ est de dimension injective finie pour tout idéal maximal $m$ de $A$.

Pour qu’un anneau local noethérien $A$ soit un anneau de Gorenstein, il faut et il suffit que $\mathrm{di}_A(A)$ soit finie ; pour qu’un anneau noethérien $A$ soit un anneau de Gorenstein, il faut et il suffit qu’il en soit ainsi de $A_m$ pour tout idéal maximal $m$ de $A$.

#### Proposition 10 {#ac-x-s3-prop-10 .statement}

Soit $A$ un anneau de Gorenstein ; alors $A$ est un anneau de Macaulay, et satisfait à $\mathrm{di}_A(A) = \dim(A)$.

Pour tout idéal maximal $m$ de $A$, on a
$$
\begin{align*}
\dim(A_m) &\leq \mathrm{di}_{A_m}(A_m) & (\text{n}^\circ 6, \text{prop. 8}) \\
\mathrm{di}_{A_m}(A_m) &= \mathrm{prof}(A_m) & (\text{n}^\circ 6, \text{prop. 9}) \\
\mathrm{prof}(A_m) &\leq \dim(A_m) & (§ 1, \text{n}^\circ 4, \text{cor. 2 du th. 2}) ;
\end{align*}
$$
il en résulte que $A$ est un anneau de Macaulay, et que $\mathrm{di}_A(A) = \dim(A)$ par passage à la borne supérieure (n° 2, prop. 3).

Ainsi les anneaux noethériens $A$ tels que $\mathrm{di}_A(A)$ soit finie sont les anneaux de Gorenstein de dimension finie (prop. 3 du n° 2), et les anneaux noethériens tels que le $A$-module $A$ soit injectif sont les anneaux de Gorenstein artiniens.

Exemples. 1) Pour toute partie multiplicative $S$ d’un anneau de Gorenstein $A$, l’anneau de fractions $S^{-1}A$ est un anneau de Gorenstein : en effet, soit $q$ un idéal maximal de $S^{-1}A$ ; il est de la forme $S^{-1}p$, où $p$ est un idéal premier de $A$ ne rencontrant pas $S$. Soit $m$ un idéal maximal de $A$ contenant $p$ ; alors l’anneau $B = (S^{-1}A)_q$ est isomorphe à $A_p$ (II, § 2, n° 5, prop. 11), donc à un anneau de fractions de $A_m$, et par suite satisfait à $\mathrm{di}_B(B) < +\infty$ (n° 2, cor. 1 de la prop. 3).

2) Soit $A$ un anneau de Gorenstein et soit $J$ un idéal de $A$, engendré par une suite $A$-régulière $x$. L’anneau quotient $A/J$ est un anneau de Gorenstein : en effet, pour tout idéal maximal $m$ de $A$ contenant $J$, l’image dans $A_m$ de la suite $x$ est $A_m$-régulière et engendre l’idéal $J_m$, de sorte que $A_m/J_m$ est un anneau de Gorenstein d’après le cor. de la prop. 7 (n° 4).

3) Soient $A$ un anneau local noethérien, $J$ un idéal de $A$ engendré par une suite $A$-régulière d’éléments de $m_A$. Si $A/J$ est un anneau de Gorenstein, il en est de même de $A$ (n° 4, cor. de la prop. 7).

4) Soit $A$ un anneau local noethérien régulier ; alors $A$ est un anneau de Gorenstein. En effet, soit $x$ un système de coordonnées de $A$ (VIII, § 5, n° 1, déf. 1). La suite $x$ est $A$-régulière (*loc. cit.*, n° 2, th. 1) et engendre l’idéal $m_A$ ; on peut donc appliquer l’exemple 3.

5) Tout anneau quotient d’un anneau principal est un anneau de Gorenstein (exemple 2). En particulier, toute algèbre monogène sur un corps est un anneau de Gorenstein.

#### Lemme 1 {#ac-x-s3-lem-1 .statement}

Soit $A$ un anneau local artinien. Les conditions suivantes sont équivalentes :

(i) $A$ est un anneau de Gorenstein ;
(ii) le $A$-module $A$ est injectif ;
(iii) le $\kappa_A$-espace vectoriel $\mathrm{Hom}_A(\kappa_A, A)$ est de dimension 1.

Rappelons (A, VIII, p. 3.5) que $A$ possède un idéal non nul minimal ; un tel idéal est un module simple, donc isomorphe à $\kappa_A$. Le $\kappa_A$-espace vectoriel $\mathrm{Hom}_A(\kappa_A, A)$ est donc non nul ; dire qu’il est de dimension 1 signifie que $A$ contient un seul idéal non nul minimal, qui est donc le socle de $A$ (A, VIII, § 4, n° 6).

L’équivalence de (i) et (ii) a été démontrée après la prop. 10. Supposons le $A$-module $A$ injectif. Soient $x$ et $y$ deux éléments non nuls de $A$ annulés par $m_A$. Il existe une unique application $A$-linéaire $\varphi : Ax \to A$ telle que $\varphi(x) = y$ ; comme $A$ est injectif, elle s’étend en un endomorphisme de $A$, ce qui entraîne que $y$ appartient à $Ax$, d’où (iii).

Supposons inversement que $\mathrm{Hom}_A(\kappa_A, A)$ soit de dimension 1. Soit $M$ un $A$-module de type fini ; il est de longueur finie, donc possède une suite de composition dont les quotients sont isomorphes à $\kappa_A$. On en déduit par récurrence sur la longueur de $M$ l’inégalité $\mathrm{long}_A(\mathrm{Hom}_A(M, A)) \leqslant \mathrm{long}_A(M)$. Dans la suite exacte des modules d’extensions

$$
0 \to \mathrm{Hom}_A(\kappa_A, A) \to \mathrm{Hom}_A(A, A) \xrightarrow{\alpha} \mathrm{Hom}_A(m_A, A) \to \mathrm{Ext}_A^1(\kappa_A, A) \to 0 ,
$$

on a donc $\mathrm{long}_A(\mathrm{Hom}_A(m_A, A)) \leqslant \mathrm{long}_A(m_A) = \mathrm{long}(A) - 1 = \mathrm{long}_A(\mathrm{Im}\, \alpha)$. Par suite $\alpha$ est surjective, $\mathrm{Ext}_A^1(\kappa_A, A)$ est nul et le $A$-module $A$ est injectif (n° 3, prop. 4).

#### Lemme 2 {#ac-x-s3-lem-2 .statement}

Soit $A$ un anneau local noethérien tel que $\mathrm{di}_A(A) = +\infty$. On a $\mathrm{Ext}_A^i(\kappa_A, A) \neq 0$ pour tout entier $i \geqslant \dim(A)$.

Raisonnons par récurrence sur $\dim(A)$. Lorsque $\dim(A) = 0$, $m_A$ est l’unique idéal premier de $A$ et l’assertion résulte de la prop. 6 du n° 3. Supposons donc $\dim(A) > 0$ et soit $p$ un idéal premier de $A$ distinct de $m_A$ ; on a alors $\dim(A_p) < \dim(A)$. Si $\mathrm{di}_{A_p}(A_p) = +\infty$, l’hypothèse de récurrence implique $\mathrm{Ext}_{A_p}^j(\kappa(p), A_p) \neq 0$ pour tout entier $j \geqslant \dim(A_p)$ ; d’après le lemme 3 du § 1, n° 7, cela implique $\mathrm{Ext}_A^i(\kappa_A, A) \neq 0$ pour tout entier $i \geqslant \dim(A_p) + \dim(A/p)$, et en particulier pour $i \geqslant \dim(A)$ (VIII, § 1, n° 3, prop. 8, b)).

Il nous reste à traiter le cas où $\mathrm{di}_A(A)$ est infinie mais où la dimension injective de $A_p$ est finie pour tout idéal premier $p$ de $A$ distinct de $m_A$. Pour un tel idéal, on a dans ce cas, d’après la prop. 10, $\mathrm{di}_{A_p}(A_p) = \dim(A_p) < \dim(A)$, donc $\mathrm{Ext}_{A_p}^i(\kappa(p), A_p) = 0$ pour $i \geqslant \dim(A)$. Puisque $\mathrm{di}_A(A)$ est infinie, la prop. 6 du n° 3 impose alors $\mathrm{Ext}_A^i(\kappa_A, A) \neq 0$ pour tout entier $i \geqslant \dim(A)$.

Théorème 2 (Bass). Soit $A$ un anneau local noethérien ; posons $d = \dim(A)$. Soient $x = (x_1, \ldots, x_d)$ une suite sécante maximale d’éléments de $m_A$, et $x$ l’idéal qu’elle engendre. Les conditions suivantes sont équivalentes :

(i) $\Lambda$ est un anneau de Gorenstein ;
(ii) on a $\operatorname{di}_\Lambda(A) = d$;
(iii) il existe un entier $i > d$ tel que $\operatorname{Ext}^i_\Lambda(\kappa_A, A) = 0$;
(iv) on a $\operatorname{Ext}^i_\Lambda(\kappa_A, A) = 0$ pour $i < d$ et le $\kappa_A$-espace vectoriel $\operatorname{Ext}^d_\Lambda(\kappa_A, A)$ est de dimension 1 ;
(v) l’anneau $A$ est de Macaulay et le $\kappa_A$-espace vectoriel $\operatorname{Hom}_A(\kappa_A, A/x)$ est de dimension 1 ;
(vi) la suite $x$ est $A$-régulière et le $\kappa_A$-espace vectoriel $\operatorname{Hom}_A(\kappa_A, A/x)$ est de dimension 1.

L’équivalence de (i), (ii) et (iii) résulte du lemme 2 et de la prop. 10. Si $\operatorname{Ext}^i_\Lambda(\kappa_A, A)$ est nul pour tout entier $i < d$, l’anneau $A$ est de Macaulay (§ 2, n° 3, prop. 3) ; si l’anneau $A$ est de Macaulay, la suite $x$ est $A$-régulière (*loc. cit.*, th. 1) ; si la suite $x$ est $A$-régulière, on a $\operatorname{Ext}^i_\Lambda(\kappa_A, A) = 0$ pour $i < d$ et les $\kappa_A$-espaces vectoriels $\operatorname{Ext}^d_\Lambda(\kappa_A, A)$ et $\operatorname{Hom}_A(\kappa_A, A/x)$ sont isomorphes (A, X, p. 166, prop. 9). Cela prouve l’équivalence des conditions (iv), (v) et (vi).

Prouvons que (i) implique (v) : si $A$ est un anneau de Gorenstein, c’est un anneau de Macaulay (prop. 10). La suite $x$ est alors $A$-régulière (§ 2, n° 3, prop. 4), donc $A/x$ est un anneau artinien de Gorenstein (exemple 2), de sorte que le $\kappa_A$-espace vectoriel $\operatorname{Hom}_A(\kappa_A, A/x)$ est de dimension 1.

Prouvons enfin que (vi) implique (i) : sous l’hypothèse (vi), l’anneau $A/x$ est un anneau de Gorenstein (lemme 1), donc $A$ est un anneau de Gorenstein (exemple 3).

#### Corollaire {#ac-x-s3-n7-cor-1 .statement}

*Soit $\Lambda$ un anneau local noethérien de dimension d. Le $\Lambda$-module $\operatorname{Ext}^d_\Lambda(\kappa_A, A)$ n’est pas nul.*

Cela résulte du th. 2 si $\Lambda$ est un anneau de Gorenstein et du lemme 2 sinon.

#### Proposition 11 {#ac-x-s3-prop-11 .statement}

*Soit $A$ un anneau noethérien. Les conditions suivantes sont équivalentes :*

(i) $A$ est un anneau de Gorenstein ;
(ii) pour tout idéal premier $p$ de $A$, le $\kappa(p)$-espace vectoriel $\operatorname{Ext}^i_{A_p}(\kappa(p), A_p)$ est nul pour $i \neq \operatorname{ht}(p)$ et de dimension 1 pour $i = \operatorname{ht}(p)$.
(iii) pour tout idéal maximal $m$ de $A$, il existe un entier $i > \operatorname{ht}(m)$ tel que $\operatorname{Ext}^i_{A_m}(A/m, A_m) = 0$.

(i) $\Rightarrow$ (ii) : cela résulte du th. 2 appliqué à l’anneau local de Gorenstein $A_p$ (exemple 1).
(ii) $\Rightarrow$ (iii) : c’est trivial.
(iii) $\Rightarrow$ (i) : sous l’hypothèse (iii), $A_m$ est un anneau de Gorenstein pour tout idéal maximal $m$ de $A$ (th. 2), et $A$ est de Gorenstein.

### 8. Anneaux de Gorenstein et algèbres plates

Proposition 12. Soit $\rho : A \to B$ un homomorphisme local d’anneaux locaux noethériens, faisant de $B$ un $A$-module plat. Les conditions suivantes sont équivalentes :

(i) $B$ est un anneau de Gorenstein ;
(ii) $A$ et $\kappa_A \otimes_A B$ sont des anneaux de Gorenstein.

Traitons d’abord le cas où les anneaux $A$ et $B$ sont artiniens. Notons $C$ l’anneau local $\kappa_A \otimes_A B$; son corps résiduel $\kappa_C$ s’identifie à $\kappa_B$. Puisque $B$ est plat sur $A$, le $B$-module $\mathrm{Hom}_B(C, B)$ est isomorphe à $\mathrm{Hom}_A(\kappa_A, A) \otimes_A B$ (I, § 2, n° 10, prop. 11), donc à $\mathrm{Hom}_A(\kappa_A, A) \otimes_{\kappa_A} C$. On en déduit une suite d’isomorphismes

$$
\mathrm{Hom}_B(\kappa_B, B) \longrightarrow \mathrm{Hom}_C(\kappa_C, \mathrm{Hom}_B(C, B)) \longrightarrow \mathrm{Hom}_C(\kappa_C, \mathrm{Hom}_A(\kappa_A, A) \otimes_{\kappa_A} C)
$$
$$
\longrightarrow \mathrm{Hom}_A(\kappa_A, A) \otimes_{\kappa_A} \mathrm{Hom}_C(\kappa_C, C) .
$$

En particulier, on a $[\mathrm{Hom}_B(\kappa_B, B) : \kappa_B] = [\mathrm{Hom}_A(\kappa_A, A) : \kappa_A] \ [\mathrm{Hom}_C(\kappa_C, C) : \kappa_C]$
et la proposition résulte alors du lemme 1 du n° 7.

Passons au cas général. Si l’on remplace dans l’énoncé le mot « Gorenstein » par le mot « Macaulay », la proposition est un cas particulier de la prop. 10 du § 2, n° 7. On peut donc supposer que les anneaux $A$, $B$ et $C = \kappa_A \otimes_A B$ sont de Macaulay. Le $B$-module $C$ est macaulayen ($§ 2$, n° 1, exemple 4). Posons $r = \dim(A)$, $s = \dim(C)$. Il existe une suite $A$-régulière $(x_1, \ldots, x_r)$ d’éléments de $m_A$ et une suite $(y_1, \ldots, y_s)$ d’éléments de $m_B$ régulière pour le $B$-module $C$ ($§ 2$, n° 3, prop. 3) ; notons $x$ l’idéal de $A$ et $\mathfrak{y}$ l’idéal de $B$ qu’elles engendrent respectivement. La suite $(y_1, \ldots, y_s, \rho(x_1), \ldots, \rho(x_r))$ est $B$-régulière ($§ 1$, n° 6, prop. 11) et le $A$-module $B/\mathfrak{y}$ est plat (*loc. cit.*, prop. 10). L’homomorphisme de $A/x$ dans $B/(xB + \mathfrak{y})$ déduit de $\rho$ par passage aux quotients fait donc de $B/(xB + \mathfrak{y})$ un $(A/x)$-module plat et l’anneau $\kappa_{A/x} \otimes_{A/x} B/(xB + \mathfrak{y})$ est isomorphe à $C/\mathfrak{y}C$. La proposition résulte ainsi de la première partie de la démonstration, compte tenu de l’exemple 3 du n° 7.

#### Corollaire 1 {#ac-x-s3-prop-11-cor-1 .statement}

Soit $\rho : A \to B$ un homomorphisme d’anneaux noethériens faisant de $B$ un $A$-module plat. Les conditions suivantes sont équivalentes :

(i) $B$ est un anneau de Gorenstein ;
(ii) (resp. (iii)) pour tout idéal premier (resp. maximal) $q$ de $B$, les anneaux $A_{\rho^{-1}(q)}$ et $\kappa(\rho^{-1}(q)) \otimes_A B$ sont de Gorenstein.

Si de plus $B$ est un $A$-module fidèlement plat, ces conditions entraînent que $A$ est un anneau de Gorenstein.

Soit $q$ un idéal premier de $B$; posons $p = \rho^{-1}(q)$. L’anneau $B_q$, isomorphe à un anneau de fractions de $B_p$, est plat sur $A_p$. Pour que $B_q$ soit un anneau de Gorenstein, il faut et il suffit que les anneaux $A_p$ et $\kappa(p) \otimes_{A_p} B_q$ le soient (prop. 12).

(i) $\Rightarrow$ (ii) : soient $q$ un idéal premier de $B$ et $p = \rho^{-1}(q)$. Si $B$ est un anneau de Gorenstein, il en est de même de $B_q$, donc de $A_p$ et $\kappa(p) \otimes_{A_p} B_q$ d’après ce qui précède. D’après la remarque du $§ 2$, n° 6, l’anneau local de $\kappa(p) \otimes_A B$ en un idéal premier quelconque est alors un anneau de Gorenstein, ce qui entraîne que $\kappa(p) \otimes_A B$ est un anneau de Gorenstein, d’où (ii).

(ii) $\Rightarrow$ (iii) : c’est clair.

(iii) $\Rightarrow$ (i) : pour tout idéal maximal $n$ de $B$, il résulte du début de la démonstration (appliqué avec $q = n$) que $B_n$ est un anneau de Gorenstein, d’où (i).

Si $B$ est un $A$-module fidèlement plat, l’application $^a\rho : \mathrm{Spec}(B) \longrightarrow \mathrm{Spec}(\Lambda)$ est surjective (II, § 2, n° 5, cor. 4 de la prop. 11), d’où la dernière assertion.

#### Corollaire 2 {#ac-x-s3-prop-11-cor-2 .statement}

Soient $A$ un anneau noethérien, $J$ un idéal de $A$, $\hat{A}$ le séparé complété de $A$ pour la topologie $J$-adique. Considérons les conditions suivantes :

(i) $A$ est un anneau de Gorenstein ;
(ii) $\hat{A}$ est un anneau de Gorenstein ;
(iii) pour tout idéal maximal $m$ de $A$ contenant $J$, $A_m$ est un anneau de Gorenstein ;
(iv) pour tout idéal premier $p$ de $A$ tel que $p + J \neq A$, $A_p$ et $\kappa(p) \otimes_A \hat{A}$ sont des anneaux de Gorenstein.

Les conditions (ii) à (iv) sont équivalentes, et sont entraînées par (i). Lorsque l’idéal $J$ est contenu dans le radical de $A$, les conditions (i) à (iv) sont équivalentes.

On déduit ce corollaire du cor. 1 de la même façon que l’on a déduit de la prop. 9 du § 2, n° 7, son corollaire 4 : il suffit dans la démonstration de remplacer le mot « Macaulay » par le mot « Gorenstein ».

#### Corollaire 3 {#ac-x-s3-prop-11-cor-3 .statement}

Soient $A$ un anneau de Gorenstein et $(T_i)_{i \in I}$ une famille finie d’indéterminées. Les anneaux $A[(T_i)_{i \in I}]$ et $A[[T_i]_{i \in I}]$ sont des anneaux de Gorenstein.

Pour tout corps $k$, l’anneau $k[T]$ est de Gorenstein (n° 7, exemple 5) ; par ailleurs l’anneau $A[T]$ est noethérien. C’est donc un anneau de Gorenstein (cor. 1). On en déduit par récurrence sur $\mathrm{Card}(I)$ que $A[(T_i)_{i \in I}]$ est un anneau de Gorenstein ; puis on applique le cor. 2.

## EXERCICES {#ac-x-s3-exercises}

See the [exercises for § 3](exercises/s3/).
