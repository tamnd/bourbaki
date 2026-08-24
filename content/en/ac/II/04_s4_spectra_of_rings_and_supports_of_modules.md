---
book: ac
book_title: Commutative Algebra
chapter: II
chapter_title: LOCALIZATION
section: 4
section_title: Spectra of rings and supports of modules
lang: en
source: ac-i-vii
book_pages: 94-107, 140-146
pdf_pages: 0114-0127, 0160-0166
extraction: ocr
subsections:
    - "no": 1
      title: IRREDUCIBLE SPACES
      page: 94
      pdf_page: 114
    - "no": 2
      title: NOETHERIAN TOPOLOGICAL SPACES
      page: 97
      pdf_page: 117
    - "no": 3
      title: THE PRIME SPECTRUM OF A RING
      page: 98
      pdf_page: 118
    - "no": 4
      title: THE SUPPORT OF A MODULE
      page: 104
      pdf_page: 124
statements: 49
exercises: 28
content_sha256: 89a8077d0943105425d457afe72555ad4be848322acd21ae5c3646e85ddcc868
---

## 4. SPECTRA OF RINGS AND SUPPORTS OF MODULES

### 1. IRREDUCIBLE SPACES

#### Definition 1 {#ac-ii-s4-def-1 .statement}

A topological space $ X $ is called irreducible if every finite intersection of non-empty open sets of $ X $ is non-empty.

By considering the empty family of open sets of $ X $ it is seen that an irreducible space is non-empty; for a topological space $ X $ to be irreducible, it is necessary and sufficient that it be non-empty and that the intersection of two non-empty open sets of $ X $ be always non-empty (or, what amounts to the same thing, that the union of two closed sets distinct from $ X $ be always distinct from $ X $).

#### Proposition 1 {#ac-ii-s4-prop-1 .statement}

Let $ X $ be a non-empty topological space. The following conditions are equivalent:
(a) $ X $ is irreducible;
(b) every non-empty open set of $ X $ is dense in $ X $;
(c) every open set of $ X $ is connected.

By definition, a set which is dense in $ X $ is a set which meets every non-empty open set, hence (a) and (b) are equivalent. It is immediate that (c) implies (a), for if $ U_1 $ and $ U_2 $ are disjoint non-empty open sets, $ U_1 \cup U_2 $ is a disconnected open set. Finally let us show that (a) implies (c): if $ U $ is a disconnected open set, it is the union of two disjoint non-empty sets $ U', U'' $ which are open in $ U $ and hence also open in $ X $, which implies that $ X $ is not irreducible.

A Hausdorff space is irreducible only if it consists of a single point.

A subset $ E $ of a topological space $ X $ is called an irreducible set if the subspace $ E $ of $ X $ is irreducible. For this to be so, it is necessary and sufficient that, for every pair of sets $ U, V $ which are open in $ X $ and meet $ E $, $ U \cap V $ also meet $ E $, or (what amounts to the same thing) that, for every pair of sets $ F, G $ which are closed in $ X $ and satisfy $ E \subset F \cup G $, $ E \subset F $ or $ E \subset G $. By induction on $ n $, we deduce that, if $ (F_i)_{1 \leq i \leq n} $ is a finite family of closed sets of $ X $ such that $ E \subset \bigcup_{i=1}^n F_i $, there exists an index $ i $ such that $ E \subset F_i $.

#### Proposition 2 {#ac-ii-s4-prop-2 .statement}

In a topological space $ X $, for a set $ E $ to be irreducible, it is necessary and sufficient that its closure $ \overline{E} $ be so.

For an open set of $ X $ to meet $ E $, it is necessary and sufficient that it meet $ \overline{E} $; then the proposition follows from the above remarks.

#### Proposition 3 {#ac-ii-s4-prop-3 .statement}

(i) *If $ X $ is an irreducible space, every non-empty open subset of $ X $ is irreducible.*

(ii) *Let $ (U_\alpha)_{\alpha \in A} $ be a non-empty covering of a topological space $ X $ consisting of open sets such that $ U_\alpha \cap U_\beta = \emptyset $ for every pair of indices $ (\alpha, \beta) $. If the sets $ U_\alpha $ are irreducible, the space $ X $ is irreducible.*

(i) If $ X $ is irreducible, $ U \subset X $ non-empty and open in $ X $ and $ V \subset U $ non-empty and open in $ U $, $ V $ is also open in $ X $, therefore dense in $ X $ and *a fortiori* dense in $ U $. Then $ U $ is irreducible (Proposition 1).

(ii) Let us show that, for every non-empty open set $ V $ in $ X $, $ V \cap U_\alpha \neq \emptyset $ for all $ \alpha \in A $: it follows that $ V \cap U_\alpha $ is dense in $ U_\alpha $, by hypothesis, hence that $ V $ is dense in $ X $ and this proves that $ X $ is irreducible (Proposition 1). Now there exists at least one index $ y $ such that $ V \cap U_y \neq \emptyset $; as $ U_\alpha \cap U_y \neq \emptyset $ for all $ \alpha $ and $ V \cap U_y $ is dense in $ U_y $, $ U_y \cap V \neq \emptyset $ and *a fortiori* $ U_y \cap V \neq \emptyset $, which completes the proof of (ii).

#### Proposition 4 {#ac-ii-s4-prop-4 .statement}

*Let $ X $ and $ Y $ be two topological spaces and $ f $ a continuous mapping from $ X $ to $ Y $. For every irreducible subset $ E $ of $ X $, $ f(E) $ is an irreducible subset of $ Y $.*

If $ U, V $ are two open sets of $ Y $ which meet $ f(E) $, $ f^{-1}(U) $ and $ f^{-1}(V) $ are open sets of $ X $ which meet $ E $. Consequently, $ f^{-1}(U) \cap f^{-1}(V) = f^{-1}(U \cap V) $ meets $ E $, which implies that $ U \cap V $ meets $ f(E) $ and proves the proposition.

#### Definition 2 {#ac-ii-s4-def-2 .statement}

*Every maximal irreducible subset of a topological space $ X $ is called an irreducible component of $ X $.*

It follows from Proposition 2 that every irreducible component of $ X $ is *closed* in $ X $.

#### Proposition 5 {#ac-ii-s4-prop-5 .statement}

*Let $ X $ be a topological space. Every irreducible subset of $ X $ is contained in an irreducible component of $ X $ and $ X $ is the union of its irreducible components.*

