---
book: alg
book_title: Algebra
chapter: I
chapter_title: ALGEBRAIC STRUCTURES
section: 5
section_title: Groups operating on a set
lang: en
source: alg-i-iii
source_edition: 1998, Springer
pdf_pages: 0076-0089, 0164-0171
extraction: ocr
subsections:
    - "no": 1
      title: MONOID OPERATING ON A SET
      page: 0
      pdf_page: 76
    - "no": 2
      title: STABILIZER, FIXER
      page: 0
      pdf_page: 78
    - "no": 3
      title: INNER AUTOMORPHISMS
      page: 0
      pdf_page: 79
    - "no": 4
      title: ORBITS
      page: 0
      pdf_page: 80
    - "no": 5
      title: HOMOGENEOUS SETS
      page: 0
      pdf_page: 82
    - "no": 6
      title: HOMOGENEOUS PRINCIPAL SETS
      page: 0
      pdf_page: 84
    - "no": 7
      title: PERMUTATION GROUPS OF A FINITE SET
      page: 0
      pdf_page: 85
statements: 32
exercises: 29
content_sha256: 605c0e618797b31a8a044a2bed5b6ec188866b18a0efb8640705a9dbb17c2a1b
---

## § 5. GROUPS OPERATING ON A SET

### 1. MONOID OPERATING ON A SET

#### Definition 1 {#alg-i-s5-def-1 .statement}

Let M be a monoid, with law written multiplicatively and identity element denoted by e, and E a set. An action $\alpha \mapsto f_\alpha$ of M on E is called a left (resp. right) operation of M on E if $f_e = \mathrm{Id}_E$ and $f_{\alpha \beta} = f_\alpha \circ f_\beta$ (resp. $f_{\alpha \beta} = f_\beta \circ f_\alpha$) for all $\alpha, \beta \in M$.

In other words, a left (resp. right) operation of a monoid M on a set E is a monoid homomorphism of M into the monoid $E^E$ (resp. the opposite monoid of $E^E$) with composition of mappings. If the law of action corresponding to the action of M is denoted by left (resp. right) multiplication, the fact that this action is a left (resp. right) operation may be expressed by the formulae

(1)
$$
e.x = x; \quad \alpha.(\beta.x) = (\alpha \beta).x \quad \text{for } \alpha, \beta \in M \text{ and } x \in E.
$$
(resp. $x.e = x; \quad (x.\alpha).\beta = x.(\alpha \beta) \quad \text{for } \alpha, \beta \in M \text{ and } x \in E$).

Under these conditions, it is also said that M operates on E on the left (resp. right) and that the corresponding laws of action are laws of left (resp. right) operation of the monoid M on E.

Let M be a monoid; a set E with a left (resp. right) operation of M on E is called a left (resp. right) M-set. The monoid M is said to operate on the left (resp. right) faithfully if the mapping $\alpha \mapsto f_\alpha$ of M into $E^E$ is injective.

#### Example {#alg-i-s5-n1-exa-1 .statement}

(1) Let E be a set; the canonical action of $E^E$ on E (§ 3, no. 1, Example 3) is a left operation.

(2) Let M be a monoid. The left (resp. right) action of M on itself derived from the law on M (§ 3, no. 3, Example 7) is a left (resp. right) operation of M on itself. When considering this operation, we say that M operates on itself by left (resp. right) translation.

Let E be a left (resp. right) M-set and $M^0$ the opposite monoid to M. Under the same action, the monoid $M^0$ operates on E on the right (resp. left). The $M^0$-set obtained is called opposite to the M-set E. The definitions and results relating to left M-sets carry over to right $M^0$-sets when passing to the opposite structures.

In the rest of this paragraph, we shall consider, unless otherwise stated, only left M-sets which we shall call simply M-sets. Their law of action will be denoted by left multiplication.

Let E be a set. Let G be a group operating on E. For all $\alpha$ in G, the element of $E^E$ defined by $\alpha$ is a permutation of E ($\S$ 2, no. 3, Example 2). Being given an operation of G on E therefore amounts to being given a homomorphism of G into $\mathfrak{S}_E$.

In conformity with $\S$ 3, no. 3, we make the following definition:

#### Definition 2 {#alg-i-s5-def-2 .statement}

*Let M be a monoid and E and E' M-sets. A mapping f of E into E' such that, for all $x \in E$ and all $\alpha \in M$, $f(\alpha.x) = \alpha.f(x)$ is called an M-set homomorphism (or M-morphism, or mapping compatible with the operations of M).*

The identity mapping of an M-set is an M-morphism. The composition of two M-morphisms is an M-morphism. For a mapping of one M-set into another to be an isomorphism, it is necessary and sufficient that it be a bijective M-morphism and the inverse mapping is then an M-morphism.

Let $(E_i)_{i \in I}$ be a family of M-sets and let E be the product set of $E_i$. The monoid M operates on E by $\alpha.(x_i)_{i \in I} = (\alpha.x_i)_{i \in I}$ and E, with this action, is an M-set; let E' be an M-set; a mapping f of E' into E is an M-morphism if and only if $pr_i \circ f$ is an M-morphism of E' into $E_i$ for all $i \in I$.

Let E be an M-set and F a stable subset of E under the action of M; with the induced law, F is an M-set and the canonical injection $F \to E$ is an M-morphism.

Let E be an M-set and R an equivalence relation on E compatible with the action of M; the quotient $E/R$ with the quotient action is an M-set and the canonical mapping $E \to E/R$ is an M-morphism.

Let $\phi : M \to M'$ be a monoid homomorphism, E an M-set and E' an $M'$-set. A mapping f of E into E' such that, for all $x \in E$ and $\alpha \in M$,

$$
f(\alpha.x) = \phi(\alpha).f(x)
$$

