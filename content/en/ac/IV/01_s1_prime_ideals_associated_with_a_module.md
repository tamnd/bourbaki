---
book: ac
book_title: Commutative Algebra
chapter: IV
chapter_title: ASSOCIATED PRIME IDEALS AND PRIMARY DECOMPOSITION
section: 1
section_title: Prime ideals associated with a module
lang: en
source: ac-i-vii
book_pages: 261-267, 286-290
pdf_pages: 0281-0287, 0306-0310
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF ASSOCIATED PRIME IDEALS
      page: 261
      pdf_page: 281
    - "no": 2
      title: LOCALIZATION OF ASSOCIATED PRIME IDEALS
      page: 263
      pdf_page: 283
    - "no": 3
      title: RELATIONS WITH THE SUPPORT
      page: 265
      pdf_page: 285
    - "no": 4
      title: THE CASE OF FINITELY GENERATED MODULES OVER A NOETHERIAN RING
      page: 265
      pdf_page: 285
statements: 24
exercises: 19
content_sha256: 1ed80928e0879cd38edab9973cd115adfa10d290548548ffd7851ca1c83aa9ab
---

## 1. PRIME IDEALS ASSOCIATED WITH A MODULE

### 1. DEFINITION OF ASSOCIATED PRIME IDEALS

#### Definition 1 {#ac-iv-s1-def-1 .statement}

Let M be a module over a ring A. A prime ideal p is said to be associated with M if there exists x ∈ M such that p is equal to the annihilator & x. The set of prime ideals associated with M is denoted by Ass_A(M), or simply Ass(M).

\* Example. Let a be an ideal in the polynomial ring A = \mathbf{C}[X_1, ..., X_n], V the corresponding affine algebraic variety and V_1, ..., V_p the irreducible components of V. If M is taken to be the ring A/a of functions which are regular on V, the set of prime ideals associated with M consists of the ideals of V_1, ..., V_p and in general other prime ideals each of which contains one of the ideals of the V_i. \*

As the annihilator of 0 is A, an element x ∈ M whose annihilator is a prime ideal is necessarily ≠ 0. To say that a prime idea p is associated with M

(*) The results of this chapter depend only on Books I to VI and Chapters I to III of this Book, excluding Chapter I, § 4 and Chapter III, § 5.

amounts to saying that $ M $ contains a submodule *isomorphic to* $ A/p $ (namely $ Ax $, for all $ x \in M $ whose annihilator is $ p $).

If an $ A $-module $ M $ is the union of a family $ (M_i)_{i \in I} $ of submodules, then clearly
$$
\operatorname{Ass}(M) = \bigcup_{i \in I} \operatorname{Ass}(M_i).
$$

#### Proposition 1 {#ac-iv-s1-prop-1 .statement}

*For every prime ideal $ p $ of a ring $ A $ and every submodule $ M \neq 0 $ of $ A/p $, $ \operatorname{Ass}(M) = \{p\} $.*

As the ring $ A/p $ is an integral domain, the annihilator of an element $ \neq 0 $ of $ A/p $ is $ p $.

#### Proposition 2 {#ac-iv-s1-prop-2 .statement}

*Let $ M $ be a module over a ring $ A $. Every maximal element of the set of ideals $ \operatorname{Ann}(x) $ of $ A $, where $ x $ runs through the set of elements $ \neq 0 $ of $ M $, belongs to $ \operatorname{Ass}(M) $.*

Let $ a = \operatorname{Ann}(x) $ ($ x \in M, x \neq 0 $) be such a maximal element; it is sufficient to show that $ a $ is prime. As $ x \neq 0 $, $ a \neq A $. Let $ b, c $ be elements of $ A $ such that $ bc \in a $ and $ c \notin a $. Then $ cx \neq 0 $, $ b \in \operatorname{Ann}(cx) $ and $ a \subset \operatorname{Ann}(cx) $. As $ a $ is maximal, $ \operatorname{Ann}(cx) = a $, whence $ b \in a $, so that $ a $ is prime.

