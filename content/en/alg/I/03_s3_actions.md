---
book: alg
book_title: Algebra
chapter: I
chapter_title: ALGEBRAIC STRUCTURES
section: 3
section_title: Actions
lang: en
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 24-29, 129-132
pdf_pages: 0048-0053, 0153-0156
extraction: ocr
subsections:
    - "no": 1
      title: ACTIONS
      page: 24
      pdf_page: 48
    - "no": 2
      title: SUBSETS STABLE UNDER AN ACTION. INDUCED ACTION
      page: 26
      pdf_page: 50
    - "no": 3
      title: QUOTIENT ACTION
      page: 26
      pdf_page: 50
    - "no": 4
      title: DISTRIBUTIVITY
      page: 27
      pdf_page: 51
    - "no": 5
      title: DISTRIBUTIVITY OF ONE INTERNAL LAW WITH RESPECT TO ANOTHER
      page: 29
      pdf_page: 53
statements: 14
exercises: 10
content_sha256: ea8e120387da4eeeb5565a60d17f5eac8359a45e81eafde8841009256e414458
---

## § 3. ACTIONS

### 1. ACTIONS

#### Definition 1 {#alg-i-s3-def-1 .statement}

*Let $\Omega$ and E be two sets. A mapping of $\Omega$ into the set $E^E$ of mappings of E into itself is called an action of $\Omega$ on E.*

Let $\alpha \mapsto f_\alpha$ be an action of $\Omega$ on E. The mapping $(\alpha, x) \mapsto f_\alpha(x)$ (resp. $(x, \alpha) \mapsto f_\alpha(x)$) is called the *law of left* (resp. *right*) *action of $\Omega$ on E*† *associated with the given action of $\Omega$ on E*. Given a mapping $g$ of $\Omega \times E$ (resp. $E \times \Omega$) into E, there exists one and only one action $\alpha \mapsto f_\alpha$ of $\Omega$ on E such that the associated law of left (resp. right) action is $g$ (*Set Theory*, II, § 5, no. 2, Proposition 3).

In this chapter we shall say, for the sake of abbreviation, "law of action"

† Or sometimes the *external law of composition* on E with $\Omega$ as operating set.

instead of "law of left action". The element $f_\alpha(x)$ of E (for $\alpha \in \Omega$ and $x \in E$) is sometimes called the *transform* of $x$ under $\alpha$ or the *composition* of $\alpha$ and $x$. It is often denoted by left (resp. right) multiplicative notation $\alpha . x$ (resp. $x . \alpha$), the dot may be omitted; the composition of $\alpha$ and $x$ is then called the *product* of $\alpha$ and $x$ (resp. $x$ and $\alpha$). The exponential notation $x^\alpha$ is also used. In the arguments of the following paragraphs we shall generally use the notation $\alpha \perp x$. The elements of $\Omega$ are often called *operators*.

#### Example {#alg-i-s3-n1-exa-1 .statement}

(1) Let E be an associative magma written multiplicatively. The mapping which associates with a strictly positive integer $n$ the mapping $x \mapsto x^n$ of E into itself is an action of $\mathbf{N}^*$ on E. If E is a group, the mapping which associates with a rational integer $a$ the mapping $x \mapsto x^a$ of E into E is an action of $\mathbf{Z}$ on E.

(2) Let E be a magma with law denoted by $\top$. The mapping which associates with $x \in E$ the mapping $A \mapsto x \top A$ of the set of subsets of E into itself is an action of E on $\mathcal{P}(E)$.

(3) Let E be a set. The identity mapping of $E^E$ is an action of $E^E$ on E, called the *canonical action*. The corresponding law of action is the mapping $(f, x) \mapsto f(x)$ of $E^E \times E$ into E.

(4) Let $(\Omega_i)_{i \in I}$ be a family of sets. For all $i \in I$, let $f_i : \Omega_i \to E^E$ be an action of $\Omega_i$ on E. Let $\Omega$ be the sum of the $\Omega_i$ (*Set Theory*, II, § 4, no. 8). The mapping $f$ of $\Omega$ onto $E^E$, extending the $f_i$, is an action of $\Omega$ on E. This allows us to reduce the study of a family of actions to that of a single action.

