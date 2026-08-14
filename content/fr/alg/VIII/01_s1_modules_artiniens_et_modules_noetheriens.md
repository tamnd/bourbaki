---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Modules et anneaux semi-simples
section: 1
section_title: Modules artiniens et modules noethériens
lang: fr
source: alg-viii-fr
book_pages: A VIII.1-A VIII.22
pdf_pages: 0012-0033
extraction: native
subsections:
    - "no": 1
      title: Modules artiniens et modules noethériens
      page: 1
      pdf_page: 12
    - "no": 2
      title: Anneaux artiniens et anneaux noethériens
      page: 4
      pdf_page: 15
    - "no": 3
      title: Contremodule
      page: 8
      pdf_page: 19
    - "no": 4
      title: Polynômes à coefficients dans un anneau noethérien
      page: 9
      pdf_page: 20
statements: 36
exercises: 28
content_sha256: 2b08bf5d172d32adbe9fb5702b2f948e3152a8025e0501c9e93de6eefe5eac90
---

## § 1. MODULES ARTINIENS ET MODULES NOETHÉRIENS

### 1. Modules artiniens et modules noethériens

#### Définition 1 {#alg-viii-s1-def-1 .statement tag=0001}

Soit A un anneau. On dit qu’un A-module M est artinien (resp. noethérien) s’il vérifie les conditions équivalentes suivantes :

(i) Tout ensemble non vide de sous-modules de M, ordonné par la relation d’inclusion, possède un élément minimal (resp. maximal) ;

(ii) Toute suite décroissante (resp. croissante) de sous-modules de M est stationnaire.

L’équivalence des conditions (i) et (ii) résulte de E, III, p. 51, prop. 6.

Pour qu’un A-module M soit artinien (resp. noethérien), il faut et il suffit que M, considéré comme module sur l’anneau $A_M$ des homothéties, le soit.

Soit M un A-module artinien (resp. noethérien). Tout ensemble non vide de sous-modules de M, ordonné par inclusion, qui est filtrant décroissant (resp. filtrant croissant) possède un plus petit élément (resp. un plus grand élément) (E, III, p. 13, prop. 10).

Soient M un A-module artinien (resp. noethérien) et $(M_i)_{i\in I}$ une famille de sous-modules de M. Les intersections (resp. sommes) des sous-familles finies de la famille $(M_i)_{i\in I}$ forment un ensemble non vide filtrant décroissant (resp. filtrant croissant) de sous-modules de M. Il existe donc une partie finie J de I tel que $\bigcap_{i\in I}M_i=\bigcap_{i\in J}M_i$ (resp. $\sum_{i\in I}M_i=\sum_{i\in J}M_i)$.

#### Exemple 1 {#alg-viii-s1-n1-exa-1 .statement tag=0002}

Un espace vectoriel de dimension finie sur un corps est artinien et noethérien.

#### Exemple 2 {#alg-viii-s1-n1-exa-2 .statement tag=0003}

Soit M un A-module. S’il existe une famille infinie $(M_i)_{i\in I}$ de sous-modules non nuls de M dont la somme est directe, M n’est ni artinien, ni noethérien : en effet, pour toute suite infinie $(J_n)$ strictement décroissante (resp. strictement croissante) de parties de I, la suite infinie $(\sum_{i\in J_n}M_i)$ de sous-modules de M est strictement décroissante (resp. strictement croissante). En particulier, un espace vectoriel de dimension infinie sur un corps n’est ni artinien ni noethérien.

#### Exemple 3 {#alg-viii-s1-n1-exa-3 .statement tag=0004}

On verra plus loin que le $\mathbf{Z}$-module $\mathbf{Z}$est noethérien, mais non artinien (VIII,

p. 5, exemple 3$).*$

#### Exemple 4 {#alg-viii-s1-n1-exa-4 .statement tag=0005}

Soient $p$ un nombre premier et $M_p$ le composant $p$-primaire du $\mathbf{Z}$-module de torsion $\mathbf{Q}/\mathbf{Z}$(VII, p. 8). Tout sous-module de $M_p$ est égal soit à $M_p$, soit à $p^{-n}\mathbf{Z}/\mathbf{Z}$ pour un entier $n\in \mathbf{N}$(VII, p. 53, exerc. 3). Par suite, $M_p$ est un $\mathbf{Z}$-module artinien, mais non noethérien.

#### Proposition 1 {#alg-viii-s1-prop-1 .statement tag=0006}

Pour qu’un A-module M soit de longueur finie (II, p. 21), il faut et il suffit qu’il soit à la fois artinien et noethérien.

Supposons que M soit de longueur finie $d$. Alors toute suite strictement croissante ou strictement décroissante de sous-modules de M comporte au plus $d+ 1$ termes (I, p. 42). Par suite M est artinien et noethérien.

