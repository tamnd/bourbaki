---
book: top
book_title: General Topology
chapter: X
chapter_title: Function spaces
section: 2
section_title: Equicontinuous sets
lang: en
source: top-v-x
pdf_pages: 0289-0299, 0327-0333
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION AND GENERAL CRITERIA
      page: 0
      pdf_page: 289
    - "no": 2
      title: SPECIAL CRITERIA FOR EQUICONTINUITY
      page: 0
      pdf_page: 293
    - "no": 3
      title: CLOSURE OF AN EQUICONTINUOUS SET
      page: 0
      pdf_page: 295
    - "no": 4
      title: POINTWISE CONVERGENCE AND COMPACT CONVERGENCE ON EQUICONTINUOUS SETS
      page: 0
      pdf_page: 295
    - "no": 5
      title: COMPACT SETS OF CONTINUOUS MAPPINGS
      page: 0
      pdf_page: 296
statements: 24
exercises: 16
content_sha256: 0e518ac6230012625e0fe16b513a7814cbf8c8e0459e8869ade391e4e1719c46
---

## 2. EQUICONTINUOUS SETS

### 1. DEFINITION AND GENERAL CRITERIA

#### Definition 1 {#top-x-s2-def-1 .statement}

*Let $X$ be a topological space and $Y$ a uniform space. A subset $H$ of $\mathcal{F}(X; Y)$ is said to be equicontinuous at a point $x_0 \in X$ if, for each entourage $V$ of $Y$, there is a neighbourhood $U$ of $x_0$ in $X$ such that* (f(x_0), f(x)) \in V \text{ for all } x \in U \text{ and all } f \in H. \text{ H is said to be equicontinuous if it is equicontinuous at every point of } X.

#### Definition 2 {#top-x-s2-def-2 .statement}

