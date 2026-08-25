---
book: top
book_title: General Topology
chapter: I
chapter_title: Topological Structures
section: 5
section_title: Open mappings and closed mappings
lang: en
source: top-i-iv
pdf_pages: 0056-0063, 0133-0134
extraction: ocr
subsections:
    - "no": 1
      title: OPEN MAPPINGS AND CLOSED MAPPINGS
      page: 0
      pdf_page: 56
    - "no": 2
      title: OPEN EQUIVALENCE RELATIONS AND CLOSED EQUIVALENCE RELATIONS
      page: 0
      pdf_page: 58
    - "no": 3
      title: PROPERTIES PECULIAR TO OPEN MAPPINGS
      page: 0
      pdf_page: 60
    - "no": 4
      title: PROPERTIES PECULIAR TO CLOSED MAPPINGS
      page: 0
      pdf_page: 62
statements: 19
exercises: 7
content_sha256: 4bd44bbdc7549036da9b797314f4f397254ee681b4ed5c187bdeceb598f632df
---

## 5. OPEN MAPPINGS AND CLOSED MAPPINGS

### 1. OPEN MAPPINGS AND CLOSED MAPPINGS

#### Definition 1 {#top-i-s5-def-1 .statement}

*Let $X, X'$ be two topological spaces. A mapping $f : X \to X'$ is open (resp. closed) if the image under $f$ of each open (resp. closed) set of $X$ is open (resp. closed) in $X'$.*

In particular, $f(X)$ is then an open (resp. closed) subset of $X'$.

#### Example 1 {#top-i-s5-n1-exa-1 .statement}

Let $A$ be a subspace of a topological space $X$. Then the canonical injection $j : A \to X$ is open (resp. closed) if and only if $A$ is open (resp. closed) in $X$ (\S 3, no. 1).
2) For a bijection $f$ of a topological space $X$ onto a topological space $X'$ to be a *homeomorphism* it is necessary and sufficient that $f$ is *continuous and open*, or *continuous and closed*.

3) Let $f$ be a surjection of a set $X$ onto a topological space $X'$; if we give $X$ the topology which is the inverse image under $f$ of the topology of $X'$ (\$ 2, no. 3, Example 1), then $f$ is continuous, open and closed.

4) In a product space
$$
X = \prod_{i \in I} X_i,
$$
each projection $\mathrm{pr}_i : X \to X_i$ is a continuous open mapping, but is not necessarily closed (\$ 4, no. 2, Proposition 5).

\* 5) A holomorphic function on an open subset $A$ of $C$ is an open mapping of $A$ into $C$. \*
6) Let $X, X'$ be two topological spaces and $f$ a continuous, but not bicontinuous, bijection of $X$ onto $X'$. Then the inverse bijection $g : X' \to X$ is an open and closed mapping of $X'$ onto $X$, but is not continuous.

#### Proposition 1 {#top-i-s5-prop-1 .statement}

*Let $X, X', X''$ be three topological spaces, and let $f : X \to X', \ g : X' \to X''$ be two mappings. Then:*

a) *If $f$ and $g$ are open (resp. closed), so is $g \circ f$.*

b) *If $g \circ f$ is open (resp. closed) and if $f$ is continuous and surjective, then $g$ is open (resp. closed).*

c) *If $g \circ f$ is open (resp. closed) and if $g$ is continuous and injective, then $f$ is open (resp. closed).*

From Definition 1. a) follows immediately. To prove b) it is enough to remark that every open (resp. closed) subset $A'$ of $X'$ can be written as $f(A)$, where $A = f^{-1}(A')$ is open (resp. closed) in $X$ (\$ 2, no. 1, Theorem 1); hence $g(A') = g(f(A))$ is open (resp. closed) in $X''$. Finally, to prove c), we remark that $f(A) = g^{-1}(g(f(A)))$ for every subset $A$ of $X$; by hypothesis, if $A$ is open (resp. closed) in $X$, then $g(f(A))$ is open (resp. closed) in $X''$, hence $f(A)$ is open (resp. closed) in $X'$ by \$ 2, no. 1, Theorem 1.