Réciproquement, supposons que M soit artinien et noethérien. Soit $\mathscr{S}$ l’ensemble des sous-modules de longueur finie de M. Le sous-module nul appartient à $\mathscr{S}$, et comme M est noethérien, $\mathscr{S}$ possède un élément maximal N. Raisonnons par l’absurde en supposant que $M\not= N$. L’ensemble des sous-modules de M distincts de N et contenant N possède alors un élément minimal P, puisque M est artinien. Le module $P/N$ est de longueur 1 et, comme N est un module de longueur finie, il en est de même de P (II, p. 21, prop. 16). Ceci contredit la définition de N.

#### Proposition 2 {#alg-viii-s1-prop-2 .statement tag=0007}

Pour qu’un A-module M soit noethérien, il faut et il suffit que tout sous-module de M soit de type fini.

Supposons d’abord que tout sous-module de M soit de type fini. Soit $(P_n)_{n\in\mathbf{N}}$ une suite croissante de sous-modules de M et soit P sa réunion. C’est un sous-module de M. Il existe par hypothèse une partie finie F de M engendrant le module P ; soit alors $n\in \mathbf{N}$un entier tel que $F\subset P_n$. On a donc $P_n= P$ et la suite $(P_n)_{n\in\mathbf{N}}$ est stationnaire. Cela prouve que le module M est noethérien.

La réciproque résulte de l’énoncé plus précis suivant :

#### Lemme 1 {#alg-viii-s1-lem-1 .statement tag=0008}

Soient M un A-module noethérien et E une partie de M. Il existe une partie finie F de E engendrant le même sous-module que E.

En effet, d’après VIII, p. 2, il existe une partie finie F de E telle que $\sum_{x\in E}Ax=$ $\sum_{x\in F}Ax$.

#### Proposition 3 {#alg-viii-s1-prop-3 .statement tag=0009}

Soient M un A-module et N un sous-module de M. Pour que M soit artinien (resp. noethérien), il faut et il suffit que N et $M/N$le soient.

Nous donnerons la démonstration dans le cas des modules artiniens, le cas des modules noethériens étant analogue.

Supposons M artinien. Tout sous-module de N étant un sous-module de M, le module N est artinien. Soit $(P_n)_{n\in\mathbf{N}}$ une suite décroissante de sous-modules de $M/N$. Il existe une suite décroissante $(Q_n)_{n\in\mathbf{N}}$ de sous-modules de M contenant N, telle que $P_n= Q_n/N$ pour tout $n\in \mathbf{N}$(I, p. 39, th. 4). Comme M est artinien, la suite $(Q_n)$ est stationnaire, donc aussi la suite $(P_n)$. Par suite, le module $M/N$ est artinien.

Réciproquement, supposons les modules N et $M/N$ artiniens et considérons une suite décroissante $(P_n)$ de sous-modules de M. La suite des sous-modules $P'_n= N\cap P_n$ de N est stationnaire. De même, la suite des sous-modules $P''_n= (N + P_n)/N$ de $M/N$ est stationnaire. Il existe donc un entier $m\in \mathbf{N}$tel que l’on ait $P'_n= P'_m$ et $P''_n= P''_m$ pour tout entier $n\geqslant m$. La suite $(P_n)$ est alors stationnaire en vertu du lemme suivant :

#### Lemme 2 {#alg-viii-s1-lem-2 .statement tag=00QV}

Soient M un A-module, N, P et Q des sous-modules de M. On suppose que l’on a $P\subset Q$, $N\cap P = N\cap Q$et N + P = N + Q. On a alors P = Q.

Soit $x$ un élément de Q. Il appartient à N + P ; il existe donc un élément $y$ de P tel que $x-y\in N$. Comme Q contient $P,x-y$ appartient à $N\cap Q$, donc à P. Par suite, $x$ appartient à P.

#### Corollaire {#alg-viii-s1-n1-cor-1 .statement tag=000A}

Soient M un A-module et $(M_i)_{i\in I}$ une famille finie de sous-modules de M.

a) Si les modules $M_i$ sont artiniens (resp. noethériens), il en est de même de leur somme $\sum_{i\in I}M_i$.

b) Si les modules $M/M_i$ sont artiniens (resp. noethériens), il en est de même du module $M/\bigcap_{i\in I}M_i$.

Par récurrence, il suffit de traiter le cas où $I =\{1,2\}$. Le module $M_2/(M_1\cap M_2)$, quotient de $M_2$, est isomorphe au sous-module $(M_1+ M_2)/M_1$ de $M/M_1$ (I, p. 39, th. 4).

Sous l’hypothèse a), $M_1$ et $(M_1+ M_2)/M_1$ sont artiniens (resp. noethériens) ; il en est donc de même de $M_1+ M_2$ (prop. 3).

Sous l’hypothèse b), $M/M_2$ et $M_2/(M_1\cap M_2)$ sont artiniens (resp. noethériens) ; il en est donc de même de $M/(M_1\cap M_2) ($loc. cit.).

