---
book: top
book_title: General Topology
chapter: I
chapter_title: Topological Structures
section: 10
section_title: Proper mappings
lang: en
source: top-i-iv
pdf_pages: 0103-0113, 0156-0161
extraction: ocr
subsections:
    - "no": 1
      title: PROPER MAPPINGS
      page: 0
      pdf_page: 103
    - "no": 2
      title: CHARACTERIZATION OF PROPER MAPPINGS BY COMPACTNESS PROPERTIES
      page: 0
      pdf_page: 107
    - "no": 3
      title: PROPER MAPPINGS INTO LOCALLY COMPACT SPACES
      page: 0
      pdf_page: 110
    - "no": 4
      title: QUOTIENT SPACES OF COMPACT SPACES AND LOCALLY COMPACT SPACES
      page: 0
      pdf_page: 111
statements: 25
exercises: 8
content_sha256: a1ec5404bc216e6059c71632bd54b95434a91b8772e2e71228f45d94583c0177
---

## 10. PROPER MAPPINGS

*In this section we denote by $ \iota_X $ the identity mapping of a set $ X $ onto itself.*

### 1. PROPER MAPPINGS

If $ f : X \to Y $ and $ f' : X' \to Y' $ are two *continuous closed* mappings, the product $ f \times f' : X \times X' \to Y \times Y' $ is not necessarily a closed map, even if $ f $ is of the form $ \iota_X $.

#### Example {#top-i-s10-n1-exa-1 .statement}

Every constant mapping into a Hausdorff space is closed. But it $ f $ is the constant mapping $ Q \to 0 $, then $ f \times \iota_Q $ is the mapping $ (x, y) \to (0, y) $ of $ Q^2 $ into $ Q^2 $, so it is the second projection and is not closed (\S 4, no. 2, Remark 1).

#### Definition 1 {#top-i-s10-def-1 .statement}

*Let $ f $ be a mapping of a topological space $ X $ into a topological space $ Y $. $ f $ is said to be proper if $ f $ is continuous and if the mapping $ f \times \iota_Z : X \times Z \to Y \times Z $ is closed, for every topological space $ Z $.*

We shall give other characterizations of proper mappings in no. 2 and 3.

If in Definition 1 we take the space $ Z $ to consist of a single point, we see that:

#### Proposition 1 {#top-i-s10-prop-1 .statement}

*Every proper mapping is closed.*

#### Proposition 2 {#top-i-s10-prop-2 .statement}

*Let $ f : X \to Y $ be a continuous injection. Then the following three statements are equivalent:*
a) $ f $ is proper.
b) $ f $ is closed.
c) $ f $ is a homeomorphism of $ X $ onto a closed subset of $ Y $.

We have just seen that a) implies b). Since the equivalence relation $ f(x) = f(x') $ is the equality relation, the quotient space of $ X $ with respect to this relation can be identified with $ X $; hence b) implies c) by reason of § 5, no. 2, Proposition 3. Finally, if c) is satisfied then $ f \times \iota_Z $ is a homeomorphism of $ X \times Z $ onto a closed subspace of $ Y \times Z $ and is therefore a closed mapping; hence c) implies a).

#### Proposition 3 {#top-i-s10-prop-3 .statement}

*Let $ f : X \to Y $ be a continuous mapping. If $ T $ is any subset of $ Y $, let $ f_T $ denote the mapping $ \overline{f}^{-1}(T) \to T $ which agrees with $ f $ on $ \overline{f}^{-1}(T) $.*
a) *If $ f $ is proper, so is $ f_T $.*
b) *Let $ (T(i))_{i \in I} $ be a family of subsets of $ Y $ whose interiors cover $ Y $, or which is a locally finite closed covering of $ Y $; then if each of the mappings $ f_{T(i)} $ is proper, so is $ f $.*

