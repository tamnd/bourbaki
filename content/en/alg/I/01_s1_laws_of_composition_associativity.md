---
book: alg
book_title: Algebra
chapter: I
chapter_title: ALGEBRAIC STRUCTURES
section: 1
section_title: Laws of composition; associativity; commutativity
lang: en
source: alg-i-iii
source_edition: 1998, Springer
pdf_pages: 0025-0036, 0148-0150
extraction: ocr
subsections:
    - "no": 1
      title: LAWS OF COMPOSITION
      page: 0
      pdf_page: 25
    - "no": 2
      title: COMPOSITION OF AN ORDERED SEQUENCE OF ELEMENTS
      page: 0
      pdf_page: 27
    - "no": 3
      title: ASSOCIATIVE LAWS
      page: 0
      pdf_page: 28
    - "no": 4
      title: STABLE SUBSETS. INDUCED LAWS
      page: 0
      pdf_page: 30
    - "no": 5
      title: PERMUTABLE ELEMENTS. COMMUTATIVE LAWS
      page: 0
      pdf_page: 31
    - "no": 6
      title: QUOTIENT LAWS
      page: 0
      pdf_page: 35
statements: 31
exercises: 16
content_sha256: ee4e463c2bea3d268def69cc870b68653ee33956e50d1763ff66c0f237db3f9e
---

## § 1. LAWS OF COMPOSITION; ASSOCIATIVITY; COMMUTATIVITY

### 1. LAWS OF COMPOSITION

#### Definition 1 {#alg-i-s1-def-1 .statement}

Let E be a set. A mapping f of E × E into E is called a law of composition on E. The value f(x, y) of f for an ordered pair (x, y) ∈ E × E is called the composition of x and y under this law. A set with a law of composition is called a magma.

The composition of x and y is usually denoted by writing x and y in a definite order and separating them by a characteristic symbol of the law in question (a symbol which it may be agreed to omit). Among the symbols most often used are + and ., the usual convection being to omit the latter if desired; with these symbols the composition of x and y is written respectively as x + y and x.y or xy. A law denoted by the symbol + is usually called addition (the composition x + y being called the sum of x and y) and we say that it is written additively; a law denoted by the symbol . is usually called multiplication (the composition x.y = xy being called the product of x and y) and we say that it is written multiplicatively. In the general arguments of paragraphs 1 to 3 of this chapter we shall generally use the symbols ⊔ and ⊓ to denote arbitrary laws of composition.

By an abuse of language, a mapping of a subset of E × E into E is sometimes called a law of composition not everywhere defined on E.

#### Example {#alg-i-s1-n1-exa-1 .statement}

(1) The mappings (X, Y) ↦ X ∪ Y and (X, Y) ↦ X ∩ Y are laws of composition on the set of subsets of a set E.

(2) On the set N of natural numbers, addition, multiplication and exponentiation are laws of composition (the compositions of x ∈ N and y ∈ N under these laws being denoted respectively by x + y, xy or x.y and x^y) (Set Theory, III, § 3, no. 4).

(3) Let E be a set; the mapping (X, Y) ↦ X ⋅ Y is a law of composition on the set of subsets of E × E (Set Theory, II, § 3, no. 3, Definition 6); the mapping (f, g) ↦ f ⋅ g is a law of composition on the set of mappings of E into E (Set Theory, II, § 5, no. 2).

(4) Let E be a lattice (Set Theory, III, § 1, no. 11); if sup(x, y) denotes the least upper bound of the set {x, y}, the mapping (x, y) ↦ sup(x, y) is a law of composition on E. Similarly for the greatest lower bound inf(x, y). Example 1 above is a particular case of this with $\mathfrak{P}(E)$ ordered by inclusion.

(5) Let $(E_t)_{t \in I}$ be a family of magmas. Let $\tau_t$ denote the law of composition on $E_t$. The mapping
$$
((x_i), (y_i)) \mapsto ((x_i \tau_t y_i))
$$
is a law of composition on the product $E = \prod_{t \in I} E_t$, called the *product* of the laws $\tau_t$. The set E with this law is called the *product magma* of the magmas $E_t$. In particular, if all the magmas $E_t$ are equal to the same magma M, we obtain the *magma of mappings of I from M*.

Let $(x, y) \mapsto x \tau y$ be a law of composition on a set E. Given any two subsets X, Y of E, $X \tau Y$ (provided this notation does not lead to confusion†) will denote the set of elements $x \tau y$ in E, where $x \in X, y \in Y$ (in other words, the image of $X \times Y$ under the mapping $(x, y) \mapsto x \tau y$).

