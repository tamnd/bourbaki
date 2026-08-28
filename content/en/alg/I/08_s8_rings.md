---
book: alg
book_title: Algebra
chapter: I
chapter_title: ALGEBRAIC STRUCTURES
section: 8
section_title: Rings
lang: en
source: alg-i-iii
source_edition: 1998, Springer
pdf_pages: 0120-0138, 0195-0198
extraction: ocr
subsections:
    - "no": 1
      title: RINGS
      page: 0
      pdf_page: 120
    - "no": 2
      title: CONSEQUENCES OF DISTRIBUTIVITY
      page: 0
      pdf_page: 122
    - "no": 3
      title: EXAMPLES OF RINGS
      page: 0
      pdf_page: 125
    - "no": 4
      title: RING HOMOMORPHISMS
      page: 0
      pdf_page: 126
    - "no": 5
      title: SUBRINGS
      page: 0
      pdf_page: 127
    - "no": 6
      title: IDEALS
      page: 0
      pdf_page: 127
    - "no": 7
      title: QUOTIENT RINGS
      page: 0
      pdf_page: 129
    - "no": 8
      title: SUBRINGS AND IDEALS IN A QUOTIENT RING
      page: 0
      pdf_page: 130
    - "no": 9
      title: MULTIPLICATION OF IDEALS
      page: 0
      pdf_page: 131
    - "no": 10
      title: PRODUCT OF RINGS
      page: 0
      pdf_page: 132
    - "no": 11
      title: DIRECT DECOMPOSITION OF A RING
      page: 0
      pdf_page: 134
    - "no": 12
      title: RINGS OF FRACTIONS
      page: 0
      pdf_page: 136
statements: 31
exercises: 16
content_sha256: 82f3b9f6c044b6246eb0c2be0d3c2c67423e560bf34edc83e7cf960aed7cd234
---

## § 8. RINGS

### 1. RINGS

#### Definition 1 {#alg-i-s8-def-1 .statement}

*A ring is a set* $\mathbf{A}$ *with two laws of composition called respectively addition and multiplication, satisfying the following axioms*:

(AN I) *Under addition* $\mathbf{A}$ *is a commutative group*.
(AN II) *Multiplication is associative and possesses an identity element*.
(AN III) *Multiplication is distributive with respect to addition*.
*The ring* $\mathbf{A}$ *is said to be commutative if its multiplication is commutative*.

In what follows, $(x, y) \mapsto x + y$ denotes addition and $(x, y) \mapsto xy$ multiplication; $0$ denotes the identity element for addition and $1$ that for multiplication. Finally, $-x$ denotes the negative of $x$ under addition. The axioms of a ring are therefore expressed by the following identities:

$$
\begin{array}{ll}
(1) & x + (y + z) = (x + y) + z \quad \text{(associativity of addition)} \\
(2) & x + y = y + x \quad \text{(commutativity of addition)} \\
(3) & 0 + x = x + 0 = x \quad \text{(zero)} \\
(4) & x + (-x) = (-x) + x = 0 \quad \text{(negative)} \\
(5) & x(yz) = (xy)z \quad \text{(associativity of multiplication)} \\
(6) & x.1 = 1.x = x \quad \text{(unit element)} \\
(7) & (x + y).z = xz + yz \\
(8) & x.(y + z) = xy + xz \quad \text{(distributivity)}
\end{array}
$$

Finally the ring $\mathbf{A}$ is commutative if $xy = yx$ for $x, y$ in $\mathbf{A}$.

With addition alone $\mathbf{A}$ is a commutative group called the *additive group* of $\mathbf{A}$. For all $x \in \mathbf{A}$, we define the left homothety $\gamma_x$ and right homothety $\delta_x$ by $\gamma_x(y) = xy$, $\delta_x(y) = yx$. By formulae (7) and (8), $\gamma_x$ and $\delta_x$ are endomorphisms of the additive group of $\mathbf{A}$ and thus map zero to zero and negative to negative. Therefore

$$
\begin{align*}
(9) & \quad x.0 = 0.x = 0 \\
(10) & \quad x.(-y) = (-x).y = -xy;
\end{align*}
$$
it follows that $(-x)(-y) = -((-x).y) = -(-xy)$, whence
$$(11) \quad (-x)(-y) = xy.$$
Formulae (10) and (11) constitute the *sign rule*. It follows that
$$-x = (-1)x = x(-1)$$
and $(-1)(-1) = 1$.

From (11) it follows by induction on $n$ that
$$(12) \quad (-x)^n = \begin{cases} x^n & \text{if } n \text{ is even} \\ -x^n & \text{if } n \text{ is odd.} \end{cases}$$

When we speak of *cancellable* elements, *invertible* elements, *permutable* elements, *central* elements, *centralizer* or *centre* of a ring $\mathbf{A}$, all these notions will refer to the multiplication on $\mathbf{A}$. If $x, y \in \mathbf{A}$ and $y$ is invertible, the element $xy^{-1}$ of $\mathbf{A}$ is also denoted by $x/y$ when $\mathbf{A}$ is commutative. The set of invertible elements of $\mathbf{A}$ is stable under multiplication. Under the law induced by multiplication it is a group called the *multiplicative group* of $\mathbf{A}$, sometimes denoted by $\mathbf{A}^*$.

Let $x, y$ be in $\mathbf{A}$. $x$ is said to be a *left* (resp. *right*) *multiple* of $y$ if there exists $y' \in \mathbf{A}$ such that $x = y'y$ (resp. $x = yy'$); it is also said that $y$ is a *right* (resp.

left) divisor of x. When A is commutative, there is no need to distinguish between "left" and "right".

In conformity with the above terminology, every element $y \in \mathbf{A}$ would be considered as a right and left divisor of 0; but, by an abuse of language, in general the term "right (resp. left) divisor of 0" is reserved for elements $y$ such that there exists $x \neq 0$ in A satisfying the relation $xy = 0$ (resp. $yx = 0$). In other words, the right (resp. left) divisors of zero are the right (resp. left) non-cancellable elements.

Let $x \in \mathbf{A}$. $x$ is called nilpotent if there exists an integer $n > 0$ with $x^n = 0$. The element $1 - x$ is then invertible, with inverse equal to
$$
1 + x + x^2 + \cdots + x^{n-1}.
$$

As A is a commutative group under addition, the element $nx$ for $n \in \mathbf{Z}$ and $x \in \mathbf{A}$ has been defined (§ 2, no. 8). As $\gamma_x$ and $\delta_x$ are endomorphisms of the additive group A, $\gamma_x(ny) = n\gamma_x(y)$ and $\delta_y(nx) = n\delta_y(x)$, whence
$$
x.(ny) = (nx).y = n.(xy).
$$
In particular, $nx = (n.1)x$.

A set A with addition and multiplication satisfying the axioms of a ring with the exception of that assuring the existence of the identity element under multiplication, is called a pseudo-ring.

### 2. CONSEQUENCES OF DISTRIBUTIVITY

Distributivity of multiplication with respect to addition allows us to apply Proposition 1 of § 3, no. 4, which gives
$$
\prod_{i=1}^n \left( \sum_{\lambda \in L_i} x_{i,\lambda} \right) = \sum_{\alpha_1, \ldots, \alpha_n} \prod_{i=1}^n x_{i, \alpha_i}
$$
where the sum extends over all sequences $(\alpha_1, \ldots, \alpha_n)$ belonging to $L_1 \times \cdots \times L_n$ and for $i = 1, \ldots, n$ the family $(x_{i,\lambda})_{\lambda \in L_i}$ of elements of the ring A is of finite support.

#### Proposition 1 {#alg-i-s8-prop-1 .statement}

