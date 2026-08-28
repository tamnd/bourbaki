---
book: ac
book_title: Commutative Algebra
chapter: IV
chapter_title: ASSOCIATED PRIME IDEALS AND PRIMARY DECOMPOSITION
section: 2
section_title: Primary decomposition
lang: en
source: ac-i-vii
book_pages: 267-282, 290-301
pdf_pages: 0287-0302, 0310-0321
extraction: ocr
subsections:
    - "no": 1
      title: PRIMARY S BMODULES
      page: 267
      pdf_page: 287
    - "no": 2
      title: THE EXISTENCE OF A PRIMARY DECOMPOSITION
      page: 270
      pdf_page: 290
    - "no": 3
      title: UNIQUENESS PROPERTIES IN THE PRIMARY DECOMPOSITION
      page: 270
      pdf_page: 290
    - "no": 4
      title: THE LOCALIZATION OF A PRIMARY DECOMPOSITION
      page: 272
      pdf_page: 292
    - "no": 5
      title: RINGS AND MODULES OF FINITE LENGTH
      page: 274
      pdf_page: 294
    - "no": 6
      title: PRIMARY DECOMPOSITION AND EXTENSION OF SCALARS
      page: 279
      pdf_page: 299
statements: 39
exercises: 28
content_sha256: 9353d19272573d950f92fba8db2374013f868c6b8d590a53b7b8f6262334c6e8
---

## 2. PRIMARY DECOMPOSITION

### 1. PRIMARY S BMODULES

#### Proposition 1 {#ac-iv-s2-prop-1 .statement}

Let $A$ be a Noetherian ring and $M$ an $A$-module. The following conditions are equivalent:
(a) $\operatorname{Ass}(M)$ is reduced to a single element.

(b) $M \neq 0$ and every homothety of $M$ is either injective or almost nilpotent ($§ 1$, no. 4). *If* these conditions are fulfilled and $p$ is the set of $a \in A$ such that the homothety $a_M$ is almost nilpotent, then $\operatorname{Ass}(M) = \{p\}$.

This follows immediately from $§ 1$, no. 4, Corollary to Proposition 9 and no. 1, Corollary 2 to Proposition 2.

#### Definition 1 {#ac-iv-s2-def-1 .statement}

*Let $A$ be a Noetherian ring, $N$ an $A$-module and $Q$ a submodule of $N$. *If* the module $M = N/Q$ satisfies the conditions of Proposition 1, $Q$ is called *p-primary with respect to* $N$ (or *in* $N$).

When there is no ambiguity, we shall simply say that $Q$ is "p-primary" or "primary"; clearly for every submodule $N' \neq Q$ of $N$ containing $Q$, $Q$ is p-primary in $N'$.

Definition 1 applies in particular to the case $N = A$; the submodules of $N$ are then the *ideals* of $A$ and hence an ideal $q$ of $A$ is called *primary* if $\operatorname{Ass}(A/q)$ has a single element or, what amounts to the same, if $A \neq q$ and every divisor of zero in the ring $A/q$ is *nilpotent*. If $q$ is p-primary, it follows from Definition 1 that $p$ is the *radical* (Chapter II, $§ 2$, no. 6) of the ideal $q$.

#### Remark {#ac-iv-s2-n1-rem-1 .statement}

Let $q$ be a p-primary submodule of an $A$-module $N$. If $N/Q$ is *finitely generated*, there exists an integer $k > 0$ such that $p^k N \subset Q$ by $§ 1$, no. 4, Proposition 9.

*Examples*

#### Example 1 {#ac-iv-s2-n1-exa-1 .statement}

If $p$ is a prime ideal of $A$, $p$ is p-primary ($§ 1$, no. 1, Proposition 1).

#### Example 2 {#ac-iv-s2-n1-exa-2 .statement}

Let $q$ be an ideal of $A$ such that there exists *a single* prime ideal $m$ (necessarily maximal) containing $q$; then, if $M$ is an $A$-module such that $qM \neq M$, $qM$ is *m-primary* with respect to $M$. For every element of $\operatorname{Ass}(M/qM)$ contains $q$, hence is equal to $m$ and $\operatorname{Ass}(M/qM) \neq 0$ ($§ 1$, no. 1, Corollary 1 to Proposition 2). In particular $q$ is an *m-primary* ideal in $A$.

#### Example 3 {#ac-iv-s2-n1-exa-3 .statement}

Let $m$ be a *maximal* ideal of $A$; the m-primary ideals are then the ideals $q$ of $A$ for which there exists an integer $n \geq 1$ such that $m^n \subset q \subset m$. For if $m^n \subset q \subset m$, $m$ is the only prime ideal containing $q$ (Chapter 11, $§ 1$, no. 1, Corollary to Proposition 1) and the conclusion follows from *Example 2*; conversely, if $q$ is m-primary, $m$ is the radical of $q$ and there therefore exists $n \geq 1$ such that $m^n \subset q$ (Chapter II, $§ 2$, no. 6, Proposition 15).

#### Example 4 {#ac-iv-s2-n1-exa-4 .statement}

In a *principal ideal domain* $A$, the primary ideals are $(0)$ and the ideals of the form $Ap^n$, where $p$ is an extremal element and $n \geq 1$; this follows immediately from *Example 3*.

#### Example 5 {#ac-iv-s2-n1-exa-5 .statement}

The powers of any prime ideal are not necessarily primary ideals (Exercise 1). On the other hand, there exist primary ideals which are not powers of prime ideals (Exercise 1).

#### Proposition 2 {#ac-iv-s2-prop-2 .statement}

Let M be a module over a Noetherian ring A, p a prime ideal of A and $(\mathcal{Q}_i)_{i \in I}$ a non-empty finite family of submodules of M which are p-primary with respect to M. Then $\bigcap_{i \in I} \mathcal{Q}_i$ is p-primary with respect to M.

$M / (\bigcap_{i \in I} \mathcal{Q}_i)$ is isomorphic to a submodule $\neq 0$ of the direct sum $\bigoplus_{i \in I} (M / \mathcal{Q}_i)$. Now

$$
\operatorname{Ass}\left( \bigoplus_{i \in I} (M / \mathcal{Q}_i) \right) = \bigcup_{i \in I} \operatorname{Ass}(M / \mathcal{Q}_i) = \{p\}
$$

(§ 1, no. 1, Corollary 1 to Proposition 3). Hence $\operatorname{Ass}\left(M / (\bigcap_{i \in I} \mathcal{Q}_i)\right) = \{p\}$ (§ 1, no. 1, Proposition 3 and Corollary 1 to Proposition 2).

#### Proposition 3 {#ac-iv-s2-prop-3 .statement}

Let A be a Noetherian ring, S a multiplicative subset of A, p a prime ideal of A, M an A-module, N a submodule of M and $i = i_A^S$ the canonical mapping of M to $S^{-1}M$.

(i) Suppose that $p \cap S \neq \varnothing$. If N is p-primary with respect to M, then $S^{-1}N = S^{-1}M$.

