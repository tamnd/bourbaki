---
book: top
book_title: General Topology
chapter: IX
chapter_title: Use of real numbers in general topology
section: 1
section_title: Generation of a uniformity by a family of pseudometrics; uniformizable spaces
lang: en
source: top-v-x
pdf_pages: 0143-0153, 0224-0232
extraction: ocr
subsections:
    - "no": 1
      title: PSEUDOMETRICS
      page: 0
      pdf_page: 143
    - "no": 2
      title: DEFINITION OF A UNIFORMITY BY MEANS OF A FAMILY OF PSEUDOMETRICS
      page: 0
      pdf_page: 144
    - "no": 3
      title: PROPERTIES OF UNIFORMITIES DEFINED BY FAMILIES OF PSEUDOMETRICS
      page: 0
      pdf_page: 147
    - "no": 4
      title: CONSTRUCTION OF A FAMILY OF PSEUDOMETRICS DEFINING A UNIFORMITY
      page: 0
      pdf_page: 148
    - "no": 5
      title: UNIFORMIZABLE SPACES
      page: 0
      pdf_page: 150
    - "no": 6
      title: SEMI-CONTINUOUS FUNCTIONS ON A UNIFORMIZABLE SPACE
      page: 0
      pdf_page: 152
statements: 15
exercises: 22
content_sha256: d46241dcc6e0b3fdc75ac577e2626154c33e198b02447a07198d181994f0f47a
---

## 1. GENERATION OF A UNIFORMITY BY A FAMILY OF PSEUDOMETRICS; UNIFORMIZABLE SPACES

### 1. PSEUDOMETRICS

Definition I. *If X is a set, a pseudometric on X is any mapping f of X × X into the interval [0, +∞] of the extended real line $\overline{\mathbf{R}}$ which satisfies the following conditions:

(EC_I) *For all $x \in X, f(x, x) = 0$.
(EC_{II}) *For all $x \in X$ and all $y \in X, f(x, y) = f(y, x)$ (symmetry).
(EC_{III}) *For all $x, y, z$ in X,
$$
f(x, y) \leq f(x, z) + f(z, y)
$$
(triangle inequality).

#### Example 1 {#top-ix-s1-n1-exa-1 .statement}

On real number space $\mathbf{R}^n$, Euclidean distance (Chapter VI, § 2, no. 1) is a pseudometric.
2) If X is any set, the function f defined on $X \times X$ by the conditions $f(x, x) = 0$ for all $x \in X, f(x, y) = +\infty$ if $x \neq y$ is a pseudometric on X.
3) If X is any set and if g is any finite real-valued function defined on X, then the function f defined on $X \times X$ by $f(x, y) = |g(x) - g(y)|$ is a pseudometric on X.
\* 4) Let X be the set of all continuous mappings of the interval [0, 1] of $\mathbf{R}$ into $\mathbf{R}$. If for each pair of elements $x, y$ of X we put
$$
f(x, y) = \int_0^1 |x(t) - y(t)| \, dt,
$$
then f is a pseudometric on X. \*

Remarks:
1) Example 2 above shows that a pseudometric can take the value $+\infty$ for certain pairs of elements of $X$.
2) If $f$ is a pseudometric on $X$, we can in general have $f(x, y) = 0$ without $x = y$, as Example 3 above shows (cf. § 2).

From the triangle inequality it follows that if $f(x, z)$ and $f(y, z)$ are finite then so is $f(x, y)$; moreover, in this case we have
$$
f(x, z) \leq f(y, z) + f(x, y) \quad \text{and} \quad f(y, z) \leq f(x, z) + f(x, y),
$$
so that
(I)
$$
|f(x, z) - f(y, z)| \leq f(x, y).
$$

If $f$ is a pseudometric on $X$, then so is $kf$ for any finite real number $k > 0$. If $\{f_i\}_{i \in I}$ is any family of pseudometrics on $X$, the sum $\sum_{i \in I} f_i$ is defined for all $x, y \in X \setminus X$; if $f$ denotes the value of this sum, then $f$ is a pseudometric on $X$. Again, the supremum of the family $\{f_i\}$ (Chapter IV, § 5, no. 5) is a pseudometric on $X$, for the relations $f_i(x, y) \leq f_i(x, z) + f_i(z, y)$ imply
$$
\sup_{i \in I} f_i(x, y) \leq \sup_{i \in I} (f_i(x, z) + f_i(z, y)) \leq \sup_{i \in I} f_i(x, z) + \sup_{i \in I} f_i(z, y)
$$
[Chapter IV, § 5, no. 7, formula (17)].

