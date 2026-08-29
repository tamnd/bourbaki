---
book: ta
book_title: Topologie algébrique
chapter: I
chapter_title: REVÊTEMENTS
section: 5
section_title: Revêtements principaux
lang: en
source: ta-i-iv-fr
book_pages: TA I.91-TA I.119, TA I.147-TA I.149
pdf_pages: 0107-0135, 0163-0165
extraction: native
subsections:
    - "no": 1
      title: Espaces fibrés principaux
      page: 91
      pdf_page: 107
    - "no": 2
      title: Revêtements principaux
      page: 97
      pdf_page: 113
    - "no": 3
      title: Opérations propres et libres de groupes discrets
      page: 99
      pdf_page: 115
    - "no": 4
      title: Revêtements galoisiens
      page: 101
      pdf_page: 117
    - "no": 5
      title: Espaces fibrés associés
      page: 104
      pdf_page: 120
    - "no": 6
      title: Revêtements associés
      page: 108
      pdf_page: 124
    - "no": 7
      title: Espaces fibrés principaux définis par des cocycles
      page: 114
      pdf_page: 130
statements: 58
exercises: 4
content_sha256: b2aa9fda240c14a456e34d8b7b5d0b17468650d8303a0134aea07d1f327022fd
translated_from: content/fr/ta/I/05_s5_revetements_principaux.md
source_lang: fr
translation_method: machine
source_content_sha256: 9e0b3a2880661b1773a660710a4f7e83d91b83a46e2464d3bcc6276f1a0f64a2
translation_model: gpt-5.4
translation_run: translate-en-mt-ccfd4e75
glossary_version: 34
glossary_terms_sha256: 9e5805c1780ce639f7482c316bee4d24f69319ea5cf3ab7e15ebe75a5f51edb6
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 5. PRINCIPAL FIBRE SPACES

### 1. Principal fibre spaces

#### Definition 1 {#ta-i-s5-def-1 .statement tag=01Q5}

Let G be a topological group and B a topological space. A (right) principal fibre space with base B and group G is a B-space $(E, p)$ endowed with a right operation of G on E (A, I, p. 50) having the following property:

(FP) For every point $b$ of B, there exists a neighbourhood U of $b$ and a

U-isomorphism $f: U\times G\rightarrow \overset{-1}{p}(U)$ such that for all $u\in U$

and $g,g'\in G$, one has $f(u, gg') =f(u, g)\cdot g'$.

Instead of saying that $(E, p)$ is a principal fibre space with base B and group G, one sometimes says that the quadruple $(E,G,B, p)$ is a principal fibration (cf. VAR, R, § 6), or, by abuse, that the mapping $p: E\rightarrow B$ is a principal fibration with base B and group G.

When no doubt is possible as to the base B, the group G and the operation of G on E, we shall simply say that $(E, p)$ is a principal fibre space.

Let G be a topological group. Let $(E, p)$ be a B-space endowed with a left operation of G. If, for the right operation of the group $G^{\circ}$ opposite to the given operation (A, I, p. 50), $(E, p)$ is a right principal fibre space with group $G^{\circ}$, one says that $(E, p)$ is a left principal fibre space with group G.

A principal fibre space is a locally trivial fibre space (I, p. 68, def. 1).

It follows from property (FP) that the group G acts continuously (TG, III, p. 9) and freely on E, and that the orbits of this operation are the fibres of the B-space $(E, p)$. The mapping $p': E/G\rightarrow B$ deduced from $p$ is continuous and bijective. Again from property (FP), the mapping $p$ is open (TG, I, p. 30, prop. 2 and p. 26, prop. 5); hence $p'$ is a homeomorphism (TG, I, p. 32, prop. 3).

Let $(E, p)$ and $(E', p')$ be principal fibre spaces with base B and group G. A mapping $f: E\rightarrow E'$ is said to be a morphism of principal fibre spaces (with base B and group G) if $f$ is a B-morphism and if one has $f(x\cdot g) =f(x)\cdot g$ for every $x\in E$ and every $g\in G$. Let $(E'', p'')$ be a principal fibre space with base B and group G. If $f: E\rightarrow E'$ and $g: E'\rightarrow E''$ are morphisms of principal fibre spaces, the mapping $g\circ f: E\rightarrow E''$ is a morphism of principal fibre spaces. In accordance with the general definitions (E, IV, p. 11), one may take as morphisms of the structure of principal fibre space with base B and group G those defined above. We denote by $\mathscr{C}_B^G(E; E')$ the set of morphisms of principal fibre spaces from $(E, p)$ into $(E', p')$.

A trivial principal fibre space with base B and group G is the B-space $(B\times G$, pr$_1)$ endowed with the law of right operation of G on $B\times G$ defined by $(b, g)\cdot h= (b, gh)$.

A principal fibre space $(E, p)$ with base B and group G is said to be trivializable if there exists an isomorphism of $(E, p)$ onto the trivial principal fibre space $(B\times G$, pr$_1)$; such an isomorphism is called a trivialization of the principal fibre space $(E, p)$. Property (FP) expresses that there exists an open covering $(U_i)_{i\in I}$ of B such that, for every $i\in I$, the $U_i$-space $(\overset{-1}{p}(U_i), p|U_i)$, endowed with the right operation of G deduced from that of G on E, is a trivializable principal fibre space.

#### Example 1 {#ta-i-s5-n1-exa-1 .statement tag=01Q6}

Let $(E, p)$ be a principal fibre space with base B and group G, and let A be a subspace of B. The subspace $E_A=\overset{-1}{p}(A)$ of E is stable under the operation of G, and the mapping $p_A: E_A\rightarrow A$ makes it into a principal fibre space with base A and group G. One says that $(E_A, p_A)$ is the principal fibre space induced by $(E, p)$ over A.

#### Example 2 {#ta-i-s5-n1-exa-2 .statement tag=01Q7}

Let $(E, p)$ be a principal fibre space with base B and group G; let $(E', p')$ be a principal fibre space with base $B'$ and group $G'$. We define a law of operation on the right of the group $G\times G'$ on the space $E\times E'$ by putting $(x, x')\cdot (g, g') = (x\cdot g, x'\cdot g')$ for $x\in E,x'\in E',g\in G$ and $g'\in G'$; this operation is continuous. Let U be an open subset of B and $f: U\times G\rightarrow \overset{-1}{p}(U)$ a trivialization of the U-space $(\overset{-1}{p}(U), p_U)$;

