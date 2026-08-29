---
book: alg
book_title: Algebra
chapter: X
chapter_title: ALGÈBRE HOMOLOGIQUE
section: 3
section_title: Résolutions
lang: fr
source: alg-x-fr
book_pages: A X.46-A X.61, A X.178-A X.184
pdf_pages: 0052-0067, 0184-0190
extraction: ocr
subsections:
    - "no": 1
      title: Prolongement de morphismes de complexes
      page: 46
      pdf_page: 52
    - "no": 2
      title: Résolutions
      page: 48
      pdf_page: 54
    - "no": 3
      title: La résolution libre canonique
      page: 50
      pdf_page: 56
    - "no": 4
      title: La résolution injective canonique
      page: 52
      pdf_page: 58
    - "no": 5
      title: Résolutions de type fini
      page: 53
      pdf_page: 59
    - "no": 6
      title: ' Résolutions projectives minimales'
      page: 54
      pdf_page: 60
    - "no": 7
      title: Résolutions graduées
      page: 56
      pdf_page: 62
    - "no": 8
      title: La résolution standard
      page: 57
      pdf_page: 63
    - "no": 9
      title: Résolutions et groupes de Grothendieck
      page: 58
      pdf_page: 64
statements: 29
exercises: 19
content_sha256: 5ebb6c8a429b73fb0e96f7c1b840436916f3f85cfd822df95c442238a2791ff1
---

## § 3. RÉSOLUTIONS

On conserve les conventions du paragraphe précédent.

### 1. Prolongement de morphismes de complexes

#### Lemme 1 {#alg-x-s3-lem-1 .statement}

Considérons un diagramme de A-modules et d’homomorphismes

$$
\begin{array}{ccc}
M' & \xrightarrow{\alpha'} & M \\
f' \downarrow & & f \downarrow \\
N' & \xrightarrow{\beta'} & N
\end{array}
\quad
\begin{array}{ccc}
M & \xrightarrow{\alpha} & M'' \\
f \downarrow & & k'' \downarrow \\
N & \xrightarrow{\beta} & N''
\end{array}
$$

tel que $f \circ \alpha' = \beta \circ f', \alpha \circ \alpha' = 0, \mathrm{Ker}\ \beta = \mathrm{Im}\ \beta', \text{et } f = k'' \circ \alpha + \beta \circ k \text{ et où } M' \text{ est projectif. Il existe un A-homomorphisme } k': M' \to N' \text{ tel que } f' = k \circ \alpha' + \beta' \circ k'.$

En effet, posons $g = f' - k \circ \alpha'$; on a
$$
\beta \circ g = \beta \circ f' - \beta \circ k \circ \alpha' = f \circ \alpha' - \beta \circ k \circ \alpha' = k'' \circ \alpha \circ \alpha' = 0.
$$
Cela implique $\mathrm{Im}\ (g) \subset \mathrm{Ker}\ (\beta) = \mathrm{Im}\ (\beta')$. Comme $M'$ est projectif, il existe donc un A-homomorphisme $k': M' \to N'$ tel que $\beta' \circ k' = g$, d’où le lemme.

#### Lemme 2 {#alg-x-s3-lem-2 .statement}

Si dans le diagramme commutatif de A-modules et d’homomorphismes

$$
\begin{array}{ccc}
M' & \xrightarrow{\alpha'} & M \\
& \downarrow u & \downarrow u'' \\
N' & \xrightarrow{\beta'} & N
\end{array}
\quad
\begin{array}{ccc}
M & \xrightarrow{\alpha} & M'' \\
& \downarrow & \downarrow \\
N & \xrightarrow{\beta} & N''
\end{array}
$$

on a $\alpha \circ \alpha' = 0, \mathrm{Ker}\ \beta = \mathrm{Im}\ \beta'$ et si $M'$ est projectif, il existe un A-homomorphisme $u': M' \to N'$ tel que $\beta' \circ u' = u \circ \alpha'$.

Il suffit de poser $k'' = u'', k = -u, f = 0, f' = 0$ et $u' = k'$ dans le lemme 1.

Lemme 1 bis. — Considérons un diagramme de A-modules et d’homomorphismes

$$
\begin{array}{ccc}
M' & \xrightarrow{\alpha'} & M \\
k' \downarrow & & k \downarrow \\
N' & \xrightarrow{\beta'} & N
\end{array}
\quad
\begin{array}{ccc}
M & \xrightarrow{\alpha} & M'' \\
f' \downarrow & & f \downarrow \\
N & \xrightarrow{\beta} & N''
\end{array}
$$

tel que $f \circ \alpha' = \beta \circ f'$, $\mathrm{Ker}\, \alpha = \mathrm{Im}\, \alpha'$, $\beta \circ \beta' = 0$, et $f' = k \circ \alpha' + \beta' \circ k'$ et où $N''$ est injectif. Il existe un $A$-homomorphisme $k'' : M'' \to N''$ tel que $f = k'' \circ \alpha + \beta \circ k$.

En effet, posons $g = f - \beta \circ k$, on a
$$
g \circ \alpha' = f \circ \alpha' - \beta \circ k \circ \alpha' = \beta \circ f' - \beta \circ k \circ \alpha' = \beta \circ \beta' \circ k' = 0 .
$$
Cela implique $\mathrm{Ker}\, g \supset \mathrm{Im}\, \alpha' = \mathrm{Ker}\, \alpha$. Comme $N''$ est injectif, il existe donc (X, p. 16, remarque) un $A$-homomorphisme $k' : M'' \to N''$ tel que $g = k'' \circ \alpha$, d’où le lemme.

Lemme 2 bis. — Si, dans le diagramme commutatif de $A$-modules et d’homomorphismes

$$
\begin{array}{ccc}
M' & \xrightarrow{\alpha'} & M \xrightarrow{\alpha} M'' \\
u' \downarrow & & u \downarrow \\
N' & \xrightarrow{\beta'} & N \xrightarrow{\beta} N''
\end{array}
$$

on a $\mathrm{Ker}\, \alpha = \mathrm{Im}\, \alpha', \beta \circ \beta' = 0$ et si $N''$ est injectif, il existe un $A$-homomorphisme $u'' : M'' \to N''$ tel que $u'' \circ \alpha = \beta \circ u$.
Il suffit de poser $u' = k', u = -k, f = 0, f' = 0$ et $k'' = u''$ dans le lemme 1 bis.

#### Proposition 1 {#alg-x-s3-prop-1 .statement}

Soient $(P, d_P)$ et $(E, d_E)$ deux complexes de $A$-modules et $r$ un entier.

a) Soit $(u_i : P_i \to E_i)_{i \leq r}$ une famille d’homomorphismes telle que $d_E \circ u_i = u_{i-1} \circ d_P$ pour $i \leq r$. Supposons que $P_i$ soit projectif pour $i > r$ et que $H_i(E) = 0$ pour $i \geq r$. Alors la famille des $u_i$ se prolonge en un morphisme de complexes de $P$ dans $E$; deux tels prolongements sont homotopes.