### 2. DEFINITION OF A UNIFORMITY BY MEANS OF A FAMILY OF PSEUDOMETRICS

We have seen in Chapter VI, § 2, no. 3 that if, for each real number $s > 0$, we denote by $U_s$ the set of all pairs $(x, y)$ of points of $\mathbf{R}^n$ whose Euclidean distance apart is $\leq s$, then the $U_s$ form a fundamental system of entourages of the uniformity of $\mathbf{R}^n$ as $s$ runs through the set of real numbers $> 0$.

More generally, let $f$ be a pseudometric on a set $X$: for each $s > 0$, let $U_s$ denote $f^{-1}([0, s])$, and let us show that, as $s$ runs through the set of all real numbers $> 0$, the $U_s$ form a fundamental system of a uniformity on $X$. Axiom $U_1$ is satisfied by reason of $\mathrm{(EC_1)}$: if $s = t$, we have $U_s \subset U_t$ and therefore the $U_s$ satisfy $B_1$: by $\mathrm{(EC_{11})}$, we have $U_s \cup U_s$ and therefore $U_{2s}$ is satisfied; finally, by $\mathrm{(EC_{111})}$, we have $U_s = U_{2s}$, so that $U_{2s}$ is satisfied. (Cf. Chapter II, § 1, no. 1, Definition 2). Consequently we may make the following definition:

#### Definition 2 {#top-ix-s1-def-2 .statement}

Given a pseudometric $f$ on a set $X$, the uniformity defined by $f$ is the uniformity on $X$ which has as a fundamental system of entourages the family of sets $\overline{f}^{-1}([0, a])$, where $a$ runs through the set of all real numbers $> 0$.

Two pseudometrics on $X$ are said to be equivalent if they define the same uniformity.

#### Remark 1 {#top-ix-s1-n2-rem-1 .statement}

If $(a_n)$ is any sequence of numbers $> 0$ and tending to 0, the $U_{a_n}$ form a fundamental system of entourages of the uniformity defined by $f$.
2) The definition of a uniformity by a pseudometric $f$ consists in taking as a fundamental system of entourages the inverse image under $f$ of the neighbourhood filter of 0 in the subspace $[0, +\infty]$ of $\overline{\mathbf{R}}$. Note that this procedure is quite analogous to that which allowed us to define the uniformities on a topological group (Chapter III, § 3, no. 1).

Let $f$ and $g$ be two pseudometrics on $X$. From Definition 2 it follows that the uniformity defined by $f$ is coarser than the uniformity defined by $g$ if and only if, for each $a > 0$ there exists $b > 0$ such that the relation $g(x, y) \leq b$ implies $f(x, y) \leq a$. A necessary and sufficient condition for $f$ and $g$ to be equivalent pseudometrics is that for each $a > 0$ there exists $b > 0$ such that $g(x, y) \leq b$ implies $f(x, y) \leq a$, and $f(x, y) \leq b$ implies $g(x, y) \leq a$.

In particular, if there exists a constant $k$ such that $f \leq kg$, the uniformity defined by $f$ is coarser than the uniformity defined by $g$.

Let $\varphi$ be a mapping of the interval $[0, +\infty]$ into itself, satisfying the following conditions: 1) $\varphi(0) = 0$, and $\varphi$ is continuous at 0; 2) $\varphi$ is increasing in $[0, +\infty]$ and is strictly increasing in a neighbourhood of 0; 3) for all $u \geq 0$ and $v \geq 0$, we have $\varphi(u + v) \leq \varphi(u) + \varphi(v)$. Then if $f$ is any pseudometric on a set $X$, the composition $g = \varphi \circ f$ is a pseudometric equivalent to $f$.

The reader may easily verify that we may, for example, take $\varphi$ to be any one of the following functions:

$$
\sqrt{u}, \quad \log (1 + u), \quad \frac{u}{1 + u}, \quad \inf (u, 1).
$$

The last two examples show that there always exist bounded pseudometrics equivalent to any given pseudometric (finite or not).

#### Definition 3 {#top-ix-s1-def-3 .statement}

If $(f_i)_{i \in I}$ is a family of pseudometrics on a set $X$, then the least upper bound of the set of uniformities defined on $X$ by the pseudometrics $f_i$ is called the uniformity defined by the family $(f_i)$.

