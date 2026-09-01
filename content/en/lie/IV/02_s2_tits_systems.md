---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IV
chapter_title: COXETER GROUPS AND TITS SYSTEMS
section: 2
section_title: Tits Systems
lang: en
source: lie-iv-vi
pdf_pages: 0028-0039, 0057-0072
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITIONS AND FIRST PROPERTIES
      page: 0
      pdf_page: 28
    - "no": 2
      title: AN EXAMPLE
      page: 0
      pdf_page: 30
    - "no": 3
      title: DECOMPOSITION OF G INTO DOUBLE COSETS
      page: 0
      pdf_page: 31
    - "no": 4
      title: RELATIONS WITH COXETER SYSTEMS
      page: 0
      pdf_page: 32
    - "no": 5
      title: SUBGROUPS OF G CONTAINING B
      page: 0
      pdf_page: 34
    - "no": 6
      title: PARABOLIC SUBGROUPS
      page: 0
      pdf_page: 35
    - "no": 7
      title: SIMPLICITY THEOREMS
      page: 0
      pdf_page: 36
statements: 30
exercises: 29
content_sha256: ccce30facb7daeeb1f882ab3b15679e0177fc6be4aed4b3638cf63dca4b4ec2f
---

## § 2. TITS SYSTEMS

In this paragraph, the letters G, B, N, S, T, W have the meaning indicated in no. 1 below.

### 1. DEFINITIONS AND FIRST PROPERTIES

Let G be a group and B a subgroup of G. The group $B \times B$ acts on G by $(b, b').g = bg{b'}^{-1}$ for $b, b' \in B$ and $g \in G$. The orbits of $B \times B$ on G are the sets $BgB$ for $g \in G$, and are called the double cosets of G with respect to B. They form a partition of G; the corresponding quotient is denoted by $B \backslash G / B$. If C and $C'$ are double cosets, $CC'$ is a union of double cosets.

#### Definition 1 {#lie-iv-s2-def-1 .statement}

A Tits system is a quadruple $(G, B, N, S)$, where G is a group, B and N are two subgroups of G and S is a subset of $N/(B \cap N)$, satisfying the following axioms:

(T1) The set $B \cup N$ generates G and $B \cap N$ is a normal subgroup of N.
(T2) The set S generates the group $W = N/(B \cap N)$ and consists of elements of order 2.
(T3) $sBw \subset BwB \cup BswB$ for $s \in S$ and $w \in W$.
(T4) For all $s \in S$, $sBs \notin B$.

The group $W = N/(B \cap N)$ is sometimes called the Weyl group of the Tits system $(G, B, N, S)$.

5 Every element of W is a coset modulo $B \cap N$, and is thus a subset of G; hence products such as $BwB$ make sense. More generally, for any subset A of W, we denote by BAB the subset $\bigcup_{w \in A} BwB$.

#### Remark 1 {#lie-iv-s2-n1-rem-1 .statement}

We shall see in no. 5 (Cor. of Th. 3) that, if $(G, B, N)$ is given, there exists at most one subset $S$ of $N/(B \cap N)$ such that $(G, B, N, S)$ is a Tits system.

#### Remark 2 {#lie-iv-s2-n1-rem-2 .statement}

Let $(G, B, N, S)$ be a Tits system, and let $Z$ be a normal subgroup of $G$ contained in $B$. Let $G' = G/Z, B' = B/Z, N' = N/(Z \cap N)$, and let $S'$ be the image of $S$ in $N'/(B' \cap N')$. Then one sees immediately that $(G', B', N', S')$ is a Tits system.

Throughout this paragraph, with $(G, B, N, S)$ denoting a Tits system, we set $T = B \cap N$ and $W = N/T$. A double coset means a double coset of $G$ with respect to $B$. For any $w \in W$, we set $C(w) = BwB$; this is a double coset.

We are going to deduce several elementary consequences of the axioms (T1) to (T4). We denote by $w, w', \ldots$ elements of $W$ and by $s, s', \ldots$ elements of $S$. The following relations are clear:

$$
C(1) = B, \quad C(ww') \subset C(w).C(w'), \quad C(w^{-1}) = C(w)^{-1}.
$$

Axiom (T3) can also be written in the form

$$
C(s).C(w) \subset C(w) \cup C(sw).
$$

