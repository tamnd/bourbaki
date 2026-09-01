---
book: fvr
book_title: Functions of a Real Variable
chapter: IV
chapter_title: DIFFERENTIAL EQUATIONS
section: 2
section_title: LINEAR DIFFERENTIAL EQUATIONS
lang: en
source: fvr-i-vii
book_pages: 177-198, 204-206
pdf_pages: 0192-0213, 0219-0221
extraction: ocr
subsections:
    - "no": 1
      title: EXISTENCE OF INTEGRALS OF A LINEAR DIFFERENTIAL EQUATION
      page: 177
      pdf_page: 192
    - "no": 2
      title: LINEARITY OF THE INTEGRALS OF A LINEAR DIFFERENTIAL EQUATION
      page: 179
      pdf_page: 194
    - "no": 3
      title: INTEGRATING THE INHOMOGENEOUS LINEAR EQUATION
      page: 182
      pdf_page: 197
    - "no": 4
      title: FUNDAMENTAL SYSTEMS OF INTEGRALS OF A LINEAR SYSTEM OF SCALAR DIFFERENTIAL EQUATIONS
      page: 183
      pdf_page: 198
    - "no": 5
      title: ADJOINT EQUATION
      page: 186
      pdf_page: 201
    - "no": 6
      title: LINEAR DIFFERENTIAL EQUATIONS WITH CONSTANT COEFFICIENTS
      page: 188
      pdf_page: 203
    - "no": 7
      title: LINEAR EQUATIONS OF ORDER $n$
      page: 192
      pdf_page: 207
    - "no": 8
      title: LINEAR EQUATIONS OF ORDER $n$ WITH CONSTANT COEFFICIENTS
      page: 194
      pdf_page: 209
    - "no": 9
      title: SYSTEMS OF LINEAR EQUATIONS WITH CONSTANT COEFFICIENTS
      page: 196
      pdf_page: 211
statements: 25
exercises: 10
content_sha256: ed9860cc26b65ff84c11e78ae048f5030e2943903c24c951c87f27907207fd41
---

## § 2. LINEAR DIFFERENTIAL EQUATIONS

### 1. EXISTENCE OF INTEGRALS OF A LINEAR DIFFERENTIAL EQUATION

Let E be a complete normed space over the field $\mathbf{R}$, and J an interval in $\mathbf{R}$, not reducing to a point. One says that the differential equation

$$
\frac{d\mathbf{x}}{dt} = \mathbf{f}(t, \mathbf{x})
$$

(1) where $f$ is defined on $J \times E$, is a *linear* equation if, for every $t \in J$, the map $x \mapsto f(t, x)$ is a *continuous affine linear map* $^1$ from $E$ into itself; if one puts $b(t) = f(t, 0)$ the map $x \mapsto f(t, x) - f(t, 0) = f(t, x) - b(t)$ is then a continuous linear map from $E$ to itself; from now on we shall denote this map by $A(t)$ and write $A(t).x$, (or simply $A(t)x$) for its value at the point $x \in E$; thus the linear differential equation (1) may be written

$$
\frac{dx}{dt} = A(t).x + b(t)
$$

(2)

where $b$ is a map from $J$ into $E$; when $b = 0$ one says that the linear differential equation (2) is *homogeneous*.

#### Example 1 {#fvr-iv-s2-n1-exa-1 .statement}

When $E$ is of finite dimension $n$ over $\mathbf{R}$ one can identify the endomorphism $A(t)$ with its *matrix* $\left(a_{ij}(t)\right)$ *with respect to any basis of* $E$ (*Alg.*, II, p. 343); when one identifies a vector $x \in E$ with the column matrix $(x_j)$ of its components with respect to the basis of $E$ under consideration the expression $A(t).x$ conforms to the general conventions of Algebra (*Alg.*, II, p. 343, prop 2). In this case, equation (2) is equivalent to the system of scalar differential equations

$$
\frac{dx_i}{dt} = \sum_{j=1}^n a_{ij}(t)x_j + b_i(t) \qquad (1 \leq i \leq n).
$$

(3)

#### Example 2 {#fvr-iv-s2-n1-exa-2 .statement}

Let $G$ be a *complete normed algebra* over $\mathbf{R}$, and $a(t)$, $b(t)$ and $c(t)$ three maps from $J$ into $G$; the equation

$$
\frac{dx}{dt} = a(t)x + x b(t) + c(t)
$$

is a linear differential equation; here $A(t)$ is the linear map $x \mapsto a(t)x + x b(t)$ of $G$ to itself.

For every $t \in J$, $A(t)$ is an element of the set $\mathcal{L}(E)$ of continuous linear maps from $E$ to itself (continuous endomorphisms of $E$); one knows (*Gen. Top.*, X, p. 298) that $\mathcal{L}(E)$, endowed with the *norm* $\|U\| = \sup_{\|x\| \leq 1} \|Ux\|$ is a *complete normed algebra* over the field $\mathbf{R}$, and that $\|UV\| \leq \|U\|\ \|V\|$.

*Throughout this section we shall assume that the following conditions are satisfied:*

a) *The map* $t \mapsto A(t)$ *of* $J$ *into* $\mathcal{L}(E)$ *is regulated*.

b) *The map* $t \mapsto b(t)$ *of* $J$ *into* $E$ *is regulated*.

When $E$ has dimension $n$, $\mathcal{L}(E)$ is isomorphic to $\mathbf{R}^{n^2}$ (as a topological vector space) and condition *a*) means that each of the elements $a_{ij}(t)$ of the matrix $A(t)$ is a *regulated* function on $J$.

(1) Recall that if $E$ is of finite dimension then every affine linear map from $E$ into itself is continuous (*Gen. Top.*, VI, p. 33 and 37).

Since $\|A(t')\mathbf{x} - A(t)\mathbf{x}\| \leq \|A(t') - A(t)\|\|\mathbf{x}\|$, the map
$$
t \mapsto A(t).\mathbf{x} + \mathbf{b}(t)
$$
is regulated for every $\mathbf{x} \in E$; further,
$$
\|A(t)\mathbf{x}_1 - A(t)\mathbf{x}_2\| = \|A(t)(\mathbf{x}_1 - \mathbf{x}_2)\| \leq \|A(t)\|\|\mathbf{x}_1 - \mathbf{x}_2\|
$$
for any $t \in J$ and $\mathbf{x}_1, \mathbf{x}_2$ in $E$; in other words, the right-hand side of (2) satisfies the conditions of lemma 1 of IV, p. 165 and is Lipschitz with respect to the regulated function $\|A(t)\|$ on $J \times E$. In consequence (IV, p. 173, cor. 2):

#### Theorem 1 {#fvr-iv-s2-thm-1 .statement}

*Let* $t \mapsto A(t)$ *be a regulated map of* $J$ *into* $\mathcal{L}(E)$, *and* $t \mapsto \mathbf{b}(t)$ *be a regulated map of* $J$ *into* $E$. *For every point* $(t_0, \mathbf{x}_0)$ *of* $J \times E$ *the linear equation* (2) *admits one and only one solution defined on all of* $J$ *and equal to* $\mathbf{x}_0$ *at the point* $t_0$.

### 2. LINEARITY OF THE INTEGRALS OF A LINEAR DIFFERENTIAL EQUATION

Solving a linear differential equation (2) is a linear problem (*Alg.*, II, p. 240); the homogeneous linear equation
$$
\frac{d\mathbf{x}}{dt} = A(t).\mathbf{x}
$$
is said to be *associated* with the inhomogeneous equation (2); and one knows (*Alg.*, II, p. 241, prop. 14) that if $\mathbf{u}_1$ is an integral of the inhomogeneous equation (2) then every integral of this equation is of the form $\mathbf{u} + \mathbf{u}_1$ where $\mathbf{u}_1$ is a solution of the associated homogeneous equation (4), and conversely. We shall first study in this subsection the integrals of a *homogeneous* equation (4).

#### Proposition 1 {#fvr-iv-s2-prop-1 .statement}

*The set* $\mathcal{I}$ *of integrals of the homogeneous linear equation* (4), *defined on* $J$, *is a vector subspace of the space* $C(J; E)$ *of continuous maps from* $J$ *into* $E$.

The proof is immediate.

#### Theorem 2 {#fvr-iv-s2-thm-2 .statement}

*For every point* $(t_0, \mathbf{x}_0)$ *of* $J \times E$ *let* $\mathbf{u}(t, t_0, \mathbf{x}_0)$ *be the integral of the homogeneous equation* (4) *defined on* $J$ *and equal to* $\mathbf{x}_0$ *at* $t_0$.
1. *For every point* $t \in J$ *the map* $\mathbf{x}_0 \mapsto \mathbf{u}(t, t_0, \mathbf{x}_0)$ *is a bijective bicontinuous linear map* $C(t, t_0)$ *of* $E$ *to itself*.
2. *The map* $t \mapsto C(t, t_0)$ *of* $J$ *into* $\mathcal{L}(E)$ *is identical to the integral of the homogeneous linear differential equation*
$$
\frac{dU}{dt} = A(t)\ U
$$
*which takes the value* $I$ **(the identity map of* $E$ *to itself)* *at the point* $t_0$.
3. *For any points* $s, t, u$ *of* $J$
$$
C(s, u) = C(s, t)C(t, u), \qquad C(s, t) = (C(t, s))^{-1}.
$$

