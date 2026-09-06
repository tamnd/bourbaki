---
book: alg
book_title: Algebra
chapter: X
chapter_title: ALGÈBRE HOMOLOGIQUE
section: 8
section_title: Dimension homologique
lang: fr
source: alg-x-fr
book_pages: A X.134-A X.146, A X.202-A X.206
pdf_pages: 0140-0152, 0208-0212
extraction: ocr
subsections:
    - "no": 1
      title: Dimension projective d’un module
      page: 134
      pdf_page: 140
    - "no": 2
      title: L’homomorphisme $\operatorname{Tor}_n^A(P, M) \to \operatorname{Hom}_A(\operatorname{Ext}_A^n(M, A), P)$
      page: 137
      pdf_page: 143
    - "no": 3
      title: Dimension homologique d’un anneau
      page: 138
      pdf_page: 144
    - "no": 4
      title: Anneaux de dimension homologique 0
      page: 140
      pdf_page: 146
    - "no": 5
      title: Anneaux de dimension homologique 1
      page: 140
      pdf_page: 146
    - "no": 6
      title: Dimension homologique des anneaux de polynômes
      page: 141
      pdf_page: 147
    - "no": 7
      title: Dimension homologique des modules gradués
      page: 143
      pdf_page: 149
statements: 34
exercises: 28
content_sha256: 01423d7f9d05c6000bce1884bf08ce49ac1e4be4045d9ae6bb8edef4dbad7463
---

## § 8. DIMENSION HOMOLOGIQUE

Dans ce paragraphe, on reprend les conventions du § 5.

### 1. Dimension projective d’un module

#### Définition 1 {#alg-x-s8-def-1 .statement}

*Soit $M$ un $A$-module. On appelle dimension projective de $M$, et on note $\mathrm{dp}_A(M)$ la borne inférieure dans $\overline{\mathbf{Z}}$ des longueurs des résolutions projectives de $M$* (X, p. 48).

On a donc $\mathrm{dp}_A(0) = -\infty$, $\mathrm{dp}_A(M) \geq 0$ si $M \neq 0$. Pour que $M$ soit projectif, il faut et il suffit que $\mathrm{dp}_A(M) \leq 0$.

#### Lemme 1 {#alg-x-s8-lem-1 .statement}

*Si $\mathrm{dp}_A(M) < n < +\infty$, on a $\mathrm{Ext}_A^n(M, N) = 0$ pour tout $A$-module $N$ et $\mathrm{Tor}_n^A(P, M) = 0$ pour tout $A$-module à droite $P$.
Cela résulte aussitôt du fait que $M$ possède une résolution projective de longueur $< n$ et de X, p. 100, th. 1.

#### Proposition 1 {#alg-x-s8-prop-1 .statement}

*Soient $M$ un $A$-module et $n$ un entier $\geq 0$. Les conditions suivantes sont équivalentes* :
(i) $\mathrm{dp}_A(M) \leq n$ (*i.e.* (déf. 1), $M$ possède une résolution projective de longueur $\leq n$);
(ii) $\mathrm{Ext}_A^r(M, N) = 0$ pour tout $A$-module $N$ et tout entier $r > n$;
(iii) $\mathrm{Ext}_A^{n+1}(M, N) = 0$ pour tout $A$-module $N$;
(iv) *pour toute suite exacte*
$$
0 \to K \to P_{n-1} \to \ldots \to P_0 \to M \to 0
$$
*où les $P_i$ sont projectifs, $K$ est projectif*.

(i) ⇒ (ii) : cela résulte du lemme 1.
(ii) ⇒ (iii) : c'est trivial.
(iii) ⇒ (iv) : dans la situation de (iv), on a pour tout A-module N un isomorphisme de $\mathrm{Ext}_A^1(K, N)$ sur $\mathrm{Ext}_A^{n+1}(M, N)$ (X, p. 128, cor. 4) ; si (iii) est satisfait, on a
$$
\mathrm{Ext}_A^1(K, N) = 0
$$
pour tout N et K est projectif (X, p. 93, prop. 10).
(iv) ⇒ (i) : considérons la suite exacte (X, p. 50)
$$
0 \to Z_{n-1}(M) \to L_{n-1}(M) \to \ldots \to L_0(M) \to M \to 0 .
$$
Si (iv) est satisfait, $Z_{n-1}(M)$ est projectif et M possède une résolution projective de longueur $\leq n$.

#### Corollaire 1 {#alg-x-s8-prop-1-cor-1 .statement}

Soit $(M_i)_{i \in E}$ une famille de A-modules. On a
$$
\mathrm{dp}_A \left( \bigoplus_{i \in E} M_i \right) = \sup_{i \in E} \mathrm{dp}_A(M_i) .
$$
Cela résulte de l'équivalence des conditions (i) et (iii) de la prop. 1. et de la prop. 7 de X, p. 89.

Dans l'énoncé suivant, on convient que $\pm \infty + 1 = \pm \infty - 1 = \pm \infty$.

#### Corollaire 2 {#alg-x-s8-prop-1-cor-2 .statement}

Soit
$$
0 \to M' \to M \to M'' \to 0
$$
une suite exacte de A-modules.

