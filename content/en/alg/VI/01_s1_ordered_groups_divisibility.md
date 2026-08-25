---
book: alg
book_title: Algebra
chapter: VI
chapter_title: ORDERED GROUPS AND FIELDS
section: 1
section_title: Ordered groups. Divisibility
lang: en
source: alg-iv-vii
source_edition: 2003, Springer
pdf_pages: 0312-0330, 0341-0348
extraction: ocr
subsections:
    - "no": 1
      title: Definition of ordered monoids and groups
      page: 0
      pdf_page: 312
    - "no": 2
      title: Pre-ordered monoids and groups
      page: 3
      pdf_page: 314
    - "no": 3
      title: Positive elements
      page: 3
      pdf_page: 314
    - "no": 4
      title: Filtered groups
      page: 4
      pdf_page: 315
    - "no": 5
      title: Divisibility relations in a field
      page: 5
      pdf_page: 316
    - "no": 6
      title: Elementary operations on ordered groups
      page: 7
      pdf_page: 318
    - "no": 7
      title: Increasing homomorphisms of ordered groups
      page: 7
      pdf_page: 318
    - "no": 8
      title: Suprema and infima in an ordered group
      page: 8
      pdf_page: 319
    - "no": 9
      title: Lattice ordered groups
      page: 10
      pdf_page: 321
    - "no": 10
      title: The decomposition theorem
      page: 11
      pdf_page: 322
    - "no": 11
      title: Positive and negative parts
      page: 12
      pdf_page: 323
    - "no": 12
      title: Coprime elements
      page: 13
      pdf_page: 324
    - "no": 13
      title: Irreducible elements
      page: 17
      pdf_page: 328
statements: 52
exercises: 34
content_sha256: 7807160be0ee4703e84d6ac63919ca0a7e810af32944eb915f0916f77170d87d
---

## § 1. ORDERED GROUPS. DIVISIBILITY

The notions and results presented in this section concern the study of order relations in commutative monoids (I, p. 12, Def. 2), the most important case being that of abelian groups. Unless explicitly stated otherwise, we will use additive notation for the composition law in all groups and monoids under study. On the other hand, as we go along we will present certain important algebraic applications of the theory of ordered groups and monoids, and we will accordingly translate certain of our results into the multiplicative notation which is appropriate for these applications.

### 1. Definition of ordered monoids and groups

#### Definition 1 {#alg-vi-s1-def-1 .statement}

— A commutative monoid structure (written additively) and an ordering (written $ \leq $) on a set $ M $ are said to be compatible if they satisfy the following axiom:

(OM) For each $ z \in M $, the relation $ x \leq y $ implies $ x + z \leq y + z $.

A set $ M $ equipped with a commutative monoid structure and an ordering which are compatible is called an ordered monoid; if its commutative monoid structure is a group structure, then it is called an ordered group.

In an analogous fashion, we can define the notion of a noncommutative ordered monoid (VI, p. 30, Ex. 1).

If an ordering is compatible with a given monoid structure, then so is the opposite ordering.

#### Example 1 {#alg-vi-s1-n1-exa-1 .statement}

The additive group of the rational integers, and that of the rational numbers, are ordered groups under the ordering defined in I, pp. 21 and 117. *The same is true for the additive group of the real numbers (Gen. Top., IV, p 3). \*

#### Example 2 {#alg-vi-s1-n1-exa-2 .statement}

*The additive group of finite numerical functions defined on a set $ E $ is an ordered group under the ordering « $ f(x) \leq g(x) $ for all $ x \in E $ », written $ f \leq g $. This relation says that the graph of the function $ f $ lies below that of the function $ g $. The reader may find it convenient to think in terms of this graphical interpretation occasionally. \*

According to general definitions (Set Theory, IV, p. 264), a bijective map $ f $ from an ordered monoid M onto an ordered monoid M' is called an *isomorphism* of M onto M' if the structure of M' is obtained from that of M by transporting it along $ f $. This is equivalent to saying that $ f $ is a mapping *onto* M' such that

$$
f(x + y) = f(x) + f(y)
$$