let $U'$ be an open subset of $B'$ and $f': U'\times G'\rightarrow (^-{p'}^1)(U')$ a trivialization of the $U'$-space ($(^-{p'}^1)(U'), p'_U$). The mapping $((b, b'),(g, g'))\mapsto$ $(f(b, g), f'(b', g'))$ is a $(U\times U')$-isomorphism $f''$ of $(U\times U')\times (G\times G')$

onto $\overset{-1}{p}(U)\times (^-{p'}^1)(U')$ and one has

$$
f''((b, b'),(gh, g'h')) = (f(b, gh), f'(b', g'h')) =f''((b, b'),(g, g'))\cdot (h, h')
$$

It follows that the $(B\times B')$-space $E\times E'$, endowed with the law of operation of $G\times G'$ defined above, is a principal fibre space, called the product of the principal fibre spaces E and $E'$.

#### Example 3 {#ta-i-s5-n1-exa-3 .statement tag=01Q8}

In particular, when $B = B'$, the B-space $E\times_BE'$ is identified with the principal fibre space with group $G\times G'$ induced by $E\times E'$ over the diagonal $\Delta_B$ of $B\times B$. Endowed with this structure of principal fibre space, the B-space $E\times_BE'$ is called the fibre product of the principal fibre spaces E and $E'$.

#### Example 4 {#ta-i-s5-n1-exa-4 .statement tag=01Q9}

Let E be a principal fibre space with base B and group G and let F be a topological space. The $(B\times F)$-space $E\times F$ endowed with the law of operation $(x, y)\cdot g= (x\cdot g, y)$, for $x\in E,y\in F$ and $g\in G$, is a principal fibre space with group G. This is the particular case of Example 2, where $p'$ is the identity mapping of F and $G'$ is a group reduced to the identity element.

#### Example 5 {#ta-i-s5-n1-exa-5 .statement tag=01QA}

Let B be a topological space and $(E, p)$ a principal fibre space with base B and group G. Let $B'$ be a topological space and $f: B'\rightarrow B$ a continuous mapping. The group G operates on the right in the fibre product $B'\times_BE$ by the law $(b', x)\cdot g= (b', x\cdot g)$, for $b'\in B',x\in E$ and $g\in G$. This operation is continuous and free; the orbits are the fibres of the mapping pr$_1: B'\times_BE\rightarrow B'$. It follows from Examples 1 and 4 above and Remark 2 of I, p. 16 that the $B'$-space $B'\times_BE$ is a principal fibre space with group G. It is called the principal fibre space deduced from $(E, p)$ by the base change $f$, or again the inverse image of $(E, p)$ by $f$.

#### Proposition 1 {#ta-i-s5-prop-1 .statement tag=01QB}

Every morphism of principal fibre spaces is an isomorphism.

Let $f: B\times G\rightarrow B\times G$ be a morphism of the trivial principal fibre space $(B\times G$, pr$_1)$ into itself and let $\varphi : B\times G\rightarrow G$ be the continuous mapping pr$_2\circ f$, so that $f(b, g) = (b, \varphi (b, g))$. For every $b\in B$ and all $g,h\in G$, one has $\varphi (b, gh) =\varphi (b, g)\cdot h$, whence $\varphi (b, g) =\varphi (b, e)\cdot g$, where $e$ denotes the identity element of G. The morphism $f$ is therefore an isomorphism whose inverse morphism $f^{-1}$ is defined by $f^{-1}(b, g) =$ $(b, \varphi (b, e)^{-1}g)$ for $(b, g)\in B\times G$.

Now let E and $E'$ be principal fibre spaces and let $f: E\rightarrow E'$ be a morphism of principal fibre spaces. In view of property (FP), for every point $b\in B$, there exists an open neighbourhood U of $b$ such that the principal fibre spaces $E_U$ and $E'_U$ are trivializable. By passing to subspaces, $f$ induces a morphism $f_U: E_U\rightarrow E'_U$ of principal fibre spaces; by what precedes, this morphism $f_U$ is an isomorphism. In particular, $f_b: E_b\rightarrow E'_b$ is a bijection. There then exists a unique mapping $g: E'\rightarrow E$ which induces the bijection $f_b^{-1}$ by passing to subspaces. By Proposition 4 of I, p. 19, the mapping $g$ is continuous, hence $f$ is an isomorphism of principal fibre spaces.

#### Corollary {#ta-i-s5-n1-cor-1 .statement tag=01QC}

Let G be a topological group, $(E, p)$ and $(E', p')$ principal fibre spaces of group G and with bases B and $B'$ respectively. Let $f: B'\rightarrow$ B and $f': E'\rightarrow$ E be continuous mappings such that $p\circ f'=f\circ p'$ and such that, for every $x'\in E'$ and every $g\in G$, $f'(x'\cdot g) =f'(x')\cdot g$. Then the square

${E'}^{f'}$ E

$p'p$

${B'}^f$ B

is a cartesian square.

In fact, the mapping $h: E'\rightarrow B'\times_BE$ defined by $h(x') =$ $(p'(x'), f'(x'))$ for $x'\in E'$, is a $B'$-morphism of principal coverings, hence an isomorphism; moreover pr$_2\circ h=f'$, whence the result (I, p. 8, Prop. 2).

Under the hypotheses of the preceding corollary, one sometimes says that $f'$ is an $f$-morphism of principal fibre spaces.

#### Proposition 2 {#ta-i-s5-prop-2 .statement tag=01QD}

Let $(E, p)$ be a principal fibre space with base B and group G, and let $\varepsilon$ be the section $b\mapsto (b, e)$ of the trivial principal fibre space $(B\times G$, pr$_1)$, where $e$ denotes the identity element of G. The mapping $h\mapsto h\circ \varepsilon$ is a bijection of $\mathscr{C}_B^G(B\times G; E)$ onto the set $\mathscr{S}(B; E)$ of continuous sections of $p$. The inverse bijection associates to a continuous section $s$ of $p$ the B-morphism $(b, g)\mapsto s(b)\cdot g$.

#### Corollary {#ta-i-s5-n1-cor-2 .statement tag=01QE}

A principal fibre space is trivializable if and only if it admits a continuous section.

#### Proposition 3 {#ta-i-s5-prop-3 .statement tag=01QF}

Let E and B be topological spaces, $p: E\rightarrow B$ a continuous mapping and G a topological group operating on the right on E. The following conditions are equivalent:

(i) Endowed with the mapping $p$, E is a principal fibre space with base B and group G;

(ii) For every $x\in E$ and every $g\in G$, one has $p(x\cdot g) =p(x)$, the mapping $\theta : (x, g)\mapsto (x, x\cdot g)$ is a homeomorphism of $E\times G$ onto $E\times_BE$ and every point of B possesses a neighbourhood over which there exists a continuous section of the mapping $p$.

(i)$\Rightarrow$(ii) : Suppose that $(E, p)$ is a principal fibre space. The group G operates continuously and freely in E, with the fibres of $p$ as orbits. Hence the mapping $\theta$ is bijective and continuous. More precisely, if $E\times_BE$ is endowed with the operation of G defined by $(x, y)\cdot g= (x, y\cdot g)$, the mapping $\theta$ is an E-morphism of the trivial principal fibre space $E\times G$ into the principal fibre space $(E\times_BE\rightarrow E$, pr$_1)$ (example 5), hence an isomorphism (prop. 1). The other assertions of (ii) result immediately from the definition.

(ii)$\Rightarrow$(i) : Put $\varphi =$ pr$_2\circ \theta^{-1}$, so that, for every $(x, y)\in$ $E\times_BE$, one has

$$
\theta^{-1}(x, y) = (x, \varphi (x, y)) \tag{1}
$$

The mapping $\varphi : E\times_BE\rightarrow G$ is continuous and, for $(x, y)\in E\times_BE$, the element $\varphi (x, y)$ is the unique element $g$ of G such that $y=x\cdot g$. Let $b$ be a point of B; let U be a neighbourhood of $b$ and let $s$ be a continuous section of $p$ over U. For $(u, g)\in U\times G$, put $f(u, g) =s(u)\cdot$ $g$; the mapping $f$ is a U-morphism of $U\times G$ into $\overset{-1}{p}(U)$. For $y\in \overset{-1}{p}(U)$, put $f'(y) = (p(y), \varphi (s(p(y)), y))$. The mapping $f'$ is a U-morphism of $\overset{-1}{p}(U)$ into $U\times G$. One has

$$
(f\circ f')(y) =s(p(y))\cdot \varphi (s(p(y)), y) =y
$$

On the other hand, for $(u, g)\in U\times G$, one has

$$
(f'\circ f)(u, g) =f'(s(u)\cdot g) = (u, \varphi (s(u), s(u)\cdot g)) = (u, g)
$$

Hence $f$ is a U-isomorphism. It follows that $(E, p)$ is a principal fibre space with base B and group G.

#### Remark 1 {#ta-i-s5-n1-rem-1 .statement tag=01QG}

Let $(E, p)$ be a principal fibre space with base B and group G. With the notation of proposition 3, the mapping $\theta^{-1}: E\times_BE\rightarrow E\times G$ is a trivialisation of the principal fibre space pr$_1: E\times_BE\rightarrow E$. One says that $\theta^{-1}$ is the canonical trivialisation of this principal fibre space.

#### Corollary 1 {#ta-i-s5-prop-3-cor-1 .statement tag=01QH}

Let G be a topological group operating continuously on the right in a topological space E. The following conditions are equivalent:

(i) The orbit space $E/G$ is Hausdorff and the space E, endowed with the canonical mapping $p: E\rightarrow E/G$, is a principal fibre space with group G;

(ii) The group G operates properly (TG, III, p. 27) and freely in E, and every point of $E/G$ possesses a neighbourhood over which there exists a continuous section of the mapping $p$.

Put $B = E/G$. Under each of the hypotheses (i) and (ii), the group G operates continuously and freely in E, so that the mapping $\theta : (x, g)\mapsto (x, x\cdot g)$ is a continuous bijection of $E\times G$ onto $E\times_BE$. Let us place ourselves under this hypothesis and denote by $\varphi : E\times_BE\rightarrow G$ the mapping pr$_2\circ \theta^{-1}$. Having regard to formula (1), in order that $\theta$ be a homeomorphism, it is necessary and sufficient that the mapping $\varphi$ be continuous. On the other hand, since the equivalence relation defined by G is open (TG, III, p. 10, lemma 2), in order that the space $E/G$ be Hausdorff, it is necessary and sufficient that the graph $E\times_BE$ of this equivalence relation be closed in $E\times E$ (TG, I, p. 55, prop. 8). Finally (TG, III, p. 31, prop. 6), in order that G operate properly in E, it is necessary and sufficient that $E\times_BE$ be closed in $E\times E$ and that the mapping $\varphi$ be continuous. The equivalence of conditions (i) and (ii) then follows from prop. 3.

#### Corollary 2 {#ta-i-s5-prop-3-cor-2 .statement tag=01QI}

Let G be a topological group, let H be a subgroup of G, and let $p: G\rightarrow G/H$ be the canonical mapping. If the mapping $p$ possesses a continuous section over a nonempty open set of $G/H$, the mapping $p$ makes G into a principal fibre space with base $G/H$ and group H.

By left translations, every point of $G/H$ possesses a neighbourhood over which the mapping $p$ possesses a continuous section. On the other hand, for $(g, g')$ belonging to $G\times G$, put $\varphi (g, g') =$ $g^{-1}g'$. If $p(g) =p(g'),\varphi (g, g')$ belongs to H. The mapping $(g, g')\mapsto$ $(g, \varphi (g, g'))$ of $G\times_{G/H}G$ into $G\times H$ is continuous and is the inverse of the continuous mapping $\theta : G\times H\rightarrow G\times_{G/H}G$ defined by $\theta (g, h) = (g, gh)$, whence the corollary.

#### Remark 2 {#ta-i-s5-n1-rem-2 .statement tag=01QJ}

This situation presents itself in particular when G is a real Lie group, of finite dimension, countable at infinity, operating transitively and analytically on an analytic manifold X. If one takes for H the stabiliser of a point of X, the mapping $p$ is a submersion of G onto the homogeneous Lie space $G/H$, isomorphic to X (LIE, III, p. 109, corollary). It therefore possesses local sections (VAR, p. 50).

### 2. Principal Coverings

#### Definition 2 {#ta-i-s5-def-2 .statement tag=01QK}

Let B be a topological space and let G be a group. Endow G with the discrete topology. A principal fibre space with base B and group G is called a principal covering of B with group G.

This terminology is legitimate, for such a B-space is a covering of B.

A principal covering with group G of a nonempty topological space possesses a degree, equal to Card G.

#### Proposition 4 {#ta-i-s5-prop-4 .statement tag=01QL}

Let B be a topological space, $(E, p)$ a B-space, and G a discrete topological group operating on the right on E. The following assertions are equivalent:

(i) The B-space E is a principal covering with group G;

(ii) For every $g\in G$ and every $x\in E$, one has $p(x\cdot g) =p(x)$, the mapping $p$ induces a homeomorphism of $E/G$ onto B, and the mapping $\theta : (x, g)\mapsto (x, x\cdot g)$ is a homeomorphism of $E\times G$ onto $E\times_BE$;

(iii) The group G operates continuously and freely in E, the mapping $p$ is etale, and its fibres are the orbits of G.

(i)$\Rightarrow$(ii) : This follows from I, p. 91 and from proposition 3 of I, p. 94.

(ii)$\Rightarrow$(iii): Under assumption (ii), the action law of G is continuous, and the mapping $p$ is surjective and open (TG, III, p. 10, lemma 2). Let $x\in E$; the mapping $\theta$ induces a bijection of $\{x\} \times G$ onto $\{x\} \times$ $\overset{-1}{p}(p(x))$, hence the group G operates freely and its orbits are the fibres of $p$. If $e$ denotes the identity element of G, the diagonal of $E\times_BE$ is the image of $E\times  \{e\}$ under the homeomorphism $\theta$. Since the group G is discrete, the set $\{e\}$ is open in G, therefore the diagonal $\Delta_E$ is open in $E\times_BE$. By proposition 7 of I, p. 31, the mapping $p$ is étale.

(iii)$\Rightarrow$(i): Every fibre of $p$ being an orbit of the operation of G in E, the mapping $p$ is surjective. Since the mapping $p$ is étale, for every point $b$ of B, there exists an open neighbourhood U of $b$ and a continuous section $s$ of $p$ over U. The set $s(U)$ is open in E and $s$ induces a homeomorphism of U onto $s(U)$ (I, p. 30, cor. 3). For every $g\in G$, the set $s(U)\cdot g$ is open in E and the union of the sets $s(U)\cdot g$, for all $g\in G$, is equal to $\overset{-1}{p}(U)$. If $g$ and $g'$ are two distinct elements of G, the sets $s(U)\cdot g$ and $s(U)\cdot g'$ are disjoint, since G operates freely in E. The mapping $f: U\times G\rightarrow$ $\overset{-1}{p}(U)$ defined by $f(u, g) =s(u)\cdot g$ for $(u, g)\in U\times G$ is therefore a homeomorphism of $U\times G$ onto $\overset{-1}{p}(U)$, compatible with the right operations of G. By definition, E is therefore a principal covering of B with group G.

#### Example 1 {#ta-i-s5-n2-exa-1 .statement tag=01QM}

Let E be a topological space, G a discrete topological group operating continuously and freely in E on the right. In order that the canonical mapping $p: E\rightarrow E/G$ make E a principal covering of $E/G$, it is necessary and sufficient that it be étale (condition (iii) of proposition 4). For example, suppose there exists a topological space X and an étale mapping $q: E\rightarrow X$ compatible with the operation of G in E; then E is a principal covering of $E/G$. In fact, let us denote by $q': E/G\rightarrow X$ the mapping deduced from $q$; one has $q=q'\circ p$, therefore $p$ is étale by proposition 6, d) of I, p. 29.

#### Example 2 {#ta-i-s5-n2-exa-2 .statement tag=01QN}

Let $q: E\rightarrow$ X be an étale and separated mapping. The group Aut$_X(E)$, endowed with the discrete topology, operates continuously on the left in E. If the space E is connected, this operation is free (I, p. 34, corollary 2). Let us denote by G the group Aut$_X(E)^{\circ}$ and endow E with the right operation opposite to that of Aut$_X(E)$. By the preceding example, the space E, endowed with the canonical mapping $p: E\rightarrow E/G$, is a principal covering with group G.

### 3. Proper and free operations of discrete groups

#### Theorem 1 {#ta-i-s5-thm-1 .statement tag=01QO}

Let G be a discrete group operating continuously on the right in a topological space E. Suppose that every point of E possesses a neighbourhood U such that $U\cap (U\cdot g) =\emptyset$ for every element $g$ of G other than the identity element. Then the canonical mapping $p: E\rightarrow E/G$ makes E a principal covering of $E/G$ with group G.

The operation of G in E is free by assumption, so it is enough to prove that the mapping $p$ is étale (I, p. 98, example 1). Let $x$ be a point of E and let U be an open neighbourhood of $x$ such that $U\cap U\cdot g=\emptyset$ for every element $g$ of G distinct from the identity element. The mapping $p$ is open (TG, III, p. 10, lemma 2) and induces an injective, continuous and open mapping of U onto $p(U)$, hence a homeomorphism, which proves that the mapping $p$ is étale.

#### Example 1 {#ta-i-s5-n3-exa-1 .statement tag=01QP}

Let $n$ be an integer $\geqslant 0$, let $\mathbf{P}_n(\mathbf{R})$ be the projective space of dimension $n$ (TG, VI, p. 13) and let $\mathbf{S}_n$ be the unit sphere of $\mathbf{R}^{n+1}$ (TG, VI, p. 9). The canonical mapping of $\mathbf{S}_n$ onto $\mathbf{P}_n(\mathbf{R})$ makes $\mathbf{S}_n$ into a principal covering of group $\{1,-1\}$, this group operating by homotheties; the orbits are the pairs of diametrically opposite points.

#### Example 2 {#ta-i-s5-n3-exa-2 .statement tag=01QQ}

Every covering of degree 2 possesses a unique structure of principal covering of group $\mathbf{Z}/2\mathbf{Z}$.

#### Example 3 {#ta-i-s5-n3-exa-3 .statement tag=01QR}

Let X be a separated differentiable manifold locally of finite dimension over $\mathbf{R}$, and let $\widetilde{X}$ be the manifold of orientations of the tangent bundle of X (VAR, R, 10.2.4). The space $\widetilde{X}$, endowed with its canonical projection onto X, is a principal covering of X of group $\{1,-1\}$.

#### Corollary 1 {#ta-i-s5-thm-1-cor-1 .statement tag=01QS}

Let G be a discrete topological group operating continuously on the right in a topological space E. The following conditions are equivalent:

(i) The group G operates properly and freely in E;

(ii) The space $E/G$ is separated and the space E is a principal covering with base $E/G$ and group G.

Moreover, under these conditions, the space E is separated.

Suppose condition (i) satisfied. Then the spaces E and $E/G$ are separated (TG, III, p. 29, prop. 3) and for every $x\in E$ there exists an open neighbourhood U of $x$ in E such that $U\cap (U\cdot g) =\emptyset$ for every element $g$ of G other than the identity element (TG, III, p. 32, prop. 8). By Theorem 1, condition (ii) is then satisfied.

The implication (ii)$\Rightarrow$(i) follows from corollary 1 of I, p. 96.

#### Corollary 2 {#ta-i-s5-thm-1-cor-2 .statement tag=01QT}

Let G be a topological group and let H be a discrete subgroup of G. Let H operate on G by right translations. Then the canonical mapping of G into the space $G/H$ of left classes modulo H endows G with a structure of principal covering of $G/H$ of group H.

Let V be a neighbourhood of the identity element $e$ of G such that $H\cap V =\{e\}$. There exists an open neighbourhood U of $e$ in G such that $U^{-1}\cdot U\subset V$ (TG, III, p. 3) and consequently $U\cap U\cdot h=\emptyset$ for every $h\in H,h=\not e$. Corollary 2 of I, p. 100 therefore follows from theorem 1.

#### Example 4 {#ta-i-s5-n3-exa-4 .statement tag=01QU}

Endowed with the canonical mapping of $\mathbf{R}$ onto $\mathbf{T}=\mathbf{R}/\mathbf{Z}$ (TG, V, p. $2$)$,\mathbf{R}$ is a principal covering of $\mathbf{R}/\mathbf{Z}$ of group $\mathbf{Z}$.

#### Remark 1 {#ta-i-s5-n3-rem-1 .statement tag=01QV}

Let G be a separated topological group, K a compact subgroup of G and H a discrete subgroup of G. The group G operates continuously and properly on the right in the space $K\backslash G$ of right classes modulo K (TG, III, p. 30, corollary). Since the group H is closed in G, it also operates properly in $K\backslash G$ (TG, III, p. 27, example 1). If, moreover, one has $H\cap gKg^{-1}=\{e\}$ for every $g\in G$, the group H operates freely in $K\backslash G$. The space $K\backslash G$ is then a principal covering of group H of $K\backslash G/H$ by corollary 1.

#### Corollary 3 {#ta-i-s5-thm-1-cor-3 .statement tag=01QW}

Let G and $G'$ be topological groups, and let $\varphi : G\rightarrow G'$ be a continuous, open and surjective homomorphism. Suppose that the kernel H of $\varphi$ is discrete. Then, for the operation of H in G by right translations, $\varphi$ makes G into a principal covering of $G'$ of group H.

If moreover the group G is connected, H is contained in the center of G.

The homomorphism $\varphi$ induces a topological group isomorphism of $G/H$ onto $G'$ (TG, III, p. 16, prop. 24), whence the first assertion by Corollary 2. Suppose the group G connected. For every $h\in H$, the continuous mapping of G into H defined by $g\mapsto ghg^{-1}$ is constant, with value $h$. The group H is therefore contained in the center of G.

#### Remark 2 {#ta-i-s5-n3-rem-2 .statement tag=01QX}

Let G and $G'$ be topological groups and let $\varphi : G\rightarrow G'$ be a continuous open homomorphism. If the group $G'$ is connected, the homomorphism $\varphi$ is surjective. In fact, $\varphi (G)$ is an open, therefore closed, subgroup of $G'$, and consequently equal to $G'$.

#### Remark 3 {#ta-i-s5-n3-rem-3 .statement tag=01QY}

Let G be a locally compact group countable at infinity and let $G'$ be a separated topological group whose underlying space is a Baire space. Every continuous surjective homomorphism of G into $G'$ is open (TG, IX, p. 56, corollary and TG, III, p. 16, prop. 24).

#### Example 5 {#ta-i-s5-n3-exa-5 .statement tag=01QZ}

For every integer $n >$ 0, let us denote by $\mu_n$ the group of $n$th roots of unity in $\mathbf{C}$ (A, V, p. 75). The mapping $z\mapsto z^n$ makes $\mathbf{C}^*$ into a principal covering of $\mathbf{C}^*$ with group $\mu_n$, this group operating in $\mathbf{C}^*$ by multiplication.

#### Example 6 {#ta-i-s5-n3-exa-6 .statement tag=01R0}

Endowed with the mapping $z\mapsto e^{2\pi iz}$ (TG, VIII, p. 8, remark), the space $\mathbf{C}$ is a principal covering of $\mathbf{C}^*$ with group $\mathbf{Z}$. The mapping $x\mapsto e^{2\pi ix}=\mathbf{e}(x)$ of $\mathbf{R}$ onto $\mathbf{S}_1$ makes $\mathbf{R}$ into a principal covering of $\mathbf{S}_1$ with group $\mathbf{Z}$.

### 4. Galois Coverings

#### Definition 3 {#ta-i-s5-def-3 .statement tag=01R1}

Let B be a nonempty topological space. A covering E of B is said to be Galois if it is connected and if, for every point $b$ of B, the operation of the group Aut$_B(E)$ of B-automorphisms of E on the fibre $E_b$ is transitive.

Let E be a Galois covering of a topological space B and let $p$ be its projection. The mapping $p$ is surjective (A, I, p. 56, def. 6); therefore the space B is connected. Consequently, the covering $(E, p)$ has a nonzero degree.

#### Proposition 5 {#ta-i-s5-prop-5 .statement tag=01R2}

Let B be a nonempty topological space and let E be a Galois covering of B. The mapping $(h, x)\mapsto h(x)$ of Aut$_B(E)\times E$ into E is a right operation law of the group Aut$_B(E)^{\circ}$ on E which makes E into a principal covering with group Aut$_B(E)^{\circ}$.

Let us endow the group Aut$_B(E)^{\circ}$ with the discrete topology; the operation law $(h, x)\mapsto h(x)$ is then continuous. This operation is free (I, p. 34, Corollary 2 of Proposition 11). Since E is a Galois covering of B, its fibres are the orbits of this operation. By Proposition 4 of I, p. 97, E is a principal covering with group Aut$_B(E)^{\circ}$.

#### Theorem 2 {#ta-i-s5-thm-2 .statement tag=01R3}

Let B be a connected topological space, let E be a covering of B, connected and nonempty. The following properties are equivalent:

(i) The covering E is Galois;

(ii) There exists a discrete topological group G and a continuous right operation of G on E making E into a principal covering with group G;

(iii) The covering $E\times_BE$ of E defined by the projection pr$_1$ is trivializable.

When these conditions are satisfied, the canonical mapping $G\rightarrow$ Aut$_B(E)^{\circ}$ defined by the operation of G is a group isomorphism.

If, moreover, the space B is locally connected, the preceding properties are equivalent to the following property:

(i$'$) There exists a point $b$ of B such that the operation of the group Aut$_B(E)$ on the fibre $E_b$ is transitive.

The implication (i)$\Rightarrow$(ii) results from proposition 5 and the implication (ii)$\Rightarrow$(iii) from remark 1 of I, p. 95. Let us prove (iii)$\Rightarrow$(i). Let us denote by $p: E\rightarrow B$ the projection of the covering E. Since B is connected, this covering has a degree, and this degree is not zero since E is not empty. Let $b$ be a point of B. Let us prove that the operation of Aut$_B(E)$ on the fibre $E_b$ is transitive. From the above, this fibre is not empty. Let $x$ and $x'$ be points of $E_b$. The B-morphisms $h: E\rightarrow E$ such that $h(x) =x'$ correspond bijectively to the continuous sections $s$ of the mapping pr$_1: E\times_BE\rightarrow E$ such that $s(x) = (x, x')$ (I, p. 9, prop. 3). Under assumption (iii), such a section exists (I, p. 70, cor. 2) and is unique (I, p. 34, cor. 1 of prop. 11) since the space E is connected. Thus, for every pair $(x, x')\in E\times_BE$, there exists a unique B-morphism $h: E\rightarrow E$ such that $h(x) =x'$. If $h': E\rightarrow E$ is the unique B-morphism such that $h'(x') =x$, one has $h'(h(x)) =x$ and $h(h'(x')) =x'$, whence $h'\circ h=$ Id$_E$ and $h\circ h'=$ Id$_{E'}$. This proves that $h$ is a B-automorphism of E. Hence the covering E is galoisian.

We have proved that conditions (i), (ii), (iii) are equivalent. Suppose them satisfied. Let $\delta : G\rightarrow$ Aut$_B(E)$ be the mapping which to $g\in G$ associates the B-automorphism $x\mapsto x\cdot g$ of E. The mapping $\delta$ is a group homomorphism of G into Aut$_B(E)^{\circ}$. Since G operates freely in E, the mapping $\delta$ is injective. Let $h\in$ Aut$_B(E)$, let $x\in$ E and let $g$ be the unique element of G such that $x\cdot g=h(x)$. The B-morphisms $h$ and $\delta (g)$ coincide at $x$, hence everywhere, since the space E is connected (I, p. 34, cor. 1 of prop. 11), which proves that $\delta$ is an isomorphism.

Now suppose the space B locally connected and let us prove, under assumption (i$'$), that the covering E is galoisian. Let $E'$ be the quotient space of E by the right operation of Aut$_B(E)^{\circ}$ and let us denote by $q: E\rightarrow E'$ the canonical mapping. It makes E into a surjective covering of $E'($I, p. 98, example 2); the mapping $p: E\rightarrow B$ defines by passing to the quotient a continuous mapping $p': E'\rightarrow B$ such that $p'\circ q=p$. Since the space B is locally connected, the B-space $(E', p')$ is a covering (I, p. 81, prop. 7). Under assumption (i$'$), there exists a point $b$ of B such that the fibre $E'_b$ has exactly one element; since the space B is connected, the same is then true for every point $b$ of B (I, p. 74, prop. 4), which proves that E is a galoisian covering of B.

#### Proposition 6 {#ta-i-s5-prop-6 .statement tag=01R4}

Let B be a topological space and G a group. Let $(E, p)$ be a principal covering of B with group G. Suppose the space B connected and locally connected. Let $E_0$ be a connected component of E and let $G_0$ be the stabilizer subgroup of G of $E_0$ (A, I, p. 51). The B-space $(E_0, p|E_0)$ is a principal covering for the right operation of $G_0$ in $E_0$. This covering is Galois.

Since the space B is locally connected, the same is true of E, so that $E_0$ is an open subspace of E (TG, I, p. 85, prop. 11). Since it is also closed (TG, I, p. 83), the space $E_0$ is therefore a covering of B (I, p. 80, cor. 1). Since B is connected, this covering has a degree; since $E_0$ is not empty, all the fibres of $p|E_0$ are therefore non-empty. Let $x$ be a point of $E_0$, let $x'\in E_0$ be such that $p(x') =p(x)$; there exists an element $g\in G$ such that $x\cdot g=x'$. Since the connected components $E_0$ and $E_0\cdot g$ then have a common point, they are equal, whence $g\in G_0$. Thus, the group $G_0$ operates transitively in the fibre of the B-space $E_0$ at $p(x)$. Proposition 6 follows.

#### Remark {#ta-i-s5-n4-rem-1 .statement tag=01R5}

If, in proposition 6, one does not suppose the space B locally connected, it may happen that the space $E_0$ is not a covering of B (I, p. 147, exerc. 1).

### 5. Associated fibre spaces

Let E and F be sets and let G be a group operating on the right on E and on the left on F. The group G operates on the right on the product $E\times F$ by the law $(x, y)\cdot g= (x\cdot g, g^{-1}\cdot y)$, for $g\in G$, $(x, y)\in E\times F$. The quotient set of $E\times F$ by this operation is denoted by $E\times^GF$.

When E and F are topological spaces, the set $E\times^GF$ is endowed with the quotient topology of that of $E\times F$. The canonical mapping of $E\times F$ onto $E\times^GF$ is continuous. If the group G operates continuously in E and F, it is open.

Moreover, let $F'$ be a set on which G operates on the left and let $h: F\rightarrow F'$ be a mapping compatible with the operations of G on F and $F'$ (A, I, p. 50). The mapping Id$_E\times h: E\times F\rightarrow E\times F'$ is compatible with the operations of G and defines by passing to the quotients a mapping denoted by Id$_E\times^Gh$ of $E\times^GF$ into $E\times^GF'$.

If $h: F\rightarrow F'$ is a continuous mapping (compatible with the operations of G on F and $F'$), the mapping Id$_E\times^Gh$ is continuous (TG, I, p. 21, prop. 6).

#### Example 1 {#ta-i-s5-n5-exa-1 .statement tag=01R6}

Let F be a topological space and let G be a topological group operating continuously on the left in F. If the topological space G is endowed with the operation of G by right translations, the space $G\times^GF$ is canonically identified with F in the following way. The continuous mappings $\varphi : F\rightarrow G\times F$ and $\psi : G\times F\rightarrow$ F defined by $\varphi (f) = (e, f)$ (where $e$ denotes the identity element of G) and $\psi (g, f) =g\cdot f$ induce continuous mappings $\overline{\varphi}: F\rightarrow G\times^GF$ and $\overline{\psi}: G\times^GF\rightarrow F$ which are reciprocal to one another.

#### Example 2 {#ta-i-s5-n5-exa-2 .statement tag=01R7}

Example 1 is generalized as follows. Let B and F be topological spaces and let G be a topological group operating continuously on the left in F. By passing to the quotients, the mapping of $B\times F$ into $(B\times G)\times F$ given by $(b, f)\mapsto ((b, e), f)$ and the mapping of $(B\times G)\times F$ into $B\times F$ given by $((b, g), f)\mapsto (b, gf)$ define reciprocal B-isomorphisms $B\times F\rightarrow (B\times G)\times^GF$ and $(B\times G)\times^GF\rightarrow B\times F$.

#### Example 3 {#ta-i-s5-n5-exa-3 .statement tag=01R8}

Analogously, let E be a topological space and let G be a topological group operating continuously on the right in E. If the topological space G is endowed with the operation of G by left translations, the space $E\times^GG$ is identified with E.

Let E and F be topological spaces and let G be a topological group operating continuously on the right in E and on the left in F. Let B be a topological space and let $p: E\rightarrow B$ be a continuous mapping such that $p(x\cdot g) =p(x)$ for $x\in E$ and $g\in G$. The mapping $p\circ$ pr$_1: E\times F\rightarrow B$ defines, by passing to the quotient, a continuous mapping $p^F: E\times^GF\rightarrow B$ and the canonical mapping $\pi : E\times F\rightarrow E\times^GF$ is a B-morphism.

Let $B'$ be a topological space and let $h: B'\rightarrow B$ be a continuous mapping. The group G operates continuously on the right in $B'\times_BE$ by the operation law $((b', x), g)\mapsto (b', x\cdot g)$. By composing the canonical isomorphism $((b', x), y)\mapsto (b',(x, y))$ of $(B'\times_BE)\times F$ onto $B'\times_B(E\times F)$ and the mapping Id$_{B'}\times \pi$ of $B'\times_B(E\times F)$ into $B'\times_B(E\times^GF)$, one obtains a continuous mapping $\lambda_0: (B'\times_BE)\times F\rightarrow B'\times_B(E\times^GF)$. It defines, by passing to the quotient, a continuous mapping

$$
\lambda : (B'\times_BE)\times^GF\rightarrow B'\times_B(E\times^GF)
$$

#### Lemma {#ta-i-s5-n5-lem-1 .statement tag=01R9}

The mapping $\lambda$ is a homeomorphism.

The mapping $\lambda_0$ is surjective and two elements of $(B'\times_BE)\times F$ have the same image under $\lambda_0$ if and only if they belong to the same orbit for the operation of G in $(B'\times_BE)\times F$. It follows that the mapping $\lambda$ is bijective. Since the mapping $\pi$ is open, the same is true of the mapping Id$_{B'}\times_B\pi ($I, p. 17, prop. 8), hence of $\lambda_0$ and of $\lambda$ (TG, I, p. 32, prop. 3), which proves that $\lambda$ is a homeomorphism.

#### Proposition 7 {#ta-i-s5-prop-7 .statement tag=01RA}

Let B be a topological space, let G be a topological group, let $(E, p)$ be a principal fibred space over B with group G and let F be a topological space in which the group G operates continuously on the left.

a) The topological space $E\times^GF$ endowed with the continuous mapping $p^F: E\times^GF\rightarrow B$ deduced from the mapping $p\circ$pr$_1: E\times F\rightarrow B$ by passing to the quotient is a locally trivial fibred space over B of fibre type F; it is trivializable if the fibred space over B E is trivializable.

b) Let $\pi : E\times F\rightarrow E\times^GF$ be the canonical surjection. The mapping $\mu: E\times F\rightarrow E\times_B(E\times^GF)$ which associates to $(x, f)$ the element $(x, \pi (x, f))$ is a homeomorphism whose inverse mapping is a trivialization of the locally trivial fibred space over E $(E\times_B(E\times^GF)$, pr$_1)$.

Suppose first that E is the trivial principal fibred space over B $B\times G$. By example 2, the space $E\times^GF$ is then identified with $B\times F$ and the mapping $p^F$ with the first projection pr$_1: B\times F\rightarrow B$, which proves that $(E\times^GF, p^F)$ is a trivializable fibred space over B in this case. In the general case, every point of B possesses a neighbourhood U such that the mapping $p_U:\overset{-1}{p}(U)\rightarrow U$ makes $\overset{-1}{p}(U)$ into a trivializable principal fibred space over U. From what precedes, $(\overset{-1}{p}(U)\times^GF\rightarrow U,(p_U)^F)$ is a trivializable fibred space over U. By the above lemma, applied to the case where $B'= U$ and $h: U\rightarrow B$ is the canonical injection, the same is

true of the fibred space over U ($(p^{-F1})(U),(p^F)_U$) deduced from $(E\times^GF, p^F)$ by restriction above U. This proves that $(E\times^GF, p^F)$ is a locally trivial fibred space over B and concludes the proof of assertion a).

The mapping $\theta : E\times G\rightarrow E\times_BE$ defined by $\theta (x, g) = (x, x\cdot g)$ is a homeomorphism (I, p. 94, prop. 3) compatible with the operations of G on $E\times G$ and on $E\times_BE$ given by $((x, g), g')\mapsto (x, gg')$ and $((x, y), g')\mapsto (x, yg')$ respectively. By passing to quotients, $\theta$ therefore induces a homeomorphism $\theta '$ of $(E\times G)\times^GF$ onto $(E\times_B$ $E)\times^GF$. The mapping $\mu$ is the composite of the homeomorphism $E\times F\rightarrow$ $(E\times G)\times^GF$ (example 2), of $\theta '$, and of the canonical homeomorphism $(E\times_BE)\times^GF\rightarrow E\times_B(E\times^GF)$ (I, p. 105, lemma), whence b).

Under the hypotheses of proposition 7, the locally trivial fibred B-space ($E\times^GF, p^F$) is called the locally trivial fibred space of fibre type F associated with the principal fibred space $(E, p)$. All the fibres of the B-space $E\times^GF$ are homeomorphic to the space F. In particular, if the space F is discrete, the mapping $p^F$ is a covering.

#### Example 4 {#ta-i-s5-n5-exa-4 .statement tag=01RB}

Let B be a topological space, G a topological group, and let $(E, p)$ be a principal fibred B-space with group G. Let H be a subgroup of G.

Let us denote by $\varphi : E\rightarrow E\times (G/H)$ and $\psi : E\times (G/H)\rightarrow E/H$ the mappings defined by $\varphi (x) = (x,H)$ and $\psi (x, gH) = (x\cdot g)H$. They are compatible with the projections onto B and with the operations of G and define, by passing to quotients, morphisms of B-spaces $\overline{\varphi}: E/H\rightarrow E\times^G(G/H)$ and $\overline{\psi}: E\times^G(G/H)\rightarrow E/H$, inverse to one another. One says that $\overline{\varphi}$ is the canonical homeomorphism of $E/H$ onto $E\times^G(G/H)$. In particular, the topological space $E/H$ endowed with the continuous mapping $p_H: E/H\rightarrow B$ is a locally trivial fibred B-space of fibre type $G/H$.

If, moreover, H is a normal subgroup of G, the action of G endows the B-space $E/H$, by passing to quotients, with a structure of principal fibred space with group $G/H$.

In particular, if E is a principal covering of B with group G, $E/H$ is a covering of B; if H is normal in G, it is a principal covering with group $G/H$.

#### Example 5 {#ta-i-s5-n5-exa-5 .statement tag=01RC}

Let B be a topological space, let G be a topological group, and let E be a principal fibred B-space with group G. Let F be a topological homogeneous space relative to G (TG, III, p. 12). Let $y$ be a point of F and let $G_y$ be its stabiliser. The mapping $\varphi_y:x\mapsto (x, y)$ of E into $E\times F$ defines, by passing to quotients, a homeomorphism $\overline{\varphi}_y$ of $E/G_y$ onto $E\times^GF$. When the group G is abelian, the subgroup $G_y$ does not depend on the point $y$, but the homeomorphism $\overline{\varphi}_y$, in general, does depend on it.

#### Example 6 {#ta-i-s5-n5-exa-6 .statement tag=01RD}

Let B be a topological space, let G be a topological group, let $(E, p)$ be a principal fibred B-space with group G. Let H be a topological group and let $f: G\rightarrow H$ be a morphism of topological groups; let us endow H with the left operation of G given by $g\cdot h=f(g)h$.

Let $q: E\times H\rightarrow E\times^GH$ be the canonical mapping; it is open, hence universally strict (I, p. 20, corollary 11). The mapping $m: (x, h, h')\mapsto q(x, hh')$ of $E\times H\times H$ into $E\times^GH$ is continuous. Let $(x, h)\in E\times H,h'\in H$ and $g\in G$; we have $m(xg, f(g)^{-1}h, h') =$ $q(xg, f(g)^{-1}hh') =q(x, hh') =m(x, h, h')$. Consequently, there exists a unique mapping

$$
m': (E\times^GH)\times H\rightarrow E\times^GH
$$

such that $m'(q(x, h), h') =q(x, h, h')$ for all $x\in E$ and all $h, h'\in H$. Since $q$ is universally strict, the mapping $m'$ is continuous. This is a right operation of the topological group H on the B-space $E\times^GH$.

Let U be an open subset of B such that $E_U$ is isomorphic to the principal fibre bundle over U, $U\times G$. Endowed with the operation of H, the U-space $(E\times^GH)_U$ is identified with the principal fibre bundle $U\times H$. This proves that $E\times^GH$ is a principal fibre bundle over B with group H.

#### Definition 4 {#ta-i-s5-def-4 .statement tag=01RE}

Let B be a topological space and let G be a topological group. A locally trivial fibre space X over B is said to be associated with a principal fibre bundle E over B with group G if there exists a topological space F on which the group G operates continuously on the left and a B-isomorphism of $E\times^GF$ onto X.

Let E be a principal fibre bundle over B with group G and let X be a locally trivial fibre space over B associated with E. If the principal fibre bundle E is trivializable, X is trivializable (Prop. 7). If $B'$ is a topological space and $h: B'\rightarrow B$ a continuous mapping, the locally trivial fibre space over $B'$, $B'\times_BX$, deduced from X by base change is associated with the principal fibre bundle over $B'$, $B'\times_BE$ (I, p. 105, lemma).

### 6. Associated Coverings

Let B be a topological space, let G be a discrete topological group and let E be a principal covering of B with group G. Let F be a G-set; if F is endowed with the discrete topology, the group G acts continuously on F. The B-space $E\times^GF$ is then a covering. It is called the covering of B with fibre type F associated with the principal covering E.

#### Definition 5 {#ta-i-s5-def-5 .statement tag=01RF}

Let B be a topological space, let G be a discrete topological group and let E be a principal covering of B with group G. A covering X of B is said to be associated with the principal covering E if there exists a G-set F and a B-isomorphism of $E\times^GF$ onto X.

Let B be a topological space, let G be a discrete topological group and let E be a covering of B, principal with group G.

For every covering X of B, the group G operates on the left on $\mathscr{C}_B(E; X)$ by the law defined by $(g\cdot h)(x) =h(x\cdot g)$ for $x\in E$, $g\in G,h\in \mathscr{C}_B(E; X)$.

For every G-set F endowed with the discrete topology, let us define a mapping $\alpha_F: F\rightarrow \mathscr{C}_B(E; E\times^GF)$ by:

(2) $\alpha_F(y)(x) =\pi (x, y)$ for $y\in F$ and $x\in E$,

where $\pi : E\times F\rightarrow E\times^GF$ is the canonical surjection. The mapping $\alpha_F$ is compatible with the operations of G on F and on $\mathscr{C}_B(E; E\times^GF)$.

For every covering X of B, there exists a unique mapping $\beta_X$ from $E\times^G\mathscr{C}_B(E; X)$ into X such that:

(3) $\beta_X(\pi (x, h)) =h(x)$ for $h\in \mathscr{C}_B(E; X)$ and $x\in E$.

In fact, one has $(g^{-1}\cdot h)(x\cdot g) =h(x)$ for $x\in E,g\in G$ and $h\in \mathscr{C}_B(E; X)$, by definition of the operation of G on $\mathscr{C}_B(E; X)$. When the set $\mathscr{C}_B(E; X)$ is endowed with the discrete topology, the mapping $\beta_X$ is a B-morphism of coverings.

When $X = E\times^GF$, one has

(4) $\beta_X(\pi (x, \alpha_F(y))) =\pi (x, y)$ for $x\in X$ and $y\in F$.

#### Proposition 8 {#ta-i-s5-prop-8 .statement tag=01RG}

Let B be a connected nonempty topological space. Let G be a discrete group and let $(E, p)$ be a principal covering of B with group G. Suppose that E is connected. With the above notation, one has:

a) For every G-set F endowed with the discrete topology, the mapping $\alpha_F$ is an isomorphism of the G-set F onto the G-set $\mathscr{C}_B(E; E\times^GF)$.

b) Let X be a covering of B. The B-morphism $\beta_X$ is an isomorphism of $E\times^G\mathscr{C}_B(E; X)$ onto X if and only if the covering $(E\times_BX$, pr$_1)$ of E is trivializable.

a) Let $y$ and $y'$ be points of F such that $\alpha_F(y) =\alpha_F(y')$. The space E is not empty; let us choose a point $x$ in it. We have $\pi (x, y) =\pi (x, y')$ in $E\times^GF$. Hence there exists $g\in G$ such that $x\cdot g=x$ and $g^{-1}\cdot y=y'$. The first equality implies that $g$ is the identity element $e$ of G, hence $y=y'$. Thus the mapping $\alpha_F$ is injective. On the other hand, let $h\in$ $\mathscr{C}_B(E; E\times^GF)$ and let $x$ be a point of E. Let $x'\in E,y'\in F$ be such that $h(x) =\pi (x', y')$. In particular, $p(x) =p(x')$; there then exists an element $g$ of G such that $x'=x\cdot g$, and we also have $h(x) =\pi (x, y)$, where we have set $y=g\cdot y'$. The B-morphisms $h$ and $\alpha_F(y)$ coincide at the point $x$ of E; they are therefore equal since the space E is connected (I, p. 34, cor. 1 of prop. 11), and this proves that the mapping $\alpha_F$ is surjective.

b) By proposition 7, b) of I, p. 105 applied to $F =\mathscr{C}_B(E; X)$, the covering $p^*(E\times^G\mathscr{C}_B(E; X))$ of E is isomorphic to the trivial covering $E\times \mathscr{C}_B(E; X)$. If $\beta_X$ is an isomorphism, the covering $p^*(X)$ of E is therefore trivializable. Conversely, suppose that the covering $p^*(X)$ is trivializable and let us prove that the B-morphism $\beta_X$ is bijective; it will follow that $\beta_X$ is a B-isomorphism (I, p. 30, cor. 2 of prop. 6).

