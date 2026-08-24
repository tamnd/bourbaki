---
book: int
book_title: Integration
chapter: IX
chapter_title: MEASURES ON HAUSDORFF TOPOLOGICAL SPACES
section: 3
section_title: Measures and additive set functions
lang: en
source: int-vii-ix
book_pages: INT IX.41-INT IX.49, INT IX.108-INT IX.112
pdf_pages: 0223-0231, 0290-0294
extraction: ocr
subsections:
    - "no": 1
      title: Measures and additive set functions of compact sets
      page: 41
      pdf_page: 223
    - "no": 2
      title: Inner regular set functions
      page: 44
      pdf_page: 226
    - "no": 3
      title: Radon spaces
      page: 46
      pdf_page: 228
statements: 16
exercises: 18
content_sha256: 154c3b35da5d10fc4c76d66d0ad120ae0866649bb9aeba5c68df370ca9d0a1c6
---

## § 3. MEASURES AND ADDITIVE SET FUNCTIONS

In this section, we shall denote by $ \mathcal{K}(T) $ and $ \mathcal{B}(T) $, respectively, the set of compact subsets of a Hausdorff topological space T and the Borel tribe of T.

### 1. Measures and additive set functions of compact sets

#### Theorem 1 {#int-ix-s3-thm-1 .statement}

— Let T be a topological space, and I a mapping of $ \mathcal{K}(T) $ into $ \mathbf{R}_+ $. In order that there exist a measure $ \mu $ on T such that $ I(K) = \mu^\bullet(K) $ for all $ K \in \mathcal{K}(T) $, it is necessary and sufficient that I satisfy the following conditions:

1) If K and L are compact subsets of T such that $ K \subset L $, then $ I(K) \leq I(L) $ ('I is increasing').

2) If K and L are compact subsets of T, then $ I(K \cup L) \leq I(K) + I(L) $.

3) If K and L are disjoint compact subsets of T, then $ I(K \cup L) = I(K) + I(L) $ ('I is additive').

4) For every decreasing directed family $ (K_\alpha)_{\alpha \in A} $ of compact subsets of T, one has $ I(\bigcap_{\alpha \in A} K_\alpha) = \inf_{\alpha \in A} I(K_\alpha) $.

5) For every $ x \in T $, there exists a neighborhood V of x such that
$$
\sup_{\substack{K \in \mathcal{K}(T) \\ K \subset V}} I(K) < +\infty
$$
('I is locally bounded').

The measure $ \mu $ is then unique.

The uniqueness of $ \mu $ follows from the Cor. of Prop. 2 of \S 1, No. 2. The above conditions are necessary, the first three in obvious fashion, the last from the fact that $ \mu^\bullet $ is a locally bounded encumbrance, and condition 4) by the Cor. of Prop. 5 of \S 1, No. 6.

To show that these conditions are sufficient, we begin by treating the case that T is compact.

#### Lemma 1 {#int-ix-s3-lem-1 .statement}

Assume that T is compact, and set l = I(T). For every $ A \subset T $, set

$$
J(A) = \sup_{\substack{K \in \mathcal{K}(T) \\ K \subset A}} I(K)
$$

and let $ \Phi $ be the set of $ A \subset T $ such that $ J(A) + J(\mathbf{C}A) = l $. The set $ \Phi $ is then a clan that contains $ \mathcal{K}(T) $, and the function $ J $ on $ \Phi $ is increasing and additive.

It is clear that $ J $ is an increasing set function, extending $ I $, and that $ J(A) + J(\mathbf{C}A) \leq l $ for every $ A \subset T $.

Let $ K $ and $ S $ be two compact sets in $ T $; we are first going to show that

$$
J(K \cap S) + J(\mathbf{C}K \cap S) = J(S).
$$