Let X and Y be two uniform spaces. A subset H of $\mathcal{F}(X; Y)$ is said to be uniformly equicontinuous if, for each entourage V of Y, there exists an entourage U of X such that we have $(f(x), f(x')) \in V$ whenever $(x, x') \in U$ and $f \in H$.

A family $(f_i)_{i \in I}$ of mappings of X into Y is said to be equicontinuous at a point $x_0$ (resp. equicontinuous, uniformly equicontinuous) if the set of the $f_i$ is equicontinuous at $x_0$ (resp. equicontinuous, uniformly equicontinuous).

It is clear that if $H \subset \mathcal{F}(X; Y)$ is equicontinuous at $x_0$, then each $f \in H$ is continuous at $x_0$; if H is equicontinuous, then each $f \in H$ is continuous on X, i.e. $H \subset C(X; Y)$. Likewise, if H is uniformly equicontinuous (X being a uniform space), every $f \in H$ is uniformly continuous on X. It is also clear that a uniformly equicontinuous set of mappings is equicontinuous; but a set of uniformly continuous mappings can be equicontinuous without being uniformly equicontinuous (see Exercise 1; Corollary 2 to Proposition 1; and no. 2, Proposition 4).

#### Example 1 {#top-x-s2-n1-exa-1 .statement}

Let X be a topological space (resp. a uniform space) and Y a uniform space. Every finite set of continuous (resp. uniformly continuous) mappings of X into Y is equicontinuous (resp. uniformly equicontinuous).

#### Example 2 {#top-x-s2-n1-exa-2 .statement}

Let X, Y be two metric spaces, d (resp. $d'$) the metric on X (resp. Y), and let k, $\alpha$ be two real numbers > 0. Then the set of all mappings $f : X \to Y$ such that
$$
d'(f(x), f(x')) \leq k(d(x, x'))^\alpha
$$
for each pair of points $x, x'$ of X, is uniformly equicontinuous. For example, the set of all isometries (Chapter IX, § 2, no. 2) of X onto a subset of Y is uniformly equicontinuous.

\* Let H be a set of real-valued functions defined on an interval $I \subset \mathbf{R}$, which are differentiable on I and are such that $|f'(x)| \leq k$ for all $x \in I$ and all $f \in H$. Then H is uniformly equicontinuous, because if $x_1, x_2$ are any two points of I we have $|f(x_1) - f(x_2)| \leq k|x_1 - x_2|$ for each $f \in H$ by the mean value theorem. \*

#### Example 3 {#top-x-s2-n1-exa-3 .statement}

Let G be a topological group, let Y be a uniform space and let $f : G \to Y$ be a uniformly continuous mapping [G being endowed with its left uniformity (Chapter III, § 3, no. 1)]. For each $s \in G$, let $f_s$ be the mapping $x \to f(sx)$ of G into Y. Then the set of mappings $f_s (s \in G)$ is uniformly equicontinuous, since the relation $x^{-1}x' \in V$ is equivalent to $(sx)^{-1}(sx') \in V$.

#### Proposition 1 {#top-x-s2-prop-1 .statement}

Let T be a set, let $\mathcal{S}$ be a set of subsets of T, let Y be a uniform space, X a topological (resp. uniform) space, and let f be a mapping of $T \times X$ into $Y$. For each $A \in \mathcal{S}$, let $H_A \subset \mathcal{F}(X; Y)$ be the set of all mappings $x \to f(t, x)$ as $t$ runs through $A$. Then the mapping $x \to f(., x)$ of $X$ into $\mathcal{F}_\mathcal{S}(T; Y)$ is continuous at a point $x_0 \in X$ (resp. uniformly continuous) if and only if the set $H_A$ is equicontinuous at $x_0$ (resp. uniformly equicontinuous) for all $A \in \mathcal{S}$.

Consider first the particular case where $\mathcal{S} = \{ T \}$, i.e. $\mathcal{F}_\mathcal{S}(T; Y) = \mathcal{F}_u(T; Y)$. For each entourage $V$ of $Y$, the condition $(f(., x), f(., x')) \in W(V)$ signifies that $(f(t, x), f(t, x')) \in V$ for all $t \in T$. To say that $x \to f(., x)$ is continuous at $x_0$ (resp. is uniformly continuous) is therefore equivalent to saying that, for each entourage $V$ of $Y$, there is a neighbourhood $U$ of $x_0$ in $X$ (resp. an entourage $M$ of $X$) such that the relation $x \in U$ [resp. $(x, x') \in M$] implies $(f(t, x), f(t, x_0)) \in V$ [resp. $(f(t, x), f(t, x')) \in V$] for all $t \in T$, and the proposition follows from Definitions 1 and 2. In the general case, we have to express that, for each $A \in \mathcal{S}$, the mapping $x \to f(., x)|A$ of $X$ into $\mathcal{F}_u(A; Y)$ is continuous at $x_0$ (resp. uniformly continuous), by virtue of § 1, no. 2; from what has been said, this is equivalent to saying that, for each $A \in \mathcal{S}$, $H_A$ is equicontinuous at $x_0$ (resp. uniformly equicontinuous).

Proposition 1 allows us to translate Definitions 1 and 2 into forms which are sometimes useful, by applying it to the case where $T = H$ and $f$ is the mapping $(h, x) \to h(x)$ of $H \times X$ into $Y$; since $f(., x)$ is the mapping $h \to h(x)$ of $H$ into $Y$, we see that:

#### Corollary 1 {#top-x-s2-prop-1-cor-1 .statement}

Let $X$ be a topological (resp. uniform) space, $Y$ a uniform space and $H$ a subset of $\mathcal{F}(X; Y)$. For each $x \in X$, let $\tilde{x}$ denote the mapping $h \to h(x)$ of $H$ into $Y$. Then $H$ is equicontinuous at $x_0$ (resp. uniformly equicontinuous) if and only if the mapping $x \to \tilde{x}$ of $X$ into the uniform space $\mathcal{F}_u(H; Y)$ is continuous at $x_0$ (resp. uniformly continuous).

In particular, if $X$ is compact, every continuous mapping of $X$ into $\mathcal{F}_u(H; Y)$ is uniformly continuous (Chapter II, § 4, no. 1, Theorem 2). Therefore:

#### Corollary 2 {#top-x-s2-prop-1-cor-2 .statement}

Let $X$ be a compact space, $Y$ a uniform space. Then every equicontinuous subset of $\mathcal{F}(X; Y)$ is uniformly equicontinuous.