a) On a
$$
\mathrm{dp}_A(M) \leq \sup (\mathrm{dp}_A(M'), \mathrm{dp}_A(M'')) .
$$
L'égalité a lieu dès que $\mathrm{dp}_A(M'') \neq \mathrm{dp}_A(M') + 1$.

b) On a
$$
\mathrm{dp}_A(M'') \leq \sup (\mathrm{dp}_A(M), \mathrm{dp}_A(M') + 1) .
$$
L'égalité a lieu dès que $\mathrm{dp}_A(M) \neq \mathrm{dp}_A(M')$.

c) On a
$$
\mathrm{dp}_A(M') \leq \sup (\mathrm{dp}_A(M), \mathrm{dp}_A(M'') - 1) .
$$
L'égalité a lieu dès que $\mathrm{dp}_A(M) \neq \mathrm{dp}_A(M'')$.

Démontrons par exemple a), les démonstrations de b) et c) étant analogues.
Si N est un A-module quelconque et n un entier $\geq 0$, on a une suite exacte
$$
\mathrm{Ext}_A^{n+1}(M'', N) \to \mathrm{Ext}_A^{n+1}(M, N) \to \mathrm{Ext}_A^{n+1}(M', N) \to \mathrm{Ext}_A^{n+2}(M'', N)
$$
$$
\to \mathrm{Ext}_A^{n+2}(M, N) .
$$
Si $\mathrm{dp}_A(M'), \mathrm{dp}_A(M'') \leq n$, alors $\mathrm{Ext}_A^{n+1}(M', N) = 0$ et $\mathrm{Ext}_A^{n+1}(M'', N) = 0$ (prop. 1) donc $\mathrm{Ext}_A^{n+1}(M, N) = 0$ et $\mathrm{dp}_A(M) \leq n$ (prop. 1), de sorte que
$$
\mathrm{dp}_A(M) \leq \sup (\mathrm{dp}_A(M'), \mathrm{dp}_A(M'')) .
$$

Si $\mathrm{dp}_A(M)<\sup\bigl(\mathrm{dp}_A(M'),\mathrm{dp}_A(M'')\bigr)$, alors nécessairement $\mathrm{dp}_A(M)<+\infty$. Pour tout $n>\mathrm{dp}_A(M)$, et tout A-module N, on a

$$
\operatorname{Ext}_A^{n+1}(M',N)\ne0\Longleftrightarrow\operatorname{Ext}_A^{n+2}(M'',N)\ne0,
$$

d’après la suite exacte précédente ; d’après la prop. 1, cela implique aussitôt $\mathrm{dp}_A(M'')=\mathrm{dp}_A(M')+1$, puisque l’une des quantités $\mathrm{dp}_A(M')$, $\mathrm{dp}_A(M'')$ est $>\mathrm{dp}_A(M)$.

**Example.** — Soit $a$ un élément de A qui n’est ni inversible, ni diviseur de zéro à droite.
Alors $\mathrm{dp}_A(A/Aa)=1$.

En effet, d’après la suite exacte $0\longrightarrow A_s\xrightarrow{\varphi} A_s\longrightarrow A/Aa\longrightarrow0$, où $\varphi(x)=xa$, on a $\mathrm{dp}_A(A/Aa)\leq1$. Si $\mathrm{dp}_A(A/Aa)<1$, alors $A/Aa$ est projectif, et il existe une application A-linéaire $\psi:A_s\longrightarrow A_s$ telle que $\psi\circ\varphi=\mathrm{Id}$ ; cela implique

$$
1=\psi(\varphi(1))=\psi(a)=a.\psi(1)
$$

et $a$ est inversible.

#### Proposition 2 {#alg-x-s8-prop-2 .statement}

Supposons A noethérien à gauche. Soient M un A-module de type fini et $n$ un entier $\geq0$. Les conditions suivantes sont équivalentes :

(i) $\mathrm{dp}_A(M)\leq n$.

(i bis) M possède une résolution projective P de longueur $\leq n$ telle que $P_i$ soit un A-module de type fini pour chaque $i$.

(ii) $\operatorname{Ext}_A^r(M,N)=0$ pour tout A-module de type fini N et tout entier $r>n$.

(iii) $\operatorname{Ext}_A^{n+1}(M,N)=0$ pour tout A-module de type fini N.

(iv) $\operatorname{Tor}^A_r(P,M)=0$ pour tout A-module à droite P et tout $r>n$.

(v) $\operatorname{Tor}^A_{n+1}(A/a,M)=0$ pour tout idéal à droite de type fini $a$ de A.

(i bis) $\Rightarrow$ (i) : c’est trivial.

(i) $\Rightarrow$ (ii) : cela résulte du lemme 1.

(ii) $\Rightarrow$ (iii) : c’est trivial.

(iii) $\Rightarrow$ (i) : d’après (iii) et X, p. 107, prop. 5, on a $\operatorname{Ext}_A^{n+1}(M,N)=0$ pour tout A-module N, d’où (i) d’après la prop. 1.

(i) $\Rightarrow$ (iv) : cela résulte du lemme 1.

(iv) $\Rightarrow$ (v) : c’est trivial.

(v) $\Rightarrow$ (i bis) : soit $(L,d)$ une résolution libre de M telle que $L_r$ soit de type fini pour tout $r$ (X, p. 53, prop. 6). Posons $K=\mathrm{Z}_{n-1}(L)$ ; alors K est de type fini comme sous-module de $L_{n-1}$ et on a une suite exacte

$$
0\longrightarrow K\longrightarrow L_{n-1}\longrightarrow L_{n-2}\longrightarrow\cdots\longrightarrow L_1\longrightarrow L_0\longrightarrow M\longrightarrow0.
\tag{1}
$$

D’après (v) et X, p. 131, cor. 3, on a $\operatorname{Tor}^A_1(A/a,K)=0$ pour tout idéal à droite de type fini $a$ de A. D’après le th. 2 de X, p. 74, le A-module K est plat ; comme il est de type fini, donc de présentation finie (X, p. 10, prop. 5), il est projectif (X, p. 13, cor.), donc (1) est une résolution projective de M.

#### Corollaire {#alg-x-s8-n1-cor-1 .statement}

Supposons $A$ noethérien à gauche et soit $\mathcal{C}_0$ (resp. $\mathcal{C}$) l’ensemble des classes des $A$-modules projectifs de type fini (resp. des $A$-modules de dimension projective finie et de type fini). Alors l’homomorphisme des groupes de Grothendieck $K(\mathcal{C}_0) \to K(\mathcal{C})$ est bijectif.

Cela résulte de X, p. 58, th. 1 (notons que $\mathcal{C}_0$ et $\mathcal{C}$ sont exacts à gauche d’après le cor. 2).

### 2. L’homomorphisme $\operatorname{Tor}_n^A(P, M) \to \operatorname{Hom}_A(\operatorname{Ext}_A^n(M, A), P)$

Soient $M$ un $A$-module à gauche, $P$ un $A$-module à droite, $n$ un entier $\geqslant 0$. L’application $k$-bilinéaire (X, p. 129)

$$
c_{P;M,A_s} : \operatorname{Ext}_A^n(M, A) \times \operatorname{Tor}_n^A(P, M) \to P \otimes_A A
$$

correspond à une application $k$-linéaire

(2)
$$
\operatorname{Tor}_n^A(P, M) \to \operatorname{Hom}_k(\operatorname{Ext}_A^n(M, A), P);
$$

de plus, si l’on munit $\operatorname{Ext}_A^n(M, A)$ de la structure de $A$-module à droite provenant de la structure de bimodule de $A$, l’image de (2) est formée d’applications $A$-linéaires, comme on le vérifie aussitôt ; on en déduit un $k$-homomorphisme, dit canonique

(3)
$$
\operatorname{Tor}_n^A(P, M) \to \operatorname{Hom}_A(\operatorname{Ext}_A^n(M, A), P).
$$

#### Proposition 3 {#alg-x-s8-prop-3 .statement}

a) Si $\mathrm{dp}_A(M) \leqslant n$, l’homomorphisme canonique (3) est injectif.
b) Si $\mathrm{dp}_A(M) \leqslant n$, si $A$ est noethérien à gauche et si $M$ est de type fini, l’homomorphisme canonique (3) est bijectif.

Raisonnons par récurrence sur $n$. Si $n = 0$, $M$ est projectif, l’homomorphisme (3) se réduit à l’homomorphisme canonique $P \otimes_A M \to \operatorname{Hom}_A(M^*, P)$ de II, p. 77, et la proposition résulte de loc. cit., corollaire. Si $n > 0$, soit

(4)
$$
0 \to N \to L \to M \to 0
$$

une suite exacte de $A$-modules où $L$ est libre (et de type fini dans le cas $b$) ; alors $\mathrm{dp}_A(N) \leqslant n - 1$ (X, p. 135, cor. 2, c)) et $N$ est de type fini dans le cas $b$.

Soit $\theta \in \operatorname{Ext}_A^1(M, N)$ la classe associée à la suite exacte (4) (X, p. 117, déf. 1). Notons
$$
u_n : \operatorname{Ext}_A^{n-1}(N, A) \to \operatorname{Ext}_A^n(M, A) \qquad v_n : \operatorname{Tor}_n^A(P, M) \to \operatorname{Tor}_{n-1}^A(P, N)
$$
les applications définies par $u_n(\alpha) = \alpha \circ \theta$ et $v_n(\beta) = \theta \circ \beta$. On a
$$
(\alpha \circ \theta) \circ \beta = \alpha \circ (\theta \circ \beta)
$$

pour tous $\alpha\in\operatorname{Ext}_A^{n-1}(N,A)$, $\beta\in\operatorname{Tor}_n^A(P,M)$ (X, p. 129, prop. 6), de sorte que le
diagramme

$$
\begin{array}{ccc}
\operatorname{Tor}_n^A(P,M)&\longrightarrow&\operatorname{Hom}_A(\operatorname{Ext}_A^n(M,A),P)\\
\downarrow v_n&&\downarrow\operatorname{Hom}(u_n,1)\\
\operatorname{Tor}_{n-1}^A(P,N)&\longrightarrow&\operatorname{Hom}_A(\operatorname{Ext}_A^{n-1}(N,A),P),
\end{array}
\tag{5}
$$

où les flèches horizontales sont les homomorphismes canoniques, est commutatif.

Si $n=1$, on a ainsi un diagramme commutatif :

$$
\begin{array}{ccccc}
0&&&&0\\
\downarrow&&&&\downarrow\\
\operatorname{Tor}_1^A(P,M)&\longrightarrow&\operatorname{Hom}_A(\operatorname{Ext}_A^1(M,A),P)\\
\downarrow v_1&&&&\downarrow\operatorname{Hom}(u_1,1)\\
P\otimes_A N&\longrightarrow&\operatorname{Hom}_A(N^*,P)\\
\downarrow&&&&\downarrow\\
P\otimes_A L&\longrightarrow&\operatorname{Hom}_A(L^*,P)
\end{array}
$$

où les colonnes sont exactes ; on en déduit le résultat dans ce cas. Si $n\geq 2$, les appli-
cations $u_n$ et $v_n$ sont bijectives (X, p. 128, cor. 4 et p. 131, cor. 3). D’après l’hypothèse
de récurrence, l’homomorphisme canonique

$$
\operatorname{Tor}_{n-1}^A(P,N)\longrightarrow\operatorname{Hom}_A(\operatorname{Ext}_A^{n-1}(N,A),P)
$$

est injectif (resp. bijectif) ; le diagramme (5) montre qu’il en est de même de l’homo-
morphisme canonique $\operatorname{Tor}_n^A(P,M)\longrightarrow\operatorname{Hom}_A(\operatorname{Ext}_A^n(M,A),P)$, ce qui achève la
démonstration.

### 3. Dimension homologique d’un anneau

#### Définition 2 {#alg-x-s8-def-2 .statement}

On appelle dimension homologique de $A$ et on note $\operatorname{dh}(A)$ la borne
supérieure dans $\mathbf{Z}$ de l’ensemble des entiers $n$ pour lesquels il existe deux $A$-modules M
et N tels que $\operatorname{Ext}_A^n(M,N)\neq 0$.

On a $\operatorname{dh}(0)=-\infty$, $\operatorname{dh}(A)\geq 0$ si $A\neq 0$. On verra ci-dessous que $\operatorname{dh}(A)=1$ si
$A$ est principal et n’est pas un corps, et que, si K est un corps commutatif

$$
\operatorname{dh}(K[X_1,\ldots,X_n])=n.
$$

#### Proposition 4 {#alg-x-s8-prop-4 .statement}

Soit $n$ un entier $\geq 0$. Les conditions suivantes sont équivalentes :

(i) $\operatorname{dh}(A)\leq n$,

(ii) pour tout $A$-module M, on a $\mathrm{dp}_A(M)\leq n$,

(ii′) pour tout $A$-module M de type fini, on a $\mathrm{dp}_A(M)\leq n$,

(iii) pour toute suite exacte

$$
0 \to K \to P_{n-1} \to P_{n-2} \to \ldots \to P_0
$$

où les $P_i$ sont projectifs, $K$ est projectif,

(iv) pour toute suite exacte

$$
I^0 \to I^1 \to \ldots \to I^{n-1} \to N \to 0
$$

où les $I^i$ sont injectifs, $N$ est injectif,

(v) tout $A$-module possède une résolution injective de longueur $\leq n$.

L’équivalence des conditions (i), (ii) et (iii) résulte de la prop. 1. On a évidemment (ii) $\Rightarrow$ (ii’). Il nous suffit donc de prouver (ii’) $\Rightarrow$ (iv) $\Rightarrow$ (v) $\Rightarrow$ (i).

(ii’) $\Rightarrow$ (iv) : avec les notations de (iv), soit $K$ le noyau de $I^0 \to I^1$. D’après X, p. 128, cor. 4, on a pour tout $A$-module $M$ un isomorphisme $\mathrm{Ext}_A^1(M, N) \to \mathrm{Ext}_A^{n+1}(M, K)$; il résulte alors de (ii’) que $\mathrm{Ext}_A^1(M, N)$ est nul pour tout $A$-module de type fini $M$. D’après X, p. 93, prop. 11, cela implique que $N$ est injectif, d’où (iv).

(iv) $\Rightarrow$ (v) : soit $M$ un $A$-module. Appliquant (iv) à la suite exacte

$$
0 \to M \to I^0(M) \to I^1(M) \to \ldots \to I^{n-1}(M) \to K^{n-1}(M) \to 0
$$

de X, p. 52, on conclut que $K^{n-1}(M)$ est injectif, d’où (v).

(v) $\Rightarrow$ (i) : cela résulte de X, p. 100, th. 1.

#### Remarque 1 {#alg-x-s8-n3-rem-1 .statement}

Si $\mathrm{dh}(A) \leq n < +\infty$, on a $\mathrm{Tor}_{n+1}^A(P, M) = 0$ pour tout $A$-module $M$ et tout $A$-module à droite $P$, puisque $\mathrm{dp}_A(M) \leq n$ (cf. lemme 1).

#### Remarque 2 {#alg-x-s8-n3-rem-2 .statement}

Pour que $\mathrm{dh}(A)$ soit finie, il faut et il suffit que $\mathrm{dp}_A(M)$ soit finie pour tout $A$-module $M$ non nul. Cela résulte en effet de ce qui précède et de X, p. 135, cor. 1.

#### Corollaire {#alg-x-s8-n3-cor-1 .statement}

Supposons $A$ noethérien à gauche et soit $n$ un entier $> 0$. Les conditions suivantes sont équivalentes :

(i) $\mathrm{dh}(A) \leq n$,

(ii) pour tout couple de $A$-modules $M$ et $N$ de type fini, on a $\mathrm{Ext}_A^{n+1}(M, N) = 0$,

(iii) pour tout $A$-module à gauche $M$ de type fini et tout $A$-module à droite $P$ de type fini, on a $\mathrm{Tor}_{n+1}^A(P, M) = 0$.

Cela résulte des prop. 2 et 4.

#### Remarque {#alg-x-s8-n3-rem-3 .statement}

D’après l’équivalence de (i) et (iii), on a $\mathrm{dh}(A) = \mathrm{dh}(A^\circ)$ si $A$ est noethérien à droite et à gauche. Cette égalité n’est pas satisfaite en général (X, p. 204, exercice 20).

#### Proposition 5 {#alg-x-s8-prop-5 .statement}

Supposons $A$ noethérien à gauche et de dimension homologique finie et soit $\mathcal{C}_0$ (resp. $\mathcal{C}$) l’ensemble des classes de $A$-modules projectifs de type fini (resp. des $A$-modules de type fini). Alors l’homomorphisme canonique des groupes de Grothendieck $K(\mathcal{C}_0) \to K(\mathcal{C})$ est bijectif.

Cela résulte de X, p. 137, cor.

### 4. Anneaux de dimension homologique 0

#### Proposition 6 {#alg-x-s8-prop-6 .statement}

Les conditions suivantes sont équivalentes :
(i) tout A-module est projectif,
(ii) tout A-module est injectif,
(iii) tout idéal de A est un module injectif,
(iv) dh(A) ≤ 0,
(v) A est semi-simple,
(vi) A est nœthérien et tout A-module est plat;
(vii) tout complexe de A-modules est scindé,
(viii) toute suite exacte de A-modules est scindée.

D’après la prop. 4, on a (i) ⇔ (ii) ⇔ (iv); d’après le cor. 1 à la prop. 4, on a (vi) ⇒ (iv). D’après X, p. 35, exemple 4, on a (i) ⇒ (vii); comme (ii) ⇒ (iii) et (vii) ⇒ (viii) sont triviales et que (viii) ⇒ (i) résulte de II, p. 39, prop. 4, il reste à prouver (iii) ⇒ (v) et (v) ⇒ (vi); la dernière assertion résulte de VIII, § 5, no 1, prop. 1 et 2; enfin si tout idéal de A est injectif, il est facteur direct dans A, d’où (iii) ⇒ (v).

### 5. Anneaux de dimension homologique 1

#### Proposition 7 {#alg-x-s8-prop-7 .statement}

Les conditions suivantes sont équivalentes :
(i) dh(A) ≤ 1,
(ii) tout sous-module d’un module projectif est projectif,
(ii’) tout idéal de A est projectif,
(iii) tout quotient d’un A-module injectif est injectif,
(iv) pour tout complexe projectif C, il existe un homologisme φ : C → H(C) tel que H(φ) = 1_{H(C)},
(v) pour tout complexe injectif C, il existe un homologisme ψ : H(C) → C tel que H(ψ) = 1_{H(C)}.

(i) ⇔ (ii) ⇔ (iii) : cela résulte de la prop. 4 de X, p. 138.
(ii) ⇒ (iv) : soit C un complexe projectif. Si (ii) est vérifié, le sous-module B(C) de C est projectif, d’où (iv) d’après X, p. 35, remarque b).
(iii) ⇒ (v) : soit C un complexe injectif. Si (iii) est vérifié, le quotient B_n(C) de C_{n+1} est injectif pour tout n, d’où (v) d’après X, p. 35, remarque a).
(iv) ⇒ (ii) : soient P un A-module projectif, M un sous-module de P, i : M → P l’injection canonique. Soit p : L → M un homomorphisme surjectif d’un module libre L sur M. Considérons le complexe projectif C tel que C_1 = L, C_0 = P, C_i = 0 pour i ≠ 0, 1, d_1 = i ◦ p. Si (iv) est satisfait, soit φ : C → H(C) un homologisme tel que H(φ) = 1_{H(C)}. Comme H_1(C) = Ker p, φ_1 est un projecteur de L sur Ker p, donc la suite exacte

$$
0 \to \mathrm{Ker}\ p \to L \xrightarrow{p} M \to 0
$$

est scindée et M est isomorphe à un facteur direct de L, donc est projectif.

$(v)\Rightarrow(iii)$ : soient I un module injectif, M un quotient de I, $\pi : I\to M$ la projection canonique. Soit $i : M\to J$ un homomorphisme injectif de M dans un module injectif J. Considérons le complexe injectif C tel que $C^0=I$, $C^1=J$, $C^i=0$ pour $i\ne0,1$, $d^0=i\circ\pi$. Si (v) est satisfait, soit $\psi : H(C)\to C$ un homomorphisme tel que $H(\psi)=1_{H(C)}$. Comme

$$H^1(C)=\operatorname{Coker}i,$$

$\psi^1$ est une section de la projection canonique $J\to\operatorname{Coker}i$, et M est facteur direct dans J, donc injectif.

$(ii)\Rightarrow(ii')$ : c’est trivial.

$(ii')\Rightarrow(ii)$ : cela résulte de VII, § 3, cor. 1 au th. 1.

#### Exemple {#alg-x-s8-n5-exa-1 .statement}

Si A est principal, alors $\operatorname{dh}(A)\leq1$.

#### Remarque {#alg-x-s8-n5-rem-1 .statement}

Si A est (commutatif) intègre, les conditions précédentes équivalent aussi aux suivantes :

$(iii')$ : tout A-module divisible est injectif,

$(vi)$ : tout A-module sans torsion est plat et A est noethérien.

Les anneaux intègres vérifiant ces conditions sont appelés anneaux de Dedekind (cf. X, p. 204, exercice 12 et AC, VII, § 2, no 2, th. 1).

#### Corollaire {#alg-x-s8-n5-cor-1 .statement}

Soient A un anneau de dimension homologique $\leq 1$, C un complexe de A-modules projectifs, $\widetilde C$ un complexe de A-modules à droite projectifs, C′ un complexe de A-modules injectifs, P un A-module à droite, M un A-module à gauche, n un entier. On a alors des suites exactes scindées

$$0\to\bigoplus_{p+q=n}H_p(\widetilde C)\otimes_A H_q(C)\xrightarrow{\gamma}H_n(\widetilde C\otimes_A C)\xrightarrow{\alpha}\bigoplus_{p+q=n-1}\operatorname{Tor}_1^A(H_p(\widetilde C),H_q(C))\to0,$$

$$0\to\prod_p\operatorname{Ext}_A^1(H_p(C),H^{n-p-1}(C'))\xrightarrow{\beta}H^n(\operatorname{Homgr}_A(C,C'))\xrightarrow{\lambda}\prod_p\operatorname{Homgr}_A(H_p(C),H^{n-p}(C'))\to0,$$

$$0\to P\otimes_A H_n(C)\xrightarrow{\gamma}H_n(P\otimes_A C)\xrightarrow{\alpha}\operatorname{Tor}_1^A(P,H_{n-1}(C))\to0,$$

$$0\to\operatorname{Ext}_A^1(H_{n-1}(C),M)\xrightarrow{\beta}H^n(\operatorname{Homgr}_A(C,M))\xrightarrow{\lambda}\operatorname{Hom}_A(H_n(C),M)\to0.$$

Puisque $Z(C)$, $B(C)$, $Z(\widetilde C)$ et $B(\widetilde C)$ sont projectifs et $B(C')$ injectif, cela résulte de X, p. 78, cor. 2, p. 96, cor. 1 et p. 98, cor. 2.

### 6. Dimension homologique des anneaux de polynômes

#### Lemme 2 {#alg-x-s8-lem-2 .statement}

Soient $\rho : A\to A'$ un homomorphisme d’anneaux, M un A-module, M′ un A′-module. Si le A-module $A'_d$ est plat, on a $\mathrm{dp}_A(A'\otimes_A M)\leq\mathrm{dp}_A(M)$. Si le A-module $A'_s$ est projectif, on a $\mathrm{dp}_A(M')\leq\mathrm{dp}_{A'}(M')$.

La première assertion est claire si $\mathrm{dp}_A(M) = \pm \infty$; si $\mathrm{dp}_A(M) = n \in \mathbf{N}$, il existe une suite exacte de $A$-modules

$$
0 \to P_n \to P_{n-1} \to \ldots \to P_0 \to M \to 0
$$

où les $P_i$ sont projectifs ; la suite de $A'$-modules

$$
0 \to A' \otimes_A P_n \to A' \otimes_A P_{n-1} \to \ldots \to A' \otimes_A P_0 \to A' \otimes_A M \to 0
$$

est exacte, puisque $A'_d$ est plat, et les $A'$-modules $A' \otimes_A P_i$ sont projectifs (II, p. 89, cor.) ; donc $\mathrm{dp}_{A'}(A' \otimes_A M) \leq n = \mathrm{dp}_A(M)$. La seconde assertion est claire si $\mathrm{dp}_{A'}(M') = \pm \infty$; si $\mathrm{dp}_{A'}(M') = m \in \mathbf{N}$, il existe une suite exacte de $A'$-modules

$$
0 \to P'_m \to P'_{m-1} \to \ldots \to P'_0 \to M' \to 0 ,
$$

où les $P'_i$ sont projectifs ; la suite des $A$-modules sous-jacents est exacte. D’autre part chaque $P'_i$ est un sous-$A'$-module facteur direct d’un module ${A'_s}^{(1)}$, donc est un $A$-module projectif ; on a donc $\mathrm{dp}_A(M') \leq m = \mathrm{dp}_{A'}(M')$.

#### Lemme 3 {#alg-x-s8-lem-3 .statement}

*Supposons A commutatif et soit M un A[X]-module.*
  a) *On a* $\mathrm{dp}_A(M) \leq \mathrm{dp}_{A[X]}(M) \leq \mathrm{dp}_A(M) + 1$.
  b) *Si l’homothétie* $X_M$ *est injective, on a* $\mathrm{dp}_A(M/XM) \leq \mathrm{dp}_{A[X]}(M)$.
  c) *Si* $XM = 0$, *on a* $\mathrm{dp}_A(M) + 1 = \mathrm{dp}_{A[X]}(M)$.
  a) On a une suite exacte de $A[X]$-modules (III, p. 106 et VII, § 5, no 1)

$$
0 \to A[X] \otimes_A M \to A[X] \otimes_A M \to M \to 0 ;
$$

l’assertion *a)* résulte alors de X, p. 135, cor. 2 et du lemme 2.

*b)* Si $\mathrm{dp}_{A[X]}(M) = \pm \infty$, l’assertion est triviale. Si $M$ est projectif et non nul, alors le $A$-module $M/XM$ s’identifie à $A \otimes_{A[X]} M$, donc est projectif, et on a $\mathrm{dp}_A(M/XM) \leq 0 = \mathrm{dp}_{A[X]}(M)$. Raisonnons par récurrence sur $\mathrm{dp}_{A[X]}(M) = n$, supposé $> 0$. Considérons une suite exacte de $A[X]$-modules $0 \to N \to L \to M \to 0$, où $L$ est un $A[X]$-module libre ; appliquant au diagramme

$$
\begin{array}{ccc}
0 & \longrightarrow & N \longrightarrow L \longrightarrow M \longrightarrow 0 \\
& & \downarrow \quad \downarrow \quad \downarrow \\
0 & \longrightarrow & N \longrightarrow L \longrightarrow M \longrightarrow 0
\end{array}
$$

la prop. 2 de X, p. 4, on voit que $X_N$ est injectif et qu’on a la suite exacte

$$
0 \to N/XN \to L/XL \to M/XM \to 0 .
$$

Comme $L$ est libre sur $A[X]$, $L/XL$ est libre sur $A$ et l’on a

$$
\mathrm{dp}_{A[X]}(N) = n - 1 , \quad \mathrm{dp}_A(M/XM) \leq 1 + \mathrm{dp}_A(N/XN) ;
$$

comme $\mathrm{dp}_A(N/XN) \leq n - 1$ d’après l’hypothèse de récurrence, on en tire $\mathrm{dp}_A(M/XM) \leq n$, ce qu’il fallait démontrer.

c) L’assertion est triviale si $\mathrm{dp}_{A[X]}(M) = \pm \infty$, et aussi si $\mathrm{dp}_{A[X]}(M) = 0$ (qui est impossible puisque $XM = 0$). On peut donc supposer $\mathrm{dp}_{A[X]}(M) = n > 0$. Considérant comme ci-dessus une suite exacte $0 \to N \to L \to M \to 0$, où $L$ est un $A[X]$-module libre, on obtient une suite exacte de $A$-modules

$$
0 \to M \to N/XN \to L/XL \to M \to 0 .
$$

D’après b), on a $\mathrm{dp}_A(N/XN) \leq \mathrm{dp}_{A[X]}(N) = \mathrm{dp}_{A[X]}(M) - 1 = n - 1$; comme $\mathrm{dp}_A(L/XL) = 0$, on déduit de la suite exacte précédente, en appliquant deux fois $X$, p. 135, cor. 2, que $\mathrm{dp}_A(M) \leq n - 1$. Mais, d’après a), on a

