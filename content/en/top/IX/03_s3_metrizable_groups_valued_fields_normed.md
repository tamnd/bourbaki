---
book: top
book_title: General Topology
chapter: IX
chapter_title: Use of real numbers in general topology
section: 3
section_title: Metrizable groups, valued fields, normed spaces and algebras
lang: en
source: top-v-x
pdf_pages: 0167-0185, 0242-0245
extraction: ocr
subsections:
    - "no": 1
      title: METRIZABLE TOPOLOGICAL GROUPS
      page: 0
      pdf_page: 167
    - "no": 2
      title: VALUED DIVISION RINGS
      page: 0
      pdf_page: 171
    - "no": 3
      title: NORMED SPACES OVER A VALUED DIVISION RING
      page: 0
      pdf_page: 175
    - "no": 4
      title: QUOTIENT SPACES AND PRODUCT SPACES OF NORMED SPACES
      page: 0
      pdf_page: 178
    - "no": 5
      title: CONTINUOUS MULTILINEAR FUNCTIONS
      page: 0
      pdf_page: 179
    - "no": 6
      title: ABSOLUTELY SUMMABLE FAMILIES IN A NORMED SPACE
      page: 0
      pdf_page: 180
    - "no": 7
      title: NORMED ALGEBRAS OVER A VALUED FIELD
      page: 0
      pdf_page: 181
statements: 40
exercises: 4
content_sha256: 8b0735f9661569735192e866f56800cc2ca77e68b63b4e1c9aade01fcd82bfa5
---

## 3. METRIZABLE GROUPS, VALUED FIELDS, NORMED SPACES AND ALGEBRAS

### 1. METRIZABLE TOPOLOGICAL GROUPS

#### Proposition 1 {#top-ix-s3-prop-1 .statement}

The left and right uniformities of a topological group $G$ are metrizable if and only if $G$ is Hausdorff and the identity element $e$ of $G$ has a countable fundamental system of neighbourhoods.

The condition is clearly necessary. Conversely, if it is satisfied, let $(V_n)$ be a fundamental system of neighbourhoods of $e$; if $U_n$ denotes the set of pairs $(x, y) \in G \times G$ such that $x^{-1}y \in V_n$, then the $U_n$ form a countable fundamental system of entourages of the left uniformity of $G$; since this uniformity is Hausdorff, it follows from § 2, no. 4, Theorem 1 that it is metrizable. Similarly for the right uniformity of $G$.

A topological group $G$ is said to be *metrizable* if its topology is metrizable. Proposition 1 then shows that its two uniformities are metrizable.

This result can be sharpened with the help of the following notion:

#### Definition 1 {#top-ix-s3-def-1 .statement}

*A metric* $d$ *on a group* $G$ *(written multiplicatively)* *is said to be left-invariant* (resp. *right-invariant*) *if we have*

$$
d(zx, zy) = d(x, y) \quad [\text{resp. } d(xz, yz) = d(x, y)]
$$

*for all* $x, y, z$ *in* $G$.

#### Proposition 2 {#top-ix-s3-prop-2 .statement}

*The left* (resp. *right*) *uniformity of a metrizable group* $G$ *can be defined by a left-invariant* (resp. *right-invariant*) *metric on* $G$.

Suppose that the fundamental system $(V_n)$ of neighbourhoods of $e$ consists of symmetric neighbourhoods such that $V_{n+1}^3 \subset V_n$ for each $n$. Then the corresponding entourages $U_n$ of the left uniformity are symmetric entourages such that $U_{n+1} \subset U_n$. The method used in the proof of Proposition 2 of § 1, no. 4 allows us to construct, from the sequence of entourages $(U_n)$, a metric $d$ on $G$ compatible with the left uniformity of $G$; and since for each $z \in G$ the mapping $(x, y) \to (zx, zy)$ leaves each of the $U_n$ invariant, the definition of $d$ shows that it is a left-invariant metric. This method also holds for the right uniformity.

Note that, if the two uniformities of $G$ are distinct, the metric $d$ is not right-invariant, and hence in general $d(x^{-1}, y^{-1}) \neq d(x, y)$.

In particular, if $G$ is a metrizable abelian group, its uniformity is defined by an invariant metric $d$: if $G$ is written additively, we have

$$
d(x, y) = d(0, y - x) = d(0, x - y).
$$

We shall often write $|x|$ (or $||x|$) for $d(0, x)$; we have then

$$
d(x, y) = |x - y|.
$$

The function $|x|$ satisfies the following three conditions:

a) $|-x| = |x|$ for all $x \in G$.

b) $|x + y| \leq |x| + |y|$ for all $x \in G$ and all $y \in G$.

c) $|x| = 0$ if and only if $x = 0$.

Conversely:

#### Proposition 3 {#top-ix-s3-prop-3 .statement}

*Let $G$ be an abelian group, written additively, and let $x \to |x|$ be a mapping $G \to \mathbf{R}$ which satisfies conditions a), b) and c) above. Then the function $d(x, y) = |x - y|$ is an invariant metric on $G$; the topology $\mathcal{T}$ which it defines on $G$ is compatible with the group structure of $G$, and the uniformity defined by $d$ is the same as the uniformity of the topological group obtained by endowing $G$ with the topology $\mathcal{T}$.*

The function $d(x, y)$ is a metric on $G$, for the relation $d(x, y) = 0$ is equivalent to $x = y$ by c); we have $d(x, y) = d(y, x)$ by a); and

$$
d(x, y) = |(x - z) + (z - y)| \leq |x - z| + |z - y| = d(x, z) + d(z, y)
$$

by b). Moreover, $d$ is invariant, since $(x + z) - (y + z) = x - y$.
For each real number $x > 0$, let $V_x$ be the set of all $x \in G$ such that $|x| < x$; then the $V_x$ form a fundamental system $\mathfrak{S}$ of neighbourhoods of $0$ for the topology $\mathcal{T}$, and since $d$ is invariant, $a + \mathfrak{S}$ is a fundamental system of neighbourhoods of $a$ for the topology $\mathcal{T}$, for each $a \in G$. By a), the $V_x$ are symmetric, and by b), we have $V_a + V_x \subset V_{2a}$; hence the topology $\mathcal{T}$ is compatible with the group structure of $G$ (Chapter III, § 1, no. 2). The last part of the proposition follows immediately.

Conditions a', b' and c' are equivalent to c) together with the condition

$$
|x - y| \leq |x| + |y|.
$$

For a' and b' clearly imply b'); conversely, taking $x = 0$ in b') and using c), we see that $|-y| \leq |y|$; replacing $y$ by $-y$ it follows that $|-y| = |y|$, which is a); replacing $y$ by $-y$ in b') we then get b').

#### Proposition 4 {#top-ix-s3-prop-4 .statement}

*If G is a metrizable group, then every Hausdorff quotient group G/H of G is metrizable. If G is also complete, then G/H is complete (*).*

The first part of the proposition is a consequence of the fact that the identity element of G/H has a countable fundamental system of neighbourhoods in G/H; for if (V_n) is a fundamental system of neighbourhoods of e in G, then the canonical images $\dot{V}_n$ of the sets V_n in G/H form a fundamental system of neighbourhoods of the identity element of G/H (Chapter III, § 2, no. 6, Proposition 17).