Now suppose we have a set $T$, a topological space $X$, a uniform space $Y$ and a mapping $f : T \times X \to Y$. Let $\tilde{f}$ denote the mapping $x \to f(., x)$ of $X$ into $\mathcal{F}_u(T; Y)$, and let us consider the canonical mapping $\theta : (t, g) \to g(t)$ of $T \times \mathcal{F}_u(T; Y)$ into $Y$. It is clear that the diagram

$$
\begin{array}{ccc}
T \times X & \xrightarrow{f} & Y \\
\downarrow_{\iota_T \times \tilde{f}} & & \uparrow \theta \\
T \times \mathcal{F}_u(T; Y)
\end{array}
$$

(where $i_T$ is the identity mapping of T) is commutative. Suppose now that T is endowed with a topology and that, for each $x \in X$, the mapping $f(., x) : t \to f(t., x)$ is continuous; we can then replace $\mathcal{F}_u(T; Y)$ by $\mathcal{C}_u(T; Y)$ in the above diagram. But we know that $\theta$ is continuous from § 1, no. 6, Proposition 9; hence if $\tilde{f}$ is continuous it follows that $f$ is continuous. Since the continuity of $\tilde{f}$ can be expressed with the help of Proposition 1, we obtain the following result:

#### Corollary 3 {#top-x-s2-prop-1-cor-3 .statement}

*Let T, X be topological spaces, let Y be a uniform space and let f be a mapping of T × X into Y. Then f is continuous, provided that the following conditions are satisfied:*

1) *For each $x \in X$, the partial mapping $t \to f(t, x)$ is continuous.*

2) *As t runs through T, the partial mappings $x \to f(t, x)$ form an equicontinuous subset of $\mathcal{F}(X; Y)$.*

In particular, take T to be a subset H of $\mathcal{F}(X; Y)$ and f to be the canonical mapping $(h, x) \to h(x)$ of $H \times X$ into Y; condition 1) of Corollary 3 means that H is endowed with a topology finer than that of pointwise convergence, and condition 2) means that H is equicontinuous. Hence:

#### Corollary 4 {#top-x-s2-prop-1-cor-4 .statement}

*Let X be a topological space, Y a uniform space, H an equicontinuous set of mappings of X into Y. If H is endowed with the topology of pointwise convergence, then the mapping $(h, x) \to h(x)$ of $H \times X$ into Y is continuous.*

More intuitively, this expresses the fact that if $h \in H$ converges *pointwise* to $h_0 \in H$ and if $x \in X$ converges to $x_0$, then $h(x)$ converges to $h_0(x_0)$.

#### Corollary 5 {#top-x-s2-prop-1-cor-5 .statement}

*Let X be a topological space, let Y, Z be two uniform spaces and let H be an equicontinuous set of mappings of Y into Z. If H, $\mathcal{C}(X; Y)$ and $\mathcal{C}(X; Z)$ are endowed with the topology of pointwise convergence, then the mapping $(u, v) \to u \circ v$ of $H \times \mathcal{C}(X; Y)$ into $\mathcal{C}(X; Z)$ is continuous.*

We have to show that, for each $x \in X$, the mapping $(u, v) \to u(v(x))$ of $H \times \mathcal{C}(X; Y)$ into Z is continuous. Now $v \to v(x)$ is continuous on H (§ 1, no. 2, Remark 6), and it follows from Corollary 4 that $(u, y) \to u(y)$ is a continuous mapping of $H \times Y$ into Z; since $(u, v) \to u(v(x))$ is the composition of $(u, y) \to u(y)$ and $(u, v) \to (u, v(x))$, the result is proved.

The following proposition and its corollary are the analogues of Corollaries 3 and 4 of Proposition 1 for uniformly equicontinuous sets of mappings:

#### Proposition 2 {#top-x-s2-prop-2 .statement}

Let T, X, Y be uniform spaces and let f be a mapping of T × X into Y. Then f is uniformly continuous if and only if the following two conditions are satisfied:

1) The mappings x → f(t, x) (t ∈ T) form a uniformly equicontinuous subset of $\mathcal{F}(X; Y)$.

