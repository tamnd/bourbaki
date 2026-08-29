---
book: ac
book_title: Commutative Algebra
chapter: X
chapter_title: Profondeur, régularité, dualité
section: 8
section_title: Dualité des modules de longueur finie
lang: fr
source: ac-x-fr
pdf_pages: 0104-0123, 0172-0174
extraction: ocr
subsections:
    - "no": 1
      title: Modules injectifs indécomposables
      page: 0
      pdf_page: 104
    - "no": 2
      title: Structure des modules injectifs indécomposables
      page: 0
      pdf_page: 105
    - "no": 3
      title: Dualité de Matlis
      page: 110
      pdf_page: 109
    - "no": 4
      title: Dualité des modules de longueur finie
      page: 114
      pdf_page: 113
    - "no": 5
      title: Foncteurs dualisants
      page: 115
      pdf_page: 114
    - "no": 6
      title: Changement d’anneaux ; dualité de Macaulay
      page: 119
      pdf_page: 118
    - "no": 7
      title: Dualité des modules d’extensions et des produits de torsion
      page: 0
      pdf_page: 119
statements: 31
exercises: 10
content_sha256: 77f9377a8e567979844890a8c62bb0a878d9c20aeb59902a661be4f0e8769c2f
---

## § 8. DUALITÉ DES MODULES DE LONGUEUR FINIE

### 1. Modules injectifs indécomposables

Soit $A$ un anneau. La relation « $I$ est une classe de $A$-modules injectifs indécomposables » est collectivisante (A, X, p. 21, cor. 1) ; nous noterons $\mathscr{J}(A)$ l’ensemble des classes de $A$-modules injectifs indécomposables.

#### Proposition 1 {#ac-x-s8-prop-1 .statement}

Soit $A$ un anneau noethérien. Pour tout idéal premier $\mathfrak{p}$ de $A$, soit $e_{\mathfrak{p}} : A/\mathfrak{p} \to I(\mathfrak{p})$ une enveloppe injective de $A/\mathfrak{p}$ (A, X, § 1, n° 9).

a) Les $A$-modules $I(\mathfrak{p})$ sont indécomposables.

b) Soit $I$ un $A$-module injectif indécomposable ; l’ensemble $\mathrm{Ass}(I)$ est réduit à un élément.

c) L’application $\mathfrak{p} \mapsto \mathrm{cl}(I(\mathfrak{p}))$ est une bijection de $\mathrm{Spec}(A)$ sur $\mathscr{J}(A)$. La bijection réciproque associe à un élément $I$ de $\mathscr{J}(A)$ l’unique élément de $\mathrm{Ass}(I)$.

Soit $\mathfrak{p} \in \mathrm{Spec}(A)$ ; prouvons que le module $I(\mathfrak{p})$ est indécomposable. D’après A, X, p. 21, cor. 2, il suffit de prouver que si $a$ et $b$ sont des idéaux de $A$ contenant $\mathfrak{p}$ et distincts de $\mathfrak{p}$, l’idéal $a \cap b$ est distinct de $\mathfrak{p}$; or si $a$ est un élément de $a - \mathfrak{p}$ et $b$ un élément de $b - \mathfrak{p}$, le produit $ab$ appartient à $(a \cap b) - \mathfrak{p}$.

Soit $I$ un $A$-module injectif indécomposable, et soient $\mathfrak{p}, \mathfrak{q}$ des éléments de $\mathrm{Ass}(I)$. Alors $I$ contient un sous-module $M$ isomorphe à $A/\mathfrak{p}$ et un sous-module $N$ isomorphe à $A/\mathfrak{q}$. On a $M \cap N \neq 0$ (A, X, p. 21, prop. 14) ; pour tout élément $x$ non nul de $M \cap N$, on a $\mathfrak{p} = \mathrm{Ann} x = \mathfrak{q}$. Comme $\mathrm{Ass}(I)$ n’est pas vide (IV, § 1, n° 1, cor. 1 de la prop. 2), il est réduit à un élément $\mathfrak{p}(I)$.

Nous avons ainsi défini deux applications $\mathfrak{p} \mapsto \mathrm{cl}(I(\mathfrak{p}))$ de $\mathrm{Spec}(A)$ dans $\mathscr{J}(A)$ et $I \mapsto \mathfrak{p}(I)$ de $\mathscr{J}(A)$ dans $\mathrm{Spec}(A)$ ; prouvons que ces deux applications sont des bijections réciproques l’une de l’autre. Soit $\mathfrak{p} \in \mathrm{Spec}(A)$ ; alors $\mathfrak{p}$ appartient à $\mathrm{Ass}(I(\mathfrak{p}))$, et c’est donc l’unique élément de $\mathrm{Ass}(I(\mathfrak{p}))$. Soient $I$ un $A$-module injectif indécomposable, et $\mathfrak{p}$ l’unique élément de $\mathrm{Ass}(I)$ ; alors $I$ est une enveloppe injective de $A/\mathfrak{p}$ (A, X, p. 21, prop. 14). Cela achève la démonstration de la proposition.

#### Remarque 1 {#ac-x-s8-n1-rem-1 .statement}

Soit $I$ un $A$-module injectif indécomposable, et soit $\mathfrak{p}$ l’unique élément de $\mathrm{Ass}(I)$ ; d’après la prop. 1, $I$ contient un sous-module isomorphe à $A/\mathfrak{p}$ dont il est enveloppe injective. En général un tel sous-module n’est pas unique, comme on le constate en prenant $A = \mathbf{Z}$, $\mathfrak{p} = 0$, $I = \mathbf{Q}$.

Pour chaque idéal premier $\mathfrak{p}$ de $A$, choisissons comme ci-dessus une enveloppe injective $(I(\mathfrak{p}), e_{\mathfrak{p}})$ de $A/\mathfrak{p}$. D’après A, X, p. 22, th. 3, on a :

#### Théorème 1 {#ac-x-s8-thm-1 .statement}

Soit $A$ un anneau noethérien. Pour tout $A$-module injectif $I$, il existe une famille de cardinaux $(a_{\mathfrak{p}})_{\mathfrak{p} \in \mathrm{Spec}(A)}$, et une seule, telle que $I$ soit isomorphe à $\bigoplus_{\mathfrak{p}} I(\mathfrak{p})^{(a_{\mathfrak{p}})}$.

#### Remarque 2 {#ac-x-s8-n1-rem-2 .statement}

Soient $A$ un anneau noethérien, $M$ un $A$-module, $e : M \to I$ une enveloppe injective de $M$. *L’ensemble Ass(M) est égal à Ass(I)* : en effet l’inclusion $Ass(M) \subset Ass(I)$ est évidente. D’autre part, si $p$ est un élément de $Ass(I)$, $I$ contient un sous-module $N$ isomorphe à $A/p$ ; comme le $A$-module $e^{-1}(N)$ est non nul, on a $Ass(e^{-1}(N)) = \{p\}$ (IV, § 1, n° 1, prop. 1). Cela prouve que $p$ est associé à $e^{-1}(N)$, donc à $M$, d’où notre assertion.

Prenons les notations du théorème, et supposons de plus $Ass(M)$ fini. Pour tout $q \in Ass(M)$, notons $Q_q$ l’intersection avec $M$ de $\bigoplus_{p \in Ass(M) - \{q\}} I(p)^{(a_p)}$. Alors $(Q_q)_{q \in Ass(M)}$ *est une décomposition primaire réduite de 0 dans M* (IV, § 2, n° 3, déf. 3). On a en effet $\cap Q_q = 0$ ; comme $M/Q_q$ s’identifie à un sous-module non nul de $I(q)^{(a_q)}$, on a $Ass(M/Q_q) = \{q\}$, et il suffit d’appliquer la prop. 4 de *loc. cit*.

#### Exemple {#ac-x-s8-n1-exa-1 .statement}

Soit $A$ un anneau principal, et soit $K$ son corps des fractions. Les $A$-modules injectifs sont les $A$-modules divisibles (A, X, p. 17, cor. 2). Le $A$-module $K$ est une enveloppe injective de $A$ (A, X, p. 20, exemple 1). Soient $p$ un élément extrémal de $A$, et $p$ l’idéal (maximal) $Ap$ ; notons $e : A/p \longrightarrow K/A_p$ l’homomorphisme qui applique la classe d’un élément $a \in A$ sur la classe de $a/p$. Prouvons que $(K/A_p, e)$ *est une enveloppe injective de $A/p$*. L’homomorphisme $e$ est injectif. Le $A$-module $K/A_p$ est un quotient d’un module divisible, donc est divisible. Soit $x$ un élément non nul de $K/A_p$ ; c’est la classe d’un élément $a/p^n$ de $K$, avec $a \in A - \{0\}$ et $n \geqslant 1$ (A, VII, p. 10, th. 2). On a alors $p^{n-1}x = e(a)$, donc $e^{-1}(Ax) \neq 0$, ce qui prouve notre assertion.

Il résulte alors du th. 1 que *tout $A$-module divisible est somme directe de $A$-modules isomorphes à $K$ ou à $K/A_p$ pour un idéal maximal (principal) $p$ de $A$*.

### 2. Structure des modules injectifs indécomposables

#### Lemme 1 {#ac-x-s8-lem-1 .statement}

Soient $A$ un anneau, $a$ un idéal de $A$, et $I$ un $A$-module. Pour tout entier $n \geqslant 0$, notons $I_n$ le sous-module de $I$ formé des éléments annulés par $a^n$.

a) *Supposons le $A$-module $I$ injectif. Alors le $A/a^n$-module $I_n$ est injectif pour tout $n \geqslant 0$*.

b) *Supposons que l’anneau $A$ soit noethérien, et que pour tout $n \geqslant 0$ le $A/a^n$-module $I_n$ soit injectif. Alors la réunion des $I_n$ est un $A$-module injectif*.

a) Le $A/a^n$-module $I_n$ est isomorphe à $\operatorname{Hom}_A(A/a^n, I)$, qui est injectif (A, X, p. 18, prop. 11).

b) Soient $J$ la réunion des $I_n$, $b$ un idéal de $A$ et $f : b \to J$ un $A$-homomorphisme. Il s’agit (A, X, p. 16, prop. 10) de prouver qu’il existe un élément $x$ de $J$ tel qu’on ait $f(b) = bx$ pour tout $b \in b$. Puisque $b$ est de type fini, il existe un entier $n$ tel qu’on ait $f(b) \subset I_n$, c’est-à-dire $f(a^n b) = 0$. D’après le cor. 2 de la prop. 1 de III, § 3, n° 1, il existe un entier $m \geqslant n$ tel que $a^m \cap b \subset a^n b$, donc $f(a^m \cap b) = 0$. Alors $f$ induit une application $A/a^m$-linéaire de $b/(a^m \cap b)$ dans $I_m$ ; comme le $A/a^m$-module $I_m$ est injectif, il existe un élément $x$ de $I_m$ tel qu’on ait $f(b) = bx$ pour tout $b \in b$, d’où b).