By prop. 1, $\mathbf{u}(t, t_0, \mathbf{x}_1) + \mathbf{u}(t, t_0, \mathbf{x}_2)$ (resp. $\lambda \mathbf{u}(t, t_0, \mathbf{x}_0)$) is an integral of (4) and takes the value $\mathbf{x}_1 + \mathbf{x}_2$ (resp. $\lambda \mathbf{x}_0$) at $t_0$, so, by th. 1 of IV, p. 179, is identical to $\mathbf{u}(t, t_0, \mathbf{x}_1 + \mathbf{x}_2)$ (resp. $\mathbf{u}(t, t_0, \lambda \mathbf{x}_0)$); the map $\mathbf{x}_0 \mapsto \mathbf{u}(t, t_0, \mathbf{x}_0)$ is thus a linear map $C(t, t_0)$ of E into itself, and one can write $\mathbf{u}(t, t_0, \mathbf{x}_0) = C(t, t_0). \mathbf{x}_0$.

Since the map $(X, Y) \mapsto XY$ of $\mathcal{L}(E) \times \mathcal{L}(E)$ into $\mathcal{L}(E)$ is continuous (*Gen. Top.*, X, p. 298, prop. 8), the map $t \mapsto A(t)U$ of J into $\mathcal{L}(E)$ is regulated for all $U \in \mathcal{L}(E)$; further (*Gen. Top.*, X, p. 296)

$$
\| A(t)X - A(t)Y \| = \| A(t)(X - Y) \| \leq \| A(t) \| \| X - Y \|,
$$

so one can apply th. I of IV, p. 179 to the homogeneous linear equation (5); let $V(t)$ be the integral of this equation defined on J and equal to $I$ at $t_0$. One has (I, p. 6, prop. 3)

$$
\frac{d}{dt} (V(t)\mathbf{x}_0) = \frac{dV(t)}{dt} \mathbf{x}_0 = A(t)(V(t)\mathbf{x}_0)
$$

and for $t = t_0$ we have $V(t)\mathbf{x}_0 = I\mathbf{x}_0 = \mathbf{x}_0$; by th. 1 of IV, p. 179 one must have $V(t).\mathbf{x}_0 = C(t, t_0)\mathbf{x}_0$ for all $\mathbf{x}_0 \in E$, that is, $V(t) = C(t, t_0)$; this proves that $C(t, t_0)$ belongs to $\mathcal{L}(E)$, in other words, that $\mathbf{x}_0 \mapsto C(t, t_0).\mathbf{x}_0$ is continuous on E, and that the map $t \mapsto C(t, t_0)$ is the integral of (5) which is equal to $I$ at $t_0$.

Finally, the integral $s \mapsto C(s, u).\mathbf{x}_0$ of (4) is equal to $C(t, u).\mathbf{x}_0$ at the point $t$, so, by definition,

$$
C(s, u).\mathbf{x}_0 = C(s, t)(C(t, u).\mathbf{x}_0) = (C(s, t)C(t, u)).\mathbf{x}_0
$$

for any $\mathbf{x}_0 \in E$, whence the first relation (6); since $C(s, s) = I$ one has $C(s, t)C(t, s) = I$, for any $s$ and $t$ in J; this proves (*Set Theory*, II, p. 86, corollary) that $C(t, t_0)$ is a bijective map of E onto itself, with inverse map $C(t_0, t)$. This completes the proof of the theorem.

One says that $C(t, t_0)$ is the *resolvent* of equation (2) of IV, p. 178.

#### Corollary 1 {#fvr-iv-s2-thm-2-cor-1 .statement}

*The map which to every point $\mathbf{x}_0 \in E$ associates the continuous function $t \mapsto C(t, t_0).\mathbf{x}_0$, defined on J, is an isomorphism of the normed space E onto the vector space $\mathcal{I}$ of integrals of (4), endowed with the topology of compact convergence.*

It is certainly a bijective linear map of E onto $\mathcal{I}$: now $C(t, t_0)$ is bounded on a compact set $K \subset J$, so $\| C(t, t_0).\mathbf{x}_0 \| \leq M \| \mathbf{x}_0 \|$ for any $t \in K$ and $\mathbf{x}_0 \in E$, which shows that this map is continuous; and since

$$
C(t_0, t_0).\mathbf{x}_0 = \mathbf{x}_0,
$$

it is clear that the inverse map is also continuous.

#### Corollary 2 {#fvr-iv-s2-thm-2-cor-2 .statement}

*The map $(s, t) \mapsto C(s, t)$ of $J \times J$ into $\mathcal{L}(E)$ is continuous.*

By (6) we have $C(s, t) = C(s, t_0) \left( C(t, t_0) \right)^{-1}$; now, the map $(X, Y) \mapsto XY$ of $\mathcal{L}(E) \times \mathcal{L}(E)$ into $\mathcal{L}(E)$ is continuous, as is the map $X \mapsto X^{-1}$ of the (open) group of invertible elements of $\mathcal{L}(E)$ onto itself (TG, IX, p. 40, prop. 14).

One may note that the map
$$
t \mapsto C(t_0, t) = (C(t, t_0))^{-1}
$$
admits a derivative equal to $-(C(t, t_0))^{-1} (dC(t, t_0)/dt)(C(t, t_0))^{-1}$ (on the complement of a countable set) (I, p. 8, prop. 4), that is to say (by IV, p. 179, formula (5)) equal to $-C(t_0, t) A(t)$.

#### Corollary 3 {#fvr-iv-s2-thm-2-cor-3 .statement}

*Let K be a compact interval contained in J, and let $k = \sup_{t \in K} \|A(t)\|$. For all t and $t_0$ in K*
$$
\|C(t, t_0) - I\| \leq e^{k|t-t_0|} - 1 .
$$ (7)

Indeed, $\|A(t)x_0\| \leq k \|x_0\|$ for all $t \in K$; on K the constant function equal to $x_0$ is thus an approximate integral to within $k \|x_0\|$ by equation (4) of IV, p. 18; by formula (15) of IV, p. 170, one thus has
$$
\|C(t, t_0)x_0 - x_0\| \leq \|x_0\| (e^{k|t-t_0|} - 1)
$$
for any $t$ and $t_0$ in K, and $x_0$ in E, which is equivalent to the inequality (7) by the definition of the norm on $\mathcal{L}(E)$.

#### Proposition 2 {#fvr-iv-s2-prop-2 .statement}

*Let B be a continuous endomorphism of E, independent of t, and commuting with A(t) for all $t \in J$; then B commutes with $C(t, t_0)$ for all t and $t_0$ in J.*

Indeed, by (5)
$$
\frac{d}{dt}(BC) = BAC = ABC \quad \text{and} \quad \frac{d}{dt}(CB) = ACB ,
$$
so $\frac{d}{dt}(BC - CB) = A(BC - CB)$; but $BC(t_0, t_0) - C(t_0, t_0)B = 0$, so (IV, p. 179, th. 1) $BC(t, t_0) - C(t, t_0)B = 0$ for all $t \in J$.

An important instance of prop. 2 is that where E is endowed with the structure of a normed vector space with respect to the *field of complex numbers* $\mathbf{C}$, and where, for every $t \in J$, $A(t)$ is an endomorphism of E for this vector space structure; this means that $A(t)$ commutes with the continuous endomorphism $x \mapsto tx$ of E (for the vector space structure *over* $\mathbf{R}$); then $C(t, t_0)$ commutes with this endomorphism, which means that for any $t$ and $t_0$ in J, the map $C(t, t_0)$ is a continuous endomorphism for the normed vector space structure of E over $\mathbf{C}$.

### 3. INTEGRATING THE INHOMOGENEOUS LINEAR EQUATION

Integrating the inhomogeneous linear equation

$$
\frac{d\mathbf{x}}{dt} = A(t).\mathbf{x} + \mathbf{b}(t)
$$

reduces to integrating the associated homogeneous equation

$$
\frac{d\mathbf{x}}{dt} = A(t).\mathbf{x}
$$

and evaluating a primitive. With the notation of th. 2 of IV, p. 179, let us put $\mathbf{x} = C(t, t_0).\mathbf{z}$, whence, from the second formula (6) of IV, p. 179, $\mathbf{z} = C(t_0, t).\mathbf{x}$; if $\mathbf{x}$ is an integral of (2) then $\mathbf{z}$ is an integral of the equation $\frac{d}{dt}\left(C(t, t_0).\mathbf{z}\right) = A(t)C(t, t_0).\mathbf{z} + \mathbf{b}(t)$; since the bilinear map

