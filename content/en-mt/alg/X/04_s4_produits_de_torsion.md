---
book: alg
book_title: Algebra
chapter: X
chapter_title: ALGÈBRE HOMOLOGIQUE
section: 4
section_title: Produits de torsion
lang: en
source: alg-x-fr
book_pages: A X.61-A X.81, A X.184-A X.186
pdf_pages: 0067-0087, 0190-0192
extraction: ocr
subsections:
    - "no": 1
      title: Produit tensoriel de deux complexes
      page: 61
      pdf_page: 67
    - "no": 2
      title: Produits tensoriels et homotopie
      page: 64
      pdf_page: 70
    - "no": 3
      title: Produit tensoriel par un complexe plat borné à droite
      page: 66
      pdf_page: 72
    - "no": 4
      title: Définition et premières propriétés du produit de torsion
      page: 67
      pdf_page: 73
    - "no": 5
      title: Les homomorphismes de liaison et les suites exactes
      page: 71
      pdf_page: 77
    - "no": 6
      title: Modules plats et produits de torsion
      page: 74
      pdf_page: 80
    - "no": 7
      title: ' **Formule de Künneth**'
      page: 76
      pdf_page: 82
    - "no": 8
      title: Complexes bornés et plats sur un anneau noethérien
      page: 79
      pdf_page: 85
    - "no": 9
      title: Généralisation aux complexes de multimodules
      page: 80
      pdf_page: 86
statements: 39
exercises: 9
content_sha256: 1e9d4f753de7f9be6f651b6d95c57033b3cee123d3b97133eeb5db3f8cebd78e
translated_from: content/fr/alg/X/04_s4_produits_de_torsion.md
source_lang: fr
translation_method: machine
source_content_sha256: 0dd07ce8e9ce8109b1e39864b92a50b62e2990891ab5bf56dbf260ccfcff8d83
translation_model: nemotron-3-ultra-free, hy3-free, laguna-s-2.1-free
translation_run: translate-en-mt-81336cab
glossary_version: 34
glossary_terms_sha256: e9a63306b95092393b2384b16f6f12312320051bcf809925133b257a906f66e9
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 4. Torsion product

*In sections 4 to 8, we denote by $k$ a commutative ring, and by $A$ an associative unital $k$-algebra. The role of $k$ is auxiliary; we mainly have in view the following three special cases:*

a) we consider an arbitrary ring $A$, we set $k=\mathbf{Z}$ and we endow $A$ with its natural structure of $\mathbf{Z}$-algebra,

b) we consider an arbitrary ring $A$, we take for $k$ the center of $A$,

c) we consider a commutative ring $A$ and we take $k=A$.

### 1. Tensor product of two complexes

Let $(C,d)$ be a complex of right $A$-modules and $(C',d')$ a complex of left $A$-modules.

Let us endow the $k$-module $C\otimes_A C'$ with the grading such that

$$
(C\otimes_A C')_n=\sum_{p+q=n}(C_p\otimes C'_q)
$$

and let $D$ be the unique $k$-linear endomorphism of degree $(-1)$ of $C\otimes_A C'$ such that