Two families of pseudometrics on $X$ are said to be equivalent if they define the same uniformity on $X$.

From the definition of the least upper bound of a set of uniformities (Chapter II, § 2, no. 5), the filter of entourages of the uniformity $U$ defined on $X$ by a family of pseudometrics $(f_i)_{i \in I}$ is the filter *generated* (Chapter I, § 6, no. 2) by the family of sets $f_i^{-1}([0, a])$, where $i$ runs through $I$ and $a$ runs through the set of real numbers $> 0$. In other words, we obtain a fundamental system of entourages of $\mathcal{U}$ by proceeding as follows: we take at random a finite number of indices $i_1, i_2, \ldots, i_n$ and, corresponding to each $i_k$, a number $a_k > 0$; then we consider the set $V$ of pairs $(x, y) \in X \times X$ such that $f_{i_k}(x, y) \leq a_k$ for $1 \leq k \leq n$; these sets $V$ (for all possible choices of $n$, the $i_k$ and the $a_k$) form a fundamental system of entourages for $\mathcal{U}$. Moreover, we may restrict ourselves to the case in which all the $a_k$ are equal to the *same* number $a > 0$, since the entourage consisting of all pairs $(x, y)$ such that

$$
\sup_{1 \leq k \leq n} (f_{i_k}(x, y)) \leq \inf_{1 \leq k \leq n} a_k
$$

is evidently contained in $V$.

For each finite subset $H$ of $I$, let $g_H$ denote the upper envelope of the family $(f_i)_{i \in H}$. As $H$ runs through the set of all finite subsets of $I$ and $a$ runs through the set of real numbers $> 0$, the sets $g_H^{-1}([0, a])$ form a *fundamental system of entourages* of the uniformity $\mathcal{U}$. Now the $g_H$ are *pseudometrics* on $X$ (no. 1), and the upper envelope of a finite number of functions of the family $(g_H)$ belongs to this family, by definition; we express this property by saying that the family of pseudometrics $(g_H)$ is *saturated*. The family of pseudometrics $(g_H)$ is therefore *equivalent* to the family $(f_i)$, and is said to be the family of pseudometrics obtained by *saturating* $(f_i)$. From what has just been said it follows that we may always restrict ourselves to considering uniformities defined by *saturated* families of pseudometrics.

In the particular case where $I$ is a *finite* set, this argument shows that the uniformity defined by the family of pseudometrics $(f_i)_{i \in I}$ is also defined by the *single* pseudometric $g = \sup_{i \in I} f_i$.

Let $\mathcal{U}, \mathcal{U}'$ be two uniformities on $X$, defined respectively by two *saturated* families $(f_i)_{i \in I}, (g_x)_{x \in K}$. Then $\mathcal{U}$ is *coarser* than $\mathcal{U}'$ if and only if, for each index $i \in I$ and each real number $a > 0$, there is an index $x \in K$ and a number $b > 0$ such that the relation $g_x(x, y) \leq b$ implies $f_i(x, y) \leq a$.

*Example of a uniformity defined by a family of pseudometrics.* Let $(f_i)_{i \in I}$ be an arbitrary family of (finite) *real-valued functions* defined on a set $X$. Let $\mathcal{U}$ be the coarsest uniformity on $X$ with respect to which the $f_i$ are uniformly continuous (Chapter II, § 2, no. 3). Then it follows from the definition of the entourages of $\mathcal{U}$ (*loc. cit.*) that $\mathcal{U}$ is the uniformity defined on $X$ by the pseudometrics

$$
g_i(x, y) = |f_i(x) - f_i(y)|.
$$

### 3. PROPERTIES OF UNIFORMITIES DEFINED BY FAMILIES OF PSEUDOMETRICS

Let $\mathcal{U}$ be a uniformity defined on a set $X$ by a family of finite pseudometrics $(f_i)$. If we endow $X \times X$ with the uniformity which is the product of $\mathcal{U}$ by itself, then each of the real-valued functions $f_i$ is *uniformly continuous* on $X \times X$; for by (1) we have

$$
|f_i(x, y) - f_i(x', y')| \leq f_i(x, x') + f_i(y, y'),
$$

and therefore the relations $f_i(x, x') \leq \varepsilon/2, f_i(y, y') \leq \varepsilon/2$ imply

$$
|f_i(x, y) - f_i(x', y')| \leq \varepsilon.
$$

