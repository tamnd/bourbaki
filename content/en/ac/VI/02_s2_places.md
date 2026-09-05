---
book: ac
book_title: Commutative Algebra
chapter: VI
chapter_title: VALUATIONS
section: 2
section_title: Places
lang: en
source: ac-i-vii
book_pages: 381-385, 444-446
pdf_pages: 0399-0403, 0462-0464
extraction: ocr
subsections:
    - "no": 1
      title: THE NOTION OF MORPHISM FOR LAWS OF COMPOSITION NOT EVERYWHERE DEFINED
      page: 381
      pdf_page: 399
    - "no": 2
      title: PLACES
      page: 381
      pdf_page: 399
    - "no": 3
      title: PLACES AND VALUATION RINGS
      page: 383
      pdf_page: 401
    - "no": 4
      title: EXTENSION OF PLACES
      page: 384
      pdf_page: 402
    - "no": 5
      title: CHARACTERIZATION OF INTEGRAL ELEMENTS BY MEANS OF PLACES
      page: 385
      pdf_page: 403
statements: 9
exercises: 6
content_sha256: b544413d10331937b891740ab23ca115c16171f1f2b46cac7186286bd8362f62
---

## 2. PLACES

### 1. THE NOTION OF MORPHISM FOR LAWS OF COMPOSITION NOT EVERYWHERE DEFINED

#### Definition 1 {#ac-vi-s2-def-1 .statement}

*Let E and E' be two sets each with an internal law of composition denoted by $(x, y) \mapsto x * y$, not necessarily everywhere defined. A mapping $f : E \to E'$ is a morphism if, for all $x, y$ in E such that $f(x) * f(y)$ is defined, the composition $x * y$ is also defined and:*

(1)
$$
f(x * y) = f(x) * f(y).
$$
More briefly, we may say that formula (1) must hold every time the right hand side has a meaning.

The notion of morphism is distinct from that of representation (*Algebra*, Chapter I, § 1, no. 1), where it is demanded that equation (1) hold whenever the left hand side has a meaning. Of course, the two notions coincide for laws of composition everywhere defined.

#### Definition 2 {#ac-vi-s2-def-2 .statement}

*Let E and E' be two sets each with a family of internal laws of composition $(x, y) \mapsto x *_{\alpha} y, \alpha \in I$. A mapping $f : E \to E'$ is a morphism if it is a morphism for each of the laws of composition $(x, y) \mapsto x *_{\alpha} y$.*

Just as representations, so morphisms satisfy axioms (MO_I), (MO_{II}), (MO_{III}) of *Set Theory*, Chapter IV, § 2. Iff: $E \to E'$ is a morphism, $f(E)$ is a stable subset of $\mathbf{R}'$.

### 2. PLACES

If K is a field, recall that $\mathbf{K}$ denotes the set the sum of K and an element denoted by $\infty$ (*Algebra*, Chapter 11, § 9, no. 9); the laws of composition of K extend to $\mathbf{K}$ by setting (*loc. cit.*)

(2)
$$
a + \infty = \infty \quad \text{for } a \in \mathbf{K}, \quad a \neq \infty,
$$
(3)
$$
\infty . a = a . \infty = \infty \quad \text{for } a \in \tilde{\mathbf{K}}, \quad a \neq 0.
$$

The only compositions not defined are therefore the compositions to $+ \infty$, $\infty . 0$ and $0 . \infty$. On the other hand, the mappings $x \mapsto -x$ and $x \mapsto x^{-1}$ extend similarly to $\tilde{K}$ by setting $-\infty = \infty, 0^{-1} = \infty, \infty^{-1} = 0$. We shall also write $x + (-y) = x - y$.

The set $\tilde{K}$, called the *projective field* associated with $K$, can be identified with the *projective line* $P_1(K)$ (*loc. cit.*).

#### Definition 3 {#ac-vi-s2-def-3 .statement}

*Let $K$ and $L$ be two fields. Every morphism* $f$ *of* $K$ *to* $\tilde{L}$ *(for addition and multiplication)* *such that* $f(1) = 1$ *is called a place of* $K$ *with values in* $L$.

In other words, if $x$ and $y$ are elements of $K$ and $f(x) + f(y)$ (resp. $f(x)f(y)$) is defined, then $x + y$ (resp. $xy$) is defined and

