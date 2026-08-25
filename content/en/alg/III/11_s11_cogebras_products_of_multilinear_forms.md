---
book: alg
book_title: Algebra
chapter: III
chapter_title: TENSOR ALGEBRAS, EXTERIOR ALGEBRAS, SYMMETRIC ALGEBRAS
section: 11
section_title: Cogebras, products of multilinear forms, inner products and duality
lang: en
source: alg-i-iii
source_edition: 1998, Springer
pdf_pages: 0598-0635, 0671-0678
extraction: ocr
subsections:
    - "no": 1
      title: COGEBRAS
      page: 0
      pdf_page: 598
    - "no": 2
      title: COASSOCIATIVITY, COCOMMUTATIVITY, COUNIT
      page: 0
      pdf_page: 602
    - "no": 3
      title: PROPERTIES OF GRADED COGEBRAS OF TYPE N
      page: 0
      pdf_page: 608
    - "no": 4
      title: BIGEBRAS AND SKEW-BIGEBRAS
      page: 0
      pdf_page: 609
    - "no": 5
      title: THE GRADED DUALS $T(M)^{*gr}$, $S(M)^{*gr}$ AND $\bigwedge(M)^{*gr}$
      page: 0
      pdf_page: 611
    - "no": 6
      title: 'INNER PRODUCTS: CASE OF ALGEBRAS'
      page: 0
      pdf_page: 618
    - "no": 7
      title: 'INNER PRODUCTS: CASE OF COGEbras'
      page: 0
      pdf_page: 621
    - "no": 8
      title: 'INNER PRODUCTS: CASE OF BIGEBRAS'
      page: 0
      pdf_page: 624
    - "no": 9
      title: INNER PRODUCTS BETWEEN $T(M)$ AND $T(M^*)$, $S(M)$ AND $S(M^*)$, $\Lambda(M)$ AND $\Lambda(M^*)$
      page: 0
      pdf_page: 627
    - "no": 10
      title: EXPLICIT FORM OF INNER PRODUCTS IN THE CASE OF A FINITELY GENERATED FREE MODULE
      page: 0
      pdf_page: 629
    - "no": 11
      title: ISOMORPHISMS BETWEEN $\wedge^p(M)$ AND $\wedge^{n-p}(M^*)$ FOR AN $n$-DIMENSIONAL FREE MODULE M
      page: 0
      pdf_page: 631
    - "no": 12
      title: APPLICATION TO THE SUBSPACE ASSOCIATED WITH A p-VECTOR
      page: 0
      pdf_page: 632
    - "no": 13
      title: PURE $p$-VECTORS. GRASSMANNIANS
      page: 0
      pdf_page: 633
statements: 40
exercises: 25
content_sha256: 90494d968c59422cd10c0c094900dde16ccd49c45c755154b67be626cbb3b8af
---

## § 11. COGEBRAS, PRODUCTS OF MULTILINEAR FORMS, INNER PRODUCTS AND DUALITY

In this paragraph, A is a commutative ring with the trivial graduation. For a graded A-module M of type N, M^{gr} will denote the graded A-module of type N, whose homogeneous elements of degrees n are the A-linear forms which are zero on M_k for all k ≠ n.

### 1. COGEBRAS

#### Definition 1 {#alg-iii-s11-def-1 .statement}

A cogebr a over A (or A-cogebra, or simply cogebr a if no confusion can arise) is a set E with a structure defined by giving the following:
(1) an A-module structure on E;
(2) an A-linear mapping c: E → E ⊗_A E called the coproduct of E.

#### Definition 2 {#alg-iii-s11-def-2 .statement}

Given two cogebras E, E', whose coproducts are denoted respectively by c and c', a morphism of E into E' is an A-linear mapping u: E → E' such that
(1) $(u \otimes u) \circ c = c' \circ u,$ in other words, it renders commutative the diagram of A-linear mappings

$$
\begin{array}{ccc}
E & \xrightarrow{u} & E' \\
\downarrow c & & \downarrow c' \\
E \otimes_A E & \xrightarrow{u \otimes u} & E' \otimes_A E'
\end{array}
$$

It is immediately verified that the identity mapping is a morphism, that the composition of two morphisms is a morphism and that every bijective morphism is an isomorphism.

#### Example {#alg-iii-s11-n1-exa-1 .statement}

(1) The canonical isomorphism $A \to A \otimes_A A$ (II, § 3, no. 5) defines an A-cogebra structure on A.

(2) Let E be a cogebra, $c$ its coproduct and $\sigma$ the canonical automorphism of the A-module $E \otimes_A E$ such that $\sigma(x \otimes y) = y \otimes x$ for $x \in E, y \in E$; the A-linear mapping $\sigma \circ c$ defines a new cogebra structure on E. With this structure E is called the *opposite* cogebra to the given cogebra E.

(3) Let B be an A-*algebra* and let $m : B \otimes_A B \to B$ be the A-linear mapping defining multiplication on B (\S 1, no. 3). The transpose $^t m$ is then an A-linear mapping of the dual $B^*$ of the A-module B into the dual $(B \otimes_A B)^*$ of the A-module $B \otimes_A B$. If also B is a *finitely generated projective* A-module, the canonical mapping $\mu : B^* \otimes_A B^* \to (B \otimes_A B)^*$ is an A-module isomorphism (II, § 4, no. 4); the mapping $c = \mu^{-1} \circ ^t m$ is then a coproduct defining a *cogebra* structure on the *dual* $B^*$ of the A-module B.

(4) Let X be a set, $A^{(X)}$ the A-module of formal linear combinations of elements of X with coefficients in A (II, § 1, no. 11) and $(e_x)_{x \in X}$ the canonical basis of $A^{(X)}$. An A-linear mapping $c : A^{(X)} \to A^{(X)} \otimes_A A^{(X)}$ is defined by the condition $c(e_x) = e_x \otimes e_x$ and a canonical cogebra structure is thus obtained on $A^{(X)}$.

(5) Let M be an A-module and $T(M)$ the tensor algebra of M (\S 5, no. 1); by II, § 3, no. 9 there exists one and only one A-linear mapping $c$ of the A-module $T(M)$ into the A-module $T(M) \otimes_A T(M)$ such that, for all $n \geq 0$,

$$
c(x_1 x_2 \ldots x_n) = \sum_{0 \leq p \leq n} (x_1 x_2 \ldots x_p) \otimes (x_{p+1} \ldots x_n)
$$

for all $x_i \in M$ ($x_1 x_2 \ldots x_n$ denotes the product in the algebra $T(M)$). Thus $T(M)$ is given a *cogebra* structure.

(6) Let M be an A-module and $S(M)$ the symmetric algebra of M (\S 6, no. 1); the diagonal mapping $\Delta : x \mapsto (x, x)$ of M into $M \times M$ is an A-linear mapping to which there therefore corresponds a homomorphism $S(\Delta)$ of the A-algebra $S(M)$ into the A-algebra $S(M \times M)$ (\S 6, no. 2, Proposition 3). On the other hand, in § 6, no. 6 we defined a canonical graded algebra isomorphism $h : S(M \times M) \to S(M) \otimes_A S(M)$; by composition we therefore obtain an *A-algebra* homomorphism

$$
c = h \circ S(\Delta) : S(M) \to S(M) \otimes_A S(M),
$$

thus defining on $S(M)$ a *cogebra* structure. For all $x \in M$, by definition $S(\Delta)(x) = (x, x)$ and the definition of $h$ given in § 6, no. 6 shows that

$$
h((x, x)) = x \otimes 1 + 1 \otimes x.
$$

It follows that $c$ is the unique algebra homomorphism such that, for all $x \in M$,

(4)
$$
c(x) = x \otimes 1 + 1 \otimes x.
$$

As $c$ is an algebra homomorphism, it follows that, for every sequence $(x_i)_{1 \leq i \leq n}$ of $n$ elements of $M$,

(5)
$$
c(x_1 x_2 \ldots x_n) = \prod_{i=1}^n (x_i \otimes 1 + 1 \otimes x_i)
$$
$$
= \sum (x_{i_1} \ldots x_{i_p}) \otimes (x_{j_1} \ldots x_{j_{n-p}})
$$

the summation on the right hand side of (5) being taken over all ordered pairs of strictly increasing sequences (in some cases empty)

$$
i_1 < i_2 < \cdots < i_p, \quad j_1 < j_2 < \cdots < j_{n-p}
$$

of elements of $\{1, n\}$, whose sets of elements are complementary. The element $c(x_1 x_2 \ldots x_n)$ is an element of *total degree* $n$ in $S(M) \otimes_A S(M)$ and its component of bidegree $(p, n-p)$ is

(6)
$$
\sum_{\sigma} (x_{\sigma(1)} \ldots x_{\sigma(p)}) \otimes (x_{\sigma(p+1)} \ldots x_{\sigma(n)})
$$

where the summation is taken over all permutations $\sigma \in S_n$ which are *increasing* in each of the intervals $\{1, p\}$ and $\{p+1, n\}$.

(7) Let $M$ be an $A$-module and proceed with the exterior algebra $\Lambda(M)$ as with $S(M)$ in *Example* 6; the diagonal mapping $\Delta : M \to M \times M$ this time defines a homomorphism $\Lambda(\Delta)$ of the $A$-algebra $\Lambda(M)$ into the $A$-algebra $\Lambda(M \times M)$ (\S 7, no. 2, Proposition 2); on the other hand there is a canonical graded algebra isomorphism

$$
h : \Lambda(M \times M) \to \Lambda(M)^g \otimes_A \Lambda(M)
$$

(\S 7, no. 7, Proposition 10), whence by composition there is an *algebra* homomorphism $c = h \circ \Lambda(\Delta) : \Lambda(M) \to \Lambda(M)^g \otimes_A \Lambda(M)$, which can be considered as an $A$-module homomorphism $\Lambda(M) \to \Lambda(M) \otimes_A \Lambda(M)$ and which therefore defines on $\Lambda(M)$ a *cogebra* structure. It can be proved as in *Example* 6 that $c$ is the unique algebra homomorphism such that, for all $x \in M$,

(7)
$$
c(x) = x \otimes 1 + 1 \otimes x,
$$

whence, for every sequence $(x_i)_{1 \leq i \leq n}$ of elements of $M$,
$$
c(x_1 \wedge x_2 \wedge \cdots \wedge x_n) = (x_1 \otimes 1 + 1 \otimes x_1) \wedge \ldots \wedge (x_n \otimes 1 + 1 \otimes x_n)
$$
where the product on the right hand side is taken in the algebra
$$
\bigwedge(M)^{\mathfrak{g}} \otimes_A \bigwedge(M);
$$
to calculate this product, consider, for every ordered pair of strictly increasing sequences $i_1 < i_2 < \cdots < i_p,\ j_1 < j_2 < \cdots < j_{n-p}$ of elements of $[1, n]$, whose sets of elements are complementary, the product $y_1 y_2 \ldots y_n$, where $y_{i_h} = x_{i_h} \otimes 1$ ($1 \leq h \leq p$) and $y_{j_k} = 1 \otimes x_{j_k}$ ($1 \leq k \leq n - p$) and the sum is taken over all these products. As the graded algebra $\bigwedge(M)^{\mathfrak{g}} \otimes_A \bigwedge(M)$ is anticommutative and the elements $x_i \otimes 1$ and $1 \otimes x_i$ are of total degree 1, by § 4, no. 6, Lemma 3 and Lemma 1,
$$(8)\quad c(x_1 \wedge x_2 \wedge \cdots \wedge x_n)$$
$$
= \sum (-1)^v (x_{i_1} \wedge \cdots \wedge x_{i_p}) \otimes (x_{j_1} \wedge \cdots \wedge x_{j_{n-p}})
$$
$v$ being the number of ordered pairs $(h, k)$ such that $j_k < i_h$ and the summation being taken over the same set as in (5). The element $c(x_1 \wedge \cdots \wedge x_n)$ is of *total degree* $n$ in $\bigwedge(M)^{\mathfrak{g}} \otimes_A \bigwedge(M)$ and its homogeneous component of bi-degree $(p, n - p)$ is equal to
$$(9)\quad \sum_{\sigma} \varepsilon_\sigma (x_{\sigma(1)} \wedge \cdots \wedge x_{\sigma(p)}) \otimes (x_{\sigma(p+1)} \wedge \cdots \wedge x_{\sigma(n)})
$$
the summation being taken over permutations $\sigma \in S_n$ which are *increasing in each of the intervals* $[1, p]$ and $[p + 1, n]$.

When in future we speak of $A^{(x)}, T(M), S(M)$ or $\bigwedge(M)$ as *cogebras*, we shall mean, unless otherwise mentioned, with the cogebra structures defined in *Examples* 4, 5, 6 and 7 respectively.

