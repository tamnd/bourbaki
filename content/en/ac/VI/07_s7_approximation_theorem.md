---
book: ac
book_title: Commutative Algebra
chapter: VI
chapter_title: VALUATIONS
section: 7
section_title: Approximation theorem
lang: en
source: ac-i-vii
book_pages: 412-416, 460-461
pdf_pages: 0430-0434, 0478-0479
extraction: ocr
subsections:
    - "no": 1
      title: THE INTERSECTION OF A FINITE NUMBER OF VALUATION RINGS
      page: 412
      pdf_page: 430
    - "no": 2
      title: INDEPENDENT VALUATIONS
      page: 413
      pdf_page: 431
    - "no": 3
      title: THE CASE OF ABSOLUTE VALUES
      page: 415
      pdf_page: 433
statements: 14
exercises: 3
content_sha256: c3aad445a74a634a4e68fae3d957708fb3ee60bb71eec383f8e89568290b9ba9
---

## 7. THE APPROXIMATION THEOREM

### 1. THE INTERSECTION OF A FINITE NUMBER OF VALUATION RINGS

#### Proposition 1 {#ac-vi-s7-prop-1 .statement}

Let $ K $ be a field, $(\mathbf{A}_i)_{1 \leq i \leq n}$ ajinitefamily of valuation rings of $ K $ and $ B = \bigcap_{i=1}^n \mathbf{A}_i $. We write $ p_i = B \cap m(\mathbf{A}_i) $. Then $ A_i = B_{p_i} $ for all $ i $ and the jield of ructions of $ B $ is $ K $.

Clearly $ B_{p_i} \subset A_i $. To prove the converse inclusion we need the following lemma:

#### Lemma 1 {#ac-vi-s7-lem-1 .statement}

Let $ v_i $ ($ 1 \leq i \leq n $) be ualuations on the jield $ K $ and $ x \in K^* $. Then there exists a polynomialf $ (X) $ of theform

$$
f(X) = 1 + n_1 X + \cdots + n_{k-1} X^{k-1} + X^k \quad (k \geq 2,\ n_j \in \mathbf{Z} \text{ for } 1 \leq j \leq k - 1)
$$

such that $ f(x) \neq 0 $ and the element $ z = f(x)^{-1} $ enjoys the following propertiesfor $ 1 \leq i \leq n $:

$$
v_i(z) = 0 \qquad \text{if} \quad v_i(x) \geq 0 \\
v_i(z) + v_i(x) > 0 \qquad \text{if} \quad v_i(x) < 0.
$$

Assuming this lemma for a moment, we show how it implies that $ A_1 \subset B_{p_1} $. Let $ x $ be a non-zero element of $ A_i $. We apply the lemma to $ x $ and valuations $ v_i $ associated with the $ \mathbf{A}_i $. Then $ v_i(z) \geq 0 $ and $ v_i(zx) \geq 0 $ for all $ i $, hence $ z \in B $ and $ zx \in B $. As $ v_1(x) \geq 0 $, $ v_1(z) = 0 $ and hence $ z \notin p_1 $. Hence $ x = zx/z \in B_{p_1} $. The field of fractions of $ B $ then contains $ A_1 $ and hence is $ K $.

We now pass to the proof of the lemma. Let $ I $ be the set of indices $ i $ such that $ v_i(x) \geq 0 $. For all $ i \in I $, let $ \bar{x}_i $ denote the canonical image of $ x $ in $ \kappa(\mathbf{A}_i) $. For all $ i \in I $ we construct a polynomialf, as follows: if there exists a polynomial $ g(X) $ of the form (1) such that $ g(\bar{x}_i) = 0 $ in $ \kappa(\mathbf{A}_i) $, we takef, to be such a polynomial; otherwise we take $ f_i = 1 $. Then we write $ f(X) = 1 + X^2 \prod_{i \in I} f_i(X) $. It is obviously a polynomial of the form (1). If $ i \in I $, then $ f(x) \in A_i $ and alsof $ (\bar{x}_i) \neq 0 $ by construction; hence $ f(x) \notin m(\mathbf{A}_i) $, $ v_i(f(x)) = 0 $ and $ v(z) = 0 $. If $ i \notin I $, then $ v_i(x) < 0 $, whence $ v_i(f(x)) = kv_i(x) $ (\S 3, no. 1, Proposition 1) and

$$
v_i(x) + v_i(z) = (1 - k)v_i(x) > 0
$$

(since $ k \geq 2 $). Whence the lemma.

#### Proposition 2 {#ac-vi-s7-prop-2 .statement}

With the hypotheses of Proposition 1 suppose further that $ \mathbf{A}_i \not\subset \mathbf{A}_j $ for $ i \neq j $. Then the $ p_i $ are distinct maximal ideals of $ B $ and every maximal ideal of $ B $ is equal to one of the $ p_i $.