To show that G/H is complete if G is complete, it is enough, by § 2, no. 6, Proposition 9, to show that every Cauchy sequence $(\dot{x}_n)$ (with respect to the left uniformity of G/H) is convergent. We may assume, by passing to a subsequence of $(\dot{x}_n)$ if necessary, that for each pair of indices $p, q$ such that $p \geq n$ and $q \geq n$, we have $\dot{x}_p^{-1}\dot{x}_q \in \dot{V}_n$; this means that for each pair of points $y \in \dot{x}_p, z \in \dot{x}_q$, we have $y^{-1}z \in HV_n = V_nH$; and therefore, for each $y \in \dot{x}_p$, the intersection of $\dot{x}_q$ and the neighbourhood $yV_n$ of $y$ is not empty. Suppose then that the sequence (V_n) has been chosen so that $V_{n+1}^2 \subset V_n$, and define inductively a sequence $(x_n)$ of points of G, such that $x_n \in \dot{x}_n$ and $x_{n+1} \in x_n V_n$; this is possible by what has been said. It follows then by induction that for each $p > 0$ we have $x_{n+p} \in x_n V_n V_{n+1} \ldots V_{n+p-1} \subset x_n V_{n-1}$. The sequence $(x_n)$ is therefore a Cauchy sequence in G, so it converges to a point $a$; and it follows immediately that the canonical image $\dot{a}$ of $a$ in G/H is the limit of the sequence $(\dot{x}_n)$.

#### Corollary 1 {#top-ix-s3-prop-4-cor-1 .statement}

*Let G be a complete metrizable group, let G_0 be a dense subgroup of G and let H_0 be a closed normal subgroup of G_0. If H is the closure of H_0 in G, the quotient group G_0/H_0 has a completion isomorphic to G/H.*

H is a normal subgroup of G (Chapter III, § 2, no. 3, Proposition 8) and Proposition 4 shows that G/H is complete. Also if $\varphi$ is the canonical mapping of G onto G/H, it is clear that $\varphi(G_0)$ is dense in G/H. The result therefore follows from Chapter III, § 2, no. 7, Proposition 21.

Let G, G' be two Hausdorff abelian topological groups, and $\hat{G}, \hat{G}'$ their respective completions. We recall (Chapter III, § 3, no. 3, Proposition 5) that if $u$ is a continuous homomorphism of G into G', then $u$ is uniformly continuous and extends uniquely to a continuous homomorphism of $\hat{G}$ into $\hat{G}'$, which we shall denote by $\hat{u}$ in the remainder

(*) There exist non-metrizable complete groups G containing a closed subgroup H such that G/H is not complete.

of this subsection. The diagram

$$
\begin{array}{ccc}
G & \xrightarrow{u} & G' \\
i \downarrow & & i' \downarrow \\
\hat{G} & \xrightarrow{\hat{u}} & \hat{G}'
\end{array}
$$

in which $i, i'$ are the canonical injections) is commutative. If $v$ is a continuous homomorphism of $G'$ into a Hausdorff abelian topological group $G''$, and if $w = v \circ u$, then it is follows immediately that $\hat{w} = \hat{v} \circ \hat{u}$.

Let $H$ be a closed subgroup of $G$ and let $E = G/H$. Let $j : H \to G$ and $p : G \to E$ be the canonical mappings. Let $\overline{H}$ be the closure of $H$ in $\hat{G}$; $\overline{H}$ is a complete group and we identify it with the completion $\hat{H}$ of $H$. The continuous extension $\hat{j}$ of $j$ to $\hat{H}$ is evidently the canonical injection of $\hat{H}$ in $\hat{G}$.

Suppose from now on that $G$ is metrizable. Then the canonical mapping of $E = GH$ into $\hat{G}\hat{H}$ is a topological isomorphism of $E$ onto a dense subgroup of the complete group $\hat{G}/\hat{H}$ (Corollary 1), and thus we may identify $\hat{G}\hat{H}$ with $\hat{E}$ and the continuous extension $\hat{p}$ of $p$ to $\hat{G}$ with the canonical mapping of $\hat{G}$ onto $\hat{G}/\hat{H}$.

#### Corollary 2 {#top-ix-s3-prop-4-cor-2 .statement}

*Let $G, G'$ be two metrizable abelian topological groups; let $u : G \to G'$ be a strict morphism with kernel $N$ and image $P$. Then $\hat{u} : \hat{G} \to \hat{G}'$ is a strict morphism with kernel $\hat{N}$ and image $\hat{P}$.*

Let $u = j \circ v \circ p$ be the canonical factorization of $u$, where $v$ is an isomorphism of the topological group $G/N$ onto the topological group $u(G) = P$. We have $\hat{u} = \hat{j} \circ \hat{v} \circ \hat{p}$, and we have seen that $\hat{p}$ is the canonical mapping of $\hat{G}$ onto $\hat{G}\hat{N}$, and that $\hat{j}$ is the canonical mapping of $\hat{P}$ into $\hat{G}$. On the other hand, $\hat{v}$ is an isomorphism of $\hat{G}/\hat{N}$ onto $\hat{P}$ (Chapter III, § 3, no. 4, Proposition 5), whence the result.

#### Corollary 3 {#top-ix-s3-prop-4-cor-3 .statement}

*Let $G, G', G''$ be three metrizable abelian topological groups and let $u : G \to G'$ and $v : G' \to G''$ be two strict morphisms such that the sequence $G \xrightarrow{u} G' \xrightarrow{v} G''$ is exact [i.e., $u(G) = \overline{v}(0)$]. Then the sequence $\hat{G} \xrightarrow{\hat{u}} \hat{G}' \xrightarrow{\hat{v}} \hat{G}''$ is exact.*

For if we put $N = u(G) = \overline{v}(0)$, it follows from Corollary 2 that $\hat{N}$ is both the image of $\hat{u}$ and the kernel of $\hat{v}$.

#### Remark 1 {#top-ix-s3-n1-rem-1 .statement}

Let $G$ be a non-Hausdorff topological group such that the Hausdorff group associated with $G$ is metrizable; equivalently, such that the identity element of $G$ has a countable fundamental system of neighbourhoods in G. The proof of Proposition 4 applies to this case without modification, H being an arbitrary normal subgroup of G, and shows that the Hausdorff group associated with G/H is metrizable, and that G/H is a complete group (in general not Hausdorff) whenever G is complete.

#### Remark 2 {#top-ix-s3-n1-rem-2 .statement}

Let d be a left-invariant metric which defines the topology of a metrizable group G, and let H be a closed normal subgroup of G. If $\dot{x}$ and $\dot{y}$ are any two points of G/H, consider the distance $d(\dot{x}, \dot{y})$ of the two closed subsets $\dot{x}, \dot{y}$ in G (\S 2, no. 2); we shall see that this function is a left-invariant metric on G/H and defines the topology of this quotient group.