If $a \in E$ we usually write $a \tau Y$ instead of $\{a\} \tau Y$ and $X \tau a$ instead of $X \tau \{a\}$. The mapping $(X, Y) \mapsto X \tau Y$ is a law of composition on the set of subsets of E.

#### Definition 2 {#alg-i-s1-def-2 .statement}

*Let E be a magma and $\tau$ denote its law of composition. The law of composition $(x, y) \mapsto y \tau x$ on E is called the opposite of the above. The set E with this law is called the opposite magma of E.*

Let E and E' be two magmas; we shall denote their laws by the same symbol $\tau$. Conforming with the general definitions (*Set Theory*, IV, § 1, no. 5), a bijective mapping f of E onto E' such that
$$
f(x \tau y) = f(x) \tau f(y)
$$
for every ordered pair $(x, y) \in E \times E$ is called an *isomorphism of E onto E'*. E and E' are said to be *isomorphic* if there exists an isomorphism of E onto E'.

More generally:

#### Definition 3 {#alg-i-s1-def-3 .statement}

*A mapping f of E into E' such that relation (1) holds for every ordered pair $(x, y) \in E \times E$ is called a homomorphism, or morphism, of E into E'; if $E = E'$, f is called an endomorphism of E.*

The identity mapping of a magma E is a homomorphism, the composition of two homomorphism is a homomorphism.

† The following is an example where this principle would lead to confusion and should therefore not be used. Suppose that the law of composition in question is the law $(A, B) \mapsto A \cup B$ between subsets of a set E; a law of composition
$$
(\mathcal{A}, \mathcal{B}) \mapsto F(\mathcal{A}, \mathcal{B})
$$
is derived between subsets of $\mathfrak{P}(E)$, $F(\mathcal{A}, \mathcal{B})$ being the set of $A \cup B$ with $A \in \mathcal{A}, B \in \mathcal{B}$; but $F(\mathcal{A}, \mathcal{B})$ should not be denoted by $\mathcal{A} \cup \mathcal{B}$, as this notation already has a different meaning (the union of $\mathcal{A}$ and $\mathcal{B}$ considered as subsets of $\mathfrak{P}(E)$).

For a mapping $f$ of E into E' to be an isomorphism, it is necessary and sufficient that it be a bijective homomorphism and $f^{-1}$ is then an isomorphism of E' onto E.

### 2. COMPOSITION OF AN ORDERED SEQUENCE OF ELEMENTS

Recall that a family of elements of a set E is a mapping $i \mapsto x_i$ of a set I (called an indexing set) into E; a family $(x_i)_{i \in I}$ is called finite if the indexing set is finite.

A finite family $(x_i)_{i \in I}$ of elements of E whose indexing set I is totally ordered is called an ordered sequence of elements of E.

In particular, every finite sequence $(x_i)_{i \in H}$, where H is a finite subset of the set $\mathbf{N}$ of natural numbers, can be considered as an ordered sequence if H is given the order relation induced by the relation $m \leq n$ between natural numbers.

Two ordered sequences $(x_i)_{i \in I}$ and $(y_k)_{k \in K}$ are called similar if there exists an ordered set isomorphism $\phi$ of I onto K such that $y_{\phi(i)} = x_i$ for all $i \in I$.

Every ordered sequence $(x_\alpha)_{\alpha \in A}$ is similar to a suitable finite sequence. For there exists an increasing bijection of A onto an interval $[0, n]$ of $\mathbf{N}$.

#### Definition 4 {#alg-i-s1-def-4 .statement}

*Let* $(x_\alpha)_{\alpha \in A}$ *be an ordered sequence of elements in a magma E whose indexing set A is non-empty. The composition (under the law T) of the ordered sequence* $(x_\alpha)_{\alpha \in A}$, *denoted by* $\prod_{\alpha \in A} x_\alpha$, *is the element of E defined by induction on the number of elements in A as follows:*

(1) *if* $A = \{\beta\}$ *then* $\prod_{\alpha \in A} x_\alpha = x_\beta$;

(2) *if* A *has* $p > 1$ *elements, $\beta$ is the least element of* A *and* $A' = A - \{\beta\}$, *then* $\prod_{\alpha \in A} x_\alpha = x_\beta \ T \left( \prod_{\alpha \in A'} x_\alpha \right)$.

It follows immediately (by induction on the number of elements in the indexing sets) that the compositions of two similar ordered sequences are equal; in particular, the composition of any ordered sequence is equal to the composition of a finite sequence. If $A = \{\lambda, \mu, \nu\}$ has three elements ($\lambda < \mu < \nu$) the composition $\prod_{\alpha \in A} x_\alpha$ is $x_\lambda \ T \ (x_\mu \ T \ x_\nu)$.