Let A be a commutative ring and $(x_\lambda)_{\lambda \in L}$ a finite family of elements of A. For every family of positive integers $\beta = (\beta_\lambda)_{\lambda \in L}$, let $|\beta| = \sum_{\lambda \in L} \beta_\lambda$. Then
$$
\left( \sum_{\lambda \in L} x_\lambda \right)^n = \sum_{|\beta|=n} \frac{n!}{\prod_{\lambda \in L} \beta_\lambda!} \prod_{\lambda \in L} x_\lambda^{\beta_\lambda}.
$$
We apply formula (13) with $L_i = L$ and $x_{i,\lambda} = x_\lambda$ for $1 \leq i \leq n$. Then
$$
\left( \sum_{\lambda \in L} x_\lambda \right)^n = \sum_{\alpha_1, \ldots, \alpha_n} x_{\alpha_1} \cdots x_{\alpha_n},
$$
the sum extending over all sequences $\alpha = (\alpha_1, \ldots, \alpha_n) \in L^n$.

Let $\alpha$ be in $L^n$; for all $\lambda \in L$ let $U_\lambda^\alpha$ denote the set of integers $i$ such that $1 \leq i \leq n$ and $\alpha_i = \lambda$ and let $\Phi(\alpha) = (U_\lambda^\alpha)_{\lambda \in L}$. It is immediate that $\Phi$ is a bijection of $L^n$ onto the set of partitions of $\{1, 2, \ldots, n\}$ indexed by $L$. For all $\beta \in \mathbf{N}^L$ such that $|\beta| = n$, let $L_\beta^n$ denote the set of $\alpha \in L^n$ such that $\mathrm{Card}\ U_\beta^\alpha = \beta_\lambda$ for all $\lambda \in L$. It follows that the family $(L_\beta^n)_{|\beta|=n}$ is a partition of $L^n$ and that

$$
\mathrm{Card}\ L_\beta^n = \frac{n!}{\prod_{\lambda \in L} \beta_\lambda!}
$$

(§ 5, no. 5).

Finally, for $\alpha \in L_\beta^n$,

$$
x_{\alpha_1} \cdots x_{\alpha_n} = \prod_{\lambda \in L} \prod_{i \in U_\lambda^\alpha} x_{\alpha_i} = \prod_{\lambda \in L} \prod_{i \in U_\lambda^\alpha} x_\lambda = \prod_{\lambda \in L} x_\lambda,
$$

whence

$$
\sum_{(\alpha_1, \ldots, \alpha_n)} x_{\alpha_1} \cdots x_{\alpha_n} = \sum_{|\beta|=n} \sum_{\alpha \in L_\beta^n} x_{\alpha_1} \cdots x_{\alpha_n}
= \sum_{|\beta|=n} \sum_{\alpha \in L_\beta^n} \prod_{\lambda \in L} x_\lambda^{\beta_\lambda}
= \sum_{|\beta|=n} \frac{n!}{\prod_{\lambda \in L} \beta_\lambda!} x_\lambda^{\beta_\lambda}
$$

and formula (14) thus follows from (15).

#### Corollary 1 (binomial formula) {#alg-i-s8-prop-1-cor-1 .statement}

*Let x and y be two elements of a commutative ring A. Then*:

$$
(x + y)^n = \sum_{p=0}^n \binom{n}{p} x^p y^{n-p}.
$$

Formula (14) applied to $L = \{1, 2\}$, $x_1 = x$ and $x_2 = y$ gives

$$
(x + y)^n = \sum_{p+q=n} \frac{n!}{p! q!} x^p y^q,
$$

the sum extending over ordered pairs of positive integers $p, q$ with $p + q = n$. The binomial formula follows immediately from this (*Set Theory*, III, § 5, no. 8).

#### Corollary 2 {#alg-i-s8-prop-1-cor-2 .statement}

*Let A be a commutative ring, X a set, $\mathbf{u} = (u_x)_{x \in X}$ and $\mathbf{v} = (v_x)_{x \in X}$ two families of elements of A. Let $\mathbf{u} + \mathbf{v}$ denote the family $(u_x + v_x)_{x \in X}$. For all $\lambda \in \mathbf{N}^{(X)}$ we write $\lambda! = \prod_{x \in X} \lambda(x)!$. Then for all $\alpha \in \mathbf{N}^{(X)}$, in the notation of § 7, no. 8,

$$
(\mathbf{u} + \mathbf{v})^\alpha = \sum_{\beta + \gamma = \alpha} \frac{\alpha!}{\beta! \gamma!} \mathbf{u}^\beta \mathbf{v}^\gamma.
$$

For $x \in X$,

$$
(u_x + v_x)^{\alpha(x)} = \sum_{m+n=\alpha(x)} \frac{\alpha(x)!}{m! n!} u_x^m v_x^n
$$

by Corollary 1. Taking the product of these equations for $x \in X$ and using (13), we obtain the corollary.

#### Proposition 2 {#alg-i-s8-prop-2 .statement}

*Let $A$ be a ring, $x_1, \ldots, x_n$ elements of $A$ and $I = \{1, 2, \ldots, n\}$. For $H \subset I$, we write $x_H = \sum_{i \in H} x_i$. Then*

$$
(-1)^n \sum_{\sigma \in S_n} x_{\sigma(1)} \cdots x_{\sigma(n)} = \sum_{H \subset I} (-1)^{\mathrm{Card}\, H}(x_H)^n.
$$

*In particular, if $A$ is commutative,

$$
(-1)^n n! x_1 x_2 \cdots x_n = \sum_{H \subset I} (-1)^{\mathrm{Card}\, H}(x_H)^n.
$$

Let $C$ be the set of mappings of $I$ into $\{0, 1\}$. If each $H \subset I$ is mapped to its characteristic function, a bijection is obtained of $\mathcal{P}(I)$ onto $C$. The right hand side of (16) is thus equal to:

$$
\sum_{a \in C} (-1)^{a(1)+\cdots+a(n)} \left( \sum_{i \in I} a(i) x_i \right)^n
$$
$$
= \sum_{a \in C} (-1)^{a(1)+\cdots+a(n)} \sum_{(i_1, \ldots, i_n) \in I^n} a(i_1) \ldots a(i_n) x_{i_1} \ldots x_{i_n}
$$
$$
= \sum_{(i_1, \ldots, i_n) \in I^n} c_{i_1 \ldots i_n} x_{i_1} \ldots x_{i_n}
$$

where

$$
c_{i_1 \ldots i_n} = \sum_{a \in C} (-1)^{a(1)+\cdots+a(n)} a(i_1) \ldots a(i_n).
$$

(1) Suppose that $(i_1, \ldots, i_n)$ is not a permutation of $I$. There exists a $j \in I$ distinct from $i_1, \ldots, i_n$. Let $C'$ be the set of $a \in C$ such that $a(j) = 0$. For all $a \in C'$, let $a^*$ be the sum of $a$ and the characteristic function of $\{j\}$. Then $a^*(1) + \cdots + a^*(n) = a(1) + \cdots + a(n) + 1$ and hence