If $ p_i \subset p_j $ for $ i \neq j $, $ \mathbf{A}_i = B_{p_i} \supset B_{p_j} = \mathbf{A}_j $. It is then sufficient to apply Chapter II, \S 3, no. 5, Corollary to Proposition 17.

#### Corollary 1 {#ac-vi-s7-prop-2-cor-1 .statement}

Suppose that $ A_i \not\subset A_j $ for $ i \neq j $. For every family of elements $ a_i \in A_i $ ($ 1 \leq i \leq n $), there exists $ x \in B $ such that $ x \equiv a_i \pmod{m(A_i)} $ for $ 1 \leq i \leq n $.

Since the $ p_i $ are maximal ideals of $ B $, $ A_i/m(A_i) = B_{p_i}/p_iB_{p_i} = B/p_i $ and it may therefore be assumed that $ a_i \in B $ for all $ i $. The corollary then follows from the fact that the canonical mapping from $ B $ to $ \prod_{i=1}^n (B/p_i) $ is surjective (Chapter 11, § 1, no. 2, Proposition 5).

#### Corollary 2 {#ac-vi-s7-prop-2-cor-2 .statement}

Suppose that $ A_i \not\subset A_j $ for $ i \neq j $. There exist elements $ x_i $ ($ 1 \leq i \leq n $) of $ K $ such that $ v_i(x_i) = 0 $ and $ v_j(x_i) > 0 $ for $ i \neq j $.

For each index $ i $ apply Corollary 1 to the family $ (a_i) $ such that $ a_i = 1 $ and $ a_j = 0 $ for $ j \neq i $.

#### Corollary 3 {#ac-vi-s7-prop-2-cor-3 .statement}

Every valuation ring of $ K $ containing $ B $ contains one of the $ A_i $.

We may confine our attention to the case where $ A_i \not\subset A_j $ for $ i \# j $. Let $ V $ be a valuation ring of $ K $ containing $ B $. We write
$$
p = m(V) \cap B.
$$
There exists a maximal ideal $ p_i $ of $ B $ containing $ p $, whence
$$
A_i = B_{p_i} \subset B, \subset V.
$$

### 2. INDEPENDENT VALUATIONS

#### Definition 1 {#ac-vi-s7-def-1 .statement}

Let $ A $ and $ A' $ be two valuation rings of the same field $ K $. $ A $ and $ A' $ are called independent if $ K $ is the ring generated by $ A $ and $ A' $. Two valuations on $ K $ are called independent if their rings are independent and dependent otherwise.

An improper valuation on $ K $ is independent of every valuation on $ K $. For two valuations of height 1 on $ K $ to be independent, it is necessary and sufficient that they be not equivalent (§ 4, no. 5, Proposition 6 (c)).

#### Theorem 1 (Approximation Theorem for Valuations) {#ac-vi-s7-thm-1 .statement}

Let $ v_i $ ($ 1 \leq i \leq n $) be valuations on a field $ K $ which are independent in pairs and $ \Gamma_i $ the order group of $ v_i $. Let $ a_i \in K $ and $ \alpha_i \in \Gamma_i $ ($ 1 \leq i \leq n $). Then there exists $ x \in K $ such that $ v_i(x - a_i) \geq \alpha_i $ for all $ i $

If $ v_i $ is improper, then $ a_i = 0 $ and the relation $ v_i(x - a_i) \geq a_i $ is true for all $ x \in K $. We may therefore assume that the $ v_i $ are not improper.

Let $ A_i $ be the ring of $ v_i $, $ B = \bigcap_{i=1}^n A_i $ and $ p_i = m(A_i) \cap B $. By Proposition 1 of no. 1, the $ a_i $ may be written $ a_i = b_i/s $ ($ b_i \in B, s \in B - \{0\} $); if we write $ x = y/s $ and $ \alpha_i' = \alpha_i + v_i(s) $, then $ v_i(y - 6_i) \geq \alpha_i' $. This shows that we may assume that $ a_i \in B $ for all $ i $; we may also assume that $ \alpha_i > 0 $ for all $ i $. Let $ v_i $ be the set of z \in \mathbf{K} \text{ such that } v_i(z) \geq a, \text{ we write } q_i = v_i \cap B. \text{ For } x \in B, v_i(x - a_i) \geq \alpha_i \text{ is equivalent to } x \equiv a_i (\mathfrak{q}_i). \text{ We therefore need to show that the canonical homomorphism } B \to \prod_{i=1}^n (B/q_i) \text{ is surjective, that is that } q_i + q_j = B \text{ for } i \neq j \text{ (Chapter 11, § 1, no. 2, Proposition 5). As the maximal ideals of B are the } \mathfrak{p}_i \text{ (Proposition 2), it will suffice for this to show that } q_i \notin \mathfrak{p}_j \text{ for } i \neq j.

