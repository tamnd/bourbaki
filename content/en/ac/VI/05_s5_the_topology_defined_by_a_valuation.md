---
book: ac
book_title: Commutative Algebra
chapter: VI
chapter_title: VALUATIONS
section: 5
section_title: The topology defined by a valuation
lang: en
source: ac-i-vii
book_pages: 399-403, 454-459
pdf_pages: 0417-0421, 0472-0477
extraction: ocr
subsections:
    - "no": 1
      title: THE TOPOLOGY DEFINED BY A VALUATION
      page: 399
      pdf_page: 417
    - "no": 2
      title: TOPOLOGICAL VECTOR SPACES OVER A FIELD WITH A VALUATION
      page: 401
      pdf_page: 419
    - "no": 3
      title: THE COMPLETION OF A FIELD WITH A VALUATION
      page: 402
      pdf_page: 420
statements: 10
exercises: 9
content_sha256: 9cd13a5bfd2f4741f437a89f3a3f7401bd3878e9426716d3050719cf0d878bbd
---

## 5. THE TOPOLOGY DEFINED BY A VALUATION

### 1. THE TOPOLOGY DEFINED BY A VALUATION

Let K be a not necessarily commutative field, v a valuation on K and G the totally ordered group $v(K^*)$. For all $a \in G$ let V, be the set of $x \in K$ such that $v(x) > a$; this set is an additive subgroup of K (\S 3, no. 1). There exists a unique topology $\mathcal{T}_v$ on K for which the V, form a fundamental system of neighbourhoods of 0 (*General Topology*, Chapter III, \S 1, no. 2, Example). For v to be improper, it is necessary and sufficient that $\mathcal{T}_v$ be the discrete topology.

#### Lemma 1 {#ac-vi-s5-lem-1 .statement}

*Let $x \in K^*, y \in K^*$ and $\alpha \in G$. If*
$$
v(x - y) > \sup(\alpha + 2v(y), v(y)),
$$
*then* $v(x^{-1} - y^{-1}) > a$.

$x^{-1} - y^{-1} = x^{-1}(y - x)y^{-1}$ and hence
$$
v(x^{-1} - y^{-1}) = v(x - y) - v(x) - v(y).
$$
If $v(x - y) > v(y)$, Proposition 1 of \S 3, no. 1 implies that $v(x) = v(y)$, since $x = y + (x - y)$. Moreover, if $v(x - y) > a + 2v(y)$, then
$$
v(x^{-1} - y^{-1}) > a + 2v(y) - 2v(y) = a.
$$

#### Proposition 1 {#ac-vi-s5-prop-1 .statement}

*The topology $\mathcal{T}_v$ is Hausdorff and compatible with the field structure on K. The mapping $v : K^* \to G$ is continuous if G is given the discrete topology.*

Let $x \in K^*$ and $a = v(x)$; then $x \notin V_a$ which shows that $\mathcal{T}_v$ is Hausdorff. For all $x_0 \in K$ and $a \in G$, there exists $\beta \in G$ such that $x_0 V_\beta \subset V_\alpha$ and $V_\beta x_0 \subset V$, (it is sufficient to take $\beta \geqslant a - v(x_0)$). On the other hand, if $a \geqslant 0$, then $V_\alpha V_\alpha \subset V_v$. The axioms (AV_I) and (AV_{II}) of *General Topology*, Chapter III, § 6, no. 3 being thus satisfied, $ \mathcal{T}_v $ is compatible with the ring structure on $ K $. Let $ x_0 \in K^* $; if $ x \in K^* $ satisfies $ v(x - x_0) > \sup(\alpha + 2v(x_0), v(x_0)) $, then $ v(x^{-1} - x_0^{-1}) > a $ (Lemma 1), which shows that $ x \mapsto x^{-1} $ is continuous and that $ \mathcal{T}_v $ is therefore compatible with the field structure on $ K $. Finally, the single condition $ v(x - x_0) > v(x_0) $ implies $ v(x) = v(x_0) $ ($ \S 3 $, no. 1, Proposition 1) and hence the mapping $ v : K^* \to G $ is continuous if $ G $ is given the discrete topology.

