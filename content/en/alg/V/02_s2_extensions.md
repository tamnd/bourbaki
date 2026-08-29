---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 2
section_title: Extensions
lang: en
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A V.9-A V.15, A V.146-A V.147
pdf_pages: 0123-0129, 0260-0261
extraction: ocr
subsections:
    - "no": 1
      title: The structure of an extension
      page: 9
      pdf_page: 123
    - "no": 2
      title: Degree of an extension
      page: 10
      pdf_page: 124
    - "no": 3
      title: Adjunction
      page: 10
      pdf_page: 124
    - "no": 4
      title: Composite extensions
      page: 12
      pdf_page: 126
    - "no": 5
      title: Linearly disjoint extensions
      page: 13
      pdf_page: 127
statements: 19
exercises: 4
content_sha256: 577f8f2cd0d7531154d44ed4dfc254c2023dc0e83a12625db63a8875dd8f9066
---

## § 2. EXTENSIONS

### 1. The structure of an extension

#### Definition 1 {#alg-v-s2-def-1 .statement}

— Let K be a field. By an extension of K we understand a K-algebra whose underlying ring is a field. By a subextension (or sub-K-extension) of the extension E we understand a sub-K-algebra of E which is a field.
Let E be an extension of K. The mapping u : A ↦ λ . 1 of K into E is a ring homomorphism; by I, p. 115, u induces an isomorphism of K onto a subfield u(K) of E.
Conversely, if K, E are fields and u is a homomorphism of K into E, then u defines on E a structure of extension of K (III, p. 433). By abuse of language one sometimes says that (E, u) is an extension of K.
An extension is said to be trivial if u(K) = E, that is, if E is a vector space of dimension 1 over K.
Let L be an extension field of K. When we consider L as extension of K, we understand by this the extension (L, j) of K, where j is the canonical injection of K into L, or also L with the corresponding K-algebra structure. The subextensions of L are then the intermediate fields between K and L, that is, the subfields of L containing K. If L' is another extension field of K, a K-homomorphism of L into L' is then a homomorphism f of L into L' such that f(x) = x for all x ∈ K. We note that if f is any endomorphism of the field L, then the set of elements of L invariant under f is a subfield K' of L, and that f is then a K'-endomorphism of L.
In particular let P be the prime subfield of a field L. We can consider L as an extension of P, and every endomorphism of L is then a P-endomorphism.
Let (E, u) be an extension of K; since u defines an isomorphism of K onto a subfield K_1 of E, there is in general no difficulty in identifying K with K_1 by means of u. One case where we cannot allow such an identification is that where K = E and where u is thus an endomorphism of K; most frequently u will be an automorphism of K, or the mapping u ↦ u'', when the field K is of characteristic ≠ 0.
It is clear that every extension of K is isomorphic to an extension (L, j), where L is a field containing K as subfield and j is the canonical injection of K into L.

### 2. Degree of an extension

Let $A$ be an algebra over a field $K$. It is in particular a vector space over $K$; the dimension of this vector space is called the degree of $A$ over $K$ and is written $[A : K]$ (II, p. 293). By definition $[A : K]$ is thus the cardinal of any basis of $A$ over $K$. This definition applies in particular to the case of extensions of $K$.

An extension of degree 1 is trivial. An extension of degree 2 (resp. 3 etc.) is called quadratic (resp. cubic etc.). An extension of finite degree is sometimes called, by abuse of language, a finite extension.

#### Theorem 1 {#alg-v-s2-thm-1 .statement}

*Let $E$ be an extension of $K$ and $A$ an algebra over $E$. Then we have $[A : K] = [A : E] \cdot [E : K]$. In particular, if $F$ is an extension of $E$, we have*

$$
[F : K] = [F : E] \cdot [E : K].
$$

The theorem is just a special case of II, p. 222, Prop. 25; more precisely, if $(a_i)$, , , is a basis of $A$ over $E$ and $(b_j)$, $\in M$ a basis of $E$ over $K$, then the family $(a_\lambda b_\mu)_{(\lambda,\mu) \in L \times J}$ is a basis of $A$ over $K$.

#### Corollary 1 {#alg-v-s2-thm-1-cor-1 .statement}