For $\mathcal{U}$ to be *Hausdorff* it is necessary and sufficient, from the definition of the entourages of $\mathcal{U}$, that for each pair of *distinct* points $x, y$ of $X$ there is an index $i$ such that $f_i(x, y) \neq 0$.

In particular, if $\mathcal{U}$ is defined by a *single* pseudometric $f$, then $\mathcal{U}$ is Hausdorff if and only if the relation $f(x, y) = 0$ implies $x = y$ (cf. § 2). If $\mathcal{U}$ is not Hausdorff, the intersection of all the entourages of $\mathcal{U}$ is the subset of $X \times X$ consisting of pairs $(x, y)$ such that $f_i(x, y) = 0$ for all $i$; this subset is the graph of an equivalence relation $R$ on $X$, and the Hausdorff uniformity associated with $\mathcal{U}$ is defined on $X/R$ (cf. Chapter II, § 3, no. 8). It is then easily verified that the functions $f_i$ are compatible (in $x$ and in $y$) with the relation $R$ (*Set Theory*, R, § 5, no. 7) and that the functions $\overline{f_i}$, obtained from $f_i$ by passing to the quotient (with respect to $x$ and $y$), are pseudometrics on $X/R$ which define the Hausdorff uniformity associated with $\mathcal{U}$ (cf. § 2, no. 1).

If $A$ is a non-empty subset of $X$, the restriction to $A \times A$ of a pseudometric on $X$ is clearly a pseudometric on $A$. The uniformity *induced* by $\mathcal{U}$ on $A$ is clearly that defined by the family of restrictions to $A \times A$ of the pseudometrics $f_i$.

Let us now look at the *completion* of the uniform space $X$ when $\mathcal{U}$ is Hausdorff.

#### Proposition 1 {#top-ix-s1-prop-1 .statement}

*Let $X$ be a Hausdorff uniform space whose uniformity $\mathcal{U}$ is defined by a family of finite pseudometrics* $(f_i)$, *and let* $\hat{X}$ *be the completion* of $X$. Then the functions $f_i$ can be extended by continuity to $\hat{X} \times \hat{X}$; the extended functions $\bar{f}_i$ are finite pseudometrics on $\hat{X} \times \hat{X}$, and the family $(f_i)$ defines the uniformity of $\hat{X}$.

First, the $f_i$ can be extended by continuity to $\hat{X} \times \hat{X}$, because they are uniformly continuous on $X \times X$; and the extended functions $\bar{f}_i$ are uniformly continuous on $\hat{X} \times \hat{X}$ (Chapter II, § 3, no. 6, Theorem 2); moreover, they are pseudometrics on $\hat{X}$ by virtue of the principle of extension of inequalities (Chapter IV, § 5, no. 2, Theorem 1). Let $\mathcal{U}_1$ denote the uniformity on $\hat{X}$ obtained by completion, and let $\mathcal{U}_2$ denote the uniformity defined by the family of pseudometrics $(\bar{f}_i)$. Then $\mathcal{U}_2$ is coarser than $\mathcal{U}_1$; for each $\bar{f}_i$ is uniformly continuous on $\hat{X} \times \hat{X}$ with respect to $\mathcal{U}_1$, and hence for each $a > 0$ there exists an entourage $V$ of $\mathcal{U}_1$ such that, whenever $(x, y) \in V$, we have $|\bar{f}_i(x, y) - \bar{f}_i(x, x)| \leq a$, that is [since $\bar{f}_i(x, x) = 0$], $V \subset \bar{f}_i([0, a])$; hence every entourage of $\mathcal{U}_2$ is an entourage of $\mathcal{U}_1$. On the other hand, $\mathcal{U}_1$ and $\mathcal{U}_2$ induce the same uniformity $\mathcal{U}$ on $X$. As $\hat{X}$ is complete with respect to $\mathcal{U}_1$, it follows that $\mathcal{U}_1$ and $\mathcal{U}_2$ are identical (Chapter II, § 3, no. 7, Proposition 14).

### 4. CONSTRUCTION OF A FAMILY OF PSEUDOMETRICS DEFINING A UNIFORMITY

The significance of defining a uniformity by means of a family of pseudometrics lies in the fact that all uniformities can be so obtained. Namely:

#### Theorem 1 {#top-ix-s1-thm-1 .statement}