(that is to say a homomorphism of the monoid M onto the monoid M'), and that the relations $ x \leq y $ and $ f(x) \leq f(y) $ are equivalent (whence in particular $ f(x) = f(y) $ implies $ x = y $, that is $ f $ is injective).

#### Proposition 1 (« addition of inequalities ») {#alg-vi-s1-prop-1 .statement}

— *In an ordered monoid M*, let $ (x_i) $ and $ (y_i) $ ($ 1 \leq i \leq n $) be two sequences of n elements such that $ x_i \leq y_i $ for all $ i $; then one has

$$
x_1 + \cdots + x_n \leq y_1 + \cdots + y_n
$$

*If moreover all the elements $ x_i, y_i $ are cancellable (I, p. 15, Def. 5) (in particular if M is a group), and if $ x_i < y_i $ for some $ i $, then*

$$
x_1 + \cdots + x_n < y_1 + \cdots + y_n .
$$

The general case reduces by induction to the case $ n = 2 $, using the fact that a sum of cancellable elements is cancellable for the second assertion (I, p. 15, Prop. 2). The first assertion follows from the relations

$$
x_1 + x_2 \leq x_1 + y_2 \quad \text{and} \quad x_1 + y_2 \leq y_1 + y_2 ,
$$

which are consequences of the hypotheses and of (OM). This being the case, the relation

$$
x_1 + x_2 = y_1 + y_2
$$

would imply

$$
x_1 + x_2 = x_1 + y_2 = y_1 + y_2 ,
$$

whence $ x_2 = y_2 $ and $ x_1 = y_1 $ if $ x $, and $ y_2 $ are cancellable, which proves the second assertion.

#### Proposition 2 {#alg-vi-s1-prop-2 .statement}

*In an ordered group G* the relations $ x \leq y $ *and* $ x + z \leq y + z $ *are equivalent*.

Indeed one can obtain each from the other by adding $ z $ or $ (-z) $ to both sides.

This fact can be expressed by saying that, in an ordered group G, the ordering is *translation-invariant*. In other words a translation is an *automorphism* of the *ordering* of an ordered group.

#### Corollary {#alg-vi-s1-n1-cor-1 .statement}

— In an ordered group $ G $, the relations $ x \leq y $, $ 0 \leq y - x $, $ x - y \leq 0 $ and $ -y \leq -x $ are equivalent.

In fact, we apply Prop. 2, successively taking $ z = -x $, $ z = -y $ and $ z = -(x + y) $.

In particular we deduce from this corollary that if $ G $ is an ordered group, the map $ x \mapsto -x $ from $ G $ to itself takes the ordering of $ G $ to the opposite ordering.

### 2. Pre-ordered monoids and groups

Recall that if a relation $ x \leq y $ between elements of a set $ E $ is reflexive and transitive, it is called a pre-order relation (Set Theory, III, p. 133). The relation « $ x \leq y $ and $ y \leq x $ » is an equivalence relation $ S $ on $ E $, compatible with the relation $ x \leq y $; on passing to the quotient, the relation $ \leq $ induces an order relation on $ E/S $, called the order relation associated to $ \leq $.

#### Definition 2 {#alg-vi-s1-def-2 .statement}

— A pre-order relation (written $ \leq $) and a commutative monoid structure (written additively) on a set $ M $ are said to be compatible if they satisfy the following axiom:

(POM) For each $ z \in M $, the relation $ x \leq y $ implies $ x + z \leq y + z $.

A set $ M $ equipped with a commutative monoid structure and a pre-order relation which are compatible is called a pre-ordered monoid.

Let $ M $ be a pre-ordered monoid, and $ S $ the equivalence relation « $ x \leq y $ and $ y \leq x $ ». By virtue of (POM) the relation $ x \equiv x' \pmod{S} $ implies $ x + y \leq x' + y $ and $ x' + y \leq x + y $ for all $ y \in M $, that is $ x + y \equiv x' + y \pmod{S} $. In other words the equivalence relation $ S $ is compatible with addition in $ M $ (I, p. 11). Thus the quotient by $ S $ of the addition law on $ M $, together with the ordering associated to $ \leq $, gives $ M/S $ the structure of an ordered monoid. In the case where $ M $ is a pre-ordered group, the group $ M/S $ is the quotient of $ M $ by the subgroup consisting of all elements $ x $ such that $ x \leq 0 $ and $ 0 \leq x $.

### 3. Positive elements

Let $ G $ be a pre-ordered group with pre-order relation $ \leq $; if $ 0 \leq x $ and $ 0 \leq y $ then we deduce that $ y \leq x + y $ by (POM), and so $ 0 \leq x + y $ by transitivity; this says that the set $ G_+ $ of elements $ x \in G $ such that $ 0 \leq x $ is closed under addition; moreover, the relation $ x \leq y $ is equivalent to $ 0 \leq y - x $, that is to $ y - x \in G_+ $. Conversely:

#### Proposition 3 {#alg-vi-s1-prop-3 .statement}

— If $ P $ is a subset of an abelian group $ G $, containing $ 0 $ and such that $ P + P \subset P $, then the relation $ y - x \in P $ is a pre-order relation compatible with the group structure of $ G $. For this relation to make $ G $ an ordered group it is necessary and sufficient to have $ P \cap (-P) = \{0\} $; for $ G $ to be a totally ordered group under this ordering it is necessary and sufficient to have in addition $ P \cup (-P) = G $.

It is immediate that the relation $ y - x \in P $ is reflexive and transitive, and (if it is written $ x \leq y $) satisfies the axiom *POM*. To prove the second assertion it is enough to remark that $ P \cap (-P) $ is the subgroup $ G' $ consisting of elements $ x $ such that $ 0 \leq x $ and $ x \leq 0 $. Finally, to say that $ G $ is totally ordered means that, for each pair of elements $ x, y $ of $ G $, at least one of the elements $ x - y, y - x $ belongs to $ P $, which completes the proof.

#### Definition 3 {#alg-vi-s1-def-3 .statement}

*In an ordered group $ G $, any element $ x $ such that $ 0 \leq x $ (resp. $ x \leq 0 $) is called a positive (resp. negative) element.*

Note that $ 0 $ is the only element which is *both positive and negative* ; any element $ x $ such that $ 0 < x $ (resp. $ x < 0 $) is called *strictly positive* (resp. *strictly negative*).

#### Example {#alg-vi-s1-n3-exa-1 .statement}

— In the additive group $ \mathbf{Z} \times \mathbf{Z} $, let $ P $ be the set of elements $ (x, y) $ satisfying two inequalities $ ax + by \geq 0 $ and $ cx + dy \geq 0 $, where $ a, b, c, d $ are integers (* or real numbers *) such that $ ad - bc \neq 0 $; the « cone » $ P $ satisfies the first two conditions of Prop. 3. In this way various orderings compatible with the group structure of $ \mathbf{Z} \times \mathbf{Z} $ can be defined ; the group is not totally ordered under any of these orderings.

#### Remark {#alg-vi-s1-n3-rem-1 .statement}

— By virtue of the condition $ P + P \subset P $, the relation $ x \geq 0 $ in an ordered group implies that $ nx \geq 0 $ for every natural number $ n $. If in addition the positive element $ x $ of $ G $ has finite order $ n $, then $ -x = (n-1)x $ is positive ; since

$$
P \cap (-P) = \{0\},
$$

this implies that $ x = 0 $. In particular, if every element of $ G $ has finite order, then $ P = \{0\} $; the relation $ x \leq y $ is then equivalent to $ x = y $ (the *discrete* ordering).

### 4. Filtered groups

Recall (*Set Theory*, III, p. 145) that an ordered set $ G $ is *right* (resp. *left*) *filtered*\footnote{1} if for each pair $ (x, y) $ of elements of $ G $ there exists $ z \in G $ such that $ x \leq z $ and $ y \leq z $ (resp. $ z \leq x $ and $ z \leq y $). Every right filtered ordered group $ G $ is also left filtered and conversely : indeed, since there exists $ z \in G $ such that $ -x \leq z $ and $ -y \leq z $, we have $ -z \leq x $ and $ -z \leq y $ (VI, p. 3, Cor.). We will therefore speak simply of filtered groups.

#### Proposition 4 {#alg-vi-s1-prop-4 .statement}

*For an ordered group $ G $ to be filtered it is necessary and sufficient that it be generated by its positive elements, that is that every element be the difference of two positive elements.*

Indeed if $ G $ is filtered, then for each $ x \in G $ there exists a positive element $ z $ such that $ x \leq z $, and $ x $ is the difference of the two positive elements $ z $ and $ z - x $. Conversely, if $ x = u - v $ and $ y = w - t $ with $ u, v, w, t $ positive, then the element $ u + w $ is greater than $ x $ and greater than $ y $.

1 The terminology used in *loc. cit.* is *directed*.

#### Proposition 5 {#alg-vi-s1-prop-5 .statement}

— *If* $(x_i)$ *is a finite family of elements of a filtered group G, then there exists* $z \in G$ *such that* $x_i + z$ *is positive for each i.*

*If* $x_i = u_i - v_i$, *with* $u_i$ *and* $v_i$ *positive, it is enough to take* $z$ *to be the sum of the family* $(v_i)$.

### 5. Divisibility relations in a field

Here we will define certain ordered groups which play an important part in algebra. The notation usually used for these groups is multiplicative; the application of results previously obtained in additive notation to these groups thus presupposes the translation to multiplicative notation — which should present no difficulty to the reader. *Throughout this section, the letter A will denote an integral domain and K its field of fractions* (*l*, p. 116).

In the multiplicative group $\mathbf{K}^*$ of nonzero elements of $\mathbf{K}$, the set P of nonzero elements of A is closed under multiplication, since A is a ring. Hence it defines a pre-order relation on $\mathbf{K}^*$ by $x^{-1}y \in P$, that is « there exists $z \in P$ such that $y = zx$ », which makes $\mathbf{K}^*$ *apre-ordered group* (written multiplicatively) (*VI*, p. 3, Prop. 3). Extending the terminology relating to elements of A (I, p. 97) to $\mathbf{K}^*$, the relation $x^{-1}y \in P$ can also be expressed as : *x divides y*, or x is a *divisor of y*, or y is a *multiple of x* (relative to the ring A); and we will call the relation $x^{-1}y \in P$ the *divisibility relation* in $\mathbf{K}^*$ relative to the ring A. The relation « x 'divides y » is denoted $x \mid y$, and its negation $x \nmid y$. The elements of P are none other than the *multiples of 1*.

#### Remark 1 {#alg-vi-s1-n5-rem-1 .statement}

The divisibility relation in $\mathbf{K}^*$ depends in an essential way on the particular ring A. If $A = K$ we obtain the « trivial » relation, under which $x \mid y$ for every pair $(x, y)$ of elements of $\mathbf{K}^*$. Let p and q be prime numbers; the rational numbers r/s whose denominators are not multiples of $p$ (resp. q) form a subring $\mathbf{Z}_{(p)}$ (resp. $\mathbf{Z}_{(q)}$) of $\mathbf{Q}$; the divisibility relations in $\mathbf{Q}^*$ relative to these two rings are distinct if $p \neq q$, the number $p/q$ being a multiple of 1 under one relation but not under the other.

#### Remark 2 {#alg-vi-s1-n5-rem-2 .statement}

We will sometimes extend the definition of the relation $x \mid y$ to pairs of elements of $\mathbf{K}$ (rather than only $\mathbf{K}^*$), this relation being taken to mean « there exists $z \in A$ such that $y = zx$ »; hence we will have $x \mid 0$ for all $x \in K$. This allows us to state the following results without restrictions : if $x \mid y$ and $x \mid z$ then $x \mid (y - z)$; if $x \mid y$ and $x \nmid z$ then $x \nmid (y - z)$. In the same way we can extend all the corresponding terminology.

To obtain an *order relation* (No. 2) from the divisibility relation we have to pass to the quotient group of $\mathbf{K}^*$ by the subgroup $\mathbf{A}^*$ of elements $x \in \mathbf{K}^*$ such that $x \mid 1$ and $1 \mid x$; these are the elements of P which are *divisors of 1*, that is to say the *invertible* elements of $A$; by abuse of language they are often called the units of the ring A. The quotient group $\mathbf{K}^*/\mathbf{A}^*$ is then an ordered group. Two elements $x$ and $y$ of $\mathbf{K}^*$ which belong to the same coset of $\mathbf{A}^*$ are said to be *associate*; this means that $x \mid y$ and $y \mid x$. If on the other hand x divides y without y dividing x, we say that x strictly divides y, or that x is a strict divisor of y, or that y is a strict multiple of x.

Note that $ K^*/A^* $ is a *filtered* group, since K is the field of fractions of A (VI, p. 4, Prop. 4).

To say that two elements x and y of $ K^* $ are associate amounts to saying that they have *the* same multiples in K, by virtue of the transitivity of the divisibility relation. For all $ x \in K $, we will denote by $ Ax $ the set of all elements zx with $ z \in A $; the set $ Ax $ is a submodule of K regarded as an A-module. Extending the terminology relating to the case where $ x \in A $, we will call it a principal fractional ideal of the field K relative to the ring A. In contrast the ideals of the ring A are said to be integral.

Note that if $ A \neq K $ then a principal fractional ideal $ \neq \{0\} $ is not an ideal of K considered as a ring.

The principal fractional ideal $ Ax $ is also denoted (x). We will write $ x \equiv 0 $ (mody) for $ x \in Ay $ and $ x \equiv x' $ (mody) for $ x - x' \in Ay $; if $ x \equiv x' $ (mody) then $ zx \equiv zx' $ (mod $ zy $) for any $ z \in K $.

Note that $ x \equiv x' $ (mod y) does not imply $ zx \equiv zx' $ (mod y) unless $ z \in A $. Thus in $ \mathbf{Q} $, relative to $ \mathbf{Z} $, we have $ 4 \equiv 2 $ (mod 2) but not $ 2 \equiv 1 $ (mod 2).

The relation $ x | y $ is obviously equivalent to $ (x) \supset (y) $. The mapping $ x \mapsto (x) $ from $ K^* $ onto the set $ \mathcal{P}^* $ of principal fractional ideals $ \neq (0) $ of K thus defines, on passing to the quotient, a bijective mapping from $ K^*/A^* $ onto $ \mathcal{P}^* $; translating the group structure of $ K^*/A^* $ to $ \mathcal{P}^* $ by means of this mapping, we are led to define the product of two principal fractional ideals (x) and (y) to be the ideal (xy ), which depends only on (x) and (y). Equipped with this law and the order relation $ (x) \supset (y) $, the set $ \mathcal{P}^* $ is an ordered group, isomorphic to $ K^*/A^* $. By convention we will identify $ \mathcal{P}^* $ with $ K^*/A^* $ via the above map.

Note that the relation « x divides y » which, in the case of positive integers, implies that x is smaller than y, corresponds to the inclusion $ (x) \supset (y) $, in which the ideal (x) is « greater » than the ideal (y). We can keep this « order reversal » in mind by noting that for example 7 has a more multiples » than 91.

If we extend the relation $ x | y $ to all elements of K, this relation is still equivalent to $ (x) \supset (y) $ in the set $ \mathcal{P} $ of all principal fractional ideals of K (in which $ (0) $ is the smallest element under the relation of inclusion).

As in the previous sections, we will generally be using additive notation in the sequel. However, terminology relating to divisibility will be introduced following the corresponding additive terminology, in paragraphs preceded by the sign (DIV) (in which it is understood that the notation used is that of the present section). In order to make the reader's task easier, certain results will be translated into the language of divisibility, the translation of Prop. 7, for example, being denoted « PROPOSITION 7 (DIV) ».

### 6. Elementary operations on ordered groups

Let H be a subgroup of an ordered group G; it is clear that the restriction to H of the ordering of G is compatible with the group structure of H; we will always take H to be ordered in this way, unless otherwise stated. If P is the set of positive elements of G then the set of positive elements of H is H ∩ P.

Let (G,) be a family of ordered groups; according to the definition of the product of ordered sets (Set Theory, III, p. 137) the product group G = $ \prod G_i $ is equipped with an ordering, the relation « (x,) ≤ (y,) » between two elements of G being by definition the same as « x, ≤ y, for all α ». It is immediate that this ordering is compatible with the group structure of G; this ordering makes G an ordered group which we call the product of the ordered groups G,. The positive elements of G are those elements all of whose components are positive. In the case where all the factors G, are identical to the same ordered group H, then G is the group H' of maps from the index set I into H, the relation « f ≤ g » between two maps from I into H being the same as « f(α) ≤ g(α) for all α ∈ I »; the positive maps are those which take only positive values. The direct sum of a family (G,) of ordered groups is defined as an ordered subgroup of their product (II, p. 202).

Let (G_i)_i, be a family of ordered groups whose index set I is well ordered: recall (Set Theory, III, p. 157) that an order relation, called the lexicographic ordering, is defined on the product set G = $ \prod G_i $, the relation « (x,) < (y,) » between two elements of G being by definition the same as « if β is the smallest of the indices i such that x_i ≠ y_i, then x_β < y_β ». Recall that the product of a well ordered family of totally ordered sets is totally ordered under the lexicographic ordering. In the general case, the lexicographic ordering on G is compatible with its group structure, as is immediately verified; equipped with this ordering, the group G is thus an ordered group, called the lexicographic product of the well ordered family of ordered groups (G,).

#### Remark 1 {#alg-vi-s1-n6-rem-1 .statement}

In the commonest cases, the well ordered index set I will be a finite interval (1, n) in N.
    2) The set of positive elements of the lexicographic product G consists of 0 and those nonzero elements whose nonzero component of least index is positive.