Let $ \alpha \in G $ and $ V'_\alpha $ be the set of $ x \in K $ such that $ v(x) \geq \alpha $. If $ \beta < a $, then $ V_\beta \supset V'_\alpha \supset V_v $. If $ v $ is not improper, it is therefore seen that the $ V'_\alpha $ form a fundamental system of neighbourhoods of 0 for $ \mathcal{T}_v $.

The $ V_v $ and the $ V'_\alpha $ are open additive subgroups and therefore closed in $ K $ and therefore the topological field $ K $ is *totally disconnected*. As every non-zero ideal of the ring of $ v $ contains a $ V_v $, it is *open and closed* in $ K $. The quotient topology on the residue field of $ v $ is therefore *discrete*.

Let $ A $ be the ring of $ u $. If $ v $ is discrete, Proposition 8 of $ \S 3 $, no. 6 shows that the topology induced by $ \mathcal{T}_v $ on $ A $ is the $ m(A) $-adic topology. This is not so in general (Exercise 4).

#### Proposition 2 {#ac-vi-s5-prop-2 .statement}

*Let $ K $ be a not necessarily commutative field, $ v $ a non-improper valuation on $ K $, $ A $ the ring of $ v $ and $ m $ the ideal of $ v $. For $ K $ with the topology $ \mathcal{T}_v $ to be locally compact, it is necessary and sufficient that the following conditions be fulfilled:*

(i) $ K $ is complete;
(ii) $ v $ is discrete;
(iii) *the residue field $ \kappa(A) $ is finite.*

*If so*, $ A $ is compact.

Suppose $ K $ is locally compact. Then it is complete (*General Topology*, Chapter 111, $ \S 3 $, no. 3, Corollary 1 to Proposition 4); further there exists a compact neighbourhood of 0, which contains a neighbourhood $ V'_a $, where $ a $ belongs to the value group of $ v $; in other words, there exists $ a \neq 0 $ in $ K^* $ such that $ A . a $ is compact and it follows that $ A = (A . a)a^{-1} $ is compact. As every ideal $ b \neq (0) $ of $ A $ is open, $ A/b $ is compact and discrete (*General Topology*, Chapter III, $ \S 2 $, no. 5, Proposition 14) and therefore finite and in particular $ \kappa(A) = A/m $ is finite. Moreover, for $ y \neq 0 $ in $ m $, the ring $ A/Ay $ being finite, there is only a finite number of ideals of $ A $ containing $ Ay $ and the set $ P $ of elements of the form $ v(x) $ such that

$$
0 < v(x) \leq v(y)
$$

is finite; as $ v(K^*) $ is totally ordered, $ P $ has a least element $ y $. Then for all $ x \in A $ such that $ v(x) > 0 $, either $ v(x) > v(y) \geq y $, or $ v(x) \leq v(y) $ and then $ v(x) \geq y $ by definition, so that $ y $ is the least of the elements $ > 0 $ of $ v(K^*) $. *As* $ P $ *is* finite, there is a greatest integer $ m \geq 0 $ such that $ my \in P $, whence my \leq v(y) < (m+1)\gamma. We deduce that 0 \leq v(y) - my < y and by definition of y this implies $ v(y) = my $. Therefore $ v(K^*) = \mathbf{Z}.\gamma $ and the valuation $ v $ is discrete.