2) The mappings t → f(t, x) (x ∈ X) form a uniformly equicontinuous subset of $\mathcal{F}(T; Y)$.

It is easily seen that the conditions are necessary. Conversely, suppose that they are satisfied. Let W be an entourage of Y; then there exists an entourage U of T and an entourage V of X such that:

1) $(t', t'') \in U$ implies that, for each $x \in X$,
$$
(f(t', x), f(t'', x)) \in W.
$$

2) $(x', x'') \in V$ implies that, for each $t \in T$,
$$
(f(t, x'), f(t, x'')) \in W.
$$

It is now clear that the relation "$(t', t'') \in U$ and $(x', x'') \in V$" implies that $(f(t', x'), f(t'', x'')) \in \hat{W}$, whence the result.

In particular, take T to be a subset H of $\mathcal{F}(X; Y)$, endowed with the uniformity of uniform convergence, and take f to be the canonical mapping $(h, x) \to h(x)$; then condition 2) of Proposition 2 is automatically satisfied because, for each entourage W of Y, the set of pairs $(h', h'')$ such that $(h'(x), h''(x)) \in W$ for all $x \in X$ is by definition an entourage of the uniform structure of H. Hence only condition 1) has to be expressed; in other words:

#### Corollary {#top-x-s2-n1-cor-1 .statement}

Let X, Y be two uniform spaces and let H be a subset of $\mathcal{F}(X; Y)$. Then H is uniformly equicontinuous if and only if the mapping $(h, x) \to h(x)$ of $H \times X$ into Y is uniformly continuous, H being endowed with the uniformity of uniform convergence.

### 2. SPECIAL CRITERIA FOR EQUICONTINUITY

It is clear that every subset of an equicontinuous (resp. uniformly equicontinuous) set is equicontinuous (resp. uniformly equicontinuous). Again, if X is a topological (resp. uniform) space and Y is a uniform space, every finite union of equicontinuous (resp. uniformly equicontinuous) subsets of $\mathcal{F}(X; Y)$ is equicontinuous (resp. uniformly equicontinuous).

Let X, X' be two topological (resp. uniform) spaces, let Y, Y' be two uniform spaces, let $f : X \to X'$ be a continuous (resp. uniformly continuous) mapping and let $g : Y \to Y'$ be a uniformly continuous mapping.

It follows immediately from the definitions that the mapping $u \to g \circ u \circ f$ of $\mathcal{F}(X; Y)$ into $\mathcal{F}(X'; Y')$ transforms equicontinuous (resp. uniformly equicontinuous) sets into equicontinuous (resp. uniformly equicontinuous) sets.

#### Proposition 3 {#top-x-s2-prop-3 .statement}

*Let $X$ be a topological (resp. uniform) space, let $(Y_i)_{i \in I}$ be a family of uniform spaces, let $Y$ be a set, and for each $i \in I$, let $f_i$ be a mapping of $Y$ into $Y_i$. Let $Y$ be endowed with the coarsest uniformity for which all the $f_i$ are uniformly continuous. For a subset $H$ of $\mathcal{F}(X; Y)$ to be equicontinuous (resp. uniformly equicontinuous) it is necessary and sufficient that, for each $i \in I$, the image of $H$ under the mapping $u \to f_i \circ u$ be an equicontinuous (resp. uniformly equicontinuous) subset of $\mathcal{F}(X; Y_i)$.*

This is an immediate consequence of Definitions 1 and 2 and the definition of the entourages of $Y$.

#### Proposition 4 {#top-x-s2-prop-4 .statement}

*Let $X, Y$ be two uniform spaces and let $H$ be a set of uniformly continuous mappings of $X$ into $Y$. Let $\hat{X}, \hat{Y}$ be the Hausdorff completions of $X, Y$ respectively, and let $\tilde{H}$ denote the set of mappings $\hat{u} : \hat{X} \to \hat{Y}$ as $u$ runs through $H$ (Chapter II, § 3, no. 7, Proposition 15). Then $H$ is uniformly equicontinuous if and only if $\tilde{H}$ is uniformly equicontinuous.*

We recall that the diagram

$$
\begin{array}{ccc}
X & \xrightarrow{u} & Y \\
i \downarrow & & j \downarrow \\
\hat{X} & \xrightarrow{\hat{u}} & \hat{Y}
\end{array}
$$

is commutative, where $i$ and $j$ are the canonical mappings; moreover, the uniformity of $X$ (resp. $Y$) is the inverse image under $i$ (resp. $j$) of that of $\hat{X}$ (resp. $\hat{Y}$). Hence $H$ is uniformly equicontinuous if and only if its image under the mapping $u \to j \circ u$ is uniformly equicontinuous (Proposition 3), and we may already restrict ourselves to the case where $Y$ is Hausdorff and complete; moreover, if $\tilde{H}$ is uniformly equicontinuous then so is $H$, because it is the image of $\tilde{H}$ under the mapping $\hat{u} \to \hat{u} \circ i$; thus it remains to prove the converse when $Y = \hat{Y}$. Let $V$ be a closed entourage of $Y$; by hypothesis there is an entourage $U$ of $X$ such that the relations $(x, x') \in U$ and $u \in H$ imply that $(u(x), u(x')) \in V$. Now, if $U'$ is the image of $U$ under $i \times i$, the closure $\overline{U'}$ of $U'$ in $\hat{X} \times \hat{X}$ is an entourage of $\hat{X}$ (Chapter II, § 3, no. 7, Proposition 12); the hypothesis implies that, whenever $(z, z') \in U'$ and $u \in H$, we have $(\hat{u}(z), \hat{u}(z')) \in V$. Since $V$ is closed and $\hat{u}$ is continuous, we have also $(\hat{u}(t), \hat{u}(t')) \in V$ for all $(t, t') \in \overline{U'}$ and all $u \in H$; this completes the proof.

#### Proposition 5 {#top-x-s2-prop-5 .statement}

Let $G, G'$ be two topological groups endowed with their left uniformities, and let $H$ be a set of homomorphisms of $G$ into $G'$. Then the following conditions are equivalent:
a) $H$ is equicontinuous at the identity element $e$ of $G$,
b) $H$ is equicontinuous,
c) $H$ is uniformly equicontinuous.

