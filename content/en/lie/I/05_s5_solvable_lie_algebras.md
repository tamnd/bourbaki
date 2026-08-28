---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: I
chapter_title: Lie Algebras
section: 5
section_title: Solvable Lie algebras
lang: en
source: lie-i-iii
pdf_pages: 0061-0068, 0117-0119
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF SOLVABLE LIE ALGEBRAS
      page: 0
      pdf_page: 61
    - "no": 2
      title: RADICAL OF A LIE ALGEBRA
      page: 0
      pdf_page: 62
    - "no": 3
      title: NILPOTENT RADICAL OF A LIE ALGEBRA
      page: 0
      pdf_page: 62
    - "no": 4
      title: A CRITERION FOR SOLVABILITY
      page: 0
      pdf_page: 65
    - "no": 5
      title: FURTHER PROPERTIES OF THE RADICAL
      page: 0
      pdf_page: 66
    - "no": 6
      title: EXTENSION OF THE BASE FIELD
      page: 0
      pdf_page: 67
statements: 27
exercises: 17
content_sha256: bc96d56afc3255aae8af0a123337b972ece4e127279103def5f9db7ba948b944
---

## § 5. SOLVABLE LIE ALGEBRAS

Recall that $K$ henceforth denotes a field of characteristic 0 and that all Lie algebras are assumed to be finite-dimensional over $K$.†

### 1. DEFINITION OF SOLVABLE LIE ALGEBRAS

#### Definition 1 {#lie-i-s5-def-1 .statement}

*A Lie algebra $g$ is called solvable if its kth derived algebra $D^k g$ is zero for sufficiently large $k$.*

A nilpotent Lie algebra is solvable.

#### Proposition 1 {#lie-i-s5-prop-1 .statement}

*Subalgebras and quotient algebras of a solvable Lie algebra are solvable. Every extension of a solvable algebra by a solvable algebra is solvable. Every finite product of solvable algebras is solvable.*

Let $g$ be a Lie algebra, $g'$ a subalgebra, $h$ an ideal of $g$, $t = g/h$ and $\phi$ the canonical mapping of $g$ onto $t$. If $g$ is solvable then $D^k g = \{0\}$ for some integer $k$, hence $D^k g' \subset D^k g = \{0\}$, $D^k t = \phi(D^k g) = \{0\}$ and hence $g'$ and $t$ are solvable. If $h$ and $t$ are solvable there exist integers $s, t$ such that

$$
D^s h = D^t t = \{0\};
$$

then $D^t g \subset h$, hence $D^{s+t} g = D^s(D^t g) \subset D^s h = \{0\}$ and $g$ is solvable. The last assertion follows from the second by induction on the number of factors.

#### Proposition 2 {#lie-i-s5-prop-2 .statement}

*Let $g$ be a Lie algebra. The following conditions are equivalent:*

(a) $g$ is solvable;
(b) *there exists a decreasing sequence $g = g_0 \supset g_1 \supset \cdots \supset g_n = \{0\}$ of ideals of $g$ such that the algebras $g_i/g_{i+1}$ are commutative ($i = 0, 1, \ldots, n-1$);*
(c) *there exists a decreasing sequence $g = g'_0 \supset g'_1 \supset \cdots \supset g'_p = \{0\}$ of subalgebras of $g$ such that $g'_{i+1}$ is an ideal of $g'_i$ and $g'_i/g'_{i+1}$ is commutative ($i = 0, 1, \ldots, p-1$);*
(d) *there exists a decreasing sequence $g = g''_0 \supset g''_1 \supset \cdots \supset g''_q = \{0\}$ of subalgebras of $g$ such that $g''_{i+1}$ is an ideal of $g''_i$ of codimension 1 ($i = 0, 1, \ldots, q-1$).*

(a) $\Rightarrow$ (b): it suffices to consider the sequence of derived ideals of $g$.
(b) $\Rightarrow$ (c): this is obvious.
(c) $\Rightarrow$ (d): suppose that condition (c) holds; every vector subspace of $g'_i$ containing $g'_{i+1}$ is an ideal of $g'_i$, whence immediately (d).
(d) $\Rightarrow$ (a): this follows immediately from the fact that an extension of a solvable algebra by a solvable algebra is solvable.

