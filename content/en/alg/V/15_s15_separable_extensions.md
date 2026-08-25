---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 15
section_title: Separable extensions
lang: en
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A V.118-A V.126, A V.175-A V.177
pdf_pages: 0232-0240, 0289-0291
extraction: ocr
subsections:
    - "no": 1
      title: Characterization of the nilpotent elements of a ring
      page: 118
      pdf_page: 232
    - "no": 2
      title: Separable algebras
      page: 119
      pdf_page: 233
    - "no": 3
      title: Separable extensions
      page: 121
      pdf_page: 235
    - "no": 4
      title: Mac Lane's separability criterion
      page: 122
      pdf_page: 236
    - "no": 5
      title: Extensions of a perfect field
      page: 125
      pdf_page: 239
    - "no": 6
      title: The characterization of separability by automorphisms
      page: 125
      pdf_page: 239
statements: 21
exercises: 12
content_sha256: 6e23f56602ad2acdd225f6676142a1a51ca45a73e6a8b8edcd197f9955bb9d4a
---

## § 15. SEPARABLE EXTENSIONS

### 1. Characterization of the nilpotent elements of a ring

#### Proposition 1 {#alg-v-s15-prop-1 .statement}

— *Let A be a commutative ring and x an element of A. For x to be nilpotent it is necessary and sufficient that $1 - xT$ be invertible in the ring $A[T]$.*

We note that $A[T]$ is a subring of the formal power series ring $A[[T]]$ and that $1 - xT$ has in $A[[T]]$ the inverse $\sum_{n=0}^{\infty} x^n T^n$ (IV, p. 30, Prop. 5). For $1 - xT$ to be invertible in $A[T]$ it is necessary and sufficient for $\sum_{n=0}^{\infty} x^n T^n$ to be a polynomial, that is, for x to be nilpotent.

#### Proposition 2 {#alg-v-s15-prop-2 .statement}

— *Let A be a commutative ring. The set of nilpotent elements of A is an ideal of A equal to the intersection of the set of all prime ideals of A.*

Let x be a nilpotent element of A and p a prime ideal of A. The residue class of $x \mod p$ is a nilpotent element of the integral domain $A/p$, hence is zero; thus we have $x \in p$.

Let x be a non-nilpotent element of A. By Prop. 1 the principal ideal $(1 - xT)$ of $A[T]$ is distinct from $A[T]$. By Krull's theorem (I, p. 104) there exists a maximal ideal m of $A[T]$ containing $1 - xT$. Then m is a prime ideal of $A[T]$, hence $p = A \cap m$ is a prime ideal of A. We have $1 \notin m$ and $1 - Tx \in m$, hence $Tx \notin m$ and *a fortiori* $x \notin p$.

We have thus shown that the set $\mathfrak{n}$ of nilpotent elements of A is the intersection of the set of all prime ideals of A; since every intersection of ideals is an ideal, $\mathfrak{n}$ is an ideal.

#### Corollary {#alg-v-s15-n1-cor-1 .statement}

— *For a commutative ring to be reduced* (*V*, p. 34, Def. 2) *it is necessary and sufficient for it to be isomorphic to a subring of a product of fields*.

The condition is clearly sufficient.

Let $\mathbf{A}$ be reduced. By Prop. 2 the intersection $n$ of the set of prime ideals of $\mathbf{A}$ is reduced to 0. For every prime ideal $\mathfrak{p}$ of $\mathbf{A}$, let $k(\mathfrak{p})$ be the field of fractions of $\mathbf{A}/\mathfrak{p}$ and $\varphi_n$ the canonical homomorphism of $\mathbf{A}$ into $k(\mathfrak{p})$. Let $\varphi$ be the homomorphism of $\mathbf{A}$ into $\prod_{\mathfrak{p}} k(\mathfrak{p})$ whose component of index $\mathfrak{p}$ is $\varphi_{\mathfrak{p}}$. The kernel of $\varphi_{\mathfrak{p}}$ is $\mathfrak{p}$, hence that of $\varphi$ is $n = 0$; therefore $\varphi$ is an isomorphism of $\mathbf{A}$ onto a subring of $\prod_{\mathfrak{p}} k(\mathfrak{p})$.