$$
\tag{1}
D(x\otimes x')=dx\otimes x'+(-1)^p x\otimes d'x',
\qquad x\in C_p,\ y\in C'_q,\ p,\ q\in\mathbf{Z}.
$$

We have $D\circ D=0$ since, with the notations of (1)

$$
D^2(x\otimes x')=ddx\otimes x'+(-1)^{p-1}dx\otimes d'x'+(-1)^pdx\otimes d'x'-x\otimes d'd'x'.
$$

The complex of $k$-modules $(C\otimes_A C',D)$ is called the *tensor product complex* of the complexes $(C,d)$ and $(C',d')$.

#### Remark 1 {#alg-x-s4-n1-rem-1 .statement}

When $C'$ is reduced to $C'_0=M$, then $(C\otimes_A C')_n=C_n\otimes_A M$ and $D=d\otimes 1_M$; for example $C\otimes_A A_s$ is naturally identified with $C$. Similarly, when $C$ is reduced to $C_0=P$, then $(C\otimes_A C')_n=P\otimes_A C'_n$ and $D=1_P\otimes d$.

#### Remark 2 {#alg-x-s4-n1-rem-2 .statement}

For every integer $r$, we have $(C\otimes_A C')(r)=C(r)\otimes_A C'$, but $(C\otimes_A C')(r)$ and $C\otimes_A C'(r)$ do not in general have the same differential.

Let $p, q$ be two integers, $x \in Z_p(C), x' \in Z_q(C')$; then the element $x \otimes x'$ of $C_p \otimes C'_q$ belongs to $Z_{p+q}(C \otimes C')$ by (1); moreover, if $y \in C_{p+1}, y' \in C'_{q+1}$, we have
$$
(x + dy) \otimes (x' + d'y') = x \otimes x' + D(y \otimes x' + (-1)^p (x + dy) \otimes y');
$$
by passing to the quotients, we deduce a $k$-linear mapping, called canonical
$$
\gamma_{p,q}(C, C') : H_p(C) \otimes_A H_q(C') \to H_{p+q}(C \otimes_A C');
$$
if we endow $H(C) \otimes_A H(C')$ with the grading such that
$$
(H(C) \otimes H(C'))_n = \sum_{p+q=n} H_p(C) \otimes_A H_q(C'),
$$
the $\gamma_{p,q}$ define a graded $k$-linear mapping of degree 0
$$
\gamma(C, C') : H(C) \otimes_A H(C') \to H(C \otimes_A C').
$$
Prop. 6 of II, p. 59, can be reformulated as follows:

#### Proposition 1 {#alg-x-s4-prop-1 .statement}

*If the complexes $C$ and $C'$ are zero on the right, $C \otimes_A C'$ is zero on the right and the canonical $k$-linear mapping*
$$
\gamma_{0,0}(C, C') : H_0(C) \otimes_A H_0(C') \to H_0(C \otimes_A C')
$$
*is bijective*.

Let $u : (C, d) \to (C_1, d_1)$ be a morphism of complexes of right $A$-modules and $u' : (C', d') \to (C'_1, d'_1)$ a morphism of complexes of left $A$-modules; then $u \otimes u' : C \otimes_A C' \to C_1 \otimes_A C'_1$ is a morphism of complexes of $k$-modules; indeed, it is graded of degree 0, and if we denote by $D$ and $D_1$ the differentials of $C \otimes C'$ and $C_1 \otimes C'_1$, we have for $p, q \in \mathbf{Z}, x \in C_p, x' \in C'_q$,
$$
(u \otimes u') (D(x \otimes x')) = u(dx) \otimes u'(x') + (-1)^p u(x) \otimes u'(d'x') =
= d_1 u(x) \otimes u'(x') + (-1)^p u(x) \otimes d'_1 u'(x') = D_1(u(x) \otimes u'(x')) .
$$
Moreover the following diagram is commutative :
$$
\begin{array}{ccc}
H(C) \otimes_A H(C') & \xrightarrow{\gamma(C, C')} & H(C \otimes_A C') \\
H(u) \otimes H(u') \downarrow & & \downarrow H(u \otimes u') \\
H(C_1) \otimes_A H(C'_1) & \xrightarrow{\gamma(C_1, C'_1)} & H(C_1 \otimes_A C'_1)
\end{array}
$$

Let $A^\circ$ be the $k$-algebra opposite to $A$, $C^\circ$ (resp. ${C'}^\circ$) the complex $C$ (resp. $C'$) considered as a complex of left $A^\circ$-modules (resp. right). Let us denote by
$$
\sigma(C, C') : C \otimes_A C' \to {C'}^\circ \otimes_{A^\circ} C^\circ
$$
the unique graded $k$-linear mapping of degree 0 such that, for $x \in C_p, x' \in C'_q, p, q \in \mathbf{Z}$, we have
$$
\sigma(C, C') (x \otimes x') = (-1)^{pq} x' \otimes x .
$$

#### Proposition 2 {#alg-x-s4-prop-2 .statement}

The mapping $\sigma(C, C') : C \otimes_A C' \to {C'}^\circ \otimes_A C^\circ$ is an isomorphism of complexes of $k$-modules, whose reciprocal isomorphism is $\sigma({C'}^\circ, C^\circ)$.

Since the mappings $\sigma(C, C')$ and $\sigma({C'}^\circ, C^\circ)$ are reciprocal to each other, it suffices to prove that $\sigma(C, C')$ is a morphism of complexes. Now, for
$$
x \in C_p = C_p^\circ, \quad x' \in C'_q = C_{q'}^\circ, \quad p, q \in \mathbf{Z},
$$
we have, denoting by $D'$ the differential of $C' \otimes_{A^\circ} C$,
$$
\begin{align*}
\sigma(C, C') \circ D(x \otimes x') &= \sigma(C, C') (dx \otimes x' + (-1)^p x \otimes d'x') = \\
&= (-1)^{(p+1)q} x' \otimes dx + (-1)^{p+p(q+1)} d'x' \otimes x = (-1)^{pq} d'x' \otimes x + (-1)^{pq+q} x' \otimes dx \\
&= (-1)^{pq} D'(x' \otimes x) = D^\circ \circ \sigma(C, C') (x \otimes x');
\end{align*}
$$
which gives $\sigma(C, C') \circ D = D^\circ \circ \sigma(C, C')$, whence the assertion sought.

The isomorphism $\sigma(C, C') : C \otimes_A C' \to {C'}^\circ \otimes_A C^\circ$ is called the *commutation isomorphism* of the tensor product of the complexes $C$ and $C'$.

If $u : C \to C_1$ and $v : C' \to C'_1$ are two morphisms of complexes as above, we have a commutative diagram :

$$
\begin{array}{ccc}
C \otimes_A C' & \xrightarrow{\sigma(C, C')} & {C'}^\circ \otimes_A C^\circ \\
u \otimes u' \downarrow & & \downarrow u' \otimes u \\
C_1 \otimes_A C'_1 & \xrightarrow{\sigma(C_1, C'_1)} & C'_1{}^\circ \otimes_A C_1^\circ.
\end{array}
$$

Suppose for the end of this number that the ring $A$ is *commutative* (*cf.* No. 9 for the general case).

Let $C, C', C''$ be three complexes of $A$-modules; the canonical homomorphism of $A$-modules (III, p. 64)
$$
\varphi : (C \otimes_A C') \otimes_A C'' \to C \otimes_A (C' \otimes_A C'')
$$
is an *isomorphism of complexes*, as is immediately verified using the definitions.

More generally, let $(C^{(i)}, d^{(i)})_{i \in I}$ be a *family of complexes* of $A$-modules, where the set $I$ is *finite and totally ordered*; we shall identify $I$ with the interval $[1, r]$ of $\mathbf{N}$ to simplify the notation. Let us endow the $A$-module $C = \bigotimes_{i=1}^r C^{(i)}$ with the grading such that
$$
C_n = \sum_{p_1 + p_2 + \cdots + p_r = n} (C^{(1)})_{p_1} \otimes (C^{(2)})_{p_2} \otimes \cdots \otimes (C^{(r)})_{p_r},
$$
and define a graded $A$-endomorphism of degree $(-1)$ of $C$ by
$$
D(x_1 \otimes \ldots \otimes x_r) = \sum_{j=1}^r (-1)^{p_1 + \cdots + p_{j-1}} x_1 \otimes \ldots \otimes x_{j-1} \otimes d_j x_j \otimes x_{j+1} \otimes \ldots \otimes x_r
$$
where $x_i \in (C^{(i)})_{p_i}$ for $i = 1, \ldots, n$. Then $(C, D)$ is a complex of $A$-modules called the tensor product complex of the family $(C_i, d_i)$. For every strictly increasing sequence $r_0, ..., r_k$ of $[0, r]$ such that $r_0 = 0,\ r_k = r$, the canonical associativity isomorphism

$$
\bigotimes_{j=0}^{k-1} \left( \bigotimes_{i=r_j+1}^{r_{j+1}} C^{(i)} \right) \to \bigotimes_{i=1}^r C^{(i)}
$$

is an isomorphism of complexes.

We define as above a graded homomorphism of degree 0

$$
\gamma((C^{(i)})) : \bigotimes_{i \in I} H(C^{(i)}) \to H \left( \bigotimes_{i \in I} C^{(i)} \right)
$$

#### Remark 3 {#alg-x-s4-n1-rem-3 .statement}

One can define the tensor product of a finite family of complexes without endowing the index set with a total order (X, p. 185, Exercise 3).

#### Remark 4 {#alg-x-s4-n1-rem-4 .statement}

Suppose that each $C^{(i)}$ is endowed with a graded algebra structure compatible with its grading and such that the $d^{(i)}$ are antiderivations (III, p. 117). Let us then endow $\bigotimes_{i \in I} C^{(i)}$ with the left graded tensor product algebra structure of the given structures (III, p. 49). Then $D$ is an antiderivation. Indeed, using the associativity of the tensor product, we may assume that $I = \{1, 2\}$; let then $p_1,\ q_1,\ p_2,\ q_2 \in \mathbf{Z},\ x_1 \in (C^{(1)})_{p_1},\ y_1 \in (C^{(1)})_{q_1},\ x_2 \in (C^{(2)})_{p_2},\ y_2 \in (C^{(2)})_{q_2}$; we have

$$
(D(x_1 \otimes x_2))(y_1 \otimes y_2) + (-1)^{p_1+p_2} (x_1 \otimes x_2)(D(y_1 \otimes y_2)) =
$$
$$
= (dx_1 \otimes x_2 + (-1)^{p_1} x_1 \otimes dx_2)(y_1 \otimes y_2) +
$$
$$
+ (-1)^{p_1+p_2} (x_1 \otimes x_2)(dy_1 \otimes y_2 + (-1)^{q_1} y_1 \otimes dy_2) =
$$
$$
= (-1)^{p_2 q_1} (dx_1) y_1 \otimes x_2 y_2 + (-1)^{p_1+(p_2-1)q_1} x_1 y_1 \otimes (dx_2) y_2 +
$$
$$
+ (-1)^{p_1+p_2+p_2(q_1-1)} x_1 dy_1 \otimes x_2 y_2 + (-1)^{p_1+p_2+q_1+p_2 q_1} x_1 y_1 \otimes x_2 dy_2
$$
$$
= (-1)^{p_2 q_1} [(dx_1) y_1 + (-1)^{p_1} x_1 dy_1] \otimes x_2 y_2 +
$$
$$
+ (-1)^{p_1+q_1+p_2 q_1} x_1 y_1 \otimes ((dx_2) y_2 + (-1)^{p_2} x_2 dy_2)
$$
$$
= (-1)^{p_2 q_1} [d(x_1 y_1) \otimes x_2 y_2 + (-1)^{p_1+q_1} x_1 y_1 \otimes d(x_2 y_2)]
$$
$$
= (-1)^{p_2 q_1} D(x_1 y_1 \otimes x_2 y_2) = D((x_1 \otimes x_2)(y_1 \otimes y_2)).
$$

### 2. Tensor products and homotopy

#### Proposition 3 {#alg-x-s4-prop-3 .statement}

Let $C,\ C_1$ be two complexes of right $A$-modules, $C',\ C'_1$ two complexes of left $A$-modules, and $u : C \to C_1,\ v : C \to C_1,\ u' : C' \to C'_1,\ v' : C' \to C'_1$ be morphisms of complexes.

a) If $u$ and $u'$ are homotopic to $v$ and $v'$ respectively, then the two morphisms $u \otimes u'$ and $v \otimes v'$ from $C \otimes_A C'$ to $C_1 \otimes_A C'_1$ are homotopic.

b) If $u$ and $u'$ are homotopy equivalences, $u \otimes u'$ is a homotopy equivalence.

c) If $C$ or $C'$ is homotopic to zero, $C \otimes_A C'$ is homotopic to zero.

Let us denote by the same letter $d$ the differentials of the complexes $C,\ C_1,\ C',\ C'_1$ and by $D$ the differentials of the complexes $C \otimes_A C'$ and $C_1 \otimes_A C'_1$.

If $u$ (resp. $u'$) is homotopic to $v$ (resp. $v'$), there exists a graded homomorphism of degree 1 $s:C\to C_1$ (resp. $s':C'\to C'_1$) such that

$$
(2)\qquad u-v=ds+sd\qquad\text{(resp. }u'-v'=ds'+s'd\text{)}.
$$

Let $S:C\otimes_A C'\to C_1\otimes_A C'_1$ be the unique graded homomorphism of degree 1 such that, for $x\in C_p,\ y\in C'_q,\ p,q\in\mathbf Z$, we have

$$
(3)\qquad S(x\otimes y)=s(x)\otimes u'(y)+(-1)^p v(x)\otimes s'(y).
$$

Then, with the previous notations:

$$
\begin{aligned}
(DS+SD)(x\otimes y)&=D(sx\otimes u'y)+(-1)^pD(vx\otimes s'y)+S(dx\otimes y)\\
&\quad+(-1)^pS(x\otimes dy)=\\
&=dsx\otimes u'y+(-1)^{p+1}sx\otimes du'y+(-1)^pdvx\otimes s'y+vx\otimes ds'y\\
&\quad+sdx\otimes u'y+(-1)^{p-1}vdx\otimes s'y+(-1)^psx\otimes u'dy+vx\otimes s'dy\\
&=(ds+sd)(x)\otimes u'y+vx\otimes(ds'+s'd)(y)\\
&=(ux-vx)\otimes u'y+vx\otimes(u'y-v'y)=ux\otimes u'y-vx\otimes v'y.
\end{aligned}
$$

This gives $DS+SD=u\otimes u'-v\otimes v'$, whence a).

Let us prove b). If $u$ and $u'$ are homotopy equivalences, there exist homomorphisms of complexes $\alpha:C_1\to C$ and $\alpha':C'_1\to C'$ such that $u\circ\alpha,\ \alpha\circ u',\ \alpha'\circ u'$ are homotopic respectively to $\mathrm{Id}_{C_1},\ \mathrm{Id}_C,\ \mathrm{Id}_{C'_1},\ \mathrm{Id}_{C'}$. Then $(u\otimes u')\circ(\alpha\otimes\alpha')$, which is equal to $(u\circ\alpha)\otimes(u'\circ\alpha')$, is homotopic by a) to $\mathrm{Id}_{C_1}\otimes\mathrm{Id}_{C'_1}=\mathrm{Id}_{C_1\otimes C'_1}$, while $(\alpha\otimes\alpha')\circ(u\otimes u')$ is homotopic to $\mathrm{Id}_{C\otimes C'}$, whence b). Finally, c) follows from b) applied to the case where $C_1$ or $C'_1$ is zero.

#### Corollary 1 {#alg-x-s4-prop-3-cor-1 .statement}

Let $C'$ be a split complex of left $A$-modules such that $H(C')$ is flat. For every complex $C$ of right $A$-modules, the canonical mapping

$$
\gamma(C,C'):H(C)\otimes_AH(C')\longrightarrow H(C\otimes_A C')
$$

is bijective.

By X, p. 35, def. 6, there exists a homotopy equivalence $u':C'\to H(C')$. By prop. 3, $1_C\otimes u':C\otimes_A C'\to C\otimes_AH(C')$ is a homotopy equivalence; since

$$
H(1_C\otimes u')\circ\gamma(C,C')=\gamma(C,H(C'))\circ(1_C\otimes H(u')),
$$

and $H(1_C\otimes u')$ and $H(u')$ are bijective, it suffices to prove that $\gamma(C,H(C'))$ is bijective, and we are reduced to the case where $C'$ is flat and has zero differential. In this case the canonical exact sequences

$$
\mathrm{(I)}\qquad 0\longrightarrow Z(C)\xrightarrow{i}C\xrightarrow{\partial}B(C)\longrightarrow0
$$

$$
\mathrm{(II)}\qquad 0\longrightarrow B(C)\xrightarrow{j}Z(C)\xrightarrow{\pi}H(C)\longrightarrow0
$$

give exact sequences:

$$
0 \longrightarrow Z(C) \otimes_A C' \xrightarrow{i\otimes 1} C \otimes_A C' \xrightarrow{\delta\otimes 1} B(C) \otimes_A C' \longrightarrow 0
$$

$$
0 \longrightarrow B(C) \otimes_A C' \xrightarrow{j\otimes 1} Z(C) \otimes_A C' \xrightarrow{\pi\otimes 1} H(C) \otimes_A C' \longrightarrow 0.
$$

Since $d=i\circ j\circ\delta$, we have $D=d\otimes 1_{C'}=(i\otimes 1)\circ(j\otimes 1)\circ(\delta\otimes 1)$, which shows that the canonical mappings $Z(C)\otimes_A C'\to Z(C\otimes_A C')$ and $B(C)\otimes_A C'\to B(C\otimes_A C')$ are bijective, hence also $\gamma(C,C')$ by passing to quotients.

#### Corollary 2 {#alg-x-s4-prop-3-cor-2 .statement}

Let $\mathbf N$ be a flat left $A$-module. For every complex $C$ of right $A$-modules, the canonical homomorphisms

$$
\gamma_n(C,\mathbf N): H_n(C)\otimes_A \mathbf N \longrightarrow H_n(C\otimes_A \mathbf N)
$$

are bijective.

#### Corollary 3 {#alg-x-s4-prop-3-cor-3 .statement}

Let $C'$ be a complex of left $A$-modules such that $B(C')$ and $H(C')$ are projective. For every complex $C$ of right $A$-modules, the mapping $\gamma(C,C')$ is bijective.

Indeed, $C'$ is split (X, p. 35, example 4) and $H(C')$ is projective; therefore we can apply corollary 1.

#### Remark 1 {#alg-x-s4-n2-rem-1 .statement}

Using the commutation isomorphisms, one deduces from corollaries 1, 2 and 3 the analogous statements obtained by exchanging the roles of the two arguments of the tensor products.

#### Remark 2 {#alg-x-s4-n2-rem-2 .statement}

We shall see below (X, p. 79, Cor. 4) that the conclusion of Cor. 1 is also true when one assumes $C'$ and $H(C')$ flat and $C'$ bounded on the right.

### 3. Tensor product by a flat complex bounded on the right

#### Lemma 1 {#alg-x-s4-lem-1 .statement}

Let C be a complex of right A-modules and E a complex of left A-modules. We assume that $H(C)=0$ and that E is flat and bounded on the right. Then $H(C\otimes_A E)=0$.

For $k\in\mathbf Z$, let $T^{(k)}$ be the subcomplex of $C\otimes_A E$ such that

$$
T_n^{(k)}=\sum_{\substack{p+q=n\\q\leq k}} C_p\otimes_A E_q\ ;
$$

then $T^{(k-1)}\subset T^{(k)}$ and we have an exact sequence of complexes

$$
0\longrightarrow T^{(k-1)}\xrightarrow{i_k}T^{(k)}\xrightarrow{\pi}C\otimes_A E_k(-k)\longrightarrow 0
$$

where $i_k$ is the canonical injection and where $\pi$ projects the preceding direct sum onto its factor $C_{n-k}\otimes_A E_k=(C\otimes_A E_k(-k))_n$. By Cor. 2 above, we have $H(C\otimes_A E_k(-k))=0$, hence $i_k$ is a homomorphism. We have $T^{(k)}=0$ for $k$ sufficiently small, since $E$ is bounded on the right, hence $H(T^{(k)})=0$ for all $k$ by induction on $k$. Finally, the canonical morphism $\underset{\longrightarrow}{\lim}\,T^{(k)}\to C\otimes_A E$ is obviously an isomorphism, hence $H(C\otimes_A E)=0$ (X, p. 28, Prop. 1).

#### Lemma 2 {#alg-x-s4-lem-2 .statement}

If $u:C\to C'$ is a morphism of complexes of right A-modules and $E$ a complex of left A-modules, then the complexes $\operatorname{Con}(u)\otimes_A E$ and $\operatorname{Con}(u\otimes 1_E)$ are isomorphic.

By definition, $\operatorname{Con}(u)\otimes_A E$ is the graded module $(C'(-1)\oplus C)\otimes_A E$ endowed with the differential $D$ such that, for $x\in C_p$, $y'\in C'(-1)_p=C'_{p-1}$, $z\in E_q$, we have

(4)
$$
D(y',x)\otimes z=(-dy',dx-u(y'))\otimes z+(-1)^p(y',x)\otimes dz,
$$

while $\operatorname{Con}(u\otimes 1_E)$ is the graded module $(C'\otimes_A E)(-1)\oplus(C\otimes_A E)$ endowed with the differential $D_1$ such that, for $x\in C_p$, $y'\in C'_{p-1}$, $z\in E_q$, we have

$$
D_1(y'\otimes z,x\otimes z)=(-dy'\otimes z-(-1)^{p-1}y'\otimes dz,dx\otimes z+(-1)^p x\otimes dz-u(y')\otimes z)
$$

$$
=(-dy'\otimes z,(dx-u(y'))\otimes z)+(-1)^p(y'\otimes dz,x\otimes dz),
$$

whence the assertion.

#### Proposition 4 {#alg-x-s4-prop-4 .statement}

Let $u:C\to C'$ be a homology isomorphism of complexes of right A-modules and $E$ a complex of left A-modules, flat and bounded on the right. Then

$$
u\otimes 1_E:C\otimes_A E\to C'\otimes_A E
$$

is a homology isomorphism of complexes of $k$-modules.

Indeed, by X, p. 38, Cor., $u$ (resp. $u\otimes 1_E$) is a homology isomorphism if and only if $H(\operatorname{Con}(u))=0$ (resp. $H(\operatorname{Con}(u\otimes 1_E))=0$). The conclusion then follows from Lemmas 1 and 2.

#### Remark {#alg-x-s4-n3-rem-1 .statement}

Using the commutation isomorphisms, one deduces from the preceding statements the analogous statements obtained by exchanging the roles of the two arguments of the tensor products.

### 4. Definition and first properties of the torsion product

For every A-module $E$, we denote by $p_E:L(E)\to E$ the canonical free resolution of $E$ (X, p. 50).

#### Definition 1 {#alg-x-s4-def-1 .statement}

Let $M$ be a right A-module and $N$ a left A-module. We call the torsion product of $M$ and $N$ the graded $k$-module

(4)
$$
\operatorname{Tor}^A(M,N)=H(L(M)\otimes_A L(N)).
$$

The homogeneous components of $\operatorname{Tor}^A(M,N)$ are denoted

(5)
$$
\operatorname{Tor}^A_n(M,N)=H_n(L(M)\otimes_A L(N)).
$$

Since $L(M)$ and $L(N)$ are zero on the right, we have

(6)
$$
\operatorname{Tor}_n^A(M, N) = 0 \quad \text{for } n < 0 .
$$

#### Remark 1 {#alg-x-s4-n4-rem-1 .statement}

We will see below (X, p. 107, Proposition 6) finiteness properties of the modules $\operatorname{Tor}^A(M, N)$. For example, if $A$ is commutative noetherian and if $M$ and $N$ are $A$-modules of finite type, every $A$-module $\operatorname{Tor}_n^A(M, N)$ is of finite type.

Let $f : M \to M'$ be a homomorphism of right $A$-modules and $g : N \to N'$ a homomorphism of left $A$-modules. We define $\operatorname{Tor}^A(f, g) = H(L(f) \otimes_A L(g))$; this is a homomorphism of graded $k$-modules

$$
\operatorname{Tor}^A(f, g) : \operatorname{Tor}^A(M, N) \to \operatorname{Tor}^A(M', N')
$$

whose homogeneous components are denoted

$$
\operatorname{Tor}_n^A(f, g) : \operatorname{Tor}_n^A(M, N) \to \operatorname{Tor}_n^A(M', N') .
$$

According to Proposition 1 of X, p. 62, the canonical homomorphism

$$
\gamma_{0,0} : H_0(L(M)) \otimes_A H_0(L(N)) \to H_0(L(M) \otimes_A L(N))
$$

is bijective; using the isomorphisms $M \to H_0(L(M))$ and $N \to H_0(L(N))$, we deduce from it an isomorphism, called *canonical*

(7)
$$
\gamma_{M,N} : M \otimes_A N \to \operatorname{Tor}_0^A(M, N) .
$$

We will always identify $\operatorname{Tor}_0^A(M, N)$ with $M \otimes_A N$ through this isomorphism. Hence the $k$-linear map $\operatorname{Tor}_0^A(f, g)$ is identified with $f \otimes g$.

#### Remark 2 {#alg-x-s4-n4-rem-2 .statement}

The complex morphism $p_M \otimes p_N : L(M) \otimes_A L(N) \to M \otimes_A N$ induces on the degree 0 homology the isomorphism

$$
\gamma_{M,N}^{-1} : \operatorname{Tor}_0^A(M, N) \to M \otimes_A N
$$

inverse to $\gamma_{M,N}$.

We have $L(1_M) = 1_{L(M)}$, $L(1_N) = 1_{L(N)}$, hence by passage to the homology:

(8)
$$
\operatorname{Tor}^A(1_M, 1_N) = 1_{\operatorname{Tor}^A(M, N)} .
$$

If $f' : M' \to M''$ (resp. $g' : N' \to N''$) is a homomorphism of right $A$-modules (resp. left $A$-modules), we have $L(g' \circ g) = L(g') \circ L(g)$ and $L(f' \circ f) = L(f') \circ L(f)$, hence

(9)
$$
\operatorname{Tor}^A(f' \circ f, g' \circ g) = \operatorname{Tor}^A(f', g') \circ \operatorname{Tor}^A(f, g) .
$$

Consider the morphisms of $k$-complexes

$$
L(M) \otimes_A N \xleftarrow{1 \otimes p_N} L(M) \otimes_A L(N) \xrightarrow{p_M \otimes 1} M \otimes_A L(N)
$$

and the $k$-homomorphisms they induce in homology:

$$
H(L(M) \otimes_A N) \xleftarrow{\psi_M(N)} \mathrm{Tor}^A(M, N) \xrightarrow{\overline{\psi}_N(M)} H(M \otimes_A L(N)) ;
$$

according to Proposition 4 of X, p. 67, $1 \otimes p_N$ and $p_M \otimes 1$ are homology morphisms. Therefore:

**Proposition 5. — The $k$-homomorphisms**

$$
\begin{aligned}
& \psi_M(N) : \mathrm{Tor}^A(M, N) \to H(L(M) \otimes_A N) \\
& \overline{\psi}_N(M) : \mathrm{Tor}^A(M, N) \to H(M \otimes_A L(N))
\end{aligned}
$$

are *bijective*.

**Corollary. — If $M$ or $N$ is flat, $\mathrm{Tor}_i^A(M, N) = 0$ for $i \geqslant 0$.**

Suppose that $N$ (resp. $M$) is flat. Then $p_M \otimes 1 : L(M) \otimes_A N \to M \otimes_A N$ (resp. $1 \otimes p_N : M \otimes_A L(N) \to M \otimes_A N$) is a homology morphism (X, p. 67, Proposition 4), hence $H_i(L(M) \otimes_A N)$ (resp. $H_i(M \otimes_A L(N))$) vanishes for $i > 0$.

*Remark 3. — If $g : N \to N'$ is a homomorphism of left A-modules, then*

$$
(1_{L(M)} \otimes g) \circ (1_{L(M)} \otimes 1_N) = (1_{L(M)} \otimes 1_N) \circ (1_{L(M)} \otimes L(g)) ,
$$

therefore the diagram

$$
\begin{array}{ccc}
\mathrm{Tor}^A(M, N) & \xrightarrow{\psi_{M(N)}} & H(L(M) \otimes_A N) \\
\mathrm{Tor}^A(1, g) \downarrow & & \downarrow H(1 \otimes g) \\
\mathrm{Tor}^A(M, N') & \xrightarrow{\psi_{M(N')}} & H(L(M) \otimes_A N')
\end{array}
$$

is commutative.

Analogously, if $f : M \to M'$ is a homomorphism of right A-modules, one has a commutative diagram :

$$
\begin{array}{ccc}
\mathrm{Tor}^A(M, N) & \xrightarrow{\overline{\psi}_{N(M)}} & H(M \otimes_A L(N)) \\
\mathrm{Tor}^A(f, 1) \downarrow & & \downarrow H(f \otimes 1) \\
\mathrm{Tor}^A(M', N) & \xrightarrow{\overline{\psi}_{N(M')}} & H(M' \otimes_A L(N)) .
\end{array}
$$

**Proposition 6. — The mapping** $(f, g) \mapsto \mathrm{Tor}^A(f, g) :$

$$
\mathrm{Hom}_A(M, M') \times \mathrm{Hom}_A(N, N') \to \mathrm{Hom}_k(\mathrm{Tor}^A(M, N), \mathrm{Tor}^A(M', N'))
$$

*is $k$*-bilinear.

Let $f \in \mathrm{Hom}_A(M, M')$, $g_1, g_2 \in \mathrm{Hom}_A(N, N')$, $\lambda_1, \lambda_2 \in k$. Then the morphisms

$$
\lambda_1(L(f) \otimes g_1) + \lambda_2(L(f) \otimes g_2) \quad \text{and} \quad L(f) \otimes (\lambda_1 g_1 + \lambda_2 g_2)
$$

from $L(M) \otimes_A N$ into $L(M) \otimes_A N'$ coincide; by prop. 5 and Remark 3, one therefore has

(10) $$
\mathrm{Tor}^A(f, \lambda_1 g_1 + \lambda_2 g_2) = \lambda_1 \mathrm{Tor}^A(f, g_1) + \lambda_2 \mathrm{Tor}^A(f, g_2).
$$

One reasons analogously for the mapping $f \mapsto \mathrm{Tor}^A(f, g)$.

#### Corollary {#alg-x-s4-n4-cor-1 .statement}

*Let $\lambda \in k$. If $\lambda$ annihilates $M$ or $N$, it annihilates $\mathrm{Tor}^A(M, N)$.*

Indeed, $\lambda . 1_{\mathrm{Tor}(M, N)} = \mathrm{Tor}(\lambda . 1_M, 1_N) = \mathrm{Tor}(1_M, \lambda . 1_N)$.

#### Proposition 7 {#alg-x-s4-prop-7 .statement}

*Let I and J be two sets, $(M_\alpha)_{\alpha \in I}$ a family of right A-modules, $(N_\beta)_{\beta \in J}$ a family of left A-modules. The homomorphism*

$$
\bigoplus_{\alpha \in I, \beta \in J} \mathrm{Tor}^A(M_\alpha, N_\beta) \to \mathrm{Tor}^A\left( \bigoplus_{\alpha \in I} M_\alpha, \bigoplus_{\beta \in J} N_\beta \right)
$$

*deduced from the canonical homomorphisms* $M_\alpha \to \bigoplus M_\alpha$ *and* $N_\beta \to \bigoplus N_\beta$ *is bijective*.

It suffices to prove that for every right module $M$ (resp. every left module $N$), the canonical homomorphism

$$
\bigoplus_{\beta \in J} \mathrm{Tor}^A(M, N_\beta) \to \mathrm{Tor}^A(M, \bigoplus_{\beta \in J} N_\beta)
$$

(resp. $\bigoplus_{\alpha \in I} \mathrm{Tor}^A(M_\alpha, N) \to \mathrm{Tor}^A(\bigoplus_{\alpha \in I} M_\alpha, N)$) is bijective. Now this follows from the preceding, from Proposition 1 of X, p. 28, and from the canonical isomorphisms :

$$
\bigoplus_{\beta} (L(M) \otimes_A N_\beta) \to L(M) \otimes_A (\bigoplus_{\beta} N_\beta),
$$

$$
\bigoplus_{\alpha} (M_\alpha \otimes_A L(N)) \to (\bigoplus_{\alpha} M_\alpha) \otimes_A L(N).
$$

An analogous reasoning gives :

#### Proposition 8 {#alg-x-s4-prop-8 .statement}

*Let I (resp. J) be a right filtered preordered set, (($M_\alpha$, $u_{\alpha', \alpha}$) (resp. (($N_\beta$, $v_{\beta', \beta}$))) an inductive system of right A-modules (resp. left) relative to I (resp. J). The homomorphism of graded k-modules*

$$
\lim_{\longrightarrow (\alpha, \beta) \in I \times J} \mathrm{Tor}^A(M_\alpha, N_\beta) \to \mathrm{Tor}^A\left( \lim_{\longrightarrow \alpha \in I} M_\alpha, \lim_{\longrightarrow \beta \in J} N_\beta \right),
$$

*deduced from the canonical A-homomorphisms* $M_\alpha \to \lim_{\longrightarrow} M_\alpha$ *and* $N_\beta \to \lim_{\longrightarrow} N_\beta$, *is bijective*.

In particular, taking $J = I$ and remarking that the $(\alpha, \alpha), \alpha \in I$, form a cofinal subset of $I \times I$, one obtains :

#### Corollary {#alg-x-s4-n4-cor-2 .statement}

Let I be a right filtered preordered set, $(M_i, u_{ji})$ (resp. $(N_i, v_{ji})$) an inductive system of right $A$-modules (resp. left) relative to I. The homomorphism of graded $k$-modules

$$
\lim_{\longrightarrow i \in I} \operatorname{Tor}^A(M_i, N_i) \to \operatorname{Tor}^A\left(\lim_{\longrightarrow i \in I} M_i, \lim_{\longrightarrow i \in I} N_i\right),
$$

deduced from the canonical $A$-homomorphisms $M_i \to \lim_{\longrightarrow} M_i$ and $N_j \to \lim_{\longrightarrow} N_j$ is bijective.

#### 5. Linking Homomorphisms and Exact Sequences

Let $M$ be a right $A$-module, $N$ a left $A$-module, $A^\circ$ the opposite ring of $A$, $M^\circ$ the $A^\circ$-left module underlying $M$, $N^\circ$ the $A^\circ$-right module underlying $N$. We have $L(M^\circ ) = L(M)^\circ $ and $L(N^\circ ) = L(N)^\circ $, whence a commutation isomorphism (X, p. 63, prop. 2)

$$
\sigma(L(M), L(N)) : L(M) \otimes_A L(N) \to L(N^\circ) \otimes_{A^\circ} L(M^\circ).
$$

Passing to homology, $\sigma(L(M), L(N))$ induces a graded isomorphism of degree 0 $\sigma_{M,N} : \operatorname{Tor}^A(M, N) \to \operatorname{Tor}^{A^\circ}(N^\circ, M^\circ)$ called the *commutation isomorphism of torsion products*.

Let us note that $\sigma_{N^\circ, M^\circ} \circ \sigma_{M,N} = \mathrm{Id}_{\operatorname{Tor}(M,N)}$ and that $\sigma_{M,N}$ induces on the degree 0 terms the commutation homomorphism of the tensor product. On the other hand, if $f : M \to M'$ and $g : N \to N'$ are homomorphisms of $A$-modules, then

$$
\operatorname{Tor}^{A^\circ}(g, f) \circ \sigma_{M,N} = \sigma_{M', N'} \circ \operatorname{Tor}^A(f, g).
$$

### 5. The linking homomorphisms and exact sequences

Let $M$ be a right $A$-module. Let us recall that for every left $A$-module $N$, an isomorphism

$$
\psi_M(N) : \operatorname{Tor}^A(M, N) \to H(L(M) \otimes_A N)
$$

was defined in the previous section (X, p. 69, prop. 5). Let

$$(\mathcal{E})$$
$$
0 \to N' \xrightarrow{u} N \xrightarrow{v} N'' \to 0
$$

be an exact sequence of left $A$-modules; then the sequence of $k$-complexes

$$(\mathcal{ME})$$
$$
0 \longrightarrow L(M) \otimes_A N' \xrightarrow{1 \otimes u} L(M) \otimes_A N \xrightarrow{1 \otimes v} L(M) \otimes_A N'' \longrightarrow 0
$$

is then exact (X, p. 66, Lemma 1); denote by

$$
\partial^{(\mathcal{ME})} : H(L(M) \otimes_A N'') \to H(L(M) \otimes_A N')
$$

the corresponding linking homomorphism (X, p. 29).

#### Definition 2 {#alg-x-s4-def-2 .statement}

The linking homomorphism of torsion products, relative to the module $M$ and the exact sequence $\mathcal{E}$, is the composite homomorphism

$$
\partial(M, \mathcal{E}) = \psi_M(N')^{-1} \circ \partial^{(M\mathcal{E})} \circ \psi_M(N'') : \mathrm{Tor}^A(M, N'') \to \mathrm{Tor}^A(M, N')
$$

This is a graded $k$-homomorphism of degree $-1$, whose homogeneous components are denoted $\partial_n(M, \mathcal{E}) : \mathrm{Tor}_n^A(M, N'') \to \mathrm{Tor}_{n-1}^A(M, N')$.

#### Theorem 1 {#alg-x-s4-thm-1 .statement}

The left-infinite sequence of $k$-module homomorphisms

$$
\cdots \longrightarrow \mathrm{Tor}_n^A(M, N') \xrightarrow{\mathrm{Tor}_n^A(1, u)} \mathrm{Tor}_n^A(M, N) \xrightarrow{\mathrm{Tor}_n^A(1, v)} \mathrm{Tor}_n^A(M, N'')
$$
$$
\xrightarrow{\partial_n(M, \mathcal{E})} \mathrm{Tor}_{n-1}^A(M, N') \xrightarrow{\mathrm{Tor}_{n-1}^A(1, u)} \cdots \xrightarrow{\mathrm{Tor}_1^A(1, v)} \mathrm{Tor}_1^A(M, N'')
$$
$$
\xrightarrow{\hat{c}_1(M, \mathcal{E})} M \otimes_A N' \xrightarrow{1 \otimes u} M \otimes_A N \xrightarrow{1 \otimes v} M \otimes_A N'' \longrightarrow 0
$$

is exact.

To see this, consider the diagram

$$
\begin{array}{ccccccccc}
\mathrm{Tor}(M, N') & \xrightarrow{\mathrm{Tor}(1, u)} & \mathrm{Tor}(M, N) & \xrightarrow{\mathrm{Tor}(1, v)} & \mathrm{Tor}(M, N'') & \xrightarrow{\partial(M, \mathcal{E})} & \mathrm{Tor}(M, N') & \xrightarrow{\mathrm{Tor}(1, u)} & \mathrm{Tor}(M, N) \\
\psi_M(N') \downarrow & & \psi_M(N) \downarrow & & \psi_M(N'') \downarrow & & \psi_M(N') \downarrow & & \psi_M(N') \downarrow \\
H(L(M) \otimes N') & \xrightarrow{H(1 \otimes u)} & H(L(M) \otimes N) & \xrightarrow{H(1 \otimes v)} & H(L(M \otimes N'') & \xrightarrow{\partial^{(M\mathcal{ME})}} & H(L(M) \otimes N') & \xrightarrow{H(1 \otimes u)} & H(L(M) \otimes N)
\end{array}
$$

It commutes according to (X, p. 69, Remark 3) and Definition 2. Furthermore, the bottom row is exact (X, p. 30, Thm. 1), and the different $\psi_M$ are bijections (X, p. 69, prop. 5).

#### Corollary 1 {#alg-x-s4-thm-1-cor-1 .statement}

If $\mathrm{Tor}_1^A(M, N'') = 0$, the sequence

$$
0 \longrightarrow M \otimes_A N' \xrightarrow{1 \otimes u} M \otimes_A N \xrightarrow{1 \otimes v} M \otimes_A N'' \longrightarrow 0
$$

is exact.

#### Corollary 2 {#alg-x-s4-thm-1-cor-2 .statement}

Let $0 \to C' \xrightarrow{u} C \xrightarrow{v} C'' \to 0$ be an exact sequence of complexes of left $A$-modules, and let $E$ be a complex of right $A$-modules. If $C''$ or $E$ is flat, the sequence

$$
0 \longrightarrow E \otimes_A C' \xrightarrow{1 \otimes u} E \otimes_A C \xrightarrow{1 \otimes v} E \otimes_A C'' \longrightarrow 0
$$

is exact.

Indeed, $\mathrm{Tor}_1^A(E, C'') = 0$ according to X, p. 69, Corollary to prop. 5.

#### Example {#alg-x-s4-n5-exa-1 .statement}

Let $a$ be an ideal of $A$. The exact sequence

$$
0 \to a \to A_s \to A/a \to 0
$$

of left a-modules, gives rise to an exact sequence of torsion products, in which the terms Tor$_i^A$ (M, A) are zero for $i > 0$. From this one deduces isomorphisms

$$
\operatorname{Tor}_{i+1}^A(M, A/\alpha) \to \operatorname{Tor}_i^A(M, \alpha), \quad i > 0
$$

and an exact sequence

$$
0 \to \operatorname{Tor}_1^A(M, A\alpha) \to M \otimes_A \alpha \to M \otimes_A A \to M \otimes A \alpha \to 0 :
$$

it follows that $\operatorname{Tor}_1^A(M, A/\alpha)$ is identified with the kernel of the canonical homomorphism $M \otimes_A \alpha \to M$.

For example, taking for M a module of the form $A_d/b$, where b is a right ideal of A, one obtains an isomorphism of $\operatorname{Tor}_1^A(A/b, A/\alpha)$ onto $(\alpha \cap b)/ba$.

#### Proposition 9 {#alg-x-s4-prop-9 .statement}

*Let f : M → M$_1$ be a homomorphism of right a-modules and*

$$
\begin{array}{ccccccccc}
0 & \longrightarrow & N' & \xrightarrow{u} & N & \xrightarrow{v} & N'' & \longrightarrow & 0 \\
& & g' \downarrow & & g \downarrow & & g'' \downarrow & & \\
0 & \longrightarrow & N'_1 & \xrightarrow{u_1} & N_1 & \xrightarrow{v_1} & N''_1 & \longrightarrow & 0
\end{array}
$$

*(E$_1$)*

*a commutative diagram with exact rows of homomorphisms of left a-modules. The diagram of k-modules*

$$
\begin{array}{ccc}
\operatorname{Tor}^A(M, N'') & \xrightarrow{\partial(M, E)} & \operatorname{Tor}^A(M, N') \\
\operatorname{Tor}^A(f, g'') \downarrow & & \operatorname{Tor}^A(f, g') \downarrow \\
\operatorname{Tor}^A(M_1, N''_1) & \xrightarrow{\partial(M_1, E_1)} & \operatorname{Tor}^A(M_1, N'_1)
\end{array}
$$

*is commutative.*

This follows from X, p. 31, prop. 2, applied to the commutative diagram

$$
\begin{array}{ccccccccc}
0 & \longrightarrow & L(M) \otimes_A N' & \xrightarrow{1 \otimes u} & L(M) \otimes_A N & \xrightarrow{1 \otimes v} & L(M) \otimes_A N'' & \longrightarrow & 0 \\
& & L(f) \otimes g' \downarrow & & L(f) \otimes g \downarrow & & L(f) \otimes g'' \downarrow & & \\
0 & \longrightarrow & L(M_1) \otimes_A N'_1 & \xrightarrow{1 \otimes u_1} & L(M_1) \otimes_A N_1 & \xrightarrow{1 \otimes v_1} & L(M_1) \otimes_A N''_1 & \longrightarrow & 0 .
\end{array}
$$

In an analogous way, if N is a left a-module and

$$(F)$$
$$
0 \to M' \xrightarrow{r} M \xrightarrow{s} M'' \to 0
$$

an exact sequence of right a-modules, one defines *linking homomorphisms*

$$
\partial(F, N) : \operatorname{Tor}^A(M'', N) \to \operatorname{Tor}^A(M', N)
$$
$$
\partial_n(F, N) : \operatorname{Tor}_n^A(M'', N) \to \operatorname{Tor}_{n-1}^A(M', N)
$$

by $\partial(\mathcal F,\mathbf N)=\overline{\psi}_{\mathbf N}(M')^{-1}\circ\partial(\mathcal F^{\mathbf N})\circ\overline{\psi}_{\mathbf N}(M'')$, where $\partial(\mathcal F^{\mathbf N})$ is the linking homomorphism of
the exact sequence

$$(\mathcal F_{\mathbf N})\qquad 0\longrightarrow M'\otimes_A L(N)\longrightarrow M\otimes_A L(N)\longrightarrow M''\otimes_A L(N)\longrightarrow 0$$

deduced from $\mathcal F$, and one has:

**THEOREM 1 bis.** — *The left-unbounded sequence of homomorphisms of $k$-modules*

$$\longrightarrow \operatorname{Tor}_n^A(M',N)\xrightarrow{\operatorname{Tor}_n^A(r,1)}\operatorname{Tor}_n^A(M,N)\xrightarrow{\operatorname{Tor}_n^A(s,1)}\operatorname{Tor}_n^A(M'',N)\xrightarrow{\partial_n(\mathcal F,N)}\operatorname{Tor}_{n-1}^A(M',N)$$

$$\cdots\longrightarrow \operatorname{Tor}_1^A(M'',N)\xrightarrow{\partial_1(\mathcal F,N)}M'\otimes_A N\xrightarrow{r\otimes1}M\otimes_A N\xrightarrow{s\otimes1}M''\otimes_A N\longrightarrow0$$

*is exact.*

We leave to the reader the task of stating and proving the properties analogous to the corollaries of th. 1 and to prop. 9. Moreover:

#### Proposition 10 {#alg-x-s4-prop-10 .statement}

*Let us denote by $(\mathcal F^\circ)$ the exact sequence of left $A$-modules*

$$0\longrightarrow M'\xrightarrow{r}M\xrightarrow{s}M''\longrightarrow0.$$

*The diagram*

$$
\begin{array}{ccccc}
\operatorname{Tor}^A(M'',N)&\xrightarrow{\partial(\mathcal F,N)}&\operatorname{Tor}^A(M',N)\\
\Big\downarrow{\sigma_{M'',N}}&&\Big\downarrow{\sigma_{M',N}}\\
\operatorname{Tor}^{A^\circ}(N^\circ,{M''}^\circ)&\xrightarrow{\partial(N^\circ,\mathcal F^\circ)}&\operatorname{Tor}^{A^\circ}(N^\circ,{M'}^\circ)
\end{array}
$$

*is commutative.*

Indeed, this follows from X, p. 31, prop. 2, applied to the commutative diagram

$$
\begin{array}{ccccccccc}
0&\longrightarrow&M'\otimes_A L(N)&\xrightarrow{r\otimes1}&M\otimes_A L(N)&\xrightarrow{s\otimes1}&M''\otimes_A L(N)&\longrightarrow&0\\
&&\Big\downarrow{\sigma(M',L(N))}&&\Big\downarrow{\sigma(M,L(N))}&&\Big\downarrow{\sigma(M'',L(N))}\\
0&\longrightarrow&L(N^\circ)\otimes_{A^\circ}{M'}^\circ&\xrightarrow{1\otimes r}&L(N^\circ)\otimes_{A^\circ}M^\circ&\xrightarrow{1\otimes s}&L(N^\circ)\otimes_{A^\circ}{M''}^\circ&\longrightarrow&0 .
\end{array}
$$

We shall see later other commutation relations *(cf.* X, p. 131, cor. 1*).*

### 6. Flat modules and torsion products

#### Theorem 2 {#alg-x-s4-thm-2 .statement}

*Let E be a right $A$-module. The following conditions are equi-*
*valent :*

(i) E *is flat* ;

(ii) *for every* left $A$-module F, *and every integer* $n>0$, *one has*

$$\operatorname{Tor}_n^A(E,F)=0\,;$$

(iii) For every cyclic left $A$-module $F$ of finite presentation, we have
$$
\operatorname{Tor}_1^A(E, F) = 0 ;
$$
(iv) For every left ideal $a$ of $A$ of finite type, the canonical mapping $E \otimes_A a \to E$ is injective;
(v) For every exact sequence of right $A$-modules of the form
$$
0 \to G \xrightarrow{\nu} H \xrightarrow{w} E \to 0,
$$
and every left $A$-module $F$, the sequence
$$
0 \longrightarrow G \otimes_A F \xrightarrow{\nu \otimes 1} H \otimes_A F \xrightarrow{w \otimes 1} E \otimes_A F \longrightarrow 0
$$
is exact.
(i) $\Rightarrow$ (ii): This is the corollary to Prop. 5 of X, p. 69.
(ii) $\Rightarrow$ (iii): This is trivial.
(iii) $\Leftrightarrow$ (iv): Every cyclic left $A$-module of finite presentation is isomorphic to a quotient $A/a$, where $a$ is a left ideal of finite type, so (iii) is equivalent to (iv) according to X, p. 72, Example.
(iii) $\Rightarrow$ (i): According to X, p. 8, Prop. 3, X, p. 72, Th. 1, $E$ is flat as soon as $\operatorname{Tor}_1^A(E, F) = 0$ for every left $A$-module $F$. If (iii) is satisfied, this is the case when $F$ is cyclic and of finite presentation. According to X, p. 11, Prop. 7, every $A$-module (resp. every cyclic $A$-module) is a filtered inductive limit of modules of finite presentation (resp. of cyclic modules of finite presentation); hence, according to X, p. 70, Prop. 8, it suffices to prove that if $\operatorname{Tor}_1^A(E, F) = 0$ when $F$ is cyclic, then this is also the case when $F$ is of finite type. We therefore proceed by induction on the cardinal of a system of generators $(f_1, \ldots, f_n)$ of $F$; the exact sequence
$$
0 \to Af_1 \to F \to F/Af_1 \to 0
$$
gives rise to an exact sequence
$$
\operatorname{Tor}_1^A(E, Af_1) \to \operatorname{Tor}_1^A(E, F) \to \operatorname{Tor}_1^A(E, F/Af_1),
$$
so that $\operatorname{Tor}_1^A(E, F) = 0$ since $\operatorname{Tor}_1^A(E, Af_1) = 0$ and $\operatorname{Tor}_1^A(E, F/Af_1) = 0$ by the induction hypothesis.
(i) $\Rightarrow$ (v): This is Corollary 2 to Th. 1 (X, p. 72).
(v) $\Rightarrow$ (iii): The exact sequence (X, p. 50)
$$
0 \longrightarrow Z_0(E) \xrightarrow{i_E} L_0(E) \xrightarrow{p_E} E \longrightarrow 0
$$
gives rise, for every left $A$-module $F$, to an exact sequence
$$
0 \longrightarrow \operatorname{Tor}_1^A(E, F) \longrightarrow Z_0(E) \otimes_A F \xrightarrow{i_E \otimes 1} L_0(E) \otimes_A F \xrightarrow{p_E \otimes 1} E \otimes_A F \longrightarrow 0.
$$
If (v) is satisfied, we have $\operatorname{Tor}_1^A(E, F) = 0$, whence (iii).

#### Corollary 1 {#alg-x-s4-thm-2-cor-1 .statement}

Let $0 \to E' \to E \to E'' \to 0$ be an exact sequence of right $A$-modules. Assume that $E''$ is flat. Then $E$ is flat if and only if $E'$ is flat.

Let $F$ be a left $A$-module. Since $\operatorname{Tor}^A_i(E'', F)=0$ for $i=1,2$ (Th. 2, (i) $\Rightarrow$ (ii)), we have an exact sequence
$$
0\longrightarrow \operatorname{Tor}^A_1(E',F)\longrightarrow \operatorname{Tor}^A_1(E,F)\longrightarrow 0
$$
whence the assertion (Th. 2, (i) $\Leftrightarrow$ (iii)).

**Corollary 2. —** *Let*
$$
0\longrightarrow E_n\longrightarrow E_{n-1}\longrightarrow\cdots\longrightarrow E_1\longrightarrow0
$$
*be an exact sequence of right $A$-modules.* *If $E_i$ is flat for $i=1,\ldots,n-1$, then $E_n$ is flat.*

### 7. **Künneth Formula**

In this section, we consider a complex $(C,d)$ of right $A$-modules and a complex $(C',d')$ of left $A$-modules. Let
(I)
$$
0\longrightarrow Z(C)\xrightarrow{i}C\xrightarrow{\delta}B(C)(-1)\longrightarrow0,
$$
(II)
$$
0\longrightarrow B(C)\xrightarrow{i}Z(C)\xrightarrow{p}H(C)\longrightarrow0;$$
be the canonical exact sequences.

From $\delta$ we deduce a $k$-homomorphism

$$
H(\delta\otimes 1):H(C\otimes_A C')\longrightarrow H(B(C)\otimes_A C')(-1);
$$

from (II) we deduce a connecting homomorphism

$$
\partial(\mathrm{II},H(C')): \operatorname{Tor}^A_1(H(C),H(C'))\longrightarrow B(C)\otimes_A H(C');
$$

if we equip $\operatorname{Tor}^A_1(H(C),H(C'))$ with the grading whose homogeneous component of degree $n$ is

$$
\bigoplus_{p+q=n}\operatorname{Tor}^A_1(H_p(C),H_q(C')),
$$

this connecting homomorphism is graded of degree 0. We also have a canonical homomorphism (X, p. 62)

$$
\gamma(B(C),C'): B(C)\otimes_A H(C')\longrightarrow H(B(C)\otimes_A C').
$$

With these notations:

#### Theorem 3. — *Assume that the $A$-modules $B(C)$ and $Z(C)$ are flat. There exists a unique homomorphism of graded $k$-modules, of degree $-1$,

$$
\alpha:H(C\otimes_A C')\longrightarrow\operatorname{Tor}^A_1(H(C),H(C'))
$$

making the following diagram commute*

$$
\begin{array}{ccc}
H(C\otimes_A C') & \xrightarrow{\alpha} & \operatorname{Tor}^A_1(H(C),H(C'))(-1)\\
{\scriptstyle H(\delta\otimes1)}\downarrow & & \downarrow{\scriptstyle\partial(\mathrm{II},H(C'))}\\
H(B(C)\otimes_A C')(-1) & \xleftarrow{\gamma(B(C),C')} & (B(C)\otimes_A H(C'))(-1).
\end{array}
$$

The sequence of graded $k$-modules

$$
0 \longrightarrow \mathrm{H}(C) \otimes_A \mathrm{H}(C') \xrightarrow{\gamma(C,C')} \mathrm{H}(C \otimes_A C') \xrightarrow{\alpha} \mathrm{Tor}_1^A(\mathrm{H}(C), \mathrm{H}(C'))(-1) \longrightarrow 0
$$

is exact.

Thus, for each $n$, we have an exact sequence

(11)
$$
\begin{array}{cccccc}
0 & \longrightarrow & \bigoplus_{p+q=n} \mathrm{H}_p(C) \otimes_A \mathrm{H}_q(C') & \xrightarrow{\gamma_n(C,C')} & \mathrm{H}_n(C \otimes_A C') \\
& & & \xrightarrow{\alpha_n} & \bigoplus_{p+q=n-1} \mathrm{Tor}_1^A(\mathrm{H}_p(C), \mathrm{H}_q(C')) & \longrightarrow 0 .
\end{array}
$$

For simplicity, set $B = B(C)$, $Z = Z(C)$, $H = H(C)$, and $H' = H(C')$.

Since $B$ is flat, from (I) we deduce an exact sequence (X, p. 72, Corollary 2)

(12)
$$
0 \longrightarrow Z \otimes_A C' \xrightarrow{j \otimes 1} C \otimes_A C' \xrightarrow{\delta \otimes 1} (B \otimes_A C')(-1) \longrightarrow 0 .
$$

#### Lemma 3 {#alg-x-s4-lem-3 .statement}

The connecting homomorphism $\mathrm{H}(B \otimes_A C') \to \mathrm{H}(Z \otimes_A C')$ associated with the exact sequence (12) is equal to $\mathrm{H}(i \otimes 1)$.

Indeed, let $a \in \mathrm{H}(B \otimes_A C')$; since $B$ is flat, $a$ belongs to the image of $B \otimes_A Z(C')$, hence can be written as $\sum_\lambda da_\lambda \otimes b_\lambda$, where $a_\lambda \in C$, $b_\lambda \in C'$, and $db_\lambda = 0$. The image of the class of $a$ under the connecting homomorphism is, by definition, the class of $D(\sum a_\lambda \otimes b_\lambda) = \sum da_\lambda \otimes b_\lambda = (i \otimes 1)(a)$, which proves the lemma.

The associated homology exact sequence to (12) is therefore

$$
\mathrm{H}(B \otimes_A C') \xrightarrow{\mathrm{H}(i \otimes 1)} \mathrm{H}(Z \otimes_A C') \xrightarrow{\mathrm{H}(j \otimes 1)} \mathrm{H}(C \otimes_A C')
$$
$$
\xrightarrow{\mathrm{H}(\delta \otimes 1)} \mathrm{H}(B \otimes_A C')(-1) \xrightarrow{\mathrm{H}(i \otimes 1)} \mathrm{H}(Z \otimes_A C')(-1) .
$$

On the other hand, since $Z$ is flat, from (II) we obtain a sequence of graded $k$-modules

$$
0 \longrightarrow \operatorname{Tor}_1^A(H, H') \xrightarrow{\partial(\mathrm{II}, H')} B \otimes_A H' \xrightarrow{i \otimes 1} Z \otimes_A H' \xrightarrow{p \otimes 1} H \otimes_A H' \longrightarrow 0 ;
$$

finally, we have the canonical homomorphisms of No. 1

$$
\gamma_B = \gamma(B, C') : B \otimes_A H' \to \mathrm{H}(B \otimes_A C')
$$
$$
\gamma_Z = \gamma(Z, C') : Z \otimes_A H' \to \mathrm{H}(Z \otimes_A C')
$$
$$
\gamma_C = \gamma(C, C') : H \otimes_A H' \to \mathrm{H}(C \otimes_A C') ,
$$

whence a diagram of graded $k$-modules, with *exact rows*:

$$
\begin{array}{ccccccccc}
B \otimes H' & \xrightarrow{i \otimes 1} & Z \otimes H' & \xrightarrow{p \otimes 1} & H \otimes H' & \longrightarrow & 0 \\
\downarrow \gamma_B & & \downarrow \gamma_Z & & \downarrow \gamma_C & & \\
H(B \otimes C') & \xrightarrow{H(i \otimes 1)} & H(Z \otimes C') & \xrightarrow{H(j \otimes 1)} & H(C \otimes_A C') & \xrightarrow{H(\delta \otimes 1)} & H(B \otimes C')(-1) & \xrightarrow{H(i \otimes 1)} & H(Z \otimes C')(-1)
\end{array}
$$

$$
0 \longrightarrow \operatorname{Tor}_1^A(H, H')(-1) \xrightarrow{\partial(\mathrm{II}, H')} (B \otimes H')(-1) \xrightarrow{i \otimes 1} (Z \otimes H')(-1),
$$

which is *commutative by definition of the homomorphisms $\gamma$*. But since the complexes $B$ and $Z$ are split and flat, $\gamma_B$ and $\gamma_Z$ are *bijective* (X, p. 65, Corollary 1). From this, on the one hand, we deduce that $\gamma_C$ is injective and has image equal to $\operatorname{Ker} H(\delta \otimes 1)$, and on the other hand, that $\gamma_B \circ \partial(\mathrm{II}, H')$ is injective with image equal to $\operatorname{Im} H(\delta \otimes 1)$. The theorem follows immediately from this.

#### Corollary 1 {#alg-x-s4-lem-3-cor-1 .statement}

*If $B(C)$ and $Z(C)$ are flat, then for every left $A$-module $N$ and every integer $n$, there is an exact sequence*

(13) $$ 0 \longrightarrow H_n(C) \otimes_A N \xrightarrow{\gamma_n} H_n(C \otimes_A N) \xrightarrow{\alpha_n} \operatorname{Tor}_1^A(H_{n-1}(C), N) \longrightarrow 0 . $$

#### Corollary 2 {#alg-x-s4-lem-3-cor-2 .statement}

*Suppose $B(C)$ and $B(C')$ are projective and $Z(C)$ is flat. Then the sequences of $k$-modules (11) and (13) are exact and split.*
This follows from the theorem and the following lemma:

#### Lemma 4 {#alg-x-s4-lem-4 .statement}

*If $B(C)$ and $B(C')$ are projective, then the canonical homomorphism*
$$ \gamma(C, C') : H(C) \otimes_A H(C') \to H(C \otimes_A C') $$
*has a $k$-linear retraction.*
Indeed by X, p. 65, *remark b)*, there exist homologisms $\varphi : C \to H(C)$ and $\varphi' : C' \to H(C')$ such that $H(\varphi) = 1_{H(C)}$ and $H(\varphi') = 1_{H(C')}$. In the commutative diagram

$$
\begin{array}{ccc}
H(C) \otimes_A H(C') & \xrightarrow{\gamma(C, C')} & H(C \otimes_A C') \\
\downarrow H(\varphi) \otimes H(\varphi') & & \downarrow H(\varphi \otimes \varphi') \\
H(C) \otimes_A H(C') & \xrightarrow{\gamma(H(C), H(C'))} & H(C) \otimes_A H(C')
\end{array}
$$

$H(\varphi) \otimes H(\varphi')$ and $\gamma(H(C), H(C'))$ are the identity, whence the assertion.

**Corollary 3** (*universal coefficient formula*). — *Suppose the ring $A$ is principal. If the complexes $C$ and $C'$ are free, the sequences of $A$-modules (11) are exact and split; if the complex $C$ is free, the sequences of $A$-modules (13) are exact and split for every $A$-module $N$.*
Indeed, $B(C), Z(C)$ and $B(C')$ are submodules of the free modules $C, C, C'$, so are free (VII, § 3, cor. 2 to th. 1), and we apply cor. 2.

#### Corollary 4 (« Künneth formula ») {#alg-x-s4-lem-4-cor-4 .statement}

Suppose C bounded on the right, C and H(C) flat; then the canonical homomorphism

$$
\gamma(C, C') : H(C) \otimes_A H(C') \to H(C \otimes_A C')
$$

is bijective.

By the theorem, it suffices to proving that B(C) and Z(C) are flat. Now one has exact sequences

$$
\begin{align*}
0 &\to B_n(C) \to Z_n(C) \to H_n(C) \to 0 \\
0 &\to Z_n(C) \to C_n \to B_{n-1}(C) \to 0,
\end{align*}
$$

whence, by X, p. 75, cor. 1, implications (B_{n-1}(C) is flat) $\Rightarrow$ (Z_n(C) is flat) $\Rightarrow$ (B_n(C) is flat) ; we conclude by remarking that B_n(C) = 0 for n small enough.

#### Corollary 5 {#alg-x-s4-lem-4-cor-5 .statement}

Let u : C \to C' be a homologism of complexes of right a-modules, flat and bounded on the right. For every complex E of left a-modules, the morphism $u \otimes 1_E : C \otimes_A E \to C' \otimes_A E$ is a homologism.

Indeed, Con (u) is a flat complex, bounded on the right and of zero homology; then one has H(Con (u) \otimes_A E) = 0 by cor. 4, hence H(Con (u \otimes 1_E)) = 0 (X, p. 67, lemma 2), and $u \otimes 1_E$ is a homologism.

### 8. Bounded and flat complexes over a noetherian ring

#### Proposition 11 {#alg-x-s4-prop-11 .statement}

Suppose A left noetherian, and let C be a bounded and flat complex of left a-modules such that H(C) is a finitely generated a-module. Let a and b be two integers such that a \leq b and H_n(C) = 0 for n < a, C_n = 0 for n > b. There exists a complex P of left a-modules such that P_n is projective and finitely generated for each n, and P_n = 0 for n \notin [a, b], and a homologism u : P \to C. Moreover, for every complex E of right a-modules, the homomorphism

$$
H(1_E \otimes u) : H(E \otimes_A P) \to H(E \otimes_A C) \quad \text{is bijective}.
$$

By X, p. 53, prop. 7, there exists a complex (L, d) such that L_n is free and finitely generated for each n, and zero when n < a, and a homologism f : L \to C. Let P be the quotient complex L/L', where L'_n = 0 for n < b, L'_n = L_n for n > b, L'_b = B_b(L). Since C_n = 0 for n > b, f(L') = 0, so f factors through a morphism of complexes u : P \to C.

$$
\begin{array}{ccccccccc}
\ldots & \longrightarrow & L_{b+1} & \xrightarrow{d_{b+1}} & L_b & \xrightarrow{d_b} & L_{b-1} & \longrightarrow & \ldots \\
& & \downarrow & & \downarrow & & \downarrow & & \\
& & 0 & \longrightarrow & P_b & \longrightarrow & P_{b-1} & \longrightarrow & \ldots \\
& & \downarrow & & \downarrow^{u_b} & & \downarrow^{u_{b-1}} & & \\
& & 0 & \longrightarrow & C_b & \longrightarrow & C_{b-1} & \longrightarrow & \ldots
\end{array}
$$

Since $f$ is a homologism, one has $H(\operatorname{Con}(f))=0$, whence an exact sequence

$$
\cdots \longrightarrow L_{b+1} \xrightarrow{d_{b+1}} L_b \longrightarrow L_{b-1}\oplus C_b \longrightarrow L_{b-2}\oplus C_{b-1} \longrightarrow \cdots
$$

One then has an exact sequence

$$
0\longrightarrow P_b\longrightarrow L_{b-1}\oplus C_b\longrightarrow L_{b-2}\oplus C_{b-1}\longrightarrow\cdots.
$$

This shows on the one hand that the cone of $u$ is of zero homology, so that $u$ is a homologism, on the other hand that the module $P_b$ is *flat* (X, p. 76, cor. 2) ; since $P_b$ is finitely generated as a quotient of $L_{b+1}$, it is *projective* (X, p. 13, cor.). The pair $(P,u)$ then satisfies the required condition. The last assertion follows from X, p. 79, cor. 5.

\* **Example.** — Let A be a commutative noetherian ring, X a proper and flat A-scheme, $\mathcal F$ a coherent $\mathcal C_X$-module, flat over A. There exists a bounded complex P consisting of finitely generated projective A-modules such that for every A-module M, $H(X,\mathcal F\otimes_A M)$ identifies naturally with $H(P\otimes_A M)$. Indeed, let $\mathcal U$ be a covering of X by a finite number of affine open sets, $\mathcal C(\mathcal U,\mathcal F)$ the associated Čech complex. One shows that $H^i(\mathcal C(\mathcal U,\mathcal F))$ is isomorphic to the A-module $H^i(X,\mathcal F)$, and that the latter is finitely generated; moreover, for every A-module M, the complex $\mathcal C(\mathcal U,\mathcal F)\otimes_A M$ is isomorphic to $\mathcal C(\mathcal U,\mathcal F\otimes_A M)$. Applying Prop. 11 to the complex $\mathcal C(\mathcal U,\mathcal F)$ (which is bounded), one obtains a complex P that answers the question.

For every point $y$ of Spec (A), let $\kappa(y)$ denote the residue field of A at $y$, $X_y=X\otimes_A\kappa(y)$ the fibre of X over $y$, $\mathcal F_y=\mathcal F\otimes_A\kappa(y)$, and set $h^p(y)=\dim_{\kappa(y)}H^p(X_y,\mathcal F_y)$ for $p\geq 0$.

One easily deduces the following results from the existence of the complex P :

(i) the function $h^p$ is upper semi-continuous on Spec (A) ;

(ii) the function $\displaystyle\sum_{p\geq 0}(-1)^p h^p$ is locally constant on Spec (A). \*

### 9. Generalization to multimodule complexes

Let B and B′ be two rings, C a complex of (B, A)-bimodules, C′ a complex of (A, B′)-bimodules (X, p. 43); then $(C\otimes_A C',D)$ (X, p. 61) is a complex of (B, B′)-bimodules and the canonical homomorphism

$$
\gamma:H(C)\otimes_A H(C')\longrightarrow H(C\otimes_A C')
$$

is compatible with the (B, B′)-bimodule structures of the two members.

If B″ is a third ring, and C″ a complex of (B′, B″)-bimodules, the canonical homomorphism (II, p. 64, Prop. 8)

$$
(C\otimes_A C')\otimes_{B'}C''\longrightarrow C\otimes_A(C'\otimes_{B'}C'')
$$

is an isomorphism of complexes of (B, B″)-bimodules.

More generally, we leave it to the reader to develop the theory of tensor products of finite, totally ordered families of *multimodule complexes* on the model of No. 1 (X, p. 63) and of II, pp. 65–72 (associativity, commutativity, … isomorphisms).

Let B and B' be two rings, M a (B, A)-bimodule, N an (A, B')-bimodule :
then $L(M)\otimes_A L(N)$ is a complex of (B, B')-bimodules, so that $\operatorname{Tor}^A(M,N)$ is endowed with a natural structure of graded (B, B')-bimodule; on the term of degree 0, this structure coincides with that of $M\otimes_A N$.

If $\lambda\in B$, $\lambda'\in B'$, and if we denote by $\lambda_M,\lambda_N,\lambda_T,\lambda'_T$ the homotheties $x\mapsto\lambda x$, $y\mapsto y\lambda'$, $z\mapsto\lambda z$, $z\mapsto z\lambda'$ of $M$, $N$, $\operatorname{Tor}^A(M,N)$, $\operatorname{Tor}^A(M,N)$ respectively, then

$$
\lambda_T=\operatorname{Tor}^A(\lambda_M,1_N),\qquad
\lambda'_T=\operatorname{Tor}^A(1_M,\lambda_N'),
$$

which gives another description of the bimodule structure of $\operatorname{Tor}^A(M,N)$.
We leave it to the reader to generalize Nos. 5 and 7 to the case of multimodule complexes.

## EXERCISES {#alg-x-s4-exercises}

See the [exercises for § 4](exercises/s4/).
