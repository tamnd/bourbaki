---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Modules et anneaux semi-simples
section: 11
section_title: Groupes de Grothendieck
lang: fr
source: alg-viii-fr
book_pages: A VIII.179-A VIII.205
pdf_pages: 0184-0210
extraction: native
subsections:
    - "no": 1
      title: Fonctions additives de modules
      page: 179
      pdf_page: 184
    - "no": 2
      title: Groupe de Grothendieck d’un ensemble additif de modules
      page: 182
      pdf_page: 187
    - "no": 3
      title: Utilisation des suites de composition
      page: 185
      pdf_page: 190
    - "no": 4
      title: Le groupe de Grothendieck R(A)
      page: 186
      pdf_page: 191
    - "no": 5
      title: Changement d’anneaux
      page: 189
      pdf_page: 194
    - "no": 6
      title: Le groupe de Grothendieck $R_K(A)$
      page: 189
      pdf_page: 194
    - "no": 7
      title: Structure multiplicative dans $K(\mathscr{C})$
      page: 191
      pdf_page: 196
    - "no": 8
      title: Le groupe de Grothendieck $K_0(A)$
      page: 195
      pdf_page: 200
    - "no": 9
      title: Le groupe de Grothendieck $K_0(A)$d’un anneau artinien
      page: 196
      pdf_page: 201
    - "no": 10
      title: Changement d’anneau pour $K_0(A)$
      page: 197
      pdf_page: 202
    - "no": 11
      title: Réciprocité de Frobenius
      page: 197
      pdf_page: 202
    - "no": 12
      title: Cas des anneaux simples
      page: 199
      pdf_page: 204
statements: 38
exercises: 14
content_sha256: fd7b17e55eb01d077b55b41989952c9f95f654fe728871874512c95173cd150f
---

## § 11. GROUPES DE GROTHENDIECK

### 1. Fonctions additives de modules

Soit A un anneau et soit $\mathscr{C}$ un ensemble de classes de A-modules (VIII, p. 47) ; on dit qu’un A-module est de type $\mathscr{C}$ si sa classe appartient à $\mathscr{C}$.

#### Définition 1 {#alg-viii-s11-def-1 .statement tag=00CS}

On dit que l’ensemble $\mathscr{C}$ de classes de A-modules est additif si tout module nul est de type $\mathscr{C}$ et que la somme directe de deux modules de type $\mathscr{C}$ est de type $\mathscr{C}$. On dit que $\mathscr{C}$ est héréditaire s’il est additif et que les sous-modules et les modules quotients d’un module de type $\mathscr{C}$ sont de type $\mathscr{C}$.

#### Exemple 1 {#alg-viii-s11-n1-exa-1 .statement tag=00CT}

L’ensemble des classes des A-modules de longueur finie est héréditaire (II, p. 21, prop. 16).

#### Exemple 2 {#alg-viii-s11-n1-exa-2 .statement tag=00CU}

L’ensemble des classes de A-modules de type fini est additif. Si l’anneau A est noethérien, il est héréditaire (VIII, p. 3, prop. 3 et VIII, p. 7, prop. 4).

#### Exemple 3 {#alg-viii-s11-n1-exa-3 .statement tag=00CV}

L’ensemble des classes de A-modules projectifs de type fini est additif mais n’est pas héréditaire en général.

#### Définition 2 {#alg-viii-s11-def-2 .statement tag=00CW}

Soit $\varphi$ une application de $\mathscr{C}$ dans un groupe commutatif G (noté additivement) ; posons $\varphi (E) =\varphi$(cl(E)) pour tout A-module E de type $\mathscr{C}$. On dit que $\varphi$ est une fonction additive de modules (resp. une fonction faiblement additive de modules) si l’on a $\varphi (E) =\varphi (E') +\varphi (E'')$pour toute suite exacte (resp. pour toute suite exacte scindée)

$$
0\longrightarrow E'\longrightarrow E\longrightarrow E''\longrightarrow 0
$$

de modules de type $\mathscr{C}$.

#### Exemple 4 {#alg-viii-s11-n1-exa-4 .statement tag=00CX}

Soit $\mathscr{C}$ l’ensemble des classes des A-modules de longueur finie. L’application long$_A:\mathscr{C}\rightarrow \mathbf{Z}$qui associe à toute classe de A-modules de longueur finie sa longueur, est une fonction additive de modules (II, p. 22, cor. 3). Les résultats de ce numéro sont une généralisation des résultats sur les modules de longueur finie établis dans II, p. 21 à 23.

Dans toute la suite de ce numéro, on considère une ensemble additif $\mathscr{C}$ de A-modules et une application additice $\varphi$ de $\mathscr{C}$ dans un groupe abélien G.

Soient E et $E'$ des modules de type $\mathscr{C}$; alors $E\oplus E'$ est de type $\mathscr{C}$, et il existe une suite exacte scindée (II, p. 20)

$$
0\longrightarrow E\longrightarrow E\oplus E'\longrightarrow E'\longrightarrow 0
$$

on en déduit

$$
\varphi (E\oplus E') =\varphi (E) +\varphi (E') \tag{1}
$$

En particulier, on a $\varphi (0) = 0$.

#### Proposition 1 {#alg-viii-s11-prop-1 .statement tag=00CY}

On suppose que $\mathscr{C}$ est héréditaire. Soient E et F des A-modules et $u: E\rightarrow F$une application linéaire.

a) Si E ou F est de type $\mathscr{C}$, il en est de même de l’image de $u$.

b) Si E est de type $\mathscr{C}$, il en est de même du noyau de $u$ et l’on a

(2) $\varphi (E) =\varphi$(Ker $u) +\varphi$(Im $u)$.

c) Si F est de type $\mathscr{C}$, il en est de même du conoyau de $u$, et l’on a

(3) $\varphi (F) =\varphi$(Im $u) +\varphi$(Coker $u)$.

La proposition résulte de l’existence de suites exactes

$0\longrightarrow$ Ker $u\longrightarrow E\longrightarrow$ Im $u\longrightarrow 0$

$0\longrightarrow$ Im $u\longrightarrow F\longrightarrow$ Coker $u\longrightarrow 0$.

#### Corollaire {#alg-viii-s11-n1-cor-1 .statement tag=00CZ}

Soit $(E_i)_{0\leqslant i\leqslant n}$ une suite finie de modules de type $\mathscr{C}$. S’il existe une suite exacte

0 // $E_0^{u_0}$ // $E_1^{u_1}$ /$/. .$. // $E_{n-1}^{u_{n-1}}/$/ $E_n$ // $0$,

on a

$$
\sum_{i=0}^n(-1)^i\varphi (E_i) = 0 \tag{4}
$$

Prouvons le corollaire par récurrence sur $n$, les cas $n= 0$ et $n= 1$ étant triviaux. Soit donc $n\geqslant 1$ et soit

$$
0\longrightarrow E_0\longrightarrow^{u_0}E_1\longrightarrow^{u_1}. . .\longrightarrow E_{n-1}\longrightarrow^{u_{n-1}}E_n\longrightarrow^{u_n}E_{n+1}\longrightarrow 0
$$

une suite exacte de modules de type $\mathscr{C}$. D’après la prop. 1, le noyau F de $u_n$ est un module de type $\mathscr{C}$ et l’on a

$$
\varphi (F) =\varphi (E_n)-\varphi (E_{n+1}) \tag{5}
$$

Par ailleurs, on a une suite exacte

$$
0\longrightarrow E_0\longrightarrow E_1\longrightarrow E_2\longrightarrow . . .\longrightarrow E_{n-1}\longrightarrow F\longrightarrow 0
$$

et l’hypothèse de récurrence fournit la relation

$$
n\sum_{i=0}^{-1}(-1)^i\varphi (E_i) + (-1)^n\varphi (F) = 0 \tag{6}
$$

De (5) et (6), on tire aussitôt $\sum^{n+1}_{i=0}(-1)^i\varphi (E_i) = 0$ et le corollaire en résulte.

#### Proposition 2 {#alg-viii-s11-prop-2 .statement tag=00D0}

Supposons que l’ensemble $\mathscr{C}$ soit héréditaire. Soit E un A-module et soient M et N des sous-modules de E.

a) Si les modules M et N sont de type $\mathscr{C}$, il en est de même des modules $M\cap N$ et M + N, et l’on a

$$
\varphi (M + N) +\varphi (M\cap N) =\varphi (M) +\varphi (N)
$$

b) Si les modules $E/M$et $E/N$sont de type $\mathscr{C}$, il en est de même des modules $E/(M\cap N)$et $E/(M + N)$et l’on a

$$
\varphi (E/(M + N)) +\varphi (E/(M\cap N)) =\varphi (E/M) +\varphi (E/N)
$$

Les assertions a) et b) résultent de l’existence des suites exactes (II, p. 17, prop. 10)

$$
0\rightarrow M\cap N\rightarrow M\oplus N\rightarrow M + N\rightarrow 0
$$

et

$$
0\rightarrow E/(M\cap N)\rightarrow (E/M)\oplus (E/N)\rightarrow E/(M + N)\rightarrow 0
$$

#### Proposition 3 {#alg-viii-s11-prop-3 .statement tag=00D1}

Supposons $\mathscr{C}$ héréditaire. Soient E un module de type $\mathscr{C}$ et $(E_i)_{0\leqslant i\leqslant n}$ une suite de composition de E (I, p. 39). Pour $1\leqslant i\leqslant n$, le module $E_{i-1}/E_i$ est de type $\mathscr{C}$ et l’on a

$$
\varphi (E) =\sum_{i=1}^n\varphi (E_{i-1}/E_i)
$$

Comme $\mathscr{C}$ est héréditaire, les modules $E_0/E_1$ et $E_1$ sont de type $\mathscr{C}$ et l’on a $\varphi (E) =\varphi (E_0/E_1)+\varphi (E_1)$. Comme la suite $(E_{i+1})_{0\leqslant i\leqslant n-1}$ est une suite de composition de $E_1$, la prop. 3 se démontre par récurrence sur $n$.