Moreover, since $C(sw) \subset C(s).C(w)$ by (1) and since $C(s).C(w)$ is a union of double cosets, there are only two possibilities:

$$
C(s).C(w) = \begin{cases}
C(sw) & \text{if } C(w) \not\subset C(s).C(w) \\
C(w) \cup C(sw) & \text{if } C(w) \subset C(s).C(w).
\end{cases}
$$

By (T4), $B \neq C(s).C(s)$; putting $w = s$ in (3) and using the relation $s^2 = 1$, we obtain

$$
C(s).C(s) = B \cup C(s).
$$

This formula shows that $B \cup C(s)$ is a subgroup of $G$. Multiplying both sides of (4) on the right by $C(w)$, and using formula (3) and the relation

$$
B.C(w) = C(w),
$$

we obtain

$$
C(s).C(s).C(w) = C(w) \cup C(sw).
$$

Taking the inverses of the sets entering into formulas (2), (3) and (5) and then replacing $w$ by $w^{-1}$, we obtain the formulas

$$
C(w).C(s) \subset C(w) \cup C(ws)
$$
$$
C(w).C(s) = \begin{cases}
C(ws) & \text{if } C(w) \not\subset C(w).C(s) \\
C(w) \cup C(ws) & \text{if } C(w) \subset C(w).C(s)
\end{cases}
$$
$$
C(w).C(s).C(s) = C(w) \cup C(ws).
$$

#### Lemma 1 {#lie-iv-s2-lem-1 .statement}

Let $s_1, \ldots, s_q \in S$ and let $w \in W$. We have
$$
C(s_1 \ldots s_q).C(w) \subset \bigcup_{(i_1, \ldots, i_p)} C(s_{i_1} \ldots s_{i_p} w),
$$
where $(i_1, \ldots, i_p)$ denotes the set of strictly increasing sequences of integers in the interval $[1, q]$.

We argue by induction on $q$, the case $q = 0$ being trivial. If $q \geqslant 1$, we have $C(s_1 \ldots s_q).C(w) \subset C(s_1).C(s_2 \ldots s_q).C(w)$. By the induction hypothesis, $C(s_2 \ldots s_q).C(w)$ is contained in the union of the $C(s_{j_1} \ldots s_{j_p} w)$, where
$$
2 \leq j_1 < \cdots < j_p \leq q.
$$
By (T3), the set $C(s_1).C(s_{j_1} \ldots s_{j_p} w)$ is contained in the union of the sets $C(s_1 s_{j_1} \ldots s_{j_p} w)$ and $C(s_{j_1} \ldots s_{j_p} w)$. This proves the lemma.

### 2. AN EXAMPLE

Let $k$ be a field, $n$ an integer $\geq 0$, and $(e_i)$ the canonical basis of $k^n$. Let $G = \mathbf{GL}(n, k)$, let $B$ be the upper triangular subgroup of $G$, and let $N$ be the subgroup of $G$ consisting of the matrices having exactly one non-zero element in each row and column. An element of $N$ permutes the lines $ke_i$; this gives rise to a surjective homomorphism $N \to \mathcal{S}_n$ whose kernel is the subgroup $T = B \cap N$ of diagonal matrices, and allows us to identify $W = N/T$ with $\mathcal{S}_n$. We denote by $s_j$ ($1 \leq j \leq n-1$) the element of $W$ corresponding to the transposition of $j$ and $j+1$; let $S$ be the set of $s_j$. *The quadruple* $(G, B, N, S)$ *is a Tits system*. Indeed:

Axiom (T1) follows from Cor. 2 of Prop. 14 of *Algebra*, Chap. II, § 10, no. 13.

