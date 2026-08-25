---
book: alg
book_title: Algebra
chapter: II
chapter_title: LINEAR ALGEBRA
section: 9
section_title: Affine spaces and projective spaces
lang: en
source: alg-i-iii
source_edition: 1998, Springer
pdf_pages: 0349-0361, 0434-0441
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF AFFINE SPACES
      page: 0
      pdf_page: 349
    - "no": 2
      title: BARYCENTRIC CALCULUS
      page: 0
      pdf_page: 350
    - "no": 3
      title: AFFINE LINEAR VARIETIES
      page: 0
      pdf_page: 351
    - "no": 4
      title: AFFINE LINEAR MAPPINGS
      page: 0
      pdf_page: 353
    - "no": 5
      title: DEFINITION OF PROJECTIVE SPACES
      page: 0
      pdf_page: 355
    - "no": 6
      title: HOMOGENEOUS COORDINATES
      page: 0
      pdf_page: 355
    - "no": 7
      title: PROJECTIVE LINEAR VARIETIES
      page: 0
      pdf_page: 356
    - "no": 8
      title: PROJECTIVE COMPLETION OF AN AFFINE SPACE
      page: 0
      pdf_page: 357
    - "no": 9
      title: EXTENSION OF RATIONAL FUNCTIONS
      page: 0
      pdf_page: 358
    - "no": 10
      title: PROJECTIVE LINEAR MAPPINGS
      page: 0
      pdf_page: 359
    - "no": 11
      title: PROJECTIVE SPACE STRUCTURE
      page: 0
      pdf_page: 361
statements: 12
exercises: 6
content_sha256: e8f5479c926f36efd930209e9e33bd70d93806fd5c3cf7274d90e1ef224a7e56
---

## § 9. AFFINE SPACES AND PROJECTIVE SPACES

### 1. DEFINITION OF AFFINE SPACES

#### Definition 1 {#alg-ii-s9-def-1 .statement}

*Given a left (resp. right) vector space T over a field K, an affine space attached to T is any homogeneous space E of the additive group T* (I, § 5, no. 5) *such that 0 is the only operator in T leaving invariant all the elements of E* (that is, T *operates faithfully and transitively on E*). *Under these conditions, T is called the translation space of E and its elements are called the translations of E* (or *free vectors of E*).

In what follows we shall confine our attention to the case where T is a left vector space over K. The dimension (over K) of the translation vector space T of an affine space E is called the *dimension* of E (over K) and is denoted by dim E or $\dim_K E$. An affine space of dimension one (resp. two) is called an *affine line* (resp. an *affine plane*). The elements of an affine space are also called *points*.

Under the conditions of Definition 1, for $t \in T$ and $a \in E$ we shall denote by $t + a$ or $a + t$ the transform of the point a under t. Then the relations

$$
s + (t + a) = (s + t) + a, \quad 0 + a = a
$$

hold for $s \in T, t \in T, a \in E$. The mapping $x \mapsto x + t$ is a bijection of E onto itself, which we identify with t. Definition 1 moreover implies that, for all $a \in E$, the mapping $t \mapsto t + a$ is a *bijection* of T onto E. In other words, given two points $a, b$ of E, there exists one and only one translation t such that $b = t + a$; we shall denote this translation by $b - a$; then the formulae

$$
a - a = 0, \quad a - b = -(b - a), \quad b = (b - a) + a
$$
$$
(c - b) + (b - a) = c - a
$$

hold for $a \in E, b \in E, c \in E$. If four points $a, b, a', b'$ of E are such that $b - a = b' - a'$, the formula