#### Corollary 1 {#ac-iv-s1-prop-2-cor-1 .statement}

*Let $ M $ be a module over a Noetherian ring $ A $. Then the condition $ M \neq \{0\} $ is equivalent to $ \operatorname{Ass}(M) \neq \varnothing $.*

If $ M = \{0\} $, clearly $ \operatorname{Ass}(M) $ is empty (without any hypothesis on $ A $). If $ M \neq \{0\} $, the set of ideals of the form $ \operatorname{Ann}(x) $, where $ x \in M $ and $ x \neq 0 $, is non-empty and consists of ideals $ \# A $; as $ A $ is Noetherian, this set has a maximal element; then it suffices to apply Proposition 2.

#### Corollary 2 {#ac-iv-s1-prop-2-cor-2 .statement}

*Let $ A $ be a Noetherian ring, $ M $ an $ A $-module and $ a $ an element of $ A $. For the homothety on $ M $ with ratio $ a $ to be injective, it is necessary and sufficient that $ a $ belong to no prime ideal associated with $ M $.*

If $ a $ belongs to a prime ideal $ p \in \operatorname{Ass}(M) $, then $ p = \operatorname{Ann}(x) $, where $ x \in M, x \neq 0 $; whence $ ax = 0 $ and the homothety with ratio $ a $ is not injective. Conversely, if $ ax = 0 $ for some $ x \in M $ such that $ x \# 0 $, then $ Ax \# \{0\} $, whence $ \operatorname{Ass}(x) \neq \varnothing $ (Corollary 1). Let $ p \in \operatorname{Ass}(Ax) $; then obviously $ p \in \operatorname{Ass}(M) $ and $ p = \operatorname{Ann}(bx) $, where $ b \in A $; whence $ a \in p $, since $ abx = 0 $.

#### Corollary 3 {#ac-iv-s1-prop-2-cor-3 .statement}

*The set of divisors of zero in a Noetherian ring $ A $ is the union of the ideals $ p \in \operatorname{Ass}(A) $.*

#### Proposition 3 {#ac-iv-s1-prop-3 .statement}

*Let $ A $ be a ring, $ M $ an $ A $-module and $ N $ a submodule of $ N $. Then*
$$
\operatorname{Ass}(N) \subset \operatorname{Ass}(M) \subset \operatorname{Ass}(N) \cup \operatorname{Ass}(M/N).
$$
*The inclusion $ \operatorname{Ass}(N) \subset \operatorname{Ass}(M) $ is obvious. Let $ p \in \operatorname{Ass}(M) $, $ E $ be a submodule of $ M $ isomorphic to $ A/p $ and $ F = E \cap N $. If $ F = \{0\} $, $ E $ is isomorphic to a* submodule of $ M/N $, whence $ p \in \operatorname{Ass}(M/N) $. If $ F \neq \{0\} $, the annihilator of every element $ \neq 0 $ of $ F $ is $ p $ (Proposition 1) and hence $ p \in \operatorname{Ass}(F) \subset \operatorname{Ass}(N) $.

#### Corollary 1 {#ac-iv-s1-prop-3-cor-1 .statement}

*If an A-module $ M $ is the direct sum of a family $ (M_i)_{i \in I} $ of submodules, then* $ \operatorname{Ass}(M) = \bigcup_{i \in I} \operatorname{Ass}(M_i) $.

It may be reduced to the case where $ I $ is finite by means of (1), then to the case where $ \operatorname{Card}(I) = 2 $ by induction on $ \operatorname{Card}(I) $. Then let $ I = \{i, j\} $, where $ i \neq j $; as $ M/M_i $ is isomorphic to $ M_j $, $ \operatorname{Ass}(M) \subset \operatorname{Ass}(M_i) \cup \operatorname{Ass}(M_j) $ (Proposition 3); moreover, $ \operatorname{Ass}(M_i) $ and $ \operatorname{Ass}(M_j) $ are contained in $ \operatorname{Ass}(M) $ (Proposition 3), whence the result.

