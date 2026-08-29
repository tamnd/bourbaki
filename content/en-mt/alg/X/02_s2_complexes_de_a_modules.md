---
book: alg
book_title: Algebra
chapter: X
chapter_title: ALGÈBRE HOMOLOGIQUE
section: 2
section_title: Complexes de A-modules
lang: en
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
statements: 56
exercises: 18
content_sha256: 861a391434771556fa8eb6b95600862c1fab35a9ef0810851b123295d669544a
translated_from: content/fr/alg/X/02_s2_complexes_de_a_modules.md
source_lang: fr
translation_method: machine
source_content_sha256: e39dbf624efa7299900b2ff6aa5b6b432df163fe6dd11f43a39e7879f80cefb3
translation_model: gpt-5-mini, hy3-free, nemotron-3-ultra-free, laguna-s-2.1-free, gpt-5-6
translation_run: translate-en-mt-33bc941f
glossary_version: 34
glossary_terms_sha256: 105b6b8d5fe35d922dcc81d919bbefb638092f6e71ef47c7aa5a5c6a49b81208
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 2. COMPLEXES OF a-MODULES

*In this paragraph, $A$ denotes a ring. When we speak of $A$-modules without further specification, it will always be a question of left $A$-modules.*

*We shall call graded modules the graded modules of type $\mathbf{Z}$ (II, p. 164).*

*If $M$ is a graded $A$-module, of grading $(M_n)_{n\in\mathbf{Z}}$, we put $M^n=M_{-n}$ and say that $M_n$ (resp. $M^n$) is the homogeneous component of descending degree $n$ (resp. of ascending degree $n$) of $M$. If $u:M\to N$ is a graded homomorphism of degree $p$ of graded $A$-modules (II, p. 166), we denote by $u_n:M_n\to M_{n+p}$ (resp. $u^n:M^n\to M^{n-p}$) the homomorphism deduced from $u$; it is called the homogeneous component of descending degree (resp. ascending degree) $n$ of $u$; one also says that $u$ is of descending degree $p$ or of ascending degree $-p$.*

### 1. Complexes of a-Modules

#### Definition 1 {#alg-x-s2-def-1 .statement}

*A differential complex of $A$-modules is a pair $(C,d)$ formed by a graded $A$-module $C$ and an endomorphism $d:C\to C$ graded of descending degree $-1$ and such that $d\circ d=0$.*

It is also called a complex of $A$-modules, or an $A$-complex, or a complex. One often writes C in place of (C, d); the endomorphism d is called the differential of the complex (C, d), or by abuse of language of C.

If C_n (resp. C^n) is the homogeneous component of descending degree (resp. ascending degree) n of C, the datum of d is equivalent to that of the sequence of homomorphisms

(1)
$$
\cdots \longrightarrow C_{n+1} \xrightarrow{d_{n+1}} C_n \xrightarrow{d_n} C_{n-1} \longrightarrow \cdots
$$
resp.

(1')
$$
\cdots \longrightarrow C^{n-1} \xrightarrow{d^{n-1}} C^n \xrightarrow{d^n} C^{n+1} \longrightarrow \cdots
$$
such that $d_n \circ d_{n+1} = 0$ for all $n \in \mathbf{Z}$ (resp. $d^n \circ d^{n-1} = 0$ for all $n \in \mathbf{Z}$). By abuse of language, one will also call a complex the datum of such a sequence of $A$-modules and homomorphisms.

One will remark, as a mnemonic device, that when one “follows the direction of the arrows” in the diagrams (1) and (1’), the descending degree decreases and the ascending degree increases.

Every graded $A$-module will tacitly be considered as a complex by endowing it with the zero differential; the complexes thus obtained will be called complexes with zero differential. In particular, every $A$-module M will be endowed with the unique structure of $A$-complex such that $M_0 = M^0 = M$. The complex (C, d) is said to be zero if C is reduced to 0. In the sequel, we denote by 0 a zero complex, chosen once and for all.

Adjoin to the ordered set $\mathbf{Z}$ two elements denoted $-\infty$ and $+\infty$; denote by $\overline{\mathbf{Z}}$ the set obtained, and endow it with the order relation extending that of $\mathbf{Z}$ and such that $-\infty < n < +\infty$ for all $n \in \mathbf{Z}$; every subset of $\overline{\mathbf{Z}}$ possesses a greatest lower bound and a greatest upper bound.

Let C be a complex; one calls the right and left bounds $^1$ of C the elements $b_d(C)$ and $b_g(C)$ of $\overline{\mathbf{Z}}$ defined by
$$
b_d(C) = \inf \{ n \in \mathbf{Z}, C_n \neq 0 \}, \quad b_g(C) = \sup \{ n \in \mathbf{Z}, C_n \neq 0 \}.
$$
One says that C is zero on the right if $b_d(C) \geqslant 0$, bounded on the right if $b_d(C) \neq -\infty$, zero on the left if $b_g(C) \leqslant 0$, bounded on the left if $b_g(C) \neq +\infty$; one says that C is bounded if
$$
b_d(C) \neq -\infty, \quad b_g(C) \neq +\infty.
$$
One calls the length $^2$ of C and denotes by $l(C)$ the element of $\overline{\mathbf{Z}}$ defined as follows: if C is zero, $l(C) = -\infty$; if C is bounded and nonzero $l(C) = b_g(C) - b_d(C)$; if C

$^1$ The words right and left are relative to the description of C by means of the diagrams (1) and (1’).
$^2$ One must not confuse the notion of length of the complex (C, d) with that of length of the module C (II, p. 21).

is not bounded, $l(C) = + \infty$. \* With the conventions of TG, IV, p. 13-17, one always has $l(C) = b_g(C) - b_d(C)$. \*

For example, if $k$ consecutive components of $C$ are non-zero, the others being zero, one has $l(C) = k - 1$ if $k > 0$, $l(C) = - \infty$ if $k = 0$.

One says that the complex $(C, d)$ is free, projective, flat, injective, if each of the modules $C_n$ is so. It will be noted that the complex $(C, d)$ is projective or flat if and only if the module $C$ is so (II, p. 39, prop. 3 and X, p. 8, prop. 4), but that $C$ can be free without the complex $(C, d)$ being so (since a direct factor of a free module is not always free), analogously $(C, d)$ can be injective without $C$ being so (X, p. 170, exercise 21).

Let $(C, d)$ be a complex. Put $Z(C, d) = \mathrm{Ker}\,(d)$, $B(C, d) = \mathrm{Im}\,(d)$; these are graded submodules of $C$, called respectively the module of cycles and the module of boundaries of $(C, d)$; the homogeneous components of $Z(C, d)$ and $B(C, d)$ are denoted $Z_n(C, d) = Z^{-n}(C, d)$, $B_n(C, d) = B^{-n}(C, d)$; one has $Z_n(C, d) = \mathrm{Ker}\,(d_n)$, $B_n(C, d) = \mathrm{Im}\,(d_{n+1})$, $Z^n(C, d) = \mathrm{Ker}\,(d^n)$, $B^n(C, d) = \mathrm{Im}\,(d^{n-1})$.

Since $d \circ d = 0$, one has $B(C) \subset Z(C)$; two cycles are said to be homologous if their difference is a boundary; the graded quotient module $H(C, d) = Z(C, d)/B(C, d)$ is called the homology module of $(C, d)$; its elements are the homology classes; its homogeneous components are denoted $H_n(C, d) = H^{-n}(C, d)$.

#### Example {#alg-x-s2-n1-exa-1 .statement}

If $C$ has zero differential, one has $Z(C) = C$, $B(C) = 0$ and $H(C)$ identifies canonically with $C$.

There are exact sequences, called canonical:

(I$_n$) $$ 0 \to Z_n(C) \to C_n \xrightarrow{\delta_n} B_{n-1}(C) \to 0 $$
(II$_n$) $$ 0 \to B_n(C) \to Z_n(C) \to H_n(C) \to 0 $$
(III$_n$) $$ 0 \to B_n(C) \to C_n \to C_n/B_n(C) \to 0 $$
(IV$_n$) $$ 0 \to H_n(C) \to C_n/B_n(C) \xrightarrow{\overline{\delta}_n} B_{n-1}(C) \to 0 $$

where $\delta_n$ and $\overline{\delta}_n$ are deduced from $d_n$. By combining (IV$_n$) and (II$_{n-1}$), one obtains the exact sequence

(V$_n$) $$ 0 \to H_n(C) \to C_n/B_n(C) \to Z_{n-1}(C) \to H_{n-1}(C) \to 0 , $$

which is also written, changing $n$ into $-n$

(V$^n$) $$ 0 \to H^n(C) \to C^n/B^n(C) \to Z^{n+1}(C) \to H^{n+1}(C) \to 0 . $$

#### Definition 2 {#alg-x-s2-def-2 .statement}

Let $(C, d)$ and $(C', d')$ be two complexes. A morphism $^1$ from $(C, d)$ to $(C', d')$ is a graded A-homomorphism $u$ of degree 0 from $C$ to $C'$ such that
$$
d' \circ u = u \circ d .
$$

¹ Or morphism of degree 0 (cf. X, p. 81).

For every $n$, we therefore have $d'_n \circ u_n = u_{n-1} \circ d_n$ and ${d''}^n \circ u^n = u^{n+1} \circ d^n$. We have
$$
u(Z(C)) \subset Z(C') , \quad u(B(C)) \subset B(C') ,
$$
and we denote by $Z(u) : Z(C) \to Z(C')$, $B(u) : B(C) \to B(C')$, $H(u) : H(C) \to H(C')$ the homomorphisms of A-modules deduced from this; the homogeneous components of these morphisms are denoted $Z_n(u)$, $Z^n(u)$, ...

If $v$ is another morphism from $(C, d)$ to $(C', d')$, then $u + v$ is a morphism from $(C, d)$ to $(C', d')$, and we have
$$
Z(u + v) = Z(u) + Z(v) , \quad B(u + v) = B(u) + B(v) , \quad H(u + v) = H(u) + H(v) .
$$
Analogously, if $A$ is an algebra over a commutative ring $k$, and if $\lambda \in k$, then $\lambda u$ is a morphism from $(C, d)$ to $(C', d')$ and we have
$$
Z(\lambda u) = \lambda Z(u) , \quad B(\lambda u) = \lambda B(u) , \quad H(\lambda u) = \lambda H(u) .
$$
If $u' : (C', d') \to (C'', d'')$ is another morphism of complexes, then $u' \circ u$ is a morphism from $(C, d)$ to $(C'', d'')$ and we have
$$
Z(u' \circ u) = Z(u') \circ Z(u) , \quad B(u' \circ u) = B(u') \circ B(u) , \quad H(u' \circ u) = H(u') \circ H(u) .
$$
It is clear that a bijective morphism is an isomorphism.

#### Definition 3 {#alg-x-s2-def-3 .statement}

Let $(C, d)$ and $(C', d')$ be two complexes. A homological isomorphism (or quasi-isomorphism) from $(C, d)$ to $(C', d')$ is a morphism $u$ from $(C, d)$ to $(C', d')$ such that $H(u)$ is bijective.

Every isomorphism is a homological isomorphism, every morphism composed of homological isomorphisms is a homological isomorphism.

We say that $(C, d)$ is of null homology if $H(C) = 0$, that is to say if the unique morphism of complexes $0 \to C$ (resp. $C \to 0$) is a homological isomorphism. We say that $(C, d)$ is acyclic in descending degree $n$ (resp. in ascending degree $n$) if $H_n(C) = 0$ (resp. $H^n(C) = 0$).

Let $(C, d)$ be a complex and $p \in \mathbf{Z}$. The $p$-th translate of $(C, d)$ is the complex $(C(p), d(p))$ obtained as follows: $C(p)$ is the a-module obtained by shifting the grading of $C$ by $p$ (II, p. 163; Example 3), so that
$$
C(p)_n = C_{n+p} , \quad C(p)^n = C^{n-p} ;
$$
in particular $C(p)_0 = C_p$; note also that $C$ is the direct sum of its graded submodules $C_p(-p)$, $p \in \mathbf{Z}$ (resp. $C^p(p)$, $p \in \mathbf{Z}$). We set $d(p) = (-1)^p d$.
We have $Z(C(p)) = Z(C)(p)$, $B(C(p)) = B(C)(p)$ and $H(C(p)) = H(C)(p)$.

For example, $d$ is a morphism of complexes from $C$ to $C(-1)$ and
$$
H(d) : H(C) \to H(C)(-1)
$$
is zero.

For every morphism of complexes $u : (C,d) \to (C',d')$, and every $p \in \mathbf{Z}$, $u$ is also a morphism from $(C(p),d(p))$ to $(C'(p),d'(p))$; it is sometimes denoted $u(p)$ and we have
$$
u(p)_n = u_{n+p}, \qquad u(p)^n = u^{n-p}.
$$

### 2. Operations on complexes

On the set $A \times A$, the two laws
$$
(a,b) + (a',b') = (a+a',b+b')
$$
$$
(a,b)(a',b') = (aa',ab'+ba')
$$
define a ring structure, denoted $A(\varepsilon)$, with unit element $1=(1,0)$; the injection $a \mapsto (a,0)=a1$ allows us to identify $A$ with a subring of $A(\varepsilon)$; the module $A(\varepsilon)$ is free with basis $\{1,\varepsilon\}$ where $\varepsilon=(0,1)$; we have $\varepsilon^2=0$ and $\varepsilon$ is central in $A(\varepsilon)$.

When $A$ is commutative, $A(\varepsilon)$ is an algebra of dual numbers over $A$ (III, p. 15).

Let us equip $A(\varepsilon)$ with the ring grading (II, p. 164) for which $A(\varepsilon)_0 = A\mathbin{.}1$, $A(\varepsilon)_{-1} = A\mathbin{.}\varepsilon$, and $A(\varepsilon)_n = 0$ for $n \neq 0, -1$. It is clear that giving an $A$-complex structure on a set $C$ is equivalent to giving on $C$ a graded $A(\varepsilon)$-module structure, the differential $d$ corresponding to the homothety $\varepsilon_C$; analogously, morphisms of complexes correspond to degree 0 graded homomorphisms of graded $A(\varepsilon)$-modules. The species of graded $A(\varepsilon)$-module structures and of $A$-complex structures are therefore equivalent (E, IV, p. 9-10). We shall use this fact to carry over to the theory of complexes the usual notions of graded module theory.

To the notion of graded $A(\varepsilon)$-submodule corresponds that of a subcomplex: a subcomplex of the complex $(C,d)$ is thus a graded submodule $C'$ of $C$ such that, for all $n \in \mathbf{Z}$, $d_n(C'_n) \subset C'_{n-1}$; if we denote by $d'$ the graded $A$-homomorphism of $C'$ into $C'$ induced by $d$, then $(C', d')$ is a complex structure, called the one induced by $(C,d)$. Unless explicitly stated otherwise, any subcomplex will be assumed to be endowed with the induced structure.

We leave it to the reader to develop in the same way the notions of quotient complex, exact sequence of complexes, kernel, cokernel, image of a morphism of complexes, according to the dictionary below:

$$
\begin{array}{rcl}
A(\varepsilon)\text{-module gradué quotient} & = & \textit{complexe quotient},\\[2mm]
\left.
\begin{array}{l}
\text{noyau, conoyau, image d’un }A(\varepsilon)\text{-}\\
\text{homomorphisme gradué de degré 0}
\end{array}
\right\} & = &
\begin{array}{l}
\textit{noyau, conoyau, image d’un morphisme}\\
\textit{de complexes},
\end{array}\\[4mm]
\left.
\begin{array}{l}
\text{suite exacte de }A(\varepsilon)\text{-modules gradués et d’homomorphismes gradués}\\
\text{de degré 0}
\end{array}
\right\} & = & \textit{suite exacte de complexes.}
\end{array}
$$

