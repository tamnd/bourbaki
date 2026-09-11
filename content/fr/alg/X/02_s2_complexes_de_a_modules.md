---
book: alg
book_title: Algebra
chapter: X
chapter_title: ALGÈBRE HOMOLOGIQUE
section: 2
section_title: Complexes de A-modules
lang: fr
source: alg-x-fr
book_pages: A X.23-A X.46, A X.173-A X.178
pdf_pages: 0029-0052, 0179-0184
extraction: ocr
subsections:
    - "no": 1
      title: Complexes de A-modules
      page: 23
      pdf_page: 29
    - "no": 2
      title: ' Opérations sur les complexes'
      page: 27
      pdf_page: 33
    - "no": 3
      title: L’homomorphisme de liaison et la suite exacte d’homologie
      page: 29
      pdf_page: 35
    - "no": 4
      title: Homotopies
      page: 32
      pdf_page: 38
    - "no": 5
      title: Complexes scindés
      page: 34
      pdf_page: 40
    - "no": 6
      title: Cône et cylindre d’un morphisme de complexes
      page: 36
      pdf_page: 42
    - "no": 7
      title: Le cône d’un morphisme injectif ; nouvelle définition de l’homomorphisme de liaison
      page: 39
      pdf_page: 45
    - "no": 8
      title: Caractéristiques d’Euler-Poincaré
      page: 40
      pdf_page: 46
    - "no": 9
      title: Complexes de modules à droite, complexes de multimodules
      page: 43
      pdf_page: 49
    - "no": 10
      title: 'Exemple : complexe de de Rham'
      page: 43
      pdf_page: 49
statements: 59
exercises: 18
content_sha256: 000a48d0cc41203e5b65717dc12655c3172e383b3cbca3cef557d81d8756d9cb
---

## § 2. COMPLEXES DE A-MODULES

*Dans ce paragraphe, on désigne par $A$ un anneau. Lorsque nous parlerons de $A$-modules sans préciser, il sera toujours question de $A$-modules à gauche.*

*Nous appellerons modules gradués les modules gradués de type $\mathbf{Z}$ (II, p. 164).*

*Si $M$ est un $A$-module gradué, de graduation $(M_n)_{n\in\mathbf{Z}}$, on pose $M^n=M_{-n}$ et on dit que $M_n$ (resp. $M^n$) est la composante homogène de degré descendant $n$ (resp. de degré ascendant $n$) de $M$. Si $u:M\to N$ est un homomorphisme gradué de degré $p$ de $A$-modules gradués (II, p. 166), on note $u_n:M_n\to M_{n+p}$ (resp. $u^n:M^n\to M^{n-p}$) l’homomorphisme déduit de $u$ ; on l’appelle la composante homogène de degré descendant (resp. ascendant) $n$ de $u$ ; on dit aussi que $u$ est de degré descendant $p$ ou de degré ascendant $-p$.*

### 1. Complexes de A-modules

#### Définition 1 {#alg-x-s2-def-1 .statement}

*Un complexe différentiel de A-modules est un couple $(C,d)$ formé d’un $A$-module gradué $C$ et d’un endomorphisme $d:C\to C$ gradué de degré descendant $-1$ et tel que $d\circ d=0$.*

On dit aussi complexe de A-modules, ou A-complexe, ou complexe. On écrit souvent C au lieu de (C, d) ; l’endomorphisme d s’appelle la différentielle du complexe (C, d), ou par abus de langage de C.

Si C_n (resp. C^n) est la composante homogène de degré descendant (resp. ascendant) n de C, la donnée de d équivaut à celle de la suite d’homomorphismes

(1)
$$
\cdots \longrightarrow C_{n+1} \xrightarrow{d_{n+1}} C_n \xrightarrow{d_n} C_{n-1} \longrightarrow \cdots
$$
resp.

(1')
$$
\cdots \longrightarrow C^{n-1} \xrightarrow{d^{n-1}} C^n \xrightarrow{d^n} C^{n+1} \longrightarrow \cdots
$$
telle que $d_n \circ d_{n+1} = 0$ pour tout $n \in \mathbf{Z}$ (resp. $d^n \circ d^{n-1} = 0$ pour tout $n \in \mathbf{Z}$). Par abus de langage, on appellera aussi complexe la donnée d’une telle suite de A-modules et d’homomorphismes.

On remarquera, à titre mnémotechnique, que lorsqu’on « suit le sens des flèches » dans les diagrammes (1) et (1’), le degré descendant diminue et le degré ascendant augmente.

Tout A-module gradué sera tacitement considéré comme un complexe en le munissant de la différentielle nulle ; les complexes ainsi obtenus seront appelés complexes à différentielle nulle. En particulier, tout A-module M sera muni de l’unique structure de A-complexe telle que $M_0 = M^0 = M$. Le complexe (C, d) est dit nul si C est réduit à 0. Dans la suite, on note 0 un complexe nul, choisi une fois pour toutes.

Adjoignons à l’ensemble ordonné $\mathbf{Z}$ deux éléments notés $-\infty$ et $+\infty$; notons $\overline{\mathbf{Z}}$ l’ensemble obtenu, et munissons-le de la relation d’ordre prolongeant celle de $\mathbf{Z}$ et telle que $-\infty < n < +\infty$ pour tout $n \in \mathbf{Z}$; toute partie de $\overline{\mathbf{Z}}$ possède une borne inférieure et une borne supérieure.

Soit C un complexe ; on appelle bornes droite et gauche $^1$ de C les éléments $b_d(C)$ et $b_g(C)$ de $\overline{\mathbf{Z}}$ définis par
$$
b_d(C) = \inf \{ n \in \mathbf{Z}, C_n \neq 0 \}, \quad b_g(C) = \sup \{ n \in \mathbf{Z}, C_n \neq 0 \}.
$$
On dit que C est nul à droite si $b_d(C) \geqslant 0$, borné à droite si $b_d(C) \neq -\infty$, nul à gauche si $b_g(C) \leqslant 0$, borné à gauche si $b_g(C) \neq +\infty$; on dit que C est borné si
$$
b_d(C) \neq -\infty, \quad b_g(C) \neq +\infty.
$$
On appelle longueur $^2$ de C et on note $l(C)$ l’élément de $\overline{\mathbf{Z}}$ défini comme suit : si C est nul, $l(C) = -\infty$; si C est borné et non nul $l(C) = b_g(C) - b_d(C)$; si C

$^1$ Les mots de droite et gauche sont relatifs à la description de C à l’aide des diagrammes (1) et (1’).
$^2$ On ne confondra pas la notion de longueur du complexe (C, d) et celle de longueur du module C (II, p. 21).

n’est pas borné, $l(C) = + \infty$. \* Avec les conventions de TG, IV, p. 13-17, on a toujours $l(C) = b_g(C) - b_d(C)$. \*

Par exemple, si $k$ composantes consécutives de $C$ sont non nulles, les autres étant nulles, on a $l(C) = k - 1$ si $k > 0$, $l(C) = - \infty$ si $k = 0$.

On dit que le complexe $(C, d)$ est libre, projectif, plat, injectif, si chacun des modules $C_n$ l’est. On notera que le complexe $(C, d)$ est projectif ou plat si et seulement si le module $C$ l’est (II, p. 39, prop. 3 et X, p. 8, prop. 4), mais que $C$ peut être libre sans que le complexe $(C, d)$ le soit (puisqu’un facteur direct d’un module libre n’est pas toujours libre), de même que $(C, d)$ peut être injectif sans que $C$ le soit (X, p. 170, exercice 21).

Soit $(C, d)$ un complexe. On pose $Z(C, d) = \mathrm{Ker}\,(d)$, $B(C, d) = \mathrm{Im}\,(d)$; ce sont des sous-modules gradués de $C$, appelés respectivement le module des cycles et le module des bords de $(C, d)$; les composantes homogènes de $Z(C, d)$ et $B(C, d)$ se notent $Z_n(C, d) = Z^{-n}(C, d)$, $B_n(C, d) = B^{-n}(C, d)$; on a $Z_n(C, d) = \mathrm{Ker}\,(d_n)$, $B_n(C, d) = \mathrm{Im}\,(d_{n+1})$, $Z^n(C, d) = \mathrm{Ker}\,(d^n)$, $B^n(C, d) = \mathrm{Im}\,(d^{n-1})$.

Puisque $d \circ d = 0$, on a $B(C) \subset Z(C)$; deux cycles sont dits homologues si leur différence est un bord; le module gradué quotient $H(C, d) = Z(C, d)/B(C, d)$ est appelé le module d’homologie de $(C, d)$; ses éléments sont les classes d’homologie; ses composantes homogènes sont notées $H_n(C, d) = H^{-n}(C, d)$.

#### Exemple {#alg-x-s2-n1-exa-1 .statement}

Si $C$ est à différentielle nulle, on a $Z(C) = C$, $B(C) = 0$ et $H(C)$ s’identifie canoniquement à $C$.

On a des suites exactes, dites canoniques :

(I$_n$) $$ 0 \to Z_n(C) \to C_n \xrightarrow{\delta_n} B_{n-1}(C) \to 0 $$
(II$_n$) $$ 0 \to B_n(C) \to Z_n(C) \to H_n(C) \to 0 $$
(III$_n$) $$ 0 \to B_n(C) \to C_n \to C_n/B_n(C) \to 0 $$
(IV$_n$) $$ 0 \to H_n(C) \to C_n/B_n(C) \xrightarrow{\overline{\delta}_n} B_{n-1}(C) \to 0 $$

où $\delta_n$ et $\overline{\delta}_n$ sont déduits de $d_n$. Par combinaison de (IV$_n$) et (II$_{n-1}$), on obtient la suite exacte

(V$_n$) $$ 0 \to H_n(C) \to C_n/B_n(C) \to Z_{n-1}(C) \to H_{n-1}(C) \to 0 , $$

qui s’écrit aussi, changeant $n$ en $-n$

(V$^n$) $$ 0 \to H^n(C) \to C^n/B^n(C) \to Z^{n+1}(C) \to H^{n+1}(C) \to 0 . $$

#### Définition 2 {#alg-x-s2-def-2 .statement}

Soient $(C, d)$ et $(C', d')$ deux complexes. Un morphisme $^1$ de $(C, d)$ dans $(C', d')$ est un A-homomorphisme gradué $u$ de degré 0 de $C$ dans $C'$ tel que
$$
d' \circ u = u \circ d .
$$

¹ Ou morphisme de degré 0 (cf. X, p. 81).

Pour tout $n$, on a donc $d'_n \circ u_n = u_{n-1} \circ d_n$ et ${d''}^n \circ u^n = u^{n+1} \circ d^n$. On a
$$
u(Z(C)) \subset Z(C') , \quad u(B(C)) \subset B(C') ,
$$
et on note $Z(u) : Z(C) \to Z(C')$, $B(u) : B(C) \to B(C')$, $H(u) : H(C) \to H(C')$, les homomorphismes de A-modules qu’on en déduit ; les composantes homogènes de ces morphismes sont notées $Z_n(u)$, $Z^n(u)$, ...

Si $v$ est un autre morphisme de $(C, d)$ dans $(C', d')$, alors $u + v$ est un morphisme de $(C, d)$ dans $(C', d')$, et on a
$$
Z(u + v) = Z(u) + Z(v) , \quad B(u + v) = B(u) + B(v) , \quad H(u + v) = H(u) + H(v) .
$$
De même, si $A$ est une algèbre sur un anneau commutatif $k$, et si $\lambda \in k$, alors $\lambda u$ est un morphisme de $(C, d)$ dans $(C', d')$ et on a
$$
Z(\lambda u) = \lambda Z(u) , \quad B(\lambda u) = \lambda B(u) , \quad H(\lambda u) = \lambda H(u) .
$$
Si $u' : (C', d') \to (C'', d'')$ est un autre morphisme de complexes, alors $u' \circ u$ est un morphisme de $(C, d)$ dans $(C'', d'')$ et on a
$$
Z(u' \circ u) = Z(u') \circ Z(u) , \quad B(u' \circ u) = B(u') \circ B(u) , \quad H(u' \circ u) = H(u') \circ H(u) .
$$
Il est clair qu’un morphisme bijectif est un isomorphisme.

#### Définition 3 {#alg-x-s2-def-3 .statement}

Soient $(C, d)$ et $(C', d')$ deux complexes. Un homologisme (ou quasi-isomorphisme) de $(C, d)$ dans $(C', d')$ est un morphisme $u$ de $(C, d)$ dans $(C', d')$ tel que $H(u)$ soit bijectif.

Tout isomorphisme est un homologisme, tout morphisme composé d’homologismes est un homologisme.

On dit que $(C, d)$ est d’homologie nulle si $H(C) = 0$, c’est-à-dire si l’unique morphisme de complexes $0 \to C$ (resp. $C \to 0$) est un homologisme. On dit que $(C, d)$ est acyclique en degré descendant $n$ (resp. en degré ascendant $n$) si $H_n(C) = 0$ (resp. $H^n(C) = 0$).

Soient $(C, d)$ un complexe et $p \in \mathbf{Z}$. On appelle $p$-ième translaté de $(C, d)$ le complexe $(C(p), d(p))$ obtenu comme suit : $C(p)$ est le A-module obtenu par décalage de $p$ de la graduation de $C$ (II, p. 163; exemple 3), de sorte que
$$
C(p)_n = C_{n+p} , \quad C(p)^n = C^{n-p} ;
$$
en particulier $C(p)_0 = C_p$; on notera aussi que $C$ est la somme directe de ses sous-modules gradués $C_p(-p)$, $p \in \mathbf{Z}$ (resp. $C^p(p)$, $p \in \mathbf{Z}$). On pose $d(p) = (-1)^p d$.
On a $Z(C(p)) = Z(C)(p)$, $B(C(p)) = B(C)(p)$ et $H(C(p)) = H(C)(p)$.

Par exemple, $d$ est un morphisme de complexes de $C$ dans $C(-1)$ et
$$
H(d) : H(C) \to H(C)(-1)
$$
est nul.

Pour tout morphisme de complexes $u : (C,d) \to (C',d')$, et tout $p \in \mathbf{Z}$, $u$ est aussi un morphisme de $(C(p),d(p))$ dans $(C'(p),d'(p))$ ; on le note parfois $u(p)$ et on a

$$
u(p)_n = u_{n+p}, \qquad u(p)^n = u^{n-p}.
$$

### 2.  Opérations sur les complexes

Sur l’ensemble $A \times A$, les deux lois

$$
(a,b) + (a',b') = (a+a',b+b')
$$

$$
(a,b)(a',b') = (aa',ab'+ba')
$$

définissent une structure d’anneau, notée $A(\varepsilon)$, d’élément unité $1=(1,0)$ ; l’injection $a \mapsto (a,0)=a1$ permet d’identifier $A$ à un sous-anneau de $A(\varepsilon)$ ; le module $A(\varepsilon)$ est libre de base $\{1,\varepsilon\}$ où $\varepsilon=(0,1)$ ; on a $\varepsilon^2=0$ et $\varepsilon$ est central dans $A(\varepsilon)$.

Lorsque $A$ est commutatif, $A(\varepsilon)$ est une algèbre de nombres duaux sur $A$ (III, p. 15).

Munissons $A(\varepsilon)$ de la graduation d’anneau (II, p. 164) pour laquelle $A(\varepsilon)_0=A\mathbin{.}1$, $A(\varepsilon)_{-1}=A\mathbin{.}\varepsilon$ et $A(\varepsilon)_n=0$ pour $n\neq 0,-1$. Il est clair que se donner une structure de $A$-complexe sur un ensemble $C$ revient à se donner sur $C$ une structure de $A(\varepsilon)$-module gradué, la différentielle $d$ correspondant à l’homothétie $\varepsilon_C$ ; de même les morphismes de complexes correspondent aux homomorphismes gradués de degré 0 de $A(\varepsilon)$-modules gradués. Les espèces de structure de $A(\varepsilon)$-modules gradués et de $A$-complexes sont donc équivalentes (E, IV, p. 9-10). Nous utiliserons ce fait pour transporter à la théorie des complexes, les notions usuelles de la théorie des modules gradués.

A la notion de sous-$A(\varepsilon)$-module gradué correspond celle de sous-complexe : un sous-complexe du complexe $(C,d)$ est donc un sous-module gradué $C'$ de $C$ tel que, pour tout $n\in\mathbf{Z}$, $d_n(C'_n)\subset C'_{n-1}$ ; si on note $d'$ le $A$-homomorphisme gradué de $C'$ dans $C'$ déduit de $d$, alors $(C',d')$ est une structure de complexe, dite induite par $(C,d)$. Sauf mention expresse du contraire, tout sous-complexe sera muni de la structure induite.

Nous laissons au lecteur le soin d’expli de même les notions de complexe-quotient, suite exacte de complexes, noyau, conoyau, image d’un morphisme de complexes, suivant le dictionnaire ci-dessous :

$$
\begin{array}{rcl}
A(\varepsilon)\text{-module gradué quotient} & = & \textit{complexe quotient},\\[2mm]
\left.
\begin{array}{l}
\text{noyau, conoyau, image d’un }A(\varepsilon)\text{-}\\
\text{homomorphisme gradué de degré 0}
\end{array}
\right\}
& = &
\begin{array}{l}
\textit{noyau, conoyau, image d’un morphisme}\\
\textit{de complexes},
\end{array}\\[4mm]
\left.
\begin{array}{l}
\text{suite exacte de }A(\varepsilon)\text{-modules gradués et d’homomorphismes gradués}\\
\text{de degré 0}
\end{array}
\right\}
& = & \textit{suite exacte de complexes.}
\end{array}
$$