It is enough to show that a) implies c). Let $V'$ be a neighbourhood of the identity element $e'$ of $G'$; then, by hypothesis, there is a neighbourhood $V$ of $e$ in $G$ such that $u(V) \subset V'$ for all $u \in H$; since the elements of $H$ are homomorphisms, the relation $x^{-1} y \in V$ implies that we have
$$
(u(x))^{-1} u(y) = u(x^{-1} y) \in V'.
$$
In view of the definition of the entourages of the left uniformities of $G$ and $G'$ (Chapter III, § 3, no. 1), the result follows.

### 3. CLOSURE OF AN EQUICONTINUOUS SET

#### Proposition 6 {#top-x-s2-prop-6 .statement}

Let $X$ be a topological (resp. uniform) space, let $Y$ be a uniform space and let $H$ be a subset of $\mathcal{F}(X; Y)$. Then $H$ is equicontinuous at a point $x_0 \in X$ (resp. uniformly equicontinuous) if and only if the closure $\overline{H}$ of $H$ in $\mathcal{F}_s(X; Y)$ is equicontinuous at $x_0$ (resp. uniformly equicontinuous).

The condition is sufficient, trivially. To show that it is necessary, consider an entourage $V$ of $Y$ which is closed in $Y \times Y$; by hypothesis, there is a neighbourhood $U$ of $x_0$ in $X$ (resp. an entourage $M$ of $X$) such that the relation $x \in U$ (resp. $(x', x'') \in M$) implies $(h(x_0), h(x)) \in V$ [resp. $(h(x'), h(x'')) \in V$] for all $h \in H$. Since $V$ is closed, the mappings $h \in \mathcal{F}(X; Y)$ which satisfy the relation $(h(x_0), h(x)) \in V$ for all $x \in U$ [resp. the relation $(h(x'), h(x'')) \in V$ for all $(x', x'') \in M$] form a closed subset of $\mathcal{F}_s(X; Y)$ (§ 1, no. 2, Remark 6); since this closed subset contains $H$, it contains $\overline{H}$. Hence the result, since the closed entourages of $Y$ form a fundamental system of entourages (Chapter II, § 1, no. 2, Proposition 2, Corollary 2).

### 4. POINTWISE CONVERGENCE AND COMPACT CONVERGENCE ON EQUICONTINUOUS SETS

#### Theorem 1 {#top-x-s2-thm-1 .statement}

Let $X$ be a topological (resp. uniform) space, let $Y$ be a uniform space and let $H$ be an equicontinuous (resp. uniformly equicontinuous) subset of $\mathcal{C}(X; Y)$. Then the following uniformities on $H$ are identical: the uniformity of compact (resp. precompact) convergence, the uniformity of pointwise convergence and the uniformity of pointwise convergence in a dense subset $D$ of $X$.

It is enough to show that the last uniformity on $H$ is finer than the first; in other words that, given an entourage $V$ of $Y$ and a compact (resp. precompact) subset $A$ of $X$, there exists an entourage $W$ of $Y$ and a finite subset $F$ of $D$ such that the relation

$$
(2)\quad u \in H,\ v \in H\ \text{and}\ (u(x), v(x)) \in W\ \text{for all}\ x \in F
$$

implies

$$
(3)\quad (u(x),\ v(x)) \in V\ \text{for all}\ x \in A.
$$

Suppose first that $A$ is compact and $H$ equicontinuous. Given a symmetric entourage $W$ of $Y$, every point $x \in X$ has a neighbourhood $U(x)$ such that the relation $x' \in U(x)$ implies $(u(x),\ u(x')) \in W$ for all $u \in H$. We can therefore cover the compact set $A$ by a finite number of open sets $U_i$ such that, for each pair of points $x',\ x''$ of the same set $U_i$, we have $(u(x'),\ u(x'')) \in \hat{W}$ for all $u \in H$. Let $a_i$ be a point of $D \cap U_i$, let $F$ be the set of the $a_i$, and suppose that (2) is true; then for each $x \in A$ there exists an index $i$ such that $a_i$ and $x$ belong to the same set $U_i$, so that we have $(u(x),\ u(a_i)) \in \hat{W}$ and $(v(a'),\ v(x)) \in \hat{W}$; thus (2) implies (3) provided that $W$ is chosen so that $\hat{W} \subset V$.

If $A$ is precompact and $H$ uniformly equicontinuous, we use Proposition 4 of no. 2; it is enough to note that $i(A)$ is compact in $\hat{X}$, $i(D)$ dense in $\hat{X}$ and that the entourages of $Y$ are the inverse images of those of $\hat{Y}$ under the mapping $j \times j$.

#### Corollary {#top-x-s2-n4-cor-1 .statement}

*Under the hypotheses of Theorem 1, the closure $\overline{H}$ of $H$ in $\mathcal{F}(X; Y)$ with respect to the topology of pointwise convergence is the same as the closure of $H$ in $\mathcal{C}(X; Y)$ with respect to the topology of compact (resp. precompact) convergence.*

For the set $\overline{H}$ is equicontinuous (resp. uniformly equicontinuous) by Proposition 6 of no. 3, and hence is contained in $\mathcal{C}(X; Y)$; the result follows immediately from the fact that, on $\overline{H}$, the two topologies under consideration are the same, by virtue of Theorem 1.

### 5. COMPACT SETS OF CONTINUOUS MAPPINGS

#### Theorem 2 (Ascoli) {#top-x-s2-thm-2 .statement}

*Let $X$ be a topological (resp. uniform) space, let $\mathcal{S}$ be a covering of $X$, let $Y$ be a uniform space and $H$ a set of mappings of $X$ into $Y$ such that, for each $A \in \mathcal{S}$ and each $u \in H$, the restriction of $u$ to $A$ is continuous (resp. uniformly continuous). Then, for $H$ to be precompact with respect to the uniformity of $\mathcal{S}$-convergence, it is necessary in all cases and also sufficient* if the sets $A \in \mathcal{S}$ are compact (resp. precompact) that the following conditions should be satisfied:

a) For each $A \in \mathcal{S}$, the set $H|A \subset \mathcal{F}(A; Y)$ of restrictions to $A$ of functions of $H$ is equicontinuous (resp. uniformly equicontinuous).

b) For each $x \in X$, the set $H(x) \subset Y$ of points $u(x)$ ($u \in H$) is precompact.