### 2. Groupe de Grothendieck d’un ensemble additif de modules

Soit A un anneau. Dans ce numéro, on considère un ensemble additif $\mathscr{C}$ de classes de A-modules ; on identifie $\mathscr{C}$ à la base canonique du groupe commutatif libre $\mathbf{Z}^{(\mathscr{C})}$. Pour toute suite exacte

$$
(\mathscr{E})0\longrightarrow E'\longrightarrow E\longrightarrow E''\longrightarrow 0
$$

de modules de type $\mathscr{C}$, on note $r_{\mathscr{E}}$ l’élément cl(E) $-$ cl(E$')-$ cl(E$'')$ de $\mathbf{Z}^{(\mathscr{C})}$. Soit R le sous-groupe de $\mathbf{Z}^{(\mathscr{C})}$ engendré par les éléments de la forme $r_{\mathscr{E}}$; le groupe quotient $\mathbf{Z}^{(\mathscr{C})}/R$ s’appelle le groupe de Grothendieck de $\mathscr{C}$ et se note $K(\mathscr{C})$. Pour tout module E de type $\mathscr{C}$, on note $[E]_{\mathscr{C}}$ (ou parfois [E] lorsqu’il n’y a pas d’ambiguïté sur $\mathscr{C})$ l’image de cl(E) dans $K(\mathscr{C})$. On a alors la propriété universelle suivante :

#### Proposition 4 {#alg-viii-s11-prop-4 .statement tag=00D2}

a) L’application $E\rightarrow [E]_{\mathscr{C}}$ de $\mathscr{C}$ dans $K(\mathscr{C})$est additive.

b) Soit G un groupe commutatif et soit $\varphi :\mathscr{C}\rightarrow G$une fonction additive de modules. Il existe un homomorphisme $u: K(\mathscr{C})\rightarrow G$et un seul, tel que l’on ait $\varphi (E) =u([E]_{\mathscr{C}})$pour tout module E de type $\mathscr{C}$.

L’assertion a) est évidente. Prouvons b). Il existe un homomorphisme $u': \mathbf{Z}^{(\mathscr{C})}\rightarrow G$ qui prolonge $\varphi$. Comme $\varphi$ est additive, on a $u'(r_{\mathscr{E}}) = 0$ pour toute suite exacte $(\mathscr{E})$ de modules de type $\mathscr{C}$, donc R est contenu dans le noyau de $u'$. Par suite $u'$ définit par passage au quotient un homomorphisme $u$ de $K(\mathscr{C})$ dans G et il est clair qu’on a $\varphi (E) =u([E]_{\mathscr{C}})$ pour tout A-module de type $\mathscr{C}$. Le groupe $K(\mathscr{C})$ est engendré par l’ensemble des éléments $[E]_{\mathscr{C}}$ pour E parcourant $\mathscr{C}$, d’où l’unicité de $u$.

Soient $\mathscr{C}$ et $\mathscr{D}$ des ensembles additifs de classes de A-modules tels que $\mathscr{C}\subset \mathscr{D}$. L’application $E\rightarrow [E]_{\mathscr{D}}$ de $\mathscr{C}$ dans le groupe de Grothendieck $K(\mathscr{D})$ étant additive, il existe un homomorphisme $\gamma_{\mathscr{D},\mathscr{C}}: K(\mathscr{C})\rightarrow K(\mathscr{D})$, dit canonique, caractérisé par la formule $\gamma_{\mathscr{D},\mathscr{C}}([E]_{\mathscr{C}}) = [E]_{\mathscr{D}}$ pour tout module E de type $\mathscr{C}$. Il n’est pas toujours injectif (VIII, p. 205, exerc. 13).

#### Exemple {#alg-viii-s11-n2-exa-1 .statement tag=00D3}

$*$Soient A un anneau commutatif noethérien et Σ son spectre. Pour tout entier $n\geqslant 0$, notons $\mathscr{C}^{\geqslant n}$ l’ensemble des classes de A-modules de type fini dont le support est de codimension $\geqslant n$ dans Σ. Posons $K(n,A) = K(\mathscr{C}^{\geqslant n})$ et $\gamma_n=\gamma_{\mathscr{C}^{\geqslant n},\mathscr{C}^{\geqslant n+1}}$. On a donc une suite d’homomorphismes

$$
\gamma_n: K(n+ 1,A)\longrightarrow K(n,A)
$$

On peut démontrer (AC, VIII, p. 13, prop. 10) que dans $K(n,A)$, les éléments $[A/\mathfrak{p}]_{\mathscr{C}_n}$, où $\mathfrak{p}$ parcourt l’ensemble des éléments de Σ de hauteur $n$, forment une base d’un $\mathbf{Z}$-module supplémentaire de l’image de $\gamma_n$. Plus précisément, pour tout module E de type $\mathscr{C}^{\geqslant n}$, on a

$[E]_{\mathscr{C}^{\geqslant n}}\equiv \sum$ long$_{A_{\mathfrak{p}}}(E_{\mathfrak{p}})\cdot [A/\mathfrak{p}]_{\mathscr{C}^{\geqslant n}}$ (mod. Im$\gamma_n).*$

$\{\mathfrak{p}\in \Sigma |$ht($\mathfrak{p}$)$=n\}$

Le groupe $K(\mathscr{C})$ est engendré par les éléments de la forme $[E]_{\mathscr{C}}$ (avec $E\in \mathscr{C})$ et l’on a $[E\oplus E']_{\mathscr{C}}= [E]_{\mathscr{C}}+ [E']_{\mathscr{C}}$ d’après la formule (1) (VIII, p. 180) ; tout élément de $K(\mathscr{C})$ est donc de la forme $[E]_{\mathscr{C}}-[F]_{\mathscr{C}}$, où E et F appartiennent à $\mathscr{C}$.

Un élément de $K(\mathscr{C})$ est dit effectif s’il est de la forme $[E]_{\mathscr{C}}$ pour un A-module E de type $\mathscr{C}$. L’ensemble des éléments effectifs de $K(\mathscr{C})$ se note $K(\mathscr{C})^+$; c’est un sous-monoïde de $K(\mathscr{C})$ et $K(\mathscr{C})$ s’identifie au groupe des différences de $K(\mathscr{C})^+$ (I, p. 19).

#### Proposition 5 {#alg-viii-s11-prop-5 .statement tag=00D4}

Soient E et F des modules de type $\mathscr{C}$. Pour que l’on ait l’égalité $[E]_{\mathscr{C}}= [F]_{\mathscr{C}}$, il faut et il suffit qu’il existe des suites exactes de modules de type $\mathscr{C}$ $(\mathscr{E})0\longrightarrow L\longrightarrow P\longrightarrow M\longrightarrow 0$

$$
(\mathscr{F})0\longrightarrow L\longrightarrow Q\longrightarrow M\longrightarrow 0
$$

telles que $E\oplus Q$soit isomorphe à $F\oplus P$.

La condition énoncée est suffisante, car elle entraîne les relations

$$
[P]_{\mathscr{C}}= [L]_{\mathscr{C}}+ [M]_{\mathscr{C}},[Q]_{\mathscr{C}}= [L]_{\mathscr{C}}+ [M]_{\mathscr{C}},[E]_{\mathscr{C}}+ [Q]_{\mathscr{C}}= [F]_{\mathscr{C}}+ [P]_{\mathscr{C}}
$$

d’où $[E]_{\mathscr{C}}= [F]_{\mathscr{C}}$.

Supposons maintenant que l’on ait $[E]_{\mathscr{C}}= [F]_{\mathscr{C}}$. D’après la construction du groupe $K(\mathscr{C})$, il existe deux familles finies de suites exactes de modules de type $\mathscr{C}$ $(\mathscr{G}_i)0\longrightarrow G'_i\longrightarrow G_i\longrightarrow G''_i\longrightarrow 0$

pour $i\in I$ et

$$
(\mathscr{H}_j)0\longrightarrow H'_j\longrightarrow H_j\longrightarrow H''_j\longrightarrow 0
$$

pour $j\in J$, telles que l’on ait dans $\mathbf{Z}^{(\mathscr{C})}$

cl(E) $-$ cl(F) $=\sum_{j\in J}r_{\mathscr{H}_j}-\sum_{i\in I}r_{\mathscr{G}_i}$.

Plus explicitement, cette relation s’écrit