#### Corollary 2 {#ac-iv-s1-prop-3-cor-2 .statement}

*Let $ M $ be an A-module and $ (Q_i)_{i \in I} $ a finite family of submodules of $ M $. If* $ \bigcap_{i \in I} Q_i = \{0\} $, *then*
$$
\operatorname{Ass}(M) \subset \bigcup_{i \in I} \operatorname{Ass}(M/Q_i).
$$
The canonical mapping $ M \to \bigoplus_{i \in I} (M/Q_i) $ is injective; then it suffices to apply Proposition 3 and its Corollary 1.

#### Proposition 4 {#ac-iv-s1-prop-4 .statement}

*Let $ M $ be an A-module and $ \Phi $ a subset of $ \operatorname{Ass}(M) $. Then there exists a submodule $ N $ of $ M $ such that* $ \operatorname{Ass}(N) = \operatorname{Ass}(M) - \Phi $ *and* $ \operatorname{Ass}(M/N) = \Phi $.

Let $ \mathcal{E} $ be the set of submodules $ P $ of $ M $ such that $ \operatorname{Ass}(P) \subset \operatorname{Ass}(M) - \Phi $. Formula (1) shows that the set $ \mathcal{E} $, ordered by inclusion, is *inductive*; moreover, $ \{0\} \in \mathcal{E} $ and hence $ \mathcal{E} \neq \varnothing $. Let $ N $ be a maximal element of $ \mathcal{E} $. Then $ \operatorname{Ass}(N) \subset \operatorname{Ass}(M) - \Phi $. We shall see that $ \operatorname{Ass}(M/N) \subset \Phi $, which, by Proposition 3, will complete the proof. Let $ p \in \operatorname{Ass}(M/N) $; then $ M/N $ contains a submodule $ F/N $ isomorphic to $ A/p $. By Propositions 1 and 3, $ \operatorname{Ass}(F) \subset \operatorname{Ass}(N) \cup \{p\} $. Since $ N $ is maximal in $ \mathcal{E} $, $ F \notin \mathcal{E} $ and hence $ p \in \Phi $.

### 2. LOCALIZATION OF ASSOCIATED PRIME IDEALS

#### Proposition 5 {#ac-iv-s1-prop-5 .statement}

*Let $ A $ be a ring, $ S $ a multiplicative subset of $ A $, $ \Phi $ the set of prime ideals of $ A $ which do not meet $ S $ and $ M $ an A-module. Then*:
(i) *The mapping* $ p \mapsto S^{-1}p $ *is a bijection of* $ \operatorname{Ass}_A(M) \cap \Phi $ *onto a subset of* $ \operatorname{Ass}_{S^{-1}A}(S^{-1}M) $.
(ii) *If* $ p \in \Phi $ *is a finitely generated ideal and* $ S^{-1}p \in \operatorname{Ass}_{S^{-1}A}(S^{-1}M) $, *then* $ p \in \operatorname{Ass}_A(M) $.