b) Soit $(u^i : P^i \to E^i)_{i \leq r}$ une famille d’homomorphismes telle que $u^i \circ d_P = d_E \circ u^{i-1}$ pour $i \leq r$. Supposons que $E^i$ soit injectif pour $i > r$ et que $H^i(P) = 0$ pour $i \geq r$. Alors la famille des $u^i$ se prolonge en un morphisme de complexes de $P$ dans $E$; deux tels prolongements sont homotopes.

Démontrons a). L’existence d’un prolongement $v$ de la famille $(u_i)_{i \leq r}$ résulte aussitôt du lemme 2 par récurrence. Soit $v'$ un autre prolongement ; posons $f = v' - v$, et construisons par récurrence sur l’entier $n$ un homomorphisme $k_n : P_n \to E_{n+1}$ tel que $f_n = d_E \circ k_n + k_{n-1} \circ d_P$. Pour $i \leq r$, on prend $k_i = 0$. Soit $n \geq r$ et supposons les $k_i$ construits pour $i \leq n$. Considérons alors le diagramme

$$
\begin{array}{cccccc}
P_{n+1} & \xrightarrow{d_P} & P_n & \xrightarrow{d_P} & P_{n-1} \\
f_{n+1} \downarrow & & & & k_{n-1} \downarrow \\
E_{n+2} & \xrightarrow{d_E} & E_{n+1} & \xrightarrow{d_E} & E_n .
\end{array}
$$

Les hypothèses du lemme 1 sont satisfaites ; il existe donc un $A$-homomorphisme $k_{n+1} : P_{n+1} \to E_{n+2}$ tel que $f_{n+1} = d_E \circ k_{n+1} + k_n \circ d_P$, d’où a).

La démonstration de b) est analogue, via les lemmes 1 bis et 2 bis.

### 2. Résolutions

Dans la suite, on identifie toujours un module au complexe dont il est la composante de degré zéro et dont toutes les autres composantes sont nulles.

#### Définition 1 {#alg-x-s3-def-1 .statement}

Soit $M$ un $A$-module. Une résolution gauche de $M$ est un couple $(P,p)$ où $P$ est un complexe nul à droite et $p:P\to M$ est un homomorphisme. Une résolution droite de $M$ est un couple $(e,E)$ où $E$ est un complexe nul à gauche et $e:M\to E$ un homomorphisme.

On appelle longueur de la résolution $(P,p)$ (resp. $(e,E)$) la longueur du complexe $P$ (resp. $E$). Si $(P,p)$ et $(P',p')$ (resp. $(e,E)$ et $(e',E')$) sont deux résolutions gauches (resp. droites) de $M$, un morphisme de complexes $f:P\to P'$ tel que $p'\circ f=p$ (resp. $g:E\to E'$ tel que $g\circ e=e'$) est appelé un morphisme de résolutions.

#### Proposition 2 {#alg-x-s3-prop-2 .statement}

Soient $P$ un complexe nul à droite et $p:P\to M$ un morphisme.
Pour que $(P,p)$ soit une résolution gauche de $M$, il faut et il suffit que la suite

(1)

$$
\cdots\longrightarrow P_n\xrightarrow{d_P}P_{n-1}\longrightarrow\cdots\longrightarrow P_1\xrightarrow{d_P}P_0\xrightarrow{p}M\longrightarrow0
$$

soit exacte.

En effet, dire que $p:P\to M$ est un homomorphisme signifie que $H_i(P)=0$ pour $i>0$ et que $p_0$ induit un isomorphisme de $\operatorname{Coker}(d_P:P_1\to P_0)$ sur $M$.

De même :

**Proposition 2bis.** — Soient $E$ un complexe nul à gauche et $e:M\to E$ un morphisme.
Pour que $(e,E)$ soit une résolution droite de $M$, il faut et il suffit que la suite

(1 bis)

$$
0\longrightarrow M\xrightarrow{e_0}E^0\xrightarrow{d_E}E^1\longrightarrow\cdots\longrightarrow E^n\xrightarrow{d_E}E^{n+1}\longrightarrow\cdots
$$

soit exacte.

Par abus de langage, on dit souvent que la suite (1) (resp. (1 bis)) est une résolution gauche (resp. droite) de $M$.

#### Définition 2 {#alg-x-s3-def-2 .statement}

Une résolution projective (resp. libre, resp. plate) du $A$-module $M$ est une résolution gauche $(P,p)$ de $M$ telle que le complexe $P$ soit projectif (resp. libre, resp. plat) (X, p. 25). Une résolution injective de $M$ est une résolution droite $(e,E)$ de $M$ telle que le complexe $E$ soit injectif (loc. cit.).

#### Exemple 1 {#alg-x-s3-n2-exa-1 .statement}

Supposons que l’anneau $A$ soit principal ; soient $M$ un $A$-module et $(x_i)_{i\in I}$ une famille génératrice de $M$. Notons $L_0$ le module libre $A^{(I)}$, $(e_i)$ sa base canonique et définissons $p:L_0\to M$ par $p(e_i)=x_i$. Le morphisme $p$ est surjectif et son noyau $L_1$ est un $A$-module libre d’après VII, § 3, cor. 2 au th. 1, donc la suite exacte

$$
0\longrightarrow L_1\longrightarrow L_0\xrightarrow{p}M\longrightarrow0
$$

est une résolution libre de $M$ de longueur 1. Si $I$ est fini, $L_0$ et $L_1$ sont de type fini.

#### Exemple 2 {#alg-x-s3-n2-exa-2 .statement}

Supposons A commutatif ; soient E un A-module et u un endomorphisme de E. Notons $E_u$ le $A[X]$-module obtenu en munissant E de la structure définie par

$$
(p, x) \mapsto p(u)(x) \quad \text{pour} \quad p \in A[X] \quad \text{et} \quad x \in E.
$$

D’après III, p. 106, on a une suite exacte :

$$
0 \to A[X] \otimes_A E \xrightarrow{\psi} A[X] \otimes_A E \xrightarrow{\varphi} E_u \to 0
$$

où $\varphi(p \otimes x) = p.x$ et $\psi(p \otimes x) = Xp \otimes x - p \otimes u(x)$ pour $p \in A[X]$ et $x \in E$. Cette suite exacte est une résolution de longueur 1 de $E_u$, libre (resp. projective, resp. de type fini) si E est un A-module libre (resp. projectif, resp. de type fini).

#### Exemple 3 {#alg-x-s3-n2-exa-3 .statement}

Si A est principal, la suite exacte

$$
0 \to A \to K \to K/A \to 0
$$

est une résolution injective de longueur 1 du A-module $A_s$ (X, p. 18, exemple 1).

#### Proposition 3 {#alg-x-s3-prop-3 .statement}

Soient $f : M' \to M$ un homomorphisme de A-modules, $p' : P' \to M'$ un morphisme dans $M'$ d’un complexe nul à droite et projectif $P'$, et $p : P \to M$ une résolution gauche de M. Il existe un morphisme de complexes $\tilde{f} : P' \to P$, et un seul à homotopie près, tel que $p \circ \tilde{f} = f \circ p'$.