On considering the restrictions of $ I $ to $ \mathcal{K}(S) $ and of $ J $ to $ \mathfrak{P}(S) $, one reduces immediately to the case that $ S = T $. Since $ T $ is normal, $ K $ is the intersection of the decreasing directed family of its compact neighborhoods, and condition 4) implies the existence, for every $ \varepsilon > 0 $, of a compact neighborhood $ H $ of $ K $ such that $ I(H) \leq I(K) + \varepsilon $. Let $ L $ be the closure of $ T - H $; $ L $ is compact, $ L \cap K = \varnothing $ and $ H \cup L = T $, therefore $ l = I(H \cup L) \leq I(H) + I(L) \leq I(K) + I(L) + \varepsilon $ (condition 2)), whence the relation $ J(K) + J(\mathbf{C}K) \geq I(K) + I(L) \geq l - \varepsilon $. Since $ \varepsilon $ is arbitrary, $ J(K) + J(\mathbf{C}K) = l $. This proves the formula (2), as well as the inclusion $ \mathcal{K}(T) \subset \Phi $.

Let us now prove that $ \Phi $ is a clan. Since $ \Phi $ is obviously stable under passage to the complement, it suffices to show that if $ A_1 $ and $ A_2 $ denote elements of $ \Phi $, then $ A_1 \cup A_2 \in \Phi $, or again that

$$
J(A_1 \cup A_2) + J(\mathbf{C}(A_1 \cup A_2)) \geq l.
$$

Denote by $ \varepsilon $ a number $ > 0 $, and, for $ i = 1, 2 $, let $ K_i $ be a compact set contained in $ A_i $, and $ L_i $ a compact set contained in $ \mathbf{C}A_i $, such that

$$
I(K_i) \geq J(A_i) - \varepsilon, \quad I(L_i) \geq J(\mathbf{C}A_i) - \varepsilon.
$$

Set $ M_1 = K_1 \cup L_1 $; the relations $ l = J(M_1) + J(\mathbf{C}M_1) $ and

$$
J(M_1) = I(K_1) + I(L_1) \geq J(A_1) + J(\mathbf{C}A_1) - 2\varepsilon = l - 2\varepsilon
$$

imply that $ J(\mathbf{C}M_1) \leq 2\varepsilon $. Then if $ S $ is a compact subset of $ T $, the relation (2) (applied to $ K = M_1 $) implies $ J(S) \leq J(M_1 \cap S) + 2\varepsilon $, whence

$$
J(S) \leq J(K_1 \cap S) + J(L_1 \cap S) + 2\varepsilon.
$$

Let us add the inequalities obtained by making $ S = K_2 $ and $ S = L_2 $, and take into account the inequality $ J(K_2) + J(L_2) \geq l - 2\varepsilon $ and the fact that $ K_1 \cap K_2 $, $ L_1 \cap K_2 $ and $ K_1 \cap L_2 $ are three disjoint compact sets contained in $ A_1 \cup A_2 $. Denoting by $ C $ the union of these three compact sets, it follows that

$$
l - 2\varepsilon \leq J(K_2) + J(L_2) \leq J(C) + J(L_1 \cap L_2) + 4\varepsilon \\
\leq J(A_1 \cup A_2) + J(\mathcal{C}(A_1 \cup A_2)) + 4\varepsilon,
$$

whence immediately the desired formula (3), in view of the arbitrariness of $ \varepsilon $. This having been established, the preceding inequalities imply that $ J(C) \geq J(A_1 \cup A_2) - 6\varepsilon $; if $ A_1 $ and $ A_2 $ are disjoint, then $ C $ is the union of $ K_1 \cap L_2 \subset A_1 $ and $ K_2 \cap L_1 \subset A_2 $, from which one deduces that $ J(A_1 \cup A_2) \leq J(A_1) + J(A_2) $. The reverse inequality being obvious, $ J $ is indeed additive on $ \Phi $, and the lemma is established.

