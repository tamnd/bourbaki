---
book: alg
book_title: Algebra
chapter: X
chapter_title: ALGÈBRE HOMOLOGIQUE
section: 9
section_title: Complexes de Koszul
lang: en
source: alg-x-fr
book_pages: A X.147-A X.168, A X.206-A X.216
pdf_pages: 0153-0174, 0212-0222
extraction: ocr
subsections:
    - "no": 1
      title: Les complexes $\mathbf{K}(u)$, $\mathbf{K}.(u, C)$, $\mathbf{K}^*(u, C)$
      page: 147
      pdf_page: 153
    - "no": 2
      title: Fonctorialité
      page: 150
      pdf_page: 156
    - "no": 3
      title: 'Exemple 1 : le complexe $S(L) \otimes_A \Lambda(L)$'
      page: 151
      pdf_page: 157
    - "no": 4
      title: 'Exemple 2 : le cas d’un module libre'
      page: 153
      pdf_page: 159
    - "no": 5
      title: 'Exemple 3 : le cas $L = A$'
      page: 156
      pdf_page: 162
    - "no": 6
      title: Familles complètement sécantes
      page: 157
      pdf_page: 163
    - "no": 7
      title: Un critère pour les suites complètement sécante
      page: 159
      pdf_page: 165
    - "no": 8
      title: 'Démonstration du théorème 1 : première partie'
      page: 161
      pdf_page: 167
    - "no": 9
      title: 'Démonstration du théorème 1 : deuxième partie'
      page: 163
      pdf_page: 169
    - "no": 10
      title: Classe d’extensions associée à une suite régulière
      page: 165
      pdf_page: 171
statements: 35
exercises: 10
content_sha256: d4957bb3ac1fc8e376a572314bfd00cbabab87776df84d39b3e13113c9574cf0
translated_from: content/fr/alg/X/09_s9_complexes_de_koszul.md
source_lang: fr
translation_method: machine
source_content_sha256: 234fe2945aa4e961036016372d407d506dc8b4e0d5b9dad9251bdb87e41d0c74
translation_model: gpt-5-6, gpt-5.4, gpt-5-6-mini
translation_run: translate-en-mt-2cb97f2e
glossary_version: 34
glossary_terms_sha256: bd089b249cb1135d6ab514c65821b3fa53ae7e31d056e188b3c4103257fbba2e
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 9. KOSZUL COMPLEXES

In this paragraph, all the rings considered are commutative.

### 1. The complexes $\mathbf{K}(u)$, $\mathbf{K}.(u, C)$, $\mathbf{K}^*(u, C)$

Let $A$ be a ring, $L$ an $A$-module, $u : L \to A$ a linear form, and $\Lambda(L)$ the exterior algebra of the $A$-module $L$. For $x \in \Lambda(L)$, denote by $d_u(x)$ the interior product $x \cdot u$ (III, p. 161, example). According to loc. cit., p. 162, formula (60), one has

$$
(1)\quad d_u(e_1 \wedge \ldots \wedge e_n) = \sum_{i=1}^n (-1)^{i+1} u(e_i) \; e_1 \wedge \ldots \wedge e_{i-1} \wedge e_{i+1} \wedge \ldots \wedge e_n
$$

for $e_1, \ldots, e_n$ in $L$. According to III, p. 164 and 165, the mapping $d_u : \Lambda(L) \to \Lambda(L)$ is an antidifferentiation of degree $(-1)$ and of square zero. It is the unique antidifferentiation of the $A$-algebra $\Lambda(L)$ which extends $u : \Lambda^1(L) \to \Lambda^0(L)$.

#### Definition 1 {#alg-x-s9-def-1 .statement}

The complex $(\Lambda(L), d_u)$ is denoted by $\mathbf{K}^A(u)$ or $\mathbf{K}(u)$.

One should note that $\mathbf{K}_n(u) = \Lambda^n(L) = \mathbf{K}^{-n}(u)$. It is clear that $\mathbf{K}(u)$ is zero on the right and that $H_0(\mathbf{K}(u)) = \mathrm{Coker}\,(u) = A/q$ where $q$ is the ideal $u(L)$ of $A$.

For every complex of $A$-modules $C$, put

$$
\begin{aligned}
\mathbf{K}^A(u, C) &= C \otimes_A \mathbf{K}^A(u), \\
H^A(u, C) &= H(C \otimes_A \mathbf{K}^A(u)) \\
H_r^A(u, C) &= H_r(C \otimes_A \mathbf{K}^A(u)),
\end{aligned}
$$
$$
\begin{aligned}
\mathbf{K}^*_A(u, C) &= \mathrm{Homgr}_A(\mathbf{K}^A(u), C), \\
H^*_A(u, C) &= H(\mathrm{Homgr}_A(\mathbf{K}^A(u), C)), \\
H^r_A(u, C) &= H^r(\mathrm{Homgr}_A(\mathbf{K}^A(u), C)).
\end{aligned}
$$

There are therefore canonical homomorphisms of $A$-modules (X, p. 62 and p. 82)

$$
\begin{aligned}
\gamma_0 : H_0(C) \otimes_A A/q &\to H^A_0(u, C), \\
\lambda^0 : H^0_A(u, C) &\to \mathrm{Hom}_A(A/q, H^0(C)).
\end{aligned}
$$

#### Lemma 1 {#alg-x-s9-lem-1 .statement}

If the complex $C$ is zero on the right (resp. on the left), then $\mathbf{K}^A(u, C)$ (resp. $\mathbf{K}^*_A(u, c)$) is zero on the right (resp. on the left), and $\gamma_0$ (resp. $\lambda^0$) is bijective.

This follows from X, p. 62, prop. 1 and p. 82, prop. 1.

#### Proposition 1 {#alg-x-s9-prop-1 .statement}

Let $x \in L$; denote by $R_x : y \mapsto x \wedge y$ the left multiplication by $x$ in the algebra $\Lambda(L)$. Then $d_u \circ R_x + R_x \circ d_u = u(x) \cdot 1_{\Lambda(L)} = u(x)_{\Lambda(L)}$.

Indeed $(d_u \circ R_x + R_x \circ d_u)(y) = d_u(x \wedge y) + x \wedge d_u(y)$; since $d_u$ is an antidifferentiation, $d_u(x \wedge y) + x \wedge d_u(y) = d_u(x) \wedge y = u(x) \cdot y$.

#### Corollary 1 {#alg-x-s9-prop-1-cor-1 .statement}

If $u$ is surjective, $K(u)$ is homotopic to zero (X, p. 34) as well as $K^A(u, C)$ and $K_A^*(u, C)$ for every complex $C$.

Indeed, there exists $x \in L$ such that $u(x) = 1$. Then $K(u)$ is homotopic to zero by the proposition 1, and therefore also $K^A(u, C)$ (X, p. 64, prop. 3) and $K_A^*(u, C)$ (X, p. 83, prop. 3).

#### Corollary 2 {#alg-x-s9-prop-1-cor-2 .statement}

Let $C$ be a complex, Ann (C) its annihilator. Then $q + \mathrm{Ann}(C)$ annihilates $H^A(u, C)$ and $H_A^*(u, C)$.

For every $\lambda \in q$, the homothety $\lambda_{K(u)}$ is homotopic to zero by the proposition, hence so also are $1_C \otimes \lambda_{K(u)}$ and Homgr ($\lambda_{K(u)}, 1_C$) by X, p. 64, prop. 3 and X, p. 83, prop. 3; it follows that $\lambda$ annihilates $H(u, C)$ and $H^*(u, C)$. If $\lambda \in \mathrm{Ann}(C)$, then $1_{K(u)} \otimes \lambda_C$ and Homgr ($1_{K(u)}, \lambda_C$) are zero.

Suppose $L$ projective (resp. $K(u)$ acyclic in degrees > 0). Then the complex $\Lambda(L)$ is projective by III, p. 87, cor. 2 (resp. is a resolution of $A/q$); by X, p. 102 (resp. p. 100), one therefore has, for every $A$-module $M$, homomorphisms

(2) $H_r^A(u, M) \to \mathrm{Tor}_r^A(A/q, M)$, $\mathrm{Ext}_A^r(A/q, M) \to H_r^A(u, M)$
resp.
(3) $\mathrm{Tor}_r^A(A/q, M) \to H_r^A(u, M)$, $H_r(u, M) \to \mathrm{Ext}_A^r(A/q, M)$.

If $L$ is projective and $K(u)$ acyclic in degrees > 0, the homomorphisms (2) and (3) above are bijective and reciprocal to one another (X, p. 102, prop. 1).

#### Proposition 2 {#alg-x-s9-prop-2 .statement}

Let $(L_i)_{i \in I}$ be a family of $A$-modules, where the set $I$ is finite and totally ordered. Let $u$ be a linear form on $\bigoplus_{i \in I} L_i$, $u_i$ its restriction to $L_i$.

The canonical isomorphism of $A$-algebras (III, p. 84)

$$
g : \bigotimes_{i \in I} \Lambda(L_i) \to \Lambda(\bigoplus_{i \in I} L_i)
$$

is an isomorphism of the complex $\bigotimes_{i \in I} K(u_i)$ (X, p. 63) onto the complex $K(u)$.

In fact, by X, p. 64, remark 4, the differential $D$ of the complex $\bigotimes_{i \in I} K(u_i)$ is an antiderivation; the antiderivations $d_u$ and $g \circ D \circ g^{-1}$ of $\Lambda(\bigoplus L_i)$ coincide on $\bigoplus L_i$ with the mapping $x \mapsto u(x).1$ of $\bigoplus L_i$ into $\Lambda(\bigoplus L_i)$, hence are equal (III, p. 128, cor.).