Considérons le complexe $\overline{P}$ défini comme suit : $\overline{P}_n = P_n$ pour $n \neq -1$, $\overline{P}_{-1} = M$, $d_{\overline{P},n} = d_{P,n}$ pour $n \neq 0, -1$, $d_{\overline{P},0} = p_0$, $d_{\overline{P},-1} = 0$, et le complexe $\overline{P}'$ défini de façon analogue. Appliquant aux complexes $\overline{P}$ et $\overline{P}'$ la prop. 1 a) avec $r = 0$, $u_i = 0$ pour $i < -1$ et $u_{-1} = f$, on obtient la prop. 3.

#### Corollaire {#alg-x-s3-n2-cor-1 .statement}

Soient $(P, p)$ et $(P', p')$ deux résolutions projectives de M. Il existe un homotopisme et un seul à homotopie près $\alpha : P' \to P$ tel que $p \circ \alpha = p'$.

En effet, il existe un morphisme $\alpha : P' \to P$ (resp. $\beta : P \to P'$) tel que $p \circ \alpha = p'$ (resp. $p' \circ \beta = p$). Comme $p \circ \alpha \circ \beta = p$ (resp. $p' \circ \beta \circ \alpha = p'$), $\alpha \circ \beta$ est homotope à $1_P$ (resp. $\beta \circ \alpha$ est homotope à $1_{P'}$).

PROPOSITION 3 bis. — Soient $g : N \to N'$ un homomorphisme de A-modules, $e' : N' \to E'$ un morphisme de $N'$ dans un complexe nul à gauche et injectif $E'$, et $e : N \to E$ une résolution droite de N. Il existe un morphisme de complexes $\tilde{g} : E \to E'$, et un seul à homotopie près, tel que $\tilde{g} \circ e = e' \circ g$.

Cela se démontre comme la prop. 3 à l’aide de la prop. 1 b).

#### Corollaire {#alg-x-s3-n2-cor-2 .statement}

Soient $(e, E)$ et $(e', E')$ deux résolutions injectives de N ; il existe un homotopisme $\alpha : E \to E'$ et un seul à homotopie près tel que $\alpha \circ e = e'$.

### 3. La résolution libre canonique

Pour tout A-module M, notons L_0(M) le A-module libre A^{(M)} de base M, (e_m)_{m \in M} sa base canonique et $p_M : L_0(M) \to M$ l’homomorphisme tel que
$$
p_M(e_m) = m , \quad m \in M .
$$
Posons $Z_0(M) = \mathrm{Ker}\, p_M$ et soit $i_M : Z_0(M) \to L_0(M)$ l’injection canonique. On a une suite exacte
$$
(1) \qquad 0 \longrightarrow Z_0(M) \xrightarrow{i_M} L_0(M) \xrightarrow{p_M} M \longrightarrow 0 .
$$
On définit un module gradué L(M) en posant $L_n(M) = 0$ pour $n < 0$ et, par récurrence sur l’entier $n > 0$
$$
(2) \qquad L_n(M) = L_0(Z_{n-1}(M)) ; \qquad Z_n(M) = Z_0(Z_{n-1}(M)) .
$$
On définit des A-homomorphismes $d_n^M : L_n(M) \to L_{n-1}(M)$ par
$$
(3) \qquad \left\{ \begin{array}{ll}
d_n^M = 0 , & n \leqslant 0 , \\
d_1^M = i_M \circ p_{Z_0(M)} , \\
d_n^M = i_{Z_{n-2}(M)} \circ p_{Z_{n-1}(M)} , & n > 1 .
\end{array} \right.
$$
On a par construction une suite exacte
$$
\longrightarrow L_n(M) \xrightarrow{d_n^M} L_{n-1}(M) \longrightarrow \cdots \longrightarrow L_0(M) \xrightarrow{p_M} M \longrightarrow 0 ,
$$
de sorte que, si l’on étend $p_M$ en un morphisme de complexes
$$
p_M : (L(M), d^M) \to M ,
$$
on obtient une résolution libre de M, dite résolution libre canonique de M.

Soit $f : M \to N$ un homomorphisme de A-modules. Notons
$$
L_0(f) : L_0(M) \to L_0(N)
$$
l’unique A-homomorphisme tel que $L_0(f)(e_m) = e_{f(m)}$ pour tout $m \in M$. On a
$$
(4) \qquad p_N \circ L_0(f) = f \circ p_M .
$$
Par suite, $L_0(f)$ induit un A-homomorphisme $Z_0(f) : Z_0(M) \to Z_0(N)$ et on a
$$
(5) \qquad i_N \circ Z_0(f) = L_0(f) \circ i_M .
$$
Posons $L_n(f) = 0$, pour $n < 0$ et définissons par récurrence sur l’entier $n > 0$, des homomorphismes $L_n(f) : L_n(M) \to L_n(N)$ et $Z_n(f) : Z_n(M) \to Z_n(N)$ par
$$
(6) \qquad \left\{ \begin{array}{l}
L_n(f) = L_0(Z_{n-1}(f)) \\
Z_n(f) = Z_0(Z_{n-1}(f)) .
\end{array} \right.
$$

#### Proposition 4 {#alg-x-s3-prop-4 .statement}

$L(f) : L(M) \to L(N)$ est un morphisme de complexes de A-modules ; on a $p_M \circ L(f) = f \circ p_N$.

Il s’agit de prouver, pour tout entier $n > 0$, la formule

$$
d_n^N \circ L_n(f) = L_{n-1}(f) \circ d_n^M .
$$

On a d’abord

$$
\begin{align*}
d_1^N \circ L_1(f) &= i_N \circ p_{Z_0(N)} \circ L_0(Z_0(f)) & \text{(d’après (3) et (6))} \\
&= i_N \circ Z_0(f) \circ p_{Z_0(M)} & \text{(d’après (4))} \\
&= L_0(f) \circ i_M \circ p_{Z_0(M)} & \text{(d’après (5))} \\
&= L_0(f) \circ d_1^M & \text{(d’après (3))} .
\end{align*}
$$

Lorsque $n > 1$, on a successivement

$$
\begin{align*}
d_n^N \circ L_n(f) &= i_{Z_{n-2}(N)} \circ p_{Z_{n-1}(N)} \circ L_0(Z_{n-1}(f)) & \text{(d’après (3) et (6))} \\
&= i_{Z_{n-2}(N)} \circ Z_{n-1}(f) \circ p_{Z_{n-1}(M)} & \text{(d’après (4))} \\
&= i_{Z_{n-2}(N)} \circ Z_0(Z_{n-2}(f)) \circ p_{Z_{n-1}(M)} & \text{(d’après (6))} \\
&= L_0(Z_{n-2}(f)) \circ i_{Z_{n-2}(M)} \circ p_{Z_{n-1}(M)} & \text{(d’après (5))} \\
&= L_{n-1}(f) \circ d_n^M & \text{(d’après (3) et (6))} .
\end{align*}
$$

On a aussitôt

(7)
$$
L(1_M) = 1_{L(M)} .
$$

D’autre part, si $g : N \to P$ est un homomorphisme de A-modules, on a

(8)
$$
L(g \circ f) = L(g) \circ L(f) .
$$

En effet, on a pour $m \in M$,
$$
L_0(g \circ f)(e_m) = e_{g \circ f(m)} = L_0(g)(e_{f(m)}) = L_0(g) \circ L_0(f)(e_m) ,
$$
donc $L_0(g \circ f) = L(g) \circ L(f)$; par conséquent $Z_0(g \circ f) = Z_0(g) \circ Z_0(f)$; d’où aussitôt $L_n(g \circ f) = L_n(g) \circ L_n(f)$, pour $n \geqslant 0$, par récurrence sur $n$, d’où (8).

#### Remarque {#alg-x-s3-n3-rem-1 .statement}

Si $f, g \in \mathrm{Hom}_A(M, N)$, on n’a pas $L(f + g) = L(f) + L(g)$. Cependant ces deux morphismes sont homotopes d’après X, p. 49, prop. 3.

Soit $M$ un A-module à droite ; notons $A^\circ$ l’anneau opposé à $A$, $M^\circ$ le $A^\circ$-module sous-jacent à $M$, $L(M^\circ)$ sa résolution libre canonique. On note $L(M)$ et on appelle résolution libre canonique de $M$ le A-complexe $L(M^\circ)^\circ$ sous-jacent à $L(M^\circ)$. On a donc

$$
L(M^\circ) = L(M)^\circ .
$$

### 4. La résolution injective canonique

Soit $F$ le $A$-module $\operatorname{Hom}_{\mathbf Z}(A,\mathbf Q/\mathbf Z)$ ; pour tout $A$-module $M$, on pose $I^0(M)=F^{\operatorname{Hom}_A(M,F)}$ et on note $e_M:M\longrightarrow I^0(M)$ l’homomorphisme qui à $m\in M$ associe la famille $(\varphi(m))_{\varphi\in\operatorname{Hom}_A(M,F)}$. D’après X, p. 19, cor. 2, $I^0(M)$ est un $A$-module injectif et $e_M$ est injectif. Posons $K^0(M)=\operatorname{Coker}e_M$ et notons $q_M:I^0(M)\longrightarrow K^0(M)$ la projection canonique. On a donc une suite exacte

$$
0\longrightarrow M\xrightarrow{e_M} I^0(M)\xrightarrow{q_M} K^0(M)\longrightarrow 0.
$$

On définit un $A$-module gradué $I(M)$ en posant $I^n(M)=0$ pour $n<0$ et, par récurrence sur l’entier $n>0$,

(9)
$$
I^n(M)=I^0(K^{n-1}(M)),\qquad K^n(M)=K^0(K^{n+1}(M)).
$$

On définit des $A$-homomorphismes $\delta_M^n:I^n(M)\longrightarrow I^{n+1}(M)$ par

(10)
$$
\left\{
\begin{aligned}
\delta_M^n&=0, && n<0,\\
\delta_M^0&=\epsilon_{K^0(M)}\circ q_M,\\
\delta_M^n&=\epsilon_{K^n(M)}\circ q_{K^{n-1}(M)}, && n>0.
\end{aligned}
\right.
$$

On a par construction une suite exacte

$$
0\longrightarrow M\xrightarrow{e_M} I^0(M)\xrightarrow{\delta_M^0}\cdots\longrightarrow I^n(M)\xrightarrow{\delta_M^n}I^{n+1}(M)\longrightarrow\cdots,
$$

de sorte que, si l’on étend $e_M$ en un morphisme de complexes

$$
e_M:M\longrightarrow (I(M),\delta_M),
$$

on obtient une résolution injective de $M$, dite résolution injective canonique de $M$.

Soit $f:M\longrightarrow N$ un homomorphisme de $A$-modules. Notons $I^0(f)$ l’homomorphisme de $I^0(M)=F^{\operatorname{Hom}_A(M,F)}$ dans $I^0(N)=F^{\operatorname{Hom}_A(N,F)}$ qui applique la famille $(x_\varphi)_{\varphi\in\operatorname{Hom}_A(M,F)}$ sur la famille $(x_{\psi\circ f})_{\psi\in\operatorname{Hom}_A(N,F)}$. On a :

(11)
$$
I^0(f)\circ e_M=e_N\circ f.
$$

Par suite, $I^0(f)$ induit un homomorphisme $K^0(f):K^0(M)\longrightarrow K^0(N)$ et on a

(12)
$$
K^0(f)\circ q_M=q_N\circ K^0(f).
$$

Posons $I^n(f)=0$ pour $n<0$ et définissons, par récurrence sur l’entier $n>0$, des homomorphismes $I^n(f):I^n(M)\longrightarrow I^n(N)$ et $K^n(f):K^n(M)\longrightarrow K^n(N)$ par :

(13)
$$
\left\{
\begin{aligned}
I^n(f)&=I^0(K^{n-1}(f)),\\
K^n(f)&=K^0(K^{n-1}(f)).
\end{aligned}
\right.
$$

#### Proposition 5 {#alg-x-s3-prop-5 .statement}

I(f) : I(M) → I(N) est un morphisme de complexes de A-modules ; on a I(f) ◦ e_M = e_N ◦ f.
Cela se démontre de manière analogue à la prop. 4.

On a
(14)
$$
I(1_M) = 1_{I(M)}
$$
et pour tout homomorphisme $g : N \to P$ de A-modules
(15)
$$
I(g \circ f) = I(g) \circ I(f) .
$$

#### Remarque {#alg-x-s3-n4-rem-1 .statement}

Si $f, g \in \mathrm{Hom}_A(M, N)$, on n’a pas $I(f + g) = I(f) + I(g)$. Cependant, ces deux morphismes sont homotopes d’après X, p. 49, prop. 3 bis.

Si M est un A-module à droite, on pose $I(M) = I(M^\circ)^\circ$; on l’appelle la résolution injective canonique de M et on a
$$
I(M^\circ) = I(M)^\circ .
$$

### 5. Résolutions de type fini

Il résulte notamment des deux numéros précédents que tout A-module possède des résolutions injectives, des résolutions libres (donc aussi des résolutions projectives ou plates). Dans certains cas, on peut préciser davantage :

Supposons A noethérien à gauche et soit M un A-module. Construisons par récurrence des suites $(L_n)_{n \geq 0}$, $(Z_n)_{n \geq 0}$, $(d_n)_{n \geq 1}$ où, pour tout $n \geq 0$, $L_n$ est un A-module libre de type fini, $Z_n$ un sous-module de $L_n$ et $d_{n+1} : L_{n+1} \to L_n$ un homomorphisme. Pour cela, choisissons une famille génératrice finie $(m_i)_{i \in I_0}$ de M, posons $L_0 = A^{(I_0)}$, définissons $p : L_0 \to M$ par $p(e_i) = m_i$ et posons $Z_0 = \mathrm{Ker}\,(p)$. Pour $n \geq 0$, les modules $L_n$ et $Z_n$ étant construits, $Z_n$ est de type fini puisque contenu dans $L_n$; choisissons une famille génératrice finie $(x_{n,i})_{i \in I_{n+1}}$ de $Z_n$; posons $L_{n+1} = A^{(I_{n+1})}$, définissons $d_{n+1}$ par $d_{n+1}(e_i) = x_{n,i}$ et posons $Z_{n+1} = \mathrm{Ker}\,(d_{n+1})$.

On a par construction une suite exacte
$$
\cdots \longrightarrow L_{n+1} \xrightarrow{d_{n+1}} L_n \longrightarrow \cdots \longrightarrow L_0 \xrightarrow{p} M \longrightarrow 0 ,
$$
d’où :

#### Proposition 6 {#alg-x-s3-prop-6 .statement}

Lorsque A est noethérien à gauche, tout A-module de type fini M possède une résolution libre $p : L \to M$ telle que $L_n$ soit de type fini pour tout entier n.
Plus généralement :

#### Proposition 7 {#alg-x-s3-prop-7 .statement}

Soit C un A-complexe et soit $a \in \mathbf{Z}$ tel que $H_n(C) = 0$ pour $n < a$.
a) Il existe un A-complexe libre L tel que $L_n = 0$ pour $n < a$ et un homologisme $f : L \to C$.

b) Supposons $A$ noethérien à gauche et les $A$-modules $H_n(C)$, $n\in \mathbf{Z}$, de type fini.
Il existe un $A$-complexe libre $L$ tel que $L_n=0$ pour $n<a$ et que $L_n$ soit un $A$-module de type fini pour tout $n$, et un homomorphisme $f:L\to C$.

Soit $C'$ le sous-complexe de $C$ tel que $C'_n=C_n$ pour $n>a$, $C'_a=Z_a(C)$, $C'_n=0$ pour $n<a$ ; alors l’injection canonique de $C'$ dans $C$ est un homomorphisme. Remplaçant $C$ par $C'$, on peut donc supposer que $C_n=0$ pour $n<a$. L’énoncé résulte alors de l’application itérée du lemme suivant, pour $r=a,a+1,\ldots$ :

#### Lemme 3 {#alg-x-s3-lem-3 .statement}

Soient $C$ un complexe et $r\in \mathbf{Z}$. Il existe un complexe $C'$ et un homomorphisme $f:C'\to C$ tels que $f_n:C'_n\to C_n$ soit un isomorphisme pour $n<r$ et que $C'_r$ soit un $A$-module libre. Si $A$ est noethérien et les $A$-modules $H_r(C)$ et $C_{r-1}$ de type fini, on peut imposer que $C'_r$ soit de type fini.

a) Soit d’abord $h:M\to C_r$ un homomorphisme de $A$-modules ; notons $d=(d_n)$ la différentielle de $C$. Soit $N$ le sous-module de $M\times C_{r+1}$ formé des couples $(m,x)$ tels que $h(m)=d_{r+1}(x)$ ; définissons un complexe $(C',d')$ par $C'_n=C_n$ pour $n\ne r,r+1$, $C'_r=M$, $C'_{r+1}=N$, $d'_n=d_n$ pour $n\ne r,r+1$, $d'_r=h$, $d'_{r+1}(m,x)=m$ pour $(m,x)\in N$ et $d'_{r+2}(y)=(0,d_{r+2}(y))$ pour $y\in C_{r+2}$. Considérons aussi le morphisme de complexes $f:C'\to C$ tel que $f_n=1_{C_n}$ pour $n\ne r,r+1$, $f_r=h$, $f_{r+1}(m,x)=x$.

b) Le complexe $\operatorname{Ker}f$ est nul en degré $\ne r,r+1$ et la différentielle $d'_{r+1}$ induit un isomorphisme de $\operatorname{Ker}f_{r+1}$ sur $\operatorname{Ker}f_r$, donc $H(\operatorname{Ker}f)=0$.

c) Lorsque l’application composée $M\xrightarrow{h}C_r\to C_r/B_r(C)$ est surjective, on voit de même que $H(\operatorname{Coker}f)=0$, et $f$ est alors un homomorphisme (X, p. 31, cor. 2).

