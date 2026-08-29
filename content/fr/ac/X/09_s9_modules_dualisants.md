---
book: ac
book_title: Commutative Algebra
chapter: X
chapter_title: Profondeur, régularité, dualité
section: 9
section_title: Modules dualisants
lang: fr
source: ac-x-fr
pdf_pages: 0124-0140, 0174-0177
extraction: ocr
subsections:
    - "no": 1
      title: Modules dualisants
      page: 0
      pdf_page: 124
    - "no": 2
      title: Quotient par une suite régulière
      page: 128
      pdf_page: 127
    - "no": 3
      title: Changement d’anneaux
      page: 130
      pdf_page: 129
    - "no": 4
      title: Structure des modules dualisants
      page: 133
      pdf_page: 132
    - "no": 5
      title: Dualité des modules de type fini
      page: 134
      pdf_page: 133
    - "no": 6
      title: 'Exemple : le cas de la dimension 1'
      page: 0
      pdf_page: 136
statements: 31
exercises: 12
content_sha256: e91759ba70639eaebfa25698b669acf6e3da97d31ed7579081129197fa443e8f
---

## § 9. MODULES DUALISANTS

### 1. Modules dualisants

#### Définition 1 {#ac-x-s9-def-1 .statement}

Soit $A$ un anneau noethérien. On dit qu’un $\Lambda$-module $\Omega$ est dualisant s’il est de type fini et si, pour tout idéal maximal $m$ de $\Lambda$, le $A/m$-espace vectoriel $\mathrm{Ext}_A^i(A/m, \Omega)$ est nul pour $i \neq \mathrm{ht}(m)$ et de dimension 1 pour $i = \mathrm{ht}(m)$.

Pour tout idéal maximal $m$ de $A$ et tout entier $i$, le $A/m$-espace vectoriel $\mathrm{Ext}_A^i(A/m, \Omega)$ est canoniquement isomorphe à $\mathrm{Ext}_{A_m}^i(A/m, \Omega_m)$ ($\S$ 3, n° 2, prop. 2). Par suite, pour qu’un $A$-module de type fini $\Omega$ soit dualisant, il faut et il suffit que le $A_m$-module $\Omega_m$ soit dualisant pour tout idéal maximal $m$ de $A$.

#### Exemple 1 {#ac-x-s9-n1-exa-1 .statement}

Si l’anneau $A$ est local et artinien, les $A$-modules dualisants sont les $A$-modules injectifs de type fini $\Omega$ tels que $\mathrm{Hom}_A(\kappa_A, \Omega)$ soit de dimension 1 ($\S$ 3, n° 3, prop. 6), c’est-à-dire les $A$-modules de Matlis ($\S$ 8, n° 3).

#### Exemple 2 {#ac-x-s9-n1-exa-2 .statement}

Pour qu’un anneau noethérien $A$ soit de Gorenstein, il faut et il suffit que le $A$-module $A$ soit dualisant ($\S$ 3, n° 7, prop. 11). En particulier, le $A$-module $A$ est dualisant lorsque $A$ est régulier.

#### Remarque 1 {#ac-x-s9-n1-rem-1 .statement}

Soient $A$ un anneau local noethérien et $\Omega$ un $A$-module de type fini. Le corps résiduel $\kappa_{\widehat{A}}$ s’identifie à $\kappa_A$, et le $\widehat{A}$-module $\widehat{\Omega}$ à $\widehat{A} \otimes_A \Omega$ (III, $\S$ 3, n° 4, th. 3). Il résulte alors de A, X, p. 111, prop. 10 que le $\kappa_A$-espace vectoriel $\mathrm{Ext}_A^i(\kappa_A, \Omega)$ est canoniquement isomorphe à $\mathrm{Ext}_{\widehat{A}}^i(\kappa_{\widehat{A}}, \widehat{\Omega})$. Par suite pour que le $A$-module $\Omega$ soit dualisant, il faut et il suffit que le $\widehat{A}$-module $\widehat{\Omega}$ soit dualisant.

#### Remarque 2 {#ac-x-s9-n1-rem-2 .statement}

Soit $\Omega$ un $A$-module dualisant ; pour tout $A$-module projectif $L$ de rang 1, le $A$-module $\Omega \otimes_A L$ est dualisant (A, X, p. 108, prop. 7, b)). Nous verrons ci-dessous (n° 4, prop. 6) que tout $A$-module dualisant est isomorphe à un module de cette forme.

#### Proposition 1 {#ac-x-s9-prop-1 .statement}

Soient $A$ un anneau noethérien et $\Omega$ un $A$-module dualisant.

a) $A$ est un anneau de Macaulay, et le $A$-module $\Omega$ est macaulayen.

b) On a $\mathrm{di}_A(\Omega) = \dim(\Omega) = \dim(A)$.

Supposons d’abord l’anneau $A$ local, et notons $d$ sa dimension. La prop. 6 du $\S$ 3, n° 3 implique $\mathrm{di}_A(\Omega) = d$, donc $\mathrm{prof}(A) = d$ d’après la prop. 9 du $\S$ 3, n° 6, de sorte que $A$ est un anneau de Macaulay. De plus, on a $\mathrm{prof}(\Omega) = d$ par définition de la profondeur ; comme on a $\mathrm{prof}(\Omega) \leq \dim(\Omega) \leq d$, on en déduit la proposition dans ce cas.

Dans le cas général, le $A_m$-module $\Omega_m$ est dualisant pour tout idéal maximal $m$ de $A$, donc $A_m$ est un anneau de Macaulay et $\Omega_m$ un $A_m$-module macaulayen d’après ce qui précède, ce qui implique a). De plus on a $\mathrm{di}_{A_m}(\Omega_m) = \dim(\Omega_m) = \dim(A_m)$ pour tout idéal maximal $m$, d’où b) par passage à la borne supérieure ($§ 3$, n° 2, prop. 3).

#### Proposition 2 {#ac-x-s9-prop-2 .statement}

*Soient A un anneau noethérien, $\Omega$ un A-module dualisant. Pour tout idéal premier $p$ de A, le $A_p$-module $\Omega_p$ est dualisant.*

Considérons une chaîne saturée $p \subset p_1 \subset \ldots \subset p_r$ d’idéaux premiers de A telle que l’idéal $p_r$ soit maximal. Raisonnant par récurrence sur $r$, on peut supposer que le $A_{p_1}$-module $\Omega_{p_1}$ est dualisant. Remplaçant A par $A_{p_1}$ et $p$ par $pA_{p_1}$, on se ramène au cas où l’anneau A est local et où la chaîne $p \subset m_A$ est saturée.

Posons alors $d = \dim(A) = \mathrm{ht}(m_A)$. On a $\dim(A_p) = \mathrm{ht}(p) = d - 1$ puisque A est un anneau de Macaulay ($§ 2$, n° 2, cor. de la prop. 2). Pour tout entier $i$, le $A_p$-module $\mathrm{Ext}^i_{A_p}(\kappa(p), \Omega_p)$ est isomorphe à $\mathrm{Ext}^i_A(A/p, \Omega)_p$ ($§ 3$, n° 2, prop. 2) ; il suffit donc de démontrer que le $A/p$-module $\mathrm{Ext}^i_A(A/p, \Omega)$ est nul pour $i \neq d - 1$ et de rang un pour $i = d - 1$.

Soient $x$ un élément de $m_A - p$, et $\overline{x}$ sa classe dans $A/p$. Considérons la suite exacte de A-modules

$$
0 \to A/p \xrightarrow{\overline{x}} A/p \longrightarrow A/(p + xA) \to 0 .
$$

Le A-module $A/(p + xA)$ est de longueur finie puisque son support est réduit à $m_A$; comme le A-module $\Omega$ est dualisant, on a $\mathrm{Ext}^i_A(A/(p + xA), \Omega) = 0$ pour $i \neq d$ ($§ 8$, n° 5, exemple 3). On déduit alors de la suite exacte des modules d’extensions associée à la suite ci-dessus et à $\Omega$ que l’homothétie de rapport $x$ dans le A-module $\mathrm{Ext}^i_A(A/p, \Omega)$ est surjective pour $i \neq d - 1$, ce qui implique que ce module est nul (lemme de Nakayama). En particulier $\mathrm{Ext}^d_A(A/p, \Omega)$ est nul, et l’on obtient une suite exacte

$$
0 \to \mathrm{Ext}^{d-1}_A(A/p, \Omega) \xrightarrow{x} \mathrm{Ext}^{d-1}_A(A/p, \Omega) \longrightarrow \mathrm{Ext}^d_A(A/(p + xA), \Omega) \to 0 .
$$

On a $\mathrm{long}_A(\mathrm{Ext}^i_A(A/(p + xA), \Omega)) = \mathrm{long}_A(A/(p + xA))$ (*loc. cit.*); la proposition résulte alors du lemme suivant, appliqué à l’anneau $B = A/p$ et au B-module $M = \mathrm{Ext}^{d-1}_A(A/p, \Omega)$ :

#### Lemme 1 {#ac-x-s9-lem-1 .statement}

*Soient B un anneau noethérien local, intègre, de dimension 1, et M un B-module sans torsion de type fini. On suppose qu’on a $\mathrm{long}_B(M/xM) = \mathrm{long}_B(B/xB)$ pour tout élément non nul x de B. Alors le B-module M est de rang 1.*

