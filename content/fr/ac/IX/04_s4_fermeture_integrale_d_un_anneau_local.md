---
book: ac
book_title: Commutative Algebra
chapter: IX
chapter_title: ANNEAUX LOCAUX NOETHÉRIENS COMPLETS
section: 4
section_title: Fermeture intégrale d'un anneau local complet
lang: fr
source: ac-viii-ix-fr
book_pages: AC IX.78-AC IX.84
pdf_pages: 0142-0148, 0190-0196
extraction: ocr
subsections:
    - "no": 1
      title: Anneaux japonais
      page: 30
      pdf_page: 142
    - "no": 2
      title: Théorème de Nagata
      page: 0
      pdf_page: 143
    - "no": 3
      title: Quelques lemmes
      page: 33
      pdf_page: 145
    - "no": 4
      title: Anneaux de Nagata
      page: 0
      pdf_page: 146
statements: 25
exercises: 32
content_sha256: cb927004891b75f7bec7495a3fa16bafa8f97a5ce54d872780a5fd5e2ad7a98d
---

## § 4. FERMETURE INTÉGRALE D’UN ANNEAU LOCAL COMPLET

### 1. Anneaux japonais

#### Définition 1 {#ac-ix-s4-def-1 .statement}

Soit $A$ un anneau noethérien intègre. On dit que $A$ est japonais si la fermeture intégrale de $A$ dans toute extension finie de son corps des fractions est une $A$-algèbre finie.

#### Remarque 1 {#ac-ix-s4-n1-rem-1 .statement}

Il revient au même de dire que $A$ satisfait à la condition suivante : toute $A$-algèbre intègre $B$ entière sur $A$, contenue dans une extension de type fini du corps des fractions $K$ de $A$, est une $A$-algèbre finie. En effet, le corps des fractions $L$ de $B$ est une extension algébrique de $K$, donc est de degré fini sur $K$ (A, V, p. 112, cor. 1 de la prop. 17). La $A$-algèbre $B$ est contenue dans la fermeture intégrale de $A$ dans $L$, et est donc finie si cette dernière est finie.

#### Exemple {#ac-ix-s4-n1-exa-1 .statement}

Toute algèbre intègre de type fini sur un corps est un anneau japonais (V, § 3, no 2, th. 2).

#### Proposition 1 {#ac-ix-s4-prop-1 .statement}

Soient A un anneau noethérien intègre, K son corps des fractions. Supposons que pour toute extension finie radicielle L de K, la fermeture intégrale de A dans L soit une A-algèbre finie. Alors l’anneau A est japonais.

Soit E une extension finie de K. Soient N une extension finie quasi-galoisienne de K contenant E (A, V, p. 54, cor. 1), et L le corps des invariants du groupe des K-auto-morphismes de N. Alors (A, V, p. 73, prop. 13), L est une extension radicielle de K et N est une extension séparable de L. La fermeture intégrale B de A dans L est donc par hypothèse une A-algèbre finie ; la fermeture intégrale C de B dans N est une B-algèbre finie (V, § 1, no 6, cor. 1 à la prop. 18), donc une A-algèbre finie. La fermeture intégrale de A dans E est contenue dans C, donc est une A-algèbre finie puisque A est noethérien.

#### Corollaire {#ac-ix-s4-n1-cor-1 .statement}

Supposons le corps K parfait (par exemple de caractéristique 0). Alors A est japonais si et seulement si sa clôture intégrale est une A-algèbre finie.

#### Proposition 2 {#ac-ix-s4-prop-2 .statement}

Soient B un anneau noethérien intègre et A un sous-anneau noethérien de B, tel que B soit une A-algèbre finie. Pour que A soit japonais, il faut et il suffit que B soit japonais.

