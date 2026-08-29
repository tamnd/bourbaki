---
book: ac
book_title: Commutative Algebra
chapter: II
chapter_title: LOCALIZATION
section: 1
section_title: Prime ideals
lang: en
source: ac-i-vii
book_pages: 51-55, 121-123
pdf_pages: 0071-0075, 0141-0143
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF PRIME IDEALS
      page: 51
      pdf_page: 71
    - "no": 2
      title: RELATIVELY PRIME IDEALS
      page: 53
      pdf_page: 73
statements: 9
exercises: 11
content_sha256: eaf2b502618aa5ba762ff7b78f5dd83041b3b831304194dfec9cee96f2fab555
---

## 1. PRIME IDEALS

### 1. DEFINITION OF PRIME IDEALS

#### Definition 1 {#ac-ii-s1-def-1 .statement}

An ideal $p$ of a ring $A$ is called prime if the ring $A/p$ is an integral domain.

By this definition, an ideal $p$ of a ring $A$ is prime if the following two conditions hold:
(1) $p \neq A$;
(2) if $x, y$ are two elements of $A$ such that $x \notin p$ and $y \notin p$, then $xy \notin p$.

These conditions can also be expressed by saying that the product of any finite family of elements of $\mathfrak{g}p$ belongs to $\mathfrak{g}p$, as applying this condition to the empty set yields $1 \notin p$.

A maximal ideal $m$ of $A$ is prime since $A/m$ is a field; then it follows from Krull's theorem (Algebra, Chapter I, § 8, no. 7, Theorem 2) that every ideal of

(*) With the exception of the statements placed between two asterisks: \* ... *, the results of this chapter depend only on Books I to VI and Chapter I, §§ 1–3 of this Book.

A *other than* $\mathbf{A}$ is contained in at least one prime ideal. In particular, for prime ideals to exist in a ring $\mathbf{A}$, it is necessary and sufficient that $\mathbf{A}$ be not reduced to 0.

Let $f : \mathbf{A} \to \mathbf{B}$ be a ring homomorphism and $q$ an ideal of $\mathbf{B}$. Set $p = f^{-1}(q)$; the homomorphism $\overline{f} : \mathbf{A}/p \to \mathbf{B}/q$ derived from $f$ by taking quotients is injective. Suppose that $q$ is prime; as the ring $\mathbf{B}/q$ is an integral domain, so is $\mathbf{A}/p$, being isomorphic to a subring of $\mathbf{B}/q$; consequently the ideal $p = f^{-1}(q)$ is prime. In particular, let $\mathbf{A}$ be a subring of $\mathbf{B}$; for every ideal $q$ of $\mathbf{B}$, $q \cap \mathbf{A}$ is a prime ideal $\mathbf{A}$. If $f$ is surjective, $\overline{f}$ is an isomorphism; the conditions "p is prime" and "$q$ is prime" are then equivalent. Hence, if $p$ and $a$ are ideals of $\mathbf{A}$ such that $a \subset p$, a necessary and sufficient condition for $p$ to be prime is that $p/a$ be prime in $\mathbf{A}/a$.

#### Proposition 1 {#ac-ii-s1-prop-1 .statement}

*Let $\mathbf{A}$ be a ring, $a_1, a_2, \ldots, a_n$ ideals of $\mathbf{A}$ and $p$ a prime ideal of $\mathbf{A}$. If $p$ contains the product $a_1 a_2 \ldots a_n$, it contains at least one of the $a_i$.*

Suppose in fact that $p$ contains none of the $a_i$. For $1 \leq i \leq n$ there exists then an element $s_i \in a_i \cap p$; then $s = s_1 s_2 \ldots s_n$ is contained in $a_1 a_2 \ldots a_n$, and is not contained in $p$, which is absurd.

#### Corollary {#ac-ii-s1-n1-cor-1 .statement}

*Let $m$ be a maximal ideal of $\mathbf{A}$; for every integer $n > 0$, the only prime ideal containing $m^n$ is $m$.*

Such an ideal $p$ must contain $m$ by Proposition 1 applied to $a_i = m$ for $1 \leq i \leq n$; as $m$ is maximal, $p = m$.

#### Proposition 2 {#ac-ii-s1-prop-2 .statement}

*Let $\mathbf{A}$ be a ring, $a$ a non-empty set of $\mathbf{A}$ which is closed under addition and multiplication and $(p_i)_{i \in I}$ a non-empty finite family of ideals of $\mathbf{A}$. Suppose that $a$ is contained in the union of the $p_i$ and that at most two of the $p_i$ are not prime. Then $a$ is contained in one of the $p_i$.*