Conversely, suppose conditions (i), (ii), (iii) hold. We may restrict our attention to the case where $ v $ is normed; let $ u $ be a uniformizer for $ v $. Then $ \kappa(A) = A/Au $ and hence $ A/Au $ is finite. As $ x \mapsto xu^n $ defines by taking quotients an isomorphism of the additive group $ A/Au $ onto $ Au^n/Au^{n+1} $, $ A/Au^j $ is finite for all $ j \geq 0 $. As $ A $ is closed in $ K $, it is complete and hence isomorphic to the inverse limit of the $ A/Au^j $ (General Topology, Chapter 111, § 7, no. 3, Proposition 2) and therefore compact. Since $ A $ is open in $ K $, it is therefore seen that $ K $ is locally compact.

#### Remark {#ac-vi-s5-n1-rem-1 .statement}

Note that it is sufficient in this proof to suppose that $ A $ is complete.

We shall see in § 9 that a field $ K $ fulfilling the conditions of Proposition 2 admits a centre which is either a finite algebraic extension of a $ p $-adic field, or a field $ \mathbf{F}_q((T)) $ of formal power series over a finite field; moreover $ K $ is of finite rank over its centre.

### 2. TOPOLOGICAL VECTOR SPACES OVER A FIELD WITH A VALUATION

Throughout let $ K $ be a (not necessarily commutative) field, $ v $ a valuation on $ K $ and $ G $ its order group. $ K $ is given the topology $ \mathcal{T}_v $.

#### Proposition 3 {#ac-vi-s5-prop-3 .statement}

Let $ E $ be a left topological vector space over $ K $ which is Hausdorff and of dimension 1. Suppose that $ v $ is not improper. For all $ x_0 \neq 0 $ in $ E $, the mapping $ a \mapsto ax_0 $ of $ K_s $ onto $ E $ is a topological isomorphism.

This mapping is a continuous algebraic isomorphism. It is sufficient to show that it is bicontinuous. Let $ \alpha \in G $. We need to show that there exists a neighbourhood $ V $ of 0 in $ E $ such that the relation $ ax_0 \in V $ implies $ v(a) > a $. Let $ a, \in K^* $ be such that $ v(a_0) = a $. As $ E $ is Hausdorff, there exists a neighbourhood $ W $ of 0 in $ E $ such that $ a_0x_0 \notin W $. As $ v $ is not improper, there exist a neighbourhood $ W' $ of 0 in $ E $ and an element $ \beta $ of $ G $ such that the relations $ y \in W' $, $ v(a) \geq \beta $ imply $ ay \in W $. Let $ a, \in K^* $ be such that $ v(a_1) = -\beta $. The relations $ ax_0 \in a_1^{-1}W' $ and $ v(a) \leq a $ imply $ a_1ax_0 \in W $ and $ v(a_0a^{-1}a_1^{-1}) = \alpha + \beta - v(a) \geq \beta $ and hence $ a_0x_0 = a_0a^{-1}a_1^{-1}(a_1ax_0) \in W $, which is absurd; in other words, the relation $ ax, \in a_1^{-1}W $ implies $ v(a) > a $.

#### Corollary {#ac-vi-s5-n2-cor-1 .statement}

Let $ E $ be a left topological vectorspace over $ K $, $ H $ a closed hyperplane of $ E $ and $ D $ a 1-dimensional vector subspace of $ E $ an algebraic supplement of $ H $. Suppose that $ v $ is not improper. Then $ D $ is a topological supplement of $ H $.

Taking account of Propositions 1 and 3, the proof is the same as that of Topological Vector Spaces, Chapter I, § 2, Corollary 2 to Theorem 1.

#### Proposition 4 {#ac-vi-s5-prop-4 .statement}

Suppose that $ v $ is not improper and $ K $ is complete. Let $ E $ be a left topological vector space over $ K $, which is Hausdorff and of finite dimension $ n $. For every basis $ (e_i)_{1 \leq i \leq n} $ of $ E $ over $ K $, the mapping $ (a_i) \mapsto \sum_{i=1}^n a_i e_i $ of $ K^n_s $ onto $ E $ is a topological vector space isomorphism.