Soit en effet $r$ le rang de M ; il existe un sous-module L de M libre de rang $r$ tel que $M/L$ soit un module de torsion (VII, § 4, n° 1, cor. de la prop. 1), donc de longueur finie (VII, § 2, n° 5, lemme 1). L’annulateur de $M/L$ n’est pas réduit à 0, et contient donc un élément non nul $x$ de $m_B$. Considérons le diagramme commutatif

$$
\begin{array}{cccccccc}
0 & \to & L & \longrightarrow & M & \longrightarrow & M/L & \to 0 \\
& & \downarrow_{x_L} & & \downarrow_{x_M} & & \downarrow_0 & \\
0 & \to & L & \longrightarrow & M & \longrightarrow & M/L & \to 0 .
\end{array}
$$

D’après le lemme du serpent (A, X, p. 4, prop. 2), on en déduit une suite exacte

$$
0 \to M/L \longrightarrow L/xL \longrightarrow M/xM \longrightarrow M/L \to 0 ,
$$

d’où $\operatorname{long}(M/xM) = \operatorname{long}(L/xL)$. Comme $\operatorname{long}(M/xM) = \operatorname{long}(B/xB)$ par hypothèse et $\operatorname{long}(L/xL) = r \operatorname{long}(B/xB)$, on en déduit $r = 1$.

#### Corollaire 1 {#ac-x-s9-lem-1-cor-1 .statement}

*Pour toute partie multiplicative S de A, le S$^{-1}$A-module S$^{-1}\Omega$ est dualisant.*

#### Corollaire 2 {#ac-x-s9-lem-1-cor-2 .statement}

*Le support de $\Omega$ est égal à Spec(A).*

En effet un module dualisant sur un anneau local est non nul par définition.

#### Corollaire 3 {#ac-x-s9-lem-1-cor-3 .statement}

*Soit M un A-module de type fini, et soit i un entier. Le A-module $\operatorname{Ext}_A^i(M, \Omega)$ est de type fini, et son support est de codimension $\geqslant i$ dans Spec(A).*

La première assertion résulte de A, X, p. 108, cor. Soit $\mathfrak{p}$ un idéal premier du support de $\operatorname{Ext}_A^i(M, \Omega)$. On a $\operatorname{Ext}_A^i(M, \Omega)_\mathfrak{p} \neq 0$, donc $\operatorname{Ext}_{A_\mathfrak{p}}^i(M_\mathfrak{p}, \Omega_\mathfrak{p}) \neq 0$ (§ 3, n° 2, prop. 2), ce qui implique $\operatorname{di}_{A_\mathfrak{p}}(\Omega_\mathfrak{p}) \geqslant i$. Comme $\Omega_\mathfrak{p}$ est un $A_\mathfrak{p}$-module dualisant (prop. 2), on a $\operatorname{di}_{A_\mathfrak{p}}(\Omega_\mathfrak{p}) = \dim(A_\mathfrak{p})$ (prop. 1), d’où le corollaire.

#### Proposition 3 {#ac-x-s9-prop-3 .statement}

*Soient A un anneau local noethérien, $\Omega$ un A-module dualisant et M un A-module de type fini.

a) *On a $\operatorname{Ext}_A^i(M, \Omega) = 0$ pour $i < \dim(A) - \dim_A(M)$.*

b) *Posons $c = \dim(A) - \dim_A(M)$. Si M est non nul, le A-module $\operatorname{Ext}_A^c(M, \Omega)$ n’est pas nul.*

c) *On a $\operatorname{Ext}_A^i(M, \Omega) = 0$ pour $i > \dim(A) - \operatorname{prof}_A(M)$.*

Supposons M non nul et désignons par F son support. D’après la prop. 9 du § 1, n° 5, la conjonction des assertions a) et b) est équivalente à $\operatorname{prof}_F(\Omega) = c$. Or puisque $\Omega$ est macaulayen et que son support est égal à Spec(A) (prop. 1 et cor. 2 de la prop. 2), on a

$$
\operatorname{prof}_F(\Omega) = \operatorname{codim}(F, \operatorname{Spec}(A)) = c
$$

(§ 2, n° 1, cor. de la prop. 1 et n° 2, cor. de la prop. 2).

Prouvons c) par récurrence sur la profondeur de M. Si $\operatorname{prof}_A(M) = 0$, on a bien $\operatorname{Ext}_A^i(M, \Omega) = 0$ pour $i > \dim(A)$, puisque $\operatorname{di}_A(\Omega) = \dim(A)$ (prop. 1). Supposons $\operatorname{prof}_A(M) > 0$ ; il existe alors un élément $x$ de $\mathfrak{m}_A$ tel que l’homothétie de rapport $x$ soit injective dans M. On a $\operatorname{prof}_A(M/xM) = \operatorname{prof}_A(M) - 1$ (§ 1, n° 4, prop. 7).

Considérons la suite exacte des modules d’extensions

$$
\operatorname{Ext}_A^i(M, \Omega) \xrightarrow{x} \operatorname{Ext}_A^i(M, \Omega) \longrightarrow \operatorname{Ext}_A^{i+1}(M/xM, \Omega)
$$

associée à la suite exacte

$$
0 \to M \xrightarrow{x} M \longrightarrow M/xM \to 0 .
$$

Pour $i > \dim(A) - \operatorname{prof}_A(M)$, le $A$-module $\operatorname{Ext}_A^{i+1}(M/xM, \Omega)$ est nul par l’hypothèse de récurrence, donc l’homothétie de rapport $x$ est surjective dans $\operatorname{Ext}_A^i(M, \Omega)$, ce qui implique que ce $A$-module est nul (lemme de Nakayama). Cela prouve c).

#### Corollaire {#ac-x-s9-n1-cor-1 .statement}

*Si $M$ est macaulayen, on a $\operatorname{Ext}_A^i(M, \Omega) = 0$ pour $i \neq c$; le $A$-module $\operatorname{Ext}_A^c(M, \Omega)$ est macaulayen, et son support est égal à celui de $M$.*

La première assertion résulte de la prop. 3, a) et c). Soit $p \in \operatorname{Supp}(M)$; d’après la prop. 1 du § 2, n° 1, appliquée à $M$ et à $A$, on a

$$
\dim(A_p) - \dim_{A_p}(M_p) = \dim(A) - \dim_A(M) = c ;
$$

puisque le $A_p$-module $\Omega_p$ est dualisant (prop. 2), il résulte de la prop. 3, b) que le $A_p$-module $\operatorname{Ext}_A^c(M_p, \Omega_p)$ n’est pas nul. Par suite le support de $\operatorname{Ext}_A^c(M, \Omega)$ est égal à celui de $M$.

Prouvons enfin, par récurrence sur $\dim(M)$, que le $A$-module $\operatorname{Ext}_A^c(M, \Omega)$ est macaulayen. L’assertion est satisfaite lorsque $\dim(M) = 0$ puisque tout module de longueur finie est macaulayen. Supposons $\dim(M) > 0$ et choisissons un élément $x$ de $\mathfrak{m}_A$ tel que l’homothétie $x_M$ soit injective. Le $A$-module $M/xM$ est macaulayen ($§ 2$, n° 3, prop. 4), de dimension $\dim(M) - 1$. Compte tenu de ce qui précède, la suite exacte des modules d’extensions associée à la suite exacte $0 \to M \xrightarrow{x} M \longrightarrow M/xM \to 0$ se réduit à

$$
0 \to \operatorname{Ext}_A^c(M, \Omega) \xrightarrow{x} \operatorname{Ext}_A^c(M, \Omega) \longrightarrow \operatorname{Ext}_A^{c+1}(M/xM, \Omega) \to 0 ;
$$

la prop. 4 du § 2, n° 3 et l’hypothèse de récurrence entraînent alors que $\operatorname{Ext}_A^c(M, \Omega)$ est macaulayen, d’où le corollaire.

### 2. Quotient par une suite régulière

#### Proposition 4 {#ac-x-s9-prop-4 .statement}

*Soient $A$ un anneau noethérien, $J$ un idéal de $A$ engendré par une suite $A$-régulière $x$, et $\Omega$ un $A$-module de type fini.

a) Si le $A$-module $\Omega$ est dualisant, la suite $x$ est $\Omega$-régulière et le $A/J$-module $\Omega/J\Omega$ est dualisant ;

b) Si le $A/J$-module $\Omega/J\Omega$ est dualisant, que $J$ est contenu dans le radical de $A$ et que la suite $x$ est $\Omega$-régulière, le $A$-module $\Omega$ est dualisant.*

Raisonnant par récurrence sur la longueur de la suite $x$, on se ramène au cas où celle-ci est réduite à un élément $x$. Supposons que le $A$-module $\Omega$ soit dualisant. Pour tout idéal maximal $m$ de $A$ contenant $x$, on a $\dim(A_m/xA_m) = \dim(A_m) - 1$