1) Let us show first that conditions a) and b) are necessary. We know (§ 1, no. 2, Remark 6) that the mapping $u \to u(x)$ of $\mathcal{F}_{\mathcal{S}}(X; Y)$ into $Y$ is uniformly continuous; hence, if $H$ is precompact, so is $H(x)$ (Chapter II, § 4, no. 2, Proposition 2), which proves b). To prove a), consider a set $A \in \mathcal{S}$, a point $x_0 \in A$ and an entourage $V$ of $Y$; since $H$ is precompact it can be covered by a finite number of $W(A, V)$-small sets; in other words there is a finite sequence $(u_i)$ of elements of $H$ such that, for each $u \in H$, we have

$$
(u(x),\ u_i(x)) \in V \quad \text{for all } x \in A
$$

for at least one index $i$.

Since each of the $u_i|A$ is continuous at $x_0$ (resp. uniformly continuous) there is a neighbourhood $U_i$ of $x_0$ in $A$ (resp. an entourage $M_i$ of $A$) such that

$$
x \in U_i \implies (u_i(x), u_i(x_0)) \in V,
$$

(resp. such that

$$
(x', x'') \in M_i \implies (u_i(x'), u_i(x'')) \in V.)
$$

Let $U$ (resp. $M$) be the intersection of the $U_i$ (resp. $M_i$); it is a neighbourhood of $x_0$ in $A$ (resp. an entourage of $A$). For each $u \in H$ there is an index $i$ for which (4) holds; writing condition (4) for $x_0$ and for $x$ (resp. for $x'$ and $x''$) and taking account of (5) [resp. (6)], we see immediately that the relation $x \in U$ [resp. $(x', x'') \in M$] implies $(u(x),\ u(x_0)) \in \overset{\circ}{V}$ [resp. $(u(x'),\ u(x'')) \in \overset{\circ}{V}$], for each $u \in H$; and this establishes a).

2) Now let us show that the conditions a) and b) are sufficient if the sets $A \in \mathcal{S}$ are compact (resp. precompact). Condition b) implies that $H$ is precompact with respect to the uniformity of pointwise convergence (Chapter II, § 4, no. 2, Proposition 3). But it follows from condition a) and Theorem 1 of no. 4 that on $H|A$ the uniformity of pointwise convergence in $A$ coincides with the uniformity of uniform convergence in $A$; hence $H|A$ is precompact in $\mathcal{F}_u(A; Y)$, which implies that $H$ is precompact with respect to the uniformity of $\mathcal{S}$-convergence (§ 1, no. 2).