is called a $\phi$-morphism of E into E' (cf. $\S$ 3, no. 1).

*Extension of a law of operation.* Given (for example) three sets $F_1, F_2, F_3$, permutations $f_1, f_2, f_3$ of $F_1, F_2, F_3$ respectively and an echelon F on the base sets $F_1, F_2, F_3$ (*Set Theory*, IV, $\S$ 1, no. 1), we can define, proceeding step by step on the construction of the echelon F, a permutation of F called the *canonical extension* of $f_1, f_2, f_3$ to F (*Set Theory*, IV, $\S$ 1, no. 2); we shall denote it by $\phi_F(f_1, f_2, f_3)$.

Then let G be a group and $h_i$ a homomorphism of G into the symmetric group of $F_i$ ($i = 1, 2, 3$), in other words an operation of G on $F_i$. The mapping $x \mapsto x_F = \phi_F(h_1(x), h_2(x), h_3(x))$ is a homomorphism of G into $\mathfrak{S}_F$, in other words an operation of G on F, called the *extension* of $h_1, h_2, h_3$ to F. Let P be a subset of F such that, for all $x \in G$, $x_F(P) = P$; let $x_P$ be the restriction of $x_F$ to

P; then the mapping $x \mapsto x_P$ is an operation of G on P, also called the extension of $h_1, h_2, h_3$ to P.

For example, let K and L be two echelons on $F_1, F_2, F_3$; take F to be the set of subsets of $K \times L$ and P to be the set of mappings of K into L, identified with their graphs. If $w \in P$ and $x \in G$, $x_P(w)$ is the mapping $k \mapsto x_L(w(x_K^{-1}(k)))$ of K into L.

### 2. STABILIZER, FIXER

#### Definition 3 {#alg-i-s5-def-3 .statement}

*Let M be a monoid operating on a set E and A and B subsets of E. The set of $\alpha \in M$ such that $\alpha A \subset B$ (resp. $\alpha A = B$) is called the transporter (resp. strict transporter) of A to B. The transporter (resp. strict transporter) of A to A is called the stabilizer (resp. strict stabilizer) of A. The set of $\alpha \in M$ such that $\alpha a = a$ for all $a \in A$ is called the fixer of A.*

An element $\alpha$ of M is said to stabilize (resp. stabilize strictly, resp. fix) a subset A of E if $\alpha$ belongs to the stabilizer (resp. strict stabilizer, resp. fixer) of A. A subset P of M is said to stabilize (resp. stabilize strictly, resp. fix) a subset A of E if all the elements of P stabilize (resp. strictly stabilize, resp. fix) A. The fixer of A is contained in the strict stabilizer of A which itself is contained in the stabilizer of A.

#### Proposition 1 {#alg-i-s5-prop-1 .statement}

*Let M be a monoid operating on a set E and A a subset of E.*
(a) *The stabilizer, strict stabilizer and fixer of A are submonoids of M.*
(b) *Let $\alpha$ be an invertible element of M; if $\alpha$ belongs to the strict stabilizer (resp. fixer) of A, so does $\alpha^{-1}$.*

Let e be the identity element of M; then $ea = a$ for every element $a \in A$ and therefore e belongs to the fixer of A. Let $\alpha$ and $\beta$ be elements of E which stabilize A. Then $(\alpha \beta)A = \alpha(\beta A) \subset \alpha A \subset A$ and therefore the stabilizer of A is a submonoid of M. Similarly for the strict stabilizer and fixer of A, whence (a). If $\alpha A = A$, then $A = \alpha^{-1}(\alpha A) = \alpha^{-1}A$. If for all $a \in A$, $\alpha a = a$, then $a = \alpha^{-1}(\alpha a) = \alpha^{-1}a$, whence (b).

#### Corollary {#alg-i-s5-n2-cor-1 .statement}

*Let G be a group operating on a set E and A be a subset of E. The strict stabilizer S and the fixer F of A are subgroups of G and F is a normal subgroup of S.*

The first assertion follows from the proposition and F is the kernel of the homomorphism of S into $\mathfrak{S}_A$ associated with the operation of S on A.

A group G operates faithfully on a set E if and only if the fixer of E consists of the identity element of G. The fixer of E is the kernel of the given homomorphism of G into $\mathfrak{S}_E$; this homomorphism is injective if and only if its kernel consists of the identity element (§ 4, no. 5, Theorem 3).

Let M be a monoid, E an M-set and $a$ an element of E. The fixer, strict stabilizer and stabilizer of $\{a\}$ are equal; this monoid is called equally the fixer or stabilizer of $a$. The fixer of a subset A of E is the intersection of the fixers of the elements of A. $a$ is called an invariant element of E if the fixer of $a$ is the monoid M. M is said to operate trivially on E if every element of E is invariant.

#### Proposition 2 {#alg-i-s5-prop-2 .statement}

*Let G be a group operating on a set E and, for all $x \in E$, let $S_x$ be the stabilizer of x. For all $\alpha \in G$, $S_{\alpha x} = \alpha S_x \alpha^{-1}$.*

If $s \in S_x$, then $\alpha s \alpha^{-1}(\alpha x) = \alpha s x = \alpha x$, whence $\alpha S_x \alpha^{-1} \subset S_{\alpha x}$. As $x = \alpha^{-1}(\alpha x)$, $\alpha^{-1} S_{\alpha x} \alpha \subset S_x$, whence $S_{\alpha x} \subset \alpha S_x \alpha^{-1}$.

It is seen similarly that, if A and B are two subsets of E and T is the transporter (resp. strict transporter) of A to B, then the transporter (resp. strict transporter) of $\alpha A$ to $\alpha B$ is equal to $\alpha T \alpha^{-1}$.

### 3. INNER AUTOMORPHISMS

Let G be a group. The set Aut(G) of automorphisms of the group G is a subgroup of $\mathcal{G}_G$ (§ 4, no. 1, Example 2).

