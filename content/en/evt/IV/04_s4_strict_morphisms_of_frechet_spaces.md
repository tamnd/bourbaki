---
book: evt
book_title: Topological Vector Spaces
chapter: IV
chapter_title: DUALITY IN TOPOLOGICAL VECTOR SPACES
section: 4
section_title: Strict morphisms of Fréchet spaces
lang: en
source: evt-i-v
book_pages: TVS IV.26-TVS IV.32, TVS IV.62-TVS IV.67
pdf_pages: 0208-0214, 0244-0249
extraction: ocr
subsections:
    - "no": 1
      title: Characterizations of strict morphisms
      page: 27
      pdf_page: 209
    - "no": 2
      title: Strict morphisms of Fréchet spaces
      page: 28
      pdf_page: 210
    - "no": 3
      title: Criteria for surjectivity
      page: 31
      pdf_page: 213
statements: 13
exercises: 23
content_sha256: cc509bcb798ea7e4a952cb37673057b3029e76b3360b2b4288406331099feba7
---

## § 4. STRICT MORPHISMS OF FRÉCHET SPACES

For every locally convex space E, let S(E) denote the set of all continuous seminorms on E. For every $p \in S(E)$, let $H_p$ denote the set of all linear forms f on E such that $|f| \leqslant p$. The family $(H_p)_{p \in S(E)}$ is a base for the bornology consisting of equicontinuous subsets of $E'$.

### 1. Characterizations of strict morphisms

#### Proposition 1 {#evt-iv-s4-prop-1 .statement}

Let E and F be two locally convex spaces and u a continuous linear mapping from E into F. In order that u be a strict morphism, it is necessary and sufficient that the following condition be satisfied:

(MS) For every semi-norm $p \in S(E)$, which is null on the kernel of u, there exists q in S(F) such that $p \leq q \circ u$.

Let N be the kernel and M the image of u; we introduce the canonical decomposition of u, let

$$
E \xrightarrow{\pi} E/N \xrightarrow{\tilde{u}} M \xrightarrow{} F .
$$

The continuous semi-norms on E which are null on N, are the semi-norms $p_1 \circ \pi$ where $p_1$ ranges over S(E/N); similarly S(M) consists of the semi-norms $q_1$ for which there exists $q \in S(F)$ with $q_1 \leq q/F$. Finally, u is a strict morphism if and only if the bijective continuous linear mapping $\tilde{u}$ has a continuous inverse; this also means that every semi-norm in S(E/N) is of the form $q_1 \circ \tilde{u}$ with $q_1$ in S(M). Prop. 1 follows immediately from these remarks.

#### Proposition 2 {#evt-iv-s4-prop-2 .statement}

Let E and F be two Hausdorff locally convex spaces and u a continuous linear mapping from E into F. In order that u be a strict morphism, it is necessary and sufficient that its transpose $^t u : F' \to E'$ satisfy the following conditions:

a) The image of $^t u$ is closed in $E'$ for $\sigma(E', E)$.

b) Every equicontinuous subset of $E'$, contained in the image of $^t u$ is the image under $^t u$ of an equicontinuous subset of $F'$.

If this is so, we have $\operatorname{Ker} ^t u = (\operatorname{Im} u)^{\circ}$ and $\operatorname{Im} ^t u = (\operatorname{Ker} u)^{\circ}$ and there exist canonical isomorphisms from Coker $^t u$ onto the dual of Ker u and from Ker $^t u$ onto the dual of Coker u.