Par exemple, les suites exactes canoniques du n° 1 donnent des suites exactes de complexes, dites canoniques

(I) $0 \to Z(C) \to C \xrightarrow{\delta} B(C) (-1) \to 0$,
(II) $0 \to B(C) \to Z(C) \to H(C) \to 0$,
(III) $0 \to B(C) \to C \to C/B(C) \to 0$,
(IV) $0 \to H(C) \to C/B(C) \xrightarrow{\delta} B(C) (-1) \to 0$,
(V) $0 \to H(C) \to C/B(C) \to Z(C) (-1) \to H(C) (-1) \to 0$.

On définit de même les notions de somme directe de complexes, système inductif de complexes, limite inductive d’un système inductif de complexes.

Soit $(C_i, d_i)$ une famille de complexes. On appelle produit de cette famille et on note $\prod_{i \in I} (C_i, d_i)$ le complexe $(C, d)$ obtenu comme suit :

a) pour chaque $n \in \mathbf{Z}$, $C_n$ est le A-module produit $\prod_{i \in I} (C_i)_n$ des composantes homogènes $(C_i)_n$ des complexes donnés,
b) pour chaque $n \in \mathbf{Z}$, $d_n : C_n \to C_{n-1}$ est le A-homomorphisme de composantes $(d_i)_n$.

Lorsque I est fini, $\prod_{i \in I} (C_i, d_i)$ est égal à $\bigoplus_{i \in I} (C_i, d_i)$. On prendra garde qu’en général, le A-module sous-jacent au complexe produit $\prod_{i \in I} (C_i, d_i)$ n’est pas le A-module produit $\prod_{i \in I} C_i$.

Considérons une famille (resp. un système inductif filtrant) $(C_i)_{i \in I}$ de complexes. Soit C la somme directe (resp. la limite inductive) des $C_i$, et soient $\alpha_i : C_i \to C$ les homomorphismes canoniques. Alors les $H(\alpha_i) : H(C_i) \to H(C)$ définissent un homomorphisme gradué de degré 0, dit canonique, de $\bigoplus_{i \in I} H(C_i)$ (resp. $\varprojlim_{i \in I} H(C_i)$) dans $H(C)$. De même, les projections canoniques $\prod_{i \in I} C_i \to C_i$ définissent un homomorphisme gradué de degré 0, dit canonique, de $H(\prod_{i \in I} C_i)$ dans $\prod_{i \in I} (H(C_i))$.

#### Proposition 1 {#alg-x-s2-prop-1 .statement}

Pour toute famille de complexes $(C_i)_{i \in I}$, les homomorphismes canoniques
$$
\bigoplus_{i \in I} H(C_i) \to H(\bigoplus_{i \in I} C_i), \quad H(\prod_{i \in I} C_i) \to \prod_{i \in I} H(C_i)
$$
sont bijectifs.

Pour tout système inductif filtrant de complexes $(C_i)_{i \in I}$, l’homomorphisme canonique
$$
\varprojlim_{i \in I} H(C_i) \to H(\varprojlim_{i \in I} C_i)
$$
est bijectif.

Cela résulte aussitôt de II, p. 14, cor. 1 à la prop. 7, p. 11, cor. à la prop. 5, et p. 91, prop. 3.

### 3. L’homomorphisme de liaison et la suite exacte d’homologie

Dans ce numéro, on considère une suite exacte de complexes
$$
0 \longrightarrow C' \xrightarrow{u} C \xrightarrow{v} C'' \longrightarrow 0 ;
$$
notons par la même lettre $d$ les différentielles de $C, C'$ et $C''$.

Soit $\Gamma$ l’ensemble des $x \in C$ tels que $dx \in \operatorname{Im}(u)$; pour $x \in \Gamma$, on a
$$
d(\bar{u}^{-1}(dx)) = \bar{u}^{-1}(dd(x)) = 0 ,
$$
donc $\bar{u}^{-1}(dx) \in Z(C')$; on a aussi $dv(x) = v(dx) \in \operatorname{Im}(v \circ u) = 0$, donc $v(x) \in Z(C'')$; considérons alors l’application linéaire $\varphi : \Gamma \to H(C'') \times H(C')$ qui applique tout élément $x \in \Gamma$ sur la classe de $(v(x), \bar{u}^{-1}(dx))$.

#### Lemme 1 {#alg-x-s2-lem-1 .statement}

L’image $\varphi(\Gamma)$ de $\Gamma$ dans $H(C'') \times H(C')$ est le graphe d’un A-homomorphisme gradué de degré $-1$ de $H(C'')$ dans $H(C')$.

a) Si $x \in \Gamma$ et si $v(x) \in B(C'')$, alors $\bar{u}^{-1}(dx) \in B(C')$ : il existe en effet $z'' \in C''$ tel que $v(x) = dz''$, puis $z \in C$ tel que $z'' = v(z)$, donc $v(x) = v(dz)$, puis $t' \in C'$ tel que $x - dz = u(t')$, ce qui donne $dx = u(dt')$, donc $\bar{u}^{-1}(dx) = dt' \in B(C')$.

b) Tout élément de $Z(C'')$ est l’image par $v$ d’un élément $x$ de $C$ tel que $v(dx) = 0$, i.e. $dx \in \operatorname{Im} u$, c’est-à-dire tel que $x \in \Gamma$.

c) Il résulte de a) et b) que $\varphi(\Gamma)$ est bien un graphe fonctionnel ; comme $\varphi$ est bihomogène de bidegré $(0, -1)$, cela achève la démonstration.