Axiom (T2) is proved in *Algebra*, Chap. I, Correction to p. 97.
Axiom (T4) is immediate.
It remains to verify axiom (T3), i.e.
$$
s_j B w \subset B w B \cup B s_j w B \quad \text{for } 1 \leq j \leq n-1, w \in W,
$$
or equivalently,
$$
s_j B \subset B B' \cup B s_j B', \quad \text{with } B' = w B w^{-1}.
$$
Let $G_j$ be the subgroup of $G$ consisting of the elements that fix the $e_i$ for $i \neq j, j+1$ and stabilize the plane spanned by $e_j$ and $e_{j+1}$; this group is isomorphic to $\mathbf{GL}(2, k)$. One checks that $G_j B = B G_j$. Since $s_j \in G_j$, we have $s_j B \subset B G_j$, and it suffices to prove that
$$
G_j \subset (B \cap G_j)(B' \cap G_j) \cup (\cap G_j) s_j (B' \cap G_j).
$$
Identify $G_j$ with $\mathbf{GL}(2, k)$; the group $B \cap G_j$ is then identified with the upper triangular subgroup $B_2$ of $\mathbf{GL}(2, k)$, while the group $B' \cap G_j$ is identified with $B_2$ when $w(j) < w(j+1)$ and with the lower triangular subgroup $B_2^-$ otherwise. In the first case, the formula to be proved can be written

$$
\mathbf{GL}(2, k) = B_2 \cup B_2 s B_2 \quad \text{where } s = \begin{pmatrix} 0 & 1 \\ 1 & 0 \end{pmatrix};
$$

this follows for example from the fact that $B_2$ is the stabilizer of a point for the action of $\mathbf{GL}(2, k)$ on the projective line $\mathbf{P}_1(k)$, and acts transitively on the complement of this point. In the second case, the formula to be proved can be written

$$
\mathbf{GL}(2, k) = B_2 B_2^- \cup B_2 s B_2^-;
$$

since $B_2^- = s B_2 s$, this follows from the preceding formula by multiplying on the right by $s$.

### 3. DECOMPOSITION OF G INTO DOUBLE COSETS

#### Theorem 1 {#lie-iv-s2-thm-1 .statement}

*We have $G = \mathrm{BWB}$. The map $w \mapsto C(w)$ is a bijection from $W$ to the set $B \backslash G / B$ of double cosets of $G$ with respect to $B$.*

It is clear that $\mathrm{BWB}$ is stable under $x \mapsto x^{-1}$, and Lemma 1 shows that it is stable under the product. Since it contains $B$ and $N$, it is equal to $G$.

It remains to prove that $C(w) \neq C(w')$ if $w \neq w'$. For this, we shall prove by induction on the integer $q$ the following assertion:

(A_q) If $w$ and $w'$ are distinct elements of $W$ such that $l_S(w) \geq l_S(w') = q$, then $C(w) \neq C(w')$.

(For the definition of $l_S(w)$, see § 1, no. 1.)

This assertion is clear for $q = 0$, since then $w' = 1$ and $w \neq 1$, hence $C(w') = B$ and $C(w) \neq B$.

Assume that $q \geq 1$ and that $w, w'$ satisfy the hypotheses of (A_q). There exists $s \in S$ such that $sw'$ is of length $q - 1$. We have