Let us complete the proof of the theorem for the case that $ T $ is compact. Let $ \mathcal{E}(\Phi) $ be the vector space of $ \Phi $-step functions on $ T $, equipped with the topology of uniform convergence (Ch. IV, §4, No. 9, Def. 4); we shall again denote by $ J $ the positive linear form on $ \mathcal{E}(\Phi) $ associated with the additive function $ J $ (loc. cit., Prop. 18). Since $ J(T) = l $, $ J $ is continuous and has norm $ l $. Let then $ \mathcal{H} $ be the closure of $ \mathcal{E}(\Phi) $ for the topology of uniform convergence; one verifies at once that $ J $ may be extended by continuity to a *positive* linear form on $ \mathcal{H} $, again denoted $ J $. Since $ \mathcal{H} $ contains $ \mathcal{C}(T) $ (loc. cit., No. 10, Prop. 19) the restriction of $ J $ to $ \mathcal{C}(T) $ is a positive measure $ \mu $. It remains to show that $ \mu^\bullet(K) = I(K) $ for every compact subset $ K $ of $ T $. Now, we have $ \mu^\bullet(K) = \inf_{f \in S_K} \mu^\bullet(f) $, where $ S_K $ denotes the set of elements of $ \mathcal{C}(T) $ that are $ \geq \varphi_K $ (\S1, No. 6, Prop. 5). Since $ J(f) = \mu^\bullet(f) $ for $ f \in \mathcal{C}(T) $, it clearly suffices to show that $ J(K) \geq \inf_{f \in S_K} J(f) $. As in the proof of Lemma 1, let $ H $ be a compact neighborhood of $ K $ such that $ J(H) \leq J(K) + \varepsilon $, and let $ f $ be a continuous function on $ T $, between 0 and 1, equal to 1 on $ K $ and to 0 outside $ H $ (GT, IX, §4, No. 1, Prop. 1). Then

$$
J(f) \leq J(H) \leq J(K) + \varepsilon;
$$

$ \varepsilon $ being arbitrary, the desired inequality is proved, and the theorem is thus established when $ T $ is compact.

Let us now pass to the general case. For every compact set $ L $ in $ T $, let $ I_L $ be the restriction of $ I $ to $ \mathfrak{K}(L) $. By the special case just treated, there exists a measure $ \mu_L $ on $ L $, unique, such that $ \mu_L(K) = I_L(K) $ for every compact set $ K \subset L $. Let then $ L' $ be a compact set contained in $ L $; we have $ (\mu_L)_{L'}^\bullet(K) = \mu_{L'}^\bullet(K) = \mu_{L'}^\bullet(K) $ for every compact set $ K \subset L' $, therefore $ \mu_{L'} = (\mu_L)_{L'} $; the mapping $ \mu : L \mapsto \mu_L $ is a premeasure. The condition 5) expresses that $ \mu $ is a measure, and the relation $ I(K) = \mu^*(K) $ for all compact $ K \subset T $ is obvious.

#### Remark 1 {#int-ix-s3-n1-rem-1 .statement}

The condition 4) may be replaced, in the statement of Theorem 1, by the following condition ('right-continuity'):
$ 4') $ For every $ K \in \mathcal{K}(T) $ and every $ \varepsilon > 0 $, there exists an open set $ U $ containing $ K $, such that $ I(H) \leq I(K) + \varepsilon $ for every compact set $ H \subset U $.
For, if $ \mu $ is a measure, the function $ I : K \mapsto \mu^*(K) $ satisfies $ 4' $ (\S 1, No. 9, Prop. 13). Conversely, suppose that $ I $ satisfies 1) and $ 4' $; let us show that $ I $ then satisfies 4). With notations as in the statement of Theorem 1, choose an $ \varepsilon > 0 $ and an open set $ U $ containing the compact set $ K = \bigcap_{\alpha \in A} K_\alpha $ and such that $ 4' $) is satisfied. There then exists an index $ \beta \in A $ such that $ K_\beta \subset U $, and this implies
$$
\inf_{\alpha \in A} I(K_\alpha) \leq I(K_\beta) \leq I(K) + \varepsilon
$$
and 4) is indeed verified.
2) The set of conditions 2) and 3) may be replaced, in the statement of Theorem 1, by the following condition:
If $ K $ and $ L $ are compact subsets of $ T $, then
$$
I(K \cup L) + I(K \cap L) = I(K) + I(L).
$$
Indeed, this condition implies 2) and 3), and on the other hand
$$
\mu^*(K \cup L) = \mu^*(K \cap L) = \mu^*(K) + \mu^*(L)
$$
for every measure $ \mu $, by virtue of the relation $ \varphi_{K \cup L} + \varphi_{K \cap L} = \varphi_K + \varphi_L $ between the characteristic functions.