Notons K (resp. L) le corps des fractions de A (resp. B). Supposons d’abord A japonais, et soit M une extension finie de L. Notons C la fermeture intégrale de B dans M. D’après V, § 1, no 1, prop. 6, C est la fermeture intégrale de A dans M, donc est une A-algèbre finie puisque M est une extension finie de K et que A est japonais. A fortiori, C est une B-algèbre finie. Ceci prouve que B est japonais.

Inversement, supposons B japonais et soit N une extension finie de K. Notons D la fermeture intégrale de A dans N. Soit E une extension de K composée de L et N ; comme B est japonais, la fermeture intégrale D’ de B dans E est une B-algèbre finie, donc une A-algèbre finie ; le A-module D qui est un sous-module de D’ est donc de type fini, ce qui entraîne que A est japonais.

### 2. Théorème de Nagata

#### Théorème 1 (Tate) {#ac-ix-s4-thm-1 .statement}

Soient A un anneau noethérien intégralement clos, a un élément de A. On suppose que l’idéal $aA$ est premier, que l’anneau $A/aA$ est japonais et que A est complet pour la topologie $aA$-adique. Alors l’anneau A est japonais.

a) Soit K le corps des fractions de A. L’assertion étant triviale lorsque K est de caractéristique 0 (n° 1, corollaire de la prop. 1), on peut supposer K de caractéristique $p > 0$. On peut aussi supposer $a \neq 0$.

Soient L une extension finie radicielle de K et q une puissance de p telle que $L \subset K^{1/q}$. Posons $x = a^{1/q}$ et $M = L(x)$. D’après la prop. 1 du n° 1, il suffit de démontrer que la fermeture intégrale B de A dans M est une A-algèbre finie.

b) Démontrons d’abord que l’idéal $xB$ est l’unique idéal premier de B au-dessus de $aA$. Il existe en effet au moins un idéal premier de B au-dessus de $aA$ (V, § 2, n° 1, th. 1). Soit q l’un de ces idéaux. On a $x^q = a \in q$, d’où $xB \subset q$ puisque q est premier. Inversement, soit y un élément de q ; l’élément $y^q$ de K est entier sur A, donc appartient à A puisque A est intégralement clos. Puisque $q \cap A = aA$, il existe un élément $\alpha$ de A tel que $y^q = a\alpha = x^q\alpha$. Par conséquent l’élément $y/x$ de M est entier sur A, donc appartient à B ; ainsi on a $y \in xB$, d’où $q = xB$, ce qui démontre notre assertion.

c) Il en résulte que l’anneau $B_{xB}$ est la fermeture intégrale dans M de l’anneau $A_{aA}$ (V, § 1, n° 5, prop. 16 et § 2, n° 1, prop. 2). D’après VI, § 3, n° 6, prop. 9, $A_{aA}$ est un anneau de valuation discrète ; on déduit alors du théorème de Krull-Akizuki (VII, § 2, n° 5, prop. 5) que le corps $\kappa(xB)$ est une extension finie de $\kappa(aA)$ et que $B_{xB}$ est noethérien.

d) L’anneau $B/xB$ est entier sur l’anneau japonais $A/aA$ et son corps des fractions est une extension finie du corps des fractions de ce dernier. Par conséquent, $B/xB$ est un $(A/aA)$-module de type fini. Pour tout entier $i \geq 0$, il en est de même du module $x^iB/x^{i+1}B$ ; par suite le $(A/aA)$-module $B/aB$ possède une suite de composition de longueur q dont les quotients sont des $(A/aA)$-modules de type fini, donc est lui-même un $(A/aA)$-module de type fini.

e) Munissons l’anneau A de la filtration $(aA)$-adique et l’anneau B de la filtration $(aB)$-adique. Alors A est complet par hypothèse ; comme $B_{xB}$ est intègre et noethérien, la filtration $aB_{xB}$-adique de $B_{xB}$ est séparée (III, § 3, n° 2, corollaire à la prop. 5) ; par suite on a $\bigcap a^nB \subset \bigcap a^nB_{xB} = \{0\}$, et la filtration $aB$-adique de B est séparée ; le gr(A)-module gr(B) est engendré par gr_0(B), donc est de type fini d’après d). Il résulte alors de III, § 2, n° 9, cor. 1 à la prop. 12, que B est un A-module de type fini, ce qui achève la démonstration.