*Let $K, E, F$ be three fields such that $K \subset E \subset F$ and $[F : K]$ is finite. Then the degrees $[E : K]$ and $[F : E]$ are divisors of $[F : K]$.

If the degree $[F : K]$ is prime, there is thus no subextension of $F$ other than $K$ and $F$. But note that when $[F : K]$ is not prime, there is not necessarily a subextension of $F$ other than $K$ and $F$ (cf. V, p. 146, Exercise 1).*

#### Corollary 2 {#alg-v-s2-thm-1-cor-2 .statement}

*Let $K, E$ and $F$ be three fields such that $K \subset E \subset F$. Suppose that $[F : K]$ is finite, then the relation $[E : K] = [F : K]$ is equivalent to $E = F$ and the relation $[F : E] = [F : K]$ is equivalent to $E = K$.

For if $L$ is an extension field of $L'$ then $[L : L'] = 1$ is equivalent to $L' = L$.*

#### Proposition 1 {#alg-v-s2-prop-1 .statement}

*Let $A$ be an algebra of finite degree over a field $K$. If an element $a \in A$ is not a left (resp. right) divisor of zero in $A$, then it is invertible in $A$.

For the vector space $A$ over $K$ is of finite dimension, by hypothesis, and the linear mapping $x \mapsto ax$ (resp. $x \mapsto xa$) of $A$ into $A$ injective; it is therefore bijective (II, p. 298, Cor.) and hence (I, p. 16, Remark) $a$ is invertible in $A$.*

#### Corollary {#alg-v-s2-n2-cor-1 .statement}

*Let $A$ be a commutative algebra of finite degree over a field $K$. If $A$ is an integral domain, then it is a field.*

### 3. Adjunction

Let $E$ be an extension of a field $K$. Given a family $x = (x_i)_{i \in I}$ of elements of $E$, we denote by $K(x_i)_{i \in I}$ (or $K(x)$ or also $K(x_1, \ldots, x_r)$ when $I$ is the interval (1, n) of N) the least subextension of E containing the members of the family $(x_i)_i$; we say that $K(x_i)_i \in I$ is obtained by adjunction to K of the elements of the family $(x_i)_i, I$ and that the family $(x_i)_i, I$ (or the set of its elements) is a generating family of $K(x_i)_i \in I$ with respect to K (or over K). The field $K(x_i)_i \in I$ depends only on the set A of elements of the family $(x_i)_i \in I$; we also denote it by $K(A)$. In particular we have $K(E) = E$ and $K(\emptyset) = K . 1$. All that has been said applies in particular when E is a field containing K as subfield.

It should be observed that A is not in general a generating set of the algebra $K(A)$, in other words that $K(A) \neq K[A]$. "Nevertheless we shall see that $K(A) = K[A]$ when $K(A)$ is an algebraic extension of K (V, p. 18, Cor. 1). \*

#### Proposition 2 {#alg-v-s2-prop-2 .statement}

— *If M and N are any two subsets of an extension of a field K, then* $K(M \cup N) = K(M)(N) = K(N)(M)$.

For $K(M \cup N)$ contains $K(M)$ and N and hence $K(M)(N)$; since $K(M)(N)$ is a field containing $K \cup M \cup N$, it contains $K(M \cup N)$, whence the proposition.

We shall sometimes write $K(M, N)$ instead of $K(M \cup N)$.

#### Remark {#alg-v-s2-n3-rem-1 .statement}