d) Lorsque $A$ est supposé noethérien et les $A$-modules $H_r(C)$ et $C_{r-1}$ de type fini, alors $C_r/B_r(C)$ est de type fini, en vertu de la suite exacte (X, p. 25)

$$
0\to H_r(C)\to C_r/B_r(C)\to C_{r-1}\ ;
$$

il existe alors un $A$-module libre de type fini $M$ et un homomorphisme $h:M\to C_r$ tel que la condition de c) soit satisfaite ; dans le cas général, il existe un module libre $M$ et un homomorphisme surjectif $h:M\to C_r$. Cela achève la démonstration.

### 6.  Résolutions projectives minimales

Soit $M$ un $A$-module et soit

$$
(P)\qquad \cdots \longrightarrow F_n \xrightarrow{d_n} F_{n-1}\longrightarrow \cdots \longrightarrow F_0\xrightarrow{d_0} M\longrightarrow 0
$$

une résolution de $M$. On dit que $(P)$ est une résolution projective minimale si, pour tout $n\geq 0$, l’homomorphisme $\delta_n:P_n\to \operatorname{Im}(d_n)$ induit par $d_n$ est une couverture projective (VIII, § 8, no 5).

#### Proposition 8 {#alg-x-s3-prop-8 .statement}

Soient $M$ un $A$-module, $P$ et $P'$ deux résolutions projectives minimales de $M$ et $f:P\to P'$ un morphisme de résolutions. Alors $f$ est un isomorphisme.
En particulier, deux résolutions projectives minimales de $M$ sont isomorphes.