#### Proposition 2 {#top-i-s5-prop-2 .statement}

*Let $X, Y$ be two topological spaces, $f$ a mapping of $X$ into $Y$. For each subset $T$ of $Y$ let $f_T$ denote the mapping of $f^{-1}(T)$ into $T$ which agrees with $f$ on $f^{-1}(T)$.*

a) *If $f$ is open (resp. closed), $f_T$ is open (resp. closed).*

b) *Let $(T(i))_{i \in I}$ be a family of subsets of $Y$ whose interiors cover $Y$, or which is a locally finite closed covering of $Y$; if all the $f_{T(i)}$ are open (resp. closed), then $f$ is open (resp. closed).*

a) If $A$ is an open (resp. closed) subset of $f^{-1}(T)$, then there is an open (resp. closed) subset $B$ of $X$ such that $A = B \cap f^{-1}(T)$, and therefore f_T(A) = f(B) \cap T; by hypothesis, $f(B)$ is open (resp. closed), so that $f_T(A)$ is open (resp. closed) in $T$.

$b)$ Let $B$ be an open (resp. closed) subset of $X$, and let $B_i$ denote $B \cap f^{-1}(T(i))$; then $f(B) \cap T(i) = f_{T(i)}(B_i)$. Since $f_{T(i)}(B_i)$ is open (resp. closed) in $T(i)$ by hypothesis, it follows that $f(B)$ is open (resp. closed) in $Y$, by Proposition 3 of § 3, no. 1.

#### Corollary {#top-i-s5-n1-cor-1 .statement}

*Let $(T(i))_{i \in I}$ be a family of subsets of $Y$ whose interiors cover $Y$, or which is a locally finite closed covering of $Y$. If $f : X \to Y$ is continuous and if each of the $f_{T(i)}$ is a homeomorphism of $f^{-1}(T(i))$ onto $T(i)$, then $f$ is a homeomorphism of $X$ onto $Y$.*

For $f$ is clearly bijective, and is open by virtue of Proposition 2.

### 2. OPEN EQUIVALENCE RELATIONS AND CLOSED EQUIVALENCE RELATIONS

#### Definition 2 {#top-i-s5-def-2 .statement}

*An equivalence relation $R$ on a topological space $X$ is said to be open (resp. closed) if the canonical mapping of $X$ onto $X/R$ is open (resp. closed).*

It comes to the same thing to say that the *saturation* of each open (resp. closed) subset of $X$ with respect to $R$ is open (resp. closed) in $X$ (\S 3, no. 4).

#### Example 1 {#top-i-s5-n2-exa-1 .statement}

Let $X$ be a topological space, $\Gamma$ a *group of homeomorphisms* of $X$ onto itself, and let $R$ be the equivalence relation

"there exists $\sigma \in \Gamma$ such that $y = \sigma(x)$"