The mapping $\beta_X$ is deduced by passing to the quotient from the mapping $\gamma : E\times \mathscr{C}_B(E; X)\rightarrow X$ defined by $\gamma (x, h) =h(x)$. Let us prove that the mapping $\gamma$ is surjective. Let $x$ be a point of X. The projection of the B-space E is surjective, for it is a principal covering; there therefore exists a point $y$ of E such that $(y, x)\in E\times_BX$. There then exists a continuous section $s$ of the trivializable covering pr$_1: E\times_BX\rightarrow E$ such that $s(y) = (y, x)$. The mapping $h=$ pr$_2\circ s: E\rightarrow X$ is a B-morphism, and we have $h(y) =x$, whence the surjectivity of the mapping $\gamma$ and, consequently, that of the mapping $\beta_X$.

Let us prove finally that $\beta_X$ is injective. Let $(x, h)$ and $(x', h')$ be elements of $E\times \mathscr{C}_B(E; X)$ such that $h(x) =h'(x')$. Observe that $x$ and $x'$ have the same projection in B; there therefore exists an element $g$ of G such that $x'=x\cdot g$. We then have $h(x) =h'(x\cdot g) = (g\cdot h')(x)$. Since the space E is connected, we have $h=g\cdot h'($I, p. 34, cor. 1 of prop. 11). Thus, $(x, h)$ and $(x', h')$ have the same class in $E\times^G\mathscr{C}_B(E; X)$, which proves that the mapping $\beta_X$ is injective, and completes the proof.