Notons \overline{A} l’anneau A/xA ; soit m un idéal maximal de A contenant x, et soit \overline{m} son image dans \overline{A}. Le A-module A/m est annulé par x, et s’identifie à \overline{A}/\overline{m} ; on dispose donc pour tout entier i \geqslant 1 d’un isomorphisme Ext^i_A(A/m, \Omega) \longrightarrow \operatorname{Ext}^{i-1}_{\overline{A}}(\overline{A}/\overline{m}, \Omega/x\Omega) (§ 3, n° 4, prop. 7). On a

$$
\operatorname{ht}(\overline{m}) = \dim(\overline{A}_m) = \dim(A_m/xA_m) = \dim(A_m) - 1 = \operatorname{ht}(m) - 1
$$

(VIII, § 3, n° 1, cor. 2, a)). Or les idéaux maximaux de \overline{A} sont les idéaux \overline{m}, où m est un idéal maximal de A contenant x ; si de plus x appartient au radical de A, tout idéal maximal de A contient x. La proposition en résulte.

#### Corollaire 1 {#ac-x-s9-prop-4-cor-1 .statement}

**Soit A un anneau noethérien intègre. Tout A-module dualisant est sans torsion et de rang 1.**

Soit \Omega un A-module dualisant ; il est sans torsion d’après la prop. 4. Soit K le corps des fractions de A ; le K-espace vectoriel K \otimes_A \Omega est dualisant (n° 1, prop. 2), donc de dimension 1.

#### Corollaire 2 {#ac-x-s9-prop-4-cor-2 .statement}

**Soient A un anneau de Macaulay local, \Omega un A-module de type fini, et x une suite sécante maximale d’éléments de m_A, engendrant un idéal J. Les conditions suivantes sont équivalentes :**

(i) le A-module \Omega est dualisant ;
(ii) le A-module \Omega est macaulayen de dimension égale à \dim(A), et \Omega/J\Omega est un module injectif indécomposable sur l’anneau local artinien A/J ;
(iii) la suite x est \Omega-régulière et \Omega/J\Omega est un module injectif indécomposable sur l’anneau local artinien A/J ;
(iv) la suite x est \Omega-régulière, on a \operatorname{long}_A(\Omega/J\Omega) = \operatorname{long}_A(A/J) et le \kappa_A-espace vectoriel \operatorname{Hom}_A(\kappa_A, \Omega/J\Omega) est de dimension 1.

(i) \Rightarrow (ii) : si \Omega est dualisant, il est macaulayen et de dimension \dim(A) (n° 1, prop. 1). La suite x est A-régulière puisque A est un anneau de Macaulay ; d’après la prop. 4, le A/J-module \Omega/J\Omega est dualisant, donc est un A/J-module de Matlis (n° 1, exemple 1).

(ii) \Rightarrow (iii) : sous l’hypothèse (ii), on a \dim(\Omega) = \dim(A) et \dim(\Omega/J\Omega) = \dim(A/J) = 0, de sorte que la suite x est sécante pour \Omega, donc \Omega-régulière (§ 2, n° 3, th. 1).

(iii) \Rightarrow (i) : sous les hypothèses de (iii), le A/J-module \Omega/J\Omega est un A-module de Matlis, donc est dualisant (n° 1, exemple 1) ; d’après la prop. 4 le A-module \Omega est dualisant.

(iii) \Leftrightarrow (iv) : cela résulte de la remarque du § 8, n° 3.

### 3. Changement d’anneaux

#### Proposition 5 {#ac-x-s9-prop-5 .statement}

Soit $\rho : A \to B$ un homomorphisme d’anneaux noethériens, faisant de $B$ un $A$-module plat. On suppose que pour tout idéal maximal $n$ de $B$, l’anneau $\kappa(\rho^{-1}(n)) \otimes_A B$ est un anneau de Gorenstein. Soit $\Omega$ un $A$-module dualisant ; le $B$-module $\Omega_{(B)}$ est dualisant.

Soient $n$ un idéal maximal de $B$, et $p$ son image réciproque dans $A$. Le $A_p$-module $B_n$ est plat, le $A_p$-module $\Omega_p$ est dualisant, $\Omega_{(B)} \otimes_B B_n$ s’identifie à $\Omega_p \otimes_{A_p} B_n$ et $\kappa_{A_p} \otimes_{A_p} B_n$, qui s’identifie à un anneau de fractions de $\kappa(p) \otimes_A B$, est un anneau de Gorenstein. Il suffit donc de démontrer la proposition lorsque $\rho$ est un homomorphisme local d’anneaux locaux, ce que nous supposerons désormais.

Traitons d’abord le cas où les anneaux $A$ et $B$ sont artiniens. Posons $C = B/\mathfrak{m}_A B$. Puisque $B$ est plat sur $A$, le $B$-module $\mathrm{Hom}_B(C, \Omega_{(B)})$ est isomorphe à $\mathrm{Hom}_A(\kappa_A, \Omega) \otimes_A B$ (I, § 2, n° 10, prop. 11), donc à $\mathrm{Hom}_A(\kappa_A, \Omega) \otimes_{\kappa_A} C$. On en déduit une suite d’isomorphismes

$$
\mathrm{Hom}_B(\kappa_B, \Omega_{(B)}) \longrightarrow \mathrm{Hom}_C(\kappa_C, \mathrm{Hom}_B(C, \Omega_{(B)})) \longrightarrow \mathrm{Hom}_C(\kappa_C, \mathrm{Hom}_A(\kappa_A, \Omega) \otimes_{\kappa_A} C)
$$
$$
\longrightarrow \mathrm{Hom}_A(\kappa_A, \Omega) \otimes_{\kappa_A} \mathrm{Hom}_C(\kappa_C, C) .
$$

Le $\kappa_A$-espace vectoriel $\mathrm{Hom}_A(\kappa_A, \Omega)$ est de dimension 1 puisque $\Omega$ est dualisant, et il en est de même du $\kappa_C$-espace vectoriel $\mathrm{Hom}_C(\kappa_C, C)$ puisque $C$ est un anneau de Gorenstein ; par suite le $\kappa_B$-espace vectoriel $\mathrm{Hom}_B(\kappa_B, \Omega_{(B)})$ est de dimension 1.

Soit $M$ un $B$-module de longueur finie ; prouvons par récurrence sur $\mathrm{long}_B(M)$ qu’on a $\mathrm{long}_B(\mathrm{Hom}_B(M, \Omega_{(B)})) \leqslant \mathrm{long}_B(M)$. L’assertion est claire si $M = 0$, et elle résulte de ce qui précède si $M = \kappa_B$. Supposons $\mathrm{long}_B(M) \geqslant 2$. Il existe une suite exacte de $B$-modules
$$
0 \to M' \to M \to \kappa_B \to 0
$$
avec $\mathrm{long}_B(M') < \mathrm{long}_B(M)$. On en déduit une suite exacte
$$
0 \to \mathrm{Hom}_B(\kappa_B, \Omega_{(B)}) \to \mathrm{Hom}_B(M, \Omega_{(B)}) \to \mathrm{Hom}_B(M', \Omega_{(B)}) ,
$$
et l’on conclut en appliquant l’hypothèse de récurrence à $M'$.

Soit $N$ le noyau de la surjection canonique de $\kappa_A \otimes_A B$ sur $\kappa_B$. Posons $m = \mathrm{long}_B(\kappa_A \otimes_A B)$; on a $\mathrm{long}_B(N) = m - 1$. Considérons la suite exacte de $B$-modules
$$
0 \to \mathrm{Hom}_B(\kappa_B, \Omega_{(B)}) \longrightarrow \mathrm{Hom}_B(\kappa_A \otimes_A B, \Omega_{(B)}) \longrightarrow \mathrm{Hom}_B(N, \Omega_{(B)})
$$
$$
\longrightarrow \mathrm{Ext}_B^1(\kappa_B, \Omega_{(B)}) \longrightarrow \mathrm{Ext}_B^1(\kappa_A \otimes_A B, \Omega_{(B)}) .
$$

Les $B$-modules $\mathrm{Hom}_B(\kappa_A \otimes_A B, \Omega_{(B)})$ et $\mathrm{Ext}_B^1(\kappa_A \otimes_A B, \Omega_{(B)})$ sont respectivement isomorphes à $\mathrm{Hom}_A(\kappa_A, \Omega) \otimes_A B$ et $\mathrm{Ext}_A^1(\kappa_A, \Omega) \otimes_A B$, c’est-à-dire à $\kappa_A \otimes_A B$ et à 0. Les longueurs des $B$-modules $\mathrm{Hom}_B(\kappa_B, \Omega_{(B)})$ et $\mathrm{Hom}_B(\kappa_A \otimes_A B, \Omega_{(B)})$ sont 1 et $m$, et celle de $\mathrm{Hom}_B(N, \Omega_{(B)})$) est $\leqslant m - 1$; on en déduit que le $B$-module $\mathrm{Ext}_B^1(\kappa_B, \Omega_{(B)})$ est nul. D’après la prop. 6 du § 3, n° 3, le $B$-module $\Omega_{(B)}$ est injectif ; par suite c’est un module dualisant (n° 1, exemple 1).

Passons au cas général. Posons $C = \kappa_A \otimes_A B$; c’est par hypothèse un anneau de Gorenstein, donc un anneau de Macaulay ($§ 3, n° 7$, prop. 10). D’après la prop. 1 du n° 1, $A$ est un anneau de Macaulay, et le $A$-module $\Omega$ est macaulayen. Par suite $B$ est un anneau de Macaulay, et le $B$-module $\Omega_{(B)}$ est macaulayen ($§ 2, n° 7$, cor. 1 de la prop. 9). Posons $r = \dim(A)$, $s = \dim(C)$. Il existe une suite $(x_1, \ldots, x_r)$ d’éléments de $\mathfrak{m}_A$ régulière pour les $A$-modules $A$ et $\Omega$, et une suite $(y_1, \ldots, y_s)$ d’éléments de $\mathfrak{m}_B$ régulière pour le $B$-module $C$; notons $x$ l’idéal de $A$ et $\mathfrak{g}$ l’idéal de $B$ qu’elles engendrent respectivement. La suite $(y_1, \ldots, y_s, \rho(x_1), \ldots, \rho(x_r))$ est régulière pour les $B$-modules $B$ et $\Omega_{(B)}$ ($§ 1, n° 6$, prop. 11), et le $A$-module $B/\mathfrak{g}$ est plat (*loc. cit.*, prop. 10). Posons $A' = A/x$, $B' = B/(xB + \mathfrak{g})$ et notons $\rho' : A' \to B'$ l’homomorphisme déduit de $\rho$ par passage aux quotients. Les anneaux $A'$ et $B'$ sont artiniens, le $A'$-module $B'$ est plat, l’anneau $\kappa_{A'} \otimes_{A'} B'$, qui s’identifie à $C/\mathfrak{g}$, est un anneau de Gorenstein ($§ 3, n° 7$, exemple 2) et le $A'$-module $\Omega_{(A')}$ est dualisant (n° 2, prop. 4). D’après la première partie de la démonstration, le $B'$-module $\Omega_{(B')}$ est dualisant. Il résulte alors de *loc. cit.* que le $B$-module $\Omega_{(B)}$ est dualisant.