Notice first that if $x \in \dot{x}$ and $y \in \dot{y}$ we have $d(\dot{x}, \dot{y}) = d(x, Hy)$; for $d(x, Hy) = \inf_{h \in H} d(x, h y)$, and therefore $d(h'x, Hy) = d(x, Hy)$ for all $h' \in H$, since d is left-invariant; this proves the assertion (\S 2, no. 2). Hence for each $\dot{z} \in G/H$ we have [\S 2, no. 2, formula (2)]

$$
|d(\dot{x}, \dot{z}) - d(\dot{y}, \dot{z})| = |d(x, \dot{z}) - d(y, \dot{z})| \leq d(x, y);
$$

and since this inequality is valid for all $x \in \dot{x}$ and all $y \in \dot{y}$, we have $|d(\dot{x}, \dot{z}) - d(\dot{y}, \dot{z})| \leq d(\dot{x}, \dot{y})$, which shows that $d(\dot{x}, \dot{y})$ is a metric on G/H. Moreover, for any $z \in \dot{z}$, we have

$$
d(\dot{z}x, \dot{z}y) = \inf_{h \in H} d(zx, hzy)
$$

from above; but since $hzy = z(z^{-1}hz) y$ and since $z^{-1}hz$ runs through H as h runs through H (H being normal), the left-invariance of $d(x, y)$ shows that we have $d(zx, Hz y) = d(x, Hy) = d(\dot{x}, \dot{y})$. Finally, if V is a neighbourhood of e in G defined by $d(e, x) < \alpha$, the image V of V in G/H is the set defined by $d(e, \dot{x}) < \alpha$; this completes the proof.

### 2. VALUED DIVISION RINGS

#### Definition 2 {#top-ix-s3-def-2 .statement}

An absolute value on a division ring K is a mapping $x \to |x|$ of K into $\mathbf{R}_+$ which satisfies the following conditions:

(VM_I) $|x| = 0$ if and only if $x = 0$.
(VM_II) $|xy| = |x| \cdot |y|$ for all $x, y$ in K.
(VM_III) $|x + y| \leq |x| + |y|$ for all $x, y$ in K.

By (VM_II) we have $|x| = |1| \cdot |x|$, and since by (VM_I) there is at least one x such that $|x| \neq 0$, we have $|1| = 1$; it follows that $1 = |1|^2$, hence $|1| = 1$ and consequently

$$
|-x| = |-1| |x| = |x|;
$$

therefore $|x - y| \leq |x| + |y|$ for all $x, y$ in K. We can therefore say that $d(x, y) = |x - y|$ is an invariant metric on the additive group K, and that the mapping $x \to |x|$ is a homomorphism of the multiplicative group $K^*$ of non-zero elements of $K$ into the multiplicative group $\mathbf{R}_+^*$ of real numbers $> 0$.

The invariant metric $|x - y|$ defines a metric space topology on $K$, compatible with its additive group structure (no. 1, Proposition 3); but, moreover, this topology is compatible with the division ring structure of $K$. For the continuity of $xy$ on $K \times K$ follows from the relation

$$
xy - x_0 y_0 = (x - x_0)(y - y_0) + (x - x_0)y_0 + x_0(y - y_0),
$$

which gives

$$
|xy - x_0 y_0| \leq |x - x_0| \cdot |y - y_0| + |x_0| \cdot |y - y_0| + |y_0| \cdot |x - x_0|.
$$

Likewise, the continuity of $x^{-1}$ at every point $x_0 \neq 0$ follows from the identity $x^{-1} - x_0^{-1} = x^{-1}(x_0 - x)x_0^{-1}$, which gives, by (VM_{II}),

$$
|x^{-1} - x_0^{-1}| = \frac{|x - x_0|}{|x_0| \cdot |x|};
$$

now if $\varepsilon > 0$ is such that $\varepsilon < |x_0|$, the relation $|x - x_0| \leq \varepsilon$ implies $|x| \geq |x_0| - \varepsilon$, whence $|x^{-1} - x_0^{-1}| \leq \varepsilon / |x_0|(|x_0| - \varepsilon)$; and this establishes the continuity of $x^{-1}$ at the point $x_0$.

#### Definition 3 {#top-ix-s3-def-3 .statement}

*A valued division ring is a division ring* $K$ *endowed with the structure defined by a given absolute value on* $K$.

A valued division ring will always be considered as endowed with the topology defined by its absolute value, which makes it a *topological* division ring. If $K_0$ is a division subring of a valued division ring $K$, the restriction to $K_0$ of the absolute value on $K$ is an absolute value on $K_0$, which defines on $K_0$ the topology induced by the topology of $K$.

#### Example 1 {#top-ix-s3-n2-exa-1 .statement}

Let $K$ be an arbitrary division ring. For each $x \in K$, put $|x| = 1$ if $x \neq 0$, and $|0| = 0$. The mapping $x \to |x|$ so defined is an absolute value on $K$, called the *improper* absolute value. The topology defined by an absolute value $|x|$ on a division ring $K$ is *discrete* if and only if $|x|$ is the improper absolute value. This condition is clearly sufficient; conversely, if the topology of $K$ is discrete, $|x|$ can take no value $\alpha > 0$ other than 1; for if we had $|x_0| = \alpha < 1$, the sequence $(x_0^n)$ would consist of non-zero terms and would converge to 0; to deal with the case $\alpha > 1$, consider $x_0^{-1}$ in place of $x_0$.

#### Example 2 {#top-ix-s3-n2-exa-2 .statement}

The absolute value of a real number (Chapter IV, § 1, no. 6) satisfies axioms (VM_I), (VM_{II}) and (VM_{III}), and the topology it defines on the field $\mathbf{R}$ is the topology of the real line. On the field $\mathbf{C}$ of complex numbers (identified with $\mathbf{R}^2$) [resp. the division ring $\mathbf{H}$ of quaternions (identified with $\mathbf{R}^4$)] the Euclidean norm is again an absolute value and defines the topology of the field $\mathbf{C}$ (resp. the division ring $\mathbf{H}$) (Chapter VIII, § 1, nos. 2 and 4).

#### Example 3 {#top-ix-s3-n2-exa-3 .statement}

On a division ring $K$, a real valuation is a function $v$ defined on $K^*$ with values in $\mathbf{R}$ which satisfies the following conditions: a) if $x \in K^*$ and $y \in K^*$, then $v(xy) = v(x) + v(y)$; b) if in addition $x + y \neq 0$, then $v(x + y) \geq \inf(v(x), v(y))$. If $a$ is any real number $> 1$, we can then define an absolute value on $K$ by putting $|x| = a^{-v(x)}$ for $x \neq 0$, and $|0| = 0$. For the relation $v(xy) = v(x) + v(y)$ for $x \neq 0$ and $y \neq 0$ implies the relation $|xy| = |x|.|y|$ for these values of $x$ and $y$, and this relation is trivially true if one of $x, y$ is zero; likewise, from the relation $v(x + y) \geq \inf(v(x), v(y))$ for $x \neq 0, y \neq 0$ and $x + y \neq 0$ we deduce $|x + y| \leq \sup(|x|, |y|) \leq |x| + |y|$, and these inequalities are still satisfied if one of $x, y, x + y$ is zero. In particular, if $v_p(x)$ is the $p$-adic valuation on the field $\mathbf{Q}$ of rational numbers (the exponent of $p$ in the decomposition of $x$ into a product of prime factors), then the corresponding absolute value $|x|_p = p^{-v_p(x)}$ is called the $p$-adic absolute value on the field $\mathbf{Q}$ (cf. Chapter III, § 6, Exercise 23).

#### Remark {#top-ix-s3-n2-rem-1 .statement}

If $x$ is a root of unity in a valued division ring, then $|x| = 1$, for $x^n = 1$ implies $|x|^n = 1$ and hence $|x| = 1$. In particular, the only absolute value on a finite field is the improper absolute value, since every element $\neq 0$ of such a field is a root of unity.

#### Definition 4 {#top-ix-s3-def-4 .statement}