between $x$ and $y$ (thus $R$ is the equivalence relation whose classes are the *orbits* of $\Gamma$ in $X$. The relation $R$ is *open*, for the saturation of a subset $A$ of $X$ with respect to $R$ is open so is each $\sigma(A)$ and hence so is their union.

\* On the real line $\mathbf{R}$ the equivalence relation $x \equiv y \pmod{1}$ is open, since it is derived as above from the group of translations

$$
x \to x + n \qquad (n \in \mathbf{Z})
$$

(see Chapter III, § 2, no. 4). \*

#### Example 2 {#top-i-s5-n2-exa-2 .statement}

Let $X$ be the sum of a family $(X_i)$ of subspaces of $X$, and let $X/R$ be the space obtained by *pasting together* the $X_i$ along *open* subsets $A_{ix}$ by means of bijections $h_{ix}$ (\S 2, no. 5); and suppose that $h_{ix}$ is a *homeomorphism* of $A_{ix}$ onto $A_{x'}$ for each pair of indices $(i, x)$.

Then the relation R is open. For if U is open in X, the saturation of U is the union of the $h_{x!}(U \cap A_{ix})$; since $U \cap A_{ix}$ is open in $A_{ix}$, $h_{x!}(U \cap A_{ix})$ is open in $A_{ix}$ and therefore in X.

#### Example 3 {#top-i-s5-n2-exa-3 .statement}

With the notation of Example 2, suppose now that the $A_{ix}$ are closed and the $h_{x!}$ are homeomorphisms; further suppose that for each index i there is only a finite number of indices x such that $A_{ix} \neq \varnothing$ (i.e. each $X_i$ is "stuck" to only a finite number of $X_x$). Then the relation R is closed. For if F is any closed subset of X, the saturation of F is the union of the sets $h_{x!}(F \cap A_{ix}) \subset A_{ix}$; the assumptions made imply that this family is locally finite, and $h_{x!}(F \cap A_{ix})$ is closed in $A_{ix}$ and therefore in X. The result therefore follows from Proposition 4 of § 1, no. 5.

#### Proposition 3 {#top-i-s5-prop-3 .statement}

Let X, Y be two topological spaces, let $f : X \to Y$ be a continuous mapping, let R be the equivalence relation $f(x) = f(y)$ on X, and let $X \xrightarrow{p} X/R \xrightarrow{h} f(X) \xrightarrow{i} Y$ be the canonical decomposition of f. Then the following three statements are equivalent:

a) f is an open mapping.

b) The three mappings p, h, i are open.

c) The equivalence relation R is open, h is a homeomorphism, and $f(X)$ is an open subset of Y.

Also the preceding proposition remains true if "open" is replaced by "closed" throughout.

Since the injection i is continuous, it follows from Proposition 1 c) of no. 1 that if f is open then so is $h \circ p$; since p is surjective and continuous, Proposition 1 b) shows that h is open; h is in any case a continuous bijection; thus h is a homeomorphism, and therefore, from Proposition 1 a) of no. 1, $p = \overline{h}^{-1} \circ (h \circ p)$ is an open mapping. Also [no. 1, Proposition 1 b)] $i \circ h$ is open; hence [no. 1, Proposition 1 a)] so is $i = (i \circ h) \circ \overline{h}^{-1}$. This proves that a) implies b). Conversely, Proposition 1 a) of no. 1 shows that b) implies a). Finally, the equivalence of b) and c) follows immediately from the definitions.

The proof in the case of closed mappings is analogous, mutatis mutandis.

#### Proposition 4 {#top-i-s5-prop-4 .statement}

Let R be an open (resp. closed) equivalence relation on a topological space X, and f the canonical mapping $X \to X/R$. Let A be a subset of X and suppose that one of the following two conditions is satisfied:

a) A is open (resp. closed) in X.

b) A is saturated with respect to R.

Then the relation $R_A$ induced on A is open (resp. closed) and the canonical mapping of $A/R_A$ onto $f(A)$ is a homeomorphism.

Consider the commutative diagram (i) of § 3, no. 6, which gives the canonical decomposition of $f \circ j$. Under condition a), $j$ is open (resp. closed) and so is $f$ by hypothesis; hence $f \circ j$ is open (resp. closed) [no. 1, Proposition 1 a)], and the result follows from Proposition 3. Under condition b) we have
$$
A = \overline{f}^{-1}(f(A)),
$$
and $h \circ \varphi$ is the mapping of $A$ into $f(A)$ which agrees with $f$ on $A$; by virtue of Proposition 2 a) of no. 1, $h \circ \varphi$ is open (resp. closed), and the result again follows from Proposition 3, applied to $h \circ \varphi$.

### 3. PROPERTIES PECULIAR TO OPEN MAPPINGS

#### Proposition 5 {#top-i-s5-prop-5 .statement}

*Let $X, Y$ be two topological spaces, $f$ a mapping of $X$ into $Y, \mathcal{B}$ a base of the topology of $X$. Then the following statements are equivalent*:

a) *$f$ is an open mapping*.