Let $C$ and $C'$ be two complexes of $A$-modules. One has (X, p. 63 and p. 99) canonical isomorphisms of complexes

$$
C \otimes_A (C' \otimes_A K(u)) \to (C \otimes_A C') \otimes_A K(u)
$$
$$
\mathrm{Homgr}_A(C', \mathrm{Homgr}_A(K(u), C)) \to \mathrm{Homgr}_A(C' \otimes_A K(u), C),
$$

that is, *isomorphisms*

(4) $$
C \otimes_A K^A(u, C') \to K^A(u, C \otimes_A C')
$$

(5) $$
\operatorname{Homgr}_A(C', K^i_A(u, C)) \to \operatorname{Homgr}_A(K^A(u, C'), C)
$$

Dans (4) and (5), take $C' = K(u')$, where $u' : L' \to A$ is a linear form on an $A$-module $L'$, and note that $K^A(u, K(u'))$ which is equal by definition to $K(u') \otimes_A K(u)$ is identified, according to Prop. 2, with $K(u' \oplus u)$ where $u' \oplus u : L' \oplus L \to A$ is the linear form $(x', x) \mapsto u'(x') + u(x)$. We then obtain isomorphisms of complexes

(6) $$
K^A(u' \oplus u, C) \to K^A(u, K^A(u', C))
$$

(7) $$
K^i_A(u', K^i_A(u, C)) \to K^i_A(u' \oplus u, C)
$$

By passing to homology, we deduce isomorphisms of $A$-modules

$$
H^A_r(u' \oplus u, C) \to H^A_r(u, K^A(u', C)) , \qquad r \in \mathbf{Z} ,
$$
$$
H^r_A(u', K^i_A(u, C)) \to H^r_A(u' \oplus u, C) , \qquad r \in \mathbf{Z} .
$$

Finally note that the homomorphism deduced from the product in the algebra $\Lambda(L)$

$$
m : K^A(u) \otimes_A K^A(u) \to K^A(u)
$$

is a morphism of *complexes* (since $d_u$ is an antiderivation). Supposing that $L$ is *free of rank n* and composing with the morphism of complexes $K^A(u) \to \Lambda^n L(-n)$ which is the identity in degree $n$, we deduce a morphism of complexes

$$
\chi : K^A(u) \otimes_A K^A(u) \to \Lambda^n L(-n) ;
$$

to this morphism corresponds canonically, according to X, p. 99, Prop. 12, a morphism of complexes

$$
\varphi : K^A(u) \to \operatorname{Homgr}_A(K^A(u), \Lambda^n L(-n))
$$

which is *bijective* (III, p. 87, formula (20)). For every complex $C$, we deduce a composed isomorphism

$$
K^A(u, C) = C \otimes_A K^A(u) \xrightarrow{1 \otimes \varphi} C \otimes \operatorname{Homgr}_A(K^A(u), \Lambda^n L(-n)) \to \\
\to \operatorname{Homgr}_A(K^A(u), C \otimes_A \Lambda^n L(-n)) = K^i_A(u, C \otimes_A \Lambda^n L(-n)) .
$$

By passing to homology, we therefore have *canonical* isomorphisms

(8) $$
H^A_r(u, C) \to H^{n-r}_A(u, C \otimes_A \Lambda^n L) , \qquad r \in \mathbf{Z} .
$$

*Remarks. — 1)* \* The above remains valid when $L$ is projective of rank $n$. \*

2) Since $L$ is free of rank $n$, $\Lambda^n L$ is isomorphic to $A$, and we have non-canonical isomorphisms $H^A_r(u,C)\to H^{n-r}_A(u,C)$.

### 2. Functoriality

Let $f:C\to C'$ be a morphism of complexes. We denote

$$
K^A(u,f):K^A(u,C)\to K^A(u,C'),
$$

$$
K_A(u,f):K_A(u,C)\to K_A(u,C'),
$$

the morphisms of complexes $f\otimes 1_{K(u)}$ and $\operatorname{Hom}_{A}(1_{K(u)},f)$.

We denote by $H^A(u,f):H^A(u,C)\to H^A(u,C')$, $H_A(u,f):H_A(u,C)\to H_A(u,C')$,
$H^A_r(u,f):H^A_r(u,C)\to H^A_r(u,C')$, $H^A_r(u,f):H^A_r(u,C)\to H^A_r(u,C')$ the morphisms induced in homology. The mapping $f\mapsto K^A(u,f)$ is linear; if $g:C'\to C''$ is another morphism of complexes, we have $K^A(u,g\circ f)=K^A(u,g)\circ K^A(u,f)$; analogously for $K_A$, $H^A$, $H_A$, $H^A_r$, $H^A_r$.

Let $0\to C'\xrightarrow{f}C\xrightarrow{g}C''\to0$ be an exact sequence of complexes.

a) Suppose $L$ is flat; then $\Lambda(L)$ is flat (X, p. 15, Cor.). The sequence

$$
0\to K^A(u,C')\xrightarrow{K^A(u,f)}K^A(u,C)\xrightarrow{K^A(u,g)}K^A(u,C'')\to0
$$

is then exact, and gives rise (X, p. 30) to an exact sequence of homology

$$
\cdots\to H^A_n(u,C')\xrightarrow{H_n(u,f)}H^A_n(u,C)
\xrightarrow{H_n(u,g)}H^A_n(u,C'')
\xrightarrow{\partial_n}H^A_{n-1}(u,C')\to\cdots .
$$

b) Suppose $L$ is projective; then $\Lambda(L)$ is projective. The sequence

$$
0\to K_A(u,C')\xrightarrow{K_A(u,f)}K_A(u,C)
\xrightarrow{K_A(u,g)}K_A(u,C'')\to0
$$

is then exact, and gives rise to an exact sequence of homology

$$
\cdots\to H^n_A(u,C')\xrightarrow{H^n(u,f)}H^n_A(u,C)
\xrightarrow{H^n(u,g)}H^n_A(u,C'')
\xrightarrow{\delta^n}H^{n+1}_A(u,C')\to\cdots .
$$

Let $\rho:A\to A'$ be a ring homomorphism, $L'$ the $A'$-module $A'\otimes_A L$, $u':L'\to A'$ the linear form $1\otimes u$. The bijective canonical homomorphism (III, p. 83, Prop. 8)

$$
\psi:\Lambda_{A'}(A'\otimes_A L)\to A'\otimes_A\Lambda_A(L)
$$

is an isomorphism of complexes of $A'$-modules. It follows that:

1) for every complex of $A'$-modules $C'$, an isomorphism of complexes of $A$-modules

$$
K^{A'}_{A}(u',C')\to K^A_A(u,C'),
$$

composed of the diagram

$$
C' \otimes_{A'} (\Lambda_A(A' \otimes_A L)) \xrightarrow{1_C \otimes \psi} C' \otimes_{A'} A' \otimes_A \Lambda_A(L) \to C' \otimes_A \Lambda_A(L)
$$

where $\varphi$ is the canonical bijection (III, p. 85, Prop. 14);

2) for every complex of $A$-modules $C$, an *isomorphism* of complexes of $A'$-modules

$$
K^A(u, A' \otimes_A C) \to A' \otimes_A K^A(u, C),
$$

whence homomorphisms of $A'$-modules

$$
A' \otimes_A H_n^A(u, C) \to H_n^{A'}(u', A' \otimes_A C),
$$

which are bijective when $A'$ is *flat* over $A$ (X, p. 66, Cor. 2).

Let $L'$ be an $A$-module, $u' : L' \to A$ a linear form, $f : L \to L'$ an $A$-homomorphism such that $u' \circ f = u$. It follows from III, p. 161, formula (55), that the homomorphism $\Lambda(f) : \Lambda(L) \to \Lambda(L')$ satisfies $d_u \circ \Lambda(f) = \Lambda(f) \circ d_{u'}$, hence defines a *morphism of complexes* $\Lambda(u) : K^A(u) \to K^A(u')$. If $C$ is an $A$-complex, it follows that there are morphisms of complexes

$1_C \otimes \Lambda(u) : K^A(u, C) \to K^A(u', C)$ and $\mathrm{Homgr}(\Lambda(u), 1_C) : K_A^*(u', C) \to K_A^*(u, C)$.

If $f$ is bijective, all these morphisms are isomorphisms.

### 3. Example 1: the complex $S(L) \otimes_A \Lambda(L)$

Let $A$ be a ring, $L$ an $A$-module, $S(L)$ its symmetric algebra, $S(L) \otimes_A L$ the $S(L)$-module deduced by extension of scalars, $u : S(L) \otimes_A L \to S(L)$ the linear form such that $u(s \otimes x) = sx$ for $s \in S(L), x \in L$. By the canonical isomorphism of $S(L)$-modules (III, p. 83, Prop. 8)

$$
\Lambda_{S(L)}(S(L) \otimes_A L) \to S(L) \otimes_A \Lambda(L),
$$

the differential of the complex $K^{S(L)}(u)$ is carried over into the mapping

$$
d : S(L) \otimes_A \Lambda(L) \to S(L) \otimes_A \Lambda(L)
$$

such that, for $x_1, ..., x_p, y_1, ..., y_q$ in $L$, one has

$$
\begin{align}
(9) \quad d((x_1 ... x_p) \otimes (y_1 \wedge ... \wedge y_q)) \\
&= \sum_{i=1}^q (-1)^{i+1} y_i x_1 ... x_p \otimes (y_1 \wedge ... \wedge y_{i-1} \wedge y_{i+1} \wedge ... \wedge y_q).
\end{align}
$$

Note that $d$ maps $S^p(L) \otimes \Lambda^q(L)$ into $S^{p+1}(L) \otimes \Lambda^{q-1}(L)$, hence that the *complex of $A$-modules* $S(L) \otimes \Lambda(L)$ decomposes into the direct sum of the complexes described by the following diagrams:

$$
(\mathcal{E}_n) : 0 \to S^0 L \otimes_A \Lambda^n L \to S^1 L \otimes_A \Lambda^{n-1} L \to ... \to S^n L \otimes_A \Lambda^0 L \to 0, \quad n \in \mathbf{N}.
$$

If the A-module L is the direct sum of a finite family $(L_i)_{i \in I}$ where I is totally ordered, the canonical bijection

$$
\bigotimes_{i \in I} (\mathbf{S}(L_i) \otimes_A \Lambda(L_i)) \to \mathbf{S}(L) \otimes_A \Lambda(L)
$$

is an isomorphism of complexes of A-modules (this follows from prop. 2 of X, p. 148 or from formula (9) above).

#### Proposition 3 {#alg-x-s9-prop-3 .statement}

*If the A-module L is flat, the sequences $(\mathcal{E}_n)$ above are exact for $n > 0$.*

*a)* Let us first note that, if $p_L$ is the composite homomorphism

$$
\mathbf{S}(L) \otimes \Lambda(L) \xrightarrow{\alpha} \mathbf{S}^0(L) \otimes \Lambda^0(L) \xrightarrow{\beta} A,
$$

where $\alpha$ is the tensor product of the canonical projections and $\beta$ the canonical isomorphism, it remains to prove that $H(p_L)$ is *bijective*.

*b)* If $L = 0$ or if $L = A$, the proposition is obvious.

*c)* Suppose L is free of finite rank; write it as the direct sum $L_1 \oplus ... \oplus L_n$ of free A-modules of rank 1. According to the remark preceding the proposition, the complex $\mathbf{S}(L) \otimes \Lambda(L)$ is isomorphic to the tensor product of the $n$ *free* complexes $\mathbf{S}(L_i) \otimes \Lambda(L_i)$ whose homology is *free* according to *b)*. According to X, p. 79, cor. 4, the canonical homomorphism

$$
\gamma : \bigoplus_{i=1}^n H(\mathbf{S}(L_i) \otimes \Lambda(L_i)) \to H(\mathbf{S}(L) \otimes \Lambda(L))
$$

is bijective. According to *b)* $H(p_{L_i})$ is bijective for every $i$. Since $\bigotimes_{i=1}^n H(p_{L_i}) = H(p_L) \circ \gamma$,

