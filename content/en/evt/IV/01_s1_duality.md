---
book: evt
book_title: Topological Vector Spaces
chapter: IV
chapter_title: DUALITY IN TOPOLOGICAL VECTOR SPACES
section: 1
section_title: Duality
lang: en
source: evt-i-v
pdf_pages: 0183-0196, 0229-0234
extraction: ocr
subsections:
    - "no": 1
      title: Topologies compatible with a duality
      page: 0
      pdf_page: 183
    - "no": 2
      title: Mackey topology and weakened topology on a locally convex space
      page: 4
      pdf_page: 186
    - "no": 3
      title: Transpose of a continuous linear mapping
      page: 6
      pdf_page: 188
    - "no": 4
      title: Dual of a quotient space and of a subspace
      page: 8
      pdf_page: 190
    - "no": 5
      title: Dual of a direct sum and of a product
      page: 11
      pdf_page: 193
statements: 36
exercises: 25
content_sha256: 478f6ad3ca16e707ec8cc287c3cd8cef7e449a078422de8ef6615ad156944a4e
---

## § 1. DUALITY

### 1. Topologies compatible with a duality

In this section, E and F denote two vector spaces put into duality by a bilinear form B (II, p. 40). We recall (II, p. 41) that we defined two linear mappings

$$
d_B : F \to E^*, \quad s_B : E \to F^*
$$

characterized by the relation

(1)
$$
B(x, y) = \langle x, d_B(y) \rangle = \langle y, s_B(x) \rangle
$$

for $x \in E, \ y \in F$.

#### Definition 1 {#evt-iv-s1-def-1 .statement}

*A locally convex topology $\mathcal{T}$ on E is said to be compatible with the duality between E and F if $d_B$ is a bijection from F onto the dual of the locally convex space obtained by assigning the topology $\mathcal{T}$ to E.*

If there exists one such topology $\mathcal{T}$, the mapping $d_B$ is injective, that is to say, the duality between E and F is separating in F (II, p. 41).

#### Proposition 1 {#evt-iv-s1-prop-1 .statement}

(i) *The closed convex subsets in E are the same for all the locally convex topologies on E which are compatible with the duality between E and F.*
(ii) *The bounded subsets of E are the same for all the locally convex topologies on E which are compatible with the duality between E and F.*

Let $\mathcal{T}$ be a topology on E compatible with the duality between E and F, hence finer than $\sigma(E, F)$. If a convex subset of E is closed for $\mathcal{T}$, it is the intersection of closed, real half-spaces (II, p. 38, cor. 1), hence it is closed for $\sigma(E, F)$. This proves (i). Assertion (ii) was proved in cor. 3 of III, p. 27.

Let $F_\sigma$ denote the vector space F endowed with the weak topology $\sigma(F, E)$. Then the linear mapping $s_B$ maps E onto the dual $(F_\sigma)'$ of $F_\sigma$ (II, p. 43, prop. 3). Let $\mathfrak{S}$ be a family of bounded subsets of $F_\sigma$. By abuse of language, the inverse image under $s_B$ of the $\mathfrak{S}$-topology on $(F_\sigma)'$ is called the $\mathfrak{S}\text{-topology on } E$. It is defined by the family of semi-norms

$$
p_A(x) = \sup_{y \in A} |B(x, y)|,
$$

where A runs through $\mathfrak{S}$. In particular, when $\mathfrak{S}$ is the family of finite subsets of F, the $\mathfrak{S}$-topology is precisely the weak topology $\sigma(E, F)$.

#### Definition 2 {#evt-iv-s1-def-2 .statement}

*Let E and F be two spaces in duality. The Mackey topology on E, denoted by $\tau(E, F)$ is defined as the $\mathfrak{S}$-topology on E, where $\mathfrak{S}$ is the family of all subsets of F whose image in $E^*$ (under $d_B$) is convex, balanced and compact for $\sigma(E^*, E)$.*

When the duality between E and F is separating in F, $d_B$ is injective and the topology $\sigma(F, E)$ on F is the inverse image under $d_B$ of the topology $\sigma(E^*, E)$ on $E^*$. In this case, $\mathfrak{S}$ consists of all those subsets of F which are convex, balanced and compact for $\sigma(F, E)$.

In general, if $F_1 = d_B(F) \subset E^*$, and if we denote by $(x, y_1) \mapsto B_1(x, y_1)$ the restriction of the canonical bilinear form $(x, x^*) \mapsto \langle x, x^* \rangle$ to $E \times F_1$, then E and $F_1$ are put in duality by $B_1$, and this duality is separating in $F_1$, since by definition we have $B(x, y) = B_1(x, d_B(y))$, def. 2 shows that $\tau(E, F) = \tau(E, F_1)$.

#### Remark 1 {#evt-iv-s1-n1-rem-1 .statement}

— Let A be a compact convex subset of a Hausdorff locally convex space G, and let $\tilde{A}$ be the closed convex balanced envelope of A. When the field K is $\mathbf{R}$, the set $\tilde{A}$ is the closed convex envelope of $A \cup (-A)$; when K is $\mathbf{C}$, the set $\tilde{A}$ is contained in the closed convex envelope of $2A \cup (-2A) \cup (2iA) \cup (-2iA)$. Consequently (II, p. 14, prop. 15), $\tilde{A}$ is compact.

We deduce, in particular, that when the duality between E and F is separating in F, *the Mackey topology $\tau(E, F)$ is also the $\mathfrak{S}'$-topology, where $\mathfrak{S}'$ is the set of all convex subsets of F which are compact for $\sigma(F, E)$*. In an analogous way we define the Mackey topology $\tau(F, E)$ on F.

**Theorem 1 (Mackey).** — *Let E and F be two spaces in duality; suppose that the duality is separating in F. In order that a locally convex topology $\mathcal{T}$ on E be compatible with the duality between E and F, it is necessary and sufficient that $\mathcal{T}$ be finer than the topology $\sigma(E, F)$ and coarser than the Mackey topology $\tau(E, F)$.*

Identify F with its image in $E^*$ under $d_B$. Let $\mathfrak{S}_0$ denote the set of all subsets of F which are convex, balanced and compact for $\sigma(F, E)$. By definition, $\tau(E, F)$ is the $\mathfrak{S}_0$-topology on E, hence is finer than $\sigma(E, F)$.