Taking account of Proposition 3 and its corollary, the proof is the same as that of Topological Vector Spaces, Chapter I, § 2, Theorem 2.

#### Corollary {#ac-vi-s5-n2-cor-2 .statement}

Suppose that $ v $ is not improper and $ K $ is complete. Let $ E $ be a Hausdorff topological vector space over $ K $ and $ F $ a finite-dimensional vector subspace of $ E $. Then $ F $ is closed.

$ F $ is complete.

### 3. THE COMPLETION OF A FIELD WITH A VALUATION

#### Proposition 5 {#ac-vi-s5-prop-5 .statement}

Let $ K $ be a not necessarily commutative field, $ v $ a valuation on $ K $ and $ G $ the group $ v(K^*) $ with the discrete topology.

(a) The completion ring $ \hat{K} $ of $ K $ (with $ \mathcal{T}_v $) is a topological field.

(b) The mapping $ v : K^* \to G $ can be extended uniquely to a continuous mapping $ 8 : \hat{K}^* \to G $. The mapping $ 0 $ (extended by $ \hat{v}(0) = +\infty $) is a valuation on $ \hat{K} $ and $ \hat{v}(\hat{K}^*) = v(K^*) $.

(c) The topology on $ \hat{K} $ is the topology defined by the valuation $ 0 $.

(d) For all $ a \in G $ let $ V_\alpha, V'_\alpha $ be the subgroups of $ K $ defined by the conditions $ v(x) > a, v(x) \geq a $. Then the closures $ \overline{V}_\alpha, \overline{V}'_\alpha $ of $ V_\alpha, V'_\alpha $ in $ \hat{K} $ are defined by the conditions $ \hat{v}(x) > a, \hat{v}(x) \geq a $ respectively.

(e) The ring of $ 0 $ is the completion $ \hat{A} $ of the ring $ A $ of $ v $; the ideal of $ 0 $ is the completion $ \hat{m} $ of the ideal $ m $ of $ v $.

(f) $ \hat{A} = A + m $; the residue field of $ 8 $ is canonically identified with that of $ v $.

To prove (a) it suffices (General Topology, Chapter III, § 6, no. 8, Proposition 7) to show the following: let $ \mathfrak{F} $ be a Cauchy filter (with respect to the additive uniform structure) on $ K^* $ for which $ 0 $ is not a cluster point; then the image of $ \mathfrak{F} $ under the bijection $ x \mapsto x^{-1} $ is a Cauchy filter (with respect to the additive uniform structure). For since $ 0 $ is not a cluster point of $ \mathfrak{F} $, there exists $ M \in \mathfrak{F} $ and $ \beta \in G $ such that $ \beta $ is an upper bound of $ v(M) $. Let $ a \in G $. If $ M' $ is an element of $ \mathfrak{F} $ contained in $ M $ and such that $ v(x - y) > \sup(\alpha + 2\beta, \beta) $ for $ x \in M' $ and $ y \in M' $, then $ v(x^{-1} - y^{-1}) > a $ for $ x \in M' $ and $ y \in M' $ (no. 1, Lemma 1). Whence (a).

By Proposition 1 of no. 1, $ v|K^* $ is a continuous homomorphism from $ K^* $ to $ G $ and hence can be extended uniquely to a continuous homomorphism $ 0 $ from $ K^* $ to $ G $. the Relation

$$
\hat{v}(x + y) \geq \inf(\hat{v}(x), \hat{v}(y))
$$

holds in $ K^* $ and hence also holds in $ \hat{K}^* $ by continuity. Thus 0 (extended by $ \hat{v}(0) = +\infty $) is a valuation on $ \mathbf{K} $ and (b) is proved.

