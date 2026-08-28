---
book: int
book_title: Integration
chapter: IX
chapter_title: MEASURES ON HAUSDORFF TOPOLOGICAL SPACES
section: 4
section_title: Inverse limits of measures
lang: en
source: int-vii-ix
book_pages: INT IX.49-INT IX.55, INT IX.112-INT IX.113
pdf_pages: 0231-0237, 0294-0295
extraction: ocr
subsections:
    - "no": 1
      title: Complements on compact spaces and inverse limits
      page: 50
      pdf_page: 232
    - "no": 2
      title: Inverse systems of measures
      page: 50
      pdf_page: 232
    - "no": 3
      title: The case of countable inverse systems
      page: 54
      pdf_page: 236
statements: 7
exercises: 2
content_sha256: b4e7cd1d1788dbad199a14046cb0e8a2678d3219bed052cfd2b9150b2bbab48e
---

## § 4. INVERSE LIMITS OF MEASURES

*Throughout this section, I denotes a nonempty set, equipped with a preorder relation, denoted $i \leq j$, and directed for this relation. Recall (GT, I, §4, No. 4) that an inverse system of topological spaces indexed by I is a family $(T_i, p_{ij})$ where $T_i$ is a topological space and $p_{ij}$ is a continuous mapping of $T_j$ into $T_i$ for $i \leq j$, where $p_{ii}$ is the identity mapping of $T_i$, and where $p_{ik} = p_{ij} \circ p_{jk}$ for $i \leq j \leq k$. Let T be a topological space and $(p_i)_{i \in I}$ a family of continuous mappings $p_i : T \to T_i$. The family $(p_i)_{i \in I}$ is said to be coherent if $p_i = p_{ij} \circ p_j$ for $i \leq j$, and it is said to be separating if for distinct $x, y$ in T there exists an $i \in I$ such that $p_i(x) \neq p_i(y)$. When $T = \varprojlim T_i$ and $p_i$ is the canonical mapping of T into $T_i$, the family $(p_i)_{i \in I}$ is coherent and separating.*

(3) In a Souslin space, every Borel set is a Souslin set (GT, IX, §6, No. 3, Prop. 11).
(4) More generally, if $f : X \to Y$ is a continuous bijection between Souslin spaces, then $\mu \mapsto f(\mu)$ is a bijective mapping of the set of bounded measures on X onto the set of bounded measures on Y (§ 2, No. 4, Prop. 9).

### 1. Complements on compact spaces and inverse limits

#### Proposition 1 {#int-ix-s4-prop-1 .statement}

— Let X and Y be two topological spaces and f a continuous mapping of X into Y. Let $(K_\alpha)_{\alpha \in A}$ be a decreasing directed family of compact subsets of X, with intersection K. Then $f(K) = \bigcap_{\alpha \in A} f(K_\alpha)$.

For, let y be a point of $\bigcap_{\alpha \in A} f(K_\alpha)$; for every $\alpha \in A$, the set $L_\alpha = K_\alpha \cap f^{-1}(y)$ is compact and nonempty. The family $(L_\alpha)_{\alpha \in A}$ is directed downward, therefore its intersection L is nonempty. Now, $L = K \cap f^{-1}(y)$, whence $y \in f(K)$. We have thus proved the inclusion $f(K) \supset \bigcap_{\alpha \in A} f(K_\alpha)$, and the reverse inclusion is obvious.

#### Proposition 2 {#int-ix-s4-prop-2 .statement}

— Let there be given an inverse system $(T_i, p_{ij})$ of topological spaces indexed by I, a topological space T, and a coherent and separating family of continuous mappings $p_i : T \to T_i$. Then:

a) For every compact subset K of T, one has $K = \bigcap_{i \in I} p_i^{-1}(p_i(K))$.

b) Let K and L be two disjoint compact subsets of T. There exists an $i \in I$ such that $p_j(K)$ and $p_j(L)$ are disjoint for $j \geq i$.

