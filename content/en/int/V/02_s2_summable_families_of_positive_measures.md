---
book: int
book_title: Integration
chapter: V
chapter_title: INTEGRATION OF MEASURES
section: 2
section_title: Summable families of positive measures
lang: en
source: int-i-vi
book_pages: INT V.95-INT V.96
pdf_pages: 0266-0270, 0350-0351
extraction: ocr
subsections:
    - "no": 1
      title: Definition of summable families of measures
      page: 11
      pdf_page: 266
    - "no": 2
      title: Integration with respect to a sum of positive measures
      page: 12
      pdf_page: 267
    - "no": 3
      title: Decomposition of a measure as a sum of measures with compact support
      page: 14
      pdf_page: 269
statements: 12
exercises: 4
content_sha256: 290c436e1eb1835d7f3151eac47140087383fdc5ddbccba20fa7ed077333c707
---

## § 2. SUMMABLE FAMILIES OF POSITIVE MEASURES

### 1. Definition of summable families of measures

Let $(\lambda_\alpha)_{\alpha \in A}$ be a family of positive measures on a locally compact space X; the family $(\lambda_\alpha)_{\alpha \in A}$ is said to be a *summable family of measures* if it is summable in the vector space $\mathcal{M}(X)$ of real measures on X, equipped with the vague topology (GT, III, §5, No. 1). This amounts to saying that for every function $f \in \mathcal{K}(X)$, the family of numbers $\lambda_\alpha(f)$ is summable in $\mathbf{R}$. For, this condition is obviously necessary; conversely, if it is satisfied then the linear form $f \mapsto \sum_{\alpha \in A} \lambda_\alpha(f)$ on $\mathcal{K}(X)$ is positive, hence is a positive measure $\nu$ (Ch. III, §1, No. 5, Th. 1), and one verifies immediately that the finite partial sums of the family $(\lambda_\alpha)$ converge vaguely to $\nu$, with respect to the section filter of the set of finite subsets of A (GT, III, §5, No. 1, Def. 1).

Since every element of $\mathcal{K}(X)$ is the difference of two elements of $\mathcal{K}_+(X)$, the family $(\lambda_\alpha)$ is summable if and only if
$$
\sum_{\alpha \in A} \lambda_\alpha(f) < +\infty
$$

for every function $f \in \mathcal{K}_+(X)$. This condition is also equivalent to the following:

(2)
$$
\sum_{\alpha \in A} \lambda_\alpha(K) < +\infty
$$
for every compact set $K \subset X$.

For, (2) implies (1) because $f \leq \|f\| \cdot \varphi_S$, where S denotes the compact support of $f$. Conversely, if K is a compact set, there exists a function $f \in \mathcal{K}_+(X)$ such that $\varphi_K \leq f$ (Ch. III, §1, No. 2, Lemma 1), and it follows that (1) implies (2).

#### Remark 1 {#int-v-s2-n1-rem-1 .statement}

It is immediate that, when the family $(\lambda_\alpha)_{\alpha \in A}$ is summable, its sum is the supremum in $\mathcal{M}_+(X)$ of the finite partial sums $\sum_{\alpha \in J} \lambda_\alpha$, where J runs over the set of finite subsets of A.

#### Remark 2 {#int-v-s2-n1-rem-2 .statement}

Let $(\theta_\alpha)_{\alpha \in A}$ be a family of complex measures on X; the family $(\theta_\alpha)$ is said to be *summable* if the family $(|\theta_\alpha|)$ of positive measures is summable; *it is not sufficient for this* that the family $(\theta_\alpha)$ be summable in the vector space $\mathcal{M}(X; \mathbf{C})$ equipped with the vague topology (cf. Exer. 3).

### 2. Integration with respect to a sum of positive measures

*Throughout this No.*, X denotes a locally compact space, $(\lambda_\alpha)_{\alpha \in A}$ a summable family of positive measures on X, and $\nu$ the measure $\sum_{\alpha \in A} \lambda_\alpha$.

#### Proposition 1 {#int-v-s2-prop-1 .statement}

— *Let f be a positive numerical function defined on X. Then*
$$
\nu^\bullet(f) = \sum_{\alpha \in A} \lambda_\alpha^\bullet(f).
$$

This follows at once from Remark 1, Prop. 11 of §1, No. 3 and Prop. 3 of §1, No. 1.

#### Corollary 1 {#int-v-s2-prop-1-cor-1 .statement}

— *For every compact (resp. open and relatively compact) subset M of X,
$$
\nu(M) = \sum_{\alpha \in A} \lambda_\alpha(M).
$$*

#### Corollary 2 {#int-v-s2-prop-1-cor-2 .statement}