L’homomorphisme gradué de degré $-1$ de $H(C'')$ dans $H(C')$ ainsi défini s’appelle l’homomorphisme de liaison relatif à la suite exacte $(u, v)$; on le note $\partial(u, v)$ ou $\partial_{u,v}$ ou simplement $\partial$. Ses composantes homogènes sont notées
$$
\partial_n(u, v) : H_n(C'') \to H_{n-1}(C') \quad \text{et} \quad \partial^n(u, v) : H^n(C'') \to H^{n+1}(C') .
$$

Par définition, pour construire l’image d’une classe $\alpha \in H_n(C'')$ par $\partial$, on choisit un cycle $z'' \in Z_n(C'')$ dans la classe $\alpha$, puis un élément $x$ de $C_n$ tel que $v(x) = z''$; alors $dx$ est de la forme $u(t')$, $t' \in C'_{n-1}$, et $\partial(\alpha)$ est la classe d’homologie de $t'$.

En termes de correspondances, $\partial_n(u, v)$ s’obtient donc à partir de la correspondance $\bar{u}_{n-1}^{-1} \circ d_n \circ \bar{v}_n^{-1}$ entre $C''_n$ et $C'_{n-1}$, par passage aux sous-ensembles $Z_n(C'')$ et $Z_{n-1}(C')$, puis à leurs quotients $H_n(C'')$ et $H_{n-1}(C')$. Cela montre notamment que, si on remplace $C, C', C'', u, v$ par $C(p), C'(p), C''(p), u(p), v(p)$, on a
$$
\partial(u(p), v(p)) = (-1)^p \partial(u, v) ;
$$
de même, si $\lambda$ et $\mu$ sont deux éléments inversibles du centre de $A$, on a
$$
\partial(\lambda u, \mu v) = \lambda^{-1} \mu^{-1} \partial(u, v) .
$$

On peut aussi relier $\partial(u, v)$ au diagramme du serpent (X, p. 4). D’après loc. cit., prop. 2, les suites
$$
0 \longrightarrow Z_n(C') \xrightarrow{Z_n(u)} Z_n(C) \xrightarrow{Z_n(v)} Z_n(C'')
$$

et

$$
C'_n/B_n(C') \xrightarrow{\overline{u}_n} C_n/B_n(C) \xrightarrow{\overline{v}_n} C''_n/B_n(C'') \longrightarrow 0 ,
$$

où $\overline{u}_n$ et $\overline{v}_n$ sont déduits de $u$ et $v$, sont exactes. Utilisant les suites exactes canoniques $(V_n)$, on obtient un *diagramme commutatif* à lignes et colonnes exactes

$$
\begin{array}{ccccccccc}
&&0&&0&&0&&\\
&&\downarrow&&\downarrow&&\downarrow&&\\
&&H_n(C')&\xrightarrow{H_n(u)}&H_n(C)&\xrightarrow{H_n(v)}&H_n(C'')&&\\
&&\downarrow&&\downarrow&&\downarrow&&\\
0&\longrightarrow&C'_n/B_n(C')&\xrightarrow{\overline{u}_n}&C_n/B_n(C)&\xrightarrow{\overline{v}_n}&C''_n/B_n(C'')&\longrightarrow&0\\
&&\downarrow&&\downarrow&&\downarrow&&\\
0&\longrightarrow&Z_{n-1}(C')&\xrightarrow{Z_{n-1}(u)}&Z_{n-1}(C)&\xrightarrow{Z_{n-1}(v)}&Z_{n-1}(C'')&&\\
&&\downarrow&&\downarrow&&\downarrow&&\\
&&H_{n-1}(C')&\xrightarrow{H_{n-1}(u)}&H_{n-1}(C)&\xrightarrow{H_{n-1}(v)}&H_{n-1}(C'')&&\\
&&\downarrow&&\downarrow&&\downarrow&&\\
&&0&&0&&0&&
\end{array}
$$

L’homomorphisme $H_n(C'')\to H_{n-1}(C')$ associé à ce diagramme (loc. cit., prop. 2, (iii)) coïncide par construction avec $\partial_n(u,v)$. Cela entraîne en outre que la suite d’homomorphismes $(H_n(u),\ H_n(v),\ \partial_n(u,v),\ H_{n-1}(u),\ H_{n-1}(v))$ est exacte ; par conséquent :

#### Théorème 1 {#alg-x-s2-thm-1 .statement}

*La suite illimitée d’homomorphismes de* $A$-*modules*

$$
\cdots \longrightarrow H_{n+1}(C'') \xrightarrow{\partial_{n+1}(u,v)} H_n(C') \xrightarrow{H_n(u)} H_n(C) \xrightarrow{H_n(v)} H_n(C'')
$$

$$
\xrightarrow{\partial_n(u,v)} H_{n-1}(C') \xrightarrow{H_{n-1}(u)} H_{n-1}(C) \xrightarrow{H_{n-1}(v)} H_{n-1}(C'') \xrightarrow{\partial_{n-1}(u,v)} H_{n-2}(C') \longrightarrow \cdots
$$

*est exacte.*

Cette suite s’appelle la *suite exacte d’homologie* associée à la suite exacte $(u,v)$ ; on l’écrit parfois sous la forme d’un *triangle exact de* $A$-*modules*

$$
\begin{array}{ccc}
&&H(C)\\
&\nearrow^{H(u)}&\searrow^{H(v)}\\
H(C')&\xleftarrow{\partial(u,v)}&H(C'') .
\end{array}
$$

#### Corollaire 1 {#alg-x-s2-thm-1-cor-1 .statement}

*Si deux des complexes* $C$, $C'$, $C''$ *sont d’homologie nulle, le troisième l’est aussi. Pour que* $u$ *(resp.* $v$*) soit un homomorphisme, il faut et il suffit que* $C''$ *(resp.* $C'$*) soit d’homologie nulle. Pour que* $\partial(u,v)$ *soit bijectif, il faut et il suffit que* $C$ *soit d’homologie nulle.*

#### Corollaire 2 {#alg-x-s2-thm-1-cor-2 .statement}

Soit u un morphisme de complexes. Si Ker u et Coker u sont d’homologie nulle, alors u est un homologisme.

En effet, soit u : E → E’ un morphisme de complexes. Si Ker u (resp. Coker u) est d’homologie nulle, alors le morphisme canonique E → Im u (resp. Im u → E’) est un homologisme d’après le corollaire 1.

#### Proposition 2 {#alg-x-s2-prop-2 .statement}

Considérons un diagramme commutatif de complexes à lignes exactes

$$
\begin{array}{ccccccccc}
0 & \longrightarrow & C' & \xrightarrow{u} & C & \xrightarrow{v} & C'' & \longrightarrow & 0 \\
& & f' \downarrow & & f \downarrow & & f'' \downarrow & & \\
0 & \longrightarrow & C'_1 & \xrightarrow{u_1} & C_1 & \xrightarrow{v_1} & C''_1 & \longrightarrow & 0 .
\end{array}
$$

Alors $\mathrm{H}(f') \circ \partial(u, v) = \partial(u_1, v_1) \circ \mathrm{H}(f'')$.

Soit $\alpha'' \in \mathrm{H}(C'')$; soient $z''$ un cycle de classe $\alpha''$ et $x$ un élément de $C$ tel que $v(x) = z''$; on a

$$
(\partial_{u_1, v_1} \circ \mathrm{H}(f'')) (\alpha'') = \partial_{u_1, v_1}(\overline{f''(z'')}) = \overline{u_1^{-1}(df(x))} = \overline{f'(u_1^{-1}(dx))} =
= \mathrm{H}(f') (\overline{u^{-1}(dx)}) = (\mathrm{H}(f') \circ \partial_{u, v}) (\alpha'') .
$$

#### Exemple {#alg-x-s2-n3-exa-1 .statement}

Soit C un complexe. Considérons la suite exacte canonique

(I)
$$
0 \longrightarrow Z(C) \xrightarrow{j} C \xrightarrow{\delta} B(C) (-1) \longrightarrow 0 ,
$$
et soit $i : B(C) \to Z(C)$ l’injection canonique. Alors l’homomorphisme de liaison $\partial(j, \delta) : \mathrm{H}(B(C)) (-1) \to \mathrm{H}(Z(C)) (-1)$ s’identifie à $\mathrm{H}(i) (-1)$, comme on le vérifie aussitôt. Comme $\mathrm{H}(\delta) = 0$, la suite exacte d’homologie associée à (I) se décompose en les suites exactes courtes

(II_n)
$$
0 \longrightarrow B_n(C) \xrightarrow{i} Z_n(C) \xrightarrow{\mathrm{H}(j)} H_n(C) \longrightarrow 0 .
$$

\* Applications :

1) Homologie singulière

Soit A un anneau. Pour tout espace topologique X, on définit le complexe singulier $C(X, A)$ de X à coefficients dans A de la façon suivante :

Dans $\mathbf{R}^{(N)}$, notons $(e_n)$ la base canonique ; on appelle n-simplexe canonique l’enveloppe convexe $\Delta_n$ de $\{ e_0, ..., e_n \}$. Pour $i \in \{ 0, ..., n \}$, on définit l’application affine $\iota_i : \Delta_{n-1} \to \Delta_n$ par $\iota_i(e_k) = e_k$ pour $k < i$ et $\iota_i(e_k) = e_{k+1}$ pour $k \geq i$. On note $C_n(X, A)$ le A-module $A^{(\Sigma_n(X))}$, où $\Sigma_n(X)$ est l’ensemble des applications continues de $\Delta_n$ dans X ; pour $n < 0$, on pose $C_n = 0$. Pour $i \in \{ 0, ..., n \}$, on définit l’application linéaire $\partial_{n, i} : C_n(X, A) \to C_{n-1}(X, A)$ par $\partial_{n, i}(e_s) = e_{s \circ \iota_i}$ pour $s \in \Sigma_n(X)$, et on pose $d_n = \Sigma (-1)^i \partial_{n, i}$. On vérifie que

$$
... C_n(X, A) \xrightarrow{d_n} C_{n-1}(X, A) \to ...
$$

est un complexe. Son homologie est appelée l’homologie singulière de X à coefficients dans A et se note $\mathrm{H}(X, A)$ ou simplement $\mathrm{H}(X)$.

Si Y est un sous-espace de X, on note $C(X, Y, A)$ le complexe quotient $C(X, A)/C(Y, A)$, et $\mathrm{H}(X, Y, A)$ son homologie. Il résulte du théorème 1 que l’on a une suite exacte :

$$
... \to \mathrm{H}_n(Y, A) \to \mathrm{H}_n(X, A) \to \mathrm{H}_n(X, Y, A) \to \mathrm{H}_{n-1}(Y, A) \to \mathrm{H}_{n-1}(X, A) \to ...
$$

2) Complexes cellulaires finis

Soit X un espace topologique séparé. Une décomposition cellulaire finie de X est donnée par une suite croissante $(X_n)_{n \in \mathbf{Z}}$ de sous-espaces fermés de X satisfaisant aux conditions suivantes :
(i) $X_n = \varnothing$ pour $n < 0$;
(ii) il existe un N tel que $X_N = X$ (donc $X_n = X$ pour $n > N$);
(iii) pour tout n, l’espace $X_n - X_{n-1}$ n’a qu’un nombre fini de composantes connexes, appelées cellules de dimension n;
(iv) pour tout n, et pour toute composante connexe C de $X_n - X_{n-1}$, il existe un homéomorphisme de la boule euclidienne ouverte $\hat{B}_n$ de dimension n (TG, VI, p. 10) sur C qui se prolonge en une application continue de la boule fermée dans X.

On peut montrer que ces conditions entraînent que $H_n(X_n, X_{n-1}, A)$ est un A-module libre $\Gamma_n$ de rang égal au nombre de cellules de dimension n, et que $H_i(X_n, X_{n-1}, A) = 0$ pour $i \neq n$. On a $C(X_n, X_{n-1}, A) = C(X_n, X_{n-2}, A)/C(X_{n-1}, X_{n-2}, A)$, d’où une suite exacte

$$
H_n(X_n, X_{n-2}) \longrightarrow H_n(X_n, X_{n-1}) \xrightarrow{d_n} H_{n-1}(X_{n-1}, X_{n-2}) \longrightarrow H_{n-1}(X_n, X_{n-2}) ,
$$

comportant un homomorphisme de liaison $d_n : \Gamma_n \to \Gamma_{n-1}$. On a $d_n \circ d_{n+1} = 0$, ce qui permet de définir un complexe $\Gamma : \cdots \to \Gamma_n \xrightarrow{d_n} \Gamma_{n-1} \to \cdots$.

La suite exacte

$$
H_{n+1}(X_p, X_{p-1}) \to H_n(X_{p-1}) \to H_n(X_p) \to H_n(X_p, X_{p-1}) \to H_{n-1}(X_{p-1})
$$

montre par récurrence sur p que $H_n(X_p) = 0$ pour $p < n$, que $H_n(X_n) = \mathrm{Ker}\,(d_n : \Gamma_n \to \Gamma_{n-1})$ et que $H_n(X_p) = H_n(\Gamma)$ pour $p > n$. En particulier $H_n(X)$ s’identifie à $H_n(\Gamma)$.

#### Exemple {#alg-x-s2-n3-exa-2 .statement}

Considérons le produit de sphères $S_2 \times S_2$ et l’espace projectif complexe $P_2(\mathbf{C})$.
Soit $b \in S_2$, on définit une décomposition cellulaire $(Y_n)$ de $Y = S_2 \times S_2$ en posant

$$
Y_0 = Y_1 = \{ (b, b) \} , \quad Y_2 = Y_3 = (\{ b \} \times S_2) \cup (S_2 \times \{ b \}) \quad \text{et} \quad Y_4 = S_2 \times S_2 ;
$$

cette décomposition comporte une cellule de dimension 0, deux de dimension 2 et une de dimension 4. Les différentielles du complexe associé sont nécessairement nulles, donc $H_0(Y)$, $H_2(Y)$ et $H_4(Y)$ sont libres de rang 1, 2 et 1 respectivement, et $H_n(Y) = 0$ pour $n \notin \{ 0, 2, 4 \}$.
On obtient une décomposition cellulaire $(Z_n)$ de $P_2(\mathbf{C})$ en posant

$$
Z_0 = Z_1 = \{ c \} , \quad Z_2 = Z_3 = P_1(\mathbf{C}) , \quad Z_4 = P_2(\mathbf{C}) ,
$$

l’espace $P_1(\mathbf{C})$ étant plongé dans $P_2(\mathbf{C})$ (TG, VIII, p. 20), et c étant un point de $P_1(\mathbf{C})$; cette décomposition comporte une cellule de dimension 0, une de dimension 2 et une de dimension 4. Ici encore les différentielles du complexe sont nécessairement nulles, et il en résulte que $H_n(P_2(\mathbf{C}))$ est isomorphe à A pour $n \in \{ 0, 2, 4 \}$ et à 0 sinon.
Comme les modules d’homologie en degré 2 des deux espaces considérés sont libres de rang 2 et 1 respectivement, ces espaces ne sont pas homéomorphes. \*

### 4. Homotopies

#### Définition 4 {#alg-x-s2-def-4 .statement}

Soient $(C, d)$ et $(C', d')$ deux complexes, $f$ et $g$ deux morphismes de C dans $C'$. On appelle homotopie reliant $f$ à $g$ tout A-homomorphisme gradué s de degré 1 de C dans $C'$ tel que $g - f = d' \circ s + s \circ d$.
On dit que $f$ et $g$ sont homotopes, s’il existe une homotopie reliant $f$ à $g$.
Si $h$ est un troisième morphisme de C dans $C'$ et si $s$ (resp. $t$) est une homotopie reliant $f$ à $g$ (resp. $g$ à $h$), alors $s + t$ est une homotopie reliant $f$ à $h$; par suite, la relation « $f$ et $g$ sont deux morphismes homotopes de $C$ dans $C'$ » est une relation d’équivalence, dont les classes sont appelées les *classes d’homotopie de morphismes de $C$ dans $C'$*.

\* Etant donnés deux espaces topologiques $X$ et $Y$, et une application continue $f : X \to Y$, on définit une application linéaire $f_*$ du complexe singulier (*cf. n° 3*) $C(X, A)$ dans $C(Y, A)$ en posant $f_*(e_s) = e_{f \circ s}$ pour $s \in \Sigma_n(X)$. Cette application est un morphisme de complexes.
Deux applications continues $f$ et $g$ de $X$ dans $Y$ sont dites topologiquement *homotopes* s’il existe une application continue $h$ de $[0, 1] \times X$ dans $Y$ telle que $h(0, x) = f(x)$ et $h(1, x) = g(x)$ pour tout $x \in X$. On montre que, si $f$ et $g$ sont topologiquement homotopes, les morphismes $f_*$ et $g_*$ sont homotopes au sens de la définition 4 ci-dessus. C’est ce fait qui est à l’origine de la terminologie utilisée en algèbre. \*

#### Proposition 3 {#alg-x-s2-prop-3 .statement}

*Si $f$ et $g$ sont deux morphismes homotopes de $C$ dans $C'$, alors $\mathrm{H}(f) = \mathrm{H}(g)$.* Soit $s$ une homotopie reliant $f$ à $g$. On a
$$
(g - f)(\mathbf{Z}(C)) = (d' \circ s + s \circ d)(\mathbf{Z}(C)) = (d' \circ s)(\mathbf{Z}(C)) \subset \mathbf{B}(C') ,
$$
donc $\mathrm{H}(g - f) = 0$ et $\mathrm{H}(g) = \mathrm{H}(f)$.

#### Corollaire {#alg-x-s2-n4-cor-1 .statement}

*Un morphisme homotope à un homologisme est un homologisme.*

#### Proposition 4 {#alg-x-s2-prop-4 .statement}

*Soient $C, C', D, D'$ quatre complexes, $f : C \to C'$, $g : C \to C'$, $u : D \to C$, $v : C' \to D'$ quatre morphismes. Si $s$ est une homotopie reliant $f$ à $g$, alors $v \circ s \circ u$ est une homotopie reliant $v \circ f \circ u$ à $v \circ g \circ u$. Si $f$ et $g$ sont homotopes, $v \circ f \circ u$ et $v \circ g \circ u$ le sont aussi.*
C’est clair.

#### Corollaire {#alg-x-s2-n4-cor-2 .statement}

*Soient $C, C', C''$ trois complexes, $f$ et $g$ deux morphismes de $C$ dans $C'$, $f_1$ et $g_1$ deux morphismes de $C'$ dans $C''$. Si $s$ et $s_1$ sont des homotopies reliant $f$ à $g$ et $f_1$ à $g_1$ respectivement, alors $s_1 \circ f + g_1 \circ s$ est une homotopie reliant $f_1 \circ f$ à $g_1 \circ g$. Si $f$ et $f_1$ sont homotopes à $g$ et $g_1$ respectivement, alors $f_1 \circ f$ est homotope à $g_1 \circ g$.
En effet, $s_1 \circ f$ relie $f_1 \circ f$ à $g_1 \circ f$ et $g_1 \circ s$ relie $g_1 \circ f$ à $g_1 \circ g$.

#### Définition 5 {#alg-x-s2-def-5 .statement}

*Un morphisme de complexes $f : C \to C'$ est appelé un homotopisme s’il existe un morphisme $f' : C' \to C$ tel que $f' \circ f$ et $f \circ f'$ soient homotopes à $1_C$ et $1_{C'}$ respectivement.*
Il est clair que $f'$ est alors aussi un homotopisme ; on dit aussi que $f'$ est *réciproque de $f$ à homotopie près*. Si $f'$ et $f'_1$ sont tous deux réciproques de $f$ à homotopie près, alors $f'$ et $f'_1$ sont homotopes (en effet d’après le corollaire précédent, $f'_1 = f'_1 \circ 1_{C'}$ est homotope à $f'_1 \circ f \circ f'$, donc à $1_C \circ f' = f'$).

#### Proposition 5 {#alg-x-s2-prop-5 .statement}

*Un homotopisme est un homologisme ; un morphisme composé d’homotopismes est un homotopisme. Un morphisme homotope à un homotopisme est un homotopisme.*
Soient $f : C \to C'$ et $f_1 : C' \to C''$ des homotopismes de complexes, $f' : C' \to C$ et $f'_1 : C'' \to C'$ des morphismes réciproques à homotopie près. On a
$$
\mathrm{H}(f') \circ \mathrm{H}(f) = \mathrm{H}(f' \circ f) = \mathrm{H}(1_C) = 1_{\mathrm{H}(C)} \quad (\text{prop. 3})
$$

et de même $\mathrm{H}(f) \circ \mathrm{H}(f') = 1_{\mathrm{H}(C')}$, donc $\mathrm{H}(f)$ est bijectif et $f$ est un homologisme. D’autre part, $(f' \circ f'_1) \circ (f_1 \circ f)$ est homotope à $f' \circ 1_C' \circ f$ (prop. 4), donc à $1_C$; de même, $(f_1 \circ f) \circ (f' \circ f'_1)$ est homotope à $1_{C''}$ et $f_1 \circ f$ est un homotopisme. Enfin, si $g : C \to C'$ est un morphisme homotope à $f$, $f' \circ g$ est homotope à $f' \circ f$, donc à $1_C$; de même, $g \circ f'$ est homotope à $f \circ f'$, donc à $1_{C'}$ et $g$ est un homotopisme.

#### Corollaire {#alg-x-s2-n4-cor-3 .statement}

Soient $C, C', D, D'$ quatre complexes, $f : C \to C'$ un morphisme, $u : D \to C$ et $v : C' \to D'$ des homotopismes. Pour que $v \circ f \circ u$ soit un homotopisme (resp. un homologisme), il faut et il suffit que $f$ en soit un.

Si $f$ est un homotopisme (resp. un homologisme), alors $v \circ f \circ u$ est composé d’homotopismes (resp. d’homologismes), donc en est un. Inversement, soit $\overline{u}$ et $\overline{v}$ des morphismes réciproques de $u$ et $v$ à homotopie près ; alors $\overline{v} \circ (v \circ f \circ u) \circ \overline{u}$ est homotope à $f$ d’après la prop. 4 ; d’où la conclusion d’après la prop. 5, et le corollaire de la prop. 3.

On dit que le complexe $C$ est homotope à zéro si $1_C$ est homotope à l’application nulle, c’est-à-dire s’il existe un $A$-endomorphisme gradué $s$ de degré 1 de $C$ tel que $1_C = s \circ d + d \circ s$. Cela revient aussi à dire que l’unique morphisme $0 \to C$ (resp. $C \to 0$) est un homotopisme. Un complexe homotope à zéro est d’homologie nulle (prop. 5).

#### Exemple {#alg-x-s2-n4-exa-1 .statement}

Soient $u : M \to N$ et $v : N \to P$ des homomorphismes de $A$-modules tels que $v \circ u = 0$ ; soit $C$ le complexe tel que $C_2 = M, C_1 = N, C_0 = P, C_i = 0$ pour $i \neq 0, 1, 2$, $d_2 = u, d_1 = v, d_i = 0$ pour $i \neq 1, 2$. Alors $C$ est d’homologie nulle si et seulement si la suite $0 \to M \xrightarrow{u} N \xrightarrow{v} P \to 0$ est exacte. Il est homotope à zéro si et seulement si cette suite est scindée. En effet, dire que $C$ est homotope à zéro signifie qu’il existe des $A$-homomorphismes $s : P \to N$ et $t : N \to M$ tels que $v \circ s = 1_P, s \circ v + u \circ t = 1_N, t \circ u = 1_M$ ; cela implique que la suite est scindée ; inversement si $s$ est une section $A$-linéaire de $v$, on définit $t$ par $u \circ t = 1_N - s \circ v$, ce qui est possible puisque $v \circ (1_N - s \circ v) = v - v \circ s \circ v = 0$.

### 5. Complexes scindés

#### Proposition 6 {#alg-x-s2-prop-6 .statement}

Soit $(C, d)$ un complexe. Les conditions suivantes sont équivalentes :
(i) il existe un homotopisme de $(C, d)$ sur $(\mathrm{H}(C), 0)$ ;
(ii) il existe un $A$-endomorphisme $s$ de $C$, gradué de degré 1, tel que $d = d \circ s \circ d$ ;
(iii) $B(C)$ et $Z(C)$ sont des sous-modules facteurs directs de $C$ ;
(iv) $(C, d)$ est somme directe de sous-complexes qui sont soit de longueur 0, soit de longueur 1 et d’homologie nulle.

(i) $\Rightarrow$ (ii) : soit $\varphi : C \to \mathrm{H}(C)$ un homotopisme ; il existe alors un morphisme de complexes $\psi : \mathrm{H}(C) \to C$ et un endomorphisme $s$ de $C$, gradué de degré 1 tel que $\psi \circ \varphi = 1_C - s \circ d - d \circ s$. On a $d \circ \psi = \psi \circ 0 = 0$, donc
$$
0 = d \circ \psi \circ \varphi = d - d \circ s \circ d - d \circ d \circ s = d - d \circ s \circ d ,
$$
d’où (ii) .

$(ii) \Rightarrow (iii)$ : soit $s$ comme dans (ii). Alors $d \circ (1_C-s\circ d)=0$, donc $1_C-s\circ d$ est un projecteur de $C$ sur $Z(C)$, et $(d\circ s)\circ d=d$, donc $d\circ s$ est un projecteur de $C$ sur $B(C)$.

$(iii) \Rightarrow (iv)$ : pour chaque $n\in\mathbf{Z}$, posons $Z_n=Z_n(C)$, $B_n=B_n(C)$ et choisissons des sous-modules $K_n$ et $B'_n$ de $C_n$ tels que $C_n=B'_n\oplus Z_n$, $Z_n=K_n\oplus B_n$. Alors

$$
E_{(n)}=K_n(-n)\quad\text{et}\quad F_{(n)}=B'_n(-n)\oplus B_{n-1}(1-n)
$$

sont des sous-complexes de $(C,d)$ ; on a

$$
(C,d)=\bigoplus_{n\in\mathbf{Z}}(E_{(n)}\oplus F_{(n)})
$$

; chaque $E_{(n)}$ est, soit nul, soit de longueur $0$, chaque $F_{(n)}$ est soit nul, soit de longueur $1$ et d’homologie nulle, d’où (iv).

$(iv) \Rightarrow (i)$ : il suffit de remarquer que (i) est satisfait lorsque $C$ est de longueur zéro, ou d’homologie nulle et de longueur 1.

#### Définition 6 {#alg-x-s2-def-6 .statement}

*Un complexe $C$ est dit scindé s’il satisfait aux conditions équivalentes de la prop. 6.*

Un endomorphisme $s$ de $C$ satisfaisant à la condition (ii) de la prop. 6 est appelé une *scission* de $C$.

#### Exemple 1 {#alg-x-s2-n5-exa-1 .statement}

Un complexe à différentielle nulle est scindé.

#### Exemple 2 {#alg-x-s2-n5-exa-2 .statement}

Les complexes homotopes à zéro sont les complexes scindés d’homologie nulle, *i.e.* les complexes $C$ tels que $H(C)=0$ et que $Z(C)$ soit facteur direct dans $C$.

#### Exemple 3 {#alg-x-s2-n5-exa-3 .statement}

Soient $f:M\to N$ un homomorphisme de A-modules et $C$ le complexe tel que $C_1=M$, $C_0=N$, $C_i=0$ pour $i\ne0,1$, $d_1=f$, $d_i=0$ pour $i\ne1$. Alors $C$ est scindé si et seulement si $\operatorname{Ker}f$ est facteur direct dans $M$ et $\operatorname{Im}f$ facteur direct dans $N$.

#### Exemple 4 {#alg-x-s2-n5-exa-4 .statement}

*Le complexe $C$ est scindé dès que $B(C)$ et $H(C)$ sont projectifs (resp. dès que $B_n(C)$ et $H_n(C)$ sont injectifs pour chaque $n$).* En effet, d’après les suites exactes $(I_n)$ à $(IV_n)$ du n° 1, $Z(C)$ est alors facteur direct dans $C$ et $B(C)$ facteur direct de $Z(C)$ (resp. $B(C)$ est facteur direct dans $C$ et $Z(C)/B(C)$ facteur direct dans $C/B(C)$).

#### Exemple 5 {#alg-x-s2-n5-exa-5 .statement}

En particulier, si A est principal, un complexe libre $C$ est scindé si et seulement si $H(C)$ est libre (c’est-à-dire $H_n(C)$ libre pour tout $n\in\mathbf{Z}$).

#### Remarque {#alg-x-s2-n5-rem-1 .statement}

a) Supposons que la suite exacte canonique de A-modules gradués

$$
\tag{II}
0\longrightarrow B(C)\longrightarrow Z(C)\xrightarrow{\pi}H(C)\longrightarrow0
$$

soit *scindée* (cela a lieu par exemple si $H(C)$ est projectif, ou $B_n(C)$ injectif pour chaque $n$) ; soit $\sigma:H(C)\to Z(C)$ une section A-linéaire graduée de $\pi$, et soit $\psi$ l’homomorphisme $x\mapsto\sigma(x)$ de $H(C)$ dans $C$. Alors $\psi$ est un *homologisme* de $(H(C),0)$ dans $C$, tel que

$$
H(\psi)=1_{H(C)}.
$$

b) Supposons que la suite exacte canonique de A-modules gradués

$$
\tag{IV}
0\longrightarrow H(C)\xrightarrow{i}C/B(C)\longrightarrow B(C)(-1)\longrightarrow0
$$

soit *scindée* (cela a lieu par exemple si $B(C)$ est projectif, ou $H_n(C)$ injectif pour chaque $n$); soit $\tau : C/B(C) \to H(C)$ une rétraction A-linéaire graduée de $i$ et $\varphi$ l’homomorphisme de $C$ dans $H(C)$ qui associe à chaque élément de $C$ l’image par $\tau$ de sa classe modulo $B(C)$. Alors $\varphi$ est un *homologisme de $C$ dans $(H(C), 0)$ tel que* $H(\varphi) = 1_{H(C)}$.

### 6. Cône et cylindre d’un morphisme de complexes

Soit $u : (C', d') \to (C, d)$ un morphisme de complexes. Soient $\mathrm{Cyl}\,(u)$ et $\mathrm{Con}\,(u)$ les A-modules gradués $\mathrm{Cyl}\,(u) = C' \oplus C'(-1) \oplus C$, $\mathrm{Con}\,(u) = C'(-1) \oplus C$, et définissons des applications A-linéaires graduées de degré $(-1)$

$$
\overline{D} : \mathrm{Cyl}\,(u) \to \mathrm{Cyl}\,(u) , \quad \overline{D}(x', y', x) = (d'x' + y', -d'y', dx - u(y')),
$$
$$
D : \mathrm{Con}\,(u) \to \mathrm{Con}\,(u) , \quad D(y', x) = (-d'y', dx - u(y')) .
$$

(Ici, et dans la suite, on note $x, y, \ldots$ des éléments arbitraires de $C$, $x', y', \ldots$ des éléments arbitraires de $C'$.)

#### Lemme 2 {#alg-x-s2-lem-2 .statement}

(*Cyl* $(u)$, $\overline{D}$) *et* (*Con* $(u)$, $D$) *sont des complexes de A-modules*.

En effet, on a
$$
\overline{D} \circ \overline{D}(x', y', x) = \overline{D}(d'x' + y', -d'y', dx - u(y')) =
$$
$$
= (d'(d'x' + y') - d'y', -d'(-d'y'), d(dx - u(y')) - u(-d'y')) = 0
$$
puisque $d' \circ d' = 0$, $d \circ d = 0$ et $d \circ u = u \circ d'$. De même $D \circ D = 0$.