Soit $\alpha$ un idéal de $A$; nous conviendrons dans ce qui suit de poser $\alpha^n = A$ pour tout entier $n \leq 0$. Soit $E$ un $A$-module. Pour tout $n \in \mathbf{Z}$, notons $E_n$ le sous-module de $E$ formé des éléments annulés par $\alpha^n$; soit $\mathrm{gr}^\alpha(E)$ le $A$-module gradué de type $\mathbf{Z}$ tel que $\mathrm{gr}^\alpha(E)_m = E_{-m+1}/E_{-m}$ pour tout entier $m$. Le module $\mathrm{gr}^\alpha(E)_m$ est nul pour $m \geq 1$, et $\mathrm{gr}^\alpha(E)_0$ s’identifie à $E_1$. Notons $\mathrm{gr}(A)$ l’anneau gradué associé à $A$ pour la filtration $\alpha$-adique : on a $\mathrm{gr}(A)_n = \alpha^n/\alpha^{n+1}$ pour tout $n \in \mathbf{Z}$. Soient $n$ et $m$ des entiers. On déduit par passage aux quotients de l’application bilinéaire $(a, x) \mapsto ax$ de $\alpha^n \times E_{-m+1}$ dans $E_{-m-n+1}$ une application $A/\alpha$-bilinéaire

$$
\alpha_{n,m} : \mathrm{gr}(A)_n \times \mathrm{gr}^\alpha(E)_m \longrightarrow \mathrm{gr}^\alpha(E)_{n+m},
$$

qui définit sur $\mathrm{gr}^\alpha(E)$ une structure de $\mathrm{gr}(A)$-module gradué. Pour tout $n \in \mathbf{Z}$, on déduit de l’application $A/\alpha$-bilinéaire $\alpha_{n,-n} : \mathrm{gr}(A)_n \times \mathrm{gr}^\alpha(E)_{-n} \longrightarrow E_1$ une application $A/\alpha$-linéaire $\beta_{E,n} : \mathrm{gr}^\alpha(E)_{-n} \longrightarrow \mathrm{Hom}_{A/\alpha}(\mathrm{gr}(A)_n, E_1)$; les applications $\beta_{E,n}$ sont les composantes d’un homomorphisme de $A/\alpha$-modules gradués, dit *canonique*

$$
\beta_E : \mathrm{gr}^\alpha(E) \longrightarrow \mathrm{Hom}_{\mathrm{gr}_{A/\alpha}}(\mathrm{gr}(A), E_1).
$$

Pour $a \in \mathrm{gr}(A)$, $x \in \mathrm{gr}^\alpha(E)$, $\beta_E(x)(a)$ est par définition le composant dans $\mathrm{gr}^\alpha(E)_0 = E_1$ de l’élément $ax$ de $\mathrm{gr}^\alpha(E)$. Il en résulte que $\beta_E$ est $\mathrm{gr}(A)$-linéaire lorsqu’on munit $\mathrm{Hom}_{\mathrm{gr}_{A/\alpha}}(\mathrm{gr}(A), E_1)$ de la structure de $\mathrm{gr}(A)$-module définie par la formule $(bf)(a) = f(ab)$ pour $a, b$ dans $\mathrm{gr}(A)$ et $f$ dans $\mathrm{Hom}_{\mathrm{gr}_{A/\alpha}}(\mathrm{gr}(A), E_1)$.

#### Proposition 2 {#ac-x-s8-prop-2 .statement}

*Soient $A$ un anneau noethérien, $\alpha$ un idéal de $A$, $E$ un $A$-module et $M$ un sous-$A$-module de $E$ annulé par $\alpha$. Les conditions suivantes sont équivalentes :*
    (i) *$E$ est une enveloppe injective de $M$* ;
    (ii) *le $\Lambda/\alpha$-module $E_1$ est une enveloppe injective du $A/\alpha$-module $M$, le module $E$ est réunion des $E_n$ et l’application canonique $\beta_E$ est bijective*.

Supposons la condition (i) satisfaite. Le $A/\alpha$-module $E_1$ est injectif (lemme 1, a)), et contient $M$; comme tout sous-$\Lambda/\alpha$-module de $E_1$ est un sous-$A$-module de $E$, $E_1$ est une enveloppe injective du $\Lambda/\alpha$-module $M$. D’après le lemme 1, la réunion des $E_n$ est un sous-$A$-module injectif de $E$ contenant $M$, donc égal à $E$. Puisque $E$ est injectif, on a pour tout $n \geq 0$ une suite exacte

$$
0 \to \mathrm{Hom}_A(A/\alpha^n, E) \longrightarrow \mathrm{Hom}_A(A/\alpha^{n+1}, E) \longrightarrow \mathrm{Hom}_A(\alpha^n/\alpha^{n+1}, E) \to 0;
$$

comme $\mathrm{Hom}_A(A/\alpha^m, E)$ s’identifie à $E_m$ pour tout $m$ et que l’injection canonique de $\mathrm{Hom}_A(\alpha^n/\alpha^{n+1}, E_1)$ dans $\mathrm{Hom}_A(\alpha^n/\alpha^{n+1}, E)$ est bijective, on en déduit que l’homomorphisme canonique $\beta_E$ est bijectif, d’où (ii).

Supposons (ii) satisfaite. Soit $e : M \to I$ une enveloppe injective de $M$. Puisque $I$ est injectif, il existe une application $A$-linéaire $\varphi : E \to I$ prolongeant $e$. Mais $\varphi$ applique $E_n$ dans $I_n$ pour tout $n$, donc induit des homomorphismes gr^{a}(\varphi) : \operatorname{gr}^{a}(E) \to \operatorname{gr}^{a}(I) \text{ et } \varphi_1 : E_1 \to I_1 \text{ rendant commutatif le diagramme}

$$
\begin{array}{ccc}
\operatorname{gr}^{a}(E) & \xrightarrow{\beta_E} & \operatorname{Homgr}_{A/\alpha}(\operatorname{gr}(A), E_1) \\
\downarrow \operatorname{gr}^{a}(\varphi) & & \downarrow \operatorname{Homgr}(1, \varphi_1) \\
\operatorname{gr}^{a}(I) & \xrightarrow{\beta_I} & \operatorname{Homgr}_{A/\alpha}(\operatorname{gr}(A), I_1)
\end{array}
$$

Puisque $E_1$ et $I_1$ sont des enveloppes injectives du $A/\alpha$-module $M$, l’homomorphisme $\varphi_1$ est bijectif ; puisque $\beta_E$ et $\beta_I$ sont bijectifs, il en résulte que $\operatorname{gr}^{a}(\varphi)$ est bijectif. Cela implique, par récurrence sur $n$, que $\varphi$ induit une bijection de $E_n$ sur $I_n$ pour tout $n \geq 1$ ; donc $\varphi$ est bijectif, ce qui entraîne (i).

#### Lemme 2 {#ac-x-s8-lem-2 .statement}

*Soient $A$ un anneau, $\alpha$ un idéal de type fini de $A$, et $M$ un $A$-module dont tout élément est annulé par une puissance de $\alpha$. Notons $\widehat{A}$ le séparé complété de $A$ pour la topologie $\alpha$-adique.*

a) *Il existe sur $M$ une unique structure de $\widehat{A}$-module étendant la structure de $A$-module donnée.*

b) *Les sous-$\widehat{A}$-modules de $M$ sont ses sous-$A$-modules, et l’on a $\operatorname{Hom}_A(M, P) = \operatorname{Hom}_{\widehat{A}}(M, P)$ pour tout $\widehat{A}$-module $P$.

a) Identifions $\widehat{A}$ à la limite projective des anneaux $A/\alpha^n$, et munissons $M$ de la topologie discrète. Soient $a = (a_n)$ un élément de $\widehat{A}$, et $x$ un élément de $M$. Comme $x$ est annulé par une puissance de $\alpha$, la suite $(a_n x)$ est stationnaire ; notons $ax$ sa limite. L’application $(a, x) \mapsto ax$ définit sur $M$ une structure de $\widehat{A}$-module qui étend la structure de $A$-module donnée.

Inversement, supposons donnée une telle structure sur $M$ ; soient $a = (a_n)$ un élément de $\widehat{A}$, $x$ un élément de $M$ et $m$ un entier tel que $\alpha^m x = 0$. Pour tout entier $n$, $a - a_n$ appartient à $\alpha^n$, qui est égal à $\alpha^n \widehat{A}$ (III, § 2, n° 12, cor. 2 de la prop. 16) ; on a donc $ax = a_n x$ pour $n \geq m$, d’où l’assertion d’unicité.

b) Il résulte de ce qui précède qu’on a $Ax = \widehat{A}x$ pour tout $x \in M$ ; les sous-$\widehat{A}$-modules de $M$ sont donc ses sous-$A$-modules. Enfin, soit $u$ un homomorphisme $A$-linéaire de $M$ dans un $\widehat{A}$-module $P$. Soient $a = (a_n)$ un élément de $\widehat{A}$, $x$ un élément de $M$ et $m$ un entier tel que $\alpha^m x = 0$ ; on a $\alpha^m u(x) = 0$. Comme $a - a_m$ appartient à $\alpha^m \widehat{A}$, on a

$$
u(ax) = u(a_m x) = a_m u(x) = au(x),
$$

de sorte que $u$ est $\widehat{A}$-linéaire.

#### Proposition 3 {#ac-x-s8-prop-3 .statement}

*Soient $A$ un anneau noethérien, $p$ un idéal premier de $A$ et $e : A/p \to I$ une enveloppe injective du $A$-module $A/p$. Pour tout entier $n \geq 0$, désignons par $I_n$ le sous-module de $I$ formé des éléments annulés par $p^n$.*