$$
l_S(w) > l_S(sw')
$$

hence $w \neq sw'$. Moreover, $sw \neq sw'$; by formula (3) of § 1, no. 1, we have

$$
l_S(sw) \geq l_S(w) - 1 \geq l_S(sw') = q - 1.
$$

By the induction hypothesis, $C(sw')$ is distinct from $C(w)$ and from $C(sw)$; from formula (2) it follows that

$$
C(sw') \cap C(s).C(w) = \varnothing.
$$

Since $C(sw') \subset C(s).C(w')$, we have finally that $C(w) \neq C(w')$.

#### Remark {#lie-iv-s2-n3-rem-1 .statement}

Axiom (T4) was not used in the preceding proof.

### 4. RELATIONS WITH COXETER SYSTEMS

#### Theorem 2 {#lie-iv-s2-thm-2 .statement}

The pair $(W, S)$ is a Coxeter system. Moreover, for $s \in S$ and $w \in W$, the relations $C(sw) = C(s).C(w)$ and $l_S(sw) > l_S(w)$ are equivalent.

For any $s \in S$, let $P_s$ be the set of elements $w \in W$ such that
$$
C(s).C(w) = C(sw).
$$
We are going to verify that the $P_s$ satisfy conditions (A'), (B') and (C) of § 1, no. 7; the two assertions of the theorem will then follow from Prop. 6 of § 1, no. 7.

Condition (A') is clear.

We verify (B'). If $P_s$ and $sP_s$ had an element $w$ in common, we would have $w \in P_s$ and $sw \in P_s$, and hence
$$
C(s).C(w) = C(sw), \qquad C(s).C(sw) = C(w).
$$
It would follow that $C(s).C(s).C(w) = C(w)$ and, by formula (5), this would imply that $C(w) = C(sw)$, which would contradict Th. 1.

We verify (C). Let $s, s' \in S$ and $w, w' \in W$ with $w' = ws'$. The assumption that $w \in P_s$ and $w' \notin P_s$ implies that
$$
C(sw) = C(s).C(w) \tag{9}
$$
$$
C(w') \subset C(s).C(w') \tag{10}
$$
by (3).

From (9) and the relation $w = w's'$, it follows that
$$
C(s)w's'B = C(sw). \tag{11}
$$
By formula (2'), $C(w').C(s') \subset C(w') \cup C(w's')$, which immediately implies that
$$
C(w')s'B \subset C(ws') \cup C(w). \tag{12}
$$
Since $C(w')$ is a union of left cosets $gB$ and since
$$
C(s).C(w') = C(s)w'B,
$$
formula (10) shows that $C(s)w'$ meets $C(w')$ and *a fortiori* that $C(s)w's'B$ meets $C(w')s'B$. It follows from formulas (11) and (12) that the double coset $C(sw)$ is equal to one of the double cosets $C(ws')$ and $C(w)$; since $sw \neq w$, Th. 1 allows us to conclude that $sw = ws'$.

#### Corollary 1 {#lie-iv-s2-thm-2-cor-1 .statement}

*Let* $w_1, \ldots, w_q \in W$ *and let* $w = w_1 \ldots w_q$. *If*
$$
l_S(w) = l_S(w_1) + \cdots + l_S(w_q),
$$
*then*
$$
C(w) = C(w_1) \ldots C(w_q).
$$

On taking reduced decompositions of the $w_i$, one is reduced to the case of a reduced decomposition

$$
w = s_1 \ldots s_q, \quad \text{with } s_i \in S.
$$

If $u = s_2 \ldots s_q$, then $w = s_1 u$ and $l_S(s_1 u) > l_S(u)$, so $C(w) = C(s_1).C(u)$ by the theorem. The required formula follows from this by induction on $q$.

#### Corollary 2 {#lie-iv-s2-thm-2-cor-2 .statement}

*Let $w \in W$ and let $T_w$ be the subset of $W$ associated to $w$ by the procedure of Lemma 2 of § 1, no. 4. If $t \in T_w$, then*

$$
C(t) \subset C(w).C(w^{-1}).
$$

If $t \in T_w$, there exist by definition elements $w', w'' \in W$ and $s \in S$ such that

$$
w = w' s w'', \quad l_S(w) = l_S(w') + l_S(w'') + 1 \quad \text{and} \quad t = w' s {w'}^{-1}.
$$

By Cor. 1,

$$
C(w).C(w^{-1}) = C(w').C(s).C(w'').C({w''}^{-1}).C(s).C({w'}^{-1}).
$$

Hence,

$$
C(w).C(w^{-1}) \supset C(w').C(s).C(s).C({w'}^{-1}).
$$

By (4), $C(s) \subset C(s).C(s)$. Hence,

$$
C(w).C(w^{-1}) \supset C(w').C(s).C({w'}^{-1}) \supset C(t).
$$

#### Corollary 3 {#lie-iv-s2-thm-2-cor-3 .statement}

*Let $w \in W$ and let $H_w$ be the subgroup of $G$ generated by $C(w).C(w^{-1})$. Then:*

a) *For any reduced decomposition $(s_1, \ldots, s_q)$ of $w$,*

$$
C(s_j) \subset H_w \quad \text{for } 1 \leq j \leq q.
$$

b) *The group $H_w$ contains $C(w)$ and is generated by $C(w)$.*

We prove a) by induction on $j$. Assume that $C(s_k)$ is contained in $H_w$ for $k < j$. Let

$$
t = (s_1 \ldots s_{j-1}) s_j (s_1 \ldots s_{j-1})^{-1}.
$$

The element $t$ belongs to the subset $T_w$ of $W$ defined in Lemma 2 of § 1, no. 4. By Cor. 2, $C(t) \subset H_w$, and hence $C(s_j) \subset H_w$.

Since $C(w) = C(s_1) \ldots C(s_q)$, cf. Cor. 1, we have $C(w) \subset H_w$, and b) follows.

#### Example {#lie-iv-s2-n4-exa-1 .statement}

Th. 2, applied to the Tits system described in no. 2, shows that *the symmetric group* $\mathfrak{S}_n$, with the set of transpositions of consecutive elements, *is a Coxeter group*.

### 5. SUBGROUPS OF G CONTAINING B

For any subset X of S, we denote by W_X the subgroup of W generated by X (cf. §1, no. 8) and by G_X the union BW_XB of the double cosets C(w), w ∈ W_X. We have G_∅ = B and G_S = G.

#### Theorem 3 {#lie-iv-s2-thm-3 .statement}

a) For any subset X of S, the set G_X is a subgroup of G, generated by $\bigcup_{s \in X} C(s)$.

b) The map X ↦ G_X is a bijection from $\mathcal{P}(S)$ to the set of subgroups of G containing B.

c) Let (X_i)_{i \in I} be a family of subsets of X. If $X = \bigcap_{i \in I} X_i$, then $G_X = \bigcap_{i \in I} G_{X_i}$.