#### Corollaire {#ac-x-s9-n3-cor-1 .statement}

*Soit A un anneau noethérien, admettant un module dualisant $\Omega$; soit B une algèbre de polynômes sur A en un nombre fini d’indéterminées. Le B-module $\Omega_{(B)}$ est dualisant.*

En effet, pour tout idéal premier $\mathfrak{p}$ de $A$, l’anneau $\kappa(\mathfrak{p}) \otimes_A A[X]$ s’identifie à $\kappa(\mathfrak{p})[X]$, qui est régulier, donc de Gorenstein.

#### Proposition 6 {#ac-x-s9-prop-6 .statement}

*Soient $\Lambda$ un anneau local noethérien et $\Omega$ un $A$-module dualisant. Soit B une A-algèbre finie ; on suppose que le A-module B est macaulayen. Le B-module $\mathrm{Ext}_A^i(B, \Omega)$ est nul pour $i \neq \dim(A) - \dim(B)$ et dualisant pour $i = \dim(A) - \dim(B)$.

On a $\dim(B) = \dim_A(B) \leq \dim(\Lambda)$ (VIII, § 2, n° 3, th. 1 c)); posons $c = \dim(A) - \dim(B)$. On a $\mathrm{Ext}_A^i(B, \Omega) = 0$ pour $i \neq c$ puisque le $A$-module $B$ est macaulayen (n° 1, cor. de la prop. 3). Prouvons que le B-module $\mathrm{Ext}_A^c(B, \Omega)$ est dualisant.

Supposons d’abord $\dim(B) = 0$. Le spectre $X$ de $B$ est fini et formé d’idéaux maximaux (IV, § 2, n° 5, prop. 9); l’application canonique $B \to \prod_{n \in X} B_n$ est un isomorphisme (*loc. cit.*, cor. 1). Le B-module $\Omega' = \mathrm{Ext}_A^c(B, \Omega)$ est donc somme directe des modules $\mathrm{Ext}_A^c(B_n, \Omega)$; comme $\mathrm{Ext}_A^c(B_n, \Omega)$ est à support dans $\{n\}$, il s’identifie à $\Omega'_n$. On a $\dim(B_n) = 0$ pour tout $n$; pour prouver que le B-module $\Omega'$ est dualisant, il suffit donc de prouver qu’il en est ainsi du $B_n$-module $\mathrm{Ext}_A^c(B_n, \Omega)$ pour tout $n \in X$, ce qui nous ramène au cas où l’anneau $B$ est *local*. Dans ce cas, d’après l’exemple 6 du § 8, n° 5, le B-module $\mathrm{Ext}_A^c(B, \Omega)$ est isomorphe à $\mathrm{Hom}_A(B, I)$, où $I$ est un $A$-module de Matlis; c’est par conséquent un B-module de Matlis ($§ 8, n° 6$, cor. de la prop. 5), donc un B-module dualisant (n° 1, exemple 1).

Supposons maintenant $\dim(B) > 0$ et raisonnons par récurrence sur $\dim(B)$. On a $\mathrm{prof}_A(B) = \dim_A(B) = \dim(B)$, d’où $\mathrm{prof}_A(B) > 0$; d’autre part on a $\mathrm{prof}(A) = \dim(A) > 0$ (n° 1, prop. 1), et par suite $\mathrm{prof}_A(A \oplus B) > 0$. Il existe donc un élément $x$ de $\mathfrak{m}_A$ tel que les homothéties $x_A$ et $x_B$ soient injectives.

Considérons la suite exacte des modules d’extensions associée à la suite exacte $0 \to B \xrightarrow{x_B} B \longrightarrow B/xB \to 0$ et au A-module $\Omega$. Le A-module $B/xB$ est macaulayen ($§ 2$, n° 1, exemple 3), de dimension $\dim(B) - 1$ (VIII, $§ 3$, n° 2, prop. 3) ; on a donc $\mathrm{Ext}_A^i(B/xB, \Omega) = 0$ pour $i \neq c + 1$ (n° 1, cor. de la prop. 3). Comme on a $\mathrm{Ext}_A^i(B, \Omega) = 0$ pour $i \neq c$, on obtient une suite exacte de B-modules

$$
0 \to \mathrm{Ext}_A^c(B, \Omega) \xrightarrow{x} \mathrm{Ext}_A^c(B, \Omega) \longrightarrow \mathrm{Ext}_A^{c+1}(B/xB, \Omega) \to 0 .
$$

Par l’hypothèse de récurrence, le $B/xB$-module $\mathrm{Ext}_A^{c+1}(B/xB, \Omega)$ est dualisant. Comme la A-algèbre B est finie, l’image de $m_A$ dans B est contenue dans le radical de B (V, $§ 2$, n° 1, prop. 1) ; d’après la prop. 4 du n° 2, le B-module $\mathrm{Ext}_A^c(B, \Omega)$ est dualisant.

#### Corollaire 1 {#ac-x-s9-prop-6-cor-1 .statement}

*Soient A un anneau noethérien, $\Omega$ un A-module dualisant, et B une A-algèbre finie ; on suppose que le A-module B est macaulayen. Le B-module $\mathrm{Ext}_A(B, \Omega)$ est dualisant.*

Notons $\Omega'$ le B-module $\mathrm{Ext}_A(B, \Omega)$. Soit $n$ un idéal maximal de B ; son image réciproque dans A est un idéal maximal $m$ (V, $§ 2$, n° 1, prop. 1). La $A_m$-algèbre $B_m = A_m \otimes_A B$ est finie, et c’est un $A_m$-module macaulayen ; d’après la proposition, le $B_m$-module $\Omega'_m$, qui s’identifie à $\mathrm{Ext}_{A_m}(B_m, \Omega_m)$ ($§ 3$, n° 2, prop. 2) est dualisant. Comme $B_n$ est un anneau de fractions de $B_m$, le $B_n$-module $\Omega'_n$ est dualisant, d’où le corollaire.

#### Remarque {#ac-x-s9-n3-rem-1 .statement}

Gardons les hypothèses du cor. 1 et supposons en outre que l’homomorphisme canonique $\rho : A \to B$ soit injectif. On a alors $\dim(A_m) = \dim(B_m)$ pour tout idéal maximal $m$ de A (VIII, $§ 2$, n° 3, th. 1 a)). D’après la prop. 6 et le cor. 1, $\mathrm{Ext}_A^i(B, \Omega)$ est nul pour $i \neq 0$, et le B-module $\mathrm{Hom}_A(B, \Omega)$ est dualisant.

#### Corollaire 2 {#ac-x-s9-prop-6-cor-2 .statement}

*Si un anneau noethérien A possède un module dualisant, toute A-algèbre de type fini qui est un anneau de Macaulay possède un module dualisant.*

Cela résulte du cor. 1 et du cor. de la prop. 5.

#### Corollaire 3 {#ac-x-s9-prop-6-cor-3 .statement}

*Tout anneau de Macaulay présentable (en particulier, tout anneau de Macaulay local complet) possède un module dualisant.*

Soient en effet R un anneau régulier et A un anneau de Macaulay quotient de R. Le R-module A est macaulayen ($§ 2$, n° 5, exemple 5), et R possède un module dualisant (n° 1, exemple 2) ; il en est donc de même de A d’après le cor. 1. Par ailleurs on a déjà observé qu’un anneau noethérien local complet est présentable ($§ 4$, n° 4, prop. 6, c)).