(5) Given an action of $\Omega$ on E with law denoted by $\perp$, a subset $\Xi$ of $\Omega$ and a subset X of E, $\Xi \perp X$ denotes the set of $\alpha \perp x$ with $\alpha \in \Xi$ and $x \in X$; when $\Xi$ consists of a single element $\alpha$, we generally write $\alpha \perp X$ instead of $\{\alpha\} \perp X$. The mapping which associates with $\alpha \in \Omega$ the mapping $X \mapsto \alpha \perp X$ is an action of $\Omega$ on $\mathcal{P}(E)$, which is said to be *derived* from the given action by extension to the set of subsets.

(6) Let $\alpha \mapsto f_\alpha$ be an action of $\Omega$ on E. Let g be a mapping of $\Omega'$ into $\Omega$. Then the mapping $\beta \mapsto f_{g(\beta)}$ is an action of $\Omega'$ on E.

(7) Let $f : E \times E \to E$ be a law of composition on a set E. The mapping $\gamma : x \mapsto \gamma_x$ (resp. $\delta : x \mapsto \delta_x$) (§ 2, no. 2) which associates with the element $x \in E$ left (resp. right) translation by $x$ is an action of E on itself; it is called the *left* (resp. *right*) *action* of E on itself *derived* from the given law. When $f$ is commutative, these two actions coincide.

The law of left (resp. right) action associated with $\gamma$ is $f$ (resp. the opposite law to $f$). The law of right (resp. left) action associated with $\delta$ is $f$ (resp. the opposite law to $f$).

Let $\Omega, E, F$ be sets, $\alpha \mapsto f_\alpha$ an action of $\Omega$ on E and $\alpha \mapsto g_\alpha$ an action of $\Omega$ on F. An $\Omega$-*morphism of E into F*, or *mapping of E into F compatible with the action of $\Omega$*, is a mapping $h$ of E into F such that

$$
g_\alpha(h(x)) = h(f_\alpha(x))
$$

for all $\alpha \in \Omega$ and $x \in E$. The composition of two $\Omega$-morphisms is an $\Omega$-morphism.

Let $\Omega, \Xi, E, F$ be sets, $\alpha \mapsto f_\alpha$ an action of $\Omega$ on $E$, $\beta \mapsto g_\beta$ an action of $\Xi$ on $F$ and $\phi$ a mapping of $\Omega$ into $\Omega'$. A $\phi$-morphism of $E$ into $F$ is a mapping $h$ of $E$ into $F$ such that
$$
g_{\phi(\alpha)}(h(x)) = h(f_\alpha(x))
$$
for all $\alpha \in \Omega$ and $x \in E$.

### 2. SUBSETS STABLE UNDER AN ACTION. INDUCED ACTION

#### Definition 2 {#alg-i-s3-def-2 .statement}

*A subset $A$ of a set $E$ is called stable under an action $\alpha \mapsto f_\alpha$ of $\Omega$ on $E$ if $f_\alpha(A) \subset A$ for all $\alpha \in \Omega$. An element $x$ of $E$ is called invariant under an element $\alpha$ of $\Omega$ if $f_\alpha(x) = x$.*

The intersection of a family of stable subsets of $E$ under a given action is stable. There therefore exists a smallest stable subset of $E$ containing a given subset $X$ of $E$; it is said to be *generated* by $X$; it consists of the elements $(f_{\alpha_1} \circ f_{\alpha_2} \circ \cdots \circ f_{\alpha_n})(x)$, where $x \in X, n \geq 0, \alpha_i \in \Omega$ for all $i$.

#### Remark {#alg-i-s3-n2-rem-1 .statement}