— *For a subset N of X to be locally $\nu$-negligible, it is necessary and sufficient that, for every $\alpha \in A$, N be locally $\lambda_\alpha$-negligible.*

#### Corollary 3 {#int-v-s2-prop-1-cor-3 .statement}

— *For every function $f \in \mathcal{F}_+(X)$,
$$
\nu^*(f) \geq \sum_{\alpha \in A} \lambda_\alpha^*(f).
$$*

The inequality is obvious if $f$ is not $\nu$-moderated, because then $\nu^*(f) = +\infty$ ($\S 1$, No. 2, Prop. 7). If $f$ is $\nu$-moderated then $f$ is $\lambda_\alpha$-moderated for every $\alpha \in A$, because every $\nu$-integrable open set is $\lambda_\alpha$-integrable; the relation (4) then follows at once from (3) and from Prop. 7 of $\S 1$, No. 2.

It can happen that the two members of (4) are not equal, even when $A$ is countable and each of the $\lambda_\alpha$ is a point measure ($\S 1$, Exer. 4 a)).

#### Proposition 2 {#int-v-s2-prop-2 .statement}

— *Let $f$ be a mapping of $X$ into a topological space $G$. For $f$ to be $\nu$-measurable, it is necessary and sufficient that $f$ be $\lambda_\alpha$-measurable for every $\alpha \in A$.*

This follows at once from Cor. 2 of Prop. 11 of $\S 1$.

#### Proposition 3 {#int-v-s2-prop-3 .statement}

— *For a mapping $f$ of $X$ into a Banach space $F$ to be essentially $\nu$-integrable, it is necessary and sufficient that $f$ be essentially $\lambda_\alpha$-integrable for every $\alpha \in A$ and that*

$$
\sum_{\alpha \in A} \int^\bullet |f| \, d\lambda_\alpha < +\infty .
$$

*The family $(\int f \, d\lambda_\alpha)_{\alpha \in A}$ is then absolutely summable in $F$, and*

$$
\int f \, d\nu = \sum_{\alpha \in A} \int f \, d\lambda_\alpha .
$$

Indeed, for $f$ to be essentially $\nu$-integrable (resp. essentially $\lambda_\alpha$-integrable), it is necessary and sufficient that $f$ be measurable for the measure $\nu$ (resp. $\lambda_\alpha$) and that $\nu^\bullet(|f|) < +\infty$ (resp. $\lambda_\alpha^\bullet(|f|) < +\infty$), by virtue of Prop. 9 of $\S 1$, No. 3. The first part of the statement therefore follows at once from Props. 2 and 1. If $f$ is essentially $\nu$-integrable, the inequality

$$
\sum_{\alpha \in A} \left| \int f \, d\lambda_\alpha \right| \leq \sum_{\alpha \in A} \int |f| \, d\lambda_\alpha = \nu(|f|)
$$

implies that the family $(\int f \, d\lambda_\alpha)$ is absolutely summable in $F$, and that the norm of the sum is less than or equal to the norm of $f$ in $\mathcal{L}_F^1(\nu)$. The set of $f \in \mathcal{L}_F^1(\nu)$ that satisfy (6) is thus a closed linear subspace $\mathcal{H}$ of $\mathcal{L}_F^1(\nu)$; now, this subspace is also dense in $\mathcal{L}_F^1(\nu)$, because it contains the functions of the form $f \cdot a$, where $a \in F$ and $f$ denotes a finite integrable positive function (Prop. 1). Therefore $\mathcal{H} = \mathcal{L}_F^1(\nu)$ and the proposition is established.

Prop. 3 can also be deduced from the general theorem on integration that will be proved in §3 (No. 3, Th. 1).

#### Corollary 1 {#int-v-s2-prop-3-cor-1 .statement}

— Suppose that $f$ is $\nu$-integrable; then $f$ is $\lambda_\alpha$-integrable for every $\alpha \in A$, and formula (6) holds. Conversely, if the set $A$ is finite and $f$ is $\lambda_\alpha$-integrable for every $\alpha \in A$, then the function $f$ is $\nu$-integrable.

If $f$ is $\nu$-integrable, then $f$ is essentially $\nu$-integrable and $\nu$-moderated (\S1, No. 3, Cor. of Prop. 9); $f$ is therefore essentially $\lambda_\alpha$-integrable and $\lambda_\alpha$-moderated, hence $\lambda_\alpha$-integrable, for every $\alpha \in A$. Conversely, if $A$ is finite and if $f$ is $\lambda_\alpha$-integrable for all $\alpha \in A$, then $f$ is essentially $\nu$-integrable by Prop. 3, and it suffices to verify that $\nu^*(|f|) < +\infty$; this follows at once from the relation $\nu^* = \sum_{\alpha \in A} \lambda_\alpha^*$ (Ch. IV, §1, No. 3, Prop. 15).