#### Corollary 1 {#ta-i-s5-prop-8-cor-1 .statement tag=01RH}

Let $(E, p)$ be a principal covering of B of group G; suppose that E is connected and nonempty. A covering X of B is associable to E if and only if the covering $p^*(X)$ is trivializable.

If the covering $p^*(X)$ is trivializable, it follows from proposition 8, b), that the covering X is associable to E. In this case, the mapping $\beta_X$ identifies the covering X with the covering of fibre-type $\mathscr{C}_B(E; X)$ associated to E. Conversely, let F be a G-set endowed with the discrete topology and suppose that one has $X = E\times^GF$. Then $\alpha_F$ is an isomorphism (loc. cit., a)) and formula (4) implies that $\beta_X$ is an isomorphism. Consequently, the covering $p^*(X)$ is trivializable (prop. 8, b)), whence the corollary.

#### Corollary 2 {#ta-i-s5-prop-8-cor-2 .statement tag=01RI}

Let B be a connected and locally connected topological space, let $(E, p)$ be a principal covering of B of group G. Let $E_0$ be a connected component of E and let $G_0$ be the subgroup of G stabilizer of $E_0$. The B-space $(E_0, p|E_0)$ is a principal covering of group $G_0($I, p. 103, prop. 6).

Every covering X of B which is associable to the principal covering E is associable to the principal covering $E_0$. In particular, the covering E is associable to the principal covering $E_0$.

