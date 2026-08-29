---
book: alg
book_title: Algebra
chapter: X
chapter_title: ALGÈBRE HOMOLOGIQUE
section: 5
section_title: Modules d’extensions
lang: fr
source: alg-x-fr
book_pages: A X.81-A X.100
pdf_pages: 0087-0106, 0193-0194
extraction: ocr
subsections:
    - "no": 1
      title: ' Complexes d’homomorphismes'
      page: 81
      pdf_page: 87
    - "no": 2
      title: Complexes d’homomorphismes et homotopies
      page: 83
      pdf_page: 89
    - "no": 3
      title: Définition et premières propriétés des modules d’extensions
      page: 86
      pdf_page: 92
    - "no": 4
      title: Les homomorphismes de liaison et les suites exactes
      page: 89
      pdf_page: 95
    - "no": 5
      title: Modules projectifs, modules injectifs et modules d’extensions
      page: 93
      pdf_page: 99
    - "no": 6
      title: Formule des coefficients universels
      page: 94
      pdf_page: 100
    - "no": 7
      title: Généralisation aux complexes de multimodules ; les isomorphismes canoniques
      page: 98
      pdf_page: 104
statements: 36
exercises: 8
content_sha256: a8e0b6026ac3a6b3cf91b3261cf288e27bfe5f90539217221d869c3e7ea01bd3
---

## § 5. MODULES D’EXTENSIONS

*On conserve les notations générales du paragraphe 4. On convient de plus que, sauf mention expresse du contraire, tous les modules considérés sont des modules à gauche, tous les complexes considérés des complexes de modules à gauche.*

### 1.  Complexes d’homomorphismes

Soient $(C,d)$ et $(C',d')$ deux A-complexes. Considérons le $k$-module gradué $\operatorname{Homgr}_A(C,C')$ (II, p. 174, 175) : pour $n\in\mathbf{Z}$, $\operatorname{Homgr}_A(C,C')_n$ est le $k$-mod. le des applications A-linéaires graduées de degré $n$ de $C$ dans $C'$ ; autrement dit $\operatorname{Homgr}_A(C,C')$ s’identifie canoniquement au A-module