$$
(U, y) \mapsto U.y
$$

of $\mathcal{L}(\mathbf{E}) \times \mathbf{E}$ into $\mathbf{E}$ is continuous (\emph{Gen. Top.}, X, p. 297, prop. 6), $\mathbf{z}$ admits a derivative (except on a countable subset of J) and one has, by the formula for differentiating a bilinear function (I, p. 6, prop. 3)

$$
\frac{d}{dt}\left(C(t, t_0).\mathbf{z}\right) = \frac{dC(t, t_0)}{dt}.\mathbf{z} + C(t, t_0).\frac{d\mathbf{z}}{dt} = A(t)C(t, t_0).\mathbf{z} + C(t, t_0).\frac{d\mathbf{z}}{dt}
$$

(replacing $dC(t, t_0)/dt$ by $A(t)C(t, t_0)$ according to (5) (IV, p. 179)). The equation for $\mathbf{z}$ then reduces to $C(t, t_0).d\mathbf{z}/dt = \mathbf{b}(t)$, or again to

$$
\frac{d\mathbf{z}}{dt} = C(t_0, t).\mathbf{b}(t)
$$

by the second formula (6) of IV, p. 179. Now the right-hand side of equation (8) is a regulated function on J, having been obtained by substituting the regulated functions $U$ and $y$ in the continuous bilinear function $U.y$ (\emph{cf.} II, p. 55, cor. 2); equation (8) thus has one and only one integral taking the value $\mathbf{x}_0$ at $t_0$, given by the formula

$$
\mathbf{z}(t) = \mathbf{x}_0 + \int_{t_0}^t C(t_0, s).\mathbf{b}(s)\,ds.
$$

Since one has $C(t, t_0).\int_{t_0}^t C(t_0, s).\mathbf{b}(s)\,ds = \int_{t_0}^t C(t, t_0)C(t_0, s).\mathbf{b}(s)\,ds$ (II, p. 59, formula (9)), one obtains (taking account of the first formula (6) of IV, p. 179) the following result:

#### Proposition 3 {#fvr-iv-s2-prop-3 .statement}

*With the notation of th. 2* (IV, p. 179), *for every point* $(t_0, \mathbf{x}_0)$ *of* $J \times \mathbf{E}$ *the integral of the linear equation* (2) *defined on* $J$ *and equal to* $\mathbf{x}_0$ *at* $t_0$ *is given by the formula*

$$
\mathbf{u}(t) = C(t, t_0).\mathbf{x}_0 + \int_{t_0}^t C(t, s).\mathbf{b}(s)\,ds.
$$

The method which leads to formula (10), which consists of taking the function $\mathbf{z}$ as a new unknown function, is often called the "method of variation of parameters".

### 4. FUNDAMENTAL SYSTEMS OF INTEGRALS OF A LINEAR SYSTEM OF SCALAR DIFFERENTIAL EQUATIONS

In this subsection and the next we shall consider the case where E is a vector space of finite dimension n over the field $\mathbf{C}$ of complex numbers (so of dimension 2n over $\mathbf{R}$), and where, for every $t \in J$, $A(t)$ is an endomorphism of E with respect to the vector space structure over $\mathbf{C}$. One can then identify $A(t)$ with its matrix $(a_{ij}(t))$ with respect to a basis of E (over the field $\mathbf{C}$), the $a_{ij}$ this time being $n^2$ complex functions defined and regulated on J; letting $x_j$ ($1 \leq j \leq n$) denote the (complex) components of a vector $x \in E$ with respect to the chosen basis, the linear equation

$$
\frac{d\mathbf{x}}{dt} = A(t).\mathbf{x} + \mathbf{b}(t)
$$

is again equivalent to the system

$$
\frac{dx_i}{dt} = \sum_{j=1}^n a_{ij}(t)x_j + b_i(t) \qquad (1 \leq i \leq n).
$$

Theorems 1 (IV, p. 179) and 2 (IV, p. 179) and prop. 2 (IV, p. 181) then show that for every $\mathbf{x}_0 = (x_{k0})_{1 \leq k \leq n}$ in E there exists one and only one integral $\mathbf{u} = (u_k)_{1 \leq k \leq n}$ of the equation

$$
\frac{d\mathbf{x}}{dt} = A(t).\mathbf{x}
$$

defined on E and equal to $\mathbf{x}_0$ at the point $t_0$; this integral can be written

$$
\mathbf{u}(t, t_0, \mathbf{x}_0) = C(t, t_0).\mathbf{x}_0,
$$

$C(t, t_0)$ being an invertible square matrix $(c_{ij}(t, t_0))$ of order $n$ whose entries are continuous complex functions on $J \times J$ and such that $t \mapsto c_{ij}(t, t_0)$ is a primitive of a regulated function on J.

In the particular case where $n = 1$ the system (3) reduces to a single scalar equation

$$
\frac{dx}{dt} = a(t)x + b(t)
$$

$a(t)$ and $b(t)$ being complex regulated functions on J); one verifies immediately that the (one element) matrix $C(t, t_0)$ is equal to $\exp \left( \int_{t_0}^t a(s)\, ds \right)$; the integral of (11) equal to $x_0$ at the point $t_0$ is thus given explicitly by the formula

$$
u(t) = x_0 \exp \left( \int_{t_0}^t a(s)\, ds \right) + \int_{t_0}^t b(s) \exp \left( \int_{t_0}^\tau a(\tau)\, d\tau \right) ds.
$$

In the space $\mathcal{C}(J; E)$ of continuous maps from J into E, endowed with the topology of compact convergence, the set $\mathcal{I}$ of integrals of equation (4) is a vector subspace (over $\mathbf{C}$) isomorphic to E, therefore to $\mathbf{C}^n$ (IV, p. 180, cor. 1, and IV, p. 181, prop. 2).

A basis $(\mathbf{u}_j)_{1 \leq j \leq n}$ of this space (over the field $\mathbf{C}$) is called a *fundamental system* of integrals of (4).

#### Proposition 4 {#fvr-iv-s2-prop-4 .statement}

*For the $n$ integrals $\mathbf{u}_j$ ($1 \leq j \leq n$) of equation (4) to form a fundamental system it is necessary and sufficient that their values $\mathbf{u}_j(t_0)$ at a point $t_0 \in J$ be linearly independent vectors in $E$.*

Indeed, the map which to every $\mathbf{x}_0 \in E$ associates the integral $t \mapsto C(t, t_0).\mathbf{x}_0$ is an isomorphism of $E$ onto $\mathcal{I}$ (IV, p. 180, cor. 1 and IV, p. 181, prop. 2).

If $(\mathbf{e}_j)_{1 \leq j \leq n}$ is any basis of $E$ over $\mathbf{C}$, the $n$ integrals
$$
\mathbf{u}_j(t) = C(t, t_0).\mathbf{e}_j \qquad (1 \leq j \leq n)
$$
thus form a fundamental system; if one identifies $C(t, t_0)$ with its matrix with respect to the basis $(\mathbf{e}_j)$ the integrals $\mathbf{u}_j$ are precisely the *columns* of the matrix $C(t, t_0)$. The integral of (4) that takes the value $\mathbf{x}_0 = \sum_{j=1}^n \lambda_j \mathbf{e}_j$ at the point $t_0$ is then $C(t, t_0).\mathbf{x}_0 = \sum_{k=1}^n \lambda_k \mathbf{u}_k(t)$.

Given *any* $n$ integrals $\mathbf{u}_j$ ($1 \leq j \leq n$) of (4) one terms the *determinant* of these $n$ integrals at a point $t \in J$ with respect to a basis $(\mathbf{e}_j)_{1 \leq j \leq n}$ of $E$, the determinant
$$
\Delta(t) = (\mathbf{u}_1(t), \ \mathbf{u}_2(t), \ \ldots, \ \mathbf{u}_n(t))
$$
of the $n$ vectors $\mathbf{u}_j(t)$ with respect to the basis $(\mathbf{e}_j)$ (*Alg.*, III, p. 522). One has (*Alg.*, III, p. 523, prop. 2)
$$
\Delta(t) = \Delta(t_0) \det \left( C(t, t_0) \right).
$$

By prop. 4 of IV, p. 184, for $(\mathbf{u}_j)_{1 \leq j \leq n}$ to be a fundamental system of integrals of (4) it is necessary and sufficient that the determinant $\Delta(t)$ of the $\mathbf{u}_j$ be $\neq 0$ at some one point $t_0$ of $J$; the formula (14) then shows that $\Delta(t) \neq 0$ at every point of $J$, in other words, that the vectors $\mathbf{u}_j(t)$ ($1 \leq j \leq n$) are always linearly independent.

