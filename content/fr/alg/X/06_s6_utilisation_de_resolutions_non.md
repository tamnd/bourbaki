---
book: alg
book_title: Algebra
chapter: X
chapter_title: ALGÈBRE HOMOLOGIQUE
section: 6
section_title: Utilisation de résolutions non canoniques
lang: fr
source: alg-x-fr
book_pages: A X.100-A X.113, A X.189-A X.197
pdf_pages: 0106-0119, 0195-0203
extraction: ocr
subsections:
    - "no": 1
      title: Calcul des modules $\mathrm{Tor}^A(P, M)$ et $\mathrm{Ext}_A(M, N)$
      page: 100
      pdf_page: 106
    - "no": 2
      title: Calcul des applications $\mathrm{Tor}^A(g, f)$ et $\mathrm{Ext}_A(f, h)$
      page: 103
      pdf_page: 109
    - "no": 3
      title: Calcul des homomorphismes de liaison
      page: 104
      pdf_page: 110
    - "no": 4
      title: Finitude des modules d’extensions et de torsion
      page: 107
      pdf_page: 113
    - "no": 5
      title: Les homomorphismes $\operatorname{Tor}^{B}(P,N) \otimes_{A} Q \to \operatorname{Tor}^{B}(P,N \otimes_{A} Q)$ et $\operatorname{Ext}_{B}(M,N) \otimes_{A} Q \to \operatorname{Ext}_{B}(M,N \otimes_{A} Q)$
      page: 108
      pdf_page: 114
    - "no": 6
      title: Les homomorphismes $\mathrm{Tor}^B(P, N \otimes_A Q) \to \mathrm{Tor}^A(P \otimes_B N, Q)$ et $\mathrm{Ext}_A(Q, \mathrm{Hom}_B(N, M)) \to \mathrm{Ext}_B(N \otimes_A Q, M)$
      page: 109
      pdf_page: 115
    - "no": 7
      title: Les homomorphismes $B \otimes_A \mathrm{Tor}^A(E, F) \to \mathrm{Tor}^B(E \otimes_A B, B \otimes_A F)$ et $B \otimes_A \mathrm{Ext}_A(E, F) \to \mathrm{Ext}_B(B \otimes_A E, B \otimes_A F)$
      page: 110
      pdf_page: 116
    - "no": 8
      title: 'Application : homologie et cohomologie des groupes'
      page: 111
      pdf_page: 117
statements: 30
exercises: 18
content_sha256: 908be744602e152c7d063ad7bc7de7071838f03e3a57fb041dfa7346f158a9b6
---

## § 6. UTILISATION DE RÉSOLUTIONS NON CANONIQUES

On reprend les conventions du § 4.

### 1. Calcul des modules $\mathrm{Tor}^A(P, M)$ et $\mathrm{Ext}_A(M, N)$

Soient $M, N$ des $A$-modules à gauche, $P$ un $A$-module à droite. Soient d’autre part $a : R \to M$ une résolution gauche de $M$, $b : S \to P$ une résolution gauche de $P$ et $c : N \to E$ une résolution droite de $N$.

D’après $X$, p. 49, prop. 3 et 3 bis, il existe des morphismes de complexes $\alpha : L(M) \to R$, $\beta : L(P) \to S$, $\gamma : E \to I(N)$ tels que $a \circ \alpha = p_M$, $b \circ \beta = p_P$, $\gamma \circ C = e_N$, et les classes d’homotopie de $\alpha, \beta, \gamma$ ne dépendent que des résolutions données. D’après $X$, p. 64, prop. 3 et $X$, p. 84, prop. 3, les classes d’homotopie des morphismes

$$
\beta \otimes \alpha : L(P) \otimes_A L(M) \to S \otimes_A R,
$$
$$
\mathrm{Homgr}_A(\alpha, \gamma) : \mathrm{Homgr}_A(R, E) \to \mathrm{Homgr}_A(L(M), I(N))
$$

ne dépendent que des résolutions données, d’où par passage à l’homologie des $k$-homomorphismes gradués de degré 0

$$
\psi(S, R) : \mathrm{Tor}^A(P, M) \to H(S \otimes_A R),
$$
$$
\varphi(R, E) : H(\mathrm{Homgr}_A(R, E)) \to \mathrm{Ext}_A(M, N),
$$

indépendants des choix de $\alpha, \beta, \gamma$.

Par exemple, prenant pour $a, b, c$ les applications identiques de $M, P, N$ respectivement, on trouve les homomorphismes $\psi(P, M) : \mathrm{Tor}^A(P, M) \to P \otimes_A M$ et $\varphi(M, N) : \mathrm{Hom}_A(M, N) \to \mathrm{Ext}_A(M, N)$ introduits en $X$, p. 68, remarque 2) et $X$, p. 87, remarque 2).

#### Théorème 1 {#alg-x-s6-thm-1 .statement}

a) Si l’une des résolutions $R$ ou $S$ est plate, alors $\psi(S, R)$ est un isomorphisme de $k$-modules gradués.

b) Si $R$ est projective ou si $E$ est injective, $\varphi(R, E)$ est un isomorphisme de $k$-modules gradués.

a) Supposons par exemple $\mathbf R$ plat, et choisissons $\alpha$ et $\beta$ comme ci-dessus. L’homomorphisme $\beta\otimes\alpha$ est le composé des morphismes

$$
L(P)\otimes_A L(M)\xrightarrow{1_{L(P)}\otimes\alpha}L(P)\otimes_A\mathbf R\xrightarrow{\beta\otimes1_{\mathbf R}}S\otimes_A\mathbf R.
$$

Comme $L(P)$ (resp. $\mathbf R$) est plat et $\alpha$ (resp. $\beta$) est un homomorphisme, $1_{L(P)}\otimes\alpha$ (resp. $\beta\otimes1_{\mathbf R}$) en est un, d’après la prop. 4 de X, p. 67. Donc $\beta\otimes\alpha$ est un homomorphisme et $\psi(S,R)=H(\beta\otimes\alpha)$ est bijectif.

b) On raisonne de même, en utilisant la prop. 4 de X, p. 86.

#### Corollaire {#alg-x-s6-n1-cor-1 .statement}

Si $R$ est une résolution plate de $M$, l’homomorphisme

$$
\psi(P,R):\operatorname{Tor}^A(P,M)\longrightarrow H(P\otimes_A R)
$$

est bijectif. Si $R$ est une résolution projective de $M$, l’homomorphisme

$$
\varphi(R,N):H(\operatorname{Homgr}_A(R,N))\longrightarrow \operatorname{Ext}_A(M,N)
$$

est bijectif. Si $E$ est une résolution injective de $N$, l’homomorphisme

$$
\varphi(M,E):H(\operatorname{Homgr}_A(M,E))\longrightarrow \operatorname{Ext}_A(M,N)
$$

est bijectif.

#### Remarque {#alg-x-s6-n1-rem-1 .statement}

Le diagramme de $k$-modules

