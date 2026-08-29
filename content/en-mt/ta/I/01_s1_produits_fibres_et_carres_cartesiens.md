---
book: ta
book_title: Topologie algébrique
chapter: I
chapter_title: REVÊTEMENTS
section: 1
section_title: Produits fibrés et carrés cartésiens
lang: en
source: ta-i-iv-fr
book_pages: TA I.1-TA I.24, TA I.139
pdf_pages: 0017-0040, 0155-0155
extraction: native
subsections:
    - "no": 1
      title: Structure de B-espace
      page: 1
      pdf_page: 17
    - "no": 2
      title: Opérations sur les B-espaces
      page: 2
      pdf_page: 18
    - "no": 3
      title: Produit fibré de deux B-espaces
      page: 3
      pdf_page: 19
    - "no": 4
      title: Changement de base
      page: 4
      pdf_page: 20
    - "no": 5
      title: Produit fibré d’une famille de B-espaces
      page: 5
      pdf_page: 21
    - "no": 6
      title: Carrés cartésiens
      page: 6
      pdf_page: 22
    - "no": 7
      title: Carrés cartésiens construits par passage aux sous-espaces
      page: 9
      pdf_page: 25
    - "no": 8
      title: Carrés cartésiens construits par produits, produits fibrés et sommes
      page: 11
      pdf_page: 27
    - "no": 9
      title: Composition de carrés cartésiens
      page: 15
      pdf_page: 31
    - "no": 10
      title: Applications strictes
      page: 17
      pdf_page: 33
    - "no": 11
      title: Applications universellement strictes
      page: 20
      pdf_page: 36
statements: 44
exercises: 2
content_sha256: 73da3f125059daba7ca5accf87dc18d7a25a1c3ad2a43b8a6572294c162df91a
translated_from: content/fr/ta/I/01_s1_produits_fibres_et_carres_cartesiens.md
source_lang: fr
translation_method: machine
source_content_sha256: 3d812fa4803abbe5bd107374726b69bde6a21ada1b7be0aa98125d4d9ada3bb3
translation_model: gpt-5.4
translation_run: translate-en-mt-72ca6bd3
glossary_version: 34
glossary_terms_sha256: 317ad8ad8d591a633db89c64a5e9b4ccfc57aa3615c100fe8d811a5206638b37
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 1. FIBRED PRODUCTS AND CARTESIAN SQUARES

### 1. Structure of a B-space

Let B be a topological space.

#### Definition 1 {#ta-i-s1-def-1 .statement tag=01L9}

A topological B-space (or simply a B-space) is a topological space X, endowed with a continuous mapping $p$ of X into B. The mapping $p$ is called the projection of the B-space X.

Let X, $X'$ be B-spaces and $p,p'$ their respective projections. A B-morphism of X into $X'$ is a continuous mapping $f$ of X into $X'$ such that $p'\circ f=p$.

It is sometimes convenient to denote by $(X, p)$ the B-space obtained by endowing the topological space X with the continuous mapping $p$.

The composite of two B-morphisms is a B-morphism. The isomorphisms of B-spaces, also called B-isomorphisms, are the B-morphisms which are homeomorphisms.

Thus, if one calls a B-space structure on a set X the datum of a topology on X and of a continuous mapping $p: X\rightarrow B$, one can take the B-morphisms as morphisms of the B-space structure (E, IV, p. 11).

© N. Bourbaki and Springer-Verlag Berlin Heidelberg 2  016

N. Bourbaki, Algebraic Topology, DOI 10.1007/978-3-662-49361-8_1  1

Let X, $X'$ be B-spaces. We denote by $\mathscr{C}_B(X; X')$ the set of B-morphisms of X into $X'$, by Isom$_B(X; X')$ the set of B-isomorphisms of X into $X'$, and by Aut$_B(X)$ the set of B-automorphisms of X, that is to say of B-isomorphisms of X into X.

Let X be a B-space and $p$ its projection. If B is endowed with the B-space structure whose projection is Id$_B$, the set $\mathscr{C}_B(B; X)$ is the set of continuous sections (E, II, p. 18, Definition 11) of $p$.

Let X be a B-space, $p$ its projection and $b$ a point of B. The subspace $\overset{-1}{p}(b)$ of X is called the fibre of X at $b$ (or the fibre of $p$ at $b$) and denoted by $X_b$. In order that a continuous mapping $f$ of X into a B-space $X'$ be a B-morphism, it is necessary and sufficient that $f(X_b)$ be contained in $X'_b$ for every $b\in B$.

Let X be a B-space and $p$ its projection. Let $f$ be a continuous mapping of a topological space $B'$ into B. A continuous mapping $g: B'\rightarrow X$ such that $p\circ g=f$ is called a continuous lifting of $f$ to X. In other words, if $B'$ is endowed with the B-space structure of projection $f$, the continuous liftings of $f$ to X are the B-morphisms of $B'$ into X.

### 2. Operations on B-spaces

Let B be a topological space.

Let X be a B-space and $p$ its projection. Every topological subspace Y of X is endowed with the B-space structure whose projection is $p|Y$. Let A be a subspace of B; endowed with the mapping $p_A:\overset{-1}{p}(A)\rightarrow A$ deduced from $p$ by passing to subsets, the topological space $\overset{-1}{p}(A)$ is an A-space. It is called the A-space induced by $(X, p)$ over A and is sometimes denoted by $X_A$.

Let $(X_i)_{i\in I}$ be a family of B-spaces, and let $p_i$ be the projection of $X_i$. The sum space $X =\coprod_{i\in I}X_i$ (TG, I, p. 15), endowed with the mapping $p: X\rightarrow$ B defined by $p(i, x) =p_i(x)$ (for $i\in$ I and $x\in X_i$), is a B-space called the sum of the family of B-spaces $(X_i)_{i\in I}$. The canonical injections $X_i\rightarrow X$ are B-morphisms.

Let X be a B-space, $p$ its projection, and let R be an equivalence relation on X. Let us denote by $X/R$ the quotient space (TG, I, p. 20, def. 3). If the mapping $p: X\rightarrow B$ is compatible with the relation R (E, II, p. 44), the mapping $p': X/R\rightarrow B$ deduced from $p$ by passing to the quotient is continuous (TG, I, p. 21, prop. 6); the B-space obtained by endowing $X/R$ with the projection $p'$ is then called the quotient B-space of X by the relation R.

### 3. Fibred product of two B-spaces