a) Le $A$-module $I$ est réunion des $I_n$. L’injection $\Lambda / \mathfrak{p} \to I_1$ se prolonge en un isomorphisme de $\kappa(\mathfrak{p})$ sur $I_1$; identifions $\kappa(\mathfrak{p})$ à $I_1$ à l’aide de cet isomorphisme. Pour chaque entier $n \geqslant 0$, la structure de $\Lambda / \mathfrak{p}$-module de $I_{n+1}/I_n$ provient par restriction des scalaires d’une unique structure de $\kappa(\mathfrak{p})$-espace vectoriel ; l’homomorphisme canonique $\beta_{I,-n}: I_{n+1}/I_n \longrightarrow \mathrm{Hom}_{\Lambda/\mathfrak{p}}(\mathfrak{p}^n/\mathfrak{p}^{n+1}, \kappa(\mathfrak{p}))$ est un isomorphisme de $\kappa(\mathfrak{p})$-espaces vectoriels de dimension finie.

b) Il existe une unique structure de $\widehat{A_p}$-module sur $I$ induisant sa structure de $A$-module. L’homomorphisme canonique $\widehat{A_p} \longrightarrow \mathrm{End}_A(I)$ est bijectif.

D’après A, X, p. 20, exemple 1, le $A/\mathfrak{p}$-module $\kappa(\mathfrak{p})$ est une enveloppe injective de $A/\mathfrak{p}$. Il résulte donc de la prop. 2 que $I_1$ s’identifie à $\kappa(\mathfrak{p})$, que $I$ est réunion des $I_m$, et que pour chaque entier $n \geqslant 0$, $\beta_{I,-n}$ est un isomorphisme de $A/\mathfrak{p}$-modules. Pour tout élément non nul $a$ de $A/\mathfrak{p}$, l’homothétie de rapport $a$ est inversible dans $\mathrm{Hom}_{A/\mathfrak{p}}(\mathfrak{p}^n/\mathfrak{p}^{n+1}, \kappa(\mathfrak{p}))$, donc aussi dans $I_{n+1}/I_n$, ce qui achève de prouver a).

Soit $s \in A - \mathfrak{p}$. Comme l’homothétie $s_{A/\mathfrak{p}}$ est injective, la trace de $\mathrm{Ker}\, s_I$ sur $A/\mathfrak{p}$ est nulle, ce qui entraîne que l’homothétie $s_I$ est injective. Alors $s_I$ est un sous-module facteur direct de $I$ (A, X, p. 19, cor. 4), donc égal à $I$ puisque $I$ est indécomposable ($n^\circ 1$, prop. 1), de sorte que l’homothétie $s_I$ est bijective. Il existe donc une unique structure de $A_p$-module sur $I$ induisant sa structure de $A$-module ; elle s’étend de manière unique en une structure de $\widehat{A_p}$-module (lemme 2).

Pour chaque entier $n$, on déduit de l’homomorphisme d’anneaux canonique $\Lambda_p \longrightarrow \mathrm{End}_A(I)$ une application $A$-linéaire $\alpha_n : A_p/\mathfrak{p}^n A_p \longrightarrow \mathrm{Hom}_A(I_n, I)$. Considérons le diagramme commutatif à lignes exactes

$$
\begin{array}{ccccccccc}
0 & \longrightarrow & \mathfrak{p}^n A_p/\mathfrak{p}^{n+1} A_p & \longrightarrow & A_p/\mathfrak{p}^{n+1} A_p & \longrightarrow & A_p/\mathfrak{p}^n A_p & \longrightarrow & 0 \\
& & \downarrow \alpha'_{n+1} & & \downarrow \alpha_{n+1} & & \downarrow \alpha_n & & \\
0 & \longrightarrow & \mathrm{Hom}_A(I_{n+1}/I_n, I_1) & \longrightarrow & \mathrm{Hom}_A(I_{n+1}, I) & \longrightarrow & \mathrm{Hom}_A(I_n, I) & \longrightarrow & 0
\end{array}
$$

où $\alpha'_{n+1}$ est l’homomorphisme induit par $\alpha_{n+1}$. Considérons l’application $\kappa(\mathfrak{p})$-bilinéaire canonique

$$
\alpha_{n,-n} : \mathfrak{p}^n A_p/\mathfrak{p}^{n+1} A_p \times I_{n+1}/I_n \longrightarrow I_1
$$

(formule (1)). L’application linéaire $I_{n+1}/I_n \longrightarrow \mathrm{Hom}_{\kappa(\mathfrak{p})}(\mathfrak{p}^n A_p/\mathfrak{p}^{n+1} A_p, I_1)$ qui lui est associée à gauche s’identifie à $\beta_{I,-n}$, et celle qui lui est associée à droite est $\alpha'_{n+1}$. Comme $\beta_{I,-n}$ est bijective d’après a), il en est de même de $\alpha'_{n+1}$; on déduit alors du diagramme ci-dessus, par récurrence sur $n$, que $\alpha_n$ est un isomorphisme pour tout $n$. Comme $I$ est réunion des $I_n$, l’application canonique $\mathrm{End}_A(I) \to \varprojlim \mathrm{Hom}_A(I_n, I)$ est bijective ; l’homomorphisme d’anneaux $\widehat{A_p} \to \mathrm{End}_A(I)$, qui s’identifie à la limite projective des applications $\alpha_n$, est donc bijectif.

#### Remarque {#ac-x-s8-n2-rem-1 .statement}

Il résulte de la démonstration précédente que l’annulateur de $I_n$ dans $\widehat{A_p}$ (resp. dans $A_p$) est $\mathfrak{p}^n \widehat{A_p}$ (resp. $\mathfrak{p}^n A_p$). Par suite l’annulateur du $A$-module $I_n$ est l’image réciproque dans $A$ de l’idéal $\mathfrak{p}^n A_p$, que l’on note parfois $\mathfrak{p}^{(n)}$ et que l’on appelle la puissance symbolique $n$-ième de l’idéal premier $\mathfrak{p}$.

#### Corollaire {#ac-x-s8-n2-cor-1 .statement}

Soit J un A-module injectif tel que Ass_A(J) = {p}.

a) L’application canonique J → A_p ⊗_A J est bijective.

b) Notons E le A/p-module Hom_A(A/p, J). Il existe sur E une unique structure de κ(p)-espace vectoriel prolongeant sa structure de A/p-module ; le A-module J est isomorphe à I([E:κ(p)]).

En effet, J est isomorphe à un A-module I^{(c)}, où c est un cardinal convenable (n° 1, th. 1). Le corollaire résulte de la proposition lorsque J = I et le cas général s’en déduit aussitôt.

### 3. Dualité de Matlis

Dans ce numéro, on suppose que l’anneau A est local noethérien.

#### Définition {#ac-x-s8-n3-def-1 .statement}

On dit qu’un A-module I est un A-module de Matlis s’il est injectif, que m_A est son unique idéal premier associé et que le κ_A-espace vectoriel Hom_A(κ_A, I) est de dimension 1.

Soit e : κ_A → I une enveloppe injective de κ_A (A, X, p. 20, th. 2). Le A-module I est un module de Matlis, et tout A-module de Matlis est isomorphe à I (n° 2, cor. de la prop. 3). Si A est un anneau de valuation discrète, de corps des fractions K, le A-module K/A est un module de Matlis (n° 1, exemple). Si A est un anneau local artinien, le A-module A est un module de Matlis si et seulement si A est un anneau de Gorenstein (§ 3, n° 7, lemme 1).

Soit I un A-module de Matlis. Pour tout entier n ≥ 0, notons I_n le sous-A-module de I formé des éléments annulés par m_A^n. D’après la prop. 2 du n° 2, le A-module I est réunion des I_n, le A-module I_1 est de longueur 1 (c’est-à-dire isomorphe à κ_A) et le A-module I est une enveloppe injective de I_1 ; en outre, l’homomorphisme canonique de gr(A)-modules gradués

$$
\beta : \operatorname{gr}^{m_A}(I) \longrightarrow \operatorname{Hom}_{\kappa_A}(\operatorname{gr}(A), I_1)
$$

est un isomorphisme. D’après la prop. 3 du n° 2, la structure de A-module de I s’étend en une unique structure de $\widehat{A}$-module, et l’homomorphisme canonique $\widehat{A} \to \operatorname{End}_A(I)$ est bijectif.

#### Lemme 3 {#ac-x-s8-lem-3 .statement}

Soit I un A-module de Matlis. Alors :

a) I est un $\widehat{A}$-module de Matlis ;
b) le A-module I est artinien et cogénérateur (A, X, p. 18, déf. 3).

Puisque le A-module I est injectif, le A/m_A^n-module I_n est injectif pour chaque n (n° 2, lemme 1, a)). Comme I_n est l’ensemble des éléments de I annulés par m_A^n, le $\widehat{A}$-module I est injectif (lemme 1, b)). Il est indécomposable sur $\widehat{A}$ puisqu’il l’est sur A ; comme il contient le sous-$\widehat{A}$-module I_1 isomorphe à $\kappa_A$, on a $m_{\widehat{A}} \in \operatorname{Ass}_{\widehat{A}}(I)$, donc $\operatorname{Ass}_{\widehat{A}}(I) = \{ m_{\widehat{A}} \}$ (prop. 1), d’où a).

Prouvons maintenant que I est artinien. À tout sous-A-module M de I, associons l’idéal gradué $a_M$ de gr(A) défini de la façon suivante : un élément de gr(A)_n appartient à $(\mathfrak{a}_M)_n$ s’il est annulé par toutes les formes linéaires $\beta(x)$, où $x$ parcourt $((M \cap I_{n+1}) + I_n)/I_n$. Soient $M$ et $N$ des sous-modules de $I$ tels que $N \subset M$; on a $\mathfrak{a}_M \subset \mathfrak{a}_N$. Supposons $\mathfrak{a}_M = \mathfrak{a}_N$; on a $(M \cap I_{n+1}) + I_n = (N \cap I_{n+1}) + I_n$ pour tout $n$ puisque $\beta$ est un isomorphisme. Par récurrence sur $n$ on en déduit $M \cap I_{n+1} = N \cap I_{n+1}$ pour tout $n$, d’où finalement $M = N$.

Cela étant, soit $M_0 \supset M_1 \supset \ldots \supset M_n \supset \ldots$ une suite décroissante de sous-A-modules de $I$; la suite croissante $\mathfrak{a}_{M_0} \subset \mathfrak{a}_{M_1} \subset \ldots$ est stationnaire, puisque $\mathrm{gr}(A)$ est une $\kappa_A$-algèbre de type fini. La suite $(M_i)_{i \geq 0}$ est donc stationnaire, ce qui entraîne que le A-module $I$ est artinien. Enfin, le A-module $I$ est cogénérateur en vertu de A, X, p. 18, prop. 12.

Soit $M$ un A-module. Rappelons (A, VIII, § 4, n° 6) que le socle de $M$ est la somme des sous-modules simples de $M$, c’est-à-dire l’ensemble des éléments de $M$ annulés par $m_A$; c’est un $\kappa_A$-espace vectoriel, canoniquement isomorphe à $\mathrm{Hom}_A(\kappa_A, M)$.