Posons $\widetilde P_n=P_n$ pour $n\ne-1$ et $\widetilde P_{-1}=M$ ; définissons de même $\widetilde P'_n$ et posons $f_{-1}=1_M$. Montrons par récurrence à partir de $-1$ que $f_n:\widetilde P_n\to\widetilde P'_n$ est un isomorphisme pour tout $n$. C’est évident pour $n=-1$ ; supposons que $f_n$ et $f_{n-1}$ soient des isomorphismes. Il résulte de la commutativité du diagramme :

$$
\begin{array}{ccc}
P_n & \xrightarrow{\ d_n\ } & P_{n-1}\\
{\scriptstyle f_n}\downarrow && \downarrow{\scriptstyle f_{n-1}}\\
P'_n & \xrightarrow{\ d'_n\ } & P'_{n-1}
\end{array}
$$

que $f_n$ induit un isomorphisme $g_n$ de $\operatorname{Ker}d_n$ sur $\operatorname{Ker}d'_n$. Il résulte alors de la commutativité du diagramme :

$$
\begin{array}{ccc}
P_{n+1} & \xrightarrow{\ \delta_{n+1}\ } & \operatorname{Ker}d_n\\
{\scriptstyle f_{n+1}}\downarrow && \downarrow{\scriptstyle g_n}\\
P'_{n+1} & \xrightarrow{\ \delta'_{n+1}\ } & \operatorname{Ker}d'_n
\end{array}
$$

et de VIII, *loc. cit.*, que $f_{n+1}$ est un isomorphisme.

#### Corollaire {#alg-x-s3-n6-cor-1 .statement}

*Soient $M$ un $A$-module, $P$ et $P'$ deux résolutions projectives de $M$ ; on suppose que $P$ est minimale. Soient $f:P\to P'$ et $g:P'\to P$ deux morphismes de résolutions. Alors $f$ est injectif, $g$ est surjectif, et $P'$ est somme directe des sous-complexes $\operatorname{Im}f$ et $\operatorname{Ker}g$. De plus $\operatorname{Ker}g$ est d’homologie nulle.*

