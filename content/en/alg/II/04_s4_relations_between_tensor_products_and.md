---
book: alg
book_title: Algebra
chapter: II
chapter_title: LINEAR ALGEBRA
section: 4
section_title: Relations between tensor products and homomorphism modules
lang: en
source: alg-i-iii
source_edition: 1998, Springer
pdf_pages: 0291-0300, 0420-0422
extraction: ocr
subsections:
    - "no": 1
      title: THE ISOMORPHISMS $ \operatorname{Hom}_B(E \otimes_A F, G) \to \operatorname{Hom}_A(F, \operatorname{Hom}_B(E, G)) $ AND $ \operatorname{Hom}_c(E \otimes_A F, G) \to \operatorname{Hom}_A(E, \operatorname{Hom}_c(F, G)) $
      page: 0
      pdf_page: 291
    - "no": 2
      title: THE HOMOMORPHISM** $ E^* \otimes_A F \to \mathrm{Hom}_A(E, F) $
      page: 0
      pdf_page: 292
    - "no": 3
      title: TRACE OF AN ENDOMORPHISM
      page: 0
      pdf_page: 297
    - "no": 4
      title: THE HOMOMORPHISM $\operatorname{Hom}_c(E_1, F_1) \otimes_c \operatorname{Hom}_c(E_2, F_2) \to \operatorname{Hom}_c(E_1 \otimes_c E_2, F_1 \otimes_c F_2)$
      page: 0
      pdf_page: 298
statements: 15
exercises: 9
content_sha256: b9c301046b44f9223afedd5ec05acb598f0ddabb1140f8edcfc362bcf970fd1d
---

## § 4. RELATIONS BETWEEN TENSOR PRODUCTS AND HOMOMORPHISM MODULES

### 1. THE ISOMORPHISMS $ \operatorname{Hom}_B(E \otimes_A F, G) \to \operatorname{Hom}_A(F, \operatorname{Hom}_B(E, G)) $ AND $ \operatorname{Hom}_c(E \otimes_A F, G) \to \operatorname{Hom}_A(E, \operatorname{Hom}_c(F, G)) $

Let E be a right A-module, F a left A-module, G a $ \mathbf{Z} $-module and H the $ \mathbf{Z} $-module of mappings $ f : E \times F \to G $ which are $ \mathbf{Z} $-bilinear and satisfy

(1)
$$
f(x \lambda, y) = f(x, \lambda y) \quad \text{for } x \in E, y \in F, \lambda \in A.
$$

It has been seen (\S 3, no. 1, Proposition 1) that there exists a canonical $ \mathbf{Z} $-module homomorphism

(2)
$$
H \to \operatorname{Hom}_{\mathbf{Z}}(E \otimes_A F, G).
$$

On the other hand, a left A-module structure has been defined on $ \operatorname{Hom}_{\mathbf{Z}}(E, G) $ and a right A-module structure on $ \operatorname{Hom}_{\mathbf{Z}}(F, G) $ (\S 3, no. 3); we may therefore consider the $ \mathbf{Z} $-modules $ \operatorname{Hom}_A(E, \operatorname{Hom}_{\mathbf{Z}}(F, G)) $ and $ \operatorname{Hom}_A(F, \operatorname{Hom}_{\mathbf{Z}}(E, G)) $. A mapping $ f $ of $ E \times F $ into G is canonically identified with a mapping of E into the set $ G^F $ of mappings of F into G (*Set Theory*, II, \S 5, no. 2); by expressing the fact that the latter mapping belongs to $ \operatorname{Hom}_A(E, \operatorname{Hom}_{\mathbf{Z}}(F, G)) $, we obtain precisely the fact that $ f $ is biadditive and conditions (1); whence there is a canonical isomorphism

(3)
$$
H \to \operatorname{Hom}_A(E, \operatorname{Hom}_{\mathbf{Z}}(F, G))
$$
and similarly there is defined a canonical isomorphism

(4)
$$
H \to \operatorname{Hom}_A(F, \operatorname{Hom}_{\mathbf{Z}}(E, G)).
$$