$$
\mathrm{dp}_A(M) \geq \mathrm{dp}_{A[X]}(M) - 1 = n - 1 ,
$$

d’où c).

#### Théorème 1 {#alg-x-s8-thm-1 .statement}

*Supposons $A$ commutatif. Alors*

$$
dh(A[X]) = dh(A) + 1 .
$$

Pour tout $A[X]$-module $M$, on a (*lemme 3*)

$$
\mathrm{dp}_{A[X]}(M) \leq \mathrm{dp}_A(M) + 1 \leq dh(A) + 1
$$

donc $dh(A[X]) \leq dh(A) + 1$; inversement, si $M$ est un $A$-module, soit $\overline{M}$ le $A[X]$-module obtenu en munissant $M$ de la structure pour laquelle $XM = 0$, alors (*lemme 3*)

$$
\mathrm{dp}_A(M) = \mathrm{dp}_{A[X]}(\overline{M}) - 1 \leq dh(A[X]) - 1 ,
$$

donc $dh(A) \leq dh(A[X]) - 1$.

#### Corollaire 1 {#alg-x-s8-thm-1-cor-1 .statement}

*Supposons $A$ commutatif. On a*

$$
dh(A[X_1, ..., X_n]) = dh(A) + n .
$$

Cela résulte du théorème par récurrence sur $n$.