(7) cl(E) $+\sum_{i\in I}$ cl(G$_i) +\sum_{j\in J}$ cl(H$'_j) +\sum_{j\in J}$ cl(H$''_j)$

= cl(F) $+\sum_{i\in I}$ cl(G$'_i) +\sum_{i\in I}$ cl(G$''_i) +\sum_{j\in J}$ cl(H$_j)$. Posons $G =\bigoplus_{i\in I}G_i, G'=\bigoplus_{i\in I}G'_i$, etc. Par passage aux sommes directes, on construit des suites exactes

$(\mathscr{G})$ 0 // $G'^p$ // G $^q$ // $G''$ // 0

$(\mathscr{H})$ 0 // $H'^r$ // H $^s$ // $H''$ // 0

formées de modules de type $\mathscr{C}$.

Par ailleurs, soient $M_1, . . . ,M_m,N_1, . . . ,N_n$ des A-modules de type $\mathscr{C}$. Si l’on a $\sum^m_{i=1}$ cl(M$_i) =\sum^n_{j=1}$ cl(N$_j)$ dans le groupe $\mathbf{Z}^{(\mathscr{C})}$, on a $m=n$ et il existe une permutation $\sigma \in \mathfrak{S}_m$ telle que cl(M$_i) =$ cl(N$_{\sigma(i)})$ pour tout $1\leqslant i\leqslant m$ (I, p. 90, prop. 11) ; par suite, les modules $\oplus^m_{i=1}M_i$ et $\oplus^n_{j=1}N_j$ sont isomorphes. En particulier, on déduit de (7) l’existence d’un isomorphisme de $E\oplus Q$ sur $F\oplus P$, où l’on a posé

$$
P = G'\oplus G''\oplus H,Q = G\oplus H'\oplus H''
$$

On pose aussi

$$
L = G'\oplus H',M = G''\oplus H''
$$

Les modules L, M, P, Q sont de type $\mathscr{C}$ et la suite

$(\mathscr{E})$ 0 // L $^{\lambda}$ // P $^{\mu}$ // M // $0$,

où l’on définit $\lambda$ et $\mu$ par

$$
\lambda (g', h') = (g',0, r(h')),\mu (g', g'', h) = (g'', s(h))
$$

est exacte. On construit de manière analogue une suite exacte

$$
(\mathscr{F})0\longrightarrow L\longrightarrow Q\longrightarrow M\longrightarrow 0
$$

ce qui conclut la démonstration.

Pour la loi de composition $(E,E')\rightarrow$ cl(E $\oplus E')$, l’ensemble $\mathscr{C}$ est un monoïde commutatif. On note parfois $K'(\mathscr{C})$ le groupe des différences du monoïde commutatif $\mathscr{C}$ (I, p. 19), et on l’appelle le groupe de Grothendieck de $\mathscr{C}$ pour les sommes directes. Pour tout module E de type $\mathscr{C}$, on note $[E]'_{\mathscr{C}}$ l’image de cl(E) dans $K'(\mathscr{C})$.

#### Proposition 6 {#alg-viii-s11-prop-6 .statement tag=00D5}

a) L’application $E\rightarrow [E]'_{\mathscr{C}}$ de $\mathscr{C}$ dans $K'(\mathscr{C})$est une fonction faiblement additive de modules.

b) Soit G un groupe commutatif et soit $\varphi :\mathscr{C}\rightarrow G$une fonction faiblement additive de modules. Il existe un homomorphisme de groupes $u: K'(\mathscr{C})\rightarrow G$, et un seul, tel que l’on ait $\varphi (E) =u([E]'_{\mathscr{C}})$pour tout module E de type $\mathscr{C}$.

c) Soient E et F des modules de type $\mathscr{C}$. Pour que l’on ait $[E]'_{\mathscr{C}}= [F]'_{\mathscr{C}}$ il faut et il suffit qu’il existe un module M de type $\mathscr{C}$ tel que $E\oplus M$soit isomorphe à $F\oplus M$.

L’assertion a) est évidente. L’assertion b) résulte de (I, p. 18, th. 1) et l’assertion c) de (I, p. 18, prop. 6).

Comme l’application $E\rightarrow [E]_{\mathscr{C}}$ de $\mathscr{C}$ dans $K(\mathscr{C})$ est une fonction faiblement additive de modules, on en déduit un homomorphisme $u: K'(\mathscr{C})\rightarrow K(\mathscr{C})$. Cet homomorphisme est surjectif mais n’est pas toujours un isomorphisme (VIII, p. 187, remarque 2).

Soit $R'$ le sous-groupe de $\mathbf{Z}^{(\mathscr{C})}$ engendré par les éléments de la forme $r_{\mathscr{E}}$, où $\mathscr{E}$ est une suite exacte scindée de A-modules de type $\mathscr{C}$, c’est-à-dire par les éléments de la forme cl(E$'\oplus E'')-$ cl(E$')-$ cl(E$'')$, où $E'$ et $E''$ sont des modules de type $\mathscr{C}$. L’application canonique de $\mathscr{C}$ dans le groupe quotient $\mathbf{Z}^{(\mathscr{C})}/R'$ se prolonge en un homomorphisme de groupes $v: K'(\mathscr{C})\rightarrow \mathbf{Z}^{(\mathscr{C})}/R'$. C’est un isomorphisme. En effet, l’application canonique de $\mathscr{C}$ dans $K'(\mathscr{C})$ se prolonge en un homomorphisme de groupes de $\mathbf{Z}^{(\mathscr{C})}$ dans $K'(\mathscr{C})$ dont le noyau contient $R'$, d’où par passage au quotient un homomorphisme $v': \mathbf{Z}^{(\mathscr{C})}/R'\rightarrow K'(\mathscr{C})$; il est clair que $v$ et $v'$ sont des bijections réciproques l’une de l’autre.

Un élément de $K'(\mathscr{C})$ est dit effectif s’il est de la forme $[E]'_{\mathscr{C}}$ pour un A-module E de type $\mathscr{C}$. L’ensemble des éléments effectifs de $K'(\mathscr{C})$ se note $K'(\mathscr{C})^+$.

### 3. Utilisation des suites de composition

Soit A un anneau. Soient E un A-module de longueur finie et S un A-module simple. D’après le théorème de Jordan-Hölder (I, p. 41, th. 6), le nombre des quotients d’une suite de Jordan-Hölder de E qui sont isomorphes à S est indépendant de la suite. On le note $\ell_S(E)$ et on l’appelle la multiplicité de S dans E. On appelle support du A-module E l’ensemble des classes de A-modules simples S telles que $\ell_S(E)\not= 0$. Lorsque E est semi-simple de longueur finie, l’entier $\ell_S(E)$ est la longueur [E : S] du composant isotypique de type S de E (VIII, p. 68), et la notion de support coïncide avec celle introduite en VIII, p. 62.

#### Lemme 1 {#alg-viii-s11-lem-1 .statement tag=00D6}

Soient E, $E'$ et $E''$ des A-modules de longueur finie et

0 // $E'^i$ // E $^p$ // $E''$ // 0

une suite exacte. On a $\ell_S(E) =\ell_S(E') +\ell_S(E'')$.

Soient $\Sigma '$ et $\Sigma ''$ des suites de Jordan-Hölder de $i(E')$ et de $E/i(E')$ respectivement ; il existe une suite de Jordan-Hölder Σ de E dont la suite des quotients s’obtient en juxtaposant la suite des quotients de Σ et celle de $\Sigma '$ (I, p. 42).

#### Proposition 7 {#alg-viii-s11-prop-7 .statement tag=00D7}

Soit $\mathscr{C}$ un ensemble héréditaire de classes de modules tel que tout module de type $\mathscr{C}$ soit de longueur finie. Soit $\mathscr{S}$ l’ensemble des classes de modules simples appartenant à $\mathscr{C}$. Alors la famille $([S]_{\mathscr{C}})_{S\in\mathscr{S}}$ est une base du $\mathbf{Z}$-module $K(\mathscr{C})$et l’on a

$$
[E]_{\mathscr{C}}=\sum_{S\in\mathscr{S}}\ell_S(E)[S]_{\mathscr{C}} \tag{8}
$$

pour tout module E de type $\mathscr{C}$.

La formule (8) résulte de la prop. 3 appliquée à une suite de Jordan-Hölder de E. D’après le lemme 1, il existe pour tout élément S de $\mathscr{S}$ une application $\mathbf{Z}$-linéaire $\varphi_S$ de $K(\mathscr{C})$ dans $\mathbf{Z}$telle que $\varphi_S([E]_{\mathscr{C}}) =\ell_S(E)$ pour tout module E de type $\mathscr{C}$. En particulier, on a $\varphi_S([S]_{\mathscr{C}}) = 1$ et $\varphi_S([S']_{\mathscr{C}}) = 0$ pour tout $S'\not= S$ dans $\mathscr{S}$. Il en résulte que les éléments de la forme $[S]_{\mathscr{C}}$ (pour $S\in \mathscr{S})$ sont linéairement indépendants sur $\mathbf{Z}$; ces éléments engendrent $K(\mathscr{C})$ d’après la formule (8).

#### Corollaire {#alg-viii-s11-n3-cor-1 .statement tag=00D8}

Soient E et F des modules semi-simples de type $\mathscr{C}$. Pour que E soit isomorphe à F, il faut et il suffit que l’on ait $[E]_{\mathscr{C}}= [F]_{\mathscr{C}}$ dans $K(\mathscr{C})$.

En effet, on a $[E]_{\mathscr{C}}=\sum_{S\in\mathscr{S}}\ell_S(E)[S]_{\mathscr{C}}$ et une formule analogue pour F, et E est isomorphe à F si et seulement si l’on a $\ell_S(E) =\ell_S(F)$ pour tout $S\in \mathscr{S}$ (VIII, p. 68).

#### Remarque {#alg-viii-s11-n3-rem-1 .statement tag=00D9}

L’ensemble $K(\mathscr{C})^+$ est le sous-monoïde de $K(\mathscr{C})$ engendré par la famille $([S]_{\mathscr{C}})_{S\in\mathscr{S}}$.

### 4. Le groupe de Grothendieck R(A)

Soit A un anneau. Soit $\mathscr{F}(A)$ l’ensemble des classes de A-modules de type fini (VIII, p. 47) ; les classes des A-modules de longueur finie forment un sous-ensemble $\mathscr{L}\mathscr{F}(A)$ de $\mathscr{F}(A)$; on a vu que $\mathscr{L}\mathscr{F}(A)$ est un ensemble héréditaire de classes de modules. On note R(A) le groupe de Grothendieck associé à $\mathscr{L}\mathscr{F}$(A), et [E] l’image dans R(A) de la classe d’un A-module E de longueur finie.

Les résultats du numéro 3 entraînent ce qui suit :

a) Soit $\mathscr{S}(A)$ l’ensemble des classes de A-modules simples. La famille $([S])_{S\in\mathscr{S}(A)}$ est une base du $\mathbf{Z}$-module R(A).

b) Soient E et F des A-modules semi-simples de longueur finie. Pour que E et F soient isomorphes, il faut et il suffit que l’on ait [E] = [F] dans R(A).

c) Soient E un A-module de longueur finie, et $(E_i)_{0\leqslant i\leqslant n}$ une suite de JordanHölder de E. Posons $F =\bigoplus^n_{i=1}(E_{i-1}/E_i)$. Alors F est un A-module semi-simple de longueur finie, et l’on a [E] = [F] dans R(A).

d) Soit $\ell : R(A)\rightarrow \mathbf{Z}$l’homomorphisme caractérisé par $\ell ([S]) = 1$ pour tout A-module simple S. On a alors $\ell ([E]) =\sum_{S\in\mathscr{S}(A)}\ell_S(E) =$ long$_A(E)$ pour tout A-module E de longueur finie.

