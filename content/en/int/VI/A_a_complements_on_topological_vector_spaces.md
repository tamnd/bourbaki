---
book: int
book_title: Integration
chapter: VI
chapter_title: VECTORIAL INTEGRATION
section: 0
section_title: Complements on topological vector spaces
appendix: true
lang: en
source: int-i-vi
pdf_pages: 0443-0447
extraction: ocr
subsections:
    - "no": 1
      title: Bilinear forms and linear mappings
      page: 0
      pdf_page: 443
    - "no": 2
      title: Some types of spaces having the property (GDF)
      page: 54
      pdf_page: 445
statements: 6
exercises: 0
content_sha256: 8240c45f1ffa0d8d8e08d1eb351824879072712524201a0c8f5557c34643b259
---

## APPENDIX

# Complements on topological vector spaces

### 1. Bilinear forms and linear mappings

Let $(F_1, G_1), (F_2, G_2)$ be two pairs of (real or complex) vector spaces in separating duality (TVS, II, §6, No. 1); assume each of these spaces to be equipped with the corresponding weak topology (*loc. cit.*, No. 2); if A and B are any two of these spaces, as usual we denote by $\mathcal{L}(A; B)$ the vector space of continuous linear mappings of A into B, and by $\mathfrak{B}(A, B)$ the vector space of *separately continuous* bilinear forms on $A \times B$.

For every separately continuous bilinear form $\Phi$ on $F_1 \times F_2$, $x_1 \mapsto \Phi(x_1, x_2)$ is a continuous linear form on $F_1$, therefore there exists one and only one element ${}^r\Phi(x_2) \in G_1$ such that

$$
\Phi(x_1, x_2) = \langle x_1, {}^r\Phi(x_2) \rangle
$$

for $x_1 \in F_1, x_2 \in F_2$ (TVS, III, §5, No. 1, (1)). Moreover, this formula shows that the mapping $x_2 \mapsto {}^r\Phi(x_2)$ is linear and continuous for the (weak) topologies of $F_2$ and $G_1$. Conversely, for every continuous linear mapping $u$ of $F_2$ into $G_1$, $(x_1, x_2) \mapsto \Phi(x_1, x_2) = \langle x_1, u(x_2) \rangle$ is a separately continuous bilinear form on $F_1 \times F_2$, and ${}^r\Phi = u$. One thus defines an isomorphism $r : \Phi \mapsto {}^r\Phi$ of $\mathfrak{B}(F_1, F_2)$ onto $\mathcal{L}(F_2; G_1)$, said to be *canonical*.

Similarly, the formula

$$
\Phi(x_1, x_2) = \langle {}^l\Phi(x_1), x_2 \rangle
$$

defines a *canonical isomorphism* $l : \Phi \mapsto {}^l\Phi$ of $\mathfrak{B}(F_1, F_2)$ onto $\mathcal{L}(F_1; G_2)$; and one obviously has the commutative diagram

$$
\begin{array}{ccc}
\mathcal{B}(F_1, F_2) & & \\
l & l^{-1} & r^{-1} \\
& & \\
\mathcal{L}(F_1; G_2) & \xleftarrow{t} & \mathcal{L}(F_2; G_1)
\end{array}
$$

where $t$ is the isomorphism of transposition $u \mapsto {}^t u$. In view of the definition of the weak topologies on $G_1$ and $G_2$, it is moreover immediate that when $\mathcal{B}(F_1, F_2)$, $\mathcal{L}(F_1; G_2)$ and $\mathcal{L}(F_2; G_1)$ are equipped with the topology of pointwise convergence, the isomorphisms in the preceding diagram are isomorphisms for the topological vector space structures.