#### Lemma 1 {#evt-iv-s1-lem-1 .statement}

*The subspace F of E* consists of all linear forms on E which are continuous for $\tau(E, F)$.

Every element of F is a continuous mapping for $\sigma(E, F)$, hence for $\tau(E, F)$.

Conversely, let $f \in E^*$ be continuous for $\tau(E, F)$. There exists a neighbourhood U of 0 in E (for $\tau(E, F)$), such that $|f| \leq 1$ on U; we can assume that there exists a set $A \in \mathcal{S}_0$ such that $U = A^\circ$. In other words, $f$ belongs to the bipolar $A^{\circ\circ}$ of A for the duality between $E^*$ and E. But the topology $\sigma(F, E)$ on F is induced by $\sigma(E^*, E)$; consequently A is convex, balanced and compact for $\sigma(E^*, E)$, and the theorem of bipolars (II, p. 44, th. 1) implies the equality $A = A^{\circ\circ}$. Therefore we have that $f \in F$, from which the lemma follows.

#### Lemma 2 {#evt-iv-s1-lem-2 .statement}

*Let $\mathcal{T}$ be a locally convex topology on E such that every linear form on E which is continuous for $\mathcal{T}$ belongs to F. Then $\mathcal{T}$ is coarser than $\tau(E, F)$.*

*Let $\mathcal{U}$ be the set of convex, balanced neighbourhoods of 0 for $\mathcal{T}$. Let $\mathcal{S}$ be the set of polars in F of elements of $\mathcal{U}$. By cor. 2 of III, p. 17, we have $\mathcal{S} \subset \mathcal{S}_0$, and by cor. 1 of prop. 7 of III, p. 19, $\mathcal{T}$ is identical with the $\mathcal{S}'$-topology, where $\mathcal{S}'$ is the set of polars of sets of $\mathcal{U}$ in the dual $E'$ of E. But $E' \subset F$, by hypothesis, hence every set of $\mathcal{S}'$ is contained in a set of $\mathcal{S}$; and the lemma follows.*

Let $\mathcal{T}$ be a topology on E compatible with the duality between E and F. Then $\mathcal{T}$ is coarser than $\tau(E, F)$ by lemma 2, and evidently $\mathcal{T}$ is finer than $\sigma(E, F)$. Conversely, F is the dual of E for the topology $\tau(E, F)$ (lemma 1) and for the topology $\sigma(E, F)$ (II, p. 43, prop. 3), hence also for every topology intermediate between $\tau(E, F)$ and $\sigma(E, F)$.

#### Corollary {#evt-iv-s1-n1-cor-1 .statement}

*Let p be a semi-norm on E. The following conditions are equivalent :*

(i) *p is continuous for the topology $\tau(E, F)$;*
(ii) *every linear form f on E, such that $|f| \leq p$, comes from an element of F.*

(i) $\Rightarrow$ (ii) : if p is continuous for $\tau(E, F)$, every linear form f on E such that $|f| \leq p$ is continuous for $\tau(E, F)$, hence comes from an element of F by lemma 1.

(ii) $\Rightarrow$ (i) : let $\mathcal{T}$ be the topology on E defined by the semi-norm p. If condition (ii) is satisfied, the linear forms on E which are continuous for $\mathcal{T}$ belong to F. By lemma 2 $\mathcal{T}$ is coarser than $\tau(E, F)$, hence p is continuous for $\tau(E, F)$.

#### Remark 2 {#evt-iv-s1-n1-rem-2 .statement}

*Let K be a convex subset of F which is compact for the weak topology $\sigma(F, E)$ and $\mu$ a positive measure on K. Put*

$$
p(x) = \int_K |B(x, y)| \, d\mu(y)
$$

for all $x \in E$. It is immediate that p is a semi-norm. Moreover, for every $x \in E$, the relation « $|B(x, y)| \leq 1$ for all $y \in K$ » implies that $p(x) \leq \mu(K)$. This proves that the semi-norm p on E is continuous for the Mackey topology $\tau(E, F)$. \*

#### Example {#evt-iv-s1-n1-exa-1 .statement}

Let G be a locally convex space and G' its dual. On G', the weak topology $\sigma(G', G)$ and the topology of convex compact convergence (III, p. 14) are compatible with the duality between G' and G. In general, the strong topology and the topology of compact convergence on G' are not compatible with the duality between G' and G. Recall however that when G is Hausdorff and quasi-complete, the topology of compact convergence on G' coincides with that of convex compact convergence (III, p. 8), hence is compatible with the duality between G' and G.

#### Definition 3 {#evt-iv-s1-def-3 .statement}

*Let E and F be two vector spaces in duality, and $\mathcal{T}$ the family of subsets of F which are bounded for $\sigma(F, E)$. Then the $\mathcal{T}$-topology on F is denoted by $\beta(E, F)$.*

Similarly, we define the topology $\beta(F, E)$ on F. It can be seen easily that the topology $\beta(E, F)$ is identical with $\beta(E, F/E^\circ)$, and we can reduce to the case when the duality between E and F is separating in F.

*Remarks. —* 3) Let $E_\sigma$ denote the space E endowed with the topology $\sigma(E, F)$. The barrels (III, p. 24) in $E_\sigma$ are the subsets of E which are convex, balanced closed and absorbent for $\sigma(E, F)$. These are none other than the polars of the subsets of F which are convex, balanced and bounded for $\sigma(F, E)$. Consequently, the family of all barrels in $E_\sigma$ is a fundamental system of neighbourhoods of 0 for the topology $\beta(E, F)$ in E. In other words, a semi-norm on E is continuous for $\beta(E, F)$ if and only if it is lower semi-continuous for $\sigma(E, F)$ (*cf.* III, p. 24, prop. 1).

4) Let $\mathcal{T}$ be a topology on E compatible with the duality between E and F. By prop. 1, (ii) of IV, p. 1, the topology $\beta(F, E)$ on F is none other than the strong topology on F, when F is identified with the dual of E (with the topology $\mathcal{T}$).