### 7. Increasing homomorphisms of ordered groups

Let G and G' be two ordered groups; among the homomorphisms f from the underlying additive group of G into that of G', it makes sense to consider the increasing maps, that is those such that x ≤ y implies f(x) ≤ f(y). Because of the relation $ f(y - x) = f(y) - f(x) $ it follows that the increasing homomorphisms from G into G' are characterised by the fact that the image of a positive element of G under such a homomorphism is a positive element of G'; if P (resp. P') denotes the set of positive elements of G (resp. G'), this can be written $ f(P) \subset P' $. It is clear that the canonical injection of a subgroup G into an ordered group G', and the projection of a product of ordered groups onto one of its factors, are increasing homomorphisms.

An isomorphism (VI, p. 2) $ f $ from an ordered group G onto an ordered group G' is a bijective homomorphism from G onto G' such that both $ f $ and the inverse homomorphism are increasing, in other words $ f(P) = P' $.

It can happen that an isomorphism from the underlying group of G onto that of G' can be increasing without the inverse isomorphism also being increasing. This is the case, for example, if $ G = G' $, if $ f $ is the identity map on G, and if $ P \subset P' $ but $ P \neq P' $. Thus in $ \mathbf{Z} $ we can take $ P' $ to be the set of (ordinary) positive integers and P to be the set of even positive integers.

