---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: I
chapter_title: Lie Algebras
section: 3
section_title: Representations
lang: en
source: lie-i-iii
pdf_pages: 0043-0056, 0103-0109
extraction: ocr
subsections:
    - "no": 1
      title: REPRESENTATIONS
      page: 0
      pdf_page: 43
    - "no": 2
      title: TENSOR PRODUCT OF REPRESENTATIONS
      page: 0
      pdf_page: 46
    - "no": 3
      title: REPRESENTATIONS ON HOMOMORPHISM MODULES
      page: 0
      pdf_page: 47
    - "no": 4
      title: EXAMPLES
      page: 0
      pdf_page: 49
    - "no": 5
      title: INVARIANT ELEMENTS
      page: 0
      pdf_page: 50
    - "no": 6
      title: INVARIANT BILINEAR FORMS
      page: 0
      pdf_page: 51
    - "no": 7
      title: CASIMIR ELEMENT
      page: 0
      pdf_page: 53
    - "no": 8
      title: EXTENSION OF THE BASE RING
      page: 0
      pdf_page: 54
statements: 24
exercises: 12
content_sha256: 7d8bba5f2b515dc174b1c1ea0359bd8646b26cd6ba716e17900d892c6d4d330a
---

## § 3. REPRESENTATIONS

### 1. REPRESENTATIONS

#### Definition 1 {#lie-i-s3-def-1 .statement}

*Let $g$ be a Lie algebra over $K$ and $M$ a $K$-module. A homomorphism of $g$ into the Lie Algebra $gl(M)$ is called a representation of $g$ on the module $M$. An injective representation is called faithful. If $K$ is a field, the dimension (finite or infinite) of $M$ over $K$ is called the dimension of the representation. The representation $x \mapsto \operatorname{ad} x$ of $g$ on the $K$-module $g$ is called the adjoint representation of $g$.*

A representation of $g$ on $M$ is thus a $K$-linear mapping $\rho$ of $g$ into the endomorphism module of $M$ such that

$$
\rho([x, y]) \cdot m = \rho(x) \rho(y) \cdot m - \rho(y) \rho(x) \cdot m
$$

for all $x \in g, y \in g, m \in M$.

#### Example {#lie-i-s3-n1-exa-1 .statement}

Let G be a real Lie group, g its Lie algebra and θ an analytic representation of G on a finite-dimensional real vector space E. Then the corresponding homomorphism of g into gl(E) is a representation of g on E.*

Let U be the enveloping algebra of g. Proposition 1 of § 2, no. 1 defines a one-to-one correspondence between the set of representations of g on M and the set of representations of U on M. On the other hand we know (Algebra, Chapter VIII, § 13, no. 1) that there is an equivalence between the notion of representation of the associative algebra U and that of left U-module.

#### Definition 2 {#lie-i-s3-def-2 .statement}

*Let g be a Lie algebra over K and U its enveloping algebra. A unitary left module over U is called a left g-module, or simply a g-module.*

If M is a g-module and x ∈ U, x_M will denote the homothety of M defined by x (cf. Algebra, Chapter VIII, § 1, no. 2).

A unitary right module over U is called a right g-module. Such a module is identified with a left U^0-module, that is (§ 2, no. 4) with a left g^0-module.

Let φ be the principal antiautomorphism of U. If M is a right g-module, a left g-module structure is defined on M by writing a.m = m.φ(a) for m ∈ M and a ∈ U.

The notions and results of the theory of modules can be translated into the language of representations:

(1) Two representations ρ and ρ' of g on M and M' are called *similar* or *isomorphic* if the g-modules M and M' are isomorphic. For this it is necessary and sufficient that there exist an isomorphism u of the K-module M onto the K-module M' such that

$$
\rho'(x) = u \circ \rho(x) \circ u^{-1}
$$

for all x ∈ g.

(2) For all i ∈ I, let ρ_i be a representation of g on M_i. Let M be the g-module the direct sum of the g-modules M_i. There is a corresponding representation ρ of g on M, called the *direct sum* of the ρ_i and denoted by $\sum_{i \in I} \rho_i$ (or $\rho_1 + \cdots + \rho_n$ in the case of n representations $\rho_1, \ldots, \rho_n$). If $m = (m_i)_{i \in I}$ is an element of M and x ∈ g, then $\rho(x).m = (\rho_i(x).m_i)_{i \in I}$.

(3) A representation ρ of g on M is called *simple* or *irreducible* if the associated g-module is simple. It amounts to the same to say that there exists no sub-K-module of M (other than {0} and M) stable under all the $\rho(x), x \in g$. A class of simple g-modules (Algebra, Chapter VIII, § 3, no. 2) defines a *class of simple representations of g*.

(4) A representation ρ of g on M is called *semi-simple* or *completely reducible* if the associated g-module is semi-simple. It amounts to the same to say that ρ is similar to a direct sum of simple representations or that every sub-K-module of

M stable under the $\rho(x)$ ($x \in g$) has a supplement stable under the $\rho(x)$ ($x \in g$) (cf. *Algebra*, Chapter VIII, § 3, no. 3).

(5) Let $\delta$ be a class of simple representations of $g$ corresponding to a class C of simple $g$-modules. On the other hand let $\rho$ be a representation of $g$ on M. The isotypical component $M_C$ of species C of the $g$-module M (*Algebra*, Chapter VIII, § 3, no. 4) is also called the *isotypical component of M of species* $\delta$. This component is the sum of the sub-K-modules of M stable under the $\rho(x)$ and on which the $\rho(x)$ induce a representation of class $\delta$; it is the direct sum of certain of these submodules; if $M_C$ is of length $n$, $\rho$ is said to *contain* $\delta$ *n times*. The sum of the different $M_C$ is direct; it is equal to M if and only if $\rho$ is semi-simple.