(8) Let $E, F$ be two $A$-cogebras and $c, c'$ their respective coproducts. Let $\tau : (E \otimes_A E) \otimes_A (F \otimes_A F) \to (E \otimes_A F) \otimes_A (E \otimes_A F)$ denote the associativity isomorphism such that $\tau((x \otimes x') \otimes (y \otimes y')) = (x \otimes y) \otimes (x' \otimes y')$ for $x, x'$ in $E$ and $y, y'$ in $F$. Then the composite linear mapping
$$
E \otimes_A F \xrightarrow{c \otimes c'} (E \otimes_A E) \otimes_A (F \otimes_A F) \xrightarrow{\tau} (E \otimes_A F) \otimes_A (E \otimes_A F)
$$
defines a cogebra structure on the $A$-module $E \otimes_A F$, called the *tensor product* of the cogebras $E$ and $F$.

Let $E$ be a cogebra and $\Delta$ a commutative monoid. A graduation $(E_\lambda)_{\lambda \in \Delta}$ on the $A$-module $E$ is said to be *compatible with the coproduct* $c$ of $E$ if $c$ is a graded homomorphism of degree $O$ of the graded $A$-module $E$ into the graded $A$-module (of type $\Delta$) $E \otimes_A E$, in other words (II, § 11, no. 5) if
$$(10)\quad c(E_\lambda) \subset \sum_{\mu + \nu = \lambda} E_\mu \otimes_A E_\nu.$$

In what follows, we shall most often limit our attention to graduations of type $\mathbf{N}$ compatible with the coproduct; a cogebrà with such a graduation will also be called a *graded cogebrà*. If F is another graded cogebrà, a *graded cogebrà morphism* $\phi : E \to F$ is by definition a cogebrà morphism (Definition 2) which is also a *graded homomorphism of degree* 0 of graded A-modules.

#### Example {#alg-iii-s11-n1-exa-2 .statement}

(9) It is immediate that the cogebras $T(M)$, $S(M)$ and $\Lambda(M)$ defined above are graded cogebras.

### 2. COASSOCIATIVITY, COCOMMUTATIVITY, COUNIT

Let E be a cogebrà, $c$ its coproduct, N, $N'$, $N''$ three A-modules and $m$ a bilinear mapping of $N \times N'$ into $N''$. Let $\tilde{m} : N \otimes_A N' \to N''$ denote the A-linear mapping corresponding to $m$. If $u : E \to N$, $v : E \to N'$ are two A-linear mappings, we derive an A-linear mapping $u \otimes v : E \otimes_A E \to N \otimes_A N'$ and a composite A-linear mapping of E into $N''$:

$$
m(u, v) : E \xrightarrow{c} E \otimes_A E \xrightarrow{u \otimes v} N \otimes_A N' \xrightarrow{\tilde{m}} N''.
$$

Clearly we have thus defined an A-bilinear mapping $(u, v) \mapsto m(u, v)$ of $\mathrm{Hom}_A(E, N) \times \mathrm{Hom}_A(E, N')$ into $\mathrm{Hom}_A(E, N'')$.

When E is a graded cogebrà, N, $N'$, $N''$ graded A-modules of the same type and $\tilde{m}$ a graded homomorphism of degree k of $N \otimes_A N'$ into $N''$, then, if $u$ (resp. $v$) is a graded homomorphism of degree $p$ (resp. $q$), $m(u, v)$ is a graded homomorphism of degree $p + q + k$.

#### Example {#alg-iii-s11-n2-exa-1 .statement}

(1) Take E to be the graded cogebrà $T(M)$ (no. 1) and suppose that N, $N'$, $N''$ have the trivial graduation. A graded homomorphism of degree $-p$ of $T(M)$ into N (resp. $N'$, $N''$) then corresponds to a multilinear mapping of $M^p$ into N (resp. $N'$, $N''$). Given a multilinear mapping $u : M^p \to N$ and a multilinear mapping $v : M^q \to N'$, the above method allows us to deduce a multilinear mapping $m(u, v) : M^{p+q} \to N''$ called the *product* (relative to $m$) of $u$ and $v$. Formulae (3) (no. 1) and (11) show that, for $x_1, \ldots, x_{p+q}$ in M,

$$
(m(u, v))(x_1, \ldots, x_{p+q}) = m(u(x_1, \ldots, x_p), v(x_{p+1}, \ldots, x_{p+q})).
$$

(2) Take E to be the graded cogebrà $S(M)$ (no. 1), preserving the same hypotheses on N, $N'$, $N''$. A graded homomorphism of degree $-p$ of $S(M)$ into N then corresponds to a *symmetric multilinear mapping* of $M^p$ into N (\S 6, no. 3). Then we derive from a symmetric multilinear mapping $u : M^p \to N$ and a symmetric multilinear mapping $v : M^q \to N'$ a symmetric multilinear mapping $m(u, v) : M^{p+q} \to N''$, also denoted (to avoid confusion) by $u._m v$ (or even $u.v$) and called the *symmetric product* (relative to $m$) of $u$ and $v$. Formulae (6) (no. 1) and (11) show that, for $x_1, \ldots, x_{p+q}$ in M,

$$(u \cdot_m v)(x_1, \ldots, x_{p+q}) = \sum_\sigma m(u(x_{\sigma(1)}, \ldots, x_{\sigma(p)}), v(x_{\sigma(p+1)}, \ldots, x_{\sigma(p+q)}))$$

the summation being taken over permutations $\sigma \in \mathfrak{S}_{p+q}$ which are increasing on each of the intervals $[1, p]$ and $[p+1, p+q]$.

(3) Take E to be the graded cogebra $\bigwedge(M)$ (no. 1). Then we deduce similarly from an alternating multilinear mapping $u : M^p \to N$ and an alternating multilinear mapping $v : M^q \to N'$ an alternating multilinear mapping $m(u, v) : M^{p+q} \to N''$, also denoted by $u \wedge_m v$ or $u \wedge v$ and called the *alternating product* (relative to $m$) of $u$ and $v$. Formulae (9) (no. 1) and (11) show in this case that, for $x_1, \ldots, x_{p+q}$ in $M$,

$$(u \wedge_m v)(x_1, \ldots, x_{p+q}) = \sum_\sigma \varepsilon_\sigma m(u(x_{\sigma(1)}, \ldots, x_{\sigma(p)}), v(x_{\sigma(p+1)}, \ldots, x_{\sigma(p+q)}))$$

the summation again being taken over permutations $\sigma \in \mathfrak{S}_{p+q}$ which are increasing on each of the intervals $[1, p]$ and $[p+1, p+q]$.

We return to the case where E is an arbitrary graded cogebra (of type N) and assume that the three modules N, N', N'' are all equal to the underlying A-module of a *graded A-algebra* B of type $\mathbf{Z}$, the mapping $m$ being multiplication in B, so that $\tilde{m} : B \otimes_A B \to B$ is a graded A-linear mapping of degree 0. Thus a *graded A-algebra* structure is obtained on the graded A-module $\mathrm{Homgr}_A(E, B) = C$.

In particular, suppose that $B = A$ (with the trivial graduation), so that $\mathrm{Homgr}_A(E, A)$ is the *graded dual* $E^{*gr}$, which thus has a graded A-algebra structure.

Let F be another graded cogebra $c'$ its coproduct and $\phi : E \to F$ a graded cogebra morphism (no. 1); then the canonical graded morphism

$$\tilde{\phi} = \mathrm{Hom}(\phi, 1_B) : \mathrm{Homgr}_A(F, B) \to \mathrm{Homgr}_A(E, B)$$

is a *graded algebra homomorphism*. For $u, v$ in $\mathrm{Homgr}_A(F, B)$ and $x \in E$,

$$(\tilde{\phi}(uv))(x) = (uv)(\phi(x)) = m((u \otimes v)(c'(\phi(x)))).$$

But by hypothesis $c'(\phi(x)) = (\phi \otimes \phi)(c(x))$, hence

$$(u \otimes v)(c'((x))) = (\tilde{\phi}(u) \otimes \tilde{\phi}(v))(c(x))$$

and therefore $\tilde{\phi}(uv) = \tilde{\phi}(u)\tilde{\phi}(v)$, which proves our assertion.

In particular, the graded transpose $^t\phi : F^{*gr} \to E^{*gr}$ is a graded algebra homomorphism.

#### Remark {#alg-iii-s11-n2-rem-1 .statement}

Suppose that the $E_p$ are finitely generated projective $A$-modules, so that the graded $A$-modules $(E \otimes_A E)^{*gr}$ and $E^{*gr} \otimes_A E^{*gr}$ can be canonically identified (II, § 4, no. 4, Corollary 1 to Proposition 4). If also the $A$-modules $A \otimes_A A$ and $A$ are then canonically identified (II, § 3, no. 4), the linear mapping $E^{*gr} \otimes_A E^{*gr} \to E^{*gr}$ which defines multiplication in $E^{*gr}$ can be called the graded transpose of the coproduct $c$.

#### Proposition 1 {#alg-iii-s11-prop-1 .statement}

*Let $E$ be a cogebra over $A$. In order that, for every associative $A$-algebra $B$, the $A$-algebra $\mathrm{Hom}_A(E, B)$ be associative, it is necessary and sufficient that the coproduct $c : E \to E \otimes_A E$ be such that the diagram*

$$
\begin{array}{ccc}
E & \xrightarrow{c} & E \otimes_A E \\
\downarrow c & & \downarrow l_E \otimes c \\
E \otimes_A E & \xrightarrow{c \otimes l_E} & E \otimes_A E \otimes_A E
\end{array}
$$

*be commutative.*

Let $B$ be an associative $A$-algebra and $u, v, w$ three elements of $C = \mathrm{Hom}_A(E, B)$. Let $m_3$ denote the $A$-linear mapping $B \otimes_A B \otimes_A B \to B$ which maps $b \otimes b' \otimes b''$ to $bb'b''$. By definition of the product on the algebra $C$, $(uv)w$ is the composite mapping

$$
E \xrightarrow{c} E \otimes E \xrightarrow{c \otimes 1_E} E \otimes E \otimes E \xrightarrow{u \otimes v \otimes w} B \otimes B \otimes B \xrightarrow{m_3} B
$$

whilst $u(vw)$ is the composite mapping

$$
E \xrightarrow{c} E \otimes E \xrightarrow{l_E \otimes c} E \otimes E \otimes E \xrightarrow{u \otimes v \otimes w} B \otimes B \otimes B \xrightarrow{m_3} B.
$$

It follows that if diagram (12) is commutative, the algebra $\mathrm{Hom}_A(E, B)$ is associative for every associative $A$-algebra $B$. To establish the converse, it suffices to show that there exists an associative $A$-algebra $B$ and three $A$-linear mappings $u, v, w$ of $E$ into $B$ such that the mapping $m_3 \circ (u \otimes v \otimes w)$ of $E \otimes E \otimes E$ into $B$ is injective. Take $B$ to be the $A$-algebra $\mathcal{T}(E)$ and $u, v, w$ the canonical mapping of $E$ into $\mathcal{T}(E)$. The mapping $m_3 \circ (u \otimes v \otimes w)$ is then the canonical mapping $E \otimes E \otimes E = \mathcal{T}^3(E) \to \mathcal{T}(E)$, which is injective.

When the cogebra $E$ satisfies the condition of Proposition 1, it is said to be coassociative.

#### Example {#alg-iii-s11-n2-exa-2 .statement}

(4) It is immediately verified that the cogebra $A$ (no. 1, Example (1)) the cogebra $A^{(X)}$ (no. 1, Example 4) and the cogebra $\mathcal{T}(M)$ (no. 1, Example 5) are coassociative. If $B$ is an associative $A$-algebra which is a finitely generated projective $A$-module, the cogebra $B^*$ (no. 1, Example 3) is coassociative: for the commutativity of diagram (12) then follows by transposition from that of the diagram which expresses the associativity of $B$ (\S 1, no. 3). Conversely, the same argument and the canonical identification of the A-module B with its bidual (II, § 2, no. 7, Corollary 4 to Proposition 13) show that if the cogebras B* is coassociative, the algebra B is associative. Finally, the cogebras S(M) and $\Lambda(M)$ (no. 1, Examples 6 and 7) are coassociative; this follows from the commutativity of the diagram

$$
\begin{array}{ccc}
M & \xrightarrow{\Delta} & M \times M \\
\downarrow & & \downarrow 1_M \times \Delta \\
M \times M & \xrightarrow{\Delta \times 1_M} & M \times M \times M
\end{array}
$$

the functorial properties of S(M) (\S 6, no. 2) and $\Lambda(M)$ (\S 7, no. 2), which give the corresponding commutative diagrams

$$
\left\{
\begin{array}{ccc}
S(M) & \xrightarrow{S(\Delta)} & S(M \times M) \\
\downarrow S(\Delta) & & \downarrow S(\Delta_M \times 1) \\
S(M \times M) & \xrightarrow{S(\Delta \times 1_M)} & S(M \times M \times M)
\end{array}
\right.
$$
$$
\left\{
\begin{array}{ccc}
\Lambda(M) & \xrightarrow{\Lambda(\Delta)} & \Lambda(M \times M) \\
\downarrow \Lambda(\Delta) & & \downarrow \Lambda(1_M \times \Delta) \\
\Lambda(M \times M) & \xrightarrow{\Lambda(\Delta \times 1_M)} & \Lambda(M \times M \times M)
\end{array}
\right.
$$

and the existence and functoriality of canonical isomorphisms for symmetric and exterior algebras of a direct sum (\S 6, no. 6 and \S 7, no. 7).

#### Proposition 2 {#alg-iii-s11-prop-2 .statement}

*Let E be a cogebras over A. In order that, for every commutative A-algebra B, the A-algebra $\mathrm{Hom}_A(E, B)$ be commutative, it is necessary and sufficient that the coproduct $c : E \to E \otimes_A E$ be such that the diagram*

$$
\begin{array}{ccc}
E & & \\
 & \swarrow_c & \searrow_c \\
E \otimes_A E & \xrightarrow{\sigma} & E \otimes_A E
\end{array}
$$

(where $\sigma$ is the symmetry homomorphism such that $\sigma(x \otimes y) = y \otimes x$) is *commutative* (in other words, it suffices that the cogebras E be *identical with its opposite* (no. 1, Example 2).

Let B be a commutative A-algebra and $u, v$ two elements of $C = \mathrm{Hom}_A(E, B)$.

By definition of the product in C, $uv$ and $vu$ are respectively equal to the composite mappings

$$
E \xrightarrow{c} E \otimes E \xrightarrow{u \otimes v} B \otimes B \xrightarrow{m} B
$$

and

$$
E \xrightarrow{c} E \otimes E \xrightarrow{v \otimes u} B \otimes B \xrightarrow{m} B.
$$

It follows that if diagram (15) is commutative the algebra $\mathrm{Hom}_A(E, B)$ is commutative for every commutative A-algebra B. To establish the converse, it suffices to show that there exist a commutative A-algebra B and two A-linear mappings $u, v$ of E into B such that $m \circ (u \otimes v): E \otimes E \to B$ is injective. Take B to be the algebra $S(E \oplus E)$ and $u$ (resp. $v$) the composition of the canonical mapping $E \oplus E \to S(E \oplus E)$ and the mapping $x \mapsto (x, 0)$ (resp. $x \mapsto (0, x)$) of E into $E \oplus E$. If $h: S(E) \otimes S(E) \to S(E \otimes E)$ is the canonical isomorphism (\S 6, no. 6, Proposition 9) and $\lambda: E \to S(E)$ is the canonical mapping, then $h^{-1} \circ m \circ (u \otimes v) = \lambda \otimes \lambda$. Now $\lambda \otimes \lambda$ is injective, for $\lambda(E)$ is a direct factor of $S(E)$ (II, \S 3, no. 7, Corollary 5 to Proposition 7).

When the cogebra E satisfies the condition of Proposition 2, it is said to be cocommutative.

#### Example {#alg-iii-s11-n2-exa-3 .statement}

(5) It is immediate that the cogebra A (no. 1, Example 1) and the cogebra $A^{(X)}$ (II, \S 11, no. 1, Example 4) are cocommutative. It follows from formula (5) of no. 1 that the cogebra $S(M)$ is cocommutative. Finally, for an A-algebra B such that the A-module B is projective and finitely generated to have the property that the cogebra $B^*$ (no. 1, Example 3) is cocommutative, it is necessary and sufficient that B be commutative; for (using the canonical identification of the A-module B with its bidual (II, \S 2, no. 7)), this follows from the fact that the commutativity of diagram (14) is equivalent by transposition to that of the diagram which expressed the commutativity of B (\S 1, no. 3).

#### Proposition 3 {#alg-iii-s11-prop-3 .statement}

*Let E be a cogebra over A. In order that, for every unital A-algebra B, the A-algebra $\mathrm{Hom}_A(E, B)$ be unital, it is necessary and sufficient that there exist a linear form $\gamma$ on E rendering commutative the diagrams*

$$
\begin{array}{ccc}
E & \xrightarrow{c} & E \otimes_A E \\
& & \downarrow \gamma \otimes 1_E \\
& & A \otimes_A E
\end{array}
$$
$h'$

$$
\begin{array}{ccc}
E & \xrightarrow{c} & E \otimes_A E \\
& & \downarrow 1_E \otimes \gamma \\
& & E \otimes_A A
\end{array}
$$
$h''$

where $c: E \to E \otimes_A E$ is the coproduct and $h'$ and $h''$ the canonical isomorphisms

(II, § 3, no. 4, Proposition 4). *The unit of* Hom$_A$(E, B) *is then the linear mapping* x $\mapsto$ $\gamma(x)1$ (where 1 denotes the unit element of B).

Let $\gamma$ be a linear form on E rendering diagram (16) commutative. Let B be a unital A-algebra with unit element 1, $\eta:A \to B$ the canonical mapping and $v = \eta \circ \gamma$ the element of the A-algebra C = Hom$_A$(E, B). For every element $u \in C$, $uv$ is the composite mapping

$$
\text{(17)} \quad E \xrightarrow{c} E \otimes E \xrightarrow{1_E \otimes \gamma} E \otimes A \xrightarrow{u \otimes \eta} B \otimes B \xrightarrow{m} B.
$$

Then $uv = m \circ (u \otimes \eta) \circ h'' = u$. It is similarly proved that $vu = u$ and hence $v$ is unit element of C. Conversely, let the A-module A $\oplus$ E be given a unital algebra structure such that $(a, x)(a', x') = (aa', ax' + a'x)$ for $a, a'$ in A and $x, x'$ in E. Let B denote the A-algebra thus defined and let C be the A-algebra Hom$_A$(E, B). Suppose that C is unital and let $e:x \mapsto (\gamma(x), \lambda(x))$ be its unit element (where $\gamma(x) \in A$ and $\lambda(x) \in E$). On the other hand let $f$ be the element $x \mapsto (0, x)$ of C. An immediate calculation shows that $fe$ is the element

$$
x \mapsto (0, (h'')^{-1}((1_E \otimes \gamma)(c(x))))
$$

of C. The condition $fe = f$ implies the commutativity of the second diagram of (16) and it is similarly seen that the condition $ef = f$ implies the commutativity of the first diagram of (16).

A linear form $\gamma$ on E rendering diagrams (16) commutative is called a *counit* of the cogebra E. A cogebra admits *at most one* counit: for it is the unit element of the algebra Hom$_A$(E, A). A cogebra with a counit is called *counital*.

#### Example {#alg-iii-s11-n2-exa-4 .statement}

(6) The identity mapping is the counit of the cogebra A; on the cogebra A$^{(X)}$ (no. 1, *Example 4*) the linear form $\gamma$ such that $\gamma(e_x) = 1$ for all $x \in X$ is the counit. On the cogebra T(M) (resp. S(M), $\Lambda(M)$) the linear form $\gamma$ such that $\gamma(1) = 1$ and $\gamma(z) = 0$ for $z$ in the $T^n(M)$ (resp. $S^n(M)$, $\Lambda^n(M)$) for $n \geq 1$ is the counit. Finally, let B be an A-algebra which is a finitely generated projective A-module and has a unit element $e$; then on the cogebra B* (no. 1, *Example 3*) the linear form $\gamma: x^* \mapsto \langle e, x^* \rangle$ is the counit, for this form is just the transpose of the A-linear mapping $\eta_e: \xi \mapsto \xi e$ of A into B and by transposition the commutativity of diagrams (16) follows from that of the diagrams which express (using $\eta_e$) the fact that $e$ is unit element of B (§ 1, no. 3); the same argument moreover shows that conversely, if the cogebra B* admits a counit $\gamma$, the transpose of $\gamma$ defines a unit element $e = t_\gamma(1)$ of B.

#### Proposition 4 {#alg-iii-s11-prop-4 .statement}

*Let E be a cogebra admitting a counit $\gamma$ and suppose that there exists in E an element e such that $\gamma(e) = 1$; then E is the direct sum of the sub-A-modules Ae and $E_{\gamma} = \mathrm{Ker}(\gamma)$ and*

$$
\text{(18)} \quad \begin{cases}
c(e) \equiv e \otimes e \pmod{E_{\gamma} \otimes E_{\gamma}} \\
c(x) \equiv x \otimes e + e \otimes x \pmod{E_{\gamma} \otimes E_{\gamma}} & \text{for all } x \in E_{\gamma}.
\end{cases}
$$

The first assertion is immediate, for $\gamma(x - \gamma(x)e) = 0$ and the relation $\gamma(\alpha e) = 0$ implies $\alpha = 0$. Let $c(e) = \sum_i s_i \otimes t_i$, so that
$$
e = \sum_i \gamma(s_i)t_i = \sum_i \gamma(t_i)s_i
$$
by (16) and $1 = \gamma(e) = \sum_i \gamma(s_i)\gamma(t_i)$. Therefore
$$
\sum_i (s_i - \gamma(s_i)e) \otimes (t_i - \gamma(t_i)e) = \sum_i s_i \otimes t_i - \sum_i e \otimes \gamma(s_i)t_i \\
- \sum_i \gamma(t_i)s_i \otimes e \\
+ \sum_i \gamma(s_i)e \otimes \gamma(t_i)e
$$
which, by the above relation, is just $c(e) - e \otimes e$; this therefore proves the first relation of (18). On the other hand the decomposition of $E \otimes E$ as a direct sum
$$
A(e \otimes e) \oplus ((Ae) \otimes E_\gamma) \oplus (E_\gamma \otimes (Ae)) \oplus (E_\gamma \otimes E_\gamma)
$$
allows us to write, for $x \in E_\gamma$, $c(x) = \lambda(e \otimes e) + (e \otimes y) + z \otimes e) + u$ where $u = \sum_j v_j \otimes w_j, y, z$ and the $v_j$ and $w_j$ belong to $E_\gamma$. The definition of the counit $\gamma$ then gives $x = \lambda e + y = \lambda e + z$ and, as $\gamma(x) = 0$, necessarily $\lambda = 0, x = y = z$, whence the second relation of (18).

#### Remark {#alg-iii-s11-n2-rem-2 .statement}

Let C be a counital coassociative A-coalgebra, B a unital associative A-algebra and M a left B-module. The A-bilinear mapping $(b, m) \mapsto bm$ of $B \times M$ into M defines an A-bilinear mapping
$$
\operatorname{Hom}_A(C, B) \times \operatorname{Hom}_A(C, M) \to \operatorname{Hom}_A(C, M)
$$
by the general procedure described at the beginning of this no. It is immediately verified that this mapping defines on $\operatorname{Hom}_A(C, M)$ a left module structure over the ring $\operatorname{Hom}_A(C, B)$.

### 3. PROPERTIES OF GRADED COGEBRAS OF TYPE N

#### Proposition 5 {#alg-iii-s11-prop-5 .statement}

(i) *Let E be a graded cogebra admitting a counit $\gamma$; then $\gamma$ is a homogeneous linear form of degree 0.*

(ii) *Suppose further that there exists an element $e \in E$ such that $E_0 = Ae$ and $\gamma(e) = 1$. Then the kernel $E_\gamma$ of $\gamma$ is equal to $E_+ = \sum_{n \geq 1} E_n$, $c(e) = e \otimes e$ and*
$$
c(x) \equiv x \otimes e + e \otimes x \ (\text{mod. } E_+ \otimes E_+)
$$
*for all* $x \in E_+$.

(i) It suffices to verify that $\gamma(x) = 0$ for $x \in E_n$, for all $n \geq 1$. Since $c$ is a graded homomorphism of degree 0,

$$
c(x) = \sum_{0 \leq j \leq n} \left( \sum_i y_{ij} \otimes z_{i, n-j} \right)
$$

with, for all $j$ such that $0 \leq j \leq n$, $y_{ij}$ and $z_{ij}$ in $E_j$; applying (16) (no. 2) we obtain

$$
x = \sum_{0 \leq j \leq n} \left( \sum_i \gamma(y_{ij}) z_{i, n-j} \right) = \sum_{0 \leq j \leq n} \left( \sum_i \gamma(z_{i, n-j}) y_{ij} \right),
$$

whence, equating the components of degree 0 and degree $n$ on the two sides

$$
x = \sum_i \gamma(y_{i0}) z_{in} = \sum_i \gamma(z_{i0}) y_{in}
$$
$$
0 = \sum_i \gamma(y_{in}) z_{i0} = \sum_i \gamma(z_{in}) y_{i0}
$$

and therefore $\gamma(x) = \sum_i \gamma(y_{in}) \gamma(z_{i0}) = \gamma(0) = 0$.

(ii) Since $\mathrm{Ker}(\gamma)$ and $E_+$ are both supplementary sub-A-modules of $Ae = E_0$ and $E_+ \subset \mathrm{Ker}(\gamma)$ by (i), $E_+ = \mathrm{Ker}(\gamma)$ (II, § 1, no. 8, Remark 1); the other assertions follow from Proposition 4 of no. 2.

#### Proposition 6 {#alg-iii-s11-prop-6 .statement}

*Let E be a graded cogebra over A. In order that, for every commutative A-algebra B, with the trivial graduation, the graded A-algebra of type $\mathbf{Z} \mathrm{Homgr}_A(E, B)$ (no. 2) be anticommutative (\S 4, no. 9, Definition 7), it is necessary and sufficient that, if $\sigma_g$ denotes the automorphism of the A-module $E \otimes_A E$ such that*

$$
\sigma_g(x_p \otimes x_q) = (-1)^{pq} x_q \otimes x_p
$$

for $x_p \in E_p, x_q \in E_q$, *where p and q are arbitrary elements of $\mathbf{N}$, the diagram*

$$
\begin{array}{ccc}
E & & \\
 & \searrow^c & \swarrow^c \\
E \otimes_A E & \xrightarrow{\sigma_g} & E \otimes_A E
\end{array}
$$

*be commutative.*

The proof is analogous to that of Proposition 2 of no. 2.

When the graded cogebra E satisfies the condition of Proposition 6, it is said to be *anticocommutative*.

#### Example {#alg-iii-s11-n3-exa-1 .statement}

It follows immediately from formula (8) of no. 1 that for every A-module M, the graded cogebra $\bigwedge(M)$ is *anticocommutative*.

### 4. BIGEBRAS AND SKEW-BIGEBRAS

#### Definition 3 {#alg-iii-s11-def-3 .statement}

*A graded bigebra (resp. skew graded bigebra) over a ring A is a set E with a graded A-algebra structure of type $\mathbf{N}$ and a graded A-cogebra structure of type $\mathbf{N}$, with the same underlying graded A-module structure and such that:*

(1) *The A-algebra E is associative and unital.*

(2) *The A-cogebra E is coassociative and counital.*
(3) *The coproduct c : E \to E \otimes_A E is a homomorphism of the graded algebra E into the graded algebra E \otimes_A E* (resp. *graded algebra E^g \otimes_A E* (cf. § 4, no. 7)).
(4) *The counit $\gamma$ of E is a homomorphism of the graded algebra E into the algebra A (with the trivial graduation) such that, if e denotes the unit element of the A-algebra E, $\gamma(e) = 1$.*

If E is a graded bigebra whose graduation is *trivial*, E is called simply a *bigebra*. A graded bigebra is called commutative (resp. cocommutative) if the underlying algebra is commutative (resp. if the underlying cogebra is cocommutative); a skew graded bigebra is called anticommutative (resp. anticocommutative) if the underlying graded algebra is anticommutative (resp. if the underlying graded cogebra is anticocommutative).

It follows from Definition 3 and no. 2, Proposition 5 that, for a graded bigebra or a skew graded bigebra E,

$$
c(e) = e \otimes e \\
c(x) \equiv x \otimes e + e \otimes x (\text{mod. } E_+ \otimes E_+) \quad \text{for } x \in E_+ = \bigoplus_{n \geq 1} E_n.
$$

If E and F are two graded bigebras (resp. two skew graded bigebras), a mapping $\phi : E \to F$ is called a *graded bigebra morphism* (resp. *skew graded bigebra morphism*) if: (1) $\phi$ is a graded algebra morphism (and hence maps the unit element of E to the unit element of F); (2) $\phi$ is a graded cogebra morphism such that, if $\gamma$ and $\gamma'$ are the respective counits of E and F, then $\gamma = \gamma' \circ \phi$.

#### Example {#alg-iii-s11-n4-exa-1 .statement}

(1) Let S be a monoid with identity element u, so that the algebra $E = A^{(S)}$ of the monoid S over A admits the unit element $e_u$ (§ 2, no. 6); it has been seen on the other hand that E has canonically a coassociative cocommutative A-cogebra structure with a counit $\gamma$ such that $\gamma(e_s) = 1$ for all $s \in S$ (no. 1, Example 4 and no. 2, Examples 4, 5 and 6). The formula $c(e_s) = e_s \otimes e_s$ giving the coproduct shows also immediately that c is an algebra homomorphism. Thus a *cocommutative bigebra* structure has been defined on E and E, with this structure, is called the *bigebra of the monoid S over A*.

If T is another monoid with unit element v, $f : S \to T$ a homomorphism such that $f(u) = v$ and $f_{(A)} : A^{(S)} \to A^{(T)}$ the A-algebra homomorphism derived from $f$ (§ 2, no. 6), it is immediately verified that $f_{(A)}$ is a *bigebra homomorphism*.

(2) Let M be an A-module. The graded A-algebra (§ 6, no. 1) and graded A-cogebra (no. 1, Example 6) structures defined on S(M) define on this set a *commutative cocommutative graded bigebra* structure; for we have seen (no. 1, Example 6) that the coproduct on S(M) is an *algebra* homomorphism and it follows from the definition of the counit $\gamma$ (no. 2, Example 6) that $\gamma(1) = 1$ and that $\gamma$ is an algebra homomorphism of E into A.

(3) Let M be an A-module. We see as in Example 2 that the graded A-algebra (\S 7, no. 1) and graded A-cogebra (no. 1, Example 7) structures on $\bigwedge(M)$ define on this set an *anticommutative anticocommutative skew graded bigebra* structure.

#### Remark {#alg-iii-s11-n4-rem-1 .statement}

If M is an A-module such that $M \otimes_A M \neq \{0\}$, the graded A-algebra (\S 5, no. 1) and graded A-cogebra (no. 1, Example 5) structures on $T(M)$ *do not define* a bigebra structure, for in general

$$
c(x_1 x_2 y_1 y_2) \neq c(x_1 x_2) c(y_1 y_2)
$$

for four elements $x_1, x_2, y_1, y_2$ of M, as formula (3) of no. 1, shows.

### 5. THE GRADED DUALS $T(M)^{*gr}$, $S(M)^{*gr}$ AND $\bigwedge(M)^{*gr}$

*From now on we return to the general conventions of the chapter on algebras, which will therefore be assumed (unless otherwise mentioned) to be associative and unital.*

Let M be an A-module; the graded A-cogebra structures defined on $T(M)$ (no. 1, Example 5), $S(M)$ (no. 1, Example 6) and $\bigwedge(M)$ (no. 1, Example 7) allow us to define canonically on the graded duals $T(M)^{*gr}$, $S(M)^{*gr}$ and $\bigwedge(M)^{*gr}$ *graded algebra* structures of type N, by virtue of no. 2, Propositions 1 and 3 and the convention made on the graduation of the graded dual of a graded module (no. 1). Moreover, the graded algebra $S(M)^{*gr}$ is *commutative* (no. 2, Proposition 2 and Example 5) and the graded algebra $\bigwedge(M)^{*gr}$ is *anticommutative* (no. 3, Proposition 6 and Example). In $\bigwedge(M)^{*gr}$ *every element of degree 1 is of zero square*; such an element is identified with a linear form $f$ on M and its square is the alternating bilinear form $f \wedge f$ on $M^2$ such that

$$
(f \wedge f)(x, y) = f(x) f(y) - f(y) f(x)
$$

(no. 2, Example 3).

Let N be another A-module and $u$ an A-linear mapping of M into N. We know that $u$ defines canonically graded algebra homomorphisms

$$
\begin{cases}
T(u): T(M) \to T(N) \\
S(u): S(M) \to S(N) \\
\bigwedge(u): \bigwedge(M) \to \bigwedge(N)
\end{cases}
$$

(\S 5, no. 2, \S 6, no. 2 and \S 7, no. 2). It is immediately verified in formula (3) of no. 1 that $T(u)$ is also a *cogebra morphism*. On the other hand, if $\Delta_M$ (resp. $\Delta_N$) denotes the diagonal mapping $M \to M \times M$ (resp. $N \to N \times N$), there is the relation $(u \times u) \circ \Delta_M = \Delta_N \circ u$; it follows that $S(u \times u) \circ S(\Delta_M) = S(\Delta_N) \circ S(u)$

(resp. $\Lambda(u \times u) \circ \Lambda(\Delta_M) = \Lambda(\Delta_N) \circ \Lambda(u)$).

Using the definition of coproduct in $S(M)$ and $\Lambda(M)$ (no. 1, Examples 6 and 7) and the functorial character of the canonical isomorphisms

$$
S(M \times M) \to S(M) \otimes_A S(M)
$$

and $\Lambda(M \times M) \to \Lambda(M)^{\text{g}} \otimes_A \Lambda(M)$, it is seen that $S(u)$ and $\Lambda(u)$ are also *cogebra morphisms*† (and hence in this case *bigebra* morphisms). It follows immediately that the *graded transposes* (II, § 11, no. 6) of the homomorphisms (23)

$$
\begin{align*}
tT(u): T(N)^{*gr} &\to T(M)^{*gr} \\
tS(u): S(N)^{*gr} &\to S(M)^{*gr} \\
t\Lambda(u): \Lambda(N)^{*gr} &\to \Lambda(M)^{*gr}
\end{align*}
$$

are *graded algebra homomorphisms*.

We now note that the dual $M^*$ of $M$ is identified with the submodule of elements of degree 1 in $T(M)^{*gr}$ (resp. $S(M)^{*gr}$, $\Lambda(M)^{*gr}$). It therefore follows from the universal property of the tensor algebra (\S 5, no. 1) and the universal property of the symmetric algebra (\S 6, no. 1) that *there exists one and only one graded algebra homomorphism*

$$
\theta_T: T(M^*) \to T(M)^{*gr}
$$

*which extends the canonical injection* $M^* \to T(M)^{*gr}$, *and one and only one graded algebra homomorphism*

$$
\theta_S: S(M^*) \to S(M)^{*gr}
$$

*which extends the canonical injection* $M^* \to S(M)^{*gr}$. On the other hand, the canonical injection of $M^*$ in the *opposite* algebra to $\Lambda(M)^{*gr}$ is such that the square of every element of $M^*$ is zero; hence (\S 7, no. 1, Proposition 1) *there exists one and only one graded algebra homomorphism*

$$
\theta_\Lambda: \Lambda(M^*) \to (\Lambda(M)^{*gr})^0
$$

*which extends the canonical injection* $M^* \to \Lambda(M)^{*gr}$.‡ These homomorphisms

† This also follows from formulae (5) and (9) of no. 1.
‡ This injection is extended to a homomorphism into the opposite algebra to $\Lambda(M)^{*gr}$ instead of a homomorphism into $\Lambda(M)^{*gr}$ for reasons of convenience in the calculations.

are functorial: for example, for every $A$-module homomorphism $u : M \to N$, the diagram

$$
\begin{array}{ccc}
T(N^*) & \xrightarrow{T(tu)} & T(M^*) \\
\theta_T \downarrow & & \theta_T \downarrow \\
T(N)^{*gr} & \xrightarrow{t_{T(n)}} & T(M)^{*gr}
\end{array}
$$

is commutative, as follows immediately from the universal property of the tensor algebra (\S 5, no. 1); there are analogous commutative diagrams for $\theta_S$ and $\theta_\wedge$.

We shall find the homomorphisms $\theta_T, \theta_S$ and $\theta_\wedge$ explicitly. For this we consider more generally a coassociative $A$-cogebra $E$ with coproduct $c$ and define by induction on $n$, for $n \geq 2$, the linear mapping $c_n$ of $E$ into $E^{\otimes n}$ by $c_2 = c$ and
$$
c_n = (c_{n-1} \otimes 1_E) \circ c.
$$
On the other hand we denote by $m_n : A^{\otimes n} \to A$ the canonical linear mapping such that $m_n(\xi_1 \otimes \xi_2 \otimes \cdots \otimes \xi_n) = \xi_1 \xi_2 \cdots \xi_n$ and note that, for $n \geq 2$,
$$
m_n = m \circ (m_{n-1} \otimes 1_A)
$$
writing $m = m_2$. With this notation:

#### Lemma 1 {#alg-iii-s11-lem-1 .statement}

(i) *In the associative algebra $E^* = \mathrm{Hom}_A(E, A)$, the product of $n$ elements $u_1, u_2, \ldots, u_n$ of degree 1 is given by*
$$
u_1 u_2 \ldots u_n = m_n \circ (u_1 \otimes u_2 \otimes \cdots \otimes u_n) \circ c_n.
$$
(ii) *Suppose also that the cogebra $E$ is graded. Then, in the graded associative algebra $E^{*gr} = \mathrm{Homgr}_A(E, A)$, the product of $n$ elements $u_1, u_2, \ldots, u_n$ of degree 1 is given by*
$$
u_1 u_2 \ldots u_n = m_n \circ (u_1 \otimes u_2 \otimes \cdots \otimes u_n) \circ \delta_n
$$
*where $\delta_n : E \to E^{\otimes n}$ is the linear mapping which maps each $x \in E$ to the component of $c_n(x)$ of multidegree $(1, 1, \ldots, 1)$.*

Formula (26) is just the definition of the product in $E^*$ for $n = 2$; to prove it by induction on $n$, observe that
$$
u_1 u_2 \ldots u_n
$$
$$
= m \circ ((u_1 u_2 \ldots u_{n-1}) \otimes u_n) \circ c
$$
$$
= m \circ ((m_{n-1} \circ (u_1 \otimes u_2 \otimes \cdots \otimes u_{n-1}) \circ c_{n-1}) \otimes u_n) \circ c
$$
$$
= m \circ (m_{n-1} \otimes 1_A) \circ (u_1 \otimes u_2 \otimes \cdots \otimes u_{n-1} \otimes u_n) \circ (c_{n-1} \otimes 1_E) \circ c
$$
$$
= m_n \circ (u_1 \otimes u_2 \otimes \cdots \otimes u_n) \circ c_n
$$
by virtue of (24), (25), II, \S 3, no. 3, formula (5) and the relation
$$
u_n = 1_A \circ u_n \circ 1_{E^*}.
$$

When E is graded and the elements $u_i \in E^{*gr}$ homogeneous of degree 1, then by definition for *homogeneous* elements $x_i \in E$,

$$
(u_1 \otimes u_2 \otimes \cdots \otimes u_n)(x_1 \otimes x_2 \otimes \cdots \otimes x_n) = 0
$$

unless all the $x_i$ are of degree 1, whence formula (27).

It follows from formulae (3), (5) and (7) of no. 1 and formula (24) that when E is taken to be one of the three graded cogebras $\mathbf{T}(M)$, $\mathbf{S}(M)$ and $\mathbf{\Lambda}(M)$, we obtain respectively by induction on $n$ (using the fact that the coproduct is a graded homomorphism of degree 0), for $x_1, x_2, \ldots, x_n$ in M:

when $E = \mathbf{T}(M)$,
$$
\delta_n(x_1 x_2 \cdots x_n) = x_1 \otimes x_2 \otimes \cdots \otimes x_n
$$

when $E = \mathbf{S}(M)$,
$$
\delta_n(x_1 x_2 \cdots x_n) = \sum_{\sigma \in \mathfrak{S}_n} x_{\sigma(1)} \otimes x_{\sigma(2)} \otimes \cdots \otimes x_{\sigma(n)}
$$

when $E = \mathbf{\Lambda}(M)$,
$$
\delta_n(x_1 x_2 \cdots x_n) = \sum_{\sigma \in \mathfrak{S}_n} \varepsilon_\sigma \cdot x_{\sigma(1)} \otimes x_{\sigma(2)} \otimes \cdots \otimes x_{\sigma(n)}.
$$

It suffices to note, for example when $E = \mathbf{\Lambda}(M)$, that in the expression
$$
c_n(x_1 x_2 \cdots x_n) = (c_{n-1} \otimes 1_E) \left( \sum (-1)^v (x_{i_1} \ldots x_{i_p}) \otimes (x_{j_1} \ldots x_{j_{n-p}}) \right)
$$
arising from formula (8) of no. 1, the only terms which can give a term of multidegree $(1, 1, \ldots, 1)$ are those for which $n - p = 1$ and hence
$$
\delta_n(x_1 x_2 \cdots x_n)
$$
is the term of multidegree $(1, 1, \ldots, 1)$ in the sum
$$
\sum_{i=1}^n (-1)^{n-i} c_{n-1}(x_1 \ldots x_{i-1} x_{i+1} \ldots x_n) \otimes x_i
$$
and this term is necessarily equal to
$$
\sum_{i=1}^n (-1)^{n-i} \delta_{n-1}(x_1 \ldots x_{i-1} x_{i+1} \ldots x_n) \otimes x_i,
$$
whence the result by the induction hypothesis.

Using Lemma 1, the product in $\mathbf{T}(M)^{*gr}$ of $n$ linear forms $x_1^*, x_2^*, \ldots, x_n^*$ of $M^*$ is given by

$$
\langle x_1^* x_2^* \ldots x_n^*, x_1 x_2 \ldots x_n \rangle = \prod_{i=1}^n \langle x_i^*, x_i \rangle
$$
for $x_i \in M$ ($1 \leq i \leq n$); the product of these $n$ forms in $\mathbf{S}(M)^{*gr}$ is given by

$$
\langle x_1^* x_2^* \ldots x_n^*, x_1 x_2 \ldots x_n \rangle = \sum_{\sigma \in \mathfrak{S}_n} \left( \prod_{i=1}^n \langle x_{\sigma(i)}^*, x_i \rangle \right);
$$

finally, the product of these forms in $\bigwedge(M)^{*gr}$ is given by
$$
\langle x_1^* x_1^* \ldots x_n^*, x_1 x_2 \ldots x_n \rangle = \det(\langle x_i^*, x_j \rangle).
$$
In each of the three cases, we have respectively
$$
\theta_T(x_1^* \otimes x_2^* \otimes \ldots \otimes x_n^*) = x_1^* x_2^* \ldots x_n^*
$$
$$
\theta_S(x_1^* x_2^* \ldots x_n^*) = x_1^* x_2^* \ldots x_n^*
$$
$$
\theta_\Lambda(x_1^* \wedge x_2^* \wedge \cdots \wedge x_n^*) = x_n^* x_{n-1}^* \ldots x_1^* = (-1)^{n(n-1)/2} x_1^* x_2^* \ldots x_n^*
$$
and hence we deduce from (28), (29) and (30) the relations
$$(28\ \mathrm{bis})\quad \langle \theta_T(x_1^* \otimes x_2^* \otimes \cdots \otimes x_n^*), x_1 \otimes x_2 \otimes \cdots \otimes x_n \rangle = \prod_{i=1}^n \langle x_i^*, x_i \rangle$$
(in other words $\theta_T$ restricted to $T^2(M^*)$ is just the canonical homomorphism of II, § 4, no. 4)
$$(29\ \mathrm{bis})\quad \langle \theta_S(x_1^* x_2^* \ldots x_n^*), x_1 x_2 \ldots x_n \rangle = \sum_{\sigma \in S_n} \left( \prod_{i=1}^n \langle x_{\sigma(i)}^*, x_i \rangle \right)$$
$$(30\ \mathrm{bis})\quad \langle \theta_\Lambda(x_1^* \wedge x_2^* \wedge \cdots \wedge x_n^*), x_1 \wedge x_2 \wedge \cdots \wedge x_n \rangle$$
$$
= (-1)^{n(n-1)/2} \det(\langle x_i^*, x_j \rangle).
$$

#### Proposition 7 {#alg-iii-s11-prop-7 .statement}

*Let M be a finitely generated projective A-module. Then the canonical homomorphisms $\theta_T : T(M^*) \to T(M)^{*gr}$ and $\theta_\Lambda : \bigwedge(M^*) \to (\bigwedge(M)^{*gr})^0$ are bijective. Also the graded dual $\bigwedge(M)^{*gr}$ is then equal to the dual $\bigwedge(M)^*$ of the A-module $\bigwedge(M)$.*

Suppose first that M has a *finite basis* $(e_i)_{1 \leq i \leq m}$ and let $(e_i^*)_{1 \leq i \leq m}$ be the dual basis of $M^*$ (II, § 10, no. 4). Formula (28 bis) shows that, for every finite sequence $s = (j_k)_{1 \leq k \leq n}$ of n elements of the interval $[1, m]$ of $\mathbf{N}$,
$$
\theta_T(e_{j_1}^* \otimes \cdots \otimes e_{j_n}^*)
$$
is the element of index s in the basis of $(T^n(M))^*$, *dual* to the basis of $T^n(M)$ consisting of the $e_s = e_{j_1} \otimes \cdots \otimes e_{j_n}$ (\S 5, no. 5, Theorem 1). Hence $\theta_T$ is bijective.

Similarly, formula (30 bis) shows that, for every finite subset H of $[1, m]$ with n elements, $(-1)^{n(n-1)/2} \theta_\Lambda(e_H^*)$ (notation of § 7, no. 8, Theorem 1) is the element of index H in the basis of $(\bigwedge^n(M))^*$, *dual* to the basis of $\bigwedge^n(M)$ consisting of the $e_H$. Hence $\theta_\Lambda$ is bijective.

Suppose now only that M is finitely generated and projective; then M is a direct factor of a finitely generated free A-module L, so that there exist two

A-linear mappings $M \xrightarrow{j} L \xrightarrow{p} M$ whose composition is the identity $l_M$. We deduce a commutative diagram

$$
\begin{array}{ccc}
T(M^*) & \xrightarrow{T(tj)} & T(L^*) \\
\theta_T \downarrow & & \theta_T \downarrow \\
T(M)^{*gr} & \xrightarrow{tT(j)} & T(L)^{*gr}
\end{array}
$$
$$
\begin{array}{ccc}
T(L^*) & \xrightarrow{T(tp)} & T(M^*) \\
\theta_T \downarrow & & \theta_T \downarrow \\
T(L)^{*gr} & \xrightarrow{tT(p)} & T(M)^{*gr}
\end{array}
$$

and an analogous commutative diagram where $T$ is replaced by $\Lambda$. The proposition then follows from the following lemma:

#### Lemma 2 {#alg-iii-s11-lem-2 .statement}

*Let*

$$
\begin{array}{ccc}
X & \xrightarrow{u} & Y & \xrightarrow{v} & X \\
f \downarrow & & g \downarrow & & f \downarrow \\
X' & \xrightarrow{u'} & Y' & \xrightarrow{v'} & X'
\end{array}
$$

*be a commutative diagram of sets and mappings such that $v \circ u$ and $v' \circ u'$ are the identity mappings of $X$ and $X'$ respectively. Then, if $g$ is injective (resp. surjective, resp. bijective), so is $f$.*

$u$ is injective since $v \circ u$ is, hence, if $g$ is injective, $u' \circ f = g \circ u$ is injective and therefore $f$ is injective. Similarly $v'$ is surjective since $v' \circ u'$ is; hence, if $g$ is surjective, $f \circ v = v' \circ g$ is surjective and therefore $f$ is surjective.

The last assertion of Proposition 7 follows from the fact that $\Lambda(M)$ is then a finitely generated A-module (\S 7, no. 3, Proposition 6 and II, \S 11, no. 6, Remark).

We now examine what can be said concerning the homomorphism $\theta_S$ when $M$ is *projective and finitely generated*. Suppose first that $M$ admits a finite basis $(e_i)_{1 \leq i \leq m}$. In the notation at the beginning of the chapter the A-module $S^n(M)$ admits as basis the family of elements $e^\alpha$ such that $|\alpha| = n$. Let $u_\alpha$ (for $|\alpha| = n$) denote the element of index $\alpha$ in the basis of $(S^n(M))^*$ *dual* to $(e^\alpha)$. The elements $u_\alpha$, for $\alpha \in \mathbf{N}^m$, therefore form a basis of the algebra $S(M)^{*gr}$ and we shall obtain the multiplication table of this basis explicitly. We write

$$
u_\alpha u_\beta = \sum_{\gamma \in \mathbf{N}^m} a_{\alpha \beta \gamma} u_\gamma \quad \text{with } a_{\alpha \beta \gamma} \in A.
$$

Then by definition

$$
a_{\alpha \beta \gamma} = \langle u_\alpha u_\beta, e^\gamma \rangle = m((u_\alpha \otimes u_\beta)(c(e^\gamma))),
$$

where $m : A \otimes A \to A$ defines the multiplication on $A$ and $c$ is the coproduct of $S(M)$. In other words, $a_{\alpha \beta \gamma}$ is just the coefficient of $e^\alpha \otimes e^\beta$ when $c(e^\gamma)$ is written in terms of the basis of $S(M) \otimes S(M)$ consisting of the $e^\xi \otimes e^\eta$, where $\xi$ and $\eta$ run through $\mathbf{N}^m$. But since $c$ is an algebra homomorphism,

$$
c(e^\gamma) = \prod_{i=1}^m (c(e_i))^{r_i} = \prod_{i=1}^m (e_i \otimes 1 + 1 \otimes e_i)^{r_i}
$$

by formula (4) of no. 1; this gives

(31)
$$
c(e^\gamma) = \sum_{\xi + \eta = \gamma} (\xi, \eta) e^\xi \otimes e^\eta
$$
where we write

(32)
$$
((\xi, \eta)) = \prod_{i=1}^n \frac{(\xi_i + \eta_i)!}{\xi_i! \eta_i!} \quad \text{(cf. § 10, no. 4, formula (18))}.
$$
Hence we obtain the multiplication table

(33)
$$
u_\alpha u_\beta = ((\alpha, \beta)) u_{\alpha + \beta}.
$$
On the other hand, if $(e_i^*)_{1 \leq i \leq m}$ is the basis of $M^*$, dual to $(e_i)$, it follows from formula (29 bis) that, for all $\alpha \in \mathbf{N}^m$,

(34)
$$
\theta_S(e^{*\alpha}) = \alpha! u_\alpha
$$
in the notation of § 6, no. 6. Hence the homomorphism $\theta_S$ is bijective if and only if the $\alpha! u_\alpha$ form a *basis* of $S(M)^{*gr}$, or also if the elements $\alpha! 1$ are *invertible*.

#### Proposition 8 {#alg-iii-s11-prop-8 .statement}

*Suppose that the ring $A$ is an algebra over the field $\mathbf{Q}$ of rational numbers; then, for every finitely generated projective $A$-module $M$, the homomorphism*

$$
\theta_S : S(M^*) \to S(M)^{*gr}
$$
*is bijective.*

It amounts to proving this when $M$ is finitely generated and free; we pass from this to the general case using Lemma 2 as in the proof of Proposition 7.

#### Remark {#alg-iii-s11-n5-rem-1 .statement}

Let $M$ be an $A$-module and $\rho : A \to B$ a commutative ring homomorphism. Then there is a commutative diagram of graded $B$-algebra homomorphisms

$$
\begin{array}{ccc}
T((M^*)_{(B)}) & \longrightarrow & (T(M)^{*gr})_{(B)} \\
\downarrow_{T(u_M)} & & \downarrow^{u_{T(M)}} \\
T((M_{(B)})^*) & \xrightarrow{\theta_T} & T(M_{(B)})^{*gr}
\end{array}
$$

where the first row is a homomorphism composed of the homomorphism $\theta_T \otimes 1_B : T(M^*) \otimes_A B \to T(M)^{*gr}$ and the canonical isomorphism

$$
T((M^*)_{(B)}) \to T(M^*) \otimes_A B
$$

§ 5, no. 3, Proposition 5). It is immediately verified, using formula (28) and the definition of the homomorphism $v_E$ (II, § 5, no. 4), that this diagram is *commutative*. When M is a *finitely generated projective* A-module, $M_{(B)}$ is a finitely generated projective B-module (II, § 5, no. 1, Corollary to Proposition 4) and all the homomorphisms of the above diagram are *bijective* (Proposition 7 and II, § 5, no. 4, Proposition 8). There are analogous commutative diagrams with T replaced by S or $\Lambda$; the diagram for $\Lambda$ also consists of bijective homomorphisms when M is projective and finitely generated (Proposition 7); if further A is an algebra over $\mathbf{Q}$, the diagram for S also consists of bijective homomorphisms (Proposition 8).

### 6. INNER PRODUCTS: CASE OF ALGEBRAS

Let $E = \bigoplus_{p \geq 0} E_p$ be a *graded A-algebra* of type $\mathbf{N}$ and P a graded A-module of type $\mathbf{Z}$; for every *homogeneous* element $x \in E_p$, *left* multiplication by x is an A-linear mapping $e(x)$ of E into itself which is *graded of degree p*. For every element $u \in \mathrm{Homgr}_A(E, P)$, the *right inner product of u by x*, denoted by $u \perp x$, is the element $u \circ e(x)$ of $\mathrm{Homgr}_A(E, P)$. We also write $(i(x))(u) = u \perp x$ and we see that $i(x)$ is a graded endomorphism of degree p of the graded A-module $\mathrm{Homgr}_A(E, P)$. If now $x = \sum_{p \geq 0} x_p$ is an arbitrary element of E (with $x_p \in E_p$ for all $p \geq 0$, $x_p = 0$ except for a finite number of values of $p$), we write $i(x) = \sum_{p=0}^\infty i(x_p)$, which is therefore an endomorphism of the A-module $\mathrm{Homgr}_A(E, P)$.

To remember which element, in the expression $u \perp x$, "operates" on the other, observe that the element x which "operates" on u is placed at the free end of the horizontal line in $\perp$.

The *associativity* of the algebra E goes over to the relation $e(xy) = e(x) \circ e(y)$ for $x, y$ homogeneous; whence, by definition of $i(x)$,

$$
i(xy) = i(y) \circ i(x)
$$

first for $x, y$ homogeneous and then, by linearity, for *arbitrary* $x, y$ in E; this may also be written

$$
(u \perp x) \perp y = u \perp (xy)
$$

for $x, y$ in E and $u \in \mathrm{Homgr}_A(E, P)$; as on the other hand clearly $i(1)$ is the identity mapping (since this follows from $e(1) = 1_E$) and $x \mapsto i(x)$ is *A-linear*, it is seen that the external law of composition $(x, u) \mapsto u \perp x$ ($x \in E, u \in \mathrm{Homgr}_A(E, P)$) defines, with addition, a *right E-module* structure on $\mathrm{Homgr}_A(E, P)$.

In particular we consider the case $P = A$, $\mathrm{Homgr}_A(E, P)$ being in this case the *graded dual* $E^{*gr}$ of $E$; $i(x)$ is then the *graded transpose* of the $A$-linear mapping $e(x)$ (II, § 11, no. 6), in other words, for all $x, y$ in $E$, $u \in E^{*gr}$,

$$
\langle u \sqcup x, y \rangle = \langle u, xy \rangle.
$$

With the convention at the beginning of the paragraph, note that, if $x \in E_p$, $i(x)$ is an endomorphism of $E^{*gr}$ *of degree* $-p$.

For every homogeneous element $x \in E_p$, *right* multiplication by $x$ is similarly denoted by $e'(x)$ and the element $u \circ e'(x)$ of $\mathrm{Homgr}_A(E, P)$, called the *left inner product of u by x*, by $x \sqcup u$; we write $i'(x) = x \sqcup u$ and $i'(x)$ is therefore a graded endomorphism of $\mathrm{Homgr}_A(E, P)$ of degree $p$; as above this definition can be extended to the case where $x$ is an arbitrary element of $E$. As in this case $e'(xy) = e'(y)e'(x)$,

$$
i'(xy) = i'(x) \circ i'(y)
$$

which may also be written

$$
x \sqcup (y \sqcup u) = (xy) \sqcup u
$$

and shows that the external law of composition $(x, u) \mapsto x \sqcup u$ defines, with addition, a *left E-module* structure on $\mathrm{Homgr}_A(E, P)$. The associativity of $E$ implies on the other hand that $e(x) \circ e'(y) = e'(y) \circ e(x)$ for $x, y$ homogeneous in $E$, whence the relation

$$
(y \sqcup u) \sqcup x = y \sqcup (u \sqcup x)
$$

so that the two external laws of composition on $\mathrm{Homgr}_A(E, P)$ define on this set an *(E, E)*-*bimodule* structure (II, § 1, no. 14).

When we take $P = A$, $i'(x)$ is the graded transpose of $e'(x)$; in other words, for all $x, y$ in $E$, $u \in E^{*gr}$,

$$
\langle y, x \sqcup u \rangle = \langle yx, u \rangle.
$$

When the graded algebra $E$ is *commutative*, obviously $u \sqcup x = x \sqcup u$. When $E$ is *anticommutative* and $P = A$, then for $x \in E_p$, $y \in E_r$ and $u \in E_q^*$, $yx = (-1)^{pr} xy$, whence, by (37) and (41), $\langle u \sqcup x, y \rangle = (-1)^{pr} \langle y, x \sqcup u \rangle$. But as the two sides of this relation are zero except for $r = q - p$,

$$
x \sqcup u = (-1)^{p(q-p)} u \sqcup x.
$$

Let $F$ be another graded $A$-algebra and $\phi : E \to F$ an $A$-homomorphism of graded algebras; then $\tilde{\phi} = \mathrm{Hom}(\phi, 1_P) : \mathrm{Homgr}_A(F, P) \to \mathrm{Homgr}_A(E, P)$ is a graded $A$-homomorphism of degree 0; by definition, for $x, y$ in $E$ and $u \in \mathrm{Homgr}_A(F, P)$

$$
\begin{align*}
(\tilde{\phi}(u \sqcup \phi(x)))(y) &= (u \sqcup \phi(x))(\phi(y)) \\
&= u(\phi(x)\phi(y)) = u(\phi(xy)) = (\tilde{\phi}(u))(xy) = (\tilde{\phi}(u) \sqcup x)(y)
\end{align*}
$$

or also

$$
\tilde{\phi}(u \sqcup \phi(x)) = \tilde{\phi}(u) \sqcup x
$$

and similarly

$$
\tilde{\phi}(\phi(x) \sqcup u) = x \sqcup \tilde{\phi}(u).
$$

In other words, when Homgr_A(F, P) is considered as an (E, E)-bimodule by means of the ring homomorphism $\phi : E \to F$, it is seen that $\tilde{\phi}$ is an (E, E)-bimodule homomorphism (or also an E-homomorphism of the (F, F)-bimodule Homgr_A(F, P) into the (E, E)-bimodule Homgr_A(E, P)).

#### Example {#alg-iii-s11-n6-exa-1 .statement}

In particular the above may be applied when E is one of the graded algebras T(M), S(M) or $\bigwedge(M)$ for an A-module M and P an A-module (with the trivial graduation). To find explicitly the bimodule structures thus obtained, note that the elements of degree $-n$ of Homgr_A(T(M), P) (resp. Homgr_A(S(M), P), resp. Homgr_A($\bigwedge(M)$, P)) are identified with the *n-linear mappings* (resp. *symmetric n-linear mappings*, resp. *alternating n-linear mappings*) of $M^n$ into P. It suffices to express the products

$$
f \sqcup (x_1 \otimes x_2 \otimes \cdots \otimes x_p)
$$

(resp. $f \sqcup (x_1 x_2 \ldots x_p)$), resp. $f \sqcup (x_1 \wedge x_2 \wedge \cdots \wedge x_p)$) for every finite sequence $(x_i)_{1 \leq i \leq p}$ of elements of M and the analogues for the left inner product. It follows immediately from the definitions that

$$
f \sqcup (x_1 \otimes x_2 \otimes \cdots \otimes x_p) = (x_1 \otimes x_2 \otimes \cdots \otimes x_p) \sqcup f = 0
$$

*if* $p > n$ and that, for $p \leq n$, $f \sqcup (x_1 \otimes x_2 \otimes \cdots \otimes x_p)$ (resp.

$$
(x_1 \otimes x_2 \otimes \cdots \otimes x_p) \sqcup f)
$$

is the *(n - p)*-linear mapping defined by

$$
\begin{cases}
(f \sqcup (x_1 \otimes x_2 \otimes \cdots \otimes x_p))(y_1, \ldots, y_{n-p}) \\
\hspace{10cm} = f(x_1, \ldots, x_p, y_1, \ldots, y_{n-p}) \\
((x_1 \otimes x_2 \otimes \cdots \otimes x_p) \sqcup f)(y_1, \ldots, y_{n-p}) \\
\hspace{10cm} = f(y_1, \ldots, y_{n-p}, x_1, \ldots, x_p).
\end{cases}
$$

For $p > n$, there are also in Homgr_A(S(M), P) (resp. Homgr_A($\bigwedge(M)$, P)) formulae (44) with $x_1 \otimes x_2 \otimes \cdots \otimes x_p$ replaced by $x_1 x_2 \ldots x_p$ (resp. $x_1 \wedge x_2 \wedge \cdots \wedge x_p$). For $p \leq n$, the same substitutions in (45) define the *symmetric* *(n - p)*-linear mappings $f \sqcup (x_1 x_2 \ldots x_p)$ and $(x_1 x_2 \ldots x_p) \sqcup f$ (resp. the *alternating* *(n - p)*-linear mappings

$$
f \sqcup (x_1 \wedge x_2 \wedge \cdots \wedge x_p) \quad \text{and} \quad (x_1 \wedge x_2 \wedge \cdots \wedge x_p) \sqcup f).
$$

When $n = p$, the above products are equal to the constant function on $M$ equal to $f(x_1, \ldots, x_p)$.

If $u : M \to N$ is an $A$-module homomorphism, $T(u) : T(M) \to T(N)$ is a graded $A$-algebra homomorphism, then it follows from what we have seen above that $(T(u))^\sim$ is a $T(M)$-homomorphism of the $(T(N), T(N))$-bimodule $\mathrm{Homgr}_A(T(N), P)$ into the $(T(M), T(M))$-bimodule $\mathrm{Homgr}_A(T(M), P)$, relative to the ring homomorphism $T(u)$. There are analogous results for $(S(u))^\sim$ and $(\wedge(u))^\sim$.

### 7. INNER PRODUCTS: CASE OF COGEbras

Let $E = \bigoplus_{p \geq 0} E_p$ be a coassociative counital graded cogebra. Then we know (no. 2, Propositions 1 and 3) that the graded dual $E^{*\mathrm{gr}}$ has (with the convention on graduations made at the beginning of the paragraph) a graded algebra structure of type $\mathbf{N}$ over $A$, the product of two elements $u, v$ of this algebra being defined by $uv = m \circ (u \otimes v) \circ c$, where $c : E \to E \otimes_A E$ is the coproduct and $m : A \otimes_A A \to A$ defines the multiplication. In other words, if, for $x \in E$, $c(x) = \sum_i y_i \otimes z_i$, we can write (canonically identifying $A \otimes_A E$ and $E$)

$$
\langle x, uv \rangle = (uv)(x) = \sum_i u(y_i)v(z_i) = v\left( \sum_i u(y_i)z_i \right)
= v(((u \otimes 1_E) \circ c)(x)) = \langle ((u \otimes 1_E) \circ c)(x), v \rangle.
$$

This can be interpreted by saying that, for all $u$ homogeneous of degree $p$ in $E^{*\mathrm{gr}}$, the left multiplication $e(u) : v \mapsto uv$ in $E^{*\mathrm{gr}}$ is the graded transpose of the graded endomorphism of degree $-p$

$$(46)$$
$$
i(u) = (u \otimes 1_E) \circ c
$$
of $E$; hence, in the above notation,

$$
(i(u))(x) = \sum_i u(y_i)z_i.
$$

Formula (46) also defines an element $i(u) \in \mathrm{Endgr}_A(E)$ for every element $u \in E^{*\mathrm{gr}}$; for all $x \in E$ and all $u \in E^{*\mathrm{gr}}$, we write

$$(47)$$
$$
x \perp u = (i(u))(x)
$$
so that, for $u$ and $v$ in $E^{*\mathrm{gr}}$,

$$
\langle x, uv \rangle = \langle x \perp u, v \rangle.
$$

The element $x \perp u$ of $E$ is called the right inner product of $x$ by $u$.

Here again the element $u$ which "operates" on $x$ is placed at the free end of the horizontal line in $\underline{\phantom{x}}$.

For any two elements $u, v$ of $E^{*\mathrm{gr}}$,

$$
x \underline{\phantom{(uv)}} = (x \underline{\phantom{u}}) \underline{\phantom{v}},
$$

in other words

$$
i(uv) = i(v) \circ i(u).
$$

As above let $c(x) = \sum_i y_i \otimes z_i$, so that $x \underline{\phantom{(uv)}} = \sum_i (uv)(y_i)z_i$. If

$$
c(y_i) = \sum_j y_{ij}' \otimes y_{ij}'',
$$

then

$$
x \underline{\phantom{(uv)}} = \sum_{i,j} u(y_{ij}')v(y_{ij}'')z_i.
$$

On the other hand, if $c(z_i) = \sum_k z_{ik}' \otimes z_{ik}''$, then

$$
(x \underline{\phantom{u}}) \underline{\phantom{v}} = \sum_{i,k} u(y_i)v(z_{ik}')z_{ik}''.
$$

Now, the coassociativity of $E$ shows that (no. 2, Proposition 1)

$$
\sum_{i,j} y_{ij}' \otimes y_{ij}'' \otimes z_i = \sum_{i,k} y_i \otimes z_{ik}' \otimes z_{ik}''
$$

and the equality of expressions (49) and (50) follows from the fact that they are respectively the image of the left and right hand sides of (51) under the linear mapping $f$ from $E \otimes E \otimes E$ to $E$ such that $f(x \otimes y \otimes z) = u(x)v(y)z$.

We recall on the other hand (no. 2, Proposition 3) that the unit element of the algebra $E^{*\mathrm{gr}}$ is the linear form $e : x \mapsto \gamma(x).1$; hence

$$
x \underline{\phantom{e}} = \sum_i \gamma(y_i)z_i = x
$$

by virtue of the definition of counit. As the mapping $u \mapsto i(u)$ is linear, it is seen that the external law of composition $(u, x) \mapsto x \underline{\phantom{u}}$ defines a *right* $E^{*\mathrm{gr}}$-module structure on $E$.

Similarly we define, for all $u \in E^{*\mathrm{gr}}$, the endomorphism of $E$

$$
i'(u) = (1_E \otimes u) \circ c
$$

and, for all $x \in E$, we write

$$
(i'(u))(x) = u \underline{\phantom{x}}
$$

and this element of $E$ is called the *left inner product of x by u*. As above it is seen that the external law $(u, v) \mapsto u \sqcup x$ defines a *left $E^{*\mathrm{gr}}$-module structure* on $E$. Moreover, these two structures are *compatible*, in other words,

$$(54)$$
$$(u \sqcup x) \sqcap v = u \sqcup (x \sqcap v)$$

for $u, v$ in $E^{*\mathrm{gr}}$ (II, § 1, no. 14). With the same notation as above, the left hand side of (54) is $\sum_{i,j} u(z_i)v(y_{ij}')y_{ij}''$ and the right hand side is $\sum_{i,k} v(y_i)u(z_{ik}'')z_{ik}'$; their equality follows from the fact that they are the respective images of the left and right hand sides of (51) under the linear mapping $g$ of $E \otimes E \otimes E$ into $E$ such that $g(x \otimes y \otimes z) = v(x)u(z)y$.

It is therefore seen that the two external laws of composition on $E$ defines on this set an $(E^{*\mathrm{gr}}, E^{*\mathrm{gr}})$*-bimodule* structure.

When the cogebra $E$ is *cocommutative*, then $u \sqcup x = x \sqcap u$ for all $x \in E$ and $u \in E^{*\mathrm{gr}}$; when it is *anticocommutative* (\S 4, no. 9) and $u \in E_p^*$ and $x \in E_q$, we can write $c(x) = \sum_{0 \leq j \leq q} \left( \sum_i y_{ij} \otimes z_{i, q-j} \right)$ with $y_{ij}$ and $z_{ij}$ in $E_j$ for all $j$ and then by hypothesis

$$\sum_i z_{ij} \otimes y_{i, q-j} = (-1)^{j(q-j)} \sum_i y_{ij} \otimes z_{i, q-j}.$$

By definition, $x \sqcap u = \sum_{0 \leq j \leq q} \left( \sum_i u(y_{ij})z_{i, q-j} \right)$ and

$$u \sqcup x = \sum_{0 \leq j \leq q} \left( \sum_i u(z_{i, q-j})y_{ij} \right).$$

As $u(y_{ij}) = 0$ (resp. $u(z_{i, q-j}) = 0$ unless $j = p$ (resp. $q - j = p$), it is seen by the above that $u \sqcup x = (-1)^{p(q-p)} x \sqcap u$.

Finally, let $\phi : E \to F$ be a *graded cogebra morphism*; then it has been seen (no. 2) that the graded transpose $t\phi : F^{*\mathrm{gr}} \to E^{*\mathrm{gr}}$ is a *graded algebra homomorphism*; therefore, for $x \in E$, $u, v$ in $F^{*\mathrm{gr}}$,

$$
\langle \phi(x \sqcap t\phi(u)), v \rangle = \langle x \sqcap t\phi(u), t\phi(v) \rangle = \langle x, t\phi(u)t\phi(v) \rangle = \langle x, t\phi(uv) \rangle
$$
$$
= \langle \phi(x), uv \rangle = \langle \phi(x) \sqcap u, v \rangle
$$

whence

$$(55)$$
$$\phi(x) \sqcap u = \phi(x \sqcap t\phi(u));$$

and similarly

$$(56)$$
$$u \sqcup \phi(x) = \phi(t\phi(u) \sqcup x).$$

In other words, $\phi$ is an $F^{*\mathrm{gr}}$*-homomorphism* of the $(E^{*\mathrm{gr}}, E^{*\mathrm{gr}})$*-bimodule* $E$ into the $(F^{*\mathrm{gr}}, F^{*\mathrm{gr}})$*-bimodule* $F$, relative to the ring homomorphism

$$
t\phi : F^{*\mathrm{gr}} \to E^{*\mathrm{gr}}.
$$

#### Example {#alg-iii-s11-n7-exa-1 .statement}

In particular the above can be applied when E is one of the graded cogebras T(M), S(M) or $\Lambda(M)$ for an A-module M (no. 1, Examples 5, 6 and 7). To find explicitly the bimodule structures thus obtained, we again identify a homogeneous element f of degree n in $T(M)^{*gr}$ (resp. $S(M)^{*gr}$, resp. $\Lambda(M)^{*gr}$) with an *n-linear form* (resp. *symmetric n-linear form*, resp. *alternating n-linear form*, also called an *n-form*) on $M^n$. It suffices to express the products

$$
(x_1 \otimes x_2 \otimes \cdots \otimes x_p) \triangleleft f \text{ (resp. } (x_1 x_2 \ldots x_p) \triangleleft f,
$$

resp. $(x_1 \wedge x_2 \wedge \cdots \wedge x_p) \triangleleft f$ for every finite sequence $(x_i)_{1 \leq i \leq p}$ of elements of M and the analogues for the left inner product. Now, definitions (46) and (52) and formulae (3), (6) and (9) of no. 1 give respectively:

$$
\begin{cases}
(x_1 \otimes x_2 \otimes \cdots \otimes x_p) \triangleleft f = f \triangleright (x_1 \otimes x_2 \otimes \cdots \otimes x_p) = 0 \\
(x_1 x_2 \ldots x_p) \triangleleft f = f \triangleright (x_1 x_2 \ldots x_p) = 0 \quad \text{for } p < n. \\
(x_1 \wedge x_2 \wedge \cdots \wedge x_p) \triangleleft f = f \triangleright (x_1 \wedge x_2 \wedge \cdots \wedge x_p) = 0
\end{cases}
$$

For $p \geq n$, we have respectively

(58) $(x_1 \otimes x_2 \otimes \cdots \otimes x_p) \triangleleft f = f(x_1, \ldots, x_n)x_{n+1} \otimes \cdots \otimes x_p$

(59) $(x_1 x_2 \ldots x_p) \triangleleft f = \sum_{\sigma} f(x_{\sigma(1)}, \ldots, x_{\sigma(n)})x_{\sigma(n+1)} \cdots x_{\sigma(p)}$

(60) $(x_1 \wedge x_2 \wedge \cdots \wedge x_p) \triangleleft f = \sum_{\sigma} \varepsilon_{\sigma} f(x_{\sigma(1)}, \ldots, x_{\sigma(n)})x_{\sigma(n+1)} \wedge \cdots \wedge x_{\sigma(p)}$

(where, in (59) and (60), the summations are taken over the permutations $\sigma \in \mathfrak{S}_p$ which are *increasing on each of the intervals* $[1, n]$ and $[n+1, p]$ of $\mathbf{N}$; and similarly

(61) $f \triangleright (x_1 \otimes x_2 \otimes \cdots \otimes x_p) = f(x_{p-n+1}, \ldots, x_p)x_1 \otimes x_2 \otimes \cdots \otimes x_{p-n}$

(62) $f \triangleright (x_1 x_2 \ldots x_p) = \sum_{\sigma} f(x_{\sigma(p-n+1)}, \ldots, x_{\sigma(p)})x_{\sigma(1)} \cdots x_{\sigma(p-n)}$

(63) $f \triangleright (x_1 \wedge x_2 \wedge \cdots \wedge x_p) = \sum_{\sigma} \varepsilon_{\sigma} f(x_{\sigma(p-n+1)}, \ldots, x_{\sigma(p)})x_{\sigma(1)} \wedge \cdots \wedge x_{\sigma(p-n)}$

(where, in (62) and (63), the summations are taken over the permutations $\sigma \in \mathfrak{S}_p$ which are *increasing on each of the intervals* $[1, p-n]$ and $[p-n+1, p]$ of $\mathbf{N}$).

### 8. INNER PRODUCTS: CASE OF BIGEBRAS

Let E be a graded bigebra (resp. skew graded bigebra) (no. 4, Definition 3); then the results of nos. 6 and 7 can be applied to define the right (resp. left) inner products $x \triangleleft u \in E$ and $u \triangleleft x \in E^{*gr}$ (resp. $u \triangleright x \in E$ and $x \triangleright u \in E^{*gr}$) for all $x \in E$ and all $u \in E^{*\mathrm{gr}}$. Thus an $(E, E)$-bimodule structure and an $(E^{*\mathrm{gr}}, E^{*\mathrm{gr}})$-bimodule structure are obtained on $E$. Further:

#### Proposition 9 {#alg-iii-s11-prop-9 .statement}

*Let $E$ be a graded bigebra (resp. skew graded bigebra). For every element $x$ of degree 1 in $E$, the left and right inner products by $x$ are derivations (resp. antiderivations) ($\S 10$, no. 2) of the algebra $E^{*\mathrm{gr}}$.*

In the notation of no. 6, for every homogeneous element $x$ of *degree* 1 in a graded bigebra (resp. a skew graded bigebra) $E$,
$$
c(x) = x \otimes 1 + 1 \otimes x,
$$
by Proposition 5 of no. 3 and the fact that $c$ is a homomorphism of degree 0. Suppose first that $E$ is a graded bigebra. For all $y \in E$, by definition
$$
\langle (uv) \mathbin{\&} x, y \rangle = \langle uv, xy \rangle = m((u \otimes v)(c(xy)))
$$
and since $c$ is an *algebra* homomorphism, $c(xy) = c(x)c(y)$. Let $c(y) = \sum_i s_i \otimes t_i$ with $s_i$ and $t_i$ in $E$; therefore
$$
c(xy) = \sum_i (xs_i) \otimes t_i + \sum_i s_i \otimes (xt_i).
$$
Hence $\langle (uv) \mathbin{\&} x, y \rangle = \sum_i u(xs_i)v(t_i) + \sum_i u(s_i)v(xt_i)$. But we may write
$$
\sum_i u(xs_i)v(t_i) = m(((u \mathbin{\&} x) \otimes v)(c(y))) = \langle (u \mathbin{\&} x)v, y \rangle
$$
and similarly
$$
\sum_i u(s_i)v(xt_i) = m((u \otimes (v \mathbin{\&} x))(c(y))) = \langle u(v \mathbin{\&} x), y \rangle,
$$
whence, returning to the notation $i(x)$ for the inner product.
$$(64)$$
$$(i(x))(uv) = ((i(x))(u))v + u((i(x))(v))$$
which proves that $i(x)$ is a *derivation* in $E^{*\mathrm{gr}}$.

Suppose now that $E$ is a *skew* graded bigebra, that $u \in E_p^*$, $v \in E_q^*$ and $y \in E_r$; then we can write
$$
c(y) = \sum_{0 \leq j \leq r} \left( \sum_i s_{ij} \otimes t_{i,r-j} \right)
$$
where the $s_{ij}$ and $t_{ij}$ belong to $E_j$; by definition of the product in $E^g \otimes_A E$, then
$$
c(xy) = c(x)c(y) = \sum_{0 \leq j \leq r} \left( \sum_i (xs_{ij}) \otimes t_{i,r-j} + (-1)^j \sum_i s_{ij} \otimes (xt_{i,r-j}) \right)
$$
whence this time
$$
\langle (uv) \mathbin{\&} x, y \rangle = \sum_{0 \leq j \leq r} \left( \sum_i u(xs_{ij})v(t_{i,r-j}) + (-1)^j \sum_i u(s_{ij})v(xt_{i,r-j}) \right).
$$

Then also $\sum_{0 \leq j \leq r} \left( \sum_i u(x s_{ij}) v(t_{i,r-j}) \right) = \langle (u \sqcup x)v, y \rangle$. On the other hand, $u(s_{ij}) = 0$ unless $j = -p$ and hence we may also write
$$
\sum_{0 \leq j \leq r} (-1)^j \left( \sum_i u(s_{ij}) v(x t_{i,r-j}) \right) = (-1)^p \langle u(v \sqcup x), y \rangle.
$$
We therefore conclude that
$$
(i(x))(uv) = ((i(x))(u))v + (-1)^p u((i(x))(v)),
$$
in other words $i(x)$ is an *antiderivation* in $E^{*gr}$. The assertions relating to the left inner product by an element $x$ of degree 1 in $E$ are proved similarly.

#### Remark {#alg-iii-s11-n8-rem-1 .statement}

(1) Let $E$ be a graded bigebra over $A$ and $N, N', N''$ three graded $A$-modules. Let $m$ be an $A$-bilinear mapping of $N \times N'$ into $N''$; for $u \in \mathrm{Homgr}_A(E, N)$ and $v \in \mathrm{Homgr}_A(E, N')$, let $u.v$ denote the graded homomorphism $m \circ (u \otimes v) \circ c$ of $E$ into $N''$. On the other hand, let $i(x)$ denote the (right or left) inner product by $x \in E$ in the $A$-modules $\mathrm{Homgr}_A(E, N)$, $\mathrm{Homgr}_A(E, N')$ and $\mathrm{Homgr}_A(E, N'')$. Then, if $x$ is *of degree* 1,
$$
(i(x))(u.v) = ((i(x))(u)).v + u.((i(x))(v))
$$
for all $u \in \mathrm{Homgr}_A(E, N)$ and $v \in \mathrm{Homgr}_A(E, N')$.

Under the same conditions, if $E$ is a skew graded bigebra and $u$ is homogeneous of degree $p$, then
$$
(i(x))(u.v) = ((i(x))(u)).v + (-1)^p u.((i(x))(v)).
$$
The proofs are the same as in Proposition 9.

(2) The same argument as in the above proof proves, more generally, that for all $x \in E$, if $c(x) = \sum_j x'_j \otimes x''_j$, then, for all $u, v$ in $E^{*gr}$, the "Leibniz formula"
$$
(i(x))(uv) = \sum_j (i(x'_j))(u).(i(x''_j))(v)
$$
holds. In particular, for every *primitive* element of a graded bigebra $E$, that is such that $c(x) = x \otimes 1 + 1 \otimes x$, $i(x)$ is a *derivation* of $E^{*gr}$.

#### Proposition 10 {#alg-iii-s11-prop-10 .statement}

*Let $E$ be a graded bigebra (resp. skew graded bigebra). For every element $f$ of degree 1 in $E^{*gr}$, the left and right inner products are derivations (resp. antiderivations) of the algebra $E$.*

Let $x \in E_p, y \in E_q$ ($p \geq 1, q \geq 1$). By Proposition 5 of no. 3, we can write
$$
c(x) = x \otimes 1 + \sum_{1 \leq j \leq p-1} \left( \sum_i x'_{ij} \otimes x''_{ij,p-j} \right) + 1 \otimes x
$$
$$
c(y) = y \otimes 1 + \sum_{1 \leq k \leq q-1} \left( \sum_i y'_{i,k} \otimes y''_{i,q-k} \right) + 1 \otimes y
$$

where $x'_{ij}$ and $x''_{ij}$ belong to $E_j$, $y'_{ik}$ and $y''_{ik}$ to $E_k$. If $E$ is a graded bigebra, the component of $c(xy) = c(x)c(y)$ belonging to $E_1 \otimes E$, is equal to
$$
\sum_i x'_{i,1} \otimes x''_{i,p-1}y + \sum_i y'_{i,1} \otimes xy''_{i,q-1}
$$
and hence by definition
$$
(xy) \leftarrow f = \sum_i f(x'_{i,1})x''_{i,p-1}y + \sum_i f(y'_{i,1})xy''_{i,q-1}
$$
$$
= (x \leftarrow f)y + x(y \leftarrow f)
$$
and the right inner product by $f$ is a *derivation*. If on the other hand $E$ is a skew graded bigebra, the component of $c(xy)$ belonging to $E_1 \otimes E$ is equal to
$$
\sum_i x'_{i,1} \otimes x''_{i,p-1}y + (-1)^p \sum_i y'_{i,1} \otimes xy''_{i,q-1}
$$
and this time we obtain
$$
(xy) \leftarrow f = (x \leftarrow f)y + (-1)^p x(y \leftarrow f)
$$
which shows that $i(f)$ is then an *antiderivation*. The argument is similar for the left inner product by $f$.

#### Example {#alg-iii-s11-n8-exa-1 .statement}

Propositions 9 and 10 apply in particular to the graded bigebra $S(M)$ and the skew graded bigebra $\Lambda(M)$. The inner products by elements of degree 1 in $S(M)$ (resp. $S(M)^{*gr}$) are *derivations* which *commute with one another*, since $S(M)$ (resp. $S(M)^{*gr}$) is commutative.

Similarly, the inner products by elements of degree 1 in $\Lambda(M)$ (resp. $\Lambda(M)^{*gr}$) are *antiderivations*, which are of *zero square*, for the square of an element of degree 1 in the algebra $\Lambda(M)$ (resp. $\Lambda(M)^{*gr}$) is zero.

### 9. INNER PRODUCTS BETWEEN $T(M)$ AND $T(M^*)$, $S(M)$ AND $S(M^*)$, $\Lambda(M)$ AND $\Lambda(M^*)$

The right inner product defines on $T(M)$ (resp. $S(M)$, resp. $\Lambda(M)$) a right module structure over the algebra $T(M)^{*gr}$ (resp. $S(M)^{*gr}$, resp. $\Lambda(M)^{*gr}$) (no. 7, *Examples*). Using the canonical homomorphisms $\theta_T$ (resp. $\theta_S$, resp. $\theta_\Lambda$) of no. 5, we derive
a right $T(M^*)$-module structure on $T(M)$
a right $S(M^*)$-module structure on $S(M)$
a left $\Lambda(M^*)$-module structure on $\Lambda(M)$.

The external law of any of these structures is also denoted by
$$
(z^*, t) \mapsto i(z^*) \cdot t
$$

(by an abuse of language); we also write $t \prec z^*$ instead of $i(z^*) . t$ in the case of $T(M)$ or $S(M)$; on the other hand, we write $z^* \prec t$ in the case of $\Lambda(M)$ and say that this is a *left* inner product of $t$ by $z^*$, since then we have a *left* $\Lambda(M^*)$-module law. For $z^*$ homogeneous of degree $n$ and $t$ homogeneous of degree $p$, $i(z^*) . t = 0$ if $p < n$ and, for $x_i \in M$ ($1 \leq i \leq p$), $x_j^* \in M^*$ ($1 \leq j \leq n$) and $p \geq n$, by virtue of formulae (58), (59) and (60) of no. 7,

$$
(66)\quad i(x_1^* \otimes x_2^* \otimes \cdots \otimes x_n^*) . (x_1 \otimes x_2 \otimes \cdots \otimes x_p)
$$
$$
= \left( \prod_{j=1}^n \langle x_j^*, x_j \rangle \right) x_{n+1} \otimes \cdots \otimes x_p
$$

$$
(67)\quad i(x_1^* x_2^* \ldots x_n^*) . (x_1 x_2 \ldots x_p) = \sum_\sigma \left( \prod_{j=1}^n \langle x_j^*, x_{\sigma(j)} \rangle \right) x_{\sigma(n+1)} \cdots x_{\sigma(p)}
$$

$$
(68)\quad i(x_1^* \wedge x_2^* \wedge \cdots \wedge x_n^*) . (x_1 \wedge x_2 \wedge \cdots \wedge x_p)
$$
$$
= (-1)^{n(n-1)/2} \sum_\sigma \varepsilon_\sigma \left( \prod_{j=1}^n \langle x_j^*, x_{\sigma(j)} \rangle \right) x_{\sigma(n+1)} \wedge \cdots \wedge x_{\sigma(p)}
$$

where, the formulae (67) and (68), $\sigma$ runs through the set of permutations $\sigma \in \mathfrak{S}_p$ which are *increasing* on the intervals $\{1, n\}$ and $\{n + 1, p\}$.

We can also write, in the inner product notation,

$$
\langle t \prec u^*, v^* \rangle = \langle t, \theta_T(u^* v^*) \rangle \quad \text{for } t \in T(M), u^*, v^* \text{ in } T(M^*)
$$
$$
\langle t \prec u^*, v^* \rangle = \langle t, \theta_S(u^* v^*) \rangle \quad \text{for } t \in S(M), u^*, v^* \text{ in } S(M^*)
$$
$$
\langle v^*, u^* \prec t \rangle = \langle \theta_\Lambda(u^* \wedge v^*), t \rangle \text{ for } t \in \Lambda(M), u^*, v^* \text{ in } \Lambda(M^*).
$$

We leave to the reader the task of finding explicitly the analogous formulae for left inner products, this time using formulae (61), (62) and (63).

The above can be applied with $M$ replaced by its dual $M^*$; $M^*$ must then be replaced by the bidual $M^{**}$ and $T(M^*)$, for example, thus has a right module structure over the algebra $T(M^{**})$. But the canonical mapping $c_M : M \to M^{**}$ defines an algebra homomorphism $T(c_M) : T(M) \to T(M^{**})$, by means of which $T(M^*)$ has a *right* $T(M)$-*module* structure. Similarly $S(M^*)$ (resp. $\Lambda(M^*)$) has a *right* $S(M)$-*module* (resp. *left* $\Lambda(M)$-*module*) structure. The explicit formulae giving the external laws of these modules are derived immediately from the above by exchanging the roles of $M$ and $M^*$. Note that, for all $x \in M$, $i(x)$ is always a *derivation* (resp. *antiderivation of zero square*) of the graded algebra $S(M^*)$ (resp. $\Lambda(M^*)$).

#### Proposition 11 {#alg-iii-s11-prop-11 .statement}

*The canonical homomorphism* $\theta_T : T(M^*) \to T(M)^{*gr}$ (resp. $\theta_S : S(M) \to S(M)^{*gr}$, resp. $\theta_\Lambda : \Lambda(M^*) \to \Lambda(M)^{*gr}$) *is a right* $T(M)$-*module* (resp. *right* $S(M)$-*module*, resp. *left* $\Lambda(M)$-*module*) *homomorphism.*

We show first that, for $z^* \in T(M^*)$ and $t \in T(M)$,

$$
\theta_T(z^* \wedge t) = \theta_T(z^*) \wedge t.
$$

Since $M$ is a generating system of the algebra $T(M)$, we need only prove (69) when $t = x \in M$; moreover we can restrict our attention to the case where $z^* = x_1^* \otimes x_2^* \otimes \cdots \otimes x_p^*$, where the $x_j^* \in M^*$, and then, by (66) with the roles of $M$ and $M^*$ interchanged, $z^* \wedge x = \langle x, x_1^* \rangle x_2^* \otimes \cdots \otimes x_p^*$. Therefore, for all $y_2, \ldots, y_p$ in $M$,

$$
\begin{align*}
\langle \theta_T(z^* \wedge x), y_2 \otimes y_3 \otimes \cdots \otimes y_p \rangle &= \langle x, x_1^* \rangle \prod_{j=2}^p \langle y_j, x_j^* \rangle \\
&= \langle \theta_T(z^*), x \otimes y_2 \otimes \cdots \otimes y_p \rangle \\
&= \langle \theta_T(z^*) \wedge x, y_2 \otimes \cdots \otimes y_p \rangle
\end{align*}
$$

whence (69).

We prove secondly that for $z^* \in S(M^*)$ and $t \in S(M)$,

$$
\theta_S(z^* \wedge t) = \theta_S(z^*) \wedge t.
$$

As above, we can limit ourselves to the case $t = x \in M$. But further, here $i(x)$ is a derivation of $S(M^*)$ and a derivation of $S(M)^{*gr}$. Therefore (\S 10, no. 7, Corollary to Proposition 9) it suffices to verify (70) for $z^* = x^* \in M^*$, since $M^*$ is a generating system of $S(M^*)$; but this is trivial, the two sides then being equal to $\langle x^*, x \rangle$. A similar argument proves the relation

$$
\theta_\wedge(t \wedge z^*) = t \wedge \theta_\wedge(z^*)
$$

for $z^* \in \Lambda(M^*)$ and $t \in \Lambda(M)$: observe then that, for $x \in M$, $i(x)$ is an antiderivation in $\Lambda(M^*)$ as well as in $\Lambda(M)^{*gr}$ and use \S 10, no. 7, Corollary to Proposition 9. There is an analogous result for left inner products.

### 10. EXPLICIT FORM OF INNER PRODUCTS IN THE CASE OF A FINITELY GENERATED FREE MODULE

Let $M$ be a finitely generated free $A$-module, $(e_i)_{1 \leq i \leq n}$ a basis of $M$ and $(e_i^*)_{1 \leq i \leq n}$ the dual basis of $M^*$. For every finite sequence $s = (i_1, \ldots, i_p)$ of elements of $\{1, n\}$, let $e_s = e_{i_1} \otimes e_{i_2} \otimes \cdots \otimes e_{i_p}$ (resp. $e_s^* = e_{i_1}^* \otimes \cdots \otimes e_{i_p}^*$). We know (\S 5, no. 5, Theorem 1) that the $e_s$ form a basis of the $A$-module $T(M)$ and the $e_s^*$ a basis of the $A$-module $T(M^*)$. If $s, t$ are two finite sequences of elements of $\{1, n\}$, let $s.t$ denote the sequence obtained as follows: if $s = (i_1, \ldots, i_p)$ and $t = (j_1, \ldots, j_q)$, $s.t$ is the sequence $(i_1, \ldots, i_p, j_1, \ldots, j_q)$ with $p + q$ terms. Then $e_{s.t} = e_s \otimes e_t$. It then follows from (66) that

$$
\begin{cases}
e_s \wedge e_t^* = 0 & \text{if } s \text{ is not of the form } t.u \\
e_{t.u} \wedge e_t^* = e_u.
\end{cases}
$$

Similarly, the symmetric algebra $S(M)$ has as basis the set of monomials $e^\alpha$ with $\alpha \in \mathbf{N}^n$ (\S 6, no. 6, Theorem 1) and $S(M^*)$ the set of monomials $e^{*\alpha}$ with $\alpha \in \mathbf{N}^n$; recall (no. 5) that $u_\alpha$, for $|\alpha| = k$, denotes the element of the basis of $(S^k(M))^*$, dual to the basis $(e^\alpha)_{|\alpha|=k}$ of $S^k(M)$; the $u_\alpha$, for $\alpha \in \mathbf{N}^n$, therefore form a basis of $S(M)^{*gr}$. The definition of right inner product by $e^\beta$ in $S(M)^{*gr}$ as the transpose of multiplication by $e^\beta$ in $S(M)$ then shows that

$$
\begin{cases}
u_\alpha \perp e^\beta = 0 & \text{if } \alpha \not\geq \beta \\
u_\alpha \perp e^\beta = u_{\alpha-\beta} & \text{if } \alpha \geq \beta.
\end{cases}
$$

(73)

Similarly, since $S(M)$ is here canonically identified with the graded dual of $S(M)^{*gr}$, $i(u_\beta)$ is the graded transpose of multiplication by $u^\beta$ in $S(M)^{*gr}$ and hence from the multiplication table (33) (no. 5) of the basis $(u_\alpha)$ we deduce that

$$
\begin{cases}
e^\alpha \perp u_\beta = 0 & \text{if } \alpha \not\geq \beta \\
e^\alpha \perp u_\beta = (\beta, \alpha - \beta)e^{\alpha-\beta} & \text{if } \alpha \geq \beta.
\end{cases}
$$

(74)

As for the right inner product of an element of $S(M)$ by an element of $S(M^*)$, the definition of this product (no. 9) and formula (34) of no. 5 allow us to deduce from (74) the formulae

$$
\begin{cases}
e^\alpha \perp e^{*\beta} = 0 & \text{if } \alpha \not\geq \beta \\
e^\alpha \perp e^{*\beta} = \frac{\alpha!}{(\alpha-\beta)!} e^{\alpha-\beta} & \text{if } \alpha \geq \beta.
\end{cases}
$$

(75)

There are analogous formulae for the inner product of an element of $S(M^*)$ by an element of $S(M)$ interchanging the roles of $M$ and $M^*$ (since $M^{**}$ is here identified with $M$).

#### Remark {#alg-iii-s11-n10-rem-1 .statement}

Being given the basis $(e_i)_{1 \leq i \leq n}$ allows us to identify the algebra $S(M)$ with the polynomial algebra $A[X_1, \ldots, X_n]$ (\S 6, no. 6); formula (75) shows that the inner product by $e^{*\alpha}$ is just the differential operator $D^\alpha = D_1^{\alpha_1}D_2^{\alpha_2}\ldots D_n^{\alpha_n}$, where $D_i = \partial/\partial X_i$ for $1 \leq i \leq n$ (\S 10, no. 11, Example).

Consider finally the exterior algebra $\Lambda(M)$, which has as basis the set of elements $e_J$, where $J$ runs through the set of subsets of the interval $\{1, n\}$ of $\mathbf{N}$ (\S 7, no. 8, Theorem 1); similarly $\Lambda(M^*)$ has as basis the elements $e_J^*$. It follows from formula (68) of no. 9 that

$$
\begin{cases}
e_K^* \wedge e_J = 0 & \text{if } K \notin J \\
e_K^* \wedge e_J = (-1)^{p(p-1)/2} \rho_{K, J-K} e_{J-K} & \text{if } K \subset J \text{ and } p = \operatorname{Card}(K),
\end{cases}
$$

(76)

where $\rho_{K, J-K}$ is the number defined by formula (19) of \S 7, no. 8. There are analogous formulae with the roles of $M$ and $M^*$ interchanged.

### 11. ISOMORPHISMS BETWEEN $\wedge^p(M)$ AND $\wedge^{n-p}(M^*)$ FOR AN $n$-DIMENSIONAL FREE MODULE M

#### Proposition 12 {#alg-iii-s11-prop-12 .statement}

*Let M be a free A-module of dimension n; let $e \in \wedge^n(M)$ be an element forming a basis of $\wedge^n(M)$ and let $e^*$ be the element of $\wedge^n(M^*)$ such that $\{(-1)^{n(n-1)/2} \theta_{\wedge}(e^*)\}$ is the dual basis of $\{e\}$ in $(\wedge^n(M))^*$. Let $\phi : \wedge(M^*) \to \wedge(M)$ be the mapping $z \mapsto z \wedge e^*$ and $\phi' : \wedge(M^*) \to \wedge(M)$ the mapping $z^* \mapsto z^* \wedge e$. Let $\phi_p$ (resp. $\phi'_p$) be the restriction of $\phi$ (resp. $\phi'$) to $\wedge^p(M)$ (resp. $\wedge^p(M^*)$). Then:

(i) *The mapping $\phi$ is a left $\wedge(M)$-module isomorphism and the mapping $\phi'$ is a left $\wedge(M^*)$-module isomorphism; moreover the mappings $\phi$ and $\phi'$ are inverses of one another.*

(ii) *The mapping $\phi_p$ is an isomorphism of the A-module $\wedge^p(M)$ onto the A-module $\wedge^{n-p}(M^*)$ and the mapping $\phi'_p$ is an isomorphism of the A-module $\wedge^p(M^*)$ onto the A-module $\wedge^{n-p}(M)$.

(iii) *If we write $B(u, v^*) = \langle u, \theta_{\wedge}(v^*) \rangle$ for $u \in \wedge(M)$ and $v^* \in \wedge(M^*)$ then, for $u^* \in \wedge^p(M^*)$ and $v^* \in \wedge^{n-p}(M^*)$,

$$
B(\phi'_p(u^*), v^*) = (-1)^{p(n-p)} B(u^*, \phi'_{n-p}(v^*)).
$$

The fact that $\phi$ is $\wedge(M)$-linear and $\phi'$ is $\wedge(M^*)$-linear follows from the formulae $(u \wedge v) \wedge e^* = u \wedge (v \wedge e^*)$ and $(u^* \wedge v^*) \wedge e = u^* \wedge (v^* \wedge e)$ (no. 6, formula (37)), using the fact that $\theta_{\wedge}$ is an isomorphism of $\wedge(M^*)$ onto the opposite algebra to $\wedge(M)^*$. On the other hand there exists a basis $(e_i)_{1 \leq i \leq n}$ of M such that

$$
e = e_1 \wedge e_2 \wedge \cdots \wedge e_n \quad \text{and} \quad e^* = (-1)^{n(n-1)/2} e_1^* \wedge e_2^* \wedge \cdots \wedge e_n^*,
$$

where $(e_i^*)$ is the basis dual to $(e_i)$. We write $I = \{1, n\}$; it follows from (76) that, for every subset J of I with p elements,

$$
\begin{cases}
\phi(e_J) = (-1)^{n(n-1)/2 + p(p-1)/2} \rho_{J, I-J} e_I^* J \\
\phi'(e_J^*) = (-1)^{p(p-1)/2} \rho_{J, I-J} e_{I-J}.
\end{cases}
$$

This proves that $\phi$ and $\phi'$ are bijective; moreover $\rho_{J, I-J} \rho_{I-J, J} = (-1)^{p(n-p)}$ (\S 7, no. 8, formula (21)); as the number

$$
\frac{n(n-1)}{2} + \frac{p(p-1)}{2} + \frac{(n-p)(n-p-1)}{2} + p(n-p) = n(n-1)
$$

is even, it follows that $\phi$ and $\phi'$ are inverses of one another. Finally, to prove (77), it suffices to take $u^* = e_J^*$ and $v^* = e_{I-J}^*$; the verification also follows from the definition of $\theta_{\wedge}$, formulae (78) and the relation $\rho_{J, I-J} \rho_{I-J, J} = (-1)^{p(n-p)}$ (\S 7, no. 8, formula (21)). Note that, for $u^* \in \wedge^p(M^*)$ and $v^* \in \wedge^{n-p}(M^*)$,

B(\phi_p'(u^*), v^*) is, to within a sign, the coefficient of $u^* \wedge v^*$ with respect to the basis $\{e^*\}$ of $\Lambda^n(M^*)$.

#### Proposition 13 {#alg-iii-s11-prop-13 .statement}

*With the hypotheses and notation of Proposition 11, for every endomorphism g of the A-module M.*

$$(79)$$
$$(\det g)\phi = \Lambda^{(tg)} \circ \phi \circ \Lambda(g).$$

Clearly $\Lambda^{(tg)} = \theta_{\Lambda}^{-1} \circ (t\Lambda(g)) \circ \theta_{\Lambda}$; since $\Lambda(g)$ is an endomorphism of the algebra $\Lambda(M)$ and by definition, for all
$$z \in \Lambda(M), \quad \theta_{\Lambda}(\Lambda(g)(z) \perp e^*) = \theta_{\Lambda}(e^*) \perp \theta_{\Lambda}(\Lambda(g)(z)),$$
we deduce from formula (42) of no. 6 that
$$
((\theta_{\Lambda}^{-1} \circ (t\Lambda(g)) \circ \theta_{\Lambda}) \circ \phi \circ \Lambda(g))(z) = \theta_{\Lambda}^{-1}(t\Lambda(g)(\theta_{\Lambda}(e^*)) \perp z)
= z \perp (\Lambda^{(tg)}(e^*)) = (\det g)(z \perp e^*) = (\det g)\phi(z)
$$
taking account of § 8, no. 4, Proposition 8.

#### Corollary {#alg-iii-s11-n11-cor-1 .statement}

*For every automorphism g of E,*
$$(80)$$
$$\Lambda^{(tg^{-1})} = (\det g)^{-1}\phi \circ (\Lambda(g)) \circ \phi^{-1}.$$

### 12. APPLICATION TO THE SUBSPACE ASSOCIATED WITH A p-VECTOR

Let K be a field and E a vector space over K. Recall that with every $p$-vector $z \in \Lambda^p(E)$ is associated a finite-dimensional subspace $M_z$ of E, namely the smallest vector subspace M of E such that $z \in \Lambda^p(M)$ (§ 7, no. 2, Corollary to Proposition 4).

#### Proposition 14 {#alg-iii-s11-prop-14 .statement}

(i) *The orthogonal of $M_z$ in $E^*$ is the set of $x^* \in E^*$ such that $x^* \perp z = 0$.*

(ii) *The subspace $M_z$ associated with z is the image of $\Lambda^{p-1}(E^*)$ under the mapping $\lambda_z : u^* \mapsto u^* \perp z$ of $\Lambda^{p-1}(E^*)$ into E.*

Let N denote the image of $\lambda_z$. For $x^* \in E^*$ and $u^* \in \Lambda^{p-1}(E^*)$,
$$
\langle \theta_{\Lambda}(x^*), u^* \perp z \rangle = \langle \theta_{\Lambda}(u^* \wedge x^*), z \rangle = (-1)^{p-1} \langle \theta_{\Lambda}(x^* \wedge u^*), z \rangle \\
= (-1)^{p-1} \langle \theta_{\Lambda}(u^*), x^* \perp z \rangle.
$$
Therefore, for $x^*$ to be orthogonal to N, it is necessary and sufficient that $x^* \perp z$ be orthogonal to $\theta_{\Lambda}(\Lambda(E^*))$. Now, the latter condition is equivalent to saying that $x^* \perp z = 0$; for let $(e_{\lambda})_{\lambda \in L}$ be a basis of E; giving L a total ordering, it has been seen (§ 7, no. 8, Theorem 1) that the $e_J$, for J running through the set $\mathcal{F}(L)$ of finite subsets of L, form a basis of $\Lambda(E)$; it then follows from formula (30) of no. 5 that the elements $\theta_{\wedge}(e_J^*)$ are, to within a sign, the coordinate forms on $\wedge(E)$ relative to the basis $(e_J)$; whence our assertion.

The orthogonal of N therefore consists of the $x^* \in E^*$ such that $x^* \perp z = 0$ and the conclusion of (i) will therefore follow from (ii).

We show first that $N \subset M_z$. Let M be a vector subspace of E such that $z \in \wedge(M)$ and let $j : M \to E$ be the canonical injection; let $\mu_z$ denote the mapping $v^* \mapsto v^* \perp z$ of $\wedge^{p-1}(M^*)$ into M; it follows from formula (60) of no. 7 that there is a canonical factorization

$$
\lambda_z : \wedge^{p-1}(E^*) \xrightarrow{\wedge^{p-1}(t_j)} \wedge^{p-1}(M^*) \xrightarrow{\mu_z} M \xrightarrow{j} E
$$

which proves that $N \subset M$ and hence $N \subset M_z$ by definition of $M_z$. It remains to verify that $N = M_z$. Suppose the converse: there would then exist a basis $(e_i)_{1 \leq i \leq n}$ of $M_z$ and an element $x^* \in E^*$ such that $\langle x^*, e_1 \rangle = 1, \langle x^*, e_j \rangle = 0$ for $2 \leq j \leq n$ and such that $x^*$ is orthogonal to N and hence $x^* \perp z = 0$. We write $z = \sum_H a_H e_H$, where the sum is taken over the subsets of $\{1, n\}$ with $p$ elements. By (68) (no. 9),

$$
x^* \perp e_H = 0 \quad \text{if } 1 \notin H \\
x^* \perp e_{\{1\} \cup H} = e_H \quad \text{if } H \subset \{2, n\}
$$

which shows that the relation $x^* \perp z = 0$ implies $a_H = 0$ for $1 \in H$. But this is impossible, for $z$ would then belong to $\wedge^p(M')$, where $M'$ is the subspace of M generated by $e_2, \ldots, e_n$.

### 13. PURE $p$-VECTORS. GRASSMANNIANS

Let K be a field and E a vector space over K. A $p$-vector $z \in \wedge^p(E)$ is called *pure* (or sometimes *decomposable*) if it is non-zero and there exist vectors $x_1, \ldots, x_p$ in E such that $z = x_1 \wedge x_2 \wedge \cdots \wedge x_p$. For this, it is necessary and sufficient that the subspace $M_z$ associated with $z$ (which is always of dimension $\geq p$ for $z \neq 0$) be *exactly* of dimension $p$ (since $\wedge^p(M_z)$ is then of dimension 1). In particular, every *non-zero* scalar, every non-zero element of $E = \wedge^1(E)$, every non-zero element of $\wedge^n(E)$, when E is of dimension $n$, is *pure*.

#### Proposition 15 {#alg-iii-s11-prop-15 .statement}

*Let E be a vector space of dimension n and let e be an element $\neq 0$ of $\wedge^n(E)$ (hence forming a basis of this vector space). Let $\phi : \wedge(E) \to \wedge(E^*)$ be the vector space isomorphism associated with e (no. 11, Proposition 12). If z is a pure element of $\wedge^p(E)$, then $\phi(z)$ is a pure element of $\wedge^{n-p}(E^*)$ and the subspaces associated with z and $\phi(z)$ are orthogonal.*

The cases $p = 0$ and $p = n$ are trivial. Suppose therefore that $1 \leq p \leq n - 1$ and let $z = x_1 \wedge \cdots \wedge x_p \neq 0$. Then there exists a basis $(e_i)_{1 \leq i \leq n}$ of E such that $e_i = x_i$ for $1 \leq i \leq p$ and $e = e_1 \wedge e_2 \wedge \cdots \wedge e_n$. It then follows from formula (78) of no. 11 that $\phi(z) = \pm e_{p+1}^* \wedge \cdots \wedge e_n^*$, whence the proposition.

#### Corollary {#alg-iii-s11-n13-cor-1 .statement}

*If E is of dimension n, every non-zero $(n-1)$-vector E is pure.*

#### Proposition 16 {#alg-iii-s11-prop-16 .statement}

*For an element $z \neq 0$ of $\bigwedge^p(E)$ to be pure, it is necessary and sufficient that, for all $u^* \in \bigwedge^{p-1}(E^*)$,

$$
(u^* \perp z) \wedge z = 0.
$$

The case $p = 0$ is trivial and we assume $p \geq 1$. If $z = x_1 \wedge \cdots \wedge x_p$, formula (68) (no. 9) with $n = p - 1$ shows that $u^* \perp z$ is a linear combination of the $x_i$ ($1 \leq i \leq p$), whence (81). If on the other hand the subspace $M_z$ associated with $z$ is of dimension $> p$, consider a basis $(e_j)_{1 \leq j \leq n}$ of this subspace with $n > p$. It follows from no. 11, Proposition 13 that each of the $e_j$ is of the form $u^* \perp z$ for some $u^* \in \bigwedge^{p-1}(E^*)$ and relation (81) therefore implies $e_j \wedge z = 0$ for $1 \leq j \leq n$. It follows that in the expression $z = \sum_H a_H e_H$ (where H runs through the set of subsets of $\{1, n\}$ with $p$ elements) all the coefficients $a_H$ are zero, whence $z = 0$, contrary to the hypothesis.

The criterion of Proposition 16 is equivalent to writing conditions (81) when $u^*$ runs through a *basis* of $\bigwedge^{p-1}(E^*)$. In particular, suppose that E is of finite dimension $n$ and let $(e_i)_{1 \leq i \leq n}$ be a basis of E. Conditions (81) are then equivalent to the conditions

$$(82-(J, H))$$
$$
\langle e_J^*, (e_H^* \perp e_I) \wedge z \rangle = 0
$$
for all subsets J, H of $\{1, n\}$ such that $\mathrm{Card}(J) = p + 1$ and $\mathrm{Card}(H) = p - 1$. Now, if I and I' are two subsets of $\{1, n\}$ with $p$ elements, formulae (76) of no. 10 and multiplication table (20) of § 7, no. 8 show that

$$
\langle e_J^*, \langle e_H^* \perp e_I \rangle \wedge e_{I'} \rangle = 0
$$
*unless* there exists an $i \in \{1, n\}$ such that $I - H = \{i\}$ and $J - I' = \{i\}$, in which case

$$(83)$$
$$
\langle e_J^*, (e_H^* \perp e_I) \wedge e_{I'} \rangle = (-1)^{(p-1)(p-2)/2} \varepsilon_{i, J, H}
$$
where $\varepsilon_{i, J, H} = \rho_{\{i\}, H} \rho_{\{i\}, I'}$; it can then be said that for $i \in J \cap C H$, $\varepsilon_{i, J, H}$ is equal to $+1$ if the number of element of J which are $< i$ and the number of elements of H which are $< i$ have the *same parity*, and $-1$ otherwise.

It follows immediately that if we write $z = \sum_I a_I e_I$, where I runs through the set of subsets of $\{1, n\}$ with $p$ elements, relation (82–(J, H)) is equivalent to the relation

$$
\sum_{i \in J \cup C_H} \varepsilon_{i, J, H} a_{J-\{i\}} a_{H \cup \{i\}} = 0.
$$

Relations (84) are called *Grassman’s relations*; these are therefore necessary and sufficient conditions (when J describes the set of subsets with $p + 1$ elements and H the set of subsets with $p - 1$ elements of $\{1, n\}$) for an element $z \neq 0$ of $\bigwedge^p(E)$ to be *pure*.

Note that relations (84) are not independent. For example, for $n = 4$ and $p = 2$, Grassmann’s relations reduce to the single relation

$$
a_{12} a_{34} - a_{13} a_{24} + a_{14} a_{23} = 0.
$$

Let $D_p(E)$ be the subset of $\bigwedge^p(E)$ consisting of the *pure* $p$-vectors; clearly $D_p(E)$ is saturated with respect to the equivalence relation between $u$ and $v$: “there exists $\lambda \in K^*$ such that $v = \lambda u$” and two elements $u, v$ of $D_p(E)$ are equivalent under this relation if and only if the subspaces $M_u$ and $M_v$ of E which are associated with them are the same. Therefore we thus obtain a *canonical bijection* of the *set of p-dimensional vector subspaces* of E onto the *image* $G_p(E)$ of $D_p(E)$ *in the projective space* $\mathbf{P}(\bigwedge^p(E))$ associated with $\bigwedge^p(E)$. The subset $G_p(E)$ of $\mathbf{P}(\bigwedge^p(E))$ is called the *Grassmannian* of index $p$ of the vector space E. When E is finite-dimensional and $(e_i)_{1 \leq i \leq n}$ is a basis of E, the Grassmannian of index $p$ is the set of points of $\mathbf{P}(\bigwedge^p(E))$ for which a system of homogeneous coordinates $(a_I)$ (relative to the basis $(e_I)$ of $\bigwedge^p(E)$) satisfies Grassmann’s relations (84).

When $E = K^n$, we sometimes write $G_{n,p}(K)$ instead of $G_p(K^n)$, so that $G_{n,1}(K) = P_{n-1}(K)$. The mapping $M \mapsto M^0$, which associates with every $p$-dimensional subspace of $K^n$ the *orthogonal* subspace in $E^*$ (identified with $K^n$ under the choice of basis dual to the canonical basis of $K^n$) therefore defines a canonical *bijection* of $G_{n,p}(K)$ onto $G_{n,n-p}(K)$; Proposition 15 shows that this bijection is the *restriction* to $G_{n,p}(K)$ of a canonical *isomorphism* of the projective space $\mathbf{P}(\bigwedge^p(K^n))$ onto the projective space $\mathbf{P}(\bigwedge^{n-p}(K^n))$.

### Exercises {#alg-iii-s11-exercises}

See the [exercises for § 11](exercises/s11/).