For example, the canonical exact sequences of No. 1 give canonical exact sequences of complexes:

(I) $0 \to Z(C) \to C \xrightarrow{\delta} B(C) (-1) \to 0$,
(II) $0 \to B(C) \to Z(C) \to H(C) \to 0$,
(III) $0 \to B(C) \to C \to C/B(C) \to 0$,
(IV) $0 \to H(C) \to C/B(C) \xrightarrow{\delta} B(C) (-1) \to 0$,
(V) $0 \to H(C) \to C/B(C) \to Z(C) (-1) \to H(C) (-1) \to 0$.

We define analogously the notions of direct sum of complexes, inductive system of complexes, inductive limit of an inductive system of complexes.

Let $(C_i, d_i)$ be a family of complexes. We call the product of this family and denote $\prod_{i \in I} (C_i, d_i)$ the complex $(C, d)$ obtained as follows:

a) for each $n \in \mathbf{Z}$, $C_n$ is the product A-module $\prod_{i \in I} (C_i)_n$ of the homogeneous components $(C_i)_n$ of the given complexes,
b) for each $n \in \mathbf{Z}$, $d_n : C_n \to C_{n-1}$ is the component A-homomorphism $(d_i)_n$.

When $I$ is finite, $\prod_{i \in I} (C_i, d_i)$ is equal to $\bigoplus_{i \in I} (C_i, d_i)$. One must note that in general, the underlying A-module of the product complex $\prod_{i \in I} (C_i, d_i)$ is not the product A-module $\prod_{i \in I} C_i$.

Consider a family (resp. a filtered inductive system) $(C_i)_{i \in I}$ of complexes. Let $C$ be the direct sum (resp. the inductive limit) of the $C_i$, and let $\alpha_i : C_i \to C$ be the canonical homomorphisms. Then the $H(\alpha_i) : H(C_i) \to H(C)$ define a canonical degree 0 graded homomorphism of $\bigoplus_{i \in I} H(C_i)$ (resp. $\varprojlim_{i \in I} H(C_i)$) into $H(C)$. Similarly, the canonical projections $\prod_{i \in I} C_i \to C_i$ define a canonical degree 0 graded homomorphism of $H(\prod_{i \in I} C_i)$ into $\prod_{i \in I} H(C_i)$.

#### Proposition 1 {#alg-x-s2-prop-1 .statement}

For any family of complexes $(C_i)_{i \in I}$, the canonical homomorphisms
$$
\bigoplus_{i \in I} H(C_i) \to H(\bigoplus_{i \in I} C_i), \quad H(\prod_{i \in I} C_i) \to \prod_{i \in I} H(C_i)
$$
are bijective.

For every inductive filtering system of complexes $(C_i)_{i \in I}$, the canonical homomorphism
$$
\varprojlim_{i \in I} H(C_i) \to H(\varprojlim_{i \in I} C_i)
$$
is bijective.

This results immediately from II, p. 14, cor. 1 to prop. 7, p. 11, cor. to prop. 5, and p. 91, prop. 3.

### 3. The connecting homomorphism and the exact homology sequence

In this number, we consider an exact sequence of complexes
$$
0 \longrightarrow C' \xrightarrow{u} C \xrightarrow{v} C'' \longrightarrow 0 ;
$$
let us denote by the same letter $d$ the differentials of $C, C'$ and $C''$.

Let $\Gamma$ be the set of the $x \in C$ such that $dx \in \operatorname{Im}(u)$; for $x \in \Gamma$, we have
$$
d(\bar{u}^{-1}(dx)) = \bar{u}^{-1}(dd(x)) = 0 ,
$$
hence $\bar{u}^{-1}(dx) \in Z(C')$; we also have $dv(x) = v(dx) \in \operatorname{Im}(v \circ u) = 0$, hence $v(x) \in Z(C'')$; let us then consider the linear mapping $\varphi : \Gamma \to H(C'') \times H(C')$ which maps every element $x \in \Gamma$ onto the class of $(v(x), \bar{u}^{-1}(dx))$.

#### Lemma 1 {#alg-x-s2-lem-1 .statement}

The image $\varphi(\Gamma)$ of $\Gamma$ in $H(C'') \times H(C')$ is the graph of a graded A-homomorphism of degree $-1$ from $H(C'')$ into $H(C')$.

a) If $x \in \Gamma$ and if $v(x) \in B(C'')$, then $\bar{u}^{-1}(dx) \in B(C')$ : there exists indeed $z'' \in C''$ such that $v(x) = dz''$, then $z \in C$ such that $z'' = v(z)$, hence $v(x) = v(dz)$, then $t' \in C'$ such that $x - dz = u(t')$, which gives $dx = u(dt')$, hence $\bar{u}^{-1}(dx) = dt' \in B(C')$.

b) Every element of $Z(C'')$ is the image by $v$ of an element $x$ of $C$ such that $v(dx) = 0$, i.e. $dx \in \operatorname{Im} u$, that is to say such that $x \in \Gamma$.

c) It follows from a) and b) that $\varphi(\Gamma)$ is indeed a functional graph; since $\varphi$ is bihomogeneous of bidegree $(0, -1)$, this completes the proof.