#### Proposition 5 {#fvr-iv-s2-prop-5 .statement}

*The determinant of the matrix $C(t, t_0)$ is given by the formula*
$$
\det \left( C(t, t_0) \right) = \exp \left( \int_{t_0}^t \operatorname{Tr}(A(s)) \, ds \right).
$$
(15)

Indeed, if one puts $\delta(t) = \det \left( C(t, t_0) \right)$ one has, by the formula for the derivative of a determinant (I, p. 8, formula (3))
$$
\frac{d \delta}{dt} = \operatorname{Tr} \left( \frac{dC(t, t_0)}{dt} (C(t, t_0))^{-1} \right) \delta(t)
$$

that is, by the differential equation (5) of IV, p. 179 satisfied by $C(t, t_0)$,

$$
\frac{d \delta}{dt} = \operatorname{Tr}(A(t)) \delta(t).
$$

Since $\delta(t_0) = 1$ the formula (15) follows from the expression (12) (IV, p. 183) for the integral of a scalar linear equation.

Specifying $n$ linearly independent integrals of (4) determines all the integrals of this equation, as we have just seen. We shall now show that for $1 \leq p \leq n$ the knowledge of $p$ linearly independent integrals $\mathbf{u}_j$ ($1 \leq j \leq p$) of equation (4) reduces the integration of this equation to that of a homogeneous linear system of $n - p$ scalar equations. Suppose that on an interval $K \subset J$ there are $n - p$ maps

$$
\mathbf{u}_{p+k} \quad (1 \leq k \leq n - p)
$$

of $K$ into $E$, which are primitives of regulated functions on $K$, and such that, for every $t \in K$, the $n$ vectors $\mathbf{u}_j(t)$ ($1 \leq j \leq n$) form a basis of $E$.

For every point $t_1 \in J$ there always exists an interval $K$, a neighbourhood of $t_1$ in $J$, on which there are defined $n - p$ functions $\mathbf{u}_{p+k}$ ($1 \leq k \leq n - p$) having the preceding properties. For, let $(\mathbf{e}_i)_{1 \leq i \leq n}$ be a basis of $E$; there exist $n - p$ vectors of this basis which form with the $\mathbf{u}_j(t_1)$ ($1 \leq j \leq p$) a basis of $E$ (Alg., II, p. 292, th. 2); suppose for example that they are $\mathbf{e}_{p+1}, \ldots, \mathbf{e}_n$; since the determinant $\det(\mathbf{u}_1(t), \ldots, \mathbf{u}_p(t), \mathbf{e}_{p+1}, \ldots, \mathbf{e}_n)$ (with respect to the basis $(\mathbf{e}_i)$) is a continuous function of $t$ and does not vanish for $t = t_1$ there exists a neighbourhood $K$ of $t_1$ on which it does not vanish; one can then take $\mathbf{u}_{p+k}(t) = \mathbf{e}_{p+k}$ ($1 \leq k \leq n - p$) for $t \in K$.

There exists an invertible matrix $B(t)$ of order $n$, whose elements are primitives of regulated functions on $K$, such that $B(t).\mathbf{e}_j = \mathbf{u}_j(t)$ for $1 \leq j \leq n$. Let us put $x = B(t).y$; then $y$ satisfies the equation $\frac{dB}{dt}.y + B(t).\frac{dy}{dt} = A(t)B(t).y$, which can also be written

$$
\frac{dy}{dt} = (B(t))^{-1} \left( A(t)B(t) - \frac{dB}{dt} \right) .y = H(t).y
$$

where $H(t) = (h_{jk}(t))$ is a matrix with regulated entries on $K$. By the definition of $B(t)$ this linear equation admits the $p$ constant vectors $\mathbf{e}_j$ ($1 \leq j \leq p$) as integrals; one concludes immediately that necessarily $h_{jk}(t) = 0$ for $1 \leq k \leq p$; thus the components $y_k$ of $y$ (with respect to the basis $(\mathbf{e}_i)$) with index $k \geq p + 1$ satisfy a homogeneous linear system of $n - p$ equations; once the solutions of this system are determined, the $dy_j/dt$ for indices $j \leq p$ are linear functions of the $y_k$ with $k \geq p + 1$, so are known, and the primitives of these functions will give the $y_j$ for indices $j \leq p$.

In particular, when one knows $n - 1$ linearly independent integrals of equation (4) of IV, p. 183, integrating this equation reduces to that of a single homogeneous scalar equation, and then the evaluation of $n$ primitives.

#### Remark 1 {#fvr-iv-s2-n4-rem-1 .statement}

All the above applies also to the case where E is of dimension $n$ over the field $\mathbf{R}$ and $A(t)$ is an endomorphism of E for every $t \in J$: one has only to replace $\mathbf{C}$ by $\mathbf{R}$ throughout.

#### Remark 2 {#fvr-iv-s2-n4-rem-2 .statement}

Let $A(t) = (a_{ij}(t))$ be a square matrix of order $n$ whose entries are real (resp. complex) regulated functions of $t$ on $J$, and let $C(t, t_0) = (c_{ij}(t, t_0))$ be the resolvent matrix of the corresponding linear system (3) (IV, p. 22). Let F be an arbitrary complete normed space over $\mathbf{R}$ (resp. $\mathbf{C}$) and let us consider the system of linear differential equations

$$
\frac{dy_i}{dt} = \sum_{j=1}^n a_{ij}(t) y_j
$$

where the unknown functions $y_j$, take their values in F. It is immediate that the solution $(\mathbf{u}_j)_{1 \leq j \leq n}$ of this system such that $\mathbf{u}_j(t_0) = \mathbf{d}_j$ for $1 \leq j \leq n$ ($\mathbf{d}_j$ being arbitrary in F) is given by the formulae

$$
\mathbf{u}_i(t) = \sum_{j=1}^n c_{ij}(t, t_0) \mathbf{d}_j \qquad (1 \leq i \leq n).
$$

We consider in particular the case where $A(t)$ is an endomorphism of a vector space E of finite dimension $n$ over $\mathbf{C}$, such that there exists a basis of E with respect to which the matrix of $A(t)$ has real elements for every $t \in J$. Then the above shows (by th. 1 of IV, p. 179) that the resolvent matrix $C(t, t_0)$ with respect to the same basis also has real elements: it suffices to consider the vector space $E_0$ over $\mathbf{R}$ generated by the basis of E under consideration, and to remark that the restriction of $A(t)$ to $E_0$ is an endomorphism of this vector space.

### 5. ADJOINT EQUATION

Assuming always that the space E is of finite dimension $n$ over $\mathbf{C}$, let $E^*$ be its dual (A, II, p. 40), which is a space of dimension $n$ over $\mathbf{C}$ (Alg., II, p. 299, th. 4); the canonical bilinear form $\langle \mathbf{x}, \mathbf{x}^* \rangle$ defined on $E \times E^*$ (Alg., II, p. 234) is continuous on this product (being a polynomial in the components of $\mathbf{x} \in E$ and $\mathbf{x}^* \in E^*$).

Given a homogeneous linear equation (4) (IV, p. 183), where $t \mapsto A(t)$ is a regulated map of J into $\mathcal{L}(E)$, let us see if there exists a map $t \mapsto \mathbf{v}(t)$ of J into $E^*$, a primitive of a regulated function on J, and such that the scalar function $t \mapsto \langle \mathbf{u}(t), \mathbf{v}(t) \rangle$ is constant on J when $\mathbf{u}$ is an arbitrary solution of (4); it comes to the same to write that the derivative of this function should be zero at every point where $\mathbf{u}$ and $\mathbf{v}$ are differentiable, that is, one must have

$$
\left\langle \frac{d\mathbf{u}}{dt}, \mathbf{v}(t) \right\rangle + \left\langle \mathbf{u}(t), \frac{d\mathbf{v}}{dt} \right\rangle = 0
$$

at such points.

Now, by (4), $\left\langle \frac{d\mathbf{u}}{dt}, \mathbf{v}(t) \right\rangle = \langle A(t).\mathbf{u}(t), \mathbf{v}(t) \rangle = -\langle \mathbf{u}(t), B(t).\mathbf{v}(t) \rangle$ where $-B(t)$ is the transpose of $A(t)$ (Alg., II, p. 234). The relation that $\mathbf{v}$ must satisfy can thus be written

$$
\left\langle \mathbf{u}(t), \frac{d\mathbf{v}}{dt} - B(t).\mathbf{v}(t) \right\rangle = 0
$$

at all points where $A(t)$ is continuous and $\mathbf{v}(t)$ is differentiable. Now for such a point $t$ and an *arbitrary* point $\mathbf{x}_0 \in \mathrm{E}$ there exists, by th. 1 of IV, p. 179, a solution $\mathbf{u}$ of (4) such that $\mathbf{u}(t) = \mathbf{x}_0$; one thus must have $\left\langle \mathbf{x}_0, \frac{d\mathbf{v}}{dt} - B(t).\mathbf{v}(t) \right\rangle = 0$ for *all* $\mathbf{x}_0 \in \mathrm{E}$, which entails $\frac{d\mathbf{v}}{dt} - B(t).\mathbf{v}(t) = 0$. Consequently:

