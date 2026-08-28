---
book: ac
book_title: Commutative Algebra
chapter: V
chapter_title: INTEGERS
section: 2
section_title: The lift of prime ideals
lang: en
source: ac-i-vii
book_pages: 325-344, 362-369
pdf_pages: 0344-0363, 0381-0388
extraction: ocr
subsections:
    - "no": 1
      title: THE FIRST EXISTENCE THEOREM
      page: 325
      pdf_page: 344
    - "no": 2
      title: DECOMPOSITION GROUP AND INERTIA GROUP
      page: 330
      pdf_page: 349
    - "no": 3
      title: DECOMPOSITION AND INERTIA FOR INTEGRALLY CLOSED DOMAINS
      page: 337
      pdf_page: 356
    - "no": 4
      title: THE SECOND EXISTENCE THEOREM
      page: 343
      pdf_page: 362
statements: 36
exercises: 22
content_sha256: 0735cbdcddf5abb906e8dd4e39035bbe753450d10e43d8bd20b9833595a17cd5
---

## 2. THE LIFT OF PRIME IDEALS

### 1. THE FIRST EXISTENCE THEOREM

#### Definition 1 {#ac-v-s2-def-1 .statement}

Let $\mathbf{A}, \mathbf{A}'$ be two rings and $h : \mathbf{A} \to \mathbf{A}'$ a ring homomorphism. An ideal $a' \in A'$ is said to lie above an ideal $a$ of $\mathbf{A}$ if $a = \overline{h}^1(a')$.

To say that a prime ideal $p'$ of $A'$ lies above an ideal $p$ of $\mathbf{A}$ therefore means that $p$ is the image of $p'$ under the continuous mapping "$h : \mathrm{Spec}(A') \to \mathrm{Spec}(A)$" associated with $h$ (Chapter 11, § 4, no. 3).

Note that for there to exist an ideal of $A'$ lying above the ideal $(0)$ of $\mathbf{A}$, it is necessary and sufficient that $h : \mathbf{A} \to \mathbf{A}'$ be injective.

Let $a$ be an ideal of $\mathbf{A}$; by taking quotients the homomorphism $h$ gives a homomorphism $h_1 : \mathbf{A}/a \to \mathbf{A}'/a'$; to say that $a'$ is an ideal of $A'$ lying above $a$ is equivalent to saying that $aA' \subset a'$ and that $a'/aA'$ is an ideal of $\mathbf{A}'/aA'$ lying above $(0)$.

#### Lemma 1 {#ac-v-s2-lem-1 .statement}