Let B be a topological space, X and $X'$ B-spaces, $p$ and $p'$ their respective projections. Let us denote by $X\times_BX'$ the topological subspace of $X\times X'$ formed by the pairs $(x, x')$ such that $p(x) =p'(x')$. The mapping $q: X\times_BX'\rightarrow B$ defined by $q(x, x') =p(x)$ is continuous.

#### Definition 2 {#ta-i-s1-def-2 .statement tag=01LA}

The topological space $X\times_BX'$ is called the fibred product of X and $X'$ over B. The B-space obtained by endowing $X\times_BX'$ with the mapping $q$ is called the product B-space of X and $X'$.

The restrictions to $X\times_BX'$ of the projections of $X\times X'$ into X and into $X'$ are again denoted by pr$_1$ and pr$_2$ and called the first and second projections of the fibred product. They are continuous and are B-morphisms, for one has $q=p\circ$ pr$_1=p'\circ$ pr$_2$.

It should be noted that $X\times_BX'$ may be empty even if X and $X'$ are non-empty: in fact, the relation $X\times_BX'=\emptyset$ is equivalent to saying that $p(X)$ and $p'(X')$ are disjoint.

Let Y be a B-space and $u: Y\rightarrow X,u': Y\rightarrow X'$ B-morphisms. There exists a unique B-morphism $v: Y\rightarrow X\times_BX'$ such that pr$_1\circ v=u$ and pr$_2\circ v$ = $u'$ (universal property of the product B-space of two B-spaces): this is the mapping $y\mapsto (u(y), u'(y))$ of Y into $X\times_BX'$, which is sometimes denoted by $(u, u')$.

Let $X,X',Y,Y'$ be B-spaces, let $f: X\rightarrow Y,f': X'\rightarrow Y'$ be B-morphisms. The mapping $(x, x')\mapsto (f(x), f'(x'))$ is a B-morphism of $X\times_BX'$ into $Y\times_BY'$, which is denoted by $f\times_Bf'$ and is called the extension of $f$ and $f'$ to fibred products.

#### Example 1 {#ta-i-s1-n3-exa-1 .statement tag=01LB}

Let X and $X'$ be B-spaces; then the mapping $(x, x')\mapsto (x', x)$ defines a B-isomorphism of $X\times_BX'$ onto $X'\times_BX$.

#### Example 2 {#ta-i-s1-n3-exa-2 .statement tag=01LC}

Let X, $X',X''$ be B-spaces and let $p,p',p''$ be their respective projections. The product B-space $(X\times_BX')\times_BX''$ is the topological subspace $X\times_BX'\times_BX''$ of $X\times X'\times X''$ formed by the triples $(x, x', x'')$ such that $p(x) =p'(x') =p''(x'')$, endowed with the projection $q: X\times_BX'\times_BX''\rightarrow B$ defined by $q(x, x', x'') =p(x)$.

#### Example 3 {#ta-i-s1-n3-exa-3 .statement tag=01LD}

Let X be a B-space and $p$ its projection. The fibred product $X\times_BX$ of X and X over B is called the fibred square of X. It is the subspace of $X\times X$ formed by the pairs $(x, x')$ such that $p(x) =p(x')$. It is endowed with the structure of a B-space whose projection is the mapping $(x, x')\mapsto$ $p(x)$. The diagonal $\Delta_X$ of $X\times X$ (E, II, p. 13) is contained in $X\times_BX$; it is also called the diagonal of $X\times_BX$. The mapping $x\mapsto (x, x)$ of X into $X\times_BX$ is a B-morphism, called the diagonal B-morphism and often denoted by $\delta_X$; it defines a B-isomorphism of X onto $\Delta_X$ (TG, I, p. 25, cor. 2).

#### Example 4 {#ta-i-s1-n3-exa-4 .statement tag=01LE}

Let $(B_i)_{i\in I}$ be a family of topological spaces and let, for each $i\in I$, $(X_i, p_i)$ and $(Y_i, q_i)$ be $B_i$-spaces. Put $B =\prod_{i\in I}B_i$, $X =\prod_{i\in I}X_i$ and $Y =\prod_{i\in I}Y_i$. Endowed with the continuous mapping $p=\prod_ip_i$ (resp. $q=\prod_iq_i$), the topological space X (resp. Y) is a B-space. By the associativity isomorphism of the topological products of $\prod_i(X_i\times Y_i)$ onto $(\prod_iX_i)\times (\prod_iY_i) = X\times Y$ (TG, I, p. 25, prop. 2), the subspace $\prod_i(X_i\times_{B_i}Y_i)$ of $\prod_i(X_i\times Y_i)$ is identified with $X\times_BY$.

#### Example 5 {#ta-i-s1-n3-exa-5 .statement tag=01LF}

Let $(X_i)_{i\in I}$ and $(Y_j)_{j\in J}$ be families of B-spaces. Let X and Y be their sums. For each $(i, j)\in I\times J$, the mapping $(x, y)\mapsto$ $((i, x),(j, y))$ is a B-isomorphism of $X_i\times_BY_j$ onto the subspace $(\{i\} \times X_i)\times_B(\{j\} \times Y_j)$ of $X\times_BY$. Since the latter form a partition of $X\times_BY$ into open subsets, the mapping

$$
h:\coprod_{(i,j)\in I\times J}(X_i\times_BY_j)\rightarrow X\times_BY
$$

defined by $h((i, j),(x, y)) = ((i, x),(j, y))$ is a B-isomorphism.

### 4. Change of base

Let B, $B'$ be topological spaces and $f: B'\rightarrow B$ a continuous mapping. Let X be a B-space. The mapping $f$ endows $B'$ with a structure of B-space, which makes it possible to define the fibred product $B'\times_BX$. The latter, endowed with the mapping pr$_1: B'\times_BX\rightarrow B'$, is a $B'$-space called the $B'$-space deduced from the B-space X by the base change $f: B'\rightarrow B$ (or by base change from B to $B'$ following $f$). It is also called the $B'$-space inverse image of X by $f$. It is denoted by $f^*(X)$, or sometimes $X_{B'}$ when there is no possible confusion about the mapping $f$.

When $B'$ is a subspace of B and $f: B'\rightarrow B$ is the canonical injection, the mapping $(b', x)\mapsto x$ of $B'\times_BX'$ into $\overset{-1}{p}(B')$ (where $p$ is the projection of X) is a $B'$-isomorphism of $f^*(X)$ onto the $B'$-space induced by X over $B'$.

Let Y be a second B-space and $u: X\rightarrow Y$ a B-morphism. The mapping Id$_{B'}\times_Bu: B'\times_BX\rightarrow B'\times_BY$ is a $B'$-morphism, called the $B'$-morphism deduced from the B-morphism $u$ by the base change $f: B'\rightarrow B$ and sometimes denoted by $f^*(u)$, or $u_{B'}$ when there is no possible confusion about the mapping $f$. It is the unique $B'$-morphism $v$ of $B'\times_BX$ into $B'\times_BY$ such that pr$_2\circ v=u\circ$ pr$_2$.

Let $B''$ be a topological space and let $g: B''\rightarrow B'$ be a continuous mapping. Then the mapping given by $(b'',(b', x))\mapsto (b'', x)$ is an isomorphism of $B''$-spaces of $g^*(f^*(X))$ onto $(f\circ g)^*(X)$, which will be said to be canonical.

### 5. Fibred product of a family of B-spaces

Let $(X_i)_{i\in I}$ be a family of B-spaces. Let $p_i: X_i\rightarrow B$ be their projections. Let $\prod_BX_i$ denote the topological subspace of $B\times \prod_{i\in I}X_i$ formed by the pairs $(b,(x_i)_{i\in I})$ such that $p_i(x_i) =b$ for all $i\in I$. The mapping $p:\prod_BX_i\rightarrow B$ defined by $p(b,(x_i)_{i\in I}) =b$ is continuous.

#### Definition 3 {#ta-i-s1-def-3 .statement tag=01LG}

The topological space $\prod_BX_i$ is called the fibred product of the family $(X_i)_{i\in I}$ over B. The B-space obtained by endowing $\prod_BX_i$ with the mapping $p$ is called the product B-space of the family $(X_i)_{i\in I}$.

Let $j\in I$. The mapping $(b, x)\mapsto$ pr$_j(x)$ of $\prod_BX_i$ into $X_j$ is called the projection of index $j$ of the fibred product and is again denoted by pr$_j$. It is continuous. It is a B-morphism, for one has $p=p_j\circ$ pr$_j$.

Let Y be a B-space and $q$ its projection. For each $i\in$ I, let $u_i: Y\rightarrow X_i$ be a B-morphism. There exists a unique B-morphism $v: Y\rightarrow$ $\prod_BX_i$ such that pr$_i\circ v=u_i$ for each $i\in I$ (universal property of the product B-space): it is the mapping of Y into $\prod_BX_i$, defined by $y\mapsto (q(y),(u_i(y))_{i\in I})$, which is sometimes denoted by $(u_i)_{i\in I}$.

Let $(X_i)_{i\in I}$ and $(Y_i)_{i\in I}$ be families of B-spaces and, for each $i\in I$, let $f_i: X_i\rightarrow Y_i$ be a B-morphism. The mapping $(b,(x_i)_{i\in I})\mapsto$ $(b,(f_i(x_i))_{i\in I})$ is a B-morphism of $\prod_BX_i$ into $\prod_BY_i$ which is denoted by $\prod_Bf_i$ and is called the extension of the family $(f_i)_{i\in I}$ to the fibred products.

#### Example 1 {#ta-i-s1-n5-exa-1 .statement tag=01LH}

When the set I is empty, the set $\prod_{i\in I}X_i$ consists of a single element and the B-space $\prod_BX_i$ is identified with B (endowed with the projection Id$_B$).

#### Example 2 {#ta-i-s1-n5-exa-2 .statement tag=01LI}

When I is not empty, one deduces from the mapping $(b, x)\mapsto x$ of $B\times \prod_{i\in I}X_i$ into $\prod_{i\in I}X_i$, by passing to subspaces, a homeomorphism of $\prod_BX_i$ onto the subspace of $\prod_{i\in I}X_i$ formed by the families $(x_i)_{i\in I}$ such that $p_i(x_i) =p_j(x_j)$ for all $i, j\in I$. This subspace will be called, by abuse, the fibred product of the family $(X_i)_{i\in I}$.

#### Example 3 {#ta-i-s1-n5-exa-3 .statement tag=01LJ}

When the set I is a set with one element $\alpha$ (resp. with two elements $\alpha$ and $\beta$; resp. with three elements $\alpha ,\beta ,\gamma$ ), the mapping pr$_{\alpha}$ (resp. (pr$_{\alpha}$, pr$_{\beta}$) ; resp. (pr$_{\alpha}$, pr$_{\beta}$, pr$_{\gamma}$)) of $\prod_BX_i$ into $X_{\alpha}$ (resp. into $X_{\alpha}\times_BX_{\beta}$; resp. into $X_{\alpha}\times_BX_{\beta}\times_BX_{\gamma}$) is a B-isomorphism. This will allow us to deduce the properties of the fibred product of two or three B-spaces from those of the fibred product of families of B-spaces.

Let $(X_i)_{i\in I}$ be a family of B-spaces and let J be a subset of I. From the mapping Id$_B\times$ pr$_J$ of $B\times \prod_{i\in I}X_i$ into $B\times \prod_{i\in J}X_i$, by passing to subsets, one deduces a B-morphism $\prod_{i\in IB}X_i\rightarrow \prod_{i\in JB}X_i$. One

again denotes it by pr$_J$ and calls it the projection of index J of the fibre product.

Let $(X_i)_{i\in I}$ be a family of B-spaces. Let $(J_{\lambda})_{\lambda\in L}$ be a partition

of I. The mapping (pr$_{J_{\lambda}}$)$_{\lambda\in L}$ of $\prod_{i\in IB}X_i\rightarrow \prod_{\lambda\in LB}(\prod_{i\in J_{\lambda}B}X_i)$ is a

B-isomorphism ("associativity" of fibre products of B-spaces).

### 6. Cartesian Squares

Let B, $B'$, X, $X'$ be topological spaces and let $f: B'\rightarrow B$, $f': X'\rightarrow X,p: X\rightarrow B,p': X'\rightarrow B'$ be continuous mappings. Such a quadruple $(f, f', p, p')$ may be represented by a diagram

${X'}^{f'}$ X

$$
p'p \tag{1}
$$

${B'}^f$ B

(E, II, p. 14). One then says: "Consider square diagram (1)," or simply "square (1)," instead of saying: "Consider the quadruple $(f, f', p, p')$ of continuous mappings." One says that square (1) is commutative if the equality

$$
f\circ p'=p\circ f'
$$

is satisfied. In this case, one often endows $B'$, X and $X'$ with the structures of B-spaces defined by the mappings $f,p$ and $f\circ p'=p\circ f'$ respectively; the mappings $p'$ and $f'$ are then B-morphisms.

#### Definition 4 {#ta-i-s1-def-4 .statement tag=01LK}

One says that square (1) is a Cartesian square of topological spaces (or, simply, that it is Cartesian) if it is commutative and if, for every topological space Y and every pair of continuous mappings $u: Y\rightarrow B',v: Y\rightarrow X$ such that $f\circ u=p\circ v$, there exists a unique continuous mapping $w: Y\rightarrow X'$ such that $p'\circ w=u$ and $f'\circ w=v$.

For square (1) to be Cartesian, it is necessary and sufficient that the square

$$
{X'}^{p'}B'
$$

$$
(1')f'f
$$

X $^p$ B

be Cartesian.

#### Proposition 1 {#ta-i-s1-prop-1 .statement tag=01LL}

For square (1) to be Cartesian, it is necessary and sufficient that it be commutative and that, for every B-space Y and every pair of B-morphisms $u: Y\rightarrow B',v: Y\rightarrow X$, there exist a unique B-morphism $w: Y\rightarrow X'$ such that $p'\circ w=u$ and $f'\circ w=v$.

Suppose that square (1) is Cartesian. Let Y be a B-space and let $u: Y\rightarrow B',v: Y\rightarrow X$ be B-morphisms. The mappings $f\circ u$ and $p\circ v$ are both equal to the projection of the B-space Y; the unique continuous mapping $w$ such that $p'\circ w=u$ and $f'\circ w=v$ is then a B-morphism. This proves the necessity of the condition.

Conversely, suppose this condition satisfied. Let Y be a topological space and let $u: Y\rightarrow B',v: Y\rightarrow X$ be continuous mappings such that $f\circ u=p\circ v$. When Y is endowed with the structure of a B-space defined by $f\circ u,u$ and $v$ are B-morphisms. Every continuous mapping $w: Y\rightarrow X'$ such that $p'\circ w=u$ and $f'\circ w=v$ being a B-morphism, there exists one and only one.

#### Proposition 2 {#ta-i-s1-prop-2 .statement tag=01LM}

Let B, $B'$ and X be topological spaces and let $p: X\rightarrow B,f: B'\rightarrow B$ be continuous mappings.

a) The square

$B'\times_BX^{pr_2}$ X

(2) pr$_{_1}p$

${B'}^f$ B

is a Cartesian square.

b) For every commutative square

${X'}^{f'}$ X

$$
p'p \tag{3}
$$

${B'}^f$ B

there exists a unique continuous mapping $h: X'\rightarrow B'\times_BX$ such that pr$_1\circ h=p'$ and pr$_2\circ h=f'$.

c) The commutative square (3) is cartesian if and only if $h$ is a homeomorphism.

Assertion a) results from Prop. 1 and from the universal property of the product B-space of two B-spaces (I, p. 3). Assertion b) follows from it.

