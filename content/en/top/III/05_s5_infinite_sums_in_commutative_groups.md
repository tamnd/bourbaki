---
book: top
book_title: General Topology
chapter: III
chapter_title: Topological Groups
section: 5
section_title: Infinite sums in commutative groups
lang: en
source: top-i-iv
pdf_pages: 0267-0276, 0320-0321
extraction: ocr
subsections:
    - "no": 1
      title: SUMMABLE FAMILIES IN A COMMUTATIVE GROUP
      page: 0
      pdf_page: 267
    - "no": 2
      title: CAUCHY'S CRITERION
      page: 0
      pdf_page: 268
    - "no": 3
      title: PARTIAL SUMS ; ASSOCIATIVITY
      page: 0
      pdf_page: 270
    - "no": 4
      title: SUMMABLE FAMILIES IN A PRODUCT OF GROUPS
      page: 0
      pdf_page: 272
    - "no": 5
      title: IMAGE OF A SUMMABLE FAMILY UNDER A CONTINUOUS HOMOMORPHISM
      page: 0
      pdf_page: 273
    - "no": 6
      title: SERIES
      page: 0
      pdf_page: 273
    - "no": 7
      title: COMMUTATIVELY CONVERGENT SERIES
      page: 0
      pdf_page: 275
statements: 19
exercises: 5
content_sha256: a04569f1d51737a665ddf223a5887f3c79270fcedf0d0fe1ed5aefa3a1a5df76
---

## 5. INFINITE SUMS IN COMMUTATIVE GROUPS

### 1. SUMMABLE FAMILIES IN A COMMUTATIVE GROUP

In this section we shall be concerned only with *Hausdorff commutative topological groups*, whose law of composition is written *additively*. Only the most important results will be translated into multiplicative notation.

Let $ G $ be a Hausdorff commutative group, let $ I $ be any index set and let $ (x_i)_{i \in I} $ be a family of points of $ G $, indexed by $ I $. With each *finite* subset $ J $ of $ I $ we associate the element $ s_J = \sum_{i \in J} x_i $ of $ G $, which we call the *finite partial sum of the family* $ (x_i)_{i \in I} $, corresponding to the set $ J $. If $ \mathfrak{F}(I) $ denotes the *set of finite subsets* of $ I $, we have thus a mapping $ J \to s_J $ of $ \mathfrak{F}(I) $ into $ G $. Now $ \mathfrak{F}(I) $ is a *directed* set with respect to the relation $ \subset $; for if $ J $ and $ J' $ are two elements of $ \mathfrak{F}(I) $, then $ J \subset J \cup J' $ and $ J' \subset J \cup J' $, and $ J \cup J' $ is a finite subset of $ I $. Let $ \Phi $ be the *section filter* of the directed set $ \mathfrak{F}(I) $ (Chapter I, § 6, no. 3).

#### Definition 1 {#top-iii-s5-def-1 .statement}

Let $(x_i)_{i \in I}$ be a family of points of a Hausdorff commutative group $G$; let $\mathcal{F}(I)$ be the set of finite subsets of the index set $I$, and for each finite subset $J$ of $I$, let $s_J$ be the sum of those $x_i$ such that $i \in J$. The family $(x_i)_{i \in I}$ is said to be summable if the mapping $J \to s_J$ has a limit with respect to the section filter $\Phi$ of the set $\mathcal{F}(I)$ directed by the relation $\subset$; this limit is then said to be the sum of the family $(x_i)_{i \in I}$ and is denoted by $\sum_{i \in I} x_i$ (or simply $\sum_i x_i$, or even $\sum x_i$, when there is no risk of ambiguity).

Definition 1 is equivalent to the following: *the family* $(x_i)$ *is summable and its sum is* $s$ *if, for each neighbourhood* $V$ *of the origin in* $G$, *there is a finite subset* $J_0$ *of* $I$ *such that for each finite subset* $J \supset J_0$ *of* $I$ *we have* $s_J \in s + V$.

If $G$ is written *multiplicatively*, and if we put $p_J = \prod_{i \in J} x_i$ for each finite subset $J$ of $I$, the family $(x_i)$ will be said to be *multipliable* if the mapping $J \to p_J$ has a limit with respect to the filter $\Phi$; this limit is called the *product* of the family $(x_i)$, and is denoted by $\prod_{i \in I} x_i$.