#### Corollaire 2 {#alg-x-s8-thm-1-cor-2 .statement}

*Soit $K$ un corps commutatif* (resp. *un anneau principal* *ou de Dedekind* *qui n’est pas un corps*). *Alors* $dh(K[X_1, ..., X_n])$ *est égal à* $n$ (resp. $n + 1$). Cela résulte de ce que $dh(K) = 0$ (resp. $dh(K) = 1$).

### 7. Dimension homologique des modules gradués

Dans ce numéro, on suppose que $A$ est un anneau gradué à degrés $\geq 0$. On note $(A_n)_{n \in \mathbf{Z}}$ sa graduation ; on a donc $A_n = 0$ pour $n < 0$, $A_0$ est un sous-anneau de $A$, $J_0 = \bigoplus_{n > 0} A_n$ est un idéal bilatère de $A$ et l’anneau gradué quotient $A/J_0$ s’identifie à $A_0$.

#### Lemme 4 {#alg-x-s8-lem-4 .statement}

Soit $M$ un $A$-module gradué borné inférieurement (X, p. 56). Si $A_0 \otimes_A M = 0$, alors $M = 0$.

Comme $A_0 \otimes_A M$ est isomorphe à $M/J_0 M$, ce n’est autre que ll, p. 171, prop. 6.