#### Définition 7 {#alg-x-s2-def-7 .statement}

*Les complexes* $\mathrm{Cyl}\,(u)$ *et* $\mathrm{Con}\,(u)$ *sont appelés respectivement le cylindre* *et le cône du morphisme* $u$.

#### Exemple {#alg-x-s2-n6-exa-1 .statement}

Soit $u : M \to N$ un homomorphisme de A-modules ; alors les seules composantes homogènes non nulles de $\mathrm{Cyl}\,(u)$ et $\mathrm{Con}\,(u)$ sont
$$
\mathrm{Cyl}_1\,(u) = M , \qquad \mathrm{Cyl}_0\,(u) = M \oplus N ,
$$
$$
\mathrm{Con}_1\,(u) = M , \qquad \mathrm{Con}_0\,(u) = N ,
$$
et on a $\overline{D}(m) = (m, -u(m))$, $D(m) = -u(m)$ pour $m \in M$; par conséquent,
$$
H_1(\mathrm{Con}\,(u)) = \mathrm{Ker}\,(u) , \quad H_0(\mathrm{Con}\,(u)) = \mathrm{Coker}\,(u) .
$$

*Soient* $X$ *et* $Y$ *deux espaces topologiques et* $f$ *une application continue de* $X$ *dans* $Y$. On appelle *cylindre* de $f$ l’espace quotient $\mathrm{Cyl}\,(f)$ de la somme topologique de $[0, 1] \times X$ et $Y$ par la relation d’équivalence identifiant le point $(1, x)$ de $[0, 1] \times X$ au point $f(x)$ de $Y$ pour tout $x \in X$. On appelle *cône* de $f$ l’espace quotient $\mathrm{Con}\,(f)$ de la somme topologique d’un espace réduit à un point $s$ et de $\mathrm{Cyl}\,(f)$ par la relation d’équivalence identifiant $s$ à l’image de $(0, x)$ pour tout $x \in X$ : on note encore $s$ l’image de $s$ dans $\mathrm{Con}\,(f)$.

