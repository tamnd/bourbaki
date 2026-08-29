---
book: ta
book_title: Topologie algébrique
chapter: I
chapter_title: REVÊTEMENTS
section: 3
section_title: Faisceaux
lang: en
source: ta-i-iv-fr
book_pages: TA I.42-TA I.67, TA I.141-TA I.145
pdf_pages: 0058-0083, 0157-0161
extraction: native
subsections:
    - "no": 1
      title: Faisceaux d’ensembles
      page: 42
      pdf_page: 58
    - "no": 2
      title: Sous-faisceaux d’un faisceau
      page: 44
      pdf_page: 60
    - "no": 3
      title: Exemples de faisceaux
      page: 44
      pdf_page: 60
    - "no": 4
      title: Morphismes de préfaisceaux
      page: 47
      pdf_page: 63
    - "no": 5
      title: Espace étalé associé à un préfaisceau
      page: 49
      pdf_page: 65
    - "no": 6
      title: Faisceau associé à un préfaisceau
      page: 53
      pdf_page: 69
    - "no": 7
      title: Image directe et image réciproque d’un faisceau
      page: 57
      pdf_page: 73
    - "no": 8
      title: Les homomorphismes $\alpha \mathbf{e}\mathbf{t}\beta$ ; adjonction
      page: 59
      pdf_page: 75
    - "no": 9
      title: Faisceaux mous
      page: 64
      pdf_page: 80
    - "no": 10
      title: Faisceaux de structures
      page: 66
      pdf_page: 82
statements: 35
exercises: 8
content_sha256: 52992bda508a3c0caa17b47af125817ccd2a2bd8f51eb6448ce1d4cae22b17ce
translated_from: content/fr/ta/I/03_s3_faisceaux.md
source_lang: fr
translation_method: machine
source_content_sha256: 2a2b4e862e0b46c186780988a45a46e15762355de71591c7cad0e6b27bacb572
translation_model: gpt-5.4, gpt-5-6-mini, gpt-5-mini
translation_run: translate-en-mt-20bb7a26
glossary_version: 34
glossary_terms_sha256: 2ee79725379082d200f4a61851ad2dbd88a173c42ba5f48d60ee203d272771fa
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 3. SHEAVES

### 1. Sheaves of sets

Let B be a topological space.

#### Definition 1 {#ta-i-s3-def-1 .statement tag=01NS}

A presheaf on B, relative to a basis $\mathscr{B}$ of the topology of B, is a projective system of sets, relative to the set of indices $\mathscr{B}$ ordered by the inclusion relation.

In other words (E, III, p. 52), a presheaf $\mathscr{F}$ on B relative to $\mathscr{B}$ is a pair $((\mathscr{F}(U))_{U\in\mathscr{B}},(f_{UV}))$, which is also denoted by $(\mathscr{F}(U), f_{UV})$, where $((\mathscr{F}(U))_{U\in\mathscr{B}}$ is a family of sets having $\mathscr{B}$ as set of indices and where for each pair $(U,V)$ of elements of $\mathscr{B}$ such that $U\subset V,f_{UV}$ is a mapping of $\mathscr{F}(V)$ into $\mathscr{F}(U)$, these mappings satisfying the following conditions:

(PF$_1$) The relations $U\subset V\subset W$ imply $f_{UW}=f_{UV}\circ f_{VW}$;

(PF$_2$) For every open set U $\in \mathscr{B},f_{UU}$ is the identity mapping of

$$
\mathscr{F}(U)
$$

A presheaf on B relative to the set of open subsets of B is simply called a presheaf on B.

Let $\mathscr{F}= (\mathscr{F}(U), f_{UV})$ be a presheaf on B, relative to a basis $\mathscr{B}$ of the topology of B. Let U be an element of the basis $\mathscr{B}$. The elements of $\mathscr{F}(U)$ are called the sections of $\mathscr{F}$ over U. If V is an element of the basis $\mathscr{B}$ containing U and $s$ an element of $\mathscr{F}(V)$, the element $f_{UV}(s)$ of $\mathscr{F}(U)$ is called the restriction of $s$ to U. If there is no danger of ambiguity concerning the mappings $f_{UV}$, the restriction of $s$ to U will be denoted by $s|U$.

Let $B'$ be an open subset of B and $\mathscr{B}'$ a basis of the topology of $B'$ such that $\mathscr{B}'\subset \mathscr{B}$. The presheaf on $B'$, relative to $\mathscr{B}'$, deduced from $\mathscr{F}$ by restriction, is called the restriction of $\mathscr{F}$ to $\mathscr{B}'$ and denoted by $\mathscr{F}|\mathscr{B}'$, the projective system $((\mathscr{F}(U))_{U\in\mathscr{B}'},(f_{UV}))$ deduced from $\mathscr{F}$ by restriction to $\mathscr{B}'$ of the set of indices (loc. cit.). When $\mathscr{F}$ is a presheaf on B and $\mathscr{B}'$ is the set of open subsets of $B'$, the presheaf $\mathscr{F}|\mathscr{B}'$ is also denoted by $\mathscr{F}|B'$ and called the presheaf deduced from $\mathscr{F}$ by restriction to $B'$.

#### Definition 2 {#ta-i-s3-def-2 .statement tag=01NT}

Let $\mathscr{F}= (\mathscr{F}(U), f_{UV})$ be a presheaf on B. One says that $\mathscr{F}$ is a sheaf on B if, for every open subset U of B and every family $(U_i)_{i\in I}$ of open subsets of B, with union U, the following properties are satisfied:

$(F_1)$ The mapping $(f_{U_iU})_{i\in I}:\mathscr{F}(U)\rightarrow \prod_{i\in I}\mathscr{F}(U_i)$ is injective ;

$(F_2)$ For every family $(s_i)\in \prod_{i\in I}\mathscr{F}(U_i)$ such that $f_{(U_i\cap U_j)U_i}(s_i) =$

$f_{(U_i\cap U_j)U_j}(s_j)$ for every pair $(i, j)\in I\times I$, there exists an element $s$

of $\mathscr{F}(U)$ such that for every $i\in I$, one has $f_{U_iU}(s) =s_i$.

#### Remark {#ta-i-s3-n1-rem-1 .statement tag=01NU}

Let $\mathscr{F}$ be a presheaf on B. For every open set U of B, $f_{\emptyset U}$ is a map of $\mathscr{F}(U)$ into $\mathscr{F}(\emptyset )$, hence $\mathscr{F}(\emptyset )$ is not empty as soon as there exists an open set U for which $\mathscr{F}(U)$ is not empty. If $\mathscr{F}$ is a sheaf, $\mathscr{F}(\emptyset )$ is a one-element set; this is seen by applying $(F_1)$ and $(F_2)$ to the covering of the empty set by the empty family ($I =\emptyset$ ).

Let $\mathscr{F}$ be a sheaf on B and let $B'$ be an open subset of B; the presheaf $\mathscr{F}|B'$ deduced from $\mathscr{F}$ by restriction to $B'$ is a sheaf, called the sheaf deduced from $\mathscr{F}$ by restriction to $B'$.

### 2. Subsheaves of a Sheaf

Let B be a topological space. Let $\mathscr{F}= (\mathscr{F}(U), f_{UV})$ be a presheaf on B, relative to a basis $\mathscr{B}$ of the topology of B.

Suppose given, for every open set $U\in \mathscr{B}$, a subset $\mathscr{L}(U)$ of $\mathscr{F}(U)$. If one has $f_{UV}(\mathscr{L}(V))\subset \mathscr{L}(U)$ for every pair $(U,V)$ of elements of $\mathscr{B}$ such that $U\subset V$, the pair $\mathscr{L}= ((\mathscr{L}(U))_{U\in\mathscr{B}},(f'_{UV}))$, where $f'_{UV}:\mathscr{L}(V)\rightarrow \mathscr{L}(U)$ is the map deduced from $f_{UV}$, is a presheaf. Such a presheaf is called a sub-presheaf of $\mathscr{F}$. Since the maps $f'_{UV}$ are determined by the given presheaf $\mathscr{F}$ and the family $(\mathscr{L}(U))_{U\in\mathscr{B}}$, one also says, by abuse of language, that the family $(\mathscr{L}(U))_{U\in\mathscr{B}}$ is a sub-presheaf of $\mathscr{F}$.

Suppose now that $\mathscr{F}$ is a sheaf on B and let, for every open subset U of B$,\mathscr{L}(U)$, a subset of $\mathscr{F}(U)$. In order that $(\mathscr{L}(U))_{U\in\mathscr{B}}$ be a sub-presheaf of $\mathscr{F}$, and that this presheaf be a sheaf, it is necessary and sufficient that the following condition be satisfied:

(F) Let $(U_i)_{i\in I}$ be a family of open sets of B, U its union, and $s$ an

element of $\mathscr{F}(U)$. In order that $s$ belong to $\mathscr{L}(U)$, it is necessary and

sufficient that for every $i$ in I$,f_{U_iU}(s)$ belong to $\mathscr{L}(U_i)$.

Indeed, if condition (F) is satisfied, one has $f_{UV}(\mathscr{L}(V))\subset \mathscr{L}(U)$ for every pair $(U,V)$ of open sets of B such that $U\subset V$ and the properties $(F_1)$ and $(F_2)$ relative to the subpresheaf $(\mathscr{L}(U))$ result from the analogous properties relative to the sheaf $\mathscr{F}$. The converse is immediate.

When condition (F) is satisfied, one says that $(\mathscr{L}(U))$ is a subsheaf of the sheaf $\mathscr{F}$.

### 3. Examples of sheaves

Let B be a topological space.

1) Sheaves of mappings

Let X be a set. For every open set U of B, denote by $\mathscr{F}(U; X)$ the set of mappings from U into X (E, II, p. 31). For every pair $(U,V)$ of open sets of B such that $U\subset V$, let $r_{UV}:\mathscr{F}(V; X)\rightarrow$ $\mathscr{F}(U; X)$ be the restriction mapping $f\mapsto f|U$. It is clear that the pair $(\mathscr{F}(U; X), r_{UV})$ is a sheaf on B. It is called the sheaf on B of mappings with values in X, and is denoted by $\mathscr{F}(B; X)$.

2) Sheaves of continuous mappings

Let X be a topological space. For every open set U of B, let $\mathscr{C}(U; X)$ be the set of continuous mappings from U into X. Then, $(\mathscr{C}(U; X))$ is a subsheaf of the sheaf $\mathscr{F}(B; X)$ by prop. 4 of TG, I, p. 19. The sheaf thus obtained is denoted by $\mathscr{C}(B; X)$ and called the sheaf on B of continuous mappings with values in X. In the particular case where X is endowed with the discrete topology, the sheaf $\mathscr{C}(B; X)$ takes the name of sheaf on B of locally constant mappings with values in X.

3) Sheaves of continuous sections

Let E be a topological space and let $p: E\rightarrow B$ be a continuous mapping. For every open set U of B, denote by $\mathscr{S}(U;p)$ (or $\mathscr{S}(U; E)$ when there is no possible confusion) the set of continuous sections of $p$ above U. The family $(\mathscr{S}(U;p))$ is a subsheaf of the sheaf $\mathscr{C}(B; E)$. The sheaf thus obtained is denoted by $\mathscr{S}(B; E)$ or simply $\mathscr{S}(E)$ and called the sheaf on B of continuous sections of the B-space $(E, p)$. We shall see in no$^o6$ below that every sheaf on B is isomorphic to the sheaf on B of continuous sections of an étalé B-space.

4) Sheaves of B-morphisms

Let $(E, p)$ and $(E', p')$ be B-spaces. For every open set U of E, denote by $\mathscr{C}_B(U; E')$ the set of B-morphisms from $(U, p|U)$ into $(E', p')$. The family $(\mathscr{C}_B(U; E'))$ is a subsheaf of the sheaf $\mathscr{C}(E; E')$. The sheaf thus obtained is denoted by $\mathscr{C}_B(E; E')$ and called the sheaf on E of B-morphisms with values in $(E', p')$. When $(E, p)$ is equal to $(B$, Id$_B)$, this sheaf is the sheaf $\mathscr{S}(B; E)$ of example 3.