#### Lemme 4 {#ac-x-s8-lem-4 .statement}

*Soient I un A-module de Matlis et M un $\Lambda$-module. Les conditions suivantes sont équivalentes :*

(i) $M$ est artinien ;
(ii) tout élément de $M$ est annulé par une puissance de $m_A$, et le socle de $M$ est de dimension finie sur $\kappa_\Lambda$ ;
(iii) il existe un entier $n \geq 0$ et une application A-linéaire injective de $M$ dans $I^n$.

*Lorsque ces conditions sont satisfaites, toute enveloppe injective de $M$ est isomorphe à $I^s$, où $s$ est la dimension sur $\kappa_A$ du socle de $M$.*

(iii) $\Rightarrow$ (i) : c’est clair puisque le A-module $I$ est artinien (lemme 3).

(i) $\Rightarrow$ (ii) : supposons $M$ artinien. Soit $x \in M$; la suite décroissante des sous-modules $m_A^n x$ de $M$ est stationnaire. Soit $n$ un entier tel que $m_A^{n+1} x = m_A^n x$; le lemme de Nakayama entraîne $m_A^n x = 0$. Par ailleurs, le socle de $M$ est artinien en tant que A-module, donc aussi en tant que $\kappa_A$-espace vectoriel, ce qui signifie qu’il est de dimension finie.

(ii) $\Rightarrow$ (iii) : supposons la condition (ii) vérifiée; soit $e : M \to J$ une enveloppe injective de $M$. On a $\mathrm{Ass}(M) \subset \{m_A\}$, donc $\mathrm{Ass}(J) \subset \{m_A\}$ (n° 1, remarque 2), et $J$ est isomorphe à $I^{(c)}$ pour un cardinal $c$ (n° 1, th. 1). Soit $x$ un élément non nul de $J$ annulé par $m_A$; comme le A-module $Ax$ est simple et que son intersection avec $e(M)$ n’est pas réduite à 0, $x$ appartient à $e(M)$. Ainsi $e$ induit un isomorphisme du socle de $M$ sur celui de $J$; par suite le socle de $M$ est de dimension $c$, ce qui prouve (iii) ainsi que la dernière assertion.

#### Lemme 5 {#ac-x-s8-lem-5 .statement}

*Tout $\widehat{\Lambda}$-module artinien est artinien en tant que $\Lambda$-module.*

Soit $M$ un $\widehat{\Lambda}$-module artinien; tout élément de $M$ est annulé par une puissance de $m_{\widehat{\Lambda}}$, donc par une puissance de $m_A$. D’après le lemme 2 du n° 2, les sous-A-modules de $M$ sont ses sous-$\widehat{\Lambda}$-modules, donc $M$ est artinien en tant que A-module.

Fixons maintenant un $A$-module de Matlis I. Pour tout $A$-module $M$, notons $D_A(M)$ le $\widehat{A}$-module
$$
D_A(M) = \operatorname{Hom}_A(M, I)
$$
Le $\widehat{A}$-module $D_A(A)$ s’identifie canoniquement à $I$, le $\widehat{A}$-module $D_A(I)$ à $\widehat{A}$ ($n^\circ 2$, prop. 3), et le $\widehat{A}$-module $D_A(\kappa_A)$ à $I_1$ (*loc. cit.*).

Pour toute application $A$-linéaire $f : M \to N$, nous noterons
$$
D_A(f) : D_A(N) \to D_A(M)
$$
l’application $\widehat{A}$-linéaire $\operatorname{Hom}_A(f, 1_I)$. Puisque le $A$-module $I$ est injectif, la suite $(D_A(g), D_A(f))$ est exacte pour toute suite exacte $(f, g)$ d’applications $A$-linéaires.

Nous appliquerons ces définitions à l’anneau $\widehat{A}$ muni du module de Matlis I (lemme 3, a)) ; pour tout $\widehat{A}$-module $P$, $D_{\widehat{A}}(P)$ est donc le sous-$\widehat{A}$-module $\operatorname{Hom}_{\widehat{A}}(P, I)$ de $D_A(P)$. Il revient au même de dire que $P$ est artinien comme $A$-module ou comme $\widehat{A}$-module (lemme 5) ; si c’est le cas on a $D_{\widehat{A}}(P) = D_A(P)$ (*loc. cit.*).

Soit $M$ un $A$-module. Pour $m \in M$, l’application $f \mapsto f(m)$ de $D_A(M)$ dans $I$ est $\widehat{A}$-linéaire ; notons-la $\alpha_M(m)$. On définit ainsi un homomorphisme $A$-linéaire
$$
\alpha_M : M \longrightarrow D_{\widehat{A}}(D_A(M))
$$
On note $\widehat{\alpha}_M : \widehat{A} \otimes_A M \longrightarrow D_{\widehat{A}}(D_A(M))$ l’application $\widehat{A}$-linéaire déduite de $\alpha_M$.

#### Théorème 2 {#ac-x-s8-thm-2 .statement}

*Soit $M$ un $A$-module.*

a) *Pour que $M$ soit artinien, il faut et il suffit que le $\widehat{A}$-module $D_A(M)$ soit de type fini. Lorsque c’est le cas, l’homomorphisme $\alpha_M$ est bijectif.*

b) *Pour que $M$ soit de type fini, il faut et il suffit que $D_A(M)$ soit artinien (comme $A$-module ou comme $\widehat{A}$-module). Dans ce cas l’homomorphisme $\widehat{\alpha}_M$ est un isomorphisme.*

c) *Pour que $M$ soit de longueur finie, il faut et il suffit que $D_A(M)$ soit de longueur finie (comme $A$-module ou comme $\widehat{A}$-module). Dans ce cas $\alpha_M$ est un isomorphisme de $M$ sur $D_A(D_A(M))$, et l’on a $\operatorname{long}_A(D_A(M)) = \operatorname{long}_A(M)$.*

Prouvons d’abord que l’homomorphisme $\alpha_M$ est injectif pour tout $A$-module $M$. Soit $m$ un élément non nul de $M$ ; son annulateur est contenu dans $m_A$. Il existe donc un $A$-homomorphisme surjectif de $Am$ sur $\kappa_A$, et par suite un homomorphisme non nul de $Am$ dans $I$. Comme $I$ est injectif, celui-ci se prolonge en un homomorphisme $f : M \to I$ tel que $f(m) \neq 0$. Cela prouve l’injectivité de $\alpha_M$.

Supposons le $A$-module $M$ artinien. D’après le lemme 4, il existe un entier $r$ et une application $A$-linéaire injective $f : M \to I^r$. L’homomorphisme $D_A(f) : D_A(I^r) \to D_A(M)$ est alors surjectif ; comme $D_A(I^r)$ s’identifie à $\widehat{A}^r$, cela prouve que le $\widehat{A}$-module $D_A(M)$ est de type fini. De manière analogue, si $M$ est de type fini, il existe un entier $n$ et un homomorphisme surjectif $u : A^n \to M$ ; l’homomorphisme $D_A(u) : D_A(M) \to I^n$ est injectif, de sorte que $D_A(M)$ est artinien (comme $A$-module ou comme $\widehat{A}$-module).

Supposons $M$ artinien. Il existe un entier $r$ et une application $A$-linéaire injective $f : M \to I^r$; puisque $I$ est artinien (lemme 3), le $A$-module $\operatorname{Coker}(f)$ l’est aussi, et on peut trouver un entier $s$ et une suite exacte de $A$-modules

$$
0 \to M \xrightarrow{f} I^r \xrightarrow{g} I^s .
$$

On en déduit un diagramme commutatif à lignes exactes

$$
\begin{array}{ccccccccc}
0 & \longrightarrow & M & \xrightarrow{f} & I^r & \xrightarrow{g} & I^s \\
& & \downarrow{\alpha_M} & & \downarrow{\alpha_{I^r}} & & \downarrow{\alpha_{I^s}} \\
0 & \to & D_{\widehat{A}}(D_A(M)) & \xrightarrow{D_{\widehat{A}}(D_A(f))} & D_{\widehat{A}}(D_A(I^r)) & \xrightarrow{D_{\widehat{A}}(D_A(g))} & D_{\widehat{A}}(D_A(I^s)) .
\end{array}
$$

Le $\widehat{A}$-module $D_{\widehat{A}}(D_A(I))$ s’identifie à $I$ et $\alpha_I$ à l’application identique ; par suite $\alpha_{I^r}$ et $\alpha_{I^s}$ sont bijectifs, et il en est de même de $\alpha_M$ (A, X, p. 7, cor. 3).

Si le $A$-module $M$ est de type fini, il existe des entiers $m$ et $n$ et une suite exacte de $A$-modules

$$
A^m \longrightarrow A^n \longrightarrow M \to 0 ;
$$

on en déduit un diagramme commutatif à lignes exactes

$$
\begin{array}{ccccccccc}
\widehat{A}^m & \longrightarrow & \widehat{A}^n & \longrightarrow & \widehat{A} \otimes_A M & \longrightarrow & 0 \\
\downarrow{\widehat{\alpha}_{A^m}} & & \downarrow{\widehat{\alpha}_{A^n}} & & \downarrow{\widehat{\alpha}_M} & & \\
\widehat{A}^m & \longrightarrow & \widehat{A}^n & \longrightarrow & D_A(D_A(M)) & \to & 0 .
\end{array}
$$

Comme $\widehat{\alpha}_A$ est égal à $1_{\widehat{A}}$, il en résulte que $\widehat{\alpha}_M$ est un isomorphisme.

Il reste à prouver l’égalité $\operatorname{long}_A(M) = \operatorname{long}_A(D_A(M))$ lorsque $M$ est de longueur finie. On peut supposer $M \neq 0$; il existe alors une suite exacte

$$
0 \to \kappa_A \longrightarrow M \longrightarrow N \to 0 ,
$$

d’où l’on déduit une suite exacte

$$
0 \to D_A(N) \longrightarrow D_A(M) \longrightarrow D_A(\kappa_A) \to 0 .
$$

On a $\operatorname{long}_A(M) = \operatorname{long}_A(N) + 1$ et

$$
\operatorname{long}_A(D_A(M)) = \operatorname{long}_A(D_A(N)) + \operatorname{long}_A(D_A(\kappa_A)) = \operatorname{long}_A(D_A(N)) + 1 ;
$$

on conclut par récurrence sur l’entier $\operatorname{long}_A(M)$.

