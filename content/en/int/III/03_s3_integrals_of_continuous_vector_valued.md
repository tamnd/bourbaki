---
book: int
book_title: Integration
chapter: III
chapter_title: MEASURES ON LOCALLY COMPACT SPACES
section: 3
section_title: Integrals of continuous vector-valued functions
lang: en
source: int-i-vi
book_pages: INT III.32-INT III.40, INT III.60
pdf_pages: 0077-0085, 0105-0105
extraction: ocr
subsections:
    - "no": 1
      title: Definition of the integral of a vector-valued function
      page: 32
      pdf_page: 77
    - "no": 2
      title: Properties of the vectorial integral
      page: 34
      pdf_page: 79
    - "no": 3
      title: Criteria for the integral to belong to $E$
      page: 37
      pdf_page: 82
    - "no": 4
      title: Continuity properties of the integral
      page: 39
      pdf_page: 84
statements: 17
exercises: 4
content_sha256: 08e80431efbc022e93acec00bafa9892334f63e19b825a718a5f6da8a6173417
---

## § 3. INTEGRALS OF CONTINUOUS VECTOR-VALUED FUNCTIONS

*Throughout this section, X denotes a locally compact space, E a locally convex space over $\mathbf{R}$ or $\mathbf{C}$. We denote by $E'$ the dual of E (the space of continuous linear forms on E) and by ${E'}^*$ the algebraic dual of $E'$ (the space of all linear forms on $E'$); for $z \in E$, $z' \in E'$, ${z'}^* \in {E'}^*$, we write $\langle z, z' \rangle = z'(z)$, $\langle {z'}^*, z' \rangle = {z'}^*(z')$.

Recall that if E is Hausdorff, then E may be identified with a linear subspace of ${E'}^*$ by identifying an element $z \in E$ with the linear form $z' \mapsto \langle z, z' \rangle$ on $E'$, and that ${E'}^*$, equipped with the weak topology $\sigma({E'}^*, E')$, may be canonically identified with the completion of E equipped with the weakened topology $\sigma(E, E')$.

### 1. Definition of the integral of a vector-valued function

Recall that a mapping f of X into E is said to be *weakly continuous* if, for every $z' \in E'$, the mapping $x \mapsto \langle f(x), z' \rangle$ of X into $\mathbf{C}$ (in other words the mapping $z' \circ f$, also denoted $\langle f, z' \rangle$) is continuous. We shall say that a mapping f of X into E is *scalarly of compact support* if, for every $z' \in E'$, the mapping $x \mapsto \langle f(x), z' \rangle$ has compact support. We denote by $\widetilde{\mathcal{K}}(X; E)$ the space of mappings of X into E that are *weakly continuous and scalarly of compact support*; it is clear that $\widetilde{\mathcal{K}}(X; E) \supset \mathcal{K}(X; E)$, but these two spaces are not necessarily identical (see *Example* 2 below); they are, however, equal when E is finite-dimensional.

Note that in the definition of a function that is weakly continuous (resp. scalarly of compact support), the topology of E intervenes only through the intermediation of the dual $E'$ of E; thus, the set of these functions is not changed when the topology of E is replaced by any locally convex topology for which the dual is the same.

If E and F are two vector spaces in duality, we note that it means the same to say that a mapping of X into E is *continuous* for $\sigma(E, F)$ and to say that it is *weakly continuous*.

Let $f$ be a mapping of $X$ into $E$, weakly continuous and scalarly of compact support, and let $\mu$ be a measure on $X$; for every $z' \in E'$ we have $z' \circ f \in \mathcal{K}(X)$; set

$$
\varphi(z') = \int \langle f(x), z' \rangle d\mu(x) = \mu(z' \circ f).
$$

It is clear that $\varphi$ is a linear form on $E'$, hence is *an element of ${E'}^*$*.

#### Definition 1 {#int-iii-s3-def-1 .statement}

*For every function $f \in \widetilde{\mathcal{K}}(X;E)$ we call integral of $f$ with respect to $\mu$, and denote by $\int f d\mu$ or $\int f(x) d\mu(x)$, or $\int f \mu$, or $\int f(x)\mu(x)$, the element of ${E'}^*$ defined by*

$$
\left\langle \int f d\mu, z' \right\rangle = \int \langle f, z' \rangle d\mu \quad \text{for all } z' \in E'.
$$

We note that even if $E$ is *Hausdorff* and $f \in \mathcal{K}(X;E)$, *one does not necessarily have* $\int f d\mu \in E$ (Exer. 1; cf. No. 3).

#### Example {#int-iii-s3-n1-exa-1 .statement}

— 1) Suppose that $E$ is *finite-dimensional* over $\mathbf{C}$ and Hausdorff, so that if $(e_i)_{1 \leq i \leq n}$ is a basis of $E$ then the mapping

$$
(\xi_1, \ldots \xi_n) \mapsto \sum_{i=1}^n \xi_i e_i
$$

is an *isomorphism* of $\mathbf{C}^n$ onto $E$. We then know that every linear form on $E$ is continuous, in other words that $E'$ is identical to the algebraic dual $E^*$ of $E$, and ${E'}^*$ may be canonically identified with $E$. Let $(e'_i)_{1 \leq i \leq n}$ be the basis of $E'$ dual to $(e_i)$; for a mapping $f$ of $X$ into $E$ to be weakly continuous and scalarly of compact support, it is necessary and sufficient that the functions $f_i = e'_i \circ f$ be continuous with compact support; we then have $f(x) = \sum_{i=1}^n f_i(x) e_i$ for all $x \in X$, and

$$
\int f d\mu = \sum_{i=1}^n \mu(f_i) e_i.
$$

2) Let us take for $E$ the space $\mathcal{M}(X; \mathbf{C})$ of measures on $X$, equipped with the *vague* topology (§ 1, No. 9); the dual $E'$ of $E$ may then be canonically identified with the space $\mathcal{K}(X; \mathbf{C})$ (TVS, II, § 6, No. 2, Prop. 3). The mapping $x \mapsto \varepsilon_x$ of $X$ into $E$ is *continuous* (§ 1, No. 9, Prop. 13), but its support is not compact if $X$ is not compact; however, it is *scalarly of compact* support, because for every function $f \in E'$ the function $x \mapsto \langle \varepsilon_x, f \rangle = f(x)$ by definition has compact support. Moreover,

$$
\int \langle \varepsilon_x, f \rangle d\mu = \int f(x) d\mu(x) = \langle \mu, f \rangle
$$

for every function $f \in \mathcal{K}(X; \mathbf{C}) = E'$, which proves that

$$
\int \varepsilon_x d\mu(x) = \mu
$$

for every measure $\mu$ on $X$.

3) If $E$ is Hausdorff then, for every point $y \in X$ and every function $f \in \widetilde{\mathcal{K}}(X; E)$, we have