(DIV) Let K be the field of rational functions $ F_2(X) $ over the field $ F_2 $ of order 2. The divisibility relations relative to the rings $ F_2[X] = A' $ and $ F_2[X^2, X^3] = A $ define two distinct ordered group structures on $ K^* $, such that $ A \subset A' $ (they are ordered group structures since 1 is the only unit in A and the only unit in A').

### 8. Suprema and infima in an ordered group

Recall (Set Theory, III, p. 141) that if the set of upper bounds of a subset F of an ordered set E (that is to say the set of $ z \in E $ such that $ x \leq z $ for all $ x \in F $) has a least element a, then this element, which is then unique, is called the supremum of F. If F is the set of elements in a family $ (x_i)_i $, of elements of E, its supremum, if it exists, is denoted $ \sup x_i $ (or $ \sup x_i $ or simply $ \sup(x_i) $) ; if it is a finite family $ (x_i) $ ($ 1 \leq i \leq n $), this supremum is also denoted $ \sup_{\text{LEI}} (x_1, \ldots, x_n) $. The infimum is defined in an analogous manner and is denoted inf. The operations sup and inf are associative and commutative.

Recall (Set Theory, loc. cit.) that if F is a subset of an ordered set E, and $ (x_i) $ a family of elements of F, then the existence of $ \sup(x_i) $ in E (which may be denoted $ \sup_E(x_i) $) does not imply the existence of a supremum of the $ x_i $ in F (which may be denoted $ \sup_F(x_i) $ when it does exist); if both exist we know only that $ \sup_E(x_i) \leq \sup_F(x_i) $; however if $ \sup_E(x_i) $ exists and belongs to F, then $ \sup_F(x_i) $ exists and is equal to $ \sup_E(x_i) $. For example, in the polynomial ring $ A = K[X, Y] $ (K a field), the principal ideals AX and AY have the ideal $ AX + AY $ as supremum (under the relation $ \subset $) in the ordered set of ideals of A, but have the ideal A as supremum in the set of all principal ideals of A.

(DIV) An element d of $ K^* $ is called a greatest common divisor, or gcd for short, of a family $ (x_i) $ of elements of $ K^* $, if the principal fractional ideal (d) is the supremum in $ \mathcal{P}^* $ (under the relation $ \subset $) of the family of ideals $ ((x_i)) $, or in other words if the relation $ z \mid d $ for $ z \in K^* $ is equivalent to « $ z \mid x_i $ for all $ i $ ». In the same way we will say that $ m \in K^* $ is a least common multiple or an lcm of the family $ (x_i) $ if $ (m) $ is the infimum in $ \mathcal{P}^* $ of the family of ideals $ ((x_i)) $, that is if m | z is equivalent to « x_i | z for all i ». It amounts to the same thing to say that $ (m) = \cap_{i} (x_i) $; indeed, the condition $ x_i | z $ for all $ i $ is equivalent to $ z \in A x $, for all $ i $, that is to $ z \in \cap_{i} (x_i) $, and the condition $ m | z $ is equivalent to $ z \in (m)^1 $.

Note that if a principal fractional ideal (d) satisfies $ (d) = \sum (x_i) $ then d is a gcd of the family $ (x_i) $; but conversely a gcd of $ (x_i) $ does not necessarily satisfy the above condition (cf. VI, p. 33, Ex. 24).

The gcd and lcm, if they exist, are well defined modulo the subgroup U of units of $ K^* $, that is two gcd's (or two lcm's) of a given family are associate ; by abuse of language we will often write gcd$(x_i)$ and lcm$(x_i)$ for any of the gcd's or lcm's of the family $ (x_i) $, whenever such elements exist.

(DIV) By abuse of language we sometimes extend the notion of gcd to a family $ (x_i) $ of elements of K, some of which may be zero ; this gcd is again defined to be an element d such that the relation $ z | d $ is equivalent to « $ z | x_i $ for all $ i $ »; clearly d is 0 if all the $ x_i $ are zero ; otherwise d is a gcd of the nonzero $ x_i $. Similarly the lcm of a family, some elements of which are zero, is 0.

In an ordered group G, an immediate consequence of the invariance under translation of the ordering (VI, p. 2, Prop. 2) is that

(1)
$$
\sup(z + x_i) = z + \sup(x_i)
$$
in the sense that, whenever one side is defined, then so is the other and the two are equal. Similarly, it follows from the fact that the map $ x \mapsto -x $ takes the ordering of G to the opposite ordering (VI, p. 3, Cor.) that

(2)
$$
\inf(-x_i) = -(\sup(x_i)),
$$
this relation being understood in the same sense as the previous one.

#### Proposition 6 {#alg-vi-s1-prop-6 .statement}

— Let $ (x_i)_{i \in A}, (y_\beta)_{\beta \in B} $ be two families of elements of an ordered group G, each having a supremum. Then the family $ (x_\alpha + y_\beta)_{(\alpha, \beta) \in A \times B} $ has a supremum, and
$$
\sup_{(\alpha, \beta) \in A \times B} (x_\alpha + y_\beta) = \sup_{\alpha \in A} x_\alpha + \sup_{\beta \in B} y_\beta.
$$
Indeed, from $ x_\alpha + y_\beta \leq z $ for all $ \alpha $ and $ \beta $, we deduce $ \sup(x_i) + \sup(y_\beta) \leq z $ for all $ \beta $, and hence $ \sup(x_i) + \sup(y_\beta) \leq z $.

1 When A is the ring of integers (resp. the polynomial ring in one indeterminate with coefficients in a field), these definitions coincide with those of I, p. 112 (resp. IV, p. 12, Def. 1).

### 9. Lattice ordered groups

Recall that an ordered set in which every non empty finite subset has a supremum and an infimum is called a lattice (E, III, p. 13). It is clear that a product of lattice ordered groups, and in particular a product of totally ordered groups, is a lattice ordered group. In contrast a subgroup of a lattice ordered group is not necessarily lattice ordered.