#### Remark 1 {#top-iii-s5-n1-rem-1 .statement}

When $I$ is *finite*, Definition 1 reduces to the ordinary definition of the sum of a finite family. More generally, if $I$ is arbitrary and $x_i = 0$ except when the index $i$ belongs to a *finite* subset $J$ of $I$, then the sum $\sum_{i \in I} x_i$ is equal to $\sum_{i \in J} x_i$.

#### Remark 2 {#top-iii-s5-n1-rem-2 .statement}

The definition of a summable family does not involve any *ordering* of the index set $I$, and we may therefore say that the notion of a sum thus defined is *commutative*. More precisely, we have the following property: let $(x_i)_{i \in I}$ be a summable family and let $\varphi$ be a bijective mapping of an index set $K$ onto the set $I$; then if we put $y_x = x_{\varphi(x)}$, the family $(y_x)_{x \in K}$ is summable and has the same sum as $(x_i)$. For if $s = \sum_{i \in I} x_i$, and if $\sum_{i \in J} x_i \in s + V$ for every finite subset $J$ containing the finite subset $J_0$, then we shall have $\sum_{x \in L} y_x \in s + V$ for every finite subset $L$ of $K$ containing $\overline{\varphi}(J_0)$.

#### Remark 3 {#top-iii-s5-n1-rem-3 .statement}

Definition 1 applies, more generally, to every family of points in a *Hausdorff topological space* $X$ on which has been defined an *associative and commutative law of composition*, written additively; for it does not make use of the axioms of topological groups.

### 2. CAUCHY'S CRITERION

Let $(x_i)_{i \in I}$ be a summable family in $G$. Then for each neighbourhood $V$ of the origin in $G$ there is a finite subset $J_0$ of $I$ such that, for each finite subset $ K $ of $ I $ *which does not meet* $ J_0 $, we have $ s_K \in V $. For $ J = J_0 \cup K $ is an arbitrary finite subset containing $ J_0 $; let $ s = \sum_{i \in J} x_i $ and let $ W $ be a symmetric neighbourhood of $ o $ such that $ W + W \subset V $; then, by Definition 1, we may choose $ J_0 $ such that $ s_J \in s + W $ and $ s_{J_0} \in S + W $, which means that $ s_K = s_J - s_{J_0} \in W + W \subset V $.

Conversely, suppose that the family $ (x_i) $ has this property. Then the image of the filter $ \Phi $, under the mapping $ J \to s_J $, is a *Cauchy filter base* in $ G $. For if $ J $ is a finite subset containing $ J_0 $, and if $ K $ denotes $ J \cap C J_0 $, then $ K \cap J_0 = \varnothing $ and $ s_K = s_J - s_{J_0} $, so that $ s_J \in s_{J_0} + V $. If $ J' $ is another finite subset containing $ J_0 $, then $ s_J - s_{J'} \in V + V $, and the result follows. Consequently:

#### Theorem 1 (Cauchy's criterion) {#top-iii-s5-thm-1 .statement}

*In a Hausdorff commutative group* $ G $, *in order that a family* $ (x_i)_{i \in I} $ *should be summable it is necessary that, for each neighbourhood* $ V $ *of the origin in* $ G $, *there is a finite subset* $ J_0 $ *of* $ I $ *such that* $ \sum_{i \in K} x_i \in V $ *for all finite subsets* $ K $ *of* $ I $ *which do not meet* $ J_0 $. *This necessary condition is also sufficient if* $ G $ *is complete*.

Thus by taking away a (sufficiently large) finite number of terms from the family $ (x_i) $, every *finite partial sum* of the surviving subfamily has to be as *close to* $ o $ *as we please*.

An immediate consequence of the first part of Theorem 1 is the following proposition:

#### Proposition 1 {#top-iii-s5-prop-1 .statement}

*If the family* $ (x_i) $ *is summable, then every neighbourhood of* $ o $ *contains all the* $ x_i $ *except for a finite subfamily* (in other words, if $ I $ is infinite, we have $ \lim x_i = o $ with respect to the *filter of complements of finite subsets of* $ I $).