To prove the first assertion, it is sufficient, by virtue of Zorn's Lemma, to prove that the set 3 of irreducible subsets of $ X $ is *inductive*. Let $ \mathcal{G} $ be a subset of $ \mathfrak{S} $ totally ordered by inclusion; we show that the union $ E $ of the sets $ F \in \mathcal{G} $ is irreducible. Let $ U, V $ be two open sets of $ X $ which meet $ E $; as $ \mathcal{G} $ is totally ordered, there exists a set $ F \in \mathcal{G} $ meeting $ U $ and $ V $; as $ F $ is irreducible, $ U \cap V $ meets $ F $ and hence also $ E $, which proves that $ E $ is irreducible and hence that 3 is inductive. The second assertion follows from the first, for every subset of $ X $ consisting of a single point is irreducible.

#### Corollary {#ac-ii-s4-n1-cor-1 .statement}

*Every connected component of a topological space $ X $ is a union of irreducible components of $ X $.*

Every irreducible subspace of $ X $ is connected by Proposition 1 and hence is contained in a connected component of $ X $.

Note that two distinct irreducible components of $ X $ may have points in common (Exercise 11).

#### Proposition 6 {#ac-ii-s4-prop-6 .statement}

*Let $ X $ be a topological space and $ (P_i)_{1 \leq i \leq n} $ ajinite covering of $ X $ consisting & irreducible closed sets. Then the irreducible components of $ X $ are the maximal elements (with respect to inclusion) of the set of $ P_i $.*

We may restrict ourselves to the case where no two $ P_i $ are comparable. If $ E $ is an irreducible subset of $ X $, then $ E \subset \bigcup_{i=1}^n P_i $, and hence $ E $ is contained in one of the closed sets $ P_i $; this proves that the $ P_i $ are the only maximal irreducible subsets of $ X $.

#### Corollary {#ac-ii-s4-n1-cor-2 .statement}

*Let $ X $ be a topological space and $ E $ a subspace with only ajinite number of distinct irreducible components $ Q_i $ ($ 1 \leq i \leq n $); then the irreducible components of the closure $ \overline{E} $ in $ X $ are the closures $ \overline{Q}_i $ of the $ Q_i $ ($ 1 \leq i \leq n $) and $ \overline{Q}_i \# \overline{Q}_j $ for $ i \neq j $.*

$ \overline{E} $ is the union of the $ \overline{Q}_i $, which are irreducible (Proposition 2); as $ Q_i $ is closed in $ E $, $ \overline{Q}_i \cap E = Q_i $; as $ Q_i \notin Q_j $ for $ i \neq j $, $ \overline{Q}_i \notin \overline{Q}_j $, whence the corollary by virtue of Proposition 6.

#### Remark {#ac-ii-s4-n1-rem-1 .statement}

Suppose that $ X $ has only ajinite number of distinct irreducible components $ X_i $ ($ 1 \leq i \leq n $); then $ U_+ = \mathbf{C}(\bigcup_{j \neq i} X_j) $ is open in $ X $ and dense in $ X_i $ since $ X_i \notin \bigcup_{j \neq i} X_j $; the $ U_i $ ($ 1 \leq i \leq n $) are therefore non-empty open sets of $ X $ which are irreducible (Proposition 2), pairwise disjoint and with their union dense in $ X $.

#### Proposition 7 {#ac-ii-s4-prop-7 .statement}

*Let $ U $ be an open subset of a topological space $ X $. The mapping $ V \mapsto \overline{V} $ (closure in $ X $) is a bijection of the set & irreducible subsets of $ U $ which are closed in $ U $ onto the set & irreducible subsets & $ X $ which are closed in $ X $ and meet $ U $; the inverse bijection is $ Z \mapsto Z \cap U $. In particular, this bijection maps the set & irreducible components & $ U $ onto the set & irreducible components & $ X $ which meet $ U $.*

If $ V $ is closed in $ U $ and irreducible, $ \overline{V} $ is irreducible (Proposition 2) and $ V = \overline{V} \cap U $. Conversely, if $ Z $ is irreducible and closed in $ X $ and meets $ U $, $ Z \cap U $ is a non-empty open subset of $ Z $, hence irreducible (Proposition 3) and dense in $ Z $ and, as $ Z $ is closed, $ Z = \overline{Z} \cap U $. This proves the proposition.

### 2. NOETHERIAN TOPOLOGICAL SPACES

#### Definition 3 {#ac-ii-s4-def-3 .statement}

A topological space $ X $ is called Noetherian if every non-empty set of closed subsets of $ X $, ordered by inclusion, has a minimal element.

It amounts to the same to say that every non-empty set of open subsets of $ X $, ordered by inclusion, has a maximal element, or that every decreasing (resp. increasing) sequence of closed (resp. open) sets is stationary (Set Theory, Chapter 111, § 6, no. 5, Proposition 6).

#### Proposition 8 {#ac-ii-s4-prop-8 .statement}

(i) Every subspace of a Noetherian space is Noetherian.
(ii) Let $ (A_i)_{i \in I} $ be a finite covering of a topological space $ X $. If the subspaces $ A_i $ of $ X $ are Noetherian, $ X $ is Noetherian.

(i) Let $ X $ be a Noetherian space, $ A $ a subspace of $ X $ and $ (F_i) $ a decreasing sequence of subsets of $ A $ which are closed in $ A $; then $ F_i = \overline{F_n} \cap A $ and the closures $ \overline{F_n} $ of the $ F_i $ in $ X $ form a decreasing sequence of closed subsets of $ X $. As this sequence is stationary, so is the sequence $ (F_i) $.

(ii) Let $ (G_n)_{n \geq 0} $ be a decreasing sequence of closed subsets of $ X $; by hypothesis, each of the sequences $ (G_n \cap A_i)_{n \geq 0} $ is stationary. As $ I $ is finite, there is an integer $ n_0 $ such that, for $ n \geq n_0 $, $ G_n \cap A_i = G_{n_0} \cap A_i $, for all $ i \in I $. But
$$
G_n = \bigcup_{i \in I} (G_n \cap A_i)
$$
and hence the sequence $ (G_n) $ is stationary and $ X $ is Noetherian.

#### Proposition 9 {#ac-ii-s4-prop-9 .statement}

For a topological space $ X $ to be Noetherian, it is necessary and sufficient that every open set in $ X $ be quasi-compact.