#### Corollaire {#ac-ix-s4-n2-cor-1 .statement}

Soient R un anneau noethérien intègre et n un entier. Si R est japonais, l’anneau $R[[T_1, ..., T_n]]$ est japonais.

Raisonnant par récurrence, on peut supposer $n = 1$. Notons S la clôture intégrale de R ; si R est japonais, S est une algèbre finie sur R, donc un anneau japonais (n° 1, prop. 2). L’anneau S[[T]] est noethérien et intégralement clos (V, § 1, n° 4, prop. 14) ; appliquant le th. 1 à $A = S[[T]]$ et $a = T$, on en déduit que S[[T]] est japonais. Par conséquent R[[T]] est japonais (n° 1, prop. 2).

#### Théorème 2 (Nagata) {#ac-ix-s4-thm-2 .statement}

Tout anneau A local noethérien intègre et complet est japonais.

D’après le th. 3 du § 2, n° 5 et le th. 2 du § 3, n° 3, il existe un entier $n \geq 0$, un anneau R qui est un corps ou un anneau de valuation discrète de corps des fractions de caractéristique 0, et un sous-anneau B de A, isomorphe à R[[T₁, ..., Tₙ]] et tel que A soit une B-algèbre finie. Alors R est japonais (n° 1, exemple et corollaire de la prop. 1), donc B est japonais (corollaire au th. 1), et A est japonais (n° 1, prop. 2).

#### Corollaire {#ac-ix-s4-n2-cor-2 .statement}

Soit A un anneau semi-local noethérien dont le complété est réduit. Alors la fermeture intégrale A' de A dans son anneau total des fractions R est une A-algèbre finie.

Supposons d’abord A local et complet, et soient p₁, ..., pₙ les idéaux premiers minimaux (distincts) de A ; pour i = 1, ..., n, notons Kᵢ le corps des fractions de A/pᵢ et Aᵢ' la clôture intégrale de A/pᵢ. Comme A est réduit, R est le produit des anneaux Kᵢ et A' le produit des anneaux Aᵢ' (V, § 1, n° 2, cor. 1 à la prop. 9). Puisque les anneaux locaux A/pᵢ sont intègres et complets, ils sont japonais (th. 2), de sorte que chaque Aᵢ' est une A-algèbre finie, et A' est une A-algèbre finie.

Si A est semi-local et complet, il est isomorphe à un produit fini d’anneaux locaux complets (III, § 2, n° 13, corollaire à la prop. 19), et on conclut aussitôt d’après ce qui précède.

Passons au cas général et notons que le complété Â de A est un anneau semi-local, complet, noethérien et fidèlement plat sur A (III, loc. cit., § 3, n° 4, corollaire de la prop. 8 et § 3, n° 5, prop. 9). Soit S l’ensemble des éléments non diviseurs de zéro de A ; on a R = S⁻¹A. Puisque Â est plat sur A, les éléments de S sont non diviseurs de zéro dans Â, et S⁻¹Â s’identifie à un sous-anneau de l’anneau total des fractions T de Â. Toujours puisque Â est plat sur A, l’anneau A' ⊗_A Â s’identifie à un sous-anneau de R ⊗_A Â = S⁻¹Â, donc aussi à un sous-anneau de T entier sur Â. D’après la première partie de la démonstration, A' ⊗_A Â est donc un Â-module de type fini ; par suite, A' est un A-module de type fini (I, § 3, n° 6, prop. 11).

Rappelons (A, V, p. 114, déf. 1) qu’une algèbre E sur un corps K est dite séparable si l’anneau L ⊗_K E est réduit pour toute extension L de K ; il suffit qu’il en soit ainsi pour toute extension finie de K. La proposition suivante généralise le th. 2 :