This *necessary* condition for a family $ (x_i) $ to be summable is *by no means sufficient* in general, even if $ G $ is complete; we shall see many examples later (see Chapter IV, § 7).

#### Corollary {#top-iii-s5-n2-cor-1 .statement}

*Let* $ (x_i)_{i \in I} $ *be a summable family in a commutative group whose identity element has a countable fundamental system of neighbourhoods. Then the set of indices* $ i $ *such that* $ x_i \neq o $ *is countable*.

Let $ (V_n) $ be a countable fundamental system of neighbourhoods of $ o $. If $ H_n $ is the set of all indices $ i $ such that $ x_i \notin V_n $, then the set $ H $ of indices $ i $ such that $ x_i \neq o $ is the union of the sets $ H_n $, and each of the $ H_n $ is *finite* by Proposition 1.

#### Remark {#top-iii-s5-n2-rem-1 .statement}

When G is written multiplicatively, Cauchy’s criterion takes the following form : for the family $ (x_i)_{i \in I} $ to be multipliable it is necessary that, for each neighbourhood V of the identity element, there should exist a finite subset $ J_0 $ of I such that, for each finite subset K of I which does not meet $ J_0 $, we have $ \prod_{i \in K} x_i \in V $; and this condition is sufficient provided that G is complete. We deduce that if I is infinite and $ (x_i) $ is multipliable, then $ \lim x_i = 1 $ with respect to the filter of complements of finite subsets of I; if in addition the identity element has a countable fundamental system of neighbourhoods, then the set of indices i such that $ x_i \neq 1 $ is countable.

### 3. PARTIAL SUMS ; ASSOCIATIVITY

#### Proposition 2 {#top-iii-s5-prop-2 .statement}

In a complete group G, every subfamily of a summable family is summable.

For if Cauchy’s criterion is satisfied by a family $ (x_i)_{i \in I} $, then it is trivially satisfied by every subfamily.

If $ (x_i)_{i \in I} $ is summable, it follows therefore that the sum $ \sum_{i \in J} x_i $ is defined for every subset J of I, finite or not : it is again called the partial sum of the family $ (x_i) $, corresponding to the subset J of the index set. The set of partial sums of a summable family is evidently contained in the closure of the set of finite partial sums.

#### Theorem 2 (Associativity of the sum) {#top-iii-s5-thm-2 .statement}

Let $ (x_i)_{i \in I} $ be a summable family in a complete group G, and let $ (I_\lambda)_{\lambda \in L} $ be any partition of I. If $ s_\lambda $ denotes $ \sum_{i \in I_\lambda} x_i $, then the family $ (s_\lambda)_{\lambda \in L} $ is summable and has the same sum as the family $ (x_i)_{i \in I} $.

Thus if we have a summable family in a complete group, we can associate its terms arbitrarily into subfamilies and form the sum of each subfamily thus obtained; the family of these partial sums is again summable and its sum is equal to that of the given family.

Let $ s = \sum_{i \in I} x_i $, and let $ V $ be any *closed* neighbourhood of 0 in $ G $. Then there is a finite subset $ J_0 $ of $ I $ such that, for each finite subset $ J $ of $ I $ which contains $ J_0 $, we have $ \sum_{i \in J} x_i \in s + V $. Let $ K_0 $ be the subset of $ L $ consisting of indices $ \lambda $ such that $ J_\lambda = I_\lambda \cap J_0 $ is *not empty*: $ K_0 $ is clearly finite. Let $ K $ be any finite subset of $ L $ which contains $ K_0 $; we shall show that $ \sum_{\lambda \in K} s_\lambda \in s + V $, which will establish the theorem.

Now $ s_\lambda $ is very close to a finite partial sum of $ (x_i) $, whose indices all belong to $ I_\lambda $; more precisely, given any symmetric neighbourhood $ W $ of 0, there exists for each $ \lambda \in K $ a finite subset $ H_\lambda $ of $ I_\lambda $, *containing* $ J_\lambda $ and such that $ s_\lambda - \sum_{i \in H_\lambda} x_i \in W $. Let $ J = \sum_{\lambda \in K} H_\lambda $; then $ J $ is a finite subset of $ I $ containing $ J_0 $, and we have

$$
\sum_{i \in J} x_i = \sum_{i \in \bigcup_{\lambda \in K} H_\lambda} x_i = \sum_{\lambda \in K} (\sum_{i \in H_\lambda} x_i)
$$

