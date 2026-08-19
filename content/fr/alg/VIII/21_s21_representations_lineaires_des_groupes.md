---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Modules et anneaux semi-simples
section: 21
section_title: Représentations linéaires des groupes finis
lang: fr
source: alg-viii-fr
book_pages: A VIII.387-A VIII.424
pdf_pages: 0389-0426
extraction: native
subsections:
    - "no": 1
      title: Représentations linéaires
      page: 387
      pdf_page: 389
    - "no": 2
      title: Le théorème de Maschke
      page: 391
      pdf_page: 393
    - "no": 3
      title: Représentations induites et coïnduites
      page: 392
      pdf_page: 394
    - "no": 4
      title: Représentations et groupe de Grothendieck
      page: 394
      pdf_page: 396
    - "no": 5
      title: Formule d’inversion de Fourier
      page: 396
      pdf_page: 398
    - "no": 6
      title: Relations d’orthogonalité de Schur
      page: 399
      pdf_page: 401
    - "no": 7
      title: Relation d’orthogonalité des caractères
      page: 400
      pdf_page: 402
    - "no": 8
      title: Fonctions centrales sur un groupe fini
      page: 401
      pdf_page: 403
    - "no": 9
      title: Cas des groupes commutatifs
      page: 404
      pdf_page: 406
    - "no": 10
      title: Caractères et groupes de Grothendieck
      page: 405
      pdf_page: 407
    - "no": 11
      title: Dimension des représentations simples
      page: 405
      pdf_page: 407
    - "no": 12
      title: Changement de corps de base
      page: 406
      pdf_page: 408
    - "no": 13
      title: Représentations linéaires complexes
      page: 411
      pdf_page: 413
statements: 36
exercises: 30
content_sha256: fc469a596fe1d09bf5ebf4fa8e0d342aa984f2b391411a2237e7be8ccbf1c3f9
---

## § 21. REPRÉSENTATIONS LINÉAIRES DES GROUPES FINIS

Dans tout ce paragraphe, on désigne par G un groupe et par K un anneau commutatif. Si G est un groupe fini, on note $|G|$ l’élément Card(G)$.1$de K. A partir du n$^o5$, on suppose que le groupe G est fini, que le corps K est algébriquement clos et que $|G|$ n’est pas nul.

### 1. Représentations linéaires

#### Définition 1 {#alg-viii-s21-def-1 .statement tag=00NC}

Soit M un K-module. On appelle représentation linéaire de G dans M tout homomorphisme de groupes de G dans le groupe linéaire $\mathbf{G}\mathbf{L}(M)$ (II, p. 5).

Soit $\pi$ une représentation linéaire de G dans un K-module M. On dit aussi que le couple $(M, \pi )$ est une représentation linéaire de G. Lorsque K est non nul et que M est un K-module libre, la dimension de M est appelée le degré (ou la dimension) de la représentation $\pi$.

Rappelons que l’application canonique $g\rightarrow e_g$ de G dans l’algèbre K[G] du groupe G est une base du K-module K[G]. Par abus, on note également $g$ l’élément $e_g$ de K[G]. Étant donnée une représentation linéaire $\pi : G\rightarrow \mathbf{G}\mathbf{L}(M)$ de G, il existe un unique homomorphisme de K-algèbres de K[G] dans End$_K(M)$ qui prolonge $\pi$ (III, p. 20, exemple) ; on note encore $\pi$ ce prolongement. C’est une représentation de l’algèbre K[G] dans M (VIII, p. 365, déf. 1), de sorte que M est un K[G]-module. Inversement, toute représentation linéaire $\rho$ de l’algèbre K[G] dans M définit une représentation linéaire de G dans M donnée par $g\rightarrow \rho (g)$.

On utilisera librement pour les représentations linéaires du groupe G la terminologie se rapportant à la structure de K[G]-module. C’est ainsi qu’on parlera de sous-représentation, de représentation simple, de somme directe de représentations, etc. Soient $(M, \pi )$ et $(M', \pi ')$ des représentations linéaires de G ; on note Hom$_G(\pi , \pi ')$ le K-module Hom$_{K[G]}(M,M')$ des homomorphismes de K[G]-modules de M dans $M'$.[^1]

Une application $f$ de G dans K est appelée fonction centrale si l’on a $f(gg') =$ $f(g'g)$ pour tout couple d’éléments $g, g'$ de G ; il revient au même de dire que l’on a $f(ghg^{-1}) =f(h)$ pour tout couple d’éléments $g, h$ de G. Les fonctions centrales sont donc les fonctions sur G dont la restriction à chaque classe de conjugaison est constante. Elles forment un sous-module de l’espace des applications de G dans K, noté $\mathscr{Z}_K(G)$. Lorsque G est fini, la K-algèbre $\mathscr{Z}_K(G)$ est un K-module libre de dimension le nombre des classes de conjugaison de G. Le centre Z(K[G]) de l’algèbre K[G] est formé des éléments $a=\sum a_gg$ de K[G] tels que $hah^{-1}=a$ pour tout $h\in G$. Or on a

$$
hah^{-1}=\sum_{g\in G}a_{h^{-1}gh}g
$$

par suite, lorsque G est fini, le centre Z(K[G]) de l’algèbre K[G] se compose des fonctions centrales.

Soit $(M, \pi )$ une représentation linéaire de G. Supposons que M soit un K-module libre de dimension finie. On appelle trace de $\pi$ la trace de la représentation de K[G] associée à $\pi$, c’est-à-dire (VIII, p. 374) la forme linéaire $a\rightarrow$ Tr($\pi (a)$) sur K[G]. Cette forme linéaire est déterminée par l’application $g\rightarrow$ Tr($\pi (g)$) de G dans K, qu’on appelle caractère de la représentation $\pi$ et qu’on note $\chi_{\pi}$. Le caractère d’une représentation est une fonction centrale (II, p. 78, prop. 3).

Soient M et $M'$ des K-modules libres de dimension finie. Soient $\pi$ et $\pi '$ des représentations linéaires de G dans M et $M'$ respectivement. Alors $M\oplus M'$ est un K-module libre de dimension finie et, par la prop. 1 de III, p. 109, on a

$$
\chi_{\pi\oplus\pi'}=\chi_{\pi}+\chi_{\pi'}
$$

Plus généralement, soit

$$
0\longrightarrow M'\longrightarrow M\longrightarrow M''\longrightarrow 0
$$

une suite exacte de K[G] modules et soient $\pi ,\pi '$ et $\pi ''$ les représentations linéaires de G associées à $M, M'$ et $M''$ respectivement. On suppose que les K-modules $M'$ et $M''$ sont libres de dimension finie. Il en est alors de même de M (II, p. 27, prop. 21) et l’on a

$$
\chi_{\pi}=\chi_{\pi'}+\chi_{\pi''} \tag{1}
$$

#### Proposition 1 {#alg-viii-s21-prop-1 .statement tag=00ND}

On suppose que K est un corps commutatif. Soient $\pi$ et $\pi '$ des représentations K-linéaires semi-simples de dimension finie de G.

a) Si les polynômes caractéristiques de $\pi (g)$et de $\pi '(g)$sont les mêmes pour tout $g\in G$, alors les représentations $\pi$ et $\pi '$ sont isomorphes.

b) On suppose en outre que K est de caractéristique 0. Si les caractères $\chi_{\pi}$ et $\chi_{\pi'}$ sont égaux, alors les représentations $\pi$ et $\pi '$ sont isomorphes.

L’assertion a) résulte du cor. 1 de VIII, p. 378 ; l’assertion b) découle du corollaire de VIII, p. 376, a).

#### Exemple 1 {#alg-viii-s21-n1-exa-1 .statement tag=00NE}

La représentation unité de G est la représentation $(K, \varepsilon )$ où $\varepsilon (g) =$ Id$_K$ pour tout $g\in G$. Son caractère est la fonction constante de valeur 1.

#### Exemple 2 {#alg-viii-s21-n1-exa-2 .statement tag=00NF}

La représentation régulière (gauche) de G est la représentation $\boldsymbol{\gamma }$ de G dans K[G] définie par $\boldsymbol{\gamma }(g)(x) =gx$ pour $g\in G$ et $x\in K[G]$. Elle correspond à la représentation régulière gauche de l’algèbre K[G] (VIII, p. 367). Supposons le groupe G fini. La représentation régulière est donc de degré fini. Pour tout élément $g$ de G distinct de l’élément neutre, la matrice de la multiplication à gauche par $g$ dans K[G], par rapport à la base canonique, est la matrice d’une permutation sans point fixe. On a donc

$|G|$ si $g$ est l’élément neutre,

$$
\chi_{\boldsymbol{\gamma }}(g) = \tag{2}
$$

0 sinon.