#### Proposition 3 {#ac-ix-s4-prop-3 .statement}

Soient A un anneau semi-local noethérien intègre, K son corps des fractions. Si la K-algèbre K ⊗_A Â est séparable, l’anneau A est japonais.

Soient L une extension finie de K et B la fermeture intégrale de A dans L. Soit F une partie finie de B telle que L = K[F] (V, § 1, n° 5, cor. 2 à la prop. 16) ; notons C la A-algèbre (finie) engendrée par F. Puisque L est le corps des fractions de C, l’anneau B est la clôture intégrale de C (V, § 1, n° 1, prop. 6) et il suffit de prouver que B est une C-algèbre finie. Or, C est un anneau semi-local noethérien (IV, § 2, n° 5, cor. 3 à la prop. 9 ) ; son complété s’identifie à C ⊗_A Â (III, § 3, n° 4, th. 3 (ii)), donc aussi à un sous-anneau de l’anneau réduit L ⊗_A Â = L ⊗_K (K ⊗_A Â) et par suite est réduit. La prop. 3 résulte donc du corollaire au th. 2.

### 3. Quelques lemmes

#### Lemme 1 {#ac-ix-s4-lem-1 .statement}

Soient A un anneau semi-local noethérien et B une A-algèbre finie. Alors l’anneau B est semi-local et noethérien ; soient m₁, ..., mₙ ses idéaux maximaux.

L’homomorphisme canonique de B dans $\prod_{i=1}^n \hat{B}_{m_i}$ se prolonge en un isomorphisme de $\hat{A} \otimes_A B$ sur $\prod_{i=1}^n \hat{B}_{m_i}$.

D’après IV, § 2, no 5, cor. 3 à la prop. 9, l’anneau B est semi-local et $m_A B$ en est un idéal de définition. D’après III, § 3, no 4, th. 3, (ii), l’anneau $\hat{A} \otimes_A B$ est le complété de B pour la topologie définie par son radical ; on applique alors III, § 2, no 13, corollaire à la prop. 19.

#### Lemme 2 {#ac-ix-s4-lem-2 .statement}

Soient A un anneau noethérien et M un A-module. L’application canonique de M dans le produit $\prod_{p \in \mathrm{Ass}(M)} M_p$ est injective.

Soit en effet m un élément non nul de M ; alors Ann(m) est contenu dans un idéal premier p de A associé à M (IV, § 1, no 1, prop. 2), et l’image de m dans $M_p$ est non nulle (II, § 2, no 2, prop. 4).

#### Lemme 3 {#ac-ix-s4-lem-3 .statement}

Soient A un anneau noethérien, x un élément de A, M un A-module de type fini, et p un idéal premier de A associé à M. On suppose que l’homothétie $x_M$ est injective. Soit q un idéal premier de A, minimal parmi ceux qui contiennent p + xA. Alors q est associé au A-module $M/xM$.

Notons N le sous-module de M formé des éléments m tels que $pm = 0$. On a $N \cap xM = xN$ ; en effet, si un élément m de M est tel que $pxm = 0$, on a $pm = 0$ puisque $x_M$ est injective, donc $m \in N$. Par conséquent, le A-module $N/xN$ est isomorphe au sous-module $(N + xM)/xM$ de $M/xM$, et il suffit de démontrer que q est associé à $N/xN$. Puisque p est associé à M, il existe un élément m de M tel que $p = \mathrm{Ann}(m)$ ; on a $m \in N$ d’où $p = \mathrm{Ann}(N)$ et par suite $\mathrm{Supp}(N/xN) = V(p + xA)$ d’après II, § 4, no 4, corollaire à la prop. 18 ; par conséquent, q est associé à $N/xN$ (IV, § 1, no 4, th. 2).

