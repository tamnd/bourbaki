---
book: alg
book_title: Algebra
chapter: V
chapter_title: Corps commutatifs
section: 17
section_title: EXTENSIONS RÉGULIÈRES
lang: fr
source: alg-iv-vii-fr
pdf_pages: 0235-0243, 0272-0289
extraction: ocr
subsections:
    - "no": 1
      title: Compléments sur la fermeture algébrique séparable
      page: 0
      pdf_page: 235
    - "no": 2
      title: Produit tensoriel d’extensions
      page: 132
      pdf_page: 236
    - "no": 3
      title: Algèbres absolument intègres
      page: 134
      pdf_page: 238
    - "no": 4
      title: Extensions régulières
      page: 0
      pdf_page: 239
    - "no": 5
      title: Caractérisation des extensions régulières
      page: 136
      pdf_page: 240
    - "no": 6
      title: Application aux extensions composées
      page: 137
      pdf_page: 241
statements: 20
exercises: 5
content_sha256: 3aaa25d7fe09d3724420e137a51a07835fc20991d574e1bfd4e14531f8a3e577
---

## § 17. EXTENSIONS RÉGULIÈRES

### 1. Compléments sur la fermeture algébrique séparable

#### Théorème 1 (Zariski) {#alg-v-s17-thm-1 .statement}

Soient K un corps, L une extension de K, $K_1$ la fermeture algébrique séparable de K dans L (V, p. 42), $K_2$ la fermeture algébrique de K dans L (V, p. 19) et $(X_i)_{i \in I}$ une famille d’indéterminées. Alors $K_1(X_i)_{i \in I}$ est la fermeture algébrique séparable de $K(X_i)_{i \in I}$ dans $L(X_i)_{i \in I}$, et $K_2(X_i)_{i \in I}$ est la fermeture algébrique de $K(X_i)_{i \in I}$ dans $L(X_i)_{i \in I}$.

A) On suppose que E est un corps et F un surcorps de E et que tout élément de F qui est algébrique séparable sur E appartient à E. Soit $u$ un élément de $F(X)$ qui est algébrique séparable sur $E(X)$; nous allons montrer que $u$ appartient à $E(X)$. Il existe dans $F[X]$ deux polynômes étrangers P et Q tels que $u = P/Q$, et l’on peut supposer que Q est unitaire. Soient S la partie finie de F formée des coefficients de P et Q, $F_0 = E(S)$, et $\Delta$ une E-dérivation de $F_0$ dans $F_0$. Soit D la dérivation de $F_0(X)$ dans lui-même qui coïncide avec $\Delta$ sur $F_0$ et annule X (V, p. 123, prop. 3).

Comme $u \in F_0(X)$ est algébrique séparable sur $E(X)$ et que D est nulle sur $E(X)$, on a $D(u) = 0$ (V, p. 123, prop. 4), d’où $D(P) . Q = P . D(Q)$. Comme P et Q sont étrangers, on en déduit que Q divise D(Q) (IV, p. 12, cor. 4). Or, on peut écrire Q sous la forme

$$
Q(X) = X^n + a_1 X^{n-1} + \cdots + a_{n-1} X + a_n
$$

avec $a_1, ..., a_n$ dans $F_0$; comme on a $D(X) = 0$, on a donc

(1)
$$
D(Q) = \Delta(a_1) X^{n-1} + \cdots + \Delta(a_{n-1}) X + \Delta(a_n)
$$

d’où $\deg D(Q) < \deg Q$. Comme Q divise D(Q), ceci n’est possible que si D(Q) est nul. Mais alors D(P) est nul puisque D(P).Q = P.D(Q). La formule (1) et une formule analogue pour P montrent alors que $\Delta$ annule l’ensemble S des coefficients de P et Q, d’où $\Delta = 0$ puisque $F_0 = E(S)$. D’après V, p. 129, cor. 2, l’extension de type fini $F_0$ de E est donc algébrique séparable ; vu les hypothèses faites sur E et F, on a $F_0 = E$, d’où finalement $u \in E(X)$.