#### Lemme 5 {#alg-x-s8-lem-5 .statement}

Soit $M$ un $A$-module gradué borné inférieurement, et soit
$$
s : A \otimes_{A_0} M/J_0 M \to M
$$
un $A$-homomorphisme gradué tel que $1 \otimes_A s : A_0 \otimes_A (A \otimes_{A_0} M/J_0 M) \to A_0 \otimes_A M$
soit l’isomorphisme canonique. Alors $s$ est surjectif. Si $\mathrm{Tor}_1^A(A_0, M) = 0$, $s$ est bijectif.

On a une suite exacte
$$
0 \to \mathrm{Ker}\ s \to A \otimes_{A_0} M J_0 M \to M \to \mathrm{Coker}\ s \to 0
$$
et les $A$-modules gradués $\mathrm{Ker}\ s$ et $\mathrm{Coker}\ s$ sont bornés inférieurement. De la suite exacte $A_0 \otimes_A (A \otimes_{A_0} M/J_0 M) \xrightarrow{1 \otimes s} A_0 \otimes_A M \to A_0 \otimes_A \mathrm{Coker}\ s \to 0$, on déduit que $A_0 \otimes_A \mathrm{Coker}\ s = 0$, donc $s$ est surjectif (lemme 4). On a alors une suite exacte
$$
\mathrm{Tor}_1^A(A_0, M) \to A_0 \otimes_A \mathrm{Ker}\ s \to A_0 \otimes_A (A \otimes_{A_0} M/J_0 M) \xrightarrow{1 \otimes s} A_0 \otimes_A M .
$$
Si $\mathrm{Tor}_1^A(A_0, M) = 0$, alors $A_0 \otimes_A \mathrm{Ker}\ s = 0$ et $s$ est injectif (lemme 4).