Si D est un corps, l’homomorphisme $\ell : R(D)\rightarrow \mathbf{Z}$est un isomorphisme.

#### Remarque 1 {#alg-viii-s11-n4-rem-1 .statement tag=00DA}

Soit $\mathscr{S}\mathscr{S}(A)$ l’ensemble héréditaire des classes de A-modules semi-simples de longueur finie. D’après la prop. 7 de VIII, p. 186, le groupe de Grothendieck $K(\mathscr{S}\mathscr{S}(A))$ est un $\mathbf{Z}$-module libre dont les éléments $[S]_{\mathscr{S}\mathscr{S}(A)}$, pour $S\in \mathscr{S}$ (A), forment une base. L’homomorphisme canonique $\gamma_{\mathscr{L}\mathscr{F}(A),\mathscr{S}\mathscr{S}(A)}$ (VIII, p. 182) est donc un isomorphisme.

#### Remarque 2 {#alg-viii-s11-n4-rem-2 .statement tag=00DB}

Soit $K'(\mathscr{L}\mathscr{F}(A))$ le groupe de Grothendieck de $\mathscr{L}\mathscr{F}(A)$ pour les sommes directes (VIII, p. 184). Le théorème de Krull-Remak-Schmidt (VIII, p. 34) entraîne que $K'(\mathscr{L}\mathscr{F}(A))$ est un $\mathbf{Z}$-module libre ayant pour base l’ensemble des classes de A-modules indécomposables de longueur finie, alors que $K(\mathscr{L}\mathscr{F}(A))$ admet pour base l’ensemble des classes de A-modules simples.

#### Remarque 3 {#alg-viii-s11-n4-rem-3 .statement tag=00DC}

Soit E un A module de longueur finie. Il existe un A-module semi-simple de longueur finie $E'$ tel que $[E] = [E']$ d’après c) et un tel module est défini à un isomorphisme près d’après b) ; on l’appelle parfois un semi-simplifié de E.

#### Proposition 8 {#alg-viii-s11-prop-8 .statement tag=00DD}

Soit A un anneau principal qui n’est pas un corps et soit L son corps des fractions. Il existe un isomorphisme $\varphi : R(A)\rightarrow L^*/A^*$ tel que l’on ait

$$
\varphi ([A/aA]) =aA^* \tag{9}
$$

pour tout $a\not= 0$dans A.

Soit P un système représentatif d’éléments extrémaux de A (VII, p. 3). Les idéaux maximaux de A sont les idéaux $pA$ pour $p\in P$; tout A-module simple est donc isomorphe à un module $A/pA$ et un seul. De plus (VII, p. 3, th. 2), le groupe commutatif $L^*/A^*$ est libre et admet pour base la famille $(pA^*)_{p\in P}$. Il existe donc un isomorphisme $\varphi$ de R(A) sur $L^*/A^*$ caractérisé par $\varphi ([A/pA]) =pA^*$ pour tout $p\in P$.

Soit $a\not= 0$ dans A. Il existe un entier $r\geqslant 0$, des éléments $p_1, . . . , p_r$ de P et un élément $u$ de $A^*$ tels qu’on ait $a=up_1. . . p_r$. Le module $A/aA$ admet la suite de composition définie par

$$
E_0= A/aA,E_i= (p_1. . . p_iA)/aA(1\leqslant i\leqslant r)
$$

et le module $E_{i-1}/E_i= (p_1. . . p_{i-1}A)/(p_1. . . p_iA)$ est isomorphe à $A/p_iA$; on a donc (VIII, p. 181, prop. 3)

$$
\varphi ([A/aA]) =\sum_{i=1}^r\varphi ([A/p_iA]) =p_1. . . p_rA^*=aA^*
$$

#### Remarque 4 {#alg-viii-s11-n4-rem-4 .statement tag=00DE}

Conservons les hypothèses et les notations de la prop. 8. Soient E un A-module de longueur finie et $a_1A, . . . , a_nA$ ses facteurs invariants (VII, p.20). Comme E est isomorphe à $\bigoplus^n_{i=1}A/a_iA$, on a

$$
\varphi ([E]) =\sum_{i=1}^n\varphi ([A/a_iA]) =a_1. . . a_nA^* \tag{10}
$$

#### Remarque 5 {#alg-viii-s11-n4-rem-5 .statement tag=00SI}

Soit A un anneau de Dedekind qui n’est pas un corps (AC, VII, § 2, n$_{\circ}1)$.

En raisonnant comme dans la prop. 8, on prouve l’existence d’un isomorphisme $\varphi$ de R(A) sur le groupe des idéaux fractionnaires de A, caractérisé par $\varphi ([A/\mathfrak{a}]) =\mathfrak{a}$ pour tout idéal non nul $\mathfrak{a}$ de $A.*$

La prop. 8 sera utilisée par exemple dans les deux cas suivants :

a) Supposons qu’on ait $A = \mathbf{Z}$. Les $\mathbf{Z}$-modules de longueur finie ne sont autres que les groupes commutatifs finis. Comme $\mathbf{Q}^*$ est produit direct de $\mathbf{Z}^*=\{1,-1\}$ et de $\mathbf{Q}^*_+$, on déduit de la prop. 8 un isomorphisme $\varphi '$ de $R(\mathbf{Z})$ sur $\mathbf{Q}^*_+$ caractérisé par

$\varphi '([G]) =$ Card(G)

pour tout groupe commutatif fini G.

b) Supposons que A soit l’anneau K[T] des polynômes en une indéterminée T à coefficients dans un corps commutatif K. Soient E un espace vectoriel de dimension finie sur K, et $u$ un endomorphisme de E. Comme en VII, p. 28, notons $E_u$ le A-module ayant E comme groupe additif sous-jacent, et pour loi d’action $(p, x)\rightarrow p(u)x$. Le A-module $E_u$ est de longueur finie. Inversement, tout A-module simple est de dimension finie sur K (VII, p. 25, remarque 4). Par conséquent, tout A-module de longueur finie est de dimension finie sur K, donc de la forme $E_u$. De plus (VII, p. 33, cor. 1), le produit des facteurs invariants de $E_u$ est égal au polynôme caractéristique $\chi_u$ de $u$. Par suite, la prop. 8 fournit un isomorphisme

$$
\varphi : R(K[T])\rightarrow K(T)^*/K^*
$$

caractérisé par $\varphi ([E_u]) =\chi_uK^*($cf. formule (10)).

### 5. Changement d’anneaux

Soient A et B des anneaux et soit $f: A\rightarrow B$ un homomorphisme d’anneaux. Soient $\mathscr{C}$ un ensemble additif de A-modules et $\mathscr{D}$ un ensemble additif de B-modules.

Supposons tout d’abord que pour tout B-module M de type $\mathscr{D}$, le A-module $f_*(M)$ obtenu par restriction à A de l’anneau des scalaires soit de type $\mathscr{C}$. Alors l’application de $\mathscr{D}$ dans $K(\mathscr{C})$ qui à M associe $[f_*(M)]_{\mathscr{C}}$ est une fonction additive de modules ; on en déduit un homomorphisme de groupes

$$
f_*: K(\mathscr{D})\longrightarrow K(\mathscr{C})
$$

On définit de même un homomorphisme de groupes $f_*: K'(\mathscr{D})\rightarrow K'(\mathscr{C})$.

On suppose maintenant que, pour tout A-module E de type $\mathscr{C}$, le B-module $f^*(E)$ déduit de E par extension des scalaires au moyen de $f$ (II, p. 82) est de type $\mathscr{D}$. L’application de $\mathscr{C}$ dans $K'(\mathscr{D})$ qui envoie un élément E de $\mathscr{C}$ sur $[f^*(E)]'_{\mathscr{D}}$ est une fonction faiblement additive de modules, elle induit donc un homomorphisme de groupes $f^*: K'(\mathscr{C})\rightarrow K'(\mathscr{D})$.

Supposons en outre que, pour toute suite exacte

$$
0\longrightarrow E'\longrightarrow E\longrightarrow E''\longrightarrow 0
$$

de A-modules de type $\mathscr{C}$, la suite de B-modules de type $\mathscr{D}$

$$
0\longrightarrow B\otimes_AE'\longrightarrow B\otimes_AE\longrightarrow B\otimes_AE''\longrightarrow 0
$$

soit exacte. C’est en particulier vérifié dans les cas suivants :

a) L’homomorphisme $f$ fait de B un A-module projectif (II, p. 58, prop. 5 et II, p. 63, cor. $6)*$ou, plus généralement, plat (X, p. 8, définition $1)*$;

b) $*$L’ensemble $\mathscr{C}$ est un ensemble de classes de A-modules projectifs ou, plus

généralement, plats (X, p. 72, cor. $2)*$.

L’application de $\mathscr{C}$ dans $K(\mathscr{D})$ qui à E associe $[f^*(E)]_{\mathscr{D}}$ est alors additive. On en déduit donc un homomorphisme de groupes $f^*: K(\mathscr{C})\rightarrow K(\mathscr{D})$.

### 6. Le groupe de Grothendieck $R_K(A)$

Soient K un corps commutatif et A une K-algèbre. L’ensemble des classes des A-modules qui sont des espaces vectoriels de dimension finie sur K est héréditaire. Le groupe de Grothendieck correspondant se note $R_K(A)$. C’est un $\mathbf{Z}$-module libre ayant pour base la famille $([S])_{S\in\mathscr{S}}$, où $\mathscr{S}$ est l’ensemble des classes des A-modules simples qui sont de dimension finie sur K. Il existe un homomorphisme