$$
H(p_L) \text{ is bijective}.
$$

*d)* In the general case, L is an inductive limit of a filtered inductive system $(L_i)_{i \in I}$ of free modules of finite rank (X, p. 14, th. 1). Since the canonical bijective homomorphism

$$
\varprojlim \mathbf{S}(L_i) \otimes \Lambda(L_i) \to \mathbf{S}(L) \otimes \Lambda(L)
$$

is an isomorphism of complexes, the proposition follows from X, p. 28, prop. 1.

#### Remark 1 {#alg-x-s9-n3-rem-1 .statement}

We shall see below (X, p. 158, example) another proof of part *c)* above.

#### Remark 2 {#alg-x-s9-n3-rem-2 .statement}

If A is a $\mathbf{Q}$-algebra, the conclusion of prop. 3 remains true without assumption on L (*cf.* X, p. 206, exercise 1).

#### Remark 3 {#alg-x-s9-n3-rem-3 .statement}

Let G be a group and $\rho : G \to \mathbf{GL}(L)$ a linear representation of G in a flat A-module L. Then the $(\mathcal{E}_n)$ are exact sequences of linear representations. Suppose L finitely generated projective, and denote by $R_A(G)$ the ring of representations of G in finitely generated projective A-modules. It follows from prop. 3 that one has in R_A(G) the relations

$$
\sum_{i=0}^{n} (-1)^i [\mathbf{S}^i(L)] [\Lambda^{n-i}(L)] = 0 , \quad n > 0 .
$$

If one considers the formal series

$$
s(T) = \sum_{i=0}^{\infty} [\mathbf{S}^i(L)] T^i \in R_A(G)[[T]] ,
$$
$$
\lambda(T) = \sum_{i=0}^{\infty} [\Lambda^i(L)] T^i \in R_A(G)[[T]] ,
$$

the relations (10) are written

$$
s(T) \lambda(-T) = 1_* .
$$

### 4. Example 2 : the case of a free module

Let k be a ring, M a k-module, I a set and p an integer $\geqslant 0$. A mapping $m : I^p \to M$ is said to be *alternating* if it satisfies the following two conditions:

a) for every permutation $\sigma \in S_p$ and every sequence $(\alpha_1, ..., \alpha_p) \in I^p$, one has

$$
m(\alpha_{\sigma(1)}, ..., \alpha_{\sigma(p)}) = \varepsilon_{\sigma} m(\alpha_1, ..., \alpha_p) ,
$$

b) for every sequence $(\alpha_1, ..., \alpha_p) \in I^p$ such that two of the indices $\alpha_1, ..., \alpha_p$ are equal, one has $m(\alpha_1, ..., \alpha_p) = 0$.
(In the case where I is a k-module and m is multilinear, one recovers the notion introduced in III, p. 80.)

*Suppose I finite* and denote by $C_I^p(M)$ the k-module of alternating mappings of $I^p$ into M.

Let $L_0$ be a k-module, $(e_i)_{i \in I}$ a family of elements of $L_0$; one defines two k-linear mappings

$$
g : \mathrm{Hom}_k (\Lambda^p L_0, M) \to C_I^p(M)
$$
$$
h : C_I^p(M) \to M \otimes_k \Lambda^p L_0
$$

as follows: if $f \in \mathrm{Hom}_k (\Lambda^p L_0, M)$, one sets

$$
g(f)(\alpha_1, ..., \alpha_p) = f(e_{\alpha_1} \wedge ... \wedge e_{\alpha_p}) ;
$$

let $m \in C_I^p(M)$, define $h(m) \in M \otimes_k \Lambda^p L_0$. For every element $(\alpha_1, ..., \alpha_p)$ of $I^p$, the element $m(\alpha_1, ..., \alpha_p) \otimes (e_{\alpha_1} \wedge ... \wedge e_{\alpha_p})$ of $\Lambda^p L_0 \otimes_k M$ is zero if $\mathrm{Card}\{ \alpha_1, ..., \alpha_p \} < p$ and is independent of the order of the indices $\alpha_1, ..., \alpha_p$ if
$$
\mathrm{Card}\{ \alpha_1, ..., \alpha_p \} = p .
$$
It depends only on the subset $J = (\alpha_1, ..., \alpha_p)$ of $I$; denote it by $h_J(m)$; we have $h_J(m) = 0$ if $\mathrm{Card}(J) < p$; we then set:
$$
h(m) = \sum_J h_J(m) ,
$$
where $J$ runs through the subsets of $I$ having $p$ elements.

#### Lemma 2 {#alg-x-s9-lem-2 .statement}

*If the k-module $L_0$ is free with basis $(e_i)_{i \in I}$, the k-linear mappings g and h are bijective.*
This follows from III, p. 79, th. 1.

Let $M$ be a $k$-module, and let $x = (x_i)_{i \in I}$ be a family of $k$-endomorphisms of $M$, pairwise permutable. Consider the polynomial ring $A = k[(X_i)_{i \in I}]$ and endow $M$ with the structure of an $A$-module such that $P(X_i) m = P(x_i) m$ for $P \in A$ and $m \in M$. Let moreover $L$ be the free $A$-module $A^I$, $(e_i)_{i \in I}$ its canonical basis and $u : L \to A$ the linear form which maps $e_i$ onto $X_i$ for all $i \in I$. Consider the complexes of $k$-modules $K_A^*(u, M)$ and $K_A^*(u, M)$; one has *canonical isomorphisms*
$$
K_A^p(u, M) = \mathrm{Hom}_A(\Lambda_A^p(A^I), M) \to \mathrm{Hom}_k(\Lambda_k^p(k^I), M) ,
$$
$$
M \otimes_k \Lambda_k^p(k^I) \to M \otimes_A \Lambda_A^p(A^I) = K_A^p(u, M) ;
$$
whence by composition with the isomorphisms $g$ and $h$ *isomorphisms of k-modules*
$$
\theta^p : K_A^p(u, M) \to C_I^p(M) ,
$$
$$
\theta_p : C_I^p(M) \to K_A^p(u, M) .
$$
We denote by
$$
\partial^p : C_I^p(M) \to C_I^{p+1}(M) ,
$$
$$
\partial_p : C_I^p(M) \to C_I^{p-1}(M) ,
$$
the $k$-homomorphisms obtained by transporting the differentials of $K_A^*(u, M)$ and $K_A^*(u, M)$ by the isomorphisms $\theta$. For example, one has:
(12) $$
(\partial^p m)(\alpha_1, ..., \alpha_{p+1}) = \sum_{j=1}^{p+1} (-1)^{j+1} x_{\alpha_j} m(\alpha_1, ..., \alpha_{j-1}, \alpha_{j+1}, ..., \alpha_{p+1}) .
$$
The complex formed by the $C_I^p(M)$ and the $\partial^p$ (resp. the $\partial_p$) is denoted by $K^*(x, M)$ (resp. $K.(x, M)$) and is called *the ascending (resp. descending) Koszul complex* associated with the module M and the sequence of endomorphisms $(x_1, ..., x_n)$. One therefore has isomorphisms of complexes of $k$-modules