(6) Let $\rho, \rho'$ be two representations of $g$. $\rho'$ is called a *subrepresentation* (resp. *quotient representation*) of $\rho$ if the module of $\rho'$ is a submodule (resp. quotient module) of the module of $\rho$.

Let M be a K-module. The zero representation of $g$ on M defines on M a $g$-module structure. With this structure M is called a *trivial* $g$-module.

Let M be a $g$-module. The quotient $g$-modules of the sub-$g$-modules of M are also the sub-$g$-modules of the quotient modules of M: they are obtained by considering two sub-$g$-modules U, $U'$ of M such that $U \supset U'$ and forming the $g$-module $U/U'$. Then if all the simple modules of the above type are isomorphic to a given simple $g$-module N, M is called a *pure* $g$-module *of species* N. If $\rho$ and $\sigma$ are the representations of $g$ corresponding to M and N, we also say that $\rho$ is *pure of species* $\sigma$.

Let $M'$ be a sub-$g$-module of M. For M to be pure of species N, it is necessary and sufficient that $M'$ and $M/M'$ be pure of species N. For the condition is obviously necessary. Suppose that it holds and let U, $U'$ be sub-$g$-modules of M such that $U' \subset U$ and $U/U'$ is simple; let $\phi$ be the canonical homomorphism of M onto $M/M'$; if $\phi(U) \neq \phi(U')$, $U/U'$ is isomorphism to $\phi(U)/\phi(U')$ and hence isomorphic to N; if $\phi(U) = \phi(U')$, then $U \subset U' + M'$, hence $U/U'$ is isomorphic to a simple submodule of $(U' + M')/U'$ and the latter module is itself isomorphic to $M'/(U' \cap M')$; hence $U/U'$ is again isomorphic to N, so that M is pure of species N.

Henceforth let M be a $g$-module and suppose that the set of sub-$g$-modules of M which are pure of species N admits a maximal element $M'$. Then every submodule $M''$ of M which is pure of species N is contained in $M'$. For $M''/(M' \cap M'')$ and $M'$ are pure of species N, hence $M' + M''$ is pure of species N by the above and hence $M' + M'' \subset M'$.

Suppose that the $g$-module M admits a Jordan-Hölder series $(M_i)_{0 \leq i \leq n}$. For M to be pure of species N, it is necessary and sufficient that $M_0/M_1, M_1/M_2, \ldots, M_{n-1}/M_n$ be isomorphic to N; for the condition is obviously necessary and its sufficiency follows immediately by induction on $n$ from what we have seen above.

#### Proposition 1 {#lie-i-s3-prop-1 .statement}

*Let g be a Lie algebra over K and a an ideal of g. Let M be a g-module* and $N$ a simple $a$-module. Consider $M$ as an $a$-module and suppose that the set of sub-$a$-modules of $M$ which are pure of species $N$ admits a maximal element $M'$. Then $M'$ is a sub-$g$-module of $M$.

Let $y \in g$. Let $\phi$ be the canonical mapping of $M$ onto $M/M'$ and $f$ the mapping $m \mapsto \phi(y_M \cdot m)$ of $M'$ into $M/M'$. It suffices to show that $f(M') = \{0\}$. Let $x \in a$. Then, for $m \in M$,

$$
x_{M/M'} \cdot f(m) = \phi(x_M y_M \cdot m) = \phi(y_M x_M \cdot m) + \phi([x, y]_M \cdot m).
$$

Now $[x, y] \in a$, whence $\phi([x, y]_M \cdot m) = 0$; on the other hand,

$$
\phi(y_M x_M \cdot m) = f(x_M \cdot m).
$$

Hence $x_{M/M'} \cdot f(m) = f(x_M \cdot m)$. It follows that $f(M')$ is a sub-$a$-module of $M/M'$ isomorphic to a quotient of $M'$ and hence pure of species $N$; hence $f(M') = \{0\}$.

#### Corollary {#lie-i-s3-n1-cor-1 .statement}

*Let $g$ be a Lie algebra over $K$ and $a$ an ideal of $g$. Let $M$ be a simple $g$-module, of finite length as a $K$-module. There exists a simple $a$-module $N$ such that $M$ is a pure $a$-module of species $N$.*

Since the $a$-module $M$ is of finite length, there exists a minimal element $N$ in the set of sub-$a$-modules of $M$: it is a simple sub-$a$-module of $M$. The largest sub-$a$-module of $M$ which is pure of species $N$ is therefore $\neq \{0\}$ and is a sub-$g$-module of $M$ (Proposition 1) and is therefore identical with $M$.

### 2. TENSOR PRODUCT OF REPRESENTATIONS

We have defined in no. 1 the direct sum of a family of representations of $g$. We shall now define other operations on representations.

Let $g_1, g_2$ be two Lie algebras over $K$ and $M_i$ a $g_i$-module ($i = 1, 2$). Let $U_i$ be the enveloping algebra of $g_i$ and $\sigma_i$ the canonical mapping of $g_i$ into $U_i$. Then $M_i$ is a left $U_i$-module and hence $M_1 \otimes_K M_2$ has a canonical left $(U_1 \otimes_K U_2)$-module structure. Now $U_1 \otimes_K U_2$ is the enveloping algebra of $g_1 \times g_2$ and the mapping $(x_1, x_2) \mapsto \sigma_1(x_1) \otimes 1 + 1 \otimes \sigma_2(x_2)$ is the canonical mapping of $g_1 \times g_2$ into this enveloping algebra (§ 2, no. 2). Hence there exists a $(g_1 \times g_2)$-module structure on $M = M_1 \otimes_K M_2$ such that:

$$
\begin{align*}
(1) \quad (x_1, x_2)_M \cdot (m_1 \otimes m_2) &= (\sigma_1(x_1) \otimes 1 + 1 \otimes \sigma_2(x_2)) \cdot (m_1 \otimes m_2) \\
&= ((x_1)_{M_1} \cdot m_1) \otimes m_2 + m_1 \otimes ((x_2)_{M_2} \cdot m_2).
\end{align*}
$$

This structure defines a representation of $g_1 \times g_2$ on $M$.

If now $g_1 = g_2 = g$, the homomorphism $x \mapsto (x, x)$ of $g$ into $g \times g$, composed with the above representation, defines a representation of $g$ on $M$ and hence a $g$-module structure on $M$ such that:

$$
(2) \quad x_M \cdot (m_1 \otimes m_2) = (x_{M_1} \cdot m_1) \otimes m_2 + m_1 \otimes (x_{M_2} \cdot m_2).
$$

By an analogous argument we see that:

#### Proposition 2 {#lie-i-s3-prop-2 .statement}

Let $g$ be a Lie algebra over $K$ and $M_i$ a $g$-module ($1 \leq i \leq n$). On the tensor product $M_1 \otimes_K M_2 \otimes \cdots \otimes M_n$, there exists one and only one $g$-module structure such that

$$
x_M \cdot (m_1 \otimes \cdots \otimes m_m) = \sum_{t=1}^n m_1 \otimes \cdots \otimes (x_{M_t} \cdot m_i) \otimes \cdots \otimes m_n
$$

for all $x \in g, m_1 \in M_1, \ldots, m_n \in M_n$.

The corresponding representation is called the *tensor product* of the given representations of $g$ on the $M_i$.

In particular, if $M$ is a $g$-module, Proposition 2 defines a $g$-module structure on each $M_p = \bigotimes^p M$ and hence on the tensor algebra $T$ of $M$.

Formula (3) shows that, for all $x \in g, x_T$ is the unique *derivation* of the algebra $T$ which extends $x_M$. We know (§ 2, no. 8) that $x_T$ defines on passing to the quotient a derivation of the symmetric algebra $S$ of $M$. Hence $S$ can be considered as a quotient $g$-module of $T$ and the $x_S$ are derivations of $S$.

Still more particularly, consider $g$ as a $g$-module by means of the adjoint representation of $g$. Let $U$ be the enveloping algebra of $g$. By Proposition 7 of § 2, $x_M$ defines on passing to the quotients a derivation of $U$ which is just the inner derivation defined by $\sigma(x)$ ($\sigma$ denoting the canonical mapping of $g$ into $U$). Then $U$ can be considered as a quotient $g$-module of $T$. If $K$ is a field of characteristic 0, the canonical isomorphism of $S$ onto $U$ is a $g$-module isomorphism (§ 2, no. 8).

### 3. REPRESENTATIONS ON HOMOMORPHISM MODULES

Again let $g_1$ and $g_2$ be two Lie algebras over $K$ and $M_i$ a $g_i$-module ($i = 1, 2$). Let $U_i$ be the enveloping algebra of $g_i$ and $\sigma_i$ the canonical mapping of $g_i$ into $U_i$. Then $M_i$ is a left $U_i$-module and hence $\mathcal{L}_K(M_1, M_2)$ has a canonical left $(U_1^0 \otimes U_2)$-module structure. Now $U_1^0 \otimes_K U_2$ is the enveloping algebra of $g_1^0 \times g_2$ and the mapping

$$
(x_1, x_2) \mapsto \sigma_1(x_1) \otimes 1 + 1 \otimes \sigma_2(x_2)
$$

is the canonical mapping of $g_1^0 \times g_2$ into this enveloping algebra. Hence there exists a $(g_1^0 \times g_2)$-module structure on $M = \mathcal{L}_K(M_1, M_2)$ such that

$$
((x_1, x_2)_M \cdot u) \cdot m_1 = ((\sigma_1(x_1) \otimes 1 + 1 \otimes \sigma_2(x_2)) \cdot u) \cdot m_1 \\
= u((x_1)_{M_1} \cdot m_1) + (x_2)_{M_2} \cdot u(m_1)
$$

for all $u \in \mathcal{L}_K(M_1, M_2), m_1 \in M_1$. This structure defines a representation of $g_1^0 \times g_2$ on $M$.

If now $g_1 = g_2 = g$, the homomorphism $x \mapsto (-x, x)$ of $g$ into $g^0 \times g$, composed with the above representation, defines a representation of $g$ on $M$ and hence a $g$-module structure on $M$ such that

$$
(x_M \cdot u) \cdot m_1 = x_{M_2} \cdot u(m_1) - u(x_{M_1} \cdot m_1)
$$

or

$$
x_M \cdot u = x_{M_2} u - u x_{M_1}.
$$

Combining these results with Proposition 2, we see that:

#### Proposition 3 {#lie-i-s3-prop-3 .statement}

*Let $g$ be a Lie algebra over $K$ and $M_i$ a $g$-module ($1 \leq i \leq n + 1$). Let $N$ be the $K$-module $\mathcal{L}_K(M_1, \ldots, M_n; M_{n+1})$ of multilinear mappings of $\prod_{i=1}^n M_i$ into $M_{n+1}$. There exists one and only one $g$-module structure on $N$ such that*

$$
(x_N \cdot u)(m_1, \ldots, m_n) = - \sum_{i=1}^n u(m_1, \ldots, x_{M_i} \cdot m_i, \ldots, m_n)
$$
$$
+ x_{M_{n+1}} \cdot u(m_1, \ldots, m_n)
$$

*for all* $x \in g, u \in N$ *and* $m_i \in M_i$ ($1 \leq i \leq n$).

In particular, let $g$ be a Lie algebra over $K$ and $M$ a $g$-module and consider $K$ as a trivial $g$-module. Proposition 3 defines a $g$-module structure on $\mathcal{L}_K(M, K) = M^*$. The corresponding representation is called the *dual* representation of the representation $x \mapsto x_M$. We have:

$$
(x_{M^*} \cdot f)(m) = -f(x_M \cdot m)
$$

for all $x \in g, f \in M^*, m \in M$. In other words:

$$
x_{M^*} = -{}^t x_M.
$$

When $K$ is a field and $M$ is finite-dimensional, the $g$-module $M$ is simple (resp. semi-simple) if and only if the $g$-module $M^*$ is simple (resp. semi-simple).

#### Proposition 4 {#lie-i-s3-prop-4 .statement}

*Let $M_1, M_2$ be two $g$-modules. The canonical $K$-linear mappings* (Algebra, Chapter II, § 4, no. 2, Proposition 2 and no. 1, Proposition 1):

$$
M_1^* \otimes_K M_2 \xrightarrow{\phi} \mathcal{L}_K(M_1, M_2), \quad \mathcal{L}_K(M_1, M_2^*) \xrightarrow{\psi} (M_1 \otimes_K M_2)^*
$$

*(where the second is bijective)* are $g$-module homomorphisms.

We write

$$
N = M_1^* \otimes M_2, \quad P = \mathcal{L}(M_1, M_2), \quad Q = \mathcal{L}(M_1, M_2^*), \quad R = (M_1 \otimes M_2)^*.
$$

Then, for $x \in g, f \in M_1^*, m_1 \in M_1, m_2 \in M_2$,

$$
((\phi x_N)(f \otimes m_2)) \cdot m_1 = (\phi(x_{M_1^*} f \otimes m_2 + f \otimes x_{M_2} m_2)) \cdot m_1 \\
= \langle x_{M_1^*} f, m_1 \rangle m_2 + \langle f, m_1 \rangle x_{M_2} m_2
$$

$$
((x_P \phi)(f \otimes m_2)) \cdot m_1 = x_{M_2}(\phi(f \otimes m_2) \cdot m_1) - \phi(f \otimes m_2)(x_{M_1} m_1) \\
= \langle f, m_1 \rangle x_{M_2} m_2 - \langle f, x_{M_1} m_1 \rangle m_2
$$

and hence $\phi x_N = x_P \phi$. On the other hand, for $x \in g, u \in \mathcal{L}(M_1, M_2^*), m_1 \in M_1, m_2 \in M_2$:

$$
(\psi x_Q u)(m_1 \otimes m_2) = \langle (x_Q u) \cdot m_1, m_2 \rangle = \langle x_{M_2^*} u m_1 - u x_{M_1} m_1, m_2 \rangle \\
(x_R \psi u)(m_1 \otimes m_2) = -\langle \psi u, x_{M_1} m_1 \otimes m_2 + m_1 \otimes x_{M_2} m_2 \rangle \\
= -\langle u x_{M_1} m_1, m_2 \rangle - \langle u m_1, x_{M_2} m_2 \rangle
$$

and hence $\psi x_Q = x_R \psi$, which completes the proof.

The $g$-modules $\mathcal{L}(M_1, M_2^*)$ and $(M_1 \otimes M_2)^*$ are identified under the isomorphism $\psi$. If $M_1$ and $M_2$ have finite bases, $\phi$ is an isomorphism (Algebra, Chapter II, § 4, no. 2, Proposition 2), which allows us to identify the $g$-modules $M_1^* \otimes M_2$ and $\mathcal{L}(M_1, M_2)$; in that case, we can therefore identify the $g$-modules $M_1^* \otimes M_2^*, \mathcal{L}(M_1, M_2^*)$ and $(M_1 \otimes M_2)^*$.

### 4. EXAMPLES

#### Example 1 {#lie-i-s3-n4-exa-1 .statement}

Let $g$ be a Lie algebra over $K$ and $M$ a $g$-module. The $g$-module structure on $M$ and the trivial $g$-module structure on $K$ define a $g$-module structure on the $K$-module $N = \mathcal{L}(M, M; K)$ of bilinear forms on $M$. Then

$$
(x_N \cdot \beta)(m, m') = -\beta(x_M \cdot m, m') + \beta(m, x_M \cdot m')
$$

for all $x \in g, m, m'$ in $M, \beta \in N$. If $\beta$ is a given element of $N$, the set of $x \in g$ such that $x_N \cdot \beta = 0$ is a subalgebra of $g$.

Let $M$ be a $K$-module and $\beta$ a bilinear form on $M$. By the above, the set of $x \in gl(M)$ such that

$$
\beta(x \cdot m, m') + \beta(m, x \cdot m') = 0
$$

for all $m \in M$ and $m' \in M$ is a Lie subalgebra of $gl(M)$. Suppose that $K$ is a field, $M$ is finite-dimensional and $\beta$ is non-degenerate. Then every $x \in gl(M)$ admits a left adjoint $x^*$ (relative to $\beta$) which is everywhere defined and the subalgebra in question is the set of $x \in gl(M)$ such that $x^* = -x$. By this process we can construct two important examples of Lie algebras:

(a) Take $M = K^n$ and

$$
\beta((\xi_1, \ldots, \xi_n), (\eta_1, \ldots, \eta_n)) = \xi_1 \eta_1 + \cdots + \xi_n \eta_n.
$$

We canonically identify $gl(K^n)$ with $M_n(K)$. Then the Lie algebra obtained is the Lie algebra of skew-symmetric matrices. *(When $K = \mathbf{R}$, this algebra is the Lie algebra of the orthogonal group $O(n, \mathbf{R})$).*

(b) Take $M = K^{2m}$ and
$$
\beta((\xi_1, \ldots, \xi_{2m}), (\eta_1, \ldots, \eta_{2m})) = \xi_1 \eta_{m+1} - \eta_1 \xi_{m+1} + \cdots + \xi_m \eta_{2m} - \eta_m \xi_{2m}.
$$
The matrix of $\beta$ with respect to the canonical basis of $K^{2m}$ is the matrix
$$
\begin{pmatrix}
0 & I_m \\
-I_m & 0
\end{pmatrix}.
$$
Let $U = \begin{pmatrix} A & B \\ C & D \end{pmatrix}$ be the matrix with respect to the canonical basis of $K^{2m}$ of an element $u$ of $\mathrm{gl}(M)$ ($A, B, C, D$ lying in $\mathbf{M}_m(K)$). By formula (50) of *Algebra*, Chapter IX, § 1, no. 10, $u^*$ has with respect to the same basis the matrix
$$
\begin{pmatrix}
0 & -I_m \\
I_m & 0
\end{pmatrix}
\begin{pmatrix}
tA & tC \\
tB & tD
\end{pmatrix}
\begin{pmatrix}
0 & I_m \\
-I_m & 0
\end{pmatrix}
= \begin{pmatrix}
tD & -tB \\
-tC & tA
\end{pmatrix}.
$$
The condition $u^* = -u$ is therefore equivalent to the conditions
$$
D = -tA \quad B = tB \quad C = tC.
$$
*When $K = \mathbf{R}$, the Lie algebra obtained is the Lie algebra of the symplectic group $\mathbf{Sp}(2m, \mathbf{R})$.*

#### Example 2 {#lie-i-s3-n4-exa-2 .statement}

We preserve the notation of *Example 1*.

The $g$-module structure on $M$ defines on the $K$-module $P = \mathcal{L}_K(M, M)$ of endomorphisms of $M$ a $g$-module structure. By (6), for all $x \in g$ and $u \in P$:
$$(11)$$
$$
x_P \cdot u = [x_M, u] = (\mathrm{ad}\, x_M) \cdot u
$$
where $\mathrm{ad}\, x_M$ denotes the image of $x_M$ under the adjoint representation of $\mathrm{gl}(M)$. In other words:
$$(12)$$
$$
x_P = \mathrm{ad}\, x_M
$$
in $\mathcal{L}(\mathcal{L}(M, M)) = \mathcal{L}(\mathrm{gl}(M))$.

### 5. INVARIANT ELEMENTS

#### Definition 3 {#lie-i-s3-def-3 .statement}

*Let $g$ be a Lie algebra and $M$ a $g$-module. An element $m \in M$ is called invariant (with respect to the $g$-module structure on $M$ or with respect to the corresponding representation of $g$) if $x_M \cdot m = 0$ for all $x \in g$.*

*Let $G$ be a connected real Lie group, $g$ its Lie algebra, $\theta$ an analytic representation of $G$ on a finite-dimensional real vector space $E$ and $\rho$ the corresponding representation of $g$ on $E$. Let $m \in E$. The element $m$ is invariant with respect to $\rho$ if and only if $\theta(g) \cdot m = m$ for all $g \in G$. This justifies the use of the word "invariant".*

#### Example 1 {#lie-i-s3-n5-exa-1 .statement}

Let $M, N$ be two $g$-modules and $P = \mathcal{L}_K(M, N)$. For an element $f$ of $P$ to be invariant, it is necessary and sufficient, by (6), that $f$ be a homomorphism of the $g$-module $M$ into the $g$-module $N$. In particular, if $M = N$ and $x_M = x_N$ for all $x \in g$, $f$ is invariant if and only if $f$ is permutable with the $x_M$.

#### Example 2 {#lie-i-s3-n5-exa-2 .statement}

Let M be a K-module with a finite basis. If M has a g-module structure, $\mathcal{L}(M, M)$ and $M^* \otimes M$ have g-module structures and the canonical mapping of $M^* \otimes M$ into $\mathcal{L}(M, M)$ is a g-module isomorphism (Proposition 4). As $1 \in \mathcal{L}(M, M)$ is obviously an invariant (cf. Example 1), the corresponding element $u$ of $M^* \otimes M$ is an invariant. If $(e_i)_{1 \leq i \leq n}$ is a basis of M and $(e_i^*)_{1 \leq i \leq n}$ is the dual basis, we have $u = \sum_{i=1}^n e_i^* \otimes e_i$.

#### Example 3 {#lie-i-s3-n5-exa-3 .statement}

Let M be a g-module. Let $\beta$ be a bilinear form on M and f the corresponding element of $\mathcal{L}(M, M^*)$. For $\beta$ to be invariant, it is necessary and sufficient that f be a g-module homomorphism (Proposition 4 and Example 1). Suppose that K is a field and that $\dim_K M < +\infty$. A non-degenerate invariant bilinear form $\beta$ on M defines an isomorphism of the g-module M onto the g-module $M^*$ and hence an isomorphism of the g-module $M \otimes M$ onto the g-module $M^* \otimes M$. Thus, by Example 2, giving $\beta$ defines canonically an invariant element c in the g-module $M \otimes M$, which can be constructed as follows: let $(e_i)_{1 \leq i \leq n}$ be a basis of M and $(e'_i)_{1 \leq i \leq n}$ the basis of M such that $\beta(e_i, e'_j) = \delta_{ij}$; then $c = \sum_{i=1}^n e_i \otimes e'_i$.

#### Proposition 5 {#lie-i-s3-prop-5 .statement}

*Let g be a Lie K-algebra, h an ideal of g, $\rho$ a representation of g on M and $\rho'$ the restriction of $\rho$ to h. Then the set N of elements of M invariant with respect to $\rho'$ is stable under $\rho(g)$.*

Let $n \in N$ and $y \in g$; for all $x \in h, [x, y] \in h$ and hence
$$
\rho(x)\rho(y)n = \rho([x, y])n + \rho(y)\rho(x)n = 0;
$$
hence $\rho(y)n \in N$.

#### Proposition 6 {#lie-i-s3-prop-6 .statement}

*Let M be a semi-simple g-module. Then the submodule $M_0$ of invariant elements of M admits one and only one supplement stable under the $x_M$, namely the submodule $M_1$ generated by the $x_M.m$ ($x \in g, m \in M$).

Let $M'$ be a submodule of M which is stable under the $x_M$ and a supplement of $M_0$ in M. For all $m \in M, m = m_0 + m'$ with $m_0 \in M_0, m' \in M'$, and hence $x_M m = x_M m' \in M'$. Hence $M_1 \subset M'$. Let $M_2$ be a submodule of $M'$ stable under the $x_M$ and supplementary to $M_1$ in $M'$. For all $m \in M_2$,
$$
x_M m \in M_2 \cap M_1 = \{0\}
$$
for all $x \in g$, hence $m \in M_0$ and hence $m = 0$. Hence $M_2 = \{0\}$, which proves that $M_1 = M'$.

### 6. INVARIANT BILINEAR FORMS

Let g be a Lie algebra over K. The adjoint representation of g on g and the zero representation of g on K define a g-module structure on the K-module

$N = \mathcal{L}(g, g; K)$ of bilinear forms on $g$. Briefly we say that a bilinear form $\beta$ on $g$ is *invariant* if it is invariant under the representation $x \mapsto x_N$. By formula (10) the necessary and sufficient condition for this to be so is that:

$$
\beta([x, y], z) = \beta(x, [y, z])
$$

for all $x, y, z$ in $g$.

Now let $\mathfrak{d}$ be the Lie algebra of derivations of $g$. The identity representation of $\mathfrak{d}$ and the zero representation of $\mathfrak{d}$ on $K$ define a representation $D \mapsto D_N$ of $\mathfrak{d}$ on $N$. Briefly we say that a bilinear form on $g$ is *completely invariant* if it is invariant under the representation $D \mapsto D_N$. A completely invariant bilinear form is invariant. For a bilinear form $\beta$ on $g$ to be completely invariant, it is necessary and sufficient that:

$$
\beta(Dx, y) + \beta(x, Dy) = 0
$$

for all $x, y$ in $g$ and $D \in \mathfrak{d}$.

#### Proposition 7 {#lie-i-s3-prop-7 .statement}

*Let $g$ be a Lie algebra, $\beta$ an invariant symmetric bilinear form on $g$ and $a$ an ideal of $g$.*

(a) *The orthogonal $a'$ of $a$ with respect to $\beta$ is an ideal of $g$.*
(b) *If $a$ is characteristic and $\beta$ is completely invariant, $a'$ is characteristic.*
(c) *If $\beta$ is non-degenerate, $a \cap a'$ is commutative.*

Let $D$ be a derivation of $g$. Suppose that $a$ is stable under $D$ and that $\beta(Dx, y) + \beta(x, Dy) = 0$ for $x, y$ in $g$. Then $z \in a'$ implies $Dz \in a'$, since, for all $t \in a$, $Dt \in a$ and hence $\beta(Dz, t) = -\beta(z, Dt) = 0$. Thus $a'$ is stable under $D$. This establishes (a) and (b).

Now let $b$ be an ideal of $g$ and suppose that the restriction of $\beta$ to $b$ is zero. For $x, y$ in $b$ and $z \in g$, $\beta([x, y], z) = \beta(x, [y, z]) = 0$, for $[y, z] \in b$. Thus $[b, b]$ is orthogonal to $g$. If $\beta$ is non-degenerate, $b$ is therefore commutative. This result applied to $a \cap a'$ proves (c).

#### Definition 4 {#lie-i-s3-def-4 .statement}

*Let $g$ be a Lie $K$-algebra and $M$ a $g$-module. Suppose that $M$, considered as a $K$-module, admits a finite basis. The bilinear form associated with the $g$-module $M$ (or with the corresponding representation) is the symmetric bilinear form $(x, y) \mapsto \operatorname{Tr}(x_M y_M)$ on $g$. If the representation in question is the adjoint representation, the associated bilinear form is called the Killing form of $g$.*

#### Proposition 8 {#lie-i-s3-prop-8 .statement}

*Let $g$ be a Lie algebra and $M$ a $g$-module. Suppose that $M$, considered as a $K$-module, admits a finite basis. The bilinear form associated with $M$ is invariant.*

For $x, y, z$ in $g$, we have:

$$
\begin{align*}
\operatorname{Tr}([x, y]_M z_M) &= \operatorname{Tr}(x_M y_M z_M) - \operatorname{Tr}(y_M x_M z_M) = \operatorname{Tr}(x_M y_M z_M) - \operatorname{Tr}(x_M z_M y_M) \\
&= \operatorname{Tr}(x_M [y, z]_M).
\end{align*}
$$

#### Proposition 9 {#lie-i-s3-prop-9 .statement}

*Suppose that $K$ is a field and that the Lie algebra $g$ is finite-dimensional* over $K$. *Let $a$ be an ideal of $g$, $\beta$ the Killing form of $g$ and $\beta'$ the Killing form of $a$. Then $\beta'$ is the restriction of $\beta$ to $a$.

Let $u$ be an endomorphism of the vector space $g$ which leaves $a$ stable. Let $v$ be the restriction of $u$ to $a$ and $w$ the endomorphism of the vector space $g/a$ derived from $u$ when passing to the quotient. Then $\operatorname{Tr} u = \operatorname{Tr} v + \operatorname{Tr} w$ as is seen by taking a basis $(x_1, \ldots, x_n)$ of $g$ of which the first $p$ elements form a basis of $a$. Then let $x \in a, y \in a$ and apply the above formula to the case where $u = (\operatorname{ad}_g x)(\operatorname{ad}_g y)$. Then $v = (\operatorname{ad}_a x)(\operatorname{ad}_a y)$ and $w = 0$. Hence $\beta(x, y) = \beta'(x, y)$.

#### Proposition 10 {#lie-i-s3-prop-10 .statement}

*Suppose that $K$ is a field and that the Lie algebra $g$ is finite-dimensional over $K$. The Killing form $\beta$ of $g$ is completely invariant.*

Let $D$ be a derivation of $g$. There exists a Lie algebra $g'$ containing $g$ as an ideal of codimension 1 and an element $x_0$ of $g'$ such that $Dx = [x_0, x]$ for all $x \in g$ (§ 1, no. 8, Example 1). Let $\beta'$ be the Killing form of $g'$. For $x, y$ in $g$, $\beta'([x, x_0], y) = \beta'(x, [x_0, y])$, that is $\beta'(Dx, y) + \beta'(x, Dy) = 0$. Now the restriction of $\beta'$ to $g$ is $\beta$ (Proposition 9). Hence the proposition.

### 7. CASIMIR ELEMENT

#### Proposition 11 {#lie-i-s3-prop-11 .statement}

*Let $g$ be a Lie algebra over a field $K$, $U$ its enveloping algebra, $h$ a finite-dimensional ideal of $g$ and $\beta$ an invariant bilinear form on $g$, whose restriction to $h$ is non-degenerate. Let $(e_i)_{1 \leq i \leq n}, (e'_j)_{1 \leq j \leq n}$ be two bases of $h$ such that $\beta(e_i, e'_j) = \delta_{ij}$. Then the element $c = \sum_{i=1}^n e_i e'_i$ of $U$ belongs to the centre of $U$ and is independent of the choice of basis $(e_i)$.

For $x \in g$ let $x_h$ be the restriction to $h$ of $\operatorname{ad}_g x$. Then $x \mapsto x_h$ is a representation of $g$ on the vector space $h$ and the restriction $\beta'$ of $\beta$ to $h$ is invariant under this representation. By no. 5, *Example 3*, the tensor $\sum_{i=1}^n e_i \otimes e'_i$ is independent of the choice of basis $(e_i)$ and is an invariant element of the tensor algebra of $h$. It is also an element of the tensor algebra $T$ of $g$, which is invariant for the representation derived from the adjoint representation of $g$. Its canonical image in $U$, that is $c$, is therefore independent of the choice of basis $(e_i)$ and is an invariant for the representation of $g$ on $U$ considered at the end of no. 2. This element is therefore permutable with every element of $g$ and therefore belongs to the centre of $U$.

When $\beta$ is the bilinear form associated with a $g$-module $M$, the element $c$ of Proposition 11 is called the *Casimir element* associated with $M$ (or with the corresponding representation). This element exists if the restriction of $\beta$ to $h$ is non-degenerate.

#### Proposition 12 {#lie-i-s3-prop-12 .statement}

*Let $g$ be a Lie algebra over a field $K$, $h$ an ideal of $g$ of finite dimension n and M a g-module of finite dimension over K. Let c be the Casimir element (assumed to exist) associated with M and h.

(a) $\operatorname{Tr}(c_M) = n$.
(b) *If M is simple and n is not divisible by the characteristic of K, $c_M$ is an automorphism of M*.

In the notation of Proposition 11,

$$
\operatorname{Tr}(c_M) = \sum_{i=1}^n \operatorname{Tr}((e_i)_M(e'_i)_M) = \sum_{i=1}^n \beta(e_i, e'_i) = n.
$$

Hence, if n is not divisible by the characteristic of K, $c_M \neq 0$. On the other hand, as c belongs to the centre of U, $c_M$ is permutable with all the $x_M, x \in g$. If further M is simple, $c_M$ is therefore invertible in $\mathcal{L}(M)$ (*Algebra*, Chapter VIII, § 4, no. 3, Proposition 2).

### 8. EXTENSION OF THE BASE RING

Let $K_1$ be a commutative ring with unit element and $\phi$ a homomorphism of K into $K_1$ mapping 1 to 1. Let g be a Lie K-algebra, U its enveloping algebra and M a left g-module, that is a left U-module. Then $M_{(K_1)}$ has a canonical left $U_{(K_1)}$-module structure and hence a left $g_{(K_1)}$-module structure. Let $\rho$ and $\rho_{(K_1)}$ be the representations of g and $g_{(K_1)}$ corresponding to M and $M_{(K_1)}$: $\rho_{(K_1)}$ is said to be derived from $\rho$ by *extending the base ring* and the results of *Algebra*, Chapter VIII, § 13, no. 4 can be applied. If $x \in g$, $\rho_{(K_1)}(x)$ is just the endomorphism $\rho(x) \otimes 1$ of $M_{(K_1)} = M \otimes_K K_1$.

Suppose that K is a field, that $K_1$ is an extension of K and that $\phi$ is the canonical injection of K into $K_1$. Let V and V' be vector subspaces of M. Let a be the vector subspace of g consisting of the $x \in g$ such that $\rho(x)(V) \subset V'$. Let $a'$ be the vector subspace of $g_{(K_1)}$ consisting of the $x' \in g_{(K_1)}$ such that $\rho_{(K_1)}(x')(V_{(K_1)}) \subset V'_{(K_1)}$. Then $a' = a_{(K_1)}$. For clearly $a_{(K_1)} \subset a'$. Now let $x' \in a'$. We may write $x' = \sum_{i=1}^n \lambda_i x_i$, where the $x_i$ are in g and the $\lambda_i$ are elements of $K_1$ linearly independent over K. For all $u \in V$, $\rho(x') \cdot u \in V'_{(K_1)}$, that is $\sum_{i=1}^n \lambda_i \rho(x_i) \cdot u \in V'_{(K_1)}$, whence $\rho(x_i) \cdot u \in V'$, hence $x_i \in a$ and $x' \in a_{(K_1)}$. This shows that $a' = a_{(K_1)}$. In particular, the *centre* of $g_{(K_1)}$ is derived from the centre of g by extending K to $K_1$: it suffices to apply the above to the adjoint representation of g. It follows that $\mathcal{C}_p(g_{(K_1)}) = (\mathcal{C}_p g)_{(K_1)}$ for all $p$. Similarly, let h be a subalgebra of g and n the *normalizer* of h in g. Then the normalizer of $h_{(K_1)}$ in $g_{(K_1)}$ is $n_{(K_1)}$.

Let K, $K_1$, g, $\rho$, M be as in the last paragraph. Let b be a vector subspace of g and W a vector subspace of M. Let V be the vector subspace of M consisting of the $m \in M$ such that $\rho(b) \cdot m \subset W$. Let V' be the vector subspace of $M_{(K_1)}$ consisting of the $m' \in M_{(K_1)}$ such that $\rho_{(K_1)}(b_{(K_1)}) \cdot m' \subset W_{(K_1)}$. As above it is seen that $V' = V_{(K_1)}$. In particular, the vector subspace of *invariants* of $M_{(K_1)}$ is derived from the vector subspace of invariants of $M$ by extending the base field from $K$ to $K_1$.

Let $K, K_1$ and $\phi$ be as at the beginning of this no. Let $g$ be a Lie $K$-algebra and $M$ and $N$ $g$-modules. If $M$ and $N$ are isomorphic $g$-modules, $M_{(K_1)}$ and $N_{(K_1)}$ are isomorphic $g_{(K_1)}$-modules. Conversely:

#### Proposition 13 {#lie-i-s3-prop-13 .statement}

*Let $K$ be a field, $K_1$ an extension of $K$, $g$ a Lie $K$-algebra and $M, N$ two $g$-modules of finite dimension over $K$. If $M_{(K_1)}$ and $N_{(K_1)}$ are isomorphic $g_{(K_1)}$-modules, $M$ and $N$ are isomorphic $g$-modules.*

The proof is in two steps.

(1) Suppose first that $K_1$ is an extension of $K$ of *finite degree* $n$. Let $U$ be the enveloping algebra of $g$, so that the enveloping algebra of $g_{(K_1)}$ is $U_{(K_1)} = U \otimes_K K_1$ (§ 2, no. 9). As $M_{(K_1)}$ and $N_{(K_1)}$ are isomorphic as $U_{(K_1)}$-modules they are *a fortiori* isomorphic as $U$-modules; but as $U$-modules they are respectively isomorphic to $M^n$ and $N^n$. Now $M$ and $N$ are $U$-modules of finite length; $M$ (resp. $N$) is therefore the direct sum of a family $(P_i^{r_i})_{1 \leq i \leq p}$ (resp. $(Q_j^{s_j})_{1 \leq j \leq q}$) of submodules such that the $P_i$ (resp. $Q_j$) are indecomposable and two $P_i$ (resp. $Q_j$) of different indices are not isomorphic (*Algebra*, Chapter VIII, § 2, no. 2, Theorem 1). Then $M^n$ (resp. $N^n$) is isomorphic to the direct sum of the $P_i^{n r_i}$ (resp. $Q_j^{n s_j}$); it follows (*loc. cit.*) that $p = q$ and that after permuting the $Q_j$ if necessary $n r_i = n s_i$ and $P_i$ is isomorphic to $Q_i$ for $1 \leq i \leq p$, hence $M$ is isomorphic to $N$.

(2) *General case.* Let $P$ be the $g$-module $\mathcal{L}_K(M, N)$ and $Q$ the subspace of invariants of $P$, that is the set of homomorphisms of the $g$-module $M$ into the $g$-module $N$. In the $g_{(K_1)}$-module $\mathcal{L}_{K_1}(M_{(K_1)}, N_{(K_1)}) = (\mathcal{L}_K(M, N))_{(K_1)}$, the subspace of invariants is $Q_{(K_1)}$. The hypothesis that $M_{(K_1)}$ and $N_{(K_1)}$ are isomorphic implies that $M$ and $N$ have the same dimension over $K$ and that there exists in $Q_{(K_1)}$ an element $g$ which is an isomorphism of $M_{(K_1)}$ onto $N_{(K_1)}$. Let $(f_1, \ldots, f_d)$ be a basis of $Q$ over $K$ and choose bases of $M$ and $N$ over $K$. If $\lambda_k \in K_1$ for $1 \leq k \leq d$, the matrix of $f = \sum_{k=1}^d \lambda_k f_k$ with respect to these bases has determinant which is a polynomial $D(\lambda_1, \ldots, \lambda_d)$ with coefficients *in* $K$. When $f = g$, this determinant is non-zero and hence the coefficients of $D$ are not all non-zero. Therefore, if $\Omega$ is the algebraic closure of $K$, there exists (since $\Omega$ is infinite) elements $\mu_k \in \Omega$ $(1 \leq k \leq d)$ such that $D(\mu_1, \ldots, \mu_d) \neq 0$ (*Algebra*, Chapter IV, § 2, no. 5, Proposition 8). If $K_2$ is the algebraic extension of $K$ generated by the $\mu_k$ $(1 \leq k \leq d)$, it follows that $\sum_{k=1}^d \mu_k f_k$ is an isomorphism of $M_{(K_2)}$ onto $N_{(K_2)}$; but $K_2$ is of finite degree over $K$ (*Algebra*, Chapter V, § 3, no. 2, Proposition 5) and hence $M$ and $N$ are isomorphic by the first part of the argument.

Again let $K, K_1$ and $\phi$ be as the beginning of this no. Let $\rho$ be a representation of $g$ on a $K$-module $M$ with a finite basis $(x_1, \ldots, x_n)$. Then the bilinear form on $g_{(K_1)}$ associated with $\rho_{(K_1)}$ is derived from the bilinear form associated with $\rho$ by extending the base ring to $K_1$ (for, if $u \in \mathcal{L}_K(M)$, $u$ has the same matrix with respect to $(x_1, \ldots, x_n)$ as $u \otimes 1$ with respect to $(x_1 \otimes 1, \ldots, x_n \otimes 1)$ and hence $u$ and $u \otimes 1$ have the same trace). In particular, if the $K$-module $g$ has a finite basis, the *Killing form* of $g_{(K_1)}$ is derived from that of $g$ by extending the base ring to $K_1$.

### Exercises {#lie-i-s3-exercises}

See the [exercises for § 3](exercises/s3/).