— Let P be the prime subfield of a field E (V, p. 2); for every subset A of E, $P(A)$ is the least subfield of E containing A. In particular if K is a subfield of E, we have $P(K \cup A) = K(A)$. If K and K' are two subfields of E, we thus have $P(K \cup K') = K(K') = K'(K)$; this field is the least subfield of E containing K or K', or also the upper bound of K and K' in the set of subfields of E, ordered by inclusion; we sometimes say that this field is the field generated by K and K' in E.

#### Proposition 3 {#alg-v-s2-prop-3 .statement}

— *Let $\mathcal{F}$ be a set of subfields of a field E, directed with respect to the relation $\subset$. The union L of the fields of $\mathcal{F}$ is a field.*

For if x and y are two elements of L, there exist two fields R, S of $\mathcal{F}$ such that $x \in R,\ y \in S$; let T be a field of $\mathcal{F}$ containing R and S; then $x \in T,\ y \in T$, hence $x + y,\ xy$ and $x^{-1}$ (if $x \neq 0$) belong to T, hence to L.

#### Corollary {#alg-v-s2-n3-cor-1 .statement}

— *Let E be an extension of a field K and $A \subset E$. The field $K(A)$ is the union of the fields $K(F)$ where F ranges over the set of all finite subsets of A.*

For the set of fields $K(F)$ is directed by the relation $\subset$, because $F \subset F'$ implies $K(F) \subset K(F')$. The union L of these fields is thus a field containing $K \cup A$ and contained in $K(A)$, and hence identical with $K(A)$.

#### Definition 2 {#alg-v-s2-def-2 .statement}

— *An extension E of a field K is said to be finitely generated if it has a finite generating family. It is called monogenous if there exists x in E such that* $E = K(x)$.

The Cor. of Prop. 3 shows that every extension E of a field K is a directed union of finitely generated extensions contained in E. It is clear that every extension E of K of finite degree is also finitely generated because a basis of E (considered as vector space over K) is also a generating family of E over K; we shall see later that the converse does not hold.

### 4. Composite extensions

Let E and F be two extensions of a field K. By a composite extension of $E$ and F we understand any triple $(L, u, v)$, where L is an extension of K, $u$ is a K-homomorphism of E into L and $v$ is a K-homomorphism of F into L, and where the field L is generated by $u(E) \cup v(F)$ (cf. Fig. 1).

![Diagram showing extensions E, F, K, L, homomorphisms u, v, r](../images/fig_1.png)

Fig. 1.

In agreement with the general definitions (E, IV, p. 6) an isomorphism of a composite extension $(L, u, v)$ of E and F onto a composite extension $(L', u', v')$ of E and F is a K-isomorphism $\varphi$ of L onto $L'$ such that $u' = \varphi \circ u$ and $v' = \varphi \circ v$.

Let $(L, u, v)$ be a composite extension of E and F. The K-linear mapping $w$ of $E \otimes_K F$ into L which sends $x \otimes y$ to $u(x)v(y)$ is a K-algebra homomorphism; in this No. we shall denote it by $u * v$. Its image is the subring of L generated by $u(E) \cup v(F)$.

#### Proposition 4 {#alg-v-s2-prop-4 .statement}

— Let E, F be two extensions of K.

a) Let $(L, u, v)$ be a composite extension of E and F; then the kernel p of the homomorphism $u * v$ of $E \otimes_K F$ into L is a prime ideal.

b) Let p be a prime ideal of $E \otimes_K F$; then there exists a composite extension $(L, u, v)$ of E and F such that p is the kernel of $u * v$, and any two such composite extensions are isomorphic.

Assertion a) follows from the fact that the kernel of a homomorphism of a ring into a field is a prime ideal (I, p. 116-117).

Let p be a prime ideal of $E \otimes_K F$, A the quotient ring $(E \otimes_K F)/p$ and L the field of fractions of A. For $x \in E$ (resp. $y \in F$) we denote by $u(x)$ (resp. $v(y)$) the residue class mod p of $x \otimes 1$ (resp. $1 \otimes y$). Then $u$ (resp. $v$) is a K-homomorphism of E (resp. F) into L and $u(E) \cup v(F)$ generates A as a ring, hence L as a field. Therefore $(L, u, v)$ is a composite extension of E and F; we see at once that $u * v$ is the canonical homomorphism of $E \otimes_K F$ into L, and its kernel is thus equal to p.

Let $(L', u', v')$ be a composite extension of E and F such that the kernel of $u' * v'$ is equal to p. Since $u * v$ and $u' * v'$ have the same kernel, there exists an isomorphism $\psi$ of A onto the image $A'$ of $u' * v'$, characterized by $u' * v' = \psi \circ (u * v)$. But $A'$ is the subring of $L'$ generated by $u'(E) \cup v'(F)$, hence L' is the field of fractions of A'. Therefore $\psi$ extends to an homomorphism $\varphi$ of L onto L' and it is clear that $\varphi$ is an isomorphism of $(L, u, v)$ onto $(L', u', v')$.