If square (3) is cartesian, there exists a unique continuous mapping $h': B'\times_BX\rightarrow X'$ such that $f'\circ h'$ = pr$_2$ and $p'\circ h'=$ pr$_1$. We have $f'\circ h'\circ h=f'$ and $p'\circ h'\circ h=p'$, whence $h'\circ h=$ Id$_{X'}$ since square (3) is cartesian. We have pr$_1\circ h\circ h'$ = pr$_1$ and pr$_2\circ h\circ h'$ = pr$_2$, whence $h\circ h'=$ Id$_{B'\times_BX}$ since square (2) is cartesian. This proves that $h$ is a homeomorphism.

Conversely, suppose that $h$ is a homeomorphism; since square (2) is cartesian, square (3) is also cartesian.

The mapping $h: X'\rightarrow B'\times_BX$ whose existence and uniqueness is asserted by assertion b) of the preceding proposition will be said to be canonical: it is the mapping denoted by $(p', f')$ in I, p. 3.

#### Proposition 3 {#ta-i-s1-prop-3 .statement tag=01LN}

Let

${X'}^{f'}$ X

$p'p$

${B'}^f$ B

be a cartesian square. For every continuous section $s$ of $p'$, the mapping $f'\circ s$ is a continuous lifting of $f$ to X. The mapping $s\mapsto f'\circ s$ is a bijection of $\mathscr{C}_{B'}(B'; X')$ onto $\mathscr{C}_B(B'; X)$.

If $s: B'\rightarrow X'$ is a continuous section of $p'$, we have $p\circ f'\circ s=$ $f\circ p'\circ s=f$, which proves that $f'\circ s$ is a continuous lifting of $f$ to X, i.e. a B-morphism from $B'$ into X. Conversely, let $g: B'\rightarrow X$ be a B-morphism. We have $f\circ$ Id$_{B'}=p\circ g$; there therefore exists, by definition of a cartesian square, a unique continuous mapping $s: B'\rightarrow X'$ such that $p'\circ s=$ Id$_{B'}$ and $f'\circ s=g$, whence the proposition.

### 7. Cartesian Squares Constructed by Passing to Subspaces

#### Proposition 4 {#ta-i-s1-prop-4 .statement tag=01LO}

Let

${X'}^{f'}$ X

$$
p'p \tag{4}
$$

${B'}^f$ B

be a cartesian square, and let $B_0,B'_0,X_0$ be subspaces of B, $B'$ and X respectively. Suppose that we have $f(B'_0)\subset B_0,p(X_0)\subset B_0$ and put $X'_0=(\overset{-1}{p}')(B'_0)\cap (\overset{-1}{f}')(X_0)$. Then the square

$$
{X'_0}^{f'_0}X_0
$$

$$
(4')p'_{_0}p_{_0}
$$

$$
{B'_0}^{f_0}B_0
$$

(where the mappings $f_0,f'_0,p_0,p'_0$ are deduced from $f,f',p,p'$ respectively by passing to the subsets) is cartesian.

Consider the canonical mapping $h: X'\rightarrow B'\times_BX$ deduced from commutative diagram (4). Since square (4) is Cartesian, $h$ is a

homeomorphism. By construction, one has $X'_0=\overset{-1}{h}(B'_0\times_{B_0}X_0)$ and the mapping $h_0: X'_0\rightarrow B'_0\times_{B_0}X_0$ deduced from commutative diagram ($4'$) is deduced from $h$ by passing to subsets. It is therefore a homeomorphism and square ($4'$) is Cartesian (Prop. 2).

#### Corollary {#ta-i-s1-n7-cor-1 .statement tag=01LP}

Let

${X'}^{f'}$ X

$p'p$

${B'}^f$ B

be a Cartesian square.

a) For every point $b'$ of $B'$, the mapping $f'$ induces a homeomorphism of the fibre $X'_{b'}$ of $p'$ onto the fibre $X_{f(b')}$ of $p$.

b) If the mapping $p$ is injective (resp. surjective, resp. bijective), the same is true of $p'$.

Let $b'$ be a point of $B'$. Put $b=f(b')$. For every $x'\in X'_{b'}$, one has $p(f'(x')) =f(p'(x')) =f(b') =b$, whence $f'(x')\in X_b$. This proves that

one has $X'_{b'}\subset (\overset{-1}{f}')(X_b)$. In Prop. 4, take $B_0=\{b\},B'_0=\{b'\}$ and $X_0= X_b$; one then has $X'_0= X'_{b'}$, whence assertion a).

For the mapping $p$ to be injective (resp. surjective, resp. bijective), it is necessary and sufficient that the cardinal of each of its fibres be less than (resp. greater than, resp. equal to) 1. Assertion b) follows.

#### Example {#ta-i-s1-n7-exa-1 .statement tag=01LQ}

Let $(X, p)$ be a B-space and A a subspace of B. The square

$\overset{-1}{p}(A)^j$ X

$$
p_{_A}p \tag{5}
$$

A $^i$ B

(where $i$ and $j$ are the canonical injections) is Cartesian.

In particular, if A and $A'$ are subspaces of the topological space B, the square

$$
A\cap A'A'
$$

(6)

A B

(where the arrows are the canonical injections) is Cartesian.

### 8. Cartesian Squares Constructed by Products, Fibre Products and Sums

#### Proposition 5 {#ta-i-s1-prop-5 .statement tag=01LR}

Let I be a set and, for every $i\in I$, let

$$
{X'_i}^{f'_i}X_i
$$

$$
p'_{_i}p_{_i} \tag{7}
$$

$$
{B'_i}^{f_i}B_i
$$

be a Cartesian square. The square

$$
\prod i\in IX'if'\prod i\in IXi
$$

$$
(7')p'p
$$

$$
\prod i\in IB'if\prod i\in IBi
$$

(where $f,f',p,p'$ are the extensions of the families $(f_i)$, $(f'_i)$, $(p_i)$, $(p'_i)$ to the products) is Cartesian.

Let Y be a topological space, let $u: Y\rightarrow \prod_iB'_i$ and $v: Y\rightarrow \prod_iX_i$ be continuous mappings such that $f\circ u=p\circ v$. For $i\in I$, put $u_i$ = pr$_i\circ u$ and $v_i=$ pr$_i\circ v$; one has $f_i\circ u_i=p_i\circ v_i$ and there exists a unique continuous mapping $w_i: Y\rightarrow X'_i$ such that $p'_i\circ w_i=u_i$ and $f'_i\circ w_i=v_i$. Then the mapping $w= (w_i)$ is a continuous mapping of Y into $\prod_iX'_i$ such that $p'\circ w=u$ and $f'\circ w=v$, and it is the only one having these properties.

#### Corollary 1 {#ta-i-s1-prop-5-cor-1 .statement tag=01LS}

Let X be a B-space, let $p$ be its projection, and let F be a topological space. The square

$$\begin{array}{ccc} X\times F & \overset{\mathrm{pr}_1}{\longrightarrow} & X \\ {\scriptstyle p\times \mathrm{Id}_F}\big\downarrow & & \big\downarrow{\scriptstyle p} \\ B\times F & \overset{\mathrm{pr}_1}{\longrightarrow} & B \end{array} \tag{8}$$

is cartesian.

Let P be a topological space consisting of a single point. Corollary 1 follows from Prop. 5 applied to the cartesian squares

$$\begin{array}{ccccccc} X & \overset{\mathrm{Id}_X}{\longrightarrow} & X & & F & \longrightarrow & P \\ {\scriptstyle p}\big\downarrow & & \big\downarrow{\scriptstyle p} & \text{and} & {\scriptstyle \mathrm{Id}_F}\big\downarrow & & \big\downarrow{\scriptstyle \mathrm{Id}_P} \\ B & \overset{\mathrm{Id}_B}{\longrightarrow} & B & & F & \longrightarrow & P \end{array}.$$

Let B and $B'$ be topological spaces and let $f: B'\rightarrow$ B be a continuous mapping. Let I be a set and, for each $i\in I$, let $X_i$ be a B-space, $X'_i$ a $B'$-space, and $f'_i: X'_i\rightarrow X_i$ a continuous mapping such that the square

$$
{X'_i}^{f'_i}X_i
$$

(9)

${B'}^f$ B

be commutative. There exists a unique continuous mapping

$$
f':\prod_{i\in IB'}X'_i\rightarrow \prod_{i\in IB}X_i
$$

such that pr$_i\circ f'=f'_i\circ$ pr$_i$ for every $i\in I$ and such that the square

$i\prod\in IB'X'if'i\prod\in I$B $Xi$

$$
(9')
$$

${B'}^f$ B be commutative (this last condition resulting from the others if I $=\not\emptyset$ ) $:$ it is the mapping deduced from the mapping

$$
f\times \prod_{i\in I}f'_i: B'\times \prod_{i\in I}X'_i\rightarrow B\times \prod_{i\in I}X_i
$$

by passing to the subsets. With these notations:

#### Corollary 2 {#ta-i-s1-prop-5-cor-2 .statement tag=01LT}

If the square (9) is cartesian for every $i\in I$, the square ($9'$) is cartesian.

From Prop. 5 one deduces a cartesian square

$$
B'\times \prod_i{X'_i}^{Id_B\times}\prod_{_i}^{f'_i}B\times \prod_iX_i
$$

$$
B'\times (B')^{If\times}\prod_{_i}^fB\times B^I
$$

Let $\Delta_{B'}$ and $\Delta_B$ denote the diagonals of $B'\times (B')^I$ and $B\times B^I$. The diagram

$i\prod\in IB'X'if'i\prod\in I$B $Xi$

$$
\Delta_{B'}\Delta_B
$$

deduced from the preceding one by passing to the subspaces is cartesian (I, p. 9, Prop. 4). It is identified with diagram ($9'$).

#### Example 1 {#ta-i-s1-n8-exa-1 .statement tag=01LU}

Let

${X'}^{f'}$ X

$p'p$

${B'}^f$ B

be a cartesian square. Then Corollary 2 yields a cartesian square

$$
X'\times_{B'}{X'}^{\varphi}X\times_BX
$$

${B'}^f$ B .

We have the relation $\overset{-1}{\varphi}(\Delta_X) = \Delta_{X'}$. In fact, by prop. 2 of I, p. 8, it is enough to consider the case where $X'= B'\times_BX$. Let then $((b, x),(b, x'))$ be an element of $X'\times_{B'}X'$ with $b\in B'$ and $x, x'\in X$. This element belongs to $\overset{-1}{\varphi}(\Delta_X)$ if and only if $x=x'$.

#### Proposition 6 {#ta-i-s1-prop-6 .statement tag=01LV}

Let I be a set and, for every $i\in I$, let

${X'_i}^{f'_i}$ X

$$
p'_{_i}p \tag{10}
$$

${B'_i}^{f_i}$ B

be a cartesian square. Let $X'$ and $B'$ be the sum spaces of the families $(X'_i)$ and $(B'_i)$ respectively. Let $f: B'\rightarrow B,f': X'\rightarrow X$ and $p': X'\rightarrow B'$ be the mappings deduced from the families $(f_i)$, $(f'_i)$ and $(p'_i)$ respectively. The square

${X'}^{f'}$ X

$$
(10')p'p
$$

${B'}^f$ B

is cartesian.

The mappings $f,f'$ and $p'$ are continuous. The commutativity of square ($10'$) follows from its definition. Let us denote by $h_i$ the canonical homeomorphism of $X'_i$ onto $B'_i\times_BX$ (I, p. 8, prop. 2) and by $h: X'\rightarrow B'\times_BX$ the canonical mapping (loc. cit.). We have $h=h''\circ h'$ where $h': X'\rightarrow \coprod(B'_i\times_BX)$ is the homeomorphism deduced from the $h_i$ and $h'':\coprod(B'_i\times_BX)\rightarrow (\coprod B'_i)\times_BX$ is that defined in example 5 of I, p. 4. We conclude by prop. 2 of I, p. 8.

#### Example 2 {#ta-i-s1-n8-exa-2 .statement tag=01LW}

Let $(X, p)$ be a B-space and let $(A_k)_{k\in K}$ be a family of subspaces of B. Let A be the sum space of the family $(A_k)_{k\in K}$ and let Y be the sum space of the family $(\overset{-1}{p}(A_k))_{k\in K}$; let us denote by $i: A\rightarrow B$, $j: Y\rightarrow X$ and $p': Y\rightarrow A$ the mappings deduced from the canonical injections of $A_k$ into B, the canonical injections of $\overset{-1}{p}(A_k)$ into X, and the mappings $p_{A_k}:\overset{-1}{p}(A_k)\rightarrow A_k$, for $k\in K$. The square

Y $^j$ X

$$
p'p \tag{11}
$$

A $^i$ B is cartesian; this follows from the example of I, p. 10 and from prop. 6.

### 9. Composition of cartesian squares

#### Proposition 7 {#ta-i-s1-prop-7 .statement tag=01LX}

Let

${X''}^{g'}X'{X'}^{f'}$ X

(12) $p''p'$ and (13) $p'p$

${B''}^gB'{B'}^f$ B

be commutative squares; consider the square

${X''}^{f'\circ g'}$ X

$$
p''p \tag{14}
$$

${B''}^{f\circ g}$ B .

It is commutative. If squares (12) and (13) are cartesian, the same is true of square (14). If squares (13) and (14) are cartesian, the same is true of square (12).

Square (14) is commutative, for we have $p\circ f'\circ g'=f\circ p'\circ g'=f\circ g\circ p''$.

Let us denote by $h': X''\rightarrow B''\times_{B'}X',h: X'\rightarrow B'\times_BX$ and $h'': X''\rightarrow B''\times_BX$ the canonical continuous mappings deduced from the commutative squares (12), (13) and (14). Moreover, let us denote

$$
j: B''\times_BX\rightarrow B''\times_{B'}(B'\times_BX)
$$

the continuous mapping which associates to $(b'', x)$ the element $(b'', g(b''), x)$. It is a homeomorphism and one has $j\circ h''=$ (Id$_{B''}\times_Bh$)$\circ h'$.

Suppose that square (13) is cartesian. Then $h$ is a homeomorphism (I, p. 8, prop 2), hence the mapping Id$_{B''}\times_Bh$ is a homeomorphism, and $h''$ is a homeomorphism if and only if $h'$ is one. This means that square (12) is cartesian if and only if square (14) is cartesian (loc. cit.).

With the notation of proposition 7, one sometimes says that square (14) is the square composed of squares (13) and (12). The first assertion expresses that the square composed of two cartesian squares is cartesian. In particular, the $B''$-spaces $g^*(f^*(X))$ and $(f\circ g)^*(X)$ are isomorphic.

#### Remark 1 {#ta-i-s1-n9-rem-1 .statement tag=01LY}

It may happen that squares (12) and (14) are cartesian without square (13) being so (I, p. 139, exerc. 2).

#### Remark 2 {#ta-i-s1-n9-rem-2 .statement tag=01LZ}

Let $p: X\rightarrow B$ and $f: B'\rightarrow B$ be continuous mappings. The mapping $g: B'\rightarrow B'\times B$ defined by $g(b') = (b', f(b'))$ is a homeomorphism of $B'$ onto the graph G of the mapping $f$ (TG, I, p. 25, cor. 2), and the fibred product $B'\times_BX$ is identified (I, p. 6) with the subspace of $B'\times X$, inverse image of G under the mapping Id$_{B'}\times p: B'\times X\rightarrow B'\times B$. By the example of I, p. 10 and cor. 1 of prop. 5 (I, p. 11), the squares

$B'\times_BX^iB'\times XB'\times X^{pr_2}$ X

pr$_1$ Id$_{B'}\times p$ and Id$_{B'}\times pp$

${B'}^gB'\times BB'\times B^{pr_2}$ B

(where $i$ denotes the canonical injection) are cartesian, and the cartesian square

$B'\times_BX^{pr_2}$ X

pr$_1p$

${B'}^f$ B

is their composite. In other words, every cartesian square is identified with the square composed of a cartesian square obtained by product (I, p. 11, cor. 1 of prop. 5, square (8)) and of a cartesian square obtained by passing to subspaces (I, p. 10, example, square (5)).

#### Remark 3 {#ta-i-s1-n9-rem-3 .statement tag=01M0}

Let

$X_1^{g_1}$ X $X_2^{g_2}$ X

(15) $p_{_1}p$ and (16) $p_{_2}p$

$B_1^{f_1}$ B $B_2^{f_2}$ B

be cartesian squares. Consider the square

$X_1\times_XX_2^g$ X

$$
p'p \tag{17}
$$

$B_1\times_BB_2^f$ B where $f$ (resp. $g$) is the mapping which defines the structure of B-space (resp. of X-space) of the fibred product $B_1\times_BB_2$ (resp. of the fibred product $X_1\times_XX_2$), and where $p'$ is the mapping deduced from $p_1\times p_2$ by passing to subsets. It is cartesian (I, p. 13, cor. 2 of prop. 5).

Consider then the following two commutative squares:

$$\begin{array}{ccc} X_1\times_XX_2 & \overset{\mathrm{pr}_1}{\longrightarrow} & X_1 \\ {\scriptstyle p'}\big\downarrow & & \big\downarrow{\scriptstyle p_1} \\ B_1\times_BB_2 & \overset{\mathrm{pr}_1}{\longrightarrow} & B_1 \end{array} \tag{18}$$

and

$$\begin{array}{ccc} X_1\times_XX_2 & \overset{\mathrm{pr}_2}{\longrightarrow} & X_2 \\ {\scriptstyle p'}\big\downarrow & & \big\downarrow{\scriptstyle p_2} \\ B_1\times_BB_2 & \overset{\mathrm{pr}_2}{\longrightarrow} & B_2 \end{array}. \tag{19}$$

Square (17) is composed of squares (15) and (18), as well as of squares (16) and (19). By prop. 7, squares (18) and (19) are cartesian.

### 10. Strict Mappings

#### Proposition 8 {#ta-i-s1-prop-8 .statement tag=01M1}

Let

$$\begin{array}{ccc} X' & \overset{f'}{\longrightarrow} & X \\ {\scriptstyle p'}\big\downarrow & & \big\downarrow{\scriptstyle p} \\ B' & \overset{f}{\longrightarrow} & B \end{array}$$

be a cartesian square. If the mapping $p$ is open ( resp. is proper, resp. has in a neighbourhood of each point a continuous section), the same is true of $p'$.

By remark 2, I, p. 16, it is enough to prove the proposition for cartesian squares of the following type:

$$\begin{array}{ccccccc} \overset{-1}{p}(A) & \overset{j}{\longrightarrow} & X & & X\times F & \overset{\mathrm{pr}_1}{\longrightarrow} & X \\ {\scriptstyle p_A}\big\downarrow & & \big\downarrow{\scriptstyle p} & \text{and} & {\scriptstyle p\times \mathrm{Id}_F}\big\downarrow & & \big\downarrow{\scriptstyle p} \\ A & \overset{i}{\longrightarrow} & B & & B\times F & \overset{\mathrm{pr}_1}{\longrightarrow} & B \end{array},$$

where F is a topological space, A a subspace of B, and $i,j$ the canonical injections. If the mapping $p$ is open, the mappings $p_A$ and $p\times$ Id$_F$ are open (TG, I, p. 30, prop. 2 and TG, I, p. 34, prop. 8). If the mapping $p$ is proper, the mappings $p_A$ and $p\times$ Id$_F$ are proper (TG, I, p. 72, prop. 3 and TG, I, p. 72, def. 1). If U is an open subset of B and $s: U\rightarrow X$ a continuous section of $p$ over U, the mapping $s|(A\cap U)$ is a continuous section of $p_A$ over $A\cap U$ and the mapping $s\times$ Id$_F$ is a continuous section of $p\times$ Id$_F$ over $U\times F$.

#### Remark 1 {#ta-i-s1-n10-rem-1 .statement tag=01M2}

With the notation of prop. 8, if $p$ is a closed mapping, this is not necessarily so for $p'($cf. TG, I, p. 72, example). However, if the mapping $p$ is closed and if A is a subspace of B, the mapping $p_A:\overset{-1}{p}(A)\rightarrow A$ is closed (TG, I, p. 30, prop. 2, a)).

#### Definition 5 {#ta-i-s1-def-5 .statement tag=01M3}

Let X and Y be topological spaces and $f: X\rightarrow Y$ a mapping. Let R be the equivalence relation associated with $f$, and

$$
X\rightarrow X/R-\overset{g}{\rightarrow}f(X)\rightarrow Y
$$

the canonical decomposition of $f$ (E, II, p. 44). One says that the mapping $f$ is strict if $g$ is a homeomorphism, when $X/R$ is endowed with the quotient topology and $f(X)$ with the topology induced by that of Y.

A strict mapping is continuous.

Let us recall (TG, I, p. 22, prop. 8) that, in order that a mapping $f$ be strict, it is necessary and sufficient that $f$ be continuous and that for every open (resp. closed) saturated subset A of X, the set $f(A)$ be open (resp. closed) in $f(X)$.

#### Example 1 {#ta-i-s1-n10-exa-1 .statement tag=01M4}

The composite of two strict mappings is not necessarily strict. In fact, every continuous mapping $f: X\rightarrow Y$ is the composite of the mapping pr$_2: X\times Y\rightarrow$ Y and of the mapping $x\mapsto (x, f(x))$ of X into $X\times Y$, which are both strict (TG, I, p. 26, prop. 5 and TG, I, p. 25, cor. 2). On the other hand, the composite of two strict and injective (resp. surjective) mappings is a strict mapping.

#### Example 2 {#ta-i-s1-n10-exa-2 .statement tag=01M5}

A continuous mapping which is open, or closed, or which possesses a continuous section, is strict. This follows from prop. 3 of TG, I, p. 32 and from prop. 9 of TG, I, p. 22.

#### Example 3 {#ta-i-s1-n10-exa-3 .statement tag=01M6}

In order that a continuous homomorphism of one topological group into another be a strict morphism (TG, III, p. 16, def. 1), it is necessary and sufficient that it be a strict mapping in the sense of Definition 5.

#### Proposition 9 {#ta-i-s1-prop-9 .statement tag=01M7}

Let X, Y and Z be topological spaces. Let $f: X\rightarrow Y$ be a continuous surjective mapping and $g: Y\rightarrow Z$ a mapping.

a) If $f$ is strict and if $g\circ f$ is continuous, the mapping $g$ is continuous.

b) If $g$ is continuous and if $g\circ f$ is strict, the mapping $g$ is strict.

c) If $f$ and $g\circ f$ are strict, $g$ is strict.

Let us prove assertion a). Let R denote the relation associated with $f$ in X; by hypothesis, the mapping of $X/R$ onto Y deduced from $f$ by passing to the quotient is a homeomorphism. The first assertion then follows from prop. 6 of I, p. 21.

Let us prove b). Let B be a closed saturated subset of Y for the relation defined by $g$ and let $A =\overset{-1}{f}(B)$. Since $f$ is continuous, A is closed in X, and A is saturated for the equivalence relation defined by $g\circ f$. Since $g\circ f$ is strict and $f$ is surjective, $g(B) =g\circ f(A)$ is therefore closed in Z. The continuous mapping $g$ is therefore strict.

Assertion c) results immediately from assertions a) and b).

#### Proposition 10 {#ta-i-s1-prop-10 .statement tag=01M8}

Let X be a topological space and let R be an equivalence relation in X. Let Y be a locally compact topological space. Let S be the equivalence relation in $X\times Y$ which is the product of the equivalence relation R in X and of the equality relation in Y. The canonical bijection $(X\times Y)/S\rightarrow (X/R)\times Y$ is a homeomorphism.

Recall that if U and V are topological spaces, $\mathscr{C}_c(U; V)$ denotes the set of continuous mappings of U into V, endowed with the topology of compact convergence (TG, X, p. 26, def. 1).

Let $p: X\rightarrow X/R$ and $q: X\times Y\rightarrow (X\times Y)/S$ be the canonical surjections. Let $g: (X\times Y)/S\rightarrow (X/R)\times Y$ denote the canonical bijection. It is continuous; let $h$ denote its inverse and let us prove that it is continuous.

The mapping $i: X\rightarrow \mathscr{C}_c(Y; X\times Y)$ such that, for every $x\in$ X, $i(x)$ is the mapping defined by $y\mapsto (x, y)$, is continuous (TG, X, p. 28, th. 3). The mapping $\widetilde{q}:\mathscr{C}_c(Y; X\times Y)\rightarrow \mathscr{C}_c(Y; (X\times Y)/S)$ which associates with a continuous mapping $\varphi$ the mapping $q\circ \varphi$, is continuous (TG, X, p. 29, prop. 9). Consequently, the mapping $\widetilde{q}\circ i: X\rightarrow \mathscr{C}_c(Y; (X\times Y)/S)$ is continuous. It is compatible with the equivalence relation R; the unique mapping $j: X/R\rightarrow \mathscr{C}_c(Y; (X\times Y)/S)$ such that $j\circ p=\widetilde{q}\circ i$ is therefore continuous. We have $h(\xi , y) =j(\xi )(y)$ for every pair $(\xi , y)\in (X/R)\times Y$. Since Y is locally compact, it then follows from TG, X, p. 28, th. 3, that the mapping $h$ is continuous.

The conclusion of Proposition 10 is no longer necessarily true if Y is not locally compact (TG, I, p. 96, exerc. 6).

#### Corollary {#ta-i-s1-n10-cor-1 .statement tag=01M9}

Let X and Y be topological spaces and let $f: X\rightarrow$ Y be a continuous mapping. Let T be a locally compact topological space. If the mapping $f$ is strict, the same is true of the mapping $f\times$ Id$_T$ of $X\times T$ into $Y\times T$.

### 11. Universally strict mappings

Let

${X'}^{f'}$ X

$p'p$

${B'}^f$ B

be a cartesian square, where the mapping $p$ is strict. The mapping $p'$ is not necessarily strict (cf. TG, I, p. 96, exerc. 6). However, if A is an open or closed subspace of B, the mapping $p_A:\overset{-1}{p}(A)\rightarrow A$ is strict (TG, I, p. 23, cor. 1).

#### Definition 6 {#ta-i-s1-def-6 .statement tag=01MA}

Let $p: X\rightarrow B$ be a continuous mapping. One says that the mapping $p$ is universally strict if for every cartesian square

${X'}^{f'}$ X

$p'p$

${B'}^f$ B

the mapping $p'$ is strict.

A universally strict mapping is strict. With the notations of Definition 6, if the mapping $p$ is universally strict, the same is true of $p'$. This results immediately from def. 6 and prop. 7 of I, p. 15.

#### Corollary {#ta-i-s1-n11-cor-1 .statement tag=01MB}

A continuous mapping which is open, or proper, or which admits in a neighbourhood of every point a continuous section, is universally strict (prop. 8 and example 2).

#### Example {#ta-i-s1-n11-exa-1 .statement tag=01MC}

Let B be a topological space and let $(A_i)_{i\in I}$ be a covering of B; let A denote the sum space of the family $(A_i)_{i\in I}$, and let $p: A\rightarrow B$ be the canonical mapping. The mapping $p$ is universally strict under each of the following two assumptions:

(i) For every point $b\in B$, there exists $i\in I$ such that $b$ is an interior point of $A_i$;

(ii) The family $(A_i)$ is locally finite and the $A_i$ are closed subsets of B.

Under assumption (i), the mapping $p$ possesses in a neighbourhood of every point a continuous section. Under assumption (ii), the mapping $p$ is proper by definition of the sum space (resp. from TG, I, p. 6, prop. 4 and TG, I, p. 75, th. 1). It is therefore universally strict.

#### Remark {#ta-i-s1-n11-rem-1 .statement tag=01MD}

A closed mapping is not necessarily universally strict (cf. TG, I, p. 96, exerc. 6).

#### Proposition 11 {#ta-i-s1-prop-11 .statement tag=01ME}

Let

${X'}^{f'}$ X

$p'p$

${B'}^f$ B

a cartesian square.

a) Suppose the mapping $f$ strict and surjective. Then, if the mapping $p'$ is open ( resp. closed, resp. proper), the same is true of $p$.

b) Suppose that the mapping $f$ is closed and surjective. Then, if the mapping $p'$ is strict, the same is true of $p$.

c) Suppose that the mapping $f$ is universally strict and surjective. Then, if the mapping $p'$ is strict, the same is true of $p$.

Let us first remark that for every subset A of X, one has

$$
p'((\overset{-1}{f}')(A)) =\overset{-1}{f}(p(A)) \tag{20}
$$

In fact, if $x'\in (\overset{-1}{f}')(A)$, then $f(p'(x')) =p\circ f'(x')\in p(A)$. Conversely, if $b'\in \overset{-1}{f}(p(A))$, let $x\in A$ be such that $f(b') =p(x)$. By definition of a cartesian square, there exists a unique $x'\in X'$ such that $f'(x') =x$ and $p'(x') =b'$, so that $b'\in p'((\overset{-1}{f}')(A))$.

Let us prove a). Suppose first that $p'$ is an open (resp. closed) mapping and let A be an open (resp. closed) set in X. The set $(\overset{-1}{f}')(A)$ is open (resp. closed) in $X'$. Hence the set $p'((\overset{-1}{f}')(A))$ is open (resp. closed) in $B'$. By relation (20), it is also saturated with respect to the equivalence relation defined by $f$. Since the mapping $f$ is supposed surjective, one then has $p(A) =$

$f(p'((\overset{-1}{f}')(A)))$, and since it is strict, the set $p(A)$ is open (resp. closed) in B. The mapping $p$ is therefore open (resp. closed).

In order that a continuous mapping be proper, it is necessary and sufficient that it be closed and that its fibres be quasi-compact (TG, I, p. 75, th. 1). If the mapping $p'$ is proper, the mapping $p$ is closed by what precedes. Let us study its fibres: if $b\in B$, let $b'\in B'$ be such that $f(b') =b$. By the corollary of I, p. 10, the mapping $f'$ induces a homeomorphism $X'_{b'}\rightarrow X_b$. Since $p'$ is proper, $X'_{b'}$ is quasi-compact, hence $X_b$ is so also. The mapping $p$ is therefore proper.