d) Let X and Y be two subsets of S. Then $G_X \subset G_Y$ (resp. $G_X = G_Y$) if and only if $X \subset Y$ (resp. $X = Y$).

It is clear that $G_X = (G_X)^{-1}$; Lemma 1 of no. 1 shows that $G_X . G_X \subset G_X$; and hence a) follows, taking into account Cor. 1 of Th. 2.

The injectivity of X ↦ G_X follows from that of X ↦ W_X (§1, no. 8, Th. 2). Conversely, let H be a subgroup of G containing B. Let U be the set of $w \in W$ such that $C(w) \subset H$. We have $H = BUB$ since H is a union of double cosets. Let $X = U \cap S$; we show that $H = G_X$. Clearly, $G_X \subset H$. On the other hand, let $u \in U$ and let $(s_1, \ldots, s_q)$ be a reduced decomposition of u. Cor. 3 of Th. 2 implies that $C(s_j) \subset H$, and hence that $s_j \in X$ for $1 \leq j \leq q$. Thus, $u \in W_X$, and since H is the union of the $C(u)$ for $u \in U$, we have $H \subset G_X$, which proves b).

Assertions c) and d) follow from analogous properties of W_X (§ 1, no. 8, Th. 2).

#### Corollary {#lie-iv-s2-n5-cor-1 .statement}

The set S consists of the elements $w \in W$ such that $w \neq 1$ and $B \cup C(w)$ is a subgroup of G.

The elements $w \in W$ such that $B \cup C(w)$ is a subgroup of G are those for which there exists $X \subset S$ with $W_X = \{1, w\}$. Moreover, if $w \neq 1$, we necessarily have Card(X) = 1 , i.e. $w \in S$.

#### Remark 1 {#lie-iv-s2-n5-rem-1 .statement}

The above corollary shows that S is determined by (G, B, N); for this reason, we sometimes allow ourselves to say that (G, B, N) is a Tits system, or that (B, N) is a Tits system in G.

#### Proposition 1 {#lie-iv-s2-prop-1 .statement}

Let X be a subset of S and N' a subgroup of N whose image in W is equal to W_X. Then, (G_X, B, N', X) is a Tits system.

We have $G_X = BW_XB = BN'B$, which shows that $G_X$ is generated by $B \cup N'$. The verification of the axioms (T1) to (T4) is now immediate.

#### Proposition 2 {#lie-iv-s2-prop-2 .statement}

Let X, Y ⊂ S and $w \in W$. We have

$$
G_X w G_Y = BW_X w W_Y B.
$$

Let $s_1, \ldots, s_q \in X$ and $t_1, \ldots, t_q \in Y$. Lemma 1 shows that
$$
C(s_1 \ldots s_q).C(w).C(t_1 \ldots t_q) \subset BW_X w W_Y B,
$$
and hence that
$$
G_X w G_Y \subset BW_X w W_Y B.
$$
The opposite inclusion is obvious.

#### Remark 2 {#lie-iv-s2-n5-rem-2 .statement}