### 2. Separable algebras

#### Definition 1 {#alg-v-s15-def-1 .statement}

*Let $\mathbf{A}$ be a commutative algebra over a field $K$. Then $A$ is said to be separable over $K$, or also a separable $K$-algebra if the ring $L \otimes_K \mathbf{A}$ is reduced for every extension $L$ of $K$*.

Every separable algebra is clearly reduced. For a partial converse see Th. 3 (*V*, p. 125).

*Examples. — 1*) Let $\mathbf{A}$ be a polynomial algebra $K[X_i]_{i \in I}$. For every extension $L$ of $K$ the ring $L \otimes_K \mathbf{A}$ is isomorphic to $L[X_i]_{i \in I}$ (III, p. 449, Remark 2) and hence is an integral domain (*IV*, p. 9, Prop. 8). In other words, every polynomial algebra over a field $K$ is a separable $K$-algebra.

2) Let $\mathbf{A}$ be a commutative algebra of finite degree over a field $K$. For $\mathbf{A}$ to be separable it is necessary and sufficient for it to be etale (*V*, p. 34, Th. 4).

3) Let $E$ be an algebraic extension of a field $K$. If $L$ is an extension of $K$, then the ring $L \otimes_K E$ is a union of the subrings $L \otimes_K F$ where $F$ ranges over the set of all subextensions of finite degree of $E$; therefore the ring $L \otimes_K E$ is reduced if and only if this is true of $L \otimes_K F$ for every subextension $F$ of $E$, of finite degree over $K$. Taking Example 2 into account we see that $E$ is a separable algebra in the sense of the above Def. 1 if and only if it is a separable algebraic extension in the sense of Def. 1 of *V*, p. 36.

#### Proposition 3 {#alg-v-s15-prop-3 .statement}

*Let $K$ be a field*.

a) *Every subalgebra of a separable $K$-algebra is separable*.

b) *Every direct limit of separable $K$-algebras is separable*.

c) *Every product of separable $K$-algebras is separable*.

d) *Let $\mathbf{A}$ be a $K$-algebra and $K'$ an extension of $K$. For $\mathbf{A}$ to be separable it is necessary and sufficient for the $K'$-algebra $\mathbf{A}_{(K')}$ obtained from $\mathbf{A}$ by extension of scalars to be separable*.

Let $L$ be an extension of $K$. Let $\mathbf{A}$ be a separable algebra over $K$ and $B$ a subalgebra of $\mathbf{A}$; then the ring $L \otimes_K \mathbf{A}$ is reduced, and $L \otimes_K B$ is isomorphic to a subring of $L \otimes_K \mathbf{A}$, hence is reduced. Thus $B$ is separable and *a)* is proved. *In the* same way $b$) may be proved, using the canonical isomorphism of $L \otimes_K \varprojlim A_i$ with $\varprojlim L \otimes_K A_i$ (II, p. 290, Prop. 7) and $c$) is proved by remarking that $L \otimes_K \left( \prod_{i \in I} A_i \right)$ is isomorphic to a subring of $\prod_{i \in I} (L \otimes_K A_i)$ (II, p. 306, Prop. 15).