Supposons $X$ et $Y$ munis de décompositions cellulaires $(X_n)$ et $(Y_n)$ (*cf.* n° 3), et supposons $f(X_n) \subset Y_n$ pour tout $n$. On obtient une décomposition cellulaire $(S_n)$ de $\mathrm{Cyl}\,(f)$ (resp. de $\mathrm{Con}\,(f)$) en prenant pour $S_n$ l’image de $(\{0\} \times X_n) \cup ([0, 1] \times X_{n-1}) \cup Y_n$
$$
(\text{resp. de } \{s\} \cup ([0, 1] \times X_{n-1}) \cup Y_n , \quad \text{si } n \geqslant 0) .
$$
Notons $\Gamma(X), \Gamma(Y), \Gamma(\mathrm{Cyl}\,(f)), \Gamma(\mathrm{Con}\,(f))$ les complexes associés à ces décompositions cellulaires.

Le complexe $\Gamma(s)$ associé à l’espace $\{ s \}$ muni de son unique décomposition cellulaire est réduit au module $\mathbf{A}$ et s’identifie à un sous-complexe de $\Gamma(\mathrm{Con}\,(f))$; notons $\Gamma(\mathrm{Con}\,(f),\,s)$ le complexe quotient. L’application $f$ définit un morphisme de complexes $\Gamma(f) : \Gamma(X) \to \Gamma(Y)$, et on peut montrer que les complexes $\Gamma(\mathrm{Cyl}\,(f))$ et $\Gamma(\mathrm{Con}\,(f),\,s)$ s’identifient respectivement à $\mathrm{Cyl}\,(\Gamma(f))$ et $\mathrm{Con}\,(\Gamma(f))$.

Par ailleurs, et sans hypothèses sur $X$ et $Y$, on associe à $f$ un morphisme de complexes $f_* : C(X,\,\mathbf{A}) \to C(Y,\,\mathbf{A})$. On peut construire des homotopismes injectifs de $\mathrm{Cyl}\,(f_*)$ dans $C(\mathrm{Cyl}\,(f),\,\mathbf{A})$ et de $\mathrm{Con}\,(f_*)$ dans $C(\mathrm{Con}\,(f),\,\{s\},\,\mathbf{A})$.
Soient $\tilde{f} : X \to \mathrm{Cyl}\,(f)$ l’application qui à $x$ associe l’image de $(0,\,x)$, $\alpha : Y \to \mathrm{Cyl}\,(f)$ l’application canonique et $\beta : \mathrm{Cyl}\,(f) \to Y$ l’application qui associe $y$ à son image dans $\mathrm{Cyl}\,(f)$ pour $y \in Y$ et $f(x)$ à l’image de $(t,\,x)$ dans $\mathrm{Cyl}\,(f)$ pour $t \in [0,\,1]$ et $x \in X$. L’application $\tilde{f}$ est un homéomorphisme de $X$ sur un fermé de $\mathrm{Cyl}\,(f)$, on a $\beta \circ \alpha = \mathrm{Id}_Y$, et $\alpha \circ \beta$ est topologiquement homotope à l’identité de $\mathrm{Cyl}\,(f)$. Ces propriétés sont à rapprocher de la proposition 7 ci-dessous. \*

Considérons maintenant les applications $\mathbf{A}$-linéaires graduées de degré 0