$$
b' = (b' - b) + (b - a) + a = (b' - a') + (a' - a) + a
$$

and the commutativity of addition in T show that $b' - b = a' - a$.

Given a point $a \in E$, the mapping $x \mapsto x - a$ is a bijection of $E$ onto $T$; when $E$ is identified with $T$ under this mapping, we say that $E$ is considered as the vector space obtained *by taking $a$ as origin* in $E$. Conversely, every vector space $T$ has canonically the structure of an affine space attached to $T$, namely the homogeneous space structure corresponding to the subgroup $\{0\}$ of $T$ (I, § 5, no. 6).

#### Remark {#alg-ii-s9-n1-rem-1 .statement}

The definitions of this no. and some of the results which follow extend immediately to the case where, instead of a vector space $T$, we consider an arbitrary *commutative group with operators* $T$.

### 2. BARYCENTRIC CALCULUS

#### Proposition 1 {#alg-ii-s9-prop-1 .statement}

*Let* $(x_i)_{i \in I}$ *be a family of points in an affine space* $E$ *and* $(\lambda_i)_{i \in L}$ *a family of elements of* $K$ *of finite support such that* $\sum_{i \in I} \lambda_i = 1$ *(*resp. $\sum_{i \in I} \lambda_i = 0$*). *If* $a$ *is any point of* $E$, *the point* $x \in E$ *defined by*
$$
x - a = \sum_{i \in I} \lambda_i (x_i - a)
$$
*(resp. the free vector* $\sum_{i \in I} \lambda_i (x_i - a)$) *is independent of the point considered.*

If $a'$ is another point of $E$, then
$$
\sum_i \lambda_i (x_i - a') = \sum_i \lambda_i ((x_i - a) + (a - a')) = \sum_i \lambda_i (x - a) + \left( \sum_i \lambda_i \right) (a - a').
$$
If $\sum_i \lambda_i = 1$, then $\sum_i \lambda_i (x_i - a) = (x - a) + (a - a') = x - a'$; if $\sum_i \lambda_i = 0$, then $\sum_i \lambda_i (x - a') = \sum_i \lambda_i (x - a)$; whence the proposition.

Under the conditions of Proposition 1, the point $x$ defined by
$$
x - a = \sum_{i \in I} \lambda_i (x_i - a)
$$
*(resp. the free vector* $\sum_{i \in I} \lambda_i (x_i - a)$) *is denoted by* $\sum_{i \in I} \lambda_i x_i$.

Thus in particular the notation $b - a$ introduced in no. 1 is recovered. When $\sum_i \lambda_i = 1$, the point $x = \sum_i \lambda_i x_i$ is called *the barycentre of the points* $x_i$ *given the masses* $\lambda_i$.

Given $m$ points $a_1, \ldots, a_m$ of $E$, whose number $m$ is not a multiple of the characteristic of $K$ (V, § 1), the point $g = \sum_{i=1}^m \frac{1}{m} a_i$ is called (by an abuse of

language) the *barycentre of the points* $a_i$ ($1 \leq i \leq m$) (for $m = 2$, we say "midpoint" instead of "barycentre"); it is characterized by the relation
$$
\sum_{i=1}^m (a_i - g) = 0.
$$

### 3. AFFINE LINEAR VARIETIES

#### Definition 2 {#alg-ii-s9-def-2 .statement}

*Given an affine space* $E$, *a subset* $V$ *of* $E$ *is called an affine linear variety* (or simply a *linear variety* or an *affine subset* of $E$) *if, for every family* $(x_i)_{i \in I}$ *of points of* $V$ *and every family* $(\lambda_i)_{i \in I}$ *of elements of* $K$ *of finite support such that* $\sum_{i \in I} \lambda_i = 1$, *the barycentre* $\sum_{i \in I} \lambda_i x_i$ *belongs to* $V$.

It amounts to the same to say that the condition of Definition 2 holds for every *finite* family of points of $V$.

The empty set is a linear variety; every intersection of linear varieties is a linear variety.

Let $V$ be a non-empty subset of $E$ and $a$ a point of $V$; the relation
$$
x - a = \sum_{i=1}^n \lambda_i (x_i - a)
$$
means that $x$ is a barycentre $\sum_{i=1}^n \lambda_i x_i + \left(1 - \sum_{i=1}^n \lambda_i\right)a$ of the family consisting of the $x_i$ and $a$. Therefore:

#### Proposition 2 {#alg-ii-s9-prop-2 .statement}

*For a non-empty subset* $V$ *of an affine space* $E$ *to be a linear variety, it is necessary and sufficient that* $V$ *be a vector subspace for the vector space structure on* $E$ *obtained by taking a point of* $V$ *as origin.*

In particular, the non-empty affine linear varieties of a vector space $T$ (considered as an affine space) are just the *translates* of the vector subspaces of $T$; the vector subspaces of $T$ are therefore the linear varieties containing 0.

Let $V$ be a non-empty linear variety of the affine space $E$; the set of free vectors $x - y$, where $x$ and $y$ run through $V$, is a vector subspace $D$ of the translation space $T$ of $E$ called the *direction* of $V$: for, if $a \in V$, then
$$
x - y = (x - a) - (y - a)
$$
and our assertion follows from Proposition 2. It is immediate that $D$ operates faithfully and transitively on $V$, which therefore has canonically the structure of an *affine space attached to* $D$. By the *dimension* of the affine variety $V$, we mean the dimension of $V$ with this affine space structure, that is the dimension of the vector space $D$. The linear varieties of dimension 0 are the points of $E$; those of dimension 1 (resp. 2) are called *lines* (resp. *planes*) of $E$.

Every vector $\neq 0$ belonging to the direction of a line is called a *direction vector* of this line; its components with respect to a basis of T form what is called a system of *direction parameters* of the line in question.

The *codimension* of a linear variety V in E is the codimension of its direction D in T; a linear variety of codimension 1 in E is called an (affine) *hyperplane* of E.

Two linear varieties with the same direction are called *parallel*; it amounts to the same to say that one is derived from the other by translation. If V is a linear variety in T (considered as an affine space), its direction is the linear variety parallel to V and containing 0.

#### Proposition 3 {#alg-ii-s9-prop-3 .statement}

*Given a family* $(a_i)_{i \in I}$ *of points of an affine space* E, *the set* V *of barycentres* $\sum_{i \in I} \lambda_i a_i$ *((\lambda_i) of finite support, $\sum_{i \in I} \lambda_i = 1$) is a linear variety of* E.

If the family $(a_i)$ is empty, then $V = \varnothing$ because of the condition $\sum_i \lambda_i = 1$. It may therefore be assumed that the family $(a_i)$ is non-empty and in this case the proposition is obvious, taking one of the $a_i$ as origin in E.

The variety V is obviously the smallest linear variety containing the $a_i$; it is said to be *generated* by the family $(a_i)$ and this family is called a *generating system* of V.

In the notation of Proposition 3, assuming the family $(a_i)$ is non-empty, for the expression for every point $x \in V$ in the form $x = \sum_i \lambda_i a_i$ to be *unique*, it is necessary and sufficient that, denoting an arbitrary index of I by $\kappa$, the family of vectors $a_i - a_\kappa$, where $i$ runs through the set of indices $\neq \kappa$, be free in T. Then the family $(a_v)_{v \in I}$ of points of E is said to be *affinely free* (or that its elements form an *affinely free system*, or are *affinely independent*) and that $\lambda_i$ is the *barycentric coordinate* of $x$ of index $i$ with respect to the affinely free family $(a_i)$.

A family $(a_i)_{i \in I}$ of points of E which is not affinely free is said to be *affinely related*.

#### Proposition 4 {#alg-ii-s9-prop-4 .statement}

*For a non-empty family* $(a_i)_{i \in I}$ *of points in an affine space* E *to be affinely related, it is necessary and sufficient that there exist a family* $(\lambda_i)_{i \in I}$ *of elements not all zero in* K, *of finite support, such that* $\sum_{i \in I} \lambda_i = 0$ *and* $\sum_{i \in I} \lambda_i a_i = 0$.

Given an index $\kappa \in I$, to say that the family of vectors $(a_i - a_\kappa)$, where $i$ runs through the set of indices $\neq \kappa$, is related in T, means that there exists a family of scalars $(\lambda_i)_{i \neq \kappa}$ not all zero such that $\sum_{i \neq \kappa} \lambda_i (a_i - a_\kappa) = 0$, which may also be written $\sum_{i \in I} \lambda_i a_i = 0$, with $\lambda_\kappa = -\sum_{i \neq \kappa} \lambda_i$, in other words $\sum_{i \in I} \lambda_i = 0$.

#### Proposition 5 {#alg-ii-s9-prop-5 .statement}

For a non-empty family $(a_i)_{i \in I}$ of points of an affine space $E$ to be affinely free, it is necessary and sufficient that, for every index $\kappa \in I$, $a_\kappa$ do not belong to the linear variety generated by the $a_i$ of index $\neq \kappa$.

The proposition is obvious if $I$ has only a single element. Otherwise, taking as origin in $E$ one of the $a_i$ of index $\neq \kappa$, the proposition follows from § 7, no. 1, Remark.

### 4. AFFINE LINEAR MAPPINGS

#### Definition 3 {#alg-ii-s9-def-3 .statement}

Given two affine spaces $E, E'$ attached to two vector spaces $T, T'$ over the same field $K$, a mapping $u$ of $E$ into $E'$ is called an affine linear mapping (or an affine mapping) if, for every family $(x_i)_{i \in I}$ of points of $E$ and every family $(\lambda_i)_{i \in I}$ such that $\sum_{i \in I} \lambda_i = 1$,

$$
u\left( \sum_{i \in I} \lambda_i x_i \right) = \sum_{i \in I} \lambda_i u(x_i).
$$

(3)

#### Proposition 6 {#alg-ii-s9-prop-6 .statement}

Let $u$ be an affine mapping of $E$ into $E'$. There exists one and only one linear mapping $v$ of $T$ into $T'$ such that

$$
u(x + t) = u(x) + v(t)
$$

for all $x \in E, t \in T$.

Let $a$ be any point of $E$. The mapping

$$
t \mapsto u(a + t) - u(a)
$$

is a linear mapping $v_a$ of $T$ into $T'$, for we may write

$$
a + \lambda t = \lambda (a + t) + (1 - \lambda)a \\
a + s + t = (a + s) + (a + t) - a
$$

and it follows from (3) that $v_a(\lambda t) = \lambda v_a(t)$ and $v_a(s + t) = v_a(s) + v_a(t)$. Moreover, if $b$ is another point of $E$, then $v_a = v_b$; for the relation

$$
(a + t) - a + b = b + t
$$

implies

$$
u(a + t) - u(a) + u(b) = u(b + t)
$$

that is $u(a + t) - u(a) = u(b + t) - u(b)$. Whence the existence of $v$; the uniqueness is immediate.

$v$ is called the linear mapping of $T$ into $T'$ associated with $u$. Conversely, for every linear mapping $v$ of $T$ into $T'$ and every ordered pair of points $a \in E, a' \in E'$, it is immediately verified that

$$
x \mapsto a' + v(x - a)
$$

is an affine mapping of E into E' whose associated linear mapping is v. To say that u is an affine mapping of E into E' therefore also means that, if an arbitrary point a in E and the point u(a) in E' are taken as origins, u is a linear mapping for the two vector spaces thus obtained.

Let E'' be a third affine space, T'' its translation space, u' an affine mapping of E' into E'' and v' the linear mapping of T' into T'' associated with u'. Clearly u' o u is an affine mapping of E into E''; moreover, for a \in E and t \in T,
$$
u'(u(a + t)) = u'(u(a) + v(t)) = u'(u(a)) + v'(v(t))
$$
and hence v' o v is the linear mapping of T into T'' associated with u' o u. For an affine mapping u to be bijective, it is necessary and sufficient that the associated linear mapping v be so, and u^{-1} is then an affine mapping whose associated linear mapping is v^{-1}.

In particular, the affine bijections of E onto itself form a group G, called the affine group of E. The mapping which associates with u \in G the linear mapping v associated with u is, by the above, a homomorphism of G onto the linear group \mathbf{GL}(T). If u is a translation, v is the identity and conversely. Hence, the kernel of the above homomorphism is the translation group T of E which is therefore a normal subgroup of G.

If u \in G, the automorphism t \mapsto utu^{-1} of T (where t is identified with the translation x \mapsto x + t) is the linear mapping v associated with u. For x \in E and t \in T, by definition
$$
x + utu^{-1} = u(u^{-1}(x) + t) = u(u^{-1}(x)) + v(t) = x + v(t)
$$
and hence utu^{-1} = v(t).

Let a \in E and G_a be the subgroup of G consisting of the u \in G such that u(a) = a. If E is identified with T by taking a as origin, G_a is identified with \mathbf{GL}(T). Every u \in G can be expressed uniquely in the form u = t_1u_1 (resp. in the form u = u_2t_2), where u_1, u_2 are in G_a and t_1, t_2 in T: for, writing t_1 = u(a) - a, u^{-1}t_1 \in G_a, whence the existence of u_1 and t_1; the existence of u_2 and t_2 is obtained analogously. The uniqueness follows from the fact that G_a \cap T reduces to the identity element of G. Moreover
$$
t_1u_1 = u_1(u_1^{-1}t_1u_1)
$$
whence u_2 = u_1, t_2 = u_1^{-1}t_1u_1. Finally, the linear mappings associated with u and u_1 are the same and hence, if as above G_a is identified with \mathbf{GL}(T), u_1 is the linear mapping from T to itself associated with u. It is thus seen that G is the semi-direct product of G_a by T (I, § 6, no. 1).

Let E, E' be two affine spaces over K. The direct (resp. inverse) image of a linear variety of E (resp. E') under an affine mapping u of E into E' is a linear variety of E' (resp. E); the rank of u is by definition the dimension of u(E); it is equal to the rank of the linear mapping associated with u. If V, V' are linear varieties of the same finite dimension m in E, E' respectively, there exists an affine mapping $u$ of $E$ into $E'$ such that $u(V) = V'$: taking as origins in $E$ and $E'$ points of $V$ and $V'$ respectively, then taking in $E$ (resp. $E'$) a basis whose first $m$ vectors form a basis of $V$ (resp. $V'$), the proposition follows immediately from § 1, no. 11, Corollary 3 to Proposition 17.

As the field $K$ has canonically a left vector space structure (of dimension 1) over $K$, it can be considered as an affine space of dimension 1. An affine mapping of an affine space $D$ (over $K$) into the affine space $K$ is also called an *affine linear function* (or an *affine function*). If a point $a$ is taken as origin in $E$, every affine function on $E$ can then be written uniquely as $x \mapsto \alpha + v(x)$, where $\alpha \in K$ and $v$ is a linear form on the vector space $E$ thus obtained; the affine functions on $E$ therefore form a *right vector space over* $K$ of dimension $1 + \dim E$. If $u$ is a non-constant affine function on $E$ and $\lambda \in K$, the set of $x \in E$ satisfying the equation $u(x) = \lambda$ is a hyperplane; conversely, for every hyperplane $H$ in $E$, there exists an affine function $u_0$ on $E$ such that $H = u_0^{-1}(0)$ and every affine function $u$ such that $H = u^{-1}(0)$ is of the form $u_0 \mu$, where $\mu \in K$ (\S 7, no. 5, Proposition 11). If $u$ is an affine function on $E$, the hyperplanes with equations $u(x) = \alpha$ and $u(x) = \beta$ are parallel.

### 5. DEFINITION OF PROJECTIVE SPACES

#### Definition 4 {#alg-ii-s9-def-4 .statement}

*Given a left (resp. right) vector space* $V$ *over a field* $K$, *the left (resp. right) projective space derived from* $V$, *denoted by* $\mathbf{P}(V)$, *is the quotient of the complement* $V - \{0\}$ *of* $\{0\}$ *in* $V$ *by the equivalence relation* $\Delta(V)$ *"there exists* $\lambda \neq 0$ *in* $K$ *such that* $y = \lambda x$ *(resp.* $y = x \lambda$ )  *between* $x$ *and* $y$ *in* $V - \{0\}$.

When $V = K_s^{n+1}$, we also write $\mathbf{P}_n(K)$ instead of $\mathbf{P}(K_s^{n+1})$ and $\Delta_n(K)$ instead of $\Delta(V)$.

Definition 4 can also be expressed by saying that $\mathbf{P}(V)$ is the set of lines (passing through 0) in $V$ with the origin removed; $\mathbf{P}(V)$ is therefore canonically identified with the set of lines (passing through 0) in $V$. The elements of a projective space are called the *points* of that space.

When $V$ is of dimension $n$, the integer $n - 1$ is called the *dimension* of the projective space $\mathbf{P}(V)$ if $n$ is finite, and the cardinal $n$ otherwise; this cardinal is denoted by $\dim_K \mathbf{P}(V)$ or $\dim \mathbf{P}(V)$. Thus a projective space of dimension $-1$ is empty and a projective space of dimension 0 is a single point. A projective space of dimension 1 (resp. 2) is called a *projective line* (resp. *projective plane*).

Henceforth we shall only consider left projective spaces.

### 6. HOMOGENEOUS COORDINATES

Let $V$ be a vector space of finite dimension $n + 1$ over $K$, $\mathbf{P}(V)$ the projective space of dimension $n$ derived from $V$ and $(e_i)_{0 \leq i \leq n}$ a basis of $V$. Let $\pi$ denote the canonical mapping of $V - \{0\}$ onto the quotient set $\mathbf{P}(V)$. For every point $x = \sum_{i=0}^{n} \xi_i e_i$ of $V - \{0\}$, $(\xi_0, \xi_1, \ldots, \xi_n)$ is called a *system of homogeneous coordinates* of the point $\pi(x)$ with respect to the basis $(e_i)$ of $V$. Every system $(\xi_i)$ of $n + 1$ elements *not all zero* of $K$ is therefore a system of homogeneous coordinates of a point of $P(V)$ with respect to $(e_i)$; for two such systems $(\xi_i)$, $(\xi'_i)$ to be systems of homogeneous coordinates of the same point of $P(V)$ with respect to the same basis $(e_i)$, it is necessary and sufficient that there exists an element $\lambda \neq 0$ of $K$ such that $\xi'_i = \lambda \xi_i$ for $0 \leq i \leq n$.

This definition is immediately generalized to the case where $V$ is infinite-dimensional.

Given another basis $(\tilde{e}_i)$ of $V$ such that $e_i = \sum_{j=0}^{n} \alpha_{ij} \tilde{e}_j$ ($0 \leq i \leq n$) and a system $(\xi_i)$ of homogeneous coordinates of $\pi(x)$ with respect to the basis $(e_i)$, for a system $(\bar{\xi}_i)$ of $n + 1$ elements of $K$ to be a system of homogeneous coordinates of $\pi(x)$ with respect to the basis $(\tilde{e}_i)$, it is necessary and sufficient that there exist $\lambda \neq 0$ in $K$ such that

$$
\lambda \bar{\xi}_i = \sum_{j=0}^{n} \xi_j \alpha_{ji} \quad \text{for } 0 \leq i \leq n.
$$

In particular, if $e_i = \gamma_i \tilde{e}_i$ with $\gamma_i \neq 0$ ($0 \leq i \leq n$), then $\bar{\xi}_i = \mu \xi_i \gamma_i$ where $\mu \neq 0$.

### 7. PROJECTIVE LINEAR VARIETIES

Let $W$ be a vector subspace of a vector space $V$; the canonical image of $W - \{0\}$ in the projective space $P(V)$ derived from $V$ is called a *projective linear variety* (or simply a *linear variety* when no confusion is to be feared); as the equivalence relation $\Delta(W)$ on $W - \{0\}$ is induced by the relation $\Delta(V)$, the projective linear variety the image of $W - \{0\}$ in $P(V)$ can be identified with the projective space $P(W)$ derived from $W$ and hence we may speak of the dimension of such a variety. In a projective space $P(V)$, the canonical image of a hyperplane (with the origin removed) of $V$ is a linear variety called a *projective hyperplane* (or simply a *hyperplane*); if $P(V)$ is of finite dimension $n$ the hyperplanes in $P(V)$ are the linear varieties of dimension $n - 1$.

Every proposition concerning vector subspaces of a vector space goes over to a proposition concerning projective linear varieties. For example, if a projective space $P(V)$ is of finite dimension $n$ and $(e_i)_{0 \leq i \leq n}$ is a basis of $V$, every linear variety $L \subset P(V)$ of dimension $r$ can be defined by a system of $n - r$ homogeneous linear equations

$$
\sum_{i=0}^{n} \xi_i \alpha_{ij} = 0 \qquad (1 \leq j \leq n - r)
$$

between the homogeneous coordinates $\xi_i$ ($0 \leq i \leq n$) of a point of $\mathbf{P}(V)$ with respect to the basis $(e_i)$, the left hand sides of (4) being linearly independent forms on V. In particular, a projective hyperplane is defined by a single homogeneous linear equation with coefficients not all zero. Conversely, the points of $\mathbf{P}(V)$ satisfying an arbitrary system of homogeneous linear equations with respect to the $\xi_i$ form a linear variety L; if the system considered consists of $k \leq n + 1$ equations, L is of dimension $\geq n - k$.

Every intersection of linear varieties of $\mathbf{P}(V)$ is a linear variety; for every subset A of $\mathbf{P}(V)$, there exists a smallest linear variety L containing A; it is called the linear variety *generated by* A and A is called a *generating system* of L.

If W is the vector subspace of V generated by $\pi^{-1}(A)$, then $L = \mathbf{P}(W)$.

If L and M are any two linear varieties in $\mathbf{P}(V)$ and N the variety generated by $L \cup M$, then (\$ 7, no. 3, Corollary 3 to Proposition 4)

$$
\text{dim } L + \text{dim } M = \text{dim}(L \cap M) + \text{dim } N.
$$

In particular, if $\mathbf{P}(V)$ is finite-dimensional and $\text{dim } L + \text{dim } M \geq \text{dim } \mathbf{P}(V)$, it follows from (5) that $L \cap M$ is non-empty.

Let $(x_i), (y_i)$ be two families of points in the vector space V with the same indexing set, such that $y_i = \lambda_i x_i$, where $\lambda_i \neq 0$ for all $i$. If the family $(x_i)$ is free, so is $(y_i)$ and conversely; then it is said that the family of points $\pi(x_i)$ of $\mathbf{P}(V)$ is *projectively free* (or simply *free*). It amounts to the same to say that for every index $\kappa$, the point $\pi(x_\kappa)$ does not belong to the linear variety generated by the $\pi(x_i)$ for $i \neq \kappa$. A family of points of $\mathbf{P}(V)$ which is not projectively free is called *projectively related* (or simply *related*).

For a family $(x_i)$ of points of $V - \{0\}$ to be such that the family $(\pi(x_i))$ is projectively free and generates $\mathbf{P}(V)$, it is necessary and sufficient that $(x_i)$ be a basis of V. If $\mathbf{P}(V)$ is of dimension $n$ the number of elements in such a family is therefore $n + 1$. Note that giving such a family $(\pi(x_i))$ in $\mathbf{P}(V)$ does not determine (even to within a left factor) the homogeneous coordinates of a given point of $\mathbf{P}(V)$ with respect to a basis $(y_i)$ of V such that $\pi(y_i) = \pi(x_i)$ for all $i$ (cf. no. 6).

### 8. PROJECTIVE COMPLETION OF AN AFFINE SPACE

Let V be a (left) vector space over a field K and consider the vector space $K_s \times V$ over K; the projective space $\mathbf{P}(K_s \times V)$ is called the projective space *canonically associated* with the vector space V. If V is of dimension $n$, $\mathbf{P}(K_s \times V)$ is of the same dimension $n$. Consider in $K_s \times V$ the affine hyperplane $V_1 = \{1\} \times V$, whose direction (no. 3) is the subspace $V_0 = \{0\} \times V$; if a line (passing through 0) of $K_s \times V$ is not contained in $V_0$, it contains a point $(\alpha, x)$ with $\alpha \neq 0$ and $x \in V$, hence it contains also the point $\alpha^{-1}(\alpha, x) = (1, \alpha^{-1}x)$ of $V_1$; the converse is immediate and it is seen that there is a one-to-one correspondence between the points of $V_1$ and the lines (passing through 0) of $K_s \times V$ not contained in $V_0$, each of the latter meeting $V_1$ in one and only one point. It follows that the mapping $x \mapsto \phi(x) = \pi(1, x)$ is an injection (called canonical) of $V$ into the projective space $P(K_s \times V)$; $V$ is often identified with its image under this injection. The complement of $\phi(V)$ in $P(K_s \times V)$ is the projective hyperplane $P(V_0)$ called the hyperplane at infinity of $P(K_s \times V)$ (or of $V$, by an abuse of language); its points are also called the "points at infinity" of $P(K_s \times V)$ (or of $V$). If $(a_i)$ is a basis of $V$ and in $K_s \times V$ the basis is taken consisting of the elements $e_i = (0, a_i)$ and the element $e_\omega = (1, 0)$, the points at infinity in $P(K_s \times V)$ are those whose homogeneous coordinate of index $\omega$ is 0.

Let $M$ be an affine linear variety in $V$ (no. 3) and $D$ its direction; the canonical image $\phi(M)$ of $M$ in $P(K_s \times V)$ is contained in the canonical image $\overline{M} = \pi(M_2)$ of the vector subspace $M_2$ of $K_s \times V$ generated by the affine variety $M_1 = \{1\} \times M$ of $K_s \times V$. More precisely, if $(a_i)$ is an affinely free system of $M$ generating $M$, the elements $(1, a_i)$ form a basis of $M_2$ and therefore $\overline{M}$ is just the projective linear variety generated by $\phi(M)$; if $M$ is finite-dimensional, $\overline{M}$ has the same dimension as $M$. The complement of $\phi(M)$ in $\overline{M}$ is the intersection of $\overline{M}$ and the hyperplane at infinity and is equal to the canonical image $\pi(M_0)$, where $M_0 = \{0\} \times D$.

Conversely, let $N$ be a projective linear variety not contained in the hyperplane at infinity and let $R = \pi^{-1}(N)$; $R \cap V_1$ is an affine linear variety of $K \times V$ of the form $\{1\} \times M$, where $M$ is an affine linear variety of $V$ and it is immediately seen that $N$ is the affine linear variety $\overline{M}$ generated by $\phi(M)$.

There is therefore a one-to-one correspondence between the affine linear varieties of $V$ and the projective linear varieties of $P(K_s \times V)$ not contained in the hyperplane at infinity; for two affine linear varieties of $V$ to be parallel, it is necessary and sufficient that the projective linear varieties which they generate have the same intersection with the hyperplane at infinity (which is sometimes expressed by saying that the two affine linear varieties in question have the same points at infinity).

### 9. EXTENSION OF RATIONAL FUNCTIONS

If the results of no. 8 are applied to the vector space $V = K_s$ of dimension 1, it is seen that there exists a canonical injection $\phi$ of $K_s$ into the projective line $P_1(K) = P(K_s \times K_s)$; for all $\xi \in K$, $\phi(\xi)$ is the point with homogeneous coordinates $(1, \xi)$ with respect to the canonical basis (\$ 1, no. 11) of $K_s \times K_s$. The complement of $\phi(K)$ in $P_1(K)$ consists of the single point with homogeneous coordinates $(0, 1)$ with respect to the above basis; it is called the "point at infinity". $P_1(K)$ is also called the projective field associated with $K$ and denoted by $\tilde{K}$, the point at infinity in $\tilde{K}$ being denoted by $\infty$.

*Consider in particular the case where $K$ is a commutative field and let f \in K(X) be a rational function in one indeterminate over K (IV, § 4); if $f \neq 0$, there is a unique expression $f = \alpha p/q$, where $\alpha \in K^*$ and $p$ and $q$ are two relatively prime monic polynomials (VII, § 1); let $m$ and $n$ be their respective degrees and let $r = \sup(m, n)$. We write
$$
p_1(T, X) = T^r p(X/T), \qquad q_1(T, X) = T^r q(X/T);
$$
$p_1$ and $q_1$ are two homogeneous polynomials of degree $r$ over $K$ such that $p(X) = p_1(1, X)$, $q(X) = q_1(1, X)$. Hence, for every element $\xi \in K$ which is not a zero of $q(X)$, $f(\xi) = \alpha p(\xi)/q(\xi)$ is defined and we may write
$$
f(\xi) = \alpha p_1(1, \xi)/q_1(1, \xi) = \alpha p_1(\lambda, \lambda \xi)/q_1(\lambda, \lambda \xi)
$$
for all $\lambda \neq 0$ in $K$. Consider then the mapping
$$
(\eta, \xi) \mapsto (q_1(\eta, \xi), p_1(\eta, \xi))
$$
of $K^2$ into itself; it is compatible with the equivalence relation $\Delta(K^2)$ and therefore defines, when passing to the quotients, a mapping $\tilde{f}$ of $\tilde{K}$ into itself which coincides with $\xi \mapsto f(\xi)$ at the points where this rational function is defined; it is said, by an abuse of language, that $\tilde{f}$ is the canonical extension of $f$ to $\tilde{K}$.

For example, if $f = 1/X$, then $\tilde{f}(0) = \infty$ and $\tilde{f}(\infty) = 0$; if
$$
f = (aX + b)/(cX + d)
$$
with $ad - bc \neq 0$, then $\tilde{f}(-d/c) = \infty$, $\tilde{f}(\infty) = a/c$ if $c \neq 0$, $\tilde{f}(\infty) = \infty$ if $c = 0$. If $f = a_0 X^n + \cdots + a_n$ is a polynomial of degree $n > 0$, then $\tilde{f}(\infty) = \infty$*

### 10. PROJECTIVE LINEAR MAPPINGS

Let $V, V'$ be two left vector spaces over a field $K$, $f$ a linear mapping of $V$ into $V'$ and $N = \overline{f}(0)$ its kernel. It is immediate that the image under $f$ of a line (passing through 0) in $V$ not contained in $N$ is a line (passing through 0) in $V'$; hence, on passing to the quotients, $f$ defines a mapping $g$ of $P(V) - P(N)$ into $P(V')$. Such a mapping is called a projective linear mapping (or, simply, a projective mapping); although it is defined on $P(V) - P(N)$ and not on $P(V)$ (when $N \neq \{0\}$), we shall say by an abuse of language that $g$ is a projective mapping of $P(V)$ into $P(V')$. The projective linear variety $P(N)$, where $g$ is not defined, is called the centre of $g$.

Note that, when $g$ is defined on the whole of $P(V)$ (that is when $N = \{0\}$), $g$ is an injection of $P(V)$ into $P(V')$.

When bases $(a_\lambda)_{\lambda \in L}, (b_\mu)_{\mu \in M}$ are given in $V$ and $V'$ respectively, a projective mapping of $P(V)$ into $P(V')$ maps a point of $P(V)$ with homogeneous coordinates $\xi_\lambda$ ($\lambda \in L$) to a point of $\mathbf{P}(V')$ with a system of homogeneous coordinates $\eta_\mu$ ($\mu \in M$) of the form

$$
\eta_\mu = \sum_{\lambda \in L} \xi_\lambda \alpha_{\lambda \mu} \quad (\alpha_{\lambda \mu} \in K).
$$

The centre of $g$ is the linear variety defined by the equations

$$
\sum_{\lambda \in L} \xi_\lambda \alpha_{\lambda \mu} = 0 \quad (\mu \in M).
$$

If $C$ is the centre of $g$ and $M$ is a linear variety of $\mathbf{P}(V)$, the image under $g$ of $M - (M \cap C)$ is a linear variety of $\mathbf{P}(V')$ denoted (by an abuse of language) by $g(M)$. Then

$$
\dim g(M) + \dim(M \cap C) + 1 = \dim M
$$

(\S 7, no. 4, formula (12)). If $M'$ is a linear variety of $\mathbf{P}(V')$, $g^{-1}(M') \cup C$ is a linear variety of $\mathbf{P}(V)$ and

$$
\dim(g^{-1}(M') \cup C) = \dim C + \dim(M' \cap g(\mathbf{P}(V))) + 1.
$$

It is said, by an abuse of language, that $g^{-1}(M') \cup C$ is the *inverse image* of $M'$ under $g$.

As the values taken by a linear mapping on a basis $(e_i)$ of $V$ can be chosen arbitrarily in $V'$, it is seen that there exists a projective linear mapping of $\mathbf{P}(V)$ into $\mathbf{P}(V')$ taking *arbitrary* values at the points $\pi(e_i)$. But (even when $g$ is everywhere defined) giving $g(\pi(e_i))$ does not determine $g$ uniquely (Exercise 10).

The composition of two projective mappings which are bijections is a projective mapping; so is the inverse mapping of such a bijection. The bijective projective mappings of a projective space $\mathbf{P}(V)$ onto itself thus form a group, called the *projective group* of $\mathbf{P}(V)$ and denoted by $\mathbf{PGL}(V)$; we write $\mathbf{PGL}_n(K)$ or $\mathbf{PGL}(n, K)$ instead of $\mathbf{PGL}(K^n_s)$.

#### Remark {#alg-ii-s9-n10-rem-1 .statement}

In a projective space $\mathbf{P}(V)$ over a field $K$, let $H = \mathbf{P}(W)$ be a hyperplane. There exists a bijective linear mapping $f$ of $V$ onto $K_s \times W$ such that $f(W) = W$; let $g$ be the projective mapping obtained from $f$ by passing to the quotients. It has been seen (no. 8) that the complement of $\mathbf{P}(W)$ in $\mathbf{P}(K_s \times W)$ can be identified with an affine space whose translation space is $W$. When $\mathbf{P}(V)$ is identified with $\mathbf{P}(K_s \times W)$ by means of $g$, it is said that $H$ *has been taken as hyperplane at infinity* in $\mathbf{P}(V)$; the complement of $H$ in $\mathbf{P}(V)$ is then identified with an affine space whose translation space is $W$.

### 11. PROJECTIVE SPACE STRUCTURE

Given a set E and a field K, a (left) projective space structure on E with respect to the field K is defined by giving a non-empty set $\Phi$ of bijections of subsets of the projective space $\mathbf{P}(K_s^{(E)})$ onto E satisfying the following axioms:

$$(\mathrm{EP}_I)$$ *The set of definition of every mapping $f \in \Phi$ is a linear variety of $\mathbf{P}(K_s^{(E)})$.*

$$(\mathrm{EP}_{II})$$ *For every ordered pair of elements $f, g$ of $\Phi$ defined respectively on the linear varieties $\mathbf{P}(V)$ and $\mathbf{P}(W)$, the bijection $h = g^{-1} \circ f$ of $\mathbf{P}(V)$ onto $\mathbf{P}(W)$ is a projective mapping.*

$$(\mathrm{EP}_{III})$$ *Conversely, if $f \in \Phi$ is defined on the linear variety $\mathbf{P}(V)$ and $h$ is a bijective projective mapping of $\mathbf{P}(V)$ onto a linear variety $\mathbf{P}(W) \subset \mathbf{P}(K_s^{(E)})$, then $f \circ h^{-1} \in \Phi$.*

Let E be a set, $(V_\lambda)_{\lambda \in L}$ a family of vector spaces over K and suppose given for each $\lambda \in L$ a bijection $f_\lambda$ of $\mathbf{P}(V_\lambda)$ onto E such that, for every ordered pair of indices $\lambda, \mu, f_\lambda^{-1} \circ f_\mu$ is a *projective mapping* of $\mathbf{P}(V_\mu)$ onto $\mathbf{P}(V_\lambda)$. Then we can define on E a projective space structure with respect to K as follows: let $(e_i)_{i \in I}$ be a basis of a space $V_\lambda$ and write $a_i = f_\lambda(\pi(e_i))$; let $b_i$ be the element of index $a_i$ in the canonical basis of $K_s^{(E)}$ (\S 1, no. 11). The relation $i \neq \kappa$ implies $b_i \neq b_\kappa$ because of the hypothesis that $f_\lambda$ is bijective; hence the $b_i$ form a basis of a vector subspace $W_0$ of $K_s^{(E)}$ and there therefore exists a bijective projective mapping $h$ of $\mathbf{P}(W_0)$ onto $\mathbf{P}(V_\lambda)$ such that $h(\pi(b_i)) = \pi(e_i)$ for all $i \in I$. If $\Phi$ is taken to be the set of all bijective projective mappings $f_\lambda \circ h \circ g^{-1}$, where $g$ runs through the set of all bijective projective mappings $\mathbf{P}(W) \subset \mathbf{P}(K_s^{(E)})$, it is immediately verified that $\Phi$ satisfies axioms (EP_I), (EP_{II}) and (EP_{III}). It is moreover immediate that $\Phi$ depends neither on the choice of index $\lambda \in L$, nor on the choice of basis $(e_i)$ in $V_\lambda$, nor on the choice of $h$.

In particular (taking L to consist of a single element), every projective space $\mathbf{P}(V)$ derived from a vector space V (no. 5, Definition 4) thus has a well determined "projective space structure" in the sense of the definition given in this no. Hence any set with a projective space structure can be called a *projective space*.

With the same notation, a *linear variety* in a projective space E is a subset M of E such that, for at least *one* bijection $f \in \Phi$ defined on $\mathbf{P}(V) \subset \mathbf{P}(K_s^{(E)})$, $f^{-1}(M)$ is a linear variety in $\mathbf{P}(V)$ in the sense of no. 7 (this property then holds for *all* $f \in \Phi$). It follows from the above that every linear variety in a projective space has canonically a projective space structure.

A projective space E is said to be *of dimension n* if, for all $f \in \Phi, f^{-1}(E)$ is a linear variety of dimension n (it suffices that this hold for *one* mapping $f \in \Phi$).

### Exercises {#alg-ii-s9-exercises}

See the [exercises for § 9](exercises/s9/).
