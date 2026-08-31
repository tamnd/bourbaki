---
book: alg
book_title: Algebra
chapter: II
chapter_title: LINEAR ALGEBRA
section: 1
section_title: Modules
lang: en
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 191-227, 380-386
pdf_pages: 0215-0251, 0404-0410
extraction: ocr
subsections:
    - "no": 1
      title: MODULES; VECTOR SPACES; LINEAR COMBINATIONS
      page: 191
      pdf_page: 215
    - "no": 2
      title: LINEAR MAPPINGS
      page: 194
      pdf_page: 218
    - "no": 3
      title: SUBMODULES; QUOTIENT MODULES
      page: 196
      pdf_page: 220
    - "no": 4
      title: EXACT SEQUENCES
      page: 197
      pdf_page: 221
    - "no": 5
      title: PRODUCTS OF MODULES
      page: 200
      pdf_page: 224
    - "no": 6
      title: DIRECT SUM OF MODULES
      page: 202
      pdf_page: 226
    - "no": 7
      title: INTERSECTION AND SUM OF SUBMODULES
      page: 205
      pdf_page: 229
    - "no": 8
      title: DIRECT SUMS OF SUBMODULES
      page: 208
      pdf_page: 232
    - "no": 9
      title: SUPPLEMENTARY SUBMODULES
      page: 210
      pdf_page: 234
    - "no": 10
      title: MODULES OF FINITE LENGTH
      page: 212
      pdf_page: 236
    - "no": 11
      title: FREE FAMILIES. BASES
      page: 214
      pdf_page: 238
    - "no": 12
      title: ANNIHILATORS. FAITHFUL MODULES. MONOGENOUS MODULES
      page: 219
      pdf_page: 243
    - "no": 13
      title: CHANGE OF RING OF SCALARS
      page: 221
      pdf_page: 245
    - "no": 14
      title: MULTIMODULES
      page: 224
      pdf_page: 248
statements: 88
exercises: 27
content_sha256: 7397d09a718f6180624ef63d3ea605fc93db2eb8eb18c2019f1e6cb60606e9b8
---

## § 1. MODULES

### 1. MODULES; VECTOR SPACES; LINEAR COMBINATIONS

#### Definition 1 {#alg-ii-s1-def-1 .statement}

*Given a ring* $\mathbf{A}$, *a left module over* $\mathbf{A}$ (*or left* $\mathbf{A}$-*module*) *is a set* $\mathbf{E}$ *with an algebraic structure defined by giving*:

(1) *a commutative group law on* $\mathbf{E}$ (*written additively in what follows*);

(2) *a law of action* $(\alpha, x) \mapsto \alpha \top x$, *whose domain of operators is the ring* $\mathbf{A}$ *and which satisfies the following axioms*:

$$
\begin{align*}
(\mathbf{M_I})\quad & \alpha \top (x + y) = (\alpha \top x) + (\alpha \top y) \text{ for all } \alpha \in \mathbf{A}, x \in \mathbf{E}, y \in \mathbf{E}; \\
(\mathbf{M_{II}})\quad & (\alpha + \beta) \top x = (\alpha \top x) + (\beta \top x) \text{ for all } \alpha \in \mathbf{A}, \beta \in \mathbf{A}, x \in \mathbf{E}; \\
(\mathbf{M_{III}})\quad & \alpha \top (\beta \top x) = (\alpha \beta) \top x \text{ for all } \alpha \in \mathbf{A}, \beta \in \mathbf{A}, x \in \mathbf{E}; \\
(\mathbf{M_{IV}})\quad & 1 \top x = x \text{ for all } x \in \mathbf{E}.
\end{align*}
$$

Axiom $(\mathbf{M_I})$ means that the external law of a left $\mathbf{A}$-module $\mathbf{E}$ is *distributive* with respect to addition on $\mathbf{E}$; a module is thus a commutative group with operators.

If in Definition 1, axiom $(\mathbf{M_{III}})$ is replaced by