5) The topology $\beta(E, F)$ on E is finer than $\tau(E, F)$. It is not, in general compatible with the duality between E and F (*cf.* however § 2). In particular, a subset of E which is bounded for $\sigma(E, F)$ is not necessarily bounded for $\beta(E, F)$.

### 2. Mackey topology and weakened topology on a locally convex space

Let E be a locally convex space and E' its dual. We put E and E' in duality by means of the canonical bilinear form $(x, x') \mapsto \langle x, x' \rangle$ on $E \times E'$. This duality is separating in E'. We shall consider three topologies on E compatible with the duality between E and E' :

a) the given topology on E, which we shall call the *initial topology*, whenever any confusion is likely to arise;

b) the topology $\sigma(E, E')$, called the *weakened topology* on E;

c) the topology $\tau(E, E')$, called the *Mackey topology* on E.

The initial topology is finer than the weakened topology and coarser than the Mackey topology; moreover, these three topologies can be distinct (IV, p. 49, exerc. 8).

By prop. 1 of IV, p. 1, these three topologies have the same closed convex sets, the same barrels, the same bounded sets and the same adapted bornologies. In particular :

#### Proposition 2 {#evt-iv-s1-prop-2 .statement}

*Let E be a locally convex space, and let A be a convex subset of E (for example, a vector subspace of E). The closure of A is the same for the initial topology and for the weakened topology of E.*

#### Remark 1 {#evt-iv-s1-n2-rem-1 .statement}

For a family $(x_i)_{i \in I}$ of elements of E to be total (resp. topologically independent) for the initial topology, it is necessary and sufficient that it is so for the weakened topology; this follows from prop. 2. Hence we can apply the criteria of II, p. 43.

#### Remark 2 {#evt-iv-s1-n2-rem-2 .statement}

Let $\mathcal{T}_1$ and $\mathcal{T}_2$ be two locally convex topologies on E, compatible with the duality between E and $E'$, $\mathcal{T}_1$ being finer than $\mathcal{T}_2$. Then every neighbourhood of 0 for $\mathcal{T}_1$, which is convex and closed for $\mathcal{T}_1$ is closed for $\mathcal{T}_2$ by prop. 1 of IV, p. 1. Consequently (GT, II, § 3, No. 3, corollary) every subset of E which is complete for $\mathcal{T}_2$ is so for $\mathcal{T}_1$ also.

In particular, every subset of E which is complete for the weakened topology is complete for the initial topology, and every subset of E complete for the initial topology is so for the Mackey topology. If E is quasi-complete for the weakened topology, it is so for every topology compatible with the duality between E and $E'$. If it is quasi-complete for the initial topology, it is so for the Mackey topology.

#### Remark 3 {#evt-iv-s1-n2-rem-3 .statement}

Suppose E is Hausdorff (for the initial topology). Let A be a subset of E which is closed and bounded for $\sigma(E, E')$, hence also for every topology compatible with the duality between E and $E'$. Since A is precompact for $\sigma(E, E')$ (III, p. 3, Remark 5), assuming that A is *compact* for $\sigma(E, E')$ is equivalent to A being *complete* for $\sigma(E, E')$.

Therefore, on account of remark 2, we see that :

#### Proposition 3 {#evt-iv-s1-prop-3 .statement}

*Suppose E is Hausdorff, and $E'$ its dual. Every subset of E which is precompact for the initial topology and compact for $\sigma(E, E')$, is compact for the initial topology.*

#### Remark 4 {#evt-iv-s1-n2-rem-4 .statement}

The topology $\beta(E, E')$ (IV, p. 4, def. 3) is finer than the Mackey topology. If $\beta(E, E')$ is distinct from $\tau(E, E')$, it is not compatible with the duality between E and $E'$. The space E is barrelled if and only if the initial topology is equal to $\beta(E, E')$ (III, p. 24).

#### Proposition 4 {#evt-iv-s1-prop-4 .statement}

*Let E be a locally convex space. The Mackey topology on E is identical with the initial topology in each of the following cases :*

a) E is barrelled;
b) E is bornological;
c) E is metrizable.

We note first that the Mackey topology on E is identical with the initial topology if and only if every convex subset of $E'$ which is compact for $\sigma(E', E)$, is equi-continuous. This is certainly the case if E is barrelled (III, p. 24, corollary).

Suppose E is bornological; let V be a convex and balanced neighbourhood of 0 in E for the topology $\tau(E, E')$. Let B be a subset of E, bounded for the initial topology. Since B is bounded for the Mackey topology, V absorbs B, and since E is bornological, V is a neighbourhood of 0 for the initial topology.

In case c), the space E is bornological (III, p. 12, prop. 2).

### 3. Transpose of a continuous linear mapping

In this section, $E_1$ and $E_2$ denote two locally convex spaces, with respective duals $E'_1$ and $E'_2$.

Let $u$ be a linear mapping from $E_1$ into $E_2$. For $u$ to be continuous when $E_1$ and $E_2$ are assigned the weakened topologies, it is necessary and sufficient that $f \circ u$ belongs to $E'_1$ for all $f \in E'_2$; this is the case if $u$ is continuous. Then the linear mapping $f \mapsto f \circ u$ from $E'_2$ into $E'_1$ is called the transpose of $u$ and is denoted by $^t u$.

#### Proposition 5 {#evt-iv-s1-prop-5 .statement}

*Let $u$ be a continuous linear mapping from $E_1$ into $E_2$.*

(i) *If $E_1$ and $E_2$ are Hausdorff then $u$ is injective if and only if the image of $^t u$ is dense in $E'_1$ for the weak topology $\sigma(E'_1 : E_1)$.*

(ii) *For $^t u$ to be injective it is necessary and sufficient that the image of $u$ is dense in $E_2$.*

A vector subspace of $E_2$ is dense for the initial topology if and only if it is dense for the weakened topology (IV, p. 4, prop. 2). Prop. 5 then follows from II, p. 47, cor. 2.

#### Proposition 6 {#evt-iv-s1-prop-6 .statement}