#### Remarque {#ac-x-s8-n3-rem-1 .statement}

Supposons l’anneau $A$ artinien. On a $\operatorname{long}_A(I) = \operatorname{long}_A(D_A(A)) = \operatorname{long}(A)$ (th. 2, c)). Soit $M$ un $A$-module de type fini ; il admet une enveloppe injective isomorphe à $I^s$, où $s$ est la dimension du socle de $M$ (lemme 4). Par suite on a $\operatorname{long}_A(M) \leq s \operatorname{long}(A)$; pour qu’il y ait égalité, il faut et il suffit que $M$ soit injectif. En particulier, pour que le $A$-module $A$ soit injectif, il faut et il suffit que son socle soit de dimension 1 ; on retrouve ainsi le lemme 1 du § 3, n° 7.

### 4. Dualité des modules de longueur finie

Soit $A$ un anneau noethérien ; notons $\Omega$ l’ensemble de ses idéaux maximaux. Généralisant la définition donnée dans le numéro précédent, nous dirons qu’un $A$-module $J$ est un $A$-module de Matlis s’il est injectif, que ses idéaux premiers associés sont les idéaux maximaux de $A$, et que pour tout idéal maximal $m$ de $A$ le $A/m$-espace vectoriel $\operatorname{Hom}_A(A/m, J)$ est de dimension 1. Pour tout $m \in \Omega$, choisissons une enveloppe injective $\kappa(m) \to I(m)$ du $A$-module $\kappa(m)$; le $A$-module $\bigoplus_{m \in \Omega} I(m)$ est un module de Matlis, et tout $A$-module de Matlis lui est isomorphe (n° 1, th. 1).

Rappelons (VIII, § 1, n° 5) qu’on note $Z_0(A)$ le $\mathbf{Z}$-module $\mathbf{Z}^{(\Omega)}$ et $\varepsilon : Z_0(A) \to \mathbf{Z}$ la forme linéaire qui applique chaque élément de la base $\Omega$ sur 1. Si $M$ est un $A$-module de longueur finie, le $A_m$-module $M_m$ est de longueur finie pour tout $m \in \Omega$, et nul sauf pour un nombre fini d’idéaux $m \in \Omega$. On pose

$$
z_0(M) = \sum_{m \in \Omega} \operatorname{long}_{A_m}(M_m)[m] \text{ dans } Z_0(A) ;
$$

on a $\operatorname{long}_A(M) = \varepsilon(z_0(M))$ (*loc. cit.*, exemple 3). Inversement, un $A$-module $N$ tel que $\operatorname{long}_{A_m}(N_m)$ soit finie pour tout $m \in \Omega$, et nulle en dehors d’un sous-ensemble fini $I$ de $\Omega$, est de longueur finie : en effet $N$ est isomorphe à un sous-module de $\bigoplus_{m \in I} N_m$ (II, § 3, n° 3, cor. 2 du th. 1), et l’on a $\operatorname{long}_{A_m}(N_m) = \operatorname{long}_A(N_m)$ puisque tout $A_m$-module simple est isomorphe à $\kappa(m)$, donc simple en tant que $A$-module.

Soit $J$ un $A$-module de Matlis. Pour tout $A$-module $M$, nous noterons $D_A(M)$ ou simplement $D(M)$ le $A$-module $\operatorname{Hom}_A(M, J)$. Soit $\alpha_M$ l’homomorphisme de $M$ dans $D(D(M))$ défini par $\alpha_M(m)(f) = f(m)$ pour $m \in M,\ f \in D(M)$.

#### Proposition 4 {#ac-x-s8-prop-4 .statement}

Pour que le A-module M soit de longueur finie, il faut et il suffit que D(M) soit de longueur finie. On a alors $z_0(D(M)) = z_0(M)$, $\operatorname{long}_A(M) = \operatorname{long}_A D(M)$, $\operatorname{Ann}_A(M) = \operatorname{Ann}_A(D(M))$, et l’application A-linéaire $\alpha_M$ est bijective.

Pour tout $m \in \Omega$, le $A_m$-module $D(M)_m$ s’identifie à $\operatorname{Hom}_{A_m}(M_m, J_m)$ (II, § 2, n° 7, prop. 19) ; la première assertion de la proposition résulte alors du th. 2, c) et de la caractérisation des modules de longueur finie donnée ci-dessus. Supposons désormais M de longueur finie ; on a $\operatorname{long}_{A_m}(D(M)_m) = \operatorname{long}_{A_m}(M_m)$ pour tout $m \in \Omega$ (*loc. cit.*), d’où $z_0(D(M)) = z_0(M)$ et $\operatorname{long}_A(D(M)) = \operatorname{long}_A(M)$. De plus l’application $(\alpha_M)_m : M_m \to D(D(M))_m$ s’identifie à l’homomorphisme canonique $\alpha_{M_m}$, qui est bijectif (*loc. cit.*) ; par suite $\alpha_M$ est bijectif.

Pour tout $a \in A$ on a $D(a_M) = a_{D(M)}$ et par suite $\operatorname{Ann}_A(M) \subset \operatorname{Ann}_A(D(M))$. Appliquant cela au A-module D(M) on en déduit l’inclusion opposée, d’où l’égalité $\operatorname{Ann}_A(M) = \operatorname{Ann}_A(D(M))$.

#### Exemple {#ac-x-s8-n4-exa-1 .statement}

Soient A un anneau principal, K son corps des fractions. *Le A-module K/A est un module de Matlis* : en effet l’application canonique de K/A dans $\prod_{m \in \Omega} K/A_m$ induit un isomorphisme de K/A dans $\bigoplus_{m \in \Omega} K/A_m$ (A, VII, p. 10, th. 2) ; l’assertion résulte alors du n° 1, exemple 1. Nous avons d’ailleurs déjà démontré en A, VII, § 4, n° 9 que l’application $\alpha_M$ est bijective pour tout A-module M de longueur finie lorsque l’anneau A est principal.

### 5. Foncteurs dualisants

Dans ce numéro, on fixe un anneau local noethérien A. On suppose donnés
a) pour tout A-module M de longueur finie, un A-module T(M) ;
b) pour toute application A-linéaire $f : M \to N$ entre A-modules de longueur finie, une application A-linéaire $T(f) : T(N) \to T(M)$,
de façon que les conditions suivantes soient satisfaites :
FD 1) Les applications $f \mapsto T(f)$ sont A-linéaires.
FD 2) Pour tout A-module de longueur finie M, on a $T(1_M) = 1_{T(M)}$.
FD 3) Pour tout diagramme $M \xrightarrow{f} N \xrightarrow{g} P$ de A-modules de longueur finie et d’applications A-linéaires, on a $T(g \circ f) = T(f) \circ T(g)$.
FD 4) Pour toute suite exacte $M' \xrightarrow{u} M \xrightarrow{v} M''$ de A-modules de longueur finie, la suite $T(M'') \xrightarrow{T(v)} T(M) \xrightarrow{T(u)} T(M')$ est exacte.
FD 5) Le A-module $T(\kappa_A)$ est de longueur 1.

De FD 1) et FD 2), on tire $T(a_M) = a T(1_M) = a 1_{T(M)} = a_{T(M)}$ pour tout $a \in A$. Prenant $M = \{0\}$, on obtient $0_{T(M)} = 1_{T(M)}$, donc $T(\{0\}) = \{0\}$. Il résulte de là et de FD 4) que pour toute application linéaire injective (resp. surjective) entre A-modules de longueur finie, l’application $T(f)$ est surjective (resp. injective).

Soit $M$ un $A$-module de longueur finie. Alors $T(M)$ est de longueur finie et l’on a $\operatorname{long}_A(T(M)) = \operatorname{long}_A(M)$ : cela résulte en effet de FD 4) et FD 5) et du fait que tout module de longueur finie admet une suite de composition dont les quotients sont isomorphes à $\kappa_A$.

Soient $M$ un $A$-module de longueur finie, et $(e_\lambda)_{\lambda \in L}$ une famille orthogonale de projecteurs de $M$ ; d’après FD 3), $(T(e_\lambda))_{\lambda \in L}$ est une famille orthogonale de projecteurs de $T(M)$. Par suite, si $M$ est somme directe d’une famille de sous-modules $(M_\lambda)_{\lambda \in L}$, et si $p_\lambda$ désigne la projection de $M$ sur $M_\lambda$, l’homomorphisme
$$
\sum_{\lambda \in L} T(p_\lambda) : \bigoplus_{\lambda \in L} T(M_\lambda) \longrightarrow T(M)
$$
est un isomorphisme.

#### Exemple 1 {#ac-x-s8-n5-exa-1 .statement}

Soit $J$ un $A$-module de Matlis. Posons $T(M) = \operatorname{Hom}_A(M, J)$ pour tout $A$-module $M$ de longueur finie et $T(f) = \operatorname{Hom}_A(f, 1_J)$ pour toute application $A$-linéaire $f$ entre $A$-modules de longueur finie. Alors les conditions FD 1) à FD 5) sont satisfaites. Nous allons voir ci-dessous (th. 3) que toute construction satisfaisant les conditions FD 1) à FD 5) est obtenue de cette façon.

#### Exemple 2 {#ac-x-s8-n5-exa-2 .statement}

Soient $C$ un complexe injectif de $A$-modules et $d$ un entier tels que $H^i(\operatorname{Homgr}_A(\kappa_A, C))$ soit nul pour $i \neq d$ et soit de longueur 1 pour $i = d$. Pour tout $A$-module $M$ de longueur finie, on a $H^i(\operatorname{Homgr}_A(M, C)) = 0$ pour $i \neq d$ : raisonnons en effet par récurrence sur la longueur de $M$, supposée $> 0$ ; il existe une suite exacte de $A$-modules $0 \to \kappa_A \to M \to N \to 0$, qui donne naissance à une suite exacte de complexes
$$
0 \to \operatorname{Homgr}_A(N, C) \longrightarrow \operatorname{Homgr}_A(M, C) \longrightarrow \operatorname{Homgr}_A(\kappa_A, C) \longrightarrow 0
$$
et la conclusion résulte de l’hypothèse de récurrence appliquée à $N$.

Posons $T(M) = H^d(\operatorname{Homgr}_A(M, C))$ pour tout $A$-module $M$ de longueur finie, et $T(f) = H^d(\operatorname{Homgr}_A(f, 1_C))$ pour toute application $A$-linéaire $f$ entre $A$-modules de longueur finie ; les conditions FD 1) à FD 5) sont satisfaites.

#### Exemple 3 {#ac-x-s8-n5-exa-3 .statement}