Let $E$ be a magma with law denoted by $\tau$. It should be noted that a subset $A$ of $E$ which is stable under the left action on $E$ on itself is not necessarily stable under the right action of $E$ on itself; a subset $A$ of $E$ stable under the left (resp. right) action of $E$ on itself is stable under the law on $E$ but the converse is not in general true. More precisely, $A$ is stable under the law on $E$ if and only if $A \tau A \subset A$ whereas $A$ is stable under the left (resp. right) action on $E$ on itself if and only if $E \tau A \subset A$ (resp. $A \tau E \subset A$).

#### Example {#alg-i-s3-n2-exa-1 .statement}

Take the magma $E$ to be the set $\mathbf{N}$ with multiplication. The set $\{1\}$ is stable under the internal law of $\mathbf{N}$, but the stable subset under the action of $\mathbf{N}$ on itself generated by $\{1\}$ is the whole of $\mathbf{N}$.

#### Definition 3 {#alg-i-s3-def-3 .statement}

*Let $\alpha \mapsto f_\alpha$ be an action of $\Omega$ on $E$ and $A$ a stable subset of $E$. The mapping which associates with an element $\alpha \in \Omega$ the restriction of $f_\alpha$ to $A$ (considered as a mapping of $A$ into itself) is an action of $\Omega$ on $A$ said to be induced by the given action.*

### 3. QUOTIENT ACTION

#### Definition 4 {#alg-i-s3-def-4 .statement}

*Let $\alpha \mapsto f_\alpha$ be an action of a set $\Omega$ on a set $E$. An equivalence relation $R$ on $E$ is said to be compatible with the given action if, for all elements $x$ and $y$ of $E$ such that $x \equiv y \pmod{R}$ and all $\alpha \in \Omega, f_\alpha(x) \equiv f_\alpha(y) \pmod{R}$. The mapping which associates with an element $\alpha \in \Omega$ the mapping of $E/R$ into itself derived from $f_\alpha$ by passing to the quotients is an action of $\Omega$ on $E/R$ called the quotient of the action of $\Omega$ on $E$.*

Let $E$ be a magma and $R$ an equivalence relation on $E$. $R$ is said to be *left* (resp. *right*) *compatible* with the law on $E$ if it is compatible with the left (resp.

right) action of E on itself derived from the law on E. For R to be compatible with the law on E it is necessary and sufficient that it be left and right compatible with the law on E.

We leave to the reader the statement and proof of the analogues of Propositions 6, 7 and 8 of § 1, no. 6.

### 4. DISTRIBUTIVITY

#### Definition 5 {#alg-i-s3-def-5 .statement}

Let $E_1, \ldots, E_n$ and F be sets and u a mapping of $E_1 \times \cdots \times E_n$ into F. Let $i \in \{1, n\}$. Suppose $E_i$ and F are given the structures of magmas. u is said to be distributive relative to the index variable i if the partial mapping

$$
x_i \mapsto u(a_1, \ldots, a_{i-1}, x_i, a_{i+1}, \ldots, a_n)
$$

is a homomorphism of $E_i$ into F for all fixed $a_j$ in $E_j$ and $j \neq i$.

If $\top$ denotes the internal laws on $E_i$ and F, the distributivity of u is given by the equations