On définit de façon similaire la représentation régulière droite de G. La représentation birégulière de G est la représentation $\rho$ de $G\times G$ dans K[G] définie par $\rho (g, g')(x) =gxg^{'-1}$ pour tout $(g, g')\in G\times G$ et tout $x\in K[G]$.

#### Exemple 3 {#alg-viii-s21-n1-exa-3 .statement tag=00NG}

Étant donnée une représentation linéaire $(M, \pi )$ de G, la représentation contragrédiente ou duale $\pi^{\vee}$ de $\pi$ est la représentation de G dans le K-module dual de M définie par la relation $\pi^{\vee}(g) =^t\pi (g^{-1})$ pour tout $g\in G ($cf. II, p. 42). Si M est un K-module libre de dimension finie, il en est de même de son dual et on a $\chi_{\pi^{\vee}}(g) =\chi_{\pi}(g^{-1})$ pour tout $g\in G$.

#### Exemple 4 {#alg-viii-s21-n1-exa-4 .statement tag=00NH}

Soient $(M, \pi )$ et $(M', \pi ')$ des représentations linéaires de G. On a défini dans l’exemple 1 de VIII, p. 193 une structure de K[G]-module sur $M\otimes_KM'$. La représentation linéaire correspondante est appelée produit tensoriel de $\pi$ et $\pi '$ et notée $\pi \otimes \pi '$. Pour $g\in G,x\in M$ et $x'\in M'$, on a $((\pi \otimes \pi ')(g))(x\otimes x') =\pi (g)x\otimes \pi '(g)x'$.

Si M et $M'$ sont des K-modules libres de dimension finie, on a, d’après la prop. 2 de III, p. 109,

$$
\chi_{\pi\otimes\pi'}=\chi_{\pi}\chi_{\pi'} \tag{3}
$$

#### Exemple 5 {#alg-viii-s21-n1-exa-5 .statement tag=00NI}

Supposons que G soit le produit $G'\times G''$ de deux groupes. L’application K-linéaire de $K[G']\otimes_KK[G'']$ dans K[G] qui envoie $g'\otimes g''$ sur $(g', g'')$ pour $g'\in G'$ et $g''\in G''$ est un isomorphisme d’algèbres. Soient $(M', \pi ')$ une représentation linéaire de $G'$, et $(M'', \pi '')$ une représentation linéaire de $G''$. On appelle produit tensoriel externe de $\pi '$ et $\pi ''$, et on note $\pi '_{\boxtimes}\pi ''$, la représentation de $G'\times G''$ dans l’espace vectoriel $M'\otimes M''$ définie par $(\pi '_{\boxtimes}\pi '')(g', g'') =\pi '(g')\otimes \pi ''(g'')$ pour $(g', g'')\in G'\times G''$. Si $M'$ et $M''$ sont des K-modules libres de dimension finie, alors $M'\otimes_KM''$ est un K-module libre de dimension finie et le caractère de la représentation $\pi '_{\boxtimes}\pi ''$ est donné par la formule

$$
\chi_{\pi'_{\boxtimes}\pi''}(g', g'') =\chi_{\pi'}(g')\chi_{\pi''}(g'')
$$

pour $g'\in G'$ et $g''\in G''$ (prop. 2 de III, p. 109).

#### Exemple 6 {#alg-viii-s21-n1-exa-6 .statement tag=00NJ}

Soit $(V, \pi )$ une représentation linéaire de G, tel que V soit un K-module libre de dimension finie. On définit une représentation $\rho$ de $G\times G$ dans End$_K(V)$ par la formule

$$
\rho (g, g')(u) =\pi (g')\circ u\circ \pi (g^{-1})
$$

L’isomorphisme de K-modules $\theta_V: V^*\otimes_KV\rightarrow$ End$_K(V)$ de II, p. 77, est un isomorphime de représentations du produit tensoriel externe $\pi^{\vee}\times \pi$ sur $\rho$. L’application $g\rightarrow \rho (1, g)$ (resp. $g\rightarrow \rho (g,1)$) est une représentation de G isomorphe à $\pi^{dim_KV}$ (resp. $(\pi^{\vee})^{dim_KV}$).

Soit L une K-algèbre commutative et soit $(M, \pi )$ une représentation linéaire du groupe G. L’homomorphisme de groupes $\pi_{(L)}: G\rightarrow \mathbf{G}\mathbf{L}(M_{(L)})$ défini par $g\rightarrow$ Id$_L\otimes \pi (g)$ est une représentation linéaire de G dans le L-module $M_{(L)}$, appelée la représentation linéaire de G déduite de la représentation $\pi$ par extension à L de l’anneau K des scalaires.

Supposons que K soit un corps et que L soit une K algèbre commutative non nulle. Soient $(M, \pi )$ et $(M', \pi ')$ des représentations linéaires de G. Les représentations $\pi$ et $\pi '$ sont isomorphes si et seulement si $\pi_{(L)}$ et $\pi '_{(L)}$ le sont (VIII, p. 34, th. 3).

On suppose en outre que l’algèbre L est une extension de K. Considérons les anneaux $R_K(G)$ et $R_L(G)$ définis dans l’exemple 1 de VIII, p. 193. L’extension des scalaires définit un homomorphisme d’anneaux

$$
u: R_K(G)\longrightarrow R_L(G)
$$

Cet homomorphisme est injectif et un élément $\xi \in R_K(G)$ est effectif si et seulement si $u(\xi )$ l’est (VIII, p. 191, th. 1).

### 2. Le théorème de Maschke

#### Théorème 1 {#alg-viii-s21-thm-1 .statement tag=00NK}

On suppose que le groupe G est fini. Soit M un K[G]-module, soit N un sous-K[G]-module de M. On suppose que N est un facteur direct du K-module M et que $|G|$ est inversible dans K. Alors N est un facteur direct du K[G]module M.

Soit $p$ un projecteur K-linéaire dans M, d’image N. On définit un endomorphisme $q$ du K-module M en posant

$$
q(x) =|G|^{-1}\sum_{g\in G}g p(g^{-1}x)
$$

pour tout $x\in M$. Comme N est stable pour l’action de G et que $p$ induit l’identité sur N, on voit que $q$ applique M dans N et induit l’identité sur N.

Le K-module M est donc somme directe de l’image N de $q$ et du noyau de $q$. On a $g q(x) =q(gx)$ pour tout $x\in M$ et tout $g\in G$, de sorte que le noyau de $q$ est un sous-K[G]-module de M. Cela prouve que N est facteur direct du K[G]-module M.

#### Corollaire 1 (Maschke) {#alg-viii-s21-thm-1-cor-1 .statement tag=00SC}

On suppose que le groupe G est fini et que K est un corps commutatif. L’algèbre K[G] est semi-simple si et seulement si l’élément $|G|$ du corps K n’est pas nul.

Supposons $|G| \not= 0$. Par le th. 1, tout sous-K[G]-module de $K[G]_s$ est un facteur direct. Donc K[G] est semi-simple.

Inversement, supposons $|G|$ nul et notons $\varepsilon$ l’élément $\sum_{g\in G}g$ du centre de K[G]. On a $\varepsilon \not= 0$ mais $\varepsilon^2=|G|\varepsilon = 0$ donc K[G] n’est pas semi-simple (VIII, p. 149, prop. 3 a) et VIII, p. 153, remarque 1).

#### Corollaire 2 {#alg-viii-s21-thm-1-cor-2 .statement tag=00NL}

On suppose que le groupe G est fini et que $|G|$ est inversible dans K. Une suite exacte de K[G]-modules est scindée si et seulement si elle est scindée en tant que suite exacte de K-modules.

Étant donnée une suite exacte de K[G]-modules

0 // ${M'}^f$ // M // $M''$ // $0$,

il suffit d’appliquer le théorème 1 à l’image du morphisme $f$.

#### Corollaire 3 {#alg-viii-s21-thm-1-cor-3 .statement tag=00NM}

On suppose que le groupe G est fini et que $|G|$ est inversible dans K. Un K[G]-module est projectif si et seulement s’il est projectif en tant que K-module.

Soit P un K[G]-module. Si P est facteur direct d’un K[G]-module libre M, il est a fortiori facteur direct du K-module libre M. La réciproque résulte du corollaire 2, compte tenu de II, p. 39, prop. 4, d).

#### Corollaire 4 {#alg-viii-s21-thm-1-cor-4 .statement tag=00NN}

a) On suppose que le groupe G est fini et que K est un corps commutatif de caractéristique 0. Pour que deux représentations linéaires, de dimension finie, de G soient isomorphes, il faut et il suffit qu’elles aient même caractère.

b) Supposons que K soit un corps parfait de caractéristique un nombre premier $p$ et que le groupe G soit fini, de cardinal premier à $p$. Pour que le caractère d’une représentation linéaire de dimension finie de G soit nul, il faut et il suffit que cette représentation soit isomorphe à la somme directe de $p$ représentations deux à deux isomorphes.

Sous les hypothèses du corollaire, toute représentation linéaire de dimension finie de G est semi-simple. Le corollaire résulte alors du cor. de VIII, p. 376.

#### Corollaire 5 {#alg-viii-s21-thm-1-cor-5 .statement tag=00NO}

Supposons que le groupe G est fini et que K est un corps commutatif dans lequel $|G| \not= 0$. Soient $\pi$ et $\pi '$ des représentations linéaires de dimension finie de G. Pour que $\pi$ et $\pi '$ soient isomorphes, il faut et il suffit que, pour tout $g$ dans G, les endomorphismes $\pi (g)$et $\pi '(g)$aient mêmes polynômes caractéristiques.

Cela résulte du cor. 1 de VIII, p. 378.

### 3. Représentations induites et coïnduites

Soit H un sous-groupe du groupe G.

Si $(V, \pi )$ est une représentation linéaire de G, la restriction de $\pi$ à H est une représentation linéaire de H dans V ; on la note Res$^G_H(\pi )$. Le K[H]-module associé à Res$^G_H(\pi )$ n’est autre que le module déduit du K[G]-module V par restriction des scalaires (II, p. 30). Si V est un K-module libre de dimension finie, le caractère de Res$^G_H(\pi )$ est la restriction à H du caractère de $\pi$.

Soit $(M, \sigma )$ une représentation de H.

Considérons K[G] comme un $(K[G]$, K[H])-bimodule et M comme un K[H]module. Le K[G]-module $\mathscr{T}(M) = K[G]\otimes_{K[H]}M$ (VIII, p. 54) définit une représentation linéaire de G, notée Ind$^G_H(\sigma )$ et qu’on appelle la représentation de G induite par $\sigma$. Si $(V, \pi )$ est une représentation linéaire de G, le K[H]-module $\mathscr{H}(V) =$ Hom$_{K[G]}(K[G],V)$ s’identifie au K[H]-module correspondant à la représentation Res$^G_H(\pi )$. Par conséquent, le morphisme d’adjonction (VIII, p. 55) fournit un isomorphisme dit canonique de K-modules de Hom$_H(\sigma$, Res$^G_H(\pi ))$ sur Hom$_G$(Ind$^G_H(\sigma ), \pi$ ) (« réciprocité de Frobenius »).

Considérons K[G] comme un $(K[H]$, K[G])-bimodule. Le K[G]-module $\mathscr{H}(M) =$ Hom$_{K[H]}(K[G],M)$ définit une représentation de G, notée Coïnd$^G_H(\sigma )$ et qu’on appelle la représentation de G coïnduite par $\sigma$. Si $(V, \pi )$ est une représentation linéaire de G, le K[H]-module $\mathscr{T}(V) = K[G]\otimes_{K[G]}V$ s’identifie au K[H]-module correspondant à la représentation Res$^G_H(\pi )$. Par conséquent, le morphisme d’adjonction (loc. cit.) fournit un isomorphisme dit canonique de K-modules de Hom$_H$(Res$^G_H(\pi ), \sigma$ ) sur Hom$_G(\pi$, Coïnd$^G_H(\sigma ))$.

Soit $\varepsilon : K[G]\rightarrow K[H]$ l’homomorphisme de K-modules caractérisé par les relations $\varepsilon (h) =h$ si $h\in H$ et $\varepsilon (g) = 0$ si $g\in G$ - H. L’application $\varepsilon$ est un homomorphisme de $(K[H]$, K[H])-bimodules. Soit $(M, \sigma )$ une représentation linéaire de H. L’application $v\rightarrow v\circ \varepsilon$ de Hom$_{K[H]}(K[H],M)$ dans Hom$_{K[H]}(K[G],M)$ est un homomorphisme de K[H]-modules. En identifiant M avec Hom$_{K[H]}(K[H],M)$, on obtient un homomorphisme de K[H]-modules de M dans Res$^G_H$(Coïnd$^G_H(\sigma )$). La réciprocité de Frobenius lui associe un homomorphisme $\iota$ de K[G]-modules de Ind$^G_H(\sigma )$ dans Coïnd$^G_H(\sigma )$ qui est caractérisé par les relations

$$
\iota (g\otimes m)(g') =\varepsilon (g'g)m
$$

pour $g, g'\in G$ et $m\in M$. Cet homomorphisme sera dit canonique.

#### Proposition 2 {#alg-viii-s21-prop-2 .statement tag=00NP}

Soit H un sous-groupe de G et soit $(M, \sigma )$une représentation linéaire de H. L’homomorphisme canonique $\iota :$ Ind$^G_H(\sigma )\rightarrow$ Coïnd$^G_H(\sigma )$est injectif. Si le sous-groupe H est d’indice fini dans G, c’est un isomorphisme de K[G]-modules.

Soit $S\subset G$ un système de représentants de $G/H$. La famille $(s)_{s\in S}$ est une base du K[H]-module à droite K[G]. Il en résulte que l’application $M^{(S)}\rightarrow$ Ind$^G_H(\sigma )$ définie par $(m_s)_{s\in S}\rightarrow \sum_{s\in S}s\otimes m_s$ est un isomorphisme de K-modules. Pour tous $s, s'\in S$ et tout $m\in M$, on a les relations