Let N be the kernel and I the image of u. By cor. 2 of II, p. 47, the kernel of $^t u$ is the orthogonal of I, and the closure of the image of $^t u$ for $\sigma(E', E)$ is the orthogonal $N^{\circ}$ of N. The conjunction of a) and b) is then equivalent to the following condition:

b') Every equicontinuous subset of $E'$ contained in $N^{\circ}$ is the image under $^t u$ of an equicontinuous subset of $F'$.

Since $N^{\circ}$ can be identified with the dual of E/N, prop. 9, (i) of IV, p. 8, shows that the equicontinuous subsets of $E'$ contained in $N^{\circ}$ are the sets which are contained in a set of the form $H_p$, where p is a continuous semi-norm on E, vanishing on N. The condition b') then says that, for every semi-norm $p \in S(E)$ which is null on N, there exists $q \in S(F)$ such that $H_p \subset ^t u(H_q)$. By Hahn-Banach theorem (II, p. 23, cor. 1 and 2, p. 63, th. 1 and cor. 1), we have $^t u(H_q) = H_{q \circ u}$, and the relations $H_p \subset H_{p'}$ and $p \leq p'$ are equivalent for all semi-norms $p$ and $p'$ in S(E). Consequently, the relation $H_p \subset ^t u(H_q)$ is equivalent to the relation $p \leq q \circ u$. By prop. 1, property b') implies that u is a strict morphism.

Suppose that u is a strict morphism. We have already seen that the kernel of $^t u$ is the orthogonal of I and the image of $^t u$ is the orthogonal of N. The cokernel of $u$ is the space $F/I$ and its dual can be identified with $I^\circ = \mathrm{Ker}\ ^t u$. Similarly, the dual of $N = \mathrm{Ker}\ u$ can be identified with $E'/N^\circ$ (IV, p. 8), *i.e.* with the cokernel of $^t u$ since $N^\circ$ is the image of $^t u$.

#### Remark {#evt-iv-s4-n1-rem-1 .statement}

— With the notations of prop. 2, property $b'$) also implies that $u$ is a strict morphism for the weakened topologies (II, p. 49, cor. 3).

#### Proposition 3 {#evt-iv-s4-prop-3 .statement}

*Let E and F be two locally convex spaces, and u a continuous linear mapping from E into F. We assume that E is Hausdorff and that F is metrizable. For u to be a strict morphism, it is necessary and sufficient that the image of $^t u$ be closed in $E'$ for the weak topology $\sigma(E', E)$.*

The necessity follows from prop. 2.

Conversely, suppose that the image of $^t u$ is closed for $\sigma(E', E)$ and introduce the canonical decomposition of $u$ as in the proof of prop. 1. By the above remarks, the inverse mapping $\tilde{u}^{-1}$ of $\tilde{u}$ is continuous for the weakened topologies. But the subspace $M = u(E)$ of F is metrizable, hence bornological (III, p. 12, prop. 2); consequently (IV, p. 7, prop. 7, (ii)), $\tilde{u}^{-1}$ is continuous, hence $u$ is a strict morphism.

### 2. Strict morphisms of Fréchet spaces

#### Theorem 1 {#evt-iv-s4-thm-1 .statement}

*Let E and F be two Fréchet spaces and u a continuous linear mapping from E into F. The following conditions are equivalent :

a) $u$ is a strict morphism.
b) $u$ is a strict morphism for the weakened topologies.
c) The image of $u$ is closed in F.
d) $^t u$ is a strict morphism from $F'$ into $E'$ for the weak topologies.
e) The image of $^t u$ is closed in $E'$ for the weak topology $\sigma(E', E)$.
f) The image of $^t u$ is closed in $E'$ for the strong topology $\beta(E', E)$.
g) $^t u$ is a strict morphism from $F'_c$ into $E'_c$ (the duals endowed with the topology of compact convergence).