Denote by $G_X \backslash G / G_Y$ the set of subsets of $G$ of the form $G_X g G_Y$, $g \in G$; and define $W_X \backslash W / W_Y$ analogously. The preceding proposition shows that the canonical bijection $w \mapsto C(w)$ from $W$ to $B \backslash G / B$ defines by passage to the quotient a *bijection* $W_X \backslash W / W_Y \to G_X \backslash G / G_Y$.

#### Proposition 3 {#lie-iv-s2-prop-3 .statement}

*Let $X \subset S$ and $g \in G$. The relation $g B g^{-1} \subset G_X$ implies that $g \in G_X$.*

Let $w \in W$ be such that $g \in C(w)$. Since $B$ is a subgroup of $G_X$, the hypothesis $g B g^{-1} \subset G_X$ implies that $C(w).C(w^{-1}) \subset G_X$, and hence that $C(w) \subset G_X$ by Cor. 3 of Th. 2, so $g$ belongs to $G_X$.

### 6. PARABOLIC SUBGROUPS

#### Definition 2 {#lie-iv-s2-def-2 .statement}

*A subgroup of $G$ is said to be parabolic if it contains a conjugate of $B$.*

It is clear that every subgroup that contains a parabolic subgroup is parabolic.

#### Proposition 4 {#lie-iv-s2-prop-4 .statement}

*Let $P$ be a subgroup of $G$.*

a) *$P$ is parabolic if and only if there exists a subset $X$ of $S$ such that $P$ is conjugate to $G_X$ (cf. no. 5 for the definition of $G_X$).*

b) *Let $X, X' \subset S$ and $g, g' \in G$ be such that $P = g G_X g^{-1} = g' G_{X'} {g'}^{-1}$. Then, $X = X'$ and $g' g^{-1} \in P$.*

Assertion a) follows from Th. 3, b).
Under the hypotheses of b), we have
$$
g^{-1} g' B {g'}^{-1} g \subset g^{-1} g' G_{X'} {g'}^{-1} = G_X,
$$
and Prop. 3 shows that $g^{-1} g' \in G_X$. Hence, $G_{X'} = G_X$ and $X' = X$ by Th. 3, b). Finally,
$$
g' g^{-1} = g . g^{-1} g' . g^{-1} \in g G_X g^{-1},
$$
which proves b).

If the parabolic subgroup $P$ is conjugate to $G_X$, where $X \subset S$, then $P$ is said to be of *type X*.

#### Theorem 4 {#lie-iv-s2-thm-4 .statement}

(i) Let $P_1$ and $P_2$ be two parabolic subgroups of $G$ whose intersection is parabolic and let $g \in G$ be such that $gP_1g^{-1} \subset P_2$. Then $g \in P_2$ and $P_1 \subset P_2$.

(ii) Two parabolic subgroups whose intersection is parabolic are not conjugate.

(iii) Let $Q_1$ and $Q_2$ be two parabolic subgroups of $G$ contained in a subgroup $Q$ of $G$. Then any $g \in G$ such that $gQ_1g^{-1} = Q_2$ belongs to $Q$.

(iv) Every parabolic subgroup is its own normaliser$^6$.

Assertion (i) follows from Props. 3 and 4, and implies (ii). Under the hypotheses of (iii), we have $gQ_1g^{-1} \subset Q$, which implies that $g \in Q$ by (i). Finally, (iv) follows from (iii) by taking $Q_1 = Q_2 = Q$.

#### Proposition 5 {#lie-iv-s2-prop-5 .statement}

Let $P_1$ and $P_2$ be two parabolic subgroups of $G$. Then $P_1 \cap P_2$ contains a conjugate of $T$.

By first transforming $P_1$ and $P_2$ by an inner automorphism of $G$, we may assume that $B \subset P_1$. Let $g \in G$ be such that $gB_2g^{-1} \subset P_2$. By Th. 1, there exist $n \in N$ and $b, b' \in B$ such that $g = bn b'$. Since $T$ is normal in $N$,

$$
P_2 \supset gB_2g^{-1} = bnBn^{-1}b^{-1} \supset bnTn^{-1}b^{-1} = bTb^{-1}
$$

and

$$
P_1 \supset B \supset bTb^{-1},
$$

which proves the proposition.

### 7. SIMPLICITY THEOREMS

#### Lemma 2 {#lie-iv-s2-lem-2 .statement}