We argue by induction on $n = \mathrm{Card}(I)$; the proposition is trivial if $n = 1$. Suppose that $n \geq 2$; if there exists an index $j$ such that $a \cap p_j \subset \bigcup_{i \neq j} p_i$, the set $a$, which is the union of the $a \cap p_i$ where $i \in I$, is contained in $\bigcup_{i \neq j} p_i$ and hence in one of the $p_i$ by the induction hypothesis. Suppose then that such an index does not exist; for every $j \in I$ let $y_j$ be an element of $a \cap p_j$ not belonging to any $p_i$ for $i \neq j$. Let $k$ be an element of $I$ chosen in such a way that $p_k$ is prime if $n > 2$ and chosen arbitrarily if $n = 2$; let $z = y_k + \prod_{i \neq k} y_i$. Then $z \in a$, since $a$ is closed under addition and multiplication; if $j \neq k$, $\prod_{i \neq k} y_i$ belongs to $p_j$, but $y_k \notin p_j$, whence $z \notin p_j$. On the other hand, $\prod_{i \neq k} y_i$ does not belong to $p_k$, as none of the factors $y_i \ (i \neq k)$ belongs to it and $p_k$ is prime if $n - 1 > 1$; as $y_k \in p_k$, $z$ does not belong to $p_k$ and the proposition is established.

### 2. RELATIVELY PRIME IDEALS

Let $A$ be a ring; two ideals $a, b$ of $A$ are called *relatively prime* if $a + b = A$. For this to be true, it is necessary and sufficient that $a + b$ be contained in no prime ideal (*Algebra*, Chapter I, § 8, no. 7, Theorem 2), in other words, that no prime ideal contain both $a$ and $b$. Two distinct maximal ideals are relatively prime.

If $A$ is a *principal ideal domain* (*Algebra*, Chapter VII, § 1), for two elements $a, b$ of $A$ to be relatively prime, it is necessary and sufficient, by Bezout’s identity (*loc. cit.*, no. 2, Theorem 1), that the ideals $Aa$ and $Ab$ be relatively prime.

#### Proposition 3 {#ac-ii-s1-prop-3 .statement}

*Let $a$ and $b$ be two relatively prime ideals of a ring $A$. Let $a'$ and $b'$ be two ideals of $A$ such that every element of $a$ (resp. $b$) has a power in $a'$ (resp. $b'$). Then $a'$ and $b'$ are relatively prime.*

Under the given hypothesis, every prime ideal which contains $a'$ contains $a$ and every prime ideal which contains $b'$ contains $b$. If a prime ideal contains $a'$ and $b'$, then it contains $a$ and $b$, which is absurd, since $a$ and $b$ are relatively prime; hence $a'$ and $b'$ are relatively prime.

#### Proposition 4 {#ac-ii-s1-prop-4 .statement}

*Let $a, b_1, \ldots, b_n$ be ideals of a ring $A$. If $a$ is relatively prime to each of the $b_i$ ($1 \leq i \leq n$), it is relatively prime to $b_1 b_2 \ldots b_n$.

Let $p$ be a prime ideal of $A$. If $p$ contains $a$ and $b_1 b_2 \ldots b_n$ it contains one of the $b_i$ (no. 1, Proposition 1), which is absurd since $a$ and $b_i$ are relatively prime.

#### Proposition 5 {#ac-ii-s1-prop-5 .statement}

*Let $(a_i)_{i \in I}$ be a non-empty finite family of ideals of a ring $A$. The following properties are equivalent =
(a) For $i \neq j$, $a_i$ and $a_j$ are relatively prime.
(b) *The canonical homomorphism* $\phi : A \to \prod_{i \neq I} (A/a_i)$ (*Algebra*, Chapter 11, § 1, no. 7) is surjective.
*If these hold, the intersection $a$ of the $a_i$ is equal to their product and the canonical homomorphism* $\phi : A/a \to \prod_{i \in I} (A/a_i)$ (*Algebra*, Chapter II, § 1, no. 7) is bijective.*

We argue by induction on $n$ the number of elements in $I$, the case $n = 1$ being trivial. Consider first the case $n = 2$. Then the equivalence of (a) and (b) follows from the exactness of the sequence

$$
0 \longrightarrow A/(a_1 \cap a_2) \xrightarrow{\psi} (A/a_1) \oplus (A/a_2) \longrightarrow A/(a_1 + a_2) \longrightarrow 0
$$