$$
\iota (s'\otimes m)(s^{-1}) =\begin{cases} m & \text{si } s=s',\\ 0 & \text{sinon.}\end{cases}
$$

Il en résulte que $\iota$ est injective.

Supposons que H est d’indice fini dans G. L’ensemble S est alors fini ; soit $\rho$ l’application de Coïnd$^G_H(\sigma )$ dans Ind$^G_H(\sigma )$ donnée par $u\rightarrow \sum_{s\in S}s\otimes u(s^{-1})$. Elle vérifie $(\iota \circ \rho (u))(s^{-1}) =u(s^{-1})$ pour $u\in$ Coïnd$^G_H(\sigma )$ et $s\in S$. Comme la famille $(s^{-1})_{s\in S}$ est une base de K[H]-module à gauche K[G], l’application $\iota \circ \rho$ est l’application identique. Par suite, $\iota$ est bijective de bijection réciproque $\rho$.

Soit H un sous-groupe d’indice fini de G. Soit $u$ une fonction centrale sur H ; notons $u^0$ la fonction sur G qui prolonge $u$ et qui s’annule en tout point de G- H. Soit S un système de représentants de $G/H$. Pour $g\in G$, posons

(4) Ind$^G_H(u)(g) =\sum_{s\in S}u^0(s^{-1}gs)$.

Notons que, pour tous $x, g\in G$ et tout $h\in H$ on a $u^0((xh)^{-1}gxh) =u^0(x^{-1}gx)$. Il en résulte que Ind$^G_H(u)$ est une fonction centrale sur G, indépendante du choix de S. On définit ainsi une application K-linéaire Ind$^G_H$ de $\mathscr{Z}_K(H)$ dans $\mathscr{Z}_K(G)$.

#### Proposition 3 {#alg-viii-s21-prop-3 .statement tag=00NQ}

Soit H un sous-groupe d’indice fini de G. Soit $(M, \sigma )$une représentation linéaire de H. Supposons que M est un K-module libre de dimension finie. Notons $(V, \pi )$la représentation de G induite par $\sigma$. Alors le K-module V est libre de dimension finie et

(5) $\chi_{\pi}=$ Ind$^G_H(\chi_{\sigma})$.

Soit S un système de représentants de $G/H$. Comme on l’a vu plus haut, l’application linéaire $M^S\rightarrow$ Ind$^G_H(M)$ donnée par $(m_s)_{s\in S}\rightarrow \sum_{s\in S}s\otimes m_s$ est un isomorphisme de K-modules. En particulier, V est un K-module libre de dimension finie. Pour tout $g\in G$, notons $M_g$ l’image de M par l’application $m\rightarrow g\otimes m$. Pour tous $g, g'\in G$, on a que $M_g= M_{g'}$ si et seulement si $gH =g'H$ et V est somme directe des sous-modules $M_s$ pour $s\in S$. Pour tous $g, g'\in G$ on a également $\pi (g)M_{g'}= M_{gg'}$. Pour tout $g\in G$, notons $S_g$ l’ensemble des éléments $s$ de S tels que $s^{-1}gs\in H$. Pour tous $g, g'\in G$ tels que $g^{'-1}gg'\in H$, l’automorphisme $\pi (g)$ de V induit un automorphisme $\pi (g)_{g'}$ de $M_{g'}$ et l’on a

Tr($\pi (g)$) $=\sum_{s\in S_g}$ Tr($\pi (g)_s$) $=\sum_{s\in S_g}$ Tr($\sigma (s^{-1}gs)$).

La dernière assertion en résulte.

### 4. Représentations et groupe de Grothendieck

On suppose dans ce numéro que K est un corps commutatif. Étant donnée une représentation linéaire $(M, \pi )$ de G, de dimension finie, on note $[\pi ]$ la classe du K[G]-module M dans l’anneau de Grothendieck $R_K(G)$ (VIII, p. 193, exemple 1).

Par définition des lois de composition de l’anneau $R_K$(G), si $\pi$ et $\pi '$ sont des représentations linéaires de dimension finie de G, on a

$$
[\pi \oplus \pi '] = [\pi ] + [\pi '],[\pi \otimes \pi '] = [\pi ] [\pi ']
$$

L’élément unité de l’anneau $R_K(G)$ est la classe de la représentation unité de G (VIII, p. 389, exemple 1).

L’anneau $R_K(G)$ est un $\mathbf{Z}$-module libre ayant pour base l’ensemble des classes des K[G]-modules simples de dimension finie sur K. Lorsque $|G|$ est inversible dans K, pour que deux représentations de dimension finie soient isomorphes, il faut et il suffit qu’elles aient la même classe dans $R_K(G)$ (VIII, p. 186, cor. et p. 391, cor. 1).

Étant donnée une représentation linéaire $(M, \pi )$ de dimension finie de G, sa contragrédiente $\pi^{\vee}$ est également de dimension finie. Les représentations $\pi$ et $(\pi^{\vee})^{\vee}$ sont isomorphes. Si $\pi '$ est également une représentation linéaire de dimension finie de G, les représentations $(\pi \otimes \pi ')^{\vee}$ et $\pi^{\vee}\otimes \pi^{'\vee}$ sont isomorphes. Si

$$
0\longrightarrow M'\longrightarrow M\longrightarrow M''\longrightarrow 0
$$

est une suite exacte de K[G]-modules de dimension finie sur K alors les représentations contragrédientes fournissent une suite exacte de K[G]-modules

$$
0\longrightarrow M^{''\vee}\longrightarrow M^{\vee}\longrightarrow M^{'\vee}\longrightarrow 0
$$

(II, p. 102, cor. du th. 5). En raison de la propriété universelle des groupes de Grothendieck (VIII, p. 182, prop. 4), il existe un automorphisme $c\rightarrow c^{\vee}$ de l’anneau $R_K(G)$ caractérisé par $[\pi ]^{\vee}= [\pi^{\vee}]$ pour toute représentation linéaire $\pi$ de G de dimension finie ; on a $(c^{\vee})^{\vee}=c$ pour tout élément $c$ de $R_K(G)$.

Soit H un sous-groupe de G. La restriction préserve les suites exactes. D’après la propriété universelle des groupes de Grothendieck (VIII, p. 182, prop. 4), il existe donc un homomorphisme de groupes, noté Res$^G_H$, de $R_K(G)$ dans $R_K(H)$ caractérisé par les relations

(6) Res$^G_H[\pi ] =$ [Res$^G_H(\pi )]$

pour toute représentation linéaire $\pi$ de G de dimension finie ; c’est un homomorphisme d’anneaux. Si H est d’indice fini dans G, par la prop. 14 de II, p. 108, on définit de manière analogue un homomorphisme de groupes Ind$^G_H$ de $R_K(H)$ dans $R_K(G)$ caractérisé par les relations

(7) Ind$^G_H[\sigma ] =$ [Ind$^G_H(\sigma )]$

pour toute représentation linéaire $\sigma$ de H de dimension finie.

D’après les relations (1) de VIII, p. 388 et (3) de VIII, p. 389 et la propriété universelle déjà citée des groupes de Grothendieck, il existe un homomorphisme d’anneaux $\Theta_G$ de $R_K(G)$ dans l’algèbre $\mathscr{Z}_K(G)$ des fonctions centrales sur G, caractérisé par $\Theta_G([\pi ]) =\chi_{\pi}$ pour toute représentation $\pi$ de dimension finie de G.

Si H est un sous-groupe de G, les homomorphismes $\Theta_G$ et $\Theta_H$ relatifs aux groupes G et H sont compatibles avec les opérations Res$^G_H$ et Ind$^G_H$ (VIII, p. 392 et VIII, p. 394, prop. 3).

Supposons que G soit le produit $G'\times G''$ de deux groupes. D’après VIII, p. 209, remarque 2, Il existe une application $\mathbf{Z}$-linéaire $\kappa$ de $R_K(G')\otimes_{\mathbf{Z}}R_K(G'')$ dans le groupe $R_K(G'\times G'')$ caractérisée par les relations $\kappa ([\pi ']\otimes [\pi '']) = [\pi '_{\boxtimes}\pi '']$ pour $\pi '$ (resp. $\pi ''$) une représentation de $G'$ (resp. $G''$) de dimension finie, $\pi '_{\boxtimes}\pi ''$ désignant leur produit tensoriel externe (VIII, p. 390, exemple 5). C’est un homomorphisme d’anneaux. Si le corps K est algébriquement clos, l’application $\kappa$ est un isomorphisme (VIII, p. 209, remarque 2).

Supposons que G soit le produit $G'\times G''$ de deux groupes. Notons $\psi$ l’homomorphisme de $\mathscr{Z}_K(G')\otimes_K\mathscr{Z}_K(G'')$ sur $\mathscr{Z}_K(G)$ qui transforme $f'\otimes f''$ en la fonction $(g', g'')\rightarrow f'(g')f''(g'')$. On a un diagramme commutatif