† The reader will note that the hypothesis on the characteristic of $K$ is not used in nos. 1 and 2 of this paragraph.

Examples of solvable Lie algebras

I. Let $g$ be a 2-dimensional vector space over $K$ and $(e_1, e_2)$ a basis of $g$. There exists one and only one alternating bilinear multiplication $(x, y) \mapsto [x, y]$ on $g$ such that $[e_1, e_2] = e_2$. It is easily verified that $g$ is thus given a solvable Lie algebra structure. Now let $h$ be a non-commutative Lie algebra of dimension 2 over $K$. We show that $h$ is isomorphic to $g$. Let $(f_1, f_2)$ be a basis of $h$. The element $[f_1, f_2]$ is non-zero (otherwise $h$ would be commutative) and hence it generates a 1-dimensional subspace $t$ of $h$. Then $[h, h] = t$. Let $(e'_1, e'_2)$ be a basis of $h$ such that $e'_2 \in t$. Then $[e'_1, e'_2] = \lambda e'_2$ with $\lambda \neq 0$. Replacing $e'_1$ by $\lambda^{-1} e_1$, it can be assumed that $\lambda = 1$, whence our assertion.

II. Formulae (5) of § 1 prove that $\mathcal{D}t(n, K) = n(n, K)$. As $n(n, K)$ is nilpotent and hence solvable, $t(n, K)$ is solvable. Therefore $st(n, K)$ is solvable. In particular, $st(2, K)$ is isomorphic to the algebra of Example I.

### 2. RADICAL OF A LIE ALGEBRA

Let $a, b$ be two solvable ideals of a Lie algebra $g$. The algebra $(a + b)/b$ is isomorphic to $a/(a \cap b)$ and hence is solvable and $a + b$, which is an extension of $(a + b)/b$ by $b$, is also solvable (Proposition 1). It follows that a maximal solvable ideal of $g$ contains every solvable ideal of $g$ and hence $g$ has a largest solvable ideal. This enables us to make the following definition:

#### Definition 2 {#lie-i-s5-def-2 .statement}

*The radical of a Lie algebra is its largest solvable ideal.*

#### Proposition 3 {#lie-i-s5-prop-3 .statement}

*The radical $r$ of a Lie algebra $g$ is the smallest ideal of $g$ such that $g/r$ has radical $\{0\}$.*

Let $a$ be an ideal of $g$ and $\phi$ the canonical mapping of $g$ onto $g/a$. If the radical of $g/a$ is zero, then $\phi(r)$, which is a solvable ideal of $g/a$, is zero; hence $r \subset a$.