$$
\int f d\varepsilon_y = f(y)
$$

because $\int \langle f, z' \rangle d\varepsilon_y = \langle f(y), z' \rangle$ by definition.

#### Remark 1 {#int-iii-s3-n1-rem-1 .statement}

If $E$ is a locally convex space and $N$ is the closure of $\{0\}$ in $E$, so that $E_1 = E/N$ is the Hausdorff locally convex space associated with $E$, we know that the duals $E'$ and $E'_1$ are identical; for a function $f$ to belong to $\widetilde{\mathcal{K}}(X; E)$, it is necessary and sufficient that $f_1 = \pi \circ f$ (where $\pi : E \to E_1$ is the canonical homomorphism) belong to $\widetilde{\mathcal{K}}(X; E_1)$, in which case $\int f d\mu = \int f_1 d\mu$. We may therefore limit ourselves to considering only *Hausdorff* locally convex spaces.

#### Remark 2 {#int-iii-s3-n1-rem-2 .statement}

Let $E$ be a locally convex space *over* $\mathbf{C}$, and let $E_0$ be the locally convex space *over* $\mathbf{R}$ underlying $E$; we know that the mapping $z' \mapsto \Re z'$ which, to every continuous (complex) linear form $z'$ on $E$, makes correspond the continuous (real) linear form $z \mapsto \Re \langle z, z' \rangle$ on $E_0$, is an $\mathbf{R}$-isomorphism of the dual $E'$ onto the dual $E'_0$ of $E_0$ (TVS, II, §8, No. 1). Similarly, the algebraic dual $E'_0*$ of the real vector space $E'_0$ may be canonically identified with the real space underlying the algebraic dual $E'*$ of $E'$. It follows that if $\mu$ is a *real measure* and $f$ a mapping in $\widetilde{\mathcal{K}}(X; E)$, the formula (1) is again valid when $f$ is regarded as taking its values in $E_0$ and the canonical bilinear forms figuring in the two members as being, respectively, relative to the duality between $E'_0$ and $E'_0*$ for the first member and the duality between $E_0$ and $E'_0$ for the second.