The graded homomorphism of degree $-1$ from $H(C'')$ into $H(C')$ thus defined is called the connecting homomorphism relative to the exact sequence $(u, v)$; it is denoted by $\partial(u, v)$ or $\partial_{u,v}$ or simply $\partial$. Its homogeneous components are denoted
$$
\partial_n(u, v) : H_n(C'') \to H_{n-1}(C') \quad \text{and} \quad \partial^n(u, v) : H^n(C'') \to H^{n+1}(C') .
$$

By definition, to construct the image of a class $\alpha \in H_n(C'')$ by $\partial$, one chooses a cycle $z'' \in Z_n(C'')$ in the class $\alpha$, then an element $x$ of $C_n$ such that $v(x) = z''$; then $dx$ is of the form $u(t')$, $t' \in C'_{n-1}$, and $\partial(\alpha)$ is the homology class of $t'$.

In terms of correspondences, $\partial_n(u, v)$ is therefore obtained from the correspondence $\bar{u}_{n-1}^{-1} \circ d_n \circ \bar{v}_n^{-1}$ between $C''_n$ and $C'_{n-1}$, by passing to the subsets $Z_n(C'')$ and $Z_{n-1}(C')$, then to their quotients $H_n(C'')$ and $H_{n-1}(C')$. This shows in particular that, if one replaces $C, C', C'', u, v$ by $C(p), C'(p), C''(p), u(p), v(p)$, one has
$$
\partial(u(p), v(p)) = (-1)^p \partial(u, v) ;
$$
analogously, if $\lambda$ and $\mu$ are two invertible elements of the center of $A$, one has
$$
\partial(\lambda u, \mu v) = \lambda^{-1} \mu^{-1} \partial(u, v) .
$$

One can also relate $\partial(u, v)$ to the snake diagram (X, p. 4). According to loc. cit., prop. 2, the sequences
$$
0 \longrightarrow Z_n(C') \xrightarrow{Z_n(u)} Z_n(C) \xrightarrow{Z_n(v)} Z_n(C'')
$$

and

$$
C'_n/B_n(C') \xrightarrow{\overline{u}_n} C_n/B_n(C) \xrightarrow{\overline{v}_n} C''_n/B_n(C'') \longrightarrow 0 ,
$$

where $\overline{u}_n$ and $\overline{v}_n$ are deduced from $u$ and $v$, are exact. Using the canonical exact sequences $(V_n)$, one obtains a *commutative diagram* with exact rows and columns

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

The homomorphism $H_n(C'')\to H_{n-1}(C')$ associated with this diagram (loc. cit., prop. 2, (iii)) coincides by construction with $\partial_n(u,v).$ This furthermore implies that the sequence of homomorphisms $(H_n(u),\ H_n(v),\ \partial_n(u,v),\ H_{n-1}(u),\ H_{n-1}(v))$ is exact; consequently:

#### Theorem 1 {#alg-x-s2-thm-1 .statement}

*The unlimited sequence of homomorphisms of* $A$-*modules*

$$
\cdots \longrightarrow H_{n+1}(C'') \xrightarrow{\partial_{n+1}(u,v)} H_n(C') \xrightarrow{H_n(u)} H_n(C) \xrightarrow{H_n(v)} H_n(C'')
$$

$$
\xrightarrow{\partial_n(u,v)} H_{n-1}(C') \xrightarrow{H_{n-1}(u)} H_{n-1}(C) \xrightarrow{H_{n-1}(v)} H_{n-1}(C'') \xrightarrow{\partial_{n-1}(u,v)} H_{n-2}(C') \longrightarrow \cdots
$$

*is exact.*

This sequence is called the *exact homology sequence* associated with the exact sequence $(u,v)$; it is sometimes written in the form of an *exact triangle of* $A$-*modules*

$$
\begin{array}{ccc}
&&H(C)\\
&\nearrow^{H(u)}&\searrow^{H(v)}\\
H(C')&\xleftarrow{\partial(u,v)}&H(C'') .
\end{array}
$$

#### Corollary 1 {#alg-x-s2-thm-1-cor-1 .statement}

*If two of the complexes* $C$, $C'$, $C''$ *have zero homology, the third one does also. For* $u$ *(resp.* $v$*) to be a homomorphism, it is necessary and sufficient that* $C''$ *(resp.* $C'$*) *have zero homology. For* $\partial(u,v)$ *to be bijective, it is necessary and sufficient that* $C$ *have zero homology.*

#### Corollary 2 {#alg-x-s2-thm-1-cor-2 .statement}

Let u be a morphism of complexes. If Ker u and Coker u have zero homology, then u is a homologism.

Indeed, let u : E → E’ be a morphism of complexes. If Ker u (resp. Coker u) has zero homology, then the canonical morphism E → Im u (resp. Im u → E’) is a homologism by Corollary 1.

#### Proposition 2 {#alg-x-s2-prop-2 .statement}

Consider a commutative diagram of complexes with exact rows

$$
\begin{array}{ccccccccc}
0 & \longrightarrow & C' & \xrightarrow{u} & C & \xrightarrow{v} & C'' & \longrightarrow & 0 \\
& & f' \downarrow & & f \downarrow & & f'' \downarrow & & \\
0 & \longrightarrow & C'_1 & \xrightarrow{u_1} & C_1 & \xrightarrow{v_1} & C''_1 & \longrightarrow & 0 .
\end{array}
$$

Then $\mathrm{H}(f') \circ \partial(u, v) = \partial(u_1, v_1) \circ \mathrm{H}(f'')$.

Let $\alpha'' \in \mathrm{H}(C'')$; let $z''$ be a cycle of class $\alpha''$ and $x$ an element of $C$ such that $v(x) = z''$. We have
$$
(\partial_{u_1, v_1} \circ \mathrm{H}(f'')) (\alpha'') = \partial_{u_1, v_1}(\overline{f''(z'')}) = \overline{u_1^{-1}(df(x))} = \overline{f'(u_1^{-1}(dx))} =
= \mathrm{H}(f') (\overline{u^{-1}(dx)}) = (\mathrm{H}(f') \circ \partial_{u, v}) (\alpha'') .
$$

#### Example {#alg-x-s2-n3-exa-1 .statement}

Let $C$ be a complex. Consider the canonical exact sequence

(I)
$$
0 \longrightarrow Z(C) \xrightarrow{j} C \xrightarrow{\delta} B(C) (-1) \longrightarrow 0 ,
$$
and let $i : B(C) \to Z(C)$ be the canonical injection. Then the linking homomorphism $\partial(j, \delta) : \mathrm{H}(B(C)) (-1) \to \mathrm{H}(Z(C)) (-1)$ identifies with $\mathrm{H}(i) (-1)$, as one verifies at once. Since $\mathrm{H}(\delta) = 0$, the homology exact sequence associated to (I) decomposes into the short exact sequences

(II_n)
$$
0 \longrightarrow B_n(C) \xrightarrow{i} Z_n(C) \xrightarrow{\mathrm{H}(j)} H_n(C) \longrightarrow 0 .
$$

\* Mappings :

1) Singular homology

Let $A$ be a ring. For any topological space $X$, we define the singular complex $C(X, A)$ of $X$ with coefficients in $A$ as follows:

In $\mathbf{R}^{(N)}$, denote by $(e_n)$ the canonical basis; we call the $n$-canonical simplex the convex hull $\Delta_n$ of $\{ e_0, ..., e_n \}$. For $i \in \{ 0, ..., n \}$, we define the affine mapping $\iota_i : \Delta_{n-1} \to \Delta_n$ by $\iota_i(e_k) = e_k$ for $k < i$ and $\iota_i(e_k) = e_{k+1}$ for $k \geq i$. We denote $C_n(X, A)$ the a-module $A^{(\Sigma_n(X))}$, where $\Sigma_n(X)$ is the set of continuous mappings from $\Delta_n$ into $X$; for $n < 0$, we set $C_n = 0$. For $i \in \{ 0, ..., n \}$, we define the linear mapping $\partial_{n, i} : C_n(X, A) \to C_{n-1}(X, A)$ by $\partial_{n, i}(e_s) = e_{s \circ \iota_i}$ for $s \in \Sigma_n(X)$, and we set $d_n = \Sigma (-1)^i \partial_{n, i}$. We verify that

$$
... C_n(X, A) \xrightarrow{d_n} C_{n-1}(X, A) \to ...
$$

is a complex. Its homology is called the singular homology of $X$ with coefficients in $A$ and is denoted $\mathrm{H}(X, A)$ or simply $\mathrm{H}(X)$.

If $Y$ is a subspace of $X$, we denote $C(X, Y, A)$ the quotient complex $C(X, A)/C(Y, A)$, and $\mathrm{H}(X, Y, A)$ its homology. It follows from Theorem 1 that there is an exact sequence:

$$
... \to \mathrm{H}_n(Y, A) \to \mathrm{H}_n(X, A) \to \mathrm{H}_n(X, Y, A) \to \mathrm{H}_{n-1}(Y, A) \to \mathrm{H}_{n-1}(X, A) \to ...
$$

2) Finite cell complexes

Let $X$ be a separated topological space. A finite cell decomposition of $X$ is given by an increasing sequence $(X_n)_{n \in \mathbf{Z}}$ of closed subspaces of $X$ satisfying the following conditions:
(i) $X_n = \varnothing$ for $n < 0$;
(ii) there exists an $N$ such that $X_N = X$ (hence $X_n = X$ for $n > N$);
(iii) for every $n$, the space $X_n - X_{n-1}$ has only a finite number of connected components, called the $n$-dimensional cells;
(iv) for every $n$, and for every connected component $C$ of $X_n - X_{n-1}$, there exists a homeomorphism from the open $n$-dimensional euclidean ball $\hat{B}_n$ (TG, VI, p. 10) onto $C$ that extends to a continuous mapping of the closed ball into $X$.

One can show that these conditions imply that $\mathrm{H}_n(X_n, X_{n-1}, A)$ is a free a-module $\Gamma_n$ of rank equal to the number of $n$-dimensional cells, and that $\mathrm{H}_i(X_n, X_{n-1}, A) = 0$ for $i \neq n$. We have $C(X_n, X_{n-1}, A) = C(X_n, X_{n-2}, A)/C(X_{n-1}, X_{n-2}, A)$, hence an exact sequence

$$
\mathrm{H}_n(X_n, X_{n-2}) \longrightarrow \mathrm{H}_n(X_n, X_{n-1}) \xrightarrow{d_n} \mathrm{H}_{n-1}(X_{n-1}, X_{n-2}) \longrightarrow \mathrm{H}_{n-1}(X_n, X_{n-2}) ,
$$

involving a linking homomorphism $d_n : \Gamma_n \to \Gamma_{n-1}$. We have $d_n \circ d_{n+1} = 0$, which allows us to define a complex $\Gamma : \cdots \to \Gamma_n \xrightarrow{d_n} \Gamma_{n-1} \to \cdots$.

The exact sequence

==========

(Note: The final line "The exact sequence" is left as part of the text since the source ends there.)

$$
H_{n+1}(X_p, X_{p-1}) \to H_n(X_{p-1}) \to H_n(X_p) \to H_n(X_p, X_{p-1}) \to H_{n-1}(X_{p-1})
$$

shows by induction on p that $H_n(X_p) = 0$ for $p < n$, that $H_n(X_n) = \mathrm{Ker}\,(d_n : \Gamma_n \to \Gamma_{n-1})$ and that $H_n(X_p) = H_n(\Gamma)$ for $p > n$. In particular $H_n(X)$ is identified with $H_n(\Gamma)$.

#### Example {#alg-x-s2-n3-exa-2 .statement}

Consider the product of spheres $S_2 \times S_2$ and the complex projective space $P_2(\mathbf{C})$.
Let $b \in S_2$, we define a cellular decomposition $(Y_n)$ of $Y = S_2 \times S_2$ by setting

$$
Y_0 = Y_1 = \{ (b, b) \} , \quad Y_2 = Y_3 = (\{ b \} \times S_2) \cup (S_2 \times \{ b \}) \quad \text{and} \quad Y_4 = S_2 \times S_2 ;
$$

this decomposition has one cell of dimension 0, two of dimension 2 and one of dimension 4. The differentials of the associated complex are necessarily zero, so $H_0(Y)$, $H_2(Y)$ and $H_4(Y)$ are free of rank 1, 2 and 1 respectively, and $H_n(Y) = 0$ for $n \notin \{ 0, 2, 4 \}$.
One obtains a cellular decomposition $(Z_n)$ of $P_2(\mathbf{C})$ by setting

$$
Z_0 = Z_1 = \{ c \} , \quad Z_2 = Z_3 = P_1(\mathbf{C}) , \quad Z_4 = P_2(\mathbf{C}) ,
$$

the space $P_1(\mathbf{C})$ being embedded in $P_2(\mathbf{C})$ (TG, VIII, p. 20), and c being a point of $P_1(\mathbf{C})$; this decomposition has one cell of dimension 0, one of dimension 2 and one of dimension 4. Here again the differentials of the complex are necessarily zero, and it follows that $H_n(P_2(\mathbf{C}))$ is isomorphic to A for $n \in \{ 0, 2, 4 \}$ and to 0 otherwise.
Since the homology modules in degree 2 of the two spaces considered are free of rank 2 and 1 respectively, these spaces are not homeomorphic. \*

### 4. Homotopies

#### Definition 4 {#alg-x-s2-def-4 .statement}

Let $(C, d)$ and $(C', d')$ be two complexes, $f$ and $g$ two morphisms from $C$ to $C'$. A homotopy connecting $f$ to $g$ is any graded A-homomorphism $s$ of degree 1 from $C$ to $C'$ such that $g - f = d' \circ s + s \circ d$.
We say that $f$ and $g$ are homotopic if there exists a homotopy connecting $f$ to $g$.
If $h$ is a third morphism from $C$ to $C'$ and if $s$ (resp. $t$) is a homotopy connecting $f$ to $g$ (resp. $g$ to $h$), then $s + t$ is a homotopy connecting $f$ to $h$; consequently, the relation « $f$ and $g$ are two homotopic morphisms from $C$ to $C'$ » is an equivalence relation, whose classes are called the *homotopy classes of morphisms from $C$ to $C'$*.

Given two topological spaces $X$ and $Y$, and a continuous mapping $f : X \to Y$, one defines a linear mapping $f_*$ from the singular complex (*cf. No. 3*) $C(X, A)$ into $C(Y, A)$ by setting $f_*(e_s) = e_{f \circ s}$ for $s \in \Sigma_n(X)$. This mapping is a morphism of complexes.
Two continuous mappings $f$ and $g$ from $X$ into $Y$ are said to be topologically *homotopic* if there exists a continuous mapping $h$ from $[0, 1] \times X$ into $Y$ such that $h(0, x) = f(x)$ and $h(1, x) = g(x)$ for all $x \in X$. One shows that, if $f$ and $g$ are topologically homotopic, the morphisms $f_*$ and $g_*$ are homotopic in the sense of Definition 4 above. It is this fact that is at the origin of the terminology used in algebra.

#### Proposition 3 {#alg-x-s2-prop-3 .statement}

*If $f$ and $g$ are two homotopic morphisms from $C$ into $C'$, then $\mathrm{H}(f) = \mathrm{H}(g)$.* Let $s$ be a homotopy connecting $f$ to $g$. One has
$$
(g - f)(\mathbf{Z}(C)) = (d' \circ s + s \circ d)(\mathbf{Z}(C)) = (d' \circ s)(\mathbf{Z}(C)) \subset \mathbf{B}(C') ,
$$
hence $\mathrm{H}(g - f) = 0$ and $\mathrm{H}(g) = \mathrm{H}(f)$.

#### Corollaire {#alg-x-s2-n4-cor-1 .statement}

*A morphism homotopic to a homology isomorphism is a homology isomorphism.*

#### Proposition 4 {#alg-x-s2-prop-4 .statement}

*Let $C, C', D, D'$ be four complexes, $f : C \to C'$, $g : C \to C'$, $u : D \to C$, $v : C' \to D'$ four morphisms. If $s$ is a homotopy connecting $f$ to $g$, then $v \circ s \circ u$ is a homotopy connecting $v \circ f \circ u$ to $v \circ g \circ u$. If $f$ and $g$ are homotopic, then $v \circ f \circ u$ and $v \circ g \circ u$ are also homotopic.*
This is clear.

#### Corollaire {#alg-x-s2-n4-cor-2 .statement}

*Let $C, C', C''$ be three complexes, $f$ and $g$ two morphisms of $C$ into $C'$, $f_1$ and $g_1$ two morphisms of $C'$ into $C''$. If $s$ and $s_1$ are homotopies relating $f$ to $g$ and $f_1$ to $g_1$ respectively, then $s_1 \circ f + g_1 \circ s$ is a homotopy relating $f_1 \circ f$ to $g_1 \circ g$. If $f$ and $f_1$ are homotopic to $g$ and $g_1$ respectively, then $f_1 \circ f$ is homotopic to $g_1 \circ g$.
Indeed, $s_1 \circ f$ relates $f_1 \circ f$ to $g_1 \circ f$ and $g_1 \circ s$ relates $g_1 \circ f$ to $g_1 \circ g$.*

#### Definition 5 {#alg-x-s2-def-5 .statement}

*A morphism of complexes $f : C \to C'$ is called a homotopism if there exists a morphism $f' : C' \to C$ such that $f' \circ f$ and $f \circ f'$ are homotopic to $1_C$ and $1_{C'}$ respectively.*

It is clear that $f'$ is then also a homotopism; one also says that $f'$ is *reciprocal of $f$ up to homotopy*. If $f'$ and $f'_1$ are both reciprocals of $f$ up to homotopy, then $f'$ and $f'_1$ are homotopic (indeed by the preceding corollary, $f'_1 = f'_1 \circ 1_{C'}$ is homotopic to $f'_1 \circ f \circ f'$, hence to $1_C \circ f' = f'$).

#### Proposition 5 {#alg-x-s2-prop-5 .statement}

*A homotopism is a homologism; a morphism composed of homotopisms is a homotopism. A morphism homotopic to a homotopism is a homotopism.*

Let $f : C \to C'$ and $f_1 : C' \to C''$ be homotopisms of complexes, $f' : C' \to C$ and $f'_1 : C'' \to C'$ morphisms reciprocal up to homotopy. We have
$$
\mathrm{H}(f') \circ \mathrm{H}(f) = \mathrm{H}(f' \circ f) = \mathrm{H}(1_C) = 1_{\mathrm{H}(C)} \quad (\text{prop. 3})
$$

and analogously $\mathrm{H}(f) \circ \mathrm{H}(f') = 1_{\mathrm{H}(C')}$, so $\mathrm{H}(f)$ is bijective and $f$ is a homology isomorphism. On the other hand, $(f' \circ f'_1) \circ (f_1 \circ f)$ is homotopic to $f' \circ 1_C' \circ f$ (prop. 4), hence to $1_C$; analogously, $(f_1 \circ f) \circ (f' \circ f'_1)$ is homotopic to $1_{C''}$ and $f_1 \circ f$ is a homotopy equivalence. Finally, if $g : C \to C'$ is a morphism homotopic to $f$, $f' \circ g$ is homotopic to $f' \circ f$, hence to $1_C$; analogously, $g \circ f'$ is homotopic to $f \circ f'$, hence to $1_{C'}$ and $g$ is a homotopy equivalence.

#### Corollary {#alg-x-s2-n4-cor-3 .statement}

Let $C, C', D, D'$ be four complexes, $f : C \to C'$ a morphism, $u : D \to C$ and $v : C' \to D'$ homotopy equivalences. For $v \circ f \circ u$ to be a homotopy equivalence (resp. a homology isomorphism), it is necessary and sufficient that $f$ be one.

If $f$ is a homotopy equivalence (resp. a homology isomorphism), then $v \circ f \circ u$ is a composition of homotopy equivalences (resp. homology isomorphisms), hence is one. Conversely, let $\overline{u}$ and $\overline{v}$ be morphisms inverse to $u$ and $v$ up to homotopy; then $\overline{v} \circ (v \circ f \circ u) \circ \overline{u}$ is homotopic to $f$ by prop. 4; whence the conclusion by prop. 5, and the corollary of prop. 3.

One says that the complex $C$ is homotopic to zero if $1_C$ is homotopic to the zero mapping, that is, if there exists a graded $A$-endomorphism $s$ of degree 1 of $C$ such that $1_C = s \circ d + d \circ s$. This also amounts to saying that the unique morphism $0 \to C$ (resp. $C \to 0$) is a homotopy equivalence. A complex homotopic to zero has zero homology (prop. 5).

#### Example {#alg-x-s2-n4-exa-1 .statement}

Let $u : M \to N$ and $v : N \to P$ be homomorphisms of $A$-modules such that $v \circ u = 0$; let $C$ be the complex such that $C_2 = M, C_1 = N, C_0 = P, C_i = 0$ for $i \neq 0, 1, 2$, $d_2 = u, d_1 = v, d_i = 0$ for $i \neq 1, 2$. Then $C$ has zero homology if and only if the sequence $0 \to M \xrightarrow{u} N \xrightarrow{v} P \to 0$ is exact. It is homotopic to zero if and only if this sequence is split. Indeed, saying that $C$ is homotopic to zero means that there exist $A$-homomorphisms $s : P \to N$ and $t : N \to M$ such that $v \circ s = 1_P, s \circ v + u \circ t = 1_N, t \circ u = 1_M$; this implies that the sequence is split; conversely, if $s$ is an $A$-linear section of $v$, one defines $t$ by $u \circ t = 1_N - s \circ v$, which is possible since $v \circ (1_N - s \circ v) = v - v \circ s \circ v = 0$.

### 5. Split complexes

#### Proposition 6 {#alg-x-s2-prop-6 .statement}

Let $(C, d)$ be a complex. The following conditions are equivalent:
(i) there exists a homotopy equivalence from $(C, d)$ to $(\mathrm{H}(C), 0)$;
(ii) there exists an $A$-endomorphism $s$ of $C$, graded of degree 1, such that $d = d \circ s \circ d$;
(iii) $B(C)$ and $Z(C)$ are direct summands of $C$;
(iv) $(C, d)$ is a direct sum of subcomplexes which are either of length 0, or of length 1 and have zero homology.

(i) $\Rightarrow$ (ii): let $\varphi : C \to \mathrm{H}(C)$ be a homotopy equivalence; then there exists a morphism of complexes $\psi : \mathrm{H}(C) \to C$ and an endomorphism $s$ of $C$, graded of degree 1, such that $\psi \circ \varphi = 1_C - s \circ d - d \circ s$. We have $d \circ \psi = \psi \circ 0 = 0$, hence
$$
0 = d \circ \psi \circ \varphi = d - d \circ s \circ d - d \circ d \circ s = d - d \circ s \circ d ,
$$
whence (ii).

$(ii) \Rightarrow (iii)$: let $s$ be as in (ii). Then $d \circ (1_C-s\circ d)=0$, so $1_C-s\circ d$ is a projector of $C$ onto $Z(C)$, and $(d\circ s)\circ d=d$, so $d\circ s$ is a projector of $C$ onto $B(C)$.

$(iii) \Rightarrow (iv)$: for each $n\in\mathbf{Z}$, let $Z_n=Z_n(C)$, $B_n=B_n(C)$ and choose submodules $K_n$ and $B'_n$ of $C_n$ such that $C_n=B'_n\oplus Z_n$, $Z_n=K_n\oplus B_n$. Then

$$
E_{(n)}=K_n(-n)\quad\text{and}\quad F_{(n)}=B'_n(-n)\oplus B_{n-1}(1-n)
$$

are subcomplexes of $(C,d)$; one has

$$
(C,d)=\bigoplus_{n\in\mathbf{Z}}(E_{(n)}\oplus F_{(n)})
$$

; each $E_{(n)}$ is either zero or of length $0$, each $F_{(n)}$ is either zero or of length $1$ and of zero homology, whence (iv).

$(iv) \Rightarrow (i)$: it suffices to remark that (i) is satisfied when $C$ is of length zero, or of zero homology and of length 1.

#### Definition 6 {#alg-x-s2-def-6 .statement}

*A complex $C$ is said to be split if it satisfies the equivalent conditions of Prop. 6.*

An endomorphism $s$ of $C$ satisfying condition (ii) of Prop. 6 is called a *splitting* of $C$.

#### Example 1 {#alg-x-s2-n5-exa-1 .statement}

A complex with zero differential is split.

#### Example 2 {#alg-x-s2-n5-exa-2 .statement}

The complexes homotopic to zero are the split complexes of zero homology, *i.e.* the complexes $C$ such that $H(C)=0$ and that $Z(C)$ is a direct factor in $C$.

#### Example 3 {#alg-x-s2-n5-exa-3 .statement}

Let $f:M\to N$ be a homomorphism of A-modules and $C$ the complex such that $C_1=M$, $C_0=N$, $C_i=0$ for $i\ne0,1$, $d_1=f$, $d_i=0$ for $i\ne1$. Then $C$ is split if and only if $\operatorname{Ker}f$ is a direct factor in $M$ and $\operatorname{Im}f$ a direct factor in $N$.

#### Example 4 {#alg-x-s2-n5-exa-4 .statement}

*The complex $C$ is split as soon as $B(C)$ and $H(C)$ are projective (resp. as soon as $B_n(C)$ and $H_n(C)$ are injective for each $n$).* Indeed, according to the exact sequences $(I_n)$ to $(IV_n)$ of No. 1, $Z(C)$ is then a direct factor in $C$ and $B(C)$ a direct factor of $Z(C)$ (resp. $B(C)$ is a direct factor in $C$ and $Z(C)/B(C)$ a direct factor in $C/B(C)$).

#### Example 5 {#alg-x-s2-n5-exa-5 .statement}

In particular, if A is principal, a free complex $C$ is split if and only if $H(C)$ is free (that is to say $H_n(C)$ free for every $n\in\mathbf{Z}$).

#### Remark {#alg-x-s2-n5-rem-1 .statement}

a) Suppose that the canonical exact sequence of graded A-modules

$$
\tag{II}
0\longrightarrow B(C)\longrightarrow Z(C)\xrightarrow{\pi}H(C)\longrightarrow0
$$

be split (this occurs for example if $H(C)$ is projective, or $B_n(C)$ injective for each $n$); let $\sigma:H(C)\to Z(C)$ be a graded A-linear section of $\pi$, and let $\psi$ be the homomorphism $x\mapsto\sigma(x)$ from $H(C)$ into $C$. Then $\psi$ is a *homologism* from $(H(C),0)$ into $C$, such that

$$
H(\psi)=1_{H(C)}.
$$

b) Suppose that the canonical exact sequence of graded A-modules

$$
\tag{IV}
0\longrightarrow H(C)\xrightarrow{i}C/B(C)\longrightarrow B(C)(-1)\longrightarrow0
$$

is split (this occurs for example if $B(C)$ is projective, or $H_n(C)$ injective for each $n$); let $\tau : C/B(C) \to H(C)$ be a graded A-linear retraction of $i$ and let $\varphi$ be the homomorphism from $C$ into $H(C)$ which associates to each element of $C$ the image by $\tau$ of its class modulo $B(C)$. Then $\varphi$ is a *homologism from $C$ into $(H(C), 0)$ such that* $H(\varphi) = 1_{H(C)}$.

### 6. Cone and cylinder of a morphism of complexes

Let $u : (C', d') \to (C, d)$ be a morphism of complexes. Let $\mathrm{Cyl}\,(u)$ and $\mathrm{Con}\,(u)$ be the graded A-modules $\mathrm{Cyl}\,(u) = C' \oplus C'(-1) \oplus C$, $\mathrm{Con}\,(u) = C'(-1) \oplus C$, and define graded A-linear mappings of degree $(-1)$

$$
\overline{D} : \mathrm{Cyl}\,(u) \to \mathrm{Cyl}\,(u) , \quad \overline{D}(x', y', x) = (d'x' + y', -d'y', dx - u(y')),
$$
$$
D : \mathrm{Con}\,(u) \to \mathrm{Con}\,(u) , \quad D(y', x) = (-d'y', dx - u(y')) .
$$

