---
book: fvr
book_title: Functions of a Real Variable
chapter: VI
chapter_title: GENERALIZED TAYLOR EXPANSIONS EULER-MACLAURIN SUMMATION FORMULA
section: 1
section_title: GENERALIZED TAYLOR EXPANSIONS
lang: en
source: fvr-i-vii
book_pages: 269-283, 291-292
pdf_pages: 0284-0298, 0306-0307
extraction: ocr
subsections:
    - "no": 1
      title: COMPOSITION OPERATORS ON AN ALGEBRA OF POLYNOMIALS
      page: 269
      pdf_page: 284
    - "no": 2
      title: APPELL POLYNOMIALS ATTACHED TO A COMPOSITION OPERATOR
      page: 272
      pdf_page: 287
    - "no": 3
      title: GENERATING SERIES FOR THE APPELL POLYNOMIALS
      page: 274
      pdf_page: 289
    - "no": 4
      title: BERNOULLI POLYNOMIALS
      page: 275
      pdf_page: 290
    - "no": 5
      title: COMPOSITION OPERATORS ON FUNCTIONS OF A REAL VARIABLE
      page: 277
      pdf_page: 292
    - "no": 6
      title: INDICATRIX OF A COMPOSITION OPERATOR
      page: 278
      pdf_page: 293
    - "no": 7
      title: THE EULER-MACLAURIN SUMMATION FORMULA
      page: 282
      pdf_page: 297
statements: 20
exercises: 3
content_sha256: c5d02763e0ba81f180ba651433971351bc4433064e4281ee8e880b60ece6ef27
---

## § 1. GENERALIZED TAYLOR EXPANSIONS

### 1. COMPOSITION OPERATORS ON AN ALGEBRA OF POLYNOMIALS

Let K be a commutative field of characteristic 0, and K[X] the algebra of polynomials in one indeterminate over K (Alg., IV. 1); throughout this section by an operator on K[X] we shall mean a linear map U of the vector space K[X] (over K) into itself; since the monomials $X^n \ (n \geqslant 0)$ form a basis for this space, U is determined by the polynomials $U(X^n)$; specifically, if $f(X) = \sum_{k=0}^\infty \lambda_k X^k$ with $\lambda_k \in K$, then
$$
U(f) = \sum_{k=0}^\infty \lambda_k U(X^k).
$$
If G is a commutative algebra over K, with an identity element, the G-module G[X] is obtained by extending the field of scalars K of the vector space K[X] to G; every operator U on K[X] extends in a unique manner to a linear map of the G-module G[X] to itself, which we again denote by U (Alg., II, p. 278); for each element $g(X) = \sum_{k=0}^\infty \gamma_k X^k$, with $\gamma_k \in G$, one has $U(g) = \sum_{k=0}^\infty \gamma_k U(X^k)$.

Consider in particular the case where G = K[Y]; then G[X] is the ring K[X,Y] of polynomials in two indeterminates over K; to avoid confusion we denote the extension of U to G[X] by $U_X$. For any polynomial $g(X, Y) = \sum_{k=0}^\infty \gamma_k(Y) X^k$ where $\gamma_k(Y) \in K[Y]$ one thus has $U_X(g) = \sum_{k=0}^\infty \gamma_k(Y) U(X^k)$. Since $U_X$ is linear one sees that if one writes $g(X, Y) = \sum_{h=0}^\infty \beta_h(X) Y^h$ then one also has $U_X(g) = \sum_{h=0}^\infty U(\beta_h) Y^h$.

Under the canonical isomorphism of K[X] onto K[Y] which associates Y with X the operator U transforms to an operator on K[Y], which we will denote $U_Y$, to avoid confusion, so that $U_Y(f(Y))$ is the polynomial obtained by replacing X by Y in the polynomial $U(f(X)) = U_X(f(X))$. This operator $U_Y$ can in turn be extended to an operator (again denoted by $U_Y$) on K[X,Y]: if $g(X, Y) = \sum_{h=0}^\infty \beta_h(X) Y^h$ then
$$
U_Y(g(X, Y)) = \sum_{h=0}^\infty \beta_h(X) U_Y(Y^h).
$$

As an example of these extensions we cite the derivation operator D on K[X] (Alg., IV. 6), which gives the partial derivation operators D_X and D_Y on K[X,Y].

For any polynomial $f \in K[X]$ we denote by $T_Y(f)$ the polynomial $f(X + Y)$ in K[X,Y]; the map $T_Y$ is a K-linear map from K[X] into K[X,Y], called a translation operator.

#### Definition 1 {#fvr-vi-s1-def-1 .statement}

*One says that an operator U on K[X] is a composition operator if it commutes with the translation operator, that is, if $U_X T_Y = T_Y U$.*

In other words, if $f$ is an arbitrary polynomial in K[X], and if $g = U(f)$, one must have $g(X + Y) = U_X(f(X + Y))$.

It follows immediately from this definition that for every polynomial $f(X) \in K[X]$ one has, in the above notation,

$$
U_X(f(X + Y)) = U_Y(f(X + Y)).
$$

(1)

#### Example 1 {#fvr-vi-s1-n1-exa-1 .statement}

For every $\lambda \in K$ the operator which to every polynomial $f(X)$ associates the polynomial $f(X + \lambda)$ is a composition operator.
2) The derivation D on K[X] is a composition operator (*cf.* prop. 1).

#### Remark {#fvr-vi-s1-n1-rem-1 .statement}