b) *For each $U \in \mathcal{B}$, $f(U)$ is open in $Y$*.

c) *For each $x \in X$ and each neighbourhood $V$ of $x$ in $X$, $f(V)$ is a neighbourhood of $f(x)$ in $Y$*.

The equivalence of a) and b) follows immediately from the definitions and from $(O_1)$; the equivalence of a) and c) is a consequence of Proposition 1 of § 1, no. 2.

#### Proposition 6 {#top-i-s5-prop-6 .statement}

*Let $R$ be an equivalence relation on a topological space $X$; then the following three conditions are equivalent*:

a) *The relation $R$ is open*.

b) *The interior of each subset which is saturated with respect to $R$ is saturated with respect to $R$*.

c) *The closure of each subset which is saturated with respect to $R$ is saturated with respect to $R$*.

By taking complements ($§ 1$, no. 6, formula (2)) we see that b) and c) are equivalent. Let us show that b) implies a): suppose condition b) is satisfied and let $U$ be an open subset of $X$, $V$ its saturation with respect to $R$; then $\dot{V} \supset U$, and since by hypothesis $\dot{V}$ is saturated, it follows that $\dot{V} = V$, and therefore the saturation of $U$ is open. Conversely, suppose condition a) is satisfied, and let $A$ be a saturated set; if $B$ is the saturation of $\dot{A}$, then $\dot{A} \subset B \subset A$, and since $B$ is open by hypothesis it follows that $B = \dot{A}$.

#### Proposition 7 {#top-i-s5-prop-7 .statement}

Let $R$ be an open equivalence relation on a topological space $X$, and let $\varphi : X \to X/R$ be the canonical mapping. If $A$ is any subset of $X$ which is saturated with respect to $R$, then the closure (resp. the interior) of $\varphi(A)$ in $X/R$ is $\varphi(\overline{A})$ (resp. $\varphi(\overset{\circ}{A})$).

Each of the two assertions of the proposition can be deduced from the other by taking complements and using formula (2) of § 1, no. 6 and the fact that if $B$ is a saturated subset of $X$ then $\varphi(\complement B) = \complement_{\varphi}(B)$. By virtue of Proposition 6, $\overline{A}$ is saturated; hence $\varphi(\overline{A})$ is closed in $X/R$, and since $A \subset \overline{A}$ we have $\varphi(A) \subset \varphi(\overline{A})$, so that $\varphi(A) \subset \varphi(\overline{A})$. But since $\varphi$ is continuous, $\varphi(\overline{A}) \subset \varphi(A)$ (\S 2, no. 1, Theorem 1), and the result follows.

#### Proposition 8 {#top-i-s5-prop-8 .statement}

Let $(X_i)_{i \in I}, (Y_i)_{i \in I}$ be two families of topological spaces indexed by the same set $I$. For each $i \in I$ let $f_i$ be an open mapping of $X_i$ into $Y_i$, and suppose that $f_i$ is surjective for all but a finite number of indices. Then the product mapping $f : (x_i) \to (f_i(x_i))$ of $\prod_{i \in I} X_i$ into $\prod_{i \in I} Y_i$ is open.

By virtue of Proposition 5 we need only prove that the image under $f$ of any elementary set $\prod_{i \in I} A_i$ in $\prod_{i \in I} X_i$ is open in $\prod_{i \in I} Y_i$. But this image is $\prod_{i \in I} f_i(A_i)$, and the hypotheses imply that $f_i(A_i)$ is open in $Y_i$ for each $i \in I$, and that $f_i(A_i) = Y_i$ for all but a finite number of indices; whence the result.

#### Corollary {#top-i-s5-n3-cor-1 .statement}

Let $(X_i)_{i \in I}$ be a family of topological spaces, and for each $i \in I$ let $R_i$ be an equivalence relation on $X_i$, and let $f_i$ be the canonical mapping $X_i \to X_i/R_i$. Let $R$ be the equivalence relation in $X = \prod_{i \in I} X_i$

"for each $i \in I$, $\operatorname{pr}_i(x) = \operatorname{pr}_i(y)$ (mod $R_i$)"