#### Proposition 3 {#alg-i-s5-prop-3 .statement}

*Let G be a group. For every element x of G, the mapping Int(x): $y \mapsto xyx^{-1}$ of G into itself is an automorphism of G. The mapping Int: $x \mapsto \operatorname{Int}(x)$ of G into Aut(G) is a group homomorphism, whose kernel is the centre of G and whose image is a normal subgroup of Aut(G).*

If $x, y$ and $z$ are elements of G, then $(xyx^{-1})(xz x^{-1}) = xyz x^{-1}$ and hence Int(x) is an endomorphism of G. For $x$ and $y$ elements of G,

$$
\operatorname{Int}(x) \circ \operatorname{Int}(y) = \operatorname{Int}(xy):
$$

for all $z \in G$, $x(yzy^{-1})x^{-1} = (xy)z(xy)^{-1}$. On the other hand, $\operatorname{Int}(e)$ is the identity mapping of G. The mapping Int is therefore a monoid homomorphism from G to the monoid End(G) of endomorphisms of the group G. As the elements of G are invertible, the mapping Int takes its values in the set Aut(G) of invertible elements of End(G) (§ 2, no. 3). Now $xyx^{-1} = y$ if and only if $x$ and $y$ commute and hence $\operatorname{Int}(x)$ is the identity mapping of G if and only if $x$ is a central element. Finally, let $\alpha$ be an automorphism of G and let $x \in G$; then

$$
\operatorname{Int}(\alpha(x)) = \alpha \circ \operatorname{Int}(x) \circ \alpha^{-1}.
$$

For $y \in G$,

$$
\alpha(x) \cdot y \cdot \alpha(x)^{-1} = \alpha(x) \cdot \alpha(\alpha^{-1}(y)) \cdot \alpha(x)^{-1} = \alpha(x \cdot \alpha^{-1}(y) \cdot x^{-1}).
$$

Hence $\alpha \cdot \operatorname{Int}(G) \cdot \alpha^{-1} \subset \operatorname{Int}(G)$.

#### Definition 4 {#alg-i-s5-def-4 .statement}

*Let G be a group and $x \in G$. The automorphism $y \mapsto xyx^{-1}$ is called the inner automorphism of G defined by x and is denoted by $\operatorname{Int} x$.*

For $x, y \in G$, we also write $x^y = y^{-1}xy = (\operatorname{Int} y^{-1})(x)$.

A subgroup of G is normal if and only if it is stable under all inner automorphisms of G (§ 4, no. 4, Definition 5). A subgroup of G is called characteristic if it stable under all automorphisms of G. The centre of a group G is a characteristic subgroup (formula (2)).

The centre of a group G is not necessarily stable under all endomorphisms of G (Exercise 22). In particular, the centre of a group with operators is not necessarily a stable subgroup.

#### Proposition 4 {#alg-i-s5-prop-4 .statement}

Let G be a group, H a characteristic (resp. normal) subgroup of G and K a characteristic subgroup of H. Then K is a characteristic (resp. normal) subgroup of G.

The restriction to H of an automorphism (resp. inner automorphism) of G is an automorphism of H and therefore leaves K invariant.

Let G be a group, A $\subset$ G and $b \in G$. b is said to normalize A if $bAb^{-1} = A$; b is said to centralize A if, for all $a \in A$, $bab^{-1} = a$. Let A and B be subsets of G; B is said to normalize (resp. centralize) A if every element of B normalizes (resp. centralizes) A.

The set of $g \in G$ which normalize (resp. centralize) A is called the normalizer (resp. centralizer) of A (cf. § 1, no. 5, Definition 9); it is often denoted by $N_G(A)$ or simply $N(A)$ (resp. $C_G(A)$ or $C(A)$). It is a subgroup of G. When A is a subgroup of G, $N_G(A)$ may be characterized as the largest subgroup of G which contains A and in which A is normal.

#### Remark {#alg-i-s5-n3-rem-1 .statement}

(1) The normalizer (resp. centralizer) of A is the strict stabilizer (resp. fixer) of A when G operates on itself by inner automorphisms. In particular the centralizer is a normal subgroup of the normalizer.

(2) The set of elements $b \in G$ such that $bAb^{-1} \subset A$ is a submonoid of G. Even when A is a subgroup of G, this set is not necessarily a subgroup of G (Exercise 27).

### 4. ORBITS

#### Definition 5 {#alg-i-s5-def-5 .statement}

Let G be a group, E a G-set and $x \in G$. An element $y \in E$ is conjugate to x under the operation of G if there exists an element $\alpha \in G$ such that $y = \alpha x$. The set of conjugate elements of x is called the orbit of x in E.

The relation "y is conjugate to x" is an equivalence relation. For $x = ex$; if $y = \alpha x$, then $x = \alpha^{-1} y$; if $y = \alpha x$ and $z = \beta y$, then $z = \beta \alpha x$. The orbits are the equivalence classes under this relation.

A subset X of E is stable if and only if it is saturated with respect to the relation of conjugation.

The mapping $\alpha \mapsto \alpha x$ of G into E is sometimes called the orbital mapping defined by x. It is a G-morphism of G (with the operation of G on itself by left translation) into E. The image $G . x$ of G under this mapping is the orbit of x.

G is said to operate freely on E if, for all $x \in E$, the orbital mapping defined by x is injective or also if the mapping $(g, x) \mapsto (gx, x)$ of $G \times E$ into $E \times E$ is injective.

#### Example {#alg-i-s5-n4-exa-1 .statement}