#### Proposition 8 {#alg-x-s8-prop-8 .statement}

Soit $M$ un $A$-module gradué borné inférieurement.

a) Les conditions suivantes sont équivalentes :
(i) $M$ est isomorphe à un $A$-module gradué de la forme $A \otimes_{A_0} N$, où $N$ est un $A_0$-module gradué projectif (resp. gradué libre) ;
(ii) $M$ est un $A$-module projectif (resp. gradué libre) ;
(iii) $M/J_0 M$ est un $A_0$-module projectif (resp. gradué libre) et $\mathrm{Tor}_1^A(A_0, M) = 0$.

b) Supposons de plus que $M$ ait un système générateur formé d’éléments homogènes de degrés bornés. Alors les conditions suivantes sont équivalentes :
(i) Le $A$-module gradué $M$ possède une suite de composition finie dont les quotients sont isomorphes à des $A$-modules gradués de la forme $A \otimes_{A_0} N$, où $N$ est un $A_0$-module gradué plat ;
(ii) $M$ est un $A$-module plat ;
(iii) $M/J_0 M$ est un $A_0$-module plat et $\mathrm{Tor}_1^A(A_0, M) = 0$.

Dans chacun des deux cas, on a évidemment (i) $\Rightarrow$ (ii) $\Rightarrow$ (iii). Il s’agit donc de démontrer (iii) $\Rightarrow$ (i).