Since K is an infinite field the operator U on K[X] is a composition operator if and only if for every polynomial $f \in K[X]$ and every element $\alpha \in K$ one has, putting $g = U(f)$, that $g(X + \alpha) = U(f(X + \alpha))$. (Alg., IV. 16, cor.).

It is clear that every linear combination of composition operators, with coefficients in K, is a composition operator; the same is true for the composition of two composition operators. In other words, the composition operators form a subalgebra $\Gamma$ of the algebra of endomorphisms of the vector space K[X].

#### Proposition 1 {#fvr-vi-s1-prop-1 .statement}

*For an operator U on K[X] to be a composition operator it is necessary and sufficient that it commute with the derivation D on K[X].*

Indeed, the Taylor formula shows that for every polynomial $f \in K[X]$ one has

$$
U_X(f(X + Y)) = U_X \left( \sum_{k=0}^{\infty} \frac{1}{k!} Y^k D^k f(X) \right) = \sum_{k=0}^{\infty} \frac{1}{k!} Y^k U(D^k f(X));
$$

if one puts $g = U(f)$ then one has

$$
g(X + Y) = \sum_{k=0}^{\infty} \frac{1}{k!} Y^k D^k g(X) = \sum_{k=0}^{\infty} \frac{1}{k!} Y^k D^k (U(f(X)));
$$

for U to be a composition operator, one must then have $UD^k = D^k U$ for every integer $k \geq 1$, and in particular $UD = DU$. Conversely, if this relation holds, it implies $UD^k = D^k U$ for every integer $k \geq 1$, by induction on $k$; the Taylor formula then shows that $g(X + Y) = U_X(f(X + Y))$.

For every polynomial $f \in K[X, Y]$ we denote by $U_0(f)$ the term *independent of* X in the polynomial $U_X(f)$; in particular, if $f \in K[X]$, $U_0(f)$ is the *constant term* in $U(f)$, and $U_0$ is a *linear form* on $K[X]$. For every polynomial $f \in K[X]$ let $g = U(f)$; by def. 1 of VI, p. 270

$$
g(X + Y) = U_X(f(X + Y)) = U_X \left( \sum_{k=0}^{\infty} \frac{1}{k!} X^k D^k f(Y) \right) = \sum_{k=0}^{\infty} \frac{1}{k!} U(X^k) D^k f(Y)
$$

and if, in this formula, one replaces X by 0, one obtains

$$
g(Y) = \sum_{k=0}^{\infty} \frac{1}{k!} U_0(X^k) D^k f(Y).
$$

Thus one sees that

$$
U(f(X)) = \sum_{k=0}^{\infty} \frac{1}{k!} \mu_k D^k f(X) \tag{2}
$$

where $\mu_k$ *is the constant term in the polynomial* $U(X^k)$.

This formula shows that the $\mu_k$ determine the composition operator $U$ completely; conversely, if $(\mu_n)$ is an *arbitrary* sequence of elements of K then the formula (2) defines an operator $U$ which clearly commutes with D, so (VI, p. 270, prop. 1) is a composition operator. From now on we shall write (2) in the form

$$
U = \sum_{k=0}^{\infty} \frac{1}{k!} \mu_k D^k. \tag{3}
$$

This formula can be interpreted in topological language as follows: if one considers the discrete topology on $K[X]$, and the topology of *simple* convergence on the algebra $\mathrm{End}(K[X])$ of endomorphisms of $K[X]$ (*Gen. Top.*, X, p. 277), the series with general term $\frac{1}{k!} \mu_k D^k$ is commutatively convergent in $\mathrm{End}(K[X])$ and has sum $U$ (*Gen. Top.*, III, p. 269).

The formula (3) shows that to every *formal series* $u(S) = \sum_{k=0}^{\infty} \alpha_k S^k$ in one indeterminate over K (*Alg.*, IV. 41) one can associate the composition operator $U = \sum_{k=0}^{\infty} \alpha_k D^k$, which in future we shall denote by $u(D)$. This remark can be clarified in the following manner:

#### Theorem 1 {#fvr-vi-s1-thm-1 .statement}

*The map which to every formal series* $u(S) = \sum_{k=0}^{\infty} \alpha_k S^k$ *in one indeterminate over* K *associates the composition operator* $u(D) = \sum_{k=0}^{\infty} \alpha_k D^k$ *on* $K[X]$ *is an isomorphism of the algebra* $K[[S]]$ *of formal series onto the algebra* $\Gamma$ *of composition operators.*

One verifies immediately that this map is an homomorphism. It remains to see that it is injective, in other words, that the relation $\sum_{k=0}^{\infty} \alpha_k D^k = 0$ implies $\alpha_k = 0$ for every $k$; now $h! \alpha_h$ is the constant term in the polynomial obtained by applying $\sum_{k=0}^{\infty} \alpha_k D^k$ to $X^h$, whence the theorem.

#### Corollary {#fvr-vi-s1-n1-cor-1 .statement}

*The algebra $\Gamma$ of composition operators in $K[X]$ is commutative.*

#### Example {#fvr-vi-s1-n1-exa-2 .statement}

If $U$ is the operator which to each polynomial $f(X)$ associates $f(X + \lambda)$ (where $\lambda \in K$), one has $U_0(X^k) = \lambda^k$, and so $U = \sum_{k=0}^{\infty} \frac{1}{k!} (\lambda D)^k$. By analogy with the series expansion of $e^{\lambda}$ (III, p. 105) we write $e^S$ or $\exp(S)$ for the formal series $\sum_{n=0}^{\infty} \frac{1}{n!} S^n$ in the ring $K[[S]]$; so one can write $U = e^{\lambda D}$. Replacing the field $K$ by the field of rational fractions $K(Y)$ in this argument one sees similarly that the *translation operator* $T_Y$ can be written $e^{YD}$.