Note that condition b) of Theorem 2 is automatically satisfied if $Y$ is a precompact space.

#### Corollary 1 {#top-x-s2-thm-2-cor-1 .statement}

Let $X$ be a topological (resp. uniform) space, let $Y$ be a Hausdorff uniform space and let $H$ be an equicontinuous (resp. uniformly equicontinuous) subset of $C(X; Y)$. Suppose that $H(x)$ is relatively compact in $Y$ for each $x \in X$. Then $H$ is relatively compact in $C(X; Y)$ with respect to the topology of compact (resp. precompact) convergence.

Let $\overline{H}$ be the closure of $H$ in $\mathcal{F}_s(X; Y)$. $\overline{H}$ is equicontinuous (resp. uniformly equicontinuous) (no. 3, Proposition 6). Moreover, we have $\overline{H}(x) \subset \overline{H(x)}$ (§ 1, no. 2, Remark 6) and therefore $\overline{H}(x)$ is also relatively compact; hence Theorem 2 shows that $\overline{H}$ is precompact with respect to $\mathcal{S}$-convergence, where $\mathcal{S}$ denotes the set of all compact (resp. precompact) subsets of $X$. Moreover, since $\overline{H(x)}$ is compact, and therefore complete, $\overline{H}$ is complete with respect to the uniformity of pointwise convergence (Chapter II, § 3, no. 5, Proposition 10 and no. 4, Proposition 8) and therefore also with respect to the uniformity of $\mathcal{S}$-convergence (§ 1, no. 5, Proposition 5, Corollary 2); $\overline{H}$ is therefore compact, since it is precompact, complete and Hausdorff (§ 1, no. 2, Proposition 1).