Two absolute values on a division ring $K$ are said to be equivalent if they define the same topology on $K$.

#### Proposition 5 {#top-ix-s3-prop-5 .statement}

Two absolute values $|x|_1, |x|_2$ on a division ring $K$, neither of which is the improper absolute value, are equivalent if and only if the relation $|x|_1 < 1$ implies $|x|_2 < 1$. There exists then a real number $\rho > 0$ such that $|x|_2 = |x|_1^\rho$ for all $x \in K$.

The condition is necessary, for the set of all $x \in K$ such that $|x|_1 < 1$ is the same as the set of all $x$ such that, with respect to the topology defined by the absolute value $|x|_1$, $\lim_{n \to \infty} x^n = 0$.

Suppose conversely that $|x|_1 < 1 \Longrightarrow |x|_2 < 1$. Then $|x|_1 > 1 \Longrightarrow |x|_2 > 1$, because $|x^{-1}|_1 < 1$ and therefore $|x^{-1}|_2 < 1$. Since by hypothesis the absolute value $|x|_1$ is not improper, there exists $x_0 \in K$ such that $|x_0|_1 > 1$. Let $a = |x_0|_1, b = |x_0|_2$ and let $\rho = \log b / \log a > 0$. Let $x \in K^*$ and put $|x|_1 = |x_0|_1^\gamma$. If $m$ and $n$ are integers such that $n > 0$ and $m/n > \gamma$, then $|x|_1 < |x_0|_1^{m/n}$, and therefore $|x^n x_0^{-m}|_1 < 1$; hence $|x^n x_0^{-m}|_2 < 1, |x|_2 < |x_0|_2^{m/n}$. Similarly, if $m/n < \gamma$, we see that $|x|_2 > |x_0|_2^{m/n}$; it follows therefore that $|x|_2 = |x_0|_2^\gamma$; in other words

$$
\log |x|_2 = \gamma \log b = \gamma \rho \log a = \rho \log |x|_1,
$$

i.e., $|x|_2 = |x|^p_1$. It is now clear that the neighbourhoods of zero for the topologies defined on $K$ by $|x|_1$ and $|x|_2$ are identical.

Conversely, if $|x|$ is any absolute value on $K$, the function $|x|^p$ is an absolute value on $K$ (equivalent to $|x|$) for all $p$ such that $0 < p \leq 1$. We have only to verify the inequality $|x + y|^p \leq |x|^p + |y|^p$; and since $|x + y|^p \leq (|x| + |y|)^p$ it is enough to show that, if $a > 0$ and $b > 0$, we have $(a + b)^p \leq a^p + b^p$ for any $p$ such that $0 < p \leq 1$. If we put $c = a/(a + b)$ and $d = b/(a + b)$, we have $c + d = 1$, and the inequality to be proved is $c^p + d^p \geq 1$; but this follows immediately from the relations $c^p \geq c$ and $d^p \geq d$, which are valid since $0 < c \leq 1$, $0 < d \leq 1$, $0 < p \leq 1$.

Hence the set of values of $r > 0$ such that $|x|^r$ is an absolute value is a finite or infinite interval of $\mathbf{R}$ with left-hand end-point $0$; if it is finite, it is evidently closed; for if we have $|x + y|^r \leq |x|^r + |y|^r$ for any $x, y$ in $K$ and all $r$ such that $0 < r < r_0$, then by continuity the inequality is still valid for $r = r_0$. If $|x|^r$ is an absolute value for all $r > 0$, then we have
$$
|x + y| \leq (|x|^r + |y|^r)^{1/r}
$$
for all $x$ and $y$ in $K$ and all $r > 0$. Now, if $a, b$ are two real numbers $\geq 0$, we have $\lim_{r \to \infty} (a^r + b^r)^{1/c} = \sup (a, b)$; for, supposing for example that $a \geq b$, we have $a \leq (a^r + b^r)^{1/r} \leq 2^{1/r} a$, and the result follows by letting $r \to + \infty$.

Thus, if $|x|^r$ is an absolute value for all $r > 0$, we have
$$
|x + y| \leq \sup (|x|, |y|)
$$
which can be expressed by saying that $v(x) = -\log |x| \ (x \neq 0)$ is a valuation on $K$.

#### Remark {#top-ix-s3-n2-rem-2 .statement}

The proof of Proposition 5 shows that, if the topology defined by $|x|_2$ is coarser than that defined by $|x|_1$, and if $|x|_1$ is not improper, then $|x|_1$ and $|x|_2$ are equivalent, for the relation $|x|_2 < 1$ then implies $|x|_2 < 1$. Thus the topologies defined by two absolute values on $K$, neither of which is improper, cannot be comparable without being identical.

#### Proposition 6 {#top-ix-s3-prop-6 .statement}

*The completion* $\hat{K}$ *of a division ring* $K$ *endowed with an absolute value* $|x|$ *is a division ring, and the function* $|x|$ *can be extended by continuity to an absolute value on* $\hat{K}$, *which defines the topology of* $\hat{K}$.

Let $\mathfrak{F}$ be a Cauchy filter on $K$ (with respect to the additive uniformity) which does not have $0$ as a cluster point; to show that $\hat{K}$ is a division ring it is enough to establish that the image of $\mathfrak{F}$ under the mapping $x \to x^{-1}$ is a Cauchy filter base (Chapter III, § 6, no. 8, Proposition 7). Now, by hypothesis there exists a real number $\alpha > 0$ and a set $A \in \mathfrak{F}$ such that $|x| \geq \alpha$ for all $x \in A$; on the other hand, for each $\varepsilon > 0$ there exists a set $B \in \mathfrak{F}$ such that $B \subset A$ and $|x - y| \leq \varepsilon$ for all $x \in B$.

and $y \in B$; hence

$$
|x^{-1} - y^{-1}| = \frac{|x - y|}{|x| \cdot |y|} \leq \frac{\varepsilon}{a^2},
$$

and the first part of the proposition follows. The invariant metric $|x - y| = d(x, y)$ extends by continuity to a metric on $\hat{K}$ (\S 2, no. 1, Proposition 1) which defines the topology of $\hat{K}$ and is invariant by the principle of extension of identities; we continue to denote this invariant metric by $d(x, y)$. If we put $|x| = d(0, x)$ for $x \in \hat{K}$, it is clear that $|x|$ is the extension by continuity of the function $|x|$ on $K$ and is therefore an absolute value on $\hat{K}$ by the principle of extension of identities.

### 3. NORMED SPACES OVER A VALUED DIVISION RING

#### Definition 5 {#top-ix-s3-def-5 .statement}

*If E is a (left) vector space over a non-discrete valued division ring K, a norm on E is a mapping $x \to p(x)$ of E into $\mathbf{R}_+$ which satisfies the following axioms*:

(NO_I) $p(x) = 0$ if and only if $x = 0$;
(NO_{II}) $p(x + y) \leq p(x) + p(y)$ for all $x, y$ in E;
(NO_{III}) $p(tx) = |t|p(x)$ for all $t \in K$ and all $x \in E$.

The normed spaces most frequently met with have either $\mathbf{R}$ or $\mathbf{C}$ as field of scalars (with the usual absolute value).

From (NO_{III}) it follows in particular that $p(-x) = p(x)$; hence if we put $d(x, y) = p(x - y)$, $d$ is an *invariant metric* on the additive group E, and defines a metric space topology compatible with the additive group structure of E (no. 1, Proposition 3); moreover, the mapping