Plus généralement, tout anneau de Macaulay quotient d’un anneau de Gorenstein possède un module dualisant. Inversement, on peut montrer qu’un anneau de Macaulay local qui possède un module dualisant est quotient d’un anneau local de Gorenstein (exerc. 1).

### 4. Structure des modules dualisants

#### Lemme 2 {#ac-x-s9-lem-2 .statement}

Soient $A$ un anneau noethérien, $M$ et $N$ des $A$-modules de type fini, $u : M \to N$ un homomorphisme. Soit $x$ un élément du radical de $A$, tel que l’homothétie $x_N$ soit injective. Si l’homomorphisme $\overline{u} : M/xM \to N/xN$ induit par $u$ est injectif (resp. surjectif, resp. bijectif), il en est de même de $u$.

L’assertion concernant la surjectivité de $u$ résulte du lemme de Nakayama (II, § 3, n° 2, cor. 1 de la prop. 4), sans hypothèse sur $x_N$. Considérons le diagramme commutatif à lignes exactes

$$
\begin{array}{ccccccc}
M & \xrightarrow{x_M} & M & \longrightarrow & M/xM \\
\downarrow u & & \downarrow u & & \downarrow \overline{u} \\
0 & \longrightarrow & N & \xrightarrow{x_N} & N & \longrightarrow & N/xN ;
\end{array}
$$

à l’aide du lemme du serpent (I, § 1, n° 4, prop. 2), on en déduit une suite exacte $\mathrm{Ker}\, u \xrightarrow{x} \mathrm{Ker}\, u \longrightarrow \mathrm{Ker}\, \overline{u}$. Si $\overline{u}$ est injective, l’homothétie de rapport $x$ est surjective dans $\mathrm{Ker}\, u$, ce qui implique $\mathrm{Ker}\, u = 0$ par le lemme de Nakayama.

#### Proposition 7 {#ac-x-s9-prop-7 .statement}

Soient $A$ un anneau noethérien et $\Omega$ un $A$-module dualisant.

a) On a $\mathrm{Ext}_A^i(\Omega, \Omega) = 0$ pour $i > 0$.

b) L’homomorphisme canonique $\gamma : A \to \mathrm{End}_A(\Omega)$ est bijectif.

c) Tout $A$-module dualisant est de la forme $\Omega \otimes_A L$ où $L$ est un $A$-module projectif de rang 1.

A) Traitons d’abord le cas où l’anneau $A$ est local. Dans ce cas la condition c) signifie simplement que deux modules dualisants sont isomorphes.

Soit $\Omega'$ un $A$-module dualisant. On a $\mathrm{prof}_A(\Omega') = \dim_A(\Omega') = \dim(A)$ (n° 1, prop. 1), donc $\mathrm{Ext}_A^i(\Omega', \Omega) = 0$ pour $i \neq 0$ (n° 1, prop. 3, c)), d’où a).

Prouvons b) et c) par récurrence sur l’entier $\dim(A)$ (égal à $\mathrm{prof}(A)$). S’il est nul, l’anneau $A$ est artinien, $\Omega'$ et $\Omega$ sont des $A$-modules de Matlis (n° 1, exemple 1) ; ils sont donc isomorphes ($\S$ 8, n° 1, prop. 1) et l’application canonique $A \to \mathrm{End}_A(\Omega)$ est bijective ($\S$ 8, n° 2, prop. 3, c)). Supposons $\dim(A) > 0$ et soit $x$ un élément simplifiable de $\mathfrak{m}_A$. L’homothétie $x_\Omega$ est injective (n° 2, prop. 4), et l’on a une suite exacte

$$
0 \to \Omega \xrightarrow{x_\Omega} \Omega \longrightarrow \Omega/x\Omega \to 0 .
$$

Puisque $\mathrm{Ext}_A^1(\Omega', \Omega)$ est nul et que $\mathrm{Hom}_A(\Omega', \Omega/x\Omega)$ s’identifie à $\mathrm{Hom}_{A/xA}(\Omega'/x\Omega', \Omega/x\Omega)$, on en déduit une suite exacte

$$
(1)\quad 0 \to \mathrm{Hom}_A(\Omega', \Omega) \xrightarrow{x} \mathrm{Hom}_A(\Omega', \Omega) \xrightarrow{p} \mathrm{Hom}_{A/xA}(\Omega'/x\Omega', \Omega/x\Omega) \to 0 ,
$$

où $p$ est l’application canonique. D’après la prop. 4, les $A/xA$-modules $\Omega/x\Omega$ et $\Omega'/x\Omega'$ sont dualisants, donc isomorphes par l’hypothèse de récurrence. Soit $\overline{u}$ un isomorphisme de $\Omega'/x\Omega'$ sur $\Omega/x\Omega$. Compte tenu de la suite exacte (1), il existe un $A$-homomorphisme $u : \Omega' \to \Omega$ tel que $p(u) = \overline{u}$; d’après le lemme 2, $u$ est bijectif, ce qui prouve c). Par l’hypothèse de récurrence, l’homomorphisme canonique $A/xA \longrightarrow \mathrm{End}_{A/xA}(\Omega/x\Omega)$ est bijectif. Compte tenu de la suite exacte (1), cet homomorphisme s’identifie à l’homomorphisme $\overline{\gamma} : A/xA \longrightarrow \mathrm{End}_A(\Omega)/x\mathrm{End}_A(\Omega)$ induit par $\gamma$; il résulte alors du lemme 2 que $\gamma$ est bijectif, d’où b).

B) Passons au cas général. Pour tout idéal maximal $m$ de $A$ et tout entier $i > 0$, on a $\mathrm{Ext}^i_{A_m}(\Omega_m, \Omega_m) = 0$ d’après ce qui précède, donc $\mathrm{Ext}^i_A(\Omega, \Omega)_m = 0$ ($§ 3$, n° 2, prop. 2), ce qui implique $\mathrm{Ext}^i_A(\Omega, \Omega) = 0$ (II, $§ 3$, n° 3, cor. 2 du th. 1). De même, l’homomorphisme $\gamma_m : A_m \to \mathrm{End}_A(\Omega)_m$ est bijectif pour tout idéal maximal $m$ de $A$, donc $\gamma$ est bijectif (*loc. cit.*, th. 1).

Prouvons enfin c). Soit $\Omega'$ un $A$-module dualisant. Désignons par $L$ le $A$-module $\mathrm{Hom}_A(\Omega', \Omega)$, et par $v : \Omega' \otimes_A L \to \Omega$ l’homomorphisme tel que $v(x \otimes f) = f(x)$ pour $x \in \Omega'$, $f \in L$. Soit $m$ un idéal maximal de $A$. Le $A_m$-module $L_m$ s’identifie à $\mathrm{Hom}_{A_m}(\Omega'_m, \Omega_m)$; d’après le cas déjà traité il est libre de rang un, et tout isomorphisme $h : \Omega'_m \to \Omega_m$ en est un générateur. Lorsqu’on identifie $L_m$ à $A_m$ à l’aide du générateur $h$, l’homomorphisme $v_m : \Omega'_m \otimes_{A_m} L_m \to \Omega_m$ s’identifie à $h$, donc est bijectif. Ceci ayant lieu pour tout idéal maximal $m$ de $A$, le $A$-module $L$ est projectif de rang un (II, $§ 5$, n° 3, th. 2), et l’homomorphisme $v$ est bijectif (II, $§ 3$, n° 3, th. 1).

#### Corollaire 1 {#ac-x-s9-prop-7-cor-1 .statement}

*Pour que $A$ soit un anneau de Gorenstein, il faut et il suffit que le $A$-module $\Omega$ soit projectif de rang 1*.

Cela résulte de l’exemple 2 du n° 1 et de la prop. 7 c).

#### Corollaire 2 {#ac-x-s9-prop-7-cor-2 .statement}

*Supposons que l’anneau $A$ soit présentable. L’ensemble des idéaux premiers $p$ de $A$ tels que $A_p$ soit un anneau de Gorenstein est ouvert dans $\mathrm{Spec}(A)$*.

Soit $p$ un idéal premier de $A$ tel que $A_p$ soit un anneau de Gorenstein. C’est alors un anneau de Macaulay ; quitte à remplacer $A$ par $A_f$, où $f$ est un élément convenable de $A - p$, on se ramène au cas où $A$ est un anneau de Macaulay ($§ 4$, n° 4, prop. 7, c)). Soit $\Omega$ un $A$-module dualisant (n° 3, cor. 3 de la prop. 6). Alors $\Omega_p$ est un module dualisant sur l’anneau de Gorenstein $A_p$ (n° 1, prop. 2), donc est libre de rang 1 (cor. 1). Par suite il existe un élément $g$ de $A - p$ tel que le $A_g$-module $\Omega_g$ soit libre de rang 1 (II, $§ 5$, n° 1, cor. de la prop. 2). Ainsi $A_g$ est un anneau de Gorenstein (cor. 1) et il en est de même de $A_q$ pour tout idéal premier $q$ de $A$ ne contenant pas $g$ ($§ 3$, n° 7, exemple 1), ce qui prouve le corollaire.

### 5. Dualité des modules de type fini