Indeed, if the covering X is associable to E, the covering $p^*(X)$ is trivializable and the covering $p^*_0(X)$ induced by $p^*(X)$ above $E_0$ is therefore trivializable.

More precisely, note that the mapping $(x, g)\mapsto x\cdot g$ of $E_0\times G$ into E induces, by passing to the quotient, a B-isomorphism of principal coverings of $E_0\times^{G_0}G$ onto E.

#### Proposition 9 {#ta-i-s5-prop-9 .statement tag=01RJ}

Let B be a topological space, let E be a principal covering of B of group G, connected and nonempty. Let F be a nonempty G-set endowed with the discrete topology. In order that the space $E\times^GF$ be connected, it is necessary and sufficient that G operate transitively in F.

Let U be a subset open and closed of $E\times^GF$. If $\pi : E\times F\rightarrow$ $E\times^GF$ denotes the canonical surjection, $\overset{-1}{\pi}(U)$ is a subset open and closed of $E\times F$ which is stable under G. Since E is connected, there exists a subset $F'\subset F$, stable under G, such that $\overset{-1}{\pi}(U) = E\times F'$, whence $U =\pi (E\times F')$. Let $F'$ and $F''$ be subsets of F stable under G such that $\pi (E\times F') =\pi (E\times F'')$; since E is not empty, one has $F'= F''$. The mapping $F'\mapsto \pi (E\times F')$ is a bijection of the set of subsets of F stable under G onto the set of subsets open and closed of $E\times^GF$. The proposition follows.

#### Proposition 10 {#ta-i-s5-prop-10 .statement tag=01RK}

Let B be a topological space, let $(E, p)$ be a principal covering of B of group G and let X be a covering of B. Suppose that E and X are connected and nonempty. The following properties are equivalent:

(i) The covering X is associable to the principal covering E;

(ii) There exists a subgroup H of G such that X is B-isomorphic to $E/H$;

(iii) There exists a surjective B-morphism $h: E\rightarrow X$;

(iv) For every point $(y, x)$ of $E\times_BX$, there exists a B-morphism $r: E\rightarrow X$ such that $r(y) =x$.

Suppose these conditions satisfied and let H be a subgroup of G such that X is B-isomorphic to $E/H$. The covering X is Galois if and only if the subgroup H is normal in G.

(i)$\Rightarrow$(ii) : Let F be a discrete G-set such that the covering $E\times^GF$ is B-isomorphic to X. The set F is nonempty and the space $E\times^GF$ is connected, hence the group G operates transitively in F (proposition 9). Then the space $E\times^GF$ is B-isomorphic to $E/H$, where H is the subgroup of G fixing a point of F (I, p. 106, example 4).

(ii)$\Rightarrow$(iii) : In fact, the canonical surjection of E onto $E/H$ is a surjective B-morphism.

(iii)$\Rightarrow$(iv) : Let $(y, x)$ be a point of $E\times_BX$. Since the mapping $h$ is surjective, there exists a point $y'$ of E such that $h(y') =x$. The points $y$ and $y'$ have the same projection in B. Since the covering E is principal with group G, there exists $g\in G$ such that $y\cdot g=y'$. The mapping $r: E\rightarrow X$ defined by $z\mapsto h(z\cdot g)$ is a B-morphism and one has $r(y) =x$.