#### Exemple 5 {#alg-viii-s1-n1-exa-5 .statement tag=000B}

Soit $(M_i)_{i\in I}$ une famille finie de A-modules. Si les modules $M_i$ sont artiniens (resp. noethériens), il en est de même de leur somme directe $\bigoplus_{i\in I}M_i$.

#### Remarque {#alg-viii-s1-n1-rem-1 .statement tag=000C}

Les définitions et résultats de ce numéro s’étendent aux groupes commutatifs à opérateurs quelconques en remplaçant dans les énoncés sous-modules par sous-groupes stables.

### 2. Anneaux artiniens et anneaux noethériens

#### Définition 2 {#alg-viii-s1-def-2 .statement tag=000D}

On dit qu’un anneau A est artinien (resp. noethérien) à gauche si le A-module à gauche $A_s$ est artinien (resp. noethérien). De même, on dit qu’un anneau A est artinien (resp. noethérien) à droite si le A-module à droite $A_d$ est artinien (resp. noethérien).

Un anneau A est artinien (resp. noethérien) à droite si et seulement si l’anneau opposé $A^o$ est artinien (resp. noethérien) à gauche. Pour un anneau A commutatif, les propriétés d’être artinien à gauche et artinien à droite coïncident, et lorsqu’elles sont satisfaites, on dit que l’anneau A est artinien ; on adopte une convention analogue pour « noethérien ». Il existe des anneaux non commutatifs artiniens à gauche mais non à droite, et des anneaux non commutatifs noethériens à gauche mais non à droite (VIII, p. 13, exerc. 3).

Soit A un anneau. Par définition, les conditions suivantes sont équivalentes :

(i) L’anneau A est artinien à gauche ;

(ii) Tout ensemble non vide d’idéaux à gauche de A, ordonné par inclusion, possède un élément minimal ;

(iii) Toute suite décroissante d’idéaux à gauche de A est stationnaire.

Compte tenu de la prop. 2 de VIII, p. 3 les conditions suivantes sont équivalentes :

(i) L’anneau A est noethérien à gauche ;

(ii) Tout ensemble non vide d’idéaux à gauche de A, ordonné par inclusion, possède un élément maximal ;

(iii) Toute suite croissante d’idéaux à gauche de A est stationnaire ;

(iv) Tout idéal à gauche de A est engendré par une partie finie de A.

#### Exemple 1 {#alg-viii-s1-n2-exa-1 .statement tag=000E}

Un corps est un anneau artinien et noethérien, à gauche et à droite.

#### Exemple 2 {#alg-viii-s1-n2-exa-2 .statement tag=000F}

Soient A un anneau et D un sous-anneau de A. On suppose que D est un corps et que A est un espace vectoriel à gauche de dimension finie sur D. Comme tout idéal à gauche de A est un sous-D-espace vectoriel de A, l’anneau A est artinien et noethérien à gauche. En particulier, une algèbre de dimension finie sur un corps commutatif est un anneau artinien et noethérien, à gauche et à droite.

#### Exemple 3 {#alg-viii-s1-n2-exa-3 .statement tag=000G}

Un anneau principal (VII, p. 1, déf. 1) est noethérien. Un anneau intègre A qui n’est pas un corps n’est pas un anneau artinien : pour tout élément $a$ de A, non nul et non inversible, la suite des idéaux $a^nA$ (pour $n\in \mathbf{N})$ est strictement décroissante. En particulier, l’anneau $\mathbf{Z}$des entiers rationnels est noethérien, mais n’est pas artinien.

#### Exemple 4 {#alg-viii-s1-n2-exa-4 .statement tag=000H}

Soit M un A-module, somme directe d’une famille infinie $(M_i)_{i\in I}$ de sous-modules non nuls. Soit E l’anneau des endomorphismes de M. Pour tout $i\in I$, soit $\mathfrak{a}_i$ (resp. $\mathfrak{b}_i)$ l’ensemble des éléments de E dont le noyau contient $\sum_{j\not=i}M_j$ (resp. dont l’image est contenue dans $M_i)$. Alors $(\mathfrak{a}_i)$ est une famille infinie d’idéaux à gauche non nuls de E dont la somme est directe, et $(\mathfrak{b}_i)$ est une famille infinie d’idéaux à droite non nuls de E dont la somme est directe. Par suite l’anneau E n’est artinien (resp. noethérien) ni à gauche, ni à droite (VIII, p. 2, exemple 2). En particulier, l’anneau des endomorphismes d’un espace vectoriel de dimension infinie n’est artinien (resp. noethérien) ni à gauche, ni à droite.

#### Théorème 1 {#alg-viii-s1-thm-1 .statement tag=00QW}

Soit A un anneau artinien à gauche. Le A-module $A_s$ est de longueur finie.

Nous utiliserons dans la démonstration le lemme suivant :

#### Lemme 3 {#alg-viii-s1-lem-3 .statement tag=000I}