$$
\begin{array}{ccc}
\operatorname{Tor}^A(P,M)&\xrightarrow{\psi(S,R)}&H(S\otimes_A R)\\
\downarrow{\sigma_{P,M}}&&\downarrow{H(\sigma(S,R))}\\
\operatorname{Tor}^{A^\circ}(M^\circ,P^\circ)&\xrightarrow{\psi(R^\circ,S^\circ)}&H(R^\circ\otimes_{A^\circ}S^\circ),
\end{array}
$$

où $\sigma_{P,M}$ et $\sigma(S,R)$ sont les *isomorphismes de commutation* (X, p. 71 et 63), est commutatif : il se déduit en effet, par passage à l’homologie, du diagramme commutatif de complexes

$$
\begin{array}{ccc}
L(P)\otimes_A L(M)&\xrightarrow{\beta\otimes\alpha}&S\otimes_A R\\
\downarrow{\sigma(L(P),L(M))}&&\downarrow{\sigma(S,R)}\\
L(M^\circ)\otimes_{A^\circ}L(P^\circ)&\xrightarrow{\alpha\otimes\beta}&R^\circ\otimes_{A^\circ}S^\circ
\end{array}
$$

(« les morphismes $\psi$ sont compatibles avec les isomorphismes de commutation »).

De même, soient $a_1:R_1\to M$, $b_1:S_1\to P$, $c_1:N\to E_1$ des morphismes de complexes, où $R_1$ et $S_1$ sont projectifs et nuls à droite et $E_1$ injectif et nul à gauche. D’après X, p. 49, prop. 3 et 3 bis, il existe des morphismes de complexes

$$
\alpha_1:R_1\to L(M),\qquad \beta_1:S_1\to L(P),\qquad \gamma_1:I(N)\to E_1
$$

tels que $p_M \circ \alpha_1 = a_1, p_P \circ \beta_1 = b_1, \gamma_1 \circ e_N = c_1$, d'où des morphismes de complexes

$$
\beta_1 \otimes \alpha_1 : S_1 \otimes_A R_1 \to L(P) \otimes_A L(M),
$$

$$
\operatorname{Homgr}_A (\alpha_1, \gamma_1) : \operatorname{Homgr}_A (L(M), l(N)) \to \operatorname{Homgr}_A (R_1, E_1),
$$

et par passage à l'homologie des *applications k-linéaires graduées de degré* 0 :

$$
\psi'(S_1, R_1) : H(S_1 \otimes_A R_1) \to \operatorname{Tor}^A (P, M)
$$
$$
\varphi'(R_1, E_1) : \operatorname{Ext}_A (M, N) \to H(\operatorname{Homgr}_A (R_1, E_1))
$$

dont on vérifie comme ci-dessus qu'ils sont indépendants du choix de $\alpha_1, \beta_1, \gamma_1$.

#### Proposition 1 {#alg-x-s6-prop-1 .statement}

*Si* $a_1, b_1, c_1$ *sont des homologismes,* $\psi'(S_1, R_1)$ *et* $\varphi'(R_1, E_1)$ *sont les bijections réciproques des bijections* $\psi(S_1, R_1)$ *et* $\varphi(R_1, E_1)$ *respectivement.*

En effet, $f = (\beta \otimes \alpha) \circ (\beta_1 \otimes \alpha_1)$ est un morphisme du complexe $S_1 \otimes_A R_1$ dans lui-même, et on a $(h_1 \circ \alpha_1) \circ f = f$. D'après X, p. 49, prop. 3 et 3 *bis*, $f$ est un homotopisme, donc $H(f) = 1$ et

$$
\psi(S_1, R_1) \circ \psi'(B_1, R_1) = H(\beta \otimes \alpha) \circ H(\beta_1 \otimes \alpha_1) = H(f) = 1;
$$

de même $\psi'(S_1, R_1) \circ \psi(S_1, R_1) = 1$. On raisonne de manière analogue pour les applications $\varphi$ et $\varphi'$.

#### Exemple 1 {#alg-x-s6-n1-exa-1 .statement}

Soit $a$ un élément de $A$ tel que l'application $\varphi : x \mapsto xa$ de $A$ dans lui-même soit injective (*«* $a$ n'est pas diviseur de zéro à droite *»*). En utilisant la résolution

$$
0 \to A_s \xrightarrow{\varphi} A_s \to A/Aa \to 0
$$

on voit que pour tout $A$-module à droite $M$, on a

$$
\operatorname{Tor}_i^A (M, A/Aa) = 0 \quad \text{pour } i > 1
$$

et que le $k$-module $\operatorname{Tor}_1^A (M, A/Aa)$ est isomorphe à $\operatorname{Ker} (a_M)$.

De même, pour tout $A$-module à gauche $M$, on a

$$
\operatorname{Ext}_A^i (A/Aa, M) = 0 \quad \text{pour } i > 1
$$

et le $k$-module $\operatorname{Ext}_A^1 (A/Aa, M)$ est isomorphe à $M/aM$.

#### Exemple 2 {#alg-x-s6-n1-exa-2 .statement}

Supposons $A$ intègre ; soient $K$ le corps des fractions de $A$ et $M$ un $A$-module. En utilisant la résolution plate

$$
0 \to A \to K \to K/A \to 0
$$

(X, p. 9, *exemple* 5), on voit que $\operatorname{Tor}_i^A (K/A, M) = 0$ pour $i > 1$; de plus, compte tenu de II, p. 116, prop. 26, (ii), le $A$-module $\operatorname{Tor}_1^A (K, A, M)$ est isomorphe au sous-module de torsion de $M$.

#### Exemple 3 {#alg-x-s6-n1-exa-3 .statement}

Supposons que $A$ soit un anneau local noethérien, notons $m$ son idéal maximal, et posons $\kappa = A/m$. Soient $M$ un $A$-module de type fini et $P$ une résolution projective minimale de $M$ (X, p. 54). Pour tout $n \geqslant 0$, les $\kappa$-espaces vectoriels $\mathrm{Tor}_n^A(\kappa, M)$ et $\mathrm{Ext}_A^n(M, \kappa)$ sont de dimension finie, égale au rang du $A$-module libre $P_n$; en effet, les complexes $\kappa \otimes_A P$ et $\mathrm{Homgr}_A(P, \kappa)$ sont à différentielle nulle.

### 2. Calcul des applications $\mathrm{Tor}^A(g, f)$ et $\mathrm{Ext}_A(f, h)$

Soient $f : M \to M', h : N' \to N$ des homomorphismes de $A$-modules à gauche, $g : P \to P'$ un homomorphisme de $A$-modules à droite, $a : R \to M, a' : R' \to M'$, $b : S \to P, b' : S' \to P'$, des résolutions gauches de $M, M', P, P'$, respectivement, $c : N \to E, c' : N' \to E'$ des résolutions droites de $N$ et $N'$, $\tilde{f} : R \to R', \tilde{g} : S \to S', \tilde{h} : E' \to E$ des morphismes de complexes tels que