a) Le $A$-module gradué $A \otimes_{A_0} M/J_0 M$ est un $A$-module projectif puisque $M/J_0 M$ est un $A_0$-module projectif. L’homomorphisme canonique de $A$-modules
$$
p : M \to M/J_0 M
$$
est surjectif ; il existe donc un $A$-homomorphisme gradué de degré zéro
$$
s : A \otimes_{A_0} M/J_0 M \to M
$$
tel que $p \circ s(a \otimes x) = ax$ pour $a \in A$ et $x \in M/J_0 M$.

D’après le lemme 5, $s$ est un isomorphisme de $A$-modules de $A\otimes_{A_0}M/J_0M$ sur $M$, d’où (i).

b) D’après l’hypothèse sur $M$, il existe des entiers $a,b$ avec $a\leq b$ tels que $M$ soit engendré par $\displaystyle\bigoplus_{a\leq i\leq b}M_i$. Raisonnons par récurrence sur l’entier positif $b-a$.

Si $b-a=0$, alors $M$ est engendré par $M_a$ et le $A_0$-homomorphisme canonique
$$
M_a\longrightarrow M/J_0M
$$
est bijectif; on déduit alors du $A$-homomorphisme $A\otimes_{A_0}M_a\longrightarrow M$ défini par la structure de $A$-module de $M$ un $A$-homomorphisme gradué
$$
s:A\otimes_{A_0}M/J_0M\longrightarrow M
$$
satisfaisant à la condition du lemme 5. Alors, d’après le lemme 5, $s$ est bijectif, d’où (i).

