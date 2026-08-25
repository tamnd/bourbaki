---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 4
section_title: Algebraically closed extensions
lang: en
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A V.19-A V.24, A V.150
pdf_pages: 0133-0138, 0264-0264
extraction: ocr
subsections:
    - "no": 1
      title: Algebraically closed fields
      page: 19
      pdf_page: 133
    - "no": 2
      title: Splitting extensions
      page: 21
      pdf_page: 135
    - "no": 3
      title: Algebraic closure of a field
      page: 22
      pdf_page: 136
statements: 19
exercises: 2
content_sha256: 0448b33c97d3ed2ba38e209e2edbe541f08218127e30ebd49790a9cf61517aa2
---

## § 4. ALGEBRAICALLY CLOSED EXTENSIONS

### 1. Algebraically closed fields

#### Proposition 1 {#alg-v-s4-prop-1 .statement}

— Let K be a field; then the following properties are equivalent:
(AC) Every non-constant polynomial of K[X] splits in K[X] into a product of polynomials of degree 1 (distinct or not).
(AC') Every non-constant polynomial of K[X] has at least one root in K.
(AC'') Every irreducible polynomial in K[X] is of degree 1.

(AC) Every algebraic extension of K is of degree 1 (in other words, K is relatively algebraically closed in every extension field of K).

Let us first prove the equivalence of the properties (AC), (AC') and (AC''). Clearly (AC) implies (AC). Since every non-constant polynomial of K[X] is divisible by an irreducible polynomial (IV, p. 13, Prop. 13) and every polynomial of degree 1 in K[X] clearly admits a root in K, we see that (AC) implies (AC'). The condition (AC') implies by induction on n, that every polynomial of degree n in K[X] is a product of n polynomials of degree 1 (IV, p. 14, Prop. 1), hence (AC') implies (AC).

It remains to see that (AC) and (AC) are equivalent. If (AC'') holds, every element of an extension field L of K which is algebraic over K is of degree 1 (V, p. 16, Th. 1), hence belongs to K, which establishes (AC). Conversely, let f be an irreducible polynomial of degree $n \geq 1$ in K[X]; the quotient algebra K[X]/(f) is of degree n over K and is a field, hence an algebraic extension of degree n of K (V, p. 18, Prop. 2). Now it is clear that (AC) implies (AC'').

#### Definition 1 {#alg-v-s4-def-1 .statement}

A field K is said to be algebraically closed if it possesses the (equivalent) properties (AC), (AC'), (AC), (AC).

\* Example 1. — The field C of complex numbers is algebraically closed (Gen. Top., VIII, p. 100). \*

A field K which is relatively algebraically closed in an extension field E of K is not necessarily algebraically closed (in effect every field is relatively algebraically closed in itself, and there exist fields that are not algebraically closed, for example Q or $\mathbf{F}_p$ \* or R *). However:

#### Proposition 2 {#alg-v-s4-prop-2 .statement}

Let $\Omega$ be an algebraically closed field and K a subfield of $\Omega$. Then the relative algebraic closure $\bar{K}$ of K in $\Omega$ is an algebraically closed field.

Let f be a non-constant polynomial in $\bar{K}[X] \subset \Omega[X]$. Since $\Omega$ is algebraically closed, the polynomial f has at least one root in $\Omega$, and since this root is algebraic over $\bar{K}$, it belongs to $\bar{K}$ (V, p. 19, Prop. 4). Therefore $\bar{K}$ satisfies (AC').

\* Example 2. — By Prop. 2 the set of all complex numbers that are algebraic over Q (often called briefly algebraic numbers) is an algebraically closed field. \*

#### Proposition 3 {#alg-v-s4-prop-3 .statement}

Every algebraically closed field is infinite.

Let K be a finite field and put $f(X) = 1 + \prod_{a \in K} (X - a)$. The polynomial $f \in K[X]$ is non-constant and $f(a) = 1$ for each $a \in K$. So the field K does not satisfy (AC') and hence is not algebraically closed.

#### Theorem 1 (Steinitz) {#alg-v-s4-thm-1 .statement}

Let K be a field, E an algebraic extension of K and $\Omega$ an algebraically closed extension of K; then there exists a K-homomorphism of E into R.

By V, p. 13, Scholium, there exists an extension field $\Omega'$ of $\Omega$ and a K-homomorphism u of E into $\Omega'$. Let $x \in E$; since x is algebraic over K, u(x) is algebraic over u(K) and *a fortiori* over $\Omega$ (V, p. 17, Cor. 2); since $\Omega$ is algebraically closed, we thus have $u(x) \in O$. It follows that $u$ maps $E$ into $O$.

### 2. Splitting extensions

#### Definition 2 {#alg-v-s4-def-2 .statement}

*Let K be a field and $(f_i)_{i \in I}$ a family of non-constant polynomials in $K[X]$. By a splitting extension of $(f_i)_i$, we understand any extension $E$ of $K$ with the following properties :*

*a) For each $i \in I$, the polynomial $f_i$ splits in $E[X]$ into a product of polynomials of degree 1.*

*b) For each $i \in I$ let $R_i$ be the set of roots of $f_i$ in $E$, then $E = K \left( \bigcup_{i \in I} R_i \right)$.*

Sometimes the term « splitting field » is used instead of « splitting extension ».

*Remarks. — 1) For each $i \in I$ let $c_i$ be a non-zero element of $K$ and let $f'_i = c_i f_i$. Then it is clear that every splitting extension for the family $(f_i)_i$, is also a splitting extension for the family $(f'_i)_{i \in I}$ and conversely. In particular, in studying splitting extensions we may limit ourselves to the case of monic polynomials.*