On the other hand, the inverse image $\phi^{-1}(r')$ of the radical $r'$ of $g/r$ is an ideal of $g$ which is solvable by Proposition 1 and hence is equal to $r$; therefore $r' = \{0\}$.

#### Proposition 4 {#lie-i-s5-prop-4 .statement}

*Let $g_1, \ldots, g_n$ be Lie algebras. The radical $r$ of the product of the $g_i$ is the product of the radicals $r_i$ of the $g_i$.*

The product $r'$ of the $r_i$ is a solvable ideal (Proposition 1) and hence $r' \subset r$. The canonical image of $r$ in $g_i$ is a solvable ideal of $g_i$ and hence is contained in $r_i$; hence $r \subset r'$.

### 3. NILPOTENT RADICAL OF A LIE ALGEBRA

#### Definition 3 {#lie-i-s5-def-3 .statement}

*Let $g$ be a Lie algebra. The nilpotent radical of $g$ is the intersection of the kernels of the finite-dimensional simple representations of $g$.*

#### Remark {#lie-i-s5-n3-rem-1 .statement}

(1) Let $s$ be the nilpotent radical of $g$. As every decreasing sequence of vector subspaces of $g$ is stationary, there exists a finite number of finite-dimensional simple representations of $g$ whose kernels have intersection $s$.

The direct sum of these representations is semi-simple and has kernel s. It follows that the set of kernels of finite-dimensional semi-simple representations of g has a least element, namely s.

(2) By Proposition 4 (c) of § 4, no. 3, s is also the intersection of the largest nilpotency ideals of the finite-dimensional representations of g. In particular, s is contained in the largest nilpotent ideal of g and is therefore a nilpotent ideal of g.

(3) Every linear form $\lambda$ on g which is zero on $\mathcal{D}g$ is a simple representation (with space K) of g, whence $\lambda(s) = \{0\}$. It follows that $s \subset \mathcal{D}g$. On the other hand, s is contained in the radical r of g by Remark 2. We shall prove that $s = r \cap \mathcal{D}g$.

#### Lemma 1 {#lie-i-s5-lem-1 .statement}

Let V be a finite-dimensional vector space over K, g a subalgebra of gl(V) such that V is a simple g-module and a a commutative ideal of g. Then $a \cap \mathcal{D}g = \{0\}$. Let S be the subalgebra of $\mathcal{L}(V)$ generated by 1 and a.

If b is an ideal of g contained in a such that $\operatorname{Tr} bs = 0$ for all $b \in b$ and all $s \in S$, then in particular, by definition of S, $\operatorname{Tr}(b^n) = 0$ for every integer $n > 0$ and hence b is nilpotent (Algebra, Chapter VII, § 5, no. 5, Corollary 4 to Proposition 13); as the elements of b are all nilpotent, $b = \{0\}$ (§ 4, no. 3, Lemma 2). We first apply this to the ideal $[g, a]$ of g. If $x \in g, a \in a, s \in S$, then $\operatorname{Tr}[x, a]s = \operatorname{Tr}(xas - axs) = \operatorname{Tr} x(as - sa) = 0$ since $as = sa$; hence $[g, a] = \{0\}$. Hence the elements of g commute with those of a and hence also with those of S. If $x, y$ belong to g and $s \in S$, then

$$
\operatorname{Tr}[x, y]s = \operatorname{Tr}(xys - yxs) = \operatorname{Tr} x(ys - sy) = 0
$$

since $ys = sy$; then taking b to be the ideal $\mathcal{D}g \cap a$, it follows that $\mathcal{D}g \cap a = \{0\}$.

#### Theorem 1 {#lie-i-s5-thm-1 .statement}

Let g be a Lie algebra, r its radical and s its nilpotent radical. Then $s = \mathcal{D}g \cap r$.

We already know that $s \subset \mathcal{D}g \cap r$. Hence it will suffice to show that if $\rho$ is a finite-dimensional simple representation of g then $\rho(\mathcal{D}g \cap r) = \{0\}$. Let k be the least integer $\geq 0$ such that $\rho(\mathcal{D}^{k+1}r) = \{0\}$; we write $g' = \rho(g)$, $a' = \rho(D^k r)$; as $\mathcal{D}^k r$ is an ideal of g, $a'$ is an ideal of $g'$; this ideal is commutative since $\rho(\mathcal{D}^{k+1}r) = \{0\}$. If V is the space of $\rho$, $g' \subset \operatorname{gl}(V)$ and V is a simple $g'$-module. Then $\rho(\mathcal{D}g \cap \mathcal{D}^k r) \subset \mathcal{D}g' \cap a' = \{0\}$. If $k > 0$, then $\mathcal{D}^k r \subset \mathcal{D}g$ and $\rho(\mathcal{D}^k r) = \{0\}$, contrary to the definition of k. Hence $k = 0$, that is

$$
\rho(\mathcal{D}g \cap r) = \{0\}.
$$

#### Corollary 1 {#lie-i-s5-thm-1-cor-1 .statement}

Let g be a solvable Lie algebra. The nilpotent radical of g is $\mathcal{D}g$. If $\rho$ is a finite-dimensional simple representation of g, $\rho(g)$ is commutative and the associative algebra L generated by 1 and $\rho(g)$ is a field of finite degree over K.

Here $r = g$, whence $s = \mathcal{D}g$. Hence $\varphi(\mathcal{D}g) = \{0\}$, which shows that $g' = \rho(g)$ is commutative. Every element $\neq 0$ of $L$ is invertible by Schur’s Lemma; hence $L$ is a field.

**Corollary 2 (Lie’s Theorem).** *Let $g$ be a solvable Lie algebra; suppose that $K$ is algebraically closed. Let $M$ be a $g$-module of finite dimension over $K$ and let $(M_i)_{0 \leq i \leq r}$ be a Jordan-Hölder series of $M$. Then $M_{i-1}/M_i$ is of dimension 1 over $K$ for $1 \leq i \leq r$ and, for all $x \in g$, $x_{M_{i-1}/M_i} = \lambda_i(x) \cdot 1$, where $\lambda_i$ is a linear form on $g$ which is zero on $\mathcal{D}g$. In particular, every simple $g$-module of finite dimension over $K$ is in fact of dimension 1.*

Let $\rho_i$ be the representation of $g$ on $M_{i-1}/M_i$. The associative algebra $L_i$ generated by 1 and $\rho_i(g)$ is a field, a finite extension of $K$ and therefore equal to $K$; and $M_{i-1}/M_i$ is a simple $L_i$-module, whence $\dim M_{i-1}/M_i = 1$. The rest of the corollary is obvious.

#### Remark {#lie-i-s5-n3-rem-2 .statement}

(1) If $(M_i)_{0 \leq i \leq r}$ is replaced by another Jordan-Hölder series of $M$, the sequence $(\lambda_1, \ldots, \lambda_r)$ is replaced by a sequence of the form $(\lambda_{\pi(1)}, \ldots, \lambda_{\pi(r)})$, where $\pi$ is a permutation of $\{1, \ldots, r\}$, as follows from the Jordan-Hölder Theorem.

(2) Let $(e_1, \ldots, e_r)$ be a basis of $M$ such that $e_i \in M_{i-1}, e_i \notin M_i$ ($1 \leq i \leq r$). If $x \in g$ the endomorphism of $M$ corresponding to $x$ is represented with respect to this basis by a triangular matrix whose diagonal coefficients are

$$
\lambda_1(x), \ldots, \lambda_r(x).
$$

#### Corollary 3 {#lie-i-s5-thm-1-cor-3 .statement}

*Suppose that $K$ is algebraically closed. If $g$ is an $r$-dimensional solvable Lie algebra, every ideal of $g$ is a term of a decreasing sequence of ideals of dimensions $r, r-1, \ldots, 0$.*

Every ideal is part of a Jordan-Hölder series of $g$, considered as the space of the adjoint representation (*Algebra*, Chapter I, § 6, no. 14, Corollary to Theorem 8); then it suffices to apply Corollary 2.

#### Corollary 4 {#lie-i-s5-thm-1-cor-4 .statement}

*Suppose that $K = \mathbf{R}$. Let $g$ be a solvable Lie algebra. Every simple representation of $g$ is of dimension $\leq 2$. Every ideal of $g$ is a term of a decreasing sequence $(g_i)_{0 \leq i \leq m}$ of ideals such that $g_0 = g, g_m = \{0\}, \dim g_{i-1}/g_i \leq 2$ ($1 \leq i \leq m$).

This is proved in a similar way to that for Corollaries 2 and 3, using the fact that every algebraic extension of $\mathbf{R}$ is of degree $\leq 2$.*

#### Corollary 5 {#lie-i-s5-thm-1-cor-5 .statement}

*For a Lie algebra $g$ to be solvable, it is necessary and sufficient that $\mathcal{D}g$ be nilpotent.*

The condition is necessary by Corollary 1. It is sufficient since $g/\mathcal{D}g$ is commutative.

#### Corollary 6 {#lie-i-s5-thm-1-cor-6 .statement}

*Let $\varphi$ be a finite-dimensional representation of a Lie algebra $g$. Let* r be the radical of g. Every element $x \in r$ such that $\rho(x)$ is nilpotent belongs to the largest nilpotency ideal $n$ of $\rho$.

Let V be the space of $\rho$; let $(V_i)_{0 \leq i \leq r}$ be a Jordan-Hölder series for the r-module structure on V and let $\rho_i$ be the representation of r with space $V_i / V_{i-1}$ ($1 \leq i \leq r$). If $\rho(x)$ is nilpotent, so is $\rho_i(x)$; as for all $i$ the algebra generated by $\rho_i(x)$ is a field, $\rho_i(x) = 0$. Conversely, if $\rho_i(x) = 0$ for all $i$, $\rho(x) = 0$. This shows that the set $a$ of $x \in r$ such that $\rho(x)$ is nilpotent is an ideal of r. On the other hand, $[g, a] \subset \mathcal{D}g \cap r \subset n \cap r \subset a$ and hence $a$ is an ideal of g. This proves that $a \subset n$.

#### Corollary 7 {#lie-i-s5-thm-1-cor-7 .statement}

Let g be a Lie algebra and r its radical. The following four sets are identical: (a) the largest nilpotent ideal of g; (b) the largest nilpotent ideal of r; (c) the set of $x \in r$ such that $\mathrm{ad}_g x$ is nilpotent; (d) the set of $x \in r$ such that $\mathrm{ad}_r x$ is nilpotent.

Let these sets be denoted by $a, b, c, d$. The inclusions $a \subset b \subset d \subset c$ are clear. $c \subset a$ by Corollary 6 applied to the adjoint representation of g.

### 4. A CRITERION FOR SOLVABILITY

#### Lemma 2 {#lie-i-s5-lem-2 .statement}

Let $x$ be an endomorphism of a finite-dimensional vector space V and s (resp. n) its semi-simple (resp. nilpotent) component (cf. Algebra, Chapter VIII, § 9, no. 4, Definition 4). Let $\mathrm{ad}\, x, \mathrm{ad}\, s, \mathrm{ad}\, n$ be the respective images of $x, s, n$ in the adjoint representation of $\mathfrak{gl}(V)$. Then $\mathrm{ad}\, s$ (resp. $\mathrm{ad}\, n$) is the semi-simple (resp. nilpotent) component of $\mathrm{ad}\, x$ and is equal to a polynomial in $\mathrm{ad}\, x$ with coefficients in K and no constant term.

We know that $\mathrm{ad}\, x = \mathrm{ad}\, s + \mathrm{ad}\, n, [\mathrm{ad}\, s, \mathrm{ad}\, n] = 0$ and $\mathrm{ad}\, n$ is nilpotent ($§ 4$, Lemma 1). We show that $\mathrm{ad}\, s$ is semi-simple. It suffices to do this when K is algebraically closed (cf. Algebra, Chapter VIII, § 9, no. 2, Proposition 3). Then let $(e_i)_{1 \leq i \leq n}$ be a basis of V such that $s(e_i) = \lambda_i e_i$ ($\lambda_i \in K$). Let $(E_{ij})$ be the canonical basis of $M_n(K) = \mathfrak{gl}(V)$. By formulae (5) of $§ 1$,

$$
(\mathrm{ad}\, s)\cdot E_{ij} = (\lambda_i - \lambda_j)E_{ij}
$$

and hence $\mathrm{ad}\, s$ is semi-simple. The last assertion of the lemma follows from Algebra, Chapter VIII, § 9, no. 4, Proposition 8.

#### Lemma 3 {#lie-i-s5-lem-3 .statement}

Let M be a finite-dimensional vector space, A and B two vector subspaces of $\mathfrak{gl}(M)$ such that $B \subset A$ and T the set of $t \in \mathfrak{gl}(M)$ such that $[t, A] \subset B$. If $z \in T$ is such that $\mathrm{Tr}(zu) = 0$ for all $u \in T$, then $z$ is nilpotent.

It suffices to prove this when K is algebraically closed, which we shall assume henceforth. Let s and n be the semi-simple and nilpotent components of z and let $(e_i)$ be a basis of M such that $s(e_i) = \lambda_i e_i$ ($\lambda_i \in K$). Let $V \subset K$ be the vector space over $\mathbf{Q}$ generated by the $\lambda_i$. We need to prove that $V = \{0\}$. Let f be a $\mathbf{Q}$-linear form on V and let t be the endomorphism of M such that

$te_i = f(\lambda_i)e_i$. If $(E_{ij})$ is the canonical basis of $\mathfrak{gl}(M)$ defined by $E_{ij}e_k = \delta_{jk}e_i$, then
$$
\begin{align*}
(\mathrm{ad}\ s)E_{ij} &= (\lambda_i - \lambda_j)E_{ij} \\
(\mathrm{ad}\ t)E_{ij} &= (f(\lambda_i) - f(\lambda_j))E_{ij}.
\end{align*}
$$

There exists a polynomial P with no constant term and with coefficients in K such that $P(\lambda_i - \lambda_j) = f(\lambda_i) - f(\lambda_j)$ for all i and j (for if $\lambda_i - \lambda_j = \lambda_h - \lambda_k$, then $f(\lambda_i) - f(\lambda_j) = f(\lambda_h) - f(\lambda_k)$ and, if $\lambda_i - \lambda_j = 0$, $f(\lambda_i) - f(\lambda_j) = 0$). Then $\mathrm{ad}\ t = P(\mathrm{ad}\ s)$. On the other hand, $\mathrm{ad}\ s$ is a polynomial with no constant term in $\mathrm{ad}\ z$. Now $(\mathrm{ad}\ z)(A) \subset B$, whence also $(\mathrm{ad}\ t)(A) \subset B$. By the hypothesis $0 = \mathrm{Tr}(zt) = \sum \lambda_i f(\lambda_i)$, whence $0 = f(\mathrm{Tr}(zt)) = \sum f(\lambda_i)^2$. Since the $f(\lambda_i)$ are rational numbers, $f = 0$, which completes the proof.

#### Theorem 2 (Cartan's criterion) {#lie-i-s5-thm-2 .statement}

*Let g be a Lie algebra, M a finite-dimensional vector space, ρ a representation of g on M and β the bilinear form on g associated with ρ. Then ρ(g) is solvable if and only if 𝒟g is orthogonal to g with respect to β.*

It can obviously be reduced to the case where g is a Lie subalgebra of $\mathfrak{gl}(M)$ and ρ is the identity mapping. If g is solvable, 𝒟g is contained in the largest nilpotency ideal of the identity representation of g (Theorem 1) and hence is orthogonal to g with respect to β (§ 4, Proposition 4 (d)). Suppose that 𝒟g is orthogonal to g with respect to β. We prove that g is solvable. Let T be the set of $t \in \mathfrak{gl}(M)$ such that $[t, g] \subset \mathscr{D}g$. If $t \in T$ and x, y belong to g, then $[t, x] \in \mathscr{D}g$ and hence
$$
\mathrm{Tr}(t[x, y]) = \beta([t, x], y) = 0
$$
whence by linearity $\mathrm{Tr}(tu) = 0$ for all $u \in \mathscr{D}g$. Also, clearly $\mathscr{D}g \subset T$. Hence (Lemma 3) every element of 𝒟g is nilpotent. It follows that 𝒟g is nilpotent (§ 4, Corollary 3 to Theorem 1) and hence that g is solvable (no. 3, Corollary 5 to Theorem 1).

### 5. FURTHER PROPERTIES OF THE RADICAL

#### Proposition 5 {#lie-i-s5-prop-5 .statement}

*Let g be a Lie algebra and r its radical.*
(a) *If ρ is a finite-dimensional representation of g and β is the associated bilinear form, r and 𝒟g are orthogonal with respect to β.*
(b) *r is the orthogonal of 𝒟g with respect to the Killing form.*
Let x, y be in g, $z \in r$. Then $[y, z] \in \mathscr{D}g \cap r$ and hence
$$
\beta([x, y], z) = \beta(x, [y, z]) = 0
$$
(Theorem 1). Hence (a).
Let r' be the orthogonal of 𝒟g with respect to the Killing form. It is an ideal of g (§ 3, no. 6, Proposition 7 (a)) which contains r by the above. On the other hand, the image s of r' under the adjoint representation of g is solvable (Theorem 2) and hence r' is solvable being a central extension of s. Hence r' ⊂ r.

#### Corollary 1 {#lie-i-s5-prop-5-cor-1 .statement}

Let g be a Lie algebra. Then g is solvable if and only if $\mathcal{D}g$ is orthogonal to g with respect to the Killing form.

This is an immediate consequence of Proposition 5 (b).

#### Corollary 2 {#lie-i-s5-prop-5-cor-2 .statement}

The radical r of a Lie algebra g is a characteristic ideal.

$\mathcal{D}g$ is a characteristic ideal and the Killing form is completely invariant (§ 3, no. 6, Proposition 10). Hence the orthogonal of $\mathcal{D}g$ with respect to the Killing form is a characteristic ideal (§ 3, no. 6, Proposition 7 (b)).

#### Corollary 3 {#lie-i-s5-prop-5-cor-3 .statement}

Let g be a Lie algebra, r its radical and a an ideal of g. Then the radical of a is equal to $r \cap a$.

r ∩ a is a solvable ideal of a and hence is contained in the radical r' of a. Conversely, r' is an ideal of g (Corollary 2 and § 1, no. 4, Proposition 2) and hence r' ⊂ r.

Corollary 2 can be made more precise as follows:

#### Proposition 6 {#lie-i-s5-prop-6 .statement}

Let g be a Lie algebra, r its radical and n its largest nilpotent ideal. Every derivation of g maps r into n.

Let D be a derivation of g. Let g' = g + Kx_0 be a Lie algebra in which g is an ideal of codimension 1 such that Dx = [x_0, x] for all x ∈ g (§ 1, no. 8, Example 1). By Corollary 3 to Proposition 5, r is contained in the radical r' of g'. Then D(r) = [x_0, r] ⊂ [g', g'] ∩ r' = s'. For all x ∈ s', ad_{g'} x is nilpotent (Theorem 1). Hence, for all x ∈ s' ∩ g, ad_g x is nilpotent. Hence D(r) is contained in the nilpotent ideal s' ∩ g of g.

#### Corollary {#lie-i-s5-n5-cor-1 .statement}

The largest nilpotent ideal of a Lie algebra is a characteristic ideal.

#### Remark {#lie-i-s5-n5-rem-1 .statement}

To summarize some of the above results, note that, if r, n, s, t denote respectively the radical of g, the largest nilpotent ideal of g, the nilpotent radical of g and the orthogonal of g with respect to the Killing form, then

$$
r \supset t \supset n \supset s.
$$

The inclusion r ⊃ t follows from Proposition 5 (b). The inclusion t ⊃ n follows from § 4, no. 4, Proposition 6 (b). The inclusion n ⊃ s has been pointed out in Remark 2 of no. 3.

### 6. EXTENSION OF THE BASE FIELD

Let g be a Lie K-algebra and K_1 an extension of K. Clearly g_{(K_1)} is solvable if and only if g is solvable, since $\mathcal{D}^n(g_{(K_1)}) = (\mathcal{D}^n g)_{(K_1)}$.

Let r be the radical of g. Then $r_{(K_1)}$ *is the radical of* $g_{(K_1)}$. For let $\beta$ be the Killing form of g. As r is the orthogonal of $\mathcal{D}g$ with respect to $\beta$ (Proposition 5 (b)), $r_{(K_1)}$ is the orthogonal of $(\mathcal{D}g)_{(K_1)} = \mathcal{D}(g_{(K_1)})$ with respect to the form derived from $\beta$ by extension from K to $K_1$, that is the Killing form of $g_{(K_1)}$ (§ 3, no. 8). Our assertion then follows from a further application of Proposition 5 (b).

### Exercises {#lie-i-s5-exercises}

The conventions of § 5 remain valid unless otherwise mentioned.

See the [exercises for § 5](exercises/s5/).