(1) $$
u(a_1, \ldots, a_{i-1}, x_i \top x'_i, a_{i+1}, a_n) \\
= u(a_1, \ldots, a_{i-1}, x_i, a_{i+1}, \ldots, a_n) \top u(a_1, \ldots, a_{i-1}, x'_i, a_{i+1}, \ldots, a_n)
$$

for $i = 1, 2, \ldots, n, a_1 \in E_1, \ldots, a_{i-1} \in E_{i-1}, x_i \in E_i, x'_i \in E_i, a_{i+1} \in E_{i+1}, \ldots, a_n \in E_n$.

#### Example {#alg-i-s3-n4-exa-1 .statement}

Let E be a monoid (resp. group) written multiplicatively. The mapping $(n, x) \mapsto x^n$ of $\mathbf{N} \times E$ (resp. $\mathbf{Z} \times E$) into E is distributive with respect to the first variable by the equation $x^{m+n} = x^m x^n$ (with addition as law on $\mathbf{N}$). If E is commutative, this mapping is distributive with respect to the second variable by the equation $(xy)^n = x^n y^n$.

#### Proposition 1 {#alg-i-s3-prop-1 .statement}

Let $E_1, E_2, \ldots, E_n$ and F be commutative monoids written additively and let u be a mapping of $E_1 \times \cdots \times E_n$ into F, which is distributive with respect to all the variables. For $i = 1, 2, \ldots, n$, let $L_i$ be a non-empty finite set and $(x_{i,\lambda})_{\lambda \in L_i}$ a family of elements of $E_i$. Let $y_i = \sum_{\lambda \in L_i} x_{i,\lambda}$ for $i = 1, 2, \ldots, n$. Then

(2) $$
u(y_1, \ldots, y_n) = \sum_\alpha u(x_1, \alpha_1, \ldots, x_n, \alpha_n)
$$

the sum being taken over all sequences $\alpha = (\alpha_1, \ldots, \alpha_n)$ belonging to $L_1 \times \cdots \times L_n$.

We argue by induction on n, the case $n = 1$ following from formula (2) of § 1, no. 2. From the same reference

(3) $$
u(y_1, \ldots, y_{n-1}, y_n) = \sum_{\alpha_n \in L_n} u(y_1, \ldots, y_{n-1}, x_n, \alpha_n)
$$

for $y_n = \sum_{\alpha_n \in L_n} x_{n,\alpha_n}$ and the mapping $z \mapsto u(y_1, \ldots, y_{n-1}, z)$ of $E_n$ into $F$ is a magma homomorphism. By the induction hypothesis applied to the distributive mappings $(z_1, \ldots, z_{n-1}) \mapsto u(z_1, \ldots, z_{n-1}, x_n, \alpha_n)$ from $E_1 \times \cdots \times E_{n-1}$ to $F$,

(4)
$$
u(y_1, \ldots, y_{n-1}, x_n, \alpha_n) = \sum_{\alpha_1, \ldots, \alpha_{n-1}} u(x_1, \alpha_1, \ldots, x_{n-1}, \alpha_{n-1}, x_n, \alpha_n),
$$
the sum being taken over the sequences $(\alpha_1, \ldots, \alpha_{n-1})$ belonging to $M = L_1 \times \cdots \times L_{n-1}$. Now $L_1 \times \cdots \times L_n = M \times L_n$; writing
$$
t_{\alpha_1, \ldots, \alpha_n} = u(x_1, \alpha_1, \ldots, x_n, \alpha_n),
$$
we have
(5)
$$
\sum_{\alpha_1, \ldots, \alpha_n} t_{\alpha_1, \ldots, \alpha_n} = \sum_{\alpha_n} \left( \sum_{\alpha_1, \ldots, \alpha_{n-1}} t_{\alpha_1, \ldots, \alpha_{n-1}, \alpha_n} \right)
$$
by formula (7) of § 1, no. 5. (2) follows immediately from (3), (4) and (5).

#### Remark {#alg-i-s3-n4-rem-1 .statement}

If $u(a_1, \ldots, a_{i-1}, 0, a_{i+1}, \ldots, a_n) = 0$ for $i = 1, 2, \ldots, n$ and $a_j \in E_j$ ($j \neq i$), then formula (2) remains true for families $(x_i, \lambda)_{\lambda \in L_i}$ of finite support.

A special case of Definition 5 is that where $u$ is the law of action associated with the action of a set $\Omega$ on a magma $E$. If $u$ is distributive with respect to the second variable, it is also said that the action of $\Omega$ on the magma $E$ is distributive. In other words:

#### Definition 6 {#alg-i-s3-def-6 .statement}

*An action* $\alpha \mapsto f_\alpha$ *of a set* $\Omega$ *on a magma* $E$ *is said to be distributive if, for all* $\alpha \in \Omega$, *the mapping* $f_\alpha$ *is an endomorphism of the magma* $E$.

If $\top$ denotes the law of the magma $E$ and $\perp$ the law of action associated with the action of $\Omega$ on $E$, the distributivity of the latter is then expressed by the formula
(6)
$$
\alpha \perp (x \top y) = (\alpha \perp x) \top (\alpha \perp y) \quad \text{(for } \alpha \in \Omega \text{ and } x, y \in E\text{)}.
$$

By an abuse of language, it is also said that the law $\perp$ is distributive (or right distributive) with respect to the law $\top$.

Formula (2) of § 1, no. 2 shows that then, for every ordered sequence $(x_\lambda)_{\lambda \in L}$ of elements of $E$ and every $\alpha \in \Omega$,
(7)
$$
\alpha \perp \left( \bigwedge_{\lambda \in L} x_\lambda \right) = \bigwedge_{\lambda \in L} (\alpha \perp x_\lambda).
$$

If an action $\alpha \mapsto f_\alpha$ is distributive and an equivalence relation $R$ on $E$ is compatible with the law of composition of $E$ and the action $\alpha \mapsto f_\alpha$, the quotient action on $E/R$ is distributive.

When the law on $E$ is written multiplicatively, we often use the exponential notation $x^\alpha$ for a law of action which is distributive with respect to this multiplication, so that distributivity is expressed by the identity $(xy)^\alpha = x^\alpha y^\alpha$. If the law on E is written additively, we often use left (resp. right) multiplicative notation $\alpha . x$ (resp. $x . \alpha$) for a law of action which is distributive with respect to this addition, the distributivity being expressed by the identity

$$
\alpha(x + y) = \alpha x + \alpha y \quad (\text{resp. } (x + y)\alpha = x\alpha + y\alpha).
$$

We may also consider the case where $\Omega$ has an internal law, denoted by $\overline{T}$, and the law of action is distributive with respect to the first variable, which means that

(8)
$$
(\alpha \overline{T} \beta) \perp x = (\alpha \perp x) T (\beta \perp x)
$$
for all $\alpha, \beta \in \Omega$ and $x \in E$. Then, by formula (2) of § 1, no. 2

(9)
$$
\left( \overline{T}_{\lambda \in L} \alpha_{\lambda} \right) \perp x = \overline{T}_{\lambda \in L} (\alpha_{\lambda} \perp x)
$$
for every ordered sequence $(\alpha_{\lambda})_{\lambda \in L}$ of elements of $\Omega$ and all $x \in E$.

### 5. DISTRIBUTIVITY OF ONE INTERNAL LAW WITH RESPECT TO ANOTHER

#### Definition 7 {#alg-i-s3-def-7 .statement}

Let $T$ and $\perp$ be two internal laws on a set E. The law $\perp$ is said to be distributive with respect to the law $T$ if

(10)
$$
x \perp (y T z) = (x \perp y) T (x \perp z)
$$
(11)
$$
(x T y) \perp z = (x \perp z) T (y \perp z)
$$
for all $x, y, z$ in E.

Note that (10) and (11) are equivalent if the law $\perp$ is commutative. In general, one of the laws is written additively and the other multiplicatively; if multiplication is distributive with respect to addition, then:

(12)
$$
x . (y + z) = x . y + x . z
$$
(13)
$$
(x + y) . z = x . z + y . z
$$

#### Example {#alg-i-s3-n5-exa-1 .statement}

(1) In the set $\mathcal{P}(E)$ of subsets of a set E, each of the internal laws $\cap$ and $\cup$ is distributive with respect to itself and the other. This follows from formulae of the form

$$
A \cap (B \cup C) = (A \cap B) \cup (A \cap C)
$$
$$
A \cup (B \cap C) = (A \cup B) \cap (A \cup C).
$$

(2) In $\mathbf{Z}$ (and more generally, in any totally ordered set) each of laws sup and inf is distributive with respect to the other and with respect to itself.

(3) In $\mathbf{Z}$(*and more generally in any ring*) multiplication is distributive with respect to addition.

(4) In $\mathbf{N}$ addition and multiplication are distributive with respect to the laws sup and inf.

### Exercises {#alg-i-s3-exercises}

See the [exercises for § 3](exercises/s3/).