Suppose now that E and G also have left (resp. right) B-module structures and that the A-module and B-module structures on E are compatible. Then $ E \otimes_A F $ has canonically a left (resp. right) B-module structure (\S 3, no. 4) and on the other hand $ \operatorname{Hom}_B(E, G) $ has canonically a left A-module structure (\S 1, no. 14). We may therefore consider the $ \mathbf{Z} $-modules $ \operatorname{Hom}_B(E \otimes_A F, G) $ and $ \operatorname{Hom}_A(F, \operatorname{Hom}_B(E, G)) $, which are submodules of $ \operatorname{Hom}_{\mathbf{Z}}(E \otimes_A F, G) $ and $ \operatorname{Hom}_A(F, \operatorname{Hom}_{\mathbf{Z}}(E, G)) $ respectively (\S 2, no. 1, Theorem 2). We examine under what condition a mapping $ f \in H $ has as image under the isomorphisms (2) and (4) an element of $ \operatorname{Hom}_B(E \otimes_A F, G) $ and an element of $ \operatorname{Hom}_A(E, \operatorname{Hom}_B(F, G)) $ respectively; in each of the two cases we find the *same* condition

$$
f(\beta x, y) = \beta f(x, y)
$$
(resp. $ f(x \beta, y) = f(x, y) \beta $)

for $ x \in E, y \in F, \beta \in B $.

Similarly, suppose that F and G are left (resp. right) C-modules and that the A-module and C-module structures on F are compatible. Then, for a mapping $ f \in H $ to have as image under (2) or (3) an element of $ \mathrm{Hom}_C(E \otimes_A F, G) $ or $ \mathrm{Hom}_A(E, \mathrm{Hom}_C(F, G)) $ respectively, it is necessary and sufficient that it satisfy the same condition

$$
f(x, \gamma y) = \gamma f(x, y)
$$
(resp. $ f(x, y \gamma) = f(x, y) \gamma $)

for $ x \in E, y \in F, \gamma \in C $.

We have therefore established the following result (in the notation introduced above):

#### Proposition 1 {#alg-ii-s4-prop-1 .statement}

(a) *Let E be a (B, A)-bimodule, F a left A-module and G a left B-module. For every mapping $ g \in \mathrm{Hom}_B(E \otimes_A F, G) $, let $ g' $ be the mapping of F into $ \mathrm{Hom}_B(E, G) $ defined by $ (g'(y))(x) = g(x \otimes y) $ for $ x \in E, y \in F $. The mapping $ g \mapsto g' $ is an isomorphism*

(5)
$$
\beta : \mathrm{Hom}_B(E \otimes_A F, G) \to \mathrm{Hom}_A(F, \mathrm{Hom}_B(E, G)).
$$

(b) *Let E be a right A-module, F an (A, C)-bimodule and G a right C-module. For every mapping $ h \in \mathrm{Hom}_C(E \otimes_A F, G) $, let $ h' $ be the mapping of E into $ \mathrm{Hom}_C(F, G) $ defined by $ (h'(x))(y) = h(x \otimes y) $ for $ x \in E, y \in F $. The mapping $ h \mapsto h' $ is an isomorphism*

(6)
$$
\gamma : \mathrm{Hom}_C(E \otimes_A F, G) \to \mathrm{Hom}_A(E, \mathrm{Hom}_C(F, G)).
$$

In particular B and C may be taken to be a subring $ \Gamma $ of the centre of the ring A; then for every $ \Gamma $-module G, the three $ \Gamma $-modules

$$
\mathrm{Hom}_\Gamma(E \otimes_A F, G), \quad \mathrm{Hom}_A(E, \mathrm{Hom}_\Gamma(F, G)), \quad \mathrm{Hom}_A(F, \mathrm{Hom}_\Gamma(E, G))
$$

are canonically isomorphic to the $ \Gamma $-module of $ \Gamma $-*bilinear* mappings of $ E \times F $ into G which satisfy (1). More particularly:

#### Corollary {#alg-ii-s4-n1-cor-1 .statement}

*If C is a commutative ring and E, F, G three C-modules, then the C-modules*
$$
\mathrm{Hom}_C(E \otimes_C F, G), \qquad \mathrm{Hom}_C(E, \mathrm{Hom}_C(F, G)),
$$
$$
\mathrm{Hom}_C(F, \mathrm{Hom}_C(E, G)), \qquad \mathcal{L}_2(E, F; G)
$$
*are canonically isomorphic.*

### 2. THE HOMOMORPHISM** $ E^* \otimes_A F \to \mathrm{Hom}_A(E, F) $