$$
\theta^*: K_A^*(u, M) \to K^*(x, M),
$$
$$
\theta_*: K_*(x, M) \to K_A^*(u, M).
$$

#### Remark {#alg-x-s9-n4-rem-1 .statement}

Conversely, let B be a $k$-algebra, L a free B-module with basis $(e_i)_{i \in I}$, and M a B-module. The datum of a linear form $u : L \to B$ is equivalent to that of a family $x = (x_i)_{i \in I}$ of elements of B, by the relation $x_i = u(e_i)$. The underlying complex of $k$-modules of $K_B^*(u, M)$ (resp. $K^B(u, M)$) is then identified, by the isomorphism $\theta^*$ (resp. $\theta_*$) with the Koszul complex $K^*(x, M)$ (resp. $K_*(x, M)$). For example $K^B(u)$ is identified with $K^*(x, B)$.

The notations $H_*(x, M)$, $H_*(x, M)$, etc., are introduced as in No. 1 (X, p. 147), and all the results of Nos. 1 and 2 apply mutatis mutandis, the module $A^I$ being free. We have for example isomorphisms

$$
H_0(x, M) \to M/(x) M
$$
$$
H^0(x, M) \to \operatorname{Hom}_A(A/(x), M),
$$

where $(x)$ denotes the ideal $\sum A x_i$ of A. For example also, if $K_*(x, A)$ is acyclic in degrees $> 0$, we have isomorphisms

$$
H_r(x, M) \to \operatorname{Tor}_r^A(k, M),
$$
$$
\operatorname{Ext}_A^r(k, M) \to H^r(x, M).
$$

Finally, suppose that I is (finite and) totally ordered, for example $I = \{ 1, ..., n \}$; identify $\Lambda^n(A^I)$ with A thanks to the basis element $e_1 \wedge ... \wedge e_n$ and translate the isomorphism $K_p^A(u, M) \to K_A^{n-p}(u, M)$ of X, p. 149. It becomes, by transport by $(\theta_p)$ and $(\theta^{n-p})$, the isomorphism

$$
C_1^p(M) \to C_1^{n-p}(M)
$$

which associates with $m \in C_1^p(M)$ the element $\tilde{m}$ of $C_1^{n-p}(M)$ such that

$$
m(\alpha_1, ..., \alpha_p) = \tilde{m}(\beta_1, ..., \beta_{n-p})
$$

if $(\alpha_1, ..., \alpha_p, \beta_1, ..., \beta_{n-p})$ is an *even* permutation of $\{ 1, ..., n \}$. Let us also remark that when $I = \{ 1, ..., n \}$, we can identify $C_1^p(M)$ with the set of families $m(\alpha_1, ..., \alpha_p)$ of elements of M where $\alpha_1 < \alpha_2 < ... < \alpha_p$; formula (12) remains valid, as does relation (13).

#### Example {#alg-x-s9-n4-exa-1 .statement}

Take $M = k[T_1, ..., T_n]$; the Koszul complex $K (\partial/\partial T, M)$ associated with the sequence of endomorphisms $(\partial/\partial T_1, ..., \partial/\partial T_n)$ is identified with the de Rham complex of $k[x_1, ..., x_n]$ over $k$ (X, p. 44): with $m \in C_{\{1,...,n\}}^p(M)$, we associate the differential form

$$
\omega(m) = \sum_{\alpha_1 < ... < \alpha_p} m(\alpha_1, ..., \alpha_p)\ dx_{\alpha_1} \wedge ... \wedge dx_{\alpha_p},
$$

cf. formula (12) and Example 1, p. 44.

### 5. Example 3 : the case $L = A$

If $L = A$, put $u(1) = x \in A$. The complex $K(u)$ is then of length 1, we have $K_0(u) = K_1(u) = A$ and $d_1(a) = xa$, hence for every $A$-module $M$, $K_0(u, M)$, $K_1(u, M)$, $K^0(u, M)$ and $K^1(u, M)$ are identified with $M$, the differentials

$$
d_1 : K_1(u, M) \to K_0(u, M) \quad \text{and} \quad d^0 : K^0(u, M) \to K^1(u, M)
$$

being $m \mapsto xm$. We therefore have isomorphisms

$$
H_0(x, M) \to A/xA \otimes_A M \leftarrow H^1(x, M),
$$
$$
H_1(x, M) \to \mathrm{Hom}_A(A/xA, M) \leftarrow H^0(x, M).
$$

#### Lemma 3 {#alg-x-s9-lem-3 .statement}

Let $K$ be a complex such that $K_i = 0$ for $i \neq 0, 1$, and let $C$ be a complex and $p$ an integer.

a) If $K$ is flat, there is for every $p \in \mathbf{N}$ an exact sequence

$$
0 \to H_0(K \otimes_A H_p(C)) \to H_p(K \otimes_A C) \to H_1(K \otimes_A H_{p-1}(C)) \to 0.
$$

b) If $K$ is projective, we have for every $p \in \mathbf{N}$ an exact sequence

$$
0 \to H^1(\mathrm{Homgr}_A(K, H^{p-1}(C))) \to H^p(\mathrm{Homgr}_A(K, C))
$$
$$
\to H^0(\mathrm{Homgr}_A(K, H^p(C))) \to 0.
$$

Let us prove a), the proof of b) being analogous. For every $i$, denote by $K_{(i)}$ the complex $K_i(-i)$. We have an exact sequence of complexes, split as a sequence of $A$-modules

$$
0 \to K_{(0)} \xrightarrow{\alpha} K \xrightarrow{\beta} K_{(1)} \to 0;
$$

the sequence

$$
\begin{array}{ccccccccc}
0 & \longrightarrow & K_{(0)} \otimes_A C & \xrightarrow{\alpha \otimes 1} & K \otimes_A C & \xrightarrow{\beta \otimes 1} & K_{(1)} \otimes_A C & \longrightarrow & 0
\end{array}
$$

is exact, and $K$ being flat, the homomorphisms

$$
\gamma_{0,p}(K_{(0)}, C) : K_{(0)} \otimes_A H_p(C) \to H_p(K_{(0)} \otimes_A C)
$$
$$
\gamma_{1,p-1}(K_{(1)}, C) : K_{(1)} \otimes_A H_{p-1}(C) \to H_p(K_{(1)} \otimes_A C)
$$

are bijective (X, p. 66, cor. 2). Let us calculate the connecting homomorphism $\partial(\alpha \otimes 1,\beta \otimes 1)$; by definition, it maps the class of the cycle $\sum a_i \otimes b_i$ onto that of $\sum d a_i \otimes b_i$, which means that

$$
\partial(\alpha \otimes 1,\beta \otimes 1)\circ\gamma(K_{(1)},\mathbf C)=\gamma(K_{(0)},\mathbf C)\circ(d_K\otimes 1).
$$

The exact homology sequence associated with (14) therefore has the form

$$
K_1\otimes H_p(\mathbf C)\xrightarrow{d_k\otimes 1}K_0\otimes H_p(\mathbf C)\longrightarrow H_p(K\otimes\mathbf C)
$$

$$
\hspace{7cm}\longrightarrow K_1\otimes H_{p-1}(\mathbf C)\xrightarrow{d_k\otimes 1}K_0\otimes H_{p-1}(\mathbf C),
$$

whence a).

Applying Lemma 3, a) to the complex $K(u)$, and using the commutation isomorphisms, we obtain:

#### Proposition 4 {#alg-x-s9-prop-4 .statement}

*For every complex $C$, there are exact sequences .*

$$
0\longrightarrow A/xA\otimes_A H_p(C)\longrightarrow H_p(x,C)\longrightarrow \operatorname{Hom}_A(A/xA,H_{p-1}(C))\longrightarrow 0.
$$

#### Corollary 1 {#alg-x-s9-prop-4-cor-1 .statement}

*For $H_p(x,C)=0$ to hold, it is necessary and sufficient that the homothety with ratio $x$ in $H_p(C)$ be surjective and that the homothety with ratio $x$ in $H_{p-1}(C)$ be injective.*

#### Corollary 2 {#alg-x-s9-prop-4-cor-2 .statement}

*Let $x=(x_1,\ldots,x_n)$ be a sequence of elements of $A$, $M$ an $A$-module, $x'$ the sequence $(x_1,\ldots,x_{n-1})$. We have exact sequences*

$$
0\longrightarrow A/x_nA\otimes_A H_p(x',M)\longrightarrow H_p(x,M)\longrightarrow \operatorname{Hom}_A(A/x_nA,H_{p-1}(x',M))\longrightarrow 0.
$$

#### Corollary 3 {#alg-x-s9-prop-4-cor-3 .statement}

*For $H_i(x,M)$ to be zero for all $i>0$, it is necessary and sufficient that the homothety with ratio $x_n$ in $H_i(x',M)$ be bijective for $i>0$, and that the homothety with ratio $x_n$ in $M/(x')M$ be injective.*

### 6. Completely transverse families

Let $A$ be a ring, $M$ an $A$-module, $x=(x_i)_{i\in I}$ a family of elements of $A$.

#### Definition 2 {#alg-x-s9-def-2 .statement}

*The family $x$ is said to be completely transverse for $M$ if one has $H_i(x,M)=0$ for $i>0$.*

If $I$ is finite, it amounts to the same thing (X, p. 150) to say that one has $H^i(x,M)=0$ for $i<\operatorname{Card}(I)$.

The following proposition makes it possible to give examples of completely transverse families.

#### Proposition 5 {#alg-x-s9-prop-5 .statement}