#### Lemme 4 {#ac-ix-s4-lem-4 .statement}

Soient A un anneau de valuation discrète, B un anneau local noethérien, et $\rho : A \to B$ un homomorphisme local et plat. Si l’anneau $\kappa_A \otimes_A B$ est réduit, alors B est réduit.

Supposons qu’il existe un élément nilpotent non nul x de B, et soit $\pi$ une uniformisante de A. Puisqu’on a $\pi B \subset m_B$, l’anneau B est séparé pour la topologie $\pi B$-adique. Il existe donc $n \in \mathbf{N}$ et $y \in B$ avec $x = \pi^n y$ et $y \notin \pi B$. Puisque B est plat sur A, la multiplication par $\pi$ est injective dans B. La classe de y dans $B/\pi B$ est donc un élément nilpotent non nul, ce qui contredit l’hypothèse.

### 4. Anneaux de Nagata

#### Définition 2 {#ac-ix-s4-def-2 .statement}

On dit qu’un anneau A est un anneau de Nagata s’il est noethérien et si, pour tout idéal premier p de A, l’anneau noethérien intègre $A/p$ est japonais (no 1, déf. 1).

#### Exemple 1 {#ac-ix-s4-n4-exa-1 .statement}

Toute algèbre de type fini sur un corps est un anneau de Nagata (no 1, exemple).

#### Exemple 2 {#ac-ix-s4-n4-exa-2 .statement}

Tout anneau noethérien local complet est un anneau de Nagata (n° 2, th. 2).

#### Exemple 3 {#ac-ix-s4-n4-exa-3 .statement}

L’anneau $\mathbf{Z}$ est un anneau de Nagata (n° 1, exemple et corollaire de la prop. 1).

#### Exemple 4 {#ac-ix-s4-n4-exa-4 .statement}

On peut montrer (exerc. 30) que toute algèbre de type fini sur un anneau de Nagata est un anneau de Nagata.

#### Proposition 4 {#ac-ix-s4-prop-4 .statement}

Soit $A$ un anneau de Nagata.
a) Toute $A$-algèbre finie est un anneau de Nagata.
b) Pour toute partie multiplicative $S$ de $A$, l’anneau $S^{-1}A$ est un anneau de Nagata.
a) Soit $B$ une $A$-algèbre finie, $\rho : A \to B$ l’homomorphisme canonique. Pour tout idéal premier $p$ de $B$, l’anneau $B/p$ qui est une algèbre finie sur l’anneau japonais $A/\rho^{-1}(p)$, est japonais (n° 1, prop. 2).
b) Soit $q$ un idéal premier de $S^{-1}A$; alors il existe un idéal premier $p$ de $A$ tel que $q = S^{-1}p$. L’anneau $(S^{-1}A)/q$ est un anneau de fractions de l’anneau japonais $A/p$, donc est japonais (n° 1, remarque 2).

#### Théorème 3 (Zariski-Nagata) {#ac-ix-s4-thm-3 .statement}