Let $h : \mathbf{A} \to \mathbf{A}'$ be a ring homomorphism, $S$ a multiplicative subset of $\mathbf{A}$, $i = i_A^S : \mathbf{A} \to S^{-1}\mathbf{A}$, $i' = i_{A'}^{h(S)} : \mathbf{A}' \to S^{-1}\mathbf{A}' = (h(S))^{-1}\mathbf{A}'$ the canonical homomorphisms and $h_1 = S^{-1}h : S^{-1}\mathbf{A} \to S^{-1}\mathbf{A}'$, so that there is a commutative diagram

$$
\begin{array}{ccc}
\mathbf{A} & \xrightarrow{h} & \mathbf{A}' \\
i \downarrow & & i' \downarrow \\
S^{-1}\mathbf{A} & \xrightarrow{h_1} & S^{-1}\mathbf{A}'
\end{array}
$$

Let $p$ be a prime ideal of $\mathbf{A}$ such that $p \cap S = \varnothing$. Then $a' \mapsto S^{-1}a'$ is a surjective mapping of the set $\mathcal{F}$ of ideals of $\mathbf{A}'$ lying above $p$ onto the set $\mathcal{F}_1$ of ideals of $S^{-1}\mathbf{A}'$ lying above $S^{-1}p$ and the mapping $a'_1 \mapsto i'(a'_1)$ is a bijection of $\mathcal{F}_1$ onto the set of ideals belonging to $\mathcal{F}$ and is saturated with respect to $h(S)$; in particular $p' \mapsto S^{-1}p'$ is a bijection of the set of prime ideals of $\mathbf{A}'$ lying above $p$ onto the set of prime ideals of $S^{-1}\mathbf{A}'$ lying above $S^{-1}p$.

We know that $S^{-1}p$ is a prime ideal of $S^{-1}\mathbf{A}$ and that $i_1(S^{-1}p) = p$ (Chapter 11, § 2, no. 5, Proposition 11); if there exists an ideal $b'$ of $S^{-1}\mathbf{A}'$ lying above $S^{-1}p$, then $h(i_1(b')) = i(h_1(b')) = p$; as $S^{-1}i'(b') = b'$ (loc. cit.), this already shows that the image of $\mathcal{F}$ under the mapping $a' \mapsto S^{-1}a'$ contains $\mathcal{F}_1$. On the other hand, if $a' \in \mathcal{F}$, $a \in A$ and $s \in S$, there are the following equivalences

$$
h_1(a/s) \in S^{-1}a' \iff h(a)/h(s) \in S^{-1}a'
$$
$\iff$ there exists $t \in S$ such that $h(t)h(a) \in a'$
$\iff$ there exists $t \in S$ such that $ta \in \mathfrak{p}$
$\iff a/z \in S^{-1}\mathfrak{p}$.

Hence $h_1^{-1}(S^{-1}a') = S^{-1}\mathfrak{p}$, which completes the proof that the image of $\mathcal{F}$ under the mapping $a' \mapsto S^{-1}a'$ is equal to $\mathcal{F}_1$; the other assertions follow from Chapter 11, § 2, no. 5, Proposition 11.

#### Proposition 1 {#ac-v-s2-prop-1 .statement}

*Let $h : A \to A'$ be a ring homomorphism such that $A'$ is integral over $A$, $\mathfrak{p}'$ a prime ideal of $A'$ and $\mathfrak{p} = h^{-1}(\mathfrak{p}')$. For $\mathfrak{p}$ to be maximal, it is necessary and sufficient that $\mathfrak{p}'$ be so.*

Let us write $B = A/\mathfrak{p}$, $B' = A'/\mathfrak{p}'$ and let $h_1 : B \to B'$ be the homomorphism derived from $h$ by taking quotients; $B$ and $B'$ are integral domains and $B'$ is integral over $B$ ($§ 1$, no. 1, Proposition 2). To say that $\mathfrak{p}$ (resp. $\mathfrak{p}'$) is maximal means that $B$ (resp. $B'$) is a field. The proposition then follows from the following lemma:

#### Lemma 2 {#ac-v-s2-lem-2 .statement}

*Let $B$ be an integral domain and $A$ a subring of $B$ such that $B$ is integral over $A$. For $B$ to be a field, it is necessary and sufficient that $A$ be a field.*

If $A$ is a field, then, for ally $\neq 0$ in $B$, $A[y]$ is by hypothesis ($§ 1$, Theorem 1) a finitely generated $A$-module; as $A[y]$ is an integral domain, it is a field (*Algebra*, Chapter V, § 2, no. 1, Proposition 1) and *a fortiori* $y$ is invertible in $B$ and hence $B$ is a field. Conversely, suppose that $B$ is a field and let $z \neq 0$ in $A$; as $z^{-1} \in B$, $z^{-1}$ is integral over $A$, in other words there is an equation of integral dependence

$$
z^{-n} + a_1 z^{-(n-1)} + \ldots + a_n = 0
$$

where the $a_i \in A$; now this relation shows that

$$
-z^{-1} = a_1 + a_2 z + \ldots + a_n z^{n-1} \in A,
$$

hence $A$ is certainly a field.

#### Corollary 1 {#ac-v-s2-lem-2-cor-1 .statement}

*Let $h : A \to A'$ a ring homomorphism such that $A'$ is integral over $A$, $\mathfrak{p}$ a prime ideal of $A$ and $\mathfrak{p}'$ and $a'$ two ideals of $A'$ lying above $\mathfrak{p}$ such that $\mathfrak{p}' \subset a'$. If $\mathfrak{p}'$ is prime, then $a' = \mathfrak{p}'$.*

Let us write $S = A - \mathfrak{p}$; then $S^{-1}A'$ is integral over $S^{-1}A$ ($§ 1$, no. 5, Proposition

16), $S^{-1}p$ is a maximal ideal of $S^{-1}A$ (Chapter 11, § 2, no. 5, Proposition 11), $S^{-1}a'$ and $S^{-1}p'$ are ideals of $S^{-1}A'$ lying above $S^{-1}p$ (Lemma 1) and $S^{-1}a' \supseteq S^{-1}p'$. As $S^{-1}p'$ is prime, it is maximal by Proposition 1 and hence $S^{-1}p' = S^{-1}a'$; therefore $a'$ is contained in the saturation of $p'$ with respect to $h(S)$, which is equal to $p'$ (Chapter II, § 2, no. 5, Proposition 11).

#### Corollary 2 {#ac-v-s2-lem-2-cor-2 .statement}

Let $A'$ be an integral domain, $A$ a subring of $A'$ such that $A'$ is integral over $A$ and $f$ a homomorphism from $A'$ to a ring $B$. If the restriction off to $A$ is injective $f$ is injective.

If $a'$ is the kernel off, the hypothesis means that $a' \cap A = (0)$; as $A'$ is an integral domain, Corollary 1 may be applied taking $p$ and $p'$ to be the ideal (0) of $A$ and the ideal (0) of $A'$ respectively, whence $a' = (0)$.

#### Corollary 3 {#ac-v-s2-lem-2-cor-3 .statement}

Let $h : A \to A'$ be a ring homomorphism such that $A'$ is integral over $A$ and $m$ a maximal ideal of $A$ and suppose that there are in $A'$ only a finite number of distinct maximal ideals $m'_j$ ($1 \leq j \leq n$) lying above $m$. Let $q'_j$ be the saturation of $mA'$ with respect to $m'_j$ (Chapter II, § 2, no. 4). Then:
(i) In the ring $A'/q'_j$ the divisors of zero are the elements of $m'_j/q'_j$ and they are nilpotent ($1 \leq j \leq n$).
(ii) $mA' = \bigcap_j q'_j = \prod_j q'_j$.
(iii) The canonical homomorphism $A'/mA' \to \prod_j (A'/q'_j)$ is bijective.

For a prime ideal of $A'$ to contain $mA'$, it is necessary and sufficient that its inverse image under $h$ contain $m$ and hence that it lie above $m$, since $m$ is maximal in $A$; the $m'_j$ are therefore the only prime ideals of $A'$ containing $mA'$ (Proposition 1) and therefore $c' = \bigcap_j m'_j$ is the radical of $mA'$ (Chapter II, § 2, no. 6, Corollary 1 to Proposition 13). By definition of $q'_j$, the class mod. $q'_j$ of an element of $A' - m'_j$ is not a divisor of 0 in $A'/q'_j$; on the other hand, as the $m'_j$ are distinct maximal ideals, for every index $j$ there exists an element $a'_j$ belonging to $\bigcap_j m'_j$ and not to $m'_j$ (Chapter II, § 1, no. 1, Proposition 4): then, for all $x \notin m'_j, a'_j x \in r'$, hence the class mod. $q'_j$ of $a'_j x$ is nilpotent and, as that of $a'_j$ is not a divisor of 0, we conclude that the class of $x$ is nilpotent; in other words $m'_j$ is the radical of $q'_j$, which proves (i). It follows that the $q'_j$ are relatively prime in pairs (Chapter II, § 1, no. 1, Proposition 3); (iii) will therefore be a consequence of (ii), taking account of Chapter II, § 1, no. 2, Proposition 5. To establish (ii), we note that in the ring $A'/mA'$ the $m'_j/mA'$ are the only maximal ideals and $q'_j/mA'$ is the saturation of (0) with respect to $m'_j/mA'$ (Chapter 11, § 2, no. 4); we may therefore restrict our attention to the case $mA' = (0)$; the assertion of (ii) then follows from Chapter II, § 3, no. 3, Corollary 2 to Theorem 1.

Remark (1) If $A'$ is Noetherian, it follows from (i) and (ii) that $(q'_j)_{1 \leq j \leq n}$ is the unique primary decomposition of $mA'$ (Chapter IV, § 2, no. 3).

#### Theorem 1 {#ac-v-s2-thm-1 .statement}

Let $h : A \to A'$ be an injective ring homomorphism such that $A$ is integral over $A$ and $p$ a prime ideal of $A$. There exists a prime ideal $p'$ of $A'$ lying above $p$.

Suppose first that $A$ is a local ring and $p$ the maximal ideal of $A$; then, for every maximal ideal $m'$ of $A'$, $h^{-1}(m')$ is a maximal ideal of $A$ (Proposition 1) and hence equal to $p$, which proves the theorem in this case (since $A'$ contains $A$ by hypothesis and is therefore not reduced to 0). In the general case, let us write $S = A - p$; then $S^{-1}A$ is a local ring whose maximal ideal is $S^{-1}p$ (Chapter 11, § 2, no. 5, Proposition 11), $S^{-1}h : S^{-1}A \to S^{-1}A$, is injective (Chapter II, § 2, no. 4, Theorem 1) and $S^{-1}A'$ is integral over $S^{-1}A$ ($§ 1$, no. 5, Proposition 16); then there exists a prime ideal $q'$ of $S^{-1}A'$ lying above $S^{-1}p$ and we know that $q' = S^{-1}p'$, where $p'$ is a prime ideal of $A'$ lying above $p$ (Lemma 1).

If $h : A \to A'$ is not injective, Theorem 1 is no longer necessarily true, as the example of the homomorphism $Z \to \mathbf{Z}/n\mathbf{Z} \ (n > 1)$ shows. However Theorem 1 can be applied to the canonical injection $h(A) \to A'$; in other words, the statement of Theorem 1 is true for prime ideals $p$ containing $\mathrm{Ker}(h)$.

#### Corollary 1 {#ac-v-s2-thm-1-cor-1 .statement}

With the hypotheses and notation of Theorem 1, $\bar{h}^{-1}(pA') = p$.

$pA' \subset p'$ and $\bar{h}(p') = p$.

#### Corollary 2 {#ac-v-s2-thm-1-cor-2 .statement}

Let $h : A \to A'$ be a ring homomorphism such that $A'$ is integral over $A$, $a$ and $p$ two ideals of $A$ such that $a \subset p$ and $a'$ an ideal of $A'$ lying above $a$. Suppose that $p$ is prime. Then there exists a prime ideal $p'$ of $A'$ lying above $p$ and containing $a'$.

If $h_1 : A/a \to A'/a'$ is the homomorphism derived from $h$ by taking quotients, $h_1$ is injective by hypothesis and $A'/a'$ is integral over $A/a$ ($§ 1$, no. 1, Proposition 2); then there exists a prime ideal $p'/a'$ of $A'/a'$ (p' prime in $A$) lying above $p/a$ (Theorem 1) and $p'$ is the required ideal.

#### Corollary 3 {#ac-v-s2-thm-1-cor-3 .statement}

Let $A$ be a ring and $A'$ a ring containing $A$ and integral over $A$. If $\mathcal{R}'$ is the Jacobson radical of $A'$, $\mathcal{R}' \cap A$ is the Jacobson radical of $A$.

Let $32$ be the Jacobson radical of $A$. For every maximal ideal $m'$ of $A'$, $m' \cap A$ is a maximal ideal of $A$ (Proposition 1), hence $\mathcal{R} \subset m' \cap A$ and therefore $\mathcal{R} \subset \mathcal{R}' \cap A$ (Algebra, Chapter VIII, § 5, no. 3, Definition 3). Conversely, let $x \in 32' \cap A$; for every maximal ideal $m$ of $A$, there exists a prime ideal of $A'$ lying above $m$ (Theorem 1) and this ideal $m'$ is necessarily maximal (Proposition 1), hence $x \in m' \cap A = m$ and therefore $x \in 32$.

#### Corollary 4 {#ac-v-s2-thm-1-cor-4 .statement}

Let $A$ be a ring, $A'$ a ring containing $A$ and integral over $A$ and $f$ a homomorphism from $A$ to an algebraically closed field $L$. Then $f$ can be extended to a homomorphism from $A'$ to $L$.

Let $\mathfrak{p}$ be the kernel of $f$, which is a prime ideal since $f(A) \subset L$ is an integral domain; let $\mathfrak{p}'$ be a prime ideal of $A'$ lying above $\mathfrak{p}$ (Theorem 1). Then $A/\mathfrak{p}$ is canonically identified with a subring of $A'/\mathfrak{p}'$ and $A'/\mathfrak{p}'$ is integral over $A/\mathfrak{p}$ ($§ 1$, no. 1, Proposition 2). The homomorphism $f$ defines, by taking the quotient, an isomorphism of $A/\mathfrak{p}$ onto the subring $f(A)$ of $L$, which can be extended to an isomorphism $g$ of the field of fractions $K$ of $A/\mathfrak{p}$ onto a subfield of $L$. As the field of fractions $K'$ of $A'/\mathfrak{p}'$ is algebraic over $K$, $g$ can be extended to an isomorphism $g'$ of $K'$ onto a subfield of $L$ (Algebra, Chapter V, $§ 4$, no. 2, Corollary to Theorem 1); if $\pi': A' \to A'/\mathfrak{p}'$ is the canonical homomorphism, $g' \circ \pi'$ is a homomorphism from $A'$ to $L$ extending $f$.

Remark (2). Let $h : A \to A'$ be a ring homomorphism such that $A'$ is integral over $A$; then the associated continuous mapping $^a h : \mathrm{Spec}(A') \to \mathrm{Spec}(A)$ is closed. For every ideal $a'$ of $A'$, $A'/a'$ is integral over $A'$, hence also over $A$ ($§ 1$, no. 1, Proposition 6) and $\mathrm{Spec}(A'/a')$ is identified with a closed subspace $V(a')$ of $\mathrm{Spec}(A')$; to show that $^a h$ is closed, we see then (replacing $A'$ by $A'/a'$) that it is sufficient to prove that the image of $\mathrm{Spec}(A)'$ under $^a h$ is a closed subset of $\mathrm{Spec}(A)$; now it follows from Theorem 1 that this image is just the set of prime ideals of $A$ containing the ideal $\mathrm{Ker}(h)$ and this set is closed by definition of the topology on $\mathrm{Spec}(A)$.

#### Proposition 2 {#ac-v-s2-prop-2 .statement}

Let $h : A \to A'$ be a ring homomorphism such that $A'$ is integral over $A$, $\mathfrak{p}$ a prime ideal of $A$, $S = A - \mathfrak{p}$, $(p'_i)_{i \in I}$ the family of all the prime ideals $\mathfrak{p}$ of $A'$ lying above $\mathfrak{p}$ and $S' = \bigcap_{i \in I} (A' - p_i)$; then $S^{-1}A' = {S'}^{-1}A'$.

In fact, by definition $h(S) \subset S'$ and, as

$$
h(S)^{-1}A' = S^{-1}A',
$$

it suffices to prove, by virtue of Chapter II, $§ 2$, no. 3, Proposition 8, that, if a prime ideal $q'$ of $A'$ does not meet $h(S)$, it does not meet $S'$ either. Now, suppose that $q' \cap h(S) = \varnothing$ and let $q = h^{-1}(q')$; then $q \cap S = \varnothing$, in other words $q \subset \mathfrak{p}$. As $q'$ lies above $q$ by definition, it follows from Corollary 2 to Proposition 1 that there is an index $c$ such that $q' \subset p'_c$ and hence $q' \cap S' = \varnothing$, which completes the proof.

#### Proposition 3 {#ac-v-s2-prop-3 .statement}

Let $h : A \to A'$ be a ring homomorphism such that $A'$ is a finitely generated $A$-module; then, for every prime ideal $\mathfrak{p}$ of $A$, the set of prime ideals of $A'$ lying above $\mathfrak{p}$ is finite.

Let $S = A - p$; by Lemma 1 we may replace $A$ by $S^{-1}A$, $A'$ by $S^{-1}A'$ (which is a finitely generated $S^{-1}A$-module) and $p$ by $S^{-1}p$; in other words, we may assume that $A$ is a local ring and $p$ is its maximal ideal. Then (by the remark made at the beginning of this no.) $A$ may be replaced by $A/p$, $A'$ by $A'/pA'$ and $p$ by $(0)$, for $A'/pA' = (A/p) \otimes_A A'$ is a finitely generated $(A/p)$-module. Thus we have finally reduced the problem to proving the proposition when $A$ is a field and $p = (0)$; $A'$ is then an $A$-algebra of finite rank and therefore Artinian and we know that in such an algebra there is only a finite number of prime ideals (Chapter IV, § 2, no. 5, Proposition 9).

### 2. DECOMPOSITION GROUP AND INERTIA GROUP

#### Definition 2 {#ac-v-s2-def-2 .statement}

Let $A'$ be a ring and $G$ a group operating on $A'$ ($§ 1$, no. 9). Given a prime ideal $p' \subset A'$ the subgroup of elements $\sigma \in G$ such that $\sigma.p' = p'$ is called the decomposition group of $p'$ (with respect to $G$) and is denoted by $G^z(p')$. The ring of elements of $A'$ invariant under $G^z(p')$ is called the decomposition ring of $p'$ (with respect to $G$) and is denoted by $A^z(p')$ (*).

We often write $G^z$ and $A^z$ instead of $G^z(p')$ and $A^z(p')$ respectively, when there is no ambiguity.

For all $\sigma \in G^z(p')$ we also denote by $z \mapsto \sigma.z$ the endomorphism of the ring $A'/p'$ derived from the endomorphism $x \mapsto \sigma.x$ of $A'$ by taking quotients; clearly the group $G^z(p')$ operates in this way on the ring $A'/p'$.

#### Definition 3 {#ac-v-s2-def-3 .statement}

With the notation of Definition 2, the subgroup of $G^z(p')$ consisting of those $\sigma$ such that the endomorphism $z \mapsto \sigma.z$ of $A'/p'$ is the identity is called the inertia group of $p'$ (with respect to $G$) and denoted by $G^T(p')$ (or $G^T$). The ring of elements of $A'$ invariant under $G^T(p')$ is called the inertia ring of $p'$ (with respect to $G$) and is denoted by $A^T(p')$ (or $A^T$) (†).

If $A$ is the subring of $A'$ consisting of the invariants of $G$, clearly

$$
A \subset A^z(p') \subset A^T(p') \subset A'.
$$

It follows from Definitions 2 and 3 that, for all $p \in G$,

$$
G^z(\rho.p') = \rho G^z(p') \rho^{-1}, \quad G^T(\rho.p') = \rho G^T(p') \rho^{-1}.
$$

If, for all $\sigma \in G^z(p')$, $\bar{\sigma}$ is the automorphism $z \mapsto \sigma.z$ of $A'/p'$, $\sigma \mapsto \bar{\sigma}$ is a homomorphism (called canonical) of $G^z$ to the group $\Gamma_0$ of automorphisms of

(*) The letter $Z$ is the initial of the German word "Zerlegung" which means "decomposition."
(†) The letter T is the initial of the German word "Tragheit" which means "inertia."

A'/p' leaving invariant the elements of $A^{\mathbf{Z}}/(p' \cap A^{\mathbf{Z}})$ (canonically identified with a subring of $A'/p'$) and by definition $\mathcal{G}^{\Gamma}(p')$ is the kernel of this canonical homomorphism; $\mathcal{G}^{\Gamma}$ is therefore a normal subgroup of $\mathcal{G}^{\mathbf{Z}}$. If $k'$ is the field of fractions of $A'/p'$, every automorphism of $A'/p'$ can be extended uniquely to an automorphism of $k'$, so that $\sigma \mapsto \bar{\sigma}$ can be considered as a homomorphism from $\mathcal{G}^{\mathbf{Z}}(p')$ to the group of automorphisms of $k'$. Note finally that, since $\mathcal{G}^{\Gamma}$ is normal in $\mathcal{G}^{\mathbf{Z}}$, $A^{\Gamma}$ is stable under $\mathcal{G}^{\mathbf{Z}}$.

#### Lemma 3 {#ac-v-s2-lem-3 .statement}

*Let $A'$ be a ring, $\mathcal{G}$ a group operating on $A'$, $A$ the ring of invariants of $\mathcal{G}$, $p'$ a prime ideal of $A'$ and $S$ a multiplicative subset of $A$ not meeting $p'$. Then $\mathcal{G}^{\mathbf{Z}}(S^{-1}p') = \mathcal{G}^{\mathbf{Z}}(p')$, $\mathcal{G}^{\Gamma}(S^{-1}p') = \mathcal{G}^{\Gamma}(p')$ and, if $\mathcal{G}$ is locally finite, $S^{-1}A^{\mathbf{Z}}(p') = A^{\mathbf{Z}}(S^{-1}p')$ and $S^{-1}A^{\Gamma}(p') = A^{\Gamma}(S^{-1}p')$.*

As the elements of $S$ are invariant under $\mathcal{G}$, clearly, if $\sigma.p' = p'$, also $\sigma.(S^{-1}p') = S^{-1}p'$. Conversely, suppose that $\sigma \in \mathcal{G}$ is such that $\sigma.(S^{-1}p') = S^{-1}p'$; then, if $x \in p'$, $(\sigma.x)/1 \in S^{-1}p'$ and there therefore exists $s \in S$ such that $s(\sigma.x) \in p'$, whence $\sigma.x \in p'$ since $p'$ is prime and $s \notin p'$; this proves that $\sigma.p' \subset p'$ and it can be similarly shown that $\sigma^{-1}.p' \subset p'$, hence $\sigma.p' = p'$ and $\sigma \in \mathcal{G}^{\mathbf{Z}}(p')$. If $\sigma \in \mathcal{G}^{\Gamma}(p')$, then $\sigma.x - x \in p'$ for all $x \in A'$, hence also, for all $s \in S$,

$$
\sigma.(x/s) - (x/s) = (O.x - x)/s \in S^{-1}p'
$$

and therefore $\sigma \in \mathcal{G}^{\Gamma}(S^{-1}p')$. Conversely, suppose that $\sigma \in \mathcal{G}^{\Gamma}(S^{-1}p')$; then, for all $x \in A'$, $\sigma.(x/1) - (x/1) \in S^{-1}p'$ and therefore there exists $s \in S$ such that $s(\sigma.x - x) \in p'$, whence as above $\sigma.x - x \in p'$, which proves that $\sigma \in \mathcal{G}^{\Gamma}(p')$. The last two assertions follow from § 1, no. 9, Proposition 23.

#### Theorem 2 {#ac-v-s2-thm-2 .statement}

*Let $A'$ be a ring, $\mathcal{G}$ a finite group operating on $A'$ and $A$ the ring of invariants of $\mathcal{G}$, so that $A'$ is integral over $A$ (§ 1, no. 9, Proposition 22).*

(i) *Given two prime ideals $p', q'$ of $A'$ lying above the same prime ideal $p$ of $A$, there exists $\sigma \in \mathcal{G}$ such that $q' = \sigma.p'$; in other words, $\mathcal{G}$ operates transitively on the set of prime ideals of $A'$ lying above $p$.*

(ii) *Let $p'$ be a prime ideal of $A'$, $p = p' \cap A$ and $k$ (resp. $k'$) the field of fractions of $A/p$ (resp. $A'/p'$). Then $k'$ is a quasi-Galois extension (*) of $k$ and the canonical homomorphism $\sigma \mapsto \bar{\sigma}$ from $\mathcal{G}^{\mathbf{Z}}(p')$ to the group $\Gamma$ of $k$-automorphisms of $k'$ defines, by taking the quotient, an isomorphism of $\mathcal{G}^{\mathbf{Z}}(p')/\mathcal{G}^{\Gamma}(p')$ onto $\Gamma$.*

(*) In order to avoid confusion with other meanings of the word "normal" we henceforth use the term "quasi-Galois extension" as synonymous with the term "normal extension" defined in Algebra, Chapter V, § 6, no. 2, Definition 2.

(i) If $x \in \mathfrak{q}$ then $\prod_{\sigma \in \mathcal{G}} \sigma.x \in q' \cap A = p \subset p'$; then there exists $\sigma \in \mathcal{G}$ such that $\sigma.x \in p'$, that is $x \in \sigma^{-1}.q'$. We conclude that $q' \subset \bigcup_{\sigma \in \mathcal{G}} \mathfrak{s}.\mathfrak{p}'$ and hence (since $\mathcal{G}$ is finite and the $\mathfrak{s}.\mathfrak{p}'$ prime) there exists $\sigma \in \mathcal{G}$ such that $\mathfrak{q}' \subset \mathfrak{s}.\mathfrak{p}'$ (Chapter II, § 1, no. 1, Proposition 2); as $q'$ and $\sigma.\mathfrak{p}'$ both lie above $p$, $q' = \sigma.\mathfrak{p}'$ (no. 1, Corollary 1 to Proposition 1).

(ii) To see that $k'$ is a quasi-Galois extension of $k$, it suffices to prove that every element $\bar{x} \in A'/p'$ is a root of a polynomial $P$ in $k[X]$ all of whose roots are in $A'/p'$ (Algebra, Chapter V, § 6, no. 3, Corollary 3 to Proposition 9). Now, let $x \in A'$ be a representative of the class $\bar{x}$; the polynomial $Q(X) = \prod_{\sigma \in \mathcal{G}} (X - \sigma.x)$ has all its coefficients in $A$; let $P(X)$ be the polynomial in $(A/p)[X]$ whose coefficients are the images of those of $Q$ under the canonical homomorphism $\pi : A \to A/p$. As $\pi$ may be considered as the restriction to $A$ of the canonical homomorphism $\pi' : A' \to A'/p'$, it is seen that $P$ is the product in $(A'/p')[X]$ of the linear factors $X - \pi'(\sigma.x)$ and therefore solves the problem since $\bar{x} = \pi'(x)$.

Clearly, for all $\sigma \in \mathcal{G}^z$, $\hat{\sigma}$ is a $k$-automorphism of $k'$; it remains to verify that $\sigma \mapsto \hat{\sigma}$ maps $\mathcal{G}^z$ onto the group of all $k$-automorphisms of $k'$. Let us write $S = A - p$; $k$ and $k'$ are not changed by replacing $A'$ and $p'$ by $S^{-1}A'$ and $S^{-1}p'$ respectively, by virtue of § 1, no. 9, Proposition 23 and the relation $S^{-1}p' \cap S^{-1}A = S^{-1}(A \cap p') = S^{-1}p$ (Chapter 11, § 2, no. 4); it follows from Lemma 3 that neither $\mathcal{G}^z$ nor its operation on $k'$ is changed; we may therefore restrict our attention to the case where $p$ is maximal, in which case we know that so is $p'$ (no. 1, Proposition 1) and every element of $k'$ is therefore of the form $\pi'(x)$ for some $x \in A'$; it has been seen above that such an element is a root of a polynomial in $k[X]$ of degree $\leq \mathrm{Card}(\mathcal{G})$. As every finite separable extension of $k$ admits a primitive element (Algebra, Chapter V, § 7, no. 7, Proposition 12 and § 11, no. 4, Proposition 4), it is seen that every finite separable extension of $k$ contained in $k'$ is of degree $\leq \mathrm{Card}(\mathcal{G})$, whence it follows that the greatest separable extension $k'_s$ of $k$ contained in $k'$ (Algebra, Chapter V, § 7, no. 6, Proposition 11) is of degree $\leq \mathrm{Card}(\mathcal{G})$ (Algebra, Chapter V, § 3, no. 2, Remark 2). Let $y \in A'$ be an element such that $\pi'(y)$ is a primitive element of $k'_s$. The ideals $\sigma.p'$ for $\sigma \in \mathcal{G} - \mathcal{G}^z$ are maximal and distinct from $p'$ by definition; there therefore exists $x \in A'$ such that $x \equiv y \pmod{p'}$ and $x \in \sigma^{-1}p'$ for $\sigma \in \mathcal{G} - \mathcal{G}^z$ (Chapter 11, § 1, no. 2, Proposition 5). This being so, let $u$ be a $k$-automorphism of $k'$ and let $P(X) = \prod_{\sigma \in \mathcal{G}} (X - \pi'(\sigma.x))$; as $\pi'(x)$ is a root of $P$ and $P \in k[X]$, $u(\pi'(x))$ is also a root of $P$ in $k'$ and hence there exists $\tau \in \mathcal{G}$ such that

$$
u(\pi'(x)) = \pi'(\tau.x);
$$

but $u(\pi'(x)) \neq 0$ and, for $\sigma \in \mathcal{G} - \mathcal{G}^z$, $\sigma.x \in p'$ and hence $\pi'(\sigma.x) = 0$; we conclude that necessarily $\tau \in \mathcal{G}^z$. But as $u$ and $\tilde{\tau}$ have the same value for the primitive element $\pi'(y) = \pi'(x)$ of $k'_s$, they coincide on $k'_s$ and, as $k'$ is a radicial extension of $k'_s$, they coincide on $k'$.

#### Corollary {#ac-v-s2-n2-cor-1 .statement}

*With the hypotheses and notation Of Theorem 2, let $f_1, f_2$ be two homomorphisms of $A$ to a field $L$ with the same restriction to $A$. Then there exists $\sigma \in \mathcal{G}$ such that*

$$
f_2(x) = f_1(\sigma.x)
$$

*for all* $x \in A'$.

Let $p'_i$ be the kernel of $f_i$ ($i = 1, 2$) which is a prime ideal of $A'$; by hypothesis $p'_1 \cap A = p'_2 \cap A$ and this intersection is a prime ideal $p$ of $A$; there therefore exists $\tau \in \mathcal{G}$ such that $\tau.p'_2 = p'_1$ (Theorem 2 (i)); replacing $f_1$ by the homomorphism $x \mapsto f_1(\tau.x)$ we may then assume that $p'_2 = p'_1$ (an ideal which we shall denote by $p'$). By taking the quotient we then derive from $f_1$ and $f_2$ two injective homomorphisms $f'_1, f'_2$ from $A'/p'$ to $L$ which therefore extend to two injective homomorphisms $f''_1, f''_2$ from the field of fractions $k'$ of $A'/p'$ to $L$. As $k'$ is a quasi-Galois extension of $k$, so is $k''_1 = f''_1(k')$ and $k''_2 = f''_2(k')$ (k being identified with a subfield of $L$) and, as there is a k-isomorphism of $k''_1$ onto $k''_2, k''_1 = k''_2$ (*Algebra*, Chapter V, § 6, Proposition 6). Thus $f''_1 \circ {f''_2}^{-1}$ is a k-automorphism of $k'$; by Theorem 2 (ii) it is therefore of the form 6, where $\sigma \in \mathcal{G}^z(p')$. In particular, for all $x \in A'$ the elements $f_2(x)$ and $f_1(\sigma.x)$ are equal.

**Remarks**

(1) Note that under the hypotheses of Theorem 2 $k'$ may be *infinite* over $k$ if $k'$ is not separable over $k$ (Exercise 9).

(2) Clearly $k$ is a *Galois* extension of $k$ if the field $k$ is *perfect*. It is then finite over $k$.

#### Proposition 4 {#ac-v-s2-prop-4 .statement}

*Let $A'$ be a ring, $\mathcal{G}$ a finite group operating on $A'$, $\mathcal{H}$ a subgroup of $\mathcal{G}$, $A$ and $B$ the rings of invariants of $\mathcal{G}$ and $\mathcal{H}$ respectively and $p'$ a prime ideal of $A$; let us write $p = A \cap p'$ and $p(B) = B \cap p'$.

(i) For $\mathcal{H}$ to be contained in the decomposition group $\mathcal{G}^z(p')$, it is necessary and sufficient that $p'$ be the only prime ideal of $A$ lying above $p(B)$.

(ii) *If $\mathcal{H}$ contains $\mathcal{G}^z(p')$, the following conditions are satisfied*:
(a) *The rings $A/p$ and $B/p(B)$ have the same field of fractions*.
(b) *The maximal ideal of the local ring $B_{p(B)}$ is equal to $pB_{p(B)}$*.

(iii) *Suppose further that $A'$ is an integral domain and that $\bigcap_{n \geq 0} p^nA'_p = 0$; then conditions (a) and (b) & (ii) imply that $\mathcal{G}^z(p')$ leaves invariant the elements of $B$*.

(i) It follows from Theorem 2 (i) that the prime ideals of $A$ lying above $p(B)$ are the ideals of the form $\sigma.p'$, where $\sigma \in \mathcal{H}$; whence immediately (i).

(ii) We write $S = A - p$; we know that the rings of invariants of $\mathcal{G}$ and $\mathcal{H}$ in $S^{-1}A'$ are respectively $S^{-1}A$ and $S^{-1}B$ (§ 1, no. 9, Proposition 23) and $\mathcal{G}^{\mathbf{Z}}(S^{-1}p) = \mathcal{G}^{\mathbf{Z}}(p')$ (Lemma 3); finally $S^{-1}p(B) = S^{-1}p' \cap S^{-1}B$ (Chapter II, § 2, no. 4), the local ring of the prime ideal $S^{-1}p(B)$ of the ring $S^{-1}B$ is canonically isomorphic to $B_{p(B)}$ and its residue field is isomorphic to the field of fractions of $B/p(B)$ (Chapter II, § 2, no. 5, Proposition 11). We can therefore show (ii) restricting our attention to the case where $p$ is maximal. To establish (a) it will be sufficient to prove that

$$
B = A + p(B)
$$

for this will show that the fields $A/p$ and $B/p(B)$ are *canonically isomorphic*. By Theorem 2 there is only a finite number of prime ideals of $A'$ lying above $p$ and by Theorem 1 of no. 1 there is at least one prime ideal of $A'$ lying above every prime ideal of $B$; this implies that there is only a *finite* number of prime ideals of $B$ lying above $p$; let $n_j$ ($1 \leq j \leq r$) denote those of these ideals which are $\neq p(B)$. Let $x$ be an element of $B$; as the ideals $p(B)$ and $n_j$ are maximal (no. 1, Proposition 1), there exists $y \in B$ such that $y \equiv x$ (mod. $p(B)$) and $y \in n_j$ for $1 \leq j \leq r$ (Chapter 11, § 1, no. 2, Proposition 5). Let $y_1 = y, y_2, \ldots, y_q$ be distinct elements of the orbit of $y$ under $\mathcal{G}$; clearly

$$
z = y_1 + y_2 + \cdots + y_q \in A,
$$

and to establish (3) it will be sufficient to show that $y_i \in p'$ for $i \geq 2$, for then we shall deduce that $z - y \in p' \cap B = p(B)$, whence $x \in A + p(B)$ since $x \equiv y$ (mod. $p(B)$). Then let $i \geq 2$ and $\sigma \in \mathcal{G}$ such that $\sigma.y = y_i$; we show that $\sigma^{-1}.p'$ does not lie above $p(B)$. For otherwise there would exist $\tau \in \mathcal{H}$ such that $\sigma^{-1}.p' = \tau.p'$ (Theorem 2 (i)), whence $(\tau^{-1}\sigma^{-1}).p' = p'$, in other words $\tau^{-1}\sigma^{-1} \in \mathcal{G}^{\mathbf{Z}} \subset \mathcal{H}$ by hypothesis, whence $\sigma \in \mathcal{H}$; but as $y \in B$ and $\sigma.y \neq y$, this is absurd. We conclude that $\sigma^{-1}.p'$ lies above one of the ideals $n_j$ and, as $y \in n_j$ by construction, certainly $y \in \sigma^{-1}.p'$ or $y_i = \sigma.y \in p'$.

To prove (b) it will suffice to establish that $p(B)$ is contained in the *saturation* $q$ of the ideal $pB$ with respect to $p(B)$ (Chapter II, § 2, no. 4, Proposition 10); as $p(B)$ is contained in none of the $n_j$ ($1 \leq j \leq r$), it will suffice even to prove that

$$
p(B) \subset q \cup n_1 \cup \cdots \cup n_r
$$

by Chapter II, § 1, no. 1, Proposition 2. For this, we consider an element $u \in p(B)$ belonging to none of the $n_j$ ($1 \leq j \leq r$) (Chapter 11, § 1, no. 1, Proposition 2); let $u_1 = u, u_2, \ldots, u_m$ be the distinct elements of the orbit of $u$ under $\mathcal{G}$; we write $w = u_1u_2 \ldots u_m, v = u_2 \ldots u_m$; clearly $w \in A$; on the other hand, if $\tau \in \mathcal{H}$, $\tau.u = u$ and hence necessarily $\tau.u_i \neq u$ for $i \geq 2$, which shows that $\tau.v = v$ and hence $v \in B$. It can be shown as in the proof of (a) that, if $\sigma \in \mathcal{G}$ is such that $\sigma.u = u_i$ where $i \geq 2$, $\sigma^{-1}.p'$ lies above one of the $n_j$ and, as $u \notin n_j$, also $u \notin \sigma^{-1}.p'$, in other words $u_i \notin p'$. We conclude that $v \notin p'$ and therefore $v \notin p(B)$. On the other hand clearly $w \in p' \cap A = p$ and the relation $w = uv$ shows that $u$ is in the saturation of $pB$ with respect to $p(B)$ and hence establishes (4).

(iii) Suppose that $A'$ is an integral domain, that $\bigcap_{n \geq 0} p^n A'_p = 0$ and that conditions (a) and (b) of (ii) hold. With the same notation as in (ii), clearly $S^{-1}A'$ is an integral domain and $S^{-1}A'_p = A'_p$; it is therefore possible to replace $A'$ and $p'$ by $S^{-1}A'$ and $S^{-1}p'$, in other words, suppose also that the ideal $p$ is maximal. The hypotheses (a) and (b) then imply that

$$
\mathbf{B}_{p(B)} = A + p \mathbf{B}_{p(B)}
$$

By induction on $n$ we deduce that $\mathbf{B}_{p(B)} = A + p^n \mathbf{B}_{p(B)}$ for all $n > 0$. Then let $\sigma$ be an element of $\mathcal{G}^\mathbf{Z}$ and $x$ be an element of $B$. For all $n > 0$, there exists $a_n \in A$ such that $x - a_n \in p^n \mathbf{B}_{p(B)} \subset p^n A'_p$; as $\sigma.a_n = a$, and $\sigma.p' = p'$, we deduce that $\sigma.x - x \in p^n A'_p$. Since this relation holds for all $n$, we conclude from the hypothesis that $\sigma.x = x$.

h a r k s

(3) If $A'$ is an integral domain and Noetherian, the condition $\bigcap_{n \geq 1} p^n A'_p = 0$ always holds (Chapter III, § 3, no. 2, Corollary to Proposition 5). It can be shown that this condition is also satisfied if $A'$ is assumed to be an integral domain and $A$ to be Noetherian.

(4) If $p$ is not a maximal ideal of $A$ relation (3) does not necessarily hold under the hypotheses of (ii) and therefore $A/p$ and $B/p(B)$ are not necessarily isomorphic even if we take $\mathcal{H} = \mathcal{G}^\mathbf{Z}$, whence $B = A''$ (Exercise 10).

#### Corollary 1 {#ac-v-s2-prop-4-cor-1 .statement}

Under the hypotheses Of Theorem 2 the rings $A/p$ and $A^\mathbf{Z}/(p' \cap A^\mathbf{Z})$ have the same field Of fractions and the maximal ideal of the local ring $(A^\mathbf{Z})'_{p' \cap A^\mathbf{Z}}$ is generated by $p$.

#### Corollary 2 {#ac-v-s2-prop-4-cor-2 .statement}

Let $A'$ be an integral domain, $\mathcal{G}$ a finite group operating on $A'$, $A'$ the ring of invariants of $\mathcal{G}$ and $p'$ a prime ideal of $A'$; let $K, K^\mathbf{Z}$ and $K$ be the fields of fractions of $A, A^\mathbf{Z}$ and $A'$ respectively. Then $K'$ is a Galois extension Of $K$ and the subfields $L$ of $K$ containing $K$ and such that $p'$ is the only prime ideal of $A'$ lying above the ideal $p' \cap L$ of $A' \cap L$ are just those which contain $K^\mathbf{Z}$.

$\mathcal{G}$ operates on $K'$ and $K$ is the field of invariants of $\mathcal{G}$ in $K'$ (§ 1, no. 9, Proposition 23 applied to $S = A - \{0\}$) and similarly $K^\mathbf{Z}$ is the field of invariants of $\mathcal{G}^\mathbf{Z}$; by definition $K'$ is therefore a Galois extension of $K$. If is the subgroup of $\mathcal{G}$ consisting of those $\sigma \in \mathcal{G}$ leaving invariant the elements of L, to say that L contains $K^{\mathbf{Z}}$ means that $\mathcal{H}$ is contained in $\mathcal{G}^{\mathbf{Z}}$ (Algebra, Chapter V, § 10, no. 5, Theorem 3) and, as L is the field of invariants of $\mathcal{H}$ in $K'$, $A' \cap L$ is the ring of invariants of $\mathcal{H}$ in $A'$; the second assertion then follows from Proposition 4 (i).

#### Definition 4 {#ac-v-s2-def-4 .statement}

*With the hypotheses and notation of Corollary 2 to Proposition 4, a prime ideal $\mathfrak{p}$ of $A$ is said to decompose completely in $K'$ if the number of prime ideals of $A'$ lying above $\mathfrak{p}$ is equal to $[K':K]$.*

It amounts to the same to say that, for a prime ideal $\mathfrak{p}'$ of $A'$ lying over $\mathfrak{p}$, the subgroup $\mathcal{G}^{\mathbf{Z}}(\mathfrak{p}')$ is equal to the subgroup $\mathcal{M}$ leaving invariant all the elements of $A'$, or that $A^{\mathbf{Z}}(\mathfrak{p}') = A'$, or that $\mathcal{G}/\mathcal{M}$ operates faithfully on the set of prime ideals of $A'$ lying above $\mathfrak{p}$.

#### Corollary 3 {#ac-v-s2-def-4-cor-3 .statement}

*Let $A'$ be an integral domain, $\mathcal{G}$ a finite commutative group operating on $A'$, $A$ the ring of invariants of $\mathcal{G}$, $\mathfrak{p}$ a prime ideal of $A$ and $K$ and $K'$ the fields of fractions of $A$ and $A'$ respectively. Then the prime ideals of $A'$ lying above $\mathfrak{p}$ all have the same decomposition ring $A^{\mathbf{Z}}$ and the field of fractions $K^{\mathbf{Z}}$ of $A^{\mathbf{Z}}$ is the greatest intermediate field between $K$ and $K'$ in which $\mathfrak{p}$ decomposes completely.*

If $\mathfrak{p}'$ is a prime ideal of $A'$ lying above $\mathfrak{p}$, then $\mathcal{G}^{\mathbf{Z}}(\sigma.\mathfrak{p}') = \mathcal{G}^{\mathbf{Z}}(\mathfrak{p}')$ since $\mathcal{G}$ is commutative (formula (2)), hence (Theorem 2 (i)) all the prime ideals of $A'$ lying above $\mathfrak{p}$ have the same decomposition group $\mathcal{G}^{\mathbf{Z}}$ and therefore the same decomposition ring $A^{\mathbf{Z}}$; their number is $(\mathcal{G}:\mathcal{G}^{\mathbf{Z}})$. Let L be an intermediate field between K and $K'$ and let $\mathcal{H}$ be the subgroup of $\mathcal{G}$ leaving invariant the elements of L; the decomposition group of $\mathfrak{p}'$ with respect to $\mathcal{H}$ is $\mathcal{G}^{\mathbf{Z}} \cap \mathcal{H}$; as $A' \cap L$ is the ring of invariants of $\mathcal{H}$ in $A'$, the number of prime ideals of $A'$ lying above $\mathfrak{p}' \cap L$ is $(\mathcal{H}:(\mathcal{G}^{\mathbf{Z}} \cap \mathcal{H})) = (\mathcal{H}\mathcal{G}^{\mathbf{Z}}:\mathcal{G}^{\mathbf{Z}})$ (since $\mathcal{G}$ is commutative). The number of prime ideals of $A' \cap L$ lying above $\mathfrak{p}$ is therefore $(\mathcal{G}:\mathcal{H}\mathcal{G}^{\mathbf{Z}})$. For $\mathfrak{p}$ to decompose completely in L, it is necessary and sufficient therefore that $(\mathcal{G}:\mathcal{H}\mathcal{G}^{\mathbf{Z}}) = [L:K] = (\mathcal{G}:\mathcal{H})$ and, as $\mathcal{H} \subset \mathcal{H}\mathcal{G}^{\mathbf{Z}}$, this is equivalent to $\mathcal{H}\mathcal{G}^{\mathbf{Z}} = \mathcal{H}$ or also to $\mathcal{G}^{\mathbf{Z}} \subset \mathcal{H}$ and finally to $L \subset K^{\mathbf{Z}}$.

#### Proposition 5 {#ac-v-s2-prop-5 .statement}

*With the hypotheses and notation of Theorem 2, the field of fractions $k^T$ of $A^T/(\mathfrak{p}' \cap A^T)$ is equal to the greatest separable extension $k'_s$ of $k$ contained in $k'$.*

As in Proposition 4 this may be reduced to the case where $\mathfrak{p}$ is a maximal ideal of $A$, which implies that $\mathfrak{p}'$, $\mathfrak{p}' \cap A^{\mathbf{Z}}$ and $\mathfrak{p}' \cap A^T$ are maximal in $A'$, $A^{\mathbf{Z}}$ and $A^T$ respectively (no. 1, Proposition 1).

For all $x \in A'$, the polynomial $P(X) = \prod_{\sigma \in \mathcal{G}^T} (X - \sigma.x)$ has its coefficients in the inertia ring $A^T$ and, by definition of $\mathcal{G}^T$, all its roots in $A'$ are congruent mod. $\mathfrak{p}'$; the polynomial $\pi'(P)$ over $A^T/(\mathfrak{p}' \cap A^T)$ whose coefficients are the canonical images of those of P under the homomorphism $\pi':A' \to A'/\mathfrak{p}'$ therefore has all its roots in $A'/\mathfrak{p}'$ equal to the image of $x$, which shows that $k'$ is a radicial extension of $k^T$; whence $k'_s \subset k^T$, since every element of $k'_s$ is separable over k and a fortiori over $k^T$.

We know that $k'_s$ is a Galois extension of k (Algebra, Chapter V, § 10, no. 9, Proposition 14) and it follows from Theorem 2 that its Galois group is isomorphic to $\mathcal{G}' = \mathcal{G}^z / \mathcal{G}^T$. As $k^T$ is a radicial extension of $k'_s$, $k^T$ is a quasi-Galois extension of k and the separable factor of the degree of $k^T$ over k is $q = (\mathcal{G}^z : \mathcal{G}^T )$. It remains to see that $k^T$ is a separable extension of k. We have seen above that $\mathcal{G}'$ is identified with an automorphism group of $A^T$ and that $A^z$ is the ring of invariants of $\mathcal{G}'$. If $x \in A^T$, the polynomial $Q(X) = \prod_{\sigma' \in \mathcal{G}'} (X - \sigma'(x))$ therefore has its coefficients in $A^z$; the polynomial over $A^z / (p' \cap A^z)$ whose coefficients are the images of those of Q under $\pi'$ is of degree $q$ and has a root $\pi'(x) \in A^T / (p' \cap A^T )$. As $A^z / (p' \cap A^z) = k$ by Proposition 4 (ii), we see that every element of $k^T$ is of degree $\leq q$ over k.

This being so, let k, be the field of invariants of the group of k-automorphisms of the quasi-Galois extension $k^T$ of $k$; then $[k^T : k_1] = q$ (Algebra, Chapter V, § 10, no. 9, Proposition 14). Let $u$ be a primitive element of $k^T$ over $k_1$; as it is of degree $q$ over k, and of degree $\leq q$ over k, it is of degree $q$ over k and its minimal polynomial over k, has coefficients in $k$; this shows that $u$ is separable over k. On the other hand, for all $v \in k_1$, there exists a power $p'$ of the characteristic exponent p such that $v^{p'} \in k$. We conclude that $k(u - v)$, which contains
$$
(u - v)^{p'} = u^{p'} - v^{p'},
$$
contains $u^{p'}$ and consequently $k(u^{p'})$. But as $u$ is separable over $k$, $k(u) = k(u^{p'})$ (Algebra, Chapter V, § 8, no. 3, Proposition 4), whence $k(u) \subset k(u - v)$. As $u$ is of degree $q$ over k and $u - v$ of degree $\leq q$, it follows that $k(u) = k(u - v)$, whence $v \in k(u)$. This shows that $v$ is separable over k, hence $k_1 = k$ and $k^T$ is separable over $k$.

#### Corollary {#ac-v-s2-n2-cor-2 .statement}

*If the order of the inertia group $\mathcal{G}^T(p')$ is relatively prime to the characteristic exponent p of k, the field $k'$ is a Galois extension of k.*

With the notation of the proof of Proposition 5, the polynomial $\pi'(P)$ has coefficients in $k^T = k'_s$ and all its roots equal to $\pi'(x)$; we immediately deduce that $\pi'(P)$ is a power of a minimal polynomial of $\pi'(x)$ over $k'_s$; but the latter has degree equal to a power of p and hence, as the degree of $\pi'(P)$ is equal to the order of $\mathcal{G}^T$, the hypothesis implies that $\pi'(x) \in k'_s$, in other words $k'_s = k'$.

### 3. DECOMPOSITION AND INERTIA FOR INTEGRALLY CLOSED DOMAINS

#### Lemma 4 {#ac-v-s2-lem-4 .statement}

*Let A be an integrally closed domain, K its field of fractions, p the characteristic exponent of K, K' a radicial extension of K and A' a subring of K' containing A and integral over A. For every prime ideal p of A, there exists a unique prim ideal* p' of $A'$ lying above $p$ and $p'$ is the set of $x \in A'$ such that there exists an integer $m \geq 0$ for which $x^{p^m} \in p$.

The existence of $p'$ follows from no. 1, Theorem 1. If $x \in p'$, there exists $m \geq 0$ such that $x^{p^m} \in K$, whence $x^{p^m} \in A$ since $A$ is integrally closed, hence $x^{p^m} \in p' \cap A = p$. Conversely, if $x \in A'$ is such that $x^{p^m} \in p \subset p'$, then $x \in p$ since $p'$ is prime.

Remark (1). It follows from § 1, no. 3, Corollary to Proposition 11 that the integral closure of $A$ in $K'$ is the set of $x \in K'$ such that there exists $m \geq 0$ for which $x^{p^m} \in A$ (Algebra, Chapter V, § 8, no. 1, Proposition 1).

#### Proposition 6 {#ac-v-s2-prop-6 .statement}

Let $A$ be an integrally closed domain, $K$ its field of fractions, $K'$ a quasi-Galois extension of $K$ and $A'$ the integral closure of $A$ in $K'$. Then:

(i) For every prime ideal $p$ of $A$, the group $\mathcal{G}$ of $K$-automorphisms of $K'$ operates transitively on the set of prime ideals of $A'$ lying over $p$.

(ii) For every prime ideal $p'$ of $A'$, the field of fractions $k'$ of $A'/p'$ is a quasi-Galois extension of the field of fractions $k$ of $A/(A \cap p')$ and the canonical homomorphism $\sigma \mapsto \tilde{\sigma}$ from $\mathcal{G}^Z(p')$ to the group $\Gamma$ of $k$-automorphisms of $k'$ defines, by taking the quotient, a bijection of $\mathcal{G}^Z(p')/\mathcal{G}^T(p')$ onto $\Gamma$.

(A) Suppose first that $K'$ is ajinite Galois extension of $K$. Then $A = A \cap K$ since $A$ is integrally closed and $A$ is therefore the ring of invariants of $\mathcal{G}$ in $A'$. As $\mathcal{G}$ is finite, the proposition follows in this case from no. 2, Theorem 2.

(B) Suppose secondly that $K'$ is any Galois extension of $K$. Then $K'$ is the union of a right directed family $(K_\alpha)_{\alpha \in I}$ of finite Galois extensions of $K$. To show (i), consider two prime ideals $p', q'$ of $A'$ lying above $p$. For all $\alpha \in I$, $p' \cap K_\alpha$ and $q' \cap K_\alpha$ are two prime ideals of $A \cap K_\alpha$, lying above $p$. Since $A' \cap K_\alpha$ is the integral closure of $A$ in $K_\alpha$, and the restrictions to $K_\alpha$ of the elements of $\mathcal{G}$ form the group of $K$-automorphisms of $K$, it follows from case (A) that there exists $\sigma \in \mathcal{G}$ such that $(\sigma.(p' \cap K_\alpha)) = q' \cap K_\alpha$. Let $\mathcal{E}_\alpha$ be the set of $\sigma \in \mathcal{G}$ which have the above property. Let $\sigma \in \mathcal{G} - 8$; then, for all $\tau \in \mathcal{G}$ leaving invariant the elements of $K_\alpha$, (QT) $(\sigma.(p' \cap K_\alpha)) = \varrho.(p' \cap K_\alpha) \neq q' \cap K_\alpha$, and hence $\sigma \tau \in \mathcal{G} - b$. It follows that $\mathcal{E}_\alpha$ is closed in the topological Galois group $\mathcal{G}$ (Algebra, Chapter V, Appendix 11, no. 1) and clearly the family $(\mathcal{E}_\alpha)_{\alpha \in I}$ is left directed. As $\mathcal{G}$ is compact (loc. cit., no. 2, Proposition 3) and the $\mathcal{E}_\alpha$ are non-empty, the intersection $\mathcal{E}$ of the family $(8,)$ is non-empty and $\sigma.p' = q'$ for all $\sigma \in \mathcal{E}$, whence (i).

To show (ii), note that $k'$ is the union of the right directed family $(k_\alpha)_{\alpha \in I}$, where $k_\alpha$ is the field of fractions of $(A' \cap K_\alpha)/(p' \cap K_\alpha)$. As each $k_\alpha$ is a quasi-Galois extension of $k$ by (A), so is $k'$ (Algebra, Chapter V, § 6, no. 3, Proposition 8). On the other hand, let $u$ be a $k$-automorphism of $k'$ and let $\pi': A' \to A'/p'$ be the canonical homomorphism. By virtue of no. 2, Theorem 2 applied to $A' \cap K_\alpha$, there exists for all $\alpha$ a non-empty set $F_\alpha$ of elements $\sigma \in \mathcal{G}$ such that $\sigma.(p' \cap K_\alpha) = p' \cap K_\alpha$ and $u(\pi'(x)) = \pi'(\sigma.x)$ for all $x \in A' \cap K_\alpha$. As above it is seen that $\mathcal{F}_\alpha$ is closed in $\mathcal{G}$ and, as $(\mathcal{F}_\alpha)$ is a left directed set, its intersection $\mathcal{F}$ is non-empty. Clearly for $\alpha \in \mathcal{F}$, $\alpha \in \mathcal{G}^\mathbf{Z}(p')$ and $\tilde{\sigma} = u$, which completes the proof of (ii) in this case.

(C) *General care*. The field of invariants $K_1$ of $\mathcal{G}$ is a radicial extension of $K$ (*Algebra*, Chapter V, § 10, no. 9, Proposition 14); there therefore exists a single prime ideal $p_1$ of $A_1 = A' \cap K_1$ lying above $p$ (Lemma 4). If $p'$ and $q'$ are two prime ideals of $A'$ lying above $p$, then they lie above $p_1$; as $K'$ is a Galois extension of $K$, and $A' \cap K$, is integrally closed (§ 1, no. 2, Proposition 7 and Corollary to Proposition 8), it follows from (B) that there exists $\sigma \in \mathcal{G}$ such that $(1.p' = q'$; whence (i). On the other hand, clearly the field of fractions $k$, of $A_1/p_1$ is a radicial extension of $k$ (A being integrally closed); as $k'$ is a quasi-Galois extension of $k$, by (B), $k'$ is a quasi-Galois extension of $k$, every $k$-isomorphism of $k'$ to an algebraically closed extension of $k'$ being a $k_1$-isomorphism. This last remark shows also, taking account of (B), that every $k$-automorphism of $k'$ is of the form $\tilde{\sigma}$ where $\alpha \in \mathcal{G}^\mathbf{Z}(p')$, which completes the proof of (ii).

*Remark*

(2) Suppose that $K$ is a *Galois* extension of $K$ and let us keep the notation of the proof of Proposition 6; for all $a$ let $\mathcal{G}_a^\mathbf{Z}$ (resp. $\mathcal{G}_a^\mathbf{T}$) be the subgroup of $\mathcal{G}$ consisting of the $\sigma$ whose restriction to $A' \cap K$, belongs to $\mathcal{G}^\mathbf{Z}(p' \cap K_\alpha)$ (resp. $\mathcal{G}^\mathbf{T}(p' \cap K_\alpha)$). The proof of Proposition 6 shows that these subgroups are *closed* in $\mathcal{G}$ and that
$$
\mathcal{G}^\mathbf{Z}(p') = \bigcap_a \mathcal{G}_a^\mathbf{Z} \quad \text{and} \quad \mathcal{G}^\mathbf{T}(p') = \bigcap_a \mathcal{G}_a^\mathbf{T}.
$$
Moreover, the set of restrictions to $A' \cap K$, of the elements of $\mathcal{G}$ (resp. $\mathcal{G}_a^\mathbf{T}$) is the whole of the group $\mathcal{G}^\mathbf{Z}(p' \cap K_\alpha)$ (resp. $\mathcal{G}^\mathbf{T}(p' \cap K_\alpha)$), every $K$-automorphism of $K$, extending to an element of $\mathcal{G}$.

With the same hypotheses, the ring $A^\mathbf{Z}(p')$ (resp. $A^\mathbf{T}(p')$) is the *union* of the directed family of the $A^\mathbf{Z}(p' \cap K_\alpha)$ (resp. $A^\mathbf{T}(p' \cap K_\alpha)$); in fact, every $x \in A^\mathbf{Z}(p')$ (resp. every $x \in A^\mathbf{T}(p')$) belongs to one of the $K$, and by the above there exists a $\beta$ such that $K_\alpha \subset K_\beta$ and the restrictions to $A' \cap K$, of the elements of $\mathcal{G}^\mathbf{Z}(p')$ (resp. $\mathcal{G}^\mathbf{T}(p')$) are the same as the restrictions to $A' \cap K$, of the elements of $\mathcal{G}^\mathbf{Z}(p' \cap K_\beta)$ (resp. $\mathcal{G}^\mathbf{T}(p' \cap K_\beta)$), the groups $\mathcal{G}^\mathbf{Z}(p' \cap K_\alpha)$ and $\mathcal{G}^\mathbf{T}(p' \cap K_\beta)$ being finite; hence $x$ belongs to $A^\mathbf{Z}(p' \cap K_\beta)$ (resp. $A^\mathbf{T}(p' \cap K_\beta)$).

#### Corollary 1 {#ac-v-s2-prop-6-cor-1 .statement}

*Under the hypotheses of Proposition 6, let f be a homomorphism from A to a field L and g_1, g_2 two homomorphisms from A' to L which extend f. Then there exists a K-automorphism $\sigma \in K'$ such that $g_1 = g_2 \circ \sigma$.*

The proof starting from Proposition 6 is the same as that of the Corollary to Theorem 2 starting from the latter.

#### Corollary 2 {#ac-v-s2-prop-6-cor-2 .statement}

*Let A be an integrally closed domain, K its field of fractions, K' a finite algebraic extension of K and A' a subring of K' containing A and integral over A.*

(i) For every prime ideal $\mathfrak{p}$ of $A$ the set of prime ideals of $A'$ lying above $\mathfrak{p}$ is finite.
(ii) If $\mathfrak{p}'$ is a prime ideal of $A'$ lying above $\mathfrak{p}$, every element of $A'/\mathfrak{p}'$ is of degree $\leq [\mathbf{K}':\mathbf{K}]$ over the field of fractions of $A/\mathfrak{p}$.

(i) Let $K''$ be the quasi-Galois extension of $K$ generated by $K'$ in an algebraic closure of $K'$ and $A''$ the integral closure of $A$ in $K''$. The field $K''$ is a finite extension of $K$ (Algebra, Chapter V, § 6, no. 3, Corollary 1 to Proposition 9) and hence its group of $K$-automorphisms is finite; it follows that the set of prime ideals of $A''$ lying above $\mathfrak{p}$ is finite (Proposition 6 (i)). On the other hand, as $A''$ is integral over $A$, the mapping $\mathfrak{p}'' \mapsto \mathfrak{p}'' \cap A'$ of the set of prime ideals of $A''$ lying above $\mathfrak{p}$ to the set of prime ideals of $A'$ lying above $x$ is surjective (no. 1, Theorem 1).

(ii) The coefficients of the minimal polynomial (over $K$) of any element $x' \in A'$ belong to $A$ ($§ 1$, no. 3, Corollary to Proposition 10); applying the canonical homomorphism $\pi': A' \to A'/\mathfrak{p}'$ to the coefficients of this polynomial, an equation of integral dependence with coefficients in $A/\mathfrak{p}$ and of degree $\leq [\mathbf{K}':\mathbf{K}]$ is obtained for the class mod. $\mathfrak{p}'$ of $x$; whence the conclusion.

#### Corollary 3 {#ac-v-s2-prop-6-cor-3 .statement}

With the hypotheses and notation of Corollary 2, if $A$ is semi-local, so is $A'$.

For every maximal ideal $m'$ of $A'$, $m' \cap A$ is a maximal ideal of $A$ (no. 1, Proposition 1); the corollary then follows from Corollary 2, since by hypothesis the set of maximal ideals of $A$ is finite.

#### Corollary 4 {#ac-v-s2-prop-6-cor-4 .statement}

Let $A$ be an integrally closed domain, $K$ its field of fractions, $K$ a Galois extension of $K$, $A'$ the integral closure of $A$ in $K'$, $\mathfrak{p}'$ a prime ideal of $A$, $\mathfrak{p} = A \cap \mathfrak{p}'$ and $k$ and $k'$ the fields of fractions of $A/\mathfrak{p}$ and $A'/\mathfrak{p}'$ respectively. Then:

(i) The field of fractions of $A^{\mathbf{Z}}/(\mathfrak{p}' \cap A^{\mathbf{Z}})$ is equal to $k$ and the maximal ideal of the local ring of $A^{\mathbf{Z}}$ relative to $\mathfrak{p}' \cap A^{\mathbf{Z}}$ is generated by $\mathfrak{p}$.

(ii) The field of fractions $k^T$ of $A^T/(\mathfrak{p}' \cap A^T)$ is the greatest separable extension of $k$ contained in $k'$.

The ring $A$ is the ring of invariants in $A'$ of the Galois group of $K'$ over $K$; if $K'$ is of finite degree over $K$, the corollary then follows from Propositions 4 and 5 of no. 2. Consider now the general case, $K'$ therefore being the union of a right directed set $(K_i)$ of finite Galois extensions of $K$. Then:

(i) If $x, y$ are two elements of $A^{\mathbf{Z}}$, where $y \notin \mathfrak{p}'$, there is an index $\alpha$ such that $x$ and $y$ belong to $A^{\mathbf{Z}}(\mathfrak{p}' \cap K_{\alpha})$ (Remark 2); by Proposition 4 of no. 2, there are $x_0, y_0$ in $A$ with $y_0 \notin \mathfrak{p}'$ such that $xy_0 - x_0y \in \mathfrak{p}'$, which proves the first assertion of (i); if further $x \in \mathfrak{p}'$, we may assume that $y_0$ satisfies
$$
xy_0 \in \mathfrak{p}A^{\mathbf{Z}}(\mathfrak{p}' \cap K_{\alpha}) \subset \mathfrak{p}A^{\mathbf{Z}}(\mathfrak{p}'),
$$
which proves the second assertion of (i).

(ii) Suppose now that $x \in A^T$; there exists $\alpha$ such that $x \in A^T(p' \cap K,)$ (Remark 2) and Proposition 5 of no. 2 shows that the class $\bar{x}$ of $x \mod.(p' \cap K, \cap A^T)$ is algebraic and separable over $k$; *a fortiori* the class $\mod.(p' \cap A^T)$ of $x$ is separable over $k$; to complete the proof of the corollary, it is sufficient to show that $k'$ is a *radicial* extension of $k^T$. Now, $k'$ is the union of the right directed family of fields of fractions $k_\alpha$ of the rings $(A' \cap K_\alpha)/(p' \cap K,)$. It follows therefore from Proposition 5 that, if an element of $k'$ belongs to $k$, it is radicial over the field of fractions of

$$
A^T(p' \cap K_\alpha)/(p' \cap A^T(p' \cap K_\alpha))
$$

and *a fortiori* over $k^T$ (by virtue of Remark 2).

#### Definition 5 {#ac-v-s2-def-5 .statement}

*With the hypotheses and notation of Proposition 6, the field of invariants $K^Z(p')$ (resp. $K^T(p')$) of the group $G^Z(p')$ (resp. $G^T(p')$) in the field $K'$ is called the decomposition field* (resp. *inertia field*) *of $p'$ with respect to $K$*.

We also write $K^Z$ (resp. $K^T$) in place of $K^Z(p')$ (resp. $K^T(p')$). It follows from § 1, no. 9, Proposition 23 that $K^Z$ (resp. $K^T$) is the field *of fractions* of the ring $A^Z$ (resp. $A^T$); $A^Z$ (resp. $A^T$) is the integral closure of $A$ in $K^Z$ (resp. $K^T$).

*Remarks*

(3) Under the conditions of Corollary 4 of Proposition 6 and assuming that $[K':K]$ is *finite*, the number of distinct prime ideals lying above $p$ is $[K^Z:K]$, this degree being equal to the index ('3:*G*Z*) by Galois theory; moreover, it follows from Galois theory that

$$(6)$$
$$
[K^T:K^Z] = (G^Z:G^T) = [k^T:k].
$$

(4) Let $A$ be an integrally closed domain, $K$ its field of fractions, $K'$ a *finite* algebraic extension of $K$ and $A'$ the integral closure of $A$ in $K'$. Then, for every prime ideal $p$ of $A$, *the number* $\&$ *prime ideals* $\&$ *of* $A'$ *lying above* $p$ *is at most* $[K':K]_s$ (the separable factor of the degree of $K$ over $K$). We may first restrict our attention to the case where $K$ is a separable extension of $K$, for in general $K$ is a radicial extension of the greatest separable extension $K_0$ of $K$ contained in $K'$, $[K':K]_s = [K_0:K]$ by definition and, if $A$, is the integral closure of $A$ in $K_0$, the prime ideals of $A$, and $A'$ are in one-to-one correspondence (Lemma 4). Suppose therefore that $K$ is separable over $K$ and let $N$ be the Galois extension of $K$ generated by $K$ in an algebraic closure of $K$, $G$ its Galois group, $B$ the integral closure of $A$ in $N$ and $\mathfrak{P}$ a prime ideal of $B$ lying above $p$. Let $\mathcal{H}$ be the Galois group of $N$ over $K$ and $G^Z$ the decomposition group of $\mathfrak{P}$; the prime ideals of $B$ lying above $p$ are the $s.\mathfrak{P}$ where $s \in G$ (no. 2, Theorem 2) and the relation $s.\mathfrak{P} = s'.\mathfrak{P}$ means that $s' = sg$ where $g \in G^Z$. On the other hand in order that $s.\mathfrak{P} \cap K' = s'.\mathfrak{P} \cap K'$, it is necessary and sufficient that $s'.\mathfrak{P} = ts.\mathfrak{P}$, where $t \in \mathcal{H}$ (no. 2, Theorem 2), whence finally $s' = tsg$ where $t \in \mathcal{H}$ and $g \in G^Z$. The number of prime ideals of $A'$ lying above $p$ is therefore equal to the *number of classes of $G$ under the equivalence relation* "there exists $t \in \mathcal{H}$ and $g \in G^{\mathbf{Z}}$ such that $s' = tsg$" between $s$ and $s'$; clearly this number is at most equal to the index $(G : \mathcal{H})$, the number of right cosets of $\mathcal{H}$ in $G$, and $(G : \mathcal{H}) = [K' : K]$ by Galois theory.

#### Proposition 7 {#ac-v-s2-prop-7 .statement}

*Let $A$ be an integrally closed domain, $K$ its field of fractions, $K'$ a Galois extension of $K$, $\mathcal{G}$ its Galois group, $A'$ the integral closure of $A$ in $K'$, $p'$ a prime ideal of $A'$ and $p = A \cap p'$. Finally, let $L$ be a subfield of $K'$ containing $K$ and let $p(L) = p' \cap L$.

(i) *The decomposition field* (resp. *inertia field*) *of $p'$ with respect to $L$ is $L(K^{\mathbf{Z}})$ (resp. $L(K^T)$); *if further $L$ is a Galois extension of $K$, the decomposition field of $p(L)$ with respect to $K$ is $L \cap K^{\mathbf{Z}}$.

(ii) *If $L$ is contained in $K^{\mathbf{Z}}$, $A/p$ and $(A' \cap L)/p(L)$ have the same field of fractions and in the local ring $A' \cap L$ corresponding to the prime ideal $p(L)$, the maximal ideal is generated by $p$. Conversely, if these two conditions hold and further $\bigcap_{n > 0} p^n A'_p = 0$, $L$ is contained in $K^{\mathbf{Z}}$.

(i) If $\mathcal{H}$ is the subgroup of $\mathcal{G}$ leaving invariant the elements of $L$, clearly the decomposition group (resp. inertia group) of $p'$ with respect to $L$ is $G^{\mathbf{Z}} \cap \mathcal{H}$ (resp. $G^T \cap \mathcal{H}$) and the first assertion follows from Galois theory if $K'$ is a *finite* Galois extension of $K$ (*Algebra*, Chapter V, § 10, no. 6, Corollary 1 to Theorem 3); in the general case it follows from the fact that $A^{\mathbf{Z}}$ (resp. $A^T$) is the union of the $A^{\mathbf{Z}}(p' \cap K_\alpha)$ (resp. $A^T(p' \cap K_\beta)$) in the notation of *Remark 2*: every element $x \in K'$ belongs to some $K$, and if it is invariant under $G^{\mathbf{Z}}(p') \cap \mathcal{H}$ (resp. $G^T(p') \cap \mathcal{H}$) it is also invariant under $G^{\mathbf{Z}}(p' \cap K_{\beta'}) \cap \mathcal{H}$ (resp. $G^T(p' \cap K_{\beta'}) \cap \mathcal{H}$) for some suitable $\beta'$; hence it belongs by the beginning of the argument to

$$
L(K^{\mathbf{Z}}(p' \cap K_{\alpha})) \subset L(K^{\mathbf{Z}}) \quad (\text{resp. } L(K^T(p' \cap K_{\beta})) \subset L(K^T)).
$$

Suppose now that $L$ is a Galois extension of $K$; the restriction to $L$ of every $\sigma \in G^{\mathbf{Z}}$ then leaves invariant $p(L) = p' \cap L$ and hence belongs to the decomposition group of $p(L)$ with respect to $K$. Conversely, let $\tau$ be an automorphism of $L$ belonging to this group and let $\sigma$ be an extension of $\tau$ to a $K$-automorphism of $K'$; we write $q' = \sigma.p'$. As $p'$ and $q'$ both lie above $p(L)$, there exists an automorphism $\rho \in \mathcal{H}$ such that $q' = \rho.p'$, whence $\rho^{-1}\sigma \in G^{\mathbf{Z}}$ and $\tau$ is the restriction of $\rho^{-1}\sigma$ to $L$; in other words, the decomposition group of $p(L)$ with respect to $K$ is identical with the group of restrictions to $L$ of the automorphisms $\sigma \in G^{\mathbf{Z}}$, which proves the second assertion.

(ii) To say that $L \subset K^{\mathbf{Z}}$ means that $\mathcal{H} \supset G^{\mathbf{Z}}$ and the assertions of (ii) are therefore special cases of no. 2, Proposition 4 (ii) and (iii) when $[K':K]$ is finite. In the general case the argument is as in the proof of Proposition 6.

### 4. THE SECOND EXISTENCE THEOREM

#### Theorem 3 {#ac-v-s2-thm-3 .statement}

Let $A$ be an integrally closed domain and $A'$ a ring containing $A$ and integral over $A$. Suppose that $0$ is the only element of $A$ which is a divisor of $0$ in $A'$. Let $p, q$ be two prime ideals of $A$ such that $q \supset p$ and $q'$ a prime ideal of $A$ lying above $q$. Then there exists a prime ideal $p'$ of $A$ lying above $p$ and such that $q' \supset p'$.

Suppose first that $A'$ is an integral domain. Let $K, K'$ be the fields of fractions of $A$ and $A'$ respectively; let $K''$ be the algebraic closure of $K$ and $A$ the integral closure of $A$ in $K''$; then $A \subset A' \subset A''$. Let $p''$ be a prime ideal of $A''$ lying above $p$ (no. 1, Theorem 1), $q''$ a prime ideal of $A''$ lying above $q$ and such that $p'' \subset q''$ (no. 1, Corollary 2 to Theorem 1) and finally $q_1''$ a prime ideal of $A''$ lying above $q'$ (no. 1, Theorem 1). By no. 3, Proposition 6 (i), there exists a $K$-automorphism $\sigma$ of $K''$ such that $Q.q'' = q_1''$. Then $Q.p''$ is a prime ideal of $A''$ lying above $p$ such that $Q.p'' = q_1''$ and hence $p' = A' \cap \sigma.p''$ is a prime ideal of $A'$ lying above $p$ and contained in $A' \cap q_1'' = q'$.

We pass to the general case. As $A$ is an integral domain and $q'$ is prime, the subsets $A - \{0\}$ and $A' - q'$ of $A'$ are multiplicative; then their product $S = (A - \{0\})(A' - q')$ is a multiplicative subset of $A'$ which does not contain 0 since the non-zero elements of $A$ are not divisors of 0 in $A'$. Then there exists (Chapter II, §2, no. 5, Corollary 2 to Proposition 11) a prime ideal $m'$ of $A'$ disjoint from $S$, in other words such that $m' \subset q'$ and $m' \cap A = 0$. Let $h$ be the canonical homomorphism $A' \to A'/m'$. The restriction of $h$ to $A$ is injective and hence $h(A)$ is integrally closed. As $m' \subset q'$, $h(q')$ is a prime ideal of $A'/m'$ lying above $h(q)$; since $A'/m'$ is an integral domain, the first part of the proof proves that there exists a prime ideal $n'$ of $A'/m'$ such that $n' \cap h(A) = h(p)$ and $h(q') \supset n'$. The ideal $p' = h^{-1}(n')$ is a prime ideal of $A'$ and $q' \supset p'$, since $q'$ contains the kernel of $h$. As $n' \supset h(p)$, $p' \supset p$. Finally, for $x \in p' \cap A$, $h(x) \in n' \cap h(A) = h(p)$ and hence $x \in p$ since the restriction of $h$ to $A$ is injective; hence $p' \cap A = p$.

#### Corollary {#ac-v-s2-n4-cor-1 .statement}

Under the hypotheses on $A$ and $A'$ of Theorem 3, let $p$ be a prime ideal of $A$. The prime ideals of $A'$ lying above $p$ are the minimal elements of the set $\mathcal{E}$ of prime ideals of $A'$ containing $pA'$.

A prime ideal of $A'$ lying above $p$ is minimal in $\mathcal{E}$ by virtue of no. 1, Corollary 1 to Proposition 1. Conversely, let $q'$ be a minimal element of $\mathcal{E}$. As $q' \cap A \supset p$, Theorem 3 shows that there exists a prime ideal $p'$ of $A'$ lying above $p$ such that $q' \supset p'$. As $p'$ contains $pA'$, the hypothesis made on $q'$ implies that $q' = p'$ and hence $q'$ lies above $p$.

\* Let $V, V'$ be two affine algebraic varieties and $f$ a morphism of $V'$ to $V$ such that $f(V')$ is dense in $V$. Let $A$ (resp. $A'$) be the ring of functions regular on $V$ (resp. $V'$); having been given $f$ we can identify $A$ with a sub-ring of $A'$; suppose that $A'$ is integral over $A$. Theorem 1 of no. 1 shows that for every irreducible subvariety W of V there exists an irreducible subvariety W' of V' such that f(W') is a dense subset of W; in particular, every point of V is the image of an irreducible subvariety of V', which shows that f is surjective. Similarly, the restriction of f to every irreducible subvariety W' of V' maps W' onto an irreducible subvariety of V. Corollary 2 to Theorem 1, no. 1 shows that, if W and X are two irreducible subvarieties of V such that W ⊃ X and if W' is an irreducible subvariety of V' such that f(W') = W, then there exists an irreducible subvariety X' of V' contained in W' and such that f(X') = X.

If A is integrally closed, V is called normal. Theorem 3 shows that, if V is normal, if W and X are irreducible subvarieties of V such that W ⊃ X and if X' is an irreducible subvariety of V' such that f(X') = X, then there exists a subvariety W' of V' containing X' and such that f(W') = W. Finally, the Corollary to Theorem 3 shows that, if V is normal and W is an irreducible subvariety of V, the irreducible subvarieties W' of V' such that f(W') = W are just the irreducible components of $\overline{f}(W)$.

### Exercises {#ac-v-s2-exercises}

See the [exercises for § 2](exercises/s2/).