Furthermore, in the ring $K[[S, T]]$ of formal series in two indeterminates over $K$ one has

$$
(\exp S)(\exp T) = \sum_{p,q} \frac{S^p}{p!} \frac{T^q}{q!}
$$
$$
= \sum_{n=0}^{\infty} \frac{1}{n!} \left( \binom{n}{0} S^n + \binom{n}{1} S^{n-1} T + \cdots + \binom{n}{n} T^n \right)
$$
$$
= \exp(S + T)
$$

and in particular
$$
(\exp S)(\exp(-S)) = 1
$$
which justifies the notation we have introduced.

#### Scholium {#fvr-vi-s1-n1-sch-1 .statement}

The isomorphism of the algebra $K[[S]]$ of formal series and the algebra $\Gamma$ of composition operators on $K[X]$ sometimes allows one to prove propositions on formal series most simply, by proving them for the corresponding composition operators (*cf.* VI, p. 274, prop. 6).

### 2. APPELL POLYNOMIALS ATTACHED TO A COMPOSITION OPERATOR

Given a composition operator $U = \sum_{k=0}^{\infty} \alpha_k D^k \neq 0$ let $p$ be the least of the integers $k$ such that $\alpha_k \neq 0$; we shall say that $p$ is the *order* of the operator $U$.

#### Proposition 2 {#fvr-vi-s1-prop-2 .statement}

Every composition operator of order 0 is invertible in the algebra $\Gamma$ of composition operators on $\mathbf{K}[X]$.

Indeed, a formal series $\sum_{k=0}^{\infty} \alpha_k S^k$ such that $\alpha_0 \neq 0$ is invertible in the ring $\mathbf{K}[[S]]$ (Alg., IV. 41); the proposition thus follows from th. 1 of VI, p. 271.

#### Proposition 3 {#fvr-vi-s1-prop-3 .statement}

Let $U$ be a composition operator of order $p$; then $U(f) = 0$ for every polynomial $f$ of degree $< p$; for every polynomial $f \neq 0$ of degree $n \geq p$, $U(f)$ is a polynomial $\neq 0$ of degree $n - p$.

This is an immediate consequence of formula (2) of VI, p. 271 and of the definition of the order of $U$.

It is clear that every operator $U$ of order $p$ can be written in a unique way as $U = D^p V = V D^p$, where $V$ is an operator of order 0 (and so invertible).

#### Definition 2 {#fvr-vi-s1-def-2 .statement}

Let $U = D^p V$ be a composition operator of order $p$ on $\mathbf{K}[X]$. The polynomial $u_n(X) = V^{-1}(X^n)$ is called the Appell polynomial of index $n$ attached to the operator $U$.

If $V^{-1} = \sum_{k=0}^{\infty} \frac{1}{k!} \beta_k D^k$ (with $\beta_0 \neq 0$) one thus has
$$
u_n(X) = \sum_{k=0}^{n} \binom{n}{k} \beta_k X^{n-k}.
$$
(6)

One verifies that $u_n$ is a polynomial of degree $n$ (prop. 3); further
$$
u_n(0) = \beta_n.
$$

#### Proposition 4 {#fvr-vi-s1-prop-4 .statement}

The Appell polynomials attached to $U$ satisfy the relations
$$
\frac{d u_n}{d X} = n \, u_{n-1}
$$
(7)
$$
u_n(X + Y) = \sum_{k=0}^{n} \binom{n}{k} u_{n-k}(X) Y^k
$$
(8)
$$
U(u_n(X)) = \frac{n!}{(n-p)!} X^{n-p}.
$$
(9)

These formulae are in fact respectively equivalent to the following relations (bearing def. 2 in mind):

$$
DV^{-1} = V^{-1}D \tag{10}
$$
$$
(\exp(YD_X))V_X^{-1} = V_X^{-1}\exp(YD_X) \tag{11}
$$
$$
UV^{-1} = D^p. \tag{12}
$$

#### Proposition 5 {#fvr-vi-s1-prop-5 .statement}

*For every polynomial $f \in K[X]$ and every composition operator of order $p$ one has*

$$
f^{(p)}(X + Y) = \sum_{k=0}^{\infty} \frac{1}{k!} U \left( f^{(k)}(X) \right) u_k(Y) \tag{13}
$$
*(generalized Taylor expansion)*.

Indeed, if one puts $U = D^p V = V D^p$ one has (VI, p. 270, formula (1))

$$
V_X^{-1}(f(X + Y)) = V_Y^{-1}(f(X + Y)) = \sum_{k=0}^{\infty} \frac{1}{k!} f^{(k)}(X) u_k(Y) \tag{14}
$$
the Taylor formula and by def. 2 of VI, p. 273; it suffices to apply the operator $U$ to the first and last terms of formula (14) to obtain (13).

### 3. GENERATING SERIES FOR THE APPELL POLYNOMIALS