Soient A un anneau et $n$ un entier naturel. Un A-module artinien M qui est somme d’une famille de sous-modules de longueur $\leqslant n$ est de longueur finie.

Raisonnons par récurrence sur $n$. Supposons d’abord $n= 1$. Si M n’était pas de longueur finie, nous pourrions construire une suite $(M_m)_{m\in\mathbf{N}}$ de sous-modules de longueur 1 de M, avec $M_m\not\subset (\sum_{i<m}M_i)$ pour tout $m\in \mathbf{N}$. Nous aurions alors $M_m\cap \sum_{i<m}M_i= 0$ pour tout $m$, et la somme de la famille $(M_m)_{m\in\mathbf{N}}$ serait directe. Mais ceci contredirait le fait que le A-module M est artinien (VIII, p. 2, exemple 2).

Supposons maintenant $n\geqslant 2$. Soit $(M_i)_{i\in I}$ une famille de sous-modules de longueur $\leqslant n$ de M, de somme M. Choisissons pour tout $i\in I$ un sous-module $M'_i$ de $M_i$ de longueur $\leqslant n-1$, tel que $M_i/M'_i$ soit de longueur $\leqslant 1$. Posons $M'=\sum M'_i$, et notons $M''_i$ l’image de $M_i$ dans $M''= M/M'$. Les modules $M''_i$ sont de longueur $\leqslant 1$ et leur somme est $M''$. Les modules $M'$ et $M''$ sont artiniens (VIII, p. 3, prop. 3) ; d’après l’hypothèse de récurrence, ils sont de longueur finie. Donc M est de longueur finie (II, p. 21, prop. 16).

Démontrons maintenant le th. 1. Notons $\mathscr{S}$ l’ensemble des idéaux à gauche $\mathfrak{a}$ de A, tels que le module $A_s/\mathfrak{a}$ soit de longueur finie. Soit $(\mathfrak{a}_i)_{i\in I}$ une famille finie d’éléments de $\mathscr{S}$. D’après la prop. 1 de VIII, p. 2, le A-module $A_s/\mathfrak{a}_i$ est artinien et noethérien pour tout $i\in I$. Par suite, $A_s/\bigcap_{i\in I}\mathfrak{a}_i$ est artinien et noethérien (VIII, p. 4, cor. de la prop. 3), donc de longueur finie (VIII, p. 2, prop. 1). Cela démontre que $\mathscr{S}$ est filtrant décroissant pour la relation d’inclusion. Comme l’anneau A est artinien à gauche, l’ensemble $\mathscr{S}$ possède un plus petit élément $\mathfrak{b}$. Notons $n$ la longueur du A-module $A_s/\mathfrak{b}$.

Soient $x$ un élément de $A_s$ et $\mathfrak{a}$ son annulateur (II, p. 28). Le A-module $Ax$ est isomorphe à $A_s/\mathfrak{a}$. Si $Ax$ est de longueur finie, $\mathfrak{a}$ appartient à $\mathscr{S}$, donc $\mathfrak{a}$ contient $\mathfrak{b}$ et $Ax$ est de longueur $\leqslant n$. Ainsi, tout idéal à gauche monogène de A qui est de longueur finie est de longueur $\leqslant n$. Soit $\mathfrak{c}$ la somme de ces idéaux ; c’est un idéal à gauche de A, de longueur finie d’après le lemme 3. Tout idéal à gauche de longueur finie de A est somme d’idéaux à gauche monogènes de longueur finie, donc est contenu dans $\mathfrak{c}$. Ainsi $\mathfrak{c}$ est le plus grand idéal à gauche de longueur finie de A.

Si $\mathfrak{c}$ était distinct de A, l’ensemble des idéaux à gauche de A contenant $\mathfrak{c}$ et distincts de $\mathfrak{c}$ posséderait un élément minimal $\mathfrak{c}'$. Le A-module $\mathfrak{c}'/\mathfrak{c}$ serait de longueur 1 et $\mathfrak{c}'$ serait de longueur finie, ce qui contredirait la maximalité de $\mathfrak{c}$. On a donc $\mathfrak{c}= A$, le A-module $A_s$ est de longueur finie.

#### Corollaire {#alg-viii-s1-n2-cor-1 .statement tag=000J}

Tout anneau artinien à gauche est noethérien à gauche.

Soit A un anneau artinien à gauche. Par le théorème 1, le A-module $A_s$ est de longueur finie. On applique alors la prop. 1 de VIII, p. 2.

Soit A un anneau artinien à gauche (resp. à droite) ; la longueur du A-module $A_s$ (resp. $A_d)$ (I, p. 42) est appelée la longueur à gauche (resp. à droite) de l’anneau A. Lorsque A est un anneau commutatif et artinien, ces deux longueurs coïncident et sont appelées simplement la longueur de A. Lorsque A est artinien à droite et à gauche mais n’est pas commutatif, les longueurs à gauche et à droite de A ne sont pas nécessairement égales (VIII, p. 13, exerc. 3).