We shall use the notation of $d$). For every extension $L'$ of $K'$ the rings $L' \otimes_{K'} A_{(K')}$ and $L' \otimes_K A$ are isomorphic (II, p. 278, Prop. 2). We conclude that if $A$ is a separable $K$-algebra, then $A_{(K')}$ is a separable $K'$-algebra. Conversely suppose that $A_{(K')}$ is a separable $K'$-algebra ; the preceding remark shows that $L' \otimes_K A$ is reduced for every extension $L'$ of $K$ containing $K'$ as subextension. Let $L$ be an extension of $K$; by the Scholium (V, p. 13) there exists an extension $L'$ of $K$ containing $K'$ as a subextension and a $K$-homomorphism of $L$ into $L'$; the ring $L \otimes_K A$ is thus isomorphic to a subring of $L' \otimes_K A$ and hence reduced. This proves that $A$ is a separable $K$-algebra.

#### Proposition 4 {#alg-v-s15-prop-4 .statement}

— *Let $A$ be a separable algebra over a field $K$ and let $B$ be the total ring of fractions of $A$; then the $K$-algebra $B$ is separable.*

Let $S$ be the set of cancellable elements of $A$. We have identified $A$ with a subring of $B$ (I, p. 113); further, every element of $S$ is invertible in $B$ and every element of $B$ has the form $a s^{-1}$ with $a \in A$ and $s \in S$. Let $L$ be an extension of $K$ and $x$ a nilpotent element of $L \otimes_K B$. Then $x$ may be written in the form
$$
x = \sum_{i=1}^n y_i \otimes a_i s_i^{-1}
$$
with $y_i \in L, a_i \in A, s_i \in S$ for $1 \leq i \leq n$. If we put $s = s_1 \ldots s_n$
then $x(1 \otimes s)$ belongs to the subring $L \otimes_K A$ of $L \otimes_K B$; since $x(1 \otimes s)$ is nilpotent and $A$ separable over $K$, we have $x(1 \otimes s) = 0$, and since $s$ is invertible in $B$ we find that $x = 0$. This proves the ring $L \otimes_K B$ to be reduced, whence the proposition.

#### Proposition 5 {#alg-v-s15-prop-5 .statement}

— *Let $K$ be a field and $A, B$ commutative $K$-algebras. If $A$ is reduced and $B$ separable then $A \otimes_K B$ is reduced.*

By the Cor. of Prop. 2 (V, p. 119) $A$ is isomorphic to a subalgebra of a product $\prod_{i \in I} L_i$ where $L_i$ is an extension of $K$ for $i \in I$. Therefore $A \otimes_K B$ is isomorphic to a subring of $\left( \prod_{i \in I} L_i \right) \otimes_K B$ and this latter ring is isomorphic to a subring of $\prod_{i \in I} (L_i \otimes_K B)$ (II, p. 306, Prop. 15). Since $B$ is separable, each of the rings $L_i \otimes_K B$ is reduced, and so the same is true of $\prod_{i \in I} (L_i \otimes_K B)$, and *a fortiori* of $A \otimes_K B$.

#### Corollary 1 {#alg-v-s15-prop-5-cor-1 .statement}

— *Let $K$ be a field, $L$ a separable extension of $K$ and $f$ a polynomial in $K[X]$. If $f$ has no multiple factors in $K[X]$, it has also no multiple factors in $L[X]$.*

If $f$ has no multiple factor in $K[X]$, the quotient ring $K[X]/(f)$ is reduced; for $f$ is a product of irreducible polynomials $f_i$ relatively prime in pairs, hence

K[X]/(f) is isomorphic, by I, p. 110, Prop. 9, to the product of fields K[X]/(f_i). By Prop. 5 the ring L[X]/(f), being isomorphic to L ⊗_K K[X]/(f ), is reduced; if g is a non-constant polynomial of L[X] such that g^2 divides f, then the residue class of fg^{-1} in L[X]/(f) is a non-zero nilpotent element; hence f has no multiple factors in L[X].

#### Corollary 2 {#alg-v-s15-prop-5-cor-2 .statement}

— Let A and B be two commutative K-algebras. *If* A and B are separable, the same is true of A ⊗_K B.

Let L be an extension of K. The ring L ⊗_K A is reduced because A is separable; now Prop. 5 shows the ring (L ⊗_K A) ⊗_K B (isomorphic to L ⊗_K (A ⊗_K B)) to be reduced, whence the Corollary.

### 3. Separable extensions

Let K be a field. Since any extension of K is a K-algebra, the notion of separability introduced in Def. 1 (V, p. 119) applies in particular to the case of extensions of K. By example 3 (V, p. 119) that definition of separability agrees in the case of algebraic extensions with that of § 7 (V, p. 36, Def. 1).

#### Proposition 6 {#alg-v-s15-prop-6 .statement}

— Every pure extension of a *field* K is separable.
This follows at once from Example 1 (V, p. 119) and Prop. 4 (V, p. 120).

#### Proposition 7 {#alg-v-s15-prop-7 .statement}

— Let E be a field, G a group of *automorphisms* of E and K the *subfield* of E consisting of the invariants of G. Then E is a separable extension of K.

Let L be an extension of K; there exists an algebraically closed extension Ω of L whose transcendence degree over K is at least equal to that of E over K. By Cor. 1 (V, p. 117) there exists a K-homomorphism u of E into R. We denote by v the Ω-algebra homomorphism of A = Ω ⊗_K E into Ω which maps λ ⊗ x to λ . u(x) for λ ∈ Ω and x ∈ Ω; we write a for the kernel of v.

For every s ∈ G let h_s be the automorphism Id, ⊗ s of the 0-algebra A; the kernel of the homomorphism v ∘ h_s of A into Ω is the prime ideal a_s = h_s^{-1}(a) of A. It is clear that the ideal b = ⋂_{s ∈ G} a_s of A is stable under the automorphisms h_s. Therefore (V, p. 63, Cor.) the ideal b is of the form c ⊗_K E, where c is an ideal of Ω. Now b ⊂ a ≠ A, and so c ≠ Ω; since Ω is a field, we have c = 0, hence b = 0.

The family (a_s), _s ∈ G of prime ideals of A thus has zero intersection. By Prop. 2 (V, p. 118) the ring is reduced, and a fortiori the same holds of the subring L ⊗_K E of A. Since L was an arbitrary extension of K, this proves that E is separable over K.

#### Proposition 8 {#alg-v-s15-prop-8 .statement}

— Let L be an extension of a field K. If L is separable over K, every subextension of L is separable over K. Conversely, if every finitely generated subextension of L is separable over K, then L is separable over K.

This follows at once from Prop. 3, a) and b) (V, p. 119).

Thus separability may be called a property of « finite character ».

#### Proposition 9 {#alg-v-s15-prop-9 .statement}

— Let L be an extension of a field K and M a commutative L-algebra (for example, an extension of L). If M is separable over L and L is separable over K, then M is separable over K.

Let K' be an extension of K. Since L is a separable extension of K, the ring $K' \otimes_K L$ is reduced; since M is a separable L-algebra, Prop. 5 (V, p. 120) shows the ring $(K' \otimes_K L) \otimes_L M$ to be reduced. Now the ring $K' \otimes_K M$ is isomorphic to $(K' \otimes_K L) \otimes_L M$ (II, p. 278, Prop. 2), hence is reduced. This proves that M is separable over K.

If the extension M is separable over K, it is not necessarily separable over L (cf. however V, p. 124, Cor. 3). For example, if p is a prime number, the field $F_p(X)$ of rational fractions in one indeterminate X over $F_p$ is separable over $F_p$ (V, p. 121, Prop. 6) but it is a p-radical algebraic extension of $F_p(X^p)$; in particular $F_p(X)$ is not separable over $F_p(X^p)$.

Later (V, p. 137 Prop. 5) we shall study the separability of composite extensions.

### 4. Mac Lane's separability criterion

#### Theorem 1 {#alg-v-s15-thm-1 .statement}

— Let K be a field of characteristic 0. Every reduced K-algebra and in particular every extension of K is separable over K.

We first show that every extension L of K is separable. Let B be a transcendence basis of L over K (V, p. 109, Th. 1) and let $L_1 = K(B)$. Then $L_1$ is separable over K (V, p. 121, Prop. 6). Further, L is an algebraic extension of $L_1$ and $L_1$ is a field of characteristic 0; therefore L is separable over $L_1$ (V, p. 37, Cor.). By Prop. 9, L is thus separable over K.

Now let A be a reduced algebra over the field K. By the Cor. of Prop. 2 (V, p. 119) there exists a family $(L_i)_{i \in I}$ of extensions of K such that A is isomorphic to a subalgebra of $\prod_{i \in I} L_i$. Each of the algebras $L_i$ is separable over K by what has been said and so A has the same property, by Prop. 3 a) and c) (V, p. 119).

#### Theorem 2 {#alg-v-s15-thm-2 .statement}

— Let K be a field of characteristic $p \neq 0$, $K^{p^{-\infty}}$ a perfect closure of K and A a commutative K-algebra. The following properties are equivalent:
a) A is separable.
b) There exists an extension K' of K such that K' is perfect and $K' \otimes_K A$ is reduced.
c) The ring $K^{p^{-\infty}} \otimes_K A$ is reduced.

d) *The ring* $K' \otimes_K A$ *is reduced for every extension* $K'$ *of* $K$ *which is of finite degree and* $p$*-radical of height* $\leqslant 1$.