#### Corollary 2 {#top-x-s2-thm-2-cor-2 .statement}

Let $X$ be a topological (resp. uniform) space, let $Y$ be a complete Hausdorff uniform space and let $H$ be an equicontinuous (resp. uniformly equicontinuous) subset of $C(X; Y)$. Suppose that $H(x)$ is relatively compact in $Y$ for all $x \in D$, where $D$ is a dense subset of $X$. Then $H$ is relatively compact in $C(X; Y)$ with respect to the topology of compact (resp. precompact) convergence.

It is enough to show that $H(x)$ is relatively compact for all $x \in X$, for we can then apply Corollary 1. Since $Y$ is complete it is enough to show that $H(x)$ is precompact for all $x \in X$. Now if $V$ is any symmetric entourage of $Y$, there is a neighbourhood $U$ of $x$ such that $(u(x), u(x')) \in V$ for all $x' \in U$ and all $u \in H$. By hypothesis there exists $x' \in U \cap D$, and since $H(x')$ is relatively compact in $Y$, there exists a finite number of points $y_k \in Y$ such that $H(x')$ is contained in the union of the sets $V(y_k)$; hence $H(x)$ is contained in the union of the sets $V(y_k)$, and the proof is complete.

#### Corollary 3 {#top-x-s2-thm-2-cor-3 .statement}

Let $X$ be a locally compact space, $Y$ a Hausdorff uniform space, $H$ a subset of $C(X; Y)$. Then $H$ is relatively compact in $C_c(X; Y)$ if and only if $H$ is equicontinuous and $H(x)$ relatively compact in $Y$ for all $x \in X$.

In view of Corollary 1 it is enough to show that, if $H$ is relatively compact in $C_c(X; Y)$, then $H$ is equicontinuous. Now each point $x \in X$ has a compact neighbourhood $A$, and it follows from Theorem 2 that $H/A$ is equicontinuous; this implies that $H$ is equicontinuous at $x$, and the result is proved.

#### Remark {#top-x-s2-n5-rem-1 .statement}

Let $X$ be a topological space, $Y$ a uniform space and $\mathcal{S}$ a set of subsets of $X$. Then on every *precompact* subset $H$ of $\mathcal{F}_{\mathcal{S}}(X; Y)$, the uniformity of $\mathcal{S}$-convergence is the same as the uniformity of pointwise convergence in $B = \bigcup_{A \in \mathcal{S}} A$. We can reduce to the case where $B = X$ and $Y$ is Hausdorff and complete; for if $j$ is the canonical injection $B \to X$ and $i$ the canonical mapping $Y \to \hat{Y}$, the uniformity of $\mathcal{S}$-convergence on $\mathcal{F}(X; Y)$ is the inverse image of the uniformity of $\mathcal{S}$-convergence on $\mathcal{F}(B; \hat{Y})$ under the mapping $\theta : u \to i \circ u \circ j$ (§ 1, no. 4, Proposition 4), and $H$ is precompact if and only if $\theta(H)$ is (Chapter II, § 4, no. 2, Proposition 3). This being so, if $B = X$ and $Y$ is Hausdorff and complete, $\mathcal{F}_{\mathcal{S}}(X; Y)$ is Hausdorff and complete (§ 1, no. 2, Proposition 1 and no. 5, Theorem 1); hence the closure $\overline{H}$ of $H$ in this space is *compact*. On $\overline{H}$, the topology of pointwise convergence is Hausdorff (§ 1, no. 2, Proposition 1) and coarser than that of $\mathcal{S}$-convergence; hence these two topologies coincide (Chapter I, § 9, no. 4, Theorem 2, Corollary 3) and consequently so do the uniformities of $\mathcal{S}$-convergence and pointwise convergence (Chapter II, § 4, no. 1, Theorem 1).

### Exercises {#top-x-s2-exercises}

See the [exercises for § 2](exercises/s2/).
