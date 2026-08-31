---
book: alg
book_title: Algebra
chapter: III
chapter_title: TENSOR ALGEBRAS, EXTERIOR ALGEBRAS, SYMMETRIC ALGEBRAS
section: 2
section_title: Examples of algebras
lang: en
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 438-457, 618-626
pdf_pages: 0462-0481, 0642-0650
extraction: ocr
subsections:
    - "no": 1
      title: ENDOMORPHISM ALGEBRAS
      page: 438
      pdf_page: 462
    - "no": 2
      title: MATRIX ELEMENTS
      page: 438
      pdf_page: 462
    - "no": 3
      title: QUADRATIC ALGEBRAS
      page: 439
      pdf_page: 463
    - "no": 4
      title: CAYLEY ALGEBRAS
      page: 441
      pdf_page: 465
    - "no": 5
      title: CONSTRUCTION OF CAYLEY ALGEBRAS. QUATERNIONS
      page: 443
      pdf_page: 467
    - "no": 6
      title: ALGEBRA OF A MAGMA, A MONOID, A GROUP
      page: 446
      pdf_page: 470
    - "no": 7
      title: FREE ALGEBRAS
      page: 448
      pdf_page: 472
    - "no": 8
      title: DEFINITION OF AN ALGEBRA BY GENERATORS AND RELATIONS
      page: 450
      pdf_page: 474
    - "no": 9
      title: POLYNOMIAL ALGEBRAS
      page: 452
      pdf_page: 476
    - "no": 10
      title: TOTAL ALGEBRA OF A MONOID
      page: 454
      pdf_page: 478
    - "no": 11
      title: FORMAL POWER SERIES OVER A COMMUTATIVE RING
      page: 455
      pdf_page: 479
statements: 17
exercises: 3
content_sha256: bd5951cd090d56ae73c754360396e4a160968b09d8b97344a2867e90be9ed798
---

## § 2. EXAMPLES OF ALGEBRAS

Throughout this paragraph, A denotes a commutative ring.

### 1. ENDOMORPHISM ALGEBRAS

Let B be an associative A-algebra with a unit element denoted by 1 and let M be a right B-module. We know that the ring $E = \mathrm{End}_B(M)$ also has a module structure over the centre of B. Now the image of the homomorphism $h : \alpha \mapsto \alpha . 1$ of A into B is contained in the centre of B (§ 1, no. 1); hence $h$ gives E an A-module structure. Further, for $\alpha \in A$ and $f, g$ in E,

$$
\alpha(f \circ g) = f \circ (\alpha g) = (\alpha f) \circ g;
$$

hence multiplication in E and the A-module structure on E define an associative A-algebra structure on E; the identity mapping of M is a unit element of this algebra.

### 2. MATRIX ELEMENTS

Let B be a unital associative A-algebra and $\mathbf{M}_n(B)$ the set of square matrice of order n over B (II, § 10, no. 7). Then $\mathbf{M}_n(B)$ has an A-module structure defined by $\alpha . (b_{ij}) = (\alpha b_{ij})$ ($\alpha \in A, b_{ij} \in B, 1 \leq i \leq n, 1 \leq j \leq n$); this structure and matrix multiplication define a unital associative A-algebra structure on $\mathbf{M}_n(B)$. The canonical bijection of $\mathbf{M}_n(B)$ onto $\mathrm{End}_B(B_d^n)$ (II, § 10, no. 7) is an A-algebra isomorphism.

When $B = A$, the A-algebra $\mathbf{M}_n(A)$ admits a canonical basis $(E_{ij})$ consisting of the matrix units (II, § 10, no. 3); the corresponding multiplication table is

$$
E_{ij} E_{hk} = \delta_{jh} E_{ik}.
$$

The unit element $I_n$ is equal to $\sum_{i=1}^n E_{ii}$.

### 3. QUADRATIC ALGEBRAS

Let $\alpha, \beta$ be two elements of A and $(e_1, e_2)$ the canonical basis of $A^2$. The quadratic algebra of type $(\alpha, \beta)$ over A is the A-module $A^2$ with the algebra structure defined by the multiplication table (§ 1, no. 7)

$$
e_1^2 = e_1, \quad e_1 e_2 = e_2 e_1 = e_2, \quad e_2^2 = \alpha e_1 + \beta e_2.
$$

An A-algebra E isomorphic to a quadratic algebra is also called a quadratic algebra. It amounts to the same to say that E admits a basis of two elements one of which is the unit element.

It can be shown that every unital A-algebra which admits a basis of two elements is a quadratic algebra (Exercise 1).

If a basis $(e_1, e_2)$ of an A-algebra has multiplication table (2), it is called a basis of type $(\alpha, \beta)$. By an abuse of language, a quadratic algebra is said to be of type $(\alpha, \beta)$ when it has a basis of type $(\alpha, \beta)$.

#### Proposition 1 {#alg-iii-s2-prop-1 .statement}

*A quadratic algebra E is associative and commutative.*

The fact that E is commutative follows from the equation $e_1 e_2 = e_2 e_1$ in (2); similarly, to verify associativity, it suffices to see that $x(yz) = (xy)z$ when $x, y, z$ are each equal to $e_1$ or $e_2$. Now, this relation is obvious if at least one of the elements $x, y, z$ is equal to $e_1$; it is also true for $x = y = z = e_2$ since E is commutative; whence the proposition.

Let $e$ denote the unit element of a quadratic algebra E and let $(e, i)$ be a basis of E of type $(\alpha, \beta)$; every other basis of E containing $e$ is therefore of the form $(e, j)$ with $j = \gamma e + \delta i$ (II, § 7, no. 2, Corollary to Proposition 3); moreover, for $(e, j)$ to be a basis of E, it is necessary and sufficient that $\delta$ be invertible in A; the condition is obviously sufficient; conversely, if $\bar{i}$ is the canonical image of $i$ in $E/Ae$, $\bar{i}$ and $\bar{j} = \delta \bar{i}$ must each form a basis of $E/Ae$, whence the necessity of the condition. Then

$$
j^2 = (\gamma^2 + \alpha \delta^2)e + (2\gamma \delta + \beta \delta^2)i = (\alpha \delta^2 - \gamma^2 - \beta \gamma \delta)e + (2\gamma + \beta \delta)j;
$$

thus it is seen that E is of type

$$
(\alpha \delta^2 - \gamma^2 - \beta \gamma \delta, 2\gamma + \beta \delta)
$$

for all invertible $\delta \in A$ and all $\gamma \in A$. In particular, if $E$ is of type $(\alpha, 2\beta')$, $i$ is also of type $(\alpha + {\beta'}^2, 0)$ as is seen by taking $\gamma = -\beta'$ and $\delta = 1$.

#### Proposition 2 {#alg-iii-s2-prop-2 .statement}

*Let $E$ be a quadratic $A$-algebra and $e$ its unit element. For all $u \in E$, let $T(u)$ be the trace of the endomorphism $m_u : x \mapsto ux$ of the free $A$-module $E$ (II, § 4, no. 3). Then the mapping $s$ defined by $s(u) = T(u).e - u$ is an automorphism of the algebra $E$ and $s^2(u) = u$ for all $u \in E$.*

Let $(e, i)$ be a basis of $E$ of type $(\alpha, \beta)$; then $T(e) = 2$, when $s(e) = e$, and $T(i) = \beta$, whence $s(i) = \beta e - i$. Hence $(e, s(i))$ is a basis of $E$, whose type is given by (3) with $\gamma = \beta$ and $\delta = -1$, which again gives $(\alpha, \beta)$; it follows that $s$ is an automorphism of the algebra $E$. As $m_{s(u)} = s m_u s^{-1}$, the endomorphisms $m_u$ and $m_{s(u)}$ of the $A$-module $E$ have the same trace (II, § 4, no. 3, Proposition 3), whence

$$
s^2(u) = T(u).e - s(u) = T(u).e - (T(u).e - u) = u
$$

for all $u \in E$.

The automorphism $s$ is called *conjugation* of the $A$-algebra $E$ and $s(u)$ the *conjugate* of $u$.

