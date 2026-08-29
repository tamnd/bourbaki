---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: I
chapter_title: Lie Algebras
section: 1
section_title: Definition of Lie algebras
lang: en
source: lie-i-iii
book_pages: 1-12, 73-83
pdf_pages: 0019-0030, 0091-0101
extraction: ocr
subsections:
    - "no": 1
      title: ALGEBRAS
      page: 1
      pdf_page: 19
    - "no": 2
      title: LIE ALGEBRAS
      page: 3
      pdf_page: 21
    - "no": 3
      title: COMMUTATIVE LIE ALGEBRAS
      page: 5
      pdf_page: 23
    - "no": 4
      title: IDEALS
      page: 5
      pdf_page: 23
    - "no": 5
      title: DERIVED SERIES, LOWER CENTRAL SERIES
      page: 6
      pdf_page: 24
    - "no": 6
      title: UPPER CENTRAL SERIES
      page: 6
      pdf_page: 24
    - "no": 7
      title: EXTENSIONS
      page: 7
      pdf_page: 25
    - "no": 8
      title: SEMI-DIRECT PRODUCTS
      page: 8
      pdf_page: 26
    - "no": 9
      title: CHANGE OF BASE RING
      page: 11
      pdf_page: 29
statements: 19
exercises: 27
content_sha256: 34c36ec4b6364065c59b2c64940de2dd7a1af068ca79123de094195be8edaedd
---

## § 1. DEFINITION OF LIE ALGEBRAS

### 1. ALGEBRAS

Let M be a unitary module over K with a bilinear mapping $(x, y) \mapsto xy$ of $M \times M$ into M. All the axioms for algebras are satisfied except associativity of multiplication. By an abuse of language, M is called a not necessarily associative algebra over K, or sometimes, when no confusion can arise, an algebra over K. In this no. we shall use the latter notation.

If the K-module M is given the multiplication $(x, y) \mapsto yx$ an algebra is obtained called the opposite of the above algebra.

A sub-K-module N of M which is stable under multiplication is given the structure of an algebra over K in an obvious way. N is called a subalgebra of M. N is called a left (resp. right) ideal of M if the conditions $x \in N, y \in M$ imply $yx \in N$ (resp. $xy \in N$). If N is both a left ideal and a right ideal of M, N is called a two-sided ideal of M. In this case the multiplication on M enables us to define, on passing to the quotient, a bilinear multiplication on the quotient module $M/N$ such that $M/N$ has an algebra structure. $M/N$ is called the quotient algebra of M by N.

† The propositions proved in this chapter depend only on the properties established in Books I to VI and on certain results of Commutative Algebra, Chapter III, § 2.

Let $M_1$ and $M_2$ be two algebras over $K$ and $\phi$ a mapping of $M_1$ into $M_2$. $\phi$ is called a *homomorphism* if $\phi$ is $K$-linear and $\phi(xy) = \phi(x)\phi(y)$ for $x \in M_1, y \in M_1$. The kernel $N$ of $\phi$ is a two-sided ideal of $M_1$ and the image of $\phi$ is a subalgebra of $M_2$. On passing to the quotient, $\phi$ defines an isomorphism of the algebra $M_1/N$ onto the algebra $\phi(M_1)$.

Let $M$ be an algebra over $K$. A mapping $D$ of $M$ into $M$ is called a *derivation* of $M$ if it is $K$-linear and $D(xy) = (Dx)y + x(Dy)$ for all $x \in M$ and $y \in M$. This definition generalizes Definition 3 of *Algebra*, Chapter IV, § 4, no. 3. The kernel of a derivation of $M$ is a subalgebra of $M$. If $D_1$ and $D_2$ are derivations of $M$, then $D_1D_2 - D_2D_1$ is a derivation of $M$ (cf. *Algebra*, Chapter IV, § 4, no. 3, Proposition 5: the proof of this proposition does not use the associativity of the algebra).

Let $M_1$ and $M_2$ be two algebras over $K$. On the product $K$-module $M = M_1 \times M_2$ we define a multiplication by writing

$$
(x_1, x_2)(y_1, y_2) = (x_1y_1, x_2y_2),
$$

for all $x_1, y_1$ in $M_1$, $x_2, y_2$ in $M_2$. The algebra thus defined is called the *product algebra* of $M_1$ and $M_2$. The mapping $x_1 \mapsto (x_1, 0)$ (resp. $x_2 \mapsto (0, x_2)$) is an isomorphism of $M_1$ (resp. $M_2$) onto a two-sided ideal of $M$. Under these isomorphisms $M_1$ and $M_2$ are identified with two-sided ideals of $M$. The $K$-module $M$ is then the direct sum of $M_1$ and $M_2$. Conversely, let $M$ be an algebra over $K$ and $M_1, M_2$ two two-sided ideals of $M$ such that $M$ is the direct sum of $M_1$ and $M_2$. Then $M_1M_2 \subset M_1 \cap M_2 = \{0\}$; then, if $x_1, y_1$ belong to $M_1$ and $x_2, y_2$ to $M_2$, then $(x_1 + x_2)(y_1 + y_2) = x_1y_1 + x_2y_2$, so that $M$ is identified with the product algebra $M_1 \times M_2$. Every left (resp. right, two-sided) ideal of $M_1$ is a left (resp. right, two-sided) ideal of $M$. We leave to the reader the task of formulating the analogous results in the case of an arbitrary finite family of algebras.