*Let $u$ be a linear mapping from $E_1$ into $E_2$ which is continuous for the weakened topologies. For $i = 1, 2$, let $\mathfrak{S}_i$ be a family of bounded subsets of $E_i$. In order that $^t u$ is a continuous mapping from $(E'_2)_{\mathfrak{S}_2}$ into $(E'_1)_{\mathfrak{S}_1}$, it is necessary and sufficient that, for every set $A \in \mathfrak{S}_1$, there exist sets $A_1, ..., A_n$ in $\mathfrak{S}_2$ and a real number $\lambda > 0$ such that $\lambda \cdot u(A)$ is contained in the closed convex balanced envelope of $A_1 \cup ... \cup A_n$\footnote{In other words, $u(\mathfrak{S}_1)$ is contained in the smallest adapted bornology containing $\mathfrak{S}_2$ (III, p. 3).}.*

This is an immediate consequence of prop. 2 of III, p. 15.

#### Corollary {#evt-iv-s1-n3-cor-1 .statement}

*Let $u$ be a continuous linear mapping from $E_1$ into $E_2$. Then $^t u$ is continuous when the duals $E'_i$ are assigned the following topologies:*
a) *the weak topologies $\sigma(E'_i, E_i)$;*
b) *the strong topologies $\beta(E'_i, E_i)$;*
c) *the Mackey topologies $\tau(E'_i, E_i)$;*
d) *the topologies of precompact convergence.*
*Moreover, if $E_2$ is Hausdorff, $^t u$ is continuous when the duals $E'_i$ are assigned:*
e) *the topologies of compact convergence* (resp. *compact convex*).

The only point which requires a proof is the case c), when the topologies of $E_1$ and $E_2$ are not necessarily Hausdorff. Then for every linear form $f \in E'_1*$, $f \circ ^t u$ is a linear form on $E'_2$; hence there is a linear mapping $v : E'_1* \to E'_2*$ which is continuous for the topologies $\sigma(E'_1*, E'_1)$ and $\sigma(E'_2*, E'_2)$ and is such that $d_{B_2} \circ u = v \circ d_{B_1}$, where $d_{B_i}$ is the canonical mapping from $E_i$ into $E'_i*$ ($i = 1, 2$). Consequently, if $A$ is a subset of $E_1$ such that $d_{B_1}(A)$ is convex, balanced and compact for $\sigma(E'_1*, E'_1)$ then $d_{B_2}(u(A)) = v(d_{B_1}(A))$ is convex, balanced and compact for $\sigma(E'_2*, E'_2)$ since the topologies $\sigma(E'_1*, E'_1)$ and $\sigma(E'_2*, E'_2)$ are Hausdorff.

#### Proposition 7 {#evt-iv-s1-prop-7 .statement}

— Let $u : E_1 \to E_2$ be a linear mapping. We assume that $u$ is continuous for the weakened topologies of $E_1$ and $E_2$.

(i) The mapping $u$ is continuous if $E_1$ and $E_2$ are assigned their Mackey topologies.

(ii) If $E_1$ is bornological or barrelled, then $u$ is continuous for the initial topologies of $E_1$ and $E_2$.

(iii) In order that $u$ be continuous for the initial topologies of $E_1$ and $E_2$, it is necessary and sufficient that the image under $'u$ of every equicontinuous subset of $E_2'$ be equicontinuous in $E_1'$.

The hypothesis implies that $'u$ is continuous for the weak topologies $\sigma(E_2', E_2)$ and $\sigma(E_1', E_1)$ (II, p. 46, corollary) hence the image under $'u$ of a convex, balanced and compact subset for $\sigma(E_2', E_2)$ is convex, balanced and compact for $\sigma(E_1', E_1)$, the topologies $\sigma(E_2', E_2)$ and $\sigma(E_1', E_1)$ being Hausdorff. Therefore, assertion (i) follows from GT, X, § 1, No. 4, prop. 3, b). Assertion (ii) is a consequence of (i) : for, if $E_1$ is bornological or barrelled, its initial topology is the Mackey topology, and the Mackey topology of $E_2$ is finer than the initial topology of $E_2$. Finally, the initial topology of $E_i$ is that of uniform convergence on equicontinuous subsets of $E_i'$ (III, p. 19, cor. 1 of prop. 7). This proves (iii).

#### Corollary {#evt-iv-s1-n3-cor-2 .statement}

— Suppose $E_1$ is a normed space. Let $u$ be a linear mapping from $E_1$ into $E_2$. The following properties are equivalent :

a) $u$ is continuous;

b) $u$ is continuous for the weakened topologies;

c) the image of the unit ball in $E_1$ under $u$ is bounded in $E_2$;

d) for every sequence $(x_n)$ of points of $E_1$ tending to 0 for the initial topology, the sequence $(u(x_n))$ is bounded for the weakened topology of $E_2$.

Since $E_1$ is bornological the equivalence of a) and b) follows from prop. 7; that of a) and c) is immediate. The equivalence of a) and d) follows from prop. 1 of IV, p. 1, and from prop. 1 of III, p. 11.

#### Proposition 8 {#evt-iv-s1-prop-8 .statement}

— (i) Let $E$ be a normed space, with dual $E'$. For every $x \in E$, we have