*Let $x=(x_1,\ldots,x_n)$ be a sequence of elements of $A$. If for $i=1,\ldots,n$, the homothety of ratio $x_i$ in the $A$-module $M/(x_1M+\cdots+x_{i-1}M)$ is injective, the sequence $x$ is completely secant for $M$.*

A sequence satisfying the conditions of the proposition is said to be regular for M, or M-regular. We shall note that this property depends in general on the order of the $x_i$; for example the sequence $(1, 0)$ is always M-regular, whereas the sequence $(0, 1)$ is so only if M is zero. On the other hand, the fact that a sequence is completely secant does not depend on the order of the terms.

Let us prove the proposition by induction on $n$, the case $n = 0$ being immediate. Put $x' = (x_1, ..., x_{n-1})$; if the sequence $x$ is M-regular, the sequence $x'$ is M-regular and multiplication by $x_n$ in $M/(x')M$ is injective; by the induction hypothesis, we have $H_i(x', M) = 0$ for $i > 0$; it then follows from cor. 3 of X, p. 157, that $H_i(x, M) = 0$ for $i > 0$.

#### Example {#alg-x-s9-n6-exa-1 .statement}

Let $k$ be a ring; take $A = k[X_1, ..., X_n]$ and $x = (X_1, ..., X_n)$. The sequence $x$ is A-regular and the proposition gives again the acyclicity in degrees $> 0$ of the complex $S_k(k^n) \otimes_k \Lambda_k(k^n)$ (cf. X, p. 152, prop. 3).
Likewise in the ring of formal series $\hat{A} = k[[X_1, ..., X_n]]$, the sequence $(X_1, ..., X_n)$ is $\hat{A}$-regular, hence completely secant for $\hat{A}$.

#### Proposition 6 {#alg-x-s9-prop-6 .statement}

a) If $\sum_{i \in I} x_i A = A$, the family $(x_i)_{i \in I}$ is completely secant for M.
b) Let $x = (x_1, ..., x_n)$ be a sequence of elements of A. Let $(a_{ij}) \in \mathrm{GL}_n(A)$; put
$$
y_i = \sum_j a_{ij} x_j.
$$
If the sequence $x$ is completely secant for M, the same is true of the sequence $(y_1, ..., y_n)$.
c) Let $k_1, ..., k_n$ be integers $\geqslant 1$; in order that the sequence $(x_1^{k_1}, ..., x_n^{k_n})$ be completely secant for M, it is necessary and sufficient that the sequence $x$ be completely secant for M.
Assertion a) follows from cor. 1, p. 148.
Let us prove b). Let $f : A^n \to A^n$ be the isomorphism defined by the matrix $^t(a_{ij})$; it follows from X, p. 151, that $1_M \otimes \Lambda(f)$ is an isomorphism of the complex $K.(y, M)$ onto the complex $K.(x, M)$, whence b).
To prove c), it is obviously enough to prove that if $k$ is an integer $\geqslant 1$, the sequence $(x_1, ..., x_{n-1}, x_n^k)$ is completely secant for M if and only if the same is true of the sequence $x$. Let $x' = (x_1, ..., x_{n-1})$; by cor. 3, p. 157, the first condition (resp. the second) means that the homothety of ratio $x_n^k$ (resp. $x_n$) is bijective in $H_i(x', M)$ for $i \geqslant 1$ and injective in $M/(x')M$. These two conditions are clearly equivalent, whence c).

#### Remark 1 {#alg-x-s9-n6-rem-1 .statement}

The assertion analogous to c) for regular sequences is true (X, p. 207, exercise 5).

#### Proposition 7 {#alg-x-s9-prop-7 .statement}

a) Let N be a flat A-module. If the family x is completely secant for M, it is so for $M \otimes_A N$.

b) Let $0 \to M' \to M \to M'' \to 0$ be an exact sequence of $A$-modules. If the family $x$ is completely transverse for $M'$ and for $M''$, it is so for $M$.

The complex $K.(x, M \otimes_A N)$ is isomorphic by definition to $K.(x, M) \otimes_A N$; since $N$ is flat, one deduces from this an isomorphism $H.(x, M) \otimes_A N \to H.(x, M \otimes_A N)$ (X, p. 66, cor. 2), whence a).

The complex $K.(x)$ being flat, one has an exact sequence of complexes

$$
0 \to K.(x, M') \to K.(x, M) \to K.(x, M'') \to 0 ;
$$

assertion b) follows from the associated exact homology sequence.

#### Remark 2 {#alg-x-s9-n6-rem-2 .statement}

The analogous assertions to a) and b) for regular sequences are immediate.

#### Remark 3 {#alg-x-s9-n6-rem-3 .statement}

If the family $x$ is completely transverse for $A$, the complex $K.(x, A)$ defines a free resolution of the $A$-module $A/x$, with $x = \sum_{i \in I} x_i A$; therefore for every integer $i \geqslant 0$ and for every $A$-module $M$ there are isomorphisms

$$
\text{Ext}_A^{n-i}(A/x, M) \to H^{n-i}(x, M) \to H_i(x, M) \to \operatorname{Tor}_i^A(A/x, M) .
$$

#### Remark 4 {#alg-x-s9-n6-rem-4 .statement}

One says that the sequence $x = (x_1, ..., x_n)$ is $M$-coregular if (denoting by $(x_i)_M$ the homothety of ratio $x_i$ in $M$) the homothety of ratio $x_i$ in the module

$$
\operatorname{Ker}(x_1)_M \cap ... \cap \operatorname{Ker}(x_{i-1})_M
$$

is surjective for $i = 1, ..., n$. *One then has* $H_i(x, M) = 0$ for $i < n$: this is proved in the same way as prop. 5.

Take for example $A = k[D_1, ..., D_n]$, where $k$ is a $\mathbf{Q}$-algebra, and $M = k[T_1, ..., T_n]$, endowed with the $A$-module structure such that $D_i P = \partial P / \partial T_i$ for every $P \in M$ ($1 \leqslant i \leqslant n$). One verifies immediately that the sequence $(D_1, ..., D_n)$ is $M$-coregular; taking into account the example p. 155, one deduces that *the de Rham complex of* $k[T_1, ..., T_n]$ *over* $k$ *is acyclic in degrees* $> 0$.

### 7. A criterion for completely transverse sequences

Let $A$ be a ring, $M$ an $A$-module, $x$ an ideal of $A$. The *$x$-adic* *topology* on $M$ is defined to be the topology compatible with the group structure of $M$ for which the set of submodules $x^r M$ ($r \geqslant 0$) is a fundamental system of neighbourhoods of zero (TG, III, p. 5, example). This topology is separated if and only if

$$
\bigcap_{r \geqslant 0} x^r = 0 .
$$

Suppose now that the ideal $x$ is generated by a sequence $x = (x_1, ..., x_n)$ of elements of A. Consider the graded $A$-module $\bigoplus_{r \geq 0} x^r M$ and the graded $A$-homomorphism of degree 0

$$
a_M^x : A[X_1, ..., X_n] \otimes_A M \to \bigoplus_{r \geq 0} x^r M
$$

such that $a_M^x(P \otimes m) = P(x_1, ..., x_n) m$ if P is a homogeneous polynomial in $X_1, ..., X_n$ and $m \in M$. Let $\mathfrak{d}$ be the ideal of $A[X_1, ..., X_n]$ generated by the elements $(x_i X_j - x_j X_i)$ for $1 \leq i < j \leq n$. We have $P(x_1, ..., x_n) = 0$ if $P \in \mathfrak{d}$, so that $a_M^x$ gives by passing to the quotient an A-homomorphism graded of degree 0

$$
\alpha_M^x : (A[X_1, ..., X_n]/\mathfrak{d}) \otimes_A M \to \bigoplus_{r \geq 0} x^r M .
$$

By tensor product with $A/x$, we deduce from $\alpha_M^x$ an A-homomorphism graded of degree 0

$$
\beta_M^x : (A/x)[X_1, ..., X_n] \otimes_A M \to \bigoplus_{r \geq 0} (x^r M/x^{r+1} M) .
$$

The homomorphisms $a_M^x, \alpha_M^x$ and $\beta_M^x$ are surjective.

#### Theorem 1 {#alg-x-s9-thm-1 .statement}

Consider the following conditions:
(i) The sequence $x$ is M-regular (X, p. 158).
(ii) The sequence $x$ is completely secant for M (X, p. 157, def. 2).
(iii) One has $H_1(x, M) = 0$.
(iv) The homomorphism $\alpha_M^x : (A[X_1, ..., X_n]/\mathfrak{d}) \otimes_A M \to \bigoplus_{r \geq 0} x^r M$ is bijective.
(v) The homomorphism $\beta_M^x : (A/x)[X_1, ..., X_n] \otimes_A M \to \bigoplus_{r \geq 0} (x^r M/x^{r+1} M)$ is bijective.

Then one has the implications (i) $\Rightarrow$ (ii) $\Rightarrow$ (iii) $\Leftrightarrow$ (iv) $\Rightarrow$ (v). If for $1 \leq i \leq n$ the A-module $M/(x_1 M + \cdots + x_{i-1} M)$ is separated for the $x$-adic topology, the conditions (i) to (v) are equivalent.

The theorem will be proved in Nos 8 and 9.

*COROLLARY 1. — If A is noetherian, if the A-module M is of finite type and if the $x_i$ belong to the radical of A, the conditions (i) to (v) of the theorem are equivalent.
Indeed, on each of the modules $M/(x_1 M + \cdots + x_{i-1} M)$ the $x$-adic topology is separated (AC III, § 3, No. 3, prop. 6).

#### Corollary 2 {#alg-x-s9-thm-1-cor-2 .statement}