e) *For every family* $(a_i)_{i \in I}$, *of elements of* $A$ *linearly free over* $K$, *the family* $(a_i^p)_{i \in I}$, *is linearly free over* $K$.

f) *There exists a basis* $(a_i)_{i \in I}$, *of the vector* $K$*-space* $A$ *suck that the family* $(a_i^p)_{i \in I}$, *is linearly free over* $K$.

If an extension $K'$ of $K$ is a perfect field, it contains a subextension $K$-isomorphic to $K^{p^{-\infty}}$ ($V$, p. 6, Prop. 3); moreover, every $p$-radical extension of $K$ is isomorphic to a subextension of $K^{p^{-\infty}}$ ($V$, p. 26, Prop. 3). These remarks show the implications $a) \Rightarrow b) \Rightarrow c) \Rightarrow d)$.

Let us prove that $d)$ implies $e)$. Let $(a_i)_{i \in I}$, be a linearly free family in $A$ and let $(A_i)_{i \in I}$, be a family of finite support in $K$ such that $\sum \lambda_i a_i^p = 0$. Let $K'$ be the subextension of $K^{p^{-\infty}}$ generated by the elements $\lambda_i^{p^{-1}}$; it is of finite degree and height $\leqslant 1$. Put $x = \sum_{i \in I} \lambda_i^{p^{-1}} \otimes a_i$ in $K' \otimes_K A$; we have

