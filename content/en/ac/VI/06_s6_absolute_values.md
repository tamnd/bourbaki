---
book: ac
book_title: Commutative Algebra
chapter: VI
chapter_title: VALUATIONS
section: 6
section_title: Absolute values
lang: en
source: ac-i-vii
book_pages: 403-411, 459-460
pdf_pages: 0421-0429, 0477-0478
extraction: ocr
subsections:
    - "no": 1
      title: PRELIMINARIES ON ABSOLUTE VALUES
      page: 403
      pdf_page: 421
    - "no": 2
      title: ULTRAMETRIC ABSOLUTE VALUES
      page: 405
      pdf_page: 423
    - "no": 3
      title: ABSOLUTE VALUES ON Q
      page: 406
      pdf_page: 424
    - "no": 4
      title: STRUCTURE OF FIELDS WITH A NON-ULTRAMETRIC ABSOLUTE VALUE
      page: 407
      pdf_page: 425
statements: 10
exercises: 2
content_sha256: 578267c10123fcc3d07b0471b59c89f82aaafae830bfa33156bb526052bd76d0
---

## 6. ABSOLUTE VALUES

### 1. PRELIMINARIES ON ABSOLUTE VALUES

Let $K$ be a field (commutative or not). Recall (General Topology, Chapter IX, § 3, no. 2, Definition 2) that an absolute value on $K$ is any mapping $f$ from $K$ to $\mathbf{R}_+$ satisfying the following axioms:

(VA,) The relation $f(x) = 0$ is equivalent to $x = 0$.
(VAII) $f(xy) = f(x)f(y)$ for all $x, y$ in $K$.
(VAIll) $f(x + y) \leq f(x) + f(y)$ for all $x, y$ in $K$.

It follows from (VA,) and (VAII) that $f(1) = 1, f(-1) = 1$ and
$$
f(x^{-1}) = \frac{1}{f(x)}
$$
for $x \neq 0$.

For a mapping $f$ from $K$ to $\mathbf{R}$, and a real number $A > 0$, let $(\mathrm{U}_A)$ denote the relation
$$
f(x + y) \leq A \cdot \sup(f(x), f(y)) \quad \text{for all } x, y \text{ in } K.
$$

We shall denote by $\mathscr{V}(K)$ the set of mappings $f$ from $K$ to $\mathbf{R}_+$ satisfying (VAI) and (VAII) and for which there exists an $A > 0$ (depending on $f$) such that $(\mathrm{U}_A)$ holds.

Note that iff $\in \mathscr{V}(K)$, then, putting $x = 1, y = 0$ in $(\mathrm{U}_A)$,
$$
1 = f(1) \leq A \cdot \sup(f(1), f(0)) = A.
$$

#### Proposition 1 {#ac-vi-s6-prop-1 .statement}

For a mapping $f$ from $K$ to $\mathbf{R}$, satisfying (VA,) and (VAII) to belong to $\mathscr{V}(K)$, it is necessary and sufficient that $f(1 + x)$ be bounded in the set of $x \in K$ such that $f(x) \leq 1$.

If $f$ satisfies $(\mathbf{U}_A)$, then $f(1 + x) \leq A$ if $f(x) \leq 1$. Conversely, suppose that $f(x + 1) \leq A$ for the $x \in K$ such that $f(x) \leq 1$ (which implies that $A \geq f(1) = 1$); then, if $x = 0$ or $y = 0$, condition $(\mathbf{U}_A)$ is fulfilled; if on the other hand $x \neq 0$ and $y \neq 0$, we may assume for example that $f(y) \leq f(x)$, hence, by $(\mathbf{VA}_s)$, $f(yx^{-1}) \leq 1$ and therefore $f(1 + yx^{-1}) \leq A$, which gives, by virtue of $(\mathbf{VA}_{II})$, $f(x + y)f(x)^{-1} \leq A$; whence

