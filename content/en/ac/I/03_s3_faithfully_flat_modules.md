---
book: ac
book_title: Commutative Algebra
chapter: I
chapter_title: FLAT MODULES
section: 3
section_title: Faithfully flat modules
lang: en
source: ac-i-vii
book_pages: 27-36, 49-50
pdf_pages: 0047-0056, 0069-0070
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF FAITHFULLY FLAT MODULES
      page: 27
      pdf_page: 47
    - "no": 2
      title: TENSOR PRODUCTS OF FAITHFULLY FLAT MODULES
      page: 30
      pdf_page: 50
    - "no": 3
      title: CHANGE OF RING
      page: 31
      pdf_page: 51
    - "no": 4
      title: RESTRICTION OF SCALARS
      page: 31
      pdf_page: 51
    - "no": 5
      title: FAITHFULLY FLAT RINGS
      page: 32
      pdf_page: 52
    - "no": 6
      title: FAITHFULLY FLAT RINGS AND FINITENESS CONDITIONS
      page: 34
      pdf_page: 54
    - "no": 7
      title: LINEAR EQUATIONS OVER A FAITHFULLY FLAT RING
      page: 35
      pdf_page: 55
statements: 18
exercises: 10
content_sha256: 6eca3d9ab803d413bfaf6f39a861f11ddce5dbf12fbed96d89ca819c7210a451
---

## 3. FAITHFULLY FLAT MODULES

### 1. DEFINITION OF FAITHFULLY FLAT MODULES

#### Proposition 1 {#ac-i-s3-prop-1 .statement}

Let $E$ be a right $A$-module. The following four properties are equivalent:

(a) For a sequence $N' \xrightarrow{v} N \xrightarrow{w} N''$ of left $A$-modules to be exact, it is necessary and sufficient that the sequence
$$
E \otimes_A N' \xrightarrow{1 \otimes v} E \otimes_A N \xrightarrow{1 \otimes w} E \otimes_A N''
$$
be exact.

(b) $E$ is flat and, for every left $A$-module $N$, the relation $E \otimes_A N = 0$ implies $N = 0$.

(c) $E$ is flat and, for every homomorphism $v : N' \to N$ of left $A$-modules, the relation $1_E \otimes v = 0$ implies $v = 0$.

(d) $E$ is flat and, for every maximal left ideal $m$ of $A$, $E \neq Em$.

To simplify the writing we set $T(Q) = E \otimes_A Q$ for every left $A$-module $Q$ and $T(v) = 1_E \otimes v$ for every homomorphism $v$ of left $A$-modules.

We prove first the equivalence of (a), (b) and (c).

We prove that (a) implies (b). If (a) holds, clearly $E$ is flat (\$2, no. 3, Proposition 1). On the other hand, let $N$ be a left $A$-module such that $T(N) = 0$ and consider the sequence $0 \to N \to 0$; the hypothesis $T(N) = 0$ means that the sequence $0 \to T(N) \to 0$ is exact. By (a) the sequence $0 \to N \to 0$ is exact, whence $N = 0$.

We show that (b) implies (c). Suppose that (b) holds and let $u : N' \to N$ be a homomorphism and $I$ its image. As the image of $T(v)$ is identified with $T(I)$ (\$2, no. 3, Remark 2), the hypothesis $T(v) = 0$ implies $T(I) = 0$, hence $I = 0$ by (b) and consequently $v = 0$.