### 2. Properties of the vectorial integral

#### Proposition 1 {#int-iii-s3-prop-1 .statement}

— *The mapping*

$$
(f, \mu) \mapsto \int f d\mu
$$

of $\widetilde{\mathcal{K}}(X; E) \times \mathcal{M}(X; \mathbf{C})$ into $E'*$ *is bilinear*.

The proposition follows immediately from Def. 1 of No. 1.

Let $u$ be a continuous linear mapping of $E$ into a locally convex space $F$; we know that the transpose $^t u$ is a linear mapping of the dual $F'$ of $F$ into the dual $E'$ of $E$; we shall denote by $^{tt} u$ the mapping ${E'}^* \to {F'}^*$, the transpose of $^t u$ (in the algebraic sense); when $E$ and $F$ are Hausdorff and are canonically identified with subspaces of ${E'}^*$ and ${F'}^*$, respectively, $^{tt} u$ extends the mapping $u$. With these notations:

#### Proposition 2 {#int-iii-s3-prop-2 .statement}

— Let $u$ be a continuous linear mapping of $E$ into a locally convex space $F$; for every function $f \in \widetilde{\mathcal{K}}(X;E)$, the function $u \circ f$ belongs to $\widetilde{\mathcal{K}}(X;F)$ and

$$
\int u(f(x))\, d\mu(x) = ^{tt} u \left( \int f(x)\, d\mu(x) \right).
$$