Let $ Z $ be a topological space. If $ T $ is any subset of $ Y $, we have
$$
f_T \times \iota_Z = (f \times \iota_Z)_{T \times Z};
$$
if $ f $ is proper, then $ f \times \iota_Z $ is closed, hence so is $ (f \times \iota_Z)_{T \times Z} $ [§ 5, no. 1, Proposition 2 a)], whence a) is proved. If now $ (T(i))_{i \in I} $ satisfies one of the two conditions stated in b), then the covering $ (T(i) \times Z)_{i \in I} $ of $ Y \times Z $ has the same property; if the $ f_{T(i)} $ are proper then the mappings
$$
(f \times \iota_Z)_{T(i) \times Z}
$$
are closed, whence $ f \times \iota_Z $ is closed [§ 5, no. 1, Proposition 2 b)]. This completes the proof.

#### Proposition 4 {#top-i-s10-prop-4 .statement}

*Let $ I $ be a finite set and for each $ i \in I $ let $ f_i : X_i \to Y_i $ be a continuous mapping. Let $ X = \prod_{i \in I} X_i, \ Y = \prod_{i \in I} Y_i, $ and let $ f : X \to Y $* be the product mapping $ (x_i) \to (f_i(x_i)) $. Then:
a) *If each of the $ f_i $ is proper, then $ f $ is proper.*
b) *If $ f $ is proper and if the $ X_i $ are non-empty, then each of the $ f_i $ is proper.*

(We shall see in no. 2, Theorem 1, Corollary 3, that this proposition extends to infinite products.)

By induction it is enough to consider the case where $ I = \{1, 2\} $.
a) Suppose that $ f_1, f_2 $ are proper, and let $ Z $ be a topological space; $ f_1 \times f_2 \times \iota_Z $ is the composition of $ \iota_{Y_1} \times f_2 \times \iota_Z $ and
$$
f_1 \times \iota_{X_2} \times \iota_Z;
$$
these two mappings are closed by hypothesis, hence so is $ f_1 \times f_2 \times \iota_Z $ [\S 5, no. 1, Proposition 1 a)], whence $ f_1 \times f_2 $ is proper.

b) Now suppose $ f $ is proper. Let $ F $ be a closed subset of $ X_2 \times Z $ and let $ G $ be the image of $ F $ in $ Y_2 \times Z $ under the mapping $ f_2 \times \iota_Z $. Then the image of $ X_1 \times F $ in $ Y_1 \times Y_2 \times Z $ under $ f_1 \times f_2 \times \iota_Z $ is $ f_1(X_1) \times G $. By hypothesis, this is closed in $ Y_1 \times Y_2 \times Z $; if $ X_1 \neq \emptyset $, then $ f_1(X_1) $ is not empty, which implies that $ G $ is closed in $ Y_2 \times Z $ (\S 4, no. 3, Corollary to Proposition 7); hence $ f_2 $ is proper. Similarly $ f_1 $ is proper if $ X_2 \neq \emptyset $.

#### Proposition 5 {#top-i-s10-prop-5 .statement}

*Let $ f : X \to X' $ and $ g : X' \to X'' $ be two continuous mappings.*
a) *If $ f $ and $ g $ are proper, then $ g \circ f $ is proper.*
b) *If $ g \circ f $ is proper and $ f $ is surjective, then $ g $ is proper.*
c) *If $ g \circ f $ is proper and $ g $ is injective, then $ f $ is proper.*
d) *If $ g \circ f $ is proper and $ X' $ is Hausdorff, then $ f $ is proper.*

Let $ Z $ be a topological space. We have
$$
(g \circ f) \times \iota_Z = (g \times \iota_Z) \circ (f \times \iota_Z);
$$
if $ f $ and $ g $ are proper, then $ f \times \iota_Z $ and $ g \times \iota_Z $ are closed; hence [\S 5, no. 1, Proposition 1 a)] $ (g \circ f) \times \iota_Z $ is closed; this proves a). The proof of b) [resp. c)] runs along the same lines, using part b) [resp. c)] of Proposition 1 of \S 5, no. 1, and remarking that if $ f $ is surjective (resp. if $ g $ is injective) then $ f \times \iota_Z $ is surjective (resp. $ g \times \iota_Z $ is injective). Finally, to prove d), consider the commutative diagram