$$
f(x + y) = f(x) + f(y)
$$
$$
f(xy) = f(x)f(y).
$$

As $\infty + \infty$ is not defined, neither is $f(\infty) + f(\infty)$, which shows that
$$
f(\infty) = \infty.
$$

Similarly, since $0 \cdot \infty$ is not defined, neither is $f(0)f(\infty)$, which, by virtue of (6), implies
$$
f(0) = 0.
$$

On the other hand
$$
f(a^{-1}) = f(a)^{-1} \quad \text{for all } a \in \tilde{K}.
$$

If $f(a)f(a^{-1})$ is defined, $aa^{-1}$ is defined and hence is equal to 1; then $f(a)f(a^{-1}) = f(1) = 1$, which proves (8) in this case. If $f(a)f(a)^{-1}$ is not defined, then, either $f(a) = 0$ and $f(a^{-1}) = \infty$ or $f(a) = \infty$ and $f(a^{-1}) = 0$ and (8) still holds.

Similarly it can be shown that
$$
f(-a) = -f(a) \quad \text{for all } a \in K.
$$

From formulae (8) and (9) it follows that $f$ is also a morphism for the laws of composition $(x, y) \mapsto x - y$ and $(x, y) \mapsto xy^{-1}$.

For $x \in \tilde{K}$, $f$ is called finite at $x$ if $f(x) \neq \infty$; this implies $x \in K$ by (6).

If $f : K \to \tilde{L}$ is a place, $f(K)$ is a subset of $\tilde{L}$ which is stable for the laws of composition $(x, y) \mapsto x + y, (x, y) \mapsto x - y, (x, y) \mapsto xy$ and $(x, y) \mapsto xy^{-1}$ and which contains 1. If E is the set of finite elements of $f(\tilde{K})$, E is a subfield of L and $f(\tilde{K}) = \tilde{E}$. By an abuse of language E is called the *valuefield* off.

The *composite* mapping of two places is a place.

Let F be an isomorphism of a field K onto a subfield of a field L; let us extend $f$ to $K$ by setting $f(\infty) = \infty$. Thus we obtain a place of K with values in L which is called *trivial* and which is often identified with the isomorphism $f$.

### 3. PLACES AND VALUATION RINGS

#### Proposition 1 {#ac-vi-s2-prop-1 .statement}

Let K be a field, $\mathbf{A}$ a valuation ring of K and $\kappa(\mathbf{A})$ the residue field of $\mathbf{A}$. We extend the canonical mapping of $\mathbf{A}$ onto $\kappa(\mathbf{A})$ to a mapping $h_{\mathbf{A}} : \tilde{K} \to (\kappa(\mathbf{A}))$ by the equation $h_{\mathbf{A}}(x) = \infty$ if $x \notin \mathbf{A}$. The mapping $h_{\mathbf{A}}$ thus defined is a place of K whose valuefield is $\kappa(\mathbf{A})$.

Clearly $h_{\mathbf{A}}(1) = 1$.

We show that $h_{\mathbf{A}}$ is a morphism for addition. Let $x, y$ be two elements of $\tilde{K}$ such that $h_{\mathbf{A}}(x) + h_{\mathbf{A}}(y)$ is defined. One of the two elements $x, y$ belongs then to $\mathbf{A}$ and hence $x + y$ is defined. If $x \in \mathbf{A}$ and $y \in \mathbf{A}$, clearly

$$
h_{\mathbf{A}}(x) + h_{\mathbf{A}}(y) = h_{\mathbf{A}}(x + y)
$$

holds. If $x \in \mathbf{A}$ and $y \notin \mathbf{A}$, then $x + y \notin \mathbf{A}$ and the two sides of the above formula equal $\infty$.

We show finally that $h_{\mathbf{A}}$ is a morphism for multiplication. Let $x \in K, y \in K$ be such that $h_{\mathbf{A}}(x)h_{\mathbf{A}}(y)$ is defined. If $x \in \mathbf{A}$ and $y \in \mathbf{A}$, clearly $xy$ is defined and $h_{\mathbf{A}}(x)h_{\mathbf{A}}(y) = h_{\mathbf{A}}(xy)$. Suppose now that one of the elements $x, y$, for example $y$, does not belong to $\mathbf{A}$; as $h_{\mathbf{A}}(y) = \infty$, $h_{\mathbf{A}}(x) \neq 0$, that is $x \notin m(\mathbf{A})$, whence $x^{-1} \in \mathbf{A}$; it follows that $xy$ is defined and that $xy \notin \mathbf{A}$, whence