Let us prove b) and c). Let Y = $p(X)$ and $Y'=p'(X')$ ; relation (20) applied to X implies that $Y'=\overset{-1}{f}(Y)$. Let $g$ denote the mapping of $Y'$ into Y induced by $f$. In case b), the mapping $g$ is strict by remark 1, I, p. 18. In case c), it is strict by virtue of definition 6 since the square

$Y'$ Y

$B'$ B

is cartesian.

Let $q$ and $q'$ denote the mappings of X into Y and of $X'$ into $Y'$ induced by $p$ and $p'$, so that the square

${X'}^{f'}$ X

$q'q$

${Y'}^g$ Y

is cartesian. Since the mappings $g$ and $q'$ are both strict and surjective, their composite $g\circ q'$ is strict. Hence $q\circ f'$ is strict and $p\circ f'$ is itself strict. Since $f$ is surjective, $f'$ is so also and $p$ is strict by prop. 9, b) of I, p. 18.

#### Corollary 1 {#ta-i-s1-prop-11-cor-1 .statement tag=01MF}

Suppose that the mapping $f$ is universally strict and surjective and that the mapping $p'$ is universally strict. Then the mapping $p$ is universally strict.

Let

Y $^{g'}$ X

$qp$

C $^g$ B

be a cartesian square; it is a question of proving that the mapping $q$ is strict. By remark 3 of I, p. 16, the squares

$$
X'\times_XY^{pr_1}X'
$$

$rp'$

$$
B'\times_BC^{pr_1}B'
$$

and

$X'\times_XY^{pr_2}$ Y

$$
rq \tag{21}
$$

$B'\times_BC^{pr_2}$ C

are cartesian, where $r: X'\times_XY\rightarrow B'\times_BC$ denotes the mapping induced by $(p', q)$. Since the mapping $f$ is universally strict and surjective, the same is true of the mapping pr$_2: B'\times_BC\rightarrow C$ (I, p. 20, def. 6 and I, p. 10, cor. of prop. 4). On the other hand, the mapping $r$ is strict, since $p'$ is assumed universally strict. By prop. 11, c) applied to the cartesian square (21), the mapping $q$ is strict.

#### Corollary 2 {#ta-i-s1-prop-11-cor-2 .statement tag=01MG}

Let B and X be topological spaces and let $p: X\rightarrow B$ be a continuous mapping. Let $(A_i)_{i\in I}$ be a family of subsets of B which is an open covering of B, or else a locally finite closed covering of B. If for every $i\in$ I, the mapping $p_{A_i}:\overset{-1}{p}(A_i)\rightarrow A_i$ is strict ( resp. universally strict), the mapping $p$ is strict ( resp. universally strict).

For every $i\in I$, put $Y_i=\overset{-1}{p}(A_i)$ and $p_i=p_{A_i}$. Let A be the sum space of the family $(A_i)_{i\in I}$, Y the sum space of the family $(Y_i)_{i\in I}$; let us denote by $f: A\rightarrow B$ (resp. $g: Y\rightarrow X,q: Y\rightarrow A$) the mapping deduced from the family of canonical injections $A_i\rightarrow B$ (resp. from the canonical injections $Y_i\rightarrow X$, from the mappings $p_i$). The square

Y $^g$ X

$qp$

A $^f$ B

is a cartesian square (examples, I, p. 10 and p. 14). By the corollary, I, p. 20, the mapping $f$ is universally strict. By proposition 11, it is therefore enough to prove that the mapping $q$ is strict (resp. universally strict) if the mappings $p_i$, for $i\in I$, are so. We are thus reduced to proving the corollary when the sets $A_i$, $i\in I$, constitute a partition of the space B into open and closed subsets, which we shall henceforth suppose.

Suppose that each of the mappings $p_i,i\in I$, is strict. If U is an open subset of X and saturated for the equivalence relation defined by $p$, the set $p_i(X_i\cap U)$ is open in $A_i$ and $p(U) =$ $\bigcup_{i\in I}p_i(X_i\cap U)$ is open in B. The mapping $p$ is therefore strict.

Suppose now that each of the mappings $p_i,i\in I$, is universally strict, and now prove that the mapping $p$ is universally strict. Let C be a topological space and $h: C\rightarrow B$ a continuous mapping. It is a question of proving that the mapping pr$_1: X\times_BC\rightarrow C$ is strict. The space C is identified with the sum space of the family of the $C_i=\overset{-1}{h}(A_i)$ and the space $X\times_BC$ is identified with the sum space of the family of the $X\times_BC_i= X_i\times_{A_i}C_i$. Since $p_i$ is universally strict, the mapping pr$_1: X_i\times_{A_i}C_i\rightarrow C_i$ is strict. By what precedes, the mapping pr$_1: X\times_BC\rightarrow C$ is strict. This proves that the mapping $p$ is universally strict.

## EXERCISES {#ta-i-s1-exercises}

See the [exercises for § 1](exercises/s1/).