$$
a' \circ \tilde{f} = f \circ a, \quad b' \circ \tilde{g} = g \circ b, \quad \tilde{h} \circ c' = c \circ h .
$$

#### Proposition 2 {#alg-x-s6-prop-2 .statement}

*Les deux diagrammes suivants sont commutatifs* :

$$
\begin{array}{ccc}
\mathrm{Tor}^A(P, M) & \xrightarrow{\psi(S, R)} & \mathrm{H}(S \otimes_A R) \\
\mathrm{Tor}^A(g, f) \downarrow & & \downarrow \mathrm{H}(\tilde{g} \otimes \tilde{f}) \\
\mathrm{Tor}^A(P', M') & \xrightarrow{\psi(S', R')} & \mathrm{H}(S' \otimes_A R') ,
\end{array}
$$

$$
\begin{array}{ccc}
\mathrm{H}(\mathrm{Homgr}_A(R', E')) & \xrightarrow{\varphi(R', E')} & \mathrm{Ext}_A(M', N') \\
\mathrm{H}(\mathrm{Homgr}_A(\tilde{f}, \tilde{h})) \downarrow & & \downarrow \mathrm{Ext}_A(f, h) \\
\mathrm{H}(\mathrm{Homgr}_A(R, E)) & \xrightarrow{\varphi(R, E)} & \mathrm{Ext}_A(M, N) .
\end{array}
$$

Soient $\alpha : L(M) \to R, \alpha' : L(M') \to R', \gamma : L(P) \to S, \gamma' : L(P') \to S'$ des morphismes de complexes tels que

$$
a \circ \alpha = p_M, \quad a' \circ \alpha' = p_{M'}, \quad b \circ \gamma = p_P, \quad b' \circ \gamma' = p_{P'} .
$$

Par définition, $\mathrm{H}(\tilde{g} \otimes \tilde{f}) \circ \psi(S, R)$ est égal à

$$
\mathrm{H}(\tilde{g} \otimes \tilde{f}) \circ \mathrm{H}(\gamma \otimes \alpha) = \mathrm{H}((\tilde{g} \circ \gamma) \otimes (\tilde{f} \circ \alpha)) ,
$$

tandis que $\psi(S', R') \circ \mathrm{Tor}^A(g, f)$ est égal à

$$
\mathrm{H}(\gamma' \otimes \alpha') \circ \mathrm{H}(L(g) \otimes L(f)) = \mathrm{H}((\gamma' \circ L(g)) \otimes (\alpha' \circ L(f))) .
$$

D'autre part, $\alpha' \circ L(f)$ et $\tilde{f} \circ \alpha$ sont deux morphismes de $L(M)$ dans $R'$ tels que $a' \circ (\alpha' \circ L(f)) = p_{M'} \circ L(f) = f \circ p_M = f \circ a \circ \alpha = a' \circ (\tilde{f} \circ \alpha)$. D'après X, p. 49, prop. 3, $\alpha' \circ L(f)$ et $\tilde{f} \circ \alpha$ sont homotopes ; de même $\gamma' \circ L(g)$ et $\tilde{g} \circ \gamma$ sont homotopes, ainsi par conséquent que $(\gamma' \circ L(g)) \otimes (\alpha' \circ L(f))$ et $(\tilde{g} \circ \gamma) \otimes (\tilde{f} \circ \alpha)$ d’après la prop. 3 de X, p. 64. On a donc

$$
H(\tilde{g} \otimes \tilde{f}) \circ \psi(S, R) = H((\tilde{g} \circ \gamma) \otimes (\tilde{f} \circ \alpha)) = H((\gamma' \circ L(g)) \otimes (\alpha' \circ L(f)))
$$
$$
= \psi(S', R') \circ \mathrm{Tor}^A(g, f) .
$$

On raisonne de manière analogue pour le second diagramme.

#### Remarque {#alg-x-s6-n2-rem-1 .statement}

Considérons de même des diagrammes commutatifs de morphismes de complexes

$$
\begin{array}{ccc}
R_1 & \xrightarrow{a_1} & M \\
\tilde{f} \downarrow & & \downarrow f \\
R'_1 & \xrightarrow{a'_1} & M'
\end{array}
$$
$$
\begin{array}{ccc}
S_1 & \xrightarrow{b_1} & P \\
\tilde{g} \downarrow & & g \downarrow \\
S'_1 & \xrightarrow{b'_1} & P'
\end{array}
$$
$$
\begin{array}{ccc}
N' & \xrightarrow{c'_1} & E' \\
h \downarrow & & \tilde{h} \downarrow \\
N & \xrightarrow{c_1} & E_1
\end{array}
$$

où les complexes $R_1, R'_1, S_1, S'_1$ sont projectifs et nuls à droite et où les complexes $E_1, E'_1$ sont injectifs et nuls à gauche. Alors

$$
\mathrm{Tor}^A(g, f) \circ \psi'(S_1, R_1) = \psi'(S'_1, R'_1) \circ H(\tilde{g} \otimes \tilde{f})
$$
$$
\varphi'(R_1, E_1) \circ \mathrm{Ext}_A(f, h) = H(\mathrm{Homgr}_A(\tilde{f}, \tilde{h})) \circ \varphi'(R'_1, E'_1)
$$

comme on le démontre de manière analogue à la prop. 2.

### 3. Calcul des homomorphismes de liaison

Considérons un diagramme commutatif

(1)
$$
\begin{array}{ccccccccc}
0 & \longrightarrow & R' & \xrightarrow{\tilde{u}} & R & \xrightarrow{\tilde{v}} & R'' & \longrightarrow & 0 \\
& & a' \downarrow & & a \downarrow & & a'' \downarrow & & \\
0 & \longrightarrow & M' & \xrightarrow{u} & M & \xrightarrow{v} & M'' & \longrightarrow & 0
\end{array}
$$

(2)

où la première ligne (1) est une suite exacte de complexes de A-modules à gauche, la seconde ligne (2) est une suite exacte de A-modules à gauche et où les flèches verticales sont des résolutions gauches.

#### Proposition 3 {#alg-x-s6-prop-3 .statement}

a) Soient $P$ un A-module, $b : S \to P$ une résolution gauche de $P$; supposons que la suite de complexes de k-modules

(3)
$$
0 \to S \otimes_A R' \xrightarrow{1_S \otimes \tilde{u}} S \otimes_A R \xrightarrow{1_S \otimes \tilde{v}} S \otimes_A R'' \to 0
$$

soit exacte. Alors le diagramme suivant est commutatif :