$$
h_{\mathbf{A}}(xy) = \infty = h_{\mathbf{A}}(x)h_{\mathbf{A}}(y).
$$

This proves Proposition 1.

If $j$ is an isomorphism of $\kappa(\mathbf{A})$ onto a subfield of a field L, $j \circ h_{\mathbf{A}} : \tilde{K} \to \tilde{L}$ is a place of K with values in L. The above process in fact provides all the places on K. To be precise:

#### Proposition 2 {#ac-vi-s2-prop-2 .statement}

Let K and L be two fields and f a place of K with values in L. Then there exists a valuation ring $\mathbf{A}$ of K and an isomorphism $j$ of $\kappa(\mathbf{A})$ onto a subfield of L such that $f = j \circ h_{\mathbf{A}}$; these conditions determine $\mathbf{A}$ and $j$ uniquely. The ring $\mathbf{A}$ is the set of $x \in K$ such that $f(x) \neq \infty$ and $m(\mathbf{A})$ is the set of $x \in K$ such that $f(x) = 0$.

If $f = j \circ h_{\mathbf{A}}$, the condition $f(x) \neq \infty$ (resp. $f(x) = 0$) is equivalent to the condition $h_{\mathbf{A}}(x) \neq \infty$ (resp. $h_{\mathbf{A}}(x) = 0$) and hence to the condition $x \in \mathbf{A}$ (resp. $x \in m(\mathbf{A})$). Hence $\mathbf{A}$ is determined uniquely and, as $h_{\mathbf{A}}$ is surjective, $j$ is also unique.

Now let $f$ be any place of K with values in L; let $\mathbf{A}$ denote the set of $x \in K$ such that $f(x) \neq \infty$. If $x \in \mathbf{A}$ and $y \in \mathbf{A}$, the compositions $f(x) - f(y)$ and $f(x)f(y)$ are defined and $\neq \infty$, which shows that $x - y \in \mathbf{A}$ and $xy \in \mathbf{A}$; hence $\mathbf{A}$ is a subring of K. If $x \notin \mathbf{A}$, then $f(x) = \infty$, hence $f(x^{-1}) = 0$ and $x^{-1}$ belongs to the kernel $m$ of the homomorphism $f'$ obtained by restricting $f$ to $\mathbf{A}$. Conversely if $y \in m$, then $y^{-1} \notin \mathbf{A}$. This shows that $\mathbf{A}$ is a valuation ring of K and that $m$ is its maximal ideal. Let $j$ be the injective homomorphism from $\kappa(\mathbf{A})$ to L derived from f' by passing to the quotient. Then $f(x) = j(h_A(x))$ for all $x \in A$ and this equation remains true for $x \notin A$, the two sides being then equal to $\infty$.

The decomposition $f = j \circ h_A$ is called the canonical decomposition of the placef. $A$ is called the ring off, $m(A)$ the ideal of $f$ and $\kappa(A)$ the residue field off. For two places $f : \mathbf{K} \to \mathbf{L}$ and $f' : \mathbf{K} \to \mathbf{L}'$ to have the same ring, it is necessary and sufficient that there exist an isomorphisms of the value field off onto that off such that $f' = s \circ f$; then $f$ and $f'$ are called equivalent. It is seen that every result on valuation rings can be translated into a result on places and conversely; this is what we shall do in the following nos.

