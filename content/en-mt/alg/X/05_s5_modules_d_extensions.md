---
book: alg
book_title: Algebra
chapter: X
chapter_title: ALGÈBRE HOMOLOGIQUE
section: 5
section_title: Modules d’extensions
lang: en
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
content_sha256: 2a8f00d4abc6191a2668f4c8873a54f6d7bcf2ec527b7111642fb1cc059355aa
translated_from: content/fr/alg/X/05_s5_modules_d_extensions.md
source_lang: fr
translation_method: machine
source_content_sha256: a8e0b6026ac3a6b3cf91b3261cf288e27bfe5f90539217221d869c3e7ea01bd3
translation_model: gpt-5-6-mini, hy3-free, laguna-s-2.1-free, nemotron-3-ultra-free
translation_run: translate-en-mt-be8c3dec
glossary_version: 34
glossary_terms_sha256: a8e8fd62ccc6c8574c03c75e13f51f61ebe5105b7077ae53935ae1a651920352
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 5. MODULES OF EXTENSIONS

*We retain the general notations of paragraph 4. We shall also agree that, unless explicitly stated otherwise, all the modules considered are left modules, all the complexes considered are complexes of left modules.*

### 1.  Complexes of homomorphisms

Let $(C,d)$ and $(C',d')$ be two A-complexes. Consider the graded $k$-module $\operatorname{Homgr}_A(C,C')$ (II, p. 174, 175): for $n\in\mathbf{Z}$, $\operatorname{Homgr}_A(C,C')_n$ is the $k$-module of graded A-linear mappings of degree $n$ from $C$ into $C'$; in other words $\operatorname{Homgr}_A(C,C')$ is canonically identified with the a-module