En effet, $\alpha=g\circ f$ est un automorphisme de $P$ (prop. 8). Posons $\widetilde f=f\circ\alpha^{-1}$.

On a

$$
\operatorname{Im}\widetilde f=\operatorname{Im}f
\quad\text{et}\quad
g\circ\widetilde f=1_P,
$$

ce qui montre que $P'=\operatorname{Im}\widetilde f\oplus\operatorname{Ker}g$. Comme la suite

$$
0\longrightarrow\operatorname{Ker}g\longrightarrow P'
\xrightarrow{\ g\ }P\longrightarrow0
$$

est exacte et que $g$ est un homomorphisme, $\operatorname{Ker}g$ est d’homologie nulle.

#### Proposition 9 {#alg-x-s3-prop-9 .statement}

*Soient $M$ un $A$-module et $(P,p)$ une résolution projective de $M$. Notons $r$ le radical de $A$. On suppose, ou bien que $P_n$ est un $A$-module de type fini pour tout $n$, ou bien que $r$ est nilpotent. Alors pour que $(P,p)$ soit minimale, il faut et il suffit que le complexe $(A/r)\otimes_A P$ soit à différentielle nulle, autrement dit que*

$$
d_{n+1}(P_{n+1})\subset rP_n\quad\text{pour tout }n\geq0.
$$

Supposons que $(P,p)$ soit minimale. D’après VIII, *loc. cit.*, l’homomorphisme

$$
1\otimes\delta_n:(A/r)\otimes_A P_n\longrightarrow(A/r)\otimes_A\operatorname{Im}d_n
$$

est un isomorphisme. Il résulte alors de la suite exacte

$$
0\longrightarrow\operatorname{Im}d_{n+1}
\xrightarrow{\ j_n\ }P_n
\xrightarrow{\ \delta_n\ }\operatorname{Im}d_n
\longrightarrow0
$$

que l’homomorphisme $1 \otimes j_n : (A/r) \otimes_A \operatorname{Im} d_{n+1} \to (A/r) \otimes_A P_n$ est nul ; comme $d_{n+1} = j_n \circ \delta_{n+1}$, on en déduit que $1_{A/r} \otimes d_{n+1} = 0$ pour $n \geqslant 0$.

Inversement, supposons que pour tout $n \geqslant 1$, $1 \otimes d_n$ soit nul, autrement dit que $\operatorname{Im} d_n = \operatorname{Ker} d_{n-1}$ soit contenu dans $rP_{n-1}$. Puisque $\delta_{n-1}$ est surjectif, il résulte de VIII, loc. cit. que $\delta_{n-1}$ est une couverture projective pour $n \geqslant 1$, donc que $(P, p)$ est minimale.

#### Proposition 10 {#alg-x-s3-prop-10 .statement}

*Supposons que A soit un anneau local nœthérien à gauche, et soit M un A-module de type fini. Alors M possède une résolution minimale (P, p) ; pour tout $n \geqslant 0$, $P_n$ est un module libre de type fini.*

En effet, dans la construction faite au n° 5 (p. 53), on peut en vertu de VIII, loc. cit. prendre pour $(L_0, p)$ une couverture projective de M, et pour $L_{n+1}$ une couverture projective de $\operatorname{Ker} d_n$. La résolution obtenue est alors minimale.

*Remarques. — 1) Notons m l’idéal maximal de A et posons $k = A/m$. Soit P une résolution projective minimale de M, et posons $b_n = \dim_k (k \otimes_A P_n)$. Alors $P_n$ est un A-module libre de rang $b_n$. Il résulte du corollaire de la prop. 8 que pour toute autre résolution projective $P'$ de M, on a $\dim_k (k \otimes_A P'_n) \geqslant b_n$, et que l’égalité a lieu si et seulement si $P'$ est minimale.

2) D’après la prop. 9, $b_n$ est la dimension sur $k$ de $H_n(k \otimes_A P)$, *autrement dit de $\operatorname{Tor}_n^A(k, M)$*. C’est aussi la dimension sur $k$ de $\operatorname{Ext}_A^n(M, k)$ (*cf. X, p. 103, remarque 3)*.

### 7. Résolutions graduées

Dans ce numéro, on suppose que l’anneau A est muni d’une graduation $(A_n)_{n \in \mathbf{Z}}$, telle que $A_n = 0$ pour $n < 0$. On dit qu’un A-module gradué M est *borné inférieurement* si $M_n = 0$ pour $n$ assez petit ; tout A-module gradué de type fini est borné inférieurement.

#### Proposition 11 {#alg-x-s3-prop-11 .statement}

*Si M est un A-module gradué borné inférieurement (resp. si M est un A-module gradué de type fini et si A est nœthérien à gauche), il existe une suite exacte illimitée à gauche de A-modules gradués*

$$
\cdots \longrightarrow L_n \xrightarrow{d_n} L_{n-1} \longrightarrow \cdots \longrightarrow L_1 \xrightarrow{d_1} L_0 \xrightarrow{d_0} M \longrightarrow 0
$$

*où les $L_i$ sont gradués libres et bornés inférieurement (resp. gradués libres et de type fini), et où les $d_i$ sont des homomorphismes gradués de degré 0.*

Si N est un A-module gradué et borné inférieurement (resp. et de type fini sur A nœthérien) il existe un A-module gradué libre et borné inférieurement (resp. et de type fini) L et un homomorphisme gradué surjectif $L \to N$ (II, p. 167, *remarque 3*).

Cela étant, supposons donnée une suite exacte de A-modules gradués et d’homomorphismes gradués de degré 0

$$
L_n \xrightarrow{d_n} L_{n-1} \longrightarrow \cdots \longrightarrow L_0 \xrightarrow{d_0} M \longrightarrow 0,
$$

où les $L_i, i = 0, \ldots, n$, sont gradués libres et bornés inférieurement (resp. gradués libres et de type fini). Alors $N = \mathrm{Ker}\, d_n$ est borné inférieurement (resp. de type fini) ; il existe donc un A-module gradué libre et borné inférieurement (resp. gradué libre et de type fini) $L_{n+1}$ et un homomorphisme gradué $d_{n+1} : L_{n+1} \to L_n$ de degré 0, tel que $\mathrm{Im}\, d_{n+1} = N$; la suite

$$
L_{n+1} \xrightarrow{d_{n+1}} L_n \xrightarrow{d_n} L_{n-1} \longrightarrow \cdots \longrightarrow L_0 \xrightarrow{d_0} M \longrightarrow 0
$$

est alors exacte. La proposition résulte alors de ce qui précède par récurrence sur $n$.

### 8. La résolution standard

Dans ce numéro, on suppose que l’anneau $A$ est une algèbre (associative et unifière) sur un anneau commutatif $k$. Pour $n \geqslant 0$, on note $B_n$ le produit tensoriel sur $k$ de $(n + 2)$ modules égaux à $A$. On le considère comme un $(A, A)$-bimodule en le munissant de la structure de A-module à gauche (resp. à droite) déduite de la structure de A-module à gauche (resp. à droite) du premier (resp. du dernier) facteur du produit tensoriel.