$$
\begin{array}{ccc}
X & \overset{\varphi}{\to} & X \times X' \\
f \downarrow & & \downarrow (g \circ f) \times \iota_{X'} \\
X' & \underset{\psi}{\to} & X'' \times X'
\end{array}
$$

where $ \varphi(x) = (x, f(x)) $ and $ \psi(x') = (g(x'), x') $. The mapping $ \varphi $ (resp. $ \psi $) is a homeomorphism of $ X $ (resp. $ X' $) onto the graph of $ f $ (resp. the reflection of the graph of $ g $) (\S 4, no. 1, Proposition 1, Corollary 2). Further, since $ X' $ is Hausdorff, the graph $ \varphi(X) $ of $ f $ is closed in $ X \times X' $ (\S 8, no. 1, Proposition 2, Corollary 2). Hence (Proposition 2) $ \varphi $ is proper; on the other hand Proposition 4 shows that $ (g \circ f) \times i_{X'} $ is proper. By a) above and the commutativity of the diagram (1), $ \psi \circ f $ is proper; but $ \psi $ is injective and therefore $ f $ is proper by c) above.

#### Remark {#top-i-s10-n1-rem-1 .statement}

If $ X' $ is not Hausdorff it can happen that $ g \circ f $ is proper and $ f $ not; for example, take $ X $ and $ X'' $ to consist of one point and $ X' $ to consist of two points, with the coarsest topology.

Corollary 1. *If $ f : X \to Y $ is a proper mapping, then the restriction of $ f $ to a closed subset $ F $ of $ X $ is a proper mapping of $ F $ into $ Y $.*

For this restriction is the composition $ f \circ j $, where $ j : F \to X $ is the canonical injection, which is proper by Proposition 2.

Corollary 2. *Let $ f : X \to Y $ be a proper mapping, where $ X $ is Hausdorff. Then the subspace $ f(X) $ of $ Y $ is Hausdorff.*

By reason of Proposition 5 c) we need only consider the case where $ f(X) = Y $. Then the diagonal of $ Y \times Y $ is the image under $ f \times f $ of the diagonal of $ X $, which is closed (\S 8, no. 1, Proposition 1); $ f \times f $ is proper (Proposition 4); hence the diagonal of $ Y \times Y $ is closed (Proposition 1) and therefore $ Y $ is Hausdorff (\S 8, no. 1, Proposition 1).

Corollary 3. *Let $ I $ be a finite set and for each $ i \in I $, let $ f_i : X \to Y_i $ be a proper mapping. If $ X $ is Hausdorff, then the mapping $ x \mapsto (f_i(x)) $ of $ X $ into $ \prod_{i \in I} Y_i $ is proper.*

This mapping is the composition of the product mapping $ (x_i) \mapsto (f_i(x_i)) $ of $ X^I $ into $ \prod_i Y_i $ and the diagonal mapping of $ X $ into $ X^I $; since the latter is proper (by Proposition 2 and \S 8, no. 1, Proposition 1) the conclusion follows from Proposition 4 and Proposition 5 a).

Corollary 4. *Let $ X $ and $ Y $ be two topological spaces, $ f : X \to Y $ a continuous mapping, $ R $ the equivalence relation $ f(x) = f(y) $ on $ X $, and*
$$
X \xrightarrow{p} X/R \xrightarrow{h} f(X) \xrightarrow{i} Y
$$
*the canonical decomposition of $ f $.* *Then for $ f $ to be proper it is necessary and sufficient that $ p $ is proper, $ h $ a homeomorphism and $ f(X) $ a closed subset of $ Y $.*

The conditions are sufficient by virtue of Proposition 5 a) and Proposition 2. Conversely, if $ f $ is proper, then $ f $ is closed; hence $ f(X) $ is closed in $ Y $ and $ h $ is a homeomorphism ($ \S 5 $, no. 2, Proposition 3); also $ h \circ p $ is proper by Proposition 5 c); hence $ p = h^{-1} \circ (h \circ p) $ is proper by Proposition 5 a).

### 2. CHARACTERIZATION OF PROPER MAPPINGS BY COMPACTNESS PROPERTIES

In this subsection we shall denote by $ P $ a space consisting of a single point, with its unique topology.

#### Lemma 1 {#top-i-s10-lem-1 .statement}

*Let $ X $ be a topological space such that the constant mapping $ X \to P $ is proper. Then $ X $ is quasi-compact.*