B) Supposons maintenant que le corps E soit algébriquement fermé dans le surcorps F et notons $p$ l’exposant caractéristique de E. Soit $u$ un élément de $F(X)$ algébrique sur $E(X)$. Il existe un entier $f \geqslant 0$ tel que $v = u^{p^f}$ soit algébrique et séparable sur $E(X)$ (V, p. 42, prop. 13). D’après A), on a donc $v \in E(X)$. Il existe une unique représentation de $u$ sous la forme $P/Q$ avec des polynômes P et Q étrangers dans $F[X]$, et Q unitaire ; on a une décomposition analogue $v = P_1/Q_1$ avec $P_1$ et $Q_1$ étrangers dans $E[X]$ et $Q_1$ unitaire. On en déduit $P_1/Q_1 = P^{p^f}/Q^{p^f}$; les polynômes $P^{p^f}$ et $Q^{p^f}$ sont étrangers dans $F[X]$ (IV, p. 12, cor. 6), de même que $P_1$ et $Q_1$, et $Q^{p^f}$ est unitaire. On en conclut $P^{p^f} = P_1 \in E[X]$ et $Q^{p^f} = Q_1 \in E[X]$. Par suite, les coefficients de P et Q sont radiciels sur E, donc appartiennent à E puisque E est algébriquement fermé dans F. On a donc $P \in E[X]$, $Q \in E[X]$ et finalement $u \in E(X)$. On a prouvé que $E(X)$ est algébriquement fermé dans $F(X)$.

C) Reprenons les notations du théorème 1. Comme $K_1$ est une extension algébrique séparable de K, l’extension $K_1(X_i)_{i \in I}$ de $K(X_i)_{i \in I}$ est algébrique et séparable (V, p. 38, prop. 6). De plus, tout élément de L qui est algébrique et séparable sur $K_1$ appartient à $K_1$ (V, p. 42, prop. 13, a)). Soit J une partie finie de I ; par une récurrence immédiate sur le cardinal de J, on déduit de A) que tout élément de $L(X_i)_{i \in J}$ qui est algébrique et séparable sur $K(X_i)_{i \in J}$ appartient à $K_1(X_i)_{i \in J}$. Soit enfin $u$ un élément de $L(X_i)_{i \in I}$ algébrique et séparable sur $K(X_i)_{i \in I}$; il existe une partie finie J de I telle que $u$ appartienne à $L(X_i)_{i \in J}$ et soit algébrique et séparable sur $K(X_i)_{i \in J}$; d’après ce qui précède, $u$ appartient à $K_1(X_i)_{i \in J}$ et *a fortiori* à $K_1(X_i)_{i \in I}$.

On vient de déduire de A) que $K_1(X_i)_{i \in I}$ est la fermeture séparable de $K(X_i)_{i \in I}$ dans $L(X_i)_{i \in I}$; on déduit de manière analogue de B) que $K_2(X_i)_{i \in I}$ est la fermeture algébrique de $K(X_i)_{i \in I}$ dans $L(X_i)_{i \in I}$.

### 2. Produit tensoriel d’extensions

#### Proposition 1 {#alg-v-s17-prop-1 .statement}

*Soient $\Omega$ une extension d’un corps K et L, M deux sous-extensions de $\Omega$ algébriquement disjointes sur K. On suppose que la fermeture algébrique séparable* de K dans L est égale à K $^1$. Soient $\varphi$ l’homomorphisme de K-algèbres de $L \otimes_K M$ dans $\Omega$ transformant $x \otimes y$ en $xy$ pour $x \in L$ et $y \in M$, et $p$ le noyau de $\varphi$. Alors $p$ est l’ensemble des éléments nilpotents de $L \otimes_K M$ et c’est le plus petit des idéaux premiers de $L \otimes_K M$.