Pour $n \geqslant 1$, on définit des homomorphismes de bimodules $d_n^i$ (pour $0 \leqslant i \leqslant n$) et $d_n$ de $B_n$ dans $B_{n-1}$, par les formules :

$$
d_n^i(x_0 \otimes \ldots \otimes x_{n+1}) = x_0 \otimes \ldots \otimes x_i\, x_{i+1} \otimes \ldots \otimes x_{n+1}, \quad 0 \leqslant i \leqslant n,
$$
$$
d_n = \sum_{i=0}^n (-1)^i d_n^i.
$$

Il est clair que
$$
d_{n-1}^i \circ d_n^j = d_{n-1}^{j-1} \circ d_n^i \quad \text{pour} \quad i < j
$$
et par suite
$$
d_{n-1} \circ d_n = \sum_{0 \leqslant i < j \leqslant n} (-1)^{i+j} d_{n-1}^i \circ d_n^j + \sum_{0 \leqslant j \leqslant i \leqslant n-1} (-1)^{i+j} d_{n-1}^i \circ d_n^j = 0.
$$

Par conséquent, si l’on pose $B_n = 0$ pour $n < 0$ et $d_n = 0$ pour $n \leqslant 0$, la suite $(B_n, d_n)$ définit un complexe de $(A, A)$-bimodules (X, p. 43), qui sera noté $B(A)$. Pour tout A-module à gauche $M$, on note $B(A, M)$ le complexe formé des $B_n \otimes_A M$ et des $d_n \otimes 1_M$, \* autrement dit le complexe produit tensoriel $B(A) \otimes_A M *$; c’est un complexe de A-modules à gauche.

On définit une application A-linéaire $\varepsilon_M$ de $B_0(A, M) = (A \otimes_k A) \otimes_A M$ dans $M$ par la formule $\varepsilon_M(a \otimes b \otimes m) = abm$ pour $a, b \in A, m \in M$. On a $\varepsilon_M \circ d_1 = 0$, de sorte que l’homomorphisme gradué $\overline{\varepsilon}_M : B(A, M) \to M$, qui coïncide avec $\varepsilon_M$ en degré 0, est un morphisme de complexes de A-modules.

#### Proposition 12 {#alg-x-s3-prop-12 .statement}

L’application $\overline{\varepsilon}_M : B(A, M) \to M$ est un homotopisme de complexes de $k$-modules. En particulier, le complexe $B(A, M)$ est scindé sur $k$, et $(B(A, M), \overline{\varepsilon}_M)$ est une résolution gauche du $A$-module $M$.

Pour $n \geqslant 0$, définissons une application $k$-linéaire $s_n : B_n \to B_{n+1}$ par la formule :

$$
s_n(x_0 \otimes \ldots \otimes x_{n+1}) = 1 \otimes x_0 \otimes \ldots \otimes x_{n+1} \quad \text{pour } x_0, \ldots, x_{n+1} \in A .
$$

C’est un homomorphisme de $A$-modules à droite, qui vérifie les identités :

$$
d_{n+1}^i \circ s_n = s_{n-1} \circ d_n^{i-1} \quad \text{pour } n \geqslant 1 , \quad 1 \leqslant i \leqslant n + 1 ,
$$
$$
d_{n+1}^0 \circ s_n = 1_{B_n} \qquad \text{pour } n \geqslant 1 ,
$$

et on a par suite

(16)
$$
d_{n+1} \circ s_n + s_{n-1} \circ d_n = 1_{B_n} \quad \text{pour } n \geqslant 1 .
$$

De plus, on a

(17)
$$
d_1 \circ s_0(x_0 \otimes x_1) = x_0 \otimes x_1 - 1 \otimes x_0 x_1 \quad \text{pour } x_0, x_1 \in A .
$$

Notons $\eta : A \to A \otimes_k A$ l’application définie par $\eta(a) = 1 \otimes a$, et $\overline{\eta} : A \to B(A)$ le morphisme de complexes qui coïncide avec $\eta$ en degré 0. Il est clair que $\overline{\varepsilon}_A \circ \overline{\eta} = 1_A$; les formules (16) et (17) montrent que $d \circ s + s \circ d = 1_{B(A)} - \overline{\eta} \circ \overline{\varepsilon}_A$. Posant $\overline{\eta}_M = \overline{\eta} \otimes 1_M$, $d_M = d \otimes 1_M$ et $s_M = s \otimes 1_M$, on en déduit que $\overline{\varepsilon}_M \circ \overline{\eta}_M = 1_M$ et $d_M \circ s_M + s_M \circ d_M = 1_{B(A,M)} - \overline{\eta}_M \circ \overline{\varepsilon}_M$. Autrement dit, (X, p. 33, déf. 5), $\overline{\varepsilon}_M$ est un homotopisme de complexes de $k$-modules. Les autres assertions de la proposition s’en déduisent aussitôt.

#### Définition 3 {#alg-x-s3-def-3 .statement}

La résolution gauche $(B(A, M), \overline{\varepsilon}_M)$ de $M$ s’appelle la résolution standard du $A$-module $M$.

Si $A$ et $M$ sont des $k$-modules projectifs (resp. libres, resp. plats), la résolution standard $B(A, M)$ est une résolution projective (resp. libre, resp. plate) de $M$.

### 9. Résolutions et groupes de Grothendieck

Si $\mathcal{C}$ est un ensemble de classes de $A$-modules, on dira qu’une résolution gauche $(P, p)$ est bornée de type $\mathcal{C}$ si le complexe $P$ est borné de type $\mathcal{C}$ (X, p. 41).

#### Théorème 1 {#alg-x-s3-thm-1 .statement}

Soient $\mathcal{C}_0$ et $\mathcal{C}$ deux ensembles additifs et exacts à gauche de classe de $A$-modules tels que $\mathcal{C}_0 \subset \mathcal{C}$ et que tout $A$-module de type $\mathcal{C}$ possède une résolution gauche bornée de type $\mathcal{C}_0$. Alors l’homomorphisme $\alpha : K(\mathcal{C}_0) \to K(\mathcal{C})$ déduit de l’inclusion de $\mathcal{C}_0$ dans $\mathcal{C}$ est bijectif ; si $M$ est un $A$-module de type $\mathcal{C}$ et $P$ une résolution gauche de $M$ bornée de type $\mathcal{C}_0$, on a $\alpha^{-1}([M]_{\mathcal{C}}) = \chi_{\mathcal{C}_0}(P)$ (X, p. 41, exemple 6).

#### Lemme 4 {#alg-x-s3-lem-4 .statement}

Soient $f : M' \to M$ un homomorphisme de $A$-modules de type $\mathcal{C}$, et $p : P \to M$ une résolution gauche de $P$ bornée de type $\mathcal{C}_0$. Il existe une résolution gauche $p' : P' \to M'$ bornée de type $\mathcal{C}_0$ et un morphisme de complexes $u : P' \to P$ tel que $p \circ u = f \circ p'$.

Raisonnons par récurrence sur la longueur $n$ de $P$, l’assertion étant triviale lorsque celle-ci est $< 0$. Considérons l’application $g : M' \times P_0 \to M$ telle que