a) Let x be a point of $\bigcap_{i \in I} p_i^{-1}(p_i(K))$; for every $i \in I$, the set $K_i$ of points y in K such that $p_i(y) = p_i(x)$ is a nonempty closed subset of K. For $i \leq j$ we have $K_i \supset K_j$, and, since K is compact, the set $\bigcap_{i \in I} K_i$ is therefore nonempty. Let y be a point of $\bigcap_{i \in I} K_i$; we have $y \in K$ and $p_i(y) = p_i(x)$ for all $i \in I$, whence $y = x$; finally, $x \in K$, which proves the inclusion $K \supset \bigcap_{i \in I} p_i^{-1}(p_i(K))$; the reverse inclusion is obvious.

b) For every $i \in I$, set $M_i = p_i^{-1}(p_i(K)) \cap L$; this is a closed subset of the compact space L, we have $M_i \supset M_j$ for $i \leq j$, and, by a),

$$
\bigcap_{i \in I} M_i = K \cap L = \varnothing.
$$

Consequently, there exists an index i such that $M_i = \varnothing$. For $j \geq i$, we have $p_j^{-1}(p_j(K)) \cap L = M_j \subset M_i = \varnothing$, whence $p_j(K) \cap p_j(L) = \varnothing$.

### 2. Inverse systems of measures

#### Definition 1 {#int-ix-s4-def-1 .statement}

— Let $\mathcal{T} = (T_i, p_{ij})$ be an inverse system of topological spaces indexed by I. One calls inverse system (resp. sub-inverse system) of measures on $\mathcal{T}$ a family $(\mu_i)_{i \in I}$, where $\mu_i$ is a bounded measure on $T_i$ for all $i \in I$, and where $\mu_i = p_{ij}(\mu_j)$ (resp. $\mu_i \geq p_{ij}(\mu_j)$) for $i \leq j$.

#### Proposition 3 {#int-ix-s4-prop-3 .statement}

*Let there be given an inverse system of topological spaces $\mathcal{T} = (T_i, p_{ij})$ indexed by $I$, a topological space $T$, a coherent and separating family of continuous mappings $p_i : T \to T_i$ (for $i \in I$) and a sub-inverse system $(\mu_i)_{i \in I}$ of measures on $\mathcal{T}$. For every compact subset K of $T$, set*

$$
J(K) = \inf_{i \in I} \mu_i^\bullet(p_i(K)).
$$

*Then there exists a bounded measure $\pi$ on $T$, and only one, such that $\pi^\bullet(K) = J(K)$ for every compact subset $K$ of $T$. One has $\mu_i \geq p_i(\pi)$ for all $i \in I$, and $\pi$ is the largest measure on $T$ satisfying this condition.*

Let us first prove that $J(K)$ is the limit of $\mu_i^\bullet((p_i(K)))$ with respect to the section filter $\mathfrak{F}$ of the directed preordered set $I$: for this, it suffices (GT, IV, §5, No. 2, Th. 2) to show that $\mu_i^\bullet(p_i(K)) \geq \mu_j^\bullet(p_j(K))$ for $i \leq j$; now, setting $\mu_{ij}' = p_{ij}(\mu_j)$, we have $\mu_{ij}' \leq \mu_i$ and $p_j(K) \subset \overline{p_{ij}}^{-1}(p_i(K))$, whence

$$
\mu_j^\bullet(p_j(K)) \leq \mu_j^\bullet(\overline{p_{ij}}^{-1}(p_i(K))) = (\mu_{ij}')^\bullet(p_i(K)) \leq \mu_i^\bullet(p_i(K)).
$$

Let us now pass to the study of the properties of the function $J$:
1) It is clear that $J(K) \leq J(L)$ when $K \subset L$.
2) Let $K$ and $L$ be two compact subsets of $T$. For every $i \in I$, we have $p_i(K \cup L) = p_i(K) \cup p_i(L)$, whence

$$
\mu_i^\bullet(p_i(K \cup L)) \leq \mu_i^\bullet(p_i(K)) + \mu_i^\bullet(p_i(L));
$$

passing to the limit with respect to the filter $\mathfrak{F}$, we obtain $J(K \cup L) \leq J(K) + J(L)$.
3) Suppose that the compact sets $K$ and $L$ are disjoint. By Prop. 2 of No. 1, there exists an $i \in I$ such that $p_j(K) \cap p_j(L) = \varnothing$ for $j \geq i$. For $j \geq i$ we therefore have