dim$: R_K(A)\longrightarrow \mathbf{Z}$

caractérisé par dim([E]) = [E : K] pour tout A-module E de dimension finie sur K. Lorsque A = K, c’est un isomorphisme. Le sous-monoïde des éléments effectifs est noté $R_K(A)^+$.

#### Lemme 2 {#alg-viii-s11-lem-2 .statement tag=00DF}

Soient M, $M'$ des A-modules qui sont des espaces vectoriels de dimension finie sur K. Pour que les supports (VIII, p. 185) de M et $M'$ soient disjoints, il faut et il suffit qu’il existe $a\in A$tel que $a_M= 0$et $a_{M'}= 1$.

Supposons qu’il existe $a\in A$ tel que $a_M= 0$ et $a_{M'}= 1$. Soit S un A-module simple. Si cl(S) appartient au support $\mathscr{S}_M$ de M, le A-module S est isomorphe à l’un des quotients d’une suite de Jordan-Hölder de M et l’on a $a_S= 0$. De même, si cl(S) appartient au support $\mathscr{S}_{M'}$ de $M'$, on a $a_S= 1$. Il en résulte que $\mathscr{S}_M$ et $\mathscr{S}_{M'}$ sont disjoints.

Inversement, supposons que les ensembles $\mathscr{S}_M$ et $\mathscr{S}_{M'}$ soient disjoints. Il sont finis car M et $M'$ sont de dimension finie sur K. Tout A-module simple S dont la classe appartient à $\mathscr{S}_M\cup \mathscr{S}_{M'}$ est de dimension finie sur K et a fortiori sur le corps End$_A(S)$. D’après le cor. 1 de la prop. 4 (VIII, p. 79), il existe un élément $b\in A$ tel que l’on ait $b_S= 0$ pour tout A-module simple S dont la classe appartient à $\mathscr{S}_M$ et $b_S= 1$ pour tout A-module simple S dont la classe appartient à $\mathscr{S}_{M'}$. Soit $(M_i)_{0\leqslant i\leqslant n}$ une suite de Jordan-Hölder de M. On a d’après ce qui précède $bM_i\subset M_{i+1}$ pour $0\leqslant i < n$, d’où $(b^n)_M= 0$. On démontre de même l’existence d’un entier naturel $m$ tel que $((1-b)^m)_{M'}= 0$. Posons $P(X) = 1-(1-X^n)^m$ et $a= P(b)$. Le polynôme P(X) est multiple de $X^n$, donc on a $a_M= 0$; le polynôme $1-P(X)$ est multiple de $(1-X)^m$, donc on a $a_{M'}= 1$. Cela termine la démonstration.

Soit L une extension de K. Si M est un A-module qui est de dimension finie sur $K, M_{(L)}$ est un $A_{(L)}$-module qui est de dimension finie sur L. De plus pour toute suite exacte

$$
0\longrightarrow M'\longrightarrow M\longrightarrow M''\longrightarrow 0
$$

de A-modules, la suite de $A_{(L)}$-modules

$$
0\longrightarrow M'_{(L)}\longrightarrow M_{(L)}\longrightarrow M''_{(L)}\longrightarrow 0
$$

qui s’en déduit par extension des scalaires est exacte (II, p. 108, prop. 14). Il existe donc un unique homomorphisme $u: R_K(A)\rightarrow R_L(A_{(L)})$ tel que $u([M]) = [M_{(L)}]$ pour tout A-module M qui est de dimension finie sur K (VIII, p. 189).

#### Théorème 1 {#alg-viii-s11-thm-1 .statement tag=00DG}

L’homomorphisme $u: R_K(A)\rightarrow R_L(A_{(L)})$défini ci-dessus est injectif. Soit $\xi$ un élément de $R_K(A)$. Pour que $\xi$ soit effectif il faut et il suffit que $u(\xi )$le soit.

#### Lemme 3 {#alg-viii-s11-lem-3 .statement tag=00DH}

Soient S et T deux A-modules simples, de dimension finie sur K, non isomorphes. Les supports des $A_{(L)}$-modules $S_{(L)}$ et $T_{(L)}$ sont disjoints.

D’après le lemme 2, il existe un élément $a\in A$ tel que $a_S= 0$ et $a_T= 1$. L’élément $1\otimes a$ de $A_{(L)}$ opère comme 0 sur $S_{(L)}$ et comme 1 sur $T_{(L)}$. D’après le lemme 2, les supports des $A_{(L)}$-modules $S_{(L)}$ et $T_{(L)}$ sont disjoints.

Démontrons le th. 1. Soit $\mathscr{S}$ l’ensemble des classes de A-modules simples qui sont de dimension finie sur K. La famille $([S])_{S\in\mathscr{S}}$ est une base du $\mathbf{Z}$-module $R_K(A)$. Soit $S\in \mathscr{S}$. Le $A_{(L)}$-module $S_{(L)}$ n’est pas nul, donc son support n’est pas vide. Soit $S'$ un élément de ce support. D’après le lemme 1 de VIII, p. 185, il existe un homomorphisme $f_{S'}: R_L(A_{(L)})\rightarrow \mathbf{Z}$tel que $f_{S'}([E]) =\ell_{S'}(E)$ pour tout $A_{(L)}$-module E qui est de dimension finie sur L. On a $f_{S'}([S_{(L)}])\not= 0$ par construction et $f([T_{(L)}]) = 0$ pour tout $T\in \mathscr{S}-\{S\}$ d’après le lemme 3. Nous avons ainsi prouvé que les éléments de $R_L(A_{(L)})$ de la forme $[S_{(L)}]$, pour $S\in \mathscr{S}$, sont linéairement indépendants sur $\mathbf{Z}$. Il en résulte que l’homomorphisme $u$ est injectif.

Soit $S\in \mathscr{S}$ et soit $S'$ un élément du support de $S_{(L)}$. Pour tout $\xi \in R_K$(A), la coordonnée de $\xi$ d’indice [S] dans la base $([S])_{S\in\mathscr{S}}$ est $f_{S'}(u(\xi ))/[S_{(L)}: S']$. Il en résulte que si $u(\xi )$ est effectif, $\xi$ l’est également.

### 7. Structure multiplicative dans $K(\mathscr{C})$

Soient K un anneau commutatif et A une bigèbre sur l’anneau K (III, p. 148), de coproduit $c$ et de coünité $\gamma$. Sauf mention du contraire, les produits tensoriels sont relatifs à K. Soient E et F des A-modules (à gauche). Le produit tensoriel $E\otimes F$ est muni d’une structure de $(A\otimes$ A)-module caractérisée par la formule

$$
(a\otimes b)(x\otimes y) =ax\otimes by \tag{11}
$$

pour $a, b\in A,x\in E$ et $y\in F$. Au moyen de l’homomorphisme $c: A\rightarrow A\otimes A$, on déduit de ce $(A\otimes$ A)-module un A-module $c_*(E\otimes F)$ (II, p. 30). Plus explicitement, soit $a\in A$; si $c(a) =\sum_ia_i\otimes b_i$, on a

$$
a(x\otimes y) =\sum_ia_ix\otimes b_iy \tag{12}
$$

pour $x\in E$ et $y\in F$. Par abus, on notera encore $E\otimes F$ le A-module ainsi obtenu. On déduit aussitôt de la coassociativité de $c$ que l’isomorphisme canonique de K-modules

$$
\varphi : (E\otimes F)\otimes G\longrightarrow E\otimes (F\otimes G)
$$

est A-linéaire, quels que soient les A-modules E, F et G. De même, si la bigèbre A est cocommutative, l’isomorphisme canonique de $E\otimes F$ sur $F\otimes E$ est A-linéaire. Enfin, soit $K_{\gamma}$ le A-module ayant K pour groupe sous-jacent, avec la loi externe $(a, x)\rightarrow \gamma (a)x$; l’isomophisme canonique de $K\otimes E$ (resp. $E\otimes K)$ sur E est un isomorphisme de A-modules de $K_{\gamma}\otimes E$ (resp. $E\otimes K_{\gamma})$ sur E.

#### Proposition 9 {#alg-viii-s11-prop-9 .statement tag=00DI}

Soient K un anneau commutatif, A une bigèbre sur K de coünité $\gamma$, et $\mathscr{C}$ un ensemble additif de classes de A-modules possédant les propriétés suivantes :

(i) Tout A-module de type $\mathscr{C}$ est un K-module projectif $(*$ou plus généralement plat$*)$;

(ii) Si les A-modules E et F sont de type $\mathscr{C}$, il en est de même du A-module $E\otimes F$;

(iii) Le A-module $K_{\gamma}$ défini ci-dessus est de type $\mathscr{C}$.

Il existe alors sur le groupe additif $K(\mathscr{C})$une unique structure d’anneau dont la multiplication satisfait à

$$
[E]_{\mathscr{C}}[F]_{\mathscr{C}}= [E\otimes F]_{\mathscr{C}}
$$

quels que soient les A-modules E et F de type $\mathscr{C}$. L’élément unité de $K(\mathscr{C})$est $[K_{\gamma}]_{\mathscr{C}}$. Si la bigèbre A est cocommutative, l’anneau $K(\mathscr{C})$est commutatif.

Muni de la loi de composition définie par $(E,F)\rightarrow$ cl(E$\otimes F)$, l’ensemble $\mathscr{C}$ est un monoïde admettant cl(K$_{\gamma})$ comme élément unité. Par suite $\mathbf{Z}^{(\mathscr{C})}$ est canoniquement muni d’une structure d’anneau dont la multiplication est caractérisée par la formule (13) cl(E) cl(F) = cl(E$\otimes F)$

et dont l’élément unité est cl(K$_{\gamma})$ (III, p. 19).

Étant donnés un A-module F de type $\mathscr{C}$ et une suite exacte

$$
(\mathscr{E})0\longrightarrow E'\longrightarrow E\longrightarrow E''\longrightarrow 0
$$

de A-modules de type $\mathscr{C}$, la suite

$$
(\mathscr{E}\otimes F)0\longrightarrow E'\otimes F\longrightarrow E\otimes F\longrightarrow E''\otimes F\longrightarrow 0
$$

déduite de $(\mathscr{E})$ est exacte car F est projectif $(*$ou plus généralement plat$*)$ sur K (II, p. 58, prop. 5 et p. 63, cor. 6). On a alors, avec les notations du n$^o2$

(14) $r_{\mathscr{E}\otimes F}=r_{\mathscr{E}}$ cl(F). Il en résulte que le sous-groupe R de $\mathbf{Z}^{(\mathscr{C})}$ engendré par les éléments de la forme $r_{\mathscr{E}}$ est un idéal à droite de l’anneau $\mathbf{Z}^{(\mathscr{C})}$, et on démontre de même que c’est un idéal à gauche de $\mathbf{Z}^{(\mathscr{C})}$. Par définition, $K(\mathscr{C})$ est le groupe quotient $\mathbf{Z}^{(\mathscr{C})}/R$; il existe donc sur $K(\mathscr{C})$ une unique structure d’anneau dont la multiplication satisfait à $[E]_{\mathscr{C}}[F]_{\mathscr{C}}= [E\otimes F]_{\mathscr{C}}$ quels que soient les A-modules E et F de type $\mathscr{C}$. Son élément unité est $[K_{\gamma}]$.

Lorsque la bigèbre A est cocommutative, le monoïde $\mathscr{C}$ est commutatif ; il en résulte que l’anneau $\mathbf{Z}^{(\mathscr{C})}$ et l’anneau quotient $K(\mathscr{C})$ sont commutatifs.

#### Remarque {#alg-viii-s11-n7-rem-1 .statement tag=00DJ}

Sous les seules hypothèses (i) et (ii) de la prop. 9, le groupe de Grothendieck $K'(\mathscr{C})$ pour les sommes directes (VIII, p. 184) possède une unique structure d’anneau dont la multiplication satisfait à $[E]'_{\mathscr{C}}[F]'_{\mathscr{C}}= [E\otimes F]'_{\mathscr{C}}$. Son élément unité est $[K_{\gamma}]'_{\mathscr{C}}$. L’anneau $K'(\mathscr{C})$ est commutatif si la bigèbre A est cocommutative. La démonstration est analogue à celle de la prop. 9, compte tenu du fait que le groupe $K'(\mathscr{C})$ s’identifie à $\mathbf{Z}^{(\mathscr{C})}/R'$, où $R'$ est le sous-groupe de $\mathbf{Z}^{(\mathscr{C})}$ engendré par les éléments de la forme cl(E$'\oplus E'')-$ cl(E$')-$ cl(E$'') ($loc. cit.).

Sous les hypothèses (i), (ii) et (iii) de la prop. 9, l’anneau $K(\mathscr{C})$ est appelé l’anneau de Grothendieck de $\mathscr{C}$. Ces hypothèses sont vérifiées en particulier lorsque K est un corps et $\mathscr{C}$ l’ensemble des classes des A-modules qui sont de dimension finie sur K. Par conséquent :

#### Corollaire {#alg-viii-s11-n7-cor-1 .statement tag=00DK}

Soit A une bigèbre de coünité $\gamma$ sur un corps commutatif K. Il existe alors sur le groupe additif $R_K(A)$une unique structure d’anneau dont la multiplication satisfait à

$$
[E]_{\mathscr{C}}[F]_{\mathscr{C}}= [E\otimes_KF]_{\mathscr{C}}
$$

quels que soient les A-modules E et F de dimension finie sur K. L’élément unité de $R_K(A)$est $[K_{\gamma}]_{\mathscr{C}}$. Si la bigèbre A est cocommutative, l’anneau $R_K(A)$est commutatif.

#### Exemple 1 {#alg-viii-s11-n7-exa-1 .statement tag=00DL}

Soit K un corps commutatif. Soit G un groupe et soit K[G] l’algèbre du groupe G. Nous identifierons G à son image canonique dans K[G] (III, p. 19).

On munit K[G] de la structure de bigèbre dont le coproduit $c$ et la coünité $\gamma$ sont donnés par

$$
c(g) =g\otimes g,\gamma (g) = 1(g\in G) \tag{15}
$$

Soient E et F des K[G]-modules ; d’après la formule (12), la structure de K[G]-module sur $E\otimes F$ est donc donnée par

$$
g(x\otimes y) =gx\otimes gy(g\in G, x\in E, y\in F) \tag{16}
$$

Le K[G]-module $K_{\gamma}$ est l’espace vectoriel K, muni de l’action de G définie par $g\lambda =\lambda$ pour $g\in G$ et $\lambda \in K$.

L’anneau $R_K(K[G])$ est aussi noté $R_K(G)$. Il est commutatif ; sa multiplication est donnée par $[E] [F] = [E\otimes_KF]$ et l’élément unité de $R_K(G)$ est $[K_{\gamma}]$.

#### Exemple 2 {#alg-viii-s11-n7-exa-2 .statement tag=00DM}

Soient $\mathfrak{g}$ une algèbre de Lie sur un corps commutatif K, et $U(\mathfrak{g})$ son algèbre

enveloppante ; on identifie $\mathfrak{g}$ à son image canonique dans $U(\mathfrak{g})$ (LIE, I, p. 33, cor. 2). On munit $U(\mathfrak{g})$ de la structure de bigèbre pour laquelle le coproduit $c$ et la coünité $\gamma$ sont donnés par

$$
c(\xi ) =\xi \otimes 1 + 1\otimes \xi ,\gamma (\xi ) = 0 \tag{17}
$$

pour $\xi \in \mathfrak{g}$ (LIE, II, p. 11).

Soient E et F des $U(\mathfrak{g}$)-modules ; d’après la formule (17), la structure de $U(\mathfrak{g})$-module sur $E\otimes F$ est caractérisée par

$$
\xi (x\otimes y) =\xi x\otimes y+x\otimes \xi y \tag{18}
$$

pour $\xi \in \mathfrak{g},x\in E$ et $y\in F$.

L’anneau de Grothendieck $R_K(U(\mathfrak{g}))$ est aussi noté $\mathscr{R}(\mathfrak{g})$ dans LIE, VIII, p. $133.*$

Soit A un anneau commutatif. On peut considérer A comme une bigèbre cocommutative sur lui-même dont le coproduit est l’isomorphisme naturel de A sur $A\otimes_AA$ et la coünité est Id$_A$ (III, p. 149). D’après la prop. 9, on obtient le résultat suivant :

#### Proposition 10 {#alg-viii-s11-prop-10 .statement tag=00DN}

Soit A un anneau commutatif et soit $\mathscr{C}$ un ensemble additif de classes de A-modules satisfaisant aux trois hypothèses suivantes :

(i) Tout A-module de type $\mathscr{C}$ est projectif $(*$ou plus généralement plat$*)$;

(ii) Si E et F sont des A-modules de type $\mathscr{C}$, le A-module $E\otimes_AF$est aussi de type $\mathscr{C}$;

(iii) Le A-module A est de type $\mathscr{C}$.

Il existe alors sur le groupe additif $K(\mathscr{C})$une unique structure d’anneau satisfaisant à $[E]_{\mathscr{C}}[F]_{\mathscr{C}}= [E\otimes_AF]_{\mathscr{C}}$ pour tout couple de A-modules E, F de type $\mathscr{C}$. L’élément unité de $K(\mathscr{C})$est $[A]_{\mathscr{C}}$.

### 8. Le groupe de Grothendieck $K_0(A)$

Soit A un anneau. L’ensemble $\mathscr{P}(A)$ des classes de A-modules projectifs de type fini est additif ; on note $K_0(A)$ le groupe de Grothendieck $K(\mathscr{P}(A))$.

Pour la loi de composition $(E,E')\rightarrow$ cl(E$\oplus E')$, l’ensemble $\mathscr{P}(A)$ est un monoïde commutatif. De plus, toute suite exacte de A-modules projectifs

$$
0\longrightarrow E'\longrightarrow E\longrightarrow E''\longrightarrow 0
$$

est scindée (II, p. 39, prop. 4), de sorte que E est isomorphe à $E'\oplus E''$. L’application $E\rightarrow [E]$ de $\mathscr{P}(A)$ dans $K_0(A)$ définit donc un isomorphisme du groupe des différences du monoïde $\mathscr{P}(A)$ sur $K_0(A)$ (VIII, p. 184).

Pour tout module P projectif de type fini, il existe un module $P'$ projectif de type fini tel que $P\oplus P'$ soit libre (II, p. 40, cor.1). Soient E et F des A-modules projectifs de type fini ; d’après I, p. 18, prop. 6 on a [E] = [F] dans $K_0(A)$ si et seulement s’il existe un A-module libre de type fini L tel que les A-modules $E\oplus L$ et $F\oplus L$ soient isomorphes. On dit alors que E et F sont stablement isomorphes ; cela n’entraîne pas nécessairement que E et F soient isomorphes (VIII, p. 202, exerc. 2 et VIII, p. 205, exerc. 14).

Lorsque l’anneau A est commutatif, il existe sur le groupe additif $K_0(A)$ une structure d’anneau commutatif, dont la multiplication est caractérisée par la formule $[E]_{\mathscr{P}(A)}[F]_{\mathscr{P}(A)}= [E\otimes_AF]_{\mathscr{P}(A)}$ (VIII, p. 194, prop. 10).

#### Remarque {#alg-viii-s11-n8-rem-1 .statement tag=00DO}

Soit A un anneau semi-simple. Tout A-module est alors semi-simple et projectif (VIII, p. 134, prop. 4), d’où l’égalité

$$
\mathscr{L}\mathscr{F}(A) =\mathscr{S}\mathscr{S}(A) =\mathscr{P}(A)
$$

(cf. le n$^o4$ pour la définition de $\mathscr{L}\mathscr{F}(A)$ et $\mathscr{S}\mathscr{S}(A))$. On a donc $K_0(A) = R(A)$ d’après la définition de ces groupes de Grothendieck.

#### Exemple {#alg-viii-s11-n8-exa-1 .statement tag=00DP}

Si tout A-module projectif de type fini est libre, alors le rang définit un isomorphisme de $K_0(A)$ sur $\mathbf{Z}$. C’est en particulier le cas si A est un anneau principal (VII, p. 14, cor. 3) ou si A est un anneau local (VIII, p. 33, cor. 6).

### 9. Le groupe de Grothendieck $K_0(A)$d’un anneau artinien

Soit A un anneau artinien à gauche. Soit $\mathfrak{r}$ son radical ; c’est un idéal bilatère nilpotent de A et l’anneau $A/\mathfrak{r}$ est semi-simple (VIII, p. 169, prop. 1). D’après le corollaire de VIII, p. 172, l’application $P\rightarrow$ cl(P$/\mathfrak{r}P)$ est un isomorphisme du monoïde $\mathscr{P}(A)$ sur le monoïde $\mathscr{P}(A/\mathfrak{r})$; on en déduit un isomorphisme de groupes $\gamma$ de $K_0(A)$ sur $K_0(A/\mathfrak{r})$, caractérisé par la relation $\gamma ([P]_{\mathscr{P}(A)}) = [P/\mathfrak{r}P]_{\mathscr{P}(A/\mathfrak{r})}$ pour tout A-module projectif de type fini P.

Comme l’anneau $A/\mathfrak{r}$ est semi-simple, la remarque ci-dessus entraîne l’égalité $R(A/\mathfrak{r}) = K_0(A/\mathfrak{r})$. Les modules de longueur finie sur l’anneau $A/\mathfrak{r}$ ne sont autres que les modules semi-simples de longueur finie sur l’anneau A (VIII, p. 170, prop 2) ; par suite, on peut identifier $\mathscr{L}\mathscr{F}(A/\mathfrak{r})$ à $\mathscr{S}\mathscr{S}$ (A), et $R(A/\mathfrak{r})$ à $K(\mathscr{S}\mathscr{S}(A))$. On note $\delta$ l’homomorphisme $\gamma_{\mathscr{L}\mathscr{F}(A),\mathscr{S}\mathscr{S}(A)}$ de $R(A/\mathfrak{r}) = K(\mathscr{S}\mathscr{S}(A))$ sur $R(A) = K(\mathscr{L}\mathscr{F}(A))$ (VIII, p. 187, remarque 1), c’est un isomorphisme. Enfin, on a $\mathscr{P}(A)\subset \mathscr{L}\mathscr{F}(A)$ et l’on pose $\varepsilon =\gamma_{\mathscr{L}\mathscr{F}(A),\mathscr{P}(A)}$. On a donc défini un diagramme

$K_0(A)$== // $K^{\gamma}_0(A/\mathfrak{r}) = R(A/\mathfrak{r})$

==

==

$_{\varepsilon}$ = $\delta$

$$
R(A)
$$

Notons $\mathscr{S}$ l’ensemble (fini) des classes de A-modules simples ; pour tout $\lambda \in \mathscr{S}$, choisissons un module $S_{\lambda}$ de classe $\lambda$ et une couverture projective $(P_{\lambda}, u_{\lambda})$ de $S_{\lambda}$ (VIII, p. 171, prop. 4). Il résulte de la prop. 6 de VIII, p. 172 que $K_0(A)$ est un $\mathbf{Z}$-module libre ayant pour base la famille $([P_{\lambda}]_{\mathscr{P}(A)})_{\lambda\in\mathscr{S}}$. De plus, comme $S_{\lambda}$ est isomorphe à $P_{\lambda}/\mathfrak{r}P_{\lambda}$ (VIII, p. 172$),\gamma$ transforme la base $([P_{\lambda}]_{\mathscr{P}(A)})_{\lambda\in\mathscr{S}}$ de $K_0(A)$ en la base $([S_{\lambda}])_{\lambda\in\mathscr{S}}$ de $R(A/\mathfrak{r})$. L’isomorphisme $\delta$ transforme la base $([S_{\lambda}])_{\lambda\in\mathscr{S}}$ de $R(A/\mathfrak{r})$ en la base $([S_{\lambda}])_{\lambda\in\mathscr{S}}$ de R(A).

On appelle matrice de Cartan de A la matrice $(a_{\lambda \mu})$ de l’homomorphisme de $\mathbf{Z}$-modules $\varepsilon : K_0(A)\rightarrow R(A)$ par rapport aux bases $([P_{\lambda}]_{\mathscr{P}(A)})_{\lambda\in\mathscr{S}}$ de $K_0(A)$ et $([S_{\lambda}])_{\lambda\in\mathscr{S}}$ de R(A). Par définition, on a

(19) $[P_{\mu}] =\sum_{\lambda\in\mathscr{S}}a_{\lambda \mu}[S_{\lambda}]$ (pour $\mu \in \mathscr{S})$

dans le groupe R(A). Autrement dit, $a_{\lambda \mu}$ est le nombre de quotients isomorphes à $S_{\lambda}$ dans une suite de Jordan-Hölder du A-module $P_{\mu}$.

Posons $\pi =\varepsilon \circ \gamma^{-1}\circ \delta^{-1}$; c’est un endomorphisme du groupe R(A). Si M est un A-module semi-simple de type fini et $(P, u)$ une couverture projective de M, on a $\pi ([M]) = [P]$. D’après la formule (19), la matrice de $\pi$ par rapport à la base $([S_{\lambda}])_{\lambda\in\mathscr{S}}$ de R(A) n’est autre que la matrice de Cartan de A.

### 10. Changement d’anneau pour $K_0(A)$

Soient A et B des anneaux. Soit $f: A\rightarrow B$ un homomorphisme d’anneaux. Si P est un A-module projectif de type fini, le B-module $f^*(P) = B\otimes_AP$ est projectif de type fini (II, p. 84, cor.) ; l’application $P\rightarrow$ cl($f^*(P)$) est un homomorphisme du monoïde $\mathscr{P}(A)$ dans le monoïde $\mathscr{P}$(B), et définit donc un homomorphisme $f^*:$ $K_0(A)\rightarrow K_0(B)$ caractérisé par la relation $f^*([P]_{\mathscr{P}(A)}) = [f^*(P)]_{\mathscr{P}(B)}$ pour tout A-module projectif de type fini P. Si $g: B\rightarrow C$ est un second homomorphisme d’anneaux, il résulte de la transitivité de l’extension des scalaires (II, p. 83, prop. 2) que les homomorphismes $(g\circ f)^*$ et $g^*\circ f^*$ de $K_0(A)$ dans $K_0(C)$ sont égaux.

Supposons que $f$ fasse de B un A-module à gauche projectif de type fini. Soit Q un B-module à gauche projectif de type fini. Alors Q est facteur direct d’un B-module libre de type fini, qui est lui-même projectif de type fini sur A. Par conséquent, le A-module $f_*(Q)$ déduit de Q par restriction des scalaires est projectif de type fini. On en déduit comme ci-dessus un homomorphisme $f_*: K_0(B)\rightarrow K_0(A)$ caractérisé par la relation $f_*([Q]_{\mathscr{P}(B)}) = [f_*(Q)]_{\mathscr{P}(A)}$ pour tout B-module projectif de type fini Q. Si $g: B\rightarrow C$ est un homomorphisme d’anneaux qui fait de C un B-module projectif de type fini, les homomorphismes $(g\circ f)_*$ et $f_*\circ g_*$ de $K_0(C)$ dans $K_0(A)$ sont égaux.

### 11. Réciprocité de Frobenius

Soit A un anneau semi-simple. Soit $f$ un homomorphisme de A dans un anneau semi-simple B. Soient S un A-module simple, T un B-module simple, D et E les commutants de S et T respectivement. D’après le lemme de Schur (VIII, p. 43, cor.), D et E sont des corps. Soit H l’ensemble des homomorphismes A-linéaires de S dans $f_*(T)$. On munit H de la structure de $(E$, D)-bimodule dont les lois d’action sont $(e, u)\rightarrow e\circ u$ et $(d, u)\rightarrow u\circ d$ (pour $e\in E,u\in H,d\in D)$.

#### Proposition 11 {#alg-viii-s11-prop-11 .statement tag=00DQ}

a) La multiplicité $[f_*(T) : S]$du A-module simple S dans le A-module semi-simple $f_*(T)$est égale à la dimension de H considéré comme espace vectoriel à droite sur D.