$$
\bigoplus_{n\in\mathbf{Z}}\prod_{p\in\mathbf{Z}}\operatorname{Hom}_A(C_p,C'_{p+n})
=
\bigoplus_{n\in\mathbf{Z}}\prod_{p+q=n}\operatorname{Hom}_A(C_p,{C'}^q).
$$

Define $k$-linear mappings

$$
D_n:\operatorname{Homgr}_A(C,C')_n\longrightarrow
\operatorname{Homgr}_A(C,C')_{n-1},\qquad n\in\mathbf{Z},
$$

by

(1) $$
D_n(f)=d'\circ f-(-1)^n f\circ d;
$$

we have

$$
D_{n-1}\circ D_n(f)
=D_{n-1}\bigl(d'\circ f-(-1)^n f\circ d\bigr)
=d'\circ d'\circ f-(-1)^n d'\circ f\circ d
$$

$$
\qquad\qquad{}-(-1)^{n-1}d'\circ f\circ d-f\circ d\circ d=0.
$$

Then $(\operatorname{Homgr}_A(C,C'),D)$ is a complex of $k$-modules called the *complex of homomorphisms of $C$ into $C'$*.

For example, Homgr_A (A, C') is canonically identified with C'. Note also that, for every $n \in \mathbf{Z}$, one has $\mathrm{Homgr}_A (C, C') (n) = \mathrm{Homgr}_A (C, C'(n))$.

The elements of $Z_n(\mathrm{Homgr}_A (C, C'))$ are the graded homomorphisms $f$ of (descending) degree $n$ from $C$ into $C'$ such that $d' \circ f = (-1)^n f \circ d$, that is to say the morphisms of complexes from $C$ into $C'(n)$, or equivalently from $C(p)$ into $C'(p+n)$ for any fixed $p$. They are called the *morphisms of complexes of degree* (descending) $n$ *from C into C'*; if $f, g \in Z_n(\mathrm{Homgr}_A (C, C'))$ and $s \in \mathrm{Homgr}_A (C, C')_{n+1}$, then the condition $g - f = Ds$ means that $s$ is a homotopy linking the morphisms $f$ and $g$ from $C$ into $C'(n)$, so that $H_n(\mathrm{Homgr}_A (C, C'))$ *is the k-module of the homotopy classes of morphisms of descending degree n from C into C'*.

Let $\alpha \in H_n(\mathrm{Homgr}_A (C, C'))$ and $p \in \mathbf{Z}$. Represent $\alpha$ by $f \in Z_n(\mathrm{Homgr}_A (C, C'))$; then $f$ is a morphism of complexes from $C$ into $C'(n)$, hence $H_p(f)$ is a homomorphism from $H_p(C)$ into $H_p(C'(n)) = H_{p+n}(C')$; since $H_p(f)$ depends only on the homotopy class $\alpha$ of $f$ (X, p. 33, prop. 3), we deduce a canonical homomorphism of $k$-modules

$$
H_n(\mathrm{Homgr}_A (C, C')) \to \mathrm{Hom}_A (H_p(C), H_{p+n}(C')) ,
$$

whence a *graded k-linear mapping of degree* 0, called *canonical*

$$
\lambda(C, C') : H(\mathrm{Homgr}_A (C, C')) \to \dot{\mathrm{Homgr}}_A (H(C), H(C')) .
$$

The homogeneous components of $\lambda(C, C')$ will often be denoted:

$$
\lambda^n(C, C') : H^n(\mathrm{Homgr}_A (C, C')) \to \prod_{p+q=n} \mathrm{Hom}_A (H_p(C), H^q(C')) .
$$

#### Proposition 1 {#alg-x-s5-prop-1 .statement}

*If C is zero on the right and C' zero on the left, then Homgr_A (C, C') is zero on the left, and the canonical k-linear mapping*

$$
\lambda^0(C, C') : H^0(\mathrm{Homgr}_A (C, C')) \to \mathrm{Hom}_A (H_0(C), H^0(C'))
$$

*is bijective*.

We have exact sequences

$$
\begin{aligned}
&0 \longrightarrow H^0(C') \xrightarrow{i} {C'}^0 \xrightarrow{{d'}^0} {C'}^1 \\
&C_1 \xrightarrow{d_1} C_0 \xrightarrow{p} H_0(C) \longrightarrow 0 .
\end{aligned}
$$

On the other hand $\mathrm{Homgr}_A^0 (C, C')$ is identified with $\mathrm{Hom}_A (C_0, {C'}^0)$, $Z^0(\mathrm{Homgr}_A (C, C'))$ then being identified with the set of $f : C_0 \to {C'}^0$ such that ${d'}^0 \circ f = 0, f \circ d_1 = 0$; $B^0(\mathrm{Homgr}_A (C, C'))$ is zero; finally the mapping $\lambda^0$ associates to the class of $f$ modulo $\{0\}$ the homomorphism $\varphi : H_0(C) \to H^0(C')$ such that $f = i \circ \varphi \circ p$, whence the proposition.

Let $u : \tilde{C} \to C$ and $u' : C' \to \tilde{C}'$ be morphisms of complexes; then the canonical homomorphism $\mathrm{Homgr}_A (u, u') : \mathrm{Homgr}_A (C, C') \to \mathrm{Homgr}_A (\tilde{C}, \tilde{C}')$, defined by $f \mapsto u' \circ f \circ u$, is a morphism of complexes, as follows immediately from formula (1). Moreover, the following diagram is commutative

$$
\begin{array}{ccc}
H(\mathrm{Homgr}_A(C, C')) & \xrightarrow{\lambda(C, C')} & \mathrm{Homgr}_A(H(C), H(C')) \\
\downarrow H(\mathrm{Homgr}_A(u, u')) & & \downarrow \mathrm{Homgr}_A(H(u), H(u')) \\
H(\mathrm{Homgr}_A(\tilde{C}, \tilde{C}')) & \xrightarrow{\lambda(\tilde{C}, \tilde{C}') } & \mathrm{Homgr}_A(H(\tilde{C}), H(\tilde{C}')) .
\end{array}
$$

#### Proposition 2 {#alg-x-s5-prop-2 .statement}

*a) Let $C' \xrightarrow{u} C \xrightarrow{v} C''$ be an exact sequence of $A$-complexes, $P$ a projective complex, $E$ an injective complex (X, p. 25). Then the sequences*

$$
\mathrm{Homgr}_A(P, C') \xrightarrow{\mathrm{Homgr}(1,u)} \mathrm{Homgr}_A(P, C) \xrightarrow{\mathrm{Homgr}(1,v)} \mathrm{Homgr}_A(P, C'')
$$

*and*

$$
\mathrm{Homgr}_A(C'', E) \xrightarrow{\mathrm{Homgr}(v,1)} \mathrm{Homgr}_A(C, E) \xrightarrow{\mathrm{Homgr}(u,1)} \mathrm{Homgr}_A(C', E)
$$

*are exact sequences of complexes of $k$-modules.*

*b) Let $0 \to C' \xrightarrow{u} C \xrightarrow{v} C'' \to 0$ be a sequence of $A$-complexes which is split as an exact sequence of graded $A$-modules (this is the case for example if $C'$ is injective, or if $C''$ is projective). Then for any complex $E$, the sequences*

$$
0 \to \mathrm{Homgr}_A(E, C') \xrightarrow{\mathrm{Homgr}(1,u)} \mathrm{Homgr}_A(E, C) \xrightarrow{\mathrm{Homgr}(1,v)} \mathrm{Homgr}_A(E, C'') \to 0
$$

$$
0 \to \mathrm{Homgr}_A(C'', E) \xrightarrow{\mathrm{Homgr}(v,1)} \mathrm{Homgr}_A(C, E) \xrightarrow{\mathrm{Homgr}(u,1)} \mathrm{Homgr}_A(C', E) \to 0
$$

*are exact sequences of complexes of $k$-modules.*

In case *a)*, we remark that the sequences

$$
\mathrm{Hom}_A(P_p, C'_q) \to \mathrm{Hom}_A(P_p, C_q) \to \mathrm{Hom}_A(P_p, C''_q)
$$

*and*

$$
\mathrm{Hom}_A(C''_q, E_p) \to \mathrm{Hom}_A(C_q, E_p) \to \mathrm{Hom}_A(C'_q, E_p)
$$

are exact for all $p, q \in \mathbf{Z}$, and we apply II, p. 10, prop. 5 and II, p. 13, prop. 7. The proof of *b)* is analogous.

### 2. Complexes of homomorphisms and homotopies

#### Proposition 3 {#alg-x-s5-prop-3 .statement}

*Let $C, \tilde{C}, C', \tilde{C}'$ be four $A$-complexes, $u : \tilde{C} \to C, v : \tilde{C} \to C, u' : C' \to \tilde{C}'$ and $v' : C' \to \tilde{C}'$ four morphisms of complexes.

a) If $u$ and $u'$ are homotopic to $v$ and $v'$ respectively, then the two morphisms $\mathrm{Homgr}_A(u, u')$ and $\mathrm{Homgr}_A(v, v')$ from $\mathrm{Homgr}_A(C, C')$ to $\mathrm{Homgr}_A(\tilde{C}, \tilde{C}')$ are homotopic.

b) If $u$ and $u'$ are homotopisms, $\mathrm{Homgr}_A(u, u')$ is a homotopism.

c) If $C$ or $C'$ is homotopic to zero, $\mathrm{Homgr}_A(C, C')$ is homotopic to zero.*

Let us denote by the same letter $d$ the differentials of the complexes $C$, $C_1$, $C'$, $C'_1$, and by $D$ the differentials of $\mathrm{Homgr}_A(C,C')$ and $\mathrm{Homgr}_A(C_1,C'_1)$. If $u$ (resp. $u'$) is homotopic to $v$ (resp. $v'$), there exists a graded homomorphism of degree $1$,

$$
w:C_1\to C\qquad\text{(resp. }w':C'\to C'_1\text{)}
$$

such that

$$
\tag{2}
u-v=dw+wd\qquad\text{(resp. }u'-v'=dw'+w'd\text{)}
$$

Let $W:\mathrm{Homgr}_A(C,C')\to\mathrm{Homgr}_A(C_1,C'_1)$ be the graded homomorphism of degree $1$ such that, for $f\in\mathrm{Homgr}_A(C,C')_n$, $n\in\mathbf{Z}$, one has

$$
\tag{3}
W(f)=w'fu+(-1)^n v'fw.
$$

We then have

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

This is written as $DW+WD=\mathrm{Homgr}_A(u,u')-\mathrm{Homgr}_A(v,v')$, whence a).

Let us prove b). If $u$ and $u'$ are homotopy equivalences, let $\alpha:C\to\widetilde C$ and $\alpha':\widetilde C'\to C'$ be morphisms of complexes such that $u\circ\alpha$, $\alpha\circ u$, $u'\circ\alpha'$, $\alpha'\circ u'$ are homotopic respectively to $\mathrm{Id}_C$, $\mathrm{Id}_{\widetilde C}$, $\mathrm{Id}_{\widetilde C'}$, $\mathrm{Id}_{C'}$. Then $\mathrm{Homgr}(u,u')\circ\mathrm{Homgr}(\alpha,\alpha')$, which is equal to $\mathrm{Homgr}(\alpha\circ u,u'\circ\alpha')$, is homotopic by a) to

$$
\mathrm{Homgr}_A(\mathrm{Id}_C,\mathrm{Id}_{C'})=\mathrm{Id}_{\mathrm{Homgr}_A(C,C')};
$$

analogously $\mathrm{Homgr}(\alpha,\alpha')\circ\mathrm{Homgr}(u,u')$ is homotopic to $\mathrm{Id}_{\mathrm{Homgr}(\widetilde C,\widetilde C')}$, whence b).

Finally c) follows from b) (applied to the case where $\widetilde C$ or $\widetilde C'$ is zero).

#### Corollary 1 {#alg-x-s5-prop-3-cor-1 .statement}

If $C$ is split and $H(C)$ projective (resp. if $C'$ is split and $H_n(C')$ injective for each $n$), then the canonical homomorphism

$$
\lambda(C,C'):\ H(\mathrm{Homgr}_A(C,C'))\to\mathrm{Homgr}_A(H(C),H(C'))
$$

is bijective.

Suppose for example $C'$ split and $H(C')$ injective for each $n$, the case where $C$ is split and $H(C)$ projective being proved in an analogous manner. By X, p. 35, def. 6, there exists a homotopy equivalence $u':C'\to H(C')$ ; by Proposition 3, $\mathrm{Homgr}_A(1,u')$ is a homotopy equivalence from $\mathrm{Homgr}_A(C,C')$ onto $\mathrm{Homgr}_A(C,H(C'))$ ; since

$$
\mathrm{Homgr}_A(1,H(u'))\circ\lambda(C,C')=\lambda(C,H(C'))\circ H(\mathrm{Homgr}_A(1,u'))
$$

and that $\mathrm{Homgr}_A(1,H(u'))$ and $H(\mathrm{Homgr}_A(1,u'))$ are bijective, it is enough for us to prove that $\lambda(C, H(C'))$ is bijective, which brings us back to the case where $C'$ is injective and has zero differential.

The canonical exact sequences (X, p. 28)

(III) $$
0 \to B(C) \xrightarrow{i} C \xrightarrow{\delta} C/B(C) \to 0
$$
(IV) $$
0 \to H(C) \xrightarrow{j} C/B(C) \xrightarrow{\delta} B(C) \to 0
$$

give exact sequences (X, p. 83, Proposition 2, a))

$$
0 \to \mathrm{Homgr}_A(C/B(C), C') \xrightarrow{l'} \mathrm{Homgr}_A(C, C') \xrightarrow{l} \mathrm{Homgr}_A(B(C), C') \to 0
$$
$$
0 \to \mathrm{Homgr}_A(B(C), C') \xrightarrow{\Delta} \mathrm{Homgr}_A(C/B(C), C') \xrightarrow{j} \mathrm{Homgr}_A(H(C), C') \to 0 .
$$

Since $d_C = i \circ \delta \circ p$, the differential $D$ of $\mathrm{Homgr}_A(C, C')$ is given by $D_n = (-1)^{n+1} P_n \circ \Delta_n \circ l_n$; we then have

$$
\mathrm{Z}(\mathrm{Homgr}_A(C, C')) = \mathrm{Ker}\,(P \circ \Delta \circ I) = \mathrm{Ker}\,I = \mathrm{Im}\,P,
$$
$$
\mathrm{B}(\mathrm{Homgr}_A(C, C')) = \mathrm{Im}\,(P \circ \Delta \circ I) = P(\mathrm{Im}\,\Delta) = P(\mathrm{Ker}\,J) ;
$$

whence an isomorphism $\varphi : H(\mathrm{Homgr}_A(C, C')) \to \mathrm{Homgr}_A(H(C), C')$ such that, if $a \in \mathrm{Homgr}_A(C/B(C), C')$, the image of the class of $P(a)$ under $\varphi$ is $J(a)$; we immediately verify that $\varphi$ coincides with the canonical homomorphism $\lambda$.

#### Corollary 2 {#alg-x-s5-prop-3-cor-2 .statement}

Assume that $B(C)$ and $H(C)$ are projective (resp. $B_n(C')$ and $H_n(C')$ are injective for every $n$). Then $\lambda(C, C')$ is bijective.

Indeed, $C$ (resp. $C'$) is then split, by X, p. 35, Example 4, and we apply Corollary 1.

#### Corollary 3 {#alg-x-s5-prop-3-cor-3 .statement}

Let $M$ be a projective $A$-module (resp. an injective $A$-module). For every complex $C$ of $A$-modules and every integer $n$, the canonical homomorphism

$$
H^n(\mathrm{Homgr}_A(M, C)) \to \mathrm{Hom}_A(M, H^n(C))
$$

(resp. $H^n(\mathrm{Homgr}_A(C, M)) \to \mathrm{Hom}_A(H_n(C), M)$) is bijective.

#### Lemma 1 {#alg-x-s5-lem-1 .statement}

a) If $C$ or $C'$ is bounded on the right, if $C$ is projective and if $H(C') = 0$, then $H(\mathrm{Homgr}_A(C, C')) = 0$.
    b) If $C$ or $C'$ is bounded on the left, if $C'$ is injective and if $H(C) = 0$, then $H(\mathrm{Homgr}_A(C, C')) = 0$.

Let $f \in Z_n(\mathrm{Homgr}_A(C, C'))$; $f$ is then a morphism of complexes from $C$ to $C'(n)$; in case a) (resp. b)), $f_m$ vanishes for $m$ sufficiently small (resp. sufficiently large). By X, p. 47, Proposition 1, $f$ is then homotopic to zero, hence belongs to $B_n(\mathrm{Homgr}_A(C, C'))$, which gives the conclusion.

#### Proposition 4 {#alg-x-s5-prop-4 .statement}

Let $u : C' \to C$ be a morphism of complexes, $P$ a projective complex, $E$ an injective complex.

a) If $P$ is bounded on the right, or if $C$ and $C'$ are bounded on the right, then

$$
\operatorname{Homgr}_A(1, u) : \operatorname{Homgr}_A(P, C') \to \operatorname{Homgr}_A(P, C)
$$

is a morphism.

b) If $E$ is bounded on the left, or if $C$ and $C'$ are bounded on the left, then

$$
\operatorname{Homgr}_A(u, 1) : \operatorname{Homgr}_A(C, E) \to \operatorname{Homgr}_A(C', E)
$$

is a morphism.

Assume first that $u$ is injective and set $C'' = \operatorname{Coker}\ u$. Since $u$ is a morphism, $C''$ is of zero homology. We have, on the other hand, exact sequences (Proposition 2)

==========

By Lemma 1, $\operatorname{Homgr}_A(P, C'')$ is of zero homology in case $a$, $\operatorname{Homgr}_A(C'', E)$ is of zero homology in case $b$, hence the conclusion.

In the general case, there exists (X, p. 38, cor. to Prop. 7) a complex $\tilde{C}'$, which is right-bounded (resp. left-bounded) when $C$ and $C'$ are, an injective morphism $\tilde{u}: C' \to \tilde{C}'$ and a homotopy $\beta: \tilde{C}' \to C$ such that $u = \beta \circ \tilde{u}$. Then $\tilde{u}$ is a *morphism* (X, p. 34, cor. to Prop. 5); by what was shown above, $\operatorname{Homgr}_A(l_P, \tilde{u})$ (resp. $\operatorname{Homgr}_A(\tilde{u}, l_E)$) is a morphism in case $a$ (resp. $b$). Moreover, $\operatorname{Homgr}_A(l_P, \beta)$ (resp. $\operatorname{Homgr}_A(\beta, l_E)$) is a homotopy (Prop. 3); therefore, $\operatorname{Homgr}_A(l_P, u)$ (resp. $\operatorname{Homgr}_A(u, l_E)$) is the composite of two morphisms, hence is a morphism.

### 3. Definition and First Properties of Extension Modules

For any $A$-module $E$, we denote by $p_E : L(E) \to E$ (resp. $e_E : E \to I(E)$) the canonical free (resp. injective) resolution, cf. X, p. 50 (resp. p. 52).

#### Definition 1 {#alg-x-s5-def-1 .statement}

Let $M$ and $N$ be two $A$-modules. The module of extensions of $N$ by $M$ is the graded $k$-module

$$
\text{(4)} \quad \operatorname{Ext}_A(M, N) = H(\operatorname{Homgr}_A(L(M), I(N))) .
$$

The homogeneous components of $\operatorname{Ext}_A(M, N)$ are denoted

$$
\text{(5)} \quad \operatorname{Ext}_A^n(M, N) = H^n(\operatorname{Homgr}_A(L(M), I(N))) .
$$

As $L(M)$ (resp. $I(N)$) is zero to the right (resp. to the left), we have

(6)
$$
\operatorname{Ext}^{n}_{A}(M,N)=0\qquad\text{pour }n<0.
$$

#### Remark 1 {#alg-x-s5-n3-rem-1 .statement}

We will see below (X, p. 107, Prop. 6) some finiteness properties of the modules $\operatorname{Ext}^{n}_{A}(M,N)$. For example, if $A$ is commutative and noetherian, and if $M$ and $N$ are $A$-modules of finite type, each $A$-module $\operatorname{Ext}^{n}_{A}(M,N)$ is of finite type.

Let $f : M' \to M$ and $g : N \to N’$ be homomorphisms of $A$-modules. Set

$$
\operatorname{Ext}_{A}(f,g)=H(\operatorname{Homgr}_{A}(L(f),I(g))) \,;
$$

this is a homomorphism of degree 0 of graded $k$-modules

$$
\operatorname{Ext}_{A}(f,g):\operatorname{Ext}_{A}(M,N)\to\operatorname{Ext}_{A}(M',N')\,,
$$

whose homogeneous components are denoted

$$
\operatorname{Ext}^{n}_{A}(f,g):\operatorname{Ext}^{n}_{A}(M,N)\to\operatorname{Ext}^{n}_{A}(M',N')\,.
$$

According to Prop. 1 of [X], p. 82, the canonical homomorphism

$$
\lambda^{0}(L(M),I(N)):H^{0}(\operatorname{Homgr}_{A}(L(M),I(N)))
\to\operatorname{Hom}_{A}(H_{0}(L(M)),H^{0}(I(N)))
$$

is bijective; using the isomorphisms $M\to H_{0}(L(M))$ and $H^{0}(I(N))\to N$, one deduces a *canonical isomorphism*

(7)
$$
\lambda_{M,N}:\operatorname{Ext}^{0}_{A}(M,N)\to\operatorname{Hom}_{A}(M,N)\,.
$$

*We will always identify* $\operatorname{Ext}^{0}_{A}(M,N)$ with $\operatorname{Hom}_{A}(M,N)$ via this isomorphism. Then the $k$-linear map $\operatorname{Ext}_{A}(f,g)$ can be identified with $\operatorname{Hom}_{A}(f,g)$.

#### Remark 2 {#alg-x-s5-n3-rem-2 .statement}

The morphism of complexes

$$
\operatorname{Homgr}_{A}(p_{M},\epsilon_{N}):\operatorname{Hom}_{A}(M,N)\to\operatorname{Homgr}_{A}(L(M),I(N))
$$

induces on the homology in degree 0 the isomorphism

$$
\lambda^{-1}_{M,N}:\operatorname{Hom}_{A}(M,N)\to\operatorname{Ext}^{0}_{A}(M,N)
$$

reciprocal to $\lambda_{M,N}$.

We have $L(1_{M})=1_{L(M)}$, $I(1_{N})=1_{I(N)}$, hence by passing to homology

(8)
$$
\operatorname{Ext}_{A}(1_{M},1_{N})=1_{\operatorname{Ext}_{A}(M,N)}\,.
$$

If $f' : M''\to M'$ and $g' : N'\to N''$ are $A$-module homomorphisms, we have $L(f\circ f')=L(f)\circ L(f')$, $I(g'\circ g)=I(g')\circ I(g)$, and thus...

(9)
$$
\operatorname{Ext}_{A}(f\circ f',g'\circ g)=\operatorname{Ext}_{A}(f',g')\circ\operatorname{Ext}_{A}(f,g)\,.
$$

Consider the morphisms of $k$-complexes
$$
\operatorname{Homgr}_A(L(M), N) \xrightarrow{\operatorname{Homgr}_A(1, e_N)} \operatorname{Homgr}_A(L(M), I(N)) \xleftarrow{\operatorname{Homgr}_A(p_M, 1)} \operatorname{Homgr}_A(M, I(N)),
$$
and the homomorphisms they induce in homology:
$$
H(\operatorname{Homgr}_A(L(M), N)) \xrightarrow{\varphi_{M(N)}} \operatorname{Ext}_A(M, N) \xleftarrow{\overline{\varphi}_{N(M)}} H(\operatorname{Homgr}_A(M, I(N))) .
$$
According to Proposition 4 of X, p. 86, $\operatorname{Homgr}_A(1, e_N)$ and $\operatorname{Homgr}_A(p_M, 1)$ are homologisms, hence:

#### Proposition 5 {#alg-x-s5-prop-5 .statement}

*The $k$-homomorphisms*
$$
\begin{aligned}
&\varphi_M(N) : H(\operatorname{Homgr}_A(L(M), N)) \to \operatorname{Ext}_A(M, N) \\
&\text{and} \quad \overline{\varphi}_N(M) : H(\operatorname{Homgr}_A(M, I(N))) \to \operatorname{Ext}_A(M, N) \text{ are bijective}.
\end{aligned}
$$

#### Corollaire {#alg-x-s5-n3-cor-1 .statement}

If $M$ is projective (resp. if $N$ is injective), then $\operatorname{Ext}_A^i(M, N) = 0$ for $i > 0$.
Indeed, $\operatorname{Homgr}_A(1, e_N) : \operatorname{Hom}_A(M, N) \to \operatorname{Homgr}_A(M, I(N))$ (resp. $\operatorname{Homgr}_A(p_M, 1) : \operatorname{Hom}_A(M, N) \to \operatorname{Homgr}_A(L(M), N)$) is then a homologism (X, p. 86, Prop. 4), yielding the conclusion.

*Remarks. — 3)* Let $g : N \to N'$ be a homomorphism of $A$-modules. Then
$$
\operatorname{Homgr}_A(1_{L(M)}, g) \circ \operatorname{Homgr}_A(1_{L(M)}, e_N) = \operatorname{Homgr}_A(1_{L(M)}, e_{N'}) \circ \operatorname{Homgr}_A(1_{L(M)}, I(g)),
$$
and hence the diagram
$$
\begin{array}{ccc}
H(\operatorname{Homgr}_A(L(M), N)) & \xrightarrow{\varphi_{M(N)}} & \operatorname{Ext}_A(M, N) \\
\operatorname{H}(\operatorname{Homgr}_A(1_{L(M)}, g)) \downarrow & & \downarrow \operatorname{Ext}_A(1_M, g) \\
H(\operatorname{Homgr}_A(L(M), N')) & \xrightarrow{\varphi_{M(N')}} & \operatorname{Ext}_A(M, N')
\end{array}
$$
is commutative.

4) Analogously, if $f : M' \to M$ is a homomorphism of $A$-modules, the diagram
$$
\begin{array}{ccc}
H(\operatorname{Homgr}_A(M, I(N))) & \xrightarrow{\overline{\varphi}_{N(M)}} & \operatorname{Ext}_A(M, N) \\
\operatorname{H}(\operatorname{Homgr}_A(f, 1_{I(N)})) \downarrow & & \downarrow \operatorname{Ext}_A(f, 1_N) \\
H(\operatorname{Homgr}_A(M', I(N))) & \xrightarrow{\overline{\varphi}_{N(M')}} & \operatorname{Ext}_A(M', N)
\end{array}
$$
is commutative.

#### Proposition 6 {#alg-x-s5-prop-6 .statement}

The mapping $(f,g) \mapsto \operatorname{Ext}_A(f,g) :$
$$
\operatorname{Hom}_A(M',M)\times\operatorname{Hom}_A(N,N')\longrightarrow
\operatorname{Homgr}_k\bigl(\operatorname{Ext}_A(M,N),\operatorname{Ext}_A(M',N')\bigr)
$$
is $k$-bilinear.

Let $f\in\operatorname{Hom}_A(M',M)$, $g_1,g_2\in\operatorname{Hom}_A(N,N')$, $\lambda_1,\lambda_2\in k$. The morphisms $\operatorname{Homgr}_A(L(f),\lambda_1g_1+\lambda_2g_2)$ and $\lambda_1\operatorname{Homgr}_A(L(f),g_1)+\lambda_2\operatorname{Homgr}_A(L(f),g_2)$ from $\operatorname{Homgr}_A(L(M),N)$ to $\operatorname{Homgr}_A(L(M),N')$ coincide, hence, by Proposition 5 and Remark 3,

(10)     $\operatorname{Ext}_A(f,\lambda_1g_1+\lambda_2g_2)=\lambda_1\operatorname{Ext}_A(f,g_1)+\lambda_2\operatorname{Ext}_A(f,g_2)$.

Argue similarly for the mapping $f \mapsto \operatorname{Ext}_A(f,g)$.

#### Corollaire {#alg-x-s5-n3-cor-2 .statement}

Let $\lambda \in k$. If $\lambda$ annihilates $M$ or $N$, then it annihilates $\operatorname{Ext}_A(M,N)$. Indeed, $\lambda \cdot 1_{\operatorname{Ext}_A(M,N)} = \operatorname{Ext}_A(\lambda 1_M, 1_N) = \operatorname{Ext}_A(1_M, \lambda 1_N)$.

#### Proposition 7 {#alg-x-s5-prop-7 .statement}

Let $I$ and $J$ be two sets, $(M_\alpha)_{\alpha\in I}$ and $(N_\beta)_{\beta\in J}$ two families of $A$-modules; the homomorphism
$$
\operatorname{Ext}_A\left(\bigoplus_{\alpha\in I}M_\alpha,\prod_{\beta\in J}N_\beta\right)
\longrightarrow
\prod_{\substack{\beta\in J,\ \alpha\in I}}
\operatorname{Ext}_A(M_\alpha,N_\beta)
$$
induced by the canonical homomorphisms $M_\alpha \to \bigoplus_{\alpha\in I} M_\alpha$ and $\prod_{\beta\in J} N_\beta \to N_\beta$ is bijective.

It suffices to prove that for every $A$-module $M$ (resp. $N$), the homomorphisms
$$
\operatorname{Ext}(M, \prod_\beta N_\beta) \to \prod_\beta \operatorname{Ext}(M,N_\beta)
$$
(resp. $\operatorname{Ext}(\bigoplus M_\alpha,N)\to\prod_\alpha\operatorname{Ext}(M_\alpha,N)$)
are bijective. This follows from what has already been shown, from Proposition 1 of X, p. 28, and the canonical isomorphisms $\operatorname{Homgr}_A(L(M), \prod N_\beta) \to \prod \operatorname{Homgr}_A(L(M),N_\beta)$ and $\operatorname{Homgr}_A(\bigoplus M_\alpha, I(N)) \to \prod \operatorname{Homgr}_A(M_\alpha, I(N))$.

#### Remarque 5 {#alg-x-s5-n3-rem-5 .statement}

Let $P^\circ$ and $Q^\circ$ be two right $A$-modules. We define $\operatorname{Ext}_A(P,Q)$ by

$$
\operatorname{Ext}_A(P,Q)=H(\operatorname{Homgr}_A(L(P),I(Q)))=H(\operatorname{Homgr}_{A^\circ}(L(P^\circ),I(Q^\circ)))
$$

$$
=\operatorname{Ext}_{A^\circ}(P^\circ,Q^\circ).
$$

All the definitions and propositions of this paragraph therefore apply to right $A$-modules by considering them as left modules over the ring $A^\circ$.

### 4. The connecting homomorphisms and exact sequences

Let $M$ be an $A$-module. Recall that for every $A$-module $N$, we defined in the previous number an isomorphism of $k$-modules

$$
\varphi_M(N):H(\operatorname{Homgr}_A(L(M),N))\longrightarrow\operatorname{Ext}_A(M,N).
$$

Let

$$(\mathcal{E})\qquad 0\longrightarrow N'\xrightarrow{u}N\xrightarrow{v}N''\longrightarrow0$$

Bourbaki. — Algèbre X                                                                                                                             4 an exact sequence of $A$-modules ; the sequence of $k$-complexes

$$
(\mathcal{E}) \quad 0 \longrightarrow \operatorname{Homgr}_A(L(M), N') \xrightarrow{\operatorname{Homgr}(1,u)} \operatorname{Homgr}_A(L(M), N) \\
\phantom{(M\mathcal{E})} \phantom{0} \xrightarrow{\operatorname{Homgr}(1,v)} \operatorname{Homgr}_A(L(M), N'') \longrightarrow 0
$$

is then exact ($X$, p. 83, prop. 2, $a$), let

$$
\partial_{(M\mathcal{E})} : H(\operatorname{Homgr}_A(L(M), N'')) \to H(\operatorname{Homgr}_A(L(M), N'))
$$

be the corresponding connecting homomorphism ($X$, p. 29).

#### Definition 2 {#alg-x-s5-def-2 .statement}

*We call the composite homomorphism the connecting homomorphism of the extension modules relative to the module $M$ and to the exact sequence $\mathcal{E}$*

$$
\delta(M, \mathcal{E}) = \varphi_M(N') \circ \partial_{(M\mathcal{E})} \circ \varphi_M(N'')^{-1} : \operatorname{Ext}_A(M, N'') \to \operatorname{Ext}_A(M, N')
$$

This is a graded $k$-homomorphism of ascending degree 1, whose homogeneous components are denoted $\delta^n(M, \mathcal{E}) : \operatorname{Ext}_A^n(M, N'') \to \operatorname{Ext}_A^{n+1}(M, N')$.

#### Theorem 1 {#alg-x-s5-thm-1 .statement}

*The right-unbounded sequence of homomorphisms of $k$-modules*

$$
0 \longrightarrow \operatorname{Hom}_A(M, N') \xrightarrow{\operatorname{Hom}(1,u)} \operatorname{Hom}_A(M, N) \xrightarrow{\operatorname{Hom}(1,v)} \operatorname{Hom}_A(M, N'')
$$
$$
\phantom{0} \xrightarrow{\delta_{(M,\mathcal{E})}} \operatorname{Ext}_A^1(M, N') \to \cdots \xrightarrow{\delta^{n-1}(M,\mathcal{E})} \operatorname{Ext}_A^n(M, N') \xrightarrow{\operatorname{Ext}^n(1,u)} \operatorname{Ext}_A^n(M, N)
$$
$$
\phantom{0} \xrightarrow{\operatorname{Ext}^n(1,v)} \operatorname{Ext}_A^n(M, N'') \xrightarrow{\delta^n(M,\mathcal{E})} \operatorname{Ext}_A^{n+1}(M, N') \to \cdots
$$

*is exact*.

Consider indeed the diagram on page X.91.
It is commutative by the *remark* 3 of $X$, p. 88 and def. 2 ; moreover the bottom row is exact ($X$, p. 30, th. 1), and the vertical arrows are bijective ($X$, p. 88, prop. 5).

#### Corollary {#alg-x-s5-n4-cor-1 .statement}

*If* $\operatorname{Ext}_A^1(M, N') = 0$, *the sequence*

$$
0 \longrightarrow \operatorname{Hom}_A(M, N') \xrightarrow{\operatorname{Hom}(1,u)} \operatorname{Hom}_A(M, N) \xrightarrow{\operatorname{Hom}(1,v)} \operatorname{Hom}_A(M, N'') \longrightarrow 0
$$

*is exact*.

#### Proposition 8 {#alg-x-s5-prop-8 .statement}

*Let* $f : M_1 \to M$ *be a homomorphism of* $A$*-modules* and

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

a commutative diagram of $A$-modules with exact rows. The diagram of $k$-modules

$$
\begin{array}{ccc}
\mathrm{Ext}_A(M, N'') & \xrightarrow{\delta(M, \mathscr{E})} & \mathrm{Ext}_A(M, N') \\
\mathrm{Ext}(f, g'') \downarrow & & \mathrm{Ext}(f, g') \downarrow \\
\mathrm{Ext}_A(M_1, N''_1) & \xrightarrow{\delta(M, \mathscr{E}_1)} & \mathrm{Ext}_A(M_1, N'_1)
\end{array}
$$

is commutative.
This follows from X, p. 31, prop. 2 applied to the commutative diagram

$$
\begin{array}{ccccccccc}
& & \mathrm{Homgr}(1, u) & & & & \mathrm{Homgr}(1, v) & & \\
0 \to \mathrm{Homgr}_A(L(M), N') & \to & \mathrm{Homgr}_A(L(M), N) & \to & \mathrm{Homgr}_A(L(M), N'') & \to & 0 \\
\mathrm{Homgr}(L(f), g') \downarrow & & \mathrm{Homgr}(L(f), g) \downarrow & & \mathrm{Homgr}(L(f), g'') \downarrow & & \\
0 \to \mathrm{Homgr}_A(L(M_1), N'_1) & \to & \mathrm{Homgr}_A(L(M_1), N_1) & \to & \mathrm{Homgr}_A(L(M_1), N''_1) & \to & 0
\end{array}
$$

Let $N$ be an $A$-module, and
$$(\mathcal{F})$$
$$0 \to M' \xrightarrow{r} M \xrightarrow{s} M'' \to 0$$
an exact sequence of $A$-modules; the sequence of complexes
$$(\mathcal{F}_N)$$
$$0 \longrightarrow \mathrm{Homgr}_A(M'', I(N)) \xrightarrow{\mathrm{Homgr}(s, 1)} \mathrm{Homgr}_A(M, I(N))$$
$$\xrightarrow{\mathrm{Homgr}(r, 1)} \mathrm{Homgr}_A(M', I(N)) \longrightarrow 0$$
is exact (X, p. 83, prop. 2, $a$) ; let
$$\partial(\mathcal{F}_N) : \mathrm{H}(\mathrm{Homgr}_A(M', I(N))) \to \mathrm{H}(\mathrm{Homgr}_A(M'', I(N)))$$
be the corresponding connecting homomorphism.

#### Definition 3 {#alg-x-s5-def-3 .statement}

One calls connecting homomorphism of extension modules relative to the exact sequence $(\mathcal{F})$ and to the module $N$, the composite homomorphism
$$\delta(\mathcal{F}, N) : \overline{\varphi}_N(M'') \circ \partial(\mathcal{F}_N) \circ \overline{\varphi}_N(M')^{-1} : \mathrm{Ext}_A(M', N) \to \mathrm{Ext}_A(M'', N).$$
It is a graded $k$-homomorphism of ascending degree 1, whose homogeneous components are denoted $\delta^n(\mathcal{F}, N) : \mathrm{Ext}_A^n(M', N) \to \mathrm{Ext}_A^{n+1}(M'', N)$.
One then proves as above the following statements:

#### Theorem 2 {#alg-x-s5-thm-2 .statement}

The right-unbounded sequence of homomorphisms of $k$-modules
$$0 \longrightarrow \mathrm{Hom}_A(M'', N) \xrightarrow{\mathrm{Hom}(s, 1)} \mathrm{Hom}_A(M, N) \xrightarrow{\mathrm{Hom}(r, 1)} \mathrm{Hom}_A(M', N)$$
$$\xrightarrow{\delta^0(\mathcal{F}, N)} \mathrm{Ext}_A^1(M'', N) \to \cdots \xrightarrow{\delta^{n-1}(\mathcal{F}, N)} \mathrm{Ext}_A^n(M'', N) \xrightarrow{\mathrm{Ext}^n(s, 1)} \mathrm{Ext}_A^n(M, N)$$
$$\xrightarrow{\mathrm{Ext}^n(r, 1)} \mathrm{Ext}_A^n(M', N) \xrightarrow{\delta^n(\mathcal{F}, N)} \mathrm{Ext}_A^{n+1}(M'', N) \to \cdots$$
is exact.

#### Corollary {#alg-x-s5-n4-cor-2 .statement}

If $\operatorname{Ext}_A^1(M'', N) = 0$, the sequence

$$
0 \longrightarrow \operatorname{Hom}_A(M'', N) \xrightarrow{\operatorname{Hom}(s, 1)} \operatorname{Hom}_A(M, N) \xrightarrow{\operatorname{Hom}(r, 1)} \operatorname{Hom}_A(M', N) \longrightarrow 0
$$

is exact.

#### Proposition 9 {#alg-x-s5-prop-9 .statement}

Let $g : N \to N_1$ be a homomorphism of $A$-modules and

$$
\begin{array}{cccccc}
(\mathcal{F}_1) & 0 \to M'_1 \xrightarrow{r_1} M_1 \xrightarrow{s_1} M''_1 \to 0 \\
& f' \downarrow & f \downarrow & f'' \downarrow \\
(\mathcal{F}) & 0 \to M' \xrightarrow{r} M \xrightarrow{s} M'' \to 0
\end{array}
$$

a commutative diagram of $A$-modules with exact rows. The diagram of $k$-modules

$$
\begin{array}{ccc}
\operatorname{Ext}_A(M', N) & \xrightarrow{\delta(\mathcal{F}, N)} & \operatorname{Ext}_A(M'', N) \\
\operatorname{Ext}_A(f', g) \downarrow & & \operatorname{Ext}_A(f'', g) \downarrow \\
\operatorname{Ext}_A(M'_1, N_1) & \xrightarrow{\delta(\mathcal{F}_1, N_1)} & \operatorname{Ext}_A(M''_1, N_1)
\end{array}
$$

is commutative.

### 5. Projective modules, injective modules and extension modules

#### Proposition 10 {#alg-x-s5-prop-10 .statement}

Let $M$ be an $A$-module. The following conditions are equivalent:

(i) $M$ is projective.
(ii) $\operatorname{Ext}_A^i(M, N) = 0$ for every $A$-module $N$ and for every integer $i > 0$.
(iii) $\operatorname{Ext}_A^1(M, N) = 0$ for every $A$-module $N$.
(iv) There exists an exact sequence

$$
0 \to K \xrightarrow{\nu} P \xrightarrow{\iota} M \to 0,
$$

where $P$ is projective, and where $\operatorname{Ext}_A^1(M, K) = 0$.

(i) $\Rightarrow$ (ii) : this is the corollary of prop. 5 of X, p. 88.
(ii) $\Rightarrow$ (iii) : this is trivial.
(iii) $\Rightarrow$ (iv) : this is clear since $M$ is quotient of a free module $P$.
(iv) $\Rightarrow$ (i) : since $\operatorname{Ext}_A^1(M, K) = 0$, the canonical mapping

$$
\operatorname{Hom}_A(M, P) \to \operatorname{Hom}_A(M, M)
$$

is surjective (X, p. 90, corollary); hence there exists an $A$-linear section of $\nu$ and $M$ is isomorphic to a direct factor of $P$, and therefore is projective.

#### Proposition 11 {#alg-x-s5-prop-11 .statement}

Let $N$ be an $A$-module. The following conditions are equivalent:

(i) $N$ is injective.
(ii) $\operatorname{Ext}_A^i(M, N) = 0$ for every $A$-module $M$ and every integer $i > 0$.

(iii) $\mathrm{Ext}_A^1(M, N) = 0$ for every $A$-module $M$.

(iv) There exists an exact sequence

$$
0 \to N \xrightarrow{u} I \xrightarrow{v} C \to 0,
$$

where $I$ is injective and where $\mathrm{Ext}_A^1(C, N) = 0$;

(v) $\mathrm{Ext}_A^1(M, N) = 0$ for every cyclic $A$-module $M$.

(i) $\Rightarrow$ (ii) : this is the corollary of Prop. 5 of X, p. 88.

(ii) $\Rightarrow$ (iii) $\Rightarrow$ (v) : this is trivial.

(iii) $\Rightarrow$ (iv) : this is clear since $N$ is a submodule of an injective module (X, p. 19, Cor. 3).

(iv) $\Rightarrow$ (i) : since $\mathrm{Ext}_A^1(C, N) = 0$, the canonical homomorphism

$$
\mathrm{Hom}_A(I, N) \to \mathrm{Hom}_A(N, N)
$$

is surjective (X, p. 93, Corollary); there therefore exists an $A$-linear retraction of $u$ and $N$ is isomorphic to a direct factor of $I$, hence is injective (X, p. 16, Prop. 9).

(v) $\Rightarrow$ (i) : if $\alpha$ is an ideal of $A$, we have $\mathrm{Ext}_A^1(A/\alpha, N) = 0$; the canonical mapping $\mathrm{Hom}_A(A, N) \to \mathrm{Hom}_A(\alpha, N)$ is therefore surjective and $N$ is injective (X, p. 16, Prop. 10).

### 6. Universal coefficient formula

In this number, we consider two complexes of $A$-modules $(C, d)$ and $(C', d')$. Let us consider the canonical exact sequences:

(I)

$$
0 \to Z(C) \xrightarrow{j} C \xrightarrow{\delta} B(C)(-1) \to 0,
$$

(II_p)

$$
0 \to B_p(C) \xrightarrow{i} Z_p(C) \xrightarrow{\rho} H_p(C) \to 0;
$$

from $\delta$ we derive a $k$-homomorphism

$$
H(\mathrm{Homgr}(\delta, 1)) : H(Homgr_A(B(C), C'))(1) \to H(Homgr_A(C, C'));
$$

from (II_p) we derive connecting homomorphisms:

$$
\delta(11_p, H^q(C')) : \mathrm{Hom}_A(B_p(C), H^q(C')) \to \mathrm{Ext}_A^1(H_p(C), H^q(C')) .
$$

hence, by passing to the product, homomorphisms of $k$-modules

$$
\varphi^n : \mathrm{Homgr}_A^n(B(C), H(C')) \to \prod_{p+q=n} \mathrm{Ext}_A^1(H_p(C), H^q(C'))
$$

We also have canonical homomorphisms (X, p. 82)

$$
\lambda^n(B(C), C') : H^n(Homgr_A(B(C), C')) \to \mathrm{Homgr}_A^n(B(C), H(C')) .
$$

With these notations:

#### Theorem 3 {#alg-x-s5-thm-3 .statement}

Suppose the $A$-modules $B(C)$ and $Z(C)$ are projective. There exists, for each $n$, a unique homomorphism of $k$-modules

$$
\beta^n : \prod_{p+q=n-1} \mathrm{Ext}_A^1(H_p(C), H^q(C')) \to H^n(\mathrm{Homgr}_A(C, C'))
$$

making the diagram

$$
\begin{array}{ccc}
\mathrm{Homgr}_A^{n-1}(B(C), H(C')) & \xleftarrow{\lambda^{n-1}(B(C), C')} & H^{n-1}(\mathrm{Homgr}_A(B(C), C')) \\
\downarrow \varphi^{n-1} & & \downarrow H^n(\mathrm{Homgr}(\delta, 1)) \\
\prod_{p+q=n-1} \mathrm{Ext}_A^1(H_p(C), H^q(C')) & \xrightarrow{\beta^n} & H^n(\mathrm{Homgr}_A(C, C')) .
\end{array}
$$

commutative.

The sequences of graded $k$-modules

(11) $0 \to \prod_{p+q=n-1} \mathrm{Ext}_A^1(H_p(C), H^q(C')) \xrightarrow{\beta^n} H^n(\mathrm{Homgr}_A(C, C'))$

$$
\xrightarrow{\lambda^n(C, C')} \prod_{p+q=n} \mathrm{Hom}_A(H_p(C), H^q(C')) \to 0
$$

are exact.

#### Remark {#alg-x-s5-n6-rem-1 .statement}

One can prove an analogous statement, assuming $B_n(C')$ and $C'/B_n(C')$ are injective for each $n$.

Set for simplicity $B = B(C)$, $Z = Z(C)$, $H = H(C)$ and $H' = H(C')$. Since $B$ is projective, we derive from (1) an exact sequence

(12) $0 \to \mathrm{Homgr}_A(B, C')(1) \xrightarrow{\mathrm{Homgr}(\delta, 1)} \mathrm{Homgr}_A(C, C')$

$$
\xrightarrow{\mathrm{Homgr}(i, 1)} \mathrm{Homgr}_A(Z, C') \to 0 .
$$

#### Lemma 2 {#alg-x-s5-lem-2 .statement}

The connecting homomorphism

$$
H^n(\mathrm{Homgr}_A(Z, C')) \to H^n(\mathrm{Homgr}_A(B, C'))
$$

associated to (12) is equal to $(-1)^{n+1} H(\mathrm{Homgr}(i, 1))$.

Proof. Indeed, let $a \in Z^n(\mathrm{Homgr}_A(Z, C'))$; this is a morphism of complexes of ascending degree $n$ from $Z$ to $C'$, whose values are therefore in $Z(C')$. Since the exact sequence (1) is split ($B$ being projective), $a$ extends to an element $b$ of $\mathrm{Homgr}_A^n(C, Z(C'))$. By definition, the image of the class of $a$ by the connecting homomorphism in question is the class in $H^n(\mathrm{Homgr}_A(B, C'))$ of the homomorphism $u$ from $B(C)$ to $C'$ such that for $x \in C$, we have

$$
u(dx) = Db(x) = d'b(x) - (-1)^n b(dx) = (-1)^{n+1} b(dx) = (-1)^{n+1} a(dx),
$$

hence the assertion.

The homology exact sequence associated to (12) therefore gives the exact sequence
→ H^n(\mathrm{Homgr}_A(Z, C')) \xrightarrow{\mathrm{H}(\mathrm{Homgr}(i,1))} H^n(\mathrm{Homgr}_A(B, C'))
\xrightarrow{\mathrm{H}(\mathrm{Homgr}(\delta,1))} H^{n+1}(\mathrm{Homgr}_A(C, C')) \xrightarrow{\mathrm{H}(\mathrm{Homgr}(j,1))} H^{n+1}(\mathrm{Homgr}_A(Z, C')) \to \ldots .

Moreover, since $Z$ is projective, we obtain from (II_p) exact sequences
0 \to \mathrm{Hom}_A(H_p, H'^q) \to \mathrm{Hom}_A(Z_p, H'^q) \to \mathrm{Hom}_A(B_p, H'^q) \to \mathrm{Ext}_A^1(H_p, H'^q) \to 0 ,
hence, by passing to products, exact sequences
0 \to \mathrm{Homgr}_A^n(H, H') \to \mathrm{Homgr}_A^n(Z, H') \to \mathrm{Homgr}_A^n(B, H')
\to \prod_{p+q=n} \mathrm{Ext}_A^1(H_p, H'^q) \to 0 .
Finally, we have the canonical homomorphisms of No. 1:
$$
\begin{align*}
\lambda_B &= \lambda(B, C') : \mathrm{H}(\mathrm{Homgr}_A(B, C')) \to \mathrm{Homgr}_A(B, H') , \\
\lambda_Z &= \lambda(Z, C') : \mathrm{H}(\mathrm{Homgr}_A(Z, C')) \to \mathrm{Homgr}_A(Z, H') , \\
\lambda_C &= \lambda(C, C') : \mathrm{H}(\mathrm{Homgr}_A(C, C')) \to \mathrm{Homgr}_A(H, H') ,
\end{align*}
$$
whence the diagram with exact rows of page X.97.

This diagram is commutative by construction of the homomorphisms $\lambda$. Moreover, since the complexes B and Z are split and projective, $\lambda_B$ and $\lambda_Z$ are bijective ($\lambda$, p. 84, cor. 1). One deduces from this, on the one hand that $\lambda_C^n$ is surjective, with kernel equal to $\mathrm{Im}\ H^n(\mathrm{Homgr}(\delta, 1))$, and on the other hand that $\varphi^{n-1} \circ \lambda_B^{n-1}$ is surjective, with kernel equal to $\mathrm{Ker}\ H^n(\mathrm{Homgr}(\delta, 1))$. The theorem follows immediately from this.

#### Corollary 1 {#alg-x-s5-lem-2-cor-1 .statement}

Assume B(C) and Z(C) projective and B^n(C') injective for each n. Then the exact sequences (11) are split.
This follows from the theorem and the following lemma:

#### Lemma 3 {#alg-x-s5-lem-3 .statement}

If B(C) is projective and B_n(C') injective for each n, the canonical homomorphism $\lambda(C, C') : \mathrm{H}(\mathrm{Homgr}_A(C, C')) \to \mathrm{Homgr}_A(\mathrm{H}(C), \mathrm{H}(C'))$ has a linear section k.

Indeed, by X, p. 35, remarks a) and b), there exist homologisms
$$
\varphi : C \to \mathrm{H}(C) \quad \text{and} \quad \varphi' : \mathrm{H}(C') \to C'
$$
such that $\mathrm{H}(\varphi) = 1_{\mathrm{H}(C)}$ and $\mathrm{H}(\varphi') = 1_{\mathrm{H}(C')}$.
In the commutative diagram
$$
\begin{array}{ccc}
\mathrm{H}(\mathrm{Homgr}_A(\mathrm{H}(C), \mathrm{H}(C'))) & \xrightarrow{\mathrm{H}(\mathrm{Homgr}(\varphi, \varphi'))} & \mathrm{H}(\mathrm{Homgr}_A(C, C')) \\
\lambda(\mathrm{H}(C), \mathrm{H}(C')) \downarrow & & \downarrow \lambda(C, C') \\
\mathrm{Homgr}_A(\mathrm{H}(C), \mathrm{H}(C')) & \xrightarrow{\mathrm{Homgr}(\mathrm{H}(\varphi), \mathrm{H}(\varphi'))} & \mathrm{Homgr}_A(\mathrm{H}(C), \mathrm{H}(C')) ,
\end{array}
$$
$\lambda(\mathrm{H}(C), \mathrm{H}(C'))$ is bijective and $\mathrm{Homgr}(\mathrm{H}(\varphi), \mathrm{H}(\varphi'))$ is the identity, whence the assertion.

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

#### Corollary 2 {#alg-x-s5-lem-3-cor-2 .statement}

If $B(C)$ and $Z(C)$ are projective, one has, for every $A$-module $N$ and every integer $n$, a split exact sequence:

(13) $0 \longrightarrow \mathrm{Ext}_A^1(H_{n-1}(C), N) \xrightarrow{\beta^n} H^n(\mathrm{Homgr}_A(C, N)) \xrightarrow{\lambda^n} \mathrm{Hom}_A(H_n(C), N) \longrightarrow 0$.

#### Corollary 3 (« universal coefficient formula ») {#alg-x-s5-lem-3-cor-3 .statement}

Assume $A$ principal and $C$ free. One has for every $A$-module $N$ and every integer $n$ a split exact sequence (13).
Indeed $B(C)$ and $Z(C)$ are free as submodules of the free module $C$ (VII. § 3, cor. 2 to th. 1).

#### Corollary 4 {#alg-x-s5-lem-3-cor-4 .statement}

If $C$ is bounded on the right and if $C$ and $H(C)$ are projective, then

$$
\lambda(C, C') : H(\mathrm{Homgr}_A(C, C')) \to \mathrm{Homgr}_A(H(C), H(C'))
$$

is bijective.
By the theorem, it suffices to prove that $B(C)$ and $Z(C)$ are projective. Now one has exact sequences

$$
\begin{align*}
0 &\to B_n(C) \to Z_n(C) \to H_n(C) \to 0 \\
0 &\to Z_n(C) \to C_n \to B_{n-1}(C) \to 0,
\end{align*}
$$

therefore $(B_{n-1}(C) \text{ is projective}) \Rightarrow (Z_n(C) \text{ is projective}) \Rightarrow (B_n(C) \text{ is projective}).$ One concludes by remarking that $B_n(C) = 0$ for $n$ sufficiently small.

### 7. Generalization to complexes of multimodules ; the canonical isomorphisms

Let $B, B'$ be two rings, $C$ a complex of $(A, B)$-bimodules, $C'$ a complex of $(A, B')$-bimodules ; then $(\mathrm{Homgr}_A(C, C'), D)$ is a complex of $(B, B')$-bimodules and the canonical homomorphism $\lambda : H(\mathrm{Homgr}_A(C, C')) \to \mathrm{Homgr}_A(H(C), H(C'))$ is a homomorphism of $(B, B')$-bimodules.

If $M$ is an $(A, B)$-bimodule and $N$ an $(A, B')$-bimodule, then $\mathrm{Homgr}_A(L(M), I(N))$ is a complex of $(B, B')$-bimodules, so that $\mathrm{Ext}_A(M, N)$ is endowed with a natural structure of graded $(B, B')$-bimodule ; on the term of degree 0, this structure coincides with that of $\mathrm{Hom}_A(M, N)$ (II, p. 35).

If $\lambda \in B, \lambda' \in B'$ and if we denote by $\lambda_M, \lambda'_N, \lambda_E, \lambda'_E$ the homotheties $x \mapsto x\lambda, y \mapsto y\lambda', z \mapsto \lambda z, z \mapsto z\lambda'$ of $M, N, \mathrm{Ext}_A(M, N), \mathrm{Ext}_A(M, N)$ respectively, then

$$
\lambda_E = \mathrm{Ext}_A(\lambda_M, 1), \quad \lambda'_E = \mathrm{Ext}(1, \lambda'_N),
$$

which gives another description of the bimodule structure of $\mathrm{Ext}_A(M, N)$.

We leave to the reader the task of generalizing Nos. 4 and 6 to the case of complexes of multimodules.

Let $C, C', C''$ be complexes of $A$-modules. The composition of the mappings defines a graded homomorphism of degree zero :

(14)
$$
\mathrm{Homgr}_A(C', C'') \otimes_k \mathrm{Homgr}_A(C, C') \to \mathrm{Homgr}_A(C, C'').
$$

Let B, B', E be rings, C, C', C'' complexes of (B', A)-bimodules, (A, E)-bimodules, (B, E)-bimodules respectively. By restriction of the canonical isomorphism of II, p. 73, one obtains a bijective homomorphism of (B, B')-bimodules :

(15) $\operatorname{Homgr}_E(C \otimes_A C', C'') \to \operatorname{Homgr}_A(C, \operatorname{Homgr}_E(C', C''))$.

Finally, let B be a ring, C a complex of right B-modules, C' a complex of right A-modules, C'' a complex of (B, A)-bimodules. One deduces from the canonical homomorphisms (II. p. 75)

$$
C_p \otimes_B \operatorname{Hom}_A(C'_q, C''_r) \to \operatorname{Hom}_A(C'_q, C_p \otimes_B C''_r)
$$

a graded homomorphism of degree zero :

(16) $C \otimes_B \operatorname{Homgr}_A(C', C'') \to \operatorname{Homgr}_A(C', C \otimes_B C'')$.

This homomorphism is bijective when C is a finitely generated projective module (II, p. 75, prop. 2).

#### Proposition 12 {#alg-x-s5-prop-12 .statement}

The homomorphisms (14), (15), (16) are morphisms of complexes.

Let us prove it for example for the homomorphism (14). Denote

$$
\kappa : \operatorname{Homgr}_A(C', C'') \otimes_k \operatorname{Homgr}_A(C, C') \to \operatorname{Homgr}_A(C, C')
$$

this homomorphism. Let $f \in \operatorname{Homgr}_A(C', C'')_p$ and $g \in \operatorname{Homgr}_A(C, C')_q$; then by definition one has $\kappa(f \otimes g) = f \circ g$. Moreover :

$$
\mathrm{D}(f \otimes g) = \mathrm{D}f \otimes g + (-1)^p f \otimes \mathrm{D}g = (d'' \circ f) \otimes g - (-1)^p (f \circ d') \otimes g +
+ (-1)^p f \otimes (d' \circ g) - (-1)^{p+q} f \otimes (g \circ d),
$$

whence

$$
\kappa(\mathrm{D}(f \otimes g)) = d'' \circ f \circ g - (-1)^p f \circ d' \circ g +
+ (-1)^p f \circ d' \circ g - (-1)^{p+q} f \circ g \circ d \\
= d'' \circ f \circ g - (-1)^{p+q} f \circ g \circ d = \mathrm{D}(f \circ g) = \mathrm{D}(\kappa(f \otimes g)).
$$

One proves analogously that the homomorphisms (15) and (16) are morphisms of complexes.

One deduces from the morphism (14) homomorphisms of $k$-modules (X, p. 62)

(17) $\mathrm{H}^p(\operatorname{Homgr}_A(C', C'')) \otimes_k \mathrm{H}^q(\operatorname{Homgr}_A(C, C')) \to \mathrm{H}^{p+q}(\operatorname{Homgr}_A(C, C''))$.

Taking $C = A$, one sees that the homomorphism :

(18) $\operatorname{Homgr}_A(C', C'') \otimes_k C' \to C''$ which maps $f \otimes x$ to $f(x)$ is a morphism of complexes of left $A$-modules ; there is associated to it a canonical homomorphism ($X$, p. 80) of graded $A$-modules $\gamma : H(\mathrm{Homgr}_A(C', C'')) \otimes_k H(C') \to H(C'')$, which corresponds to the canonical homomorphism of $k$-modules

$$
\lambda : H(\mathrm{Homgr}_A(C', C'')) \to \mathrm{Homgr}_A(H(C'), H(C''))
$$

## EXERCISES {#alg-x-s5-exercises}

See the [exercises for § 5](exercises/s5/).
