---
book: alg
book_title: Algebra
chapter: X
chapter_title: ALGÈBRE HOMOLOGIQUE
section: 7
section_title: Produit de composition
lang: en
source: alg-x-fr
book_pages: A X.113-A X.134, A X.197-A X.202
pdf_pages: 0119-0140, 0203-0208
extraction: ocr
subsections:
    - "no": 1
      title: L’homomorphisme $\mathrm{Ext}_A(N, P) \otimes \mathrm{Ext}_A(M, N) \to \mathrm{Ext}_A(M, P)$
      page: 113
      pdf_page: 119
    - "no": 2
      title: Les sept calculs du produit de composition
      page: 115
      pdf_page: 121
    - "no": 3
      title: La classe associée à une suite exacte
      page: 116
      pdf_page: 122
    - "no": 4
      title: Propriétés de la classe associée à une suite exacte
      page: 118
      pdf_page: 124
    - "no": 5
      title: Relation entre suites exactes et éléments de $\mathrm{Ext}_A(M, N)$
      page: 121
      pdf_page: 127
    - "no": 6
      title: Produit de composition et homomorphismes de liaison des modules d’extensions
      page: 125
      pdf_page: 131
    - "no": 7
      title: L’homomorphisme $\mathrm{Ext}_A(P, Q) \otimes \mathrm{Tor}^A(P, M) \to \mathrm{Tor}^A(Q, M)$
      page: 128
      pdf_page: 134
    - "no": 8
      title: Produits de composition et homomorphismes de liaison des produits de torsion
      page: 130
      pdf_page: 136
    - "no": 9
      title: Calcul des produits de composition par décalage de résolutions
      page: 132
      pdf_page: 138
statements: 34
exercises: 11
content_sha256: 7e4ae25ed21a48d4bbe1a0c05879d017dc278aa2aa837d499da6ec6fda46b955
translated_from: content/fr/alg/X/07_s7_produit_de_composition.md
source_lang: fr
translation_method: machine
source_content_sha256: 8030f2c6ec5b3b69eb251de1fd3bb272ebbe075c7b637f8643776b9f19219334
translation_model: laguna-s-2.1-free, hy3-free, gpt-5-mini
translation_run: translate-en-mt-71c9c53e
glossary_version: 34
glossary_terms_sha256: f4a4017097f8eea157b34f1309e4365164fca37744cec533cd038752055a4d12
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 7. COMPOSITION PRODUCT

*We follow the general conventions of §4.*

### 1. The homomorphism $\mathrm{Ext}_A(N, P) \otimes \mathrm{Ext}_A(M, N) \to \mathrm{Ext}_A(M, P)$

Let $M$ and $N$ be two left $A$-modules. Consider the homomorphisms $p_M : L(M) \to M$, $e_M : M \to I(M)$, and $e_M \circ p_M : L(M) \to I(M)$; by Prop. 4 of X, p. 86, we deduce from this a *bijective* homomorphism

$$
a_{M,N} = H(\mathrm{Homgr}_A(e_M \circ p_M, 1)) : H(\mathrm{Homgr}_A(I(M), I(N))) \to \mathrm{Ext}_A(M, N) .
$$

Recall also (X, p. 82) that $H^n(\mathrm{Homgr}_A(I(M), I(N)))$ is the set of homotopy classes of degree-increasing morphisms from the complex $I(M)$ to the complex $I(N)$. For example, if $f \in \mathrm{Hom}_A(M, N)$, the homotopy class of $I(f)$ is sent by $a_{M,N}$ to $f$.

If $P$ is a third left $A$-module, we have by X, p. 99, a canonical $k$-homomorphism

$$
H(\mathrm{Homgr}_A(I(N), I(P))) \otimes_k H(\mathrm{Homgr}_A(I(M), I(N))) \to H(\mathrm{Homgr}_A(I(M), I(P)))
$$

from which we deduce by transport via the isomorphisms $a_{N,P}$, $a_{M,N}$, $a_{M,P}$ a $k$-homomorphism (called the *composition homomorphism*):

$$
c_{M,N,P}: \mathrm{Ext}_A(N, P) \otimes_k \mathrm{Ext}_A(M, N) \to \mathrm{Ext}_A(M, P)
$$

This corresponds to a *bilinear mapping*

(1)

$$
\mathrm{Ext}_A(N, P) \times \mathrm{Ext}_A(M, N) \to \mathrm{Ext}_A(M, P)
$$

which decomposes into homogeneous components

(2)

$$
\mathrm{Ext}_A^i(N, P) \times \mathrm{Ext}_A^j(M, N) \to \mathrm{Ext}_A^{i+j}(M, P)
$$

If $u \in \mathrm{Ext}_A(N, P)$, $v \in \mathrm{Ext}_A(M, N)$, the image of $(u, v)$ under (1) is called the *composition product of $u$ and $v$* and is denoted $u \circ v$. If $g$ (resp. $f$) is a degree-increasing morphism of degree $j$ (resp. $i$) from $I(M)$ to $I(N)$ (resp. from $I(N)$ to $I(P)$), whose homotopy class is $\bar{g}$ (resp. $\bar{f}$), then the composition product $a_{N,P}(\bar{f}) \circ a_{M,N}(\bar{g})$ is the image under $a_{M,P}$ of the homotopy class of the morphism $f \circ g$ from $I(M)$ to $I(P)$.

#### Example 1 {#alg-x-s7-n1-exa-1 .statement}

If $u \in \mathrm{Hom}_A(N, P)$, $v \in \mathrm{Hom}_A(M, N)$, then $u \circ v$ is the composite of $u$ and $v$.

#### Example 2 {#alg-x-s7-n1-exa-2 .statement}

If $u \in \mathrm{Hom}_A(N, P)$, $v \in \mathrm{Ext}_A(M, N)$, then

$$
u \circ v = \mathrm{Ext}_A(l_M, u)(v) \in \mathrm{Ext}_A(M, P):
$$

analogously, if $u \in \mathrm{Ext}_A(N, P)$, $v \in \mathrm{Hom}_A(M, N)$, then

$$
u \circ v = \mathrm{Ext}_A(v, l_P)(u) \in \mathrm{Ext}_A(M, P).
$$

This follows from the definitions and the remarks of X. p. 88.

If $Q, M, N, P$ are four left $A$-modules, and if

$$
u \in \mathrm{Ext}_A(N, P), \quad v \in \mathrm{Ext}_A(M, N), \quad w \in \mathrm{Ext}_A(Q, M),
$$

then $(u \circ v) \circ w = u \circ (v \circ w)$: the composition product is *associative*; we will therefore denote the composition of several elements without parentheses. In particular, by Example 2:

#### Example 3 {#alg-x-s7-n1-exa-3 .statement}

Let $M, N, M', N'$ be four left $A$-modules. If $u \in \mathrm{Ext}_A(M, N)$, $f \in \mathrm{Hom}_A(M', M)$, $g \in \mathrm{Hom}_A(N, N')$, then

(3)

$$
\mathrm{Ext}_A(f, g)(u) = g \circ u \circ f \in \mathrm{Ext}_A(M', N').
$$

This provides a new proof of the $k$-bilinearity of the mapping $(f, g) \to \mathrm{Ext}_A(f, g)$ (X, p. 88, Prop. 6).

### 2. Seven calculations of the composition product

==========

Let $M$, $M'$ and $M''$ be three left $A$-modules, $a : R \to M$, $a' : R' \to M'$ and $a'' : R'' \to M''$ projective resolutions, $c : M \to E$, $c' : M' \to E'$ and $c'' : M'' \to E''$ injective resolutions. It follows from X, p. 100, Th. 1 and p. 103, Prop. 2, that the diagram :

