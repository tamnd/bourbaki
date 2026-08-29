---
book: ac
book_title: Commutative Algebra
chapter: VIII
chapter_title: DIMENSION
section: 1
section_title: Dimension de Krull d’un anneau
lang: en
source: ac-viii-ix-fr
book_pages: AC VIII.81-AC VIII.83
pdf_pages: 0005-0017, 0085-0087
extraction: ocr
subsections:
    - "no": 1
      title: Dimension de Krull d’un espace topologique
      page: 0
      pdf_page: 5
    - "no": 2
      title: Codimension d’une partie fermée
      page: 4
      pdf_page: 8
    - "no": 3
      title: Dimension d’un anneau, hauteur d’un idéal
      page: 6
      pdf_page: 10
    - "no": 4
      title: Dimension d’un module de type fini
      page: 10
      pdf_page: 14
    - "no": 5
      title: Cycles associés à un module
      page: 11
      pdf_page: 15
statements: 48
exercises: 17
content_sha256: 4ad0eb0f476452fa6aae6b7aefc9c174eae5e33a449664a5e3bb8d39db37c88d
translated_from: content/fr/ac/VIII/01_s1_dimension_de_krull_d_un_anneau.md
source_lang: fr
translation_method: machine
source_content_sha256: 39579207db3a1ec2253382ca725a94cb3a2ec6751a183b5842e7d93e1c5e7a32
translation_model: gpt-5.4
translation_run: translate-en-mt-19bddbec
glossary_version: 34
glossary_terms_sha256: a055231993bfec6f55fd1c3b30994f7ba0db74fcd788d1a51e943d376fccac0b
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 1. KRULL DIMENSION OF A RING

### 1. Krull Dimension of a Topological Space

#### Definition 1 {#ac-viii-s1-def-1 .statement}

Let $I$ be an ordered set. A nonempty finite totally ordered subset of $I$ is called a chain in $I$. Let $c$ be a chain in $I$; the smallest and greatest elements of $c$ are called the extremities of $c$. The integer $\mathrm{Card}(c) - 1$ is called the length of $c$. The inclusion relation in the set of subsets of $I$ induces an order relation in the set of chains in $I$. A chain $c$ in $I$ is said to be saturated if it is maximal among the chains in $I$ having the same extremities as $c$.

To designate a chain c of length n, we shall often write: “the chain $i_0 < \cdots < i_n$”, where the $i_k$ are the elements of c indexed in strictly increasing order by the integers from 0 to n.

Let X be a topological space. We equip the set of irreducible closed subsets of X (II, § 4, No. 1, Def. 1) with the order relation defined by inclusion. Whenever we speak of a chain of irreducible closed subsets of X, this will always mean a chain with respect to this order relation.

#### Definition 2 {#ac-viii-s1-def-2 .statement}

The Krull dimension of the topological space X is, by definition, and is denoted by dim kr(X), or simply dim(X), the least upper bound in $\overline{\mathbf{R}}$ of the set of lengths of chains of irreducible closed subsets of X.
For every point x of X, the Krull dimension of X at x is, by definition, and is denoted by $\dim_x(X)$, the greatest lower bound of the dimensions of the open neighbourhoods of x.

We have $\dim(\varnothing) = -\infty$. On the other hand, if X is nonempty, the closure of every point of X is an irreducible closed subset of X (II, § 4, No. 1, Prop. 2), and therefore the dimension of X is either $+\infty$ or a positive integer. Suppose that X is separated and nonempty; then every irreducible subset of X is reduced to a point, and X is of dimension 0.
The definition of Krull dimension is therefore devoid of interest for separated spaces, but it is specially adapted to the topological spaces encountered in Commutative Algebra (spectra of rings, \* schemes *, ...). In this chapter, no confusion is to be feared with other notions of dimension of topological spaces (for example, that of Lebesgue), and we shall simply say “dimension” for “Krull dimension”.

#### Proposition 1 {#ac-viii-s1-prop-1 .statement}

Let X be a topological space.
a) If Y is a subspace of X, then $\dim(Y) \leq \dim(X)$, and $\dim_y(Y) \leq \dim_y(X)$ for every point y of Y.
b) Let x be a point of X and V a neighbourhood of x in X. Then $\dim_x(X) = \dim_x(V)$.
c) Let $(X_i)_{i \in I}$ be a finite family of closed subsets of X such that $X = \bigcup_{i \in I} X_i$. Then $\dim(X) = \sup_{i \in I} \dim(X_i)$ and, for every point x of X, one has $\dim_x(X) = \sup_{i \in J_x} \dim_x(X_i)$, where $J_x$ denotes the set of $i \in I$ such that $x \in X_i$.

Let us prove a). If Z is an irreducible closed subset of Y, its closure $\overline{Z}$ in X is irreducible (II, § 4, No. 1, Prop. 2), and one has $\overline{Z} \cap Y = Z$. Thus every chain c of irreducible closed subsets of Y defines, by passing to the closure in X, a chain of irreducible closed subsets of X, of the same length as c. The inequality $\dim(Y) \leq \dim(X)$ follows from this. If U is an open subset of X containing a point y of Y, then therefore $\dim(U \cap Y) \leq \dim(U)$, whence $\dim_y(Y) \leq \dim_y(X)$.
Let us prove b). By definition one has $\dim_x(X) \leq \dim_x(V)$, and the opposite inequality follows from a).
Let us prove c). Let $Z_0 \subset \ldots \subset Z_n$ be a chain of irreducible closed subsets of X. One has $Z_n = \bigcup_{i \in I} (Z_n \cap X_i)$ and each of the sets $Z_n \cap X_i$ is closed in $Z_n$;

since I is finite, $Z_n$ is contained in one of the $X_i$. Consequently, one has $\dim(X) \leq \sup_{i} \dim(X_i)$, whence equality by *a*).