$$(t, x) \to tx$$

is *continuous* on $K \times E$; for we have

$$tx - t_0 x_0 = (t - t_0)(x - x_0) + (t - t_0)x + t_0(x - x_0)$$

and therefore

$$p(tx - t_0 x_0) \leq |t - t_0| p(x - x_0) + |t - t_0| p(x) + |t_0| p(x - x_0),$$

which shows that the left-hand side can be made as small as we please by taking $|t - t_0|$ and $p(x - x_0)$ sufficiently small.

Let E be a subset of K. A function $f : E \to K$ is called a normed space over K.

A normed space is endowed with the topology and the uniformity defined by its norm.

Consider a finite-dimensional division ring K. Considered as a real vector space, the absolute value $|x|$ is a norm.

The norm $\|x\| = \sqrt{\sum x_i^2}$, which we have called the Euclidean norm on the space $\mathbf{R}^n$ (Chapter VI, § 2) is evidently a norm in the sense of Definition 3. So are the functions $\sup |x_i|$ and $\sum |x_i|$.

Let $S(E; K')$ be the set of all functions $f$ on a set E which take their values in a division ring $K'$ and are such that the real-valued function $x \mapsto f(x)$ is bounded on E. This set is clearly a vector space over $K'$. Let us denote by $p(f) = \sup_{x \in E} f(x)$, then $p$ is a norm on the vector space $S(E; K')$ (cf. Chapter X, § 1).

\* 4) On the vector space $C(I; \mathbf{R})$ of all finite continuous real-valued functions defined on the interval $I = [0, 1]$ of $\mathbf{R}$, the function

$$
p(x) = \int_0^1 |x(t)| \, dt
$$

is a norm.

In a normed space E, the closed ball B with centre o and radius 1, that is the set of all $x$ such that $p(x) \leq 1$, will be called the unit ball of E. We shall show that a fundamental system of neighbourhoods of o is formed by the translations of the unit ball by the elements of K. The open ball with centre o and radius 1 is the closed ball with centre o and radius 1; hence it is enough to show that for each real number $r > 0$ there exists $k \in \mathbf{N}$ such that $0 < |k| < r$; it is sufficient to take $k = \lfloor c/r \rfloor$, where $c$ is a sufficiently large integer, in order that $|k|^2 < r$.

Let E be a normed space over a non-discrete valued field $K$.

#### Proposition 7 {#top-ix-s3-prop-7 .statement}

Two norms $p, q$ on a vector space $E$ are equivalent if and only if there exist two numbers $a > 0, b > 0$ such that

(I)
$$
a . p(x) \leq q(x) \leq b . p(x)
$$
for all $x \in E$.

These inequalities are sufficient, for it follows from the relation $a . p(x) \leq q(x)$ that, for each $r > 0$, the closed ball with centre o and radius $ar$ (relative to the norm $q$) is contained in the closed ball with centre o and radius $r$ (relative to the norm $p$); hence the topology defined by $q$ is finer than the topology defined by $p$. Similarly the inequality $q(x) \leq b . p(x)$ shows that the topology defined by $p$ is finer than that defined by $q$, and hence $p$ and $q$ are equivalent.

Let us now show that the inequalities (I) are necessary. If the topology defined by $q$ is finer than the topology defined by $p$, then the unit ball with respect to $p$ contains a closed ball with centre o and radius $\alpha > 0$ with respect to $q$; i.e., the relation $q(x) \leq \alpha$ implies $p(x) \leq 1$. If $t_0 \in K$ is such that $0 < |t_0| < 1$, then for each $x \neq o$ in $E$ there is a unique rational integer $k$ such that $\alpha |t_0| < q(t_0^k x) \leq \alpha$; therefore $p(t_0^k x) \leq 1$, so that
$$
p(x) \leq \frac{1}{|t_0|^k} \leq \frac{1}{\alpha |t_0|} q(x);
$$
putting $a = \alpha |t_0|$ we have therefore $a . p(x) \leq q(x)$ for all $x \neq o$, and this inequality is also valid when $x = o$. Similarly we show that if the topology defined by $p$ is finer than that defined by $q$, there exists $b > 0$ such that $q(x) \leq b . p(x)$.

#### Example {#top-ix-s3-n3-exa-1 .statement}

In the space $\mathbf{R}^n$, the three norms
$$
\sqrt{\sum_{i=1}^n x_i^2}, \quad \sup_{1 \leq i \leq n} |x_i| \quad \text{and} \quad \sum_{i=1}^n |x_i|
$$
are equivalent, because we have
(2)
$$
\sup_{1 \leq i \leq n} |x_i| \leq \sqrt{\sum_{i=1}^n x_i^2} \leq \sum_{i=1}^n |x_i| \leq n . \sup_{1 \leq i \leq n} |x_i|.
$$

#### Proposition 8 {#top-ix-s3-prop-8 .statement}

Let $E$ be a normed space over a non-discrete valued division ring, let $p$ be the norm on $E$, and let $\hat{E}$ be the additive topological group which is the completion of the additive group $E$. Then the function $(t, x) \to tx$ can be extended by continuity to $\hat{K} \times \hat{E}$ and defines on $\hat{E}$ a vector space structure over $\hat{K}$; the norm $p$ can be extended by continuity to a norm $\bar{p}$ on $\hat{E}$ which defines the topology of $\hat{E}$.

The extension of $tx$ by continuity is a particular case of the theorem of extension of a continuous bilinear mapping of a product of two abelian groups into a third (Chapter III, § 6, no. 5, Theorem 1); we have $1.x = x$ and $t(u x) = (t u)x$ for $t \in \hat{K}$, $u \in \hat{K}$ and $x \in \hat{E}$, by the principle of extension of identities; hence the external law $(t, x) \to t x$ indeed defines on $\hat{E}$ a structure of a vector space over $\hat{K}$. On the other hand, the invariant metric $\overline{d}(x, y) = \overline{p}(x - y)$ extends to an invariant metric $\overline{d}$ on $\hat{E}$ (\S 2, no. 1, Proposition 1) which defines the topology of $\hat{E}$; if we set $\overline{p}(x) = \overline{d}(0, x)$, then $\overline{p}$ is the extension of $p$ by continuity, and satisfies axioms (NO_I) and (NO_{II}); by virtue of the continuity of $t x$ on $\hat{K} \times \hat{E}$, $\overline{p}$ also satisfies (NO_{III}) (principle of extension of identities) and is therefore a norm on $\hat{E}$.

When we have to consider a definite normed space structure on a vector space $E$, we shall usually denote the norm of a vector $x$ by $||x||$, unless this notation is likely to lead to confusion.

### 4. QUOTIENT SPACES AND PRODUCT SPACES OF NORMED SPACES

#### Proposition 9 {#top-ix-s3-prop-9 .statement}

*Let $E$ be a normed space over a non-discrete valued division ring $K$, and let $H$ be a closed vector subspace of $E$. If, for each class $\dot{x} \in E/H$, we put $||\dot{x}|| = \inf_{x \in \dot{x}} ||x||$, the function $||\dot{x}||$ is a norm on the vector space $E/H$, and the topology defined by this norm is the quotient by $H$ of the topology of $E$.*