For every continuous linear form $z' \in F'$, we have $z' \circ u \circ f = y' \circ f$ on setting $y' = z' \circ u = {}^t u(z') \in E'$, whence the first assertion; moreover, for all $z' \in F'$,

$$
\left\langle \int (u \circ f)\, d\mu, z' \right\rangle = \int \langle u \circ f, z' \rangle\, d\mu = \int \langle f, {}^t u(z') \rangle\, d\mu \\
= \left\langle \int f\, d\mu, {}^t u(z') \right\rangle = \left\langle {}^{tt} u \left( \int f\, d\mu \right), z' \right\rangle,
$$

whence the formula (2).

#### Proposition 3 {#int-iii-s3-prop-3 .statement}

— For every function $g \in \mathcal{C}(X;\mathbf{C})$ and every function $f \in \widetilde{\mathcal{K}}(X;E)$, the function $gf$ belongs to $\widetilde{\mathcal{K}}(X;E)$ and

$$
\int f\, d(g \cdot \mu) = \int fg\, d\mu.
$$

Indeed, for every $z' \in E'$, $\langle gf, z' \rangle = g \langle f, z' \rangle$, whence the first assertion; moreover,

$$
\left\langle \int f\, d(g \cdot \mu), z' \right\rangle = \int \langle f, z' \rangle\, d(g \cdot \mu) = \int g \langle f, z' \rangle\, d\mu \\
= \int \langle gf, z' \rangle\, d\mu = \left\langle \int gf\, d\mu, z' \right\rangle,
$$

whence (3).

#### Proposition 4 {#int-iii-s3-prop-4 .statement}

— Let $\mu$ be a positive measure on $X$, $S$ its support, and $f$ a function in $\widetilde{\mathcal{K}}(X;E)$. Suppose $E$ is Hausdorff, and equip the space ${E'}^*$ with the weak topology $\sigma({E'}^*, E')$.

(i) *The integral* $\int f\, d\mu$ *belongs to the closure* C *in* E'** *of the convex cone generated by* f(S).

(ii) *If* $\mu$ *is bounded, then the integral* $\int f\, d\mu$ *belongs to the set* $\| \mu \| \cdot D$, *where* D *is the closed convex envelope of* f(S) *in* E'**.

If E is complex, we equip E with its underlying *real* vector space structure, which, as we have seen, does not modify the formula (1).

(i) We know that C is the intersection of the closed half-spaces in E'** that contain f(S) and are determined by closed hyperplanes passing through 0; it therefore suffices to prove that, for $z' \in E'$, the relation $\langle f(x), z' \rangle \geq 0$ for all $x \in S$ implies

$$
\left\langle \int f\, d\mu, z' \right\rangle \geq 0;
$$

but since

$$
\left\langle \int f\, d\mu, z' \right\rangle = \int \langle f, z' \rangle\, d\mu,
$$

this follows from §2, No. 3, Cor. 2 of Prop. 8.

(ii) We know that D is the intersection of the closed half-spaces in E'** that contain f(S); it therefore suffices to show that, for $z' \in E'$, the relation $\langle f(x), z' \rangle \leq a$ for all $x \in S$ implies

$$
\left\langle \int f\, d\mu, z' \right\rangle \leq a \| \mu \|;
$$

but this follows from §2, No. 3, Cor. 3 of Prop. 8.

#### Corollary {#int-iii-s3-n2-cor-1 .statement}

*Let* $\mu$ *be a positive measure on* X, $f$ *a mapping belonging to* $\mathcal{K}(X;E)$, *and* D *the closed convex envelope of* f(X) *in* E'**. *There exists a number* $a > 0$ *such that* $\int f\, d\mu \in a \cdot D$.

*If* $\nu$ *is any measure on* X, *there exist numbers* $a_1, a_2, a_3, a_4 > 0$ *such that* $\int f\, d\nu \in a_1 D - a_2 D + i a_3 D - i a_4 D$.

Suppose first that $\mu$ is positive; by hypothesis, the support K of f is compact; if $\nu$ is the restriction of $\mu$ to a relatively compact open neighborhood of K, then $\nu$ is bounded and $\int f\, d\mu = \int f\, d\nu \in \| \nu \| \cdot D$ by Prop. 4, (ii). The second result follows from this, since any complex measure may be written as $\mu_1 - \mu_2 + i \mu_3 - i \mu_4$, where the $\mu_j$ are positive.

#### Proposition 5 {#int-iii-s3-prop-5 .statement}

*Suppose that the space* X *is compact, and let* f *be a continuous mapping of* X *into a Hausdorff locally convex space* E. *The closed convex envelope of* f(X) *in* E'** *(for* $\sigma(E', E')$) *is equal to the set of vectors* $\int f\, d\mu$ *for all of the positive measures* $\mu$ *on* X *of total mass* 1.

Let C be the closed convex envelope of f(X) in E'**; since f(X) is compact and E'** is *complete*, C is compact. We already know (Prop. 4) that $\int f d\mu \in C$ for every measure $\mu$ belonging to the convex set $H$ of positive measures on $X$ of total mass equal to 1. On the other hand, $H$ is convex and *compact* for the vague topology (§ 1, No. 9, Cor. 3 of Prop. 15) and is the closure (for this topology) of the convex set $H_0$ of positive measures of mass 1 and *finite* support (§ 2, No. 4, Cor. 3 of Th. 1). Now, the image of $H_0$ under the mapping $\mu \mapsto \int f d\mu$ is the convex envelope $C_0$ of $f(X)$ in ${E'}^*$. On the other hand, this mapping is continuous for the vague topology on $\mathcal{M}(X; C)$ and the topology $\sigma({E'}^*, E')$ on ${E'}^*$ since $\langle \int f d\mu, z' \rangle = \int \langle f, z' \rangle d\mu$ by definition; thus the image of $H = \overline{H_0}$ is a *compact* convex set containing $C_0$ and contained in $C$; since $C = \overline{C_0}$, this image is equal to $C$.

#### Proposition 6 {#int-iii-s3-prop-6 .statement}

*For every continuous mapping with compact support $f$ of $X$ into a Hausdorff locally convex space $E$, every continuous semi-norm $q$ on $E$ and every measure $\mu$ on $X$ such that $\int f d\mu \in E$,*

$$
q \left( \int f d\mu \right) \leq \int (q \circ f) \ d|\mu|.
$$

Let $D$ be the set of $z \in E$ such that $q(z) \leq 1$; $D$ is closed, convex and contains 0, therefore $D = D^{o o}$ (TVS, II, § 6, No. 3, Cor. 3 of Th. 1). It therefore suffices to prove that for every $z' \in D^o$,

$$
\left| \left\langle \int f d\mu, z' \right\rangle \right| \leq \int (q \circ f) \ d|\mu|;
$$

since

$$
\left\langle \int f d\mu, z' \right\rangle = \int \langle f, z' \rangle d\mu,
$$

and since, by the definition of $D^o$,

$$
|\langle f(x), z' \rangle| \leq q(f(x))
$$

for all $x \in X$, the desired inequality follows from the inequality (13) of § 1, No. 6.

### 3. Criteria for the integral to belong to $E$

#### Proposition 7 {#int-iii-s3-prop-7 .statement}

*Let $E$ be a Hausdorff locally convex space, and $f \in \mathcal{K}(X; E)$. If $f(X)$ is contained in a complete convex subset $A$ of $E$, then $\int f d\mu \in E$.*

Let K be the support of f, which is compact by hypothesis. Since f is zero on X − K, f(X) is equal to f(K) or to f(K) ∪ {0}, therefore is compact since f is continuous and E is Hausdorff; the closed convex envelope C of f(X) in E is then precompact (for the uniform structure induced by that of E) (TVS, II, §4, No. 1, Prop. 3). But since C is a closed subset of the complete space A, C is complete and therefore compact; a fortiori, C is compact for the weakened topology σ(E, E′); but since that topology is induced by σ(E′*, E′), C is the closed convex envelope of f(X) in E′* for the topology σ(E′*, E′); the proof is therefore concluded by the Corollary of Prop. 4 of No. 2.

#### Corollary 1 {#int-iii-s3-prop-7-cor-1 .statement}

— Let E be a Hausdorff locally convex space; for every function f ∈ 𝒦(X; E), $\int f d\mu$ belongs to the completion $\widehat{E}$ of E.

Since the duals of E and $\widehat{E}$ are identical, it suffices to apply Prop. 7 while regarding f as taking its values in $\widehat{E}$.

#### Corollary 2 {#int-iii-s3-prop-7-cor-2 .statement}

— If E is a quasi-complete Hausdorff locally convex space, then $\int f d\mu \in E$ for every function f ∈ 𝒦(X; E).

As noted at the beginning of the proof of Prop. 7, f(X) is compact and its closed convex envelope C in E is precompact, hence bounded; but since the set C is closed and bounded, it is complete by hypothesis, and it suffices to apply Prop. 7.

We shall see, in Ch. VI, §1, No. 2, other criteria for $\int f d\mu$ to belong to E, which apply in particular to the functions in $\widetilde{\mathcal{K}}(X; E)$ and not just those in $\mathcal{K}(X; E)$.

Corollary 2 of Proposition 7 may be applied in the following two cases:
1° E is a Banach space; 2° E is the dual of a barreled Hausdorff locally convex space G, and E is equipped with an $\mathcal{S}$-topology, where $\mathcal{S}$ is a covering of G by bounded subsets (TVS, III, §4, No. 2, Cor. 4 of Th. 1). For example, Cor. 2 of Prop. 7 can be applied when E is the weak dual of a Banach space, or a space of measures $\mathcal{M}(Y; \mathbf{C})$ equipped with the vague topology.

If X = $\mathbf{R}$, $\mu$ is Lebesgue measure on $\mathbf{R}$, and E is a Banach space, then the integral $\int f d\mu$ of a function in $\mathcal{K}(X; E)$ is none other than the integral

$$
\int_{-\infty}^{+\infty} f(x)\, dx
$$

defined in FRV, II, §2, No. 1; this follows from formula (1), and from FRV, I, §1, No. 2, Cor. of Prop. 2.

### 4. Continuity properties of the integral

#### Proposition 8 {#int-iii-s3-prop-8 .statement}

— Suppose that E is Hausdorff; let $\mu$ be a measure on X. The mapping $f \mapsto \int f d\mu$ of $\mathcal{K}(X;E)$ into $\widehat{E}$ (No. 3, Cor. 1 of Prop. 7) is the unique continuous linear mapping $\Phi$ such that $\Phi(g \cdot a) = \mu(g) \cdot a$ for every vector $a \in E$ and every function $g \in \mathcal{K}(X;\mathbf{C})$.

To prove the continuity of the mapping $f \mapsto \int f d\mu$, it suffices to show that its restriction to $\mathcal{K}(X,K;E)$ is continuous for every compact subset K of X (TVS, II, §4, No. 4, Prop. 5). We note that if the topology of E is defined by a family of semi-norms $(q_\alpha)$, that of $\mathcal{K}(X,K;E)$ is defined by the family of semi-norms

$$
p_\alpha(f) = \sup_{x \in K} q_\alpha(f(x)) .
$$

Now, let $h$ be a continuous mapping of X into $[0,1]$, with compact support and such that $h(x) = 1$ on K; by No. 2, Prop. 6 we have, for every function $f \in \mathcal{K}(X,K;E)$,

$$
q_\alpha \left( \int f d\mu \right) = q_\alpha \left( \int h f d\mu \right) \leq \int h(x) q_\alpha(f(x)) d|\mu|(x) \leq |\mu|(h) \cdot p_\alpha(f)
$$

(the $q_\alpha$ being extended by continuity to $\widehat{E}$), which proves the continuity of $f \mapsto \int f d\mu$. On the other hand, with the notations of the statement,

$$
\int (g(x) \cdot a) d\mu(x) = \mu(g) \cdot a
$$

by virtue of No. 1, Example 1 and Prop. 2 of No. 2 applied to the canonical injection $\mathbf{C} \cdot a \to E$. Moreover, the subspace of $\mathcal{K}(X;E)$ formed by the linear combinations $\sum_i g_i \cdot a_i$, where $a_i \in E$ and $g_i \in \mathcal{K}(X;\mathbf{C})$, is dense in $\mathcal{K}(X;E)$ (§1, No. 2, Prop. 5), which completes the proof.

#### Proposition 9 {#int-iii-s3-prop-9 .statement}

— Suppose that E is Hausdorff; let $f$ be a continuous mapping of X into E with compact support. When the space $\mathcal{M}(X;\mathbf{C})$ is equipped with the topology of strictly compact convergence (§1, No. 10), the mapping $\mu \mapsto \int f d\mu$ of $\mathcal{M}(X;\mathbf{C})$ into $\widehat{E}$ is the unique continuous linear mapping $\Psi$ such that $\Psi(\varepsilon_x) = f(x)$ for all $x \in X$.

For every $z' \in E'$,

$$
\left\langle \int f d\varepsilon_x, z' \right\rangle = \int (z' \circ f) d\varepsilon_x = z'(f(x)) = \langle f(x), z' \rangle ,
$$

whence $\int f\, d\varepsilon_x = f(x)$. We know, moreover, that the set of point measures is total in $\mathcal{M}(X; \mathbf{C})$ for the topology of strictly compact convergence (§ 2, No. 4, Cor. 4 of Th. 1). Thus it all comes down to proving the continuity of the linear mapping $u : \mu \mapsto \int f\, d\mu$. For this, consider the linear mapping $v : z' \mapsto \langle f, z' \rangle$ of $E'$ into $\mathcal{K}(X; \mathbf{C})$, and let us show that the image under $v$ of an equicontinuous subset $H$ of $E'$ is contained in a strictly compact subset of $\mathcal{K}(X; \mathbf{C})$. For, if $K$ is the support of $f$, the functions $\langle f, z' \rangle$ for $z' \in H$ have support contained in $K$; on the other hand, these functions form an equicontinuous set, and for each $x \in X$ the set of $z'(f(x))$ is bounded; our assertion therefore follows from Ascoli’s theorem (GT, X, § 2, No. 5, Cor. 3 of Th. 2). Now, it follows from formula (1) of No. 1 that $u$ is none other than the restriction to $\mathcal{M}(X; \mathbf{C})$ of the transpose $^t v$ (in the algebraic sense); its continuity therefore follows from the foregoing (TVS, IV, § 1, No. 3, Prop. 6).

#### Corollary {#int-iii-s3-n4-cor-1 .statement}

— *With hypotheses and notations as in Prop. 9, the restriction of the mapping* $\mu \mapsto \int f\, d\mu$ *to the set* $\mathcal{M}_+(X)$ *of positive measures, or to a vaguely bounded subset B of* $\mathcal{M}(X; \mathbf{C})$, *is vaguely continuous.*

For, it follows from § 1, No. 10, Props. 17 and 18 that, on $\mathcal{M}_+(X)$ or on $B$, the topology induced by the topology of strictly compact convergence is the same as the topology induced by the vague topology.

However, the mapping $\mu \mapsto \int f\, d\mu$ is not necessarily continuous on all of $\mathcal{M}(X; \mathbf{C})$ for the vague topology (Exer. 2).

### Exercises {#int-iii-s3-exercises}

See the [exercises for § 3](exercises/s3/).