Now let $E, F$ be two Hausdorff locally convex spaces, $E', F'$ their respective duals; we denote by $E_\sigma, F_\sigma$ the spaces $E, F$ equipped with the weakened topologies $\sigma(E, E')$, $\sigma(F, F')$, and by $E'_s, F'_s$ the spaces $E', F'$ equipped with the weak topologies $\sigma(E', E)$, $\sigma(F', F)$. Thus, the preceding remarks establish canonical isomorphisms between the three spaces $\mathcal{B}(E_\sigma, F'_s)$, $\mathcal{L}(E_\sigma; F_\sigma)$ and $\mathcal{L}(F'_s; E'_s)$, and also between the three spaces $\mathcal{B}(E_\sigma, F_\sigma)$, $\mathcal{L}(E_\sigma; F'_s)$ and $\mathcal{L}(F_\sigma; E'_s)$. One will observe that $\mathcal{B}(E_\sigma, F_\sigma)$ is also equal to the space $\mathcal{B}(E, F)$ of separately continuous bilinear forms on $E \times F$ ($E$ and $F$ being equipped with their original topologies), since every continuous linear form on $E$ (resp. $F$) is continuous on $E_\sigma$ (resp. $F_\sigma$) and conversely (TVS, II, §6, No. 1 and No. 2, Prop. 3).

Let $\mathcal{B}(E, F)$ be the space of continuous bilinear forms on $E \times F$ ($E$ and $F$ being equipped with their original topologies); then $\mathcal{B}(E, F) \subset \mathcal{B}(E, F)$.

#### Proposition 1 {#int-vi-a0-prop-1 .statement}

*For a bilinear form $\Phi \in \mathcal{B}(E, F)$ to belong to $\mathcal{B}(E, F)$, it is necessary and sufficient that there exist a neighborhood of 0 in $E$ whose image under ${}^l \Phi$ is an equicontinuous subset of $F'$.*

For, to say that $\Phi$ is continuous means that there exists a balanced convex neighborhood $V$ (resp. $W$) of 0 in $E$ (resp. $F$) such that $|\Phi(x, y)| \leq 1$ for $x \in V$, $y \in W$; this may be written $|\langle {}^l \Phi(x), y \rangle| \leq 1$ for $x \in V$, $y \in W$, or also ${}^l \Phi(V) \subset W^\circ$; whence the proposition, taking into account the fact that every equicontinuous subset of $F'$ is contained in the polar of a neighborhood of 0 in $F$.

#### Corollary {#int-vi-a0-n1-cor-1 .statement}

*If $\Phi$ is a continuous bilinear form on $E \times F$, then ${}^l \Phi$ is a continuous linear mapping of $E$ into the strong dual $F'_b$ of $F$. If, moreover, $E$ and $F$ are normed spaces, then $\|{}^l \Phi\| = \|\Phi\|$.*

The first assertion follows from Prop. 1 and the fact that every neighborhood of 0 in $F'_b$ absorbs every equicontinuous subset of $F'$. If $E$ and $F$ are normed, then

$$
\|\Phi\| = \sup_{\|x\| \leq 1, \|y\| \leq 1} |\Phi(x, y)| = \sup_{\|x\| \leq 1} \left( \sup_{\|y\| \leq 1} |\langle l \Phi(x), y \rangle| \right)
= \sup_{\|x\| \leq 1} \|l \Phi(x)\| = \|l \Phi\|,
$$

whence the second assertion.

Interchanging the roles of E and F, one obtains results analogous to Prop. 1 and its corollary for the linear mappings $r \Phi$; we leave to the reader the task of stating them.

### 2. Some types of spaces having the property (GDF)

We already know that every Fréchet space has the property (GDF) (TVS, I, §3, No. 3, Cor. 5 of Th. 1).

#### Proposition 2 {#int-vi-a0-prop-2 .statement}

— Let E be a vector space, $(F_\alpha)_{\alpha \in A}$ a family of locally compact spaces having the property (GDF), and for each $\alpha \in A$ let $h_\alpha$ be a linear mapping of $F_\alpha$ into E. If E is equipped with the finest locally convex topology that makes the $h_\alpha$ continuous, then E has the property (GDF).

Let $u$ be a linear mapping of E into a Banach space B, such that every limit in $E \times B$ of every convergent sequence of points of the graph $\Gamma$ of $u$ also belongs to $\Gamma$. It suffices to show that, for every $\alpha \in A$, $u \circ h_\alpha$ is continuous on $F_\alpha$ (TVS, II, §4, No. 4, Prop. 5). Now, let $(x_n)$ be a sequence of elements of $F_\alpha$ having a limit $a$ and such that the sequence $\left(u(h_\alpha(x_n))\right)$ has a limit $b \in B$. Since $h_\alpha$ is continuous, $h_\alpha(a)$ is a limit of the sequence $(h_\alpha(x_n))$ in E; therefore by hypothesis $b = u(h_\alpha(a))$ and, since $F_\alpha$ has the property (GDF), $u \circ h_\alpha$ is continuous.

#### Corollary {#int-vi-a0-n2-cor-1 .statement}

— Every quotient space of a locally convex space having the property (GDF) has the property (GDF).

#### Proposition 3 {#int-vi-a0-prop-3 .statement}

— The strong dual of a reflexive Fréchet space has the property (GDF).

This is a consequence of Prop. 2 and the following lemma (or TVS, IV, §3, No. 4, Prop. 4):

#### Lemma {#int-vi-a0-n2-lem-1 .statement}

Let F be a Fréchet space, $F'$ its strong dual, $F''$ its bidual. If every subset of $F''$, bounded for $\sigma(F'', F')$, is contained in the closure (for $\sigma(F'', F')$) of a bounded subset of F, then $F'$ is the direct limit of a sequence of Banach spaces.

For, let $(V_n)$ be a decreasing fundamental sequence of convex, balanced and closed neighborhoods of 0 in F. For every integer $n$, let $G_n$ be the linear subspace of $F'$ generated by the polar $V_n^\circ$ of $V_n$. In $G_n$, $V_n^\circ$ is an absorbent convex set, therefore its gauge $p_n$ is a norm on $G_n$; moreover, $V_n^\circ$ is a complete subset of the strong dual $F'$ (TVS, III, §3, No. 8, Prop. 11); thus $G_n$, equipped with the norm $p_n$, is a Banach space (GT, III, §3, No. 5, Cor. 2 of Prop. 9). We are going to show that the strong topology on $F'$ is the direct limit of these Banach space topologies on the $G_n$, or again that, for a strongly closed, balanced, convex subset U of $F'$ to be a strong neighborhood of 0, it is necessary and sufficient that it absorb each of the $V_n^\circ$. It is obvious that this condition is necessary; to see that it is sufficient, it will suffice to prove that U contains a barrel of $F'$. Indeed, its polar $U^\circ$ in $F''$ will then be bounded for $\sigma(F'', F')$, hence, by hypothesis, will be contained in the closure (for $\sigma(F'', F')$) of a bounded subset B of F, from which one can conclude that U (which is closed for $\sigma(F', F'')$) contains the strong neighborhood $B^\circ$ of 0 (TVS, II, §6, No. 3, Th. 1 and §8, No. 4).

By hypothesis, for every integer $n$ there exists a number $\lambda_n > 0$ such that $\lambda_n V_n^\circ \subset \frac{1}{2}U$; let $A_n$ be the convex envelope of the union of the $\lambda_i V_i^\circ$ for $i \leq n$. Then $A_n \subset \frac{1}{2}U$ for every $n$; let W be the union of the $A_n$; W is a convex, balanced, absorbent set contained in $\frac{1}{2}U$, and it will suffice to show that its strong closure (which is a barrel) is contained in U.

Thus, let $x'$ be a point of $F'$ not belonging to U. Since each of the $V_n^\circ$ is compact for $\sigma(F', F)$, the same is true of the $A_n$ (TVS, II, §2, No. 6, Prop. 15), and since $x' \notin 2A_n$, there exists an element $x_n$ belonging to the polar of $A_n$ in F such that $\langle x', x_n \rangle = 2$ (TVS, II, §5, No. 3, Prop. 4). The sequence $(x_n)$ is bounded in F: for, every $y' \in F'$ belongs to some $V_k^\circ$, consequently $|\langle y', x_n \rangle| \leq \lambda_k^{-1}$ for $n \geq k$, whence our assertion (TVS, IV, §1, No. 1, Prop. 1). Let C be a bounded, balanced convex set in F containing all the $x_n$; $C^\circ$ is then a neighborhood of 0 in $F'$, and the polar $C^{\circ\circ}$ of $C^\circ$ in $F''$ is compact for $\sigma(F'', F')$ (TVS, III, §3, No. 4, Cor. 2 of Prop. 4 and No. 5, Prop. 7). Thus one sees that the sequence $(x_n)$ has a cluster point $x''$ in $F''$ for $\sigma(F'', F')$; obviously $\langle x', x'' \rangle = 2$ and, on the other hand, $x''$ belongs to the polar of $A_n$ in $F''$ for every $n$, hence to the polar $W^\circ$ of W in $F''$. From this, one concludes that $x' \notin W^{\circ\circ}$, hence is not in the closure of W for $\sigma(F', F'')$ (TVS, II, §6, No. 3, Th. 1 and §8, No. 4), therefore *a fortiori* for the strong topology, which completes the proof.

Exercises