Let $M$ be an algebra over $K$ and suppose that the $K$-module $M$ admits a basis $(a_\lambda)_{\lambda \in L}$. There exists a unique system $(\gamma_{\lambda \mu \nu})_{(\lambda, \mu, \nu) \in L \times L \times L}$ of elements of $K$ such that $a_\lambda a_\mu = \sum_v \gamma_{\lambda \mu v} a_v$ for all $\lambda, \mu$ in $L$. The $\gamma_{\lambda \mu \nu}$ are called the *constants of structure of $M$ with respect to the basis* $(a_\lambda)$.

Let $M$ be an algebra over $K$, $K_0$ a commutative ring with unit element and $\rho$ a homomorphism of $K_0$ into $K$ mapping unit element to unit element. Then $M$ can be considered as an algebra over $K_0$ by writing $\alpha.x = \rho(\alpha).x$ for $\alpha \in K_0, x \in M$. This is the case in particular when $K_0$ is a subring of $K$ containing the unit element and $\rho$ is taken to be the inclusion mapping of $K_0$ into $K$.

Let $M$ be an algebra over $K$, $K_1$ a commutative ring with unit element and $\sigma$ a homomorphism of $K$ into $K_1$ mapping unit element to unit element. Let $M_{(K_1, \sigma)} = M_{(K_1)}$ be the $K_1$-module derived from $M$ by extending the ring of scalars to $K_1$ (*Algebra*, Chapter II, § 5). The product on $M$ defines canonically a $K_1$-bilinear mapping of $M_{(K_1)} \times M_{(K_1)}$ into $M_{(K_1)}$ (*Algebra*, Chapter IX, § 1, no. 4) such that $M_{(K_1)}$ is given the structure of an algebra over $K_1$ (which is said to be *derived from* $M$ *by extending the ring of scalars to* $K_1$). This is the case in particular when $K$ is a subring of $K_1$ containing the unit element and $\sigma$ the inclusion mapping of $K$ into $K_1$.

### 2. LIE ALGEBRAS

#### Definition 1 {#lie-i-s1-def-1 .statement}

*An algebra g over K is called a Lie algebra over K if its multiplication (denoted by $(x, y) \mapsto [x, y]$) satisfies the identities:*

(1) $$ [x, x] = 0 $$

(2) $$ [x, [y, z]] + [y, [z, x]] + [z, [x, y]] = 0 $$

*for all* $x, y, z$ *in g*.

The product $[x, y]$ is called the *bracket* of $x$ and $y$. Identity (2) is called the *Jacobi identity*.

The bracket $[x, y]$ is an alternating bilinear function of $x$ and $y$. We have the identity:

(3) $$ [x, y] = -[y, x] $$

so that the Jacobi identity can be written:

(4) $$ [x, [y, z]] = [[x, y], z] + [y, [x, z]]. $$

Every subalgebra and every quotient algebra of a Lie algebra is a Lie algebra. Every product of Lie algebras is a Lie algebra. If $g$ is a Lie algebra, the opposite algebra $g^0$ is a Lie algebra and the mapping $x \mapsto -x$ an isomorphism of $g$ onto $g^0$, by virtue of identity (3).

#### Example 1 {#lie-i-s1-n2-exa-1 .statement}

Let $L$ be an associative algebra over $K$. The bracket $[x, y] = xy - yx$ is a bilinear function of $x$ and $y$. It is easily verified that the law of composition $(x, y) \mapsto [x, y]$ on the $K$-module $L$ makes $L$ into a Lie algebra over $K$.

#### Example 2 {#lie-i-s1-n2-exa-2 .statement}

In Example 1 choose $L$ to be the associative algebra of endomorphisms of a $K$-module $E$. We obtain the *Lie algebra of endomorphisms of* $E$, denoted by $gl(E)$. (If $E = K^n$, the Lie algebra $gl(E)$ is denoted by $gl(n, K)$.)

Every Lie subalgebra of $gl(E)$ is a Lie algebra over $K$. In particular:
(1) If $E$ is given a (not necessarily associative) algebra structure, the derivations of $E$ form a Lie algebra over $K$.
(2) If $E$ admits a finite basis, the endomorphisms of $E$ of zero trace form a Lie algebra over $K$ denoted by $sl(E)$ (or $sl(n, K)$ if $E = K^n$).
(3) The set $M_n(K)$ of square matrices of order $n$ can be considered as a Lie algebra over K canonically isomorphic to gl(n, K). Let $(E_{ij})$ be the canonical basis of $\mathbf{M}_n(K)$ (Algebra, Chapter II, § 10, no. 3). It follows easily that:

$$
\begin{cases}
[E_{ij}, E_{kl}] = 0 & \text{if } j \neq k \text{ and } i \neq l \\
[E_{ij}, E_{jl}] = E_{il} & \text{if } i \neq l \\
[E_{ij}, E_{kt}] = -E_{kj} & \text{if } j \neq k \\
[E_{ij}, E_{ji}] = E_{ii} - E_{jj}
\end{cases}
$$

(5)

The Lie subalgebra of $\mathbf{M}_n(K)$ consisting of the triangular matrices (resp. triangular matrices of zero trace, resp. triangular matrices of zero diagonal) is denoted by $t(n, K)$ (resp. st(n, K), resp. n(n, K)) (Algebra, Chapter II, § 10; no. 7).

*Example 3. Let V be an infinitely differentiable real manifold. The differential operators with infinitely differentiable real coefficients constitute an associative algebra over $\mathbf{R}$ and hence, by Example 1, a Lie algebra $\Delta$ over $\mathbf{R}$. The bracket of two infinitely differentiable vector fields on V is an infinitely differentiable vector field and hence the infinitely differentiable vector fields on V constitute a Lie subalgebra $\mathfrak{f}$ of $\Delta$. If V is a real *Lie group*, the left invariant vector fields constitute a Lie subalgebra $g$ of $\mathfrak{f}$ called the *Lie algebra* of V. The vector space $g$ is identified with the tangent space to V at $e$ (the identity element of V). Let V' be another real Lie group, $e'$ its identity element and $g'$ its Lie algebra. Every analytic homomorphism of V into V' defines a linear mapping of the tangent space to V at $e$ into the tangent space to V' at $e'$; this mapping is a homomorphism of the Lie algebra $g$ into the Lie algebra $g'$. If V is the linear group of a finite-dimensional real vector space E there exists a canonical isomorphism of $gl(E)$ onto the Lie algebra $g$ of V, under which $g$ is identified with $gl(E)$.*

#### Definition 2 {#lie-i-s1-def-2 .statement}

*Let g be a Lie algebra and x an element of g. The linear mapping $y \mapsto [x, y]$ of g into g is called the adjoint linear mapping of x and is denoted by $\operatorname{ad}_g x$ or $\operatorname{ad} x$.*

#### Proposition 1 {#lie-i-s1-prop-1 .statement}

*Let g be a Lie algebra. For all $x \in g$, $\operatorname{ad} x$ is a derivation. The mapping $x \mapsto \operatorname{ad} x$ is a homomorphism of the Lie algebra g into the Lie algebra $\mathfrak{d}$ of derivations of g. If $D \in \mathfrak{d}$ and $x \in g$, $[D, \operatorname{ad} x] = \operatorname{ad}(Dx)$.

Identity (4) can be written:

$$
(\operatorname{ad} x) \cdot [y, z] = [(\operatorname{ad} x) \cdot y, z] + [y, (\operatorname{ad} x) \cdot z]
$$

or:

$$
(\operatorname{ad}[x, y]) \cdot z = (\operatorname{ad} x) \cdot ((\operatorname{ad} y) \cdot z) - (\operatorname{ad} y) \cdot ((\operatorname{ad} x) \cdot z)
$$

whence the first two assertions. On the other hand, if $D \in \mathfrak{d}$, $x \in g$, $y \in g$, then $[D, \operatorname{ad} x] \cdot y = D([x, y]) - [x, Dy] = [Dx, y] = (\operatorname{ad} Dx) \cdot y$, whence the last assertion.

The mapping $\operatorname{ad} x$ is also called the *inner derivation* defined by $x$.

### 3. COMMUTATIVE LIE ALGEBRAS

#### Definition 3 {#lie-i-s1-def-3 .statement}

*Two elements x, y of a Lie algebra are said to be permutable if [x, y] = 0. g is said to be commutative if any two of its elements are permutable.*

#### Example 1 {#lie-i-s1-n3-exa-1 .statement}

Let L be an associative algebra and g the Lie algebra defined by it (no. 2, Example 1). Two elements x, y are permutable in g if and only if xy = yx in L.

*Example 2. If a real Lie group G is commutative, its Lie algebra is commutative.*

Every K-module can obviously be given a unique commutative Lie algebra structure over K.

If g is a Lie algebra, every monogenous submodule of g is a commutative Lie subalgebra of g.

### 4. IDEALS

It follows from identity (3) that in a Lie algebra g there is no distinction between left ideals and right ideals, every ideal being two-sided. We therefore speak simply of ideals.