Suppose that there exists $ i, j $ such that $ q_i \subset \mathfrak{p}_j $ and $ i \neq j $. We shall see shortly that the radical of $ q_i $ is a *prime* ideal $ p $ of B. Then $ p \subset \mathfrak{p}_j $ and also $ p \subset \mathfrak{p}_i $ since $ \alpha_i > 0 $ and hence $ q_i \subset \mathfrak{p}_i $. Therefore $ A_1 = B_s \subset B_p $ (no. 1, Proposition 1) and similarly $ A_1 \subset B_r $. Now, as $ v_i \neq (0) $ and $ v_i = B_{\mathfrak{p}_i} q_i $ (Chapter 11, § 2, no. 4, Proposition 10), $ q_i \neq (0) $, whence $ p \neq (0) $ and $ B_r \neq K $. This contradicts the hypothesis that $ A_1 $ and $ A_1 $ are independent.

It remains to show that $ p $ is prime. Now this follows from the following lemma:

#### Lemma 2 {#ac-vi-s7-lem-2 .statement}

*Let A be a valuation ring and b an ideal of A distinct from A. Then the radical c of b is a prime ideal.*

Suppose that $ xy \in c $. Then there exists $ n \geq 1 $ such that $ (xy)^n \in b $. Let $ v $ be a valuation associated with A. If, for example, $ v(x) \geq v(y) $, then

$$
v(x^{2n}) \geq v(x^n y^n),
$$

whence $ x^{2n} \in b $ and $ x \in c $.

#### Corollary 1 {#ac-vi-s7-lem-2-cor-1 .statement}

*For every family of elements $ \gamma_i \in \Gamma_i $ ($ 1 \leq i \leq n $), there exists $ x \in K $ such that $ v_i(x) = \gamma_i $ ($ 1 \leq i \leq n $).

We may assume that $ A_i \neq K $ for all $ i $. Then, there exists for all $ i $ an $ a_i \in K $ such that $ v_i(a_i) = \gamma_i $ and an $ a_r \in \Gamma_r $ such that $ \gamma_i < a_r $. We apply Theorem 1 to these elements $ a_i $: there exists $ x \in K $ such that $ v_i(x - a_i) > v_i(a_i) $; whence, as $ x = a_i + (x - a_i) $, $ v_i(x) = v_i(a_i) = \gamma_i $ ($ \S 3 $, no. 1, Proposition 1).

#### Corollary 2 {#ac-vi-s7-lem-2-cor-2 .statement}

*Let $ \mathcal{T}_i $ be the topology defined on $ K $ by $ v_i $; let $ K^n $ be given the topology the product of the $ \mathcal{T}_i $. If the $ v_i $ are not improper, the diagonal of $ K^n $ is dense in $ K^n $.

#### Proposition 3 {#ac-vi-s7-prop-3 .statement}

*Let $ v $ and $ v' $ be two non-improper valuations on the same field $ K $. For $ v $ and $ v' $ to define the same topology on $ K $, it is necessary and sufficient that they be dependent.