Let A, B be two rings, E a left A-module, F a left B-module and G an (A, B)-*bimodule*. The $ \mathbf{Z} $-module $ \mathrm{Hom}_A(E, G) $ has canonically a *right* B-*module* structure (\S 1, no. 14) such that $(u\beta)(x) = u(x)\beta$ for $\beta \in B$, $u \in \mathrm{Hom}_A(E, G)$, $x \in E$. On the other hand, $G \otimes_B F$ has canonically a *left A-module* structure (\S 3, no. 4). We shall define a *canonical $\mathbf{Z}$-homomorphism*

$$
\nu : \mathrm{Hom}_A(E, G) \otimes_B F \to \mathrm{Hom}_A(E, G \otimes_B F).
$$

To this end, we consider, for all $y \in F$ and all $u \in \mathrm{Hom}_A(E, G)$, the mapping $\nu'(u, y) : x \mapsto u(x) \otimes y$ of $E$ onto $G \otimes_B F$. It is immediately verified that $\nu'(u, y)$ is $A$-linear and that $\nu'$ is a $\mathbf{Z}$-bilinear mapping of $\mathrm{Hom}_A(E, G) \times F$ into $\mathrm{Hom}_A(E, G \otimes_B F)$; moreover, for all $\beta \in B$, $\nu'(u\beta, y)$ and $\nu'(u, \beta y)$ are equal, for $(u(x)\beta) \otimes y = u(x) \otimes (\beta y)$. We conclude (\S 3, no. 1, Proposition 1) the existence of the desired homomorphism $\nu$ such that $\nu(u \otimes y)$ is the $A$-linear mapping $x \mapsto u(x) \otimes y$.

It is immediately verified that, if $E$ is an $(A, (C'_i); (D'_j))$-multimodule, $F$ a $(B, (C''_h); (D''_k))$-multimodule and $G$ an $(A, (C'''_1); B, (D'''_m))$-multimodule, the mapping (7) is a $((D'_j), (C''_h), (C'''_1); (C'_i), (D''_k), (D'''_m))$-multimodule homomorphism.

#### Proposition 2 {#alg-ii-s4-prop-2 .statement}

(i) *When $F$ is a projective* (resp. *finitely generated projective*) *B-module, the canonical homomorphism (7) is injective* (resp. *bijective*).

(ii) *When $E$ is a finitely generated projective $A$-module, the canonical homomorphism (7) is bijective*.

(i) Fixing $E$ and $G$, for *every* left $B$-module $F$, we write

$$
T(F) = \mathrm{Hom}_A(E, G) \otimes_B F, \quad T'(F) = \mathrm{Hom}_A(E, G \otimes_B F);
$$

for every left $B$-module homomorphism $u : F \to F'$, we write $T(u) = 1 \otimes u$ (1 here denoting the identity mapping of $\mathrm{Hom}_A(E, G)$),

$$
T'(u) = \mathrm{Hom}(1_E, 1_G \otimes u);
$$

on the other hand we write $\nu_F$ instead of $\nu$. Then we have the following lemmas:

#### Lemma 1 {#alg-ii-s4-lem-1 .statement}

*For every homomorphism $u : F \to F'$, the diagram*

$$
\begin{array}{ccc}
T(F) & \xrightarrow{\nu_F} & T'(F) \\
\downarrow T(u) & & \downarrow T'(u) \\
T(F') & \xrightarrow{\nu_{F'}} & T'(F')
\end{array}
$$

is *commutative*.

The verification is immediate.

#### Lemma 2 {#alg-ii-s4-lem-2 .statement}

Let $ M, N $ be two supplementary submodules in $ F $ and $ i : M \to F, j : N \to F $ the canonical injections. The diagram

$$
\begin{array}{ccc}
T(M) \oplus T(N) & \xrightarrow{\nu_M \oplus \nu_N} & T'(M) \oplus T'(N) \\
\downarrow T(i) + T(j) & & \downarrow T'(i) + T'(j) \\
T(F) & \xrightarrow{\nu_F} & T'(F)
\end{array}
$$

is commutative and the vertical arrows are bijective.

The commutativity follows from Lemma 1, the other assertions from § 1, no. 6, Corollary 2 to Proposition 6 and § 3, no. 7, Proposition 7.

#### Lemma 3 {#alg-ii-s4-lem-3 .statement}

Under the hypotheses of Lemma 2, for $ \nu_F $ to be injective (resp. surjective), it is necessary and sufficient that $ \nu_M $ and $ \nu_N $ be so.