### 2. Inner regular set functions

#### Definition 1 {#int-ix-s3-def-1 .statement}

Let $ T $ be a topological space, and let $ \mathcal{B}(T) $ be the Borel tribe of $ T $; let $ I $ be a mapping of $ \mathcal{B}(T) $ into $ \overline{\mathbf{R}}_+ $.
a) $ I $ is said to be countably additive if, for every sequence $ (A_n) $ of pairwise disjoint elements of $ \mathcal{B}(T) $,
$$
I\left( \bigcup_n A_n \right) = \sum_n I(A_n).
$$
b) $ I $ is said to be inner regular if, for every set $ A \in \mathcal{B}(T) $,
$$
I(A) = \sup_K I(K),
$$
where $ K $ runs over the set of compact subsets of $ A $.

c) I is said to be bounded (resp. locally bounded) if $ I(T) < +\infty $ (resp. if every point $ x \in T $ admits an open neighborhood $ V $ such that $ I(V) < +\infty $).

#### Remark 1 {#int-ix-s3-n2-rem-1 .statement}

The condition a) clearly implies that I is an increasing mapping of $ \mathcal{B}(T) $ (ordered by inclusion) into $ \overline{\mathbf{R}}_+ $.

#### Remark 2 {#int-ix-s3-n2-rem-2 .statement}

Suppose that I is countably additive; let $ (A_n)_{n \in \mathbf{N}} $ be an increasing sequence of Borel sets, and let $ A = \bigcup_{n \in \mathbf{N}} A_n $. The sets $ D_0 = A_0 $, $ D_n = A_n - A_{n-1} $ being pairwise disjoint, and their union being A, we have $ I(A) = \sum_n I(D_n) = \lim_{n \to \infty} I(A_n) $. Similarly, if $ (B_n) $ is a decreasing sequence of Borel sets, and if $ I(B_0) < +\infty $, then $ I(\bigcap_n B_n) = \lim_{n \to \infty} I(B_n) $: it suffices to apply the preceding to the sets $ A_n = B_0 - B_n $.

#### Remark 3 {#int-ix-s3-n2-rem-3 .statement}

Let $ (A_n) $ be any sequence of Borel sets of T. If I is countably additive, then $ I(\bigcup_n A_n) \leq \sum_n I(A_n) $. By the preceding remark, it suffices to establish this inequality for a finite sequence. One immediately reduces to the case of two sets $ A_1 $ and $ A_2 $; but the relation (4) implies that

$$
I(A_1 \cup A_2) = I(A_1) + I(A_2 - (A_1 \cap A_2)) \leq I(A_1) + I(A_2).
$$

The desired inequality then follows immediately.

#### Remark 4 {#int-ix-s3-n2-rem-4 .statement}

If I is a countably additive and locally bounded function, the preceding remark implies at once that $ I(K) < +\infty $ for every compact set $ K \subset T $.

#### Remark 5 {#int-ix-s3-n2-rem-5 .statement}

One can show that if I is additive, that is, satisfies (4) for finite sequences, and if I is inner regular, then I is countably additive (Exer. 7). The reader can also ascertain that only additivity and inner regularity are used in the proof of Th. 2 below.

#### Theorem 2 {#int-ix-s3-thm-2 .statement}

— Let T be a topological space, and let I be a function defined on $ \mathcal{B}(T) $, with values in $ \overline{\mathbf{R}}_+ $. In order that there exist a measure $ \mu $ on T such that $ \mu^*(A) = I(A) $ for every $ A \in \mathcal{B}(T) $, it is necessary and sufficient that I be countably additive, locally bounded and inner regular. The measure $ \mu $ is then unique.

These three conditions are necessary: for, the mapping $ A \mapsto \mu^*(A) $ on $ \mathcal{B}(T) $ is countably additive (\S 1, No. 5, Cor. of Prop. 4), locally bounded by the definition of measures (\S 1, No. 2, Def. 5), and inner regular by Remark 3 of \S 1, No. 2.