Now let $x$ be a point of $X$ and $n = \sup_{i \in J_x} \dim_x(X_i)$, where $J_x$ is as in the statement. One has $\dim_x(X) \geq n$ by *a*), and, to establish equality, one may suppose $n$ finite. For every $i \in J_x$, let $U_i$ be an open neighbourhood of $x$ in $X$, such that $\dim(U_i \cap X_i) \leq n$. Put $U = (\bigcap_{i \in J_x} U_i) \cap (\bigcap_{i \in I - J_x} \mathcal{C} X_i)$; the set $U$ is open in $X$. Moreover, one has $\dim(U) = \sup_{i \in J_x} \dim(U \cap X_i) \leq n$ by the preceding paragraph, hence $\dim_x(X) \leq n$.

#### Corollary {#ac-viii-s1-n1-cor-1 .statement}

*a*) *The dimension of the topological space $X$ is the least upper bound of the dimensions of its irreducible components* (II, § 4, No. 1, Def. 2).

*b*) *Let $x$ be a point of $X$. Then $\dim_x(X) \geq \sup \dim_x(X_i)$, where $X_i$ runs through the family of irreducible components of $X$ that contain $x$; there is equality if $x$ has a neighbourhood $V$ which has only a finite number of irreducible components (which is the case for example if $V$ is noetherian)*.

The first assertion is immediate since the chains of irreducible closed subsets of $X$ are the chains of irreducible closed subsets of the irreducible components of $X$ (II, § 4, No. 1, Prop. 5). The inequality $\dim_x(X) \geq \sup_{i} \dim_x(X_i)$ follows from Prop. 1, *a*). Let $V$ be a neighbourhood of $x$ which has only a finite number of irreducible components, and let $(V_j)_{j \in J}$ be the family of irreducible components of $V$ which contain $x$. It follows from Prop. 1, *b*) and *c*) that one has
$$
\dim_x(X) = \dim_x(V) = \sup_{j \in J} \dim_x(V_j);
$$
one concludes by remarking that each of the $V_j$ is contained in one of the $X_i$, $i \in J_x$, and that one therefore has $\sup_{j \in J} \dim_x(V_j) \leq \sup_{i \in J_x} \dim_x(X_i)$.

#### Proposition 2 {#ac-viii-s1-prop-2 .statement}

*Let $X$ be a topological space. Then $\dim(X) = \sup_{x \in X} \dim_x(X)$*.

In fact, by definition one has $\dim(X) \geq \dim_x(X)$ for every $x \in X$. On the other hand, if $Z_0 \subset ... \subset Z_n$ is a chain of irreducible closed subsets of $X$, for every $x \in Z_0$ and every open neighbourhood $U$ of $x$, the sets $Z_0 \cap U, ..., Z_n \cap U$ form a chain of irreducible closed subsets of $U$ (II, § 4, No. 1, Prop. 7). Hence $\dim_x(X) \geq n$, whence $\dim(X) \leq \sup_{x \in X} \dim_x(X)$.

#### Corollary {#ac-viii-s1-n1-cor-2 .statement}

*If $(X_\alpha)_{\alpha \in A}$ is an open covering, or a locally finite closed covering, of a topological space $X$, one has*
$$
\dim(X) = \sup_{\alpha \in A} \dim(X_\alpha).
$$

It is enough to prove that, for every point $x$ of $X$, one has $\dim_x(X) = \sup_{\alpha \in A_x} \dim_x(X_\alpha)$, where $A_x$ is the set of $\alpha \in A$ such that $x \in X_\alpha$. This is clear in the case of an open covering, and follows from Prop. 1, c), in the case of a locally finite closed covering.

### 2. Codimension of a closed subset

#### Definition 3 {#ac-viii-s1-def-3 .statement}

Let X be a topological space.

a) If Y is an irreducible closed subset of X, the codimension of Y in X is defined to be the least upper bound in $\overline{\mathbf{R}}$ of the lengths of chains of irreducible closed subsets of X of which Y is the smallest element.

b) If Y is a closed subset of X, the codimension of Y in X is defined to be the greatest lower bound in $\overline{\mathbf{R}}$ of the codimensions, in X, of the irreducible components of Y, and is denoted by $\operatorname{codim}(Y, X)$.

#### Remark 1 {#ac-viii-s1-n2-rem-1 .statement}

The codimension of a closed subset Y of X is therefore the greatest lower bound of the codimensions of the irreducible closed subsets of Y. One has $\operatorname{codim}(\varnothing, X) = +\infty$ and, if X is not empty, $\operatorname{codim}(X, X) = 0$. Every nonempty closed subset of X contains an irreducible closed subset (II, § 4, No. 1, Prop. 5); the codimension in X of a closed subset Y is therefore always a positive integer or $+\infty$; it is zero if and only if Y contains an irreducible component of X.

#### Remark 2 {#ac-viii-s1-n2-rem-2 .statement}

If Y is a nonempty closed subset of X, one has $\operatorname{codim}(Y, X) \leq \dim(X)$. One has $\dim(X) = \sup_Y \operatorname{codim}(Y, X)$, where Y runs through the set of irreducible closed subsets of X. If Y and Y’ are two closed subsets of X such that $Y' \subset Y$, one has $\operatorname{codim}(Y, X) \leq \operatorname{codim}(Y', X)$.

#### Remark 3 {#ac-viii-s1-n2-rem-3 .statement}

Let $Y$ be a closed subset of the topological space $X$ and $(X_\alpha)_{\alpha \in A}$ (resp. $(Y_\beta)_{\beta \in B}$) the family of irreducible components of $X$ (resp. of $Y$). For each $\beta \in B$, let $A(\beta)$ denote the set of $\alpha \in A$ such that $Y_\beta \subset X_\alpha$. Since every irreducible subset of $X$ is contained in one of the $X_\alpha$ (II, § 4, No. 1, Prop. 5), it follows from Def. 3 that one has:

$$
\operatorname{codim}(Y, X) = \inf_{\beta \in B} \sup_{\alpha \in A(\beta)} \operatorname{codim}(Y_\beta, X_\alpha).
$$