$$
\mu_j^\bullet(p_j(K \cup L)) = \mu_j^\bullet(p_j(K)) + \mu_j^\bullet(p_j(L)),
$$

whence $J(K \cup L) = J(K) + J(L)$ on passing to the limit with respect to the filter $\mathfrak{F}$.
4) Let $(K_\alpha)_{\alpha \in A}$ be a decreasing directed family of compact subsets of $T$, with intersection $K$. By Prop. 1 of No. 1, $p_i(K) = \bigcap_{\alpha \in A} p_i(K_\alpha)$ and therefore $\mu_i^\bullet(p_i(K)) = \inf_{\alpha \in A} \mu_i^\bullet(p_i(K_\alpha))$ for all $i \in I$ (§ 1, No. 6, Cor. of Prop. 5). From this, one deduces
$$
J(K) = \inf_{i \in I} \mu_i^\bullet(p_i(K)) = \inf_{i \in I} \inf_{\alpha \in A} \mu_i^\bullet(p_i(K_\alpha))
= \inf_{\alpha \in A} \inf_{i \in I} \mu_i^\bullet(p_i(K_\alpha)) = \inf_{\alpha \in A} J(K_\alpha).
$$
5) Let us choose an $i \in I$ and set $c = \mu_i^\bullet(T_i)$. Then $c$ is finite and $J(K) \leq \mu_i^\bullet(p_i(K)) \leq \mu_i^\bullet(T_i)$, thus $J(K) \leq c$ for every compact set $K$ in $T$.

The preceding properties permit applying Th. 1 of § 3, No. 1; we conclude that there exists one and only one bounded measure $\pi$ on $T$ such that $\pi^\bullet(K) = J(K)$ for every compact subset $K$ of $T$. For every $i \in I$, let us denote by $\nu_i$ the measure on $T_i$ that is the image of $\pi$ under $p_i$. Let $i \in I$, $A$ a compact subset of $T_i$, and $\mathcal{L}$ the set of compact subsets of $\overline{p_i^{-1}(A)}$. By Remark 3 of § 1, No. 2, we have $\pi^\bullet(\overline{p_i^{-1}(A)}) = \sup_{K \in \mathcal{L}} \pi^\bullet(K)$; moreover, $\nu_i^\bullet(A) = \pi^\bullet(\overline{p_i^{-1}(A)})$ and $J(K) = \pi^\bullet(K)$ for $K \in \mathcal{L}$, whence $\nu_i^\bullet(A) = \sup_{K \in \mathcal{L}} J(K)$.

For $K \in \mathcal{L}$, we have $p_i(K) \subset A$, whence $J(K) \leq \mu_i^\bullet(p_i(K)) \leq \mu_i^\bullet(A)$ and finally $\nu_i^\bullet(A) \leq \mu_i^\bullet(A)$. Since $A$ is an arbitrary compact set in $T_i$, we conclude that $\nu_i \leq \mu_i$. The last assertion of the proposition is obvious.

Q.E.D.

#### Theorem 1 (Prokhorov) {#int-ix-s4-thm-1 .statement}

— *Let $\mathcal{T} = (T_i, p_{ij})$ be an inverse system of topological spaces indexed by $I$, $T$ a topological space and $(p_i)_{i \in I}$ a coherent and separating family of continuous mappings $p_i : T \to T_i$. Finally, let $(\mu_i)_{i \in I}$ be an inverse system of measures on $\mathcal{T}$.

For there to exist a bounded measure $\mu$ on $T$ such that $p_i(\mu) = \mu_i$ for all $i \in I$, it is necessary and sufficient that the following condition be satisfied:

(P) *for every $\varepsilon > 0$, there exists a compact subset $K$ of $T$ such that $\mu_i^\bullet(T_i - p_i(K)) \leq \varepsilon$ for all $i \in I$.

When this is so, the measure $\mu$ is uniquely determined and*
$$
\mu^\bullet(K) = \inf_i \mu_i^\bullet(p_i(K))
$$
*for every compact set $K$ in $T$*.