Examples Of places
(1) Let $K$ be a field. The identity mapping on $K$ is a trivial place with ring $K$ and ideal $(0)$.
(2) Let $k$ be a field. For all $u \in k((T))^\sim$, let us write $f(u) = \infty$ if $u \notin k[[T]]$ and define $f(u)$ to be the constant term of $u$ if $u \in k[[T]]$. Then $f$ is a place of $k((T))$, with residue field $k$ and ring $k[[T]]$. For $k[[T]]$ is a valuation ring of $k((T))$ (§ 1, no. 4, Example 3 ) and the restriction of $f$ to $k[[T]]$ is identified with the canonical homomorphism of $k[[T]]$ onto its residue field.
(3) Let $k$ be a field, $a$ an element of $k$ and $A$ the set of $u \in k(X)$ such that $a$ is substitutable in $u$ (Algebra, Chapter IV, § 3, no. 2). If $p$ denotes the prime ideal $(X - a)$ of $k[X]$, then $A = k[X]_p$, so that $A$ is a valuation ring of $k(X)$ (§ 1, no. 4, Proposition 2). For all $u \in k(X)^\sim$, let us write $f(u) = \infty$ if $u \notin A$ and $f(u) = u(a)$ if $u \in A$. Then $f$ is a place of $k(X)$ with residue field $k$ and ring $A$; for the restriction off to $A$ is a homomorphism of $A$ onto $k$ (Algebra, Chapter IV, § 3, Proposition 2) of kernel $pA = m(A)$. The element $f(u) \in k$ is said to be obtained by putting $X = a$ in $u$.
\* (4) Let $S$ be a connected complex analytic variety of dimension 1 and $K$ the field of meromorphic functions on $S$. For all $z_0 \in S$, the mapping $f \mapsto f(z_0)$ from $K$ to $\mathbf{C}$ is a place of $K$ whose ring is the set off $\in K$ which are holomorphic at $z_0$ and whose ideal is the set off $\in K$ which are zero at $z_0$. It is this example and other analogues which are the origin of the term "place".*

### 4. EXTENSION OF PLACES

#### Proposition 3 {#ac-vi-s2-prop-3 .statement}

Let $K$ be a field, $S$ a subring of $K$ and $f$ a homomorphism from $S$ to an algebraically closed field $L$. Then there exists a place of $K$ with values in $L$ which extends $f$.

Taking account of Proposition 1, this is a translation of Theorem 2 of § 1, no. 2.

#### Proposition 4 {#ac-vi-s2-prop-4 .statement}

Let $K$ be a field, $f$ a place of $K$ with values in a field $L$ and $K'$ an extension of $K$. Then there exists an extension $L'$ of $L$ and a place $f'$ of $K'$ with values in $L'$ which extends $f$. If $x_1, \ldots, x_n$ are elements of $K$ which are algebraically independent over $K$ and $a,, \ldots, a,,$ any elements $\in L, f'$ may be chosen such that $f(x_i) = a,$ for $1 \leq i \leq n.$

Let $V$ be the ring off, $g$ the restriction off to $V$ and $g'$ the extension of $g$ to $V[x_1, \ldots, x_n]$ such that $g'(x_i) = a,$ for $1 \leq i \leq n.$ It is sufficient to take $L'$ to be an algebraic closure of $L$ and apply Proposition 3 to $g'$ and $L'$: we obtain a placef': $K' \to \tilde{L}'$ which extends $g'$; if $x \in K - V,$ then $x^{-1} \in m(V),$ whence $f(x^{-1}) = g(x^{-1}) = 0$ and $f'(x) = \infty = f(x);$ hencef' extendsf.

### 5. CHARACTERIZATION OF INTEGRAL ELEMENTS BY MEANS OF PLACES

#### Proposition 5 {#ac-vi-s2-prop-5 .statement}

Let $K$ be a field, $S$ a subring of $K, h$ a homomorphism from $S$ to a field and $p$ the kernel of $h.$ For an element $x$ of $K$ to be integral over the local ring $S,$ it is necessary and sufficient that every place of $K$ extending $h$ be finite at $x.$

If $f$ is a place of $K$ extending $h, f$ is finite on $S_p$ and zero on $pS_p$ and hence the ring of the place $f$ dominates $S_p.$ Conversely, if $V$ is a valuation ring of $K$ which dominates $S_p,$ $V$ is the ring of a placef whose restriction to $S$ is a homomorphism with the same kernel as $h;$ replacing $f$ by an equivalent place, it is seen that $V$ is the ring of a place of $K$ which extends $h.$ To say that every place of $K$ extending $h$ is finite at $x$ is equivalent to saying that $x$ belongs to all the valuation rings of $K$ which dominate $S_p.$ The proposition then follows from Theorem 3 of § 1, no. 3.

#### Proposition 6 {#ac-vi-s2-prop-6 .statement}

Let $K$ be a field and $S$ a subring of $K.$ For an element $x \in K$ to be integral over $S,$ it is necessary and sufficient that every place of $K$ which is finite on $S$ be finite at $x.$

This is also a consequence of Theorem 3 of § 1, no. 3.

### Exercises {#ac-vi-s2-exercises}

See the [exercises for § 2](exercises/s2/).