#### Exemple 5 {#alg-viii-s1-n2-exa-5 .statement tag=000K}

Les longueurs à gauche et à droite d’un corps sont égales à 1.

#### Proposition 4 {#alg-viii-s1-prop-4 .statement tag=000L}

a) Soient A un anneau noethérien à gauche et M un A-module à gauche de type fini. Le module M est noethérien et tout sous-module de M est de type fini.

b) Soient A un anneau artinien à gauche et M un A-module à gauche. Les conditions suivantes sont équivalentes : le module M est de type fini ; le module M est artinien ; le module M est de longueur finie ; le module M est noethérien.

Démontrons a). Tout sous-module monogène de M est isomorphe à un quotient de $A_s$, donc est noethérien par la prop. 3 de VIII, p. 3. Le module M est une somme finie de tels sous-modules, il est donc noethérien par le cor. (VIII, p. 4) de la prop. 3. Tout sous-module de M est alors de type fini (VIII, p. 3, prop. 2).

Supposons maintenant l’anneau A artinien à gauche. On démontre comme dans l’alinéa précédent que si le A-module M est de type fini, il est artinien. S’il est artinien, il est de longueur finie : en effet ses sous-modules monogènes sont isomorphes à des quotients de $A_s$, donc sont de longueur finie inférieure à celle de $A_s$ et l’assertion résulte du lemme 3. Tout module de longueur finie est noethérien et tout module noethérien est de type fini. Cela démontre b).

#### Proposition 5 {#alg-viii-s1-prop-5 .statement tag=000M}

a) Soit A un anneau artinien (resp. noethérien) à gauche et soit $\varphi : A\rightarrow B$un homomorphisme d’anneaux qui fasse de B un A-module à gauche de type fini. L’anneau B est artinien (resp. noethérien) à gauche.

b) Soit A un anneau artinien (resp. noethérien) à gauche et soit $\mathfrak{a}$ un idéal bilatère de A ; l’anneau $A/\mathfrak{a}$ est artinien (resp. noethérien) à gauche.

c) Soit $(A_i)_{i\in I}$ une famille finie d’anneaux artiniens (resp. noethériens) à gauche. L’anneau $\prod_{i\in I}A_i$ est artinien (resp. noethérien) à gauche.

Nous traiterons le cas des anneaux artiniens, le cas des anneaux noethériens étant analogue.

Démontrons a). D’après la prop. 4, $B_s$ est un A-module à gauche artinien, et a fortiori un B-module à gauche artinien.

L’assertion b) résulte de l’assertion a) appliquée à l’homomorphisme canonique de A sur $A/\mathfrak{a}$.

Prouvons c). Posons $A =\prod_{i\in I}A_i$. Par hypothèse, $(A_i)_s$ est un $A_i$-module à gauche artinien, et a fortiori un A-module à gauche artinien. D’après l’exemple 5 de VIII, p. 4, le A-module $A_s$ est artinien.

#### Corollaire {#alg-viii-s1-n2-cor-2 .statement tag=000N}

Les idéaux premiers d’un anneau commutatif artinien sont ses idéaux maximaux.

Dans tout anneau commutatif, un idéal maximal est premier. Soit A un anneau commutatif artinien. Soit $\mathfrak{p}$ un idéal premier de A. L’anneau $A/\mathfrak{p}$ est intègre et artinien (prop. 5), donc est un corps (VIII, p. 5, exemple 3). Par conséquent, l’idéal $\mathfrak{p}$ est maximal.

☡ L’anneau de polynômes $\mathbf{Q}[(X_n)_{n\in\mathbf{N}}]$ est intègre ; il n’est pas noethérien (ni artinien) (VIII, p. 14, exerc. 9). C’est un sous-anneau de son corps des fractions, qui est, lui, un anneau artinien (et noethérien).

### 3. Contremodule

#### Définition 3 {#alg-viii-s1-def-3 .statement tag=000O}

Soient A un anneau, M un A-module et E l’anneau des endomorphismes de M. On appelle contremodule de M le E-module à gauche ayant même groupe additif sous-jacent que M et pour loi d’action $(c, x)\rightarrow c(x)$.

Soit Z le centre de l’anneau A. Pour tout $a\in Z$, l’homothétie $a_M$ appartient à E. Par suite, E est canoniquement muni d’une structure d’algèbre sur Z. En particulier, si M est un Z-module de type fini, le contremodule de M est de type fini.

#### Lemme 4 {#alg-viii-s1-lem-4 .statement tag=000P}

Soient M un A-module à gauche dont le contremodule est de type fini. Il existe un entier naturel $m$ et une application $A_M$-linéaire injective de $(A_M)_s$ dans $M^m$.