This follows from Lemma 2 and § 1, no. 6, Corollary 1 to Proposition 6.

Then Lemma 3, together with § 2, no. 2, Proposition 4, shows that it suffices to consider the case where $ F $ is a free module. But, if $ (b_\mu) $ is a basis of $ F $, every element of $ \mathrm{Hom}_A(E, G) \otimes_B F $ may then be written uniquely as $ \sum_\mu u_\mu \otimes b_\mu $, where $ u_\mu \in \mathrm{Hom}_A(E, G) $ (\S 3, no. 7, Corollary 1 to Proposition 7); the image of this element under $ \nu $ is the $ A $-linear mapping $ x \mapsto \sum_\mu u_\mu(x) \otimes b_\mu $; it cannot be zero for all $ x \in E $ unless $ u_\mu(x) = 0 $ for all $ x \in E $ and all $ \mu $, which is equivalent to saying that $ u_\mu = 0 $ for all $ \mu $; hence $ \nu $ is injective. When also $ F $ admits a finite basis, Lemma 3 shows (by induction on the number of elements in the basis of $ F $) that to prove that $ \nu $ is surjective, it suffices to do so when $ F = B_s $; but in this case the two sides of (7) are canonically identified with $ \mathrm{Hom}_A(E, G) $ (\S 3, no. 4, Proposition 4) and $ \nu $ becomes the identity.

(ii) To show the proposition when $ E $ is projective and finitely generated, this time we fix $ F $ and $ G $ and write, for every left $ A $-module $ E $,

$$
T(E) = \mathrm{Hom}_A(E, G) \otimes_B F, \qquad T'(E) = \mathrm{Hom}_A(E, G \otimes_B F)
$$

and, for every left $ A $-module homomorphism $ v : E \to E' $,

$$
T(v) = \mathrm{Hom}(v, 1_G) \otimes 1_F, \qquad T'(v) = \mathrm{Hom}(v, 1_G \otimes 1_F);
$$

on the other hand, we write $ \nu_E $ instead of $ \nu $. Then we have the two lemmas:

#### Lemma 4 {#alg-ii-s4-lem-4 .statement}

For every homomorphism $ v : E \to E' $, the diagram

$$
\begin{array}{ccc}
T(E') & \xrightarrow{\nu_{E'}} & T'(E') \\
\downarrow T(v) & & \downarrow T'(v) \\
T(E) & \xrightarrow{\nu_E} & T'(E)
\end{array}
$$

is commutative.

#### Lemma 5 {#alg-ii-s4-lem-5 .statement}

Let $ M $ and $ N $ be two supplementary submodules in $ E $ and $ p : E \to M, q : E \to N $ the canonical projections. The diagram

$$
\begin{array}{ccc}
T(M) \oplus T(N) & \xrightarrow{\nu_M \oplus \nu_N} & T'(M) \oplus T'(N) \\
\downarrow T(p) + T(q) & & \downarrow T'(p) + T'(q) \\
T(E) & \xrightarrow{\nu_E} & T'(E)
\end{array}
$$

is commutative and the vertical arrows are bijective.

They are proved as Lemmas 1 and 2, taking account of § 1, no. 6, Corollary 2 to Proposition 6, § 2, no. 1, Proposition 1 and § 3, no. 7, Proposition 7.

The remainder of the proof then proceeds as in (i) and is reduced to the case where $ E = A_s $; the two sides of (7) are then canonically identified with $ G \otimes_B F $ and $ \nu $ becomes the identity.

In particular take $ B = A $ and $ G $ the $(A, A)$-bimodule $ {}_sA_d $ ($ \S 3 $, no. 4), so that the right $ A $-module $ \mathrm{Hom}_A(E, {}_sA_d) $ is just the dual $ E^* $ of $ E $ and $ ({}_sA_d) \otimes_A F $ is canonically identified with $ F $ ($ \S 3 $, no. 4, Proposition 4). Homomorphism (7) then becomes a canonical $ \mathbf{Z} $-homomorphism

$$(11)$$
$$
\theta : E^* \otimes_A F \to \mathrm{Hom}_A(E, F)
$$
and $ \theta(x^* \otimes y) $ is the linear mapping of $ E $ into $ F $
$$
x \mapsto \langle x, x^* \rangle y.
$$