(Here, and in what follows, $x, y, \ldots$ denote arbitrary elements of $C$, $x', y', \ldots$ arbitrary elements of $C'$.)

#### Lemma 2 {#alg-x-s2-lem-2 .statement}

(*Cyl* $(u)$, $\overline{D}$) *and* (*Con* $(u)$, $D$) *are complexes of A-modules*.

Indeed, one has
$$
\overline{D} \circ \overline{D}(x', y', x) = \overline{D}(d'x' + y', -d'y', dx - u(y')) =
$$
$$
= (d'(d'x' + y') - d'y', -d'(-d'y'), d(dx - u(y')) - u(-d'y')) = 0
$$
since $d' \circ d' = 0$, $d \circ d = 0$ and $d \circ u = u \circ d'$. Similarly $D \circ D = 0$.

#### Definition 7 {#alg-x-s2-def-7 .statement}

*The complexes* $\mathrm{Cyl}\,(u)$ *and* $\mathrm{Con}\,(u)$ *are called respectively the cylinder* *and the cone of the morphism* $u$.

#### Example {#alg-x-s2-n6-exa-1 .statement}

Let $u : M \to N$ be a homomorphism of A-modules; then the only non-zero homogeneous components of $\mathrm{Cyl}\,(u)$ and $\mathrm{Con}\,(u)$ are
$$
\mathrm{Cyl}_1\,(u) = M , \qquad \mathrm{Cyl}_0\,(u) = M \oplus N ,
$$
$$
\mathrm{Con}_1\,(u) = M , \qquad \mathrm{Con}_0\,(u) = N ,
$$
and we have $\overline{D}(m) = (m, -u(m))$, $D(m) = -u(m)$ for $m \in M$; consequently,
$$
H_1(\mathrm{Con}\,(u)) = \mathrm{Ker}\,(u) , \quad H_0(\mathrm{Con}\,(u)) = \mathrm{Coker}\,(u) .
$$