By Remark 2 of no. 1, $d(\dot{x}, \dot{y}) = ||\dot{x} - \dot{y}||$ is an invariant metric on $E/H$ which defines the quotient by $H$ of the topology of $E$. It remains only to show that $||t \dot{x}|| = |t| \cdot ||\dot{x}||$, and this follows immediately from the definition of $||\dot{x}||$ [Chapter IV, § 5, no. 7, formula (23)].

The norm $||\dot{x}||$ may also be interpreted as follows: it is the distance (in $E$) *of every point* $x \in \dot{x}$ *from the subspace* $H$, for the points of $\dot{x}$ are the points $x - z$, where $z$ runs through $H$.

#### Proposition 10 {#top-ix-s3-prop-10 .statement}

*Let $(E_i)_{1 \leq i \leq n}$ be a finite family of normed spaces over a non-discrete valued division ring $K$, and let $E = \prod_{i=1}^n E_i$ be the product vector space. If for each $x = (x_i) \in E$ we put $||x|| = \sup_{1 \leq i \leq n} ||x_i||$, then the function $||x||$ is a norm on $E$, and the topology it defines on $E$ is the product of the topologies of the $E_i$.

For if $x = (x_i)$ and $y = (y_i)$, we have $x + y = (x_i + y_i)$ and therefore
$$
||x + y|| = \sup_i ||x_i + y_i|| \leq \sup_i (||x_i|| + ||y_i||)
\leq \sup_i ||x_i|| + \sup_i ||y_i|| = ||x|| + ||y||.
$$

On the other hand, it is clear that $||tx|| = |t|.||x||$, and that if $||x|| = 0$, then $||x_i|| = 0$ and therefore $x_i = 0$ for $1 \leq i \leq n$, so that $x = 0$; hence $||x||$ is a norm on $E$. Also the relation $||x|| < a$ is equivalent to the $n$ relations $||x_i|| < a$, and therefore the norm $||x||$ defines the product topology on $E$.

Similarly we can show that the functions $\sum_{i=1}^n ||x_i||$ and $\sqrt{\sum_{i=1}^n ||x_i||^2}$ are norms on $E$; the inequalities (2) show that all three norms are *equivalent*.

In particular, in the (left or right) vector space $K^n$, if we put

$$
p_1(x) = \sup_i |x_i|, \quad p_2(x) = \sum_{i=1}^n |x_i|, \quad p_3(x) = \sqrt{\sum_{i=1}^n |x_i|^2}
$$

for $x = (x_i)_{1 \leq i \leq n}$, then the three functions $p_1, p_2, p_3$ are equivalent norms which define on $K^n$ the topology which is the product of the topologies of the factors $K$.

### 5. CONTINUOUS MULTILINEAR FUNCTIONS

#### Theorem 1 {#top-ix-s3-thm-1 .statement}

*Let $E_i (1 \leq i \leq n)$ and $F$ be normed spaces over a non-discrete valued division ring $K$, and let $f$ be a multilinear mapping of $\prod_{i=1}^n E_i$ into $F$. Then $f$ is continuous on $\prod_{i=1}^n E_i$ if and only if there exists a real number $a > 0$ such that, for all $x_i \in E_i \ (1 \leq i \leq n)$, we have*

$$
||f(x_1, x_2, \ldots, x_n)|| \leq a . ||x_1|| . ||x_2|| \ldots ||x_n||
$$

(3)

The condition is *necessary*. For if $f$ is continuous at the point $(0, 0, \ldots, 0)$ there exists a number $b > 0$ such that the relations $||x_i|| \leq b \ (1 \leq i \leq n)$ imply $||f(x_1, \ldots, x_n)|| \leq 1$. Let $t_0$ be an element of $K$ such that $0 < |t_0| < 1$; then for *every* point $(x_i) \in \prod_{i=1}^n E_i$ such that none of the $x_i$ is zero, there exist $n$ rational integers $k_i$ such that $b|t_0| < ||t_0^{k_i} x_i|| \leq b$; consequently we have

$$
|t_0|^{k_1 + k_2 + \cdots + k_n} ||f(x_1, x_2, \ldots, x_n)|| \leq 1;
$$

on the other hand we have $\frac{1}{|t_0|^{k_i}} \leq \frac{1}{b|t_0|} ||x_i||$, and the relation (3) therefore follows, with $a = (1/b|t_0|)^n$. This relation is evidently still valid when one of the $x_i$ is zero.

The condition is sufficient. We shall show that, if it is satisfied, $f$ is continuous at every point $(a_i)$ of $\prod_{i=1}^n E_i$. We can write

$$
f(x_1, \ldots, x_n) - f(a_1, \ldots, a_n) = \sum_{i=1}^n f(a_1, \ldots, a_{i-1}, x_i - a_i, x_{i+1}, \ldots, x_n).
$$

Now, using (3), the conditions $||x_i - a_i|| \leq r$ ($1 \leq i \leq n$) imply that

$$
||f(a_1, \ldots, a_{i-1}, x_i - a_i, x_{i+1}, \ldots, x_n)|| \leq ar \prod_{k \neq i}^n (||a_k|| + r);
$$

hence, if $c$ is the maximum of the numbers $||a_i||$ ($1 \leq i \leq n$), we have

$$
||f(x_1, \ldots, x_n) - f(a_1, \ldots, a_n)|| \leq nar (c + r)^{n-1}.
$$

Since the right-hand side of this inequality is a polynomial in $r$ with zero constant term, it tends to 0 as $r$ tends to 0; hence $f$ is continuous.

#### Remark {#top-ix-s3-n5-rem-1 .statement}

Two of the propositions proved earlier are consequences of this theorem: the continuity of the bilinear function $tr$, by virtue of the relation $xr = t \cdot x$; and Proposition 7, by applying Theorem 1 to the identity mapping of $E$, considered as a linear mapping of the space $E$, endowed with the norm $p$ into the space $E$ endowed with the norm $q$ (or vice versa).

### 6. ABSOLUTELY SUMMABLE FAMILIES IN A NORMED SPACE

#### Definition 8 {#top-ix-s3-def-8 .statement}

In a normed space $E$, a family $(x_i)$ of points of $E$ is said to be absolutely summable if the family $(||x_i||)$ of norms of the $x_i$ is summable in $\mathbf{R}$.

This concept appears to depend on the norm chosen on $E$; but by Proposition 7 of no. 3 and the comparison principle for summable families of real numbers, a family which is absolutely summable with respect to a norm $p$ on $E$ is absolutely summable with respect to any norm on $E$ which is equivalent to $p$.

If $(x_i)_{i \in I}$ is a family of points of $E$ which is summable and absolutely summable, we have

$$
\left\| \sum_{i \in I} x_i \right\| \leq \sum_{i \in I} \|x_i\|.
$$

Indeed, for each finite subset $J$ of $I$ we have $\left\| \sum_{i \in J} x_i \right\| \leq \sum_{i \in J} \|x_i\|$, and the inequality (4) follows by passing to the limit with respect to the directed set of finite subsets of $I$.

#### Proposition 11 {#top-ix-s3-prop-11 .statement}

In a complete normed space E, every absolutely summable family is summable.

For if $(x_i)$ is an absolutely summable family in E, then for each $\varepsilon > 0$ there is a finite subset J of the index set I such that, for each finite subset H of I which does not meet J, we have $\sum_{i \in H} ||x_i|| \leq \varepsilon$; hence *a fortiori* $\left\| \sum_{i \in H} x_i \right\| \leq \varepsilon$, and this proves the proposition, since E is complete (Cauchy’s criterion, Chapter III, § 5, no. 2, Theorem 1).