(1) Let G be a group and consider the operation of G on itself by inner automorphisms. Two elements of G which are conjugate under this operation are called conjugate under inner automorphisms or simply conjugate. The orbits are called conjugacy classes. Similarly, two subsets H and H' of G are called conjugate if there exists an element $\alpha \in G$ such that $H' = \alpha . H . \alpha^{-1}$, that is if they are conjugate under the extension to $\mathcal{P}(G)$ of the operation of G on itself by inner automorphisms.

(2) *In the space $\mathbf{R}^n$, the orbit of a point x under the action of the orthogonal group $\mathbf{O}(n, \mathbf{R})$ is the Euclidean sphere of radius $\|x\|_*$.

The stabilizers of two conjugate elements of E are conjugate subgroups of G (no. 2, Proposition 2).

The quotient set of E under the relation of conjugation is the set of orbits of E; it is sometimes denoted by E/G or G\|E. (Sometimes the notation E/G is reserved for the case where E is a right G-set and the notation G\|E for the case where E is a left G-set.)

Let G be a group operating on a set E on the right. Let H be a normal subgroup of G. The group G operates on E/H on the right, the corresponding law of right action being $(xH, g) \mapsto xHg = xgH$; under this operation, H operates trivially, whence a right operation of G/H on E/H. Let $\phi$ be the canonical mapping of E/H onto E/G; the inverse images under $\phi$ of the points of E/G are the orbits of G (or of G/H) in E/H. Hence $\phi$ defines when passing to the quotient a bijection, called canonical, of $(E/H)/G = (E/H)/(G/H)$ onto E/G.

Let G (resp. H) be a group operating on a set E on the left (resp. right). Suppose that the actions of G and H on E commute, that is

$$
(g.x).h = g.(x.h) \quad \text{for } g \in G, x \in E \text{ and } h \in H.
$$

The action of H on E is also a left operation of the opposite group $H^0$ to H. It then follows from § 4, no. 9, Proposition 12 that the mapping which associates with the element $(g, h) \in G \times H^0$ the mapping $x \mapsto g . x . h$ of E into itself is a left operation of $G \times H^0$ on E. The orbit of an element $x \in E$ under this operation is the set $GxH$. The set of these orbits is denoted by $G\|E/H$. On the other hand, the operation of G (resp. H) is compatible with the relation of conjugation with respect to the operation of H (resp. G) and the set of orbits $G\|(E/H)$ (resp. $(G\|E)/H$) is identified with $G\|E/H$: in the diagram

$$
\begin{array}{ccc}
& & E \\
& \swarrow_{\alpha} & \searrow_{\beta} \\
G\|E & & E/H \\
& \downarrow_{\varepsilon} & \\
& & G\|E/H \\
& \searrow_{\delta} & \swarrow_{\gamma}
\end{array}
$$

(where $\alpha, \beta, \gamma, \delta, \varepsilon$ denote the canonical mappings of taking quotients), $\gamma \circ \alpha = \delta \circ \beta = \varepsilon$.

Let G be a group and H a subgroup of G. Consider the right operation of H on G by right translation (no. 1, Example 2). The set of orbits $G/H$ is the set of left cosets modulo H; note that G operates on $G/H$ on the left by the law $(g, xH) \mapsto gxH$ (cf. no. 5). Similarly, the set of right cosets modulo H is the set $H\backslash G$ of orbits of the left operation of H on G by left translation. If K is a subgroup of G containing H and $\Gamma$ is a left (resp. right) coset modulo H, then $\Gamma K$ (resp. $K\Gamma$) is a left (resp. right) coset modulo K. The mapping $\Gamma \mapsto \Gamma K$ (resp. $\Gamma \mapsto K\Gamma$) is called the canonical mapping of $G/H$ into $G/K$ (resp. of $H\backslash G$ into $K\backslash G$). It is surjective.

Let G be a group and H and K two subgroups of G. Let H operate on G on the left by left translation and K on the right by right translation; these two operations commute, which allows us to consider the set $H\backslash G/K$. The elements of $H\backslash G/K$ are called the double cosets of G modulo H and K. When $K = H$, we simply say double cosets modulo H. For the canonical mapping of $G/H$ onto $H\backslash G/H$ to be a bijection, it is necessary and sufficient that H be a normal subgroup of G.

### 5. HOMOGENEOUS SETS

#### Definition 6 {#alg-i-s5-def-6 .statement}

*Let G be a group. An operation of G on a set E is called transitive if there exists an element $x \in E$ whose orbit is E. A G-set E is called homogeneous if the operation of G on E is transitive.*

It is also said that G *operates transitively* on E; or that E is a *homogeneous set under* G. It amounts to the same to say that E *is non-empty* and that, for all elements $x$ and $y$ of E, there exists an element $\alpha \in G$ such that $\alpha.x = y$.

#### Example {#alg-i-s5-n5-exa-1 .statement}

If E is a G-set, each orbit of E, with the induced operation, is a homogeneous set under G.

Let G be a group and H a subgroup of G. Consider the set $G/H$ of left cosets modulo H. The group G operates on $G/H$ on the left by $(g, xH) \mapsto gxH$. Let N be the normalizer of H. The group N operates on $G/H$ on the right by $(xH, n) \mapsto xHn = xnH$. This operation induces on H the trivial operation and hence, on passing to the quotient, $N/H$ operates on $G/H$ on the right. Let $\phi : (N/H)^0 \to S_{G/H}$ be the homomorphism corresponding to this operation.

#### Proposition 5 {#alg-i-s5-prop-5 .statement}

*With the above notation, G/H is a homogeneous G-set. The mapping $\phi$ induces an isomorphism of $(N/H)^0$ onto the group of automorphisms of the G-set G/H.*

The orbit in $G/H$ of the element $e = H$ is $G/H$, whence the first assertion. We now prove the second. If $n \in N$ defines by right translation the identity mapping on $G/H$, then $e.n = e$, that is $H.n = H$, whence $n \in H$. Therefore