*Example. Let G be a Lie group, g its Lie algebra and H a Lie subgroup of G. Every left invariant vector field on H defines canonically a left invariant vector field on G, whence there is a canonical injection of the Lie algebra h of H into g; h is identified with a Lie subalgebra of g under this injection. If H is normal in G, the canonical image of h in g is an ideal of g.*

An ideal of g is a submodule of g which is stable under the inner derivations of g.

#### Definition 4 {#lie-i-s1-def-4 .statement}

*A submodule of g which is stable under every derivation of g is called a characteristic ideal of g.*

#### Proposition 2 {#lie-i-s1-prop-2 .statement}

*Let g be a Lie algebra, a an ideal (resp. a characteristic ideal) of g and b a characteristic ideal of a. Then b is an ideal (resp. a characteristic ideal) of g.*

Every inner derivation (resp. every derivation) of g leaves a stable and induces on a a derivation and hence leaves b stable.

Let g be a Lie algebra. If a and b are ideals of g, a + b and a ∩ b are ideals of g.

Let a and b be two submodules of g. By an abuse of notation, the submodule of g generated by the elements of the form [x, y] (x ∈ a, y ∈ b) is denoted by [a, b]. We have [a, b] = [b, a] by identity (3). If z ∈ g, [z, a], or [a, z], denotes the submodule [Kz, a] = (ad z)(a).

#### Proposition 3 {#lie-i-s1-prop-3 .statement}

*If a and b are ideals (resp. characteristic ideals) of g, [a, b] is an ideal (resp. a characteristic ideal) of g.*

Let D be an inner derivation (resp. a derivation) of g. If $x \in a$ and $y \in b$, then
$$
D([x, y]) = [Dx, y] + [x, Dy] \in [a, b].
$$
Hence the proposition.

If a is a submodule of g, the set of $x \in g$ such that $(\mathrm{ad}\ x).a \subset a$ is a subalgebra n of g called the *normalizer* of a in g. If further a is a subalgebra of g, then $a \subset n$ and a is an ideal of n.

### 5. DERIVED SERIES, LOWER CENTRAL SERIES

The characteristic ideal $[g, g]$ is called the *derived ideal* of a Lie algebra g and denoted by $\mathcal{D}g$.

Every submodule of g containing $\mathcal{D}g$ is an ideal of g.

The *derived series* of g is the decreasing sequence $\mathcal{D}^0g, \mathcal{D}^1g, \ldots$ of characteristic ideals of g defined inductively as follows: (1) $\mathcal{D}^0g = g$; (2) $\mathcal{D}^{p+1}g = [\mathcal{D}^pg, \mathcal{D}^pg]$.

The *lower central series* of g is the decreasing sequence $\mathcal{C}^1g, \mathcal{C}^2g, \ldots$ of characteristic ideals of g defined inductively as follows: (1) $\mathcal{C}^1g = g$; (2) $\mathcal{C}^{p+1}g = [g, \mathcal{C}^pg]$. Then $\mathcal{C}^2g = \mathcal{D}g$ and $\mathcal{C}^{p+1}g \supset \mathcal{D}^pg$ for all $p$, as is immediately seen by induction on $p$.

#### Proposition 4 {#lie-i-s1-prop-4 .statement}

*Let g and h be two Lie algebras over K and f a homomorphism of g onto h. Then $f(\mathcal{D}^pg) = \mathcal{D}^pf, f(\mathcal{C}^pg) = \mathcal{C}^ph$.*

If a and b are submodules of g, it follows immediately that
$$
f([a, b]) = [f(a), f(b)].
$$
The proposition is then immediate by induction on $p$.

#### Corollary {#lie-i-s1-n5-cor-1 .statement}

*Let g be a Lie algebra and a an ideal of g. For the Lie algebra $g/a$ to be commutative, it is necessary and sufficient that $a \supset \mathcal{D}g$.*

To say that $g/a$ is commutative amounts to saying that $\mathcal{D}(g/a) = \{0\}$.
But $\mathcal{D}(g/a)$ is, by Proposition 4, the canonical image of $\mathcal{D}g$ in $g/a$.

### 6. UPPER CENTRAL SERIES

Let g be a Lie algebra and P a subset of g. The *centralizer* of P in g is the set of elements of g which are permutable with those of P. This centralizer is the intersection of the kernels of the ad $y$, where $y$ runs through P; it is therefore a subalgebra of g.

#### Proposition 5 {#lie-i-s1-prop-5 .statement}

*Let g be a Lie algebra and a an ideal (resp. a characteristic ideal) of g. The centralizer $a'$ of a in g is an ideal (resp. a characteristic ideal) of g.*

Let D be an inner derivation (resp. a derivation) of g. If $x \in a'$ and $y \in a$, then
$$
[Dx, y] = D([x, y]) - [x, Dy] = 0;
$$
hence $Dx \in a'$. Hence the proposition.