Remark (1). The characterization of *projective* $ A $-modules given in $ \S 2 $, no. 6, Proposition 12, can also be expressed as follows: for a left $ A $-module $ E $ to be projective, it is necessary and sufficient that the canonical homomorphism
$$
\theta_E : E^* \otimes_A E \to \mathrm{Hom}_A(E, E) = \mathrm{End}_A(E)
$$
be such that $ 1_E $ belongs to the image of $ \theta_E $.

#### Corollary {#alg-ii-s4-n2-cor-1 .statement}

(i) *When $ F $ is a projective* (resp. *finitely generated projective*) *module, the canonical homomorphism* (11) *is injective* (resp. *bijective*).
(ii) *When $ E $ is a finitely generated projective module, the canonical homomorphism* (11) *is bijective*.

Even when $ E $ and $ F $ are both finitely generated, $ \theta $ is not necessarily surjective, as is shown by the example $ A = \mathbf{Z}, E = F = \mathbf{Z}/2\mathbf{Z} $; the right hand side of (11) is non-zero but $ E^* = 0 $. On the other hand, examples can be given where $ E $ is *free*, but (11) is neither injective nor surjective (Exercise 3(b)).

When E admits a finite basis $(e_i)$, the inverse isomorphism $\theta^{-1}$ of $\theta$ can be found explicitly as follows. Let $(e_i^*)$ be the dual basis of $(e_i)$ (\S 2, no. 6); for all $u \in \mathrm{Hom}(E, F)$ and all $x = \sum_i \xi_i e_i$ with $\xi_i \in A$,

$$
u(x) = \sum_i \xi_i u(e_i) = \sum_i \langle x, e_i^* \rangle u(e_i)
$$

and therefore $u = \sum_i \theta(e_i^* \otimes u(e_i))$, in other words

$$
\theta^{-1}(u) = \sum_i e_i^* \otimes u(e_i).
$$

In particular, if further $F = E$, it is seen that the image under $\theta_E^{-1}$ of the identity mapping $1_E$ is the element $\sum_i e_i^* \otimes e_i$, which is therefore *independent* of the basis $(e_i)$ considered in E.

Note on the other hand that when E is a finitely generated projective module the *ring* structure on $\mathrm{End}_A(E)$ can be transported by $\theta_E^{-1}$ to $E^* \otimes_A E$; it is immediately verified that, for $x, y$ in E, $x^*, y^*$ in $E^*$, in the ring $\mathrm{End}_A(E)$,

$$
\theta_E(x^* \otimes x) \circ \theta_E(y^* \otimes y) = \theta_E((y^* \langle y, x^* \rangle) \otimes x).
$$

*Remark* (2). Let E be a *right* A-module; replacing E by $E^*$ in (11), we obtain a canonical $\mathbf{Z}$-homomorphism

$$
E^{**} \otimes_A F \to \mathrm{Hom}_A(E^*, F).
$$

On the other hand, there is a canonical A-homomorphism $c_E : E \to E^{**}$, whence there is a $\mathbf{Z}$-homomorphism $c_E \otimes 1_F : E \otimes_A F \to E^{**} \otimes_A F$; composing the latter with the homomorphism (14), we hence obtain a canonical $\mathbf{Z}$-homomorphism

$$
\theta' : E \otimes_A F \to \mathrm{Hom}_A(E^*, F)
$$

such that $\theta'(x \otimes y)$ is the linear mapping

$$
x^* \mapsto \langle x, x^* \rangle y.
$$

If E *and* F are *projective* modules, the mapping (15) is *injective*. For $c_E$ is then injective (\S 2, no. 7, Corollary 4 to Proposition 13) and as F is projective, the $\mathbf{Z}$-homomorphism $c_E \otimes 1_F : E \otimes_A F \to E^{**} \otimes_A F$ is also injective (\S 3, no. 7, Corollary 6 to Proposition 7); finally, it has been seen (Proposition 2) that the homomorphism (14) is injective, whence the conclusion.

If E is *projective* and *finitely generated*, the mapping (15) is *bijective* for the two mappings of which it is composed are then bijective (\S 2, no. 7, Corollary 4 to Proposition 13 and Proposition 2 above).

### 3. TRACE OF AN ENDOMORPHISM

Let $ C $ be a *commutative* ring and $ E $ a $ C $-module. The mapping $ (x^*, x) \mapsto \langle x, x^* \rangle $ of $ E^* \times E $ into $ C $ is then $ C $*-bilinear*, since, for all $ \gamma \in C $, $ \langle \gamma x, x^* \rangle = \gamma \langle x, x^* \rangle $ and $ \langle x, x^* \gamma \rangle = \langle x, x^* \rangle \gamma $; we derive a canonical $ C $*-linear* mapping