Suppose that A is a graded ring with positive degrees, M a bounded below graded A-module, and the $x_i$ homogeneous elements of degree > 0 of A. Then the conditions (i) to (v) of the theorem are equivalent.
The $x$-adic topology is indeed separated for every bounded below graded A-module N, since if $N_n = 0$ for $n < n_0$ one has $x^a N \subset \sum_{j \geq n_0 + a} N_j$ for all $a \geq 0$.

#### Corollary 3 {#alg-x-s9-thm-1-cor-3 .statement}

Suppose that the modules $M/(x_1M+\cdots+x_{i-1}M)$ are separated for the $\mathfrak{x}$-adic topology $(1\leq i\leq n)$ ; let p be an integer between $1$ and $n$. In order that the sequence $\mathfrak{x}$ be completely secant for $M$, it is necessary and sufficient that the sequence $(x_1,\ldots,x_p)$ be completely secant for $M$ and that the sequence $(x_{p+1},\ldots,x_n)$ be completely secant for $M/(x_1M+\cdots+x_pM)$.

Indeed the corollary is evident if in the statement one replaces “completely secant sequences” by “regular sequences”; but the two notions coincide here by the theorem.

#### Remark {#alg-x-s9-n7-rem-1 .statement}

Let $\mathfrak{x}=(x_1,\ldots,x_n)$ be a sequence of elements of $A$ such that $H_1(\mathfrak{x},A)=0$; then the kernel of the surjective homomorphism $u:A^n\to\mathfrak{x}$ such that
$$
u\left(\sum a_i e_i\right)=\sum a_i x_i
$$
is generated by the elements $X_j e_i-X_i e_j$; consequently, the $A$-algebra $A[X_1,\ldots,X_n]/\mathfrak{d}$ is isomorphic to the symmetric algebra $S_A(\mathfrak{x})$ (III, p. 69, prop. 4). It therefore follows from Theorem 1 that the algebra homomorphism
$$
S_A(\mathfrak{x})\longrightarrow\bigoplus_n \mathfrak{x}^n
$$
induced by the canonical injection of $\mathfrak{x}$ into $\bigoplus_n\mathfrak{x}^n$ is an isomorphism. The same holds for the homomorphism
$$
S_A(\mathfrak{x}/\mathfrak{x}^2)\longrightarrow\bigoplus_n\mathfrak{x}^n/\mathfrak{x}^{n+1}.
$$

### 8. Proof of Theorem 1: first part

The implication (i) $\Rightarrow$ (ii) has already been proved (X, p. 157, prop. 5). The implication (ii) $\Rightarrow$ (iii) is obvious; the same is true of (iv) $\Rightarrow$ (v), since $\beta_M^x$ is identified with $\alpha_M^x\otimes 1_{A/\mathfrak{x}}$.

To show that (iv) implies (iii), consider the homomorphism $(\alpha_M^x)_1$ induced on the components of degree 1. Let $E$ denote the graded $A$-module $A[X_1,\ldots,X_n]$; the $A$-module $E_1$ is free with basis $X_1,\ldots,X_n$ and $\mathfrak{d}_1$ is the sub-$A$-module of $E_1$ generated by the elements $(x_iX_j-x_jX_i)$ for $1\leq i<j\leq n$. Consequently $((E/\mathfrak{d})\otimes_A M)_1$ is identified with $K_1(\mathfrak{x},M)/B_1(K_\bullet(\mathfrak{x},M))$, the homomorphism $(\alpha_M^x)_1$ being identified with the mapping of $K_1(\mathfrak{x},M)/B_1(K_\bullet(\mathfrak{x},M))$ into $B_0(K_\bullet(\mathfrak{x},M))$ induced by $d_1$. Thus the vanishing of $H_1(\mathfrak{x},M)$ is equivalent to the injectivity of $(\alpha_M^x)_1$, whence the implication (iv) $\Rightarrow$ (iii).

To prove that (iii) implies (iv), we shall use the following lemma:

#### Lemma 4 {#alg-x-s9-lem-4 .statement}

Let $A_0$ be the ring $\mathbf{Z}[T_1,\ldots,T_n]$, and let $u:A_0[X_1,\ldots,X_n]\to A_0[U]$ be the homomorphism of $A_0$-algebras such that $u(X_i)=T_iU$. The kernel of $u$ is the ideal $\mathfrak{d}_0$ of $A_0[X_1,\ldots,X_n]$ generated by the elements $(T_iX_j-T_jX_i)$ for $1\leq i<j\leq n$. If $t$ is the ideal of $A_0$ generated by $(T_1,\ldots,T_n)$, $u$ induces an isomorphism
$$
\bar{u}:A_0[X_1,\ldots,X_n]/\mathfrak{d}_0\longrightarrow\bigoplus_{r\geq0}t^r.
$$

It is obviously enough to prove the first assertion. For every sequence of natural integers $\alpha=(\alpha_1,\ldots,\alpha_n)$ and every integer $k\in[0,n]$, let $P_{\alpha,k}$ denote the monomial
$$
T_1^{\alpha_1}\cdots T_k^{\alpha_k}X_{k+1}^{\alpha_{k+1}}\cdots X_n^{\alpha_n};
$$

let $N$ be the sub-$\mathbf{Z}$-module of $A_0[X_1, ..., X_n]$ generated by the $P_{\alpha, k}$ for $\alpha \in \mathbf{N}^n$ and $0 \leq k \leq n$. We shall prove that the restriction of $u$ to $N$ is injective and that $A_0[X_1, ..., X_n] = \mathfrak{d}_0 + N$; since we have $\mathfrak{d}_0 \subset \mathrm{Ker}\,u$, this will entail the lemma.

Observe that $N$ is generated by the set $S$ formed by $P_{0,0} = 1$ and by those of the $P_{\alpha, k}$ for which $\alpha_k \neq 0$. To prove the injectivity of the restriction of $u$ to $N$, it suffices to show that two distinct elements of $S$ have as their images by $u$ distinct monomials in $A_0[U]$. Now we have $u(P_{\alpha, k}) = T^\alpha U^{\sum \alpha_i}_{i \geq k}$, so that the equality $u(P_{\alpha, k}) = u(P_{\alpha', k'})$ entails $\alpha = \alpha'$ and $\sum_{i \geq k} \alpha_i = \sum_{i \geq k'} \alpha_i$. Suppose that $P_{\alpha, k}$ and $P_{\alpha', k'}$ belong to $S$. If $\alpha = 0$, then we have $k = k' = 0$; if $\alpha \neq 0$, we obtain $k = k'$ since $\alpha_k$ and $\alpha_{k'}$ are different from zero, whence the result.

Show that every monomial $T^\alpha X^\beta \in A_0[X_1, ..., X_n]$ is congruent modulo $\mathfrak{d}_0$ to a $P_{\eta, k}$. For every sequence $\lambda \in \mathbf{N}^n$, we shall denote by $i(\lambda)$ (resp. $j(\lambda)$) the smallest (resp. the largest) integer $k \in [1, n]$ such that $\lambda_k \neq 0$. Among the monomials $T^\gamma X^\delta$ which are congruent to $T^\alpha X^\beta$ modulo $\mathfrak{d}_0$, choose one for which the rational integer $j(\gamma) - i(\delta)$ is minimal; let us show that we then have $j(\gamma) - i(\delta) < 0$. Suppose that we have $j(\gamma) \geq i(\delta)$; put $j = j(\gamma), i = i(\delta)$, and let $\varepsilon = \inf (\gamma_j, \delta_i)$. Since $(T_j^\varepsilon X_i^\varepsilon - T_i^\varepsilon X_j^\varepsilon)$ is divisible by $(T_j X_i - T_i X_j)$, and therefore belongs to $\mathfrak{d}_0$, we see that $T^\gamma X^\delta$ is congruent modulo $\mathfrak{d}_0$ to $T^{\gamma'} X^{\delta'}$, where $\gamma'_i = \gamma_i + \varepsilon, \gamma'_j = \gamma_j - \varepsilon, \gamma'_k = \gamma_k$ for $k \neq i, j$, and $\delta'_i = \delta_i - \varepsilon, \delta'_j = \delta_j + \varepsilon, \delta'_k = \delta_k$ for $k \neq i, j$. Since $\gamma'_j$ or $\delta'_i$ is zero, we have $j(\gamma') - i(\delta') < j(\gamma) - i(\delta)$ which contradicts the minimal character of $j(\gamma) - i(\delta)$.

Consequently we have $j(\gamma) < i(\delta)$, whence $T^\gamma X^\delta \in N$, which completes the proof of the lemma.

Let us prove that (iii) implies (iv). Consider the ring $A_0 = \mathbf{Z}[T_1, ..., T_n]$ and the ideal t of $A_0$ generated by $T_1, ..., T_n$. Endow $M$ with the structure of $A_0$-module for which $T_i m = x_i m$ for $m \in M, 1 \leq i \leq n$. According to X, p. 155, $H_i(x, M)$ is identified canonically with $H_i(T, M)$.

Since the sequence $T$ is regular for $A_0$, it follows from the implication (i) $\Rightarrow$ (ii) that the complex $K.(T, A_0)$ defines a free resolution of the $A_0$-module $A_0/t$. Let us remark that the latter is identified with $\mathbf{Z}$, endowed with the structure of $A_0$-module such that $T_i \mathbf{Z} = 0$ for $1 \leq i \leq n$. Thus the condition (iii) is equivalent to $\mathrm{Tor}_1^{A_0}(M, \mathbf{Z}) = 0$.

Let us show that (iii) implies $\mathrm{Tor}_1^{A_0}(M, A_0/t^r) = 0$ for all $r \geq 1$. This results from what precedes for $r = 1$. In the general case, consider the exact sequence

$$
0 \to t^r/t^{r+1} \to A_0/t^{r+1} \to A_0/t^r \to 0,
$$

The $A_0$-module $t^r/t^{r+1}$ is isomorphic to a finite product of copies of $\mathbf{Z}$; we therefore have $\mathrm{Tor}_1^{A_0}(M, t^r/t^{r+1}) = 0$. It follows, by induction on $r$, that

$$
\mathrm{Tor}_1^{A_0}(M, A_0/t^r) = 0 \quad \text{for all } r,
$$

The exact sequence (16) therefore provides, by tensor product with $M$, an exact sequence

$$
0 \to (t^r/t^{r+1}) \otimes_{A_0} M \to M/x^{r+1} M \to M/x^r M \to 0
$$

whence an isomorphism of $(t'/{t'}^{r+1}) \otimes_{A_0} M$ onto $x' M/{x'}^{r+1} M$. By considering the exact sequence $0 \to {t'}^{r+1} \to t' \to t'/{t'}^{r+1} \to 0$, one then sees by induction on $r$ that the mapping $m_r : t' \otimes_{A_0} M \to x' M$, induced by the operation of $A_0$ in $M$, is an isomorphism.