Let E be the ring of *formal series* in an indeterminate S, with coefficients in the ring of polynomials $K[X]$ (*Alg.*, IV. 41); in other words, the ring of formal series $g(X, S) = \sum_{n=0}^{\infty} \alpha_n(X) S^n$ where the $\alpha_n$ belong to $K[X]$. For every operator $U$ on $K[X]$ we defines a map $U_X$ of E to itself by putting $U_X(g(X, S)) = \sum_{n=0}^{\infty} U(\alpha_n) S^n$. It is clear that E is a module over the ring $K[[S]]$ of formal series in S with coefficients in $K$; by the linearity of $U$ on $K[X]$ one verifies immediately that for every element $\theta \in K[[S]]$ and every $g \in E$ one has $U_X(\theta g) = \theta U_X(g)$; in other words, $U_X$ is a linear map of the module E into itself.

#### Proposition 6 {#fvr-vi-s1-prop-6 .statement}

*Let $U = D^p V = u(D)$ be a composition operator of order $p$ on $K[X]$, $u(S)$ being a formal power series of order $p$ in $K[[S]]$. Then*

$$
U_X \left( \exp(XS) \right) = u(S) \exp(XS) \tag{15}
$$
$$
\frac{S^p}{u(S)} \exp(XS) = \sum_{n=0}^{\infty} \frac{1}{n!} u_n(X) S^n \tag{16}
$$
*n being the Appell polynomial of index n attached to U*.

By the scholium to th. 1 (VI, p. 271), to establish (15) it is enough to show that for every polynomial $f(Y) \in K[Y]$ one has

$$
U_X \left( \exp(XD_Y)(f(Y)) \right) = u(D_Y)(\exp(XD_Y)(f(Y))).
$$

Now the first term in (17) is $U_X(f(X + Y))$, and, since $U = u(D)$, the second term in (17) is $U_Y(f(X + Y))$, so the identity (17) reduces to (1) (VI, p. 270).

It now suffices to apply (15) to the composition operator $V^{-1} = D^p / u(D)$ to obtain (16), since, by definition, one has

$$
V^{-1}(\exp(XS)) = \sum_{n=0}^{\infty} \frac{1}{n!} u_n(X) S^n.
$$

Note that (16) can also be obtained by multiplying the formal series $S^p / u(S)$ and $\exp(XS)$, taking account of (6).

One says that the formal series (16) is the generating series of the Appell polynomials attached to $U$.

### 4. BERNOULLI POLYNOMIALS

Consider the composition operator $U$ defined by

$$
U(f(X)) = f(X + 1) - f(X);
$$

one can write $U = e^D - 1$ (VI, p. 270, Example 1); this is an operator of order 1, and if one puts $U = DV$ one has $V^{-1} = \frac{D}{e^D - 1}$. The Appell polynomial of degree $n$ corresponding to the operator $U$ is called the Bernoulli polynomial of degree $n$ and is denoted by $B_n(X)$; if one puts $b_n = B_n(0)$ one has the formulae

$$
B_n(X) = \sum_{k=0}^{n} \binom{n}{k} b_{n-k} X^k
$$
(18)

$$
\frac{S \, e^{XS}}{e^S - 1} = \sum_{n=0}^{\infty} \frac{1}{n!} B_n(X) S^n
$$
(19)

and in particular

$$
\frac{S}{e^S - 1} = \sum_{n=0}^{\infty} \frac{1}{n!} b_n S^n
$$
(20)

The formulae (7) and (9) of VI, p. 273, give, for the Bernoulli polynomials, the relations

$$
\frac{dB_n}{dX} = n B_{n-1}(X)
$$
(21)

$$
B_n(X + 1) - B_n(X) = n X^{n-1}.
$$
(22)

In particular, one has $B_n(1) - B_n(0) = 0$ for $n > 1$, which, taking account of (18), gives the induction relation

$$
\sum_{m=0}^{n-1} \binom{n}{m} b_m = 0 \quad \text{(for } n > 1)
$$

which enables one to calculate the $b_n$ step-by-step. These numbers are clearly *rational*; since one can write

$$
\frac{S}{e^S - 1} = -\frac{S}{2} + \frac{S}{2} \frac{e^S + 1}{e^S - 1}
$$

and since (VI, p. 272, formula (5))

$$
\frac{e^{-S} + 1}{e^{-S} - 1} = -\frac{e^S + 1}{e^S - 1}
$$

one sees that in the formal series for $\frac{S}{2} \frac{e^S + 1}{e^S - 1}$ all the terms of *odd* degree have coefficient zero; so one has

$$
b_0 = 1, \qquad b_1 = -\frac{1}{2}, \qquad b_{2n-1} = 0 \quad \text{for } n > 1.
$$

The rational numbers $b_{2n}$ ($n \geq 1$) are called the *Bernoulli numbers*; we shall see (VI, p. 288) that $b_{2n}$ has the sign of $(-1)^{n-1}$. The formula (23) gives, for the first values of $n$,

$$
\begin{align*}
b_2 &= \frac{1}{6}, & b_4 &= -\frac{1}{30}, & b_6 &= \frac{1}{42}, & b_8 &= -\frac{1}{30}, \\
b_{10} &= \frac{5}{66}, & b_{12} &= -\frac{691}{2730}, & b_{14} &= \frac{7}{6}, \\
b_{16} &= -\frac{3617}{510}, & b_{18} &= \frac{43867}{798}, & b_{20} &= -\frac{174611}{330}, & b_{22} &= \frac{854513}{138}, \\
b_{24} &= -\frac{236364091}{2730}, & b_{26} &= \frac{8553103}{6}, & b_{28} &= -\frac{23749461029}{870}.
\end{align*}
$$