Given a uniformity $\mathcal{U}$ on a set $X$, there is a family of pseudometrics on $X$ such that the uniformity defined by this family is identical with $\mathcal{U}$.

For each entourage $V$ of the uniformity $\mathcal{U}$, define inductively a sequence of symmetric entourages $(U_n)$ such that $U_1 \subset V$ and $U_{n+1} \subset U_n$ for all $n \geq 1$. The sequence $(U_n)$ is a fundamental system of entourages of a uniformity $\mathcal{U}_V$ coarser than $\mathcal{U}$; moreover, it is clear that $\mathcal{U}$ is the least upper bound of all the uniformities $U_V$ as $V$ runs through the filter of entourages of $\mathcal{U}$. Theorem 1 is therefore a consequence of the following proposition:

#### Proposition 2 {#top-ix-s1-prop-2 .statement}

If a uniformity $\mathcal{U}$ on $X$ has a countable fundamental system of entourages, then there is a pseudometric $f$ on $X$ such that $\mathcal{U}$ is identical with the uniformity defined by $f$.

Let $(V_n)$ be a countable fundamental system of entourages of $\mathcal{U}$. Define inductively a sequence $(U_n)$ of symmetric entourages of $\mathcal{U}$ such that $U_1 \subset V_1$ and
$$
\bigcup_{n+1}^3 \subset U_n \cap V_n \quad \text{for} \quad n \geq 1.
$$
Clearly $(U_n)$ is another fundamental system of entourages of $\mathcal{U}$, and we have in particular $\bigcup_{n+1}^3 \subset U_n$ for $n \geq 1$. We define a real-valued function $g$ on $X \times X$ as follows: $g(x, y) = 0$ if $(x, y) \in U_n$ for all $n$; $g(x, y) = 2^{-k}$ if $(x, y) \in U_n$ for $1 \leq n \leq k$, but $(x, y) \notin U_{k+1}$; $g(x, y) = 1$ if $(x, y) \notin U_1$. The function $g$ is symmetric and positive, and we have $g(x, x) = 0$ for all $x \in X$. Put
$$
f(x, y) = \inf \sum_{i=0}^{p-1} g(z_i, z_{i+1}),
$$
the greatest lower bound being taken over the set of all finite sequences $(z_i)_{0 \leq i \leq p}$ ($p$ arbitrary) such that $z_0 = x$ and $z_p = y$. We shall show that $f$ is a *pseudometric* which satisfies the inequalities
$$
\frac{1}{2} g(x, y) \leq f(x, y) \leq g(x, y).
$$
It follows immediately from the definition that $f$ is symmetric and positive and satisfies the triangle inequality. Also it is clear that $f(x, y) \leq g(x, y)$, hence $f(x, x) = 0$ for all $x \in X$, and therefore $f$ is a pseudometric. To prove the left-hand half of the inequalities (2), let us show by induction on $p$ that, for every finite sequence $(z_i)_{0 \leq i \leq p}$ of $p + 1$ points of $X$ such that $z_0 = x$ and $z_p = y$, we have
$$
\sum_{i=0}^{p-1} g(z_i, z_{i+1}) \geq \frac{1}{2} g(x, y).
$$
This is clear if $p = 1$. Put $a = \sum_{i=0}^{p-1} g(z_i, z_{i+1})$; the inequality (3) is true if $a \geq 1/2$, because $g(x, y) \leq 1$. Suppose then that $a < 1/2$, and let $h$ be the largest of the indices $q$ such that
$$
\sum_{i < q} g(z_i, z_{i+1}) \leq \frac{a}{2};
$$
we have then $\sum_{i < h} g(z_i, z_{i+1}) \leq a/2$ and $\sum_{i < h+1} g(z_i, z_{i+1}) > a/2$, whence
$$
\sum_{i > h} g(z_i, z_{i+1}) \leq \frac{a}{2}.
$$

By the inductive hypothesis we have $g(x, z_h) \leq a$ and $g(z_{h+1}, y) \leq a$; on the other hand it is clear that $g(z_h, z_{h+1}) \leq a$. Let $k$ be the smallest integer $> 0$ such that $2^{-k} \leq a$; then $k \geq 2$, and $(x, z_h) \in U_k, (z_h, z_{h+1}) \in U_k, (z_{h+1}, y) \in U_k$ by the definition of $g$; hence $(x, y) \in U_k \subset U_{k-1}^3$, which implies that $g(x, y) \leq 2^{1-k} \leq 2a$.