(We shall see a little later on (Theorem 1, Corollary 1) that this property characterizes quasi-compact spaces.)

We may restrict ourselves to the case where $ X $ is not empty. Let $ \mathcal{F} $ be a filter on $ X $, and $ X' = X \cup \{ \omega \} $ the topological space associated with $ \mathcal{F} $ ($ \S 6 $, no. 5, Example). Let $ \Delta $ be the subset of $ X \times X' $ consisting of all $ (x, x) $ where $ x \in X $, and let $ F = \overline{\Delta} $ be the closure of $ \Delta $ in $ X \times X' $. In view of the hypothesis on $ X $, the image of $ F $ under the projection $ X \times X' \to X' $ is closed in $ X' $; this image contains $ X $ and therefore contains $ \omega $, which lies in the closure of $ X $; in other words, there is a point $ x \in X $ such that $ (x, \omega) \in F $. By the definition of the topology of $ X \times X' $, this means that, for each neighbourhood $ V $ of $ x $ in $ X $ and each $ M \in \mathcal{F} $, we have $ (V \times M) \cap \Delta \neq \emptyset $, i.e. $ V \cap M \neq \emptyset $, so that $ x $ is a cluster point of the filter $ \mathcal{F} $, and therefore $ X $ is quasi-compact.

Q.E.D.

#### Theorem 1 {#top-i-s10-thm-1 .statement}

*Let $ f : X \to Y $ be a continuous mapping. Then the following four statements are equivalent:

a) $ f $ is proper.
b) $ f $ is closed and $ \overline{f}^{-1}(y) $ is quasi-compact for each $ y \in Y $.
c) *If $ \mathcal{F} $ is a filter on $ X $ and if $ y \in Y $ is a cluster point of $ f(\mathcal{F}) $ then there is a cluster point $ x $ of $ \mathcal{F} $ such that $ f(x) = y $.*
d) *If $ \mathcal{U} $ is an ultrafilter on $ X $ and if $ y \in Y $ is a limit point of the ultrafilter base $ f(\mathcal{U}) $, then there is a limit point $ x $ of $ \mathcal{U} $ such that $ f(x) = y $.*

a) $ \Longrightarrow $ b): If $ f $ is proper then $ f $ is closed (no. 1, Proposition 1) and for each $ y \in Y $ the mapping $ f_{|y|} : \overline{f}^{-1}(y) \to \{ y \} $ is proper [no. 1, Proposition 3a)]. By Lemma 1, this implies that $ \overline{f}^{-1}(y) $ is quasi-compact.

b) $ \Longrightarrow $ c): Suppose $ \mathfrak{F} $ and $ y $ satisfy the hypotheses of c). Let $ \mathcal{B} $ be the filter base on $ X $ formed by the closures of the sets of $ \mathfrak{F} $. Since $ f $ is closed, we have $ f(\overline{M}) = f(M) $ for each $ M \in \mathfrak{F} $ (\S 5, no. 4, Proposition 9). This shows that the sets $ \overline{M} \cap \overline{f}^{-1}(y) $ are non-empty for all $ M \in \mathfrak{F} $, and hence form a filter base on $ \overline{f}^{-1}(y) $ whose elements are closed subsets of $ \overline{f}^{-1}(y) $. Since $ \overline{f}^{-1}(y) $ is quasi-compact, there is a point $ x \in \overline{f}^{-1}(y) $ which belongs to all the sets $ M $ as $ M $ runs through $ \mathfrak{F} $. Hence $ f(x) = y $ and $ x $ is a cluster point of $ \mathfrak{F} $.

c) $ \Longrightarrow $ d): Trivial.