$R_K(G')\otimes_{\mathbf{Z}}R_K(G'')^{\kappa}$ // $R_K(G)$

$\Theta_{G'}\otimes \Theta_{G''}\Theta_G$

$\mathscr{Z}_K(G')\otimes_K\mathscr{Z}_K(G'')^{\psi}$ /$/\mathscr{Z}_K(G)$.

### 5. Formule d’inversion de Fourier

On suppose pour le reste de ce paragraphe que le groupe G est fini, que K est un corps algébriquement clos, dont la caractéristique ne divise pas l’ordre de G, de sorte que l’élément $|G|$ de K n’est pas nul.

L’algèbre K[G] est semi-simple (théorème de Maschke) et de dimension finie. Notons $\widehat{G}$ l’ensemble des classes de K[G]-modules simples. Pour tout $\lambda \in \widehat{G}$, choisissons une représentation linéaire $(V_{\lambda}, \pi_{\lambda})$ de G dont le K[G]-module associé ait pour classe $\lambda$. L’ensemble $\widehat{G}$ est fini et les espaces vectoriels $V_{\lambda}$ sont de dimension finie (VIII, p. 137, exemple). Pour tout $\lambda \in \widehat{G}$, notons $d_{\lambda}$ le degré de la représentation $\pi_{\lambda}$, c’est-à-dire la dimension du K-espace vectoriel $V_{\lambda}$, et $\chi_{\lambda}$ son caractère.

Notons $F(\widehat{G})$ l’algèbre produit $\prod_{\lambda\in\widehat{G}}$ End$_K(V_{\lambda})$ et $\overline{\mathscr{F}}$ l’application de K[G] dans $F(\widehat{G})$ définie par $\overline{\mathscr{F}}(a) = (\pi_{\lambda}(a))_{\lambda\in\widehat{G}}$. Comme le corps K est algébriquement clos, l’application $\mathscr{F}$ est un isomorphisme d’algèbres (loc. cit.).

Pour tout $\lambda \in \widehat{G}$, la dimension de l’algèbre End$_K(V_{\lambda})$ est $d^2_{\lambda}$; celle de l’algèbre K[G] est Card(G) ; on a donc la relation

(8) Card(G) $=\sum_{\lambda\in\widehat{G}}d^2_{\lambda}$.

Notons $\tau$ la trace dans l’algèbre K[G] ; par définition, la trace $\tau (a)$ d’un élément $a$ de K[G] est la trace de l’endomorphisme $x\rightarrow ax$ de K[G] (III, p. 110). Soit $a=\sum_{g\in G}a_gg$ un élément de K[G] ; d’après la formule (2), on a $\tau (ag^{-1}) =|G|a_g$ pour tout $g\in G$, d’où la relation

$$
a=|G|^{-1}\sum_{g\in G}\tau (ag^{-1})g \tag{9}
$$

Notons $\widehat{\tau}$ la trace dans l’algèbre $F(\widehat{G})$. Soit $A = (A_{\lambda})_{\lambda\in\widehat{G}}$ un élément de $F(\widehat{G})$; on a (cf. III, p. 111, exemple 3)

(10) $\widehat{\tau}(A) =\sum_{\lambda\in\widehat{G}}d_{\lambda}$ Tr(A$_{\lambda}$).

Comme l’application $\overline{\mathscr{F}}$ est un isomorphisme de K-algèbres, on a $\widehat{\tau}\circ \overline{\mathscr{F}}=\tau$, d’où

$\tau (a) =\widehat{\tau}(\overline{\mathscr{F}}(a)) =\widehat{\tau}((\pi_{\lambda}(a))_{\lambda\in\widehat{G}})=\sum_{\lambda\in\widehat{G}}d_{\lambda}$ Tr($\pi_{\lambda}(a)$) $=\sum_{\lambda\in\widehat{G}}d_{\lambda}$ Tr$_{\lambda}(a)$

pour tout $a\in K[G]$, c’est-à-dire

(11) $\tau =\sum_{\lambda\in\widehat{G}}d_{\lambda}$ Tr$_{\lambda}$.

D’après (2), pour $g\in G$, on a donc

$\sum|G|$ si $g$ est l’élément neutre

$$
d_{\lambda}\chi_{\lambda}(g) = \tag{12}
$$

$_{\lambda\in\widehat{G}}$ 0 sinon.

Pour $a\in K[G]$, la relation (9) prend la forme suivante :

(13) $a=|G|^{-1}\sum_{g\in G}\sum_{\lambda\in\widehat{G}}d_{\lambda}$ Tr($\pi_{\lambda}(a)\pi_{\lambda}(g^{-1})$)$g$;

il en résulte que, pour tout élément $A = (A_{\lambda})_{\lambda\in\widehat{G}}$ de $F(\widehat{G})$, on a

(14) $\overline{\mathscr{F}}^{-1}(A) =|G|^{-1}\sum_{g\in G}\sum_{\lambda\in\widehat{G}}d_{\lambda}$ Tr(A$_{\lambda}\pi_{\lambda}(g^{-1})$)$g$.

(« Formule d’inversion de Fourier »).

Pour $\mu \in \widehat{G}$, notons $j_{\mu}:$ End$_K(V_{\mu})\longrightarrow \prod_{\lambda\in\widehat{G}}$ End$_K(V_{\lambda})$ l’application telle que $j_{\mu}(u) = (v_{\lambda})$ où $v_{\lambda}= 0$ si $\lambda \not=\mu$ et $v_{\mu}=u$. Par la formule (14),

(15) $\overline{\mathscr{F}}^{-1}(j_{\mu}(u)) =|G|^{-1}d_{\mu}\sum_{g\in G}$ Tr($u\pi_{\mu}(g^{-1})$)$g$.

Le centre de l’algèbre $F(\widehat{G}) =\prod_{\lambda\in\widehat{G}}$ End$_K(V_{\lambda})$ se compose des familles $(a_{\lambda}1_{V_{\lambda}})_{\lambda\in\widehat{G}}$, où $(a_{\lambda})$ est une famille d’éléments de K. C’est l’image par $\mathscr{F}$ du centre de l’algèbre K[G]. Celui-ci possède donc une base $(e_{\lambda})_{\lambda\in\widehat{G}}$ caractérisée par la condition

$$
\pi_{\lambda}(e_{\mu}) =\delta_{\lambda \mu}1_{V_{\lambda}} \tag{16}
$$

pour $\lambda , \mu \in \widehat{G}$, où $\delta_{\lambda \mu}$ désigne le symbole de Kronecker. D’après la formule (15), on a, pour tout $\mu \in \widehat{G}$,

$$
e_{\mu}=|G|^{-1}d_{\mu}\sum_{g\in G}\chi_{\mu}(g^{-1})g \tag{17}
$$

Ces éléments satisfont aux relations

(18) $\sum_{\lambda\in\widehat{G}}e_{\lambda}= 1,e^2_{\mu}=e_{\mu}$, et $e_{\mu}e_{\nu}= 0$

pour tous $\mu , \nu \in \widehat{G}$ tels que $\mu \not=\nu$; ce sont les idempotents indécomposables de Z(K[G]) (VIII, p. 143, prop. 15)

#### Remarque {#alg-viii-s21-n5-rem-1 .statement tag=00NR}

Soit $(V, \pi )$ une représentation linéaire de G. D’après le théorème de Maschke, le K[G]-module V est semi-simple. Pour tout $\lambda \in \widehat{G}$, notons $V^{\lambda}$ le composant isotypique de type $\lambda$ du K[G]-module V ; on a $V =\bigoplus_{\lambda\in\widehat{G}}V^{\lambda}$. D’après la prop. 15 de VIII, p. 143 et la formule (17), le projecteur de V d’image $V^{\lambda}$ associé à cette décomposition de V est égal à

$$
\pi (e_{\lambda}) =|G|^{-1}d_{\lambda}\sum_{g\in G}\chi_{\lambda}(g^{-1})\pi (g) \tag{19}
$$

En appliquant cette formule à $\pi =\pi_{\lambda}$, on obtient que l’élément $d_{\lambda}.1$ de K n’est pas nul. Nous verrons plus loin (VIII, p. 410, cor. 2) que $d_{\mu}$ divise le cardinal de G.

Soit $\lambda$ un élément de $\widehat{G}$. L’application $\pi_{\lambda}$ de K[G] dans End$_K(V_{\lambda})$ induit un isomorphisme de $(K[G],K[G])$ bimodules de $e_{\lambda}K[G]$ sur End$_K(V_{\lambda})$. Par la prop. 15 de VIII, p. 143, le sous-K[G]-module $e_{\lambda}K[G]$ est le composant isotypique de type $\lambda$ de K[G]. C’est aussi le composant isotypique de type $\lambda^{\vee}$ pour le représentation régulière droite de G (VIII, p. 139, prop. 11) ainsi que le composant isotypique de type $\lambda \times \lambda^{\vee}$ pour la représentation birégulière (VIII, p. 373, prop. 4).

### 6. Relations d’orthogonalité de Schur

Conservons les notations du numéro précédent. Soient $\lambda$ un élément de $\widehat{G},u$ et $v$ des éléments de End$_K(V_{\lambda})$; d’après la formule (10), on a

$\widehat{\tau}(j_{\lambda}(u)j_{\lambda}(v)) =d_{\lambda}$ Tr($uv$).

Comme $\tau = \widehat{\tau}\circ \overline{\mathscr{F}}$, on déduit des formules (2) et (15) la relation

$d^2_{\lambda}|G|^{-1}\sum_{g\in G}$ Tr($u\pi_{\lambda}(g)$) Tr($v\pi_{\lambda}(g^{-1})$) $=d_{\lambda}$ Tr($uv$).

On a remarqué plus haut que $d_{\lambda}.1\not= 0$ dans le corps K ; on en déduit

(20) $|G|^{-1}\sum_{g\in G}$ Tr($u\pi_{\lambda}(g)$) Tr($v\pi_{\lambda}(g^{-1})$) $=d^{-1}_{\lambda}$ Tr($uv$).

Spécialisons cette relation au cas où $u$ et $v$ sont de rang $\leqslant 1$; on obtient

$$
|G|^{-1}\sum_{g\in G}\langle x^*, \pi_{\lambda}(g)x\rangle  \langle y^*, \pi_{\lambda}(g^{-1})y\rangle =d^{-1}_{\lambda}\langle x^*, y\rangle \langle y^*, x\rangle \tag{21}
$$

pour $x,y$ dans $V_{\lambda}$ et $x^*, y^*$ dans le dual $V^*_{\lambda}$ de $V_{\lambda}$.

Pour tout $\lambda \in \widehat{G}$, soit $(e_{\lambda ,j})_{1\leqslant j\leqslant d_{\lambda}}$ une base de $V_{\lambda}$; notons $(\pi_{ij}^{\lambda}(g))$ la matrice de l’endomorphisme $\pi_{\lambda}(g)$ de $V_{\lambda}$ par rapport à cette base. Si l’on note $(e^*_{\lambda ,i})_{1\leqslant i\leqslant d_{\lambda}}$ la base de $V^*_{\lambda}$ duale de $(e_{\lambda ,j})$, on a $\pi_{ij}^{\lambda}(g) =\langle e^*_{\lambda ,i}, \pi_{\lambda}(g)e_{\lambda ,j}\rangle$, d’où

$$
|G|^{-1}\sum_{g\in G}\pi^{\lambda}_{ij}(g)\pi^{\lambda}_{k\ell}(g^{-1}) =d^{-1}_{\lambda}\delta_{i\ell}\delta_{jk} \tag{22}
$$

Soient maintenant $\lambda$ et $\mu$ deux éléments distincts de $\widehat{G}$ et soient $u\in$ End$_K(V_{\lambda})$ et $v\in$ End$_K(V_{\mu})$. À nouveau d’après la relation (15), on a

(23) $\sum_{g\in G}$ Tr($u\pi_{\lambda}(g)$) Tr($v\pi_{\mu}(g^{-1})$) $= 0$.

On en déduit comme plus haut

$$
\sum_{g\in G}\langle x^*, \pi_{\lambda}(g)x\rangle  \langle y^*, \pi_{\mu}(g^{-1})y\rangle = 0 \tag{24}
$$

pour $x\in V_{\lambda},x^*\in V^*_{\lambda},y\in V_{\mu}$ et $y^*\in V^*_{\mu}$; on a aussi

$$
\sum_{g\in G}\pi_{ij}^{\lambda}(g)\pi_{k\ell}^{\mu}(g^{-1}) = 0 \tag{25}
$$

pour $i, j$ dans $[1, d_{\lambda}]$ et $k, \ell$ dans $[1, d_{\mu}]$.

Les relations (20) à (25) sont connues sous le nom de relations d’orthogonalité de Schur.

#### Remarque {#alg-viii-s21-n6-rem-1 .statement tag=00NS}

Identifions l’algèbre End$_K(V_{\lambda})$ à l’algèbre de matrices $\mathbf{M}_{d_{\lambda}}(K)$ au moyen de la base $(e_{\lambda ,j})$ de $V_{\lambda}$. L’application $\overline{\mathscr{F}}^{-1}$ est un isomorphisme de l’algèbre $\prod_{\lambda}\mathbf{M}_{d_{\lambda}}(K)$ sur l’algèbre K[G]. Pour $\mu \in \widehat{G}$, notons $E^{\mu}_{ij}$ l’élément de $\prod_{\lambda}\mathbf{M}_{d_{\lambda}}(K)$ dont la composante d’indice $\mu$ est l’unité matricielle $E_{ij}$ de $\mathbf{M}_{d_{\mu}}(K)$ (II, p. 142) et dont les autres composantes sont nulles ; posons $u^{\mu}_{ij}=\overline{\mathscr{F}}^{-1}(E^{\mu}_{ij})$. La famille des éléments $u^{\lambda}_{ij}$, pour $\lambda \in \widehat{G}, 1\leqslant i\leqslant d_{\lambda}, 1\leqslant j\leqslant d_{\lambda}$, est une base de l’algèbre K[G] ; la table de multiplication est

$$
u^{\lambda}_{ij}u^{\mu}_{k\ell}=\delta_{\lambda \mu}\delta_{jk}u^{\lambda}_{i\ell} \tag{26}
$$

De plus, d’après la formule (15), on a

$$
u^{\lambda}_{ij}=|G|^{-1}d_{\lambda}\sum_{g\in G}\pi_{ji}^{\lambda}(g^{-1})g \tag{27}
$$

### 7. Relation d’orthogonalité des caractères

Conservons les notations des numéros 5 et 6. Rappelons que Z(K[G]) est formé des fonctions centrales.

On définit une application bilinéaire symétrique de $K[G]\times K[G]$ dans K par la formule

$$
\langle f, f'\rangle_G=|G|^{-1}\sum_{g\in G}f_gf'_{g_{-1}} \tag{28}
$$

pour tous $f=\sum f_gg$ et $f'=\sum f'_gg$ appartenant à K[G]. On a $\langle f, f'\rangle_G=|G|^{-2}\tau (f f')$.

#### Proposition 4 (Relation d’orthogonalité des caractères) {#alg-viii-s21-prop-4 .statement tag=00SG}

Pour $\lambda$ et $\mu$ dans $\widehat{G}$, on a $\langle \chi_{\lambda}, \chi_{\mu}\rangle_G=\delta_{\lambda \mu}$.

C’est le cas particulier des relations (20) et (23), où les endomorphismes $u$ et $v$ sont pris égaux à l’identité.

#### Corollaire {#alg-viii-s21-n7-cor-1 .statement tag=00NT}

Soient $\pi$ et $\pi '$ des représentations linéaires de dimension finie de G. On a, dans le corps K,

(29) $\langle \chi_{\pi}, \chi_{\pi'}\rangle_G=$ (dim$_K$ Hom$_G(\pi , \pi ')$)$.1$.

Supposons d’abord que $\pi$ et $\pi '$ soient des représentations simples. L’espace vectoriel Hom$_G(\pi , \pi ')$ est de dimension 1 ou 0 suivant que $\pi$ et $\pi '$ sont isomorphes ou non (lemme de Schur, VIII, p. 43, prop. 2). La formule (29) résulte dans ce cas de la proposition 4.