To show that the condition is necessary, it is sufficient, by virtue of Proposition 8, to prove that every Noetherian space $ X $ is quasi-compact. Let $ (U_i)_{i \in I} $ be an open covering of $ X $; the set of finite unions of sets $ U_i $ is non-empty and hence admits a maximal element $ V = \bigcup_{i \in H} U_i $, where $ H $ is a finite subset of $ I $. By definition, $ V \cup U_i = V $ for all $ i \in I $ and hence $ V = X $.

Conversely, suppose that every open set of $ X $ is quasi-compact and let $ (U_i) $ be an increasing sequence of open subsets of $ X $. The union $ V $ of the $ U_i $ is open and hence quasi-compact; as $ (U_i) $ is an open covering of $ V $, there is a finite subfamily of $(U_i)$ which is a covering of $V$ and hence $V = U_n$ for some index $n$, which proves that the sequence $(U_i)$ is stationary.

**Lemma 1 ("Principle of Noetherian induction").** *Let E be an ordered set every non-empty subset of which admits a minimal element. Let F be a subset of E with the following property : if $a \in E$ is such that the relation $x < a$ implies $x \in F$, then $a \in F$. Then $F = E$.*

Suppose $F \neq E$; then $CF$ would have a minimal element $b$. By definition, $x \in F$ for all $x < b$, which implies that $b \in F$, which is a contradiction.

#### Proposition 10 {#ac-ii-s4-prop-10 .statement}

*If X is a Noetherian space, the set of irreducible components of X (and a fortiori the set of connected components of X) is finite.*

It is sufficient to prove that X is a finite union of irreducible closed subsets (no. **1**, Proposition 6). Let us show that the principle of Noetherian induction can be applied taking E to be the set of closed subsets of X, ordered by inclusion, and F to be the set of finite unions of irreducible closed subsets. Let Y be a closed subset of X such that every closed subset $\neq Y$ of Y belongs to F. If Y is irreducible, then $Y \in F$ by definition; otherwise, Y is the union of two closed subsets $Y_1,\ Y_2$ which are distinct from Y. Then $Y_1 \in F$ and $Y_2 \in F$ by hypothesis, whence $Y \in F$ by definition of F.

In particular it follows that a *Hausdorff* Noetherian space is necessarily *finite*.

### 3. THE PRIME SPECTRUM OF A RING

Let A be a ring and X the set of prime ideals of A. For every subset M of A, we denote by $V(M)$ the set of prime ideals of A containing M; clearly, if $a$ is the ideal of A generated by M, $V(M) = V(a)$; if M consists of a single element f, we write $V(f)$ instead of $V(\{f\})$ and we have $V(f) = V(Af)$. The mapping $M \mapsto V(M)$ is *decreasing* with respect to inclusion in A and X. Moreover, the following formulae hold :

(1)
$$
V(0) = X, \quad V(1) = O;
$$

(2)
$$
V\left(\bigcup_{i \in I} M_i\right) = V\left(\sum_{i \in I} M_i\right) = \bigcap_{i \in I} V(M_i)
$$
for every family $(M_i)_{i \in I}$ of subsets of A;