On considère dans ce numéro un anneau noethérien $A$ *de dimension finie* qui possède un module dualisant $\Omega$. On a alors $\mathrm{di}_A(\Omega) = \dim(A) < +\infty$ (n° 1, prop. 1). *Choisissons une résolution injective de longueur finie* $e : \Omega \to (I, \delta)$. Pour tout complexe $C$ de $A$-modules, notons $D(C)$ le complexe $\mathrm{Homgr}_A(C, I)$. Cela s’applique en particulier à tout $A$-module $M$, considéré comme un complexe concentré en degré 0 ; on a alors $D(M)^i = \mathrm{Hom}_A(M, I^i)$ pour tout entier $i$. Rappelons qu’on a construit en A, X, p. 100, th. 1, un isomorphisme canonique

$$
\varphi(M, I) : H(D(M)) \longrightarrow \mathrm{Ext}_A(M, \Omega)
$$

*Exemples.—* 1) Le complexe $D(A) = \mathrm{Homgr}_A(A, 1)$ s’identifie à $I$. L’application $e : \Omega \to D(A)$ est par définition un homologisme.

2) L’homomorphisme $e \in \mathrm{Homgr}_A(\Omega, I)^0$ est un élément de $D(\Omega)^0$; l’application A-linéaire $\tilde{e} : A \to D(\Omega)$ telle que $\tilde{e}(1) = e$ est un homologisme (n° 4, prop. 7, a) et b)).

3) Soit S une partie multiplicative de A. Le $S^{-1}A$-module $S^{-1}\Omega$ est dualisant (n° 1, cor. 1 de la prop. 2); les $S^{-1}A$-modules $S^{-1}I^i$ sont injectifs (cor. 1 de la prop. 3 du § 3, n° 2) et le morphisme $e' : S^{-1}\Omega \to S^{-1}I$ déduit de $e$ est une résolution injective de $S^{-1}\Omega$, à laquelle on peut donc appliquer ce qui précède. Pour tout complexe C de type fini (et en particulier tout A-module M de type fini), l’homomorphisme canonique de $S^{-1}D(C)$ dans $\mathrm{Homgr}_{S^{-1}A}(S^{-1}C, S^{-1}I) = D(S^{-1}C)$ est bijectif.

4) Soient A un anneau de Dedekind, K son corps des fractions. Le A-module A est dualisant et admet la résolution injective I de longueur 1 définie par la suite exacte

$$
0 \to A \xrightarrow{e} K \xrightarrow{\delta} K/A \to 0
$$

où $\delta$ est la surjection canonique. Pour tout A-module M, le complexe $D(M)$ est le complexe concentré en degrés 0 et 1

$$
\ldots \longrightarrow 0 \longrightarrow \mathrm{Hom}_A(M, K) \xrightarrow{d} \mathrm{Hom}_A(M, K/A) \longrightarrow 0 \longrightarrow \ldots
$$

avec $d = \mathrm{Hom}_A(1_M, \delta)$. On a une suite exacte

$$
0 \to \mathrm{Hom}_A(M, A) \longrightarrow D(M)^0 \xrightarrow{d} D(M)^1 \longrightarrow \mathrm{Ext}_A^1(M, A) \to 0 .
$$

Pour tout morphisme de complexes $f : C \to C'$, on note $D(f) : D(C') \to D(C)$ le morphisme de complexes $\mathrm{Homgr}_A(f, 1_I)$. Si $f$ est un homologisme, $D(f)$ est un homologisme (A, X, p. 86, prop. 4, b)). Si $C' \xrightarrow{f} C \xrightarrow{g} C''$ est une suite exacte de complexes, la suite de complexes $D(C'') \xrightarrow{D(g)} D(C) \xrightarrow{D(f)} D(C')$ est exacte (A, X, p. 83, prop. 2, a)).

Soit M un A-module. À chaque élément $m$ de M, associons l’application $\alpha_M(m) : f \mapsto f(m)$ de $D(M)$ dans I ; c’est un élément de $D(D(M))_0 = \mathrm{Homgr}_A(D(M), I)_0$. Il résulte des définitions que $\alpha_M(m)$ est un morphisme de complexes, donc un élément de $Z_0(D(D(M)))$.

On définit ainsi un morphisme de complexes :

$$
\alpha_M : M \to D(D(M)),
$$

d’où, par passage à l’homologie, un homomorphisme de A-modules

$$
\alpha_M : M \to H_0(D(D(M))).
$$

#### Théorème 1 {#ac-x-s9-thm-1 .statement}

**Soit $M$ un $A$-module de type fini. Alors $\alpha_M$ est un homologisme : on a $H_i(D(D(M))) = 0$ pour $i \neq 0$ et l’homomorphisme $\alpha_M$ est bijectif.**

Prenons d’abord $M = A$. L’application $e : \Omega \to D(A)$ est un homologisme (exemple 1), donc aussi l’application $D(e) : D(D(A)) \to D(\Omega)$. L’application $\tilde{e} : A \to D(\Omega)$ est un homologisme (exemple 2), et on a $D(e) \circ \alpha_A = \tilde{e}$; ainsi $\alpha_A$ est un homologisme, ce qui prouve le théorème dans ce cas. Il en résulte que $\alpha_M$ est un homologisme lorsque le $A$-module $M$ est libre de type fini.

Passons au cas général ; nous allons prouver par récurrence sur l’entier $n$ l’assertion suivante :

$(A_n)$ *pour tout $A$-module de type fini $M$, l’homomorphisme $H_i(\alpha_M)$ est bijectif pour $i \leq n$.*

Cela signifie aussi que $H_i(D(D(M)))$ est nul pour $i \neq 0$ et $i \leq n$, et que $\alpha_M$ est bijectif si $n \geq 0$. Observons que $(A_n)$ est vérifiée pour $n < -d$, où $d$ est la longueur du complexe $I$ : en effet le $A$-module $D(D(M))_i$ est égal à $\bigoplus_p \mathrm{Hom}_A(\mathrm{Hom}_A(M, I^p), I^{p-i})$, donc est nul pour $i < -d$ et $i > d$.

Prouvons l’implication $(A_n) \Rightarrow (A_{n+1})$. Soit $M$ un $A$-module de type fini. Il existe un $A$-module libre de type fini $L$ et une suite exacte $0 \to N \xrightarrow{u} L \xrightarrow{v} M \to 0$.

La suite $0 \to D(M) \xrightarrow{D(v)} D(L) \xrightarrow{D(u)} D(N) \to 0$ est exacte ; de même, si l’on pose $u' = D(D(u))$ et $v' = D(D(v))$, la suite $0 \to D(D(N)) \xrightarrow{u'} D(D(L)) \xrightarrow{v'} D(D(M)) \to 0$ est exacte.

Puisque $H_i(D(D(L)))$ est nul pour $i \neq 0$, on a des isomorphismes

$$
H_i(D(D(M)))) \longrightarrow H_{i-1}(D(D(N))) \quad \text{pour } i \neq 0, 1 ;
$$

cela entraîne l’implication $(A_n) \Rightarrow (A_{n+1})$ pour $n \neq -1$ et $n \neq 0$. Considérons le diagramme commutatif à lignes exactes

$$
\begin{array}{ccccccccc}
0 & \to & N & \xrightarrow{u} & L & \xrightarrow{v} & M & \to & 0 \\
& & \downarrow{\alpha_N} & & \downarrow{\alpha_L} & & \downarrow{\alpha_M} & & \\
0 & \to & H_1(D(D(M))) & \longrightarrow & H_0(D(D(N))) & \xrightarrow{H_0(u')} & H_0(D(D(L))) & \xrightarrow{H_0(v')} & H_0(D(D(M))) \longrightarrow H_{-1}(D(D(N)))
\end{array}
$$

où $\alpha_L$ est bijectif. Si $(A_0)$ est satisfaite, l’homomorphisme $\alpha_N$ est également bijectif, donc $H_0(u')$ est injectif et l’on obtient $H_1(D(D(M))) = 0$, d’où $(A_1)$. Si $(A_{-1})$

Ainsi $(A_n)$ est vraie pour tout $n$, ce qui démontre le théorème.

Soit $M$ un $A$-module de type fini ; posons $c = \dim(A) - \dim_A(M)$. Notons $D'(M)$ le sous-complexe de $D(M)$ égal à $\bigoplus_{i < c} D(M)^i \bigoplus Z^c(D(M))$, et

$$
j : D'(M) \to D(M)
$$

l’injection canonique. On déduit de la surjection canonique $Z^c(D(M)) \to H^c(D(M))$ et de l’isomorphisme $\varphi(M, I)$ un morphisme de complexes

$$
p : D'(M)(-c) \to \mathrm{Ext}_A^c(M, \Omega)
$$

comme $H^i(D(M))$ est nul pour $i < c$ (n° 1, prop. 3 a)), $(D'(M)(-c), p)$ est une résolution gauche de $\mathrm{Ext}_A^c(M, \Omega)$. D’après A, X, p. 100, th. 1, on a un isomorphisme canonique

$$
\varphi^0(D'(M)(-c), I) : H_0(D(D'(M))) \to \mathrm{Ext}_A^c(\mathrm{Ext}_A^c(M, \Omega), \Omega)
$$