(iv)$\Rightarrow$(i) : Since X is not empty and the projection of E onto B is surjective, the space $E\times_BX$ is not empty. Hence there exists a B-morphism $r$ of E into X. The mapping (Id$_E, r$)$: E\rightarrow E\times_BX$ is a section of the covering $p^*(X)$ of E. Since the space E is connected, it follows from Corollary 2 of proposition 1 of I, p. 69 that the covering $p^*(X)$ is trivializable, which proves that the covering X is associable to the Galois covering $p$ (proposition 8).

Suppose now that these conditions are satisfied. We denote by X the B-space $E/H$, by $q$ its projection, and by $h: E\rightarrow E/H$ the canonical mapping.

If the group H is normal in G, then X is a principal covering with group $G/H$ (I, p. 106, example 4). Since X and B are connected and nonempty, X is a Galois covering of B (I, p. 102, theorem 2). Conversely, suppose that $E/H$ is a Galois covering of B and let K = Aut$_B(E/H)^{\circ}$. One defines a mapping $\alpha : E\times G\rightarrow K$ by associating to $(t, g)\in E\times G$ the unique element $k$ of K such that $h(t\cdot g) =h(t)\cdot k$. It is continuous because it is obtained by composing the continuous mapping $(t, g)\mapsto (h(t), h(t\cdot g))$ of $E\times G$ into $X\times_BX$ with the canonical trivialization (I, p. 95, remark 1) $X\times_BX\rightarrow X\times K$ of $q^*(X)$. Since E is connected and K is a discrete group, the continuous mapping $t\mapsto \alpha (t, g)$ is constant, for every $g\in G$; we denote by $\alpha (g)$ its value. If $t\in E,g\in G$ and $g'\in H$, one then has

$$
h(t) =h(t\cdot g^{-1}g) =h(t\cdot g^{-1})\cdot \alpha (g) =h(t\cdot g^{-1}\cdot g')\cdot \alpha (g) =h(t\cdot (g^{-1}g'g))
$$

It follows that $g^{-1}g'g$ belong to H and hence that H is normal in G.

#### Corollary {#ta-i-s5-n6-cor-1 .statement tag=01RL}

Let E be a Galois covering of B and let X be a covering of B, connected and nonempty. Suppose that X is a finite covering or else that the space B is locally connected. If there exists a B-morphism $h: E\rightarrow X$, the covering X is associable to the principal covering E.

In both cases, the B-morphism $h$ is a covering (I, p. 77, Cor. 3 of theorem 1, and I, p. 78, proposition 5), and a nonempty covering of a connected space is surjective (I, p. 68).

#### Theorem 3 {#ta-i-s5-thm-3 .statement tag=01RM}

Let B be a nonempty, connected and locally connected topological space. Every covering of B is associable to a Galois covering; every finite covering of B is associable to a finite Galois covering.

Let X be a covering of B, and let us denote by $q$ its projection. Since the space B is connected and nonempty, the covering X has a degree; let us denote this degree by F and endow the set F with the discrete topology. Since the space B is locally connected, the sheaf $\mathscr{I}$ = $\mathscr{I}$som$_B(B\times F; X)$ is locally constant and at every point $b$ of B its stalk $\mathscr{I}_b$ is canonically isomorphic to the set $\mathscr{B}(F; X_b)$ of bijections of F onto the fibre $X_b($I, p. 89, prop. 12). Let $E = E_{\mathscr{I}}$ be the covering associated with the locally constant sheaf $\mathscr{I}($I, p. 86, corollary).