#### Remark 4 {#ac-viii-s1-n2-rem-4 .statement}

Let $(Y_i)_{i \in I}$ be a finite family of closed subsets of $X$ and $Y = \bigcup_{i \in I} Y_i$; one has

$$
\operatorname{codim}(Y, X) = \inf_{i \in I} \operatorname{codim}(Y_i, X).
$$

In fact, every irreducible component of $Y$ is contained in one of the $Y_i$.

#### Proposition 3 {#ac-viii-s1-prop-3 .statement}

Let $X$ be a topological space.

a) For every nonempty closed subset $Y$ of $X$, one has

$$
\dim(Y) + \operatorname{codim}(Y, X) \leq \dim(X).
$$

b) If $Y, Z, T$ are closed subsets of $X$ such that $Y \subset Z \subset T$, one has

$$
\operatorname{codim}(Y, Z) + \operatorname{codim}(Z, T) \leq \operatorname{codim}(Y, T).
$$

It is enough to prove assertion a) in the case where $\dim(X)$ is finite. In this case, $\dim(Y)$ and $\operatorname{codim}(Y, X)$ are finite. There exists a chain $Y_0 \subset ... \subset Y_n$ of irreducible closed subsets of $Y$, of length $n = \dim(Y)$, and a chain $Y_n \subset ... \subset Y_{n+p}$ of irreducible closed subsets of $X$, of length $p \geq \operatorname{codim}(Y, X)$. It follows that $\dim(X) \geq n + p$, whence a). To establish b), one may suppose $Y$ irreducible. Since one has $\operatorname{codim}(Y, Z) \leq \operatorname{codim}(Y, T)$, the inequality is proved if $\operatorname{codim}(Y, Z) = +\infty$. Otherwise, let $Z_0$ be an irreducible component of $Z$ containing $Y$ and such that $\operatorname{codim}(Y, Z) = \operatorname{codim}(Y, Z_0)$. One has $\operatorname{codim}(Z, T) \leq \operatorname{codim}(Z_0, T)$, and one sees, as above, that $\operatorname{codim}(Y, Z_0) + \operatorname{codim}(Z_0, T) \leq \operatorname{codim}(Y, T)$, whence b).

#### Definition 4 {#ac-viii-s1-def-4 .statement}

A topological space $X$ is said to be catenary if, for every pair $(Y, Z)$ of irreducible closed subsets of $X$ such that $Y \subset Z$, every saturated chain of irreducible closed subsets with extremities $Y$ and $Z$ is of length $\operatorname{codim}(Y, Z)$.

It comes to the same thing to say that, for every pair $(Y, Z)$ of irreducible closed subsets of $X$ such that $\operatorname{codim}(Y, Z)$ is finite, all saturated chains with extremities $Y$ and $Z$ have the same length, and that, for every pair $(Y, Z)$ such that $\operatorname{codim}(Y, Z) = +\infty$, there exists no saturated chain with extremities $Y$ and $Z$.

Every closed subspace of a catenary space is catenary. In order that a space be catenary, it is necessary and sufficient that its irreducible components be so.

#### Proposition 4 {#ac-viii-s1-prop-4 .statement}

Let $X$ be a topological space. In order that $X$ be catenary, it is necessary and sufficient that, for every triplet $(Y, Z, T)$ of irreducible closed subsets of $X$ such that $Y \subset Z \subset T$, one have:

$$
\operatorname{codim}(Y, T) = \operatorname{codim}(Y, Z) + \operatorname{codim}(Z, T)
$$

Suppose $X$ catenary. In view of Prop. 3, b), it is enough to prove the relation when $\operatorname{codim}(Y, Z)$ and $\operatorname{codim}(Z, T)$ are finite. By joining end to end a saturated chain of irreducible closed subsets with extremities $Y$ and $Z$, of length $\operatorname{codim}(Y, Z)$, and a saturated chain of irreducible closed subsets with extremities $Z$ and $T$, of length $\operatorname{codim}(Z, T)$, one obtains a saturated chain with extremities $Y$ and $T$, of length $\operatorname{codim}(Y, Z) + \operatorname{codim}(Z, T)$. But, since $X$ is catenary, this length is necessarily equal to $\operatorname{codim}(Y, T)$.

Conversely, suppose that one has $\operatorname{codim}(Y, T) = \operatorname{codim}(Y, Z) + \operatorname{codim}(Z, T)$ for any irreducible closed subsets $Y, Z, T$ of $X$ such that $Y \subset Z \subset T$, and let us prove that $X$ is catenary. To do this, let us prove by induction on the integer $n \geq 0$ that, for every saturated chain $Z_0 \subset ... \subset Z_n$ of irreducible closed subsets of $X$, one has $\operatorname{codim}(Z_0, Z_n) = n$. If $n = 0$, this is clear. Let $n > 0$, and suppose the property holds for chains of length $\leq n - 1$. If $Z_0 \subset ... \subset Z_n$ is a saturated chain of length $n$, then $Z_0 \subset ... \subset Z_{n-1}$ is a saturated chain of length $n - 1$, hence $\operatorname{codim}(Z_0, Z_{n-1}) = n - 1$. In view of the assumption made on $X$, one has $\operatorname{codim}(Z_0, Z_n) = \operatorname{codim}(Z_0, Z_{n-1}) + \operatorname{codim}(Z_{n-1}, Z_n) = (n - 1) + 1 = n$.

#### Corollary {#ac-viii-s1-n2-cor-1 .statement}

Let X be an irreducible topological space of finite dimension. In order that X be catenary, it is necessary and sufficient that, for every pair (Y, Z) of irreducible closed subsets of X such that Y ⊂ Z, one has codim(Y, X) = codim(Y, Z) + codim(Z, X).