Dans le cas général, la représentation $\pi$ (resp. $\pi '$) est somme directe de représentations simples $\pi_1, . . . , \pi_m$ (resp. $\pi '_1, . . . , \pi '_n$). L’espace Hom$_G(\pi , \pi ')$ est isomorphe à la somme directe des espaces Hom$_G(\pi_i, \pi '_j)$, pour $1\leqslant i\leqslant m, 1\leqslant j\leqslant n$, et l’on a

$$
\chi_{\pi}=\chi_{\pi_1}+\cdots +\chi_{\pi_m},\chi_{\pi'}=\chi_{\pi'_1}+\cdots +\chi_{\pi'_n}
$$

Par linéarité, la démonstration de la formule (29) est ramenée au cas des représentations simples.

### 8. Fonctions centrales sur un groupe fini

#### Proposition 5 {#alg-viii-s21-prop-5 .statement tag=00NU}

La famille $(\chi_{\lambda})_{\lambda\in\widehat{G}}$ est une base de l’espace vectoriel des fonctions centrales. Le nombre de classes de représentations linéaires simples de G est égal au nombre de classes de conjugaison de G.

Pour $a=\sum_{g\in G}a_gg\in K[G]$, notons $a^{\vee}=\sum_{g\in G}a_{g^{-1}}g$; l’application $a\rightarrow a^{\vee}$ est un antiautomorphisme involutif de l’algèbre K[G]. D’après la formule (17), on a $e_{\lambda}=|G|^{-1}d_{\lambda}\chi^{\vee}_{\lambda}$ pour tout $\lambda \in \widehat{G}$. La proposition résulte alors de ce que la famille $(e_{\lambda})_{\lambda\in\widehat{G}}$ est une base du centre de K[G].

Notons $\mathscr{C}$ l’ensemble des classes de conjugaison de G. Soit C un élément de $\mathscr{C}$; l’image $C^{-1}$ de C par l’application $g\rightarrow g^{-1}$ est une classe de conjugaison. Les centralisateurs des éléments de C sont des sous-groupes de G conjugués entre eux ; leur cardinal $d(C)$ satisfait à

(30) Card(G) = Card(C) $d(C)$.

En particulier, on a $d(C).1\not= 0$ dans le corps K.

Soit $f$ une fonction centrale sur G. Pour toute classe de conjugaison C, notons $f(C)$ la valeur commune des $f(x)$ pour $x\in C$. Avec cette notation, la relation d’orthogonalité des caractères (VIII, p. 400, prop. 4) s’écrit

$$
\sum_{C\in\mathscr{C}}\chi_{\lambda}(C^{-1})\chi_{\mu}(C)d(C)^{-1}=\delta_{\lambda \mu} \tag{31}
$$

pour $\lambda$ et $\mu$ dans $\widehat{G}$.

Notons A la matrice de type $\widehat{G}\times \mathscr{C}$ d’éléments $\chi_{\lambda}(C)$ et B la matrice de type $\mathscr{C}\times \widehat{G}$, d’éléments $\chi_{\lambda}(C^{-1})d(C)^{-1}$. Les ensembles $\widehat{G}$ et $\mathscr{C}$ ont le même cardinal (prop. 5) ; la relation (31) exprime que la matrice produit AB est la matrice unité de type $\widehat{G}\times \widehat{G}$. D’après la prop. 11 de II, p. 159, la matrice produit BA est la matrice unité de type $\mathscr{C}\times \mathscr{C}$; autrement dit, on a la relation

$$
\sum_{\lambda\in\widehat{G}}\chi_{\lambda}(C^{-1})\chi_{\lambda}(C') =d(C)\delta_{CC'} \tag{32}
$$

pour C et $C'$ dans $\mathscr{C}$ (appelée parfois « seconde relation d’orthogonalité des caractères »).

Soit H un sous-groupe de G. Remarquons que l’entier Card(H) divise Card(G) et que $|G|$ n’est pas nul dans K ; on a donc $|H| \not= 0$ dans K.

Notons Res$^G_H$ l’application linéaire de Z(K[G]) dans Z(K[H]) qui associe à une fonction centrale sur G sa restriction à H. Si $\chi_{\pi}$ est le caractère d’une représentation de dimension finie $\pi$ de G, on a vu que Res$^G_H(\chi_{\pi})$ est le caractère de la représentation Res$^G_H(\pi )$ de H.

#### Proposition 6 {#alg-viii-s21-prop-6 .statement tag=00NV}

Soient $f$ une fonction centrale sur G et $u$ une fonction centrale sur H. On a

(33) $\langle$Ind$^G_H(u), f\rangle_G=\langle u$, Res$^G_H(f)\rangle_H$.

Les caractères des représentations simples de G forment une base de Z(K[G]) (VIII, p. 401, prop. 5) et il en est de même pour H. Il suffit donc d’établir (33) dans le cas où $f$ est le caractère $\chi_{\pi}$ d’une représentation simple $\pi$ de G et $u$ le caractère $\chi_{\sigma}$ d’une représentation simple $\sigma$ de H. Dans ce cas, Ind$^G_H(u)$ est le caractère de la représentation Ind$^G_H(\sigma )$ de G et, d’après VIII, p. 400, corollaire, on a

$\langle$Ind$^G_H(u), f\rangle_G=$ (dim$_K$ Hom$_G$(Ind$^G_H(\sigma ), \pi$ ))$.1$.

On établit de même la relation

$\langle u$, Res$^G_H(f)\rangle_H=$ (dim$_K$ Hom$_H(\sigma$, Res$^G_H(\pi )$))$.1$

et l’égalité (33) résulte de la réciprocité de Frobenius.

#### Proposition 7 {#alg-viii-s21-prop-7 .statement tag=00NW}

Soit $f$ une application de G dans K. Les assertions suivantes sont équivalentes :

(i) Il existe un élément $\lambda$ de $\widehat{G}$ et un élément $a$ de K tels que $f=a\chi_{\lambda}$;

(ii) Pour tout couple $(g, g')$d’éléments de G, on a

$$
f(g)f(g') =|G|^{-1}f(1)\sum_{h\in G}f(hgh^{-1}g') \tag{34}
$$

Soit $\lambda$ un élément de $\widehat{G}$; pour tout endomorphisme $u$ de $V_{\lambda}$, posons

$$
u^{\natural}=|G|^{-1}\sum_{h\in G}\pi_{\lambda}(h)u \pi_{\lambda}(h^{-1}) \tag{35}
$$

L’endomorphisme $u^{\natural}$ de $V_{\lambda}$ est K[G]-linéaire ; d’après le lemme de Schur (VIII, p. 43, th. 1)$,u^{\natural}$ est une homothétie ; comme $u$ et $u^{\natural}$ ont la même trace, on a donc

$u^{\natural}=d^{-1}_{\lambda}$ Tr($u$) $1_{V_{\lambda}}$.

Soient $u$ et $v$ des endomorphismes de $V_{\lambda}$; on en déduit

(36) Tr($u$) Tr($v$) $=d_{\lambda}$ Tr($u^{\natural}v$) $=d_{\lambda}|G|^{-1}\sum_{h\in G}$ Tr($\pi_{\lambda}(h)u \pi_{\lambda}(h^{-1})v$).

Prenons $u=\pi_{\lambda}(g),v=\pi_{\lambda}(g')$ dans la formule (36) ; la relation (34) pour $f=\chi_{\lambda}$ en résulte.

Inversement, supposons la condition (ii) satisfaite. Si l’on a $f(1) = 0$, on en déduit $f(g)f(g') = 0$ pour tout couple $(g, g')$ d’éléments de G, d’où $f= 0$. On peut donc supposer $f(1)\not= 0$. Prenons $g'= 1$ dans (34), on obtient la relation

$$
f(g) =|G|^{-1}\sum_{h\in G}f(hgh^{-1})
$$

pour tout $g\in G$, ce qui entraîne que $f$ est une fonction centrale. D’après la proposition 5, il existe une famille $(a_{\lambda})$ d’éléments de K telle que $f=\sum_{\lambda\in\widehat{G}}a_{\lambda}\chi_{\lambda}$. Remplaçons $f$ par cette expression dans la formule (34) ; tenant compte de ce que chacun des caractères $\chi_{\lambda}$ satisfait aussi à cette relation, on trouve

$$
\sum_{\lambda ,\mu\in\widehat{G}}a_{\lambda}a_{\mu}\chi_{\lambda}(g)\chi_{\mu}(g') =\sum_{\lambda\in\widehat{G}}a_{\lambda}d^{-1}_{\lambda}f(1)\chi_{\lambda}(g)\chi_{\lambda}(g') \tag{37}
$$

pour $g, g'\in G$. La relation précédente s’écrit également

$$
\sum_{\lambda ,\mu}(a_{\lambda}a_{\mu}-\delta_{\lambda \mu}a_{\lambda}d^{-1}_{\lambda}f(1))\chi_{\lambda}(g)\chi_{\mu}(g') = 0 \tag{38}
$$

pour $g, g'\in G$. Or les fonctions $\chi_{\lambda}$, pour $\lambda \in \widehat{G}$, sont linéairement indépendantes (prop. 5 de VIII, p. 401) ; on en déduit que

$$
a_{\lambda}a_{\mu}=\delta_{\lambda \mu}a_{\lambda}d^{-1}_{\lambda}f(1)
$$

pour $\lambda , \mu \in \widehat{G}$. En particulier, $a_{\lambda}a_{\mu}= 0$ dès que $\lambda \not=\mu$. Par suite, il existe au plus un élément $\lambda$ de $\widehat{G}$ tel que $a_{\lambda}\not= 0$ et l’on a $f=a_{\lambda}\chi_{\lambda}$, d’où (i).

### 9. Cas des groupes commutatifs

Dans ce numéro, on suppose que le groupe G est commutatif.

D’après le lemme de Schur (VIII, p. 44, cor. 1), toute représentation simple de G est de dimension 1. Soient $(M, \pi )$ une telle représentation et $\chi$ son caractère ; pour tout $g\in G$ et tout $x\in M$, on a $\pi (g)(x) =\chi (g)x$. Par suite, le caractère $\chi$ est un homomorphisme de G dans le groupe multiplicatif $K^*$ de K. Inversement, tout homomorphisme de G dans $K^*$ est le caractère d’une représentation de degré 1 de G. Ainsi l’ensemble $\widehat{G}$ des classes de K[G]-modules simples s’identifie à l’ensemble Hom(G$,K^*$) des homomorphismes de G dans $K^*$. On en déduit une structure de groupe commutatif sur $\widehat{G}$; le produit dans $\widehat{G}$ correspond au produit tensoriel des représentations. Les groupes G et $\widehat{G}$ ont même cardinal d’après la prop. 5 de VIII, p. 401. Toute fonction sur G est centrale et $\widehat{G}$ est une base de l’espace vectoriel des applications de G dans K (loc. cit.). En vertu de la relation d’orthogonalité des caractères, une telle application $f$ se décompose sur la base $\widehat{G}$ de la manière suivante :

$$
f=\sum_{\chi\in\widehat{G}}\langle \chi , f\rangle_G\chi \tag{39}
$$

Pour des applications $f$ et $f'$ de G dans K, on a la relation

$$
\langle f, f'\rangle_G=\sum_{\chi\in\widehat{G}}\langle \chi , f\rangle_G\langle \chi , f'\rangle_G \tag{40}
$$

Soit $(V, \pi )$ une représentation linéaire de G. Pour tout $\chi \in \widehat{G}$, notons $V^{\chi}$ le sous-espace de V formé des vecteurs $v$ tels que $\pi (g)(v) =\chi (g)v$ pour tout $g\in G$; l’espace $V^{\chi}$ est le composant isotypique de type $\chi$ du K[G]-module V. L’espace V est somme directe de la famille $(V^{\chi})_{\chi\in\widehat{G}}$ et le projecteur $p_{\chi}$ de V d’image $V^{\chi}$ associé à cette décomposition est donné par

$$
p_{\chi}=|G|^{-1}\sum_{g\in G}\chi (g^{-1})\pi (g) \tag{41}
$$

en vertu de la relation (19).

#### Remarque {#alg-viii-s21-n9-rem-1 .statement tag=00NX}

Soit $n$ le cardinal du groupe G et soit $\mu_n(K)$ le groupe des racines $n$-èmes de l’unité dans K. Pour tout $g\in G$, on a $g^n= 1$; par suite, $\widehat{G}$ s’identifie au groupe Hom(G$, \mu_n(K)$). Le groupe $\mu_n(K)$ est cyclique d’ordre $n$ (V, p. 75, th. 1). Le groupe $\widehat{G}$ est donc isomorphe au groupe D(G) = Hom(G$,\mathbf{Q}/\mathbf{Z}$). D’après VII, p. 25, prop. 10, le groupe $\widehat{G}$ est isomorphe au groupe G et l’application qui, à tout élément $g$ de G, associe l’homomorphisme $\chi \rightarrow \chi (g)$ de $\widehat{G}$ dans $K^*$ est un isomorphisme de G sur $\widehat{G}$.

### 10. Caractères et groupes de Grothendieck

Notons $\theta_G$ l’homomorphisme de K-algèbres de $K\otimes_{\mathbf{Z}}R_K(G)$ dans $\mathscr{Z}_K(G)$ qui transforme $1\otimes [\pi ]$ en $\chi_{\pi}$ pour toute représentation $\pi$ de dimension finie.

#### Proposition 8 {#alg-viii-s21-prop-8 .statement tag=00NY}

a) L’homomorphisme $\theta_G$ est un isomorphisme de $K\otimes_{\mathbf{Z}}R_K(G)$ sur $\mathscr{Z}_K(G)$.

b) Supposons K de caractéristique 0. Alors $\Theta_G$ définit un isomorphisme de $R_K(G)$sur le sous-anneau de $\mathscr{Z}_K(G)$formé des combinaisons linéaires à coefficients entiers des caractères $\chi_{\lambda}$, pour $\lambda$ parcourant $\widehat{G}$.

La famille $([\lambda ])_{\lambda\in\widehat{G}}$ est une base du $\mathbf{Z}$-module $R_K(G)$ et la famille $(\chi_{\lambda})_{\lambda\in\widehat{G}}$ est une base du K-espace vectoriel $\mathscr{Z}_K(G)$. Les assertions a) et b) en résultent (VIII, p. 401, prop. 5).

### 11. Dimension des représentations simples

Notons $n$ le cardinal du groupe G. Soit $\pi$ une représentation linéaire de G dans un K-espace vectoriel M de dimension finie. Pour tout $g\in G$, on a $\pi (g)^n= 1_M$, donc le polynôme minimal de $\pi (g)$ divise $T^n-1$. Comme $n.1\not= 0$ dans K, ce polynôme minimal est séparable (V, p. 75), et comme le corps K est algébriquement clos, l’endomorphisme $\pi (g)$ de M est diagonalisable (VII, p. 39, prop. 12). Les valeurs propres de $\pi (g)$ sont des racines $n$-èmes de l’unité et, pour tout $\alpha \in K$, la multiplicité géométrique de $\alpha$ comme valeur propre de $\pi (g)$ (VII, p. 29, déf. 1) est égale à la multiplicité de $\alpha$ comme racine du polynôme caractéristique de $\pi (g)$. Notons $\mathscr{O}_n$ le sous-groupe de K engendré par l’ensemble $\mu_n(K)$ des racines $n$-èmes de l’unité ; c’est un $\mathbf{Z}$-module de type fini et un sous-anneau de K. Le caractère de $\pi$ prend ses valeurs dans $\mathscr{O}_n$.

#### Proposition 9 {#alg-viii-s21-prop-9 .statement tag=00NZ}

Supposons le corps K de caractéristique nulle. Alors le degré de toute représentation simple de G divise le cardinal de G.

Soient $(V, \pi )$ une représentation simple de G et $\chi$ son caractère. Pour tout élément $a$ de Z(K[G]), l’endomorphisme $\pi (a)$ de V est une homothétie (VIII, p. 43, th. 1) ; notons $\varphi (a)$ le scalaire tel que $\pi (a) =\varphi (a)_V$. L’application $\varphi$ de Z(K[G]) dans K ainsi définie est un homomorphisme d’algèbres. Prenons $a=\sum_{g\in G}\chi (g^{-1})g$; d’après la remarque de VIII, p. 398, on a $\varphi (a) =$ (dim $V$)$^{-1}|G|$. D’autre part $a$ appartient au sous-anneau $\mathscr{O}_n[G]\cap Z(K[G])$ de K[G], qui est un $\mathbf{Z}$-module de type fini (VII, p. 15, cor.). Ainsi l’élément $\varphi (a) =$ (dim $V$)$^{-1}|G|$ de K appartient à un sous-anneau de K qui est un $\mathbf{Z}$-module de type fini. On conclut à l’aide du lemme suivant :

#### Lemme {#alg-viii-s21-n11-lem-1 .statement tag=00O0}

Soit L une extension de $\mathbf{Q}$. Soit A un sous-anneau de L. On suppose que A est un $\mathbf{Z}$-module de type fini. On a $A\cap \mathbf{Q} = \mathbf{Z}$.

Comme le $\mathbf{Z}$-module $A\cap \mathbf{Q}$est de type fini, il existe un entier N strictement positif tel que $A\cap \mathbf{Q}$soit contenu dans $\frac{1}{N}\mathbf{Z}$. Soit $x$ un élément de $\mathbf{Q}-\mathbf{Z}$; écrivons $x=\frac{p}{q}$, où $p$ et $q$ sont des entiers premiers entre eux et $q\geqslant 2$. On a $q^N\geqslant 2^N>N$ (E, III, p. 30, th. 2), les entiers $p^N$ et $q^N$ sont premiers entre eux et par suite $x^N\in /\frac{1}{N}\mathbf{Z}$. Par conséquent $x$ n’appartient pas à A, d’où le lemme.

Nous étendrons au numéro suivant la proposition 9 au cas où l’on suppose seulement que la caractéristique de K ne divise pas l’ordre de G.

### 12. Changement de corps de base

Conservons les notations du numéro précédent. Soit $K'$ un corps algébriquement clos tel que l’élément $n.1$ de $K'$ ne soit pas nul. Les groupes $\mu_n(K)$ et $\mu_n(K')$ sont cycliques d’ordre $n$ (V, p. 75, th. 1). Choisissons un isomorphisme $\varphi$ de $\mu_n(K)$ sur $\mu_n(K')$. Soit $\pi$ une représentation linéaire de G dans un K-espace vectoriel de dimension finie et soit $\pi '$ une représentation linéaire de G dans un $K'$-espace vectoriel de dimension finie. On dira que $\pi$ et $\pi '$ sont apparentées (par $\varphi$ ) si pour tout $g\in G$ et tout $\omega \in \mu_n$(K), la multiplicité de $\omega$ comme valeur propre de $\pi (g)$ est égale à la multiplicité de $\varphi (\omega )$ comme valeur propre de $\pi '(g)$. S’il en est ainsi, $\pi$ et $\pi '$ ont même dimension, comme on le voit en prenant $g= 1$.

Soient $\pi_1$ et $\pi_2$ (resp. $\pi '_1$ et $\pi '_2$) des représentations linéaires de G dans des espaces vectoriels de dimension finie sur K (resp. $K'$). On a les propriétés suivantes :

a) Si $\pi_1$ est apparentée à $\pi '_1$ et $\pi '_2$, alors $\pi '_1$ et $\pi '_2$ sont isomorphes ;

b) Si $\pi_1$ est apparentée à $\pi '_1$, et $\pi_2$ à $\pi '_2$, alors $\pi_1\oplus \pi_2$ est apparentée à $\pi '_1\oplus \pi '_2$, et $\pi_1\otimes \pi_2$ est apparentée à $\pi '_1\otimes \pi '_2$.