N/H operates faithfully on G/H on the right and $\phi$ is injective. The left operation of G and right operation of N/H on G/H commute and hence the operators of N/H define G-morphisms of G/H into itself, which are necessarily G-automorphisms since they are bijective. Therefore $\phi$ takes its values in the group $\Phi$ of G-automorphisms of G/H. We show that the image of $\phi$ is $\Phi$. Let $f \in \Phi$. By transporting the structure, the stabilizer of $f(\dot{e})$ in G is equal to the stabilizer of $\dot{e}$ and hence to H. Let $n \in G$ be such that $f(\dot{e}) = n\dot{e}$. The stabilizer of $n\dot{e}$ in G is $nHn^{-1}$ (no. 2, Proposition 2), whence $nHn^{-1} = H$ and $n \in N$. For every element $xH$ of G/H, $f(xH) = f(x.\dot{e}) = x.f(\dot{e}) = xnH = xHn$ and $f$ coincides with the mapping defined by $n$.

#### Remark {#alg-i-s5-n5-rem-1 .statement}

(1) Let G be a group, H a subgroup of G and $\phi : G \to \mathcal{S}_{G/H}$ the homomorphism corresponding to the operation of G on G/H. The kernel of $\phi$ is the intersection of the conjugates of H (no. 2, Proposition 2). It is also the largest normal subgroup contained in H (no. 3). In particular, G operates faithfully on G/H if and only if the intersection of the conjugates of H reduces to $\{e\}$.

(2) Let G be a group and H and K subgroups such that H is a normal subgroup of K. Then K/H operates on the G-set G/H on the right and the canonical mapping of G/H onto G/K defines on passing to the quotient a G-set isomorphism $(G/H)/(K/H) \to G/K$ (cf. no. 4).

#### Proposition 6 {#alg-i-s5-prop-6 .statement}

*Let G be a group, E a homogeneous G-set, $a \in E$, H the stabilizer of a and K a subgroup of G contained in H. There exists one and only one G-morphism f of G/K into E such that $f(e.K) = a$. If K = H, f is an isomorphism.*

If f is a solution, then $f(x.K) = x.a$ for all x in G, whence the uniqueness; we show the existence. The orbital mapping defined by a is compatible with the equivalence relation $y \in xK$ on G. For, if $y = xk, k \in K$, then
$$
y.a = xk.a = x.a.
$$
A mapping f is thus derived of G/K into H which satisfies $f(x.K) = x.a$ for all x in G. This mapping is a G-morphism and $f(K) = a$. This mapping is surjective for its image is a non-empty stable subset of E. Suppose now that K = H and let us show that f is injective. If $f(x.H) = f(y.H)$, then $x.a = y.a$, whence $x^{-1}y.a = a$ and $x^{-1}y \in H$, whence $x.H = y.H$.

#### Theorem 1 {#alg-i-s5-thm-1 .statement}

*Let G be a group.*
(a) *Every homogeneous G-set is isomorphic to a homogeneous G-set of the form G/H where H is a subgroup of G.*
(b) *Let H and H' be two subgroups of G. The G-sets G/H and G/H' are isomorphic if and only if H and H' are conjugate.*

As a homogeneous G-set is non-empty, assertion (a) follows from Proposition 6. We show (b). Let $f : G/H \to G/H'$ be a G-set isomorphism. The subgroup H is the stabilizer of H and hence, by transport of structure, the stabilizer of an element of $G/H'$. The subgroups $H$ and $H'$ are therefore conjugate (no. 2, Proposition 2). If $H' = \alpha H \alpha^{-1}$, $H'$ is the stabilizer of the element $\alpha . H$ of $G/H$ (no. 2, Proposition 2) and hence $G/H'$ is isomorphic to $G/H$ (Proposition 6).

#### Example {#alg-i-s5-n5-exa-2 .statement}

(1) Let $E$ be a non-empty set. The group $S_E$ operates transitively on $E$. If $x$ and $y$ are two elements of $E$, the mapping $\tau : E \to E$ such that $\tau(x) = y$, $\tau(y) = x$ and $\tau(z) = z$ for $z \neq x, y$, is a permutation of $E$. Let $a \in E$. The stabilizer of $a$ is identified with $S_F$, where $F = E - \{a\}$. The homogeneous $G$-set $E$ is thus isomorphic to $S_E / S_F$.

(2) Let $E$ be a set of $n$ elements and $(p_i)_{i \in I}$ a finite family of integers $> 0$ such that $\sum_i p_i = n$. Let $X$ be the set of partitions $(F_i)_{i \in I}$ of $E$ such that $\mathrm{Card}(F_i) = p_i$ for all $i$. The group $S_E$ operates transitively on $X$. The stabilizer $H$ of an element $(F_i)_{i \in I}$ of $X$ is canonically isomorphic to $\prod_{i \in I} S_{F_i}$ and is hence of order $\prod_{i \in I} p_i!$. Applying Theorem 1 and § 4, no. 4, Corollary to Proposition 4, a new proof is obtained of the fact that

$$
\mathrm{Card}(X) = \frac{n!}{\prod_{i \in I} p_i!}
$$

In particular, take $I = \{1, 2, \ldots, r\}$, $E = \{1, 2, \ldots, n\}$,

$$
F_i = \{p_1 + \cdots + p_{i-1} + 1, \ldots, p_1 + \cdots + p_i\}
$$

for $1 \leq i \leq r$. Let $S$ be the set of $\tau \in S_E$ such that $\tau|_{F_i}$ is increasing for $1 \leq i \leq r$. If $(G_1, \ldots, G_r) \in X$ there exists one and only one $\tau \in S$ which maps $(F_1, \ldots, F_r)$ to $(G_1, \ldots, G_r)$. In other words, each left coset of $S_E$ modulo $H$ meets $S$ in one and only one point.