A series whose general term is $x_n$ is said to be *absolutely convergent* in E if the series whose general term is $||x_n||$ is convergent in $\mathbf{R}$, or (equivalently) if the family $(x_n)$ is absolutely summable; consequently (Chapter III, § 5, no. 7, Proposition 9):

#### Corollary {#top-ix-s3-n6-cor-1 .statement}

In a complete normed space E, every absolutely convergent series is *commutatively convergent*.

The converse of Proposition 11 is in general *false*.

Consider for example the space $\mathcal{B}(\mathbf{N}; \mathbf{R})$ of bounded sequences $x = (x_n)_{n \in \mathbf{N}}$ of real numbers, with the norm $||x|| = \sup_n |x_n|$. Let $x_m$ be the sequence $(x_{mn})_{n \in \mathbf{N}}$ such that $x_{mn} = 0$ if $m \neq n$ and $x_{mm} = 1/m$ for $m \geq 1$. It is immediately verified that the sequence $(x_m)_{m \in \mathbf{N}}$ is summable in $\mathcal{B}(\mathbf{N}; \mathbf{R})$ and that its sum is the element $y = (y_n)$ such that $y_0 = 0$ and $y_n = 1/n$ if $n \geq 1$; but since $||x_m|| = 1/m$, the sequence of norms of the $x_m$ is not summable in $\mathbf{R}$.

However, we have seen in Chapter VII, § 3, no. 1, that every summable family in $\mathbf{R}^n$ is absolutely summable.

### 7. NORMED ALGEBRAS OVER A VALUED FIELD

#### Definition 9 {#top-ix-s3-def-9 .statement}

*If A is an algebra over a non-discrete valued field K, a norm $p(x)$ on A (A being considered as a vector space over K) is said to be compatible with the algebra structure of A if the topology it defines is compatible with the ring structure of A. An algebra over K, endowed with the structure defined by a norm compatible with the algebra structure, is called a normed algebra.*

If A is a normed algebra over K, and if $p(x)$ is the norm on A, the bilinear mapping $(x, y) \to xy$ of $A \times A$ into A is continuous, by hypothesis; hence by Theorem 1 of no. 5 there exists a real number $a > 0$ such that $p(xy) \leq a \cdot p(x)p(y)$. Replacing $p(x)$ by the equivalent norm $a \cdot p(x)$, we may therefore always assume that the norm $||x||$ on a normed algebra A is such that

$$
||xy|| \leq ||x|| \cdot ||y||.
$$

It follows from (5) by induction that, for each integer $n > 0$, we have

$$
||x^n|| \leq ||x||^n.
$$

#### Example 1 {#top-ix-s3-n7-exa-1 .statement}

Let $K$ be a valued division ring and let $K'$ be a subfield of the centre of $K$ such that the trace on $K'$ of the absolute value $|x|$ of $K$ is not the improper absolute value on $K'$. Then $K$, with $|x|$ as norm, is a normed algebra over $K'$.

#### Example 2 {#top-ix-s3-n7-exa-2 .statement}

Let $K$ be a non-discrete valued field and let $M_n(K)$ be the ring of square matrices of order $n$ over $K$. Regarded as a vector space over $K$, $M_n(K)$ is isomorphic to $K^{n^2}$. If for each $X = (x_{ij}) \in M_n(K)$ we define $\|X\| = \sup_{i,j} |x_{ij}|$, then $\|X\|$ is a norm on $M_n(K)$, and the topology defined by this norm is the product topology on $K^{n^2}$ (Proposition 10); from this it follows (because of the continuity of polynomials in any number of variables over $K$) that this norm is compatible with the $K$-algebra structure of $M_n(K)$.

#### Example 3 {#top-ix-s3-n7-exa-3 .statement}

The set $\mathcal{B}(X; K)$ of all functions $f$ on a set $X$ with values in a non-discrete valued field $K$, such that $x \to |f(x)|$ is bounded on $X$, is an algebra over $K$; the norm $\|f\| = \sup_{x \in X} |f(x)|$ is compatible with the ring structure of $\mathcal{B}(X; K)$, because we have $\|fg\| \leq \|f\|\cdot\|g\|$ (cf. Chapter X, § 1).

Let $a$ be a closed two-sided ideal in a normed algebra $A$. If in the quotient algebra $A/a$ we put $||\dot{x}|| = \inf_{x \in X} ||x||$, we get a norm on $A/a$ which defines the topology which is the quotient by $a$ of the topology of $A$ (Proposition 9); since this quotient topology is compatible with the quotient ring structure of $A/a$ (Chapter III, § 6, no. 4) it follows that the quotient algebra $A/a$, with the norm $||x||$, is a normed algebra.

Likewise, if $(A_i)_{1 \leq i \leq n}$ is a family of $n$ normed algebras over a valued field $K$, and if in the product algebra $A = \prod_{i=1}^n A_i$ we put $||x|| = \sup_i ||x_i||$, where $x = (x_i)$, we have a norm on $A$ which defines the product of the topologies of the $A_i$ (Proposition 10); since this topology is compatible with the ring structure of $A$ (Chapter III, § 6, no. 4), it follows that the product algebra $A$, with the norm $||x||$, is a normed algebra.

Let $A$ be a normed algebra over a valued field $K$. The completion $\hat{A}$ of $A$ (Chapter III, § 6, no. 5, Proposition 6) is also endowed with a $\hat{K}$-vector space structure (no. 3, Proposition 8), and it is clear from the principle of extension of identities that we have $t(xy) = (tx)y = x(ty)$ for all $t \in \hat{K}$ and all $x, y \in \hat{A}$. Hence $\hat{A}$ is an algebra over $\hat{K}$; on the other hand (no. 3, Proposition 8), the norm on $A$ extends by continuity to a norm which defines the topology of $\hat{A}$, and therefore $\hat{A}$, endowed with this norm, is a *normed algebra* over the field $\hat{K}$.

If $(x_\lambda)_{\lambda \in L}$ and $(y_\mu)_{\mu \in M}$ are two absolutely summable families in a normed algebra $A$, the family $(x_\lambda y_\mu)_{(\lambda, \mu) \in L \times M}$ is absolutely summable, because $||x_\lambda y_\mu|| \leq ||x_\lambda|| \cdot ||y_\mu||$ (Chapter IV, § 7, no. 3, Proposition 1); if in addition $A$ is complete, all three families are summable and we have
$$
\sum_{(\lambda, \mu) \in L \times M} x_\lambda y_\mu = \left( \sum_{\lambda \in L} x_\lambda \right) \left( \sum_{\mu \in M} y_\mu \right)
$$
by the associativity of the sum on the left-hand side (Chapter III, § 5, no. 3, formula (2)).

If the normed algebra $A$ has an identity element $e \neq 0$, the mapping $t \to te$ is an isomorphism of the field structure of $K$ onto that of the subfield $Ke$ of $A$; this isomorphism is also an isomorphism of the topological field structure of $K$ onto that of $Ke$ (the topology of the latter being induced by that of $A$), for the restriction $||te||$ of the norm of $A$ to $Ke$ is a norm equivalent to the absolute value
$$
|t| = \frac{1}{||e||} ||te||.
$$
If $||e|| = 1$ we have $||te|| = |t|$, and we can then identify the valued field $K$ with the normed subfield $Ke$ of $A$, and in particular we may denote the identity element of $A$ by the symbol 1.