$$
f(x + y) \leq Af(x) \leq A \sup(f(x), f(y)).
$$

If $f$ is an absolute value on $K$, then $f(n.1) \leq n$ by induction on the integer $n > 0$ starting from $(\mathbf{VA}_{III})$; conversely:

#### Proposition 2 {#ac-vi-s6-prop-2 .statement}

*Let $f$ be a mapping of $K$ to $\mathbf{R}_+$ belonging to $\mathcal{V}(K)$; if there exists $C > 0$ such that $f(n.1) \leq C$ for every integer $n > 0$, $f$ is an absolute value on $K$.*

By induction on $r > 0$ we deduce from $(\mathbf{U}_A)$ the relation

$$(1)$$
$$
f(x_1 + x_2 + \cdots + x_{2^r}) \leq A^r \sup_{1 \leq i \leq 2^r} f(x_i)
$$

for every family $(x_i)$ of $2^r$ elements of $K$. We set $n = 2^r - 1$; for all $x \in K$, we deduce from (1)

$$
(f(1 + x))^n = f((1 + x)^n) = f\left( \sum_{i=0}^n \binom{n}{i} x^i \right) \leq A^r \sup \left( f\left( \binom{n}{i} \right) (f(x))^i \right)
$$
$$
\leq CA^r \sum_{i=0}^n \binom{n}{i} (f(x))^i = CA^r (1 + f(x))^n
$$

for $f\left( \binom{n}{i} \right) \leq C \binom{n}{i}$; therefore
$$
f(1 + x) \leq C^{1/n} A^{r/n} (1 + f(x)).
$$

Letting $r$ tend to $+\infty$, we obtain $f(1 + x) \leq 1 + f(x)$ for all $x \in K$; applying this inequality with $x$ replaced by $xy^{-1}$ (where $y \neq 0$) and taking account of $(\mathbf{VA}_{II})$, we obtain relation $(\mathbf{VA}_{III})$, which proves the proposition.

#### Corollary 1 {#ac-vi-s6-prop-2-cor-1 .statement}

*For a mapping $f$ from $K$ to $\mathbf{R}_+$ to be an absolute value, it is necessary and sufficient that it satisfy conditions $(\mathbf{VA}_I)$, $(\mathbf{VA}_{II})$ and $(\mathbf{U}_2)$.*

It is necessary, for $(\mathbf{VA}_{II})$ implies
$$
f(x + y) \leq f(x) + f(y) \leq 2 \sup(f(x), f(y)).
$$

Conversely, suppose $f$ satisfies $(\mathbf{VA}_I)$, $(\mathbf{VA}_s)$ and $(\mathbf{U}_2)$; for every integer $n > 0$, let $r$ be the least integer such that $2^r \geq n$; if in (1) $A$ is replaced by 2, the $x_i$ of index $i \leq n$ by 1 and the $x_i$ of index $i > n$ by 0, we obtain
$$
f(n.1) \leq 2^r < 2n;
$$
then Proposition 2 may be applied with $C = 2$ and hence $f$ is an absolute value.

#### Corollary 2 {#ac-vi-s6-prop-2-cor-2 .statement}

For a mapping $f$ of $K$ to $\mathbf{R}_+$ to belong to $\mathcal{V}(K)$, it is necessary and sufficient that it be of the form $g^t$, where $t > 0$ and $g$ is an absolute value on $K$.

To say that $f$ satisfies $(\mathbf{U}_A)$ is equivalent to saying that $f^s$ satisfies $(\mathbf{U}_{A^s})$; as there exists $s > 0$ such that $A^s \leq 2$, Corollary 1 shows that for such a value of $s$, $f^s$ is an absolute value.

### 2. ULTRAMETRIC ABSOLUTE VALUES

A mapping $f$ of $K$ to $\mathbf{R}_+$ is called an ultrametric absolute value if it satisfies conditions $(\mathrm{VA}_I)$, $(\mathrm{VA}_{II})$ and $(\mathrm{U},)$ (which obviously implies that $f$ is an absolute value).