Let us first prove the uniqueness of $\mu$. Let $\mu$ be a bounded measure on $T$ such that $p_i(\mu) = \mu_i$ for all $i \in I$. Let $K$ be a compact subset of $T$; by Prop. 2 of No. 1, the set $K$ is the intersection of the decreasing directed family $(\overline{p_i^{-1}(p_i(K))})_{i \in I}$ of *closed* subsets of $T$. By the Cor. of Prop. 5 of § 1, No. 6, we therefore have
$$
\mu^\bullet(K) = \inf_{i \in I} \mu^\bullet(\overline{p_i^{-1}(p_i(K))}) = \inf_{i \in I} \mu_i^\bullet(p_i(K)),
$$

which establishes the formula (2). Since two measures that coincide on the set of compact sets are equal (§ 1, No. 2, Cor. of Prop. 2), it follows that $\mu$ is unique.

By Prop. 3, there exists a bounded measure $\pi$ on $T$ such that $\pi^\bullet(K) = \inf_{i \in I} \mu_i^\bullet(p_i(K))$ for every compact subset $K$ of $T$. By formula (2), the existence of a bounded measure $\mu$ on $T$ such that $p_i(\mu) = \mu_i$ for all $i \in I$ is therefore equivalent to the relation:

(P') $p_i(\pi) = \mu_i$ for all $i \in I$.

For $i \leq j$, we have $\mu_i = p_{ij}(\mu_j)$, whence $\mu_i^\bullet(T_i) = \mu_j^\bullet(T_j)$; since $I$ is directed, there exists a finite number $c \geq 0$ such that $\mu_i^\bullet(T_i) = c$ for all $i \in I$. By Prop. 3, the measure $\mu_i - p_i(\pi)$ is positive, hence is zero if and only if its total mass is zero, that is, if $\mu_i(T_i) = p_i(\pi)^\bullet(T_i)$. Since $p_i(\pi)^\bullet(T_i) = \pi^\bullet(T)$, the condition (P') is thus equivalent to $\pi^\bullet(T) = c$, that is (§ 1, No. 2, Remark 3) to the property:

(P'') $\sup_{K \in \mathcal{K}} \pi^\bullet(K) = c$, where $\mathcal{K}$ is the set of compact subsets of $T$.

Now, for $K \in \mathcal{K}$, we have

$$
\pi^\bullet(K) = \inf_{i \in I} \mu_i^\bullet(p_i(K)) = c - \sup_{i \in I} \mu_i^\bullet(T_i - p_i(K))
$$

and this formula immediately implies the equivalence of (P) and (P'').

Q.E.D.

Let $(T_i, p_{ij})$ be an inverse system of topological spaces. Set $T = \lim_{\leftarrow} T_i$ and denote by $p_i$ the canonical mapping of $T$ into $T_i$. Generalizing Def. 2 of Ch. III, § 4, No. 5, we shall say that a bounded measure $\mu$ on $T$ is the *inverse limit of an inverse system* $(\mu_i)_{i \in I}$ *of measures* if $\mu_i = p_i(\mu)$ for all $i \in I$. Th. 1 provides a criterion for the existence of inverse limits of measures. When the spaces $T_i$ are *compact*, and the mappings $p_{ij}$ surjective, $T$ is compact and $p_i(T) = T_i$ for every $i \in I$; the condition (P) is therefore fulfilled, and in this case we recover Prop. 8, (iv) of Ch. III, § 4, No. 5.

#### Remark {#int-ix-s4-n2-rem-1 .statement}

— Let $(\mu_i)_{i \in I}$ be an inverse system of measures on the inverse system of spaces $\mathcal{T} = (T_i, p_{ij})$. Assume given a topological space $T'$ and continuous mappings $p'_i : T' \to T_i$; assume that the family $(p'_i)_{i \in I}$ is coherent, but not necessarily separating. *If Prokhorov's condition (P) is satisfied by the family* $(p'_i)_{i \in I}$, *there exists a measure* $\mu'$ (*not necessarily unique*) *on* $T'$ *such that* $p'_i(\mu') = \mu_i$ *for all* $i \in I$.