(ii) Suppose that $p \cap S = \varnothing$. For N to be p-primary with respect to M, it is necessary and sufficient that N be of the form $i_1(N')$, where $N'$ is a sub-$S^{-1}A$-module of $S^{-1}M$ which is $(S^{-1}p)$-primary with respect to $S^{-1}M$; then $N' = S^{-1}N$.

(i) If $p \cap S \neq \varnothing$ and N is p-primary with respect to M, then

$$
\operatorname{Ass}_{S^{-1}A}(S^{-1}(M/N)) = \varnothing
$$

(§ 1, no. 2, Corollary to Proposition 5) and hence $S^{-1}(M/N) = 0$ (§ 1, no. 1, Corollary 1 to Proposition 2), whence $S^{-1}M/S^{-1}N = 0$.

(ii) Suppose that $p \cap S = \varnothing$. If N is p-primary with respect to M, then $\operatorname{Ass}_{S^{-1}A}(S^{-1}(M/N)) = \{S^{-1}p\}$ (§ 1, no. 2, Corollary to Proposition 5) and hence the submodule $N' = S^{-1}N$ of $S^{-1}M$ is $(S^{-1}p)$-primary; moreover, if $s \in S$ and $m \in M$ are such that $sm \in N$, then $m \in N$, for the homothety with ratio s in M/N is injective, whence $N = i_1(N')$ (Chapter II, § 2, no. 4, Proposition 10). Conversely, let $N'$ be a submodule of $S^{-1}M$ which is $(S^{-1}p)$-primary with respect to $S^{-1}M$; let us write $N = i_1(N')$; then $N' = S^{-1}N$ (Chapter II, § 2, no. 4, Proposition 10) and $\operatorname{Ass}_{S^{-1}A}(S^{-1}(M/N)) = \operatorname{Ass}_{S^{-1}A}((S^{-1}M)/N') = \{S^{-1}p\}$. As the canonical mapping $M/N \to S(M/N)$ is injective, no prime ideal of A associated with M/N meets S (§ 1, no. 2, Proposition 6); it follows that $\operatorname{Ass}(M/N) = \{p\}$ (§ 1, no. 2, Corollary to Proposition 5), so that N is p-primary with respect to M.

### 2. THE EXISTENCE OF A PRIMARY DECOMPOSITION

#### Definition 2 {#ac-iv-s2-def-2 .statement}

Let $A$ be a Noetherian ring, $M$ an $A$-module and $N$ a submodule of $M$. A finite family $(\mathcal{Q}_i)_{i \in I}$ of submodules of $M$ which are primary with respect to $M$ and such that $N = \bigcap_{i \in I} \mathcal{Q}_i$ is called a primary decomposition of $N$ in $M$.

#### Example {#ac-iv-s2-n2-exa-1 .statement}

Let us take $A = \mathbf{Z}$, $M = \mathbf{Z}$, $N = n\mathbf{Z}$ for some integer $n > 0$. If $n = p_1^{\alpha_1} \cdots p_k^{\alpha_k}$ is the decomposition of $n$ into prime factors,
$$
n\mathbf{Z} = (p_1^{\alpha_1}\mathbf{Z}) \cap \ldots \cap (p_k^{\alpha_k}\mathbf{Z})
$$
is a primary decomposition of $n\mathbf{Z}$ in $\mathbf{Z}$ by Example 4 of no. 1.

By an abuse of language, the relation $N = \bigcap_{i \in I} \mathcal{Q}_i$ is called a primary decomposition of $N$ in $M$. It amounts to the same to say that $\{0\} = \bigcap_{i \in I} (\mathcal{Q}_i/N)$ is a primary decomposition of $\{0\}$ in $M/N$. If $(\mathcal{Q}_i)_{i \in I}$ is a primary decomposition of $N$ in $M$, the canonical mapping from $M/N$ to $\bigoplus_{i \in I} (M/\mathcal{Q}_i)$ is injective. Conversely let $N$ be a submodule of $M$ and $f$ an injective homomorphism from $M/N$ to a finite direct sum $P = \bigoplus_{i \in I} P_i$, where each set $\operatorname{Ass}(P_i)$ is reduced to a single element $p_i$; let $f_i$ be the homomorphism $M/N \to P_i$ obtained by taking the composition off with the projection $P \to P_i$, and let $Q_i/N$ be the kernel off.; then the $Q_i$ distinct from $M$ are primary with respect to $M$ (no. 1, Definition 1) and $N = \bigcap_{i \in I} Q_i$. Moreover, $\operatorname{Ass}(M/N) \subset \bigcup_{i \in I} \{p_i\}$ by virtue of § 1, no. 1, Proposition 3.

#### Theorem 1 {#ac-iv-s2-thm-1 .statement}

Let $M$ be a finitely generated module over a Noetherian ring and let $N$ be a submodule of $M$. There exists a primary decomposition of $N$ of the form
$$
N = \bigcap_{p \in \operatorname{Ass}(M/N)} Q(p)
$$
where, for all $p \in \operatorname{Ass}(M/N)$, $Q(p)$ is $p$-primary with respect to $M$.

We may replace $M$ by $M/N$ and therefore suppose that $N = 0$. By § 1, no. 4, Corollary to Theorem 2, $\operatorname{Ass}(M)$ is finite; by § 1, no. 1, Proposition 4, there exists, for each $p \in \operatorname{Ass}(M)$, a submodule $Q(p)$ of $M$ such that $\operatorname{Ass}(M/Q(p)) = \{p\}$ and $\operatorname{Ass}(Q(p)) = \operatorname{Ass}(M) - \{p\}$. Let us write $P = \bigcap_{p \in \operatorname{Ass}(M)} Q(p)$; for all $p \in \operatorname{Ass}(M)$, $\operatorname{Ass}(P) \subset \operatorname{Ass}(Q(p))$ and hence $\operatorname{Ass}(P) = \varnothing$, which implies $P = 0$ (§ 1, no. 1, Corollary 1 to Proposition 2) and therefore proves the theorem.

### 3. UNIQUENESS PROPERTIES IN THE PRIMARY DECOMPOSITION

#### Definition 3 {#ac-iv-s2-def-3 .statement}

Let $M$ be a module over a Noetherian ring and $N$ a submodule of $M$. A primary decomposition $N = \bigcap_{i \in I} Q_i$ of $N$ in $M$ is called reduced if the following conditions are fulfilled:

(a) *there exists no index* $i \in I$ *such that* $\bigcap_{j \neq i} Q_j \subset Q_i;$

(b) *if* $\operatorname{Ass}(M/Q_i) = \{p_i\}$, *the* $p_i$ (*i* $\in I$) *are distinct*.

From every primary decomposition $N = \bigcap_{i \in I} Q_i$ of $N$ in $M$ a *reduced* primary decomposition of $M$ in $N$ can be deduced as follows: let $J$ be a minimal element of the set of subsets $I'$ of $I$ such that $N = \bigcap_{i \in I'} Q_i$. Clearly $(Q_i)_{i \in J}$ satisfies condition (a). Then let $\Phi$ be the set of $p_i$ for $i \in J$; for all $p \in \Phi$, let $H(p)$ be the set of $i \in J$ such that $p_i = p$ and let $Q(p) = \bigcap_{i \in H(p)} Q_i$; it follows from Proposition 2 of no. 1 that $Q(p)$ is $p$-primary with respect to $M$; further $N = \bigcap_{p \in \Phi} Q(p)$ and the family $Q((p))_{p \in \Phi}$ is therefore a reduced primary decomposition of $N$ in $M$.

We shall see that the primary decomposition defined in the proof of Theorem 1 of no. 2 is *reduced*; this follows from the following proposition:

#### Proposition 4 {#ac-iv-s2-prop-4 .statement}