#### Proposition 6 {#fvr-iv-s2-prop-6 .statement}

*The map $t \mapsto \mathbf{v}(t)$ of J into $\mathrm{E}^*$, a primitive of a regulated function on J, is such that $\langle \mathbf{u}(t), \mathbf{v}(t) \rangle$ is constant on J for every solution $\mathbf{u}$ of the equation* (4) *of IV, p. 183 if and only if $\mathbf{v}$ is a solution of the homogeneous linear equation*

$$
\frac{d\mathbf{x}}{dt} = B(t).\mathbf{x} \tag{16}
$$

*where $-B(t)$ is the transpose of $A(t)$.*

Equation (16) is called the *adjoint* of (4); clearly (4) is the adjoint of (16). The elements of the matrix $B(t)$ being regulated functions of $t$ on J, the results obtained above on linear equations apply to (16). In particular, the integral of (16) taking the value $\mathbf{x}_0^*$ at the point $t_0$ can be written as $H(t, t_0).\mathbf{x}_0^*$, where $H(t, t_0)$ is a bijective linear map of $\mathrm{E}^*$ onto itself, identical to the integral of the equation

$$
\frac{dV}{dt} = B(t)V \tag{17}
$$

which takes the value $I$ at the point $t_0$. As a result one has (with the notation of IV, p. 179)

$$
\left\langle C(t, t_0).\mathbf{x}_0, H(t, t_0).\mathbf{x}_0^* \right\rangle = \left\langle \mathbf{x}_0, \mathbf{x}_0^* \right\rangle
$$

for any $\mathbf{x}_0 \in \mathrm{E}$ and $\mathbf{x}_0^* \in \mathrm{E}^*$, which shows that

$$
H(t, t_0) = \check{C}(t, t_0) \tag{18}
$$

(the *contragradient* of $C(t, t_0)$). In particular, if one knows a fundamental system of integrals of the adjoint equation (16) the matrix $H(t, t_0)$ is determined, so is $C(t, t_0)$ also, and as a result, so are *all* the integrals of equation (4).

#### Remark {#fvr-iv-s2-n5-rem-1 .statement}

Let E and F be two complete normed spaces over $\mathbf{R}$ (or over $\mathbf{C}$), and $(\mathbf{x}, \mathbf{y}) \mapsto \langle \mathbf{x}, \mathbf{y} \rangle$ a *continuous* bilinear form on $\mathrm{E} \times \mathrm{F}$, such that the relation “$\langle \mathbf{x}, \mathbf{y} \rangle = 0$ for all $\mathbf{y} \in \mathrm{F}$” (resp. $\langle \mathbf{x}, \mathbf{y} \rangle = 0$ for all $\mathbf{x} \in \mathrm{E}$”) implies $\mathbf{x} = 0$ (resp. $\mathbf{y} = 0$). Suppose further that for every $t \in \mathrm{J}$ there is a continuous linear map $B(t)$ of F into itself, such that $\langle A(t).\mathbf{x}, \mathbf{y} \rangle + \langle \mathbf{x}, B(t).\mathbf{y} \rangle = 0$ for every $(\mathbf{x}, \mathbf{y}) \in \mathrm{E} \times \mathrm{F}$. In these circumstances one sees as before that for a map $t \mapsto \mathbf{v}(t)$ of J into F, a primitive of a regulated function, to be such that $\langle \mathbf{u}(t), \mathbf{v}(t) \rangle$ is *constant* for *every* integral $\mathbf{u}$ of (4), it is necessary and sufficient that $\mathbf{v}$ should be an integral of (16), which again we call the *adjoint* of (4).

### 6. LINEAR DIFFERENTIAL EQUATIONS WITH CONSTANT COEFFICIENTS

Suppose again that E is an arbitrary complete normed space over $\mathbf{R}$; let A be a continuous endomorphism of A, independent of t, and consider the homogeneous linear equation

$$
\frac{d\mathbf{x}}{dt} = A.\mathbf{x}.
$$

When E is of finite dimension the equation (19) is equivalent to a homogeneous system (3) (IV, p. 183) of scalar differential equations, where the coefficients $a_{ij}$ are constant.

By th. 1 (IV, p. 179), every integral of (19) is defined on all of $\mathbf{R}$; by th. 2 (IV, p. 179) the integral of (19) taking the value $\mathbf{x}_0$ at a point $t_0 \in \mathbf{R}$ can be written as $C(t, t_0)\mathbf{x}_0$, where $C(t, t_0)$ is a bijective bicontinuous linear map of E onto itself that satisfies the equation

$$
\frac{dU}{dt} = AU
$$

and is such that $C(t_0, t_0) = I$. Moreover, we have the identity

$$
C(t + \tau, t_0 + \tau) = C(t, t_0)
$$

for any $\tau \in \mathbf{R}$: indeed, one has $dC(s, t_0 + \tau)/ds = AC(s, t_0 + \tau)$ by (20), and since A is constant one also has

$$
\frac{dC(t + \tau, t_0 + \tau)}{dt} = AC(t + \tau, t_0 + \tau);
$$

moreover

$$
C(t_0 + \tau, t_0 + \tau) = I = C(t_0, t_0).
$$

whence we have the identity (21), since the integral of (20) equal to I at the point $t_0$ is unique.

If one puts $C_0(t) = C(t, 0)$ then $C(t, t_0) = C_0(t - t_0)$; moreover, for every $\lambda \in \mathbf{R}$, $C_0(\lambda t)$ is identical to the integral of the equation

$$
\frac{dU}{dt} = \lambda AU
$$

which takes the value I at the point 0. We make the following definition:

#### Definition 1 {#fvr-iv-s2-def-1 .statement}

*Given a continuous endomorphism A of E we denote by $e^A$ or $\exp A$ the automorphism of E equal to the value at the point $t = 1$ of the integral of the equation (20) which takes the value I at the point $t = 0$.*

With this notation the remarks preceding def. 1 show that

$$
C(t, t_0) = \exp \left( A(t - t_0) \right).
$$

The exponential notation just introduced is justified by the following properties, which are entirely analogous to those of the function exp z, for z real or complex (cf. III, p. 98 and 106):

#### Proposition 7 {#fvr-iv-s2-prop-7 .statement}

1' *The map* $X \mapsto e^X$ *is a continuous map of* $\mathcal{L}(E)$ *into the group of automorphisms of* E *(*invertible elements of* $\mathcal{L}(E)$).

2 *The map* $t \mapsto e^{Xt}$ *of* $\mathbf{R}$ *into* $\mathcal{L}(E)$ *is differentiable, and*

$$
\frac{d}{dt} (e^{Xt}) = X e^{Xt} = e^{Xt} X.
$$ (24)

3 *For any* $X \in \mathcal{L}(E)$ *one has*

$$
e^X = \sum_{n=0}^{\infty} \frac{X^n}{n!}
$$ (25)

*the right-hand side being absolutely and uniformly convergent on every bounded subset of* $\mathcal{L}(E)$; *in particular,* $e^{It} = e^t I$ *for* $t \in \mathbf{R}$.

4) *If* X *and* Y *commute then* Y *and* $e^Y$ *commute with* $e^X$, *and*

$$
e^{X+Y} = e^X e^Y.
$$ (26)

The relation (24) follows from the expression (23) for $C(t, 0)$ and from the fact that this function is an integral of (20); by recursion on n one deduces from (24) that $t \mapsto e^{Xt}$ is indefinitely differentiable on $\mathbf{R}$ and that

$$
D^n (e^{Xt}) = X^n e^{Xt}.
$$

By Taylor’s formula one thus can write

$$
e^X = I + \frac{X}{1!} + \frac{X^2}{2!} + \cdots + \frac{X^n}{n!} + X^{n+1} \int_0^1 \frac{(1-t)^n}{n!} e^{Xt} \, dt.
$$ (27)

On the other hand, cor. 3 of IV, p. 181 shows that $\| e^{Xt} \| \leq \exp (\| X \| |t| )$. Thus the remainder $r_n(X) = X^{n+1} \int_0^1 \frac{(1-t)^n}{n!} e^{Xt} \, dt$ in formula (27) satisfies the inequality

$$
\| r_n(X) \| \leq \frac{\| X \|^{n+1}}{(n+1)!} e^{\| X \| }
$$

whence one deduces the formula (25), the series on the right-hand side being absolutely and uniformly convergent on every bounded subset of $\mathcal{L}(E)$. For every pair of elements $X,\ T$ of $\mathcal{L}(E)$ one thus has

$$
e^{X+T} - e^X = \sum_{n=1}^{\infty} \frac{1}{n!} ((X+T)^n - X^n ).
$$