#### Corollary 2 {#int-v-s2-prop-3-cor-2 .statement}

— Let $\theta$ be a complex measure on $X$; set $\theta_1 = (\Re \theta)^+$, $\theta_2 = (\Re \theta)^-$, $\theta_3 = (\Im \theta)^+$, $\theta_4 = (\Im \theta)^-$. In order that a mapping $f$ of $X$ into a topological space $G$ (resp. into a Banach space $F$) be measurable (resp. essentially integrable, integrable) for the measure $\theta$, it is necessary and sufficient that it be measurable (resp. essentially integrable, integrable) for each of the measures $\theta_i$ ($i = 1, 2, 3, 4$).

If $f$ is measurable (resp. essentially integrable, integrable) for $\theta$, then $f$ is by definition measurable (resp. essentially integrable, integrable) for the measure $|\theta|$, hence also for the measures $\theta_i$, which are $\leq |\theta|$. Conversely, if $f$ is measurable (resp. essentially integrable, integrable) for the measures $\theta_i$, then Prop. 2 (resp. Prop. 3, Cor. 1 of Prop. 3) implies that $f$ is measurable (resp. essentially integrable, integrable) for the measure $\theta_1 + \theta_2 + \theta_3 + \theta_4$, which is $\geq |\theta|$.

### 3. Decomposition of a measure as a sum of measures with compact support

#### Proposition 4 {#int-v-s2-prop-4 .statement}

— Let $\mu$ be a positive measure on a locally compact space $T$, and let $\mathfrak{K}$ be a $\mu$-dense set of compact subsets of $T$. There exists a summable family $(\mu_\alpha)_{\alpha \in A}$ of positive measures on $T$ such that $\mu = \sum_{\alpha \in A} \mu_\alpha$, and such that the supports of the measures $\mu_\alpha$ belong to $\mathfrak{K}$ and form a locally countable family of pairwise disjoint compact sets.

If the measure $\mu$ is moderated, the index set $A$ may be taken to be countable.

Consider a locally countable family $(K_\alpha)_{\alpha \in A}$ of pairwise disjoint elements of $\mathfrak{K}$ such that the set $N = T - \bigcup_{\alpha \in A} K_\alpha$ is locally $\mu$-negligible

(Ch. IV, §5, No. 9, Prop. 14). For every function $f \in \mathcal{K}(T)$, set
$$
\mu_\alpha(f) = \mu(f \varphi_{K_\alpha});
$$
the linear form $\mu_\alpha$ on $\mathcal{K}(T)$ is positive, therefore is a positive measure, with support contained in $K_\alpha$. Since every compact set contained in an element of $\mathfrak{K}$ belongs to $\mathfrak{K}$, $\operatorname{Supp}(\mu_\alpha) \in \mathfrak{K}$ for all $\alpha \in A$. It remains only to show that the family $(\mu_\alpha)$ is summable and that its sum is equal to $\mu$, in other words that $\sum_{\alpha \in A} \mu_\alpha(f) = \mu(f)$ for every function $f \in \mathcal{K}_+(T)$.

Now, let $S$ be the (compact) support of $f$, and let $A'$ be the countable set formed by the $\alpha \in A$ such that $S \cap K_\alpha \neq \varnothing$. Since the set $N \cap S$ is $\mu$-negligible,
$$
\begin{align*}
\mu(f) &= \mu(f \varphi_S) = \sum_{\alpha \in A'} \mu(f \varphi_{S \cap K_\alpha}) = \sum_{\alpha \in A'} \mu(f \varphi_{K_\alpha}) \\
&= \sum_{\alpha \in A} \mu(f \varphi_{K_\alpha}) = \sum_{\alpha \in A} \mu_\alpha(f).
\end{align*}
$$
This completes the proof of the general case. If $\mu$ is moderated, then the set $T$ is $\mu$-moderated and so $T$ is the union of a sequence $(L_n)$ of compact sets and a negligible set (\S 1, No. 2, Prop. 5); let $A'$ be the countable set of $\alpha \in A$ such that $K_\alpha$ intersects one of the $L_n$. Then $\mu_\alpha = 0$ for $\alpha \notin A'$, and the last sentence of the statement follows immediately.

#### Remark {#int-v-s2-n3-rem-1 .statement}

A positive measure may be the sum of a sequence of measures with compact support, and not be moderated (see Exer. 4 a) of \S 1).

### Exercises {#int-v-s2-exercises}

See the [exercises for § 2](exercises/s2/).