between $x$ and $y$, and let $f$ be the product mapping $(x_i) \to (f_i(x_i))$ of $X$ into $\prod_{i \in I} (X_i/R_i)$. If each of the relations $R_i$ is open, then the relation $R$ is open, and the bijection associated with $f$ is a homeomorphism of $X/R$ onto $\prod_{i \in I} (X_i/R_i)$.

$R$ is the relation $f(x) = f(y)$. Since $f$ is continuous and open by Proposition 8 above and § 4, no. 1, Corollary 1 of Proposition 1, the result follows from Proposition 3 of no. 2.

In particular, if $R$ (resp. $S$) is an open equivalence relation on a topological space $X$ (resp. $Y$), then the canonical bijection of

$$
(X \times Y)/(R \times S) \quad \text{onto} \quad (X/R) \times (Y/S)
$$

is a homeomorphism. If R and S are not assumed to be open, this bijection is continuous but is not necessarily a homeomorphism, even if one of the relations R, S is the relation of equality (Exercise 6).

### 4. PROPERTIES PECULIAR TO CLOSED MAPPINGS

#### Proposition 9 {#top-i-s5-prop-9 .statement}

Let X, X' be two topological spaces. A necessary and sufficient condition for a mapping f : X → X' to be continuous and closed is that f(Ā) = f(A) for every subset A of X.

The condition is sufficient, for it obviously implies that f is closed, and it also implies that f is continuous by reason of § 2, no. 1, Theorem 1. Conversely, if f is continuous and closed, we have f(A) ⊂ f(Ā) ⊂ f(A) by § 2, no. 1, Theorem 1; also f(Ā) is closed in X' by hypothesis; hence f(Ā) = f(A).

#### Proposition 10 {#top-i-s5-prop-10 .statement}

Let R be an equivalence relation on a topological space X. Then R is closed if and only if every equivalence class M mod R possesses a fundamental system of neighbourhoods which are saturated with respect to R.

Suppose R is closed, and let U be an arbitrary open neighbourhood of M; since F = ĈU is closed in X, the saturation S of F with respect to R is closed in X. Since M is saturated with respect to R, we have M ∩ S = ∅, and thus V = ĈS is an open neighbourhood of M, saturated with respect to R and contained in U.

To prove the converse, let F be any closed subset of X. Let T be the saturation of F with respect to R, let x be a point of ĈT, and let M be the equivalence class of x; then M ∩ T = ∅ and a fortiori M ∩ F = ∅, so that U = ĈF is a neighbourhood of M. Hence there is a neighbourhood V ⊂ U of M such that V is saturated with respect to R; V does not meet F, hence does not meet T, so that ĈT is a neighbourhood of M and therefore of x. This shows that ĈT is open (§ 1, no. 2, Proposition 1), i.e. T is closed.

#### Remark {#top-i-s5-n4-rem-1 .statement}

Proposition 10 implies the following: if R is closed and if φ denotes the canonical mapping X → X/R, then for each x ∈ X and each neighbourhood U of the equivalence class of x in X, φ(U) is a neighbourhood of φ(x) in X/R. It should be carefully noticed that this statement by no means implies that for every neighbourhood V of x, φ(V) is a neighbourhood of φ(x); in other words (no. 3, Proposition 5) a closed equivalence relation is not necessarily open (Exercise 2). Conversely, an open equivalence relation is not necessarily closed (no. 1, Example 4);

for if $U$ is a neighbourhood in $X$ of an equivalence class $M$, then for each $x \in M$ and each neighbourhood $V \subset U$ of $x$, the saturation of $V$ is certainly a neighbourhood of $M$ in $X$, but this neighbourhood is *not necessarily contained in* $U$.

Finally, there are equivalence relations other than equality which are both open and closed (Exercise 3) and equivalence relations which are neither open nor closed ($\S 8$, Exercise 10).

### Exercises {#top-i-s5-exercises}

See the [exercises for § 5](exercises/s5/).