$$
\begin{array}{ccc}
\operatorname{Tor}^{A}(P,M'')&\xrightarrow{\partial(P,(2))}&\operatorname{Tor}^{A}(P,M')\\
\Big\downarrow\vcenter{\rlap{$\psi(S,R'')$}}&&\Big\downarrow\vcenter{\rlap{$\psi(S,R')$}}\\
H(S\otimes_A R'')&\xrightarrow{\partial(3)}&H(S\otimes_A R').
\end{array}
$$

b) Soient $N$ un $A$-module à gauche, $c:N\to E$ une résolution droite de $N$; supposons que la suite de complexes de $k$-modules

(4)

$$
0\longrightarrow \operatorname{Homgr}_A(R'',E)
\xrightarrow{\operatorname{Homgr}_A(\tilde{\imath},1)}
\operatorname{Homgr}_A(R,E)
\xrightarrow{\operatorname{Homgr}_A(\tilde{u},1)}
\operatorname{Homgr}'_A(R',E)\longrightarrow 0
$$

soit exacte. Alors le diagramme suivant est commutatif :

$$
\begin{array}{ccc}
H(\operatorname{Homgr}_A(R',E))
&\xrightarrow{\delta((4))}
&H(\operatorname{Homgr}_A(R'',E))
\\
\Big\downarrow\vcenter{\rlap{$\varphi(R',E)$}}
&&
\Big\downarrow\vcenter{\rlap{$\varphi(R'',E)$}}
\\
\operatorname{Ext}_A(M',N)
&\xrightarrow{\partial((2),N)}
&\operatorname{Ext}_A(M'',N).
\end{array}
$$

Démontrons par exemple a). Soit $\beta:L(P)\to S$ un morphisme de complexes tel que
$t\circ\beta=p_P$; considérons le diagramme de $k$-complexes

$$
\begin{array}{ccccccccc}
0&\longrightarrow&S\otimes_A R'&\xrightarrow{1\otimes\tilde{u}}&S\otimes_A R&\xrightarrow{1\otimes\tilde{v}}&S\otimes_A R''&\longrightarrow&0\\
&&\Big\uparrow\vcenter{\rlap{$\beta\otimes1_R$}}&&\Big\uparrow\vcenter{\rlap{$\beta\otimes1_R$}}&&\Big\uparrow\vcenter{\rlap{$\beta\otimes1_{R'}$}}&&\\
0&\longrightarrow&L(P)\otimes_A R'&\xrightarrow{1\otimes\tilde{u}}&L(P)\otimes_A R&\xrightarrow{1\otimes\tilde{v}}&L(P)\otimes_A R''&\longrightarrow&0\\
&&\Big\downarrow\vcenter{\rlap{$1\otimes a'$}}&&\Big\downarrow\vcenter{\rlap{$1\otimes a$}}&&\Big\downarrow\vcenter{\rlap{$1\otimes a''$}}&&\\
0&\longrightarrow&L(P)\otimes_A M'&\xrightarrow{1\otimes u}&L(P)\otimes_A M&\xrightarrow{1\otimes v}&L(P)\otimes_A M''&\longrightarrow&0.
\end{array}
$$

Il est commutatif à lignes exactes (d’après l’hypothèse pour la première ligne, et le fait que $L(P)$ est plat pour les deux autres). On a donc un diagramme commutatif (X, p. 31, prop. 2, et X, p. 72, déf. 2)

$$
\begin{array}{ccc}
H(S\otimes_A R'')&\xrightarrow{\partial(3)}&H(S\otimes_A R')\\
\Big\uparrow\vcenter{\rlap{$H(\beta\otimes1)$}}&&\Big\uparrow\vcenter{\rlap{$H(\beta\otimes1)$}}\\
H(L(P)\otimes_A R'')&\longrightarrow&H(L(P)\otimes_A R')\\
\Big\downarrow\vcenter{\rlap{$H(1\otimes a'')$}}&&\Big\downarrow\vcenter{\rlap{$H(1\otimes a')$}}\\
H(L(P)\otimes_A M'')&\longrightarrow&H(L(P)\otimes_A M')\\
\Big\uparrow\vcenter{\rlap{$\psi_P(M'')$}}&&\Big\uparrow\vcenter{\rlap{$\psi_P(M')$}}\\
\operatorname{Tor}(P,M'')&\xrightarrow{\partial(P,(2))}&\operatorname{Tor}(P,M').
\end{array}
$$

D’après X, p. 67, prop. 4, H(1 ⊗ a'') et H(1 ⊗ a') sont bijectifs ; d’autre part, par définition des homomorphismes ψ, on a H(β ⊗ 1) ◦ ψ(L(P), R'') = ψ(S, R'') et H(1 ⊗ a'') ◦ ψ(L(P), R'') = ψ(L(P), M'') = ψ_p(M''), donc

$$
ψ(S, R'') = H(β ⊗ 1) ◦ H(1 ⊗ a'')^{-1} ◦ ψ_p(M'');
$$

de même, $ψ(S, R') = H(β ⊗ 1) ◦ H(1 ⊗ a')^{-1} ◦ ψ_p(M')$, et l’assertion cherchée $\partial((3)) ◦ ψ(S, R'') = ψ(S, R') ◦ \partial(P, (2))$ résulte de la commutativité du diagramme précédent.

#### Remarque 1 {#alg-x-s6-n3-rem-1 .statement}

Utilisant les isomorphismes de commutation, on déduit de a) l’énoncé analogue obtenu en échangeant les rôles des deux arguments du produit tensoriel.

#### Remarque 2 {#alg-x-s6-n3-rem-2 .statement}

Avec les notations de a), supposons soit S plat, soit R, R', R'' plats ; alors d’une part la suite (3) est exacte (X, p. 72, cor. 2) et on peut appliquer la prop. 3 ; d’autre part $ψ(S, R')$ est bijectif (th. 1), donc

$$
\partial(P, (2)) = ψ(S, R')^{-1} ◦ \partial((3)) ◦ ψ(S, R'').
$$

#### Remarque 3 {#alg-x-s6-n3-rem-3 .statement}

Avec les notations de b), supposons soit E injectif, soit R, R', R'' projectifs ; alors d’une part la suite (4) est exacte (X, p. 83, prop. 2) et on peut appliquer la prop. 3 ; d’autre part, $φ(R', E)$ est bijectif (th. 1) ; donc

$$
δ((2), N) = φ(R'', E) ◦ \partial((4)) ◦ φ(R', E)^{-1}.
$$

Considérons maintenant un diagramme commutatif

(5)
$$
\begin{array}{ccccccccc}
0 & \rightarrow & N' & \xrightarrow{r} & N & \xrightarrow{s} & N'' & \rightarrow & 0 \\
   &           & c'   &         &   &         & c''   &         &
\end{array}
$$

(6)
$$
\begin{array}{ccccccccc}
0 & \rightarrow & E' & \xrightarrow{\tilde{r}} & E & \xrightarrow{\tilde{s}} & E'' & \rightarrow & 0
\end{array}
$$

dont la première ligne (5) est une suite exacte de A-modules à gauche, la seconde ligne (6) une suite exacte de complexes de A-modules à gauche et où les flèches verticales sont des résolutions droites. En raisonnant comme dans la prop. 3, on démontre la proposition suivante :

#### Proposition 4 {#alg-x-s6-prop-4 .statement}

Soient M un A-module à gauche, a : R → M une résolution gauche de M telle que la suite

(7)
$$
0 \rightarrow \mathrm{Homgr}_A(R, E') \xrightarrow{\mathrm{Homgr}(\tilde{s}, 1)} \mathrm{Homgr}_A(R, E) \xrightarrow{\mathrm{Homgr}(\tilde{r}, 1)} \mathrm{Homgr}_A(R, E'') \rightarrow 0
$$

soit exacte. Alors le diagramme suivant est commutatif.

$$
\begin{array}{ccc}
\mathrm{H}(\mathrm{Homgr}_A(R, E'')) & \xrightarrow{\partial((7))} & \mathrm{H}(\mathrm{Homgr}_A(R, E')) \\
\varphi(R, E'') \downarrow & & \downarrow \varphi(R, E') \\
\mathrm{Ext}_A(M, N'') & \xrightarrow{\delta(M, (5))} & \mathrm{Ext}_A(M, N')
\end{array}
$$

#### Remarque 4 {#alg-x-s6-n3-rem-4 .statement}

Si R est projectif ou si E, E', E'' sont injectifs, la suite (7) est exacte ($\lambda$, p. 83, prop. 2); de plus, $\varphi(R, E'')$ est bijectif (th. 1); donc

$$
\delta(M, (5)) = \varphi(R, E') \circ \partial((7)) \circ \varphi(R, E'')^{-1}.
$$

#### Remarque 5 {#alg-x-s6-n3-rem-5 .statement}

Nous laissons au lecteur le soin d’énoncer et de démontrer les propositions analogues aux prop. 3 et 4 et relatives aux homomorphismes $\psi_1$ et $\varphi_1$.

### 4. Finitude des modules d’extensions et de torsion

Soient M un A-module à gauche, I un ensemble préordonné filtrant, $(N_i, u_{ji})$ un système inductif de A-modules à gauche relatifs à I, $N = \lim N_i$ sa limite inductive, $u_i : N_i \to N,\ i \in I$, l’application canonique. Alors $(\mathrm{Ext}_A(M, N_i), \mathrm{Ext}_A(l_M, u_{ji}))$ est un système inductif de $k$-modules et $(\mathrm{Ext}_A(l_M, u_i))$ un système inductif d’applications, dont la limite inductive est un homomorphisme de $k$-modules gradués, dit *canonique*

$$
\lim_{i \in I} \mathrm{Ext}_A(M, N_i) \to \mathrm{Ext}_A(M, \lim_{i \in I} N_i).
$$

#### Proposition 5 {#alg-x-s6-prop-5 .statement}

*Si A est nœthérien à gauche et si M est un A-module de type fini, l’homomorphisme canonique (8) est bijectif.*

Soit en effet (X, p. 53, prop. 6) $p : L \to M$ une résolution libre de M telle que $L_n$ soit de type fini pour chaque $n$. Le morphisme canonique de $k$-complexes

$$
u : \lim \mathrm{Homgr}_A(L, N_i) \to \mathrm{Homgr}_A(L, \lim N_i)
$$

est bijectif, donc aussi l’homomorphisme

$$
\lim \mathrm{H}(\mathrm{Homgr}_A(L, N_i)) \to \mathrm{H}(\mathrm{Homgr}_A(L, \lim N_i))
$$

déduit des homomorphismes $\mathrm{H}(\mathrm{Homgr}(l, u_i))$ (X, p. 28, prop. 1). On conclut alors par la prop. 2 (X, p. 103) et le th. 1 (X, p. 100).

#### Proposition 6 {#alg-x-s6-prop-6 .statement}

*Soient B un anneau et N un (A, B)-bimodule, qui est un B-module nœthérien (resp. de longueur finie).

a) Supposons A nœthérien à droite et soit M un A-module à droite de type fini. Alors les B-modules (X, p. 81) $\mathrm{Tor}_n^A(M, N)$ sont nœthériens (resp. de longueur finie).

b) Supposons A nœthérien à gauche et soit M un A-module à gauche de type fini. Alors les B-modules (X, p. 98) $\mathrm{Ext}_A^n(M, N)$ sont nœthériens (resp. de longueur finie).

Choisissons une résolution libre $p : L \to M$ telle que chacun des A-modules $L_n$ soit de type fini (X, p. 53, prop. 6), et soit C le complexe de B-modules $L \otimes_A N$ dans le cas $a$, $\mathrm{Homgr}_A(L, N)$ dans le cas $b$. Chacun des B-modules $C_n$ est isomorphe à un produit d’un nombre fini d’exemplaires de N, donc est nœthérien (resp. de longueur finie); il en est donc de même des modules $\mathrm{H}_n(C)$. Or, d’après X, p. 100, th. 1, ceux-ci sont isomorphes aux $\mathrm{Tor}_n^A(M, N)$ dans le cas $a$, aux $\mathrm{Ext}_A^{-n}(M, N)$ dans le cas $b$.

#### Corollaire {#alg-x-s6-n4-cor-1 .statement}

Soient $\rho : A \to B$ un homomorphisme d’anneaux commutatifs noethériens, $M$ un $A$-module de type fini, $N$ un $B$-module. Si $N$ est un $B$-module de type fini (resp. de longueur finie), il en est de même des $B$-modules $\operatorname{Tor}^{A}_{n}(M,N)$ et $\operatorname{Ext}^{n}_{A}(M,N)$.

### 5. Les homomorphismes $\operatorname{Tor}^{B}(P,N) \otimes_{A} Q \to \operatorname{Tor}^{B}(P,N \otimes_{A} Q)$ et $\operatorname{Ext}_{B}(M,N) \otimes_{A} Q \to \operatorname{Ext}_{B}(M,N \otimes_{A} Q)$

Soient $B$ un anneau, $N$ un $(B,A)$-bimodule, $M$ un $B$-module à gauche, $P$ un
$B$-module à droite, $Q$ un $A$-module à gauche.
D’après X, p. 62, on dispose d’un homomorphisme

$$
\gamma_{1} : H(L(P) \otimes_{B} N) \otimes_{A} Q \to H(L(P) \otimes_{B} N \otimes_{A} Q) \,;
$$

par ailleurs (X, p. 69, prop. 5), on a des isomorphismes

$$
\psi_{1}(N) : \operatorname{Tor}^{B}(P,N) \otimes_{A} Q \to H(L(P) \otimes_{B} N) \otimes_{A} Q \,,
$$

$$
\psi_{1}(N \otimes_{A} Q) : \operatorname{Tor}^{B}(P,N \otimes_{A} Q) \to H(L(P) \otimes_{B} N \otimes_{A} Q) \,.
$$

L’homomorphisme gradué de degré 0, dit *canonique*

(9)

$$
\operatorname{Tor}^{B}(P,N) \otimes_{A} Q \to \operatorname{Tor}^{B}(P,N \otimes_{A} Q)
$$

est défini comme le composé $\psi_{P}(N \otimes_{A} Q)^{-1} \circ \gamma_{1} \circ (\psi_{P}(N) \otimes 1_{Q})$.

De même, on déduit du morphisme canonique de complexes

$$
\alpha : \operatorname{Homgr}_{B}(L(M),N) \otimes_{A} Q \to \operatorname{Homgr}_{B}(L(M),N \otimes_{A} Q)
$$

un homomorphisme $H(\alpha)$; on dispose de l’homomorphisme canonique (X, p. 62)

$$
\gamma_{2} : H(\operatorname{Homgr}_{B}(L(M),N)) \otimes_{A} Q \to H(\operatorname{Homgr}_{B}(L(M),N \otimes_{A} Q)) \,,
$$

et des isomorphismes (X, p. 88, prop. 5)

$$
\varphi_{M}(N) : H(\operatorname{Homgr}_{B}(L(M),N)) \otimes_{A} Q \to \operatorname{Ext}_{B}(M,N) \otimes_{A} Q \,,
$$

$$
\varphi_{M}(N \otimes_{A} Q) : H(\operatorname{Homgr}_{B}(L(M),N \otimes_{A} Q)) \to \operatorname{Ext}_{B}(M,N \otimes_{A} Q) \,.
$$

L’homomorphisme gradué de degré 0, dit *canonique*

(10)

$$
\operatorname{Ext}_{B}(M,N) \otimes_{A} Q \to \operatorname{Ext}_{B}(M,N \otimes_{A} Q)
$$

est défini comme le composé

$$
\varphi_{M}(N \otimes_{A} Q) \circ H(\alpha) \circ (\varphi_{M}(N) \otimes 1_{Q})^{-1} \,.
$$

#### Proposition 7 {#alg-x-s6-prop-7 .statement}

a) Si le $A$-module $Q$ est plat, l’homomorphisme (9) est bijectif.
b) Si le $A$-module $Q$ est projectif de type fini, l’homomorphisme (10) est bijectif.

c) Si le $A$-module $Q$ est plat, l’anneau $B$ noethérien et le $B$-module $M$ de type fini, l’homomorphisme (10) est bijectif.

a) Si $Q$ est plat, $\gamma_1$ est bijectif ($X$, p. 66, cor. 2).

b) Si $Q$ est projectif de type fini, il est plat, donc $\gamma_2$ est bijectif, et de plus $\alpha$ est bijectif (II, p. 75, prop. 2, a)).

c) Sous les hypothèses de c), $\gamma_2$ est bijectif puisque $Q$ est plat. Par ailleurs ($X$, p. 53, prop. 6), il existe une résolution $L$ de $M$ telle que chaque $L_n$ soit libre de type fini ; soit $u : L(M) \to L$ un homotopisme ($X$, p. 49, cor. à la prop. 3) ; dans le diagramme commutatif,

$$
\begin{array}{ccc}
\mathrm{Homgr}_B(L(M), N) \otimes_A Q & \xrightarrow{\alpha} & \mathrm{Homgr}_B(L(M), N \otimes_A Q) \\
\uparrow & & \uparrow \\
\mathrm{Homgr}_B(L, N) \otimes_A Q & \xrightarrow{\bar{\alpha}} & \mathrm{Homgr}_B(L, N \otimes_A Q).
\end{array}
$$

les flèches verticales déduites de $u$ sont des homotopismes ($X$, p. 64, prop. 3 et p. 83, prop. 3) et $\bar{\alpha}$ est bijectif (II, p. 75, prop. 2 (ii)) ; donc $H(\alpha)$ est bijectif, et l’homomorphisme (10) est bijectif.

### 6. Les homomorphismes $\mathrm{Tor}^B(P, N \otimes_A Q) \to \mathrm{Tor}^A(P \otimes_B N, Q)$ et $\mathrm{Ext}_A(Q, \mathrm{Hom}_B(N, M)) \to \mathrm{Ext}_B(N \otimes_A Q, M)$

Gardons les notations précédentes, et supposons $N$ plat sur $A$. Alors le morphisme $N \otimes_A L(Q) \xrightarrow{1 \otimes p_Q} N \otimes_A Q$ est un homologisme ($X$, p. 67, prop. 4), d’où des homomorphismes

$$
\psi(P, N \otimes_A L(Q)) : \mathrm{Tor}^B(P, N \otimes_A Q) \to H(P \otimes_B N \otimes_A L(Q))
$$
$$
\varphi(N \otimes_A L(Q), M) : H(\mathrm{Homgr}_B(N \otimes_A L(Q), M)) \to \mathrm{Ext}_B(N \otimes_A Q, M).
$$

Utilisant alors les *isomorphismes*

$$
\overline{\psi}_Q(P \otimes_B N) : \mathrm{Tor}^A(P \otimes_B N, Q) \to H(P \otimes_B N \otimes_A L(Q)),
$$
$$
\beta : \mathrm{Homgr}_A(L(Q), \mathrm{Hom}_B(N, M)) \to \mathrm{Homgr}_B(N \otimes_A L(Q), M),
$$
$$
\varphi_Q(\mathrm{Hom}_B(N, M)) : H(\mathrm{Homgr}_A(L(Q), \mathrm{Hom}_B(N, M))) \to \mathrm{Ext}_A(Q, \mathrm{Hom}_B(N, M)),
$$

on en déduit des homomorphismes gradués de degré 0 dits *canoniques* :

(11) $$ \mathrm{Tor}^B(P, N \otimes_A Q) \to \mathrm{Tor}^A(P \otimes_B N, Q) $$
(12) $$ \mathrm{Ext}_A(Q, \mathrm{Hom}_B(N, M)) \to \mathrm{Ext}_B(N \otimes_A Q, M). $$

#### Proposition 8 {#alg-x-s6-prop-8 .statement}

*a)* Si $N$ est plat sur $A$ et sur $B$, l’homomorphisme (11) est bijectif.

*b)* Si $N$ est plat sur $A$ et projectif sur $B$, l’homomorphisme (12) est bijectif.

En effet $N \otimes_A L(Q)$ est isomorphe à une somme directe d'exemplaires de $N$, donc est un $B$-module plat (resp. projectif) lorsque le $B$-module $N$ est plat (resp. projectif); on applique alors le th. 1 (X, p. 100).

### 7. Les homomorphismes $B \otimes_A \mathrm{Tor}^A(E, F) \to \mathrm{Tor}^B(E \otimes_A B, B \otimes_A F)$ et $B \otimes_A \mathrm{Ext}_A(E, F) \to \mathrm{Ext}_B(B \otimes_A E, B \otimes_A F)$

Dans ce numéro, on suppose que $A$ est *commutatif*; on se donne un homomorphisme d'anneaux $\rho : A \to B$ tel que $\rho(A)$ soit contenu dans le centre de $B$ et deux $A$-modules $E$ et $F$. On a un isomorphisme canonique de complexes de $A$-modules

$$
u : B \otimes_A (L(E) \otimes_A L(F)) \to (L(E) \otimes_A B) \otimes_B (B \otimes_A L(F));
$$

d'autre part, puisque $L(E) \otimes_A B$ et $B \otimes_A L(F)$ sont des $B$-complexes *libres*, on a un homomorphisme canonique de $A$-modules gradués (X, p. 102)

$$
\psi'(L(E) \otimes_A B, B \otimes_A L(F)) : H((L(E) \otimes_A B) \otimes_B (B \otimes_A L(F)))
$$
$$
\to \mathrm{Tor}^B(E \otimes_A B, B \otimes_A F)
$$

enfin, on dispose d'un homomorphisme (X, p. 62)

$$
\gamma : B \otimes_A \mathrm{Tor}^A(E, F) \to H(B \otimes_A L(E) \otimes_A L(F)).
$$

L'homomorphisme *canonique* de $B$-modules gradués

(13)
$$
B \otimes_A \mathrm{Tor}^A(E, F) \to \mathrm{Tor}^B(E \otimes_A B, B \otimes_A F)
$$

est défini comme le composé $\psi'(L(E) \otimes_A B, B \otimes_A L(F)) \circ H(u) \circ \gamma$.

#### Proposition 9 {#alg-x-s6-prop-9 .statement}

*Si $B$ est plat sur $A$, l'homomorphisme (13) est bijectif.*
En effet $\psi'(L(E) \otimes_A B, B \otimes_A L(F))$ est bijectif (X, p. 102, prop. 1) et $\gamma$ est bijectif (X, p. 66, cor. 2).

Supposons $B$ *plat* sur $A$. Substituant dans l'homomorphisme (12) $E$ à $Q$, $B$ à $N$ et $B \otimes_A F$ à $M$, on obtient un homomorphisme

$$
\mathrm{Ext}_A(E, B \otimes_A F) \to \mathrm{Ext}_B(B \otimes_A E, B \otimes_A F)
$$

qui est bijectif d'après la prop. 8. Substituant dans l'homomorphisme (10) $E$ à $M$, $F$ à $N$, $A$ à $B$, $B$ à $Q$, et échangeant les facteurs des produits tensoriels, on obtient un homomorphisme de $B$-modules

$$
B \otimes_A \mathrm{Ext}_A(E, F) \to \mathrm{Ext}_A(E, B \otimes_A F),
$$

d'où par composition un homomorphisme dit *canonique*

(14)
$$
B \otimes_A \mathrm{Ext}_A(E, F) \to \mathrm{Ext}_B(B \otimes_A E, B \otimes_A F).
$$

#### Proposition 10 {#alg-x-s6-prop-10 .statement}

L’homomorphisme (14) est bijectif dans les cas suivants :
a) B est un A-module projectif de type fini ;
b) B est un A-module plat, A est noethérien, et E est un A-module de type fini.
Cela résulte de la prop. 7 (X, p. 108).

### 8. Application : homologie et cohomologie des groupes

Soient G un groupe, $\mathbf{Z}^{(G)}$ son algèbre sur $\mathbf{Z}$ (III, p. 19). Rappelons (cf. III, p. 20, exemple) que si M est un groupe commutatif, il revient au même de se donner une action de G sur M (c’est-à-dire un homomorphisme $\tau : G \to \mathrm{Aut}(M)$), ou une structure de $\mathbf{Z}^{(G)}$-module à gauche sur le groupe additif M. En particulier, on considérera le groupe $\mathbf{Z}$ comme un $\mathbf{Z}^{(G)}$-module à gauche en le munissant de l’action triviale.

#### Définition 1 {#alg-x-s6-def-1 .statement}

Soient M un $\mathbf{Z}^{(G)}$-module à gauche (resp. à droite), n un entier $\geqslant 0$. Le groupe $\mathrm{Ext}_{\mathbf{Z}^{(G)}}^n(\mathbf{Z}, M)$ (resp. $\mathrm{Tor}_n^{\mathbf{Z}^{(G)}}(M, \mathbf{Z})$) est noté $H^n(G, M)$ (resp. $H_n(G, M)$) et appelé n-ième groupe de cohomologie (resp. d’homologie) de G à coefficients dans M.

La résolution standard (X, p. 58) $B(\mathbf{Z}^{(G)}, \mathbf{Z})$ est une résolution libre du $\mathbf{Z}^{(G)}$-module $\mathbf{Z}$; il en résulte que les groupes $H^n(G, M)$ (resp. $H_n(G, M)$) s’identifient aux groupes d’homologie du complexe :

$$
\mathrm{Hom}_{\mathbf{Z}^{(G)}}(B(\mathbf{Z}^{(G)}, \mathbf{Z}), M) \quad (\text{resp. } M \otimes_{\mathbf{Z}^{(G)}} B(\mathbf{Z}^{(G)}, \mathbf{Z})) .
$$

En utilisant l’isomorphisme canonique de $(\mathbf{Z}^{(G)})^{\otimes n}$ sur $\mathbf{Z}^{(G^n)}$ (III, p. 36) et les propriétés de l’extension des scalaires (II, p. 82) on conclut que $H^n(G, M)$ est canoniquement isomorphe au groupe d’homologie de degré ascendant $n$ du complexe $C(G, M)$ défini de la façon suivante : $C^n(G, M) = 0$ pour $n < 0$; pour $n \geqslant 0$, $C^n(G, M)$ est le $\mathbf{Z}$-module des applications de $G^n$ dans M; pour $n \geqslant 0$, la différentielle $d^n : C^n(G, M) \to C^{n+1}(G, M)$ est donnée par

$$
(d^n f)(g_0, ..., g_n) = g_0 \cdot f(g_1, ..., g_n) + \sum_{i=0}^{n-1} (-1)^{i+1} f(g_0, ..., g_i g_{i+1}, ..., g_n)
$$
$$
+ (-1)^{n+1} f(g_0, ..., g_{n-1})
$$

quels que soient $f$ dans $C^n(G, M)$ et $g_0, ..., g_n$ dans G.

De même, $H_n(G, M)$ s’identifie au groupe d’homologie de degré $n$ du complexe $C'(G, M)$, où $C'_n(G, M) = M \otimes_{\mathbf{Z}} \mathbf{Z}^{(G^n)}$ pour $n \geqslant 0$, $C'_n(G, M) = 0$ pour $n < 0$, la différentielle $d_n : C'_n(G, M) \to C'_{n-1}(G, M)$ étant définie par :

$$
d_n(m \otimes e_{g_1, ..., g_n}) = m \cdot g_1 \otimes e_{g_2, ..., g_n} + \sum_{i=1}^{n-1} (-1)^i m \otimes e_{g_1, ..., g_i g_{i+1}, ..., g_n}
$$
$$
+ (-1)^n m \otimes e_{g_1, ..., g_{n-1}}
$$

quels que soient $n \geqslant 1$, $m$ dans M et $g_1, ..., g_n$ dans G.

#### Exemple 1 {#alg-x-s6-n8-exa-1 .statement}

Il résulte directement de la définition que $H^0(G, M)$ est isomorphe au sous-module des éléments de $M$ invariants sous l’action de $G$, et $H_0(G, M)$ au module quotient de $M$ par le sous-module engendré par les éléments $m.g-m$ pour $m\in M$, $g\in G$.

#### Exemple 2 {#alg-x-s6-n8-exa-2 .statement}

Il résulte de ce qui précède que $H^1(G, M)$ est isomorphe au $\mathbf{Z}$-module $Z^1(G, M)/B^1(G, M)$, où $Z^1(G, M)$ est le $\mathbf{Z}$-module des applications $f$ de $G$ dans $M$ vérifiant :

$$
f(g_1,g_2)=g_1.f(g_2)+f(g_1)\quad\text{pour tous }g_1,g_2\text{ dans }G,
$$

et $B^1(G, M)$ est le sous $\mathbf{Z}$-module de $Z^1(G, M)$ formé des $f$ pour lesquelles il existe un élément $m$ de $M$ tel que :

$$
f(g)=g.m-m\quad\text{pour tout }g\in G.
$$

On dit parfois que $Z^1(G, M)$ est le $\mathbf{Z}$-module des homomorphismes croisés de $G$ dans $M$, et $B^1(G, M)$ le sous-module des homomorphismes croisés principaux.

Notons $\iota:G\to \operatorname{Aut}(M)$ l’homomorphisme déduit de l’action de $G$ ; considérons le produit semi-direct externe $M\times_{\iota}G$ et l’extension $\xi_{\iota}:M\times_{\iota}G\to G$ (I, p. 64). Soit $e:G\to M\times_{\iota}G$ une application telle que $\rho\circ e=1_G$ ; on a $e=(f,1_G)$, où $f\in C^1(G,M)$. Pour que $e$ soit un homomorphisme (c’est-à-dire une section de l’extension $\xi_{\iota}$) il faut et il suffit que $f\in Z^1(G,M)$. Pour que deux sections de $\xi_{\iota}$ soient conjuguées par un élément de $i(M)$, il faut et il suffit que les homomorphismes croisés correspondants aient même classe dans $H^1(G,M)$.

Lorsque $G$ opère trivialement sur $M$, on a $B^1(G,M)=0$ et $H^1(G,M)$ est isomorphe au $\mathbf{Z}$-module des homomorphismes de groupes de $G$ dans $M$.

#### Exemple 3 {#alg-x-s6-n8-exa-3 .statement}

De même $H^2(G,M)$ est isomorphe au $\mathbf{Z}$-module $Z^2(G,M)/B^2(G,M)$, où $Z^2(G,M)$ est le $\mathbf{Z}$-module des applications $f$ de $G\times G$ dans $M$, vérifiant :

$$
g_1.f(g_2,g_3)-f(g_1g_2,g_3)+f(g_1,g_2g_3)-f(g_1,g_2)=0
$$

quels que soient $g_1,g_2,g_3$ dans $G$, et $B^2(G,M)$ est le sous-$\mathbf{Z}$-module de $Z^2(G,M)$ formé des $f$ pour lesquelles il existe une application $h$ de $G$ dans $M$ telle que :

$$
f(g_1,g_2)=g_1.h(g_2)-h(g_1g_2)+h(g_1)
$$

quels que soient $g_1,g_2$ dans $G$.

On retrouve ainsi la définition du groupe $H^2(G,M)$ donnée en VIII, App. II en particulier qu’il existe un isomorphisme canonique de $H^2(G,M)$ sur le groupe des classes d’extension de $G$ par $M$ (loc. cit.).

#### Exemple 4 {#alg-x-s6-n8-exa-4 .statement}

Soit $M$ un $\mathbf{Z}$-module, que l’on considère comme un $\mathbf{Z}^{(G)}$-module à droite en faisant opérer $G$ trivialement. Le groupe $H_1(G,M)$ est isomorphe au quotient de $M\otimes_{\mathbf{Z}}\mathbf{Z}^{(G)}$ par le sous-$\mathbf{Z}$-module engendré par les éléments $m\otimes(e_{g_1g_2}-e_{g_1}-e_{g_2})$ pour $m$ dans $M$, $g_1,g_2$ dans $G$ ; il en résulte facilement que $H_1(G,M)$ est isomorphe à $M\otimes_{\mathbf{Z}}(G/(G,G))$.

Notons $\sigma$ l’anti-automorphisme de $\mathbf{Z}^{(G)}$ défini par $\sigma(e_g) = e_{g^{-1}}$ pour $g \in G$. Tout $\mathbf{Z}^{(G)}$-module à gauche peut être considéré comme un $\mathbf{Z}^{(G)}$-module à droite à l’aide de $\sigma$, et réciproquement. Ceci permet par exemple de définir les groupes $H_q(G, M)$ pour un $\mathbf{Z}^{(G)}$-module à gauche $M$, en posant $H_q(G, M) = H_q(G, \sigma_*(M)) = \mathrm{Tor}_q^{\mathbf{Z}^{(G)}}(\mathbf{Z}, M)$.

#### Lemme 1 {#alg-x-s6-lem-1 .statement}

*Soit $M$ un $\mathbf{Z}$-module ; notons $M^G$ le groupe $\mathrm{Hom}_{\mathbf{Z}}(\mathbf{Z}^{(G)}, M)$ muni de sa structure naturelle de $\mathbf{Z}^{(G)}$-module à gauche. Alors :*

$$
H^i(G, M^G) = 0 \quad \text{pour} \quad i \geqslant 1 .
$$

Il résulte en effet de la prop. 8, b) (X, p. 109), appliquée avec $A = N = \mathbf{Z}^{(G)}$ et $B = Q = \mathbf{Z}$, que l’on a un isomorphisme canonique :

$$
\mathrm{Ext}_{\mathbf{Z}^{(G)}}(\mathbf{Z}, M^G) \to \mathrm{Ext}_{\mathbf{Z}}(\mathbf{Z}, M)
$$

d’où le lemme.

#### Proposition 11 {#alg-x-s6-prop-11 .statement}

*Soit $L$ une extension galoisienne de degré fini d’un corps commutatif $K$, de groupe de Galois $G$.
a) *On a* $H^i(G, L) = 0$ *pour* $i \geqslant 1$.
b) *On a* $H^1(G, L^*) = 0$.
c) *Le groupe* $H^2(G, L^*)$ *est canoniquement isomorphe au groupe* $\mathrm{Br}(K, L)$ *(VIII, § 13)*.

Le théorème de la base normale (V, §10, n° 9, th. 6) montre que $L$ est isomorphe comme $\mathbf{Z}^{(G)}$-module à $K^G = \mathrm{Hom}_{\mathbf{Z}}(\mathbf{Z}^{(G)}, K)$; l’assertion a) résulte alors du lemme 1. Compte tenu de l’exemple 2, l’assertion b) résulte de V, §10, n° 5, cor. 1 à la prop. 9 : enfin l’assertion c) a été démontrée en VIII, §13.

## EXERCICES {#alg-x-s6-exercises}

See the [exercises for § 6](exercises/s6/).