$$
x^p = \sum_{i \in I} \lambda_i \otimes a_i^p = 1 \otimes \sum_{i \in I} \lambda_i a_i^p = 0
$$

By the hypothesis $d)$ we have $x = 0$, whence $A_i = 0$ for all $i \in I$.

Clearly $e)$ implies $f)$ and it remains to show that $f)$ implies $a)$. Thus let $(a_i)_{i \in I}$ be a basis of $A$ over $K$ such that the family $(a_i^p)_{i \in I}$ is linearly free over $K$. Let $L$ be an extension of $K$ and let $x$ be an element of $L \otimes_K A$ such that $x^p = 0$. Write $x = \sum_{i \in I} \lambda_i \otimes a_i$ with $A_i \in L$ for all $i \in I$. We have $x^p = \sum_{i \in I} \lambda_i^p \otimes a_i^p = 0$ and since the family $(a_i^p)_{i \in I}$, is linearly free over $K$, we have $\lambda_i^p = 0$, whence $\lambda_i = 0$ for all $i \in I$; it follows that $x = 0$. So we have proved that $x^p = 0$ implies $x = 0$ in $L \otimes_K A$, from which it follows at once that $L \otimes_K A$ is reduced.

#### Corollary 1 (Mac Lane) {#alg-v-s15-thm-2-cor-1 .statement}

— *Let* $K$ *be a field of characteristic exponent* $p$, $\Omega$ *a perfect extension of* $K$ *and* $L$ *a subextension of* $\Omega$. *Then the following conditions are equivalent*:

a) $L$ *is separable over* $K$.

b) $L$ *is linearly disjoint from* $K^{p^{-\infty}}$ *over* $K$.

c) $L$ *is linearly disjoint over* $K$ *from every* $p$*-radical extension of* $K$ *contained in* $\Omega$, *of finite degree and height* $\leqslant 1$.