Thus, in the product ordered group $ Z \times Z $, the « antidiagonal » (set of pairs $(n, n')$ such that $n + n' = 0$) is ordered with the discrete ordering, and hence is not a lattice ordered group. *The additive group of polynomials in one real variable (VI, p. 1, example 2) is a filtered group (since both $p(x)$ and $q(x)$ are less than $(p(x))^2 + (q(x))^2 + 1$) which one can show is not lattice ordered. \*

#### Proposition 7 {#alg-vi-s1-prop-7 .statement}

— *If x and y are two elements of an ordered group G, and if one of the elements $\inf(x, y)$, $\sup(x, y)$ exists, then so does the other, and $x + y = \inf(x, y) - \sup(x, y)$.

Indeed, according to the relations (1) and (2) (VI, p. 9) we have

$$
\sup(a - x, a - y) = a + \sup(-x, -y) = a - \inf(x, y),
$$

and it suffices to take $a = x + y$.

#### Proposition 7 {#alg-vi-s1-div-prop-7 .statement}

— *If $a, b \in K^*$, and if d is a gcd of a and b, and m an lcm of a and b, then the product dm is an associate of ab.

#### Proposition 8 {#alg-vi-s1-prop-8 .statement}

— *Let P be the set of positive elements of an ordered group G. For G to be lattice ordered, it is necessary and sufficient that $G = P - P$, and that in addition P, equipped with the induced ordering, satisfies one or other of the following conditions:

a) Each pair of elements of P has a supremum in P.
b) Each pair of elements of P has an infimum in P.

The necessity of these conditions is obvious : indeed the relation $G = P - P$ says that G is filtered (VI, p. 4, Prop. 4); on the other hand the supremum and infimum *in* G of two elements of P are positive, so are also their supremum and infimum in P.

Conversely, note first that under hypothesis a) (resp. b)), every pair of elements x, y of P has a supremum (resp. infimum) *in* G equal to its supremum a (resp. infimum b) *in* P. This is obvious for a, since any upper bound for x and y is positive; for b, let $z \in G$ be a lower bound for x and y; then there exists $u \in P$ such that $z + u \in P$, since $G = P - P$; now $\inf_P(x + u, y + u)$ is greater than $b + u$, and so is of the form $b + c + u$ ($c \geq 0$); since $b + c$ is less than x and less than y, we have $c = 0$; hence $\inf_P(x + u, y + u) = b + u$, which implies $z + u \leq b + u$, thus $z \leq b$ and b is certainly the infimum of x and y in G. Now if x and y are arbitrary elements of G we translate them into P: let $v \in P$ be such that $x + v$ and $y + v$ are positive (VI, p. 5, Prop. 5); under hypothesis a) (resp. b)) there exists a supremum (resp. infimum) for $ x + v $ and $ y + v $ in $ P $, and hence also in $ G $ by what we have just seen; by translation $ x $ and $ y $ have a supremum (resp. infimum) in $ G $; the existence of one of these implies the other, by Prop. 7, and this shows that the conditions are sufficient.

### 10. The decomposition theorem

#### Theorem 1 (decomposition theorem) {#alg-vi-s1-thm-1 .statement}

— *Let* $(x_i)_{1 \leq i \leq p}$ *and* $(y_j)_{1 \leq j \leq q}$ *be two finite sequences of positive elements of a lattice ordered group* $G$ *such that* $$
\sum_{i=1}^p x_i = \sum_{j=1}^q y_j ;
$$ *then there exists a double sequence* $(z_{ij})_{1 \leq i \leq p, 1 \leq j \leq q}$ *of positive elements of* $G$ *such that* $x_i = \sum_{j=1}^q z_{ij}$ *for all* $i$, *and* $y_j = \sum_{i=1}^p z_{ij}$ *for all* $j$.

1) Let us prove the theorem first for the case $p = q = 2$. Let $x, x', y, y'$ be positive elements of $G$ such that $x + x' = y + y'$, and put $a = \sup(0, x - y')$. Since
$$
x - y' = y - x'
$$
is less than $x$ and less than $y$, it follows that $b = x - a$ and $c = y - a$ are positive, as is $d = a - (x - y')$. Also we have
$$
x = a + b, \quad x' = c + d, \quad y = a + c \quad \text{and} \quad y' = b + d .
$$

2) Let us now show that if the theorem is true for $p < m$ and $q = n$ ($m > 2,\ n \geq 2$) then it is true for $p = m$ and $q = n$. By hypothesis we have $x, + \sum_{i=1}^{m-1} x_i = \sum_{j=1}^n y_j$. The theorem being true for $p = 2$ and $q = n$, there exist two finite sequences $(z_j'), (z_j'')$ of $n$ positive terms such that $\sum_{i=1}^{m-1} x_i = \sum_{j=1}^n z_j'$, $x_m = \sum_{j=1}^n z_j''$, and $y_j = z_j' + z_j''$ for $1 \leq j \leq n$. On the other hand, since the theorem is true for $p = m - 1$ and $q = n$, there exists a double sequence $(u_{ij})_{1 \leq i \leq m-1, 1 \leq j \leq n}$ such that $x_i = \sum_{j=1}^n u_{ij}$ for $1 \leq i \leq m - 1$, and $z_j' = \sum_{i=1}^{m-1} u_{ij}$ for $1 \leq j \leq n$. Putting
$$
z_{ij} = u_{ij} \quad \text{for} \quad 1 \leq i \leq m - 1 , \quad \text{and} \quad z_{mj} = z_j'' \quad (1 \leq j \leq n) ,
$$
we certainly obtain a double sequence satisfying the conditions of the theorem.

3) By interchanging the $x_i$ and the $y_j$ we see in the same way that, if the theorem is true for $p = m$ and $q < n$ ($m \geq 2,\ n > 2$), then it is true for $p = m$ and $q = n$. The theorem is thus proved by double induction starting from the case $p = q = 2$, for it is trivially true whenever $p \leq 1$ or $q \leq 1$.

#### Corollary {#alg-vi-s1-n10-cor-1 .statement}

— Let $ y, x_1, x_2, \ldots, x_n $ be $ n + 1 $ positive elements of $ G $ such that $ y \leq \sum_{i=1}^n x_i $; then there exist $ n $ positive elements $ y_i $ ($ 1 \leq i \leq n $) such that $ y_i \leq x_i $ and $ y = \sum_{i=1}^n y_i $.

It is sufficient to apply theorem 1 to the sequence $ (x_i) $ and the sequence consisting of the two elements $ y $ and $ z = \left( \sum_{i=1}^n x_i \right) - y $.

### 11. Positive and negative parts

#### Definition 4 {#alg-vi-s1-def-4 .statement}

— In a lattice ordered group $ G $ the positive part (resp. negative part, absolute value) of an element $ x \in G $ is the element $ \sup(x, 0) $ (resp. $ \sup(-x, 0) $, $ \sup(x, -x) $), which is denoted $ x^+ $ (resp. $ x^- $, $ |x| $).

Despite its name, the negative part $ x^- $ is a positive element.

Clearly $ x^- = (-x)^+ $ and $ |-x| = |x| $. Let us also note the following formulae, the first of which is an immediate consequence of the definitions and of the invariance of the ordering under translation, and the second of which follows from the first by Prop. 7 of VI, p. 10:

$$
\begin{cases}
\sup(x, y) = x + (y - x)^+ \\
\inf(x, y) = y - (y - x)^+
\end{cases}
$$

#### Proposition 9 {#alg-vi-s1-prop-9 .statement}

— a) For each element $ x $ of a lattice ordered group $ G $ we have $ x = x^+ - x^- $ and $ \inf(x^+, x^-) = 0 $.