Note that the numerators 691, 3617, 43867 are prime; the prime factorisations of the others are

$$
\begin{align*}
174611 &= 283 \times 617 \\
854513 &= 11 \times 131 \times 593 \\
236364091 &= 103 \times 2294797 \\
8553103 &= 13 \times 657931 \\
23749461029 &= 7 \times 9349 \times 362903.
\end{align*}
$$

From these we deduce expressions for the first Bernoulli polynomials

$$
\begin{align*}
B_0(X) &= 1, & B_1(X) &= X - \frac{1}{2}, & B_2(X) &= X^2 - X + \frac{1}{6}, \\
B_3(X) &= X^3 - \frac{3}{2}X^2 + \frac{1}{2}X, & B_4(X) &= X^4 - 2X^3 + X^2 - \frac{1}{30}.
\end{align*}
$$

### 5. COMPOSITION OPERATORS ON FUNCTIONS OF A REAL VARIABLE

Let I be an interval in $\mathbf{R}$ containing the interval $\mathbf{R}_+ = [0, +\infty[$; let E be a vector space over the field $\mathbf{C}$, formed of functions of a real variable with complex values, defined on I. We suppose that for every $a \geqslant 0$ and every function $f \in E$ the function $x \mapsto f(x + a)$ belongs to E; further, we assume that E contains the restrictions to I of the *polynomials with complex coefficients* and the *exponentials* $e^{\lambda x}$, where $\lambda$ is an arbitrary *complex* number. Any linear map $U$ of E into the space of all maps from I into the field $\mathbf{C}$ of complex numbers will be called an *operator* on E; if $f \in E$ and $g = U(f)$ it will be convenient to use the notation

$$
g(x) = U_{\xi}^{\xi}(f(\xi))
$$

where $\xi$ is a *dummy* variable in the functional symbolism of the right-hand term (*cf.* II, p. 58). For every $a \geqslant 0$ the operator which to any function $f \in E$ associates the restriction to I of the function $x \mapsto f(x + a)$ is called the *translation operator by a*.

#### Definition 3 {#fvr-vi-s1-def-3 .statement}

*One says that an operator U on E is a composition operator if, for every $a \geqslant 0$, it is permutable with the translation operator by a*.

In the notation introduced above, this definition becomes the identity

$$
U_{x+a}^{\xi}(f(\xi)) = U_x^{\xi}(f(\xi + a))
$$

in $x$ and $a$ ($x \in I, a \geqslant 0$). One can exchange the rôles of $x$ and $a$ in this identity if $x \geqslant 0$, then put $a = 0$; one thus obtains for $x \geqslant 0$

$$
U_x^{\xi}(f(\xi)) = U_0^{\xi}(f(\xi + x))
$$

where $U_0$ is the *linear form* on E which to each function $f \in E$ associates the value $g(0)$ of $g = U(f)$.

If $f$ is a polynomial, one has $f(\xi + x) = \sum_{k=0}^{\infty} \frac{1}{k!} f^{(k)}(\xi) x^k$, and formula (26) shows that $U(f)$ is also a polynomial; restricted to the set of polynomials in $x$, with coefficients in $\mathbf{C}$, (a set which one can identify with the algebra $\mathbf{C}[X]$), the operator $U$ is then a composition operator in the sense of def. I of VI, p. 270, and all the results of the preceding sections can be applied to it.

We again write $u_n$ for the Appell polynomials attached to the operator $U$. To the generalized Taylor expansion of a polynomial (VI, p. 274, formula (13)) there corresponds, for more general functions, the following result:

#### Theorem 2 {#fvr-vi-s1-thm-2 .statement}

*Let f be a function admitting a continuous $(n + 1)^{th}$ derivative on I, and belonging, with all its derivatives $f^{(m)}$ for $1 \leq m \leq n$, to E. If U is a composition operator of order $p \leq n$ on E one has, for $x \geq 0$ and $h \geq 0$*

$$
f^{(p)}(x + h) = \sum_{m=0}^{n} \frac{1}{m!} u_m(x) U_h^\xi \left( f^{(m)}(\xi) \right) + R_n(x, h)
$$
(27)

with
$$
R_n(x, h) = -U_h^\xi \left( \int_0^{\xi - x - h} \frac{1}{n!} u_n(x + \eta) f^{(n+1)}(\xi - \eta) d\eta \right)
$$
(28)
*(generalized Taylor expansion)*.

Consider the integral $\int_0^{\xi - x - h} \frac{1}{n!} u_n(x + \eta) f^{(n+1)}(\xi - \eta) d\eta$, defined for all $\xi \in I$,
and apply to it the formula for integration by parts of order $n + 1$ (II, p. 59, formula (11)); taking account of the relations
$$
u_n^{(k)} = n(n-1)\ldots(n-k+1)u_{n-k}
$$
derived from (7) (VI, p. 273) by recursion, one obtains
$$
\int_0^{\xi - x - h} \frac{1}{n!} u_n(x + \eta) f^{(n+1)}(\xi - \eta) d\eta
$$
$$
= \sum_{m=0}^{n} \frac{1}{m!} u_m(x) f^{(m)}(\xi) - \sum_{m=0}^{n} \frac{1}{m!} u_m(\xi - h) f^{(m)}(x + h).
$$
(29)

We apply the operator $U$ to the two sides of (29), considered as functions of $\xi$, then take the value of the function so obtained for the value $h$ of the variable $\xi$; remarking that, by the formulae (26) (VI, p. 277) and (9) (VI, p. 272), one has
$$
U_h^\xi (u_m(\xi - h)) = U_0^\xi (u_m(\xi)) = \begin{cases} 0 & \text{for } m \neq p \\ p! & \text{for } m = p \end{cases}
$$
one finally obtains (27).

### 6. INDICATRIX OF A COMPOSITION OPERATOR

With the same hypotheses as in n° 5, the formula (26) of (VI, p. 277) applied to the function $e^{\lambda x}$, gives
$$
U_\lambda^\xi (e^{\lambda \xi}) = U_0^\xi (e^{\lambda x} e^{\lambda \xi}) = e^{\lambda x} U_0^\xi (e^{\lambda \xi}) = u(\lambda) e^{\lambda x}
$$
(30)
on putting $u(\lambda) = U_0^\xi (e^{\lambda \xi})$. One says that the function $u(\lambda)$, defined on $\mathbf{C}$, with complex values, is the *indicatrix* of the composition operator $U$. Note that if the restriction of $U$ to the ring $\mathbf{C}[X]$ of polynomials is equal to the series
$$
D^p \sum_{n=0}^{\infty} \alpha_n D^n
$$
(VI, p. 271, th. 1) (which we have denoted $u(D)$ in VI, p. 271), the series of *complex terms* with general term $\alpha_n \lambda^{n+p}$ *is not necessarily convergent* for $\lambda \neq 0$, and that even if it converges for certain values of $\lambda$, the sum *is not necessarily equal to the indicatrix* $u(\lambda)$ *of U* (VI, p. 291, exerc. 2). We shall say that the composition operator $U$ is *regular* if there exists a neighbourhood of 0 in $\mathbf{C}$ such that the series with general term $\alpha_n \lambda^{n+p}$ is *absolutely convergent* and has sum *equal to the indicatrix* $u(\lambda)$ on this neighbourhood$^1$. Let us apply formula (27) of VI, p. 278, to the function $e^{\lambda x}$, making $h = 0$; since $D^m(e^{\lambda x}) = \lambda^m e^{\lambda x}$ one has $U_0^\xi \left( D^m(e^{\lambda x}) \right) = \lambda^m u(\lambda)$; it then follows that for every complex $\lambda$ such that $u(\lambda) \neq 0$

$$
\frac{\lambda^p e^{\lambda x}}{u(\lambda)} = \sum_{m=0}^n u_m(x) \frac{\lambda^m}{m!} - \frac{\lambda^{n+1}}{u(\lambda)} U_0^\xi \left( \int_0^{\xi-x} \frac{1}{n!} u_n(x+\eta) e^{\lambda(\xi-\eta)} d\eta \right)
$$

and in particular, for $x = 0$

$$
\frac{\lambda^p}{u(\lambda)} = \sum_{m=0}^n \beta_m \frac{\lambda^m}{m!} - \frac{\lambda^{n+1}}{u(\lambda)} U_0^\xi \left( \int_0^{\xi} \frac{1}{n!} u_n(\eta) e^{\lambda(\xi-\eta)} d\eta \right)
$$

with $\beta_m = u_m(0)$.

If $U$ is a *regular* operator, for all $\lambda \in \mathbf{C}$ such that the entire series $u(\lambda) = \sum_{n=0}^\infty \alpha_n \lambda^{n+p}$ and $\sum_{n=0}^\infty \beta_n \frac{\lambda^n}{n!}$ are absolutely convergent$^2$, it follows from formula (16) and the formula for the product of two absolutely convergent series (*Gen. Top.*, VIII, p. 115, prop. 1) that one has

$$
\frac{\lambda^p}{u(\lambda)} = \sum_{n=0}^\infty \beta_n \frac{\lambda^n}{n!}.
$$

Similarly, since the Taylor expansion of $e^{\lambda x}$ is absolutely convergent for every $\lambda \in \mathbf{C}$ and every $x \in \mathbf{C}$ (III, p. 106) one also has (formulae (6) (VI, p. 273) and (16) (VI, p. 274)), for all the values considered and for all $x \in \mathbf{C}$

$$
\frac{\lambda^n e^{\lambda x}}{u(\lambda)} = \sum_{n=0}^\infty u_n(x) \frac{\lambda^n}{n!}.
$$

#### Remark {#fvr-vi-s1-n6-rem-1 .statement}

One can use formula (33) (resp. (34)) to calculate the $\beta_n$ (resp. the $u_n(x)$) by using the following lemma on entire series:

(1) Later we shall study series whose general terms are of the form $c_n z^n$ ($c_n \in \mathbf{C}, z \in \mathbf{C}$), which one calls *entire series*; in particular we shall see that when such a series is absolutely convergent for $z = z_0$ it is *normally convergent* for $|z| \leq |z_0|$.
(2) It follows from the theory of entire series that when one of these series is absolutely convergent in a neighbourhood $V$ of 0, the other is absolutely convergent in a neighbourhood $W \subset V$ of 0.

emma. **If two entire series** $\sum_{n=0}^{\infty} c_n \lambda^n,\ \sum_{n=0}^{\infty} d_n \lambda^n$ **are absolutely convergent for all** $\lambda$ **in a neighbourhood of** $0$, **and if** $\sum_{n=0}^{\infty} c_n \lambda^n = \sum_{n=0}^{\infty} d_n \lambda^n$ **for these values of** $\lambda$, **then** $c_n = d_n$ **for all integers** $n \geqslant 0$.

If, by any procedure, one can find an entire series that converges to $\lambda^p / u(\lambda)$ on a neighbourhood of $0$, then the coefficients of this series are necessarily equal to the $\beta_n / n!$. Is this procedure that we shall apply in the examples that follow.

#### Example 1 {#fvr-vi-s1-n6-exa-1 .statement}

If $U$ is the identity map one has $u(\lambda) = 1$ and the operator $U$ is clearly singular; since $u_n(x) = x^n$ the formula (27) of VI, p. 278, can be written, putting $\xi = \xi - \eta$

$$
f(x + h) = \sum_{n=0}^{\infty} \frac{1}{m!} f^{(m)}(h) x^m + \int_h^{x+h} f^{(n+1)}(t) \frac{(x + h - t)^n}{n!} dt
$$

that is, it reduces to the Taylor formula (II, p. 62).

#### Example 2 {#fvr-vi-s1-n6-exa-2 .statement}

Let us take for $U$ the composition operator which, to every function $f$ defined on $\mathbf{R}_+$, associates the function $x \mapsto f(x + 1) - f(x)$; then

$$
U_{\lambda}^{\xi} (f(\xi)) = f(x + 1) - f(x);
$$

we have seen (VI, p. 275) that the restriction of $U$ to $\mathbf{C}[X]$ is equal to $e^D - 1$. Since, on the other hand, $u(\lambda) = e^{\lambda} - 1$, the operator $U$ is *regular*; we shall see (VI, p. 288) how to determine the Bernoulli numbers $b_n$ by calculating an expansion of $\frac{\lambda}{e^{\lambda} - 1}$ as a convergent entire series. On applying formula (27) of VI, p. 278 to a *primitive* of a function $f$ admitting a continuous $n^{th}$ derivative on $\mathbf{R}_+$, we obtain

$$
f(x + h) = \int_h^{h+1} f(t) dt
$$
$$
+ \sum_{m=1}^n \frac{1}{m!} B_m(x) \left( f^{(m-1)}(h+1) - f^{(m-1)}(h) \right) + R_n(x, h)
$$

with

This lemma is a particular case of a general result that we will prove later; here is the proof. If an entire series $\sum_{n=0}^{\infty} c_n \lambda^n$ is absolutely convergent for $\lambda = \lambda_0$ then for every integer $k \geqslant 0$ the series $\sum_{n=0}^{\infty} c_{n+k} \lambda^n$ is normally convergent for $|\lambda| \leqslant |\lambda_0|$, so is continuous on this disc (*Gen. Top.*, X, p. 283); one concludes that $\sum_{n=k+1}^{\infty} c_n \lambda^n = o(\lambda^k)$ on a neighbourhood of $0$. The lemma then follows from the uniqueness of the coefficients of an asymptotic expansion of a function in terms of the $\lambda^n$ (V, p. 223).

$$
R_n(x, h) = - \int_0^{1-x} \frac{B_n(x + \eta)}{n!} f^{(n)}(h + 1 - \eta) d\eta \\
+ \int_0^{-x} \frac{B_n(x + \eta)}{n!} f^{(n)}(h - \eta) d\eta.
$$

(36)

#### Example 3 {#fvr-vi-s1-n6-exa-3 .statement}

Let E be the vector space of functions $f$ defined and continuous on $\mathbf{R}$, and such that the integral $\int_{-\infty}^{+\infty} f(x + \xi) e^{-\xi^2/2} d\xi$ converges for all $x \geq 0$. The operator U defined by

$$
U_\lambda^\xi \left( f(\xi) \right) = \frac{1}{\sqrt{2\pi}} \int_{-\infty}^{+\infty} e^{-\xi^2/2} f(x + \xi) d\xi
$$

is then defined on E and is clearly a composition operator. The space E contains all the exponentials $e^{\lambda x}$ ($\lambda$ arbitrary complex), and one has

$$
u(\lambda) = \frac{1}{\sqrt{2\pi}} \int_{-\infty}^{+\infty} e^{-(\xi^2/2) + \lambda \xi} d\xi \\
= \frac{1}{\sqrt{2\pi}} e^{\lambda^2/2} \int_{-\infty}^{+\infty} e^{-(\xi - \lambda)^2/2} d\xi = e^{\lambda^2/2}
$$

(cf. III, p. 120, exerc. 24, and VII, p. 313, formula (22)). One has $n! \alpha_n = U_0^\xi (\xi^n) = \frac{1}{\sqrt{2\pi}} \int_{-\infty}^{+\infty} e^{-\xi^2/2} \xi^n d\xi$. For every integer $n$ one can write

$$
\sum_{k=0}^n \int_{-\infty}^{+\infty} \frac{|\lambda \xi|^k}{k!} e^{-\xi^2/2} d\xi \leq 2 \int_0^{+\infty} e^{-(\xi^2/2) + |\lambda| \xi} d\xi.
$$

The series $\sum_{n=0}^{\infty} e^{-\xi^2/2} \frac{(\lambda \xi)^n}{n!}$ can therefore be integrated term-by-term over $\mathbf{R}$ (II, p. 72, cor. 1), which proves that the series $\sum_{n=0}^{\infty} \alpha_n \lambda^n$ converges absolutely for every $\lambda \in \mathbf{C}$, and has a sum equal to $u(\lambda) = e^{\lambda^2/2} = \sum_{n=0}^{\infty} \frac{\lambda^{2n}}{2^n n!}$; thus the operator $U$ is regular. Applying the lemma mentioned above shows that $\alpha_{2n} = 1/2^n n!,\ \alpha_{2n+1} = 0$ for every $n \geq 0$; the operator $U$ is thus of order 0. One has

$$
\frac{1}{u(\lambda)} = e^{-\lambda^2/2} = \sum_{n=0}^{\infty} \frac{(-1)^n \lambda^{2n}}{2^n n!},
$$

the series being absolutely convergent for every $\lambda \in \mathbf{C}$; another application of the lemma shows that $\beta_{2n} = \frac{(-1)^n (2n)!}{2^n n!},\ \beta_{2n+1} = 0$; further, the series $\sum_{n=0}^{\infty} \frac{\lambda^n}{n!} u_n(x)$ is absolutely convergent for every $\lambda \in \mathbf{C}$ and every $x \in \mathbf{R}$, and one has

$$
\sum_{n=0}^{\infty} \frac{\lambda^n}{n!} u_n(x) = \exp \left( -\frac{\lambda^2}{2} + \lambda x \right) = \exp \left( \frac{x^2}{2} \right) \exp \left( -\frac{1}{2} (\lambda - x)^2 \right).
$$

On applying the Taylor formula to the function $\exp(-x^2/2)$ one then obtains the following expression for the polynomials $u_n(x)$:

$$
u_n(x) = (-1)^n e^{\lambda^2/2} \frac{d^n}{dx^n} (e^{-x^2/2}).
$$

This polynomial is called the *Hermite polynomial* of degree $n$, and is often denoted by $\mathrm{H}_n(x)$. The formulae (7), (8) and (9) of VI, p. 273, here give

$$
\frac{d \mathrm{H}_n}{dx} = n \mathrm{H}_{n-1}(x)
$$

$$
\mathrm{H}_n(x+y) = \sum_{k=0}^n \binom{n}{k} \mathrm{H}_{n-k}(x) y^k
$$

$$
\frac{1}{\sqrt{2\pi}} \int_{-\infty}^{+\infty} e^{-\xi^2/2} \mathrm{H}_n(x+\xi) d\xi = x^n
$$

and the formula (27) of VI, p. 278, becomes, for $h = 0$

$$
\sqrt{2\pi} f(x) = \sum_{m=0}^n \left( \int_{-\infty}^{+\infty} e^{\xi^2/2} f^{(m)}(\xi) d\xi \right) \frac{\mathrm{H}_m(x)}{m!}
$$
$$
- \int_{-\infty}^{+\infty} d\xi \int_0^\xi \frac{\mathrm{H}_n(x+\eta)}{n!} e^{-(\xi+\eta)^2/2} f^{(n+1)}(x+\xi-\eta) d\eta.
$$

### 7. THE EULER-MACLAURIN SUMMATION FORMULA

In the formula (35) of VI, p. 280, let us replace $x$ by 0 and $h$ by $x$; since $\mathrm{B}_m(0) = b_m$ it follows from the relations (24) of VI, p. 276, that for each integer $p > 0$ one can write

$$
f(x) = \int_x^{x+1} f(t) dt - \frac{1}{2} (f(x+1) - f(x))
$$
$$
+ \sum_{k=1}^p \frac{b_{2k}}{(2k)!} \left( f^{(2k-1)}(x+1) - f^{(2k-1)}(x) \right) + R_p(x)
$$
with
$$
R_p(x) = - \frac{1}{(2p+1)!} \int_0^1 \mathrm{B}_{2p+1}(t) f^{(2p+1)}(x+1-t) dt.
$$
In this formula let us successively replace $x$ by $x+1, x+2, \ldots, x+n$, and combine the formulae obtained, one by one; we obtain

$$
\begin{cases}
f(x) + f(x+1) + \cdots + f(x+n) \\
= \int_x^{x+n+1} f(t) dt - \frac{1}{2} (f(x+n+1) - f(x)) \\
+ \sum_{k=1}^p \frac{b_{2k}}{(2k)!} \left( f^{(2k-1)}(x+n+1) - f^{(2k-1)}(x) \right) + T_p(x, n)
\end{cases}
$$
with
$$
T_p(x, n) = - \frac{1}{(2p+1)!} \int_0^1 \mathrm{B}_{2p+1}(t) \left( \sum_{k=0}^n f^{(2p+1)}(x+k+1-t) \right) dt.
$$

The remainder $T_p(x, n)$ in this formula can be rewritten in the following way: denote by $\overline{B}_{2p+1}(t)$ the *periodic* function with period 1 which is equal to $B_{2p+1}(t)$ on the interval $[0, 1[$. Then

$$
\int_0^1 B_{2p+1}(t) f^{(2p+1)}(x + k + 1 - t) \, dt = \int_k^{k+1} \overline{B}_{2p+1}(1 - s) f^{(2p+1)}(x + s) \, ds
$$

and consequently

$$
T_p(x, n) = - \frac{1}{(2p+1)!} \int_0^{n+1} \overline{B}_{2p+1}(1 - s) f^{(2p+1)}(x + s) ds.
$$ (41)

The formula (39) is called the *Euler-Maclaurin summation formula*; it is applicable to every complex function having a continuous $(2p + 1)^{th}$ derivative on an interval $[x_0, +\infty[$, for every $x \geq x_0$. We shall see (VI, p. 288) how to estimate the *remainder* $T_p(x, n)$ in this formula.

### Exercises {#fvr-vi-s1-exercises}

See the [exercises for § 1](exercises/s1/).