(3)
$$
V(a \cap a') = V(aa') = V(a) \cup V(a')
$$
for every pair of ideals $a,\ a'$ in A. Formulae (1) and (2) are obvious; on the other hand, formula (3) means that, for a prime ideal $p$ of A to contain one of the ideals $ a $ or $ a' $, it is necessary and sufficient that it contain $ aa' $ or that it contain $ a \cap a' $; then it is a consequence of § 1, no. 1, Proposition 1. The second formula (1) has the following converse: if $ a $ is an ideal of $ A $ such that $ V(a) = \varnothing $, then $ a = A $, for there is no maximal ideal of $ A $ containing $ a $. Finally, if $ a $ is an ideal of $ A $ and $ r(a) $ is its *radical* ($ \S 2 $, no. 6, Definition 4), then

$$
V(a) = V(r(a))
$$

as follows from $ \S 2 $, no. 6, Corollary 1 to Proposition 13.

Formulae (1) to (3) show that the subsets $ V(M) $ of $ X $ satisfy the *closed set* axioms of a topology (*General Topology*, Chapter I, $ \S 1 $, no. 4).

#### Definition 4 {#ac-ii-s4-def-4 .statement}

*Let $ A $ be a ring. The set $ X $ of prime ideals of $ A $, with the topology whose closed sets are the sets $ V(M) $, where $ M $ runs through $ \mathfrak{P}(A) $, is called the prime spectrum of $ A $ and denoted by $ \mathrm{Spec}(A) $. The topology thus defined is called the spectral or Zariski topology on $ X $.*

Clearly the relation $ \mathrm{Spec}(A) = \varnothing $ is equivalent to $ A = \{0\} $.

Let $ X $ be the prime spectrum of a ring $ A $; for all $ f \in A $, let us denote by $ X_f $ the set of prime ideals of $ A $ *not containing* $ f $; then $ X_f = X - V(f) $ and $ X_f $ is therefore an *open* set. By (2), every closed subset of $ X $ is an intersection of closed sets of the form $ V(f) $ and hence the $ X $, form a *base* of the spectral topology on $ X $. Moreover, it follows immediately from the definitions that

$$
X_0 = O,\quad X_1 = X,
$$

and more generally $ X_{f^{-1}} = X $ for every invertible element $ f $ of $ A $;

$$
X_{g^{-1}} = X, nX, \quad \text{for all } f, g \text{ in } A.
$$

For every subset $ Y $ of $ X $, let us denote by $ \mathfrak{J}(Y) $ the intersection of the prime ideals of $ A $ which belong to $ Y $. Clearly $ \mathfrak{J}(Y) $ is an ideal of $ A $ and the mapping $ Y \mapsto \mathfrak{J}(Y) $ is *decreasing* with respect to inclusion in $ X $ and $ A $. Clearly the relations

$$
\mathfrak{J}(\varnothing) = A
$$
$$
\mathfrak{J}\left( \bigcup_{\lambda \in L} Y_\lambda \right) = \bigcap_{\lambda \in L} \mathfrak{J}(Y_\lambda)
$$

hold for every family $ (Y_\lambda)_{\lambda \in L} $ of subsets of $ X $. Moreover:

#### Proposition 11 {#ac-ii-s4-prop-11 .statement}

*Let $ A $ be a ring, $ a $ an ideal of $ A $ and $ Y $ a subset of $ X = \mathrm{Spec}(A) $.
(i) $ V(a) $ is closed in $ X $ and $ \mathfrak{J}(Y) $ is an ideal of $ A $ which is equal to its radical.
(ii) $ \mathfrak{J}(V(a)) $ *is the radical of* $ a $ *and* $ V(\mathfrak{J}(Y)) $ *is the closure of* $ Y $ *in* $ X $.*

(iii) The mappings 3 and V define decreasing bijections, one of which is the inverse of the other, between the set of closed subsets of X and the set of ideals of A which are equal to their radicals.

Assertion (i) and the first assertion of (ii) follow from the definitions and § 2, no. 6, Corollary 1 to Proposition 13. If a closed set V(M) (for some M ⊂ A) contains Y, then M ⊂ p for every prime ideal p ∈ Y, whence M ⊂ J(Y) and consequently V(M) ⊃ V(J(Y)); as Y ⊂ V(J(Y)), V(J(Y)) is the smallest closed set of X containing Y, which completes the proof of (ii). Finally, it follows from (ii) that, if a is a prime ideal equal to its radical, then J(V(a)) = a and that, if Y is closed in X, then V(J(Y)) = Y; this proves (iii).

It follows immediately from Proposition 11 that, if M is any subset of A and Y is any subset of X, then V(M) = V(J(V(M))) and J(Y) = J(V(J(Y))).

#### Corollary 1 {#ac-ii-s4-prop-11-cor-1 .statement}

For every family (Y_λ)_{λ ∈ L} of closed subsets of X, J(∩_{λ ∈ L} Y_λ) is the radical of the sum of the ideals J(Y_λ).

It follows from Proposition 11 (iii) that J(∩_{λ ∈ L} Y_λ) is the smallest ideal which is equal to its radical and contains all the J(Y_λ); this ideal then contains ∑_{λ ∈ L} J(Y_λ) and therefore also the radical of ∑_{λ ∈ L} J(Y_λ) (§ 2, no. 6, Corollary 2 to Proposition 13), whence the corollary.

#### Corollary 2 {#ac-ii-s4-prop-11-cor-2 .statement}

Let r(a) denote the radical of an ideal a of A; if a and b are two ideals of A, the relation V(a) ⊂ V(b) is equivalent to b ⊂ r(a) and r(b) ⊂ r(a).

It is immediate that the relations b ⊂ r(a) and r(b) ⊂ r(a) are equivalent and, as V(a) = V(r(a)), the corollary follows immediately from Proposition 11, (iii).

#### Corollary 3 {#ac-ii-s4-prop-11-cor-3 .statement}

Let (f_λ)_{λ ∈ L} be a family of elements of A. For an element g ∈ A to satisfy X_g ⊂ ∪_{λ ∈ L} X_{f_λ}, it is necessary and sufficient that there exist an integer n > 0 such that g^n belongs to the ideal generated by the f_λ.

The relation X_g ⊂ ∪_{λ ∈ L} X_{f_λ} is equivalent to V(g) ⊃ ∩_{λ ∈ L} V(f_λ) and it is sufficient to apply Corollary 2.

COROLLARY 4, For two elements f, g of A to satisfy X_f = X_g, it is necessary and sufficient that there exist two integers m > 0, n > 0 such that f^m ∈ Ag and g^n ∈ Af.

#### Corollary 5 {#ac-ii-s4-prop-11-cor-5 .statement}

For $ f \in A $ to satisfy $ X_f = \varnothing $, it is necessary and sufficient that $ f $ be nilpotent.

This follows immediately from Corollary 4.

#### Corollary 6 {#ac-ii-s4-prop-11-cor-6 .statement}

The closure of a set consisting of a point $ p \in X = \mathrm{Spec}(A) $ is the set $ V(p) $ of prime ideals containing $ p $. For the set $ \{p\} $ to be closed in $ X $ (or, as we shall also say by an abuse of language, for $ p $ to be a closedpoint of $ X $), it is necessary and sufficient that $ p $ be maximal.

#### Corollary 7 {#ac-ii-s4-prop-11-cor-7 .statement}

If $ A $ is a Noetherian ring, $ X = \mathrm{Spec}(A) $ is a Noetherian space.

#### Proposition 12 {#ac-ii-s4-prop-12 .statement}

For all $ f \in A $, the open set $ X_f $ in $ X = \mathrm{Spec}(A) $ is quasi-compact; in particular, the space $ X $ is quasi-compact.

As the $ X_g $ form a base of the topology, it is sufficient to prove that, if $ (g_\lambda)_{\lambda \in L} $ is a family of elements of $ A $ such that $ X_f \subset \bigcup_{\lambda \in L} X_{g_\lambda} $, then there exists a finite subfamily $ (g_{\lambda_i})_{i \in I} $ such that $ X_f = \bigcup_{i \in I} X_{g_{\lambda_i}} $. But the relation $ X_f = \bigcup_{\lambda \in L} X_{g_\lambda} $ means that there exists an integer $ n > 0 $ and a finite subfamily $ (g_{\lambda_i})_{i \in I} $ such that "f" belongs to the ideal generated by that subfamily (Corollary 3 to Proposition 11); whence the proposition.

#### Proposition 13 {#ac-ii-s4-prop-13 .statement}

Let $ A, A' $ be two rings, $ X = \mathrm{Spec}(A), X' = \mathrm{Spec}(A') $ and $ h $ a homomorphism from $ A $ to $ A' $; the mapping $ ^a h : p' \mapsto \overline{h}(p') $ from $ X' $ to $ X $ is continuous.

For $ M \subset A $, the set $ (^a h)^{-1}(V(M)) $ is the set of prime ideals $ p' $ of $ A' $ such that $ M \subset \overline{h}(p') $, which is equivalent to $ h(M) \subset p' $; this set is then equal to $ V(h(M)) $ and is therefore closed.

We call $ ^a h $ the mapping associated with the homomorphism $ h $.

#### Remark {#ac-ii-s4-n3-rem-1 .statement}

If $ h $ is surjective and $ a $ is its kernel, it follows from the definition of the spectral topology that $ ^a h $ is a homeomorphism of $ X' $ onto the closed subspace $ V(a) $ of $ X $; for a prime ideal $ p' $ of $ A' $ to contain an ideal $ b' $ of $ A' $, it is necessary and sufficient that $ \overline{h}(p') $ contain $ \overline{h}(b') $; we see first that $ ^a h $ is injective by taking $ b' $ to be prime; moreover, for every ideal $ b' $ of $ A' $, the image under $ ^a h $ of $ V(b') $ is $ V(\overline{h}(b')) $, whence our assertion, the ideals of the form $ \overline{h}(b') $ all being ideals of $ A $ which contain $ a $.

#### Corollary {#ac-ii-s4-n3-cor-1 .statement}

Let $ S $ be a multiplicative subset of $ A $, $ A' = S^{-1}A $ and $ h $ the canonical homomorphism $ i_A^S $; then $ ^a h $ is a homeomorphism of $ X' = \mathrm{Spec}(A') $ onto the subspace of $ X = \mathrm{Spec}(A) $ consisting of the prime ideals of $ A $ which do not meet $ S $.

#### Proposition 14 {#ac-ii-s4-prop-14 .statement}

*Let $ A $ be a ring. For a subset $ Y $ of $ X = \mathrm{Spec}(A) $ to be irreducible, it is necessary and sufficient that the ideal $ \mathfrak{J}(Y) $ be prime.*

Writing $ p = \mathfrak{J}(Y) $, we note that, for an element $ f \in A $, the relation $ f \in p $ is equivalent to $ Y \subset V(f) $. Suppose that $ Y $ is irreducible and let $ f, g $ be elements of $ A $ such that $ fg \in p $. Then
$$
Y \subset V(fg) = V(f) \cup V(g);
$$
as $ Y $ is irreducible and $ V(f) $ and $ V(g) $ are closed, $ Y \subset V(f) $ or $ Y \subset V(g) $, hence $ f \in p $ or $ g \in p $, which proves that $ p $ is prime.

Suppose now that $ p $ is prime; then $ \overline{Y} = V(p) $ (Proposition 11 (ii)) and, as $ p $ is prime, $ p = \mathfrak{J}(\{p\}) $, whence $ \overline{Y} = V(\mathfrak{J}(\{p\})) = \{p\} $ (Proposition 11 (ii)). As a set consisting of a single point is irreducible, $ Y $ is irreducible (no. 1, Proposition 2).

#### Corollary 1 {#ac-ii-s4-prop-14-cor-1 .statement}

*For a ring $ A $ to be such that $ X = \mathrm{Spec}(A) $ is irreducible, it is necessary and sufficient that the quotient of $ A $ by its nilradical $ \mathfrak{N} $ be an integral domain.*

By Proposition 11 (i), $ \mathfrak{J}(X) $ is the radical of the ideal $ (0) $, that is $ \mathfrak{N} $.

#### Corollary 2 {#ac-ii-s4-prop-14-cor-2 .statement}

*The mapping $ p \mapsto V(p) $ is a bijection of $ X = \mathrm{Spec}(A) $ onto the set of irreducible closed subsets of $ X $; in particular the irreducible components of a closed subset $ Y $ of $ X $ are the sets $ V(p) $, where $ p $ runs through the set of minimal elements of the set of prime ideals of $ A $ which contain $ \mathfrak{J}(Y) $.*

As $ \mathfrak{J}(V(p)) = p $ for every prime ideal $ p $ of $ A $ and $ Y = V(\mathfrak{J}(Y)) $ for every closed subset $ Y $ of $ X $, the first assertion follows from Proposition 14; on the other hand, for $ Y \supset V(p) $, it is necessary and sufficient that
$$
p = \mathfrak{J}(V(p)) \supset \mathfrak{J}(Y)
$$
(Proposition 11), whence the second assertion.

#### Corollary 3 {#ac-ii-s4-prop-14-cor-3 .statement}

*The set of minimal prime ideals of a Noetherian ring $ A $ is finite.*

$ X = \mathrm{Spec}(A) $ has only a finite number of irreducible components (Corollary 7 to Proposition 11 and no. 2, Proposition 10) and the corollary follows from Corollary 2 above.

#### Proposition 15 {#ac-ii-s4-prop-15 .statement}

Let $ A $ be a ring, $ I $ a finite set and $ E $ the set of orthogonal families $ (e_i)_{i \in I} $ of idempotents $ e_i \neq 0 $ of $ A $ such that $ \sum_{i \in I} e_i = 1 $. For all $ (e_i)_{i \in I} \in E $, we set $ \overline{\omega}((e_i)_{i \in I}) = (\mathrm{V}(A(1 - e_i)))_{i \in I} $, $ \sigma((e_i)_{i \in I}) = (Ae_i)_{i \in I} $. Then $ \overline{\omega} $ is a bijection of $ E $ onto the set $ P $ of partitions $ (U_i)_{i \in I} $ of $ X = \mathrm{Spec}(A) $ into open sets and $ \sigma $ is a bijection of $ E $ onto the set $ S $ of families $ (a_i)_{i \in I} $ of ideals $ \neq 0 $ of $ A $ such that $ A $ is the direct sum of the $ a_i $.

Let $ (e_i)_{i \in I} $ be an element of $ E $ and set $ Y_i = \mathrm{V}(A(1 - e_i)) $; if $ i \neq j $, then $ 1 = 1 - e_i + e_i(1 - e_j) \in A(1 - e_i) + A(1 - e_j) $, whence $ Y_i \cap Y_j = \varnothing $ (formulae (1) and (2)). On the other hand,

$$
\bigcup_{i \in I} Y_i = \mathrm{V}\left( \prod_{i \in I} A(1 - e_i) \right)
$$

(formula (3));

by hypothesis $ \prod_{i \in I} (1 - e_i) = 1 - \sum_{i \in I} e_i = 0 $, whence $ \bigcup_{i \in I} Y_i = X $ (formula (I)). As the $ Y_i $ are closed, they are also open, whence $ \overline{\omega}(E) \subset P $. Also, obviously $ A = \sum_{i \in I} Ae_i $; if $ 0 = \sum_{i \in I} a_i e_i $ where $ a_i \in A $, we obtain, by multiplying by $ e_i $, $ O = a_i e_i^2 = a_i e_i $ for all $ i $; this proves that $ \sigma(E) \subset S $.

#### Lemma 2 {#ac-ii-s4-lem-2 .statement}

*If* $ e, f $ *are two idempotents of* $ A $ *such that* $ Ae $ *and* $ Af $ *have the same radical* then $ e = f $.

There exists by hypothesis integers $ m \geq 0, n \geq 0 $ such that $ e = e^m \in Af $ and $ f = f^n \in Ae $; let $ x, y $ be elements of $ A $ such that $ e = xf, f = ye $; then $ ef = x^2 = x = e $ and similarly $ ef = ye^2 = ye = f $, whence $ e = f $.

Lemma 2 and Corollary 2 to Proposition 11 show that the mappings $ \overline{\omega} $ and $ \sigma $ are *injective*.

Let us show that $ \sigma $ is surjective. If $ (a_i)_{i \in I} $ is an element of $ S $, there are elements $ e_i \in a_i $ such that $ 1 = \sum_{i \in I} e_i $; if $ i \neq j $, then $ e_i e_j \in a_i \cap a_j = \{0\} $, whence

$$
e_i = \sum_{j \in I} e_i e_j = e_i^2;
$$

finally, $ Ae_i \subset a_i $, for all $ i \in I $ and $ \sum_{i \in I} Ae_i = A $, whence $ Ae_i = a_i $.

It remains to prove that $ \overline{\omega} $ is surjective. Let $ (U_i)_{i \in I} $ be an element of $ P $ and set $ Z_i = \bigcup_{j \neq i} U_j $; as $ U_i $ and $ Z_i $ are closed, there exist ideals $ a_i, b_i $ of $ A $ such that $ U_i = \mathrm{V}(a_i), Z_i = \mathrm{V}(b_i) $. We now show that it is possible to suppose further that $ a_i \cap b_i = 0 $. Now $ U_i \cap Z_i = \varnothing $, whence $ a_i + b_i = A $; let $ a_i, b_i \in a_i, b_i $ be such that $ a_i + b_i = 1 $. Then $ X = U_i \cup Z_i = \mathrm{V}(a_i b_i) $ (formula (3)); every element of $ a_i b_i $ is therefore nilpotent (Corollary 2 to Proposition 11); let $ p $ be an integer such that $ a_i^p b_i^p = 0 $. Then $ U_i \subset \mathrm{V}(Aa_i) = \mathrm{V}(Aa_i^p) $,

$$
Z_i \subset \mathrm{V}(Ab_i) = \mathrm{V}(Ab_i^p)
$$

and $ V(Aa_i) \cap V(Ab_i) = V(Aa_i + Ab_i) = \varnothing $, hence $ U_i = V(Aa_i^p) $ and $ Z_i = V(Ab_i^p) $, which establishes our assertion by replacing $ a_i $ by $ Aa_i^p $ and $ b_i $ by $ Ab_i^p $. The ideals $ a_i $ and $ b_i $ thus chosen, it follows from the fact that $ \sigma $ is bijective that there exist two idempotents $ f_i \in a_i, e_i \in b_i $ such that $ 1 = e_i + f_i, e_i f_i = 0, a_i = Af_i, b_i = Ae_i $. If $ i \neq j $, then $ X = Z, \cup Z_j = V(Ae_i e_j) $, and as $ e_i e_j $ is idempotent, Lemma 2 shows that $ e_i e_j = 0 $. Finally $ e = \sum_{i \in I} e_i $ is idempotent and $ e_i \in Ae $ for all $ i \in I $, whence $ V(Ae) \subset Z $, for all $ i $; it follows that

$$
V(Ae) = \varnothing = V(A.1)
$$

and Lemma 2 shows also that $ e = 1 $.

#### Corollary 1 {#ac-ii-s4-lem-2-cor-1 .statement}

Let $ A $ be a ring, $ r $ a nil ideal of $ A $ and $ h : A \to A/r $ the canonical homomorphism. For every finite orthogonal family $ (e'_i)_{i \in I} $ of idempotents of $ A/r $ such that $ \sum_{i \in I} e'_i = 1 $, there exists a finite orthogonal family $ (e_i)_{i \in I} $ of idempotents of $ A $ such that $ \sum_{i \in I} e_i = 1 $ and $ h(e_i) = e'_i $ for all $ i \in I $.

We write $ A' = A/r $. We know (Remark following Proposition 13) that

$$
ah : \operatorname{Spec}(A') \to \operatorname{Spec}(A)
$$

is a homeomorphism, every prime ideal of $ A $ containing $ r $ by hypothesis. Proposition 15 shows that there exists in $ A $ a finite orthogonal family $ (e_i)_{i \in I} $, of idempotents such that $ \sum_{i \in I} e_i = 1 $ and that the image under $ ah $ of $ V(A'(1 - e'_i)) $ is $ V(A(1 - e_i)) $. But clearly $ V(A(1 - e_i)) $ is also the image under $ ah $ of

$$
V(A'(1 - h(e'_i)));
$$

as $ 1 - e'_i $ and $ 1 - h(e_i) $ are idempotent, Lemma 2 shows that $ e'_i = h(e_i) $, whence the corollary.

#### Corollary 2 {#ac-ii-s4-lem-2-cor-2 .statement}

For the prime spectrum $ X = \operatorname{Spec}(A) $ of a ring $ A $ to be connected, it is necessary and sufficient that $ A $ contain no idempotents other than $ 0 $ and $ 1 $.

To say that $ X $ is not connected means that there exists in $ X $ a set which is open and closed and distinct from $ \varnothing $ and $ X $.

### 4. THE SUPPORT OF A MODULE

#### Definition 5 {#ac-ii-s4-def-5 .statement}

Let $ A $ be a ring and $ M $ an $ A $-module. The set of prime ideals $ p $ of $ A $ such that $ M_p \neq 0 $ is called the support of $ M $ and is denoted by $ \operatorname{Supp}(M) $.

As every maximal ideal of $ A $ is prime, it follows immediately from § 3, no. 3, Corollary 2 to Theorem 1, that for $ A $-module $ M $ to be equal to $ 0 $, it is necessary and sufficient that $ \operatorname{Supp}(M) = \varnothing $.

#### Example {#ac-ii-s4-n4-exa-1 .statement}

Let $ a $ be an ideal of $ A $; in the notation of no. 3, we have
$$
V(a) = \operatorname{Supp}(A/a).
$$
If $ p $ is a prime of $ A $ such that $ a \notin p $, then $ (A/a)_p = 0 $ (\S 3, no. 1, Remark 3); if on the other hand $ a \subset p $, $ aA_p $ is contained in the maximal ideal $ pA_p $ of $ A $, and $ (A/a)_p $ is isomorphic to $ A_p/aA_p $ and hence is non-zero (\S 3, no. 1, Proposition 3); whence our assertion.
In particular, $ \operatorname{Supp}(A) = \operatorname{Spec}(A) $.

#### Proposition 16 {#ac-ii-s4-prop-16 .statement}

Let $ A $ be a ring and $ M $ an $ A $-module.
(i) *If $ N $ is a submodule of $ M $, then*
$$
\operatorname{Supp}(M) = \operatorname{Supp}(N) \cup \operatorname{Supp}(M/N).
$$
(ii) *If $ M $ is the sum of a family $ (N_i)_{i \in I} $ of submodules, then*
$$
\operatorname{Supp}(M) = \bigcup_{i \in I} \operatorname{Supp}(N_i).
$$
(i) From the exact sequence $ 0 \to N \to M \to M/N \to 0 $, we derive, for every prime ideal $ p $ of $ A $, the exact sequence
$$
0 \to N_p \to M_p \to (M/N)_p \to 0
$$
(\S 2, no. 4, Theorem 1). For $ M $, to be reduced to 0, it is necessary and sufficient that $ N_p $ and $ (M/N)_p $ be so. In other words, the relation $ p \notin \operatorname{Supp}(M) $ is equivalent to "p $ \notin \operatorname{Supp}(N) $ and $ p \notin \operatorname{Supp}(M/N) $", which proves (i).
(ii) For every prime ideal $ p $ of $ A $, $ M $, is the sum of the family of submodules $ (N_i)_p $ (\S 2, no. 4). To say that $ M, \neq 0 $ means that there exists $ i \in I $ such that $ (N_i)_p \neq 0 $, whence (ii).

#### Corollary {#ac-ii-s4-n4-cor-1 .statement}

*Let $ A $ be a ring, $ M $ an $ A $-module, $ (m_i)_{i \in I} $ a system of generators of $ M $ and $ a $, the annihilator of $ m_i $. Then*
$$
\operatorname{Supp}(M) = \bigcup_{i \in I} V(a_i).
$$
$ \operatorname{Supp}(M) = \bigcup_{i \in I} \operatorname{Supp}(Am_i) $ by Proposition 16 (ii). On the other hand, $ Am_i $ is isomorphic to the $ A $-module $ A/a_i $ and we have seen that
$$
\operatorname{Supp}(A/a_i) = V(a_i)
$$
(Example above).

#### Proposition 17 {#ac-ii-s4-prop-17 .statement}

*Let $ A $ be a ring, $ M $ an $ A $-module and $ a $ its annihilator; if $ M $ is finitely generated, then* $ \operatorname{Supp}(M) = V(a) $ *and* $ \operatorname{Supp}(M) $ *is therefore closed in* $ \operatorname{Spec}(A) $.
Let $ (m_i)_{1 \leq i \leq n} $ be a system of generators of $ M $ and let $ a $, be the annihilator of $ m_i $; then $ a = \bigcap_{i=1}^n a_i $, hence $ V(a) = \bigcup_{i=1}^n V(a_i) $ (no. 3, equation (3)) and the Proposition follows from the Corollary to Proposition 16.

#### Corollary 1 {#ac-ii-s4-prop-17-cor-1 .statement}

Let $ A $ be a ring, $ M $ a finitely generated $ A $-module and $ a $ an element of $ A $. For $ a $ to belong to every prime ideal of the support of $ M $, it is necessary and sufficient that the homothety of $ M $ with ratio $ a $ be nilpotent.

It follows from Proposition 17 that the intersection of the prime ideals belonging to $ \operatorname{Supp}(M) $ is the radical of the annihilator $ a $ of $ M $ (no. 3, Proposition 11 (ii)). To say that $ a $ belongs to this radical is equivalent to saying that there exist a power $ a^k \in a $ and hence that $ a^k M = 0 $.

#### Corollary 2 {#ac-ii-s4-prop-17-cor-2 .statement}

Let $ A $ be a Noetherian ring, $ M $ a finitely generated $ A $-module and $ a $ an ideal of $ A $. For $ \operatorname{Supp}(M) \subset V(a) $, it is necessary and sufficient that there exist an integer $ k $ such that $ a^k M = 0 $.

If $ b $ is the annihilator of $ M $, the relation $ \operatorname{Supp}(M) \subset V(a) $ is equivalent to $ V(b) \subset V(a) $ by Proposition 17 and hence to $ a \subset r(b) $, where $ r(b) $ is the radical of $ b $ (no. 3, Corollary 2 to Proposition 11). Since $ A $ is Noetherian, this condition is also equivalent to the existence of an integer $ k > 0 $ such that $ a^k \subset b $ (\S 2, no. 6, Proposition 15).

#### Proposition 18 {#ac-ii-s4-prop-18 .statement}

Let $ M, M' $ be two finitely generated modules over a ring $ A $; then

$$
\operatorname{Supp}(M \otimes_A M') = \operatorname{Supp}(M) \cap \operatorname{Supp}(M').
$$

We need to prove that, if $ p $ is a prime ideal of $ A $, the relations $ (M \otimes_A M')_p \neq 0 $ and "$ M_p \neq 0 $ and $ M'_p \neq 0 $" are equivalent. As the $ A_p $-modules $ M, \otimes_{A_p} M'_p $ and $ (M \otimes_A M')_p $ are isomorphic (\S 2, no. 7, Proposition 18), our assertion follows from the following lemma:

#### Lemma 3 {#ac-ii-s4-lem-3 .statement}

Let $ B $ be a local ring and $ E $ and $ E' $ two finitely generated $ B $-modules. If $ E \neq 0 $ and $ E' \neq 0 $, then $ E \otimes_B E' \neq 0 $.

Let $ k $ be the residue field of $ B $. By virtue of \S 3, no. 2, Proposition 4, $ k \otimes_B E \neq 0 $ and $ k \otimes_B E' \neq 0 $; then we deduce that

$$
(k \otimes_B E) \otimes_k (k \otimes_B E') \neq 0
$$

(Algebra, Chapter II, \S 3, no. 7). But, since the tensor product is associative (loc. cit., \S 3, no. 8), this tensor product is isomorphic to

$$
E \otimes_B ((k \otimes_k k) \otimes_B E') = E \otimes_B (k \otimes_B E')
$$

and therefore to $ k \otimes_B (E \otimes_B E') $, whence the lemma.

#### Corollary {#ac-ii-s4-n4-cor-2 .statement}

Let $ M $ be a finitely generated $ A $-module and $ n $ its annihilator. For every ideal $ a $ of $ A $, $ \operatorname{Supp}(M/aM) = V(a) \cap V(n) = V(a + n) $.

$ M/aM = M \otimes_A (A/a) $ and $ A/a $ is finitely generated.

#### Proposition 19 {#ac-ii-s4-prop-19 .statement}

Let $ A, B $ be two rings, $ \phi : A \to B $ a homomorphism and
$$
^{a}\phi : \operatorname{Spec}(B) \to \operatorname{Spec}(A)
$$
the continuous mapping associated with $ \phi $ (Proposition 13). For every $ A $-module $ M $,
$$
\operatorname{Supp}(M_{(B)}) \subset ^{a}\phi(\operatorname{Supp}(M)) ; \text{if also } M \text{ is finitely generated, then}
$$
$$
\operatorname{Supp}(M_{(B)}) = ^{a}\phi^{-1}(\operatorname{Supp}(M)).
$$
Let $ q $ be a prime ideal of $ B $ and $ p = \phi^{-1}(q) $. Suppose that $ q $ belongs to $ \operatorname{Supp}(M_{(B)}) $; then $ M_{(B)} \otimes_B B_q = (M \otimes_A B) \otimes_B B_q = M \otimes_A B_q = (M \otimes_A A_p) \otimes_A B_q $, since the homomorphism $ A \to B \to B_q $ factors into $ A \to A_p \to B_q $ (\$2, no. 1, Proposition 2); the hypothesis $ M_{(B)} \otimes_B B_q \neq 0 $ implies therefore $ M \otimes_A A_q \neq 0 $, whence the first assertion. As the homomorphism $ \phi_q : A_p \to B_q $ is local, the second assertion follows from the following lemma:

#### Lemma 4 {#ac-ii-s4-lem-4 .statement}

Let $ A, B $ be two local rings, $ p : A \to B $ a local homomorphism and $ E $ a finitely generated $ A $-module. If $ E \neq 0 $, then $ E_{(B)} \neq 0 $.

Let $ m $ be the maximal ideal of $ A $ and $ k = A/m $ the residue field; the hypothesis implies that $ B \otimes_A k = B/mB \neq 0 $; since the tensor product is associative, $ (E \otimes_A B) \otimes_A k $ is isomorphic to $ E \otimes_A (B \otimes_A k) $, hence also to $ E \otimes_A (k \otimes_k (B \otimes_A k)) $ and finally to $ (E \otimes_A k) \otimes_k (B \otimes_A k) $; by § 3, no. 2, Proposition 4, $ E \otimes_A k \neq 0 $, hence $ (E \otimes_A B) \otimes_A k \neq 0 $ (Algebra, Chapter II, § 3, no. 7) and a fortiori $ E \otimes_A B \neq 0 $.

#### Proposition 20 {#ac-ii-s4-prop-20 .statement}

Let $ A $ be a ring and $ M $ a finitely generated $ A $-module. For every prime ideal $ p \in \operatorname{Supp}(M) $, there exists a non-zero $ A $-homomorphism $ w : M \to A/p $.

Let $ p \in \operatorname{Supp}(M) $. As $ M $ is finitely generated and $ M_p \neq 0 $,
$$
M_p/pM_p = M_p \otimes_A (A_p/pA_p) \neq 0
$$
(\$3, no. 2, Proposition 4). Let $ K = A_p/pA_p $ be the field of fractions of the integral domain $ A/p $; since $ M_p/pM_p $ is a vector space over $ K $, which is not reduced to 0, there exists a non-zero linear form $ u : M_p/pM_p \to K $. If $ (x_i)_1 <_n^* $ is a system of generators of $ M $, $ \bar{x}_i $ the image of $ x_i $, in the $ (A/p) $-module $ M_p/pM_p $, there exists an element $ \alpha \neq 0 $ of $ A/p $ such that the $ \alpha u(\bar{x}_i) $ belong to $ A/p $ for $ 1 \leq i \leq n $; hence $ v = \alpha u $ is a non-zero $ (A/p) $-linear mapping from $ M_p/pM_p $ to $ A/p $. The composition
$$
w : M \longrightarrow M, \longrightarrow M_p/pM_p \overset{v}{\longrightarrow} A/p
$$
is therefore the required homomorphism.

### Exercises {#ac-ii-s4-exercises}

(b) Let $ n = \dim(M) $. The direct factors of M of dimension 1 (resp. $ n - 1 $) are called *lines* (resp. hyperplanes). An automorphism $ u \in \mathbf{GL}(M) $ distinct from the identity is called a *transvection* if there exists a hyperplane H of M all of whose elements are invariant under $ u $; then $ u(x) = x + a\phi(x) $, where $ \phi $ is a linear form on M such that $ H = \mathrm{Ker}(\phi) $ and $ a \in H $; obtain the converse. If A is commutative, show that every automorphism $ u \in \mathbf{GL}(M) $ of determinant 1 is a product of transvections (observe that, in the matrix of $ u $ with respect to any basis of M, every column contains at least one invertible element of A and a matrix of the form $ I + E_{ij} \ (i \neq j) $ is the matrix of a transvection).

(c) Give an example of an automorphism $ u \in \mathbf{GL}(M) $ such that the kernel of $ 1 - u $ is not a direct factor of M (take A to be the local ring $ K[[X]] $ of formal power series in one indeterminate over a field K and $ M = A $).

(d) Give an example of direct factors N, P of M (necessarily free) such that $ N + P $ and $ N \cap P $ are not direct factors of M. (Take $ A = K[X]/(X^2) $, where K is a field and $ M = A^2 $.)

¶ 15. Let A be a (commutative) ring and M an A-module.

(a) For a submodule M' of M to be pure (Chapter I, § 2, Exercise 24), it is necessary and sufficient that, for every maximal ideal $ m $ of A, $ M'_m $ be a pure sub-&-module of $ M_m $ (use Theorem 1 of no. 3).

(b) Suppose that A is a local ring with maximal ideal $ m $ and M a finitely generated free A-module. For a finitely generated submodule M' of M to be pure, it is necessary and sufficient that it be a direct factor of M. (Using Corollary 1 to Proposition 5 of no. 2, reduce it to proving that, if $ M' \subset mM $, $ M' $ can only be a pure submodule of M if $ M' = 0 $.)

16. Let $ (A_\lambda, f_{\mu\lambda}) $ be a direct system of local rings, such that the $ f_{\mu\lambda} $ are local homomorphisms; let $ m_\lambda $ be the maximal ideal of $ A_\lambda $ and $ K_\lambda = A_\lambda/m_\lambda $. Then $ A = \varprojlim A_\lambda $ is a local ring whose maximal ideal is $ m = \varprojlim m_\lambda $ and residue field is $ \bar{K} = \varprojlim K_\lambda $. Moreover, if $ m_\mu = A_\mu m_\lambda $ for $ \lambda < \mu $, then $ m = Am $, for all $ \lambda $.

94

See the [exercises for § 4](exercises/s4/).