We now show (d). Let $ a \in G $ and $ x \in \mathcal{S}, -\{0\} $. For $ y $ in $ V $, sufficiently close to $ x $, $ \hat{v}(x) = \hat{v}(y) = v(y) $ and hence $ \hat{v}(x) > a $. Conversely, let $ x \in \hat{K}^* $ be such that $ \hat{v}(x) > a $; for $ y $ in $ K^* $ sufficiently close to $ x $, $ v(y) = \hat{v}(y) = \hat{v}(x) $ and therefore $ y \in V $, whence $ x \in \mathcal{S} $. Thus $ \mathcal{S} $ is the set of $ x \in \hat{K} $ such that $ \hat{v}(x) > a $. The argument is analogous for $ V'_a $. This proves (d).

Taking account of Proposition 7 of General Topology, Chapter III, § 3, no. 4, assertion (c) is a consequence of (d). Assertion (e) is a special case of (d). Finally let $ x \in \hat{A} $; there exists $ y \in A $ such that $ \hat{v}(x - y) > 0 $; then $ z = x - y \in \hat{m} $ and hence $ x = y + z \in A + \hat{m} $; thus $ \hat{A} = A + \hat{m} $, which shows (f).

#### Remark {#ac-vi-s5-n3-rem-1 .statement}

For all $ x \in \hat{K} $ not belonging to $ \hat{A} $, there exists $ x_0 \in K $ such that $ \hat{v}(x - x_0) > 0 $, $ \hat{v}(x) = \hat{v}(x_0) = v(x_0) < 0 $; then $ x_0^{-1} x \in \hat{A} $ and, as $ x_0^{-1} \in A $, it is seen that, if we set $ S = A - \{0\} $, it is possible to write $ \hat{K} = S^{-1} \hat{A} $.

### Exercises {#ac-vi-s5-exercises}

degree $ n > 1 $ and such that $ a_i \neq 0 $; show that there exists a strictly increasing sequence $ (i_k)_{0 \leq k \leq r} $ of integers in the interval $[0, n]$ such that: (1) $ i_0 = 0 $, $ i_r = n $; (2) $ v(a_{i_k}) $ is finite for $ 0 \leq k \leq r $; (3) for every index $ j $ such that $ 0 \leq j \leq n $ distinct from the $ i_k $, such that $ v(a_j) $ is finite, the point
$$
(j, v(a_j)) \in \mathbf{R}^2
$$
lies above the line passing through the points $ (i_k, v(a_{i_k})) $ and $ (i_{k+1}, v(a_{i_{k+1}})) $ and strictly above that line if $ j < i_k $ or $ j > i_{k+1} $. The union of the segments joining the points $ (i_k, v(a_{i_k})) $ and $ (i_{k+1}, v(a_{i_{k+1}})) $ is called the Newton polygon of P, the above segments are called the sides and the points $ (i_k, v(a_{i_k})) $ the vertices of the polygon.

(b) Suppose that all the zeros of P belong to K. Show that for the valuations of all the zeros of P to be the same, it is necessary and sufficient that $ r = 1 $ (in other words, that the Newton polygon reduce to a single side). (To show that the condition is sufficient, consider the Newton polygon of a product $ P_1P_2 $ where all the zeros of $ P_1 $ are invertible in the ring of $ v $, whilst all those of $ P_2 $ belong to the ideal of $ v $.)

(c) Suppose that all the zeros of P belong to K; form the Newton polygon of P and write.
$$
\rho_k = i_{k+1} - i_k, \quad \sigma_k = (v(a_{i_{k+1}}) - v(a_{i_k}))/\rho_k.
$$
Show that, for $ 0 \leq k \leq r - 1 $, P admits exactly $ \rho_k $ zeros (counted with their orders of multiplicity) whose valuations are all equal to $ \sigma_k $ (use (b) and argue by induction on $ r $).

(d) Generalize to the case of any valuation $ v $ (embed the order group $ \Gamma $ of $ v $ in the vector Q-space $ \Gamma_{(0)} $, which has a natural totally ordered group structure).

95

See the [exercises for § 5](exercises/s5/).