$$
\bigoplus_{n\in\mathbf{Z}}\prod_{p\in\mathbf{Z}}\operatorname{Hom}_A(C_p,C'_{p+n})
=
\bigoplus_{n\in\mathbf{Z}}\prod_{p+q=n}\operatorname{Hom}_A(C_p,{C'}^q).
$$

Définissons des applications $k$-linéaires

$$
D_n:\operatorname{Homgr}_A(C,C')_n\longrightarrow
\operatorname{Homgr}_A(C,C')_{n-1},\qquad n\in\mathbf{Z},
$$

par

(1) $$
D_n(f)=d'\circ f-(-1)^n f\circ d;
$$

on a

$$
D_{n-1}\circ D_n(f)
=D_{n-1}\bigl(d'\circ f-(-1)^n f\circ d\bigr)
=d'\circ d'\circ f-(-1)^n d'\circ f\circ d
$$

$$
\qquad\qquad{}-(-1)^{n-1}d'\circ f\circ d-f\circ d\circ d=0.
$$

Alors $(\operatorname{Homgr}_A(C,C'),D)$ est un complexe de $k$-modules appelé *complexe des homomorphismes de $C$ dans $C'$*.

Par exemple, Homgr_A (A, C') s’identifie canoniquement à C'. Notons aussi que, pour tout $n \in \mathbf{Z}$, on a $\mathrm{Homgr}_A (C, C') (n) = \mathrm{Homgr}_A (C, C'(n))$.

Les éléments de $Z_n(\mathrm{Homgr}_A (C, C'))$ sont les homomorphismes gradués $f$ de degré (descendant) $n$ de $C$ dans $C'$ tels que $d' \circ f = (-1)^n f \circ d$, c’est-à-dire les morphismes de complexes de $C$ dans $C'(n)$, ou encore de $C(p)$ dans $C'(p+n)$ pour $p$ quelconque fixé. On dit que ce sont les *morphismes de complexes de degré* (descendant) $n$ *de C dans C'* ; si $f, g \in Z_n(\mathrm{Homgr}_A (C, C'))$ et $s \in \mathrm{Homgr}_A (C, C')_{n+1}$, alors la condition $g - f = Ds$ signifie que $s$ est une homotopie reliant les morphismes $f$ et $g$ de $C$ dans $C'(n)$, de sorte que $H_n(\mathrm{Homgr}_A (C, C'))$ *est le k-module des classes d’homotopie de morphismes de degré (descendant) n de C dans C'*.

Soient $\alpha \in H_n(\mathrm{Homgr}_A (C, C'))$ et $p \in \mathbf{Z}$. Représentons $\alpha$ par $f \in Z_n(\mathrm{Homgr}_A (C, C'))$; alors $f$ est un morphisme de complexes de $C$ dans $C'(n)$, donc $H_p(f)$ est un homomorphisme de $H_p(C)$ dans $H_p(C'(n)) = H_{p+n}(C')$; comme $H_p(f)$ ne dépend que de la classe d’homotopie $\alpha$ de $f$ (X, p. 33, prop. 3), on en déduit un homomorphisme canonique de $k$-modules

$$
H_n(\mathrm{Homgr}_A (C, C')) \to \mathrm{Hom}_A (H_p(C), H_{p+n}(C')) ,
$$

d’où une *application k-linéaire graduée de degré* 0, dite *canonique*

$$
\lambda(C, C') : H(\mathrm{Homgr}_A (C, C')) \to \dot{\mathrm{Homgr}}_A (H(C), H(C')) .
$$

Les composantes homogènes de $\lambda(C, C')$ seront souvent notées :

$$
\lambda^n(C, C') : H^n(\mathrm{Homgr}_A (C, C')) \to \prod_{p+q=n} \mathrm{Hom}_A (H_p(C), H^q(C')) .
$$

#### Proposition 1 {#alg-x-s5-prop-1 .statement}

*Si C est nul à droite et C' nul à gauche, alors Homgr_A (C, C') est nul à gauche, et l’application k-linéaire canonique*

$$
\lambda^0(C, C') : H^0(\mathrm{Homgr}_A (C, C')) \to \mathrm{Hom}_A (H_0(C), H^0(C'))
$$

*est bijective*.

On a des suites exactes

$$
\begin{aligned}
&0 \longrightarrow H^0(C') \xrightarrow{i} {C'}^0 \xrightarrow{{d'}^0} {C'}^1 \\
&C_1 \xrightarrow{d_1} C_0 \xrightarrow{p} H_0(C) \longrightarrow 0 .
\end{aligned}
$$

D’autre part $\mathrm{Homgr}_A^0 (C, C')$ s’identifie à $\mathrm{Hom}_A (C_0, {C'}^0)$, $Z^0(\mathrm{Homgr}_A (C, C'))$ s’identifiant alors à l’ensemble des $f : C_0 \to {C'}^0$ tels que ${d'}^0 \circ f = 0, f \circ d_1 = 0$; $B^0(\mathrm{Homgr}_A (C, C'))$ est nul ; enfin l’application $\lambda^0$ associe à la classe de $f$ modulo $\{0\}$ l’homomorphisme $\varphi : H_0(C) \to H^0(C')$ tel que $f = i \circ \varphi \circ p$, d’où la proposition.

Soient $u : \tilde{C} \to C$ et $u' : C' \to \tilde{C}'$ des morphismes de complexes ; alors l’homomorphisme canonique $\mathrm{Homgr}_A (u, u') : \mathrm{Homgr}_A (C, C') \to \mathrm{Homgr}_A (\tilde{C}, \tilde{C}')$, défini par $f \mapsto u' \circ f \circ u$, est un morphisme de complexes, comme il résulte aussitôt de la formule (1). De plus, le diagramme suivant est commutatif

$$
\begin{array}{ccc}
H(\mathrm{Homgr}_A(C, C')) & \xrightarrow{\lambda(C, C')} & \mathrm{Homgr}_A(H(C), H(C')) \\
\downarrow H(\mathrm{Homgr}_A(u, u')) & & \downarrow \mathrm{Homgr}_A(H(u), H(u')) \\
H(\mathrm{Homgr}_A(\tilde{C}, \tilde{C}')) & \xrightarrow{\lambda(\tilde{C}, \tilde{C}') } & \mathrm{Homgr}_A(H(\tilde{C}), H(\tilde{C}')) .
\end{array}
$$

#### Proposition 2 {#alg-x-s5-prop-2 .statement}

*a) Soient $C' \xrightarrow{u} C \xrightarrow{v} C''$ une suite exacte de $A$-complexes, $P$ complexe projectif, $E$ un complexe injectif (X, p. 25). Alors les suites*

$$
\mathrm{Homgr}_A(P, C') \xrightarrow{\mathrm{Homgr}(1,u)} \mathrm{Homgr}_A(P, C) \xrightarrow{\mathrm{Homgr}(1,v)} \mathrm{Homgr}_A(P, C'')
$$
*et*
$$
\mathrm{Homgr}_A(C'', E) \xrightarrow{\mathrm{Homgr}(v,1)} \mathrm{Homgr}_A(C, E) \xrightarrow{\mathrm{Homgr}(u,1)} \mathrm{Homgr}_A(C', E)
$$
*sont des suites exactes de complexes de $k$-modules.*

*b) Soit $0 \to C' \xrightarrow{u} C \xrightarrow{v} C'' \to 0$ une suite de $A$-complexes qui est scindée en tant que suite exacte de $A$-modules gradués (c’est le cas par exemple si $C'$ est injectif, ou si $C''$ est projectif). Alors pour tout complexe $E$, les suites*

$$
0 \to \mathrm{Homgr}_A(E, C') \xrightarrow{\mathrm{Homgr}(1,u)} \mathrm{Homgr}_A(E, C) \xrightarrow{\mathrm{Homgr}(1,v)} \mathrm{Homgr}_A(E, C'') \to 0
$$
$$
0 \to \mathrm{Homgr}_A(C'', E) \xrightarrow{\mathrm{Homgr}(v,1)} \mathrm{Homgr}_A(C, E) \xrightarrow{\mathrm{Homgr}(u,1)} \mathrm{Homgr}_A(C', E) \to 0
$$
*sont des suites exactes de complexes de $k$-modules.*

Dans le cas *a)*, on remarque que les suites
$$
\mathrm{Hom}_A(P_p, C'_q) \to \mathrm{Hom}_A(P_p, C_q) \to \mathrm{Hom}_A(P_p, C''_q)
$$
*et*
$$
\mathrm{Hom}_A(C''_q, E_p) \to \mathrm{Hom}_A(C_q, E_p) \to \mathrm{Hom}_A(C'_q, E_p)
$$
sont exactes pour tous $p, q \in \mathbf{Z}$, et on applique II, p. 10, prop. 5 et II, p. 13, prop. 7. La démonstration de *b)* est analogue.

### 2. Complexes d’homomorphismes et homotopies

#### Proposition 3 {#alg-x-s5-prop-3 .statement}

*Soient $C, \tilde{C}, C', \tilde{C}'$ quatre $A$-complexes, $u : \tilde{C} \to C, v : \tilde{C} \to C, u' : C' \to \tilde{C}'$ et $v' : C' \to \tilde{C}'$ quatre morphismes de complexes.

a) Si $u$ et $u'$ sont homotopes à $v$ et $v'$ respectivement, alors les deux morphismes $\mathrm{Homgr}_A(u, u')$ et $\mathrm{Homgr}_A(v, v')$ de $\mathrm{Homgr}_A(C, C')$ dans $\mathrm{Homgr}_A(\tilde{C}, \tilde{C}')$ sont homotopes.

b) Si $u$ et $u'$ sont des homotopismes, $\mathrm{Homgr}_A(u, u')$ est un homotopisme.

c) Si $C$ ou $C'$ est homotope à zéro, $\mathrm{Homgr}_A(C, C')$ est homotope à zéro.*

Notons par la même lettre $d$ les différentielles des complexes $C$, $C_1$, $C'$, $C'_1$, et par $D$ les différentielles de $\mathrm{Homgr}_A(C,C')$ et $\mathrm{Homgr}_A(C_1,C'_1)$. Si $u$ (resp. $u'$) est homotope à $v$ (resp. $v'$), il existe un homomorphisme gradué de degré $1$,

$$
w:C_1\to C\qquad\text{(resp. }w':C'\to C'_1\text{)}
$$

tel que

$$
\tag{2}
u-v=dw+wd\qquad\text{(resp. }u'-v'=dw'+w'd\text{)}
$$

Soit $W:\mathrm{Homgr}_A(C,C')\to\mathrm{Homgr}_A(C_1,C'_1)$ l’homomorphisme gradué de degré $1$ tel que, pour $f\in\mathrm{Homgr}_A(C,C')_n$, $n\in\mathbf{Z}$, on ait

$$
\tag{3}
W(f)=w'fu+(-1)^n v'fw.
$$

On a alors

$$
(DW+WD)(f)=D[w'fu+(-1)^n v'fw]+W[df-(-1)^nfd]
$$

$$
=dw'fu-(-1)^{n+1}w'fud+(-1)^ndv'fw+v'fwd
$$

$$
\qquad+w'dfu+(-1)^{n+1}v'dfw-(-1)^nw'fdu+v'fdw
$$

$$
=(dw'+w'd)fu+v'f(wd+dw)
$$

$$
=(u'-v')fu+v'f(u-v)=u'fu-v'fv;
$$

cela s’écrit $DW+WD=\mathrm{Homgr}_A(u,u')-\mathrm{Homgr}_A(v,v')$, d’où a).

Démontrons b). Si $u$ et $u'$ sont des homotopismes, soient $\alpha:C\to\widetilde C$ et $\alpha':\widetilde C'\to C'$ des morphismes de complexes tels que $u\circ\alpha$, $\alpha\circ u$, $u'\circ\alpha'$, $\alpha'\circ u'$ soient homotopes respectivement à $\mathrm{Id}_C$, $\mathrm{Id}_{\widetilde C}$, $\mathrm{Id}_{\widetilde C'}$, $\mathrm{Id}_{C'}$. Alors $\mathrm{Homgr}(u,u')\circ\mathrm{Homgr}(\alpha,\alpha')$, qui est égal à $\mathrm{Homgr}(\alpha\circ u,u'\circ\alpha')$, est homotope d’après a) à

$$
\mathrm{Homgr}_A(\mathrm{Id}_C,\mathrm{Id}_{C'})=\mathrm{Id}_{\mathrm{Homgr}_A(C,C')};
$$

de même $\mathrm{Homgr}(\alpha,\alpha')\circ\mathrm{Homgr}(u,u')$ est homotope à $\mathrm{Id}_{\mathrm{Homgr}(\widetilde C,\widetilde C')}$, d’où b).

Enfin c) résulte de b) (appliqué au cas où $\widetilde C$ ou $\widetilde C'$ est nul).

#### Corollaire 1 {#alg-x-s5-prop-3-cor-1 .statement}

Si $C$ est scindé et $H(C)$ projectif (resp. si $C'$ est scindé et $H_n(C')$ injectif pour chaque $n$), alors l’homomorphisme canonique

$$
\lambda(C,C'):\ H(\mathrm{Homgr}_A(C,C'))\to\mathrm{Homgr}_A(H(C),H(C'))
$$

est bijectif.

Supposons par exemple $C'$ scindé et $H(C')$ injectif pour chaque $n$, le cas où $C$ est scindé et $H(C)$ projectif se démontrant de manière analogue. D’après X, p. 35, déf. 6, il existe un homotopisme $u':C'\to H(C')$ ; d’après la prop. 3, $\mathrm{Homgr}_A(1,u')$ est un homotopisme de $\mathrm{Homgr}_A(C,C')$ sur $\mathrm{Homgr}_A(C,H(C'))$ ; comme

$$
\mathrm{Homgr}_A(1,H(u'))\circ\lambda(C,C')=\lambda(C,H(C'))\circ H(\mathrm{Homgr}_A(1,u'))
$$

et que $\mathrm{Homgr}_A(1,H(u'))$ et $H(\mathrm{Homgr}_A(1,u'))$ sont bijectifs, il nous suffit de prouver que $\lambda(C, H(C'))$ est bijectif, ce qui nous ramène au cas où $C'$ est injectif et à différentielle nulle.

Alors les suites exactes canoniques (X, p. 28)

(III) $$
0 \to B(C) \xrightarrow{i} C \xrightarrow{\delta} C/B(C) \to 0
$$
(IV) $$
0 \to H(C) \xrightarrow{j} C/B(C) \xrightarrow{\delta} B(C) \to 0
$$

donnent des suites exactes (X, p. 83, prop. 2, a))

$$
0 \to \mathrm{Homgr}_A(C/B(C), C') \xrightarrow{l'} \mathrm{Homgr}_A(C, C') \xrightarrow{l} \mathrm{Homgr}_A(B(C), C') \to 0
$$
$$
0 \to \mathrm{Homgr}_A(B(C), C') \xrightarrow{\Delta} \mathrm{Homgr}_A(C/B(C), C') \xrightarrow{j} \mathrm{Homgr}_A(H(C), C') \to 0 .
$$

Comme $d_C = i \circ \delta \circ p$, la différentielle D de Homgr (C, C') est donnée par $D_n = (-1)^{n+1} P_n \circ \Delta_n \circ l_n$; on a alors

$$
\mathrm{Z}(\mathrm{Homgr}_A(C, C')) = \mathrm{Ker}\,(P \circ \Delta \circ I) = \mathrm{Ker}\,I = \mathrm{Im}\,P,
$$
$$
\mathrm{B}(\mathrm{Homgr}_A(C, C')) = \mathrm{Im}\,(P \circ \Delta \circ I) = P(\mathrm{Im}\,\Delta) = P(\mathrm{Ker}\,J) ;
$$

d’où un isomorphisme $\varphi : H(\mathrm{Homgr}_A(C, C')) \to \mathrm{Homgr}_A(H(C), C')$ tel que, si $a \in \mathrm{Homgr}_A(C/B(C), C')$, alors l’image par $\varphi$ de la classe de $P(a)$ est $J(a)$; on vérifie aussitôt que $\varphi$ s’identifie à l’homomorphisme canonique $\lambda$.

#### Corollaire 2 {#alg-x-s5-prop-3-cor-2 .statement}

Supposons $B(C)$ et $H(C)$ projectifs (resp. $B_n(C')$ et $H_n(C')$ injectifs pour chaque $n$). Alors $\lambda(C, C')$ est bijectif.

En effet $C$ (resp. $C'$) est alors scindé d’après X, p. 35, exemple 4, et on applique le cor. 1.

#### Corollaire 3 {#alg-x-s5-prop-3-cor-3 .statement}

Soit M un A-module projectif (resp. injectif). Pour tout complexe C de A-modules et tout entier $n$, l’homomorphisme canonique

$$
H^n(\mathrm{Homgr}_A(M, C)) \to \mathrm{Hom}_A(M, H^n(C))
$$
(resp. $H^n(\mathrm{Homgr}_A(C, M)) \to \mathrm{Hom}_A(H_n(C), M)$) est bijectif.

#### Lemme 1 {#alg-x-s5-lem-1 .statement}

a) Si C ou $C'$ est borné à droite, si C est projectif et si $H(C') = 0$, alors $H(\mathrm{Homgr}_A(C, C')) = 0$.
    b) Si C ou $C'$ est borné à gauche, si $C'$ est injectif et si $H(C) = 0$, alors $H(\mathrm{Homgr}_A(C, C')) = 0$.

Soit $f \in Z_n(\mathrm{Homgr}_A(C, C'))$; $f$ est donc un morphisme de complexes de C dans $C'(n)$; dans le cas a) (resp. b)), $f_m$ est nul pour $m$ assez petit (resp. assez grand). D’après X, p. 47, prop. 1, $f$ est alors homotope à zéro, donc appartient à $B_n(\mathrm{Homgr}_A(C, C'))$, d’où la conclusion.

#### Proposition 4 {#alg-x-s5-prop-4 .statement}

Soient $u : C' \to C$ un homologisme de complexes, $P$ un complexe projectif, $E$ un complexe injectif.

a) Si $P$ est borné à droite, ou si $C$ et $C'$ sont bornés à droite, alors

$$
\operatorname{Homgr}_A(1, u) : \operatorname{Homgr}_A(P, C') \to \operatorname{Homgr}_A(P, C)
$$

est un homologisme.

b) Si $E$ est borné à gauche, ou bien si $C$ et $C'$ sont bornés à gauche, alors

$$
\operatorname{Homgr}_A(u, 1) : \operatorname{Homgr}_A(C, E) \to \operatorname{Homgr}_A(C', E)
$$

est un homologisme.

Supposons d’abord $u$ injectif et posons $C'' = \operatorname{Coker}\ u$. Comme $u$ est un homologisme, $C''$ est d’homologie nulle. On a d’autre part des suites exactes (prop. 2)

$$
\begin{aligned}
0 &\to \operatorname{Homgr}_A(P, C') \xrightarrow{\operatorname{Homgr}(1, u)} \operatorname{Homgr}_A(P, C) \to \operatorname{Homgr}_A(P, C'') \to 0 \\
0 &\to \operatorname{Homgr}_A(C'', E) \to \operatorname{Homgr}_A(C, E) \xrightarrow{\operatorname{Homgr}(u, 1)} \operatorname{Homgr}_A(C', E) \to 0
\end{aligned}
$$

d’après le lemme 1, $\operatorname{Homgr}_A(P, C'')$ est d’homologie nulle dans le cas $a$, $\operatorname{Homgr}_A(C'', E)$ est d’homologie nulle dans le cas $b$, d’où la conclusion.

Dans le cas général, il existe (X, p. 38, cor. à la prop. 7) un complexe $\tilde{C}'$, qui est borné à droite (resp. à gauche) lorsque $C$ et $C'$ le sont, un morphisme injectif $\tilde{u} : C' \to \tilde{C}'$ et un homotopisme $\beta : \tilde{C}' \to C$ tel que $u = \beta \circ \tilde{u}$. Alors $\tilde{u}$ est un homologisme (X, p. 34, cor. à la prop. 5) ; d’après ce qui précède, $\operatorname{Homgr}_A(l_P, \tilde{u})$ (resp. $\operatorname{Homgr}_A(\tilde{u}, l_E)$) est un homologisme dans le cas $a$ (resp. $b$). D’autre part $\operatorname{Homgr}_A(l_P, \beta)$ (resp. $\operatorname{Homgr}_A(\beta, l_E)$) est un homotopisme (prop. 3) ; alors $\operatorname{Homgr}_A(l_P, u)$ (resp. $\operatorname{Homgr}_A(u, l_E)$) est composé de deux homologismes, donc est un homologisme.

### 3. Définition et premières propriétés des modules d’extensions

Pour tout $A$-module $E$, on note $p_E : L(E) \to E$ (resp. $e_E : E \to I(E)$) la résolution libre (resp. injective) canonique, cf. X, p. 50 (resp. p. 52).

#### Définition 1 {#alg-x-s5-def-1 .statement}

Soient $M$ et $N$ deux $A$-modules. On appelle module d’extensions de $N$ par $M$, le $k$-module gradué

$$
\text{(4)} \quad \operatorname{Ext}_A(M, N) = H(\operatorname{Homgr}_A(L(M), I(N))) .
$$

Les composantes homogènes de $\operatorname{Ext}_A(M, N)$ sont notées

$$
\text{(5)} \quad \operatorname{Ext}_A^n(M, N) = H^n(\operatorname{Homgr}_A(L(M), I(N))) .
$$

Comme $L(M)$ (resp. $I(N)$) est nul à droite (resp. gauche), on a

(6)
$$
\operatorname{Ext}^{n}_{A}(M,N)=0\qquad\text{pour }n<0.
$$

#### Remarque 1 {#alg-x-s5-n3-rem-1 .statement}

Nous verrons ci-dessous (X, p. 107, prop. 6) des propriétés de finitude des modules $\operatorname{Ext}^{n}_{A}(M,N)$. Par exemple si $A$ est commutatif noethérien, et si $M$ et $N$ sont des A-modules de type fini, chaque A-module $\operatorname{Ext}^{n}_{A}(M,N)$ est de type fini.

Soient $f : M' \to M$ et $g : N \to N'$ des homomorphismes de A-modules, on pose

$$
\operatorname{Ext}_{A}(f,g)=H(\operatorname{Homgr}_{A}(L(f),I(g)))\,;
$$

c’est un homomorphisme de degré 0 de $k$-modules gradués

$$
\operatorname{Ext}_{A}(f,g):\operatorname{Ext}_{A}(M,N)\to\operatorname{Ext}_{A}(M',N')\,,
$$

dont les composantes homogènes sont notées

$$
\operatorname{Ext}^{n}_{A}(f,g):\operatorname{Ext}^{n}_{A}(M,N)\to\operatorname{Ext}^{n}_{A}(M',N')\,.
$$

D’après la prop. 1 de X, p. 82, l’homomorphisme canonique

$$
\lambda^{0}(L(M),I(N)):H^{0}(\operatorname{Homgr}_{A}(L(M),I(N)))
\to\operatorname{Hom}_{A}(H_{0}(L(M)),H^{0}(I(N)))
$$

est bijectif ; utilisant les isomorphismes $M\to H_{0}(L(M))$ et $H^{0}(I(N))\to N$, on en déduit un *isomorphisme* dit *canonique*

(7)
$$
\lambda_{M,N}:\operatorname{Ext}^{0}_{A}(M,N)\to\operatorname{Hom}_{A}(M,N)\,.
$$

*On identifiera toujours* $\operatorname{Ext}^{0}_{A}(M,N)$ à $\operatorname{Hom}_{A}(M,N)$ par cet isomorphisme. Alors l’application $k$-linéaire $\operatorname{Ext}_{A}(f,g)$ s’identifie à $\operatorname{Hom}_{A}(f,g)$.

#### Remarque 2 {#alg-x-s5-n3-rem-2 .statement}

Le morphisme de complexes

$$
\operatorname{Homgr}_{A}(p_{M},\epsilon_{N}):\operatorname{Hom}_{A}(M,N)\to\operatorname{Homgr}_{A}(L(M),I(N))
$$

induit sur l’homologie de degré 0 l’isomorphisme

$$
\lambda^{-1}_{M,N}:\operatorname{Hom}_{A}(M,N)\to\operatorname{Ext}^{0}_{A}(M,N)
$$

réciproque de $\lambda_{M,N}$.

On a $L(1_{M})=1_{L(M)}$, $I(1_{N})=1_{I(N)}$, donc par passage à l’homologie

(8)
$$
\operatorname{Ext}_{A}(1_{M},1_{N})=1_{\operatorname{Ext}_{A}(M,N)}\,.
$$

Si $f' : M''\to M'$ et $g' : N'\to N''$ sont des homomorphismes de A-modules, on a $L(f\circ f')=L(f)\circ L(f')$ et $I(g'\circ g)=I(g')\circ I(g)$, donc

(9)
$$
\operatorname{Ext}_{A}(f\circ f',g'\circ g)=\operatorname{Ext}_{A}(f',g')\circ\operatorname{Ext}_{A}(f,g)\,.
$$

Considérons les morphismes de $k$-complexes
$$
\operatorname{Homgr}_A(L(M), N) \xrightarrow{\operatorname{Homgr}_A(1, e_N)} \operatorname{Homgr}_A(L(M), I(N)) \xleftarrow{\operatorname{Homgr}_A(p_M, 1)} \operatorname{Homgr}_A(M, I(N)),
$$
et les homomorphismes qu’ils induisent en homologie
$$
H(\operatorname{Homgr}_A(L(M), N)) \xrightarrow{\varphi_{M(N)}} \operatorname{Ext}_A(M, N) \xleftarrow{\overline{\varphi}_{N(M)}} H(\operatorname{Homgr}_A(M, I(N))) .
$$
D’après la prop. 4 de X, p. 86, $\operatorname{Homgr}_A(1, e_N)$ et $\operatorname{Homgr}_A(p_M, 1)$ sont des homologismes, d’où :

#### Proposition 5 {#alg-x-s5-prop-5 .statement}

*Les k-homomorphismes*
$$
\begin{aligned}
&\varphi_M(N) : H(\operatorname{Homgr}_A(L(M), N)) \to \operatorname{Ext}_A(M, N) \\
&\text{et} \quad \overline{\varphi}_N(M) : H(\operatorname{Homgr}_A(M, I(N))) \to \operatorname{Ext}_A(M, N) \text{ sont bijectifs}.
\end{aligned}
$$

#### Corollaire {#alg-x-s5-n3-cor-1 .statement}

*Si M est projectif (resp. si N est injectif), on a $\operatorname{Ext}_A^i(M, N) = 0$ pour $i > 0$.
En effet,
$$
\operatorname{Homgr}_A(1, e_N) : \operatorname{Hom}_A(M, N) \to \operatorname{Homgr}_A(M, I(N))
$$
(resp. $\operatorname{Homgr}_A(p_M, 1) : \operatorname{Hom}_A(M, N) \to \operatorname{Homgr}_A(L(M), N)$) est alors un homologisme (X, p. 86, prop. 4), d’où la conclusion.

*Remarques. — 3)* Si $g : N \to N'$ est un homomorphisme de A-modules, alors
$$
\operatorname{Homgr}_A(1_{L(M)}, g) \circ \operatorname{Homgr}_A(1_{L(M)}, e_N) = \operatorname{Homgr}_A(1_{L(M)}, e_{N'}) \circ \operatorname{Homgr}_A(1_{L(M)}, I(g))
$$
donc le diagramme
$$
\begin{array}{ccc}
H(\operatorname{Homgr}_A(L(M), N)) & \xrightarrow{\varphi_{M(N)}} & \operatorname{Ext}_A(M, N) \\
\operatorname{H}(\operatorname{Homgr}_A(1_{L(M)}, g)) \downarrow & & \downarrow \operatorname{Ext}_A(1_M, g) \\
H(\operatorname{Homgr}_A(L(M), N')) & \xrightarrow{\varphi_{M(N')}} & \operatorname{Ext}_A(M, N')
\end{array}
$$
est commutatif.

4) De même, si $f : M' \to M$ est un homomorphisme de A-modules, le diagramme
$$
\begin{array}{ccc}
H(\operatorname{Homgr}_A(M, I(N))) & \xrightarrow{\overline{\varphi}_{N(M)}} & \operatorname{Ext}_A(M, N) \\
\operatorname{H}(\operatorname{Homgr}_A(f, 1_{I(N)})) \downarrow & & \downarrow \operatorname{Ext}_A(f, 1_N) \\
H(\operatorname{Homgr}_A(M', I(N))) & \xrightarrow{\overline{\varphi}_{N(M')}} & \operatorname{Ext}_A(M', N)
\end{array}
$$
est commutatif.

#### Proposition 6 {#alg-x-s5-prop-6 .statement}

*L’application $(f,g)\mapsto \operatorname{Ext}_A(f,g)$ :*

$$
\operatorname{Hom}_A(M',M)\times\operatorname{Hom}_A(N,N')\longrightarrow
\operatorname{Homgr}_k\bigl(\operatorname{Ext}_A(M,N),\operatorname{Ext}_A(M',N')\bigr)
$$

*est $k$-bilinéaire.*

Soit $f\in\operatorname{Hom}_A(M',M)$, $g_1,g_2\in\operatorname{Hom}_A(N,N')$, $\lambda_1,\lambda_2\in k$ ; alors les morphismes $\operatorname{Homgr}_A(L(f),\lambda_1g_1+\lambda_2g_2)$ et $\lambda_1\operatorname{Homgr}_A(L(f),g_1)+\lambda_2\operatorname{Homgr}_A(L(f),g_2)$ de $\operatorname{Homgr}_A(L(M),N)$ dans $\operatorname{Homgr}_A(L(M),N')$ coïncident ; donc, d’après la prop. 5 et la *remarque* 3,

(10)     $\operatorname{Ext}_A(f,\lambda_1g_1+\lambda_2g_2)=\lambda_1\operatorname{Ext}_A(f,g_1)+\lambda_2\operatorname{Ext}_A(f,g_2)$.

On raisonne de même pour l’application $f\mapsto\operatorname{Ext}_A(f,g)$.

#### Corollaire {#alg-x-s5-n3-cor-2 .statement}

Soit $\lambda\in k$. Si $\lambda$ annule $M$ ou $N$, il annule $\operatorname{Ext}_A(M,N)$. En effet $\lambda 1_{\operatorname{Ext}(M,N)}=\operatorname{Ext}(\lambda 1_M,1_N)=\operatorname{Ext}(1_M,\lambda 1_N)$.

#### Proposition 7 {#alg-x-s5-prop-7 .statement}

Soient $I$ et $J$ deux ensembles, $(M_\alpha)_{\alpha\in I}$ et $(N_\beta)_{\beta\in J}$ deux familles de $A$-modules ; l’homomorphisme

$$
\operatorname{Ext}_A\left(\bigoplus_{\alpha\in I}M_\alpha,\prod_{\beta\in J}N_\beta\right)
\longrightarrow
\prod_{\substack{\beta\in J,\ \alpha\in I}}
\operatorname{Ext}_A(M_\alpha,N_\beta)
$$

déduit des homomorphismes canoniques $M_\alpha\to\bigoplus_{\alpha\in I}M_\alpha$ et $\prod_{\beta\in J}N_\beta\to N_\beta$ est bijectif.

Il suffit de prouver que pour tout $A$-module $M$ (resp. $N$), les homomorphismes

$$
\operatorname{Ext}(M,\prod_\beta N_\beta)\to\prod_\beta\operatorname{Ext}(M,N_\beta)
$$

(resp. $\operatorname{Ext}(\bigoplus M_\alpha,N)\to\prod_\alpha\operatorname{Ext}(M_\alpha,N)$)

sont bijectifs. Or cela résulte de ce qui précède, de la prop. 1 de X, p. 28, et des isomorphismes canoniques $\operatorname{Homgr}_A(L(M),\prod N_\beta)\to\prod\operatorname{Homgr}_A(L(M),N_\beta)$ et $\operatorname{Homgr}_A(\bigoplus M_\alpha,I(N))\to\prod\operatorname{Homgr}_A(M_\alpha,I(N))$.

#### Remarque 5 {#alg-x-s5-n3-rem-5 .statement}

Soient $P^\circ$ et $Q^\circ$ deux $A$-modules à droite. On définit $\operatorname{Ext}_A(P,Q)$ par

$$
\operatorname{Ext}_A(P,Q)=H(\operatorname{Homgr}_A(L(P),I(Q)))=H(\operatorname{Homgr}_{A^\circ}(L(P^\circ),I(Q^\circ)))
$$

$$
=\operatorname{Ext}_{A^\circ}(P^\circ,Q^\circ).
$$

Toutes les définitions et propositions de ce paragraphe s’appliquent donc aux $A$-modules à droite en les considérant comme modules à gauche sur l’anneau $A^\circ$.

### 4. Les homomorphismes de liaison et les suites exactes

Soit $M$ un $A$-module. Rappelons que pour tout $A$-module $N$, on a défini au numéro précédent un isomorphisme de $k$-modules

$$
\varphi_M(N):H(\operatorname{Homgr}_A(L(M),N))\longrightarrow\operatorname{Ext}_A(M,N).
$$

Soit

$$(\mathcal{E})\qquad 0\longrightarrow N'\xrightarrow{u}N\xrightarrow{v}N''\longrightarrow0$$

Bourbaki. — Algèbre X                                                                                                                             4 une suite exacte de $A$-modules ; la suite de $k$-complexes

$$
(\mathcal{E}) \quad 0 \longrightarrow \operatorname{Homgr}_A(L(M), N') \xrightarrow{\operatorname{Homgr}(1,u)} \operatorname{Homgr}_A(L(M), N) \\
\phantom{(M\mathcal{E})} \phantom{0} \xrightarrow{\operatorname{Homgr}(1,v)} \operatorname{Homgr}_A(L(M), N'') \longrightarrow 0
$$

est alors exacte ($X$, p. 83, prop. 2, $a$), soit

$$
\partial_{(M\mathcal{E})} : H(\operatorname{Homgr}_A(L(M), N'')) \to H(\operatorname{Homgr}_A(L(M), N'))
$$

l’homomorphisme de liaison correspondant ($X$, p. 29).

#### Définition 2 {#alg-x-s5-def-2 .statement}

*On appelle homomorphisme de liaison des modules d’extensions relatif au module $M$ et à la suite exacte $\mathcal{E}$ l’homomorphisme composé*

$$
\delta(M, \mathcal{E}) = \varphi_M(N') \circ \partial_{(M\mathcal{E})} \circ \varphi_M(N'')^{-1} : \operatorname{Ext}_A(M, N'') \to \operatorname{Ext}_A(M, N')
$$

C’est un $k$-homomorphisme gradué de degré ascendant 1, dont les composantes homogènes sont notées $\delta^n(M, \mathcal{E}) : \operatorname{Ext}_A^n(M, N'') \to \operatorname{Ext}_A^{n+1}(M, N')$.

#### Théorème 1 {#alg-x-s5-thm-1 .statement}

*La suite illimitée à droite d’homomorphismes de $k$-modules*

$$
0 \longrightarrow \operatorname{Hom}_A(M, N') \xrightarrow{\operatorname{Hom}(1,u)} \operatorname{Hom}_A(M, N) \xrightarrow{\operatorname{Hom}(1,v)} \operatorname{Hom}_A(M, N'')
$$
$$
\phantom{0} \xrightarrow{\delta_{(M,\mathcal{E})}} \operatorname{Ext}_A^1(M, N') \to \cdots \xrightarrow{\delta^{n-1}(M,\mathcal{E})} \operatorname{Ext}_A^n(M, N') \xrightarrow{\operatorname{Ext}^n(1,u)} \operatorname{Ext}_A^n(M, N)
$$
$$
\phantom{0} \xrightarrow{\operatorname{Ext}^n(1,v)} \operatorname{Ext}_A^n(M, N'') \xrightarrow{\delta^n(M,\mathcal{E})} \operatorname{Ext}_A^{n+1}(M, N') \to \cdots
$$

*est exacte*.

Considérons en effet le diagramme de la page X.91.
Il est commutatif d’après la *remarque* 3 de $X$, p. 88 et la déf. 2 ; d’autre part la ligne inférieure est exacte ($X$, p. 30, th. 1), et les flèches verticales sont bijectives ($X$, p. 88, prop. 5).

#### Corollaire {#alg-x-s5-n4-cor-1 .statement}

*Si* $\operatorname{Ext}_A^1(M, N') = 0$, *la suite*

$$
0 \longrightarrow \operatorname{Hom}_A(M, N') \xrightarrow{\operatorname{Hom}(1,u)} \operatorname{Hom}_A(M, N) \xrightarrow{\operatorname{Hom}(1,v)} \operatorname{Hom}_A(M, N'') \longrightarrow 0
$$

*est exacte*.

#### Proposition 8 {#alg-x-s5-prop-8 .statement}

*Soient* $f : M_1 \to M$ *un homomorphisme de* $A$*-modules* et

$$
\begin{array}{cccccccccc}
(\mathcal{E}) & 0 & \longrightarrow & N' & \xrightarrow{u} & N & \xrightarrow{v} & N'' & \longrightarrow & 0 \\
& & & g' \downarrow & & g \downarrow & & g'' \downarrow & & \\
(\mathcal{E}_1) & 0 & \longrightarrow & N'_1 & \xrightarrow{u_1} & N_1 & \xrightarrow{v_1} & N''_1 & \longrightarrow & 0
\end{array}
$$

$$
\begin{array}{ccccc}
\operatorname{Ext}(M,N') & \xrightarrow{\operatorname{Ext}(1,u)} & \operatorname{Ext}(M,N) & \xrightarrow{\operatorname{Ext}(1,v)} & \operatorname{Ext}(M,N'') \xrightarrow{\delta(M,\mathcal{G})} \operatorname{Ext}(M,N') \xrightarrow{\operatorname{Ext}(1,u)} \operatorname{Ext}(M,N)\\[6pt]
\Big\uparrow\vcenter{\rlap{$\scriptstyle\varphi_M(N')$}} && \Big\uparrow\vcenter{\rlap{$\scriptstyle\varphi_M(N)$}} && \Big\uparrow\vcenter{\rlap{$\scriptstyle\varphi_M(N'')$}} \qquad\qquad\Big\uparrow\vcenter{\rlap{$\scriptstyle\varphi_M(N')$}}\\[6pt]
H(\operatorname{Homgr}(L(M),N')) & \xrightarrow{H(\operatorname{Homgr}(1,u))} & H(\operatorname{Homgr}(L(M),N)) & \xrightarrow{H(\operatorname{Homgr}(1,v))} & H(\operatorname{Homgr}(L(M),N'')) \xrightarrow{\partial(M\mathcal{G})} H(\operatorname{Homgr}(L(M),N')) \xrightarrow{H(\operatorname{Homgr}(1,u))} H(\operatorname{Homgr}(L(M),N))
\end{array}
$$

un diagramme commutatif de $A$-modules à lignes exactes. Le diagramme de $k$-modules

$$
\begin{array}{ccc}
\mathrm{Ext}_A(M, N'') & \xrightarrow{\delta(M, \mathscr{E})} & \mathrm{Ext}_A(M, N') \\
\mathrm{Ext}(f, g'') \downarrow & & \mathrm{Ext}(f, g') \downarrow \\
\mathrm{Ext}_A(M_1, N''_1) & \xrightarrow{\delta(M, \mathscr{E}_1)} & \mathrm{Ext}_A(M_1, N'_1)
\end{array}
$$

est commutatif.
Cela résulte de X, p. 31, prop. 2 appliqué au diagramme commutatif

$$
\begin{array}{ccccccccc}
& & \mathrm{Homgr}(1, u) & & & & \mathrm{Homgr}(1, v) & & \\
0 \to \mathrm{Homgr}_A(L(M), N') & \to & \mathrm{Homgr}_A(L(M), N) & \to & \mathrm{Homgr}_A(L(M), N'') & \to & 0 \\
\mathrm{Homgr}(L(f), g') \downarrow & & \mathrm{Homgr}(L(f), g) \downarrow & & \mathrm{Homgr}(L(f), g'') \downarrow & & \\
0 \to \mathrm{Homgr}_A(L(M_1), N'_1) & \to & \mathrm{Homgr}_A(L(M_1), N_1) & \to & \mathrm{Homgr}_A(L(M_1), N''_1) & \to & 0
\end{array}
$$

Soient $N$ un $A$-module, et
$$(\mathcal{F})$$
$$0 \to M' \xrightarrow{r} M \xrightarrow{s} M'' \to 0$$
une suite exacte de $A$-modules ; la suite de complexes
$$(\mathcal{F}_N)$$
$$0 \longrightarrow \mathrm{Homgr}_A(M'', I(N)) \xrightarrow{\mathrm{Homgr}(s, 1)} \mathrm{Homgr}_A(M, I(N))$$
$$\xrightarrow{\mathrm{Homgr}(r, 1)} \mathrm{Homgr}_A(M', I(N)) \longrightarrow 0$$
est exacte (X, p. 83, prop. 2, $a$) ; soit
$$\partial(\mathcal{F}_N) : \mathrm{H}(\mathrm{Homgr}_A(M', I(N))) \to \mathrm{H}(\mathrm{Homgr}_A(M'', I(N)))$$
l’homomorphisme de liaison correspondant.

#### Définition 3 {#alg-x-s5-def-3 .statement}

On appelle homomorphisme de liaison des modules d’extensions relatif à la suite exacte $(\mathcal{F})$ et au module $N$, l’homomorphisme composé
$$\delta(\mathcal{F}, N) : \overline{\varphi}_N(M'') \circ \partial(\mathcal{F}_N) \circ \overline{\varphi}_N(M')^{-1} : \mathrm{Ext}_A(M', N) \to \mathrm{Ext}_A(M'', N).$$
C’est un $k$-homomorphisme gradué de degré ascendant 1, dont les composantes homogènes sont notées $\delta^n(\mathcal{F}, N) : \mathrm{Ext}_A^n(M', N) \to \mathrm{Ext}_A^{n+1}(M'', N)$.
On démontre alors comme ci-dessus les énoncés suivants :

#### Théorème 2 {#alg-x-s5-thm-2 .statement}

La suite illimitée à droite d’homomorphismes de $k$-modules
$$0 \longrightarrow \mathrm{Hom}_A(M'', N) \xrightarrow{\mathrm{Hom}(s, 1)} \mathrm{Hom}_A(M, N) \xrightarrow{\mathrm{Hom}(r, 1)} \mathrm{Hom}_A(M', N)$$
$$\xrightarrow{\delta^0(\mathcal{F}, N)} \mathrm{Ext}_A^1(M'', N) \to \cdots \xrightarrow{\delta^{n-1}(\mathcal{F}, N)} \mathrm{Ext}_A^n(M'', N) \xrightarrow{\mathrm{Ext}^n(s, 1)} \mathrm{Ext}_A^n(M, N)$$
$$\xrightarrow{\mathrm{Ext}^n(r, 1)} \mathrm{Ext}_A^n(M', N) \xrightarrow{\delta^n(\mathcal{F}, N)} \mathrm{Ext}_A^{n+1}(M'', N) \to \cdots$$
est exacte.

#### Corollaire {#alg-x-s5-n4-cor-2 .statement}

Si $\operatorname{Ext}_A^1(M'', N) = 0$, la suite

$$
0 \longrightarrow \operatorname{Hom}_A(M'', N) \xrightarrow{\operatorname{Hom}(s, 1)} \operatorname{Hom}_A(M, N) \xrightarrow{\operatorname{Hom}(r, 1)} \operatorname{Hom}_A(M', N) \longrightarrow 0
$$

est exacte.

#### Proposition 9 {#alg-x-s5-prop-9 .statement}

Soient $g : N \to N_1$ un homomorphisme de $A$-modules et

$$
\begin{array}{cccccc}
(\mathcal{F}_1) & 0 \to M'_1 \xrightarrow{r_1} M_1 \xrightarrow{s_1} M''_1 \to 0 \\
& f' \downarrow & f \downarrow & f'' \downarrow \\
(\mathcal{F}) & 0 \to M' \xrightarrow{r} M \xrightarrow{s} M'' \to 0
\end{array}
$$

un diagramme commutatif de $A$-modules à lignes exactes. Le diagramme de $k$-modules

$$
\begin{array}{ccc}
\operatorname{Ext}_A(M', N) & \xrightarrow{\delta(\mathcal{F}, N)} & \operatorname{Ext}_A(M'', N) \\
\operatorname{Ext}_A(f', g) \downarrow & & \operatorname{Ext}_A(f'', g) \downarrow \\
\operatorname{Ext}_A(M'_1, N_1) & \xrightarrow{\delta(\mathcal{F}_1, N_1)} & \operatorname{Ext}_A(M''_1, N_1)
\end{array}
$$

est commutatif.

### 5. Modules projectifs, modules injectifs et modules d’extensions

#### Proposition 10 {#alg-x-s5-prop-10 .statement}

Soit $M$ un $A$-module. Les conditions suivantes sont équivalentes :

(i) $M$ est projectif.
(ii) $\operatorname{Ext}_A^i(M, N) = 0$ pour tout $A$-module $N$ et pour tout entier $i > 0$.
(iii) $\operatorname{Ext}_A^1(M, N) = 0$ pour tout $A$-module $N$.
(iv) Il existe une suite exacte

$$
0 \to K \xrightarrow{\nu} P \xrightarrow{\iota} M \to 0,
$$

où $P$ est projectif, et où $\operatorname{Ext}_A^1(M, K) = 0$.

(i) $\Rightarrow$ (ii) : c’est le corollaire de la prop. 5 de X, p. 88.
(ii) $\Rightarrow$ (iii) : c’est trivial.
(iii) $\Rightarrow$ (iv) : c’est clair puisque $M$ est quotient d’un module libre $P$.
(iv) $\Rightarrow$ (i) : puisque $\operatorname{Ext}_A^1(M, K) = 0$, l’application canonique

$$
\operatorname{Hom}_A(M, P) \to \operatorname{Hom}_A(M, M)
$$

est surjective (X, p. 90, corollaire); il existe donc une section $A$-linéaire de $\nu$ et $M$ est isomorphe à un facteur direct de $P$, donc est projectif.

#### Proposition 11 {#alg-x-s5-prop-11 .statement}

Soit $N$ un $A$-module. Les conditions suivantes sont équivalentes :

(i) $N$ est injectif.
(ii) $\operatorname{Ext}_A^i(M, N) = 0$ pour tout $A$-module $M$ et tout entier $i > 0$.

(iii) $\mathrm{Ext}_A^1(M, N) = 0$ pour tout $A$-module $M$.

(iv) Il existe une suite exacte

$$
0 \to N \xrightarrow{u} I \xrightarrow{v} C \to 0,
$$

où $I$ est injectif et où $\mathrm{Ext}_A^1(C, N) = 0$;

(v) $\mathrm{Ext}_A^1(M, N) = 0$ pour tout $A$-module monogène $M$.

(i) $\Rightarrow$ (ii) : c'est le corollaire de la prop. 5 de X, p. 88.

(ii) $\Rightarrow$ (iii) $\Rightarrow$ (v) : c'est trivial.

(iii) $\Rightarrow$ (iv) : c'est clair puisque $N$ est un sous-module d'un module injectif (X, p. 19, cor. 3).

(iv) $\Rightarrow$ (i) : puisque $\mathrm{Ext}_A^1(C, N) = 0$, l'homomorphisme canonique

$$
\mathrm{Hom}_A(I, N) \to \mathrm{Hom}_A(N, N)
$$

est surjectif (X, p. 93, corollaire) ; il existe donc une rétraction $A$-linéaire de $u$ et $N$ est isomorphe à un facteur direct de $I$, donc est injectif (X, p. 16, prop. 9).

(v) $\Rightarrow$ (i) : si $\alpha$ est un idéal de $A$, on a $\mathrm{Ext}_A^1(A/\alpha, N) = 0$; l'application canonique $\mathrm{Hom}_A(A, N) \to \mathrm{Hom}_A(\alpha, N)$ est donc surjective et $N$ est injectif (X, p. 16, prop. 10).

### 6. Formule des coefficients universels

Dans ce numéro, on considère deux complexes de $A$-modules $(C, d)$ et $(C', d')$. Considérons les suites exactes canoniques :

(I)

$$
0 \to Z(C) \xrightarrow{j} C \xrightarrow{\delta} B(C)(-1) \to 0,
$$

(II_p)

$$
0 \to B_p(C) \xrightarrow{i} Z_p(C) \xrightarrow{\rho} H_p(C) \to 0;
$$

on déduit de $\delta$ un $k$-homomorphisme

$$
H(\mathrm{Homgr}(\delta, 1)) : H(Homgr_A(B(C), C'))(1) \to H(Homgr_A(C, C'));
$$

on déduit de (II_p) des homomorphismes de liaisons :

$$
\delta(11_p, H^q(C')) : \mathrm{Hom}_A(B_p(C), H^q(C')) \to \mathrm{Ext}_A^1(H_p(C), H^q(C')) .
$$

d'où, par passage au produit, des homomorphismes de $k$-modules

$$
\varphi^n : \mathrm{Homgr}_A^n(B(C), H(C')) \to \prod_{p+q=n} \mathrm{Ext}_A^1(H_p(C), H^q(C'))
$$

On dispose par ailleurs d'homomorphismes canoniques (X, p. 82)

$$
\lambda^n(B(C), C') : H^n(Homgr_A(B(C), C')) \to \mathrm{Homgr}_A^n(B(C), H(C')) .
$$

Avec ces notations :

#### Théorème 3 {#alg-x-s5-thm-3 .statement}

Supposons les A-modules B(C) et Z(C) projectifs. Il existe, pour chaque n, un unique homomorphisme de k-modules

$$
\beta^n : \prod_{p+q=n-1} \mathrm{Ext}_A^1(H_p(C), H^q(C')) \to H^n(\mathrm{Homgr}_A(C, C'))
$$

rendant commutatif le diagramme

$$
\begin{array}{ccc}
\mathrm{Homgr}_A^{n-1}(B(C), H(C')) & \xleftarrow{\lambda^{n-1}(B(C), C')} & H^{n-1}(\mathrm{Homgr}_A(B(C), C')) \\
\downarrow \varphi^{n-1} & & \downarrow H^n(\mathrm{Homgr}(\delta, 1)) \\
\prod_{p+q=n-1} \mathrm{Ext}_A^1(H_p(C), H^q(C')) & \xrightarrow{\beta^n} & H^n(\mathrm{Homgr}_A(C, C')) .
\end{array}
$$

Les suites de k-modules gradués

(11) $0 \to \prod_{p+q=n-1} \mathrm{Ext}_A^1(H_p(C), H^q(C')) \xrightarrow{\beta^n} H^n(\mathrm{Homgr}_A(C, C'))$

$$
\xrightarrow{\lambda^n(C, C')} \prod_{p+q=n} \mathrm{Hom}_A(H_p(C), H^q(C')) \to 0
$$

sont exactes.

#### Remarque {#alg-x-s5-n6-rem-1 .statement}

On peut démontrer un énoncé analogue, en supposant B_n(C') et C'/B_n(C') injectifs pour chaque n.

Posons pour simplifier B = B(C), Z = Z(C), H = H(C) et H' = H(C'). Comme B est projectif, on déduit de (1) une suite exacte

(12) $0 \to \mathrm{Homgr}_A(B, C')(1) \xrightarrow{\mathrm{Homgr}(\delta, 1)} \mathrm{Homgr}_A(C, C')$

$$
\xrightarrow{\mathrm{Homgr}(i, 1)} \mathrm{Homgr}_A(Z, C') \to 0 .
$$

#### Lemme 2 {#alg-x-s5-lem-2 .statement}

L’homomorphisme de liaison

$$
H^n(\mathrm{Homgr}_A(Z, C')) \to H^n(\mathrm{Homgr}_A(B, C'))
$$

associé à (12) est égal à $(-1)^{n+1} H(\mathrm{Homgr}(i, 1))$.

En effet, soit $a \in Z^n(\mathrm{Homgr}_A(Z, C'))$; c’est un morphisme de complexes de degré ascendant n de Z dans C', dont les valeurs sont donc dans Z(C'). Puisque la suite exacte (1) est scindée (B étant projectif), a se prolonge en un élément b de $\mathrm{Homgr}_A^n(C, Z(C'))$. Par définition, l’image de la classe de a par l’homomorphisme de liaison cherché est la classe dans $H^n(\mathrm{Homgr}_A(B, C'))$ de l’homomorphisme u de B(C) dans C' tel que pour $x \in C$, on ait

$$
u(dx) = Db(x) = d'b(x) - (-1)^n b(dx) = (-1)^{n+1} b(dx) = (-1)^{n+1} a(dx),
$$

d’où l’assertion.

La suite exacte d’homologie associée à (12) donne donc la suite exacte
→ H^n(\mathrm{Homgr}_A(Z, C')) \xrightarrow{\mathrm{H}(\mathrm{Homgr}(i,1))} H^n(\mathrm{Homgr}_A(B, C'))
\xrightarrow{\mathrm{H}(\mathrm{Homgr}(\delta,1))} H^{n+1}(\mathrm{Homgr}_A(C, C')) \xrightarrow{\mathrm{H}(\mathrm{Homgr}(j,1))} H^{n+1}(\mathrm{Homgr}_A(Z, C')) \to \ldots .

Par ailleurs, puisque Z est projectif, on tire de (11_p) des suites exactes
0 \to \mathrm{Hom}_A(H_p, H'^q) \to \mathrm{Hom}_A(Z_p, H'^q) \to \mathrm{Hom}_A(B_p, H'^q) \to \mathrm{Ext}_A^1(H_p, H'^q) \to 0 ,
d’où, par passage aux produits, des suites exactes
0 \to \mathrm{Homgr}_A^n(H, H') \to \mathrm{Homgr}_A^n(Z, H') \to \mathrm{Homgr}_A^n(B, H')
\to \prod_{p+q=n} \mathrm{Ext}_A^1(H_p, H'^q) \to 0 .
Enfin, on dispose des homomorphismes canoniques du n° 1 :
$$
\begin{align*}
\lambda_B &= \lambda(B, C') : \mathrm{H}(\mathrm{Homgr}_A(B, C')) \to \mathrm{Homgr}_A(B, H') , \\
\lambda_Z &= \lambda(Z, C') : \mathrm{H}(\mathrm{Homgr}_A(Z, C')) \to \mathrm{Homgr}_A(Z, H') , \\
\lambda_C &= \lambda(C, C') : \mathrm{H}(\mathrm{Homgr}_A(C, C')) \to \mathrm{Homgr}_A(H, H') ,
\end{align*}
$$
d’où le diagramme à lignes exactes de la page X.97.

Ce diagramme est commutatif par construction des homomorphismes $\lambda$. Par ailleurs, comme les complexes B et Z sont scindés et projectifs, $\lambda_B$ et $\lambda_Z$ sont bijectifs ($\lambda$, p. 84, cor. 1). On en déduit, d’une part que $\lambda_C^n$ est surjectif, de noyau égal à $\mathrm{Im}\ H^n(\mathrm{Homgr}(\delta, 1))$, d’autre part que $\varphi^{n-1} \circ \lambda_B^{n-1}$ est surjectif, de noyau égal à $\mathrm{Ker}\ H^n(\mathrm{Homgr}(\delta, 1))$. Le théorème résulte immédiatement de là.

#### Corollaire 1 {#alg-x-s5-lem-2-cor-1 .statement}

Supposons B(C) et Z(C) projectifs et B^n(C') injectif pour chaque n. Alors les suites exactes (11) sont scindées.
Cela résulte du théorème et du lemme suivant :

#### Lemme 3 {#alg-x-s5-lem-3 .statement}

Si B(C) est projectif et B_n(C') injectif pour chaque n, l’homomorphisme canonique $\lambda(C, C') : \mathrm{H}(\mathrm{Homgr}_A(C, C')) \to \mathrm{Homgr}_A(\mathrm{H}(C), \mathrm{H}(C'))$ possède une section k linéaire.

En effet, d’après X, p. 35, remarques a) et b), il existe des homologismes
$$
\varphi : C \to \mathrm{H}(C) \quad \text{et} \quad \varphi' : \mathrm{H}(C') \to C'
$$
tels que $\mathrm{H}(\varphi) = 1_{\mathrm{H}(C)}$ et $\mathrm{H}(\varphi') = 1_{\mathrm{H}(C')}$.
Dans le diagramme commutatif
$$
\begin{array}{ccc}
\mathrm{H}(\mathrm{Homgr}_A(\mathrm{H}(C), \mathrm{H}(C'))) & \xrightarrow{\mathrm{H}(\mathrm{Homgr}(\varphi, \varphi'))} & \mathrm{H}(\mathrm{Homgr}_A(C, C')) \\
\lambda(\mathrm{H}(C), \mathrm{H}(C')) \downarrow & & \downarrow \lambda(C, C') \\
\mathrm{Homgr}_A(\mathrm{H}(C), \mathrm{H}(C')) & \xrightarrow{\mathrm{Homgr}(\mathrm{H}(\varphi), \mathrm{H}(\varphi'))} & \mathrm{Homgr}_A(\mathrm{H}(C), \mathrm{H}(C')) ,
\end{array}
$$
$\lambda(\mathrm{H}(C), \mathrm{H}(C'))$ est bijectif et $\mathrm{Homgr}(\mathrm{H}(\varphi), \mathrm{H}(\varphi'))$ est l’identité, d’où l’assertion.

$$
\begin{array}{ccccccccc}
\operatorname{Homgr}_{A}^{n-1}(Z,H')&
\xrightarrow{\operatorname{Homgr}^{n-1}(i,1)}&
\operatorname{Homgr}_{A}^{n-1}(B,H')&
\xrightarrow{\varphi^{n-1}}&
\displaystyle\prod_{p+q=n-1}\operatorname{Ext}^{1}(H_p,H^q)&
\longrightarrow&0
\\[2ex]
\uparrow\scriptstyle{\lambda_Z^{n-1}}&&
\uparrow\scriptstyle{\lambda_B^{n-1}}&&&&
\\[-1ex]
H^{n-1}(\operatorname{Homgr}_{A}(Z,C'))&
\xrightarrow{H^{n-1}(\operatorname{Homgr}(i,1))}&
H^{n-1}(\operatorname{Homgr}_{A}(B,C'))&
\xrightarrow{H^n(\operatorname{Homgr}(\delta,1))}&
H^n(\operatorname{Homgr}_{A}(C,C'))&
\xrightarrow{H^n(\operatorname{Homgr}(j,1))}&
H^n(\operatorname{Homgr}_{A}(Z,C'))&
\xrightarrow{H^n(\operatorname{Homgr}(i,1))}&
H^n(\operatorname{Homgr}_{A}(B,C'))
\\[2ex]
&&&&
\uparrow\scriptstyle{\lambda_C^n}&&
\uparrow\scriptstyle{\lambda_Z^n}&&
\uparrow\scriptstyle{\lambda_B^n}
\\[-1ex]
&&&
0\longrightarrow&
\operatorname{Homgr}_{A}^{n}(H,H')&
\xrightarrow{\operatorname{Homgr}^{n}(j,1)}&
\operatorname{Homgr}_{A}^{n}(Z,H')&
\xrightarrow{\operatorname{Homgr}^{n}(i,1)}&
\operatorname{Homgr}_{A}^{n}(B,H')
\end{array}
$$

#### Corollaire 2 {#alg-x-s5-lem-3-cor-2 .statement}

Si $B(C)$ et $Z(C)$ sont projectifs, on a, pour tout $A$-module $N$ et tout entier $n$, une suite exacte scindée :

(13) $0 \longrightarrow \mathrm{Ext}_A^1(H_{n-1}(C), N) \xrightarrow{\beta^n} H^n(\mathrm{Homgr}_A(C, N)) \xrightarrow{\lambda^n} \mathrm{Hom}_A(H_n(C), N) \longrightarrow 0$.

#### Corollaire 3 (« formule des coefficients universels ») {#alg-x-s5-lem-3-cor-3 .statement}

Supposons $A$ principal et $C$ libre. On a pour tout $A$-module $N$ et tout entier $n$ une suite exacte scindée (13).
En effet $B(C)$ et $Z(C)$ sont libres comme sous-modules du module libre $C$ (VII. § 3, cor. 2 au th. 1).

#### Corollaire 4 {#alg-x-s5-lem-3-cor-4 .statement}

Si $C$ est borné à droite et si $C$ et $H(C)$ sont projectifs, alors

$$
\lambda(C, C') : H(\mathrm{Homgr}_A(C, C')) \to \mathrm{Homgr}_A(H(C), H(C'))
$$

est bijectif.
D’après le théorème, il suffit de prouver que $B(C)$ et $Z(C)$ sont projectifs. Or on a des suites exactes

$$
\begin{align*}
0 &\to B_n(C) \to Z_n(C) \to H_n(C) \to 0 \\
0 &\to Z_n(C) \to C_n \to B_{n-1}(C) \to 0,
\end{align*}
$$

donc $(B_{n-1}(C) \text{ est projectif}) \Rightarrow (Z_n(C) \text{ est projectif}) \Rightarrow (B_n(C) \text{ est projectif}).$ On conclut en remarquant que $B_n(C) = 0$ pour $n$ assez petit.

### 7. Généralisation aux complexes de multimodules ; les isomorphismes canoniques
Soient $B, B'$ deux anneaux, $C$ un complexe de $(A, B)$-bimodules, $C'$ un complexe de $(A, B')$-bimodules ; alors $(\mathrm{Homgr}_A(C, C'), D)$ est un complexe de $(B, B')$-bimodules et l’homomorphisme canonique $\lambda : H(\mathrm{Homgr}_A(C, C')) \to \mathrm{Homgr}_A(H(C), H(C'))$ est un homomorphisme de $(B, B')$-bimodules.
Si $M$ est un $(A, B)$-bimodule et $N$ un $(A, B')$-bimodule, alors $\mathrm{Homgr}_A(L(M), I(N))$ est un complexe de $(B, B')$-bimodules, de sorte que $\mathrm{Ext}_A(M, N)$ est muni d’une structure naturelle de $(B, B')$-bimodule gradué ; sur le terme de degré 0, cette structure coïncide avec celle de $\mathrm{Hom}_A(M, N)$ (II, p. 35).
Si $\lambda \in B, \lambda' \in B'$ et si on note $\lambda_M, \lambda'_N, \lambda_E, \lambda'_E$ les homothéties $x \mapsto x\lambda, y \mapsto y\lambda', z \mapsto \lambda z, z \mapsto z\lambda'$ de $M, N, \mathrm{Ext}_A(M, N), \mathrm{Ext}_A(M, N)$ respectivement, on a alors

$$
\lambda_E = \mathrm{Ext}_A(\lambda_M, 1), \quad \lambda'_E = \mathrm{Ext}(1, \lambda'_N),
$$

ce qui fournit une autre description de la structure de bimodule de $\mathrm{Ext}_A(M, N)$.
Nous laissons au lecteur le soin de généraliser les n°s 4 et 6 au cas des complexes de multimodules.
Soient $C, C', C''$ des complexes de $A$-modules. La composition des applications définit un homomorphisme gradué de degré zéro :

(14)
$$
\mathrm{Homgr}_A(C', C'') \otimes_k \mathrm{Homgr}_A(C, C') \to \mathrm{Homgr}_A(C, C'').
$$

Soient B, B', E des anneaux, C, C', C'' des complexes de (B', A)-bimodules, (A, E)-bimodules, (B, E)-bimodules respectivement. Par restriction de l'isomorphisme canonique de II, p. 73, on obtient un homomorphisme bijectif de (B, B')-bimodules :

(15) $\operatorname{Homgr}_E(C \otimes_A C', C'') \to \operatorname{Homgr}_A(C, \operatorname{Homgr}_E(C', C''))$.

Soient enfin B un anneau, C un complexe de B-modules à droite, C' un complexe de A-modules à droite, C'' un complexe de (B, A)-bimodules. On déduit des homomorphismes canoniques (II. p. 75)

$$
C_p \otimes_B \operatorname{Hom}_A(C'_q, C''_r) \to \operatorname{Hom}_A(C'_q, C_p \otimes_B C''_r)
$$

un homomorphisme gradué de degré zéro :

(16) $C \otimes_B \operatorname{Homgr}_A(C', C'') \to \operatorname{Homgr}_A(C', C \otimes_B C'')$.

Cet homomorphisme est bijectif lorsque C est un module projectif de type fini (II, p. 75, prop. 2).

#### Proposition 12 {#alg-x-s5-prop-12 .statement}

Les homomorphismes (14), (15), (16) sont des morphismes de complexes.

Démontrons-le par exemple pour l'homomorphisme (14). Notons

$$
\kappa : \operatorname{Homgr}_A(C', C'') \otimes_k \operatorname{Homgr}_A(C, C') \to \operatorname{Homgr}_A(C, C'')
$$

cet homomorphisme. Soient $f \in \operatorname{Homgr}_A(C', C'')_p$ et $g \in \operatorname{Homgr}_A(C, C')_q$; on a alors par définition $\kappa(f \otimes g) = f \circ g$. De plus :

$$
\mathrm{D}(f \otimes g) = \mathrm{D}f \otimes g + (-1)^p f \otimes \mathrm{D}g = (d'' \circ f) \otimes g - (-1)^p (f \circ d') \otimes g +
+ (-1)^p f \otimes (d' \circ g) - (-1)^{p+q} f \otimes (g \circ d),
$$

d'où

$$
\kappa(\mathrm{D}(f \otimes g)) = d'' \circ f \circ g - (-1)^p f \circ d' \circ g +
+ (-1)^p f \circ d' \circ g - (-1)^{p+q} f \circ g \circ d \\
= d'' \circ f \circ g - (-1)^{p+q} f \circ g \circ d = \mathrm{D}(f \circ g) = \mathrm{D}(\kappa(f \otimes g)).
$$

On démontre de même que les homomorphismes (15) et (16) sont des morphismes de complexes.

On déduit du morphisme (14) des homomorphismes de $k$-modules (X, p. 62)

(17) $\mathrm{H}^p(\operatorname{Homgr}_A(C', C'')) \otimes_k \mathrm{H}^q(\operatorname{Homgr}_A(C, C')) \to \mathrm{H}^{p+q}(\operatorname{Homgr}_A(C, C''))$.

Faisant $C = A$, on voit que l'homomorphisme :

(18) $\operatorname{Homgr}_A(C', C'') \otimes_k C' \to C''$ qui applique $f \otimes x$ sur $f(x)$ est un morphisme de complexes de $A$-modules à gauche ; il lui est associé un homomorphisme canonique ($X$, p. 80) de $A$-modules gradués $\gamma : H(\mathrm{Homgr}_A(C', C'')) \otimes_k H(C') \to H(C'')$, qui correspond à l’homomorphisme canonique de $k$-modules

$$
\lambda : H(\mathrm{Homgr}_A(C', C'')) \to \mathrm{Homgr}_A(H(C'), H(C''))
$$

## EXERCICES {#alg-x-s5-exercises}

See the [exercises for § 5](exercises/s5/).