$$
g(x, r') = f(x) - p_0(r')
$$
pour $x \in M', r' \in P_0$,

et son noyau $K$; le $A$-module $K$ est de type $\mathcal{C}$ puisque $g$ est surjective et que $M' \times P_0$ et $M$ sont de type $\mathcal{C}$. Soit $h : P'_0 \to K$ un homomorphisme surjectif où $P'_0$ est de type $\mathcal{C}_0$; notons $p'_0 : P'_0 \to M'$ (resp. $u_0 : P'_0 \to P_0$) l’homomorphisme composé de $h$ et de la projection $K \to M$ (resp. $K \to P_0$); l’homomorphisme $p'_0$ est surjectif et on a un diagramme commutatif

$$
\begin{array}{ccc}
P'_0 & \xrightarrow{u_0} & P_0 \\
p'_0 \downarrow & & \downarrow p_0 \\
M' & \xrightarrow{f} & M .
\end{array}
$$

Il suffit alors d’appliquer l’hypothèse de récurrence à l’homomorphisme

$$
\operatorname{Ker} p'_0 \to \operatorname{Ker} p_0
$$

déduit de $u_0$.

#### Lemme 5 {#alg-x-s3-lem-5 .statement}

Considérons un diagramme commutatif

$$
\begin{array}{ccc}
P' & \xrightarrow{u} & P \\
p' \downarrow & & \downarrow p \\
0 & \xrightarrow{f} & M \to M'' \to 0
\end{array}
$$

où $(P, p)$ (resp. $(P', p')$) est une résolution gauche de $M$ (resp. $M'$), et où la ligne horizontale du bas est une suite exacte. Il existe un homologisme $p'' : \operatorname{Con}(u) \to M''$.

En effet, la suite exacte (X, p. 37, prop. 7)

$$
0 \to P \xrightarrow{\pi} \operatorname{Con}(u) \xrightarrow{\delta} P'(-1) \to 0
$$

donne une suite exacte d’homologie

$$
\to H_n(P) \to H_n(\operatorname{Con}(u)) \to H_{n-1}(P') \to \cdots
$$
$$
\cdots \to H_1(\operatorname{Con}(u)) \to H_0(P') \xrightarrow{\hat{\partial}} H_0(P) \to H_0(\operatorname{Con}(u)) \to 0 .
$$

D’après X, p. 38, lemme 3 a), on a $\partial = - H_0(u)$. Comme $H_n(P) = 0 = H_n(P')$ pour $n > 0$ et que $H_0(u) : H_0(P') \to H_0(P)$ s’identifie à $f : M' \to M$, on en conclut que $H_n(\operatorname{Con}(u)) = 0$ pour $n > 0$ et que $H_0(\operatorname{Con}(u))$ est isomorphe à $M''$, d’où le lemme.

Démontrons maintenant le théorème.

a) Soit M un A-module de type $\mathcal{C}$. Pour toute résolution gauche $(P, p)$ de M bornée de type $\mathcal{C}_0$, l’élément $\chi_{\mathcal{C}_0}(P)$ de $K(\mathcal{C}_0)$ ne dépend que de M. En effet, soient $(P_1, p_1)$ et $(P_2, p_2)$ deux résolutions de ce type. Considérons la résolution
$$
(P_1 \times P_2, p_1 \times p_2)
$$
du A-module $M \times M$ et l’homomorphisme $\Delta : x \mapsto (x, x)$ de M dans $M \times M$. D’après le lemme 4, il existe une résolution $(Q, q)$ de M bornée de type $\mathcal{C}_0$ et un diagramme commutatif
$$
\begin{array}{ccc}
Q & \xrightarrow{u} & P_1 \times P_2 \\
q \downarrow & & \downarrow p_1 \times p_2 \\
M & \xrightarrow{\Delta} & M \times M ;
\end{array}
$$
on en déduit un diagramme commutatif
$$
\begin{array}{ccc}
Q & \xrightarrow{u \circ pr_i} & P_i \\
q \downarrow & & \downarrow p_i \\
M & \xrightarrow{1_M} & M , \quad i = 1, 2 .
\end{array}
$$
D’après le lemme 5, Con $(u \circ pr_i)$ est d’homologie nulle, donc $u \circ pr_i$ est un homologisme et $\chi_{\mathcal{C}_0}(Q) = \chi_{\mathcal{C}_0}(P_i)$ (X, p. 41, prop. 10); il s’ensuit que $\chi_{\mathcal{C}_0}(P_1) = \chi_{\mathcal{C}_0}(P_2)$ comme annoncé.

b) Pour tout A-module M de type $\mathcal{C}$, soit $\varphi(M) \in K(\mathcal{C}_0)$ la valeur commune des $\chi_{\mathcal{C}_0}(P)$ pour toutes les résolutions gauches P de M bornées de type $\mathcal{C}_0$. Montrons que la fonction $\varphi : \mathcal{C} \to K(\mathcal{C}_0)$ est additive. Soit donc
$$
0 \to M' \xrightarrow{f} M \to M'' \to 0
$$
une suite exacte de A-modules de type $\mathcal{C}$. D’après le lemme 4, il existe un diagramme commutatif
$$
\begin{array}{ccc}
P' & \xrightarrow{u} & P \\
p' \downarrow & & \downarrow p \\
0 & \xrightarrow{f} & M \xrightarrow{g} M'' \to 0
\end{array}
$$
où $(P, p)$ et $(P', p')$ sont des résolutions gauches bornées de type $\mathcal{C}_0$. Alors on a
$$
\varphi(M) = \chi_{\mathcal{C}_0}(P) , \qquad \varphi(M') = \chi_{\mathcal{C}_0}(P')
$$
et d’après le lemme 5
$$
\varphi(M'') = \chi_{\mathcal{C}_0}(\mathrm{Con}\,(u)) = \chi_{\mathcal{C}_0}(P) - \chi_{\mathcal{C}_0}(P') = \varphi(M) - \varphi(M') ;
$$
ce qu’on voulait démontrer.

c) Soit alors $\beta : K(\mathscr{C}) \to K(\mathscr{C}_0)$ l’homomorphisme tel que, avec les notations précédentes, on ait $\beta([M]_{\mathscr{C}})=\chi_{\mathscr{C}_0}(P)$. Comme $p$ est un homomolisme, on a $\chi_{\mathscr{C}}(P)=[M]_{\mathscr{C}}$, donc $\alpha\circ\beta([M]_{\mathscr{C}})=\alpha(\chi_{\mathscr{C}_0}(P))=\chi_{\mathscr{C}}(P)=[M]_{\mathscr{C}}$ et $\alpha\circ\beta=1_{K(\mathscr{C})}$. Si $M$ est de type $\mathscr{C}_0$, alors $(M,1_M)$ est une résolution de $M$, donc $\varphi(M)=[M]_{\mathscr{C}_0}$ et $\beta\circ\alpha=1_{K(\mathscr{C}_0)}$, ce qui achève la démonstration.

Nous appliquerons ce théorème aux modules de « dimension projective finie » au § 8 (X, p. 137).

## EXERCICES {#alg-x-s3-exercises}

See the [exercises for § 3](exercises/s3/).