#### Proposition 3 {#ac-vi-s6-prop-3 .statement}

Let $f$ be a mapping of $K$ to $\mathbf{R}_+$. The following properties are equivalent:
(a) $f$ is an ultrametric absolute value.
(b) There exists a valuation $v$ on $K$ with values in $\mathbf{R}$ and a real number $a$ such that $0 < a < 1$ and $f = a''$.
(c) $f$ belongs to $\mathcal{V}(K)$ and $f(n.1) \leq 1$ for every integer $n > 0$.
(d) For all $s > 0$, $f^s$ is an absolute value.

For every real number $c$ such that $0 < c < 1$, the mapping $t \mapsto c^t$ is an isomorphism of the ordered group $\mathbf{R}$ (with the opposite ordering to the usual ordering) on the ordered group $\mathbf{R}_+^*$; this shows the equivalence of (a) and (b). Clearly (a) implies (c); (c) implies (d), for we deduce from (c) that
$$
(f(n.1))^s \leq 1 \leq n
$$
for every integer $n > 0$ and Proposition 2 of no. 1 shows that $f''$ is an absolute value. Finally (d) implies (a): for iff" is an absolute value, it satisfies $(\mathbf{U}_2)$ and hence $f$ satisfies $(\mathbf{U}_{2^{1/s}})$ for all $s > 0$ and therefore also $(\mathbf{U}_1)$, letting $s$ tend to $+\infty$.

#### Corollary {#ac-vi-s6-n2-cor-1 .statement}

If $K$ is a (not necessarily commutative) field of characteristic $p > 0$, every function on $\mathcal{V}(K)$ is an ultrametric absolute value.

Every non-zero element $z = n.1$ ($n$ an integer $> 0$) belongs to the prime subfield $\mathbf{F}_p$ of $K$ and hence satisfies the relation $z^{p-1} = 1$, which implies $f(z) = 1$ and we may apply Proposition 3 (c).

Given a real number $c$ such that $0 < c < 1$, the formulae
$$
f(x) = c^{v(x)}, \quad v(x) = \log, f(x)
$$
therefore establish a one-to-one correspondence between ultrametric absolute values on $K$ and valuations on $K$ with real values. The improper valuation corresponds to the improper absolute value (General Topology, Chapter IX, § 3, no. 2). Let $v_1, v_2$ be two valuations on $K$ with real values and $f_1, f_2$ the corresponding absolute values; for $v_1$ and $v_2$ to be equivalent, it is necessary and sufficient that $f_1$ and $f_2$ be so: for to say that $v_1$ and $v_2$ are equivalent amounts to saying that the relations $v_1(x) \geq 0$ and $v_2(x) \geq 0$ are equivalent or again that the relations $f_1(x) \leq 1$ and $f_2(x) \leq 1$ are equivalent; it is therefore sufficient to apply Proposition 5 of *General Topology*, Chapter IX, § 3, no. 2. Moreover (*loc. cit.*) for the topologies defined on K by $f_1$ and $f_2$ to be identical, it is necessary and sufficient that $f_1$ and $f_2$ be equivalent.

### 3. ABSOLUTE VALUES ON Q

#### Proposition 4 {#ac-vi-s6-prop-4 .statement}

*Let $f$ be a mapping of $\mathbf{Q}$ to $\mathbf{R}_+$ belonging to $\mathcal{V}(\mathbf{Q})$. Then:*

(i) *Either $f$ is the improper absolute value on $\mathbf{Q}$.*

(ii) *Or there exists a real number $a$ and a prime number $p$ such that $0 < a < 1$ and $f = a^{v_p}$, where $v_p$ is the $p$-adic valuation.*

(iii) *Or there exists $s > 0$ such that $f(x) = |x|^s$ for all $x \in \mathbf{Q}$.*