(3) *Let $n$ be an integer $\geq 1$. The orthogonal group $O(n, \mathbf{R})$ operates transitively on the unit sphere $S_{n-1}$ in $\mathbf{R}^n$. The stabilizer of the point $(0, \ldots, 0, 1)$ is identified with the orthogonal group $O(n-1, \mathbf{R})$. The homogeneous $O(n, \mathbf{R})$-set $S_{n-1}$ is thus isomorphic to $O(n, \mathbf{R})/O(n-1, \mathbf{R})$.*

### 6. HOMOGENEOUS PRINCIPAL SETS

#### Definition 7 {#alg-i-s5-def-7 .statement}

*Let $G$ be a group. An operation of $G$ on a set $E$ is called simply transitive if there exists an element $x$ of $E$ such that the orbital mapping defined by $x$ is a bijection. A set $E$, together with a simply transitive left action of $G$ on $E$, is called a left homogeneous principal $G$-set (or left homogeneous principal set under $G$).*

It amounts to the same to say that $G$ operates freely and transitively on $E$, or also that there exists an element $x \in E$ such that the orbital mapping defined by $x$ is an isomorphism of the $G$-set $G$ (where $G$ operates by left translation) onto $E$; or also that the two following conditions are satisfied:

(i) $E$ is non-empty.
(ii) for all elements $x$ and $y$ of $E$, there exists one and only one element $\alpha \in G$ such that $\alpha x = y$.

Condition (ii) is also equivalent to the following condition:

(iii) the mapping $(\alpha, x) \mapsto (\alpha x, x)$ is a bijection of $G \times E$ onto $E \times E$.

We leave to the reader the task of defining right homogeneous principal G-sets.

#### Example {#alg-i-s5-n6-exa-1 .statement}

(1) Let G operate on itself by left (resp. right) translation. Thus a left (resp. right) homogeneous principal G-set structure is defined on G, which is sometimes denoted by $G_s$ (resp. $G_d$).

(2) Let E be a homogeneous set under a *commutative* group G. If G operates faithfully on E, the latter is a homogeneous principal G-set.

(3) Let E and F be two isomorphic sets with structures of the same species and let Isom(E, F) be the set of isomorphisms of E onto F (with the given structures). The group Aut(E) of automorphisms of E (with the given structure) operates on Isom(E, F) on the right by the law $(\sigma, f) \mapsto f \circ \sigma$ and Isom(E, F) is a right homogeneous principal Aut(E)-set. Similarly, the group Aut(F) operates on Isom(E, F) on the left by the law $(\sigma, f) \mapsto \sigma \circ f$ and Isom(E, F) is a left homogeneous principal Aut(F)-set.

(4) *A homogeneous principal set under the additive group of a vector space is called an *affine space* (cf. II, § 9, no. 1).*

The group of automorphisms of the homogeneous principal G-set $G_s$ (Example 1) is the group of right translations of G which is identified with $G^0$ (no. 5, Proposition 5). Let E be a homogeneous principal G-set and $a$ an element of E. The orbital mapping $\omega_a$ defined by $a$ is an isomorphism of the G-set $G_s$ onto E. By transporting the structure an isomorphism $\psi_a$ is derived of $G^0$ onto Aut(E). It should be noted that $\psi_a$ *in general depends on a*; more precisely, for $\alpha \in G$,

$$
\psi_{\alpha a} = \psi_a \circ \operatorname{Int}_{G^0}(\alpha) = \psi_a \circ \operatorname{Int}(\alpha^{-1}).
$$

For, writing $\delta_a$ for the translation $x \mapsto x \alpha$ on G,

$$
\omega_{\alpha a} = \phi \omega_a \circ \delta_\alpha
$$
and
$$
\psi_a(x) = \omega_a \circ \delta_x \circ \omega_a^{-1}, \quad x \in G,
$$
whence
$$
\psi_{\alpha a}(x) = \omega_a \circ \delta_\alpha \circ \delta_x \circ \delta_\alpha^{-1} \circ \omega_a^{-1} = \omega_a \circ \delta_{\alpha^{-1} x \alpha} \circ \omega_a^{-1} = \psi_a(\alpha^{-1} x \alpha).
$$

### 7. PERMUTATION GROUPS OF A FINITE SET

If E is a finite set with $n$ elements, the symmetric group $\mathfrak{S}_E$ (§ 4, no. 1) is a finite group of order $n!$. When E is the interval $\{1, n\}$ of the set $\mathbf{N}$ of natural numbers, the corresponding symmetric group is denoted by $\mathfrak{S}_n$; the symmetric group of any set with $n$ elements is isomorphic to $\mathfrak{S}_n$.

#### Definition 8 {#alg-i-s5-def-8 .statement}

Let E be a finite set, $\zeta \in \mathfrak{S}_E$ a permutation of E and $\bar{\zeta}$ the subgroup of $\mathfrak{S}_E$ generated by $\zeta$. $\zeta$ is called a cycle if, under the operation of $\bar{\zeta}$ on E, there exists one and only one orbit which is not reduced to a single element. This orbit is called the support of $\zeta$.

Let $\zeta$ be a cycle. The support $\operatorname{supp}(\zeta)$ of $\zeta$ is the set of $x \in E$ such that $\zeta(x) \neq x$.

The order of a cycle $\zeta$ is equal to the cardinal of its support. The subgroup $\bar{\zeta}$ generated by $\zeta$ operates transitively and faithfully on $\operatorname{supp}(\zeta)$. As $\zeta$ is commutative, $\operatorname{supp}(\zeta)$ is a principal set under $\bar{\zeta}$ (no. 6, Example 2) and hence $\operatorname{Card}(\operatorname{supp}(\zeta)) = \operatorname{Card}(\bar{\zeta})$.

#### Lemma 1 {#alg-i-s5-lem-1 .statement}