$$
(\mathbf{M'_{III}})\quad \alpha \top (\beta \top x) = (\beta \alpha) \top x \text{ for all } \alpha \in \mathbf{A}, \beta \in \mathbf{A}, x \in \mathbf{E},
$$

E with the algebraic structure thus defined is a right module over A or a right A-module.

When speaking of A-modules (left or right), the elements of the ring A are often called scalars.

Usually the external law of composition of a left A-module (resp. right A-module) is written multiplicatively, with the operator written on the left (resp. right); condition (M_{III}) is then written $\alpha(\beta x) = (\alpha\beta)x$, condition (M'_{III}) is written $(x\beta)\alpha = x(\beta\alpha)$.

If $A^0$ denotes the opposite ring to A (I, § 8, no. 3), every right module E over the ring A is a left module over the ring $A^0$. It follows that an exposition can be given of the properties of modules whilst systematically confining attention either to left modules or to right modules; in §§ 1 and 2 we shall in general give this exposition for left modules and when we speak of a module (without specifying which type) we shall mean a left module whose external law will be written multiplicatively. When the ring A is commutative the notions of right module and left module with respect to A are identical.

For all $\alpha \in A$, the mapping $x \mapsto \alpha x$ of an A-module E into itself is called the homothety of ratio $\alpha$ of E (I, § 4, no. 2); by (M_I) a homothety is an endomorphism of the commutative group structure (without operators) on E, but not in general of the module structure on E (I, § 4, no. 2; cf. II, § 1, no. 2 and no. 13). Hence $\alpha 0 = 0$ and $\alpha(-x) = -(\alpha x)$; if $\alpha$ is an invertible element of A, the homothety $x \mapsto \alpha x$ is an automorphism of the commutative group structure (without operators) on E, for the relation $y = \alpha x$ implies by virtue of (M_IV), $x = \alpha^{-1}(\alpha x) = \alpha^{-1}y$.

Similarly, by virtue of (M_{II}), for all $x \in E$, the mapping $\alpha \mapsto \alpha x$ is a homomorphism of the additive group A into the commutative group (without operators) E; hence $0x = 0$ and $(-\alpha)x = -(\alpha x)$; moreover, by (M_IV), for every integer $n \in \mathbf{Z}$, $n.x = (n.1)x$.

When the ring A consists only of the element 0, every A-module E consists only of the element 0, for then $1 = 0$ in A, whence, for all $x \in E$,
$x = 1.x = 0.x = 0$.

#### Example {#alg-ii-s1-n1-exa-1 .statement}

(1) Let $\phi$ be a homomorphism of a ring A into a ring B; the mapping $(a, x) \mapsto \phi(a)x$ (resp. $(a, x) \mapsto x\phi(a)$) of $A \times B$ into B defines on B a left (resp. right) A-module structure. In particular if $\phi$ is taken to be the identity mapping on A, a canonical left (resp. right) A-module structure is obtained on A; to avoid confusion, the set A with this structure is denoted by $A_s$ (resp. $A_d$).

(2) On a commutative group G (written additively) the group with operators structure defined by the external law $(n, x) \mapsto n.x$ (I, § 3, no. 1) is a module structure over the ring $\mathbf{Z}$ of rational integers.

(3) Let E be a commutative group written additively, $\mathcal{E}$ the endomorphism ring of E (I, § 8, no. 3: recall that the product $fg$ of two endomorphisms is by definition the composite endomorphism $f \circ g$). The external law $(f, x) \mapsto f(x)$ between operators $f \in \mathscr{E}$ and elements $x \in E$ defines on E a canonical left $\mathscr{E}$-module structure.

Consider now a ring A and suppose there is given on E a left (resp. right) A-module structure; for all $\alpha \in A$, the homothety $h_\alpha : x \mapsto \alpha x$ (resp. $x \mapsto x\alpha$) belongs to $\mathscr{E}$; the mapping $\phi : \alpha \mapsto h_\alpha$ is a homomorphism of the ring A (resp. the opposite ring $A^0$) into the ring $\mathscr{E}$ and by definition $\alpha x = (\phi(\alpha))(x)$ (resp. $x\alpha = (\phi(\alpha))(x)$). Conversely, giving a ring homomorphism $\phi : A \to \mathscr{E}$ (resp. $\phi : A^0 \to \mathscr{E}$) defines a left (resp. right) A-module structure on E by the above formulae. In other words, being given a left (resp. right) A-module structure on an additive group E with additive law the given group law is equivalent to being given a ring homomorphism $A \to \mathscr{E}$ (resp. $A^0 \to \mathscr{E}$).

#### Definition 2 {#alg-ii-s1-def-2 .statement}

*A left (resp. right) vector space over a field K is a left (resp. right) K-module.*

The elements of a vector space are sometimes called *vectors*.

#### Example {#alg-ii-s1-n1-exa-2 .statement}

(4) A field is both a left and a right vector space with respect to any of its subfields.

*(5)* The real number space of three dimensions $\mathbf{R}^3$ is a vector space with respect to the field of real numbers $\mathbf{R}$, the product $tx$ of a real number $t$ and a point $x$ with coordinates $x_1, x_2, x_3$ being the point with coordinates $tx_1, tx_2, tx_3$. Similarly, the set of real-valued functions defined on an arbitrary set F is a vector space with respect to $\mathbf{R}$, the product $tf$ of a real number $t$ and a function $f$ being the real-valued function $x \mapsto tf(x)$.*

For two families $(x_i)_{i \in I}, (y_i)_{i \in I}$ of elements of an A-module E of finite support (I, § 2, no. 1), the following equations hold:

(1)
$$
\sum_{i \in I} (x_i + y_i) = \sum_{i \in I} x_i + \sum_{i \in I} y_i
$$

(2)
$$
\alpha \cdot \sum_{i \in I} x_i = \sum_{i \in I} (\alpha x_i) \quad \text{for all } \alpha \in A;
$$
the equations are immediately reduced to the analogous equations for finite sums by considering a finite subset H of I containing the supports of $(x_i)$ and $(y_i)$.

#### Definition 3 {#alg-ii-s1-def-3 .statement}

*An element x of an A-module E is said to be a linear combination with coefficients in A of a family $(a_i)_{i \in I}$ of elements of E if there exists a family $(\lambda_i)_{i \in I}$ of elements of A, of finite support, such that $x = \sum_{i \in I} \lambda_i a_i$.*

In general there are several distinct families $(\lambda_i)$ satisfying this condition (cf. no. 11).

Note that 0 is the only linear combination of the empty family of elements of E (by the convention of I, § 2, no. 1).

### 2. LINEAR MAPPINGS

#### Definition 4 {#alg-ii-s1-def-4 .statement}

Let E and F be two (left) modules with respect to the same ring A. A linear mapping (or A-linear mapping, or homomorphism, or A-homomorphism) of E into F is any mapping u : E → F such that:

(3) $u(x + y) = u(x) + u(y)$ for $x \in E, y \in E;$

(4G) $u(\lambda . x) = \lambda . u(x)$ for $\lambda \in A, x \in E.$

If E and F are two right A-modules, a linear mapping $u : E \to F$ is a mapping satisfying (3) and

(4D) $u(x . \lambda) = u(x) . \lambda$ for $\lambda \in A, x \in E.$

#### Remark {#alg-ii-s1-n2-rem-1 .statement}

When E and F are two commutative groups considered as modules over the ring $\mathbf{Z}$ (no. 1), every homomorphism $u$ of the group E (without operators) into the group F (without operators) is also a linear mapping of E into F, since for n an integer > 0, the relation $u(n . x) = n . u(x)$ follows from $u(x + y) = u(x) + u(y)$ by induction on n and for $n = -m < 0$,
$$
u(n . x) = u(-(m . x)) = -u(m . x) = -(m . u(x)) = n . u(x).
$$

#### Example {#alg-ii-s1-n2-exa-1 .statement}

(1) Let E be an A-module and a an element of E; the mapping $\lambda \mapsto \lambda a$ of the A-module $A_s$ into E is a linear mapping $\theta_a$ such that $\theta_a(1) = a.$
*(2) Let I be an open interval of the real line $\mathbf{R}$, E the vector space of differentiable real-valued functions on I and F the vector space of all real-valued functions defined on I. The mapping $x \mapsto x'$ which associates with every differentiable function x its derivative is a linear mapping from E to F.*

Note that a homothety $x \mapsto \alpha x$ on an A-module E is not necessarily a linear mapping: in other words, the relation $\alpha(\lambda x) = \lambda(\alpha x)$ does not necessarily hold for all $\lambda \in A$ and $x \in E$. This relation is however true when $\alpha$ belongs to the centre of A; $x \mapsto \alpha x$ is then called a central homothety (cf. no. 13).

If $u : E \to F$ is a linear mapping, then, for every family $(x_i)_{i \in I}$ of elements of E and every family $(\lambda_i)_{i \in I}$ of elements of A such that the support of the family $(\lambda_i x_i)_{i \in I}$ is finite,

$$
u\left( \sum_{i \in I} \lambda_i x_i \right) = \sum_{i \in I} \lambda_i u(x_i)
$$

as follows immediately from (3) and (4G) by induction on the cardinal of the support of the family $(\lambda_i x_i)$.

#### Proposition 1 {#alg-ii-s1-prop-1 .statement}

Let E, F, G be three A-modules, u a linear mapping of E into F and v a linear mapping of F into G. Then the composite mapping $v \circ u$ is linear.

(1) *If u:E → F and v:F → E are two linear mappings such that v ∘ u is the identity mapping on E and u ∘ v is the identity mapping on F, u is an isomorphism of E onto F and v is the inverse isomorphism.*

(2) *Every bijective linear mapping u:E → F is an isomorphism of E onto F.*

These propositions follow immediately from Definition 4.

Propositions 1 and 2 show that linear mappings can be taken as the *morphisms* for the species of A-module structures (*Set Theory*, IV, § 2, no. 1); we shall henceforth always assume that this choice of morphisms has been made.

Given two left (resp. right) A-modules E and F, let Hom(E, F) or Hom_A(E, F) denote the set of linear mappings of E into F.

The set Hom(E, F) is a *commutative ring*, a subgroup of the product commutative group F^E of all mappings of E into F (I, § 4, no. 8); recall that for two elements u, v of F^E and for all x ∈ E,

$$(u + v)(x) = u(x) + v(x), \quad (-u)(x) = -u(x)$$

whence it follows immediately that, if u and v are linear, so are u + v and −u. If G is a third left (resp. right) A-module, f, f_1, f_2 elements of Hom(E, F) and g, g_1, g_2 elements of Hom(F, G), the following relations are immediately verified:

(6) $$g \circ (f_1 + f_2) = g \circ f_1 + g \circ f_2$$
(7) $$(g_1 + g_2) \circ f = g_1 \circ f + g_2 \circ f$$
(8) $$g \circ (-f) = (-g) \circ f = -(g \circ f).$$

In particular, the law of composition (f, g) ↦ f ∘ g on Hom(E, E) defines with the above additive group structure a *ring* structure on Hom(E, E) whose unit element, denoted by 1_E or Id_E, is the identity mapping on E; the linear mappings of E into itself are also called *endomorphisms* of the A-module E and the ring Hom(E, E) is also denoted by End(E) or End_A(E). The *automorphisms* of the A-module E are just the *invertible* elements of End(E) (Proposition 2); they form a multiplicative *group*, denoted by Aut(E) or GL(E) which is also called the *linear group* relative to E.

It follows from (6) and (7) that, for two A-modules E, F, Hom(E, F) has the canonical structure of a *left module* over the ring Hom(F, F) and of a *right module* over Hom(E, E).

Let E, F, E', F' be four (left) A-modules, u:E' → E and v:F → F' A-linear mappings. If every element f ∈ Hom(E, F) is associated with the element v ∘ f ∘ u ∈ Hom(E', F'), a mapping

$$\operatorname{Hom}(E, F) \to \operatorname{Hom}(E', F')$$

is defined, which is $\mathbf{Z}$-linear and which is denoted by $\mathrm{Hom}(u, v)$ or $\mathrm{Hom}_A(u, v)$. If $u, u_1, u_2$ belong to $\mathrm{Hom}(E', E)$ and $v, v_1, v_2$ to $\mathrm{Hom}(F, F')$, then

$$
\begin{cases}
\mathrm{Hom}(u_1 + u_2, v) = \mathrm{Hom}(u_1, v) + \mathrm{Hom}(u_2, v) \\
\mathrm{Hom}(u, v_1 + v_2) = \mathrm{Hom}(u, v_1) + \mathrm{Hom}(u, v_2)
\end{cases}
$$

Let $E'', F''$ be two $A$-modules, $u': E'' \to E'$ and $v': F' \to F''$ linear mappings. Then

$$
\mathrm{Hom}(u \circ u', v' \circ v) = \mathrm{Hom}(u', v') \circ \mathrm{Hom}(u, v).
$$

If $u$ is an isomorphism of $E'$ onto $E$ and $v$ an isomorphism of $F$ onto $F'$, $\mathrm{Hom}(u, v)$ is an isomorphism of $\mathrm{Hom}(E, F)$ onto $\mathrm{Hom}(E', F')$ whose inverse isomorphism is $\mathrm{Hom}(u^{-1}, v^{-1})$ by (10).

If $h$ (resp. $k$) is an endomorphism of $E$ (resp. $F$), $\mathrm{Hom}(h, 1_F)$ (resp. $\mathrm{Hom}(1_E, k)$) is just the homothety with ratio $h$ (resp. $k$) for the right (resp. left) module structure on the ring $\mathrm{End}(E)$ (resp. $\mathrm{End}(F)$) defined above.

### 3. SUBMODULES; QUOTIENT MODULES

Let $E$ be an $A$-module and $M$ a subset of $E$; for the $A$-module structure on $E$ to induce an $A$-module structure on $M$, it is necessary and sufficient that $M$ be a stable subgroup of $E$ (I, § 4, no. 3), for if this is so, the structure of a group with operators induced on $M$ obviously satisfies axioms ($M_{II}$), ($M_{III}$) and ($M_{IV}$); then $M$ with this structure (or, by an abuse of language, the set $M$ itself) is called a submodule of $E$; the canonical injection $M \to E$ is a linear mapping. When $E$ is a vector space, its submodules are called vector subspaces (or simply subspaces if no confusion can arise).

#### Example {#alg-ii-s1-n3-exa-1 .statement}

(1) In any module $E$ the set consisting of 0 is a submodule (the zero submodule, often denoted by 0, by an abuse of notation).
(2) Let $A$ be a ring. The submodules of $A_s$ (resp. $A_d$) are just the left ideals (resp. right ideals) of the ring $A$.
(3) Let $E$ be an $A$-module, $x$ an element of $E$ and $a$ a left ideal of $A$. The set of elements $\alpha x$, where $\alpha$ runs through $a$, is a submodule of $E$, denoted by $ax$.
(4) In a commutative group $G$ considered as a $\mathbf{Z}$-module (no. 1), every subgroup of $G$ is also a submodule.

*(5) Let $I$ be an open interval of the real line $\mathbf{R}$; the set $C$ of real-valued functions defined and continuous on $I$ is a vector subspace of the vector space $\mathbf{R}^I$ of all real-valued functions defined on $I$. Similarly, the set $D$ of differentiable functions on $I$ is a vector subspace of $C_*$*

Let $E$ be an $A$-module. Every equivalence relation compatible (I, § 1, no. 6) with the module structure on $E$ is of the form $x - y \in M$, where $M$ is a stable subgroup of E (I, § 4, no. 4), that is a submodule of E. It is immediately verified that the structure of a group with operators on the quotient group E/M (I, § 4, no. 4) is an A-module structure, under which the canonical mapping $E \to E/M$ is linear; with this structure, E/M is called the *quotient module* of E by the submodule M. A quotient module of a vector space E is called a *quotient vector space* (or simply *quotient space*) of E.

*Example* (6). Every left ideal $a$ in a ring A defines a quotient module $A_s/a$ of the left A-module $A_s$; by an abuse of notation, this quotient module is often denoted by $A/a$.

Let E, F be two A-modules. It follows from the general properties of groups with operators (I, § 4, no. 5) (or directly from the definitions) that if $u : E \to F$ is a linear mapping, the image under $u$ of any submodule of E is a submodule of F and the inverse image under $u$ of any submodule of F is a submodule of E. In particular, the *kernel* $N = \overline{u}^{-1}(0)$ is a submodule of E and the image $u(E)$ of E under $u$ is a submodule of F (I, § 4, no. 6, Proposition 7); by an abuse of language $u(E)$ is called the *image of u*. The quotient module $E/N$ is also called the *coimage* of $u$ and the quotient module $F/u(E)$ the *cokernel* of $u$. In the *canonical decomposition* of $u$ (I, § 4, no. 5)

$$
u : E \xrightarrow{p} E/N \xrightarrow{v} u(E) \xrightarrow{i} F
$$

$v$ is an *isomorphism* of the coimage of $u$ onto the image of $u$ (no. 2, Proposition 2). For $u$ to be *injective*, it is necessary and sufficient that its kernel be zero; for $u$ to be *surjective*, it is necessary and sufficient that its cokernel be zero.

The kernel, image, coimage and cokernel of $u$ are denoted respectively by Ker $u$, Im $u$, Coim $u$, Coker $u$.

#### Remark {#alg-ii-s1-n3-rem-1 .statement}

Let M be a submodule of an A-module E and $\phi : E \to E/M$ the canonical homomorphism. For an A-linear mapping $u : E \to F$ to be of the form $v \circ \phi$, where $v$ is a linear mapping of E/M into F, it is necessary and sufficient that $M \subset \mathrm{Ker}(u)$; for, if this condition holds, the relation $x - y \in M$ implies $u(x) = u(y)$, hence $u$ is compatible with this equivalence relation and clearly the mapping $v : E/M \to F$ derived from $u$ by taking quotients is linear.

### 4. EXACT SEQUENCES

#### Definition 5 {#alg-ii-s1-def-5 .statement}

*Let F, G, H be three A-modules; let f be a homomorphism of F into G and g a homomorphism of G into H. The ordered pair (f, g) is called an exact sequence if*

$$
g^{-1}(0) = f(F)
$$

*in other words, if the kernel of g is equal to the image of f.*

The diagram

(12)
$$
F \xrightarrow{f} G \xrightarrow{g} H
$$
is also called an *exact sequence*.

We consider similarly a diagram consisting of four A-modules and three homomorphisms:

(13)
$$
E \xrightarrow{f} F \xrightarrow{g} G \xrightarrow{h} H.
$$

This diagram is called *exact at* F if the diagram $E \xrightarrow{f} F \xrightarrow{g} G$ is exact; it is called *exact at* G if $F \xrightarrow{g} G \xrightarrow{h} H$ is exact. If diagram (13) is *exact at* F *and at* G, it is simply called *exact*, or an *exact sequence*. Exact sequences with an arbitrary number of terms are defined similarly.

#### Remark {#alg-ii-s1-n4-rem-1 .statement}

(1) If the ordered pair $(f, g)$ is an exact sequence, then $g \circ f = 0$; but of course this property does not characterize exact sequences, for it only means that the image of $f$ is *contained* in the kernel of $g$.

In the statements below, E, F, G denote A-modules, 0 the A-module reduced to its identity element; the arrows represent A-module homomorphisms. As there is only one homomorphism from the module 0 to a module E (resp. of E to 0), there is no point in giving these homomorphisms a name in the exact sequences where they appear.

#### Proposition 3 {#alg-ii-s1-prop-3 .statement}

(a) *For*
$$
0 \longrightarrow E \xrightarrow{f} F
$$
*to be an exact sequence, it is necessary and sufficient that* $f$ *be injective*.

(b) *For*
$$
E \xrightarrow{f} F \longrightarrow 0
$$
*to be an exact sequence, it is necessary and sufficient that* $f$ *be surjective*.

(c) *For*
$$
0 \longrightarrow E \xrightarrow{f} F \longrightarrow 0
$$
*to be an exact sequence, it is necessary and sufficient that* $f$ *be bijective* (in other words (no. 2, Proposition 2) that $f$ be an *isomorphism* of E onto F).

(d) *If* F *is a submodule of* E *and* $i : F \to E$ *is the canonical injection,* $p : E \to E/F$ *the canonical homomorphism, the diagram*
(14)
$$
0 \longrightarrow F \xrightarrow{i} E \xrightarrow{p} E/F \longrightarrow 0
$$
*is an exact sequence.*

(e) *If $f : E \to F$ is a homomorphism, the diagram*

$$
0 \longrightarrow f^{-1}(0) \overset{i}{\longrightarrow} E \overset{f}{\longrightarrow} F \overset{p}{\longrightarrow} F/f(E) \to 0
$$

*(where $i$ is the canonical injection and $p$ the canonical surjection) is an exact sequence.*

The proposition follows immediately from the definitions and Proposition 2 of no. 2.

#### Remark {#alg-ii-s1-n4-rem-2 .statement}

(2) To say that there is an exact sequence

$$
0 \longrightarrow E \overset{f}{\longrightarrow} F \overset{g}{\longrightarrow} G \longrightarrow 0
$$

means that $f$ is injective, $g$ surjective and that the canonical bijection associated with $g$ is an *isomorphism* of $F/f(E)$ onto $G$. It is also said that the triple $(F, f, g)$ is an *extension of the module G by the module E* (I, § 6, no. 7).

(3) If there is an exact sequence with 4 terms

$$
E \overset{f}{\longrightarrow} F \overset{g}{\longrightarrow} G \overset{h}{\longrightarrow} H
$$

the cokernel of $f$ is $F/f(E) = F/g^{-1}(0)$ and the kernel of $h$ is $g(F)$; the canonical bijection associated with $g$ is therefore an *isomorphism*

$$
\operatorname{Coker} f \to \operatorname{Ker} h.
$$

(4) Consider an ordered pair of A-module homomorphisms

$$(15)$$
$$
E \overset{f}{\longrightarrow} F \overset{g}{\longrightarrow} G.
$$

For diagram (15) to be an exact sequence, it is necessary and sufficient that there exist two A-modules S, T and homomorphisms $a : E \to S,\ b : S \to F,\ c : F \to T,\ d : T \to G$ such that the three sequences

$$(16)$$
$$
\begin{cases}
E \overset{a}{\longrightarrow} S \longrightarrow 0 \\
0 \longrightarrow S \overset{b}{\longrightarrow} F \overset{c}{\longrightarrow} T \longrightarrow 0 \\
0 \longrightarrow T \overset{d}{\longrightarrow} G
\end{cases}
$$

are *exact* and $f = b \circ a$ and $g = d \circ c$.

If (15) is an exact sequence, then take $S = f(E) = g^{-1}(0)$ and $T = g(F)$, $b$ and $d$ being the canonical injections and $a$ (resp. $c$) the homomorphism with the same graph as $f$ (resp. $g$). Conversely, if S, T, a, b, c, d satisfy the above conditions, then $f(E) = b(a(E)) = b(S)$ and $g^{-1}(0) = c(d(0)) = c(0)$, hence the exactness of (16) shows that $f(E) = g^{-1}(0)$.

The use of explicit letters to denote homomorphisms in an exact sequence is often dispensed with when it is not necessary for the arguments.

#### Remark {#alg-ii-s1-n4-rem-3 .statement}

(5) The definition of an exact sequence extends immediately to groups which are not necessarily commutative; in this case of course multiplicative notation is used with 0 replaced by 1 in the formulae (if no confusion arises). Parts (a), (b), (c) of Proposition 3 are still valid and also (d) when F is a normal subgroup of E. Remark 2 and Proposition 3(e) hold on condition that $f(E)$ is a normal subgroup of F; Remarks 3 and 4 are valid without modification.

### 5. PRODUCTS OF MODULES

Let $(E_i)_{i \in I}$ be a family of modules over the same ring A. It is immediately verified that the product of the module structures on the $E_i$ ($I, § 4,$ no. 8) is an A-module structure on the product set $E = \prod_{i \in I} E_i$. With this structure the set E is called the product module of the modules $E_i$; if $x = (x_i), y = (y_i)$ are two elements of E, then

$$
\begin{cases}
x + y = (x_i + y_i) \\
\lambda \cdot x = (\lambda x_i)
\end{cases}
$$
for all $\lambda \in A$.

Formulae (17) express the fact that the projections $pr_i : E \to E_i$ are linear mappings; these mappings are obviously surjective.

Recall that if the indexing set I is empty, the product set $\prod_{i \in I} E_i$ then consists of a single element; the product module structure on this set is then that under which this unique element is 0.

#### Proposition 4 {#alg-ii-s1-prop-4 .statement}

*Let* $E = \prod_{i \in I} E_i$ *be the product of a family of A-modules* $(E_i)_{i \in I}$. *For every A-module* F *and every family of linear mappings* $f_i : F \to E_i$ *there exists one and only one mapping* f *of* F *into* E *such that* $pr_i \circ f = f_i$ *for all* $i \in I$ *and this mapping is linear*.

This follows directly from the definitions.

Product of modules is "associative": if $(J_\lambda)_{\lambda \in L}$ is a partition of I, the canonical mapping
$$
\prod_{i \in I} E_i \to \prod_{\lambda \in L} \left( \prod_{i \in J_\lambda} E_i \right)
$$
is an isomorphism.

#### Proposition 5 {#alg-ii-s1-prop-5 .statement}

(i) *Let* $(E_i)_{i \in I}, (F_i)_{i \in I}$ *be two families of A-modules with the same indexing set* I; *for every family of linear mappings* $f_i : E_i \to F_i$ ($i \in I$), *the mapping* $f : (x_i) \to (f_i(x_i))$ *of* $\prod_i E_i$ *into* $\prod_i F_i$ *(sometimes denoted by* $\prod_i f_i$) *is linear*.

(ii) *Let* $(G_i)_{i \in I}$ *be a third family of A-modules with* I *as indexing set and, for all* $i \in I,$ let $g_i : F_i \to G_i$ be a linear mapping; let $g = \prod_i g_i$. For each of the sequences $E_i \xrightarrow{f_i} F_i \xrightarrow{g_i} G_i$ to be exact, it is necessary and sufficient that the sequence

$$
\prod_i E_i \xrightarrow{f} \prod_i F_i \xrightarrow{g} \prod_i G_i
$$

be exact.

Assertion (i) follows immediately from the definitions. On the other hand, to say that $y = (y_i)$ belongs to $\operatorname{Ker}(g)$ means that $g_i(y_i) = 0$ for all $i \in I$ and hence that $y_i \in \operatorname{Ker}(g_i)$ for all $i \in I$; similarly, to say that $y$ belongs to $\operatorname{Im}(f)$ means that there exists $x = (x_i) \in \prod_i E_i$ such that $y = f(x)$, which is equivalent to saying that $y_i = f_i(x_i)$ for all $i \in I$ or also that $y_i \in \operatorname{Im}(f_i)$ for all $i \in I$; whence (ii).

#### Corollary {#alg-ii-s1-n5-cor-1 .statement}

Under the conditions of Proposition 5, (i),

$$
\operatorname{Ker}(f) = \prod_{i \in I} \operatorname{Ker}(f_i), \qquad \operatorname{Im}(f) = \prod_{i \in I} \operatorname{Im}(f_i)
$$

and there are canonical isomorphisms

$$
\operatorname{Coim}(f) \to \prod_{i \in I} \operatorname{Coim}(f_i), \qquad \operatorname{Coker}(f) = \prod_{i \in I} \operatorname{Coker}(f_i)
$$

obtained by respectively associating with the class of an element $x = (x_i)$ of $\prod_i E_i$, mod $\operatorname{Ker}(f)$, (resp. with the class of an element $y = (y_i)$ of $\prod_i F_i$, mod. $\operatorname{Im}(f)$) the family of classes of the $x_i$ mod. $\operatorname{Ker}(f_i)$ (resp. the family of classes of the $y_i$ mod. $\operatorname{Im}(f)$).

In particular, for $f$ to be injective (resp. surjective, bijective, zero) it is necessary and sufficient that, for all $i \in I$, $f_i$ be injective (resp. surjective, bijective, zero).

If, for all $i \in I$, we consider a submodule $F_i$ of $E_i$, the module $\prod_{i \in I} F_i$ is a submodule of $\prod_{i \in I} E_i$ and by virtue of the Corollary to Proposition 5, there is a canonical isomorphism

$$
\prod_{i \in I} (E_i/F_i) \to \left( \prod_{i \in I} E_i \right) / \left( \prod_{i \in I} F_i \right).
$$

An important example of a product of modules is that where all the factor modules are equal to the same module $F$; their product $F^I$ is then just the set of mappings of $I$ into $F$. The diagonal mapping $F \to F^I$ mapping $x \in F$ to the constant function equal to $x$ on $I$ is linear. If $(E_i)_{i \in I}$ is a family of $A$-modules and, for all $i \in I$, $f_i : F \to E_i$ is a linear mapping, then the linear mapping $x \mapsto (f_i(x))$ of $F$ into $\prod_{i \in I} E_i$ is the composition of the mapping $(x_i) \mapsto (f_i(x_i))$ of $F^I$ into $\prod_{i \in I} E_i$ and the diagonal mapping $F \to F^I$.

### 6. DIRECT SUM OF MODULES

Let $(E_i)_{i \in I}$ be a family of A-modules and $F = \prod_{i \in I} E_i$ their product. The set $E$ of $x \in F$ such that $\mathrm{pr}_i x = 0$ except for a finite number of indices is obviously a submodule of $F$, called the external direct sum (or simply direct sum) of the family of modules $(E_i)$ and denoted by $\bigoplus_{i \in I} E_i$ (I, § 4, no. 9). When I is finite, then $\bigoplus_{i \in I} E_i = \prod_{i \in I} E_i$; if $I = \{p, q\}$ (interval of $\mathbf{Z}$), we also write

$$
\bigoplus_{i \in I} E_i = E_p \oplus E_{p+1} \oplus \cdots \oplus E_q.
$$

For all $\kappa \in I$, let $j_\kappa$ be the mapping $E_\kappa \to F$ which associates with each $x_\kappa \in E_\kappa$ the element of $F$ such that $\mathrm{pr}_i(j_\kappa(x_\kappa)) = 0$ for $i \neq \kappa$ and $\mathrm{pr}_\kappa(j_\kappa(x_\kappa)) = x_\kappa$; it is immediate that $j_\kappa$ is an injective linear mapping of $E_\kappa$ into the direct sum $E$ of the $E_i$, which we shall call the canonical injection; the submodule $j_\kappa(E_\kappa)$ of $E$, isomorphic to $E_\kappa$, is called the component submodule of $E$ of index $\kappa$. It is often identified with $E_\kappa$ by means of $j_\kappa$.

For all $x \in E = \bigoplus_{i \in I} E_i$, we have therefore

$$
x = \sum_{i \in I} j_i(\mathrm{pr}_i x).
$$

(20)

#### Proposition 6 {#alg-ii-s1-prop-6 .statement}

*Let* $(E_i)_{i \in I}$ *be a family of A-modules*, $M$ *an A-module and, for all* $i \in I$, *let* $f_i : E_i \to M$ *be a linear mapping*. *Then there exists one and only one linear mapping* $g : \bigoplus_{i \in I} E_i \to M$ *such that, for all* $i \in I$:

$$
g \circ j_i = f_i.
$$

(21)

By virtue of (20), if $g$ exists, then necessarily, for all $x \in \bigoplus_{i \in I} E_i$,

$$
g(x) = \sum_i g(j_i(\mathrm{pr}_i(x))) = \sum_i f_i(\mathrm{pr}_i(x)),
$$

whence the uniqueness of $g$. Conversely, setting $g(x) = \sum_i f_i(\mathrm{pr}_i(x))$ for all $x \in \bigoplus_{i \in I} E_i$, it is immediately verified that a linear mapping has been defined satisfying the conditions of the statement.

When no confusion can arise, we write $g = \sum_{i \in I} f_i$ (which is contrary to the conventions of I, § 2, no. 1, when the family $(f_i)$ is not of finite support).

In particular, if J is any subset of I, the canonical injections $j_i$ for $i \in J$ define a canonical linear mapping $j_J : \bigoplus_{i \in J} E_i \to \bigoplus_{i \in I} E_i$, which associates with each $(x_i)_{i \in I}$ the element $(x'_i)_{i \in I}$ such that $x'_i = x_i$ for $i \in J$, $x'_i = 0$ for $i \notin J$; this mapping is obviously injective. Moreover, if $(J_\lambda)_{\lambda \in L}$ is a partition of I, the mapping $i : \bigoplus_{\lambda \in L} \left( \bigoplus_{i \in J_\lambda} E_i \right) \to \bigoplus_{i \in I} E_i$ corresponding to the family $(j_{J_\lambda})$ by Proposition 6 is an *isomorphism* called canonical ("associativity" of direct sums).

#### Corollary 1 {#alg-ii-s1-prop-6-cor-1 .statement}

*Let $(E_i)_{i \in I}, (F_\lambda)_{\lambda \in L}$ be two families of A-modules. The mapping*
$$
\text{Hom}_A \left( \bigoplus_{i \in I} E_i, \prod_{\lambda \in L} F_\lambda \right) \to \prod_{(i, \lambda) \in I \times L} \text{Hom}_A(E_i, F_\lambda)
$$
*which associates with each $g \in \text{Hom}_A \left( \bigoplus_{i \in I} E_i, \prod_{\lambda \in L} F_\lambda \right)$ the family $(\operatorname{pr}_\lambda \circ g \circ j_i)$, is a $\mathbf{Z}$-module isomorphism (called canonical).*

This follows from Proposition 6 and no. 5, Proposition 4.

#### Corollary 2 {#alg-ii-s1-prop-6-cor-2 .statement}

*Let $(E_i)_{i \in I}$ be a family of A-modules, F an A-module and, for each $i \in I$, let $f_i : E_i \to F$ be a linear mapping. For $f = \sum_{i \in I} f_i$ to be an isomorphism of $E = \bigoplus_{i \in I} E_i$ onto F, it is necessary and sufficient that there exist for each $i \in I$ a linear mapping $g_i : F \to E_i$ with the following properties:*
(1) $g_i \circ f_i = 1_{E_i}$ for all $i \in I$.
(2) $g_i \circ f_\kappa = 0$ for $i \neq \kappa$.
(3) *For all $y \in F$, the family $(g_i(y))$ has finite support and*
$$
y = \sum_{i \in I} f_i(g_i(y)).
$$
Note that if I is finite, the last condition may also be written as
$$
\sum_{i \in I} f_i \circ g_i = 1_F.
$$
Obviously the conditions are necessary for they are satisfied by the $g_i = \operatorname{pr}_i \circ f_i^{-1}$. Conversely if they hold, for all $y \in F$, $g(y) = \sum_i j_i(g_i(y))$ is defined and it is immediate that $g$ is a linear mapping of F into E. For all $y \in F$, $f(g(y)) = \sum_i f_i(g_i(y)) = y$ by hypothesis. On the other hand, for all $x \in E$, $g_\kappa(f(x)) = g_\kappa \left( \sum_i f_i(\operatorname{pr}_i(x)) \right) = g_\kappa(f_\kappa(\operatorname{pr}_\kappa(x))) = \operatorname{pr}_\kappa(x)$ by hypothesis;

therefore $g(f(x)) = \sum_i j_i(g_i(f(x))) = \sum_i j_i(\mathrm{pr}_i(x)) = x$, which proves the corollary.

#### Proposition 7 {#alg-ii-s1-prop-7 .statement}

(i) *Let* $(E_i)_{i \in I}, (F_i)_{i \in I}$ *be two families of* $A$*-modules with the same indexing set* $I$; *for every family of linear mappings* $f_i : E_i \to F_i$ ($i \in I$), *the restriction to* $\bigoplus_{i \in I} E_i$ *of the linear mapping* $(x_i) \mapsto (f_i(x_i))$ *is a linear mapping* $f : \bigoplus_{i \in I} E_i \to \bigoplus_{i \in I} F_i$ *denoted by* $\bigoplus_{i \in I} f_i$ *or* $\bigoplus_i f_i$ *(where* $f = f_p \oplus f_{p+1} \oplus \cdots \oplus f_q$ *if* $I = [p, q]$ *is an interval in* $\mathbf{Z}$*).*

(ii) *Let* $(G_i)_{i \in I}$ *be a third family of* $A$*-modules with* $I$ *as indexing set and, for all* $i \in I$, *let* $g_i : F_i \to G_i$ *be a linear mapping; we write* $g = \bigoplus_i g_i$. *For each of the sequences* $E_i \xrightarrow{f_i} F_i \xrightarrow{g_i} G_i$ *to be exact, it is necessary and sufficient that the sequence*
$$
\bigoplus_i E_i \xrightarrow{f} \bigoplus_i F_i \xrightarrow{g} \bigoplus_i G_i
$$
*be exact*.

Obviously, for all $(x_i) \in \bigoplus_i E_i$, the family $(f_i(x_i))$ has finite support, whence (i). On the other hand, to say that an element $y = (y_i)$ of $\bigoplus_i F_i$ belongs to $\mathrm{Ker}(g)$ means that $y_i \in \mathrm{Ker}(g_i)$ for all $i \in I$ (no. 5, Proposition 5); similarly, if $y_i \in \mathrm{Im}(f_i)$ for all $i \in I$, there exists for each $i \in I$ an $x_i \in E_i$ such that $y_i = f_i(x_i)$ and when $y_i = 0$, it may be supposed that $x_i = 0$; hence $y \in \mathrm{Im}(f)$ and the converse is obvious.

#### Corollary 1 {#alg-ii-s1-prop-7-cor-1 .statement}

*Under the conditions of Proposition 7, (i),*
$$
\mathrm{Ker}(f) = \bigoplus_{i \in I} \mathrm{Ker}(f_i), \qquad \mathrm{Im}(f) = \bigoplus_{i \in I} \mathrm{Im}(f_i)
$$
*and there are canonical isomorphisms*
$$
\mathrm{Coim}(f) \to \bigoplus_{i \in I} \mathrm{Coim}(f_i), \qquad \mathrm{Coker}(f) \to \bigoplus_{i \in I} \mathrm{Coker}(f_i)
$$
*defined as in no. 5, Corollary to Proposition 5. In particular, for* $f$ *to be injective (resp. surjective, bijective, zero), it is necessary and sufficient that each of the* $f_i$ *be injective (resp surjective, bijective, zero)*.

If, for all $i \in I$, we consider a submodule $F_i$ of $E_i$, the module $\bigoplus_{i \in I} F_i$ is a submodule of $\bigoplus_{i \in I} E_i$ and, by virtue of Corollary 1 to Proposition 7, there is a canonical isomorphism
$$
\bigoplus_{i \in I} (E_i/F_i) \to \left( \bigoplus_{i \in I} E_i \right) / \left( \bigoplus_{i \in I} F_i \right).
$$

#### Corollary 2 {#alg-ii-s1-prop-7-cor-2 .statement}

Let $(E_i)_{i \in I}, (E'_i)_{i \in I}, (F_\lambda)_{\lambda \in L}, (F'_\lambda)_{\lambda \in L}$ be four families of $A$-modules and, for each $i \in I$ (resp. each $\lambda \in L$), $u_i : E'_i \to E_i$ (resp. $v_\lambda : F_\lambda \to F'_\lambda$) a linear mapping. Then the diagram

$$
\begin{array}{ccc}
\operatorname{Hom}\left( \bigoplus_{i \in I} E'_i, \prod_{\lambda \in L} F'_\lambda \right) & \xrightarrow{\phi'} & \prod_{(i, \lambda) \in I \times L} \operatorname{Hom}(E'_i, F'_\lambda) \\
\uparrow & & \uparrow \\
\operatorname{Hom}\left( \bigoplus_i u_i, \prod_\lambda v_\lambda \right) & & \prod \operatorname{Hom}(u_i, v_\lambda) \\
\operatorname{Hom}\left( \bigoplus_{i \in I} E_i, \prod_{\lambda \in L} F_\lambda \right) & \xrightarrow{\phi} & \prod_{(i, \lambda) \in I \times L} \operatorname{Hom}(E_i, F_\lambda)
\end{array}
$$

(where $\phi$ and $\phi'$ are the canonical isomorphisms defined in Corollary 1 to Proposition 6) is commutative.

The verification follows immediately from the definitions.

When all the $E_i$ are equal to the same $A$-module $E$, the direct sum $\bigoplus_{i \in I} E_i$ is also denoted by $E^{(I)}$: its elements are the mappings of $I$ into $E$ with finite support. If, for all $i$, $f_i$ is taken to be the identity mapping $E \to E$, by Proposition 6, a linear mapping $E^{(I)} \to E$ is obtained, called *codiagonal*, which associates with every family $(x_i)_{i \in I}$ of elements of $E$, of finite support, its *sum* $\sum_{i \in I} x_i$.

#### Remark {#alg-ii-s1-n6-rem-1 .statement}

Recall that the definition of direct sum extends immediately to a family $(E_i)_{i \in I}$ of *groups* which are not necessarily commutative, multiplicative notation of course replacing the additive notation; we then say "*restricted product*" or "*restricted sum*" instead of "*direct sum*" (I, § 4, no. 9).

Note that $E$ is a *normal* subgroup of the product $F = \prod_{i \in I} E_i$ and that each of the $j_k(E_k)$ is a *normal* subgroup of $F$; moreover, for two distinct indices $\lambda, \mu$, every element of $j_\lambda(E_\lambda)$ is *permutable* with every element of $j_\mu(E_\mu)$. Proposition 6 extends to the general case with the hypothesis that, for two distinct indices $\lambda, \mu$, every element of $f_\lambda(E_\lambda)$ is *permutable* in $M$ with every element of $f_\mu(E_\mu)$ (I, § 4, no. 9, Proposition 12). The property of "*associativity*" of the restricted sum follows immediately from this. Proposition 7 and its Corollaries 1 and 2 hold without modification.

### 7. INTERSECTION AND SUM OF SUBMODULES

For every family $(M_i)_{i \in I}$ of submodules of an $A$-module $E$, the intersection $\bigcap_{i \in I} E_i$ is a submodule of $E$. If, for each $i \in I$, $\phi_i$ denotes the canonical homomorphism $E \to E/M_i$, $\bigcap_{i \in I} M_i$ is the *kernel* of the homomorphism $\phi : x \mapsto (\phi_i(x))$ of $E$ into $\prod_{i \in I} (E/M_i)$, in other words, there is an *exact sequence*

$$
0 \longrightarrow \bigcap_{i \in I} M_i \longrightarrow E \xrightarrow{\phi} \prod_{i \in I} (E/M_i).
$$

The linear mapping $\phi$ and the mapping
$$
E / \left( \bigcap_{i \in I} M_i \right) \to \prod_{i \in I} (E / M_i)
$$
which is obtained by passing to the quotient, are called canonical.

In particular:

#### Proposition 8 {#alg-ii-s1-prop-8 .statement}

*If a family* $(M_i)_{i \in I}$ *of submodules of* $E$ *has intersection reduced to* $0$ *E is canonically isomorphic to a submodule of* $\prod_{i \in I} (E / M_i)$.

Given a subset $X$ of an $A$-module $E$, the intersection $F$ of the submodules of $E$ containing $X$ is called the submodule *generated* by $X$ and $X$ is called a *generating set* (or *generating system*) of $F$ (I, § 4, no. 3); for a family $(a_i)_{i \in I}$ of elements of $E$, the submodule generated by the set of $a_i$ is called the submodule generated by the family $(a_i)$.

An $A$-module is called *finitely generated* if it has a *finite* generating set.

#### Proposition 9 {#alg-ii-s1-prop-9 .statement}

*The submodule generated by a family* $(a_i)_{i \in I}$ *of elements of an* $A$*-module* $E$ *is the set of linear combinations of the family* $(a_i)$.

Every submodule of $E$ which contains all the $a_i$ also contains the linear combinations of the $a_i$. Conversely, formulae (1) and (2) of no. 1 prove that the set of linear combinations of the $a_i$ is a submodule of $E$ which obviously contains all the $a_i$ and is therefore the smallest submodule containing them.

#### Corollary 1 {#alg-ii-s1-prop-9-cor-1 .statement}

*Let* $u : E \to F$ *be a linear mapping, S a subset of* $E$ *and* $M$ *the submodule of* $E$ *generated by* $S$. *Then* $u(M)$ *is the submodule of* $F$ *generated by* $u(S)$.

In particular, the image under $u$ of any finitely generated submodule of $E$ is a finitely generated submodule of $F$.

#### Remark {#alg-ii-s1-n7-rem-1 .statement}

If $u(x) = 0$ for all $x \in S$, then also $u(x) = 0$ for all $x \in M$. We shall sometimes refer to this result as the *"principle of extension of linear identities"* or *"principle of extension by linearity"*.

In particular, to verify that a linear mapping $u : E \to F$ is of the form $v \circ \phi$, where $v : E / M \to F$ is linear and $\phi : E \to E / M$ is the canonical projection, it suffices to verify that $u(S) = 0$.

#### Corollary 2 {#alg-ii-s1-prop-9-cor-2 .statement}

*The submodule generated by the union of a family* $(M_i)_{i \in I}$ *of submodules of a module* $E$ *is identical with the set of sums* $\sum_{i \in I} x_i$, *where* $(x_i)_{i \in I}$ *runs through the set of families of elements of* $E$ *of finite support such that* $x_i \in M_i$ *for all* $i \in I$.

Clearly every linear combination of elements of $\bigcup_{i \in I} M_i$ is of the above form; the converse is obvious.

The submodule of E generated by the union of a family $(M_i)_{i \in I}$ of submodules of E is called the *sum* of the family $(M_i)$ and is denoted by $\sum_{i \in I} M_i$.

If for all $i \in I$, $h_i$ is the canonical injection $M_i \to E$ and $h : (x_i) \mapsto \sum_i h_i(x_i)$ the linear mapping of $\bigoplus_{i \in I} M_i$ into E corresponding to the family $(h_i)$ (no. 6, Proposition 6), $\sum_{i \in I} M_i$ is the *image* of $h$; in other words, there is an *exact sequence*

$$
\bigoplus_{i \in I} M_i \xrightarrow{h} E \longrightarrow E / \left( \sum_{i \in I} M_i \right) \longrightarrow 0.
$$

#### Corollary 3 {#alg-ii-s1-prop-9-cor-3 .statement}

*If* $(M_\lambda)_{\lambda \in L}$ *is a right directed family of submodules of an A-module E, the sum* $\sum_{\lambda \in L} M_\lambda$ *is identical with the union* $\bigcup_{\lambda \in L} M_\lambda$.

$\bigcup_{\lambda \in L} M_\lambda \subset \sum_{\lambda \in L} M_\lambda$ *is always true without hypothesis; on the other hand, for every finite subfamily* $(M_\lambda)_{\lambda \in J}$ *of* $(M_\lambda)_{\lambda \in L}$, *there exists by hypothesis a* $\mu \in L$ *such that* $M_\lambda \subset M_\mu$ *for all* $\lambda \in J$, *hence* $\sum_{\lambda \in L} M_\lambda \subset M_\mu$ *and it thus follows from Corollary 2 that* $\sum_{\lambda \in L} M_\lambda \subset \bigcup_{\lambda \in L} M_\lambda$.

#### Corollary 4 {#alg-ii-s1-prop-9-cor-4 .statement}

*Let* $0 \to E \xrightarrow{f} F \xrightarrow{g} G \to 0$ *be an exact sequence of A-modules, S a generating system of* E, *T a generating system of* G. *If T' is a subset of F such that* $g(T') = T$, *T' \cup f(S) is a generating system of* F.

The submodule F' of F generated by T' \cup f(S) contains $f(E)$ and, as $g(F')$ contains T, $g(F') = G$; hence $F' = F$.

#### Corollary 5 {#alg-ii-s1-prop-9-cor-5 .statement}

*In an exact sequence* $0 \to E \to F \to G \to 0$ *of A-modules, if E and G are finitely generated, so is F.*

#### Proposition 10 {#alg-ii-s1-prop-10 .statement}

*Let* M, N *be two submodules of an A-module E. Then there are two exact sequences*

$$
\begin{align*}
&0 \longrightarrow M \cap N \xrightarrow{u} M \oplus N \xrightarrow{i-j} M + N \longrightarrow 0 \\
&0 \longrightarrow E/(M \cap N) \xrightarrow{v} (E/M) \oplus (E/N) \xrightarrow{p-q} E/(M + N) \longrightarrow 0
\end{align*}
$$

*where* $i : M \to M + N$, $j : N \to M + N$ *are the canonical injections,*
$$
p : E/M \to E/(M + N) \quad \text{and} \quad q : E/N \to E/(M + N)
$$

*the canonical surjections and where the homomorphisms u and v are defined as follow:*

if $f : M \cap N \to M \to M \oplus N$ and $g : M \cap N \to N \to M \oplus N$ are the canonical injections, $u = f + g$, and if $r : E/(M \cap N) \to E/M \to (E/M) \oplus (E/N)$ and
$$
s : E/(M \cap N) \to E/N \to (E/M) \oplus (E/N)
$$
are the canonical mappings, $v = r + s$.

We prove the exactness of (29): obviously $i - j$ is surjective and $u$ is injective. On the other hand, to say that $(i - j)(x, y) = 0$, where $x \in M$ and $y \in N$, means that $i(x) - j(y) = 0$, hence $i(x) = j(y) = z \in M \cap N$, whence by definition $x = f(z), y = g(z)$, which proves that $\operatorname{Ker}(i - j) = \operatorname{Im} u$.

We prove the exactness of (30): clearly $p - q$ is surjective. On the other hand, to say that $v(t) = 0$ for $t \in E/(M \cap N)$ means that $r(t) = s(t) = 0$, hence $t$ is the class mod. $(M \cap N)$ of an element $z \in E$ whose classes mod. $M$ and mod. $N$ are zero, which implies $z \in M \cap N$ and $t = 0$. Finally, to say that $(p - q)(x, y) = 0$, where $x \in E/M, y \in E/N$ means that $p(x) = q(y)$, or also that there exist two elements $z', z''$ of $E$ whose classes mod. $M$ and mod. $N$ are respectively $x$ and $y$ and which are such that $z' - z'' \in M + N$. Hence there are $t' \in M, t'' \in N$ such that $z' - z'' = t' - t''$, whence
$$
z' - t' = z'' - t'' = z.
$$
Let $w$ be the class mod. $(M \cap N)$ of $z; r(w)$ is the class mod. $M$ of $z$ and hence also that of $z'$, that is $x$; similarly $s(w) = y$, which completes the proof that $\operatorname{Ker}(p - q) = \operatorname{Im} v$.

### 8. DIRECT SUMS OF SUBMODULES

#### Definition 6 {#alg-ii-s1-def-6 .statement}

*An A-module* $E$ *is said to be the direct sum of a family* $(M_\iota)_{\iota \in I}$ *of submodules of* $E$ *if the canonical mapping* $\bigoplus_{\iota \in I} M_\iota \to E$ *(no. 6)* *is an isomorphism*.

It amounts to the same to say that every $x \in E$ can be written *in a unique way* in the form $x = \sum_{\iota \in I} x_\iota$, where $x_\iota \in E_\iota$ for all $\iota \in I$; the element $x_\iota$ thus corresponding to $x$ is called the *component* of $x$ in $E_\iota$; the mapping $x \mapsto x_\iota$ is *linear*.

#### Remark {#alg-ii-s1-n8-rem-1 .statement}

(1) Let $(M_\iota)_{\iota \in I}, (N_\iota)_{\iota \in I}$ be two families of submodules of a module $E$, with the same indexing set; suppose that $E$ is *both* the direct sum of the family $(M_\iota)$ and of the family $(N_\iota)$ and *that* $N_\iota \subset M_\iota$ for all $\iota \in I$. Then $N_\iota = M_\iota$ *for all* $\iota \in I$, as follows immediately from no. 6, Corollary 1 to Proposition 7 applied to the canonical injections $f_\iota : N_\iota \to M_\iota$.

#### Proposition 11 {#alg-ii-s1-prop-11 .statement}

*Let* $(M_\iota)_{\iota \in I}$ *be a family of submodules of an A-module* $E$. *The following properties are equivalent*:

(a) *The submodule* $\sum_{\iota \in I} M_\iota$ *is the direct sum of the family* $(M_\iota)_{\iota \in I}$.

(b) *The relation* $\sum_{i \in I} x_i = 0$, *where* $x_i \in M_i$ *for all* $i \in I$, *implies* $x_i = 0$ *for all* $i \in I$.

(c) *For all* $\kappa \in I$, *the intersection of* $M_\kappa$ *and* $\sum_{i \neq \kappa} M_i$ *reduces to* 0.

It is immediate that (a) and (b) are equivalent, since the relation $\sum_i x_i = \sum_i y_i$ is equivalent to $\sum_i (x_i - y_i) = 0$. On the other hand, by virtue of Definition 6, (a) implies (c) by the uniqueness of the expression of an element of $\bigoplus_{i \in I} M_i$ as a direct sum of elements $x_i \in M_i$. Finally, the relation $\sum_i x_i = 0$, where $x_i \in M_i$ for all $i$, can be written, for all $\kappa \in I$, $x_\kappa = \sum_{i \neq \kappa} (-x_i)$; condition (c) then implies $x_\kappa = 0$ for all $\kappa \in I$, hence (c) implies (b).

#### Definition 7 {#alg-ii-s1-def-7 .statement}

*An endomorphism e of an A-module E is called a projector if* $e \circ e = e$ *(in other words, if e is an idempotent in the ring End(E)). In* $\operatorname{End}(E)$ *a family* $(e_\lambda)_{\lambda \in L}$ *of projectors is called orthogonal if* $e_\lambda \circ e_\mu = 0$ *for* $\lambda \neq \mu$.

#### Proposition 12 {#alg-ii-s1-prop-12 .statement}

*Let E be an A-module.*

(i) *If E is the direct sum of a family* $(M_\lambda)_{\lambda \in L}$ *of submodules and, for all* $x \in E$, $e_\lambda(x)$ *is the component of x in* $M_\lambda$, $(e_\lambda)$ *is an orthogonal family of projectors such that* $x = \sum_{\lambda \in L} e_\lambda(x)$ *for all* $x \in E$.

(ii) *Conversely, if* $(e_\lambda)_{\lambda \in L}$ *is an orthogonal family of projectors in* $\operatorname{End}(E)$ *such that* $x = \sum_{\lambda \in L} e_\lambda(x)$ *for all* $x \in E$, *E is the direct sum of the family of submodules* $M_\lambda = e_\lambda(E)$.

Property (i) follows from the definitions and (ii) is a special case of no. 6, Corollary 2 to Proposition 6, applied to the canonical injections $M_\lambda \to E$ and the mappings $e_\lambda : E \to M_\lambda$.

Note that when L is finite the condition $x = \sum_{\lambda \in L} e_\lambda(x)$ for all $x \in E$ may also be written in $\operatorname{End}(E)$.

(31)
$$
1_E = \sum_{\lambda \in L} e_\lambda.
$$

#### Corollary {#alg-ii-s1-n8-cor-1 .statement}

*For every projector e of E, E is the direct sum of the image* $M = e(E)$ *and the kernel* $N = e^{-1}(0)$ *of e; for all* $x = x_1 + x_2 \in E$ *with* $x_1 \in M$ *and* $x_2 \in N$, $x_1 = e(x)$; *1 − e is a projector of E of image N and kernel M*.

$(1 - e)^2 = 1 - 2e + e^2 = 1 - e$ *in* $\operatorname{End}(E)$ *and hence* $1 - e$ *is a projector; as also* $e(1 - e) = (1 - e)e = e - e^2 = 0$, *E is the direct sum of the images* $M$ *and* $N$ *of e and* $1 - e$ *by Proposition 12. Finally, for all* $x \in E$, *the relation* $x \in M$ *is equivalent to* $x = e(x)$; *for* $x = e(x)$ *implies by definition* $x \in M$ *and, conversely, if* $x = e(x')$ *with* $x' \in E$, *then* $e(x) = e^2(x') = e(x') = x;$

this shows therefore that M is the kernel of $1 - e$ and, exchanging the roles of $e$ and $1 - e$, it is similarly seen that N is the kernel of $e$.

#### Remark {#alg-ii-s1-n8-rem-2 .statement}

(2) Let E, F be two A-modules such that E is the direct sum of a finite family $(M_i)_{1 \leq i \leq m}$ of submodules and F the direct sum of a finite family $(N_j)_{1 \leq j \leq n}$ of submodules. Then it is known (no. 6, Corollary 1 to Proposition 6) that $\mathrm{Hom}_A(E, F)$ is canonically identified with the product $\prod_{i,j} \mathrm{Hom}_A(M_i, N_j)$; to be precise, to a family $(u_{ji})$, where $u_{ji} \in \mathrm{Hom}_A(M_i, N_j)$ there corresponds the linear mapping $u : E \to F$ defined as follows. It suffices to define the restriction of $u$ to each of the $M_i$ and for each $x_i \in M_i$,
$$
u(x_i) = \sum_{j=1}^n u_{ji}(x_i).
$$
Now let G be a third A-module, the direct sum of a finite family $(P_k)_{1 \leq k \leq p}$ of submodules; let $v$ be a linear mapping of F into G and let $(v_{kj}) \in \prod_{j,k} \mathrm{Hom}_A(N_j, P_k)$ be the family corresponding to it canonically. For all $x_i \in M_i$,
$$
v(u(x_i)) = \sum_{j=1}^n v(u_{ji}(x_i)) = \sum_{k=1}^p \sum_{j=1}^n v_{kj}(u_{ji}(x_i)).
$$
Thus it is seen that if we write
$$
w_{ki} = \sum_{j=1}^n v_{kj} \circ u_{ji} \in \mathrm{Hom}_A(M_i, P_k)
$$
the family $(w_{ki})$ corresponds canonically to the composite linear mapping $w = v \circ u$ from E to G (cf. § 10, no. 5).

### 9. SUPPLEMENTARY SUBMODULES

#### Definition 8 {#alg-ii-s1-def-8 .statement}

In an A-module E, two submodules $M_1, M_2$ are said to be supplementary if E is the direct sum of $M_1$ and $M_2$.

Proposition 11 of no. 8 shows that, for $M_1$ and $M_2$ to be supplementary, it is necessary and sufficient that $M_1 + M_2 = E$ and $M_1 \cap M_2 = \{0\}$ (cf. I, § 4, no. 9, Proposition 15).

#### Proposition 13 {#alg-ii-s1-prop-13 .statement}

Let $M_1, M_2$ be two supplementary submodules in an A-module E. The restriction to $M_1$ of the canonical mapping $E \to E/M_2$ is an isomorphism of $M_1$ onto $E/M_2$.

This linear mapping is surjective since $M_1 + M_2 = E$ and it is injective since its kernel is the intersection of $M_1$ and the kernel $M_2$ of $E \to E/M_2$ and hence reduces to $\{0\}$.

#### Corollary {#alg-ii-s1-n9-cor-1 .statement}

If $M_2$ and $M_2'$ are two supplements of the same submodule $M_1$ of E, the set of ordered pairs $(x, x') \in M_2 \times M_2'$ such that $x - x' \in M_1$ is the graph of an isomorphism of $M_2$ onto $M_2'$.

It is immediate that it is the graph of the composite isomorphism $M_2 \to E/M_1 \to M'_2$.

#### Definition 9 {#alg-ii-s1-def-9 .statement}

*A submodule $M$ of an $A$-module $E$ is called a direct factor of $E$ if it has a supplementary submodule in $E$.*

When this is so, $E/M$ is isomorphic to a supplement of $M$ (Proposition 13).

A submodule does not necessarily admit a supplement (Exercise 11). When a submodule is a direct factor, it has in general several distinct supplements; these supplements are however canonically isomorphic to one another (Corollary to Proposition 13).

#### Proposition 14 {#alg-ii-s1-prop-14 .statement}

*For a submodule $M$ of a module $E$ to be a direct factor, it is necessary and sufficient that there exist a projector of $E$ whose image is $M$ or a projector of $E$ whose kernel is $M$.*

This follows immediately from no. 8, Proposition 12 and Corollary.

#### Proposition 15 {#alg-ii-s1-prop-15 .statement}

*Given an exact sequence of $A$-modules*
$$
(33)\quad 0 \longrightarrow E \xrightarrow{f} F \xrightarrow{g} G \longrightarrow 0
$$
*the following propositions are equivalent:*
(a) *The submodule $f(E)$ of $F$ is a direct factor.*
(b) *There exists a linear retraction $r : F \to E$ associated with $f$ (Set Theory, II, § 3, no. 8, Definition 11).*
(c) *There exists a linear section $s : G \to F$ associated with $g$ (Set Theory, II, § 3, no. 8, Definition 11).*
*When this is so, $f + s : E \oplus G \to F$ is an isomorphism.*

If there exists a projector $e$ in $\mathrm{End}(F)$ such that $e(F) = f(E)$, the homomorphism $f^{-1} \circ e : F \to E$ is a linear retraction associated with $f$; conversely, if there exists such a retraction $r$, it is immediate that $f \circ r$ is a projector in $F$ whose image is $f(E)$, hence (a) and (b) are equivalent (Proposition 14). If $f(E)$ admits a supplement $E'$ in $F$ and $j : E' \to F$ is the canonical injection, $g \circ j$ is an isomorphism of $E'$ onto $G$ and the inverse isomorphism, considered as a mapping of $G$ into $F$, is a linear section associated with $g$. Conversely, if such a section $s$ exists, $s \circ g$ is a projector in $F$ whose kernel is $f(E)$, hence (a) and (c) are equivalent (Proposition 14). Moreover $s$ is a bijection of $G$ onto $s(G)$ and as $s(G)$ is supplementary to $f(E)$, $f + s$ is an isomorphism.

Note that being given $r$ (resp. $s$) is equivalent to being given a supplement of $f(E)$ in $F$, namely the kernel of $r$ (resp. image of $s$).

When the exact sequence (33) satisfies the conditions of Proposition 15, it is said to *split* or $(F, f, g)$ is said to be a *trivial* extension of $G$ by $E$ (I, § 6, no. 1).

#### Corollary 1 {#alg-ii-s1-prop-15-cor-1 .statement}

Let $u : E \to F$ be a linear mapping. For there to exist a linear mapping $v : F \to E$ such that $u \circ v = 1_F$ (the case where $u$ is said to be right invertible and $v$ is said to be the right inverse of $u$), it is necessary and sufficient that $u$ be surjective and that its kernel be a direct factor in $E$. The submodule $\operatorname{Im}(v)$ of $E$ is then a supplement of $\operatorname{Ker}(u)$.

It is obviously necessary that $u$ be surjective; as $v$ is then a section associated with $u$, the conclusion follows from Proposition 15.

#### Corollary 2 {#alg-ii-s1-prop-15-cor-2 .statement}

Let $u : E \to F$ be a linear mapping. For there to exist a linear mapping $v : F \to E$ such that $v \circ u = 1_E$ (the case where $u$ is said to be left invertible and $v$ is said to be the left inverse of $u$), it is necessary and sufficient that $u$ be injective and that its image be a direct factor in $F$. The submodule $\operatorname{Ker}(v)$ of $F$ is then a supplement of $\operatorname{Im}(u)$.

It is obviously necessary that $u$ be injective; as $v$ is then a retraction associated with $u$, the conclusion also follows from Proposition 15.

#### Remark {#alg-ii-s1-n9-rem-1 .statement}

(1) Let $M, N$ be two supplementary submodules in an $A$-module $E$, $p, q$ the projectors of $E$ onto $M$ and $N$ respectively, corresponding to the decomposition of $E$ as a direct sum of $M$ and $N$. It is known (no. 6, Corollary 1 to Proposition 6) that, for every $A$-module $F$, the mapping $(u, v) \mapsto u \circ p + v \circ q$ is an isomorphism of
$$
\operatorname{Hom}_A(M, F) \oplus \operatorname{Hom}_A(N, F)
$$
onto $\operatorname{Hom}_A(E, F)$. The image of $\operatorname{Hom}_A(M, F)$ under this isomorphism is the set of linear mappings $w : E \to F$ such that $w(x) = 0$ for all $x \in N$.

(2) If $M, N$ are two submodules of $E$ such that $M \cap N$ is a direct factor of $M$ and $N$, then $M \cap N$ is also a direct factor of $M + N$: if $P$ (resp. $Q$) is a supplement of $M \cap N$ in $M$ (resp. $N$), $M + N$ is the direct sum of $M \cap N, P$ and $Q$, as is immediately verified.

### 10. MODULES OF FINITE LENGTH

Recall (I, § 4, no. 4, Definition 7) that an $A$-module $M$ is called simple if it is not reduced to 0 and it contains no submodule distinct from $M$ and $\{0\}$. An $A$-module $M$ is said to be of finite length if it has a Jordan-Hölder series $(M_i)_{0 \leq i \leq n}$ and the number $n$ of quotients of this series (which does not depend on the Jordan-Hölder series of $M$ considered) is then called the length of $M$ (I, § 4, no. 7, Definition 11); we shall denote it by $\operatorname{long}(M)$ or $\operatorname{long}_A(M)$. An $A$-module which is reduced to 0 is of length 0; if $M$ is a non-zero $A$-module of finite length then $\operatorname{long}(M) > 0$.

#### Proposition 16 {#alg-ii-s1-prop-16 .statement}

Let $M$ be an $A$-module and $N$ a submodule of $M$; for $M$ to be of finite length, it is necessary and sufficient that $N$ and $M/N$ be so, and then
$$
\operatorname{long}(N) + \operatorname{long}(M/N) = \operatorname{long}(M).
$$
The proof has been given in I, § 4, no. 7, Proposition 10.

#### Corollary 1 {#alg-ii-s1-prop-16-cor-1 .statement}

Let $M$ be an $A$-module of finite length; for a submodule $N$ of $M$ to be equal to $M$, it is necessary and sufficient that $\operatorname{long}(N) = \operatorname{long}(M)$.

#### Corollary 2 {#alg-ii-s1-prop-16-cor-2 .statement}

Let $u : M \to N$ be an $A$-module homomorphism. If $M$ or $N$ is of finite length, so is $\operatorname{Im}(u)$. If $M$ is of finite length, so is $\operatorname{Ker}(u)$ and
$$
\operatorname{long}(\operatorname{Im}(u)) + \operatorname{long}(\operatorname{Ker}(u)) = \operatorname{long}(M).
$$
If $N$ is of finite length, so is $\operatorname{Coker}(u)$ and
$$
\operatorname{long}(\operatorname{Im}(u)) + \operatorname{long}(\operatorname{Coker}(u)) = \operatorname{long}(N).
$$

#### Corollary 3 {#alg-ii-s1-prop-16-cor-3 .statement}

Let $(M_i)_{0 \leq i \leq n}$ be a finite family of $A$-modules of finite length. If there exists an exact sequence of linear mappings
$$
0 \longrightarrow M_0 \xrightarrow{u_0} M_1 \xrightarrow{u_1} M_2 \longrightarrow \cdots \longrightarrow M_{n-1} \xrightarrow{u_{n-1}} M_n \longrightarrow 0
$$
then
$$
\sum_{k=0}^n (-1)^k \operatorname{long}(M_k) = 0.
$$
The corollary is obvious for $n = 1$ and is just Proposition 16 for $n = 2$; we argue by induction on $n$. If $M'_{n-1} = \operatorname{Im}(u_{n-2})$, then, by the induction hypothesis,
$$
\sum_{k=0}^{n-2} (-1)^k \operatorname{long}(M_k) + (-1)^{n-1} \operatorname{long}(M'_{n-1}) = 0.
$$
On the other hand, the exact sequence $0 \to M'_{n-1} \to M_{n-1} \to M_n \to 0$ gives
$$
\operatorname{long}(M'_{n-1}) + \operatorname{long}(M_n) = \operatorname{long}(M_{n-1}),
$$
whence relation (38).

#### Corollary 4 {#alg-ii-s1-prop-16-cor-4 .statement}

Let $M$ and $N$ be two submodules of finite length of an $A$-module $E$; then $M + N$ is of finite length and
$$
\operatorname{long}(M + N) + \operatorname{long}(M \cap N) = \operatorname{long}(M) + \operatorname{long}(N).
$$
It suffices to apply Corollary 3 to the exact sequence (29) (no. 7).
$$
0 \to M \cap N \to M \oplus N \to M + N \to 0
$$
using the fact that $\operatorname{long}(M \oplus N) = \operatorname{long}(M) + \operatorname{long}(N)$ by (34).

#### Corollary 5 {#alg-ii-s1-prop-16-cor-5 .statement}

Let $M$ be an $A$-module the sum of a family $(N_i)$ of submodules of finite length. Then $M$ is of finite length and
$$
\operatorname{long}(M) \leq \sum_i \operatorname{long}(N_i).
$$

Moreover, for the two sides of (40) to be equal, it is necessary and sufficient that M be the direct sum of the $N_i$.

It has been seen (no. 7, formula (28)) that there is a canonical surjective linear mapping $h : \bigoplus_i N_i \to M$; hence the corollary follows from (35).

#### Corollary 6 {#alg-ii-s1-prop-16-cor-6 .statement}

*Let M and N be two submodules of an A-module E such that E/M and E/N are modules of finite length; then E/(M \cap N) is of finite length and*

$$
\text{(41)} \quad \text{long}(E/(M \cap N)) + \text{long}(E/(M + N)) = \text{long}(E/M) + \text{long}(E/N).
$$

It suffices to apply Corollary 3 to the exact sequence (30)

$$
0 \to E/(M \cap N) \to (E/M) \oplus (E/N) \to E/(M + N) \to 0
$$

using the fact that

$$
\text{long}((E/M) \oplus (E/N)) = \text{long}(E/M) + \text{long}(E/N).
$$

#### Corollary 7 {#alg-ii-s1-prop-16-cor-7 .statement}

*Let $(M_i)$ be a finite family of submodules of an A-module E such that the $E/M_i$ are modules of finite length. Then $E/(\bigcap_i M_i)$ is of finite length and*

$$
\text{(42)} \quad \text{long}\left(E/(\bigcap_i M_i)\right) \leq \sum_i \text{long}(E/M_i).
$$

It has been seen (formula (27)) that there is a canonical injective linear mapping $E/(\bigcap_i M_i) \to \bigoplus_i (E/M_i)$.

#### Remark {#alg-ii-s1-n10-rem-1 .statement}

With the exception of no. 7, Proposition 9, *all* the results of nos. 2 to 10 are valid for arbitrary *commutative groups with operators*, submodules (resp. quotient modules) being replaced in the statements by stable subgroups (resp. quotient groups by stable subgroups); we also make the convention of calling homomorphisms of groups with operators "linear mappings". The corollaries to no. 7, Proposition 9 are also valid for commutative groups with operators: this is obvious for Corollaries 4 and 5, as also for Corollary 2, since $\alpha \left( \sum_{i \in I} x_i \right) = \sum_{i \in I} \alpha x_i$ for every operator $\alpha$, and Corollary 3 follows from it. As for Corollary 1, it suffices to note that if N is a stable subgroup of F containing $u(S)$, $u^{-1}(N)$ is a stable subgroup of E containing S, hence $u^{-1}(N)$ contains M and therefore $u(M) \subset N$.

### 11. FREE FAMILIES. BASES

Let A be a ring, T a set and consider the A-module $A_s^{(T)}$. By definition, it is the external direct sum of a family $(M_t)_{t \in T}$ of A-modules all equal to $A_s$ and for all $t \in T$ there is a canonical injection $j_t : A_s \to A_s^{(T)}$ (no. 6). We write j_t(1) = e_t so that $e_t = (\delta_{tt'})_{t' \in T}$, where $\delta_{tt'}$ is equal to 0 if $t' \neq t$, to 1 if $t' = t$ ("Kronecker symbol"; $(t, t') \mapsto \delta_{tt'}$ is just the characteristic function of the diagonal of $T \times T$); every $x = (\xi_t)_{t \in T} \in A_s^{(T)}$ may then be written uniquely:
$$
x = \sum_{t \in T} \xi_t e_t.
$$
The mapping $\phi : t \mapsto e_t$ of $T$ into $A_s^{(T)}$ is called canonical; it is injective if $A$ is non-zero. We shall see that the ordered pair $(A_s^{(T)}, \phi)$ is a solution of a universal mapping problem (Set Theory, IV, § 3, no. 1).

#### Proposition 17 {#alg-ii-s1-prop-17 .statement}

*For every A-module E and every mapping $f : T \to E$, there exists one and only one A-linear mapping $g : A_s^{(T)} \to E$ such that $f = g \circ \phi$.*

The condition $f = g \circ \phi$ means that $g(e_t) = f(t)$ for all $t \in T$, which is equivalent to $g(\xi e_t) = \xi f(t)$ for all $\xi \in A$ and all $t \in T$ and also means that $g \circ j_t$ is the linear mapping $\xi \mapsto \xi f(t)$ of $A_s$ into $E$ for all $t \in T$; the proposition is therefore a special case of no. 6, Proposition 6.

The linear mapping $g$ is said to be *determined* by the family $(f(t))_{t \in T}$ of elements of $E$; by definition
$$
g\left( \sum_{t \in T} \xi_t e_t \right) = \sum_{t \in T} \xi_t f(t).
$$

The kernel $R$ of $g$ is the set of $(\xi_t) \in A_s^{(T)}$ such that $\sum_t \xi_t f(t) = 0$; it is sometimes said that the module $R$ is *the module of linear relations between the elements of the family* $(f(t))_{t \in T}$. The exact sequence
$$
0 \longrightarrow R \longrightarrow A_s^{(T)} \overset{g}{\longrightarrow} E
$$
is said to be *determined* by the family $(f(t))_{t \in T}$.

#### Corollary 1 {#alg-ii-s1-prop-17-cor-1 .statement}

*Let $T, T'$ be two sets, $g : T \to T'$ a mapping. Then there exists one and only one A-linear mapping $f : A^{(T)} \to A^{(T')}$ which renders commutative the diagram*
$$
\begin{array}{ccc}
T & \overset{g}{\longrightarrow} & T' \\
\downarrow \phi & & \downarrow \phi' \\
A^{(T)} & \overset{f}{\longrightarrow} & A^{(T')}
\end{array}
$$
*where $\phi$ and $\phi'$ are the canonical mappings.*

It suffices to apply Proposition 17 to the composite mapping $T \overset{g}{\to} T' \overset{\phi'}{\to} A^{(T')}$.

#### Corollary 2 {#alg-ii-s1-prop-17-cor-2 .statement}

*For a family $(a_t)_{t \in T}$ of elements of an A-module E to be a generating system of E, it is necessary and sufficient that the linear mapping $A_s^{(T)} \to E$ determined by this family be surjective.*

This is just another way of expressing Proposition 9 of no. 7.

#### Definition 10 {#alg-ii-s1-def-10 .statement}

*A family* $(a_t)_{t \in T}$ *of elements of an* $\mathbf{A}$*-module* $E$ *is called a free family* (resp. *a basis of* $E$) *if the linear mapping* $A_s^{(T)} \to E$ *determined by this family is injective* (resp. *bijective*). *A module is called free if it has a basis*.

In particular, a commutative group $G$ is called *free* if $G$ (written additively) is a *free* $\mathbf{Z}$*-module* (cf. I, § 7, no. 7).

Definition 10, together with Corollary 2 to Proposition 17, show that a basis of an $\mathbf{A}$-module $E$ is a *free generating family* of $E$. Every free family of elements of $E$ is thus a basis of the submodule it generates.

By definition, the $\mathbf{A}$-module $A_s^{(T)}$ is free and the family $(e_t)_{t \in T}$ is a basis (called *canonical*) of this $\mathbf{A}$-module. When $\mathbf{A} \neq \{0\}$, $T$ is often identified with the set of $e_t$ by the canonical bijection $t \mapsto e_t$; this amounts to writing $\sum_{t \in T} \xi_t \cdot t$ instead of $\sum_{t \in T} \xi_t a_t$ for the elements of $A_s^{(T)}$. When this convention is adopted, the elements of $A_s^{(T)}$ are called *formal linear combinations* (with coefficients in $\mathbf{A}$) *of the elements of* $T$.

Definition 10 and Proposition 17 give immediately the following result:

#### Corollary 3 {#alg-ii-s1-def-10-cor-3 .statement}

*Let* $E$ *be a free* $\mathbf{A}$*-module*, $(a_t)_{t \in T}$ *a basis of* $E$, $F$ *an* $\mathbf{A}$*-module and* $(b_t)_{t \in T}$ *a family of elements of* $F$. *There exists one and only one linear mapping* $f : E \to F$ *such that*
$$
f(a_t) = b_t \quad \text{for all } t \in T.
$$
*For* $f$ *to be injective* (resp. *surjective*), *it is necessary and sufficient that* $(b_t)$ *be a free family in* $F$ (resp. *a generating system of* $F$).

When a family $(a_t)_{t \in T}$ is not free, it is called *related*. Definition 10 may also be expressed as follows: to say that the family $(a_t)_{t \in T}$ is *free* means that the relation $\sum_{t \in T} \lambda_t a_t = 0$ (where the family $(\lambda_t)$ is of finite support) implies $\lambda_t = 0$ for all $t \in T$; to say that $(a_t)_{t \in T}$ is a *basis* of $E$ means that every $x \in E$ can be written in one and only one way in the form $x = \sum_{t \in T} \xi_t a_t$; for all $t \in T$, $\xi_t$ is then called the *component* (or *coordinate*) *of* $x$ *of index* $t$ *with respect to the basis* $(a_t)$; the mapping $x \to \xi_t$ from $E$ to $A_s$ is *linear*.

Suppose $\mathbf{A} \neq \{0\}$; then, in an $\mathbf{A}$-module $E$, two elements of a free family $(a_t)_{t \in T}$ whose indices are distinct are themselves *distinct*: for if $a_{t'} = a_{t''}$ for $t' \neq t''$, then $\sum_{t \in T} \lambda_t a_t = 0$ with $\lambda_{t'} = 1$, $\lambda_{t''} = -1$ and $\lambda_t = 0$ for the elements of $T$ distinct from $t'$ and $t''$. A subset $S$ of $E$ will be called a *free subset* (resp. a *basis* of $E$) if the family defined by the identity mapping of $S$ onto itself is free (resp. a basis of $E$); every family defined by a bijective mapping of an indexing set onto $S$ is then free (resp. a basis). The elements of a free subset of $E$ are also called *linearly independent*.

If a subset of E is not free, it is called related or a related system and its elements are said to be linearly dependent.

Every subset of a free subset is free; in particular, the empty subset is free and is a basis of the submodule {0} of E.

#### Proposition 18 {#alg-ii-s1-prop-18 .statement}

*For a family $(a_t)_{t \in T}$ of a module E to be free, it is necessary and sufficient that every finite subfamily of $(a_t)_{t \in T}$ be free.*

This follows immediately from the definition.

Proposition 18 shows that the set of free subsets of E, ordered by inclusion, is inductive (*Set Theory*, III, § 2, no. 4); as it is non-empty (since $\varnothing$ belongs to it), it has a maximal element $(a_l)_{l \in I}$ by Zorn’s Lemma. It follows (if $A \neq \{0\}$) that for all $x \in E$ there exist an element $\mu \neq 0$ of A and a family $(\xi_l)$ of element A such that $\mu x = \sum_l \xi_l a_l$ (cf. § 7, no. 1).

#### Proposition 19 {#alg-ii-s1-prop-19 .statement}

*Let E be an A-module, the direct sum of a family $(M_\lambda)_{\lambda \in L}$ of submodules. If, for each $\lambda \in L$, $S_\lambda$ is a free subset (resp. generating set, basis) of $M_\lambda$, then $S = \bigcup_{\lambda \in L} S_\lambda$ is a free subset (resp. generating set, basis) of E.*

The proposition follows from the definitions and the relation $A_s^{(S)} = \bigoplus_{\lambda \in L} A_s^{(S_\lambda)}$ (associativity of direct sums, cf. no. 6).

#### Remark {#alg-ii-s1-n11-rem-1 .statement}

(1) By Definition 10, if $A \neq \{0\}$ and $(a_l)_{l \in I}$ is a free family, no element $a_\kappa$ can be equal to a linear combination of the $a_l$ of index $l \neq \kappa$. But conversely, a family $(a_l)$ satisfying this condition is not necessarily a free family. For example, let A be an integral domain and $a, b$ two distinct non-zero elements; in A, considered as an A-module, $a$ and $b$ form a related system, since $(-b)a + ab = 0$. But in general there does not exist an element $x \in A$ such that $a = xb$ of $b = xa$ (cf. however § 7, no. 1, *Remark*).

An element $x$ of a module E is called *free* if $\{x\}$ is a free subset, that is if the relation $\alpha x = 0$ implies $\alpha = 0$. Every element of a free subset is free and in particular 0 cannot belong to any free subset when $A \neq \{0\}$.

#### Remark {#alg-ii-s1-n11-rem-2 .statement}

(2) A free module can have elements $\neq 0$ which are not free: for example, the A-module $A_s$ is free but the right divisors of zero in A are not free elements of $A_s$.

(3) In the additive group $\mathbf{Z}/(n)$ ($n$ an integer $\geq 2$) considered as a $\mathbf{Z}$-module, no element is free and *a fortiori* $\mathbf{Z}/(n)$ is not a free module.

(4) It can happen that every element $\neq 0$ of an A-module is free without the module being free. For example, the field $\mathbf{Q}$ of rational numbers is a $\mathbf{Z}$-module with this property, for two elements $\neq 0$ of $\mathbf{Q}$ always form a related system and a basis of $\mathbf{Q}$ could therefore only contain a single element $a$; but the elements of $\mathbf{Q}$ are not all of the form $na$ with $n \in \mathbf{Z}$ (cf. VII, § 3).

#### Proposition 20 {#alg-ii-s1-prop-20 .statement}

*Every A-module E is isomorphic to a quotient module of a free A-module.*

If T is a generating set of E, there exists a surjective linear mapping $A_s^{(T)} \to E$ (Corollary 2 to Proposition 17), and if R is the kernel of this mapping, E is isomorphic to $A_s^{(T)}/R$.

In particular we may take $T = E$; then there is a surjective linear mapping $A_s^{(E)} \to E$, called *canonical*.

In particular, to say that an A-module E is *finitely generated* (no. 7) means that it is isomorphic to a quotient of a free A-module with a *finite basis* or also that there exists an exact sequence of the form

$$
A_s^n \to E \to 0 \quad (n \text{ an integer } > 0).
$$

Note that if $A \neq \{0\}$ every basis of a *finitely generated* free module E is necessarily *finite*, for if S is a finite generating system and B a basis of E, each element of S is a linear combination of a finite number of elements of B and if B' is the set of all the elements of B which figure thus in the expression for the elements of S, B' is finite and every $x \in E$ is a linear combination of elements of B', hence $B' = B$.

#### Proposition 21 {#alg-ii-s1-prop-21 .statement}

*Every exact sequence of A-modules*

$$
0 \longrightarrow G \xrightarrow{g} E \xrightarrow{f} F \longrightarrow 0
$$

*in which F is a free A-module, splits* (no. 9). *To be precise, if* $(b_\lambda)_{\lambda \in L}$ *is a basis of F and, for each* $\lambda \in L$, $a_\lambda$ *is an element of E such that* $f(a_\lambda) = b_\lambda$, *the family* $(a_\lambda)_{\lambda \in L}$ *is free and generates a supplementary submodule to g(G)*.

There exists one and only one linear mapping $h : F \to E$ such that $h(b_\lambda) = a_\lambda$ for all $\lambda \in L$ (Corollary 3 to Proposition 17). As h is a linear section associated with f, the proposition follows from I, § 4, no. 9, Proposition 15.

#### Remark {#alg-ii-s1-n11-rem-3 .statement}

(5) Let $(a_i)_{1 \leq i \leq n}$ be a *basis* of an A-module E and let $(b_i)_{1 \leq i \leq n}$ be a family of elements of E given by the relations

$$
b_i = \lambda_{1i} a_1 + \cdots + \lambda_{ii} a_i \quad (1 \leq i \leq n)
$$

where $\lambda_{ii}$ is *invertible* in A; then $(b_i)_{1 \leq i \leq n}$ is a *basis* of E. It suffices to argue by induction on $n$, the proposition being obvious for $n = 1$. If E' is the submodule of E generated by the family $(a_i)_{1 \leq i \leq n-1}$, it follows from the induction hypothesis that $(b_i)_{1 \leq i \leq n-1}$ is a basis of E'; on the other hand, it follows from (46) that if $\mu b_n \in E'$ with $\mu \in A$, then also $\mu \lambda_{nn} a_n \in E'$, whence $\mu = 0$ since $\lambda_{nn}$ is invertible. The family $(b_i)_{1 \leq i \leq n}$ is thus free and, as
$$
a_n = -\lambda_{nn}^{-1}\lambda_{1n}a_1 - \cdots - \lambda_{nn}^{-1}\lambda_{n-1,n}a_{n-1} + \lambda_{nn}^{-1}b_n
$$
it is seen that $(b_i)_{1 \leq i \leq n}$ is a generating system of E, which completes the proof. This result is easily generalized to a family $(a_i)_{i \in I}$ whose indexing set I is well ordered.

### 12. ANNIHILATORS. FAITHFUL MODULES. MONOGENOUS MODULES

#### Definition 11 {#alg-ii-s1-def-11 .statement}

*The annihilator of a subset S of an A-module E is the set of elements $\alpha \in A$ such that $\alpha x = 0$ for all $x \in S$.*

The annihilator of S is usually denoted by Ann(S); for a subset S consisting of a single element x, we write Ann(x) instead of Ann(\{x\}) and call Ann(x) *the annihilator of x*.

The relation $\alpha x = 0$ may also be expressed by saying that *x is annihilated by $\alpha$*.

It is immediate that the annihilator of an arbitrary subset S of E is a *left ideal* of A; for it to be equal to A, it is necessary and sufficient (by virtue of (M_IV)) that $S = \{0\}$. If two subsets S, T of E are such that $S \subset T$, the annihilator of T is contained in the annihilator of S. If $(S_i)_{i \in I}$ is an arbitrary family of subsets of E, the annihilator of the union $\bigcup_i S_i$ is the intersection of the annihilators of the $S_i$. In particular, the annihilator of a subset S of E is the intersection of the annihilators of the elements of S. To say that an element of E is *free* is equivalent to saying that its annihilator is $\{0\}$. For all $x \in E$ and all $\alpha \in A$, the annihilator of $\alpha x$ is the set of $\beta \in A$ such that $\beta \alpha \in \mathrm{Ann}(x)$.

The annihilator of a *submodule* M of E is a *two-sided ideal* of A; for, if $\alpha x = 0$ for all $x \in M$, then also $\alpha (\beta x) = 0$ for all $x \in M$ and all $\beta \in A$, hence $\alpha \beta$ belongs to the annihilator of M for all $\beta \in A$. In particular, the annihilator of E is a two-sided ideal of A.

For all $\alpha \in A$, let $h_\alpha$ be the homothety $x \mapsto \alpha x$; it is known that the mapping $\alpha \mapsto h_\alpha$ of A into the endomorphism ring $\mathcal{E} = \mathrm{Hom}_\mathbf{Z}(E, E)$ of the commutative group (without operators) E, is a *ring homomorphism* (§ 2, no. 5). The inverse image of 0 under this homomorphism is the *annihilator* $a$ of E; the image of A under the homomorphism $\alpha \mapsto h_\alpha$ is therefore isomorphic to the quotient ring $A/a$. The module E is called *faithful* if its annihilator $a$ reduces to 0.

Let E be any A-module, $a$ a two-sided ideal of A contained in Ann(E) and let $\dot{\alpha}$ be an element of the quotient ring $A/a$; for all $x \in E$, the element $\alpha x$ is the same for all the $\alpha \in A$ belonging to the class $\dot{\alpha}$ mod. $a$; if this element is denoted by $\dot{\alpha} x$, it is immediately seen that the mapping (α, x) ↦ αx defines (with addition on E) an (A/α)-module structure on E. When α = Ann(E), the (A/α)-module E thus defined is *faithful*; we shall say that it is the faithful module *associated* with the A-module E. Observe that every submodule of an A-module E is also a submodule of the associated faithful module and conversely.

#### Definition 12 {#alg-ii-s1-def-12 .statement}

*A module is called monogenous if it is generated by a single element.*

Proposition 9 of no. 7 shows that, if E is a monogenous A-module and a is an element generating E, E is identical with the set A.a of ξa, where ξ runs through A.

#### Example {#alg-ii-s1-n12-exa-1 .statement}

(1) Every monogenous group, being commutative (I, § 4, no. 10, Proposition 18), is a monogenous $\mathbf{Z}$-module.
(2) If A is a commutative ring, the monogenous submodules of the A-module A are just the *principal ideals* (I, § 8, no. 6) of the ring A.
(3) Every *simple* A-module E is monogenous, since the submodule of E generated by an element ≠ 0 of E is necessarily equal to E.

#### Proposition 22 {#alg-ii-s1-prop-22 .statement}

*Let A be a ring. Every quotient module of $A_s$ is monogenous. Conversely, let E be a monogenous A-module, c a generator of E and a its annihilator; the linear mapping $\xi \mapsto \xi c$ defines, when passing to the quotient, an isomorphism of $A_s/a$ onto E.*

As $A_s$ is itself monogenous, being generated by 1, the first assertion follows from no. 7, Corollary 1 to Proposition 9. The second is obvious, since $\xi \mapsto \xi c$ is by hypothesis surjective and has kernel a.

Note that, if A is not commutative, the annihilators of two distinct generators c, c' of a monogenous A-module E are in general *distinct* and are also distinct from the annihilator of the module E. On the other hand, if A is *commutative*, the annihilator of a generator c of E is contained in the annihilator of every element of E and hence is the annihilator of the whole of E.

#### Corollary {#alg-ii-s1-n12-cor-1 .statement}

*Every submodule of a monogenous A-module E is isomorphic to a quotient module b/a where a and b are two left-ideals of A such that a ⊂ b. Every quotient module of a monogenous A-module is monogenous.*

The second assertion is immediate and the first follows from Proposition 22 and I, § 4, no. 6, Theorem 4.

Note on the other hand that a submodule of a monogenous module is not necessarily monogenous. For example, if A is a commutative ring in which there exist non-principal ideals (VII, § 1, no. 1), these ideals are non-monogenous submodules of the monogenous A-module A.

It follows from the definitions that a submodule of an A-module E generated by a family $(a_i)$ of elements of E is the *sum* of the monogenous submodules

Aa_i of E; for (a_i) to be a basis of E, it is necessary and sufficient that each of the a_i be a free element of E and that the sum of the Aa_i be direct.

#### Proposition 23 {#alg-ii-s1-prop-23 .statement}

Let E be an A-module, the direct sum of an infinite family (M_i)_{i \in I} of non-zero submodules. For every generating system S of E, Card(S) \geq Card(I).

For all x \in S, let C_x be the finite set of indices i \in I such that the component of x in M_i is \neq 0 and let C = \bigcup_{x \in S} C_x. Every x \in S belongs by definition to the submodule of E the direct sum of the M_i for i \in C and the hypothesis that S generates E implies therefore that C = I; as I is by hypothesis infinite, so is S (Set Theory, III, § 5, no. 1, Corollary 1 to Proposition 1); therefore Card(I) = Card(C) \leq Card(S) (Set Theory, III, § 6, no. 3, Corollary 3 to Theorem 2).

#### Corollary 1 {#alg-ii-s1-prop-23-cor-1 .statement}

Under the hypotheses of Proposition 23, suppose that each M_i is monogenous and that E is the direct sum of a second family (N_\lambda)_{\lambda \in L} of non-zero monogenous submodules. Then Card(L) = Card(I).

If b_\lambda is a generator of N_\lambda, the set of b_\lambda is a generating system of E, hence Card(L) \geq Card(I). In particular L is infinite and, exchanging the roles of (M_i) and (N_\lambda), similarly Card(I) \geq Card(L), whence the corollary.

#### Corollary 2 {#alg-ii-s1-prop-23-cor-2 .statement}

If a module E admits an infinite basis B, every generating system of E has cardinal \geq Card(B) and every basis of E is equipotent to B.

### 13. CHANGE OF RING OF SCALARS

Let A, B be two rings and \rho a homomorphism of the ring B into the ring A. For every A-module E, the external law (\beta, x) \mapsto \rho(\beta)x defines (with addition) a B-module structure said to be associated with \rho and the A-module structure on E; this B-module is denoted by \rho_*(E) or E_{[B]} (and even simply E if no confusion can arise). In particular, if B is a subring of A and \rho : B \to A is the canonical injection, E_{[B]} is called the B-module obtained by restricting the ring of scalars A to B; by an abuse of language, this expression is also used when the homomorphism \rho is arbitrary.

If F is a submodule of the A-module E, \rho_*(F) is a submodule of \rho_*(E) and \rho_*(E/F) is equal to \rho_*(E)/\rho_*(F).

Let E, F be two A-modules; every A-linear mapping u : E \to F is also a B-linear mapping E_{[B]} \to F_{[B]} denoted by \rho_*(u); in other words, there is a canonical injection of \mathbf{Z}-modules

(47)
$$
\operatorname{Hom}_A(E, F) \to \operatorname{Hom}_B(E_{[B]}, F_{[B]}).
$$

This mapping is not necessarily bijective; in other words a B-linear mapping E_{[B]} \to F_{[B]} is not necessarily A-linear. For example, a sub-B-module of E_{[B]} is not necessarily a sub-A-module of E: if A is a field and B a subfield of $A$, the vector subspace $B_s$ of the vector $B$-space $(A_s)_{[B]}$ is not a vector sub-$A$-space if $B \neq A$.

It is immediate that, for every family $(E_i)_{i \in I}$ of $A$-modules, the $B$-module $\rho_*\left(\prod_{i \in I} E_i\right)$ (resp. $\rho_*\left(\bigoplus_{i \in I} E_i\right)$) is equal to $\prod_{i \in I} \rho_*(E_i)$ (resp. $\bigoplus_{i \in I} \rho_*(E_i)$).

Every generating system of $\rho_*(E)$ is a generating system of $E$ but the converse is not necessarily true.

#### Proposition 24 {#alg-ii-s1-prop-24 .statement}

*Let $A, B$ be two rings and $\rho : B \to A$ a ring homomorphism.*

(i) *If $\rho$ is surjective, the canonical mapping (47) is bijective. For every $A$-module $E$, every sub-$B$-module of $\rho_*(E)$ is a sub-$A$-module of $E$; every generating system of $E$ is a generating system of $\rho_*(E)$.*

(ii) *If $\rho$ is injective, every free family in the $A$-module $E$ is a free family in the $B$-module $\rho_*(E)$.*

The proposition follows immediately from the definitions.

Note that even if $\rho$ is injective, a free family in $\rho_*(E)$ is not necessarily free in $E$.

*For example, 1 and $\sqrt{2}$ do not form a free system in $\mathbf{R}$ considered as a vector $\mathbf{R}$-space, although they form a free system in $\mathbf{R}$ considered as a vector $\mathbf{Q}$-space (cf. Remark 1).*

#### Proposition 25 {#alg-ii-s1-prop-25 .statement}

*Let $A, B$ be two rings, $\rho : B \to A$ a ring homomorphism and $E$ an $A$-module. Let $(\alpha_\lambda)_{\lambda \in L}$ be a generating system (resp. free family of elements, basis) of $A$ considered as a left $B$-module. Let $(a_\mu)_{\mu \in M}$ be a generating system (resp. free family of elements, basis) of the $A$-module $E$. Then $(\alpha_\lambda a_\mu)_{(\lambda, \mu) \in L \times M}$ is a generating system (resp. (when $\rho$ is injective) free family of elements, basis) of the $B$-module $\rho_*(E)$.*

If $x = \sum_{\mu \in M} \gamma_\mu a_\mu$, where $\gamma_\mu \in A$ and $(\alpha_\lambda)$ is a generating system of $A$, we may write $\gamma_\mu = \sum_{\lambda \in L} \rho(\beta_{\lambda \mu}) \alpha_\lambda$, with $\beta_{\lambda \mu} \in B$, for all $\mu \in M$, whence $x = \sum_{\lambda, \mu} \rho(\beta_{\lambda \mu}) \alpha_\lambda a_\mu$. On the other hand, if $(\alpha_\lambda)$ and $(a_\mu)$ are free families, a relation $\sum_{\lambda, \mu} \rho(\beta_{\lambda \mu}) \alpha_\lambda a_\mu = 0$, with $\beta_{\lambda \mu} \in B$, may be written $\sum_{\mu \in M} \left( \sum_{\lambda \in L} \rho(\beta_{\lambda \mu}) \alpha_\lambda \right) a_\mu = 0$; it thus implies $\sum_{\lambda \in L} \rho(\beta_{\lambda \mu}) \alpha_\lambda = 0$ for all $\mu \in M$ and therefore $\beta_{\lambda \mu} = 0$ for all $\lambda, \mu$ if $\rho$ is injective.

#### Corollary {#alg-ii-s1-n13-cor-1 .statement}

*If $A$ is a finitely generated left $B$-module and $E$ a finitely generated left $A$-module, $\rho_*(E)$ is a finitely generated left $A$-module.*

Let $C$ be a third ring, $\rho' : C \to B$ a ring homomorphism and $\rho'' = \rho \circ \rho'$ the composite homomorphism. It follows immediately from the definitions that $\rho''_*(E) = \rho'_*(\rho_*(E))$ for every $A$-module $E$. In particular, if $\rho$ is an *isomorphism* of $B$ onto $A$, then $E = \rho'_*(\rho_*(E))$, where $\rho'$ denotes the inverse isomorphism of $\rho$.

#### Remark {#alg-ii-s1-n13-rem-1 .statement}

(1) Let $K$ be a field and $A$ a subring of $K$ with the following property: for every finite family $(\xi_i)_{1 \leq i \leq n}$ of elements of $K$, there exists a $\gamma \in A$ which is non-zero and such that $\gamma \xi_i \in A$ for $1 \leq i \leq n$ (a hypothesis which is always satisfied when $A$ is *commutative* and $K$ is the field of fractions of $A$). Let $E$ be a vector space over $K$ and $E_{[A]}$ the $A$-module obtained by restricting the ring of scalars to $A$. Then, if a family $(x_\lambda)_{\lambda \in L}$ is *free in* $E_{[A]}$ it is also *free in* $E$. Attention may be confined to the case where $L = \{1, n\}$; if there were a relation $\sum_{i=1}^n \xi_i x_i = 0$ with $\xi_i \in K$, the $\xi_i$ not all zero, it would follow that for all $\beta \in A$, $\sum_{i=1}^n (\beta \xi_i) x_i = 0$. By hypothesis we can suppose $\beta \neq 0$ in $A$ such that $\beta \xi_i = \alpha_i$ belongs to $A$ for all $i$; but the relation $\sum_{i=1}^n \alpha_i x_i = 0$ is contrary to the hypothesis, the $\alpha_i$ being not all zero.

(2) If the ring homomorphism $\rho : B \to A$ is surjective and $b$ is its kernel (so that $A$ is canonically identified with $B/b$), then, for every $A$-module $E$, $b$ is contained in the annihilator of $\rho_*(E)$ and $E$ is the $A$-module derived from $\rho_*(E)$ by the process defined in no. 12.

Let $A, B$ be two rings and $\rho : B \to A$ a homomorphism. Let $E$ be an $A$-module and $F$ a $B$-module; a *B-linear* mapping $u : F \to \rho_*(E)$ (also called a *B-linear mapping of* $F$ *into* $E$ if no confusion arises) is also called a *semi-linear mapping* (relative to $\rho$) of the $B$-module $F$ into the $A$-module $E$; it is also said that the ordered pair $(u, \rho)$ is a *dimorphism* of $F$ into $E$; this therefore means that, for $x \in F, y \in F$ and $\beta \in B$,

$$
\begin{cases}
u(x + y) = u(x) + u(y) \\
u(\beta x) = \rho(\beta) u(x).
\end{cases}
$$

The set $\mathrm{Hom}_B(F, \rho_*(E))$ of $B$-linear mappings of $F$ into $E$ is also written as $\mathrm{Hom}_B(F, E)$ if no confusion can arise.

When $\rho$ is an *isomorphism* of $B$ onto $A$, the relation $u(\beta x) = \rho(\beta) u(x)$ for all $\beta \in B$ may also be written as $u(\rho'(\alpha)x) = \alpha x$ for all $\alpha \in A$, where $\rho'$ denotes the inverse isomorphism of $\rho$; to say that $u$ is semi-linear for $\rho$ is then equivalent to saying that $u$ is an *A-linear mapping of* $\rho'_*(F)$ *into* $E$.

#### Example {#alg-ii-s1-n13-exa-1 .statement}

It has been seen (no. 1) that a homothety $h_\alpha : x \mapsto \alpha x$ on an $A$-module $E$ is not necessarily a linear mapping. But if $\alpha$ is *invertible*, $h_\alpha$ is a *semi-linear* mapping (which is moreover bijective) relative to the inner automorphism $\xi \mapsto \alpha \xi \alpha^{-1}$ of $A$, for $\alpha(\lambda x) = (\alpha \lambda \alpha^{-1})(\alpha x)$.

Let C be a third ring, $\rho': C \to B$ a homomorphism and G a C-module. If $v: G \to F$ is a semi-linear mapping relative to $\rho'$, the composition $w = u \circ v$ is a semi-linear mapping of G into E relative to the homomorphism $\rho'' = \rho \circ \rho'$. If $\rho$ is an *isomorphism* and $u: F \to E$ is a *bijective* semi-linear mapping relative to $\rho$, the inverse mapping $u': E \to F$ is a semi-linear mapping *relative to the inverse isomorphism* $\rho': A \to B$ of $\rho$.

It is thus seen that, for the species of structure defined by giving on an ordered pair (A, E) of sets a ring structure on A and a left A-module structure on E, the *dimorphisms* $(u, \phi)$ can be taken as *morphisms* (*Set Theory*, IV, § 2, no. 1); we shall always assume in what follows that this choice of morphisms has been made.

*Remark (3)*. Let $A_1, A_2$ be two rings, $A = A_1 \times A_2$ their product and let $e_1 = (1, 0),\ e_2 = (0, 1)$ in A, so that $A_1$ and $A_2$ are canonically identified with the two-sided ideals $Ae_1$ and $Ae_2$ of A. For every A-module E, $e_1E$ and $e_2E$ are sub-A-modules $E_1,\ E_2$ of E, annihilated respectively by $e_2$ and $e_1$, so that, canonically identifying $A/Ae_2$ with $A_1$ and $A/Ae_1$ with $A_2$, $E_1$ (resp. $E_2$) is given an $A_1$-module (resp. $A_2$-module) structure. Moreover, E is the *direct sum* of $E_1$ and $E_2$, for every $x \in E$ can be written as $x = e_1x + e_2x$ and the relation $e_1x = e_2y$ implies $e_1x = e_1^2x = e_1e_2y = 0$. Conversely, for every ordered pair consisting of an $A_1$-module $F_1$ and an $A_2$-module $F_2$, let $E_1$ be the A-module $(p_1) * (F_1)$, $E_2$ the A-module $(p_2) * (F_2)$, $p_1$ and $p_2$ being the projections of A onto $A_1$ and $A_2$ respectively; then in the A-module $E = E_1 \oplus E_2,\ E_1 = e_1E,\ E_2 = e_2E$. The study of A-modules is thus reduced to that of $A_1$-modules and that of $A_2$-modules. In particular, every submodule M of E is of the form $M_1 \oplus M_2$, where $M_1 = e_1M$ and $M_2 = e_2M$.

### 14. MULTIMODULES

Let A, B be two rings and consider on a set E two left module structures with the *same* additive law and whose ring of operators are respectively A and B; let $\mathscr{E}$ be the endomorphism ring of the additive group E and for all $\alpha \in A$ (resp. $\beta \in B$) let $h_\alpha$ (resp. $h'_\beta$) denote the element $x \mapsto \alpha x$ (resp. $x \mapsto \beta x$) of $\mathscr{E}$. Clearly the three following properties are equivalent: (a) $h_\alpha \circ h'_\beta = h'_\beta \circ h_\alpha$ for all $\alpha$ and $\beta$; (b) the image of A under the homomorphism $a \mapsto h_\alpha$ is *contained in* $\mathrm{Hom}_B(E, E)$; (c) the image of B under the homomorphism $\beta \mapsto h'_\beta$ is *contained in* $\mathrm{Hom}_A(E, E)$. When the A-module (resp. B-module) structure in question is a right module structure, the ring A (resp. B) must be replaced in (b) (resp. (c)) by $A^0$ (resp. $B^0$). The above properties can be expressed by saying that the two (left or right) module structures defined on E are *compatible*.

#### Definition 13 {#alg-ii-s1-def-13 .statement}

*Let* $(A_\lambda)_{\lambda \in L},\ (B_\mu)_{\mu \in M}$ *be two families of rings; an* $((A_\lambda),\ (B_\mu))$*-multimodule* (or *multimodule over the families of rings* $(A_\lambda)_{\lambda \in L},\ (B_\mu)_{\mu \in M}$) *is a set* E *with, for each* $\lambda \in L$, *a left* $A_\lambda$*-module structure and, for each* $\mu \in M$, *a right* $B_\mu$*-module structure, all these module structures being compatible with one another.*

When the family $(B_\mu)$ (resp. $(A_\lambda)$) is empty, E is called a *left* (resp. *right*) *multimodule*. When Card(L) + Card(M) = 2, we say "*bimodule*" instead of "*multimodule*"; it is then often convenient to consider (as can always be done by replacing a ring of operators by its opposite, cf. no. 1) a bimodule as having a *left module* structure with respect to a ring A and a *right module* structure with respect to a ring B, the permutability of the laws then being expressed by the relation

$$
\alpha(x\beta) = (\alpha x)\beta \quad \text{for } x \in E, \alpha \in A, \beta \in B.
$$

It is then also said that E is an *(A, B)*-*bimodule*.

Two *multimodule* structures on a set E are said to be *compatible* if all the module structures on E which define one or the other of these multimodule structures are compatible with one another.

#### Example {#alg-ii-s1-n14-exa-1 .statement}

(1) On a ring A the module structures of $A_s$ and $A_d$ are compatible and A can therefore be considered canonically as an (A, A)-bimodule.

(2) A left A-module E has a canonical left module structure over the ring $\operatorname{End}_A(E)$ and the A-module and $\operatorname{End}_A(E)$-module structures on E are *compatible*.

Clearly when E is a multimodule over two families $(A_\lambda)_{\lambda \in L}, (B_\mu)_{\mu \in M}$ of rings, E is also a multimodule over any two subfamilies $(A_\lambda)_{\lambda \in L'}, (B_\mu)_{\mu \in M'}$, where the $A_\lambda$-module and $B_\mu$-module structures for $\lambda \in L'$ and $\mu \in M'$ are those initially given.

Since multimodules are particular examples of commutative groups with operators, the results of nos. 2 to 10 (cf. no. 10, *Remark*) can be applied to them; in particular, if E, F are two $((A_\lambda), (B_\mu))$-multimodules, a *homomorphism* $u : E \to F$ is a mapping which is an $A_\lambda$-homomorphism for all $\lambda \in L$ and a $B_\mu$-homomorphism for all $\mu \in M$. The stable subgroups of an $((A_\lambda), (B_\mu))$-multimodule are $((A_\lambda), (B_\mu))$-multimodules (called *submultimodules*), as also are the quotients by such subgroups (called *quotient multimodules*); similarly for products and direct sums.

Let E be an $((A_\lambda), (B_\mu))$-multimodule and for each $\lambda \in L$ (resp. $\mu \in M$) let $\phi_\lambda : A'_\lambda \to A_\lambda$ (resp. $\psi_\mu : B'_\mu \to B_\mu$) be a ring homomorphism; clearly the $A'_\lambda$-module structures associated with the $\phi_\lambda$ and the $A_\lambda$-module structures given on E and the $B'_\mu$-module structures associated with the $\psi_\mu$ and the $B_\lambda$-module structures given on E are compatible with one another and hence define on E an $((A'_\lambda), (B'_\mu))$-multimodule structure, said to be *associated* with the given $((A_\lambda), (B_\mu))$-multimodule structure and the $\phi_\lambda$ and $\psi_\mu$.

If E, F are two $((A_\lambda), (B_\mu))$-multimodules, the additive group of homomorphisms of E into F is denoted by $\operatorname{Hom}_{(A_\lambda), (B_\mu)}(E, F)$ (or simply $\operatorname{Hom}(E, F)$). Formulae (6) to (8) of no. 2 are obviously valid for $((A_\lambda), (B_\mu))$-multimodule homomorphisms and, in particular, $\operatorname{Hom}(E, E) = \operatorname{End}(E)$ has a *ring* structure;

moreover Hom(E, F) has a canonical *left* End(F)-module structure and *right* End(E)-module structure, these two structures being compatible; in other words, Hom(E, F) has a canonical (End(F), End(E))-**bimodule** structure.

Suppose now that E has a multimodule structure whose rings of left (resp. right) operators are on the one hand the $A_\lambda$ for $\lambda \in L$ (resp. the $B_\mu$ for $\mu \in M$) and on the other the rings of another family $(A'_{\lambda'})_{\lambda' \in L'}$ (resp. $(B'_{\mu'})_{\mu' \in M'}$). Suppose similarly that F has a multimodule structure whose rings of left (resp. right) operators are on the one hand the $A_\lambda$ for $\lambda \in L$ (resp. the $B_\mu$ for $\mu \in M$) and on the other the rings of another family $(A''_{\lambda''})_{\lambda'' \in L''}$ (resp. $(B''_{\mu''})_{\mu'' \in M''}$); to abbreviate we shall say that E is an (($A_\lambda$), ($A'_{\lambda'}$); ($B_\mu$), ($B'_{\mu'}$))-multimodule and F an (($A_\lambda$), ($A''_{\lambda''}$); ($B_\mu$), ($B''_{\mu''}$))-multimodule. Consider E and F as (($A_\lambda$), ($B_\mu$))-multimodules, thus *restricting* the operators to the subfamilies ($A_\lambda$) and ($B_\mu$). By what was said at the beginnings of this no., the multimodule structures given on E and F define canonically ring homomorphisms

$$
A'_{\lambda'} \to \operatorname{End}_{(A_\lambda), (B_\mu)}(E), \qquad {B'_{\mu'}}^0 \to \operatorname{End}_{(A_\lambda), (B_\mu)}(E),
$$
$$
A''_{\lambda''} \to \operatorname{End}_{(A_\lambda), (B_\mu)}(F), \qquad B''_{\mu''} \to \operatorname{End}_{(A_\lambda), (B_\mu)}(F);
$$

moreover, two elements of $\operatorname{End}_{(A_\lambda), (B_\mu)}(E)$ (resp. $\operatorname{End}_{(A_\lambda), (B_\mu)}(F)$) respective images of elements of two distinct rings among the $A'_{\lambda'}$, or the ${B'_{\mu'}}^0$ (resp. the $A''_{\lambda''}$ or the $B''_{\mu''}$) are permutable; it follows that the above homomorphisms define on $\operatorname{Hom}_{(A_\lambda), (B_\mu)}(E, F)$ a *multimodule* structure whose rings of *left* operators are the $A''_{\lambda''}$ ($\lambda'' \in L''$) and the $B'_{\mu'}$ ($\mu' \in M'$) and whose rings of *right* operators are the $A'_{\lambda'}$ ($\lambda' \in L'$) and the $B''_{\mu''}$ ($\mu'' \in M''$).

If now $E'$ is an (($A_\lambda$), ($A'_{\lambda'}$); ($B_\mu$), ($B'_{\mu'}$))-multimodule and $F'$ an (($A_\lambda$), ($A''_{\lambda''}$); ($B_\mu$), ($B''_{\mu''}$))-multimodule, $\operatorname{Hom}_{(A_\lambda), (B_\mu)}(E', F')$ is an

$$
((A''_{\lambda''}), (B'_{\mu'}); (A'_{\lambda'}), (B''_{\mu''}))\text{-multimodule};
$$

if $u : E' \to E, v : F \to F'$ are multimodule homomorphisms,

$$
\operatorname{Hom}(u, v) : \operatorname{Hom}_{(A_\lambda), (B_\mu)}(E, F) \to \operatorname{Hom}_{(A_\lambda), (B_\mu)}(E', F')
$$

is defined as in no. 2 and is a *multimodule* homomorphism.

#### Remark {#alg-ii-s1-n14-rem-1 .statement}

(1) Let F be an A-module and C the *centre* of the ring A; as central homotheties commute with all homotheties, F has a *bimodule* structure whose rings of left operators are A and C. If E is another A-module, $\operatorname{Hom}_A(E, F)$ has therefore a canonical C-*module* structure (where, for $f \in \operatorname{Hom}_A(E, F)$ and $\gamma \in C$, $\gamma f$ is the homomorphism $x \mapsto \gamma f(x)$); if E', F' are two A-modules, $u : E' \to E, v : F \to F'$ two A-homomorphisms, the mapping $\operatorname{Hom}(u, v)$ is C-*linear*.

(2) Let E be a left A-module; as A has a canonical (A, A)-bimodule structure, so has the direct sum $A^{(T)}$ for any indexing set T; by the above, $\mathrm{Hom}_A(A_s^{(T)}, E)$ has a canonical *left A-module* structure arising from the *right* A-module structure on $A_s^{(T)}$: for $f \in \mathrm{Hom}_A(A_s^{(T)}, E)$ and $\alpha \in A$, $\alpha f$ is the linear mapping $x \mapsto f(x\alpha)$. Corollary 2 to Proposition 17 of no. 11 defines a canonical mapping $j_{E, T}$ from the product module $E^T$ to $\mathrm{Hom}_A(A_s^{(T)}, E)$, the image under $j_{E, T}$ of a family $(x_t)_{t \in T}$ being the linear mapping $f : A_s^{(T)} \to E$ such that $f(e_t) = x_t$ for all $t \in T$ (where $(e_t)$ is the canonical basis of $A_s^{(T)}$); it is known (*loc. cit.*) that $j_{E, T}$ is *bijective* and it follows from the definition given above of the A-module structure on $\mathrm{Hom}_A(A_s^{(T)}, E)$ that $j_{E, T}$ is *A-linear*. Finally, if $u : E \to F$ is an A-module homomorphism, the diagram

$$
\begin{array}{ccc}
E^T & \xrightarrow{j_{E, T}} & \mathrm{Hom}_A(A_s^{(T)}, E) \\
u^T \downarrow & & \downarrow \mathrm{Hom}(1, u) \\
F^T & \xrightarrow{j_{F, T}} & \mathrm{Hom}_A(A_s^{(T)}, F)
\end{array}
$$

is *commutative*.

Note that when T consists of a single element, $j_E : E \to \mathrm{Hom}_A(A_s, E)$ is just the mapping $x \mapsto \theta_x$ defined in no. 2, *Example* 1.

### Exercises {#alg-ii-s1-exercises}

See the [exercises for § 1](exercises/s1/).