$$
\|x\| = \sup_{x' \in E', \|x'\| \leq 1} |\langle x, x' \rangle|.
$$

(ii) Let $E_1$ and $E_2$ be two normed spaces and $u$ a continuous linear mapping from $E_1$ into $E_2$. We have

$$
\|u\| = \|t u\|.
$$

Let $x \in E$. For every $x' \in E'$ such that $\|x'\| \leq 1$, we have

$$
|\langle x, x' \rangle| \leq \|x\| \cdot \|x'\| \leq \|x\|.
$$

By Hahn-Banach theorem (II, p. 23, cor. 2), there exists an element $x'$ in $E'$ such that $\|x'\| \leq 1$ and $\langle x, x' \rangle = \|x\|$. This proves (i).

Let us now prove (ii). By formula (3) and the definition of the transpose, we have

$$
\|^{t}u\| = \sup_{\|y'\| \leq 1} \|^{t}u(y')\| = \sup_{\|y'\| \leq 1, \|x\| \leq 1} |\langle x, ^{t}u(y') \rangle|
= \sup_{\|x\| \leq 1, \|y'\| \leq 1} |\langle u(x), y' \rangle| = \sup_{\|x\| \leq 1} \|u(x)\| = \|u\|.
$$

#### Remark 1 {#evt-iv-s1-n3-rem-1 .statement}

Formula (3) is a particular case of (4), corresponding to the linear mapping $\lambda \mapsto \lambda x$ from K into E.

#### Remark 2 {#evt-iv-s1-n3-rem-2 .statement}

Put $B(x, y') = \langle u(x), y' \rangle = \langle x, ^{t}u(y') \rangle$ for $x \in E_1,\ y' \in E'_2$. The above proof shows that B is a continuous bilinear form on $E_1 \times E'_2$, with norm (GT, X, § 3, No. 2) equal to $\|u\|$.

#### Corollary {#evt-iv-s1-n3-cor-3 .statement}

— *Let $\dot{E}$ be a normed space satisfying the first axiom of countability. There exists a countable subset D of $E' - \{0\}$ such that we have*

$$
\|x\| = \sup_{\xi \in D} |\langle x, \xi \rangle| / \|\xi\|
$$

*for all* $x \in E$.

Let B' be the unit ball of the dual $E'$ of E with the weak topology $\sigma(E', E)$ assigned to it. Then B' is a compact metrizable space (III, p. 19, cor. 2); hence there exists a countable dense subset D' in B'. Put $D = D' \cap (E' - \{0\})$. Let $x \in E$; the mapping $x' \mapsto \langle x, x' \rangle$ from B' into K is continuous, therefore

$$
\sup_{x' \in B'} |\langle x, x' \rangle| = \sup_{\xi \in D'} |\langle x, \xi \rangle| \leq \sup_{\xi \in D} |\langle x, \xi \rangle| / \|\xi\| \leq \|x\|.
$$

Formula (5) now follows from (3).

### 4. Dual of a quotient space and of a subspace

Throughout this section, E denotes a locally convex space, M a vector subspace of E, and $M^\circ$ the orthogonal of M in the dual $E'$ of E. Let $p$ be the canonical mapping from E onto $E/M$; then $^{t}p$ is injective, with image $M^\circ$, hence defines a vector space isomorphism (not topological)

$$
\pi : (E/M)' \to M^\circ .
$$

Similarly, let $i$ be the canonical injection from M into E. Then $^{t}i$ is surjective (II, p. 24, prop. 2); its kernel is equal to $M^\circ$, and we get a vector space isomorphism (not topological)

$$
i : E'/M^\circ \to M'.
$$

#### Proposition 9 {#evt-iv-s1-prop-9 .statement}

— (i) *For a subset A of* $(E/M)'$ *to be equicontinuous, it is necessary and sufficient that* $\pi(A)$ *is an equicontinuous subset of* $E'$.

(ii) Let $\mathfrak{S}$ be a set of bounded subsets of $E$, and $\mathfrak{S}_1$ the set of the images of subsets $A \in \mathfrak{S}$ in $E/M$. Then $\pi$ is an isomorphism from $(E/M)'_{\mathfrak{S}_1}$ onto $M^\circ$, where $M^\circ$ is assigned the topology induced by that of $E'_{\mathfrak{S}}$.

(iii) Suppose $E$ is a normed space then $\pi$ is an isometry from the normed space $(E/M)'$ onto the normed subspace $M^\circ$ of $E'$.

Let $A$ be a subset of $(E/M)'$ and $B = {}^t p(A) \subset E'$. Put
$$
q(\xi) = \sup_{\xi' \in A} |\langle \xi, \xi' \rangle|
$$
for all $\xi \in E/M$. In order that $A$ be equicontinuous, it is necessary and sufficient that the mapping $q$ from $E/M$ into $\overline{\mathbf{R}}_+$ is a continuous semi-norm. This implies that $q \circ p$ is a continuous semi-norm on $E$ (II, p. 27, prop. 5, (ii)). Since we have
$$
(q \circ p)(x) = \sup_{x' \in B} |\langle x, x' \rangle|
$$
for all $x \in E$, this in turn implies that $B$ is equicontinuous in $E'$, and (i) follows.

Let $A \in \mathfrak{S}$ and let $f$ be a continuous linear form on $E/M$. For every $\lambda \in \mathbf{R}_+$, we have $|f| \leq \lambda$ on $p(A)$ if and only if $|{}^t p(f)| \leq \lambda$ on $A$; hence (ii).

Finally we prove (iii). Let $y'$ be in $(E/M)'$. An element in $E/M$ has norm $< 1$ if and only if it is the image under $p$ of an element of norm $< 1$ in $E$. Hence
$$
\begin{align*}
\|y'\| &= \sup_{y \in E/M, \|y\| < 1} |\langle y, y' \rangle| = \sup_{x \in E, \|x\| < 1} |\langle p(x), y' \rangle| \\
&= \sup_{x \in E, \|x\| < 1} |\langle x, {}^t p(y') \rangle| = \|{}^t p(y')\|,
\end{align*}
$$
and ${}^t p$ induces an isometry from $(E/M)'$ onto $M^\circ$.

#### Proposition 10 {#evt-iv-s1-prop-10 .statement}

— (i) For a subset $A$ of $M'$ to be equicontinuous, it is necessary and sufficient that it is the image under ${}^t i$ of an equicontinuous subset of $E'$.

(ii) Suppose $M$ is closed in $E$. Let $\mathfrak{S}$ be a covering of $E$ consisting of bounded subsets and let $\mathfrak{S}_1$ be the set of subsets of $M$ of the form $M \cap A$ for $A$ in $\mathfrak{S}$. The bijective linear mapping $i$ from $E'_{\mathfrak{S}}/M^\circ$ onto $M'_{\mathfrak{S}_1}$ is continuous. It is a homeomorphism if $\mathfrak{S}$ is a directed set for the relation $\subset$ and consists of closed convex and compact sets for $\sigma(E, E')$.

(iii) If $E$ is assumed to be normed, then $i$ is an isometry from $E'/M^\circ$ onto $M'$.

The image under ${}^t i$ of an equicontinuous subset of $E'$ is an equicontinuous subset of $M'$ (IV, p. 7, prop. 7). Conversely, let $A$ be an equicontinuous subset of $M'$. The topology of $M$ is defined by the set of restrictions to $M$ of the continuous semi-norms on $E$. Hence there exists a continuous semi-norm $p$ on $E$ such that $|f(x)| \leq p(x)$ for all $f \in A$ and for all $x \in M$. Let $B$ be the set of all linear forms $g$ on $E$ such that $|g| \leq p$ and whose restriction to $M$ belongs to $A$. The set $B$ is equicontinuous in $E'$; by Hahn-Banach theorem (II, p. 23, cor. 1), we have ${}^t i(B) = A$, hence (i) follows.

We now prove (ii). By prop. 6 of IV, p. 6, the linear mapping ${}^t i$ from $E'_{\mathfrak{S}}$ into $M'_{\mathfrak{S}_1}$ is continuous, and defines, by passing to the quotient, a continuous linear mapping $\iota$ from $E'_\mathcal{S}/M^\circ$ onto $M'_{\mathcal{S}_1}$. Let $\mathcal{T}$ be the topology on $M'$ obtained by transferring that of $E'_\mathcal{S}/M^\circ$ by $\iota$; this is finer than the $\mathcal{S}_1$-topology.

Suppose now that $\mathcal{S}$ is a directed set for $\subset$ and consists of closed, convex, balanced and compact sets for $\sigma(E, E')$. To show that $\iota$ is a homeomorphism, *i.e.* that $\mathcal{T}$ is coarser than the $\mathcal{S}_1$-topology on $M'$, it is enough to prove that $\mathcal{T}$ is compatible with the duality between $M'$ and $M$ and that every equicontinuous set in $M$ (considered as the dual of $M$ with $\mathcal{T}$) is contained in the homothetic of a set belonging to $\mathcal{S}_1$. Since $\mathcal{T}$ is finer than the $\mathcal{S}_1$-topology and $\mathcal{S}_1$ is a covering of $M$, the linear form $y' \mapsto \langle y, y' \rangle$ on $M'$ is continuous for $\mathcal{T}$ for every $y \in M$. Let $f$ be a linear form on $M'$ which is continuous for $\mathcal{T}$; then $f \circ \iota$ is a continuous linear form on $E'_\mathcal{S}$. The $\mathcal{S}$-topology on $E'$ is coarser than the Mackey topology $\tau(E', E)$; for, the mapping $d_B : E \to {E'}^*$ is continuous for the topologies $\sigma(E, E')$ and $\sigma({E'}^*, E')$, and since the latter is Hausdorff, the image under $d_B$ of a set which is compact for $\sigma(E, E')$ is compact for $\sigma({E'}^*, E')$. By lemma 1 of IV, p. 3, there exists $x_0 \in E$ such that $f(\iota(x')) = \langle x_0, x' \rangle$ for all $x' \in E'$. In particular, $\langle x_0, x' \rangle = 0$ for all $x' \in M^\circ$, and since $M$ is closed in $E$, we have $x_0 \in M$ (II, p. 45, cor. 2); and finally, $f(y') = \langle x_0, y' \rangle$ for all $y' \in M'$. This proves that $\mathcal{T}$ *is compatible with the duality between* $M$ *and* $M'$.

Now let $A$ be a subset of $M$ equicontinuous for the topology $\mathcal{T}$ on $M'$. By the definition of $\mathcal{T}$, and in view of the hypothesis that $\mathcal{S}$ is directed, this means that there exists a set $B \in \mathcal{S}$ containing 0 and such that the upper bound $\lambda$ of the numbers $|\langle y, x' \rangle|$ for $y \in A$ and $x' \in B^\circ$, is finite (III, p. 19, prop. 7). Since $B$ is closed in $E$, the theorem of bipolars (II, p. 44, th. 1) shows that we have $A \subset \lambda(B \cap M)$; this completes the proof of (ii).

We shall now prove (iii). Let $y' \in M'$. We shall prove the formula

$$
\|y'\| = \inf_{\iota(x') = y'} \|x'\|.
$$

By prop. 8, (ii) of IV, p. 7, we have $\|\iota\| = \|i\|$, and so $\|\iota\| \leq 1$, and

$$
\|y'\| \leq \inf_{\iota(x') = y'} \|x'\|.
$$

By Hahn-Banach theorem (II, p. 23, cor. 3), there exists a linear form $x'_0$ on $E$ which extends $y'$ and is of the same norm; hence we get the inequality opposite to (7), since $\iota(x'_0) = y'$.

#### Remark {#evt-iv-s1-n4-rem-1 .statement}

— We know (II, p. 48, prop. 7, (ii)) that $\iota$ is a topological vector space isomorphism from $E'_s/M^\circ$ onto $M'_s$ (weak duals). For the topology of compact convex convergence, prop. 10 shows that $\iota$ is an isomorphism from $E'_{cc}/M^\circ$ onto $M'_{cc}$ when $E$ is Hausdorff and $M$ closed in $E$. For the strong topologies, $\iota$ is a continuous mapping from $E'_b/M^\circ$ onto $M'_b$; it is an isomorphism if $E$ is a Banach space \* or if $E$ is semi-reflexive and $M$ is closed in $E$ (IV, p. 15) *, but this is not always so if $E$ is a Fréchet space (IV, p. 58, exerc. 5, *c*)).

#### Proposition 11 {#evt-iv-s1-prop-11 .statement}

— (i) *The weakened topology on* $E/M$ *is the quotient of that on* $E$; *the weakened topology on* $M$ *is induced by that of* $E$.

(ii) *The Mackey topology on E/M is the quotient of that on E; the Mackey topology on M is finer than the topology induced by τ(E, E').*

Assertion (i) follows from prop. 7 of II, p. 48.

The canonical injection $i : M \to E$ is continuous for the weakened topologies, hence for the Mackey topologies $\tau(M, M')$ and $\tau(E, E')$ (IV, p. 7, prop. 7). Similarly, the canonical projection $p : E \to E/M$ is continuous for the Mackey topologies. We see immediately that the quotient topology on $E/M$ obtained from $\tau(E, E')$ is compatible with the duality between $E/M$ and $(E/M)'$, hence is coarser than the Mackey topology on $E/M$, by Mackey's theorem (IV, p. 2, th. 1). This proves (ii).

### 5. Dual of a direct sum and of a product

For every $i \in I$, let $(E_i, F_i)$ be a pair of vector spaces, set in duality by a bilinear form $B_i$. We put $E = \prod_{i \in I} E_i$ and $F = \bigoplus_{i \in I} F_i$, and we identify each $F_i$ with a subspace of $F$. We put $E$ and $F$ in duality by means of the bilinear form

$$
B(x, y) = \sum_{i \in I} B_i(x_i, y_i) \quad \text{for} \quad x = (x_i) \quad \text{and} \quad y = (y_i)
$$

(the family $(B_i(x_i, y_i))_{i \in I}$ has finite support).

We recall (II, p. 50, prop. 8) that the weak topology $\sigma(E, F)$ is the product of the weak topologies $\sigma(E_i, F_i)$.

#### Lemma 3 {#evt-iv-s1-lem-3 .statement}

— (i) *For every $i \in I$, let $\mathfrak{S}_i$ be a family of subsets of $F_i$, which is bounded for $\sigma(F_i, E_i)$; put $\mathfrak{S} = \bigcup_{i \in I} \mathfrak{S}_i$. Then the $\mathfrak{S}$-topology on $E$ is the product of the $\mathfrak{S}_i$-topologies on the $E_i$.*

(ii) *For every $i \in I$, let $\mathfrak{J}_i$ be an adapted bornology on the space $E_i$ endowed with the weak topology $\sigma(E_i, F_i)$, none equal to $\{ \varnothing \}$. Let $\mathfrak{J}$ be the family of subsets $A$ of $E = \prod_{i \in I} E_i$ such that $\operatorname{pr}_i(A) \in \mathfrak{J}_i$ for all $i \in I$. Then the $\mathfrak{J}$-topology on $F$ is the direct sum of the $\mathfrak{J}_i$-topologies on the $F_i$.*

Let $\mathcal{T}$ be the product of the $\mathfrak{S}_i$-topologies. The sets of the form

$$
A = \prod_{i \in J} A_i^\circ \times \prod_{i \in I - J} E_i
$$

where $J \subset I$ is finite and $A_i \in \mathfrak{S}_i$ for all $i \in J$, form a fundamental system of neighbourhoods of 0 for $\mathcal{T}$. We have $A = (\bigcup_{i \in J} A_i)^\circ$, hence $\mathcal{T}$ is identical with the $\mathfrak{S}$-topology. This proves (i).

We assign the $\mathfrak{J}$-topology to $F$ and the $\mathfrak{J}_i$-topology to each $F_i$. For every subset $A$ of $E$, we have $F_i \cap A^\circ = \operatorname{pr}_i(A)^\circ$, hence the injection from $F_i$ into $F$ is continuous. Let $q$ be a semi-norm on $F$; we assume that the restriction $q_i$ of $q$ to $F_i$ is continuous for all $i \in I$. Then we can find non-empty subsets $A_i \in \mathfrak{J}_i$ such that we have

$$
q_i(y_i) \leq \sup_{x_i \in A_i} |B_i(x_i, y_i)| \quad (y_i \in F_i) .
$$

Put $A = \prod_{i \in I} A_i$; then $A \in \mathfrak{J}$. For $y = (y_i)_{i \in I}$ in $F$, we have
$$
q(y) \leq \sum_{i \in I} q_i(y_i) \leq \sum_{i \in I} \sup_{x_i \in A_i} |B_i(x_i, y_i)| = \sup_{x \in A} |B(x, y)|,
$$
where the last equality follows from (8) since the family $(y_i)_{i \in I}$ has finite support and the $A_i$ are non-empty and can be assumed balanced (GT, IV, § 5, No. 7, cor. 2 to prop. 12). This inequality proves that $q$ is continuous on $F$, and hence (ii).

#### Proposition 12 {#evt-iv-s1-prop-12 .statement}

*The topology $\beta(F, E)$ is the direct sum of the topologies $\beta(F_i, E_i)$. The topology $\beta(E, F)$ is the product of the topologies $\beta(E_i, F_i)$.*

We shall apply lemma 3 taking for $\mathfrak{S}_i$ the family of all subsets of $F_i$ which are bounded for $\sigma(F_i, E_i)$ and for $\mathfrak{J}_i$ the family of all subsets of $E_i$ which are bounded for $\sigma(E_i, F_i)$.

By cor. 2 of III, p. 4, $\mathfrak{J}$ is the family of all subsets of $E_i$ which are bounded for the product topology of the $\sigma(E_i, F_i)$, which is identical with $\sigma(E, F)$. Hence our assertion on $\beta(F, E)$ follows.

We endow $F = \bigoplus_{i \in I} F_i$ with the topology $\mathcal{T}$ which is the direct sum of the topologies $\sigma(F_i, E_i)$. Then the dual of $F$ consists of the linear forms $y \mapsto B(x, y)$ where $x$ runs through $E$ (II, p. 30, prop. 6). By prop. 1 of IV, p. 1, the topologies $\mathcal{T}$ and $\sigma(F, E)$ have the same bounded sets. Assume first that that the topologies $\sigma(F_i, E_i)$ are Hausdorff. By prop. 5 of III, p. 5, these sets are contained in a subset of the form $\sum_{i \in J} B_i$ with $J \subset I$ finite and $B_i$ bounded in $F_i$ (for $\sigma(F_i, E_i)$) for all $i \in J$. Since $\sum_{i \in J} B_i$ is contained in the convex envelope of $\bigcup_{i \in J} nB_i$, where $n = \mathrm{Card}(J)$, we can apply lemma 3, to prove the assertion on $\beta(E, F)$ in this case.

For the general case, let $N_i$ be the intersection of all neighbourhoods of 0 for $\sigma(F_i, E_i)$, and let $N = \sum_{i \in I} N_i$; then $F/N$ is the topological direct sum of the $F_i/N_i$ (II, p. 31, prop. 8); we deduce from this that every subset of $F$ which is bounded for $\mathcal{T}$ is contained in a set of the form $N + \sum_{i \in J} B_i$ with $J \subset I$ finite and $B_i$ bounded in $F_i$ for all $i \in J$ (III, p. 2, *Remark* 3); since the polar of this set in $E$ is the same as that of $\sum_{i \in J} B_i$, the result follows as above.

#### Proposition 13 {#evt-iv-s1-prop-13 .statement}

*The Mackey topology $\tau(F, E)$ is the direct sum of the Mackey topologies $\tau(F_i, E_i)$. The topology $\tau(E, F)$ is the product of the topologies $\tau(E_i, F_i)$.*

The assertion on $\tau(F, E)$ follows from lemma 3 (ii) and the following property : for a closed, convex and balanced subset of $F^* = \prod_{i \in I} F_i^*$ to be compact for $\sigma(F^*, F)$, it is necessary and sufficient that its projection on each $F_i^*$ is compact for $\sigma(F_i^*, F_i)$.

To prove the assertion on $\tau(E, F)$, assume first that the topologies $\sigma(F_i, E_i)$ are Hausdorff, it is enough (lemma 3 (i)) to prove that every subset $A$ of $F$ which is convex, balanced and compact for $\sigma(F, E)$ is contained in a set of the form $\sum_{i \in J} A_i$ where $J \subset I$ is finite and where $A_i$ is convex, balanced and compact for $\sigma(F_i, E_i)$. But such a subset is bounded for $\sigma(F, E)$. By the proof of prop. 12, there exists a finite subset $J$ of $I$ such that $A \subset \sum_{i \in J} F_i$, and it is enough to take for $A_i$ the projection of $A$ on $F_i$.

In the general case, with the same notations as in the proof of prop. 12, we have $\tau(E_i, F_i) = \tau(E_i, F_i/N_i)$ and $\tau(E, F) = \tau(E, F/N)$ (IV, p. 2) and since $F/N$ is the topological direct sum of the $F_i/N_i$, we have reduced to the preceding case.

Q.E.D.

For the remainder of this paragraph, we assume that $(E_i)_{i \in I}$ is a family of locally convex spaces. Let $S$ denote the topological direct sum of the $E_i$ and $P$, their product. We define a linear mapping $\theta : S' \to \prod_{i \in I} E_i'$, said to be *canonical*, by

$$
\theta(x') = (x'|E_i)_{i \in I} \quad (x' \in S')
$$

(where $S'$ denotes the dual of $S$, and $E_i'$ that of $E_i$).

#### Proposition 14 {#evt-iv-s1-prop-14 .statement}

(i) *The mapping $\theta$ is an isomorphism from the strong (resp. weak) dual of $S = \bigoplus_{i \in I} E_i$ onto the product of the strong (resp. weak) duals of the $E_i$:*

(ii) *For a subset $A$ of $S'$ to be equicontinuous, it is necessary and sufficient that the projection of $\theta(A)$ onto $E_i'$ be equicontinuous for all $i \in I$.*

(iii) *The Mackey topology $\tau(S, S')$ is the direct sum of the Mackey topologies $\tau(E_i, E_i')$.*

(iv) *The topology $\beta(S, S')$ is the direct sum of the topologies $\beta(E_i, E_i')$.*

That $\theta$ is bijective follows immediately from the definition of a topological direct sum (II, p. 30, prop. 6). Assertion (i) then follows from prop. 12 of IV, p. 12, for the strong topologies, and from prop. 8 of II, p. 50, for the weak topologies. Similarly (iii) follows from prop. 13 (IV, p. 12) and (iv) from prop. 12 (IV, p. 12).

To prove (ii), let $A$ be a subset of $S'$. Put

$$
q(x) = \sup_{x' \in A} |\langle x, x' \rangle| \quad \text{for} \quad x \in S ;
$$

let $q_i$ denote the restriction of $q$ to $E_i$, whence

$$
q_i(x_i) = \sup_{x_i' \in A_i} |\langle x_i, x_i' \rangle| \quad \text{for} \quad x_i \in E_i ,
$$

where $A_i$ denotes the projection of $\theta(A)$ on $E_i'$. For $A$ to be equicontinuous, it is necessary and sufficient that $q$ is finite (that is, that each $q_i$ is finite) and continuous. In view of the characterization of continuous semi-norms on a topological direct sum (II, p. 27, prop. 5), this is the same as assuming that each $q_i$ is continuous, or in fact, that each set $A_i$ is equicontinuous.

Let $\phi$ be the linear mapping, said to be *canonical*, from $\bigoplus_{i \in I} E_i'$ into the dual $P'$ of $P = \prod_{i \in I} E_i$, defined by the formula

$$
\langle x, \phi(x') \rangle = \sum_{i \in I} \langle x_i, x'_i \rangle
$$

for $x = (x_i)$ in $P$ and $x' = (x'_i)$ in $\bigoplus_{i \in I} E'_i$.

#### Proposition 15 {#evt-iv-s1-prop-15 .statement}

— (i) *The map $\phi$ is an isomorphism from the topological direct sum of the strong duals of the $E_i$ onto the strong dual of $P = \prod_{i \in I} E_i$.*

(ii) *For a subset $A$ of $P'$ to be equicontinuous, it is necessary and sufficient that it is contained in a finite sum $\sum_{i \in J} \phi(A_i)$, where $J \subset I$ is finite and where $A_i$ is equicontinuous in $E'_i$ for all $i \in J$.*

(iii) *The Mackey topology $\tau(P, P')$ is the product of the topologies $\tau(E_i, E'_i)$.*

(iv) *The topology $\beta(P, P')$ is the product of the topologies $\beta(E_i, E'_i)$.*

It is immediate that $\phi$ is injective. A fundamental system of neighbourhoods of 0 in $P$ consists of sets of the form $V = \prod_{i \in J} V_i \times \prod_{i \in I - J} E_i$, where $J \subset I$ is finite and $V_i$ is a neighbourhood of 0 in $E_i$ for $i$ in $J$. The polar of $V$ in $P'$ is equal to $\sum_{i \in J} \phi(V_i^0)$.

This proves the surjectivity of $\phi$ and also assertion (ii).

Assertions (i) and (iv) follow from prop. 12 (IV, p. 12) and (iii) from prop. 13 (IV, p. 12).

#### Corollary {#evt-iv-s1-n5-cor-1 .statement}

— *Every product of barrelled spaces is barrelled.*

A locally convex space $E$ is barrelled if and only if the initial topology is identical with $\beta(E, E')$ (IV, p. 4, *Remark 3*). Hence it is enough to apply prop. 15 (iv).

### Exercises {#evt-iv-s1-exercises}

See the [exercises for § 1](exercises/s1/).