Recall (Chapter II, § 2, no. 5, Proposition 11) that the mapping $ p \mapsto S^{-1}p $ is a bijection of $ \Phi $ onto the set of prime ideals of $ S^{-1}A $. If $ p \in \operatorname{Ass}_A(M) \cap \Phi $, $ p $ is the annihilator of a monogenous submodule $ N $ of $ M $; then $ S^{-1}p $ is the annihilator of the monogenous submodule $ S^{-1}N $ of $ S^{-1}M $ (Chapter II, § 2, no. 4, formula (9)) and hence $ S^{-1}\mathfrak{p} \in \mathrm{Ass}_{S^{-1}A}(S^{-1}M) $. Conversely, suppose that $ \mathfrak{p} \in \Phi $ is finitely generated and such that $ S^{-1}\mathfrak{p} $ is associated with $ S^{-1}M $; then there exists $ x \in M $ and $ t \in S $ such that $ S^{-1}\mathfrak{p} $ is the annihilator of $ x/t $. Let $ (a_i)_{1 \leq i \leq n} $ be a system of generators of $ \mathfrak{p} $; then $ (a_i/1)(x/t) = 0 $ and hence there exists $ s_i \in S $ such that $ s_i a_i x = 0 \ (1 \leq i \leq n) $. Let us write $ s = s_1 s_2 \ldots s_n $; for all $ a \in \mathfrak{p} $, $ s a x = 0 $, whence $ p \subset \mathrm{Ann}(s x) $; on the other hand, if $ b \in A $ satisfies $ b s x = 0 $, then $ b/1 \in S^{-1}\mathfrak{p} $ by definition, whence $ b \in \mathfrak{p} $. Then $ \mathfrak{p} = \mathrm{Ann}(s x) $ and $ \mathfrak{p} \in \mathrm{Ass}_A(M) $.

#### Corollary {#ac-iv-s1-n2-cor-1 .statement}

*If the ring A is Noetherian, the mapping $ \mathfrak{p} \mapsto S^{-1}\mathfrak{p} $ is a bijection of $ \mathrm{Ass}_A(M) \cap \Phi $ onto $ \mathrm{Ass}_{S^{-1}A}(S^{-1}M) $.*

If A is not Noetherian, the mapping $ p \mapsto S^{-1}p $ of $ \mathrm{Ass}_A(M) \cap \Phi $ to $ \mathrm{Ass}_{S^{-1}A}(S^{-1}M) $ is not necessarily surjective (Exercise 1).

#### Proposition 6 {#ac-iv-s1-prop-6 .statement}

*Let A be a Noetherian ring, M an A-module, S a multiplicative subset of A and Y the set of elements of $ \mathrm{Ass}_A(M) $ which do not meet S. Then the kernel N of the canonical mapping $ M \to S^{-1}M $ is the unique submodule of M which satisfies the relations*

$$
\mathrm{Ass}(N) = \mathrm{Ass}(M) - \Psi, \quad \mathrm{Ass}(M/N) = \Psi.
$$