$$
\tau : E^* \otimes_C E \to C
$$

such that $ \tau(x^* \otimes x) = \langle x, x^* \rangle $ (\S 3, no. 5). Suppose now also that $ E $ is a *finitely generated projective* $ C $-module; the canonical isomorphism (11) of no. 2 is then a $ C $*-module* isomorphism and we can therefore define by transporting the structure a *canonical linear form* $ \mathrm{Tr} = \tau \circ \theta_E^{-1} $ on the $ C $-module $ \mathrm{End}_C(E) $. For all $ u \in \mathrm{End}_C(E) $ the scalar $ \mathrm{Tr}(u) $ is called the *trace* of the endomorphism $ u $; every $ u \in \mathrm{End}_C(E) $ can be written (in general in an infinity of ways) in the form $ x \mapsto \sum_i \langle x, x_i^* \rangle y_i $ where $ x_i^* \in E^* $ and $ y_i \in E_i $ by virtue of no. 2, Corollary to Proposition 2; then

$$
\mathrm{Tr}(u) = \sum_i \langle y_i, x_i^* \rangle \quad \text{(cf. \S 10, no. 11).}
$$

By definition,

$$
\mathrm{Tr}(u + v) = \mathrm{Tr}(u) + \mathrm{Tr}(v)
$$
$$
\mathrm{Tr}(\gamma u) = \gamma \mathrm{Tr}(u)
$$

for $ u, v $ in $ \mathrm{End}_C(E) $ and $ \gamma \in C $. Moreover:

#### Proposition 3 {#alg-ii-s4-prop-3 .statement}

*Let $ C $ be a commutative ring, $ E, F $ two finitely generated projective $ C $*-modules* and $ u : E \to F $ and $ v : F \to E $ two linear mappings; then*

$$
\mathrm{Tr}(v \circ u) = \mathrm{Tr}(u \circ v).
$$

The two mappings $ (u, v) \mapsto \mathrm{Tr}(u \circ v), (u, v) \mapsto \mathrm{Tr}(v \circ u) $ of

$$
\mathrm{Hom}_C(E, F) \times \mathrm{Hom}_C(F, E)
$$

into $ C $ are $ C $*-bilinear*; it therefore suffices to verify (20) when $ u $ is of the form $ x \mapsto \langle x, a^* \rangle b $ and $ v $ of the form $ y \mapsto \langle y, b^* \rangle a $, with $ a \in E, a^* \in E^*, b \in F, b^* \in F^* $. But then $ v \circ u $ is the mapping $ x \mapsto \langle x, a^* \rangle \langle b, b^* \rangle a $ and $ u \circ v $ the mapping $ y \mapsto \langle y, b^* \rangle \langle a, a^* \rangle b $. Formula (17) shows that the values of the two sides of (20) are equal to $ \langle a, a^* \rangle \langle b, b^* \rangle $.

#### Corollary {#alg-ii-s4-n3-cor-1 .statement}

*If $ u_1, \ldots, u_p $ are endomorphisms of $ E $, then*

$$
\mathrm{Tr}(u_1 \circ u_2 \circ \cdots \circ u_p) = \mathrm{Tr}(u_i \circ u_{i+1} \circ \cdots \circ u_p \circ u_1 \circ \cdots \circ u_{i-1})
$$

*for* $ 1 \leq i \leq p $ ("invariance of the trace under cyclic permutation").

It suffices to apply (20) to the product

$$(u_1 \circ u_2 \circ \cdots \circ u_{i-1}) \circ (u_i \circ u_{i+1} \circ \cdots \circ u_p).$$

Note that on the other hand it is not necessarily true that

$$\operatorname{Tr}(u \circ v \circ w) = \operatorname{Tr}(u \circ w \circ v)$$

for three endomorphisms $u, v, w$ of E.

### 4. THE HOMOMORPHISM $\operatorname{Hom}_c(E_1, F_1) \otimes_c \operatorname{Hom}_c(E_2, F_2) \to \operatorname{Hom}_c(E_1 \otimes_c E_2, F_1 \otimes_c F_2)$

Let C be a *commutative* ring and $E_1, E_2, F_1, F_2$ four C-modules; in § 3, no. 5, formula (13) we defined a canonical C-module homomorphism