The condition is necessary by Prop. 4. Conversely, suppose it satisfied, and denote by c(Z) the integer codim(Z, X) for every irreducible closed subset Z of X. If Y, Z, T are three irreducible closed subsets of X such that Y ⊂ Z ⊂ T, one has
$$
\begin{align*}
\operatorname{codim}(Y, Z) + \operatorname{codim}(Z, T) &= (c(Y) - c(Z)) + (c(Z) - c(T)) \\
&= c(Y) - c(T) \\
&= \operatorname{codim}(Y, T),
\end{align*}
$$
and X is catenary by Prop. 4.

#### Proposition 5 {#ac-viii-s1-prop-5 .statement}

Let X be a topological space of finite dimension. Suppose that all maximal chains of irreducible closed subsets of X have the same length. Then X is catenary; for every irreducible closed subset Z of X, one has
$$
\operatorname{codim}(Z, X) = \dim(X) - \dim(Z);
$$
for every pair (Y, Z) of irreducible closed subsets of X such that Y ⊂ Z, one has
$$
\operatorname{codim}(Y, Z) = \dim(Z) - \dim(Y).
$$

Let Y and Z be two irreducible closed subsets of X such that Y ⊂ Z. Let Y_0 ⊂ ... ⊂ Y_p be a chain such that Y_p = Y and p = \dim(Y), Z_0 ⊂ ... ⊂ Z_q a chain such that Z_0 = Z and q = \operatorname{codim}(Z, X). For every saturated chain T_0 ⊂ ... ⊂ T_r such that T_0 = Y and T_r = Z, the chain
$$
Y_0 \subset ... \subset Y_{p-1} \subset T_0 \subset ... \subset T_r \subset Z_1 ... \subset Z_q
$$
is maximal, and of length p + q + r; by the assumption made on X, one has therefore p + q + r = \dim(X), that is r = \dim(X) - \dim(Y) - \operatorname{codim}(Z, X). It follows that X is catenary and that, for Y and Z as above, one has
$$
\dim(Y) + \operatorname{codim}(Y, Z) = \dim(X) - \operatorname{codim}(Z, X).
$$
Taking Y = Z, one sees that the second member is equal to \dim(Z), whence the proposition.

### 3. Dimension of a ring, height of an ideal

#### Definition 5 {#ac-viii-s1-def-5 .statement}

The Krull dimension, or simply dimension, of a (commutative) ring A is by definition the Krull dimension of the topological space Spec(A) (II, § 4, No. 3, Def. 4); it is denoted by \dim(A). If p is a prime ideal of A, the dimension of A at p is by definition the number \dim_p(\operatorname{Spec}(A)); it is denoted by \dim_p(A).

The mapping $p \mapsto V(p)$ is a decreasing bijection of the set of prime ideals of $A$ onto the set of irreducible closed subsets of $\mathrm{Spec}(A)$ (*loc. cit.*, Cor. 2 to Prop. 14). *The dimension of $A$ is therefore the least upper bound of the set of lengths of chains of prime ideals of $A$*; it is equal to $-\infty, +\infty$ or to a positive integer.

Let $p \in \mathrm{Spec}(A)$; the sets $\mathrm{Spec}(A)_f$, where $f$ runs through $A$, form a basis for the topology of $\mathrm{Spec}(A)$, and $p$ belongs to the open set $\mathrm{Spec}(A)_f$ if and only if $f$ does not belong to $p$. Consequently, $\dim_p(A)$ is the greatest lower bound of the numbers $\dim(A_f)$, where $f$ runs through $A - p$ (II, § 5, No. 1, Prop. 1).

#### Example 1 {#ac-viii-s1-n3-exa-1 .statement}

One has $\dim(A) < 0$ if and only if $A$ is reduced to 0. In order that one have $\dim(A) \leqslant 0$, it is necessary and sufficient that every prime ideal of $A$ be maximal. Integral rings of dimension 0 are fields. A noetherian ring is of dimension $\leqslant 0$ if and only if it is artinian (IV, § 2, No. 5, prop. 9).

#### Example 2 {#ac-viii-s1-n3-exa-2 .statement}

Dedekind rings are noetherian integrally closed rings of dimension $\leqslant 1$ (VII, § 2, No. 2, th. 1). More generally, by V, § 1, No. 2, cor. 2 to prop. 9, a ring is a finite product of Dedekind rings if and only if it is noetherian, reduced, integrally closed in its total ring of fractions, and of dimension $\leqslant 1$.

#### Example 3 {#ac-viii-s1-n3-exa-3 .statement}

If $A$ is a valuation ring (VI, § 1, No. 2, def. 2), its dimension is equal to the height of the valuation (VI, § 4, No. 4, prop. 5).

#### Example 4 {#ac-viii-s1-n3-exa-4 .statement}

Let $A$ be a ring. One has
$$
\dim(A[X]) \geqslant \dim(A) + 1 .
$$
In fact, if $p_0 \subset ... \subset p_n$ is a chain of prime ideals of $A$, of length $n$, one obtains a chain $p'_0 \subset ... \subset p'_{n+1}$ of prime ideals of $A[X]$, of length $n + 1$, by putting $p'_i = p_i A[X]$ for $0 \leq i \leq n$, and $p'_{n+1} = p_n A[X] + XA[X]$.

By the same reasoning, one proves the inequality $\dim(A[[X]]) \geqslant \dim(A) + 1$. One deduces by induction the inequalities
$$
\dim(A[X_1, ..., X_n]) \geqslant \dim(A) + n ,
$$
$$
\dim(A[[X_1, ..., X_n]]) \geqslant \dim(A) + n .
$$

We shall prove later (§ 3, No. 4, cor. 3 to prop. 7 and cor. 3 to prop. 8) that one has equality in the two preceding formulae when $A$ is noetherian.

#### Example 5 {#ac-viii-s1-n3-exa-5 .statement}

Let $X$ be a complex analytic variety. If $X$ is of complex dimension $n$ at a point $x$ of $X$, the local ring of germs at $x$ of analytic functions on $X$ is of dimension $n$. \*

#### Example 6 {#ac-viii-s1-n3-exa-6 .statement}