(Algebra, Chapter II, § 1, no. 7, formula (30)). Moreover, there exist $e_1 \in a$, and $e_2 \in a_2$ such that $1 = e_1 + e_2$; then, for all $x \in a = a_1 \cap a_2$, $x = xe_1 + xe_2$; but by definition $xe_1 \in a_1 a_2$ and $xe_2 \in a_1 a_2$, hence $x \in a_1 a_2$; whence $a \subset a_1 a_2$ and the converse inclusion is obvious.

In the general case, suppose that condition (a) holds and let $k$ be an element of $I$ and $b_k = \bigcap_{i \neq k} a_i$; the induction hypothesis implies that $b_k = \prod_{i \in I} a_i$, and it follows from Proposition 4 that $a$, and $b$, are relatively prime; then

$$
a = \bigcap_{i \in I} a_i = a, \quad \cap b_k = a_k b_k = \prod_{i \in I} a_i,
$$

by the first part of the argument and for the same reason the canonical homomorphism $A/a \twoheadrightarrow (A/a_k) \times (A/b_k)$ is bijective; by the induction hypothesis the canonical homomorphism $A/b_k \to \prod_{i \neq k} (A/a_i)$ is bijective and so then is the composite homomorphism

$$
A/a \to (A/a_k) \times (A/b_k) \to (A/a_k) \times \prod_{i \neq k} (A/a_i) = \prod_{i \in I} (A/a_i)
$$

which is precisely $\psi$; that is, (b) holds. Conversely, suppose that (b) holds. We show that the $a_i$ are necessarily relatively prime in pairs. In the contrary case, there would exist an ideal $c \neq A$ containing $a_i$ and $a_j$, for $i \neq j$. We set $a_h' = a_h$ for $h$ not equal to $i$ or $j$ and $a_i' = a_j' = c$; the canonical homomorphism $\phi': A \to \prod_{i \in I} (A/a_i')$ can be written as the composite mapping

$$
A \xrightarrow{\phi} \prod_{i \in I} (A/a_i) \xrightarrow{f} \prod_{i \in I} (A/a_i')
$$

$f$ being the product of the canonical homomorphisms $A/a_i \to A/a_i'$; clearly $\phi'$ is not surjective, the projection of $+(A)$ onto $(A/a_i') \times (A/a_i')$ being the diagonal of the product $(A/c) \times (A/c)$, which is distinct from this product since $c \neq A$. As $f$ is surjective, this shows that $\phi$ is not surjective.

#### Proposition 6 {#ac-ii-s1-prop-6 .statement}

*Let $(a_i)_{i \in I}$ be a non-empty finite family of ideals of a ring $A$ which are relatively prime in pairs; let $a$ be the intersection of the $a_i$. For every $A$-module $M$, the canonical mapping $M \to \prod_{i \in I} (M/a_i M)$ is surjective and its kernel is $aM$.*

Clearly the canonical mapping of $M$ to $\prod_{i \in I} (M/a_i M)$ is zero on $aM$; then, by taking quotients, it defines a homomorphism $A : M/aM \to \prod_{i \in I} (M/a_i M)$. On the other hand, by Proposition 5, the canonical homomorphism
$$
\psi : A/a \to \prod_{i \in I} (A/a_i)
$$
is bijective. Then so is $1_M \otimes \psi : M \otimes (A/a) \to M \otimes \prod_{i \in I} (A/a_i)$. Now $M \otimes (A/a)$ is identified with $M/aM$ and $M \otimes \prod_{i \in I} (A/a_i)$ with $\prod_{i \in I} M \otimes (A/a_i)$, which is itself identified with $\prod_{i \in I} (M/a_i M)$. It is immediately verified that the above identifications transforms $1_M \otimes \psi$ into $\lambda$, whence the proposition.

#### Example {#ac-ii-s1-n2-exa-1 .statement}

Let $K$ be a field, $a, (1 \leq i \leq m)$ distinct elements of $K$ and, for each $i$, let $g_i$ be a polynomial in $K[X]$; the principal ideal $(X - a_i) = m_i$ is maximal in $K[X]$, hence, for every system $(n_i)_{1 \leq i \leq m}$ of $m$ integers $\geq 1$, the ideals $m_i^{n_i}$ are relatively prime in pairs. Then it follows from Proposition 5 that there exists a polynomial $f \in K[X]$ such that $f(X) \equiv g_i(X) \pmod{(X - a_i)^{n_i}}$ for $1 \leq i \leq m$, the difference of two such polynomials being divisible by $\omega(X) = \prod_{i=1}^m (X - a_i)^{n_i}$. If all the $n_i$ are taken equal to 1, we find the problem is solved explicitly by Lagrange's interpolation formula (*Algebra*, Chapter IV, § 2, no. 4).

### Exercises {#ac-ii-s1-exercises}

See the [exercises for § 1](exercises/s1/).