To prove (iv), it remains to observe that the diagram

$$
\begin{array}{ccc}
(A_0[X_1, ..., X_n]/\mathcal{D}_0) \otimes_{A_0} M & \xrightarrow{\bar{u} \otimes 1_M} & \bigoplus_{r \geq 0} (t' \otimes_{A_0} M) \\
\downarrow e & & \downarrow \oplus m_r \\
(A[X_1, ..., X_n]/\mathcal{D}) \otimes_A M & \xrightarrow{\alpha_M^x} & \bigoplus_{r \geq 0} x' M
\end{array}
$$

where $e$ is the canonical isomorphism of extension of scalars (II, p. 85, prop. 6), is commutative, and to apply Lemma 4.

### 9. Proof of Theorem 1: second part

Let us again consider the exact sequence

(16)
$$
0 \longrightarrow t'/{t'}^{r+1} \xrightarrow{i_r} A_0/{t'}^{r+1} \xrightarrow{p_r} A_0/t' \longrightarrow 0
$$

and the associated exact sequence of torsion modules

(18)
$$
\begin{array}{cccccc}
\mathrm{Tor}_1^{A_0}(A_0/{t'}^{r+1}, M) & \longrightarrow & \mathrm{Tor}_1^{A_0}(A_0/t', M) \\
\longrightarrow (t'/{t'}^{r+1}) \otimes_{A_0} M & \xrightarrow{i_r \otimes 1_M} & (A_0/{t'}^{r+1}) \otimes_{A_0} M & \xrightarrow{p_r \otimes 1_M} & (A_0/t') \otimes_{A_0} M & \longrightarrow 0 .
\end{array}
$$

The kernel of $p_r \otimes 1_M$ is identified with $x' M/{x'}^{r+1} M$; moreover $t'/{t'}^{r+1}$ is annihilated by the $T_i$ and is identified with the homogeneous component of degree $r$ of $A_0$, so that the homomorphism $(t'/{t'}^{r+1}) \otimes_{A_0} M \to x' M/{x'}^{r+1} M$ deduced from $i_r \otimes 1_M$ is identified with the homogeneous component of degree $r$ of the homomorphism $\beta_M^x$. It follows therefore from the exact sequence (18) that condition (v) is equivalent to

(v') : *the homomorphism* $\mathrm{Tor}_1^{A_0}(p_r, 1_M)$ : $\mathrm{Tor}_1^{A_0}(A_0/{t'}^{r+1}, M) \to \mathrm{Tor}_1^{A_0}(A_0/t', M)$ *is surjective for all* $r \geq 1$.

It remains for us to prove the implication (v) $\Rightarrow$ (i) when the modules
$$
M/(x_1 M + \cdots + x_{i-1} M)
$$
are separated for the $x$-adic topology ($1 \leq i \leq n$). Let $\overline{M}$ denote the $A$-module $M/x_1 M$. By definition, the sequence $x$ is regular for $M$ if and only if $(x_1)_M$ is injective and the sequence $x' = (x_2, ..., x_n)$ is regular for $\overline{M}$. Reasoning by induction on $n$, it therefore suffices to prove that, if $M$ is separated for the $x$-adic topology and if $\beta_M^x$ is bijective, then $(x_1)_M$ is injective and $\beta_M^{x'}$ is bijective. Now the bijectivity of $\beta_M^x$ implies in particular that the homothety with ratio $x_1$ in $\bigoplus r x' M/{x'}^{r+1} M$ is injective, hence that $\mathrm{Ker}\,(x_1)_M \subset \bigcap_i x^i M$ and consequently that $(x_1)_M$ is injective if the $x$-adic topology on $M$ is separated.

We are thus reduced to proving that if $(x_1)_M$ is injective and if $M$ satisfies condition (v'), then $\overline{M}$ satisfies condition (v') relative to the sequence $x'$.

By assumption, we have an exact sequence
$$
0 \longrightarrow M \xrightarrow{(x_1)_M} M \longrightarrow \overline{M} \longrightarrow 0;
$$
let $\overline{A}_0 = A_0 / T_1 A_0,\ \overline{t} = t \overline{A}_0$. Let $q : L \to M$ be a free resolution of the $A_0$-module $M$; since the homothety with ratio $T_1$ is injective in $A_0$, it is injective in $L$, and we have an exact sequence of complexes
$$
0 \longrightarrow L \xrightarrow{(x_1)_L} L \longrightarrow \overline{L} \longrightarrow 0
$$
with $\overline{L} = L / x_1 L$, and a commutative diagram
$$
\begin{array}{ccc}
0 & \longrightarrow & L \xrightarrow{(x_1)_L} L \longrightarrow \overline{L} \longrightarrow 0 \\
   &                & \downarrow q        \downarrow q        \downarrow \overline{q} \\
0 & \longrightarrow & M \xrightarrow{(x_1)_M} M \longrightarrow \overline{M} \longrightarrow 0 .
\end{array}
$$