Let $k$ be a field and $A$ a nonzero integral $k$-algebra. Then one has $\dim(A) = 0$. This results from cor. 1 to prop. 1 of V, § 2, No. 1, and from the fact that $\dim(k) = 0$.

#### Example 7 {#ac-viii-s1-n3-exa-7 .statement}

If $\mathfrak{n}$ is a nilideal of $A$, $\mathrm{Spec}(A)$ is homeomorphic to $\mathrm{Spec}(A/\mathfrak{n})$ (II, § 4, No. 3, remark). Therefore one has $\dim(A/\mathfrak{n}) = \dim(A)$; in particular, one has $\dim(A) = \dim(A_{\mathrm{red}})$ where $A_{\mathrm{red}}$ is the quotient of the ring $A$ by its nilradical.

#### Example 8 {#ac-viii-s1-n3-exa-8 .statement}

There exist noetherian rings of infinite dimension (p. 83, exercise 13). We shall see below (§ 3, No. 1, cor. 1 to prop. 2) that every noetherian local ring is of finite dimension.

#### Proposition 6 {#ac-viii-s1-prop-6 .statement}

Let A be a ring.
a) If a is an ideal of A, one has dim(A/a) $\leq$ dim(A).
b) If S is a multiplicative subset of A, one has dim(S$^{-1}$A) $\leq$ dim(A).
c) One has dim(A) = sup dim(A/p), where p runs through the set of minimal prime ideals of A.
d) If A has only a finite number of minimal prime ideals (for example if A is noetherian (II, § 4, No. 3, cor. 3 to prop. 14)) and if p is a prime ideal of A, one has
$$
\dim_p(A) = \sup_q \dim_{p/q}(A/q),
$$
where q runs through the set of minimal prime ideals of A contained in p.
e) Let a be an ideal of A which is contained in no minimal prime ideal of A; then one has dim(A) $\geq$ dim(A/a) + 1. In particular, if A is integral, one has dim(A) $\geq$ dim(A/a) + 1 for every nonzero ideal a of A.

By the remark of II, § 4, No. 3, if a is an ideal of A, the topological space Spec(A/a) is homeomorphic to the closed subspace V(a) of Spec(A). Assertion a) results from this and from prop. 1, a) of No. 1. Assertion b) results from loc. cit., corollary to prop. 13. By loc. cit., cor. 2 to prop. 14, the irreducible components of Spec(A) are homeomorphic to the spaces Spec(A/p), where p is a minimal prime ideal of A, and assertion c) results from the corollary of prop. 1 of No. 1. Under the assumption of d), the space Spec(A) has only a finite number of irreducible components; the irreducible components of Spec(A) containing p are the sets V(q), where q is a minimal prime ideal contained in p. Assertion d) then results from cor., b) of prop. 1 of No. 1.

Let us prove e) finally. It is a question of proving that, for every chain $p_0 \subset ... \subset p_n$ of prime ideals of A such that $a \subset p_0$, one has dim(A) $\geq n + 1$. In view of the assumption made on a, there exists a prime ideal $p_{-1}$ of A contained in $p_0$, distinct from $p_0$, and $p_{-1} \subset p_0 \subset ... \subset p_n$ is a chain of prime ideals of A, of length $n + 1$.

#### Remark 1 {#ac-viii-s1-n3-rem-1 .statement}

Let $\rho : A \to B$ be a homomorphism of rings. Then dim(B) is the least upper bound of the numbers dim(B/$\rho(p)$.B), where p runs through the set of minimal prime ideals of A: in fact, for every minimal prime ideal q of B, there exists a minimal prime ideal p of A contained in $\rho^{-1}(q)$ (II, § 2, No. 6, Lemma 2), and one has
$$
\dim(B/q) \leq \dim(B/\rho(p).B) \leq \dim(B)
$$
by Proposition 6, a); one concludes by Proposition 6, c).

#### Definition 6 {#ac-viii-s1-def-6 .statement}

Let a be an ideal of a ring A. The codimension of V(a) in Spec(A) is called the height of the ideal a and is denoted by ht(a).

Assume that A is an integral domain. Then the prime ideals of height 1 of A in the sense of Definition 4 of VII, § 1, No. 6, are the prime ideals of height 1 in the sense of the above definition.

#### Proposition 7 {#ac-viii-s1-prop-7 .statement}

a) The height of a prime ideal p of A is the least upper bound of the lengths of chains of prime ideals $p_0 \subset ... \subset p_n$ such that $p_n = p$.

b) Let p be a prime ideal of A and a an ideal of A. Then one has $\dim(A_p/aA_p) = -\infty$ if a is not contained in p, and $\dim(A_p/aA_p) = \operatorname{codim}(V(p), V(a))$ if a is contained in p. In particular, if p is a prime ideal of A, one has $\dim(A_p) = \operatorname{ht}(p)$.

c) If a is an ideal of A, one has $\operatorname{ht}(a) = \inf_{p} \operatorname{ht}(p) = \inf_{p} \dim(A_p)$ where p runs through the set of prime ideals of A containing a.

Assertion a) is the translation of Definition 3, a) of No. 2. Assertion b) follows from the fact that the mapping $q \mapsto q(A_p/aA_p)$ is an increasing isomorphism of the set of prime ideals q of A such that $a \subset q \subset p$ onto the set of prime ideals of the local ring $A_p/aA_p$ (II, § 2, No. 5, Proposition 11). Let a be an ideal of A; the irreducible closed subsets of $V(a)$ are the sets $V(p)$, where p is a prime ideal of A containing a. Assertion c) therefore follows from Remark 1 of No. 2.

#### Corollary {#ac-viii-s1-n3-cor-1 .statement}

Let p be a prime ideal of A and S a multiplicative subset of A not meeting p. Then $\operatorname{ht}(p) = \operatorname{ht}(S^{-1}p)$.

This follows from Proposition 7, a), and from II, § 2, No. 5, Proposition 11.