Let $H$ be a normal subgroup of $G$. There exists a subset $X$ of $S$ such that $BH = G_X$ and such that every element of $X$ commutes with every element of $S - X$.

Since $BH$ is a subgroup of $G$ containing $B$, there exists a unique subset $X$ of $S$ such that $BH = G_X$ (Th. 3).

Let $s_1 \in X$ and $s_2 \in S - X$; let $n_1$ and $n_2$ be representatives in $N$ of $s_1$ and $s_2$, respectively. Then $n_1 \in G_X = BH$ and there exists $b \in B$ such that $bn_1 \in H$. Since $H$ is normal in $G$, the element $h = n_2 b n_1 n_2^{-1}$ of $G$ belongs to $H$. This means that

$$
h \in C(s_2).C(s_1).C(s_2).
$$

If the length of $s_2 s_1 s_2$ is equal to 3, Cor. 1 of Th. 2 implies that

$$
C(s_2).C(s_1).C(s_2) = C(s_2 s_1 s_2),
$$

(6) If $H$ is a subgroup of a group $G$, the normaliser of $H$ in $G$ is the subgroup $\mathfrak{N}(H)$ consisting of the elements $g$ of $G$ such that $gHg^{-1} = H$. A subgroup $H'$ is said to normalise $H$ if $H' \subset \mathfrak{N}(H)$, in which case $HH' = H'H$ is a subgroup of $G$ in which $H$ is normal.

and hence that $h \in H \cap C(s_2 s_1 s_2)$. Since $H \cap C(s_2 s_1 s_2)$ is non-empty, $s_2 s_1 s_2 \in W_X$. As $(s_2, s_1, s_2)$ is a reduced decomposition, it follows that $s_2 \in X$, contrary to our assumption.

Thus $l_S(s_2 s_1 s_2) \leq 2$; if $l_S(s_2 s_1 s_2) = 1$, then $s_1 s_2 \in S$ and so $(s_1 s_2)^2 = 1$, or $s_1 s_2 = s_2 s_1$. If $l_S(s_2 s_1 s_2) = 2$, property (E) of §1, no. 5 implies that $s_2 s_1 = s_1 s_2$, since $s_1 \neq s_2$. Q.E.D.

The following property of a group U enters into Th. 5 below:

(R) *For any normal subgroup V of U distinct from U, the commutator subgroup* (cf. *Algebra*, Chap. I, §6, no. 8) *of U/V is distinct from U/V*.

Every soluble group satisfies (R); in particular, every abelian group satisfies (R). It can be shown that the symmetric group $\mathfrak{S}_n$ satisfies (R) (cf. Exerc. 29).

#### Theorem 5 {#lie-iv-s2-thm-5 .statement}

*Let Z be the intersection of the conjugates of B, let U be a subgroup of B and let G_1 be the subgroup generated by the conjugates of U in G. We make the following assumptions:*

(1) *U is normal in B and B = UT*.
(2) *U has property (R)*.
(3) *G_1 is equal to its commutator subgroup*.
(4) *The Coxeter system (W, S) is irreducible* (cf. §1, no. 9).

*Then every subgroup H of G normalised by G_1 is either contained in Z or contains G_1*.

*First we show that G = G_1 T*. The group $G_1 T$ contains B and hence is its own normaliser (Th. 4); but as N normalises $G_1$ and T, it also normalises $G_1 T$, so $N \subset G_1 T$. Since G is generated by B and N, it follows that $G = G_1 T$.

*Next, set*

$$
G' = G_1 H, \quad B' = B \cap G', \quad N' = N \cap G',
T' = T \cap G' = B' \cap N' \quad \text{and} \quad W' = N'/T'.
$$

We have $G = G'T$ since $G'$ contains $G_1$, and hence $N = N'T$. The inclusion of $N'$ into N thus defines, on passing to the quotient, an isomorphism $\alpha : W' \to W$. Let $S' = \alpha^{-1}(S)$.

*We now show that (G', B', N', S') is a Tits system*. Since $G = BNB$ and $B = TU = UT$, we have $G = UNU$. Since U is a subgroup of $G'$, it follows that $G' = UN'U$; since $U \subset B'$, this proves (T1). Axiom (T2) is satisfied since $\alpha$ is an isomorphism. Let $w \in W$ and let $w' = \alpha^{-1}(w)$ be the corresponding element of $W'$. We have