Hence the inequalities (2) are proved; they show that, for each $a > 0$, the set $f^{-1}([0, a])$ contains $U_k$ for each index $k$ such that $2^{-k} < a$, and conversely that each $U_k$ contains the set $f^{-1}([0, 2^{-k-1}])$; hence the sets $f^{-1}([0, a])$ form a fundamental system of entourages of the structure $\mathcal{U}$.

Q.E.D.

#### Remark {#top-ix-s1-n4-rem-1 .statement}

A uniformity $\mathcal{U}$ on $X$ is defined by the family $\Phi$ of all pseudometrics on $X$ which are uniformly continuous on $X \times X$. For clearly the uniformity defined by the family $\Phi$ is coarser than $\mathcal{U}$; conversely, Theorem 1 shows that there is a subfamily of $\Phi$ which defines the uniformity $\mathcal{U}$ and therefore the uniformity defined by $\Phi$ is finer than $\mathcal{U}$.

### 5. UNIFORMIZABLE SPACES

In Chapter II, § 4, no. 1, we posed the problem of characterizing uniformizable topological spaces. The solution is given by the following theorem:

#### Theorem 2 {#top-ix-s1-thm-2 .statement}

*A topological space* $X$ *is uniformizable if and only if it satisfies the following axiom:*

(OIV) *Given any point* $x_0 \in X$ *and any neighbourhood* $V$ *of* $x_0$, *there exists a continuous real-valued function on* $X$ *which takes its values in* $[0, 1]$, *is equal to* $0$ *at* $x_0$, *and is equal to* $1$ *on* $C_V$.

The condition is necessary. For if there is a uniformity on $X$ compatible with the topology of $X$, then by Theorem 1 this uniformity can be defined by a family $(f_i)$ of pseudometrics on $X$, and we may assume with no loss of generality that this family is *saturated* (no. 2). From the definition of the entourages of the uniformity defined by such a family of pseudometrics, there is a pseudometric $f_\alpha$ of the family $(f_i)$, and a number $a > 0$, such that $f_\alpha(x_0, x) \geq a$ for all $x \in C_V$. It follows that the function $g(x) = \inf \left( 1, \frac{1}{a} f_\alpha(x_0, x) \right)$ satisfies all the conditions laid down in (OIV).

The condition is sufficient. For let $\Phi$ be the set of all *continuous mappings* of $X$ into $[0, 1]$. Axiom (OIV) shows that *the coarsest uniformity with respect to which all the functions belonging to* $\Phi$ *are uniformly continuous is compatible* with the topology of $X$ (Chapter II, § 2, no. 3).

#### Definition 4 {#top-ix-s1-def-4 .statement}

*A topological space is said to be completely regular if it is uniformizable and Hausdorff.*

Equivalently, in view of Theorem 2, a space is completely regular if it satisfies axioms (H) [cf. Chapter I, § 8, no. 1, Proposition 1] and (O_{IV}).

#### Remark {#top-ix-s1-n5-rem-1 .statement}

Axiom (O_{IV}) implies (O_{III}) (cf. Chapter I, § 8, no. 4), for if V is a neighbourhood of x_0 and if f is a continuous real-valued function on X with values in [0, 1], such that f(x_0) = 0, f(x) = 1 for all x \in \overline{V}, then the set \overline{f}([0, 1/2]) is a closed neighbourhood of x_0 contained in V. In particular, every *completely regular* space is *regular* (which justifies the terminology). But there are examples of regular spaces which are not completely regular (*), so that (O_{III}) does not imply (O_{IV}).

Every compact space is completely regular (Chapter II, § 4, no. 1, Theorem 1) and therefore so is every subspace of a compact space. We can now complete this proposition by proving its *converse*:

#### Proposition 3 {#top-ix-s1-prop-3 .statement}

*A topological space X is completely regular if and only if it is homeomorphic to a subspace of a compact space.*

Consider the coarsest uniformity on X with respect to which all continuous mappings of X into [0, 1] are uniformly continuous; we have already used this uniformity in the proof of Theorem 2, where we saw that it is compatible with the topology of X if X is uniformizable. Furthermore, this uniformity is a structure of a *precompact* space, by the compactness of the interval [0, 1] and Proposition 3 of Chapter II, § 4, no. 2. If X is Hausdorff, the completion of X with respect to this is therefore compact, and the proposition is proved.