*2) Suppose that I is finite and put $f = \prod_{i \in I} f_i$. Using the uniqueness of the decomposition of a polynomial into irreducible factors in $E[X]$ (IV, p. 13, Prop. 13), we can easily show that a splitting extension for the polynomial $f$ is a splitting extension for the family $(f_i)_i$, and conversely. In other words, the case of a finite family may be reduced to the case of a single polynomial.*

*3) Let $f \in K[X]$ be a polynomial of degree $\geq 1$ and let $E$ be a splitting extension of $f$. If $x_1, \ldots, x_n$ are the roots off in $E$, we thus have $E = K(x_1, \ldots, x_n)$ and $[E : K]$ is finite ($V$, p. 18, Th. 2); but it may happen that $E$ is distinct from the subfields $K(x_1), \ldots, K(x_n)$ generated by a single root; this can happen even when $f$ is irreducible$^1$. We note however that when $f$ is irreducible, the fields $K(x_i)$ all have the same degree $n$ over $K$, and whenever $E$ is equal to one of them, we have $[E : K] = n$ and hence $E = K(x_1) = \cdots = K(x_n)$.*

#### Proposition 4 {#alg-v-s4-prop-4 .statement}

*Let K be a field and $(f_i)_{i \in I}$ a family of non-constant polynomials in $K[X]$; then there exists a splitting extension for the family $(f_i)_{i \in I}$.*

We may take the polynomials $f_i$ to be monic (Remark 1). Let $i \in I$ and let the degree of $f_i$ be $d_i$. By IV, p. 73, Prop. 5 there exists a commutative algebra $A$, over $K$, not reduced to 0, and elements $\xi_{i,1}, \ldots, \xi_{i,d_i}$ of $A_i$ such that :

*a) the algebra $A_i$ is generated by $(\xi_{i,1}, \ldots, \xi_{i,d_i})$;*

\footnotetext{1 Take for example $K = \mathbf{Q}$ and $f = X^3 - 2$.}

b) we have $f_i(X) = \prod_{k=1}^{d_i} (X - \xi_{i,k})$ in $A_i[X]$.