#### Proposition 8 {#ac-viii-s1-prop-8 .statement}

Let A be a ring.

a) One has $\dim(A) = \sup_m \dim(A_m) = \sup_m \operatorname{ht}(m)$, where m runs through the set of maximal (resp. prime) ideals of A.

b) Let b be an ideal of A distinct from A, and a an ideal of A contained in b. Then one has $\operatorname{codim}(V(b), V(a)) + \dim(A/b) \leq \dim(A/a)$. In particular, for every ideal b of A distinct from A, one has the inequality $\operatorname{ht}(b) + \dim(A/b) \leq \dim(A)$.

The first assertion follows from Remark 2 of No. 2 and from Proposition 7, b). The second follows from Proposition 3, a) of No. 2 and from the relations $\dim(A/b) = \dim(V(b))$, $\dim(A/a) = \dim(V(a))$.

#### Definition 7 {#ac-viii-s1-def-7 .statement}

A ring A is said to be catenary if the topological space Spec(A) is catenary (No. 2, Definition 4).

This therefore means that, for every pair (p, q) of prime ideals of A such that $q \subset p$, all saturated chains of prime ideals of A with endpoints p and q have length $\operatorname{codim}(V(p), V(q)) = \dim(A_p/qA_p)$.

#### Remark 2 {#ac-viii-s1-n3-rem-2 .statement}

Every quotient ring of a catenary ring is catenary. In order that the ring A be catenary, it is necessary and sufficient that, for every prime ideal p of A, the ring $A_p$ be catenary.

#### Remark 3 {#ac-viii-s1-n3-rem-3 .statement}

By Proposition 7, b) and Proposition 4 of No. 2, the ring A is catenary if and only if, for every triple (p, q, r) of prime ideals of A such that $r \subset q \subset p$, one has dim(A_p/qA_p) + dim(A_q/rA_q) = dim(A_p/rA_p). If A is an integral domain and of finite dimension, then A is catenary if and only if one has ht(q) + dim(A_p/qA_p) = ht(p) for every pair (p, q) of prime ideals of A such that q ⊂ p. In fact, the topological space Spec(A) is then irreducible and of finite dimension, and one applies the Corollary to Proposition 4 of No. 2.

#### Remark 4 {#ac-viii-s1-n3-rem-4 .statement}

Let A be a ring of finite dimension, all maximal chains of whose prime ideals have the same length. Then A is catenary, one has ht(p) + dim(A/p) = dim(A) for every prime ideal p of A, and dim(A_p/qA_p) + dim(A/p) = dim(A/q) for every pair (p, q) of prime ideals of A such that q ⊂ p (No. 2, Proposition 5).

#### Remark 5 {#ac-viii-s1-n3-rem-5 .statement}

We shall see in § 2, No. 4, that every finitely generated algebra over a field is a catenary ring. There exist noetherian local rings which are not catenary (p. 83, Exercise 16).

### 4. Dimension of a finitely generated module

#### Definition 8 {#ac-viii-s1-def-8 .statement}

Let A be a ring and M a finitely generated A-module. The Krull dimension (or simply dimension $^1$) of the A-module M is the Krull dimension of the support of M (II, § 4, No. 4, Definition 5); it is denoted by $\dim_A(M)$ (or $\dim(M)$ if there is no ambiguity).

The support of the A-module A is Spec(A); the dimension of the A-module A is therefore equal to the dimension of the ring A.

Let M be a finitely generated A-module and α its annihilator; one has

$$
\operatorname{Supp}(M) = V(\alpha) = \operatorname{Supp}(A/\alpha)
$$

(II, § 4, n° 4, prop. 17). Hence the dimension of the A-module M, the dimension of the A-module A/α, the dimension of the ring A/α and the dimension of the (A/α)-module M all coincide; it is the least upper bound of the set of lengths of chains $p_0 \subset ... \subset p_n$ of prime ideals of A such that $\alpha \subset p_0$. By prop. 6, c) of n° 3, the dimension of M is also the least upper bound of the dimensions of the rings (or of the A-modules) A/p, where p ranges over the set of prime ideals of A, minimal among those which contain α.

#### Remark 1 {#ac-viii-s1-n4-rem-1 .statement}

Let A be a noetherian ring and M a finitely generated A-module. It is equivalent to say that $\dim_A(M) \leq 0$, or that the elements of Supp(M) are maximal ideals of A, or that M is of finite length (IV, § 2, n° 5, prop. 7).

#### Remark 2 {#ac-viii-s1-n4-rem-2 .statement}

If M is a finitely generated module over a noetherian ring A, $\dim_A(M)$ is the least upper bound of the numbers $\dim(A/p)$, where p ranges over the set $\operatorname{Ass}_A(M)$ of prime ideals of A associated with M (IV, § 1, n° 4, th. 2).

1 If A is a field, the Krull dimension of M is $\leq 0$. Care must be taken not to confuse the Krull dimension of M with the dimension (or rank) of the vector space M over the field A (A, II, p. 97, déf. 1).

#### Proposition 9 {#ac-viii-s1-prop-9 .statement}

Let $A$ be a ring and $M$ a finitely generated $A$-module.

a) For every $p \in \mathrm{Supp}(M)$, one has $\dim_{A_p}(M_p) = \mathrm{codim}(V(p), \mathrm{Supp}(M))$.

b) $\dim_A(M)$ is the least upper bound of the $\dim_{A_p}(M_p)$, where $p$ ranges over $\mathrm{Spec}(A)$ (resp. where $p$ ranges over the set of maximal ideals of $A$ belonging to $\mathrm{Supp}(M)$).

c) Let $M'$ be a finitely generated submodule of $M$; then

$$
\dim_A(M) = \sup(\dim_A(M'), \dim_A(M/M')) .
$$

a) Let $a$ be the annihilator of $M$; then the annihilator of the $A_p$-module $M_p$ is $aA_p$ (II, § 2, n° 4, formule (9)), whence $\dim_{A_p}(M_p) = \dim(A_p/aA_p)$. One concludes by prop. 7, b) of n° 3.