en le composant avec l’homomorphisme $H_0(D(j)) : H_0(D(D(M))) \to H_0(D(D'(M)))$

on obtient donc un homomorphisme

$$
H_0(D(D(M))) \to \mathrm{Ext}_A^c(\mathrm{Ext}_A^c(M, \Omega), \Omega),
$$

d’où finalement, par composition avec $\alpha_M$, un homomorphisme canonique

$$
\beta_M : M \to \mathrm{Ext}_A^c(\mathrm{Ext}_A^c(M, \Omega), \Omega).
$$

#### Corollaire {#ac-x-s9-n5-cor-1 .statement}

Si le $A$-module $M$ est macaulayen, l’homomorphisme $\beta_M$ est bijectif.

Si $M$ est macaulayen, le $A$-module $H^i(D(M))$ est nul pour $i \neq c$ (n° 1, cor. de la prop. 3), de sorte que l’injection canonique $j : D'(M) \to D(M)$ est un homologisme ; par suite le morphisme de complexes $D(j) : D(D(M)) \to D(D'(M))$ est un homologisme (A, X, p. 86, prop. 4). Ainsi $H_0(D(j))$ est bijectif ; d’autre part $\alpha_M$ est bijectif par le th. 1, d’où le corollaire.

Lorsque le $A$-module $M$ est de longueur finie, le $A$-module $\mathrm{Ext}_A^c(M, \Omega)$ s’identifie au dual de Matlis de $M$ ($cf.$ § 8, n° 5, exemple 3 et th. 3), et l’on retrouve la prop. 4 du § 8, n° 4.

### 6. Exemple : le cas de la dimension 1

Dans ce numéro, on considère un anneau $A$ intègre, noethérien, de dimension 1, admettant un module dualisant $\Omega$. On note $K$ le corps des fractions de $A$, et $V$ le $K$-espace vectoriel $K \otimes_A \Omega$.

L’homomorphisme canonique $\Omega \to V$ est injectif, et le K-espace vectoriel V est de dimension 1 (n° 2, cor. 1 de la prop. 4) ; identifions $\Omega$ à un sous-A-module de V.

#### Proposition 8 {#ac-x-s9-prop-8 .statement}

*Le A-module $V/\Omega$ est un module de Matlis.*

Considérons la suite exacte

$$
0 \to \Omega \to V \to V/\Omega \to 0 ;
$$

le A-module V est injectif (A, X, p. 18, exemple 1), et l’on a $\mathrm{di}_A(\Omega) = 1$ (n° 1, prop. 1). On en déduit d’une part que $V/\Omega$ est injectif (§ 3, n° 1, prop. 1), d’autre part, que pour tout idéal maximal $m$ de A, le $A/m$-espace vectoriel $\mathrm{Hom}_A(A/m, V/\Omega)$ est isomorphe à $\mathrm{Ext}_A^1(A/m, \Omega)$, donc de dimension 1. Comme $V/\Omega$ est un module de torsion, ses idéaux premiers associés sont maximaux ; cela démontre la proposition (§ 8, n° 4).

Soit M un A-module ; conformément à *loc. cit.*, nous noterons D(M) le A-module $\mathrm{Hom}_A(M, V/\Omega)$. On peut appliquer les constructions du n° 5 en prenant pour I le complexe

$$
\cdots 0 \to V \xrightarrow{p} V/\Omega \to 0 \cdots
$$

où V est placé en degré 0, et p désigne la surjection canonique. Le complexe $\mathbf{D}(M)$ est

$$
\cdots 0 \to \mathrm{Hom}_A(M, V) \xrightarrow{p_M} \mathbf{D}(M) \to 0 \cdots ,
$$

avec $p_M = \mathrm{Hom}(1_M, p)$. On a un isomorphisme canonique de A-modules gradués $\varphi(M, I) : \mathrm{H}(\mathbf{D}(M)) \to \mathrm{Ext}_A(M, \Omega)$ (A, X, p. 100, th. 1).

Lorsque M est un module de torsion, le module $\mathbf{D}(M)^0 = \mathrm{Hom}_A(M, V)$ est nul, et $\varphi(M, I)$ est un isomorphisme de $\mathbf{D}(M)$ sur $\mathrm{Ext}_A^1(M, \Omega)$ ; le morphisme $\alpha_M : M \to \mathbf{D}(\mathbf{D}(M))$ n’est autre que l’homomorphisme canonique de A-modules

$$
\alpha_M : M \to \mathbf{D}(\mathbf{D}(M))
$$

défini au § 8, n° 3, qui est un isomorphisme lorsque M est de type fini (c’est-à-dire de longueur finie). On retrouve dans ce cas la situation de *loc. cit*.

Revenons au cas général, et supposons le A-module M de type fini. Alors $\mathbf{D}(M)$ est un module de torsion, donc le A-module $\mathbf{D}(\mathbf{D}(M))^{-1} = \mathrm{Hom}_A(\mathbf{D}(M), V)$ est nul. D’autre part le A-module $\mathrm{Hom}_A(\mathbf{D}(M)^0, V) = \mathrm{Hom}_A(\mathrm{Hom}_A(M, V), V)$ s’identifie naturellement à $K \otimes_A M$, de façon que l’homomorphisme

$$
\mathrm{Hom}(1, p) : \mathrm{Hom}_A(\mathrm{Hom}_A(M, V), V) \to \mathbf{D}(\mathrm{Hom}_A(M, V))
$$

s’identifie à l’application

$$
j : K \otimes_A M \to \mathbf{D}(\mathrm{Hom}_A(M, V))
$$

telle que $j(\lambda \otimes m)(f) = p(\lambda f(m))$ pour $\lambda \in K,\ m \in M,\ f \in \mathrm{Hom}_A(M, V)$. Le th. 1 du n° 5 se traduit donc par l’exactitude de la suite

$$
0 \longrightarrow M \xrightarrow{(i, \alpha_M)} (K \otimes_A M) \oplus D(D(M)) \xrightarrow{(j, -D(p_M))} D(\mathrm{Hom}_A(M, V)) \longrightarrow 0,
$$

où $i$ désigne l’application canonique de $M$ dans $K \otimes_A M$. Le noyau de $i$ s’identifie au sous-module de torsion $T(M)$ de $M$, et son conoyau à $(K/A) \otimes_A M$. Considérons le diagramme commutatif à lignes exactes

$$
\begin{array}{ccccccccc}
0 & \to & T(M) & \longrightarrow & M & \xrightarrow{i} & K \otimes_A M & \longrightarrow & (K/A) \otimes_A M \longrightarrow 0 \\
& & \downarrow{\alpha_M} & & & & \downarrow{j} & & \\
0 & \to & D(\mathrm{Ext}_A^1(M, \Omega)) & \longrightarrow & D(D(M)) & \xrightarrow{D(p_M)} & D(\mathrm{Hom}_A(M, V)) & \longrightarrow & D(\mathrm{Hom}_A(M, \Omega)) \longrightarrow 0
\end{array}
$$

où la seconde ligne est obtenue par dualité de Matlis à partir de la suite exacte

$$
0 \to \mathrm{Hom}_A(M, \Omega) \longrightarrow \mathrm{Hom}_A(M, V) \xrightarrow{p_M} \mathrm{Hom}_A(M, V/\Omega) \longrightarrow \mathrm{Ext}_A^1(M, \Omega) \to 0.
$$

Le th. 1 signifie alors que les homomorphismes de $A$-modules

$$
\gamma^0(M) : T(M) \longrightarrow D(\mathrm{Ext}_A^1(M, \Omega)) \quad \text{et} \quad \gamma^1(M) : (K/A) \otimes_A M \longrightarrow D(\mathrm{Hom}_A(M, \Omega))
$$

déduits de $\alpha_M$ et $j$ respectivement, sont bijectifs. Comme le $A$-module $T(M)$ est de longueur finie, le $A$-module $\mathrm{Ext}_A^1(M, \Omega)$ est de longueur finie et s’identifie au dual de Matlis $D(T(M))$, et l’on a $[\mathrm{Ext}_A^1(M, \Omega)] = [T(M)]$ dans le groupe $Z_0(A)$ et $\mathrm{long}_A(\mathrm{Ext}_A^1(M, \Omega)) = \mathrm{long}_A(T(M))$ (§ 8, n° 4, prop. 4). D’autre part, lorsqu’on prend $M = A$, on obtient un isomorphisme canonique $\gamma^1(A) : K/A \to D(\Omega)$.

Soit $B$ un sous-anneau de $K$ contenant $A$, fini sur $A$. Pour tout idéal maximal $m$ de $A$, on a $\mathrm{prof}_{A_m}(B_m) = \dim_{A_m}(B_m) = 1$ (§ 1, n° 1, remarque 2 et VIII, § 2, n° 3, th. 1), de sorte que $B$ est un $A$-module macaulayen. Par conséquent le $B$-module $\Omega_B = \mathrm{Hom}_A(B, \Omega)$ est dualisant (n° 3, remarque). L’application canonique de $\Omega_B = \mathrm{Hom}_A(B, \Omega)$ dans $\Omega = \mathrm{Hom}_A(A, \Omega)$ est injective ; son image est formée des éléments $\omega$ de $\Omega$ tels que le sous-B-module $B\omega$ de $V$ soit contenu dans $\Omega$. Ainsi $\Omega_B$ s’identifie au plus grand sous-B-module de $\Omega$. Le $A$-module $B/A$ est de longueur finie ; la suite exacte

$$
0 \to \Omega_B \to \Omega \to \mathrm{Ext}_A^1(B/A, \Omega) \to 0
$$

permet d’identifier $\Omega/\Omega_B$ à $\mathrm{Ext}_A^1(B/A, \Omega)$, donc d’après ce qui précède à $D(B/A)$. En particulier, on a $[B/A] = [\Omega/\Omega_B]$ dans $Z_0(A)$ et $\mathrm{Ann}_A(B/A) = \mathrm{Ann}_A(\Omega/\Omega_B)$ (§ 8, n° 4, prop. 4).

L’idéal $c = \mathrm{Ann}_A(B/A)$ est le transporteur $A : B$, c’est-à-dire (VII, § 1, n° 1) l’ensemble des éléments $x$ de $K$ tels que $xB \subset A$. C’est un idéal (non nul) de

A et de B ; c’est en fait le plus grand idéal de B contenu dans A. Puisque $\Omega_B : \Omega \subset \Omega : \Omega = A$ (n° 4, prop. 7, b)), on a $\operatorname{Ann}_A(\Omega/\Omega_B) = \Omega_B : \Omega$, d’où finalement
$$
c = \operatorname{Ann}_A(B/A) = \operatorname{Ann}_A(\Omega/\Omega_B) = \Omega_B : \Omega .
$$
Puisque $\Omega_B$ est un B-module, la relation $x \Omega \subset \Omega_B$ équivaut à $xB\Omega \subset \Omega_B$, de sorte que l’on a aussi $c = \Omega_B : B\Omega$.