Let $(\zeta_i)_{i \in I}$ be a family of cycles whose supports are pairwise disjoint. Then the $\zeta_i$ are pairwise permutable. Let $\sigma = \prod_{i \in I} \zeta_i$ and $\bar{\sigma}$ be the subgroup generated by $\sigma$. Then $\sigma(x) = \zeta_i(x)$ for $x \in S_i, i \in I$, and $\sigma(x) = x$ for $x \notin \bigcup_{i \in I} S_i$. The mapping $i \mapsto S_i$ is a bijection of I onto the set of $\bar{\sigma}$-orbits not consisting of a single element.

Let $\zeta$ and $\zeta'$ be two cycles whose supports are disjoint. If
$$
x \notin \operatorname{supp}(\zeta) \cup \operatorname{supp}(\zeta'),
$$
then $\zeta \zeta'(x) = \zeta' \zeta(x) = x$. If $x$ belongs to the support of $\zeta$, then $\zeta'(x) = x$, and $\zeta(x)$ belongs to the support of $\zeta$, whence $\zeta \zeta'(x) = \zeta' \zeta(x) = \zeta(x)$. Similarly when $x$ belongs to the support of $\zeta'$, then $\zeta' \zeta(x) = \zeta \zeta'(x) = \zeta'(x)$. Hence $\zeta \zeta' = \zeta' \zeta$. Therefore the $\zeta_i$ are pairwise permutable and, for $i \in I$ and $x \in S_i$, $\sigma(x) = \zeta_i(x) \in S_i$. The mappings $\sigma$ and $\zeta_i$ coincide on $S_i$, hence $S_i$ is stable under $\sigma$ and the subgroup of $\mathfrak{S}_{S_i}$ generated by the restriction of $\sigma$ to $S_i$ operates transitively on $S_i$; therefore $S_i$ is a $\bar{\sigma}$-orbit. As the $S_i$ are non-empty and are pairwise disjoint, the mapping $i \mapsto S_i$ is injective. As $\bigcup_i S_i$ is the set of $x$ such that $\sigma(x) \neq x$, every $\bar{\sigma}$-orbit not consisting of a single element is one of the $S_i$.

#### Proposition 7 {#alg-i-s5-prop-7 .statement}

Let E be a finite set and $\sigma$ a permutation of E. There exists one and only one finite set C of cycles satisfying the two following conditions:

(a) the supports of the elements of C are pairwise disjoints;

(b) $\sigma = \prod_{\zeta \in C} \zeta$ (the elements of C being pairwise permutable by Lemma 1).

Let $\bar{\sigma}$ be the subgroup generated by $\sigma$ and let S be the set of $\bar{\sigma}$-orbits not consisting of a single element. For $s \in S$, write $\zeta_s(x) = \sigma(x)$ if $x \in s$ and $\zeta_s(x) = x$ if $x \notin s$. For all $s \in S$, $\zeta_s$ is a cycle whose support is $s$ and $\sigma = \prod_{s \in S} \zeta_s$, as is seen by applying the two sides to any element of E. The uniqueness of C follows from Lemma 1.

#### Definition 9 {#alg-i-s5-def-9 .statement}

*A cycle of order 2 is called a transposition.*

Let $x$ and $y$ be two *distinct* elements of E. Let $\tau_{x,y}$ denote the unique transposition with support $\{x, y\}$.

For every permutation $\sigma$ of E the permutation $\sigma \cdot \tau_{x,y} \cdot \sigma^{-1}$ is a transposition whose support is $\{\sigma(x), \sigma(y)\}$. Hence:

(4)
$$
\sigma \cdot \tau_{x,y} \cdot \sigma^{-1} = \tau_{\sigma(x), \sigma(y)}.
$$

Transpositions thus form a conjugacy class in the group $\mathfrak{S}_E$.

#### Proposition 8 {#alg-i-s5-prop-8 .statement}

*Let E be a finite set. The group $\mathfrak{S}_E$ is generated by the transpositions.*

For every permutation $\sigma$ let $F_\sigma$ be the set of $x \in E$ such that $\sigma(x) = x$. We show by descending induction on $p$ that every permutation $\sigma$ such that $\mathrm{Card}(F_\sigma) = p$ is a product of transpositions. If $p \geq \mathrm{Card}(E)$, the permutation $\sigma$ is the identity mapping of E; it is the product of the empty family of transpositions. If $p < \mathrm{Card}(E)$, suppose that the property is proved for every permutation $\sigma'$ such that $\mathrm{Card}(F_{\sigma'}) > p$. Now $E - F_\sigma \neq \varnothing$; let $x \in E - F_\sigma$ and $y \in \sigma(x)$. Then $y \neq x$ and $y \in E - F_\sigma$. Let $\sigma' = \tau_{x,y} \cdot \sigma$. The set $F_{\sigma'}$ contains $F_\sigma$ and $x$ and hence $\mathrm{Card}(F_{\sigma'}) > \mathrm{Card}(F_\sigma) = p$. By the induction hypothesis $\sigma'$ is a product of transpositions and hence $\sigma = \tau_{x,y} \cdot \sigma'$ is a product of transpositions.

#### Proposition 9 {#alg-i-s5-prop-9 .statement}

*Let n be an integer $\geq 0$. The group $\mathfrak{S}_n$ is generated by the transpositions* $(\tau_{i, i+1})_{1 \leq i \leq n-1}$.

By virtue of Proposition 8, it suffices to show that every transposition $\tau_{p,q}$, $1 \leq p < q \leq n$, belongs to the subgroup H generated by the $\tau_{i, i+1}$, $1 \leq i \leq n-1$. We show this by induction on $q-p$. For $q-p = 1$, it is obvious. If $q-p > 1$, then (formula (4)) $\tau_{p,q} = \tau_{q-1,q} \tau_{p,q-1} \tau_{q-1,q}$. By the induction hypothesis $\tau_{p,q-1} \in H$ and therefore $\tau_{p,q} \in H$.

If $\sigma \in \mathfrak{S}_n$, every ordered pair $(i, j)$ of elements of $\{1, n\}$ such that $i < j$ and $\sigma(i) > \sigma(j)$ is called an *inversion* of $\sigma$. Let $\nu(\sigma)$ denote the number of inversions of $\sigma$.

Let P be the additive group of mappings from $\mathbf{Z}^n$ to $\mathbf{Z}$. For $f \in P$ and $\sigma \in \mathfrak{S}_n$, let $\sigma f$ be the element of P defined by

(5)
$$
\sigma f(z_1, \ldots, z_n) = f(z_{\sigma(1)}, \ldots, z_{\sigma(n)}).
$$

The action of $\mathfrak{S}_n$ on P thus defined is an operation; for all $\sigma, \tau \in \mathfrak{S}_n$ and $f \in P$, $\sigma f = f$ and
$$
\begin{align*}
(\tau(\sigma f))(z_1, \ldots, z_n) &= \sigma f(z_{\tau(1)}, \ldots, z_{\tau(n)}) = f(z_{\tau \sigma(1)}, \ldots, z_{\tau \sigma(n)}) \\
&= ((\tau \sigma) f)(z_1, \ldots, z_n).
\end{align*}
$$
Formula (5) shows that $\sigma(-f) = -\sigma f$ for $\sigma \in \mathfrak{S}_n$ and $f \in P$.

Let $p$ be the element of P defined by

$$
p(z_1, \ldots, z_n) = \prod_{i < j} (z_j - z_i).
$$

#### Lemma 2 {#alg-i-s5-lem-2 .statement}

$p \neq 0$ and $\sigma p = (-1)^{\nu(\sigma)}$ for $\sigma \in \mathfrak{S}_n$.

$p(1, 2, \ldots, n) = \prod_{i < j} (j - i) \neq 0$ and hence $p \neq 0$. On the other hand, if $\sigma \in \mathfrak{S}_n$, then

$$
\sigma p(z_1, \ldots, z_n) = p(z_{\sigma(1)}, \ldots, z_{\sigma(n)}) = \prod_{i < j} (z_{\sigma(j)} - z_{\sigma(i)}).
$$

Let C be the set of ordered pairs $(i, j)$ such that $1 \leq i \leq n,\ 1 \leq j \leq n,\ i < j$. A permutation $\theta$ is defined on C by setting $\theta(i, j) = (\sigma(i), \sigma(j))$ if $(i, j)$ is not an inversion, $\theta(i, j) = (\sigma(j), \sigma(i))$ if $(i, j)$ is an inversion. This implies $\sigma p = (-1)^{\nu(\sigma)} p$.

#### Theorem 2 {#alg-i-s5-thm-2 .statement}

*Let E be a finite set. There exists one and only one homomorphism $\varepsilon$ from $\mathfrak{S}_n$ to the multiplicative group $\{-1, +1\}$ such that $\varepsilon(\tau) = -1$ for every transposition $\tau$.*

The uniqueness follows from Proposition 8. We show the existence. By transporting the structure, it may be assumed that $E = \{1, n\}$. Using the above notation, let $\varepsilon(\sigma) = (-1)^{\nu(\sigma)}$. Then (Lemma 2)

$$
\sigma(\sigma' p) = \sigma(\varepsilon(\sigma') p) = \varepsilon(\sigma') (\sigma p) = \varepsilon(\sigma') \varepsilon(\sigma) p.
$$

On the other hand,

$$
\sigma(\sigma' p) = (\sigma \sigma') p = \varepsilon(\sigma \sigma') p.
$$

As $p \neq -p$, it follows that $\varepsilon(\sigma \sigma') = \varepsilon(\sigma) \varepsilon(\sigma')$ and thus $\varepsilon$ is a homomorphism. We now show that, for every transposition $\tau$, $\varepsilon(\tau) = -1$. $\nu(\tau_{n-1, n}) = 1$, whence $\varepsilon(\tau_{n-1, n}) = -1$. As every transposition $\tau$ is conjugate to $\tau_{n-1, n}$ and the group $\{-1, +1\}$ is commutative, $\varepsilon(\tau) = \varepsilon(\tau_{n-1, n}) = -1$.

#### Definition 10 {#alg-i-s5-def-10 .statement}

*In the notation of Theorem 2, the number $\varepsilon(\sigma)$ (also denoted $\varepsilon_\sigma$) is called the signature of the permutation $\sigma$. The kernel of the homomorphism $\varepsilon$ is called the alternating group of E.*

$\sigma$ is called *even* (resp. *odd*) if $\varepsilon(\sigma) = 1$ (resp. $\varepsilon(\sigma) = -1$). The alternating group of E is denoted by $\mathfrak{A}_E$. It is a normal subgroup of $\mathfrak{S}_E$. When $E = \{1, n\}$, it is simply denoted by $\mathfrak{A}_n$. When the cardinal $n$ of E is $\geq 2$, it is a subgroup of index 2 and hence of order $n! / 2$. It can be shown that, for $n = 3$ or $n \geq 5$, the group $\mathfrak{A}_n$ is a simple group (*cf. Exercise 16*).

#### Example {#alg-i-s5-n7-exa-1 .statement}

If $\sigma$ is a cycle of order $d$, then
$$
\varepsilon(\sigma) = (-1)^{d-1}.
$$
The number of inversions of the permutation
$$
(1, 2, 3, \ldots, d) \mapsto (d, 1, 2, \ldots, d-1)
$$
is equal to $d-1$.

### Exercises {#alg-i-s5-exercises}

See the [exercises for § 5](exercises/s5/).