#### Remark {#alg-i-s1-n2-rem-1 .statement}

Note that there is a certain arbitrariness about the definition of the composition of an ordered sequence; the induction we introduced proceeds "from right to left". If we proceeded "from left to right", the composition of the above ordered sequence $(x_\lambda, x_\mu, x_\nu)$ would be $(x_\lambda \ T \ x_\mu) \ T \ x_\nu$.

As a matter of notation, the composition of an ordered sequence $(x_\alpha)_{\alpha \in A}$ is written $\prod_{\alpha \in A}$ for a law denoted by $\perp$; for a law written additively it is usually denoted by $\sum_{\alpha \in A} x_\alpha$ and called the sum of the ordered sequence $(x_\alpha)_{\alpha \in A}$ (the $x_\alpha$ being called the terms of the sum); for a law written multiplicatively it is usually denoted by $\prod_{\alpha \in A} x_\alpha$ and called the *product* of the ordered sequence $(x_\alpha)$ (the $x_\alpha$ being called the *factors* of the product).†

When there is no possible confusion over the indexing set (nor over its ordering) it is often dispensed with in the notation for the composition of an ordered sequence and we then write, for example for a law written additively,
$\sum_\alpha x_\alpha$ instead of $\sum_{\alpha \in A} x_\alpha$; similarly for the other notations.

For a law denoted by $\top$ the composition of a *sequence* $(x_i)$ with indexing set a non-empty interval $[p, q]$ of $\mathbf{N}$ is denoted by $\prod_{p \leq i \leq q} x_i$ or $\prod_{i=p}^q x_i$; similarly for laws denoted by other symbols.

Let E and F be two magmas whose laws of composition are denoted by $\top$ and $f$ a homomorphism of E into F. For every ordered sequence $(x_\alpha)_{\alpha \in A}$ of elements of E
$$
f\left( \prod_{\alpha \in A} \right) = \prod_{\alpha \in A} f(x_\alpha).
$$

### 3. ASSOCIATIVE LAWS

#### Definition 5 {#alg-i-s1-def-5 .statement}

*A law of composition* $(x, y) \mapsto x \top y$ *on a set* E *is called associative if, for all elements* $x, y, z$ *in* E,
$$
(x \top y) \top z = x \top (y \top z).
$$
*A magma whose law is associative is called an associative magma*.

The opposite law of an associative law is associative.

#### Example {#alg-i-s1-n3-exa-1 .statement}

(1) Addition and multiplication of natural numbers are associative laws of composition on $\mathbf{N}$ (*Set Theory*, III, § 3, no. 3, Corollary to Proposition 5)
(2) The laws cited in Examples (1), (3) and (4) of no. 1 are associative.

#### Theorem 1 (Associativity theorem) {#alg-i-s1-thm-1 .statement}

*Let* E *be an associative magma whose law is denoted by* $\top$. *Let* A *be a totally ordered non-empty finite set, which is the union of an ordered sequence of non-empty subsets* $(B_i)_{i \in I}$ *such that the relations* $\alpha \in B_i, \beta \in B_j, i < j$ *imply* $\alpha < \beta$; *let* $(x_\alpha)_{\alpha \in A}$ *be an ordered sequence of elements in* E *with* A *as indexing set*. *Then*
$$
\prod_{\alpha \in A} x_\alpha = \prod_{i \in I} \left( \prod_{\alpha \in B_i} x_\alpha \right)
$$

† The use of this terminology and the notation $\prod_{\alpha \in A} x_\alpha$ must be avoided if there is any risk of confusion with the product of the sets $x_\alpha$ defined in the theory of sets (*Set Theory*, II, § 5, no. 3). However, if the $x_\alpha$ are cardinals and addition (resp. multiplication) is the cardinal sum (resp. the cardinal product), the cardinal denoted by $\sum_{\alpha \in A} x_\alpha$ (resp. $\prod_{\alpha \in A} x_\alpha$) in the above notation is the cardinal sum (resp. cardinal product) of the family $(x_\alpha)_{\alpha \in A}$ (*Set Theory*, III, § 3, no. 3).

§ 1.3

We prove the theorem by induction on the cardinal $n$ of $A$. Let $p$ be the cardinal of $I$ and $h$ its least element; let $J = I - \{h\}$. If $n = 1$, as the $B_i$ are non-empty, of necessity $p = 1$ and the theorem is obvious. Otherwise, assuming the theorem holds for an indexing set with at most $n - 1$ elements, we distinguish two cases:

(a) $B_h$ has a single element $\beta$. Let $C = \bigcup_{i \in J} B_i$. The left-hand side of (3) is equal, by definition, to $x_\beta \top \left( \prod_{\alpha \in C} x_\alpha \right)$; the right-hand side is equal, by definition, to
$$
x_\beta \top \left( \prod_{i \in J} \left( \prod_{\alpha \in B_i} x_\alpha \right) \right);
$$
the result follows from the fact that the theorem is assumed true for $C$ and $(B_i)_{i \in J}$.

(b) Otherwise, let $\beta$ be the least element of $A$ (and hence of $B_h$); let $A' = A - \{\beta\}$ and let $B'_i = A' \cap B_i$ for $i \in I$; then $B'_i = B_i$ for $i \in J$. The set $A'$ has $n - 1$ elements and the conditions of the theorem hold for $A'$ and its subsets $B'_i$; hence by hypothesis:
$$
\prod_{\alpha \in A'} x_\alpha = \left( \prod_{\alpha \in B'_h} x_\alpha \right) \top \left( \prod_{i \in J} \left( \prod_{\alpha \in B_i} x_\alpha \right) \right).
$$
Forming the composition of $x_\beta$ with each side, we have on the left-hand side side, by definition, $\prod_{\alpha \in A} x_\alpha$ and on the right-hand side, using the associativity,
$$
\left( x_\beta \top \left( \prod_{\alpha \in B'_h} x_\alpha \right) \right) \top \left( \prod_{i \in J} \left( \prod_{\alpha \in B_i} x_\alpha \right) \right)
$$
which is equal, by Definition 3, to the right-hand side of formula (3).

For an associative law denoted by $\top$ the composition $\prod_{p \leq i \leq q} x_i$ of a sequence $(x_i)_{i \in [p, q]}$ is also denoted (since no confusion can arise) by
$$
x_p \top \cdots \top x_q.
$$
A particular case of Theorem 1 is the formula
$$
x_0 \top x_1 \top \cdots \top x_n = (x_0 \top x_1 \top \cdots \top x_{n-1}) \top x_n.
$$
Consider an ordered sequence of $n$ terms all of whose terms are equal to the same element $x \in E$. The composition of this sequence is denoted by $\prod^n x$ for a law denoted by $\top$, $\prod^n x$ for a law denoted by $\perp$. For a law written multiplicatively the composition is denoted by $x^n$ and called the $n$-th *power* of $x$. For a law written additively the composition is usually denoted by $nx$. The associativity theorem applied to an ordered sequence all of whose terms are equal gives the equation

$$
\frac{n_1 + n_2 + \cdots + n_p}{T} x = \left( \frac{n_1}{T} x \right) T \left( \frac{n_2}{T} x \right) T \cdots T \left( \frac{n_p}{T} x \right).
$$

In particular, if $p = 2$,

$$
\frac{m+n}{T} x = \left( \frac{m}{T} x \right) T \left( \frac{n}{T} x \right)
$$
and if $n_1 = n_2 = \cdots = n_p = m$,
$$
\frac{pm}{T} x = \frac{p}{T} \left( \frac{m}{T} x \right).
$$

If $X$ is a subset of $E$, we sometimes denote, in conformity with the above notation, by $\frac{p}{T} X$ the set $X_1 T X_2 T \cdots T X_p$, where
$$
X_1 = X_2 = \cdots = X_p = X;
$$
it is thus the set of all compositions $x_1 T x_2 T \cdots T x_p$ with $x_1 \in X, x_2 \in X, \ldots, x_p \in X$.

It is important not to confuse this set with the set of $\frac{p}{T} x$, where $x$ runs through $X$.

### 4. STABLE SUBSETS. INDUCED LAWS

#### Definition 6 {#alg-i-s1-def-6 .statement}

*A subset $A$ of a set $E$ is called stable under the law of composition $T$ on $E$ if the composition of two elements of $A$ belongs to $A$. The mapping $(x, y) \mapsto x T y$ of $A \times A$ into $A$ is then called the law induced on $A$ by the law $T$. The set $A$ with the law induced by $T$ is called a submagma of $E$.*

In other words, for $A$ to be stable under a law $T$ it is necessary and sufficient that $A T A \subset A$. A stable subset of $E$ and the corresponding submagma are often identified.

The intersection of a family of stable subsets of $E$ is stable; in particular there exists a smallest stable subset $A$ of $E$ containing a given subset $X$; it is said to be *generated* by $X$ and $X$ is called a *generating system* of $A$ or a *generating set* of $A$. The corresponding submagma is also said to be *generated* by $X$.

#### Proposition 1 {#alg-i-s1-prop-1 .statement}

*Let $E$ and $F$ be two magmas and $f$ a homomorphism of $E$ into $F$.
(i) The image under $f$ of a stable subset of $E$ is a stable subset of $F$.
(ii) The inverse image under $f$ of a stable subset $F$ is a stable subset of $E$.
(iii) Let $X$ be a subset of $E$. The image under $f$ of the stable subset of $E$ generated by $X$ is the stable subset of $F$ generated by $f(X)$.
(iv) If $g$ is a second homomorphism of $E$ from $F$ the set of elements $x$ of $E$ such that $f(x) = g(x)$ is a stable subset of $E$.*

Assertions (i), (ii) and (iv) are obvious; we prove (iii). Let $\overline{X}$ be the stable subset of E generated by X and $\overline{f(X)}$ the stable subset of F generated by $f(X)$. By (i) $\overline{f(X)} \subset f(\overline{X})$ and by (ii) $\overline{X} \subset f^{-1}(\overline{f(X)})$, whence $f(\overline{X}) \subset \overline{f(X)}$.

#### Proposition 2 {#alg-i-s1-prop-2 .statement}

*Let E be an associative magma and X a subset of E. Let X' be the set of $x_1 \top x_2 \top \cdots \top x_n$, where $n \geq 1$ and where $x_i \in X$ for $1 \leq i \leq n$. The stable subset generated by X is equal to X'._

It follows immediately by induction on n that the composition of an ordered sequence of n terms belonging to X belongs to the stable subset generated by X; it is therefore sufficient to verify that X' is stable. Now if u and v are elements of X' they are of the form $u = x_0 \top x_1 \top \cdots \top x_{n-1}$, $v = x_n \top x_{n+1} \top \cdots \top x_{n+p}$ with $x_i \in X$ for $0 \leq i \leq n + p$; then (Theorem 1) $u \top v = x_0 \top x_1 \top \cdots \top x_{n+p}$ belongs to X'.

#### Example {#alg-i-s1-n4-exa-1 .statement}

(1) In the set $\mathbf{N}$ of natural numbers the stable subset under addition generated by {1} is the set of integers $\geq 1$; under multiplication the set {1} is stable.

(2) Given a law $\top$ on a set E, for a subset {h} consisting of a single element to be stable under the law $\top$ it is necessary and sufficient that $h \top h = h$; h is then said to be *idempotent*. For example, every element of a lattice is idempotent for each of the laws sup and inf.

(3) For an associative law $\top$ on a set E the stable subset generated by a set {a} consisting of a single element is the set of elements $\overline{\top}^n a$, where n runs through the set of integers $> 0$.

### 5. PERMUTABLE ELEMENTS. COMMUTATIVE LAWS

#### Definition 7 {#alg-i-s1-def-7 .statement}

*Let E be a magma whose law is denoted by $\top$. Two elements x and y of E are said to commute (or to be permutable) if $y \top x = x \top y$.*

#### Definition 8 {#alg-i-s1-def-8 .statement}

*A law of composition on a set E is called commutative if any two elements of E commute under this law. A magma whose law of composition is commutative is called a commutative magma.*

A commutative law is equal to its opposite.

#### Example {#alg-i-s1-n5-exa-1 .statement}

(1) Addition and multiplication of natural numbers are commutative laws on $\mathbf{N}$ (*Set Theory*, III, § 3, no. 3, Corollary to Proposition 5).

(2) On a lattice the laws sup and inf are commutative; so, in particular, are the laws $\cup$ and $\cap$ between subsets of a set E.

(3) Let E be a set of cardinal $> 1$. The law $(f, g) \mapsto f \circ g$ between mappings of E into E is not commutative as is seen by taking f and g to be distinct constant mappings, but the identity mapping is permutable with every mapping.

(4) Let $(x, y) \mapsto x \top y$ be a commutative law on $E$; the law
$$
(X, Y) \mapsto X \top Y
$$
between subsets of $E$ is commutative.

#### Definition 9 {#alg-i-s1-def-9 .statement}

*Let $E$ be a magma and $X$ a subset of $E$. The set of elements of $E$ which commute with each of the elements of $X$ is called the centralizer of $X$.*

Let $X$ and $Y$ be two subsets of $E$ and $X'$ and $Y'$ their respective centralizers. If $X \subset Y$, then $Y' \subset X'$.

Let $(X_i)_{i \in I}$ be a family of subsets of $E$ and for all $i \in I$ let $X'_i$ be the centralizer of $X_i$. The centralizer of $\bigcup_{i \in I} X_i$ is $\bigcap_{i \in I} X'_i$.

Let $X$ be a subset of $E$ and $X'$ the centralizer of $X$. The centralizer $X''$ of $X'$ is called the *bicentralizer* of $X$. Then $X \subset X''$. The centralizer $X'''$ of $X''$ is equal to $X'$. For $X'$ is contained in its bicentralizer $X'''$ and the relation $X \subset X''$ implies $X'''' \subset X'$.

#### Proposition 3 {#alg-i-s1-prop-3 .statement}

*Let $E$ be an associative magma whose law is denoted by $\top$. If an element $x$ of $E$ commutes with each of the elements $y$ and $z$ of $E$, it commutes with $y \top z$.*

For
$$
x \top (y \top z) = (x \top y) \top z = (y \top x) \top z \\
= y \top (x \top z) = y \top (z \top x) = (y \top z) \top x.
$$

#### Corollary {#alg-i-s1-n5-cor-1 .statement}

*Let $E$ be an associative magma. The centralizer of any subset of $E$ is a stable subset of $E$.*

#### Definition 10 {#alg-i-s1-def-10 .statement}

*The centralizer of a magma $E$ is called the centre of $E$. An element of the centre of $E$ is called a central element of $E$.*

If $E$ is an associative magma its centre is a stable subset by the Corollary to Proposition 3 and the law induced on its centre is commutative.

#### Proposition 4 {#alg-i-s1-prop-4 .statement}

*Let $E$ be an associative magma, $X$ and $Y$ two subsets of $E$. If every element of $X$ commutes with every element of $Y$ every element of the stable subset generated by $X$ commutes with every element of the stable subset generated by $Y$.*

Let $X'$ and $X''$ be the centralizer and bicentralizer of $X$. They are stable subsets of $E$. Now $X \subset X''$ and $Y \subset X'$ and hence $X''$ (resp. $X'$) contains the stable subset of $E$ generated by $X$ (resp. $Y$). As every element of $X''$ commutes with every element of $X'$, the proposition follows.

#### Corollary 1 {#alg-i-s1-prop-4-cor-1 .statement}

*If $x$ and $y$ are permutable under the associative law $\top$ so are $\top^m x$ and $\top^n y$ for all integers $m > 0$ and $n > 0$; in particular $\top^m x$ and $\top^n x$ are permutable for all $x$ and all integers $m > 0$ and $n > 0$.*

#### Corollary 2 {#alg-i-s1-prop-4-cor-2 .statement}

*If all pairs of elements of a subset X are permutable under an associative law T, the law induced by T on the stable subset generated by X is associative and commutative.*

#### Theorem 2 (Commutativity theorem) {#alg-i-s1-thm-2 .statement}

*Let T be an associative law of composition on E; let $(x_\alpha)_{\alpha \in A}$ be a non-empty finite family of elements of E which are pairwise permutable; let B and C be two totally ordered sets with A as underlying set. Then*
$$
\prod_{\alpha \in B} x_\alpha = \prod_{\alpha \in C} x_\alpha.
$$

Since the theorem is true if A has a single element, we argue by induction on the number $p$ of elements in A. Let $p$ be an integer > 1 and suppose the theorem is true when Card A < $p$. We prove it for Card A = $p$. It may be assumed that A is the interval $[0, p - 1]$ in $\mathbf{N}$; the composition of the ordered sequence $(x_\alpha)_{\alpha \in A}$ defined by the natural order relation on A is $\prod_{i=0}^{p-1} x_i$.

Let A be given another total ordering and let h be the least element of A under this ordering and A' the set of other elements of A (totally ordered by the induced ordering). Suppose first $0 < h < p - 1$ and let P = $\{0, 1, \ldots, h - 1\}$ and Q = $\{h + 1, \ldots, p - 1\}$; the theorem being assumed true for A', applying the associativity theorem, we obtain (since $A' = P \cup Q$)

$$
\prod_{\alpha \in A'} x_\alpha = \left( \prod_{i=0}^{h-1} x_i \right) \circ \left( \prod_{i=h+1}^{p-1} x_i \right)
$$

whence, composing $x_h$ with both sides and repeatedly applying the commutativity and associativity of T:

$$
\begin{align*}
\prod_{\alpha \in A} x_\alpha &= x_h \circ \left( \prod_{\alpha \in A'} x_\alpha \right) = x_h \circ \left( \prod_{i=0}^{h-1} x_i \right) \circ \left( \prod_{i=h+1}^{p-1} x_i \right) \\
&= \left( \prod_{i=0}^{h-1} x_i \right) \circ x_h \circ \left( \prod_{i=h+1}^{p-1} x_i \right) = \prod_{i=0}^{p-1} x_i,
\end{align*}
$$

which proves the theorem for this case. If $h = 0$ or $h = p - 1$, the same result follows, but more simply, the terms arising from P or the terms arising from Q not appearing in the formulae.

Under a commutative associative law on a set E the *composition* of a *finite family* $(x_\alpha)_{\alpha \in A}$ of elements of E is by definition the common value of the composition of all the *ordered sequences* obtained by totally ordering A in all possible ways. This composition will still be denoted by $\prod_{\alpha \in A} x_\alpha$ under a law denoted by T; similarly for other notations.

#### Theorem 3 {#alg-i-s1-thm-3 .statement}

*Let T be an associative law on E and $(x_\alpha)_{\alpha \in A}$ a non-empty finite family of elements of E which are pairwise permutable. If A is a union of non-empty subsets $(B_i)_{i \in I}$ which are pairwise disjoint, then*

$$
\prod_{\alpha \in A} x_\alpha = \prod_{i \in I} \left( \prod_{\alpha \in B_i} x_\alpha \right).
$$

This follows from Theorem 2 if $A$ and $I$ are totally ordered so that the $B_i$ satisfy the conditions of Theorem 1.

We single out two important special cases of this theorem:

1. If $(x_{\alpha \beta})_{(\alpha, \beta) \in A \times B}$ is a finite family of permutable elements of an associative magma whose indexing set is the product of two non-empty finite sets $A, B$ (a "double family"), then

$$
\prod_{(\alpha, \beta) \in A \times B} x_{\alpha \beta} = \prod_{\alpha \in A} \left( \prod_{\beta \in B} x_{\alpha \beta} \right) = \prod_{\beta \in B} \left( \prod_{\alpha \in A} x_{\alpha \beta} \right)
$$

as follows from Theorem 3 by considering $A \times B$ as the union of the sets $\{\alpha\} \times B$ on the one hand and of the sets $A \times \{\beta\}$ on the other.

For example, if $B$ has $n$ elements and for each $\alpha \in A$ all the $x_{\alpha \beta}$ have the same value $x_\alpha$, then

$$
\prod_{\alpha \in A} \left( \prod^n_{\beta=1} x_\alpha \right) = \prod^n_{\alpha=1} \left( \prod_{\alpha \in A} x_\alpha \right).
$$

If $B$ has two elements, we obtain the following results: let $(x_\alpha)_{\alpha \in A}, (y_\alpha)_{\alpha \in A}$ be two non-empty families of elements of $E$. If the $x_\alpha$ and the $y_\beta$ are pairwise permutable, then

$$
\prod_{\alpha \in A} x_\alpha \prod_{\alpha \in A} y_\alpha = \left( \prod_{\alpha \in A} x_\alpha \right) \prod_{\alpha \in A} y_\alpha.
$$

Because of formula (7) the composition of a double sequence $(x_{ij})$ whose indexing set is the product of two intervals $\{p, q\}$ and $\{r, s\}$ in $\mathbf{N}$ is often denoted for a commutative associative law written additively by

$$
\sum_{i=p}^q \sum_{j=r}^s x_{ij} \quad \text{or} \quad \sum_{j=r}^s \sum_{i=p}^q x_{ij}
$$

and similarly for laws denoted by other symbols.

2. Let $n$ be an integer $> 0$ and let $A$ be the set of ordered pairs of integers $(i, j)$ such that $0 \leq i \leq n, 0 \leq j \leq n$ and $i < j$; the composition of a family $(x_{ij})_{(i, j) \in A}$ (under a commutative associative law) is also denoted by $\prod_{0 \leq i < j \leq n} x_{ij}$ (or simply $\prod_{i < j} x_{ij}$, if no confusion arises); Theorem 3 here gives the formulae

$$
\prod_{0 \leq i < j \leq n} x_{ij} = \prod_{i=0}^{n-1} \left( \prod_{j=i+1}^n x_{ij} \right) = \prod_{j=1}^n \left( \prod_{i=0}^{j-1} x_{ij} \right).
$$

There are analogous formulae to (7) for a family whose indexing set is the product of more than two sets and analogous formulae to (10) for a family whose indexing set is the set $S_p$ of *strictly increasing sequences* $(i_k)_{1 \leq k \leq p}$ of $p$ integers such that $0 \leq i_k \leq n$ ($p \leq n + 1$): in the latter case the composition of the family $(x_{i_1 i_2 \ldots i_p})_{(i_1, \ldots, i_p) \in S_p}$ is denoted by

$$
\prod_{0 \leq i_1 < i_2 < \cdots < i_p < n} x_{i_1 i_2 \ldots i_p} \quad \text{or simply} \quad \prod_{i_1 < i_2 < \cdots < i_p} x_{i_1 i_2 \ldots i_p}.
$$

#### Proposition 5 {#alg-i-s1-prop-5 .statement}

Let E and F be magmas whose laws are denoted by T and let f and g be homomorphisms of E into F. Let f T g be the mapping x ↦ f(x) T g(x) of E into F. If F is associative and commutative, f T g is a homomorphism.

For all elements x and y of E:

$$(f T g)(x T y) = f(x T y) T g(x T y) = f(x) T f(y) T g(x) T g(y)$$
$$= f(x) T g(x) T f(y) T g(y) = ((f T g)(x)) T ((f T g)(y)).$$

### 6. QUOTIENT LAWS

#### Definition 11 {#alg-i-s1-def-11 .statement}

Let E be a set. A law of composition T and an equivalence relation R on E are said to be compatible if the relations x ≡ x' (mod R) and y ≡ y' (mod R) (for x, x', y, y' ∈ E) imply x T y ≡ x' T y' (mod R); the law of composition on the quotient set E/R which maps the equivalence classes of x and y to the equivalence class of x T y is called the quotient law of the law T with respect to R. The set E/R with the quotient law is called the quotient magma of E with respect to R.

To say that an equivalence relation R on E is compatible with the internal law of composition f: E × E → E on E means that the mapping f is compatible (in the sense of Set Theory, II, § 6, no. 5) with the product equivalence relation R × R on E × E and the equivalence relation R on E. (Set Theory, II, § 6, no. 8). This also means that the graph of R is a submagma of E × E.

If the law T is associative (resp. commutative) so is the quotient law (more briefly we say that associativity, or commutativity, is preserved when passing to the quotient).

The canonical mapping from the magma E to the magma E/R is a homomorphism.

For a mapping g of E/R into a magma F to be a homomorphism it is necessary and sufficient that the composition of g with the canonical mapping of E onto E/R be a homomorphism.

The two following propositions are immediate from the definitions:

#### Proposition 6 {#alg-i-s1-prop-6 .statement}

Let E and F be two magmas and f a homomorphism of E into F. Let R[x, y] denote the relation f(x) = f(y) between elements x, y of E. Then R is an equivalence relation on E compatible with the law on E and the mapping of E/R onto f(E) derived from f by passing to the quotient is an isomorphism of the quotient magma E/R onto the submagma f(E) of F.

#### Proposition 7 {#alg-i-s1-prop-7 .statement}

Let E be a magma and R an equivalence relation on E compatible with the law on E. For an equivalence relation S on E/R to be compatible with the quotient law it is necessary and sufficient that S be of the form T/R where T is an equivalence relation on E implied by R and compatible with the law on E. The canonical mapping of E/T onto (E/R)/(T/R) (Set Theory, II, § 6, no. 7) is then a magma isomorphism.

#### Proposition 8 {#alg-i-s1-prop-8 .statement}

Let E be a magma, A a stable subset of E and R an equivalence relation on E compatible with the law on E. The saturation B of A with respect to R (Set

Let $\top$ denote the law on $E$. If $x$ and $y$ are two elements of $B$ there exist two elements $x'$ and $y'$ of $A$ such that $x \equiv x' \pmod{R}$ and $y \equiv y' \pmod{R}$; then $x \top y \equiv x' \top y' \pmod{R}$ and $x' \top y' \in A$, whence $x \top y \in B$. Thus $B$ is a stable subset of $E$ and the other assertions are obvious.

Let $M$ be a magma and $((u_\alpha, v_\alpha))_{\alpha \in I}$ a family of elements of $M \times M$. Consider all the equivalence relations $S$ on $M$ which are compatible with the law on $M$ and such that $u_\alpha \equiv v_\alpha \pmod{S}$ for all $\alpha \in I$. The intersection of the graphs of these relations is the graph of an equivalence relation $R$ which is compatible with the law on $M$ and such that $u_\alpha \equiv v_\alpha \pmod{R}$. Hence $R$ is the finest (Set Theory, III, § 1, nos. 3 and 7) equivalence relation with these two properties. It is called the equivalence relation compatible with the law on $M$ generated by the $(u_\alpha, v_\alpha)$.

#### Proposition 9 {#alg-i-s1-prop-9 .statement}

Preserving the above notation, let $f$ be a homomorphism of $M$ into a magma such that $f(u_\alpha) = f(v_\alpha)$ for all $\alpha \in I$. Then $f$ is compatible with $R$.

Let $T$ be the equivalence relation associated with $f$. Then $u_\alpha \equiv v_\alpha \pmod{T}$ for all $\alpha \in I$ and $T$ is compatible with the law on $M$, hence $T$ is coarser than $R$; this proves the proposition.

### Exercises {#alg-i-s1-exercises}

See the [exercises for § 1](exercises/s1/).