If $u = \xi e + \eta i$, with $\xi, \eta$ in $A$, then $s(u) = (\xi + \beta \eta)e - \eta i$, whence

(4)
$$
T(u)e = u + s(u) = (2\xi + \beta \eta)e
$$
(5)
$$
u.s(u) = (\xi^2 + \beta \xi \eta - \alpha \eta^2)e = N(u)e
$$

where we have written $N(u) = \xi^2 + \beta \xi \eta - \alpha \eta^2$. The elements $T(u)$ and $N(u)$ (or, when $A$ and $Ae$ are canonically identified, the elements $T(u)e$ and $N(u)e$) are called respectively the *trace* and *norm* of $u$.

When $\beta = 0$, the above formulae are simplified to

(6)
$$
s(\xi e + \eta i) = \xi e - \eta i, \quad T(\xi e + \eta i) = 2\xi, \quad N(\xi e + \eta i) = \xi^2 - \alpha \eta^2.
$$

Clearly $T$ is a *linear form* on $E$*and* $N$ is a *quadratic form* on $E$ (IX, § 3, no. 4)*. As $E$ is commutative and associative, it follows from (5) that

(7)
$$
N(uv) = N(u)N(v).
$$

For $u$ to be *invertible in* $E$, it is necessary and sufficient that $N(u)$ be *invertible in* $A$. For, as $N(e) = 1$, the necessity of the condition follows from (7), writing $v = u^{-1}$. Conversely, if $N(u)$ is invertible in $A$, it follows from (5) that $u$ is invertible and that

(8)
$$
u^{-1} = (N(u))^{-1}s(u).
$$

*It can be proved that $N(u)$ is the determinant (§ 8, no. 1) of the endomorphism $m_u$ (cf. § 9 no. 3, Example 1).*

The following proposition gives the structure of quadratic algebras over a commutative field:

#### Proposition 3 {#alg-iii-s2-prop-3 .statement}

*Let E be a quadratic A-algebra of type* $(\alpha, \beta)$.

(i) *If A is a field and contains no element* $\zeta$ *such that* $\zeta^2 = \alpha + \beta \zeta$, *E is a (commutative) field* (cf. V, § 3).

(ii) *If the ring* A *contains an element* $\zeta$ *such that* $\zeta^2 = \alpha + \beta \zeta$ *and* $\beta - 2\zeta$ *is invertible* (resp. zero), *E is isomorphic to* A $\times$ A *resp. is of type* $(0, 0))$.

We prove (i). Let $\xi, \eta$ be two elements of A and $u = \xi e + \eta i$. If $\eta \neq 0$ and we write $\theta = -\xi \eta^{-1}$, then $\mathrm{N}(u) = \eta^2 (\theta^2 - \beta \theta - \alpha)$ by (5), whence $\mathrm{N}(u) \neq 0$ by virtue of the hypothesis on A; if $\eta = 0$, then $\mathrm{N}(u) = \xi^2$. In any case, if $u \neq 0$, then $\mathrm{N}(u) \neq 0$, hence $\mathrm{N}(u)$ is invertible in A and therefore $u$ is invertible in E.

We now prove (ii). The canonical basis $(e_1, e_2)$ of the algebra A $\times$ A is of type $(0, 1)$. We have seen (formula (3)) that E is of type

$$
(\alpha \delta^2 - \gamma^2 - \beta \gamma \delta, 2\gamma + \beta \delta)
$$

for all $\gamma \in A$ and all $\delta$ invertible in A. If $\beta - 2\zeta$ is invertible, take $\delta = (\beta - 2\zeta)^{-1}$ and $\gamma = -\zeta (\beta - 2\zeta)^{-1}$; then $2\gamma + \beta \delta = 1$ and

$$
\alpha \delta^2 - \gamma^2 - \beta \gamma \delta = \delta^2 (\alpha - \zeta^2 + \beta \zeta) = 0;
$$

thus E is of type $(0, 1)$ and hence isomorphic to A $\times$ A. If $\beta - 2\zeta = 0$, it has already been remarked that E is of type $(\alpha + \zeta^2, 0)$ and hence of type $(0, 0)$ since $\alpha + \zeta^2 = 2\zeta^2 - \beta \zeta = 0$.

A quadratic A-algebra of type $(0, 0)$ is also called an *algebra of dual numbers* over A.

### 4. CAYLEY ALGEBRAS

#### Definition 1 {#alg-iii-s2-def-1 .statement}

*A Cayley algebra over* A *is an ordered pair* (E, s), *where* E *is an algebra over* A *with a unit element* e *and* s *is an antiautomorphism of* E *such that*

$$
u + s(u) \in Ae \quad \text{and} \quad u.s(u) \in Ae
$$

*for all* $u \in E$.

$s$ is called the *conjugation* of the Cayley algebra (E, s) and $s(u)$ the *conjugate* of $u$. The condition $u + s(u) \in Ae$ implies that $u$ and $s(u)$ are *permutable*. We write

(9) $$
T(u) = u + s(u)
$$
(10) $$
N(u) = u.s(u) = s(u).u
$$

and these elements of the subalgebra $Ae$ are called respectively the *Cayley trace* and *norm* of $u$.

The ordered pair consisting of a quadratic algebra E and its conjugation s (which is an antiautomorphism since E is commutative) (no. 3) is a Cayley algebra.

Let (E, s) be a Cayley algebra; as $s(e) = e,\ s(u + s(u)) = u + s(u)$, in other words $s(u) + s^2(u) = u + s(u)$ or also

$$
s^2(u) = u
$$

so that $s^2$ is the identity mapping of E. It follows that

$$
T(s(u)) = T(u), \quad N(s(u)) = N(u).
$$

Finally, the relation $(u - u)(u - s(u)) = 0$ gives

$$
u^2 - T(u).u + N(u) = 0
$$

for all $u \in E$.

#### Proposition 4 {#alg-iii-s2-prop-4 .statement}

*Let E be an A-algebra and s and s' antiautomorphisms of E such that (E, s) and (E, s') are Cayley algebras. If E admits a basis containing the unit element e, then s' = s.*

Clearly $s'(u) = s(u) = u$ for all $u \in Ae$. If T, N (resp. T', N') are the trace and norm functions for (E, s) (resp. (E, s')), it follows from (13) that

$$
(T(u) - T'(u)).u - (N(u) - N'(u)) = 0.
$$

Let B be a basis of E containing e and u an element of B distinct from e; then $T(u) - T'(u) = 0$, whence $s(u) = s'(u)$. As s and s' coincide on B, they are equal.

In what follows, we shall write $\bar{u} = s(u)$, so that