Posons E = End$_A(M)$. Soit $(x_1, . . . , x_m)$ une famille génératrice finie du E-module M. L’application $\varphi :a\rightarrow (ax_1, . . . , ax_m)$ de $(A_M)_s$ dans $M^m$ est $A_M$-linéaire. Soit $a$ un élément de $A_M$ tel que $\varphi (a) = 0$. L’ensemble des éléments $x$ de M tels que $ax= 0$ est un sous-E-module de M contenant $x_1, . . . , x_m$, donc égal à M, ce qui entraîne $a= 0$.

#### Proposition 6 {#alg-viii-s1-prop-6 .statement tag=000Q}

Soit M un A-module à gauche artinien (resp. noethérien) dont le contremodule est de type fini. L’anneau $A_M$ des homothéties de M est artinien (resp. noethérien) à gauche.

Cela résulte du lemme 4 et de la prop. 3 de VIII, p. 3.

#### Corollaire {#alg-viii-s1-n3-cor-1 .statement tag=000R}

Soit A un anneau commutatif.

a) Soit M un A-module noethérien. L’anneau $A_M$ est noethérien.

b) Soit M un A-module de longueur finie. L’anneau $A_M$ est artinien.

Soit M un A-module. Sous les hypothèses de a) ou de b), le A-module M est de type fini. Comme A est commutatif, $A_M$ est contenu dans l’anneau End$_A$(M), de sorte que le contremodule de M est de type fini. Il suffit alors d’appliquer la prop. 6.

#### Remarque {#alg-viii-s1-n3-rem-1 .statement tag=000S}

Soit A un anneau. Un A-module à gauche artinien M dont le contremodule est de type fini est de longueur finie : en effet, l’anneau $A_M$ des homothéties de M est artinien à gauche (prop. 6) et M est un module artinien sur $A_M$; d’après VIII, p. 7, prop. 4, M est un module de longueur finie sur $A_M$, et donc aussi sur A.

En particulier, tout module artinien de type fini sur un anneau commutatif est de longueur finie. Par contre, un module artinien de type fini sur un anneau non commutatif n’est pas nécessairement de longueur finie (VIII, p. 15, exerc. 12).

### 4. Polynômes à coefficients dans un anneau noethérien

Soient A un anneau, $\sigma$ un endomorphisme de l’anneau A et $d$ un endomorphisme du groupe additif de A, satisfaisant la relation

$$
d(ab) =\sigma (a)d(b) +d(a)b \tag{1}
$$

pour tous $a, b\in A$. Autrement dit, $d$ est une dérivation de l’anneau A dans le $(A,A)$-bimodule obtenu en munissant le groupe additif de A de la loi d’action à gauche $(a, x)\rightarrow \sigma (a)x$, et de la loi d’action à droite $(a, x)\rightarrow xa$. On a $d(1) = 0$ (III, p. 122, prop. 3).

Rappelons (IV, p. 2) que A[X] désigne le $\mathbf{Z}$-module $A\otimes_{\mathbf{Z}}\mathbf{Z}[X]$ des polynômes en une indéterminée à coefficients dans A. On le munit de sa structure naturelle de A-module à gauche. La famille $(X^n)_{n\in\mathbf{N}}$ en est une base. On identifie A à son image par l’application $a\rightarrow a\otimes 1$.

#### Proposition 7 {#alg-viii-s1-prop-7 .statement tag=00QX}

Soient A$,\sigma ,d$ comme ci-dessus. Il existe sur le groupe A[X] une unique structure d’anneau possédant les propriétés suivantes :

a) L’addition de cet anneau est l’addition usuelle de A[X] ;

b) La multiplication de cet anneau prolonge celle de A ;

c) Le produit dans cet anneau d’une suite $(a,X, . . . ,X)$, formée d’un élément $a$ de A suivi de $n$ termes égaux à X, est le polynôme $aX^n$;

d) On a dans cet anneau $Xa=\sigma (a)X +d(a)$pour tout $a\in A$.

Notons E l’anneau des endomorphismes du groupe additif A[X]. L’application qui à $a\in A$ associe l’homothétie $a_M$ du A-module à gauche M = A[X] est un homomorphisme d’anneaux de A dans E. Considérons les éléments $u,\sigma_M$ et $d_M$ de E définis par $u(\sum b_nX^n) =\sum b_nX^{n+1},\sigma_M(\sum b_nX^n) =\sum\sigma (b_n)X^n,d_M(\sum b_nX^n) =$ $\sum d(b_n)X^n$. On a, pour tout $a\in A$

$$
u a_M=a_Mu ,\sigma_Ma_M=\sigma (a)_M\sigma_M,d_Ma_M=\sigma (a)_Md_M+d(a)_M \tag{2}
$$

Posons

$$
X_M=\sigma_Mu+d_M \tag{3}
$$

Il résulte de (2) que l’on a, pour tout $a\in A$,

$$
X_Ma_M=\sigma (a)_MX_M+d(a)_M \tag{4}
$$

Considérons l’application $\varphi : A[X]\rightarrow E$ définie par