*Let* $X$ *and* $Y$ *be two topological spaces and* $f$ *a continuous mapping from* $X$ *into* $Y$. The *cylinder* of $f$ is called the quotient space $\mathrm{Cyl}\,(f)$ of the topological sum of $[0, 1] \times X$ and $Y$ by the equivalence relation identifying the point $(1, x)$ of $[0, 1] \times X$ with the point $f(x)$ of $Y$ for every $x \in X$. The *cone* of $f$ is called the quotient space $\mathrm{Con}\,(f)$ of the topological sum of a space reduced to a point $s$ and $\mathrm{Cyl}\,(f)$ by the equivalence relation identifying $s$ with the image of $(0, x)$ for every $x \in X$: we still denote by $s$ the image of $s$ in $\mathrm{Con}\,(f)$.

Suppose that $X$ and $Y$ are endowed with cellular decompositions $(X_n)$ and $(Y_n)$ (*cf.* No. 3), and suppose that $f(X_n) \subset Y_n$ for every $n$. We obtain a cellular decomposition $(S_n)$ of $\mathrm{Cyl}\,(f)$ (resp. of $\mathrm{Con}\,(f)$) by taking for $S_n$ the image of $(\{0\} \times X_n) \cup ([0, 1] \times X_{n-1}) \cup Y_n$
$$
(\text{resp. of } \{s\} \cup ([0, 1] \times X_{n-1}) \cup Y_n , \quad \text{if } n \geqslant 0) .
$$
Let $\Gamma(X), \Gamma(Y), \Gamma(\mathrm{Cyl}\,(f)), \Gamma(\mathrm{Con}\,(f))$ denote the complexes associated with these cellular decompositions.

The complex $\Gamma(s)$ associated with the space $\{ s \}$ endowed with its unique cellular decomposition is reduced to the module $\mathbf{A}$ and is identified with a subcomplex of $\Gamma(\mathrm{Con}\,(f))$; let $\Gamma(\mathrm{Con}\,(f),\,s)$ denote the quotient complex. The mapping $f$ defines a morphism of complexes $\Gamma(f) : \Gamma(X) \to \Gamma(Y)$, and one can show that the complexes $\Gamma(\mathrm{Cyl}\,(f))$ and $\Gamma(\mathrm{Con}\,(f),\,s)$ are identified respectively with $\mathrm{Cyl}\,(\Gamma(f))$ and $\mathrm{Con}\,(\Gamma(f))$.