Let G be the group of permutations of F. For every $g\in G$, one defines as follows a morphism $\gamma '(g)$ of the sheaf $\mathscr{I}$ into itself: for every open subset U of B, the mapping $\gamma '(g)_U$ associates with a U-isomorphism $\varphi : U\times F\rightarrow \overset{-1}{q}(U)$ the U-isomorphism defined by $(b, f)\mapsto \varphi (b, g(f))$ for $b\in U$ and $f\in F$. One has $\gamma '$(Id$_F$) $=$ Id$_{\mathscr{I}}$ and $\gamma '(g\circ g') =\gamma '(g')\circ \gamma '(g)$, for $g,g'\in G$, so that for every $g\in G,\gamma '(g)$ is an automorphism of the sheaf $\mathscr{I}$. The B-morphism $\gamma (g): E\rightarrow E$ associated with $\gamma '(g)$ is an automorphism (I, p. 50). If $x= [U, \varphi , b]$ is an element of E, where U is an open subset of B$,b$ a point of U and $\varphi$ a U-isomorphism of $U\times F$ onto $\overset{-1}{q}(U)$, one has $\gamma (g)(x) = [U, \psi , b]$, where $\psi$ is defined by $\psi (a, f) =\varphi (a, g(f))$, for $a\in$ U and $f\in$ F. If $g$ and $g'$ are elements of G, one has $\gamma (g\circ g') =\gamma (g')\circ \gamma (g)$. One has $\gamma$(Id$_F$) $=$ Id$_E$. One thus defines a continuous right operation law of G in E by setting $x\cdot g=\gamma (g)(x)$, for $x\in E$ and $g\in G$. The group G operates simply transitively on every fibre of E, so that the covering E endowed with this operation is a principal covering with group G (I, p. 97, prop. 4). Let $h$ be the mapping from $E\times F$ into X defined by $h([U, \varphi , b], f) =\varphi (b, f)$ for every open subset U of B, every point $b$ of U and every U-isomorphism $\varphi$ of $U\times F$ onto $\overset{-1}{q}(U)$. By definition of the topology of E, it is continuous; it is a B-morphism. For every element $g$ of G and every point $(x, f)$ of $E\times F$, one has $h(x, g(f)) =h(x\cdot g, f)$. The mapping $h$ therefore defines, by passing to the quotient, a B-morphism $h': E\times^GF\rightarrow X$. For every point $b$ of B, the mapping $h_b: E_b\times F\rightarrow X_b$ identifies with the mapping $(\varphi , f)\mapsto \varphi (f)$ from $\mathscr{B}(F; X_b)\times F$ into $X_b$, so that the mapping $h'_b$ is bijective. Consequently, $h'$ is a B-isomorphism of $E\times^GF$ onto X (I, p. 30, cor. 2 of prop. 6).

As the space B is connected, locally connected and nonempty, the covering X, associated with the principal covering E, is associated with a Galois covering (I, p. 110, corollary 2). If the covering X is finite, the same is true of the covering E, hence X is associated with a finite Galois covering (loc. cit.).

### 7. Principal Fibre Spaces Defined by Cocycles

#### Definition 6 {#ta-i-s5-def-6 .statement tag=01RN}

Let B be a topological space, let G be a topological group, and let $\mathscr{U}= (U_i)_{i\in I}$ be an open covering of B. A continuous 1-cocycle on B with values in G, subordinate to $\mathscr{U}$, is by definition the data, for each pair $(i, j)$ of elements of I, of a continuous mapping $g_{i,j}$ of $U_i\cap U_j$ into G, such that for every triplet $(i, j, k)\in I\times I\times I$ and every point $b$ of $U_i\cap U_j\cap U_k$, one has

$$
g_{i,k}(b) =g_{i,j}(b)g_{j,k}(b)
$$

We denote by $Z^1_{cont}(B,\mathscr{U},G)$ the set of continuous 1-cocycles on B with values in G, subordinate to the covering $\mathscr{U}$.

In this section, we shall simply say cocycle instead of continuous 1-cocycle.

Let $(E, p)$ be a principal fibre space over B of group G, and let $\mathscr{U}$ = $(U_i)_{i\in I}$ be a covering of B by open sets $U_i$. One says that E is trivializable over $\mathscr{U}$ if, for every $i\in I$, E is trivializable over $U_i$. One then calls a $\mathscr{U}$ -trivialization of E a family $(f_i)_{i\in I}$, where $f_i:\overset{-1}{p}(U_i)\rightarrow U_i\times G$ is a trivialization of E over $U_i$.

Let $\mathscr{U}= (U_i)_{i\in I}$ be a covering of B by open sets, and let $(E, p)$ be a principal fibre space over B of group G endowed with a $\mathscr{U}$ -trivialization $(f_i)_{i\in I}$. For every pair $(i, j)\in I\times I$, let us denote by $g_{ij}$ the mapping of $U_i\cap U_j$ into G defined by

$$
(b, g_{ij}(b)) =f_i\circ f_j^{-1}(b, e)
$$

where $e$ denotes the identity element of G. It is continuous.

Since $f_i$ and $f_j$ are compatible with the operations of G, one has

$$
(f_i\circ f_j^{-1})(b, g) = (b, g_{ij}(b)g)
$$

for $b\in U_i\cap U_j$ and $g\in G$. If $b$ is a point of $U_i\cap U_j\cap U_k$ (where $i,j$, $k\in I$), one has

$$
(f_i\circ f_k^{-1})(b, e) = (b, g_{ik}(b))
$$

and

$$
(f_i\circ f_k^{-1})(b, e) = (f_i\circ f_j^{-1})\circ (f_j\circ f_k^{-1})(b, e)
$$

$$
= (f_i\circ f_j^{-1})(b, g_{jk}(b)) = (b, g_{ij}(b)g_{jk}(b))
$$

It follows that

$$
g_{ik}(b) =g_{ij}(b)g_{jk}(b)
$$

so that the family $(g_{ij})$ is a cocycle on B with values in G, subordinate to the covering $\mathscr{U}$. It is called the cocycle defined by the family of trivializations $(f_i)_{i\in I}$.

Let B, G and $\mathscr{U}$ be as in definition 6, and let $(g_{ij})\in$ $Z^1_{cont}(B,\mathscr{U},G)$ be a cocycle. For every pair $(i, j)\in I\times I$, the mapping $\gamma_{ij}: (U_i\cap U_j)\times G\rightarrow (U_i\cap U_j)\times G$ defined by

(5) $\gamma_{ij}(b, g) = (b, g_{ij}(b)g)$ for $b\in U_i\cap U_j$ and $g\in G$

is an isomorphism of principal fibre spaces with base $U_i\cap U_j$. For every triplet $(i, j, k)\in I\times I\times I$ and every pair $(b, g)\in (U_i\cap U_j\cap U_k)\times G$, one has :

$$
\gamma_{ik}(b, g) =\gamma_{ij}\circ \gamma_{jk}(b, g)
$$

Let F be the topological space obtained by gluing the spaces $U_i\times G$ along the $(U_i\cap U_j)\times G$ by means of the bijections $\gamma_{ij}$ (TG, I, p. 16). For each $i\in I$, the image of $U_i\times G$ in F is an open set of F (TG, I, p. 17, Prop. 9). The canonical projections $p_i: U_i\times G\rightarrow U_i$ glue together to give a continuous mapping $p$ of F into B. Since the mappings $\gamma_{ij}$ are compatible with the right operations of G in the spaces $U_i\times G$, one deduces a continuous law of operation of G on the right in F which makes F into a principal fibre space with base B and group G, endowed with a trivialization over each $U_i$. One says that F is the principal fibre space defined by the cocycle $(g_{ij})$.

#### Definition 7 {#ta-i-s5-def-7 .statement tag=01RO}

Let B be a topological space, G a topological group and $\mathscr{U}= (U_i)_{i\in I}$ an open covering of B. Two cocycles $(g_{ij})$ and $(g'_{ij})$ of $Z^1_{cont}(B,\mathscr{U},G)$ are said to be cohomologous if there exists a family $(h_i)_{i\in I}$ of continuous mappings $h_i: U_i\rightarrow G$ such that one has

$$
g'_{ij}(b) =h_i(b)g_{ij}(b)h_j(b)^{-1} \tag{6}
$$

for every pair $(i, j)\in I\times I$ and every $b\in U_i\cap U_j$.

The relation “$(g_{ij})$ is cohomologous to $(g'_{ij})$” is an equivalence relation in the set $Z^1_{cont}(B,\mathscr{U},G)$. We denote by $H^1_{cont}(B,\mathscr{U},G)$ the quotient set of $Z^1_{cont}(B,\mathscr{U},G)$ for this equivalence relation.

#### Proposition 11 {#ta-i-s5-prop-11 .statement tag=01RP}

Let B be a topological space, G a topological group and $\mathscr{U}= (U_i)_{i\in I}$ an open covering of B.

a) Every principal fibre space over B with group G which is trivializable over $\mathscr{U}$ is isomorphic to a principal fibre space defined by a cocycle of $Z^1_{cont}(B,\mathscr{U},G)$.

b) Let $(E, p)$ and $(E', p')$ be principal fibre spaces over B which are trivializable over $\mathscr{U}$. Let $(f_i)_{i\in I}($ resp. $(f'_i)_{i\in I})$ be a trivialization of $(E, p)$ ( resp. of $(E', p')$) adapted to $\mathscr{U}$, and let us denote by $(g_{ij})_{(i,j)\in I\times I}$ ( resp. $(g'_{i,j})_{(i,j)\in I\times I}$) the cocycle defined by this trivialization. Then the principal fibre spaces $(E, p)$ and $(E', p')$ are isomorphic if and only if these cocycles are cohomologous.

Let us prove b). Let $\varphi : E\rightarrow E'$ be an isomorphism of principal fibre spaces with base B and group G. For each $i\in I$, let $h_i$ be the continuous mapping of $U_i$ into G defined by

$$
(b, h_i(b)) =f'_i\circ \varphi \circ f_i^{-1}(b, e)
$$

Since, for each $i\in I,f_i$ and $f'_i$ are compatible with the operations of G, one has for every $b\in U_i$ and every $g\in G$,

$$
(f'_i\circ \varphi \circ f_i^{-1})(b, g) = (b, h_i(b)g)
$$

and

$$
(f_i\circ \varphi^{-1}\circ (f'_i)^{-1})(b, g) = (b, h_i(b)^{-1}g)
$$

Hence, for every pair $(i, j)\in I\times I$ and every point $b$ of $U_i\cap U_j:$ $f'_i\circ (f'_j)^{-1}(b, e) = (f'_i\circ \varphi \circ f_i^{-1})\circ (f_i\circ f_j^{-1})\circ (f_j\circ \varphi^{-1}\circ (f'_j)^{-1})(b, e)$

$$
= (b, h_i(b)g_{ij}(b)h_j(b)^{-1})
$$

so that one has

$$
g'_{ij}(b) =h_i(b)g_{ij}(b)h_j(b)^{-1}
$$

This proves that the cocycles $(g_{ij})$ and $(g'_{ij})$ are cohomologous.

Conversely, suppose that these cocycles are cohomologous, and let $(h_i)_{i\in I}$ be a family of continuous mappings $h_i: U_i\rightarrow G$ such that $g'_{ij}(b) =h_i(b)g_{ij}(b)h_j(b)^{-1}$ for $i,j\in I$ and $b\in U_i\cap U_j$. For

$i\in I$, let $\varphi_i:\overset{-1}{p}(U_i)\rightarrow (^-{p'}^1)(U_i)$ be the mapping defined by $f'_i\circ \varphi_i\circ$ $f_i^{-1}(b, g) = (b, h_i(b)g)$, for $b\in U_i$ and $g\in G$. It is an isomorphism of principal fibre spaces with basis $U_i$ and group G. For $(i, j)\in$ $I\times I$, let us denote by $\gamma_{ij}$ and $\gamma '_{ij}$ the gluing homeomorphisms associated as above with the cocycles $(g_{ij})$ and $(g'_{ij})$ respectively (I, p. 115, formula (5)), so that $f_i(b, g) =\gamma_{ij}\circ f_j(b, g)$ and $f'_i(b, g) =\gamma '_{ij}\circ f'_j(b, g)$ for every $(b, g)\in (U_i\cap U_j)\times G$. Consequently, for $(i, j)\in I\times I$ and $(b, g)\in (U_i\cap U_j)\times G$, we have the relations

$$
f'_i\circ \varphi_j\circ f_i^{-1}(b, g) =\gamma '_{ij}\circ (f'_j\circ \varphi_j\circ f_j^{-1})(b, g_{ij}(b)^{-1}g)
$$

$$
=\gamma '_{ij}(b, h_j(b)g_{ij}(b)^{-1}g)
$$

$$
= (b, g'_{ij}(b)h_j(b)g_{ij}(b)^{-1}g)
$$

$$
= (b, h_i(b)g) =f'_i\circ \varphi_i\circ f_i^{-1}(b, g)
$$

This proves that $\varphi_i$ and $\varphi_j$ coincide on $\overset{-1}{p}(U_i\cap U_j)$. The morphisms $\varphi_i$ therefore glue together to a B-morphism of principal fibre spaces from E to $E'$. Assertion b) follows, since every morphism of principal fibre spaces with basis B and group G is an isomorphism (I, p. 93, Prop. 1).

Let us now prove a). Let $(E, p)$ be a principal fibre space with group G endowed, for each $i\in I$, with a trivialization $f_i:\overset{-1}{p}(U_i)\rightarrow$ $U_i\times G$ over $U_i$. Let $(g_{ij})$ be the cocycle defined by this family, and let F then be the principal fibre space defined by the cocycle $(g_{ij})$. By construction, the principal fibre space F is endowed with a trivialization over $\mathscr{U}$; this trivialization defines the cocycle $(g_{ij})$. By assertion b), the principal fibre space $(E, p)$ is isomorphic to F.

Let B be a topological space and G a topological group. Let $(E, p)$ be a principal fibre space with basis B and group G. Let $s$ be a section of the surjective mapping $p$ (E, II, p. 19, Prop. 8). The mapping $f: B\times G\rightarrow E$ defined by $f(b, g) =s(b)\cdot g$ is a bijection compatible with the action of G. Endow $B\times G$ with the topology obtained by transport of structure; $(B\times G$, pr$_1)$ is then a principal fibre space with basis B and group G isomorphic to E. There therefore exists a set T of principal fibre spaces with basis B and group G such that every principal fibre space with basis B and group G is isomorphic to an element of T. Let us denote by $P(B,G)$ the set of isomorphism classes of principal fibre spaces with basis B and group G (E, II, p. 47).

Let $\mathscr{U}= (U_i)_{i\in I}$ be an open covering of B. Let $P(B,\mathscr{U},G)$ denote the subset of $P(B,G)$ consisting of the isomorphism classes of principal bundles which are trivializable over $\mathscr{U}$. By proposition 11, there exists a mapping $r_{\mathscr{U}}$ of $H^1_{cont}(B,\mathscr{U},G)$ into $P(B,\mathscr{U},G)$ which associates with the class of a cocycle $(g_{ij})\in Z^1_{cont}(B,\mathscr{U},G)$ the isomorphism class of the principal fibre space defined by this cocycle; it is a bijection (loc. cit.). The inverse bijection $s_{\mathscr{U}}$ associates with the isomorphism class in $H^1_{cont}(B,\mathscr{U},G)$ of a principal fibre space E, trivializable over $\mathscr{U}$, the class of the cocycle defined by an arbitrary family of trivializations of E over $\mathscr{U}$. Under this correspondence, the isomorphism class of the trivial principal fibre space $B\times G$ corresponds to the cohomology class of the constant cocycle $g_{ij}=e$, also called the trivial cocycle.

By virtue of the definition of a principal fibre space, the set $P(B,G)$ is the union of the sets of the form $P(B,\mathscr{U},G)$, where $\mathscr{U}$ is an open covering of B.

Let $\mathscr{U}= (U_i)_{i\in I}$ be an open covering of B and let $\mathscr{V}= (V_k)_{k\in K}$ be an open covering of B finer than $\mathscr{U}$. We have $P(B,\mathscr{U},G)\subset$ $P(B,\mathscr{V},G)$; let $i_{\mathscr{V} \mathscr{U}}$ denote the canonical injection defined by this inclusion. Choose a mapping $\varphi : K\rightarrow I$ such that $V_k\subset U_{\varphi(k)}$ for every $k\in K$. Given a cocycle $(g_{ij})\in Z^1_{cont}(B,\mathscr{U},G)$, set, for every pair $(k, \ell )\in K\times K,\overline{g}_{k\ell}=g_{\varphi(k)\varphi(\ell)}|V_k\cap V_{\ell}$.

The family $(\overline{g}_{k\ell})$ is a cocycle on B, with values in G, subordinate to $\mathscr{V}$. If $(g'_{ij})\in Z^1_{cont}(B,\mathscr{U},G)$ is a cocycle cohomologous to the cocycle $(g_{ij})$, the cocycle $(\overline{g}'_{k\ell})$ deduced from $(g'_{k\ell})$ is cohomologous to the cocycle $(\overline{g}_{k\ell})$. It follows that there is a mapping

$$
c(\varphi ): H^1_{cont}(B,\mathscr{U},G)\rightarrow H^1_{cont}(B,\mathscr{V},G)
$$

which associates with the class of $(g_{ij})$ the class of $(\overline{g}_{k\ell})$.

Let E be a principal fibre space with base B and group G and, for every $i\in$ I, let $f_i: E_{U_i}\rightarrow U_i\times G$ be a trivialization of the principal $U_i$-bundle $E_{U_i}$. For every $k\in$ K, let $f'_k: E_{V_k}\rightarrow V_k\times G$ be the trivialization deduced from $f_{\varphi(k)}$ by passing to subsets. Let $(g_{ij})\in Z^1_{cont}(B,\mathscr{U},G)$ be the cocycle defined by the family $(f_i)$; the cocycle defined by the family $(f'_k)$ is precisely the cocycle $(\overline{g}_{k\ell})$ defined above. Thus, the following diagram is commutative:

$$
H^1_{cont}(B,\mathscr{U},G)^{c(\varphi)}H^1_{cont}(B,\mathscr{V},G)
$$

$r_{\mathscr{U}}r_{\mathscr{V}}$

$$
P(B,\mathscr{U},G)^{i_{\mathscr{V} \mathscr{U}}}P(B,\mathscr{V},G)
$$

Since the mappings $r_{\mathscr{U}}$ and $r_{\mathscr{V}}$ are bijective, the mapping $c(\varphi )$, analogously to $i_{\mathscr{V} \mathscr{U}}$, is an injection and does not depend on the choice of $\varphi$. Henceforth we shall write $c_{\mathscr{V} \mathscr{U}}$ instead of $c(\varphi )$.

Let $\mathscr{R}$ be the set of elements of $\mathfrak{P}(\mathfrak{P}(B))$ which are open coverings of B. For every open covering $\mathscr{U}$ of B, there exists an open covering $\mathscr{V}$ belonging to $\mathscr{R}$ such that $\mathscr{U}$ is both finer and coarser than $\mathscr{U}$. The set $\mathscr{R}$ is ordered and filtering for the relation $\leqslant$ defined by $\mathscr{U}\leqslant \mathscr{V}$ if $\mathscr{V}$ is a covering finer than $\mathscr{U}$. It follows from the foregoing that an inductive system $(H^1_{cont}(B,\mathscr{U},G), c_{\mathscr{V} \mathscr{U}})$ relative to the filtered ordered set $\mathscr{R}$ has been defined and that the family $(r_{\mathscr{U}})$ is an inductive system of bijective mappings of $(H^1_{cont}(B,\mathscr{U},G), c_{\mathscr{V} \mathscr{U}})$ into $(P(B,\mathscr{U},G), i_{\mathscr{V} \mathscr{U}})$. If we denote by $H^1_{cont}(B,G)$ the inductive limit of the system $(H^1_{cont}(B,\mathscr{U},G), c_{\mathscr{V} \mathscr{U}})$ and by $r: H^1_{cont}(B,G)\rightarrow P(B,G)$ the inductive limit of the family $(r_{\mathscr{U}})$, we therefore have:

#### Theorem 4 {#ta-i-s5-thm-4 .statement tag=01RQ}

The mapping $r: H^1_{cont}(B,G)\rightarrow P(B,G)$ is bijective.

Let $\mathscr{U}= (U_i)_{i\in I}$ be an open covering of B; let us denote by $c_{\mathscr{U}}$ the canonical mapping $H^1_{cont}(B,\mathscr{U},G)\rightarrow H^1_{cont}(B,G)$. If $(g_{ij})$ is a cocycle on B, with values in G, subordinate to the open covering $\mathscr{U}$, the element $c_{\mathscr{U}}((g_{ij}))$ of $H^1_{cont}(B,G)$ is called the cohomology class of the cocycle $(g_{ij})$.

## EXERCISES {#ta-i-s5-exercises}

See the [exercises for § 5](exercises/s5/).