By Proposition 4 of no. 1, there exists a submodule $ N' $ of M which satisfies the relations $ \mathrm{Ass}(N') = \mathrm{Ass}(M) - Y $ and $ \mathrm{Ass}(M/N') = \Psi $. We need to prove $ N = N' $. Consider the commutative diagram

$$
\begin{array}{ccc}
M & \xrightarrow{p} & M/N' \\
|u| & & |v| \\
S^{-1}M & \xrightarrow{S^{-1}p} & S^{-1}(M/N')
\end{array}
$$

where $ p, u, v $ are the canonical homomorphisms. We shall show that $ S^{-1}p $ and $ v $ are injective, which will prove that $ u $ and $ p $ have the same kernel and hence $ N = N' $.

As $ \mathrm{Ass}(N') \cap \Psi = \varnothing $, every element of $ \mathrm{Ass}(N') $ meets S. Then $ \mathrm{Ass}_{S^{-1}A}(S^{-1}N') = \varnothing $ (Corollary to Proposition 5), whence $ S^{-1}N' = \{0\} $ (no. 1, Corollary 1 to Proposition 2), which proves that $ S^{-1}p $ is injective (Chapter II, §2, no. 4, Theorem 1). On the other hand, if $ x $ belongs to the kernel K of $ v $, then $ \mathrm{Ann}(x) \cap S \neq \varnothing $ (Chapter II, §2, no. 2, Proposition 4); hence $ \mathrm{Ass}(K) = \varnothing $ since $ \mathrm{Ass}(K) \subset \mathrm{Ass}(M/N') = \Psi $; we deduce that $ K = \{0\} $ (no. 1, Corollary 1 to Proposition 2) and $ v $ is injective.

### 3. RELATIONS WITH THE SUPPORT

Let M be a module over a ring A. Recall that the set of prime ideals $ \mathfrak{p} $ of A such that $ M, \neq 0 $ is called the support of M and is denoted by $ \operatorname{Supp}(M) $ (Chapter II, § 4, no. 4, Definition 5).

#### Proposition 7 {#ac-iv-s1-prop-7 .statement}

Let A be a ring and M an A-module.

(i) Every prime ideal $ \mathfrak{p} $ of A containing an element $ \in \operatorname{Ass}(M) $ belongs to $ \operatorname{Supp}(M) $.

(ii) Conversely, if A is Noetherian, every ideal $ \mathfrak{p} \in \operatorname{Supp}(M) $ contains an element $ \in \operatorname{Ass}(M) $.

If $ \mathfrak{p} $ contains an element $ q $ of $ \operatorname{Ass}(M) $, then $ q \cap (A - \mathfrak{p}) = \varnothing $ and hence, if we write $ S = A - \mathfrak{p} $, $ S^{-1}\mathfrak{p} $ is a prime ideal associated with $ S^{-1}M = M $, (no. 2, Proposition 5) and *a fortiori* $ M, \# 0 $, hence $ \mathfrak{p} \in \operatorname{Supp}(M) $. Conversely, if A is Noetherian, so is A, (Chapter II, § 2, no. 4, Corollary 2 to Proposition 10). If $ M_{\mathfrak{p}} \neq 0 $, then $ \operatorname{Ass}_{A_{\mathfrak{p}}}(M_{\mathfrak{p}}) \neq 0 $ (no. 1, Corollary 1 to Proposition 2) and hence there exists $ q \in \operatorname{Ass}_A(M) $ such that $ q \cap (A - \mathfrak{p}) = \varnothing $ (no. 2, Corollary to Proposition 5).

#### Corollary 1 {#ac-iv-s1-prop-7-cor-1 .statement}

If M is a module over a Noetherian ring, then $ \operatorname{Ass}(M) \subset \operatorname{Supp}(M) $ and these two sets have the same minimal elements.

#### Corollary 2 {#ac-iv-s1-prop-7-cor-2 .statement}

The nilradical of a Noetherian ring A is the intersection of the ideals $ \mathfrak{p} \in \operatorname{Ass}(A) $.

We know that the nilradical of A is the intersection of the minimal elements of $ \operatorname{Spec}(A) = \operatorname{Supp}(A) $ (Chapter II, § 2, no. 6, Proposition 13).

### 4. THE CASE OF FINITELY GENERATED MODULES OVER A NOETHERIAN RING

#### Theorem 1 {#ac-iv-s1-thm-1 .statement}

Let A be a Noetherian ring and M a finitely generated A-module. There exists a composition series $ (M_i)_{0 \leq i \leq n} $ of M such that, for $ 0 \leq i \leq n - 1 $, $ M_i / M_{i+1} $ is isomorphic to $ A / \mathfrak{p}_i $, where $ \mathfrak{p}_i $ is a prime ideal of A.

Let $ \mathcal{G} $ be the set of submodules of M which have a composition series with the property of the statement. As $ \mathcal{G} $ is non-empty (for $ \{0\} $ belongs to $ \mathcal{G} $) and M is Noetherian, $ \mathcal{G} $ has a maximal element N. If $ M \neq N $, then $ M/N \neq 0 $ and hence $ \operatorname{Ass}(M/N) \neq \varnothing $ (no. 1, Corollary 1 to Proposition 2); $ M/N $ therefore contains a submodule $ N'/N $ isomorphic to an A-module of the form $ A/\mathfrak{p} $, where $ \mathfrak{p} $ is prime; then by definition $ N' \in \mathcal{G} $, which contradicts the maximal character of N. Then necessarily $ N = M $.

#### Theorem 2 {#ac-iv-s1-thm-2 .statement}

Let M be a finitely generated module over a Noetherian ring A and $ (M_i)_{0 \leq i \leq n} $ a composition series of M such that, for $ 0 \leq i \leq n - 1 $, $ M_i / M_{i+1} $ is isomorphic to $ A / \mathfrak{p}_i $ where $ \mathfrak{p}_i $ is a prime ideal of A. Then

(4)
$$
\operatorname{Ass}(M) \subset \{\mathfrak{p}_0, \ldots, \mathfrak{p}_{n-1}\} \subset \operatorname{Supp}(M);
$$

the minimal elements of these three sets are the same and coincide with the minimal elements of the set of prime ideals containing Ann(M).

The inclusion Ass(M) $ \subset \{p_0, \ldots, p_{n-1}\} $ follows immediately from Propositions 1 and 3 of no. 1. For $ 0 \leq i \leq n - 1 $,

$$
p_i \in \operatorname{Supp}(A/p_i) = \operatorname{Supp}(M_i/M_{i+1})
$$

(Chapter II, § 4, no. 4, Example), whence $ p_i \in \operatorname{Supp}(M_i) \subset \operatorname{Supp}(M) $ (Chapter II, § 4, no. 4, Proposition 16), which shows the inclusion

$$
\{p_0, \ldots, p_{n-1}\} \subset \operatorname{Supp}(M).
$$

Corollary 1 to Proposition 7 of no. 3 shows that Ass(M) and Supp(M) have the same minimal elements and (4) shows that these are just the minimal elements of $ \{p_0, \ldots, p_{n-1}\} $. The last assertion then follows from Chapter II, § 4, no. 4, Proposition 17.

#### Corollary {#ac-iv-s1-n4-cor-1 .statement}

*If M is a finitely generated module over a Noetherian ring A, Ass(M) is finite.*

Under the conditions of Theorem 2, the set $ \{p_0, \ldots, p_{n-1}\} $ is not necessarily determined uniquely by M; in particular it may be distinct from Ass(M) (Exercise 6).

#### Proposition 8 {#ac-iv-s1-prop-8 .statement}

*Let A be a Noetherian ring, a an ideal of A and M a finitely generated A-module. The following conditions are equivalent:*

(a) *there exists an element x $ \# O $ of M such that $ ax = 0 $.*
(b) *for all $ a \in a $, there exists an element x $ \neq O $ of M such that $ ax = 0 $;*
(c) *there exists $ p \in \operatorname{Ass}(M) $ such that $ a \subset p $.*

Clearly (a) implies (b). By virtue of no. 1, Corollary 2 to Proposition 2, condition (b) means that the ideal a is contained in the union of the prime ideals associated with M and hence in one of them since Ass(M) is finite (Chapter 11, § 1, no. 1, Proposition 2); thus (b) implies (c). Finally, if there exists $ p \in \operatorname{Ass}(M) $ such that $ a \subset p $, p is the annihilator of an element $ x \neq 0 $ of M (no. 1, Definition 1) and $ ax = 0 $; thus (c) implies (a).

#### Proposition 9 {#ac-iv-s1-prop-9 .statement}

*Let A be a Noetherian ring, a an ideal of A and M a finitely generated A-module. For there to exist an integer $ n > 0 $ such that $ a^n M = 0 $, it is necessary and sufficient that a be contained in the intersection of the prime ideals associated with M.*

This intersection is also that of the minimal elements of Supp(M) (no. 3, Corollary 1 to Proposition 7) and to say that a is contained in this intersection is equivalent to saying that $ V(a) \supset \operatorname{Supp}(M) $ in the notation of Chapter II, § 4; the conclusion then follows from Chapter 11, § 4, no. 4, Corollary 2 to Proposition 17.

#### Definition 2 {#ac-iv-s1-def-2 .statement}

Given an $ A $-module $ M $, an endomorphism $ u $ of $ M $ is called almost nilpotent if, for all $ x \in M $, there exists an integer $ n(x) > 0 $ such that $ u^{n(x)}(x) = 0 $.

If $ M $ is finitely generated, every almost nilpotent endomorphism is nilpotent.

#### Corollary {#ac-iv-s1-n4-cor-2 .statement}

Let $ A $ be a Noetherian ring. $ M $ an $ A $-module and $ a $ an element of $ A $. For the homomorphism $ a_M : x \mapsto ax $ of $ M $ to be almost nilpotent, it is necessary and sufficient that $ a $ belong to every ideal of $ \operatorname{Ass}(M) $.

The condition of the statement is equivalent to saying that for all $ x \in M $ there exists $ n(x) > 0 $ such that $ (Aa)^{n(x)}(Ax) = 0 $; by Proposition 9 this means also that $ a $ belongs to all the prime ideals associated with the submodule $ Ax $ of $ M $; the corollary then follows from the fact that $ \operatorname{Ass}(M) $ is the union of the $ \operatorname{Ass}(Ax) $ where $ x $ runs through $ M $ (no. 1, formula (1)).

#### Proposition 10 {#ac-iv-s1-prop-10 .statement}

Let $ A $ be a Noetherian ring, $ E $ a finitely generated $ A $-module and $ F $ an $ A $-module. Then

$$
\operatorname{Ass}(\operatorname{Hom}_A(E, F)) = \operatorname{Ass}(F) \cap \operatorname{Supp}(E).
$$

By hypothesis, $ E $ is isomorphic to an $ A $-module of the form $ A^n/R $, hence $ \operatorname{Hom}_A(E, F) $ is isomorphic to a submodule of $ \operatorname{Hom}_A(A^n, F) $ and the latter is isomorphic to $ F^n $; now, $ \operatorname{Ass}(F^n) = \operatorname{Ass}(F) $ (no. 1, Corollary 1 to Proposition 3); thus $ \operatorname{Ass}(\operatorname{Hom}_A(E, F)) \subset \operatorname{Ass}(F) $. On the other hand,

$$
\operatorname{Supp}(\operatorname{Hom}_A(E, F)) \subset \operatorname{Supp}(E):
$$

for every prime ideal $ p $ of $ A $, $ \operatorname{Hom}_{A_p}(E_p, F_p) $ is isomorphic to $ (\operatorname{Hom}_A(E, F))_p $ (Chapter 11, § 2, no. 7, Proposition 19), whence our assertion immediately; then we conclude from Theorem 2 that

$$
\operatorname{Ass}(\operatorname{Hom}_A(E, F)) \subset \operatorname{Supp}(E).
$$

Conversely, let $ p $ be a prime ideal of $ A $ belonging to $ \operatorname{Ass}(F) \cap \operatorname{Supp}(E) $. By definition, $ F $ contains a submodule isomorphic to $ A/p $. On the other hand, since $ E $ is finitely generated and $ E, \neq 0 $, we know that there exists a homomorphism $ w \neq 0 $ from $ E $ to $ A/p $ (Chapter II, § 4, no. 4, Proposition 20). As there exists an injective homomorphism $ j $ from $ A/p $ to $ F $, $ j \circ w \in \operatorname{Hom}(E, F) $ and $ j \circ w \neq 0 $. On the other hand, the relation $ aw = 0 $ for some $ a \in A $ is equivalent to $ a \in p $, the annihilator of every element $ \neq 0 $ of $ A/p $ being $ p $; then certainly $ p \in \operatorname{Ass}(\operatorname{Hom}_A(E, F)) $.

### Exercises {#ac-iv-s1-exercises}

See the [exercises for § 1](exercises/s1/).