$$
\left\{\begin{array}{lll}
u + \bar{u} = T(u), & u\bar{u} = \bar{u}u = N(u), & \bar{u} = u \\
u + v = \bar{u} + \bar{v}, & \alpha u = \alpha \bar{u}, & uv = \bar{v}.\bar{u}
\end{array}\right.
$$

for $u, v$ in E, $\alpha \in A$; moreover

$$
T(e) = 2e, \quad N(e) = e.
$$

From the formula

$$
T(uv) = uv + \overline{uv} = uv + \bar{v}.\bar{u} = uv + (T(v) - v)(T(u) - u),
$$

we deduce that

$$
uv + vu = T(u)v + T(v)u + (T(uv) - T(u)T(v))
$$

whence, exchanging $u$ and $v$,

$$
T(vu) = T(uv).
$$

On the other hand, $N(u + v) = (u + v)(\bar{u} + \bar{v}) = N(u) + N(v) + T(u\bar{v})$, whence

(18)
$$
T(v\bar{u}) = T(u\bar{v}) = N(u + v) - N(u) - N(v).
$$

Now, (16) applied with $u$ replaced by $\bar{u}$ gives
$$
T(u\bar{v}) = T(u)T(v) + \bar{u}v + v\bar{u} - T(u)v - T(v)\bar{u} = T(u)T(v) - uv - \bar{v}.\bar{u};
$$
whence

(19)
$$
T(v\bar{u}) = T(u\bar{v}) = N(u + v) - N(u) - N(v) = T(u)T(v) - T(uv).
$$

Finally, clearly for all $\alpha \in A$,

(20)
$$
N(\alpha u) = \alpha^2 N(u);
$$
in particular $N(2u) = 4N(u)$, so that formula (19) gives

(21)
$$
(T(u))^2 - T(u^2) = 2N(u).
$$

Clearly $T$ is a linear form on the $(Ae)$-module $E$. As $(u, v) \mapsto T(v\bar{u})$ is a bilinear form on this module, *it follows from (18) and (20) that $N$ is a quadratic form (cf. IX, § 3, no. 4).*

### 5. CONSTRUCTION OF CAYLEY ALGEBRAS. QUATERNIONS

Let $(E, s)$ be a Cayley algebra over $A$, for which we shall use the notation of no. 4, and let $\gamma \in A$. Let $F$ be the algebra over $A$ whose underlying module is $E \times E$ and whose multiplication is defined by

(22)
$$
(x, y)(x', y') = (xx' + \gamma \bar{y}'y, y\bar{x}' + y'x);
$$
clearly $(e, 0)$ is unit element of $F$ and $E \times \{0\}$ is a subalgebra of $F$ isomorphic to $E$; we shall *identify* it with $E$ in what follows, so that $x \in E$ is identified with $(x, 0)$ and in particular $e$ is identified with the unit element of $F$.

Let $t$ be the permutation of $F$ defined by

(23)
$$
t((x, y)) = (\bar{x}, -y) \quad (x \in E, y \in E).
$$

#### Proposition 5 {#alg-iii-s2-prop-5 .statement}

(i) *The ordered pair $(F, t)$ is a Cayley algebra over $A$*.

(ii) *Let $j = (0, e)$, so that $(x, y) = xe + yj$ for $x \in E, y \in E$. The Cayley trace and norm $T_F$ and $N_F$ of $F$ are given by the formulae*

(24)
$$
T_F(xe + yj) = T(x), \quad N_F(xe + yj) = N(x) - \gamma N(y).
$$

(iii) *For $F$ to be associative, it is necessary and sufficient that $E$ be associative and commutative.*

For $(x, y) \in \mathbf{F}$,

$$
(x, y) + t((x, y)) = (x + \overline{x}, 0) = T(x)e
$$
(25)
$$
(x, y)t((x, y)) = (x, y)(\overline{x}, -y) = (xx - \gamma \overline{y}y, y\overline{x} - yx)
= (\mathrm{N}(x) - \gamma \mathrm{N}(y), 0) = (\mathrm{N}(x) - \gamma \mathrm{N}(y))e.
$$
(26)

To prove both (i) and (ii), it therefore suffices to show that $t$ is an antiautomorphism of $\mathbf{F}$. Clearly $t$ is an A-linear bijection. On the other hand,
$$
t((x, y) \cdot (x', y')) = t((xx' + \gamma \overline{y}'y, y\overline{x}' + y'x)) = (\overline{x}'\overline{x} + \gamma \overline{y}y', -y\overline{x} - y'x)
= (\overline{x}', -y')(\overline{x}, -y) = t((x', y'))t((x, y))
$$
and hence $t$ is an antiautomorphism.

It remains to prove (iii). As E is identified with a subalgebra of F, E may be assumed to be associative. Let $u = (x, y)$, $u' = (x', y')$, $u'' = (x'', y'')$ be elements of F. Then
$$
\begin{cases}
(uu')u'' = ((xx' + \gamma \overline{y}'y)x'' + \gamma \overline{y}''(\overline{y}x' + y'x), \\
\phantom{(uu')u'' = } (y\overline{x}' + y'x)\overline{x}'' + y''(xx' + \gamma \overline{y}'y)) \\
u(u'u'') = (x(x'x'' + \gamma \overline{y}''y') + (\gamma(x''\overline{y}' + \overline{x}'\overline{y}'')y, \\
\phantom{u(u'u'') = } y(\overline{x}''\overline{x}' + \gamma \overline{y}'y'') + (y'\overline{x}'' + y''x')x).
\end{cases}
$$
(27)

Examining these formulae shows that the commutativity of E implies the associativity of F. Conversely, if F is associative, formulae (27) applied with $y = y' = 0$, $x'' = 0$ and $y'' = e$ give $(0, x'x) = (0, xx')$, that is $x'x = xx'$ for all $x, x'$ in E; thus E is then commutative.

Note also that, in the above notation, for $x, y$ in E,
$$
yj = j\overline{y}, \quad x(yj) = (yx)j, \quad (xj)y = (x\overline{y})j, \quad (xj)(yj) = \overline{y}xe
$$
(28)
$$
j^2 = e.
$$
(29)

The Cayley algebra $(\mathbf{F}, t)$ is called the *Cayley extension of* $(\mathbf{E}, s)$ *defined by* $\gamma$.

#### Example {#alg-iii-s2-n5-exa-1 .statement}

(1) If we take $\mathbf{E} = \mathbf{A}$ (and hence $s = 1_A$), the algebra $\mathbf{F}$ is a *quadratic A-algebra* with basis $(e, j)$ where $j^2 = \gamma e$.

(2) Take E to be a *quadratic algebra of type* $(\alpha, \beta)$, so that the underlying module of E is $\mathbf{A}^2$, with multiplication table (2) (no. 3) for the canonical basis. Take s to be conjugation of E (no. 3, Proposition 2). Then, for all $\gamma \in \mathbf{A}$, the Cayley extension F of $(\mathbf{E}, s)$ defined by $\gamma$ is called the *quaternion algebra of type* $(\alpha, \beta, \gamma)$, which is *associative* by no. 3, Proposition 1 and Proposition 5 above; its underlying module is $\mathbf{A}^4$ and, if $(e, i, j, k)$ denotes the canonical basis of $\mathbf{A}^4$, the corresponding multiplication table is given by
$$
\left\{\begin{array}{lll}
i^2 = \alpha e + \beta i, & ij = k, & ik = \alpha j + \beta k, \\
ji = \beta j - k, & j^2 = \gamma e, & jk = \beta \gamma e - \gamma i, \\
ki = -\alpha j, & kj = \gamma i, & k^2 = -\alpha \gamma e.
\end{array}\right.
$$
(30)

Further, for $u = \rho e + \xi i + \eta j + \zeta k$ (with $\rho, \xi, \eta, \zeta$ in $\mathbf{A}$), we have (writing $\bar{u}$ instead of $t(u)$ and identifying $\mathbf{A}$ with $\mathbf{Ae}$):

$$
\left\{
\begin{array}{l}
u = (\rho + \beta \xi)e - \xi i - \eta j - \zeta k \\
T_F(u) = 2\rho + \beta \xi \\
N_F(u) = \rho^2 + \beta \rho \xi - \alpha \xi^2 - \gamma (\eta^2 + \beta \eta \zeta - \alpha \zeta^2).
\end{array}
\right.
$$

Formulae (30) follow from (28) and (29) and formulae (31) from (23) and (24), taking account of the formulae for the quadratic algebra E.

Then, for $u, v$ in F,

$$
N_F(uv) = N_F(u)N_F(v)
$$

for $N_F(uv) = uv.\overline{uv} = uv(\overline{v}.\overline{u}) = u(v\overline{v})\overline{u} = (u\overline{u})(v\overline{v})$ by virtue of the associativity and the fact that $N_F(u)$ belongs to the centre of F.

An A-algebra isomorphic to a quaternion algebra is also called a *quaternion algebra*; if a basis of such an algebra has multiplication table (30), it is called a *basis of type* $(\alpha, \beta, \gamma)$. By an abuse of language, a quaternion algebra is said to be *of type* $(\alpha, \beta, \gamma)$ when it has a basis of type $(\alpha, \beta, \gamma)$.

When $\beta = 0$, formulae (30) and (31) simplify to

$$
\left\{
\begin{array}{lll}
i^2 = \alpha e, & ij = k, & ik = \alpha j, \\
ji = -k, & j^2 = \gamma e, & jk = -\gamma i, \\
ki = -\alpha i, & kj = \gamma i, & k^2 = -\alpha \gamma e,
\end{array}
\right.
$$

and

$$
\left\{
\begin{array}{l}
\bar{u} = \rho e - \xi i - \eta j - \zeta k \\
T_F(u) = 2\rho \\
N_F(u) = \rho^2 - \alpha \xi^2 - \gamma \eta^2 + \alpha \gamma \zeta^2.
\end{array}
\right.
$$

Then $(\alpha, \beta, \gamma)$ is replaced throughout by $(\alpha, \gamma)$ in the above expressions. It is immediate that the quaternion algebras of types $(\alpha, \gamma)$ and $(\gamma, \alpha)$ are *isomorphic*.

Note that formulae (32) show that F is not commutative when $-1 \neq 1$ in $\mathbf{A}$.

*Taking A to be the field $\mathbf{R}$ of real numbers and $\alpha = \gamma = -1, \beta = 0$, the corresponding algebra F is called the *algebra of Hamiltonian quaternions* and is denoted by $\mathbf{H}$. If $u = \rho e + \xi i + \eta j + \zeta k$ ($\rho, \xi, \eta, \zeta$ in $\mathbf{R}$) is an element $\neq 0$ in $\mathbf{H}$, the formula $u\bar{u} = \bar{u}u = \rho^2 + \xi^2 + \eta^2 + \zeta^2$ (cf. (34)) shows that $N(u) \neq 0$ in $\mathbf{R}$, so that $u$ admits an *inverse* $u^{-1} = N(u)^{-1}\bar{u}$ in $\mathbf{H}$ and that $\mathbf{H}$ is therefore a *non-commutative field*.

(3) If E is taken to be a quaternion algebra (cf. *Example 2*), the Cayley extension of E defined by an element $\delta \in \mathbf{A}$ is in general non-associative

(Proposition 5); it is called an octonion algebra over A (cf. Appendix, no. 3).

### 6. ALGEBRA OF A MAGMA, A MONOID, A GROUP

Recall that a magma is a set with a law of composition (I, § 1, no. 1). Let S be a magma written multiplicatively and let E = A^{(S)} be the A-module of formal linear combinations of elements of S (II, § 1, no. 11); we know that a canonical mapping s \mapsto e_s is defined of S into A^{(S)} such that the family (e_s)_{s \in S} is a basis (called canonical) of A^{(S)}, every element of A^{(S)} being then written uniquely in the form $\sum_{s \in S} \alpha_s e_s$, where (\alpha_s) is a family of elements of A of finite support. Then an A-algebra structure is defined on E by taking as multiplication table of the canonical basis

$$
e_s e_t = e_{st}.
$$

The algebra E thus defined is called the algebra of the magma S over A. If $x = \sum_{s \in S} \xi_s e_s$ and $y = \sum_{s \in S} \eta_s e_s$ are two elements of E, then

$$
xy = \sum_{s \in S} \left( \sum_{tu = s} \xi_t \eta_u \right) e_s.
$$

When S is a monoid (resp. group), E is called the algebra of the monoid (resp. group) S over A; it is then an associative algebra (§ 1, no. 7); similarly, when S is a commutative monoid, its algebra is associative and commutative. Finally if the magma S admits an identity element u, $e_u$ is unit element of the algebra E; as the element $e_u$ is free, A is then identified with the sub-algebra Ae_u of E.

When A \neq \{0\}, S is sometimes identified with its image under the injection s \mapsto e_s, so that an element of E is written as $\sum_{s \in S} \alpha_s s$; but this identification is not possible (without causing confusion) when S is written additively. Then $e^s$ is also often written instead of $e_s$.

Let B be another commutative ring and $\rho : A \to B$ a ring homomorphism; consider the algebras E = A^{(S)} and E' = B^{(S)} of the same magma S over A and B and let $(e_s)_{s \in S}$ and $(e'_s)_{s \in S}$ be their respective canonical bases. The algebra B^{(S)} is canonically identified, under the A-linear mapping j such that $j(e_s \otimes 1) = e'_s$ for all $s \in S$, with the algebra A^{(S)} \otimes_A B obtained from A^{(S)} by extending the ring of scalars to B (II, § 1, no. 11, Corollary 3 to Proposition 17).

#### Proposition 6 {#alg-iii-s2-prop-6 .statement}

*Let S be a magma, F an A-algebra and f a homomorphism of*

S into F with only its multiplicative structure. Then there exists one and only one A-algebra homomorphism $\bar{f}: A^{(S)} \to F$ rendering commutative the diagram

$$
\begin{array}{ccc}
S & \xrightarrow{f} & F \\
| & & | \\
A^{(S)} & \xrightarrow{\bar{f}} & F
\end{array}
$$

(where the vertical arrow on the left is the canonical mapping $s \mapsto e_s$).

Let $\bar{f}: A^{(S)} \to F$ be the unique A-module homomorphism such that $\bar{f}(e_s) = \bar{f}(s)$ (II, § 1, no. 11, Corollary 3 to Proposition 17); it suffices to verify that $\bar{f}$ is an algebra homomorphism and for this it suffices to prove that $\bar{f}(e_s e_t) = \bar{f}(e_s) \bar{f}(e_t)$, which follows immediately from the definition and the hypothesis $f(st) = f(s)f(t)$.

Proposition 6 expresses the fact that the ordered pair consisting of $A^{(S)}$ and the canonical mapping $s \mapsto e_s$ is a solution of the universal mapping problem (Set Theory, IV, § 3, no. 1) where $\Sigma$ is the species of A-algebra structure and the $\alpha$-mappings the homomorphisms of S into an A-algebra with only its multiplicative law.

#### Corollary {#alg-iii-s2-n6-cor-1 .statement}

Let S, S' be two magmas and $g: S \to S'$ a homomorphism. Then there exists one and only one A-algebra homomorphism $u: A^{(S)} \to A^{(S')}$ rendering commutative the diagram

$$
\begin{array}{ccc}
S & \xrightarrow{g} & S' \\
| & & | \\
A^{(S)} & \xrightarrow{u} & A^{(S')}
\end{array}
$$

(where the vertical arrows are the canonical mappings).

It suffices to apply Proposition 6 taking $f$ to be the composite mapping $S \xrightarrow{g} S' \to A^{(S')}$.

In particular, if T is a stable subset of the magma S (I, § 1, no. 4), the set of elements $\sum_{s \in T} \alpha_s e_s$ of $A^{(S)}$ is a subalgebra of $A^{(S)}$ canonically isomorphic to the algebra $A^{(T)}$ and sometimes identified with the latter.

#### Example {#alg-iii-s2-n6-exa-1 .statement}

Let V be an A-module and S a monoid which operates on V on the left; this means (I, § 5, no. 1) that there is given a mapping $(s, x) \mapsto s.x$ of S into V such that $s.(x + y) = s.x + s.y, s.(\alpha x) = \alpha(s.x)$ and $s.(t.x) = (st).x$ for $s, t$ in S, $x, y$ in V and $\alpha \in A$ and, denoting by e the identity element of S, e.x = x for x ∈ V. Writing f(s)(x) = s.x, f is a homomorphism of S into the algebra End_A(V) (with only its multiplicative law), mapping the identity element e to the unit element l_V. Applying Proposition 6, an A-algebra homomorphism $\bar{f}: A^{(S)} \to \mathrm{End}_A(V)$ is obtained, which gives the underlying group of V a left module structure over $A^{(S)}$.

This allows us to reduce the study of commutative groups with operators to that of modules. For let M be a commutative group with operators written additively, all of whose external laws are written multiplicatively. Let $\Omega$ be the sum set (Set Theory, II, § 4, no. 8) of the domains of operators of the various external laws on M, each of these domains being canonically identified with a subset of $\Omega$. Let Mo($\Omega$) be the free monoid (I § 7, no. 2) constructed on $\Omega$; a law of action

$$
(s, x) \mapsto s.x
$$

is defined on M with Mo($\Omega$) as domain of operators, by induction on the length of the word s in Mo($\Omega$); if s is of length 0, it is the empty word e and we write $e.x = x$ for all $x \in M$. If x is of length $n \geq 1$, it can be written uniquely as $s = tu$, where u is of length $n - 1$ and t of length 1, so that $t \in \Omega$; we then write $s.x = t.(u.x)$. For any two words s, $s'$ in Mo($\Omega$), the relation $s.(s'.x) = (ss').x$ is verified by induction on the length of s.

Then applying the method described above, a left $\mathbf{Z}^{(Mo(\Omega))}$-module structure is obtained on M and it is verified without difficulty that the usual notions in the theory of groups with operators (stable subgroups, homomorphisms) are the same for commutative groups with operators and the modules thus associated with them.

### 7. FREE ALGEBRAS

#### Definition 2 {#alg-iii-s2-def-2 .statement}

*Let I be a set; let M(I) (resp. Mo(I), resp. $\mathbf{N}^{(I)}$) denote the free magma (resp. free monoid, resp. free commutative monoid) derived from I. The algebra of M(I) (resp. Mo(I), resp. $\mathbf{N}^{(I)}$) over A is called the free algebra (resp. free associative algebra, resp. free commutative associative algebra (or, by an abuse of language, free commutative algebra)) of the set I over the ring A.*

We shall denote the free algebra (resp. free associative algebra, resp. free commutative algebra) of I over A by Lib_A(I) (resp. Libas_A(I), resp. Libasc_A(I)). By composing the canonical mapping of I into M(I) (resp. Mo(I), resp. $\mathbf{N}^{(I)}$) with the canonical mapping of M(I) (resp. Mo(I), resp. $\mathbf{N}^{(I)}$) into Lib_A(I) (resp. Libas_A(I), resp. Libasc_A(I)), a canonical mapping is obtained of I into Lib_A(I) (resp. Libas_A(I), resp. Libasc_A(I)), which is injective if $A \neq \{0\}$. We shall denote the image of an element $i \in I$ under this canonical mapping by $X_i$ and we shall say that $X_i$ is the indeterminate of index i of Lib_A(I) (resp. Libas_A(I), resp. Libasc_A(I)).

As Mo(I) and $\mathbf{N}^{(I)}$ each have an identity element, Libas_A(I) and Libasc_A(I) are unital associative algebras and further Libasc_A(I) is commutative. If e is the unit element of Libas_A(I) (resp. Libasc_A(I)), the mapping $\alpha \mapsto \alpha e$ is an isomorphism of A onto a subring of the centre of Libas_A(I) (resp. Libasc_A(I)), which is identified with A (no. 1).

#### Proposition 7 {#alg-iii-s2-prop-7 .statement}

*Let I be a set and F an algebra (resp. unital associative algebra, resp. unital commutative associative algebra) over A. For every mapping $f : I \to F$, there exists one and only one homomorphism (resp. unital homomorphism) $\bar{f}$ of Lib_A(I) (resp. Libas_A(I), resp. Libasc_A(I)) into F such that $\bar{f}(X_i) = f(i)$ for all $i \in I$.*

Let $F_m$ be the magma (resp. monoid) obtained by giving the set F its multiplicative law of composition. There is one and only one homomorphism (resp. unital homomorphism) $g$ of M(I) (resp. Mo(I), resp. $\mathbf{N}^{(I)}$) into $F_m$ such that $g(i) = f(i)$ for all $i \in I$ (I, § 7, nos. 1, 2 and 7); Proposition 7 then follows from no. 6, Proposition 6.

#### Remark {#alg-iii-s2-n7-rem-1 .statement}

(1) We shall later define an isomorphism of Libas_A(I) onto the tensor algebra of the free module $A^{(I)}$ (§ 5, no. 5) and also an isomorphism of Libasc_A(I) onto the symmetric algebra of $A^{(I)}$ (§ 6, no. 6).

(2) Let $\rho$ be a unital homomorphism of A into a commutative ring B. As has been seen (§ 2, no. 6), an isomorphism $\sigma$ is derived from $\rho$ of Lib_B(I) (resp. Libas_B(I), resp. Libasc_B(I)) onto the algebra $(\mathrm{Lib}_A(I))_{(B)}$ (resp. $(\mathrm{Libas}_A(I))_{(B)}$, resp. $(\mathrm{Libasc}_A(I))_{(B)}$) obtained by extending the scalars to B by means of $\rho$; if $X_i^A, X_i^B$ are the indeterminates of index $i$ corresponding respectively to A and B, then $\sigma(X_i^B) = X_i^A \otimes 1$.

(3) Let J be a subset of I; we know that M(J) is identified with a stable subset of the magma M(I) and hence (no. 6) Lib_A(J) is canonically identified with a subalgebra of Lib_A(I), generated by the $X_i$ such that $i \in J$; it is said that only the indeterminates of indices belonging to J occur in an element of Lib_A(J). The definition given in no. 6 of the algebra of a magma shows that Lib_A(I) is the union of the directed family of subalgebras Lib_A(J) when J runs through the set of *finite* subsets of I. There are analogous results for Libas_A(I) and Libasc_A(I).

(4) With element s of M(I) (resp. Mo(I), resp. $\mathbf{N}^{(I)}$) is associated its *length* $l(s)$, which is an integer $\geqslant 1$ (resp. $\geqslant 0$) such that $l(ss') = l(s) + l(s')$ (I, § 7, nos. 1, 2 and 7). If $e_s$ is the element of Lib_A(I) (resp. Libas_A(I), resp. Libasc_A(I)) corresponding to s, the *total degree* (or simply the *degree* of an element $x = \sum_s \alpha_s e_s \neq 0$ of Lib_A(I) (resp. Libas_A(A), resp. Libasc_A(I)) is the greatest of the numbers $l(s)$ when s runs through the (non-empty by hypothesis) set of elements such that $\alpha_s \neq 0$. For example, if $i, j, k$ are three distinct elements of I, the element $(X_i(X_jX_k))X_i - (X_iX_j)(X_kX_i)$ is an element $\neq 0$ of total degree 4 in Lib_A(I).

### 8. DEFINITION OF AN ALGEBRA BY GENERATORS AND RELATIONS

Let F be an algebra over A and $(x_i)_{i \in I}$ a family of elements of F. By no. 7, Proposition 7, there exists a unique homomorphism $f : \mathrm{Lib}_A(I) \to F$ such that $f(X_i) = x_i$ for all $i \in I$. For $f$ to be surjective, it is necessary and sufficient that $(x_i)_{i \in I}$ be a generating system of F.

If $U \in \mathrm{Lib}_A(I)$, $f(U)$ is called the *element of F derived from U by substituting the elements $x_i$ for the indeterminates $X_i$*, or also the *value* of U for the values $x_i$ of the indeterminates $X_i$; it is usually denoted by $U((x_i)_{i \in I})$; in particular $U((X_i)_{i \in I}) = U$. If $\lambda$ is a homomorphism of F into an algebra $F'$ over A, then
$$
\lambda(U((x_i)_{i \in I})) = U((\lambda(x_i))_{i \in I}).
$$

Consider in particular the case where $F = \mathrm{Lib}_A(J)$, where J is another set; for every family $(H_i)_{i \in I}$ of elements of $\mathrm{Lib}_A(J)$ and every family $(y_j')_{j \in J}$ of elements of an A-algebra $F'$,
$$
U((H_i)_{i \in I}))((y_j')_{j \in J}) = U((H_i((y_j')_{j \in J})))_{i \in I}).
$$
(37)

In the above notation, every element U of $\mathrm{Lib}_A(I)$ such that $U((x_i)_{i \in I}) = 0$, or also such that $f(U) = 0$, is called a *relator* of the family $(x_i)_{i \in I}$ in F. The two-sided ideal $\mathrm{Ker}(f)$ consisting of these elements is called the *ideal of relators* of $(x_i)$.

Let $(R_j)_{j \in J}$ be a family of elements of $\mathrm{Lib}_A(I)$. $((x_i)_{i \in I}, (R_j)_{j \in J})$ is called a *presentation* of the algebra F if $(x_i)_{i \in I}$ is a generating system of F and the two-sided ideal of $\mathrm{Lib}_A(I)$ generated by the $R_j$ is equal to the ideal of relators of the family $(x_i)_{i \in I}$; the $x_i$ are called the *generators* and the $R_j$ the *relators* of the presentation.

Consider now any set I and a family $(R_j)_{j \in J}$ of elements of $\mathrm{Lib}_A(I)$. The quotient algebra E of $\mathrm{Lib}_A(I)$ by the two-sided ideal generated by the family $(R_j)$ is called the *universal algebra defined by the generating system I related by the family of relators* $(R_j)_{j \in J}$. Clearly, if $\overline{X}_i$ denotes the image of $X_i$ in E,
$$
((\overline{X}_i)_{i \in I}, (R_j)_{j \in J})
$$
is a *presentation* of E. Moreover, if $(x_i)_{i \in I}$ is a family of elements of an algebra F and $R_j((x_i)_{i \in I}) = 0$ for all $j \in J$, there exists a unique homomorphism $g : E \to F$ such that $g(\overline{X}_i) = x_i$ for all $i \in I$; for $((x_i)_{i \in I}, (R_j)_{j \in J})$ to be a presentation of F, it is necessary and sufficient that $g$ be *bijective*.

These remarks justify the following abuse of language: instead of saying "*$((x_i)_{i \in I}, (R_j)_{j \in J})$ is a presentation of F*", it is also said that "*F is the algebra generated by the generators $x_i$ subject to the relations $R_j((x_i)_{i \in I}) = 0$*". When the $R_j$ are of the form $P_j - Q_j$, it is also said that "*F is the algebra generated by the $x_i$ subject to the relations $P_j((x_i)) = Q_j((x_i))$*".

Let H be a set; we shall say that an element S of $\mathrm{Lib}_A(H)$ is a *universal* relator for an A-algebra F is $S((x_h)_{h \in H}) = 0$ for *every* family $(x_h)_{h \in H}$ of elements of F with H as indexing set.

#### Example {#alg-iii-s2-n8-exa-1 .statement}

(1) Take $H = \{1, 2, 3\}$; the algebras which admit
$$
(X_1 X_2) X_3 - X_1 (X_2 X_3)
$$
as universal relator are the associative algebras. The algebras which admit $X_1 X_2 - X_2 X_1$ as universal relator are the commutative algebras. *The algebras which admit the universal relators $X_1 X_1$ and
$$
(X_1 X_2) X_3 + (X_2 X_3) X_1 + (X_3 X_1) X_2
$$
as universal relator are the Lie algebras.*

Let I be a set; let a family $(S_k)_{k \in K}$ of elements of Lib_A(H) be given and consider the set T of elements of Lib_A(I) of the form $S_k((U_h))_{h \in H}$, where k runs through K and, for each k, $(U_h)_{h \in H}$ runs through the set of families of elements of Lib_A(I) with H as indexing set; consider a family $(R_j)_{j \in J}$ with T as set of elements. Then let F be the universal algebra defined by the generating system I related by the family $(R_j)_{j \in J}$ and let $u : \mathrm{Lib}_A(I) \to F$ be the canonical homomorphism, so that Ker(u) is generated by the elements $S_k((U_h)_{h \in H})$ for all $k \in K$ and all families $(U_h)_{h \in H}$ of elements of Lib_A(I); clearly each of the $S_k$ ($k \in K$) is a *universal relator* for F. Now let F' be an algebra admitting a generating system $(x_i)_{i \in I}$, for which each of the $S_k$ is a universal relator, and let $u' : \mathrm{Lib}_A(I) \to F'$ be the homomorphism such that $u'(X_i) = x_i$ for all $i \in I$; clearly Ker(u) $\subset$ Ker(u') and hence $u'$ can be written uniquely in the form $u' = h \circ u$, where $h : F \to F'$ is a homomorphism such that $h(\overline{X}_i) = x_i$ for all $i \in I$. For this reason F is called *the universal algebra defined by the generating system I*, *corresponding to the family of universal relators* $(S_k)_{k \in K}$. By an abuse of language, F is sometimes called the universal algebra generated by I and subject to the *identities* $S_k((u_h)) = 0$ for every family $(u_h)_{h \in H}$ of elements of F.

*Example* 2. Let L' be the universal algebra generated by I and subject to the identities $(uv)w - u(vw) = 0$ for every family of three elements of L' and let L'' be the algebra obtained by adjoining a unit element to L'; then there exists a unique unital isomorphism g of L'' onto Libas_A(I) such that $g(\overline{X}_i) = X_i$ for all $i \in I$. For clearly L'' is associative and the existence of the homomorphism g follows from the definition of L' and the remarks preceding it; but then clearly L'' satisfies the universal property (no. 7, Proposition 7) which characterizes Libas_A(I), whence the conclusion.

Considerations analogous to the above can be applied to associative algebras (resp. commutative associative algebras), taking account of the following remarks. When the context gives sufficient indication that the algebras considered are unital algebras, by an abuse of language, a family of elements $(x_i)_{i \in I}$ of an algebra $F$, such that the subalgebra generated by the $x_i$ ($i \in I$) and the unit element is equal to $F$, is often called a generating system of $F$. Then let $F$ be a unital associative algebra over $A$ and let $(x_i)_{i \in I}$ be a family of elements of $F$; by virtue of no. 7, Proposition 7, there exists a unique unital homomorphism $f : \mathrm{Libas}_A(I) \to F$ such that $f(X_i) = x_i$ for all $i \in I$; if $U \in \mathrm{Libas}_A(I)$, $f(U)$ is also called the element of $F$ derived from $U$ by substituting the elements $x_i$ for the indeterminates $X_i$ and it is also denoted by $U((x_i)_{i \in I})$. Then the notions of relator, presentation and universal relator go over immediately to associative algebras; it suffices simply to replace $\mathrm{Lib}_A(I)$ throughout by $\mathrm{Libas}_A(I)$. *The universal unital associative algebra defined by the generating system I related by the family of relators* $(R_j)_{j \in J}$ is the quotient algebra of $\mathrm{Libas}_A(I)$ by the two-sided ideal generated by the family $(R_j)$. The universal unital associative algebra generated by the generating system $I$, corresponding to a family of universal relators is defined similarly. We leave to the reader the task of stating the analogous definitions relative to commutative associative algebras with $\mathrm{Libasc}_A(I)$ substituted for $\mathrm{Libas}_A(I)$.

#### Example 3 {#alg-iii-s2-n8-exa-3 .statement}

Let $L'$ be the universal unital associative algebra generated by $I$ and subject to the identities $uv - vu = 0$ for every family of two elements of $L'$. It is seen, as in *Example 2*, that $L'$ is canonically isomorphic to $\mathrm{Libasc}_A(I)$.

### 9. POLYNOMIAL ALGEBRAS

Let $B$ be a unital *commutative* associative $A$-algebra and let $(x_i)_{i \in I}$ be a family of elements of $B$; the subalgebra of $B$ generated by the $x_i$ ($i \in I$) and the unit element is denoted by $A[(x_i)_{i \in I}]_B$ or simply $A[(x_i)_{i \in I}]$ when no confusion can arise. For every set $I$, the algebra $\mathrm{Libasc}_A(I)$ is therefore equal to $A[(X_i)_{i \in I}]$ (also denoted by $A[X_i]_{i \in I}$); the latter notation, which has the advantage of indicating the notation chosen to denote the indeterminates, is the one we shall generally use in the rest of this Treatise. The elements of $A[(X_i)_{i \in I}]$ are called *polynomials in the indeterminates* $X_i$ ($i \in I$) *with coefficients in* $A$; it is a convention that, when it is said "let $A[(X_i)_{i \in I}]$ be a polynomial algebra", the $X_i$ are always understood to be the indeterminates. For every subset $J$ of $I$, the use of the above notation amounts to identifying $\mathrm{Libasc}_A(J)$ with the algebra of $\mathrm{Libasc}_A(I)$ generated by the $X_i$ of index $i \in J$ and the unit element (cf. no. 7, *Remark (3)*). For $I = \{1, 2, \ldots, n\}$, we write $A[X_1, X_2, \ldots, X_n]$ instead of $A[(X_i)_{i \in I}]$.

If $I$ and $I'$ are two equipotent sets, the algebras $\mathrm{Libasc}_A(I)$ and $\mathrm{Libasc}_A(I')$ are isomorphic. $A[X]$ is often used to denote the polynomial algebra corresponding to an unspecified indexing set with *a single* element, $X$ denoting the unique indeterminate; similarly, $A[X, Y]$, $A[X, Y, Z]$, ... are used to denote the polynomial algebras corresponding to unspecified indexing sets with 2, 3, ... elements. Note that, by virtue of the conventions made above, $A[X]$ and $A[Y]$ are for example (distinct) subalgebras of $A[X, Y, Z]$ if $A \neq \{0\}$.

The elements
$$
X^\nu = \prod_{i \in I} X_i^{\nu(i)},
$$
where $\nu$ runs through $\mathbf{N}^{(I)}$ form a basis of the polynomial algebra $A[(X_i)_{i \in I}]$. These elements are called *monomials* in the indeterminates $X_i$ and the number $|\nu| = \sum_{i \in I} \nu(i)$ is called the *degree* (or *total degree*) of the monomial $X^\nu$. The unique monomial of degree 0 is the unit element of $A[(X_i)_{i \in I}]$; it is often identified with the unit element 1 of $A$. Every polynomial $u$ of $A[(X_i)_{i \in I}]$ can be written uniquely as
$$
u = \sum_{\nu \in \mathbf{N}^{(I)}} \alpha_\nu X^\nu
$$
with $\alpha_\nu \in A$; the elements $\alpha_\nu$, zero except for a finite number of indices $\nu \in \mathbf{N}^{(I)}$, are called the *coefficients* of $u$; the elements $\alpha_\nu X^\nu$ are called the *terms* of $u$ (the element $\alpha_\nu X^\nu$ often being called the "term in $X^\nu$"); in particular the term $\alpha_0 X^0$ (identified with $\alpha_0 \in A$) is called the *constant term* of $u$. If $J$ is a subset of $I$, $u$ belongs to $A[(X_i)_{i \in J}]$ if and only if $\alpha_\nu = 0$ for $\nu \notin \mathbf{N}^{(J)}$. It follows that $A[(X_i)_{i \in I}]$ is the union of the subalgebras $A[(X_i)_{i \in J}]$, where $J$ runs through the set of finite subsets of $I$. If $\alpha_\nu = 0$ for $|\nu| > n$, $u$ is said to be a *polynomial of degree* $\leq n$. When $\alpha_\nu = 0$, (by an abuse of language) $u$ is said to *contain no term in* $X^\nu$; in particular, when $\alpha_0 = 0$, $u$ is said to be a polynomial *with no constant term*.

For every *non-zero* polynomial $u = \sum \alpha_\nu X^\nu$, the *degree* (or *total degree*) of $u$ is the greatest of the integers $|\nu|$ of the multiindices $\nu$ such that $\alpha_\nu \neq 0$.

Let $F$ be a unital associative $A$-algebra and let $(x_i)_{i \in I}$ be a family of elements of $F$, which are *pairwise permutable*. The subalgebra $F'$ of $F$ generated by the $x_i$ and the unit element is commutative (§ 1, no. 7), which allows us to define substituting the $x_i$ for the $X_i$ in the polynomial $u \in A[(X_i)_{i \in I}]$ (although $F$ is not necessarily commutative): $u((x_i)_{i \in I})$ is an element of $F'$ and therefore of $F$ and $h: u \to u((x_i)_{i \in I})$ is a homomorphism of $A[(X_i)_{i \in I}]$ into $F$. The elements of the kernel of $h$ are the relators of the family $(x_i)$ in $A[(X_i)_{i \in I}]$, also called *polynomial relators* (with coefficients in $A$) between the $x_i$. The image of the homomorphism $h$ is the subalgebra $F'$, also denoted by $A[(x_i)_{i \in I}]$ (even when $F$ is not commutative); if $a$ is the ideal of polynomial relators between the $x_i$, then there is an exact sequence of $A$-modules
$$
0 \longrightarrow a \longrightarrow A[(X_i)_{i \in I}] \xrightarrow{h} A[(x_i)_{i \in I}] \longrightarrow 0.
$$

#### Proposition 8 {#alg-iii-s2-prop-8 .statement}

*Let $A[(X_i)_{i \in I}]$ be a polynomial algebra, $J$ a subset of $I$ and $K$ the complement of $J$ in $I$. Writing $A' = A[(X_j)_{j \in J}]$ and denoting by $X'_k$ ($k \in K$) the* indeterminates in the polynomial algebra Libasc_{A'}(K) = A'[(X'_k)_{k \in K}], there exists a unique ring isomorphism of A'[(X'_k)_{k \in K}] onto A[(X_i)_{i \in I}] which coincides with the identity on A' and maps X'_k to X_k for all k \in K.

Clearly A[(X_i)_{i \in I}] is an A'-algebra generated by the X_k for k \in K. On the other hand, as a polynomial relator between the X_k (k \in K) with coefficients in A' can be written uniquely as $\sum_v h_v((X_j)_{j \in J}) X^v$ where v runs through a finite subset of $\mathbf{N}^{(K)}$ and where the h_v are elements of A[(X_j)_{j \in J}], the h_v must be polynomial relators between the X_j with coefficients in A and hence are all zero, which proves the proposition.

The isomorphism described in Proposition 8 is often used to identify the elements of A[(X_i)_{i \in I}] with polynomials with coefficients in A' = A[(X_j)_{j \in J}]. If u is an element $\neq 0$ of A[(X_i)_{i \in I}], its total degree considered as an element of A'[(X_k)_{k \in K}] is also called its degree with respect to the X_i of index i \in K.

#### Remark {#alg-iii-s2-n9-rem-1 .statement}

Let I and J be two sets and (P_j)_{j \in J} a family of elements of $\mathbf{Z}[(X_i)_{i \in I}]$; if Q is an element of $\mathbf{Z}[(X_j)_{j \in J}]$ such that $Q((P_j)_{j \in J}) = 0$, then, for every family $(b_i)_{i \in I}$ of pairwise permutable elements of a ring B,
$$
Q((P_j((b_i)_{i \in I}))_{j \in J}) = 0.
$$
The relations which hold of the form $Q((P_j)_{j \in J}) = 0$ are sometimes called polynomial identities. For example
$$
(X_1 + X_2)^2 - X_1^2 - X_2^2 - 2X_1X_2 = 0
$$
with
$$
Q = Y_1^2 - Y_2, \quad P_1 = X_1 + X_2, \quad P_2 = X_1^2 + X_2^2 + 2X_1X_2
$$
$$
X_1^n - X_2^n - (X_1 - X_2)(X_1^{n-1} + X_1^{n-2}X_2 + \cdots + X_2^{n-1}) = 0
$$
with
$$
Q = Y_1 - Y_2Y_3, \quad P_1 = X_1^n - X_2^n, \quad P_2 = X_1 - X_2,
$$
$$
P_3 = X_1^{n-1} + X_1^{n-2}X_2 + \cdots + X_2^{n-1}
$$
are polynomial identities.

### 10. TOTAL ALGEBRA OF A MONOID

The algebra of a monoid S over A is (as an A-module) the submodule of the product $A^S$ consisting of the families $(\alpha_s)_{s \in S}$ of finite support; the multiplication in this algebra is defined by the relations $(\alpha_s)(\beta_s) = (\gamma_s)$, where, for all $s \in S$,
$$
\gamma_s = \sum_{tu = s} \alpha_t \beta_u
$$

(cf. no. 6, formula (35)). The sum on the right hand side of (38) is meaningful because $(\alpha_s)$ and $(\beta_s)$ are families of finite support and so therefore is the double family $(\alpha_t\beta_u)_{(t,u)\in S\times S}$. But the right hand side of (38) is also meaningful for *arbitrary* elements $(\alpha_s),\ \beta_s)$ of $A^S$ when the monoid $S$ satisfies the following condition:

(D) *For all* $s\in S$, *there exists only a finite number of ordered pairs* $(t,u)$ *in* $S\times S$ *such that* $tu=s$.

Suppose then that $S$ satisfies condition (D); a multiplication law can then be defined on the product A-module $A^S$ by formula (38). It is immediate that the multiplication thus defined on $A^S$ is A-bilinear; also it is *associative*, since, for $\alpha,\beta,\gamma$ in $A^S$,

$$
\sum_{uvw=t} \alpha_u\beta_v\gamma_w = \sum_{rw=t} \left( \left( \sum_{uv=r} \alpha_u\beta_v \right) \gamma_w \right) = \sum_{us=t} \left( \alpha_u \left( \sum_{vw=s} \beta_v\gamma_w \right) \right).
$$

This multiplication and the A-module structure on $A^S$ therefore define on $A^S$ a unital *associative algebra* structure over A; we shall say that the set $A^S$, with this structure, is the *total algebra* of the monoid S over A.

It is immediate that the *algebra* $A^{(S)}$ of the monoid S over A (also called the *restricted algebra* of S when necessary to avoid confusion) is a *subalgebra* of the total algebra of S over A (and is identical with the latter when S is finite). *By an abuse of language*, every element $(\xi_s)_{s\in S}$ of the total algebra of S over A is also denoted by the same notation $\sum_{s\in S} \xi_s e_s$ (or even $\sum_{s\in S} \xi_s s$) as the elements of the restricted algebra of S; of course the summation symbol appearing in this notation corresponds to no algebraic operation because it is taken over an *infinity* of terms $\neq 0$ in general. With this notation, multiplication in the total algebra of S is also given by formula (35) of no. 6.

If S is commutative, so is its total algebra $A^S$. If T is a submonoid of S, the total algebra $A^T$ of the monoid is canonically identified with a subalgebra of the total algebra of S. If $\rho : A \to B$ is a ring homomorphism, the canonical extension $\rho^S : A^S \to B^S$ is an A-homomorphism of the total algebra of S over A into the total algebra of S over B, which extends the canonical homomorphism $A^{(S)} \to B^{(S)}$.

### 11. FORMAL POWER SERIES OVER A COMMUTATIVE RING

For every set I, the additive monoid $N^{(I)}$ satisfies condition (D) of no. 10; for, if $s = (n_i)_{i\in I}$ with $n_i = 0$ except for the indices $i$ in a finite subset H of I, the relation $s = t + u$ with $t = (p_i)_{i\in I}$ and $u = (q_i)_{i\in I}$ is equivalent to $p_i + q_i = n_i$ for all $i$; but this implies $p_i = q_i = 0$ for $i \notin H$ and $p_i \leq n_i, q_i \leq n_i$ for $i \in H$; there are therefore $\prod_{i\in H} (n_i + 1)$ ordered pairs $(t, u)$ in $N^{(I)}$ such that $t + u = s$.

We can therefore consider the total algebra of the monoid $\mathbf{N}^{(I)}$ over $A$, which contains the (restricted) algebra $A[\mathbf{X}_i]_{i \in I}$ of this monoid. It is a unital commutative associative algebra called the algebra of formal power series in the indeterminates $X_i \ (i \in I)$ with coefficients in $A$ and denoted by $A[[\mathbf{X}_i]]_{i \in I}$; its elements are called formal power series in the indeterminates $X_i \ (i \in I)$ with coefficients in $A$. Such an element $(\alpha_v)_{v \in \mathbf{N}^{(I)}}$ is also denoted, following the convention made in no. 10, by $\sum_{v \in \mathbf{N}^{(I)}} \alpha_v X^v$; the $\alpha_v$ are the coefficients of the formal power series and the $\alpha_v X^v$ its terms; a polynomial in the $X_i$ is therefore a formal power series with only a finite number of terms $\neq 0$.

Clearly an algebra isomorphism $A[[\mathbf{X}_i]]_{i \in I_1} \to A[[\mathbf{X}_i]]_{i \in I_2}$ is canonically derived from every bijection $\sigma : I_1 \to I_2$ by mapping the formal power series $\sum_{(n_i)} \alpha_{(n_i)} \cdot \prod_{i \in I_1} X_i^{n_i}$ to the formal power series $\sum_{(n_i)} \alpha_{(n_i)} \cdot \prod_{i \in I_1} X_{\sigma(i)}^{n_i}$.

Let $J$ be a subset of $I$; the algebra $A[[\mathbf{X}_i]]_{i \in J}$ can be identified with a subalgebra of $A[[\mathbf{X}_i]]_{i \in I}$ consisting of the formal power series $\sum_{(n_i)} \alpha_{(n_i)} \cdot \prod_{i \in I} X_i^{n_i}$ where $\alpha_{(n_i)} = 0$ for every element $(n_i) \in \mathbf{N}^{(I)}$ such that $n_i \neq 0$ for at least one index $i \in I - J$. Further, if $K = I - J$, $A[[\mathbf{X}_i]]_{i \in I}$ is canonically identified with $(A[[\mathbf{X}_j]]_{j \in J})[[\mathbf{X}_k]]_{k \in K}$, by identifying the formal power series $\sum_{(n_i)} \alpha_{(n_i)} \cdot \prod_{i \in I} X_i^{n_i}$ with the formal power series $\sum_{(m_k)} \beta_{(m_k)} \cdot \prod_{k \in K} X_k^{m_k}$, where
$$
\beta_{(m_k)} = \sum_{(p_j)} \gamma_{(p_j)} \cdot \prod_{j \in J} X_j^{p_j}
$$
with $\gamma_{(p_j)} = \alpha_{(n_i)}$ for the sequence $(n_i)$ such that $n_i = p_i$ for $i \in J$ and $n_i = m_i$ for $i \in K$.

Given a formal power series $u = \sum_v \alpha_v X^v$, the terms $\alpha_v X^v$ such that $|v| = p$ are called the terms in $u$ of total degree $p$. The formal power series $u_p$ whose terms of total degree $p$ are those of $u$ and whose other terms are zero, is called the homogenous part of $u$ of degree $p$; when $I$ is finite, $u_p$ is a polynomial for all $p$; $u_0$ is identified with an element of $A$ (also called the constant term of $u$). If $u$ and $v$ are two formal power series and $w = uv$, then
$$
w_p = \sum_{r=0}^p u_r v_{p-r}
$$
for every integer $p \geq 0$.

For every formal power series $u \neq 0$, the least integer $p \geq 0$ such that $u_p \neq 0$ is called the total order (or simply the order) of $u$. If this order is denoted by $\omega(u)$ and $u$ and $v$ are two formal power series $\neq 0$, then
$$
\omega(u + v) \geq \inf(\omega(u), \omega(v)) \quad \text{if } u + v \neq 0 \\
\omega(uv) \geq \omega(u) + \omega(v) \quad \text{if } uv \neq 0.
$$

Further, if $\omega(u) \neq \omega(v)$, then necessarily $u + v \neq 0$ and the two sides of (40) are equal.

Note that the order of 0 *is not defined*. By an abuse of language, it is a convention to say that "f is a formal power series of order $\geq p$ (resp. $> p$)" if the homogeneous part of f of degree n is zero for all $n < p$ (resp. $n \leq p$); 0 is therefore a "formal power series of order $> p$" for *every* integer $p \geq 0$.

Let J be a subset of I and let $A[[X_i]]_{i \in I}$ be identified as above with $B[[X_k]]_{k \in K}$, where $K = I - J$ and $B = A[[X_j]]_{j \in J}$; corresponding to the above definitions applied to $B[[X_k]]_{k \in K}$ there are new definitions for the formal power series $u \in A[[X_i]]_{i \in I}$; a term $\alpha_{(n_i)} \cdot \prod_{i \in I} X_i^{n_i}$ is said to be *of degree p in the $X_i$ of index* $i \in K$ if $\sum_{i \in K} n_i = p$ and the formal power series of $B[[X_k]]_{k \in K}$ with the same terms of degree $p$ as $u$ and the others zero is *called the homogenous part of degree p in the $X_i$ of index* $i \in K$. If $u \neq 0$, the *order* $\omega_K(u)$ with respect to the $X_i$ of index $i \in K$ is the smallest of the integers $p \geq 0$ such that the homogeneous part of $u$ of degree $p$ in the $X_i$ of index $i \in K$ is $\neq 0$. Inequalities (40) and (41) still hold when $\omega$ is replaced by $\omega_K$.

### Exercises {#alg-iii-s2-exercises}

See the [exercises for § 2](exercises/s2/).