Soit $A$ un anneau semi-local noethérien. Les conditions suivantes sont équivalentes :
(i) $A$ est un anneau de Nagata ;
(ii) pour tout idéal premier $p$ de $A$, la $\kappa(p)$-algèbre $\kappa(p) \otimes_A \hat{A}$ est séparable ;
(iii) pour toute $A$-algèbre réduite $R$, l’anneau $R \otimes_A \hat{A}$ est réduit.
Démontrons d’abord l’équivalence des conditions (ii) et (iii). L’implication (iii) $\Rightarrow$ (ii) est triviale ; supposons inversement que $A$ satisfasse à la condition (ii). Alors, pour toute $A$-algèbre $K$ qui est un corps, l’anneau $K \otimes_A \hat{A}$ est réduit. Soit maintenant $C$ une $A$-algèbre réduite de type fini ; l’anneau $C$, étant noethérien, est isomorphe à un sous-anneau d’un produit fini $K_1 \times \cdots \times K_n$ de corps (IV, § 2, n° 5, prop. 10) ; puisque $\hat{A}$ est plat sur $A$, l’anneau $C \otimes_A \hat{A}$ est isomorphe à un sous-anneau de l’anneau réduit $\prod_i (K_i \otimes_A \hat{A})$, donc est réduit. Soit enfin $R$ une $A$-algèbre réduite quelconque ; alors $R$ est réunion de la famille filtrante $(C_\alpha)$ de ses sous-algèbres de type fini, et $R \otimes_A \hat{A}$ est limite inductive de la famille filtrante $(C_\alpha \otimes_A \hat{A})$ d’anneaux réduits, donc est réduit.
Montrons que (ii) implique (i). Soit $p$ un idéal premier de $A$; le corps des fractions $K$ de l’anneau $A/p$ s’identifie à $\kappa(p)$, et la $K$-algèbre $K \otimes_{A/p} (\widehat{A/p})$ s’identifie à $\kappa(p) \otimes_{A/p} \hat{A}/p\hat{A}$, donc à $\kappa(p) \otimes_A \hat{A}$. Si $\kappa(p) \otimes_A \hat{A}$ est une $\kappa(p)$-algèbre séparable, l’anneau $A/p$ est japonais (n° 2, prop. 3).
Démontrons l’implication (i) $\Rightarrow$ (ii) par récurrence sur $\dim(A)$. Elle est évidente si $\dim(A) = 0$ puisqu’alors $A$ est artinien, donc complet. Soit $n$ un entier $> 0$; considérons l’hypothèse suivante :

(R$_n$) $\left\{ \begin{array}{l}
\text{pour tout anneau local noethérien de Nagata } C \text{ de dimension } < n \text{ et tout idéal premier } r \text{ de } C, \text{ l’anneau } \kappa(r) \otimes_C \hat{C} \text{ est réduit.}
\end{array} \right.$

Soit $A$ un anneau semi-local noethérien de Nagata de dimension $n$, soient $p$ un idéal premier de $A$ et $L$ une extension finie du corps $\kappa(p)$; il suffit de démontrer,

#### Corollaire 1 {#ac-ix-s4-thm-3-cor-1 .statement}

*Le complété d’un anneau de Nagata local et réduit est réduit.*
Il suffit en effet de poser R = A dans le th. 3, (iii).

#### Corollaire 2 (Chevalley) {#ac-ix-s4-thm-3-cor-2 .statement}

*Soient A une algèbre réduite de type fini sur un corps, et p un idéal premier de A. Le complété de l’anneau local $A_p$ est réduit.*
Comme A est réduit, l’anneau local $A_p$ est réduit ; de plus A est un anneau de Nagata (exemple 1), donc $A_p$ est un anneau de Nagata (prop. 4), et le cor. 2 résulte du cor. 1, appliqué à l’anneau $A_p$.

#### Corollaire 3 {#ac-ix-s4-thm-3-cor-3 .statement}

*Soient k un corps de caractéristique 0, et A une k-algèbre locale et noethérienne. Pour que A soit un anneau de Nagata, il faut et il suffit que, pour tout idéal premier p de A, l’anneau $(\widehat{A/p})$ soit réduit.*
En effet, puisque les corps $\kappa(p)$ sont de caractéristique 0, il est équivalent de dire que les algèbres $\kappa(p) \otimes_A \hat{A} = \kappa(p) \otimes_{A/p} (\widehat{A/p})$ sont réduites ou qu’elles sont séparables (A, V, p. 117, th. 1), ce qui montre que la condition énoncée est suffisante (th. 3, (ii) ⇒ (i)) ; elle est par ailleurs nécessaire (th. 3, (i) ⇒ (iii) avec R = A/p).

## EXERCICES {#ac-ix-s4-exercises}

See the [exercises for § 4](exercises/s4/).