Quitte à remplacer $\Omega$ par une clôture algébrique, on peut supposer que $\Omega$ est algébriquement clos. Notons B une base de transcendance de M sur K, N la fermeture algébrique de K(B) dans $\Omega$ et $N_s$ (resp. $N_r$) l’ensemble des éléments de N qui sont séparables (resp. radiciels) sur K(B). Remarquons que M est algébrique sur K(B), donc que N est la fermeture algébrique de M dans $\Omega$.

$$
\begin{array}{ccccccccc}
L & \longrightarrow & L(B) & \longrightarrow & L(B \cup N_s) \\
& & \uparrow & & \uparrow \\
K & \longrightarrow & K(B) & \longrightarrow & N_s \\
& & \downarrow & & \downarrow \\
& & M & & N \\
& & \downarrow & & \downarrow \\
& & N_r & & N & \longrightarrow & \Omega
\end{array}
$$

Fig. 1.

Définissons la chaîne suivante d’homomorphismes :

$$
L \otimes_K M \xrightarrow{\alpha} L \otimes_K N \xrightarrow{\beta} (L \otimes_K K(B)) \otimes_{K(B)} N \xrightarrow{\gamma} L(B) \otimes_{K(B)} N
$$
$$
\xrightarrow{\delta} L(B) \otimes_{K(B)} N_s \otimes_{K(B)} N_r \xrightarrow{\varepsilon} L(B \cup N_s) \otimes_{K(B)} N_r \xrightarrow{\zeta} \Omega .
$$

On a $\alpha = \mathrm{Id}_L \otimes u$ où $u$ est l’injection canonique de M dans N, donc $\alpha$ est injectif. L’application $\beta$ est l’isomorphisme de groupes commutatifs qui transforme $x \otimes y$ en $(x \otimes 1) \otimes y$ (II, p. 83, prop. 2) pour $x \in L$ et $y \in N$. On a $\gamma = v \otimes \mathrm{Id}_N$, où $v$ est l’homomorphisme de K-algèbres de $L \otimes_K K(B)$ dans $L(B)$ qui transforme $x \otimes y$ en $xy$ pour $x \in L$ et $y \in K(B)$; comme L et M sont algébriquement disjointes sur K, la prop. 14 (V, p. 109) montre que L et K(B) sont linéairement disjointes sur K ; autrement dit, $v$ est injectif, donc $\gamma$ est injectif. Comme N est une extension quasi-galoisienne de K(B), il existe (V, p. 73, prop. 13) un isomorphisme $w$ de K(B)-algèbres de $N_s \otimes_{K(B)} N_r$ sur N qui transforme $x \otimes y$ en $xy$ pour $x \in N_s$ et $y \in N_r$ : on a noté $\delta$ l’isomorphisme $\mathrm{Id}_{L(B)} \otimes w^{-1}$. D’après le th. 1 (V, p. 131) et l’hypothèse faite sur l’extension L de K, tout élément de L(B) qui est algébrique et séparable sur K(B) appartient à K(B) ; en particulier, on a $L(B) \cap N_s = K(B)$. Comme $N_s$ est une extension galoisienne de K(B), le th. 5 (V, p. 68) montre qu’il existe un isomorphisme $w'$ de K(B)-algèbres de $L(B) \otimes_{K(B)} N_s$ sur $L(B \cup N_s)$ transformant $x \otimes y$ en $xy$ pour $x \in L(B)$ et $y \in N_s$ ; on a noté $\varepsilon$ l’isomorphisme $w' \otimes \mathrm{Id}_{N_r}$. Enfin,

$^1$ On exprime parfois cette hypothèse en disant que L est une extension primaire de K.

ζ est l’homomorphisme de K-algèbres transformant $x \otimes y$ en $xy$ pour $x \in L(B \cup N_s)$ et $y \in N_r$.