Let $g$ be a Lie algebra. The centralizer of $g$ in $g$ is called the centre of $g$, that is the characteristic ideal of $x \in g$ such that $[x, y] = 0$ for all $y \in g$. The centre of $g$ is the kernel of the homomorphism $x \mapsto \mathrm{ad}\, x$.

The upper central series of $g$ is the increasing sequence $\mathcal{C}_0 g, \mathcal{C}_1 g, \ldots$ of characteristic ideals of $g$ defined inductively as follows: (1) $\mathcal{C}_0 g = \{0\}$; (2) $\mathcal{C}_{p+1} g$ is the inverse image under the canonical mapping of $g$ onto $g / \mathcal{C}_p g$ of the centre of $g / \mathcal{C}_p g$
The ideal $\mathcal{C}_1 g$ is the centre of $g$.

### 7. EXTENSIONS

#### Definition 5 {#lie-i-s1-def-5 .statement}

Let $a$ and $b$ be two Lie algebras over $K$. An extension of $b$ by $a$ is a sequence:

$$
a \xrightarrow{\lambda} g \xrightarrow{\mu} b
$$

where $g$ is a Lie algebra over $K$, $\mu$ a surjective homomorphism of $g$ onto $b$ and $\lambda$ an injective homomorphism of $a$ onto the kernel of $\mu$.

The kernel $n$ of $\mu$ is called the kernel of the extension. The homomorphism $\lambda$ is an isomorphism of $a$ onto $n$ and the homomorphism $\mu$ defines an isomorphism of $g / n$ onto $b$ when passing to the quotient.
By an abuse of language, $g$ is also called an extension of $b$ by $a$.

Two extensions:

$$
a \xrightarrow{\lambda} g \xrightarrow{\mu} b, \quad a \xrightarrow{\lambda'} g' \xrightarrow{\mu'} b
$$

are said to be equivalent if there exists a homomorphism $f$ of $g$ into $g'$ such that the following diagram:

$$
\begin{array}{ccccc}
a & \xrightarrow{\lambda} & g & \xrightarrow{\mu} & b \\
& & f \downarrow & & \\
& & g' & \xrightarrow{\mu'} & b \\
a & \xrightarrow{\lambda'} & g' & \xrightarrow{\mu'} & b
\end{array}
$$

is commutative (that is such that $f \circ \lambda = \lambda', \mu' \circ f = \mu$). We show that such a homomorphism is necessarily bijective. First $f$ is injective. For if $x \in g$ is such that $f(x) = 0$, then $\mu(x) = \mu'(f(x)) = 0$ and hence $x = \lambda(y)$ for some $y \in a$; then $\lambda'(y) = f(\lambda(y)) = f(x) = 0$, hence $y = 0$ and hence $x = 0$. On the other hand, $f$ is surjective. For $\mu' \circ f = \mu$ is surjective and hence $f(g) + \lambda'(a) = g'$; on the other hand $f(g) \supset f(\lambda(a)) = \lambda'(a)$.

It follows from this that the relation just defined between two extensions of $b$ by $a$ is an equivalence relation.

#### Proposition 6 {#lie-i-s1-prop-6 .statement}

Let

$$
a \xrightarrow{\lambda} g \xrightarrow{\mu} b
$$

be an extension of $b$ by $a$ and $n$ its kernel.

(a) *If there exists a subalgebra m of g supplementary to n in g, the restriction of μ to m is an isomorphism of m onto b. If ν denotes the inverse isomorphism of this restriction, ν is a homomorphism of b into g and μ ∘ ν is the identity automorphism of b.*

(b) *Conversely, if there exists a homomorphism ν of b into g such that μ ∘ ν is the identity automorphism of b, then ν(b) is a supplementary subalgebra of n in g.*

The assertions of (a) are immediate. On the other hand, let ν be a homomorphism of b into g such that μ ∘ ν is the identity automorphism of b. Then ν(b) is a subalgebra of g and g is the direct sum of ν(b) and $\mu^{-1}(0) = n$ (*Algebra*, Chapter VIII, § 1, no. 1).

#### Definition 6 {#lie-i-s1-def-6 .statement}

*Let*

$$
a \xrightarrow{\lambda} g \xrightarrow{\mu} b
$$

*be an extension of b by a and n its kernel. This extension is called inessential (resp. trivial) if there exists a subalgebra (resp. an ideal) of g supplementary to n in g. This extension is called central if n is contained in the centre of g.*

If the extension is trivial, let m be an ideal of g supplementary to n in g. Then (cf. no. 1) g is canonically identified with the Lie algebra m × n and hence with the Lie algebra a × b. Conversely, let a and b be two Lie algebras; then a × b is a trivial extension of a by b.

An inessential central extension is trivial. For let g be a Lie algebra, n an ideal of g contained in the centre of g and m a subalgebra of g supplementary to n in g. Then [m, g] = [m, m] + [m, n] = [m, m] ⊂ m and hence m is an ideal of g.

### 8. SEMI-DIRECT PRODUCTS

Let a and b be two Lie algebras over K. It is not easy to construct all the extensions of b by a. But we shall describe quite simply all the *inessential* extensions of b by a.

Let g be an inessential extension of b by a. We identify a with an ideal of g, b with a subalgebra of g supplementary to a and the module g with the module a × b. For all $b \in b$, let $\phi_b$ be the restriction to a of $\mathrm{ad}_g\ b$; this is a derivation of a and the mapping $b \mapsto \phi_b$ is a homomorphism of b into the Lie algebra of derivations of a. On the other hand, for $a, a'$ in a and $b, b'$ in b, we have:

$$
[(a, b), (a', b')] = [a + b, a' + b']
= [a, a'] + [a, b'] + [b, a'] + [b, b']
= ([a, a'] + \phi_b a' - \phi_{b'} a, [b, b']).
$$

Conversely, let a and b be Lie algebras over K and $b \mapsto \phi_b$ a homomorphism of b into the Lie algebra of derivations of a. On the product *g of the K-modules* a and b we define the bracket of two elements by writing:

$$
[(a, b), (a', b')] = ([a, a'] + \phi_b a' - \phi_{b'} a, [b, b'])
$$

for all $a, a'$ in $a$, $b, b'$ in $b$. It is immediate that this bracket is an alternating bilinear function of $(a, b), (a', b')$; we show that, given 3 elements $(a, b), (a', b'), (a'', b'')$ of $a \times b$:

(7)
$$
[(a, b), [(a', b'), (a'', b'')]] + [(a', b'), [(a'', b''), (a, b)]] \\
+ [(a'', b''), [(a, b), (a', b')]] = 0.
$$

As the left hand side of (7) is an alternating trilinear function of $(a, b), (a', b'), (a'', b'')$, it suffices to make the verification when this system of elements takes one of the following forms:

(8) $(a, 0), (a', 0), (a'', 0)$

(9) $(a, 0), (a', 0), (0, b'')$

(10) $(a, 0), (0, b'), (0, b'')$

(11) $(0, b), (0, b'), (0, b'')$.

In cases (8) and (11), relation (7) is an immediate consequence of the Jacobi identity in $a$ and $b$. In case (9), we have

$$
[(a, 0), [(a', 0), (0, b'')]] = [(a, 0), (-\phi_{b''}a', 0)] = (-[a, \phi_{b''}a'], 0)
$$
$$
[(a', 0), [(0, b''), (a, 0)]] = [(a', 0), (\phi_{b''}a, 0)] = ([a', \phi_{b''}a], 0)
$$
$$
[(0, b''), [(a, 0), (a', 0)]] = [(0, b''), ([a, a'], 0)] = (\phi_{b''}([a, a']), 0)
$$

and relation (7) follows from the equation:
$$
\phi_{b''}([a, a']) = [\phi_{b''}a, a'] + [a, \phi_{b''}a'].
$$

In case (10), we have:

$$
[(a, 0), [(0, b'), (0, b'')]] = [(a, 0), (0, [b', b''])] = (-\phi_{[b', b'']}a, 0)
$$
$$
[(0, b'), [(0, b''), (a, 0)]] = [(0, b'), (\phi_{b''}a, 0)] = (\phi_{b'}\phi_{b''}a, 0)
$$
$$
[(0, b''), [(a, 0), (0, b')]] = [(0, b''), (-\phi_{b'}a, 0)] = (-\phi_{b''}\phi_{b'}a, 0)
$$

and relation (7) follows from the equation:
$$
\phi_{[b', b'']} = \phi_{b'}\phi_{b''} - \phi_{b''}\phi_{b'}.
$$

Hence a Lie algebra structure has been defined on $g$. The mapping $(a, b) \mapsto b$ of $g$ onto $b$ is a homomorphism $\mu$ whose kernel $n$ is the ideal of elements of $g$ of the form $(a, 0)$. The mapping $a \mapsto (a, 0)$ is an isomorphism $\lambda$ of $a$ onto $n$. Hence:

(12)
$$
a \xrightarrow{\lambda} g \xrightarrow{\mu} b
$$

is an extension of $b$ by $a$ of kernel $n$, which is said to be *canonically defined by* $a, b, \phi$. The mapping $b \mapsto (0, b)$ is an isomorphism $\nu$ of $b$ onto a subalgebra of $g$ supplementary to $n$ in $g$; hence the extension is inessential.

If $a$ is identified with $n$ under $\lambda$ and $b$ with $v(b)$ under $v$, then, for $a \in a$ and $b \in b$:

$$
(\mathrm{ad}\ b).a = [(0, b), (a, 0)] = (\phi_b a, 0) = \phi_b a.
$$

When $\phi = 0$, $g$ is the product Lie algebra of $b$ and $a$. In the general case, $g$ is called the *semi-direct product of $b$ by $a$* (corresponding to the homomorphism $b \mapsto \phi_b$ of $b$ into the Lie algebra of derivations of $a$).

We have therefore established the following proposition:

#### Proposition 7 {#lie-i-s1-prop-7 .statement}

*Let $a$ and $b$ be two Lie algebras over $K$,*

$$
a \xrightarrow{\lambda} g \xrightarrow{\mu} b
$$

*an inessential extension of $b$ by $a$, $\nu$ an isomorphism of $b$ onto a subalgebra of $g$ such that $\mu \circ \nu$ is the identity automorphism of $b$ and $\phi$ the corresponding homomorphism of $b$ into the Lie algebra of derivations of $a$.* Let

$$
a \xrightarrow{\lambda_0} g_0 \xrightarrow{\mu_0} b
$$

*be the inessential extension of $b$ by $a$ canonically defined by $\phi$.* Then the mapping $(a, b) \mapsto \lambda(a) + \nu(b)$ is an isomorphism $f$ of $g_0$ onto $g$ and the following diagram

$$
\begin{array}{ccccc}
& & \\
a & \xrightarrow{\lambda_0} & g_0 & \xrightarrow{\mu_0} & b \\
& \searrow f & \downarrow & \nearrow \mu_0 \\
& & g & & \\
& \swarrow i & & \searrow \mu \\
& & & &
\end{array}
$$

*is commutative, so that the two extensions are equivalent.*

#### Example 1 {#lie-i-s1-n8-exa-1 .statement}

Let $g$ be a Lie algebra over $K$ and $D$ a derivation of $g$. Let $h$ be the *commutative* Lie algebra $K$. The mapping $\lambda \mapsto \lambda D (\lambda \in K)$ is a homomorphism of $h$ into the Lie algebra of derivations of $g$. We form the corresponding semi-direct product $t$ of $h$ by $g$. Let $x_0$ be the element $(0, 1)$ of $t$. For all $x \in g$, $Dx = [x_0, x]$.

#### Example 2 {#lie-i-s1-n8-exa-2 .statement}

Let $g$ be a Lie algebra over $K$, $M$ a $K$-module and $\rho$ a homomorphism of $g$ into $\mathfrak{gl}(M)$. If $M$ is considered as a commutative Lie algebra, the Lie algebra of derivations of $M$ is $\mathfrak{gl}(M)$. We can therefore form the semi-direct product $h$ of $g$ by $M$ corresponding to $\rho$.

In particular, let $g = \mathfrak{gl}(M)$ and $\rho$ be the identity mapping of $\mathfrak{gl}(M)$. The semi-direct product of $g$ by $M$ is then denoted by $\mathfrak{af}(M)$ (or $\mathfrak{af}(n, K)$ if $M = K^n$). An element of $\mathfrak{af}(M)$ is an ordered pair $(m, u)$, where $m \in M, u \in \mathfrak{gl}(M)$; and the bracket is defined by

$$
[(m, u), (m', u')] = (u(m') - u'(m), [u, u']).
$$

*When M is a finite-dimensional vector space over $\mathbf{R}$, $\mathfrak{af}(M)$ is canonically identified with the Lie algebra of the *affine group* of M.*

Let $t$ be a Lie algebra over K. A linear mapping $\theta$ of $t$ into $\mathfrak{af}(M)$ can be written $x \mapsto ((\zeta(x), \eta(x)))$, where $\zeta$ is a linear mapping of $t$ into $M$ and $\eta$ a linear mapping of $t$ into $gl(M)$. We examine the conditions that $\zeta$ and $\eta$ must satisfy for $\theta$ to be a homomorphism. For $x \in t, y \in t$, we must have

$$
\theta([x, y]) = [\theta(x), \theta(y)]
$$

that is

$$
(\zeta([x, y]), \eta([x, y])) = [(\zeta(x), \eta(x)), (\zeta(y), \eta(y))] \\
= (\eta(x) \cdot \zeta(y) - \eta(y) \cdot \zeta(x), [\eta(x), \eta(y)]).
$$

Hence for $\theta$ to be a homomorphism of $t$ into $\mathfrak{af}(M)$, it is necessary and sufficient that $\eta$ be a homomorphism of $t$ into $gl(M)$ and that $\zeta$ satisfy the relation:

(13)
$$
\zeta([x, y]) = \eta(x) \cdot \zeta(y) - \eta(y) \cdot \zeta(x).
$$

Let N be the K-module $M \times K$. We take $t$ to be the subalgebra of $gl(N)$ consisting of the $w \in gl(N)$ such that $w(N) \subset M$. For all $w \in t$, let $\eta(w) \in gl(M)$ be the restriction of $w$ to $M$ and let $\zeta(w) = w(0, 1) \in M$. For $w_1 \in t, w_2 \in t$,

$$
\zeta([w_1, w_2]) = w_1(\zeta(w_2)) - w_2(\zeta(w_1)) = \eta(w_1) \cdot \zeta(w_2) - \eta(w_2) \cdot \zeta(w_1).
$$

Hence the mapping $w \mapsto (\zeta(w)), \eta(w))$ is a homomorphism $\theta$ of $t$ into $\mathfrak{af}(M)$. Clearly $\theta$ is *bijective*. Let $\phi = \theta^{-1}$. If $(m, u) \in \mathfrak{af}(M)$, $\phi(m, u)$ is the element $w$ of $t$ defined by

$$
w(m', \lambda) = (u(m') + \lambda m, 0).
$$

$\mathfrak{af}(M)$ is often identified with the subalgebra $t$ of $gl(N)$ under the isomorphism $\phi$.

*When M is a finite-dimensional vector space over $\mathbf{R}$, the homomorphism $\phi$ of $\mathfrak{af}(M)$ into $gl(N)$ corresponds to a canonical homomorphism $\psi$ of the affine group A of M into the group $\mathbf{GL}(N)$; if $a \in A, \psi(a)$ is the unique element $g$ of $\mathbf{GL}(N)$ such that $g(m, 1) = (a(m), 1)$ for all $m \in M$. This homomorphism is injective and $\psi(A)$ is the set of automorphisms of N which leave invariant all the linear varieties of N parallel to M.*

### 9. CHANGE OF BASE RING

Let $K_0$ be a commutative ring with unit element and $\rho$ a homomorphism of $K_0$ into K mapping unit element to unit element. Let $g$ be a Lie algebra over K. Let $g'$ be the algebra obtained by considering $g$ as an algebra over $K_0$ by means of $\rho$ (cf. no. 1). Then $g'$ is a Lie algebra. The subalgebras (resp. ideals) of $g$ are subalgebras (resp. ideals) of $g'$. If $a$ and $b$ are submodules of $g$, the bracket $[a, b]$ is the same in $g$ and in $g'$; for $[a, b]$ is the set of elements of the form

$$
\sum_{i=1}^n [x_i, y_i]
$$

where $x_i \in a, y_i \in b$. It follows that $\mathcal{D}^p g = \mathcal{D}^p g', \mathcal{C}^p g = \mathcal{C}^p g'$ for all $p$.

The centralizer of a subset is the same in $g$ and $g'$. Hence $\mathcal{C}_p g = \mathcal{C}_p g'$ for all $p$.

Let $K_1$ be a commutative ring with unit element and $\sigma$ a homomorphism of $K$ into $K_1$ mapping unit element to unit element. Let $g$ be a Lie algebra over $K$. Let $g_{(K_1)}$ be the algebra over $K_1$ derived from $g$ by extending the base ring (cf. no. 1). Then $g_{(K_1)}$ is a Lie algebra. If $a$ is a subalgebra (resp. an ideal) of $g$, the canonical image of $a_{(K_1)}$ in $g_{(K_1)}$ is a subalgebra (resp. an ideal) of $g_{(K_1)}$. If $a$ and $b$ are submodules of $g$, the canonical image in $g_{(K_1)}$ of $[a, b]_{(K_1)}$ is equal to the bracket of the canonical images of $a_{(K_1)}$ and $b_{(K_1)}$. It follows that $\mathcal{D}^p(g_{(K_1)})$ is the canonical image of $(\mathcal{D}^p g)_{(K_1)}$ and that $\mathcal{C}^p(g_{(K_1)})$ is the canonical image of $\mathcal{C}^p(g_{(K_1)})$.

If $K$ is a field, $K_1$ an extension field of $K$ and $\sigma$ the canonical injection of $K$ into $K_1$, then with the usual identifications we have
$$
[a, b]_{(K_1)} = [a_{(K_1)}, b_{(K_1)}], \quad \mathcal{D}^p(g_{(K_1)}) = (\mathcal{D}^p g)_{(K_1)},
$$
$$
\mathcal{C}^p(g_{(K_1)}) = (\mathcal{C}^p g)_{(K_1)}.
$$

These results are completed in § 2, no. 9.

If $M$ is a finite-dimensional vector space over the field $K$, $M_{(K_1)}$ is a finite-dimensional vector space over $K_1$ and the associative algebra $\mathcal{L}(M_{(K_1)})$ is canonically identified with the associative algebra $\mathcal{L}(M)_{(K_1)}$. Hence the Lie algebra $gl(M_{(K_1)})$ is canonically identified with the Lie algebra $gl(M)_{(K_1)}$.

### Exercises {#lie-i-s1-exercises}

See the [exercises for § 1](exercises/s1/).