*Let* $M$ *be a module over a Noetherian ring, N a submodule of M, $N = \bigcap_{i \in I} Q_i$ *a primary decomposition of N in M and, for all* $i \in I$, *let* $\{p_i\} = \operatorname{Ass}(M/Q_i)$. *For this decomposition to be reduced, it is necessary and sufficient that the* $p_i$ *be distinct and belong to* $\operatorname{Ass}(M/N)$; *then*

(2)
$$
\operatorname{Ass}(M/N) = \bigcup_{i \in I} \{p_i\}
$$

(3)
$$
\operatorname{Ass}(Q_i/N) = \bigcup_{j \neq i} \{p_j\} \quad \text{for all } i \in I.
$$

If the condition of the statement is fulfilled, $N = \bigcap_{j \neq i} Q_j$ cannot hold, for we would deduce that $\operatorname{Ass}(M/N) \subset \bigcup_{j \neq i} \{p_j\}$ (§ 1, no. 1, Corollary 2 to Proposition 3) contrary to the hypothesis; the primary decomposition $(Q_i)_{i \in I}$ of $N$ is then certainly reduced. Conversely, $\operatorname{Ass}(M/N) \subset \bigcup_{i \in I} \{p_i\}$ always holds (§ 1, no. 1, Corollary 2 to Proposition 3); on the other hand, for all $i \in I$, let us write $P_i = \bigcap_j Q_j$; then $P_i \cap Q_i = N$ and $P_i \neq N$ if $(Q_i)_{i \in I}$ is reduced, hence $P_i/N$ is non-zero and is isomorphic to the submodule $(P_i + Q_i)/Q_i$ of $M/Q_i$, whence $\{p_i\} = \operatorname{Ass}(P_i/N)$ (§ 1, no. 1, Proposition 3 and Corollary 1 to Proposition 2); as $P_i/N \subset M/N, p_i \in \operatorname{Ass}(M/N)$, which completes the proof of the necessity of the condition in the statement and formula (2). Finally, as $N = \bigcap_{j \neq i} (Q_j \cap Q_i), \operatorname{Ass}(Q_i/N) \subset \bigcup_{j \neq i} \operatorname{Ass}(Q_i/(Q_j \cap Q_i))$ (§ 1, no. 1, Corollary 2 to Proposition 3); but $Q_i/(Q_j \cap Q_i)$ is isomorphic to the submodule $(Q_i + Q_j)/Q_j$ of $M/Q_j$, hence $\operatorname{Ass}(Q_i/(Q_j \cap Q_i)) \subset \{p_j\}$ and
$$
\operatorname{Ass}(Q_i/N) \subset \bigcup_{j \neq i} \{p_j\};
$$

#### Corollary {#ac-iv-s2-n3-cor-1 .statement}

Let $A$ be a Noetherian ring, $M$ an $A$-module, $N$ a submodule of $M$ and $(Q_i)_{i \in I}$ a primary decomposition of $N$ in $M$. Then $\mathrm{Card}(I) \geq \mathrm{Card}(\mathrm{Ass}(M/N))$; for $(Q_i)_{i \in I}$ to be a reduced primary decomposition, it is necessary and sufficient that $\mathrm{Card}(I) = \mathrm{Card}(\mathrm{Ass}(M/N))$.

It follows from the remarks preceding Proposition 4 that there exists a reduced primary decomposition $(R_j)_{j \in J}$ of $N$ in $M$ such that $\mathrm{Card}(J) \leq \mathrm{Card}(I)$; the first assertion then follows from the second and the latter is a consequence of Proposition 4.

#### Proposition 5 {#ac-iv-s2-prop-5 .statement}

Let $A$ be a Noetherian ring, $M$ an $A$-module, $N$ a submodule of $M$, $N = \bigcap_{i \in I} Q_i$ a reduced primary decomposition of $N$ in $M$ and, for all $i \in I$, let $\{p_i\} = \mathrm{Ass}(M/Q_i)$. If $p_i$ is a minimal element of $\mathrm{Ass}(M/N)$, $Q_i$ is equal to the saturation on $N$ with respect to $p_i$ (Chapter 11, § 2, no. 4) (cf. Exercise 2).

We can obviously restrict our attention to the case where $N = 0$, replacing if need be $M$ by $M/N$. If $p_i$ is minimal in $\mathrm{Ass}(M)$, the set of elements of $\mathrm{Ass}(M)$ which do not meet $A - p_i$ reduces to $p_i$; the proposition then follows from formula (3) above and § 1, no. 2, Proposition 6, the kernel of the canonical mapping $M \to M_0$, being equal to the saturation of 0 with respect to $p_i$ (Chapter 11, § 2, no. 4).

#### Remark {#ac-iv-s2-n3-rem-1 .statement}