$$
\begin{align*}
\tilde{u} : C' &\to \mathrm{Cyl}\,(u)\,, & \tilde{u}(x') &= (x',\,0,\,0)\,, \\
\alpha : C &\to \mathrm{Cyl}\,(u)\,, & \alpha(x) &= (0,\,0,\,x)\,, \\
\beta : \mathrm{Cyl}\,(u) &\to C\,, & \beta(x',\,y',\,x) &= u(x') + x\,, \\
\pi : C &\to \mathrm{Con}\,(u)\,, & \pi(x) &= (0,\,x)\,, \\
\tilde{\pi} : \mathrm{Cyl}\,(u) &\to \mathrm{Con}\,(u)\,, & \tilde{\pi}(x',\,y',\,x) &= (y',\,x)\,, \\
\delta : \mathrm{Con}\,(u) &\to C'(-1)\,, & \delta(y',\,x) &= y'\,.
\end{align*}
$$

#### Proposition 7 {#alg-x-s2-prop-7 .statement}

*a)* *Les applications* $\tilde{u},\, \alpha,\, \beta,\, \pi,\, \tilde{\pi},\, \delta$ *sont des morphismes de complexes* : on a $u = \beta \circ \tilde{u},\, \pi = \tilde{\pi} \circ \alpha,\, \beta \circ \alpha = 1_C$.

*b)* *Les suites de morphismes de complexes*

(6) $$ 0 \to C' \xrightarrow{\tilde{u}} \mathrm{Cyl}\,(u) \xrightarrow{\tilde{\pi}} \mathrm{Con}\,(u) \to 0 $$

(7) $$ 0 \to C \xrightarrow{\pi} \mathrm{Con}\,(u) \xrightarrow{\delta} C'(-1) \to 0 $$

*sont exactes*.

*c)* *Les morphismes* $\alpha : C \to \mathrm{Cyl}\,(u)$ *et* $\beta : \mathrm{Cyl}\,(u) \to C$ *sont des homotopismes réciproques l’un de l’autre à homotopie près*.

L’assertion *a)* est équivalente aux formules

$$
\begin{align*}
\tilde{u} \circ d' &= \overline{D} \circ \tilde{u}\,, & \alpha \circ d &= \overline{D} \circ \alpha\,, & \beta \circ \overline{D} &= d \circ \beta\,, & \pi \circ d &= D \circ \pi\,, \\
\tilde{\pi} \circ \overline{D} &= D \circ \tilde{\pi}\,, & \delta \circ D &= -d' \circ \delta\,, & u &= \beta \circ \tilde{u}\,, & \pi &= \tilde{\pi} \circ \alpha\,, & \beta \circ \alpha &= 1_C
\end{align*}
$$

qui se vérifient par des calculs immédiats. L’assertion *b)* est triviale. Démontrons *c)* ; on a d’une part $\beta \circ \alpha = 1_C$; d’autre part si $\sigma : \mathrm{Cyl}\,(u) \to \mathrm{Cyl}\,(u)$ est l’application $\mathbf{A}$-linéaire graduée de degré 1 telle que $\sigma(x',\,y',\,x) = (0,\,x',\,0)$, on vérifie aussitôt que

$$
\overline{D} \circ \sigma + \sigma \circ \overline{D} + \alpha \circ \beta = 1_{\mathrm{Cyl}\,(u)}\,,
$$

d’où *c)*.

On peut résumer la prop. 7 par le diagramme commutatif suivant, où les lignes sont exactes, et où les flèches verticales sont des homotopismes :

$$
\begin{array}{ccccccccc}
0 & \longrightarrow & C & \xrightarrow{\pi} & \mathrm{Con}\,(u) & \xrightarrow{\delta} & C'(-1) & \longrightarrow & 0 \\
& & \downarrow^{\alpha} & & \downarrow^1 & & & & \\
0 & \longrightarrow & C' & \xrightarrow{\tilde{u}} & \mathrm{Cyl}\,(u) & \xrightarrow{\tilde{\pi}} & \mathrm{Con}\,(u) & \longrightarrow & 0 \\
& & \downarrow^1 & & \downarrow^{\beta} & & & & \\
& & C' & \xrightarrow{u} & C & & & &
\end{array}
$$

#### Corollaire {#alg-x-s2-n6-cor-1 .statement}

*Pour tout morphisme de complexes* $u : C' \to C$, *il existe un morphisme injectif de complexes* $\tilde{u} : C' \to C_1$ *et un homotopisme* $\beta : C_1 \to C$ *tel que* $u = \beta \circ \tilde{u}$.

#### Lemme 3 {#alg-x-s2-lem-3 .statement}

*a)* *L’homomorphisme de liaison*
$$
\partial_{n+1}(\pi, \delta) : H_n(C') \to H_n(C)
$$
*relatif à la suite exacte (7) est égal à* $-H_n(u)$.

*b)* *L’homomorphisme de liaison*
$$
\partial_n(\tilde{u}, \tilde{\pi}) : H_n(\mathrm{Con}\,(u)) \to H_{n-1}(C')
$$
*relatif à la suite exacte (6) est égal à* $H_n(\delta)$.

Soit $x' \in Z_n(C')$; comme $x' = \delta(x', 0)$ et que
$$
- D(x', 0) = (d'x', u(x')) = (0, u(x')) = \pi(u(x')) ,
$$
$\partial(\pi, \delta)$ applique par définition la classe de $x'$ dans $H_n(C')$ sur la classe de $-u(x')$ dans $H_n(C)$, d’où *a)*.

Soit $(y', x) \in \mathrm{Con}_n(u)$ tel que $D(y', x) = 0$; on a alors $(-d'y', dx - u(y')) = 0$. Comme $(y', x) = \tilde{\pi}(0, y', x)$ et que
$$
\overline{D}(0, y', x) = (y', -d'y', dx - u(y')) = (y', 0, 0) = \tilde{u}(\delta(y', x)) ,
$$
$\partial(\tilde{u}, \tilde{\pi})$ applique par définition la classe de $(y', x)$ dans $H_n(\mathrm{Con}\,(u))$ sur la classe de $\delta(y', x)$ dans $H_{n-1}(C')$, d’où *b)*.

#### Proposition 8 {#alg-x-s2-prop-8 .statement}

*On a la suite exacte illimitée*
(8) $$ \cdots \longrightarrow H_n(C') \xrightarrow{H_n(u)} H_n(C) \xrightarrow{H_n(\pi)} H_n(\mathrm{Con}\,(u)) \xrightarrow{H_n(\delta)} H_{n-1}(C') \longrightarrow \cdots . $$

En effet, compte tenu du *lemme 3, a)*, cela résulte du théorème 1 de X, p. 30, appliqué à la suite exacte (7).

#### Corollaire {#alg-x-s2-n6-cor-2 .statement}

*Pour que u soit un homologisme, il faut et il suffit que Con (u) soit d’homologie nulle.*

#### Remarque {#alg-x-s2-n6-rem-1 .statement}

Considérons le diagramme

$$
\begin{array}{ccccccccc}
\cdots & \longrightarrow & H_n(C') & \xrightarrow{H_n(\tilde{u})} & H_n(\mathrm{Cyl}\,(u)) & \xrightarrow{H_n(\pi)} & H_n(\mathrm{Con}\,(u)) & \xrightarrow{\partial_n(\tilde{u},\pi)} & H_{n-1}(C') \longrightarrow \cdots \\
& & \downarrow 1 & & \downarrow H_n(\beta) & & \downarrow 1 & & \downarrow 1 \\
\cdots & \longrightarrow & H_n(C') & \xrightarrow{H_n(u)} & H_n(C) & \xrightarrow{H_n(\pi)} & H_n(\mathrm{Con}\,(u)) & \xrightarrow{H_n(\delta)} & H_{n-1}(C') \longrightarrow \cdots
\end{array}
$$

où la première ligne (resp. la seconde) est la suite exacte d’homologie associée à la suite exacte (6) (resp. (7)). Les applications $H_n(\beta)$ sont bijectives (prop. 7, c)) et le diagramme est commutatif, puisque
a) $u = \beta \circ \tilde{u}$ (prop. 7, a)) donc $H_n(u) = H_n(\beta) \circ H_n(\tilde{u})$,
b) $H_n(\beta) = H_n(\alpha)^{-1}$ et $\pi = \tilde{\pi} \circ \alpha$ (prop. 7, a) et c)), donc $H_n(\tilde{\pi}) = H_n(\pi) \circ H_n(\beta)$,
c) $H_n(\delta) = \partial_n(\tilde{u},\tilde{\pi})$ (*lemme 3, b*)).

### 7. Le cône d’un morphisme injectif ; nouvelle définition de l’homomorphisme de liaison

Considérons maintenant une suite exacte de complexes

(9)
$$
0 \to C' \xrightarrow{u} C \xrightarrow{v} C'' \to 0 .
$$

