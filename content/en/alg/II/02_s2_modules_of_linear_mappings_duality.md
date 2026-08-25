---
book: alg
book_title: Algebra
chapter: II
chapter_title: LINEAR ALGEBRA
section: 2
section_title: Modules of linear mappings. Duality
lang: en
source: alg-i-iii
source_edition: 1998, Springer
pdf_pages: 0251-0267, 0410-0419
extraction: ocr
subsections:
    - "no": 1
      title: PROPERTIES OF $ \mathrm{Hom}_A(E, F) $ RELATIVE TO EXACT SEQUENCES
      page: 0
      pdf_page: 251
    - "no": 2
      title: PROJECTIVE MODULES
      page: 0
      pdf_page: 255
    - "no": 3
      title: LINEAR FORMS; DUAL OF A MODULE
      page: 0
      pdf_page: 256
    - "no": 4
      title: ORTHOGONALITY
      page: 0
      pdf_page: 258
    - "no": 5
      title: TRANSPOSE OF A LINEAR MAPPING
      page: 0
      pdf_page: 258
    - "no": 6
      title: DUAL OF A QUOTIENT MODULE. DUAL OF A DIRECT SUM. DUAL BASES
      page: 0
      pdf_page: 260
    - "no": 7
      title: BIDUAL
      page: 0
      pdf_page: 263
    - "no": 8
      title: LINEAR EQUATIONS
      page: 0
      pdf_page: 264
statements: 42
exercises: 3
content_sha256: 3b782f3a14dd64b6c4820e944b52b743d6c50f9a631627053d96cf898326cdfe
---

## § 2. MODULES OF LINEAR MAPPINGS. DUALITY

### 1. PROPERTIES OF $ \mathrm{Hom}_A(E, F) $ RELATIVE TO EXACT SEQUENCES

#### Theorem 1 {#alg-ii-s2-thm-1 .statement}

*Let A be a ring, E', E, E'' three A-modules and u : E' \to E, v : E \to E'' two homomorphisms. For the sequence*

$$
\text{(1)} \quad E' \xrightarrow{u} E \xrightarrow{v} E'' \longrightarrow 0
$$

*to be exact, it is necessary and sufficient that, for every A-module F, the sequence*