For every open set U of B, let $\mathscr{M}(U)$ be the set of U-morphisms

from $\overset{-1}{p}(U)$ into $(^-{p'}^1)(U)$. For every pair $(U,V)$ of open sets of B such that $U\subset V$, let $m_{UV}:\mathscr{M}(V)\rightarrow \mathscr{M}(U)$ be the mapping which to a V-morphism

$f:\overset{-1}{p}(V)\rightarrow (^-{p'}^1)(V)$ associates the U-morphism from $\overset{-1}{p}(U)$ into $(^-{p'}^1)(U)$ deduced from $f$ by passing to the subsets. Then $(\mathscr{M}(U), m_{UV})$ is a sheaf on B. It is denoted by $\mathscr{M}$or$_B(E; E')$ and is called the sheaf on B of B-morphisms from $(E, p)$ into $(E', p')$.

For every open set U of B, let $\mathscr{I}$s(U) be the subset of $\mathscr{M}(U)$

consisting of the U-isomorphisms of $\overset{-1}{p}(U)$ into $(^-{p'}^1)(U)$. The family $(\mathscr{I}$s(U)) is a sub-sheaf of the sheaf $\mathscr{M}$or$_B(E; E')$ of morphisms from $(E, p)$ into $(E', p')$. The sheaf thus obtained is denoted $\mathscr{I}$som$_B(E; E')$ and is called the sheaf on B of B-isomorphisms from $(E, p)$ into $(E', p')$.

5) Sheaves of mappings of class $C^r$

Let X and Y be manifolds of class $C^r$ over a field K (the conventions concerning K and $r$ being those of VAR, R). For every open set U of X, let $\mathscr{C}^r(U; Y)$ be the set of morphisms of class $C^r$ from U into Y. The family $(\mathscr{C}^r(U; Y))$ is a sub-sheaf of the sheaf $\mathscr{C}(X; Y)$. The sheaf thus obtained is denoted $\mathscr{C}^r(X; Y)$ and is called the sheaf on X of mappings of class $C^r$ with values in Y (cf. VAR, R, 5.4.2).

6) Sheaves of subspaces

If U and V are open sets of B such that $U\subset V$, denote by $i_{UV}:\mathfrak{P}(V)\rightarrow$ $\mathfrak{P}(U)$ the mapping which, to a subset A of V, associates $A\cap U$. The pair $(\mathfrak{P}(U), i_{UV})$ is a sheaf, called the sheaf of subspaces of B and denoted $\mathfrak{P}(B)$. Indeed, if X denotes the set $\{0; 1\}$, the mapping which associates to every subset A of U its characteristic function $\varphi^U_A: U\rightarrow X$ is a bijection of $\mathfrak{P}(U)$ onto $\mathscr{F}(U; X)$ (E, III, p. 38) ; moreover, if U and V are open sets such that $U\subset V$, for every subset A of V$,\varphi^U_{A\cap U}$ is the restriction to U of $\varphi^V_A$ so that $\mathfrak{P}(B)$ is identified with the sheaf on B of mappings with values in X.

Let, for every open set U of B$,\mathscr{L}(U)$ be a subset of $\mathfrak{P}(U)$. In order that $(\mathscr{L}(U))$ be a sub-sheaf of $\mathfrak{P}(B)$, it is necessary and sufficient that the following condition be satisfied:

$(F')$ Let $(U_i)_{i\in I}$ be a family of open sets of B, U its union, and A a

subset of U ; in order that A belong to $\mathscr{L}(U)$, it is necessary and

sufficient that for every $i$ in I, $A\cap U_i$ belong to $\mathscr{L}(U_i)$.

For example, if $\mathscr{L}(U)$ is the set of closed subsets of U, condition $(F')$ is satisfied.

7) Products of sheaves

Let $\mathscr{B}$ be a basis of the topology of B and let I be a set. For every $i\in I$, let $\mathscr{F}_i= (\mathscr{F}_i(U), f_{i,UV})$ be a presheaf on B relative to the basis $\mathscr{B}$. For every open set $U\in \mathscr{B}$, put $\mathscr{F}(U) =\prod_{i\in I}\mathscr{F}_i(U)$, and for every pair $(U,V)$ of elements of $\mathscr{B}$ such that $U\subset V$, denote by $f_{UV}$ the mapping $(f_{i,UV})_{i\in I}:\mathscr{F}(V)\rightarrow \mathscr{F}(U)$. Then $(\mathscr{F}(U), f_{UV})$ is a presheaf on B relative to $\mathscr{B}$ called the product presheaf of the family $(\mathscr{F}_i)$ and denoted $\prod_{i\in I}\mathscr{F}_i$. It is a sheaf if for every $i\in I,\mathscr{F}_i$ is a sheaf.

### 4. Morphisms of presheaves

#### Definition 3 {#ta-i-s3-def-3 .statement tag=01NV}

Let B be a topological space, $\mathscr{B}$ a basis of the topology of B$,\mathscr{F}= (\mathscr{F}(U), f_{UV})$ and $\mathscr{G}= (\mathscr{G}(U), g_{UV})$ presheaves on B relative to $\mathscr{B}$. A morphism of presheaves from $\mathscr{F}$ to $\mathscr{G}$ is called a projective system of mappings from $\mathscr{F}$ to $\mathscr{G}$.

In other words (E, III, p. 54), a morphism of presheaves from $\mathscr{F}$ to $\mathscr{G}$ is a family $(\varphi_U)_{U\in\mathscr{B}}$ such that :

(MPF$_1$) For every open set U belonging to $\mathscr{B},\varphi_U$ is a mapping

from $\mathscr{F}(U)$ into $\mathscr{G}(U)$ ;

(MPF$_2$) For every pair $(U,V)$ of open sets belonging to $\mathscr{B}$ such that

$U\subset V$, one has $\varphi_U\circ f_{UV}=g_{UV}\circ \varphi_V$.

When $\mathscr{F}$ and $\mathscr{G}$ are sheaves, a morphism of presheaves from $\mathscr{F}$ to $\mathscr{G}$ is also called a morphism of sheaves. If $\mathscr{F}$ and $\mathscr{G}$ are presheaves on B relative to $\mathscr{B}$, the morphisms of presheaves from $\mathscr{F}$ to $\mathscr{G}$ constitute a set denoted Mor($\mathscr{F};\mathscr{G}$). Instead of saying : “let $\varphi$ be a morphism of presheaves from $\mathscr{F}$ to $\mathscr{G}$”, one will often say “let $\varphi :\mathscr{F}\rightarrow \mathscr{G}$ be a morphism of presheaves”.

Let $\mathscr{F},\mathscr{G},\mathscr{H}$ be presheaves on B relative to $\mathscr{B}$ and let $\varphi :\mathscr{F}\rightarrow \mathscr{G}$, $\psi :\mathscr{G}\rightarrow \mathscr{H}$ be morphisms of presheaves. The family $(\psi_U\circ \varphi_U)_{U\in\mathscr{B}}$ is a morphism of presheaves from $\mathscr{F}$ into $\mathscr{H}$ which is denoted by $\psi \circ \varphi$. The family (Id$_{\mathscr{F}(U)}$)$_{U\in\mathscr{B}}$ is a morphism of presheaves from $\mathscr{F}$ into itself which is denoted by Id$_{\mathscr{F}}$.

For a morphism of presheaves $\varphi = (\varphi_U):\mathscr{F}\rightarrow \mathscr{G}$ to be an isomorphism, it is necessary and sufficient that, for every open subset U of $\mathscr{B},\varphi_U$ be a bijection from $\mathscr{F}(U)$ onto $\mathscr{G}(U)$. It is equivalent to saying that there exists a morphism of presheaves $\psi :\mathscr{G}\rightarrow \mathscr{F}$ such that $\psi \circ \varphi =$ Id$_{\mathscr{F}}$ and $\varphi \circ \psi =$ Id$_{\mathscr{G}}$.

Let $\mathscr{F}$ and $\mathscr{G}$ be presheaves on B, relative to a base $\mathscr{B}$ of the topology of B, let $B'$ be an open subset of B and let $\mathscr{B}'$ be a base of the topology of $B'$ such that $\mathscr{B}'\subset \mathscr{B}$. Let $\varphi = (\varphi_U)_{U\in\mathscr{B}}$ be a morphism of presheaves from $\mathscr{F}$ into $\mathscr{G}$. Then $(\varphi_U)_{U\in\mathscr{B}'}$ is a morphism of presheaves from $\mathscr{F}|\mathscr{B}'$ into $\mathscr{G}|\mathscr{B}'$, which is denoted by $\varphi |\mathscr{B}'$. When $\mathscr{B}$ is the set of open subsets of B and $\mathscr{B}'$ the set of open subsets of $B',\varphi |\mathscr{B}'$ is a morphism of presheaves from $\mathscr{F}|B'$ into $\mathscr{G}|B'$ and is also denoted by $\varphi |B'$.

#### Example 1 {#ta-i-s3-n4-exa-1 .statement tag=01NW}

Let B be a topological space, let $(E, p)$ and $(E', p')$ be B-spaces and let $f: E\rightarrow E'$ be a B-morphism. For every open subset U of B, define the mapping $f_U:\mathscr{S}(U; E)\rightarrow \mathscr{S}(U; E')$ by $f_U(s) =$ $f\circ s$. The family $\mathscr{S}(f) = (f_U)$ is a morphism of presheaves from $\mathscr{S}(B; E)$ into $\mathscr{S}(B; E')$. If $(E'', p'')$ is a B-space and $g: E'\rightarrow E''$ is a B-morphism, one has $\mathscr{S}(g\circ f) =\mathscr{S}(g)\circ \mathscr{S}(f)$.

#### Example 2 {#ta-i-s3-n4-exa-2 .statement tag=01NX}

Let B be a topological space, $\mathscr{B}$ a basis of the topology of B, $\mathscr{F}= (\mathscr{F}(U), f_{UV})$ a presheaf on B relative to $\mathscr{B}$ and $\mathscr{L}= (\mathscr{L}(U))$ a subpresheaf of $\mathscr{F}$. For every open set $U\in \mathscr{B}$, denote by $i_U$ the canonical injection of $\mathscr{L}(U)$ into $\mathscr{F}(U)$. Then $i= (i_U)_{U\in\mathscr{B}}$ is a morphism of presheaves from $\mathscr{L}$ into $\mathscr{F}$. We say that $i$ is the canonical morphism from $\mathscr{L}$ into $\mathscr{F}$.

#### Example 3 {#ta-i-s3-n4-exa-3 .statement tag=01NY}

Let B be a topological space, $\mathscr{B}$ a basis of the topology of B and I a set. For every $i\in I$, let $\mathscr{F}_i= (\mathscr{F}_i(U), f_{i,UV})$ be a presheaf on B relative to $\mathscr{B}$. Denote by $\mathscr{F}$ the product presheaf of the family $(\mathscr{F}_i)_{i\in I}$. For every open set $U\in \mathscr{B}$, one has $\mathscr{F}(U) =\prod_{i\in I}\mathscr{F}_i(U)$; for every $i\in I$, denote by pr$_{i,U}:\mathscr{F}(U)\rightarrow \mathscr{F}_i(U)$ the projection of index $i$. It follows immediately from the definition of the presheaf $\mathscr{F}$ that the family pr$_i$ = (pr$_{i,U}$)$_{U\in\mathscr{B}}$ is a morphism of presheaves from $\mathscr{F}$ into $\mathscr{F}_i$. The morphism pr$_i$ is called the projection morphism of index $i$. For every presheaf $\mathscr{F}'$ on B relative to $\mathscr{B}$ and every family $(\psi_i)_{i\in I}$, where $\psi_i$ is a morphism of presheaves from $\mathscr{F}'$ into $\mathscr{F}_i$, there exists a unique morphism of presheaves $\psi :\mathscr{F}'\rightarrow \mathscr{F}$ such that for every $i\in I$, pr$_i\circ \psi =\psi_i$.

#### Example 4 {#ta-i-s3-n4-exa-4 .statement tag=01NZ}

Let X be a differential manifold of class $C^{\infty}$ over $\mathbf{R}$ and let $\mathscr{C}^{\infty}(X;\mathbf{R})$ be the sheaf on X of numerical functions of class $C^{\infty}$. If P is a differential operator with $C^{\infty}$ coefficients on X, the family of the restrictions of P to the open sets of X is a morphism of the sheaf $\mathscr{C}^{\infty}(X;\mathbf{R})$ into itself. One can prove that conversely, every $\mathbf{R}$-linear morphism of the sheaf $\mathscr{C}^{\infty}(X;\mathbf{R})$ into itself is locally of this form (I, p. 142, exerc. 3).

### 5. Étale space associated with a presheaf

Let B be a topological space, $\mathscr{B}$ a basis of the topology of B and $\mathscr{F}= (\mathscr{F}(U), r_{UV})$ a presheaf on B relative to the basis $\mathscr{B}$. Let L be the set of couples $(U, s)$ with U $\in \mathscr{B}$ and $s\in \mathscr{F}(U)$. Let $X_{\mathscr{F}}$ denote the sum space of the family $(U)_{(U,s)\in L}$. Thus $X_{\mathscr{F}}$ is the set of triples $(U, s, x)$ where $U\in \mathscr{B},s\in \mathscr{F}(U),x\in U$. Let $R_{\mathscr{F}}$ be the relation in the set $X_{\mathscr{F}}$ defined by $R_{\mathscr{F}}((U, s, x),(U', s', x'))$ if and only if « $x$ = $x'$ and there exists W $\in \mathscr{B}$ such that $x\in W$, W $\subset U\cap U'$ and $r_{WU}(s) =r_{WU'}(s')$ ». The relation $R_{\mathscr{F}}$ is an equivalence relation in $X_{\mathscr{F}}:$ it is, by definition, reflexive and symmetric; let us prove that it is transitive. Let $\xi = (U, s, x),\xi '= (U', s', x')$ and $\xi ''$ = $(U'', s'', x'')$ be elements of $X_{\mathscr{F}}$ such that one has $R_{\mathscr{F}}(\xi , \xi ')$ and $R_{\mathscr{F}}(\xi ', \xi '')$. We then have $x=x'$ = $x''$ and there exist two elements $W'$ and $W''$ of $\mathscr{B}$ containing $x$ such that $W'\subset U\cap U',W''\subset U'\cap U'',r_{W'U}(s) =$ $r_{W'U'}(s'),r_{W''U'}(s') =r_{W''U''}(s'')$. Let W be an element of $\mathscr{B}$ containing $x$ and contained in $W'\cap W''$. We then have $W\subset U\cap U''$,

$$
r_{WU}(s) =r_{WW'}\circ r_{W'U}(s) =r_{WW'}\circ r_{W'U'}(s') =r_{WU'}(s')
$$

and, analogously, $r_{WU'}(s') =r_{WU''}(s'')$. Consequently, we have $R_{\mathscr{F}}(\xi , \xi '')$ and the relation $R_{\mathscr{F}}$ is transitive.

Let $E_{\mathscr{F}}$ denote the quotient set $X_{\mathscr{F}}/R_{\mathscr{F}}$ and $[U, s, x]$ the canonical image in $E_{\mathscr{F}}$ of an element $(U, s, x)$ of $X_{\mathscr{F}}$. For $U\in \mathscr{B}$ and $s\in \mathscr{F}(U)$, let $\sigma_{\mathscr{F}}(U, s): U\rightarrow E_{\mathscr{F}}$ denote the mapping $x\mapsto [U, s, x]$. Endow the set $E_{\mathscr{F}}$ with the quotient topology, that is, the finest topology for which the mappings $\sigma_{\mathscr{F}}(U, s)$ for $U\in \mathscr{B}$ and $s\in \mathscr{F}(U)$ are continuous. The mapping pr$_3: X_{\mathscr{F}}\rightarrow B$ defines, after passing to the quotient, a continuous mapping $p: E_{\mathscr{F}}\rightarrow B$ : one has $p([U, s, x]) =x$.

#### Proposition 1 {#ta-i-s3-prop-1 .statement tag=01O0}

The mapping $p: E_{\mathscr{F}}\rightarrow$ B is etale. For every open set $U\in \mathscr{B}$ and every $s\in \mathscr{F}(U)$, the mapping $\sigma_{\mathscr{F}}(U, s)$ is therefore a continuous section of $p$ over U.

Let $\lambda = (U, s)$ and $\mu= (U', s')$ be elements of L. By definition of the relation $R_{\mathscr{F}}$, the set $A_{\lambda \mu}$ of points $x$ of $U\cap U'$ at which $\sigma_{\mathscr{F}}(U, s)$ and $\sigma_{\mathscr{F}}(U', s')$ coincide is the interior in B, of the set of $x\in U\cap U'$ such that $s(x) =s'(x)$. It follows that $A_{\mu\lambda}= A_{\lambda \mu}$. We then denote by $h_{\mu\lambda}: A_{\lambda \mu}\rightarrow A_{\mu\lambda}$ the mapping Id$_{A_{\lambda \mu}}$. The set $E_{\mathscr{F}}$ is obtained by gluing together the open sets U along the $A_{\lambda \mu}$ by means of the bijections $h_{\mu\lambda}$ (TG, I, p. 16). By prop. 9 of TG, I, p. 17, the mapping $\sigma_{\mathscr{F}}(U, s)$ induces a homeomorphism of U onto an open subset of $E_{\mathscr{F}}$. This proves that the mapping $p$ is etale (I, p. 33, prop 9).

For every open set $U\in \mathscr{B}$ and every $s\in \mathscr{F}(U)$, one has $\sigma_{\mathscr{F}}(U, s)(x) =$ $[U, s, x]$ for every $x\in U$. The second assertion therefore follows from the definition of $p$.

#### Definition 4 {#ta-i-s3-def-4 .statement tag=01O1}

The spread B-space $(E_{\mathscr{F}}, p)$ defined above is called the spread B-space associated with the presheaf $\mathscr{F}$. For $x\in B$, the fibre of $E_{\mathscr{F}}$ at $x$ is called the stalk of the presheaf $\mathscr{F}$ at $x$ and is denoted by $\mathscr{F}_x$. For every open set $U\in \mathscr{B}$, every section $s\in \mathscr{F}(U)$ of $\mathscr{F}$ over U and every point $x$ of U, the element $[U, s, x]$ of $E_{\mathscr{F}}$ is called the germ at $x$ of the section $s$.

Let $a$ be a point of B. The set $\mathscr{B}(a)$ of open sets $U\in \mathscr{B}$ containing $a$ and ordered by the relation $\supset$ is filtering. From $\mathscr{F}$ one deduces, by restriction of the set of indices to $\mathscr{B}(a)$, an inductive system $((\mathscr{F}(U))_{U\in\mathscr{B}(a)},(r_{UV}))$. By definition (E, III, p. 60), the inductive limit of this system is the quotient of the set of pairs $(U, s)$ such that $a\in U$ and $s\in \mathscr{F}(U)$ by the equivalence relation R defined by $R((U, s),(U', s'))$ if and only if there exists W $\in \mathscr{B}$ containing $a$ and contained in $U\cap U'$ and such that $r_{WU}(s) =r_{WU'}(s')$. This limit is therefore identified with the stalk $\mathscr{F}_a$ of $\mathscr{F}$ at $a$, by definition of inductive limits.

Let $\mathscr{G}$ be a presheaf on B relative to the basis $\mathscr{B}$ and let $\varphi = (\varphi_U)_{U\in\mathscr{B}}$ be a morphism of presheaves from $\mathscr{F}$ into $\mathscr{G}$. The mapping $(U, s, x)\mapsto$ $(U, \varphi_U(s), x)$ from $X_{\mathscr{F}}$ into $X_{\mathscr{G}}$ is compatible with the equivalence relations $R_{\mathscr{F}}$ and $R_{\mathscr{G}}$, by definition of a morphism of presheaves. Let us denote by $E(\varphi ): E_{\mathscr{F}}\rightarrow E_{\mathscr{G}}$ the mapping deduced from it by passing to the quotients. For every $U\in \mathscr{B}$ and every $s\in \mathscr{F}(U)$, we have

$$
E(\varphi )\circ \sigma_{\mathscr{F}}(U, s) =\sigma_{\mathscr{G}}(U, \varphi_U(s))
$$

consequently, the mapping $E(\varphi )$ is continuous. The mapping $E(\varphi )$ is a B-morphism; it is said to be the B-morphism of $E_{\mathscr{F}}$ into $E_{\mathscr{G}}$ associated with the morphism of presheaves $\varphi$. For every $a\in B$, by restriction to the fibres at $a$, $E(\varphi )$ defines a mapping of the stalk $\mathscr{F}_a$ of $\mathscr{F}$ into the stalk $\mathscr{G}_a$ of $\mathscr{G}$; it is denoted by $\varphi_a$. It is also the inductive limit of the mappings $\varphi_U$ (E, III, p. 63), where U ranges over the set $\mathscr{B}(a)$ of open sets belonging to the base $\mathscr{B}$ and containing $a$.

We have E(Id$_{\mathscr{F}}$) $=$ Id$_{E_{\mathscr{F}}}$.

Let $\mathscr{H}$ be a presheaf on B relative to $\mathscr{B}$ and let $\psi = (\psi_U)$ be a morphism of presheaves from $\mathscr{G}$ into $\mathscr{H}$. For $[U, s, x]\in E_{\mathscr{F}}$, we have

$$
E(\psi \circ \varphi )([U, s, x]) = [U, \psi_U\circ \varphi_U(s), x]
$$

$$
= E(\psi )([U, \varphi_U(s), x])
$$

$$
= E(\psi )\circ E(\varphi )([U, s, x])
$$

Consequently, we have $E(\psi \circ \varphi ) = E(\psi )\circ E(\varphi )$. In particular, if $a$ is a point of B, $(\psi \circ \varphi )_a=\psi_a\circ \varphi_a$.

If $\varphi$ is an isomorphism, the same is true of $E(\varphi )$.

#### Remark {#ta-i-s3-n5-rem-1 .statement tag=01O2}

Let $\mathscr{F}$ be a sheaf on B relative to the base $\mathscr{B}$. Let $B'$ be an open subset of B, let $\mathscr{B}'$ be a basis of the topology of $B'$ such that $\mathscr{B}'\subset \mathscr{B}$. Let $\mathscr{F}|\mathscr{B}'$ be the presheaf on $B'$ relative to the base $\mathscr{B}'$ deduced from $\mathscr{F}$ by restriction.

1) The set $X_{\mathscr{F}|\mathscr{B}'}$ is then a subset of $X_{\mathscr{F}}$ and the equivalence relation $R_{\mathscr{F}}$ induces in $X_{\mathscr{F}|\mathscr{B}'}$ the equivalence relation $R_{\mathscr{F}|\mathscr{B}'}$. Hence one deduces a canonical injection $i$ of $E_{\mathscr{F}|\mathscr{B}'}$ into $E_{\mathscr{F}}$. Its image is $\overset{-1}{p}(B')$ since for every element $[U, s, x]$ of $\overset{-1}{p}(B')$, there exists an element V of $\mathscr{B}'$ such that $x\in V$ and $V\subset U$, and one has $[U, s, x] =i([V, r_{VU}(s), x])$. The mapping $i$ is continuous because the topology of $X_{\mathscr{F}|\mathscr{B}'}$ is the finest making continuous the mappings defined by $x\mapsto [U, s, x]$, for $U\in \mathscr{B}'$ and $s\in \mathscr{F}(U)$. By corollary 2 of Proposition 6 in I, p. 30, the canonical injection $i$ of $E_{\mathscr{F}|\mathscr{B}'}$ into $E_{\mathscr{F}}$ induces a $B'$-isomorphism of $E_{\mathscr{F}|\mathscr{B}'}$ onto $\overset{-1}{p}(B')$.

In particular, when $B'$ is equal to B$,i: E_{\mathscr{F}|\mathscr{B}'}\rightarrow E_{\mathscr{F}}$ is a B-isomorphism of étalé spaces.

2) Let $\mathscr{G}$ be a presheaf on B relative to the base $\mathscr{B}$ and let $\varphi :\mathscr{F}\rightarrow \mathscr{G}$ be a morphism of presheaves. The family $\varphi '= (\varphi_U)_{U\in\mathscr{B}'}$ is a morphism of presheaves from $\mathscr{F}|\mathscr{B}'$ into $\mathscr{G}|\mathscr{B}'$. The diagram

$$
E\mathscr{F}|\mathscr{B}'E(\varphi ')E\mathscr{G}|\mathscr{B}'
$$

$ii'$

$E_{\mathscr{F}}^{E(\varphi)}E_{\mathscr{G}}$ , where $i$ and $i'$ are the canonical injections, is commutative.

#### Example 1 {#ta-i-s3-n5-exa-1 .statement tag=01O3}

Let B be a topological space, $\mathscr{B}$ a base of the topology of B and F a set. Take for $\mathscr{F}$ the presheaf on B relative to $\mathscr{B}$ defined by $\mathscr{F}(U) = F$ for every $U\in \mathscr{B}$ and $r_{UV}$ = Id$_F$ for every pair $(U,V)$ of elements of $\mathscr{B}$ such that $U\subset V$. The mapping $[U, s, x]\mapsto (x, s(x))$ is a B-isomorphism of the B-space $E_{\mathscr{F}}$ onto the B-space $B\times F$ where F is endowed with the discrete topology. It will be noted that when $\mathscr{B}$ is the set of open subsets of B, the presheaf $\mathscr{F}$ on B is a sheaf only if the set F is reduced to a point (cf. I, p. 43, remark).

#### Example 2 {#ta-i-s3-n5-exa-2 .statement tag=01O4}

Let B be a topological space and $(E, p)$ a B-space. Let $\mathscr{F}$ be the sheaf on B of continuous sections of $(E, p)$. The mapping $(U, s, x)\mapsto s(x)$ of $X_{\mathscr{F}}$ into E is compatible with the equivalence relation $R_{\mathscr{F}}$. The mapping $e: E_{\mathscr{F}}\rightarrow E$ deduced from it by passing to the quotient is a B-morphism; the B-morphism $e$ is said to be canonical. The image of $e$ is the union of the images of the continuous sections of $p$ over the open sets of B. The mapping $e$ is therefore surjective if $p$ is etale (I, p. 33, prop. 9). On the other hand, the mapping $e$ is injective if and only if for every open set U of B and every pair $(s, s')$ of continuous sections of $p$ on U, the set of points $x\in U$ such that $s(x) =s'(x)$ is open; this is in particular the case if $p$ is etale (I, p. 34, prop. 11, b)). Consequently, if $(E, p)$ is an etale B-space, the mapping $e$ is a B-isomorphism.

#### Example 3 {#ta-i-s3-n5-exa-3 .statement tag=01O5}

Let B be a topological space, $\mathscr{B}$ a base of the topology of B$,\mathscr{F}$ a presheaf on B relative to $\mathscr{B}$ and $\mathscr{L}$ a sub-presheaf of $\mathscr{F}$. Then the set $X_{\mathscr{L}}$ is contained in the set $X_{\mathscr{F}}$ and the equivalence relation $R_{\mathscr{F}}$ induces in $X_{\mathscr{L}}$ the equivalence relation $R_{\mathscr{L}}$. The B-morphism $E(i): E_{\mathscr{L}}\rightarrow E_{\mathscr{F}}$ associated with the canonical morphism $i:\mathscr{L}\rightarrow \mathscr{F}($I, p. 48, example 2) is therefore injective. Since $E_{\mathscr{L}}$ and $E_{\mathscr{F}}$ are etale B-spaces, the mapping $E(i)$ is open and even etale (I, p. 30, cor. 1), and therefore induces a homeomorphism of $E_{\mathscr{L}}$ onto an open subset of $E_{\mathscr{F}}$.

### 6. Sheaf associated with a presheaf

Let us retain the notation of No.$^o5$. The sheaf associated with the presheaf $\mathscr{F}$ is the sheaf $\mathscr{S}(B; E_{\mathscr{F}})$ of continuous sections of the etale B-space $E_{\mathscr{F}}$ associated with the presheaf $\mathscr{F}$, and is denoted by $\widetilde{\mathscr{F}}$. For every open set $U\in \mathscr{B}$, let $\sigma_{\mathscr{F}}(U):\mathscr{F}(U)\rightarrow \widetilde{\mathscr{F}}(U)$ denote the mapping which, to $s\in \mathscr{F}(U)$, associates the continuous section $\sigma_{\mathscr{F}}(U, s):x\mapsto [U, s, x]$ of $E_{\mathscr{F}}$ over U. By definition of the equivalence relation $R_{\mathscr{F}}$, the family $\sigma_{\mathscr{F}}= (\sigma_{\mathscr{F}}(U))_{U\in\mathscr{B}}$ is a morphism of presheaves from $\mathscr{F}$ into the presheaf $\widetilde{\mathscr{F}}|\mathscr{B}$. The morphism $\sigma_{\mathscr{F}}$ is called the canonical morphism of $\mathscr{F}$ into $\widetilde{\mathscr{F}}|\mathscr{B}$.

Let us denote by $j_{\mathscr{F}}: E_{\mathscr{F}}\rightarrow E_{\mathscr{F}}$ the B-morphism composed of the canonical B-isomorphism $E_{\mathscr{F}|\mathscr{B}}\rightarrow E_{\mathscr{F}}\widetilde{(}I$, p. 51) and the B-morphism $E(\sigma_{\mathscr{F}}): E_{\mathscr{F}}\rightarrow$ $E_{\widetilde{\mathscr{F}}|\mathscr{B}}$. Let us note$\widetilde{s}$ on the other hand by $e_{\mathscr{F}}:E_{\widetilde{\mathscr{F}}}\rightarrow E_{\mathscr{F}}$ the canonical B-isomorphism (I, p. 52, example 2).

#### Proposition 2 {#ta-i-s3-prop-2 .statement tag=01O6}

The mapping $j_{\mathscr{F}}$ is the inverse B-isomorphism of $e_{\mathscr{F}}$.

For $U\in \mathscr{B},s\in \mathscr{F}(U)$ and $x\in U$, one has by definition of $j_{\mathscr{F}}:$

$$
j_{\mathscr{F}}([U, s, x]) = [U, \sigma_{\mathscr{F}}(U, s), x]
$$

whence $e_{\mathscr{F}}(j_{\mathscr{F}}([U, s, x])) =\sigma_{\mathscr{F}}(U, s)(x) = [U, s, x]$. This proves the proposition.

#### Corollary {#ta-i-s3-n6-cor-1 .statement tag=01O7}

For every $a\in B$, the mapping $(\sigma_{\mathscr{F}})_a:\mathscr{F}_a\rightarrow \widetilde{\mathscr{F}}_a$ is bijective.

Since $j_{\mathscr{F}}$ is a B-isomorphism, the same is true of $E(\sigma_{\mathscr{F}})$, and $(\sigma_{\mathscr{F}})_a$ is deduced from it by passing to the fibres at $a$.

Let $\mathscr{G}$ be a presheaf on B relative to $\mathscr{B}$ and let $\varphi :\mathscr{F}\rightarrow \mathscr{G}$ be a morphism of presheaves. One denotes by $\widetilde{\varphi}:\widetilde{\mathscr{F}}\rightarrow \widetilde{\mathscr{G}}$ the morphism of sheaves $\mathscr{S}_{E(\varphi)}($I, p. 48, example 1), where $E(\varphi ): E_{\mathscr{F}}\rightarrow E_{\mathscr{G}}$ is the B-morphism associated with $\varphi$. For every open set $U\in \mathscr{B}$ and every $s\in \mathscr{F}(U)$, one has, by definition,

$$
\widetilde{\varphi}_U(\sigma_{\mathscr{F}}(U, s)) = E(\varphi )\circ \sigma_{\mathscr{F}}(U, s) =\sigma_{\mathscr{G}}(U, \varphi_U(s))
$$

One has therefore:

(1) $\widetilde{\varphi}_U\circ \sigma_{\mathscr{F}}(U) =\sigma_{\mathscr{G}}(U)\circ \varphi_U$, for every $U\in \mathscr{B}$. In other words:

$$
\widetilde{\varphi}|\mathscr{B}\circ \sigma_{\mathscr{F}}=\sigma_{\mathscr{G}}\circ \varphi \tag{2}
$$

#### Proposition 3 {#ta-i-s3-prop-3 .statement tag=01O8}

Let B be a topological space, let $\mathscr{B}$ be a basis of the topology of B, let $\mathscr{F}= (\mathscr{F}(U), f_{UV})$ be a presheaf on B relative to $\mathscr{B}$, let $\widetilde{\mathscr{F}}$ be the associated sheaf and let $\sigma_{\mathscr{F}}:\mathscr{F}\rightarrow \widetilde{\mathscr{F}}|\mathscr{B}$ be the canonical morphism. Given a sheaf $\mathscr{G}= (\mathscr{G}(U), g_{UV})$ on B and a morphism of presheaves $\varphi :\mathscr{F}\rightarrow \mathscr{G}|\mathscr{B}$, there exists a unique morphism of sheaves $\psi :\widetilde{\mathscr{F}}\rightarrow \mathscr{G}$ such that $\psi |\mathscr{B}\circ \sigma_{\mathscr{F}}=\varphi$.

#### Lemma {#ta-i-s3-n6-lem-1 .statement tag=01O9}

Let U be an open subset of B and $s: U\rightarrow E_{\mathscr{F}}$ a continuous section of $E_{\mathscr{F}}$ over U. For every point $a$ of U, there exist an open set $V\in \mathscr{B}$ such that $a\in V$ and $V\subset U$, and an element $v$ of $\mathscr{F}(V)$ such that $s|V =\sigma_{\mathscr{F}}(V, v)$.

Let $a\in U$. By definition of the space $E_{\mathscr{F}}$, there exist an open set $V'\in \mathscr{B}$ such that $a\in V'$ and an element $t$ of $\mathscr{F}(V')$ such that $s(a) = [V', t, a]$. Then $s$ and $\sigma_{\mathscr{F}}(V', t)$ induce by restriction two continuous sections of $E_{\mathscr{F}}$ over $V'\cap U$ which are equal at the point $a$. By Prop. 11, b) of I, p. 34, there exists an open neighbourhood V of $a$, contained in $V'\cap U$, belonging to $\mathscr{B}$, such that $s$ and $\sigma_{\mathscr{F}}(V', t)$ are equal at every point of V. If we put $v=f_{VV'}(t)$, we indeed have $s|V =\sigma_{\mathscr{F}}(V, v)$.

Let us prove the proposition. For every open set U of B and every section $s\in \widetilde{\mathscr{F}}(U)$, let us denote by $D(U, s)$ the set of pairs $(V, v)$ such that $V\in \mathscr{B},V\subset U,v\in \mathscr{F}(U)$ and $s|V =\sigma_{\mathscr{F}}(V, v)$. It follows from the lemma that these open sets V form a covering of U.

If there exists a morphism $\psi :\widetilde{\mathscr{F}}\rightarrow \mathscr{G}$ such that $\psi |\mathscr{B}\circ \sigma_{\mathscr{F}}=\varphi$, then, for every open set U of B, every section $s\in \widetilde{\mathscr{F}}(U)$ and every pair $(V, v)\in D(U, s)$, we have $g_{VU}(\psi_U(s)) =\psi_V(s|V) =\varphi_V(v)$. This proves the uniqueness of $\psi$ by virtue of property $(F_1)$ of sheaves.

Let U be an open set of B and $s$ an element of $\widetilde{\mathscr{F}}(U)$. Let $(V, v)$ and $(V', v')$ be elements of $D(U, s)$. We have $s(a) = [V, v, a] = [V', v', a]$ for every point $a\in V\cap V'$. There therefore exists a pair $(W, w)\in D(V\cap V', s)$ such that $a\in W$ and $f_{WV}(v) =f_{WV}(v') =w$. We then have

$$
g_{W(V\cap V')}\circ g_{(V\cap V')V}(\varphi_V(v)) =g_{WV}(\varphi_V(v)) =\varphi_W(f_{WV}(v)) =\varphi_W(w)
$$

and analogously,

$$
g_{W(V\cap V')}\circ g_{(V\cap V')V'}(\varphi_{V'}(v')) =\varphi_W(w)
$$

whence

$$
g_{W(V\cap V')}\circ g_{(V\cap V')V}(\varphi_V(v)) =g_{W(V\cap V')}\circ g_{(V\cap V')V'}(\varphi_{V'}(v'))
$$

By property $(F_1)$ of sheaves, we therefore have

$$
g_{(V\cap V')V}(\varphi_V(v)) =g_{(V\cap V')V'}(\varphi_{V'}(v'))
$$

By properties $(F_1)$ and $(F_2)$ of sheaves, there exists a unique element $\psi_U(s)\in \mathscr{G}(U)$ such that one has:

(3) $g_{VU}(\psi_U(s)) =\varphi_V(v)$ for every $(V, v)\in D(u, s)$.

Let $\psi_U:\widetilde{\mathscr{F}}(U)\rightarrow \mathscr{G}(U)$ be the resulting mapping. It follows immediately from (3) that the family $\psi = (\psi_U)$ is a morphism of sheaves and that one has $\varphi_V=\psi_V\circ \sigma_{\mathscr{F}}(V)$ for every $V\in \mathscr{B}$.

#### Corollary 1 {#ta-i-s3-prop-3-cor-1 .statement tag=01OA}

Let B be a topological space, $\mathscr{F}$ a presheaf on B$,\widetilde{\mathscr{F}}$ the associated sheaf and $\sigma_{\mathscr{F}}:\mathscr{F}\rightarrow \widetilde{\mathscr{F}}$ the canonical morphism. For $\mathscr{F}$ to be a sheaf, it is necessary and sufficient that $\sigma_{\mathscr{F}}$ be an isomorphism.

If $\sigma_{\mathscr{F}}$ is an isomorphism, $\mathscr{F}$ is a sheaf. Conversely, if $\mathscr{F}$ is a sheaf, there exists by proposition 3 a morphism $\varphi :\widetilde{\mathscr{F}}\rightarrow \mathscr{F}$ such that $\varphi \circ \sigma_{\mathscr{F}}=$ Id$_{\mathscr{F}}$. Since Id$_{\mathscr{F}}$ is the unique morphism $\psi :\widetilde{\mathscr{F}}\rightarrow \widetilde{\mathscr{F}}$ such that $\psi \circ \sigma_{\mathscr{F}}=\sigma_{\mathscr{F}}$, one has therefore $\widetilde{\sigma}_{\mathscr{F}}\circ \varphi =$ Id$_{\widetilde{\mathscr{F}}}$.

#### Remark {#ta-i-s3-n6-rem-1 .statement tag=01OB}

Let B be a topological space, $\mathscr{F}$ a presheaf on B, $\mathscr{G}$ a sheaf on B and $\varphi :\mathscr{F}\rightarrow \mathscr{G}$ a morphism of presheaves. The canonical morphism $\sigma_{\mathscr{G}}:\mathscr{G}\rightarrow \widetilde{\mathscr{G}}$ is an isomorphism by corollary 1. By relation (2) of I, p. 54, the unique morphism $\psi :\widetilde{\mathscr{F}}\rightarrow \mathscr{G}$ such that $\psi \circ \sigma_{\mathscr{F}}=\varphi$ is therefore $\sigma^{-1}_{\mathscr{G}}\circ \widetilde{\varphi}$.

#### Corollary 2 {#ta-i-s3-prop-3-cor-2 .statement tag=01OC}

Let B be a topological space, $\mathscr{F}$ and $\mathscr{G}$ sheaves on B and $\varphi$ a morphism of sheaves from $\mathscr{F}$ into $\mathscr{G}$. The following assertions are equivalent:

(i) $\varphi$ is an isomorphism;

(ii) There exists a basis $\mathscr{B}$ of the topology of B such that for every $U\in \mathscr{B}$, the mapping $\varphi_U$ is bijective;

(iii) For every point $a$ of B, the mapping $\varphi_a$ is a bijection of the stalk $\mathscr{F}_a$ onto the stalk $\mathscr{G}_a$.

The implication (i)$\Rightarrow$(ii) is immediate.

(ii)$\Rightarrow$(iii) : consider the commutative diagram (I, p. 51)

$$
E\mathscr{F}|\mathscr{B}E(\varphi |\mathscr{B})E\mathscr{G}|\mathscr{B}
$$

$$
E_{\mathscr{F}}^{E(\varphi)}E_{\mathscr{G}}
$$

where the vertical arrows are the canonical B-isomorphisms. If condition (ii) is satisfied, $E(\varphi |\mathscr{B})$ is a B-isomorphism, hence $E(\varphi )$ is also one. The mappings $\varphi_a$ are deduced from $E(\varphi )$ by passing to the fibres and are therefore bijective.

(iii)$\Rightarrow$(i) : under assumption (iii), the mapping $E(\varphi ): E_{\mathscr{F}}\rightarrow E_{\mathscr{G}}$ is a bijective B-morphism of étalé spaces and therefore is a B-isomorphism (I, p. 30, cor. 2 of prop. 6). Hence the morphism $\widetilde{\varphi}:\widetilde{\mathscr{F}}\rightarrow \widetilde{\mathscr{G}}$ is an isomorphism. Since $\mathscr{F}$ and $\mathscr{G}$ are sheaves, the canonical morphisms $\sigma_{\mathscr{F}}:\mathscr{F}\rightarrow \widetilde{\mathscr{F}}$ and $\sigma_{\mathscr{G}}:\mathscr{G}\rightarrow \widetilde{\mathscr{G}}$ are isomorphisms (corollary 1) and one has $\widetilde{\varphi}\circ \sigma_{\mathscr{F}}=\sigma_{\mathscr{G}}\circ \varphi ($I, p. 54, relation (2)) hence $\varphi$ is an isomorphism.

#### Scholium {#ta-i-s3-n6-sch-1 .statement tag=01OD}

Let B be a topological space. To every sheaf $\mathscr{F}$ on B, one associates an étalé B-space $E_{\mathscr{F}}$ (I, p. 50, def. 4). To every étalé B-space T, one associates the sheaf $\mathscr{S}(T)$ on B of its continuous sections (I, p. 45, example 3). A canonical isomorphism of sheaves $\sigma_{\mathscr{F}}:\mathscr{F}\rightarrow \mathscr{S}(E_{\mathscr{F}})$ has been defined (I, p. 55, cor. 1) and a canonical isomorphism of étalé B-spaces $e_T: E_{\mathscr{S}(T)}\rightarrow T$ (I, p. 52, example 2).

For every pair $(\mathscr{F},\mathscr{G})$ of sheaves on B, a mapping $\varphi \mapsto E(\varphi )$ of the set of morphisms of sheaves from $\mathscr{F}$ into $\mathscr{G}$ into the set of B-morphisms from $E_{\mathscr{F}}$ into $E_{\mathscr{G}}$ has been defined (I, p. 50). One has the relations

E(Id$_{\mathscr{F}}$) $=$ Id$_{E_{\mathscr{F}}},E(\psi \circ \varphi ) = E(\psi )\circ E(\varphi )$.

For every pair $(T,U)$ of étalé spaces over B, a mapping $f\mapsto \mathscr{S}(f)$ from the set of B-morphisms of T into U to the set of sheaf morphisms of $\mathscr{S}(T)$ into $\mathscr{S}(U)$ was defined (I, p. 48, Example 1). One has the relations

$\mathscr{S}$ (Id$_T$) $=$ Id$_{\mathscr{S}(T)},\mathscr{S}(g\circ f) =\mathscr{S}(g)\circ \mathscr{S}(f)$.

With the preceding notation, the following diagrams are commutative:

$$
\mathscr{F}^{\varphi}\mathscr{G}E_{\mathscr{S}(T)}^{E(\mathscr{S}(f))}E_{\mathscr{S}(U)}
$$

(4) $\sigma_{_{\mathscr{F}}}\sigma_{_{\mathscr{G}}}$ (5) $e_{_T}e_{_U}$

$\mathscr{S}(E_{\mathscr{F}})^{\mathscr{S}(E(\varphi))}\mathscr{S}(E_{\mathscr{G}})$, T $^fU$.

This follows from I, p. 54, formula (2) for the first, and is an immediate consequence of the definitions for the second. This implies that for every pair $(\mathscr{F},\mathscr{G})$ of sheaves on B and every pair $(T,U)$ of étalé spaces over B, the mappings $\varphi \mapsto E(\varphi )$ and $f\mapsto \mathscr{S}(f)$ considered above are bijective.

These results make it possible to deduce a statement concerning étalé spaces over B from a statement concerning sheaves on B, and conversely.

### 7. Direct image and inverse image of a sheaf

Let A and B be topological spaces and let $u: A\rightarrow B$ be a continuous mapping.

Let $\mathscr{F}= (\mathscr{F}(U), f_{UV})$ be a presheaf on A. We define a presheaf $\mathscr{F}'$ on B as follows: for every open set U of B, put $\mathscr{F}'(U) =\mathscr{F}(\overset{-1}{u}(U))$ and for every pair $(U,V)$ of open sets of B such that U $\subset V$, put $f'_{UV}=f_{\overset{-1}{u}(U)\overset{-1}{u}(V)}$. Then $(\mathscr{F}'(U), f'_{UV})$ is a presheaf on B. It is denoted by $u_*(\mathscr{F})$ and is called the direct image presheaf of the presheaf $\mathscr{F}$ by the mapping $u$.

If $(U_i)_{i\in I}$ is a family of open sets of B, one has $\overset{-1}{u}(\bigcup_{i\in I}U_i) =$ $\bigcup_{i\in I}\overset{-1}{u}(U_i)$ and $\overset{-1}{u}(\bigcap_{i\in I}U_i) =\bigcap_{i\in I}\overset{-1}{u}(U_i)$ (E, II, p. 25, Prop. 3 and 4). It follows at once that, if $\mathscr{F}$ has property $(F_1)$ (resp. $(F_2)$) of sheaves (I, p. 43), the same is true of $u_*(\mathscr{F})$. Consequently, the direct image of a sheaf is a sheaf.

Let $\mathscr{F}_1$ and $\mathscr{F}_2$ be presheaves on A and let $\varphi :\mathscr{F}_1\rightarrow \mathscr{F}_2$ be a presheaf morphism. Then there exists a unique presheaf morphism $u_*\varphi :u_*\mathscr{F}_1\rightarrow u_*\mathscr{F}_2$ such that for every open set U of B, the mapping $(u_*\varphi )(U): (u_*\mathscr{F}_1)(U)\rightarrow (u_*\mathscr{F}_2)(U)$ is the mapping $\varphi (\overset{-1}{u}(U)):\mathscr{F}_1(\overset{-1}{u}(U))\rightarrow \mathscr{F}_2(\overset{-1}{u}(U))$. If $\mathscr{F}_3$ is a presheaf on A and if $\psi :\mathscr{F}_2\rightarrow \mathscr{F}_3$ is a presheaf morphism, one has $u_*(\psi \circ \varphi ) =u_*(\psi )\circ u_*(\varphi )$.

Let C be a topological space and let $v: B\rightarrow$ C be a continuous mapping. If $\mathscr{F}$ is a presheaf on A, the presheaves $v_*(u_*(\mathscr{F}))$ and $(v\circ u)_*(\mathscr{F})$ coincide. If $\varphi :\mathscr{F}_1\rightarrow \mathscr{F}_2$ is a presheaf morphism on A, one has the equality $v_*(u_*(\varphi )) = (v\circ u)_*(\varphi )$.

#### Example 1 {#ta-i-s3-n7-exa-1 .statement tag=01OE}

Let B be a topological space, A a subspace of B and $\mathscr{F}= (\mathscr{F}(U), f_{UV})$ a presheaf on A. Let $i: A\rightarrow B$ denote the canonical injection. Then one has $i_*(\mathscr{F}) = (\mathscr{F}'(U), f'_{UV})$ where for every open set U of B$,\mathscr{F}'(U) =\mathscr{F}(U\cap A)$, and for every pair $(U,V)$ of open sets of B with $U\subset V,f'_{UV}=f_{(U\cap A)(V\cap A)}$.

Let now $\mathscr{G}$ be a presheaf on B. The inverse image of the presheaf $\mathscr{G}$ by $u$ is defined to be, and is denoted by $u^*(\mathscr{G})$, the sheaf $\mathscr{C}_B(A; E_{\mathscr{G}})$ on A of B-morphisms with values in the B-space $E_{\mathscr{G}}($I, p. 45, example 4). It is canonically isomorphic to the sheaf on A of sections of the étalé A-space $A\times_BE_{\mathscr{G}}$ (I, p. 9, prop. 3). From this one deduces (I, p. 52, example 2) a canonical isomorphism $\varphi$ of the étalé space associated with $u^*(\mathscr{G})$ onto the A-space $A\times_BE_{\mathscr{G}}$. If moreover $\mathscr{G}$ is a sheaf, for every point $a$ of A there is a canonical bijection $\psi_a:u^*(\mathscr{G})_a\rightarrow \mathscr{G}_{u(a)}:$ for every open neighbourhood U of $a$ in A and every B-morphism $f: U\rightarrow E_{\mathscr{G}}$, one has

$$
\varphi ([U, f, a]) = (a, f(a)),\psi_a([U, f, a]) =f(a)
$$

Let $\mathscr{G}_1$ and $\mathscr{G}_2$ be presheaves on B and let $\varphi :\mathscr{G}_1\rightarrow \mathscr{G}_2$ be a morphism of presheaves. By base change of the morphism of étalé B-spaces $E(\varphi ): E_{\mathscr{G}_1}\rightarrow E_{\mathscr{G}_2}$ one obtains a morphism of étalé A-spaces $A\times_BE_{\mathscr{G}_1}\rightarrow A\times_BE_{\mathscr{G}_2}$, whence a morphism of sheaves on A$,u^*(\varphi ):u^*(\mathscr{G}_1)\rightarrow u^*(\mathscr{G}_2)$. Let $\mathscr{G}_3$ be a presheaf on B and let $\psi :\mathscr{G}_2\rightarrow \mathscr{G}_3$ be a morphism of presheaves. Then one has the equality $u^*(\psi \circ \varphi ) =u^*(\psi )\circ u^*(\varphi )$.

Let C be a topological space and let $v: B\rightarrow$ C be a continuous mapping. If $\mathscr{G}$ is a presheaf on C, the sheaves $u^*(v^*(\mathscr{G}))$ and $(v\circ u)^*(\mathscr{G})$ are canonically identified (I, p. 5). If $\varphi :\mathscr{G}_1\rightarrow \mathscr{G}_2$ is a morphism of presheaves on C, one has moreover $u^*(v^*(\varphi )) = (v\circ u)^*(\varphi )$.

#### Remark {#ta-i-s3-n7-rem-1 .statement tag=01OF}

The canonical morphism $\sigma_{\mathscr{G}}:\mathscr{G}\rightarrow \widetilde{\mathscr{G}}$ of I, p. 53 corresponds, in terms of étalé spaces, to the isomorphism $j_{\mathscr{G}}$ of proposition 2 of I, p. 53. It follows that $u^*(\sigma_{\mathscr{G}})$ is an isomorphism. In particular, if A = B and $u=$ Id$_A$, the presheaf $u^*(\mathscr{F})$ is the sheaf $\widetilde{\mathscr{F}}$.

#### Example 2 {#ta-i-s3-n7-exa-2 .statement tag=01OG}

Let B be a topological space and A a subspace of B. Let $i: A\rightarrow B$ denote the canonical injection. For every sheaf $\mathscr{G}$ on B, let $\mathscr{G}_A$ denote the sheaf $i^*(\mathscr{G})$, and say that $\mathscr{G}_A$ is the sheaf on A induced by the sheaf $\mathscr{G}$. The sheaf $\mathscr{G}_A$ is identified with the sheaf $\mathscr{S}(A; (E_{\mathscr{G}})_A)$ of sections of the étalé A-space induced by $E_{\mathscr{G}}$ over A.

Suppose that A is an open subspace of B, and let $\mathscr{G}$ be a sheaf on B. By definition, the sheaf $\mathscr{G}_A$ is the sheaf $\widetilde{\mathscr{G}}|A$ deduced from $\widetilde{\mathscr{G}}$ by restriction to the open set A (I, p. 43). Let $\sigma_{\mathscr{G}}:\mathscr{G}\rightarrow \widetilde{\mathscr{G}}$ be the canonical isomorphism (I, p. 55, cor. 1). Then $\sigma_{\mathscr{G}}|A$ is an isomorphism, called canonical, of the sheaf $\mathscr{G}|A$ onto the sheaf $\mathscr{G}_A$ which is called the canonical isomorphism of $\mathscr{G}|A$ onto $\mathscr{G}_A$.

### 8. The homomorphisms $\alpha \mathbf{e}\mathbf{t}\beta$ ; adjunction

Let A and B be topological spaces and let $u: A\rightarrow B$ be a continuous mapping. Let $\mathscr{G}$ be a presheaf on B. By definition of the direct image of presheaves, a section of the sheaf $u_*u^*\mathscr{G}$ over an open set U of B is a section of the sheaf $u^*\mathscr{G}$ over the open set $\overset{-1}{u}(U)$ of A, that is, a B-morphism $\overset{-1}{u}(U)\rightarrow E_{\mathscr{G}}$. Thus one defines a sheaf morphism $\widetilde{\mathscr{G}}\rightarrow u_*u^*\mathscr{G}$ by associating with the section $s$ of $E_{\mathscr{G}}$ over an open set U of B the section $s\circ u$ of $E_{\mathscr{G}}$ over $\overset{-1}{u}(U)$. The composition of this morphism and of the canonical morphism $\sigma_{\mathscr{G}}:\mathscr{G}\rightarrow \widetilde{\mathscr{G}}$ (I, p. 53) is a presheaf morphism $\mathscr{G}\rightarrow u_*u^*\mathscr{G}$ which will be denoted by $\beta_{\mathscr{G}}^u$, or even $\beta_{\mathscr{G}}$ if there is no ambiguity as to the mapping $u$.

#### Remark 1 {#ta-i-s3-n8-rem-1 .statement tag=01OH}

Let A, B, C be topological spaces, let $u: A\rightarrow B,v: B\rightarrow C$ be continuous mappings; put $w=v\circ u$. Let $\mathscr{G}$ be a presheaf on C.

Let U be an open set of C and $s$ a section of $E_{\mathscr{G}}$ over U. Then $\beta_{\mathscr{G}}^v(s)$ is the section $s\circ v$ of $E_{\mathscr{G}}$ over $\overset{-1}{v}(U)$, and $v_*(\beta_{v^*\mathscr{G}}^u)(\beta^v_{\mathscr{G}}(s))$ is the section $s\circ v\circ u=s\circ w$ of $E_{\mathscr{G}}$ over $\overset{-1}{u}(\overset{-1}{v}(U)) =\overset{-1}{w}(U)$.

It follows that $\beta_{\mathscr{G}}^w=v_*(\beta_{v^*\mathscr{G}}^u)\circ \beta_{\mathscr{G}}^v$.

#### Remark 2 {#ta-i-s3-n8-rem-2 .statement tag=01OI}

If $\gamma :\mathscr{G}_1\rightarrow \mathscr{G}_2$ is a presheaf morphism on B, the presheaf morphisms $\beta_{\mathscr{G}_2}\circ \gamma$ and $u_*u^*(\gamma )\circ \beta_{\mathscr{G}_1}$ are equal. In fact, if V is an open set of B and $s\in \mathscr{G}_1(V),\beta_{\mathscr{G}_1}(s)$ is the section $t$ of $A\times_BE_{\mathscr{G}_1}$ over $\overset{-1}{u}(V)$, defined by $x\mapsto (x,[V, s, u(x)])$. The image of $t$ under $u^*(\gamma )$ is therefore the section of $A\times_BE_{\mathscr{G}_2}$ over $\overset{-1}{u}(V)$ given by $x\mapsto (x,[V, \gamma (s), u(x)])$. Hence indeed $u_*u^*(\gamma )\circ \beta_{\mathscr{G}_1}(s) =\beta_{\mathscr{G}_2}(\gamma (s))$.

#### Proposition 4 {#ta-i-s3-prop-4 .statement tag=01OJ}

Let A and B be topological spaces, $u: A\rightarrow B$ a continuous mapping, $\mathscr{G}$ a presheaf on B$,\mathscr{F}$ a sheaf on A.

For every presheaf morphism $\varphi :\mathscr{G}\rightarrow u_*\mathscr{F}$, there exists a unique sheaf morphism $\psi :u^*(\mathscr{G})\rightarrow \mathscr{F}$ such that $\varphi =u_*(\psi )\circ \beta_{\mathscr{G}}$.

In other words, the canonical mapping

Mor($u^*(\mathscr{G}),\mathscr{F}$)$\rightarrow$ Mor($\mathscr{G}, u_*(\mathscr{F})$)$,\psi \mapsto u_*(\psi )\circ \beta_{\mathscr{G}}$

is a bijection.

With the notation of proposition 4, one will sometimes denote $\psi =\varphi^{\sharp}$ and $\varphi =\psi^{\flat}$.

Let us prove proposition 4. By remark 2 applied to the morphism $\sigma_{\mathscr{G}}:\mathscr{G}\rightarrow \widetilde{\mathscr{G}}$, the morphism $\beta_{\mathscr{G}}$ is equal to the composition

$$
u_*(u^*(\sigma_{\mathscr{G}})^{-1})\circ \beta_{\widetilde{\mathscr{G}}}\circ \sigma_{\mathscr{G}}
$$

where $u^*(\sigma_{\mathscr{G}}):u^*(\mathscr{G})\rightarrow u^*(\widetilde{\mathscr{G}})$ is the canonical isomorphism of the remark in I, p. 58. Let $\widetilde{\varphi}:\widetilde{\mathscr{G}}\rightarrow u_*\mathscr{F}$ be the unique sheaf morphism such that $\widetilde{\varphi}\circ \sigma_{\mathscr{G}}=\varphi ($I, p. 54, prop. 3). It is then enough to prove that there exists a unique sheaf morphism $\widetilde{\psi}:u^*(\mathscr{G})\rightarrow \mathscr{F}$ such that $u_*(\widetilde{\psi})\circ \beta_{\mathscr{G}}=\widetilde{\varphi}$.

We p$\widetilde{o}$ssibly may therefore suppose that $\mathscr{G}$ is a sheaf. In order that a sheaf morphism $\psi :u^*(\mathscr{G})\rightarrow \mathscr{F}$ satisfy the conclusion of proposition 4, it is necessary and sufficient that for every open set V of B and every section $t$ of $E_{\mathscr{G}}$ over V, one have

$$
\varphi_V(t) =\psi_{\overset{-1}{u}(V)}(t\circ u|\overset{-1}{u}(V)) \tag{6}
$$

Let $U_0$ be an open set of A and $s_0$ an element of $u^*(\mathscr{G})(U_0)$, in other words a B-morphism from $U_0$ into $E_{\mathscr{G}}$. Let $S(U_0, s_0)$ be the set of triples $(U,V, t)$ where U is an open set of A contained in $U_0$, V is an open set of B such that $u(U)\subset V$, and $t$ a section of $E_{\mathscr{G}}$ over V such that one has

$$
t\circ u|U =s_0|U \tag{7}
$$

If $U_1$ and $U_2$ are open sets of A with $U_1\subset U_2$, let us denote by $f_{U_1U_2}$ the restriction mapping $\mathscr{F}(U_2)\rightarrow \mathscr{F}(U_1)$. For every $(U,V, t)\in S(U_0, s_0)$, one then has the relation

$$
f_{UU_0}(\psi_{U_0}(s_0)) =\psi_U(s_0|U)
$$

$$
=\psi_U(t\circ u|U)
$$

$$
=f_{U\overset{-1}{u}(V)}(\psi_{\overset{-1}{u}(V)}(t\circ u|\overset{-1}{u}(V)))
$$

Consequently, if $\psi :u^*(\mathscr{G})\rightarrow \mathscr{F}$ satisfies (6), one has

$$
f_{UU_0}(\psi_{U_0}(s_0)) =f_{U\overset{-1}{u}(V)}(\varphi_V(t)) \tag{8}
$$

Let us prove that, for every point $a$ of $U_0$, there exists a triple $(U,V, t)\in S(U_0, s_0)$ such that $a\in U$. For indeed, let $a$ be a point of $U_0$. There exists an open neighbourhood V of B containing $u(a)$ and a section $t$ of the étale space $E_{\mathscr{G}}$ over V such that $t(u(a)) =s_0(a)$ (I, p. 33, prop. 9). Let $U_1=\overset{-1}{u}(V)\cap U_0$. The sections $s_0|U_1$ and $t\circ u|U_1$ of the $U_1$-étale space $E_{\mathscr{G}}\times_BU_1$ coincide at the point $a$. By proposition 11, b) of I, p. 34, the set of points where they coincide is an open set U of $U_1$ containing $a$. The triple $(U,V, t)$ then belongs to $S(U_0, s_0)$.

Formula (8) and property $(F_1)$ of sheaves (I, p. 43) then imply the uniqueness of $\psi$.

Let $(U,V, t)$ and $(U',V', t')$ be elements of $S(U_0, s_0)$. By relation (7), the restrictions of $t$ and $t'$ to $u(U\cap U')$ coincide. By Prop. 11, b) of I, p. 34, there exists an open set W of B such that $u(U\cap U')\subset$ $W\subset V\cap V'$ and $t|W =t'|W$. Hence

$$
f_{\overset{-1}{u}(W)\overset{-1}{u}(V)}(\varphi_V(t)) =\varphi_W(t|W) =\varphi_W(t'|W) =f_{\overset{-1}{u}(W)\overset{-1}{u}(V')}(\varphi_{V'}(t'))
$$

whence

$$
f_{(U\cap U')\overset{-1}{u}(V)}(\varphi_V(t)) =f_{(U\cap U')\overset{-1}{u}(V')}(\varphi_{V'}(t')) \tag{9}
$$

By properties $(F_1)$ and $(F_2)$ for the sheaf $\mathscr{F}$, there exists a unique element $s'$ of $\mathscr{F}(U_0)$ such that for every triple $(U,V, t)$ of $S(U_0, s_0)$, one has:

$$
f_{UU_0}(s') =f_{U\overset{-1}{u}(V)}(\varphi_V(t)) \tag{10}
$$

Let us denote this element by $\psi_{U_0}(s_0)$.

Let $U_1$ be an open set contained in $U_0$ and let $s_1=s_0|U_1$. If $(U,V, t)\in$ $S(U_1, s_1)$, U is an open set contained in $U_0$ and $t\circ u|U =s_1|U =s_0|U$, hence $(U, v, t)\in S(U_0, s_0)$ and relation (10) then implies that

$$
f_{UU_1}(f_{U_1U_0}(\psi_{U_0}(s_0))) =f_{UU_0}(\psi_{U_0}(s_0)) =f_{U\overset{-1}{u}(V)}(\varphi_V(t))
$$

By definition of $\psi_{U_1}(s_1)$, one therefore has $\psi_{U_1}(s_1) =f_{U_1U_0}(\psi_{U_0}(s_0))$. This proves that the family $\psi = (\psi_U)$ is a morphism of sheaves from $u^*(\mathscr{G})$ into $\mathscr{F}$.

Let us prove that $\psi$ satisfies relation (6). Let V thus be an open set of B and let $t$ be a section of $E_{\mathscr{G}}$ over V. If U = $\overset{-1}{u}(V)$ and if $s=t\circ u|U$, the triple $(U,V, t)$ belongs to $S(U, s)$ and relation (6) is an immediate consequence of relation (10), applied to $U = U_0$.

#### Proposition 5 {#ta-i-s3-prop-5 .statement tag=01OK}

Let A and B be topological spaces and let $u: A\rightarrow B$ be a continuous mapping.

a) Let $\mathscr{G}_1$ and $\mathscr{G}_2$ be presheaves on B and let $\gamma :\mathscr{G}_1\rightarrow \mathscr{G}_2$ be a morphism of presheaves. Let moreover $\mathscr{F}$ be a sheaf on A and $\varphi :\mathscr{G}_2\rightarrow u_*\mathscr{F}$ a morphism of presheaves. One has the equality

$$
(\varphi \circ \gamma )^{\sharp}=\varphi^{\sharp}\circ u^*(\gamma ) \tag{11}
$$

b) Let $\mathscr{F}_1,\mathscr{F}_2$ be sheaves on A and let $\mathscr{G}$ be a presheaf on B. Let $\varphi :\mathscr{F}_1\rightarrow \mathscr{F}_2$ be a morphism of sheaves and let $\gamma :\mathscr{G}\rightarrow$ $u_*\mathscr{F}_1$ be a morphism of presheaves. One has the relation

$$
(u_*(\varphi )\circ \gamma )^{\sharp}=\varphi \circ \gamma^{\sharp}
$$

a) By definition of $\varphi^{\sharp}$ and Remark 2 of I, p. 60, one has

$$
\varphi \circ \gamma =u_*(\varphi^{\sharp})\circ \beta_{\mathscr{G}_2}\circ \gamma =u_*(\varphi^{\sharp})\circ u_*u^*(\gamma )\circ \beta_{\mathscr{G}_1}
$$

Consequently, $\varphi \circ \gamma =u_*(\varphi^{\sharp}\circ u^*(\gamma ))\circ \beta_{\mathscr{G}_1}$, whence relation (11).

b) By definition of $\gamma^{\sharp}$, one has

$$
u_*(\varphi )\circ \gamma =u_*(\varphi )\circ u_*(\gamma^{\sharp})\circ \beta_{\mathscr{G}}=u_*(\varphi \circ \gamma^{\sharp})\circ \beta_{\mathscr{G}}
$$

whence the announced relation, having regard to the definition of $(u_*(\varphi )\circ \gamma )^{\sharp}$.

Put $\alpha_{\mathscr{F}}$ = Id$^{\sharp}_{u_*(\mathscr{F})}$; it is the unique sheaf morphism $\rho :u^*(u_*(\mathscr{F}))\rightarrow \mathscr{F}$ such that

Id$_{u_*(\mathscr{F})}=u_*(\rho )\circ \beta_{u_*(\mathscr{F})}$.

Relation (11), applied to $\mathscr{G}_2=u_*(\mathscr{F})$ and to the morphism $\varphi =$ Id$_{u_*(\mathscr{F})}$, yields for every presheaf morphism $\gamma :\mathscr{G}\rightarrow u_*(\mathscr{F})$ the factorization

$$
\gamma^{\sharp}=\alpha_{\mathscr{F}}\circ u^*(\gamma )
$$

It then follows from proposition 4 that for every sheaf morphism $\psi$ of $u^*(\mathscr{G})$ into $\mathscr{F},\psi^{\flat}$ is the unique morphism $\varphi :\mathscr{G}\rightarrow u_*(\mathscr{F})$ such that $\psi =\alpha_{\mathscr{F}}\circ u^*(\varphi )$.

#### Example 1 {#ta-i-s3-n8-exa-1 .statement tag=01OL}

Consider a topological space B, a subspace A of B, and denote by $i: A\rightarrow B$ the canonical injection. Let $(E, p)$ and $(E', p')$ be B-spaces. Take for $\mathscr{G}$ the sheaf $\mathscr{M}$or$_B(E; E')$ (I, p. 45, example 4) and for $\mathscr{F}$ the sheaf $\mathscr{M}$or$_A(E_A; E'_A)$. For every open set V of B and every V-morphism $f: E_V\rightarrow E'_V$, put $\varphi_V(f) =f_{V\cap A}$, where $f_{V\cap A}$ is the $(V\cap A)$-morphism of $E_{V\cap A}$ into $E'_{V\cap A}$ induced by $f$. The family $\varphi = (\varphi_V)$ resulting is a sheaf morphism of $\mathscr{G}$ into $i_*\mathscr{F}$. By proposition 4, there exists a unique sheaf morphism $\psi :\mathscr{M}$or$_B(E; E')_A\rightarrow \mathscr{M}$or$_A(E_A; E'_A)$ such that one has

$$
\psi_{V\cap A}(\sigma_{\mathscr{G}}(V, f)|V\cap A) =f_{V\cap A} \tag{12}
$$

for every open set V of B and every $f\in \mathscr{C}_V(E_V; E'_V)$. The morphism $\psi$ is called the canonical morphism of $\mathscr{M}$or$_B(E; E')_A$ into $\mathscr{M}$or$_A(E_A; E'_A)$.

If A is reduced to a point $a$, this morphism is identified with the stalk morphism at $a$ of the sheaf $\mathscr{M}$or$_B(E; E')$ onto the set $\mathscr{C}(E_a; E'_a)$.

By passing to subsheaves, the morphism $\psi$ induces a canonical morphism of $\mathscr{I}$som$_B(E; E')_A$ into $\mathscr{I}$som$_A(E_A; E'_A)$.

#### Example 2 {#ta-i-s3-n8-exa-2 .statement tag=01OM}

Let A, B, C be topological spaces and let $u: A\rightarrow B$, $v: B\rightarrow C$ be continuous mappings; put $w=v\circ u$. Let E and $E'$ be C-spaces. The canonical morphism from $\mathscr{M}$or$_C(E; E')_A$ into $\mathscr{M}$or$_A(E_A; E'_A)$ is the composite morphism of the morphism $\mathscr{M}$or$_C(E; E')_A\rightarrow \mathscr{M}$or$_B(E_B; E'_B)_A$ deduced from the canonical morphism of $\mathscr{M}$or$_C(E; E')_B$ into $\mathscr{M}$or$_B(E_B; E'_B)$ and the canonical morphism of $\mathscr{M}$or$_B(E_B,E'_B)_A$ into $\mathscr{M}$or$_A(E_A,E'_A)$.

### 9. Soft Sheaves

#### Definition 5 {#ta-i-s3-def-5 .statement tag=01ON}

Let $p: E\rightarrow B$ be an étale mapping. One says that the mapping $p$ is soft, or that the étale B-space $(E, p)$ is soft, if every continuous section of $p$ over a closed subspace of B extends to a continuous section of $p$ over B.

Let $\mathscr{F}$ be a sheaf on B. One says that $\mathscr{F}$ is a soft sheaf if the associated étale space (I, p. 50, def. 4) is soft.

Let $\mathscr{F}$ be a sheaf on B. The sheaf $\mathscr{F}$ is soft if and only if for every closed Z of B, every open neighbourhood U of Z and every $s\in \mathscr{F}(U)$, there exist $t\in \mathscr{F}(B)$ and an open neighbourhood V of Z contained in U such that $s|V =t|V$.

If $\mathscr{F}$ is a soft sheaf, $\mathscr{F}(B)$ is nonempty: in fact, the unique section of the étale space $E_{\mathscr{F}}$ associated with $\mathscr{F}$ over $\emptyset$ extends to a continuous section of $E_{\mathscr{F}}$ over B.

Let $p: E\rightarrow B$ be an étale mapping and let A be a closed subspace of B. If $p$ is soft, the mapping $p_A:\overset{-1}{p}(A)\rightarrow A$ is soft. Equivalently, if $\mathscr{F}$ is a soft sheaf on B, the sheaf induced on a closed subspace A is soft.

#### Proposition 6 {#ta-i-s3-prop-6 .statement tag=01OO}

Let B be a topological space, $\mathscr{F}$ a sheaf on B and $(A_i)_{i\in I}$ a locally finite closed covering of B. In order that the sheaf $\mathscr{F}$ be soft, it is necessary and sufficient that, for every $i\in I$, the induced sheaf $\mathscr{F}_{A_i}$ be soft.

The condition is obviously necessary. Let us prove that it is sufficient. Let us denote by $p: E\rightarrow B$ the étale B-space $E_{\mathscr{F}}$ associated with the sheaf $\mathscr{F}$. Let A be a closed subspace of B and $s: A\rightarrow E$ a continuous section of $p$ over A; it is a question of proving that $s$ possesses a continuous extension to B. For every subset J of I, put $A_J=\bigcup_{i\in J}A_i$; the set $A_J$ is closed in B (TG, I, p. 6, prop. 4).

Let $\mathscr{S}$ be the set of pairs $(J, t)$ where J is a subset of I and $t$ a continuous section of E over $A_J$ which coincides with $s$ in $A\cap A_J$. Let us make $\mathscr{S}$ into an ordered set by the ordering relation denoted by $\leqslant$ for which $(J, t)\leqslant (J', t')$ if $J\subset J'$ and $t'|A_J=t$. For $\sigma = (J, t)\in \mathscr{S}$, we write $J_{\sigma}= J$ and $t_{\sigma}=t$. Let us show that the ordered set $\mathscr{S}$ is inductive. Let S be a totally ordered subset of $\mathscr{S}$. Put $J =\bigcup_{\sigma\in S}J_{\sigma}$; this is a subset of I. One then defines a section $t$ of E over $A_J$ by setting $t(x) =t_{\sigma}(x)$, if $x\in A_{J_{\sigma}}$; thus $t|A\cap A_J=s$. Let $j\in J$ and let $\sigma \in S$ be such that $j\in J_{\sigma}$; since $t|A_j=t_{\sigma}|A_j$, the restriction of $t$ to $A_j$ is continuous. It then follows from TG, I, p. 19, Prop. 4 that $t$ is continuous. Thus, $(J, t)$ is an element of $\mathscr{S}$; by construction, it is an upper bound of S. This proves that the set $\mathscr{S}$ is inductive. It therefore possesses a maximal element $(J, t)$ (E, III, p. 20, th. 2).

Let us reason by contradiction, supposing that J $= I\not$ . Let $i$ be an element of I-J. Put $A'= (A_i\cap A)\cup (A_i\cap A_J)$ and define a section $s'$ of E over $A'$ by:

$'s(a)$ for $a\in A_i\cap A$,

$$
s(a) =
$$

$t(a)$ for $a\in A_i\cap A_J$,

which is possible since $s$ and $t$ coincide on $A\cap A_J$. Moreover, since $A_i\cap A$ and $A_i\cap A_J$ are closed, the section $s'$ is continuous (TG, I, p. 19, prop. 4). By hypothesis, there exists a continuous section $s_i: A_i\rightarrow E$ extending $s'$. Since the restrictions of $s_i$ and $t$ to $A_J\cap A_i$ are equal, the continuous section $t': A_{J\cup \{i\}}\rightarrow E$ which coincides with $t$ on $A_J$ and with $s_i$ on $A_i$ is a continuous section of $p$ over $A_{J\cup \{i\}}$, extending $s|A\cap A_{J\cup \{i\}}$. We then have $(J, t)<(J\cup  \{i\}, t')$, which contradicts the hypothesis that $(J, t)$ is maximal.

Thus, J = I, hence $A_J= B$ and $t$ is a continuous section of E over B extending $s$.

#### Corollary 1 {#ta-i-s3-prop-6-cor-1 .statement tag=01OP}

Let B be a paracompact space, $\mathscr{F}$ a sheaf on B and $(U_i)_{i\in I}$ an open covering of B. If, for every $i\in I$, the induced sheaf $\mathscr{F}|U_i$ is soft, then the sheaf $\mathscr{F}$ is soft.

There exists in fact a locally finite closed covering $(F_j)_{j\in J}$ finer than the covering $(U_i)_{i\in I}$ (TG, IX, p. 49, prop. 4 and p. 48, cor. 1). Consequently, for every $j\in J$, the sheaf $\mathscr{F}|F_j$ is soft and the proposition implies that the sheaf $\mathscr{F}$ is soft.

#### Corollary 2 {#ta-i-s3-prop-6-cor-2 .statement tag=01OQ}

Let B be a paracompact space, $\mathscr{F}$ a sheaf on B and $(A_i)_{i\in I}$ a locally finite closed covering of B. In order that the sheaf $\mathscr{F}$ be soft, it is necessary and sufficient that the following condition be satisfied:

For every $i\in I$, every closed subset A of $A_i$, every open set V of B containing A and every element $s$ of $\mathscr{F}(V)$, there exist an open neighbourhood U of $A_i$ in B, an element $t$ of $\mathscr{F}(U)$ and an open neighbourhood W of A in B contained in $U\cap V$ such that $t|W =s|W$.

Suppose that the sheaf $\mathscr{F}$ is soft, and let us show that the condition is satisfied. Let $i\in I$, let A be a closed subset of $A_i$, let V be an open subset of B containing A and let $s$ be an element of $\mathscr{F}(V)$. Put $s_0=\sigma_{\mathscr{F}}(s)$. It is a continuous section over V of the étalé space $E_{\mathscr{F}}$. Since $A_i$ is closed, A is closed in B and $s_0|A$ extends to a section $t_0: B\rightarrow E_{\mathscr{F}}$, by definition of a soft sheaf. The sections $s_0$ and $t_0|V$ of the étalé space over V $E_{\mathscr{F}}\times_BV$ coincide on A, hence on a neighbourhood W of A (I, p. 34, prop. 11, b)).

Conversely, suppose that the condition of the corollary is satisfied. By proposition 6, it is enough to prove that, for every $i\in I$, the sheaf $\mathscr{F}_{A_i}$ is soft. Let A be a closed subset of $A_i$ and let $s_0$ be a section of the etale space of $\mathscr{F}|A_i$ over A, that is, a continuous section over A of the etale space $E_{\mathscr{F}}$. Since A is closed in B and since B is paracompact, $s_0$ extends to a section $s$ over a neighbourhood V of A in B (I, p. 37, th. 2). By hypothesis, there exists an open neighbourhood U of $A_i$ in B and a section $t$ of $E_{\mathscr{F}}$ over U which coincides with $s$ on a neighbourhood of A. The restriction of $t$ to $A_i$ is a section of $\mathscr{F}_{A_i}$ which extends $s_0$. The sheaf $\mathscr{F}_{A_i}$ is therefore soft. By proposition 6, the sheaf $\mathscr{F}$ is soft.

### 10. Sheaves of structures

Suppose given a Species of structures Σ and a notion of $\sigma$-morphism relative to this Species of structures.

Let B be a topological space.

A presheaf $\mathscr{F}$ on B is said to be with values in the Species of structures Σ if, for every open set U of B, the set $\mathscr{F}(U)$ is endowed with a structure of Species Σ and if the restriction mappings are $\sigma$-morphisms.

Such a presheaf will be said to be a sheaf with values in the Species of structures Σ if, moreover, it is a sheaf of sets.

If $\mathscr{F}$ and $\mathscr{G}$ are presheaves with values in the Species of structures Σ, a morphism $\varphi$ is said to be a morphism of presheaves with values in Σ if, for every open set U, the mapping $\varphi (U)$ is a $\sigma$-morphism.

Thus one speaks, for example, of sheaves of groups, of abelian groups, of $k$-modules (for a fixed ring $k$), of rings, of $k$-algebras (for a fixed commutative ring $k$).

The sheaf on B of mappings with values in a group (resp. an abelian group, resp. a $k$-module, resp. a ring, resp. a $k$-algebra) is naturally endowed with a structure of sheaf of groups (resp. of abelian groups, resp. of $k$-modules, resp. of rings, resp. of $k$-algebras). If X is a differentiable manifold of class $C^r$ over $\mathbf{R}$, the sheaf $\mathscr{C}^r(X;\mathbf{R})$ of numerical functions of class $C^r$ is a sheaf of $\mathbf{R}$-algebras, and the sheaf on X of sections of class $C^r$ of a vector bundle E over X is a sheaf of $\mathbf{R}$-vector spaces; a differential operator defines a morphism of sheaves of $\mathbf{R}$-vector spaces.

For these Species of structures Σ, it follows from the construction which we have given that the sheaf $\widetilde{F}$ associated with a presheaf $\mathscr{F}$ with values in the Species of structures Σ (groups, abelian groups, $k$-modules, rings, $k$-algebras) is a sheaf with values in this Species of structures, and that the canonical morphism $j_{\mathscr{F}}:\mathscr{F}\rightarrow \widetilde{\mathscr{F}}$ is a morphism of presheaves with values in the Species of structures Σ.

For example, the sheaf on B of mappings with values in a group is naturally endowed with a structure of sheaf of groups.

Let A and B be topological spaces and let $u: A\rightarrow B$ be a continuous mapping. If $\mathscr{F}$ is a (pre)sheaf on A with values in the Species of structures Σ, the same is true of the direct image (pre)sheaf $u_*(\mathscr{F})$ of the (pre)sheaf $\mathscr{F}$ under $u$.

Suppose moreover that the Species of structures Σ is that of groups, abelian groups, $k$-modules, rings or $k$-algebras. If $\mathscr{G}$ is a (pre)sheaf on B with values in the Species of structures Σ, then the sheaf $u^*\mathscr{G}$ on A, inverse image of the presheaf $\mathscr{G}$ by the mapping $u$, is endowed with a sheaf structure with values in Σ. In this case, the adjunction morphisms $\alpha$ and $\beta$ are morphisms of presheaves with values in the Species of structures Σ. In particular, if $\varphi :\mathscr{G}\rightarrow u_*\mathscr{F}$ is a morphism of presheaves with values in Σ, the same is true of the morphism $\varphi^{\sharp}$; if $\psi :u^*(\mathscr{G})\rightarrow \mathscr{F}$ is a morphism of presheaves with values in Σ, the same is true of the morphism $\psi^{\flat}$.

## EXERCISES {#ta-i-s3-exercises}

See the [exercises for § 3](exercises/s3/).