Ce qui précède montre que $\eta = \varepsilon \delta \gamma \beta \alpha$ est un homomorphisme injectif de K-algèbres de $L \otimes_K M$ dans $L(B \cup N_s) \otimes_{K(B)} N_r$. De plus, tout élément de M est de la forme $\sum_{i=1}^n a_i b_i$ avec $a_i \in N_s$ et $b_i \in N_r$ pour $1 \leq i \leq n$; on en déduit aussitôt $\varphi = \zeta \eta$.

Le noyau $\mathfrak{p}$ de $\varphi$ est un idéal premier de $L \otimes_K M$, donc tout élément nilpotent de $L \otimes_K M$ appartient à $\mathfrak{p}$ d’après la prop. 2 (V, p. 113). Réciproquement, soit $a$ un élément de $\mathfrak{p}$; posons $\eta(a) = \sum_{i=1}^s b_i \otimes c_i$ avec $b_i \in L(B \cup N_s)$ et $c_i \in N_r$ pour $1 \leq i \leq s$. Comme $N_r$ est une extension radicielle de $K(B)$, il existe un entier $f \geq 0$ tel que $c_i^{p^f}$ appartienne à $K(B)$ pour $1 \leq i \leq s$ (on note $p$ l’exposant caractéristique de $K$). Mais on a

$$
\eta(a^{p^f}) = \sum_{i=1}^s b_i^{p^f} \otimes c_i^{p^f} = (\sum_{i=1}^s b_i^{p^f} c_i^{p^f}) \otimes 1 = \zeta \eta(a)^{p^f} \otimes 1 = 0
$$

et comme $\eta$ est injectif, on a finalement $a^{p^f} = 0$. On a donc prouvé que $\mathfrak{p}$ est l’ensemble des éléments nilpotents de $L \otimes_K M$. Tout idéal premier de $L \otimes_K M$ contient alors $\mathfrak{p}$ d’après la prop. 2 (V, p. 113).

#### Corollaire {#alg-v-s17-n2-cor-1 .statement}

Soient $L$ et $M$ deux extensions d’un corps $K$. On suppose que la fermeture algébrique séparable de $K$ dans $L$ est égale à $K$. Alors l’ensemble $\mathfrak{p}$ des éléments nilpotents de $L \otimes_K M$ est un idéal premier. Si de plus $L$ ou $M$ est séparable sur $K$, alors $L \otimes_K M$ est intègre.

On peut supposer que $L$ et $M$ sont des sous-extensions algébriquement disjointes d’une extension $\Omega$ de $K$ (V, p. 111, th. 5); alors $\mathfrak{p}$ est un idéal premier d’après la prop. 1 (V, p. 132). Si de plus $L$ ou $M$ est séparable sur $K$, alors $L \otimes_K M$ est un anneau réduit d’après la définition des extensions séparables (V, p. 114, déf. 1); on a donc $\mathfrak{p} = 0$ et $L \otimes_K M$ est intègre, puisque $\mathfrak{p}$ est premier.

### 3. Algèbres absolument intègres

#### Définition 1 {#alg-v-s17-def-1 .statement}

Soit $K$ un corps. On dit qu’une algèbre $A$ sur $K$ est absolument intègre si l’anneau $L \otimes_K A$ est intègre pour toute extension $L$ de $K$.

Une algèbre absolument intègre est en particulier un anneau intègre donc commutatif.

#### Proposition 2 {#alg-v-s17-prop-2 .statement}

Soient $A$ et $B$ deux algèbres sur un corps $K$. Si $A$ est intègre et $B$ absolument intègre, alors $A \otimes_K B$ est intègre.

Soit $L$ le corps des fractions de $A$. Comme $B$ est absolument intègre, l’anneau $L \otimes_K B$ est intègre; or l’anneau $A \otimes_K B$ est isomorphe à un sous-anneau de $L \otimes_K B$, donc est intègre.

#### Proposition 3 {#alg-v-s17-prop-3 .statement}

Soit $K$ un corps.

a) Toute sous-algèbre d’une $K$-algèbre absolument intègre est absolument intègre.

b) Le produit tensoriel de deux $K$-algèbres absolument intègres est absolument intègre.