*In care (iii) for $f$ to be an absolute value on $\mathbf{Q}$, it is necessary and sufficient that $0 < s \leq 1$.*

Suppose first that $f(n) \leq 1$ for every integer $n > 0$. By Proposition 3 of no. 2 there exist a real number $b$ and a valuation $v$ on $\mathbf{Q}$ such that $0 < b < 1$ and $f = b^v$. Now, we know (\S 3, no. 4, *Example 4*) that the only valuations on $\mathbf{Q}$ are (up to equivalence) the improper valuation and the $p$-adic valuations $v_p$; we therefore have either case (i) or case (ii).

Suppose from now on that there exists an integer $h > 0$ such that $f(h) > 1$; by no. 1, Corollary 2 to Proposition 2, there exists a number $\rho > 0$ such that $f^\rho$ is an absolute value; let us write

$$
g(x) = \rho \log(f(x))/\log|x|
$$

for every rational number $x \neq 0$. Let $a, b$ be two integers $\geq 2$; for every integer $n \geq 2$ let $q(n)$ denote the integral part of $n \log a/\log b$, in other words the least integer $m$ such that $a^n < b^{m+1}$; the expansion of $a^n$ to base $b$ is therefore

$$
a^n = c_0 + c_1 b + \ldots + c_{q(n)} b^{q(n)}
$$

where $0 \leq c_i < b$ for $0 \leq i \leq q(n)$. As $f^\rho$ is an absolute value, $f^\rho(c_i) \leq c_i \leq b$ and we therefore deduce from (2) that

$$
(f(a))^{n\rho} = (f(a^n))^\rho \leq b(1 + (f(b))^\rho + \ldots + (f(b))^{q(n)\rho})
$$
$$
\leq b(q(n) + 1)(\sup(1, (f(b))^\rho))^{q(n)}.
$$

Taking logarithms on both sides of this inequality and dividing by $n \log a$, we obtain

$$
g(a) \leq \frac{\log b}{n \log a} + \frac{\log(q(n) + 1)}{q(n)} \cdot \frac{q(n)}{n \log a} + \frac{\sup(0, \rho \log f(b))}{\log a} \cdot \frac{q(n)}{n}.
$$

Note now that as $n$ tends to $+\infty$, $q(n)/n$ tends to $\log a/\log b$; therefore $q(n)$ tends to $+\infty$ and

$$
\log(q(n) + 1)/q(n)
$$

tends to 0 (Functions of a Real Variable, Chapter III, § 2, no. 1). Taking the limit in (3), we obtain

(4) $$
g(a) \leq \frac{\sup(0, \rho \log f(b))}{\log b} = \sup(0, g(b)).
$$

But $f(h) > 1$, whence $g(h) > 0$; if $a$ is replaced by $h$ in (4), we obtain $\sup(0, g(b)) > 0$ and hence

$$
\sup(0, g(b)) = g(b).
$$

Then, for any integers $a, b$ at least equal to 2, $g(a) \leq g(b)$ and therefore $g(a) = g(b)$, exchanging the roles of $a$ and $b$. In other words, there exists a constant $\lambda$ such that $g(a) = A$ for every integer $a \geq 2$; if we write $s = \lambda / \rho$, then $f(a) = |a|^s$ for every integer $a \geq 2$. As $f(xy) = f(x)f(y)$ and $f(-x) = f(x)$, $f(x) = |x|^s$ for all $x \in Q$. Finally, if $0 < s \leq 1$, we know that $x \mapsto |x|^s$ is an absolute value (General Topology, Chapter IX, § 3, no. 2); conversely, if $s$ is such that $x \mapsto |x|^s$ is an absolute value on $Q$, then $(1 + 1)^s \leq 1^s + 1^s$, that is $2^s \leq 2$, whence $s \leq 1$.