We pass to existence. It is clear that the restriction of I to $ \mathcal{K}(T) $ satisfies conditions 1), 2), 3) and 5) of the statement of Th. 1; let us show that 4) is satisfied as well. Let K be a compact subset of T, the intersection of a decreasing directed family $ (K_\alpha)_{\alpha \in A} $ of compact sets, and let $ \varepsilon $ be a number $ > 0 $; I being locally bounded, there exists an open (hence Borel) neighborhood V of K such that $ I(V) < +\infty $, and then there exists an index $ \alpha $ such that $ K_\alpha \subset V $; changing notation if necessary, we can suppose that $ K_\alpha \subset V $ for all $ \alpha \in A $. By the inner regularity of I, there exists a compact set $ L \subset V - K $ such that $ I(L) \geq I(V - K) - \varepsilon $; since L does not intersect K, there exists an index $ \alpha $ such that $ L \cap K_\alpha = \varnothing $, and one then has $ I(V - K_\alpha) \geq I(L) \geq I(V - K) - \varepsilon $. Since $ K_\alpha \subset V $, it follows that $ I(K_\alpha) \leq I(K) + \varepsilon $ and the condition 4) is verified.

By Th. 1, there exists a measure $ \mu $ such that $ \mu^\bullet(K) = I(K) $ for all $ K \in \mathcal{K}(T) $. The inner regularity of the set functions $ \mu^\bullet $ and $ I $ on $ \mathcal{B}(T) $ then implies that $ \mu^\bullet(A) = I(A) $ for all $ A \in \mathcal{B}(T) $, and existence is proved. The uniqueness of $ \mu $ follows from the uniqueness assertion of Th. 1.

### 3. Radon spaces

#### Definition 2 {#int-ix-s3-def-2 .statement}

*Let T be a topological space. One says that T is a Radon (resp. strongly Radon) space if T is Hausdorff and if every function defined on the Borel tribe $ \mathcal{B}(T) $ of T, with values in $ \overline{\mathbf{R}}_+ $, that is countably additive and bounded (resp. locally bounded) is inner regular.*

For example, we shall see later on (Prop. 3) that every Polish space is strongly Radon. In particular, every locally compact space with a countable base is strongly Radon.

There exist Radon spaces that are not strongly Radon.

#### Proposition 1 {#int-ix-s3-prop-1 .statement}

*Every Lindelöf*$ ^{(1)} $* Radon space is strongly Radon.*

Let T be a Lindelöf space that is Radon, and let I be a set function on the tribe $ \mathcal{B}(T) $ that is positive, countably additive and locally bounded. The open sets V such that $ I(V) < +\infty $ form a covering of T, from which one can extract a countable covering $ (V_n)_{n \in \mathbf{N}} $. Set $ G_n = V_0 \cup V_1 \cup \cdots \cup V_n $ for every $ n \in \mathbf{N} $; set $ H_0 = G_0 $ and $ H_n = G_n - G_{n-1} $ for $ n \geq 1 $; finally, denote by $ I_n $ the set function $ A \mapsto I(A \cap H_n) $ on $ \mathcal{B}(T) $, which is obviously countably additive and bounded. Since the sets $ H_n $ form a partition of T, we have $ I = \sum_n I_n $. The space T being Radon, for every $ n \in \mathbf{N} $ there exists a bounded measure $ \mu_n $ on T such that $ \mu_n^\bullet(A) = I_n(A) $ for all $ A \in \mathcal{B}(T) $; therefore also $ \sum_n \mu_n^\bullet(A) = I(A) $. Since I is locally bounded, the family $ (\mu_n) $ is summable (\S 1, No. 7, Prop. 7); if $ \mu $ denotes $ \sum_n \mu_n $, we have $ \mu^\bullet(A) = I(A) $ for all $ A \in \mathcal{B}(T) $, and it follows that I is inner regular. In other words, T is strongly Radon.

Recall that a subset A of a topological space T is said to be *universally measurable* if A is $ \mu $-measurable for every measure $ \mu $ on T. This is equivalent to saying that A is $ \mu $-measurable for every measure $ \mu $ on T with *compact support* (\S 1, No. 8, Prop. 9).