(21) $\lambda : \operatorname{Hom}(E_1, F_1) \otimes \operatorname{Hom}(E_2, F_2) \to \operatorname{Hom}(E_1 \otimes E_2, F_1 \otimes F_2)$.

#### Proposition 4 {#alg-ii-s4-prop-4 .statement}

*When one of the ordered pairs* $(E_1, E_2), (E_1, F_1), (E_2, F_2)$ *consists of finitely generated projective C-modules, the canonical homomorphism* (21) *is bijective.*

It is obviously sufficient to perform the proof for the ordered pairs $(E_1, F_1)$ and $(E_1, E_2)$.

We consider first the case of the ordered pair $(E_1, F_1)$; we fix $E_2, F_1, F_2$ and write for *every* C-module $T(E) = \operatorname{Hom}(E, F_1) \otimes_c \operatorname{Hom}(E_2, F_2)$ and $T'(E) = \operatorname{Hom}(E \otimes E_2, F_1 \otimes F_2)$ and, for every C-homomorphism $v : E \to E'$,

$$T(v) = \operatorname{Hom}(v, 1_{F_1}) \otimes 1_{\operatorname{Hom}(E_2, F_2)}$$

and

$$T'(v) = \operatorname{Hom}(v \otimes 1_{E_2}, 1_{F_1 \otimes F_2}).$$

Then *Lemmas 4 and 5* (no. 2) (*where v* is replaced by $\lambda$) *are valid* and are proved by completely analogous methods.

We next fix $E_2$ and $F_2$ and this time write, for every C-module F,

$$T(F) = \operatorname{Hom}(C, F) \otimes_c \operatorname{Hom}(E_2, F_2)$$ and $T'(F) = \operatorname{Hom}(C \otimes E_2, F \otimes F_2)$ and, for every C-homomorphism $u : F \to F'$,

$$T(u) = \operatorname{Hom}(1_C, u) \otimes 1_{\operatorname{Hom}(E_2, F_2)}$$

and

$$T'(u) = \operatorname{Hom}(1_C \otimes 1_{E_2}, u \otimes 1_{F_2}).$$

This time it is immediately verified that *Lemmas 1 and 2* (no. 2) (*where $\lambda$ always replaces v*) *are valid*.

This being so, we show the proposition first when $E_1 = C$ and $F_1$ is projective and finitely generated. The argument of no. 2 (which rests on Lemmas 1 and 2), together with the above remarks, reduces this to proving the proposition when also $F_1 = C$; then $\operatorname{Hom}(E_1, F_1), E_1 \otimes E_2$ and $F_1 \otimes F_2$ are identified with C, $E_2$ and $F_2$ respectively (\S 3, no. 4, Proposition 4); the two sides of (21)

THE HOMOMORPHISM $ \operatorname{Hom}_c(E_1, F_1) \otimes_c \operatorname{Hom}(E_2, F_2) $

are then both canonically identified with $ \operatorname{Hom}(E_2, F_2) $ and, after these identifications, it is verified that $ \lambda $ becomes the identity.

We now suppose that $ F_1 $ is projective and finitely generated; the argument of no. 2 (depending this time on Lemmas 4 and 5) reduces the proof for $ E_1 $ any finitely generated projective module to the case where $ E_1 = C $, that is to the first case dealt with.

For the ordered pair $ (E_1, E_2) $, the procedure is similar, this time applying Lemmas 4 and 5 twice; we leave the details to the reader.