L’assertion a) résulte du cor. 5 de VIII, p. 392 et l’assertion b) est claire.

On note ici $\mathscr{S}_K(G)$ l’ensemble des classes de K[G]-modules simples, noté précédemment $\widehat{G}$ et on définit $\mathscr{S}_{K'}(G)$ de manière analogue. Les ensembles $\mathscr{S}_K(G)$ et $\mathscr{S}_{K'}(G)$ sont tous deux finis, de cardinal le nombre de clases de conjugaison (VIII, p. 401, prop. 5).

#### Proposition 10 {#alg-viii-s21-prop-10 .statement tag=00O1}

Il existe une unique application $\varphi_G$ de $\mathscr{S}_K(G)$dans $\mathscr{S}_{K'}(G)$ telle que $\lambda$ et $\varphi_G(\lambda )$soient apparentées par $\varphi$ pour tout $\lambda$ dans $\mathscr{S}_K(G)$. De plus, $\varphi_G$ est bijective.

L’unicité de $\varphi_G$ résulte de la propriété a) ci-dessus.

A) Supposons le corps K de caractéristique 0.

Le groupe $\mu_n(K)$ est cyclique (V, p. 75, th. 1) ; choisissons un générateur $\zeta$ de ce groupe. Considérons l’homomorphisme d’anneaux $\rho : \mathbf{Z}[X]\rightarrow \mathscr{O}_n$ qui applique X sur $\zeta$. Il est surjectif. Le polynôme cyclotomique $\Phi_n(X)$ est irréductible dans $\mathbf{Q}[X]$ (V, p. 80, th. 2) ; c’est donc le polynôme minimal de $\zeta$ sur $\mathbf{Q}$. Le polynôme $\Phi_n$ est un polynôme unitaire à coefficients entiers (V, p. 78). Soit $P\in \mathbf{Z}[X]$ un polynôme tel que $P(\zeta ) = 0$; d’après la division euclidienne des polynômes (IV, p. 10), il existe deux polynômes Q et R de $\mathbf{Z}[X]$ tels que P = QΦ$_n+ R$ et deg(R) $<$ deg(Φ$_n$). On a $R(\zeta ) = 0$, donc R = 0 puisque $\Phi_n$ est le polynôme minimal de $\zeta$. Par conséquent, le noyau de $\rho$ est l’idéal $\Phi_n\mathbf{Z}[X]$ de $\mathbf{Z}[X]$ et $\rho$ induit un isomorphisme d’anneaux de $\mathbf{Z}[X]/\Phi_n\mathbf{Z}[X]$ sur $\mathscr{O}_n$.