c) Soient $A$ une $K$-algèbre absolument intègre et $K'$ une extension de $K$. Pour que $A$ soit absolument intègre, il faut et il suffit que la $K'$-algèbre $A_{(K')}$ déduite de $A$ par extension des scalaires soit absolument intègre.

La démonstration de a) (resp. c)) est identique à celle de la partie a) (resp. d)) de la prop. 3 de V, p. 114, en y remplaçant partout « réduit » par « intègre » et « séparable » par « absolument intègre ». Démontrons b).

Soient $A$ et $B$ deux $K$-algèbres absolument intègres. Soit $L$ une extension de $K$. Comme $A$ est absolument intègre, l’anneau $L \otimes_K A$ est intègre. D’après la prop. 2, l’anneau $(L \otimes_K A) \otimes_K B$ est donc intègre puisque $B$ est absolument intègre. Finalement, l’anneau $L \otimes_K (A \otimes_K B)$ est isomorphe à $(L \otimes_K A) \otimes_K B$, donc est intègre. Cela prouve que $A \otimes_K B$ est absolument intègre.

### 4. Extensions régulières

#### Définition 2 {#alg-v-s17-def-2 .statement}

On dit qu’une extension d’un corps $K$ est régulière si c’est une $K$-algèbre absolument intègre.

#### Proposition 4 {#alg-v-s17-prop-4 .statement}

Soient $A$ une algèbre intègre sur un corps $K$, et $E$ son corps des fractions. Soit $L$ une extension de $K$; si l’anneau $L \otimes_K A$ est intègre, il en est de même de $L \otimes_K E$.

Si l’anneau $L \otimes_K A$ est intègre, il se plonge dans son corps des fractions $F$. Posons $u(x) = x \otimes 1$ pour $x \in L$, et notons $v$ le $K$-homomorphisme de $E$ dans $F$ qui prolonge l’homomorphisme injectif $y \mapsto 1 \otimes y$ de $A$ dans $F$. D’après la prop. 6 (V, p. 14), les sous-corps $u(L)$ et $v(E)$ de $F$ sont linéairement disjoints sur $K$; par suite, l’homomorphisme $u * v$ de $L \otimes_K E$ dans $F$ (V, p. 12) est injectif. Ceci prouve que l’anneau $L \otimes_K E$ est intègre.

#### Corollaire {#alg-v-s17-n4-cor-1 .statement}

Pour que $A$ soit absolument intègre, il faut et il suffit que son corps des fractions soit une extension régulière de $K$.

La condition est nécessaire d’après la prop. 4 et suffisante d’après la prop. 3, a).

#### Proposition 5 {#alg-v-s17-prop-5 .statement}

Toute extension pure d’un corps $K$ est régulière.

D’après le corollaire précédent, il suffit de prouver que toute algèbre de polynômes $A = K[X_i]_{i \in I}$ est absolument intègre sur $K$. Soit $L$ une extension de $K$; l’anneau $L \otimes_K A$ est isomorphe à $L[X_i]_{i \in I}$ (III, p. 22, remarque 2), donc est intègre (IV, p. 9, prop. 8).

#### Proposition 6 {#alg-v-s17-prop-6 .statement}

Soit $L$ une extension d’un corps $K$. Si $L$ est régulière, toute sous-extension de $L$ est régulière. Inversement si toute sous-extension de type fini de $L$ est régulière, alors $L$ est régulière.

La première assertion résulte de la prop. 3, $a$.

Soit $M$ une extension de $K$, et soit $\mathcal{U}$ l’ensemble des sous-extensions de type fini de $L$. Pour tout $E \in \mathcal{U}$, l’anneau $M \otimes_K E$ s’identifie à un sous-anneau de $M \otimes_K L$, et l’on définit ainsi une famille filtrante croissante de sous-anneaux de $M \otimes_K L$, de réunion $M \otimes_K L$. On en déduit immédiatement la seconde assertion.

#### Proposition 7 {#alg-v-s17-prop-7 .statement}