$$
\begin{array}{cccccc}
H(\mathrm{Homgr}_A(M, E')) & \longrightarrow & H(\mathrm{Homgr}_A(R, E')) & \longrightarrow & H(\mathrm{Homgr}_A(R, M')) \\
\uparrow & & \downarrow & & \uparrow \\
H(\mathrm{Homgr}_A(E, E')) & \xrightarrow{\varphi(E, E')} & \mathrm{Ext}_A(M, M') & \xleftarrow{\varphi(R, R')} & H(\mathrm{Homgr}_A(R, R')) \\
& \swarrow_{\varphi(M, E')} & & \searrow^{\varphi(R, M')} & \\
& & H(\mathrm{Homgr}_A(R, E')) & &
\end{array}
$$

where the unlabeled arrows are deduced canonically from $c, a, c', a'$, is commutative, and that all the arrows are isomorphisms, which gives five descriptions of $\mathrm{Ext}_A(M, M')$. Analogously, one obtains five descriptions of $\mathrm{Ext}_A(M', M'')$, and as many of $\mathrm{Ext}_A(M, M'')$.

Consider now the seven composition homomorphisms

$$
H(\mathrm{Homgr}_A(C', C'')) \otimes_k H(\mathrm{Homgr}_A(C, C')) \to H(\mathrm{Homgr}_A(C, C''))
$$

where one takes successively for $(C, C', C'')$ the seven triplets $(R, R', R''), (R, R', M''), (R, R', E''), (R, M', E''), (R, E', E''), (M, E', E''), (E, E', E'')$.

![Diagram of the seven computations of the composition product](https://i.imgur.com/3Q5z5QG.png)

Fig. 1.

Identifying $H(\mathrm{Homgr}_A(C, C'))$ with $\mathrm{Ext}(M, M')$ by the isomorphism above, and analogously for $H(\mathrm{Homgr}_A(C', C''))$ and $H(\mathrm{Homgr}_A(C, C''))$, one obtains *seven homomorphisms*

$$
\mathrm{Ext}_A(M', M'') \otimes_k \mathrm{Ext}_A(M, M') \to \mathrm{Ext}_A(M, M'')
$$

These seven homomorphisms coincide, and are independent of the choice of resolutions. In particular, they coincide with the homomorphism which was defined in No. 2, via the triplet $(I(M), I(M'), I(M''))$. This follows indeed from the interpretation of the modules H(Homgr $(C, C')$) as module of homotopy classes of morphisms of complexes of C into C’, and from the fact that if in a diagram of complexes

$$
\begin{array}{ccccc}
C & \xrightarrow{\ f\ } & C' & \xrightarrow{\ g\ } & C''\\
\downarrow\scriptstyle{\alpha} & & \downarrow\scriptstyle{\alpha'} & & \downarrow\scriptstyle{\alpha''}\\
C_1 & \xrightarrow{\ f_1\ } & C'_1 & \xrightarrow{\ g_1\ } & C''_1
\end{array}
$$

$\alpha'' \circ g$ is homotopic to $g_1 \circ \alpha'$ and $\alpha' \circ f$ homotopic to $f_1 \circ \alpha$, then $\alpha'' \circ g \circ f$ is homotopic to $g_1 \circ f_1 \circ \alpha$ (X, p. 33, Prop. 4 and Cor.).

In what follows, we shall use according to the case one or the other of the seven preceding constructions of the composition homomorphisms.

### 3. The class associated with an exact sequence

#### Proposition 1 {#alg-x-s7-prop-1 .statement}

Let $(C,d)$ and $(C',d')$ be two complexes of left $A$-modules and $n,p,q$ three integers such that $p \geq q$. For $p \geq i \geq q-1$, let $f_i:C_i\longrightarrow C'_{i+n+1}$ be a homomorphism of $A$-modules such that $f_p\circ d=0$, $f_i\circ d=d'\circ f_{i+1}$ for $p>i\geq q-1$, and $d'\circ f_{q-1}=0$ (see fig. 2).

$$
\begin{array}{ccccccccccccc}
C_{p+1}&\xrightarrow{\ d\ }&C_p&\xrightarrow{\ d\ }&C_{p-1}&\xrightarrow{\ d\ }&\cdots&\xrightarrow{\ d\ }&C_q&\xrightarrow{\ d\ }&C_{q-1}&\xrightarrow{\ d\ }&C_{q-2}\\
0\downarrow&&\downarrow f_p&&\downarrow f_{p-1}&&&&\downarrow f_q&&\downarrow f_{q-1}&&\downarrow 0\\
C'_{p+n+2}&\xrightarrow{\ d'\ }&C'_{p+n+1}&\xrightarrow{\ d'\ }&C'_{p+n}&\xrightarrow{\ d'\ }&\cdots&\xrightarrow{\ d'\ }&C'_{q+n+1}&\xrightarrow{\ d'\ }&C'_{q+n}&\xrightarrow{\ d'\ }&C'_{q+n-1}
\end{array}
$$

Fig. 2.

Set $\alpha=f_{p-1}\circ d=d'\circ f_p$, $\beta=f_{q-1}\circ d=d'\circ f_q$, and let $a$ (resp. $b$) be the graded $A$-homomorphism of degree $n$ from $C$ into $C'$ whose only non-zero bi-homogeneous component is $\alpha$ (resp. $\beta$). Then one has $a\in Z_n(\operatorname{Homgr}_A(C,C'))$, $b\in Z_n(\operatorname{Homgr}_A(C,C'))$ and

$$
a-(-1)^{(n+1)(p-q)}b\in B_n(\operatorname{Homgr}_A(C,C')).
$$

One has $d'\circ\alpha=d'\circ f_{p-1}\circ d=0$, $\alpha\circ d=f_{p-1}\circ d\circ d=0$, so

$$
a\in Z_n(\operatorname{Homgr}_A(C,C')) ;
$$

Analogously $b\in Z_n(\operatorname{Homgr}_A(C,C'))$. Set $\varepsilon=(-1)^{n+1}$. We have, in the complex $\operatorname{Homgr}_A(C,C')$ the relations

$$
Df_{p-1}=d'\circ f_{p-1}-\varepsilon f_{p-1}\circ d=f_{p-2}\circ d-\varepsilon\alpha
$$

$$
Df_i=d'\circ f_i-\varepsilon f_i\circ d=f_{i-1}\circ d-\varepsilon f_{i+1}\circ d\qquad (p-1>i>q)
$$

$$
Df_q=d'\circ f_q-\varepsilon f_q\circ d=\beta-\varepsilon f_q\circ d .
$$

thence

$$
\sum_{i=1}^{p-q} \varepsilon^i Df_{p-i} = \varepsilon^{p-q} \beta - \alpha,
$$

which proves the lemma.

Consider two left A-modules M and N and an exact sequence of A-modules

(4)
$$
0 \to N \to R_n \to R_{n-1} \to \ldots \to R_1 \to M \to 0.
$$

By prop. 3 and 3 bis of X, p. 49, there exists a commutative diagram:

(5)

$$
\begin{array}{ccccccccccccc}
0 & \longrightarrow & N & \xrightarrow{e_N} & I^0(N) & \longrightarrow & \ldots & \longrightarrow & I^{n-1}(N) & \xrightarrow{\delta^{n-1}} & I^n(N) & \xrightarrow{\delta^n} & I^{n+1}(N) \\
& & \uparrow & & \uparrow & & & & \uparrow & & \uparrow & & \uparrow \\
0 & \longrightarrow & N & \longrightarrow & R_n & \longrightarrow & \ldots & \longrightarrow & R_1 & \longrightarrow & M & \longrightarrow & 0 \\
& & \uparrow & & \uparrow & & & & \uparrow & & \uparrow & & \uparrow \\
L_{n+1}(M) & \xrightarrow{d_{n+1}} & L_n(M) & \xrightarrow{d_n} & L_{n-1}(M) & \longrightarrow & \ldots & \xrightarrow{d_1} & L_0(M) & \xrightarrow{p_M} & M & \longrightarrow & 0.
\end{array}
$$

Consider the two elements $b$ and $a$ of $\mathrm{Homgr}_A(L(M), I(N))$ whose only non-zero bihomogeneous components are

$$
b^n = e_N \circ u_n : L_n(M) \to I^0(N) \quad \text{and} \quad a^n = v^n \circ p_M : L_0(M) \to I^n(N)
$$

respectively.

#### Proposition 2 {#alg-x-s7-prop-2 .statement}

*We have* $a, b \in Z^n(\mathrm{Homgr}_A(L(M), I(N)))$. *Moreover*, the classes $\overline{a}$ and $\overline{b}$ of $a$ and $b$ in $H^n(\mathrm{Homgr}_A(L(M), I(N))) = \mathrm{Ext}_A^n(M, N)$ depend only on the exact sequence (4) and are equal.

By prop. 1, applied to the two extreme rows of (5) and to the composed vertical arrows, with $p = n, q = 0$, we have $a, b \in Z^n(\mathrm{Homgr}_A(I(M), L(N)))$ and

$$
a - b = a - (-1)^{(n+1)n} b \in B^n(\mathrm{Homgr}_A(L(M), I(N))) .
$$

Since $a$ (resp. $b$) is independent of the choice of $u$ (resp. $v$), the element $\overline{a} = \overline{b}$ of $\mathrm{Ext}_A^n(M, N)$ is independent of the choice of the morphisms $u$ and $v$, whence the proposition.

#### Definition 1 {#alg-x-s7-def-1 .statement}

*We call the class associated with the exact sequence* (4) *the element* $\theta$ *of* $\mathrm{Ext}_A^n(M, N)$ *defined by* $\theta = (-1)^{n(n+1)/2} \overline{a} = (-1)^{n(n+1)/2} \overline{b}$.

#### Remark 1 {#alg-x-s7-n3-rem-1 .statement}

Let (P, p) be a projective resolution of M. By X, p. 49. prop. 3, there exists a commutative diagram

$$
\begin{array}{ccccccccccccc}
0 & \longrightarrow & N & \longrightarrow & R_n & \longrightarrow & \ldots & \longrightarrow & R_1 & \longrightarrow & M & \longrightarrow & 0 \\
& & \uparrow & & \uparrow & & & & \uparrow & & \uparrow & & \uparrow \\
P_n & \longrightarrow & P_{n-1} & \longrightarrow & \ldots & \longrightarrow & P_0 & \xrightarrow{p} & M & \longrightarrow & 0.
\end{array}
$$

With the notations of § 6, θ is the image under φ(P, N) of the homotopy class of the morphism P → N defined by (−1)^{n(n+1)/2} \tilde{u}_n. Analogously, if (e, E) is an injective resolution of N, there exists a commutative diagram

$$
\begin{array}{cccccccccccc}
0 & \longrightarrow & N & \longrightarrow & E^0 & \longrightarrow & \ldots \longrightarrow & E^{n-1} & \longrightarrow & E^n \\
& & ^{1_N}\uparrow & & ^{\tilde{v}^0}\uparrow & & & ^{\tilde{v}^{n-1}}\uparrow & & ^{\tilde{v}^n}\uparrow \\
0 & \longrightarrow & N & \longrightarrow & R_n & \longrightarrow & \ldots \longrightarrow & R_1 & \longrightarrow & M & \longrightarrow & 0 .
\end{array}
$$

and θ is the image under φ(M, E) of the homotopy class of the morphism M → E defined by (−1)^{n(n+1)/2} v^n. This follows from the construction of θ and the definitions of φ(P, N) and φ(M, E).

#### Remark 2 {#alg-x-s7-n3-rem-2 .statement}

When $n = 0$, the exact sequence (4) reads $0 \to N \xrightarrow{f} M \to 0$, and the associated class is $f^{-1} \in \mathrm{Hom}_A(M, N) = \mathrm{Ext}^0_A(M, N)$.

### 4. Properties of the class associated with an exact sequence

#### Proposition 3 {#alg-x-s7-prop-3 .statement}

Let

(6)
$$
0 \to P \to S_m \to S_{m-1} \to \ldots \to S_1 \xrightarrow{\lambda} N \to 0
$$
(7)
$$
0 \to N \twoheadrightarrow R_n \to R_{n-1} \to \ldots \to R_1 \to M \to 0
$$
be two exact sequences of left A-modules with respective classes θ ∈ Ext^m_A(N, P) and θ' ∈ Ext^n_A(M, N). The class in Ext^{m+n}_A(M, P) associated with the exact sequence (8)
$$
0 \to P \to S_m \to \ldots \to S_1 \xrightarrow{\mu \circ \lambda} R_n \to \ldots \to R_1 \to M \to 0
$$
is the composition product θ ∘ θ'.

Choose commutative diagrams

$$
\begin{array}{cccccccccccc}
0 & \longrightarrow & P & \longrightarrow & I^0(P) & \longrightarrow & \ldots \longrightarrow & I^{m-1}(P) & \xrightarrow{\delta_P^{m-1}} & I^m(P) \\
& & ^{l_P}\uparrow & & ^{w^0}\uparrow & & & ^{w^{m-1}}\uparrow & & ^{w^m}\uparrow \\
0 & \longrightarrow & P & \longrightarrow & S_m & \longrightarrow & \ldots \longrightarrow & S_1 & \xrightarrow{\lambda} & N & \longrightarrow & 0 ,
\end{array}
$$
$$
\begin{array}{cccccccccccc}
0 & \longrightarrow & N & \xrightarrow{e_N} & I^0(N) & \longrightarrow & \ldots \longrightarrow & I^{n-1}(N) & \longrightarrow & I^n(N) \\
& & ^{1_N}\uparrow & & ^{v^0}\uparrow & & & ^{v^{n-1}}\uparrow & & ^{v^n}\uparrow \\
0 & \longrightarrow & N & \xrightarrow{\mu} & R_n & \longrightarrow & \ldots \longrightarrow & R_1 & \longrightarrow & M & \longrightarrow & 0 .
\end{array}
$$

Since $I^m(P)$ is injective, there exists a homomorphism $h^0 \colon I^0(N) \rightarrow I^m(P)$ such that $w^m = h^0 \circ e_N$; according to X, p. 49, Proposition 3 bis, $h^0$ extends to a morphism of complexes $h \colon I(N) \rightarrow I(P)\, (-m)$. Thus $w^m = h^0 \circ e_N = h^0 \circ v^0 \circ \mu$, hence
$$
\delta_I^{m-1} \circ w^{m-1} = w^m \circ \lambda = h^0 \circ v^0 \circ (\mu \circ \lambda),
$$

and the following diagram is commutative:

$$
\begin{array}{ccccccccccccccccccc}
0&\longrightarrow&P&\longrightarrow&I^0(P)&\longrightarrow&\cdots&\longrightarrow&I^{m-1}(P)&\longrightarrow&I^m(P)&\longrightarrow&I^{m+1}(P)&\longrightarrow&\cdots&\longrightarrow&I^{m+n}(P)\\
&&\uparrow^{i_P}&&\uparrow^{w^0}&&&&\uparrow^{w^{m-1}}&&\uparrow^{t^0}&&\uparrow^{t^1}&&&&\uparrow^{t^n}\\
0&\longrightarrow&P&\longrightarrow&S_m&\longrightarrow&\cdots&\longrightarrow&S_1&\xrightarrow[\mu\circ\lambda]{}&R_n&\longrightarrow&R_{n-1}&\longrightarrow&\cdots&\longrightarrow&M&\longrightarrow&0
\end{array}
$$

where $t^0=h^0\circ v^0$, $t^1=(-1)^m h^1\circ v^1$, $\ldots$, $t^i=(-1)^{mi}h^i\circ v^i$, $\ldots$, $t^n=(-1)^{mn}h^n\circ v^n$.

The class $\theta$ associated to (6) is that of $(-1)^{m(m+1)/2}w^m\in\operatorname{Homgr}_A^m(N,I(P))$, corresponding by the isomorphism $\alpha_{N,P}$ to the class of $(-1)^{m(m+1)/2}h\in\operatorname{Homgr}_A^m(I(N),I(P))$; the class $\theta'$ associated to (7) is that of $(-1)^{n(n+1)/2}v^n\in\operatorname{Homgr}^n(M,I(N))$, the class associated to (8) is that of $(-1)^{(m+n)(m+n+1)/2}t^n\in\operatorname{Homgr}^{m+n}(M,I(P))$, hence the conclusion, according to the definition of the composition product (X, p. 114) and the formula

$$
m(m+1)/2+n(n+1)/2=(m+n)(m+n+1)/2-mn.
$$

4. — Considérons un diagramme commutatif de $A$-modules à lignes exactes

$$
\begin{array}{ccccccccccccccc}
0&\longrightarrow&N&\longrightarrow&R_n&\longrightarrow&R_{n-1}&\longrightarrow&\cdots&\longrightarrow&R_1&\longrightarrow&M&\longrightarrow&0\\
&&\downarrow^{g}&&\downarrow&&\downarrow&&&&\downarrow&&\downarrow^{f}&&\\
0&\longrightarrow&N'&\longrightarrow&R'_n&\longrightarrow&R'_{n-1}&\longrightarrow&\cdots&\longrightarrow&R'_1&\longrightarrow&M'&\longrightarrow&0.
\end{array}
$$

Let $\theta$ (resp. $\theta'$) be the class of the first (resp. second) row in

$$
\operatorname{Ext}_A^n(M,N)\quad\text{(resp. }\operatorname{Ext}_A^n(M',N')\text{)}.
$$

In $\operatorname{Ext}_A^n(M,N')$, we have $\theta'\circ f=g\circ\theta$.

Indeed, consider a commutative diagram

$$
\begin{array}{ccccccccccccc}
L_n(M)&\xrightarrow{d_n}&L_{n-1}(M)&\longrightarrow&\cdots&\longrightarrow&L_0(M)&\xrightarrow{p_M}&M&\longrightarrow&0\\
\downarrow^{u_n}&&\downarrow&&&&\downarrow&&\downarrow^{1}\\
0&\longrightarrow&N&\longrightarrow&R_n&\longrightarrow&\cdots&\longrightarrow&R_1&\longrightarrow&M&\longrightarrow&0\\
&&\downarrow^{g}&&\downarrow&&&&\downarrow&&\downarrow^{f}\\
0&\longrightarrow&N'&\longrightarrow&R'_n&\longrightarrow&\cdots&\longrightarrow&R'_1&\longrightarrow&M'&\longrightarrow&0\\
&&\downarrow&&\downarrow&&&&\downarrow&&\downarrow^{v^n}\\
0&\longrightarrow&N'&\xrightarrow{\epsilon_{N'}}&I^0(N')&\xrightarrow{\delta^0}&\cdots&\longrightarrow&I^{n-1}(N')&\xrightarrow{\delta^{n-1}}&I^n(N')
\end{array}
$$

By definition, $\theta'\circ f$ is the class of $(-1)^{n(n+1)/2}v^n\circ f\circ p_M\in\operatorname{Homgr}^n(L(M),I(N'))$, while $g\circ\theta$ is the class of $(-1)^{n(n+1)/2}\epsilon_{N'}\circ g\circ u_n$. According to Lemma 1, applied to the two extreme lines of the diagram, these two classes are equal.

#### Corollary 1 {#alg-x-s7-prop-3-cor-1 .statement}

Consider a commutative diagram with exact rows

$$
\begin{array}{cccccccccccc}
0 & \rightarrow & N & \rightarrow & R_n & \rightarrow & \cdots \rightarrow & R_1 & \rightarrow & M & \rightarrow & 0 \\
\downarrow & & \downarrow & & \downarrow & & & \downarrow & & \downarrow & & \downarrow \\
0 & \rightarrow & N & \rightarrow & R'_n & \rightarrow & \cdots \rightarrow & R'_1 & \rightarrow & M & \rightarrow & 0 ;
\end{array}
$$

the two rows of the diagram have the same associated class in $\mathrm{Ext}_A^n(M, N)$.

#### Corollary 2 {#alg-x-s7-prop-3-cor-2 .statement}

Let

$$
0 \to N \xrightarrow{f_{n-1}} R_n \xrightarrow{f_n} R_{n-1} \to \cdots \xrightarrow{f_2} R_1 \xrightarrow{f_1} M \to 0
$$

be an exact sequence, $\theta \in \mathrm{Ext}_A^n(M, N)$ its associated class, $a_1, \ldots, a_{n+1}$ invisible elements of $k$. The associated class of the exact sequence

$$
0 \to N \xrightarrow{a_{n+1} f_{n+1}} R_n \xrightarrow{a_n f_n} R_{n-1} \to \cdots \xrightarrow{a_2 f_2} R_1 \xrightarrow{a_1 f_1} M \to 0
$$

is $(a_1^{-1}\, a_2^{-1}\, \ldots\, a_{n+1}^{-1})\ \theta$.

Indeed, there is a commutative diagram

$$
\begin{array}{ccccccccccccccc}
0 & \rightarrow & N & \xrightarrow{a_{n+1} f_{n+1}} & R_n & \rightarrow & \cdots & \rightarrow & R_2 & \xrightarrow{a_2 f_2} & R_1 & \xrightarrow{a_1 f_1} & M & \rightarrow & 0 \\
& & \downarrow a_1 \ldots a_{n+1} & & \downarrow a_1 \ldots a_n & & & \downarrow a_1 a_2 & & \downarrow a_1 & & \downarrow 1 \\
0 & \rightarrow & N & \xrightarrow{f_{n+1}} & R_n & \rightarrow & \cdots & \rightarrow & R_2 & \xrightarrow{f_2} & R_1 & \xrightarrow{f_1} & M & \rightarrow & 0 .
\end{array}
$$

and we apply the proposition.

#### Corollary 3 {#alg-x-s7-prop-3-cor-3 .statement}

Let $0 \to N \xrightarrow{f_{n-1}} R_n \xrightarrow{f_n} \cdots \to R_1 \xrightarrow{f_1} M \to 0$ be an exact sequence, $\theta$ its class in $\mathrm{Ext}_A^n(M, N)$, $u \colon M' \to M$ and $v \colon N \to N'$ homomorphisms of $A$-modules.

a) The element $v \circ \theta$ of $\mathrm{Ext}_A^n(M, N')$ is equal to the class of the exact sequence

$$
0 \to N' \xrightarrow{f_{n'+1}} R'_n \xrightarrow{f_{n'}} R_{n-1} \xrightarrow{f_{n-1}} \cdots \to R_1 \to M \to 0 ,
$$

where $R'_n$ is the $A$-quotient module of $R_n \oplus N'$ by the submodule formed by the pairs $(f_{n+1}(x), -v(x))$ for $x \in N$, and where $f_{n'+1}'$ (resp. $f_{n'}'$) is deduced from the canonical injection (resp. from $(f_n, 0)$) by passing to quotients.

b) The element $\theta \circ u$ of $\mathrm{Ext}_A^n(M', N)$ is the class of the exact sequence

$$
0 \to N \to R_n \to \cdots \to R_2 \xrightarrow{f_2''} R'_1 \xrightarrow{f_1''} M' \to 0 ,
$$

where $R'_1$ is the fibre product $R_1 \times_M M'$, that is to say (I, p. 44) the submodule of $R_1 \times M'$ formed by the pairs $(x, y)$ such that $f_1(x) = u(y)$, and where $f_2''$ (resp. $f_1''$) is deduced from $(f_2, 0)$ (resp. from the second projection).

Let us prove for example $a$. Let $z$ be an element of $R'_n$ such that $f'_n(z) = 0$; if $z$ is the class of a pair $(x, y)$, with $x \in R_n$, $y \in N'$, one has $f_n(x) = 0$, so that there exists an element $t \in N$ such that $x = f_{n+1}(t)$. Then one has $z = f'_{n+1}(y + v(t))$, which proves that $\mathrm{Ker}\ f'_n = \mathrm{Im}\ f'_{n+1}$. The injectivity of $f'_{n+1}$ follows from that of $f_{n+1}$.

Let $j : R_n \to R'_n$ be the homomorphism deduced from the canonical injection; one has a commutative diagram of exact sequences:

$$
\begin{array}{ccccccccccccc}
0 & \longrightarrow & N & \xrightarrow{f_{n+1}} & R_n & \xrightarrow{f_n} & R_{n-1} & \longrightarrow & \ldots & \longrightarrow & M & \longrightarrow & 0 \\
& & \downarrow v & & \downarrow j & & \downarrow 1 & & & & \downarrow 1 & & \\
0 & \longrightarrow & N' & \xrightarrow{f'_{n+1}} & R'_n & \xrightarrow{f'_n} & R'_{n-1} & \longrightarrow & \ldots & \longrightarrow & M & \longrightarrow & 0 ;
\end{array}
$$

assertion $a$ then follows from the proposition.

The proof of $b$ is analogous.

#### Remark {#alg-x-s7-n4-rem-1 .statement}

Let $\theta \in \mathrm{Ext}^n_A(M, N)$, resp. $\theta' \in \mathrm{Ext}^n_A(M', N')$, be the class of an exact sequence

$$
0 \to N \xrightarrow{f_{n+1}} R_n \to \ldots \to R_1 \xrightarrow{f_1} M \to 0,
$$
resp. $0 \to N' \xrightarrow{f'_{n+1}} R'_n \to \ldots \to R'_1 \xrightarrow{f'_1} M' \to 0.$

Let $i_N,\ i_{N'}$, be the canonical injections of $N$ and $N'$ into $N \oplus N'$, $q_M,\ q_{M'}$, the projections of $M \oplus M'$ onto $M$ and $M'$. Consider the homomorphism

$$
m = \mathrm{Ext}\,(q_M,\ i_N) \oplus \mathrm{Ext}\,(q_{M'},\ i_{N'})
$$

from $\mathrm{Ext}_A(M, N) \oplus \mathrm{Ext}_A(M', N')$ into $\mathrm{Ext}_A(M \oplus M', N \oplus N')$. *The element*

$$
m(\theta, \theta') = i_N \circ \theta \circ q_M + i_{N'} \circ \theta' \circ q_{M'}
$$

*is the class of the exact sequence*

$$
0 \to N \oplus N' \xrightarrow{f_{n-1} \oplus f'_{n-1}} R_n \oplus R'_n \to \ldots \to R_1 \oplus R'_1 \xrightarrow{f_1 \oplus f'_1} M \oplus M' \to 0 .
$$

Indeed, if one denotes this class by $\theta''$, it follows from prop. 4 that one has

$$
\theta'' \circ i_M = i_N \circ \theta = m(\theta, \theta') \circ i_M \quad \text{and} \quad \theta'' \circ i_{M'} = i_{N'} \circ \theta = m(\theta, \theta') \circ i_{M'} ;
$$

by X, p. 89, prop. 7, this entails $\theta'' = m(\theta, \theta')$.

### 5. Relation between exact sequences and elements of $\mathrm{Ext}_A(M, N)$

#### Theorem 1 {#alg-x-s7-thm-1 .statement}

*Let $n$ be an integer $\geqslant 1$, $M$ and $N$ two $A$-modules.*

a) *Every element of $\mathrm{Ext}^n_A(M, N)$ is the class of an exact sequence* (X, p. 117, def. 1).

b) *Let* $0 \to N \xrightarrow{f_{n+1}} R_n \xrightarrow{f_n} \ldots \to R_1 \xrightarrow{f_1} M \to 0$ and $0 \to N \xrightarrow{f_{n+1}} R'_n \xrightarrow{f_n} \ldots \to R'_1 \xrightarrow{f_1} M \to 0$

be exact sequences, $\theta$ and $\theta'$ the associated classes. The following conditions are equivalent:

(i) $\theta = \theta'$;

(ii) there exists a commutative diagram with exact rows:

$$
\begin{array}{ccccccccccccc}
0 & \longrightarrow & N & \xrightarrow{f_{n+1}} & R_n & \longrightarrow & \ldots & \longrightarrow & R_1 & \xrightarrow{f_1} & M & \longrightarrow & 0 \\
& & 1_N \uparrow & & \uparrow & & & & \uparrow & & 1_M \uparrow \\
0 & \longrightarrow & N & \longrightarrow & R''_n & \longrightarrow & \ldots & \longrightarrow & R''_1 & \longrightarrow & M & \longrightarrow & 0 \\
& & 1_N \downarrow & & \downarrow & & & & \downarrow & & 1_M \downarrow \\
0 & \longrightarrow & N & \xrightarrow{f'_{n+1}} & R'_n & \longrightarrow & \ldots & \longrightarrow & R'_1 & \xrightarrow{f'_1} & M & \longrightarrow & 0 ;
\end{array}
$$

(iii) there exists a commutative diagram with exact rows:

$$
\begin{array}{ccccccccccccc}
0 & \longrightarrow & N & \xrightarrow{f_{n+1}} & R_n & \longrightarrow & \ldots & \longrightarrow & R_1 & \xrightarrow{f_1} & M & \longrightarrow & 0 \\
& & 1_N \downarrow & & \downarrow & & & & \downarrow & & 1_M \downarrow \\
0 & \longrightarrow & N & \longrightarrow & R''_n & \longrightarrow & \ldots & \longrightarrow & R''_1 & \longrightarrow & M & \longrightarrow & 0 \\
& & 1_N \uparrow & & \uparrow & & & & \uparrow & & 1_M \uparrow \\
0 & \longrightarrow & N & \xrightarrow{f'_{n+1}} & R'_n & \longrightarrow & \ldots & \longrightarrow & R'_1 & \xrightarrow{f'_1} & M & \longrightarrow & 0 .
\end{array}
$$

Let us prove $a$. Let $\alpha \in \mathrm{Ext}_A^n(M, N)$, and let $P$ be a projective resolution of $M$. Let $a : P(n) \to N$ be a morphism of complexes representing $\alpha$; its unique non-zero component is an $A$-homomorphism $u : P_n \to N$ which satisfies $u \circ d_{n+1} = 0$, hence factors as $u = \overline{u} \circ \delta_n$, where $\delta_n : P_n \to Z_{n-1}$ is the mapping induced by $d_n$ (we put $Z_{n-1} = \mathrm{Im}\, d_n$) and $\overline{u}$ is an $A$-homomorphism from $Z_{n-1}$ into $N$. By Remark 1, p. 117, the class $\theta \in \mathrm{Ext}_A^n(M, Z_{n-1})$ of the exact sequence

$$
0 \to Z_{n-1} \to P_{n-1} \to \ldots \to P_0 \to M \to 0
$$

is equal to the homotopy class of the morphism $(-1)^{n(n+1)/2} \delta_n$. We therefore have

$$
\alpha = (-1)^{n(n+1)/2} \overline{u} \circ \theta ,
$$

which makes it possible, by Cor. 3, p. 120, to represent $\alpha$ as the class of an exact sequence.

Let us prove $b$. It follows from Cor. 1 of X, p. 120 that (ii) $\Rightarrow$ (i) and that (iii) $\Rightarrow$ (i). Suppose that (i) is satisfied, and let $P$ be a projective resolution of $M$. There exists a commutative diagram

$$
\begin{array}{cccccccccccccc}
0 & \rightarrow & N & \xrightarrow{f_{n+1}} & R_n & \rightarrow & R_{n-1} & \rightarrow & \ldots \rightarrow & R_1 & \rightarrow & M & \rightarrow & 0 \\
& & u_n \uparrow & & u_{n-1} \uparrow & & u_{n-2} \uparrow & & & & & & 1_M \uparrow \\
& & P_n & \xrightarrow{d_n} & P_{n-1} & \rightarrow & P_{n-2} & \rightarrow & \ldots \rightarrow & P_0 & \rightarrow & M & \rightarrow & 0 \\
& & u'_n \downarrow & & u'_{n-1} \downarrow & & u'_{n-2} \downarrow & & & & & & 1_M \downarrow \\
0 & \rightarrow & N & \xrightarrow{f'_{n+1}} & R'_n & \rightarrow & R'_{n-1} & \rightarrow & \ldots \rightarrow & R'_1 & \rightarrow & M & \rightarrow & 0 .
\end{array}
$$

The morphisms from $P(n)$ into $N$ defined by $u_n$ and $u'_n$ are homotopic, since they both belong to the class $(-1)^{n(n+1)/2} \theta$, hence $u'_n - u_n$ is of the form $w \circ d_n$, where $w : P_{n-1} \to N$ is an $A$-homomorphism. Replacing $u'_{n-1}$ by $u'_{n-1} - f'_{n+1} \circ w$ and $u'_n$ by $u_n$, we reduce to the case where $u_n = u'_n$. This makes it possible to construct a new commutative diagram with exact rows:

$$
\begin{array}{cccccccccccccc}
0 & \rightarrow & N & \rightarrow & R_n & \rightarrow & R_{n-1} & \rightarrow & \ldots \rightarrow & R_1 & \rightarrow & M & \rightarrow & 0 \\
& & 1_N \uparrow & & v \uparrow & & u_{n-2} \uparrow & & & & & & 1_M \uparrow \\
0 & \rightarrow & N & \rightarrow & N' & \rightarrow & P_{n-2} & \rightarrow & \ldots \rightarrow & P_0 & \rightarrow & M & \rightarrow & 0 \\
& & 1_N \downarrow & & v' \downarrow & & u'_{n-2} \downarrow & & & & & & 1_M \downarrow \\
0 & \rightarrow & N & \rightarrow & R'_n & \rightarrow & R'_{n-1} & \rightarrow & \ldots \rightarrow & R'_1 & \rightarrow & M & \rightarrow & 0
\end{array}
$$

where $N'$ is the quotient of $P_{n-1} \oplus N$ by the submodule formed by the couples $(d_n(x), -u_n(x))$ for $x \in P_n$, and where $v$ (resp. $v'$) is defined by passing to the quotient from the mapping $u_{n-1} \oplus f_{n+1}$ (resp. $u'_{n-1} \oplus f'_{n+1}$). Condition (ii) is therefore satisfied.

Suppose again that condition (i) is satisfied, and let $E$ be an injective resolution of $N$. There exists a commutative diagram

$$
\begin{array}{cccccccccccc}
0 & \rightarrow & N & \rightarrow & R_n & \rightarrow & \ldots \rightarrow & R_1 & \rightarrow & M & \rightarrow & 0 \\
& & 1_N \downarrow & & v_0 \downarrow & & & & & & & \\
0 & \rightarrow & N' & \rightarrow & E^0 & \xrightarrow{\delta^0} & \ldots \rightarrow & E^{n-1} & \xrightarrow{\delta^{n-1}} & E^n \\
& & 1_N \uparrow & & v'_0 \uparrow & & & & & & & \\
0 & \rightarrow & N & \rightarrow & R'_n & \rightarrow & \ldots \rightarrow & R'_1 & \rightarrow & M & \rightarrow & 0
\end{array}
$$

and we show as above that we can assume $v'_n = v_n$. We then have a commutative diagram with exact rows

$$
\begin{array}{cccccccccccccc}
0 & \rightarrow & N & \rightarrow & R_n & \rightarrow & \ldots \rightarrow & R_2 & \rightarrow & R_1 & \rightarrow & M & \rightarrow & 0 \\
& & 1_N \downarrow & & \downarrow & & & & & & & & 1_M \downarrow \\
0 & \rightarrow & N & \rightarrow & E^0 & \rightarrow & \ldots \rightarrow & E^{n-2} & \rightarrow & M' & \rightarrow & M & \rightarrow & 0 \\
& & 1_N \uparrow & & \uparrow & & & & & & & & 1_M \uparrow \\
0 & \rightarrow & N & \rightarrow & R'_n & \rightarrow & \ldots \rightarrow & R'_2 & \rightarrow & R'_1 & \rightarrow & M & \rightarrow & 0
\end{array}
$$

with $M' = M \times_{\mathbf{R}_1} E_{n-1}$ (cf. X, p. 120, cor. 3, b)). Condition (iii) is therefore satisfied, which completes the proof of the theorem.

#### Remark 1 {#alg-x-s7-n5-rem-1 .statement}

If the ring $A$ is Noetherian, and if the $A$-modules $M$ and $N$ are of finite type, it follows from the proof of a) that every element of $\mathrm{Ext}_A^n(M, N)$ is the class associated with an exact sequence $0 \to N \to R_n \to \ldots \to R_1 \to M \to 0$ where the $R_i$ are of finite type.

#### Corollary {#alg-x-s7-n5-cor-1 .statement}

*Let* $0 \to N \xrightarrow{f} R \xrightarrow{g} M \to 0$ *and* $0 \to N \xrightarrow{f'} R' \xrightarrow{g'} M \to 0$ *be two exact sequences*, $\theta$ *and* $\theta'$ *their associated classes in* $\mathrm{Ext}^1(M, N)$. *For* $\theta = \theta'$ *to hold, it is necessary and sufficient that there exists an* A-homomorphism $h : R \to R'$ *making the diagram*

$$
\begin{array}{ccc}
& & R \\
N & \xrightarrow{f} & R \\
& \downarrow h & \downarrow g \\
& & M \\
& \xrightarrow{f'} & R' \\
& & \xrightarrow{g'}
\end{array}
$$

*commutative. Such a homomorphism is necessarily an isomorphism.*

The condition is sufficient according to cor. 1 of prop. 4. If $\theta = \theta'$, there exists a commutative diagram with exact rows:

$$
\begin{array}{ccccccccc}
0 & \longrightarrow & N & \longrightarrow & R & \longrightarrow & M & \longrightarrow & 0 \\
& & ^{1_N} & & ^{h'} & & ^{1_M} & & \\
0 & \longrightarrow & N & \longrightarrow & R'' & \longrightarrow & M & \longrightarrow & 0 \\
& & ^{1_N} & & ^{h''} & & ^{1_M} & & \\
0 & \longrightarrow & N & \longrightarrow & R' & \longrightarrow & M & \longrightarrow & 0 .
\end{array}
$$

The homomorphisms $h'$ and $h''$ are isomorphisms according to X, p. 7, cor. 3, and $h = h'' \circ {h'}^{-1}$ answers the question. The last assertion follows from *loc. cit.*

#### Remark 2 {#alg-x-s7-n5-rem-2 .statement}

Theorem 1 provides a description of $\mathrm{Ext}_A^n(M, N)$ as a set of equivalence classes of exact sequences; it is easy to describe the group law obtained on this set by transport of structure. Indeed, let $\theta$ (resp. $\theta'$) be the class of an exact sequence $0 \to N \xrightarrow{f_{n+1}} R_n \xrightarrow{f_n} \ldots \to R_1 \to M \to 0$ (resp. $0 \to N \xrightarrow{f'_{n+1}} R'_n \xrightarrow{f'_n} \ldots \to R'_1 \to M \to 0$). Let $\Delta : M \to M \oplus M$ and $\nabla : N \oplus N \to N$ be the $A$-linear maps defined by $\Delta(x) = (x, x)$ for $x \in M$ and $\nabla(y, z) = y + z$ for $y, z \in N$. Consider the mapping

$$
m : \mathrm{Ext}_A(M, N) \oplus \mathrm{Ext}_A(M, N) \to \mathrm{Ext}_A(M \oplus M, N \oplus N)
$$

defined in the *remark*, p. 121. With the notations of *loc. cit.*, one has $\nabla \circ i_N = 1_N$ and $q_M \circ \Delta = 1_M$, and thus $\theta + \theta' = \nabla \circ m(\theta, \theta') \circ \Delta$. Taking into account *loc. cit.* and cor. 3, p. 120, this provides an exact sequence of class $\theta+\theta'$: for example, if $n \geq 2$, one can take the sequence

$$
0\longrightarrow \mathbf{N}\longrightarrow R_n''\longrightarrow R_{n-1}\oplus R'_{n-1}\xrightarrow{\,f_{n-1}\oplus f'_{n-1}\,}\cdots\longrightarrow R_2\oplus R'_2\longrightarrow R'_1\longrightarrow M\longrightarrow0
$$

where $R_n''$ is the quotient of $R_n\oplus R'_n$ by the submodule formed by the couples

$$
\left(f_{n+1}(x),-f'_{n+1}(x)\right)\quad\text{pour }x\in\mathbf{N},
$$

and where $R''_1=R_1\times_M R'_1$.

### 6. Composition Product and Connecting Homomorphisms of Extension Modules

#### Proposition 5 {#alg-x-s7-prop-5 .statement}

Let

$$(\mathcal{E})\qquad 0\longrightarrow M'\xrightarrow{\,f\,}M\xrightarrow{\,g\,}M''\longrightarrow0$$

be an exact sequence of left $A$-modules, $\theta\in\operatorname{Ext}^1_A(M'',M')$ the associated class, $N$ a left $A$-module, $n$ an integer.

a) The connecting homomorphism $\delta^n(N,\mathcal{E}):\operatorname{Ext}^n_A(N,M'')\longrightarrow\operatorname{Ext}^{n+1}_A(N,M')$ is the composition product $\alpha\mapsto\theta\circ\alpha$ with $\theta$.

#### Corollaire 1 {#alg-x-s7-prop-5-cor-1 .statement}

a) The *connecting homomorphism* $\mathrm{Hom}_A(M'', M'') \to \mathrm{Ext}_A^1(M'', M')$ *sends* $1_{M''}$ *to* $\theta$.

b) The *connecting homomorphism* $\mathrm{Hom}_A(M', M') \to \mathrm{Ext}_A^1(M'', M')$ *sends* $1_{M'}$ *to* $-\theta$.

#### Corollaire 2 {#alg-x-s7-prop-5-cor-2 .statement}

*Consider two short exact sequences of left A-modules*

$$
\begin{align*}
0 &\to M' \to M \to M'' \to 0 \\
0 &\to N' \to N \to N'' \to 0 .
\end{align*}
$$

*Then the composite connecting homomorphisms*

$$
\operatorname{Ext}_A^n(M',N'') \to \operatorname{Ext}_A^{n+1}(M'',N'') \to \operatorname{Ext}_A^{n+2}(M'',N')
$$

*and*

$$
\operatorname{Ext}_A^n(M',N'') \to \operatorname{Ext}_A^{n+1}(M',N') \to \operatorname{Ext}_A^{n+2}(M'',N')
$$

*are opposite.*

Indeed, let $\theta_1$, $\theta_2$ be the classes associated with the given exact sequences, and let $\alpha \in \operatorname{Ext}_A^n(M', M'')$. The images of $\alpha$ are respectively

$$
\theta_2 \circ \bigl((-1)^{n+1} \alpha \circ \theta_1\bigr) \quad \text{and} \quad (\theta_2 \circ \alpha) \circ \bigl((-1)^{n+2} \theta_1\bigr).
$$

Consider a short exact sequence of left A-modules

$$
(\mathcal{S}) \qquad 0 \to N \to R_n \xrightarrow{f_n} R_{n-1} \xrightarrow{f_{n-1}} \cdots \to R_1 \xrightarrow{f_1} M \to 0
$$

and set $K_0=M$, $K_i=\operatorname{Ker}f_i$, $i=1,\ldots,n-1$, $K_n=N$. We therefore have exact sequences

$$
(9)\qquad 0\to K_i\to R_i\to K_{i-1}\to0,\qquad 1\leq i\leq n,
$$

to which are associated for every $A$ left module $P$, connecting homomorphisms

$$
\operatorname{Ext}_A^m(P,K_{i-1})\to\operatorname{Ext}_A^{m+1}(P,K_i),
$$

$$
\operatorname{Ext}_A^m(K_i,P)\to\operatorname{Ext}_A^{m+1}(K_{i-1},P),
$$

whence by composition of the *iterated connecting homomorphisms*, associated with $(\mathcal{S})$

$$
\delta^m(P,\mathcal{S}):\operatorname{Ext}_A^m(P,M)\to\operatorname{Ext}_A^{m+n}(P,N)
$$

$$
\delta^m(\mathcal{S},P):\operatorname{Ext}_A^m(N,P)\to\operatorname{Ext}_A^{m+n}(M,P).
$$

#### Corollary 3 {#alg-x-s7-prop-5-cor-3 .statement}

If $\theta\in\operatorname{Ext}_A^n(M,N)$ is the class of the exact sequence $(\mathcal{S})$, we have

$$
\delta^m(P,\mathcal{S})(\alpha)=\theta\circ\alpha,\qquad
\delta^m(\mathcal{S},P)(\beta)=(-1)^{mn+n(n+1)/2}\beta\circ\theta.
$$

If $\theta_i\in\operatorname{Ext}_A^1(K_{i-1},K_i)$ is the class associated with the exact sequence (9), we have by Proposition 5

$$
\delta^m(P,\mathcal{S})(\alpha)=\theta_n\circ\cdots\circ\theta_2\circ\theta_1\circ\alpha
$$

$$
\delta^m(\mathcal{S},P)(\beta)=(-1)^{(m+1)+\cdots+(m+n)}\beta\circ\theta_n\circ\cdots\circ\theta_1.
$$

Moreover, by Proposition 3 (X, p. 118), we have $\theta=\theta_n\circ\cdots\circ\theta_1$. The corollary follows immediately from this, and from the relation (E, III, p. 44)

$$
(m+1)+\cdots+(m+n)=mn+n(n+1)/2.
$$

#### Corollary 4 {#alg-x-s7-prop-5-cor-4 .statement}

If each module $R_i,\ i = 1, ..., n,$ is injective (resp. projective), the mapping $\alpha \mapsto \theta \circ \alpha$ (resp. $\alpha \mapsto \alpha \circ \theta$) from $\mathrm{Ext}_A^m(P, M)$ to $\mathrm{Ext}_A^{m+n}(P, N)$ (resp. from $\mathrm{Ext}_A^m(N, P)$ to $\mathrm{Ext}_A^{m+n}(M, P)$) is bijective for every $A$-module $P$ and every integer $m > 0$.

This indeed follows from Corollary 3 and the exact sequences

$$
\mathrm{Ext}_A^{m+i-1}(P, R_i) \to \mathrm{Ext}_A^{m+i-1}(P, K_{i-1}) \to \mathrm{Ext}_A^{m+i}(P, K_i) \to \mathrm{Ext}_A^{m+i}(P, R_i)
$$
(resp. $\mathrm{Ext}_A^{m+i-1}(R_i, P) \to \mathrm{Ext}_A^{m+i-1}(K_i, P) \to \mathrm{Ext}_A^{m+i}(K_{i-1}, P) \to \mathrm{Ext}_A^{m+i}(R_i, P)$),
whose extreme terms are zero by assumption.

#### Remark {#alg-x-s7-n6-rem-1 .statement}

The definitions and propositions of Nos. 3 to 6 apply to $A$ right modules, considered as left modules over the ring $A^\circ$ opposite to $A$.

### 7. The homomorphism $\mathrm{Ext}_A(P, Q) \otimes \mathrm{Tor}^A(P, M) \to \mathrm{Tor}^A(Q, M)$

Let $M$ be a $A$ left module, $P$ and $Q$ two $A$ right modules. Consider the homomorphism $\mathrm{Homgr}_A(L(P), L(Q)) \otimes_k (L(P) \otimes_A L(M)) \to L(Q) \otimes_A L(M)$ which associates with $f \otimes (x \otimes y)$ the element $f(x) \otimes y$. By X, p. 99, it is a morphism of complexes. We deduce from this a graded $k$-linear mapping of degree 0

$$
H(\mathrm{Homgr}_A(L(P), L(Q))) \otimes_k \mathrm{Tor}^A(P, M) \to \mathrm{Tor}^A(Q, M)
$$

then by the isomorphism $\varphi(L(P), L(Q))$ of § 6 (X, p. 100, th. 1), a graded $k$-linear mapping of degree 0

(10)
$$
\mathrm{Ext}_A(P, Q) \otimes_k \mathrm{Tor}^A(P, M) \to \mathrm{Tor}^A(Q, M),
$$
corresponding to $k$-bilinear mappings

(11)
$$
c_{P, Q; M}: \mathrm{Ext}_A^n(P, Q) \times \mathrm{Tor}_m^A(P, M) \to \mathrm{Tor}_{m-n}^A(Q, M);
$$
The image of the pair $(\alpha, \gamma)$ under $c_{P, Q; M}$ is called the composition product of $\alpha$ and $\gamma$ and is denoted by $\alpha \circ \gamma$.

By construction, $\alpha \circ \gamma$ is obtained as follows: one represents $\alpha$ by a morphism of complexes $f : L(P) \to L(Q)(-n)$, $\gamma$ by an element $z \in Z_m(L(P) \otimes_A L(M))$, and $\alpha \otimes \gamma$ is the class of the element

$$
(f \otimes 1)(z) \in Z_m(L(Q)(-n) \otimes_A L(M)) = Z_{m-n}(L(Q) \otimes_A L(M)).
$$

For example, if $\alpha \in \mathrm{Hom}_A(P, Q)$, then $\alpha \circ \gamma = \mathrm{Tor}(\alpha, 1)(\gamma)$.

#### Remark 1 {#alg-x-s7-n7-rem-1 .statement}

If one uses the isomorphisms $\psi$ of X, p. 69, one can also define the composition product by the commutative diagram

$$
\begin{array}{ccc}
\mathrm{Ext}_A^n(P, Q) \times \mathrm{Tor}_m^A(P, M) & \xrightarrow{c_{P,Q;M}} & \mathrm{Tor}_{m-n}^A(Q, M) \\
\bar{a}_{P,Q} \times \psi_{P(M)} \downarrow & & \downarrow \psi_{Q(M)} \\
H^n(\mathrm{Homgr}_A(L(P), L(Q))) \times H_m(L(P) \otimes_A M) & \longrightarrow & H_{m-n}(L(Q) \otimes_A M);
\end{array}
$$

in other words, one represents $\alpha$ by a morphism $f$ from $L(P)$ to $L(Q) (-n)$, $\gamma$ by a cycle $x \in L_m(P) \otimes_A M$, and $\alpha \circ \gamma$ is the class of the cycle

$$
(f_m \otimes 1_M)(x) \in L_{m-n}(Q) \otimes_A M.
$$

#### Remark 2 {#alg-x-s7-n7-rem-2 .statement}

One can also use the resolutions $l(P)$ and $l(Q)$.

Analogously, if $N$ is a second left $A$-module, one defines a composition product $(\mu, \gamma) \mapsto \mu \circ \gamma$ denoted

$$
c_{P:M,N}: \mathrm{Ext}_A^r(M, N) \times \mathrm{Tor}_m^A(P, M) \to \mathrm{Tor}_{m-r}^A(P, N)
$$

by the commutative diagram

$$
\begin{array}{ccc}
\mathrm{Ext}_A^r(M, N) \times \mathrm{Tor}_m^A(P, M) & \xrightarrow{c_{P:M,N}} & \mathrm{Tor}_{m-r}^A(P, N) \\
1 \times \sigma_{P,M,r} \downarrow & & \downarrow \sigma_{P,N,m-r} \\
\mathrm{Ext}_A^r(M^\circ, N^\circ) \times \mathrm{Tor}_m^{A^\circ}(M^\circ, P^\circ) & \xrightarrow{c_{M^\circ,N^\circ,P^\circ}} & \mathrm{Tor}_{m-r}^{A^\circ}(N^\circ, P^\circ)
\end{array}
$$

where $\sigma$ denotes the commutation isomorphisms (X, p. 71).

If $\mu \in \mathrm{Ext}_A^r(M, N)$ is the class of the morphism $g : L(M) \to L(N) (-r)$, and if $\gamma \in \mathrm{Tor}_m^A(P, M)$ is the class of the cycle $z = \sum z_{ij}$, where $z_{ij} \in L_i(P) \otimes_A L_j(M)$, then $\mu \circ \gamma$ is therefore the class of the cycle $\sum (-1)^{ir} (1 \otimes g)(z_{ij})$.

One can also represent $\gamma$ by a cycle $y \in P \otimes L_m(M)$, and $\mu \circ \gamma$ is the class of the cycle $(1 \otimes g)(y) \in P \otimes L_{m-r}(M)$.

#### Proposition 6 {#alg-x-s7-prop-6 .statement}

Let $K, M, N$ be left $A$-modules, $P, Q, R$ right $A$-modules,
$\alpha \in \mathrm{Ext}_A^n(P, Q)$, $\beta \in \mathrm{Ext}_A^p(Q, R)$, $\lambda \in \mathrm{Ext}_A^r(K, M)$, $\mu \in \mathrm{Ext}_A^s(M, N)$, $\gamma \in \mathrm{Tor}_m^A(P, K)$.
Then
(13) $$ (\beta \circ \alpha) \circ \gamma = \beta \circ (\alpha \circ \gamma) \quad \text{in} \quad \mathrm{Tor}_{m-p-n}^A(R, K), $$
(14) $$ (\mu \circ \lambda) \circ \gamma = \mu \circ (\lambda \circ \gamma) \quad \text{in} \quad \mathrm{Tor}_{n-r-s}^A(P, N), $$
(15) $$ \alpha \circ (\lambda \circ \gamma) = (-1)^{nr} \lambda \circ (\alpha \circ \gamma) \quad \text{in} \quad \mathrm{Tor}_{m-p-r}^A(Q, M). $$

Formulas (13) and (14) follow immediately from the definitions. Let us prove (15).
Let $z = \sum z_{ij}$, $z_{ij} \in L_i(P) \otimes L_j(K)$ be a cycle representing $\gamma$, $f : L(P) \to L(Q) (-n)$ and $g : L(K) \to L(M) (-r)$ morphisms representing $\alpha$ and $\lambda$. Then $\lambda \circ (\alpha \circ \gamma)$ is the class of $\sum (-1)^{(i-n)r} (f \otimes g)(z_{ij})$ and $\alpha \circ (\lambda \circ \gamma)$ is the class of

$$
\sum (-1)^{ir} (f \otimes g)(z_{ij}), \quad \text{whence (15)}.
$$

### 8. Composition products and connecting homomorphisms of torsion products

#### Proposition 7 {#alg-x-s7-prop-7 .statement}

a) Let

(ε)
$$
0 \to P' \xrightarrow{f} P \xrightarrow{g} P'' \to 0
$$
be an exact sequence of right $A$-modules, $\theta \in \mathrm{Ext}_A^1(P'', P')$ the associated class, $M$ a left $A$-module. The connecting homomorphism
$$
\delta_n(\mathcal{E}, M) : \mathrm{Tor}_n^A(P'', M) \to \mathrm{Tor}_{n-1}^A(P', M) \text{ is the mapping } \gamma \mapsto \theta \circ \gamma .
$$

b) Let

(ε₁)
$$
0 \to M' \to M \to M'' \to 0
$$
be an exact sequence of left $A$-modules, $\theta_1 \in \mathrm{Ext}_A^1(M'', M')$ the associated class, $P$ a right $A$-module. The connecting homomorphism
$$
\delta_n(P, \mathcal{E}_1) : \mathrm{Tor}_n^A(P, M'') \to \mathrm{Tor}_{n-1}^A(P, M') \text{ is the mapping } \gamma \mapsto \theta_1 \circ \gamma .
$$
Let $\gamma \in \mathrm{Tor}_n^A(P'', M)$ be the class of a cycle $z'' \in \dot{Z}_n(L(P'') \otimes_A L(M))$, and let
$$
\begin{array}{ccccccccc}
0 & \longrightarrow & P' & \xrightarrow{f} & P & \xrightarrow{g} & P'' & \longrightarrow & 0 \\
& & \uparrow u_1 & & \uparrow u_0 & & \uparrow 1 & & \\
L_1(P'') & \xrightarrow{d_1} & L_0(P'') & \xrightarrow{p_0''} & P'' & \longrightarrow & 0
\end{array}
$$
be a commutative diagram. We shall denote by $p' : L(P') \to P'$ and $p'' : L(P'') \to P''$ the canonical morphisms of complexes. By definition, $\delta(\gamma) \in \mathrm{Tor}_{n-1}^A(P', M)$ is obtained as follows: one chooses $x \in P \otimes L_n(M)$ such that $(g \otimes 1)(x) = (p'' \otimes 1)(z'')$ and $\delta(\gamma)$ is the class of cycles $z' \in Z_{n-1}(L(P') \otimes L(M))$ such that
$$
(f \otimes 1)(p' \otimes 1)(z') = (1 \otimes d_n)(x) .
$$
For $0 \leq i \leq n$, let $z''_i$ be the component of $z''$ in $L_i(P'') \otimes L_{n-i}(M)$; we have
$$
0 = Dz'' = \sum_i (d_i \otimes 1 + (-1)^i \otimes d_{n-i})(z''_i) ,
$$
hence $(d_i \otimes 1)(z''_i) = (-1)^i \otimes d_{n-i+1}(z''_{i-1})$ and in particular
$$
(d_1 \otimes 1)(z''_1) = -1 \otimes d_n(z''_0) .
$$
Let us then choose $x = (u_0 \otimes 1)(z''_0)$: we indeed have
$$
(g \otimes 1)(x) = (p_0'' \otimes 1)(z''_0) = (p'' \otimes 1)(z'') .
$$
Since
$$
(1 \otimes d_n)(x) = (u_0 \otimes 1)(1 \otimes d_n)(z''_0) = - (u_0 \otimes 1)(d_1 \otimes 1)(z''_1)
= - (f \otimes 1)(u_1 \otimes 1)(z''_1) ,
$$

it follows that $\delta(\gamma)$ is the class of cycles $z' \in Z_{n-1}(L(P') \otimes_A L(M))$ such that $(p' \otimes 1)(z') = - (u_1 \otimes 1)(z''_1)$. But, by definition, the class $\theta$ corresponds via the isomorphism $\mathrm{Ext}_A^1(P'', P') \to H^1(\mathrm{Homgr}_A(L(P''), P'))$ to the class of the morphism $f : L(P'')(1) \to P'$ defined by $- u_1$, and the product $\theta \circ \gamma$ is the class of cycles
$$
\overline{z}' \in Z_{n-1}(L(P') \otimes_A L(M)) \quad \text{such that} \quad (p \otimes 1)(\overline{z}') = f(z'') = - (u_1 \otimes 1)(z''_1),
$$
which completes the proof of a). Assertion b) follows from a) by the commutation isomorphisms.

#### Corollary 1 {#alg-x-s7-prop-7-cor-1 .statement}

*Let* $0 \to P' \to P \to P'' \to 0$ *be an exact sequence of right* $A$-*modules*, $0 \to M' \to M \to M'' \to 0$ *be an exact sequence of left* $A$-*modules*. *Then the composed homomorphisms of connecting homomorphisms*
$$
\mathrm{Tor}_n^A(P'', M'') \to \mathrm{Tor}_{n-1}^A(P'', M') \to \mathrm{Tor}_{n-2}^A(P', M')
$$
*and*
$$
\mathrm{Tor}_n^A(P'', M'') \to \mathrm{Tor}_{n-1}^A(P', M'') \to \mathrm{Tor}_{n-2}^A(P', M')
$$
*are opposite*.

Indeed, if $\theta$ and $\theta_1$ are the classes associated with the given exact sequences, and if $\gamma \in \mathrm{Tor}_n^A(P'', M'')$, the images of $\gamma$ are respectively $\theta \circ (\theta_1 \circ \gamma)$ and $\theta_1 \circ (\theta \circ \gamma)$, hence are opposite by prop. 6.

Let us resume the notations of X, p. 127 and consider the sequence $(\mathscr{S})$ of left $A$-modules and the connecting homomorphisms associated with the exact sequences (9)
$$
\mathrm{Tor}_m^A(P, K_{i-1}) \to \mathrm{Tor}_{m-1}^A(P, K_i);
$$
we deduce from this by composition of the *iterated connecting homomorphisms*
$$
\hat{\partial}_m(P, \mathscr{S}) : \mathrm{Tor}_m^A(P, M) \to \mathrm{Tor}_{m-n}^A(P, N).
$$
Then by prop. 7 and prop. 3 of X, p. 118 :

#### Corollary 2 {#alg-x-s7-prop-7-cor-2 .statement}

If $\theta \in \mathrm{Ext}_A^n(M, N)$ is the class associated with the exact sequence $(\mathscr{S})$, we have $\hat{\partial}_m(P, \mathscr{S})(\alpha) = \theta \circ \alpha$ for all $\alpha \in \mathrm{Tor}_m^A(P, M)}$.

#### Corollary 3 {#alg-x-s7-prop-7-cor-3 .statement}

If all the modules $R_i$, $i = 1, ..., n$, are flat, the mapping $\alpha \mapsto \theta \circ \alpha$ from $\mathrm{Tor}_{m+n}^A(P, M)$ to $\mathrm{Tor}_m^A(P, N)$ is bijective for every right $A$-module $P$ and every integer $m > 0$.

This follows from Cor. 2 and the exact sequences

$$
\mathrm{Tor}_{m+n-i+1}^A(P, R_i) \to \mathrm{Tor}_{m+n-i+1}^A(P, K_{i-1}) \xrightarrow{\hat{\partial}} \mathrm{Tor}_{m+n-i}^A(P, K_i) \to \mathrm{Tor}_{m+n-i}^A(P, R_i)
$$

where the extreme terms are zero by hypothesis.

Analogously, if

$$(\mathcal{S}_1)$$
$$0 \to Q \to S_n \to S_{n-1} \to \ldots \to S_1 \to P \to 0$$

is an exact sequence of right $A$-modules, and $M$ a left $A$-module, we define *iterated connecting homomorphisms*

$$\partial^m(\mathcal{S}_1, M) : \mathrm{Tor}_m^A(P, M) \to \mathrm{Tor}_{m-n}^A(Q, M)$$

and we have:

#### Corollary 4 {#alg-x-s7-prop-7-cor-4 .statement}

If $\theta_1 \in \mathrm{Ext}_A^n(P, Q)$ is the class associated with the exact sequence $(\mathcal{S}_1)$, we have $\partial^m(\mathcal{S}_1, M)(\alpha) = \theta_1 \circ \alpha$ for all $\alpha \in \mathrm{Tor}_m^A(P, M)}$.

### 9. Computation of Composition Products by Resolution Shifts

Let

(16)
$$0 \to M \xrightarrow{\iota} K_n \to K_{n-1} \to \ldots \to K_1 \xrightarrow{\rho} M' \to 0$$

be an exact sequence of left $A$-modules and $\theta \in \mathrm{Ext}_A^n(M', M)$ the associated class.

Let $a : (R, d) \to M$ be a left resolution of $M$; hence there is an exact sequence

$$ \to R_k \xrightarrow{d_k} R_{k-1} \to \ldots \xrightarrow{d_1} R_0 \xrightarrow{a_0} M \to 0.$$

and by shifting $n$ (X, p. 26) an exact sequence

(17)
$$\to R_k \xrightarrow{(-1)^n d_k} R_{k-1} \to \ldots \xrightarrow{(-1)^n d_1} R_0 \xrightarrow{(-1)^n a_0} M \to 0.$$

We deduce from (16) and (17) an exact sequence

$$\to R_k \xrightarrow{(-1)^n d_k} R_{k-1} \to \ldots \xrightarrow{(-1)^n d_1} R_0 \xrightarrow{(-1)^n f \circ a_0} K_n \to K_{n-1} \to \ldots \to K_1 \to M' \to 0$$

thereby obtaining a resolution $R'$ of $M'$; let $\varphi : R' \to R(-n)$ be the morphism such that $\varphi_k = 1_{R_{k-n}}$ for $k \geq n$.

If $N$ is a left $A$-module and $P$ a right $A$-module, we therefore have mappings

$$\mathrm{H}(1_P \otimes \varphi) : \mathrm{H}(P \otimes_A R') \to \mathrm{H}(P \otimes_A R)(-n)$$
$$\mathrm{H}(\mathrm{Homgr}_A(\varphi, 1_N)) : \mathrm{H}(\mathrm{Homgr}_A(R, N))(n) \to \mathrm{H}(\mathrm{Homgr}_A(R', N)).$$

Let $k$ be an integer.

#### Proposition 8 {#alg-x-s7-prop-8 .statement}

*a)* The following diagram, where $h_\theta(\alpha) = \theta \circ \alpha$, is commutative

$$
\begin{array}{ccc}
\mathrm{Tor}_{k+n}^A(P, M') & \xrightarrow{h_\theta} & \mathrm{Tor}_k^A(P, M) \\
\psi_{k+n}(P, R') \downarrow & & \downarrow \psi_k(P, R) \\
\mathrm{H}_{k+n}(P \otimes_A R') & \xrightarrow{H_{k+n}(1 \otimes \varphi)} & \mathrm{H}_k(P \otimes_A R)
\end{array}
$$

b) The following diagram, where $\delta_\theta(\beta) = \beta \circ \theta$, is commutative

$$
\begin{array}{ccc}
H^k(\mathrm{Homgr}_A(R, N)) & \xrightarrow{H^{k+n}(\mathrm{Homgr}_A(\varphi, 1))} & H^{k+n}(\mathrm{Homgr}_A(R', N)) \\
\varphi^k(R, N) \downarrow & & \varphi^{k+n}(R', N) \downarrow \\
\mathrm{Ext}_A^k(M, N) & \xrightarrow{\delta_\theta} & \mathrm{Ext}_A^{k+n}(M', N).
\end{array}
$$

Let $\alpha : L(M) \to R$ be a morphism of complexes such that $a \circ \alpha = p_M$ and let

$$
\begin{array}{ccccccccc}
L_n(M') & \longrightarrow & L_{n-1}(M') & \longrightarrow & \ldots & \longrightarrow & L_0(M') & \longrightarrow & M' \longrightarrow 0 \\
u_n \downarrow & & u_{n-1} \downarrow & & & & u_0 \downarrow & & 1 \downarrow \\
0 & \longrightarrow & M & \xrightarrow{f} & K_n & \longrightarrow & \ldots & \longrightarrow & K_1 \longrightarrow M' \longrightarrow 0
\end{array}
$$

a commutative diagram, let us choose a homomorphism $v_n : L_n(M') \to L_0(M)$ such that $p_M \circ v_n = (-1)^n u_n$; by *X*, p. 47, Proposition 1, a), $v_n$ extends to a morphism of complexes $v : L(M') \to L(M)$ $(-n)$, and $\theta$ is the image under the canonical isomorphism $H^n(\mathrm{Homgr}_A(L(M'), L(M))) \to \mathrm{Ext}_A^n(M', M)$ of the class of $v$ (*X*, p. 117, Remark 1). We define a morphism of complexes $\beta : L(M') \to R'$ by $\beta_p = u_p$ for $p \leq n - 1$, $\beta_p = \alpha_{p-n} \circ v_p$ for $p \geq n$, and we have

$$
\varphi \circ \beta = \alpha(-n) \circ v.
$$

On the other hand, by definition of the mappings $\varphi$ and $\psi$, we have

$$
\begin{aligned}
& \psi_k(P, R) = H_k(p_P \otimes \alpha), \quad \varphi^k(R, N) = H^k(\mathrm{Homgr}_A(\alpha, e_N)), \\
& \psi_{k+n}(P, R') = H_{k+n}(p_P \otimes \beta), \quad \varphi^{k+n}(R', \tilde{N}) = H^{k+n}(\mathrm{Homgr}_A(\beta, e_N)).
\end{aligned}
$$

Finally, by definition of the composition product, we have

$$
h_\theta = H(1_{L(P)} \otimes v), \quad \delta_\theta = H(\mathrm{Homgr}_A(v, 1_{L(N)})) .
$$

Consequently, we have the equalities

$$
\begin{aligned}
\psi_k(P, R) \circ h_\theta &= H_k(p_P \otimes \alpha) \circ H_k(1_{L(P)} \otimes v) = H_k(p_P \otimes (\alpha \circ v)) = H_{k+n}(p_P \otimes (\varphi \circ \beta)) \\
&= H_{k+n}(1 \otimes \varphi) \circ H_{k+n}(p_P \circ \beta) = H_{k+n}(1 \otimes \varphi) \circ \psi_{k+n}(P, R'),
\end{aligned}
$$

from which a) follows; the proof of b) is analogous.

#### Remark {#alg-x-s7-n9-rem-1 .statement}

Via the commutation isomorphisms, we deduce from a) an analogous statement in the case of an exact sequence (16) of right A-modules.

Let $b : M' \to E'$ be a right resolution of $M'$; we thus have an exact sequence

$$
0 \to M' \xrightarrow{b^0} {E'}^0 \xrightarrow{\delta^0} {E'}^1 \to \ldots \to {E'}^k \xrightarrow{\delta^k} {E'}^{k+1}
$$

corresponding to a right resolution $E$ of $M$; let $\sigma : E'(n) \to E$ be the morphism such that $\sigma^k = 1_{{E'}^{k-n}}$ for $k \geq n$. We thus have homomorphisms

$$
H(\mathrm{Homgr}_A(1_N, \sigma)) : H(\mathrm{Homgr}_A(N, E'))(n) \to H(\mathrm{Homgr}_A(N, E)) .
$$

#### Proposition 9 {#alg-x-s7-prop-9 .statement}

*The following diagram, where $\gamma_\theta(\alpha) = \theta \circ \alpha$, is commutative*:

$$
\begin{array}{ccc}
H^k(\mathrm{Homgr}_A(N, E')) & \xrightarrow{H^{k+n}(\mathrm{Homgr}_A(1_N, \sigma))} & H^{k+n}(\mathrm{Homgr}_A(N, E)) \\
\downarrow \varphi^k(N, E') & & \downarrow \varphi^{k+n}(N, E) \\
\mathrm{Ext}_A^k(N, M') & \xrightarrow{\gamma_\theta} & \mathrm{Ext}_A^{k+n}(N, M)
\end{array}
$$

This is proved in a way analogous to Proposition 8.

## Exercises {#alg-x-s7-exercises}
See the [exercises for § 7](exercises/s7/).