The equivalence of a), b) and e) follows from prop. 3 of IV, p. 28 and the remark preceding it. That of a) and c) is precisely cor. 3 of I, p. 19. The remark of IV, p. 28, also shows that d) is equivalent to the fact that, the image of $u$ is closed for the weakened topology $\sigma(F, F')$ of F; the equivalence of c) and d) then follows from prop. 2 of IV, p. 4.

We now prove the equivalence of e) and f). It is enough to prove that f) implies e). Suppose that the image of $^t u$ is closed for $\beta(E', E)$ in $E'$. On account of the Banach-Dieudonné theorem (IV, p. 25, cor. 2), it is enough to prove that for every convex balanced neighbourhood U of 0 in E, the intersection $B = ^t u(F') \cap U$ is compact for $\sigma(E', E)$. The strong dual $E'_b$ of the Fréchet space E is complete (IV, p. 22, prop. 2), hence the closed subset B of $E'_b$ is complete, and so the normed space $E'_B$ is complete (III, p. 8, corollary). Let $(V_n)$ be a decreasing sequence forming a fundamental system of neighbourhoods of 0 in F. Then $F'$ is the union of sets $C = V_n^\circ$ which are compact for $\sigma(F', F)$, hence $E'_B = \bigcup_n B_n$, with $B_n = E'_B \cap ^t u(C_n)$. Since $E'_B$ is a Baire space, and each of the sets $B_n$ is convex balanced and closed, there exists a real number $r > 0$ and an integer $n$ such that $B \subset r.B_n$. Then we have $B = U^\circ \cap {}^t u(r.C_n)$; since the sets $U^\circ$ and $r.C_n$ are compact and ${}^t u$ is continuous for the weak topologies, $B$ is compact for $\sigma(E', E)$. This completes the proof of the equivalence of $e)$ and $f)$.

Finally the equivalence of $g)$ and the preceding conditions follows from prop. 18 of GT, X, § 2, No. 10 and the following lemma.

#### Lemma 1 {#evt-iv-s4-lem-1 .statement}

*Let E and F be two Hausdorff locally convex and quasi-complete spaces and u a continuous linear mapping from E into F. For ${}^t u$ to be a strict morphism from $F'_c$ into $E'_c$, it is necessary and sufficient that the image $u(E)$ of u be closed, and that every compact subset of $u(E)$ be the image under u of a compact subset of E.*

By Mackey’s th. (IV, p. 2, th. 1) and the fact that on $E'$ (resp. F) the topology of compact convergence coincides with that of convex compact convergence (IV, p. 4), we can identity E (resp. F) with the dual $E'_c$ (resp. $F'_c$). Then $u$ is the transpose of ${}^t u$, and the equicontinuous subsets of E (resp. F) are the relatively compact sets. Lemma 1 then follows from prop. 2 (IV, p. 27), since $u(E)$ is closed in F if and only if it is closed for the weakened topology $\sigma(F, F')$ (IV, p. 4, prop. 2).

#### Corollary 1 {#evt-iv-s4-lem-1-cor-1 .statement}

*Under the hypothesis of th. 1, the following conditions are equivalent :*
(i) *u is a strict injective morphism ;*
(ii) *${}^t u$ is a strict surjective morphism for the weak topologies.*
(iii) *${}^t u$ is surjective.*

The implication (i) $\Rightarrow$ (ii) follows immediately from the equivalence of conditions $a)$, $d)$ and $e)$ of th. 1 and from IV, p. 6, prop. 5. It is clear that (ii) implies (iii). Finally, we prove that (iii) implies (i) : if ${}^t u$ is surjective $u$ is a strict morphism by the equivalence of $a)$ and $e)$ in th. 1 ; that $u$ is injective follows from prop. 5 of IV, p. 6.

#### Corollary 2 {#evt-iv-s4-lem-1-cor-2 .statement}

*Under the hypothesis of th. 1, the following conditions are equivalent :*
(i) *u is surjective ;*
(ii) *u is a strict surjective morphism ;*
(iii) *${}^t u$ is a strict injective morphism for the weak topologies.*

The equivalence of (i) and (ii) follows from Banach’s th. (I, p. 17, th. 1).