Dans le cas général, soient $M^{(a)}$ le sous-$A$-module (gradué) de $M$ engendré par $M_a$ et $M'$ le quotient $M/M^{(a)}$. On a une suite exacte
$$
0\longrightarrow M^{(a)}\xrightarrow{f}M\xrightarrow{g}M'\longrightarrow0,
$$
d’où, puisque $\operatorname{Tor}_1^A(A_0,M)=0$ par hypothèse, des suites exactes
$$
\tag{6}
\operatorname{Tor}_2^A(A_0,M')\longrightarrow\operatorname{Tor}_1^A(A_0,M^{(a)})\longrightarrow0
$$
$$
\tag{7}
0\longrightarrow\operatorname{Tor}_1^A(A_0,M')\longrightarrow M^{(a)}/J_0M^{(a)}
\xrightarrow{1\otimes f}M/J_0M\xrightarrow{1\otimes g}M'/J_0M'\longrightarrow0.
$$

Mais l’homomorphisme canonique $M_a\longrightarrow M^{(a)}/J_0M^{(a)}$ est bijectif. Il s’ensuit que l’homomorphisme $1\otimes f:M^{(a)}/J_0M^{(a)}\longrightarrow M/J_0M$ est injectif et que son image est un sous-$A_0$-module facteur direct de $M/J_0M$. Il résulte alors de la suite exacte (7) que $\operatorname{Tor}_1^A(A_0,M')=0$ et que le $A_0$-module $M'/J_0M'$ est plat puisque isomorphe à un facteur direct de $M/J_0M$. D’après l’hypothèse de récurrence (qui s’applique à $M'$ puisque celui-ci est engendré par les $M'_i$ pour $a<i\leq b$), $M'$ satisfait à la condition (i), donc est plat. On déduit alors de la suite exacte (6) que $\operatorname{Tor}_1^A(A_0,M^{(a)})=0$, mais $M^{(a)}/J_0M^{(a)}$ s’identifie à $M_a$ qui est un $A_0$-module plat (comme sous-module facteur direct de $M/J_0M$) ; d’après ce qu’on a déjà démontré, le $A$-module gradué $M^{(a)}$ est isomorphe à $A\otimes_{A_0}M_a$, donc satisfait aussi à (i), ce qui achève la démonstration.

#### Corollaire 1 {#alg-x-s8-prop-8-cor-1 .statement}

Soit $M$ un $A$-module gradué de type fini. Si le $A_0$-module $M/J_0M$ est projectif (resp. gradué libre, resp. plat) et si $\operatorname{Tor}_1^A(A_0,M)=0$, alors le $A$-module $M$ est projectif (resp. gradué libre, resp. plat).

#### Corollaire 2 {#alg-x-s8-prop-8-cor-2 .statement}

Supposons que tout $A_0$-module projectif soit libre (resp. que $A$ soit noethérien et que tout $A_0$-module projectif de type fini soit libre). Soit $M$ un $A$-module gradué borné inférieurement (resp. un $A$-module gradué de type fini) et soit $n$ un entier $\geq 0$ tel que $\operatorname{pd}_A(M)\leq n$. Il existe une suite exacte de $A$-modules gradués et d’homomorphismes gradués de degré $0$
$$
0\longrightarrow L_n\longrightarrow L_{n-1}\longrightarrow\cdots\longrightarrow L_0\longrightarrow M\longrightarrow0
$$

où les $L_i$ sont gradués libres et bornés inférieurement (resp. gradués libres et de type fini).

En effet, il existe (X, p. 56, prop. 11) une suite exacte de A-modules gradués et d’homomorphismes de degré 0
$$
0 \to L_n \to L_{n-1} \to \ldots \to L_0 \to M \to 0
$$
où les $L_i$ sont bornés inférieurement (resp. de type fini) pour $0 \leq i \leq n$ et gradués libres pour $0 \leq i \leq n - 1$.

Comme $\mathrm{dp}_A(M) \leq n$, le A-module $L_n$ est projectif ; donc $A_0 \otimes_A L_n$ est un $A_0$-module projectif, donc gradué libre ; comme $L_n$ est borné inférieurement et $A_0 \otimes_A L_n$ gradué libre, $L_n$ est gradué libre (prop. 7).

#### Corollaire 3 (Théorème des syzygies de Hilbert) {#alg-x-s8-prop-8-cor-3 .statement}

*Supposons que $A_0$ soit un corps commutatif et que $A$ soit engendré comme $A_0$-algèbre par $n$ éléments homogènes de degrés $> 0$ algébriquement indépendants. Pour tout $A$-module gradué $M$ borné inférieurement (resp. de type fini), il existe une suite exacte de $A$-modules gradués et d’homomorphismes gradués de degrés 0*
$$
0 \to L_n \to L_{n-1} \to \ldots \to L_0 \to M \to 0,
$$
où les $L_i$ sont gradués libres et bornés inférieurement (resp. et de type fini).

En effet, $dh(A) = n$ d’après le théorème 1 de X, p. 143, et on applique le cor. 2.

#### Remarque {#alg-x-s8-n7-rem-1 .statement}

Le cor. 2 s’applique également aux cas suivants :
a) $A_0$ est principal et $A = A_0[X_1, ..., X_{n-1}]$;
b) *$A_0$ est noethérien local régulier de dimension $r$ et $A = A_0[X_1, ..., X_n, r]$.*

#### Corollaire 4 {#alg-x-s8-prop-8-cor-4 .statement}

*Supposons $A_0$ semi-simple. Soient $M$ un $A$-module gradué borné inférieurement et $n$ un entier $\geq 0$. Pour que $\mathrm{dp}_A(M) \leq n$, il faut et il suffit que*
$$
\operatorname{Tor}_{n+1}^A(A_0, M) = 0.
$$
Si $\mathrm{dp}_A(M) \leq n$, alors $\operatorname{Tor}_{n+1}^A(A_0, M) = 0$ (X, p. 135, lemme 1). Inversement, soit $0 \to K \to L_{n-1} \to ... \to L_1 \to L_0 \to M \to 0$ une suite exacte de $A$-modules gradués bornés inférieurement telle que $L_0, ..., L_{n-1}$ soient gradués libres (X, p. 56, prop. 11); d’après le cor. 3 de X, p. 131, l’égalité $\operatorname{Tor}_{n+1}^A(A_0, M) = 0$ implique $\operatorname{Tor}_1^A(A_0, K) = 0$; comme $K/J_0 K$ est un $A_0$-module projectif puisque $A_0$ est semi-simple (X, p. 140, prop. 6), $K$ est projectif d’après la prop. 8 (X, p. 144), et $\mathrm{dp}_A(M) \leq n$.

#### Corollaire 5 {#alg-x-s8-prop-8-cor-5 .statement}

*Supposons l’anneau $A_0$ semi-simple. Si $\operatorname{Tor}_{n+1}^A(A_0, A_0) = 0$, on a $\mathrm{dp}_A(M) \leq n$ pour tout $A$-module gradué borné inférieurement.

Notons $A^\circ$ l’anneau gradué opposé à $A$ : on a $(A^\circ)_0 = (A_0)^\circ$, donc $(A^\circ)_0$ est semi-simple (VIII, § 5, n° 1, remarque 3). Comme $\operatorname{Tor}_{n+1}^{A^\circ}(A_0^\circ, A_0^\circ) = 0$, on a $\mathrm{dp}_A(A_{0s}^\circ) \leq n$ d’après le cor. 4 : cela implique $\operatorname{Tor}_{n+1}^{A^\circ}(M_0, A_0^\circ) = 0$ pour tout $A$-module $M$, donc $\operatorname{Tor}_{n+1}^A(A_0, M) = 0$ et on applique le cor. 4.

## EXERCICES {#alg-x-s8-exercises}

See the [exercises for § 8](exercises/s8/).