$$
BwB = BwB' = Bw'B', \quad \text{since } B = B'T.
$$

From this we conclude that $G' \cap BwB = B'w'B'$, which means that the inclusion of $G'$ into G defines on passing to the quotient a bijection from

B'\setminus G'/B' to B\setminus G/B. Axiom (T3) follows immediately. Axiom (T4) follows from B = B'T.

The subgroup H is normal in G'. By Lemma 2 applied to (G', B', N', S'), there exists a subset X' of S' such that B'H = G'_X', and every element of S' - X' commutes with every element of X'. In view of assumption (4), there are only two possibilities:

a) X' = \varnothing, i.e. B'H = B', so H \subset B' \subset B. If g \in G, then g = g_1 t with g_1 \in G_1, t \in T, and H \subset g_1 B g_1^{-1} since G_1 normalises H. Thus H \subset g B g^{-1}, and since Z is the intersection of the g B g^{-1}, we have H \subset Z.

b) X' = S', i.e. B'H = G'. Since G = G'T, we have

$$ G = B'HT = HB'T = HB. $$

As B normalises U, every conjugate of U is of the form hUh^{-1} with h \in H. Such a subgroup is contained in the group UH, hence G_1 \subset UH by the definition of G_1. Thus, we have the isomorphisms

$$ U/(U \cap H) \cong UH/H = G_1 H/H \cong G_1/(G_1 \cap H). $$

By assumption (3), G_1/(G_1 \cap H) is equal to its commutator subgroup. Assumption (2) now shows that the group U/(U \cap H), which is isomorphic to G_1/(G_1 \cap H), reduces to the identity element. Hence G_1 \cap H = G_1 and G_1 \subset H, which completes the proof.

#### Corollary {#lie-iv-s2-n7-cor-1 .statement}

Under the assumptions of Th. 5, the group G_1/(G_1 \cap Z) is either simple non-abelian or reduces to the identity element.

Th. 5 shows that G_1/(G_1 \cap Z) is simple or reduces to the identity element. On the other hand, assumption (3) implies that it is equal to its commutator subgroup. Hence the corollary.

#### Remark 1 {#lie-iv-s2-n7-rem-1 .statement}

Assumptions (2), (3), (4) were not used in the proof that (G', B', N', S') is a Tits system.

#### Remark 2 {#lie-iv-s2-n7-rem-2 .statement}

Suppose that Z \cap U = \{1\}. Since Z and U are normal in B, it follows that every element of Z commutes with every element of U, and hence with every element of G_1. In view of the preceding corollary, it follows that G_1 \cap Z is the centre of G_1.

#### Remark 3 {#lie-iv-s2-n7-rem-3 .statement}

Assumption (3) is implied by the following condition:

(3') U is generated by the commutators b^{-1} u^{-1} b u with u \in U and b \in B \cap G_1.

#### Example 1 {#lie-iv-s2-n7-exa-1 .statement}

Let k be a field, n an integer \geqslant 0, G = \mathbf{GL}(n, k), and let (G, B, N, S) be the Tits system described in no. 2. Let U be the strictly upper triangular subgroup of G, i.e. the subgroup of B consisting of the matrices whose diagonal entries are equal to 1. Condition (1) in Th. 5 is immediate, and so is (2) since U is soluble. Condition (4) is satisfied if $n \geq 2$. One can show (cf. *Algebra*, Chap. II, § 10, Exerc. 13) that (3) is satisfied if $n \geq 3$ and Card$(k) \geq 4$. Under these conditions, we conclude that $G_1 / (G_1 \cap Z)$ is *simple* and that $G_1 \cap Z$ is the centre of $G_1$ (cf. *Remark* 2).

When $k$ is commutative, $G_1 = \mathbf{SL}(n, k)$ (cf. *Algebra*, Chap. III, § 8, no. 9).

#### Example 2 {#lie-iv-s2-n7-exa-2 .statement}

Let $g$ be a simple Lie algebra over $\mathbf{C}$, and let $G$ be the group of inner automorphisms of $g$ (cf. Chap. III, § 6, no. 2, Prop. 2). By using Th. 5, one can show that $G$ is simple non-abelian.*

### Exercises {#lie-iv-s2-exercises}

See the [exercises for § 2](exercises/s2/).