by the associativity of finite sums. Hence by reason of the choice of $ J_0 $ and the $ H_\lambda $, we have

$$
\sum_{\lambda \in K} s_\lambda \in s + V + nW
$$

where $ n $ is the number of elements in $ K $; this relation holds for each $ W $, hence also $ \sum_{\lambda \in K} s_\lambda \in s + V $, since $ V $ (being closed) is the intersection of the neighbourhoods $ V + nW $ [§ 3, no. 1, formula (1)].

We can thus write the *associativity formula* for sums:

(I)

$$
\sum_{\lambda \in L} (\sum_{i \in I_\lambda} x_i) = \sum_{i \in \bigcup_{\lambda \in L} I_\lambda} x_i,
$$

which is valid whenever the family $ (I_\lambda) $ is a *partition* of its union and the right-hand side is defined. In particular, if the index set is a *product* $ I = L \times M $, and if the "double" family $ (x_{\lambda \mu})_{(\lambda, \mu) \in L \times M} $ is *summable*, we have the *formula of change of order of summation*

(2)

$$
\sum_{(\lambda, \mu) \in L \times M} x_{\lambda \mu} = \sum_{\lambda \in L} (\sum_{\mu \in M} x_{\lambda \mu}) = \sum_{\mu \in M} (\sum_{\lambda \in L} x_{\lambda \mu}).
$$

It should be remarked that the *left-hand side* of (1) can have a meaning, without the right-hand side being defined. Consider for example the case where $ I = LX \{1, 2\} $ and $ L $ is infinite, and $ I_\lambda $ consists of the two elements $ (\lambda, 1) $ and $ (\lambda, 2) $; if we take $ x_{\lambda, 1} = a,\ x_{\lambda, 2} = -a $, where $ a $ is any non-zero element of $ G $, then all the partial sums corresponding to the $ I_\lambda $ are zero, and therefore the left-hand side of (1) is defined and equal to 0, whereas the right-hand side of (1) has no meaning, as Proposition 1 shows.

Likewise, it can happen that the left-hand side of (2) is not defined but that each of the two "double sums" in (2) has a meaning; and the elements of $ G $ which they represent need not be equal (see Chapter IV, § 7, Exercise 17).

Thus although it is always possible to "associate" the terms of a sum, it is not possible, on the other hand, to "dissociate" into their elements those terms of a sum which appear themselves as sums. Nevertheless, this operation is legitimate whenever the number of these "dissociable" terms is finite.

#### Proposition 3 {#top-iii-s5-prop-3 .statement}

Let $ (x_i)_{i \in I} $ be a family of points of a group $ G $, and let $ (I_\lambda)_{\lambda \in L} $ be a finite partition of $ I $. If each of the subfamilies $ (x_i)_{i \in I_\lambda} $ is summable, then the family $ (x_i)_{i \in I} $ is summable and the formula (1) is valid.

It is enough to prove the proposition when $ L = (1,2) $; having done so, we then proceed by induction on the number of elements of $ L $. Let $ s_1 = \sum_{i \in I_1} x_i $ and $ s_2 = \sum_{i \in I_2} x_i $. For each neighbourhood $ V $ of the origin, there is a finite subset $ J_1 $ (resp. $ J_2 $) of $ I_1 $ (resp. $ I_2 $) such that, for each finite subset $ H_1 $ (resp. $ H_2 $) of $ I_1 $ (resp. $ I_2 $) containing $ J_1 $ (resp. $ J_2 $), we have $ \sum_{i \in H_1} x_i \in S_1 + V $ (resp. $ \sum_{i \in H_2} x_i \in s_2 + V $). If we put $ J_0 = J_1 \cup J_2 $, it follows that, for each finite subset $ H $ of $ I $ which contains $ J_0 $, we have $ \sum_{i \in H} x_i \in S_1 + s_2 + V + V $, and the result follows.

### 4. SUMMABLE FAMILIES IN A PRODUCT OF GROUPS

#### Proposition 4 {#top-iii-s5-prop-4 .statement}