$$
\varphi (\sum a_nX^n)=\sum(a_n)_M(X_M)^n \tag{5}
$$

C’est un homomorphisme de groupes. On démontre par récurrence que l’on a $(X_M)^n(1) = X^n$ pour tout $n\in \mathbf{N}$. On a donc $\varphi (P)(1) = P$ pour tout $P\in A[X]$, ce qui prouve que l’homomorphisme $\varphi$ est injectif. Notons B son image. L’ensemble B est un sous-groupe de E ; il contient 1, est stable par multiplication à gauche par $a_M$ pour $a\in A$, et par $X_M$ d’après (4). C’est donc un sous-anneau de E. L’unique structure d’anneau sur A[X] déduite de celle de B par transport de structure par $\varphi$ possède les propriétés de la prop. 7, la propriété d) résultant de la formule (4).

Si A[X] est muni d’une structure d’anneau possédant les propriétés de la prop. 7, l’homothétie à gauche $\boldsymbol{\gamma }_X$ de cet anneau (I, p. 92) applique nécessairement $bX^n$ sur $\sigma (b)X^{n+1}+d(b)X^n$ pour $b\in A$ et $n\in \mathbf{N}$, donc est égale à $X_M$. L’homothétie $\boldsymbol{\gamma }_a$ est nécessairement égale à $a_M$ pour tout $a\in A$. Il s’ensuit que l’on a $\boldsymbol{\gamma }_P=\varphi (P)$ pour tout $P\in A[X]$, d’où l’assertion d’unicité de la prop. 7.

L’ensemble A[X], muni de l’unique structure d’anneau satisfaisant aux conditions de la prop. 7, est noté $A[X]_{\sigma ,d}$ et appelé l’anneau de polynômes en X à coefficients dans A, relatif à $\sigma$ et $d$. On le note simplement $A[X]_{\sigma}$ lorsque $d$ est l’application nulle, et A[X] lorsque de plus $\sigma$ est l’application identique de A. Cette notation est compatible avec celle introduite en IV, p. 1 pour un anneau A commutatif.

#### Remarque {#alg-viii-s1-n4-rem-1 .statement tag=000T}

L’anneau $A[X]_{\sigma ,d}$ possède la propriété universelle suivante : étant donnés un anneau $A'$, un homomorphisme d’anneaux $f: A\rightarrow A'$ et un élément $x$ de $A'$ tels que $xf(a) =f(\sigma (a))x+f(d(a))$pour tout $a\in A$, il existe un unique homomorphisme d’anneaux $g: A[X]_{\sigma ,d}\rightarrow A'$ qui prolonge $f$ et applique X sur $x$.

L’assertion d’unicité est claire. Montrons que l’application $g: A[X]_{\sigma ,d}\rightarrow$ $A'$ définie par $g(\sum a_nX^n) =\sum f(a_n)x^n$ possède les propriétés requises. Elle prolonge $f$, applique X sur $x$ et est un homomorphisme de groupes. On a $g(1) =$ 1. Pour $a\in A$ et $Q =\sum a_nX^n$ dans $A[X]_{\sigma ,d}$, on a

$$
g(aQ) =g(\sum aa_nX^n)=\sum f(aa_n)x^n=f(a)\sum f(a_n)x_n=g(a)g(Q)
$$

ainsi que

$g$(XQ) $=g(\sum (\sigma (a_n)X^{n+1}+d(a_n)X^n))$

$$
=\sum(f(\sigma (a_n))x^{n+1}+f(d(a_n))x^n) =x\sum f(a_n)x^n=g(X)g(Q)
$$

On en déduit que l’on a $g(P)g(Q) =g$(PQ) pour $P,Q$ dans $A[X]_{\sigma ,d}$ et donc que $g$ est un homomorphisme d’anneaux.

#### Théorème 2 {#alg-viii-s1-thm-2 .statement tag=000U}

Soit A un anneau noethérien à gauche et soient $\sigma$ un automorphisme de A et $d$ un endomorphisme du groupe additif de A satisfaisant la relation (1). L’anneau $A[X]_{\sigma ,d}$ est noethérien à gauche.

Posons $B = A[X]_{\sigma ,d}$. Pour tout entier $n\geqslant 0$, notons $B_n$ l’ensemble des éléments de B de la forme $a_0+a_1X +\cdots +a_nX^n$. C’est un sous-A-module à gauche de B. L’application $\varphi_n: B_n\rightarrow A_s$ définie par $\varphi_n(a_0+a_1X+\cdots +a_nX^n) =a_n$ est A-linéaire.

Soit $\mathfrak{b}$ un idéal à gauche de B. Pour tout entier $n\geqslant 0$, l’ensemble $\mathfrak{a}_n=\varphi_n(\mathfrak{b}\cap B_n)$ est un idéal à gauche de A. Comme on a $Xa=\sigma (a)X +d(a)$ pour tout $a\in A$, on a