d) $ \Longrightarrow $ a): We show first that if d) is satisfied, then $ f $ is a closed mapping. Let $ A $ be a non-empty closed subset of $ X $ and let $ \mathfrak{F} $ be the filter of subsets of $ X $ which contain $ A $. Then $ A $ is the set of cluster points of $ \mathfrak{F} $. Let $ B $ be the set of cluster points of the filter base $ f(\mathfrak{F}) $ on $ Y $; $ B $ is closed and clearly contains $ f(A) $; we shall show that $ B = f(A) $. Let $ y \in B $ and let $ \mathcal{B} $ be the neighbourhood filter of $ y $ in $ Y $; then by hypothesis every set of $ \mathfrak{W} = \overline{f}^{-1}(\mathcal{B}) $ meets every set of $ \mathfrak{F} $; hence $ \mathfrak{W} $ is a filter base on $ X $ and there is an ultrafilter $ U $ on $ X $ which is finer than both $ \mathfrak{F} $ and the filter whose base is $ \mathfrak{W} $ (\S 6, no. 2, Proposition 1, Corollary 1 and no. 4, Theorem 1). The ultrafilter whose base is $ f(U) $ is finer than $ \mathcal{B} $ and therefore converges to $ y $. By virtue of d) there is a point $ x \in X $ such that $ f(x) = y $ and $ U $ converges to $ x $; since $ U $ is finer than $ \mathfrak{F} $, $ x $ is a cluster point of $ \mathfrak{F} $; hence $ x \in A $. This shows that $ B = f(A) $ and therefore that $ f $ is closed.

To complete the proof we have to show that $ f \times \iota_Z $ is closed for every topological space $ Z $. From what has been proved it is enough to show that if $ f $ satisfies condition d), then so does $ f \times \iota_Z $. This is a consequence of the following general lemma:

#### Lemma 2 {#top-i-s10-lem-2 .statement}

*If* $ (f_i)_{i \in I} $ *is a family of continuous mappings* $ f_i : X_i \to Y_i $, *each of which satisfies condition d)* of Theorem 1, *then the product mapping*
$$
f : (x_i) \to (f_i(x_i))
$$
*also satisfies* d).

Let $ U $ be an ultrafilter on $ X = \prod_i X_i $, and let $ y = (y_i) $ be a point of $ Y = \prod_i Y_i $ such that $ f(U) $ converges to $ y $. This means that each of the ultrafilter bases $ \operatorname{pr}_i(f(U)) = f_i(\operatorname{pr}_i(U)) $ converges to $ y_i $ (\S 7, no. 6, Proposition 10, Corollary 1). By virtue of condition d), for each $ i \in I $ there exists $ x_i \in X_i $ such that $ f_i(x_i) = y_i $ and $ \operatorname{pr}_i(U) $ converges to $ x_i $; but then $ U $ converges to $ x = (x_i) $ (*loc. cit.*) and we have $ f(x) = y $. This completes the proof of Lemma 2 and hence of Theorem 1.

#### Corollary 1 {#top-i-s10-lem-2-cor-1 .statement}

*A topological space* $ X $ *is quasi-compact if and only if the mapping* $ X \to P $ *is proper*.

Apply a) $ \iff $ b) to $ X \to P $.

#### Corollary 2 {#top-i-s10-lem-2-cor-2 .statement}

*Every continuous mapping* $ f $ *of a quasi-compact space* $ X $ *into a Hausdorff space* $ Y $ *is proper*.

The composition $ X \xrightarrow{f} Y \to P $ is proper by Corollary 1; hence $ f $ is proper by no. 1, Proposition 5 d). Alternatively we may apply the criterion b) of Theorem 1, using § 9, no. 4, Theorem 2, Corollary 2.

#### Corollary 3 {#top-i-s10-lem-2-cor-3 .statement}

*If* $ (f_i) $ *is a family of proper mappings, then the product mapping* $ (x_i) \to (f_i(x_i)) $ *is proper*.

In view of Theorem 1, this is just Lemma 2 above.

If we apply this corollary to the family of mappings $ X_i \to P $ and use Corollary 1, we have Tychonoff’s theorem (§ 9, no 5, Theorem 3).

#### Corollary 4 {#top-i-s10-lem-2-cor-4 .statement}

*Let* $ X $ *be a Hausdorff space, and let* $ f_i : X \to Y_i $ *be a family of proper mappings. Then the mapping* $ f : x \to (f_i(x)) $ *of* $ X $ *into* $ \prod_i Y_i $ *is proper*.

The proof is the same as in the case of a finite family (no. 1, Proposition 5, Corollary 3), using Corollary 3 above and the fact that the diagonal of $ X^1 $ is closed (§ 8, no. 1, Proposition 1).

#### Corollary 5 {#top-i-s10-lem-2-cor-5 .statement}