In what follows we shall be concerned only with normed algebras which have an identity element $e$, and in which the norm satisfies the inequality (5); putting $x = y = e$ in this inequality, it follows that $||e|| \geq 1$.

#### Proposition 12 {#top-ix-s3-prop-12 .statement}

*If the series whose general term is $z^n$ is convergent in $A$, then $e - z$ is a unit of $A$ and we have*
$$
(e - z)^{-1} = \sum_{n=0}^\infty z^n.
$$
*Conversely, if $||z|| < 1$ and if $e - z$ is a unit in $A$, then the series whose general term is $z^n$ is convergent and formula (7) is valid.*

For each $p > 0$ we have
$$
(e - z) \sum_{n=0}^p z^n = e - z^{p+1}.
$$
If the series whose general term is $z^n$ is convergent and if $y$ is its sum, then $z^n$ tends to 0 as $n \to + \infty$; hence by passing to the limit in (8) we have $(e - z)y = e$; similarly we prove that $y(e - z) = e$, and hence $y = (e - z)^{-1}$ (note that this part of the argument is valid in any topological ring which has an identity element).

Conversely, if $||z|| < 1$, then since $||z^{p+1}|| \leq ||z||^{p+1}$, it follows that $z^{p+1}$ tends to 0 as $p \to +\infty$; multiplying both sides (8) on the left by $(e-z)^{-1}$ and letting $p$ tend to infinity, we see that the series whose general term is $z^n$ converges and has $(e-z)^{-1}$ as its sum.

#### Corollary {#top-ix-s3-n7-cor-1 .statement}

*Let A be a complete normed algebra. Then for each $z \in A$ such that $||z|| < 1$, $e - z$ is a unit in A.*

The series whose general term is $z^n$ is absolutely convergent, since $||z^n|| \leq ||z||^n$ for $n > 0$, and is therefore convergent, since A is complete (no. 6, Proposition 11).

#### Proposition 13 {#top-ix-s3-prop-13 .statement}

*Let G be the group of units of a complete normed algebra A. Then G is an open subset of A; the topology induced on G by the topology of A is compatible with the group structure of G; and G, endowed with this topology, is a complete group* (with respect to each of its two uniformities).

The corollary to Proposition 12 shows that G contains a neighbourhood V of $e$ in A; hence, for each $x_0 \in G$, the elements of $x_0V$ are units, and $x_0V$ is a neighbourhood of $x_0$ in A, since $x \mapsto x_0x$ is a homeomorphism of A onto itself ($x_0$ being a unit of A). Hence G is open in A.

To show that the topology induced on G by the topology of A is compatible with the group structure of G, it is sufficient to show that the function $x^{-1}$ is *continuous* on G. Let $x_0 \in G$, and for each $x \in G$, write $x$ in the form $x = x_0(e + u)$, so that $u = x_0^{-1}(x - x_0)$; then $||u|| \leq ||x_0^{-1}|| \cdot ||x - x_0||$, and thus if $||x - x_0|| \leq 1 / ||x_0^{-1}||$, we have $||u|| \leq 1$, $e + u = x_0^{-1}x$ is a unit, the series whose general term is $(-1)^n u^n$ is absolutely convergent, and

$$
x^{-1} = (e + u)^{-1} x_0^{-1} = x_0^{-1} + \left( \sum_{n=1}^{\infty} (-1)^n u^n \right) x_0^{-1},
$$

from which it follows that

$$
||x_0^{-1} - x_0^{-1}|| \leq \left| \left| \sum_{n=0}^{\infty} (-1)^n u^n \right| \right| \cdot ||u|| \cdot ||x_0^{-1}|| \\
\leq \left| \left| \sum_{n=0}^{\infty} (-1)^n u^n \right| \right| \cdot ||x_0^{-1}|^2 \cdot ||x - x_0||.
$$

As $x$ tends to $x_0$, $||x - x_0||$ tends to 0, and since

$$
\left| \left| \sum_{n=0}^{\infty} (-1)^n u^n \right| \right| \leq ||e|| + \frac{||u||}{1 - ||u||}
$$

remains bounded, it follows that $x^{-1}$ tends to $x_0^{-1}$.

Finally, to show that the left uniformity of G is complete, let us show that every Cauchy filter $\tilde{\mathcal{F}}$ with respect to this uniformity is a Cauchy filter with respect to the *additive* uniformity of $A$ and converges to a point of $G$. For each $\varepsilon$ such that $0 < \varepsilon < 1$, there is a set $M \in \mathfrak{F}$ such that $||x^{-1}y - e|| \leq \varepsilon$ for all $x, y$ in $M$, i.e., such that
$$
||y - x|| \leq \varepsilon \ ||x||.
$$
Let $a$ be a point of $M$; for each $x \in M$ we have $||x - a|| \leq \varepsilon \ ||a||$, and therefore $||x|| \leq (1 + \varepsilon)||a||$. On the other hand, there exists a set $N \subset M$ belonging to $\mathfrak{F}$ and such that $||x^{-1}y - e|| \leq \varepsilon/(1 + \varepsilon)||a||$ for all $x$ and $y$ in $N$; it follows that $||y - x|| \leq \varepsilon ||x||/(1 + \varepsilon)||a|| \leq \varepsilon$, which shows that $\mathfrak{F}$ is a Cauchy filter with respect to the additive uniformity of $A$, and therefore converges to a point $x_0$, since $A$ is complete. Since $x_0$ is the limit of $\mathfrak{F}$, we have $||x^{-1}x_0 - e|| \leq \varepsilon$ for all $x \in M$ by the principle of extension of inequalities; since $\varepsilon > 1$, it follows that $x^{-1}x_0$ is a unit in $A$; hence $x_0$ is a unit, i.e., $x_0 \in G$.

#### Proposition 14 {#top-ix-s3-prop-14 .statement}

*In a complete valued division ring, the multiplicative group of non-zero elements is a complete group.*

The proof is similar to that of Proposition 13; we have only to replace the norm of $A$ by the absolute value of the division ring under consideration.

Note that we cannot apply Proposition 13 directly, because a (non-commutative) valued division ring is not necessarily an algebra over a *non-discrete* valued field (the restriction of the absolute value to the centre of the division ring might be improper).

#### Remark {#top-ix-s3-n7-rem-1 .statement}

Proposition 13 is not necessarily true for a non-complete normed algebra. For example, in the algebra $C(I; \mathbf{R})$ of all finite continuous real-valued functions on $I = [0, 1]$ [the norm being $||x|| = \sup_{t \in I} |x(t)|$], the subalgebra $P$ of all *polynomials* in $t$ (restricted to $I$) is *not* complete; if $x(t)$ is any non-constant polynomial, then $1 + \varepsilon x$ is arbitrarily close to the identity element 1 of $P$ when $\varepsilon$ is arbitrarily small, but $1 + \varepsilon x$ is not a unit *in* $P$. However, if $A$ is a non-complete normed algebra, $G$ its group of units, $\hat{A}$ the completion of $A$, then $G$ is a subgroup of the group of units of $\hat{A}$, and therefore the topology induced on $G$ by the topology of $A$ is compatible with the group structure of $G$.

### Exercises {#top-ix-s3-exercises}

See the [exercises for § 3](exercises/s3/).