We show that (c) implies (a). Suppose then that (c) holds and consider a sequence
$$
N' \xrightarrow{v} N \xrightarrow{w} N''
$$
of homomorphisms of left $A$-modules and the corresponding sequence
$$
T(N') \xrightarrow{T(v)} T(N) \xrightarrow{T(w)} T(N'').
$$

If the sequence (1) is exact, so is (2), since $E$ is flat (\$2, no. 3, Proposition 1). Conversely, if (2) is exact, we have first $T(w \circ v) = T(w) \circ T(v) = 0$, hence $w \circ v = 0$ by hypothesis. Set $I = v(N')$ and $K = \overline{w}(0)$; then $I$ is contained in $K$ by the above. Consider the exact sequence
$$
0 \to I \xrightarrow{i} K \xrightarrow{p} K/I \to 0
$$
$i$ and $p$ being the canonical mappings. As $E$ is flat, the sequence
$$
0 \to T(I) \xrightarrow{T(i)} T(K) \xrightarrow{T(p)} T(K/I) \to 0
$$
is exact, in other words, $T(K/I)$ is isomorphic to $T(K)/T(I)$, which is 0 by hypothesis, since $T(I)$ (resp. $T(K)$) is identified with the image of $T(v)$ (resp. the kernel of $T(w)$) (\$2, no. 3, Remark 2). But the relation $T(p) = 0$ implies $p = 0$ by hypothesis, hence $K = I$, which proves that the sequence (1) is exact.

Finally we show the equivalence of (b) and (d). If (b) holds, then

$$
E/E_m = E \otimes_A (A_s/m) \neq 0
$$

since $A_s/m \neq 0$; whence (d). Conversely, suppose that (d) holds; every left ideal $a \neq A$ of $A$ is contained in a maximal left ideal $m$ (*Algebra*, Chapter I, §8, no. 7, Theorem 2), then the hypothesis $E \neq Em$ implies $E \neq Ea$, in other words, $E \otimes_A (A_s/a) \neq 0$. That is to say, for every *monogenous* left $A$-module $N \neq 0$, $T(N) \neq 0$. If now $N$ is any left $A$-module \#0, it contains a monogenous submodule $N' \neq 0$; since $E$ is flat, $T(N')$ is identified with a subgroup of $T(N)$; we have just seen that $T(N') \neq 0$, hence $T(N) \neq 0$.

#### Definition 1 {#ac-i-s3-def-1 .statement}

*A right $A$-module* $E$ *is called faithfully flat if it satisfies the four equivalent conditions of Proposition 1.*

Faithfully flat left $A$-modules are defined similarly; clearly, for a left $A$-module $E$ to be faithfully flat, it is necessary and sufficient that $E$, considered as a right $A^0$-module, be faithfully flat.

#### Remark {#ac-i-s3-n1-rem-1 .statement}

If $E$ is a faithfully flat $A$-module, $E$ is a *faithful* $A$-module: for, if an element $a \in A$ is such that $xa = 0$ for all $x \in E$, the homothety $h : b \mapsto ba$ in $A$ is such that $1, \otimes h = 0$; whence $h = 0$ by property (c) of Proposition 1, that is $a = 0$ since $A$ has a unit element.

*Examples*
(1) The direct sum of a flat module and faithfully flat module is a faithfully flat module by virtue of property (d) of Proposition 1 and § 2, no. 3, Proposition 2.
(2) *As $A$*, is faithfully flat by virtue of criterion (d) of Proposition 1 and § 2, no. 4, *Example* 1, it follows from (1) that every free module *not reduced to 0* is faithfully flat. On the other hand, there exist non-zero direct factors of free modules (in other words, non-zero projective modules) which are faithful but *not* faithfully flat (Exercise 2).
(3) Let $A$ be a *principal ideal domain*. For an $A$-module $E$ to be faithfully flat, it is necessary and sufficient that it be *torsion-free* and $E \neq Ep$ for every irreducible element (*Algebra*, Chapter VII, § 1, no. 3) $p$ of $A$; this follows immediately from § 2, no. 4, Proposition 3 and criterion (d) of Proposition 1.
(4) Example (3) shows that the $\mathbf{Z}$-module $\mathbf{Q}$ is a flat and faithful module, but *not faithfully flat*.

#### Proposition 2 {#ac-i-s3-prop-2 .statement}

*Let $E$ be a faithfully flat right $A$-module and $u : N' \to N$ a left $A$-module homomorphism. For $u$ to be injective (resp. surjective, bijective), it is necessary and sufficient that $1_E \otimes u : E \otimes_A N' \to E \otimes_A N$ be so.*

This is an immediate consequence of criterion (a) of Proposition 1.

#### Proposition 3 {#ac-i-s3-prop-3 .statement}

Let $0 \to E' \to E \to E'' \to +0$ be an exact sequence of right $A$-modules. Suppose that $E'$ and $E''$ are flat and that one of them is faithfully flat. Then $E$ is faithfully flat.

We know already that $E$ is flat ($\S 2$, no. 5, Proposition 5). We verify that $E$ has property (b) of Proposition 1. Let $N$ be a left $A$-module. As $E''$ is flat, there is an exact sequence

$$
0 \to E' \otimes_A N \to E \otimes_A N \to E'' \otimes_A N \to 0
$$

($\S 2$, no. 5, Proposition 4). If $E \otimes_A N = 0$, it follows that $E' \otimes_A N$ and $E'' \otimes_A N$ are zero; as one of the modules $E'$, $E''$ is faithfully flat, this implies that $N = 0$.

### 2. TENSOR PRODUCTS OF FAITHFULLY FLAT MODULES

#### Proposition 4 {#ac-i-s3-prop-4 .statement}

Let $R, S$ be two rings, $E$ a right $R$-module and $F$ an $(R, S)$-bimodule. Suppose that $E$ is faithfully flat. Then, for $F$ to be a flat (resp. faithfully flat) $S$-module, it is necessary and sufficient that $E \otimes_R F$ be so.

(1) If $F$ is flat, $E \otimes_R F$ is flat ($\S 2$, no. 7, Proposition 8).

(2) Suppose that $E \otimes_R F$ is flat and let $\nu : N' \to N$ be an injective left $S$-module homomorphism. The homomorphism

$$
l_E \otimes l_F \otimes \nu : E \otimes_R F \otimes_S N' \to E \otimes_R F \otimes_S N
$$

is then injective ($\S 2$, no. 3, Proposition 1). It follows from Proposition 2 of no. 1 that $l_F \otimes \nu : F \otimes_S N' \to F \otimes_S N$ is injective; then $F$ is a flat $S$-module ($\S 2$, no. 3, Proposition 1).

(3) Suppose that $F$ is faithfully flat and let $N$ be a left $S$-module such that $E \otimes_R F \otimes_S N = 0$. Since $E$ is faithfully flat, this implies that $F \otimes_S N = 0$, whence $N = 0$ since $F$ is faithfully flat; this proves that $E \otimes_R F$ is faithfully flat.

(4) Suppose that $E \otimes_R F$ is faithfully flat and let $N$ be a left $S$-module such that $F \otimes_S N = 0$. Then $E \otimes_R F \otimes_S N = 0$, whence $N = 0$, which shows that $F$ is faithfully flat.

#### Corollary {#ac-i-s3-n2-cor-1 .statement}

Let $C$ be a commutative ring and $E$ and $F$ two faithfully flat $C$-modules. Then the $C$-module $E \otimes_C F$ is faithfully flat.

Apply Proposition 4 with $R = S = C$.

### 3. CHANGE OF RING

#### Proposition 5 {#ac-i-s3-prop-5 .statement}

Let $\rho$ be a homomorphism from a ring $A$ to a ring $B$. If $E$ is a faithfully flat right $A$-module, the right $B$-module $\rho^*(E) = E_{(B)} = E \otimes_A B$ is faithfully flat.

Apply Proposition 4 of no. 2 with $R = A, S = F = B$, noting that the $B$-module $B_d$ is faithfully flat.

#### Corollary {#ac-i-s3-n3-cor-1 .statement}

*If $E$ is a faithfully flat right $A$-module and if $a$ is a two-sided ideal of $A$, the right $(A/a)$-module $E/Ea$ is faithfully flat.*

Apply Proposition 5 with $B = A/a, \rho$ being the canonical homomorphism.

#### Proposition 6 {#ac-i-s3-prop-6 .statement}

Let $A$ be a commutative ring, $B$ an algebra over $A$ and $\rho : a \mapsto a . 1$ the canonical homomorphism of $A$ to $B$. Suppose that $B$ is a faithfully flat $A$-module. Then, for an $A$-module $E$ to be flat (resp. faithfully flat), it is necessary and sufficient that the right $B$-module $E_{(B)} = E \otimes_A B$ be flat (resp. faithfully flat).

(1) If $E$ is flat (resp. faithfully flat), $E_{(B)}$ is flat (resp. faithfully flat) by § 2, no. 7, Corollary 2 to Proposition 8 (resp. by Proposition 5).

(2) Suppose that $E_{(B)}$ is flat and let $\nu : N' \to N$ be an injective $A$-module homomorphism. By § 2, no. 7, Corollary 3, the $A$-module $E \otimes_A B$ is flat, hence the homomorphism $1, \otimes 1_B \otimes \nu : E \otimes_A B \otimes_A N' \to E \otimes_A B \otimes_A N$ is injective. As the right and left $A$-module structures on $B$ coincide, this homomorphism is identified with

$$
1_E \otimes \nu \otimes 1_B : E \otimes_A N' \otimes_A B \to E \otimes_A N \otimes_A B.
$$

As $B$ is a faithfully flat $A$-module, it follows that $1_E \otimes \nu : E \otimes_A N' \to E \otimes_A N$ is injective (no. 1, Proposition 2), which shows that $E$ is flat.

(3) Suppose finally that $E_{(B)}$ is faithfully flat. First of all $E$ is flat by (2). Also let $N$ be an $A$-module such that $E \otimes_A N = 0$. Then $E \otimes_A N \otimes_A B = 0$, whence, since the right and left $A$-module structures on $B$ coincide, $E \otimes_A B \otimes_A N = 0$, which may also be written $(E \otimes_A B) \otimes_B (B \otimes_A N) = 0$. As $E_{(B)}$ is a faithfully flat $B$-module, this implies that $B \otimes_A N = 0$ (no. 1, Proposition 1), whence $N = 0$ since $B$ is a faithfully flat $A$-module (no. 1, Proposition 1).

### 4. RESTRICTION OF SCALARS

#### Proposition 7 {#ac-i-s3-prop-7 .statement}

*Let $A, B$ be two rings and $\rho$ a homomorphism of $A$ to $B$. Let $E$ be a faithfully flat right $B$-module. For $\rho^*(E)$ to be a flat (resp. faithfully flat) right $A$-module, it is necessary and sufficient that $B$ be a flat (resp. faithfully flat) right $A$-module.*

Applying Proposition 4 of no. 2 with $B, A, E, B$ in place of $R, S, E, F$ respectively, and the right $A$-module structure on $B$ being defined by $\rho$, it is seen that

B is a flat (resp. faithfully flat) A-module if and only if $E \otimes_B B = \rho^*(E)$ is a flat (resp. faithfully flat) A-module.

Remarks
(1) Proposition 7 shows that, for B to be a faithfully flat A-module, it is sufficient that there exist one faithfully flat B-module which is also a faithfully flat A-module.
(2) Let A, B, C be three rings and $\rho : A \to B, \sigma : B \to C$ two ring homomorphisms. Proposition 7 shows that if C is a faithfully flat B-module and B a faithfully flat A-module, then C is a faithfully flat A-module. If C is a faithfully flat B-module and a faithfully flat A-module, then B is a faithfully flat A-module (taking the modules as right modules, to fix the ideas). On the other hand B and C may be faithfully flat A-modules without C being a faithfully flat B-module (Exercise 7).

### 5. FAITHFULLY FLAT RINGS

#### Proposition 8 {#ac-i-s3-prop-8 .statement}

Let A, B be two rings and $\rho$ a homomorphism from A to B. Suppose that there exists a right B-module E such that $\rho_*(E)$ is a faithfully flat A-module. Then:
(i) For every left A-module F, the canonical homomorphism $j : F \to F_{(B)} = B \otimes_A F$ (such that $j(x) = 1 \otimes x$ for all $x \in F$) is injective.
(ii) For every left ideal a of A, $\overline{\rho}^{-1}(Ba) = a$.
(iii) The homomorphisms $\rho$ is injective.
(iv) For every maximal left ideal m of A, there exists a maximal left ideal n of B such that $\overline{\rho}^{-1}(n) = m$.

We prove (i). We know (Algebra, Chapter 11, § 5, no. 2, Corollary to Proposition 5) that for every right B-module M, the canonical A-homomorphism $i : M \to \rho_*(M) \otimes_A B = \rho^*(\rho_*(M))$ defined by $i(y) = y \otimes 1$ is injective and that the A-module $i(M)$ is a direct factor of $\rho_*(M) \otimes_A B$. Hence, for every left A-module F,

$$
i \otimes 1_F : \rho_*(M) \otimes_A F \to \rho_*(M) \otimes_A B \otimes_A F
$$

is injective (\S 2, no. 1, Lemma 2). Taking $M = E$, it follows (since $i \otimes 1_F = 1_M \otimes j$) that $j$ is injective (no. 1, Proposition 2).

Assertion (ii) follows from (i) by taking $F = A_s/a$ and (iii) from (ii) by taking $a = \{0\}$.

Finally, if m is a maximal left ideal of A, then $\overline{\rho}^{-1}(Bm) = m$ by (ii), and consequently $Bm \# B$. Then there exists a maximal left ideal n of B containing Bm (Algebra, Chapter I, § 8, no. 7, Theorem 2); then $m \subset \overline{\rho}^{-1}(n)$ and as $\rho(1) \notin n$, $1 \notin \overline{\rho}^{-1}(n)$. Consequently $\overline{\rho}^{-1}(n) = m$.

If $A$ and $B$ satisfy the conditions of Proposition 8, $A$ is usually identified with a subring of $B$ by means of $\rho$.

#### Corollary {#ac-i-s3-n5-cor-1 .statement}

Under the hypotheses of Proposition 8, if $B$ is left Noetherian (resp. Artinian), so is $A$.

If (a) is a non-stationary increasing (resp. decreasing) sequence of left ideals of $A$, the sequence $(\mathrm{Ba}_n)$ of ideals of $B$ is non-stationary and increasing (resp. decreasing) since $\rho^{-1}(\mathrm{Ba}_n) = a_n$ contrary to the hypothesis.

*Remark (1). If $A$ and $B$ are commutative, we shall see in Chapter II, § 2, no. 5, Corollary 4 to Proposition 11, that the hypothesis of Proposition 8 implies that for every prime ideal $p$ of $A$, there exists a prime ideal $q$ of $B$ such that $\rho^{-1}(q) = p$ (where $p = A \cap q$ when $A$ is identified with a subring of $B$).*

An important application of Proposition 8 is when $B$ is itself a faithfully flat $A$-module. But in this case we have the following more precise proposition:

#### Proposition 9 {#ac-i-s3-prop-9 .statement}

Let $A, B$ be two rings and $\rho$ a homomorphism of $A$ to $B$. The following five properties are equivalent:
(a) The right $A$-module $B$ is faithfully flat.
(b) The homomorphism $\rho$ is injective and the right $A$-module $B/\rho(A)$ is flat.
(c) The right $A$-module $B$ is flat and, for every left $A$-module $F$, the canonical homomorphism $x \mapsto 1 @ x$ of $F$ to $B @ * F$ is injective.
(d) The right $A$-module $B$ is flat and, for every left ideal $a$ of $A$, $\rho^{-1}(\mathrm{Ba}) = a$.
(e) The right $A$-module $B$ is flat and, for every maximal left ideal $m$ of $A$, there exists a maximal left ideal $n$ of $B$ such that $\rho^{-1}(n) = m$.

By Proposition 8, (a) implies each of the properties (c), (d), (e). On the other hand, if (e) holds, then $Bm \# B$ for every maximal left ideal $m$ of $A$ (since there exists a maximal left ideal $n$ of $B$ such that $Bm \subset n$), and $B$ is a faithfully flat $A$-module by criterion (d) of Proposition 1 of no. 1; hence (e) implies (a).

We shall now prove that (c) $\Rightarrow$ (d) $\Rightarrow$ (b) $\Rightarrow$ (a), which will complete the proof. In the first place, (c) implies (d) by taking $F = A_s/a$ in (c). If (d) holds, by taking $a = \{0\}$ it follows that $\rho$ is injective; (d) and § 2, no. 6, Corollary to Proposition 7 imply that $B/\rho(A)$ is a flat right $A$-module, that is (d) implies (b). Finally, if (b) holds, Proposition 3 of no. 1 applied to the exact sequence

$$
0 \longrightarrow A_a \xrightarrow{\rho} B \longrightarrow B/\rho(A) \longrightarrow 0
$$

shows that $B$ is a faithfully flat right $A$-module, since $A_a$ is faithfully flat.

*Remark (2). If $A$ and $B$ are commutative, we shall see in Chapter II, § 2 no. 5, Corollary 4 to Proposition 11 that the conditions of Proposition 9 are equivalent to the following:

(f) B *is a flat A-module and, for every prime ideal* $\mathfrak{p}$ *of* $A$, *there exists an ideal* $q$ *of* $B$ *such that* $\bar{\rho}^{-1}(q) = \mathfrak{p}$.

Under the conditions of Proposition 9, let us identify $A$ with a *subring* of $B$ by means of $\mathfrak{p}$. The relation $\bar{\rho}^{-1}(Ba) = a$ then reads $A \cap Ba = a$. On the other hand if $F$ is a left $A$-module, $F$ is identified with its image in $B \otimes_A F$ under the canonical mapping $x \mapsto 1 @ x$; if $X$ is an additive subgroup of $F$, then we denote by $BX$ the left sub-B-module of $B \otimes_A F$ generated by $X$. With this notation, we have:

#### Proposition 10 {#ac-i-s3-prop-10 .statement}

*Let* $B$ *be a ring and* $A$ *a subring of* $B$ *such that* $B$ *is a faithfully flat right* $A$-*module. Let* $F$ *be a left* $A$-*module, $F', F''$ *two submodules of* $F$. *Then:*
(i) *The canonical mapping* $B \otimes_A F' \to B \otimes_A F$ *is an isomorphism of* $B \otimes_A F'$ *onto* $BF'$.
(ii) $F \cap BF' = F'$.
(iii) $B(F' + F'') = BF' + BF''$.
(iv) $B(F' \cap F'') = BF' \cap BF''$.

As $B$ is a flat right $A$-module, the canonical mapping
$$
B \otimes_A F' \to B \otimes_A F
$$
is injective; taking account of the identifications made, its image is $BF'$, which proves (i). Assertion (ii) follows from § 2, no. 6, Proposition 7, applied with $E = B$, $E' = A$, and using the formulae $A \otimes_A F = F$ and $A \otimes_A F' = F'$. Assertion (iii) is trivial and (iv) follows from § 2, no. 6, Proposition 6.

### 6. FAITHFULLY FLAT RINGS AND FINITENESS CONDITIONS

#### Proposition 11 {#ac-i-s3-prop-11 .statement}

*Let* $B$ *be a ring and* $A$ *a subring of* $B$ *such that* $B$ *is a faithfully flat right* $A$-*module. For a left* $A$-*module* $F$ *to be definitely generated (resp. finitely presented), it is necessary and sufficient that the* $B$-*module* $B \otimes_A F$ *be finitely generated (resp. finitely presented).*

(1) Without any hypothesis on $B$, clearly, if $F$ is a finitely generated left $A$-module, $B \otimes_A F$ is a finitely generated left $B$-module. Conversely, if $B \otimes_A F$ is a finitely generated $B$-module, it is generated by a finite number of elements of the form $1 \otimes x_i$ with $x_i \in F$; if $M$ is a sub-A-module of $F$ generated by the $x_i$ and $j$ the canonical injection $M \to F$, $1, \otimes j : B \otimes_A M \to B \otimes_A F$ is a surjective homomorphism, hence $j$ is surjective (no. 1, Proposition 2), which proves that $F$ is finitely generated.

(2) *If* $F$ *admits a finite presentation, so does* $B \otimes_A F$ *without any hypothesis* on B (\S 2, no. 8). It remains to prove that, if $B \otimes_A F$ admits a finite presentation, so does F. We already know from (1) that F is finitely generated, hence there exists a surjective homomorphism $u : L \to F$, where L is a finitely generated free A-module. Let R be the kernel of u, so that $B \otimes_A R$ is identified with the kernel of the surjective homomorphism $l_B \otimes u : B \otimes_A L \to B \otimes_A F$ (\S 2, no. 3, *Remark 2*). As $B \otimes_A F$ admits a finite presentation by hypothesis, we conclude (\S 2, no. 8, Lemma 9) that $B \otimes_A R$ is finitely generated; then it follows from (1) that R is a finitely generated A-module and consequently F admits a finite presentation.

#### Proposition 12 {#ac-i-s3-prop-12 .statement}

*Let B be a ring and A a commutative subring of the centre of B such that B is a faithfully flat A-module. For an A-module F to be projective and finitely generated, it is necessary and sufficient that $B \otimes_A F$ be a finitely generated projective left B-module.*

The condition is obviously necessary without any hypothesis on A or B (*Algebra*, Chapter II, \S 5, no. 1, Corollary to Proposition 4); we prove that it is sufficient. If a finitely generated projective module admits a finite presentation (\S 2, no. 8, Lemma 8), the hypothesis implies that F admits a finite presentation by virtue of Proposition 11, hence, for every A-module M, there is a canonical isomorphism

$$
\omega : B \otimes_A \operatorname{Hom}_A(F, M) \to \operatorname{Hom}_B(B \otimes_A F, B \otimes_A M)
$$

(\S 2, no. 10, Proposition 11). Then let $v : M \to M''$ be a *surjective* A-module homomorphism and consider the commutative diagram

$$
\begin{array}{ccc}
B \otimes_A \operatorname{Hom}_A(F, M) & \xrightarrow{\omega} & \operatorname{Hom}_B(B \otimes_A F, B \otimes_A M) \\
1_B \otimes \operatorname{Hom}(1_F, v) \downarrow & & \downarrow \operatorname{Hom}(1_B \otimes F, 1_B \otimes v) \\
B \otimes_A \operatorname{Hom}_A(F, M'') & \xrightarrow{\omega} & \operatorname{Hom}_B(B \otimes_A F, B \otimes_A M'')
\end{array}
$$

As $1_B \otimes v$ is surjective and $B \otimes_A F$ is assumed projective, $\operatorname{Hom}(1_{B \otimes F}, 1_B \otimes v)$ is *surjective* (*Algebra*, Chapter II, \S 2, no. 2, Proposition 4) and so then is $1_B \otimes \operatorname{Hom}(1_F, v)$. But as B is a faithfully flat A-module, $\operatorname{Hom}(1_F, v)$ is itself surjective (no. 1, Proposition 2), hence F is a projective A-module (*Algebra*, Chapter II, \S 2, no. 2, Proposition 4).

### 7. LINEAR EQUATIONS OVER A FAITHFULLY FLAT RING

Let B be a ring and A a subring of B. We shall say that the ordered pair (A, B) has the *linear extension property* if it satisfies the following condition:

(E) Every solution $(y_k)_{1 \leq k \leq n}$, consisting of elements of $B$, of a system of linear equations

$$
\sum_{k=1}^n y_k c_{ki} = d_i \quad (1 \leq i \leq m)
$$

whose coefficients $c_{ki}$ and right-hand sides $d_i$ belong to $A$, is of the form

$$
y_k = x_k + \sum_{j=1}^p b_j z_{jk} \quad (1 \leq k \leq n)
$$

where $(x_k)$ is a solution of (3) consisting of elements of $A$, the $b_j$ belong to $B$ and each of the $(z_{jk})_{1 \leq k \leq n}$ is a solution of the homogeneous linear system associated with (3), consisting of elements of $A$.

#### Proposition 13 {#ac-i-s3-prop-13 .statement}

Let $A$ be a subring of a ring $B$. For the ordered pair $(A, B)$ to satisfy the linear extension property, it is necessary and sufficient that $B$ be a faithfully flat $A$-module.

The condition is *sufficient*. For, as $B$ is a flat $A$-module, every solution with elements in $B$ of the *homogeneous* linear system associated with (3) is a linear combination with coefficients in $B$ of solutions consisting of elements of $A$ (\S 2, no. 11, Corollary 2, to Proposition 13). The problem then reduces to proving that the existence of a solution of (3) with elements in $B$ implies the existence of *one* solution with elements in $A$. Now if we set

$$
c_k = (c_{ki})_{1 \leq i \leq m} \in A_s^m, \qquad d = (d_i) \in A_s^m,
$$

system (3) is equivalent to the equation $\sum_{k=1}^n y_k \otimes c_k = 1 \otimes \mathrm{din}\, B \otimes_A A_s^m = B_s^m$.

In other words, if $M$ is the sub-$A$-module of $A_s^m$ generated by the $c_k$ $(1 \leq k \leq n)$, the existence of the solution $(y_k)$ of (3) is equivalent (with the identifications made in no. 5) to the relation $d \in BM \cap A_s^m$; but as $BM \cap A_s^m = M$ (no. 5, Proposition 10, (ii)), it implies $d \in M$, that is, the existence of a solution $(x_k)$ of system (3) with elements in $A$.

The condition is *necessary*. For suppose that $(A, B)$ satisfies the linear extension property; we know already that $B$ is a flat right $A$-module (\S 2, no. 11, Corollary 2 to Proposition 13); we prove that, for every left ideal $a$ of $A$, $Ba \cap A = a$, which shows that $B$ is a faithfully flat right $A$-module (no. 5, Proposition 9, (d)). Now, let $x \in Ba \cap A$; there exists by hypothesis $y_i \in B$ and $a_i \in a$ such that $\sum_i y_i a_i = x$; property (E) applied to this linear equation with coefficients and right hand side in $A$ shows that there exist $x_i \in A$ such that $x = \sum_i x_i a_i$, hence $x \in a$.

### Exercises {#ac-i-s3-exercises}

See the [exercises for § 3](exercises/s3/).