*If* $ X $ *is any quasi-compact space and* $ Y $ *is any topological space, then the projection* $ \mathrm{pr}_2 : X \times Y \to Y $ *is proper*.

For we may identify $ Y $ with $ P \times Y $ and $ \mathrm{pr}_2 $ with the product of $ X \to P $ and $ \iota_Y $, both of which are proper mappings.

#### Example {#top-i-s10-n2-exa-1 .statement}

Let $ X $ be a set, and let $ f : X \to X' $ be a mapping of $ X $ onto a topological space $ X' $; topologize $ X $ with the inverse image under $ f $ of the topology of $ X' $. Then $ f $ is *proper*, for $ f $ is closed (§ 5, no. 1, Example 3) and the inverse image of a point of $ X' $ is a subspace of $ X $ whose topology is the coarsest topology and is therefore quasi-compact.

#### Remark {#top-i-s10-n2-rem-1 .statement}

When $ Y $ is *Hausdorff*, condition d) of Theorem 1 is equivalent to the following:

d') *If* $ \mathcal{U} $ *is an ultrafilter on* $ X $ *such that* $ f(\mathcal{U}) $ *is a convergent filter base, then* $ \mathcal{U} $ *is convergent*.

For if $ \mathcal{U} $ converges to $ x $ and $ f(\mathcal{U}) $ converges to $ y $, then the uniqueness of the limit in $ Y $ and the continuity of $ f $ show that we must have $ y = f(x) $. Likewise, Y being Hausdorff, condition c) of Theorem 1 is equivalent to:

c') *If $ \mathfrak{F} $ is a filter on X such that $ f(\mathfrak{F}) $ has a cluster point, then $ \mathfrak{F} $ has a cluster point.*

For c) $ \Longrightarrow $ c') $ \Longrightarrow $ d') $ \Longrightarrow $ d) $ \Longrightarrow $ c).

On the other hand, if Y is not Hausdorff, then d') no longer implies d); for example, take X to consist of one point and Y to consist of two points, with the coarsest topology.

#### Proposition 6 {#top-i-s10-prop-6 .statement}

*Let $ f : X \to Y $ be a proper mapping, and let K be a quasi-compact subset of Y. Then $ \overline{f}^{-1}(K) $ is quasi-compact.*

By Proposition 3 of no. 1, the mapping $ f_K : \overline{f}^{-1}(K) \to K $ is proper. Since $ K \to P $ is a proper mapping (Theorem 1, Corollary 1) it follows from no. 1, Proposition 5 a) that the composition $ \overline{f}^{-1}(K) \xrightarrow{f_K} K \to P $ is proper, whence $ \overline{f}^{-1}(K) $ is quasi-compact by Theorem 1, Corollary 1.

### 3. PROPER MAPPINGS INTO LOCALLY COMPACT SPACES

#### Proposition 7 {#top-i-s10-prop-7 .statement}

*Let f be a continuous mapping of a Hausdorff space X into a locally compact space Y. Then f is proper if and only if the inverse image under f of every compact subset of Y is compact. Further, if f is proper then X is locally compact.*

If f is proper and K is a compact subset of Y, then $ \overline{f}^{-1}(K) $ is compact by Proposition 6 of no. 2. Conversely, if this condition is satisfied, let $ (\mathbf{U}_\alpha) $ be a covering of Y by relatively compact open sets. Then the sets $ \overline{f}^{-1}(\overline{\mathbf{U}}_\alpha) $ are compact in X and their interiors cover X; since X is Hausdorff this shows that X is locally compact. Furthermore, each of the mappings $ f_{\overline{\mathbf{U}}_\alpha} : \overline{f}^{-1}(\alpha \overline{\mathbf{U}}) \to \overline{\mathbf{U}}_\alpha $ is proper (no. 2, Theorem 1, Corollary 2) and therefore f is proper by Proposition 3 b) of no. 1.

#### Corollary {#top-i-s10-n3-cor-1 .statement}

*Let X, X' be two locally compact spaces, and let Y (resp. Y') be the compact space obtained by adjoining a point at infinity $ \omega $ (resp. $ \omega' $) to X (resp. X') (\S 9, no. 8). Then a continuous mapping $ f : X \to X' $ is proper if and only if its extension $ \overline{f} : Y \to Y' $, such that $ \overline{f}(\omega) = \omega' $, is continuous.*