b) For every expression of $ x $ as the difference of two positive elements, say $ x = u - v $, we have $ u = x^+ + w $ and $ v = x^- + w $ with $ w = \inf(u, v) $. In particular if $ \inf(u, v) = 0 $ then $ u = x^+ $ and $ v = x^- $.

c) The relation « $ x \leq y $ » is equivalent to « $ x^+ \leq y^+ $ and $ x^- \geq y^- $ ».

d) We have $ |x| = x^+ + x^- \geq 0 $.

e) For any $ x $ and $ y $ in $ G $, we have the inequality $ |x + y| \leq |x| + |y| $, and more generally $ \left| \sum_{i=1}^n x_i \right| \leq \sum_{i=1}^n |x_i| $ for any finite family $ (x_i) $ of elements of $ G $.

f) For any $ x $ and $ y $ in $ G $ we have $ ||x| - |y|| \leq |x - y| $.

We will prove a) and b) simultaneously. If $ x = u - v $ with $ u $ and $ v $ positive, then $ u $ a $ x $, so $ u \geq \sup(x, 0) = x^+ $, and $ w = u - x^+ $ is positive. On the other hand we have

$$
x^+ - x = \sup(x, 0) - x = \sup(x - x, -x) = x
$$

from which it follows that $ x = x^+ - x^- $, and $ v - x^- = w $. If $ z \leq x^- $ then $ z \leq x^+ - x $, and so $ x \leq x^+ - z $; if also $ z \leq x^+ $, then $ x^z - z $ is positive, and so x^i \leq x^+ - z \text{ by definition of } x^i. \text{ Hence we have } z \leq 0, \text{ which implies } \inf(x^+, x^-) = 0, \text{ whence by translation } \inf(u, v) = w.

c) The relation $ x \leq y $ implies $ \sup(y, 0) \geq x $ and $ \sup(y, 0) \geq 0 $, hence $ x^i \leq y^i $; similarly if $ -y \leq -x $ we deduce $ x^- \geq y^- $. The converse implication follows immediately from $ x = x^+ - x $ and $ y = y^+ - y $.

d) Since $ x \leq x^+ $ and $ -x \leq x^- $, it is clear that
$$
|x| = \sup(x, -x) \leq x^+ + x
$$
Conversely, if $ a \geq x $ and $ a \geq -x $ then we deduce from c) that $ a^+ \geq x^+ $, $ a^+ \geq x^- $, $ a^- \leq x^- $ and $ a^- \leq x^+ $; since $ a^- $ is positive and $ \inf(x^i, x^-) = 0 $, the last two inequalities imply $ a^- = 0 $ and $ a = a^+ $; the first two inequalities then give $ a \geq \sup(x^+, x^-) $, and $ \sup(x^+, x^-) $ is equal to $ x^+ + x^- $ by a) and by Prop. 7 of VI, p. 10.

e) Since $ x $ and $ y $ s $ |x| $ and $ y $, we have $ x + y \leq |x| + |y| $; since $ -x \leq |x| $ and $ -y \leq |y| $, we have $ -x - y \leq |x| + |y| $; whence the first inequality. The second follows by induction on n.

f) Replacing x and y by y and x - y in e), we obtain
$$
|x| - |y| \leq |x - y|
$$
similarly we have $ |y| - |x| \leq |y - x| = |x - y| $; whence the stated result.

#### Remark {#alg-vi-s1-n11-rem-1 .statement}

We deduce from d) that $ |x| = 0 $ implies $ x = 0 $ (for $ x^+ $ and $ x^- $ are positive); thus $ x \neq 0 $ implies $ |x| > 0 $.

#### Proposition 9 {#alg-vi-s1-div-prop-9 .statement}

— If the group $ \mathcal{P}^* $ of principal fractional ideals of K is lattice ordered, then every element x of $ K^* $ can be written in the form $ x = uv^{-1} $, where u and v are elements of A such that $ 1 = \gcd(u, v) $; for any other expression $ x = u'{v'}^{-1} $ of x as the quotient of two elements of A, we have $ u' = uw $ and $ v' = vw $, where w is a gcd of $ u', v' $; in particular if $ 1 = \gcd(u', v') $ then u' and v' are associates of u and v respectively.

Such an expression $ uv^{-1} $ for an element x of $ K^* $ is often called a reduced fraction.

### 12. Coprime elements

#### Definition 5 {#alg-vi-s1-def-5 .statement}

— In an ordered group two elements x and y are called coprime if $ \inf(x, y) = 0 $.

In some cases it is natural to define two elements to be coprime if $ \inf(|x|, |y|) = 0 $ (cf. INT, II, § 1) or to introduce the corresponding terminology in divisibility theory. We shall not do so here.

Two coprime elements are necessarily positive. The positive and negative parts $ x^+ $ and $ x^- $ of x are coprime (VI, p. 12, Prop. 9, a)). The elements $ x_i $ of a family (x,)_, , are said to be *setwise coprime* if $ \inf_{i \in I} x_i = 0 $; if the $ x_i $ are all $ \geq 0 $ then it is sufficient for there to exist a finite subset J of I such that the corresponding elements are setwise coprime. The elements of a family (x,) are said to be *pairwise coprime* if $ \inf(x_i, x_j) = 0 $ for every pair $ (\ell, \kappa) $ of distinct indices.

The $ x_i $ can be setwise coprime without being pairwise coprime.

If x and y are coprime, we also say that x is coprime to y, or that y is coprime to X

(DIV) Two elements x and y of K are said to be *coprime* if the principal ideals (x) and (y) are nonzero and coprime in $ \mathcal{P}^* $; this amounts to saying that 1 is a gcd of x and y, and implies that x and y *belong* to A. For example the numerator and denominator of a reduced fraction are coprime. The notions of pairwise and setwise coprime elements are defined similarly.

(DIV) When x and y are coprime, they are often said to be « prime to one another »; it is convenient to avoid this terminology, which can lead to confusion with the notion of prime numbers (I, p. 50, Def. 16).

#### Proposition 10 {#alg-vi-s1-prop-10 .statement}

*Let x, y and z be three elements of an ordered group ; for x – z and y – z to be coprime, it is necessary and sufficient that z = inf (x, y).*

Indeed the relations $ z = \inf(x, y) $ and $ 0 = \inf(x - z, y - z) $ are equivalent.

**Proposition 10 (DIV).** — *Let a, b and c be three elements of K with c $ \neq 0 $; for the quotients $ ac^{-1} $ and $ bc^{-1} $ to be coprime, it is necessary and sufficient that c be a gcd of a and b.*

#### Proposition 11 {#alg-vi-s1-prop-11 .statement}

*If $ (x_i), (y_j) $ are two finite families of positive elements of a lattice ordered group, then*

$$
\inf \left( \sum_i x_i, \sum_j y_j \right) \leq \sum_{i,j} \inf(x_i, y_j)
$$

Arguing by induction on the number of elements in the families $ (x_i) $ and $ (y_j) $, it is enough to prove that, if x, y and z are positive elements, then

$$
\inf(x, y + z) \leq \inf(x, y) + \inf(x, z).
$$

Indeed, put $ t = \inf(x, y + z) $; by VI, p. 12, Cor., we can write $ t = t_1 + t_2 $ with $ 0 \leq t_1 \leq y $ and $ 0 \leq t_2 \leq z $; since $ t_1 $ and $ t_2 $ are positive, we also have $ t_1 \leq x $ and $ t_2 \leq x $, whence $ t_1 \leq \inf(x, y) $ and $ t_2 \leq \inf(x, z) $.