Now, one can write $(X + T)^n - X^n = \sum_{(V_i)} V_1 V_2 \ldots V_n$, where the sum is taken over the $2^n - 1$ sequences $(V_i)$ of elements of $\mathcal{L}(E)$ such that $V_i = X$ or $V_i = T$ for $1 \leq i \leq n$, and at least one of the $V_i$ is equal to $T$; the inequality
$$
\|(X + T)^n - X^n\| \leq (\|X\| + \|T\|)^n - \|X\|^n
$$
follows immediately, whence
$$
\|\exp(X + T) - \exp X\| \leq \exp \left( \|X\| + \|T\| \right) - \exp \|X\|
$$
which establishes the continuity of the map $X \mapsto \exp X$.

Finally, if $X$ and $Y$ commute, then $Y$ commutes with $e^{Xt}$ (IV, p. 181, prop. 2), so
$$
\frac{d}{dt} (e^{Xt} e^{Yt}) = X e^{Xt} e^{Yt} + e^{Xt} (Y e^{Yt}) = (X + Y) e^{Xt} e^{Yt}.
$$
Since, on the other hand, $e^{Xt} e^{Yt}$ is equal to $I$ for $t = 0$, one has $e^{Xt} e^{Yt} = e^{(X+Y)t}$, whence formula (26). From this latter, one deduces in particular that for arbitrary real $s$ and $t$ one has
$$
e^{X(s+t)} = e^{Xs} e^{Xt}
$$
and also that
$$
e^{-X} = (e^X)^{-1}.
$$

On the contrary one notes that (26) need not remain valid if $X$ and $Y$ are no longer assumed to commute: indeed it would imply that $\exp X$ and $\exp Y$ always commute, which is not the case, as is shown by simple examples (IV, p. 204, exerc. 3).

Now let us assume that $E$ is a vector space *of finite dimension over the field* $\mathbf{C}$, and $A$ an endomorphism of $E$ (for its vector space structure over $\mathbf{C}$) which one can identify with its matrix with respect to a basis of $E$; then, for all $t \in \mathbf{R}$, $e^{At}$ is an automorphism of $E$ for the same structure (IV, p. 181, prop. 2). Let $r_k$ ($1 \leq k \leq q$) be the distinct roots (in $\mathbf{C}$) of the *characteristic polynomial* $\varphi(r) = \det(A - rI)$ of the endomorphism $A$ (the "characteristic roots" of $A$); if $n_k$ is the order of multiplicity of $r_k$ then $\sum_{k=1}^q n_k = n$. One knows that (Alg., VII, 31, n° 3) to each root $r_k$ there corresponds a subspace $E_k$ of $E$, of dimension $n_k$, such that $E_k$ is *stable* under $A$, and that $E$ is the *direct sum* of the $E_k$: $E_k$ can be defined as the subspace of vectors $\mathbf{x}$ such that
$$
(A - r_k I)^{n_k} . \mathbf{x} = 0.
$$
Let $\mathbf{a}$ be any vector in $E$; one can write $\mathbf{a} = \sum_{k=1}^q \mathbf{a}_k$, where $\mathbf{a}_k \in E_k$; the integral of the equation (19) of IV, p. 188, taking the value $\mathbf{a}$ at the point $t = 0$ is thus given by
$$
\mathbf{u}(t) = e^{At} . \mathbf{a} = \sum_{k=1}^q e^{At} . \mathbf{a}_k = \sum_{k=1}^q e^{r_k t} e^{(A - r_k I)t} . \mathbf{a}_k.
$$

But since $\mathbf{a}_k \in E_k$ one has

$$
e^{(A - r_k I)t} \cdot \mathbf{a}_k = \mathbf{a}_k + \frac{t}{1!}(A - r_k I) \cdot \mathbf{a}_k + \frac{t^2}{2!}(A - r_k I)^2 \cdot \mathbf{a}_k + \cdots
$$
$$
+ \frac{t^{n_k - 1}}{(n_k - 1)!}(A - r_k I)^{n_k - 1} \cdot \mathbf{a}_k .
$$

Thus every integral of the equation (19) of IV, p. 188, can be written as

$$
\mathbf{u}(t) = \sum_{k=1}^q e^{r_k t} \mathbf{p}_k(t)
$$

where $\mathbf{p}_k(t)$ is a polynomial in $t$, with coefficients in the vector space $E_k$, and of degree $\leq n_k - 1$. In particular, if all the roots of the characteristic equation of $A$ are *simple*, the spaces $E_k$ ($1 \leq k \leq n$) are all of dimension 1 over the field $\mathbf{C}$, so there exist $n$ vectors $c_k$ such that the $n$ functions $e^{r_k t} c_k$ ($1 \leq k \leq n$) form a fundamental system of integrals of the equation (19) of IV, p. 188.

The characteristic roots of the endomorphism $A$ are also called *characteristic roots of the linear equation* (19) of IV, p. 188. One may observe that one obtains the characteristic equation of $A$ by writing that the function $c e^{r t}$ is an integral of (19) for a vector $c \neq 0$.

When one has determined the roots $r_k$ ($1 \leq k \leq q$) explicitly, and thus the order of multiplicity $n_k$ of $r_k$, in practice one obtains the integrals of (19) by writing that this equation is satisfied by the expression (32) of IV, p. 191, where $\mathbf{p}_k$ is an arbitrary polynomial of degree $\leq n_k - 1$, with coefficients *in* $E$; on identifying the coefficients of $e^{r_k t}$ (for $1 \leq k \leq q$) in the two sides of the equation so obtained one obtains linear equations for the coefficients of the polynomials $\mathbf{p}_k$: one establishes easily that these equations determine the terms of degree $> 0$ of $\mathbf{p}_k$ as functions of the constant term, and that the latter is a solution of the equation $(A - r_k I)^{n_k} \cdot \mathbf{x} = 0$, which defines the subspace $E_k$ (method of "undetermined coefficients").

#### Remark {#fvr-iv-s2-n6-rem-1 .statement}

When there exists a basis of $E$ such that the matrix of $A$ with respect to this basis has *real* elements (*cf.* IV, p. 186, *Remark* 2), the characteristic equation of $A$ has real coefficients. For every $\mathbf{x} = (\xi_k)_{1 \leq k \leq n}$ of $E$, expressed in the basis under consideration, let $\overline{\mathbf{x}} = (\overline{\xi}_k)_{1 \leq k \leq n}$; the map $\mathbf{x} \mapsto \overline{\mathbf{x}}$ is an antilinear involution of $E$. One knows (*Alg.*, VII) that, if $r_k$ is a non-real root of the characteristic equation, and $E_k$ is the corresponding stable subspace, then $\overline{r}_k$ is a characteristic root having the same multiplicity $n_k$ as $r_k$, and the image $E'_k$ of $E_k$ under the map $\mathbf{x} \mapsto \overline{\mathbf{x}}$ is the stable subspace corresponding to $\overline{r}_k$. One deduces from this that if $\mathbf{u}_j$ ($1 \leq j \leq n_k$) are $n_k$ linearly independent integrals with values in $E_k$, then the $2n_k$ integrals $\mathbf{u}_j + \overline{\mathbf{u}}_j,\ i(\mathbf{u}_j - \overline{\mathbf{u}}_j)$ are linearly independent, and have, with respect to the chosen basis of $E$, components which are *real* functions of $E$. If $r_k$ is a real characteristic root *Remark* 2 of IV, p. 186, shows that (with the same notation) there are $n_k$ linearly independent integrals $\mathbf{v}_j$ ($1 \leq j \leq n_k$) with values in $E_k$ whose components are real. That way one obtains a fundamental system of integrals of (19) whose components are all *real*.

### 7. LINEAR EQUATIONS OF ORDER $n$

One calls a *linear differential equation of order* $n$ an equation of the form

$$
D^n x - a_1(t) D^{n-1} x - \ldots - a_{n-1}(t) D x - a_n(t) x = b(t)
$$

where the $a_k$ ($1 \leq k \leq n$) and $b$ are real (complex) functions of the real variable $t$, defined on an interval $J$ of $\mathbf{R}$. The general procedure of IV, p. 164 shows that this equation is equivalent to the linear system of $n$ first order equations