Soient $\Omega$ un $A$-module et $d$ un entier $\geqslant 0$ tels que $\operatorname{Ext}_A^i(\kappa_A, \Omega)$ soit nul pour $i \neq d$ et soit de longueur 1 pour $i = d$. Posons $T(M) = \operatorname{Ext}_A^d(M, \Omega)$ pour tout $A$-module de longueur finie $M$ et $T(f) = \operatorname{Ext}_A^d(f, 1_\Omega)$ pour toute application $A$-linéaire $f$ entre $A$-modules de longueur finie. On a alors $\operatorname{Ext}_A^i(M, \Omega) = 0$ pour tout $A$-module de longueur finie $M$ et tout $i \neq d$, et les conditions FD 1) à FD 5) sont satisfaites : il suffit en effet d’appliquer l’exemple précédent au cas où $C$ est la résolution injective canonique de $\Omega$.

#### Exemple 4 {#ac-x-s8-n5-exa-4 .statement}

Si $A$ est un anneau de Gorenstein, par exemple un anneau régulier, on peut appliquer l’exemple 3 en prenant $\Omega = A$ et $d = \dim(A)$ (§ 3, n° 7, prop. 11).

Pour tout entier $n \geqslant 0$, posons $I_n = T(A/\mathfrak{m}_A^n)$. Pour $m \geqslant n$, notons $p_{mn} : A/\mathfrak{m}_A^m \longrightarrow A/\mathfrak{m}_A^n$ la surjection canonique et $i_{mn} : T(A/\mathfrak{m}_A^n) \longrightarrow T(A/\mathfrak{m}_A^m)$ l’application $A$-linéaire $T(p_{mn})$. Elle est injective par FD 4) et l’on a $i_{mn} \circ i_{np} = i_{mp}$ pour $m \geqslant n \geqslant p$ par FD 3). Soit $I = \varprojlim T(A/\mathfrak{m}_A^n)$ le $A$-module limite inductive du système $((I_n), (i_{mn}))$. Pour $n \geqslant 0$, l’application canonique $I_n \to I$ est injective ; nous identifierons $I_n$ à son image dans $I$, de sorte que $I$ est la réunion croissante des $I_n$.

Soient M un A-module de longueur finie, et n un entier $\geqslant 0$ tel que $m_A^n M = 0$. Pour $x \in M$, notons $\varphi_{M,x}^n$ l’application A-linéaire de $A/m_A^n$ dans M qui applique la classe de 1 sur x. L’application $T(\varphi_{M,x}^n) : T(M) \to I_n$ est A-linéaire, et l’on a $T(\varphi_{M,a x}^n) = a T(\varphi_{M,x}^n)$ pour $a \in A$ par FD 1). Par suite l’application $(x, u) \mapsto T(\varphi_{M,x}^n)(u)$ de $M \times T(M)$ dans I est A-bilinéaire. Elle ne dépend pas du choix de l’entier n : en effet, pour tout entier $q \geqslant n$ et tout élément x de M, on a $\varphi_{M,x}^q = \varphi_{M,x}^n \circ p_{q n}$, d’où par FD 3) $T(\varphi_{M,x}^q) = i_{q n} \circ T(\varphi_{M,x}^n)$. On en déduit une application A-linéaire
$$
\theta_M : T(M) \longrightarrow \operatorname{Hom}_A(M, I)
$$
satisfaisant à $\theta_M(u)(x) = T(\varphi_{M,x})(u)$ pour $u \in T(M),\ x \in M$.

#### Théorème 3 {#ac-x-s8-thm-3 .statement}

a) Le A-module I est un module de Matlis. Pour tout entier $m \geqslant 0$, $I_m$ est le sous-module de I formé des éléments annulés par $m_A^m$.

b) Pour tout A-module M de longueur finie, l’application A-linéaire $\theta_M : T(M) \to \operatorname{Hom}_A(M, I)$ est bijective.

c) Pour toute application A-linéaire $f : M \to N$ entre A-modules de longueur finie, on a $\theta_M \circ T(f) = \operatorname{Hom}_A(f, 1_I) \circ \theta_N$.

Prouvons c). Soient n un entier et M, N des A-modules de longueur finie annulés par $m_A^n$. Soit $f : M \to N$ une application A-linéaire. Pour $u$ dans $T(N)$ et x dans M, on a d’après FD 3)
$$
\begin{align*}
\theta_M(T(f)(u))(x) &= T(\varphi_{M,x}^n)(T(f)(u)) = T(f \circ \varphi_{M,x}^n)(u) \\
&= T(\varphi_{N,f(x)}^n)(u) = \theta_N(u)(f(x)) = (\theta_N(u) \circ f)(x) .
\end{align*}
$$
Cela prouve c).

Prouvons b). Considérons d’abord le cas particulier $M = A/m_A^n$. Alors $T(M)$ est égal par définition à $I_n$. Si $a$ est un élément de A, de classe $\bar{a}$ dans M, on a $\varphi_{M,\bar{a}}^n = a 1_M$, d’où $T(\varphi_{M,\bar{a}}^n) = a 1_{I_n}$; ainsi $\theta_M : I_n \to \operatorname{Hom}_A(A/m_A^n, I)$ est l’isomorphisme canonique qui envoie un élément $x$ de $I_n$ sur l’application $\bar{a} \mapsto a x$. Cela démontre b) dans ce cas.

Supposons maintenant donnée une suite exacte
$$
P \xrightarrow{u} N \xrightarrow{v} M \to 0
$$
de A-modules de longueur finie annulés par $m_A^n$. Considérons le diagramme
$$
\begin{array}{ccccccccc}
0 & \longrightarrow & T(M) & \xrightarrow{T(v)} & T(N) & \xrightarrow{T(u)} & T(P) \\
   &                & \downarrow{\theta_M} &           & \downarrow{\theta_N} &           & \downarrow{\theta_P} \\
0 & \longrightarrow & \operatorname{Hom}_A(M, I) & \xrightarrow{\operatorname{Hom}(v, 1)} & \operatorname{Hom}_A(N, I) & \xrightarrow{\operatorname{Hom}(u, 1)} & \operatorname{Hom}_A(P, I)
\end{array}
$$

il est commutatif d’après le début de la démonstration, et ses lignes sont exactes par FD 4). On en déduit que $\theta_M$ est bijectif si $\theta_P$ et $\theta_N$ le sont. Appliquant cela à une présentation
$$
(A/\mathfrak{m}_A^n)^r \longrightarrow (A/\mathfrak{m}_A^n)^s \longrightarrow M \longrightarrow 0
$$
du $A/\mathfrak{m}_A^n$-module $M$, on en déduit que $\theta_M$ est bijectif pour tout $A$-module de longueur finie annulé par $\mathfrak{m}_A^n$, d’où b).

Prouvons a). Il résulte de ce qui précède appliqué au $A$-module $A/\mathfrak{m}_A^n$ que $I_n$ est l’ensemble des éléments de $I$ qui sont annulés par $\mathfrak{m}_A^n$. Par FD 5) le $A$-module $I_1 = T(\kappa_A)$ est isomorphe à $\kappa_A$; d’après la prop. 2 du n° 2, il nous suffit de prouver que, pour tout entier $n \geqslant 0$, l’application $A$-linéaire canonique
$$
\beta : I_{n+1}/I_n \longrightarrow \mathrm{Hom}_A(\mathfrak{m}_A^n/\mathfrak{m}_A^{n+1}, I)
$$
est bijective. Or de la suite exacte
$$
0 \longrightarrow \mathfrak{m}_A^n/\mathfrak{m}_A^{n+1} \xrightarrow{u} A/\mathfrak{m}_A^{n+1} \xrightarrow{p_{n+1,n}} A/\mathfrak{m}_A^n \longrightarrow 0,
$$
on tire une suite exacte
$$
0 \longrightarrow I_n \xrightarrow{i_{n+1,n}} I_{n+1} \xrightarrow{T(u)} T(\mathfrak{m}_A^n/\mathfrak{m}_A^{n+1}) \longrightarrow 0.
$$
Composant $T(u)$ avec $\theta_{\mathfrak{m}_A^n/\mathfrak{m}_A^{n+1}}$, on obtient donc un homomorphisme surjectif
$$
\gamma : I_{n+1} \longrightarrow \mathrm{Hom}_A(\mathfrak{m}_A^n/\mathfrak{m}_A^{n+1}, I)
$$
de noyau $I_n$. D’après c), $\gamma$ est la composée des flèches $\theta_{I_{n+1}} : I_{n+1} \to \mathrm{Hom}_A(A/\mathfrak{m}_A^{n+1}, I)$ et $\mathrm{Hom}(u, 1) : \mathrm{Hom}_A(A/\mathfrak{m}_A^{n+1}, I) \to \mathrm{Hom}_A(\mathfrak{m}_A^n/\mathfrak{m}_A^{n+1}, I)$; comme $\theta_{I_{n+1}}$ est l’application linéaire associée à la multiplication $A/\mathfrak{m}_A^{n+1} \times I_{n+1} \to I$, l’isomorphisme $I_{n+1}/I_n \to \mathrm{Hom}_A(\mathfrak{m}_A^n/\mathfrak{m}_A^{n+1}, I)$ déduit de $\gamma$ coïncide avec $\beta$, ce qui achève la démonstration.

#### Exemple 5 {#ac-x-s8-n5-exa-5 .statement}

Reprenons les hypothèses et notations de l’exemple 1. Alors $T(A/\mathfrak{m}_A^n) = \mathrm{Hom}_A(A/\mathfrak{m}_A^n, J)$ s’identifie au sous-module $J_n$ de $J$ formé des éléments annulés par $\mathfrak{m}_A^n$; par passage à la limite inductive on obtient un isomorphisme canonique de $I$ sur $J$.

#### Exemple 6 {#ac-x-s8-n5-exa-6 .statement}

Reprenons les hypothèses et notations de l’exemple 3. On obtient que $I = \varinjlim \mathrm{Ext}_A^d(A/\mathfrak{m}_A^n, \Omega)$ est un $A$-module de Matlis. Pour tout $A$-module de longueur finie $M$, on dispose d’un $A$-isomorphisme canonique
$$
0_M : \mathrm{Ext}_A^d(M, \Omega) \longrightarrow \mathrm{Hom}_A(M, I);
$$
de plus cet isomorphisme est $\mathrm{End}_A(M)$-linéaire (th. 3, c)).

En particulier, si l’anneau $A$ est de Gorenstein de dimension $d$, le $A$-module $\varinjlim \mathrm{Ext}_A^d(A/\mathfrak{m}_A^n, A)$ est un module de Matlis.