By Proposition 7, f is proper if and only if, for each compact subset K' of X', $ \overline{f}^{-1}(X' - K') = X - \overline{f}^{-1}(K') $ is the complement of a compact subset of X; by the definition of the neighbourhoods of $ \omega $ (resp. $ \omega' $) in Y (resp. Y') this is so if and only if $ \overline{f} $ is continuous at $ \omega $.

### 4. QUOTIENT SPACES OF COMPACT SPACES AND LOCALLY COMPACT SPACES

#### Proposition 8 {#top-i-s10-prop-8 .statement}

Let $ X $ be a compact space, $ R $ an equivalence relation on $ X $, $ C $ the graph of $ R $ in $ X \times X $, $ f $ the canonical mapping $ X \to X/R $. Then the following conditions are equivalent:

a) $ C $ is closed in $ X \times X $.

b) $ R $ is closed.

c) $ f $ is proper.

d) $ X/R $ is Hausdorff.

Furthermore, if these conditions are satisfied then $ X/R $ is compact.

$ R $ is closed if and only if $ f $ is closed; hence b) implies c) by reason of Theorem 1b) of no. 2. That c) implies d) is a particular case of no. 1, Proposition 5, Corollary 2. d) implies a) for any topological space $ X $ ($ \S $ 8, no. 3, Proposition 8). It remains to show that a) implies b). If $ F $ is a closed subset of $ X $ its saturation (with respect to $ R $) is $ \mathrm{pr}_2(C \cap (F \times X)) $; by hypothesis, $ C \cap (F \times X) $ is a closed subset of the compact space $ X \times X $, and is therefore compact ($ \S $ 9, no. 3, Proposition 3); the result now follows from the continuity of $ \mathrm{pr}_2 $ ($ \S $ 9, no. 4, Theorem 2, Corollary 2).

Finally it is clear that if $ X/R $ is Hausdorff then it is compact ($ \S $ 9, no. 4, Theorem 2).

#### Proposition 9 {#top-i-s10-prop-9 .statement}

Let $ X $ be a locally compact space, $ R $ an equivalence relation on $ X $, $ C $ the graph of $ R $ in $ X \times X $, $ f $ the canonical mapping $ X \to X/R $; let $ X' $ be the compact space obtained by adjoining a point at infinity $ \omega $ to $ X $, and let $ R' $ be the equivalence relation on $ X' $ whose graph is $ C' = C \cup \{(\omega, \omega)\} $. Then the following conditions are equivalent:

a) $ f $ is proper.

b) The saturation of each compact subset of $ X $ with respect to $ R $ is compact.

c) $ R' $ is closed.

d) The restriction of $ \mathrm{pr}_2 $ to $ C $ is proper.

e) $ R $ is closed and the equivalence classes with respect to $ R $ are compact.

Furthermore, if these conditions are satisfied, $ X/R $ is locally compact.

a) $ \Longrightarrow $ b): Since $ X/R = f(X) $ and $ f $ is proper, $ X/R $ is Hausdorff (no. 1, Proposition 5, Corollary 2); hence the image under $ f $ of every compact subset $ K $ of $ X $ is compact ($ \S $ 9, no. 4, Theorem 2, Corollary 1).

The saturation of $ K $ with respect to $ R $ is $ \overline{f}^{-1}(f(K)) $ and is therefore compact by no. 2, Proposition 6.

b) $ \Longrightarrow $ c) : If $ F' $ is closed in $ X' $ and does not contain $ \omega $, then $ F' $ is a compact subset of $ X $; hence its saturation with respect to $ R' $, which is the same as its saturation with respect to $ R $, is compact and *a fortiori* closed in $ X' $. If $ \omega \in F' $ and if $ F = F' \cap X = F' - \{ \omega \} $, then the saturation of $ F' $ with respect to $ R' $ is the union of $ \{ \omega \} $ and the saturation $ H $ of $ F $ with respect to $ R $; hence it is enough to show that $ H $ is *closed* in $ X $ (i.e. that $ R $ is a *closed* relation). For this, it is enough to show that if $ K $ is any compact subset of $ X $ then $ H \cap K $ is compact ($ \S 9 $, no. 7, Proposition 11). Now the saturation $ L $ of $ K $ with respect to $ R $ is compact by hypothesis, and $ H \cap L $ is the saturation of $ F \cap L $, which is also compact; *a fortiori* $ H \cap K = (H \cap L) \cap K $ is compact.