Let $A$ be the tensor product of the family of algebras $(A,)_{i}$, and let $\varphi_i$ be the canonical homomorphism of $A_i$ into $A$ (III, p. 470). The algebra $A$ is then commutative and not reduced to 0; by Krull's theorem (I, p. 104), there exists thus a maximal ideal $a$ in $A$ and $E = A/a$ is an extension of the field $K$.

Denote by $\psi$ the canonical homomorphism of $A$ into $E$ and put $x_{i,k} = \psi(\varphi_i(\xi_{i,k}))$ for $i \in I$ and $l \leq k \leq d_i$. Since the algebra $A$ is generated by $\bigcup \varphi_i(A_i)$, the extension $E$ is generated by the family $(x_{i,k})$. Further, we have $i \in I$

$$
f_i(X) = \prod_{k=1}^{d_i} (X - x_{i,k}) \text{ in } E[X]. $$

Therefore $E$ is a splitting extension of the family $(f_i)_{i \in I}$.

#### Proposition 5 {#alg-v-s4-prop-5 .statement}

— *Let K be a field, $(f_i)_{i \in I}$ a family of non-constant polynomials in $K[X]$, E an extension of K, and F, F' subextensions of E which are each a splitting extension of $(f_i)_{i \in I}$. Then $F = F'$.

Let $R_i$ be the set of roots of $f_i$ in E and $R = \bigcup_{i \in I} R_i$. Since $f_i$ is a product of polynomials of the first degree lying in $F[X]$, we have $R_i \subset F$. By Def. 2, we have $F = K(R)$; in the same way we find that $F = K(R)$.

#### Corollary {#alg-v-s4-n2-cor-1 .statement}

— *Let K be a field, $(f_i)_{i \in I}$, a family of non-constant polynomials in $K[X]$ and F, F' splitting extensions of $(f_i)_{i \in I}$. Then there exists a K-isomorphism of F onto F.

This follows from Prop. 5 and V, p. 13, Cor. of Prop. 4.

### 3. Algebraic closure of a field

#### Definition 3 {#alg-v-s4-def-3 .statement}

— *Let K be a field. By an algebraic closure of K we understand any extension of K which is algebraic and algebraically closed.

#### Example 1 {#alg-v-s4-n3-exa-1 .statement}

The field C of complex numbers is an algebraic closure of the field R of real numbers (Gen. Top., VIII, p. 100) *
2) Let K be a field and $\Omega$ an algebraically closed extension of K. If $\overline{K}$ is the relative algebraic closure of K in $\Omega$, then by V, p. 20, Prop. 2, K is an algebraic closure of K. * In particular the field of all algebraic numbers (V, p. 20, Ex. 2) is an algebraic closure of the field Q of rational numbers. *

#### Proposition 6 {#alg-v-s4-prop-6 .statement}

— *Let $\Omega$ be an extension of a field K. For $\Omega$ to be an algebraic closure of K it is necessary and sufficient that it should be algebraic and that each non-constant polynomial in $K[X]$ should split in $\Omega[X]$ into a product of factors of degree 1.

The condition is necessary by (AC). Conversely, suppose that $\Omega$ is algebraic over $K$ and every non-constant polynomial over $K[X]$ is a product in $\Omega[X]$ of factors of degree 1. Let $\Omega'$ be an algebraic extension of $\Omega$ and let $x \in \Omega'$. Since $x$ is algebraic over $\Omega$ and $\Omega$ is algebraic over $K$, $x$ is algebraic over $K$ (V, p. 19, Prop. 3). Let $f$ be the minimal polynomial of $x$ over $K$. By hypothesis the polynomial $f \in K[X]$ splits in $\Omega[X]$ into a product of factors of degree 1, whence $x \in \Omega$. Thus we have $\Omega' = \Omega$ and $\Omega$ is algebraically closed because it satisfies (AC).

#### Remark 1 {#alg-v-s4-n3-rem-1 .statement}