Par ailleurs, et sans hypothèses sur $X$ et $Y$, on associe à $f$ un morphisme de complexes $f_* : C(X,\,\mathbf{A}) \to C(Y,\,\mathbf{A})$. On peut construire des homotopismes injectifs de $\mathrm{Cyl}\,(f_*)$ dans $C(\mathrm{Cyl}\,(f),\,\mathbf{A})$ et de $\mathrm{Con}\,(f_*)$ dans $C(\mathrm{Con}\,(f),\,\{s\},\,\mathbf{A})$.
Soient $\tilde{f} : X \to \mathrm{Cyl}\,(f)$ l'application qui à $x$ associe l'image de $(0,\,x)$, $\alpha : Y \to \mathrm{Cyl}\,(f)$ l'application canonique et $\beta : \mathrm{Cyl}\,(f) \to Y$ l'application qui associe $y$ à son image dans $\mathrm{Cyl}\,(f)$ pour $y \in Y$ et $f(x)$ à l'image de $(t,\,x)$ dans $\mathrm{Cyl}\,(f)$ pour $t \in [0,\,1]$ et $x \in X$. L'application $\tilde{f}$ est un homéomorphisme de $X$ sur un fermé de $\mathrm{Cyl}\,(f)$, on a $\beta \circ \alpha = \mathrm{Id}_Y$, et $\alpha \circ \beta$ est topologiquement homotope à l'identité de $\mathrm{Cyl}\,(f)$. Ces propriétés sont à rapprocher de la proposition 7 ci-dessous. \*

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

*c)* *Les morphismes* $\alpha : C \to \mathrm{Cyl}\,(u)$ *et* $\beta : \mathrm{Cyl}\,(u) \to C$ *sont des homotopismes réciproques l'un de l'autre à homotopie près*.

L'assertion *a)* est équivalente aux formules

$$
\begin{align*}
\tilde{u} \circ d' &= \overline{D} \circ \tilde{u}\,, & \alpha \circ d &= \overline{D} \circ \alpha\,, & \beta \circ \overline{D} &= d \circ \beta\,, & \pi \circ d &= D \circ \pi\,, \\
\tilde{\pi} \circ \overline{D} &= D \circ \tilde{\pi}\,, & \delta \circ D &= -d' \circ \delta\,, & u &= \beta \circ \tilde{u}\,, & \pi &= \tilde{\pi} \circ \alpha\,, & \beta \circ \alpha &= 1_C
\end{align*}
$$

qui se vérifient par des calculs immédiats. L'assertion *b)* est triviale. Démontrons *c)* ; on a d'une part $\beta \circ \alpha = 1_C$; d'autre part si $\sigma : \mathrm{Cyl}\,(u) \to \mathrm{Cyl}\,(u)$ est l'application $\mathbf{A}$-linéaire graduée de degré 1 telle que $\sigma(x',\,y',\,x) = (0,\,x',\,0)$, on vérifie aussitôt que

$$
\overline{D} \circ \sigma + \sigma \circ \overline{D} + \alpha \circ \beta = 1_{\mathrm{Cyl}\,(u)}\,,
$$

d'où *c)*.

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

*a)* *L'homomorphisme de liaison*
$$
\partial_{n+1}(\pi, \delta) : H_n(C') \to H_n(C)
$$
*relatif à la suite exacte (7) est égal à* $-H_n(u)$.

*b)* *L'homomorphisme de liaison*
$$
\partial_n(\tilde{u}, \tilde{\pi}) : H_n(\mathrm{Con}\,(u)) \to H_{n-1}(C')
$$
*relatif à la suite exacte (6) est égal à* $H_n(\delta)$.

Soit $x' \in Z_n(C')$; comme $x' = \delta(x', 0)$ et que
$$
- D(x', 0) = (d'x', u(x')) = (0, u(x')) = \pi(u(x')) ,
$$
$\partial(\pi, \delta)$ applique par définition la classe de $x'$ dans $H_n(C')$ sur la classe de $-u(x')$ dans $H_n(C)$, d'où *a)*.

Soit $(y', x) \in \mathrm{Con}_n(u)$ tel que $D(y', x) = 0$; on a alors $(-d'y', dx - u(y')) = 0$. Comme $(y', x) = \tilde{\pi}(0, y', x)$ et que
$$
\overline{D}(0, y', x) = (y', -d'y', dx - u(y')) = (y', 0, 0) = \tilde{u}(\delta(y', x)) ,
$$
$\partial(\tilde{u}, \tilde{\pi})$ applique par définition la classe de $(y', x)$ dans $H_n(\mathrm{Con}\,(u))$ sur la classe de $\delta(y', x)$ dans $H_{n-1}(C')$, d'où *b)*.

#### Proposition 8 {#alg-x-s2-prop-8 .statement}

*On a la suite exacte illimitée*
(8) $$ \cdots \longrightarrow H_n(C') \xrightarrow{H_n(u)} H_n(C) \xrightarrow{H_n(\pi)} H_n(\mathrm{Con}\,(u)) \xrightarrow{H_n(\delta)} H_{n-1}(C') \longrightarrow \cdots . $$

En effet, compte tenu du *lemme 3, a)*, cela résulte du théorème 1 de X, p. 30, appliqué à la suite exacte (7).

#### Corollaire {#alg-x-s2-n6-cor-2 .statement}

*Pour que u soit un homologisme, il faut et il suffit que Con (u) soit d'homologie nulle.*

#### Remarque {#alg-x-s2-n6-rem-1 .statement}

Considérons le diagramme

$$
\begin{array}{ccccccccc}
\cdots & \longrightarrow & H_n(C') & \xrightarrow{H_n(\tilde{u})} & H_n(\mathrm{Cyl}\,(u)) & \xrightarrow{H_n(\pi)} & H_n(\mathrm{Con}\,(u)) & \xrightarrow{\partial_n(\tilde{u},\pi)} & H_{n-1}(C') \longrightarrow \cdots \\
& & \downarrow 1 & & \downarrow H_n(\beta) & & \downarrow 1 & & \downarrow 1 \\
\cdots & \longrightarrow & H_n(C') & \xrightarrow{H_n(u)} & H_n(C) & \xrightarrow{H_n(\pi)} & H_n(\mathrm{Con}\,(u)) & \xrightarrow{H_n(\delta)} & H_{n-1}(C') \longrightarrow \cdots
\end{array}
$$

où la première ligne (resp. la seconde) est la suite exacte d'homologie associée à la suite exacte (6) (resp. (7)). Les applications $H_n(\beta)$ sont bijectives (prop. 7, c)) et le diagramme est commutatif, puisque
a) $u = \beta \circ \tilde{u}$ (prop. 7, a)) donc $H_n(u) = H_n(\beta) \circ H_n(\tilde{u})$,
b) $H_n(\beta) = H_n(\alpha)^{-1}$ et $\pi = \tilde{\pi} \circ \alpha$ (prop. 7, a) et c)), donc $H_n(\tilde{\pi}) = H_n(\pi) \circ H_n(\beta)$,
c) $H_n(\delta) = \partial_n(\tilde{u},\tilde{\pi})$ (*lemme 3, b*)).

### 7. Le cône d'un morphisme injectif ; nouvelle définition de l'homomorphisme de liaison

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
donc $\varphi$ est bien un morphisme de complexes. D'autre part, $\varphi$ est surjectif et son noyau s'identifie au complexe $(\mathbf{K}, d_\mathbf{K})$ tel que $\mathbf{K} = C'(-1) \oplus C'$,
$$
d_\mathbf{K}(y', x') = (-d'y', d'x' - y') ;
$$
si $d_\mathbf{K}(y', x') = 0$, on a $y' = d' x'$, donc $(y', x') = d_\mathbf{K}(0, -x')$; il s'ensuit que $\mathrm{H}(\mathbf{K}) = 0$ et $\varphi$ est un homologisme d'après X, p. 30, cor. 1.

#### Remarque {#alg-x-s2-n7-rem-1 .statement}

L'homologisme $\beta$ est un homotopisme, mais $\varphi$ n'est pas en général un homotopisme (*cf.* X, p. 173, exercice 8).

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