(1) Recall (GT, I, §9, Exer. 14; TG, IX, Appendix I) that a *Lindelöf space* is a topological space T such that every open covering of T contains a countable covering.

#### Proposition 2 {#int-ix-s3-prop-2 .statement}

— Let X be a topological space and T a subspace of X.

a) Suppose that T is a Radon space. Then, for every function I defined on $ \mathcal{B}(X) $ that is positive, countably additive and bounded, one has

$$
\sup_{\substack{K \text{ compact} \\ K \subset T}} I(K) = \inf_{\substack{B \in \mathcal{B}(X) \\ B \supset T}} I(B).
$$

Moreover, T is universally measurable in X.

b) Conversely, suppose that X is a Radon space and that T is universally measurable in X; then T is a Radon space.

Let us prove a). We denote by $ \alpha $ the right side of (6); for every $ n \in \mathbf{N} $, there exists a set $ C_n \in \mathcal{B}(X) $ containing T, such that $ I(C_n) \leq \alpha + 2^{-n} $. Setting $ C = \bigcap_n C_n $, we then have $ T \subset C $, $ I(C) = \alpha $. If $ A \in \mathcal{B}(T) $, let us choose a Borel set B of X such that $ A = B \cap T $ (GT, IX, §6, No. 3) and set $ J(A) = I(B \cap C) $. This number does not depend on the choice of B, for if $ B' $ is a second Borel set in X such that $ A = B' \cap T $, then $ B \cap C $ and $ B' \cap C $ differ only by a Borel set M contained in $ C - T $, and $ I(M) = 0 $ by the construction of C. Clearly $ J(K) = I(K) $ for every compact set $ K \subset T $. Let $ (A_n) $ be a sequence of Borel sets of T, pairwise disjoint, and, for each $ n $, let $ B_n $ be a Borel set of X such that $ B_n \cap T = A_n $. Replacing $ B_n $ by $ B_n - \left( \bigcup_{k < n} B_k \right) $ if necessary, we can suppose that the sets $ B_n $ are pairwise disjoint. Set $ A = \bigcup_n A_n $ and $ B = \bigcup_n B_n $; then

$$
J(A) = I(B \cap C) = \sum_n I(B_n \cap C) = \sum_n J(A_n);
$$

J is thus a countably additive and bounded function on $ \mathcal{B}(T) $. Since T is by hypothesis a Radon space, there exists a bounded measure $ \mu $ on T such that $ J(A) = \mu^\bullet(A) $ for every $ A \in \mathcal{B}(T) $; consequently

$$
\alpha = J(T) = \mu^\bullet(T) = \sup_K \mu^\bullet(K) = \sup_K J(K),
$$

by the definition of $ \mu^\bullet $. Formula (6) is thus established.

Let us now show that T is universally measurable. Let $ \lambda $ be a bounded measure on X; the preceding argument may be applied to the set function $ I : A \mapsto \lambda^\bullet(A) $ on $ \mathcal{B}(X) $, thus there exists a sequence $ (K_n) $ of compact subsets of T such that (with the above notations)

$$
\sup_n \lambda^\bullet(K_n) = J(T) = \lambda^\bullet(C).
$$

Set $ K' = \bigcup_{n \in \mathbf{N}} K_n $; $ K' $ is Borel in $ X $, $ K' \subset T \subset C $, $ \lambda^*(K') = \lambda^*(C) $, therefore these three sets differ only by $ \lambda $-negligible sets, and so $ T $ is $ \lambda $-measurable. This completes the proof of $ a) $.