We can therefore say that a completely regular space can be *embedded* in a compact space. It is often convenient to present this result in the following way:

In general, a *cube* is a topological space K^I, the product of a family of topological spaces each identical with a *compact interval* K of \mathbf{R}, indexed by an arbitrary set I. If I is finite and has n elements, we recover the notion of an *n-dimensional closed cube*, which was defined in Chapter VI, § 1, no. 1. A cube is a *compact* space (Chapter I, § 9, no. 5, Theorem 3).

#### Proposition 4 {#top-ix-s1-prop-4 .statement}

*If a topological space X is completely regular, it is homeomorphic to a subspace of a cube.*

Let $(f_i)_{i \in I}$ denote the family of all continuous mappings of X into K = [0, 1], and let g denote the mapping $x \mapsto (f_i(x))$ of X into

(*) See A. Tychonoff, *Math. Ann.*, 102, (1930), p. 553.

K¹. If $x, y$ are any two distinct points of $X$, it follows from axioms (H) and (O_IV) that there is an index $i$ such that $f_i(x) \neq f_i(y)$, and therefore $g$ is a *one-to-one* mapping of $X$ into $K^1$. Moreover, it is immediate that $g$ is an isomorphism of the coarsest uniformity on $X$ for which all the $f_i$ are uniformly continuous, onto the uniformity induced on $g(X)$ by the product uniformity of $K^1$; *a fortiori*, $g$ is a homeomorphism of $X$ onto $g(X)$.

### 6. SEMI-CONTINUOUS FUNCTIONS ON A UNIFORMIZABLE SPACE

In Chapter IV, § 6, no. 2, Corollary to Theorem 4, we showed that the upper envelope of a family of continuous real-valued functions on a topological space is a lower semi-continuous function. If the space is *uniformizable*, there is a converse to this proposition:

#### Proposition 5 {#top-ix-s1-prop-5 .statement}

*In order that every lower semi-continuous real-valued function $f$ (finite or not) on a topological space $X$ should be the upper envelope of the continuous real-valued functions on $X$ (finite or not) which are $\leq f$, it is necessary and sufficient that $X$ be uniformizable.*

The condition is *necessary*. Let $x_0$ be any point of $X$ and let $V$ be any open neighbourhood of $x_0$; then the characteristic function $\varphi_V$ of the set $V$ is lower semi-continuous (Chapter IV, § 6, no. 2, Corollary to Proposition 1); by hypothesis, there is therefore a continuous real-valued function $g$ on $X$ such that $g \leq \varphi_V$ and $g(x_0) = a > 0$. The continuous function $\inf \left( 1, \frac{1}{a} g^+ \right)$ takes its values in $[0, 1]$, is equal to 0 in $C_V$, and equal to 1 at $x_0$. Hence (Theorem 2) $X$ is uniformizable.

The condition is *sufficient*. Consider first the case in which $f$ takes its values in $[-1, +1]$. We have to show that, for each $x_0 \in X$ and each number $a < f(x_0)$, there is a continuous real-valued function $g$ on $X$ such that $g \leq f$ and $g(x_0) \geq a$. If $a \leq -1$, we may take $g$ to be the constant $-1$. If $-1 < a < f(x_0)$, there is a neighbourhood $V$ of $x_0$ such that $f(x) \geq a$ for all $x \in V$. Since $X$ is uniformizable, there is a continuous real-valued function $h$ on $X$, with values in $[0, 1]$, such that $h(x_0) = 0$ and $h(x) = 1$ for all $x \in C_V$. We may then take $g(x) = a - (a + 1)h(x)$, and we have a continuous function satisfying the stated conditions. Note that this function takes its values in $[-1, +1]$.

The general case follows by transfer of structure; for there is a strictly increasing homeomorphism of $[-1, +1]$ onto $\overline{\mathbf{R}}$ (Chapter IV, § 4, no. 2, Proposition 2), and the definition of a semi-continuous function involves only the order structure and the topology of $\overline{\mathbf{R}}$.

#### Remark {#top-ix-s1-n6-rem-1 .statement}

In the above proof we see that the function $g$ does not take the value $+1$. By transfer of structure it follows that every lower semi-continuous real-valued function $f$ on the uniformizable space $X$ is the upper envelope of the continuous real-valued functions $g \leq f$ on $X$ *which do not take the value* $+\infty$.

### Exercises {#top-ix-s1-exercises}

See the [exercises for § 1](exercises/s1/).