Dans le diagramme commutatif (10), on a $H(1_{C'})\circ\widetilde{\partial}(\tilde u,\tilde\pi)=\partial(u,v)\circ H(\varphi)$ (X, p. 31, prop. 2) et $\widetilde{\partial}(\tilde u,\tilde\pi)=H(\delta)$ (X, p. 38, *lemme 3, b*)), donc

$$
\partial(u,v)\circ H(\varphi)=H(\delta)\ ;
$$

d'autre part, $H(v)\circ H(\beta)=H(\varphi)\circ H(\tilde\pi)=H(\varphi)\circ H(\pi)\circ H(\beta)$ d'après X, p. 39, remarque. Comme $H(\beta)$ est bijectif, cela donne $H(v)=H(\varphi)\circ H(\pi)$.

On a donc $\partial(u,v)=H(\delta)\circ H(\varphi)^{-1}$, ce qui fournit une *nouvelle définition* de l'homomorphisme de liaison $\partial(u,v)$. On notera d'autre part que si on identifie $H(\operatorname{Con}(u))$ à $H(C'')$ par $H(\varphi)$, le corollaire précédent signifie que *la suite exacte* (8) *s'identifie alors à la suite exacte d'homologie relative à* (9).

### 8. Caractéristiques d'Euler-Poincaré

Dans ce no, on considère un ensemble $\mathcal C$ de classes de A-modules qui est *additif et exact à gauche*, c'est-à-dire qui satisfait aux deux conditions suivantes :

(A) *Si* $M$ *et* $N$ *sont deux A-modules de type* $\mathcal C$, $M\oplus N$ *est de type* $\mathcal C$.

(G) If $0\to M'\to M\to M''\to0$ is an exact sequence of A-modules and if $M$ and $M''$ are of type $\mathcal C$, then $M'$ is of type $\mathcal C$.

We say that $\mathcal C$ is stable if it satisfies the following conditions which imply (A) and (G):

(E) ("$\mathcal C$ is stable under extensions.") If $0\to M'\to M\to M''\to0$ is an exact sequence of A-modules and if $M'$ and $M''$ are of type $\mathcal C$, then $M$ is of type $\mathcal C$.

(S) ("$\mathcal C$ is stable under kernels and cokernels.") For every homomorphism $f$ of A-modules of type $\mathcal C$, the A-modules $\operatorname{Ker}f$ and $\operatorname{Coker}f$ are of type $\mathcal C$.

We denote by $K(\mathcal C)$ the grothendieck group of $\mathcal C$ and by $[M]_{\mathcal C}$ or $[M]$ the element of $K(\mathcal C)$ defined by the A-module $M$ (VIII, §6, No. 2). Let $G$ be a commutative group and $\varphi$ a homomorphism of $K(\mathcal C)$ into $G$.

#### Example 1 {#alg-x-s2-n8-exa-1 .statement}

If A is a field, we may take as $\mathcal C$ the set of classes of finite-dimensional vector spaces and as $\varphi$ the isomorphism of $K(\mathcal C)$ onto $\mathbf Z$ defined by $\varphi([M]) = \dim(M)$.

#### Example 2 {#alg-x-s2-n8-exa-2 .statement}

We may take as $\mathcal C$ the set of classes of modules of finite length and as $\varphi: K(\mathcal C) \to \mathbf Z$ the homomorphism defined by $\varphi([M]) = \operatorname{long}_A(M)$.

We say that a graded A-module M is of type $\mathcal C$ if $M_n$ is of type $\mathcal C$ for all n (for this, it is necessary when M is bounded and sufficient when $\mathcal C$ is stable that the module M be of type $\mathcal C$).

#### Definition 8 {#alg-x-s2-def-8 .statement}

Let M be a bounded graded A-module of type $\mathcal C$ and $(M_n)$ its grading. We call the $\varphi$-characteristic of M and denote $\chi_\varphi(M)$ or simply $\chi(M)$ the element $\sum (-1)^n \varphi([M_n])$ of G.

This definition applies in particular when M is the graded module underlying a complex of A-modules.

#### Example 3 {#alg-x-s2-n8-exa-3 .statement}

If M is bounded of type $\mathcal{C}$, it is analogously the case for $M(p)$ for every $p \in \mathbf{Z}$, and one has $\chi(M(p)) = (-1)^p \chi(M)$.

4) Let $0 \to M' \to M \to M'' \to 0$ be an exact sequence of graded A-modules and graded homomorphisms of degree 0. If M, M' and M'' are bounded of type $\mathcal{C}$, one has
$$
\chi(M) = \chi(M') + \chi(M'').
$$
If M and M'' are bounded of type $\mathcal{C}$, it is analogously the case for M'; if $\mathcal{C}$ is stable and if two of the three modules are bounded of type $\mathcal{C}$, it is analogously the case for the third.

5) Let $u : C' \to C$ be a morphism of bounded complexes of type $\mathcal{C}$. Then Con ($u$) is bounded of type $\mathcal{C}$, and one has:
$$
\chi(\operatorname{Con}(u)) = \chi(C) - \chi(C').
$$

6) One may take for G the group $K(\mathcal{C})$ itself, and for $\varphi$ the identity; in this case one denotes by $\chi_{\mathcal{C}}(M)$ the element $\chi_\varphi(M) = \sum (-1)^n[M_n]$ of $K(\mathcal{C})$.

#### Remark {#alg-x-s2-n8-rem-1 .statement}

One calls the Poincaré polynomial of M relative to $\varphi$ the element $P_M(t) = \sum \varphi([M_n]) t^n \in G \otimes \mathbf{Z}[t, t^{-1}]$. One has $P_M(1) = \varphi([M])$ and $P_M(-1) = \chi(M)$.

#### Lemma 4 {#alg-x-s2-lem-4 .statement}

Let C be a bounded complex of type $\mathcal{C}$. If $H(C) = 0$, one has $\chi(C) = 0$.
This follows from VIII, § 6, No. 1, cor. of Prop. 1.

#### Proposition 10 {#alg-x-s2-prop-10 .statement}

Let C and C' be two bounded complexes of type $\mathcal{C}$. If there exists a homologism $u : C' \to C$, one has $\chi(C) = \chi(C')$.
Indeed, Con ($u$) is bounded of type $\mathcal{C}$ and one has $\chi(\operatorname{Con}(u)) = \chi(C) - \chi(C')$; on the other hand, $H(\operatorname{Con}(u)) = 0$ by X, p. 38, cor., hence $\chi(\operatorname{Con}(u)) = 0$ (lemma 4).

#### Proposition 11 {#alg-x-s2-prop-11 .statement}

Let C be a bounded complex of type $\mathcal{C}$.
a) If $\mathcal{C}$ is stable, $H(C)$ is of type $\mathcal{C}$.
b) If $H(C)$ is of type $\mathcal{C}$, it is analogously the case for $B(C)$ and $Z(C)$, and one has $\chi(H(C)) = \chi(C)$.

a) If $\mathcal{C}$ is stable, for every $n$ the module $Z_n(C)$ is of type $\mathcal{C}$ as kernel of $d_n : C_n \to C_{n-1}$, and $H_n(C)$ is of type $\mathcal{C}$ as cokernel of $C_{n+1} \to Z_n$. On the other hand, $H_n(C) = 0$ as soon as $C_n = 0$.

b) Suppose $H(C)$ of type $\mathcal{C}$. The canonical exact sequences:

$$
0 \to Z_n(C) \to C_n \to B_{n-1}(C) \to 0
$$
$$
0 \to B_n(C) \to Z_n(C) \to H_n(C) \to 0
$$

show by induction on $n$ starting from the right bound of $C$ that $Z_n(C)$ and $B_n(C)$ are of type $\mathcal{C}$ for all $n$. One then has

$$
\chi(C) = \chi(Z(C)) + \chi(B(C) (-1)) = \chi(Z(C)) - \chi(B(C)) = \chi(H(C)) .
$$

#### Corollary {#alg-x-s2-n8-cor-1 .statement}

*If $\mathcal{C}$ is stable and $C$ is bounded of type $\mathcal{C}$, the graded module $H(C)$ is bounded of type $\mathcal{C}$ and one has $\chi(H(C)) = \chi(C)$.*

#### Proposition 12 {#alg-x-s2-prop-12 .statement}

*Let $0 \to C' \to C \to C'' \to 0$ be an exact sequence of complexes.*

*a) If $H(C), H(C')$ and $H(C'')$ are bounded of type $\mathcal{C}$, one has*
$$
\chi(H(C)) = \chi(H(C')) + \chi(H(C'')) .
$$

*b) If $\mathcal{C}$ is stable, and if two of the graded modules $H(C), H(C')$ and $H(C'')$ are bounded of type $\mathcal{C}$, the same holds for the third.*

Part a) follows from Lemma 4 applied to the complex with zero homology defined by the homology exact sequence associated with the given exact sequence. Part b) follows, by considering this homology exact sequence, from the following lemma:

*Lemma 5. — Let $M \to N \to P \to Q \to R$ be an exact sequence of $A$-modules. If $\mathcal{C}$ is stable, and if $M, N, Q$ and $R$ are of type $\mathcal{C}$, the module $P$ is of type $\mathcal{C}$.
Set $N' = \operatorname{Coker}(M \to N)$ and $Q' = \operatorname{Ker}(Q \to R)$. The modules $N'$ and $Q'$ are of type $\mathcal{C}$, and one has an exact sequence $0 \to N' \to P \to Q' \to 0$.*

#### Corollary {#alg-x-s2-n8-cor-2 .statement}

*Assume $\mathcal{C}$ stable, and let $u : C' \to C$ be a morphism of complexes such that $H(C)$ and $H(C')$ are bounded of type $\mathcal{C}$. Then $H(\operatorname{Con}(u))$ is bounded of type $\mathcal{C}$, and one has*
$$
\chi(H(\operatorname{Con}(u))) = \chi(H(C)) - \chi(H(C')) .
$$

This follows from Prop. 12 applied to the exact sequence of complexes (X, p. 37, Prop. 7)
$$
0 \to C \to \operatorname{Con}(u) \to C'(-1) \to 0 .
$$

*Remark. — Let $E$ be a complex, $h : E \to C$ and $h' : E \to C'$ be homotopy equivalences with $C$ and $C'$ bounded of type $\mathcal{C}$. Then $\chi(C) = \chi(C')$. Indeed, if $h_1$ is an inverse of $h$ up to homotopy, $h' \circ h_1$ is a homotopy equivalence, hence a homology isomorphism from $C$ to $C'$, and one can apply Prop. 10. Consequently, one can extend Definition 8 by setting $\chi(E) = \chi(C)$ whenever there exists a homotopy equivalence from $E$ to a complex $C$ bounded of type $\mathcal{C}$. Propositions 10, 11, 12 and their corollaries generalise in this setting.*

Application:

\* Let X be a topological space admitting a finite cellular decomposition (cf. No. 3).
    a) Let K and K' be two fields, put $b_i = \dim_K(H_i(X, K))$ and $b'_i = \dim_{K'}(H_i(X, K'))$. It is not necessarily the case that $b_i = b'_i$, but one has $\Sigma (-1)^i b_i = \Sigma (-1)^i b'_i$.
    b) Let $(X_n)$ and $(X'_n)$ be two finite cellular decompositions of X, and denote by $c_n$ and $c'_n$ the number of cells of dimension n in these two decompositions. One has
    $$
    \Sigma (-1)^i c_i = \Sigma (-1)^i c'_i .
    $$
    c) With the notations of a) and b), one has $\Sigma (-1)^i c_i = \Sigma (--1)^i b_i$.
    The properties a) and b) result from c), and c) results from prop. 11 applied to the complex $\Gamma$ described in No. 3, taking for $\mathcal{C}$ the class of finite-dimensional K-vector spaces and for $\varphi$ the function defined by $\varphi([M]) = \dim_K(M)$ (X, p. 40, example 1).

### 9. Complexes of right modules, complexes of multimodules

A complex of right A-modules is a graded right A-module $(M_n)_{n \in \mathbf{Z}}$ endowed with a graded endomorphism $d$ of degree -1 and square zero; it is therefore a complex of modules over the ring A opposite to A. All the definitions and properties stated in the preceding numbers therefore apply to complexes of right modules considered as complexes of modules over the ring $A^\circ$.

Similarly, if A and B are two rings, a complex of (A, B)-bimodules is a graded (A, B)-bimodule M endowed with a graded endomorphism $d$ of degree (-1) and square zero; if M is endowed with its canonical structure of $A \otimes_\mathbf{Z} B^\circ$-left module, $d$ endows it with a structure of $A \otimes_\mathbf{Z} B^-$-complex. All the definitions and properties stated in the preceding numbers therefore apply to complexes of bimodules. One defines analogously the complexes of multimodules.

### 10. Example: de Rham complex