### 6. Changement d’anneaux ; dualité de Macaulay

#### Proposition 5 {#ac-x-s8-prop-5 .statement}

Soit $\rho : A \to B$ un homomorphisme local d’anneaux locaux noethériens, tel que l’extension résiduelle $\kappa_A \to \kappa_B$ induite par $\rho$ soit de degré fini. Soit $I_A$ un $A$-module de Matlis.

a) Notons $I_B$ le sous-B-module de $\mathrm{Hom}_A(B, I_A)$ formé des $A$-homomorphismes de $B$ dans $I_A$ dont le noyau contient une puissance de $m_B$. Alors $I_B$ est un $B$-module de Matlis.

b) Soit $M$ un $B$-module. L’application canonique

$$
\alpha : \mathrm{Hom}_B(M, \mathrm{Hom}_A(B, I_A)) \longrightarrow \mathrm{Hom}_A(M, I_A)
$$

définie par $\alpha(u)(m) = u(m)(1)$ induit un $B$-isomorphisme de $D_B(M) = \mathrm{Hom}_B(M, I_B)$ sur le sous-B-module $\mathrm{Hom}_A^{cont}(M, I_A)$ de $D_A(M) = \mathrm{Hom}_A(M, I_A)$ formé des applications $f : M \to I_A$ telles que pour tout élément $m$ de $M$, il existe un entier $n \geqslant 0$ tel que $f(m^n_B m) = 0$.

La condition ci-dessus sur $f$ signifie que $f$ est continue lorsqu’on munit $I_A$ de la topologie discrète et $M$ de la topologie la plus fine qui induise sur chaque sous-module de type fini la topologie $m_B$-adique, ce qui justifie la notation. De même, la condition $g \in I_B$ signifie que $g$ est continue lorsqu’on munit $I_A$ de la topologie discrète et $B$ de la topologie $m_B$-adique.

Prouvons a). Pour tout $B$-module de longueur finie $M$, notons $T(M)$ le $B$-module $\mathrm{Hom}_A(M, I_A)$; pour toute application $B$-linéaire $f : M \to N$ entre $B$-modules de longueur finie, notons $T(f) : T(N) \to T(M)$ l’application $B$-linéaire $\mathrm{Hom}_A(f, 1_{I_A})$. La vérification des conditions FD 1) à FD 4) du n° 5 est immédiate. Par ailleurs, pour tout $B$-module de longueur finie $N$, on a $\mathrm{long}_A(N_{[A]}) = \mathrm{long}_B(N) \ [\kappa_B : \kappa_A]$; comme on a $\mathrm{long}_A(T(M)) = \mathrm{long}_A(M)$ (n° 3, th. 2), on en déduit $\mathrm{long}_B(T(M)) = \mathrm{long}_B(M)$, ce qui implique FD 5). On peut donc appliquer le théorème 3 du n° 5; on a

$$
T(B/m_B^n) = \mathrm{Hom}_A(B/m_B^n, I_A),
$$

de sorte que le $B$-module de Matlis $\varprojlim T(B/m_B^n)$ s’identifie au sous-B-module $I_B$ de $\mathrm{Hom}_A(B, I_A)$, ce qui prouve a).

Prouvons b). L’application $\alpha$ est l’inverse de l’isomorphisme canonique

$$
\beta : \mathrm{Hom}_A(M, 1_A) \longrightarrow \mathrm{Hom}_B(M, \mathrm{Hom}_A(B, I_A))
$$

qui associe à $v \in \mathrm{Hom}_A(M, I_A)$ l’application $v'$ de $M$ dans $\mathrm{Hom}_A(B, I_A)$ telle que $v'(m)(b) = v(bm)$ (A, II, p. 74, prop. 1). Pour que $v'$ prenne ses valeurs dans $I_B$, il faut et il suffit que $v$ appartienne à $\mathrm{Hom}_A^{cont}(M, I_A)$, d’où b).

#### Corollaire {#ac-x-s8-n6-cor-1 .statement}

a) Si la $A$-algèbre $B$ est finie, le $B$-module $I_B = \mathrm{Hom}_A(B, I_A)$ est un $B$-module de Matlis.

b) Si le $B$-module $M$ est artinien, l’application $\alpha$ est un $B$-isomorphisme de $D_B(M)$ sur $D_A(M)$.

La prop. 5 s’applique notamment lorsque $A$ est un corps $k$, auquel cas on peut prendre $I_A = k$, donc $D_k(M) = \mathrm{Hom}_k^{cont}(M, k)$ (« dualité de Macaulay »). On notera que l’hypothèse $[\kappa_B : k] < +\infty$ est en particulier satisfaite lorsque la $k$-algèbre $B$ est l’anneau local en un idéal maximal d’une $k$-algèbre de type fini (A, VIII, App. 3, cor. 1).

Plus particulièrement, considérons une $k$-algèbre de type fini $S$, graduée de type $\mathbf{N}$, telle que $S_0$ soit un corps, extension de degré fini de $k$. On peut appliquer la prop. 5 à l’anneau local $S'$ de $S$ en l’idéal maximal $S_+ = \bigoplus_{n > 0} S_n$ ou, ce qui revient au même, à son complété $\widehat{S} = \prod_{n \geq 0} S_n$ (III, § 1, n° 3, lemme 2 et § 2, n° 12, exemple 1). Le $S$-module $I_{\widehat{S}} = \mathrm{Hom}_k^{cont}(\widehat{S}, k)$ s’identifie alors à
$$
S^{*gr} = \bigoplus_{n \geq 0} \mathrm{Hom}_k(S_n, k)
$$
pour $s \in S$ et $u \in S^{*gr}$, l’élément $su$ de $S^{*gr}$ est le produit intérieur $s \perp u$ (A, III, p. 156 et p. 157). Prenons par exemple $S = k[T_1, \ldots, T_d]$, d’où $\widehat{S} = k[[T_1, \ldots, T_d]]$. Notons $(u_\alpha)_{\alpha \in \mathbf{N}^d}$ la base du $k$-espace vectoriel $S^{*gr}$ duale de la base $(T^\alpha)_{\alpha \in \mathbf{N}^d}$ de $S$. La structure de $S$-module de $S^{*gr}$ est alors décrite par les formules (A, III, p. 167)

$$
\begin{align*}
T^\beta u_\alpha &= u_\alpha \cdot \beta & \text{si } \alpha \geq \beta , \\
T^\beta u_\alpha &= 0 & \text{sinon}.
\end{align*}
$$

### 7. Dualité des modules d’extensions et des produits de torsion

Soient $A$ un anneau, $P$ et $J$ des $A$-modules. Pour tout complexe $C$ de $A$-modules, on a construit en A, X, p. 99, prop. 12 un isomorphisme canonique de complexes
$$
\mu : \mathrm{Homgr}_A(C \otimes_A P, J) \longrightarrow \mathrm{Homgr}_A(C, \mathrm{Hom}_A(P, J)) .
$$
Soient $M$ un $A$-module, et $(C, p)$ une résolution projective de $M$. Considérons la suite d’homomorphismes
$$
\begin{array}{ccccccccc}
\mathrm{Ext}_A(M, \mathrm{Hom}_A(P, J)) & \xrightarrow{\varphi^{-1}} & \mathrm{H}(\mathrm{Homgr}_A(C, \mathrm{Hom}_A(P, J))) & \xrightarrow{\mathrm{H}(\mu)^{-1}} & \mathrm{H}(\mathrm{Homgr}_A(C \otimes_A P, J)) \\
& \xrightarrow{u} & \mathrm{Homgr}_A(\mathrm{H}(C \otimes_A P), J) & \xrightarrow{v} & \mathrm{Homgr}_A(\mathrm{Tor}^A(M, P), J) ,
\end{array}
$$

où $\varphi$ est l’isomorphisme canonique $\varphi(C, \mathrm{Hom}_A(P, J))$ (A, X, p. 100, th. 1), $u$ l’homomorphisme canonique $\lambda(C \otimes_A P, J)$ (A, X, p. 82), et $v$ est déduit de l’isomorphisme canonique $\psi(C, P) : \mathrm{Tor}^A(M, P) \longrightarrow \mathrm{H}(C \otimes_A P)$.

Soit $(C', p')$ une autre résolution projective de $M$. D’après A, X, p. 49, cor. de la prop. 3, il existe un homotopisme de complexes $\alpha : C' \to C$ tel que $p \circ \alpha = p'$. Il résulte de A, X, p. 103, prop. 2, que l’on a $\mathrm{H}(\alpha \otimes 1_P) \circ \psi(C', P) = \psi(C, P)$ et $\varphi(C', R) \circ \mathrm{H}(\mathrm{Homgr}(\alpha, 1_R)) = \varphi(C, R)$ pour tout A-module $R$. On en déduit que l’homomorphisme gradué de degré 0

$$
\theta(M, P) : \mathrm{Ext}_A(M, \mathrm{Hom}_A(P, J)) \longrightarrow \mathrm{Homgr}_A(\mathrm{Tor}^A(M, P), J)
$$

composé de la suite d’homomorphismes ci-dessus est indépendant du choix de la résolution projective $(C, p)$ de $M$. Par construction il est $\mathrm{End}_A(J)$-linéaire.

La définition de l’homomorphisme $\theta(M, P)$ s’explicite de la façon suivante. Soient $p$ un entier, $v$ un élément de $\mathrm{Ext}_A^p(M, \mathrm{Hom}_A(P, J))$, $\tau$ un élément de $\mathrm{Tor}_p^A(M, P)$. À l’aide de l’isomorphisme $\varphi(C, \mathrm{Hom}_A(P, J))$, $v$ est représenté par une application linéaire $u : C_p \to \mathrm{Hom}_A(P, J)$ telle que $u \circ d_C = 0$; de même, à l’aide de $\psi(C, P)$, $\tau$ est représenté par un élément $\sum c_\mu \otimes p_\mu$ de $C_p \otimes P$ tel que $\sum d_C(c_\mu) \otimes p_\mu = 0$. On a alors $\theta(M, P)(v)(\tau) = \sum u(c_\mu)(p_\mu)$.

D’autre part, soit $v : C \otimes_A \mathrm{Hom}_A(P, J) \longrightarrow \mathrm{Homgr}_A(\mathrm{Homgr}_A(C, P), J)$ l’homomorphisme qui applique l’élément $c \otimes h$, pour $c \in C_p$, $h \in \mathrm{Hom}_A(P, J)$, sur l’homomorphisme $u \mapsto (-1)^p h(u(c))$. Il est gradué de degré 0 ; il est bijectif si chaque module $C_p$ est libre de type fini. On vérifie sans peine que c’est un morphisme de complexes.