Nous allons particulariser ce qui précède au cas où B est la clôture intégrale de A ; l’hypothèse que B soit un A-module de type fini est satisfaite lorsque l’anneau A est japonais (IX, § 4, n° 1, déf. 1), ce qui est le cas lorsqu’il est local et complet (*loc. cit.*, n° 2, th. 2), ou lorsqu’il est essentiellement de type fini sur un corps (*loc. cit.*, n° 1, remarque 2 et exemple). L’anneau B est alors un anneau de Dedekind (VII, § 2, n° 2, th. 1), et les B-modules sans torsion $\Omega_B$, $B\Omega$ et $c$ sont projectifs de rang 1 (VII, § 4, n° 10, prop. 22). La relation $c = \Omega_B : B\Omega$ signifie alors que l’application linéaire $c \otimes_B B\Omega \to \Omega_B$ déduite de l’action de K sur V est un isomorphisme (II, § 5, n° 6, prop. 11). On a en particulier $\Omega_B = c(B\Omega) = c\Omega$.

#### Proposition 9 {#ac-x-s9-prop-9 .statement}

*Soient B la clôture intégrale de A, et $c = A : B$. Supposons que B soit un A-module de type fini. On a l’inégalité $[B/c] \leq 2[B/A]$ dans $Z_0(A)$. Pour qu’il y ait égalité, il faut et il suffit que A soit un anneau de Gorenstein.*

On a $[B/c] = [B/A] + [A/c]$, de sorte que l’inégalité considérée équivaut à $[A/c] \leq [B/A]$.

A) Pour tout idéal maximal $m$ de A, la clôture intégrale de $A_m$ est $B_m$ (V, § 1, n° 5, cor. 1), et l’on a $c_m = A_m : B_m$. De plus on a par définition $[B/c] = \sum_m \operatorname{long}_{A_m}(B_m/c_m)[m]$ et $[B/A] = \sum_m \operatorname{long}_{A_m}(B_m/A_m)[m]$. Ceci nous ramène à démontrer la proposition lorsque l’anneau A est *local*, ce que nous supposerons désormais. Dans ce cas le groupe ordonné $Z_0(A)$ s’identifie canoniquement à $\mathbf{Z}$, de façon que la classe d’un module de longueur finie soit sa longueur. L’anneau B est semi-local et le B-module $B\Omega$ est libre de rang 1 (II, § 5, n° 3, prop. 5).

B) Si A est un anneau de Gorenstein, le A-module $\Omega$ est libre de rang 1 (n° 4, cor. 1 de la prop. 7) ; choisissons un générateur $\omega$ de $\Omega$. On a $\Omega = A\omega$ et $\Omega_B = c\Omega = c\omega$, et par suite $\operatorname{long}(A/c) = \operatorname{long}(\Omega/\Omega_B) = \operatorname{long}(B/A)$.

C) Supposons le corps résiduel $\kappa_A$ infini. Pour tout idéal maximal $n$ de B, notons $L(n)$ le $B/n$-espace vectoriel (de dimension 1) $B\Omega/nB\Omega$, et $\operatorname{pr}_n$ la projection canonique de $\bigoplus_n L(n)$ sur $L(n)$. Soit $\varphi : \Omega \longrightarrow \bigoplus_n L(n)$ la restriction à $\Omega$ de l’homomorphisme canonique $B\Omega \longrightarrow \bigoplus_n L(n)$. L’image de $\varphi$ est un sous-$\kappa_A$-espace vectoriel de $\bigoplus_n L(n)$ ; elle n’est pas contenue dans $\operatorname{Ker} \operatorname{pr}_n$, sans quoi l’on aurait $\Omega \subset nB\Omega$ et par suite $B\Omega \subset nB\Omega$, ce qui est contradictoire. Ainsi l’image de $\varphi$ n’est pas contenue dans la réunion des $\operatorname{Ker} \operatorname{pr}_n$ (A, V, p. 40, lemme 1) ; il existe donc un élément $\omega$ de $\Omega$ dont l’image dans $B\Omega/nB\Omega$ est non nulle pour tout $n$, ce qui entraîne que $\omega$ engendre le B-module $B\Omega$ (II, § 3, n° 3, prop. 11).

Soit $a \in A$ ; si $a\omega$ appartient à $\Omega_B$, on a $aB\omega \subset \Omega_B$, donc $a\Omega \subset \Omega_B$, ce qui implique $a \in c$. L’application $a \mapsto a\omega$ induit donc une injection de $A/c$ dans $\Omega/\Omega_B$ ; par suite on a $\operatorname{long}(A/c) \leq \operatorname{long}(\Omega/\Omega_B) = \operatorname{long}(B/A)$.

Si $\operatorname{long}(A/c) = \operatorname{long}(B/A)$, on a $A\omega + \Omega_B = \Omega$. On peut supposer que l’idéal $c$ est contenu dans $m_A$ (dans le cas contraire $A$ est égal à $B$, donc est un anneau de Gorenstein). Comme $\Omega_B = c\Omega$ est contenu dans $m_A\Omega$, il résulte du lemme de Nakayama que $\omega$ engendre $\Omega$. Ainsi le $A$-module $\Omega$ est monogène, donc libre de rang 1, ce qui signifie que $A$ est un anneau de Gorenstein (n° 4, cor. 1 de la prop. 7).

D) Traitons le cas général. Notons $A'$ l’anneau $A[X]$, c’est-à-dire (IX, App., n° 2) l’anneau local de l’anneau de polynômes $A[X]$ en l’idéal premier $m_A A[X]$; c’est une $A$-algèbre plate, intègre, de dimension 1, dont le corps résiduel $\kappa_{A'}$ s’identifie à $\kappa_A(X)$ et le corps des fractions à $K(X)$ (*loc. cit.*). D’après le cor. de la prop. 5 du n° 3, le $A'$-module $A' \otimes_A \Omega$ est dualisant. Posons $B' = A' \otimes_A B$; c’est la clôture intégrale de $A'$ dans $K(X)$ (V, § 1, n° 3, prop. 13 et n° 5, prop. 16). Le transporteur $c' = A' : B'$ est égal à $cA'$ (I, § 2, n° 10, formule (11)). Pour tout $A$-module $M$ de longueur finie, on a $\operatorname{long}_{A'}(A' \otimes_A M) = \operatorname{long}_A(M)$: en effet, comme la $A$-algèbre $A'$ est plate, il suffit de prouver cette relation lorsque $M$ est simple, c’est-à-dire isomorphe à $\kappa_A$; mais dans ce cas $A' \otimes_A \kappa_A$ s’identifie à $\kappa_{A'}$, d’où notre assertion. On a donc

$$
\operatorname{long}_A(B/c) = \operatorname{long}_{A'}(B'/c') \quad \text{et} \quad \operatorname{long}_A(B/A) = \operatorname{long}_{A'}(B'/A') .
$$

L’anneau $A'$ vérifie les hypothèses de la proposition, et son corps résiduel est infini. D’après la partie C) de la démonstration, on a $\operatorname{long}_{A'}(B'/c') \leq 2 \operatorname{long}_{A'}(B'/A')$, et l’égalité implique que $A'$ est un anneau de Gorenstein; mais cette dernière condition entraîne que $A$ est un anneau de Gorenstein (§ 3, n° 8, cor. 1 de la prop. 12).

## EXERCICES {#ac-x-s9-exercises}

See the [exercises for § 9](exercises/s9/).