b) This follows at once from a) and from the fact that $\dim_{A_p}(M_p) = -\infty$ if $p$ does not belong to $\mathrm{Supp}(M)$.

c) One has $\mathrm{Supp}(M) = \mathrm{Supp}(M') \cup \mathrm{Supp}(M/M')$ (II, § 4, n° 4, prop. 16), and one applies prop. 1 of n° 1.

#### Remark 3 {#ac-viii-s1-n4-rem-3 .statement}

Under the conditions of prop. 9, c), one has $\mathrm{codim}(\mathrm{Supp}(M), \mathrm{Spec}(A)) = \inf(\mathrm{codim}(\mathrm{Supp}(M'), \mathrm{Spec}(A)), \mathrm{codim}(\mathrm{Supp}(M/M'), \mathrm{Spec}(A)))$. This follows from the formula $\mathrm{Supp}(M) = \mathrm{Supp}(M') \cup \mathrm{Supp}(M/M')$ and from remark 4 of n° 2.

### 5. Cycles Associated with a Module

In this number, $A$ denotes a noetherian ring.

Let $Z(A)$ be the free $\mathbf{Z}$-module with basis the set of irreducible closed subsets of $\mathrm{Spec}(A)$; for every irreducible closed subset $Y$ of $\mathrm{Spec}(A)$, let $[Y]$ denote the corresponding element of $Z(A)$. The elements of $Z(A)$ are sometimes called cycles.

Let $M$ be a finitely generated $A$-module. For every prime ideal $p$ of $A$ which is a minimal element of $\mathrm{Supp}(M)$, one has $0 < \mathrm{long}_{A_p}(M_p) < \infty$ (IV, § 2, n° 5, cor. 2 à la prop. 7 and § 1, n° 4, th. 2); one sets

$$
z(M) = \sum_p \mathrm{long}_{A_p}(M_p).[V(p)] ,
$$

where $p$ ranges over the finite set of minimal prime ideals of $\mathrm{Supp}(M)$.

#### Remark {#ac-viii-s1-n5-rem-1 .statement}

For every $p \in \mathrm{Spec}(A)$, one has $z(A/p) = [V(p)]$. More generally, let $M$ be a finitely generated $A$-module, and let $(M_i)_{0 \leq i \leq n}$ be a composition sequence of $M$ such that for $0 \leq i \leq n-1$, the module $M_i/M_{i+1}$ is isomorphic to $A/p_i$, where $p_i$ is a prime ideal of $A$ (cf. IV, § 1, No. 4, Theorem 1); then one has $z(M) = \sum_{i \in J} [V(p_i)]$, where $J$ is the subset of $I$ consisting of the $i$ such that $p_i$ is a minimal element of $\{ p_0, ..., p_{n-1} \}$ (IV, § 1, No. 4, Theorem 2 and § 2, No. 5, Remark 1).

For every integer $d$, let us denote by $Z_{\leq d}$ (resp. $Z_d$, resp. $Z^{>d}$, resp. $Z^d$) the $\mathbf{Z}$-submodule of $Z(A)$ generated by the elements $[V(p)]$ where $p$ is a prime ideal of $A$ such that $\dim(A/p) \leq d$ (resp. $\dim(A/p) = d$, resp. $\mathrm{ht}(p) \geq d$, resp. $\mathrm{ht}(p) = d$). The elements of $Z_d$ (resp. $Z^d$) are called cycles of dimension $d$ (resp. of codimension $d$). One obviously has
$$
Z_{\leq d} = Z_{\leq d-1} \oplus Z_d,\quad Z^{>d} = Z^{>d+1} \oplus Z^d.
$$
Let moreover $C$ be the set of classes of finitely generated $A$-modules (A, VIII, § 3, No. 5), and for each integer $d$, let $C_{\leq d}$ (resp. $C^{>d}$) be the subset of $C$ consisting of the classes of finitely generated $A$-modules of dimension $\leq d$ (resp. whose support is of codimension $\geq d$ in $\mathrm{Spec}(A)$).

#### Lemma 1 {#ac-viii-s1-lem-1 .statement}

*Let $M$ be a finitely generated $A$-module and $d$ an integer.*
  *a*) *In order that $M$ be of type $C_{\leq d}$, it is necessary and sufficient that $z(M) \in Z_{\leq d}$; the projection $z_d(M)$ of $z(M)$ on $Z_d$ parallel to $Z_{\leq d-1}$ is then given by*
$$
z_d(M) = \sum_{\dim(A/p) = d} \mathrm{long}_{A_p}(M_p).[V(p)].
$$
  *b*) *In order that $M$ be of type $C^{>d}$, it is necessary and sufficient that $z(M) \in Z^{>d}$; the projection $z^d(M)$ of $z(M)$ on $Z^d$ parallel to $Z^{>d+1}$ is then given by*
$$
z^d(M) = \sum_{\mathrm{ht}(p) = d} \mathrm{long}_{A_p}(M_p).[V(p)].
$$

In order that $M$ be of type $C_{\leq d}$, that is to say of dimension $\leq d$, it is necessary and sufficient that for every minimal prime ideal $p$ of $\mathrm{Supp}(M)$, one have $\dim(A/p) \leq d$, which means that $z(M) \in Z_{\leq d}$. Suppose that one has $\dim(M) \leq d$, and let $p \in \mathrm{Spec}(A)$ be such that $\dim(A/p) = d$; then either $p \notin \mathrm{Supp}(M)$ and hence $M_p = 0$, or else $p \in \mathrm{Supp}(M)$, and $p$ is a minimal element of $\mathrm{Supp}(M)$; in both cases the coefficient of $[V(p)]$ in $z(M)$ is $\mathrm{long}_{A_p}(M_p)$, whence *a)*. Part *b)* is proved analogously; it should be noted that a finitely generated module $M$ is of type $C^{>d}$ if and only if one has $M_p = 0$ for every prime ideal $p$ of height $< d$.