Considérons la suite d’homomorphismes

$$
\begin{array}{cccccc}
\mathrm{Tor}^A(M, \mathrm{Hom}_A(P, J)) & \xrightarrow{\psi} & \mathrm{H}(C \otimes_A \mathrm{Hom}_A(P, J)) & \xrightarrow{\mathrm{H}(v)} & \mathrm{H}(\mathrm{Homgr}_A(\mathrm{Homgr}_A(C, P), J)) \\
& \xrightarrow{w} & \mathrm{Homgr}_A(\mathrm{H}(\mathrm{Homgr}_A(C, P)), J) & \xrightarrow{t} & \mathrm{Homgr}_A(\mathrm{Ext}_A(M, P), J)
\end{array}
$$

où $\psi$ est l’isomorphisme canonique $\psi(C, \mathrm{Hom}_A(P, J))$, $w$ l’homomorphisme canonique $\lambda(\mathrm{Homgr}_A(C, P), J)$ (A, X, p. 82) et $t$ est déduit de l’isomorphisme canonique $\varphi(C, P)$. On voit comme ci-dessus que l’homomorphisme composé

$$
\rho(M, P) : \mathrm{Tor}^A(M, \mathrm{Hom}_A(P, J)) \longrightarrow \mathrm{Homgr}_A(\mathrm{Ext}_A(M, P), J)
$$

est indépendant du choix de la résolution $C$; il est $\mathrm{End}_A(J)$-linéaire. Soient $p$ un entier, $\xi \in \mathrm{Tor}_p^A(M, \mathrm{Hom}_A(P, J))$, $\lambda \in \mathrm{Ext}_A^p(M, P), J)$; si $\xi$ est représenté à l’aide de $\psi(C, \mathrm{Hom}_A(P, J))$ par un élément $\sum c_\mu \otimes u_\mu$ de $C \otimes \mathrm{Hom}_A(P, J)$ tel que $\sum d_C(c_\mu) \otimes u_\mu = 0$, et $\lambda$ à l’aide de $\varphi(C, P)$ par un homomorphisme $\ell : C_p \to P$ tel que $\ell \circ d_C = 0$, on a $\rho(M, P)(\xi)(\lambda) = (-1)^p \sum u_\mu(\ell(c_\mu))$.

#### Proposition 6 {#ac-x-s8-prop-6 .statement}

*Supposons le A-module J injectif ; pour tout A-module N, possons D(N) = \mathrm{Hom}_A(N, J).*

a) Les homomorphismes $\theta^i(M, P) : \mathrm{Ext}_A^i(M, D(P)) \longrightarrow D(\mathrm{Tor}_i^A(M, P))$ sont bijectifs.

b) Si l’anneau $A$ est noethérien et le $A$-module $M$ de type fini, les homomorphismes $\rho_i(M, P) : \mathrm{Tor}_i^A(M, D(P)) \longrightarrow D(\mathrm{Ext}_A^i(M, P))$ sont bijectifs.

a) Par construction, l’homomorphisme $\theta(M, P)$ est bijectif dès que $\lambda(C \otimes_A P, J)$ est bijectif, ce qui est le cas lorsque $J$ est injectif (A, X, p. 85, cor. 2).

b) Choisissons la résolution $C$ de façon que chaque module $C_p$ soit libre de type fini (A, X, p. 53, prop. 6). Alors l’homomorphisme $\nu$ est bijectif, il en est de même de $\lambda(\mathrm{Homgr}_A(C, P), J)$ puisque $J$ est injectif, donc $\rho(M, P)$ est bijectif.

#### Remarque 1 {#ac-x-s8-n7-rem-1 .statement}

Pour tout homomorphisme $f : N \to N'$ de $A$-modules, notons $D(f) : D(N') \to D(N)$ l’homomorphisme $\mathrm{Hom}(f, 1_J)$. Soient $u : M \to M'$ et $v : P \to P'$ des homomorphismes de $A$-modules. Choisissons des résolutions projectives $(C, p)$ de $M$ et $(C', p')$ de $M'$, et un morphisme de complexes $\tilde{u} : C \to C'$ tel que $p' \circ \tilde{u} = u \circ p$ (A, X, p. 49, prop. 3). Le diagramme

$$
\begin{array}{ccc}
\mathrm{Homgr}_A(C' \otimes_A P', J) & \xrightarrow{\mu'} & \mathrm{Homgr}_A(C', \mathrm{Hom}_A(P', J)) \\
\downarrow \mathrm{Hom}(\tilde{u} \otimes v, 1_J) & & \downarrow \mathrm{Hom}(\tilde{u}, \mathrm{Hom}(v, 1)) \\
\mathrm{Homgr}_A(C \otimes_A P, J) & \xrightarrow{\mu} & \mathrm{Homgr}_A(C, \mathrm{Hom}_A(P, J))
\end{array}
$$

où $\mu$ et $\mu'$ sont les homomorphismes canoniques, est commutatif ; on déduit alors de A, X, p. 103, prop. 2 un diagramme commutatif

$$
\begin{array}{ccc}
\mathrm{Ext}_A^i(M', D(P')) & \xrightarrow{\theta^i(M', P')} & D(\mathrm{Tor}_i^A(M', P')) \\
\downarrow \mathrm{Ext}^i(u, D(v)) & & \downarrow D(\mathrm{Tor}_i(u, v)) \\
\mathrm{Ext}_A^i(M, D(P)) & \xrightarrow{\theta^i(M, P)} & D(\mathrm{Tor}_i^A(M, P))
\end{array}
$$

Soit $w : P'' \to P$ un homomorphisme de $A$-modules ; on obtient de manière analogue un diagramme commutatif

$$
\begin{array}{ccc}
\mathrm{Tor}_i^A(M, D(P)) & \xrightarrow{\rho_i(M, P)} & D(\mathrm{Ext}_A^i(M, P)) \\
\downarrow \mathrm{Tor}_i(u, D(w)) & & \downarrow D(\mathrm{Ext}^i(u, w)) \\
\mathrm{Tor}_i^A(M', D(P'')) & \xrightarrow{\rho_i(M', P'')} & D(\mathrm{Ext}_A^i(M', P''))
\end{array}
$$

#### Remarque 2 {#ac-x-s8-n7-rem-2 .statement}

Soit

$$(\mathcal{E})$$
$$0 \to M' \xrightarrow{j} M \xrightarrow{q} M'' \to 0$$

une suite exacte de $A$-modules. L’homomorphisme $L(q) : L(M) \to L(M'')$ induit sur les résolutions libres canoniques est surjectif, et le complexe $Ker\,L(q)$ définit une résolution projective de $M'$. En appliquant la prop. 3 de A, X, p. 104 à la suite exacte $0 \to Ker\,L(q) \to L(M) \to L(M'') \to 0$, on obtient des diagrammes commutatifs

$$
\begin{array}{ccc}
\mathrm{Ext}_A^i(M', D(P)) & \xrightarrow{\theta^i(M', P)} & D(\mathrm{Tor}_i^A(M', P)) \\
\downarrow & & \downarrow \\
\delta^i(\mathcal{E}, D(P)) & & (-1)^{i+1}D(\partial_{i+1}(\mathcal{E}, P))
\end{array}
$$

$$
\begin{array}{ccc}
\mathrm{Ext}_A^{i+1}(M'', D(P)) & \xrightarrow{\theta^{i+1}(M'', P)} & D(\mathrm{Tor}_{i+1}^A(M'', P)) \\
\downarrow & & \downarrow \\
\mathrm{Tor}_{i+1}^A(M'', D(P)) & \xrightarrow{\rho_{i+1}(M'', P)} & D(\mathrm{Ext}_A^{i+1}(M'', P)) \\
\downarrow & & \downarrow \\
\partial_{i+1}(\mathcal{E}, D(P)) & & (-1)^{i+1}D(\delta^i(\mathcal{E}, P))
\end{array}
$$

$$
\begin{array}{ccc}
\mathrm{Tor}_{i+1}^A(M'', D(P)) & \xrightarrow{\rho_{i+1}(M'', P)} & D(\mathrm{Ext}_A^{i+1}(M'', P)) \\
\downarrow & & \downarrow \\
\mathrm{Tor}_i^A(M', D(P)) & \xrightarrow{\rho_i(M', P)} & D(\mathrm{Ext}_A^i(M', P))
\end{array}
$$

Soit

$$(\mathcal{F})$$
$$0 \to P' \to P \to P'' \to 0$$

une suite exacte de $A$-modules ; puisque le $A$-module $J$ est injectif, on en déduit une suite exacte

$$(\mathcal{D}(\mathcal{F}))$$
$$0 \to D(P'') \to D(P) \to D(P') \to 0.$$

En appliquant A, X, p. 104, prop. 3 et p. 106, prop. 4 aux suites exactes $(\mathcal{F})$ et $(\mathcal{D}(\mathcal{F}))$, on obtient de manière analogue des diagrammes commutatifs

$$
\begin{array}{ccc}
\mathrm{Ext}_A^i(M, D(P')) & \xrightarrow{\theta^i(M, P')} & D(\mathrm{Tor}_i^A(M, P')) \\
\downarrow & & \downarrow \\
\delta^i(M, D(\mathcal{F})) & & (-1)^{i+1}D(\partial_{i+1}(M, \mathcal{F}))
\end{array}
$$

$$
\begin{array}{ccc}
\mathrm{Ext}_A^{i+1}(M, D(P'')) & \xrightarrow{\theta^{i+1}(M, P'')} & D(\mathrm{Tor}_{i+1}^A(M, P''))
\end{array}
$$

$$
\begin{array}{ccc}
\mathrm{Tor}_{i+1}^{\mathbf{A}}(M, D(P')) & \xrightarrow{\rho_{i+1}(M, P')} & D(\mathrm{Ext}_{\Lambda}^{i+1}(M, P')) \\
\downarrow & & \downarrow \\
\partial_{i+1}(M, D(\mathcal{F})) & & (-1)^i D(\delta^i(M, \mathcal{F}))
\end{array}
$$

$$
\begin{array}{ccc}
\mathrm{Tor}_{i}^{\mathbf{A}}(M, P'') & \xrightarrow{\rho_{i}(M, P'')} & D(\mathrm{Ext}_{\Lambda}^{i}(M, P''))
\end{array}
$$

## EXERCICES {#ac-x-s8-exercises}

See the [exercises for § 8](exercises/s8/).