#### Corollary 1 {#alg-vi-s1-prop-11-cor-1 .statement}

*If x and y are two coprime elements, and z a positive element, of a lattice ordered group, then $ \inf(x, z) = \inf(x, y + z) $.*

Indeed $ \inf(x, y + z) \leq \inf(x, z) $ by Prop. 11, and $ \inf(x, z) \leq \inf(x, y + z) $ since $ y \geq 0 $, whence the corollary.

#### Corollary 2 {#alg-vi-s1-prop-11-cor-2 .statement}

— In a lattice ordered group, if x and y are coprime and if z $ \geq 0 $ and $ x \leq y + z $, then $ x \leq z $.

#### Corollary 3 {#alg-vi-s1-prop-11-cor-3 .statement}

— In a lattice ordered group, if x is coprime to y and to z, then it is also coprime to $ y + z $.

#### Corollary 4 {#alg-vi-s1-prop-11-cor-4 .statement}

— If $ (x_i)_{1 \leq i \leq n} $ and $ (y_j)_{1 \leq j \leq m} $ are two finite families of elements of a lattice ordered group G, such that each $ x_i $ is coprime to each $ y_j $, then $ x_1 + \ldots + x_n $ is coprime to $ y_1 + \ldots + y_m $.
This follows from Cor. 3 by induction on m and n.

#### Corollary 5 {#alg-vi-s1-prop-11-cor-5 .statement}

— For any integer $ n \geq 0 $ we have $ (nx)^+ = nx^+ $ and $ (nx)^- = nx^- $; for all $ n \in \mathbf{Z} $ we have $ |nx| = |n| \cdot |x| $.
Indeed $ nx = nx^+ - nx^- $; since $ x^+ $ and x are coprime, so are $ nx^+ $ and $ nx^- $ if $ n \geq 0 $ (Cor. 4); the first assertion follows by Prop. 9 b) of VI, p. 12. The second follows from the first by Prop. 9 d) in the case $ n \geq 0 $; the case $ n < 0 $ follows from this as a result of the relation $ |-x| = |x| $.

#### Proposition 11 {#alg-vi-s1-div-prop-11 .statement}

— Suppose the set $ \mathcal{P}^* $ is a lattice, and let $ (a_i) $, $ (b_j) $ be two finite families of elements of A. Then every gcd of $ \prod_i a_i $ and $ \prod_j b_j $ divides the product $ \prod_{i,j} \gcd(a_i, b_j) $.

#### Corollary 1 {#alg-vi-s1-div-prop-11-cor-1 .statement}

— If a, b, c are three elements of A such that a is coprime to b, then every gcd of a and c is also a gcd of a and bc.

#### Corollary 2 (Euclid’s lemma) {#alg-vi-s1-div-prop-11-cor-2 .statement}

— Let a, b, c be three elements of A. If a is coprime to b and divides bc, then it divides c.

#### Corollary 3 {#alg-vi-s1-div-prop-11-cor-3 .statement}

— If x is coprime to y and to z, then it is coprime to yz.

#### Corollary 4 {#alg-vi-s1-div-prop-11-cor-4 .statement}

— If $ (x_i) $ and $ (y_j) $ are two finite families of elements of A such that each $ x_i $ is coprime to each $ y_j $, then the product of the $ x_i $ is coprime to the product of the $ y_j $.

#### Corollary 5 {#alg-vi-s1-div-prop-11-cor-5 .statement}

— If d is a gcd of x and y, then $ d^n $ is a gcd of $ x^n $ and $ y^n $ for each positive integer n.
Indeed $ xd^1 $ and $ yd^1 $ are coprime (Prop. 10 (DIV)), and hence so are $ x^n d^{-n} $ and $ y^n d^{-n} $ (Cor. 4).

#### Proposition 12 {#alg-vi-s1-prop-12 .statement}

— Let $ x_i $ ($ 1 \leq i \leq n $) be n pairwise coprime elements in a lattice ordered group. Then
$$
\sup(x_1, \ldots, x_n) = x_1 + \cdots + x_n .
$$

This follows from the formula $ u + v = \sup(u, v) + \inf(u, v) $ (VI, p. 10, Prop. 7) by induction on $ n $, using the fact that $ x_i $ is coprime to $ x_1 + \ldots + x_{i-1} $ for $ 2 \leq i \leq n $ (Cor. 4 to Prop. 11).

#### Remark {#alg-vi-s1-n12-rem-1 .statement}

Prop. 7 of VI, p. 10 also shows that a necessary and sufficient condition for $ x $ and $ y $ to be coprime is that $ x + y = \sup(x, y) $.

#### Proposition 12 {#alg-vi-s1-div-prop-12 .statement}

— *Let $ a_i $ be a finite number $ n $ of pairwise coprime elements of $ \mathbf{A} $; then the product $ a_1 \ldots a_n $, is an lcm of $ a_1, \ldots, a_n $.*

#### Proposition 13 {#alg-vi-s1-prop-13 .statement}

— *In a lattice ordered group $ G $, let $ (x_\alpha) $ be a family having an infimum (resp. supremum), and let $ z $ be an arbitrary element of $ G $; then the family $ (\sup(z, x_\alpha)) $ (resp. $ (\inf(z, x_\alpha)) $) has an infimum (resp. supremum) and*

$$
\begin{align*}
\inf_{\alpha} (\sup(z, x_\alpha)) &= \sup \left( z, \inf_{\alpha} x_\alpha \right) \\
\sup_{\alpha} (\inf(z, x_\alpha)) &= \inf \left( z, \sup_{\alpha} x_\alpha \right)
\end{align*}
$$

respectively.

Suppose that the family $ (x_\alpha) $ has an infimum $ y $. We will show that $ \sup(z, y) $ is an infimum of the family $ (\sup(z, x_\alpha)) $.

Indeed $ \sup(z, x_\alpha) = z + (x_\alpha - z)^+ $ and by translating we can reduce to the case $ z = 0 $, that is we must show that $ (x_\alpha^+) $ has an infimum equal to $ y^+ $. Since $ y \leq x_\alpha $ we have $ y^+ \leq x_\alpha^+ $ for all $ \alpha $ (VI, p. 12, Prop. 9, c)). Conversely, if $ a \leq x_\alpha^+ $ for all $ a $, then it follows that $ a \leq x_\alpha + x_\alpha^- $ (Prop. 9, a)); now $ y^- \geq x_\alpha^- $ since $ y \leq x_\alpha $; hence $ a \leq x_\alpha + y^- $ for all $ a $, that is $ a \leq y + y^- = y^+ $.

The other formula follows by changing to the opposite order relation.

#### Corollary {#alg-vi-s1-n12-cor-1 .statement}

— *If an element $ z $ of a lattice ordered group $ G $ is coprime to each element $ x_\alpha $ of a family having an infimum $ y $, then $ z $ is coprime to $ y $.*

This is an immediate consequence of the second formula (4).

#### Remark {#alg-vi-s1-n12-rem-2 .statement}

Applying the formulae of Prop. 13 to a family of two elements $ (x, y) $, we obtain the following formulae, which express the fact that each of the laws of composition sup, inf in a lattice ordered group is *distributive* with respect to the other :