According to Prop. 9, *c)* and Remark 3 of No. 4, the sets $C_{\leq d}$ and $C^{>d}$ are hereditary (A, VIII, § 10, No. 1, Def. 1), and one may consider the corresponding Grothendieck groups $K(C_{\leq d})$ and $K(C^{>d})$ (*loc. cit.*, No. 2); for every $A$-module $M$ of type $C_{\leq d}$ (resp. $C^{>d}$), let $[M]_{\leq d}$ (resp. $[M]^{>d}$) denote the associated element in $K(C_{\leq d})$ (resp. $K(C^{>d})$). By Lemma 1, the mappings $z_d$ and $z^d$ are additive; there therefore exist (*loc. cit.*, Prop. 3) homomorphisms
$$
\zeta_d : K(C_{\leq d}) \to Z_d,\quad \zeta^d : K(C^{>d}) \to Z^d
$$
such that $\zeta_d([M]_{\leq d}) = z_d(M)$ for every $A$-module $M$ of type $C_{\leq d}$ and $\zeta^d([N]^{>d}) = z^d(N)$ for every $A$-module $N$ of type $C^{>d}$. Moreover, since $C_{\leq d-1} \subset C_{\leq d}$ and $C^{>d+1} \subset C^{>d}$, one has canonical homomorphisms
$$
i_d : K(C_{\leq d-1}) \to K(C_{\leq d})\quad \text{and}\quad i^d : K(C^{>d+1}) \to K(C^{>d}).
$$
With these notations:

#### Proposition 10 {#ac-viii-s1-prop-10 .statement}

The sequences of $\mathbf{Z}$-modules and homomorphisms

$$
\begin{array}{cccccc}
K(\mathcal{C}_{\leq d-1}) & \xrightarrow{i_d} & K(\mathcal{C}_{\leq d}) & \xrightarrow{\zeta_d} & Z_d & \longrightarrow 0 \\
K(\mathcal{C}^{>d+1}) & \xrightarrow{i_d} & K(\mathcal{C}^{>d}) & \xrightarrow{\zeta_d} & Z^d & \longrightarrow 0
\end{array}
$$

are exact.

One has $\zeta_d \circ i_d = 0$ by Lemma 1. For every $p \in \mathrm{Spec}(A)$ such that $\dim(A/p) = d$, one has $\zeta_d([A/p]_{\leq d}) = z_d(A/p) = [V(p)]$, hence the homomorphism $\zeta_d$ is surjective. By IV, § 1, No. 4, Theorem 1, $K(\mathcal{C}_{\leq d})$ is generated by the $[A/p]_{\leq d}$, where $p \in \mathrm{Spec}(A)$ and $\dim(A/p) \leq d$; consequently, every element $\xi$ of $K(\mathcal{C}_{\leq d})$ can be written $\xi = i_d(\eta) + \sum_{i=1}^k n_i[A/p_i]_{\leq d}$, with $\eta \in K(\mathcal{C}_{\leq d-1})$, $n_i \in \mathbf{Z}$ and $\dim(A/p_i) = d$ for $1 \leq i \leq k$; one has $\zeta_d(\xi) = \sum_{i=1}^k n_i[V(p_i)]$ and consequently $\zeta_d(\xi) = 0$ implies $\xi = i_d(\eta) \in \mathrm{Im}(i_d)$, whence $\mathrm{Ker}(\zeta_d) = \mathrm{Im}(i_d)$.

One reasons analogously for the second sequence.

#### Example 1 {#ac-viii-s1-n5-exa-1 .statement}

Suppose A noetherian and integral. Then one has $Z^0 = \mathbf{Z}.[\mathrm{Spec}(A)]$; one has $\mathcal{C}^{>0} = \mathcal{C}$ and $z^0(M) = \mathrm{rg}(M).[Spec(A)]$. The modules of type $\mathcal{C}^{>1}$ are therefore the torsion modules.

#### Example 2 {#ac-viii-s1-n5-exa-2 .statement}

Suppose A noetherian and integrally closed. Then $Z^1$ is identified with the group $D(A)$ of divisors of A introduced in Chapter VII (§ 1, No. 3, Theorem 2, and No. 6, Theorem 3). The modules of type $\mathcal{C}^{>2}$ are the pseudo-null modules (VII, § 4, No. 4, Def. 2); if M is a torsion module of finite type, then $z^1(M) \in Z^1 = D(A)$ is the content $\chi(M)$ of M (VII, § 4, No. 5, Def. 4). Props. 10 and 11 of *loc. cit.* are therefore equivalent to the exactness of the sequence $K(\mathcal{C}^{>2}) \to K(\mathcal{C}^{>1}) \to Z^1 \to 0$.

#### Example 3 {#ac-viii-s1-n5-exa-3 .statement}

Modules of type $\mathcal{C}_{\leq 0}$ are the modules of dimension $\leq 0$, that is to say the modules of finite length (No. 4, Remark 1). We have $\mathrm{long}_A(M) = \varepsilon(z_0(M))$ for every finite-length A-module M, where $\varepsilon : Z_0 \to \mathbf{Z}$ associates to the linear combination $\sum_m n_m[V(m)]$ the integer $\sum_m n_m$ (IV, § 2, No. 5, corollary to Prop. 8).

#### Example 4 {#ac-viii-s1-n5-exa-4 .statement}

Suppose A is an integral domain and finite-dimensional. Put $d = \dim(A)$. Then we have $\mathcal{C}_{\leq d} = \mathcal{C}$, $Z_d = \mathbf{Z}.[\mathrm{Spec}(A)] = Z^0$, $z_d(M) = \mathrm{rg}(M).[Spec(A)] = z^0(M)$, and the modules of type $\mathcal{C}_{\leq d-1}$ are the torsion modules.

## EXERCISES {#ac-viii-s1-exercises}

See the [exercises for § 1](exercises/s1/).