If $\Omega$ is algebraic over $K$ and if every non-constant polynomial of $K[X]$ has a root in $\Omega$ then $\Omega$ is an algebraic closure of $K$ (V, p. 156, Ex. 20).

#### Proposition 7 {#alg-v-s4-prop-7 .statement}

— *Let $\Omega$ be an algebraic extension of a field $K$.
a) If $\Omega$ is algebraically closed, then every algebraic extension of $K$ is isomorphic to a subextension of $\mathbf{R}$.
b) Conversely suppose that every algebraic extension of finite degree of $K$ is isomorphic to a subextension of $\Omega$; then $\Omega$ is algebraically closed.*

Assertion *a)* follows from Th. 1 (V, p. 20). Now assume the hypotheses of *b)* and consider a non-constant polynomial $f \in K[X]$. Let E be a splitting field of $f$ (V, p. 21, Prop. 4); since E is algebraic of finite degree over $K$ (V, p. 18, Th. 2), we may suppose that E is a subextension of $\Omega$. Then the polynomial $f$ is a product of polynomials of degree 1 in $\Omega[X]$ and Prop. 6 shows that $\Omega$ is algebraically closed.

We can now prove the existence and uniqueness (up to isomorphism) of the algebraic closure of a field.

#### Theorem 2 (Steinitz) {#alg-v-s4-thm-2 .statement}

— *Let $K$ be a field; then there exists an algebraic closure of $K$. If $\Omega$ and $\Omega'$ are two algebraic closures of $K$, there exists a $K$-isomorphism of $\Omega$ onto $\Omega'$.*

By Prop. 6 an algebraic closure of $K$ is nothing other than a splitting extension for the set of all non-constant polynomials in $K[X]$. Th. 2 therefore follows from V, p. 21, Prop. 4 and V, p. 22, Cor.

#### Corollary {#alg-v-s4-n3-cor-1 .statement}

— *Let $K$ and $K'$ be two fields, $\Omega$ an algebraic closure of $K$ and $\Omega'$ an algebraic closure of $K'$. For every isomorphism $u$ of $K$ onto $K'$ there exists an isomorphism $v$ of $\Omega$ onto $\Omega'$ extending $u$.*

It is enough to apply Th. 2 to the algebraic closures $\Omega$ and $(\Omega', u)$ of $K$.

#### Remark 2 {#alg-v-s4-n3-rem-2 .statement}

In the notation of the preceding Corollary there exist in general $K$-automorphisms of $\Omega$ distinct from the identity. Hence there is in general no uniqueness about the isomorphism $v$ of $\Omega$ onto $\Omega'$ extending the isomorphisms $u$ of $K$ onto $K'$. For similar reasons there is in general more than one isomorphism of a splitting extension $E$ onto a splitting extension $E'$ for the same family $(f_i)_{i \in I}$ of polynomials. We recall that by contrast, for the perfect closure we have uniqueness (V, p. 5).

#### Remark 3 {#alg-v-s4-n3-rem-3 .statement}

Let K be a field and $\Omega$ an algebraic closure of $K$. Then the following construction may be given for a splitting extension for a family $(f_i)_{i \in I}$ of non-constant polynomials in $K[X]$: let $R_i$ be the set of roots of $f_i$ in $\Omega$ and let $R = \bigcup_{i \in I} R_i$. Then $K(R)$ is the unique subextension of $\Omega$ which is a splitting extension for $(f_i)_{i \in I}$ (V, p. 22, Prop. 5).

#### Remark 4 {#alg-v-s4-n3-rem-4 .statement}

Let K be a finite field and $\Omega$ an algebraic closure of $K$. Then $\Omega$ is infinite ($V,$ p. 20, Prop. 3); since every extension of finite degree of K is a finite field, $\Omega$ is an algebraic extension of *infinite* degree of $K$.

### Exercises {#alg-v-s4-exercises}

See the [exercises for § 4](exercises/s4/).