### 4. STRUCTURE OF FIELDS WITH A NON-ULTRAMETRIC ABSOLUTE VALUE

#### Theorem 1 (Gelfand-Mazur) {#ac-vi-s6-thm-1 .statement}

Let $K$ be an algebra over the field $\mathbf{R}$ with the two following properties:
(1) $K$ is a (not necessarily commutative) field.
(2) There exists on $K$ a norm $x \mapsto \|x\|$ compatible with the algebra structure on $K$ (General Topology, Chapter IX, § 3, no. 7, Definition 9).
Then the algebra $K$ is isomorphic to one of the algebras $\mathbf{R}, \mathbf{C}$ or $\mathbf{H}$.

Recall (loc. cit.) that it may always be assumed that $\|xy\| \leq \|x\| \cdot \|y\|$ for all $x, y$ in $K$. We shall give $K$ the topology (compatible with the algebra structure) defined by the norm.

(A) First case: $K$ is commutative and there exists $j \in K$ such that $j^2 = -1$

Then there exists an isomorphism $\sigma$ of the field $\mathbf{C}$ onto a subfield of $K$ such that $\sigma(\xi + i\eta) = \xi . 1 + \eta . j$ for $\xi, \eta$ in $\mathbf{R}$. We shall prove by reductio ad absurdum that $K = \sigma(\mathbf{C})$. Suppose then that there exists $x \in K - \sigma(\mathbf{C})$; for all $z \in \mathbf{C}, x - \sigma(z)$ is therefore invertible in $K$; let us write $F(z) = (x - \sigma(z))^{-1}$; as $\sigma$ is continuous and the inverse is continuous on $K$ (General Topology, Chapter IX, § 3, no. 7, Proposition 13 applied to the completion algebra of $K$), $F$ is a continuous mapping of $\mathbf{C}$ to $K$. Moreover, we may write for $z \neq 0$

$$
F(z) = (\sigma(z))^{-1}(x(\sigma(z))^{-1} - 1)^{-1}.
$$

But, as $(\sigma(z))^{-1} = \sigma(z^{-1})$ tends to 0 as $z$ tends to infinity in $\mathbf{C}$, it is seen that $F(z)$ tends to 0; in other words, $z \mapsto \|F(z)\|$ is a continuous real-valued function, $\geq 0$ on $\mathbf{C}$, tending to 0 at the point at infinity and which can therefore be considered as a continuous function on the compact space $\tilde{C}$ obtained by adjoining to $C$ a point at infinity. The least upper bound $a$ of $\| F \|$ on $C$ is therefore finite and $> 0$ and the set $P$ of complex numbers $z$ such that $\| F(z) \| = a$ is closed and non-empty (*General Topology*, Chapter IV, § 6, no. 1, Theorem 1).

Let $z \in P$; let us write $y = x - \sigma(z)$ and let $t$ be a complex number $\neq 0$ such that $\| \sigma(t) \| < \alpha^{-1}$, whence $\| \sigma(t) \cdot y^{-1} \| < 1$ by definition of $a$. The sequence of the $(\sigma(t) y^{-1})^n$ and that of the $n(\sigma(t) y^{-1})^n$ therefore tend to 0 in $K$ as $n$ tends to $+\infty$, for so do the corresponding sequences of norms in $R$. On the other hand note that for every polynomial $H(T) = \prod_{k=1}^p (T - \sigma(c_k))$, where the $c_k$ are distinct complex numbers, in the field $K(T)$ of rational functions