#### Remark {#alg-v-s2-n4-rem-1 .statement}

— If $p$ and $p'$ are two distinct prime ideals of $E \otimes_K F$, the corresponding *composite extensions* of $E$ and $F$ (constructed by the procedure of the above proof) are not isomorphic. However, they may nevertheless be isomorphic as *extensions* of K (*V*, p. 146, Ex. 2).

#### Corollary {#alg-v-s2-n4-cor-1 .statement}

*There exist composite extensions of E and F*.

For since the commutative ring $E \otimes_K F$ is not reduced to 0, it has prime ideals : Krull's theorem (*I*, p. 104) proves the existence of maximal ideals and every maximal ideal is prime.

We can make this corollary more precise as follows. Let $(E, u)$ and $(F, v)$ be two extensions of K ; choose a maximal ideal m of the commutative ring $E \otimes_K F$ and put $L = (E \otimes_K F)/m$; then L is an extension of K. For $x \in E$ write $u'(x)$ for the residue class of $x \otimes 1$ mod m and similarly put $v'(y)$ for the residue class of $1 \otimes y$ mod $m$ for all $y \in F$. We then have a commutative diagram of field homomorphisms

$$
\begin{array}{ccc}
F & \xrightarrow{v'} & L \\
| & & | \\
K & \xrightarrow{u} & E .
\end{array}
$$

By replacing $(L, u')$ by an isomorphic extension of E we may suppose that L contains E as subfield and that $u'$ is the canonical injection of E in L. By changing notation we thus obtain the following scholium :

#### Scholium {#alg-v-s2-n4-sch-1 .statement}

*Let K and E be two fields and u a homomorphism of K into E. If K' is a field containing K as subfield, there exists a field E' containing E as subfield and a homomorphism u' of K' into E' extending u*'.

### 5. Linearly disjoint extensions

*Throughout this No. R denotes an extension of the field K*.

Let A and B be two sub-K-algebras of R. There exists an algebra homomorphism $\varphi : A \otimes_K B \to R$ which maps $x \otimes y$ to $xy$. The image of $\varphi$ is a subring C of $\Omega$ generated by A U B. Moreover by II, p. 256, if $(b,)$ is a basis of B over K and $(a,)$ a basis of A over K, then C coincides with the set of linear combinations $\sum_{\mu} \alpha_{\mu} b_{\mu}$ where $\alpha_{\mu} \in A$, the set of all $\sum_{\lambda} \beta_{\lambda} a_{\lambda}$ where $\beta_{\lambda} \in B$ and also the set of all $\sum_{\lambda,\mu} \gamma_{\lambda\mu} a_{\lambda} b_{\mu}$, where $\gamma_{\lambda\mu} \in K$.

We shall say that A and B are *linearly disjoint over* K, if $\varphi$ is an *isomorphism* of $A \otimes_K B$ onto C. We then have $A \cap B = K$; every free subset of B (resp. A) with respect to K is then free with respect to A (resp. B); conversely, for A and B to be linearly disjoint over K, it is sufficient that there should exist *one* basis of B over K (for example) which is free with respect to A (II, p. 256 and III, p. 469).

Consider particularly the case where A and B are *subextensions* of $\Omega$.

#### Proposition 5 {#alg-v-s2-prop-5 .statement}

*Let E and F be two extensions of K contained in $\Omega$.*

*a)* *If F has finite degree over K, then the subring of $\Omega$ generated by $E \cup F$ is a field, coinciding with $E(F)$ and the degree of $E(F)$ over E is finite; we have* $[E(F):E] \leq [F:K]$, *with equality if and only if E and F are linearly disjoint over K. In that case $E(F)$ is E-*isomorphic* to $E \otimes_K F$.*

*b)* *If further E is of finite degree over K, then $E(F) = K(E \cup F)$ is of finite degree over K. We have* $[K(E \cup F):K] \leq [E:K][F:K]$ *with equality if and only if E and F are linearly disjoint over K.*