Let us pass to $ b) $. Suppose that $ X $ is a Radon space, and that $ T $ is universally measurable in $ X $. Let $ I $ be a positive function on $ \mathcal{B}(T) $ that is countably additive and bounded; the function $ A \mapsto I(A \cap T) $ on $ \mathcal{B}(X) $ is then positive, countably additive and bounded, therefore there exists a bounded measure $ \nu $ on $ X $ such that $ I(A \cap T) = \nu^*(A) $ for all $ A \in \mathcal{B}(X) $. Now, $ T $ is $ \nu $-measurable; the preceding relation shows that $ \nu^*(K) = 0 $ for every compact subset $ K $ of $ X $ that is disjoint from $ T $, therefore $ \nu $ is concentrated on $ T $. Consequently, for every Borel set $ A $ of $ X $, we have $ I(A \cap T) = \nu^*(A \cap T) = \mu^*(A \cap T) $, where $ \mu $ is the measure induced by $ \nu $ on $ T $. Finally, it follows that $ I(B) = \mu^*(B) $ for every set $ B \in \mathcal{B}(T) $ (GT, IX, §6, No. 3, *Remark 2*), and $ I $ is indeed inner regular.

#### Corollary {#int-ix-s3-n3-cor-1 .statement}

— *If $ X $ is a Radon space, then every Borel subset $ T $ of $ X $ is Radon.*

For, $ T $ is universally measurable in $ X $.

#### Proposition 3 {#int-ix-s3-prop-3 .statement}

— *Every Souslin space (in particular, every Polish or Lusin space) is strongly Radon.*

Let $ T $ be a Souslin space; since $ T $ is a Lindelöf space (TG, IX, Appendix I, Cor. of Prop. 1),(2) it suffices to show that $ T $ is Radon (Prop. 1). Let $ I $ be a function defined on $ \mathcal{B}(T) $, positive, countably additive and bounded. We extend $ I $ to $ \mathcal{P}(T) $ by setting, for every subset $ A $ of $ T $,

$$
I(A) = \inf_{\substack{B \in \mathcal{B}(T) \\ B \supseteq A}} I(B).
$$

Let us show that this extension is a *capacity* on $ T $ (GT, IX, §6, No. 9). It is clear that the relation $ A \subset A' $ implies $ I(A) \leq I(A') $. Let $ (A_n) $ be an increasing sequence of subsets of $ T $, and let $ A = \bigcup_n A_n $. The set of Borel sets that contain $ A_n $ being stable for countable intersections, there exists for each $ n $ a Borel set $ B_n $ such that $ A_n \subset B_n $ and $ I(A_n) = I(B_n) $ (cf. the proof of Prop. 2). Set $ C_n = \bigcap_{p \geq n} B_p $; $ C_n $ is Borel, and $ A_n \subset C_n \subset B_n $, therefore $ I(A_n) = I(C_n) $. On the other hand, the sequence $ (C_n) $ is increasing. Let $ C = \bigcup_n C_n $: the relation $ A \subset C $ implies that

$$
I(A) \leq I(C) = \lim_n I(C_n) = \lim_n I(A_n),
$$

(2) Every Souslin space has a countable base for open sets (GT, IX, §6, No. 2, Prop. 4), hence is Lindelöf (GT, I, §9, Exer. 14).

whence the equality $ I(A) = \lim_n I(A_n) $ is immediate. Consequently, I is a capacity.

If $(H_n)$ is a decreasing sequence of closed sets in T, obviously $ I\left( \bigcap_n H_n \right) = \inf_n I(H_n) $. It follows that every Souslin subset F of T is capacitable for I (TG, IX, §6, No. 10, Prop. 15). In particular, every Borel set A of T is capacitable (*loc. cit.*, §6, No. 3, Prop. 10).(3) In other words,

$$
I(A) = \sup_K I(K),
$$

where K runs over the set of compact sets contained in A; we have proved that I is inner regular.

#### Remark {#int-ix-s3-n3-rem-1 .statement}

— Let X be a Lusin space (in particular, any Polish space), and f a bijective continuous mapping of X onto a (Lusin) regular space Y. One knows (TG, IX, §6, No. 7, Prop. 14) that the mapping $ B \mapsto f^{-1}(B) $ is a bijection of the Borel tribe of Y onto the Borel tribe of X. The spaces X and Y are Lusin, hence strongly Radon (Prop. 3). It follows immediately that the mapping $ \mu \mapsto f(\mu) $ is a bijection of the set of bounded measures on X onto the set of bounded measures on Y.(4)

### Exercises {#int-ix-s3-exercises}

See the [exercises for § 3](exercises/s3/).