Since $q$ is a homomorphism of complexes inducing isomorphisms in homology, $\overline{q} : \overline{L} \to \overline{M}$ is a free resolution of the $\overline{A}_0$-module $\overline{M}$ (cor. 1, p. 30). For every $\overline{A}_0$-module $P$, there is a canonical isomorphism
$$
P \otimes_{A_0} L \to P \otimes_{\overline{A}_0} \overline{L},
$$
whence by passing to homology an isomorphism
$$
\varphi_P : \mathrm{Tor}_1^{A_0}(P, M) \to \mathrm{Tor}_1^{\overline{A}_0}(P, \overline{M}) .
$$
If $u : P \to P'$ is a $\overline{A}$-homomorphism, then
$$
\varphi_{P'} \circ \mathrm{Tor}_1^{A_0}(u, 1_M) = \mathrm{Tor}_1^{\overline{A}_0}(u, 1_M) \circ \varphi_P .
$$
That being so, suppose that condition (v') is satisfied for $M$, and let us prove that it is true for $\overline{M}$. Let $r$ be an integer $\geqslant 1$; we have a commutative diagram with exact rows
$$
\begin{array}{ccccccccc}
0 & \longrightarrow & A_0 / t^r & \xrightarrow{T_1} & A_0 / t^{r+1} & \longrightarrow & \overline{A}_0 / \overline{t}^{r+1} & \longrightarrow & 0 \\
   &                  & \downarrow p_{r-1} &           & \downarrow p_r &           & \downarrow \overline{p}_r &           & \\
0 & \longrightarrow & A_0 / t^{r-1} & \xrightarrow{T_1} & A_0 / t^r & \longrightarrow & \overline{A}_0 / \overline{t}^r & \longrightarrow & 0
\end{array}
$$
from which one deduces a commutative diagram with exact rows
$$
\begin{array}{ccccccccccc}
\mathrm{Tor}_1^{A_0}(A_0 / t^{r+1}, M) & \longrightarrow & \mathrm{Tor}_1^{A_0}(\overline{A}_0 / \overline{t}^{r+1}, M) & \longrightarrow & M / x^r M & \xrightarrow{x_1} & M / x^{r+1} M \\
\mathrm{Tor}_1(p_{r, r'}) & \downarrow & \mathrm{Tor}_1(\overline{p}_{r, 1}) & \downarrow & & & \downarrow \\
\mathrm{Tor}_1(A_0 / t^r, M) & \longrightarrow & \mathrm{Tor}_1^{A_0}(\overline{A}_0 / \overline{t}^r, M) & \longrightarrow & M / x^{r-1} M & \xrightarrow{x_1} & M / x^r M .
\end{array}
$$
Now multiplication by $x_1$ defines an injection of $M / x^r M$ into $M / x^{r+1} M$: this follows immediately, by induction on $r$, from the exact sequence
$$
0 \to x^{r-1} M / x^r M \to M / x^r M \to M / x^{r-1} M \to 0
$$

and from the injectivity of the homothety with ratio $x_1$ in $\bigoplus_{r \geq 0} (x^r M / x^{r+1} M)$. Condition (v) therefore implies that the homomorphism $\operatorname{Tor}_{1}^{\overline{A}_0} (\overline{p}_r, 1_M)$ is surjective for every $r \geq 1$. By composition with the isomorphisms $(\varphi_{\overline{A}_0/\overline{t}^{r+1}})^{-1}$ and $\varphi_{\overline{A}_0/\overline{t}^r}$, one deduces that the homomorphism

$$
\operatorname{Tor}_{1}^{\overline{A}_0} (\overline{p}_r, 1_M) : \operatorname{Tor}_{1}^{\overline{A}_0} (\overline{A}_0 / \overline{t}^{r+1}, M) \to \operatorname{Tor}_{1}^{\overline{A}_0} (\overline{A}_0 / \overline{t}^r, M)
$$

is surjective for $r \geq 1$, whence condition (v') for $\overline{M}$. This completes the proof of the theorem.

### 10. Class of extensions associated with a regular sequence

Let $A$ be a ring, $M$ an $A$-module, $x = (x_1, ..., x_n)$ a sequence of elements of $A$. Let $M_i$ denote the $A$-module $M / (x_1 M + \cdots + x_{i-1} M)$ for $i = 0, ..., n+1$, so that $M_0$ and $M_1$ are identified with $M$ and that $M_{n+1} = M / (x) M$. Let

$$
\overline{x}_i : M_{i-1} \to M_i , \quad i = 1, ..., n ,
$$

the $A$-homomorphism composed of the homothety of $M_{i-1}$ with ratio $x_i$ and of the canonical projection of $M_{i-1}$ onto $M_i$. Finally, let us denote by $p : M_n \to M / (x) M$ the canonical projection. The diagram

(19)

$$
0 \longrightarrow M \xrightarrow{\overline{x}_1} M_1 \xrightarrow{\overline{x}_2} M_2 \longrightarrow \cdots \xrightarrow{\overline{x}_n} M_n \xrightarrow{p} M / (x) M \longrightarrow 0
$$

is an exact sequence if and only if the sequence $x$ is $M$-regular. Henceforth suppose that the sequence $x$ is regular for $M$. The element $\theta_x \in \operatorname{Ext}_A^n (M / (x) M, M)$ associated with the exact sequence (19) is also said to be associated with the $M$-regular sequence $x$.

Let $i$ be an integer, $1 \leq i \leq n$. Note that the sequence (19) can be decomposed into the two exact sequences

(20)

$$
0 \longrightarrow M \xrightarrow{\overline{x}_1} M_1 \xrightarrow{\overline{x}_2} M_2 \longrightarrow \cdots \xrightarrow{\overline{x}_i} M_i \longrightarrow M / (x_1 M + \cdots + x_i M) \longrightarrow 0
$$

(21)

$$
0 \longrightarrow M / (x_1 M + \cdots + x_i M) \xrightarrow{\overline{x}_{i+1}} M_{i+1} \longrightarrow \cdots \longrightarrow M_n \xrightarrow{p} M / (x) M \longrightarrow 0
$$

which are none other than the exact sequences associated with the sequence $(x_1, ..., x_i)$, which is regular for $M$, and with the sequence $(x_{i+1}, ..., x_n)$, which is regular for $M / (x_1 M + \cdots + x_i M)$. Denoting by

$$
\theta_{(x_1, ..., x_i)} \in \operatorname{Ext}_A^i (M / (x_1 M + \cdots + x_i M), M)
$$
$$
\theta_{(x_{i+1}, ..., x_n)} \in \operatorname{Ext}_A^{n-i} (M / (x) M, M / (x_1 M + \cdots + x_i M)) ,
$$

the extension classes associated with (20) and (21), one has, by X, p. 118, prop. 3,

(22)
$$
\theta_{(x_1, \ldots, x_n)} = \theta_{(x_1, \ldots, x_i)} \circ \theta_{(x_{i+1}, \ldots, x_n)} .
$$

Moreover, by prop. 5 (X, p. 157), the Koszul complex $\mathbf{K}.(x, M)$ is acyclic in degrees $\neq n$, whence an exact sequence

(23)
$$
0 \longrightarrow M \xrightarrow{\partial^0} \mathbf{K}^1(x, M) \xrightarrow{\partial^1} \mathbf{K}^2(x, M) \xrightarrow{\partial^2} \cdots \longrightarrow \mathbf{K}^n(x, M) \xrightarrow{q} M/(x)M \longrightarrow 0 ,
$$
where $\mathbf{K}^0(x, M)$ has been identified with $M$ and where $q$ maps each element $m \in \mathbf{K}^n(x, M)$ to the class in $M/(x)M$ of $m(1, 2, \ldots, n) \in M$.

#### Proposition 8 {#alg-x-s9-prop-8 .statement}

*Suppose the sequence x is regular for M. The element of $\mathrm{Ext}_A^n(M/(x)M, M)$ associated with the exact sequence (23) is $(-1)^{n(n+1)/2} \theta_x$.*
For $i = 0, 1, \ldots, n$, define an A-linear mapping
$$
a^i : \mathbf{K}^i(x, M) \to M_i = M/(x_1 M + \cdots + x_{i-1} M)
$$
as follows: if $m \in \mathbf{K}^i(x, M)$, $a^i(m)$ is the class in $M_i$ of the element $m(1, 2, \ldots, i)$ of $M$. It is clear that $a^0$ is the identity mapping of $M$ and that $p \circ a^n = q$. Moreover $a^{i+1} \circ \partial^i(m)$ is the image in $M_{i+1}$ of the element
$$
\sum_{k=1}^{i+1} (-1)^{k+1} x_k m(1, 2, \ldots, k-1, k+1, \ldots, i+1) .
$$
Since $x_k$ annihilates $M_{i+1}$ for $k = 1, \ldots, i$, $a^{i+1} \circ \partial^i(m)$ is also the image of
$$
(-1)^i x_{i+1} m(1, 2, \ldots, i) ,
$$
hence
$$
a^{i+1} \circ \partial^i = (-1)^i \overline{x}_{i+1} \circ a^i .
$$
By X, p. 120, cor. 1 and 2, the element of $\mathrm{Ext}_A^n(M/(x)M, M)$ associated with (23) is equal to $\prod_{i=1}^n (-1)^i \cdot \theta_x$, whence the assertion.

#### Corollary {#alg-x-s9-n10-cor-1 .statement}

*Suppose moreover that the modules $M/(x_1 M + \cdots + x_{i-1} M)$ are separated for the (x)-adic topology, and let $(a_{ij}) \in \mathrm{GL}_n(A)$. Put*
$$
y_i = \sum_j a_{ij} x_j \quad \text{and} \quad y = (y_1, \ldots, y_n) .
$$
*Then the sequence y is regular for M, and one has $\theta_y = \det(a_{ij})^{-1} \theta_x$.*
Indeed, the sequence y is regular for M by Prop. 6 (X, p. 158) and Theorem 1 (X, p. 160); the last assertion follows from Prop. 8, and from Prop. 4 of X, p. 119.

#### Proposition 9 {#alg-x-s9-prop-9 .statement}

*Suppose the sequence x regular for M. If N is an A-module such that $(x)N = 0$, one has $\mathrm{Ext}_A^i(N, M) = 0$ for $i < n$, and the mapping $\alpha \mapsto \theta_x \circ \alpha$* from Hom_A (N, M/(x) M) into Ext^n_A (N, M) (which is also the iterated connecting homomorphism associated with (19), cf. X, p. 127, Corollary 3) is bijective.

It remains to prove that the homomorphism $\psi^i : \alpha \mapsto \theta_x \circ \alpha$ from $\mathrm{Ext}_A^{i-n}(N, M/(x) M)$ into $\mathrm{Ext}_A^i(N, M)$ is bijective for $i \leq n$. Let us reason by induction on $n$, the assertion being trivial for $n = 0$. Put $M_1 = M/x_1 M$, $x' = (x_2, ..., x_n)$, so that $x'$ is $M_1$-regular. By the induction hypothesis, the homomorphism

$$
\overline{\psi}^{i-1} : \alpha \mapsto \theta_{x'} \circ \alpha
$$

from $\mathrm{Ext}_A^{i-n}(N, M/(x) M)$ into $\mathrm{Ext}_A^{i-1}(N, M_1)$ is bijective for $i < n$. On the other hand, consider the exact sequence

$$
0 \longrightarrow M \xrightarrow{(x_1)_M} M \longrightarrow M_1 \longrightarrow 0 ;
$$

the connecting homomorphism $\mathrm{Ext}_A^i(N, M_1) \to \mathrm{Ext}_A^{i+1}(N, M)$ associated with it is $\varphi^i : \beta \mapsto \theta_{x_1} \circ \beta$ (X, p. 125, Prop. 5) ;

since one has $\mathrm{Ext}^i(1_N, (x_1)_M) = \mathrm{Ext}^i((x_1)_N, 1_M) = 0$, one deduces from this exact sequences

$$
0 \longrightarrow \mathrm{Ext}_A^i(N, M) \longrightarrow \mathrm{Ext}_A^i(N, M_1) \xrightarrow{\varphi^i} \mathrm{Ext}_A^{i+1}(N, M) \longrightarrow 0 .
$$

Since $\mathrm{Ext}_A^i(N, M_1) = 0$ for $i < n - 1$, it follows that $\mathrm{Ext}_A^{i+1}(N, M) = 0$ for $i < n - 1$, that is to say for $i + 1 < n$; it follows that $\varphi^i$ is bijective for $i < n$. Since $\psi^i(\alpha) = \theta_x \circ \alpha = \theta_{x_1} \circ \theta_{x'} \circ \alpha = \varphi^{i-1} \circ \overline{\psi}^i(\alpha)$ for $\alpha \in \mathrm{Ext}_A^{i-n}(N, M/(x) M)$, $\psi^i$ is indeed bijective for $i \leq n$.

EXERCISES

## EXERCISES {#alg-x-s9-exercises}

See the [exercises for § 9](exercises/s9/).
