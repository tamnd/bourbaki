---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: II
chapter_title: FREE LIE ALGEBRAS
section: 4
section_title: Central filtrations
lang: en
source: lie-i-iii
pdf_pages: 0160-0167, 0205-0211
extraction: ocr
subsections:
    - "no": 1
      title: REAL FILTRATIONS
      page: 0
      pdf_page: 160
    - "no": 2
      title: ORDER FUNCTION
      page: 0
      pdf_page: 161
    - "no": 3
      title: GRADED ALGEBRA ASSOCIATED WITH A FILTERED ALGEBRA
      page: 0
      pdf_page: 162
    - "no": 4
      title: CENTRAL FILTRATIONS ON A GROUP
      page: 0
      pdf_page: 163
    - "no": 5
      title: AN EXAMPLE OF A CENTRAL FILTRATION
      page: 0
      pdf_page: 165
    - "no": 6
      title: INTEGRAL CENTRAL FILTRATIONS
      page: 0
      pdf_page: 166
statements: 12
exercises: 18
content_sha256: 1325ad90b6f64f40c918361f53780fe37c172750b745daa70223fd8d6caff02f
---

## § 4. CENTRAL FILTRATIONS

### 1. REAL FILTRATIONS

#### Definition 1 {#lie-ii-s4-def-1 .statement}

Let $G$ be a group. A real filtration on $G$ is a family $(G_\alpha)_{\alpha \in \mathbf{R}}$ of subgroups of $G$ such that
$$
G_\alpha = \bigcap_{\beta < \alpha} G_\beta \quad \text{for all } \alpha \in \mathbf{R}.
$$

Formula (1) implies $G_\alpha \subset G_\beta$ for $\beta < \alpha$ and hence the family $(G_\alpha)$ is *decreasing*. The filtration $(G_\alpha)$ is called *separated* if $\bigcap_\alpha G_\alpha$ reduces to the identity element and is called *exhaustive* if $G = \bigcup_\alpha G_\alpha$.

#### Remark {#lie-ii-s4-n1-rem-1 .statement}

Let $(G_n)_{n \in \mathbf{Z}}$ be a decreasing sequence of subgroups of $G$. It is a decreasing filtration in the sense of *Commutative Algebra*, Chapter III, § 2, no. 1, Definition 1. For every integer $n$ and all $\alpha$ in the interval $]n-1, n]$ of $\mathbf{R}$, we write $H_\alpha = G_n$, in particular $H_n = G_n$. It is immediate that we thus obtain a real filtration $(H_\alpha)_{\alpha \in \mathbf{R}}$ on $G$; such a filtration will be called an *integral filtration*. Hence decreasing filtrations in the sense of *Commutative Algebra*, Chapter III, § 2, can be identified with integral filtrations.

Let $A$ be an algebra; a real filtration $(A_\alpha)$ on the additive group of $A$ is called compatible with the algebra structure if $A_\alpha . A_\beta \subset A_{\alpha + \beta}$ for $\alpha, \beta$ in $\mathbf{R}$ and $K . A_\alpha \subset A_\alpha$ for $\alpha \in \mathbf{R}$. If the filtration is exhaustive, $(A_\alpha)$ is a fundamental system of neighbourhoods of 0 under the topology on $A$ which is compatible with the algebra structure. Let $B$ be a unital algebra; a real filtration $(B_\alpha)$ on the additive group of $B$ is called compatible with the unital algebra structure if it is compatible with the algebra structure and $1 \in B_0$.

### 2. ORDER FUNCTION

Let $G$ be a group with identity element $e$. Let $(G_\alpha)$ be a real filtration on $G$. For all $x$ in $G$ let $I_x$ denote the set of real numbers $\alpha$ such that $x \in G_\alpha$. If $\alpha \in I_x$ and $\beta < \alpha$, then $\beta \in I_x$ and hence $I_x$ is an interval (*General Topology*, Chapter IV, § 2, no. 4, Proposition 1). Using relation (1), we see that $I_x$ contains its least upper bound when this is finite. Therefore $I_x$ is of the form $]-\infty, v(x)] \cap \mathbf{R}$ with $v(x) \in \overline{\mathbf{R}}$; we have $v(x) = \sup \{ \alpha \mid x \in G_\alpha \}$.

The mapping $v$ of $G$ into $\overline{\mathbf{R}}$ is called the *order function* associated with the real filtration $(G_\alpha)$ and $v(x)$ is called the *order* of $x$. This mapping has the following properties:

(a) *For $x \in G$ and $\alpha \in \mathbf{R}$, the relations $x \in G_\alpha$ and $v(x) \geq \alpha$ are equivalent.*

(b) *For $x, y$ in $G$,*
$$
v(x^{-1}) = v(x), \qquad v(e) = +\infty.
$$
$$
v(xy) \geq \inf(v(x), v(y)).
$$

*Further, we have equality in (3) if $v(x) > v(y)$.*

(c) *For all $\alpha \in \mathbf{R}$, let $G_\alpha^+$ denote the set of $x \in G$ such that $v(x) > \alpha$. Then $G_\alpha^+ = \bigcup_{\beta > \alpha} G_\beta$ and in particular $G_\alpha^+$ is a subgroup of $G$.*

Conversely, let $v$ be a mapping of $G$ into $\overline{\mathbf{R}}$ satisfying relations (2) and (3). For all $\alpha \in \mathbf{R}$, let $G_\alpha$ be the set of $x \in G$ such that $v(x) \geq \alpha$. Then $(G_\alpha)_{\alpha \in \mathbf{R}}$ is a real filtration of $G$ and $v$ is the order function associated with this filtration.

For the filtration $(G_\alpha)$ to be integral, it is necessary and sufficient that $v$ map $G$ into $\mathbf{Z} \cup \{+\infty, -\infty\}$. For it to be exhaustive (resp. separated), it is necessary and sufficient that $-v^{-1}(-\infty) = \varnothing$ (resp. $-v^{-1}(+\infty) = \{\epsilon\}$.

Let $A$ be a K-algebra (resp. unital K-algebra). By the above, the relation

$$
"x \in A_\alpha \Leftrightarrow v(x) \geq \alpha \quad \text{for } x \in A \text{ and } \alpha \in \mathbf{R}"
$$

defines a bijection of the set of exhaustive real filtrations $(A_\alpha)_{\alpha \in \mathbf{R}}$ compatible with the algebra (resp. unital algebra) structure on $A$ onto the set of mappings $v : A \to \overline{\mathbf{R}}$ not taking the value $-\infty$ and satisfying axioms (4) to (7) (resp. (4) to (8)) below:

(4) $$v(x + y) \geq \inf(v(x), v(y)) \quad (x, y \text{ in } A)$$
(5) $$v(-x) = v(x) \qquad (x \in A)$$
(6) $$v(\lambda x) \geq v(x) \qquad (\lambda \in K, x \in A)$$
(7) $$v(xy) \geq v(x) + v(y) \qquad (x, y \text{ in } A)$$
(8) $$v(1) \geq 0.$$

#### Remark {#lie-ii-s4-n2-rem-1 .statement}

If $v(x)$ is not everywhere equal to $+\infty$, conditions (7) and (8) imply $v(1) = 0$.

### 3. GRADED ALGEBRA ASSOCIATED WITH A FILTERED ALGEBRA

Let $G$ be a *commutative* group with a real filtration $(G_\alpha)_{\alpha \in \mathbf{R}}$. As before we write

$$
G_\alpha^+ = \bigcup_{\beta > \alpha} G_\beta;
$$

clearly $G_\alpha^+$ is a subgroup of $G_\alpha$. We write $\operatorname{gr}_\alpha(G) = G_\alpha / G_\alpha^+$ and

$$
\operatorname{gr}(G) = \bigoplus_{\alpha \in \mathbf{R}} \operatorname{gr}_\alpha(G).
$$

The *graded group associated with the filtered group* $G$ is the group $\operatorname{gr}(G)$ with its natural graduation of type $\mathbf{R}$.

#### Remark {#lie-ii-s4-n3-rem-1 .statement}

When the filtration $(G_\alpha)$ is integral, $\operatorname{gr}_\alpha(G) = \{0\}$ for non-integral $\alpha$ and $\operatorname{gr}_n(G) = G_n / G_{n-1}$ for every integer $n$. The definition of the associated graded group therefore coincides essentially with that of *Commutative Algebra*, Chapter III, § 2, no. 3.

Let $A$ be an algebra (resp. unital algebra) and $(A_\alpha)_{\alpha \in \mathbf{R}}$ a real filtration compatible with the algebra (resp. unital algebra) structure (no. 1). Then

$$
A_\alpha \cdot A_\beta \subset A_{\alpha + \beta}, \qquad A_\alpha^+ \cdot A_\beta + A_\alpha \cdot A_\beta^+ \subset A_{\alpha + \beta}^+
$$

and the bilinear mapping of $A_\alpha \times A_\beta$ into $A_{\alpha + \beta}$ the restriction of multiplication on $A$ defines on taking quotients a bilinear mapping

$$
\operatorname{gr}_\alpha(A) \times \operatorname{gr}_\beta(A) \to \operatorname{gr}_{\alpha + \beta}(A).
$$

We derive a bilinear mapping of gr(A) × gr(A) into gr(A) which makes it a graded algebra (resp. unital graded algebra) of type $\mathbf{R}$. If A is an associative (resp. commutative, resp. Lie) algebra, so is gr(A).

### 4. CENTRAL FILTRATIONS ON A GROUP

#### Definition 2 {#lie-ii-s4-def-2 .statement}

Let G be a group. A real filtration $(G_\alpha)$ on G is called central if $G = \bigcup_{\alpha > 0} G_\alpha$ and the commutator $(x, y) = x^{-1}y^{-1}xy$ of an element x of $G_\alpha$ and an element y of $G_\beta$ belongs to $G_{\alpha + \beta}$.

In terms of the order function v, the above definition translates into the relations
$$
v(x) > 0, \quad v((x, y)) \geq v(x) + v(y) \quad \text{for all } x, y \text{ in } G.
$$
We deduce that $v((x, y)) > v(x)$ if $v(x) \neq +\infty$; if we write $x^y = y^{-1}xy$ (cf. Algebra, Chapter I, § 6, no. 2), then $x^y = x.(x, y)$, whence
$$
v(x^y) = v(x).
$$
This relation expresses the fact that each of the subgroups $G_\alpha$ of G is normal. The $G_\alpha$ form a fundamental system of neighbourhoods of e for a topology compatible with the group structure on G (General Topology, Chapter III, § 1, no. 2, Example) said to be defined by the filtration $(G_\alpha)$.

In the rest of this no., G denotes a group with a central filtration $(G_\alpha)$. For all $\alpha \in \mathbf{R}$, we define the subgroup $G_\alpha^+$ of G by
$$
G_\alpha^+ = \bigcup_{\beta > \alpha} G_\beta.
$$
In particular $G_\alpha^+ = G_\alpha = G$ for $\alpha \leq 0$. Recall that if A and B are two subgroups of G, (A, B) denotes the subgroup of G generated by the commutators $(a, b)$ with $a \in A$ and $b \in B$. With this notation we have the formulae
$$
(G_\alpha, G_\beta) \subset G_{\alpha + \beta}
$$
$$
(G_\alpha^+, G_\beta^+) \subset G_{\alpha + \beta}^+
$$
$$
(G, G_\alpha) \subset G_\alpha^+.
$$
By (14), $G_\alpha^+$ is a normal subgroup of $G_\alpha$ for all $\alpha \in \mathbf{R}$ and the quotient group $\mathrm{gr}_\alpha(G) = G_\alpha / G_\alpha^+$ is commutative. We write $\mathrm{gr}(G) = \bigoplus_{\alpha \in \mathbf{R}} \mathrm{gr}_\alpha(G)$ and give this group the graduation of type $\mathbf{R}$ in which $\mathrm{gr}_\alpha(G)$ consists of elements of degree $\alpha$. Then $\mathrm{gr}_\alpha(G) = \{0\}$ for $\alpha \leq 0$.

#### Proposition 1 {#lie-ii-s4-prop-1 .statement}

(i) Let $\alpha, \beta$ be in $\mathbf{R}$. There exists a biadditive mapping
$$
\phi_{\alpha \beta} : \mathrm{gr}_\alpha(G) \times \mathrm{gr}_\beta(G) \to \mathrm{gr}_{\alpha + \beta}(G)
$$

which maps $(xG_\alpha^+, yG_\beta^+)$ onto $(x, y)G_{\alpha+\beta}^+$.

(ii) Let $\phi$ be the biadditive mapping of $\mathrm{gr}(G) \times \mathrm{gr}(G)$ into $\mathrm{gr}(G)$ whose restriction to $\mathrm{gr}_\alpha(G) \times \mathrm{gr}_\beta(G)$ is $\phi_{\alpha\beta}$ for every ordered pair $(\alpha, \beta)$. The mapping $\phi$ gives $\mathrm{gr}(G)$ a Lie $\mathbf{Z}$-algebra structure.

(i) Recall the identity

$$(xx', y) = (x, y)x'(x', y)$$

for $x, x', y$ in $G$ (*Algebra*, Chapter I, § 6, no. 2, formula (4 bis)).

For $x \in G_\alpha$ and $y \in G_\beta$, the class modulo $G_{\alpha+\beta}^+$ of the element $(x, y)$ of $G_{\alpha+\beta}$ will be denoted by $f(x, y)$. For $a$ in $G_{\alpha+\beta}$ and $x'$ in $G$, $a^{-1}.ax' = (a, x') \in G_{\alpha+\beta}^+$; in particular $f(x, y)$ is equal to the class modulo $G_{\alpha+\beta}^+$ of $(x, y)x'$. Formula (15) therefore implies

$$f(xx', y) = f(x, y)f(x', y).$$

Now $(y, x) = (x, y)^{-1}$, whence

$$f(y, x) = f(x, y)^{-1}.$$

From (16) and (17) we deduce

$$f(x, yy') = f(x, y)f(x, y').$$

We have to prove that the mapping $f : G_\alpha \times G_\beta \to \mathrm{gr}_{\alpha+\beta}(G)$ defines on taking quotients a mapping $\phi_{\alpha\beta} : \mathrm{gr}_\alpha(G) \times \mathrm{gr}_\beta(G) \to \mathrm{gr}_{\alpha+\beta}(G)$. By (16) and (18) it suffices to prove that $f(x, y) = 0$ if $x \in G_\alpha^+$ or $y \in G_\beta^+$, which follows from (13').

(ii) As $(x, x) = e$, it follows from (17) that $\phi$ is an alternating $\mathbf{Z}$-bilinear mapping. Hence it remains to prove that, for $u \in \mathrm{gr}_\alpha(G)$, $v \in \mathrm{gr}_\beta(G)$ and $w \in \mathrm{gr}_\gamma(G)$,

$$\phi(u, \phi(v, w)) + \phi(v, \phi(w, u)) + \phi(w, \phi(u, v)) = 0.$$

Let $x \in G_\alpha, y \in G_\beta$ and $z \in G_\gamma$ be elements representing respectively $u, v$ and $w$. We know that $x^y$ and $x$ are two elements of $G_\alpha$ which are congruent modulo $G_\alpha^+$ and hence $x^y$ is a representative of $u$ in $G_\alpha$; as $(y, z)$ is a representative of $\phi(v, w)$ in $G_{\beta+\gamma}$, we see that $(x^y, (y, z))$ is a representative of $\phi(u, \phi(v, w))$ in $G_{\alpha+\beta+\gamma}$. By cyclic permutation, we see that $(y^z, (z, x))$ and $(z^x, (x, y))$ represent respectively $\phi(v, \phi(w, u))$ and $\phi(w, \phi(u, v))$ in $G_{\alpha+\beta+\gamma}$. Relation (19) is then a consequence of the following identity (*Algebra*, Chapter I, § 6, no. 2, formula (15)):

$$(x^y, (y, z)).(y^z, (z, x)).(z^x, (x, y)) = e.$$

The Lie algebra $\mathrm{gr}(G)$ over $\mathbf{Z}$ defined in Proposition 1 is called the *graded Lie algebra associated with the filtered group* $G$.

### 5. AN EXAMPLE OF A CENTRAL FILTRATION

Let $A$ be a unital associative algebra with a unital algebra filtration $(A_\alpha)$ such that $A_0 = A$; then $A_\alpha$ is a two-sided ideal of $A$ for all $\alpha \in \mathbf{R}$. Let $A^*$ denote the multiplicative group of invertible elements of $A$. For all $\alpha > 0$, let $\Gamma_\alpha$ denote the set of $x \in A^*$ such that $x - 1 \in A_\alpha$; we write $\Gamma = \bigcup_{\alpha > 0} \Gamma_\alpha$ and $\Gamma_\beta = \Gamma$ for $\beta \leq 0$.

#### Proposition 2 {#lie-ii-s4-prop-2 .statement}

*The set $\Gamma$ is a subgroup of $A^*$ and $(\Gamma_\alpha)$ is a central filtration on $\Gamma$.*

$\Gamma = \bigcup_{\alpha > 0} \Gamma_\alpha$ by construction and the relation $\Gamma_\alpha = \bigcap_{\beta < \alpha} \Gamma_\beta$ follows from $A_\alpha = \bigcap_{\beta < \alpha} A_\beta$.

We show that $\Gamma_\alpha$ is a subgroup of $A^*$. Now $1 \in \Gamma_\alpha$; let $x, y$ be in $\Gamma_\alpha$, whence $x - 1 \in A_\alpha, y - 1 \in A_\alpha$. As $A_\alpha$ is a two-sided ideal of $A$, the formulae
$$
(21) \quad xy - 1 = (x - 1)(y - 1) + (x - 1) + (y - 1),
$$
$$
(22) \quad x^{-1} - 1 = -x^{-1}(x - 1),
$$
imply $xy - 1 \in A_\alpha$ and $x^{-1} - 1 \in A_\alpha$, whence $xy \in \Gamma_\alpha$ and $x^{-1} \in \Gamma_\alpha$.

As $\Gamma = \bigcup_{\alpha > 0} \Gamma_\alpha$, this is a subgroup of $A^*$.

Finally let $\alpha > 0, \beta > 0, x \in \Gamma_\alpha$ and $y \in \Gamma_\beta$. Let $x - 1 = \xi$ and $y - 1 = \eta$. Then
$$
(23) \quad (x, y) - 1 = x^{-1}y^{-1}(\xi \eta - \eta \xi);
$$
by hypothesis, $\xi \in A_\alpha$ and $\eta \in A_\beta$, whence $\xi \eta - \eta \xi \in A_{\alpha + \beta}$. As $A_{\alpha + \beta}$ is a two-sided ideal of $A$, $(x, y) - 1 \in A_{\alpha + \beta}$, whence $(x, y) \in \Gamma_{\alpha + \beta}$.

#### Remark {#lie-ii-s4-n5-rem-1 .statement}

Let $\alpha \geq 0, \beta \geq 0$ and $x \in \Gamma_\alpha, y \in \Gamma_\beta$. By formulae (21), (22) and (23),
$$
(24) \quad x^{-1} - 1 \equiv -(x - 1) \pmod{A_{2\alpha}}
$$
$$
(25) \quad xy - 1 \equiv (x - 1) + (y - 1) \pmod{A_{\alpha + \beta}}
$$
$$
(26) \quad (x, y) - 1 \equiv [(x - 1), (y - 1)] \pmod{A_{\alpha + \beta + \inf(\alpha, \beta)}}.
$$

We prove for example (26). If $x - 1 = \xi$ and $y - 1 = \eta$, (23) gives:
$$
(x, y) - 1 - [\xi, \eta] = ((x^{-1} - 1) + (y^{-1} - 1) + (x^{-1} - 1)(y^{-1} - 1))[\xi, \eta].
$$
Now $[\xi, \eta] \in A_{\alpha + \beta}$, $(x^{-1} - 1) \in A_\alpha$, $(y^{-1} - 1) \in A_\beta$, whence we obtain (26).

Let $G$ be a group and $\rho : G \to \Gamma$ a homomorphism. For all real $\alpha$, we write $G_\alpha = \rho^{-1}(\Gamma_\alpha)$. As $(\Gamma_\alpha)$ is a central filtration on $\Gamma$, it is immediate that $(G_\alpha)$ is a central filtration on $G$.

#### Proposition 3 {#lie-ii-s4-prop-3 .statement}

(i) *For all $\alpha \in \mathbf{R}$, there exists a unique group homomorphism $g_\alpha : \mathrm{gr}_\alpha(G) \to \mathrm{gr}_\alpha(A)$ which maps the class modulo $G_\alpha^+$ of an element $a \in G_\alpha$ to the class modulo $A_\alpha^+$ of $\rho(a) - 1$.*

(ii) Let g be the group homomorphism of gr(G) into gr(A) whose restriction to gr_\alpha(G) is g_\alpha for all \alpha. The mapping g is an injective homomorphism of Lie \mathbf{Z}-algebras.

(i) Let \alpha > 0. By hypothesis, for all a in G_\alpha, \rho(a) - 1 \in A_\alpha; let p_\alpha(a) denote the class of \rho(a) - 1 modulo A_\alpha^+. As A_{2\alpha} \subset A_\alpha^+, relation (25) implies p_\alpha(ab) = p_\alpha(a) + p_\alpha(b). Then a \in G_\alpha^+ if and only if \rho(a) - 1 \in A_\alpha^+; therefore G_\alpha^+ is the kernel of the homomorphism p_\alpha of G_\alpha into gr_\alpha(A). On passing to the quotient, p_\alpha then defines an injective homomorphism g_\alpha of gr_\alpha(G) into gr_\alpha(A).

For \alpha \leq 0, gr_\alpha(G) = \{0\} and the only choice is g_\alpha = 0.

(ii) As g_\alpha is injective for all real \alpha, g is injective. We show that g is a Lie algebra homomorphism. As gr_\alpha(G) = \{0\} for \alpha \leq 0, it suffices to establish the formula

$$
p_{\alpha+\beta}((a, b)) = [p_\alpha(a), p_\beta(b)]
$$

for \alpha > 0, \beta > 0, \rightarrow \in G_\alpha and b \in G_\beta, which follows from (26).

### 6. INTEGRAL CENTRAL FILTRATIONS

Recall (no. 1, Remark) that a filtration (G_\alpha) on the group G is called integral if G_\alpha = G_n for every integer n and all \alpha \in \{n-1, n\}. To be given an integral central filtration on a group G is equivalent to being given a sequence (G_n)_{n \geq 1} of subgroups of G satisfying the conditions

(i) \quad G_1 = G
(ii) \quad G_n \supset G_{n+1} \quad \text{for all } n \geq 1
(iii) \quad (G_m, G_n) \subset G_{m+n} \quad \text{for } m \geq 1 \text{ and } n \geq 1.

For every integer n \geq 1, G_n is a normal subgroup of G and the quotient gr_n(G) = G_n/G_{n+1} is commutative. On taking quotients, the mapping (x, y) \mapsto (x, y) = x^{-1}y^{-1}xy of G_m \times G_n into G_{m+n} allows us to define on gr(G) = \bigoplus_{n \geq 1} gr_n(G) a graded Lie algebra structure of type \mathbf{N} over the ring \mathbf{Z}.

Recall (Algebra, Chapter I, § 6, no. 3, Definition 5) that the lower central series of the group G is defined by

$$
C^1G = G, \quad C^{n+1} = (G, C^nG) \quad \text{for } n \geq 1.
$$

The corresponding filtration is called the lower central filtration of G.

#### Proposition 4 {#lie-ii-s4-prop-4 .statement}

(i) The lower central series of G is an integral central filtration on G.

(ii) If (G_n)_{n \in \mathbf{N}^*} is an integral central filtration on G, then C^nG \subset G_n for all n \in \mathbf{N}^*.

Assertion (i) has been proved in Algebra, Chapter I, § 6, no. 3, formula (7).

We prove (ii) by induction on n; C^1G = G = G_1; for n > 1,

$$
C^nG = (G, C^{n-1}G) \subset (G, G_{n-1}) \subset G_n.
$$

#### Proposition 5 {#lie-ii-s4-prop-5 .statement}

Let G be a group and gr(G) the graded Lie $\mathbf{Z}$-algebra associated with the lower central filtration on G. Then gr(G) is generated by $\mathrm{gr}_1(G) = G/(G, G)$.

Let L be the Lie subalgebra of gr(G) generated by $\mathrm{gr}_1(G)$; we show that $L \supset \mathrm{gr}_n(G)$ by induction on n, the assertion being trivial for $n = 1$. Suppose that $n > 1$ and $L \supset \mathrm{gr}_{n-1}(G)$. As $C^nG = (G, C^{n-1}G)$, the construction of the Lie algebra law on gr(G) shows immediately that

$$
\mathrm{gr}_n(G) = [\mathrm{gr}_1(G), \mathrm{gr}_{n-1}(G)] \subset L.
$$

The above proof shows that the lower central series of the Lie algebra gr(G) (§ 2, no. 7) is given by

$$
\mathcal{C}^n(\mathrm{gr}(G)) = \sum_{m \geq n} \mathrm{gr}_m(G).
$$

#### Remark {#lie-ii-s4-n6-rem-1 .statement}

Let k be a ring, n an integer $> 0$ and A the set of lower triangular matrices with n rows and n columns and elements in k. For $p \geq 0$, let $A_p$ be the set of $(x_{ij}) \in A$ such that $x_{ij} = 0$ for $i - j < p$. Then $A_0 = A$ and $A_pA_q \subset A_{p+q}$. Let $\Gamma_p = 1 + A_p$. Then $\Gamma_1$ is a subgroup of $\mathbf{GL}(n, k)$ called the strict lower triangular group of order n over k. By Proposition 2 of no. 5, $(\Gamma_p)$ is an integral filtration on $\Gamma_1$. As $\Gamma_n = \{1\}$, we see that the group $\Gamma_1$ is nilpotent (Algebra, Chapter I, § 6, no. 3, Definition 6).

### Exercises {#lie-ii-s4-exercises}

In the following exercises the letter G denotes a group.

See the [exercises for § 4](exercises/s4/).