b) La multiplicité $[f^*(S) : T]$est finie et est égale à la dimension de H considéré comme espace vectoriel à gauche sur E.

L’assertion a) résulte de la formule (11) de VIII, p. 68.

Le B-module $f^*(S)$ est semi-simple et de type fini, donc de longueur finie. D’après la formule (12) de loc. cit., on a

(20) $[f^*(S) : T] =$ dim$_E$ Hom$_B(f^*(S),T)$.

Or, on a défini en II, p. 82 (formule 2 et remarque 2) une bijection E-linéaire de Hom$_A(S, f_*(T))$ sur Hom$_B(f^*(S),T)$. L’assertion b) résulte alors de la formule (20).

#### Corollaire {#alg-viii-s11-n11-cor-1 .statement tag=00S7}

Supposons que A et B soient des algèbres semi-simples de dimension finie sur un corps commutatif K et que $f$ soit K-linéaire. Alors les K-espaces vectoriels S, T, D, E et H sont de dimension finie, et l’on a les égalités

$$
[f_*(T) : S][D : K] = [f^*(S) : T][E : K] = [H : K] \tag{21}
$$

En particulier, lorsque K est algébriquement clos, on a D = E = K et

$$
[f_*(T) : S] = [f^*(S) : T] = [H : K] \tag{22}
$$