$$
c_{i_1 \ldots i_n} = \sum_{a \in C'} (-1)^{a(1)+\cdots+a(n)} a(i_1) \ldots a(i_n) + (-1)^{a^*(1)+\cdots+a^*(n)} a^*(i_1) \ldots a^*(i_n)
$$
$$
= \sum_{a \in C'} ((-1)^{a(1)+\cdots+(n)} + (-1)^{a(1)+\cdots+a(n)+1}) a(i_1) \ldots a(i_n) = 0.
$$

(2) Suppose that there exists $\sigma \in S_n$ such that $i_1 = \sigma(1), \ldots, i_n = \sigma(n)$. Then $a(i_1) \ldots a(i_n) = 0$ unless $a$ only takes the value 1. Thus $c_{i_1 \ldots i_n} = (-1)^n$.

### 3. EXAMPLES OF RINGS

I. Zero ring. Let A be a ring. For $0 = 1$ in A, it is necessary and sufficient that A consist of a single element. The condition is obviously sufficient. On the other hand, if $0 = 1$, then, for all $x \in A$, $x = x.1 = x.0 = 0$. Such a ring is called a zero ring.

II. Ring of rational integers. With the addition defined in § 2, no. 5, and the multiplication defined in § 2, no. 6, $\mathbf{Z}$ is a commutative ring. The notation 0, 1, $-x$ is in accordance with the notation introduced earlier.

*III. Ring of real-valued functions. Let I be an interval in the set $\mathbf{R}$ of real numbers and let A be the set of continuous functions defined on I with real values. The sum $f + g$ and product $f.g$ of two functions $f$ and $g$ are defined by
$$(f + g)(t) = f(t) + g(t), \quad (fg)(t) = f(t)g(t) \quad (t \in I).$$
A commutative ring is obtained whose unit element is the constant 1.*

*IV. Convolution pseudo-ring. Let E be the set of real-valued continuous functions on $\mathbf{R}$, which are zero outside a bounded interval. The sum of two functions is defined as in III, but the product is now defined by
$$(fg)(t) = \int_{-\infty}^{\infty} f(s)g(t-s)\ ds$$
("convolution product"). Thus a commutative pseudo-ring is obtained which is not a ring (cf. Integration, VIII, §4).*

V. Opposite ring of a ring A. Let A be a ring. The set A with the same addition as A and the multiplication $(x, y) \mapsto yx$ is often denoted by $A^0$. It is a ring (called the opposite ring of A) with the same zero and same unit as A and which coincides with A if and only if A is commutative.

VI. Endomorphism ring of a commutative group. Let G be a commutative group written additively. Let E denote the set of endomorphisms of G. Given $f$ and $g$ in E, the mappings $f + g$ and $fg$ of G into G are defined by
$$(f + g)(x) = f(x) + g(x), \quad (fg)(x) = f(g(x)) \quad (x \in G).$$
By § 1, no. 5, Proposition 5, $f + g$ is an endomorphism of G and so obviously also is $fg = f \circ g$. By § 4, no. 8, E is a (commutative) group under addition. Multiplication is obviously associative and has identity element $\mathrm{Id}_G$. Also for $f, g$ and $h$ in E, we write $\phi = f.(g + h)$; for all $x \in G$,
$$\phi(x) = f((g + h)(x)) = f(g(x) + h(x)) = f(g(x)) + f(h(x))$$
for $f$ is an endomorphism of G; hence $\phi = fg + fh$ and clearly
$$(g + h)f = gf + hf.$$

Therefore E is a (not in general commutative) ring called the *endomorphism ring of G*.

VII. *Pseudo-ring of zero square.* A pseudo-ring A is said to be of zero square if $xy = 0$ for all $x, y \in A$. Let G be a commutative group. If the set G is given the addition of the group G and multiplication $(x, y) \mapsto 0$, a pseudo-ring of zero square is obtained. It is only a ring if $G = \{0\}$, in which case it is the zero ring.

### 4. RING HOMOMORPHISMS

#### Definition 2 {#alg-i-s8-def-2 .statement}

*Let A and B be two rings. A morphism, or homomorphism, of A into B is any mapping f of A into B satisfying the relations:*

$$
f(x + y) = f(x) + f(y), \quad f(xy) = f(x) \cdot f(y), \quad f(1) = 1,
$$

*for all* $x, y$ *in A*.

The composition of two ring homomorphisms is a ring homomorphism. Let A and B be two rings and $f$ a mapping of A into B; for $f$ to be an isomorphism, it is necessary and sufficient that it be a bijective homomorphism; in that case, $f^{-1}$ is a homomorphism of B into A. A homomorphism of a ring A into itself is called an *endomorphism* of A.

Let $f : A \to B$ be a ring homomorphism. The mapping $f$ is a homomorphism of the additive group of A into the additive group of B; in particular, $f(0) = 0$ and $f(-x) = -f(x)$ for all $x \in A$. The image under $f$ of an invertible element of A is an invertible element of B and $f$ induces a homomorphism of the multiplicative group of A into the multiplicative group of B.

#### Example {#alg-i-s8-n4-exa-1 .statement}

(1) Let A be a ring. It is immediately seen that the mapping $n \mapsto n \cdot 1$ of $\mathbf{Z}$ into A is the unique homomorphism of $\mathbf{Z}$ into A. In particular, the identity mapping of $\mathbf{Z}$ is the unique endomorphism of the ring $\mathbf{Z}$.

In particular, take A to be the endomorphism ring of the additive group $\mathbf{Z}$ (no. 3, Example VI). The mapping $n \mapsto n \cdot 1$ of $\mathbf{Z}$ into A is an isomorphism of $\mathbf{Z}$ onto A by the very construction of multiplication in $\mathbf{Z}$ (§ 2, no. 6).

(2) Let $a$ be an invertible element of a ring A. The mapping $x \mapsto axa^{-1}$ is an endomorphism of A for

$$
a(x + y)a^{-1} = axa^{-1} + aya^{-1},
$$
$$
a(xy)a^{-1} = (axa^{-1})(aya^{-1}).
$$

It is bijective, for the relation $x' = axa^{-1}$ is equivalent to $x = a^{-1}x'a$. It is therefore an automorphism of the ring A, called the *inner automorphism* associated with $a$.

### 5. SUBRINGS

#### Definition 3 {#alg-i-s8-def-3 .statement}

Let $A$ be a ring. A subring of $A$ is any subset $B$ of $A$ which is a subgroup of $A$ under addition, which is stable under multiplication and which contains the unit of $A$.

The above conditions may be written as follows

$$
0 \in B, \quad B + B \subset B, \quad -B \subset B, \quad B.B \subset B, \quad 1 \in B.
$$

If $B$ is a subring of $A$, it is given the addition and multiplication induced by those on $A$, which make it into a ring. The canonical injection of $B$ into $A$ is a ring homomorphism.

#### Example {#alg-i-s8-n5-exa-1 .statement}

(1) Every subgroup of the additive group $\mathbf{Z}$ which contains 1 is equal to $\mathbf{Z}$. Thus $\mathbf{Z}$ is the only subring of $\mathbf{Z}$.

(2) Let $A$ be a ring and $(A_t)_{t \in I}$ a family of subrings of $A$; it is immediate that $\bigcap_{t \in I} A_t$ is a subring of $A$. In particular, the intersection of the subrings of $A$ containing a subset $X$ of $A$ is a subring called the subring of $A$ generated by $X$.

(3) Let $X$ be a subset of a ring $A$. The centralizer of $X$ in $A$ is a subring of $A$. In particular, the centre of $A$ is a subring of $A$.

(4) Let $G$ be a commutative group with operators; let $\Omega$ denote the set of operators and $\alpha \mapsto f_\alpha$ the action of $\Omega$ on $G$. Let $E$ be the endomorphism ring of the group without operators $G$ and $F$ the set of endomorphisms of the group with operators $G$. By definition, $F$ consists of the endomorphisms $\phi$ of $G$ such that $\phi \cdot f_\alpha = f_\alpha \cdot \phi$ for all $\alpha \in \Omega$. Therefore $F$ is a subring of the ring $E$. $F$ is called the endomorphism ring of the group with operators $G$ (cf. II, § 1, no. 2). Let $F_1$ be the subring of $E$ generated by the $f_\alpha$. Then $F$ is the centralizer of $F_1$ in $E$.

### 6. IDEALS

#### Definition 4 {#alg-i-s8-def-4 .statement}

Let $A$ be a ring. A subset $a$ of $A$ is called a left (resp. right) ideal if it is a subgroup of the additive group of $A$ and the relations $a \in A, x \in a$ imply $ax \in a$ (resp. $xa \in a$). $a$ is called a two-sided ideal of $A$ if it is both a left ideal and a right ideal of $A$.

The definition of a left ideal may be expressed by the relations

$$
0 \in a, \quad a + a \subset a, \quad A.a \subset a
$$

the relation $-a \subset a$ following from the formula $(-1).x = -x$ and $A.a \subset a$. For all $x \in A$, let $\gamma_x$ be the mapping $a \mapsto xa$ of $A$ into $A$; the action $x \mapsto \gamma_x$ gives the additive group $A^+$ of $A$ the structure of a group with operators with $A$ as set of operators. The left ideals of $A$ are just the subgroups of $A^+$ which are stable under this action.

The left ideals in the ring $A$ are just the right ideals of the opposite ring $A^0$. In a commutative ring the three species of ideals are the same; they are simply called ideals.

#### Example {#alg-i-s8-n6-exa-1 .statement}

(1) Let $A$ be a ring. The set $A$ is a two-sided ideal of $A$; so is the set consisting of 0, which is called the zero ideal and sometimes denoted by 0 or $(0)$ instead of $\{0\}$.

(2) For every element $a$ of $A$, the set $A.a$ of left multiples of $a$ is a left ideal; similarly the set $a.A$ is a right ideal. When $a$ is in the centre of $A$, $A.a = a.A$; this ideal is called the principal ideal generated by $a$ and is denoted by $(a)$. $(a) = A$ if and only if $a$ is invertible.

(3) Let $M$ be a subset of $A$. The set of elements $x \in A$ such that $xy = 0$ for all $y \in M$ is a left ideal of $A$ called the left annihilator of $M$. The right annihilator of $M$ is defined similarly.

(4) Every intersection of left (resp. right, two-sided) of $A$ is a left (resp. right, two-sided) ideal. Given a subset $X$ of $A$, there thus exists a smallest left (resp. right, two-sided) ideal containing $X$; it is called the left (resp. right, two-sided) ideal generated by $X$.

Let $a$ be a left ideal of $A$. The conditions $1 \notin a, a \neq A$ are obviously equivalent.

#### Definition 5 {#alg-i-s8-def-5 .statement}

*Let $A$ be a ring. By an abuse of language, a left ideal $a$ is said to be maximal if it is a maximal element of the set of left ideals distinct from $A$.*

In other words, $a$ is maximal if $a \neq A$ and the only left ideals of $A$ containing $a$ are $a$ and $A$.

Theorem 1 (Krull). *Let $A$ be a ring and $a$ a left ideal of $A$ distinct from $A$. There exists a maximal ideal $m$ of $A$ containing $a$.*

Consider $A$ as operating on the additive group $A^+$ of $A$ by left multiplication. Then the left ideals of $A$ are the stable subgroups of $A^+$. The theorem thus follows from § 4, no. 3, Proposition 3 applied to the subset $P = \{1\}$ of $A^+$.

#### Proposition 3 {#alg-i-s8-prop-3 .statement}

*Let $A$ be a ring, $(x_\lambda)_{\lambda \in L}$ a family of elements of $A$ and $a$ (resp. $b$) the set of sums $\sum_{\lambda \in L} a_\lambda x_\lambda$ where $(a_\lambda)_{\lambda \in L}$ is a family with finite support of elements of $A$ (resp. $\sum_{\lambda \in L} a_\lambda x_\lambda b_\lambda$ where $(a_\lambda)_{\lambda \in L}, (b_\lambda)_{\lambda \in L}$ are families with finite support of elements of $A$). Then $a$ (resp. $b$) is the left (resp. two-sided) ideal of $A$ generated by the elements $x_\lambda$.

The formulae

$$
0 = \sum_{\lambda \in L} 0.x_\lambda
$$
$$
\sum_{\lambda \in L} a_\lambda x_\lambda + \sum_{\lambda \in L} a'_\lambda x_\lambda = \sum_{\lambda \in L} (a_\lambda + a'_\lambda)x_\lambda
$$
$$
a.\sum_{\lambda \in L} a_\lambda x_\lambda = \sum_{\lambda \in L} (aa_\lambda)x_\lambda
$$

prove that $a$ is a left ideal. Let $a'$ be a left ideal such that $x_\lambda \in a'$ for all $\lambda \in L$ and let $(a_\lambda)_{\lambda \in L}$ be a family with finite support in $A$. Then $a_\lambda x_\lambda \in a'$ for all $\lambda \in L$, whence $\sum_{\lambda \in L} a_\lambda x_\lambda \in a'$; hence $a \subset a'$. Hence $a$ is the left ideal of $A$ generated by the $x_\lambda$. The argument for $b$ is analogous.

#### Proposition 4 {#alg-i-s8-prop-4 .statement}

*Let $A$ be a ring and $(a_\lambda)_{\lambda \in L}$ a family of left ideals of $A$. The left ideal generated by $\bigcup_{\lambda \in L} a_\lambda$ consists of the sums $\sum_{\lambda \in L} y_\lambda$ where $(y_\lambda)_{\lambda \in L}$ is a family with finite support such that $y_\lambda \in a_\lambda$ for all $\lambda \in L$.*

Let $a$ be the set of sums $\sum_{\lambda \in L} y_\lambda$ with $y_\lambda \in a_\lambda$ for all $\lambda \in L$. The formulae $\sum_{\lambda \in L} x_\lambda + \sum_{\lambda \in L} y_\lambda = \sum_{\lambda \in L} (x_\lambda + y_\lambda)$ and $a \cdot \sum_{\lambda \in L} x_\lambda = \sum_{\lambda \in L} a x_\lambda$ shows that $a$ is a left ideal of $A$. Let $\lambda \in L$ and $x \in a_\lambda$; write $y_\lambda = x$ and $y_\mu = 0$ for $\mu \neq \lambda$; then $x = \sum_{\lambda \in L} y_\lambda$, whence $x \in a$ and finally $a_\lambda \subset a$. If a left ideal $a'$ contains $a_\lambda$ for all $\lambda \in L$, it obviously contains $a$ and hence $a$ is generated by $\bigcup_{\lambda \in L} a_\lambda$.

The ideal $a$ generated by $\bigcup_{\lambda \in L} a_\lambda$ is called *the sum of the left ideals* $a_\lambda$ and is denoted by $\sum_{\lambda \in L} a_\lambda$ (cf. II, § 1, no. 7). In particular, the sum $a_1 + a_2$ of the two left ideals consists of the sums $a_1 + a_2$ where $a_1 \in a_1$ and $a_2 \in a_2$.

### 7. QUOTIENT RINGS

Let $A$ be a ring. If $a$ is a two-sided ideal of $A$, two elements $x$ and $y$ of $A$ are said to be *congruent modulo* $a$, written $x \equiv y$ (mod. $a$) or $x \equiv y(a)$, if $x - y \in a$. This is an equivalence relation on $A$. The relations $x \equiv y(a)$ and $x' \equiv y'(a)$ imply $x + x' \equiv y + y'(a)$, $xx' \equiv xy'(a)$ for $a$ is a left ideal and $xy' \equiv yy'(a)$ for $a$ is a right ideal, whence $xx' \equiv yy'(a)$. Conversely, if $R$ is an equivalence relation on $A$ compatible with addition and multiplication, the set $a$ of $x \equiv 0$ mod. $R$ is a two-sided ideal and $x \equiv y$ mod. $R$ is equivalent to $x \equiv y$ mod. $a$.

Let $A$ be a ring and $a$ a two-sided ideal of $A$. $A/a$ denotes the quotient set of $A$ by the equivalence relation $x \equiv y(a)$, with addition and multiplication the quotients of those on $A$ ($§ 1$, no. 6, Definition 11). We show that $A/a$ is a ring:

(a) Under addition, $A/a$ is the quotient commutative group of the additive group of $A$ by the subgroup $a$.

(b) Under multiplication, $A/a$ is a monoid ($§ 2$, no. 1).

(c) Let $\xi, \eta, \zeta$ be in $A/a$ and let $\pi : A \to A/a$ be the canonical mapping; we choose elements $x, y, z$ in $A$ such that $\pi(x) = \xi, \pi(y) = \eta$ and $\pi(z) = \zeta$. Then
$$
\xi(\eta + \zeta) = \pi(x)\pi(y + z) = \pi(x(y + z)) = \pi(xy + xz)
= \pi(x)\pi(y) + \pi(x)\pi(z) = \xi\eta + \xi\zeta
$$
and the relation $(\xi + \eta)\zeta = \xi\zeta + \eta\zeta$ is established similarly.

#### Definition 6 {#alg-i-s8-def-6 .statement}

Let $A$ be a ring and $a$ a two-sided ideal of $A$. The quotient ring of $A$ by $a$, denoted by $A/a$, is the quotient set of $A$ by the equivalence relation $x \equiv y(a)$, with addition and multiplication the quotients of those on $A$.

The ring $A/\{0\}$ is isomorphic to $A$ and $A/A$ is a zero ring.

#### Theorem 2 {#alg-i-s8-thm-2 .statement}

Let $A$ be a ring and $a$ a two-sided ideal of $A$.
(a) The canonical mapping $\pi$ of $A$ onto $A/a$ is a ring homomorphism.
(b) Let $B$ be a ring and $f$ a homomorphism of $A$ into $B$. If $f(a) = \{0\}$, there exists one and only one homomorphism $\bar{f}$ of $A/a$ into $B$ such that $f = \bar{f} \circ \pi$.

By construction, $\pi(x + y) = \pi(x) + \pi(y)$ and $\pi(xy) = \pi(x)\pi(y)$ for $x, y$ in $A$; also $\pi(1)$ is the unit $\varepsilon$ of $A/a$, whence (a).

Let $A^+$ be the additive group of $A$ and $B^+$ that of $B$; as $f$ is a homomorphism of $A^+$ into $B^+$, zero on the subgroup $a$ of $A^+$, there exists (§ 4, no. 4, Proposition 5) one and only one homomorphism $\bar{f}$ of $A^+/a$ into $B^+$ such that $f = \bar{f} \circ \pi$. Let $\xi, \eta$ be in $A/a$; choose $x, y$ in $A$ with $\pi(x) = \xi$ and $\pi(y) = \eta$; then $\xi \eta = \pi(xy)$, whence

$$
\bar{f}(\xi \eta) = \bar{f}(\pi(xy)) = f(xy) = f(x)f(y) = \bar{f}(\xi)\bar{f}(\eta)
$$

and $\bar{f}(\varepsilon) = f(\pi(1)) = f(1)$, hence $\bar{f}$ is a ring homomorphism.

#### Theorem 3 {#alg-i-s8-thm-3 .statement}

Let $A$ and $B$ be rings and $f$ a homomorphism of $A$ into $B$.
(a) The kernel $a$ of $f$ is a two-sided ideal of $B$.
(b) The image $B' = f(B)$ of $f$ is a subring of $B$.
(c) Let $\pi : A \to A/a$ and $i : B' \to B$ be the canonical morphisms. There exists one and only one morphism $\bar{f}$ of $A/a$ into $B'$ such that $f = i \circ \bar{f} \circ \pi$ and $\bar{f}$ is an isomorphism.

As $f$ is a morphism of the additive group of $A$ into that of $B$, $a$ is a subgroup of $A$. If $x \in a$ and $a \in A$, then $f(ax) = f(a)f(x) = 0$, hence $ax \in a$ and similarly $xa \in a$; hence $a$ is a two-sided ideal of $A$. Assertion (b) is obvious. As $f$ is zero on $a$, there exists a morphism $\bar{f}$ of $A/a$ into $B'$ such that $f = i \circ \bar{f} \circ \pi$ (Theorem 2). The uniqueness of $\bar{f}$ and the fact that $\bar{f}$ is an isomorphism follow from Set Theory, II, § 6, no. 4.

### 8. SUBRINGS AND IDEALS IN A QUOTIENT RING

#### Proposition 5 {#alg-i-s8-prop-5 .statement}

Let $A$ and $A'$ be two rings, $f$ a homomorphism of $A$ into $A'$ and $a$ the kernel of $f$.
(a) Let $B'$ be a subring of $A'$. Then $B = f^{-1}(B')$ is a subring of $A$ containing $a$. If $f$ is surjective, then $f(B) = B'$ and $f|_B$ defines when passing to the quotient an isomorphism of $B/a$ onto $B'$.
(b) Let $b'$ be a left (resp. right, two-sided) ideal of $A'$. Then $b = f^{-1}(b')$ is a left (resp. right, two-sided) ideal of $A$ containing $a$.

(c) *If $b'$ is a two-sided ideal of $A'$, the composite mapping of the canonical morphism $A' \to A'/b'$ and $f : A \to A'$ defines, when passing to the quotient, an injective morphism $\bar{f}$ of $A/b$ into $A'/b'$. If $f$ is surjective, $\bar{f}$ is an isomorphism of $A/b$ onto $A'/b'$.

(d) *Suppose $f$ is surjective. Let $\Phi$ be the set of subrings (resp. left ideals, right ideals, two-sided ideals) of $A$ containing $a$. Let $\Phi'$ be the set of subrings (resp. left ideals, right ideals, two-sided ideals) of $A'$. The mappings $B \to f(B)$ and $B' \mapsto \bar{f}(B')^{-1}$ are inverse bijections of $\Phi$ onto $\Phi'$ and $\Phi'$ onto $\Phi$.

(a) and (b) are obvious, except the last assertion of (a) which follows from no. 7, Theorem 3.

The composite morphism $g : A \to A' \to A'/b'$ considered in (c) has kernel $b$ and hence $\bar{f}$ is an injective morphism of $A/b$ into $A'/b'$ (§ 8, no. 7, Theorem 3). If $f$ is surjective, $g$ is surjective and hence $\bar{f}$ is surjective.

Suppose $f$ is surjective. By the above, the mapping $\theta : B' \mapsto \bar{f}(B')^{-1}$ is a mapping of $\Phi'$ into $\Phi$. Clearly the mapping $\eta : B \mapsto f(B)$ is a mapping of $\Phi$ into $\Phi'$. Then $\theta \circ \eta = \mathrm{Id}_{\Phi}, \eta \circ \theta = \mathrm{Id}_{\Phi'},$ whence (d).

#### Remark {#alg-i-s8-n8-rem-1 .statement}

In the above notation, $\theta$ and $\eta$ are ordered set isomorphisms ($\Phi$ and $\Phi'$ being ordered by inclusion).

#### Corollary {#alg-i-s8-n8-cor-1 .statement}

*Let $A$ be a ring and $a$ a two-sided ideal of $A$.
(a) Every left (resp. right, two-sided) ideal of $A/a$ can be written uniquely in the form $b/a$, where $b$ is a left (resp. right, two-sided) ideal of $A$ containing $a$.
(b) If $b$ is two-sided, the composite homomorphism $A \to A/a \to (A/a)/(b/a)$ defines when passing to the quotient an isomorphism of $A/b$ onto $(A/a)/(b/a)$.*

It suffices to apply Proposition 5 to the canonical morphism of $A$ onto $A/a$.

### 9. MULTIPLICATION OF IDEALS

Let $A$ be a ring and $a$ and $b$ two-sided ideals of $A$. The set of elements of the form $x_1 y_1 + \cdots + x_n y_n$ with $n \geq 0, x_i \in a$ and $y_i \in b$ for $1 \leq i \leq n$, is obviously a two-sided ideal of $A$, which is denoted by $ab$ and called the *product* of the two-sided ideals $a$ and $b$. Under this multiplication, the set of two-sided ideals of $A$ is a monoid with unit element the two-sided ideal $A$. If $a, b, c$ are two-sided ideals of $A$, then $a(b+c) = ab + ac, (b+c)a = ba + ca$. If $A$ is commutative, multiplication of ideals is commutative.

$ab \subset aA \subset a$ and $ab \subset Ab \subset b$, hence

$$
ab \subset a \cap b.
$$

(21)

#### Proposition 6 {#alg-i-s8-prop-6 .statement}

*Let $a, b_1, \ldots, b_n$ be two-sided ideals of $A$. If $A = a + b_i$ for all $i$, then $A = a + b_1 b_2 \ldots b_n = a + (b_1 \cap b_2 \cap \cdots \cap b_n)$.*

By (21) it suffices to prove that $A = a + b_1 b_2 \ldots b_n$. By induction, it suffices to consider the case where $n = 2$. By hypothesis, there exist $a, a' \in a, b_1 \in b_1, b_2 \in b_2$ such that $1 = a + b_1 = a' + b_2$. Then
$$
1 = a' + (a + b_1) b_2 = (a' + a b_2) + b_1 b_2 \in a + b_1 b_2,
$$
whence $A = a + b_1 b_2$.

#### Proposition 7 {#alg-i-s8-prop-7 .statement}

*Let $b_1, \ldots, b_n$ be two-sided ideals of $A$ such that $b_i + b_j = A$ for $i \neq j$. Then $b_1 \cap b_2 \cap \cdots \cap b_n = \sum_{\sigma \in S_n} b_{\sigma(1)} b_{\sigma(2)} \cdots b_{\sigma(n)}$. In particular, if $A$ is commutative, $b_1 \cap b_2 \cap \cdots \cap b_n = b_1 b_2 \ldots b_n$ (cf. Exercise 2).*

Suppose first $n = 2$. There exist $a_1 \in b_1, a_2 \in b_2$ such that $a_1 + a_2 = 1$. If $x \in b_1 \cap b_2$, then $x = x(a_1 + a_2) = x a_1 + x a_2 \in b_2 b_1 + b_1 b_2$. Hence $b_1 \cap b_2 = b_1 b_2 + b_2 b_1$.

Suppose now the equation of the proposition is established for all integers $< n$. By Proposition 6, $b_n + (b_1 b_2 \ldots b_{n-1}) = A$ and hence
$$
b_1 \cap b_2 \cap \cdots \cap b_n = (b_1 \cap b_2 \cap \cdots \cap b_{n-1}) b_n + b_n (b_1 \cap b_2 \cap \cdots \cap b_{n-1})
$$
$$
= \left( \sum_{\sigma \in S_{n-1}} b_{\sigma(1)} b_{\sigma(2)} \cdots b_{\sigma(n-1)} \right) b_n
$$
$$
+ b_n \left( \sum_{\sigma \in S_{n-1}} b_{\sigma(1)} b_{\sigma(2)} \cdots b_{\sigma(n-1)} \right)
$$
$$
\subset \sum_{\tau \in S_n} b_{\tau(1)} b_{\tau(2)} \cdots b_{\tau(n)} \subset b_1 \cap b_2 \cap \cdots \cap b_n.
$$

### 10. PRODUCT OF RINGS

Let $(A_i)_{i \in I}$ be a family of rings. Let $A$ be the product set $\prod_{i \in I} A_i$. On $A$ addition and multiplication are defined by the formulae
$$
(x_i) + (y_i) = (x_i + y_i), \quad (x_i)(y_i) = (x_i y_i).
$$
It is immediately verified that $A$ is a ring called the *product* of the rings $A_i$, with zero the element $0 = (0_i)_{i \in I}$, where $0_i$ is the zero of $A_i$, and unit $1 = (1_i)_{i \in I}$, where $1_i$ is the unit of $A_i$. If the $A_i$ are commutative, so is $A$. If $C_i$ is the centre of $A_i$, the centre of $A$ is $\prod_{i \in I} C_i$.

For all $i \in I$, the projection $\mathrm{pr}_i$ of $A$ onto $A_i$ is a ring homomorphism. If $B$ is a ring and $f_i : B \to A_i$ is a family of homomorphisms, there exists a unique homomorphism $f : B \to A$ such that $f_i = \mathrm{pr}_i \circ f$ for all $i \in I$; it is given by $f(b) = (f_i(b))_{i \in I}$.

For all $i \in I$, let $a_i$ be a left ideal of $A_i$. Then $a = \prod_{i \in I} a_i$ is a left ideal of $A$. There is an analogous result for right ideals, two-sided ideals and subrings.

Suppose that $a_i$ is a two-sided ideal for all $i \in I$ and let $f_i$ denote the canonical mapping of $A_i$ onto $A_i / a_i$. Then the mapping $f : (x_i)_{i \in I} \mapsto (f_i(x_i))_{i \in I}$ of $\prod_{i \in I} A_i$ onto $\prod_{i \in I} (A_i / a_i)$ is a ring homomorphism of kernel $\prod_{i \in I} a_i$ and hence defines when passing to the quotient an isomorphism of $\left( \prod_{i \in I} A_i \right) / \left( \prod_{i \in I} a_i \right)$ onto $\prod_{i \in I} (A_i / a_i)$.

Let $(I_\lambda)_{\lambda \in L}$ be a partition of $I$. The canonical bijection of $\prod_{i \in I} A_i$ onto $\prod_{\lambda \in L} \left( \prod_{i \in I_\lambda} A_i \right)$ is a ring isomorphism, under which these two rings are identified.

Let $J \subset I$. Let $e_J$ denote the element $(x_i)_{i \in I}$ of $A$ defined by $x_i = 1_i$ for $i \in J$, $x_i = 0_i$ for $i \in I - J$. Then $e_J$ is a central idempotent ($§ 1$, no. 4) of $A$. The following formulae follow immediately:

$$
\begin{align*}
e_I &= 1; \\
e_\varnothing &= 0; \\
e_{J \cap K} &= e_J e_K & \text{for } J \subset I, K \subset I; \\
e_{J \cup K} &= e_J + e_K & \text{for } J \subset I, K \subset I, J \cap K = \varnothing; \\
\sum_\lambda e_{J_\lambda} &= 1 & \text{if } (J_\lambda) \text{ is a finite partition of } I.
\end{align*}
$$

Let $A_J = \prod_{i \in J} A_i$. Let $\eta_J$ be the canonical projection of $A$ onto $A_J$. For $x = (x_i)_{i \in J} \in A_J$, let $\varepsilon_J(x)$ be the element $(y_i)_{i \in I}$ of $A$ defined by $y_i = x_i$ for $i \in J$, $y_i = 0_i$ for $i \in I - J$. Then $\eta_J$ is a ring homomorphism of $A$ onto $A_J$, $\varepsilon_J$ is an injective homomorphism of the additive group of $A_J$ onto $A$ and in the diagram

$$
A_J \xrightarrow{\varepsilon_J} A \xrightarrow{\eta_{I-J}} A_{I-J}
$$

the kernel $a_J$ of $\eta_{I-J}$ is equal to the image of $\varepsilon_J$. Then $\varepsilon_J(xx') = \varepsilon_J(x)\varepsilon_J(x')$ for all $x, x' \in A_J$; but $\varepsilon_J$ is not in general a ring homomorphism for $\varepsilon_J(1) = e_J$. Clearly $a_J = e_J A = A e_J$.

Let $e_{(i)} = e_i$ and $a_i = a_{(i)} = e_i A = A e_i$ for all $i \in I$. Then $e_i^2 = e_i$,

$$
e_i e_j = e_j e_i = 0
$$

for $i \neq j$. If $I$ is finite, then $\sum_{i \in I} e_i = 1$, the additive group $A$ is the direct sum of the two-sided ideals $a_i$ and if $x \in A$ its component in $a_i$ is $x e_i$. The following proposition is immediately deduced.

#### Proposition 8 {#alg-i-s8-prop-8 .statement}

*Suppose $I$ is finite. If $b$ is a left or right ideal of $A$, $b$ is the direct sum of the $b \cap a_i$.*

### 11. DIRECT DECOMPOSITION OF A RING

Let $A$ be a ring and $(b_i)_{i \in I}$ a family of two-sided ideals of $A$. We shall call the homomorphism

$$
x \mapsto (\phi_i(x))_{i \in I},
$$

where $\phi_i$ is the canonical homomorphism of $A$ onto $A/b_i$, the canonical homomorphism of $A$ into $\prod_{i \in I} (A/b_i)$.

#### Proposition 9 {#alg-i-s8-prop-9 .statement}

*Let $A$ be a ring and $(b_1, \ldots, b_n)$ two-sided ideals of $A$ such that $b_i + b_j = A$ for $i \neq j$. The canonical homomorphism of $A$ into $\prod_{i=1}^n (A/b_i)$ is surjective of kernel $\bigcap_{i=1}^n b_i = \sum_{\sigma \in S_n} b_{\sigma(1)} b_{\sigma(2)} \cdots b_{\sigma(n)}.$*

Clearly the kernel is $\bigcap_{i=1}^n b_i$. To prove the surjectivity, it is necessary to show that, for every family $(x_i)_{1 \leq i \leq n}$ of elements of $A$, there exists $x \in A$ such that $x \equiv x_i (b_i)$ for all $1 \leq i \leq n$. We prove this assertion by induction on the cardinal $n$ of $I$, the case $n \leq 1$ being trivial. By the induction hypothesis, there exists $y \in A$ such that $y \equiv x_i (b_i)$ for $1 \leq i \leq n-1$. We look for an $x$ of the form $y + z$ with $z \in A$. Of necessity $z \equiv 0 (b_i)$ for $i < n$, that is $z \in b = \bigcap_{i=1}^{n-1} b_i$, and on the other hand $z \equiv x_n - y (b_n)$. Now $b_n + b = A$ by no. 9, Proposition 6, whence the existence of $z$. Finally, the second expression of the kernel follows from no. 9, Proposition 7.

#### Definition 7 {#alg-i-s8-def-7 .statement}

*Let $A$ be a ring. A finite family $(b_i)_{i \in I}$ of two-sided ideals of $A$ such that the canonical homomorphism of $A$ into $\prod_{i \in I} (A/b_i)$ is an isomorphism is called a direct decomposition of $A$.*

#### Proposition 10 {#alg-i-s8-prop-10 .statement}

*Let $A$ be a ring, $A'$ its centre and $(b_i)_{i \in I}$ a finite family of two-sided ideals of $A$. The following conditions are equivalent:

(a) the family $(b_i)_{i \in I}$ is a direct decomposition of $A$;
(b) there exists a family $(e_i)_{i \in I}$ of idempotents of $A'$ such that $e_i e_j = 0$ for $i \neq j$, $1 = \sum_{i \in I} e_i$ and $b_i = A(1 - e_i)$ for $i \in I$;
(c) $b_i + b_j = A$ for $i \neq j$ and $\bigcap_{i \in I} b_i = \{0\}$;
(d) $b_i + b_j = A$ for $i \neq j$ and $\prod_{i \in I} b_i = \{0\}$ for every total order on $I$;
(e) there exists a direct decomposition $(b'_i)_{i \in I}$ of $A'$ such that $b_i = A b'_i$ for $i \in I$.*

(a) $\Rightarrow$ (b). If condition (a) holds, $A$ may be identified with the ring $\prod_{i \in I} (A/b_i)$ and $b_i$ with the kernel of $\mathrm{pr}_i$. The existence of the $e_i$ with the properties in (b) then follows from no. 10.

(b) $\Rightarrow$ (d). Suppose that the $e_i$ exist with the properties in (b). For $i \neq j$, $1 - e_i \in b_i, \ e_i = e_i(1 - e_j) \in b_j$, hence $1 \in b_i + b_j$ and $A = b_i + b_j$. On the other hand, if I is given a total ordering and $(x_i)_{i \in I}$ is a family of elements of A, then, since the $e_i$ are central,

$$
\prod_{i \in I} x_i (1 - e_i) = \left( \prod_{i \in I} x_i \right) \left( \prod_{i \in I} (1 - e_i) \right) = \left( \prod_{i \in I} x_i \right) \left( 1 - \prod_{i \in I} e_i \right) = 0
$$

hence $\prod_{i \in I} b_i = \{0\}$.

(d) $\Rightarrow$ (c). This follows from no. 9, Proposition 7.

(c) $\Rightarrow$ (a). This follows from Proposition 9.

Thus conditions (a), (b), (c) and (d) are equivalent. Suppose they hold. By (b) $\Rightarrow$ (a), the family of $b'_i = A'(1 - e_i)$ is a direct decomposition of $A'$. Then $b_i = A(1 - e_i) = Ab'_i$ for all $i \in I$. Hence condition (e) holds.

Finally, suppose condition (e) holds. By (a) $\Rightarrow$ (b), there exists a family $(e_i)_{i \in I}$ of idempotents of $A'$ such that $e_i e_j = 0$ for $i \neq j$, $1 = \sum_{i \in I} e_i$ and $b'_i = A'(1 - e_i)$ for $i \in I$. Then $b_i = Ab'_i = A(1 - e_i)$ for $i \in I$, hence condition (b) holds.

#### Remark {#alg-i-s8-n11-rem-1 .statement}

Let A be a ring. Let $(a_i)_{i \in I}$ be a finite family of subgroups of the additive group $A^+$ of A such that $A^+$ is the direct sum of the $a_i$. Suppose $a_i a_i \subset ai$ for $i \in I$ and $a_i a_j = \{0\}$ for $i \neq j$. Then $a_i$ is for all $i \in I$ a two-sided ideal of A. With addition and multiplication induced by those on A, $a_i$ is a ring with unit element the component of $1 \in A$ in $a_i$. If $b_i = \sum_{j \neq i} a_j$, clearly the $b_i$ satisfy condition (c) of Proposition 10 and hence $(b_i)_{i \in I}$ is a direct decomposition of A, which is said to be *defined by* $(a_i)_{i \in I}$.

*Example*: *Ideals and quotient rings of* $\mathbf{Z}$

An ideal of $\mathbf{Z}$ is an additive subgroup of $\mathbf{Z}$ and hence of the form $n.\mathbf{Z}$ with $n \geqslant 0$; conversely, for every integer $n \geqslant 0$, the set $n.\mathbf{Z}$ is an ideal, the principal ideal $(n)$. Thus every ideal of $\mathbf{Z}$ is principal and is represented uniquely in the form $n\mathbf{Z}$ with $n \geqslant 0$. The ideal $(1)$ is equal to $\mathbf{Z}$, the ideal $(0)$ consists of 0 and the ideals distinct from $\mathbf{Z}$ and $\{0\}$ are therefore of the form $n\mathbf{Z}$ with $n > 1$. If $m \geqslant 1$ and $n \geqslant 1$, $m\mathbf{Z} \supset n\mathbf{Z}$ if and only if $n \in m.\mathbf{Z}$, that is $m$ divides $n$. Therefore, for the ideal $n\mathbf{Z}$ to be maximal, it is necessary and sufficient that there exist no integer $m > 1$ distinct from $n$ and dividing $n$; in other words, *the maximal ideals of* $\mathbf{Z}$ *are the ideals of the form* $p\mathbf{Z}$ *where* $p$ *is a prime number* (§ 4, no. 10, Definition 16).

Let $m$ and $n$ be two integers $\geqslant 1$. The ideal $m\mathbf{Z} + n\mathbf{Z}$ is principal, whence there is an integer $d \geqslant 1$ characterized by $d\mathbf{Z} = m\mathbf{Z} + n\mathbf{Z}$; for every integer r \geqslant 1, the relation "r divides d" is equivalent to $r\mathbf{Z} \supset d\mathbf{Z}$ and hence to "$r\mathbf{Z} \supset m\mathbf{Z}$ and $r\mathbf{Z} \supset n\mathbf{Z}$", that is to "r divides m and n". It is thus seen that the common divisors of m and n are the divisors of d and that d is *the greatest* of the divisors $\geqslant 1$ common to m and n; d is called *the greatest common divisor* (abbreviated to g.c.d.) of m and n. As $d\mathbf{Z} = m\mathbf{Z} + n\mathbf{Z}$, there exist two integers x and y such that $d = mx + ny$. m and n are said to be *relatively prime* if their g.c.d. is equal to 1. It amounts to the same to assume that there exist integers x and y with $mx + ny = 1$.

The intersection of the ideals $m\mathbf{Z}$ and $n\mathbf{Z}$ is non-zero for it contains $mn$ and hence is of the form $r\mathbf{Z}$ with $r \geqslant 1$. Arguing as above, it is seen that the multiples of r are the common multiples of m and n and that r is *the least* of the integers $\geqslant 1$ which are common multiples of m and n; it is called *the least common multiple* (l.c.m.) of m and n.

The product of the ideals $m\mathbf{Z}$ and $n\mathbf{Z}$ is the set of $\sum_{i=1}^{r} mx_i ny_i = mn \left( \sum_{i=1}^{r} x_i y_i \right)$ for $x_1, \ldots, y_r \in \mathbf{Z}$ and hence is equal to $mn\mathbf{Z}$.

For every integer $n \geqslant 1$, the quotient ring $\mathbf{Z}/n\mathbf{Z}$ is called the *ring of integers modulo n*; it has n elements, which are the classes modulo n of the integers 0, 1, 2, ..., $n - 1$. For $n = 1$, we obtain the zero ring.

#### Proposition 11 {#alg-i-s8-prop-11 .statement}

*Let $n_1, \ldots, n_d$ be integers $\geqslant 1$ which are relatively prime in pairs and $n = n_1 \ldots n_r$. The canonical homomorphism of $\mathbf{Z}$ into the product ring $\prod_{i=1}^{r} \mathbf{Z}/n_i\mathbf{Z}$ is surjective of kernel $n\mathbf{Z}$ and defines a ring isomorphism of $\mathbf{Z}/n\mathbf{Z}$ onto $\prod_{i=1}^{r} \mathbf{Z}/n_i\mathbf{Z}$.*

Let $a_i = n_i\mathbf{Z}$ for $i = 1, \ldots, r$. By hypothesis, $a_i + a_j = \mathbf{Z}$ for $i \neq j$. The proposition then follows from Proposition 9.

The above results, as also those concerning decomposition into prime factors, will be generalized in Chapter VII, § 1, which is devoted to the study of principal ideal domains and in *Commutative Algebra*, Chapter VII, § 3, which is devoted to the study of factorial domains.

### 12. RINGS OF FRACTIONS

#### Theorem 4 {#alg-i-s8-thm-4 .statement}

*Let A be a commutative ring and S a subset of A. Let $A_S$ be the monoid of fractions of A (provided only with multiplication) with denominators in S (§ 2, no. 4). Let $\varepsilon : A \to A_S$ be the canonical morphism. There exists on $A_S$ one and only one addition satisfying the following conditions:
(a) $A_S$, with this addition and its multiplication, is a commutative ring;
(b) $\varepsilon$ is a ring homomorphism.*

Suppose an addition has been found for $A_S$ satisfying conditions (a) and (b).

Let $x, y \in A_S$. Let $S'$ be the stable multiplicative submonoid of $A$ generated by $S$. There exist $a, b \in A$ and $p, q \in S'$ such that $x = a/p, y = b/q$. Then

$$
x = \varepsilon(aq)\varepsilon(pq)^{-1}, \quad y = \varepsilon(bp)\varepsilon(pq)^{-1},
$$

whence

(23)
$$
\begin{align*}
x + y &= (\varepsilon(aq) + \varepsilon(bp))\varepsilon(pq)^{-1} \\
&= \varepsilon(aq + bp)\varepsilon(pq)^{-1} \\
&= (aq + bp)/pq.
\end{align*}
$$

This proves the uniqueness of the addition.

We now *define* an addition on $A_S$ by setting $x + y = (aq + bp)/pq$. It is necessary to show that this definition does not depend on the choice of $a, b, p, q$. Now, if $a', b' \in A, p', q' \in S'$ are such that $x = a'/p', y = b'/q'$, there exist $s$ and $t$ in $S'$ such that $ap's = a'ps, bq't = b'qt$, whence

$$
(aq + bp)(p'q')(st) = (a'q' + b'p')(pq)(st)
$$

and hence

$$
(aq + bp)/pq = (a'q' + b'p')/p'q'.
$$

It is easily verified that addition in $A_S$ is associative and commutative, that $0/1$ is identity element for addition, that $(-a)/p$ is the negative of $a/p$ and that $x(y + z) = xy + xz$ for all $x, y, z \in A_S$. If $a, b \in A$, then

$$
\varepsilon(a + b) = (a + b)/1 = a/1 + b/1 = \varepsilon(a) + \varepsilon(b)
$$

and hence $\varepsilon$ is a ring homomorphism.

#### Definition 8 {#alg-i-s8-def-8 .statement}

*The ring defined in Theorem 4 is called the ring of fractions associated with $S$, or with denominators in $S$, and is denoted by $A[S^{-1}]$.*

The zero of $A[S^{-1}]$ is $0/1$, the unit of $A[S^{-1}]$ is $1/1$.

We shall return to the properties of $A[S^{-1}]$ in *Commutative Algebra*, Chapter II, § 2.

If $S$ is the set of cancellable elements of $A$, the ring $A[S^{-1}]$ is called the total ring of fractions of $A$. $A$ is then identified with a subring of $A[S^{-1}]$ by means of the mapping $\varepsilon$, which is then injective (I, § 2, no. 4, Proposition 6).

#### Theorem 5 {#alg-i-s8-thm-5 .statement}

*Let $A$ be a commutative ring, $S$ a subset of $A$, $B$ a ring and $f$ a homomorphism of $A$ into $B$ such that every element of $f(S)$ is invertible. There exists one and only one $\bar{f}$ of $A[S^{-1}]$ into $B$ such that $f = \bar{f} \circ \varepsilon$.*

We know (§ 2, no. 4, Theorem 1) that there exists one and only one morphism $\bar{f}$ of the multiplicative monoid $A[S^{-1}]$ into the multiplicative monoid $B$ such that $f = \bar{f} \circ \varepsilon$. Let $a, b \in A, p, q \in S'$ (stable multiplicative submonoid of $A$ generated by $S$). As the elements of $f(A)$ commute in pairs,
$$
\bar{f}(a/p + b/q) = \bar{f}((aq + bp)/pq) = f(aq + bp)f(pq)^{-1}
= (f(a)f(q) + f(b)f(p))f(p)^{-1}f(q)^{-1}
= f(a)f(p)^{-1} + f(b)f(q)^{-1}
= \bar{f}(a/p) + \bar{f}(b/q).
$$
Hence $\bar{f}$ is a ring homomorphism.

### Exercises {#alg-i-s8-exercises}

See the [exercises for § 8](exercises/s8/).