*Soient $L$ une extension d’un corps $K$ et $M$ une $L$-algèbre (par exemple une extension de $L$). Si $L$ est régulière sur $K$ et $M$ absolument intègre sur $L$, alors $M$ est absolument intègre sur $K$*.

Soit $E$ une extension de $K$; comme $L$ est régulière sur $K$, l’anneau $E \otimes_K L$ est intègre. D’après la prop. 2 (V, p. 134), l’anneau $(E \otimes_K L) \otimes_L M$ est donc intègre, et il en est donc de même de l’anneau $E \otimes_K M$ qui lui est isomorphe (II, p. 83, prop. 2). D’où la proposition.

#### Proposition 8 {#alg-v-s17-prop-8 .statement}

*Soient $L$ et $M$ deux extensions d’un corps $K$.
a) Si $M$ est régulière sur $K$, le corps des fractions de l’anneau intègre $L \otimes_K M$ est une extension régulière de $L$.
b) Si $L$ et $M$ sont des extensions régulières de $K$, il en est de même du corps des fractions de $L \otimes_K M$*.

L’assertion $a$) résulte de la prop. 3, $c$) (V, p. 135) et du cor. de V, p. 135 ; l’assertion $b$) résulte de la prop. 3, $b$) (V, p. 135) et du cor. de V, p. 135.

### 5. Caractérisation des extensions régulières

#### Proposition 9 {#alg-v-s17-prop-9 .statement}

*Soient $K$ un corps, $\overline{K}$ une clôture algébrique de $K$ et $L$ une extension de $K$. Les conditions suivantes sont équivalentes :
a) $L$ est séparable sur $K$ et $K$ est algébriquement fermé dans $L$.
b) $L$ est une extension régulière de $K$.
c) L’anneau $\overline{K} \otimes_K L$ est intègre.
d) Soit $\overline{L}$ une clôture algébrique de $L$. Alors $L$ est linéairement disjointe sur $K$ de la fermeture algébrique de $K$ dans $\overline{L}$.
De plus, si ces conditions sont satisfaites, l’anneau $\overline{K} \otimes_K L$ est un corps.
$a) \Rightarrow b)$ : soit $M$ une extension de $K$. Sous les hypothèses de $a$), l’anneau $M \otimes_K L$ est intègre d’après V, p. 134, cor.
$b) \Rightarrow c)$ : cela résulte de la déf. 2.
$c) \Rightarrow d)$ : avec les notations de $d$), on peut identifier $\overline{K}$ à la fermeture algébrique de $K$ dans $\overline{L}$ (V, p. 22, exemple 2). Supposons que l’anneau $A = \overline{K} \otimes_K L$ soit intègre. Soit $E$ une sous-extension de $\overline{K}$, de degré fini sur $K$; le sous-anneau $E \otimes_K L$ de $A$ est intègre, et c’est une algèbre de degré fini sur $L$; d’après le cor. de V, p. 10, c’est un corps. Comme $\overline{K}$ est réunion de l’ensemble filtrant croissant des extensions $E$ du type précédent, $A$ est un corps (V, p. 11, prop. 3). L’homomorphisme canonique de $A$ dans $\overline{L}$ qui envoie $x \otimes y$ sur $xy$ (pour $x \in \overline{K}$ et $y \in L$) est donc injectif, et par suite, $L$ et $\overline{K}$ sont linéairement disjoints sur $K$.

d) ⇒ a) : Sous les hypothèses de d), on a L ∩ \overline{K} = K, donc K est algébriquement fermé dans L ; de plus, si p est l’exposant caractéristique de K, le corps L est linéairement disjoint de K^{p^{-\infty}} sur K, donc L est séparable sur K (V, p. 118, cor. 1).

#### Corollaire 1 {#alg-v-s17-prop-9-cor-1 .statement}

Soit A une algèbre sur le corps K. Pour que A soit absolument intègre, il faut et il suffit que l’anneau \overline{K} \otimes_K A soit intègre.