$$
\begin{align*}
\sup(z, \inf(x, y)) &= \inf(\sup(z, x), \sup(z, y)) \\
\inf(z, \sup(x, y)) &= \sup(\inf(z, x), \inf(z, y)) .
\end{align*}
$$

This distributivity property is peculiar to lattice ordered *groups*, and does not extend to arbitrary lattices, or even to lattice ordered monoids (cf. VI, p. 33, Ex. 24).

### 13. Irreducible elements

#### Definition 6 {#alg-vi-s1-def-6 .statement}

— *An element x of an ordered group G is said to be irreducible if it is a minimal element in the set of strictly positive elements of G.*

Let x be an irreducible element of the ordered group G; if y is a positive element of G then the element inf(x, y), if it exists, can only be equal to x or to 0. Thus in a lattice ordered group G, every positive y is either greater than or coprime to the irreducible element x; in particular, two distinct irreducible elements are coprime.

(DIV) An element p of A is called *irreducible* if the ideal (p) is an irreducible element of the ordered group $ \mathcal{P}^* $; this says that p is neither zero nor invertible, and that any element of $ A $ which divides p is associate either to p or to 1. If $ \mathcal{P}^* $ is lattice ordered, then every $ a \in A $ is either coprime to p or a multiple of p.

*Examples (DIV). —* 1) An integer $ p > 0 $ is irreducible in $ \mathbf{Z} $ if and only if it is *prime* (I, p. 50).

2) A polynomial in one indeterminate over a field K is irreducible if and only if it is irreducible in the usual sense (IV, p. 13).

#### Proposition 14 {#alg-vi-s1-prop-14 .statement}

— *For an element $ x > 0 $ of an ordered group G to be irreducible it is sufficient that it satisfy the following property :*

(P) *The relations $ x \leq y + z,\ y \geq 0,\ z \geq 0 $ imply $ x \leq y $ or $ x \leq z $.*
*This condition is necessary when G is lattice ordered.*

If G is lattice ordered and x is irreducible, we have just seen that y is either greater than x or coprime to x; in the latter case Cor. 2 of VI, p. 15 shows that z is greater than x. Conversely, suppose the condition is satisfied: if $ 0 \leq y \leq x $ then it follows, by putting $ x = y + z\ (z \geq 0) $, that either $ x \leq y $ or $ x \leq z $; in the first case we have $ x = y $; in the second we have $ x \leq x - y $, so $ y \leq 0 $ and so $ y = 0 $; this shows that x is indeed irreducible.

#### Proposition 14 {#alg-vi-s1-div-prop-14 .statement}

— *For a nonzero element p of A to be irreducible it is sufficient that it not be a unit, and that it cannot divide a product of two elements of A without dividing one or other of them. This condition is necessary if $ \mathcal{P}^* $ is lattice ordered.*

#### Remark {#alg-vi-s1-n13-rem-1 .statement}

Proposition 14 (DIV) can also be expressed as follows: if p is a non zero element of A such that the ideal (p) is *prime* (I, p. 117, Def. 3) then p is irreducible; conversely, if $ \mathcal{P}^* $ is lattice ordered and p is irreducible then the ideal (p) is prime.

#### Proposition 15 {#alg-vi-s1-prop-15 .statement}

— *In an ordered group G, let $ (p_i)_{i \in I} $ be a family of pairwise distinct positive elements of G satisfying condition (P) (and hence irreducible). Then the map*

$$
(n_i)_{i \in I} \mapsto \sum_{i \in I} n_i p_i
$$

is an isomorphism of the ordered group $ \mathbf{Z}^{(1)} $, the direct sum of the ordered groups $ Z $ (VI, p. 7) onto the ordered subgroup of $ G $ generated by the $ p_\iota $.

It is enough to show that the relation $ \sum_{\iota \in I} n_\iota p_\iota \geq 0 $ is equivalent to $ n_\iota \geq 0 $ for all $ \iota $, for in particular the relation $ \sum_{\iota \in I} n_\iota p_\iota = 0 $ will imply $ n_\iota = 0 $ for all $ \iota $, hence this will show that the family $ (p_\iota) $ is linearly independent. Now let $ I' $ (resp. $ I'' $) be the finite subset of $ I $ consisting of those $ \iota $ such that $ n_\iota > 0 $ (resp. $ n_\iota < 0 $) ; we have

$$
\sum_{\iota \in I'} n_\iota p_\iota \geq \sum_{\iota \in I''} (-n_\iota)p_\iota .
$$

In particular, for $ \lambda \in I'' $, this implies that $ p_\lambda \leq \sum_{\iota \in I'} n_\iota p_\iota $, and it follows by induction from property (P) that we must have $ p_\lambda \leq p_\iota $ for some $ \iota \in I' $; since $ p_\iota $ is irreducible, this would imply $ p_\lambda = p_\iota $, which is absurd. Hence $ I' $ is empty, which proves the proposition.

#### Theorem 2 {#alg-vi-s1-thm-2 .statement}

— Let $ G $ be a filtered group. Then the following properties are equivalent :
a) $ G $ is isomorphic to an ordered group of the form $ \mathbf{Z}^{(1)} $.
b) $ G $ is lattice ordered and satisfies the following condition :
(MIN) Every nonempty set of positive elements of $ G $ has a minimal element.
c) $ G $ satisfies condition (MIN) and every irreducible element of $ G $ has property (P).
d) $ G $ is generated by its irreducible elements, and every irreducible element of $ G $ has property (P).

Let us show first that $ a) $ implies $ b) $. The group $ \mathbf{Z}^{(1)} $ is lattice ordered, as the direct sum of totally ordered groups. On the other hand let $ E $ be a nonempty set of positive elements of $ \mathbf{Z}^{(1)} $ and let $ x = \sum n_\iota e_\iota $ be an element of $ E $ (where $ (e_\iota) $ denotes the natural basis of $ \mathbf{Z}^{(1)} $) ; there are a finite number $ \prod (n_\iota + 1) $ of elements $ y $ of $ \mathbf{Z}^{(1)} $ such that $ 0 \leq y \leq x $, so the set $ F $ of elements of $ E $ which are less than or equal to $ x $ is $ a $ fortiori finite ; since it is nonempty, it contains a minimal element (Set Theory, III, p. 170, Cor. 2), which is clearly a minimal element of $ E $.

It is clear that $ b) $ implies $ c) $, by Prop. 14. Let us show that $ c) $ implies $ d) $. Since $ G $ is filtered, it is enough (VI, p. 4, Prop. 4) to check that the set $ F $ of positive elements of $ G $ which are sums of irreducible elements is equal to $ G_+ - \{0\} $. If this were not true, it would follow from (MIN) that the complement of $ F $ in $ G_+ - \{0\} $ would have a minimal element $ a $; by definition $ a $ is not irreducible, so is the sum of two strictly positive elements $ x $ and $ y $; since $ x < a $ and $ y < a $, these elements belong to $ F $, and so are sums of irreducible elements, and it follows that so is $ a $, which is a contradiction. Finally, $ d) $ implies $ a) $ by Prop. 15.

We will apply Th. 2 to the theory of divisibility in principal ideal domains (VII, p. 4) and in unique factorisation domains (AC, VII, § 3), as well as to the study of ideals in a Dedekind ring (AC, VII, § 2).

### Exercises {#alg-vi-s1-exercises}

See the [exercises for § 1](exercises/s1/).