For let C be the subring of $\Omega$ generated by $E \cup F$; if $(b_j)_{1 \leq j \leq n}$ is a basis of F over K, then C is the vector sub-E-space of $\Omega$ generated by the $b_j$ hence C is an algebra of *finite* rank $\leq n$ over E; since the ring C is contained in a field, it is an integral domain, and hence a *field*, by the Cor. to Prop. 1 (V, p. 10), whence $C = E(F)$ and $[E(F):E] \leq [F:K]$. The relation $[E(F):E] = [F:K]$ means that the $b_j$ are linearly independent over E, hence that E and F are linearly disjoint over K; this proves part *a)* of the proposition. Part *b)* now follows at once because $[E(F):K] = [E(F):E][E:K]$.

Let E and F be extensions of K contained in $\Omega$; if E and F are of infinite degree over K, the subring $C = K[E \cup F]$ is not necessarily a field $^1$; however the *field of fractions* of C then coincides with $K(E \cup F)$. More generally let A be a subring of E such that E is the field of fractions of A, and let B be a subring of F such that F is the field of fractions of B; then if C is the subring of $\Omega$ generated by $A \cup B$, $K(E \cup F)$ coincides with the *field of fractions* of C, because the latter field is the least subfield of $\Omega$ containing C and it contains E and F. Moreover:

#### Proposition 6 {#alg-v-s2-prop-6 .statement}

*Let E and F be two extensions of K contained in $\Omega$, and A and B two subalgebras of $\Omega$ over K such that E is the field of fractions of A and F the field of fractions of B. Then for E and F to be linearly disjoint over K it is necessary and sufficient that A and B be linearly disjoint over K.*

The condition is clearly necessary. Conversely, if A and B are linearly disjoint over K, A and F are so too, because if a family of elements of $\Omega$ is free with respect to B, it is free with respect to the field of fractions F of B (II, p. 315, Cor. 1 and p. 316, Cor. 3); now the same argument shows that E and F are linearly disjoint over K.

$^1$ It suffices to consider for example the case where $\Omega$ is the field $K(X, Y)$ of rational fractions in two indeterminates X and Y and $E = K(X), F = K(Y)$.

#### Proposition 7 {#alg-v-s2-prop-7 .statement}

— Let E and F be two extensions of K contained in $\Omega$; if E and F are linearly disjoint over K, then every subextension of E and every subextension of F are linearly disjoint over K. Conversely, if for every pair of finitely generated subextensions E', F' of E and F respectively, E' and F' are linearly disjoint over K, then E and F are linearly disjoint over K.

For the condition for E and F to be linearly disjoint over K may be expressed thus: if $(a_\alpha)$ is a free family in E and $(b_\beta)$ a free family in F, then the relation $\sum_{\alpha,\beta} \lambda_{\alpha\beta} a_\alpha b_\beta = 0$, where $\lambda_{\alpha\beta} \in K$, implies $\lambda_{\alpha\beta} = 0$ for each pair of suffixes. But this condition is satisfied for each pair of free families if it holds for each pair of finite free families.

Thus we may say, speaking intuitively, that linear disjunction is a property « of finite character ».

#### Proposition 8 {#alg-v-s2-prop-8 .statement}

— Let E, F, G be three extensions of a field K contained in $\Omega$, such that $F \subset G$. For E and G to be linearly disjoint over K it is necessary and sufficient that E and F should be linearly disjoint over K and that E(F) and G be linearly disjoint over F.

$$
\begin{array}{ccccc}
E & \longrightarrow & E(F) \\
K & \longrightarrow & F & \longrightarrow & G.
\end{array}
$$

Fig. 2.

The condition is necessary: suppose that E and G are linearly disjoint over K. The same then holds of E and F (Prop. 7); on the other hand, if B is a basis of E over K, this is also a basis of the algebra F[E] over F; since B is by hypothesis free over G, F[E] and G are linearly disjoint over F, and the same is true of $E(F) = F(E)$ and G, by Prop. 6.

The condition is sufficient: with the same notation it implies that B is free over F, hence it is a basis of F[E] over F; since F[E] and G are by hypothesis linearly disjoint over F, B is free over G, and this shows that E and G are linearly disjoint over K.

### Exercises {#alg-v-s2-exercises}

See the [exercises for § 2](exercises/s2/).