La condition énoncée est évidemment nécessaire. Inversement, supposons que l’anneau \overline{K} \otimes_K A soit intègre, et notons E le corps des fractions de A. D’après la prop. 4 (V, p. 135), l’anneau \overline{K} \otimes_K E est intègre, donc E est extension régulière de K par la proposition 9 ; on conclut par V, p. 135, cor., que A est une K-algèbre absolument intègre.

#### Corollaire 2 {#alg-v-s17-prop-9-cor-2 .statement}

Soit K un corps algébriquement clos. Toute K-algèbre intègre sur K est absolument intègre. En particulier, toute extension de K est régulière.

Cela résulte du cor. 1.

#### Corollaire 3 {#alg-v-s17-prop-9-cor-3 .statement}

Soit K un corps algébriquement clos. Si A et B sont deux K-algèbres intègres, il en est de même de A \otimes_K B.

D’après le cor. 2, A et B sont absolument intègres sur K, et il suffit d’appliquer la prop. 2 (V, p. 134).

### 6. Application aux extensions composées

#### Proposition 10 {#alg-v-s17-prop-10 .statement}

Soient L et M deux extensions d’un corps K et (E, u, v) une extension composée de L et de M (V, p. 11). On suppose que l’anneau L \otimes_K M est intègre et que les sous-extensions u(L) et v(M) de E sont algébriquement disjointes sur K. Alors u(L) et v(M) sont linéairement disjointes sur K.

Posons w = u \* v (V, p. 12). Notons F le corps des fractions de l’anneau intègre L \otimes_K M et identifions L (resp. M) à un sous-corps de F au moyen de l’application x ↦ x ⊗ 1 (resp. y ↦ 1 ⊗ y) ; alors la restriction de w à L (resp. M) est u (resp. v). Soit B une base de transcendance de M sur K (V, p. 105, th. 1).

Par hypothèse, u(L) et v(M) sont algébriquement disjointes sur K ; par suite (V, p. 109, prop. 14), u(L) et v(K(B)) sont linéairement disjointes sur K. Il existe donc un K-homomorphisme u' : L(B) → E qui coïncide avec u sur L et avec v sur K(B). Par construction, L et M sont linéairement disjoints sur K dans F ; d’après la prop. 8 (V, p. 14), les sous-corps L(B) et M de F sont linéairement disjoints sur K(B). Il existe par conséquent un K-homomorphisme w' : M[L(B)] → E qui coïncide avec u' sur L(B) et avec v sur M. Mais le corps F est engendré par M ∪ L(B) et M est algébrique sur K(B) ; on a donc M[L(B)] = F (V, p. 18, cor. 2). On conclut de là que w' est un K-isomorphisme de F sur E, dont la restriction à L (resp. M) est u (resp. v). Ceci prouve que u(L) et v(M) sont linéairement disjointes sur K.

#### Corollaire 1 {#alg-v-s17-prop-10-cor-1 .statement}

Soient Ω une extension d’un corps K et L une sous-extension de Ω régulière sur K. Toute sous-extension M de Ω qui est algébriquement disjointe de L sur K en est linéairement disjointe.

L’anneau $L \otimes_K M$ est intègre par définition d’une extension régulière, et il suffit d’appliquer la prop. 10.

#### Corollaire 2 {#alg-v-s17-prop-10-cor-2 .statement}

*Soient $\Omega$ une extension d’un corps $K$ et $L, M$ deux sous-extensions de $\Omega$. On suppose que $L$ est séparable sur $K$ et que la fermeture séparable de $K$ dans $M$ est égale à $K$. Si $L$ et $M$ sont algébriquement disjointes sur $K$, elles sont linéairement disjointes sur $K$.

D’après la prop. 10, il suffit de noter que l’anneau $L \otimes_K M$ est intègre (V, p. 134, cor.).

Exercises

## EXERCICES {#alg-v-s17-exercises}

See the [exercises for § 17](exercises/s17/).