Let $ G = \prod_{\lambda \in L} G_\lambda $ be the product of a family of Hausdorff commutative groups. Then a family $ (x_i)_{i \in I} $ of points of $ G $ is summable if and only if, for each $ \lambda \in L $, the family $ (\mathrm{pr}_\lambda x_i)_{i \in I} $ is summable; and if $ s_\lambda $ is the sum of this family, then $ s = (s_\lambda) $ is the sum of the family $ (x_i) $.

This follows immediately from the condition for convergence, with respect to a filter, of a function which takes its values in a product space (Chapter I, § 1, no. 6, Corollary 1 to Proposition 10); in effect, for each finite subset $ J $ of $ I $, we have

$$
\mathrm{pr}_\lambda \left( \sum_{i \in J} x_i \right) = \sum_{i \in J} \mathrm{pr}_\lambda x_i.
$$

### 5. IMAGE OF A SUMMABLE FAMILY UNDER A CONTINUOUS HOMOMORPHISM

#### Proposition 5 {#top-iii-s5-prop-5 .statement}

Let $ f $ be a continuous homomorphism of a commutative group $ G $ into a commutative group $ G' $. If $ (x_i) $ is a summable family in $ G $, then $ (f(x_i)) $ is a summable family in $ G' $, and we have

$$
\Sigma f(x_i) = f(\Sigma x_i).
$$

If $ J $ is any finite subset of the index set, then $ f \left( \sum_{i \in J} x_i \right) = \sum_{i \in J} f(x_i) $, and the image under $ f $ of a convergent filter base is a convergent filter base (Chapter I, § 7, no. 4, Corollary 1 to Proposition 9).

#### Proposition 6 {#top-iii-s5-prop-6 .statement}

Let $ (x_i), (y_i) $ be two summable families, with the same index set, in a group $ G $. Then the families $ (-x_i), (nx_i) $ ($ n \in \mathbf{Z} $), $ (x_i + y_i) $ are summable, and we have

$$
\begin{align*}
\Sigma(-x_i) &= -\Sigma x_i, \\
\Sigma(nx_i) &= n\Sigma x_i, \\
\Sigma(x_i + y_i) &= \Sigma x_i + \Sigma y_i.
\end{align*}
$$

For $ x \to -x $ and $ x \to nx $ are continuous homomorphisms of $ G $ into $ G $; on the other hand, if $ (x_i) $ and $ (y_i) $ are summable, then the family $ (x_i, y_i) $ is summable in $ G \times G $, and since $ (x, y) \to x + y $ is a continuous homomorphism of $ G \times G $ into $ G $, we deduce (6).

#### Remark {#top-iii-s5-n5-rem-1 .statement}

Propositions 4 and 5 again apply to the case, mentioned earlier, of summable families in a topological space $ X $ which has an associative and commutative law of composition; the same holds for Proposition 3 and formula (6) if we suppose in addition that $ x + y $ is continuous on $ X \times X $.

### 6. SERIES

Consider a sequence of points $ (x_n)_{n \in \mathbf{N}} $ in a Hausdorff commutative group, and form the sequence of *partial sums* $ s_n = \sum_{p=0}^n x_p $ ($ n \in \mathbf{N} $). The mapping $ (x_n) \to (s_n) $ is a *bijection* of the set $ G^\mathbf{N} $ of sequences $ (x_n) $ of points of $ G $, onto itself; for if the sequence $ (s_n) $ is given, the sequence $ (x_n) $ is determined by the relations $ x_0 = s_0, x_n = s_n - s_{n-1} $ ($ n \geq 1 $).

The *series defined by the sequence* $ (x_n) $, or the *series whose general term* is $ x_n $ [or simply the *series* $ (x_n) $], by abuse of language, if there is no risk of confusion] is defined to be the *pair* of sequences $ (x_n) $ and $ (s_n) $ thus associated. The series defined by the sequence $ (x_n) $ is said to be *convergent* if the sequence $ (s_n) $ is convergent; the limit of this sequence is called *the sum of the series* and is written $ \sum_{n=0}^\infty x_n $ (or $ \sum_{n=0}^\infty x_n $, by abuse of notation).

If the series whose general term is $ x_n $ is *convergent*, we shall sometimes allow ourselves, by abuse of language, to refer to it as "the series $ \sum_{n=0}^\infty x_n $" or "the series $ x_0 + x_1 + \cdots + x_n + \cdots $".