In view of the equivalence of $a)$ and $c)$ in th. 1, condition (ii) says that $u$ is a strict morphism and that its image is dense in F for $\sigma(F, F')$. The equivalence of (ii) and (iii) then follows from the equivalence of $a)$ and $d)$ in th. 1 and from prop. 5 of IV, p. 6.

If $u : E \to F$ is a strict morphism of Fréchet spaces, the transpose ${}^t u$ is not necessarily a strict morphism from $F'_b$ into $E'_b$ (IV, p. 62, exerc. 3). However, we have the following partial result :

#### Corollary 3 {#evt-iv-s4-lem-1-cor-3 .statement}

— Under the hypotheses of th. 1, the following property implies the properties a) to g) :
h) $^t u$ is a strict morphism from $F'_b$ into $E'_b$.
When E and F are both Banach spaces, or both Montel spaces, property h) is equivalent to the properties a) to g) of th. 1.
Suppose that $^t u$ is a strict morphism from $F'_b$ into $E'_b$. We shall prove that the image H of $^t u$ is closed in $E'_b$, from which the first assertion of cor. 3 will follow.
Let G be the closure of the image of $u$ in F ; the space G, with the topology induced by that of F assigned to it, is a Fréchet space. The mapping $u : E \to F$ factorizes as $u = j \circ v$ where j is the canonical injection from G into F and where $v \in \mathcal{L}(E; G)$. Then we have $^t u = ^t v \circ ^t j$, where $^t j$ is surjective, by Hahn-Banach th. (II, p. 24, prop. 2); also, $^t v$ is injective since $v(E)$ is dense in G (IV, p. 6, prop. 5). By hypothesis, the mapping $^t u$ from $F'_b$ onto H is open ; since $^t j$ is surjective and continuous, the mapping $^t v$ induces a homeomorphism from $G'_b$ onto H. But the dual $G'_b$ of the Fréchet space G is complete (IV, p. 22, prop. 2); consequently H is complete, hence closed in $E'_b$.
If E and F are Montel spaces, the strong topology on $E'$ (resp. $F'$) coincides with the topology of compact convergence, and h) is just a reformulation of g).
If E and F are Banach spaces, so are $E'_b$ and $F'_b$, and condition h) is equivalent to f) by the equivalence of a) and c) applied to $^t u : F'_b \to E'_b$.

#### Corollary 4 {#evt-iv-s4-lem-1-cor-4 .statement}

— Suppose E and F are Banach spaces. For $^t u$ to be surjective, it is necessary and sufficient that there exist a real number $r > 0$ such that $\| x \| \leq r. \| u(x) \|$ for all $x \in E$.
This is simply a reformulation of the equivalence of the conditions (i) and (iii) of cor. 1.

#### Corollary 5 {#evt-iv-s4-lem-1-cor-5 .statement}

— Let E and F be two Fréchet spaces and u a continuous linear mapping from E into F. The following conditions are equivalent :
a) u is an isomorphism from E onto F.
b) u is an isomorphism from E onto F for the weakened topologies.
c) $^t u$ is an isomorphism from $F'$ onto $E'$ for the weak topologies.
d) $^t u$ is an isomorphism from $F'$ onto $E'$ for the strong topologies.
e) $^t u$ is an isomorphism from $F'_c$ onto $E'_c$.
Since an isomorphism is none other than a strict bijective morphism, the equivalence of a) and b) follows from the equivalence of conditions a) and b) of th. 1.
It is clear that a) implies each of the conditions c), d) and e).
Conversely, suppose that one of the conditions c), d) or e) is satisfied. It follows from th. 1 and its cor. 3 that u is a strict morphism from E into F, and $^t u$ is evidently bijective. Let N (resp. I) be the kernel (resp. the image) of u. Since $^t u$ is bijective, we have $\operatorname{Im} ^t u = E'$ and $\operatorname{Ker} ^t u = \{ 0 \}$, and so $N^\circ = E'$ and $I^\circ = \{ 0 \}$ by prop. 2 of IV, p. 27. But N (resp. I) is a closed vector subspace of E (resp. F), and the theorem of bipolars (II, p. 44) implies that $N = \{ 0 \}$ and $I = F$, hence u is bijective. We have therefore proved that u is an isomorphism.

### 3. Criteria for surjectivity