c) $ \Longrightarrow $ d) : Since $ X' $ is regular ($ \S 9 $, no. 2, Corollary to Proposition 1), $ C' $ is *closed* in $ X' \times X' $ ($ \S 8 $, no. 6, Proposition 14) and therefore compact. It follows that $ C' $ is the one-point compactification of $ C $ ($ \S 9 $, no. 8, Theorem 4). Since the restriction to $ C' $ of $ pr_2 : X' \times X' \to X' $ is continuous at $ \omega $, the result follows from no. 3, Corollary to Proposition 7.

d) $ \Longrightarrow $ e) : If $ F $ is any closed subset of $ X $, then $ C \cap (F \times X) $ is closed in $ C $, whence the saturation of $ F $ with respect to $ R $, which is equal to $ pr_2(C \cap (F \times X)) $, is closed in $ X $ (no. 1, Proposition 1). Also the equivalence class of $ x \in X $ mod $ R $ is homeomorphic to the inverse image of $ \{ x \} $ under the restriction of $ pr_2 $ to $ C $ and is therefore compact [no. 2, Theorem 1 b)].

e) $ \Longrightarrow $ a) : If $ R $ is closed, then by definition $ f $ is closed, and for each $ z \in X/R $, $ f^{-1}(z) $ is an equivalence class mod $ R $ and is therefore compact; hence $ f $ is proper by Theorem 1 b) of no. 2.

Finally we have to prove that $ X/R $ is locally compact. $ X'/R' $ is compact by c) and Proposition 8; the relation $ R $ is that induced on $ X $ by $ R' $; $ X $ is open in $ X' $ and is saturated with respect to $ R' $; hence $ X/R $ is homeomorphic to the image $ f'(X) $ of $ X $ under the canonical mapping $ f' : X' \to X'/R' $ ($ \S 3 $, no. 6, Proposition 10, Corollary 1). Now $ f'(X) $ is open in $ X'/R' $, and hence is a locally compact subspace of $ X'/R' $.

Q.E.D.

Corollary. *Let $ X $ be a Hausdorff space, $ Y $ a topological space, $ f : X \to Y $ a proper mapping. Then for $ X $ to be compact (resp. locally compact) it is necessary and sufficient that $ f(X) $ is compact (resp. locally compact), and it is sufficient that $ Y $ is compact (resp. locally compact).*

#### Remark {#top-i-s10-n4-rem-1 .statement}

If X is locally compact but not compact, then a closed equivalence relation R on X need not be Hausdorff (Chapter IX, § 4, Exercise 14); and even if R is Hausdorff, X/R need not be locally compact (Exercise 17). However, we have the following criterion:

#### Proposition 10 {#top-i-s10-prop-10 .statement}

Let X be a locally compact space, R an open Hausdorff equivalence relation on X, and let f : X \to X/R be the canonical mapping. Then X/R is locally compact, and if K' is any compact subset of X/R there is a compact subset K of X such that f(K) = K'.

The first assertion is a consequence of the facts that each x \in X has a compact neighbourhood V and that f(V) is a compact neighbourhood of f(x) (\S 5, no. 3, Proposition 5 and § 9, no. 4, Theorem 2, Corollary 1). For each y \in K' let V(y) be a compact neighbourhood of some point of f^{-1}(y) in X, so that f(V(y)) is a compact neighbourhood of y. There are a finite number of points y_i \in K' such that the f(V(y_i)) cover K'. Let K_1 be the compact set $ \bigcup_i V(y_i) $ in X; we have K' \subset f(K_1); hence K = K_1 \cap f^{-1}(K') is compact (because it is closed in K_1) and f(K) = K'.

### Exercises {#top-i-s10-exercises}

See the [exercises for § 10](exercises/s10/).