A *necessary* condition for the convergence of the series whose general term is $ x_n $ is that the sequence $ (s_n) $ should be a *Cauchy sequence*, that is to say, that for each neighbourhood $ V $ of the origin in $ G $ there is an integer $ n_0 $ such that for each pair of integers $ n \geq n_0,\ p > 0 $, we have
$$
s_{n+p} - s_n = \sum_{i=n+1}^{n+p} x_i \in V.
$$
If $ G $ is *complete*, this condition is also *sufficient* (*Cauchy's criterion for series*).

If the series whose general term is $ x_n $ is convergent, we have in particular $ \lim_{n \to \infty} (s_n - s_{n-1}) = \lim_{n \to \infty} x_n = 0 $; but this *necessary* condition for convergence is by no means sufficient in general, even if $ G $ is complete (see Chapter IV, § 7).

#### Proposition 7 {#top-iii-s5-prop-7 .statement}

*If the series defined by the sequences* $ (x_n) $ *and* $ (y_n) $ *are convergent, then so are the series defined by the sequences* $ (-x_n) $ *and* $ (x_n + y_n) $, *and we have*
(7)
$$
\sum_{n=0}^\infty (-x_n) = -\sum_{n=0}^\infty x_n,
$$
(8)
$$
\sum_{n=0}^\infty (x_n + y_n) = \sum_{n=0}^\infty x_n + \sum_{n=0}^\infty y_n.
$$
This is an obvious consequence of the continuity of $ -x $ on $ G $, and of $ x + y $ on $ G \times G $.

#### Corollary {#top-iii-s5-n6-cor-1 .statement}

*If* $ (x_n), (y_n) $ *are two sequences of points of* $ G $ *such that* $ x_n = y_n $ *except for a finite number of indices, and if the series whose general term is* $ x_n $ *converges, then so does the series whose general term is* $ y_n $.

For the series whose general term is $ x_n - y_n $ has all its terms zero from a certain index onwards.

This corollary may be put in the form that *we may alter arbitrarily a finite number of terms of a convergent series without it ceasing to be convergent*.
In particular, if $ y_n = 0 $ for $ n < m $, and $ y_n = x_n $ for $ n \geq m $, we see that the series whose general term is $ y_n $ converges if and only if the series whose general term is $ x_n $ converges; its sum is denoted by $ \sum_{n=m}^{\infty} x_n $ and is called the *residue* of index $ m $ of the series $ (x_n) $. Since
$$
\sum_{n=m}^{\infty} x_n = \sum_{n=0}^{\infty} x_n - s_{m-1},
$$
the residue of index $ m $ of a convergent series *tends to* 0 as $ m $ tends to $ +\infty $.

If a sequence $ (x_n)_{n \in I} $ has as index set an infinite subset $ I $ of $ \mathbf{N} $, and if $ \varphi $ denotes the *strictly order-preserving* bijection of $ \mathbf{N} $ onto $ I $, then the series defined by the sequence $ (x_{\varphi(n)})_{n \in \mathbf{N}} $ is called, by abuse of language, the *series* defined by the sequence $ (x_n)_{n \in I} $; if this series is convergent, its sum is denoted by $ \sum_{n \in I}^{\infty} x_n $. It is immediately verified that this series converges if and only if the series whose general term is $ (z_n) $ converges, where $ z_n = x_n $ if $ n \in I $ and $ z_n = 0 $ if $ n \in \mathbf{C} I $.

It is important to notice that if the series defined by a sequence $ (x_n)_{n \in \mathbf{N}} $ converges, there can exist infinite subsets $ I $ of $ \mathbf{N} $ such that the series defined by the subsequence $ (x_n)_{n \in I} $ *does not converge* (see Exercise 5 and Chapter IV, § 7).

Propositions 4 and 5 extend immediately to series, and we leave their formulation in this case to the reader.

**Proposition 8 (Restricted associativity of series).** *Let* $ (k_n) $ *be a strictly increasing sequence of integers* $ \geqslant 0 $. *If the series whose general term is* $ x_n $ *converges, and if we put* $ u_n = \sum_{p=k_{n-1}}^{k_n-1} x_p $, *then the series whose general term is* $ u_n $ *is convergent, and we have* $ \sum_{n=0}^{\infty} u_n = \sum_{n=0}^{\infty} x_n $.

For the sequence of partial sums of the series $ (u_n) $ is a *subsequence* $ (s_{k_n-1}) $ of the sequence $ (s_n) $ of partial sums of the series $ (x_n) $.

### 7. COMMUTATIVELY CONVERGENT SERIES

Let $ (x_n) $ be a *summable* sequence in $ G $, and let $ s = \sum_{n \in \mathbf{N}} x_n $ be its sum. Then for each neighbourhood $ V $ of 0, there exists $ J_0 \in \mathcal{F}(\mathbf{N}) $ such that $ s_J \in s + V $ whenever $ J \in \mathcal{F}(\mathbf{N}) $ and $ J_0 \subset J $. Let $ m $ be the largest integer in $ J_0 $; then if $ n \geqslant m $ we have $ s_n \in s + V $, and therefore the *series* $ (x_n) $ is convergent and its sum is $ s $. But the converse is *false*:

Moreover, the definition of a convergent series essentially involves the order structure of $ \mathbf{N} $. If the series $ (x_n) $ is convergent, and if $ \sigma $ is a permutation of $ \mathbf{N} $, then the series $ (x_{\sigma(n)}) $ is not necessarily convergent (cf. Chapter IV, § 7, Exercise 15).

#### Definition 2 {#top-iii-s5-def-2 .statement}

*A series defined by a sequence* $ (x_n) $ *is said to be commutatively convergent if, for each permutation* $ \sigma $ *of* $ \mathbf{N} $, *the series defined by the sequence* $ (x_{\varphi(n)}) $ *is convergent.*

#### Proposition 9 {#top-iii-s5-prop-9 .statement}

*The series defined by the sequence* $ (x_n) $ *is commutatively convergent if and only if the sequence* $ (x_n) $ *is summable; and then, for each permutation* $ \sigma $ *of* $ \mathbf{N} $, *we have*

$$
\sum_{n=0}^{\infty} x_{\sigma} = \sum_{n \in \mathbf{N}} x_n.
$$

If the sequence is summable, then clearly the series is commutatively convergent. To prove the reverse implication we shall argue by *reductio ad absurdum* and suppose that the series $ (x_n) $ is commutatively convergent but that the sequence $ (x_n) $ is not summable. The image of the filter $ \Phi $ under the mapping $ H \to s_H $ therefore cannot be a Cauchy filter base in $ G $, otherwise this filter base would converge, since by hypothesis it has a cluster point (Chapter II, § 3, no. 2, Proposition 5, Corollary 2). Hence there is a neighbourhood $ V $ of 0 in $ G $ such that, for each finite subset $ J $ of $ \mathbf{N} $, there is a finite subset $ H $ of $ \mathbf{N} $ which does not meet $ J $ and is such that $ \sum_{n \in H} x_n \notin V $. Hence, by induction, we can define a partition of $ \mathbf{N} $ into *finite* subsets $ H_k $ ($ k \in \mathbf{N} $) such that $ \sum_{n \in H_k} x_n \notin V $ for an infinite number of indices $ k $. Clearly there is a permutation $ \sigma $ of $ \mathbf{N} $ such that for each $ k $, the values of $ n $ for which $ \sigma(n) \in H_k $ are consecutive. If $ \sigma $ is such a permutation, then the series whose general term is $ x_{\sigma(n)} $ cannot be convergent, and we have a contradiction.

If the group $ G $ is written *multiplicatively*, the *infinite product defined by a sequence* $ (x_n) $ of points of $ G $ (or *infinite product whose general term is* $ x_n $, or even *product* $ x_n $ if there is no possibility of confusion) is defined to be the pair formed by the sequence $ (x_n) $ and the sequence of partial products

$$
p_n = \prod_{k=0}^{n} x_k.
$$

The infinite product is said to *converge* if the sequence $ (p_n) $ converges, and the limit of this sequence is denoted by $ \prod_{n=0}^{\infty} x_n $ (or $ \prod_{n=0}^{\infty} x_n $ by abuse of notation). We leave to the reader the task of transcribing into multiplicative notation the properties of series which we have established.

### Exercises {#top-iii-s5-exercises}

See the [exercises for § 5](exercises/s5/).