Note that when $ E_1 = C^{(I)} $, $ E_2 = C^{(J)} $ are free (finitely generated or not), then $ \operatorname{Hom}(E_1, F_1) = F_1^I $, $ \operatorname{Hom}(E_2, F_2 = F_2^J $ and
$$
\operatorname{Hom}(E_1 \otimes E_2, F_1 \otimes F_2) = (F_1 \otimes F_2)^{I \times J}
$$
to within canonical isomorphisms and (21) is then identical with a special case of the canonical homomorphism (22) of § 3, no. 7.

When $ E_2 = C $, the canonical homomorphism (21) gives, after identifying $ \operatorname{Hom}(E_2, F_2) $ with $ F_2 $ and $ E_1 \otimes E_2 $ with $ E_1 $, a canonical homomorphism
$$
\operatorname{Hom}(E, F) \otimes G \to \operatorname{Hom}(E, F \otimes G)
$$
for any three $ C $-modules $ E, F, G $ which is just the homomorphism (7) of no. 2 for $ A = B = C $.

Note that when $ F = C $ the canonical homomorphism (22) again gives (11) (no. 2) for the case of a commutative ring.

Suppose now that $ F_1 = F_2 = C $; as $ F_1 \otimes F_2 $ is identified with $ C $, there is this time a canonical homomorphism
$$
\mu : E^* \otimes F^* \to (E \otimes F)^*
$$
for two $ C $-modules $ E, F $; for $ x^* \in E^*, y^* \in F^* $, the image of $ x^* \otimes y^* $ under the canonical homomorphism (23) is the linear form $ u $ on $ E \otimes F $ such that
$$
u(x \otimes y) = \langle x, x^* \rangle \langle y, y^* \rangle.
$$
Moreover, if $ E_1, E_2, F_1, F_2 $ are four $ C $-modules, $ f : E_1 \to E_2, g : F_1 \to F_2 $ two linear mappings, it follows immediately from (24) that the diagram
$$
\begin{array}{ccc}
E_2^* \otimes F_2^* & \xrightarrow{\mu} & (E_2 \otimes F_2)^* \\
t_f \otimes t_g \downarrow & & \downarrow t_{(f \otimes g)} \\
E_1^* \otimes F_1^* & \xrightarrow{\mu} & (E_1 \otimes F_1)^*
\end{array}
$$
is *commutative*.

#### Corollary 1 {#alg-ii-s4-prop-4-cor-1 .statement}

*If one of the modules E, F is projective and finitely generated, the canonical homomorphism (23) is bijective.*

#### Corollary 2 {#alg-ii-s4-prop-4-cor-2 .statement}

*Let E₁, E₂ be two finitely generated projective C-modules, u₁ an endomorphism of E₁ and u₂ an endomorphism of E₂; then*

$$
\text{Tr}(u₁ \otimes u₂) = \text{Tr}(u₁)\text{Tr}(u₂).
$$

By linearity, it suffices to consider the case where u₁ is of the form $ x₁ \mapsto \langle x₁, x₁^* \rangle y₁ $ and u₂ of the form $ x₂ \mapsto \langle x₂, x₂^* \rangle y₂ $; then the image of $ x₁ \otimes x₂ $ under $ u₁ \otimes u₂ $ is by definition

$$
\langle x₁, x₁^* \rangle \langle x₂, x₂^* \rangle (y₁ \otimes y₂) = \langle x₁ \otimes x₂, x₁^* \otimes x₂^* \rangle (y₁ \otimes y₂)
$$

$ x₁^* \otimes x₂^* $ being canonically identified under $ μ $ with an element of $ (E₁ \otimes E₂)^* $. As $ \langle y₁ \otimes y₂, x₁^* \otimes x₂^* \rangle = \langle y₁, x₁^* \rangle \langle y₂, x₂^* \rangle $, formula (26) follows in this case from (17).

#### Remark {#alg-ii-s4-n4-rem-1 .statement}

If E, F, G are any three C-modules, it is immediately verified that the diagram

$$
\begin{array}{ccc}
E^* \otimes F^* \otimes G^* & \xrightarrow{\mu \otimes 1} & (E \otimes F)^* \otimes G^* \\
1 \otimes \mu \downarrow & & \downarrow \mu \\
E^* \otimes (F \otimes G)^* & \xrightarrow{\mu} & (E \otimes F \otimes G)^*
\end{array}
$$

is *commutative*, by virtue of formula (24).

We note also that, without any hypothesis on the C-modules E, F, there are canonical *isomorphisms*

(28) $$(E \otimes F)^* \to \text{Hom}(E, F^*)$$
(29) $$(E \otimes F)^* \to \text{Hom}(F, E^*)$$

which are just the isomorphism (6) and (5) of no. 1 for G = C, A = B = C.

Thus a canonical one-to-one correspondence has been defined between the *bilinear forms* on E × F, the *homomorphisms of E into F* and the *homomorphisms of F into E*: if u (resp. v) is a homomorphism of E into F* (resp. of F into E*), the corresponding bilinear form is given by

$$(x, y) \mapsto \langle y, u(x) \rangle \quad (\text{resp. } (x, y) \mapsto \langle x, v(y) \rangle).$$

### Exercises {#alg-ii-s4-exercises}

See the [exercises for § 4](exercises/s4/).