Le A-module S est simple, donc monogène, et D est un sous-espace vectoriel de Hom$_K(S,S)$; donc S et D sont de dimension finie sur K. Pour une raison analogue, T et E sont de dimension finie sur K. Enfin, H est un sous-espace vectoriel de Hom$_K(S,T)$; il est donc aussi de dimension finie. La formule (21) résulte alors de la prop. 11 puisque la dimension de H sur K est égale à [H : D][D : K] et à [H : E][E : K] (II, p. 31, prop. 25). D’après le th. 1 de VIII, p. 43, si K est algébriquement clos, on a D = E = K. La deuxième partie du corollaire résulte alors de la première.

Soient A et B des algèbres semi-simples de dimension finie sur un corps commutatif K et que $f$ soit un homomorphisme de K-algèbres de A dans B.

Soit $\mathscr{S}(A)$ l’ensemble des classes de A-modules simples ; pour tout $\lambda \in \mathscr{S}$(A), soit $S_{\lambda}$ un module de classe $\lambda$, et $D_{\lambda}$ son commutant ; alors $D_{\lambda}$ est une algèbre de degré fini sur K, et l’on note $d_{\lambda}$ ce degré. On définit de manière analogue $\mathscr{S}$ (B), $T_{\mu}, E_{\mu}$ et $e_{\mu}$ pour $\mu$ dans $\mathscr{S}(B)$. Le groupe de Grothendieck $K_0(A)$ a pour base la famille $([S_{\lambda}])_{\lambda\in\mathscr{S}(A)}$ et $K_0(B)$ a pour base $([T_{\mu}])_{\mu\in\mathscr{S}(B)}$. Soient $(a_{\mu \lambda})$ la matrice de $f^*: K_0(A)\rightarrow K_0(B)$ et $(b_{\lambda \mu})$ la matrice de $f_*: K_0(B)\rightarrow K_0(A)$ par rapport à ces bases. On a par définition