The case where $K$ is of characteristic 0 is trivial because then $L$ is separable over $K$ (Th. 1) and $K^{p^{-\infty}} = K$ by convention. Suppose then that $p \neq 1$, and let us first show that $a)$ implies $b)$. Assume that $L$ is separable over $K$ and let $(a_i)_{i \in I}$, be a basis of $L$ over $K$. Let $(\lambda_i)_{i \in I}$ be a family of finite support of elements of $K^{p^{-\infty}}$ such that $\sum_{i \in I} \lambda_i a_i = 0$; there exists an integer $f \geqslant 0$ and elements μ_i of K such that λ_i = μ_i^{p^{-f}}. We have

$$
\sum_{i \in I} \mu_i a_i^{p^f} = \left( \sum_{i \in I} \lambda_i a_i \right)^{p^f} = 0
$$

and Th. 2 implies, by induction on f, that the family $(a_i^{p^f})_{i \in I}$ is linearly free over K. We thus have $\mu_i = 0$, whence $\lambda_i = 0$ for all $i \in I$. Finally L is linearly disjoint from $K^{p^{-\infty}}$ over K.

It is clear that b) implies c). Lastly suppose that c) holds and let K' be an extension of K of finite degree and p-radical of height $\leq 1$. The ring $K' \otimes_K L$ is isomorphic to a subring of $\Omega$, hence is reduced. Now it follows from Th. 2 that L is separable over K.

#### Corollary 2 {#alg-v-s15-thm-2-cor-2 .statement}

— *Let K be a field of characteristic exponent p, $K^{p^{-\infty}}$ a perfect closure of K and L a separable extension of K. Then the ring $L \otimes_K K^{p^{-\infty}}$ is a field. If moreover L is algebraic over K, then $L \otimes_K K^{p^{-\infty}}$ is a perfect closure of L.*

The case $p = 1$ is trivial, so let us suppose $p \neq 1$. Let $\Omega$ be a perfect closure of L. By Cor. 1 there exists a K-algebra homomorphism of $L \otimes_K K^{p^{-\infty}}$ onto $L[K^{p^{-\infty}}]$ which maps $x \otimes y$ to $xy$ for $x \in L$ and $y \in K^{p^{-\infty}}$. Since $K^{p^{-\infty}}$ is algebraic over K, the ring $L[K^{p^{-\infty}}]$ is a subfield of $\Omega$ (V, p. 18, Cor. 1). Suppose further that L is algebraic over K, then $L[K^p]$ is an algebraic extension of the perfect field $K^{p^{-\infty}}$, hence it is a perfect field (V, p. 43, Cor. 1); finally, since the field $L[K^{p^{-\infty}}]$ is ap-radical extension of L (V, p. 25, Cor.), it is a perfect closure of L.

#### Corollary 3 {#alg-v-s15-thm-2-cor-3 .statement}

— *Let L be an algebraic extension of K and M a commutative L-algebra (for example an extension of L). If M is separable over K, it is separable over L.*

The algebra L is K-isomorphic to a subalgebra of M, hence L is a separable extension of K. Therefore (Cor. 2) there exists an L-isomorphism of $L^{p^{-\infty}}$ onto $K^{p^{-\infty}} \otimes_K L$. The ring $L^{p^{-\infty}} \otimes_L M$ is thus isomorphic to $(K^{p^{-\infty}} \otimes_K L) \otimes_L M$, and so to $K^{p^{-\infty}} \otimes_K M$ (II, p. 278, Prop. 2) and this latter ring is reduced because M is separable over K. Thus the ring $L^{p^{-\infty}} \otimes_L M$ is reduced, which proves that M is separable over L (V, p. 122, Th. 2).

#### Remark {#alg-v-s15-n4-rem-1 .statement}

— Mac Lane's criterion may be formulated without introducing any extensions of K other than L. For by c) of Cor. 1, L is separable over K if and only if L and $K^P$ are linearly disjoint over K. Since the mapping $x \mapsto x^p$ is an isomorphism of L onto the subfield $L^P$, we obtain the following criterion (cf. V, p. 177, Ex. 11 for an analogous criterion for algebras):