$$
\text{(2)} \quad 0 \longrightarrow \mathrm{Hom}(E'', F) \xrightarrow{\bar{v}} \mathrm{Hom}(E, F) \xrightarrow{\bar{u}} \mathrm{Hom}(E', F)
$$

(where $ \bar{u} = \mathrm{Hom}(u, 1_F) $, $ \bar{v} = \mathrm{Hom}(v, 1_F) $) *be exact*.

Suppose that sequence (1) is exact. If $ w \in \mathrm{Hom}(E'', F) $ and $ \bar{v}(w) = w \circ v = 0 $, then $ w = 0 $ since $ v $ is surjective. Sequence (2) is therefore exact at $ \mathrm{Hom}(E'', F) $. We show that it is exact at $ \mathrm{Hom}(E, F) $. $ \bar{u} \circ \bar{v} = \mathrm{Hom}(v \circ u, 1_F) $ (\S 1, no. 2, formula (10)) and $ v \circ u = 0 $ since sequence (1) is exact at E. Therefore $ \bar{u} \circ \bar{v} = 0 $, that is $ \mathrm{Im}(\bar{v}) \subset \mathrm{Ker}(\bar{u}) $. On the other hand, if $ w \in \mathrm{Ker}(\bar{u}) $, then $ w \circ u = 0 $ and hence $ \mathrm{Ker}(w) \supset \mathrm{Im}(u) $. But as sequence (1) is exact at E, $ \mathrm{Im}(u) = \mathrm{Ker}(v) $ and hence $ \mathrm{Ker}(w) \supset \mathrm{Ker}(v) $; as $ v $ is surjective, it follows from \S 1, no. 3, *Remark* that there exists a $ w' \in \mathrm{Hom}(E'', F) $ such that w = w' \circ v = \bar{v}(w'). Therefore Ker(\bar{u}) \subset \operatorname{Im}(\bar{v}), which completes the proof that sequence (2) is exact.

Conversely, suppose that (2) is exact for every A-module F. As $ \bar{u} \circ \bar{v} = \operatorname{Hom}(v \circ u, 1_F) = 0, w \circ v \circ u = 0 $ for every homomorphism $ w : E'' \to F $. Taking $ F = E'' $ and $ w = 1_{E''} $, it is seen first that $ v \circ u = 0 $ and hence $ u(E') \subset \operatorname{Ker}(v) $. Now take $ F = \operatorname{Coker}(u) $ and let $ \phi : E \to F = E/u(E') $ be the canonical mapping. Then $ \bar{u}(\phi) = \phi \circ u = 0 $ by definition and hence there exists a $ \psi \in \operatorname{Hom}(E'', F) $ such that $ \phi = \bar{v}(\psi) = \psi \circ v $; this obviously implies $ u(E') = \operatorname{Ker}(\phi) \supset \operatorname{Ker}(v) $, which proves that sequence (1) is exact at E. Finally, let $ \theta $ be the canonical homomorphism of $ E'' $ onto $ F = E''/v(E) $; then $ \bar{v}(\theta) = \theta \circ v = 0 $, hence $ \theta = 0 $; therefore, $ F = \{0\} $ and $ v $ is surjective. Sequence (1) is therefore exact at $ E'' $.

#### Corollary {#alg-ii-s2-n1-cor-1 .statement}

*For an A-linear mapping* $ u : E \to F $ *to be surjective* (resp. *bijective*, resp. *zero*), *it is necessary and sufficient that, for every A-module G, the mapping* $ \operatorname{Hom}(u, 1_G) : \operatorname{Hom}(F, G) \to \operatorname{Hom}(E, G) $ *be injective* (resp. *bijective*, resp. *zero*).

It suffices to apply Theorem 1 to the case where $ E'' = \{0\} $ (resp. $ E' = \{0\} $ resp. $ E'' = E $ and $ v = 1_E $).

Note that starting from an exact sequence

$$
0 \longrightarrow E' \xrightarrow{u} E \xrightarrow{v} E'' \longrightarrow 0
$$

the corresponding sequence

$$
0 \longrightarrow \operatorname{Hom}(E'', F) \xrightarrow{\bar{v}} \operatorname{Hom}(E, F) \xrightarrow{\bar{u}} \operatorname{Hom}(E', F) \longrightarrow 0
$$

*is not necessarily exact*, in other words, the homomorphism $ \bar{u} $ is not necessarily surjective. If $ E' $ is identified with a submodule of E, this means that a linear mapping of $ E' $ into F cannot always be extended to a linear mapping of E into F (Exercises 11 and 12). However:

#### Proposition 1 {#alg-ii-s2-prop-1 .statement}

*If the exact sequence of linear mappings*

(3)
$$
0 \longrightarrow E' \xrightarrow{u} E \xrightarrow{v} E'' \longrightarrow 0
$$

*splits* (in other words, if $ u(E') $ is a *direct factor* of E) *the sequence*

(4)
$$
0 \longrightarrow \operatorname{Hom}(E'', F) \xrightarrow{\bar{v}} \operatorname{Hom}(E, F) \xrightarrow{\bar{u}} \operatorname{Hom}(E', F) \longrightarrow 0
$$

*is exact and splits*. *Conversely, if, for every A-module F, sequence (4) is exact, sequence (3) splits*.

If the exact sequence (3) splits, there exists a linear retraction $ u' : E \to E' $ associated with $ u $ (\S 1, no. 9, Proposition 15); if

$$
\bar{u}' = \operatorname{Hom}(u', 1_F) : \operatorname{Hom}(E', F) \to \operatorname{Hom}(E, F),
$$

the fact that $ u' \circ u $ is the identity implies that $ \bar{u} \circ \bar{u}' $ is the identity ($ \S 1 $, no. 2, formula (10)) and hence the first assertion follows from $ \S 1 $, no. 9, Proposition 15. Conversely, suppose sequence (4) is exact for $ F = E' $. Then there exists an element $ f \in \mathrm{Hom}(E, E') $ such that $ f \circ u = 1_{E'} $, and the conclusion follows from $ \S 1 $, no. 9, Proposition 15.

Note that the first assertion of Proposition 1 can also be considered as a special case of $ \S 1 $, no. 6, Corollary 1 to Proposition 6, canonically identifying $ \mathrm{Hom}(E', F) \oplus \mathrm{Hom}(E'', F) $ with $ \mathrm{Hom}(E' \oplus E'', F) $ by means of the $ \mathbf{Z} $-linear mapping $ \mathrm{Hom}(p', 1_F) + \mathrm{Hom}(p'', 1_F) $, where $ p': E' \oplus E'' \to E' $ and $ p'': E' \oplus E'' \to E'' $ are the canonical projections.

#### Theorem 2 {#alg-ii-s2-thm-2 .statement}

*Let $ A $ be a ring, $ F', F, F'' $ three $ A $-modules and $ u: F' \to F, v: F \to F'' $ two homomorphisms. For the sequence*

$$
0 \longrightarrow F' \xrightarrow{v} F \xrightarrow{u} F''
$$

*to be exact, it is necessary and sufficient that, for every $ A $-module $ E $, the sequence*

$$
0 \longrightarrow \mathrm{Hom}(E, F') \xrightarrow{\bar{u}} \mathrm{Hom}(E, F) \xrightarrow{\bar{v}} \mathrm{Hom}(E, F'')
$$

*(where $ \bar{u} = \mathrm{Hom}(1_E, u), \bar{v} = \mathrm{Hom}(1_E, v) $) be exact.*

Suppose that the sequence (5) is exact. Note first that

$$
\bar{v} \circ \bar{u} = \mathrm{Hom}(1_E, v \circ u) = 0
$$

(II, $ \S 1 $, no. 2, formula (10)) since $ v \circ u = 0 $. The image of $ \mathrm{Hom}(E, F') $ under $ \bar{u} $ is therefore contained in the kernel $ N $ of $ \bar{v} $; let $ f $ be the homomorphism of the $ \mathbf{Z} $-module $ \mathrm{Hom}(E, F') $ into $ N $ whose graph is equal to that of $ \bar{u} $; it is necessary to prove that $ f $ is *bijective* and hence to define a mapping $ g: N \to \mathrm{Hom}(E, F') $ such that $ f \circ g $ and $ g \circ f $ are the identity mappings. For this, let $ w $ be an element of $ N $, that is a linear mapping $ w: E \to F $ such that $ v \circ w = 0 $. The latter relation is equivalent to $ w(E) \subset \mathrm{Ker}(v) = u(F') $ by hypothesis, hence, since $ u $ is injective, there exists one and only one linear mapping $ w': E \to F' $ such that $ w = u \circ w' $ and we take $ g(w) = w' $; it is immediately verified that $ g $ satisfies the desired conditions.

Conversely, suppose that sequence (6) is exact for every $ A $-module $ E $. As $ \mathrm{Hom}(1_E, v \circ u) = \bar{v} \circ \bar{u} = 0 $, then $ v \circ u \circ w = 0 $ for every homomorphism $ w: E \to F' $. Taking $ E = F' $ and $ w = 1_{F'} $, it is seen first that $ v \circ u = 0 $ and hence $ u(F') \subset \mathrm{Ker}(v) $. Now we take $ E = \mathrm{Ker}(v) $ and let $ \phi: E \to F $ be the canonical injection. Then $ \bar{v}(\phi) = v \circ \phi = 0 $ by definition and hence there exists $ \psi \in \mathrm{Hom}(E, F') $ such that $ \phi = \bar{u}(\psi) = u \circ \psi $, which obviously implies $ \mathrm{Ker}(v) \subset u(F') $ and completes the proof of the exactness of (5) at $ F $. Finally, if $ \theta $ is the identity mapping of $ \mathrm{Ker}\, u $, then $ \bar{u}(\theta) = 0 $, hence $ \theta = 0 $ and $ \mathrm{Ker}\, u = \{0\} $, which proves the exactness of (5) at $ F' $.

#### Remark {#alg-ii-s2-n1-rem-1 .statement}

(1) Theorem 2 allows us, for every submodule F' of F, to identify Hom(E, F') with a sub-$\mathbf{Z}$-module of Hom(E, F). When this identification is made, then, for every family $(M_\lambda)$ of submodules of F

$$
\operatorname{Hom}(E, \bigcap_\lambda M_\lambda) = \bigcap_\lambda \operatorname{Hom}(E, M_\lambda)
$$

for if $u \in \operatorname{Hom}(E, F)$ belongs to each of the $\operatorname{Hom}(E, M_\lambda)$, then, for all $x \in E$, $u(x) \in M_\lambda$ for all $\lambda$ and hence $u$ maps E into $\bigcap_\lambda M_\lambda$.

#### Corollary {#alg-ii-s2-n1-cor-2 .statement}

*For an A-linear mapping* $u : E \to F$ *to be injective, it is necessary and sufficient that, for every A-module G, the mapping* $\operatorname{Hom}(1_G, u) : \operatorname{Hom}(G, E) \to \operatorname{Hom}(G, F)$ *be injective*.

It suffices to apply Theorem 2 to the case where $F' = \{0\}$.

Starting from an exact sequence

$$
0 \longrightarrow F' \xrightarrow{u} F \xrightarrow{v} F'' \longrightarrow 0
$$

the corresponding sequence

$$
0 \longrightarrow \operatorname{Hom}(E, F') \xrightarrow{\bar{u}} \operatorname{Hom}(E, F) \xrightarrow{\bar{v}} \operatorname{Hom}(E, F'') \longrightarrow 0
$$

*is not necessarily exact*, in other words $\bar{v}$ is not necessarily surjective. If $F'$ is identified with a submodule of $F$ and $F''$ with the quotient module $F/F'$, this means that a linear mapping of $E$ into $F''$ is not necessarily of the form $v \circ w$, where $w$ is a linear mapping of $E$ into $F$. However:

#### Proposition 2 {#alg-ii-s2-prop-2 .statement}

*If the exact sequence*

(7)

$$
0 \longrightarrow F' \xrightarrow{u} F \xrightarrow{v} F'' \longrightarrow 0
$$

*splits* (in other words, if $u(F')$ is a *direct factor* of $F$), *the sequence*

(8)

$$
0 \longrightarrow \operatorname{Hom}(E, F') \xrightarrow{\bar{u}} \operatorname{Hom}(E, F) \xrightarrow{\bar{v}} \operatorname{Hom}(E, F'') \longrightarrow 0
$$

*is exact and splits*. *Conversely, if sequence* (8) *is exact for every A-module E, the exact sequence* (7) *splits*.

The first assertion follows from the fact that

$$
\operatorname{Hom}(E, F') \oplus \operatorname{Hom}(E, F'')
$$

is canonically identified with $\operatorname{Hom}(E, F' \oplus F'')$ by means of the $\mathbf{Z}$-linear mapping $\operatorname{Hom}(1_E, j') + \operatorname{Hom}(1_E, j''), j' : F' \to F' \oplus F''$ and $j'' : F'' \to F' \oplus F''$ being the canonical injections (\S 1, no. 6, Corollary 1 to Proposition 6). Conversely, if sequence (8) is exact for $E = F''$, there is an element $g \in \operatorname{Hom}(F'', F)$ such that $v \circ g = 1_{F''}$ and the conclusion follows from \S 1, no. 9, Proposition 15.

Remark (2). The results of this no. are valid without modification for all commutative groups with operators.

### 2. PROJECTIVE MODULES

#### Definition 1 {#alg-ii-s2-def-1 .statement}

An A-module P is called projective if, for every exact sequence F' → F → F'' of A-linear mapping, the sequence

$$
\operatorname{Hom}(P, F') \to \operatorname{Hom}(P, F) \to \operatorname{Hom}(P, F'')
$$

is exact.

#### Proposition 3 {#alg-ii-s2-prop-3 .statement}

For an A-module P, the direct sum of a family of submodules (M_i), to be projective, it is necessary and sufficient that each of the M_i be projective.

For every A-module homomorphism u : E → F,

$$
\operatorname{Hom}(1_P, u) : \operatorname{Hom}(P, E) \to \operatorname{Hom}(P, F)
$$

is identified with $ \prod_i \operatorname{Hom}(1_{M_i}, u) $ (\S 1, no. 6, Corollary 1 to Proposition 6); the conclusion thus follows from Definition 1 and \S 1, no. 5, Proposition 5 (ii).

#### Corollary {#alg-ii-s2-n2-cor-1 .statement}

Every free A-module is projective.

It suffices by Proposition 3 to show that A_s is projective, which follows immediately from the commutativity of diagram (50) of \S 1, no. 14.

#### Proposition 4 {#alg-ii-s2-prop-4 .statement}

Let P be an A-module. The following properties are equivalent:

(a) P is projective.
(b) For every exact sequence 0 → F' → F → F'' → 0 of A-linear mappings, the sequence

$$
0 \to \operatorname{Hom}(P, F') \to \operatorname{Hom}(P, F) \to \operatorname{Hom}(P, F'') \to 0
$$

is exact.

(c) For every surjective A-module homomorphism u : E → E'' and every homomorphism f : P → E'', there exists a homomorphism g : P → E such that f = u ∘ g (it is said that f can be "lifted" to a homomorphism of P into E).

(d) Every exact sequence 0 → E' → E → P → 0 of A-linear mappings splits (and therefore P is isomorphic to a direct factor of E).

(e) P is isomorphic to a direct factor of a free A-module.

It is trivial that (a) implies (b). To see that (b) implies (c), it suffices to apply (b) to the exact sequence 0 → E' → E → E'' → 0, where E' = Ker(u), since (c) expresses the fact that

$$
\operatorname{Hom}(1_P, u) : \operatorname{Hom}(P, E) \to \operatorname{Hom}(P, E'')
$$

is surjective. To see that (c) implies (d), it suffices to apply (c) to the surjective homomorphism $ v : E \to P $ and the homomorphism $ l_P : P \to P $; the existence of a homomorphism $ g : P \to E $ such that $ l_P = v \circ g $ implies that the sequence

$$
0 \longrightarrow E' \longrightarrow E \xrightarrow{v} P \longrightarrow 0
$$

splits (\S 1, no. 9, Proposition 15). As for every A-module M there exist a free A-module L and an exact sequence $ 0 \to R \to L \to M \to 0 $ (\S 1, no. 11, Proposition 20), clearly (d) implies (e). Finally (e) implies (a) by virtue of Proposition 3 and its Corollary.

#### Corollary 1 {#alg-ii-s2-prop-4-cor-1 .statement}

*For an A-module to be projective and finitely generated, it is necessary and sufficient that it be a direct factor of a free A-module with a finite basis.*

The condition is obviously sufficient; conversely, a finitely generated projective module E is isomorphic to a quotient of a free module F with a finite basis (\S 1, no. 11) and E is isomorphic to a direct factor of F by virtue of Proposition 4 (d).

#### Corollary 2 {#alg-ii-s2-prop-4-cor-2 .statement}

*Let C be a commutative ring and E, F two finitely generated projective C-modules; then $ \operatorname{Hom}_C(E, F) $ is a finitely generated projective C-module.*

It may be assumed that there are two finitely generated free C-modules M, N such that $ M = E \oplus E', N = F \oplus F' $; it follows from \S 1, no. 6, Corollary 1 to Proposition 6 that $ \operatorname{Hom}_C(M, N) $ is finitely generated and free and on the other hand that $ \operatorname{Hom}_C(M, N) $ is isomorphic to

$$
\operatorname{Hom}_C(E, F) \oplus \operatorname{Hom}_C(E', F) \oplus \operatorname{Hom}_C(E, F') \oplus \operatorname{Hom}(E', F'),
$$

whence the corollary.

### 3. LINEAR FORMS; DUAL OF A MODULE

Let E be a *left* A-module. As A is an (A, A)-bimodule, $ \operatorname{Hom}_A(E, A_s) $ has a canonical *right* A-module structure (\S 1, no. 14).

#### Definition 2 {#alg-ii-s2-def-2 .statement}

*For every right A-module E, the right A-module $ \operatorname{Hom}_A(E, A_s) $ is called the dual module of E* (or simply the *dual†* of E) *and its elements are called the linear forms on E*.

If E is a *right* A-module, the set $ \operatorname{Hom}_A(E, A_d) $ with its canonical *left* A-module structure is likewise called the *dual* of E and its elements are called *linear forms* on E.

† In *Topological Vector Spaces*, IV, we shall define, for vector spaces with a *topology*, a notion of "dual space" which will depend on this topology and will be distinct from the one defined here. The reader must beware of incautiously applying to the "topological" dual space the properties of the "algebraic" dual which are established in this paragraph.

In this chapter, $ E^* $ will be used to denote the dual of a (left or right) A-module $ E $.

#### Example {#alg-ii-s2-n3-exa-1 .statement}

*On the vector space (with respect to the field $ \mathbf{R} $) of continuous real-valued functions on an interval $[a, b]$ of $ \mathbf{R} $, the mapping $ x \mapsto \int_a^b x(t) dt $ is a linear form.*

Let $ E $ be a left A-module and $ E^* $ its dual; for every ordered pair of elements $ x \in E, x^* \in E^* $, the element $ x^*(x) $ of A is denoted by $ \langle x, x^* \rangle $. Then the relations

$$
\begin{align*}
(9) \quad & \langle x + y, x^* \rangle = \langle x, x^* \rangle + \langle y, x^* \rangle \\
(10) \quad & \langle x, x^* + y^* \rangle = \langle x, x^* \rangle + \langle x, y^* \rangle \\
(11) \quad & \langle \alpha x, x^* \rangle = \alpha \langle x, x^* \rangle \\
(12) \quad & \langle x, x^* \alpha \rangle = \langle x, x^* \rangle \alpha
\end{align*}
$$

hold for $ x, y $ in $ E, x^*, y^* $ in $ E^* $ and $ \alpha \in A $. The mapping $ (x, x^*) \mapsto \langle x, x^* \rangle $ of $ E \times E^* $ into $ A $ is called the canonical bilinear form on $ E \times E^* $ (the notion of bilinear form will be defined generally in IX, § 1). Every linear form $ x^* $ on $ E $ can be considered as the partial mapping $ x \mapsto \langle x, x^* \rangle $ corresponding to the canonical bilinear form.

When $ E $ is a right A-module, the value $ x^*(x) $ of a linear form $ x^* \in E^* $ at an element $ x \in E $ is denoted by $ \langle x^*, x \rangle $ and the formulae corresponding to (11) and (12) are written as

$$
\begin{align*}
\langle x^*, x \alpha \rangle &= \langle x^*, x \rangle \alpha \\
\langle \alpha x^*, x \rangle &= \alpha \langle x^*, x \rangle.
\end{align*}
$$

When A is commutative, either notation is permissible.

#### Proposition 5 {#alg-ii-s2-prop-5 .statement}

For every ring A, the mapping which associates with every $ \xi \in A $ the linear form $ \eta \mapsto \eta \xi $ on $ A_s $ is an isomorphism of $ A_d $ onto the dual of $ A_s $.

It is the particular case of the canonical isomorphism $ E \to \mathrm{Hom}_A(A_s, E) $ of § 1, no. 14, Remark 2, corresponding to $ E = A_s $; the commutativity of diagram (50) of § 1, no. 14, shows that we have here an isomorphism of right A-modules.

If $ A_d $ is identified with the dual of $ A_s $ by means of the isomorphism of Proposition 5, the canonical bilinear form on $ A_s \times A_d $ is then expressed by

$$
\langle \xi, \xi^* \rangle = \xi \xi^* \quad \text{for } \xi, \xi^* \text{ in } A.
$$

Similarly, the dual of $ A_d $ is canonically identified with $ A_s $, the canonical bilinear form on $ A_d \times A_s $ being expressed by

$$
\langle \xi^*, \xi \rangle = \xi^* \xi \quad \text{for } \xi, \xi^* \text{ in } A.
$$

### 4. ORTHOGONALITY

#### Definition 3 {#alg-ii-s2-def-3 .statement}

Let E be an A-module and E* its dual; an element x ∈ E and an element x* ∈ E* are called orthogonal if ⟨x, x*⟩ = 0.

A subset M of E and a subset M' of E* are called orthogonal sets if, for all x ∈ M, x* ∈ M', x and x* are orthogonal. In particular, x* ∈ E* (resp. x ∈ E) is called orthogonal to M (resp. M') if it is orthogonal to every element of M (resp. M'). If x* and y* are orthogonal to M, so is x* + y* and x*α for all α ∈ A by virtue of (10) and (12) (no. 3), which justifies the following definition:

#### Definition 4 {#alg-ii-s2-def-4 .statement}

Given a subset M of E (resp. a subset M' of E*), the set of x* ∈ E* (resp. the set of x ∈ E) which are orthogonal to M (resp. M') is called the submodule totally orthogonal to M (resp. M') (or simply the submodule orthogonal to M (resp. M') if no confusion can arise).

By definition of a linear form, the submodule of E* orthogonal to E is reduced to 0; the submodule of E* orthogonal to {0} is identical with E*.

#### Proposition 6 {#alg-ii-s2-prop-6 .statement}

Let M, N be two subsets of E such that M ⊂ N; if M' and N' are the submodules of E* orthogonal to M and N respectively, then N' ⊂ M'.

#### Proposition 7 {#alg-ii-s2-prop-7 .statement}

Let (M_i) be a family of subsets of E; the submodule orthogonal to the union of the M_i is the intersection of the submodules M'_i which are respectively orthogonal to the M_i; this submodule is also the submodule orthogonal to the submodule of E generated by the union of the M_i.

These results are immediate consequences of the definitions.

There is an analogous proposition (which we shall leave to the reader to state) for submodules of E orthogonal to subsets of E*.

If M is a submodule of E, M' the submodule of E* orthogonal to M and M'' the submodule of E orthogonal to M', then M ⊂ M'' but it may be that M ≠ M'' (Exercise 9). Note however that if M'' is the orthogonal of M'' in E*, then M'' = M'; for M' ⊂ M'' and on the other hand the relation M ⊂ M'' implies M'' ⊂ M'.

### 5. TRANSPOSE OF A LINEAR MAPPING

Let E, F be two left A-modules; for every linear mapping u : E → F, the mapping Hom(u, l_{A_s}) is a linear mapping of the right A-module F* into the right A-module E* (§ 1, no. 2), called the transpose of u.

In other words:

#### Definition 5 {#alg-ii-s2-def-5 .statement}

For every linear mapping u of an A-module E into an A-module F, the linear mapping y* ↦ y* ∘ u of the dual F* of F into the dual E* of E is called the transpose of u and is denoted by t u.

The transpose $ ^t u $ is therefore defined by the relation
(15) $$
\langle u(x), y^* \rangle = \langle x, ^t u(y^*) \rangle \quad \text{for all } x \in E \text{ and all } y^* \in F^*.
$$

Definition 5 applies without alteration to right A-modules and is then equivalent to the relation
$$
\langle y^*, u(x) \rangle = \langle ^t u(y^*), x \rangle \quad \text{for all } x \in E \text{ and all } y^* \in F^*.
$$

Formulae (9) and (10) of § 1, no. 2 here give
(16) $$
^t(u_1 + u_2) = ^t u_1 + ^t u_2
$$
for two elements $ u_1, u_2 $ of $ \mathrm{Hom}_A(E, F) $ and
(17) $$
^t(v \circ u) = ^t u \circ ^t v
$$
for $ u \in \mathrm{Hom}_A(E, F) $ and $ v \in \mathrm{Hom}_A(F, G) $, G being a third A-module; finally, clearly
(18) $$
^t 1_E = 1_{E^*}.
$$

#### Remark {#alg-ii-s2-n5-rem-1 .statement}

From (17) and (18) it follows that if $ u $ is left (resp. right) invertible, $ ^t u $ is right (resp. left) invertible.

#### Proposition 8 {#alg-ii-s2-prop-8 .statement}

*Let $ u : E \to F $ be an A-linear mapping, M a submodule of E and $ M' $ the orthogonal of M in $ E^* $; the orthogonal of $ u(M) $ in $ F^* $ is the inverse image $ ^t u^{-1}(M') $.*

This follows immediately from (15).

#### Corollary {#alg-ii-s2-n5-cor-1 .statement}

*The orthogonal of the image $ u(E) $ in $ F^* $ is the kernel $ ^t u^{-1}(0) $ of $ ^t u $.*

The orthogonal of E in $ E^* $ is 0.

If $ u : E \to F $ is an isomorphism, $ ^t u : F^* \to E^* $ is an isomorphism and if $ v : F \to E $ is the inverse isomorphism of $ u $, $ ^t v $ is the inverse isomorphism of $ ^t u $ (formulae (17) and (18)).

#### Definition 6 {#alg-ii-s2-def-6 .statement}

*Given an isomorphism u of an A-module E onto an A-module F, the transpose of the inverse isomorphism of u (equal to the inverse isomorphism of the transpose of u) is called the contragredient isomorphism of u and denoted by $ \tilde{u} $.*

The isomorphism $ \tilde{u} $ is thus characterized by the relation
(19) $$
\langle u(x), \tilde{u}(y^*) \rangle = \langle x, x^* \rangle \quad \text{for } x \in E, x^* \in E^*.
$$

If $ v : F \to G $ is an isomorphism, the contragredient isomorphism of $ v \circ u $ is $ \tilde{v} \circ \tilde{u} $.

In particular, the mapping $ u \mapsto \tilde{u} $ is an *isomorphism* of the linear group $ \mathbf{GL}(E) $ onto a subgroup of the linear group $ \mathbf{GL}(E^*) $.

Let $ \sigma : A \to B $ be an *isomorphism* of a ring $ A $ onto a ring $ B $, $ E $ a left $ A $-module, $ F $ a left $ B $-module and $ u : E \to F $ a *semi-linear* mapping (\S 1, no. 13) *relative to* $ \sigma $. Let $ \sigma^{-1} $ be the inverse isomorphism of $ \sigma $; for all $ y^* \in F^* $, the mapping $ x \mapsto \langle u(x), y^* \rangle^{\sigma^{-1}} $ of $ E $ into $ A $ is a *linear form*; if it is also denoted by $ {}^t u(y^*) $, a mapping $ {}^t u : F^* \to E^* $ is defined which is also called the *transpose* of the semi-linear mapping $ u $; it is thus characterized by the identity

$$
\langle u(x), y^* \rangle = \langle x, {}^t u(y^*) \rangle^\sigma
$$

for $ x \in E, y^* \in F^* $. It is immediately verified that $ {}^t u $ is a *semi-linear* mapping *relative to* $ \sigma^{-1} $. If $ v $ denotes the mapping $ u $ considered as an *A-linear* mapping of $ E $ into $ \sigma_*(F) $ (\S 1, no. 13), we may write $ u = \phi \circ v $, where $ \phi $ is the identity mapping $ \sigma_*(F) \to F $, considered as a semi-linear mapping relative to $ \sigma $. It is immediate that $ {}^t u = {}^t v \circ {}^t \phi $ and $ ({}^t \phi, \sigma^{-1}) $ is a di-isomorphism of $ F^* $ onto $ (\sigma_*(F))^* $ relative to the isomorphism $ \sigma^{-1} $; this relation allows us immediately to extend the properties of transposes of linear mappings to transposes of semi-linear mappings.

### 6. DUAL OF A QUOTIENT MODULE. DUAL OF A DIRECT SUM. DUAL BASES

We apply Theorem 1 of no. 1 to the case where $ F = A_s $:

#### Proposition 9 {#alg-ii-s2-prop-9 .statement}

*Let* $ E', E, E'' $ *be A-modules and*

$$
E' \xrightarrow{u} E \xrightarrow{v} E'' \longrightarrow 0
$$

*an exact sequence of linear mappings.* *Then the sequence of transpose mappings*

$$
0 \longrightarrow {E''}^* \xrightarrow{{}^t v} E^* \xrightarrow{{}^t u} {E'}^*
$$

*is exact.*

#### Corollary {#alg-ii-s2-n6-cor-1 .statement}

*Let M be a submodule of an A-module E and $ \phi : E \to E/M $ the canonical homomorphism. Then* $ {}^t \phi $ *is an isomorphism of the dual of* $ E/M $ *onto the submodule* $ M' $ *of* $ E^* $ *orthogonal to* $ M $.

If $ j : M \to E $ is the canonical injection, the kernel of $ {}^t j $ is by definition the orthogonal of $ M $ in $ E^* $.

Moreover, in the notation of the corollary, an *injective* homomorphism $ E^*/M' \to M^* $ is obtained from $ {}^t j $ when passing to the quotient.

#### Proposition 10 {#alg-ii-s2-prop-10 .statement}

*Let* $ (E_i)_{i \in I} $ *be a family of A-modules and for all* $ i \in I $ *let* $ j_i : E_i \to E = \bigoplus_{i \in I} E_i $ *be the canonical injection.* *Then the product mapping* $ x^* \mapsto ({}^t j_i(x^*)) $

*is an isomorphism of the dual* $ E^* $ *of* $ E $ *onto the product* $ \prod_{i \in I} E_i^* $.

This is a particular case of § 1, no. 6, Corollary 1 to Proposition 6, applied to the case where $ \prod_{\lambda} F_{\lambda} = A_s $.

If, by means of the canonical injections $ j_i $, the $ E_i $ are identified with submodules of their direct sum $ E $ and if, by means of the product mapping $ x^* \mapsto (tj_i(x^*)) $, $ E^* $ is identified with $ \prod_{i \in I} E_i^* $, it can then be said that $ \prod_{i \in I} E_i^* $ is the dual of $ \bigoplus_{i \in I} E_i $, the canonical bilinear form being given by

$$
\langle (x_i), (x_i^*) \rangle = \sum_{i \in I} \langle x_i, x_i^* \rangle.
$$

(22)

#### Corollary {#alg-ii-s2-n6-cor-2 .statement}

*Let M, N be two supplementary submodules in an A-module E and $ p : E \to M, q : E \to N $ the corresponding projectors; then $ ^tp + ^tq : M^* \oplus N^* \to E^* $ is an isomorphism and $ ^tp $ (resp. $ ^tq $) is an isomorphism of $ M^* $ (resp. $ N^* $) onto the submodule of $ E^* $ orthogonal to $ N $ (resp. $ M $). Moreover, if $ i : M \to E $ and $ j : N \to E $ are the canonical injections, $ ^tp \circ ^ti $ and $ ^tq \circ ^tj $ are the projectors $ E^* \to ^tp(M^*) $, $ E^* \to ^tq(N^*) $ corresponding to the decomposition of $ E^* $ as the direct sum of $ ^tp(M^*) $ and $ ^tq(N^*) $.

$ p \circ i = 1_M, \quad q \circ j = 1_N, \quad p \circ j = q \circ i = 0, \quad i \circ p + j \circ q = 1_E $, whence, by transposition (no. 5, formulae (16), (17) and (18)), $ ^ti \circ ^tp = 1_{M^*}, \ ^tj \circ ^tq = 1_{N^*}, \ ^tj \circ ^tp = ^ti \circ ^tq = 0. \ ^tp \circ ^ti + ^tq \circ ^tj = 1_{E^*} $ and the proposition follows from § 1, no. 6, Corollary 2 to Proposition 6.

Under the hypotheses of the Corollary, $ M^* $ (resp. $ N^* $) is often identified with the orthogonal $ ^tp(M^*) $ (resp. $ ^tq(N^*) $) of $ N $ (resp. $ M $) in $ E^* $, thus identifying every linear form $ u $ on $ M $ (resp. $ N $) with the linear form on $ E $ extending $ u $ and which is zero on $ N $ (resp. $ M $).

When an A-module $ E $ admits a *basis* $ (e_t)_{t \in T} $, it has been seen that giving this basis defines canonically an isomorphism $ u : A_s^{(T)} \to E $. By virtue of Proposition 10 and no. 3, Proposition 5, the dual of $ A_s^{(T)} $ is canonically identified with the product $ A_d^T $; consider the contragredient isomorphism $ \tilde{u} : A_d^T \to E^* $. If, for all $ t \in T, f_t $ is the element of $ A_d^T $ all of whose projections are zero with the exception of that of index $ t $, which is equal to 1, and if we write $ e_t^* = \tilde{u}(f_t) $, the elements $ e_t^* $ of $ E^* $ are, by (19) and (22), characterized by the relations

$$
\langle e_t, e_{t'}^* \rangle = \begin{cases}
0 & \text{for } t' \neq t \\
1 & \text{for } t' = t.
\end{cases}
$$

(23)

It amounts to the same to say that, for all $ x = \sum_{t \in T} \xi_t e_t \in E, \ e_t^*(x) = \xi_t $; also $ e_t^* $ is called the *coordinate form* of index $ t $ on $ E $. It follows from (23) that $ (e_t^*) $ is a *free system* in $ E^* $.

In particular, if $ T $ is *finite*, the $ e_t^* $ form a *basis* of $ E^* $, the $ f_t $ then forming the canonical basis of $ A_d^T $. Hence:

#### Proposition 11 {#alg-ii-s2-prop-11 .statement}

*The dual of a free module with a basis of n elements is a free module with a basis of n elements.*

Note that the dual of a free module with an infinite basis is not necessarily a free module (VII, § 3, Exercise 10).

#### Definition 7 {#alg-ii-s2-def-7 .statement}

*If E is a free module with a finite basis* $(e_t)$, *the basis* $(e_t^*)$ *of the dual E* *of E defined by relations (23) is called the dual basis of* $(e_t)$.

Relations (23) can also be written in the form
$$
\langle e_t, e_{t'}^* \rangle = \delta_{tt'}
$$
where $\delta_{tt'}$ is the *Kronecker symbol* on $T \times T$.

Note that if $T$ is finite and $(e_t^*)$ is the dual basis of $(e_t)$, then, for
$$ x = \sum_{t \in T} \xi_t e_t \in E, \quad x^* = \sum_{t \in T} \xi_t^* e_t^* \in E^*, $$
$$
\langle x, x^* \rangle = \sum_{t \in T} \xi_t \xi_t^*.
$$

The dual basis of a finite basis of a *right* A-module is of course defined similarly.

#### Corollary {#alg-ii-s2-n6-cor-3 .statement}

*The dual of a finitely generated projective module is a finitely generated projective module.*

A finitely generated projective left A-module can be identified with a direct factor M of a free A-module $A_s^n$ with a finite basis (no. 2, Corollary 1 to Proposition 4). Then (Proposition 11 and Corollary to Proposition 10) M* is isomorphic to a direct factor of $A_d^n$, whence the corollary.

#### Proposition 12 {#alg-ii-s2-prop-12 .statement}

*Let E be an A-module and* $(a_t)_{t \in T}$ *a generating system of E. The following conditions are equivalent:*
(a) *E is a projective A-module.*
(b) *There exists a family* $(a_t^*)_{t \in T}$ *of linear forms on E such that, for all* $x \in E$, *the family* $(\langle x, a_t^* \rangle)_{t \in T}$ *has finite support and*
$$
x = \sum_{t \in T} \langle x, a_t^* \rangle a_t.
$$

There exists a surjective homomorphism $u : L \to E$, where $L = A_s^{(T)}$, such that if $(e_t)_{t \in T}$ is the canonical basis of L then $u(e_t) = a_t$ (\S 1, no. 11, Proposition 17); for E to be projective, it is necessary and sufficient that there exist a linear mapping $v : E \to L$ such that $u \circ v = 1_E$ (no. 2, Proposition 4 and \S 1, no. 9, Proposition 15). If such a mapping exists and we write ${}^tv(e_t^*) = a_t^*$, then $\langle x, a_t^* \rangle = \langle x, {}^tv(e_t^*) \rangle = \langle v(x), e_t^* \rangle$, hence the family $(\langle x, a_t^* \rangle)$ has finite support and $ x = u \left( \sum_{t \in T} \langle (x), e_t^* \rangle e_t \right) = \sum_{t \in T} \langle x, a_t^* \rangle a_t $ for all $ x \in E $. Conversely, if condition (b) of the statement is fulfilled, the sum $ \sum_{t \in T} \langle x, a_t^* \rangle e_t $ is defined for all $ x \in E $ and $ x \to \sum_{t \in T} \langle x, a_t^* \rangle e_t $ is a linear mapping $ v : E \to L $ such that $ u \circ v = 1_E $.

### 7. BIDUAL

Let E be a left A-module. The dual $ E^{**} $ of the dual $ E^* $ of E is called the bidual of E; it is also a left A-module (no. 3). For all $ x \in E $, it follows from no. 3, formulae (10) and (12), that the mapping $ x^* \mapsto \langle x, x^* \rangle $ is a linear form on the right A-module $ E^* $, in other words an element of the bidual $ E^{**} $, which we shall denote by $ \tilde{x} $; moreover, it follows immediately from (9) and (11) (no. 3) that the mapping $ c_E : x \mapsto \tilde{x} $ of E into $ E^{**} $ is linear; this mapping will be called canonical; in general, it is neither injective nor surjective, even when E is finitely generated (cf. Exercise 9(e) and § 7, no. 5, Theorem 6).

An A-module E is called reflexive if the canonical homomorphism $ c_E : E \to E^{**} $ is bijective.

Let F be a second left A-module; for every linear mapping $ u : E \to F $, the mapping $ t(tu) : E^{**} \to F^{**} $, which will also be denoted by $ tu $, is linear and the diagram

$$
\begin{array}{ccc}
E & \xrightarrow{u} & F \\
c_E \downarrow & & \downarrow c_F \\
E^{**} & \xrightarrow{tu} & F^{**}
\end{array}
$$

is commutative, as follows immediately from the definitions and formula (15) giving the transpose of a linear mapping.

#### Proposition 13 {#alg-ii-s2-prop-13 .statement}

*If E is a free module* (resp. *a free module with a finite basis*), *the canonical mapping* $ c_E : E \to E^{**} $ *is injective* (resp. *bijective*).

Let $ (e_t)_{t \in T} $ be a basis of E and let $ (e_t^*) $ be the family of corresponding coordinate forms; by definition, if $ x \in E $ is such that $ \tilde{x} = 0 $, then $ \langle x, e_t^* \rangle = 0 $ for all $ t \in T $, in other words all the coordinates of $ x $ are zero, hence $ x = 0 $. Suppose further that T is finite; since $ \langle \tilde{e}_t, e_{t'}^* \rangle = \delta_{tt'} $, $ (\tilde{e}_t) $ is the dual basis of $ (e_t^*) $ in $ E^{**} $ and, as $ c_E $ transforms a basis of E into a basis of $ E^{**} $, $ c_E $ is bijective (\S 1, no. 11, Corollary 3 to Proposition 17). We have moreover proved:

#### Corollary 1 {#alg-ii-s2-prop-13-cor-1 .statement}

*Let E be a free A-module with a finite basis; for every basis* $ (e_t) $ *of E, $ (c_E(e_t)) $ *is the dual basis of the basis* $ (e_t^*) $ *of* $ E^* $ *dual to* $ (e_t) $.

In this case it is said that $ (e_t) $ and $ (e_t^*) $ are two *dual bases of one another*.

#### Corollary 2 {#alg-ii-s2-prop-13-cor-2 .statement}

*If E is a free A-module with a finite basis, every finite basis of E* is the dual basis of a basis of E.*

It suffices to consider in E** the dual basis of the given basis and canonically to identify E with E**.

#### Corollary 3 {#alg-ii-s2-prop-13-cor-3 .statement}

*Let E, F be two A-modules each with a finite basis, E (resp. F) being canonically identified with its bidual E** (resp. F**). Then, for every linear mapping u : E → F, $ t^t u = u $.*

This follows immediately from the commutativity of diagram (27).

#### Corollary 4 {#alg-ii-s2-prop-13-cor-4 .statement}

*If P is a projective module (resp. a finitely generated projective module) the canonical mapping $ c_P : P \to P** $ is injective (resp. bijective).*

We shall use the following lemma:

#### Lemma 1 {#alg-ii-s2-lem-1 .statement}

*Let M, N be two supplementary submodules in an A-module E and i : M → E, j : N → E the canonical injections. Then the diagram*

$$
\begin{array}{ccc}
M \oplus N & \xrightarrow{c_M \oplus c_N} & M** \oplus N** \\
i + j \downarrow & & \uparrow t_{i_1} + t_{j_1} \\
E & \xrightarrow{c_E} & E**
\end{array}
$$

(28)

*is commutative.*

By definition, for $ x \in M, y \in N, z^* \in E* $,

$$
\begin{align*}
\langle c_E(i(x) + j(y)), z^* \rangle &= \langle i(x) + j(y), z^* \rangle \\
&= \langle i(x), z^* \rangle + \langle j(y), z^* \rangle \\
&= \langle x, t_i(z^*) \rangle + \langle y, t_j(z^*) \rangle \\
&= \langle c_M(x), t_i(z^*) \rangle + \langle c_N(y), t_j(z^*) \rangle \\
&= \langle t_i(c_M(x)) + t_j(c_N(y)), z^* \rangle.
\end{align*}
$$

This being so, if E is a free module (resp. a free module with a finite basis), $ c_E $ is injective (resp. bijective); on the other hand, it follows from no. 6, Proposition 10, that $ t_i \oplus t_j $ is bijective; the commutativity of diagram (28) then implies that $ c_M \oplus c_N $ is injective (resp. bijective) and so therefore are $ c_M $ and $ c_N $ (\S 1, no. 6, Corollary 1 to Proposition 7), whence the corollary, taking account of no. 2, Proposition 4.

### 8. LINEAR EQUATIONS

Let E, F be two A-modules. Every equation of the form $ u(x) = y_0 $, where $ u : E \to F $ is a given linear mapping, $ y_0 $ a given element of F and the unknown $ x $ is subjected to the condition that it take its values in E, is called a *linear* equation; $ y_0 $ is called the right hand side of the equation; if $ y_0 = 0 $, the equation is called homogeneous linear.

Every element $ x_0 \in E $ such that $ u(x_0) = y_0 $ is called a solution of the linear equation $ u(x) = y_0 $.†

It is often said, loosely speaking, that a problem is linear if it is equivalent to determining the solutions of a linear equation.

Given a linear equation $ u(x) = y_0 $, the equation $ u(x) = 0 $ is called the homogeneous linear equation associated with $ u(x) = y_0 $.

#### Proposition 14 {#alg-ii-s2-prop-14 .statement}

*If $ x_0 $ is a solution of the linear equation $ u(x) = y_0 $, the set of solutions of this equation is equal to the set of elements $ x_0 + z $, where $ z $ runs through the set of solutions of the associated homogeneous equation $ u(x) = 0 $.*

The relation $ u(x) = y_0 $ may be written as $ u(x) = u(x_0) $, which is equivalent to $ u(x - x_0) = 0 $.

In other words, if the equation $ u(x) = y_0 $ has at least one solution $ x_0 $, the set of its solutions is the set $ x_0 + \overline{u}(0) $, obtained by translation from the kernel $ \overline{u}(0) $ of $ u $. Observe that $ \overline{u}(0) $, being a submodule, is never empty, since it contains 0 (called the zero solution, or trivial solution, of the homogeneous equation $ u(x) = 0 $).

By virtue of Proposition 14, for a linear equation $ u(x) = y_0 $ to have *exactly one solution*, it is necessary and sufficient that it have at least one solution and that $ \overline{u}(0) = \{0\} $ (in other words, that the associated homogeneous equation have no non-zero solution, or also that $ u $ be *injective*); in this case, for *all* $ y \in F $, the equation $ u(x) = y $ has *at most* one solution.

#### Proposition 15 {#alg-ii-s2-prop-15 .statement}

*Let $ u $ be a linear mapping of a module $ E $ into a module $ F $. If the equation $ u(x) = y_0 $ has at least one solution, $ y_0 $ is orthogonal to the kernel of $ ^t u $.*

To say that $ u(x) = y_0 $ admits a solution means that $ y_0 \in u(E) $ and the proposition follows from no. 5, Corollary to Proposition 8.

† This is in fact an abuse of language; from the logical point of view, we are not here defining the word "solution", but simply the sentence "$ x_0 $ is a solution of the equation $ u(x) = y_0 $" as equivalent to the relation "$ x_0 \in E $ and $ u(x_0) = y_0 $". Observe that in a mathematical theory $ \mathcal{T} $ where the relation "$ A $ is a ring, $ E $ and $ F $ are $ A $-modules, $ u $ is a homomorphism of $ E $ into $ F $, $ y_0 $ an element of $ F $" is a theorem, every *term* $ T $ of $ \mathcal{T} $ such that the relation "$ T \in E $ and $ u(T) = y_0 $" is true in $ \mathcal{T} $ is a *solution* of the equation $ u(x) = y_0 $ in the sense of *Set Theory*, I, § 5, no. 2; this justifies the above abuse of language.

Observe that the necessary criterion for the existence of a solution of $ u(x) = y_0 $, given by Proposition 15, is sufficient when $ A $ is a field (\S 7, no. 6, Proposition 12), but *not in general* (Exercise 10).

#### Remark {#alg-ii-s2-n8-rem-1 .statement}

(1) Let $ E $ be an $ A $-module, $ (F_i)_{i \in I} $ a family of $ A $-modules and for all $ i \in I $ let $ u_i : E \to F_i $ be a linear mapping. Every system of linear equations
$$
u_i(x) = y_i \quad (i \in I)
$$
where the $ y_i \in F_i $ are given, is equivalent to *a single* linear equation $ u(x) = y $, where $ u $ is the mapping $ x \mapsto (u_i(x)) $ of $ E $ into $ F = \prod_{i \in I} F_i $ and $ y = (y_i) $. The system (29) is called *homogeneous* if $ y_i = 0 $ for all $ i \in I $.

(2) Suppose that $ E $ admits a *basis* $ (a_\lambda)_{\lambda \in L} $; if we set $ u(a_\lambda) = b_\lambda $ for all $ \lambda \in L $, to say that $ x = \sum_{\lambda \in L} \xi_\lambda a_\lambda $ satisfies the equation $ u(x) = y_0 $ is equivalent to saying that the family (of finite support) $ (\xi_\lambda)_{\lambda \in L} $ of elements of $ A $ satisfies the relation
$$
\sum_{\lambda \in L} \xi_\lambda b_\lambda = y_0.
$$

Conversely, looking for families $ (\xi_\lambda)_{\lambda \in L} $ of elements of $ A $ of finite support satisfying (30), is equivalent to solving the linear equation $ u(x) = y_0 $, where $ u $ is the unique linear mapping of $ E $ into $ F $ such that $ u(a_\lambda) = b_\lambda $ for all $ \lambda \in L $ (\S 1, no. 11, Corollary 3 to Proposition 17).

(3) A linear equation $ u(x) = y_0 $ is called *scalar* when $ F = A_s $ and therefore $ u $ is a *linear form* on $ E $ and $ y_0 $ a *scalar*. If $ E $ admits a basis $ (a_\lambda)_{\lambda \in L} $, it follows from *Remark* (2) that such an equation may also be written as
$$
\sum_{\lambda \in L} \xi_\lambda \alpha_\lambda = y_0 \in A
$$
where the family of scalars $ (\alpha_\lambda) $ is arbitrary and where it is understood that the family $ (\xi_\lambda) $ must have finite support. In general, by the *solution* (in $ A $) of a system of scalar linear equations
$$
\sum_{\lambda \in L} \xi_\lambda \alpha_{\lambda_i} = \eta_i \quad (i \in I)
$$
where $ \alpha_{\lambda_i} \in A $ and $ \eta_i \in A $, is understood a family $ (\xi_\lambda)_{\lambda \in L} $ of elements of $ A $ of *finite* support and satisfying (32); the $ \alpha_{\lambda_i} $ are called the *coefficients* of the system of equations and the $ \eta_i $ the *right hand sides*. The solution of such a system is equivalent to that of the equation $ u(x) = y $, where $ y = (\eta_i) $ and $ u : A_s^{(L)} \to A_s^I $ is the linear mapping
$$
(\xi_\lambda) \mapsto \left( \sum_{\lambda \in L} \xi_\lambda \alpha_{\lambda_i} \right).
$$

(4) A linear system (32) is also called a *system of left scalar linear equations* when it is necessary to avoid confusion. A system of equations
$$
\sum_{\lambda \in L} \alpha_{\lambda_i} \xi_\lambda = \eta_i \quad (i \in I)
$$

is likewise called a system of right scalar linear equations; such a system can immediately be transformed into a system (32) by considering the $ \xi_{\lambda}, \eta_i $ and $ \alpha_{\lambda_i} $ as belonging to the opposite ring $ A^0 $ to A.

### Exercises {#alg-ii-s2-exercises}

See the [exercises for § 2](exercises/s2/).