Définissons une application A-linéaire graduée de degré 0
$$
\varphi : \mathrm{Con}\,(u) \to C''
$$
par $\varphi(y', x) = v(x)$. On a alors un diagramme commutatif de A-modules à lignes exactes

(10)
$$
\begin{array}{ccccccccc}
0 & \longrightarrow & C' & \xrightarrow{\tilde{u}} & \mathrm{Cyl}\,(u) & \xrightarrow{\tilde{\pi}} & \mathrm{Con}\,(u) & \longrightarrow & 0 \\
& & \downarrow 1 & & \downarrow \beta & & \downarrow \varphi & & \\
0 & \longrightarrow & C' & \xrightarrow{u} & C & \xrightarrow{v} & C'' & \longrightarrow & 0 .
\end{array}
$$

#### Proposition 9 {#alg-x-s2-prop-9 .statement}

*Les applications* $\beta$ *et* $\varphi$ *sont des homologismes de complexes*.
Pour $\beta$, cela résulte de la prop. 7, c). On a
$$
\begin{align*}
\varphi \circ D(y', x) &= \varphi(-d'y', dx - u(y')) = v(dx - u(y')) \\
&= v(dx) = d'' v(x) = d''(\varphi(y', x)) ,
\end{align*}
$$
donc $\varphi$ est bien un morphisme de complexes. D’autre part, $\varphi$ est surjectif et son noyau s’identifie au complexe $(\mathbf{K}, d_\mathbf{K})$ tel que $\mathbf{K} = C'(-1) \oplus C'$,
$$
d_\mathbf{K}(y', x') = (-d'y', d'x' - y') ;
$$
si $d_\mathbf{K}(y', x') = 0$, on a $y' = d' x'$, donc $(y', x') = d_\mathbf{K}(0, -x')$; il s’ensuit que $\mathrm{H}(\mathbf{K}) = 0$ et $\varphi$ est un homologisme d’après X, p. 30, cor. 1.

#### Remarque {#alg-x-s2-n7-rem-1 .statement}

L’homologisme $\beta$ est un homotopisme, mais $\varphi$ n’est pas en général un homotopisme (*cf.* X, p. 173, exercice 8).

#### Corollaire {#alg-x-s2-n7-cor-1 .statement}

*Le diagramme de A-modules gradués*

$$
\begin{array}{ccccc}
&& H(\operatorname{Con}(u)) &&\\
&\nearrow^{H(\pi)}&&\searrow^{H(\delta)}&\\
H(C)& &\downarrow^{H(\varphi)}&&H(C')(-.1)\\
&\searrow_{H(\iota)}&&\nearrow_{\partial(u,v)}&\\
&&H(C'')&&
\end{array}
$$

est commutatif et $H(\varphi)$ est bijectif.

Dans le diagramme commutatif (10), on a $H(1_{C'})\circ\widetilde{\partial}(\tilde u,\tilde\pi)=\partial(u,v)\circ H(\varphi)$ (X, p. 31, prop. 2) et $\widetilde{\partial}(\tilde u,\tilde\pi)=H(\delta)$ (X, p. 38, *lemme 3, b)), donc

$$
\partial(u,v)\circ H(\varphi)=H(\delta)\ ;
$$

d’autre part, $H(v)\circ H(\beta)=H(\varphi)\circ H(\tilde\pi)=H(\varphi)\circ H(\pi)\circ H(\beta)$ d’après X, p. 39, remarque. Comme $H(\beta)$ est bijectif, cela donne $H(v)=H(\varphi)\circ H(\pi)$.

On a donc $\partial(u,v)=H(\delta)\circ H(\varphi)^{-1}$, ce qui fournit une *nouvelle définition* de l’homomorphisme de liaison $\partial(u,v)$. On notera d’autre part que si on identifie $H(\operatorname{Con}(u))$ à $H(C'')$ par $H(\varphi)$, le corollaire précédent signifie que *la suite exacte* (8) *s’identifie alors à la suite exacte d’homologie relative à* (9).

### 8. Caractéristiques d’Euler-Poincaré

Dans ce n<sup>o</sup>, on considère un ensemble $\mathcal C$ de classes de A-modules qui est *additif et exact à gauche*, c’est-à-dire qui satisfait aux deux conditions suivantes :

(A) *Si* $M$ *et* $N$ *sont deux A-modules de type* $\mathcal C$, $M\oplus N$ *est de type* $\mathcal C$.

(G) *Si* $0\to M'\to M\to M''\to0$ *est une suite exacte de A-modules et si* $M$ *et* $M''$ *sont de type* $\mathcal C$, *alors* $M'$ *est de type* $\mathcal C$.

On dit que $\mathcal C$ est stable s’il satisfait aux conditions suivantes qui impliquent (A) et (G) :

(E) (« $\mathcal C$ est stable par extensions. ») *Si* $0\to M'\to M\to M''\to0$ *est une suite exacte de A-modules et si* $M'$ *et* $M''$ *sont de type* $\mathcal C$, *alors* $M$ *est de type* $\mathcal C$.

(S) (« $\mathcal C$ est stable par noyaux et conoyaux. ») *Pour tout homomorphisme* $f$ *de A-modules de type* $\mathcal C$, *les A-modules* $\operatorname{Ker}f$ *et* $\operatorname{Coker}f$ *sont de type* $\mathcal C$.

On note $K(\mathcal C)$ le groupe de Grothendieck de $\mathcal C$ et $[M]_{\mathcal C}$ ou $[M]$ l’élément de $K(\mathcal C)$ défini par le A-module $M$ (VIII, § 6, n<sup>o</sup> 2). Soient $G$ un groupe commutatif et $\varphi$ un homomorphisme de $K(\mathcal C)$ dans $G$.

#### Exemple 1 {#alg-x-s2-n8-exa-1 .statement}

Si A est un corps, on peut prendre pour $\mathcal C$ l’ensemble des classes d’espaces vectoriels de dimension finie et pour $\varphi$ l’isomorphisme de $K(\mathcal C)$ sur $\mathbf Z$ défini par $\varphi([M])=\dim(M)$.

#### Exemple 2 {#alg-x-s2-n8-exa-2 .statement}

On peut prendre pour $\mathcal{C}$ l’ensemble des classes de modules de longueur finie et pour $\varphi : K(\mathcal{C}) \to \mathbf{Z}$ l’homomorphisme défini par $\varphi([M]) = \operatorname{long}_A(M)$.

On dit qu’un A-module gradué M est de type $\mathcal{C}$ si $M_n$ est de type $\mathcal{C}$ pour tout $n$ (pour cela, il faut si M est borné, et il suffit si $\mathcal{C}$ est stable, que le module M soit de type $\mathcal{C}$).

#### Définition 8 {#alg-x-s2-def-8 .statement}

Soient M un A-module gradué borné de type $\mathcal{C}$ et $(M_n)$ sa graduation. On appelle $\varphi$-caractéristique de M et on note $\chi_\varphi(M)$ ou simplement $\chi(M)$ l’élément $\sum (-1)^n \varphi([M_n])$ de G.
Cette définition s’applique en particulier lorsque M est le module gradué sous-jacent à un complexe de A-modules.

#### Exemple 3 {#alg-x-s2-n8-exa-3 .statement}

Si M est borné de type $\mathcal{C}$, il en est de même de $M(p)$ pour tout $p \in \mathbf{Z}$, et on a $\chi(M(p)) = (-1)^p \chi(M)$.

#### Exemple 4 {#alg-x-s2-n8-exa-4 .statement}

Soit $0 \to M' \to M \to M'' \to 0$ une suite exacte de A-modules gradués et d’homomorphismes gradués de degré 0. Si M, M’ et M'' sont bornés de type $\mathcal{C}$, on a
$$
\chi(M) = \chi(M') + \chi(M'').
$$
Si M et M'' sont bornés de type $\mathcal{C}$, il en est de même de M’ ; si $\mathcal{C}$ est stable et si deux des trois modules sont bornés de type $\mathcal{C}$, il en est de même du troisième.

#### Exemple 5 {#alg-x-s2-n8-exa-5 .statement}

Soit $u : C' \to C$ un morphisme de complexes bornés de type $\mathcal{C}$. Alors Con ($u$) est borné de type $\mathcal{C}$, et on a :
$$
\chi(\operatorname{Con}(u)) = \chi(C) - \chi(C').
$$

#### Exemple 6 {#alg-x-s2-n8-exa-6 .statement}

On peut prendre pour G le groupe $K(\mathcal{C})$ lui-même, et pour $\varphi$ l’identité ; on note dans ce cas $\chi_{\mathcal{C}}(M)$ l’élément $\chi_\varphi(M) = \sum (-1)^n[M_n]$ de $K(\mathcal{C})$.

#### Remarque {#alg-x-s2-n8-rem-1 .statement}

On appelle polynôme de Poincaré de M relativement à $\varphi$ l’élément $P_M(t) = \sum \varphi([M_n]) t^n \in G \otimes \mathbf{Z}[t, t^{-1}]$. On a $P_M(1) = \varphi([M])$ et $P_M(-1) = \chi(M)$.

#### Lemme 4 {#alg-x-s2-lem-4 .statement}

Soit C un complexe borné de type $\mathcal{C}$. Si $H(C) = 0$, on a $\chi(C) = 0$.
Cela résulte de VIII, § 6, no 1, cor. de la prop. 1.

#### Proposition 10 {#alg-x-s2-prop-10 .statement}

Soient C et C’ deux complexes bornés de type $\mathcal{C}$. S’il existe un homologisme $u : C' \to C$, on a $\chi(C) = \chi(C')$.
En effet, Con ($u$) est borné de type $\mathcal{C}$ et on a $\chi(\operatorname{Con}(u)) = \chi(C) - \chi(C')$; d’autre part, $H(\operatorname{Con}(u)) = 0$ d’après X, p. 38, cor., donc $\chi(\operatorname{Con}(u)) = 0$ (lemme 4).

#### Proposition 11 {#alg-x-s2-prop-11 .statement}

Soit C un complexe borné de type $\mathcal{C}$.
a) Si $\mathcal{C}$ est stable, $H(C)$ est de type $\mathcal{C}$.
b) Si $H(C)$ est de type $\mathcal{C}$, il en est de même de $B(C)$ et de $Z(C)$, et on a $\chi(H(C)) = \chi(C)$.

a) Si $\mathcal{C}$ est stable, pour tout $n$ le module $Z_n(C)$ est de type $\mathcal{C}$ comme noyau de $d_n : C_n \to C_{n-1}$, et $H_n(C)$ est de type $\mathcal{C}$ comme conoyau de $C_{n+1} \to Z_n$. D’autre part, $H_n(C) = 0$ dès que $C_n = 0$.

b) Supposons $H(C)$ de type $\mathcal{C}$. Les suites exactes canoniques :

$$
0 \to Z_n(C) \to C_n \to B_{n-1}(C) \to 0
$$
$$
0 \to B_n(C) \to Z_n(C) \to H_n(C) \to 0
$$

montrent par récurrence sur $n$ à partir de la borne droite de $C$ que $Z_n(C)$ et $B_n(C)$ sont de type $\mathcal{C}$ pour tout $n$. On a alors

$$
\chi(C) = \chi(Z(C)) + \chi(B(C) (-1)) = \chi(Z(C)) - \chi(B(C)) = \chi(H(C)) .
$$

#### Corollaire {#alg-x-s2-n8-cor-1 .statement}

*Si $\mathcal{C}$ est stable et $C$ borné de type $\mathcal{C}$, le module gradué $H(C)$ est borné de type $\mathcal{C}$ et on a $\chi(H(C)) = \chi(C)$.*

#### Proposition 12 {#alg-x-s2-prop-12 .statement}

*Soit $0 \to C' \to C \to C'' \to 0$ une suite exacte de complexes.*

a) *Si $H(C), H(C')$ et $H(C'')$ sont bornés de type $\mathcal{C}$, on a*
$$
\chi(H(C)) = \chi(H(C')) + \chi(H(C'')) .
$$

b) *Si $\mathcal{C}$ est stable, et si deux des modules gradués $H(C), H(C')$ et $H(C'')$ sont bornés de type $\mathcal{C}$, il en est de même du troisième.*

La partie a) résulte du lemme 4 appliqué au complexe d’homologie nulle défini par la suite exacte d’homologie associée à la suite exacte donnée. La partie b) résulte, en considérant cette suite exacte d’homologie, du lemme suivant :

*Lemme 5. — Soit $M \to N \to P \to Q \to R$ une suite exacte de $A$-modules. Si $\mathcal{C}$ est stable, et si $M, N, Q$ et $R$ sont de type $\mathcal{C}$, le module $P$ est de type $\mathcal{C}$.
Posons $N' = \operatorname{Coker}(M \to N)$ et $Q' = \operatorname{Ker}(Q \to R)$. Les modules $N'$ et $Q'$ sont de type $\mathcal{C}$, et on a une suite exacte $0 \to N' \to P \to Q' \to 0$.*

#### Corollaire {#alg-x-s2-n8-cor-2 .statement}

*Supposons $\mathcal{C}$ stable, et soit $u : C' \to C$ un morphisme de complexes tels que $H(C)$ et $H(C')$ soient bornés de type $\mathcal{C}$. Alors $H(\operatorname{Con}(u))$ est borné de type $\mathcal{C}$, et on a*
$$
\chi(H(\operatorname{Con}(u))) = \chi(H(C)) - \chi(H(C')) .
$$

Cela résulte de la prop. 12 appliquée à la suite exacte de complexes (X, p. 37, prop. 7)
$$
0 \to C \to \operatorname{Con}(u) \to C'(-1) \to 0 .
$$

*Remarque. — Soient $E$ un complexe, $h : E \to C$ et $h' : E \to C'$ des homotopismes avec $C$ et $C'$ bornés de type $\mathcal{C}$. On a alors $\chi(C) = \chi(C')$. En effet, si $h_1$ est un inverse de $h$ à homotopie près, $h' \circ h_1$ est un homotopisme, donc un homologisme de $C$ dans

C' et on peut appliquer la prop. 10. Par suite, on peut étendre la définition 8 en posant $\chi(E) = \chi(C)$ dès qu’il existe un homotopisme de E sur un complexe C borné de type $\mathcal{C}$. Les propositions 10, 11, 12 et leurs corollaires se généralisent dans ce cadre.

Application :

\* Soit X un espace topologique admettant une décomposition cellulaire finie (cf. n° 3).
    a) Soient K et K' deux corps, posons $b_i = \dim_K(H_i(X, K))$ et $b'_i = \dim_{K'}(H_i(X, K'))$. On n’a pas nécessairement $b_i = b'_i$, mais on a $\Sigma (-1)^i b_i = \Sigma (-1)^i b'_i$.
    b) Soient $(X_n)$ et $(X'_n)$ deux décompositions cellulaires finies de X, et notons $c_n$ et $c'_n$ le nombre de cellules de dimension n dans ces deux décompositions. On a
    $$
    \Sigma (-1)^i c_i = \Sigma (-1)^i c'_i .
    $$
    c) Avec les notations de a) et b), on a $\Sigma (-1)^i c_i = \Sigma (--1)^i b_i$.
    Les propriétés a) et b) résultent de c), et c) résulte de la prop. 11 appliquée au complexe $\Gamma$ décrit au n° 3, en prenant pour $\mathcal{C}$ la classe des K-espaces vectoriels de dimension finie et pour $\varphi$ la fonction définie par $\varphi([M]) = \dim_K(M)$ (X, p. 40, exemple 1).

### 9. Complexes de modules à droite, complexes de multimodules

Un complexe de A-modules à droite est un A-module à droite gradué $(M_n)_{n \in \mathbf{Z}}$ muni d’un endomorphisme $d$ gradué de degré -1 et de carré nul ; c’est donc un complexe de modules sur l’anneau A opposé à A. Toutes les définitions et propriétés énoncées dans les numéros précédents s’appliquent donc aux complexes de modules à droite considérés comme complexes de modules sur l’anneau $A^\circ$.