*L is separable over K if and only if the subfields $L^P$ and K of L are linearly disjoint over $K^P$.*

### 5. Extensions of a perfect field

For ease of reference we summarize the principal properties of extensions of perfect fields:

#### Theorem 3 {#alg-v-s15-thm-3 .statement}

— Let K be a perfect field.
a) Every algebraic extension of K is a perfect field.
b) Every extension of K is separable.
c) For a K-algebra to be separable it is necessary and sufficient that it should be reduced.
d) Let A and B be two reduced K-algebras. Then $A \otimes_K B$ is reduced.
e) If E and F are two extensions of K, then the ring $E \otimes_K F$ is reduced.

Assertion a) is just Cor. 1 of Prop. 11 (V, p. 43).
Assertion b) follows from Th. 1 (V, p. 122) when K is of characteristic 0 and from Cor. 1 (V, p. 123) when K is of characteristic $p \neq 0$.
Let us prove c). The case where K is of characteristic 0 follows from Th. 1 (V, p. 122). So it is enough to show that if K is perfect of characteristic $p \neq 0$ and A is a reduced K-algebra, then A is separable over K. But this follows from the equivalence of the conditions a) and b) of Th. 2 (V, p. 122; take $K' = K$ in b)).
Finally, d) follows from c) and Prop. 5 (V, p. 120) and e) is a particular case of d).

### 6. The characterization of separability by automorphisms

#### Theorem 4 {#alg-v-s15-thm-4 .statement}

— Let $\Omega$ be an algebraically closed extension of a field K and L a subextension of $\Omega$. Then the following conditions are equivalent:
a) L is separable over K.
b) The intersection of the kernels of the 0-algebra homomorphisms of $\Omega \otimes_K L$ into $\Omega$ is reduced to 0.
c) For any elements $a_1, \ldots, a_n$ of L linearly independent over K there exist K-automorphisms $\sigma_1, \ldots, \sigma_n$ of $\Omega$ such that $\det(\sigma_i(a_j)) \neq 0$.
d) Let V be a vector sub-K-space of L of finite dimension. Every K-linear mapping of V into $\Omega$ is a linear combination (with coefficients in R) of the restrictions to V of K-automorphisms of $\Omega$.

$d) \Rightarrow c)$: Let $a_1, \ldots, a_n$ be elements of L linearly independent over K and let V be the vector sub-K-space of L generated by $a_1, \ldots, a_n$. The mapping $f \mapsto (f(a_1), \ldots, f(a_n))$ is an R-linear bijection of $\mathrm{Hom}_K(V, R)$ onto $\Omega^n$. Suppose that d) holds, then there exist K-automorphisms $a_1, \ldots, a_n$ of $\Omega$ such that the elements $(\sigma_i(a_1), \ldots, \sigma_i(a_n))$ of $\Omega^n$ (for $1 \leq i \leq n$) form a basis of $\Omega^n$. We thus have $\det(\sigma_i(a_j)) \neq 0$, so d) implies c).

c) $\Rightarrow$ b): Assume that c) holds and let x be in $\Omega \otimes_K L$. We write x in the form $\sum_{j=1}^n x_j \otimes a_j$, with $x_1, \ldots, x_n$ in $\Omega$ and the elements $a_1, \ldots, a_n$ of L linearly independent over K. Choose K-automorphisms $\sigma_1, \ldots, \sigma_n$ of $\Omega$ such that $\det \sigma_i(a_j) \neq 0$; let $\chi_1, \ldots, \chi_n$ be the R-homomorphisms of $\Omega \otimes_K L$ into $\Omega$ such that $\chi_i(a \otimes b) = a \cdot \sigma_i(b)$ for $a \in \Omega$ and $b \in L$. Suppose that $\chi_i(x) = 0$ for $1 \leq i \leq n$, in other words, that $\sum_{j=1}^n x_j \cdot \sigma_i(a_j) = 0$ for $1 \leq i \leq n$. Since we have assumed that the matrix $(\sigma_i(a_j))$ has a non-zero determinant, we have $x_i = 0$ for $1 \leq i \leq n$ and so $x = 0$.