#### Proposition 4 {#evt-iv-s4-prop-4 .statement}

— Let E and F be two Fréchet spaces, and u a continuous linear mapping from E into F. The following conditions are equivalent :

(i) u is surjective.

(ii) For every semi-norm $p \in S(E)$, there exists $q \in S(F)$ such that we have $|f| \leq q$ for every linear form $f \in F'$ satisfying $|f \circ u| \leq p$.

(iii) For every semi-norm $p \in S(E)$, there exists $q \in S(F)$ satisfying the following property : if a linear form $f \in F'$ satisfies $|f \circ u| \leq p$, then $f$ is null on points where $q$ is null and for all $y \in F$, $r \in S(F)$, there exists $x \in E$ with $r(u(x) - y) = 0$.

(iv) For every semi-norm $p \in S(E)$, we have

$$
\sup_{\substack{f \in F \\ |f \circ u| \leq p}} |f(y)| < +\infty \quad \text{for all} \quad y \in F .
$$

We shall prove the proposition according to the following logical scheme

![Diagram showing the logical relationships between (i), (ii), (iii), and (iv)](https://i.imgur.com/3Q5z5QG.png)

If $u$ is surjective, it is a strict morphism (IV, p. 28, th. 1) then for every semi-norm $p \in S(E)$, there exists a semi-norm $q \in S(F)$ such that, for all $y \in F$ satisfying $q(y) \leq 1$, there exists $x \in E$ satisfying $p(x) \leq 1$ and $u(x) = y$. We deduce immediately that (i) implies (ii) and (iii). It is clear that (ii) implies (iv).

To prove that (iii) implies (iv), let $p$ and $q$ be as in (iii). Let $y \in F$, by (iii), there exists $x$ in $E$ such that $q(u(x) - y) = 0$. If $f \in F'$ satisfies $|f \circ u| \leq p$, then we have $f(u(x) - y) = 0$, hence

$$
|f(y)| = |f(u(x))| \leq p(x)
$$

and the relation (1) is satisfied.

Finally we prove that (iv) implies (i). Let $p \in S(E)$ and let $q$ be the superior envelope of the functions $|f|$ for $f \in F'$ satisfying $|f \circ u| \leq p$. By (iv), $q$ is finite on $F$, and is evidently a lower semi-continuous semi-norm on $F$; since $F$ is barrelled (III, p. 25, corollary), we have $q \in S(F)$. Let $B_p$ (resp. $B_q$) denote the set of all $x \in E$ (resp. $y \in F$) such that $p(x) \leq 1$ (resp. $q(y) \leq 1$). We have $q \circ u \leq p$, and so $u(B_p) \subset B_q$. The polar of $u(B_p)$ in $F'$ consists of linear forms $f \in F'$ such that $|f \circ u| \leq p$, hence $|f| \leq q$; in other words, we get $u(B_p)^{\circ} \subset B_q^{\circ}$, and finally that $\overline{u(B_p)} = B_q$ follows from the theorem of bipolars (II, p. 45, cor. 3). If $U$ is a neighbourhood of 0 in $E$, there exists $p \in S(E)$ such that $B_p \subset U$, hence $\overline{u(U)}$ contains the neighbourhood $B_q$ of 0 in $F$. This implies that $u$ is surjective (I, p. 17, th. 1).

#### Corollary {#evt-iv-s4-n3-cor-1 .statement}

— Suppose E and F are Banach spaces. The following conditions are equivalent :
(i) u is surjective.
(ii) There exists a real number r > 0, such that $\|f\| \leq r.\|^{t}u(f)\|$ for all $f \in F'$.
(iii) For all $y \in F$, we have $\sup_{\substack{f \in F' \\ \|f \circ u\| \leq 1}} |f(y)| < + \infty$.

The conditions (ii) and (iii) are in fact reformulations of conditions (ii) and (iv) of prop. 4 for Banach spaces.

### Exercises {#evt-iv-s4-exercises}

See the [exercises for § 4](exercises/s4/).