The prime ideals $p_i \in \mathrm{Ass}(M/N)$ which are not minimal elements of this set are sometimes called the *immersed* prime ideals associated with $M/N$; if $M/N$ is finitely generated, for $p_0 \in \mathrm{Ass}(M/N)$ to be immersed, it is necessary and sufficient that $V(p_0)$ *be not* an irreducible component of $\mathrm{Supp}(M/N)$ (Chapter II, § 4, no. 3, Corollary 2 to Proposition 14); if $(Q(p))_{p \in \mathrm{Ass}(M/N)}$ and $(Q'(p))_{p \in \mathrm{Ass}(M/N)}$ are two reduced primary decompositions of $N$ in $M$, it may be that $Q'(p_0) \neq Q(p_0)$ (Exercise 24 (c)); a *canonical* reduced primary decomposition of $N$ in $M$ may always be defined by imposing supplementary condition on the primary submodules which appear in it (Exercise 4).

### 4. THE LOCALIZATION OF A PRIMARY DECOMPOSITION

Given a submodule $N$ of a module $M$ over a Noetherian ring $A$, to simplify we shall denote by $D_I(M/N)$, in this no., the set of reduced primary decompositions of $N$ in $M$ whose indexing set is $I$ (equipotent to $\mathrm{Ass}(M/N)$).

#### Proposition 6 {#ac-iv-s2-prop-6 .statement}

Let $A$ be a Noetherian ring, $M$ an $A$-module, $N$ a submodule of $M$ and $I = \mathrm{Ass}(M/N)$. Let $S$ be a multiplicative subset of $A$ and $J$ the subset of $I$ consisting of the indices i such that $S \cap p_i = \varnothing$. Let $N'$ be the saturation of $N$ with respect to $S$ in $M$. Then:

(i) *If* $(Q_i)_{i \in I}$ *is an element of* $D_I(M/N)$, *the family* $(Q_i)_{i \in J}$ *is an element of* $D_J(M/N')$ *and the family* $(S^{-1}Q_i)_{i \in J}$ *is an element of* $D_J(S^{-1}M/S^{-1}N)$.

(ii) *The mapping* $(Q_i)_{i \in J} \to (S^{-1}Q_i)_{i \in J}$ *is a bijection of* $D_J(M/N')$ *onto* $D_J(S^{-1}M/S^{-1}N)$.

(iii) *If* $(Q_i)_{i \in J}$ *is an element of* $D_J(M/N')$ *and* $(R_i)_{i \in I}$ *an element of* $D_I(M/N)$, *the family* $(T_i)_{i \in I}$ *such that* $T_i = Q_i$ *for* $i \in J$ *and* $T_i = R_i$ *for* $i \in I - J$ *is an element of* $D_I(M/N)$.

(i) We know (no. 1, Proposition 3) that for $i \in J, S^{-1}Q_i$ is primary for $S^{-1}p_i$ and that for $i \in I - J, S^{-1}Q_i = S^{-1}M$; as $S^{-1}N = \bigcap S^{-1}Q_i$ (Chapter II, § 2, no. 4), then also $S^{-1}N = \bigcap_{i \in J} S^{-1}Q_i$. The $S^{-1}p_i$ for $i \in J$ are distinct and their set is $\operatorname{Ass}(S^{-1}M/S^{-1}N)$ ($§ 1$, no. 2, Corollary to Proposition 5); then (Proposition 4) $(S^{-1}Q_i)_{i \in J}$ is a reduced primary decomposition of $S^{-1}N$. Moreover, $Q_i = (i_M^S)^{-1}(S^{-1}Q_i)$ (no. 1 Proposition 3), hence $N' = (i_M^S)^{-1}(S^{-1}N) = \bigcap_{i \in J} Q_i$ and $(Q_i)_{i \in J}$ is obviously a reduced primary decomposition of $N'$ in $M$.

(ii) *As* $S^{-1}N' = S^{-1}N$, we may replace $N$ by $N'$, that is suppose that $J = I$. Let $(P_i)_{i \in I}$ be a reduced primary decomposition of $S^{-1}N$ in $S^{-1}M$ and let us write $Q_i = (i_M^S)^{-1}(P_i)$; it follows from no. 1, Proposition 3 that $Q_i$ is primary for $p_i$ ($i \in I$) and $(Q_i)_{i \in I}$ is then a reduced primary decomposition of $N$ in $M$ by virtue of no. 3, Corollary to Proposition 4. Finally, as, for all $i \in I$ and every submodule $Q'_i$ of which $M$ is $p_i$-primary with respect to $M, Q'_i = (i_M^S)^{-1}(S^{-1}Q'_i)$ by virtue of no. 1, Proposition 3 and the hypothesis $J = I$, we see that two mappings $D_I(M/N) \to D_I(S^{-1}M/S^{-1}N)$ and $D_I(S^{-1}M/S^{-1}N) \to D_I(M/N)$ have been defined whose compositions are the identities on $D_I(M/N)$ and $D_I(S^{-1}M/S^{-1}N)$, which proves (ii).

(iii) By virtue of (i), $N' = \bigcap_{i \in J} R_i$, whence

$$
N = N' \cap \bigcap_{i \in I - J} R_i = \left( \bigcap_{i \in J} Q_i \right) \cap \left( \bigcap_{i \in I - J} R_i \right)
$$

and it follows immediately from no. 3, Corollary to Proposition 4 that this primary decomposition is reduced.

#### Corollary {#ac-iv-s2-n4-cor-1 .statement}

*The mappings*

$$
D_I(M/N) \to D_J(M/N') \quad \text{and} \quad D_I(M/N) \to D_J(S^{-1}M/S^{-1}N)
$$

*defined in Proposition 6 (i)* *are surjective*.

Proposition 6 (iii) shows that the mapping $D_I(M/N) \to D_J(M/N')$ is surjective and Proposition 6 (ii) then shows that the mapping
$$
D_I(M/N) \to D_J(S^{-1}M/S^{-1}N)
$$
is surjective.

### 5. RINGS AND MODULES OF FINITE LENGTH

If an $A$-module $M$ is of finite length, we shall denote this length by $\operatorname{long}_A(M)$ or $\operatorname{long}(M)$. Recall that every Artinian ring is Noetherian (Algebra, Chapter VIII, § 6, no. 5, Corollary 3 to Proposition 12) and that every finitely generated module over an Artinian ring is of finite length (*loc. cit.*, Corollary 1 to Proposition 12). Moreover, every Artinian integral domain is a field (Algebra, Chapter VIII, § 6, no. 4, Proposition 9).

#### Proposition 7 {#ac-iv-s2-prop-7 .statement}

*Let $M$ be a finitely generated module over a Noetherian ring $A$. The following properties are equivalent:*
(a) $M$ is of finite length.
(b) *Every ideal $p \in \operatorname{Ass}(M)$ is a maximal ideal of $A$.*
(c) *Every ideal $p \in \operatorname{Supp}(M)$ is a maximal ideal of $A$.*

Let $(M_i)_{0 \leq i \leq n}$ be a composition series of $M$ such that, for $0 \leq i \leq n - 1$, $M_i/M_{i+1}$ is isomorphic to $A/p_i$, where $p_i$ is prime ($§ 1$, no. 4, Theorem 1). If $M$ is of finite length, so is each of the $A$-modules $A/p_i$, which implies that each of the rings $A/p_i$ is Artinian; but as $A/p_i$ is an integral domain, it is therefore a field, in other words $p_i$ is maximal; we conclude that (a) implies (b) ($§ 1$, no. 4, Theorem 2). Condition (b) implies (c) by $§ 1$, no. 3, Proposition 7. Finally, if all the ideals of $\operatorname{Supp}(M)$ are maximal, so are the $p_i$ ($§ 1$, no. 4, Theorem 2), hence the $A/p_i$ are simple $A$-modules and $M$ is of finite length, which completes the proof.

#### Corollary 1 {#ac-iv-s2-prop-7-cor-1 .statement}

*For every module of finite length $M$ over a Noetherian Zing $A$, $\operatorname{Ass}(M) = \operatorname{Supp}(M)$.*

Every element of $\operatorname{Supp}(M)$ is then minimal in $\operatorname{Supp}(M)$ and the conclusion follows from $§ 1$, no. 3, Corollary 1 to Proposition 7.

#### Corollary 2 {#ac-iv-s2-prop-7-cor-2 .statement}

*Let $M$ be a finitely generated module over a Noetherian ring $A$ and $p$ a prime ideal of $A$. For $M_p$ to be a non-zero $A_p$-module of finite length, it is necessary and sufficient that $p$ be a minimal element of $\operatorname{Ass}(M)$.*

By $§ 1$, no. 2, Corollary to Proposition 5, $\operatorname{Ass}_{A_p}(M_p)$ is the set of ideals $q_p$, where $q$ runs through the set of ideals of $\operatorname{Ass}(M)$ which are contained in $p$. On the other hand, $p_p$ is the unique maximal ideal of $A_p$; by Proposition 7, for $M_p$ to be an $A_p$-module of finite length, it is necessary and sufficient that no element of $\operatorname{Ass}(M)$ be strictly contained in $p$. On the other hand, for $M_p \neq 0$, it is necessary and sufficient by definition that $p \in \operatorname{Supp}(M)$ (Chapter 11, § 4, no. 4), that is that $p$ contain an element of $\operatorname{Ass}(M)$ ($§ 1$, no. 3, Proposition 7). This proves the corollary.

Remark (1). Let $M$ be a finitely generated module over a Noetherian ring $A$; let $(M_1), \ldots$ be a composition series of $M$ such that, for $0 \leq i \leq n - 1$, $M_i / M_{i+1}$ is isomorphic to $A/p_i$, where $p_i$ is a prime ideal of $A$ ($§ 1$, no. 4, Theorem 1). If $p$ is a minimal element of $\operatorname{Ass}(M)$, the length $\operatorname{long}_{A_p}(M_p)$ is equal to the *number of indices* $i$ such that $p_i = p$. For the $(M_i)_p$ form a composition series of $M$, and $(M_i)_p / (M_{i+1})_p$ is isomorphic to $(A/p_i)_p$ and hence to $\{0\}$ if $p_i \neq p$ (since $p$ is minimal in the set of $p_i$ by $§ 1$, no. 4, Theorem 2) and to $(A/p)_p$ which is a field, if $p_i = p$.

#### Proposition 8 {#ac-iv-s2-prop-8 .statement}

*Let $M$ be a module of finite length over a Noetherian ring $A$.*

(i) *There only exists a single primary decomposition of $\{0\}$ with respect to $M$ indexed by $\operatorname{Ass}(M)$ (necessarily reduced) — let $\{0\} = \bigcap_{p \in \operatorname{Ass}(M)} Q(p)$ be this decomposition, where $Q(p)$ is $p$-primary with respect to $M$.*

(ii) *There exists an integer $n_0$ such that, for all $n \geq n_0$ and all $p \in \operatorname{Ass}(M)$, $Q(p) = p^n M$.*

(iii) *For all $p \in \operatorname{Ass}(M)$, the canonical mapping of $M$ to $M_p$ is surjective and its kernel is $Q(p)$.*

(iv) *The canonical injection of $M$ into $\bigoplus_{p \in \operatorname{Ass}(M)} (M/Q(p))$ is bijective.*

As every element $p \in \operatorname{Ass}(M)$ is minimal in $\operatorname{Ass}(M)$ (Proposition 7), assertion (i) follows from no. 3, Proposition 5. As $M$ is finitely generated, there exists $n_0$ such that $p^n M \subset Q(p)$ for all $p \in \operatorname{Ass}(M)$ and all $n \geq n_0$ (no. 1, *Remark*); but as $p$ is a maximal ideal, $p^n M$ is $p$-primary with respect to $M$ (no. 1, *Examples 2 and 3*) and, as $\bigcap_{p \in \operatorname{Ass}(M)} p^n M = \{0\}$, it follows from (i) that necessarily $p^n M = Q(p)$ for all $p \in \operatorname{Ass}(M)$; whence (ii). As the $p^n$, for $p \in \operatorname{Ass}(M)$, are relatively prime in pairs (Chapter 11, § 1, no. 2, Proposition 3), the canonical mapping $M \to \bigoplus_{p \in \operatorname{Ass}(M)} (M/p^n M)$ is surjective (Chapter 11, § 1, no. 2, Proposition 6), whence (iv). Then $\operatorname{Ass}(Q(p)) = \operatorname{Ass}(M) - \{p\}$ and $\operatorname{Ass}(M/Q(p)) = \{p\}$ (no. 3, Proposition 4); as the elements of $\operatorname{Ass}(M)$ are maximal ideals, $p$ is the only element of $\operatorname{Ass}(M)$ which does not meet $A - p$; $Q(p)$ is therefore the kernel of the canonical mapping $j : M \to M_p$ ($§ 1$, no. 2, Proposition 6). If $s \in A - p$, the homothety of $M/Q(p)$ with ratio $s$ is injective by virtue of the relation $\operatorname{Ass}(M/Q(p)) = \{p\}$ (no. 1, Proposition 1); since $M/Q(p)$ is Artinian, this homothety is bijective (*Algebra*, Chapter VIII, § 1, no. 2, Lemma 3). The canonical mapping $M \to M/Q(p)$ is then written $f \circ j$, where $f : M_p \to M/Q(p)$ is an $A$-homomorphism (Chapter II, § 2, no. 2, Proposition 3); as $\operatorname{Ker}(j) = \operatorname{Ker}(f \circ j) = Q(p)$, $f$ is injective; we conclude that $j$ is surjective and $f$ bijective.

#### Corollary {#ac-iv-s2-n5-cor-1 .statement}

*If M is a module of finite length over a Noetherian ring A, then*

$$
\operatorname{long}_A(M) = \sum_{p \in \operatorname{Ass}(M)} \operatorname{long}_{A_p}(M_p).
$$

This will follow from Proposition 8 (iv) if we prove that

$$
\operatorname{long}_A(M/\mathcal{Q}(p)) = \operatorname{long}_{A_p}(M_p).
$$

Now, it follows from Proposition 1 of no. 1 that for all $s \in A - p$ the homothety with ratio s on $M/\mathcal{Q}(p)$ is injective; the homothety with ratio s on every submodule R of $M/\mathcal{Q}(p)$ is therefore injective and, as R is Artinian, it is bijective (*Algebra*, Chapter VIII, § 2, no. 2, Lemma 3); we conclude that the sub-A-modules of $M/\mathcal{Q}(p)$ are the images under the bijection $f : M, \to M/\mathcal{Q}(p)$ of the sub-A,-modules of M, (Chapter 11, § 2, no. 3), whence our assertion.

#### Proposition 9 {#ac-iv-s2-prop-9 .statement}

*Let A be a Noetherian ring. The following conditions are equivalent :*
(a) *A is Artinian.*
(b) *All the prime ideals $\mathfrak{a}$ in A are maximal ideals.*
(c) *All the elements of Ass(A) are maximal ideals.*

*If these conditions are fulfilled, A has only a finite number of prime ideals, which are all maximal and associated with the A-module A; further, A is a semi-local ring and its Jacobson radical is nilpotent.*

To say that A is Artinian is equivalent to saying that A is an A-module of finite length; hence (a) and (c) are equivalent by Proposition 7. Clearly (b) implies (c). Finally, (a) implies (b) since every Artinian integral domain is a field. The properties (a), (b) and (c) are therefore equivalent.

Suppose they hold. As every prime ideal of A belongs to Supp(A) and every element of Supp(A) contains an element of Ass(A) ($\S$ 1, no. 3, Proposition 7), it follows from (c) that Ass(A) is the set of all prime ideals of A; then A has only a finite number of prime ideals, all of them maximal and associated with the A-module A. This obviously implies that A is semi-local; finally, we know that the Jacobson radical of an Artinian ring is nilpotent (*Algebra*, Chapter VIII, § 6, no. 4, Theorem 3).

*Remark (2)* The conditions of Proposition 9 for a *Noetherian* ring A imply that the spectrum of A is *finite* and *discrete*, every point of Spec(A) being therefore closed (Chapter 11, § 4, no. 3, Corollary 6 to Proposition 11). Conversely, for a *Noetherian* ring A, to say that *every point* $\mathfrak{a}$ of Spec(A) *is closed* means that every prime ideal of A is maximal (*loc. cit.*.) and hence this condition is equivalent to that of Proposition 9.

#### Corollary 1 {#ac-iv-s2-prop-9-cor-1 .statement}

*Every Artinian ring A is isomorphic to the direct composition of a finite family of Artinian local rings.*

It follows from Proposition 9 and Proposition 8 (iii) and (iv) that, if $(\mathfrak{m}_i)_{1 \leq i \leq n}$ is the family of maximal ideals of $A$, the canonical mapping $A \to \prod_i A_{\mathfrak{m}_i}$ is bijective.

Remark (3). This corollary can also be deduced from the fact that $\operatorname{Spec}(A)$ is finite and discrete and Chapter 11, § 4, no. 3, Proposition 15.

#### Corollary 2 {#ac-iv-s2-prop-9-cor-2 .statement}

Let $A$ be a Noetherian ring and $m$ an ideal of $A$. The following conditions are equivalent:

(a) $A$ is a semi-local ring and $m$ is a defining ideal of $A$.
(b) $A$ is a Zariski ring with the $m$-adic topology and $A/m$ is Artinian.

If (a) holds, $A$ is a Zariski ring with the $m$-adic topology (Chapter III, § 3, no. 3, Example 3); further, as by hypothesis $m$ contains a power of the Jacobson radical $r$ of $A$, every prime ideal of $A$ which contains $m$ also contains $r$ (Chapter II, § 1, no. 1, Proposition 1); it is therefore maximal, since $r$ is a finite intersection of maximal ideals (\emph{loc. cit.}); Proposition 9 then shows that $A/m$ is Artinian. Conversely, if (b) holds, every maximal ideal $p$ of $A$ contains the Jacobson radical of $A$ and hence contains $m$ (Chapter III, § 3, no. 3, Proposition 6); as $A/m$ is Artinian, the ideals $p/m$ are finite in number (Proposition 9) and hence $A$ has only a finite number of maximal ideals, which implies that it is semi-local.

#### Corollary 3 {#ac-iv-s2-prop-9-cor-3 .statement}

Let $A, A'$ be two rings and $h$ a homomorphism from $A$ to $A'$. Suppose that $A$ is semi-local and Noetherian and that $A'$ is a finitely generated $A$-module. Then the ring $A'$ is semi-local and Noetherian; if $m$ is a defining ideal of $A$, $mA'$ is a defining ideal of $A'$.

We know that $A'$ is a Zariski ring with the $mA'$-adic topology (Chapter III, § 3, no. 3, Proposition 7). As $A/m$ is Artinian (Corollary 2) and $A'/mA'$ is a finitely generated $(A/m)$-module, $A'/mA'$ is an Artinian ring, hence $A'$ is semi-local and $mA'$ is a defining ideal of $A'$ (Corollary 2).

#### Corollary 4 {#ac-iv-s2-prop-9-cor-4 .statement}

Let $A$ be a complete semi-local Noetherian ring, $m$ a defining ideal of $A$, $E$ a finitely generated $A$-module and $(F_n)$ a decreasing sequence of submodules of $E$ such that $\bigcap_n F_n = 0$. Then, for all $p > 0$, there exists $n > 0$ such that $F_n \subset m^p E$.

As $A$ is a Zariski ring, $E$ is Hausdorff and the $F_n$ are closed under the $m$-adic topology. On the other hand, $E$ is complete (Chapter III, § 2, no. 12, Corollary 1 to Proposition 16). Finally, $E/m^p E$ is a finitely generated module over the ring $A/m^p$, which is Artinian (Corollary 2); then $E/m^p E$ is an Artinian $(A/m^p)$-module and hence an Artinian $A$-module. The corollary then follows from Chapter III, § 2, no. 7, Proposition 8.

#### Corollary 5 {#ac-iv-s2-prop-9-cor-5 .statement}

In a complete semi-local Noetherian ring every decreasing sequence $\phi$ ideals whose intersection is 0 is a filter base which converges to 0.

It is sufficient to apply Corollary 4 to the A-module $\mathbf{A}$.

#### Proposition 10 {#ac-iv-s2-prop-10 .statement}

Let $A$ be a Noetherian ring and $p_1, \ldots, p_n$ the prime ideals associated with the A-module $A$, where $p_i \neq p_j$ for $i \neq j$.

(i) The set $S = \bigcap_{i=1}^n (A - p_i)$ is the set of elements which are not divisors of 0 in $A$.

(ii) If all the $p_i$ are minimal elements of $\operatorname{Ass}(A)$, the total ring of fractions $S^{-1}A$ of $A$ is Artinian.

(iii) If the ring $A$ is reduced, all the $p_i$ are minimal elements of $\operatorname{Ass}(A)$ (and therefore are the minimal elements of $\operatorname{Spec}(A)$) and each of the $A_{p_i}$ is a field; for each index $i$, the canonical homomorphism $S^{-1}A \to A_{p_i}$ (Chapter II, § 2, no. 1, Corollary 1 to Proposition 2) is surjective and its kernel is $S^{-1}p_i$; finally the canonical homomorphism from $S^{-1}A$ to $\prod_{i=1}^n (S^{-1}A/S^{-1}p_i)$ is bijective.

The fact that $S$ is the set of elements which are not divisors of 0 in $\mathbf{A}$ has already been seen (§ 1, no. 1, Corollary 3 to Proposition 2). The prime ideals of $S^{-1}A$ are of the form $S^{-1}p$, where $p$ is a prime ideal of $A$ contained in $\bigcup_{i=1}^n p_i$ (Chapter 11, § 2, no. 5, Proposition 10) that is contained in one of the $p_i$ (Chapter II, § 1, no. 1, Proposition 2). If $p_i$ is a minimal element of $\operatorname{Ass}(A)$, it is a minimal element of $\operatorname{Spec}(A)$ (§ 1, no. 3, Corollary to Proposition 7); if each of the $p_i$ is a minimal element of $\operatorname{Ass}(A)$, we then see that the prime ideals of $S^{-1}A$ are the $S^{-1}p_i$ and they are therefore all maximal, which proves that $S^{-1}A$ is Artinian (Proposition 9).

Suppose finally that the ring $A$ is reduced. Then $\bigcap_{i=1}^n p_i = \{0\}$ (§ 1, no. 3, Corollary 2 to Proposition 7). We deduce that $\{0\} = \bigcap_{i=1}^n p_i$ is a *reduced* primary decomposition of the ideal $\{0\}$ (no. 3, Corollary to Proposition 4); in particular, none of the $p_i$ can contain a $p_j$ of index $j \neq i$ and therefore the $p_i$ are all minimal elements of $\operatorname{Ass}(A)$. The ring $S^{-1}A$ is then Artinian by (ii). The $S^{-1}p_i$ are prime ideals associated with the $S^{-1}A$-module $S^{-1}A$ (§ 1, no. 2, Corollary to Proposition 5) and $\{0\} = S^{-1} \left( \bigcap_{i=1}^n p_i \right) = \bigcap_{i=1}^n S^{-1}p_i$ (Chapter II, § 2, no. 4); as the $S^{-1}p_i$ are distinct, $(S^{-1}p_i)_{1 \leq i \leq n}$ is a reduced primary decomposition of $\{0\}$ in $S^{-1}A$ (no. 3, Corollary to Proposition 4). Proposition 8 then shows that the canonical homomorphismg,: $S^{-1}A \to (S^{-1}A)_{p_i}$ is surjective and has kernel $S^{-1}p_i$ and the canonical homomorphism $S^{-1}A \to \prod_{i=1}^n (S^{-1}A/S^{-1}p_i)$ is bijective. We know moreover that the canonical homomorphism $S^{-1}A \to A$, is composed of g, and an isomorphism $(S^{-1}A)_{S^{-1}p_i} \to A$, (Chapter II, § 2, no. 3, Proposition 7). Finally, it follows from Proposition 8 that $(S^{-1}A)_{S^{-1}p_i}$ is isomorphic to $S^{-1}A/S^{-1}p_i$ and hence is a field since $S^{-1}p_i$ is a maximal ideal.

### 6. PRIMARY DECOMPOSITION AND EXTENSION OF SCALARS

In this no., A and B will denote two rings and we shall consider a ring homomorphism $\rho : A \to B$ which makes $B$ into an A-algebra; recall that, for every B-module F, $\rho_*(F)$ is the commutative group F with the A-module structure defined by $a.y = \rho(a)y$ for all $a \in A, y \in F$.

#### Lemma 1 {#ac-iv-s2-lem-1 .statement}

Let A be a Noetherian ring, $p$ a prime ideal of A, E an A-module whose annihilator contains a power of $p$ and such that $\operatorname{Ass}(E) = \{p\}$ and F a B-module such that $\rho_*(F)$ is a flat A-module. The condition $\mathfrak{P} \in \operatorname{Ass}_B(E \otimes_A F)$ then implies $\rho^{-1}(\mathfrak{P}) = p$.

If n is such that $p^nE = 0$, then $p^nB \subset \operatorname{Ann}(E \otimes_A F)$, whence $p^nB \subset \mathfrak{P}$, which implies $p^n \subset \rho_1(\mathfrak{P})$ and therefore $p \subset \rho_1(\mathfrak{P})$ since $\rho_1(\mathfrak{P})$ is prime. Moreover, if $a \in A - p$, the homothety h with ratio a on E is injective ($§ 1$, no. 1, Corollary 2 to Proposition 2); as $h \otimes 1_F$ is the homothety $h'$ with ratio $\rho(a)$ on $E \otimes_A F$ and $\rho_*(F)$ is flat, $h'$ is injective (Chapter I, § 2, no. 2, Definition 1); this proves that $\rho(a) \notin \mathfrak{P}$, whence $\rho^{-1}(\mathfrak{P}) = p$.

#### Theorem 2 {#ac-iv-s2-thm-2 .statement}

Let $\rho : A \to B$ be a ring homomorphism, E an A-module and F a B-module such that $\rho_*(F)$ is a flat A-module. Then

$$
\operatorname{Ass}_B(E \otimes_A F) \supset \bigcup_{p \in \operatorname{Ass}_A(E)} \operatorname{Ass}_B(F/pF).
$$

When A is Noetherian, the two sides of (5) are equal.

Let $p \in \operatorname{Ass}_A(E)$; by definition there exists an exact sequence

$$
0 \to A/p \to E.
$$

Since F is a flat A-module we derive an exact sequence

$$
0 \to F/pF \to E \otimes_A F
$$

whence $\operatorname{Ass}_B(F/pF) \subset \operatorname{Ass}_B(E \otimes_A F)$, which proves the inclusion (5).

Suppose now that A is Noetherian and let us prove the opposite inclusion.

We proceed in stages:

(i) Suppose first that E is a finitely generated A-module and that Ass_A(E) is reduced to a single element $p$. By § 1, no. 4, Theorem 1 there exists a composition series $(E_i)_{0 \leq i \leq n}$ of E such that $E_i/E_{i+1}$ is isomorphic to $A/p_i$, where $p_i$ is a prime ideal of A; moreover ($§ 1$, no. 4, Theorem 2 and no. 3, Proposition 7) all the $p_i$ contain $p$. As F is a flat A-module, the $E_i \otimes_A F$ form a composition series of $E \otimes_A F$ and $(E_i \otimes_A F)/(E_{i+1} \otimes_A F)$ is identified with
$$
(A/p_i) \otimes_A F = F/p_i F.
$$
Then by virtue of $§ 1$, no. 1, Proposition 3
$$
\operatorname{Ass}_B(E \otimes_A F) \subset \bigcup_{i=0}^{n-1} \operatorname{Ass}_B(F/p_i F).
$$
We know that E is annihilated by a power of $p$ (no. 1, Remark); Lemma 1 then shows that, for all $\mathfrak{P} \in \operatorname{Ass}_B(E \otimes_A F)$, $\rho^{-1}(\mathfrak{P}) = p$. As $F/p_i F$ is isomorphic to $(A/p_i) \otimes_A F$, $\rho^{-1}(\mathfrak{P}') = p_i$ for all $\mathfrak{P}' \in \operatorname{Ass}_B(F/p_i F)$ by Lemma 1, whence $\operatorname{Ass}_B(E \otimes_A F) \cap \operatorname{Ass}(F/p_i F) = \varnothing$ if $p_i \neq p$, which proves the theorem in the case considered.

(ii) Suppose only that E is a finitely generated A-module. Let $p_i$ ($1 \leq i \leq n$) be the elements of $\operatorname{Ass}_A(E)$ and let $\{0\} = \bigcap^n Q_i$ be a corresponding reduced primary decomposition (no. 3); E is then isomorphic to a submodule of the direct sum of the $E_i = E/Q_i$ and, as F is a flat A-module, $E \otimes_A F$ is isomorphic to a submodule of the direct sum of B-modules $E_i \otimes_A F$. We deduce ($§ 1$, no. 1, Proposition 3 and Corollary 1 to Proposition 3) that
$$
\operatorname{Ass}_B(E \otimes_A F) \subset \bigcup_{i=1}^n \operatorname{Ass}_B(E_i \otimes_A F).
$$
But $E_i$ is a finitely generated A-module such that $\operatorname{Ass}_A(E_i)$ is reduced to a single element $p_i$ (no. 1, Definition 1). By (i), $\operatorname{Ass}_B(E_i \otimes_A F) = \operatorname{Ass}_B(F/p_i F)$, whence the theorem in this case.

(iii) *General case.* The B-module $E \otimes_A F$ is the union of the submodules $E' \otimes_A F$, where $E'$ runs through the set of finitely generated submodules of the A-module E. If $\mathfrak{P}$ belongs to $\operatorname{Ass}_B(E \otimes_A F)$, then there exists a finitely generated submodule $E'$ of E such that $\mathfrak{P} \in \operatorname{Ass}_B(E' \otimes_A F)$. By (ii), there exists $p \in \operatorname{Ass}_A(E')$ such that $\mathfrak{P} \in \operatorname{Ass}_B(F/pF)$; as $\operatorname{Ass}_A(E') \subset \operatorname{Ass}_A(E)$, this completes the proof of Theorem 2.

#### Corollary 1 {#ac-iv-s2-thm-2-cor-1 .statement}

*If A is Noetherian and $\mathfrak{P} \in \operatorname{Ass}_B(E \otimes_A F)$, then $\rho^{-1}(\mathfrak{P}) \in \operatorname{Ass}_A(E)$ and $\rho^{-1}(\mathfrak{P})$ is the only prime ideal $p$ of A such that $\mathfrak{P} \in \operatorname{Ass}_B(F/pF)$.*

#### Corollary 2 {#ac-iv-s2-thm-2-cor-2 .statement}

Suppose that $A$ and $B$ are Noetherian and that $B$ is a flat $A$-module. Let $p$ be a prime ideal of $A$, $Q \subset E$ a $p$-primary submodule and $\mathfrak{P}$ a prime ideal of $B$. For $Q \otimes_A B$ to be a $q$-primary submodule of $E \otimes_A B$, it is necessary and sufficient that $pB$ be a 'p-primary ideal' of $B$.

Let us apply Theorem 2 to the $A$-module $E/Q$ and the $B$-module $B$; then $\operatorname{Ass}_A(E/Q) = \{p\}$ and $(E/Q) \otimes_A B$ is isomorphic to $(E \otimes_A B)/(Q \otimes_A B)$ and hence $\operatorname{Ass}_B((E \otimes_A B)/(Q \otimes_A B)) = \operatorname{Ass}_B(B/pB)$. To say that $Q \otimes_A B$ is $\mathfrak{P}$-primary in $E \otimes_A B$ therefore means that $\operatorname{Ass}_B(B/pB)$ is reduced to $\mathfrak{P}$, whence the corollary.

#### Remark {#ac-iv-s2-n6-rem-1 .statement}

Suppose that $A$ and $B$ are Noetherian. Let $\mathfrak{P}$ be a prime ideal of $B$ and let $p = \overline{\rho}^{-1}(\mathfrak{P})$; let us write $S = A - p$ and let $k(p) = S^{-1}(A/p)$ be the field of fractions of $A/p$. Since $\mathfrak{P}$ contains $pB$, $\mathfrak{P}/pB$ is a prime ideal of $B/pB$. If $\rho'$ is the composite homomorphism $A \xrightarrow{\rho} B \to B/pB$, we know that $S^{-1}(B/pB)$ is identified with the ring $(\rho'(S))^{-1}(B/pB)$ and $\mathfrak{P}' = S^{-1}(\mathfrak{P}/pB)$ with an ideal of this ring (Chapter II, § 2, no. 2, Proposition 6); as $\mathfrak{P}/pB$ does not meet $\rho'(S)$, $\mathfrak{P}'$ is a prime ideal of $S^{-1}(B/pB)$ (Chapter 11, § 2, no. 5, Proposition 11); moreover there are canonical isomorphisms between $S^{-1}(B/pB)$, $S^{-1}((A/p) \otimes_A B)$ and $(S^{-1}(A/p)) \otimes_A B = k(p) \otimes_A B$; similarly $S^{-1}(F/pF)$ is canonically identified with $k(p) \otimes_A F$. This being so, under the hypotheses of Theorem 2, *in order that* $\mathfrak{P} \in \operatorname{Ass}_B(E \otimes_A F)$, *it is necessary and sufficient that* $p \in \operatorname{Ass}_A(E)$ and
$$
\mathfrak{P}' \in \operatorname{Ass}_{k(p) \otimes_A B}(k(p) \otimes_A F).
$$
For by Theorem 2 and its Corollary 1, it amounts to verifying that the conditions
$$
\text{``}\mathfrak{P} \in \operatorname{Ass}_B(F/pF)\text{''} \quad \text{and} \quad \text{``}\mathfrak{P}' \in \operatorname{Ass}_{k(p) \otimes_A B}(k(p) \otimes_A F)\text{''}
$$
are equivalent; but, as $B$ is Noetherian, this follows from § 1, no. 2, Corollary to Proposition 5 and the above identifications.

#### Proposition 11 {#ac-iv-s2-prop-11 .statement}

Suppose that $A$ and $B$ are Noetherian and that $B$ is a flat $A$-module. Let $E$ be an $A$-module and $E'$ a submodule of $E$ such that, for every ideal $p \in \operatorname{Ass}_A(E/E')$, $pB$ is a prime ideal of $B$ or equal to $B$. Let $E' = \bigcap_{p \in \operatorname{Ass}(E/E')} Q(p)$ be a reduced primary decomposition of $E'$ in $E$, $Q(p)$ being $p$-primary for all $p \in \operatorname{Ass}(E/E')$.
(i) *If* $p \in \operatorname{Ass}(E/E')$ *and* $pB = B$, *then* $Q(p) \otimes_A B = E \otimes_A B$.
(ii) *If* $p \in \operatorname{Ass}(E/E')$ *and* $pB$ *is prime*, $Q(p)$ *is* $pB$*-primary* *in* $E \otimes_A B$.
(iii) *If* $\Phi$ *is the set* $\mathfrak{p} \in \operatorname{Ass}(E/E')$ *such that* $pB$ *is prime*, *then*
$$
E' \otimes_A B = \bigcap_{p \in \Phi} (Q(p) \otimes_A B)
$$
*and this relation is a reduced primary decomposition of* $E' \otimes_A B$ *in* $E \otimes_A B$.

If $pB = B$, Theorem 2 applied to $E/\mathbf{Q}(p)$ and $B$ shows that
$$
\operatorname{Ass}_B((E/\mathbf{Q}(p)) \otimes_A B) = \varnothing
$$
and, as $B$ is Noetherian and is a flat $A$-module, we conclude (§ 1, no. 1, Corollary 1 to Proposition 2) that $\mathbf{Q}(p) \otimes_A B = E \otimes_A B$. Assertion (ii) follows from Corollary 2 to Theorem 2, taking $\mathfrak{P} = pB$. Finally the relation $E' \otimes_A B = \bigcap_{p \in \Phi} (\mathbf{Q}(p) \otimes_A B)$ follows from the fact that $B$ is a flat $A$-module (Chapter I, § 2, no. 6, Proposition 6); as $p = \overline{\rho}^{-1}(pB)$ for $p \in \Phi$ (Lemma 1), $pB \neq p'B$ for two distinct ideals $p, p'$ of the set $\Phi$; on the other hand,
$$
\operatorname{Ass}((E \otimes_A B)/(E' \otimes_A B)) = \Phi
$$
by Theorem 2; we conclude from no. 3, Proposition 4 that
$$
E' \otimes_A B = \bigcap_{p \in \Phi} (\mathbf{Q}(p) \otimes_A B)
$$
is a reduced primary decomposition.

#### Corollary {#ac-iv-s2-n6-cor-1 .statement}

*Suppose that* $pB$ *is prime for all* $p \in \operatorname{Ass}_A(E/E')$. *Then, if* $p_1, \ldots, p_n$ *are the minimal elements of* $\operatorname{Ass}_A(E/E')$, *the* $p_iB$ *are minimal elements of*
$$
\operatorname{Ass}_A((E \otimes_A B)/(E' \otimes_A B)).
$$
It follows from Proposition 11 that in this case $p_iB \neq p_jB$ for $i \# j$.

*Examples*
(1) Let us take $B = S^{-1}A$, where $S$ is a multiplicative subset of $A$; if $A$ is Noetherian, the hypotheses of Proposition 11 are satisfied and we recover a part of Proposition 6 of no. 4.
(2) Let $A$ be a Noetherian ring, $m$ an ideal of $A$ and $B$ the Hausdorff completion of $A$ with respect to the $m$-adic topology; then $B$ is a flat $A$-module and Theorem 2 may be applied with $F = B$; but in general the hypotheses of Proposition 11 are not satisfied for the prime ideals of $A$ (Chapter III, § 2, Exercise 15 (b)).
(3) Let $A$ be a Noetherian ring and $B$ the polynomial algebra $A[X_1, \ldots, X_n]$; $B$ is Noetherian and is a free $A$-module and therefore flat. Also, if $p$ is a prime ideal of $A$, $B/pB$ is isomorphic to $(A/p)[X_1, \ldots, X_n]$, which is an integral domain, and hence $pB$ is prime; the hypotheses of Proposition 11 are therefore satisfied for every $A$-module $E$ and every submodule $E'$ of $E$.
(4) Let $A$ be a finitely generated algebra over a field $k$, $K$ an extension of $k$ and $B = A \otimes_k K$ the algebra over $K$ obtained by extension of scalars; $A$ and $B$ are Noetherian and $B$ is a free $A$-module and hence Theorem 2 may be applied to $F = B$. In certain cases (for example if $k$ is algebraically closed) it can be shown that for every prime ideal $p$ of $A$, $pB$ is prime or equal to $B$; we shall return later to this example.

### Exercises {#ac-iv-s2-exercises}

See the [exercises for § 2](exercises/s2/).