De même, si A et B sont deux anneaux, un complexe de (A, B)-bimodules est un (A, B)-bimodule gradué M muni d’un endomorphisme $d$ gradué de degré (-1) et de carré nul ; si on munit M de sa structure canonique de $A \otimes_\mathbf{Z} B^\circ$-module à gauche, $d$ le munit d’une structure de $A \otimes_\mathbf{Z} B^-$-complexe. Toutes les définitions et propriétés énoncées dans les numéros précédents s’appliquent donc aux complexes de bimodules. On définit de manière analogue les complexes de multimodules.

### 10. Exemple : complexe de de Rham

Dans ce numéro, on suppose que A est une k-algèbre commutative sur un anneau commutatif k. On note $\Omega^1_{A/k}$ le A-module des k-différentielles de A (III, p. 134), $d^0 : A \to \Omega^1_{A/k}$ la k-dérivation $d_{A/k}$, et $\Omega_{A/k}$ la k-algèbre graduée $\Lambda_A(\Omega^1_{A/k})$.

#### Proposition 13 {#alg-x-s2-prop-13 .statement}

Il existe une unique k-antidérivation $d : \Omega_{A/k} \to \Omega_{A/k}$ de degré 1, de carré nul, qui prolonge la dérivation $d^0 : A \to \Omega^1_{A/k}$.

Montrons l’unicité de l’antidérivation d. Comme $d \circ d = 0$, on a pour $y, x_1, \ldots, x_p \in A$ :
$$
d(y dx_1 \wedge \ldots \wedge dx_p) = dy \wedge dx_1 \wedge \ldots \wedge dx_p .
$$
Le A-module $\Omega^p_{A/k}$ étant engendré par les éléments $dx_1 \wedge \ldots \wedge dx_p$, ceci prouve l’unicité de d.

Pour prouver l’existence, il suffit de construire un $k$-homomorphisme $d^1 : \Omega_{A/k}^1 \to \Omega_{A/k}^2$ tel que $d^1 \circ d^0 = 0$ et
$$
d^1(a \omega) = d^0(a) \wedge \omega + a d^1(\omega) \quad \text{pour } a \in A , \quad \omega \in \Omega_{A/k}^1 .
$$
En effet, il résulte alors de III, p. 128, prop. 14 (compte tenu de III, p. 118, remarque 2) qu’il existe une antidérivation $d : \Omega_{A/k} \to \Omega_{A/k}$ qui coïncide avec $d^0$ en degré 0 et avec $d^1$ en degré 1. Comme $d^0$ est nulle sur $A$, l’antidérivation $d$ est $k$-linéaire ; comme $d^1 \circ d^0 = 0$, on a $d \circ d = 0$ puisque $\Omega_{A/k}$ est engendrée comme $A$-algèbre par les éléments $d^0 a$ pour $a \in A$.

Pour définir $d^1$, rappelons (III, p. 133) que $\Omega_{A/k}^1$ est égal au $A$-module $\mathfrak{J}/\mathfrak{J}^2$, où $\mathfrak{J}$ est le noyau de la multiplication $m : A \otimes_k A \to A$. Considérons l’application $k$-linéaire $u : A \otimes_k A \to \Omega_{A/k}^2$ définie par $u(x \otimes y) = d^0(y) \wedge d^0(x)$. On a
$$
u(ax \otimes y - x \otimes ay) = d^0(y) \wedge d^0(ax) - d^0(ay) \wedge d^0(x) = d^0(xy) \wedge d^0(a)
$$
pour $x, y$ et $a$ dans $A$, d’où
$$
u((a \otimes 1 - 1 \otimes a) \xi) = d^0(m(\xi)) \wedge d^0(a) , \quad \xi \in A \otimes_k A , \quad a \in A .
$$
Comme $\mathfrak{J}$ est engendré comme $A$-module à gauche par les éléments $(a \otimes 1 - 1 \otimes a)$ pour $a \in A$, on en déduit que $u(\mathfrak{J}^2) = 0$; par conséquent $u$ définit par restriction à $\mathfrak{J}$ et passage au quotient une application $k$-linéaire $d^1 : \mathfrak{J}/\mathfrak{J}^2 \to \Omega_{A/k}^2$.

En faisant $\xi = b \otimes 1$ dans (12), avec $b \in A$, on obtient $d^1(b d^0(a)) = d^0(b) \wedge d^0(a)$; il en résulte que $d^1 \circ d^0 = 0$ et que $d^1(c \omega) = d^0(c) \wedge \omega + c d^1(\omega)$ pour $c \in A$ et $\omega = b d^0(a)$. Comme $\Omega_{A/k}^1$ est engendré comme $k$-module par les éléments $b d^0(a)$, pour $a$ et $b$ dans $A$, la formule (11) est satisfaite pour tout $\omega \in \Omega_{A/k}$, ce qui achève de prouver la proposition.

On dit parfois que les éléments $\omega \in \Omega_{A/k}^p$ sont les *formes différentielles extérieures de degré* $p$ de $A$ sur $k$, et que l’antidérivation $d$ est la *différentielle extérieure* de $\Omega_{A/k}$; le complexe $(\Omega_{A/k}, d)$ est appelé *complexe de de Rham de A sur k*, et son homologie est la *cohomologie de de Rham de A sur k*.

#### Exemple 1 {#alg-x-s2-n10-exa-1 .statement}

Prenons pour $A$ l’anneau $k[X_1, ..., X_n]$. Alors $\Omega_{A/k}^1$ est un $A$-module libre de base $dX_1, ..., dX_n$ (III, p. 134, exemple). Par conséquent, si pour toute partie $I = \{ i_1, ..., i_p \}$ de $\{ 1, n \}$ on pose $dX_I = dX_{i_1} \wedge ... \wedge dX_{i_p}$ (avec $i_1 < ... < i_p$), le $A$-module $\Omega_{A/k}^p$ admet comme base les éléments $dX_I$, où $I$ parcourt l’ensemble des parties de $\{ 1, n \}$ de cardinal $p$. On a
$$
d(P dX_I) = dP \wedge dX_I = \sum_{i \notin I} (-1)^{n(I,i)} \frac{\partial P}{\partial X_i} dX_{I \cup \{ i \}} ,
$$
où $n(I, i)$ désigne le nombre d’éléments de $I$ strictement inférieurs à $i$.

Les cycles de $Z^p(\Omega_{A/k})$ sont donc les éléments $\omega = \sum_{\operatorname{Card}(I) = p} P_I dX_I$ tels que, pour toute partie $J$ à $(p + 1)$ éléments de $\{ 1, n \}$, on ait :
$$
\sum_{i \in J} (-1)^{n(J,i)} \frac{\partial P_{J-\{i\}}}{\partial X_i} = 0 .
$$

L’élément $\omega$ est un bord si on peut choisir, pour toute partie $J \subset \{1, n\}$ à $(p - 1)$ éléments, un polynôme $Q_J \in A$ de façon que :

$$
P_I = \sum_{j \in I} (-1)^{n(I,j)} \frac{\partial Q_{I-\{j\}}}{\partial X_j}.
$$

Nous verrons au § 9 que le complexe de de Rham de $A$ sur $k$ est acyclique en degrés $> 0$ si $k$ est une $\mathbf{Q}$-algèbre (X, p. 159, *remarque 4*).

#### Exemple 2 {#alg-x-s2-n10-exa-2 .statement}

Supposons que $k = \mathbf{C}$ et $A = \mathbf{C} [X_1, ..., X_n]/(P_1, ..., P_r)$, où les $P_i$ sont des polynômes en $X_1, ..., X_n$, tels que l’ensemble des points de $\mathbf{C}^n$ où tous les $P_i$ s’annulent soit une sous-variété analytique $V$ de $\mathbf{C}^n$. On peut montrer que la cohomologie de de Rham de $A$ sur $\mathbf{C}$ est isomorphe à la *cohomologie singulière* $H(V, \mathbf{C})$.

Soient maintenant $M$ un $A$-module et $\nabla^0$ une application $k$-linéaire de $M$ dans $M \otimes_A \Omega^1_{A/k}$ telle que

$$(13)$$
$$
\nabla^0(am) = a \nabla^0(m) + m \otimes da \quad \text{pour} \quad a \in A,\ m \in M
$$
(on dit parfois que $\nabla^0$ est une *connexion* sur le $A$-module $M$).

#### Proposition 14 {#alg-x-s2-prop-14 .statement}

(i) *Il existe une unique application $k$-linéaire $\nabla$ du $\Omega_{A/k}$-module à droite $M \otimes_A \Omega_{A/k}$ dans lui-même, graduée de degré 1, qui prolonge $\nabla^0$ en degré 0 et satisfait à l’identité* :

$$(14)$$
$$
\nabla(x \omega) = (\nabla x) \omega + (-1)^p x(d\omega) \quad \text{pour} \quad x \in M \otimes_A \Omega^p_{A/k},\ \omega \in \Omega_{A/k}.
$$

(ii) *L’application composée $\nabla \circ \nabla$ est $\Omega_{A/k}$-linéaire ; en particulier l’application $R = \nabla^1 \circ \nabla^0$ de $M$ dans $M \otimes_A \Omega^2_{A/k}$ est $A$-linéaire, et on a*
$$
\nabla \circ \nabla(m \otimes \omega) = R(m).\omega \quad \text{pour} \quad m \in M,\ \omega \in \Omega_{A/k}.
$$

L’homomorphisme $R$ est parfois appelé *homomorphisme de courbure* de la connexion $\nabla^0$; s’il est nul, le couple $(M \otimes_A \Omega_{A/k}, \nabla)$ est un complexe, appelé encore *complexe de de Rham de* $(M, \nabla^0)$ *sur* $k$.

Démontrons (i). L’unicité de $\nabla$ est évidente. Définissons un $k$-homomorphisme $\overline{\nabla}$ de $M \otimes_k \Omega_{A/k}$ dans $M \otimes_A \Omega_{A/k}$ par
$$
\overline{\nabla}(m \otimes_k \omega) = (\nabla^0 m) \omega + m \otimes d\omega \quad \text{pour} \quad m \in M,\ \omega \in \Omega_{A/k}.
$$

Il résulte de (13) que $\overline{\nabla}(am \otimes \omega) = \overline{\nabla}(m \otimes a \omega)$, de sorte qu’on obtient par passage au quotient un $k$-homomorphisme $\nabla$ de $M \otimes_A \Omega_{A/k}$ dans lui-même, gradué de degré 1, prolongeant $\nabla^0$ en degré 0. Vérifions (14) : on a pour $m \in M$, $\alpha \in \Omega^p_{A/k}$, $\omega \in \Omega_{A/k}$ :
$$
\begin{align*}
\nabla((m \otimes \alpha).\omega) &= \nabla(m \otimes (\alpha \wedge \omega)) = \nabla^0(m).(\alpha \wedge \omega) + m \otimes d(\alpha \wedge \omega) \\
&= \nabla^0(m) \alpha.\omega + (m \otimes d\alpha) \omega + (-1)^p (m \otimes \alpha) d\omega \\
&= (\nabla(m \otimes \alpha)) \omega + (-1)^p (m \otimes \alpha) d\omega
\end{align*}
$$
ce qui prouve (14) pour $x = m \otimes \alpha$; le cas général s’en déduit par linéarité.

Démontrons (ii). Soient $x \in M \otimes_A \Omega_{A/k}^p, \omega \in \Omega_{A/k}$; par application répétée de (14), on obtient :
$$
\nabla \circ \nabla(x \omega) = \nabla(\nabla(x) \omega) + (-1)^p \nabla(x d \omega)
= (\nabla \circ \nabla(x)) \omega + (-1)^{p+1} \nabla(x)(d \omega) + (-1)^p \nabla(x)(d \omega)
= (\nabla \circ \nabla(x)) \omega,
$$
ce qui prouve la première assertion de (ii); les autres s’en déduisent immédiatement.

## EXERCICES {#alg-x-s2-exercises}

See the [exercises for § 2](exercises/s2/).