(6) $\varphi_{n+1}$(XQ) $=\sigma (\varphi_n(Q))$

pour tout $Q\in B_n$, d’où $\sigma (\mathfrak{a}_n)\subset \mathfrak{a}_{n+1}$. Par conséquent, la suite des idéaux $\mathfrak{a}'_n=$ $\sigma^{-n}(\mathfrak{a}_n)$ de A est croissante. Comme l’anneau A est noethérien à gauche, il existe un entier $m\geqslant 0$ tel que l’on ait $\mathfrak{a}'_n=\mathfrak{a}'_{n+1}$ pour $n\geqslant m$. Comme $\sigma$ est surjectif, on a la relation

$$
\sigma (\mathfrak{a}_n) =\mathfrak{a}_{n+1} \tag{7}
$$

pour tout entier $n\geqslant m$.

Soit $\mathfrak{c}$ l’idéal à gauche de B engendré par $\mathfrak{b}\cap B_m$; comme le A-module à gauche $B_m$ est de type fini et que l’anneau A est noethérien à gauche, le A-module à gauche $\mathfrak{b}\cap B_m$ est de type fini (VIII, p. 7, prop. 4 a)). L’idéal à gauche $\mathfrak{c}$ est donc engendré par une partie finie de B. Il est clair qu’il est contenu dans $\mathfrak{b}$. Démontrons qu’il est égal à $\mathfrak{b}$ en démontrant par récurrence que l’on a, pour tout entier $n\geqslant 0$,

$$
\mathfrak{b}\cap B_n\subset \mathfrak{c} \tag{8}
$$

La relation (8) est vraie par construction pour $n\leqslant m$. Supposons désormais que $n$ soit un entier $\geqslant m$ tel que $\mathfrak{b}\cap B_n\subset \mathfrak{c}$. Soit P un élément de $\mathfrak{b}\cap B_{n+1}$. Alors $\varphi_{n+1}(P)$ appartient à $\mathfrak{a}_{n+1}=\sigma (\mathfrak{a}_n)$ et il existe donc un élément Q de $\mathfrak{b}\cap B_n$ tel que $\varphi_{n+1}(P) =\sigma (\varphi_n(Q))$. Posons $R = P-$ XQ. Compte tenu de la relation (6), on a $\varphi_{n+1}(R) = 0$, c’est-à-dire $R\in B_n$. Comme P et Q appartiennent à l’idéal à gauche $\mathfrak{b}$ de B, il en est de même de R ; ainsi, R et Q appartiennent à $\mathfrak{b}\cap B_n$, qui est contenu dans l’idéal $\mathfrak{c}$ d’après l’hypothèse de récurrence. Par suite, P appartient à $\mathfrak{c}$. Cela prouve que l’on a $\mathfrak{b}\cap B_{n+1}\subset \mathfrak{c}$.

Ainsi, $\mathfrak{b}$ est égal à $\mathfrak{c}$; c’est donc un idéal de type fini de B. Cela démontre que l’anneau B est noethérien à gauche.

Si l’endomorphisme $\sigma$ de l’anneau A n’est pas un automorphisme, l’anneau $A[X]_{\sigma ,d}$ n’est pas nécessairement noethérien à gauche, même lorsque A est un anneau commutatif noethérien (VIII, p. 21, exerc. 26).

#### Corollaire 1 (Hilbert) {#alg-viii-s1-thm-2-cor-1 .statement tag=00RW}

Soit A un anneau commutatif et noethérien. Pour tout entier $n\geqslant 0$, l’algèbre de polynômes $A[X_1, . . . ,X_n]$est un anneau noethérien.

Cela résulte par récurrence du théorème 2, compte tenu de la prop. 8 de III, p. 26.

#### Corollaire 2 {#alg-viii-s1-thm-2-cor-2 .statement tag=000V}

Soit A un anneau commutatif et noethérien. Une A-algèbre commutative engendrée par un nombre fini d’éléments est un anneau noethérien.

Une telle algèbre est isomorphe à une algèbre de la forme $A[X_1, . . . ,X_n]/\mathfrak{a}$ où $n\geqslant 0$ et $\mathfrak{a}$ un idéal de $A[X_1, . . . ,X_n]$. On applique alors le corollaire 1 et la prop. 5 de VIII, p. 7

#### Corollaire 3 {#alg-viii-s1-thm-2-cor-3 .statement tag=000W}

Tout anneau commutatif est réunion d’une famille filtrante croissante de sous-anneaux noethériens.

Soit en effet A un anneau commutatif. Les sous-anneaux de A qui sont engendrés (en tant que $\mathbf{Z}$-algèbres) par un nombre fini d’éléments sont noethériens d’après le cor. 2. Ils forment une famille filtrante croissante de sous-anneaux de A, dont la réunion est A.

## EXERCICES {#alg-viii-s1-exercises}

See the [exercises for § 1](exercises/s1/).