Suppose that the topologies $ \mathcal{T}_v $ and $ \mathcal{T}_{v'} $, defined by $ v $ and $ v' $, are identical. Since $ \mathcal{T}_v $ is Hausdorff, the diagonal of $ K^2 $ is closed and hence $ v $ and $ v' $ are dependent (Corollary 2 to Theorem 1).

Conversely, suppose that $ v $ and $ v' $ are dependent. Then their rings $ A $ and $ A' $ are contained in the same ring $ A'' $ distinct from $ K $ and $ A'' $ is the ring of a valuation $ v'' $ ($ \S 4 $, no. 1, Proposition 1). It suffices to show that the topology $ \mathcal{T}_{v''} $ is identical with $ \mathcal{T}_v $. Let $ \Gamma $ and $ \Gamma'' $ be the order groups of $ v $ and $ v'' $. There exists an increasing homomorphism $ \lambda $ of $ \Gamma $ onto $ \Gamma'' $ such that $ v'' = A \circ v $ ($ \S 4 $, no. 3). If $ a'' \in I?'' $, let $ a \in \lambda^{-1}(a'') $; the condition $ v(x) \geq \alpha $ implies $ v''(x) \geq a'' $. Let $ \beta \in \Gamma $ and $ \beta'' = \lambda(\beta) $; the condition $ v(x) \leq \beta $ implies $ v''(x) \leq \beta'' $ and hence the condition $ v''(x) > \beta'' $ implies $ v(x) > \beta $. As $ v $ and $ v'' $ are not improper, the inequalities in question define fundamental systems of neighbourhoods of 0 for $ \mathcal{T}_v $ and $ \mathcal{T}_{v''} $. Hence $ \mathcal{T}_v = \mathcal{T}_{v''} $, which completes the proof.

Remarks
(1) Proposition 3 shows that the relation '"$ v $ and $ v' $ are dependent"' is an equivalence relation.
(2) Taking account of the relations between valuations of height 1 and ultrametric absolute values (\S 6, no. 2), Proposition 3 also follows, in the case of valuations of height 1, from the characterization of equivalent absolute values (General Topology, Chapter IX, \S 3, no. 2, Proposition 5).

#### Proposition 4 {#ac-vi-s7-prop-4 .statement}

*Let $ v_1, \ldots, v_n $ ($ n \geq 2 $) be pairwise dependent valuations on the same field $ K $. Then the rings $ A,, \ldots, A, $ of $ v_1, \ldots, v, $ generate a subring $ \delta \ K $ distinct from $ K $.*

For $ n = 2 $ Proposition 4 follows from Definition 1. Suppose it holds for $ n - 1 $ valuations. Then there exists a subring A of K distinct from K and containing $ A,, \ldots, A, $; there also exists a subring B $ \neq K $ containing A, _, and A_. As A and B contain A, _, they are comparable with respect to inclusion (\S 4, no. 1, Corollary to Proposition 1). The greater of these two therefore contains all the $ A_i $.

### 3. THE CASE OF ABSOLUTE VALUES

#### Theorem 2 (Approximation Theorem for Absolute Values) {#ac-vi-s7-thm-2 .statement}

*Let $ f_i $ ($ 1 \leq i \leq n $) be absolute values on the same field $ K $ which are not improper and no two of which are equivalent. Let $ a, \ (1 \leq i \leq n) $ be elements of $ K $ and $ \varepsilon $ a real number $ > 0 $. Then there exists $ x \in K $ such that $ f_i(x - a,) \leq \varepsilon $ for all $ i $.*

Let $ K_i $ denote the field K with the topology defined by $ f_i $. The result to be proved is equivalent to the following: in the product $ P = K_1 \times \cdots \times K_n $, the closure $ \overline{D} $ of the diagonal D is equal to P. This is obvious for $ n = 1 $. Suppose that this point has been established in the case of k absolute values for $ k < n $.

We show first that there exists, for $ 2 \leq h \leq n $, an element $ x_h $ of K such that $ f_1(x_h) < 1, f_2(x_h) > 1 $ and $ f_i(x_h) \neq 1 $ for $ 3 \leq i \leq h $. We argue by induction on $ h $. If $ h = 2 $, this follows from the fact that $ f_1 $ and $ f_2 $ are not equivalent. We therefore suppose that the existence of $ x_{h-1} $ has been shown and prove that of $ x_h $. If $ f_h(x_{h-1}) \neq 1 $, we may take $ x_h = x_{h-1} $; if $ f_h(x_{h-1}) = 1 $, we choose $ z \in K^* $ such that $ f_h(z) \neq 1 $ and $ x_h = z(x_{h-1})^s $ solves the problem for s sufficiently large. We have thus proved the existence of $ x_h $.

As the integer $ q $ tends to infinity, $ f_1(x_n^q) $ tends to 0, $ f_2(x_n^q) $ tends to $ +\infty $ and $ f_i(x_n^q) $ tends to 0 or $ +\infty $ for $ i \geq 3 $. Writing $ y_q = x_n^q(1 + x_n^q)^{-1} $,
$$
1 - y_q = (1 + x_n^q)^{-1};
$$
hence the sequence $ (y,) $ tends to 0 in $ K_1 $, to 1 in $ K_2 $ and to 0 or 1 in $ K_i $ for $ i \geq 3 $. By changing the numbering of the $ K_i $, it may therefore be assumed that there exists an integer $ r $ ($ 1 \leq r < n $) such that $ \overline{D} $ contains the point $ (e_1, \ldots, e_n) $ where $ e_i = 1 $ for $ 1 \leq i \leq r $ and $ e_i = 0 $ for $ r + 1 \leq i \leq n $. Now, $ \overline{D} $ is a vector sub-K-space of P. Hence $ \overline{D} $ contains the diagonals D' and D'' of
$$
P' = K_1 \times \cdots \times K_r,
$$
and $ P'' = K_{r+1} \times \cdots \times K_n $. By the induction hypothesis, $ P' = \overline{D}' $ and $ P'' = \overline{D}'' $. Hence $ \overline{D} = P $.

### Exercises {#ac-vi-s7-exercises}

See the [exercises for § 7](exercises/s7/).