Posons $\zeta '=\varphi (\zeta )$; c’est une racine primitive $n$-ème de l’unité dans $K'$, et l’on a donc $\Phi_n(\zeta ') = 0$ (V, p. 80, lemme 3). Par suite, il existe un homomorphisme $\varphi_0$ de l’anneau $\mathscr{O}_n$ dans le corps $K'$ qui transforme $\zeta$ en $\zeta '$; il prolonge l’application $\varphi$ de $\mu_n(K)$ dans $\mu_n(K')$. Soit $\mathscr{O}$ le sous-anneau de K formé des éléments $\frac{a}{n^r}$ avec $a\in \mathscr{O}_n$ et $r\in \mathbf{N}$. Comme $n.1$ est inversible dans $K'$, l’homomorphisme $\varphi_0$ se prolonge en un homomorphisme $\varphi_1$ de $\mathscr{O}$ dans $K'$.

Identifions l’algèbre $\mathscr{O}[G]$ du groupe G sur $\mathscr{O}$ à un sous-anneau de l’algèbre K[G], et définissons un homomorphisme d’anneaux Φ de $\mathscr{O}[G]$ dans $K'[G]$ par la formule

$$
\Phi (\sum_{g\in G}a_gg)=\sum_{g\in G}\varphi_1(a_g)g \tag{42}
$$

Notons $\mathscr{C}$ l’ensemble des classes de conjugaison de G. Pour C dans $\mathscr{C}$, notons $u_C$ l’élément $\sum_{g\in C}g$ de $\mathscr{O}[G]$; la famille $(u_C)_{C\in\mathscr{C}}$ est une base sur $\mathscr{O}$ du centre $Z(\mathscr{O}[G])$ de l’algèbre $\mathscr{O}[G]$ (VIII, p. 388). Pour tout élément $\lambda$ de $\mathscr{S}_K$(G), notons $\chi_{\lambda}$ son caractère, $d_{\lambda}$ sa dimension et $e_{\lambda}$ l’élément de K[G] défini par

$$
e_{\lambda}=|G|^{-1}d_{\lambda}\sum_{g\in G}\chi_{\lambda}(g^{-1})g \tag{43}
$$

La famille $(e_{\lambda})$ est une base sur K du centre Z(K[G]) de l’anneau K[G] (VIII, p. 398). On a

$$
e_{\lambda}=\sum_{C\in\mathscr{C}}\alpha_{\lambda ,C}u_C \tag{44}
$$

avec

$$
\alpha_{\lambda ,C}=|G|^{-1}d_{\lambda}\chi_{\lambda}(C^{-1}) \tag{45}
$$

Pour $C\in \mathscr{C}$ et $\lambda \in \mathscr{S}_K$(G), posons $\beta_{C,\lambda}=|G|d^{-1}_{\lambda}d(C)^{-1}\chi_{\lambda}(C)$. La matrice $(\alpha_{\lambda ,C})$ a ses éléments dans $\mathscr{O}$ et il résulte de la formule (31) de VIII, p. 401 que sa matrice inverse est la matrice $(\beta_{C,\lambda})$, qui a aussi ses éléments dans $\mathscr{O}$ en vertu de la prop. 9 de VIII, p. 405. Par conséquent, la famille $(e_{\lambda})$ est une base du $\mathscr{O}$-module $Z(\mathscr{O}[G])$.

Les éléments $\Phi (u_C) =\sum_{g\in C}g$ de $K'[G]$ forment une base sur $K'$ du centre $Z(K'[G])$ de l’anneau $K'[G]$. On a

$$
\Phi (e_{\lambda}) =\sum_{C\in\mathscr{C}}\varphi_1(\alpha_{\lambda ,C}) \Phi (u_C) \tag{46}
$$

et la matrice d’éléments $\varphi_1(\alpha_{\lambda ,C})$ est inversible. La famille des $\Phi (e_{\lambda})$ est donc une base de $Z(K'[G])$. La famille $(e_{\lambda})$ est une partition de l’idempotent 1 dans Z(K[G]) (VIII, p. 141 et p. 398) ; autrement dit, on a

$\sum_{\lambda}e_{\lambda}= 1,e^2_{\lambda}=e_{\lambda},e_{\lambda}e_{\mu}= 0$ si $\lambda \not=\mu$.

Il en résulte que la famille des $\Phi (e_{\lambda})$ est une partition de l’idempotent 1 dans $Z(K'[G])$; comme cette famille est une base de $Z(K'[G])$ sur $K'$, ses éléments sont les idempotents indécomposables de $Z(K'[G])$ (VIII, p. 143, remarque 4).

Pour $\lambda '$ dans $\mathscr{S}_{K'}$(G), définissons comme ci-dessus $\chi_{\lambda'},d_{\lambda'}$ et $e_{\lambda'}$. D’après VIII, p. 398, les éléments $e_{\lambda'}$ sont les idempotents indécomposables de $Z(K'[G])$. Il existe donc une bijection $\varphi_G$ de $\mathscr{S}_K(G)$ sur $\mathscr{S}_{K'}(G)$ telle que $\Phi (e_{\lambda}) =e_{\varphi_G(\lambda)}$ pour tout $\lambda$ dans $\mathscr{S}_K(G)$.

Soit $\lambda$ dans $\mathscr{S}_K(G)$; posons $\lambda '=\varphi_G(\lambda )$. Soit $(V_{\lambda}, \pi_{\lambda})$ (resp. $(V_{\lambda'}, \pi_{\lambda'})$) une représentation linéaire de G dont le K[G]-module (resp. $K'$[G]-module) associé soit de classe $\lambda$ (resp. $\lambda '$). Démontrons que $\lambda$ et $\lambda '$ sont apparentées. Soit $g$ un élément de G. Soit $\delta (T)$ le déterminant de l’endomorphisme $1 + T\pi_{\lambda}(g)$ du K[T]-module $K[T]\otimes_KV_{\lambda}$. Soient $\omega_1, . . . , \omega_{d_{\lambda}}$ les valeurs propres de $\pi_{\lambda}(g)$; on a

$$
\delta (T) = (1 + T\omega_1). . .(1 + T\omega_{d_{\lambda}})
$$

On définit de même $\delta '(T)$ et on note $\omega '_1, . . . , \omega '_{d_{\lambda'}}$ les valeurs propres de $\pi_{\lambda'}(g)$. Le $\mathscr{O}$-module $\mathscr{O}[G]$ est libre de base G et le K-espace vectoriel K[G] a pour base G. Notons Δ(T) le déterminant de la multiplication par $1 +e_{\lambda}gT$ dans le $\mathscr{O}$[T]-module $\mathscr{O}[T]\otimes_{\mathscr{O}}\mathscr{O}[G]$. C’est aussi le déterminant de la multiplication par $1 +e_{\lambda}gT$ dans le K[T]-module $K[T]\otimes_KK[G]$. Soit $\overline{\varphi}_1$ l’homomorphisme de $\mathscr{O}[T]$ dans $K'[T]$ qui prolonge $\varphi_1$ et applique T sur T. Comme G est une base du $K'$-espace vectoriel $K'[G]$, le polynôme $\overline{\varphi}_1(\Delta (T))$ est égal au déterminant $\Delta '(T)$ de la multiplication par $1 +e_{\lambda'}gT$ dans le $K'$-espace vectoriel $K'[G]$.

L’algèbre K[G] est somme directe de ses composants simples $e_{\mu}K[G]$ pour $\mu$ parcourant $\mathscr{S}_K(G)$. Pour $\mu$ distinct de $\lambda$, l’élément $e_{\lambda}g$ annule $e_{\mu}K[G]$; de plus, la multiplication par $e_{\lambda}g$ coïncide avec la multiplication par $g$ dans $e_{\lambda}K[G]$. Compte tenu de VIII, p. 398 et de l’exemple 6 de VIII, p. 390, la représentation de G dans $e_{\lambda}K[G]$ est somme directe de $d_{\lambda}$ représentations de classe $\lambda$. On a par suite $\Delta (T) =\delta (T)^{d_{\lambda}}$.

De manière analogue, on a $\Delta '(T) =\delta '(T)^{d_{\lambda'}}$.

De la relation $\Delta '(T) =\overline{\varphi}_1$(Δ(T)), on déduit d’abord que $d^2_{\lambda}=d^2_{\lambda'}$, d’où $d_{\lambda}=d_{\lambda'}$ puis le fait que la suite $\varphi (\omega_1), . . . , \varphi (\omega_{d_{\lambda}})$ se déduit de la suite $(\omega '_1, . . . , \omega '_{d'_{\lambda'}})$ par une permutation de l’ensemble des indices.

Ceci étant prouvé pour tout élément $g$ de G, les représentations $\lambda$ et $\lambda '$ sont apparentées. On a donc prouvé la proposition 10 lorsque le corps K est de caractéristique 0.

B) Cas général.

Soit L un corps algébriquement clos de caractéristique 0 (par exemple, une clôture algébrique de $\mathbf{Q}$). Notons $\mathscr{S}_L(G)$ l’ensemble des classes de L[G]-modules simples. Choisissons un isomorphisme $\eta$ du groupe $\mu_n(L)$ sur le groupe $\mu_n(K)$ et posons $\eta '=\varphi \circ \eta$. D’après la partie A) de la démonstration, il existe des bijections

$$
\eta_G:\mathscr{S}_L(G)\rightarrow \mathscr{S}_K(G), \eta '_G:\mathscr{S}_L(G)\rightarrow \mathscr{S}_{K'}(G)
$$

possédant la propriété suivante : pour tout $\lambda$ dans $\mathscr{S}_L$(G), les représentations $\lambda$ et $\eta_G(\lambda )$ sont apparentées par $\eta$, et les représentations $\lambda$ et $\eta '_G(\lambda )$ sont apparentées par $\eta '$. La bijection $\varphi_G=\eta '_G\circ \eta_G^{-1}$ convient.

La bijection $\varphi_G$ de $\mathscr{S}_K(G)$ sur $\mathscr{S}_{K'}(G)$ se prolonge en un isomorphisme, encore noté $\varphi_G$, du groupe de Grothendieck $R_K(G)$ sur le groupe $R_{K'}(G)$.

#### Remarque 1 {#alg-viii-s21-n12-rem-1 .statement tag=00O2}

Supposons que $K'$ soit une extension de K et que l’isomorphisme $\varphi$ soit l’application $\xi \rightarrow \xi .1$, alors l’application $\varphi_G$ est donnée par l’extension des scalaires de K à $K'$.

#### Corollaire 1 {#alg-viii-s21-prop-10-cor-1 .statement tag=00O3}

L’application $\varphi_G$ est un isomorphisme d’anneaux de $R_K(G)$sur $R_{K'}(G)$. Pour toute représentation $\pi$ de dimension finie de G dans un K-espace vectoriel, on a $\varphi_G([\pi ]) = [\pi ']$, où $\pi '$ est une représentation apparentée à $\pi$ par $\varphi$.

Cela résulte de la semi-simplicité des représentations de G et de la propriété b) de VIII, p. 406.

#### Corollaire 2 {#alg-viii-s21-prop-10-cor-2 .statement tag=00O4}

La dimension de toute représentation simple de G divise l’ordre de G.

Cela résulte de la prop. 10 et de la prop. 9 de VIII, p. 405.

#### Remarque 2 {#alg-viii-s21-n12-rem-2 .statement tag=00O5}