$$
\frac{H'(T)}{H(T)} = \sum_{k=1}^p \frac{1}{T - \sigma(c_k)}
$$

We apply this formula to the polynomial

$$
H(T) = T^n - (\sigma(t))^n = \prod_{k=0}^{n-1} (T - \sigma(\omega_n^k t)),
$$

where $\omega_n = \exp(2\pi i / n)$, and substitute for $T$ the element $y \in K$, which is distinct from all the $\sigma(\omega_n^k t)$. It follows (in the commutative field $K$) that

$$
\frac{ny^{n-1}}{y^n - (\sigma(t))^n} = \frac{1}{y - \sigma(t)} + \sum_{k=1}^{n-1} \frac{1}{y - \sigma(\omega_n^k t)}.
$$

Taking account of the definitions of $F$ and $y$, we obtain

$$
\begin{align}
F(z + t) + \sum_{k=1}^{n-1} F(z + \omega_n^k t) - nF(z) \\
= \frac{ny^{n-1}}{y^n - (\sigma(t))^n} - \frac{n}{y} = \frac{1}{y} \cdot \frac{n(\sigma(t) y^{-1})^n}{1 - (\sigma(t) y^{-1})^n}.
\end{align}
$$

But by virtue of the choice of $t$ and the remarks made above, the last expression in (7) tends to 0 as $n$ tends to $+\infty$; hence

$$
\| F(z + t) \| = \lim_{n \to +\infty} \| nF(z) - \sum_{k=1}^{n-1} F(z + \omega_n^k t) \|.
$$

Now, $\| F(z) \| = \alpha$ and $\| F(z + \omega_n^k t) \| \leq \alpha$ by definition of $\alpha$, whence

$$
\| nF(z) - \sum_{k=1}^{n-1} F(z + \omega_n^k t) \| \geq n \| F(z) \| - \sum_{k=1}^{n-1} \| F(z + \omega_n^k t) \| \geq n \alpha - (n-1)\alpha = \alpha.
$$

Therefore by (8), letting n tend to $+\infty$, $\|F(z + t)\| \geq a$ and by definition of $a$ this implies
$$
\|F(z + t)\| = \alpha,
$$
in other words $z + t \in P$. This proves that the set $P$ is *open* in $\mathbf{C}$; as it is also closed and non-empty and $\mathbf{C}$ is connected, $P = \mathbf{C}$ and $\|F\|$ is therefore constant on $\mathbf{C}$; as this function tends to 0 at the point at infinity, $\|F(z)\| = 0$ in $\mathbf{C}$ and in particular $\|F(0)\| = \|x^{-1}\| = 0$, which is absurd.

(B) *Second case; K is commutative and* $-1$ *is not the square of an element of K*
Let L be the commutative field obtained by adjoining to K a root j of $T^2 + 1$; L is a vector space over K admitting $(1, j)$ as a basis and L is obviously an algebra over $\mathbf{R}$. Clearly the function $x + yj \to \|x\| + \|y\|$ is a norm on L compatible with its structure as a vector space over $\mathbf{R}$; on the other hand, for $z = x + yj, z' = x' + y'j$ in L,
$$
\begin{align*}
\|zz'\| &= \|xx' - yy'\| + \|xy' + x'y\| \\
&\leq \|x\|.\|x'\| + \|y\|.\|y'\| + \|x\|.\|y'\| + \|x'\|.\|y\| \\
&= (\|x\| + \|y\|)(\|x'\| + \|y'\|) = \|z\|.\|z'\|.
\end{align*}
$$
The norm thus defined is consequently compatible with the R-algebra structure on L. By case (A) L is an R-algebra isomorphic to $\mathbf{C}$; now the only sub-R-algebra of $\mathbf{C}$ distinct from $\mathbf{C}$ is $\mathbf{R}$ and hence K is isomorphic to $\mathbf{R}$.

(C) *Third case: K is not commutative*
Let Z be the centre of K and x an element of K not in Z; the subfield $Z(x)$ of K is commutative and the norm induced by that on K is compatible with the R-algebra structure on $Z(x)$; as $Z \neq Z(x)$ and Z and $Z(x)$ are R-algebras isomorphic to $\mathbf{R}$ or $\mathbf{C}$ by virtue of (A) and (B), Z is necessarily isomorphic to $\mathbf{R}$ and $Z(x)$ to $\mathbf{C}$. For all $x \in K, Z(x)$ is therefore of rank $\leq 2$ over Z. Now we have the following lemma:

#### Lemma 1 {#ac-vi-s6-lem-1 .statement}

*Let D be a field with centre L such that, for all $x \in D, L(x)$ is an extension of L of degree $\leq m$. Then the rank of D over L is $\leq m^2$.*

We may obviously restrict our attention to the case where $D \neq L$. Then there exists in D a finite *separable* algebraic commutative extension E of L of degree $> 1$ (*Algebra*, Chapter VIII, § 10, no. 3, Lemma 1); as $E = L(x)$ for some suitable x in E (*Algebra*, Chapter V, § 7, no. 7, Proposition 12 and Chapter VII, § 5, no. 7), by hypothesis $[E : L] \leq m$. Suppose the separable extension E is taken such that $[E : L]$ is finite and as great as possible and consider the *centralizer* $E' \supset E$ of E in D, which is a field of centre E such that
$$
[D : E'] = [E : L] \leq m
$$

(Algebra, Chapter VIII, § 10, no. 2, Theorem 2). If E $\#$ E', there would exist in $\mathbf{E}'$ a finite separable algebraic extension F of $\mathbf{E}$ of degree $> 1$ (Algebra, Chapter VIII, § 10, no. 3, Lemma 1); F would therefore be a finite separable algebraic extension of L (Algebra, Chapter V, § 7, no. 4, Proposition 7) of degree $> [\mathrm{E}: \mathrm{L}]$, contrary to the definition of E; therefore $\mathbf{E}' = \mathbf{E}$, whence $[\mathrm{D}: \mathrm{L}] = [\mathrm{D}: \mathrm{E}][\mathrm{E}: \mathrm{L}] \leq m^2$.

Applying this lemma to K with $m = 2$, it is seen that K is a non-commutative extension field of R of finite rank and hence isomorphic to the field of quaternions $\mathbf{H}$ (Algebra, Chapter VIII, § 11, no. 2, Theorem 2).

Remark (1) We shall give in the chapter devoted to normed algebras a shorter proof of the Gelfand-Mazur Theorem which is valid for every Hausdorff locally convex topological algebra K over R and whose principle is the following: it is reduced (as in cases (B) and (C)) to the case where K is a commutative algebra over $\mathbf{C}$; if $x \in \mathbf{K} - \mathbf{C}.1$, we consider as above the mapping $z \mapsto (x - z.1)^{-1}$ of $\mathbf{C}$ to K, which is continuous and differentiable on $\mathbf{C}$. For every element $x'$ of the dual $\mathbf{K}'$ of the locally convex space K, $z \mapsto \langle (x - z.1)^{-1}, x' \rangle$ is then a bounded integral function on $\mathbf{C}$ and therefore constant by Liouville's Theorem and we conclude as in part (A) of the proof of Theorem 1 that this necessarily implies $\langle (x - z.1)^{-1}, x' \rangle = 0$ for all $z \in \mathbf{C}$ and all $x' \in \mathbf{K}'$; the Hahn-Banach Theorem shows that this conclusion is absurd, since $(x - z.1)^{-1} \neq 0$. Note that the argument in part (A) of the proof of Theorem 1 differs from the above only in appearance, for this argument is only a special case of that which serves to prove the maximum principle for analytic functions, the summation over the roots of unity and and passing to the limit being equivalent to calculating the integral $\int_{\gamma} \frac{\mathbf{F}(z + t)}{t} dt$ along a circle of centre 0 and the use of Cauchy's formula being avoided here, thanks to the particular form of the function F.

Theorem 2 (Ostrowski). Let K be a (not necessarily commutative) field and f an element $\mathcal{V}(K)$ which is not an ultrametric absolute value. Then there exist a unique real number $s > 0$ and an isomorphism j of K onto an everywhere dense subfield of one of the fields $\mathbf{R}, \mathbf{C}$ or $\mathbf{H}$ such that $f(x) = |j(x)|^s$ for all $x \in K$ (*). For f to be an absolute value on K, it is necessary and sufficient that $s \leq 1$.

By no. 2, Corollary to Proposition 3, K is of characteristic 0 and hence an algebra over $\mathbf{Q}$; for all $x \in \mathbf{Q}$ we write $h(x) = f(x.1)$; clearly $h \in \mathcal{V}(\mathbf{Q})$ and therefore Proposition 4 of no. 3 may be applied; neither of cases (i) and (ii) of the statement of this proposition can hold, for this would imply $f(n.1) \leq 1$ for every integer $n > 0$ and f would be an ultrametric absolute value by virtue

(*) On $\mathbf{H}$ we write $|z|^2 = z.\bar{z} = \bar{z}.z$, $\bar{z}$ being the conjugate quaternion of $z$.

of no. 2, Proposition 3. Then there exists a real number s > 0 such that h(x) = |x|^s for all x ∈ Q, that is f(x.1) = |x|^s; we write g = f^{1/s}. Then g ∈ V(K) and g(n.1) = n for every integer n; Proposition 2 of no. 1 therefore shows that g is an absolute value on K.

For x ∈ Q and y ∈ K, g(xy) = |x|g(y) and hence g is a norm on K compatible with its Q-algebra structure (with the usual absolute value on Q). The completion K of K is therefore a normed algebra over Q = R (General Topology, Chapter IX, § 3, no. 7); let ĝ be the norm on K the continuous extension of g. As g is an absolute value on K, K is a field and ĝ an absolute value on K (General Topology, Chapter IX, § 3, no. 3, Proposition 6). By Theorem 1 there exists an R-algebra isomorphismf of K̂ onto one of the fields R, C or H and g'(x) = |j(x)| is therefore an absolute value on K̂; as K̂ is finite-dimensional over R and g' and ĝ coincide on the subfield R . 1 of K̂, g' = ĝ by the following lemma:

#### Lemma 2 {#ac-vi-s6-lem-2 .statement}

Let L be a (not necessarily commutative) field and K a subfield of L such that L is ajinite-dimensional left vector space over K. Let g be an absolute value on L andf its restriction to K. If K is complete and not discrete with respect to f, L is complete with respect to g; if further g' is another absolute value on L with the same restrictionf to K, then g' = g.

As the topology defined by g is Hausdorff and compatible with the left vector K-space structure on L, the first assertion follows from Topological Vector Spaces, Chapter I, § 2, no. 3, Theorem 2. Moreover the topologies on L defined by g and g' are identical (loc. cit.) ; there therefore exists a real number s > 0 such that g' = g^s (General Topology, Chapter IX, § 3, no. 2, Proposition 5). Let x be an element of K such that f(x) ≠ 1; the equation g'(x) = g(x) proves that s = 1.

Returning to the proof of Theorem 2, it is seen that, if j denotes the restriction of f to K, j is an isomorphism of K onto an everywhere dense subfield of R, C or H and g(x) = |j(x)| for x ∈ K, whence f(x) = |j(x)|^s.

Finally note that, iff is an absolute value on K, h is an absolute value on Q and s ≤ 1 by no. 3, Proposition 4; conversely, if s ≤ 1, f = g^s is an absolute value on K since g is (General Topology, Chapter IX, § 3, no. 2); this proves the last assertion of the statement.

Remarks

(2) If K is a field and a normed algebra over R, the norm is not necessarily an absolute value on K; for example, ξ + iη → |ξ| + |η| is a norm on C compatible with its R-algebra structure.

(3) For a proof of case (C) of Theorem 1 not using the general results of Algebra, Chapter VIII, see Exercise 2.

### Exercises {#ac-vi-s6-exercises}

See the [exercises for § 6](exercises/s6/).