$$
\left\{
\begin{aligned}
\frac{dx_k}{dt} &= x_{k+1} & (1 \leq k \leq n-1) \\
\frac{dx_n}{dt} &= a_1(t)x_n + a_2(t)x_{n-1} + \cdots + a_n(t)x_1 + b(t)
\end{aligned}
\right.
$$

that is to say, to the linear equation

$$
\frac{d\mathbf{x}}{dt} = A(t).\mathbf{x} + \mathbf{b}(t)
$$

where we have put $\mathbf{x} = (x_1, x_2, \ldots, x_n) \in \mathbf{C}^n$, $\mathbf{b}(t) = (0, 0, \ldots, 0, b(t))$, and where the matrix $A(t)$ is defined by

$$
A(t) = \begin{pmatrix}
0 & 1 & 0 & \ldots & 0 \\
0 & 0 & 1 & \ldots & 0 \\
\vdots & \vdots & \vdots & \ddots & \vdots \\
0 & 0 & 0 & \ldots & 1 \\
a_n(t) & a_{n-1}(t) & a_{n-2}(t) & \ldots & a_1(t)
\end{pmatrix}.
$$

The study of the linear equation of order $n$ thus consists of applying the general results above to the particular linear equation (35). For every interval $J$ where the functions $a_j$ ($1 \leq j \leq n$) and $b$ are *regulated* there exists one and only one function $u$, defined on $J$, having a continuous derivative of order $n-1$, and a regulated derivative of order $n$ on this interval (except at the points of a countable set), satisfying (33) on the complement of a countable subset of $J$, and such that

$$
u(t_0) = x_0, \qquad Du(t_0) = x_0', \ldots, \quad D^{n-1}u(t_0) = x_0^{(n-1)}
$$

where $t_0$ is an arbitrary point of $J$, and $x_0, x_0', \ldots, x_0^{(n-1)}$ are $n$ arbitrary complex numbers.

For the $p$ integrals $u_j$ ($1 \leq j \leq p$) of the homogeneous equation

$$
D^n x - a_1(t) D^{n-1} x - \ldots - a_{n-1}(t) D x - a_n(t) x = 0
$$

associated with (33) to be linearly independent (in the space $C(J; \mathbf{C})$ of continuous maps from $J$ into $\mathbf{C}$, considered as a vector space over $\mathbf{C}$), it is necessary and sufficient that the corresponding $p$ integrals $\mathbf{u}_j = (u_j, Du_j, \ldots, D^{n-1}u_j)$ of the homogeneous equation $d\mathbf{x}/dt = A(t).\mathbf{x}$ should be linearly independent (in the space $C(J; \mathbf{C}^n)$ of continuous maps from $J$ into $\mathbf{C}^n$). It is clear that this condition is necessary.

Conversely, if there are $n$ complex constants $\lambda_j$, not all zero, such that $\sum_{j=1}^n \lambda_j u_j(t) = 0$ identically on $J$, one deduces that $\sum_{j=1}^n \lambda_j D^k u_j(t) = 0$ on $J$ for every integer $k$ such that $1 \leq k \leq n - 1$, which means that $\sum_{j=1}^n \lambda_j \mathbf{u}_j(t) = 0$ on $J$.

Consequently (IV, p. 180, cor. 1)

#### Proposition 8 {#fvr-iv-s2-prop-8 .statement}

*The set of integrals of the homogeneous linear equation (37), defined on $J$, is a vector space of dimension $n$ over the field $\mathbf{C}$.*

Given any $n$ integrals $u_j$ ($1 \leq j \leq n$) of equation (37) one calls the *Wronskian* of this system of integrals the determinant (with respect to the canonical basis of $\mathbf{C}^n$) of the corresponding $n$ integrals $\mathbf{u}_j$ of the equation $d\mathbf{x}/dt = A(t).\mathbf{x}$, that is to say, the function

$$
W(t) = \begin{vmatrix}
u_1(t) & u_2(t) & \ldots & u_n(t) \\
Du_1(t) & Du_2(t) & \ldots & Du_n(t) \\
\vdots & \vdots & \ddots & \vdots \\
D^{n-1}u_1(t) & D^{n-1}u_2(t) & \ldots & D^{n-1}u_n(t)
\end{vmatrix}.
$$

For the $n$ integrals $u_j$ to be linearly independent it is necessary and sufficient that $W(t) \neq 0$ on $J$; moreover, it suffices for this that $W(t_0) \neq 0$ at *only one* $t_0$ of $J$ (IV, p. 184, prop. 4); further, one has (IV, p. 184, prop. 5)

$$
W(t) = W(t_0) \exp \left( \int_{t_0}^t a_1(s)\, ds \right).
$$ (38)

We identify the resolvent $C(t, t_0)$ of equation (35) with its matrix with respect to the canonical basis of $\mathbf{C}^n$; the columns $\mathbf{v}_j(t, t_0)$ ($1 \leq j \leq n$) of this matrix are then $n$ linearly independent integrals

$$
\mathbf{v}_j(t, t_0) = (v_j(t, t_0), Dv_j(t, t_0), \ldots, D^{n-1}v_j(t, t_0))
$$

of the homogeneous equation $d\mathbf{x}/dt = A(t).\mathbf{x}$ which correspond to $n$ linearly independent integrals $v_j(t, t_0)$ of equation (37) such that

$$
D^{k-1}v_j(t_0, t_0) = \delta_{jk}
$$

(Kronecker delta) for $1 \leq j \leq n, 1 \leq k \leq n$ (on agreeing to put $D^0 v_j = v_j$). It results in particular that the method of variation of parameters (IV, p. 182) applied to equation (35) here gives as a particular integral of (33), equal to 0 together with its first $n-1$ derivatives at the point $t_0$, the function

$$
w(t) = \int_{t_0}^t v_n(t, s)b(s)\, ds.
$$ (39)

In the particular case of the equation $D^n x = b(t)$ the formula (39) again gives the formula expressing the $n^{th}$ primitive of the regulated function $b(t)$ which vanishes with its first $n - 1$ derivatives at the point $t_0$, namely
$$
w(t) = \int_{t_0}^t b(s) \frac{(t-s)^{n-1}}{(n-1)!} \, ds
$$
(II, p. 62, formula (19)): the integral of $D^n x = 0$ which vanishes together with its first $n - 2$ derivatives at the point $t_0$, and whose $n - 1$th derivative is equal to 1 there, is actually the polynomial $(t-t_0)^{n-1}/(n-1)!$.

### 8. LINEAR EQUATIONS OF ORDER $n$ WITH CONSTANT COEFFICIENTS

If the coefficients $a_j$ in equation (33) are constant, the corresponding matrix $A$ is constant; the characteristic equation is obtained by writing that $e^{rt}$ is a solution, which gives
$$
r^n - a_1 r^{n-1} - \ldots - a_{n-1} r - a_n = 0.
$$
Let $r_j$ ($1 \leq j \leq q$) be the distinct roots of this equation, and $n_j$ ($1 \leq j \leq q$) the multiplicity of the root $r_j \left( \sum_{j=1}^q n_j = n \right)$. By the results of IV, p. 188 to 194, to each root $r_j$ there corresponds, for the homogeneous equation
$$
D^n x - a_1 D^{n-1} x - \cdots - a_{n-1} D x - a_n x = 0
$$
a system of $n_j$ linearly independent integrals
$$
u_{jk}(t) = e^{r_j t} p_{jk}(t),
$$
where $p_{jk}$ is a polynomial (with complex coefficients) of degree $\leq n_j - 1$ ($1 \leq k \leq n_j$); further, the $n$ integrals $u_{jk}$ ($1 \leq j \leq q,\ 1 \leq k \leq n_j$) so obtained are linearly independent. It follows that the $n_j$ polynomials $p_{jk}$ ($1 \leq k \leq n_j$) are linearly independent in the space of polynomials in $t$ of degree $\leq n_j - 1$, so form a basis (over $\mathbf{C}$) of this space, since the latter is of dimension $n_j$. In other words:

#### Proposition 9 {#fvr-iv-s2-prop-9 .statement}

*Let $r_j$ ($1 \leq j \leq q$) be the distinct roots of the characteristic equation (40), and let $n_j$ be the multiplicity of the root $r_j$ ($1 \leq j \leq q$). Then the $n$ functions $t^k e^{r_j t}$ ($1 \leq k \leq n_j,\ 1 \leq j \leq q$) are linearly independent integrals of the homogeneous equation (41).*

One can prove this result directly in the following way. It follows from equation (41) that the $n^{th}$ derivative of every integral of this equation is differentiable on $\mathbf{R}$, from which one deduces immediately, by induction on the integer $m > n$, that every integral of (41) admits a derivative of order $m$, that is, is *indefinitely differentiable* on $\mathbf{R}$. Let $\mathcal{D}$ be the (non-topological) vector space over $\mathbf{C}$ of indefinitely differentiable complex-valued functions on $\mathbf{R}$; the map $x \mapsto Dx$ is an endomorphism of this space, and equation (41) can be written

$$
f(D)x = 0 \tag{42}
$$

where $f(D) = D^n - a_1 D^{n-1} - \ldots - a_{n-1} D - a_n$ (Alg., IV, p. 4).

#### Proposition 10 {#fvr-iv-s2-prop-10 .statement}

*Let g and h be two relatively prime polynomials such that $f = gh$. The subspace of solutions of (42) is the direct sum of the subspaces of solutions of the two equations*

$$
g(D)x = 0, \qquad h(D)x = 0.
$$

Now, by the Bezout identity (Alg., VII. 2, th. 1) there exist two polynomials $p(D)$ and $q(D)$ such that $p(D)g(D) + q(D)h(D) = 1$. For every solution $x$ of (42) one can write $x = y + z$, where $y = p(D)g(D)x$ and $z = q(D)h(D)x$; and then $h(D)y = p(D)(f(D)x) = 0$ and $g(D)z = q(D)(f(D)x) = 0$. On the other hand, if both $g(D)x = 0$ and $h(D)x = 0$, one deduces that

$$
x = p(D)(g(D)x) + q(D)(h(D)x) = 0,
$$

which completes the proof.

With the preceding notation one can write

$$
f(D) = \prod_{j=1}^q (D - r_j)^{n_j}
$$

and prop. 10, by induction on $q$, shows that the subspace of solutions of (42) is the direct sum of the subspaces of solutions of the $q$ equations

$$
(D - r_j)^{n_j} x = 0 \qquad (1 \leq j \leq q). \tag{43}
$$

Now, for every complex number $r$ one has

$$
D(e^{rt} x) = e^{rt}(D + r)x \tag{44}
$$

so (43) is equivalent to

$$
D^{n_j}(e^{-r_j t} x) = 0
$$

and thus has as solutions the functions $e^{r_j t} p_j(t)$, where $p_j$ runs through the set of polynomials of degree $\leq n_j - 1$; thus one recovers prop. 9 of IV, p. 194.

Assuming that the homogeneous equation (41) has been solved (that is, assuming that the characteristic roots have been found), one knows that the method of variation of parameters allows one to find the solutions of the inhomogeneous equation

$$
D^n x - a_1 D^{n-1} x - \ldots - a_{n-1} Dx - a_n x = b(t) \tag{45}
$$

where $b(t)$ is an *arbitrary* regulated function (IV, p. 182); we note that if $b(t)$ is *indefinitely differentiable* on an interval J then all the integrals of (45) are indefinitely differentiable on J. In the particular case $b(t) = e^{\alpha t} p(t)$, where $p$ is a polynomial (with complex coefficients) and $\alpha$ is an arbitrary complex number, one obtains an integral of (45) more simply by the following method. Put $x = e^{\alpha t} y$; the equation

$$
f(D)x = e^{\alpha t} p(t)
$$

can, by (44), be written

$$
f(\alpha + D)y = p(t)
$$

or, by Taylor’s formula applied to the polynomial $f(D)$,

$$
\frac{f^{(n)}(\alpha)}{n!} D^n y + \frac{f^{(n-1)}(\alpha)}{(n-1)!} D^{n-1} y + \cdots + \frac{f'(\alpha)}{1!} Dy + f(\alpha) y = p(t). \tag{46}
$$

Let $m$ be the degree of the polynomial $p(t) = \sum_{k=0}^m \lambda_k t^{m-k}$; if $f(\alpha) \neq 0$ (that is, if $\alpha$ is not a characteristic root), there exists one and only one polynomial $u(t) = \sum_{k=0}^m c_k t^{m-k}$ *of degree* $m$ which is a solution of (46), for the coefficients $c_k$ are determined by the system of linear equations

$$
f(\alpha)c_k + \binom{m-k+1}{1} f'(\alpha)c_{k-1} + \binom{m-k+2}{2} f''(\alpha)c_{k-2} + \cdots
+ \binom{m}{k} f^{(k)}(\alpha)c_0 = \lambda_k \qquad (0 \leq k \leq m)
$$

which clearly admits one and only one solution. If, on the other hand, $\alpha$ is a characteristic root, and $h$ is its multiplicity, the preceding calculation shows that there is one and only one polynomial of degree $m$ such that every solution of $D^h y = v(t)$ is an integral; in other words, every polynomial solution of (46) is then of degree $m + h$ ("resonance").

### 9. SYSTEMS OF LINEAR EQUATIONS WITH CONSTANT COEFFICIENTS

With the notation of n° 8, let us consider more generally a system of $m$ differential equations of the form

$$
\sum_{k=1}^n p_{jk}(D) x_k = b_j(t) \qquad (1 \leq j \leq m) \tag{47}
$$

where the unknowns $x_k$ ($1 \leq k \leq n$) and the right-hand sides $b_j$ ($1 \leq j \leq m$) are complex functions of the real variable $t$, and where the $p_{jk}(D)$ are polynomials (of any degree) with *constant* (complex) coefficients in the differentiation operator $D$ ($1 \leq j \leq m,\ 1 \leq k \leq n$).

Such systems are not of the same type as those considered in IV, p. 1164 (formula (5)), as the following example shows:

$$
\begin{cases}
D x_1 = a(t) \\
D^2 x_1 + D x_2 + x_2 = b(t).
\end{cases}
$$

We shall confine ourselves to the case where the functions $b_j(t)$ are *indefinitely differentiable* on the interval J, and we shall look only for solutions $(x_k)_{1 \leq k \leq n}$ which are indefinitely differentiable on J. On putting $\mathbf{b}(t) = (b_1(t), \ldots, b_m(t))$, (a map from J into $\mathbf{C}^m$), and $\mathbf{x} = (x_1, x_2, \ldots, x_n)$, the system (47) can be written as

$$
P(D) \mathbf{x} = \mathbf{b}(t)
$$

where $P(D)$ is the matrix $(p_{jk}(D))$ with m rows and n columns, whose coefficients belong to the ring $\mathbf{C}[D]$ of polynomials in D, with coefficients in $\mathbf{C}$. Let $f_j(D)$ ($1 \leq j \leq r \leq \operatorname{Min}(m, n)$) be the nonzero *similarity invariants* of the matrix $P(D)$; one knows (*Alg.*, VII, p. 32) that these are well-determined monic polynomials, such that $f_j$ divides $f_{j+1}$ for $1 \leq j \leq r - 1$ ($r$ being the *rank* of $P(D)$); further, there are two square matrices $U(D)$ and $V(D)$ of order m and n respectively, *invertible* (in the rings of square matrices of order m and n respectively, *with coefficients in the ring $\mathbf{C}[D]$ of polynomials in D with complex coefficients*), and such that all the entries of the matrix $Q(D) = (q_{jk}(D)) = U(D) P(D) V(D)$ are zero, apart from the diagonal terms $q_{jj}(D) = f_j(D)$ for $1 \leq j \leq r$. Now we put $\mathbf{y} = V^{-1}(D) \mathbf{x}$; the equation (49) is equivalent to the equation

$$
U(D) (P(D)(V(D) \mathbf{y})) = U(D) \mathbf{b}
$$

that is, to

$$
Q(D) \mathbf{y} = U(D) \mathbf{b}
$$

since $U(D)$ is invertible. Now, if $\mathbf{y} = (y_1, y_2, \ldots, y_n)$, and if

$$
U(D) \mathbf{b}(t) = (c_1(t), \ldots, c_m(t)),
$$

then equation (50) can be written

$$
f_j(D) y_j = c_j(t) \quad \text{for } 1 \leq j \leq r \tag{51}
$$
$$
0 = c_j(t) \quad \text{for } r + 1 \leq j \leq m. \tag{52}
$$

The system thus does not admit any indefinitely differentiable solutions unless the conditions (52) are satisfied; the determination of the $y_j$ for indices $j \leq r$ then reduces to integrating the r linear differential equations with constant coefficients (51); the $y_j$ for indices $> r$ are arbitrary indefinitely differentiable functions. Once the solutions $\mathbf{y}$ of (50) have thus been determined, one deduces the solutions of (47) from the formula $\mathbf{x} = V(D) \mathbf{y}$.

#### Remark 1 {#fvr-iv-s2-n9-rem-1 .statement}

Some of the polynomials $f_j(D)$ may reduce to nonzero constants; the corresponding $y_j$ are then completely determined.

#### Remark 2 {#fvr-iv-s2-n9-rem-2 .statement}

When the $b_j$ are all zero, that is, if the system (47) is *homogeneous*, the conditions (52) are always satisfied; if, further, $r = n$, one sees that the set of solutions of (47) is a vector space over $\mathbf{C}$, of dimension equal to the *sum of the degrees* of the $f_j(D)$, that is, to the *degree* of $\det(P(D))$.

#### Remark 3 {#fvr-iv-s2-n9-rem-3 .statement}

Given the polynomials $p_{jk}(D)$, a system (47) which admits solutions when the right-hand sides are indefinitely differentiable (or differentiable of a certain order) may not admit them when the right hand sides are arbitrary regulated functions: this is shown by the example (48), which has no solution when $a(t)$ is not a primitive. We shall not undertake here to seek for supplementary possibility conditions which enter when the right-hand sides are arbitrary regulated functions.

### Exercises {#fvr-iv-s2-exercises}

See the [exercises for § 2](exercises/s2/).