$$
a_{\mu \lambda}= [f^*(S_{\lambda}) : T_{\mu}],b_{\lambda \mu}= [f_*(T_{\mu}) : S_{\lambda}] \tag{23}
$$

pour $\lambda$ dans $\mathscr{S}(A)$ et $\mu$ dans $\mathscr{S}(B)$. Notons $h_{\lambda \mu}$ la dimension sur le corps K de l’espace vectoriel Hom$_A(S_{\lambda}, f_*(T_{\mu}))$. D’après le corollaire ci-dessus, on a

$$
h_{\lambda \mu}=e_{\mu}a_{\mu \lambda}=d_{\lambda}b_{\lambda \mu} \tag{24}
$$

Lorsque le corps K est algébriquement clos, on a $d_{\lambda}=e_{\mu}= 1$; par conséquent, on a (25) $a_{\mu \lambda}=b_{\lambda \mu}=h_{\lambda \mu}$.

Autrement dit, les matrices de $f_*$ et $f^*$ par rapport aux bases données de $K_0(A)$ et $K_0(B)$ sont transposées l’une de l’autre.

### 12. Cas des anneaux simples

Soient A et B des anneaux simples et $f$ un homomorphisme de A dans B. Soient S un A-module simple et T un B-module simple. On pose

(26) $i(f) = [f^*(S) : T] =$ long$_B(f^*(S))$;

on dit que le cardinal $i(f)$ est l’indice de $f$. Lorsque A est un sous-anneau de B, et $f$ l’injection canonique de A dans B, on écrit $i(B,A)$ au lieu de $i(f)$, et l’on dit que ce cardinal est l’indice de A dans B. On définit de manière analogue la hauteur $h(f)$ de $f:$

(27) $h(f) = [f_*(T) : S] =$ long$_A(f_*(T))$;

lorsque A est un sous-anneau de B et $f$ l’injection canonique de A dans B, on écrit $h(B,A)$ pour $h(f)$ et l’on dit que c’est la hauteur de A dans B.

Le A-module S est monogène, donc le B-module $f^*(S) = B\otimes_AS$ est monogène ; il en résulte que $i(f)$ est fini, donc que c’est un entier. Soit M un A-module. Notons $\mathfrak{a}$ sa longueur, alors M est isomorphe à $S^{(\mathfrak{a})}$. Donc le B-module $f_*(M)$ est isomorphe à $f_*(S)^{(\mathfrak{a})}$. Par définition de $i(f)$, on a donc

(28) long$_B(f^*(M)) =i(f)$ long$_A(M)$.

Les $\mathbf{Z}$-modules $K_0(A)$ et $K_0(B)$ sont libres de dimension 1, de bases respectives [S] et [T], et l’on a

$$
f^*([S]) =i(f)[T] \tag{29}
$$

Prenons en particulier $M = A_s$; alors $f^*(A_s) = B\otimes_AA_s$ est isomorphe à $B_s$ (II, p. 56), d’où

(30) $i(f) =$ long(B)$/$ long(A). D’après le théorème de Wedderburn (VIII, p. 116, th. 1), il existe des entiers $m\geqslant 1$ et $n\geqslant 1$ et des corps D et E tels que A soit isomorphe à $\mathbf{M}_m(D)$ et B à $\mathbf{M}_n(E)$; d’après la formule (30), on a $i(f) =_m^n$ et en particulier $m$ divise $n$.

Soit N un B-module ; notons $\mathfrak{a}$ sa longueur. Alors N est isomorphe à $T^{(\mathfrak{a})}$, donc le A-module $f_*(N)$ est isomorphe à $f_*(T)^{(\mathfrak{a})}$; par définition de $h(f)$, on a

(31) long$_A(f_*(N)) =h(f)$ long$_B(N)$.

On a vu (VIII, p. 120, prop. 5) que $f$ fait de B un A-module libre et que toutes les bases de ce module ont le même cardinal, noté $[B : A]_s$ et appelé le degré (à gauche) de B sur A. Le A-module $f_*(B_s)$ est isomorphe à $A^{[B:A]}_{s^s}$, donc il est de longueur égale à $[B : A]_s$ long(A). D’après la formule (30), et la formule (31) appliquée au cas particulier $N = B_s$, on a donc

$$
[B : A]_s=i(f)h(f) \tag{32}
$$

Supposons maintenant que B soit un A-module de type fini, c’est-à-dire que $[B : A]_s$ soit fini. Alors $h(f)$ est fini d’après la formule précédente. On a défini (VIII, p. 197) un homomorphisme de groupes $f_*$ de $K_0(B)$ dans $K_0(A)$; on a

$$
f_*([T]) =h(f)[S] \tag{33}
$$

Supposons que A et B soient des algèbres de dimension finie sur un corps commutatif K et que $f$ soit K-linéaire. Comme plus haut, il existe des entiers $m\geqslant 1$ et $n\geqslant 1$, des K-algèbres D et E qui sont de corps et des isomorphismes de K-algèbres de A sur $\mathbf{M}_m(D)$ et de B sur $\mathbf{M}_n(E)$. Posons $d= [D : K]$ et $e= [E : K]$. On a alors les relations

$_2$ 2 $n^2e$

$$
[A : K] =md,[B : K] =ne,[B : A]_s=
$$

$$
m^2d
$$

et, d’après les formules (30) et (32), les relations

$$
nne
$$

$$
i(f) =,h(f) =
$$

$$
mmd
$$

Lorsque le corps K est algébriquement clos, on a $d=e= 1$, d’où $i(f) =h(f)$ et $[B : A]_s=i(f)^2$.

Soient A, B et C des anneaux simples et soient $f: A\rightarrow B$ et $g: B\rightarrow C$ des homomorphismes. Soit S un A-module simple. Les C-modules $(g\circ f)^*(S)$ et $g^*(f^*(S))$ sont isomorphes ; on a donc, d’après les formules (26) et (28),

$i(g\circ f) =$ long$_C(g^*(f^*(S))) =i(g)$ long$_B(f^*(S)) =i(g)i(f)$. On démontre de même l’égalité $h(g\circ f) =h(g)h(f)$. Lorsque A est un sous-anneau de B, que B est un sous-anneau de C et que $f$ et $g$ sont les injections canoniques, ces égalités s’écrivent encore

$$
i(C,A) =i(C,B)i(B,A),h(C,A) =h(C,B)h(B,A) \tag{34}
$$

#### Proposition 12 {#alg-viii-s11-prop-12 .statement tag=00DR}

Soit B un anneau simple et soit A un sous-anneau simple de B. On suppose que B est un A-module à gauche de type fini. Soit M un B-module à gauche de type fini non nul. Posons $A'=$ End$_A(M)$et $B'=$ End$_B(M)$. Alors $B'$ est un sous-anneau de $A'$, les anneaux $A'$ et $B'$ sont simples, $A'$ est un $B'$-module à gauche de type fini et l’on a les égalités

$$
i(A',B') =h(B,A),h(A',B') =i(B,A),[A': B']_s= [B : A]_s
$$

D’après la prop. 4 de VIII, p. 119, l’anneau $A'$ est simple, M est un $A'$-module de longueur finie et l’on a

long$_A(M) =$ long(A$')$, long$_{A'}(M) =$ long(A).

Pour les mêmes raisons, l’anneau $B'$ est simple et l’on a

long$_B(M) =$ long(B$')$, long$_{B'}(M) =$ long(B).

D’après les formules (31) et (30), on a donc

$h(B,A) =$ long$_A(M)/$ long$_B(M) =$ long(A$')/$ long(B$') =i(A',B')$,

et la formule $h(A',B') =i(B,A)$ s’établit de manière analogue. De là on déduit

$$
[A': B']_s=i(A',B')h(A',B') =h(B,A)i(B,A) = [B : A]_s
$$

par la formule (32). En particulier, $A'$ est un $B'$-module à gauche de type fini.

## EXERCICES {#alg-viii-s11-exercises}

See the [exercises for § 11](exercises/s11/).