In this number, it is assumed that A is a commutative k-algebra over a commutative ring k. We denote by $\Omega^1_{A/k}$ the A-module of k-differentials of A (III, p. 134), $d^0 : A \to \Omega^1_{A/k}$ the k-derivation $d_{A/k}$, and $\Omega_{A/k}$ the graded k-algebra $\Lambda_A(\Omega^1_{A/k})$.

#### Proposition 13 {#alg-x-s2-prop-13 .statement}

There exists a unique k-antiderivation $d : \Omega_{A/k} \to \Omega_{A/k}$ of degree 1, square zero, which extends the derivation $d^0 : A \to \Omega^1_{A/k}$.

Let us prove the uniqueness of the antiderivation d. Since $d \circ d = 0$, one has for $y, x_1, \ldots, x_p \in A$:
$$
d(y dx_1 \wedge \ldots \wedge dx_p) = dy \wedge dx_1 \wedge \ldots \wedge dx_p .
$$
The A-module $\Omega^p_{A/k}$ being generated by the elements $dx_1 \wedge \ldots \wedge dx_p$, this proves the uniqueness of d.

To prove existence, it suffices to construct a $k$-homomorphism $d^1 : \Omega_{A/k}^1 \to \Omega_{A/k}^2$ such that $d^1 \circ d^0 = 0$ and
$$
d^1(a \omega) = d^0(a) \wedge \omega + a d^1(\omega) \quad \text{for } a \in A , \quad \omega \in \Omega_{A/k}^1 .
$$
Indeed, it then follows from III, p. 128, prop. 14 (taking into account III, p. 118, remark 2) that there exists an antiderivation $d : \Omega_{A/k} \to \Omega_{A/k}$ which coincides with $d^0$ in degree 0 and with $d^1$ in degree 1. Since $d^0$ is zero on $A$, the antiderivation $d$ is $k$-linear; since $d^1 \circ d^0 = 0$, one has $d \circ d = 0$ since $\Omega_{A/k}$ is generated as an $A$-algebra by the elements $d^0 a$ for $a \in A$.

To define $d^1$, let us recall (III, p. 133) that $\Omega_{A/k}^1$ is equal to the $A$-module $\mathfrak{J}/\mathfrak{J}^2$, where $\mathfrak{J}$ is the kernel of the multiplication $m : A \otimes_k A \to A$. Consider the $k$-linear mapping $u : A \otimes_k A \to \Omega_{A/k}^2$ defined by $u(x \otimes y) = d^0(y) \wedge d^0(x)$. We have
$$
u(ax \otimes y - x \otimes ay) = d^0(y) \wedge d^0(ax) - d^0(ay) \wedge d^0(x) = d^0(xy) \wedge d^0(a)
$$
for $x, y$ and $a$ in $A$, whence
$$
u((a \otimes 1 - 1 \otimes a) \xi) = d^0(m(\xi)) \wedge d^0(a) , \quad \xi \in A \otimes_k A , \quad a \in A .
$$
Since $\mathfrak{J}$ is generated as a left $A$-module by the elements $(a \otimes 1 - 1 \otimes a)$ for $a \in A$, we deduce that $u(\mathfrak{J}^2) = 0$; consequently $u$ defines by restriction to $\mathfrak{J}$ and passing to the quotient a $k$-linear mapping $d^1 : \mathfrak{J}/\mathfrak{J}^2 \to \Omega_{A/k}^2$.

By setting $\xi = b \otimes 1$ in (12), with $b \in A$, we obtain $d^1(b d^0(a)) = d^0(b) \wedge d^0(a)$; it follows that $d^1 \circ d^0 = 0$ and that $d^1(c \omega) = d^0(c) \wedge \omega + c d^1(\omega)$ for $c \in A$ and $\omega = b d^0(a)$. Since $\Omega_{A/k}^1$ is generated as a $k$-module by the elements $b d^0(a)$, for $a$ and $b$ in $A$, formula (11) is satisfied for all $\omega \in \Omega_{A/k}$, which completes the proof of the proposition.

One sometimes says that the elements $\omega \in \Omega_{A/k}^p$ are the *exterior differential forms of degree* $p$ of $A$ over $k$, and that the antiderivation $d$ is the *exterior differential* of $\Omega_{A/k}$; the complex $(\Omega_{A/k}, d)$ is called the *de Rham complex of A over k*, and its homology is the *de Rham cohomology of A over k*.

#### Example 1 {#alg-x-s2-n10-exa-1 .statement}

Take $A$ to be the ring $k[X_1, ..., X_n]$. Then $\Omega_{A/k}^1$ is a free $A$-module with basis $dX_1, ..., dX_n$ (III, p. 134, example). Consequently, if, for every subset $I = \{ i_1, ..., i_p \}$ of $\{ 1, n \}$, one sets $dX_I = dX_{i_1} \wedge ... \wedge dX_{i_p}$ (with $i_1 < ... < i_p$), the $A$-module $\Omega_{A/k}^p$ admits as basis the elements $dX_I$, where $I$ runs through the set of subsets of $\{ 1, n \}$ of cardinal $p$. One has
$$
d(P dX_I) = dP \wedge dX_I = \sum_{i \notin I} (-1)^{n(I,i)} \frac{\partial P}{\partial X_i} dX_{I \cup \{ i \}} ,
$$
where $n(I, i)$ denotes the number of elements of $I$ strictly less than $i$.

The cycles of $Z^p(\Omega_{A/k})$ are therefore the elements $\omega = \sum_{\operatorname{Card}(I) = p} P_I dX_I$ such that, for every subset $J$ with $(p + 1)$ elements of $\{ 1, n \}$, one has:
$$
\sum_{i \in J} (-1)^{n(J,i)} \frac{\partial P_{J-\{i\}}}{\partial X_i} = 0 .
$$

The element $\omega$ is a boundary if one can choose, for every subset $J \subset \{1, n\}$ with $(p - 1)$ elements, a polynomial $Q_J \in A$ in such a way that:

$$
P_I = \sum_{j \in I} (-1)^{n(I,j)} \frac{\partial Q_{I-\{j\}}}{\partial X_j}.
$$

We shall see in § 9 that the de Rham complex of $A$ over $k$ is acyclic in degrees $> 0$ if $k$ is a $\mathbf{Q}$-algebra (X, p. 159, *remark 4*).

#### Example 2 {#alg-x-s2-n10-exa-2 .statement}

Suppose that $k = \mathbf{C}$ and $A = \mathbf{C} [X_1, ..., X_n]/(P_1, ..., P_r)$, where the $P_i$ are polynomials in $X_1, ..., X_n$, such that the set of points of $\mathbf{C}^n$ where all the $P_i$ vanish is an analytic subvariety $V$ of $\mathbf{C}^n$. One can show that the de Rham cohomology of $A$ over $\mathbf{C}$ is isomorphic to the *singular cohomology* $H(V, \mathbf{C})$.

Let now $M$ be an $A$-module and $\nabla^0$ a $k$-linear mapping from $M$ into $M \otimes_A \Omega^1_{A/k}$ such that

$$(13)$$
$$
\nabla^0(am) = a \nabla^0(m) + m \otimes da \quad \text{for} \quad a \in A,\ m \in M
$$
(one sometimes says that $\nabla^0$ is a *connection* on the $A$-module $M$).

#### Proposition 14 {#alg-x-s2-prop-14 .statement}

(i) *There exists a unique mapping $k$-linéaire $\nabla$ from the right $\Omega_{A/k}$-module $M \otimes_A \Omega_{A/k}$ into itself, graded of degree 1, which extends $\nabla^0$ in degree 0 and satisfies the identity* :

$$(14)$$
$$
\nabla(x \omega) = (\nabla x) \omega + (-1)^p x(d\omega) \quad \text{for} \quad x \in M \otimes_A \Omega^p_{A/k},\ \omega \in \Omega_{A/k}.
$$

(ii) *The composite mapping $\nabla \circ \nabla$ is $\Omega_{A/k}$-linéaire ; in particular the mapping $R = \nabla^1 \circ \nabla^0$ from $M$ into $M \otimes_A \Omega^2_{A/k}$ is $A$-linéaire, and we have*
$$
\nabla \circ \nabla(m \otimes \omega) = R(m).\omega \quad \text{for} \quad m \in M,\ \omega \in \Omega_{A/k}.
$$

The homomorphism $R$ is sometimes called *curvature homomorphism* of the connection $\nabla^0$; if it is zero, the pair $(M \otimes_A \Omega_{A/k}, \nabla)$ is a complex, also called *de Rham complex of* $(M, \nabla^0)$ *over* $k$.

Let us prove (i). The uniqueness of $\nabla$ is obvious. Let us define a $k$-homomorphisme $\overline{\nabla}$ from $M \otimes_k \Omega_{A/k}$ into $M \otimes_A \Omega_{A/k}$ by
$$
\overline{\nabla}(m \otimes_k \omega) = (\nabla^0 m) \omega + m \otimes d\omega \quad \text{for} \quad m \in M,\ \omega \in \Omega_{A/k}.
$$

It follows from (13) that $\overline{\nabla}(am \otimes \omega) = \overline{\nabla}(m \otimes a \omega)$, so that one obtains by passing to the quotient a $k$-homomorphisme $\nabla$ from $M \otimes_A \Omega_{A/k}$ into itself, graded of degree 1, extending $\nabla^0$ in degree 0. Let us verify (14): we have for $m \in M$, $\alpha \in \Omega^p_{A/k}$, $\omega \in \Omega_{A/k}$ :
$$
\begin{align*}
\nabla((m \otimes \alpha).\omega) &= \nabla(m \otimes (\alpha \wedge \omega)) = \nabla^0(m).(\alpha \wedge \omega) + m \otimes d(\alpha \wedge \omega) \\
&= \nabla^0(m) \alpha.\omega + (m \otimes d\alpha) \omega + (-1)^p (m \otimes \alpha) d\omega \\
&= (\nabla(m \otimes \alpha)) \omega + (-1)^p (m \otimes \alpha) d\omega
\end{align*}
$$
which proves (14) for $x = m \otimes \alpha$; the general case follows by linearity.

Let us prove (ii). Let $x \in M \otimes_A \Omega_{A/k}^p, \omega \in \Omega_{A/k}$; by repeated application of (14), we obtain :
$$
\nabla \circ \nabla(x \omega) = \nabla(\nabla(x) \omega) + (-1)^p \nabla(x d \omega)
= (\nabla \circ \nabla(x)) \omega + (-1)^{p+1} \nabla(x)(d \omega) + (-1)^p \nabla(x)(d \omega)
= (\nabla \circ \nabla(x)) \omega,
$$
which proves the first assertion of (ii); the others follow immediately.

## EXERCISES {#alg-x-s2-exercises}

See the [exercises for § 2](exercises/s2/).