b) $\Rightarrow$ a): Since every extension of a field of characteristic 0 is separable (V, p. 122, Th. 1) it suffices to examine the case where K is of characteristic $p \neq 0$. Let X be the set of all R-algebra homomorphisms of $\Omega \otimes_K L$ into $\Omega$ and f the homomorphism of $\Omega \otimes_K L$ into $\Omega^X$ defined by $f(u) = (\chi(u))_{\chi \in X}$ for $u \in \Omega \otimes_K L$. Condition b) means that f is injective and so implies that the ring $\Omega \otimes_K L$ is reduced. Hence condition b) of Th. 2 (V, p. 122) is satisfied with $K' = \Omega$, so L is separable over K.

a) $\Rightarrow$ d): Suppose that L is separable over K. Let V be a vector sub-K-space of finite dimension of L, $V_{(\Omega)} = \Omega \otimes_K V$ the vector $\Omega$-space derived from V by extension of scalars and $f_0$ the linear form on $V_{(\Omega)}$ such that $f_0(x \otimes y) = xy$ for $x \in \Omega, y \in V$. Denote by G the group of K-automorphisms of $\Omega$; for $\sigma \in G$ we put $\sigma_V = \sigma \otimes \mathrm{Id}_V$ and $g_\sigma = \sigma \circ f_0 \circ \sigma_V^{-1}$.

For each $\sigma \in G$ the mapping $g_\sigma$ of $V_{(\Omega)}$ into $\Omega$ is $\Omega$-linear and maps $x \otimes y$ to $x \cdot \sigma(y)$ for $x \in \Omega, y \in V$. The kernel $N_\sigma$ of $g_\sigma$ is therefore a vector subspace of $V_{(\Omega)}$, and the same holds for $N = \cap_{\sigma \in G} N_\sigma$. If p is the characteristic exponent of K, the field of invariants of G in $\Omega$ is equal to $K^{p^{-\infty}}$ (V, p. 112, Prop. 10). We clearly have $\sigma_V(N) = N$ for all $\sigma \in G$; therefore (V, p. 63, Cor.) the vector $\Omega$-space N is generated by $N_0 = N \cap (K^{p^{-\infty}} \otimes V)$. Since L is separable over K, the fields $K^{p^{-\infty}}$ and L are linearly disjoint over K (V, p. 123, Cor. 1); we have $K^{p^{-\infty}} \otimes_K V \subset K^{p^{-\infty}} \otimes_K L$ and $f_0(x \otimes y) = xy$ for $x \in \Omega$ and $y \in V$. It follows that the restriction of $f_0$ to $K^{p^{-\infty}} \otimes_K V$ is injective. Now $f_0 = g_1$ is zero on N and a fortiori on $N_0 \subset K^{p^{-\infty}} \otimes_K V$. We thus have $N_0 = 0$, whence $N = 0$. Since V is of finite dimension over K, $V_{(\Omega)}$ is of finite dimension over $\Omega$; the intersection of the kernels of the linear forms $g_\sigma$ is zero, hence (II, p. 301, Th. 7) the family $(g_\sigma)_{\sigma \in G}$ generates the dual of $V_{(\Omega)}$. Now let $u$ be a K-linear mapping of V into $\Omega$; let $\tilde{u}$ be the linear form on $V_{(\Omega)}$ which maps $x \otimes y$ to $xu(y)$ for $x \in \Omega$ and $y \in V$. By what has been said there exist elements $\sigma_1, \ldots, \sigma_n$ of G and $\lambda_1, \ldots, \lambda_n$ of $\Omega$ such that $\tilde{u} = \sum_{i=1}^n \lambda_i g_{\sigma_i}$, whence $u(y) = \sum_{i=1}^n \lambda_i \sigma_i(y)$ for all $y \in V$. So we have shown that a) implies d).

### Exercises {#alg-v-s15-exercises}

See the [exercises for § 15](exercises/s15/).