For, set $T = \lim_{\leftarrow} T_i$ and $p' = (p'_i)_{i \in I}$, and denote by $p_i$ the canonical mapping of $T$ into $T_i$; Prokhorov's condition is satisfied by $T$ and the $p_i$, because $p_i(p'(K')) = p'_i(K')$ and $p'(K')$ is compact in $T$ for every compact subset $K'$ of $T'$. By Th. 1, there exists a bounded measure $\mu$ on $T$ such that $p_i(\mu) = \mu_i$ for all $i \in I$. Let $K'$ be a compact set in $T'$; then $\mu^\bullet(p'(K')) = \inf_{i \in I} \mu_i^\bullet(p'_i(K'))$, whence
$$
\mu^\bullet(T - p'(K')) = \sup_{i \in I} \mu_i^\bullet(T_i - p_i'(K')).
$$
Let $\varepsilon > 0$; since Prokhorov’s condition (P) is satisfied by the $p_i'$, one can therefore find a compact subset $K'$ of $T'$ such that $\mu^\bullet(T - p'(K')) \leq \varepsilon$. Prop. 8 of §2, No. 4 then establishes the existence of a bounded measure $\mu'$ on $T'$ with $\mu = p'(\mu')$, whence $\mu_i = p_i(\mu) = p_i(p'(\mu')) = p_i'(\mu')$ for all $i \in I$.

### 3. The case of countable inverse systems

#### Theorem 2 {#int-ix-s4-thm-2 .statement}

— *Assume that the directed preordered set I has a countable cofinal subset. Let $\mathcal{T} = (T_i, p_{ij})$ be an inverse system of topological spaces, $T = \lim_{\leftarrow} T_i$ and $p_i$ the canonical mapping of $T$ into $T_i$. Then every inverse system $(\mu_i)_{i \in I}$ of measures on $\mathcal{T}$ admits an inverse limit.*

We shall first treat the case that $I = \mathbf{N}$ and set $q_n = p_{n,n+1}$. Let $\varepsilon > 0$. Define recursively a sequence of compact sets $L_n \subset T_n$ as follows: $L_0$ is a compact subset of $T_0$ such that $\mu_0^\bullet(T_0 - L_0) \leq \varepsilon/2$, and for $n \geq 0$ the compact set $L_{n+1}$ is contained in $\overline{q_n^{-1}(L_n)}$ and satisfies
$$
\mu_{n+1}^\bullet(\overline{q_n^{-1}(L_n)} - L_{n+1}) \leq \varepsilon/2^{n+2}.
$$
This construction is possible by virtue of *Remark 3* of §1, No. 2. We have
$$
\begin{align*}
\mu_{n+1}^\bullet(T_{n+1} - L_{n+1}) &= \mu_{n+1}^\bullet(T_{n+1} - \overline{q_n^{-1}(L_n)}) + \mu_{n+1}^\bullet(\overline{q_n^{-1}(L_n)} - L_{n+1}) \\
&\leq \mu_{n+1}^\bullet(T_{n+1} - \overline{q_n^{-1}(L_n)}) + \varepsilon/2^{n+2} \\
&= \mu_n^\bullet(T_n - L_n) + \varepsilon/2^{n+2}
\end{align*}
$$
because $\mu_n = q_n(\mu_{n+1})$; by induction on $p$, one deduces that
$$
\mu_p^\bullet(T_p - L_p) \leq \varepsilon(1 - 1/2^{p+1}) \leq \varepsilon.
$$
Since $T$ is a closed subspace of $\prod_{n \in \mathbf{N}} T_n$ and the product space $\prod_{n \in \mathbf{N}} L_n$ is compact, the subset $L = T \cap \prod_{n \in \mathbf{N}} L_n = \bigcap_{n \in \mathbf{N}} \overline{p_n^{-1}(L_n)}$ of $T$ is compact. Let $n \in \mathbf{N}$; we have $p_n(L) = \bigcap_{m \geq n} p_{nm}(L_m)$ (GT, I, §9, No. 6, Prop. 8) and $p_{nm}(L_m) \supset p_{nm'}(L_{m'})$ for $m' \geq m \geq n$, whence
$$
\mu_n^\bullet(T_n - p_n(L)) = \lim_{m \to \infty} \mu_n^\bullet(T_n - p_{nm}(L_m)).
$$

But, for $m \geq n$, the measure $\mu_n$ is the image of $\mu_m$ under $p_{nm}$, whence

$$
\mu_n^\bullet(T_n - p_{nm}(L_m)) = \mu_m^\bullet(T_m - \overline{p}_{nm}(p_{nm}(L_m))) \leq \mu_m^\bullet(T_m - L_m) \leq \varepsilon;
$$

passing to the limit with respect to $m$, we obtain $\mu_n^\bullet(T_n - p_n(L)) \leq \varepsilon$. In other words, Prokhorov’s condition (P) is satisfied, and there exists a bounded measure $\mu$ on $T$ such that $\mu_n = p_n(\mu)$ for all $n \in \mathbf{N}$ (No. 2, Th. 1).

Let us pass to the general case: there exists in $I$ an increasing cofinal sequence $(i_n)_{n \in \mathbf{N}}$. The mapping $t \mapsto (p_{i_n}(t))_{n \in \mathbf{N}}$ is a homeomorphism of $T$ onto the inverse limit of the inverse system $(T_{i_n}, p_{i_n i_m})$ (GT, I, §4, No. 4). By the first part of the proof, there exists therefore a bounded measure $\mu$ on $T$ such that $\mu_{i_n} = p_{i_n}(\mu)$ for all $n \in \mathbf{N}$. Let $i \in I$; there exists an $n \in \mathbf{N}$ with $i \leq i_n$, whence

$$
p_i(\mu) = p_{i i_n}(p_{i_n}(\mu)) = p_{i i_n}(\mu_{i_n}) = \mu_i.
$$

Q.E.D.

Theorem 2 is often used in the following situation: let $D$ be a countable set and $(X_t)_{t \in D}$ a family of topological spaces. Let $\mathfrak{F}$ be the set of finite subsets of $D$, ordered by inclusion. For $J$ in $\mathfrak{F}$, set $X_J = \prod_{t \in J} X_t$, and for $J \subset J'$ let $p_{JJ'}$ be the canonical projection of $X_{J'}$ onto the partial product $X_J$. Also set $X = \prod_{t \in D} X_t$ and denote by $p_J$ the canonical projection of $X$ onto the partial product $X_J$. One shows easily (cf. S, III, §7, No. 2, Remark 3) that the family $(p_J)_{J \in \mathfrak{F}}$ defines a homeomorphism of $X$ onto $\lim_{\leftarrow} X_J$. An inverse system of measures is then a family of bounded measures $\mu_J$ on $X_J$ such that $\mu_J = p_{JJ'}(\mu_{J'})$ for $J \subset J'$. There exists one and only one bounded measure $\mu$ on $X$ such that $\mu_J = p_J(\mu)$ for every finite subset $J$ of $D$ (*Kolmogoroff’s theorem*). One sometimes says that $\mu$ is the measure on $\prod_{t \in D} X_t$ having *margins* $\mu_J$.

In particular, suppose given, for every $t \in D$, a measure $\nu_t$ on $X_t$ of total mass 1. Set $\mu_J = \bigotimes_{t \in J} \nu_t$ for every finite subset $J$ of $D$. Let $J \subset J'$ be two finite subsets of $D$ and let $K = J' - J$; identifying $X_{J'}$ with $X_J \times X_K$, one has $\mu_{J'} = \mu_J \otimes \mu_K$, and since the measure $\mu_K$ has total mass 1, the projection of $\mu_J \otimes \mu_K$ on $X_J$ is equal to $\mu_J$. The measure on $X$ admitting the margins $\mu_J$ is denoted $\bigotimes_{t \in D} \nu_t$ and is called the *product of the family* $(\nu_t)_{t \in D}$. When the spaces $X_t$ are compact, we recover the construction of Ch. III, §4, No. 6.

### Exercises {#int-ix-s4-exercises}

See the [exercises for § 4](exercises/s4/).