Supposons le groupe G commutatif. On a vu dans la remarque de VIII, p. 404 que $\mathscr{S}_K(G)$ s’identifie à l’ensemble Hom(G$, \mu_n(K)$). De manière analogue, $\mathscr{S}_{K'}(G)$ s’identifie à Hom(G$, \mu_n(K')$). Avec ces identifications, la bijection $\varphi_G$ n’est autre que l’application $\chi \rightarrow \varphi \circ \chi$.

#### Remarque 3 {#alg-viii-s21-n12-rem-3 .statement tag=00O6}

Soient $\pi_1$ et $\pi_2$ des représentations linéaires de G dans des espaces vectoriels de dimension finie sur K. Pour $i= 1,2$, soit $\pi '_i$ une représentation apparentée à $\pi_i$ par $\varphi$. On a

(47) dim$_K$ Hom$_K(\pi_1, \pi_2) =$ dim$_{K'}$ Hom$_{K'}(\pi '_1, \pi '_2)$.

Cela se démontre comme dans le corollaire de VIII, p. 400 par réduction au cas où les $\pi_i$ (et donc les $\pi '_i$) sont simples.

#### Remarque 4 {#alg-viii-s21-n12-rem-4 .statement tag=00O7}

Soit H un sous-groupe de G de cardinal $m$. L’isomorphisme $\varphi$ induit par passage aux sous-ensembles un isomorphisme de $\mu_m(K)$ sur $\mu_m(K')$ et, par conséquent, un isomorphisme d’anneaux $\varphi_H$ de $R_K(H)$ sur $R_{K'}(H)$ Les diagrammes suivants sont commutatifs :

$R_K(G)^{Res^G_H}/$/ $R_K(H)R_K(H)^{Ind^G_H}/$/ $R_K(G)$

$\varphi_G\varphi_H\varphi_H\varphi_G$

$R_{K'}(G)^{Res^G_H}/$/ $R_{K'}(H)R_{K'}(H)^{Ind^G_H}/$/ $R_{K'}(G)$.

La commutativité du premier diagramme est évidente et celle du deuxième s’en déduit à l’aide de la réciprocité de Frobenius et de la formule (47).

#### Remarque 5 {#alg-viii-s21-n12-rem-5 .statement tag=00O8}

Supposons que G soit le produit $G'\times G''$ de deux groupes finis. On définit, comme dans l’exemple précédent des isomorphismes $\varphi_{G'}$ et $\varphi_{G''}$. On a alors un diagramme commutatif

$R_K(G')\otimes_{\mathbf{Z}}R_K(G'')^{\kappa}$ // $R_K(G)$

$\varphi_{G'}\otimes \varphi_{G''}\varphi_G$

$R_{K'}(G')\otimes_{\mathbf{Z}}R_{K'}(G'')^{\kappa'}$ // $R_{K'}(G)$,

où les isomorphismes $\kappa$ et $\kappa '$ sont ceux définis en VIII, p. 396.

### \*13. Représentations linéaires complexes

Dans ce numéro, on suppose que K est le corps $\mathbf{C}$des nombres complexes.

Soit $(M, \pi )$ une représentation linéaire de G. On dit qu’une forme hermitienne Φ sur M est invariante par G si l’on a

$$
\Phi (\pi (g)x, \pi (g)x') = \Phi (x, x') \tag{48}
$$

pour tous $x, x'\in M$ et tout $g\in G$. Cela signifie aussi que pour tout $g\in G$ l’automorphisme $\pi (g)$ de M est unitaire par rapport à Φ.

#### Proposition 11 {#alg-viii-s21-prop-11 .statement tag=00O9}

Soit $(M, \pi )$une représentation linéaire de G, de dimension finie.

a) Il existe sur M une forme hermitienne, positive, séparante et invariante par G.

b) Supposons la représentation $\pi$ simple ; si Φ et Ψ sont des formes hermitiennes non nulles sur M, invariantes par G, il existe un nombre réel $a$ tel que $\Psi  =a\Phi$.

Sur l’espace vectoriel M, choisissons une forme hermitienne, positive et séparante, notée $\Phi_0$. On définit une forme hermitienne Φ, positive, séparante et invariante par G en posant

$$
\Phi (x, x') =\sum_{g\in G}\Phi_0(\pi (g)x, \pi (g)x') \tag{49}
$$

pour $x, x'\in M$.

Soit Ψ une forme hermitienne sur M ; il existe un unique endomorphisme A de M tel que $\Psi (x, x') = \Phi (x,Ax')$ pour $x, x'$ dans M. Si, de plus, Ψ est invariante par G, l’endomorphisme A commute aux automorphismes $\pi (g)$ pour $g\in G$. Si la représentation $\pi$ est simple, d’après le lemme de Schur (VIII, p. 43, th. 1), A est une homothétie et il existe donc un nombre complexe $a$ tel que $\Psi  =a\Phi$. Comme Φ et Ψ sont hermitiennes et Φ non nulle, $a$ est un nombre réel, d’où la proposition.

On munit l’espace vectoriel $\mathbf{C}[G]$ des fonctions complexes sur G de la structure d’espace hilbertien dont le produit scalaire est donné par

$$
\langle f|f'\rangle_G=|G|^{-1}\sum_{g\in G}\overline{f(g)}f'(g) \tag{50}
$$

Pour toute fonction $f\in \mathbf{C}[G]$, on note $f^*$ la fonction définie par

$$
f^*(g) =\overline{f(g^{-1})} \tag{51}
$$

pour $g\in G$; on a $(f^*)^*=f$. On a aussi

$$
\langle f|f'\rangle_G=\langle f^*, f'\rangle_G \tag{52}
$$

pour $f, f'\in \mathbf{C}[G]$, avec les notations de la formule (28) de VIII, p. 400. On a donc

$$
\langle f|f'\rangle_G=|G|^{-2}\tau (f^*f') \tag{53}
$$

Soit $(M, \pi )$ une représentation linéaire de G, de dimension finie. Munissons l’espace vectoriel M d’une structure d’espace hilbertien pour laquelle les endomorphismes $\pi (g)$ sont unitaires (prop. 11). Si l’on note $A^*$ l’adjoint d’un endomorphisme A de M pour cette structure, on a Tr(A$^*$) $=$ Tr(A). Pour tout $g\in G$, on a $\pi (g^{-1}) =\pi (g)^*$ d’où $\chi_{\pi}(g^{-1}) =\chi_{\pi}(g)$; autrement dit, on a $\chi_{\pi}=\chi^*_{\pi}$. La relation d’orthogonalité des caractères (VIII, p. 400, prop. 4) prend alors la forme

$$
\langle \chi_{\lambda}|\chi_{\mu}\rangle_G=\delta_{\lambda \mu} \tag{54}
$$

pour $\lambda , \mu \in \widehat{G}$; elle exprime que la famille des caractères $(\chi_{\lambda})_{\lambda\in\widehat{G}}$ des représentations simples de G est une base orthonormale de l’espace hilbertien $Z(\mathbf{C}[G])$des fonctions centrales.

Soient $\pi$ et $\pi '$ des représentations linéaires de G, de dimension finie. On a la relation $\langle \chi_{\pi}|\chi_{\pi'}\rangle_G=$ dim$_{\mathbf{C}}$ Hom$_G(\pi , \pi ')$ (VIII, p. 400, cor.). La représentation $\pi$ est irréductible si et seulement si $\langle \chi_{\pi}|\chi_{\pi}\rangle_G= 1$.

Pour tout élément $\lambda$ de $\widehat{G}$, munissons l’espace vectoriel $V_{\lambda}$ d’une structure d’espace hilbertien pour laquelle les automorphismes $\pi_{\lambda}(g)$ soient unitaires, et notons $\langle v|v'\rangle_{\lambda}$ le produit scalaire de deux éléments $v, v'$ de $V_{\lambda}$ et $u^*$ l’adjoint d’un endomorphisme $u$ de $V_{\lambda}$. Soient $A = (A_{\lambda})_{\lambda\in\widehat{G}}$ et $A'= (A'_{\lambda})_{\lambda\in\widehat{G}}$ des éléments de $F(\widehat{G})$. Notons $A^*= (A^*_{\lambda})_{\lambda\in\widehat{G}}$. On a $\mathscr{F}(a^*) = (\overline{\mathscr{F}}(a))^*$ pour tout élément $a$ de $\mathbf{C}[G]$. Posons

$$
\langle A|A'\rangle_{\widehat{G}}=|G|^{-2}\widehat{\tau}(A^*A') \tag{55}
$$

D’après la formule (10) de VIII, p. 397, on a

(56) $\langle A|A'\rangle_{\widehat{G}}=\frac{1}{||^2}\sum d_{\lambda}$ Tr(A$^*_{\lambda}A'_{\lambda}$).

G $_{\lambda\in\widehat{G}}$

Comme $\widehat{\tau}\circ \overline{\mathscr{F}}=\tau$ les formules (53) et (55) entraînent que l’application $\overline{\mathscr{F}}$ est un isomorphisme d’espaces hilbertiens de $\mathbf{C}[G]$ sur $F(\widehat{G})$.

Les relations d’orthogonalité de Schur (VIII, p. 399) peuvent être reformulées à l’aide des produits scalaires hilbertiens. Ainsi, les relations (21) et (24) donnent les assertions suivantes. Pour $\lambda \in \widehat{G}$ et pour $x, x', y, y'$ dans $V_{\lambda}$, on a

$$
|G|^{-1}\sum_{g\in G}\overline{\langle x|\pi_{\lambda}(g) x'\rangle_{\lambda}}\langle y|\pi_{\lambda}(g)y'\rangle_{\lambda}=d^{-1}_{\lambda}\overline{\langle x|y\rangle_{\lambda}}\langle x'|y'\rangle_{\lambda} \tag{57}
$$

Si $\lambda$ et $\mu$ sont deux éléments distincts de $\widehat{G}$, pour $x, x'$ dans $V_{\lambda}$ et $y, y'$ dans $V_{\mu}$, on a

$$
\sum_{g\in G}\overline{\langle x|\pi_{\lambda}(g) x'\rangle_{\lambda}}\langle y|\pi_{\mu}(g)y'\rangle_{\mu}= 0 \tag{58}
$$

Pour tout $\lambda \in \widehat{G}$, choisissons une base orthonormale $(e_{\lambda ,i})_{1\leqslant i\leqslant d_{\lambda}}$ de $V_{\lambda}$. Pour tout $g\in G$, notons $(\pi_{ij}^{\lambda}(g))$ la matrice de l’endomorphisme $\pi_{\lambda}(g)$ de $V_{\lambda}$ par rapport à cette base ; on a

$$
\pi^{\lambda}_{ij}(g) =\langle e_{\lambda ,i}|\pi_{\lambda}(g)e_{\lambda ,j}\rangle_{\lambda} \tag{59}
$$

Comme l’endomorphisme $\pi_{\lambda}(g)$ est unitaire, son inverse est égal à $\pi_{\lambda}(g)^*$, d’où (60) $\pi^{\lambda}_{ij}(g) =\pi_{ji}^{\lambda}(g^{-1})$.

Il résulte alors des formules (22) de VIII, p. 399 et (25) p. 399, que les fonctions $(d_{\lambda})^{1/2}\pi_{ij}^{\lambda}$, pour $\lambda \in \widehat{G}, 1\leqslant i\leqslant d_{\lambda}, 1\leqslant j\leqslant d_{\lambda}$, forment une base orthonormale de l’espace hilbertien $\mathbf{C}[G].*$

## EXERCICES {#alg-viii-s21-exercises}

See the [exercises for § 21](exercises/s21/).

[^1]: Les éléments de Hom$_G(\pi , \pi ')$ sont parfois appelés opérateurs d’entrelacement de $\pi$ et $\pi '$.
